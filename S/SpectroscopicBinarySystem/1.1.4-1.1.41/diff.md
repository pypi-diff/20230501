# Comparing `tmp/SpectroscopicBinarySystem-1.1.4.tar.gz` & `tmp/SpectroscopicBinarySystem-1.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpectroscopicBinarySystem-1.1.4.tar", last modified: Sun Apr 30 06:30:50 2023, max compression
+gzip compressed data, was "SpectroscopicBinarySystem-1.1.41.tar", last modified: Mon May  1 08:02:29 2023, max compression
```

## Comparing `SpectroscopicBinarySystem-1.1.4.tar` & `SpectroscopicBinarySystem-1.1.41.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 06:30:50.469345 SpectroscopicBinarySystem-1.1.4/
--rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.1.4/LICENSE
--rw-rw-rw-   0        0        0     3360 2023-04-30 06:30:50.469345 SpectroscopicBinarySystem-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2969 2023-04-30 06:30:14.000000 SpectroscopicBinarySystem-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 06:30:50.469345 SpectroscopicBinarySystem-1.1.4/SpectroscopicBinarySystem.egg-info/
--rw-rw-rw-   0        0        0     3360 2023-04-30 06:30:50.000000 SpectroscopicBinarySystem-1.1.4/SpectroscopicBinarySystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-04-30 06:30:50.000000 SpectroscopicBinarySystem-1.1.4/SpectroscopicBinarySystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 06:30:50.000000 SpectroscopicBinarySystem-1.1.4/SpectroscopicBinarySystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      174 2023-04-30 06:30:50.000000 SpectroscopicBinarySystem-1.1.4/SpectroscopicBinarySystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-04-30 06:30:50.000000 SpectroscopicBinarySystem-1.1.4/SpectroscopicBinarySystem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.1.4/pyproject.toml
--rw-rw-rw-   0        0        0      724 2023-04-30 06:30:50.477830 SpectroscopicBinarySystem-1.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-30 06:30:50.469345 SpectroscopicBinarySystem-1.1.4/spectroscopicbinarysystem/
--rw-rw-rw-   0        0        0    29339 2023-04-30 06:27:46.000000 SpectroscopicBinarySystem-1.1.4/spectroscopicbinarysystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 08:02:29.299115 SpectroscopicBinarySystem-1.1.41/
+-rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.1.41/LICENSE
+-rw-rw-rw-   0        0        0     4731 2023-05-01 08:02:29.299115 SpectroscopicBinarySystem-1.1.41/PKG-INFO
+-rw-rw-rw-   0        0        0     4339 2023-04-30 07:01:52.000000 SpectroscopicBinarySystem-1.1.41/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 08:02:29.287400 SpectroscopicBinarySystem-1.1.41/SpectroscopicBinarySystem.egg-info/
+-rw-rw-rw-   0        0        0     4731 2023-05-01 08:02:29.000000 SpectroscopicBinarySystem-1.1.41/SpectroscopicBinarySystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-05-01 08:02:29.000000 SpectroscopicBinarySystem-1.1.41/SpectroscopicBinarySystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 08:02:29.000000 SpectroscopicBinarySystem-1.1.41/SpectroscopicBinarySystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2023-05-01 08:02:29.000000 SpectroscopicBinarySystem-1.1.41/SpectroscopicBinarySystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-05-01 08:02:29.000000 SpectroscopicBinarySystem-1.1.41/SpectroscopicBinarySystem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.1.41/pyproject.toml
+-rw-rw-rw-   0        0        0      725 2023-05-01 08:02:29.299115 SpectroscopicBinarySystem-1.1.41/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-01 08:02:29.295916 SpectroscopicBinarySystem-1.1.41/spectroscopicbinarysystem/
+-rw-rw-rw-   0        0        0    29368 2023-05-01 07:46:22.000000 SpectroscopicBinarySystem-1.1.41/spectroscopicbinarysystem/__init__.py
```

### Comparing `SpectroscopicBinarySystem-1.1.4/LICENSE` & `SpectroscopicBinarySystem-1.1.41/LICENSE`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.1.4/SpectroscopicBinarySystem.egg-info/SOURCES.txt` & `SpectroscopicBinarySystem-1.1.41/SpectroscopicBinarySystem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.1.4/setup.cfg` & `SpectroscopicBinarySystem-1.1.41/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 7065 6374 726f 7363 6f70 6963   = Spectroscopic
 00000020: 4269 6e61 7279 5379 7374 656d 0d0a 7665  BinarySystem..ve
-00000030: 7273 696f 6e20 3d20 312e 312e 340d 0a61  rsion = 1.1.4..a
-00000040: 7574 686f 7220 3d20 4775 696c 6c61 756d  uthor = Guillaum
-00000050: 6520 4265 7274 7261 6e64 0d0a 6175 7468  e Bertrand..auth
-00000060: 6f72 5f65 6d61 696c 203d 2067 6265 2e69  or_email = gbe.i
-00000070: 6f40 706d 2e6d 650d 0a64 6573 6372 6970  o@pm.me..descrip
-00000080: 7469 6f6e 203d 2050 7974 686f 6e20 6173  tion = Python as
-00000090: 7472 6f6e 6f6d 7920 746f 6f6c 7320 666f  tronomy tools fo
-000000a0: 7220 7370 6563 7472 6f73 636f 7069 6320  r spectroscopic 
-000000b0: 6269 6e61 7279 2073 7973 7465 6d0d 0a6c  binary system..l
-000000c0: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
-000000d0: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
-000000e0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
-000000f0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
-00000100: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
-00000110: 0d0a 6c69 6365 6e73 6520 3d20 4253 442d  ..license = BSD-
-00000120: 332d 436c 6175 7365 0d0a 6c69 6365 6e73  3-Clause..licens
-00000130: 655f 6669 6c65 7320 3d20 4c49 4345 4e53  e_files = LICENS
-00000140: 450d 0a6b 6579 776f 7264 7320 3d20 6173  E..keywords = as
-00000150: 7472 6f6e 6f6d 792c 6173 7472 6f70 6879  tronomy,astrophy
-00000160: 7369 6373 2c73 6369 656e 6365 2c66 6974  sics,science,fit
-00000170: 732c 6d6f 6465 6c73 2c66 6974 7469 6e67  s,models,fitting
-00000180: 2c73 7065 6374 726f 7363 6f70 792c 7370  ,spectroscopy,sp
-00000190: 6563 7472 756d 0d0a 0d0a 5b6f 7074 696f  ectrum....[optio
-000001a0: 6e73 5d0d 0a70 6163 6b61 6765 7320 3d20  ns]..packages = 
-000001b0: 6669 6e64 3a0d 0a70 7974 686f 6e5f 7265  find:..python_re
-000001c0: 7175 6972 6573 203d 203e 3d33 2e31 300d  quires = >=3.10.
-000001d0: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
-000001e0: 7320 3d20 0d0a 0961 7374 726f 7079 3e3d  s = ...astropy>=
-000001f0: 352e 322e 320d 0a09 6173 7472 6f71 7565  5.2.2...astroque
-00000200: 7279 3e3d 302e 342e 360d 0a09 4269 6e61  ry>=0.4.6...Bina
-00000210: 7279 5374 6172 536f 6c76 6572 3e3d 312e  ryStarSolver>=1.
-00000220: 322e 300d 0a09 6d61 7470 6c6f 746c 6962  2.0...matplotlib
-00000230: 3e3d 332e 372e 310d 0a09 6e75 6d70 793e  >=3.7.1...numpy>
-00000240: 3d31 2e32 342e 320d 0a09 4f72 6269 7461  =1.24.2...Orbita
-00000250: 6c50 793e 3d30 2e37 2e30 0d0a 0950 7959  lPy>=0.7.0...PyY
-00000260: 414d 4c3e 3d36 2e30 0d0a 0973 7065 6375  AML>=6.0...specu
-00000270: 7469 6c73 3e3d 312e 392e 310d 0a09 4269  tils>=1.9.1...Bi
-00000280: 6e61 7279 5374 6172 536f 6c76 6572 3e3d  naryStarSolver>=
-00000290: 312e 322e 300d 0a09 706c 6f74 6c79 3e3d  1.2.0...plotly>=
-000002a0: 352e 3134 2e31 0d0a 0d0a 5b65 6767 5f69  5.14.1....[egg_i
-000002b0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
-000002c0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
-000002d0: 0d0a 0d0a                                ....
+00000030: 7273 696f 6e20 3d20 312e 312e 3431 0d0a  rsion = 1.1.41..
+00000040: 6175 7468 6f72 203d 2047 7569 6c6c 6175  author = Guillau
+00000050: 6d65 2042 6572 7472 616e 640d 0a61 7574  me Bertrand..aut
+00000060: 686f 725f 656d 6169 6c20 3d20 6762 652e  hor_email = gbe.
+00000070: 696f 4070 6d2e 6d65 0d0a 6465 7363 7269  io@pm.me..descri
+00000080: 7074 696f 6e20 3d20 5079 7468 6f6e 2061  ption = Python a
+00000090: 7374 726f 6e6f 6d79 2074 6f6f 6c73 2066  stronomy tools f
+000000a0: 6f72 2073 7065 6374 726f 7363 6f70 6963  or spectroscopic
+000000b0: 2062 696e 6172 7920 7379 7374 656d 0d0a   binary system..
+000000c0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000d0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
+000000e0: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
+000000f0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
+00000100: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
+00000110: 6e0d 0a6c 6963 656e 7365 203d 2042 5344  n..license = BSD
+00000120: 2d33 2d43 6c61 7573 650d 0a6c 6963 656e  -3-Clause..licen
+00000130: 7365 5f66 696c 6573 203d 204c 4943 454e  se_files = LICEN
+00000140: 5345 0d0a 6b65 7977 6f72 6473 203d 2061  SE..keywords = a
+00000150: 7374 726f 6e6f 6d79 2c61 7374 726f 7068  stronomy,astroph
+00000160: 7973 6963 732c 7363 6965 6e63 652c 6669  ysics,science,fi
+00000170: 7473 2c6d 6f64 656c 732c 6669 7474 696e  ts,models,fittin
+00000180: 672c 7370 6563 7472 6f73 636f 7079 2c73  g,spectroscopy,s
+00000190: 7065 6374 7275 6d0d 0a0d 0a5b 6f70 7469  pectrum....[opti
+000001a0: 6f6e 735d 0d0a 7061 636b 6167 6573 203d  ons]..packages =
+000001b0: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
+000001c0: 6571 7569 7265 7320 3d20 3e3d 332e 3130  equires = >=3.10
+000001d0: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
+000001e0: 6573 203d 200d 0a09 6173 7472 6f70 793e  es = ...astropy>
+000001f0: 3d35 2e32 2e32 0d0a 0961 7374 726f 7175  =5.2.2...astroqu
+00000200: 6572 793e 3d30 2e34 2e36 0d0a 0942 696e  ery>=0.4.6...Bin
+00000210: 6172 7953 7461 7253 6f6c 7665 723e 3d31  aryStarSolver>=1
+00000220: 2e32 2e30 0d0a 096d 6174 706c 6f74 6c69  .2.0...matplotli
+00000230: 623e 3d33 2e37 2e31 0d0a 096e 756d 7079  b>=3.7.1...numpy
+00000240: 3e3d 312e 3234 2e32 0d0a 094f 7262 6974  >=1.24.2...Orbit
+00000250: 616c 5079 3e3d 302e 372e 300d 0a09 5079  alPy>=0.7.0...Py
+00000260: 5941 4d4c 3e3d 362e 300d 0a09 7370 6563  YAML>=6.0...spec
+00000270: 7574 696c 733e 3d31 2e39 2e31 0d0a 0942  utils>=1.9.1...B
+00000280: 696e 6172 7953 7461 7253 6f6c 7665 723e  inaryStarSolver>
+00000290: 3d31 2e32 2e30 0d0a 0970 6c6f 746c 793e  =1.2.0...plotly>
+000002a0: 3d35 2e31 342e 310d 0a0d 0a5b 6567 675f  =5.14.1....[egg_
+000002b0: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+000002c0: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+000002d0: 300d 0a0d 0a                             0....
```

### Comparing `SpectroscopicBinarySystem-1.1.4/spectroscopicbinarysystem/__init__.py` & `SpectroscopicBinarySystem-1.1.41/spectroscopicbinarysystem/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -712,15 +712,16 @@
             ss = copy.copy(s)
             # apply heliocentric/barycentric correction
             ss.shift_spectrum_to(
                 radial_velocity=s.getRVCorrection())
             fluxc_resample = LinearInterpolatedResampler()
             output_spectrum1D = fluxc_resample(ss, sc)
             phase = s.getPhase()
-            indice = int(round(phase, 2) * len(y_phase))
+            indice = int(round(phase, 2) * len(y_phase))-1
+
             spec2d[:, indice] = output_spectrum1D.flux
 
         # prepare imshow
         plt.rcParams["figure.figsize"] = (8, 7)
         fig, ax = plt.subplots()
         ax.imshow(np.rot90(spec2d), extent=[wv_to_kms.min().value,
                                             wv_to_kms.max().value, 0, 1], aspect='auto')
@@ -739,7 +740,9 @@
 
         plt.tight_layout(pad=3, w_pad=0, h_pad=1)
         plt.yticks(np.arange(0, 1.01, 0.1))
         if savefig:
             plt.savefig(
                 f'{self._spectra_path}/{self._object_name}_2d_spectrum_result.png', dpi=dpi)
         plt.show()
+
+        return spec2d
```

