# Comparing `tmp/rescupybs-0.0.1.4.1-py3-none-any.whl.zip` & `tmp/rescupybs-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9034 bytes, number of entries: 10
--rw-rw-r--  2.0 unx       31 b- defN 23-Apr-17 15:02 rescupybs/__init__.py
--rw-rw-r--  2.0 unx     8451 b- defN 23-Apr-17 15:02 rescupybs/functions.py
--rw-rw-r--  2.0 unx     6786 b- defN 23-Apr-17 15:02 rescupybs/plots.py
--rw-rw-r--  2.0 unx    12318 b- defN 23-Apr-17 15:02 rescupybs/wrapper.py
--rwxrwxr-x  2.0 unx     1060 b- defN 23-Apr-17 15:02 rescupybs-0.0.1.4.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2965 b- defN 23-Apr-17 15:02 rescupybs-0.0.1.4.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-17 15:02 rescupybs-0.0.1.4.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       88 b- defN 23-Apr-17 15:02 rescupybs-0.0.1.4.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       10 b- defN 23-Apr-17 15:02 rescupybs-0.0.1.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      825 b- defN 23-Apr-17 15:02 rescupybs-0.0.1.4.1.dist-info/RECORD
-10 files, 32626 bytes uncompressed, 7620 bytes compressed:  76.6%
+Zip file size: 9402 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx       27 b- defN 23-May-01 05:23 rescupybs/__init__.py
+-rw-rw-r--  2.0 unx    13813 b- defN 23-May-01 05:23 rescupybs/functions.py
+-rw-rw-r--  2.0 unx     6786 b- defN 23-May-01 05:23 rescupybs/plots.py
+-rw-rw-r--  2.0 unx    12499 b- defN 23-May-01 05:23 rescupybs/wrapper.py
+-rwxrwxr-x  2.0 unx     1060 b- defN 23-May-01 05:24 rescupybs-0.1.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2961 b- defN 23-May-01 05:24 rescupybs-0.1.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-01 05:24 rescupybs-0.1.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       88 b- defN 23-May-01 05:24 rescupybs-0.1.0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       10 b- defN 23-May-01 05:24 rescupybs-0.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      802 b- defN 23-May-01 05:24 rescupybs-0.1.0.dist-info/RECORD
+10 files, 38138 bytes uncompressed, 8036 bytes compressed:  78.9%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: rescupybs/plots.py
 Comment: 
 
 Filename: rescupybs/wrapper.py
 Comment: 
 
-Filename: rescupybs-0.0.1.4.1.dist-info/LICENSE
+Filename: rescupybs-0.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: rescupybs-0.0.1.4.1.dist-info/METADATA
+Filename: rescupybs-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: rescupybs-0.0.1.4.1.dist-info/WHEEL
+Filename: rescupybs-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: rescupybs-0.0.1.4.1.dist-info/entry_points.txt
+Filename: rescupybs-0.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: rescupybs-0.0.1.4.1.dist-info/top_level.txt
+Filename: rescupybs-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: rescupybs-0.0.1.4.1.dist-info/RECORD
+Filename: rescupybs-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rescupybs/__init__.py

```diff
@@ -1,3 +1,3 @@
 
-__version__ = "0.0.1.4.1"
+__version__ = "0.1.0"
```

## rescupybs/functions.py

```diff
@@ -152,42 +152,166 @@
     i, cb = np.where(eigenvalues_s==min)
     return vb[0], max, cb[0], min
 
 # rescuiso
 
 def isosurfaces_wf(input, output, kpt, band, spin):
     calc = TotalEnergy.read(input+'.json')
-    if not output:
-        output = input+'_'+str(kpt)+'_'+str(band)+'_'+str(spin)+'.vasp'
-    if calc.system.hamiltonian.ispin == 1:
-        att = f"wavefunctions/{kpt + 1}/field"
-    else:
-        if spin == 1:
-            att = f"wavefunctions/spin-up/{kpt + 1}/field"
+    kpt_l = len(kpt)
+    band_l = len(band)
+    if kpt_l == 1 and band_l == 1:
+        if not output:
+            output = input+'_'+str(kpt[0])+'_'+str(band[0])+'_'+str(spin)+'.vasp'
+        if calc.system.hamiltonian.ispin == 1:
+            att = f"wavefunctions/{kpt[0] + 1}/field"
+        else:
+            if spin == 1:
+                att = f"wavefunctions/spin-up/{kpt[0] + 1}/field"
+            else:
+                att = f"wavefunctions/spin-down/{kpt[0] + 1}/field"
+        print("Reading *.h5 file ...")
+        filename = input+'.h5'
+        h = h5py.File(filename, mode="r")
+        print("Processing data ...")
+        fld = h[att][0:]
+        fld = np.transpose(fld, [i for i in range(fld.ndim - 1, -1, -1)])
+        fld = np.asfortranarray(fld)
+        fld = fld / ureg.bohr**1.5
+        fld = fld[::2, :] + 1j * fld[1::2, :]
+        fld.ito("angstrom ** -1.5")
+        if band[0] < fld.shape[-1]:
+            fld = fld[..., band[0]].magnitude
+        else:
+            raise Exception("The band is out of range in *.h5 file.")
+        f_abs = np.abs(fld)
+        f_div = np.where(np.abs(np.angle(fld)) < np.pi / 2, f_abs, -f_abs)
+        f_div = np.reshape(f_div, (f_div.shape[-1], -1), order='F').T
+    elif kpt_l == 2 and band_l == 1:
+        if not kpt[0] < kpt[1]:
+            raise Exception("Illegal input of kpt.")
+        if not output:
+            output = input+'_'+str(kpt[0])+'-'+str(kpt[1])+'_'+str(band[0])+'_'+str(spin)+'.vasp'
+        nkpts = kpt[1] - kpt[0] + 1
+        att = [''] * nkpts
+        for i in range(kpt[0], kpt[1] + 1):
+            if calc.system.hamiltonian.ispin == 1:
+                att[i] = f"wavefunctions/{i + 1}/field"
+            else:
+                if spin == 1:
+                    att[i] = f"wavefunctions/spin-up/{i + 1}/field"
+                else:
+                    att[i] = f"wavefunctions/spin-down/{i + 1}/field"
+        print("Reading *.h5 file ...")
+        filename = input+'.h5'
+        h = h5py.File(filename, mode="r")
+        print("Processing data ...")
+        for i in range(nkpts):
+            fld_i = h[att[i]][0:]
+            if i == 0:
+                fld = fld_i
+            else:
+                fld += fld_i
+        fld = np.transpose(fld, [i for i in range(fld.ndim - 1, -1, -1)])
+        fld = np.asfortranarray(fld)
+        fld = fld / ureg.bohr**1.5
+        fld = fld[::2, :] + 1j * fld[1::2, :]
+        fld.ito("angstrom ** -1.5")
+        if band[0] < fld.shape[-1]:
+            fld = fld[..., band[0]].magnitude
+        else:
+            raise Exception("The band is out of range in *.h5 file.")
+        f_abs = np.abs(fld)
+        f_div = np.where(np.abs(np.angle(fld)) < np.pi / 2, f_abs, -f_abs)
+        f_div = np.reshape(f_div, (f_div.shape[-1], -1), order='F').T
+    elif kpt_l == 1 and band_l == 2:
+        if not band[0] < band[1]:
+            raise Exception("Illegal input of band.")
+        if not output:
+            output = input+'_'+str(kpt[0])+'_'+str(band[0])+'-'+str(band[1])+'_'+str(spin)+'.vasp'
+        if calc.system.hamiltonian.ispin == 1:
+            att = f"wavefunctions/{kpt[0] + 1}/field"
+        else:
+            if spin == 1:
+                att = f"wavefunctions/spin-up/{kpt[0] + 1}/field"
+            else:
+                att = f"wavefunctions/spin-down/{kpt[0] + 1}/field"
+        print("Reading *.h5 file ...")
+        filename = input+'.h5'
+        h = h5py.File(filename, mode="r")
+        print("Processing data ...")
+        fld = h[att][0:]
+        fld = np.transpose(fld, [i for i in range(fld.ndim - 1, -1, -1)])
+        fld = np.asfortranarray(fld)
+        fld = fld / ureg.bohr**1.5
+        fld = fld[::2, :] + 1j * fld[1::2, :]
+        fld.ito("angstrom ** -1.5")
+        if band[1] < fld.shape[-1]:
+            for i in range(band[0], band[1] + 1):
+                if i == band[0]:
+                    fld_i = fld[..., i].magnitude
+                else:
+                    fld_i += fld[..., i].magnitude
+            fld = fld_i
+        else:
+            raise Exception("The band is out of range in *.h5 file.")
+        f_abs = np.abs(fld)
+        f_div = np.where(np.abs(np.angle(fld)) < np.pi / 2, f_abs, -f_abs)
+        f_div = np.reshape(f_div, (f_div.shape[-1], -1), order='F').T
+    elif kpt_l == 2 and band_l == 2:
+        if not kpt[0] < kpt[1]:
+            raise Exception("Illegal input of kpt.")
+        if not band[0] < band[1]:
+            raise Exception("Illegal input of band.")
+        if not output:
+            output = input+'_'+str(kpt[0])+'-'+str(kpt[1])+'_'+str(band[0])+'-'+str(band[1])+'_'+str(spin)+'.vasp'
+        nkpts = kpt[1] - kpt[0] + 1
+        att = [''] * nkpts
+        for i in range(kpt[0], kpt[1] + 1):
+            if calc.system.hamiltonian.ispin == 1:
+                att[i] = f"wavefunctions/{i + 1}/field"
+            else:
+                if spin == 1:
+                    att[i] = f"wavefunctions/spin-up/{i + 1}/field"
+                else:
+                    att[i] = f"wavefunctions/spin-down/{i + 1}/field"
+        print("Reading *.h5 file ...")
+        filename = input+'.h5'
+        h = h5py.File(filename, mode="r")
+        print("Processing data ...")
+        for i in range(nkpts):
+            fld_i = h[att[i]][0:]
+            if i == 0:
+                fld = fld_i
+            else:
+                fld += fld_i
+        fld = np.transpose(fld, [i for i in range(fld.ndim - 1, -1, -1)])
+        fld = np.asfortranarray(fld)
+        fld = fld / ureg.bohr**1.5
+        fld = fld[::2, :] + 1j * fld[1::2, :]
+        fld.ito("angstrom ** -1.5")
+        if band[1] < fld.shape[-1]:
+            for i in range(band[0], band[1] + 1):
+                if i == band[0]:
+                    fld_i = fld[..., i].magnitude
+                else:
+                    fld_i += fld[..., i].magnitude
+            fld = fld_i
         else:
-            att = f"wavefunctions/spin-down/{kpt + 1}/field"
-    filename = input+'.h5'
-    h = h5py.File(filename, mode="r")
-    fld = h[att][0:]
-    fld = np.transpose(fld, [i for i in range(fld.ndim - 1, -1, -1)])
-    fld = np.asfortranarray(fld)
-    fld = fld / ureg.bohr**1.5
-    fld = fld[::2, :] + 1j * fld[1::2, :]
-    fld.ito("angstrom ** -1.5")
-    if band < fld.shape[-1]:
-        fld = fld[..., band].magnitude
+            raise Exception("The band is out of range in *.h5 file.")
+        f_abs = np.abs(fld)
+        f_div = np.where(np.abs(np.angle(fld)) < np.pi / 2, f_abs, -f_abs)
+        f_div = np.reshape(f_div, (f_div.shape[-1], -1), order='F').T
     else:
-        raise Exception("The band is out of range in *.h5 file.")
-    f_abs = np.abs(fld)
-    f_div = np.where(np.abs(np.angle(fld)) < np.pi / 2, f_abs, -f_abs)
-    f_div = np.reshape(f_div, (f_div.shape[-1], -1), order='F').T
+        raise Exception("Illegal input.")
+    print("Reading structure ...")
     pbc = [1, 1, 1]
     positions = calc.system.atoms.positions
     cell = calc.system.cell.avec
     elements_symbols = calc.system.atoms.get_labels()
     stp = ats(elements_symbols,positions=positions,cell=cell,pbc=pbc)
     grid = calc.system.cell.grid
+    print("Saving data to disk ...")
     write(output, stp, direct=True, vasp5=True)
     with open(output, "a") as f:
         f.writelines(['\n']+[str(i)+' ' for i in grid]+['\n'])
         np.savetxt(f, f_div)
```

## rescupybs/wrapper.py

```diff
@@ -177,22 +177,27 @@
     parser = argparse.ArgumentParser(description='Export the wavefunction isosurface for VESTA from rescuplus calculation result *.json and *.h5 files.',
                                      epilog='''
 Example:
 rescuiso -b 1 -k 0
 ''',
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument('-v', "--version", action="version", version="rescupybs "+__version__+" from "+os.path.dirname(__file__)+' (python'+platform.python_version()+')')
-    parser.add_argument('-i', "--input",   type=str,         nargs='+', default=[], help="export the wavefunction isosurface from .json and .h5 files")
+    parser.add_argument('-i', "--input",   type=str,         nargs='+', default=[],  help="export the wavefunction isosurface from .json and .h5 files")
     parser.add_argument('-o', "--output",  type=str,         help="wavefunction isosurface for VESTA format")
-    parser.add_argument('-k', "--kpt",     type=int,         default=0, help="The kpoint in wavefunctions")
-    parser.add_argument('-b', "--band",    type=int,         default=0, help="The band in wavefunctions")
+    parser.add_argument('-k', "--kpt",     type=int,         nargs='+', default=[0], help="The kpoint in wavefunctions")
+    parser.add_argument('-b', "--band",    type=int,         nargs='+', default=[0], help="The band in wavefunctions")
     parser.add_argument('-s', "--spin",    type=int,         default=1, help="The up or down spin in wavefunctions")
 
     args = parser.parse_args()
 
+    if args.kpt[0] < 0:
+        raise Exception("Illegal input of kpt.")
+    if args.band[0] < 0:
+        raise Exception("Illegal input of band.")
+
     if not args.input:
         input = ['nano_wvf_out']
         if not os.path.exists(input[0]+'.json') and not os.path.exists(input[0]+'.h5'):
             raise Exception("The input file does not exist.")
     else:
         input = [f.rsplit('_in',1)[0]+'_out.json' if f.rsplit('.',1)[0].endswith('in') else f for i in args.input for f in glob.glob(i)]
         input = [os.path.join(i,'nano_wvf_out.json') if os.path.isdir(i) else i for i in input]
```

## Comparing `rescupybs-0.0.1.4.1.dist-info/LICENSE` & `rescupybs-0.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rescupybs-0.0.1.4.1.dist-info/METADATA` & `rescupybs-0.1.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rescupybs
-Version: 0.0.1.4.1
+Version: 0.1.0
 Summary: Band structure plot from rescuplus json file.
 Home-page: https://github.com/lkccrr/rescupybs
 Author: kan
 Author-email: luokan@hrbeu.edu.cn
 License: MIT
 Keywords: DFT rescuplus band plot
 Platform: Unix
```

