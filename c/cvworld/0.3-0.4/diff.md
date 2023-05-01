# Comparing `tmp/cvworld-0.3.tar.gz` & `tmp/cvworld-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cvworld-0.3.tar", last modified: Sun Apr 30 15:49:20 2023, max compression
+gzip compressed data, was "dist\cvworld-0.4.tar", last modified: Mon May  1 08:24:45 2023, max compression
```

## Comparing `cvworld-0.3.tar` & `cvworld-0.4.tar`

### file list

```diff
@@ -1,8 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 15:49:20.742515 cvworld-0.3/
--rw-rw-rw-   0        0        0      782 2023-04-30 15:49:20.758157 cvworld-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-30 15:49:20.742515 cvworld-0.3/cvworld/
--rw-rw-rw-   0        0        0     2400 2023-04-29 06:59:46.304811 cvworld-0.3/cvworld/FaceTrackingModule.py
--rw-rw-rw-   0        0        0     2226 2023-04-30 07:06:44.095856 cvworld-0.3/cvworld/HandTrachkingModule.py
--rw-rw-rw-   0        0        0      744 2023-04-30 15:14:31.796339 cvworld-0.3/cvworld/cornerRectModule.py
--rw-rw-rw-   0        0        0       39 2023-04-30 07:22:38.469288 cvworld-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1691 2023-04-30 15:49:15.258277 cvworld-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:24:45.786504 cvworld-0.4/
+-rw-rw-rw-   0        0        0      782 2023-05-01 08:24:45.802124 cvworld-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-01 08:24:45.786504 cvworld-0.4/cvworld/
+-rw-rw-rw-   0        0        0     2400 2023-04-29 06:59:46.304811 cvworld-0.4/cvworld/FaceTrackingModule.py
+-rw-rw-rw-   0        0        0     2226 2023-05-01 08:21:19.824516 cvworld-0.4/cvworld/HandTrachkingModule.py
+-rw-rw-rw-   0        0        0     2509 2023-05-01 08:21:19.840131 cvworld-0.4/cvworld/Utils.py
+-rw-rw-rw-   0        0        0      197 2023-05-01 08:21:27.971225 cvworld-0.4/cvworld/__init__.py
+-rw-rw-rw-   0        0        0       39 2023-04-30 07:22:38.469288 cvworld-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1691 2023-05-01 08:24:34.509982 cvworld-0.4/setup.py
```

### Comparing `cvworld-0.3/PKG-INFO` & `cvworld-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cvworld
-Version: 0.3
+Version: 0.4
 Summary: Computer Vision Helper Function
 Home-page: https://github.com/user/reponame
 Author: Sethu Raman
 Author-email: sethuramanvr046@gmail.com
 License: MIT
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Description: UNKNOWN
```

### Comparing `cvworld-0.3/cvworld/FaceTrackingModule.py` & `cvworld-0.4/cvworld/FaceTrackingModule.py`

 * *Files identical despite different names*

### Comparing `cvworld-0.3/cvworld/HandTrachkingModule.py` & `cvworld-0.4/cvworld/HandTrachkingModule.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import cv2
 import mediapipe as mp
 import time
 
 
-class handDetector():
+class HandDetector():
     def __init__(self, mode=False, maxHands=2, detectionCon=1, trackCon=0.5):
         self.mode = mode
         self.maxHands = int(maxHands)
         self.detectionCon = detectionCon
         self.trackCon = trackCon
 
         self.mpHands = mp.solutions.hands
@@ -43,15 +43,15 @@
 
         return lmList
 
 def main():
     pTime = 0
     cTime = 0
     cap = cv2.VideoCapture(0)
-    detector = handDetector()
+    detector = HandDetector()
     while True:
         success, img = cap.read()
         img = detector.findHands(img)
         lmList = detector.findPosition(img)
         if len(lmList) != 0:
             print(lmList[4])
```

### Comparing `cvworld-0.3/setup.py` & `cvworld-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'cvworld',         # How you named your package folder (MyLib)
   packages = ['cvworld'],   # Chose the same as "name"
-  version = '0.3',      # Start with a small number and increase it with every change you make
+  version = '0.4',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Computer Vision Helper Function',   # Give a short description about your library
   author = 'Sethu Raman',                   # Type in your name
   author_email = 'sethuramanvr046@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/user/reponame',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['ComputerVision', 'FaceDetection', 'HandTracking'],   # Keywords that define your package best
```

