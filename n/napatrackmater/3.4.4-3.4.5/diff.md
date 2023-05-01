# Comparing `tmp/napatrackmater-3.4.4.tar.gz` & `tmp/napatrackmater-3.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-i5a0bxb9/napatrackmater-3.4.4.tar", last modified: Mon May  1 12:29:40 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-1ep8myp0/napatrackmater-3.4.5.tar", last modified: Mon May  1 12:55:43 2023, max compression
```

## Comparing `napatrackmater-3.4.4.tar` & `napatrackmater-3.4.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-01 12:29:40.559922 napatrackmater-3.4.4/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.4.4/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-05-01 12:29:40.553119 napatrackmater-3.4.4/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.4.4/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-01 12:29:40.278622 napatrackmater-3.4.4/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1241 2023-02-11 18:25:27.000000 napatrackmater-3.4.4/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      869 2023-02-26 10:31:22.000000 napatrackmater-3.4.4/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   110918 2023-05-01 11:22:42.000000 napatrackmater-3.4.4/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.4.4/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1611 2023-03-13 20:44:39.000000 napatrackmater-3.4.4/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13023 2023-04-08 11:44:13.000000 napatrackmater-3.4.4/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.4.4/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.4.4/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6013 2023-02-25 15:35:08.000000 napatrackmater-3.4.4/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-05-01 12:28:49.000000 napatrackmater-3.4.4/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-01 12:29:40.507879 napatrackmater-3.4.4/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-05-01 12:29:39.000000 napatrackmater-3.4.4/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-05-01 12:29:39.000000 napatrackmater-3.4.4/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-05-01 12:29:39.000000 napatrackmater-3.4.4/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-05-01 12:29:39.000000 napatrackmater-3.4.4/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       36 2023-05-01 12:29:39.000000 napatrackmater-3.4.4/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-05-01 12:29:39.000000 napatrackmater-3.4.4/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-05-01 12:29:40.561317 napatrackmater-3.4.4/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1292 2023-03-14 22:29:07.000000 napatrackmater-3.4.4/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-01 12:55:43.509961 napatrackmater-3.4.5/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.4.5/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-05-01 12:55:43.503965 napatrackmater-3.4.5/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.4.5/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-01 12:55:43.176624 napatrackmater-3.4.5/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1241 2023-02-11 18:25:27.000000 napatrackmater-3.4.5/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      869 2023-02-26 10:31:22.000000 napatrackmater-3.4.5/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   110921 2023-05-01 12:54:16.000000 napatrackmater-3.4.5/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.4.5/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1611 2023-03-13 20:44:39.000000 napatrackmater-3.4.5/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13023 2023-04-08 11:44:13.000000 napatrackmater-3.4.5/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.4.5/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.4.5/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6013 2023-02-25 15:35:08.000000 napatrackmater-3.4.5/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-05-01 12:55:23.000000 napatrackmater-3.4.5/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-05-01 12:55:43.458074 napatrackmater-3.4.5/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-05-01 12:55:42.000000 napatrackmater-3.4.5/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-05-01 12:55:42.000000 napatrackmater-3.4.5/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-05-01 12:55:42.000000 napatrackmater-3.4.5/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-05-01 12:55:42.000000 napatrackmater-3.4.5/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       36 2023-05-01 12:55:42.000000 napatrackmater-3.4.5/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-05-01 12:55:42.000000 napatrackmater-3.4.5/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-05-01 12:55:43.513018 napatrackmater-3.4.5/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1292 2023-03-14 22:29:07.000000 napatrackmater-3.4.5/setup.py
```

### Comparing `napatrackmater-3.4.4/LICENSE` & `napatrackmater-3.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.4/PKG-INFO` & `napatrackmater-3.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.4.4
+Version: 3.4.5
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.4.4/README.md` & `napatrackmater-3.4.5/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.4/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.4.5/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.4/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.4.5/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.4/napatrackmater/Trackmate.py` & `napatrackmater-3.4.5/napatrackmater/Trackmate.py`

 * *Files 0% similar despite different names*

```diff
@@ -3831,3103 +3831,3103 @@
 0000ef60: 2929 2020 2020 2020 0d0a 2020 2020 2020  ))      ..      
 0000ef70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ef80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ef90: 2020 6966 2073 706f 745f 736f 7572 6365    if spot_source
 0000efa0: 5f69 6420 6e6f 7420 696e 2073 656c 662e  _id not in self.
 0000efb0: 6368 616e 6e65 6c5f 756e 6971 7565 5f73  channel_unique_s
 0000efc0: 706f 745f 7072 6f70 6572 7469 6573 2e6b  pot_properties.k
-0000efd0: 6579 7328 2920 616e 6420 7370 6f74 5f74  eys() and spot_t
-0000efe0: 6172 6765 745f 6964 206e 6f74 2069 6e20  arget_id not in 
-0000eff0: 7365 6c66 2e63 6861 6e6e 656c 5f75 6e69  self.channel_uni
-0000f000: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-0000f010: 6965 732e 6b65 7973 2829 3a20 2020 2020  ies.keys():     
-0000f020: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000efd0: 6579 7328 2920 6f72 2073 706f 745f 7461  eys() or spot_ta
+0000efe0: 7267 6574 5f69 6420 6e6f 7420 696e 2073  rget_id not in s
+0000eff0: 656c 662e 6368 616e 6e65 6c5f 756e 6971  elf.channel_uniq
+0000f000: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+0000f010: 6573 2e6b 6579 7328 293a 2020 2020 200d  es.keys():     .
+0000f020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000f030: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f050: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f060: 636f 6e64 6368 696c 642e 7265 6d6f 7665  condchild.remove
-0000f070: 2845 6467 656f 626a 6563 7429 2020 0d0a  (Edgeobject)  ..
-0000f080: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f090: 2020 2020 2020 666f 7220 7061 7265 6e74        for parent
-0000f0a0: 2069 6e20 7365 6c66 2e78 6d6c 5f72 6f6f   in self.xml_roo
-0000f0b0: 742e 6669 6e64 616c 6c28 274d 6f64 656c  t.findall('Model
-0000f0c0: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
-0000f0d0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000f0e0: 2066 6972 7374 6368 696c 6420 696e 2070   firstchild in p
-0000f0f0: 6172 656e 742e 6669 6e64 616c 6c28 2746  arent.findall('F
-0000f100: 696c 7465 7265 6454 7261 636b 7327 293a  ilteredTracks'):
-0000f110: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f120: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000f130: 7220 7365 636f 6e64 6368 696c 6420 696e  r secondchild in
-0000f140: 2066 6972 7374 6368 696c 642e 6669 6e64   firstchild.find
-0000f150: 616c 6c28 2754 7261 636b 4944 2729 3a20  all('TrackID'): 
-0000f160: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f050: 2020 2020 2020 2020 2020 2020 2073 6563               sec
+0000f060: 6f6e 6463 6869 6c64 2e72 656d 6f76 6528  ondchild.remove(
+0000f070: 4564 6765 6f62 6a65 6374 2920 200d 0a0d  Edgeobject)  ...
+0000f080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f090: 2020 2020 2066 6f72 2070 6172 656e 7420       for parent 
+0000f0a0: 696e 2073 656c 662e 786d 6c5f 726f 6f74  in self.xml_root
+0000f0b0: 2e66 696e 6461 6c6c 2827 4d6f 6465 6c27  .findall('Model'
+0000f0c0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000f0d0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000f0e0: 6669 7273 7463 6869 6c64 2069 6e20 7061  firstchild in pa
+0000f0f0: 7265 6e74 2e66 696e 6461 6c6c 2827 4669  rent.findall('Fi
+0000f100: 6c74 6572 6564 5472 6163 6b73 2729 3a0d  lteredTracks'):.
+0000f110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f120: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000f130: 2073 6563 6f6e 6463 6869 6c64 2069 6e20   secondchild in 
+0000f140: 6669 7273 7463 6869 6c64 2e66 696e 6461  firstchild.finda
+0000f150: 6c6c 2827 5472 6163 6b49 4427 293a 200d  ll('TrackID'): .
+0000f160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000f170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f180: 2020 2020 2020 6669 6c74 6572 5f74 7261        filter_tra
-0000f190: 636b 5f69 6420 3d20 696e 7428 7365 636f  ck_id = int(seco
-0000f1a0: 6e64 6368 696c 642e 6765 7428 7365 6c66  ndchild.get(self
-0000f1b0: 2e74 7261 636b 6964 5f6b 6579 2929 2020  .trackid_key))  
-0000f1c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f180: 2020 2020 2066 696c 7465 725f 7472 6163       filter_trac
+0000f190: 6b5f 6964 203d 2069 6e74 2873 6563 6f6e  k_id = int(secon
+0000f1a0: 6463 6869 6c64 2e67 6574 2873 656c 662e  dchild.get(self.
+0000f1b0: 7472 6163 6b69 645f 6b65 7929 2920 200d  trackid_key))  .
+0000f1c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0000f1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f1e0: 2020 2020 2020 6966 2066 696c 7465 725f        if filter_
-0000f1f0: 7472 6163 6b5f 6964 206e 6f74 2069 6e20  track_id not in 
-0000f200: 6368 616e 6e65 6c5f 6669 6c74 6572 6564  channel_filtered
-0000f210: 5f74 7261 636b 733a 0d0a 2020 2020 2020  _tracks:..      
+0000f1e0: 2020 2020 2069 6620 6669 6c74 6572 5f74       if filter_t
+0000f1f0: 7261 636b 5f69 6420 6e6f 7420 696e 2063  rack_id not in c
+0000f200: 6861 6e6e 656c 5f66 696c 7465 7265 645f  hannel_filtered_
+0000f210: 7472 6163 6b73 3a0d 0a20 2020 2020 2020  tracks:..       
 0000f220: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000f230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f240: 2020 2020 2020 6669 7273 7463 6869 6c64        firstchild
-0000f250: 2e72 656d 6f76 6528 7365 636f 6e64 6368  .remove(secondch
-0000f260: 696c 6429 2020 2020 2020 2020 2020 2020  ild)            
-0000f270: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000f280: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0000f290: 2020 2020 2020 2073 656c 662e 786d 6c5f         self.xml_
-0000f2a0: 7472 6565 2e77 7269 7465 286f 732e 7061  tree.write(os.pa
-0000f2b0: 7468 2e6a 6f69 6e28 7365 6c66 2e63 6861  th.join(self.cha
-0000f2c0: 6e6e 656c 5f78 6d6c 5f70 6174 682c 2073  nnel_xml_path, s
-0000f2d0: 656c 662e 6368 616e 6e65 6c5f 786d 6c5f  elf.channel_xml_
-0000f2e0: 6e61 6d65 2929 200d 0a0d 0a20 2020 2064  name)) ....    d
-0000f2f0: 6566 205f 6765 745f 786d 6c5f 6461 7461  ef _get_xml_data
-0000f300: 2873 656c 6629 3a0d 0a0d 0a20 2020 2020  (self):....     
-0000f310: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
-0000f320: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000f330: 6620 7365 6c66 2e63 6861 6e6e 656c 5f73  f self.channel_s
-0000f340: 6567 5f69 6d61 6765 2069 7320 6e6f 7420  eg_image is not 
-0000f350: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-0000f360: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f370: 662e 6368 616e 6e65 6c5f 786d 6c5f 636f  f.channel_xml_co
-0000f380: 6e74 656e 7420 3d20 7365 6c66 2e78 6d6c  ntent = self.xml
-0000f390: 5f63 6f6e 7465 6e74 0d0a 2020 2020 2020  _content..      
-0000f3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3b0: 7365 6c66 2e78 6d6c 5f74 7265 6520 3d20  self.xml_tree = 
-0000f3c0: 6574 2e70 6172 7365 2873 656c 662e 786d  et.parse(self.xm
-0000f3d0: 6c5f 7061 7468 290d 0a20 2020 2020 2020  l_path)..       
-0000f3e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f3f0: 656c 662e 786d 6c5f 726f 6f74 203d 2073  elf.xml_root = s
-0000f400: 656c 662e 786d 6c5f 7472 6565 2e67 6574  elf.xml_tree.get
-0000f410: 726f 6f74 2829 0d0a 2020 2020 2020 2020  root()..        
-0000f420: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f430: 6c66 2e63 6861 6e6e 656c 5f78 6d6c 5f6e  lf.channel_xml_n
-0000f440: 616d 6520 3d20 2773 6563 6f6e 645f 6368  ame = 'second_ch
-0000f450: 616e 6e65 6c5f 2720 2b20 6f73 2e70 6174  annel_' + os.pat
-0000f460: 682e 7370 6c69 7465 7874 286f 732e 7061  h.splitext(os.pa
-0000f470: 7468 2e62 6173 656e 616d 6528 7365 6c66  th.basename(self
-0000f480: 2e78 6d6c 5f70 6174 6829 295b 305d 202b  .xml_path))[0] +
-0000f490: 2027 2e78 6d6c 270d 0a20 2020 2020 2020   '.xml'..       
-0000f4a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f4b0: 656c 662e 6368 616e 6e65 6c5f 786d 6c5f  elf.channel_xml_
-0000f4c0: 7061 7468 203d 206f 732e 7061 7468 2e64  path = os.path.d
-0000f4d0: 6972 6e61 6d65 2873 656c 662e 786d 6c5f  irname(self.xml_
-0000f4e0: 7061 7468 290d 0a20 2020 2020 2020 2020  path)..         
-0000f4f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f500: 662e 5f63 7265 6174 655f 6368 616e 6e65  f._create_channe
-0000f510: 6c5f 7472 6565 2829 0d0a 2020 2020 2020  l_tree()..      
-0000f520: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000f530: 662e 636c 7573 7465 725f 6d6f 6465 6c20  f.cluster_model 
-0000f540: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
-0000f550: 7365 6c66 2e73 6567 5f69 6d61 6765 2069  self.seg_image i
-0000f560: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+0000f240: 2020 2020 2066 6972 7374 6368 696c 642e       firstchild.
+0000f250: 7265 6d6f 7665 2873 6563 6f6e 6463 6869  remove(secondchi
+0000f260: 6c64 2920 2020 2020 2020 2020 2020 2020  ld)             
+0000f270: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000f280: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f290: 2020 2020 2020 7365 6c66 2e78 6d6c 5f74        self.xml_t
+0000f2a0: 7265 652e 7772 6974 6528 6f73 2e70 6174  ree.write(os.pat
+0000f2b0: 682e 6a6f 696e 2873 656c 662e 6368 616e  h.join(self.chan
+0000f2c0: 6e65 6c5f 786d 6c5f 7061 7468 2c20 7365  nel_xml_path, se
+0000f2d0: 6c66 2e63 6861 6e6e 656c 5f78 6d6c 5f6e  lf.channel_xml_n
+0000f2e0: 616d 6529 2920 0d0a 0d0a 2020 2020 6465  ame)) ....    de
+0000f2f0: 6620 5f67 6574 5f78 6d6c 5f64 6174 6128  f _get_xml_data(
+0000f300: 7365 6c66 293a 0d0a 0d0a 2020 2020 2020  self):....      
+0000f310: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
+0000f320: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000f330: 2073 656c 662e 6368 616e 6e65 6c5f 7365   self.channel_se
+0000f340: 675f 696d 6167 6520 6973 206e 6f74 204e  g_image is not N
+0000f350: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+0000f360: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f370: 2e63 6861 6e6e 656c 5f78 6d6c 5f63 6f6e  .channel_xml_con
+0000f380: 7465 6e74 203d 2073 656c 662e 786d 6c5f  tent = self.xml_
+0000f390: 636f 6e74 656e 740d 0a20 2020 2020 2020  content..       
+0000f3a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000f3b0: 656c 662e 786d 6c5f 7472 6565 203d 2065  elf.xml_tree = e
+0000f3c0: 742e 7061 7273 6528 7365 6c66 2e78 6d6c  t.parse(self.xml
+0000f3d0: 5f70 6174 6829 0d0a 2020 2020 2020 2020  _path)..        
+0000f3e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f3f0: 6c66 2e78 6d6c 5f72 6f6f 7420 3d20 7365  lf.xml_root = se
+0000f400: 6c66 2e78 6d6c 5f74 7265 652e 6765 7472  lf.xml_tree.getr
+0000f410: 6f6f 7428 290d 0a20 2020 2020 2020 2020  oot()..         
+0000f420: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f430: 662e 6368 616e 6e65 6c5f 786d 6c5f 6e61  f.channel_xml_na
+0000f440: 6d65 203d 2027 7365 636f 6e64 5f63 6861  me = 'second_cha
+0000f450: 6e6e 656c 5f27 202b 206f 732e 7061 7468  nnel_' + os.path
+0000f460: 2e73 706c 6974 6578 7428 6f73 2e70 6174  .splitext(os.pat
+0000f470: 682e 6261 7365 6e61 6d65 2873 656c 662e  h.basename(self.
+0000f480: 786d 6c5f 7061 7468 2929 5b30 5d20 2b20  xml_path))[0] + 
+0000f490: 272e 786d 6c27 0d0a 2020 2020 2020 2020  '.xml'..        
+0000f4a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f4b0: 6c66 2e63 6861 6e6e 656c 5f78 6d6c 5f70  lf.channel_xml_p
+0000f4c0: 6174 6820 3d20 6f73 2e70 6174 682e 6469  ath = os.path.di
+0000f4d0: 726e 616d 6528 7365 6c66 2e78 6d6c 5f70  rname(self.xml_p
+0000f4e0: 6174 6829 0d0a 2020 2020 2020 2020 2020  ath)..          
+0000f4f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f500: 2e5f 6372 6561 7465 5f63 6861 6e6e 656c  ._create_channel
+0000f510: 5f74 7265 6528 290d 0a20 2020 2020 2020  _tree()..       
+0000f520: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000f530: 2e63 6c75 7374 6572 5f6d 6f64 656c 2069  .cluster_model i
+0000f540: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2073  s not None and s
+0000f550: 656c 662e 7365 675f 696d 6167 6520 6973  elf.seg_image is
+0000f560: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
 0000f570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f580: 2020 2020 7365 6c66 2e6d 6173 7465 725f      self.master_
-0000f590: 786d 6c5f 636f 6e74 656e 7420 3d20 7365  xml_content = se
-0000f5a0: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 0d0a  lf.xml_content..
+0000f580: 2020 2073 656c 662e 6d61 7374 6572 5f78     self.master_x
+0000f590: 6d6c 5f63 6f6e 7465 6e74 203d 2073 656c  ml_content = sel
+0000f5a0: 662e 786d 6c5f 636f 6e74 656e 740d 0a20  f.xml_content.. 
 0000f5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5c0: 2020 2020 2020 2073 656c 662e 6d61 7374         self.mast
-0000f5d0: 6572 5f78 6d6c 5f74 7265 6520 3d20 6574  er_xml_tree = et
-0000f5e0: 2e70 6172 7365 2873 656c 662e 786d 6c5f  .parse(self.xml_
-0000f5f0: 7061 7468 290d 0a20 2020 2020 2020 2020  path)..         
-0000f600: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f610: 6c66 2e6d 6173 7465 725f 786d 6c5f 726f  lf.master_xml_ro
-0000f620: 6f74 203d 2073 656c 662e 6d61 7374 6572  ot = self.master
-0000f630: 5f78 6d6c 5f74 7265 652e 6765 7472 6f6f  _xml_tree.getroo
-0000f640: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
-0000f650: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f660: 2e6d 6173 7465 725f 786d 6c5f 6e61 6d65  .master_xml_name
-0000f670: 203d 2027 6d61 7374 6572 5f27 202b 2073   = 'master_' + s
-0000f680: 656c 662e 6d61 7374 6572 5f65 7874 7261  elf.master_extra
-0000f690: 5f6e 616d 6520 202b 206f 732e 7061 7468  _name  + os.path
-0000f6a0: 2e73 706c 6974 6578 7428 6f73 2e70 6174  .splitext(os.pat
-0000f6b0: 682e 6261 7365 6e61 6d65 2873 656c 662e  h.basename(self.
-0000f6c0: 786d 6c5f 7061 7468 2929 5b30 5d20 2b20  xml_path))[0] + 
-0000f6d0: 272e 786d 6c27 0d0a 2020 2020 2020 2020  '.xml'..        
-0000f6e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f6f0: 656c 662e 6d61 7374 6572 5f78 6d6c 5f70  elf.master_xml_p
-0000f700: 6174 6820 3d20 6f73 2e70 6174 682e 6469  ath = os.path.di
-0000f710: 726e 616d 6528 7365 6c66 2e78 6d6c 5f70  rname(self.xml_p
-0000f720: 6174 6829 2020 2020 2020 0d0a 2020 2020  ath)      ..    
+0000f5c0: 2020 2020 2020 7365 6c66 2e6d 6173 7465        self.maste
+0000f5d0: 725f 786d 6c5f 7472 6565 203d 2065 742e  r_xml_tree = et.
+0000f5e0: 7061 7273 6528 7365 6c66 2e78 6d6c 5f70  parse(self.xml_p
+0000f5f0: 6174 6829 0d0a 2020 2020 2020 2020 2020  ath)..          
+0000f600: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f610: 662e 6d61 7374 6572 5f78 6d6c 5f72 6f6f  f.master_xml_roo
+0000f620: 7420 3d20 7365 6c66 2e6d 6173 7465 725f  t = self.master_
+0000f630: 786d 6c5f 7472 6565 2e67 6574 726f 6f74  xml_tree.getroot
+0000f640: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+0000f650: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f660: 6d61 7374 6572 5f78 6d6c 5f6e 616d 6520  master_xml_name 
+0000f670: 3d20 276d 6173 7465 725f 2720 2b20 7365  = 'master_' + se
+0000f680: 6c66 2e6d 6173 7465 725f 6578 7472 615f  lf.master_extra_
+0000f690: 6e61 6d65 2020 2b20 6f73 2e70 6174 682e  name  + os.path.
+0000f6a0: 7370 6c69 7465 7874 286f 732e 7061 7468  splitext(os.path
+0000f6b0: 2e62 6173 656e 616d 6528 7365 6c66 2e78  .basename(self.x
+0000f6c0: 6d6c 5f70 6174 6829 295b 305d 202b 2027  ml_path))[0] + '
+0000f6d0: 2e78 6d6c 270d 0a20 2020 2020 2020 2020  .xml'..         
+0000f6e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f6f0: 6c66 2e6d 6173 7465 725f 786d 6c5f 7061  lf.master_xml_pa
+0000f700: 7468 203d 206f 732e 7061 7468 2e64 6972  th = os.path.dir
+0000f710: 6e61 6d65 2873 656c 662e 786d 6c5f 7061  name(self.xml_pa
+0000f720: 7468 2920 2020 2020 200d 0a20 2020 2020  th)      ..     
 0000f730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f740: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000f750: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-0000f760: 5f6f 626a 6563 7473 203d 207b 7d0d 0a20  _objects = {}.. 
-0000f770: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f780: 656c 662e 756e 6971 7565 5f70 726f 7065  elf.unique_prope
-0000f790: 7274 6965 7320 3d20 7b7d 0d0a 2020 2020  rties = {}..    
-0000f7a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f7b0: 2e41 6c6c 5472 6163 6b49 6473 203d 205b  .AllTrackIds = [
-0000f7c0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-0000f7d0: 2020 2073 656c 662e 4469 7669 6469 6e67     self.Dividing
-0000f7e0: 5472 6163 6b49 6473 203d 205b 5d0d 0a20  TrackIds = [].. 
-0000f7f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f800: 656c 662e 4e6f 726d 616c 5472 6163 6b49  elf.NormalTrackI
-0000f810: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
-0000f820: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-0000f830: 6c5f 7472 6163 6b5f 7072 6f70 6572 7469  l_track_properti
-0000f840: 6573 203d 205b 5d0d 0a20 2020 2020 2020  es = []..       
-0000f850: 2020 2020 2020 2020 2073 656c 662e 7370           self.sp
-0000f860: 6c69 745f 706f 696e 7473 5f74 696d 6573  lit_points_times
-0000f870: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-0000f880: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000f890: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000f8a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f8b0: 662e 416c 6c54 7261 636b 4964 732e 6170  f.AllTrackIds.ap
-0000f8c0: 7065 6e64 284e 6f6e 6529 0d0a 2020 2020  pend(None)..    
-0000f8d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f8e0: 2e44 6976 6964 696e 6754 7261 636b 4964  .DividingTrackId
-0000f8f0: 732e 6170 7065 6e64 284e 6f6e 6529 0d0a  s.append(None)..
-0000f900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f910: 7365 6c66 2e4e 6f72 6d61 6c54 7261 636b  self.NormalTrack
-0000f920: 4964 732e 6170 7065 6e64 284e 6f6e 6529  Ids.append(None)
-0000f930: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000f940: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000f950: 2020 2020 7365 6c66 2e41 6c6c 5472 6163      self.AllTrac
-0000f960: 6b49 6473 2e61 7070 656e 6428 7365 6c66  kIds.append(self
-0000f970: 2e54 7261 636b 6964 426f 7829 0d0a 2020  .TrackidBox)..  
-0000f980: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f990: 6c66 2e44 6976 6964 696e 6754 7261 636b  lf.DividingTrack
-0000f9a0: 4964 732e 6170 7065 6e64 2873 656c 662e  Ids.append(self.
-0000f9b0: 5472 6163 6b69 6442 6f78 290d 0a20 2020  TrackidBox)..   
-0000f9c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f9d0: 662e 4e6f 726d 616c 5472 6163 6b49 6473  f.NormalTrackIds
-0000f9e0: 2e61 7070 656e 6428 7365 6c66 2e54 7261  .append(self.Tra
-0000f9f0: 636b 6964 426f 7829 0d0a 2020 2020 2020  ckidBox)..      
-0000fa00: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000fa10: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000fa20: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000fa30: 6c66 2e53 706f 746f 626a 6563 7473 203d  lf.Spotobjects =
-0000fa40: 2073 656c 662e 786d 6c5f 636f 6e74 656e   self.xml_conten
-0000fa50: 742e 6669 6e64 2827 4d6f 6465 6c27 292e  t.find('Model').
-0000fa60: 6669 6e64 2827 416c 6c53 706f 7473 2729  find('AllSpots')
-0000fa70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fa80: 2020 2320 4578 7472 6163 7420 7468 6520    # Extract the 
-0000fa90: 7472 6163 6b73 2066 726f 6d20 786d 6c0d  tracks from xml.
-0000faa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fab0: 2073 656c 662e 7472 6163 6b73 203d 2073   self.tracks = s
-0000fac0: 656c 662e 786d 6c5f 636f 6e74 656e 742e  elf.xml_content.
-0000fad0: 6669 6e64 2822 4d6f 6465 6c22 292e 6669  find("Model").fi
-0000fae0: 6e64 2822 416c 6c54 7261 636b 7322 290d  nd("AllTracks").
-0000faf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fb00: 2073 656c 662e 7365 7474 696e 6773 203d   self.settings =
-0000fb10: 2073 656c 662e 786d 6c5f 636f 6e74 656e   self.xml_conten
-0000fb20: 742e 6669 6e64 2822 5365 7474 696e 6773  t.find("Settings
-0000fb30: 2229 2e66 696e 6428 2249 6d61 6765 4461  ").find("ImageDa
-0000fb40: 7461 2229 0d0a 2020 2020 2020 2020 2020  ta")..          
-0000fb50: 2020 2020 2020 7365 6c66 2e78 6361 6c69        self.xcali
-0000fb60: 6272 6174 696f 6e20 3d20 666c 6f61 7428  bration = float(
-0000fb70: 7365 6c66 2e73 6574 7469 6e67 732e 6765  self.settings.ge
-0000fb80: 7428 2270 6978 656c 7769 6474 6822 2929  t("pixelwidth"))
-0000fb90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fba0: 2020 7365 6c66 2e79 6361 6c69 6272 6174    self.ycalibrat
-0000fbb0: 696f 6e20 3d20 666c 6f61 7428 7365 6c66  ion = float(self
-0000fbc0: 2e73 6574 7469 6e67 732e 6765 7428 2270  .settings.get("p
-0000fbd0: 6978 656c 6865 6967 6874 2229 290d 0a20  ixelheight")).. 
-0000fbe0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000fbf0: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
-0000fc00: 203d 2066 6c6f 6174 2873 656c 662e 7365   = float(self.se
-0000fc10: 7474 696e 6773 2e67 6574 2822 766f 7865  ttings.get("voxe
-0000fc20: 6c64 6570 7468 2229 290d 0a20 2020 2020  ldepth"))..     
-0000fc30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000fc40: 7463 616c 6962 7261 7469 6f6e 203d 2069  tcalibration = i
-0000fc50: 6e74 2866 6c6f 6174 2873 656c 662e 7365  nt(float(self.se
-0000fc60: 7474 696e 6773 2e67 6574 2822 7469 6d65  ttings.get("time
-0000fc70: 696e 7465 7276 616c 2229 2929 0d0a 2020  interval")))..  
-0000fc80: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000fc90: 6c66 2e64 6574 6563 746f 7273 6574 7469  lf.detectorsetti
-0000fca0: 6e67 7320 3d20 7365 6c66 2e78 6d6c 5f63  ngs = self.xml_c
-0000fcb0: 6f6e 7465 6e74 2e66 696e 6428 2253 6574  ontent.find("Set
-0000fcc0: 7469 6e67 7322 292e 6669 6e64 2822 4465  tings").find("De
-0000fcd0: 7465 6374 6f72 5365 7474 696e 6773 2229  tectorSettings")
-0000fce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fcf0: 2020 7365 6c66 2e62 6173 6963 7365 7474    self.basicsett
-0000fd00: 696e 6773 203d 2073 656c 662e 786d 6c5f  ings = self.xml_
-0000fd10: 636f 6e74 656e 742e 6669 6e64 2822 5365  content.find("Se
-0000fd20: 7474 696e 6773 2229 2e66 696e 6428 2242  ttings").find("B
-0000fd30: 6173 6963 5365 7474 696e 6773 2229 0d0a  asicSettings")..
-0000fd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd50: 7365 6c66 2e64 6574 6563 746f 7263 6861  self.detectorcha
-0000fd60: 6e6e 656c 203d 2069 6e74 2866 6c6f 6174  nnel = int(float
-0000fd70: 2873 656c 662e 6465 7465 6374 6f72 7365  (self.detectorse
-0000fd80: 7474 696e 6773 2e67 6574 2822 5441 5247  ttings.get("TARG
-0000fd90: 4554 5f43 4841 4e4e 454c 2229 2929 0d0a  ET_CHANNEL")))..
-0000fda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fdb0: 7365 6c66 2e74 7374 6172 7420 3d20 696e  self.tstart = in
-0000fdc0: 7428 666c 6f61 7428 7365 6c66 2e62 6173  t(float(self.bas
-0000fdd0: 6963 7365 7474 696e 6773 2e67 6574 2822  icsettings.get("
-0000fde0: 7473 7461 7274 2229 2929 0d0a 2020 2020  tstart")))..    
-0000fdf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fe00: 2e74 656e 6420 3d20 696e 7428 666c 6f61  .tend = int(floa
-0000fe10: 7428 7365 6c66 2e62 6173 6963 7365 7474  t(self.basicsett
-0000fe20: 696e 6773 2e67 6574 2822 7465 6e64 2229  ings.get("tend")
-0000fe30: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-0000fe40: 2020 2020 7365 6c66 2e5f 6765 745f 626f      self._get_bo
-0000fe50: 756e 6461 7279 5f70 6f69 6e74 7328 290d  undary_points().
-0000fe60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fe70: 2070 7269 6e74 2827 4974 6572 6174 696e   print('Iteratin
-0000fe80: 6720 6f76 6572 2073 706f 7473 2069 6e20  g over spots in 
-0000fe90: 6672 616d 6527 290d 0a20 2020 2020 2020  frame')..       
-0000fea0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-0000feb0: 756e 7420 3d20 300d 0a20 2020 2020 2020  unt = 0..       
-0000fec0: 2020 2020 2020 2020 2066 7574 7572 6573           futures
-0000fed0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-0000fee0: 2020 2020 2020 2020 2077 6974 6820 636f           with co
-0000fef0: 6e63 7572 7265 6e74 2e66 7574 7572 6573  ncurrent.futures
-0000ff00: 2e54 6872 6561 6450 6f6f 6c45 7865 6375  .ThreadPoolExecu
-0000ff10: 746f 7228 6d61 785f 776f 726b 6572 7320  tor(max_workers 
-0000ff20: 3d20 6f73 2e63 7075 5f63 6f75 6e74 2829  = os.cpu_count()
-0000ff30: 2920 6173 2065 7865 6375 746f 723a 0d0a  ) as executor:..
+0000f740: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000f750: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
+0000f760: 6f62 6a65 6374 7320 3d20 7b7d 0d0a 2020  objects = {}..  
+0000f770: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f780: 6c66 2e75 6e69 7175 655f 7072 6f70 6572  lf.unique_proper
+0000f790: 7469 6573 203d 207b 7d0d 0a20 2020 2020  ties = {}..     
+0000f7a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f7b0: 416c 6c54 7261 636b 4964 7320 3d20 5b5d  AllTrackIds = []
+0000f7c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f7d0: 2020 7365 6c66 2e44 6976 6964 696e 6754    self.DividingT
+0000f7e0: 7261 636b 4964 7320 3d20 5b5d 0d0a 2020  rackIds = []..  
+0000f7f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f800: 6c66 2e4e 6f72 6d61 6c54 7261 636b 4964  lf.NormalTrackId
+0000f810: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+0000f820: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+0000f830: 5f74 7261 636b 5f70 726f 7065 7274 6965  _track_propertie
+0000f840: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
+0000f850: 2020 2020 2020 2020 7365 6c66 2e73 706c          self.spl
+0000f860: 6974 5f70 6f69 6e74 735f 7469 6d65 7320  it_points_times 
+0000f870: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+0000f880: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000f890: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000f8a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f8b0: 2e41 6c6c 5472 6163 6b49 6473 2e61 7070  .AllTrackIds.app
+0000f8c0: 656e 6428 4e6f 6e65 290d 0a20 2020 2020  end(None)..     
+0000f8d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f8e0: 4469 7669 6469 6e67 5472 6163 6b49 6473  DividingTrackIds
+0000f8f0: 2e61 7070 656e 6428 4e6f 6e65 290d 0a20  .append(None).. 
+0000f900: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000f910: 656c 662e 4e6f 726d 616c 5472 6163 6b49  elf.NormalTrackI
+0000f920: 6473 2e61 7070 656e 6428 4e6f 6e65 290d  ds.append(None).
+0000f930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f940: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000f950: 2020 2073 656c 662e 416c 6c54 7261 636b     self.AllTrack
+0000f960: 4964 732e 6170 7065 6e64 2873 656c 662e  Ids.append(self.
+0000f970: 5472 6163 6b69 6442 6f78 290d 0a20 2020  TrackidBox)..   
+0000f980: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f990: 662e 4469 7669 6469 6e67 5472 6163 6b49  f.DividingTrackI
+0000f9a0: 6473 2e61 7070 656e 6428 7365 6c66 2e54  ds.append(self.T
+0000f9b0: 7261 636b 6964 426f 7829 0d0a 2020 2020  rackidBox)..    
+0000f9c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f9d0: 2e4e 6f72 6d61 6c54 7261 636b 4964 732e  .NormalTrackIds.
+0000f9e0: 6170 7065 6e64 2873 656c 662e 5472 6163  append(self.Trac
+0000f9f0: 6b69 6442 6f78 290d 0a20 2020 2020 2020  kidBox)..       
+0000fa00: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000fa10: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000fa20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000fa30: 662e 5370 6f74 6f62 6a65 6374 7320 3d20  f.Spotobjects = 
+0000fa40: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
+0000fa50: 2e66 696e 6428 274d 6f64 656c 2729 2e66  .find('Model').f
+0000fa60: 696e 6428 2741 6c6c 5370 6f74 7327 290d  ind('AllSpots').
+0000fa70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fa80: 2023 2045 7874 7261 6374 2074 6865 2074   # Extract the t
+0000fa90: 7261 636b 7320 6672 6f6d 2078 6d6c 0d0a  racks from xml..
+0000faa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fab0: 7365 6c66 2e74 7261 636b 7320 3d20 7365  self.tracks = se
+0000fac0: 6c66 2e78 6d6c 5f63 6f6e 7465 6e74 2e66  lf.xml_content.f
+0000fad0: 696e 6428 224d 6f64 656c 2229 2e66 696e  ind("Model").fin
+0000fae0: 6428 2241 6c6c 5472 6163 6b73 2229 0d0a  d("AllTracks")..
+0000faf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb00: 7365 6c66 2e73 6574 7469 6e67 7320 3d20  self.settings = 
+0000fb10: 7365 6c66 2e78 6d6c 5f63 6f6e 7465 6e74  self.xml_content
+0000fb20: 2e66 696e 6428 2253 6574 7469 6e67 7322  .find("Settings"
+0000fb30: 292e 6669 6e64 2822 496d 6167 6544 6174  ).find("ImageDat
+0000fb40: 6122 290d 0a20 2020 2020 2020 2020 2020  a")..           
+0000fb50: 2020 2020 2073 656c 662e 7863 616c 6962       self.xcalib
+0000fb60: 7261 7469 6f6e 203d 2066 6c6f 6174 2873  ration = float(s
+0000fb70: 656c 662e 7365 7474 696e 6773 2e67 6574  elf.settings.get
+0000fb80: 2822 7069 7865 6c77 6964 7468 2229 290d  ("pixelwidth")).
+0000fb90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fba0: 2073 656c 662e 7963 616c 6962 7261 7469   self.ycalibrati
+0000fbb0: 6f6e 203d 2066 6c6f 6174 2873 656c 662e  on = float(self.
+0000fbc0: 7365 7474 696e 6773 2e67 6574 2822 7069  settings.get("pi
+0000fbd0: 7865 6c68 6569 6768 7422 2929 0d0a 2020  xelheight"))..  
+0000fbe0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000fbf0: 6c66 2e7a 6361 6c69 6272 6174 696f 6e20  lf.zcalibration 
+0000fc00: 3d20 666c 6f61 7428 7365 6c66 2e73 6574  = float(self.set
+0000fc10: 7469 6e67 732e 6765 7428 2276 6f78 656c  tings.get("voxel
+0000fc20: 6465 7074 6822 2929 0d0a 2020 2020 2020  depth"))..      
+0000fc30: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+0000fc40: 6361 6c69 6272 6174 696f 6e20 3d20 696e  calibration = in
+0000fc50: 7428 666c 6f61 7428 7365 6c66 2e73 6574  t(float(self.set
+0000fc60: 7469 6e67 732e 6765 7428 2274 696d 6569  tings.get("timei
+0000fc70: 6e74 6572 7661 6c22 2929 290d 0a20 2020  nterval")))..   
+0000fc80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000fc90: 662e 6465 7465 6374 6f72 7365 7474 696e  f.detectorsettin
+0000fca0: 6773 203d 2073 656c 662e 786d 6c5f 636f  gs = self.xml_co
+0000fcb0: 6e74 656e 742e 6669 6e64 2822 5365 7474  ntent.find("Sett
+0000fcc0: 696e 6773 2229 2e66 696e 6428 2244 6574  ings").find("Det
+0000fcd0: 6563 746f 7253 6574 7469 6e67 7322 290d  ectorSettings").
+0000fce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fcf0: 2073 656c 662e 6261 7369 6373 6574 7469   self.basicsetti
+0000fd00: 6e67 7320 3d20 7365 6c66 2e78 6d6c 5f63  ngs = self.xml_c
+0000fd10: 6f6e 7465 6e74 2e66 696e 6428 2253 6574  ontent.find("Set
+0000fd20: 7469 6e67 7322 292e 6669 6e64 2822 4261  tings").find("Ba
+0000fd30: 7369 6353 6574 7469 6e67 7322 290d 0a20  sicSettings").. 
+0000fd40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000fd50: 656c 662e 6465 7465 6374 6f72 6368 616e  elf.detectorchan
+0000fd60: 6e65 6c20 3d20 696e 7428 666c 6f61 7428  nel = int(float(
+0000fd70: 7365 6c66 2e64 6574 6563 746f 7273 6574  self.detectorset
+0000fd80: 7469 6e67 732e 6765 7428 2254 4152 4745  tings.get("TARGE
+0000fd90: 545f 4348 414e 4e45 4c22 2929 290d 0a20  T_CHANNEL"))).. 
+0000fda0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000fdb0: 656c 662e 7473 7461 7274 203d 2069 6e74  elf.tstart = int
+0000fdc0: 2866 6c6f 6174 2873 656c 662e 6261 7369  (float(self.basi
+0000fdd0: 6373 6574 7469 6e67 732e 6765 7428 2274  csettings.get("t
+0000fde0: 7374 6172 7422 2929 290d 0a20 2020 2020  start")))..     
+0000fdf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000fe00: 7465 6e64 203d 2069 6e74 2866 6c6f 6174  tend = int(float
+0000fe10: 2873 656c 662e 6261 7369 6373 6574 7469  (self.basicsetti
+0000fe20: 6e67 732e 6765 7428 2274 656e 6422 2929  ngs.get("tend"))
+0000fe30: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000fe40: 2020 2073 656c 662e 5f67 6574 5f62 6f75     self._get_bou
+0000fe50: 6e64 6172 795f 706f 696e 7473 2829 0d0a  ndary_points()..
+0000fe60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe70: 7072 696e 7428 2749 7465 7261 7469 6e67  print('Iterating
+0000fe80: 206f 7665 7220 7370 6f74 7320 696e 2066   over spots in f
+0000fe90: 7261 6d65 2729 0d0a 2020 2020 2020 2020  rame')..        
+0000fea0: 2020 2020 2020 2020 7365 6c66 2e63 6f75          self.cou
+0000feb0: 6e74 203d 2030 0d0a 2020 2020 2020 2020  nt = 0..        
+0000fec0: 2020 2020 2020 2020 6675 7475 7265 7320          futures 
+0000fed0: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+0000fee0: 2020 2020 2020 2020 7769 7468 2063 6f6e          with con
+0000fef0: 6375 7272 656e 742e 6675 7475 7265 732e  current.futures.
+0000ff00: 5468 7265 6164 506f 6f6c 4578 6563 7574  ThreadPoolExecut
+0000ff10: 6f72 286d 6178 5f77 6f72 6b65 7273 203d  or(max_workers =
+0000ff20: 206f 732e 6370 755f 636f 756e 7428 2929   os.cpu_count())
+0000ff30: 2061 7320 6578 6563 7574 6f72 3a0d 0a20   as executor:.. 
 0000ff40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff50: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000ff60: 2020 2020 2020 2020 2020 666f 7220 6672            for fr
-0000ff70: 616d 6520 696e 2073 656c 662e 5370 6f74  ame in self.Spot
-0000ff80: 6f62 6a65 6374 732e 6669 6e64 616c 6c28  objects.findall(
-0000ff90: 2753 706f 7473 496e 4672 616d 6527 293a  'SpotsInFrame'):
-0000ffa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ffb0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000ffc0: 7574 7572 6573 2e61 7070 656e 6428 6578  utures.append(ex
-0000ffd0: 6563 7574 6f72 2e73 7562 6d69 7428 7365  ecutor.submit(se
-0000ffe0: 6c66 2e5f 7370 6f74 5f63 6f6d 7075 7465  lf._spot_compute
-0000fff0: 722c 2066 7261 6d65 2929 0d0a 2020 2020  r, frame))..    
-00010000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010010: 6966 2073 656c 662e 7072 6f67 7265 7373  if self.progress
-00010020: 5f62 6172 2069 7320 6e6f 7420 4e6f 6e65  _bar is not None
-00010030: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000ff50: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000ff60: 2020 2020 2020 2020 2066 6f72 2066 7261           for fra
+0000ff70: 6d65 2069 6e20 7365 6c66 2e53 706f 746f  me in self.Spoto
+0000ff80: 626a 6563 7473 2e66 696e 6461 6c6c 2827  bjects.findall('
+0000ff90: 5370 6f74 7349 6e46 7261 6d65 2729 3a0d  SpotsInFrame'):.
+0000ffa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ffb0: 2020 2020 2020 2020 2020 2020 2020 6675                fu
+0000ffc0: 7475 7265 732e 6170 7065 6e64 2865 7865  tures.append(exe
+0000ffd0: 6375 746f 722e 7375 626d 6974 2873 656c  cutor.submit(sel
+0000ffe0: 662e 5f73 706f 745f 636f 6d70 7574 6572  f._spot_computer
+0000fff0: 2c20 6672 616d 6529 290d 0a20 2020 2020  , frame))..     
+00010000: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00010010: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
+00010020: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
+00010030: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00010040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010050: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00010050: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
 00010060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010070: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-00010080: 726f 6772 6573 735f 6261 722e 6c61 6265  rogress_bar.labe
-00010090: 6c20 3d20 2243 6f6c 6c65 6374 696e 6720  l = "Collecting 
-000100a0: 5370 6f74 7322 0d0a 2020 2020 2020 2020  Spots"..        
+00010070: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+00010080: 6f67 7265 7373 5f62 6172 2e6c 6162 656c  ogress_bar.label
+00010090: 203d 2022 436f 6c6c 6563 7469 6e67 2053   = "Collecting S
+000100a0: 706f 7473 220d 0a20 2020 2020 2020 2020  pots"..         
 000100b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000100d0: 2e70 726f 6772 6573 735f 6261 722e 7261  .progress_bar.ra
-000100e0: 6e67 6520 3d20 280d 0a20 2020 2020 2020  nge = (..       
+000100c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000100d0: 7072 6f67 7265 7373 5f62 6172 2e72 616e  progress_bar.ran
+000100e0: 6765 203d 2028 0d0a 2020 2020 2020 2020  ge = (..        
 000100f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010110: 2030 2c0d 0a20 2020 2020 2020 2020 2020   0,..           
+00010110: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
 00010120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010130: 2020 2020 2020 2020 2020 2020 206c 656e               len
-00010140: 2866 7574 7572 6573 292c 0d0a 2020 2020  (futures),..    
+00010130: 2020 2020 2020 2020 2020 2020 6c65 6e28              len(
+00010140: 6675 7475 7265 7329 2c0d 0a20 2020 2020  futures),..     
 00010150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010170: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00010160: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00010170: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00010180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010190: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-000101a0: 7265 7373 5f62 6172 2e73 686f 7728 290d  ress_bar.show().
-000101b0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000101c0: 2020 2020 2020 2066 6f72 2072 2069 6e20         for r in 
-000101d0: 636f 6e63 7572 7265 6e74 2e66 7574 7572  concurrent.futur
-000101e0: 6573 2e61 735f 636f 6d70 6c65 7465 6428  es.as_completed(
-000101f0: 6675 7475 7265 7329 3a0d 0a20 2020 2020  futures):..     
+00010190: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
+000101a0: 6573 735f 6261 722e 7368 6f77 2829 0d0a  ess_bar.show()..
+000101b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000101c0: 2020 2020 2020 666f 7220 7220 696e 2063        for r in c
+000101d0: 6f6e 6375 7272 656e 742e 6675 7475 7265  oncurrent.future
+000101e0: 732e 6173 5f63 6f6d 706c 6574 6564 2866  s.as_completed(f
+000101f0: 7574 7572 6573 293a 0d0a 2020 2020 2020  utures):..      
 00010200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010210: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00010220: 656c 662e 636f 756e 7420 3d20 7365 6c66  elf.count = self
-00010230: 2e63 6f75 6e74 202b 2031 0d0a 2020 2020  .count + 1..    
+00010210: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010220: 6c66 2e63 6f75 6e74 203d 2073 656c 662e  lf.count = self.
+00010230: 636f 756e 7420 2b20 310d 0a20 2020 2020  count + 1..     
 00010240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010260: 6966 2073 656c 662e 7072 6f67 7265 7373  if self.progress
-00010270: 5f62 6172 2069 7320 6e6f 7420 4e6f 6e65  _bar is not None
-00010280: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00010250: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00010260: 6620 7365 6c66 2e70 726f 6772 6573 735f  f self.progress_
+00010270: 6261 7220 6973 206e 6f74 204e 6f6e 653a  bar is not None:
+00010280: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00010290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102a0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-000102b0: 6f67 7265 7373 5f62 6172 2e76 616c 7565  ogress_bar.value
-000102c0: 203d 2020 7365 6c66 2e63 6f75 6e74 0d0a   =  self.count..
+000102a0: 2020 2020 2020 2020 7365 6c66 2e70 726f          self.pro
+000102b0: 6772 6573 735f 6261 722e 7661 6c75 6520  gress_bar.value 
+000102c0: 3d20 2073 656c 662e 636f 756e 740d 0a20  =  self.count.. 
 000102d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000102e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102f0: 2020 2020 722e 7265 7375 6c74 2829 0d0a      r.result()..
-00010300: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010310: 2020 7072 696e 7428 6627 4974 6572 6174    print(f'Iterat
-00010320: 696e 6720 6f76 6572 2074 7261 636b 7320  ing over tracks 
-00010330: 7b6c 656e 2873 656c 662e 6669 6c74 6572  {len(self.filter
-00010340: 6564 5f74 7261 636b 5f69 6473 297d 2729  ed_track_ids)}')
-00010350: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00010360: 2020 2020 7365 6c66 2e63 6f75 6e74 203d      self.count =
-00010370: 2030 0d0a 2020 2020 2020 2020 2020 2020   0..            
-00010380: 2020 2020 6675 7475 7265 7320 3d20 5b5d      futures = []
-00010390: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000103a0: 2020 7769 7468 2063 6f6e 6375 7272 656e    with concurren
-000103b0: 742e 6675 7475 7265 732e 5468 7265 6164  t.futures.Thread
-000103c0: 506f 6f6c 4578 6563 7574 6f72 286d 6178  PoolExecutor(max
-000103d0: 5f77 6f72 6b65 7273 203d 206f 732e 6370  _workers = os.cp
-000103e0: 755f 636f 756e 7428 2929 2061 7320 6578  u_count()) as ex
-000103f0: 6563 7574 6f72 3a0d 0a20 2020 2020 2020  ecutor:..       
-00010400: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+000102f0: 2020 2072 2e72 6573 756c 7428 290d 0a0d     r.result()...
+00010300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010310: 2070 7269 6e74 2866 2749 7465 7261 7469   print(f'Iterati
+00010320: 6e67 206f 7665 7220 7472 6163 6b73 207b  ng over tracks {
+00010330: 6c65 6e28 7365 6c66 2e66 696c 7465 7265  len(self.filtere
+00010340: 645f 7472 6163 6b5f 6964 7329 7d27 2920  d_track_ids)}') 
+00010350: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00010360: 2020 2073 656c 662e 636f 756e 7420 3d20     self.count = 
+00010370: 300d 0a20 2020 2020 2020 2020 2020 2020  0..             
+00010380: 2020 2066 7574 7572 6573 203d 205b 5d0d     futures = [].
+00010390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000103a0: 2077 6974 6820 636f 6e63 7572 7265 6e74   with concurrent
+000103b0: 2e66 7574 7572 6573 2e54 6872 6561 6450  .futures.ThreadP
+000103c0: 6f6f 6c45 7865 6375 746f 7228 6d61 785f  oolExecutor(max_
+000103d0: 776f 726b 6572 7320 3d20 6f73 2e63 7075  workers = os.cpu
+000103e0: 5f63 6f75 6e74 2829 2920 6173 2065 7865  _count()) as exe
+000103f0: 6375 746f 723a 0d0a 2020 2020 2020 2020  cutor:..        
+00010400: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
 00010410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010420: 2020 2066 6f72 2074 7261 636b 2069 6e20     for track in 
-00010430: 7365 6c66 2e74 7261 636b 732e 6669 6e64  self.tracks.find
-00010440: 616c 6c28 2754 7261 636b 2729 3a0d 0a20  all('Track'):.. 
+00010420: 2020 666f 7220 7472 6163 6b20 696e 2073    for track in s
+00010430: 656c 662e 7472 6163 6b73 2e66 696e 6461  elf.tracks.finda
+00010440: 6c6c 2827 5472 6163 6b27 293a 0d0a 2020  ll('Track'):..  
 00010450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010460: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00010460: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
 00010470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010480: 2020 2020 2020 2020 2074 7261 636b 5f69           track_i
-00010490: 6420 3d20 696e 7428 7472 6163 6b2e 6765  d = int(track.ge
-000104a0: 7428 7365 6c66 2e74 7261 636b 6964 5f6b  t(self.trackid_k
-000104b0: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
+00010480: 2020 2020 2020 2020 7472 6163 6b5f 6964          track_id
+00010490: 203d 2069 6e74 2874 7261 636b 2e67 6574   = int(track.get
+000104a0: 2873 656c 662e 7472 6163 6b69 645f 6b65  (self.trackid_ke
+000104b0: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
 000104c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104d0: 2020 6966 2074 7261 636b 5f69 6420 696e    if track_id in
-000104e0: 2073 656c 662e 6669 6c74 6572 6564 5f74   self.filtered_t
-000104f0: 7261 636b 5f69 6473 3a0d 0a20 2020 2020  rack_ids:..     
+000104d0: 2069 6620 7472 6163 6b5f 6964 2069 6e20   if track_id in 
+000104e0: 7365 6c66 2e66 696c 7465 7265 645f 7472  self.filtered_tr
+000104f0: 6163 6b5f 6964 733a 0d0a 2020 2020 2020  ack_ids:..      
 00010500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010510: 2020 2020 2020 2020 2020 2020 2066 7574               fut
-00010520: 7572 6573 2e61 7070 656e 6428 6578 6563  ures.append(exec
-00010530: 7574 6f72 2e73 7562 6d69 7428 7365 6c66  utor.submit(self
-00010540: 2e5f 7472 6163 6b5f 636f 6d70 7574 6572  ._track_computer
-00010550: 2c20 7472 6163 6b2c 2074 7261 636b 5f69  , track, track_i
-00010560: 6429 290d 0a20 2020 2020 2020 2020 2020  d))..           
-00010570: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00010580: 2e70 726f 6772 6573 735f 6261 7220 6973  .progress_bar is
-00010590: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00010510: 2020 2020 2020 2020 2020 2020 6675 7475              futu
+00010520: 7265 732e 6170 7065 6e64 2865 7865 6375  res.append(execu
+00010530: 746f 722e 7375 626d 6974 2873 656c 662e  tor.submit(self.
+00010540: 5f74 7261 636b 5f63 6f6d 7075 7465 722c  _track_computer,
+00010550: 2074 7261 636b 2c20 7472 6163 6b5f 6964   track, track_id
+00010560: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00010570: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00010580: 7072 6f67 7265 7373 5f62 6172 2069 7320  progress_bar is 
+00010590: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
 000105a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105b0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+000105b0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
 000105c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000105d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105e0: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-000105f0: 5f62 6172 2e6c 6162 656c 203d 2022 436f  _bar.label = "Co
-00010600: 6c6c 6563 7469 6e67 2054 7261 636b 7322  llecting Tracks"
-00010610: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000105e0: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+000105f0: 6261 722e 6c61 6265 6c20 3d20 2243 6f6c  bar.label = "Col
+00010600: 6c65 6374 696e 6720 5472 6163 6b73 220d  lecting Tracks".
+00010610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00010620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010630: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-00010640: 6573 735f 6261 722e 7261 6e67 6520 3d20  ess_bar.range = 
-00010650: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00010630: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+00010640: 7373 5f62 6172 2e72 616e 6765 203d 2028  ss_bar.range = (
+00010650: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00010660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010670: 2020 2020 2020 2020 2020 2030 2c0d 0a20             0,.. 
+00010670: 2020 2020 2020 2020 2020 302c 0d0a 2020            0,..  
 00010680: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106a0: 2020 2020 2020 206c 656e 2873 656c 662e         len(self.
-000106b0: 6669 6c74 6572 6564 5f74 7261 636b 5f69  filtered_track_i
-000106c0: 6473 292c 0d0a 2020 2020 2020 2020 2020  ds),..          
+000106a0: 2020 2020 2020 6c65 6e28 7365 6c66 2e66        len(self.f
+000106b0: 696c 7465 7265 645f 7472 6163 6b5f 6964  iltered_track_id
+000106c0: 7329 2c0d 0a20 2020 2020 2020 2020 2020  s),..           
 000106d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106e0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+000106e0: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
 000106f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010710: 2073 656c 662e 7072 6f67 7265 7373 5f62   self.progress_b
-00010720: 6172 2e73 686f 7728 290d 0a0d 0a0d 0a20  ar.show()...... 
+00010710: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
+00010720: 722e 7368 6f77 2829 0d0a 0d0a 0d0a 2020  r.show()......  
 00010730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010740: 2020 2066 6f72 2072 2069 6e20 636f 6e63     for r in conc
-00010750: 7572 7265 6e74 2e66 7574 7572 6573 2e61  urrent.futures.a
-00010760: 735f 636f 6d70 6c65 7465 6428 6675 7475  s_completed(futu
-00010770: 7265 7329 3a0d 0a20 2020 2020 2020 2020  res):..         
+00010740: 2020 666f 7220 7220 696e 2063 6f6e 6375    for r in concu
+00010750: 7272 656e 742e 6675 7475 7265 732e 6173  rrent.futures.as
+00010760: 5f63 6f6d 706c 6574 6564 2866 7574 7572  _completed(futur
+00010770: 6573 293a 0d0a 2020 2020 2020 2020 2020  es):..          
 00010780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010790: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000107a0: 636f 756e 7420 3d20 7365 6c66 2e63 6f75  count = self.cou
-000107b0: 6e74 202b 2031 0d0a 2020 2020 2020 2020  nt + 1..        
+00010790: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+000107a0: 6f75 6e74 203d 2073 656c 662e 636f 756e  ount = self.coun
+000107b0: 7420 2b20 310d 0a20 2020 2020 2020 2020  t + 1..         
 000107c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107d0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-000107e0: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
-000107f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+000107d0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+000107e0: 6c66 2e70 726f 6772 6573 735f 6261 7220  lf.progress_bar 
+000107f0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
 00010800: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010820: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-00010830: 6573 735f 6261 722e 7661 6c75 6520 3d20  ess_bar.value = 
-00010840: 7365 6c66 2e63 6f75 6e74 0d0a 2020 2020  self.count..    
+00010820: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+00010830: 7373 5f62 6172 2e76 616c 7565 203d 2073  ss_bar.value = s
+00010840: 656c 662e 636f 756e 740d 0a20 2020 2020  elf.count..     
 00010850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010870: 722e 7265 7375 6c74 2829 0d0a 2020 2020  r.result()..    
-00010880: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00010890: 656c 662e 6368 616e 6e65 6c5f 7365 675f  elf.channel_seg_
-000108a0: 696d 6167 6520 6973 206e 6f74 204e 6f6e  image is not Non
-000108b0: 653a 2020 0d0a 2020 2020 2020 2020 2020  e:  ..          
-000108c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000108d0: 662e 5f63 7265 6174 655f 7365 636f 6e64  f._create_second
-000108e0: 5f63 6861 6e6e 656c 5f78 6d6c 2829 0d0a  _channel_xml()..
-000108f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010900: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00010910: 2020 2020 666f 7220 286b 2c76 2920 696e      for (k,v) in
-00010920: 2073 656c 662e 6772 6170 685f 7370 6c69   self.graph_spli
-00010930: 742e 6974 656d 7328 293a 0d0a 2020 2020  t.items():..    
+00010860: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00010870: 2e72 6573 756c 7428 290d 0a20 2020 2020  .result()..     
+00010880: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00010890: 6c66 2e63 6861 6e6e 656c 5f73 6567 5f69  lf.channel_seg_i
+000108a0: 6d61 6765 2069 7320 6e6f 7420 4e6f 6e65  mage is not None
+000108b0: 3a20 200d 0a20 2020 2020 2020 2020 2020  :  ..           
+000108c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000108d0: 2e5f 6372 6561 7465 5f73 6563 6f6e 645f  ._create_second_
+000108e0: 6368 616e 6e65 6c5f 786d 6c28 290d 0a20  channel_xml().. 
+000108f0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00010900: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00010910: 2020 2066 6f72 2028 6b2c 7629 2069 6e20     for (k,v) in 
+00010920: 7365 6c66 2e67 7261 7068 5f73 706c 6974  self.graph_split
+00010930: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
 00010940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010950: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00010950: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
 00010960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010970: 2020 2020 2064 6175 6768 7465 725f 7472       daughter_tr
-00010980: 6163 6b5f 6964 203d 2020 696e 7428 666c  ack_id =  int(fl
-00010990: 6f61 7428 7374 7228 7365 6c66 2e75 6e69  oat(str(self.uni
-000109a0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-000109b0: 6965 735b 696e 7428 666c 6f61 7428 6b29  ies[int(float(k)
-000109c0: 295d 5b73 656c 662e 756e 6971 7565 6964  )][self.uniqueid
-000109d0: 5f6b 6579 5d29 2929 0d0a 2020 2020 2020  _key])))..      
+00010970: 2020 2020 6461 7567 6874 6572 5f74 7261      daughter_tra
+00010980: 636b 5f69 6420 3d20 2069 6e74 2866 6c6f  ck_id =  int(flo
+00010990: 6174 2873 7472 2873 656c 662e 756e 6971  at(str(self.uniq
+000109a0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+000109b0: 6573 5b69 6e74 2866 6c6f 6174 286b 2929  es[int(float(k))
+000109c0: 5d5b 7365 6c66 2e75 6e69 7175 6569 645f  ][self.uniqueid_
+000109d0: 6b65 795d 2929 290d 0a20 2020 2020 2020  key])))..       
 000109e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109f0: 2020 2020 2020 7061 7265 6e74 5f74 7261        parent_tra
-00010a00: 636b 5f69 6420 3d20 696e 7428 666c 6f61  ck_id = int(floa
-00010a10: 7428 7374 7228 7365 6c66 2e75 6e69 7175  t(str(self.uniqu
-00010a20: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00010a30: 735b 696e 7428 666c 6f61 7428 7629 295d  s[int(float(v))]
-00010a40: 5b73 656c 662e 756e 6971 7565 6964 5f6b  [self.uniqueid_k
-00010a50: 6579 5d29 2929 0d0a 2020 2020 2020 2020  ey])))..        
+000109f0: 2020 2020 2070 6172 656e 745f 7472 6163       parent_trac
+00010a00: 6b5f 6964 203d 2069 6e74 2866 6c6f 6174  k_id = int(float
+00010a10: 2873 7472 2873 656c 662e 756e 6971 7565  (str(self.unique
+00010a20: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00010a30: 5b69 6e74 2866 6c6f 6174 2876 2929 5d5b  [int(float(v))][
+00010a40: 7365 6c66 2e75 6e69 7175 6569 645f 6b65  self.uniqueid_ke
+00010a50: 795d 2929 290d 0a20 2020 2020 2020 2020  y])))..         
 00010a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a70: 2020 2020 7365 6c66 2e67 7261 7068 5f74      self.graph_t
-00010a80: 7261 636b 735b 6461 7567 6874 6572 5f74  racks[daughter_t
-00010a90: 7261 636b 5f69 645d 203d 2070 6172 656e  rack_id] = paren
-00010aa0: 745f 7472 6163 6b5f 6964 0d0a 2020 2020  t_track_id..    
-00010ab0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010ac0: 2e5f 6765 745f 6174 7472 6962 7574 6573  ._get_attributes
-00010ad0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00010ae0: 2020 2020 6966 2073 656c 662e 636c 7573      if self.clus
-00010af0: 7465 725f 6d6f 6465 6c20 616e 6420 7365  ter_model and se
-00010b00: 6c66 2e73 6567 5f69 6d61 6765 2069 7320  lf.seg_image is 
-00010b10: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+00010a70: 2020 2073 656c 662e 6772 6170 685f 7472     self.graph_tr
+00010a80: 6163 6b73 5b64 6175 6768 7465 725f 7472  acks[daughter_tr
+00010a90: 6163 6b5f 6964 5d20 3d20 7061 7265 6e74  ack_id] = parent
+00010aa0: 5f74 7261 636b 5f69 640d 0a20 2020 2020  _track_id..     
+00010ab0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010ac0: 5f67 6574 5f61 7474 7269 6275 7465 7328  _get_attributes(
+00010ad0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00010ae0: 2020 2069 6620 7365 6c66 2e63 6c75 7374     if self.clust
+00010af0: 6572 5f6d 6f64 656c 2061 6e64 2073 656c  er_model and sel
+00010b00: 662e 7365 675f 696d 6167 6520 6973 206e  f.seg_image is n
+00010b10: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
 00010b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b30: 2020 7365 6c66 2e5f 6173 7369 676e 5f63    self._assign_c
-00010b40: 6c75 7374 6572 5f63 6c61 7373 2829 0d0a  luster_class()..
+00010b30: 2073 656c 662e 5f61 7373 6967 6e5f 636c   self._assign_cl
+00010b40: 7573 7465 725f 636c 6173 7328 290d 0a20  uster_class().. 
 00010b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b60: 2020 2020 2020 2073 656c 662e 5f63 7265         self._cre
-00010b70: 6174 655f 6d61 7374 6572 5f78 6d6c 2829  ate_master_xml()
-00010b80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00010b90: 2020 7365 6c66 2e63 6f75 6e74 203d 2030    self.count = 0
-00010ba0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00010bb0: 2020 2066 6f72 2074 7261 636b 5f69 6420     for track_id 
-00010bc0: 696e 2073 656c 662e 6669 6c74 6572 6564  in self.filtered
-00010bd0: 5f74 7261 636b 5f69 6473 3a0d 0a20 2020  _track_ids:..   
+00010b60: 2020 2020 2020 7365 6c66 2e5f 6372 6561        self._crea
+00010b70: 7465 5f6d 6173 7465 725f 786d 6c28 290d  te_master_xml().
+00010b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010b90: 2073 656c 662e 636f 756e 7420 3d20 3020   self.count = 0 
+00010ba0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010bb0: 2020 666f 7220 7472 6163 6b5f 6964 2069    for track_id i
+00010bc0: 6e20 7365 6c66 2e66 696c 7465 7265 645f  n self.filtered_
+00010bd0: 7472 6163 6b5f 6964 733a 0d0a 2020 2020  track_ids:..    
 00010be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c00: 2069 6620 7365 6c66 2e70 726f 6772 6573   if self.progres
-00010c10: 735f 6261 7220 6973 206e 6f74 204e 6f6e  s_bar is not Non
-00010c20: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00010c00: 6966 2073 656c 662e 7072 6f67 7265 7373  if self.progress
+00010c10: 5f62 6172 2069 7320 6e6f 7420 4e6f 6e65  _bar is not None
+00010c20: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
 00010c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010c50: 2e70 726f 6772 6573 735f 6261 722e 6c61  .progress_bar.la
-00010c60: 6265 6c20 3d20 224a 7573 7420 6f6e 6520  bel = "Just one 
-00010c70: 6d6f 7265 2074 6869 6e67 220d 0a20 2020  more thing"..   
+00010c40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010c50: 7072 6f67 7265 7373 5f62 6172 2e6c 6162  progress_bar.lab
+00010c60: 656c 203d 2022 4a75 7374 206f 6e65 206d  el = "Just one m
+00010c70: 6f72 6520 7468 696e 6722 0d0a 2020 2020  ore thing"..    
 00010c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ca0: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
-00010cb0: 7373 5f62 6172 2e72 616e 6765 203d 2028  ss_bar.range = (
-00010cc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00010ca0: 2020 2020 7365 6c66 2e70 726f 6772 6573      self.progres
+00010cb0: 735f 6261 722e 7261 6e67 6520 3d20 280d  s_bar.range = (.
+00010cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00010cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010cf0: 2020 302c 0d0a 2020 2020 2020 2020 2020    0,..          
+00010cf0: 2030 2c0d 0a20 2020 2020 2020 2020 2020   0,..           
 00010d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d20: 2020 2020 2020 6c65 6e28 7365 6c66 2e66        len(self.f
-00010d30: 696c 7465 7265 645f 7472 6163 6b5f 6964  iltered_track_id
-00010d40: 7329 2c0d 0a20 2020 2020 2020 2020 2020  s),..           
+00010d20: 2020 2020 206c 656e 2873 656c 662e 6669       len(self.fi
+00010d30: 6c74 6572 6564 5f74 7261 636b 5f69 6473  ltered_track_ids
+00010d40: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
 00010d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d70: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+00010d70: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00010d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010da0: 2e70 726f 6772 6573 735f 6261 722e 7368  .progress_bar.sh
-00010db0: 6f77 2829 0d0a 2020 2020 2020 2020 2020  ow()..          
+00010d90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010da0: 7072 6f67 7265 7373 5f62 6172 2e73 686f  progress_bar.sho
+00010db0: 7728 290d 0a20 2020 2020 2020 2020 2020  w()..           
 00010dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010dd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00010de0: 6c66 2e63 6f75 6e74 203d 2073 656c 662e  lf.count = self.
-00010df0: 636f 756e 7420 2b20 310d 0a20 2020 2020  count + 1..     
+00010dd0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010de0: 662e 636f 756e 7420 3d20 7365 6c66 2e63  f.count = self.c
+00010df0: 6f75 6e74 202b 2031 0d0a 2020 2020 2020  ount + 1..      
 00010e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e20: 2020 2073 656c 662e 7072 6f67 7265 7373     self.progress
-00010e30: 5f62 6172 2e76 616c 7565 203d 2073 656c  _bar.value = sel
-00010e40: 662e 636f 756e 740d 0a20 2020 2020 2020  f.count..       
+00010e20: 2020 7365 6c66 2e70 726f 6772 6573 735f    self.progress_
+00010e30: 6261 722e 7661 6c75 6520 3d20 7365 6c66  bar.value = self
+00010e40: 2e63 6f75 6e74 0d0a 2020 2020 2020 2020  .count..        
 00010e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e60: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00010e70: 662e 5f66 696e 616c 5f74 7261 636b 7328  f._final_tracks(
-00010e80: 7472 6163 6b5f 6964 2920 0d0a 0d0a 2020  track_id) ....  
-00010e90: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00010ea0: 2073 656c 662e 666f 7572 6965 723a 0d0a   self.fourier:..
+00010e60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010e70: 2e5f 6669 6e61 6c5f 7472 6163 6b73 2874  ._final_tracks(t
+00010e80: 7261 636b 5f69 6429 200d 0a0d 0a20 2020  rack_id) ....   
+00010e90: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00010ea0: 7365 6c66 2e66 6f75 7269 6572 3a0d 0a20  self.fourier:.. 
 00010eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ec0: 2020 2070 7269 6e74 2827 636f 6d70 7574     print('comput
-00010ed0: 696e 6720 466f 7572 6965 7227 290d 0a20  ing Fourier').. 
+00010ec0: 2020 7072 696e 7428 2763 6f6d 7075 7469    print('computi
+00010ed0: 6e67 2046 6f75 7269 6572 2729 0d0a 2020  ng Fourier')..  
 00010ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ef0: 2020 7365 6c66 2e5f 636f 6d70 7574 655f    self._compute_
-00010f00: 7068 656e 6f74 7970 6573 2829 2020 2020  phenotypes()    
+00010ef0: 2073 656c 662e 5f63 6f6d 7075 7465 5f70   self._compute_p
+00010f00: 6865 6e6f 7479 7065 7328 2920 2020 2020  henotypes()     
 00010f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f20: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00010f30: 2020 2020 2020 7365 6c66 2e5f 7465 6d70        self._temp
-00010f40: 6f72 616c 5f70 6c6f 7473 5f74 7261 636b  oral_plots_track
-00010f50: 6d61 7465 2829 0d0a 2020 2020 2020 2020  mate()..        
-00010f60: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
-00010f70: 6465 6620 5f63 7265 6174 655f 6d61 7374  def _create_mast
-00010f80: 6572 5f78 6d6c 2873 656c 6629 3a0d 0a20  er_xml(self):.. 
-00010f90: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00010fa0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00010fb0: 2066 6f72 2053 706f 746f 626a 6563 7420   for Spotobject 
-00010fc0: 696e 2073 656c 662e 6d61 7374 6572 5f78  in self.master_x
-00010fd0: 6d6c 5f72 6f6f 742e 6974 6572 2827 5370  ml_root.iter('Sp
-00010fe0: 6f74 2729 3a0d 0a20 2020 2020 2020 2020  ot'):..         
+00010f20: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00010f30: 2020 2020 2073 656c 662e 5f74 656d 706f       self._tempo
+00010f40: 7261 6c5f 706c 6f74 735f 7472 6163 6b6d  ral_plots_trackm
+00010f50: 6174 6528 290d 0a20 2020 2020 2020 2020  ate()..         
+00010f60: 2020 2020 2020 200d 0a0d 0a20 2020 2064         ....    d
+00010f70: 6566 205f 6372 6561 7465 5f6d 6173 7465  ef _create_maste
+00010f80: 725f 786d 6c28 7365 6c66 293a 0d0a 2020  r_xml(self):..  
+00010f90: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00010fa0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00010fb0: 666f 7220 5370 6f74 6f62 6a65 6374 2069  for Spotobject i
+00010fc0: 6e20 7365 6c66 2e6d 6173 7465 725f 786d  n self.master_xm
+00010fd0: 6c5f 726f 6f74 2e69 7465 7228 2753 706f  l_root.iter('Spo
+00010fe0: 7427 293a 0d0a 2020 2020 2020 2020 2020  t'):..          
 00010ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011000: 2020 2020 2020 2063 656c 6c5f 6964 203d         cell_id =
-00011010: 2069 6e74 2853 706f 746f 626a 6563 742e   int(Spotobject.
-00011020: 6765 7428 7365 6c66 2e73 706f 7469 645f  get(self.spotid_
-00011030: 6b65 7929 290d 0a20 2020 2020 2020 2020  key))..         
+00011000: 2020 2020 2020 6365 6c6c 5f69 6420 3d20        cell_id = 
+00011010: 696e 7428 5370 6f74 6f62 6a65 6374 2e67  int(Spotobject.g
+00011020: 6574 2873 656c 662e 7370 6f74 6964 5f6b  et(self.spotid_k
+00011030: 6579 2929 0d0a 2020 2020 2020 2020 2020  ey))..          
 00011040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011050: 2020 2020 2020 2069 6620 6365 6c6c 5f69         if cell_i
-00011060: 6420 696e 2073 656c 662e 756e 6971 7565  d in self.unique
-00011070: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00011080: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
+00011050: 2020 2020 2020 6966 2063 656c 6c5f 6964        if cell_id
+00011060: 2069 6e20 7365 6c66 2e75 6e69 7175 655f   in self.unique_
+00011070: 7370 6f74 5f70 726f 7065 7274 6965 732e  spot_properties.
+00011080: 6b65 7973 2829 3a0d 0a20 2020 2020 2020  keys():..       
 00011090: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000110a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110b0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+000110b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 000110c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110d0: 2020 2020 2020 2020 2020 666f 7220 6b20            for k 
-000110e0: 696e 2073 656c 662e 756e 6971 7565 5f73  in self.unique_s
-000110f0: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
-00011100: 656c 6c5f 6964 5d2e 6b65 7973 2829 3a0d  ell_id].keys():.
-00011110: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000110d0: 2020 2020 2020 2020 2066 6f72 206b 2069           for k i
+000110e0: 6e20 7365 6c66 2e75 6e69 7175 655f 7370  n self.unique_sp
+000110f0: 6f74 5f70 726f 7065 7274 6965 735b 6365  ot_properties[ce
+00011100: 6c6c 5f69 645d 2e6b 6579 7328 293a 0d0a  ll_id].keys():..
+00011110: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00011120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011130: 2020 2020 2020 2020 2020 2020 2020 5370                Sp
-00011140: 6f74 6f62 6a65 6374 2e73 6574 286b 2c20  otobject.set(k, 
-00011150: 7374 7228 7365 6c66 2e75 6e69 7175 655f  str(self.unique_
-00011160: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00011170: 6365 6c6c 5f69 645d 5b6b 5d29 2920 2020  cell_id][k]))   
-00011180: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00011130: 2020 2020 2020 2020 2020 2020 2053 706f               Spo
+00011140: 746f 626a 6563 742e 7365 7428 6b2c 2073  tobject.set(k, s
+00011150: 7472 2873 656c 662e 756e 6971 7565 5f73  tr(self.unique_s
+00011160: 706f 745f 7072 6f70 6572 7469 6573 5b63  pot_properties[c
+00011170: 656c 6c5f 6964 5d5b 6b5d 2929 2020 200d  ell_id][k]))   .
+00011180: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
 00011190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111a0: 2020 2020 2020 2020 2020 0d0a 0d0a 2020            ....  
-000111b0: 2020 2020 2020 2020 2073 656c 662e 6d61           self.ma
-000111c0: 7374 6572 5f78 6d6c 5f74 7265 652e 7772  ster_xml_tree.wr
-000111d0: 6974 6528 6f73 2e70 6174 682e 6a6f 696e  ite(os.path.join
-000111e0: 2873 656c 662e 6d61 7374 6572 5f78 6d6c  (self.master_xml
-000111f0: 5f70 6174 682c 2073 656c 662e 6d61 7374  _path, self.mast
-00011200: 6572 5f78 6d6c 5f6e 616d 6529 290d 0a20  er_xml_name)).. 
-00011210: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+000111a0: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+000111b0: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
+000111c0: 7465 725f 786d 6c5f 7472 6565 2e77 7269  ter_xml_tree.wri
+000111d0: 7465 286f 732e 7061 7468 2e6a 6f69 6e28  te(os.path.join(
+000111e0: 7365 6c66 2e6d 6173 7465 725f 786d 6c5f  self.master_xml_
+000111f0: 7061 7468 2c20 7365 6c66 2e6d 6173 7465  path, self.maste
+00011200: 725f 786d 6c5f 6e61 6d65 2929 0d0a 2020  r_xml_name))..  
+00011210: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
 00011220: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011240: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00011240: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
 00011250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011260: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
-00011270: 2020 2020 6465 6620 5f61 7373 6967 6e5f      def _assign_
-00011280: 636c 7573 7465 725f 636c 6173 7328 7365  cluster_class(se
-00011290: 6c66 293a 0d0a 2020 2020 2020 2020 2020  lf):..          
-000112a0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000112b0: 2020 2020 2020 2073 656c 662e 6178 6573         self.axes
-000112c0: 203d 2073 656c 662e 6178 6573 2e72 6570   = self.axes.rep
-000112d0: 6c61 6365 2822 5422 2c20 2222 290d 0a20  lace("T", "").. 
+00011260: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
+00011270: 2020 2064 6566 205f 6173 7369 676e 5f63     def _assign_c
+00011280: 6c75 7374 6572 5f63 6c61 7373 2873 656c  luster_class(sel
+00011290: 6629 3a0d 0a20 2020 2020 2020 2020 2020  f):..           
+000112a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000112b0: 2020 2020 2020 7365 6c66 2e61 7865 7320        self.axes 
+000112c0: 3d20 7365 6c66 2e61 7865 732e 7265 706c  = self.axes.repl
+000112d0: 6163 6528 2254 222c 2022 2229 0d0a 2020  ace("T", "")..  
 000112e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112f0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00011300: 2020 2020 2020 2020 2066 6f72 2063 6f75           for cou
-00011310: 6e74 2c20 7469 6d65 5f6b 6579 2069 6e20  nt, time_key in 
-00011320: 656e 756d 6572 6174 6528 7365 6c66 2e5f  enumerate(self._
-00011330: 7469 6d65 645f 6365 6e74 726f 6964 2e6b  timed_centroid.k
-00011340: 6579 7328 2929 3a0d 0a20 2020 2020 2020  eys()):..       
+000112f0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00011300: 2020 2020 2020 2020 666f 7220 636f 756e          for coun
+00011310: 742c 2074 696d 655f 6b65 7920 696e 2065  t, time_key in e
+00011320: 6e75 6d65 7261 7465 2873 656c 662e 5f74  numerate(self._t
+00011330: 696d 6564 5f63 656e 7472 6f69 642e 6b65  imed_centroid.ke
+00011340: 7973 2829 293a 0d0a 2020 2020 2020 2020  ys()):..        
 00011350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011360: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00011360: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
 00011370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011380: 2074 7265 652c 2073 706f 745f 6365 6e74   tree, spot_cent
-00011390: 726f 6964 7320 3d20 7365 6c66 2e5f 7469  roids = self._ti
-000113a0: 6d65 645f 6365 6e74 726f 6964 5b74 696d  med_centroid[tim
-000113b0: 655f 6b65 795d 0d0a 2020 2020 2020 2020  e_key]..        
+00011380: 7472 6565 2c20 7370 6f74 5f63 656e 7472  tree, spot_centr
+00011390: 6f69 6473 203d 2073 656c 662e 5f74 696d  oids = self._tim
+000113a0: 6564 5f63 656e 7472 6f69 645b 7469 6d65  ed_centroid[time
+000113b0: 5f6b 6579 5d0d 0a20 2020 2020 2020 2020  _key]..         
 000113c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113d0: 2020 2069 6620 7365 6c66 2e70 726f 6772     if self.progr
-000113e0: 6573 735f 6261 7220 6973 206e 6f74 204e  ess_bar is not N
-000113f0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+000113d0: 2020 6966 2073 656c 662e 7072 6f67 7265    if self.progre
+000113e0: 7373 5f62 6172 2069 7320 6e6f 7420 4e6f  ss_bar is not No
+000113f0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
 00011400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011410: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
-00011420: 6573 735f 6261 722e 6c61 6265 6c20 3d20  ess_bar.label = 
-00011430: 2243 6f6d 7075 7469 6e67 2063 6c75 7374  "Computing clust
-00011440: 6572 696e 6720 636c 6173 7365 7322 0d0a  ering classes"..
+00011410: 2020 2020 2073 656c 662e 7072 6f67 7265       self.progre
+00011420: 7373 5f62 6172 2e6c 6162 656c 203d 2022  ss_bar.label = "
+00011430: 436f 6d70 7574 696e 6720 636c 7573 7465  Computing cluste
+00011440: 7269 6e67 2063 6c61 7373 6573 220d 0a20  ring classes".. 
 00011450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011470: 7365 6c66 2e70 726f 6772 6573 735f 6261  self.progress_ba
-00011480: 722e 7261 6e67 6520 3d20 280d 0a20 2020  r.range = (..   
+00011460: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011470: 656c 662e 7072 6f67 7265 7373 5f62 6172  elf.progress_bar
+00011480: 2e72 616e 6765 203d 2028 0d0a 2020 2020  .range = (..    
 00011490: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000114a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000114b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114c0: 2020 2020 2020 2020 2020 2020 2030 2c0d               0,.
-000114d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000114c0: 2020 2020 2020 2020 2020 2020 302c 0d0a              0,..
+000114d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000114e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000114f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011510: 206c 656e 2873 656c 662e 5f74 696d 6564   len(self._timed
-00011520: 5f63 656e 7472 6f69 642e 6b65 7973 2829  _centroid.keys()
-00011530: 2920 2b20 312c 0d0a 2020 2020 2020 2020  ) + 1,..        
+00011510: 6c65 6e28 7365 6c66 2e5f 7469 6d65 645f  len(self._timed_
+00011520: 6365 6e74 726f 6964 2e6b 6579 7328 2929  centroid.keys())
+00011530: 202b 2031 2c0d 0a20 2020 2020 2020 2020   + 1,..         
 00011540: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011550: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011570: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+00011570: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
 00011580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011590: 2020 2020 2020 2073 656c 662e 7072 6f67         self.prog
-000115a0: 7265 7373 5f62 6172 2e76 616c 7565 203d  ress_bar.value =
-000115b0: 2020 636f 756e 7420 0d0a 2020 2020 2020    count ..      
+00011590: 2020 2020 2020 7365 6c66 2e70 726f 6772        self.progr
+000115a0: 6573 735f 6261 722e 7661 6c75 6520 3d20  ess_bar.value = 
+000115b0: 2063 6f75 6e74 200d 0a20 2020 2020 2020   count ..       
 000115c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115d0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-000115e0: 726f 6772 6573 735f 6261 722e 7368 6f77  rogress_bar.show
-000115f0: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
+000115d0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+000115e0: 6f67 7265 7373 5f62 6172 2e73 686f 7728  ogress_bar.show(
+000115f0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
 00011600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011610: 2063 6c75 7374 6572 5f65 7661 6c20 3d20   cluster_eval = 
-00011620: 436c 7573 7465 7269 6e67 2873 656c 662e  Clustering(self.
-00011630: 7365 675f 696d 6167 655b 696e 7428 7469  seg_image[int(ti
-00011640: 6d65 5f6b 6579 292c 3a5d 2c20 2073 656c  me_key),:],  sel
-00011650: 662e 6178 6573 2c20 7365 6c66 2e6e 756d  f.axes, self.num
-00011660: 5f70 6f69 6e74 732c 2073 656c 662e 636c  _points, self.cl
-00011670: 7573 7465 725f 6d6f 6465 6c2c 206b 6579  uster_model, key
-00011680: 203d 2074 696d 655f 6b65 792c 2070 726f   = time_key, pro
-00011690: 6772 6573 735f 6261 723d 7365 6c66 2e70  gress_bar=self.p
-000116a0: 726f 6772 6573 735f 6261 722c 2062 6174  rogress_bar, bat
-000116b0: 6368 5f73 697a 6520 3d20 7365 6c66 2e62  ch_size = self.b
-000116c0: 6174 6368 5f73 697a 6529 2020 2020 2020  atch_size)      
-000116d0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000116e0: 2020 2020 2020 2020 2020 2020 2020 636c                cl
-000116f0: 7573 7465 725f 6576 616c 2e5f 6372 6561  uster_eval._crea
-00011700: 7465 5f63 6c75 7374 6572 5f6c 6162 656c  te_cluster_label
-00011710: 7328 290d 0a20 2020 2020 2020 2020 2020  s()..           
-00011720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011730: 7469 6d65 645f 636c 7573 7465 725f 6c61  timed_cluster_la
-00011740: 6265 6c20 3d20 636c 7573 7465 725f 6576  bel = cluster_ev
-00011750: 616c 2e74 696d 6564 5f63 6c75 7374 6572  al.timed_cluster
-00011760: 5f6c 6162 656c 200d 0a20 2020 2020 2020  _label ..       
+00011610: 636c 7573 7465 725f 6576 616c 203d 2043  cluster_eval = C
+00011620: 6c75 7374 6572 696e 6728 7365 6c66 2e73  lustering(self.s
+00011630: 6567 5f69 6d61 6765 5b69 6e74 2874 696d  eg_image[int(tim
+00011640: 655f 6b65 7929 2c3a 5d2c 2020 7365 6c66  e_key),:],  self
+00011650: 2e61 7865 732c 2073 656c 662e 6e75 6d5f  .axes, self.num_
+00011660: 706f 696e 7473 2c20 7365 6c66 2e63 6c75  points, self.clu
+00011670: 7374 6572 5f6d 6f64 656c 2c20 6b65 7920  ster_model, key 
+00011680: 3d20 7469 6d65 5f6b 6579 2c20 7072 6f67  = time_key, prog
+00011690: 7265 7373 5f62 6172 3d73 656c 662e 7072  ress_bar=self.pr
+000116a0: 6f67 7265 7373 5f62 6172 2c20 6261 7463  ogress_bar, batc
+000116b0: 685f 7369 7a65 203d 2073 656c 662e 6261  h_size = self.ba
+000116c0: 7463 685f 7369 7a65 2920 2020 2020 2020  tch_size)       
+000116d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000116e0: 2020 2020 2020 2020 2020 2020 2063 6c75               clu
+000116f0: 7374 6572 5f65 7661 6c2e 5f63 7265 6174  ster_eval._creat
+00011700: 655f 636c 7573 7465 725f 6c61 6265 6c73  e_cluster_labels
+00011710: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00011720: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00011730: 696d 6564 5f63 6c75 7374 6572 5f6c 6162  imed_cluster_lab
+00011740: 656c 203d 2063 6c75 7374 6572 5f65 7661  el = cluster_eva
+00011750: 6c2e 7469 6d65 645f 636c 7573 7465 725f  l.timed_cluster_
+00011760: 6c61 6265 6c20 0d0a 2020 2020 2020 2020  label ..        
 00011770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011780: 2020 2020 6f75 7470 7574 5f6c 6162 656c      output_label
-00011790: 732c 206f 7574 7075 745f 636c 7573 7465  s, output_cluste
-000117a0: 725f 7363 6f72 652c 206f 7574 7075 745f  r_score, output_
-000117b0: 636c 7573 7465 725f 636c 6173 732c 206f  cluster_class, o
-000117c0: 7574 7075 745f 636c 7573 7465 725f 6365  utput_cluster_ce
-000117d0: 6e74 726f 6964 2c20 6f75 7470 7574 5f63  ntroid, output_c
-000117e0: 6c6f 7564 5f65 6363 656e 7472 6963 6974  loud_eccentricit
-000117f0: 792c 206f 7574 7075 745f 6c61 7267 6573  y, output_larges
-00011800: 745f 6569 6765 6e76 6563 746f 722c 206f  t_eigenvector, o
-00011810: 7574 7075 745f 636c 6f75 645f 7375 7266  utput_cloud_surf
-00011820: 6163 655f 6172 6561 203d 2074 696d 6564  ace_area = timed
-00011830: 5f63 6c75 7374 6572 5f6c 6162 656c 5b74  _cluster_label[t
-00011840: 696d 655f 6b65 795d 0d0a 2020 2020 2020  ime_key]..      
+00011780: 2020 206f 7574 7075 745f 6c61 6265 6c73     output_labels
+00011790: 2c20 6f75 7470 7574 5f63 6c75 7374 6572  , output_cluster
+000117a0: 5f73 636f 7265 2c20 6f75 7470 7574 5f63  _score, output_c
+000117b0: 6c75 7374 6572 5f63 6c61 7373 2c20 6f75  luster_class, ou
+000117c0: 7470 7574 5f63 6c75 7374 6572 5f63 656e  tput_cluster_cen
+000117d0: 7472 6f69 642c 206f 7574 7075 745f 636c  troid, output_cl
+000117e0: 6f75 645f 6563 6365 6e74 7269 6369 7479  oud_eccentricity
+000117f0: 2c20 6f75 7470 7574 5f6c 6172 6765 7374  , output_largest
+00011800: 5f65 6967 656e 7665 6374 6f72 2c20 6f75  _eigenvector, ou
+00011810: 7470 7574 5f63 6c6f 7564 5f73 7572 6661  tput_cloud_surfa
+00011820: 6365 5f61 7265 6120 3d20 7469 6d65 645f  ce_area = timed_
+00011830: 636c 7573 7465 725f 6c61 6265 6c5b 7469  cluster_label[ti
+00011840: 6d65 5f6b 6579 5d0d 0a20 2020 2020 2020  me_key]..       
 00011850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011860: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+00011860: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
 00011870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011880: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00011890: 286c 656e 286f 7574 7075 745f 636c 7573  (len(output_clus
-000118a0: 7465 725f 6365 6e74 726f 6964 2929 3a0d  ter_centroid)):.
-000118b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011880: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00011890: 6c65 6e28 6f75 7470 7574 5f63 6c75 7374  len(output_clust
+000118a0: 6572 5f63 656e 7472 6f69 6429 293a 0d0a  er_centroid)):..
+000118b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000118c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118d0: 2020 2020 2063 656e 7472 6f69 6420 3d20       centroid = 
-000118e0: 6f75 7470 7574 5f63 6c75 7374 6572 5f63  output_cluster_c
-000118f0: 656e 7472 6f69 645b 695d 0d0a 2020 2020  entroid[i]..    
+000118d0: 2020 2020 6365 6e74 726f 6964 203d 206f      centroid = o
+000118e0: 7574 7075 745f 636c 7573 7465 725f 6365  utput_cluster_ce
+000118f0: 6e74 726f 6964 5b69 5d0d 0a20 2020 2020  ntroid[i]..     
 00011900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011920: 636c 7573 7465 725f 636c 6173 7320 3d20  cluster_class = 
-00011930: 6f75 7470 7574 5f63 6c75 7374 6572 5f63  output_cluster_c
-00011940: 6c61 7373 5b69 5d0d 0a20 2020 2020 2020  lass[i]..       
+00011910: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00011920: 6c75 7374 6572 5f63 6c61 7373 203d 206f  luster_class = o
+00011930: 7574 7075 745f 636c 7573 7465 725f 636c  utput_cluster_cl
+00011940: 6173 735b 695d 0d0a 2020 2020 2020 2020  ass[i]..        
 00011950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011960: 2020 2020 2020 2020 2020 2020 2063 6c75               clu
-00011970: 7374 6572 5f73 636f 7265 203d 206f 7574  ster_score = out
-00011980: 7075 745f 636c 7573 7465 725f 7363 6f72  put_cluster_scor
-00011990: 655b 695d 0d0a 2020 2020 2020 2020 2020  e[i]..          
+00011960: 2020 2020 2020 2020 2020 2020 636c 7573              clus
+00011970: 7465 725f 7363 6f72 6520 3d20 6f75 7470  ter_score = outp
+00011980: 7574 5f63 6c75 7374 6572 5f73 636f 7265  ut_cluster_score
+00011990: 5b69 5d0d 0a20 2020 2020 2020 2020 2020  [i]..           
 000119a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119b0: 2020 2020 2020 2020 2020 6563 6365 6e74            eccent
-000119c0: 7269 6369 7479 5f63 6f6d 705f 6669 7273  ricity_comp_firs
-000119d0: 7479 7a20 3d20 6f75 7470 7574 5f63 6c6f  tyz = output_clo
-000119e0: 7564 5f65 6363 656e 7472 6963 6974 795b  ud_eccentricity[
-000119f0: 695d 0d0a 2020 2020 2020 2020 2020 2020  i]..            
+000119b0: 2020 2020 2020 2020 2065 6363 656e 7472           eccentr
+000119c0: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
+000119d0: 797a 203d 206f 7574 7075 745f 636c 6f75  yz = output_clou
+000119e0: 645f 6563 6365 6e74 7269 6369 7479 5b69  d_eccentricity[i
+000119f0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
 00011a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a10: 2020 2020 2020 2020 6365 6c6c 5f61 7869          cell_axi
-00011a20: 7320 3d20 6f75 7470 7574 5f6c 6172 6765  s = output_large
-00011a30: 7374 5f65 6967 656e 7665 6374 6f72 5b69  st_eigenvector[i
-00011a40: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00011a10: 2020 2020 2020 2063 656c 6c5f 6178 6973         cell_axis
+00011a20: 203d 206f 7574 7075 745f 6c61 7267 6573   = output_larges
+00011a30: 745f 6569 6765 6e76 6563 746f 725b 695d  t_eigenvector[i]
+00011a40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00011a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a60: 2020 2020 2020 2073 7572 6661 6365 5f61         surface_a
-00011a70: 7265 6120 3d20 6f75 7470 7574 5f63 6c6f  rea = output_clo
-00011a80: 7564 5f73 7572 6661 6365 5f61 7265 615b  ud_surface_area[
-00011a90: 695d 0d0a 2020 2020 2020 2020 2020 2020  i]..            
+00011a60: 2020 2020 2020 7375 7266 6163 655f 6172        surface_ar
+00011a70: 6561 203d 206f 7574 7075 745f 636c 6f75  ea = output_clou
+00011a80: 645f 7375 7266 6163 655f 6172 6561 5b69  d_surface_area[i
+00011a90: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
 00011aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ab0: 2020 2020 2020 2020 6469 7374 2c20 696e          dist, in
-00011ac0: 6465 7820 3d20 7472 6565 2e71 7565 7279  dex = tree.query
-00011ad0: 2863 656e 7472 6f69 6429 0d0a 2020 2020  (centroid)..    
+00011ab0: 2020 2020 2020 2064 6973 742c 2069 6e64         dist, ind
+00011ac0: 6578 203d 2074 7265 652e 7175 6572 7928  ex = tree.query(
+00011ad0: 6365 6e74 726f 6964 290d 0a20 2020 2020  centroid)..     
 00011ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b00: 636c 6f73 6573 745f 6365 6e74 726f 6964  closest_centroid
-00011b10: 203d 2073 706f 745f 6365 6e74 726f 6964   = spot_centroid
-00011b20: 735b 696e 6465 785d 0d0a 2020 2020 2020  s[index]..      
+00011af0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00011b00: 6c6f 7365 7374 5f63 656e 7472 6f69 6420  losest_centroid 
+00011b10: 3d20 7370 6f74 5f63 656e 7472 6f69 6473  = spot_centroids
+00011b20: 5b69 6e64 6578 5d0d 0a20 2020 2020 2020  [index]..       
 00011b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b40: 2020 2020 2020 2020 2020 2020 2020 6672                fr
-00011b50: 616d 655f 7370 6f74 5f63 656e 7472 6f69  ame_spot_centroi
-00011b60: 6420 3d20 2869 6e74 2874 696d 655f 6b65  d = (int(time_ke
-00011b70: 7929 2c63 6c6f 7365 7374 5f63 656e 7472  y),closest_centr
-00011b80: 6f69 645b 305d 2c20 636c 6f73 6573 745f  oid[0], closest_
-00011b90: 6365 6e74 726f 6964 5b31 5d2c 2063 6c6f  centroid[1], clo
-00011ba0: 7365 7374 5f63 656e 7472 6f69 645b 325d  sest_centroid[2]
-00011bb0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00011b40: 2020 2020 2020 2020 2020 2020 2066 7261               fra
+00011b50: 6d65 5f73 706f 745f 6365 6e74 726f 6964  me_spot_centroid
+00011b60: 203d 2028 696e 7428 7469 6d65 5f6b 6579   = (int(time_key
+00011b70: 292c 636c 6f73 6573 745f 6365 6e74 726f  ),closest_centro
+00011b80: 6964 5b30 5d2c 2063 6c6f 7365 7374 5f63  id[0], closest_c
+00011b90: 656e 7472 6f69 645b 315d 2c20 636c 6f73  entroid[1], clos
+00011ba0: 6573 745f 6365 6e74 726f 6964 5b32 5d29  est_centroid[2])
+00011bb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00011bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011bd0: 2020 2020 2020 2063 6c6f 7365 7374 5f63         closest_c
-00011be0: 656c 6c5f 6964 203d 2073 656c 662e 756e  ell_id = self.un
-00011bf0: 6971 7565 5f73 706f 745f 6365 6e74 726f  ique_spot_centro
-00011c00: 6964 5b66 7261 6d65 5f73 706f 745f 6365  id[frame_spot_ce
-00011c10: 6e74 726f 6964 5d0d 0a20 2020 2020 2020  ntroid]..       
+00011bd0: 2020 2020 2020 636c 6f73 6573 745f 6365        closest_ce
+00011be0: 6c6c 5f69 6420 3d20 7365 6c66 2e75 6e69  ll_id = self.uni
+00011bf0: 7175 655f 7370 6f74 5f63 656e 7472 6f69  que_spot_centroi
+00011c00: 645b 6672 616d 655f 7370 6f74 5f63 656e  d[frame_spot_cen
+00011c10: 7472 6f69 645d 0d0a 2020 2020 2020 2020  troid]..        
 00011c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c30: 2020 2020 2020 2020 2020 2020 206d 6173               mas
-00011c40: 6b5f 7665 6374 6f72 203d 205b 2066 6c6f  k_vector = [ flo
-00011c50: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00011c60: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00011c70: 6e74 2863 6c6f 7365 7374 5f63 656c 6c5f  nt(closest_cell_
-00011c80: 6964 295d 5b73 656c 662e 6d61 736b 6365  id)][self.maskce
-00011c90: 6e74 726f 6964 5f78 5f6b 6579 5d29 2c20  ntroid_x_key]), 
-00011ca0: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-00011cb0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00011cc0: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
-00011cd0: 6c6c 5f69 6429 5d5b 7365 6c66 2e6d 6173  ll_id)][self.mas
-00011ce0: 6b63 656e 7472 6f69 645f 795f 6b65 795d  kcentroid_y_key]
-00011cf0: 292c 2066 6c6f 6174 2873 656c 662e 756e  ), float(self.un
-00011d00: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00011d10: 7469 6573 5b69 6e74 2863 6c6f 7365 7374  ties[int(closest
-00011d20: 5f63 656c 6c5f 6964 295d 5b73 656c 662e  _cell_id)][self.
-00011d30: 6d61 736b 6365 6e74 726f 6964 5f7a 5f6b  maskcentroid_z_k
-00011d40: 6579 5d29 205d 0d0a 2020 2020 2020 2020  ey]) ]..        
+00011c30: 2020 2020 2020 2020 2020 2020 6d61 736b              mask
+00011c40: 5f76 6563 746f 7220 3d20 5b20 666c 6f61  _vector = [ floa
+00011c50: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00011c60: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00011c70: 7428 636c 6f73 6573 745f 6365 6c6c 5f69  t(closest_cell_i
+00011c80: 6429 5d5b 7365 6c66 2e6d 6173 6b63 656e  d)][self.maskcen
+00011c90: 7472 6f69 645f 785f 6b65 795d 292c 2066  troid_x_key]), f
+00011ca0: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+00011cb0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00011cc0: 5b69 6e74 2863 6c6f 7365 7374 5f63 656c  [int(closest_cel
+00011cd0: 6c5f 6964 295d 5b73 656c 662e 6d61 736b  l_id)][self.mask
+00011ce0: 6365 6e74 726f 6964 5f79 5f6b 6579 5d29  centroid_y_key])
+00011cf0: 2c20 666c 6f61 7428 7365 6c66 2e75 6e69  , float(self.uni
+00011d00: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00011d10: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
+00011d20: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e6d  cell_id)][self.m
+00011d30: 6173 6b63 656e 7472 6f69 645f 7a5f 6b65  askcentroid_z_ke
+00011d40: 795d 2920 5d0d 0a20 2020 2020 2020 2020  y]) ]..         
 00011d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d60: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
-00011d70: 5f61 7869 735f 6d61 736b 203d 2061 6e67  _axis_mask = ang
-00011d80: 756c 6172 5f63 6861 6e67 6528 6365 6c6c  ular_change(cell
-00011d90: 5f61 7869 732c 206d 6173 6b5f 7665 6374  _axis, mask_vect
-00011da0: 6f72 290d 0a20 2020 2020 2020 2020 2020  or)..           
+00011d60: 2020 2020 2020 2020 2020 2063 656c 6c5f             cell_
+00011d70: 6178 6973 5f6d 6173 6b20 3d20 616e 6775  axis_mask = angu
+00011d80: 6c61 725f 6368 616e 6765 2863 656c 6c5f  lar_change(cell_
+00011d90: 6178 6973 2c20 6d61 736b 5f76 6563 746f  axis, mask_vecto
+00011da0: 7229 0d0a 2020 2020 2020 2020 2020 2020  r)..            
 00011db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011dc0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00011dc0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
 00011dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011de0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00011df0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00011e00: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00011e10: 6c6f 7365 7374 5f63 656c 6c5f 6964 295d  losest_cell_id)]
-00011e20: 2e75 7064 6174 6528 7b73 656c 662e 6365  .update({self.ce
-00011e30: 6c6c 6178 6973 5f6d 6173 6b5f 6b65 7920  llaxis_mask_key 
-00011e40: 3a20 6365 6c6c 5f61 7869 735f 6d61 736b  : cell_axis_mask
-00011e50: 7d29 0d0a 2020 2020 2020 2020 2020 2020  })..            
+00011de0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00011df0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00011e00: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
+00011e10: 6f73 6573 745f 6365 6c6c 5f69 6429 5d2e  osest_cell_id)].
+00011e20: 7570 6461 7465 287b 7365 6c66 2e63 656c  update({self.cel
+00011e30: 6c61 7869 735f 6d61 736b 5f6b 6579 203a  laxis_mask_key :
+00011e40: 2063 656c 6c5f 6178 6973 5f6d 6173 6b7d   cell_axis_mask}
+00011e50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00011e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e70: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00011e80: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00011e90: 6965 735b 696e 7428 636c 6f73 6573 745f  ies[int(closest_
-00011ea0: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
-00011eb0: 287b 7365 6c66 2e63 6c75 7374 6572 636c  ({self.clustercl
-00011ec0: 6173 735f 6b65 7920 3a20 636c 7573 7465  ass_key : cluste
-00011ed0: 725f 636c 6173 737d 290d 0a20 2020 2020  r_class})..     
+00011e70: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00011e80: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00011e90: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
+00011ea0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
+00011eb0: 7b73 656c 662e 636c 7573 7465 7263 6c61  {self.clustercla
+00011ec0: 7373 5f6b 6579 203a 2063 6c75 7374 6572  ss_key : cluster
+00011ed0: 5f63 6c61 7373 7d29 0d0a 2020 2020 2020  _class})..      
 00011ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ef0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00011f00: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00011f10: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00011f20: 6c6f 7365 7374 5f63 656c 6c5f 6964 295d  losest_cell_id)]
-00011f30: 2e75 7064 6174 6528 7b73 656c 662e 636c  .update({self.cl
-00011f40: 7573 7465 7273 636f 7265 5f6b 6579 203a  usterscore_key :
-00011f50: 2063 6c75 7374 6572 5f73 636f 7265 7d29   cluster_score})
-00011f60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011ef0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00011f00: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00011f10: 726f 7065 7274 6965 735b 696e 7428 636c  roperties[int(cl
+00011f20: 6f73 6573 745f 6365 6c6c 5f69 6429 5d2e  osest_cell_id)].
+00011f30: 7570 6461 7465 287b 7365 6c66 2e63 6c75  update({self.clu
+00011f40: 7374 6572 7363 6f72 655f 6b65 7920 3a20  sterscore_key : 
+00011f50: 636c 7573 7465 725f 7363 6f72 657d 290d  cluster_score}).
+00011f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00011f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f80: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00011f90: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00011fa0: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
-00011fb0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00011fc0: 7365 6c66 2e65 6363 656e 7472 6963 6974  self.eccentricit
-00011fd0: 795f 636f 6d70 5f66 6972 7374 6b65 7920  y_comp_firstkey 
-00011fe0: 3a20 6563 6365 6e74 7269 6369 7479 5f63  : eccentricity_c
-00011ff0: 6f6d 705f 6669 7273 7479 7a5b 305d 7d29  omp_firstyz[0]})
-00012000: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011f80: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00011f90: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00011fa0: 5b69 6e74 2863 6c6f 7365 7374 5f63 656c  [int(closest_cel
+00011fb0: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+00011fc0: 656c 662e 6563 6365 6e74 7269 6369 7479  elf.eccentricity
+00011fd0: 5f63 6f6d 705f 6669 7273 746b 6579 203a  _comp_firstkey :
+00011fe0: 2065 6363 656e 7472 6963 6974 795f 636f   eccentricity_co
+00011ff0: 6d70 5f66 6972 7374 797a 5b30 5d7d 290d  mp_firstyz[0]}).
+00012000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00012010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012020: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00012030: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00012040: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
-00012050: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00012060: 7365 6c66 2e65 6363 656e 7472 6963 6974  self.eccentricit
-00012070: 795f 636f 6d70 5f73 6563 6f6e 646b 6579  y_comp_secondkey
-00012080: 203a 2065 6363 656e 7472 6963 6974 795f   : eccentricity_
-00012090: 636f 6d70 5f66 6972 7374 797a 5b31 5d7d  comp_firstyz[1]}
-000120a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00012020: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+00012030: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00012040: 5b69 6e74 2863 6c6f 7365 7374 5f63 656c  [int(closest_cel
+00012050: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
+00012060: 656c 662e 6563 6365 6e74 7269 6369 7479  elf.eccentricity
+00012070: 5f63 6f6d 705f 7365 636f 6e64 6b65 7920  _comp_secondkey 
+00012080: 3a20 6563 6365 6e74 7269 6369 7479 5f63  : eccentricity_c
+00012090: 6f6d 705f 6669 7273 7479 7a5b 315d 7d29  omp_firstyz[1]})
+000120a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 000120b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120c0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
-000120d0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-000120e0: 6573 5b69 6e74 2863 6c6f 7365 7374 5f63  es[int(closest_c
-000120f0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-00012100: 7b73 656c 662e 7375 7266 6163 655f 6172  {self.surface_ar
-00012110: 6561 5f6b 6579 203a 2073 7572 6661 6365  ea_key : surface
-00012120: 5f61 7265 617d 290d 0a0d 0a20 2020 2020  _area})....     
+000120c0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+000120d0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+000120e0: 735b 696e 7428 636c 6f73 6573 745f 6365  s[int(closest_ce
+000120f0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00012100: 7365 6c66 2e73 7572 6661 6365 5f61 7265  self.surface_are
+00012110: 615f 6b65 7920 3a20 7375 7266 6163 655f  a_key : surface_
+00012120: 6172 6561 7d29 0d0a 0d0a 2020 2020 2020  area})....      
 00012130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012140: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00012150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012160: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00012170: 286b 2c76 2920 696e 2073 656c 662e 726f  (k,v) in self.ro
-00012180: 6f74 5f73 706f 7473 2e69 7465 6d73 2829  ot_spots.items()
-00012190: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00012140: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00012150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012160: 2020 2020 2020 2020 2020 2066 6f72 2028             for (
+00012170: 6b2c 7629 2069 6e20 7365 6c66 2e72 6f6f  k,v) in self.roo
+00012180: 745f 7370 6f74 732e 6974 656d 7328 293a  t_spots.items():
+00012190: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 000121a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121b0: 2020 2020 2073 656c 662e 726f 6f74 5f73       self.root_s
-000121c0: 706f 7473 5b6b 5d20 3d20 7365 6c66 2e75  pots[k] = self.u
-000121d0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-000121e0: 7274 6965 735b 6b5d 2020 2020 2020 2020  rties[k]        
-000121f0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00012200: 2020 200d 0a20 2020 2064 6566 205f 636f     ..    def _co
-00012210: 6d70 7574 655f 7068 656e 6f74 7970 6573  mpute_phenotypes
-00012220: 2873 656c 6629 3a0d 0a0d 0a20 2020 2020  (self):....     
-00012230: 2020 2020 2066 6f72 2028 6b2c 7629 2069       for (k,v) i
-00012240: 6e20 7365 6c66 2e75 6e69 7175 655f 7472  n self.unique_tr
-00012250: 6163 6b73 2e69 7465 6d73 2829 3a0d 0a20  acks.items():.. 
-00012260: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00012270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012280: 2074 7261 636b 5f69 6420 3d20 6b0d 0a20   track_id = k.. 
-00012290: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000122a0: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
-000122b0: 6573 203d 2073 656c 662e 756e 6971 7565  es = self.unique
-000122c0: 5f74 7261 636b 5f70 726f 7065 7274 6965  _track_propertie
-000122d0: 735b 6b5d 0d0a 2020 2020 2020 2020 2020  s[k]..          
-000122e0: 2020 2020 2020 7472 6163 6b73 203d 2073        tracks = s
-000122f0: 656c 662e 756e 6971 7565 5f74 7261 636b  elf.unique_track
-00012300: 735b 6b5d 0d0a 2020 2020 2020 2020 2020  s[k]..          
-00012310: 2020 2020 2020 5a20 3d20 7472 6163 6b73        Z = tracks
-00012320: 5b3a 2c32 5d0d 0a20 2020 2020 2020 2020  [:,2]..         
-00012330: 2020 2020 2020 2059 203d 2074 7261 636b         Y = track
-00012340: 735b 3a2c 335d 0d0a 2020 2020 2020 2020  s[:,3]..        
-00012350: 2020 2020 2020 2020 5820 3d20 7472 6163          X = trac
-00012360: 6b73 5b3a 2c34 5d0d 0a20 2020 2020 2020  ks[:,4]..       
-00012370: 2020 2020 2020 2020 2074 696d 6520 3d20           time = 
-00012380: 7472 6163 6b6c 6574 5f70 726f 7065 7274  tracklet_propert
-00012390: 6965 735b 3a2c 305d 0d0a 2020 2020 2020  ies[:,0]..      
-000123a0: 2020 2020 2020 2020 2020 756e 6971 7565            unique
-000123b0: 5f69 6473 203d 2074 7261 636b 6c65 745f  _ids = tracklet_
-000123c0: 7072 6f70 6572 7469 6573 5b3a 2c31 5d0d  properties[:,1].
-000123d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000123e0: 2075 6e69 7175 655f 6964 735f 7365 7420   unique_ids_set 
-000123f0: 3d20 7365 7428 756e 6971 7565 5f69 6473  = set(unique_ids
-00012400: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00012410: 2020 2067 656e 6572 6174 696f 6e5f 6964     generation_id
-00012420: 7320 3d20 7472 6163 6b6c 6574 5f70 726f  s = tracklet_pro
-00012430: 7065 7274 6965 735b 3a2c 325d 0d0a 2020  perties[:,2]..  
-00012440: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00012450: 6469 7573 203d 2074 7261 636b 6c65 745f  dius = tracklet_
-00012460: 7072 6f70 6572 7469 6573 5b3a 2c33 5d0d  properties[:,3].
-00012470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012480: 2076 6f6c 756d 6520 3d20 7472 6163 6b6c   volume = trackl
-00012490: 6574 5f70 726f 7065 7274 6965 735b 3a2c  et_properties[:,
-000124a0: 345d 0d0a 2020 2020 2020 2020 2020 2020  4]..            
-000124b0: 2020 2020 6563 6365 6e74 7269 6369 7479      eccentricity
-000124c0: 5f63 6f6d 705f 6669 7273 7420 3d20 7472  _comp_first = tr
-000124d0: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
-000124e0: 735b 3a2c 355d 0d0a 2020 2020 2020 2020  s[:,5]..        
-000124f0: 2020 2020 2020 2020 6563 6365 6e74 7269          eccentri
-00012500: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
-00012510: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
-00012520: 6572 7469 6573 5b3a 2c36 5d0d 0a20 2020  erties[:,6]..   
-00012530: 2020 2020 2020 2020 2020 2020 2073 7572               sur
-00012540: 6661 6365 5f61 7265 6120 3d20 7472 6163  face_area = trac
-00012550: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
-00012560: 3a2c 375d 0d0a 2020 2020 2020 2020 2020  :,7]..          
-00012570: 2020 2020 2020 636c 7573 7465 725f 636c        cluster_cl
-00012580: 6173 7320 3d20 7472 6163 6b6c 6574 5f70  ass = tracklet_p
-00012590: 726f 7065 7274 6965 735b 3a2c 385d 0d0a  roperties[:,8]..
-000125a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125b0: 636c 7573 7465 725f 636c 6173 735f 7363  cluster_class_sc
-000125c0: 6f72 6520 3d20 7472 6163 6b6c 6574 5f70  ore = tracklet_p
-000125d0: 726f 7065 7274 6965 735b 3a2c 395d 0d0a  roperties[:,9]..
-000125e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125f0: 696e 7465 6e73 6974 7920 3d20 7472 6163  intensity = trac
-00012600: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
-00012610: 3a2c 3130 5d0d 0a20 2020 2020 2020 2020  :,10]..         
-00012620: 2020 2020 2020 2073 7065 6564 203d 2074         speed = t
-00012630: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
-00012640: 6573 5b3a 2c31 315d 0d0a 2020 2020 2020  es[:,11]..      
-00012650: 2020 2020 2020 2020 2020 6d6f 7469 6f6e            motion
-00012660: 5f61 6e67 6c65 203d 2074 7261 636b 6c65  _angle = trackle
-00012670: 745f 7072 6f70 6572 7469 6573 5b3a 2c31  t_properties[:,1
-00012680: 325d 0d0a 2020 2020 2020 2020 2020 2020  2]..            
-00012690: 2020 2020 6163 6365 6c65 7261 7469 6f6e      acceleration
-000126a0: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
-000126b0: 6572 7469 6573 5b3a 2c31 335d 0d0a 2020  erties[:,13]..  
-000126c0: 2020 2020 2020 2020 2020 2020 2020 6469                di
-000126d0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-000126e0: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
-000126f0: 6572 7469 6573 5b3a 2c31 345d 0d0a 2020  erties[:,14]..  
-00012700: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00012710: 6469 616c 5f61 6e67 6c65 203d 2074 7261  dial_angle = tra
-00012720: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
-00012730: 5b3a 2c31 355d 0d0a 2020 2020 2020 2020  [:,15]..        
-00012740: 2020 2020 2020 2020 6365 6c6c 5f61 7869          cell_axi
-00012750: 735f 6d61 736b 203d 2074 7261 636b 6c65  s_mask = trackle
-00012760: 745f 7072 6f70 6572 7469 6573 5b3a 2c31  t_properties[:,1
-00012770: 365d 0d0a 0d0a 0d0a 2020 2020 2020 2020  6]......        
-00012780: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00012790: 2020 2020 2020 2020 2020 756e 6971 7565            unique
-000127a0: 5f66 6674 5f70 726f 7065 7274 6965 735f  _fft_properties_
-000127b0: 7472 6163 6b6c 6574 203d 207b 7d0d 0a20  tracklet = {}.. 
-000127c0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-000127d0: 6e69 7175 655f 636c 7573 7465 725f 7072  nique_cluster_pr
-000127e0: 6f70 6572 7469 6573 5f74 7261 636b 6c65  operties_trackle
-000127f0: 7420 3d20 7b7d 0d0a 2020 2020 2020 2020  t = {}..        
-00012800: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00012810: 7175 655f 6666 745f 7072 6f70 6572 7469  que_fft_properti
-00012820: 6573 5b74 7261 636b 5f69 645d 203d 207b  es[track_id] = {
-00012830: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
-00012840: 2020 2073 656c 662e 756e 6971 7565 5f63     self.unique_c
-00012850: 6c75 7374 6572 5f70 726f 7065 7274 6965  luster_propertie
-00012860: 735b 7472 6163 6b5f 6964 5d20 3d20 7b7d  s[track_id] = {}
-00012870: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00012880: 2020 2020 756e 6971 7565 5f73 6861 7065      unique_shape
-00012890: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
-000128a0: 6b6c 6574 203d 207b 7d0d 0a20 2020 2020  klet = {}..     
-000128b0: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
-000128c0: 655f 6479 6e61 6d69 635f 7072 6f70 6572  e_dynamic_proper
-000128d0: 7469 6573 5f74 7261 636b 6c65 7420 3d20  ties_tracklet = 
-000128e0: 7b7d 0d0a 2020 2020 2020 2020 2020 2020  {}..            
-000128f0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00012900: 7368 6170 655f 7072 6f70 6572 7469 6573  shape_properties
-00012910: 5b74 7261 636b 5f69 645d 203d 207b 7d0d  [track_id] = {}.
-00012920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012930: 2073 656c 662e 756e 6971 7565 5f64 796e   self.unique_dyn
-00012940: 616d 6963 5f70 726f 7065 7274 6965 735b  amic_properties[
-00012950: 7472 6163 6b5f 6964 5d20 3d20 7b7d 0d0a  track_id] = {}..
-00012960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012970: 6578 7061 6e64 6564 5f74 696d 6520 3d20  expanded_time = 
-00012980: 6e70 2e7a 6572 6f73 2873 656c 662e 7465  np.zeros(self.te
-00012990: 6e64 202d 2073 656c 662e 7473 7461 7274  nd - self.tstart
-000129a0: 202b 2031 290d 0a20 2020 2020 2020 2020   + 1)..         
-000129b0: 2020 2020 2020 2070 6f69 6e74 5f73 616d         point_sam
-000129c0: 706c 6520 3d20 6578 7061 6e64 6564 5f74  ple = expanded_t
-000129d0: 696d 652e 7368 6170 655b 305d 0d0a 2020  ime.shape[0]..  
-000129e0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-000129f0: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
-00012a00: 2865 7870 616e 6465 645f 7469 6d65 2929  (expanded_time))
-00012a10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00012a20: 2020 2020 2020 2020 2020 6578 7061 6e64            expand
-00012a30: 6564 5f74 696d 655b 695d 203d 2069 200d  ed_time[i] = i .
-00012a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012a50: 2066 6f72 2063 7572 7265 6e74 5f75 6e69   for current_uni
-00012a60: 7175 655f 6964 2069 6e20 756e 6971 7565  que_id in unique
-00012a70: 5f69 6473 5f73 6574 3a0d 0a20 2020 2020  _ids_set:..     
-00012a80: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+000121b0: 2020 2020 7365 6c66 2e72 6f6f 745f 7370      self.root_sp
+000121c0: 6f74 735b 6b5d 203d 2073 656c 662e 756e  ots[k] = self.un
+000121d0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000121e0: 7469 6573 5b6b 5d20 2020 2020 2020 2020  ties[k]         
+000121f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012200: 2020 0d0a 2020 2020 6465 6620 5f63 6f6d    ..    def _com
+00012210: 7075 7465 5f70 6865 6e6f 7479 7065 7328  pute_phenotypes(
+00012220: 7365 6c66 293a 0d0a 0d0a 2020 2020 2020  self):....      
+00012230: 2020 2020 666f 7220 286b 2c76 2920 696e      for (k,v) in
+00012240: 2073 656c 662e 756e 6971 7565 5f74 7261   self.unique_tra
+00012250: 636b 732e 6974 656d 7328 293a 0d0a 2020  cks.items():..  
+00012260: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00012270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012280: 7472 6163 6b5f 6964 203d 206b 0d0a 2020  track_id = k..  
+00012290: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+000122a0: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
+000122b0: 7320 3d20 7365 6c66 2e75 6e69 7175 655f  s = self.unique_
+000122c0: 7472 6163 6b5f 7072 6f70 6572 7469 6573  track_properties
+000122d0: 5b6b 5d0d 0a20 2020 2020 2020 2020 2020  [k]..           
+000122e0: 2020 2020 2074 7261 636b 7320 3d20 7365       tracks = se
+000122f0: 6c66 2e75 6e69 7175 655f 7472 6163 6b73  lf.unique_tracks
+00012300: 5b6b 5d0d 0a20 2020 2020 2020 2020 2020  [k]..           
+00012310: 2020 2020 205a 203d 2074 7261 636b 735b       Z = tracks[
+00012320: 3a2c 325d 0d0a 2020 2020 2020 2020 2020  :,2]..          
+00012330: 2020 2020 2020 5920 3d20 7472 6163 6b73        Y = tracks
+00012340: 5b3a 2c33 5d0d 0a20 2020 2020 2020 2020  [:,3]..         
+00012350: 2020 2020 2020 2058 203d 2074 7261 636b         X = track
+00012360: 735b 3a2c 345d 0d0a 2020 2020 2020 2020  s[:,4]..        
+00012370: 2020 2020 2020 2020 7469 6d65 203d 2074          time = t
+00012380: 7261 636b 6c65 745f 7072 6f70 6572 7469  racklet_properti
+00012390: 6573 5b3a 2c30 5d0d 0a20 2020 2020 2020  es[:,0]..       
+000123a0: 2020 2020 2020 2020 2075 6e69 7175 655f           unique_
+000123b0: 6964 7320 3d20 7472 6163 6b6c 6574 5f70  ids = tracklet_p
+000123c0: 726f 7065 7274 6965 735b 3a2c 315d 0d0a  roperties[:,1]..
+000123d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123e0: 756e 6971 7565 5f69 6473 5f73 6574 203d  unique_ids_set =
+000123f0: 2073 6574 2875 6e69 7175 655f 6964 7329   set(unique_ids)
+00012400: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012410: 2020 6765 6e65 7261 7469 6f6e 5f69 6473    generation_ids
+00012420: 203d 2074 7261 636b 6c65 745f 7072 6f70   = tracklet_prop
+00012430: 6572 7469 6573 5b3a 2c32 5d0d 0a20 2020  erties[:,2]..   
+00012440: 2020 2020 2020 2020 2020 2020 2072 6164               rad
+00012450: 6975 7320 3d20 7472 6163 6b6c 6574 5f70  ius = tracklet_p
+00012460: 726f 7065 7274 6965 735b 3a2c 335d 0d0a  roperties[:,3]..
+00012470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012480: 766f 6c75 6d65 203d 2074 7261 636b 6c65  volume = trackle
+00012490: 745f 7072 6f70 6572 7469 6573 5b3a 2c34  t_properties[:,4
+000124a0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000124b0: 2020 2065 6363 656e 7472 6963 6974 795f     eccentricity_
+000124c0: 636f 6d70 5f66 6972 7374 203d 2074 7261  comp_first = tra
+000124d0: 636b 6c65 745f 7072 6f70 6572 7469 6573  cklet_properties
+000124e0: 5b3a 2c35 5d0d 0a20 2020 2020 2020 2020  [:,5]..         
+000124f0: 2020 2020 2020 2065 6363 656e 7472 6963         eccentric
+00012500: 6974 795f 636f 6d70 5f73 6563 6f6e 6420  ity_comp_second 
+00012510: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
+00012520: 7274 6965 735b 3a2c 365d 0d0a 2020 2020  rties[:,6]..    
+00012530: 2020 2020 2020 2020 2020 2020 7375 7266              surf
+00012540: 6163 655f 6172 6561 203d 2074 7261 636b  ace_area = track
+00012550: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
+00012560: 2c37 5d0d 0a20 2020 2020 2020 2020 2020  ,7]..           
+00012570: 2020 2020 2063 6c75 7374 6572 5f63 6c61       cluster_cla
+00012580: 7373 203d 2074 7261 636b 6c65 745f 7072  ss = tracklet_pr
+00012590: 6f70 6572 7469 6573 5b3a 2c38 5d0d 0a20  operties[:,8].. 
+000125a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000125b0: 6c75 7374 6572 5f63 6c61 7373 5f73 636f  luster_class_sco
+000125c0: 7265 203d 2074 7261 636b 6c65 745f 7072  re = tracklet_pr
+000125d0: 6f70 6572 7469 6573 5b3a 2c39 5d0d 0a20  operties[:,9].. 
+000125e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000125f0: 6e74 656e 7369 7479 203d 2074 7261 636b  ntensity = track
+00012600: 6c65 745f 7072 6f70 6572 7469 6573 5b3a  let_properties[:
+00012610: 2c31 305d 0d0a 2020 2020 2020 2020 2020  ,10]..          
+00012620: 2020 2020 2020 7370 6565 6420 3d20 7472        speed = tr
+00012630: 6163 6b6c 6574 5f70 726f 7065 7274 6965  acklet_propertie
+00012640: 735b 3a2c 3131 5d0d 0a20 2020 2020 2020  s[:,11]..       
+00012650: 2020 2020 2020 2020 206d 6f74 696f 6e5f           motion_
+00012660: 616e 676c 6520 3d20 7472 6163 6b6c 6574  angle = tracklet
+00012670: 5f70 726f 7065 7274 6965 735b 3a2c 3132  _properties[:,12
+00012680: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00012690: 2020 2061 6363 656c 6572 6174 696f 6e20     acceleration 
+000126a0: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
+000126b0: 7274 6965 735b 3a2c 3133 5d0d 0a20 2020  rties[:,13]..   
+000126c0: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+000126d0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
+000126e0: 3d20 7472 6163 6b6c 6574 5f70 726f 7065  = tracklet_prope
+000126f0: 7274 6965 735b 3a2c 3134 5d0d 0a20 2020  rties[:,14]..   
+00012700: 2020 2020 2020 2020 2020 2020 2072 6164               rad
+00012710: 6961 6c5f 616e 676c 6520 3d20 7472 6163  ial_angle = trac
+00012720: 6b6c 6574 5f70 726f 7065 7274 6965 735b  klet_properties[
+00012730: 3a2c 3135 5d0d 0a20 2020 2020 2020 2020  :,15]..         
+00012740: 2020 2020 2020 2063 656c 6c5f 6178 6973         cell_axis
+00012750: 5f6d 6173 6b20 3d20 7472 6163 6b6c 6574  _mask = tracklet
+00012760: 5f70 726f 7065 7274 6965 735b 3a2c 3136  _properties[:,16
+00012770: 5d0d 0a0d 0a0d 0a20 2020 2020 2020 2020  ]......         
+00012780: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00012790: 2020 2020 2020 2020 2075 6e69 7175 655f           unique_
+000127a0: 6666 745f 7072 6f70 6572 7469 6573 5f74  fft_properties_t
+000127b0: 7261 636b 6c65 7420 3d20 7b7d 0d0a 2020  racklet = {}..  
+000127c0: 2020 2020 2020 2020 2020 2020 2020 756e                un
+000127d0: 6971 7565 5f63 6c75 7374 6572 5f70 726f  ique_cluster_pro
+000127e0: 7065 7274 6965 735f 7472 6163 6b6c 6574  perties_tracklet
+000127f0: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
+00012800: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00012810: 7565 5f66 6674 5f70 726f 7065 7274 6965  ue_fft_propertie
+00012820: 735b 7472 6163 6b5f 6964 5d20 3d20 7b7d  s[track_id] = {}
+00012830: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012840: 2020 7365 6c66 2e75 6e69 7175 655f 636c    self.unique_cl
+00012850: 7573 7465 725f 7072 6f70 6572 7469 6573  uster_properties
+00012860: 5b74 7261 636b 5f69 645d 203d 207b 7d0d  [track_id] = {}.
+00012870: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00012880: 2020 2075 6e69 7175 655f 7368 6170 655f     unique_shape_
+00012890: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
+000128a0: 6c65 7420 3d20 7b7d 0d0a 2020 2020 2020  let = {}..      
+000128b0: 2020 2020 2020 2020 2020 756e 6971 7565            unique
+000128c0: 5f64 796e 616d 6963 5f70 726f 7065 7274  _dynamic_propert
+000128d0: 6965 735f 7472 6163 6b6c 6574 203d 207b  ies_tracklet = {
+000128e0: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
+000128f0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00012900: 6861 7065 5f70 726f 7065 7274 6965 735b  hape_properties[
+00012910: 7472 6163 6b5f 6964 5d20 3d20 7b7d 0d0a  track_id] = {}..
+00012920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012930: 7365 6c66 2e75 6e69 7175 655f 6479 6e61  self.unique_dyna
+00012940: 6d69 635f 7072 6f70 6572 7469 6573 5b74  mic_properties[t
+00012950: 7261 636b 5f69 645d 203d 207b 7d0d 0a20  rack_id] = {}.. 
+00012960: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00012970: 7870 616e 6465 645f 7469 6d65 203d 206e  xpanded_time = n
+00012980: 702e 7a65 726f 7328 7365 6c66 2e74 656e  p.zeros(self.ten
+00012990: 6420 2d20 7365 6c66 2e74 7374 6172 7420  d - self.tstart 
+000129a0: 2b20 3129 0d0a 2020 2020 2020 2020 2020  + 1)..          
+000129b0: 2020 2020 2020 706f 696e 745f 7361 6d70        point_samp
+000129c0: 6c65 203d 2065 7870 616e 6465 645f 7469  le = expanded_ti
+000129d0: 6d65 2e73 6861 7065 5b30 5d0d 0a20 2020  me.shape[0]..   
+000129e0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+000129f0: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
+00012a00: 6578 7061 6e64 6564 5f74 696d 6529 293a  expanded_time)):
+00012a10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012a20: 2020 2020 2020 2020 2065 7870 616e 6465           expande
+00012a30: 645f 7469 6d65 5b69 5d20 3d20 6920 0d0a  d_time[i] = i ..
+00012a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a50: 666f 7220 6375 7272 656e 745f 756e 6971  for current_uniq
+00012a60: 7565 5f69 6420 696e 2075 6e69 7175 655f  ue_id in unique_
+00012a70: 6964 735f 7365 743a 0d0a 2020 2020 2020  ids_set:..      
+00012a80: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
 00012a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012aa0: 2020 2065 7870 616e 6465 645f 696e 7465     expanded_inte
-00012ab0: 6e73 6974 7920 3d20 6e70 2e7a 6572 6f73  nsity = np.zeros
-00012ac0: 2873 656c 662e 7465 6e64 202d 2073 656c  (self.tend - sel
-00012ad0: 662e 7473 7461 7274 202b 2031 290d 0a20  f.tstart + 1).. 
+00012aa0: 2020 6578 7061 6e64 6564 5f69 6e74 656e    expanded_inten
+00012ab0: 7369 7479 203d 206e 702e 7a65 726f 7328  sity = np.zeros(
+00012ac0: 7365 6c66 2e74 656e 6420 2d20 7365 6c66  self.tend - self
+00012ad0: 2e74 7374 6172 7420 2b20 3129 0d0a 2020  .tstart + 1)..  
 00012ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012af0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00012b00: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00012b10: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00012b20: 656e 745f 7469 6d65 203d 205b 5d0d 0a20  ent_time = [].. 
+00012af0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00012b00: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00012b10: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012b20: 6e74 5f74 696d 6520 3d20 5b5d 0d0a 2020  nt_time = []..  
 00012b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b40: 2020 6375 7272 656e 745f 7a20 3d20 5b5d    current_z = []
-00012b50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012b60: 2020 2020 2063 7572 7265 6e74 5f79 203d       current_y =
-00012b70: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00012b80: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00012b90: 7820 3d20 5b5d 0d0a 2020 2020 2020 2020  x = []..        
-00012ba0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00012bb0: 6e74 5f69 6e74 656e 7369 7479 203d 205b  nt_intensity = [
-00012bc0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00012bd0: 2020 2020 2020 6375 7272 656e 745f 636c        current_cl
-00012be0: 7573 7465 725f 636c 6173 7320 3d20 5b5d  uster_class = []
-00012bf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00012c00: 2020 2020 2063 7572 7265 6e74 5f63 6c75       current_clu
-00012c10: 7374 6572 5f63 6c61 7373 5f73 636f 7265  ster_class_score
-00012c20: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00012c30: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00012c40: 745f 7261 6469 7573 203d 205b 5d0d 0a20  t_radius = [].. 
+00012b40: 2063 7572 7265 6e74 5f7a 203d 205b 5d0d   current_z = [].
+00012b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012b60: 2020 2020 6375 7272 656e 745f 7920 3d20      current_y = 
+00012b70: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00012b80: 2020 2020 2020 2063 7572 7265 6e74 5f78         current_x
+00012b90: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00012ba0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00012bb0: 745f 696e 7465 6e73 6974 7920 3d20 5b5d  t_intensity = []
+00012bc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012bd0: 2020 2020 2063 7572 7265 6e74 5f63 6c75       current_clu
+00012be0: 7374 6572 5f63 6c61 7373 203d 205b 5d0d  ster_class = [].
+00012bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012c00: 2020 2020 6375 7272 656e 745f 636c 7573      current_clus
+00012c10: 7465 725f 636c 6173 735f 7363 6f72 6520  ter_class_score 
+00012c20: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00012c30: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00012c40: 5f72 6164 6975 7320 3d20 5b5d 0d0a 2020  _radius = []..  
 00012c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c60: 2020 6375 7272 656e 745f 766f 6c75 6d65    current_volume
-00012c70: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00012c80: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00012c90: 745f 7370 6565 6420 3d20 5b5d 0d0a 2020  t_speed = []..  
+00012c60: 2063 7572 7265 6e74 5f76 6f6c 756d 6520   current_volume 
+00012c70: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00012c80: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00012c90: 5f73 7065 6564 203d 205b 5d0d 0a20 2020  _speed = []..   
 00012ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012cb0: 2063 7572 7265 6e74 5f6d 6f74 696f 6e5f   current_motion_
-00012cc0: 616e 676c 6520 3d20 5b5d 0d0a 2020 2020  angle = []..    
-00012cd0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00012ce0: 7572 7265 6e74 5f61 6363 656c 6572 6174  urrent_accelerat
-00012cf0: 696f 6e20 3d20 5b5d 0d0a 2020 2020 2020  ion = []..      
-00012d00: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00012d10: 7265 6e74 5f64 6973 7461 6e63 655f 6365  rent_distance_ce
-00012d20: 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a 2020  ll_mask = []..  
+00012cb0: 6375 7272 656e 745f 6d6f 7469 6f6e 5f61  current_motion_a
+00012cc0: 6e67 6c65 203d 205b 5d0d 0a20 2020 2020  ngle = []..     
+00012cd0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+00012ce0: 7272 656e 745f 6163 6365 6c65 7261 7469  rrent_accelerati
+00012cf0: 6f6e 203d 205b 5d0d 0a20 2020 2020 2020  on = []..       
+00012d00: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00012d10: 656e 745f 6469 7374 616e 6365 5f63 656c  ent_distance_cel
+00012d20: 6c5f 6d61 736b 203d 205b 5d0d 0a20 2020  l_mask = []..   
 00012d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d40: 2063 7572 7265 6e74 5f65 6363 656e 7472   current_eccentr
-00012d50: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
-00012d60: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00012d70: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00012d80: 745f 6563 6365 6e74 7269 6369 7479 5f63  t_eccentricity_c
-00012d90: 6f6d 705f 7365 636f 6e64 203d 205b 5d0d  omp_second = [].
-00012da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012db0: 2020 2020 6375 7272 656e 745f 7375 7266      current_surf
-00012dc0: 6163 655f 6172 6561 203d 205b 5d0d 0a0d  ace_area = []...
-00012dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012de0: 2020 2020 6375 7272 656e 745f 7261 6469      current_radi
-00012df0: 616c 5f61 6e67 6c65 203d 205b 5d0d 0a20  al_angle = [].. 
+00012d40: 6375 7272 656e 745f 6563 6365 6e74 7269  current_eccentri
+00012d50: 6369 7479 5f63 6f6d 705f 6669 7273 7420  city_comp_first 
+00012d60: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00012d70: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00012d80: 5f65 6363 656e 7472 6963 6974 795f 636f  _eccentricity_co
+00012d90: 6d70 5f73 6563 6f6e 6420 3d20 5b5d 0d0a  mp_second = []..
+00012da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012db0: 2020 2063 7572 7265 6e74 5f73 7572 6661     current_surfa
+00012dc0: 6365 5f61 7265 6120 3d20 5b5d 0d0a 0d0a  ce_area = []....
+00012dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012de0: 2020 2063 7572 7265 6e74 5f72 6164 6961     current_radia
+00012df0: 6c5f 616e 676c 6520 3d20 5b5d 0d0a 2020  l_angle = []..  
 00012e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e10: 2020 6375 7272 656e 745f 6365 6c6c 5f61    current_cell_a
-00012e20: 7869 735f 6d61 736b 203d 205b 5d20 0d0a  xis_mask = [] ..
+00012e10: 2063 7572 7265 6e74 5f63 656c 6c5f 6178   current_cell_ax
+00012e20: 6973 5f6d 6173 6b20 3d20 5b5d 200d 0a20  is_mask = [] .. 
 00012e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e40: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00012e50: 2020 2020 2020 2020 666f 7220 6a20 696e          for j in
-00012e60: 2072 616e 6765 2874 696d 652e 7368 6170   range(time.shap
-00012e70: 655b 305d 293a 0d0a 2020 2020 2020 2020  e[0]):..        
+00012e40: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00012e50: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
+00012e60: 7261 6e67 6528 7469 6d65 2e73 6861 7065  range(time.shape
+00012e70: 5b30 5d29 3a0d 0a20 2020 2020 2020 2020  [0]):..         
 00012e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e90: 2020 6966 2063 7572 7265 6e74 5f75 6e69    if current_uni
-00012ea0: 7175 655f 6964 203d 3d20 756e 6971 7565  que_id == unique
-00012eb0: 5f69 6473 5b6a 5d3a 0d0a 2020 2020 2020  _ids[j]:..      
+00012e90: 2069 6620 6375 7272 656e 745f 756e 6971   if current_uniq
+00012ea0: 7565 5f69 6420 3d3d 2075 6e69 7175 655f  ue_id == unique_
+00012eb0: 6964 735b 6a5d 3a0d 0a20 2020 2020 2020  ids[j]:..       
 00012ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ed0: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-00012ee0: 6e74 5f74 696d 652e 6170 7065 6e64 2874  nt_time.append(t
-00012ef0: 696d 655b 6a5d 290d 0a20 2020 2020 2020  ime[j])..       
+00012ed0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
+00012ee0: 745f 7469 6d65 2e61 7070 656e 6428 7469  t_time.append(ti
+00012ef0: 6d65 5b6a 5d29 0d0a 2020 2020 2020 2020  me[j])..        
 00012f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f10: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00012f20: 745f 7a2e 6170 7065 6e64 285a 5b6a 5d29  t_z.append(Z[j])
-00012f30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00012f10: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00012f20: 5f7a 2e61 7070 656e 6428 5a5b 6a5d 290d  _z.append(Z[j]).
+00012f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00012f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f50: 2020 2063 7572 7265 6e74 5f79 2e61 7070     current_y.app
-00012f60: 656e 6428 595b 6a5d 290d 0a20 2020 2020  end(Y[j])..     
+00012f50: 2020 6375 7272 656e 745f 792e 6170 7065    current_y.appe
+00012f60: 6e64 2859 5b6a 5d29 0d0a 2020 2020 2020  nd(Y[j])..      
 00012f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f80: 2020 2020 2020 2020 2020 2020 6375 7272              curr
-00012f90: 656e 745f 782e 6170 7065 6e64 2858 5b6a  ent_x.append(X[j
-00012fa0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00012f80: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+00012f90: 6e74 5f78 2e61 7070 656e 6428 585b 6a5d  nt_x.append(X[j]
+00012fa0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00012fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012fc0: 2020 2020 2065 7870 616e 6465 645f 696e       expanded_in
-00012fd0: 7465 6e73 6974 795b 696e 7428 7469 6d65  tensity[int(time
-00012fe0: 5b6a 5d29 5d20 3d20 696e 7465 6e73 6974  [j])] = intensit
-00012ff0: 795b 6a5d 0d0a 2020 2020 2020 2020 2020  y[j]..          
+00012fc0: 2020 2020 6578 7061 6e64 6564 5f69 6e74      expanded_int
+00012fd0: 656e 7369 7479 5b69 6e74 2874 696d 655b  ensity[int(time[
+00012fe0: 6a5d 295d 203d 2069 6e74 656e 7369 7479  j])] = intensity
+00012ff0: 5b6a 5d0d 0a20 2020 2020 2020 2020 2020  [j]..           
 00013000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013010: 2020 2020 2020 2063 7572 7265 6e74 5f69         current_i
-00013020: 6e74 656e 7369 7479 2e61 7070 656e 6428  ntensity.append(
-00013030: 696e 7465 6e73 6974 795b 6a5d 290d 0a20  intensity[j]).. 
+00013010: 2020 2020 2020 6375 7272 656e 745f 696e        current_in
+00013020: 7465 6e73 6974 792e 6170 7065 6e64 2869  tensity.append(i
+00013030: 6e74 656e 7369 7479 5b6a 5d29 0d0a 2020  ntensity[j])..  
 00013040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013060: 6375 7272 656e 745f 636c 7573 7465 725f  current_cluster_
-00013070: 636c 6173 732e 6170 7065 6e64 2863 6c75  class.append(clu
-00013080: 7374 6572 5f63 6c61 7373 5b6a 5d29 0d0a  ster_class[j])..
+00013050: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013060: 7572 7265 6e74 5f63 6c75 7374 6572 5f63  urrent_cluster_c
+00013070: 6c61 7373 2e61 7070 656e 6428 636c 7573  lass.append(clus
+00013080: 7465 725f 636c 6173 735b 6a5d 290d 0a20  ter_class[j]).. 
 00013090: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000130a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130b0: 2063 7572 7265 6e74 5f63 6c75 7374 6572   current_cluster
-000130c0: 5f63 6c61 7373 5f73 636f 7265 2e61 7070  _class_score.app
-000130d0: 656e 6428 636c 7573 7465 725f 636c 6173  end(cluster_clas
-000130e0: 735f 7363 6f72 655b 6a5d 290d 0a20 2020  s_score[j])..   
+000130b0: 6375 7272 656e 745f 636c 7573 7465 725f  current_cluster_
+000130c0: 636c 6173 735f 7363 6f72 652e 6170 7065  class_score.appe
+000130d0: 6e64 2863 6c75 7374 6572 5f63 6c61 7373  nd(cluster_class
+000130e0: 5f73 636f 7265 5b6a 5d29 0d0a 2020 2020  _score[j])..    
 000130f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013100: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00013110: 7272 656e 745f 7261 6469 7573 2e61 7070  rrent_radius.app
-00013120: 656e 6428 7261 6469 7573 5b6a 5d29 0d0a  end(radius[j])..
+00013100: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+00013110: 7265 6e74 5f72 6164 6975 732e 6170 7065  rent_radius.appe
+00013120: 6e64 2872 6164 6975 735b 6a5d 290d 0a20  nd(radius[j]).. 
 00013130: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013150: 2063 7572 7265 6e74 5f76 6f6c 756d 652e   current_volume.
-00013160: 6170 7065 6e64 2876 6f6c 756d 655b 6a5d  append(volume[j]
-00013170: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00013150: 6375 7272 656e 745f 766f 6c75 6d65 2e61  current_volume.a
+00013160: 7070 656e 6428 766f 6c75 6d65 5b6a 5d29  ppend(volume[j])
+00013170: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00013180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013190: 2020 2020 6375 7272 656e 745f 7370 6565      current_spee
-000131a0: 642e 6170 7065 6e64 2873 7065 6564 5b6a  d.append(speed[j
-000131b0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+00013190: 2020 2063 7572 7265 6e74 5f73 7065 6564     current_speed
+000131a0: 2e61 7070 656e 6428 7370 6565 645b 6a5d  .append(speed[j]
+000131b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 000131c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000131d0: 2020 2020 2063 7572 7265 6e74 5f6d 6f74       current_mot
-000131e0: 696f 6e5f 616e 676c 652e 6170 7065 6e64  ion_angle.append
-000131f0: 286d 6f74 696f 6e5f 616e 676c 655b 6a5d  (motion_angle[j]
-00013200: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000131d0: 2020 2020 6375 7272 656e 745f 6d6f 7469      current_moti
+000131e0: 6f6e 5f61 6e67 6c65 2e61 7070 656e 6428  on_angle.append(
+000131f0: 6d6f 7469 6f6e 5f61 6e67 6c65 5b6a 5d29  motion_angle[j])
+00013200: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00013210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013220: 2020 2020 6375 7272 656e 745f 6163 6365      current_acce
-00013230: 6c65 7261 7469 6f6e 2e61 7070 656e 6428  leration.append(
-00013240: 6163 6365 6c65 7261 7469 6f6e 5b6a 5d29  acceleration[j])
-00013250: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013220: 2020 2063 7572 7265 6e74 5f61 6363 656c     current_accel
+00013230: 6572 6174 696f 6e2e 6170 7065 6e64 2861  eration.append(a
+00013240: 6363 656c 6572 6174 696f 6e5b 6a5d 290d  cceleration[j]).
+00013250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00013260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013270: 2020 2063 7572 7265 6e74 5f64 6973 7461     current_dista
-00013280: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
-00013290: 7065 6e64 2864 6973 7461 6e63 655f 6365  pend(distance_ce
-000132a0: 6c6c 5f6d 6173 6b5b 6a5d 290d 0a20 2020  ll_mask[j])..   
+00013270: 2020 6375 7272 656e 745f 6469 7374 616e    current_distan
+00013280: 6365 5f63 656c 6c5f 6d61 736b 2e61 7070  ce_cell_mask.app
+00013290: 656e 6428 6469 7374 616e 6365 5f63 656c  end(distance_cel
+000132a0: 6c5f 6d61 736b 5b6a 5d29 0d0a 2020 2020  l_mask[j])..    
 000132b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132c0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-000132d0: 7272 656e 745f 6563 6365 6e74 7269 6369  rrent_eccentrici
-000132e0: 7479 5f63 6f6d 705f 6669 7273 742e 6170  ty_comp_first.ap
-000132f0: 7065 6e64 2865 6363 656e 7472 6963 6974  pend(eccentricit
-00013300: 795f 636f 6d70 5f66 6972 7374 5b6a 5d29  y_comp_first[j])
-00013310: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000132c0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+000132d0: 7265 6e74 5f65 6363 656e 7472 6963 6974  rent_eccentricit
+000132e0: 795f 636f 6d70 5f66 6972 7374 2e61 7070  y_comp_first.app
+000132f0: 656e 6428 6563 6365 6e74 7269 6369 7479  end(eccentricity
+00013300: 5f63 6f6d 705f 6669 7273 745b 6a5d 290d  _comp_first[j]).
+00013310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00013320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013330: 2020 2063 7572 7265 6e74 5f65 6363 656e     current_eccen
-00013340: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
-00013350: 6f6e 642e 6170 7065 6e64 2865 6363 656e  ond.append(eccen
-00013360: 7472 6963 6974 795f 636f 6d70 5f73 6563  tricity_comp_sec
-00013370: 6f6e 645b 6a5d 290d 0a20 2020 2020 2020  ond[j])..       
+00013330: 2020 6375 7272 656e 745f 6563 6365 6e74    current_eccent
+00013340: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
+00013350: 6e64 2e61 7070 656e 6428 6563 6365 6e74  nd.append(eccent
+00013360: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
+00013370: 6e64 5b6a 5d29 0d0a 2020 2020 2020 2020  nd[j])..        
 00013380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013390: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-000133a0: 745f 7375 7266 6163 655f 6172 6561 2e61  t_surface_area.a
-000133b0: 7070 656e 6428 7375 7266 6163 655f 6172  ppend(surface_ar
-000133c0: 6561 5b6a 5d29 0d0a 2020 2020 2020 2020  ea[j])..        
+00013390: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+000133a0: 5f73 7572 6661 6365 5f61 7265 612e 6170  _surface_area.ap
+000133b0: 7065 6e64 2873 7572 6661 6365 5f61 7265  pend(surface_are
+000133c0: 615b 6a5d 290d 0a20 2020 2020 2020 2020  a[j])..         
 000133d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133e0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-000133f0: 5f72 6164 6961 6c5f 616e 676c 652e 6170  _radial_angle.ap
-00013400: 7065 6e64 2872 6164 6961 6c5f 616e 676c  pend(radial_angl
-00013410: 655b 6a5d 290d 0a20 2020 2020 2020 2020  e[j])..         
+000133e0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+000133f0: 7261 6469 616c 5f61 6e67 6c65 2e61 7070  radial_angle.app
+00013400: 656e 6428 7261 6469 616c 5f61 6e67 6c65  end(radial_angle
+00013410: 5b6a 5d29 0d0a 2020 2020 2020 2020 2020  [j])..          
 00013420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013430: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-00013440: 6365 6c6c 5f61 7869 735f 6d61 736b 2e61  cell_axis_mask.a
-00013450: 7070 656e 6428 6365 6c6c 5f61 7869 735f  ppend(cell_axis_
-00013460: 6d61 736b 5b6a 5d29 0d0a 2020 2020 2020  mask[j])..      
-00013470: 2020 2020 2020 2020 2020 2020 2063 7572               cur
-00013480: 7265 6e74 5f74 696d 6520 3d20 6e70 2e61  rent_time = np.a
-00013490: 7361 7272 6179 2863 7572 7265 6e74 5f74  sarray(current_t
-000134a0: 696d 6529 0d0a 2020 2020 2020 2020 2020  ime)..          
-000134b0: 2020 2020 2020 2020 2063 7572 7265 6e74           current
-000134c0: 5f69 6e74 656e 7369 7479 203d 206e 702e  _intensity = np.
-000134d0: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
-000134e0: 696e 7465 6e73 6974 7929 0d0a 0d0a 0d0a  intensity)......
+00013430: 2020 2020 2020 2063 7572 7265 6e74 5f63         current_c
+00013440: 656c 6c5f 6178 6973 5f6d 6173 6b2e 6170  ell_axis_mask.ap
+00013450: 7065 6e64 2863 656c 6c5f 6178 6973 5f6d  pend(cell_axis_m
+00013460: 6173 6b5b 6a5d 290d 0a20 2020 2020 2020  ask[j])..       
+00013470: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+00013480: 656e 745f 7469 6d65 203d 206e 702e 6173  ent_time = np.as
+00013490: 6172 7261 7928 6375 7272 656e 745f 7469  array(current_ti
+000134a0: 6d65 290d 0a20 2020 2020 2020 2020 2020  me)..           
+000134b0: 2020 2020 2020 2020 6375 7272 656e 745f          current_
+000134c0: 696e 7465 6e73 6974 7920 3d20 6e70 2e61  intensity = np.a
+000134d0: 7361 7272 6179 2863 7572 7265 6e74 5f69  sarray(current_i
+000134e0: 6e74 656e 7369 7479 290d 0a0d 0a0d 0a20  ntensity)...... 
 000134f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013500: 2020 2063 7572 7265 6e74 5f63 6c75 7374     current_clust
-00013510: 6572 5f63 6c61 7373 203d 206e 702e 6173  er_class = np.as
-00013520: 6172 7261 7928 6375 7272 656e 745f 636c  array(current_cl
-00013530: 7573 7465 725f 636c 6173 7329 0d0a 2020  uster_class)..  
+00013500: 2020 6375 7272 656e 745f 636c 7573 7465    current_cluste
+00013510: 725f 636c 6173 7320 3d20 6e70 2e61 7361  r_class = np.asa
+00013520: 7272 6179 2863 7572 7265 6e74 5f63 6c75  rray(current_clu
+00013530: 7374 6572 5f63 6c61 7373 290d 0a20 2020  ster_class)..   
 00013540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013550: 2063 7572 7265 6e74 5f63 6c75 7374 6572   current_cluster
-00013560: 5f63 6c61 7373 5f73 636f 7265 203d 206e  _class_score = n
-00013570: 702e 6173 6172 7261 7928 6375 7272 656e  p.asarray(curren
-00013580: 745f 636c 7573 7465 725f 636c 6173 735f  t_cluster_class_
-00013590: 7363 6f72 6529 2020 200d 0a0d 0a20 2020  score)   ....   
-000135a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135b0: 6375 7272 656e 745f 7261 6469 7573 203d  current_radius =
-000135c0: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
-000135d0: 656e 745f 7261 6469 7573 290d 0a20 2020  ent_radius)..   
-000135e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135f0: 6375 7272 656e 745f 766f 6c75 6d65 203d  current_volume =
-00013600: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
-00013610: 656e 745f 766f 6c75 6d65 290d 0a20 2020  ent_volume)..   
-00013620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013630: 6375 7272 656e 745f 6563 6365 6e74 7269  current_eccentri
-00013640: 6369 7479 5f63 6f6d 705f 6669 7273 7420  city_comp_first 
-00013650: 3d20 6e70 2e61 7361 7272 6179 2863 7572  = np.asarray(cur
-00013660: 7265 6e74 5f65 6363 656e 7472 6963 6974  rent_eccentricit
-00013670: 795f 636f 6d70 5f66 6972 7374 290d 0a20  y_comp_first).. 
+00013550: 6375 7272 656e 745f 636c 7573 7465 725f  current_cluster_
+00013560: 636c 6173 735f 7363 6f72 6520 3d20 6e70  class_score = np
+00013570: 2e61 7361 7272 6179 2863 7572 7265 6e74  .asarray(current
+00013580: 5f63 6c75 7374 6572 5f63 6c61 7373 5f73  _cluster_class_s
+00013590: 636f 7265 2920 2020 0d0a 0d0a 2020 2020  core)   ....    
+000135a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000135b0: 7572 7265 6e74 5f72 6164 6975 7320 3d20  urrent_radius = 
+000135c0: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
+000135d0: 6e74 5f72 6164 6975 7329 0d0a 2020 2020  nt_radius)..    
+000135e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000135f0: 7572 7265 6e74 5f76 6f6c 756d 6520 3d20  urrent_volume = 
+00013600: 6e70 2e61 7361 7272 6179 2863 7572 7265  np.asarray(curre
+00013610: 6e74 5f76 6f6c 756d 6529 0d0a 2020 2020  nt_volume)..    
+00013620: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013630: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
+00013640: 6974 795f 636f 6d70 5f66 6972 7374 203d  ity_comp_first =
+00013650: 206e 702e 6173 6172 7261 7928 6375 7272   np.asarray(curr
+00013660: 656e 745f 6563 6365 6e74 7269 6369 7479  ent_eccentricity
+00013670: 5f63 6f6d 705f 6669 7273 7429 0d0a 2020  _comp_first)..  
 00013680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013690: 2020 6375 7272 656e 745f 6563 6365 6e74    current_eccent
-000136a0: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
-000136b0: 6e64 203d 206e 702e 6173 6172 7261 7928  nd = np.asarray(
-000136c0: 6375 7272 656e 745f 6563 6365 6e74 7269  current_eccentri
-000136d0: 6369 7479 5f63 6f6d 705f 7365 636f 6e64  city_comp_second
-000136e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000136f0: 2020 2020 2020 6375 7272 656e 745f 7375        current_su
-00013700: 7266 6163 655f 6172 6561 203d 206e 702e  rface_area = np.
-00013710: 6173 6172 7261 7928 6375 7272 656e 745f  asarray(current_
-00013720: 7375 7266 6163 655f 6172 6561 290d 0a0d  surface_area)...
-00013730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013740: 2020 2020 6375 7272 656e 745f 7370 6565      current_spee
-00013750: 6420 3d20 6e70 2e61 7361 7272 6179 2863  d = np.asarray(c
-00013760: 7572 7265 6e74 5f73 7065 6564 290d 0a20  urrent_speed).. 
+00013690: 2063 7572 7265 6e74 5f65 6363 656e 7472   current_eccentr
+000136a0: 6963 6974 795f 636f 6d70 5f73 6563 6f6e  icity_comp_secon
+000136b0: 6420 3d20 6e70 2e61 7361 7272 6179 2863  d = np.asarray(c
+000136c0: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
+000136d0: 6974 795f 636f 6d70 5f73 6563 6f6e 6429  ity_comp_second)
+000136e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000136f0: 2020 2020 2063 7572 7265 6e74 5f73 7572       current_sur
+00013700: 6661 6365 5f61 7265 6120 3d20 6e70 2e61  face_area = np.a
+00013710: 7361 7272 6179 2863 7572 7265 6e74 5f73  sarray(current_s
+00013720: 7572 6661 6365 5f61 7265 6129 0d0a 0d0a  urface_area)....
+00013730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013740: 2020 2063 7572 7265 6e74 5f73 7065 6564     current_speed
+00013750: 203d 206e 702e 6173 6172 7261 7928 6375   = np.asarray(cu
+00013760: 7272 656e 745f 7370 6565 6429 0d0a 2020  rrent_speed)..  
 00013770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013780: 2020 6375 7272 656e 745f 6d6f 7469 6f6e    current_motion
-00013790: 5f61 6e67 6c65 203d 206e 702e 6173 6172  _angle = np.asar
-000137a0: 7261 7928 6375 7272 656e 745f 6d6f 7469  ray(current_moti
-000137b0: 6f6e 5f61 6e67 6c65 290d 0a20 2020 2020  on_angle)..     
-000137c0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-000137d0: 7272 656e 745f 6163 6365 6c65 7261 7469  rrent_accelerati
-000137e0: 6f6e 203d 206e 702e 6173 6172 7261 7928  on = np.asarray(
-000137f0: 6375 7272 656e 745f 6163 6365 6c65 7261  current_accelera
-00013800: 7469 6f6e 290d 0a20 2020 2020 2020 2020  tion)..         
-00013810: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00013820: 745f 6469 7374 616e 6365 5f63 656c 6c5f  t_distance_cell_
-00013830: 6d61 736b 203d 206e 702e 6173 6172 7261  mask = np.asarra
-00013840: 7928 6375 7272 656e 745f 6469 7374 616e  y(current_distan
-00013850: 6365 5f63 656c 6c5f 6d61 736b 290d 0a20  ce_cell_mask).. 
+00013780: 2063 7572 7265 6e74 5f6d 6f74 696f 6e5f   current_motion_
+00013790: 616e 676c 6520 3d20 6e70 2e61 7361 7272  angle = np.asarr
+000137a0: 6179 2863 7572 7265 6e74 5f6d 6f74 696f  ay(current_motio
+000137b0: 6e5f 616e 676c 6529 0d0a 2020 2020 2020  n_angle)..      
+000137c0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+000137d0: 7265 6e74 5f61 6363 656c 6572 6174 696f  rent_acceleratio
+000137e0: 6e20 3d20 6e70 2e61 7361 7272 6179 2863  n = np.asarray(c
+000137f0: 7572 7265 6e74 5f61 6363 656c 6572 6174  urrent_accelerat
+00013800: 696f 6e29 0d0a 2020 2020 2020 2020 2020  ion)..          
+00013810: 2020 2020 2020 2020 2063 7572 7265 6e74           current
+00013820: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+00013830: 6173 6b20 3d20 6e70 2e61 7361 7272 6179  ask = np.asarray
+00013840: 2863 7572 7265 6e74 5f64 6973 7461 6e63  (current_distanc
+00013850: 655f 6365 6c6c 5f6d 6173 6b29 0d0a 2020  e_cell_mask)..  
 00013860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013870: 2020 6375 7272 656e 745f 7261 6469 616c    current_radial
-00013880: 5f61 6e67 6c65 203d 206e 702e 6173 6172  _angle = np.asar
-00013890: 7261 7928 6375 7272 656e 745f 7261 6469  ray(current_radi
-000138a0: 616c 5f61 6e67 6c65 290d 0a20 2020 2020  al_angle)..     
-000138b0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-000138c0: 7272 656e 745f 6365 6c6c 5f61 7869 735f  rrent_cell_axis_
-000138d0: 6d61 736b 203d 206e 702e 6173 6172 7261  mask = np.asarra
-000138e0: 7928 6375 7272 656e 745f 6365 6c6c 5f61  y(current_cell_a
-000138f0: 7869 735f 6d61 736b 290d 0a0d 0a0d 0a20  xis_mask)...... 
+00013870: 2063 7572 7265 6e74 5f72 6164 6961 6c5f   current_radial_
+00013880: 616e 676c 6520 3d20 6e70 2e61 7361 7272  angle = np.asarr
+00013890: 6179 2863 7572 7265 6e74 5f72 6164 6961  ay(current_radia
+000138a0: 6c5f 616e 676c 6529 0d0a 2020 2020 2020  l_angle)..      
+000138b0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+000138c0: 7265 6e74 5f63 656c 6c5f 6178 6973 5f6d  rent_cell_axis_m
+000138d0: 6173 6b20 3d20 6e70 2e61 7361 7272 6179  ask = np.asarray
+000138e0: 2863 7572 7265 6e74 5f63 656c 6c5f 6178  (current_cell_ax
+000138f0: 6973 5f6d 6173 6b29 0d0a 0d0a 0d0a 2020  is_mask)......  
 00013900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013910: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-00013920: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00013930: 2020 2020 2020 2020 2020 2020 6966 2070              if p
-00013940: 6f69 6e74 5f73 616d 706c 6520 3e20 303a  oint_sample > 0:
-00013950: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013910: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00013920: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00013930: 2020 2020 2020 2020 2020 2069 6620 706f             if po
+00013940: 696e 745f 7361 6d70 6c65 203e 2030 3a0d  int_sample > 0:.
+00013950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00013960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013970: 2020 7866 5f73 616d 706c 6520 3d20 6666    xf_sample = ff
-00013980: 7466 7265 7128 706f 696e 745f 7361 6d70  tfreq(point_samp
-00013990: 6c65 2c20 7365 6c66 2e74 6361 6c69 6272  le, self.tcalibr
-000139a0: 6174 696f 6e29 0d0a 2020 2020 2020 2020  ation)..        
+00013970: 2078 665f 7361 6d70 6c65 203d 2066 6674   xf_sample = fft
+00013980: 6672 6571 2870 6f69 6e74 5f73 616d 706c  freq(point_sampl
+00013990: 652c 2073 656c 662e 7463 616c 6962 7261  e, self.tcalibra
+000139a0: 7469 6f6e 290d 0a20 2020 2020 2020 2020  tion)..         
 000139b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139c0: 2020 2020 2020 2020 6666 7473 7472 6970          fftstrip
-000139d0: 5f73 616d 706c 6520 3d20 6666 7428 6578  _sample = fft(ex
-000139e0: 7061 6e64 6564 5f69 6e74 656e 7369 7479  panded_intensity
-000139f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000139c0: 2020 2020 2020 2066 6674 7374 7269 705f         fftstrip_
+000139d0: 7361 6d70 6c65 203d 2066 6674 2865 7870  sample = fft(exp
+000139e0: 616e 6465 645f 696e 7465 6e73 6974 7929  anded_intensity)
+000139f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00013a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a10: 2020 2066 6674 746f 7461 6c5f 7361 6d70     ffttotal_samp
-00013a20: 6c65 203d 206e 702e 6162 7328 6666 7473  le = np.abs(ffts
-00013a30: 7472 6970 5f73 616d 706c 6529 0d0a 2020  trip_sample)..  
+00013a10: 2020 6666 7474 6f74 616c 5f73 616d 706c    ffttotal_sampl
+00013a20: 6520 3d20 6e70 2e61 6273 2866 6674 7374  e = np.abs(fftst
+00013a30: 7269 705f 7361 6d70 6c65 290d 0a20 2020  rip_sample)..   
 00013a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a50: 2020 2020 2020 2020 2020 2020 2020 7866                xf
-00013a60: 5f73 616d 706c 6520 3d20 7866 5f73 616d  _sample = xf_sam
-00013a70: 706c 655b 3020 3a20 6c65 6e28 7866 5f73  ple[0 : len(xf_s
-00013a80: 616d 706c 6529 202f 2f20 325d 0d0a 2020  ample) // 2]..  
+00013a50: 2020 2020 2020 2020 2020 2020 2078 665f               xf_
+00013a60: 7361 6d70 6c65 203d 2078 665f 7361 6d70  sample = xf_samp
+00013a70: 6c65 5b30 203a 206c 656e 2878 665f 7361  le[0 : len(xf_sa
+00013a80: 6d70 6c65 2920 2f2f 2032 5d0d 0a20 2020  mple) // 2]..   
 00013a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013aa0: 2020 2020 2020 2020 2020 2020 2020 6666                ff
-00013ab0: 7474 6f74 616c 5f73 616d 706c 6520 3d20  ttotal_sample = 
-00013ac0: 6666 7474 6f74 616c 5f73 616d 706c 655b  ffttotal_sample[
-00013ad0: 3020 3a20 6c65 6e28 6666 7474 6f74 616c  0 : len(ffttotal
-00013ae0: 5f73 616d 706c 6529 202f 2f20 325d 0d0a  _sample) // 2]..
-00013af0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00013b00: 2020 2020 2075 6e69 7175 655f 6666 745f       unique_fft_
-00013b10: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
-00013b20: 6c65 745b 6375 7272 656e 745f 756e 6971  let[current_uniq
-00013b30: 7565 5f69 645d 203d 2065 7870 616e 6465  ue_id] = expande
-00013b40: 645f 7469 6d65 2c20 6578 7061 6e64 6564  d_time, expanded
-00013b50: 5f69 6e74 656e 7369 7479 2c20 7866 5f73  _intensity, xf_s
-00013b60: 616d 706c 652c 2066 6674 746f 7461 6c5f  ample, ffttotal_
-00013b70: 7361 6d70 6c65 0d0a 2020 2020 2020 2020  sample..        
-00013b80: 2020 2020 2020 2020 2020 2075 6e69 7175             uniqu
-00013b90: 655f 636c 7573 7465 725f 7072 6f70 6572  e_cluster_proper
-00013ba0: 7469 6573 5f74 7261 636b 6c65 745b 6375  ties_tracklet[cu
-00013bb0: 7272 656e 745f 756e 6971 7565 5f69 645d  rrent_unique_id]
-00013bc0: 203d 2020 6375 7272 656e 745f 7469 6d65   =  current_time
-00013bd0: 2c20 6375 7272 656e 745f 636c 7573 7465  , current_cluste
-00013be0: 725f 636c 6173 732c 2063 7572 7265 6e74  r_class, current
-00013bf0: 5f63 6c75 7374 6572 5f63 6c61 7373 5f73  _cluster_class_s
-00013c00: 636f 7265 0d0a 2020 2020 2020 2020 2020  core..          
-00013c10: 2020 2020 2020 2020 2075 6e69 7175 655f           unique_
-00013c20: 7368 6170 655f 7072 6f70 6572 7469 6573  shape_properties
-00013c30: 5f74 7261 636b 6c65 745b 6375 7272 656e  _tracklet[curren
-00013c40: 745f 756e 6971 7565 5f69 645d 203d 2063  t_unique_id] = c
-00013c50: 7572 7265 6e74 5f74 696d 652c 2063 7572  urrent_time, cur
-00013c60: 7265 6e74 5f7a 2c20 6375 7272 656e 745f  rent_z, current_
-00013c70: 792c 2063 7572 7265 6e74 5f78 2c20 6375  y, current_x, cu
-00013c80: 7272 656e 745f 7261 6469 7573 2c20 6375  rrent_radius, cu
-00013c90: 7272 656e 745f 766f 6c75 6d65 2c20 6375  rrent_volume, cu
-00013ca0: 7272 656e 745f 6563 6365 6e74 7269 6369  rrent_eccentrici
-00013cb0: 7479 5f63 6f6d 705f 6669 7273 742c 2063  ty_comp_first, c
-00013cc0: 7572 7265 6e74 5f65 6363 656e 7472 6963  urrent_eccentric
-00013cd0: 6974 795f 636f 6d70 5f73 6563 6f6e 642c  ity_comp_second,
-00013ce0: 2063 7572 7265 6e74 5f73 7572 6661 6365   current_surface
-00013cf0: 5f61 7265 612c 2063 7572 7265 6e74 5f63  _area, current_c
-00013d00: 6c75 7374 6572 5f63 6c61 7373 2c20 6375  luster_class, cu
-00013d10: 7272 656e 745f 636c 7573 7465 725f 636c  rrent_cluster_cl
-00013d20: 6173 735f 7363 6f72 650d 0a20 2020 2020  ass_score..     
-00013d30: 2020 2020 2020 2020 2020 2020 2020 756e                un
-00013d40: 6971 7565 5f64 796e 616d 6963 5f70 726f  ique_dynamic_pro
-00013d50: 7065 7274 6965 735f 7472 6163 6b6c 6574  perties_tracklet
-00013d60: 5b63 7572 7265 6e74 5f75 6e69 7175 655f  [current_unique_
-00013d70: 6964 5d20 3d20 6375 7272 656e 745f 7469  id] = current_ti
-00013d80: 6d65 2c20 6375 7272 656e 745f 7370 6565  me, current_spee
-00013d90: 642c 2063 7572 7265 6e74 5f6d 6f74 696f  d, current_motio
-00013da0: 6e5f 616e 676c 652c 2063 7572 7265 6e74  n_angle, current
-00013db0: 5f61 6363 656c 6572 6174 696f 6e2c 2063  _acceleration, c
-00013dc0: 7572 7265 6e74 5f64 6973 7461 6e63 655f  urrent_distance_
-00013dd0: 6365 6c6c 5f6d 6173 6b2c 2063 7572 7265  cell_mask, curre
-00013de0: 6e74 5f72 6164 6961 6c5f 616e 676c 652c  nt_radial_angle,
-00013df0: 2063 7572 7265 6e74 5f63 656c 6c5f 6178   current_cell_ax
-00013e00: 6973 5f6d 6173 6b0d 0a20 2020 2020 2020  is_mask..       
-00013e10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00013e20: 2e75 6e69 7175 655f 6666 745f 7072 6f70  .unique_fft_prop
-00013e30: 6572 7469 6573 5b74 7261 636b 5f69 645d  erties[track_id]
-00013e40: 2e75 7064 6174 6528 7b63 7572 7265 6e74  .update({current
-00013e50: 5f75 6e69 7175 655f 6964 3a75 6e69 7175  _unique_id:uniqu
-00013e60: 655f 6666 745f 7072 6f70 6572 7469 6573  e_fft_properties
-00013e70: 5f74 7261 636b 6c65 745b 6375 7272 656e  _tracklet[curren
-00013e80: 745f 756e 6971 7565 5f69 645d 7d29 0d0a  t_unique_id]})..
+00013aa0: 2020 2020 2020 2020 2020 2020 2066 6674               fft
+00013ab0: 746f 7461 6c5f 7361 6d70 6c65 203d 2066  total_sample = f
+00013ac0: 6674 746f 7461 6c5f 7361 6d70 6c65 5b30  fttotal_sample[0
+00013ad0: 203a 206c 656e 2866 6674 746f 7461 6c5f   : len(ffttotal_
+00013ae0: 7361 6d70 6c65 2920 2f2f 2032 5d0d 0a0d  sample) // 2]...
+00013af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013b00: 2020 2020 756e 6971 7565 5f66 6674 5f70      unique_fft_p
+00013b10: 726f 7065 7274 6965 735f 7472 6163 6b6c  roperties_trackl
+00013b20: 6574 5b63 7572 7265 6e74 5f75 6e69 7175  et[current_uniqu
+00013b30: 655f 6964 5d20 3d20 6578 7061 6e64 6564  e_id] = expanded
+00013b40: 5f74 696d 652c 2065 7870 616e 6465 645f  _time, expanded_
+00013b50: 696e 7465 6e73 6974 792c 2078 665f 7361  intensity, xf_sa
+00013b60: 6d70 6c65 2c20 6666 7474 6f74 616c 5f73  mple, ffttotal_s
+00013b70: 616d 706c 650d 0a20 2020 2020 2020 2020  ample..         
+00013b80: 2020 2020 2020 2020 2020 756e 6971 7565            unique
+00013b90: 5f63 6c75 7374 6572 5f70 726f 7065 7274  _cluster_propert
+00013ba0: 6965 735f 7472 6163 6b6c 6574 5b63 7572  ies_tracklet[cur
+00013bb0: 7265 6e74 5f75 6e69 7175 655f 6964 5d20  rent_unique_id] 
+00013bc0: 3d20 2063 7572 7265 6e74 5f74 696d 652c  =  current_time,
+00013bd0: 2063 7572 7265 6e74 5f63 6c75 7374 6572   current_cluster
+00013be0: 5f63 6c61 7373 2c20 6375 7272 656e 745f  _class, current_
+00013bf0: 636c 7573 7465 725f 636c 6173 735f 7363  cluster_class_sc
+00013c00: 6f72 650d 0a20 2020 2020 2020 2020 2020  ore..           
+00013c10: 2020 2020 2020 2020 756e 6971 7565 5f73          unique_s
+00013c20: 6861 7065 5f70 726f 7065 7274 6965 735f  hape_properties_
+00013c30: 7472 6163 6b6c 6574 5b63 7572 7265 6e74  tracklet[current
+00013c40: 5f75 6e69 7175 655f 6964 5d20 3d20 6375  _unique_id] = cu
+00013c50: 7272 656e 745f 7469 6d65 2c20 6375 7272  rrent_time, curr
+00013c60: 656e 745f 7a2c 2063 7572 7265 6e74 5f79  ent_z, current_y
+00013c70: 2c20 6375 7272 656e 745f 782c 2063 7572  , current_x, cur
+00013c80: 7265 6e74 5f72 6164 6975 732c 2063 7572  rent_radius, cur
+00013c90: 7265 6e74 5f76 6f6c 756d 652c 2063 7572  rent_volume, cur
+00013ca0: 7265 6e74 5f65 6363 656e 7472 6963 6974  rent_eccentricit
+00013cb0: 795f 636f 6d70 5f66 6972 7374 2c20 6375  y_comp_first, cu
+00013cc0: 7272 656e 745f 6563 6365 6e74 7269 6369  rrent_eccentrici
+00013cd0: 7479 5f63 6f6d 705f 7365 636f 6e64 2c20  ty_comp_second, 
+00013ce0: 6375 7272 656e 745f 7375 7266 6163 655f  current_surface_
+00013cf0: 6172 6561 2c20 6375 7272 656e 745f 636c  area, current_cl
+00013d00: 7573 7465 725f 636c 6173 732c 2063 7572  uster_class, cur
+00013d10: 7265 6e74 5f63 6c75 7374 6572 5f63 6c61  rent_cluster_cla
+00013d20: 7373 5f73 636f 7265 0d0a 2020 2020 2020  ss_score..      
+00013d30: 2020 2020 2020 2020 2020 2020 2075 6e69               uni
+00013d40: 7175 655f 6479 6e61 6d69 635f 7072 6f70  que_dynamic_prop
+00013d50: 6572 7469 6573 5f74 7261 636b 6c65 745b  erties_tracklet[
+00013d60: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
+00013d70: 645d 203d 2063 7572 7265 6e74 5f74 696d  d] = current_tim
+00013d80: 652c 2063 7572 7265 6e74 5f73 7065 6564  e, current_speed
+00013d90: 2c20 6375 7272 656e 745f 6d6f 7469 6f6e  , current_motion
+00013da0: 5f61 6e67 6c65 2c20 6375 7272 656e 745f  _angle, current_
+00013db0: 6163 6365 6c65 7261 7469 6f6e 2c20 6375  acceleration, cu
+00013dc0: 7272 656e 745f 6469 7374 616e 6365 5f63  rrent_distance_c
+00013dd0: 656c 6c5f 6d61 736b 2c20 6375 7272 656e  ell_mask, curren
+00013de0: 745f 7261 6469 616c 5f61 6e67 6c65 2c20  t_radial_angle, 
+00013df0: 6375 7272 656e 745f 6365 6c6c 5f61 7869  current_cell_axi
+00013e00: 735f 6d61 736b 0d0a 2020 2020 2020 2020  s_mask..        
+00013e10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013e20: 756e 6971 7565 5f66 6674 5f70 726f 7065  unique_fft_prope
+00013e30: 7274 6965 735b 7472 6163 6b5f 6964 5d2e  rties[track_id].
+00013e40: 7570 6461 7465 287b 6375 7272 656e 745f  update({current_
+00013e50: 756e 6971 7565 5f69 643a 756e 6971 7565  unique_id:unique
+00013e60: 5f66 6674 5f70 726f 7065 7274 6965 735f  _fft_properties_
+00013e70: 7472 6163 6b6c 6574 5b63 7572 7265 6e74  tracklet[current
+00013e80: 5f75 6e69 7175 655f 6964 5d7d 290d 0a20  _unique_id]}).. 
 00013e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ea0: 2020 2073 656c 662e 756e 6971 7565 5f63     self.unique_c
-00013eb0: 6c75 7374 6572 5f70 726f 7065 7274 6965  luster_propertie
-00013ec0: 735b 7472 6163 6b5f 6964 5d2e 7570 6461  s[track_id].upda
-00013ed0: 7465 287b 6375 7272 656e 745f 756e 6971  te({current_uniq
-00013ee0: 7565 5f69 643a 756e 6971 7565 5f63 6c75  ue_id:unique_clu
-00013ef0: 7374 6572 5f70 726f 7065 7274 6965 735f  ster_properties_
-00013f00: 7472 6163 6b6c 6574 5b63 7572 7265 6e74  tracklet[current
-00013f10: 5f75 6e69 7175 655f 6964 5d7d 290d 0a0d  _unique_id]})...
-00013f20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013f30: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00013f40: 7368 6170 655f 7072 6f70 6572 7469 6573  shape_properties
-00013f50: 5b74 7261 636b 5f69 645d 2e75 7064 6174  [track_id].updat
-00013f60: 6528 7b63 7572 7265 6e74 5f75 6e69 7175  e({current_uniqu
-00013f70: 655f 6964 3a75 6e69 7175 655f 7368 6170  e_id:unique_shap
-00013f80: 655f 7072 6f70 6572 7469 6573 5f74 7261  e_properties_tra
-00013f90: 636b 6c65 745b 6375 7272 656e 745f 756e  cklet[current_un
-00013fa0: 6971 7565 5f69 645d 7d29 0d0a 2020 2020  ique_id]})..    
-00013fb0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00013fc0: 656c 662e 756e 6971 7565 5f64 796e 616d  elf.unique_dynam
-00013fd0: 6963 5f70 726f 7065 7274 6965 735b 7472  ic_properties[tr
-00013fe0: 6163 6b5f 6964 5d2e 7570 6461 7465 287b  ack_id].update({
-00013ff0: 6375 7272 656e 745f 756e 6971 7565 5f69  current_unique_i
-00014000: 643a 756e 6971 7565 5f64 796e 616d 6963  d:unique_dynamic
-00014010: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
-00014020: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
-00014030: 7175 655f 6964 5d7d 290d 0a0d 0a20 2020  que_id]})....   
-00014040: 2064 6566 205f 7365 636f 6e64 5f63 6861   def _second_cha
-00014050: 6e6e 656c 5f73 706f 7473 2873 656c 662c  nnel_spots(self,
-00014060: 2066 7261 6d65 2c20 7a2c 2079 2c20 782c   frame, z, y, x,
-00014070: 2063 656c 6c5f 6964 2c20 7472 6163 6b5f   cell_id, track_
-00014080: 6964 293a 0d0a 2020 2020 2020 2020 2020  id):..          
-00014090: 200d 0a20 2020 2020 2020 2020 2020 2074   ..            t
-000140a0: 7265 652c 2063 656e 7472 6f69 6473 2c20  ree, centroids, 
-000140b0: 6c61 6265 6c73 2c20 766f 6c75 6d65 2c20  labels, volume, 
-000140c0: 696e 7465 6e73 6974 795f 6d65 616e 2c20  intensity_mean, 
-000140d0: 696e 7465 6e73 6974 795f 746f 7461 6c2c  intensity_total,
-000140e0: 2062 6f75 6e64 696e 675f 626f 7865 7320   bounding_boxes 
-000140f0: 3d20 7365 6c66 2e5f 7469 6d65 645f 6368  = self._timed_ch
-00014100: 616e 6e65 6c5f 7365 675f 696d 6167 655b  annel_seg_image[
-00014110: 7374 7228 696e 7428 666c 6f61 7428 6672  str(int(float(fr
-00014120: 616d 6529 2929 5d0d 0a20 2020 2020 2020  ame)))]..       
-00014130: 2020 2020 2070 6978 656c 7465 7374 6c6f       pixeltestlo
-00014140: 6361 7469 6f6e 203d 2028 7a2c 792c 7829  cation = (z,y,x)
-00014150: 0d0a 2020 2020 2020 2020 2020 2020 6469  ..            di
-00014160: 7374 2c20 696e 6465 7820 3d20 7472 6565  st, index = tree
-00014170: 2e71 7565 7279 2870 6978 656c 7465 7374  .query(pixeltest
-00014180: 6c6f 6361 7469 6f6e 290d 0a0d 0a0d 0a20  location)...... 
-00014190: 2020 2020 2020 2020 2020 2062 626f 7820             bbox 
-000141a0: 3d20 626f 756e 6469 6e67 5f62 6f78 6573  = bounding_boxes
-000141b0: 5b69 6e64 6578 5d0d 0a20 2020 2020 2020  [index]..       
-000141c0: 2020 2020 2073 697a 657a 203d 2061 6273       sizez = abs
-000141d0: 2862 626f 785b 305d 202d 2062 626f 785b  (bbox[0] - bbox[
-000141e0: 335d 290d 0a20 2020 2020 2020 2020 2020  3])..           
-000141f0: 2073 697a 6579 203d 2061 6273 2862 626f   sizey = abs(bbo
-00014200: 785b 315d 202d 2062 626f 785b 345d 290d  x[1] - bbox[4]).
-00014210: 0a20 2020 2020 2020 2020 2020 2073 697a  .            siz
-00014220: 6578 203d 2061 6273 2862 626f 785b 325d  ex = abs(bbox[2]
-00014230: 202d 2062 626f 785b 355d 2920 0d0a 2020   - bbox[5]) ..  
-00014240: 2020 2020 2020 2020 2020 7665 746f 5f76            veto_v
-00014250: 6f6c 756d 6520 3d20 7369 7a65 7820 2a20  olume = sizex * 
-00014260: 7369 7a65 7920 2a20 7369 7a65 7a0d 0a20  sizey * sizez.. 
-00014270: 2020 2020 2020 2020 2020 2076 6574 6f5f             veto_
-00014280: 7261 6469 7573 203d 206d 6174 682e 706f  radius = math.po
-00014290: 7728 3320 2a20 7665 746f 5f76 6f6c 756d  w(3 * veto_volum
-000142a0: 6520 2f20 2834 202a 206d 6174 682e 7069  e / (4 * math.pi
-000142b0: 292c 2031 2e30 202f 2033 2e30 290d 0a0d  ), 1.0 / 3.0)...
-000142c0: 0a20 2020 2020 2020 2020 2020 206c 6f63  .            loc
-000142d0: 6174 696f 6e20 3d20 2863 656e 7472 6f69  ation = (centroi
-000142e0: 6473 5b69 6e64 6578 5d5b 305d 202a 2073  ds[index][0] * s
-000142f0: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
-00014300: 2c20 6365 6e74 726f 6964 735b 696e 6465  , centroids[inde
-00014310: 785d 5b31 5d2a 7365 6c66 2e79 6361 6c69  x][1]*self.ycali
-00014320: 6272 6174 696f 6e2c 2063 656e 7472 6f69  bration, centroi
-00014330: 6473 5b69 6e64 6578 5d5b 325d 2a73 656c  ds[index][2]*sel
-00014340: 662e 7863 616c 6962 7261 7469 6f6e 290d  f.xcalibration).
-00014350: 0a20 2020 2020 2020 2020 2020 2051 5541  .            QUA
-00014360: 4c49 5459 203d 2076 6f6c 756d 655b 696e  LITY = volume[in
-00014370: 6465 785d 0d0a 2020 2020 2020 2020 2020  dex]..          
-00014380: 2020 5241 4449 5553 203d 206d 6174 682e    RADIUS = math.
-00014390: 706f 7728 5155 414c 4954 592c 2031 2e30  pow(QUALITY, 1.0
-000143a0: 2f33 2e30 2920 2a20 7365 6c66 2e78 6361  /3.0) * self.xca
-000143b0: 6c69 6272 6174 696f 6e20 2a20 7365 6c66  libration * self
-000143c0: 2e79 6361 6c69 6272 6174 696f 6e20 2a20  .ycalibration * 
-000143d0: 7365 6c66 2e7a 6361 6c69 6272 6174 696f  self.zcalibratio
-000143e0: 6e0d 0a20 2020 2020 2020 2020 2020 2064  n..            d
-000143f0: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00014400: 6b2c 206d 6173 6b63 656e 7472 6f69 6420  k, maskcentroid 
-00014410: 3d20 7365 6c66 2e5f 6765 745f 626f 756e  = self._get_boun
-00014420: 6461 7279 5f64 6973 7428 6672 616d 652c  dary_dist(frame,
-00014430: 206c 6f63 6174 696f 6e2c 2052 4144 4955   location, RADIU
-00014440: 5329 0d0a 2020 2020 2020 2020 2020 2020  S)..            
-00014450: 6966 2064 6973 7420 3c3d 2076 6574 6f5f  if dist <= veto_
-00014460: 7261 6469 7573 3a0d 0a20 2020 2020 2020  radius:..       
-00014470: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
-00014480: 616e 6e65 6c5f 756e 6971 7565 5f73 706f  annel_unique_spo
-00014490: 745f 7072 6f70 6572 7469 6573 5b63 656c  t_properties[cel
-000144a0: 6c5f 6964 5d20 3d20 7b0d 0a20 2020 2020  l_id] = {..     
+00013ea0: 2020 7365 6c66 2e75 6e69 7175 655f 636c    self.unique_cl
+00013eb0: 7573 7465 725f 7072 6f70 6572 7469 6573  uster_properties
+00013ec0: 5b74 7261 636b 5f69 645d 2e75 7064 6174  [track_id].updat
+00013ed0: 6528 7b63 7572 7265 6e74 5f75 6e69 7175  e({current_uniqu
+00013ee0: 655f 6964 3a75 6e69 7175 655f 636c 7573  e_id:unique_clus
+00013ef0: 7465 725f 7072 6f70 6572 7469 6573 5f74  ter_properties_t
+00013f00: 7261 636b 6c65 745b 6375 7272 656e 745f  racklet[current_
+00013f10: 756e 6971 7565 5f69 645d 7d29 0d0a 0d0a  unique_id]})....
+00013f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f30: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
+00013f40: 6861 7065 5f70 726f 7065 7274 6965 735b  hape_properties[
+00013f50: 7472 6163 6b5f 6964 5d2e 7570 6461 7465  track_id].update
+00013f60: 287b 6375 7272 656e 745f 756e 6971 7565  ({current_unique
+00013f70: 5f69 643a 756e 6971 7565 5f73 6861 7065  _id:unique_shape
+00013f80: 5f70 726f 7065 7274 6965 735f 7472 6163  _properties_trac
+00013f90: 6b6c 6574 5b63 7572 7265 6e74 5f75 6e69  klet[current_uni
+00013fa0: 7175 655f 6964 5d7d 290d 0a20 2020 2020  que_id]})..     
+00013fb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00013fc0: 6c66 2e75 6e69 7175 655f 6479 6e61 6d69  lf.unique_dynami
+00013fd0: 635f 7072 6f70 6572 7469 6573 5b74 7261  c_properties[tra
+00013fe0: 636b 5f69 645d 2e75 7064 6174 6528 7b63  ck_id].update({c
+00013ff0: 7572 7265 6e74 5f75 6e69 7175 655f 6964  urrent_unique_id
+00014000: 3a75 6e69 7175 655f 6479 6e61 6d69 635f  :unique_dynamic_
+00014010: 7072 6f70 6572 7469 6573 5f74 7261 636b  properties_track
+00014020: 6c65 745b 6375 7272 656e 745f 756e 6971  let[current_uniq
+00014030: 7565 5f69 645d 7d29 0d0a 0d0a 2020 2020  ue_id]})....    
+00014040: 6465 6620 5f73 6563 6f6e 645f 6368 616e  def _second_chan
+00014050: 6e65 6c5f 7370 6f74 7328 7365 6c66 2c20  nel_spots(self, 
+00014060: 6672 616d 652c 207a 2c20 792c 2078 2c20  frame, z, y, x, 
+00014070: 6365 6c6c 5f69 642c 2074 7261 636b 5f69  cell_id, track_i
+00014080: 6429 3a0d 0a20 2020 2020 2020 2020 2020  d):..           
+00014090: 0d0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
+000140a0: 6565 2c20 6365 6e74 726f 6964 732c 206c  ee, centroids, l
+000140b0: 6162 656c 732c 2076 6f6c 756d 652c 2069  abels, volume, i
+000140c0: 6e74 656e 7369 7479 5f6d 6561 6e2c 2069  ntensity_mean, i
+000140d0: 6e74 656e 7369 7479 5f74 6f74 616c 2c20  ntensity_total, 
+000140e0: 626f 756e 6469 6e67 5f62 6f78 6573 203d  bounding_boxes =
+000140f0: 2073 656c 662e 5f74 696d 6564 5f63 6861   self._timed_cha
+00014100: 6e6e 656c 5f73 6567 5f69 6d61 6765 5b73  nnel_seg_image[s
+00014110: 7472 2869 6e74 2866 6c6f 6174 2866 7261  tr(int(float(fra
+00014120: 6d65 2929 295d 0d0a 2020 2020 2020 2020  me)))]..        
+00014130: 2020 2020 7069 7865 6c74 6573 746c 6f63      pixeltestloc
+00014140: 6174 696f 6e20 3d20 287a 2c79 2c78 290d  ation = (z,y,x).
+00014150: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
+00014160: 742c 2069 6e64 6578 203d 2074 7265 652e  t, index = tree.
+00014170: 7175 6572 7928 7069 7865 6c74 6573 746c  query(pixeltestl
+00014180: 6f63 6174 696f 6e29 0d0a 0d0a 0d0a 2020  ocation)......  
+00014190: 2020 2020 2020 2020 2020 6262 6f78 203d            bbox =
+000141a0: 2062 6f75 6e64 696e 675f 626f 7865 735b   bounding_boxes[
+000141b0: 696e 6465 785d 0d0a 2020 2020 2020 2020  index]..        
+000141c0: 2020 2020 7369 7a65 7a20 3d20 6162 7328      sizez = abs(
+000141d0: 6262 6f78 5b30 5d20 2d20 6262 6f78 5b33  bbox[0] - bbox[3
+000141e0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+000141f0: 7369 7a65 7920 3d20 6162 7328 6262 6f78  sizey = abs(bbox
+00014200: 5b31 5d20 2d20 6262 6f78 5b34 5d29 0d0a  [1] - bbox[4])..
+00014210: 2020 2020 2020 2020 2020 2020 7369 7a65              size
+00014220: 7820 3d20 6162 7328 6262 6f78 5b32 5d20  x = abs(bbox[2] 
+00014230: 2d20 6262 6f78 5b35 5d29 200d 0a20 2020  - bbox[5]) ..   
+00014240: 2020 2020 2020 2020 2076 6574 6f5f 766f           veto_vo
+00014250: 6c75 6d65 203d 2073 697a 6578 202a 2073  lume = sizex * s
+00014260: 697a 6579 202a 2073 697a 657a 0d0a 2020  izey * sizez..  
+00014270: 2020 2020 2020 2020 2020 7665 746f 5f72            veto_r
+00014280: 6164 6975 7320 3d20 6d61 7468 2e70 6f77  adius = math.pow
+00014290: 2833 202a 2076 6574 6f5f 766f 6c75 6d65  (3 * veto_volume
+000142a0: 202f 2028 3420 2a20 6d61 7468 2e70 6929   / (4 * math.pi)
+000142b0: 2c20 312e 3020 2f20 332e 3029 0d0a 0d0a  , 1.0 / 3.0)....
+000142c0: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
+000142d0: 7469 6f6e 203d 2028 6365 6e74 726f 6964  tion = (centroid
+000142e0: 735b 696e 6465 785d 5b30 5d20 2a20 7365  s[index][0] * se
+000142f0: 6c66 2e7a 6361 6c69 6272 6174 696f 6e2c  lf.zcalibration,
+00014300: 2063 656e 7472 6f69 6473 5b69 6e64 6578   centroids[index
+00014310: 5d5b 315d 2a73 656c 662e 7963 616c 6962  ][1]*self.ycalib
+00014320: 7261 7469 6f6e 2c20 6365 6e74 726f 6964  ration, centroid
+00014330: 735b 696e 6465 785d 5b32 5d2a 7365 6c66  s[index][2]*self
+00014340: 2e78 6361 6c69 6272 6174 696f 6e29 0d0a  .xcalibration)..
+00014350: 2020 2020 2020 2020 2020 2020 5155 414c              QUAL
+00014360: 4954 5920 3d20 766f 6c75 6d65 5b69 6e64  ITY = volume[ind
+00014370: 6578 5d0d 0a20 2020 2020 2020 2020 2020  ex]..           
+00014380: 2052 4144 4955 5320 3d20 6d61 7468 2e70   RADIUS = math.p
+00014390: 6f77 2851 5541 4c49 5459 2c20 312e 302f  ow(QUALITY, 1.0/
+000143a0: 332e 3029 202a 2073 656c 662e 7863 616c  3.0) * self.xcal
+000143b0: 6962 7261 7469 6f6e 202a 2073 656c 662e  ibration * self.
+000143c0: 7963 616c 6962 7261 7469 6f6e 202a 2073  ycalibration * s
+000143d0: 656c 662e 7a63 616c 6962 7261 7469 6f6e  elf.zcalibration
+000143e0: 0d0a 2020 2020 2020 2020 2020 2020 6469  ..            di
+000143f0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00014400: 2c20 6d61 736b 6365 6e74 726f 6964 203d  , maskcentroid =
+00014410: 2073 656c 662e 5f67 6574 5f62 6f75 6e64   self._get_bound
+00014420: 6172 795f 6469 7374 2866 7261 6d65 2c20  ary_dist(frame, 
+00014430: 6c6f 6361 7469 6f6e 2c20 5241 4449 5553  location, RADIUS
+00014440: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00014450: 6620 6469 7374 203c 3d20 3220 2a20 7665  f dist <= 2 * ve
+00014460: 746f 5f72 6164 6975 733a 0d0a 2020 2020  to_radius:..    
+00014470: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00014480: 2e63 6861 6e6e 656c 5f75 6e69 7175 655f  .channel_unique_
+00014490: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000144a0: 6365 6c6c 5f69 645d 203d 207b 0d0a 2020  cell_id] = {..  
 000144b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144c0: 2020 2073 656c 662e 6365 6c6c 6964 5f6b     self.cellid_k
-000144d0: 6579 3a20 696e 7428 6365 6c6c 5f69 6429  ey: int(cell_id)
-000144e0: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
-000144f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014500: 2e66 7261 6d65 6964 5f6b 6579 203a 2069  .frameid_key : i
-00014510: 6e74 2866 7261 6d65 292c 0d0a 2020 2020  nt(frame),..    
+000144c0: 2020 2020 2020 7365 6c66 2e63 656c 6c69        self.celli
+000144d0: 645f 6b65 793a 2069 6e74 2863 656c 6c5f  d_key: int(cell_
+000144e0: 6964 292c 200d 0a20 2020 2020 2020 2020  id), ..         
+000144f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014500: 656c 662e 6672 616d 6569 645f 6b65 7920  elf.frameid_key 
+00014510: 3a20 696e 7428 6672 616d 6529 2c0d 0a20  : int(frame),.. 
 00014520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014530: 2020 2020 7365 6c66 2e7a 706f 7369 645f      self.zposid_
-00014540: 6b65 7920 3a20 666c 6f61 7428 6365 6e74  key : float(cent
-00014550: 726f 6964 735b 696e 6465 785d 5b30 5d2a  roids[index][0]*
-00014560: 2073 656c 662e 7a63 616c 6962 7261 7469   self.zcalibrati
-00014570: 6f6e 292c 0d0a 2020 2020 2020 2020 2020  on),..          
-00014580: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00014590: 6c66 2e79 706f 7369 645f 6b65 7920 3a20  lf.yposid_key : 
-000145a0: 666c 6f61 7428 6365 6e74 726f 6964 735b  float(centroids[
-000145b0: 696e 6465 785d 5b31 5d2a 2073 656c 662e  index][1]* self.
-000145c0: 7963 616c 6962 7261 7469 6f6e 292c 0d0a  ycalibration),..
-000145d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145e0: 2020 2020 2020 2020 7365 6c66 2e78 706f          self.xpo
-000145f0: 7369 645f 6b65 7920 3a20 666c 6f61 7428  sid_key : float(
-00014600: 6365 6e74 726f 6964 735b 696e 6465 785d  centroids[index]
-00014610: 5b32 5d2a 2073 656c 662e 7863 616c 6962  [2]* self.xcalib
-00014620: 7261 7469 6f6e 292c 0d0a 2020 2020 2020  ration),..      
+00014530: 2020 2020 2020 2073 656c 662e 7a70 6f73         self.zpos
+00014540: 6964 5f6b 6579 203a 2066 6c6f 6174 2863  id_key : float(c
+00014550: 656e 7472 6f69 6473 5b69 6e64 6578 5d5b  entroids[index][
+00014560: 305d 2a20 7365 6c66 2e7a 6361 6c69 6272  0]* self.zcalibr
+00014570: 6174 696f 6e29 2c0d 0a20 2020 2020 2020  ation),..       
+00014580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014590: 2073 656c 662e 7970 6f73 6964 5f6b 6579   self.yposid_key
+000145a0: 203a 2066 6c6f 6174 2863 656e 7472 6f69   : float(centroi
+000145b0: 6473 5b69 6e64 6578 5d5b 315d 2a20 7365  ds[index][1]* se
+000145c0: 6c66 2e79 6361 6c69 6272 6174 696f 6e29  lf.ycalibration)
+000145d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000145e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000145f0: 7870 6f73 6964 5f6b 6579 203a 2066 6c6f  xposid_key : flo
+00014600: 6174 2863 656e 7472 6f69 6473 5b69 6e64  at(centroids[ind
+00014610: 6578 5d5b 325d 2a20 7365 6c66 2e78 6361  ex][2]* self.xca
+00014620: 6c69 6272 6174 696f 6e29 2c0d 0a20 2020  libration),..   
 00014630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014640: 2020 7365 6c66 2e74 7261 636b 6964 5f6b    self.trackid_k
-00014650: 6579 3a20 696e 7428 7472 6163 6b5f 6964  ey: int(track_id
-00014660: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-00014670: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014680: 2e74 6f74 616c 5f69 6e74 656e 7369 7479  .total_intensity
-00014690: 5f6b 6579 203a 2028 666c 6f61 7428 696e  _key : (float(in
-000146a0: 7465 6e73 6974 795f 746f 7461 6c5b 696e  tensity_total[in
-000146b0: 6465 785d 2929 2c0d 0a20 2020 2020 2020  dex])),..       
+00014640: 2020 2020 2073 656c 662e 7472 6163 6b69       self.tracki
+00014650: 645f 6b65 793a 2069 6e74 2874 7261 636b  d_key: int(track
+00014660: 5f69 6429 2c0d 0a20 2020 2020 2020 2020  _id),..         
+00014670: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014680: 656c 662e 746f 7461 6c5f 696e 7465 6e73  elf.total_intens
+00014690: 6974 795f 6b65 7920 3a20 2866 6c6f 6174  ity_key : (float
+000146a0: 2869 6e74 656e 7369 7479 5f74 6f74 616c  (intensity_total
+000146b0: 5b69 6e64 6578 5d29 292c 0d0a 2020 2020  [index])),..    
 000146c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146d0: 2073 656c 662e 6d65 616e 5f69 6e74 656e   self.mean_inten
-000146e0: 7369 7479 5f6b 6579 203a 2028 666c 6f61  sity_key : (floa
-000146f0: 7428 696e 7465 6e73 6974 795f 6d65 616e  t(intensity_mean
-00014700: 5b69 6e64 6578 5d29 292c 0d0a 0d0a 2020  [index])),....  
-00014710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014720: 2020 2020 2020 7365 6c66 2e72 6164 6975        self.radiu
-00014730: 735f 6b65 7920 3a20 2866 6c6f 6174 2852  s_key : (float(R
-00014740: 4144 4955 5329 292c 0d0a 2020 2020 2020  ADIUS)),..      
+000146d0: 2020 2020 7365 6c66 2e6d 6561 6e5f 696e      self.mean_in
+000146e0: 7465 6e73 6974 795f 6b65 7920 3a20 2866  tensity_key : (f
+000146f0: 6c6f 6174 2869 6e74 656e 7369 7479 5f6d  loat(intensity_m
+00014700: 6561 6e5b 696e 6465 785d 2929 2c0d 0a0d  ean[index])),...
+00014710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014720: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
+00014730: 6469 7573 5f6b 6579 203a 2028 666c 6f61  dius_key : (floa
+00014740: 7428 5241 4449 5553 2929 2c0d 0a20 2020  t(RADIUS)),..   
 00014750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014760: 2020 7365 6c66 2e71 7561 6c69 7479 5f6b    self.quality_k
-00014770: 6579 203a 2028 666c 6f61 7428 5155 414c  ey : (float(QUAL
-00014780: 4954 5929 292c 0d0a 2020 2020 2020 2020  ITY)),..        
+00014760: 2020 2020 2073 656c 662e 7175 616c 6974       self.qualit
+00014770: 795f 6b65 7920 3a20 2866 6c6f 6174 2851  y_key : (float(Q
+00014780: 5541 4c49 5459 2929 2c0d 0a20 2020 2020  UALITY)),..     
 00014790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147a0: 7365 6c66 2e64 6973 7461 6e63 655f 6365  self.distance_ce
-000147b0: 6c6c 5f6d 6173 6b5f 6b65 793a 2066 6c6f  ll_mask_key: flo
-000147c0: 6174 2864 6973 7461 6e63 655f 6365 6c6c  at(distance_cell
-000147d0: 5f6d 6173 6b29 2c0d 0a20 2020 2020 2020  _mask),..       
+000147a0: 2020 2073 656c 662e 6469 7374 616e 6365     self.distance
+000147b0: 5f63 656c 6c5f 6d61 736b 5f6b 6579 3a20  _cell_mask_key: 
+000147c0: 666c 6f61 7428 6469 7374 616e 6365 5f63  float(distance_c
+000147d0: 656c 6c5f 6d61 736b 292c 0d0a 2020 2020  ell_mask),..    
 000147e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147f0: 2073 656c 662e 6d61 736b 6365 6e74 726f   self.maskcentro
-00014800: 6964 5f7a 5f6b 6579 3a20 666c 6f61 7428  id_z_key: float(
-00014810: 6d61 736b 6365 6e74 726f 6964 5b30 5d29  maskcentroid[0])
-00014820: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00014830: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014840: 6d61 736b 6365 6e74 726f 6964 5f79 5f6b  maskcentroid_y_k
-00014850: 6579 3a20 666c 6f61 7428 6d61 736b 6365  ey: float(maskce
-00014860: 6e74 726f 6964 5b31 5d29 2c0d 0a20 2020  ntroid[1]),..   
+000147f0: 2020 2020 7365 6c66 2e6d 6173 6b63 656e      self.maskcen
+00014800: 7472 6f69 645f 7a5f 6b65 793a 2066 6c6f  troid_z_key: flo
+00014810: 6174 286d 6173 6b63 656e 7472 6f69 645b  at(maskcentroid[
+00014820: 305d 292c 0d0a 2020 2020 2020 2020 2020  0]),..          
+00014830: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00014840: 6c66 2e6d 6173 6b63 656e 7472 6f69 645f  lf.maskcentroid_
+00014850: 795f 6b65 793a 2066 6c6f 6174 286d 6173  y_key: float(mas
+00014860: 6b63 656e 7472 6f69 645b 315d 292c 0d0a  kcentroid[1]),..
 00014870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014880: 2020 2020 2073 656c 662e 6d61 736b 6365       self.maskce
-00014890: 6e74 726f 6964 5f78 5f6b 6579 3a20 666c  ntroid_x_key: fl
-000148a0: 6f61 7428 6d61 736b 6365 6e74 726f 6964  oat(maskcentroid
-000148b0: 5b32 5d29 200d 0a0d 0a20 2020 2020 2020  [2]) ....       
-000148c0: 2020 2020 2020 2020 207d 200d 0a20 2020           } ..   
+00014880: 2020 2020 2020 2020 7365 6c66 2e6d 6173          self.mas
+00014890: 6b63 656e 7472 6f69 645f 785f 6b65 793a  kcentroid_x_key:
+000148a0: 2066 6c6f 6174 286d 6173 6b63 656e 7472   float(maskcentr
+000148b0: 6f69 645b 325d 2920 0d0a 0d0a 2020 2020  oid[2]) ....    
+000148c0: 2020 2020 2020 2020 2020 2020 7d20 0d0a              } ..
 000148d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148e0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-000148f0: 2020 2020 6465 6620 5f64 6963 745f 7570      def _dict_up
-00014900: 6461 7465 2873 656c 662c 2075 6e69 7175  date(self, uniqu
-00014910: 655f 7472 6163 6b6c 6574 5f69 6473 3a20  e_tracklet_ids: 
-00014920: 4c69 7374 2c20 2063 656c 6c5f 6964 3a20  List,  cell_id: 
-00014930: 696e 742c 2074 7261 636b 5f69 643a 2069  int, track_id: i
-00014940: 6e74 2c20 736f 7572 6365 5f69 643a 2069  nt, source_id: i
-00014950: 6e74 2c20 7461 7267 6574 5f69 643a 2069  nt, target_id: i
-00014960: 6e74 293a 0d0a 0d0a 200d 0a20 2020 2020  nt):.... ..     
-00014970: 2020 2067 656e 6572 6174 696f 6e5f 6964     generation_id
-00014980: 203d 2073 656c 662e 6765 6e65 7261 7469   = self.generati
-00014990: 6f6e 5f64 6963 745b 6365 6c6c 5f69 645d  on_dict[cell_id]
-000149a0: 0d0a 2020 2020 2020 2020 7472 6163 6b6c  ..        trackl
-000149b0: 6574 5f69 6420 3d20 7365 6c66 2e74 7261  et_id = self.tra
-000149c0: 636b 6c65 745f 6469 6374 5b63 656c 6c5f  cklet_dict[cell_
-000149d0: 6964 5d0d 0a0d 0a20 2020 2020 2020 2075  id]....        u
-000149e0: 6e69 7175 655f 6964 203d 2073 7472 2874  nique_id = str(t
-000149f0: 7261 636b 5f69 6429 202b 2073 7472 2873  rack_id) + str(s
-00014a00: 656c 662e 6d61 785f 7472 6163 6b5f 6964  elf.max_track_id
-00014a10: 2920 2b20 7374 7228 6765 6e65 7261 7469  ) + str(generati
-00014a20: 6f6e 5f69 6429 202b 2073 7472 2874 7261  on_id) + str(tra
-00014a30: 636b 6c65 745f 6964 290d 0a20 2020 2020  cklet_id)..     
-00014a40: 2020 200d 0a20 2020 2020 2020 2076 6563     ..        vec
-00014a50: 5f6d 6173 6b20 3d20 5b66 6c6f 6174 2873  _mask = [float(s
-00014a60: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00014a70: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00014a80: 656c 6c5f 6964 295d 5b73 656c 662e 6d61  ell_id)][self.ma
-00014a90: 736b 6365 6e74 726f 6964 5f78 5f6b 6579  skcentroid_x_key
-00014aa0: 5d29 2c20 666c 6f61 7428 7365 6c66 2e75  ]), float(self.u
-00014ab0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00014ac0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00014ad0: 6429 5d5b 7365 6c66 2e6d 6173 6b63 656e  d)][self.maskcen
-00014ae0: 7472 6f69 645f 795f 6b65 795d 292c 2066  troid_y_key]), f
-00014af0: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
-00014b00: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00014b10: 5b69 6e74 2863 656c 6c5f 6964 295d 5b73  [int(cell_id)][s
-00014b20: 656c 662e 6d61 736b 6365 6e74 726f 6964  elf.maskcentroid
-00014b30: 5f7a 5f6b 6579 5d29 205d 0d0a 0d0a 2020  _z_key]) ]....  
-00014b40: 2020 2020 2020 7665 635f 6365 6c6c 203d        vec_cell =
-00014b50: 205b 666c 6f61 7428 7365 6c66 2e75 6e69   [float(self.uni
-00014b60: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00014b70: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00014b80: 5d5b 7365 6c66 2e78 706f 7369 645f 6b65  ][self.xposid_ke
-00014b90: 795d 2920 2c20 0d0a 2020 2020 2020 2020  y]) , ..        
+000148e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148f0: 200d 0a20 2020 2064 6566 205f 6469 6374   ..    def _dict
+00014900: 5f75 7064 6174 6528 7365 6c66 2c20 756e  _update(self, un
+00014910: 6971 7565 5f74 7261 636b 6c65 745f 6964  ique_tracklet_id
+00014920: 733a 204c 6973 742c 2020 6365 6c6c 5f69  s: List,  cell_i
+00014930: 643a 2069 6e74 2c20 7472 6163 6b5f 6964  d: int, track_id
+00014940: 3a20 696e 742c 2073 6f75 7263 655f 6964  : int, source_id
+00014950: 3a20 696e 742c 2074 6172 6765 745f 6964  : int, target_id
+00014960: 3a20 696e 7429 3a0d 0a0d 0a20 0d0a 2020  : int):.... ..  
+00014970: 2020 2020 2020 6765 6e65 7261 7469 6f6e        generation
+00014980: 5f69 6420 3d20 7365 6c66 2e67 656e 6572  _id = self.gener
+00014990: 6174 696f 6e5f 6469 6374 5b63 656c 6c5f  ation_dict[cell_
+000149a0: 6964 5d0d 0a20 2020 2020 2020 2074 7261  id]..        tra
+000149b0: 636b 6c65 745f 6964 203d 2073 656c 662e  cklet_id = self.
+000149c0: 7472 6163 6b6c 6574 5f64 6963 745b 6365  tracklet_dict[ce
+000149d0: 6c6c 5f69 645d 0d0a 0d0a 2020 2020 2020  ll_id]....      
+000149e0: 2020 756e 6971 7565 5f69 6420 3d20 7374    unique_id = st
+000149f0: 7228 7472 6163 6b5f 6964 2920 2b20 7374  r(track_id) + st
+00014a00: 7228 7365 6c66 2e6d 6178 5f74 7261 636b  r(self.max_track
+00014a10: 5f69 6429 202b 2073 7472 2867 656e 6572  _id) + str(gener
+00014a20: 6174 696f 6e5f 6964 2920 2b20 7374 7228  ation_id) + str(
+00014a30: 7472 6163 6b6c 6574 5f69 6429 0d0a 2020  tracklet_id)..  
+00014a40: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00014a50: 7665 635f 6d61 736b 203d 205b 666c 6f61  vec_mask = [floa
+00014a60: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
+00014a70: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00014a80: 7428 6365 6c6c 5f69 6429 5d5b 7365 6c66  t(cell_id)][self
+00014a90: 2e6d 6173 6b63 656e 7472 6f69 645f 785f  .maskcentroid_x_
+00014aa0: 6b65 795d 292c 2066 6c6f 6174 2873 656c  key]), float(sel
+00014ab0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00014ac0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+00014ad0: 6c5f 6964 295d 5b73 656c 662e 6d61 736b  l_id)][self.mask
+00014ae0: 6365 6e74 726f 6964 5f79 5f6b 6579 5d29  centroid_y_key])
+00014af0: 2c20 666c 6f61 7428 7365 6c66 2e75 6e69  , float(self.uni
+00014b00: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00014b10: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00014b20: 5d5b 7365 6c66 2e6d 6173 6b63 656e 7472  ][self.maskcentr
+00014b30: 6f69 645f 7a5f 6b65 795d 2920 5d0d 0a0d  oid_z_key]) ]...
+00014b40: 0a20 2020 2020 2020 2076 6563 5f63 656c  .        vec_cel
+00014b50: 6c20 3d20 5b66 6c6f 6174 2873 656c 662e  l = [float(self.
+00014b60: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00014b70: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00014b80: 6964 295d 5b73 656c 662e 7870 6f73 6964  id)][self.xposid
+00014b90: 5f6b 6579 5d29 202c 200d 0a20 2020 2020  _key]) , ..     
 00014ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014bb0: 2020 2020 666c 6f61 7428 7365 6c66 2e75      float(self.u
-00014bc0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
-00014bd0: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
-00014be0: 6429 5d5b 7365 6c66 2e79 706f 7369 645f  d)][self.yposid_
-00014bf0: 6b65 795d 292c 200d 0a20 2020 2020 2020  key]), ..       
+00014bb0: 2020 2020 2020 2066 6c6f 6174 2873 656c         float(sel
+00014bc0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
+00014bd0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
+00014be0: 6c5f 6964 295d 5b73 656c 662e 7970 6f73  l_id)][self.ypos
+00014bf0: 6964 5f6b 6579 5d29 2c20 0d0a 2020 2020  id_key]), ..    
 00014c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c10: 2020 2020 2066 6c6f 6174 2873 656c 662e       float(self.
-00014c20: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00014c30: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00014c40: 6964 295d 5b73 656c 662e 7a70 6f73 6964  id)][self.zposid
-00014c50: 5f6b 6579 5d29 5d0d 0a0d 0a20 2020 2020  _key])]....     
-00014c60: 2020 2061 6e67 6c65 203d 2061 6e67 756c     angle = angul
-00014c70: 6172 5f63 6861 6e67 6528 7665 635f 6d61  ar_change(vec_ma
-00014c80: 736b 2c20 7665 635f 6365 6c6c 290d 0a0d  sk, vec_cell)...
-00014c90: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
-00014ca0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00014cb0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00014cc0: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00014cd0: 7261 6469 616c 5f61 6e67 6c65 5f6b 6579  radial_angle_key
-00014ce0: 203a 2061 6e67 6c65 7d29 2020 2020 2020   : angle})      
-00014cf0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00014d00: 0d0a 2020 2020 2020 2020 756e 6971 7565  ..        unique
-00014d10: 5f74 7261 636b 6c65 745f 6964 732e 6170  _tracklet_ids.ap
-00014d20: 7065 6e64 2873 7472 2875 6e69 7175 655f  pend(str(unique_
-00014d30: 6964 2929 0d0a 2020 2020 2020 2020 7365  id))..        se
-00014d40: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00014d50: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00014d60: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00014d70: 7365 6c66 2e63 6c75 7374 6572 636c 6173  self.clusterclas
-00014d80: 735f 6b65 7920 3a20 4e6f 6e65 7d29 0d0a  s_key : None})..
-00014d90: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00014da0: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00014db0: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00014dc0: 5d2e 7570 6461 7465 287b 7365 6c66 2e63  ].update({self.c
-00014dd0: 6c75 7374 6572 7363 6f72 655f 6b65 7920  lusterscore_key 
-00014de0: 3a20 307d 290d 0a20 2020 2020 2020 2073  : 0})..        s
-00014df0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00014e00: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00014e10: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-00014e20: 7b73 656c 662e 756e 6971 7565 6964 5f6b  {self.uniqueid_k
-00014e30: 6579 203a 2073 7472 2875 6e69 7175 655f  ey : str(unique_
-00014e40: 6964 297d 290d 0a20 2020 2020 2020 2073  id)})..        s
-00014e50: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00014e60: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-00014e70: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-00014e80: 7b73 656c 662e 7472 6163 6b6c 6574 6964  {self.trackletid
-00014e90: 5f6b 6579 203a 2073 7472 2874 7261 636b  _key : str(track
-00014ea0: 6c65 745f 6964 297d 2920 0d0a 2020 2020  let_id)}) ..    
-00014eb0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00014ec0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00014ed0: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
-00014ee0: 6461 7465 287b 7365 6c66 2e67 656e 6572  date({self.gener
-00014ef0: 6174 696f 6e69 645f 6b65 7920 3a20 7374  ationid_key : st
-00014f00: 7228 6765 6e65 7261 7469 6f6e 5f69 6429  r(generation_id)
-00014f10: 7d29 200d 0a20 2020 2020 2020 2073 656c  }) ..        sel
-00014f20: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-00014f30: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-00014f40: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-00014f50: 656c 662e 7472 6163 6b69 645f 6b65 7920  elf.trackid_key 
-00014f60: 3a20 7374 7228 7472 6163 6b5f 6964 297d  : str(track_id)}
-00014f70: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00014f80: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-00014f90: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-00014fa0: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-00014fb0: 662e 6d6f 7469 6f6e 5f61 6e67 6c65 5f6b  f.motion_angle_k
-00014fc0: 6579 203a 2030 2e30 7d29 0d0a 2020 2020  ey : 0.0})..    
-00014fd0: 2020 2020 7365 6c66 2e75 6e69 7175 655f      self.unique_
-00014fe0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-00014ff0: 696e 7428 6365 6c6c 5f69 6429 5d2e 7570  int(cell_id)].up
-00015000: 6461 7465 287b 7365 6c66 2e73 7065 6564  date({self.speed
-00015010: 5f6b 6579 203a 2030 2e30 7d29 0d0a 2020  _key : 0.0})..  
-00015020: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00015030: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00015040: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-00015050: 7570 6461 7465 287b 7365 6c66 2e61 6363  update({self.acc
-00015060: 656c 6572 6174 696f 6e5f 6b65 7920 3a20  eleration_key : 
-00015070: 302e 307d 290d 0a20 2020 2020 2020 2073  0.0})..        s
-00015080: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
-00015090: 7072 6f70 6572 7469 6573 5b69 6e74 2863  properties[int(c
-000150a0: 656c 6c5f 6964 295d 2e75 7064 6174 6528  ell_id)].update(
-000150b0: 7b73 656c 662e 6563 6365 6e74 7269 6369  {self.eccentrici
-000150c0: 7479 5f63 6f6d 705f 6669 7273 746b 6579  ty_comp_firstkey
-000150d0: 203a 204e 6f6e 657d 290d 0a20 2020 2020   : None})..     
-000150e0: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-000150f0: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00015100: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-00015110: 6174 6528 7b73 656c 662e 6563 6365 6e74  ate({self.eccent
-00015120: 7269 6369 7479 5f63 6f6d 705f 7365 636f  ricity_comp_seco
-00015130: 6e64 6b65 7920 3a20 4e6f 6e65 7d29 0d0a  ndkey : None})..
-00015140: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
-00015150: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
-00015160: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
-00015170: 5d2e 7570 6461 7465 287b 7365 6c66 2e73  ].update({self.s
-00015180: 7572 6661 6365 5f61 7265 615f 6b65 7920  urface_area_key 
-00015190: 3a20 4e6f 6e65 7d29 0d0a 2020 2020 2020  : None})..      
-000151a0: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
-000151b0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-000151c0: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
-000151d0: 7465 287b 7365 6c66 2e63 656c 6c61 7869  te({self.cellaxi
-000151e0: 735f 6d61 736b 5f6b 6579 203a 204e 6f6e  s_mask_key : Non
-000151f0: 657d 290d 0a0d 0a20 2020 2020 2020 2069  e})....        i
-00015200: 6620 736f 7572 6365 5f69 6420 6973 206e  f source_id is n
-00015210: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-00015220: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
-00015230: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-00015240: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
-00015250: 7570 6461 7465 287b 7365 6c66 2e62 6566  update({self.bef
-00015260: 6f72 6569 645f 6b65 7920 3a20 696e 7428  oreid_key : int(
-00015270: 736f 7572 6365 5f69 6429 7d29 0d0a 2020  source_id)})..  
-00015280: 2020 2020 2020 2020 2020 7665 635f 3120            vec_1 
-00015290: 3d20 5b66 6c6f 6174 2873 656c 662e 756e  = [float(self.un
-000152a0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-000152b0: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-000152c0: 295d 5b73 656c 662e 7870 6f73 6964 5f6b  )][self.xposid_k
-000152d0: 6579 5d29 202d 2066 6c6f 6174 2873 656c  ey]) - float(sel
-000152e0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-000152f0: 6f70 6572 7469 6573 5b69 6e74 2873 6f75  operties[int(sou
-00015300: 7263 655f 6964 295d 5b73 656c 662e 7870  rce_id)][self.xp
-00015310: 6f73 6964 5f6b 6579 5d29 2c20 0d0a 2020  osid_key]), ..  
-00015320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015330: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
-00015340: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
-00015350: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
-00015360: 6365 6c6c 5f69 6429 5d5b 7365 6c66 2e79  cell_id)][self.y
-00015370: 706f 7369 645f 6b65 795d 2920 2d20 666c  posid_key]) - fl
-00015380: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
-00015390: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000153a0: 696e 7428 736f 7572 6365 5f69 6429 5d5b  int(source_id)][
-000153b0: 7365 6c66 2e79 706f 7369 645f 6b65 795d  self.yposid_key]
-000153c0: 292c 200d 0a20 2020 2020 2020 2020 2020  ), ..           
+00014c10: 2020 2020 2020 2020 666c 6f61 7428 7365          float(se
+00014c20: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00014c30: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00014c40: 6c6c 5f69 6429 5d5b 7365 6c66 2e7a 706f  ll_id)][self.zpo
+00014c50: 7369 645f 6b65 795d 295d 0d0a 0d0a 2020  sid_key])]....  
+00014c60: 2020 2020 2020 616e 676c 6520 3d20 616e        angle = an
+00014c70: 6775 6c61 725f 6368 616e 6765 2876 6563  gular_change(vec
+00014c80: 5f6d 6173 6b2c 2076 6563 5f63 656c 6c29  _mask, vec_cell)
+00014c90: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
+00014ca0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00014cb0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+00014cc0: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+00014cd0: 6c66 2e72 6164 6961 6c5f 616e 676c 655f  lf.radial_angle_
+00014ce0: 6b65 7920 3a20 616e 676c 657d 2920 2020  key : angle})   
+00014cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d00: 200d 0a0d 0a20 2020 2020 2020 2075 6e69   ....        uni
+00014d10: 7175 655f 7472 6163 6b6c 6574 5f69 6473  que_tracklet_ids
+00014d20: 2e61 7070 656e 6428 7374 7228 756e 6971  .append(str(uniq
+00014d30: 7565 5f69 6429 290d 0a20 2020 2020 2020  ue_id))..       
+00014d40: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00014d50: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00014d60: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
+00014d70: 6528 7b73 656c 662e 636c 7573 7465 7263  e({self.clusterc
+00014d80: 6c61 7373 5f6b 6579 203a 204e 6f6e 657d  lass_key : None}
+00014d90: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00014da0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00014db0: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00014dc0: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
+00014dd0: 662e 636c 7573 7465 7273 636f 7265 5f6b  f.clusterscore_k
+00014de0: 6579 203a 2030 7d29 0d0a 2020 2020 2020  ey : 0})..      
+00014df0: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00014e00: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00014e10: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
+00014e20: 7465 287b 7365 6c66 2e75 6e69 7175 6569  te({self.uniquei
+00014e30: 645f 6b65 7920 3a20 7374 7228 756e 6971  d_key : str(uniq
+00014e40: 7565 5f69 6429 7d29 0d0a 2020 2020 2020  ue_id)})..      
+00014e50: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00014e60: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+00014e70: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
+00014e80: 7465 287b 7365 6c66 2e74 7261 636b 6c65  te({self.trackle
+00014e90: 7469 645f 6b65 7920 3a20 7374 7228 7472  tid_key : str(tr
+00014ea0: 6163 6b6c 6574 5f69 6429 7d29 200d 0a20  acklet_id)}) .. 
+00014eb0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00014ec0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00014ed0: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+00014ee0: 2e75 7064 6174 6528 7b73 656c 662e 6765  .update({self.ge
+00014ef0: 6e65 7261 7469 6f6e 6964 5f6b 6579 203a  nerationid_key :
+00014f00: 2073 7472 2867 656e 6572 6174 696f 6e5f   str(generation_
+00014f10: 6964 297d 2920 0d0a 2020 2020 2020 2020  id)}) ..        
+00014f20: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+00014f30: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00014f40: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+00014f50: 287b 7365 6c66 2e74 7261 636b 6964 5f6b  ({self.trackid_k
+00014f60: 6579 203a 2073 7472 2874 7261 636b 5f69  ey : str(track_i
+00014f70: 6429 7d29 0d0a 2020 2020 2020 2020 7365  d)})..        se
+00014f80: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+00014f90: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+00014fa0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+00014fb0: 7365 6c66 2e6d 6f74 696f 6e5f 616e 676c  self.motion_angl
+00014fc0: 655f 6b65 7920 3a20 302e 307d 290d 0a20  e_key : 0.0}).. 
+00014fd0: 2020 2020 2020 2073 656c 662e 756e 6971         self.uniq
+00014fe0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00014ff0: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
+00015000: 2e75 7064 6174 6528 7b73 656c 662e 7370  .update({self.sp
+00015010: 6565 645f 6b65 7920 3a20 302e 307d 290d  eed_key : 0.0}).
+00015020: 0a20 2020 2020 2020 2073 656c 662e 756e  .        self.un
+00015030: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00015040: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00015050: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00015060: 6163 6365 6c65 7261 7469 6f6e 5f6b 6579  acceleration_key
+00015070: 203a 2030 2e30 7d29 0d0a 2020 2020 2020   : 0.0})..      
+00015080: 2020 7365 6c66 2e75 6e69 7175 655f 7370    self.unique_sp
+00015090: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
+000150a0: 7428 6365 6c6c 5f69 6429 5d2e 7570 6461  t(cell_id)].upda
+000150b0: 7465 287b 7365 6c66 2e65 6363 656e 7472  te({self.eccentr
+000150c0: 6963 6974 795f 636f 6d70 5f66 6972 7374  icity_comp_first
+000150d0: 6b65 7920 3a20 4e6f 6e65 7d29 0d0a 2020  key : None})..  
+000150e0: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+000150f0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00015100: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+00015110: 7570 6461 7465 287b 7365 6c66 2e65 6363  update({self.ecc
+00015120: 656e 7472 6963 6974 795f 636f 6d70 5f73  entricity_comp_s
+00015130: 6563 6f6e 646b 6579 203a 204e 6f6e 657d  econdkey : None}
+00015140: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00015150: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
+00015160: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
+00015170: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
+00015180: 662e 7375 7266 6163 655f 6172 6561 5f6b  f.surface_area_k
+00015190: 6579 203a 204e 6f6e 657d 290d 0a20 2020  ey : None})..   
+000151a0: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
+000151b0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+000151c0: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
+000151d0: 7064 6174 6528 7b73 656c 662e 6365 6c6c  pdate({self.cell
+000151e0: 6178 6973 5f6d 6173 6b5f 6b65 7920 3a20  axis_mask_key : 
+000151f0: 4e6f 6e65 7d29 0d0a 0d0a 2020 2020 2020  None})....      
+00015200: 2020 6966 2073 6f75 7263 655f 6964 2069    if source_id i
+00015210: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+00015220: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
+00015230: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+00015240: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
+00015250: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
+00015260: 6265 666f 7265 6964 5f6b 6579 203a 2069  beforeid_key : i
+00015270: 6e74 2873 6f75 7263 655f 6964 297d 290d  nt(source_id)}).
+00015280: 0a20 2020 2020 2020 2020 2020 2076 6563  .            vec
+00015290: 5f31 203d 205b 666c 6f61 7428 7365 6c66  _1 = [float(self
+000152a0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+000152b0: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+000152c0: 5f69 6429 5d5b 7365 6c66 2e78 706f 7369  _id)][self.xposi
+000152d0: 645f 6b65 795d 2920 2d20 666c 6f61 7428  d_key]) - float(
+000152e0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+000152f0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+00015300: 736f 7572 6365 5f69 6429 5d5b 7365 6c66  source_id)][self
+00015310: 2e78 706f 7369 645f 6b65 795d 292c 200d  .xposid_key]), .
+00015320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015330: 2020 2020 2020 2020 2020 2020 2066 6c6f               flo
+00015340: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
+00015350: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
+00015360: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
+00015370: 662e 7970 6f73 6964 5f6b 6579 5d29 202d  f.yposid_key]) -
+00015380: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
+00015390: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+000153a0: 6573 5b69 6e74 2873 6f75 7263 655f 6964  es[int(source_id
+000153b0: 295d 5b73 656c 662e 7970 6f73 6964 5f6b  )][self.yposid_k
+000153c0: 6579 5d29 2c20 0d0a 2020 2020 2020 2020  ey]), ..        
 000153d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000153e0: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
-000153f0: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00015400: 6573 5b69 6e74 2863 656c 6c5f 6964 295d  es[int(cell_id)]
-00015410: 5b73 656c 662e 7a70 6f73 6964 5f6b 6579  [self.zposid_key
-00015420: 5d29 202d 2020 666c 6f61 7428 7365 6c66  ]) -  float(self
-00015430: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00015440: 7065 7274 6965 735b 696e 7428 736f 7572  perties[int(sour
-00015450: 6365 5f69 6429 5d5b 7365 6c66 2e7a 706f  ce_id)][self.zpo
-00015460: 7369 645f 6b65 795d 295d 0d0a 2020 2020  sid_key])]..    
-00015470: 2020 2020 2020 2020 7370 6565 6420 3d20          speed = 
-00015480: 6e70 2e73 7172 7428 6e70 2e64 6f74 2876  np.sqrt(np.dot(v
-00015490: 6563 5f31 2c20 7665 635f 3129 292f 7365  ec_1, vec_1))/se
-000154a0: 6c66 2e74 6361 6c69 6272 6174 696f 6e0d  lf.tcalibration.
-000154b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000154c0: 662e 756e 6971 7565 5f73 706f 745f 7072  f.unique_spot_pr
-000154d0: 6f70 6572 7469 6573 5b69 6e74 2863 656c  operties[int(cel
-000154e0: 6c5f 6964 295d 2e75 7064 6174 6528 7b73  l_id)].update({s
-000154f0: 656c 662e 7370 6565 645f 6b65 7920 3a20  elf.speed_key : 
-00015500: 7370 6565 647d 290d 0a0d 0a20 2020 2020  speed})....     
-00015510: 2020 2020 2020 206d 6f74 696f 6e5f 616e         motion_an
-00015520: 676c 6520 3d20 616e 6775 6c61 725f 6368  gle = angular_ch
-00015530: 616e 6765 2876 6563 5f6d 6173 6b2c 2076  ange(vec_mask, v
-00015540: 6563 5f31 290d 0a0d 0a20 2020 2020 2020  ec_1)....       
-00015550: 2020 2020 2073 656c 662e 756e 6971 7565       self.unique
-00015560: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
-00015570: 5b69 6e74 2863 656c 6c5f 6964 295d 2e75  [int(cell_id)].u
-00015580: 7064 6174 6528 7b73 656c 662e 6d6f 7469  pdate({self.moti
-00015590: 6f6e 5f61 6e67 6c65 5f6b 6579 203a 206d  on_angle_key : m
-000155a0: 6f74 696f 6e5f 616e 676c 657d 2920 0d0a  otion_angle}) ..
-000155b0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-000155c0: 2073 6f75 7263 655f 6964 2069 6e20 7365   source_id in se
-000155d0: 6c66 2e65 6467 655f 736f 7572 6365 5f6c  lf.edge_source_l
-000155e0: 6f6f 6b75 703a 0d0a 2020 2020 2020 2020  ookup:..        
-000155f0: 2020 2020 2020 2020 2020 2020 7072 655f              pre_
-00015600: 736f 7572 6365 5f69 6420 3d20 7365 6c66  source_id = self
-00015610: 2e65 6467 655f 736f 7572 6365 5f6c 6f6f  .edge_source_loo
-00015620: 6b75 705b 736f 7572 6365 5f69 645d 0d0a  kup[source_id]..
-00015630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015640: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00015650: 2020 2020 2020 2020 2020 7665 635f 3220            vec_2 
-00015660: 3d20 5b66 6c6f 6174 2873 656c 662e 756e  = [float(self.un
-00015670: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00015680: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00015690: 295d 5b73 656c 662e 7870 6f73 6964 5f6b  )][self.xposid_k
-000156a0: 6579 5d29 202d 2032 202a 2066 6c6f 6174  ey]) - 2 * float
-000156b0: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
-000156c0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
-000156d0: 2873 6f75 7263 655f 6964 295d 5b73 656c  (source_id)][sel
-000156e0: 662e 7870 6f73 6964 5f6b 6579 5d29 202b  f.xposid_key]) +
-000156f0: 2066 6c6f 6174 2873 656c 662e 756e 6971   float(self.uniq
-00015700: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
-00015710: 6573 5b69 6e74 2870 7265 5f73 6f75 7263  es[int(pre_sourc
-00015720: 655f 6964 295d 5b73 656c 662e 7870 6f73  e_id)][self.xpos
-00015730: 6964 5f6b 6579 5d29 2c20 0d0a 2020 2020  id_key]), ..    
+000153e0: 2020 2020 666c 6f61 7428 7365 6c66 2e75      float(self.u
+000153f0: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00015400: 7274 6965 735b 696e 7428 6365 6c6c 5f69  rties[int(cell_i
+00015410: 6429 5d5b 7365 6c66 2e7a 706f 7369 645f  d)][self.zposid_
+00015420: 6b65 795d 2920 2d20 2066 6c6f 6174 2873  key]) -  float(s
+00015430: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00015440: 7072 6f70 6572 7469 6573 5b69 6e74 2873  properties[int(s
+00015450: 6f75 7263 655f 6964 295d 5b73 656c 662e  ource_id)][self.
+00015460: 7a70 6f73 6964 5f6b 6579 5d29 5d0d 0a20  zposid_key])].. 
+00015470: 2020 2020 2020 2020 2020 2073 7065 6564             speed
+00015480: 203d 206e 702e 7371 7274 286e 702e 646f   = np.sqrt(np.do
+00015490: 7428 7665 635f 312c 2076 6563 5f31 2929  t(vec_1, vec_1))
+000154a0: 2f73 656c 662e 7463 616c 6962 7261 7469  /self.tcalibrati
+000154b0: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+000154c0: 7365 6c66 2e75 6e69 7175 655f 7370 6f74  self.unique_spot
+000154d0: 5f70 726f 7065 7274 6965 735b 696e 7428  _properties[int(
+000154e0: 6365 6c6c 5f69 6429 5d2e 7570 6461 7465  cell_id)].update
+000154f0: 287b 7365 6c66 2e73 7065 6564 5f6b 6579  ({self.speed_key
+00015500: 203a 2073 7065 6564 7d29 0d0a 0d0a 2020   : speed})....  
+00015510: 2020 2020 2020 2020 2020 6d6f 7469 6f6e            motion
+00015520: 5f61 6e67 6c65 203d 2061 6e67 756c 6172  _angle = angular
+00015530: 5f63 6861 6e67 6528 7665 635f 6d61 736b  _change(vec_mask
+00015540: 2c20 7665 635f 3129 0d0a 0d0a 2020 2020  , vec_1)....    
+00015550: 2020 2020 2020 2020 7365 6c66 2e75 6e69          self.uni
+00015560: 7175 655f 7370 6f74 5f70 726f 7065 7274  que_spot_propert
+00015570: 6965 735b 696e 7428 6365 6c6c 5f69 6429  ies[int(cell_id)
+00015580: 5d2e 7570 6461 7465 287b 7365 6c66 2e6d  ].update({self.m
+00015590: 6f74 696f 6e5f 616e 676c 655f 6b65 7920  otion_angle_key 
+000155a0: 3a20 6d6f 7469 6f6e 5f61 6e67 6c65 7d29  : motion_angle})
+000155b0: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+000155c0: 2069 6620 736f 7572 6365 5f69 6420 696e   if source_id in
+000155d0: 2073 656c 662e 6564 6765 5f73 6f75 7263   self.edge_sourc
+000155e0: 655f 6c6f 6f6b 7570 3a0d 0a20 2020 2020  e_lookup:..     
+000155f0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00015600: 7265 5f73 6f75 7263 655f 6964 203d 2073  re_source_id = s
+00015610: 656c 662e 6564 6765 5f73 6f75 7263 655f  elf.edge_source_
+00015620: 6c6f 6f6b 7570 5b73 6f75 7263 655f 6964  lookup[source_id
+00015630: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00015640: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00015650: 2020 2020 2020 2020 2020 2020 2076 6563               vec
+00015660: 5f32 203d 205b 666c 6f61 7428 7365 6c66  _2 = [float(self
+00015670: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00015680: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+00015690: 5f69 6429 5d5b 7365 6c66 2e78 706f 7369  _id)][self.xposi
+000156a0: 645f 6b65 795d 2920 2d20 3220 2a20 666c  d_key]) - 2 * fl
+000156b0: 6f61 7428 7365 6c66 2e75 6e69 7175 655f  oat(self.unique_
+000156c0: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
+000156d0: 696e 7428 736f 7572 6365 5f69 6429 5d5b  int(source_id)][
+000156e0: 7365 6c66 2e78 706f 7369 645f 6b65 795d  self.xposid_key]
+000156f0: 2920 2b20 666c 6f61 7428 7365 6c66 2e75  ) + float(self.u
+00015700: 6e69 7175 655f 7370 6f74 5f70 726f 7065  nique_spot_prope
+00015710: 7274 6965 735b 696e 7428 7072 655f 736f  rties[int(pre_so
+00015720: 7572 6365 5f69 6429 5d5b 7365 6c66 2e78  urce_id)][self.x
+00015730: 706f 7369 645f 6b65 795d 292c 200d 0a20  posid_key]), .. 
 00015740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015750: 2020 2020 2020 2020 666c 6f61 7428 7365          float(se
-00015760: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00015770: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00015780: 6c6c 5f69 6429 5d5b 7365 6c66 2e79 706f  ll_id)][self.ypo
-00015790: 7369 645f 6b65 795d 2920 2d20 3220 2a20  sid_key]) - 2 * 
-000157a0: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
-000157b0: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
-000157c0: 735b 696e 7428 736f 7572 6365 5f69 6429  s[int(source_id)
-000157d0: 5d5b 7365 6c66 2e79 706f 7369 645f 6b65  ][self.yposid_ke
-000157e0: 795d 2920 2b20 666c 6f61 7428 7365 6c66  y]) + float(self
-000157f0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-00015800: 7065 7274 6965 735b 696e 7428 7072 655f  perties[int(pre_
-00015810: 736f 7572 6365 5f69 6429 5d5b 7365 6c66  source_id)][self
-00015820: 2e79 706f 7369 645f 6b65 795d 292c 200d  .yposid_key]), .
-00015830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015840: 2020 2020 2020 2020 2020 2020 2066 6c6f               flo
-00015850: 6174 2873 656c 662e 756e 6971 7565 5f73  at(self.unique_s
-00015860: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00015870: 6e74 2863 656c 6c5f 6964 295d 5b73 656c  nt(cell_id)][sel
-00015880: 662e 7a70 6f73 6964 5f6b 6579 5d29 202d  f.zposid_key]) -
-00015890: 2020 3220 2a20 666c 6f61 7428 7365 6c66    2 * float(self
-000158a0: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
-000158b0: 7065 7274 6965 735b 696e 7428 736f 7572  perties[int(sour
-000158c0: 6365 5f69 6429 5d5b 7365 6c66 2e7a 706f  ce_id)][self.zpo
-000158d0: 7369 645f 6b65 795d 2920 2b20 666c 6f61  sid_key]) + floa
-000158e0: 7428 7365 6c66 2e75 6e69 7175 655f 7370  t(self.unique_sp
-000158f0: 6f74 5f70 726f 7065 7274 6965 735b 696e  ot_properties[in
-00015900: 7428 7072 655f 736f 7572 6365 5f69 6429  t(pre_source_id)
-00015910: 5d5b 7365 6c66 2e7a 706f 7369 645f 6b65  ][self.zposid_ke
-00015920: 795d 295d 0d0a 2020 2020 2020 2020 2020  y])]..          
-00015930: 2020 2020 2020 2020 2020 6163 6320 3d20            acc = 
-00015940: 6e70 2e73 7172 7428 6e70 2e64 6f74 2876  np.sqrt(np.dot(v
-00015950: 6563 5f32 2c20 7665 635f 3229 292f 7365  ec_2, vec_2))/se
-00015960: 6c66 2e74 6361 6c69 6272 6174 696f 6e0d  lf.tcalibration.
-00015970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015980: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-00015990: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000159a0: 756e 6971 7565 5f73 706f 745f 7072 6f70  unique_spot_prop
-000159b0: 6572 7469 6573 5b69 6e74 2863 656c 6c5f  erties[int(cell_
-000159c0: 6964 295d 2e75 7064 6174 6528 7b73 656c  id)].update({sel
-000159d0: 662e 6163 6365 6c65 7261 7469 6f6e 5f6b  f.acceleration_k
-000159e0: 6579 203a 2061 6363 7d29 0d0a 2020 2020  ey : acc})..    
-000159f0: 2020 2020 656c 6966 2073 6f75 7263 655f      elif source_
-00015a00: 6964 2069 7320 4e6f 6e65 3a0d 0a20 2020  id is None:..   
-00015a10: 2020 2020 2020 2020 2073 656c 662e 756e           self.un
-00015a20: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
-00015a30: 7469 6573 5b69 6e74 2863 656c 6c5f 6964  ties[int(cell_id
-00015a40: 295d 2e75 7064 6174 6528 7b73 656c 662e  )].update({self.
-00015a50: 6265 666f 7265 6964 5f6b 6579 203a 204e  beforeid_key : N
-00015a60: 6f6e 657d 2920 0d0a 2020 2020 2020 2020  one}) ..        
-00015a70: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
-00015a80: 6966 2074 6172 6765 745f 6964 2069 7320  if target_id is 
-00015a90: 6e6f 7420 4e6f 6e65 3a20 2020 2020 2020  not None:       
-00015aa0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00015ab0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
-00015ac0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
-00015ad0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
-00015ae0: 7365 6c66 2e61 6674 6572 6964 5f6b 6579  self.afterid_key
-00015af0: 203a 2069 6e74 2874 6172 6765 745f 6964   : int(target_id
-00015b00: 297d 2920 0d0a 2020 2020 2020 2020 656c  )}) ..        el
-00015b10: 6966 2074 6172 6765 745f 6964 2069 7320  if target_id is 
-00015b20: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00015b30: 2020 2073 656c 662e 756e 6971 7565 5f73     self.unique_s
-00015b40: 706f 745f 7072 6f70 6572 7469 6573 5b69  pot_properties[i
-00015b50: 6e74 2863 656c 6c5f 6964 295d 2e75 7064  nt(cell_id)].upd
-00015b60: 6174 6528 7b73 656c 662e 6166 7465 7269  ate({self.afteri
-00015b70: 645f 6b65 7920 3a20 4e6f 6e65 7d29 0d0a  d_key : None})..
-00015b80: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00015b90: 2020 2020 2020 7365 6c66 2e5f 7365 636f        self._seco
-00015ba0: 6e64 5f63 6861 6e6e 656c 5f75 7064 6174  nd_channel_updat
-00015bb0: 6528 6365 6c6c 5f69 642c 2074 7261 636b  e(cell_id, track
-00015bc0: 5f69 6429 2020 2020 0d0a 0d0a 0d0a 2020  _id)    ......  
-00015bd0: 2020 6465 6620 5f74 656d 706f 7261 6c5f    def _temporal_
-00015be0: 706c 6f74 735f 7472 6163 6b6d 6174 6528  plots_trackmate(
-00015bf0: 7365 6c66 293a 0d0a 2020 2020 0d0a 2020  self):..    ..  
-00015c00: 2020 0d0a 2020 2020 0d0a 2020 2020 2020    ..    ..      
-00015c10: 2020 2020 2020 2020 2020 7365 6c66 2e41            self.A
-00015c20: 7474 7220 3d20 7b7d 0d0a 2020 2020 2020  ttr = {}..      
-00015c30: 2020 2020 2020 2020 2020 7374 6172 7474            startt
-00015c40: 696d 6520 3d20 696e 7428 6d69 6e28 7365  ime = int(min(se
-00015c50: 6c66 2e41 6c6c 5661 6c75 6573 5b73 656c  lf.AllValues[sel
-00015c60: 662e 6672 616d 6569 645f 6b65 795d 2929  f.frameid_key]))
-00015c70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00015c80: 2020 656e 6474 696d 6520 3d20 696e 7428    endtime = int(
-00015c90: 6d61 7828 7365 6c66 2e41 6c6c 5661 6c75  max(self.AllValu
-00015ca0: 6573 5b73 656c 662e 6672 616d 6569 645f  es[self.frameid_
-00015cb0: 6b65 795d 2929 0d0a 2020 2020 2020 2020  key]))..        
-00015cc0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00015cd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015ce0: 7469 6d65 203d 205b 5d0d 0a20 2020 2020  time = []..     
-00015cf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015d00: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
-00015d10: 705f 7a20 3d20 5b5d 0d0a 2020 2020 2020  p_z = []..      
-00015d20: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00015d30: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
-00015d40: 7a20 3d20 5b5d 0d0a 0d0a 2020 2020 2020  z = []....      
-00015d50: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00015d60: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
-00015d70: 5f79 203d 205b 5d0d 0a20 2020 2020 2020  _y = []..       
-00015d80: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00015d90: 746f 7469 635f 7661 725f 6469 7370 5f79  totic_var_disp_y
-00015da0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00015db0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00015dc0: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
-00015dd0: 7820 3d20 5b5d 0d0a 2020 2020 2020 2020  x = []..        
-00015de0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00015df0: 6f74 6963 5f76 6172 5f64 6973 705f 7820  otic_var_disp_x 
-00015e00: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
-00015e10: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00015e20: 6f74 6963 5f6d 6561 6e5f 7261 6469 7573  otic_mean_radius
-00015e30: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00015e40: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00015e50: 7469 635f 7661 725f 7261 6469 7573 203d  tic_var_radius =
-00015e60: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-00015e70: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00015e80: 7469 635f 6d65 616e 5f73 7065 6564 203d  tic_mean_speed =
-00015e90: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-00015ea0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00015eb0: 635f 7661 725f 7370 6565 6420 3d20 5b5d  c_var_speed = []
-00015ec0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00015ed0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00015ee0: 5f6d 6561 6e5f 6163 6320 3d20 5b5d 0d0a  _mean_acc = []..
-00015ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f00: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
-00015f10: 5f61 6363 203d 205b 5d0d 0a0d 0a20 2020  _acc = []....   
-00015f20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015f30: 662e 6d69 746f 7469 635f 6d65 616e 5f64  f.mitotic_mean_d
-00015f40: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00015f50: 6520 3d20 5b5d 0d0a 2020 2020 2020 2020  e = []..        
-00015f60: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00015f70: 6f74 6963 5f76 6172 5f64 6972 6563 7469  otic_var_directi
-00015f80: 6f6e 616c 5f63 6861 6e67 6520 3d20 5b5d  onal_change = []
-00015f90: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00015fa0: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00015fb0: 5f6d 6561 6e5f 6469 7374 616e 6365 5f63  _mean_distance_c
-00015fc0: 656c 6c5f 6d61 736b 203d 205b 5d0d 0a20  ell_mask = [].. 
-00015fd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015fe0: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
-00015ff0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00016000: 736b 203d 205b 5d0d 0a0d 0a20 2020 2020  sk = []....     
-00016010: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016020: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-00016030: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 2020  _disp_z = []..  
-00016040: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00016050: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
-00016060: 6172 5f64 6973 705f 7a20 3d20 5b5d 0d0a  ar_disp_z = []..
-00016070: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016080: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00016090: 6963 5f6d 6561 6e5f 6469 7370 5f79 203d  ic_mean_disp_y =
-000160a0: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-000160b0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-000160c0: 746f 7469 635f 7661 725f 6469 7370 5f79  totic_var_disp_y
-000160d0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-000160e0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-000160f0: 6e5f 6d69 746f 7469 635f 6d65 616e 5f64  n_mitotic_mean_d
-00016100: 6973 705f 7820 3d20 5b5d 0d0a 2020 2020  isp_x = []..    
-00016110: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016120: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
-00016130: 5f64 6973 705f 7820 3d20 5b5d 0d0a 0d0a  _disp_x = []....
-00016140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016150: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00016160: 5f6d 6561 6e5f 7261 6469 7573 203d 205b  _mean_radius = [
-00016170: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016180: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00016190: 7469 635f 7661 725f 7261 6469 7573 203d  tic_var_radius =
-000161a0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-000161b0: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-000161c0: 6d69 746f 7469 635f 6d65 616e 5f73 7065  mitotic_mean_spe
-000161d0: 6564 203d 205b 5d0d 0a20 2020 2020 2020  ed = []..       
-000161e0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-000161f0: 6e5f 6d69 746f 7469 635f 7661 725f 7370  n_mitotic_var_sp
-00016200: 6565 6420 3d20 5b5d 0d0a 0d0a 2020 2020  eed = []....    
-00016210: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016220: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
-00016230: 6e5f 6163 6320 3d20 5b5d 0d0a 2020 2020  n_acc = []..    
-00016240: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016250: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
-00016260: 5f61 6363 203d 205b 5d0d 0a0d 0a20 2020  _acc = []....   
-00016270: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00016280: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-00016290: 616e 5f64 6972 6563 7469 6f6e 616c 5f63  an_directional_c
-000162a0: 6861 6e67 6520 3d20 5b5d 0d0a 2020 2020  hange = []..    
-000162b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000162c0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
-000162d0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-000162e0: 6e67 6520 3d20 5b5d 0d0a 0d0a 2020 2020  nge = []....    
-000162f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016300: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
-00016310: 6e5f 6469 7374 616e 6365 5f63 656c 6c5f  n_distance_cell_
-00016320: 6d61 736b 203d 205b 5d0d 0a20 2020 2020  mask = []..     
-00016330: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016340: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-00016350: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00016360: 736b 203d 205b 5d0d 0a0d 0a20 2020 2020  sk = []....     
-00016370: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016380: 616c 6c5f 6d65 616e 5f64 6973 705f 7a20  all_mean_disp_z 
-00016390: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-000163a0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
-000163b0: 6172 5f64 6973 705f 7a20 3d20 5b5d 0d0a  ar_disp_z = []..
-000163c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000163d0: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
-000163e0: 6469 7370 5f79 203d 205b 5d0d 0a20 2020  disp_y = []..   
-000163f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00016400: 662e 616c 6c5f 7661 725f 6469 7370 5f79  f.all_var_disp_y
-00016410: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-00016420: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00016430: 6c5f 6d65 616e 5f64 6973 705f 7820 3d20  l_mean_disp_x = 
-00016440: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00016450: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
-00016460: 5f64 6973 705f 7820 3d20 5b5d 0d0a 0d0a  _disp_x = []....
-00016470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016480: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 7261  self.all_mean_ra
-00016490: 6469 7573 203d 205b 5d0d 0a20 2020 2020  dius = []..     
-000164a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000164b0: 616c 6c5f 7661 725f 7261 6469 7573 203d  all_var_radius =
-000164c0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
-000164d0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-000164e0: 6d65 616e 5f73 7065 6564 203d 205b 5d0d  mean_speed = [].
-000164f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016500: 2073 656c 662e 616c 6c5f 7661 725f 7370   self.all_var_sp
-00016510: 6565 6420 3d20 5b5d 0d0a 0d0a 2020 2020  eed = []....    
-00016520: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016530: 2e61 6c6c 5f6d 6561 6e5f 6163 6320 3d20  .all_mean_acc = 
-00016540: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00016550: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
-00016560: 5f61 6363 203d 205b 5d0d 0a0d 0a20 2020  _acc = []....   
-00016570: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00016580: 662e 616c 6c5f 6d65 616e 5f64 6972 6563  f.all_mean_direc
-00016590: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
-000165a0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-000165b0: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
-000165c0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-000165d0: 6e67 6520 3d20 5b5d 0d0a 0d0a 2020 2020  nge = []....    
-000165e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000165f0: 2e61 6c6c 5f6d 6561 6e5f 6469 7374 616e  .all_mean_distan
-00016600: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
-00016610: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016620: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-00016630: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00016640: 736b 203d 205b 5d0d 0a0d 0a20 2020 2020  sk = []....     
-00016650: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016660: 6d69 746f 7469 635f 636c 7573 7465 725f  mitotic_cluster_
-00016670: 636c 6173 7320 3d20 5b5d 0d0a 2020 2020  class = []..    
-00016680: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016690: 2e6e 6f6e 5f6d 6974 6f74 6963 5f63 6c75  .non_mitotic_clu
-000166a0: 7374 6572 5f63 6c61 7373 203d 205b 5d0d  ster_class = [].
-000166b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000166c0: 2073 656c 662e 616c 6c5f 636c 7573 7465   self.all_cluste
-000166d0: 725f 636c 6173 7320 3d20 5b5d 0d0a 0d0a  r_class = []....
-000166e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000166f0: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-00016700: 203d 207b 7d0d 0a20 2020 2020 2020 2020   = {}..         
-00016710: 2020 2020 2020 2066 6f72 2028 6b2c 7629         for (k,v)
-00016720: 2069 6e20 7365 6c66 2e75 6e69 7175 655f   in self.unique_
-00016730: 7370 6f74 5f70 726f 7065 7274 6965 732e  spot_properties.
-00016740: 6974 656d 7328 293a 0d0a 2020 2020 2020  items():..      
+00015750: 2020 2020 2020 2020 2020 2066 6c6f 6174             float
+00015760: 2873 656c 662e 756e 6971 7565 5f73 706f  (self.unique_spo
+00015770: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00015780: 2863 656c 6c5f 6964 295d 5b73 656c 662e  (cell_id)][self.
+00015790: 7970 6f73 6964 5f6b 6579 5d29 202d 2032  yposid_key]) - 2
+000157a0: 202a 2066 6c6f 6174 2873 656c 662e 756e   * float(self.un
+000157b0: 6971 7565 5f73 706f 745f 7072 6f70 6572  ique_spot_proper
+000157c0: 7469 6573 5b69 6e74 2873 6f75 7263 655f  ties[int(source_
+000157d0: 6964 295d 5b73 656c 662e 7970 6f73 6964  id)][self.yposid
+000157e0: 5f6b 6579 5d29 202b 2066 6c6f 6174 2873  _key]) + float(s
+000157f0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+00015800: 7072 6f70 6572 7469 6573 5b69 6e74 2870  properties[int(p
+00015810: 7265 5f73 6f75 7263 655f 6964 295d 5b73  re_source_id)][s
+00015820: 656c 662e 7970 6f73 6964 5f6b 6579 5d29  elf.yposid_key])
+00015830: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+00015840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015850: 666c 6f61 7428 7365 6c66 2e75 6e69 7175  float(self.uniqu
+00015860: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00015870: 735b 696e 7428 6365 6c6c 5f69 6429 5d5b  s[int(cell_id)][
+00015880: 7365 6c66 2e7a 706f 7369 645f 6b65 795d  self.zposid_key]
+00015890: 2920 2d20 2032 202a 2066 6c6f 6174 2873  ) -  2 * float(s
+000158a0: 656c 662e 756e 6971 7565 5f73 706f 745f  elf.unique_spot_
+000158b0: 7072 6f70 6572 7469 6573 5b69 6e74 2873  properties[int(s
+000158c0: 6f75 7263 655f 6964 295d 5b73 656c 662e  ource_id)][self.
+000158d0: 7a70 6f73 6964 5f6b 6579 5d29 202b 2066  zposid_key]) + f
+000158e0: 6c6f 6174 2873 656c 662e 756e 6971 7565  loat(self.unique
+000158f0: 5f73 706f 745f 7072 6f70 6572 7469 6573  _spot_properties
+00015900: 5b69 6e74 2870 7265 5f73 6f75 7263 655f  [int(pre_source_
+00015910: 6964 295d 5b73 656c 662e 7a70 6f73 6964  id)][self.zposid
+00015920: 5f6b 6579 5d29 5d0d 0a20 2020 2020 2020  _key])]..       
+00015930: 2020 2020 2020 2020 2020 2020 2061 6363               acc
+00015940: 203d 206e 702e 7371 7274 286e 702e 646f   = np.sqrt(np.do
+00015950: 7428 7665 635f 322c 2076 6563 5f32 2929  t(vec_2, vec_2))
+00015960: 2f73 656c 662e 7463 616c 6962 7261 7469  /self.tcalibrati
+00015970: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
+00015980: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00015990: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000159a0: 6c66 2e75 6e69 7175 655f 7370 6f74 5f70  lf.unique_spot_p
+000159b0: 726f 7065 7274 6965 735b 696e 7428 6365  roperties[int(ce
+000159c0: 6c6c 5f69 6429 5d2e 7570 6461 7465 287b  ll_id)].update({
+000159d0: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
+000159e0: 6e5f 6b65 7920 3a20 6163 637d 290d 0a20  n_key : acc}).. 
+000159f0: 2020 2020 2020 2065 6c69 6620 736f 7572         elif sour
+00015a00: 6365 5f69 6420 6973 204e 6f6e 653a 0d0a  ce_id is None:..
+00015a10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015a20: 2e75 6e69 7175 655f 7370 6f74 5f70 726f  .unique_spot_pro
+00015a30: 7065 7274 6965 735b 696e 7428 6365 6c6c  perties[int(cell
+00015a40: 5f69 6429 5d2e 7570 6461 7465 287b 7365  _id)].update({se
+00015a50: 6c66 2e62 6566 6f72 6569 645f 6b65 7920  lf.beforeid_key 
+00015a60: 3a20 4e6f 6e65 7d29 200d 0a20 2020 2020  : None}) ..     
+00015a70: 2020 2020 2020 200d 0a0d 0a20 2020 2020         ....     
+00015a80: 2020 2069 6620 7461 7267 6574 5f69 6420     if target_id 
+00015a90: 6973 206e 6f74 204e 6f6e 653a 2020 2020  is not None:    
+00015aa0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00015ab0: 2073 656c 662e 756e 6971 7565 5f73 706f   self.unique_spo
+00015ac0: 745f 7072 6f70 6572 7469 6573 5b69 6e74  t_properties[int
+00015ad0: 2863 656c 6c5f 6964 295d 2e75 7064 6174  (cell_id)].updat
+00015ae0: 6528 7b73 656c 662e 6166 7465 7269 645f  e({self.afterid_
+00015af0: 6b65 7920 3a20 696e 7428 7461 7267 6574  key : int(target
+00015b00: 5f69 6429 7d29 200d 0a20 2020 2020 2020  _id)}) ..       
+00015b10: 2065 6c69 6620 7461 7267 6574 5f69 6420   elif target_id 
+00015b20: 6973 204e 6f6e 653a 0d0a 2020 2020 2020  is None:..      
+00015b30: 2020 2020 2020 7365 6c66 2e75 6e69 7175        self.uniqu
+00015b40: 655f 7370 6f74 5f70 726f 7065 7274 6965  e_spot_propertie
+00015b50: 735b 696e 7428 6365 6c6c 5f69 6429 5d2e  s[int(cell_id)].
+00015b60: 7570 6461 7465 287b 7365 6c66 2e61 6674  update({self.aft
+00015b70: 6572 6964 5f6b 6579 203a 204e 6f6e 657d  erid_key : None}
+00015b80: 290d 0a20 2020 2020 2020 2020 2020 200d  )..            .
+00015b90: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
+00015ba0: 6563 6f6e 645f 6368 616e 6e65 6c5f 7570  econd_channel_up
+00015bb0: 6461 7465 2863 656c 6c5f 6964 2c20 7472  date(cell_id, tr
+00015bc0: 6163 6b5f 6964 2920 2020 200d 0a0d 0a0d  ack_id)    .....
+00015bd0: 0a20 2020 2064 6566 205f 7465 6d70 6f72  .    def _tempor
+00015be0: 616c 5f70 6c6f 7473 5f74 7261 636b 6d61  al_plots_trackma
+00015bf0: 7465 2873 656c 6629 3a0d 0a20 2020 200d  te(self):..    .
+00015c00: 0a20 2020 200d 0a20 2020 200d 0a20 2020  .    ..    ..   
+00015c10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015c20: 662e 4174 7472 203d 207b 7d0d 0a20 2020  f.Attr = {}..   
+00015c30: 2020 2020 2020 2020 2020 2020 2073 7461               sta
+00015c40: 7274 7469 6d65 203d 2069 6e74 286d 696e  rttime = int(min
+00015c50: 2873 656c 662e 416c 6c56 616c 7565 735b  (self.AllValues[
+00015c60: 7365 6c66 2e66 7261 6d65 6964 5f6b 6579  self.frameid_key
+00015c70: 5d29 290d 0a20 2020 2020 2020 2020 2020  ]))..           
+00015c80: 2020 2020 2065 6e64 7469 6d65 203d 2069       endtime = i
+00015c90: 6e74 286d 6178 2873 656c 662e 416c 6c56  nt(max(self.AllV
+00015ca0: 616c 7565 735b 7365 6c66 2e66 7261 6d65  alues[self.frame
+00015cb0: 6964 5f6b 6579 5d29 290d 0a20 2020 2020  id_key]))..     
+00015cc0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00015cd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015ce0: 6c66 2e74 696d 6520 3d20 5b5d 0d0a 2020  lf.time = []..  
+00015cf0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015d00: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
+00015d10: 6469 7370 5f7a 203d 205b 5d0d 0a20 2020  disp_z = []..   
+00015d20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015d30: 662e 6d69 746f 7469 635f 7661 725f 6469  f.mitotic_var_di
+00015d40: 7370 5f7a 203d 205b 5d0d 0a0d 0a20 2020  sp_z = []....   
+00015d50: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015d60: 662e 6d69 746f 7469 635f 6d65 616e 5f64  f.mitotic_mean_d
+00015d70: 6973 705f 7920 3d20 5b5d 0d0a 2020 2020  isp_y = []..    
+00015d80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015d90: 2e6d 6974 6f74 6963 5f76 6172 5f64 6973  .mitotic_var_dis
+00015da0: 705f 7920 3d20 5b5d 0d0a 0d0a 2020 2020  p_y = []....    
+00015db0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015dc0: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
+00015dd0: 7370 5f78 203d 205b 5d0d 0a20 2020 2020  sp_x = []..     
+00015de0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015df0: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
+00015e00: 5f78 203d 205b 5d0d 0a0d 0a20 2020 2020  _x = []....     
+00015e10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015e20: 6d69 746f 7469 635f 6d65 616e 5f72 6164  mitotic_mean_rad
+00015e30: 6975 7320 3d20 5b5d 0d0a 2020 2020 2020  ius = []..      
+00015e40: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00015e50: 6974 6f74 6963 5f76 6172 5f72 6164 6975  itotic_var_radiu
+00015e60: 7320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  s = []....      
+00015e70: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00015e80: 6974 6f74 6963 5f6d 6561 6e5f 7370 6565  itotic_mean_spee
+00015e90: 6420 3d20 5b5d 0d0a 2020 2020 2020 2020  d = []..        
+00015ea0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00015eb0: 6f74 6963 5f76 6172 5f73 7065 6564 203d  otic_var_speed =
+00015ec0: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+00015ed0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00015ee0: 7469 635f 6d65 616e 5f61 6363 203d 205b  tic_mean_acc = [
+00015ef0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00015f00: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00015f10: 7661 725f 6163 6320 3d20 5b5d 0d0a 0d0a  var_acc = []....
+00015f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f30: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
+00015f40: 6e5f 6469 7265 6374 696f 6e61 6c5f 6368  n_directional_ch
+00015f50: 616e 6765 203d 205b 5d0d 0a20 2020 2020  ange = []..     
+00015f60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015f70: 6d69 746f 7469 635f 7661 725f 6469 7265  mitotic_var_dire
+00015f80: 6374 696f 6e61 6c5f 6368 616e 6765 203d  ctional_change =
+00015f90: 205b 5d0d 0a0d 0a20 2020 2020 2020 2020   []....         
+00015fa0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00015fb0: 7469 635f 6d65 616e 5f64 6973 7461 6e63  tic_mean_distanc
+00015fc0: 655f 6365 6c6c 5f6d 6173 6b20 3d20 5b5d  e_cell_mask = []
+00015fd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00015fe0: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
+00015ff0: 6172 5f64 6973 7461 6e63 655f 6365 6c6c  ar_distance_cell
+00016000: 5f6d 6173 6b20 3d20 5b5d 0d0a 0d0a 2020  _mask = []....  
+00016010: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016020: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
+00016030: 6561 6e5f 6469 7370 5f7a 203d 205b 5d0d  ean_disp_z = [].
+00016040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016050: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+00016060: 635f 7661 725f 6469 7370 5f7a 203d 205b  c_var_disp_z = [
+00016070: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+00016080: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+00016090: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
+000160a0: 7920 3d20 5b5d 0d0a 2020 2020 2020 2020  y = []..        
+000160b0: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+000160c0: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
+000160d0: 705f 7920 3d20 5b5d 0d0a 0d0a 2020 2020  p_y = []....    
+000160e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000160f0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
+00016100: 6e5f 6469 7370 5f78 203d 205b 5d0d 0a20  n_disp_x = [].. 
+00016110: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016120: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00016130: 7661 725f 6469 7370 5f78 203d 205b 5d0d  var_disp_x = [].
+00016140: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00016150: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+00016160: 7469 635f 6d65 616e 5f72 6164 6975 7320  tic_mean_radius 
+00016170: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016180: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00016190: 6974 6f74 6963 5f76 6172 5f72 6164 6975  itotic_var_radiu
+000161a0: 7320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  s = []....      
+000161b0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+000161c0: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
+000161d0: 7370 6565 6420 3d20 5b5d 0d0a 2020 2020  speed = []..    
+000161e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000161f0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
+00016200: 5f73 7065 6564 203d 205b 5d0d 0a0d 0a20  _speed = [].... 
+00016210: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016220: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00016230: 6d65 616e 5f61 6363 203d 205b 5d0d 0a20  mean_acc = [].. 
+00016240: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016250: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00016260: 7661 725f 6163 6320 3d20 5b5d 0d0a 0d0a  var_acc = []....
+00016270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016280: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+00016290: 5f6d 6561 6e5f 6469 7265 6374 696f 6e61  _mean_directiona
+000162a0: 6c5f 6368 616e 6765 203d 205b 5d0d 0a20  l_change = [].. 
+000162b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000162c0: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+000162d0: 7661 725f 6469 7265 6374 696f 6e61 6c5f  var_directional_
+000162e0: 6368 616e 6765 203d 205b 5d0d 0a0d 0a20  change = [].... 
+000162f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016300: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00016310: 6d65 616e 5f64 6973 7461 6e63 655f 6365  mean_distance_ce
+00016320: 6c6c 5f6d 6173 6b20 3d20 5b5d 0d0a 2020  ll_mask = []..  
+00016330: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016340: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+00016350: 6172 5f64 6973 7461 6e63 655f 6365 6c6c  ar_distance_cell
+00016360: 5f6d 6173 6b20 3d20 5b5d 0d0a 0d0a 2020  _mask = []....  
+00016370: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016380: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7370  lf.all_mean_disp
+00016390: 5f7a 203d 205b 5d0d 0a20 2020 2020 2020  _z = []..       
+000163a0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
+000163b0: 6c5f 7661 725f 6469 7370 5f7a 203d 205b  l_var_disp_z = [
+000163c0: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+000163d0: 2020 2020 2073 656c 662e 616c 6c5f 6d65       self.all_me
+000163e0: 616e 5f64 6973 705f 7920 3d20 5b5d 0d0a  an_disp_y = []..
+000163f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016400: 7365 6c66 2e61 6c6c 5f76 6172 5f64 6973  self.all_var_dis
+00016410: 705f 7920 3d20 5b5d 0d0a 0d0a 2020 2020  p_y = []....    
+00016420: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016430: 2e61 6c6c 5f6d 6561 6e5f 6469 7370 5f78  .all_mean_disp_x
+00016440: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016450: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00016460: 7661 725f 6469 7370 5f78 203d 205b 5d0d  var_disp_x = [].
+00016470: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00016480: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
+00016490: 5f72 6164 6975 7320 3d20 5b5d 0d0a 2020  _radius = []..  
+000164a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000164b0: 6c66 2e61 6c6c 5f76 6172 5f72 6164 6975  lf.all_var_radiu
+000164c0: 7320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  s = []....      
+000164d0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000164e0: 6c6c 5f6d 6561 6e5f 7370 6565 6420 3d20  ll_mean_speed = 
+000164f0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016500: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
+00016510: 5f73 7065 6564 203d 205b 5d0d 0a0d 0a20  _speed = [].... 
+00016520: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016530: 656c 662e 616c 6c5f 6d65 616e 5f61 6363  elf.all_mean_acc
+00016540: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016550: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00016560: 7661 725f 6163 6320 3d20 5b5d 0d0a 0d0a  var_acc = []....
+00016570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016580: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 6469  self.all_mean_di
+00016590: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+000165a0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+000165b0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+000165c0: 7661 725f 6469 7265 6374 696f 6e61 6c5f  var_directional_
+000165d0: 6368 616e 6765 203d 205b 5d0d 0a0d 0a20  change = [].... 
+000165e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000165f0: 656c 662e 616c 6c5f 6d65 616e 5f64 6973  elf.all_mean_dis
+00016600: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
+00016610: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016620: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
+00016630: 6172 5f64 6973 7461 6e63 655f 6365 6c6c  ar_distance_cell
+00016640: 5f6d 6173 6b20 3d20 5b5d 0d0a 0d0a 2020  _mask = []....  
+00016650: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016660: 6c66 2e6d 6974 6f74 6963 5f63 6c75 7374  lf.mitotic_clust
+00016670: 6572 5f63 6c61 7373 203d 205b 5d0d 0a20  er_class = [].. 
+00016680: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016690: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+000166a0: 636c 7573 7465 725f 636c 6173 7320 3d20  cluster_class = 
+000166b0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+000166c0: 2020 2020 7365 6c66 2e61 6c6c 5f63 6c75      self.all_clu
+000166d0: 7374 6572 5f63 6c61 7373 203d 205b 5d0d  ster_class = [].
+000166e0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000166f0: 2020 2061 6c6c 5f73 706f 7473 5f74 7261     all_spots_tra
+00016700: 636b 7320 3d20 7b7d 0d0a 2020 2020 2020  cks = {}..      
+00016710: 2020 2020 2020 2020 2020 666f 7220 286b            for (k
+00016720: 2c76 2920 696e 2073 656c 662e 756e 6971  ,v) in self.uniq
+00016730: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+00016740: 6573 2e69 7465 6d73 2829 3a0d 0a20 2020  es.items():..   
 00016750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016760: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016770: 2020 2020 2020 2020 616c 6c5f 7370 6f74          all_spot
-00016780: 7320 3d20 7365 6c66 2e75 6e69 7175 655f  s = self.unique_
-00016790: 7370 6f74 5f70 726f 7065 7274 6965 735b  spot_properties[
-000167a0: 6b5d 0d0a 2020 2020 2020 2020 2020 2020  k]..            
-000167b0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-000167c0: 662e 7472 6163 6b69 645f 6b65 7920 696e  f.trackid_key in
-000167d0: 2061 6c6c 5f73 706f 7473 3a0d 0a20 2020   all_spots:..   
+00016760: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+00016770: 2020 2020 2020 2020 2020 2061 6c6c 5f73             all_s
+00016780: 706f 7473 203d 2073 656c 662e 756e 6971  pots = self.uniq
+00016790: 7565 5f73 706f 745f 7072 6f70 6572 7469  ue_spot_properti
+000167a0: 6573 5b6b 5d0d 0a20 2020 2020 2020 2020  es[k]..         
+000167b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000167c0: 7365 6c66 2e74 7261 636b 6964 5f6b 6579  self.trackid_key
+000167d0: 2069 6e20 616c 6c5f 7370 6f74 733a 0d0a   in all_spots:..
 000167e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000167f0: 2020 2020 2020 2061 6c6c 5f73 706f 7473         all_spots
-00016800: 5f74 7261 636b 735b 6b5d 203d 2061 6c6c  _tracks[k] = all
-00016810: 5f73 706f 7473 0d0a 2020 2020 2020 2020  _spots..        
-00016820: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
-00016830: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00016840: 2020 2020 2020 2020 2020 2020 2020 6675                fu
-00016850: 7475 7265 7320 3d20 5b5d 0d0a 2020 2020  tures = []..    
-00016860: 2020 2020 2020 2020 2020 2020 7769 7468              with
-00016870: 2063 6f6e 6375 7272 656e 742e 6675 7475   concurrent.futu
-00016880: 7265 732e 5468 7265 6164 506f 6f6c 4578  res.ThreadPoolEx
-00016890: 6563 7574 6f72 286d 6178 5f77 6f72 6b65  ecutor(max_worke
-000168a0: 7273 203d 206f 732e 6370 755f 636f 756e  rs = os.cpu_coun
-000168b0: 7428 2929 2061 7320 6578 6563 7574 6f72  t()) as executor
-000168c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000168d0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-000168e0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000168f0: 6f72 2069 2069 6e20 7471 646d 2872 616e  or i in tqdm(ran
-00016900: 6765 2873 7461 7274 7469 6d65 2c20 656e  ge(starttime, en
-00016910: 6474 696d 6529 2c20 746f 7461 6c3d 656e  dtime), total=en
-00016920: 6474 696d 6520 2d20 7374 6172 7474 696d  dtime - starttim
-00016930: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
-00016940: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+000167f0: 2020 2020 2020 2020 2020 616c 6c5f 7370            all_sp
+00016800: 6f74 735f 7472 6163 6b73 5b6b 5d20 3d20  ots_tracks[k] = 
+00016810: 616c 6c5f 7370 6f74 730d 0a20 2020 2020  all_spots..     
+00016820: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
+00016830: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00016840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016850: 2066 7574 7572 6573 203d 205b 5d0d 0a20   futures = [].. 
+00016860: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00016870: 6974 6820 636f 6e63 7572 7265 6e74 2e66  ith concurrent.f
+00016880: 7574 7572 6573 2e54 6872 6561 6450 6f6f  utures.ThreadPoo
+00016890: 6c45 7865 6375 746f 7228 6d61 785f 776f  lExecutor(max_wo
+000168a0: 726b 6572 7320 3d20 6f73 2e63 7075 5f63  rkers = os.cpu_c
+000168b0: 6f75 6e74 2829 2920 6173 2065 7865 6375  ount()) as execu
+000168c0: 746f 723a 0d0a 2020 2020 2020 2020 2020  tor:..          
+000168d0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+000168e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168f0: 2020 666f 7220 6920 696e 2074 7164 6d28    for i in tqdm(
+00016900: 7261 6e67 6528 7374 6172 7474 696d 652c  range(starttime,
+00016910: 2065 6e64 7469 6d65 292c 2074 6f74 616c   endtime), total
+00016920: 3d65 6e64 7469 6d65 202d 2073 7461 7274  =endtime - start
+00016930: 7469 6d65 293a 0d0a 2020 2020 2020 2020  time):..        
+00016940: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
 00016950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016960: 2020 2020 2066 7574 7572 6573 2e61 7070       futures.app
-00016970: 656e 6428 6578 6563 7574 6f72 2e73 7562  end(executor.sub
-00016980: 6d69 7428 7365 6c66 2e5f 636f 6d70 7574  mit(self._comput
-00016990: 655f 7465 6d70 6f72 616c 2c20 692c 2061  e_temporal, i, a
-000169a0: 6c6c 5f73 706f 7473 5f74 7261 636b 7329  ll_spots_tracks)
-000169b0: 290d 0a20 0d0a 2020 2020 2020 2020 2020  ).. ..          
-000169c0: 2020 2020 2020 2020 2020 5b72 2e72 6573            [r.res
-000169d0: 756c 7428 2920 666f 7220 7220 696e 2063  ult() for r in c
-000169e0: 6f6e 6375 7272 656e 742e 6675 7475 7265  oncurrent.future
-000169f0: 732e 6173 5f63 6f6d 706c 6574 6564 2866  s.as_completed(f
-00016a00: 7574 7572 6573 295d 0d0a 0d0a 0d0a 2020  utures)]......  
-00016a10: 2020 6465 6620 5f63 6f6d 7075 7465 5f74    def _compute_t
-00016a20: 656d 706f 7261 6c28 7365 6c66 2c20 692c  emporal(self, i,
-00016a30: 2061 6c6c 5f73 706f 7473 5f74 7261 636b   all_spots_track
-00016a40: 7329 3a20 2020 2020 2020 2020 2020 2020  s):             
-00016a50: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00016a60: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00016a70: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 2020  _disp_z = []..  
-00016a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a90: 2020 6d69 746f 7469 635f 6469 7370 5f79    mitotic_disp_y
-00016aa0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016ab0: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00016ac0: 6963 5f64 6973 705f 7820 3d20 5b5d 0d0a  ic_disp_x = []..
-00016ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ae0: 2020 2020 6d69 746f 7469 635f 7261 6469      mitotic_radi
-00016af0: 7573 203d 205b 5d0d 0a20 2020 2020 2020  us = []..       
-00016b00: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-00016b10: 6f74 6963 5f73 7065 6564 203d 205b 5d0d  otic_speed = [].
-00016b20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016b30: 2020 2020 206d 6974 6f74 6963 5f61 6363       mitotic_acc
-00016b40: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016b50: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00016b60: 6963 5f64 6972 6563 7469 6f6e 616c 5f63  ic_directional_c
-00016b70: 6861 6e67 6520 3d20 5b5d 0d0a 2020 2020  hange = []..    
+00016960: 2020 2020 2020 2020 6675 7475 7265 732e          futures.
+00016970: 6170 7065 6e64 2865 7865 6375 746f 722e  append(executor.
+00016980: 7375 626d 6974 2873 656c 662e 5f63 6f6d  submit(self._com
+00016990: 7075 7465 5f74 656d 706f 7261 6c2c 2069  pute_temporal, i
+000169a0: 2c20 616c 6c5f 7370 6f74 735f 7472 6163  , all_spots_trac
+000169b0: 6b73 2929 0d0a 200d 0a20 2020 2020 2020  ks)).. ..       
+000169c0: 2020 2020 2020 2020 2020 2020 205b 722e               [r.
+000169d0: 7265 7375 6c74 2829 2066 6f72 2072 2069  result() for r i
+000169e0: 6e20 636f 6e63 7572 7265 6e74 2e66 7574  n concurrent.fut
+000169f0: 7572 6573 2e61 735f 636f 6d70 6c65 7465  ures.as_complete
+00016a00: 6428 6675 7475 7265 7329 5d0d 0a0d 0a0d  d(futures)].....
+00016a10: 0a20 2020 2064 6566 205f 636f 6d70 7574  .    def _comput
+00016a20: 655f 7465 6d70 6f72 616c 2873 656c 662c  e_temporal(self,
+00016a30: 2069 2c20 616c 6c5f 7370 6f74 735f 7472   i, all_spots_tr
+00016a40: 6163 6b73 293a 2020 2020 2020 2020 2020  acks):          
+00016a50: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00016a60: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
+00016a70: 7469 635f 6469 7370 5f7a 203d 205b 5d0d  tic_disp_z = [].
+00016a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016a90: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
+00016aa0: 705f 7920 3d20 5b5d 0d0a 2020 2020 2020  p_y = []..      
+00016ab0: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+00016ac0: 746f 7469 635f 6469 7370 5f78 203d 205b  totic_disp_x = [
+00016ad0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016ae0: 2020 2020 2020 206d 6974 6f74 6963 5f72         mitotic_r
+00016af0: 6164 6975 7320 3d20 5b5d 0d0a 2020 2020  adius = []..    
+00016b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b10: 6d69 746f 7469 635f 7370 6565 6420 3d20  mitotic_speed = 
+00016b20: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016b30: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+00016b40: 6163 6320 3d20 5b5d 0d0a 2020 2020 2020  acc = []..      
+00016b50: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+00016b60: 746f 7469 635f 6469 7265 6374 696f 6e61  totic_directiona
+00016b70: 6c5f 6368 616e 6765 203d 205b 5d0d 0a20  l_change = [].. 
 00016b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b90: 6d69 746f 7469 635f 636c 7573 7465 725f  mitotic_cluster_
-00016ba0: 636c 6173 7320 3d20 5b5d 0d0a 2020 2020  class = []..    
+00016b90: 2020 206d 6974 6f74 6963 5f63 6c75 7374     mitotic_clust
+00016ba0: 6572 5f63 6c61 7373 203d 205b 5d0d 0a20  er_class = [].. 
 00016bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016bc0: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
-00016bd0: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
-00016be0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00016bf0: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
-00016c00: 6963 5f64 6973 705f 7a20 3d20 5b5d 0d0a  ic_disp_z = []..
-00016c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c20: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-00016c30: 6469 7370 5f79 203d 205b 5d0d 0a20 2020  disp_y = []..   
+00016bc0: 2020 206d 6974 6f74 6963 5f64 6973 7461     mitotic_dista
+00016bd0: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
+00016be0: 5b5d 0d0a 0d0a 2020 2020 2020 2020 2020  []....          
+00016bf0: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+00016c00: 746f 7469 635f 6469 7370 5f7a 203d 205b  totic_disp_z = [
+00016c10: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016c20: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
+00016c30: 6963 5f64 6973 705f 7920 3d20 5b5d 0d0a  ic_disp_y = []..
 00016c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c50: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6973   non_mitotic_dis
-00016c60: 705f 7820 3d20 5b5d 0d0a 2020 2020 2020  p_x = []..      
-00016c70: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00016c80: 6e5f 6d69 746f 7469 635f 7261 6469 7573  n_mitotic_radius
-00016c90: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
-00016ca0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-00016cb0: 6974 6f74 6963 5f73 7065 6564 203d 205b  itotic_speed = [
-00016cc0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016cd0: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
-00016ce0: 6963 5f61 6363 203d 205b 5d0d 0a20 2020  ic_acc = []..   
+00016c50: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+00016c60: 6469 7370 5f78 203d 205b 5d0d 0a20 2020  disp_x = []..   
+00016c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c80: 206e 6f6e 5f6d 6974 6f74 6963 5f72 6164   non_mitotic_rad
+00016c90: 6975 7320 3d20 5b5d 0d0a 2020 2020 2020  ius = []..      
+00016ca0: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00016cb0: 6e5f 6d69 746f 7469 635f 7370 6565 6420  n_mitotic_speed 
+00016cc0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016cd0: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
+00016ce0: 746f 7469 635f 6163 6320 3d20 5b5d 0d0a  totic_acc = []..
 00016cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d00: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6972   non_mitotic_dir
-00016d10: 6563 7469 6f6e 616c 5f63 6861 6e67 6520  ectional_change 
-00016d20: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-00016d30: 2020 2020 2020 2020 2020 6e6f 6e5f 6d69            non_mi
-00016d40: 746f 7469 635f 636c 7573 7465 725f 636c  totic_cluster_cl
-00016d50: 6173 7320 3d20 5b5d 0d0a 2020 2020 2020  ass = []..      
-00016d60: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
-00016d70: 6e5f 6d69 746f 7469 635f 6469 7374 616e  n_mitotic_distan
-00016d80: 6365 5f63 656c 6c5f 6d61 736b 203d 205b  ce_cell_mask = [
-00016d90: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016da0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00016db0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-00016dc0: 5f64 6973 705f 7a20 3d20 5b5d 0d0a 2020  _disp_z = []..  
-00016dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016de0: 2020 616c 6c5f 6469 7370 5f79 203d 205b    all_disp_y = [
-00016df0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016e00: 2020 2020 2020 2061 6c6c 5f64 6973 705f         all_disp_
-00016e10: 7820 3d20 5b5d 0d0a 2020 2020 2020 2020  x = []..        
-00016e20: 2020 2020 2020 2020 2020 2020 616c 6c5f              all_
-00016e30: 7261 6469 7573 203d 205b 5d0d 0a20 2020  radius = []..   
+00016d00: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+00016d10: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+00016d20: 6765 203d 205b 5d0d 0a20 2020 2020 2020  ge = []..       
+00016d30: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
+00016d40: 5f6d 6974 6f74 6963 5f63 6c75 7374 6572  _mitotic_cluster
+00016d50: 5f63 6c61 7373 203d 205b 5d0d 0a20 2020  _class = []..   
+00016d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d70: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6973   non_mitotic_dis
+00016d80: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b20  tance_cell_mask 
+00016d90: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016da0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00016db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016dc0: 616c 6c5f 6469 7370 5f7a 203d 205b 5d0d  all_disp_z = [].
+00016dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016de0: 2020 2020 2061 6c6c 5f64 6973 705f 7920       all_disp_y 
+00016df0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016e00: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
+00016e10: 7370 5f78 203d 205b 5d0d 0a20 2020 2020  sp_x = []..     
+00016e20: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00016e30: 6c6c 5f72 6164 6975 7320 3d20 5b5d 0d0a  ll_radius = []..
 00016e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e50: 2061 6c6c 5f73 7065 6564 203d 205b 5d0d   all_speed = [].
-00016e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016e70: 2020 2020 2061 6c6c 5f61 6363 203d 205b       all_acc = [
-00016e80: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00016e90: 2020 2020 2020 2061 6c6c 5f64 6972 6563         all_direc
-00016ea0: 7469 6f6e 616c 5f63 6861 6e67 6520 3d20  tional_change = 
-00016eb0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
-00016ec0: 2020 2020 2020 2020 616c 6c5f 636c 7573          all_clus
-00016ed0: 7465 725f 636c 6173 7320 3d20 5b5d 0d0a  ter_class = []..
-00016ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ef0: 2020 2020 616c 6c5f 6469 7374 616e 6365      all_distance
-00016f00: 5f63 656c 6c5f 6d61 736b 203d 205b 5d0d  _cell_mask = [].
-00016f10: 0a0d 0a0d 0a0d 0a0d 0a20 2020 2020 2020  .........       
-00016f20: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00016f30: 2028 6b2c 7629 2069 6e20 616c 6c5f 7370   (k,v) in all_sp
-00016f40: 6f74 735f 7472 6163 6b73 2e69 7465 6d73  ots_tracks.items
-00016f50: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+00016e50: 2020 2020 616c 6c5f 7370 6565 6420 3d20      all_speed = 
+00016e60: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+00016e70: 2020 2020 2020 2020 616c 6c5f 6163 6320          all_acc 
+00016e80: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
+00016e90: 2020 2020 2020 2020 2020 616c 6c5f 6469            all_di
+00016ea0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00016eb0: 203d 205b 5d0d 0a20 2020 2020 2020 2020   = []..         
+00016ec0: 2020 2020 2020 2020 2020 2061 6c6c 5f63             all_c
+00016ed0: 6c75 7374 6572 5f63 6c61 7373 203d 205b  luster_class = [
+00016ee0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00016ef0: 2020 2020 2020 2061 6c6c 5f64 6973 7461         all_dista
+00016f00: 6e63 655f 6365 6c6c 5f6d 6173 6b20 3d20  nce_cell_mask = 
+00016f10: 5b5d 0d0a 0d0a 0d0a 0d0a 0d0a 2020 2020  []..........    
+00016f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f30: 666f 7220 286b 2c76 2920 696e 2061 6c6c  for (k,v) in all
+00016f40: 5f73 706f 7473 5f74 7261 636b 732e 6974  _spots_tracks.it
+00016f50: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
 00016f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f70: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-00016f80: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00016f90: 7572 7265 6e74 5f74 696d 6520 3d20 616c  urrent_time = al
-00016fa0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-00016fb0: 5d5b 7365 6c66 2e66 7261 6d65 6964 5f6b  ][self.frameid_k
-00016fc0: 6579 5d0d 0a20 2020 2020 2020 2020 2020  ey]..           
+00016f70: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
+00016f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f90: 2020 6375 7272 656e 745f 7469 6d65 203d    current_time =
+00016fa0: 2061 6c6c 5f73 706f 7473 5f74 7261 636b   all_spots_track
+00016fb0: 735b 6b5d 5b73 656c 662e 6672 616d 6569  s[k][self.framei
+00016fc0: 645f 6b65 795d 0d0a 2020 2020 2020 2020  d_key]..        
 00016fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fe0: 206d 6974 6f74 6963 203d 2061 6c6c 5f73   mitotic = all_s
-00016ff0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
-00017000: 656c 662e 6469 7669 6469 6e67 5f6b 6579  elf.dividing_key
-00017010: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00017020: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00017030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017040: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00017050: 203d 3d20 696e 7428 6375 7272 656e 745f   == int(current_
-00017060: 7469 6d65 293a 0d0a 2020 2020 2020 2020  time):..        
+00016fe0: 2020 2020 6d69 746f 7469 6320 3d20 616c      mitotic = al
+00016ff0: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
+00017000: 5d5b 7365 6c66 2e64 6976 6964 696e 675f  ][self.dividing_
+00017010: 6b65 795d 0d0a 2020 2020 2020 2020 2020  key]..          
+00017020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017030: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00017040: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00017050: 6620 6920 3d3d 2069 6e74 2863 7572 7265  f i == int(curre
+00017060: 6e74 5f74 696d 6529 3a0d 0a20 2020 2020  nt_time):..     
 00017070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017080: 2020 2020 2020 2020 2020 6966 206d 6974            if mit
-00017090: 6f74 6963 3a0d 0a20 2020 2020 2020 2020  otic:..         
+00017080: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00017090: 6d69 746f 7469 633a 0d0a 2020 2020 2020  mitotic:..      
 000170a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170b0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000170c0: 6974 6f74 6963 5f64 6973 705f 7a2e 6170  itotic_disp_z.ap
-000170d0: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-000170e0: 7261 636b 735b 6b5d 5b73 656c 662e 7a70  racks[k][self.zp
-000170f0: 6f73 6964 5f6b 6579 5d29 0d0a 2020 2020  osid_key])..    
+000170b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170c0: 2020 6d69 746f 7469 635f 6469 7370 5f7a    mitotic_disp_z
+000170d0: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
+000170e0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+000170f0: 2e7a 706f 7369 645f 6b65 795d 290d 0a20  .zposid_key]).. 
 00017100: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017120: 2020 2020 6d69 746f 7469 635f 6469 7370      mitotic_disp
-00017130: 5f79 2e61 7070 656e 6428 616c 6c5f 7370  _y.append(all_sp
-00017140: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00017150: 6c66 2e79 706f 7369 645f 6b65 795d 290d  lf.yposid_key]).
-00017160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017120: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
+00017130: 6973 705f 792e 6170 7065 6e64 2861 6c6c  isp_y.append(all
+00017140: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00017150: 5b73 656c 662e 7970 6f73 6964 5f6b 6579  [self.yposid_key
+00017160: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
 00017170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017180: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
-00017190: 5f64 6973 705f 782e 6170 7065 6e64 2861  _disp_x.append(a
-000171a0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-000171b0: 6b5d 5b73 656c 662e 7870 6f73 6964 5f6b  k][self.xposid_k
-000171c0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+00017180: 2020 2020 2020 2020 2020 2020 6d69 746f              mito
+00017190: 7469 635f 6469 7370 5f78 2e61 7070 656e  tic_disp_x.appen
+000171a0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+000171b0: 6b73 5b6b 5d5b 7365 6c66 2e78 706f 7369  ks[k][self.xposi
+000171c0: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
 000171d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171e0: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-000171f0: 746f 7469 635f 7261 6469 7573 2e61 7070  totic_radius.app
-00017200: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-00017210: 6163 6b73 5b6b 5d5b 7365 6c66 2e72 6164  acks[k][self.rad
-00017220: 6975 735f 6b65 795d 290d 0a20 2020 2020  ius_key])..     
+000171e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000171f0: 206d 6974 6f74 6963 5f72 6164 6975 732e   mitotic_radius.
+00017200: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00017210: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+00017220: 7261 6469 7573 5f6b 6579 5d29 0d0a 2020  radius_key])..  
 00017230: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017250: 2020 206d 6974 6f74 6963 5f73 7065 6564     mitotic_speed
-00017260: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-00017270: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-00017280: 2e73 7065 6564 5f6b 6579 5d29 0d0a 2020  .speed_key])..  
-00017290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017250: 2020 2020 2020 6d69 746f 7469 635f 7370        mitotic_sp
+00017260: 6565 642e 6170 7065 6e64 2861 6c6c 5f73  eed.append(all_s
+00017270: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+00017280: 656c 662e 7370 6565 645f 6b65 795d 290d  elf.speed_key]).
+00017290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000172a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000172b0: 2020 2020 2020 6d69 746f 7469 635f 6163        mitotic_ac
-000172c0: 632e 6170 7065 6e64 2861 6c6c 5f73 706f  c.append(all_spo
-000172d0: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-000172e0: 662e 6163 6365 6c65 7261 7469 6f6e 5f6b  f.acceleration_k
-000172f0: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+000172b0: 2020 2020 2020 2020 206d 6974 6f74 6963           mitotic
+000172c0: 5f61 6363 2e61 7070 656e 6428 616c 6c5f  _acc.append(all_
+000172d0: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+000172e0: 7365 6c66 2e61 6363 656c 6572 6174 696f  self.acceleratio
+000172f0: 6e5f 6b65 795d 290d 0a20 2020 2020 2020  n_key])..       
 00017300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017310: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00017320: 746f 7469 635f 6469 7265 6374 696f 6e61  totic_directiona
-00017330: 6c5f 6368 616e 6765 2e61 7070 656e 6428  l_change.append(
-00017340: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-00017350: 5b6b 5d5b 7365 6c66 2e6d 6f74 696f 6e5f  [k][self.motion_
-00017360: 616e 676c 655f 6b65 795d 290d 0a20 2020  angle_key])..   
+00017310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017320: 206d 6974 6f74 6963 5f64 6972 6563 7469   mitotic_directi
+00017330: 6f6e 616c 5f63 6861 6e67 652e 6170 7065  onal_change.appe
+00017340: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
+00017350: 636b 735b 6b5d 5b73 656c 662e 6d6f 7469  cks[k][self.moti
+00017360: 6f6e 5f61 6e67 6c65 5f6b 6579 5d29 0d0a  on_angle_key])..
 00017370: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017390: 2020 2020 206d 6974 6f74 6963 5f64 6973       mitotic_dis
-000173a0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
-000173b0: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-000173c0: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-000173d0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-000173e0: 736b 5f6b 6579 5d29 0d0a 2020 2020 2020  sk_key])..      
+00017390: 2020 2020 2020 2020 6d69 746f 7469 635f          mitotic_
+000173a0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+000173b0: 736b 2e61 7070 656e 6428 616c 6c5f 7370  sk.append(all_sp
+000173c0: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+000173d0: 6c66 2e64 6973 7461 6e63 655f 6365 6c6c  lf.distance_cell
+000173e0: 5f6d 6173 6b5f 6b65 795d 290d 0a20 2020  _mask_key])..   
 000173f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017410: 2020 6966 2073 656c 662e 636c 7573 7465    if self.cluste
-00017420: 7263 6c61 7373 5f6b 6579 2069 6e20 616c  rclass_key in al
-00017430: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-00017440: 5d2e 6b65 7973 2829 203a 0d0a 2020 2020  ].keys() :..    
+00017410: 2020 2020 2069 6620 7365 6c66 2e63 6c75       if self.clu
+00017420: 7374 6572 636c 6173 735f 6b65 7920 696e  sterclass_key in
+00017430: 2061 6c6c 5f73 706f 7473 5f74 7261 636b   all_spots_track
+00017440: 735b 6b5d 2e6b 6579 7328 2920 3a0d 0a20  s[k].keys() :.. 
 00017450: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017470: 2020 2020 2020 2020 2020 206d 6974 6f74             mitot
-00017480: 6963 5f63 6c75 7374 6572 5f63 6c61 7373  ic_cluster_class
-00017490: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
-000174a0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
-000174b0: 2e63 6c75 7374 6572 636c 6173 735f 6b65  .clusterclass_ke
-000174c0: 795d 290d 0a0d 0a0d 0a20 2020 2020 2020  y])......       
+00017470: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
+00017480: 746f 7469 635f 636c 7573 7465 725f 636c  totic_cluster_cl
+00017490: 6173 732e 6170 7065 6e64 2861 6c6c 5f73  ass.append(all_s
+000174a0: 706f 7473 5f74 7261 636b 735b 6b5d 5b73  pots_tracks[k][s
+000174b0: 656c 662e 636c 7573 7465 7263 6c61 7373  elf.clusterclass
+000174c0: 5f6b 6579 5d29 0d0a 0d0a 0d0a 2020 2020  _key])......    
 000174d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174e0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-000174f0: 7420 6d69 746f 7469 633a 0d0a 2020 2020  t mitotic:..    
+000174e0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000174f0: 206e 6f74 206d 6974 6f74 6963 3a0d 0a20   not mitotic:.. 
 00017500: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017520: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
-00017530: 6469 7370 5f7a 2e61 7070 656e 6428 616c  disp_z.append(al
-00017540: 6c5f 7370 6f74 735f 7472 6163 6b73 5b6b  l_spots_tracks[k
-00017550: 5d5b 7365 6c66 2e7a 706f 7369 645f 6b65  ][self.zposid_ke
-00017560: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+00017520: 2020 2020 2020 206e 6f6e 5f6d 6974 6f74         non_mitot
+00017530: 6963 5f64 6973 705f 7a2e 6170 7065 6e64  ic_disp_z.append
+00017540: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
+00017550: 735b 6b5d 5b73 656c 662e 7a70 6f73 6964  s[k][self.zposid
+00017560: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
 00017570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017580: 2020 2020 2020 2020 2020 2020 206e 6f6e               non
-00017590: 5f6d 6974 6f74 6963 5f64 6973 705f 792e  _mitotic_disp_y.
-000175a0: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
-000175b0: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
-000175c0: 7970 6f73 6964 5f6b 6579 5d29 0d0a 2020  yposid_key])..  
-000175d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017590: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
+000175a0: 5f79 2e61 7070 656e 6428 616c 6c5f 7370  _y.append(all_sp
+000175b0: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
+000175c0: 6c66 2e79 706f 7369 645f 6b65 795d 290d  lf.yposid_key]).
+000175d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000175e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175f0: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
-00017600: 635f 6469 7370 5f78 2e61 7070 656e 6428  c_disp_x.append(
-00017610: 616c 6c5f 7370 6f74 735f 7472 6163 6b73  all_spots_tracks
-00017620: 5b6b 5d5b 7365 6c66 2e78 706f 7369 645f  [k][self.xposid_
-00017630: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+000175f0: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+00017600: 6f74 6963 5f64 6973 705f 782e 6170 7065  otic_disp_x.appe
+00017610: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
+00017620: 636b 735b 6b5d 5b73 656c 662e 7870 6f73  cks[k][self.xpos
+00017630: 6964 5f6b 6579 5d29 0d0a 2020 2020 2020  id_key])..      
 00017640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017650: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00017660: 6f6e 5f6d 6974 6f74 6963 5f72 6164 6975  on_mitotic_radiu
-00017670: 732e 6170 7065 6e64 2861 6c6c 5f73 706f  s.append(all_spo
-00017680: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
-00017690: 662e 7261 6469 7573 5f6b 6579 5d29 0d0a  f.radius_key])..
-000176a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017660: 2020 6e6f 6e5f 6d69 746f 7469 635f 7261    non_mitotic_ra
+00017670: 6469 7573 2e61 7070 656e 6428 616c 6c5f  dius.append(all_
+00017680: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
+00017690: 7365 6c66 2e72 6164 6975 735f 6b65 795d  self.radius_key]
+000176a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 000176b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176c0: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
-000176d0: 7469 635f 7370 6565 642e 6170 7065 6e64  tic_speed.append
-000176e0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-000176f0: 735b 6b5d 5b73 656c 662e 7370 6565 645f  s[k][self.speed_
-00017700: 6b65 795d 290d 0a20 2020 2020 2020 2020  key])..         
+000176c0: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
+000176d0: 6974 6f74 6963 5f73 7065 6564 2e61 7070  itotic_speed.app
+000176e0: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+000176f0: 6163 6b73 5b6b 5d5b 7365 6c66 2e73 7065  acks[k][self.spe
+00017700: 6564 5f6b 6579 5d29 0d0a 2020 2020 2020  ed_key])..      
 00017710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017720: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00017730: 6f6e 5f6d 6974 6f74 6963 5f61 6363 2e61  on_mitotic_acc.a
-00017740: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00017750: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e61  tracks[k][self.a
-00017760: 6363 656c 6572 6174 696f 6e5f 6b65 795d  cceleration_key]
-00017770: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00017720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017730: 2020 6e6f 6e5f 6d69 746f 7469 635f 6163    non_mitotic_ac
+00017740: 632e 6170 7065 6e64 2861 6c6c 5f73 706f  c.append(all_spo
+00017750: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00017760: 662e 6163 6365 6c65 7261 7469 6f6e 5f6b  f.acceleration_k
+00017770: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
 00017780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017790: 2020 2020 2020 2020 2020 206e 6f6e 5f6d             non_m
-000177a0: 6974 6f74 6963 5f64 6972 6563 7469 6f6e  itotic_direction
-000177b0: 616c 5f63 6861 6e67 652e 6170 7065 6e64  al_change.append
-000177c0: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-000177d0: 735b 6b5d 5b73 656c 662e 6d6f 7469 6f6e  s[k][self.motion
-000177e0: 5f61 6e67 6c65 5f6b 6579 5d29 0d0a 2020  _angle_key])..  
-000177f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017790: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+000177a0: 6e5f 6d69 746f 7469 635f 6469 7265 6374  n_mitotic_direct
+000177b0: 696f 6e61 6c5f 6368 616e 6765 2e61 7070  ional_change.app
+000177c0: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+000177d0: 6163 6b73 5b6b 5d5b 7365 6c66 2e6d 6f74  acks[k][self.mot
+000177e0: 696f 6e5f 616e 676c 655f 6b65 795d 290d  ion_angle_key]).
+000177f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00017800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017810: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
-00017820: 635f 6469 7374 616e 6365 5f63 656c 6c5f  c_distance_cell_
-00017830: 6d61 736b 2e61 7070 656e 6428 616c 6c5f  mask.append(all_
-00017840: 7370 6f74 735f 7472 6163 6b73 5b6b 5d5b  spots_tracks[k][
-00017850: 7365 6c66 2e64 6973 7461 6e63 655f 6365  self.distance_ce
-00017860: 6c6c 5f6d 6173 6b5f 6b65 795d 290d 0a20  ll_mask_key]).. 
-00017870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017810: 2020 2020 2020 2020 206e 6f6e 5f6d 6974           non_mit
+00017820: 6f74 6963 5f64 6973 7461 6e63 655f 6365  otic_distance_ce
+00017830: 6c6c 5f6d 6173 6b2e 6170 7065 6e64 2861  ll_mask.append(a
+00017840: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
+00017850: 6b5d 5b73 656c 662e 6469 7374 616e 6365  k][self.distance
+00017860: 5f63 656c 6c5f 6d61 736b 5f6b 6579 5d29  _cell_mask_key])
+00017870: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00017880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017890: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-000178a0: 6c75 7374 6572 636c 6173 735f 6b65 7920  lusterclass_key 
-000178b0: 696e 2061 6c6c 5f73 706f 7473 5f74 7261  in all_spots_tra
-000178c0: 636b 735b 6b5d 2e6b 6579 7328 2920 3a0d  cks[k].keys() :.
-000178d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017890: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+000178a0: 662e 636c 7573 7465 7263 6c61 7373 5f6b  f.clusterclass_k
+000178b0: 6579 2069 6e20 616c 6c5f 7370 6f74 735f  ey in all_spots_
+000178c0: 7472 6163 6b73 5b6b 5d2e 6b65 7973 2829  tracks[k].keys()
+000178d0: 203a 0d0a 2020 2020 2020 2020 2020 2020   :..            
 000178e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000178f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017900: 6e6f 6e5f 6d69 746f 7469 635f 636c 7573  non_mitotic_clus
-00017910: 7465 725f 636c 6173 732e 6170 7065 6e64  ter_class.append
-00017920: 2861 6c6c 5f73 706f 7473 5f74 7261 636b  (all_spots_track
-00017930: 735b 6b5d 5b73 656c 662e 636c 7573 7465  s[k][self.cluste
-00017940: 7263 6c61 7373 5f6b 6579 5d29 0d0a 0d0a  rclass_key])....
-00017950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017900: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f63     non_mitotic_c
+00017910: 6c75 7374 6572 5f63 6c61 7373 2e61 7070  luster_class.app
+00017920: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
+00017930: 6163 6b73 5b6b 5d5b 7365 6c66 2e63 6c75  acks[k][self.clu
+00017940: 7374 6572 636c 6173 735f 6b65 795d 290d  sterclass_key]).
+00017950: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
 00017960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017970: 2020 616c 6c5f 6469 7370 5f7a 2e61 7070    all_disp_z.app
-00017980: 656e 6428 616c 6c5f 7370 6f74 735f 7472  end(all_spots_tr
-00017990: 6163 6b73 5b6b 5d5b 7365 6c66 2e7a 706f  acks[k][self.zpo
-000179a0: 7369 645f 6b65 795d 290d 0a20 2020 2020  sid_key])..     
+00017970: 2020 2020 2061 6c6c 5f64 6973 705f 7a2e       all_disp_z.
+00017980: 6170 7065 6e64 2861 6c6c 5f73 706f 7473  append(all_spots
+00017990: 5f74 7261 636b 735b 6b5d 5b73 656c 662e  _tracks[k][self.
+000179a0: 7a70 6f73 6964 5f6b 6579 5d29 0d0a 2020  zposid_key])..  
 000179b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179c0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-000179d0: 5f64 6973 705f 792e 6170 7065 6e64 2861  _disp_y.append(a
-000179e0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-000179f0: 6b5d 5b73 656c 662e 7970 6f73 6964 5f6b  k][self.yposid_k
-00017a00: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+000179c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000179d0: 616c 6c5f 6469 7370 5f79 2e61 7070 656e  all_disp_y.appen
+000179e0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+000179f0: 6b73 5b6b 5d5b 7365 6c66 2e79 706f 7369  ks[k][self.yposi
+00017a00: 645f 6b65 795d 290d 0a20 2020 2020 2020  d_key])..       
 00017a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a20: 2020 2020 2020 2020 616c 6c5f 6469 7370          all_disp
-00017a30: 5f78 2e61 7070 656e 6428 616c 6c5f 7370  _x.append(all_sp
-00017a40: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00017a50: 6c66 2e78 706f 7369 645f 6b65 795d 290d  lf.xposid_key]).
-00017a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017a20: 2020 2020 2020 2020 2020 2061 6c6c 5f64             all_d
+00017a30: 6973 705f 782e 6170 7065 6e64 2861 6c6c  isp_x.append(all
+00017a40: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00017a50: 5b73 656c 662e 7870 6f73 6964 5f6b 6579  [self.xposid_key
+00017a60: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
 00017a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a80: 2020 2061 6c6c 5f72 6164 6975 732e 6170     all_radius.ap
-00017a90: 7065 6e64 2861 6c6c 5f73 706f 7473 5f74  pend(all_spots_t
-00017aa0: 7261 636b 735b 6b5d 5b73 656c 662e 7261  racks[k][self.ra
-00017ab0: 6469 7573 5f6b 6579 5d29 0d0a 2020 2020  dius_key])..    
+00017a80: 2020 2020 2020 616c 6c5f 7261 6469 7573        all_radius
+00017a90: 2e61 7070 656e 6428 616c 6c5f 7370 6f74  .append(all_spot
+00017aa0: 735f 7472 6163 6b73 5b6b 5d5b 7365 6c66  s_tracks[k][self
+00017ab0: 2e72 6164 6975 735f 6b65 795d 290d 0a20  .radius_key]).. 
 00017ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ad0: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00017ae0: 6c5f 7370 6565 642e 6170 7065 6e64 2861  l_speed.append(a
-00017af0: 6c6c 5f73 706f 7473 5f74 7261 636b 735b  ll_spots_tracks[
-00017b00: 6b5d 5b73 656c 662e 7370 6565 645f 6b65  k][self.speed_ke
-00017b10: 795d 290d 0a20 2020 2020 2020 2020 2020  y])..           
+00017ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ae0: 2061 6c6c 5f73 7065 6564 2e61 7070 656e   all_speed.appen
+00017af0: 6428 616c 6c5f 7370 6f74 735f 7472 6163  d(all_spots_trac
+00017b00: 6b73 5b6b 5d5b 7365 6c66 2e73 7065 6564  ks[k][self.speed
+00017b10: 5f6b 6579 5d29 0d0a 2020 2020 2020 2020  _key])..        
 00017b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b30: 2020 2020 2020 2061 6c6c 5f61 6363 2e61         all_acc.a
-00017b40: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
-00017b50: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e61  tracks[k][self.a
-00017b60: 6363 656c 6572 6174 696f 6e5f 6b65 795d  cceleration_key]
-00017b70: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00017b30: 2020 2020 2020 2020 2020 616c 6c5f 6163            all_ac
+00017b40: 632e 6170 7065 6e64 2861 6c6c 5f73 706f  c.append(all_spo
+00017b50: 7473 5f74 7261 636b 735b 6b5d 5b73 656c  ts_tracks[k][sel
+00017b60: 662e 6163 6365 6c65 7261 7469 6f6e 5f6b  f.acceleration_k
+00017b70: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
 00017b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b90: 2020 2020 2061 6c6c 5f64 6972 6563 7469       all_directi
-00017ba0: 6f6e 616c 5f63 6861 6e67 652e 6170 7065  onal_change.appe
-00017bb0: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00017bc0: 636b 735b 6b5d 5b73 656c 662e 6d6f 7469  cks[k][self.moti
-00017bd0: 6f6e 5f61 6e67 6c65 5f6b 6579 5d29 2020  on_angle_key])  
-00017be0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00017b90: 2020 2020 2020 2020 616c 6c5f 6469 7265          all_dire
+00017ba0: 6374 696f 6e61 6c5f 6368 616e 6765 2e61  ctional_change.a
+00017bb0: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00017bc0: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e6d  tracks[k][self.m
+00017bd0: 6f74 696f 6e5f 616e 676c 655f 6b65 795d  otion_angle_key]
+00017be0: 2920 2020 0d0a 2020 2020 2020 2020 2020  )   ..          
 00017bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c00: 2020 2020 2061 6c6c 5f64 6973 7461 6e63       all_distanc
-00017c10: 655f 6365 6c6c 5f6d 6173 6b2e 6170 7065  e_cell_mask.appe
-00017c20: 6e64 2861 6c6c 5f73 706f 7473 5f74 7261  nd(all_spots_tra
-00017c30: 636b 735b 6b5d 5b73 656c 662e 6469 7374  cks[k][self.dist
-00017c40: 616e 6365 5f63 656c 6c5f 6d61 736b 5f6b  ance_cell_mask_k
-00017c50: 6579 5d29 0d0a 2020 2020 2020 2020 2020  ey])..          
+00017c00: 2020 2020 2020 2020 616c 6c5f 6469 7374          all_dist
+00017c10: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
+00017c20: 7070 656e 6428 616c 6c5f 7370 6f74 735f  ppend(all_spots_
+00017c30: 7472 6163 6b73 5b6b 5d5b 7365 6c66 2e64  tracks[k][self.d
+00017c40: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00017c50: 6b5f 6b65 795d 290d 0a20 2020 2020 2020  k_key])..       
 00017c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c70: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00017c80: 636c 7573 7465 7263 6c61 7373 5f6b 6579  clusterclass_key
-00017c90: 2069 6e20 616c 6c5f 7370 6f74 735f 7472   in all_spots_tr
-00017ca0: 6163 6b73 5b6b 5d2e 6b65 7973 2829 203a  acks[k].keys() :
-00017cb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017c70: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00017c80: 6c66 2e63 6c75 7374 6572 636c 6173 735f  lf.clusterclass_
+00017c90: 6b65 7920 696e 2061 6c6c 5f73 706f 7473  key in all_spots
+00017ca0: 5f74 7261 636b 735b 6b5d 2e6b 6579 7328  _tracks[k].keys(
+00017cb0: 2920 3a0d 0a20 2020 2020 2020 2020 2020  ) :..           
 00017cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ce0: 2061 6c6c 5f63 6c75 7374 6572 5f63 6c61   all_cluster_cla
-00017cf0: 7373 2e61 7070 656e 6428 616c 6c5f 7370  ss.append(all_sp
-00017d00: 6f74 735f 7472 6163 6b73 5b6b 5d5b 7365  ots_tracks[k][se
-00017d10: 6c66 2e63 6c75 7374 6572 636c 6173 735f  lf.clusterclass_
-00017d20: 6b65 795d 2920 2020 200d 0a20 2020 2020  key])    ..     
+00017ce0: 2020 2020 616c 6c5f 636c 7573 7465 725f      all_cluster_
+00017cf0: 636c 6173 732e 6170 7065 6e64 2861 6c6c  class.append(all
+00017d00: 5f73 706f 7473 5f74 7261 636b 735b 6b5d  _spots_tracks[k]
+00017d10: 5b73 656c 662e 636c 7573 7465 7263 6c61  [self.clustercla
+00017d20: 7373 5f6b 6579 5d29 2020 2020 0d0a 2020  ss_key])    ..  
 00017d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d50: 2020 2020 2020 2020 200d 0a0d 0a20 2020           ....   
+00017d50: 2020 2020 2020 2020 2020 2020 0d0a 0d0a              ....
 00017d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d70: 206d 6974 6f74 6963 5f64 6973 705f 7a20   mitotic_disp_z 
-00017d80: 3d20 6e70 2e61 6273 286e 702e 6469 6666  = np.abs(np.diff
-00017d90: 286d 6974 6f74 6963 5f64 6973 705f 7a29  (mitotic_disp_z)
-00017da0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00017db0: 2020 2020 2020 206d 6974 6f74 6963 5f64         mitotic_d
-00017dc0: 6973 705f 7920 3d20 6e70 2e61 6273 286e  isp_y = np.abs(n
-00017dd0: 702e 6469 6666 286d 6974 6f74 6963 5f64  p.diff(mitotic_d
-00017de0: 6973 705f 7929 290d 0a20 2020 2020 2020  isp_y))..       
-00017df0: 2020 2020 2020 2020 2020 2020 206d 6974               mit
-00017e00: 6f74 6963 5f64 6973 705f 7820 3d20 6e70  otic_disp_x = np
-00017e10: 2e61 6273 286e 702e 6469 6666 286d 6974  .abs(np.diff(mit
-00017e20: 6f74 6963 5f64 6973 705f 7829 290d 0a0d  otic_disp_x))...
-00017e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017e40: 2020 2020 206e 6f6e 5f6d 6974 6f74 6963       non_mitotic
-00017e50: 5f64 6973 705f 7a20 3d20 6e70 2e61 6273  _disp_z = np.abs
-00017e60: 286e 702e 6469 6666 286e 6f6e 5f6d 6974  (np.diff(non_mit
-00017e70: 6f74 6963 5f64 6973 705f 7a29 290d 0a20  otic_disp_z)).. 
-00017e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e90: 2020 206e 6f6e 5f6d 6974 6f74 6963 5f64     non_mitotic_d
-00017ea0: 6973 705f 7920 3d20 6e70 2e61 6273 286e  isp_y = np.abs(n
-00017eb0: 702e 6469 6666 286e 6f6e 5f6d 6974 6f74  p.diff(non_mitot
-00017ec0: 6963 5f64 6973 705f 7929 290d 0a20 2020  ic_disp_y))..   
+00017d70: 2020 2020 6d69 746f 7469 635f 6469 7370      mitotic_disp
+00017d80: 5f7a 203d 206e 702e 6162 7328 6e70 2e64  _z = np.abs(np.d
+00017d90: 6966 6628 6d69 746f 7469 635f 6469 7370  iff(mitotic_disp
+00017da0: 5f7a 2929 0d0a 2020 2020 2020 2020 2020  _z))..          
+00017db0: 2020 2020 2020 2020 2020 6d69 746f 7469            mitoti
+00017dc0: 635f 6469 7370 5f79 203d 206e 702e 6162  c_disp_y = np.ab
+00017dd0: 7328 6e70 2e64 6966 6628 6d69 746f 7469  s(np.diff(mitoti
+00017de0: 635f 6469 7370 5f79 2929 0d0a 2020 2020  c_disp_y))..    
+00017df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e00: 6d69 746f 7469 635f 6469 7370 5f78 203d  mitotic_disp_x =
+00017e10: 206e 702e 6162 7328 6e70 2e64 6966 6628   np.abs(np.diff(
+00017e20: 6d69 746f 7469 635f 6469 7370 5f78 2929  mitotic_disp_x))
+00017e30: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00017e40: 2020 2020 2020 2020 6e6f 6e5f 6d69 746f          non_mito
+00017e50: 7469 635f 6469 7370 5f7a 203d 206e 702e  tic_disp_z = np.
+00017e60: 6162 7328 6e70 2e64 6966 6628 6e6f 6e5f  abs(np.diff(non_
+00017e70: 6d69 746f 7469 635f 6469 7370 5f7a 2929  mitotic_disp_z))
+00017e80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00017e90: 2020 2020 2020 6e6f 6e5f 6d69 746f 7469        non_mitoti
+00017ea0: 635f 6469 7370 5f79 203d 206e 702e 6162  c_disp_y = np.ab
+00017eb0: 7328 6e70 2e64 6966 6628 6e6f 6e5f 6d69  s(np.diff(non_mi
+00017ec0: 746f 7469 635f 6469 7370 5f79 2929 0d0a  totic_disp_y))..
 00017ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ee0: 206e 6f6e 5f6d 6974 6f74 6963 5f64 6973   non_mitotic_dis
-00017ef0: 705f 7820 3d20 6e70 2e61 6273 286e 702e  p_x = np.abs(np.
-00017f00: 6469 6666 286e 6f6e 5f6d 6974 6f74 6963  diff(non_mitotic
-00017f10: 5f64 6973 705f 7829 290d 0a0d 0a20 2020  _disp_x))....   
+00017ee0: 2020 2020 6e6f 6e5f 6d69 746f 7469 635f      non_mitotic_
+00017ef0: 6469 7370 5f78 203d 206e 702e 6162 7328  disp_x = np.abs(
+00017f00: 6e70 2e64 6966 6628 6e6f 6e5f 6d69 746f  np.diff(non_mito
+00017f10: 7469 635f 6469 7370 5f78 2929 0d0a 0d0a  tic_disp_x))....
 00017f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f30: 2061 6c6c 5f64 6973 705f 7a20 3d20 6e70   all_disp_z = np
-00017f40: 2e61 6273 286e 702e 6469 6666 2861 6c6c  .abs(np.diff(all
-00017f50: 5f64 6973 705f 7a29 290d 0a20 2020 2020  _disp_z))..     
-00017f60: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00017f70: 6c6c 5f64 6973 705f 7920 3d20 6e70 2e61  ll_disp_y = np.a
-00017f80: 6273 286e 702e 6469 6666 2861 6c6c 5f64  bs(np.diff(all_d
-00017f90: 6973 705f 7929 290d 0a20 2020 2020 2020  isp_y))..       
-00017fa0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
-00017fb0: 5f64 6973 705f 7820 3d20 6e70 2e61 6273  _disp_x = np.abs
-00017fc0: 286e 702e 6469 6666 2861 6c6c 5f64 6973  (np.diff(all_dis
-00017fd0: 705f 7829 290d 0a0d 0a0d 0a20 2020 2020  p_x))......     
+00017f30: 2020 2020 616c 6c5f 6469 7370 5f7a 203d      all_disp_z =
+00017f40: 206e 702e 6162 7328 6e70 2e64 6966 6628   np.abs(np.diff(
+00017f50: 616c 6c5f 6469 7370 5f7a 2929 0d0a 2020  all_disp_z))..  
+00017f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f70: 2020 616c 6c5f 6469 7370 5f79 203d 206e    all_disp_y = n
+00017f80: 702e 6162 7328 6e70 2e64 6966 6628 616c  p.abs(np.diff(al
+00017f90: 6c5f 6469 7370 5f79 2929 0d0a 2020 2020  l_disp_y))..    
+00017fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017fb0: 616c 6c5f 6469 7370 5f78 203d 206e 702e  all_disp_x = np.
+00017fc0: 6162 7328 6e70 2e64 6966 6628 616c 6c5f  abs(np.diff(all_
+00017fd0: 6469 7370 5f78 2929 0d0a 0d0a 0d0a 2020  disp_x))......  
 00017fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018000: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-00018010: 2020 2020 2020 2020 2073 656c 662e 7469           self.ti
-00018020: 6d65 2e61 7070 656e 6428 6920 2a20 7365  me.append(i * se
-00018030: 6c66 2e74 6361 6c69 6272 6174 696f 6e29  lf.tcalibration)
-00018040: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00018050: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00018060: 6f74 6963 5f63 6c75 7374 6572 5f63 6c61  otic_cluster_cla
-00018070: 7373 2e61 7070 656e 6428 6e70 2e61 7361  ss.append(np.asa
-00018080: 7272 6179 286d 6974 6f74 6963 5f63 6c75  rray(mitotic_clu
-00018090: 7374 6572 5f63 6c61 7373 2929 0d0a 2020  ster_class))..  
-000180a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000180b0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-000180c0: 6963 5f63 6c75 7374 6572 5f63 6c61 7373  ic_cluster_class
-000180d0: 2e61 7070 656e 6428 6e70 2e61 7361 7272  .append(np.asarr
-000180e0: 6179 286e 6f6e 5f6d 6974 6f74 6963 5f63  ay(non_mitotic_c
-000180f0: 6c75 7374 6572 5f63 6c61 7373 2929 0d0a  luster_class))..
-00018100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018110: 2020 2020 7365 6c66 2e61 6c6c 5f63 6c75      self.all_clu
-00018120: 7374 6572 5f63 6c61 7373 2e61 7070 656e  ster_class.appen
-00018130: 6428 6e70 2e61 7361 7272 6179 2861 6c6c  d(np.asarray(all
-00018140: 5f63 6c75 7374 6572 5f63 6c61 7373 2929  _cluster_class))
-00018150: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00018160: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00018170: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f7a  otic_mean_disp_z
-00018180: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00018190: 6d69 746f 7469 635f 6469 7370 5f7a 2929  mitotic_disp_z))
-000181a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000181b0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-000181c0: 6963 5f76 6172 5f64 6973 705f 7a2e 6170  ic_var_disp_z.ap
-000181d0: 7065 6e64 286e 702e 7374 6428 6d69 746f  pend(np.std(mito
-000181e0: 7469 635f 6469 7370 5f7a 2929 0d0a 0d0a  tic_disp_z))....
-000181f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018200: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00018210: 5f6d 6561 6e5f 6469 7370 5f79 2e61 7070  _mean_disp_y.app
-00018220: 656e 6428 6e70 2e6d 6561 6e28 6d69 746f  end(np.mean(mito
-00018230: 7469 635f 6469 7370 5f79 2929 0d0a 2020  tic_disp_y))..  
-00018240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018250: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
-00018260: 6172 5f64 6973 705f 792e 6170 7065 6e64  ar_disp_y.append
-00018270: 286e 702e 7374 6428 6d69 746f 7469 635f  (np.std(mitotic_
-00018280: 6469 7370 5f79 2929 0d0a 0d0a 2020 2020  disp_y))....    
+00018000: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00018010: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018020: 2e74 696d 652e 6170 7065 6e64 2869 202a  .time.append(i *
+00018030: 2073 656c 662e 7463 616c 6962 7261 7469   self.tcalibrati
+00018040: 6f6e 290d 0a0d 0a20 2020 2020 2020 2020  on)....         
+00018050: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018060: 6d69 746f 7469 635f 636c 7573 7465 725f  mitotic_cluster_
+00018070: 636c 6173 732e 6170 7065 6e64 286e 702e  class.append(np.
+00018080: 6173 6172 7261 7928 6d69 746f 7469 635f  asarray(mitotic_
+00018090: 636c 7573 7465 725f 636c 6173 7329 290d  cluster_class)).
+000180a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000180b0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+000180c0: 746f 7469 635f 636c 7573 7465 725f 636c  totic_cluster_cl
+000180d0: 6173 732e 6170 7065 6e64 286e 702e 6173  ass.append(np.as
+000180e0: 6172 7261 7928 6e6f 6e5f 6d69 746f 7469  array(non_mitoti
+000180f0: 635f 636c 7573 7465 725f 636c 6173 7329  c_cluster_class)
+00018100: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018110: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+00018120: 636c 7573 7465 725f 636c 6173 732e 6170  cluster_class.ap
+00018130: 7065 6e64 286e 702e 6173 6172 7261 7928  pend(np.asarray(
+00018140: 616c 6c5f 636c 7573 7465 725f 636c 6173  all_cluster_clas
+00018150: 7329 290d 0a0d 0a20 2020 2020 2020 2020  s))....         
+00018160: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018170: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
+00018180: 705f 7a2e 6170 7065 6e64 286e 702e 6d65  p_z.append(np.me
+00018190: 616e 286d 6974 6f74 6963 5f64 6973 705f  an(mitotic_disp_
+000181a0: 7a29 290d 0a20 2020 2020 2020 2020 2020  z))..           
+000181b0: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+000181c0: 746f 7469 635f 7661 725f 6469 7370 5f7a  totic_var_disp_z
+000181d0: 2e61 7070 656e 6428 6e70 2e73 7464 286d  .append(np.std(m
+000181e0: 6974 6f74 6963 5f64 6973 705f 7a29 290d  itotic_disp_z)).
+000181f0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00018200: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00018210: 7469 635f 6d65 616e 5f64 6973 705f 792e  tic_mean_disp_y.
+00018220: 6170 7065 6e64 286e 702e 6d65 616e 286d  append(np.mean(m
+00018230: 6974 6f74 6963 5f64 6973 705f 7929 290d  itotic_disp_y)).
+00018240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018250: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00018260: 635f 7661 725f 6469 7370 5f79 2e61 7070  c_var_disp_y.app
+00018270: 656e 6428 6e70 2e73 7464 286d 6974 6f74  end(np.std(mitot
+00018280: 6963 5f64 6973 705f 7929 290d 0a0d 0a20  ic_disp_y)).... 
 00018290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000182a0: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
-000182b0: 6e5f 6469 7370 5f78 2e61 7070 656e 6428  n_disp_x.append(
-000182c0: 6e70 2e6d 6561 6e28 6d69 746f 7469 635f  np.mean(mitotic_
-000182d0: 6469 7370 5f78 2929 0d0a 2020 2020 2020  disp_x))..      
-000182e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000182f0: 6c66 2e6d 6974 6f74 6963 5f76 6172 5f64  lf.mitotic_var_d
-00018300: 6973 705f 782e 6170 7065 6e64 286e 702e  isp_x.append(np.
-00018310: 7374 6428 6d69 746f 7469 635f 6469 7370  std(mitotic_disp
-00018320: 5f78 2929 0d0a 0d0a 2020 2020 2020 2020  _x))....        
-00018330: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018340: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 7261  .mitotic_mean_ra
-00018350: 6469 7573 2e61 7070 656e 6428 6e70 2e6d  dius.append(np.m
-00018360: 6561 6e28 6d69 746f 7469 635f 7261 6469  ean(mitotic_radi
-00018370: 7573 2929 0d0a 2020 2020 2020 2020 2020  us))..          
-00018380: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00018390: 6974 6f74 6963 5f76 6172 5f72 6164 6975  itotic_var_radiu
-000183a0: 732e 6170 7065 6e64 286e 702e 7374 6428  s.append(np.std(
-000183b0: 6d69 746f 7469 635f 7261 6469 7573 2929  mitotic_radius))
-000183c0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000183d0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-000183e0: 6f74 6963 5f6d 6561 6e5f 7370 6565 642e  otic_mean_speed.
-000183f0: 6170 7065 6e64 286e 702e 6d65 616e 286d  append(np.mean(m
-00018400: 6974 6f74 6963 5f73 7065 6564 2929 0d0a  itotic_speed))..
-00018410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018420: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00018430: 5f76 6172 5f73 7065 6564 2e61 7070 656e  _var_speed.appen
-00018440: 6428 6e70 2e73 7464 286d 6974 6f74 6963  d(np.std(mitotic
-00018450: 5f73 7065 6564 2929 0d0a 0d0a 2020 2020  _speed))....    
+000182a0: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+000182b0: 6d65 616e 5f64 6973 705f 782e 6170 7065  mean_disp_x.appe
+000182c0: 6e64 286e 702e 6d65 616e 286d 6974 6f74  nd(np.mean(mitot
+000182d0: 6963 5f64 6973 705f 7829 290d 0a20 2020  ic_disp_x))..   
+000182e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000182f0: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
+00018300: 725f 6469 7370 5f78 2e61 7070 656e 6428  r_disp_x.append(
+00018310: 6e70 2e73 7464 286d 6974 6f74 6963 5f64  np.std(mitotic_d
+00018320: 6973 705f 7829 290d 0a0d 0a20 2020 2020  isp_x))....     
+00018330: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018340: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
+00018350: 5f72 6164 6975 732e 6170 7065 6e64 286e  _radius.append(n
+00018360: 702e 6d65 616e 286d 6974 6f74 6963 5f72  p.mean(mitotic_r
+00018370: 6164 6975 7329 290d 0a20 2020 2020 2020  adius))..       
+00018380: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018390: 662e 6d69 746f 7469 635f 7661 725f 7261  f.mitotic_var_ra
+000183a0: 6469 7573 2e61 7070 656e 6428 6e70 2e73  dius.append(np.s
+000183b0: 7464 286d 6974 6f74 6963 5f72 6164 6975  td(mitotic_radiu
+000183c0: 7329 290d 0a0d 0a20 2020 2020 2020 2020  s))....         
+000183d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000183e0: 6d69 746f 7469 635f 6d65 616e 5f73 7065  mitotic_mean_spe
+000183f0: 6564 2e61 7070 656e 6428 6e70 2e6d 6561  ed.append(np.mea
+00018400: 6e28 6d69 746f 7469 635f 7370 6565 6429  n(mitotic_speed)
+00018410: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018420: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00018430: 7469 635f 7661 725f 7370 6565 642e 6170  tic_var_speed.ap
+00018440: 7065 6e64 286e 702e 7374 6428 6d69 746f  pend(np.std(mito
+00018450: 7469 635f 7370 6565 6429 290d 0a0d 0a20  tic_speed)).... 
 00018460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018470: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
-00018480: 6e5f 6163 632e 6170 7065 6e64 286e 702e  n_acc.append(np.
-00018490: 6d65 616e 286d 6974 6f74 6963 5f61 6363  mean(mitotic_acc
-000184a0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000184b0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-000184c0: 6f74 6963 5f76 6172 5f61 6363 2e61 7070  otic_var_acc.app
-000184d0: 656e 6428 6e70 2e73 7464 286d 6974 6f74  end(np.std(mitot
-000184e0: 6963 5f61 6363 2929 0d0a 0d0a 2020 2020  ic_acc))....    
+00018470: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00018480: 6d65 616e 5f61 6363 2e61 7070 656e 6428  mean_acc.append(
+00018490: 6e70 2e6d 6561 6e28 6d69 746f 7469 635f  np.mean(mitotic_
+000184a0: 6163 6329 290d 0a20 2020 2020 2020 2020  acc))..         
+000184b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000184c0: 6d69 746f 7469 635f 7661 725f 6163 632e  mitotic_var_acc.
+000184d0: 6170 7065 6e64 286e 702e 7374 6428 6d69  append(np.std(mi
+000184e0: 746f 7469 635f 6163 6329 290d 0a0d 0a20  totic_acc)).... 
 000184f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018500: 7365 6c66 2e6d 6974 6f74 6963 5f6d 6561  self.mitotic_mea
-00018510: 6e5f 6469 7265 6374 696f 6e61 6c5f 6368  n_directional_ch
-00018520: 616e 6765 2e61 7070 656e 6428 6e70 2e6d  ange.append(np.m
-00018530: 6561 6e28 6d69 746f 7469 635f 6469 7265  ean(mitotic_dire
-00018540: 6374 696f 6e61 6c5f 6368 616e 6765 2929  ctional_change))
-00018550: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018560: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00018570: 6963 5f76 6172 5f64 6972 6563 7469 6f6e  ic_var_direction
-00018580: 616c 5f63 6861 6e67 652e 6170 7065 6e64  al_change.append
-00018590: 286e 702e 7374 6428 6d69 746f 7469 635f  (np.std(mitotic_
-000185a0: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-000185b0: 6765 2929 0d0a 0d0a 2020 2020 2020 2020  ge))....        
-000185c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000185d0: 2e6d 6974 6f74 6963 5f6d 6561 6e5f 6469  .mitotic_mean_di
-000185e0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-000185f0: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00018600: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
-00018610: 5f63 656c 6c5f 6d61 736b 2929 0d0a 2020  _cell_mask))..  
-00018620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018630: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
-00018640: 6172 5f64 6973 7461 6e63 655f 6365 6c6c  ar_distance_cell
-00018650: 5f6d 6173 6b2e 6170 7065 6e64 286e 702e  _mask.append(np.
-00018660: 7374 6428 6d69 746f 7469 635f 6469 7374  std(mitotic_dist
-00018670: 616e 6365 5f63 656c 6c5f 6d61 736b 2929  ance_cell_mask))
-00018680: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00018690: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-000186a0: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
-000186b0: 7370 5f7a 2e61 7070 656e 6428 6e70 2e6d  sp_z.append(np.m
-000186c0: 6561 6e28 6e6f 6e5f 6d69 746f 7469 635f  ean(non_mitotic_
-000186d0: 6469 7370 5f7a 2929 0d0a 2020 2020 2020  disp_z))..      
-000186e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000186f0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
-00018700: 6172 5f64 6973 705f 7a2e 6170 7065 6e64  ar_disp_z.append
-00018710: 286e 702e 7374 6428 6e6f 6e5f 6d69 746f  (np.std(non_mito
-00018720: 7469 635f 6469 7370 5f7a 2929 0d0a 0d0a  tic_disp_z))....
-00018730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018740: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
-00018750: 6f74 6963 5f6d 6561 6e5f 6469 7370 5f79  otic_mean_disp_y
-00018760: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00018770: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
-00018780: 5f79 2929 0d0a 2020 2020 2020 2020 2020  _y))..          
-00018790: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-000187a0: 6f6e 5f6d 6974 6f74 6963 5f76 6172 5f64  on_mitotic_var_d
-000187b0: 6973 705f 792e 6170 7065 6e64 286e 702e  isp_y.append(np.
-000187c0: 7374 6428 6e6f 6e5f 6d69 746f 7469 635f  std(non_mitotic_
-000187d0: 6469 7370 5f79 2929 0d0a 0d0a 2020 2020  disp_y))....    
+00018500: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00018510: 6d65 616e 5f64 6972 6563 7469 6f6e 616c  mean_directional
+00018520: 5f63 6861 6e67 652e 6170 7065 6e64 286e  _change.append(n
+00018530: 702e 6d65 616e 286d 6974 6f74 6963 5f64  p.mean(mitotic_d
+00018540: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+00018550: 6529 290d 0a20 2020 2020 2020 2020 2020  e))..           
+00018560: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+00018570: 746f 7469 635f 7661 725f 6469 7265 6374  totic_var_direct
+00018580: 696f 6e61 6c5f 6368 616e 6765 2e61 7070  ional_change.app
+00018590: 656e 6428 6e70 2e73 7464 286d 6974 6f74  end(np.std(mitot
+000185a0: 6963 5f64 6972 6563 7469 6f6e 616c 5f63  ic_directional_c
+000185b0: 6861 6e67 6529 290d 0a0d 0a20 2020 2020  hange))....     
+000185c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000185d0: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
+000185e0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+000185f0: 6173 6b2e 6170 7065 6e64 286e 702e 6d65  ask.append(np.me
+00018600: 616e 286d 6974 6f74 6963 5f64 6973 7461  an(mitotic_dista
+00018610: 6e63 655f 6365 6c6c 5f6d 6173 6b29 290d  nce_cell_mask)).
+00018620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018630: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00018640: 635f 7661 725f 6469 7374 616e 6365 5f63  c_var_distance_c
+00018650: 656c 6c5f 6d61 736b 2e61 7070 656e 6428  ell_mask.append(
+00018660: 6e70 2e73 7464 286d 6974 6f74 6963 5f64  np.std(mitotic_d
+00018670: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
+00018680: 6b29 290d 0a0d 0a20 2020 2020 2020 2020  k))....         
+00018690: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000186a0: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
+000186b0: 5f64 6973 705f 7a2e 6170 7065 6e64 286e  _disp_z.append(n
+000186c0: 702e 6d65 616e 286e 6f6e 5f6d 6974 6f74  p.mean(non_mitot
+000186d0: 6963 5f64 6973 705f 7a29 290d 0a20 2020  ic_disp_z))..   
+000186e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000186f0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+00018700: 635f 7661 725f 6469 7370 5f7a 2e61 7070  c_var_disp_z.app
+00018710: 656e 6428 6e70 2e73 7464 286e 6f6e 5f6d  end(np.std(non_m
+00018720: 6974 6f74 6963 5f64 6973 705f 7a29 290d  itotic_disp_z)).
+00018730: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00018740: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00018750: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
+00018760: 705f 792e 6170 7065 6e64 286e 702e 6d65  p_y.append(np.me
+00018770: 616e 286e 6f6e 5f6d 6974 6f74 6963 5f64  an(non_mitotic_d
+00018780: 6973 705f 7929 290d 0a20 2020 2020 2020  isp_y))..       
+00018790: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000187a0: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
+000187b0: 725f 6469 7370 5f79 2e61 7070 656e 6428  r_disp_y.append(
+000187c0: 6e70 2e73 7464 286e 6f6e 5f6d 6974 6f74  np.std(non_mitot
+000187d0: 6963 5f64 6973 705f 7929 290d 0a0d 0a20  ic_disp_y)).... 
 000187e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187f0: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00018800: 5f6d 6561 6e5f 6469 7370 5f78 2e61 7070  _mean_disp_x.app
-00018810: 656e 6428 6e70 2e6d 6561 6e28 6e6f 6e5f  end(np.mean(non_
-00018820: 6d69 746f 7469 635f 6469 7370 5f78 2929  mitotic_disp_x))
-00018830: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018840: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00018850: 6974 6f74 6963 5f76 6172 5f64 6973 705f  itotic_var_disp_
-00018860: 782e 6170 7065 6e64 286e 702e 7374 6428  x.append(np.std(
-00018870: 6e6f 6e5f 6d69 746f 7469 635f 6469 7370  non_mitotic_disp
-00018880: 5f78 2929 0d0a 0d0a 2020 2020 2020 2020  _x))....        
-00018890: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000188a0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d 6561  .non_mitotic_mea
-000188b0: 6e5f 7261 6469 7573 2e61 7070 656e 6428  n_radius.append(
-000188c0: 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69 746f  np.mean(non_mito
-000188d0: 7469 635f 7261 6469 7573 2929 0d0a 2020  tic_radius))..  
-000188e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188f0: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00018900: 6963 5f76 6172 5f72 6164 6975 732e 6170  ic_var_radius.ap
-00018910: 7065 6e64 286e 702e 7374 6428 6e6f 6e5f  pend(np.std(non_
-00018920: 6d69 746f 7469 635f 7261 6469 7573 2929  mitotic_radius))
-00018930: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00018940: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00018950: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 7370  _mitotic_mean_sp
-00018960: 6565 642e 6170 7065 6e64 286e 702e 6d65  eed.append(np.me
-00018970: 616e 286e 6f6e 5f6d 6974 6f74 6963 5f73  an(non_mitotic_s
-00018980: 7065 6564 2929 0d0a 2020 2020 2020 2020  peed))..        
-00018990: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000189a0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
-000189b0: 5f73 7065 6564 2e61 7070 656e 6428 6e70  _speed.append(np
-000189c0: 2e73 7464 286e 6f6e 5f6d 6974 6f74 6963  .std(non_mitotic
-000189d0: 5f73 7065 6564 2929 0d0a 0d0a 2020 2020  _speed))....    
+000187f0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+00018800: 7469 635f 6d65 616e 5f64 6973 705f 782e  tic_mean_disp_x.
+00018810: 6170 7065 6e64 286e 702e 6d65 616e 286e  append(np.mean(n
+00018820: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
+00018830: 7829 290d 0a20 2020 2020 2020 2020 2020  x))..           
+00018840: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00018850: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
+00018860: 7370 5f78 2e61 7070 656e 6428 6e70 2e73  sp_x.append(np.s
+00018870: 7464 286e 6f6e 5f6d 6974 6f74 6963 5f64  td(non_mitotic_d
+00018880: 6973 705f 7829 290d 0a0d 0a20 2020 2020  isp_x))....     
+00018890: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000188a0: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+000188b0: 6d65 616e 5f72 6164 6975 732e 6170 7065  mean_radius.appe
+000188c0: 6e64 286e 702e 6d65 616e 286e 6f6e 5f6d  nd(np.mean(non_m
+000188d0: 6974 6f74 6963 5f72 6164 6975 7329 290d  itotic_radius)).
+000188e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000188f0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+00018900: 746f 7469 635f 7661 725f 7261 6469 7573  totic_var_radius
+00018910: 2e61 7070 656e 6428 6e70 2e73 7464 286e  .append(np.std(n
+00018920: 6f6e 5f6d 6974 6f74 6963 5f72 6164 6975  on_mitotic_radiu
+00018930: 7329 290d 0a0d 0a20 2020 2020 2020 2020  s))....         
+00018940: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018950: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
+00018960: 5f73 7065 6564 2e61 7070 656e 6428 6e70  _speed.append(np
+00018970: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
+00018980: 635f 7370 6565 6429 290d 0a20 2020 2020  c_speed))..     
+00018990: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000189a0: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+000189b0: 7661 725f 7370 6565 642e 6170 7065 6e64  var_speed.append
+000189c0: 286e 702e 7374 6428 6e6f 6e5f 6d69 746f  (np.std(non_mito
+000189d0: 7469 635f 7370 6565 6429 290d 0a0d 0a20  tic_speed)).... 
 000189e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000189f0: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00018a00: 5f6d 6561 6e5f 6163 632e 6170 7065 6e64  _mean_acc.append
-00018a10: 286e 702e 6d65 616e 286e 6f6e 5f6d 6974  (np.mean(non_mit
-00018a20: 6f74 6963 5f61 6363 2929 0d0a 2020 2020  otic_acc))..    
+000189f0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+00018a00: 7469 635f 6d65 616e 5f61 6363 2e61 7070  tic_mean_acc.app
+00018a10: 656e 6428 6e70 2e6d 6561 6e28 6e6f 6e5f  end(np.mean(non_
+00018a20: 6d69 746f 7469 635f 6163 6329 290d 0a20  mitotic_acc)).. 
 00018a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a40: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00018a50: 5f76 6172 5f61 6363 2e61 7070 656e 6428  _var_acc.append(
-00018a60: 6e70 2e73 7464 286e 6f6e 5f6d 6974 6f74  np.std(non_mitot
-00018a70: 6963 5f61 6363 2929 0d0a 0d0a 2020 2020  ic_acc))....    
+00018a40: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+00018a50: 7469 635f 7661 725f 6163 632e 6170 7065  tic_var_acc.appe
+00018a60: 6e64 286e 702e 7374 6428 6e6f 6e5f 6d69  nd(np.std(non_mi
+00018a70: 746f 7469 635f 6163 6329 290d 0a0d 0a20  totic_acc)).... 
 00018a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a90: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00018aa0: 5f6d 6561 6e5f 6469 7265 6374 696f 6e61  _mean_directiona
-00018ab0: 6c5f 6368 616e 6765 2e61 7070 656e 6428  l_change.append(
-00018ac0: 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69 746f  np.mean(non_mito
-00018ad0: 7469 635f 6469 7265 6374 696f 6e61 6c5f  tic_directional_
-00018ae0: 6368 616e 6765 2929 0d0a 2020 2020 2020  change))..      
-00018af0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018b00: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
-00018b10: 6172 5f64 6972 6563 7469 6f6e 616c 5f63  ar_directional_c
-00018b20: 6861 6e67 652e 6170 7065 6e64 286e 702e  hange.append(np.
-00018b30: 7374 6428 6e6f 6e5f 6d69 746f 7469 635f  std(non_mitotic_
-00018b40: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-00018b50: 6765 2929 200d 0a0d 0a20 2020 2020 2020  ge)) ....       
-00018b60: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018b70: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-00018b80: 616e 5f64 6973 7461 6e63 655f 6365 6c6c  an_distance_cell
-00018b90: 5f6d 6173 6b2e 6170 7065 6e64 286e 702e  _mask.append(np.
-00018ba0: 6d65 616e 286e 6f6e 5f6d 6974 6f74 6963  mean(non_mitotic
-00018bb0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-00018bc0: 6173 6b29 290d 0a20 2020 2020 2020 2020  ask))..         
-00018bd0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018be0: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-00018bf0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00018c00: 736b 2e61 7070 656e 6428 6e70 2e73 7464  sk.append(np.std
-00018c10: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
-00018c20: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b29  tance_cell_mask)
-00018c30: 290d 0a0d 0a0d 0a20 2020 2020 2020 2020  )......         
-00018c40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018c50: 616c 6c5f 6d65 616e 5f64 6973 705f 7a2e  all_mean_disp_z.
-00018c60: 6170 7065 6e64 286e 702e 6d65 616e 2861  append(np.mean(a
-00018c70: 6c6c 5f64 6973 705f 7a29 290d 0a20 2020  ll_disp_z))..   
+00018a90: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+00018aa0: 7469 635f 6d65 616e 5f64 6972 6563 7469  tic_mean_directi
+00018ab0: 6f6e 616c 5f63 6861 6e67 652e 6170 7065  onal_change.appe
+00018ac0: 6e64 286e 702e 6d65 616e 286e 6f6e 5f6d  nd(np.mean(non_m
+00018ad0: 6974 6f74 6963 5f64 6972 6563 7469 6f6e  itotic_direction
+00018ae0: 616c 5f63 6861 6e67 6529 290d 0a20 2020  al_change))..   
+00018af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b00: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+00018b10: 635f 7661 725f 6469 7265 6374 696f 6e61  c_var_directiona
+00018b20: 6c5f 6368 616e 6765 2e61 7070 656e 6428  l_change.append(
+00018b30: 6e70 2e73 7464 286e 6f6e 5f6d 6974 6f74  np.std(non_mitot
+00018b40: 6963 5f64 6972 6563 7469 6f6e 616c 5f63  ic_directional_c
+00018b50: 6861 6e67 6529 2920 0d0a 0d0a 2020 2020  hange)) ....    
+00018b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b70: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+00018b80: 5f6d 6561 6e5f 6469 7374 616e 6365 5f63  _mean_distance_c
+00018b90: 656c 6c5f 6d61 736b 2e61 7070 656e 6428  ell_mask.append(
+00018ba0: 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69 746f  np.mean(non_mito
+00018bb0: 7469 635f 6469 7374 616e 6365 5f63 656c  tic_distance_cel
+00018bc0: 6c5f 6d61 736b 2929 0d0a 2020 2020 2020  l_mask))..      
+00018bd0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018be0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+00018bf0: 6172 5f64 6973 7461 6e63 655f 6365 6c6c  ar_distance_cell
+00018c00: 5f6d 6173 6b2e 6170 7065 6e64 286e 702e  _mask.append(np.
+00018c10: 7374 6428 6e6f 6e5f 6d69 746f 7469 635f  std(non_mitotic_
+00018c20: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00018c30: 736b 2929 0d0a 0d0a 0d0a 2020 2020 2020  sk))......      
+00018c40: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018c50: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7370  lf.all_mean_disp
+00018c60: 5f7a 2e61 7070 656e 6428 6e70 2e6d 6561  _z.append(np.mea
+00018c70: 6e28 616c 6c5f 6469 7370 5f7a 2929 0d0a  n(all_disp_z))..
 00018c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c90: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
-00018ca0: 7370 5f7a 2e61 7070 656e 6428 6e70 2e73  sp_z.append(np.s
-00018cb0: 7464 2861 6c6c 5f64 6973 705f 7a29 290d  td(all_disp_z)).
-00018cc0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00018cd0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00018ce0: 6d65 616e 5f64 6973 705f 792e 6170 7065  mean_disp_y.appe
-00018cf0: 6e64 286e 702e 6d65 616e 2861 6c6c 5f64  nd(np.mean(all_d
-00018d00: 6973 705f 7929 290d 0a20 2020 2020 2020  isp_y))..       
-00018d10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018d20: 662e 616c 6c5f 7661 725f 6469 7370 5f79  f.all_var_disp_y
-00018d30: 2e61 7070 656e 6428 6e70 2e73 7464 2861  .append(np.std(a
-00018d40: 6c6c 5f64 6973 705f 7929 290d 0a0d 0a20  ll_disp_y)).... 
-00018d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d60: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
-00018d70: 5f64 6973 705f 782e 6170 7065 6e64 286e  _disp_x.append(n
-00018d80: 702e 6d65 616e 2861 6c6c 5f64 6973 705f  p.mean(all_disp_
-00018d90: 7829 290d 0a20 2020 2020 2020 2020 2020  x))..           
-00018da0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-00018db0: 6c5f 7661 725f 6469 7370 5f78 2e61 7070  l_var_disp_x.app
-00018dc0: 656e 6428 6e70 2e73 7464 2861 6c6c 5f64  end(np.std(all_d
-00018dd0: 6973 705f 7829 290d 0a0d 0a20 2020 2020  isp_x))....     
-00018de0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018df0: 656c 662e 616c 6c5f 6d65 616e 5f72 6164  elf.all_mean_rad
-00018e00: 6975 732e 6170 7065 6e64 286e 702e 6d65  ius.append(np.me
-00018e10: 616e 2861 6c6c 5f72 6164 6975 7329 290d  an(all_radius)).
-00018e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018e30: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
-00018e40: 725f 7261 6469 7573 2e61 7070 656e 6428  r_radius.append(
-00018e50: 6e70 2e73 7464 2861 6c6c 5f72 6164 6975  np.std(all_radiu
-00018e60: 7329 290d 0a0d 0a20 2020 2020 2020 2020  s))....         
-00018e70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018e80: 616c 6c5f 6d65 616e 5f73 7065 6564 2e61  all_mean_speed.a
-00018e90: 7070 656e 6428 6e70 2e6d 6561 6e28 616c  ppend(np.mean(al
-00018ea0: 6c5f 7370 6565 6429 290d 0a20 2020 2020  l_speed))..     
-00018eb0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018ec0: 656c 662e 616c 6c5f 7661 725f 7370 6565  elf.all_var_spee
-00018ed0: 642e 6170 7065 6e64 286e 702e 7374 6428  d.append(np.std(
-00018ee0: 616c 6c5f 7370 6565 6429 290d 0a0d 0a20  all_speed)).... 
-00018ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f00: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
-00018f10: 5f61 6363 2e61 7070 656e 6428 6e70 2e6d  _acc.append(np.m
-00018f20: 6561 6e28 616c 6c5f 6163 6329 290d 0a20  ean(all_acc)).. 
-00018f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f40: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
-00018f50: 6163 632e 6170 7065 6e64 286e 702e 7374  acc.append(np.st
-00018f60: 6428 616c 6c5f 6163 6329 290d 0a0d 0a0d  d(all_acc)).....
-00018f70: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-00018f80: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-00018f90: 6d65 616e 5f64 6972 6563 7469 6f6e 616c  mean_directional
-00018fa0: 5f63 6861 6e67 652e 6170 7065 6e64 286e  _change.append(n
-00018fb0: 702e 6d65 616e 2861 6c6c 5f64 6972 6563  p.mean(all_direc
-00018fc0: 7469 6f6e 616c 5f63 6861 6e67 6529 290d  tional_change)).
-00018fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018fe0: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
-00018ff0: 725f 6469 7265 6374 696f 6e61 6c5f 6368  r_directional_ch
-00019000: 616e 6765 2e61 7070 656e 6428 6e70 2e73  ange.append(np.s
-00019010: 7464 2861 6c6c 5f64 6972 6563 7469 6f6e  td(all_direction
-00019020: 616c 5f63 6861 6e67 6529 290d 0a0d 0a20  al_change)).... 
-00019030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019040: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
-00019050: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
-00019060: 6173 6b2e 6170 7065 6e64 286e 702e 6d65  ask.append(np.me
-00019070: 616e 2861 6c6c 5f64 6973 7461 6e63 655f  an(all_distance_
-00019080: 6365 6c6c 5f6d 6173 6b29 290d 0a20 2020  cell_mask))..   
+00018c90: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
+00018ca0: 5f64 6973 705f 7a2e 6170 7065 6e64 286e  _disp_z.append(n
+00018cb0: 702e 7374 6428 616c 6c5f 6469 7370 5f7a  p.std(all_disp_z
+00018cc0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+00018cd0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00018ce0: 6c6c 5f6d 6561 6e5f 6469 7370 5f79 2e61  ll_mean_disp_y.a
+00018cf0: 7070 656e 6428 6e70 2e6d 6561 6e28 616c  ppend(np.mean(al
+00018d00: 6c5f 6469 7370 5f79 2929 0d0a 2020 2020  l_disp_y))..    
+00018d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d20: 7365 6c66 2e61 6c6c 5f76 6172 5f64 6973  self.all_var_dis
+00018d30: 705f 792e 6170 7065 6e64 286e 702e 7374  p_y.append(np.st
+00018d40: 6428 616c 6c5f 6469 7370 5f79 2929 0d0a  d(all_disp_y))..
+00018d50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018d60: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
+00018d70: 6561 6e5f 6469 7370 5f78 2e61 7070 656e  ean_disp_x.appen
+00018d80: 6428 6e70 2e6d 6561 6e28 616c 6c5f 6469  d(np.mean(all_di
+00018d90: 7370 5f78 2929 0d0a 2020 2020 2020 2020  sp_x))..        
+00018da0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018db0: 2e61 6c6c 5f76 6172 5f64 6973 705f 782e  .all_var_disp_x.
+00018dc0: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
+00018dd0: 6c5f 6469 7370 5f78 2929 0d0a 0d0a 2020  l_disp_x))....  
+00018de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018df0: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
+00018e00: 7261 6469 7573 2e61 7070 656e 6428 6e70  radius.append(np
+00018e10: 2e6d 6561 6e28 616c 6c5f 7261 6469 7573  .mean(all_radius
+00018e20: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00018e30: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00018e40: 5f76 6172 5f72 6164 6975 732e 6170 7065  _var_radius.appe
+00018e50: 6e64 286e 702e 7374 6428 616c 6c5f 7261  nd(np.std(all_ra
+00018e60: 6469 7573 2929 0d0a 0d0a 2020 2020 2020  dius))....      
+00018e70: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018e80: 6c66 2e61 6c6c 5f6d 6561 6e5f 7370 6565  lf.all_mean_spee
+00018e90: 642e 6170 7065 6e64 286e 702e 6d65 616e  d.append(np.mean
+00018ea0: 2861 6c6c 5f73 7065 6564 2929 0d0a 2020  (all_speed))..  
+00018eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ec0: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f73    self.all_var_s
+00018ed0: 7065 6564 2e61 7070 656e 6428 6e70 2e73  peed.append(np.s
+00018ee0: 7464 2861 6c6c 5f73 7065 6564 2929 0d0a  td(all_speed))..
+00018ef0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018f00: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
+00018f10: 6561 6e5f 6163 632e 6170 7065 6e64 286e  ean_acc.append(n
+00018f20: 702e 6d65 616e 2861 6c6c 5f61 6363 2929  p.mean(all_acc))
+00018f30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018f40: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
+00018f50: 6172 5f61 6363 2e61 7070 656e 6428 6e70  ar_acc.append(np
+00018f60: 2e73 7464 2861 6c6c 5f61 6363 2929 0d0a  .std(all_acc))..
+00018f70: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
+00018f80: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00018f90: 6c6c 5f6d 6561 6e5f 6469 7265 6374 696f  ll_mean_directio
+00018fa0: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
+00018fb0: 6428 6e70 2e6d 6561 6e28 616c 6c5f 6469  d(np.mean(all_di
+00018fc0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00018fd0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00018fe0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+00018ff0: 5f76 6172 5f64 6972 6563 7469 6f6e 616c  _var_directional
+00019000: 5f63 6861 6e67 652e 6170 7065 6e64 286e  _change.append(n
+00019010: 702e 7374 6428 616c 6c5f 6469 7265 6374  p.std(all_direct
+00019020: 696f 6e61 6c5f 6368 616e 6765 2929 0d0a  ional_change))..
+00019030: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019040: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
+00019050: 6561 6e5f 6469 7374 616e 6365 5f63 656c  ean_distance_cel
+00019060: 6c5f 6d61 736b 2e61 7070 656e 6428 6e70  l_mask.append(np
+00019070: 2e6d 6561 6e28 616c 6c5f 6469 7374 616e  .mean(all_distan
+00019080: 6365 5f63 656c 6c5f 6d61 736b 2929 0d0a  ce_cell_mask))..
 00019090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000190a0: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
-000190b0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-000190c0: 2e61 7070 656e 6428 6e70 2e73 7464 2861  .append(np.std(a
-000190d0: 6c6c 5f64 6973 7461 6e63 655f 6365 6c6c  ll_distance_cell
-000190e0: 5f6d 6173 6b29 290d 0a20 2020 2020 2020  _mask))..       
+000190a0: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
+000190b0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+000190c0: 6173 6b2e 6170 7065 6e64 286e 702e 7374  ask.append(np.st
+000190d0: 6428 616c 6c5f 6469 7374 616e 6365 5f63  d(all_distance_c
+000190e0: 656c 6c5f 6d61 736b 2929 0d0a 2020 2020  ell_mask))..    
 000190f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019100: 2020 2020 200d 0a20 2020 2020 2020 200d       ..        .
-00019110: 0a64 6566 2062 6f75 6e64 6172 795f 706f  .def boundary_po
-00019120: 696e 7473 286d 6173 6b2c 2078 6361 6c69  ints(mask, xcali
-00019130: 6272 6174 696f 6e2c 2079 6361 6c69 6272  bration, ycalibr
-00019140: 6174 696f 6e2c 207a 6361 6c69 6272 6174  ation, zcalibrat
-00019150: 696f 6e29 3a0d 0a0d 0a20 2020 206e 6469  ion):....    ndi
-00019160: 6d20 3d20 6c65 6e28 6d61 736b 2e73 6861  m = len(mask.sha
-00019170: 7065 290d 0a20 2020 2074 696d 6564 5f6d  pe)..    timed_m
-00019180: 6173 6b20 3d20 7b7d 0d0a 2020 2020 6d61  ask = {}..    ma
-00019190: 736b 203d 206d 6173 6b20 3e20 300d 0a20  sk = mask > 0.. 
-000191a0: 2020 206d 6173 6b20 3d20 6d61 736b 2e61     mask = mask.a
-000191b0: 7374 7970 6528 2775 696e 7438 2729 0d0a  stype('uint8')..
-000191c0: 2020 2020 2320 5958 2073 6861 7065 6420      # YX shaped 
-000191d0: 6f62 6a65 6374 0d0a 2020 2020 6966 206e  object..    if n
-000191e0: 6469 6d20 3d3d 2032 3a0d 0a20 2020 2020  dim == 2:..     
-000191f0: 2020 200d 0a20 2020 2020 2020 2062 6f75     ..        bou
-00019200: 6e64 6172 7920 3d20 6669 6e64 5f62 6f75  ndary = find_bou
-00019210: 6e64 6172 6965 7328 6d61 736b 290d 0a20  ndaries(mask).. 
-00019220: 2020 2020 2020 2072 6567 696f 6e63 656e         regioncen
-00019230: 7472 6f69 6420 3d20 2830 2c29 202b 2063  troid = (0,) + c
-00019240: 6f6d 7075 7465 5f63 656e 7472 6f69 6428  ompute_centroid(
-00019250: 626f 756e 6461 7279 2920 0d0a 2020 2020  boundary) ..    
-00019260: 2020 2020 696e 6469 6365 7320 3d20 6e70      indices = np
-00019270: 2e77 6865 7265 2862 6f75 6e64 6172 7920  .where(boundary 
-00019280: 3e20 3029 0d0a 2020 2020 2020 2020 7265  > 0)..        re
-00019290: 616c 5f69 6e64 6963 6573 203d 206e 702e  al_indices = np.
-000192a0: 7472 616e 7370 6f73 6528 6e70 2e61 7361  transpose(np.asa
-000192b0: 7272 6179 2869 6e64 6963 6573 2929 2e63  rray(indices)).c
-000192c0: 6f70 7928 290d 0a0d 0a20 2020 2020 2020  opy()....       
-000192d0: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
-000192e0: 302c 206c 656e 2872 6561 6c5f 696e 6469  0, len(real_indi
-000192f0: 6365 7329 293a 0d0a 0d0a 2020 2020 2020  ces)):....      
-00019300: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
-00019310: 6573 5b6a 5d5b 305d 203d 2072 6561 6c5f  es[j][0] = real_
-00019320: 696e 6469 6365 735b 6a5d 5b30 5d20 2a20  indices[j][0] * 
-00019330: 7963 616c 6962 7261 7469 6f6e 0d0a 2020  ycalibration..  
-00019340: 2020 2020 2020 2020 2020 7265 616c 5f69            real_i
-00019350: 6e64 6963 6573 5b6a 5d5b 315d 203d 2072  ndices[j][1] = r
-00019360: 6561 6c5f 696e 6469 6365 735b 6a5d 5b31  eal_indices[j][1
-00019370: 5d20 2a20 7863 616c 6962 7261 7469 6f6e  ] * xcalibration
-00019380: 0d0a 0d0a 2020 2020 2020 2020 7472 6565  ....        tree
-00019390: 203d 2073 7061 7469 616c 2e63 4b44 5472   = spatial.cKDTr
-000193a0: 6565 2872 6561 6c5f 696e 6469 6365 7329  ee(real_indices)
-000193b0: 0d0a 2020 2020 2020 2020 2320 5468 6973  ..        # This
-000193c0: 206f 626a 6563 7420 636f 6e74 6169 6e73   object contains
-000193d0: 206c 6973 7420 6f66 2061 6c6c 2074 6865   list of all the
-000193e0: 2070 6f69 6e74 7320 666f 7220 616c 6c20   points for all 
-000193f0: 7468 6520 6c61 6265 6c73 2069 6e20 7468  the labels in th
-00019400: 6520 4d61 736b 2069 6d61 6765 2077 6974  e Mask image wit
-00019410: 6820 7468 6520 6c61 6265 6c20 6964 2061  h the label id a
-00019420: 6e64 2076 6f6c 756d 6520 6f66 2065 6163  nd volume of eac
-00019430: 6820 6c61 6265 6c0d 0a20 2020 2020 2020  h label..       
-00019440: 2074 696d 6564 5f6d 6173 6b5b 7374 7228   timed_mask[str(
-00019450: 3029 5d20 3d20 5b74 7265 652c 2069 6e64  0)] = [tree, ind
-00019460: 6963 6573 2c20 7265 6769 6f6e 6365 6e74  ices, regioncent
-00019470: 726f 6964 5d0d 0a0d 0a20 2020 2023 2054  roid]....    # T
-00019480: 5958 2073 6861 7065 6420 6f62 6a65 6374  YX shaped object
-00019490: 0d0a 2020 2020 6966 206e 6469 6d20 3d3d  ..    if ndim ==
-000194a0: 2033 3a0d 0a0d 0a0d 0a20 2020 2020 2020   3:......       
-000194b0: 2066 6f72 2069 2069 6e20 7471 646d 2872   for i in tqdm(r
-000194c0: 616e 6765 2830 2c20 6d61 736b 2e73 6861  ange(0, mask.sha
-000194d0: 7065 5b30 5d29 293a 0d0a 2020 2020 2020  pe[0])):..      
-000194e0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000194f0: 2020 2020 2020 2020 2020 2020 626f 756e              boun
-00019500: 6461 7279 203d 2066 696e 645f 626f 756e  dary = find_boun
-00019510: 6461 7269 6573 286d 6173 6b5b 692c 3a5d  daries(mask[i,:]
-00019520: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00019530: 2020 2072 6567 696f 6e63 656e 7472 6f69     regioncentroi
-00019540: 6420 3d20 2830 2c29 202b 2063 6f6d 7075  d = (0,) + compu
-00019550: 7465 5f63 656e 7472 6f69 6428 626f 756e  te_centroid(boun
-00019560: 6461 7279 2920 0d0a 2020 2020 2020 2020  dary) ..        
-00019570: 2020 2020 2020 2020 696e 6469 6365 7320          indices 
-00019580: 3d20 6e70 2e77 6865 7265 2862 6f75 6e64  = np.where(bound
-00019590: 6172 7920 3e20 3029 0d0a 2020 2020 2020  ary > 0)..      
-000195a0: 2020 2020 2020 2020 2020 7265 616c 5f69            real_i
-000195b0: 6e64 6963 6573 203d 206e 702e 7472 616e  ndices = np.tran
-000195c0: 7370 6f73 6528 6e70 2e61 7361 7272 6179  spose(np.asarray
-000195d0: 2869 6e64 6963 6573 2929 2e63 6f70 7928  (indices)).copy(
-000195e0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-000195f0: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
-00019600: 6e67 6528 302c 206c 656e 2872 6561 6c5f  nge(0, len(real_
-00019610: 696e 6469 6365 7329 293a 0d0a 0d0a 2020  indices)):....  
-00019620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019630: 2020 7265 616c 5f69 6e64 6963 6573 5b6a    real_indices[j
-00019640: 5d5b 305d 203d 2072 6561 6c5f 696e 6469  ][0] = real_indi
-00019650: 6365 735b 6a5d 5b30 5d20 2a20 7963 616c  ces[j][0] * ycal
-00019660: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
-00019670: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00019680: 616c 5f69 6e64 6963 6573 5b6a 5d5b 315d  al_indices[j][1]
-00019690: 203d 2072 6561 6c5f 696e 6469 6365 735b   = real_indices[
-000196a0: 6a5d 5b31 5d20 2a20 7863 616c 6962 7261  j][1] * xcalibra
-000196b0: 7469 6f6e 0d0a 0d0a 2020 2020 2020 2020  tion....        
-000196c0: 2020 2020 2020 2020 7472 6565 203d 2073          tree = s
-000196d0: 7061 7469 616c 2e63 4b44 5472 6565 2872  patial.cKDTree(r
-000196e0: 6561 6c5f 696e 6469 6365 7329 0d0a 0d0a  eal_indices)....
-000196f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019700: 7469 6d65 645f 6d61 736b 5b73 7472 2869  timed_mask[str(i
-00019710: 295d 203d 205b 7472 6565 2c20 696e 6469  )] = [tree, indi
-00019720: 6365 732c 2072 6567 696f 6e63 656e 7472  ces, regioncentr
-00019730: 6f69 645d 0d0a 2020 2020 2020 2020 2020  oid]..          
-00019740: 2020 0d0a 2020 2020 2320 545a 5958 2073    ..    # TZYX s
-00019750: 6861 7065 6420 6f62 6a65 6374 0d0a 2020  haped object..  
-00019760: 2020 6966 206e 6469 6d20 3d3d 2034 3a0d    if ndim == 4:.
-00019770: 0a20 2020 2020 2020 2070 7269 6e74 2827  .        print('
-00019780: 4d61 736b 7320 6d61 6465 2069 6e74 6f20  Masks made into 
-00019790: 6120 3444 2063 796c 696e 6465 722c 2075  a 4D cylinder, u
-000197a0: 7027 290d 0a20 2020 2020 2020 2062 6f75  p')..        bou
-000197b0: 6e64 6172 7920 3d20 6e70 2e7a 6572 6f73  ndary = np.zeros
-000197c0: 280d 0a20 2020 2020 2020 2020 2020 205b  (..            [
-000197d0: 6d61 736b 2e73 6861 7065 5b30 5d2c 206d  mask.shape[0], m
-000197e0: 6173 6b2e 7368 6170 655b 315d 2c20 6d61  ask.shape[1], ma
-000197f0: 736b 2e73 6861 7065 5b32 5d2c 206d 6173  sk.shape[2], mas
-00019800: 6b2e 7368 6170 655b 335d 5d0d 0a20 2020  k.shape[3]]..   
-00019810: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00019820: 666f 7220 6920 696e 2072 616e 6765 2830  for i in range(0
-00019830: 2c20 6d61 736b 2e73 6861 7065 5b30 5d29  , mask.shape[0])
-00019840: 3a0d 0a20 2020 2020 2020 2020 2020 200d  :..            .
-00019850: 0a20 2020 2020 2020 2020 2020 2062 6f75  .            bou
-00019860: 6e64 6172 795b 692c 3a5d 203d 2066 696e  ndary[i,:] = fin
-00019870: 645f 626f 756e 6461 7269 6573 286d 6173  d_boundaries(mas
-00019880: 6b5b 692c 3a5d 290d 0a20 2020 2020 2020  k[i,:])..       
-00019890: 2020 2020 2072 6567 696f 6e63 656e 7472       regioncentr
-000198a0: 6f69 6420 3d20 636f 6d70 7574 655f 6365  oid = compute_ce
-000198b0: 6e74 726f 6964 2862 6f75 6e64 6172 795b  ntroid(boundary[
-000198c0: 692c 3a5d 2920 0d0a 2020 2020 2020 2020  i,:]) ..        
-000198d0: 2020 2020 696e 6469 6365 7320 3d20 6e70      indices = np
-000198e0: 2e77 6865 7265 2862 6f75 6e64 6172 795b  .where(boundary[
-000198f0: 692c 3a5d 203e 2030 290d 0a20 2020 2020  i,:] > 0)..     
-00019900: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
-00019910: 6365 7320 3d20 6e70 2e74 7261 6e73 706f  ces = np.transpo
-00019920: 7365 286e 702e 6173 6172 7261 7928 696e  se(np.asarray(in
-00019930: 6469 6365 7329 292e 636f 7079 2829 0d0a  dices)).copy()..
-00019940: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-00019950: 7220 6a20 696e 2072 616e 6765 2830 2c20  r j in range(0, 
-00019960: 6c65 6e28 7265 616c 5f69 6e64 6963 6573  len(real_indices
-00019970: 2929 3a0d 0a0d 0a20 2020 2020 2020 2020  )):....         
-00019980: 2020 2020 2020 2020 2020 2072 6561 6c5f             real_
-00019990: 696e 6469 6365 735b 6a5d 5b30 5d20 3d20  indices[j][0] = 
-000199a0: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
-000199b0: 305d 202a 207a 6361 6c69 6272 6174 696f  0] * zcalibratio
-000199c0: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-000199d0: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
-000199e0: 6365 735b 6a5d 5b31 5d20 3d20 7265 616c  ces[j][1] = real
-000199f0: 5f69 6e64 6963 6573 5b6a 5d5b 315d 202a  _indices[j][1] *
-00019a00: 2079 6361 6c69 6272 6174 696f 6e0d 0a20   ycalibration.. 
-00019a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a20: 2020 2072 6561 6c5f 696e 6469 6365 735b     real_indices[
-00019a30: 6a5d 5b32 5d20 3d20 7265 616c 5f69 6e64  j][2] = real_ind
-00019a40: 6963 6573 5b6a 5d5b 325d 202a 2078 6361  ices[j][2] * xca
-00019a50: 6c69 6272 6174 696f 6e0d 0a0d 0a20 2020  libration....   
-00019a60: 2020 2020 2020 2020 2074 7265 6520 3d20           tree = 
-00019a70: 7370 6174 6961 6c2e 634b 4454 7265 6528  spatial.cKDTree(
-00019a80: 7265 616c 5f69 6e64 6963 6573 290d 0a20  real_indices).. 
-00019a90: 2020 2020 2020 2020 2020 2074 696d 6564             timed
-00019aa0: 5f6d 6173 6b5b 7374 7228 6929 5d20 3d20  _mask[str(i)] = 
-00019ab0: 5b74 7265 652c 2069 6e64 6963 6573 2c20  [tree, indices, 
-00019ac0: 7265 6769 6f6e 6365 6e74 726f 6964 5d0d  regioncentroid].
-00019ad0: 0a20 2020 2070 7269 6e74 2827 436f 6d70  .    print('Comp
-00019ae0: 7574 6564 2074 6865 2062 6f75 6e64 6172  uted the boundar
-00019af0: 7920 706f 696e 7473 2729 0d0a 0d0a 2020  y points')....  
-00019b00: 2020 7265 7475 726e 2074 696d 6564 5f6d    return timed_m
-00019b10: 6173 6b2c 2062 6f75 6e64 6172 7920 2020  ask, boundary   
-00019b20: 2020 2020 200d 0a0d 0a64 6566 2063 6f6d       ....def com
-00019b30: 7075 7465 5f63 656e 7472 6f69 6428 6269  pute_centroid(bi
-00019b40: 6e61 7279 5f69 6d61 6765 293a 0d0a 2020  nary_image):..  
-00019b50: 2020 2320 456e 7375 7265 2062 696e 6172    # Ensure binar
-00019b60: 7920 696d 6167 6520 6973 2061 204e 756d  y image is a Num
-00019b70: 5079 2061 7272 6179 0d0a 2020 2020 6269  Py array..    bi
-00019b80: 6e61 7279 5f69 6d61 6765 203d 206e 702e  nary_image = np.
-00019b90: 6172 7261 7928 6269 6e61 7279 5f69 6d61  array(binary_ima
-00019ba0: 6765 290d 0a0d 0a20 2020 2077 6869 7465  ge)....    white
-00019bb0: 5f70 6978 656c 7320 3d20 6e70 2e77 6865  _pixels = np.whe
-00019bc0: 7265 2862 696e 6172 795f 696d 6167 6520  re(binary_image 
-00019bd0: 3d3d 2031 290d 0a20 2020 206e 756d 5f70  == 1)..    num_p
-00019be0: 6978 656c 7320 3d20 6c65 6e28 7768 6974  ixels = len(whit
-00019bf0: 655f 7069 7865 6c73 5b30 5d29 0d0a 0d0a  e_pixels[0])....
-00019c00: 2020 2020 2320 436f 6d70 7574 6520 7468      # Compute th
-00019c10: 6520 6365 6e74 726f 6964 206f 6620 7468  e centroid of th
-00019c20: 6520 7768 6974 6520 7069 7865 6c73 2069  e white pixels i
-00019c30: 6e20 7468 6520 626f 756e 6461 7279 2069  n the boundary i
-00019c40: 6d61 6765 0d0a 2020 2020 6365 6e74 726f  mage..    centro
-00019c50: 6964 203d 206e 702e 7a65 726f 7328 6269  id = np.zeros(bi
-00019c60: 6e61 7279 5f69 6d61 6765 2e6e 6469 6d29  nary_image.ndim)
-00019c70: 0d0a 2020 2020 666f 7220 6469 6d20 696e  ..    for dim in
-00019c80: 2072 616e 6765 2862 696e 6172 795f 696d   range(binary_im
-00019c90: 6167 652e 6e64 696d 293a 0d0a 2020 2020  age.ndim):..    
-00019ca0: 2020 2020 6365 6e74 726f 6964 5b64 696d      centroid[dim
-00019cb0: 5d20 3d20 7768 6974 655f 7069 7865 6c73  ] = white_pixels
-00019cc0: 5b64 696d 5d2e 7375 6d28 2920 2f20 6e75  [dim].sum() / nu
-00019cd0: 6d5f 7069 7865 6c73 0d0a 0d0a 2020 2020  m_pixels....    
-00019ce0: 7265 7475 726e 2063 656e 7472 6f69 640d  return centroid.
-00019cf0: 0a0d 0a0d 0a0d 0a20 0d0a 0d0a 6465 6620  ....... ....def 
-00019d00: 6765 745f 6373 765f 6461 7461 2863 7376  get_csv_data(csv
-00019d10: 293a 0d0a 0d0a 2020 2020 2020 2020 6461  ):....        da
-00019d20: 7461 7365 7420 3d20 7064 2e72 6561 645f  taset = pd.read_
-00019d30: 6373 7628 0d0a 2020 2020 2020 2020 2020  csv(..          
-00019d40: 2020 6373 762c 2064 656c 696d 6974 6572    csv, delimiter
-00019d50: 3d22 2c22 2c20 656e 636f 6469 6e67 3d22  =",", encoding="
-00019d60: 756e 6963 6f64 655f 6573 6361 7065 222c  unicode_escape",
-00019d70: 206c 6f77 5f6d 656d 6f72 793d 4661 6c73   low_memory=Fals
-00019d80: 650d 0a20 2020 2020 2020 2029 5b33 3a5d  e..        )[3:]
-00019d90: 0d0a 2020 2020 2020 2020 6461 7461 7365  ..        datase
-00019da0: 745f 696e 6465 7820 3d20 6461 7461 7365  t_index = datase
-00019db0: 742e 696e 6465 780d 0a20 2020 2020 2020  t.index..       
-00019dc0: 2072 6574 7572 6e20 6461 7461 7365 742c   return dataset,
-00019dd0: 2064 6174 6173 6574 5f69 6e64 6578 0d0a   dataset_index..
-00019de0: 2020 2020 0d0a 6465 6620 6765 745f 7370      ..def get_sp
-00019df0: 6f74 5f64 6174 6173 6574 2873 706f 745f  ot_dataset(spot_
-00019e00: 6461 7461 7365 742c 2074 7261 636b 5f61  dataset, track_a
-00019e10: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
-00019e20: 732c 2078 6361 6c69 6272 6174 696f 6e2c  s, xcalibration,
-00019e30: 2079 6361 6c69 6272 6174 696f 6e2c 207a   ycalibration, z
-00019e40: 6361 6c69 6272 6174 696f 6e2c 2041 7474  calibration, Att
-00019e50: 7269 6275 7465 426f 786e 616d 652c 2064  ributeBoxname, d
-00019e60: 6574 6563 7469 6f6e 6368 616e 6e65 6c29  etectionchannel)
-00019e70: 3a0d 0a20 2020 2020 2020 2041 6c6c 5661  :..        AllVa
-00019e80: 6c75 6573 203d 207b 7d0d 0a20 2020 2020  lues = {}..     
-00019e90: 2020 2070 6f73 6978 203d 2074 7261 636b     posix = track
-00019ea0: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-00019eb0: 6579 735b 2270 6f73 6978 225d 0d0a 2020  eys["posix"]..  
-00019ec0: 2020 2020 2020 706f 7369 7920 3d20 7472        posiy = tr
-00019ed0: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
-00019ee0: 745f 6b65 7973 5b22 706f 7369 7922 5d0d  t_keys["posiy"].
-00019ef0: 0a20 2020 2020 2020 2070 6f73 697a 203d  .        posiz =
-00019f00: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
-00019f10: 7370 6f74 5f6b 6579 735b 2270 6f73 697a  spot_keys["posiz
-00019f20: 225d 0d0a 2020 2020 2020 2020 6672 616d  "]..        fram
-00019f30: 6520 3d20 7472 6163 6b5f 616e 616c 7973  e = track_analys
-00019f40: 6973 5f73 706f 745f 6b65 7973 5b22 6672  is_spot_keys["fr
-00019f50: 616d 6522 5d0d 0a20 2020 2020 2020 200d  ame"]..        .
-00019f60: 0a20 2020 2020 2020 204c 6f63 6174 696f  .        Locatio
-00019f70: 6e58 203d 2028 0d0a 2020 2020 2020 2020  nX = (..        
-00019f80: 2020 2020 7370 6f74 5f64 6174 6173 6574      spot_dataset
-00019f90: 5b70 6f73 6978 5d2e 6173 7479 7065 2822  [posix].astype("
-00019fa0: 666c 6f61 7422 2920 2f20 7863 616c 6962  float") / xcalib
-00019fb0: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
-00019fc0: 292e 6173 7479 7065 2822 696e 7422 290d  ).astype("int").
-00019fd0: 0a20 2020 2020 2020 204c 6f63 6174 696f  .        Locatio
-00019fe0: 6e59 203d 2028 0d0a 2020 2020 2020 2020  nY = (..        
-00019ff0: 2020 2020 7370 6f74 5f64 6174 6173 6574      spot_dataset
-0001a000: 5b70 6f73 6979 5d2e 6173 7479 7065 2822  [posiy].astype("
-0001a010: 666c 6f61 7422 2920 2f20 7963 616c 6962  float") / ycalib
-0001a020: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
-0001a030: 292e 6173 7479 7065 2822 696e 7422 290d  ).astype("int").
-0001a040: 0a20 2020 2020 2020 204c 6f63 6174 696f  .        Locatio
-0001a050: 6e5a 203d 2028 0d0a 2020 2020 2020 2020  nZ = (..        
-0001a060: 2020 2020 7370 6f74 5f64 6174 6173 6574      spot_dataset
-0001a070: 5b70 6f73 697a 5d2e 6173 7479 7065 2822  [posiz].astype("
-0001a080: 666c 6f61 7422 2920 2f20 7a63 616c 6962  float") / zcalib
-0001a090: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
-0001a0a0: 292e 6173 7479 7065 2822 696e 7422 290d  ).astype("int").
-0001a0b0: 0a20 2020 2020 2020 204c 6f63 6174 696f  .        Locatio
-0001a0c0: 6e54 203d 2028 7370 6f74 5f64 6174 6173  nT = (spot_datas
-0001a0d0: 6574 5b66 7261 6d65 5d2e 6173 7479 7065  et[frame].astype
-0001a0e0: 2822 666c 6f61 7422 2929 2e61 7374 7970  ("float")).astyp
-0001a0f0: 6528 2269 6e74 2229 0d0a 2020 2020 2020  e("int")..      
-0001a100: 2020 0d0a 0d0a 2020 2020 2020 2020 6967    ....        ig
-0001a110: 6e6f 7265 5f76 616c 7565 7320 3d20 5b74  nore_values = [t
-0001a120: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
-0001a130: 6f74 5f6b 6579 735b 226d 6561 6e5f 696e  ot_keys["mean_in
-0001a140: 7465 6e73 6974 7922 5d2c 7472 6163 6b5f  tensity"],track_
-0001a150: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
-0001a160: 7973 5b22 746f 7461 6c5f 696e 7465 6e73  ys["total_intens
-0001a170: 6974 7922 5d5d 200d 0a20 2020 2020 2020  ity"]] ..       
-0001a180: 2066 6f72 2028 6b2c 7629 2069 6e20 7472   for (k,v) in tr
-0001a190: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
-0001a1a0: 745f 6b65 7973 2e69 7465 6d73 2829 3a0d  t_keys.items():.
-0001a1b0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001a1c0: 2020 2069 6620 6465 7465 6374 696f 6e63     if detectionc
-0001a1d0: 6861 6e6e 656c 203d 3d20 313a 0d0a 2020  hannel == 1:..  
-0001a1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a1f0: 2020 2069 6620 6b20 3d3d 2022 6d65 616e     if k == "mean
-0001a200: 5f69 6e74 656e 7369 7479 5f63 6832 223a  _intensity_ch2":
-0001a210: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a220: 2020 2020 2020 2020 2020 2020 2076 616c               val
-0001a230: 7565 203d 2074 7261 636b 5f61 6e61 6c79  ue = track_analy
-0001a240: 7369 735f 7370 6f74 5f6b 6579 735b 226d  sis_spot_keys["m
-0001a250: 6561 6e5f 696e 7465 6e73 6974 7922 5d0d  ean_intensity"].
-0001a260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a270: 2020 2020 2020 2020 2020 2020 416c 6c56              AllV
-0001a280: 616c 7565 735b 7661 6c75 655d 203d 2073  alues[value] = s
-0001a290: 706f 745f 6461 7461 7365 745b 765d 2e61  pot_dataset[v].a
-0001a2a0: 7374 7970 6528 2266 6c6f 6174 2229 0d0a  stype("float")..
-0001a2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a2c0: 2020 2020 2069 6620 6b20 3d3d 2022 746f       if k == "to
-0001a2d0: 7461 6c5f 696e 7465 6e73 6974 795f 6368  tal_intensity_ch
-0001a2e0: 3222 3a0d 0a20 2020 2020 2020 2020 2020  2":..           
+00019100: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00019110: 2020 0d0a 6465 6620 626f 756e 6461 7279    ..def boundary
+00019120: 5f70 6f69 6e74 7328 6d61 736b 2c20 7863  _points(mask, xc
+00019130: 616c 6962 7261 7469 6f6e 2c20 7963 616c  alibration, ycal
+00019140: 6962 7261 7469 6f6e 2c20 7a63 616c 6962  ibration, zcalib
+00019150: 7261 7469 6f6e 293a 0d0a 0d0a 2020 2020  ration):....    
+00019160: 6e64 696d 203d 206c 656e 286d 6173 6b2e  ndim = len(mask.
+00019170: 7368 6170 6529 0d0a 2020 2020 7469 6d65  shape)..    time
+00019180: 645f 6d61 736b 203d 207b 7d0d 0a20 2020  d_mask = {}..   
+00019190: 206d 6173 6b20 3d20 6d61 736b 203e 2030   mask = mask > 0
+000191a0: 0d0a 2020 2020 6d61 736b 203d 206d 6173  ..    mask = mas
+000191b0: 6b2e 6173 7479 7065 2827 7569 6e74 3827  k.astype('uint8'
+000191c0: 290d 0a20 2020 2023 2059 5820 7368 6170  )..    # YX shap
+000191d0: 6564 206f 626a 6563 740d 0a20 2020 2069  ed object..    i
+000191e0: 6620 6e64 696d 203d 3d20 323a 0d0a 2020  f ndim == 2:..  
+000191f0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00019200: 626f 756e 6461 7279 203d 2066 696e 645f  boundary = find_
+00019210: 626f 756e 6461 7269 6573 286d 6173 6b29  boundaries(mask)
+00019220: 0d0a 2020 2020 2020 2020 7265 6769 6f6e  ..        region
+00019230: 6365 6e74 726f 6964 203d 2028 302c 2920  centroid = (0,) 
+00019240: 2b20 636f 6d70 7574 655f 6365 6e74 726f  + compute_centro
+00019250: 6964 2862 6f75 6e64 6172 7929 200d 0a20  id(boundary) .. 
+00019260: 2020 2020 2020 2069 6e64 6963 6573 203d         indices =
+00019270: 206e 702e 7768 6572 6528 626f 756e 6461   np.where(bounda
+00019280: 7279 203e 2030 290d 0a20 2020 2020 2020  ry > 0)..       
+00019290: 2072 6561 6c5f 696e 6469 6365 7320 3d20   real_indices = 
+000192a0: 6e70 2e74 7261 6e73 706f 7365 286e 702e  np.transpose(np.
+000192b0: 6173 6172 7261 7928 696e 6469 6365 7329  asarray(indices)
+000192c0: 292e 636f 7079 2829 0d0a 0d0a 2020 2020  ).copy()....    
+000192d0: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
+000192e0: 6765 2830 2c20 6c65 6e28 7265 616c 5f69  ge(0, len(real_i
+000192f0: 6e64 6963 6573 2929 3a0d 0a0d 0a20 2020  ndices)):....   
+00019300: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
+00019310: 6469 6365 735b 6a5d 5b30 5d20 3d20 7265  dices[j][0] = re
+00019320: 616c 5f69 6e64 6963 6573 5b6a 5d5b 305d  al_indices[j][0]
+00019330: 202a 2079 6361 6c69 6272 6174 696f 6e0d   * ycalibration.
+00019340: 0a20 2020 2020 2020 2020 2020 2072 6561  .            rea
+00019350: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
+00019360: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
+00019370: 5d5b 315d 202a 2078 6361 6c69 6272 6174  ][1] * xcalibrat
+00019380: 696f 6e0d 0a0d 0a20 2020 2020 2020 2074  ion....        t
+00019390: 7265 6520 3d20 7370 6174 6961 6c2e 634b  ree = spatial.cK
+000193a0: 4454 7265 6528 7265 616c 5f69 6e64 6963  DTree(real_indic
+000193b0: 6573 290d 0a20 2020 2020 2020 2023 2054  es)..        # T
+000193c0: 6869 7320 6f62 6a65 6374 2063 6f6e 7461  his object conta
+000193d0: 696e 7320 6c69 7374 206f 6620 616c 6c20  ins list of all 
+000193e0: 7468 6520 706f 696e 7473 2066 6f72 2061  the points for a
+000193f0: 6c6c 2074 6865 206c 6162 656c 7320 696e  ll the labels in
+00019400: 2074 6865 204d 6173 6b20 696d 6167 6520   the Mask image 
+00019410: 7769 7468 2074 6865 206c 6162 656c 2069  with the label i
+00019420: 6420 616e 6420 766f 6c75 6d65 206f 6620  d and volume of 
+00019430: 6561 6368 206c 6162 656c 0d0a 2020 2020  each label..    
+00019440: 2020 2020 7469 6d65 645f 6d61 736b 5b73      timed_mask[s
+00019450: 7472 2830 295d 203d 205b 7472 6565 2c20  tr(0)] = [tree, 
+00019460: 696e 6469 6365 732c 2072 6567 696f 6e63  indices, regionc
+00019470: 656e 7472 6f69 645d 0d0a 0d0a 2020 2020  entroid]....    
+00019480: 2320 5459 5820 7368 6170 6564 206f 626a  # TYX shaped obj
+00019490: 6563 740d 0a20 2020 2069 6620 6e64 696d  ect..    if ndim
+000194a0: 203d 3d20 333a 0d0a 0d0a 0d0a 2020 2020   == 3:......    
+000194b0: 2020 2020 666f 7220 6920 696e 2074 7164      for i in tqd
+000194c0: 6d28 7261 6e67 6528 302c 206d 6173 6b2e  m(range(0, mask.
+000194d0: 7368 6170 655b 305d 2929 3a0d 0a20 2020  shape[0])):..   
+000194e0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+000194f0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00019500: 6f75 6e64 6172 7920 3d20 6669 6e64 5f62  oundary = find_b
+00019510: 6f75 6e64 6172 6965 7328 6d61 736b 5b69  oundaries(mask[i
+00019520: 2c3a 5d29 0d0a 2020 2020 2020 2020 2020  ,:])..          
+00019530: 2020 2020 2020 7265 6769 6f6e 6365 6e74        regioncent
+00019540: 726f 6964 203d 2028 302c 2920 2b20 636f  roid = (0,) + co
+00019550: 6d70 7574 655f 6365 6e74 726f 6964 2862  mpute_centroid(b
+00019560: 6f75 6e64 6172 7929 200d 0a20 2020 2020  oundary) ..     
+00019570: 2020 2020 2020 2020 2020 2069 6e64 6963             indic
+00019580: 6573 203d 206e 702e 7768 6572 6528 626f  es = np.where(bo
+00019590: 756e 6461 7279 203e 2030 290d 0a20 2020  undary > 0)..   
+000195a0: 2020 2020 2020 2020 2020 2020 2072 6561               rea
+000195b0: 6c5f 696e 6469 6365 7320 3d20 6e70 2e74  l_indices = np.t
+000195c0: 7261 6e73 706f 7365 286e 702e 6173 6172  ranspose(np.asar
+000195d0: 7261 7928 696e 6469 6365 7329 292e 636f  ray(indices)).co
+000195e0: 7079 2829 0d0a 0d0a 2020 2020 2020 2020  py()....        
+000195f0: 2020 2020 2020 2020 666f 7220 6a20 696e          for j in
+00019600: 2072 616e 6765 2830 2c20 6c65 6e28 7265   range(0, len(re
+00019610: 616c 5f69 6e64 6963 6573 2929 3a0d 0a0d  al_indices)):...
+00019620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019630: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
+00019640: 735b 6a5d 5b30 5d20 3d20 7265 616c 5f69  s[j][0] = real_i
+00019650: 6e64 6963 6573 5b6a 5d5b 305d 202a 2079  ndices[j][0] * y
+00019660: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
+00019670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019680: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
+00019690: 5b31 5d20 3d20 7265 616c 5f69 6e64 6963  [1] = real_indic
+000196a0: 6573 5b6a 5d5b 315d 202a 2078 6361 6c69  es[j][1] * xcali
+000196b0: 6272 6174 696f 6e0d 0a0d 0a20 2020 2020  bration....     
+000196c0: 2020 2020 2020 2020 2020 2074 7265 6520             tree 
+000196d0: 3d20 7370 6174 6961 6c2e 634b 4454 7265  = spatial.cKDTre
+000196e0: 6528 7265 616c 5f69 6e64 6963 6573 290d  e(real_indices).
+000196f0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00019700: 2020 2074 696d 6564 5f6d 6173 6b5b 7374     timed_mask[st
+00019710: 7228 6929 5d20 3d20 5b74 7265 652c 2069  r(i)] = [tree, i
+00019720: 6e64 6963 6573 2c20 7265 6769 6f6e 6365  ndices, regionce
+00019730: 6e74 726f 6964 5d0d 0a20 2020 2020 2020  ntroid]..       
+00019740: 2020 2020 200d 0a20 2020 2023 2054 5a59       ..    # TZY
+00019750: 5820 7368 6170 6564 206f 626a 6563 740d  X shaped object.
+00019760: 0a20 2020 2069 6620 6e64 696d 203d 3d20  .    if ndim == 
+00019770: 343a 0d0a 2020 2020 2020 2020 7072 696e  4:..        prin
+00019780: 7428 274d 6173 6b73 206d 6164 6520 696e  t('Masks made in
+00019790: 746f 2061 2034 4420 6379 6c69 6e64 6572  to a 4D cylinder
+000197a0: 2c20 7570 2729 0d0a 2020 2020 2020 2020  , up')..        
+000197b0: 626f 756e 6461 7279 203d 206e 702e 7a65  boundary = np.ze
+000197c0: 726f 7328 0d0a 2020 2020 2020 2020 2020  ros(..          
+000197d0: 2020 5b6d 6173 6b2e 7368 6170 655b 305d    [mask.shape[0]
+000197e0: 2c20 6d61 736b 2e73 6861 7065 5b31 5d2c  , mask.shape[1],
+000197f0: 206d 6173 6b2e 7368 6170 655b 325d 2c20   mask.shape[2], 
+00019800: 6d61 736b 2e73 6861 7065 5b33 5d5d 0d0a  mask.shape[3]]..
+00019810: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+00019820: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+00019830: 6528 302c 206d 6173 6b2e 7368 6170 655b  e(0, mask.shape[
+00019840: 305d 293a 0d0a 2020 2020 2020 2020 2020  0]):..          
+00019850: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00019860: 626f 756e 6461 7279 5b69 2c3a 5d20 3d20  boundary[i,:] = 
+00019870: 6669 6e64 5f62 6f75 6e64 6172 6965 7328  find_boundaries(
+00019880: 6d61 736b 5b69 2c3a 5d29 0d0a 2020 2020  mask[i,:])..    
+00019890: 2020 2020 2020 2020 7265 6769 6f6e 6365          regionce
+000198a0: 6e74 726f 6964 203d 2063 6f6d 7075 7465  ntroid = compute
+000198b0: 5f63 656e 7472 6f69 6428 626f 756e 6461  _centroid(bounda
+000198c0: 7279 5b69 2c3a 5d29 200d 0a20 2020 2020  ry[i,:]) ..     
+000198d0: 2020 2020 2020 2069 6e64 6963 6573 203d         indices =
+000198e0: 206e 702e 7768 6572 6528 626f 756e 6461   np.where(bounda
+000198f0: 7279 5b69 2c3a 5d20 3e20 3029 0d0a 2020  ry[i,:] > 0)..  
+00019900: 2020 2020 2020 2020 2020 7265 616c 5f69            real_i
+00019910: 6e64 6963 6573 203d 206e 702e 7472 616e  ndices = np.tran
+00019920: 7370 6f73 6528 6e70 2e61 7361 7272 6179  spose(np.asarray
+00019930: 2869 6e64 6963 6573 2929 2e63 6f70 7928  (indices)).copy(
+00019940: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00019950: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
+00019960: 302c 206c 656e 2872 6561 6c5f 696e 6469  0, len(real_indi
+00019970: 6365 7329 293a 0d0a 0d0a 2020 2020 2020  ces)):....      
+00019980: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00019990: 616c 5f69 6e64 6963 6573 5b6a 5d5b 305d  al_indices[j][0]
+000199a0: 203d 2072 6561 6c5f 696e 6469 6365 735b   = real_indices[
+000199b0: 6a5d 5b30 5d20 2a20 7a63 616c 6962 7261  j][0] * zcalibra
+000199c0: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
+000199d0: 2020 2020 2020 2020 2020 7265 616c 5f69            real_i
+000199e0: 6e64 6963 6573 5b6a 5d5b 315d 203d 2072  ndices[j][1] = r
+000199f0: 6561 6c5f 696e 6469 6365 735b 6a5d 5b31  eal_indices[j][1
+00019a00: 5d20 2a20 7963 616c 6962 7261 7469 6f6e  ] * ycalibration
+00019a10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019a20: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
+00019a30: 6573 5b6a 5d5b 325d 203d 2072 6561 6c5f  es[j][2] = real_
+00019a40: 696e 6469 6365 735b 6a5d 5b32 5d20 2a20  indices[j][2] * 
+00019a50: 7863 616c 6962 7261 7469 6f6e 0d0a 0d0a  xcalibration....
+00019a60: 2020 2020 2020 2020 2020 2020 7472 6565              tree
+00019a70: 203d 2073 7061 7469 616c 2e63 4b44 5472   = spatial.cKDTr
+00019a80: 6565 2872 6561 6c5f 696e 6469 6365 7329  ee(real_indices)
+00019a90: 0d0a 2020 2020 2020 2020 2020 2020 7469  ..            ti
+00019aa0: 6d65 645f 6d61 736b 5b73 7472 2869 295d  med_mask[str(i)]
+00019ab0: 203d 205b 7472 6565 2c20 696e 6469 6365   = [tree, indice
+00019ac0: 732c 2072 6567 696f 6e63 656e 7472 6f69  s, regioncentroi
+00019ad0: 645d 0d0a 2020 2020 7072 696e 7428 2743  d]..    print('C
+00019ae0: 6f6d 7075 7465 6420 7468 6520 626f 756e  omputed the boun
+00019af0: 6461 7279 2070 6f69 6e74 7327 290d 0a0d  dary points')...
+00019b00: 0a20 2020 2072 6574 7572 6e20 7469 6d65  .    return time
+00019b10: 645f 6d61 736b 2c20 626f 756e 6461 7279  d_mask, boundary
+00019b20: 2020 2020 2020 2020 0d0a 0d0a 6465 6620          ....def 
+00019b30: 636f 6d70 7574 655f 6365 6e74 726f 6964  compute_centroid
+00019b40: 2862 696e 6172 795f 696d 6167 6529 3a0d  (binary_image):.
+00019b50: 0a20 2020 2023 2045 6e73 7572 6520 6269  .    # Ensure bi
+00019b60: 6e61 7279 2069 6d61 6765 2069 7320 6120  nary image is a 
+00019b70: 4e75 6d50 7920 6172 7261 790d 0a20 2020  NumPy array..   
+00019b80: 2062 696e 6172 795f 696d 6167 6520 3d20   binary_image = 
+00019b90: 6e70 2e61 7272 6179 2862 696e 6172 795f  np.array(binary_
+00019ba0: 696d 6167 6529 0d0a 0d0a 2020 2020 7768  image)....    wh
+00019bb0: 6974 655f 7069 7865 6c73 203d 206e 702e  ite_pixels = np.
+00019bc0: 7768 6572 6528 6269 6e61 7279 5f69 6d61  where(binary_ima
+00019bd0: 6765 203d 3d20 3129 0d0a 2020 2020 6e75  ge == 1)..    nu
+00019be0: 6d5f 7069 7865 6c73 203d 206c 656e 2877  m_pixels = len(w
+00019bf0: 6869 7465 5f70 6978 656c 735b 305d 290d  hite_pixels[0]).
+00019c00: 0a0d 0a20 2020 2023 2043 6f6d 7075 7465  ...    # Compute
+00019c10: 2074 6865 2063 656e 7472 6f69 6420 6f66   the centroid of
+00019c20: 2074 6865 2077 6869 7465 2070 6978 656c   the white pixel
+00019c30: 7320 696e 2074 6865 2062 6f75 6e64 6172  s in the boundar
+00019c40: 7920 696d 6167 650d 0a20 2020 2063 656e  y image..    cen
+00019c50: 7472 6f69 6420 3d20 6e70 2e7a 6572 6f73  troid = np.zeros
+00019c60: 2862 696e 6172 795f 696d 6167 652e 6e64  (binary_image.nd
+00019c70: 696d 290d 0a20 2020 2066 6f72 2064 696d  im)..    for dim
+00019c80: 2069 6e20 7261 6e67 6528 6269 6e61 7279   in range(binary
+00019c90: 5f69 6d61 6765 2e6e 6469 6d29 3a0d 0a20  _image.ndim):.. 
+00019ca0: 2020 2020 2020 2063 656e 7472 6f69 645b         centroid[
+00019cb0: 6469 6d5d 203d 2077 6869 7465 5f70 6978  dim] = white_pix
+00019cc0: 656c 735b 6469 6d5d 2e73 756d 2829 202f  els[dim].sum() /
+00019cd0: 206e 756d 5f70 6978 656c 730d 0a0d 0a20   num_pixels.... 
+00019ce0: 2020 2072 6574 7572 6e20 6365 6e74 726f     return centro
+00019cf0: 6964 0d0a 0d0a 0d0a 0d0a 200d 0a0d 0a64  id........ ....d
+00019d00: 6566 2067 6574 5f63 7376 5f64 6174 6128  ef get_csv_data(
+00019d10: 6373 7629 3a0d 0a0d 0a20 2020 2020 2020  csv):....       
+00019d20: 2064 6174 6173 6574 203d 2070 642e 7265   dataset = pd.re
+00019d30: 6164 5f63 7376 280d 0a20 2020 2020 2020  ad_csv(..       
+00019d40: 2020 2020 2063 7376 2c20 6465 6c69 6d69       csv, delimi
+00019d50: 7465 723d 222c 222c 2065 6e63 6f64 696e  ter=",", encodin
+00019d60: 673d 2275 6e69 636f 6465 5f65 7363 6170  g="unicode_escap
+00019d70: 6522 2c20 6c6f 775f 6d65 6d6f 7279 3d46  e", low_memory=F
+00019d80: 616c 7365 0d0a 2020 2020 2020 2020 295b  alse..        )[
+00019d90: 333a 5d0d 0a20 2020 2020 2020 2064 6174  3:]..        dat
+00019da0: 6173 6574 5f69 6e64 6578 203d 2064 6174  aset_index = dat
+00019db0: 6173 6574 2e69 6e64 6578 0d0a 2020 2020  aset.index..    
+00019dc0: 2020 2020 7265 7475 726e 2064 6174 6173      return datas
+00019dd0: 6574 2c20 6461 7461 7365 745f 696e 6465  et, dataset_inde
+00019de0: 780d 0a20 2020 200d 0a64 6566 2067 6574  x..    ..def get
+00019df0: 5f73 706f 745f 6461 7461 7365 7428 7370  _spot_dataset(sp
+00019e00: 6f74 5f64 6174 6173 6574 2c20 7472 6163  ot_dataset, trac
+00019e10: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
+00019e20: 6b65 7973 2c20 7863 616c 6962 7261 7469  keys, xcalibrati
+00019e30: 6f6e 2c20 7963 616c 6962 7261 7469 6f6e  on, ycalibration
+00019e40: 2c20 7a63 616c 6962 7261 7469 6f6e 2c20  , zcalibration, 
+00019e50: 4174 7472 6962 7574 6542 6f78 6e61 6d65  AttributeBoxname
+00019e60: 2c20 6465 7465 6374 696f 6e63 6861 6e6e  , detectionchann
+00019e70: 656c 293a 0d0a 2020 2020 2020 2020 416c  el):..        Al
+00019e80: 6c56 616c 7565 7320 3d20 7b7d 0d0a 2020  lValues = {}..  
+00019e90: 2020 2020 2020 706f 7369 7820 3d20 7472        posix = tr
+00019ea0: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
+00019eb0: 745f 6b65 7973 5b22 706f 7369 7822 5d0d  t_keys["posix"].
+00019ec0: 0a20 2020 2020 2020 2070 6f73 6979 203d  .        posiy =
+00019ed0: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
+00019ee0: 7370 6f74 5f6b 6579 735b 2270 6f73 6979  spot_keys["posiy
+00019ef0: 225d 0d0a 2020 2020 2020 2020 706f 7369  "]..        posi
+00019f00: 7a20 3d20 7472 6163 6b5f 616e 616c 7973  z = track_analys
+00019f10: 6973 5f73 706f 745f 6b65 7973 5b22 706f  is_spot_keys["po
+00019f20: 7369 7a22 5d0d 0a20 2020 2020 2020 2066  siz"]..        f
+00019f30: 7261 6d65 203d 2074 7261 636b 5f61 6e61  rame = track_ana
+00019f40: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
+00019f50: 2266 7261 6d65 225d 0d0a 2020 2020 2020  "frame"]..      
+00019f60: 2020 0d0a 2020 2020 2020 2020 4c6f 6361    ..        Loca
+00019f70: 7469 6f6e 5820 3d20 280d 0a20 2020 2020  tionX = (..     
+00019f80: 2020 2020 2020 2073 706f 745f 6461 7461         spot_data
+00019f90: 7365 745b 706f 7369 785d 2e61 7374 7970  set[posix].astyp
+00019fa0: 6528 2266 6c6f 6174 2229 202f 2078 6361  e("float") / xca
+00019fb0: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
+00019fc0: 2020 2029 2e61 7374 7970 6528 2269 6e74     ).astype("int
+00019fd0: 2229 0d0a 2020 2020 2020 2020 4c6f 6361  ")..        Loca
+00019fe0: 7469 6f6e 5920 3d20 280d 0a20 2020 2020  tionY = (..     
+00019ff0: 2020 2020 2020 2073 706f 745f 6461 7461         spot_data
+0001a000: 7365 745b 706f 7369 795d 2e61 7374 7970  set[posiy].astyp
+0001a010: 6528 2266 6c6f 6174 2229 202f 2079 6361  e("float") / yca
+0001a020: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
+0001a030: 2020 2029 2e61 7374 7970 6528 2269 6e74     ).astype("int
+0001a040: 2229 0d0a 2020 2020 2020 2020 4c6f 6361  ")..        Loca
+0001a050: 7469 6f6e 5a20 3d20 280d 0a20 2020 2020  tionZ = (..     
+0001a060: 2020 2020 2020 2073 706f 745f 6461 7461         spot_data
+0001a070: 7365 745b 706f 7369 7a5d 2e61 7374 7970  set[posiz].astyp
+0001a080: 6528 2266 6c6f 6174 2229 202f 207a 6361  e("float") / zca
+0001a090: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
+0001a0a0: 2020 2029 2e61 7374 7970 6528 2269 6e74     ).astype("int
+0001a0b0: 2229 0d0a 2020 2020 2020 2020 4c6f 6361  ")..        Loca
+0001a0c0: 7469 6f6e 5420 3d20 2873 706f 745f 6461  tionT = (spot_da
+0001a0d0: 7461 7365 745b 6672 616d 655d 2e61 7374  taset[frame].ast
+0001a0e0: 7970 6528 2266 6c6f 6174 2229 292e 6173  ype("float")).as
+0001a0f0: 7479 7065 2822 696e 7422 290d 0a20 2020  type("int")..   
+0001a100: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
+0001a110: 2069 676e 6f72 655f 7661 6c75 6573 203d   ignore_values =
+0001a120: 205b 7472 6163 6b5f 616e 616c 7973 6973   [track_analysis
+0001a130: 5f73 706f 745f 6b65 7973 5b22 6d65 616e  _spot_keys["mean
+0001a140: 5f69 6e74 656e 7369 7479 225d 2c74 7261  _intensity"],tra
+0001a150: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+0001a160: 5f6b 6579 735b 2274 6f74 616c 5f69 6e74  _keys["total_int
+0001a170: 656e 7369 7479 225d 5d20 0d0a 2020 2020  ensity"]] ..    
+0001a180: 2020 2020 666f 7220 286b 2c76 2920 696e      for (k,v) in
+0001a190: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
+0001a1a0: 7370 6f74 5f6b 6579 732e 6974 656d 7328  spot_keys.items(
+0001a1b0: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
+0001a1c0: 2020 2020 2020 6966 2064 6574 6563 7469        if detecti
+0001a1d0: 6f6e 6368 616e 6e65 6c20 3d3d 2031 3a0d  onchannel == 1:.
+0001a1e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a1f0: 2020 2020 2020 6966 206b 203d 3d20 226d        if k == "m
+0001a200: 6561 6e5f 696e 7465 6e73 6974 795f 6368  ean_intensity_ch
+0001a210: 3222 3a0d 0a20 2020 2020 2020 2020 2020  2":..           
+0001a220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a230: 7661 6c75 6520 3d20 7472 6163 6b5f 616e  value = track_an
+0001a240: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+0001a250: 5b22 6d65 616e 5f69 6e74 656e 7369 7479  ["mean_intensity
+0001a260: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
+0001a270: 2020 2020 2020 2020 2020 2020 2020 2041                 A
+0001a280: 6c6c 5661 6c75 6573 5b76 616c 7565 5d20  llValues[value] 
+0001a290: 3d20 7370 6f74 5f64 6174 6173 6574 5b76  = spot_dataset[v
+0001a2a0: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
+0001a2b0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001a2c0: 2020 2020 2020 2020 6966 206b 203d 3d20          if k == 
+0001a2d0: 2274 6f74 616c 5f69 6e74 656e 7369 7479  "total_intensity
+0001a2e0: 5f63 6832 223a 0d0a 2020 2020 2020 2020  _ch2":..        
 0001a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a300: 7661 6c75 6520 3d20 7472 6163 6b5f 616e  value = track_an
-0001a310: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
-0001a320: 5b22 746f 7461 6c5f 696e 7465 6e73 6974  ["total_intensit
-0001a330: 7922 5d0d 0a20 2020 2020 2020 2020 2020  y"]..           
+0001a300: 2020 2076 616c 7565 203d 2074 7261 636b     value = track
+0001a310: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
+0001a320: 6579 735b 2274 6f74 616c 5f69 6e74 656e  eys["total_inten
+0001a330: 7369 7479 225d 0d0a 2020 2020 2020 2020  sity"]..        
 0001a340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a350: 416c 6c56 616c 7565 735b 7661 6c75 655d  AllValues[value]
-0001a360: 203d 2073 706f 745f 6461 7461 7365 745b   = spot_dataset[
-0001a370: 765d 2e61 7374 7970 6528 2266 6c6f 6174  v].astype("float
-0001a380: 2229 2020 2020 2020 200d 0a0d 0a20 2020  ")       ....   
-0001a390: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001a3a0: 7620 6e6f 7420 696e 2069 676e 6f72 655f  v not in ignore_
-0001a3b0: 7661 6c75 6573 3a0d 0a20 2020 2020 2020  values:..       
+0001a350: 2020 2041 6c6c 5661 6c75 6573 5b76 616c     AllValues[val
+0001a360: 7565 5d20 3d20 7370 6f74 5f64 6174 6173  ue] = spot_datas
+0001a370: 6574 5b76 5d2e 6173 7479 7065 2822 666c  et[v].astype("fl
+0001a380: 6f61 7422 2920 2020 2020 2020 0d0a 0d0a  oat")       ....
+0001a390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a3a0: 6966 2076 206e 6f74 2069 6e20 6967 6e6f  if v not in igno
+0001a3b0: 7265 5f76 616c 7565 733a 0d0a 2020 2020  re_values:..    
 0001a3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a3d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a3e0: 2020 2020 2020 2020 2041 6c6c 5661 6c75           AllValu
-0001a3f0: 6573 5b76 5d20 3d20 7370 6f74 5f64 6174  es[v] = spot_dat
-0001a400: 6173 6574 5b76 5d2e 6173 7479 7065 2822  aset[v].astype("
-0001a410: 666c 6f61 7422 290d 0a0d 0a20 2020 2020  float")....     
-0001a420: 2020 2041 6c6c 5661 6c75 6573 5b70 6f73     AllValues[pos
-0001a430: 6978 5d20 3d20 726f 756e 6428 4c6f 6361  ix] = round(Loca
-0001a440: 7469 6f6e 582c 3329 0d0a 2020 2020 2020  tionX,3)..      
-0001a450: 2020 416c 6c56 616c 7565 735b 706f 7369    AllValues[posi
-0001a460: 795d 203d 2072 6f75 6e64 284c 6f63 6174  y] = round(Locat
-0001a470: 696f 6e59 2c33 290d 0a20 2020 2020 2020  ionY,3)..       
-0001a480: 2041 6c6c 5661 6c75 6573 5b70 6f73 697a   AllValues[posiz
-0001a490: 5d20 3d20 726f 756e 6428 4c6f 6361 7469  ] = round(Locati
-0001a4a0: 6f6e 5a2c 3329 0d0a 2020 2020 2020 2020  onZ,3)..        
-0001a4b0: 416c 6c56 616c 7565 735b 6672 616d 655d  AllValues[frame]
-0001a4c0: 203d 2072 6f75 6e64 284c 6f63 6174 696f   = round(Locatio
-0001a4d0: 6e54 2c33 290d 0a20 2020 2020 2020 2041  nT,3)..        A
-0001a4e0: 7474 7269 6275 7465 6964 7320 3d20 5b5d  ttributeids = []
-0001a4f0: 0d0a 2020 2020 2020 2020 4174 7472 6962  ..        Attrib
-0001a500: 7574 6569 6473 2e61 7070 656e 6428 4174  uteids.append(At
-0001a510: 7472 6962 7574 6542 6f78 6e61 6d65 290d  tributeBoxname).
-0001a520: 0a20 2020 2020 2020 2066 6f72 2061 7474  .        for att
-0001a530: 7269 6275 7465 6e61 6d65 2069 6e20 416c  ributename in Al
-0001a540: 6c56 616c 7565 732e 6b65 7973 2829 3a0d  lValues.keys():.
-0001a550: 0a20 2020 2020 2020 2020 2020 2020 2041  .              A
-0001a560: 7474 7269 6275 7465 6964 732e 6170 7065  ttributeids.appe
-0001a570: 6e64 2861 7474 7269 6275 7465 6e61 6d65  nd(attributename
-0001a580: 2920 2020 200d 0a20 2020 2020 2020 2020  )    ..         
-0001a590: 2020 200d 0a20 2020 2020 2020 200d 0a20     ..        .. 
-0001a5a0: 2020 2020 2020 2072 6574 7572 6e20 4174         return At
-0001a5b0: 7472 6962 7574 6569 6473 2c20 416c 6c56  tributeids, AllV
-0001a5c0: 616c 7565 7320 2020 2020 0d0a 2020 2020  alues     ..    
-0001a5d0: 0d0a 6465 6620 6765 745f 7472 6163 6b5f  ..def get_track_
-0001a5e0: 6461 7461 7365 7428 7472 6163 6b5f 6461  dataset(track_da
-0001a5f0: 7461 7365 742c 2074 7261 636b 5f61 6e61  taset, track_ana
-0001a600: 6c79 7369 735f 7370 6f74 5f6b 6579 732c  lysis_spot_keys,
-0001a610: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
-0001a620: 7472 6163 6b5f 6b65 7973 2c20 5472 6163  track_keys, Trac
-0001a630: 6b41 7474 7269 6275 7465 426f 786e 616d  kAttributeBoxnam
-0001a640: 6529 3a0d 0a0d 0a20 2020 2020 2020 2041  e):....        A
-0001a650: 6c6c 5472 6163 6b56 616c 7565 7320 3d20  llTrackValues = 
-0001a660: 7b7d 0d0a 2020 2020 2020 2020 7472 6163  {}..        trac
-0001a670: 6b5f 6964 203d 2074 7261 636b 5f61 6e61  k_id = track_ana
-0001a680: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
-0001a690: 2274 7261 636b 5f69 6422 5d0d 0a20 2020  "track_id"]..   
-0001a6a0: 2020 2020 2054 6964 203d 2074 7261 636b       Tid = track
-0001a6b0: 5f64 6174 6173 6574 5b74 7261 636b 5f69  _dataset[track_i
-0001a6c0: 645d 2e61 7374 7970 6528 2266 6c6f 6174  d].astype("float
-0001a6d0: 2229 0d0a 2020 2020 2020 200d 0a20 2020  ")..       ..   
-0001a6e0: 2020 2020 2041 6c6c 5472 6163 6b56 616c       AllTrackVal
-0001a6f0: 7565 735b 7472 6163 6b5f 6964 5d20 3d20  ues[track_id] = 
-0001a700: 5469 640d 0a20 2020 2020 200d 0a20 2020  Tid..      ..   
-0001a710: 2020 2020 2066 6f72 2028 6b2c 2076 2920       for (k, v) 
-0001a720: 696e 2074 7261 636b 5f61 6e61 6c79 7369  in track_analysi
-0001a730: 735f 7472 6163 6b5f 6b65 7973 2e69 7465  s_track_keys.ite
-0001a740: 6d73 2829 3a0d 0a0d 0a20 2020 2020 2020  ms():....       
-0001a750: 2020 2020 2020 2020 2078 203d 2074 7261           x = tra
-0001a760: 636b 5f64 6174 6173 6574 5b76 5d2e 6173  ck_dataset[v].as
-0001a770: 7479 7065 2822 666c 6f61 7422 290d 0a20  type("float").. 
-0001a780: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0001a790: 696e 7661 6c20 3d20 6d69 6e28 7829 0d0a  inval = min(x)..
-0001a7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a7b0: 6d61 7876 616c 203d 206d 6178 2878 290d  maxval = max(x).
-0001a7c0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-0001a7d0: 2020 2069 6620 6d69 6e76 616c 203e 2030     if minval > 0
-0001a7e0: 2061 6e64 206d 6178 7661 6c20 3c3d 2031   and maxval <= 1
-0001a7f0: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
-0001a800: 2020 2020 2020 2020 2078 203d 2078 202b           x = x +
-0001a810: 2031 0d0a 0d0a 2020 2020 2020 2020 2020   1....          
-0001a820: 2020 2020 2020 416c 6c54 7261 636b 5661        AllTrackVa
-0001a830: 6c75 6573 5b6b 5d20 3d20 726f 756e 6428  lues[k] = round(
-0001a840: 782c 2033 290d 0a0d 0a20 2020 2020 2020  x, 3)....       
-0001a850: 2054 7261 636b 4174 7472 6962 7574 6569   TrackAttributei
-0001a860: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
-0001a870: 2054 7261 636b 4174 7472 6962 7574 6569   TrackAttributei
-0001a880: 6473 2e61 7070 656e 6428 5472 6163 6b41  ds.append(TrackA
-0001a890: 7474 7269 6275 7465 426f 786e 616d 6529  ttributeBoxname)
-0001a8a0: 0d0a 2020 2020 2020 2020 666f 7220 6174  ..        for at
-0001a8b0: 7472 6962 7574 656e 616d 6520 696e 2074  tributename in t
-0001a8c0: 7261 636b 5f61 6e61 6c79 7369 735f 7472  rack_analysis_tr
-0001a8d0: 6163 6b5f 6b65 7973 2e6b 6579 7328 293a  ack_keys.keys():
-0001a8e0: 0d0a 2020 2020 2020 2020 2020 2020 5472  ..            Tr
-0001a8f0: 6163 6b41 7474 7269 6275 7465 6964 732e  ackAttributeids.
-0001a900: 6170 7065 6e64 2861 7474 7269 6275 7465  append(attribute
-0001a910: 6e61 6d65 2920 2020 200d 0a20 2020 200d  name)    ..    .
-0001a920: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001a930: 5472 6163 6b41 7474 7269 6275 7465 6964  TrackAttributeid
-0001a940: 732c 2041 6c6c 5472 6163 6b56 616c 7565  s, AllTrackValue
-0001a950: 730d 0a20 2020 200d 0a64 6566 2067 6574  s..    ..def get
-0001a960: 5f65 6467 6573 5f64 6174 6173 6574 2865  _edges_dataset(e
-0001a970: 6467 6573 5f64 6174 6173 6574 2c20 6564  dges_dataset, ed
-0001a980: 6765 735f 6461 7461 7365 745f 696e 6465  ges_dataset_inde
-0001a990: 782c 2074 7261 636b 5f61 6e61 6c79 7369  x, track_analysi
-0001a9a0: 735f 7370 6f74 5f6b 6579 732c 2074 7261  s_spot_keys, tra
-0001a9b0: 636b 5f61 6e61 6c79 7369 735f 6564 6765  ck_analysis_edge
-0001a9c0: 735f 6b65 7973 293a 0d0a 0d0a 2020 2020  s_keys):....    
-0001a9d0: 2020 2020 416c 6c45 6467 6573 5661 6c75      AllEdgesValu
-0001a9e0: 6573 203d 207b 7d0d 0a20 2020 2020 2020  es = {}..       
-0001a9f0: 2074 7261 636b 5f69 6420 3d20 7472 6163   track_id = trac
-0001aa00: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-0001aa10: 6b65 7973 5b22 7472 6163 6b5f 6964 225d  keys["track_id"]
-0001aa20: 0d0a 2020 2020 2020 2020 5469 6420 3d20  ..        Tid = 
-0001aa30: 6564 6765 735f 6461 7461 7365 745b 7472  edges_dataset[tr
-0001aa40: 6163 6b5f 6964 5d2e 6173 7479 7065 2822  ack_id].astype("
-0001aa50: 666c 6f61 7422 290d 0a20 2020 2020 2020  float")..       
-0001aa60: 2069 6e64 6963 6573 203d 206e 702e 7768   indices = np.wh
-0001aa70: 6572 6528 5469 6420 3d3d 2030 290d 0a20  ere(Tid == 0).. 
-0001aa80: 2020 2020 2020 206d 6178 7472 6163 6b5f         maxtrack_
-0001aa90: 6964 203d 206d 6178 2854 6964 290d 0a20  id = max(Tid).. 
-0001aaa0: 2020 2020 2020 2063 6f6e 6469 7469 6f6e         condition
-0001aab0: 5f69 6e64 6963 6573 203d 2065 6467 6573  _indices = edges
-0001aac0: 5f64 6174 6173 6574 5f69 6e64 6578 5b69  _dataset_index[i
-0001aad0: 6e64 6963 6573 5d0d 0a20 2020 2020 2020  ndices]..       
-0001aae0: 2054 6964 5b63 6f6e 6469 7469 6f6e 5f69   Tid[condition_i
-0001aaf0: 6e64 6963 6573 5d20 3d20 6d61 7874 7261  ndices] = maxtra
-0001ab00: 636b 5f69 6420 2b20 310d 0a20 2020 2020  ck_id + 1..     
-0001ab10: 2020 2041 6c6c 4564 6765 7356 616c 7565     AllEdgesValue
-0001ab20: 735b 7472 6163 6b5f 6964 5d20 3d20 5469  s[track_id] = Ti
-0001ab30: 640d 0a0d 0a20 2020 2020 2020 2066 6f72  d....        for
-0001ab40: 206b 2069 6e20 7472 6163 6b5f 616e 616c   k in track_anal
-0001ab50: 7973 6973 5f65 6467 6573 5f6b 6579 732e  ysis_edges_keys.
-0001ab60: 7661 6c75 6573 2829 3a0d 0a0d 0a20 2020  values():....   
-0001ab70: 2020 2020 2020 2020 2069 6620 6b20 213d           if k !=
-0001ab80: 2074 7261 636b 5f69 643a 0d0a 2020 2020   track_id:..    
-0001ab90: 2020 2020 2020 2020 2020 2020 7820 3d20              x = 
-0001aba0: 6564 6765 735f 6461 7461 7365 745b 6b5d  edges_dataset[k]
-0001abb0: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
-0001abc0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001abd0: 2020 2020 416c 6c45 6467 6573 5661 6c75      AllEdgesValu
-0001abe0: 6573 5b6b 5d20 3d20 7820 2020 0d0a 2020  es[k] = x   ..  
-0001abf0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0001ac00: 2072 6574 7572 6e20 416c 6c45 6467 6573   return AllEdges
-0001ac10: 5661 6c75 6573 2020 200d 0a20 2020 200d  Values   ..    .
-0001ac20: 0a20 2020 2020 2020 0d0a 2020 2020 0d0a  .       ..    ..
-0001ac30: 6465 6620 7363 616c 655f 7661 6c75 6528  def scale_value(
-0001ac40: 782c 2073 6361 6c65 203d 2032 3535 202a  x, scale = 255 *
-0001ac50: 2032 3535 293a 0d0a 0d0a 0d0a 2020 2020   255):......    
-0001ac60: 2072 6574 7572 6e20 7820 2a20 7363 616c   return x * scal
-0001ac70: 6520 2020 0d0a 2020 2020 0d0a 0d0a 0d0a  e   ..    ......
-0001ac80: 6465 6620 7072 6f62 5f73 6967 6d6f 6964  def prob_sigmoid
-0001ac90: 2878 293a 0d0a 2020 2020 7265 7475 726e  (x):..    return
-0001aca0: 2031 202d 206d 6174 682e 6578 7028 2d78   1 - math.exp(-x
-0001acb0: 290d 0a0d 0a0d 0a64 6566 2061 6e67 756c  )......def angul
-0001acc0: 6172 5f63 6861 6e67 6528 7665 635f 302c  ar_change(vec_0,
-0001acd0: 2076 6563 5f31 293a 0d0a 2020 2020 2020   vec_1):..      
-0001ace0: 2020 0d0a 2020 2020 2020 2020 7665 635f    ..        vec_
-0001acf0: 3020 3d20 7665 635f 3020 2f20 6e70 2e6c  0 = vec_0 / np.l
-0001ad00: 696e 616c 672e 6e6f 726d 2876 6563 5f30  inalg.norm(vec_0
-0001ad10: 290d 0a20 2020 2020 2020 2076 6563 5f31  )..        vec_1
-0001ad20: 203d 2076 6563 5f31 202f 206e 702e 6c69   = vec_1 / np.li
-0001ad30: 6e61 6c67 2e6e 6f72 6d28 7665 635f 3129  nalg.norm(vec_1)
-0001ad40: 0d0a 2020 2020 2020 2020 616e 676c 6520  ..        angle 
-0001ad50: 3d20 6e70 2e61 7263 636f 7328 6e70 2e63  = np.arccos(np.c
-0001ad60: 6c69 7028 6e70 2e64 6f74 2876 6563 5f30  lip(np.dot(vec_0
-0001ad70: 2c20 7665 635f 3129 2c20 2d31 2e30 2c20  , vec_1), -1.0, 
-0001ad80: 312e 3029 290d 0a20 2020 2020 2020 2061  1.0))..        a
-0001ad90: 6e67 6c65 203d 2061 6e67 6c65 202a 2031  ngle = angle * 1
-0001ada0: 3830 202f 206e 702e 7069 0d0a 2020 2020  80 / np.pi..    
-0001adb0: 2020 2020 7265 7475 726e 2061 6e67 6c65      return angle
-0001adc0: 0d0a 2020 2020 200d 0a0d 0a64 6566 2065  ..     ....def e
-0001add0: 7661 6c5f 626f 6f6c 2876 616c 7565 293a  val_bool(value):
-0001ade0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001adf0: 2020 2020 0d0a 2020 2020 2020 2020 6966      ..        if
-0001ae00: 2076 616c 7565 2020 3d3d 2027 5472 7565   value  == 'True
-0001ae10: 273a 200d 0a20 2020 2020 2020 2020 2020  ': ..           
-0001ae20: 2020 2020 2064 6976 5f6b 6579 203d 2054       div_key = T
-0001ae30: 7275 650d 0a20 2020 2020 2020 2065 6c73  rue..        els
-0001ae40: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0001ae50: 2020 2020 6469 765f 6b65 7920 3d20 4661      div_key = Fa
-0001ae60: 6c73 6520 0d0a 0d0a 2020 2020 2020 2020  lse ....        
-0001ae70: 7265 7475 726e 2064 6976 5f6b 6579 2020  return div_key  
-0001ae80: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0001ae90: 0d0a 6465 6620 6368 6563 6b5f 616e 645f  ..def check_and_
-0001aea0: 7570 6461 7465 5f6d 6173 6b28 6d61 736b  update_mask(mask
-0001aeb0: 2c69 6d61 6765 293a 0d0a 2020 2020 2020  ,image):..      
-0001aec0: 200d 0a20 2020 2020 2020 2069 6620 6c65   ..        if le
-0001aed0: 6e28 6d61 736b 2e73 6861 7065 2920 3c20  n(mask.shape) < 
-0001aee0: 6c65 6e28 696d 6167 652e 7368 6170 6529  len(image.shape)
-0001aef0: 3a0d 0a20 2020 2020 2020 2020 2020 2075  :..            u
-0001af00: 7064 6174 655f 6d61 736b 203d 206e 702e  pdate_mask = np.
-0001af10: 7a65 726f 7328 0d0a 2020 2020 2020 2020  zeros(..        
+0001a3d0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0001a3e0: 2020 2020 2020 2020 2020 2020 416c 6c56              AllV
+0001a3f0: 616c 7565 735b 765d 203d 2073 706f 745f  alues[v] = spot_
+0001a400: 6461 7461 7365 745b 765d 2e61 7374 7970  dataset[v].astyp
+0001a410: 6528 2266 6c6f 6174 2229 0d0a 0d0a 2020  e("float")....  
+0001a420: 2020 2020 2020 416c 6c56 616c 7565 735b        AllValues[
+0001a430: 706f 7369 785d 203d 2072 6f75 6e64 284c  posix] = round(L
+0001a440: 6f63 6174 696f 6e58 2c33 290d 0a20 2020  ocationX,3)..   
+0001a450: 2020 2020 2041 6c6c 5661 6c75 6573 5b70       AllValues[p
+0001a460: 6f73 6979 5d20 3d20 726f 756e 6428 4c6f  osiy] = round(Lo
+0001a470: 6361 7469 6f6e 592c 3329 0d0a 2020 2020  cationY,3)..    
+0001a480: 2020 2020 416c 6c56 616c 7565 735b 706f      AllValues[po
+0001a490: 7369 7a5d 203d 2072 6f75 6e64 284c 6f63  siz] = round(Loc
+0001a4a0: 6174 696f 6e5a 2c33 290d 0a20 2020 2020  ationZ,3)..     
+0001a4b0: 2020 2041 6c6c 5661 6c75 6573 5b66 7261     AllValues[fra
+0001a4c0: 6d65 5d20 3d20 726f 756e 6428 4c6f 6361  me] = round(Loca
+0001a4d0: 7469 6f6e 542c 3329 0d0a 2020 2020 2020  tionT,3)..      
+0001a4e0: 2020 4174 7472 6962 7574 6569 6473 203d    Attributeids =
+0001a4f0: 205b 5d0d 0a20 2020 2020 2020 2041 7474   []..        Att
+0001a500: 7269 6275 7465 6964 732e 6170 7065 6e64  ributeids.append
+0001a510: 2841 7474 7269 6275 7465 426f 786e 616d  (AttributeBoxnam
+0001a520: 6529 0d0a 2020 2020 2020 2020 666f 7220  e)..        for 
+0001a530: 6174 7472 6962 7574 656e 616d 6520 696e  attributename in
+0001a540: 2041 6c6c 5661 6c75 6573 2e6b 6579 7328   AllValues.keys(
+0001a550: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0001a560: 2020 4174 7472 6962 7574 6569 6473 2e61    Attributeids.a
+0001a570: 7070 656e 6428 6174 7472 6962 7574 656e  ppend(attributen
+0001a580: 616d 6529 2020 2020 0d0a 2020 2020 2020  ame)    ..      
+0001a590: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0001a5a0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0001a5b0: 2041 7474 7269 6275 7465 6964 732c 2041   Attributeids, A
+0001a5c0: 6c6c 5661 6c75 6573 2020 2020 200d 0a20  llValues     .. 
+0001a5d0: 2020 200d 0a64 6566 2067 6574 5f74 7261     ..def get_tra
+0001a5e0: 636b 5f64 6174 6173 6574 2874 7261 636b  ck_dataset(track
+0001a5f0: 5f64 6174 6173 6574 2c20 7472 6163 6b5f  _dataset, track_
+0001a600: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+0001a610: 7973 2c20 7472 6163 6b5f 616e 616c 7973  ys, track_analys
+0001a620: 6973 5f74 7261 636b 5f6b 6579 732c 2054  is_track_keys, T
+0001a630: 7261 636b 4174 7472 6962 7574 6542 6f78  rackAttributeBox
+0001a640: 6e61 6d65 293a 0d0a 0d0a 2020 2020 2020  name):....      
+0001a650: 2020 416c 6c54 7261 636b 5661 6c75 6573    AllTrackValues
+0001a660: 203d 207b 7d0d 0a20 2020 2020 2020 2074   = {}..        t
+0001a670: 7261 636b 5f69 6420 3d20 7472 6163 6b5f  rack_id = track_
+0001a680: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+0001a690: 7973 5b22 7472 6163 6b5f 6964 225d 0d0a  ys["track_id"]..
+0001a6a0: 2020 2020 2020 2020 5469 6420 3d20 7472          Tid = tr
+0001a6b0: 6163 6b5f 6461 7461 7365 745b 7472 6163  ack_dataset[trac
+0001a6c0: 6b5f 6964 5d2e 6173 7479 7065 2822 666c  k_id].astype("fl
+0001a6d0: 6f61 7422 290d 0a20 2020 2020 2020 0d0a  oat")..       ..
+0001a6e0: 2020 2020 2020 2020 416c 6c54 7261 636b          AllTrack
+0001a6f0: 5661 6c75 6573 5b74 7261 636b 5f69 645d  Values[track_id]
+0001a700: 203d 2054 6964 0d0a 2020 2020 2020 0d0a   = Tid..      ..
+0001a710: 2020 2020 2020 2020 666f 7220 286b 2c20          for (k, 
+0001a720: 7629 2069 6e20 7472 6163 6b5f 616e 616c  v) in track_anal
+0001a730: 7973 6973 5f74 7261 636b 5f6b 6579 732e  ysis_track_keys.
+0001a740: 6974 656d 7328 293a 0d0a 0d0a 2020 2020  items():....    
+0001a750: 2020 2020 2020 2020 2020 2020 7820 3d20              x = 
+0001a760: 7472 6163 6b5f 6461 7461 7365 745b 765d  track_dataset[v]
+0001a770: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
+0001a780: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001a790: 2020 6d69 6e76 616c 203d 206d 696e 2878    minval = min(x
+0001a7a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001a7b0: 2020 206d 6178 7661 6c20 3d20 6d61 7828     maxval = max(
+0001a7c0: 7829 0d0a 0d0a 2020 2020 2020 2020 2020  x)....          
+0001a7d0: 2020 2020 2020 6966 206d 696e 7661 6c20        if minval 
+0001a7e0: 3e20 3020 616e 6420 6d61 7876 616c 203c  > 0 and maxval <
+0001a7f0: 3d20 313a 0d0a 0d0a 2020 2020 2020 2020  = 1:....        
+0001a800: 2020 2020 2020 2020 2020 2020 7820 3d20              x = 
+0001a810: 7820 2b20 310d 0a0d 0a20 2020 2020 2020  x + 1....       
+0001a820: 2020 2020 2020 2020 2041 6c6c 5472 6163           AllTrac
+0001a830: 6b56 616c 7565 735b 6b5d 203d 2072 6f75  kValues[k] = rou
+0001a840: 6e64 2878 2c20 3329 0d0a 0d0a 2020 2020  nd(x, 3)....    
+0001a850: 2020 2020 5472 6163 6b41 7474 7269 6275      TrackAttribu
+0001a860: 7465 6964 7320 3d20 5b5d 0d0a 2020 2020  teids = []..    
+0001a870: 2020 2020 5472 6163 6b41 7474 7269 6275      TrackAttribu
+0001a880: 7465 6964 732e 6170 7065 6e64 2854 7261  teids.append(Tra
+0001a890: 636b 4174 7472 6962 7574 6542 6f78 6e61  ckAttributeBoxna
+0001a8a0: 6d65 290d 0a20 2020 2020 2020 2066 6f72  me)..        for
+0001a8b0: 2061 7474 7269 6275 7465 6e61 6d65 2069   attributename i
+0001a8c0: 6e20 7472 6163 6b5f 616e 616c 7973 6973  n track_analysis
+0001a8d0: 5f74 7261 636b 5f6b 6579 732e 6b65 7973  _track_keys.keys
+0001a8e0: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+0001a8f0: 2054 7261 636b 4174 7472 6962 7574 6569   TrackAttributei
+0001a900: 6473 2e61 7070 656e 6428 6174 7472 6962  ds.append(attrib
+0001a910: 7574 656e 616d 6529 2020 2020 0d0a 2020  utename)    ..  
+0001a920: 2020 0d0a 2020 2020 2020 2020 7265 7475    ..        retu
+0001a930: 726e 2054 7261 636b 4174 7472 6962 7574  rn TrackAttribut
+0001a940: 6569 6473 2c20 416c 6c54 7261 636b 5661  eids, AllTrackVa
+0001a950: 6c75 6573 0d0a 2020 2020 0d0a 6465 6620  lues..    ..def 
+0001a960: 6765 745f 6564 6765 735f 6461 7461 7365  get_edges_datase
+0001a970: 7428 6564 6765 735f 6461 7461 7365 742c  t(edges_dataset,
+0001a980: 2065 6467 6573 5f64 6174 6173 6574 5f69   edges_dataset_i
+0001a990: 6e64 6578 2c20 7472 6163 6b5f 616e 616c  ndex, track_anal
+0001a9a0: 7973 6973 5f73 706f 745f 6b65 7973 2c20  ysis_spot_keys, 
+0001a9b0: 7472 6163 6b5f 616e 616c 7973 6973 5f65  track_analysis_e
+0001a9c0: 6467 6573 5f6b 6579 7329 3a0d 0a0d 0a20  dges_keys):.... 
+0001a9d0: 2020 2020 2020 2041 6c6c 4564 6765 7356         AllEdgesV
+0001a9e0: 616c 7565 7320 3d20 7b7d 0d0a 2020 2020  alues = {}..    
+0001a9f0: 2020 2020 7472 6163 6b5f 6964 203d 2074      track_id = t
+0001aa00: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+0001aa10: 6f74 5f6b 6579 735b 2274 7261 636b 5f69  ot_keys["track_i
+0001aa20: 6422 5d0d 0a20 2020 2020 2020 2054 6964  d"]..        Tid
+0001aa30: 203d 2065 6467 6573 5f64 6174 6173 6574   = edges_dataset
+0001aa40: 5b74 7261 636b 5f69 645d 2e61 7374 7970  [track_id].astyp
+0001aa50: 6528 2266 6c6f 6174 2229 0d0a 2020 2020  e("float")..    
+0001aa60: 2020 2020 696e 6469 6365 7320 3d20 6e70      indices = np
+0001aa70: 2e77 6865 7265 2854 6964 203d 3d20 3029  .where(Tid == 0)
+0001aa80: 0d0a 2020 2020 2020 2020 6d61 7874 7261  ..        maxtra
+0001aa90: 636b 5f69 6420 3d20 6d61 7828 5469 6429  ck_id = max(Tid)
+0001aaa0: 0d0a 2020 2020 2020 2020 636f 6e64 6974  ..        condit
+0001aab0: 696f 6e5f 696e 6469 6365 7320 3d20 6564  ion_indices = ed
+0001aac0: 6765 735f 6461 7461 7365 745f 696e 6465  ges_dataset_inde
+0001aad0: 785b 696e 6469 6365 735d 0d0a 2020 2020  x[indices]..    
+0001aae0: 2020 2020 5469 645b 636f 6e64 6974 696f      Tid[conditio
+0001aaf0: 6e5f 696e 6469 6365 735d 203d 206d 6178  n_indices] = max
+0001ab00: 7472 6163 6b5f 6964 202b 2031 0d0a 2020  track_id + 1..  
+0001ab10: 2020 2020 2020 416c 6c45 6467 6573 5661        AllEdgesVa
+0001ab20: 6c75 6573 5b74 7261 636b 5f69 645d 203d  lues[track_id] =
+0001ab30: 2054 6964 0d0a 0d0a 2020 2020 2020 2020   Tid....        
+0001ab40: 666f 7220 6b20 696e 2074 7261 636b 5f61  for k in track_a
+0001ab50: 6e61 6c79 7369 735f 6564 6765 735f 6b65  nalysis_edges_ke
+0001ab60: 7973 2e76 616c 7565 7328 293a 0d0a 0d0a  ys.values():....
+0001ab70: 2020 2020 2020 2020 2020 2020 6966 206b              if k
+0001ab80: 2021 3d20 7472 6163 6b5f 6964 3a0d 0a20   != track_id:.. 
+0001ab90: 2020 2020 2020 2020 2020 2020 2020 2078                 x
+0001aba0: 203d 2065 6467 6573 5f64 6174 6173 6574   = edges_dataset
+0001abb0: 5b6b 5d2e 6173 7479 7065 2822 666c 6f61  [k].astype("floa
+0001abc0: 7422 290d 0a0d 0a20 2020 2020 2020 2020  t")....         
+0001abd0: 2020 2020 2020 2041 6c6c 4564 6765 7356         AllEdgesV
+0001abe0: 616c 7565 735b 6b5d 203d 2078 2020 200d  alues[k] = x   .
+0001abf0: 0a20 2020 2020 2020 2020 0d0a 2020 2020  .         ..    
+0001ac00: 2020 2020 7265 7475 726e 2041 6c6c 4564      return AllEd
+0001ac10: 6765 7356 616c 7565 7320 2020 0d0a 2020  gesValues   ..  
+0001ac20: 2020 0d0a 2020 2020 2020 200d 0a20 2020    ..       ..   
+0001ac30: 200d 0a64 6566 2073 6361 6c65 5f76 616c   ..def scale_val
+0001ac40: 7565 2878 2c20 7363 616c 6520 3d20 3235  ue(x, scale = 25
+0001ac50: 3520 2a20 3235 3529 3a0d 0a0d 0a0d 0a20  5 * 255):...... 
+0001ac60: 2020 2020 7265 7475 726e 2078 202a 2073      return x * s
+0001ac70: 6361 6c65 2020 200d 0a20 2020 200d 0a0d  cale   ..    ...
+0001ac80: 0a0d 0a64 6566 2070 726f 625f 7369 676d  ...def prob_sigm
+0001ac90: 6f69 6428 7829 3a0d 0a20 2020 2072 6574  oid(x):..    ret
+0001aca0: 7572 6e20 3120 2d20 6d61 7468 2e65 7870  urn 1 - math.exp
+0001acb0: 282d 7829 0d0a 0d0a 0d0a 6465 6620 616e  (-x)......def an
+0001acc0: 6775 6c61 725f 6368 616e 6765 2876 6563  gular_change(vec
+0001acd0: 5f30 2c20 7665 635f 3129 3a0d 0a20 2020  _0, vec_1):..   
+0001ace0: 2020 2020 200d 0a20 2020 2020 2020 2076       ..        v
+0001acf0: 6563 5f30 203d 2076 6563 5f30 202f 206e  ec_0 = vec_0 / n
+0001ad00: 702e 6c69 6e61 6c67 2e6e 6f72 6d28 7665  p.linalg.norm(ve
+0001ad10: 635f 3029 0d0a 2020 2020 2020 2020 7665  c_0)..        ve
+0001ad20: 635f 3120 3d20 7665 635f 3120 2f20 6e70  c_1 = vec_1 / np
+0001ad30: 2e6c 696e 616c 672e 6e6f 726d 2876 6563  .linalg.norm(vec
+0001ad40: 5f31 290d 0a20 2020 2020 2020 2061 6e67  _1)..        ang
+0001ad50: 6c65 203d 206e 702e 6172 6363 6f73 286e  le = np.arccos(n
+0001ad60: 702e 636c 6970 286e 702e 646f 7428 7665  p.clip(np.dot(ve
+0001ad70: 635f 302c 2076 6563 5f31 292c 202d 312e  c_0, vec_1), -1.
+0001ad80: 302c 2031 2e30 2929 0d0a 2020 2020 2020  0, 1.0))..      
+0001ad90: 2020 616e 676c 6520 3d20 616e 676c 6520    angle = angle 
+0001ada0: 2a20 3138 3020 2f20 6e70 2e70 690d 0a20  * 180 / np.pi.. 
+0001adb0: 2020 2020 2020 2072 6574 7572 6e20 616e         return an
+0001adc0: 676c 650d 0a20 2020 2020 0d0a 0d0a 6465  gle..     ....de
+0001add0: 6620 6576 616c 5f62 6f6f 6c28 7661 6c75  f eval_bool(valu
+0001ade0: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
+0001adf0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001ae00: 2069 6620 7661 6c75 6520 203d 3d20 2754   if value  == 'T
+0001ae10: 7275 6527 3a20 0d0a 2020 2020 2020 2020  rue': ..        
+0001ae20: 2020 2020 2020 2020 6469 765f 6b65 7920          div_key 
+0001ae30: 3d20 5472 7565 0d0a 2020 2020 2020 2020  = True..        
+0001ae40: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+0001ae50: 2020 2020 2020 2064 6976 5f6b 6579 203d         div_key =
+0001ae60: 2046 616c 7365 200d 0a0d 0a20 2020 2020   False ....     
+0001ae70: 2020 2072 6574 7572 6e20 6469 765f 6b65     return div_ke
+0001ae80: 7920 2020 2020 2020 2020 2020 2020 2020  y               
+0001ae90: 200d 0a0d 0a64 6566 2063 6865 636b 5f61   ....def check_a
+0001aea0: 6e64 5f75 7064 6174 655f 6d61 736b 286d  nd_update_mask(m
+0001aeb0: 6173 6b2c 696d 6167 6529 3a0d 0a20 2020  ask,image):..   
+0001aec0: 2020 2020 0d0a 2020 2020 2020 2020 6966      ..        if
+0001aed0: 206c 656e 286d 6173 6b2e 7368 6170 6529   len(mask.shape)
+0001aee0: 203c 206c 656e 2869 6d61 6765 2e73 6861   < len(image.sha
+0001aef0: 7065 293a 0d0a 2020 2020 2020 2020 2020  pe):..          
+0001af00: 2020 7570 6461 7465 5f6d 6173 6b20 3d20    update_mask = 
+0001af10: 6e70 2e7a 6572 6f73 280d 0a20 2020 2020  np.zeros(..     
 0001af20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af30: 2020 2020 5b0d 0a20 2020 2020 2020 2020      [..         
+0001af30: 2020 2020 2020 205b 0d0a 2020 2020 2020         [..      
 0001af40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af50: 2020 2020 2020 2069 6d61 6765 2e73 6861         image.sha
-0001af60: 7065 5b30 5d2c 0d0a 2020 2020 2020 2020  pe[0],..        
+0001af50: 2020 2020 2020 2020 2020 696d 6167 652e            image.
+0001af60: 7368 6170 655b 305d 2c0d 0a20 2020 2020  shape[0],..     
 0001af70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af80: 2020 2020 2020 2020 696d 6167 652e 7368          image.sh
-0001af90: 6170 655b 315d 2c0d 0a20 2020 2020 2020  ape[1],..       
+0001af80: 2020 2020 2020 2020 2020 2069 6d61 6765             image
+0001af90: 2e73 6861 7065 5b31 5d2c 0d0a 2020 2020  .shape[1],..    
 0001afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001afb0: 2020 2020 2020 2020 2069 6d61 6765 2e73           image.s
-0001afc0: 6861 7065 5b32 5d2c 0d0a 2020 2020 2020  hape[2],..      
+0001afb0: 2020 2020 2020 2020 2020 2020 696d 6167              imag
+0001afc0: 652e 7368 6170 655b 325d 2c0d 0a20 2020  e.shape[2],..   
 0001afd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001afe0: 2020 2020 2020 2020 2020 696d 6167 652e            image.
-0001aff0: 7368 6170 655b 335d 2c0d 0a20 2020 2020  shape[3],..     
+0001afe0: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
+0001aff0: 6765 2e73 6861 7065 5b33 5d2c 0d0a 2020  ge.shape[3],..  
 0001b000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b010: 2020 2020 2020 205d 0d0a 2020 2020 2020         ]..      
+0001b010: 2020 2020 2020 2020 2020 5d0d 0a20 2020            ]..   
 0001b020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b030: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-0001b040: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-0001b050: 302c 2075 7064 6174 655f 6d61 736b 2e73  0, update_mask.s
-0001b060: 6861 7065 5b30 5d29 3a0d 0a20 2020 2020  hape[0]):..     
-0001b070: 2020 2020 2020 2020 2020 2066 6f72 206a             for j
-0001b080: 2069 6e20 7261 6e67 6528 302c 2075 7064   in range(0, upd
-0001b090: 6174 655f 6d61 736b 2e73 6861 7065 5b31  ate_mask.shape[1
-0001b0a0: 5d29 3a0d 0a0d 0a20 2020 2020 2020 2020  ]):....         
-0001b0b0: 2020 2020 2020 2020 2020 2075 7064 6174             updat
-0001b0c0: 655f 6d61 736b 5b69 2c20 6a2c 203a 2c20  e_mask[i, j, :, 
-0001b0d0: 3a5d 203d 206d 6173 6b5b 692c 203a 2c20  :] = mask[i, :, 
-0001b0e0: 3a5d 0d0a 2020 2020 2020 2020 656c 7365  :]..        else
-0001b0f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001b100: 2020 2075 7064 6174 655f 6d61 736b 203d     update_mask =
-0001b110: 206d 6173 6b0d 0a0d 0a20 2020 2020 2020   mask....       
-0001b120: 2072 6574 7572 6e20 7570 6461 7465 5f6d   return update_m
-0001b130: 6173 6b20 2020 2020 2020 200d 0a20 2020  ask        ..   
-0001b140: 2020 2020 0d0a                               ..
+0001b030: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+0001b040: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+0001b050: 6765 2830 2c20 7570 6461 7465 5f6d 6173  ge(0, update_mas
+0001b060: 6b2e 7368 6170 655b 305d 293a 0d0a 2020  k.shape[0]):..  
+0001b070: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0001b080: 7220 6a20 696e 2072 616e 6765 2830 2c20  r j in range(0, 
+0001b090: 7570 6461 7465 5f6d 6173 6b2e 7368 6170  update_mask.shap
+0001b0a0: 655b 315d 293a 0d0a 0d0a 2020 2020 2020  e[1]):....      
+0001b0b0: 2020 2020 2020 2020 2020 2020 2020 7570                up
+0001b0c0: 6461 7465 5f6d 6173 6b5b 692c 206a 2c20  date_mask[i, j, 
+0001b0d0: 3a2c 203a 5d20 3d20 6d61 736b 5b69 2c20  :, :] = mask[i, 
+0001b0e0: 3a2c 203a 5d0d 0a20 2020 2020 2020 2065  :, :]..        e
+0001b0f0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+0001b100: 2020 2020 2020 7570 6461 7465 5f6d 6173        update_mas
+0001b110: 6b20 3d20 6d61 736b 0d0a 0d0a 2020 2020  k = mask....    
+0001b120: 2020 2020 7265 7475 726e 2075 7064 6174      return updat
+0001b130: 655f 6d61 736b 2020 2020 2020 2020 0d0a  e_mask        ..
+0001b140: 2020 2020 2020 200d 0a                          ..
```

### Comparing `napatrackmater-3.4.4/napatrackmater/Trackvector.py` & `napatrackmater-3.4.5/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.4/napatrackmater/__init__.py` & `napatrackmater-3.4.5/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.4/napatrackmater/clustering.py` & `napatrackmater-3.4.5/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.4/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.4.5/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.4/napatrackmater/fate_mapping.py` & `napatrackmater-3.4.5/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.4/napatrackmater/pretrained.py` & `napatrackmater-3.4.5/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.4/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.4.5/napatrackmater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.4.4
+Version: 3.4.5
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.4.4/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.4.5/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.4.4/setup.py` & `napatrackmater-3.4.5/setup.py`

 * *Files identical despite different names*

