# Comparing `tmp/lumos-sat-1.0.1.tar.gz` & `tmp/lumos-sat-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumos-sat-1.0.1.tar", last modified: Thu Apr  6 21:43:48 2023, max compression
+gzip compressed data, was "lumos-sat-1.0.2.tar", last modified: Mon May  1 19:13:46 2023, max compression
```

## Comparing `lumos-sat-1.0.1.tar` & `lumos-sat-1.0.2.tar`

### file list

```diff
@@ -1,35 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 21:43:48.525725 lumos-sat-1.0.1/
--rw-rw-rw-   0        0        0     1096 2023-04-06 18:33:06.000000 lumos-sat-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       86 2023-04-06 21:38:28.000000 lumos-sat-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      834 2023-04-06 21:43:48.522734 lumos-sat-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      577 2023-04-06 19:37:58.000000 lumos-sat-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 21:43:48.462893 lumos-sat-1.0.1/lumos/
--rw-rw-rw-   0        0        0        0 2023-04-06 18:42:57.000000 lumos-sat-1.0.1/lumos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 21:43:48.475861 lumos-sat-1.0.1/lumos/brdf/
--rw-rw-rw-   0        0        0        0 2023-04-06 18:51:47.000000 lumos-sat-1.0.1/lumos/brdf/__init__.py
--rw-rw-rw-   0        0        0     2167 2023-04-06 19:00:07.000000 lumos-sat-1.0.1/lumos/brdf/fit_tools.py
--rw-rw-rw-   0        0        0     6493 2023-04-06 19:00:39.000000 lumos-sat-1.0.1/lumos/brdf/library.py
-drwxrwxrwx   0        0        0        0 2023-04-06 21:43:48.481842 lumos-sat-1.0.1/lumos/calculators/
--rw-rw-rw-   0        0        0        0 2023-04-06 18:51:54.000000 lumos-sat-1.0.1/lumos/calculators/__init__.py
--rw-rw-rw-   0        0        0     7743 2023-04-06 18:53:33.000000 lumos-sat-1.0.1/lumos/calculators/brightness_frame.py
--rw-rw-rw-   0        0        0     5378 2023-04-06 18:59:29.000000 lumos-sat-1.0.1/lumos/calculators/ground_frame.py
--rw-rw-rw-   0        0        0      207 2023-04-06 18:47:24.000000 lumos-sat-1.0.1/lumos/constants.py
--rw-rw-rw-   0        0        0     2320 2023-04-06 19:08:51.000000 lumos-sat-1.0.1/lumos/conversions.py
--rw-rw-rw-   0        0        0     2745 2023-04-06 18:49:01.000000 lumos-sat-1.0.1/lumos/functions.py
--rw-rw-rw-   0        0        0     3493 2023-04-06 18:49:21.000000 lumos-sat-1.0.1/lumos/geometry.py
-drwxrwxrwx   0        0        0        0 2023-04-06 21:43:48.498796 lumos-sat-1.0.1/lumos/plot/
--rw-rw-rw-   0        0        0        0 2023-03-10 18:54:08.000000 lumos-sat-1.0.1/lumos/plot/__init__.py
--rw-rw-rw-   0        0        0     1554 2023-04-06 19:19:50.000000 lumos-sat-1.0.1/lumos/plot/brdf.py
--rw-rw-rw-   0        0        0      213 2023-03-12 20:06:33.000000 lumos-sat-1.0.1/lumos/plot/brightness_frame.mplstyle
--rw-rw-rw-   0        0        0     3182 2023-03-14 05:45:11.000000 lumos-sat-1.0.1/lumos/plot/brightness_frame.py
--rw-rw-rw-   0        0        0      421 2023-03-14 05:45:11.000000 lumos-sat-1.0.1/lumos/plot/ground_frame.mplstyle
--rw-rw-rw-   0        0        0     8227 2023-04-06 19:04:28.000000 lumos-sat-1.0.1/lumos/plot/ground_frame.py
--rw-rw-rw-   0        0        0      524 2023-04-06 19:30:32.000000 lumos-sat-1.0.1/lumos/video_tools.py
-drwxrwxrwx   0        0        0        0 2023-04-06 21:43:48.518745 lumos-sat-1.0.1/lumos_sat.egg-info/
--rw-rw-rw-   0        0        0      834 2023-04-06 21:43:48.000000 lumos-sat-1.0.1/lumos_sat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      665 2023-04-06 21:43:48.000000 lumos-sat-1.0.1/lumos_sat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 21:43:48.000000 lumos-sat-1.0.1/lumos_sat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2023-04-06 21:43:48.000000 lumos-sat-1.0.1/lumos_sat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-06 21:43:48.000000 lumos-sat-1.0.1/lumos_sat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      588 2023-04-06 21:43:19.000000 lumos-sat-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-06 21:43:48.525725 lumos-sat-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-01 19:13:46.385365 lumos-sat-1.0.2/
+-rw-rw-rw-   0        0        0     1096 2023-04-06 18:33:06.000000 lumos-sat-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       86 2023-04-06 21:38:28.000000 lumos-sat-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      834 2023-05-01 19:13:46.384367 lumos-sat-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      577 2023-04-06 19:37:58.000000 lumos-sat-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 19:13:46.332508 lumos-sat-1.0.2/lumos/
+-rw-rw-rw-   0        0        0        0 2023-04-06 18:42:57.000000 lumos-sat-1.0.2/lumos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 19:13:46.339488 lumos-sat-1.0.2/lumos/brdf/
+-rw-rw-rw-   0        0        0        0 2023-04-06 18:51:47.000000 lumos-sat-1.0.2/lumos/brdf/__init__.py
+-rw-rw-rw-   0        0        0     2140 2023-05-01 18:30:13.000000 lumos-sat-1.0.2/lumos/brdf/fit_tools.py
+-rw-rw-rw-   0        0        0     6647 2023-05-01 18:23:06.000000 lumos-sat-1.0.2/lumos/brdf/library.py
+drwxrwxrwx   0        0        0        0 2023-05-01 19:13:46.347466 lumos-sat-1.0.2/lumos/calculators/
+-rw-rw-rw-   0        0        0        0 2023-04-06 18:51:54.000000 lumos-sat-1.0.2/lumos/calculators/__init__.py
+-rw-rw-rw-   0        0        0     8082 2023-05-01 18:45:47.000000 lumos-sat-1.0.2/lumos/calculators/brightness_frame.py
+-rw-rw-rw-   0        0        0     5378 2023-04-08 02:44:34.000000 lumos-sat-1.0.2/lumos/calculators/ground_frame.py
+-rw-rw-rw-   0        0        0      340 2023-04-09 01:56:39.000000 lumos-sat-1.0.2/lumos/constants.py
+-rw-rw-rw-   0        0        0     2369 2023-05-01 16:44:37.000000 lumos-sat-1.0.2/lumos/conversions.py
+-rw-rw-rw-   0        0        0     3479 2023-04-09 02:37:52.000000 lumos-sat-1.0.2/lumos/functions.py
+-rw-rw-rw-   0        0        0     3839 2023-05-01 17:04:37.000000 lumos-sat-1.0.2/lumos/geometry.py
+drwxrwxrwx   0        0        0        0 2023-05-01 19:13:46.357439 lumos-sat-1.0.2/lumos/plot/
+-rw-rw-rw-   0        0        0        0 2023-03-10 18:54:08.000000 lumos-sat-1.0.2/lumos/plot/__init__.py
+-rw-rw-rw-   0        0        0     2153 2023-05-01 17:13:16.000000 lumos-sat-1.0.2/lumos/plot/brdf.py
+-rw-rw-rw-   0        0        0     3029 2023-05-01 17:48:10.000000 lumos-sat-1.0.2/lumos/plot/brightness_frame.py
+-rw-rw-rw-   0        0        0     4027 2023-05-01 17:58:04.000000 lumos-sat-1.0.2/lumos/plot/ground_frame.py
+-rw-rw-rw-   0        0        0      955 2023-05-01 17:10:23.000000 lumos-sat-1.0.2/lumos/video_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-01 19:13:46.381376 lumos-sat-1.0.2/lumos_sat.egg-info/
+-rw-rw-rw-   0        0        0      834 2023-05-01 19:13:46.000000 lumos-sat-1.0.2/lumos_sat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      595 2023-05-01 19:13:46.000000 lumos-sat-1.0.2/lumos_sat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 19:13:46.000000 lumos-sat-1.0.2/lumos_sat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      220 2023-05-01 19:13:46.000000 lumos-sat-1.0.2/lumos_sat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-01 19:13:46.000000 lumos-sat-1.0.2/lumos_sat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      588 2023-05-01 18:52:42.000000 lumos-sat-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-01 19:13:46.385365 lumos-sat-1.0.2/setup.cfg
```

### Comparing `lumos-sat-1.0.1/LICENSE` & `lumos-sat-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.1/PKG-INFO` & `lumos-sat-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumos-sat
-Version: 1.0.1
+Version: 1.0.2
 Summary: Satellite Brightness Calculation Tools
 Author-email: Forrest Fankhauser <fafankhauser@ucdavis.edu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lumos-sat
```

### Comparing `lumos-sat-1.0.1/README.md` & `lumos-sat-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.1/lumos/brdf/fit_tools.py` & `lumos-sat-1.0.2/lumos/brdf/fit_tools.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,34 +3,37 @@
 """
 
 import numpy as np
 import scipy.optimize
 import lumos.conversions
 
 def fit_model(
-        data_file : str, 
-        model_func : callable, 
-        p0 : tuple[float, ...], 
-        bounds : tuple[float, ...],
-        log_space : bool = True,
-        clip : float = 1e-4
-        ) -> tuple[float, ...]:
+        data_file,
+        model_func,
+        bounds,
+        p0,
+        log_space = True,
+        clip = 0
+        ):
     
     """
     Fits a model to experimental data.
 
-    Parameters:
-        data_file (str) : File containing experimental data.
-        model_func (callable) : Given parameters *params, returns BRDF callable
-        p0 (tuple) : Initial guess for fitting parameters, passed to scipy.optimize.curve_fit
-        bounds (tuple) : Bounds for fitting parameters, passed to scipy.optimize.curve_fit
-        clip (float) : Clips BRDF data below this value
-    
-    Returns:
-        popt (tuple) : Optimal parameters returned from scipy.optimize.curve_fit
+    :param data_file: A path to a .csv file containing BRDF data. DESCRIBE FORMAT.
+    :type data_file: str
+    :param model_func: A BRDF model to fit
+    :type model_func: function
+    :param bounds: Bounds passed to :function:`scipy.optimize.curve_fit`
+    :type bounds: tuple
+    :param p0: Initial guess for parameters passed to :function:`scipy.optimize.curve_fit`
+    :type p0: tuple
+    :param log_space: Whether or not to fit BRDF in log_space
+    :type log_space: bool
+    :param clip: Removes BRDF data below this cutoff from fitting
+    :type clip: float
     """
 
     data = np.loadtxt(data_file, skiprows = 1)
 
     phi_in = np.deg2rad(data[:, 0])
     theta_in = np.deg2rad(data[:, 1])
     phi_out = np.deg2rad(data[:, 2])
```

### Comparing `lumos-sat-1.0.1/lumos/calculators/brightness_frame.py` & `lumos-sat-1.0.2/lumos/calculators/brightness_frame.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 """
 Intensity calculations in the brightness reference frame.
 """
+
 import numpy as np
 import lumos.constants
 import lumos.geometry
 
-def get_earthshine_panels(sat_z : float, angle_past_terminator : float, density : int) \
-      -> tuple[np.ndarray, ...]:
+def get_earthshine_panels(sat_z, angle_past_terminator, density):
     """
-    Creates mesh of panels on Earth's surface.
+    Creates a mesh of pixels on Earth's surface which are visible to the satellite and illuminated
+    by the sun.
 
-    Parameters:
-        sat_z (float): The height of the satellite above geodetic nadir (meters)
-        angle_past_terminator (float): The angle of the satellite past terminator (radians)
-        density (int): The density of the panels. Grid will have size density x 
-    
-    Returns:
-        x (np.ndarray): x positions of panels (meters)
-        y (np.ndarray): y positions of panels (meters)
-        z (np.ndarray): z positions of panels (meters)
-        nx (np.ndarray): x component of panel normals
-        ny (np.ndarray): y component of panel normals
-        nz (np.ndarray): z component of panel normals
-        areas (np.ndarray): areas of panels (meters ^ 2)
+    :param sat_z: The height of the satellite above the center of Earth (meters)
+    :type sat_z: float
+    :param angle_past_terminator: The angle of the satellite past the terminator (radians)
+    :type angle_past_terminator: float
+    :param density: The density of the pixels. Grid will have size density x density.
+    :type density: int
+    :returns: 
+        - (x, y, z) - Positions of pixels (meters)
+        - (nx, ny, nz) - Normal vectors of pixels
+        - areas - Areas of pixels (:math:`m^2`)
     """
+
     R = lumos.constants.EARTH_RADIUS
 
     max_angle = np.arccos(R / sat_z)
 
     angles_off_plane = np.linspace(-max_angle, max_angle, density)
     angles_on_plane = np.linspace(angle_past_terminator, max_angle, density)
 
@@ -70,51 +69,62 @@
         dy_dr * (dx_dphi * dz_dtheta - dx_dtheta * dz_dphi) +
         dz_dr * (dx_dphi * dy_dtheta - dx_dtheta * dy_dphi) )
     
     areas = determinant * d_phi * d_theta
     
     return x, y, z, nx, ny, nz, areas
 
-def calculate_intensity(sat_surfaces : list[lumos.geometry.Surface], 
-                        sat_altitude : float, 
-                        angle_past_terminator : float,
-                        observer_position : float,
-                        include_sun : bool = True, 
-                        include_earthshine : bool = True,
-                        earth_panel_density : int = 150, 
-                        earth_brdf : callable = None) -> float:
+def calculate_intensity(
+    sat_surfaces, 
+    sat_height, 
+    angle_past_terminator,
+    observer_position,
+    include_sun = True, 
+    include_earthshine = True,
+    earth_panel_density = 150, 
+    earth_brdf = None):
     '''
-        Parameters:
-            sat_surfaces (list[lumos.geometry.Surface]) : A list of lumos.geometry.general.Surface objects
-            sat_altitude (float) : Height of satellite above geodetic nadir (meters)
-            angle_past_terminator (float) : Angle of satellite past terminator (radians)
-            include_sun (bool) : Whether to include brightness directly reflected from sun
-            include_earthshine (bool) : Whether to include brightness caused by earthshine
-            earth_panel_density (int) : There will be earth_panel_density^2 panels in the earthshine mesh
-            earth_brdf (callable) : A function representing the BRDF of earth
-        
-        Returns:
-            intensity (float) : The intensity of light incident on the observer (W / m^2)
+    Calculates flux scattered by a satellite and seen by an observer.
+
+    :param sat_surfaces: List of surfaces on satellite
+    :type sat_surfaces: list[lumos.geometry.Surface]
+    :param sat_height: Height of satellite above geodetic nadir (meters)
+    :type sat_height: float
+    :param angle_past_terminator: Angle of satellite past terminator (radians)
+    :type angle_past_terminator: float
+    :param observer_position: Position of an observer, measured in brightness frame (meters)
+    :type observer_position: :class:`np.ndarray`
+    :param include_sun: Whether to include flux scattered by the satellite from the sun
+    :type include_sun: bool, optional
+    :param include_earthshine: Whether to include flux scattered by the satellite from earthshine
+    :type include_earthshine: bool, optional
+    :param earth_panel_density: There will be earth_panel_density x earth_panel_density 
+    panels in the earthshine mesh
+    :type earth_panel_density: int
+    :param earth_brdf: A function representing the BRDF of Earth's surface
+    :type earth_brdf: function
+    :return: Flux of light incident on the observer (W / m^2)
+    :rtype: float
     '''
     
-    horizon_angle = np.arccos(lumos.constants.EARTH_RADIUS / (lumos.constants.EARTH_RADIUS + sat_altitude))
+    horizon_angle = np.arccos(lumos.constants.EARTH_RADIUS / (lumos.constants.EARTH_RADIUS + sat_height))
     if angle_past_terminator > horizon_angle:
         # Inside earth's shadow
         return 0
     
     observer_x, observer_y, observer_z = observer_position[0], observer_position[1], observer_position[2]
 
     if np.arccos(observer_z / lumos.constants.EARTH_RADIUS) > horizon_angle + np.deg2rad(1):
         # Not visible to observer
         # Fudging this by 1 degree makes plots much nicer on edges
         return 0
 
     vector_2_sun = (0, np.cos(angle_past_terminator), - np.sin(angle_past_terminator))
 
-    sat_z = sat_altitude + lumos.constants.EARTH_RADIUS
+    sat_z = sat_height + lumos.constants.EARTH_RADIUS
 
     # Distances from observers to satellite
     dist_sat_2_obs = np.sqrt( observer_x**2 + observer_y**2 
                             + (observer_z - sat_z)**2 )
     
     # Unit vectors from observers to satellite
     sat_obs_x = observer_x / dist_sat_2_obs
@@ -140,36 +150,42 @@
                                 (panel_sat_x, panel_sat_y, panel_sat_z))
 
     intensity = 0
 
     for surface in sat_surfaces:
         
         if callable(surface.normal):
-            surface.normal = surface.normal(angle_past_terminator)
+            surface_normal = surface.normal(angle_past_terminator)
+        else:
+            surface_normal = surface.normal
         
         sun_contribution = 0
         earth_contribution = 0
         
-        surface_normalization = surface.normal[1] * vector_2_sun[1] + surface.normal[2] * vector_2_sun[2]
+        surface_normalization = surface_normal[1] * vector_2_sun[1] + surface_normal[2] * vector_2_sun[2]
+        surface_normalization = np.clip(surface_normalization, 0, None)
+
+        observer_normalization = surface_normal[0] * sat_obs_x + surface_normal[1] * sat_obs_y + surface_normal[2] * sat_obs_z
+        observer_normalization = np.clip(observer_normalization, 0, None)
 
         if include_sun:
             surface_brdf = surface.brdf(vector_2_sun,
-                                                surface.normal,
-                                                (sat_obs_x, sat_obs_y, sat_obs_z))
+                                        surface_normal,
+                                        (sat_obs_x, sat_obs_y, sat_obs_z))
 
-            sun_contribution = sun_contribution + surface_brdf * surface_normalization
+            sun_contribution = sun_contribution + surface_brdf * surface_normalization * observer_normalization
 
         if include_earthshine:
-            surface_normalizations = -( surface.normal[0] * panel_sat_x 
-                             + surface.normal[1] * panel_sat_y
-                             + surface.normal[2] * panel_sat_z)
+            surface_normalizations = np.clip( surface_normal[0] * panel_sat_x 
+                             + surface_normal[1] * panel_sat_y
+                             + surface_normal[2] * panel_sat_z, 0, None)**2
 
             surface_brdf = surface.brdf( (-panel_sat_x, -panel_sat_y, -panel_sat_z),
-                                                   surface.normal,
-                                                   (sat_obs_x, sat_obs_y, sat_obs_z) )
+                                          surface_normal,
+                                         (sat_obs_x, sat_obs_y, sat_obs_z) )
             
             earth_contribution = earth_contribution \
                   + np.sum(panel_brdfs * surface_brdf 
                          * panel_normalizations * surface_normalizations
                          * panel_areas / dist_panels_2_sat**2 )
         
         intensity = intensity + lumos.constants.SUN_INTENSITY * surface.area * (sun_contribution + earth_contribution) / dist_sat_2_obs ** 2
```

### Comparing `lumos-sat-1.0.1/lumos/calculators/ground_frame.py` & `lumos-sat-1.0.2/lumos/calculators/ground_frame.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.1/lumos/conversions.py` & `lumos-sat-1.0.2/lumos/conversions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,78 @@
 """ Conversions which are used throughout Lumos """
 
 import numpy as np
 import lumos.constants
 import lumos.functions
 
-def intensity_to_ab_mag(intensity : float | np.ndarray, clip : bool = True) -> float | np.ndarray:
+def intensity_to_ab_mag(intensity, clip = True):
     """
-    Converts intensity to AB Magnitude
+    Converts from intensity to AB Magnitude.
+    If clip is set to True, outputs below 12 AB Magnitude will be clipped.
 
-    Parameters:
-        intensity (np.ndarray or float) : Intensity measured in watts / meter^2
-    
-    Returns:
-        ab_mag (np.ndarray or float) : Brightness in AB Magnitude
+    :param intensity: Intensity :math:`\\frac{W}{m^2}`
+    :type intensity: :class:`np.ndarray` or float
+    :param clip: Whether or not to clip very small intensities
+    :type clip: bool, optional
+    :return: AB Magnitude
+    :rtype: :class:`np.ndarray` or float
     """
     log_val = intensity * lumos.constants.WAVELENGTH / (lumos.constants.SPEED_OF_LIGHT * 3631e-26)
     if clip:
         log_val = np.clip(log_val, 10e-6, None)
     ab_mag = -2.5 * np.log10( log_val )
     return ab_mag
 
-def altaz_to_unit(altitude : float | np.ndarray, azimuth : float | np.ndarray) \
-    -> tuple[ float | np.ndarray, ...]:
+def altaz_to_unit(altitude, azimuth):
     """
     Converts altitude and azimuth to a unit vector.
 
-    Parameters:
-        altitude (float or np.ndarray) : Altitude in HCS frame (degrees)
-        azimuth (float or np.ndarray) : Azimuth in HCS frame (degrees)
-    
-    Returns:
-        x, y, z (tuple) : Unit vector components
+    :param altitude: Altitude in HCS frame (degrees)
+    :type altitude: :class:`np.ndarray` or float
+    :param azimuth: Azimuth in HCS frame (degrees)
+    :type azimuth: :class:`np.ndarray` or float
+    :return: Unit vector components :math:`(x, y, z)`
+    :rtype: tuple
     """
     phi = np.deg2rad(90 - altitude)
     theta = np.deg2rad(azimuth)
     x = np.sin(phi) * np.cos(theta)
     y = np.sin(phi) * np.sin(theta)
     z = np.cos(phi)
     return x, y, z
 
-def unit_to_spherical(x : float | np.ndarray, y : float | np.ndarray, z : float | np.ndarray) \
-    -> tuple[float | np.ndarray]:
+def unit_to_spherical(x, y, z):
     """
-    Converts a unit vector to spherical coordinates.
+    Converts a unit vector :math:`(x, y, z)` to spherical coordinates
+    :math:`(\\phi, \\theta)`
 
-    Parameters:
-        x (float or np.ndarray)
-        y (float or np.ndarray)
-        z (float or np.ndarray)
-    
-    Returns:
-        phi, theta (tuple) : Spherical coordinate representation
+    :param x:
+    :type x: :class:`np.ndarray` or float
+    :param y:
+    :type y: :class:`np.ndarray` or float
+    :param z:
+    :type z: :class:`np.ndarray` or float
+    :return: :math:`(\\phi, \\theta)`
+    :rtype: tuple
     """
     phi = np.arccos(z)
     theta = np.arctan2(y, x)
     phi = np.rad2deg(phi)
     theta = np.rad2deg(theta)
     return phi, theta
 
-def spherical_to_unit(phi : float | np.ndarray, theta : float | np.ndarray) \
-    -> tuple[float | np.ndarray]:
+def spherical_to_unit(phi, theta):
     """
-    Converts a unit vector to spherical coordinates.
+    Converts from spherical coordinates :math:`(\\phi, \\theta)`
+    to a unit vector :math:`(x, y, z)`
 
-    Parameters:
-        phi (float or np.ndarray)
-        theta (float or np.ndarray)
-    
-    Returns:
-        x, y, z (tuple) : Unit vector representation
+    :param phi:
+    :type phi: :class:`np.ndarray` or float
+    :param theta:
+    :type theta: :class:`np.ndarray` or float
+    :return: :math:`(x, y, z)`
+    :rtype: tuple
     """
     x = np.sin(phi) * np.cos(theta)
     y = np.sin(phi) * np.sin(theta)
     z = np.cos(phi)
     return x, y, z
```

### Comparing `lumos-sat-1.0.1/lumos/geometry.py` & `lumos-sat-1.0.2/lumos/geometry.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 """
 Geometry objects which are used throughout Lumos
 """
+
 import numpy as np
 import lumos.constants
 class Surface:
-    """ Object to hold area, normal vector, and BRDF of a surface """
-    def __init__(self, area : float, normal : np.ndarray, brdf : callable):
+    """ Container to hold area, normal vector, and BRDF of a surface """
+    def __init__(self, area, normal, brdf):
         """
-        Parameters:
-            area (float) : Area of surface (meters ^ 2)
-            normal (np.ndarray) : Normal vector of surface. Measured in brightness frame.
-            brdf (callable) : BRDF of surface
+        :param area: Area of surface :math:`m^2`
+        :type area: float
+        :param normal: Normal vector of surface. Measured in brightness frame. A function of
+        the angle past terminator may be passed, which must return the surface normal as 
+        a :class:`np.ndarray` for given angles past the terminator.
+        :type normal: :class:`np.ndarray` or function
+        :param brdf: Bidirectional Reflectance Distribution Function (BRDF) of surface.
+        :type brdf: function
         """
         self.area = area
         self.normal = normal
         self.brdf = brdf
     
     def __str__(self):
         return f'| Surface \n' \
@@ -22,19 +27,20 @@
                f'|-- Normal Vector: ' \
                f'<{self.normal[0]:.2f}, {self.normal[1]:.2f}, {self.normal[2]:.2f}> \n'
 
 class EarthMesh:
     """
     A mesh of points on Earth's surface
     """
-    def __init__(self, angles_off_plane : np.ndarray, angles_on_plane : np.ndarray):
+    def __init__(self, angles_off_plane, angles_on_plane):
         """
-        Parameters:
-            angles_off_plane (np.ndarray) : 1D array of the angles-off-plane of the mesh
-            angles_on_plane (np.ndarray) : 1D array of the angles-on-plane of the mesh
+        :param angles_off_plane: 1D array of the angles-off-plane of the mesh.
+        :type angles_off_plane: :class:`np.ndarray`
+        :param angles_on_plane: 1D array of the angles-on-plane of the mesh.
+        :type angles_on_plane: :class:`np.ndarray`
         """
         self.d_phi = np.abs(angles_off_plane[1] - angles_off_plane[0])
         self.d_theta = np.abs(angles_on_plane[1] - angles_on_plane[0])
         
         self.angles_off_plane, self.angles_on_plane = np.meshgrid(angles_off_plane,
                                                                   angles_on_plane)
         
@@ -57,20 +63,22 @@
         self.shape = self.z.shape
         
 class GroundObservers(EarthMesh):
     """
     A mesh of observers visible to the satellite and on the night side of earth
     """
 
-    def __init__(self, sat_height : float, angle_past_terminator : float, density : int):
+    def __init__(self, sat_height, angle_past_terminator, density):
         """
-        Parameters:
-            sat_height (float) : Geodetic height of satellite (meters)
-            angle_past_terminator (float) : Angle of satellite past the terminator (radians)
-            density (int) : Mesh will have size density x density
+        :param sat_height: Geodetic height of satellite (meters)
+        :type sat_height: float
+        :param angle_past_terminator: Angle of satellite past the terminator (radians)
+        :type angle_past_terminator: float
+        :param density: Mesh will have size density x density
+        :type density: int
         """
         self.max_angle = np.arccos(lumos.constants.EARTH_RADIUS 
                                    / (lumos.constants.EARTH_RADIUS + sat_height))
         self.min_angle = angle_past_terminator
         
         angles_off_plane = np.linspace(-self.max_angle, self.max_angle, density)
         angles_on_plane = np.linspace(-self.max_angle, self.min_angle, density)
```

### Comparing `lumos-sat-1.0.1/lumos/plot/brdf.py` & `lumos-sat-1.0.2/lumos/plot/brdf.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,53 @@
+""" Plotting functions for BRDF """
+
 import numpy as np
-import matplotlib.pyplot as plt
-import lumos.brdf.library as brdf_library
 import lumos.conversions
 
-def plot1D(model, incident_angles = (10, 30, 50, 70)):
-    with plt.style.context(["dark_background"]):
-        for angle in incident_angles:
-            x = np.linspace(-90, 90, 400)
-            ix, iy, iz = lumos.conversions.spherical_to_unit(np.deg2rad(angle), np.pi)
-            ox, oy, oz = lumos.conversions.spherical_to_unit(np.deg2rad(x), 0)
-            y = model((ix, iy, iz), (0, 0, 1), (ox, oy, oz))
-            plt.semilogy(x, y, '--k')
-        plt.legend()
-        plt.show()
-
-def plot2D(model, incident_angles = (10, 30, 50, 70)):
-    fig, axs = plt.subplots(ncols = len(incident_angles), subplot_kw={'projection': 'polar'})
-    with plt.style.context(["dark_background"]):
-        for ax, aoi in zip(axs, incident_angles):
-            phi_out = np.linspace(0, 90, 180)
-            theta_out = np.linspace(0, 360, 360)
-            phi_out, theta_out = np.meshgrid(phi_out, theta_out)
-
-            ix, iy, iz = lumos.conversions.spherical_to_unit(np.deg2rad(aoi), np.pi)
-            ox, oy, oz = lumos.conversions.spherical_to_unit(np.deg2rad(phi_out), np.deg2rad(theta_out))
-            y = model((ix, iy, iz), (0, 0, 1), (ox, oy, oz))
-            ax.contourf(np.deg2rad(theta_out), phi_out, np.log10(y))
-            ax.set_title(r"$\phi_{in}$ = " + f"{aoi:0.1f}°")
-            ax.set_xticks([])
-            ax.set_yticks([])
-            ax.set_theta_zero_location('N')
-        plt.show()
+def plot1D(ax, brdf_model, incident_angles = (10, 30, 50, 70), log_space = True):
+    """
+    Plots the in-plane BRDF at given incident angles.
+
+    :param ax: Plotting axis
+    :type ax: :class:`matplotlib.pyplot.axes`
+    :param brdf_model: BRDF function to plot
+    :type brdf_model: function
+    :param incident_angles: Incident angles for which to plot BRDF model (degrees)
+    :type incident_angles: tuple, optional
+    :param log_space: Whether to plot in log space
+    :type log_space: bool, optional
+    """
+    for angle in incident_angles:
+        x = np.linspace(-90, 90, 400)
+        ix, iy, iz = lumos.conversions.spherical_to_unit(np.deg2rad(angle), np.pi)
+        ox, oy, oz = lumos.conversions.spherical_to_unit(np.deg2rad(x), 0)
+        y = brdf_model((ix, iy, iz), (0, 0, 1), (ox, oy, oz))
+        label = r"$\phi_{in}$ = " + f"{angle:0.1f}°"
+        if log_space:
+            ax.semilogy(x, y, label = label)
+        else:
+            ax.plot(x, y, label = label)
+    ax.legend()
+
+def plot2D(polar_ax, brdf_model, incident_angle):
+    """
+    Plots the BRDF at given incident angle.
+
+    :param ax: Plotting axis. Must have polar projection.
+    :type ax: :class:`matplotlib.axes.Axes`
+    :param brdf_model: BRDF function to plot
+    :type brdf_model: function
+    :param incident_angle: Incident angle for which to plot BRDF model (degrees)
+    :type incident_angle: float
+    """
+    phi_out = np.linspace(0, 90, 180)
+    theta_out = np.linspace(0, 360, 360)
+    phi_out, theta_out = np.meshgrid(phi_out, theta_out)
+
+    ix, iy, iz = lumos.conversions.spherical_to_unit(np.deg2rad(incident_angle), np.pi)
+    ox, oy, oz = lumos.conversions.spherical_to_unit(np.deg2rad(phi_out), np.deg2rad(theta_out))
+    y = brdf_model((ix, iy, iz), (0, 0, 1), (ox, oy, oz))
+    polar_ax.contourf(np.deg2rad(theta_out), phi_out, np.log10(y))
+    polar_ax.set_title(r"$\phi_{in}$ = " + f"{incident_angle:0.1f}°")
+    polar_ax.set_xticks([])
+    polar_ax.set_yticks([])
+    polar_ax.set_theta_zero_location('N')
```

### Comparing `lumos-sat-1.0.1/lumos_sat.egg-info/PKG-INFO` & `lumos-sat-1.0.2/lumos_sat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumos-sat
-Version: 1.0.1
+Version: 1.0.2
 Summary: Satellite Brightness Calculation Tools
 Author-email: Forrest Fankhauser <fafankhauser@ucdavis.edu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lumos-sat
```

### Comparing `lumos-sat-1.0.1/lumos_sat.egg-info/SOURCES.txt` & `lumos-sat-1.0.2/lumos_sat.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 lumos/brdf/fit_tools.py
 lumos/brdf/library.py
 lumos/calculators/__init__.py
 lumos/calculators/brightness_frame.py
 lumos/calculators/ground_frame.py
 lumos/plot/__init__.py
 lumos/plot/brdf.py
-lumos/plot/brightness_frame.mplstyle
 lumos/plot/brightness_frame.py
-lumos/plot/ground_frame.mplstyle
 lumos/plot/ground_frame.py
 lumos_sat.egg-info/PKG-INFO
 lumos_sat.egg-info/SOURCES.txt
 lumos_sat.egg-info/dependency_links.txt
 lumos_sat.egg-info/requires.txt
 lumos_sat.egg-info/top_level.txt
```

### Comparing `lumos-sat-1.0.1/pyproject.toml` & `lumos-sat-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lumos-sat"
-version = "1.0.1"
+version = "1.0.2"
 description = "Satellite Brightness Calculation Tools"
 authors = [
     {name = "Forrest Fankhauser", email = "fafankhauser@ucdavis.edu"},
 ]
 requires-python = ">=3.10"
 readme = "README.md"
```

