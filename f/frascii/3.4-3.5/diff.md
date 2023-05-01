# Comparing `tmp/frascii-3.4.tar.gz` & `tmp/frascii-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frascii-3.4.tar", last modified: Sat Apr 29 14:54:00 2023, max compression
+gzip compressed data, was "frascii-3.5.tar", last modified: Mon May  1 12:51:01 2023, max compression
```

## Comparing `frascii-3.4.tar` & `frascii-3.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-29 14:54:00.010015 frascii-3.4/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    14887 2023-04-29 14:54:00.014015 frascii-3.4/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    12821 2023-04-29 14:53:52.000000 frascii-3.4/README.md
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-29 14:54:00.010015 frascii-3.4/frascii/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2134 2023-04-29 14:53:28.000000 frascii-3.4/frascii/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     7913 2023-04-29 14:51:12.000000 frascii-3.4/frascii/commands.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-29 14:54:00.010015 frascii-3.4/frascii/fractals/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        0 2023-02-24 11:27:22.000000 frascii-3.4/frascii/fractals/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      306 2023-03-03 18:15:44.000000 frascii-3.4/frascii/fractals/cantor.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2224 2023-02-28 08:13:57.000000 frascii-3.4/frascii/fractals/dragon_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1263 2023-03-03 18:15:51.000000 frascii-3.4/frascii/fractals/fibonacci.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1816 2023-02-28 08:12:17.000000 frascii-3.4/frascii/fractals/hilbert_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3880 2023-04-26 12:53:36.000000 frascii-3.4/frascii/fractals/julia.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2078 2023-03-01 08:32:48.000000 frascii-3.4/frascii/fractals/koch.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     4110 2023-04-29 14:01:04.000000 frascii-3.4/frascii/fractals/l_system.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3707 2023-04-29 13:56:22.000000 frascii-3.4/frascii/fractals/mandelbrot.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2072 2023-02-26 23:51:55.000000 frascii-3.4/frascii/fractals/peano_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      553 2023-02-24 11:50:58.000000 frascii-3.4/frascii/fractals/sierpinski_carpet.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      395 2023-02-28 09:01:32.000000 frascii-3.4/frascii/fractals/sierpinski_triangle.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      494 2023-02-28 14:05:15.000000 frascii-3.4/frascii/fractals/vicsek.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-29 14:54:00.010015 frascii-3.4/frascii.egg-info/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    14887 2023-04-29 14:53:59.000000 frascii-3.4/frascii.egg-info/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      627 2023-04-29 14:54:00.000000 frascii-3.4/frascii.egg-info/SOURCES.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2023-04-29 14:53:59.000000 frascii-3.4/frascii.egg-info/dependency_links.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       55 2023-04-29 14:53:59.000000 frascii-3.4/frascii.egg-info/entry_points.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        8 2023-04-29 14:53:59.000000 frascii-3.4/frascii.egg-info/top_level.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       79 2023-04-29 14:54:00.014015 frascii-3.4/setup.cfg
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      572 2023-04-26 07:39:57.000000 frascii-3.4/setup.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-05-01 12:51:01.763646 frascii-3.5/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    15094 2023-05-01 12:51:01.763646 frascii-3.5/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    12996 2023-05-01 12:49:20.000000 frascii-3.5/README.md
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-05-01 12:51:01.759646 frascii-3.5/frascii/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2134 2023-05-01 12:50:42.000000 frascii-3.5/frascii/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     7940 2023-05-01 12:48:57.000000 frascii-3.5/frascii/commands.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-05-01 12:51:01.763646 frascii-3.5/frascii/fractals/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        0 2023-02-24 11:27:22.000000 frascii-3.5/frascii/fractals/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      306 2023-03-03 18:15:44.000000 frascii-3.5/frascii/fractals/cantor.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2224 2023-02-28 08:13:57.000000 frascii-3.5/frascii/fractals/dragon_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1263 2023-03-03 18:15:51.000000 frascii-3.5/frascii/fractals/fibonacci.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1816 2023-02-28 08:12:17.000000 frascii-3.5/frascii/fractals/hilbert_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3880 2023-04-26 12:53:36.000000 frascii-3.5/frascii/fractals/julia.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2078 2023-03-01 08:32:48.000000 frascii-3.5/frascii/fractals/koch.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     4110 2023-04-29 14:01:04.000000 frascii-3.5/frascii/fractals/l_system.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3707 2023-04-29 13:56:22.000000 frascii-3.5/frascii/fractals/mandelbrot.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2072 2023-02-26 23:51:55.000000 frascii-3.5/frascii/fractals/peano_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      553 2023-02-24 11:50:58.000000 frascii-3.5/frascii/fractals/sierpinski_carpet.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      395 2023-02-28 09:01:32.000000 frascii-3.5/frascii/fractals/sierpinski_triangle.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      494 2023-02-28 14:05:15.000000 frascii-3.5/frascii/fractals/vicsek.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-05-01 12:51:01.759646 frascii-3.5/frascii.egg-info/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    15094 2023-05-01 12:51:01.000000 frascii-3.5/frascii.egg-info/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      627 2023-05-01 12:51:01.000000 frascii-3.5/frascii.egg-info/SOURCES.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2023-05-01 12:51:01.000000 frascii-3.5/frascii.egg-info/dependency_links.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       55 2023-05-01 12:51:01.000000 frascii-3.5/frascii.egg-info/entry_points.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        8 2023-05-01 12:51:01.000000 frascii-3.5/frascii.egg-info/top_level.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       79 2023-05-01 12:51:01.763646 frascii-3.5/setup.cfg
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1377 2023-05-01 12:49:50.000000 frascii-3.5/setup.py
```

### Comparing `frascii-3.4/PKG-INFO` & `frascii-3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frascii
-Version: 3.4
+Version: 3.5
 Summary: UNKNOWN
 Home-page: https://github.com/LuggiStruggi/Frascii.git
 Author: Lukas König
 Author-email: lukasmkoenig@gmx.net
 License: UNKNOWN
 Description: # Frascii
         ASCII-visualizations of Fractals for the Ubuntu (or other) Terminal
@@ -49,15 +49,15 @@
         
         `frascii mandelbrot -x_radius 400 -y_radius 180 -stepsize 0.0033 -style repeating`
         
         ![Mandelbrot set in terminal by frascii](readme_images/repeating.png)
         
         `frascii mandelbrot -x_radius 300 -y_radius 300 -explore`
         
-        ![Mandelbrot set in terminal by frascii](readme_images/explore.gif)
+        ![Mandelbrot set in terminal by frascii](readme_images/zoom.gif)
         
         `frascii mandelbrot -x -1.15 -y 0.26 -x_radius 200 -y_radius 70 -stepsize 3.7e-4 -max_iter 60`
         
         ![Mandelbrot set in terminal by frascii](readme_images/mandelbrot2.png)
         
         `frascii mandelbrot`
         
@@ -215,14 +215,18 @@
                                     └─┘ │ ┌─┘                     
                                         └─┘                       
         ```
         
         
         `frascii l_system -start "A" -rules "(A->+BF-AFA-FB+),(B->-AF+BFB+FA-)" -n 4 -direction R` leads to a **Hilbert Curve**.
         
+        `frascii l_system -start "A" -rules "(A->+BF-AFA-FB+),(B->-AF+BFB+FA-)" -n 4 -direction R -animate`
+        
+        ![Hilbert curve in terminal by frascii](readme_images/hilbert_animated.gif)
+        
         `frascii l_system -start "FX" -rules "(X->X+YF+),(Y->-FX-Y)" -n 10 -direction U` leads to a **Dragon Curve**.
         
         `frascii l_system -start Y -rules "(Y->YZ-Z-Z-ZA--),(X->XZ),(Z->XF),(A->Z)" -n 6` leads to **Fibonacci Squares**.
         
         
         # Tip for better visualization
```

### Comparing `frascii-3.4/README.md` & `frascii-3.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 `frascii mandelbrot -x_radius 400 -y_radius 180 -stepsize 0.0033 -style repeating`
 
 ![Mandelbrot set in terminal by frascii](readme_images/repeating.png)
 
 `frascii mandelbrot -x_radius 300 -y_radius 300 -explore`
 
-![Mandelbrot set in terminal by frascii](readme_images/explore.gif)
+![Mandelbrot set in terminal by frascii](readme_images/zoom.gif)
 
 `frascii mandelbrot -x -1.15 -y 0.26 -x_radius 200 -y_radius 70 -stepsize 3.7e-4 -max_iter 60`
 
 ![Mandelbrot set in terminal by frascii](readme_images/mandelbrot2.png)
 
 `frascii mandelbrot`
 
@@ -207,14 +207,18 @@
                             └─┘ │ ┌─┘                     
                                 └─┘                       
 ```
 
 
 `frascii l_system -start "A" -rules "(A->+BF-AFA-FB+),(B->-AF+BFB+FA-)" -n 4 -direction R` leads to a **Hilbert Curve**.
 
+`frascii l_system -start "A" -rules "(A->+BF-AFA-FB+),(B->-AF+BFB+FA-)" -n 4 -direction R -animate`
+
+![Hilbert curve in terminal by frascii](readme_images/hilbert_animated.gif)
+
 `frascii l_system -start "FX" -rules "(X->X+YF+),(Y->-FX-Y)" -n 10 -direction U` leads to a **Dragon Curve**.
 
 `frascii l_system -start Y -rules "(Y->YZ-Z-Z-ZA--),(X->XZ),(Z->XF),(A->Z)" -n 6` leads to **Fibonacci Squares**.
 
 
 # Tip for better visualization
```

### Comparing `frascii-3.4/frascii/__init__.py` & `frascii-3.5/frascii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from frascii.fractals.vicsek import vicsek_string
 from frascii.fractals.hilbert_curve import hilbert_curve_string
 from frascii.fractals.peano_curve import peano_curve_string
 from frascii.fractals.dragon_curve import dragon_curve_string
 from frascii.fractals.fibonacci import fibonacci_string
 from frascii.fractals.l_system import l_system_string, l_system_animate
 
-__version__ = '3.4'
+__version__ = '3.5'
 
 def mandelbrot(x, y, x_radius, y_radius, stepsize, max_iter, style, grid, explore):
 	if explore:
 		x, y, x_radius, y_radius, stepsize, max_iter, style, grid = mandelbrot_explore(x, y, x_radius, y_radius, stepsize, max_iter, style, grid)
 	return mandelbrot_string(x, y, x_radius, y_radius, stepsize, max_iter, style, grid)
 
 def julia(f, x, y, x_radius, y_radius, stepsize, max_iter, style, grid, explore):
```

### Comparing `frascii-3.4/frascii/commands.py` & `frascii-3.5/frascii/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,19 +88,19 @@
 																 " Use ',' and '.' to change the amount of iteratios. Use '-' to change style."
 																 " Exit with ESC or 'x'."),
 							  action="store_true")
 	julia_parser.set_defaults(func=frascii.julia)
 
 	# L-system sub-command
 	l_system_parser = subparsers.add_parser("l_system", description="Wikipedia: https://en.wikipedia.org/wiki/L-system", formatter_class=fc)
-	l_system_parser.add_argument("-start", type=str, help="real part of the images center", nargs="?", default="F")
-	l_system_parser.add_argument("-rules", type=str, help="imaginary part of the images center", nargs="?", default="(F->F+F-F-F+F)")
-	l_system_parser.add_argument("-n", type=int, help="pixels added on left and right of center", nargs="?", default=3)
-	l_system_parser.add_argument("-direction", type=str, help="pixels added on top and bottom of center", choices=["U", "R", "D", "L"], nargs="?", default="U")
-	l_system_parser.add_argument("-animate", type=float, help="if set scene is animated with chosen delay between frames.", nargs="?", default=-1)
+	l_system_parser.add_argument("-start", type=str, help="Axiom/Starting state of the L-system", nargs="?", default="F")
+	l_system_parser.add_argument("-rules", type=str, help="The rules of the system. Should look like '(*->***),(*->***)'", nargs="?", default="(F->F+F-F-F+F)")
+	l_system_parser.add_argument("-n", type=int, help="Amount of iterations", nargs="?", default=3)
+	l_system_parser.add_argument("-direction", type=str, help="Initial direction: up, right left or down.", choices=["U", "R", "D", "L"], nargs="?", default="U")
+	l_system_parser.add_argument("-animate", type=float, help="to animate the drawing process. Time delay between frames can be given.", nargs="?", default=-1)
 	l_system_parser.set_defaults(func=frascii.l_system)
 
 
 	args = parser.parse_args()
 	if args.subcommand == None:
 		parser.print_help()
 		parser.exit()
```

### Comparing `frascii-3.4/frascii/fractals/dragon_curve.py` & `frascii-3.5/frascii/fractals/dragon_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-3.4/frascii/fractals/fibonacci.py` & `frascii-3.5/frascii/fractals/fibonacci.py`

 * *Files identical despite different names*

### Comparing `frascii-3.4/frascii/fractals/hilbert_curve.py` & `frascii-3.5/frascii/fractals/hilbert_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-3.4/frascii/fractals/julia.py` & `frascii-3.5/frascii/fractals/julia.py`

 * *Files identical despite different names*

### Comparing `frascii-3.4/frascii/fractals/koch.py` & `frascii-3.5/frascii/fractals/koch.py`

 * *Files identical despite different names*

### Comparing `frascii-3.4/frascii/fractals/l_system.py` & `frascii-3.5/frascii/fractals/l_system.py`

 * *Files identical despite different names*

### Comparing `frascii-3.4/frascii/fractals/mandelbrot.py` & `frascii-3.5/frascii/fractals/mandelbrot.py`

 * *Files identical despite different names*

### Comparing `frascii-3.4/frascii/fractals/peano_curve.py` & `frascii-3.5/frascii/fractals/peano_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-3.4/frascii/fractals/sierpinski_carpet.py` & `frascii-3.5/frascii/fractals/sierpinski_carpet.py`

 * *Files identical despite different names*

### Comparing `frascii-3.4/frascii.egg-info/PKG-INFO` & `frascii-3.5/frascii.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frascii
-Version: 3.4
+Version: 3.5
 Summary: UNKNOWN
 Home-page: https://github.com/LuggiStruggi/Frascii.git
 Author: Lukas König
 Author-email: lukasmkoenig@gmx.net
 License: UNKNOWN
 Description: # Frascii
         ASCII-visualizations of Fractals for the Ubuntu (or other) Terminal
@@ -49,15 +49,15 @@
         
         `frascii mandelbrot -x_radius 400 -y_radius 180 -stepsize 0.0033 -style repeating`
         
         ![Mandelbrot set in terminal by frascii](readme_images/repeating.png)
         
         `frascii mandelbrot -x_radius 300 -y_radius 300 -explore`
         
-        ![Mandelbrot set in terminal by frascii](readme_images/explore.gif)
+        ![Mandelbrot set in terminal by frascii](readme_images/zoom.gif)
         
         `frascii mandelbrot -x -1.15 -y 0.26 -x_radius 200 -y_radius 70 -stepsize 3.7e-4 -max_iter 60`
         
         ![Mandelbrot set in terminal by frascii](readme_images/mandelbrot2.png)
         
         `frascii mandelbrot`
         
@@ -215,14 +215,18 @@
                                     └─┘ │ ┌─┘                     
                                         └─┘                       
         ```
         
         
         `frascii l_system -start "A" -rules "(A->+BF-AFA-FB+),(B->-AF+BFB+FA-)" -n 4 -direction R` leads to a **Hilbert Curve**.
         
+        `frascii l_system -start "A" -rules "(A->+BF-AFA-FB+),(B->-AF+BFB+FA-)" -n 4 -direction R -animate`
+        
+        ![Hilbert curve in terminal by frascii](readme_images/hilbert_animated.gif)
+        
         `frascii l_system -start "FX" -rules "(X->X+YF+),(Y->-FX-Y)" -n 10 -direction U` leads to a **Dragon Curve**.
         
         `frascii l_system -start Y -rules "(Y->YZ-Z-Z-ZA--),(X->XZ),(Z->XF),(A->Z)" -n 6` leads to **Fibonacci Squares**.
         
         
         # Tip for better visualization
```

### Comparing `frascii-3.4/frascii.egg-info/SOURCES.txt` & `frascii-3.5/frascii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

