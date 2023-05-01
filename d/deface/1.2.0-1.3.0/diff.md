# Comparing `tmp/deface-1.2.0.tar.gz` & `tmp/deface-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deface-1.2.0.tar", last modified: Tue Jan 10 17:00:59 2023, max compression
+gzip compressed data, was "deface-1.3.0.tar", last modified: Mon May  1 20:24:19 2023, max compression
```

## Comparing `deface-1.2.0.tar` & `deface-1.3.0.tar`

### file list

```diff
@@ -1,21 +1,33 @@
-drwxr-xr-x   0 m4        (1000) m4        (1000)        0 2023-01-10 17:00:59.811369 deface-1.2.0/
--rw-r--r--   0 m4        (1000) m4        (1000)     1073 2020-02-04 19:18:27.000000 deface-1.2.0/LICENSE
--rw-r--r--   0 m4        (1000) m4        (1000)       80 2020-02-19 23:10:04.000000 deface-1.2.0/MANIFEST.in
--rw-r--r--   0 m4        (1000) m4        (1000)    12649 2023-01-10 17:00:59.811369 deface-1.2.0/PKG-INFO
--rw-r--r--   0 m4        (1000) m4        (1000)    12153 2021-12-10 03:18:37.000000 deface-1.2.0/README.md
-drwxr-xr-x   0 m4        (1000) m4        (1000)        0 2023-01-10 17:00:59.811369 deface-1.2.0/deface/
--rw-r--r--   0 m4        (1000) m4        (1000)       93 2020-02-19 04:48:55.000000 deface-1.2.0/deface/__init__.py
--rw-r--r--   0 m4        (1000) m4        (1000)      497 2023-01-10 17:00:59.811369 deface-1.2.0/deface/_version.py
--rw-r--r--   0 m4        (1000) m4        (1000)  7532772 2019-10-18 16:30:49.000000 deface-1.2.0/deface/centerface.onnx
--rw-r--r--   0 m4        (1000) m4        (1000)     7248 2023-01-10 16:25:32.000000 deface-1.2.0/deface/centerface.py
--rwxr-xr-x   0 m4        (1000) m4        (1000)    14169 2023-01-10 16:47:50.000000 deface-1.2.0/deface/deface.py
-drwxr-xr-x   0 m4        (1000) m4        (1000)        0 2023-01-10 17:00:59.811369 deface-1.2.0/deface.egg-info/
--rw-r--r--   0 m4        (1000) m4        (1000)    12649 2023-01-10 17:00:59.000000 deface-1.2.0/deface.egg-info/PKG-INFO
--rw-r--r--   0 m4        (1000) m4        (1000)      343 2023-01-10 17:00:59.000000 deface-1.2.0/deface.egg-info/SOURCES.txt
--rw-r--r--   0 m4        (1000) m4        (1000)        1 2023-01-10 17:00:59.000000 deface-1.2.0/deface.egg-info/dependency_links.txt
--rw-r--r--   0 m4        (1000) m4        (1000)       47 2023-01-10 17:00:59.000000 deface-1.2.0/deface.egg-info/entry_points.txt
--rw-r--r--   0 m4        (1000) m4        (1000)       84 2023-01-10 17:00:59.000000 deface-1.2.0/deface.egg-info/requires.txt
--rw-r--r--   0 m4        (1000) m4        (1000)        7 2023-01-10 17:00:59.000000 deface-1.2.0/deface.egg-info/top_level.txt
--rw-r--r--   0 m4        (1000) m4        (1000)      171 2023-01-10 17:00:59.811369 deface-1.2.0/setup.cfg
--rw-r--r--   0 m4        (1000) m4        (1000)     1119 2020-02-25 15:00:09.000000 deface-1.2.0/setup.py
--rw-r--r--   0 m4        (1000) m4        (1000)    68611 2020-02-19 04:48:55.000000 deface-1.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:24:19.761496 deface-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-01 20:24:05.000000 deface-1.3.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:24:19.749496 deface-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:24:19.749496 deface-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-01 20:24:05.000000 deface-1.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-01 20:24:05.000000 deface-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-01 20:24:05.000000 deface-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-05-01 20:24:19.761496 deface-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-05-01 20:24:05.000000 deface-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:24:19.757496 deface-1.3.0/deface/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-01 20:24:05.000000 deface-1.3.0/deface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 20:24:19.000000 deface-1.3.0/deface/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)  7532772 2023-05-01 20:24:05.000000 deface-1.3.0/deface/centerface.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-05-01 20:24:05.000000 deface-1.3.0/deface/centerface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14681 2023-05-01 20:24:05.000000 deface-1.3.0/deface/deface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:24:19.757496 deface-1.3.0/deface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-05-01 20:24:19.000000 deface-1.3.0/deface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-01 20:24:19.000000 deface-1.3.0/deface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:24:19.000000 deface-1.3.0/deface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-01 20:24:19.000000 deface-1.3.0/deface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-01 20:24:19.000000 deface-1.3.0/deface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-01 20:24:19.000000 deface-1.3.0/deface.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-01 20:24:05.000000 deface-1.3.0/deface.spec
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:24:19.761496 deface-1.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    83046 2023-05-01 20:24:05.000000 deface-1.3.0/examples/city.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    82598 2023-05-01 20:24:05.000000 deface-1.3.0/examples/city_anonymized.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    80240 2023-05-01 20:24:05.000000 deface-1.3.0/examples/city_anonymized_boxes.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    86879 2023-05-01 20:24:05.000000 deface-1.3.0/examples/city_anonymized_scores.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    78648 2023-05-01 20:24:05.000000 deface-1.3.0/examples/city_anonymized_thresh0.02.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    83369 2023-05-01 20:24:05.000000 deface-1.3.0/examples/city_anonymized_thresh0.7.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-01 20:24:05.000000 deface-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-01 20:24:05.000000 deface-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 20:24:19.761496 deface-1.3.0/setup.cfg
```

### Comparing `deface-1.2.0/LICENSE` & `deface-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deface-1.2.0/PKG-INFO` & `deface-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,48 @@
 Metadata-Version: 2.1
 Name: deface
-Version: 1.2.0
+Version: 1.3.0
 Summary: Video anonymization by face detection
-Home-page: https://github.com/ORB-HD/deface
-Author: Martin Drawitsch
-Author-email: martin.drawitsch@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
+License: MIT License
+        
+        Copyright (c) 2020 Martin Drawitsch
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: repository, https://github.com/ORB-HD/deface
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Classifier: Topic :: Scientific/Engineering :: Image Recognition
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
 License-File: LICENSE
 
 # `deface`: Video anonymization by face detection
 
 `deface` is a simple command-line tool for automatic anonymization of faces in videos or photos.
 It works by first detecting all human faces in each video frame and then applying an anonymization filter (blurring or black boxes) on each detected face region.
-All audio tracks are discarded as well.
+By default all audio tracks are discarded as well.
 
 
 Original frame | `deface` output (using default options)
 :--:|:--:
 ![examples/city.jpg](examples/city.jpg) | ![$ deface examples/city.jpg](examples/city_anonymized.jpg)
 
 
@@ -68,16 +87,16 @@
 
 The output may vary depending on your installed version, but it should look similar to this:
 
 ```
 usage: deface [--output O] [--thresh T] [--scale WxH] [--preview] [--boxes]
               [--draw-scores] [--mask-scale M]
               [--replacewith {blur,solid,none,img}] [--replaceimg REPLACEIMG]
-              [--ffmpeg-config FFMPEG_CONFIG] [--backend {auto,onnxrt,opencv}]
-              [--version] [--help]
+              [--keep-audio] [--ffmpeg-config FFMPEG_CONFIG]
+              [--backend {auto,onnxrt,opencv}] [--version] [--help]
               [input ...]
 
 Video anonymization by face detection
 
 positional arguments:
   input                 File path(s) or camera device name. It is possible to
                         pass multiple paths by separating them by spaces or by
@@ -105,14 +124,16 @@
                         applies a strong gaussian blurring, "solid" draws a
                         solid black box, "none" does leaves the input
                         unchanged and "img" replaces the face with a custom
                         image. Default: "blur".
   --replaceimg REPLACEIMG
                         Anonymization image for face regions. Requires
                         --replacewith img option.
+  --keep-audio, -k      Keep audio from video source file and copy it over to
+                        the output (only applies to videos).
   --ffmpeg-config FFMPEG_CONFIG
                         FFMPEG config arguments for encoding output videos.
                         This argument is expected in JSON notation. For a list
                         of possible options, refer to the ffmpeg-imageio docs.
                         Default: '{"codec": "libx264"}'.
   --backend {auto,onnxrt,opencv}
                         Backend for ONNX model execution. Default: "auto"
@@ -157,15 +178,15 @@
     $ deface examples/city.jpg --draw-scores -o examples/city_anonymized_scores.jpg
 
 <img src="examples/city_anonymized_scores.jpg" width="70%" alt="$ deface examples/city.jpg --draw-scores -o examples/city_anonymized_scores.jpg"/>
 
 This option can be useful to figure out an optimal value for the detection threshold that can then be set through the `--thresh` option.
 
 
-### High-resolution media and performance issues 
+### High-resolution media and performance issues
 
 Since `deface` tries to detect faces in the unscaled full-res version of input files by default, this can lead to performance issues on high-res inputs (>> 720p). In extreme cases, even detection accuracy can suffer because the detector neural network has not been trained on ultra-high-res images.
 
 To counter these performance issues, `deface` supports downsampling its inputs on-the-fly before detecting faces, and subsequently rescaling detection results to the original resolution. Downsampling only applies to the detection process, whereas the final output resolution remains the same as the input resolution.
 
 This feature is controlled through the `--scale` option, which expects a value of the form `WxH`, where `W` and `H` are the desired width and height of downscaled input representations.
 It is very important to make sure the aspect ratio of the inputs remains intact when using this option, because otherwise, distorted images are fed into the detector, resulting in decreased accuracy.
@@ -202,9 +223,7 @@
 
 
 ## Credits
 
 - `centerface.onnx` (original) and `centerface.py` (modified) are based on https://github.com/Star-Clouds/centerface (revision [8c39a49](https://github.com/Star-Clouds/CenterFace/tree/8c39a497afb78fb2c064eb84bf010c273bb7d3ce)),
   [released under MIT license](https://github.com/Star-Clouds/CenterFace/blob/36afed/LICENSE).
 - The original source of the example images in the `examples` directory can be found [here](https://www.pexels.com/de-de/foto/stadt-kreuzung-strasse-menschen-109919/) (released under the [Pexels photo license](https://www.pexels.com/photo-license/)).
-
-
```

### Comparing `deface-1.2.0/README.md` & `deface-1.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # `deface`: Video anonymization by face detection
 
 `deface` is a simple command-line tool for automatic anonymization of faces in videos or photos.
 It works by first detecting all human faces in each video frame and then applying an anonymization filter (blurring or black boxes) on each detected face region.
-All audio tracks are discarded as well.
+By default all audio tracks are discarded as well.
 
 
 Original frame | `deface` output (using default options)
 :--:|:--:
 ![examples/city.jpg](examples/city.jpg) | ![$ deface examples/city.jpg](examples/city_anonymized.jpg)
 
 
@@ -51,16 +51,16 @@
 
 The output may vary depending on your installed version, but it should look similar to this:
 
 ```
 usage: deface [--output O] [--thresh T] [--scale WxH] [--preview] [--boxes]
               [--draw-scores] [--mask-scale M]
               [--replacewith {blur,solid,none,img}] [--replaceimg REPLACEIMG]
-              [--ffmpeg-config FFMPEG_CONFIG] [--backend {auto,onnxrt,opencv}]
-              [--version] [--help]
+              [--keep-audio] [--ffmpeg-config FFMPEG_CONFIG]
+              [--backend {auto,onnxrt,opencv}] [--version] [--help]
               [input ...]
 
 Video anonymization by face detection
 
 positional arguments:
   input                 File path(s) or camera device name. It is possible to
                         pass multiple paths by separating them by spaces or by
@@ -88,14 +88,16 @@
                         applies a strong gaussian blurring, "solid" draws a
                         solid black box, "none" does leaves the input
                         unchanged and "img" replaces the face with a custom
                         image. Default: "blur".
   --replaceimg REPLACEIMG
                         Anonymization image for face regions. Requires
                         --replacewith img option.
+  --keep-audio, -k      Keep audio from video source file and copy it over to
+                        the output (only applies to videos).
   --ffmpeg-config FFMPEG_CONFIG
                         FFMPEG config arguments for encoding output videos.
                         This argument is expected in JSON notation. For a list
                         of possible options, refer to the ffmpeg-imageio docs.
                         Default: '{"codec": "libx264"}'.
   --backend {auto,onnxrt,opencv}
                         Backend for ONNX model execution. Default: "auto"
@@ -140,15 +142,15 @@
     $ deface examples/city.jpg --draw-scores -o examples/city_anonymized_scores.jpg
 
 <img src="examples/city_anonymized_scores.jpg" width="70%" alt="$ deface examples/city.jpg --draw-scores -o examples/city_anonymized_scores.jpg"/>
 
 This option can be useful to figure out an optimal value for the detection threshold that can then be set through the `--thresh` option.
 
 
-### High-resolution media and performance issues 
+### High-resolution media and performance issues
 
 Since `deface` tries to detect faces in the unscaled full-res version of input files by default, this can lead to performance issues on high-res inputs (>> 720p). In extreme cases, even detection accuracy can suffer because the detector neural network has not been trained on ultra-high-res images.
 
 To counter these performance issues, `deface` supports downsampling its inputs on-the-fly before detecting faces, and subsequently rescaling detection results to the original resolution. Downsampling only applies to the detection process, whereas the final output resolution remains the same as the input resolution.
 
 This feature is controlled through the `--scale` option, which expects a value of the form `WxH`, where `W` and `H` are the desired width and height of downscaled input representations.
 It is very important to make sure the aspect ratio of the inputs remains intact when using this option, because otherwise, distorted images are fed into the detector, resulting in decreased accuracy.
```

### Comparing `deface-1.2.0/deface/centerface.onnx` & `deface-1.3.0/deface/centerface.onnx`

 * *Files identical despite different names*

### Comparing `deface-1.2.0/deface/centerface.py` & `deface-1.3.0/deface/centerface.py`

 * *Files identical despite different names*

### Comparing `deface-1.2.0/deface/deface.py` & `deface-1.3.0/deface/deface.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import skimage.draw
 import numpy as np
 import imageio
 import imageio.plugins.ffmpeg
 import cv2
 
 from deface import __version__
+# __version__ = 'a'
 from deface.centerface import CenterFace
 
 
 # TODO: Optionally preserve audio track?
 
 
 def scale_bb(x1, y1, x2, y2, mask_scale=1.0):
@@ -107,15 +108,16 @@
         cam: bool,
         nested: bool,
         replacewith: str,
         mask_scale: float,
         ellipse: bool,
         draw_scores: bool,
         ffmpeg_config: Dict[str, str],
-        replaceimg = None
+        replaceimg = None,
+        keep_audio: bool = False,
 ):
     try:
         if 'fps' in ffmpeg_config:
             reader: imageio.plugins.ffmpeg.FfmpegFormat.Reader = imageio.get_reader(ipath, fps=ffmpeg_config['fps'])
         else:
             reader: imageio.plugins.ffmpeg.FfmpegFormat.Reader = imageio.get_reader(ipath)
 
@@ -137,17 +139,19 @@
     if nested:
         bar = tqdm.tqdm(dynamic_ncols=True, total=nframes, position=1, leave=True)
     else:
         bar = tqdm.tqdm(dynamic_ncols=True, total=nframes)
 
     if opath is not None:
         _ffmpeg_config = ffmpeg_config.copy()
-        if not 'fps' in _ffmpeg_config:
-            #  If fps is not explicitly set in ffmpeg_config, use source video fps value
-            _ffmpeg_config['fps'] = meta['fps']
+        #  If fps is not explicitly set in ffmpeg_config, use source video fps value
+        _ffmpeg_config.setdefault('fps', meta['fps'])
+        if keep_audio:  # Carry over audio from input path, use "copy" codec (no transcoding) by default
+            _ffmpeg_config.setdefault('audio_path', ipath)
+            _ffmpeg_config.setdefault('audio_codec', 'copy')
         writer: imageio.plugins.ffmpeg.FfmpegFormat.Writer = imageio.get_writer(
             opath, format='FFMPEG', mode='I', **_ffmpeg_config
         )
 
     for frame in read_iter:
         # Perform network inference, get bb dets but discard landmark predictions
         dets, _ = centerface(frame, threshold=threshold)
@@ -274,14 +278,17 @@
     parser.add_argument(
         '--replacewith', default='blur', choices=['blur', 'solid', 'none', 'img'],
         help='Anonymization filter mode for face regions. "blur" applies a strong gaussian blurring, "solid" draws a solid black box, "none" does leaves the input unchanged and "img" replaces the face with a custom image. Default: "blur".')
     parser.add_argument(
         '--replaceimg', default='replace_img.png',
         help='Anonymization image for face regions. Requires --replacewith img option.')
     parser.add_argument(
+        '--keep-audio', '-k', default=False, action='store_true',
+        help='Keep audio from video source file and copy it over to the output (only applies to videos).')
+    parser.add_argument(
         '--ffmpeg-config', default={"codec": "libx264"}, type=json.loads,
         help='FFMPEG config arguments for encoding output videos. This argument is expected in JSON notation. For a list of possible options, refer to the ffmpeg-imageio docs. Default: \'{"codec": "libx264"}\'.'
     )  # See https://imageio.readthedocs.io/en/stable/format_ffmpeg.html#parameters-for-saving
     parser.add_argument(
         '--backend', default='auto', choices=['auto', 'onnxrt', 'opencv'],
         help='Backend for ONNX model execution. Default: "auto" (prefer onnxrt if available).')
     parser.add_argument(
@@ -320,14 +327,15 @@
     base_opath = args.output
     replacewith = args.replacewith
     enable_preview = args.preview
     draw_scores = args.draw_scores
     threshold = args.thresh
     ellipse = not args.boxes
     mask_scale = args.mask_scale
+    keep_audio = args.keep_audio
     ffmpeg_config = args.ffmpeg_config
     backend = args.backend
     in_shape = args.scale
     replaceimg = None
     if in_shape is not None:
         w, h = in_shape.split('x')
         in_shape = int(w), int(h)
@@ -365,14 +373,15 @@
                 cam=is_cam,
                 replacewith=replacewith,
                 mask_scale=mask_scale,
                 ellipse=ellipse,
                 draw_scores=draw_scores,
                 enable_preview=enable_preview,
                 nested=multi_file,
+                keep_audio=keep_audio,
                 ffmpeg_config=ffmpeg_config,
                 replaceimg=replaceimg
             )
         elif filetype == 'image':
             image_detect(
                 ipath=ipath,
                 opath=opath,
```

### Comparing `deface-1.2.0/deface.egg-info/PKG-INFO` & `deface-1.3.0/deface.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,48 @@
 Metadata-Version: 2.1
 Name: deface
-Version: 1.2.0
+Version: 1.3.0
 Summary: Video anonymization by face detection
-Home-page: https://github.com/ORB-HD/deface
-Author: Martin Drawitsch
-Author-email: martin.drawitsch@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
+License: MIT License
+        
+        Copyright (c) 2020 Martin Drawitsch
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: repository, https://github.com/ORB-HD/deface
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Classifier: Topic :: Scientific/Engineering :: Image Recognition
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
 License-File: LICENSE
 
 # `deface`: Video anonymization by face detection
 
 `deface` is a simple command-line tool for automatic anonymization of faces in videos or photos.
 It works by first detecting all human faces in each video frame and then applying an anonymization filter (blurring or black boxes) on each detected face region.
-All audio tracks are discarded as well.
+By default all audio tracks are discarded as well.
 
 
 Original frame | `deface` output (using default options)
 :--:|:--:
 ![examples/city.jpg](examples/city.jpg) | ![$ deface examples/city.jpg](examples/city_anonymized.jpg)
 
 
@@ -68,16 +87,16 @@
 
 The output may vary depending on your installed version, but it should look similar to this:
 
 ```
 usage: deface [--output O] [--thresh T] [--scale WxH] [--preview] [--boxes]
               [--draw-scores] [--mask-scale M]
               [--replacewith {blur,solid,none,img}] [--replaceimg REPLACEIMG]
-              [--ffmpeg-config FFMPEG_CONFIG] [--backend {auto,onnxrt,opencv}]
-              [--version] [--help]
+              [--keep-audio] [--ffmpeg-config FFMPEG_CONFIG]
+              [--backend {auto,onnxrt,opencv}] [--version] [--help]
               [input ...]
 
 Video anonymization by face detection
 
 positional arguments:
   input                 File path(s) or camera device name. It is possible to
                         pass multiple paths by separating them by spaces or by
@@ -105,14 +124,16 @@
                         applies a strong gaussian blurring, "solid" draws a
                         solid black box, "none" does leaves the input
                         unchanged and "img" replaces the face with a custom
                         image. Default: "blur".
   --replaceimg REPLACEIMG
                         Anonymization image for face regions. Requires
                         --replacewith img option.
+  --keep-audio, -k      Keep audio from video source file and copy it over to
+                        the output (only applies to videos).
   --ffmpeg-config FFMPEG_CONFIG
                         FFMPEG config arguments for encoding output videos.
                         This argument is expected in JSON notation. For a list
                         of possible options, refer to the ffmpeg-imageio docs.
                         Default: '{"codec": "libx264"}'.
   --backend {auto,onnxrt,opencv}
                         Backend for ONNX model execution. Default: "auto"
@@ -157,15 +178,15 @@
     $ deface examples/city.jpg --draw-scores -o examples/city_anonymized_scores.jpg
 
 <img src="examples/city_anonymized_scores.jpg" width="70%" alt="$ deface examples/city.jpg --draw-scores -o examples/city_anonymized_scores.jpg"/>
 
 This option can be useful to figure out an optimal value for the detection threshold that can then be set through the `--thresh` option.
 
 
-### High-resolution media and performance issues 
+### High-resolution media and performance issues
 
 Since `deface` tries to detect faces in the unscaled full-res version of input files by default, this can lead to performance issues on high-res inputs (>> 720p). In extreme cases, even detection accuracy can suffer because the detector neural network has not been trained on ultra-high-res images.
 
 To counter these performance issues, `deface` supports downsampling its inputs on-the-fly before detecting faces, and subsequently rescaling detection results to the original resolution. Downsampling only applies to the detection process, whereas the final output resolution remains the same as the input resolution.
 
 This feature is controlled through the `--scale` option, which expects a value of the form `WxH`, where `W` and `H` are the desired width and height of downscaled input representations.
 It is very important to make sure the aspect ratio of the inputs remains intact when using this option, because otherwise, distorted images are fed into the detector, resulting in decreased accuracy.
@@ -202,9 +223,7 @@
 
 
 ## Credits
 
 - `centerface.onnx` (original) and `centerface.py` (modified) are based on https://github.com/Star-Clouds/centerface (revision [8c39a49](https://github.com/Star-Clouds/CenterFace/tree/8c39a497afb78fb2c064eb84bf010c273bb7d3ce)),
   [released under MIT license](https://github.com/Star-Clouds/CenterFace/blob/36afed/LICENSE).
 - The original source of the example images in the `examples` directory can be found [here](https://www.pexels.com/de-de/foto/stadt-kreuzung-strasse-menschen-109919/) (released under the [Pexels photo license](https://www.pexels.com/photo-license/)).
-
-
```

