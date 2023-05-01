# Comparing `tmp/gtrpy-1.7.tar.gz` & `tmp/gtrpy-1.8.tar.gz`

## Comparing `gtrpy-1.7.tar` & `gtrpy-1.8.tar`

### file list

```diff
@@ -1,167 +1,167 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 gtrpy-1.7/CONTRIBUTING.md
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 gtrpy-1.7/requirements.txt
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 gtrpy-1.7/demos/demo_1.md
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 gtrpy-1.7/demos/demo_2.md
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 gtrpy-1.7/demos/demo_3.md
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 gtrpy-1.7/demos/demo_4.md
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 gtrpy-1.7/demos/demo_5.md
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gtrpy-1.7/demos/demo_6.md
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 gtrpy-1.7/docs/equations.md
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 gtrpy-1.7/docs/image_size_data.md
--rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 gtrpy-1.7/docs/user_guide.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/__init__.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/run.py
--rw-r--r--   0        0        0    15347 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/equations/grtensorsEP.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/equations/scalarfieldEP.py
--rw-r--r--   0        0        0     8681 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/equations/tensorfieldEP.py
--rw-r--r--   0        0        0     6729 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/equations/vectorfieldEP.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/LX0.png
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/LX1.png
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/LX2.png
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/LX_scalarfield.png
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/LX_tensorfield_02.png
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/LX_tensorfield_11.png
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/LX_tensorfield_20.png
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/LX_vectorfield_01.png
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/LX_vectorfield_10.png
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/chrissymbol.png
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/cov_scalarfield.png
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/cov_tensorfield_02.png
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/cov_tensorfield_11.png
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/cov_tensorfield_20.png
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/cov_vectorfield_01.png
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/cov_vectorfield_10.png
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/e.png
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/einsteintensor.png
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/g0b.png
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/g1b.png
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/g2b.png
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/inversemetrictensor.png
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/kretschmannscalar.png
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/metrictensor.png
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/ricciscalar.png
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/riccitensor.png
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/riemanntensor.png
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/scalarfield.png
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/tensorfield_02.png
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/tensorfield_02_0.png
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/tensorfield_02_1.png
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/tensorfield_02_2.png
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/tensorfield_11.png
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/tensorfield_11_0.png
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/tensorfield_11_1.png
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/tensorfield_11_2.png
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/tensorfield_20.png
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/tensorfield_20_0.png
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/tensorfield_20_1.png
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/tensorfield_20_2.png
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/tracelessriccitensor.png
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/vectorfield_01.png
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/vectorfield_01_0.png
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/vectorfield_01_1.png
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/vectorfield_01_2.png
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/vectorfield_10.png
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/vectorfield_10_0.png
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/vectorfield_10_1.png
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/vectorfield_10_2.png
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/weyltensor.png
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/x0.png
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/x1.png
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images3D/x2.png
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/LX0.png
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/LX1.png
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/LX2.png
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/LX3.png
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/LX_scalarfield.png
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/LX_tensorfield_02.png
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/LX_tensorfield_11.png
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/LX_tensorfield_20.png
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/LX_vectorfield_01.png
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/LX_vectorfield_10.png
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/chrissymbol.png
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/cov_scalarfield.png
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/cov_tensorfield_02.png
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/cov_tensorfield_11.png
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/cov_tensorfield_20.png
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/cov_vectorfield_01.png
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/cov_vectorfield_10.png
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/einsteintensor.png
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/g0beta.png
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/g1beta.png
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/g2beta.png
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/g3beta.png
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/gamma.png
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/inversemetrictensor.png
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/killingvector.png
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/kretschmannscalar.png
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/metrictensor.png
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/ricciscalar.png
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/riccitensor.png
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/riemanntensor.png
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/scalarfield.png
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/tensorfield_02.png
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/tensorfield_02_0.png
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/tensorfield_02_1.png
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/tensorfield_02_2.png
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/tensorfield_02_3.png
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/tensorfield_11.png
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/tensorfield_11_0.png
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/tensorfield_11_1.png
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/tensorfield_11_2.png
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/tensorfield_11_3.png
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/tensorfield_20.png
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/tensorfield_20_0.png
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/tensorfield_20_1.png
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/tensorfield_20_2.png
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/tensorfield_20_3.png
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/tracelessriccitensor.png
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/vectorfield_01.png
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/vectorfield_01_0.png
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/vectorfield_01_1.png
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/vectorfield_01_2.png
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/vectorfield_01_3.png
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/vectorfield_10.png
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/vectorfield_10_0.png
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/vectorfield_10_1.png
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/vectorfield_10_2.png
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/vectorfield_10_3.png
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/weyltensor.png
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/x0.png
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/x1.png
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/x2.png
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/res/images4D/x3.png
--rw-r--r--   0        0        0    16905 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/screen/grtensorsGUI.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/screen/screen3D/coordinates.py
--rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/screen/screen3D/mainpage.py
--rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/screen/screen3D/scalarfieldGUI.py
--rw-r--r--   0        0        0    28180 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/screen/screen3D/tensorfieldGUI.py
--rw-r--r--   0        0        0    14637 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/screen/screen3D/vectorfieldGUI.py
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/screen/screen4D/coordinates.py
--rw-r--r--   0        0        0    10592 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/screen/screen4D/mainpage.py
--rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/screen/screen4D/scalarfieldGUI.py
--rw-r--r--   0        0        0    31249 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/screen/screen4D/tensorfieldGUI.py
--rw-r--r--   0        0        0    18189 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/screen/screen4D/vectorfieldGUI.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/src/fields/scalarfield.py
--rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/src/fields/tensorfield.py
--rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/src/fields/vectorfield.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/src/grtensors/__init__.py
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/src/grtensors/christoffelsymbol.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/src/grtensors/einsteintensor.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/src/grtensors/kretschmannscalar.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/src/grtensors/metrictensor.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/src/grtensors/ricciscalar.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/src/grtensors/riccitensor.py
--rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/src/grtensors/riemanntensor.py
--rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/src/grtensors/tracelessriccitensor.py
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/src/grtensors/weyltensor.py
--rw-r--r--   0        0        0     5175 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/tools/image_resizer_fields3D.py
--rw-r--r--   0        0        0     5970 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/tools/image_resizer_fields4D.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/tools/image_resizer_grtensor.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/tools/latex_image.py
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/tools/latex_output.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 gtrpy-1.7/gtrpy/tools/simplify_objects.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 gtrpy-1.7/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 gtrpy-1.7/LICENSE
--rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 gtrpy-1.7/README.md
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 gtrpy-1.7/pyproject.toml
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 gtrpy-1.7/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 gtrpy-1.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 gtrpy-1.8/requirements.txt
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 gtrpy-1.8/demos/demo_1.md
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 gtrpy-1.8/demos/demo_2.md
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 gtrpy-1.8/demos/demo_3.md
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 gtrpy-1.8/demos/demo_4.md
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 gtrpy-1.8/demos/demo_5.md
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gtrpy-1.8/demos/demo_6.md
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 gtrpy-1.8/docs/equations.md
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 gtrpy-1.8/docs/image_size_data.md
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 gtrpy-1.8/docs/user_guide.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/__init__.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/run.py
+-rw-r--r--   0        0        0    15347 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/equations/grtensorsEP.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/equations/scalarfieldEP.py
+-rw-r--r--   0        0        0     8681 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/equations/tensorfieldEP.py
+-rw-r--r--   0        0        0     6729 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/equations/vectorfieldEP.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/LX0.png
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/LX1.png
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/LX2.png
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/LX_scalarfield.png
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/LX_tensorfield_02.png
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/LX_tensorfield_11.png
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/LX_tensorfield_20.png
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/LX_vectorfield_01.png
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/LX_vectorfield_10.png
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/chrissymbol.png
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/cov_scalarfield.png
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/cov_tensorfield_02.png
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/cov_tensorfield_11.png
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/cov_tensorfield_20.png
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/cov_vectorfield_01.png
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/cov_vectorfield_10.png
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/e.png
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/einsteintensor.png
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/g0b.png
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/g1b.png
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/g2b.png
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/inversemetrictensor.png
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/kretschmannscalar.png
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/metrictensor.png
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/ricciscalar.png
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/riccitensor.png
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/riemanntensor.png
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/scalarfield.png
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/tensorfield_02.png
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/tensorfield_02_0.png
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/tensorfield_02_1.png
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/tensorfield_02_2.png
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/tensorfield_11.png
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/tensorfield_11_0.png
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/tensorfield_11_1.png
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/tensorfield_11_2.png
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/tensorfield_20.png
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/tensorfield_20_0.png
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/tensorfield_20_1.png
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/tensorfield_20_2.png
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/tracelessriccitensor.png
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/vectorfield_01.png
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/vectorfield_01_0.png
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/vectorfield_01_1.png
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/vectorfield_01_2.png
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/vectorfield_10.png
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/vectorfield_10_0.png
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/vectorfield_10_1.png
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/vectorfield_10_2.png
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/weyltensor.png
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/x0.png
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/x1.png
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images3D/x2.png
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/LX0.png
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/LX1.png
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/LX2.png
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/LX3.png
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/LX_scalarfield.png
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/LX_tensorfield_02.png
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/LX_tensorfield_11.png
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/LX_tensorfield_20.png
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/LX_vectorfield_01.png
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/LX_vectorfield_10.png
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/chrissymbol.png
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/cov_scalarfield.png
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/cov_tensorfield_02.png
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/cov_tensorfield_11.png
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/cov_tensorfield_20.png
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/cov_vectorfield_01.png
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/cov_vectorfield_10.png
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/einsteintensor.png
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/g0beta.png
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/g1beta.png
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/g2beta.png
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/g3beta.png
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/gamma.png
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/inversemetrictensor.png
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/killingvector.png
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/kretschmannscalar.png
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/metrictensor.png
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/ricciscalar.png
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/riccitensor.png
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/riemanntensor.png
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/scalarfield.png
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/tensorfield_02.png
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/tensorfield_02_0.png
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/tensorfield_02_1.png
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/tensorfield_02_2.png
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/tensorfield_02_3.png
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/tensorfield_11.png
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/tensorfield_11_0.png
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/tensorfield_11_1.png
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/tensorfield_11_2.png
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/tensorfield_11_3.png
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/tensorfield_20.png
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/tensorfield_20_0.png
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/tensorfield_20_1.png
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/tensorfield_20_2.png
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/tensorfield_20_3.png
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/tracelessriccitensor.png
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/vectorfield_01.png
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/vectorfield_01_0.png
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/vectorfield_01_1.png
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/vectorfield_01_2.png
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/vectorfield_01_3.png
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/vectorfield_10.png
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/vectorfield_10_0.png
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/vectorfield_10_1.png
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/vectorfield_10_2.png
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/vectorfield_10_3.png
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/weyltensor.png
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/x0.png
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/x1.png
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/x2.png
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/res/images4D/x3.png
+-rw-r--r--   0        0        0    16905 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/screen/grtensorsGUI.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/screen/screen3D/coordinates.py
+-rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/screen/screen3D/mainpage.py
+-rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/screen/screen3D/scalarfieldGUI.py
+-rw-r--r--   0        0        0    28180 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/screen/screen3D/tensorfieldGUI.py
+-rw-r--r--   0        0        0    14637 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/screen/screen3D/vectorfieldGUI.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/screen/screen4D/coordinates.py
+-rw-r--r--   0        0        0    10592 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/screen/screen4D/mainpage.py
+-rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/screen/screen4D/scalarfieldGUI.py
+-rw-r--r--   0        0        0    31249 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/screen/screen4D/tensorfieldGUI.py
+-rw-r--r--   0        0        0    18189 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/screen/screen4D/vectorfieldGUI.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/src/fields/scalarfield.py
+-rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/src/fields/tensorfield.py
+-rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/src/fields/vectorfield.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/src/grtensors/__init__.py
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/src/grtensors/christoffelsymbol.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/src/grtensors/einsteintensor.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/src/grtensors/kretschmannscalar.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/src/grtensors/metrictensor.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/src/grtensors/ricciscalar.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/src/grtensors/riccitensor.py
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/src/grtensors/riemanntensor.py
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/src/grtensors/tracelessriccitensor.py
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/src/grtensors/weyltensor.py
+-rw-r--r--   0        0        0     5175 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/tools/image_resizer_fields3D.py
+-rw-r--r--   0        0        0     5970 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/tools/image_resizer_fields4D.py
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/tools/image_resizer_grtensor.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/tools/latex_image.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/tools/latex_output.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 gtrpy-1.8/gtrpy/tools/simplify_objects.py
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 gtrpy-1.8/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 gtrpy-1.8/LICENSE
+-rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 gtrpy-1.8/README.md
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 gtrpy-1.8/pyproject.toml
+-rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 gtrpy-1.8/PKG-INFO
```

### Comparing `gtrpy-1.7/demos/demo_1.md` & `gtrpy-1.8/demos/demo_1.md`

 * *Files 11% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 \alpha^2(r_s)^3(sin^2(\theta))
 $$
 
 you can directly write it as
 
     alpha^2*r_s^3*sin(theta)^2
 
-and the `sympy` will interpret it as it is. In exponential expressions, you can both use `^` and `**`. You can also write `log` as usual, such as `log(10)` etc. For instance, if you want to write
+and the `sympy` will interpret it as it is. In exponential expressions, you can both use `^` and `**`. You can also write `log` as usual, such as `log(10)` etc. Also the exponential expressions ca be written as `exp()`. For instance, if you want to write
 
 $$
-\log(10)r_s^2\psi^{\eta}
+\log(10)r_s^2\psi^{\eta}e^{r}
 $$
 
 you can directly write it as
 
-    log(10)^2*r_s^2*psi^(eta)
+    log(10)^2*r_s^2*psi^(eta)*exp(r)
 
 As you can see most of the greek alphabet will be converted to its corresponding LaTeX form. Here is the list of them and corresponding results in GTRPy.
 
 $$
 {\rm alpha} - \alpha \\
 $$
```

### Comparing `gtrpy-1.7/docs/equations.md` & `gtrpy-1.8/docs/equations.md`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/docs/image_size_data.md` & `gtrpy-1.8/docs/image_size_data.md`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/docs/user_guide.md` & `gtrpy-1.8/docs/user_guide.md`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/run.py` & `gtrpy-1.8/gtrpy/run.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/equations/grtensorsEP.py` & `gtrpy-1.8/gtrpy/equations/grtensorsEP.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/equations/scalarfieldEP.py` & `gtrpy-1.8/gtrpy/equations/scalarfieldEP.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/equations/tensorfieldEP.py` & `gtrpy-1.8/gtrpy/equations/tensorfieldEP.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/equations/vectorfieldEP.py` & `gtrpy-1.8/gtrpy/equations/vectorfieldEP.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/LX_scalarfield.png` & `gtrpy-1.8/gtrpy/res/images3D/LX_scalarfield.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/LX_tensorfield_02.png` & `gtrpy-1.8/gtrpy/res/images3D/LX_tensorfield_02.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/LX_tensorfield_11.png` & `gtrpy-1.8/gtrpy/res/images3D/LX_tensorfield_11.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/LX_tensorfield_20.png` & `gtrpy-1.8/gtrpy/res/images3D/LX_tensorfield_20.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/LX_vectorfield_01.png` & `gtrpy-1.8/gtrpy/res/images3D/LX_vectorfield_01.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/LX_vectorfield_10.png` & `gtrpy-1.8/gtrpy/res/images3D/LX_vectorfield_10.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/chrissymbol.png` & `gtrpy-1.8/gtrpy/res/images3D/chrissymbol.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/cov_scalarfield.png` & `gtrpy-1.8/gtrpy/res/images3D/cov_scalarfield.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/cov_tensorfield_02.png` & `gtrpy-1.8/gtrpy/res/images3D/cov_tensorfield_02.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/cov_tensorfield_11.png` & `gtrpy-1.8/gtrpy/res/images3D/cov_tensorfield_11.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/cov_tensorfield_20.png` & `gtrpy-1.8/gtrpy/res/images3D/cov_tensorfield_20.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/cov_vectorfield_01.png` & `gtrpy-1.8/gtrpy/res/images3D/cov_vectorfield_01.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/cov_vectorfield_10.png` & `gtrpy-1.8/gtrpy/res/images3D/cov_vectorfield_10.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/einsteintensor.png` & `gtrpy-1.8/gtrpy/res/images3D/einsteintensor.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/g0b.png` & `gtrpy-1.8/gtrpy/res/images3D/g0b.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/g1b.png` & `gtrpy-1.8/gtrpy/res/images3D/g1b.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/g2b.png` & `gtrpy-1.8/gtrpy/res/images3D/g2b.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/inversemetrictensor.png` & `gtrpy-1.8/gtrpy/res/images3D/inversemetrictensor.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/metrictensor.png` & `gtrpy-1.8/gtrpy/res/images3D/metrictensor.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/riccitensor.png` & `gtrpy-1.8/gtrpy/res/images3D/riccitensor.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/riemanntensor.png` & `gtrpy-1.8/gtrpy/res/images3D/riemanntensor.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/tensorfield_02.png` & `gtrpy-1.8/gtrpy/res/images3D/tensorfield_02.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/tensorfield_11.png` & `gtrpy-1.8/gtrpy/res/images3D/tensorfield_11.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/tensorfield_20.png` & `gtrpy-1.8/gtrpy/res/images3D/tensorfield_20.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/tracelessriccitensor.png` & `gtrpy-1.8/gtrpy/res/images3D/tracelessriccitensor.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/vectorfield_01.png` & `gtrpy-1.8/gtrpy/res/images3D/vectorfield_01.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/vectorfield_10.png` & `gtrpy-1.8/gtrpy/res/images3D/vectorfield_10.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images3D/weyltensor.png` & `gtrpy-1.8/gtrpy/res/images3D/weyltensor.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/LX_scalarfield.png` & `gtrpy-1.8/gtrpy/res/images4D/LX_scalarfield.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/LX_tensorfield_02.png` & `gtrpy-1.8/gtrpy/res/images4D/LX_tensorfield_02.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/LX_tensorfield_11.png` & `gtrpy-1.8/gtrpy/res/images4D/LX_tensorfield_11.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/LX_tensorfield_20.png` & `gtrpy-1.8/gtrpy/res/images4D/LX_tensorfield_20.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/LX_vectorfield_01.png` & `gtrpy-1.8/gtrpy/res/images4D/LX_vectorfield_01.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/LX_vectorfield_10.png` & `gtrpy-1.8/gtrpy/res/images4D/LX_vectorfield_10.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/chrissymbol.png` & `gtrpy-1.8/gtrpy/res/images4D/chrissymbol.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/cov_scalarfield.png` & `gtrpy-1.8/gtrpy/res/images4D/cov_scalarfield.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/cov_tensorfield_02.png` & `gtrpy-1.8/gtrpy/res/images4D/cov_tensorfield_02.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/cov_tensorfield_11.png` & `gtrpy-1.8/gtrpy/res/images4D/cov_tensorfield_11.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/cov_tensorfield_20.png` & `gtrpy-1.8/gtrpy/res/images4D/cov_tensorfield_20.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/cov_vectorfield_01.png` & `gtrpy-1.8/gtrpy/res/images4D/cov_vectorfield_01.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/cov_vectorfield_10.png` & `gtrpy-1.8/gtrpy/res/images4D/cov_vectorfield_10.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/einsteintensor.png` & `gtrpy-1.8/gtrpy/res/images4D/einsteintensor.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/g0beta.png` & `gtrpy-1.8/gtrpy/res/images4D/g0beta.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/g1beta.png` & `gtrpy-1.8/gtrpy/res/images4D/g1beta.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/g2beta.png` & `gtrpy-1.8/gtrpy/res/images4D/g2beta.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/g3beta.png` & `gtrpy-1.8/gtrpy/res/images4D/g3beta.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/inversemetrictensor.png` & `gtrpy-1.8/gtrpy/res/images4D/inversemetrictensor.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/killingvector.png` & `gtrpy-1.8/gtrpy/res/images4D/killingvector.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/metrictensor.png` & `gtrpy-1.8/gtrpy/res/images4D/metrictensor.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/riccitensor.png` & `gtrpy-1.8/gtrpy/res/images4D/riccitensor.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/riemanntensor.png` & `gtrpy-1.8/gtrpy/res/images4D/riemanntensor.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/tensorfield_02.png` & `gtrpy-1.8/gtrpy/res/images4D/tensorfield_02.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/tensorfield_02_0.png` & `gtrpy-1.8/gtrpy/res/images4D/tensorfield_02_0.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/tensorfield_02_2.png` & `gtrpy-1.8/gtrpy/res/images4D/tensorfield_02_2.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/tensorfield_11.png` & `gtrpy-1.8/gtrpy/res/images4D/tensorfield_11.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/tensorfield_11_0.png` & `gtrpy-1.8/gtrpy/res/images4D/tensorfield_11_0.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/tensorfield_11_1.png` & `gtrpy-1.8/gtrpy/res/images4D/tensorfield_11_1.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/tensorfield_11_2.png` & `gtrpy-1.8/gtrpy/res/images4D/tensorfield_11_2.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/tensorfield_11_3.png` & `gtrpy-1.8/gtrpy/res/images4D/tensorfield_11_3.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/tensorfield_20.png` & `gtrpy-1.8/gtrpy/res/images4D/tensorfield_20.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/tensorfield_20_0.png` & `gtrpy-1.8/gtrpy/res/images4D/tensorfield_20_0.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/tensorfield_20_2.png` & `gtrpy-1.8/gtrpy/res/images4D/tensorfield_20_2.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/tensorfield_20_3.png` & `gtrpy-1.8/gtrpy/res/images4D/tensorfield_20_3.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/tracelessriccitensor.png` & `gtrpy-1.8/gtrpy/res/images4D/tracelessriccitensor.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/vectorfield_01.png` & `gtrpy-1.8/gtrpy/res/images4D/vectorfield_01.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/vectorfield_10.png` & `gtrpy-1.8/gtrpy/res/images4D/vectorfield_10.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/res/images4D/weyltensor.png` & `gtrpy-1.8/gtrpy/res/images4D/weyltensor.png`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/screen/grtensorsGUI.py` & `gtrpy-1.8/gtrpy/screen/grtensorsGUI.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/screen/screen3D/coordinates.py` & `gtrpy-1.8/gtrpy/screen/screen3D/coordinates.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/screen/screen3D/mainpage.py` & `gtrpy-1.8/gtrpy/screen/screen3D/mainpage.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/screen/screen3D/scalarfieldGUI.py` & `gtrpy-1.8/gtrpy/screen/screen3D/scalarfieldGUI.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/screen/screen3D/tensorfieldGUI.py` & `gtrpy-1.8/gtrpy/screen/screen3D/tensorfieldGUI.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/screen/screen3D/vectorfieldGUI.py` & `gtrpy-1.8/gtrpy/screen/screen3D/vectorfieldGUI.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/screen/screen4D/coordinates.py` & `gtrpy-1.8/gtrpy/screen/screen4D/coordinates.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/screen/screen4D/mainpage.py` & `gtrpy-1.8/gtrpy/screen/screen4D/mainpage.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/screen/screen4D/scalarfieldGUI.py` & `gtrpy-1.8/gtrpy/screen/screen4D/scalarfieldGUI.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/screen/screen4D/tensorfieldGUI.py` & `gtrpy-1.8/gtrpy/screen/screen4D/tensorfieldGUI.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/screen/screen4D/vectorfieldGUI.py` & `gtrpy-1.8/gtrpy/screen/screen4D/vectorfieldGUI.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/src/fields/scalarfield.py` & `gtrpy-1.8/gtrpy/src/fields/scalarfield.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/src/fields/tensorfield.py` & `gtrpy-1.8/gtrpy/src/fields/tensorfield.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/src/fields/vectorfield.py` & `gtrpy-1.8/gtrpy/src/fields/vectorfield.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/src/grtensors/christoffelsymbol.py` & `gtrpy-1.8/gtrpy/src/grtensors/christoffelsymbol.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/src/grtensors/einsteintensor.py` & `gtrpy-1.8/gtrpy/src/grtensors/einsteintensor.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/src/grtensors/kretschmannscalar.py` & `gtrpy-1.8/gtrpy/src/grtensors/kretschmannscalar.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/src/grtensors/metrictensor.py` & `gtrpy-1.8/gtrpy/src/grtensors/metrictensor.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/src/grtensors/ricciscalar.py` & `gtrpy-1.8/gtrpy/src/grtensors/ricciscalar.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/src/grtensors/riccitensor.py` & `gtrpy-1.8/gtrpy/src/grtensors/riccitensor.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/src/grtensors/riemanntensor.py` & `gtrpy-1.8/gtrpy/src/grtensors/riemanntensor.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/src/grtensors/tracelessriccitensor.py` & `gtrpy-1.8/gtrpy/src/grtensors/tracelessriccitensor.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/src/grtensors/weyltensor.py` & `gtrpy-1.8/gtrpy/src/grtensors/weyltensor.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/tools/image_resizer_fields3D.py` & `gtrpy-1.8/gtrpy/tools/image_resizer_fields3D.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/tools/image_resizer_fields4D.py` & `gtrpy-1.8/gtrpy/tools/image_resizer_fields4D.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/tools/image_resizer_grtensor.py` & `gtrpy-1.8/gtrpy/tools/image_resizer_grtensor.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/tools/latex_image.py` & `gtrpy-1.8/gtrpy/tools/latex_image.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/gtrpy/tools/latex_output.py` & `gtrpy-1.8/gtrpy/tools/latex_output.py`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/.gitignore` & `gtrpy-1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/LICENSE` & `gtrpy-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gtrpy-1.7/README.md` & `gtrpy-1.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # GTRPy
 
-GTRPy is a python package, that allows you to calculate the well-known tensors in General Theory of Relativity without *writing a single line of code*. Furthermore, you can apply many operations to 6 different type of fields, *in both 3D and 4D*.
+GTRPy is a python package that allows you to calculate the well-known tensors in the General Theory of Relativity without *writing a single line of code*. Furthermore, you can apply many operations to 6 different types of fields, *in both 3D and 4D*.
 
-> It's tested for GNU/Linux, however it should also work in macOS. If you ever encounter with a problem, feel free to create an issue.
+> It's tested for GNU/Linux. However, it should also work in macOS. If you ever encounter with a problem, feel free to create an issue.
 
 ## Installation
 
 You can easily install the GTRPy via
 
     python3 -m pip install gtrpy
 
 or, you can directly clone the repository
 
     git clone https://github.com/seVenVo1d/GTRPy.git
 
+to your favourite directory
+
 ## Requirements
 
-Install the `python` requirements by running
+Install the `python3` requirements by running
 
     python3 -m pip install numpy Pillow pysimplegui sympy
 
-Additionally, you will also need `tkinter` and `LaTeX` support to run the GTRPy. These can be easily installed by running:
+Additionally, you will also need `tkinter` and `LaTeX` support to run the GTRPy. These can be installed by running:
 
 in Fedora
 
     sudo dnf install dvipng python3-tkinter texlive-collection-latex texlive-collection-latexextra
 
 in Ubuntu
 
@@ -32,17 +34,17 @@
 
 ## User Guide
 
 To start GTRPy, simply run
 
     python3 -m gtrpy.run
 
-from the terminal (it does not matter what directory you are in, *if* you installed it via `pip`). The program will create the `logs` directory, under your current directory, which will contain the outputs of the performed operations.
+The program will create the `logs` directory under your current directory, which will contain the outputs of the performed operations.
 
-> Please take a look at the `docs/user_guide.md` for a summary of the GTRPy. To see more detailed examples, you can look at the `demos` directory.
+> Please look at the `docs/user_guide.md` for a summary of the GTRPy. You can look at the `demos` directory, to see more detailed examples.
 
 ## Current Features
 
 ### GTR Tensors
 
 Either by using predefined coordinates or by defining the coordinate system yourself, you can calculate:
 
@@ -52,31 +54,47 @@
 4. Ricci Tensor
 5. Ricci Scalar
 6. Weyl Tensor
 7. Traceless Ricci Tensor
 8. Einstein Tensor
 9. Kretschmann Scalar
 
+The one important point in GTRPy is that the variables defined in the metric tensor **must be constant**. For example, you can write the Schwarzschild Coordinates System as
+
+    g = diag[-(1-r_s/r), (1-r_s/r)**(-1), r^2, r^2sin^2(theta)]
+
+and that is totally fine for GTRPy, since `r_s = 2GM/c^2` is a constant.
+
+Let us suppose you have another variable called `F(r)` which is a function of `r`. And the metric is given as
+
+    g = diag[-1, F, r^2, r^2sin^2(theta)]
+
+Sadly, the GTRPy will interpret this `F` as a constant and not as a function of `r`. So the result will be wrong. On the other hand, if you know what that function is, for instance if `F(r) = r^3`, then you should write `r^3` instead of `F` and use the GTRPy in that way. Thus, you should write the metric as
+
+    g = diag[-1, r^3, r^2, r^2sin^2(theta)]
+
+and now, the GTRPy will work perfectly fine.
+
 ### Fields
 
-Currently, there are 6 different type of fields that you can carry out operations. These are:
+Currently, there are 6 different types of fields that you can carry out operations. These are:
 
 1. Scalar Field
 2. Type (1,0) Vector Field
 3. Type (0,1) Vector Field
 4. Type (2,0) Tensor Field
 5. Type (1,1) Tensor Field
 6. Type (0,2) Tensor Field
 
 ### Available Operations in GTRPy
 
 1. Print out the equations obtained from each operation by clicking a single button
 2. Checking the Killing field condition for a given vector field
 3. Varying the type of a given vector and tensor field
-4. Calculating Covariant and Lie derivatives for scalar, vector and tensor fields
+4. Calculating Covariant and Lie derivatives for scalar, vector, and tensor fields
 
 ## Overview
 
 4D/Main Page          |  3D/Main Page
 :-------------------------:|:-------------------------:
 ![4d_main](https://user-images.githubusercontent.com/45866787/213305163-b6470289-e167-4ffd-ab18-d592ae19011e.png) | ![3d_main](https://user-images.githubusercontent.com/45866787/213305193-9efe501f-0347-4166-a487-2cbdee3fe24c.png)
 
@@ -86,14 +104,15 @@
 
 3D/Scalar Field        |  3D/Vector Field       | 3D/Tensor Field
 :-------------------------:|:-------------------------:|:-------------------------:
 ![3d_scalar](https://user-images.githubusercontent.com/45866787/212769736-171c0a1f-63a2-44f4-96ab-b86bf6eeef8f.png) |![3d_vector](https://user-images.githubusercontent.com/45866787/212769750-de725b69-0a9f-460f-b451-5e03ecd758c5.png) | ![Screenshot from 2023-01-28 22-47-14](https://user-images.githubusercontent.com/45866787/215287851-73694819-fb9e-4d14-88c8-36718a5e1f1d.png)
 
 ## Upcoming Features
 
-1. Gradient, Divergence, Curl and Laplace operations on fields
+1. Gradient, Divergence, Curl, and Laplace operations on fields
 2. Partial and Covariant derivatives of the GTR tensors
 3. Including more coordinate systems
+4. Adding a user-defined (custom function) support
 
 ## Contributing
 
-I am looking for developers who would like to contribute to the project. If you are interested, feel free to create an issue by stating how would you like to contribute. Any help or idea is welcomed. For more information you can also look at the `CONTRIBUTING.md`.
+I am looking for developers who would like to contribute to the project. If you are interested, feel free to create an issue by stating how would you like to contribute. Any help or idea is appreciated. For more information, you can also look at the `CONTRIBUTING.md`.
```

### Comparing `gtrpy-1.7/pyproject.toml` & `gtrpy-1.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gtrpy"
-version = "1.7"
+version = "1.8"
 authors = [
   {name="Arman Çam"},
 ]
-description = "GTRPy is a python package that allows you to calculate the well-known tensors in General Theory of Relativity."
+description = "GTRPy is a python package that allows you to calculate the well-known tensors in the General Theory of Relativity."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: MacOS",
     "Operating System :: POSIX :: Linux",
```

### Comparing `gtrpy-1.7/PKG-INFO` & `gtrpy-1.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gtrpy
-Version: 1.7
-Summary: GTRPy is a python package that allows you to calculate the well-known tensors in General Theory of Relativity.
+Version: 1.8
+Summary: GTRPy is a python package that allows you to calculate the well-known tensors in the General Theory of Relativity.
 Project-URL: Homepage, https://github.com/seVenVo1d/GRPy
 Project-URL: Bug Tracker, https://github.com/seVenVo1d/GRPy/issues
 Author: Arman Çam
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -14,35 +14,37 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # GTRPy
 
-GTRPy is a python package, that allows you to calculate the well-known tensors in General Theory of Relativity without *writing a single line of code*. Furthermore, you can apply many operations to 6 different type of fields, *in both 3D and 4D*.
+GTRPy is a python package that allows you to calculate the well-known tensors in the General Theory of Relativity without *writing a single line of code*. Furthermore, you can apply many operations to 6 different types of fields, *in both 3D and 4D*.
 
-> It's tested for GNU/Linux, however it should also work in macOS. If you ever encounter with a problem, feel free to create an issue.
+> It's tested for GNU/Linux. However, it should also work in macOS. If you ever encounter with a problem, feel free to create an issue.
 
 ## Installation
 
 You can easily install the GTRPy via
 
     python3 -m pip install gtrpy
 
 or, you can directly clone the repository
 
     git clone https://github.com/seVenVo1d/GTRPy.git
 
+to your favourite directory
+
 ## Requirements
 
-Install the `python` requirements by running
+Install the `python3` requirements by running
 
     python3 -m pip install numpy Pillow pysimplegui sympy
 
-Additionally, you will also need `tkinter` and `LaTeX` support to run the GTRPy. These can be easily installed by running:
+Additionally, you will also need `tkinter` and `LaTeX` support to run the GTRPy. These can be installed by running:
 
 in Fedora
 
     sudo dnf install dvipng python3-tkinter texlive-collection-latex texlive-collection-latexextra
 
 in Ubuntu
 
@@ -50,17 +52,17 @@
 
 ## User Guide
 
 To start GTRPy, simply run
 
     python3 -m gtrpy.run
 
-from the terminal (it does not matter what directory you are in, *if* you installed it via `pip`). The program will create the `logs` directory, under your current directory, which will contain the outputs of the performed operations.
+The program will create the `logs` directory under your current directory, which will contain the outputs of the performed operations.
 
-> Please take a look at the `docs/user_guide.md` for a summary of the GTRPy. To see more detailed examples, you can look at the `demos` directory.
+> Please look at the `docs/user_guide.md` for a summary of the GTRPy. You can look at the `demos` directory, to see more detailed examples.
 
 ## Current Features
 
 ### GTR Tensors
 
 Either by using predefined coordinates or by defining the coordinate system yourself, you can calculate:
 
@@ -70,31 +72,47 @@
 4. Ricci Tensor
 5. Ricci Scalar
 6. Weyl Tensor
 7. Traceless Ricci Tensor
 8. Einstein Tensor
 9. Kretschmann Scalar
 
+The one important point in GTRPy is that the variables defined in the metric tensor **must be constant**. For example, you can write the Schwarzschild Coordinates System as
+
+    g = diag[-(1-r_s/r), (1-r_s/r)**(-1), r^2, r^2sin^2(theta)]
+
+and that is totally fine for GTRPy, since `r_s = 2GM/c^2` is a constant.
+
+Let us suppose you have another variable called `F(r)` which is a function of `r`. And the metric is given as
+
+    g = diag[-1, F, r^2, r^2sin^2(theta)]
+
+Sadly, the GTRPy will interpret this `F` as a constant and not as a function of `r`. So the result will be wrong. On the other hand, if you know what that function is, for instance if `F(r) = r^3`, then you should write `r^3` instead of `F` and use the GTRPy in that way. Thus, you should write the metric as
+
+    g = diag[-1, r^3, r^2, r^2sin^2(theta)]
+
+and now, the GTRPy will work perfectly fine.
+
 ### Fields
 
-Currently, there are 6 different type of fields that you can carry out operations. These are:
+Currently, there are 6 different types of fields that you can carry out operations. These are:
 
 1. Scalar Field
 2. Type (1,0) Vector Field
 3. Type (0,1) Vector Field
 4. Type (2,0) Tensor Field
 5. Type (1,1) Tensor Field
 6. Type (0,2) Tensor Field
 
 ### Available Operations in GTRPy
 
 1. Print out the equations obtained from each operation by clicking a single button
 2. Checking the Killing field condition for a given vector field
 3. Varying the type of a given vector and tensor field
-4. Calculating Covariant and Lie derivatives for scalar, vector and tensor fields
+4. Calculating Covariant and Lie derivatives for scalar, vector, and tensor fields
 
 ## Overview
 
 4D/Main Page          |  3D/Main Page
 :-------------------------:|:-------------------------:
 ![4d_main](https://user-images.githubusercontent.com/45866787/213305163-b6470289-e167-4ffd-ab18-d592ae19011e.png) | ![3d_main](https://user-images.githubusercontent.com/45866787/213305193-9efe501f-0347-4166-a487-2cbdee3fe24c.png)
 
@@ -104,14 +122,15 @@
 
 3D/Scalar Field        |  3D/Vector Field       | 3D/Tensor Field
 :-------------------------:|:-------------------------:|:-------------------------:
 ![3d_scalar](https://user-images.githubusercontent.com/45866787/212769736-171c0a1f-63a2-44f4-96ab-b86bf6eeef8f.png) |![3d_vector](https://user-images.githubusercontent.com/45866787/212769750-de725b69-0a9f-460f-b451-5e03ecd758c5.png) | ![Screenshot from 2023-01-28 22-47-14](https://user-images.githubusercontent.com/45866787/215287851-73694819-fb9e-4d14-88c8-36718a5e1f1d.png)
 
 ## Upcoming Features
 
-1. Gradient, Divergence, Curl and Laplace operations on fields
+1. Gradient, Divergence, Curl, and Laplace operations on fields
 2. Partial and Covariant derivatives of the GTR tensors
 3. Including more coordinate systems
+4. Adding a user-defined (custom function) support
 
 ## Contributing
 
-I am looking for developers who would like to contribute to the project. If you are interested, feel free to create an issue by stating how would you like to contribute. Any help or idea is welcomed. For more information you can also look at the `CONTRIBUTING.md`.
+I am looking for developers who would like to contribute to the project. If you are interested, feel free to create an issue by stating how would you like to contribute. Any help or idea is appreciated. For more information, you can also look at the `CONTRIBUTING.md`.
```

