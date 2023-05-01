# Comparing `tmp/lumos-sat-1.0.2.tar.gz` & `tmp/lumos-sat-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumos-sat-1.0.2.tar", last modified: Mon May  1 19:13:46 2023, max compression
+gzip compressed data, was "lumos-sat-1.0.3.tar", last modified: Mon May  1 19:43:55 2023, max compression
```

## Comparing `lumos-sat-1.0.2.tar` & `lumos-sat-1.0.3.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 19:13:46.385365 lumos-sat-1.0.2/
--rw-rw-rw-   0        0        0     1096 2023-04-06 18:33:06.000000 lumos-sat-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       86 2023-04-06 21:38:28.000000 lumos-sat-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      834 2023-05-01 19:13:46.384367 lumos-sat-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      577 2023-04-06 19:37:58.000000 lumos-sat-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 19:13:46.332508 lumos-sat-1.0.2/lumos/
--rw-rw-rw-   0        0        0        0 2023-04-06 18:42:57.000000 lumos-sat-1.0.2/lumos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:13:46.339488 lumos-sat-1.0.2/lumos/brdf/
--rw-rw-rw-   0        0        0        0 2023-04-06 18:51:47.000000 lumos-sat-1.0.2/lumos/brdf/__init__.py
--rw-rw-rw-   0        0        0     2140 2023-05-01 18:30:13.000000 lumos-sat-1.0.2/lumos/brdf/fit_tools.py
--rw-rw-rw-   0        0        0     6647 2023-05-01 18:23:06.000000 lumos-sat-1.0.2/lumos/brdf/library.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:13:46.347466 lumos-sat-1.0.2/lumos/calculators/
--rw-rw-rw-   0        0        0        0 2023-04-06 18:51:54.000000 lumos-sat-1.0.2/lumos/calculators/__init__.py
--rw-rw-rw-   0        0        0     8082 2023-05-01 18:45:47.000000 lumos-sat-1.0.2/lumos/calculators/brightness_frame.py
--rw-rw-rw-   0        0        0     5378 2023-04-08 02:44:34.000000 lumos-sat-1.0.2/lumos/calculators/ground_frame.py
--rw-rw-rw-   0        0        0      340 2023-04-09 01:56:39.000000 lumos-sat-1.0.2/lumos/constants.py
--rw-rw-rw-   0        0        0     2369 2023-05-01 16:44:37.000000 lumos-sat-1.0.2/lumos/conversions.py
--rw-rw-rw-   0        0        0     3479 2023-04-09 02:37:52.000000 lumos-sat-1.0.2/lumos/functions.py
--rw-rw-rw-   0        0        0     3839 2023-05-01 17:04:37.000000 lumos-sat-1.0.2/lumos/geometry.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:13:46.357439 lumos-sat-1.0.2/lumos/plot/
--rw-rw-rw-   0        0        0        0 2023-03-10 18:54:08.000000 lumos-sat-1.0.2/lumos/plot/__init__.py
--rw-rw-rw-   0        0        0     2153 2023-05-01 17:13:16.000000 lumos-sat-1.0.2/lumos/plot/brdf.py
--rw-rw-rw-   0        0        0     3029 2023-05-01 17:48:10.000000 lumos-sat-1.0.2/lumos/plot/brightness_frame.py
--rw-rw-rw-   0        0        0     4027 2023-05-01 17:58:04.000000 lumos-sat-1.0.2/lumos/plot/ground_frame.py
--rw-rw-rw-   0        0        0      955 2023-05-01 17:10:23.000000 lumos-sat-1.0.2/lumos/video_tools.py
-drwxrwxrwx   0        0        0        0 2023-05-01 19:13:46.381376 lumos-sat-1.0.2/lumos_sat.egg-info/
--rw-rw-rw-   0        0        0      834 2023-05-01 19:13:46.000000 lumos-sat-1.0.2/lumos_sat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      595 2023-05-01 19:13:46.000000 lumos-sat-1.0.2/lumos_sat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 19:13:46.000000 lumos-sat-1.0.2/lumos_sat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2023-05-01 19:13:46.000000 lumos-sat-1.0.2/lumos_sat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-01 19:13:46.000000 lumos-sat-1.0.2/lumos_sat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      588 2023-05-01 18:52:42.000000 lumos-sat-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-01 19:13:46.385365 lumos-sat-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-01 19:43:55.606725 lumos-sat-1.0.3/
+-rw-rw-rw-   0        0        0     1096 2023-04-06 18:33:06.000000 lumos-sat-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      834 2023-05-01 19:43:55.604730 lumos-sat-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      577 2023-04-06 19:37:58.000000 lumos-sat-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 19:43:55.533920 lumos-sat-1.0.3/lumos/
+-rw-rw-rw-   0        0        0        0 2023-04-06 18:42:57.000000 lumos-sat-1.0.3/lumos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 19:43:55.542898 lumos-sat-1.0.3/lumos/brdf/
+-rw-rw-rw-   0        0        0        0 2023-04-06 18:51:47.000000 lumos-sat-1.0.3/lumos/brdf/__init__.py
+-rw-rw-rw-   0        0        0     2140 2023-05-01 18:30:13.000000 lumos-sat-1.0.3/lumos/brdf/fit_tools.py
+-rw-rw-rw-   0        0        0     6648 2023-05-01 19:26:37.000000 lumos-sat-1.0.3/lumos/brdf/library.py
+drwxrwxrwx   0        0        0        0 2023-05-01 19:43:55.554864 lumos-sat-1.0.3/lumos/calculators/
+-rw-rw-rw-   0        0        0        0 2023-04-06 18:51:54.000000 lumos-sat-1.0.3/lumos/calculators/__init__.py
+-rw-rw-rw-   0        0        0     8086 2023-05-01 19:37:37.000000 lumos-sat-1.0.3/lumos/calculators/brightness_frame.py
+-rw-rw-rw-   0        0        0     5444 2023-05-01 19:40:31.000000 lumos-sat-1.0.3/lumos/calculators/ground_frame.py
+-rw-rw-rw-   0        0        0      340 2023-04-09 01:56:39.000000 lumos-sat-1.0.3/lumos/constants.py
+-rw-rw-rw-   0        0        0     2369 2023-05-01 16:44:37.000000 lumos-sat-1.0.3/lumos/conversions.py
+-rw-rw-rw-   0        0        0     3479 2023-04-09 02:37:52.000000 lumos-sat-1.0.3/lumos/functions.py
+-rw-rw-rw-   0        0        0     3839 2023-05-01 17:04:37.000000 lumos-sat-1.0.3/lumos/geometry.py
+drwxrwxrwx   0        0        0        0 2023-05-01 19:43:55.569824 lumos-sat-1.0.3/lumos/plot/
+-rw-rw-rw-   0        0        0        0 2023-03-10 18:54:08.000000 lumos-sat-1.0.3/lumos/plot/__init__.py
+-rw-rw-rw-   0        0        0     2153 2023-05-01 17:13:16.000000 lumos-sat-1.0.3/lumos/plot/brdf.py
+-rw-rw-rw-   0        0        0     3029 2023-05-01 17:48:10.000000 lumos-sat-1.0.3/lumos/plot/brightness_frame.py
+-rw-rw-rw-   0        0        0     4027 2023-05-01 17:58:04.000000 lumos-sat-1.0.3/lumos/plot/ground_frame.py
+-rw-rw-rw-   0        0        0      955 2023-05-01 17:10:23.000000 lumos-sat-1.0.3/lumos/video_tools.py
+drwxrwxrwx   0        0        0        0 2023-05-01 19:43:55.601741 lumos-sat-1.0.3/lumos_sat.egg-info/
+-rw-rw-rw-   0        0        0      834 2023-05-01 19:43:55.000000 lumos-sat-1.0.3/lumos_sat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      583 2023-05-01 19:43:55.000000 lumos-sat-1.0.3/lumos_sat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 19:43:55.000000 lumos-sat-1.0.3/lumos_sat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      220 2023-05-01 19:43:55.000000 lumos-sat-1.0.3/lumos_sat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-01 19:43:55.000000 lumos-sat-1.0.3/lumos_sat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      588 2023-05-01 19:42:40.000000 lumos-sat-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-01 19:43:55.606725 lumos-sat-1.0.3/setup.cfg
```

### Comparing `lumos-sat-1.0.2/LICENSE` & `lumos-sat-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.2/PKG-INFO` & `lumos-sat-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumos-sat
-Version: 1.0.2
+Version: 1.0.3
 Summary: Satellite Brightness Calculation Tools
 Author-email: Forrest Fankhauser <fafankhauser@ucdavis.edu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lumos-sat
```

### Comparing `lumos-sat-1.0.2/README.md` & `lumos-sat-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.2/lumos/brdf/fit_tools.py` & `lumos-sat-1.0.3/lumos/brdf/fit_tools.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.2/lumos/brdf/library.py` & `lumos-sat-1.0.3/lumos/brdf/library.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     
     return BRDF
 
 def GAUSSIAN(A, sigma):
     """
     Gaussian scattering model. 
 
-    :math:`BRDF = A e^{\\frac{\\hat{w}_r\\cdot\\hat{w}_o - 1}{\\sigma}}`
+    :math:`BRDF = A exp(\\frac{\\hat{w}_r\\cdot\\hat{w}_o - 1}{\\sigma})`
 
     :param A: Height of specular peak of BRDF
     :type A: float
     :param sigma: Width of specular peak
     :type sigma: float
     :return: BRDF function, where f = BRDF(incident vector, normal_vector, outgoing_vector)
     :rtype: function
```

### Comparing `lumos-sat-1.0.2/lumos/calculators/brightness_frame.py` & `lumos-sat-1.0.3/lumos/calculators/brightness_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,17 +93,16 @@
     :type angle_past_terminator: float
     :param observer_position: Position of an observer, measured in brightness frame (meters)
     :type observer_position: :class:`np.ndarray`
     :param include_sun: Whether to include flux scattered by the satellite from the sun
     :type include_sun: bool, optional
     :param include_earthshine: Whether to include flux scattered by the satellite from earthshine
     :type include_earthshine: bool, optional
-    :param earth_panel_density: There will be earth_panel_density x earth_panel_density 
-    panels in the earthshine mesh
-    :type earth_panel_density: int
+    :param earth_panel_density: There will be earth_panel_density x earth_panel_density panels in the earthshine mesh
+    :type earth_panel_density: int, optional
     :param earth_brdf: A function representing the BRDF of Earth's surface
     :type earth_brdf: function
     :return: Flux of light incident on the observer (W / m^2)
     :rtype: float
     '''
     
     horizon_angle = np.arccos(lumos.constants.EARTH_RADIUS / (lumos.constants.EARTH_RADIUS + sat_height))
```

### Comparing `lumos-sat-1.0.2/lumos/calculators/ground_frame.py` & `lumos-sat-1.0.3/lumos/calculators/ground_frame.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,34 +6,36 @@
 import lumos.calculators.brightness_frame as brightness_frame
 import lumos.constants
 import lumos.functions
 import lumos.conversions
 import lumos.geometry
 
 def get_brightness_coords(
-    sat_alt : float | np.ndarray, 
-    sat_az : float | np.ndarray, 
-    sat_height : float | np.ndarray, 
-    sun_alt : float, 
-    sun_az : float) \
-    -> tuple[float | np.ndarray, ...]:
-    '''
+    sat_alt, 
+    sat_az, 
+    sat_height, 
+    sun_alt, 
+    sun_az):
+    """
     Converts from HCS observer coordinates to brightness coordinates.
-        Parameters:
-            sat_alt (float or np.ndarray) : Altitude of satellite (degrees)
-            sat_az (float or np.ndarray) : Azimuth of satellite (degrees)
-            sat_height (float or np.ndarray) : Geodetic height of satellite (meters)
-            sun_alt (float) : Altitude of sun (degrees)
-            sun_az (float) : Azimuth of sun (degrees)
-        Returns:
-            obs_x (np.ndarray) : x-component of vector from satellite to observer in brightness frame (meters)
-            obs_y (np.ndarray) : y-component of vector from satellite to observer in brightness frame (meters)
-            obs_z (np.ndarray) : z-component of vector from satellite to observer in brightness frame (meters)
-            angle_past_terminator (np.ndarray) : Angle of satellite past the terminator (radians)
-    '''
+
+    :param sat_alt: Altitude of satellite (degrees)
+    :type sat_alt: float or :class:`np.ndarray`
+    :param sat_az: Altitude of satellite (degrees)
+    :type sat_az: float or :class:`np.ndarray`
+    :param sat_height: Geodetic height of satellite (meters)
+    :type sat_height: float or :class:`np.ndarray`
+    :param sun_alt: Altitude of sun (degrees)
+    :type sun_alt: float
+    :param sun_az: Azimuth angle of sun (degrees)
+    :type sun_az: float
+    :returns:
+        - (obs_x, obs_y, obs_z) - Vector from satellite to observer in brightness frame (meters)
+        - angle_past_terminator - Angle of satellite past terminator (radians)
+    """
 
     sat_x, sat_y, sat_z = lumos.conversions.altaz_to_unit(sat_alt, sat_az)
     sun_x, sun_y, sun_z = lumos.conversions.altaz_to_unit(sun_alt, sun_az)
 
     phi = np.arccos(sat_z) - np.arcsin(lumos.constants.EARTH_RADIUS / (lumos.constants.EARTH_RADIUS + sat_height) * np.sqrt(sat_x**2 + sat_y**2) )
     theta = np.arctan2(sat_y, sat_x)
 
@@ -71,39 +73,52 @@
     obs_z = (lumos.constants.EARTH_RADIUS + sat_height) - dist_to_sat * (T31 * sat_x + T32 * sat_y + T33 * sat_z)
 
     angle_past_terminator = -np.arcsin(T31 * sun_x + T32 * sun_y + T33 * sun_z)
 
     return obs_x, obs_y, obs_z, angle_past_terminator
 
 def calculate_intensity(
-    sat_surfaces : list[lumos.geometry.Surface], 
-    sat_heights : np.ndarray | float, 
-    sat_altitudes : np.ndarray | float, 
-    sat_azimuths : np.ndarray | float,
-    sun_altitude : float, 
-    sun_azimuth : float, 
-    **kwargs) -> np.ndarray | float:
-    '''
-    Calculates the intensity of a satellite as seen in a ground observer's reference frame.
-        Parameters:
-            sat_surfaces (list[Surface]) : A list of lumos.geometry.general.Surface objects
-            sat_heights (np.ndarray or float) : Heights of satellites above geodetic nadir (meters)
-            sat_altitudes (np.ndarray or float) : Altitude of satellites (degrees)
-            sat_azimuths (np.ndarray or float) : Azimuths of satellites (degrees)
-            sun_altitude (float) : Altitude of sun
-            sun_azimuth (float) : Azimuth of sun
-        Keyword Arguments:
-            include_sun (bool) : Whether to include brightness directly reflected from sun
-            include_earthshine (bool) : Whether to include brightness caused by earthshine
-            earth_panel_density (int) : There will be earth_panel_density^2 panels in the earthshine mesh
-            earth_brdf (callable) : A function representing the BRDF of earth
-        Returns:
-            intensity (np.ndarray) : The intensity of light incident on the observer (W / m^2)
-    '''
-
+    sat_surfaces, 
+    sat_heights, 
+    sat_altitudes, 
+    sat_azimuths,
+    sun_altitude, 
+    sun_azimuth,
+    include_sun = True,
+    include_earthshine = True,
+    earth_panel_density = 150,
+    earth_brdf = None):
+
+    """
+    Calculates the flux of a satellite seen by an observer.
+
+    :param sat_surfaces: List of surfaces on satellite
+    :type sat_surfaces: list[lumos.geometry.Surface]
+    :param sat_heights: Heights of satellite above geodetic nadir (meters)
+    :type sat_heights: float or :class:`np.ndarray`
+    :param sat_altitudes: Satellite altitudes in HCS frame (degrees)
+    :type sat_altitudes: float or :class:`np.ndarray`
+    :param sat_azimuths: Satellite azimuths in HCS frame (degrees)
+    :type sat_azimuths: float or :class:`np.ndarray`
+    :param sun_alitutde: Altitude of sun in HCS frame (degrees)
+    :type sun_altitude: float
+    :param sun_azimuth: Azimuth of sun in HCS frame (degrees)
+    :type sun_azimuth: float
+    :param include_sun: Whether to include flux scattered by the satellite from the sun
+    :type include_sun: bool, optional
+    :param include_earthshine: Whether to include flux scattered by the satellite from earthshine
+    :type include_earthshine: bool, optional
+    :param earth_panel_density: There will be earth_panel_density x earth_panel_density panels in the earthshine mesh
+    :type earth_panel_density: int, optional
+    :param earth_brdf: A function representing the BRDF of Earth's surface
+    :type earth_brdf: function
+    :return: Flux of light incident on the observer (W / m^2)
+    :rtype: float or :class:`np.ndarray`
+    """
+    
     if sun_altitude > 0:
         raise ValueError("Observatory is in daylight!")
     
     sat_alts, sat_azs = np.asarray(sat_altitudes), np.asarray(sat_azimuths)
     output_shape = sat_alts.shape
 
     if not isinstance(sat_heights, np.ndarray):
@@ -112,11 +127,13 @@
     sat_heights, sat_alts, sat_azs = sat_heights.flatten(), sat_alts.flatten(), sat_azs.flatten()
     intensity = np.zeros_like(sat_alts)
 
     obs_x, obs_y, obs_z, angle_past_terminator = get_brightness_coords(sat_alts, sat_azs, sat_heights, 
         sun_altitude, sun_azimuth)
 
     for (i, (x, y, z, alpha, h)) in enumerate(zip(obs_x, obs_y, obs_z, angle_past_terminator, sat_heights)):
-        intensity[i] = brightness_frame.calculate_intensity(sat_surfaces, h, alpha, (x, y, z), **kwargs)
-    
+        intensity[i] = brightness_frame.calculate_intensity(
+            sat_surfaces, h, alpha, (x, y, z),
+            include_sun, include_earthshine, earth_panel_density, earth_brdf)
+
     intensity = intensity.reshape(output_shape)
     return intensity
```

### Comparing `lumos-sat-1.0.2/lumos/conversions.py` & `lumos-sat-1.0.3/lumos/conversions.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.2/lumos/functions.py` & `lumos-sat-1.0.3/lumos/functions.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.2/lumos/geometry.py` & `lumos-sat-1.0.3/lumos/geometry.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.2/lumos/plot/brdf.py` & `lumos-sat-1.0.3/lumos/plot/brdf.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.2/lumos/plot/brightness_frame.py` & `lumos-sat-1.0.3/lumos/plot/brightness_frame.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.2/lumos/plot/ground_frame.py` & `lumos-sat-1.0.3/lumos/plot/ground_frame.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.2/lumos/video_tools.py` & `lumos-sat-1.0.3/lumos/video_tools.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.2/lumos_sat.egg-info/PKG-INFO` & `lumos-sat-1.0.3/lumos_sat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumos-sat
-Version: 1.0.2
+Version: 1.0.3
 Summary: Satellite Brightness Calculation Tools
 Author-email: Forrest Fankhauser <fafankhauser@ucdavis.edu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lumos-sat
```

### Comparing `lumos-sat-1.0.2/pyproject.toml` & `lumos-sat-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lumos-sat"
-version = "1.0.2"
+version = "1.0.3"
 description = "Satellite Brightness Calculation Tools"
 authors = [
     {name = "Forrest Fankhauser", email = "fafankhauser@ucdavis.edu"},
 ]
 requires-python = ">=3.10"
 readme = "README.md"
```

