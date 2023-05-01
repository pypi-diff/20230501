# Comparing `tmp/ztfidr-0.7.9.tar.gz` & `tmp/ztfidr-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ztfidr-0.7.9.tar", last modified: Fri Nov 11 13:43:13 2022, max compression
+gzip compressed data, was "ztfidr-0.8.1.tar", last modified: Mon May  1 19:23:50 2023, max compression
```

## Comparing `ztfidr-0.7.9.tar` & `ztfidr-0.8.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-11-11 13:43:13.874855 ztfidr-0.7.9/
--rwxrwxrwx   0 rigault   (2358) staff       (20)    11357 2022-04-07 08:06:46.000000 ztfidr-0.7.9/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      234 2022-11-11 13:43:13.874728 ztfidr-0.7.9/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)     2186 2022-04-30 12:26:28.000000 ztfidr-0.7.9/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)       38 2022-11-11 13:43:13.874897 ztfidr-0.7.9/setup.cfg
--rwxrwxrwx   0 rigault   (2358) staff       (20)      609 2022-11-11 13:42:57.000000 ztfidr-0.7.9/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-11-11 13:43:13.874070 ztfidr-0.7.9/ztfidr/
--rwxrwxrwx   0 rigault   (2358) staff       (20)      127 2022-11-11 13:42:53.000000 ztfidr-0.7.9/ztfidr/__init__.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    11147 2022-11-05 14:23:12.000000 ztfidr-0.7.9/ztfidr/io.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    21919 2022-10-13 13:52:33.000000 ztfidr-0.7.9/ztfidr/lightcurve.py
--rw-r--r--   0 rigault   (2358) staff       (20)    18659 2022-11-06 15:43:33.000000 ztfidr-0.7.9/ztfidr/linefitter.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     1893 2022-04-07 08:06:50.000000 ztfidr-0.7.9/ztfidr/salt2.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    24627 2022-11-11 13:41:50.000000 ztfidr-0.7.9/ztfidr/sample.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)      629 2022-05-02 15:53:23.000000 ztfidr-0.7.9/ztfidr/script.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)      950 2022-05-18 13:01:28.000000 ztfidr-0.7.9/ztfidr/snid.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    19194 2022-11-05 13:23:19.000000 ztfidr-0.7.9/ztfidr/spectroscopy.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    10144 2022-11-05 13:51:48.000000 ztfidr-0.7.9/ztfidr/target.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    18712 2022-11-10 08:58:11.000000 ztfidr-0.7.9/ztfidr/typing.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     1443 2022-04-07 08:06:50.000000 ztfidr-0.7.9/ztfidr/utils.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2022-11-11 13:43:13.874573 ztfidr-0.7.9/ztfidr.egg-info/
--rwxrwxrwx   0 rigault   (2358) staff       (20)      234 2022-11-11 13:43:13.000000 ztfidr-0.7.9/ztfidr.egg-info/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)      358 2022-11-11 13:43:13.000000 ztfidr-0.7.9/ztfidr.egg-info/SOURCES.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2022-11-11 13:43:13.000000 ztfidr-0.7.9/ztfidr.egg-info/dependency_links.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2022-11-11 13:43:13.000000 ztfidr-0.7.9/ztfidr.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-01 19:23:50.530709 ztfidr-0.8.1/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    11357 2022-04-07 08:06:46.000000 ztfidr-0.8.1/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      234 2023-05-01 19:23:50.530579 ztfidr-0.8.1/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     2186 2022-04-30 12:26:28.000000 ztfidr-0.8.1/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-05-01 19:23:50.530748 ztfidr-0.8.1/setup.cfg
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      609 2023-05-01 19:23:26.000000 ztfidr-0.8.1/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-01 19:23:50.529826 ztfidr-0.8.1/ztfidr/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      127 2023-05-01 19:23:31.000000 ztfidr-0.8.1/ztfidr/__init__.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    14133 2023-04-27 14:14:04.000000 ztfidr-0.8.1/ztfidr/io.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    22044 2023-03-20 14:23:14.000000 ztfidr-0.8.1/ztfidr/lightcurve.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    18659 2022-11-06 15:43:33.000000 ztfidr-0.8.1/ztfidr/linefitter.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     3199 2023-05-01 18:55:51.000000 ztfidr-0.8.1/ztfidr/plotting.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     1893 2022-04-07 08:06:50.000000 ztfidr-0.8.1/ztfidr/salt2.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    31042 2023-04-27 13:54:23.000000 ztfidr-0.8.1/ztfidr/sample.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      629 2022-05-02 15:53:23.000000 ztfidr-0.8.1/ztfidr/script.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      950 2022-05-18 13:01:28.000000 ztfidr-0.8.1/ztfidr/snid.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    20341 2022-11-15 12:56:31.000000 ztfidr-0.8.1/ztfidr/spectroscopy.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    10043 2022-11-19 14:22:02.000000 ztfidr-0.8.1/ztfidr/target.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    23607 2023-04-28 14:55:40.000000 ztfidr-0.8.1/ztfidr/typing.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     4034 2023-03-24 07:32:25.000000 ztfidr-0.8.1/ztfidr/utils.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-01 19:23:50.530430 ztfidr-0.8.1/ztfidr.egg-info/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      234 2023-05-01 19:23:50.000000 ztfidr-0.8.1/ztfidr.egg-info/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      377 2023-05-01 19:23:50.000000 ztfidr-0.8.1/ztfidr.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2023-05-01 19:23:50.000000 ztfidr-0.8.1/ztfidr.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2023-05-01 19:23:50.000000 ztfidr-0.8.1/ztfidr.egg-info/top_level.txt
```

### Comparing `ztfidr-0.7.9/LICENSE` & `ztfidr-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ztfidr-0.7.9/README.md` & `ztfidr-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `ztfidr-0.7.9/setup.py` & `ztfidr-0.8.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 from distutils.core import setup
 from setuptools import setup, find_packages
 
 
 packages = find_packages()
 
-VERSION = '0.7.9'
+VERSION = '0.8.1'
         
 setup(name='ztfidr',
       version=VERSION,
       description='Tools for ZTF Ia *Internal*DataReleases',
       author='Mickael Rigault',
       author_email='m.rigault@ipnl.in2p3.fr',
       url='https://github.com/MickaelRigault/ztfdr',
```

### Comparing `ztfidr-0.7.9/ztfidr/io.py` & `ztfidr-0.8.1/ztfidr/io.py`

 * *Files 15% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         return filepath
     
     return pandas.read_csv(filepath, **kwargs)
 
 def get_target_typing(load=True, index_col=0, sep=" ",
                           clean=True, **kwargs):
     """ """
-    filepath = os.path.join(IDR_PATH, "tables",
+    filepath = os.path.join(IDR_PATH, "tables/.dataset_creation/sample_def",
                             "ztfdr2_typing.csv")
     if not load:
         return filepath
     
     data = pandas.read_csv(filepath, index_col=index_col, sep=sep, **kwargs)
     if clean:
         data["typing"] = data["typing"].str.replace("[","", regex=False).str.replace("]","", regex=False).str.replace("'","") # clean
@@ -101,34 +101,98 @@
         return filepath
     
     data = pandas.read_csv(filepath, names=["ztfname"], **kwargs)
     return data["ztfname"].values.astype(str)
 
 
 # Redshifts
-def get_redshif_data(load=True, index_col=0, **kwargs):
+def get_redshif_data(load=True, index_col=0, full=False, **kwargs):
     """ """
     filepath = os.path.join(IDR_PATH, "tables",
                             "ztfdr2_redshifts.csv")
     if not load:
         return filepath
     
     data = pandas.read_csv(filepath, index_col=index_col, **kwargs)
     data.index.name = 'ztfname'
-    return data
 
+    if not full: # get only redshift and source
+        return data
+    
+    # or get them all:
+    redshift_dir = os.path.join(IDR_PATH, "tables", ".dataset_creation/redshifts")
+    redshifts = {}
+
+    
+    # Emission lines
+    sedm_em = pandas.read_csv(os.path.join(redshift_dir,
+                                            "specfile_sedm_emissionlines.csv"),
+                                  index_col=0)
+    sedm_em = sedm_em.set_index("ztfname")[["sedmredshift","sedmredshift_err"]].copy()#.rename("sedmredshift","sedm_em", axis=1)
+    sedm_em.columns = sedm_em.columns.str.replace("sedmredshift","sedm_em")
+    
+    
+    
+    nosedm_em = pandas.read_csv(os.path.join(redshift_dir,
+                                                    "specfile_nonsedm_emissionlines.csv"),
+                                     index_col=0)
+    nosedm_em = nosedm_em.set_index("ztfname")[["value","error"]].copy()#.rename("sedmredshift","sedm_em", axis=1)
+    nosedm_em.columns = ["nonsedm_em", "nonsedm_em_err"]
+    
+    # SNID
+    snidauto = pandas.read_csv(os.path.join(redshift_dir,
+                                                    "ztfdr2_snid_redshifts.csv"),
+                                     index_col=0)
+    snidauto.columns = snidauto.columns.str.replace("redshift","snidauto")
+    
+    # Host-Z
+    hostz = pandas.read_csv(os.path.join(redshift_dir,
+                                                    "ztfdr2_hostz_redshifts.csv"),
+                                     index_col=0)
+    hostz = hostz[["redshift"]]
+    hostz.columns = ["host_cat"]
+    hostz["host_cat_err"] = 1e-5
+
+
+    
+    # override
+    override = pandas.read_csv(os.path.join(redshift_dir,
+                                                    "ztfdr2_override_redshifts.csv"),
+                                     index_col=0)
+    override.columns = ["override"]
+
+    # merge them
+    
+    data = data.join(sedm_em, on="ztfname")
+    data = data.join(nosedm_em, on="ztfname")
+    data = data.join(snidauto, on="ztfname")
+    data = data.join(hostz, on="ztfname")
+    data = data.join(override, on="ztfname")
+    data
+    
+    return data
+    
 def get_snidauto_redshift(load=True, **kwargs):
     """ """
     filepath = os.path.join(IDR_PATH,"tables",
                                 ".dataset_creation/redshifts/ztfdr2_snid_redshifts.csv")
     if not load:
         return filepath
     
     return pandas.read_csv(filepath, index_col=0, **kwargs)
 
+def get_snidauto_specfile_redshift(load=True, **kwargs):
+    """ """
+    filepath = os.path.join(IDR_PATH,"tables",
+                                ".dataset_creation/redshifts/snidauto_ianorm.csv")
+    if not load:
+        return filepath
+    
+    return pandas.read_csv(filepath, index_col=0, **kwargs)
+
 # Coordinates
 def get_coords_data(load=True, index_col=0, **kwargs):
     """ """
     filepath = os.path.join(IDR_PATH, "tables",
                             "ztfdr2_coordinates.csv")
     if not load:
         return filepath
@@ -265,15 +329,16 @@
                             ".dataset_creation/sample_def/spec_class/autotyping.csv")
     if not load:
         return filepath
     return pandas.read_csv(filepath, index_col=index_col, **kwargs)
 
 
 def get_spectra_datafile(contains=None, startswith=None,
-                         snidres=False, extension=None, use_dask=False):
+                         snidres=False, extension=None, use_dask=False,
+                         add_phase=True, data=None):
     """ """
     from glob import glob
     glob_format = "*" if not startswith else f"{startswith}*"
     if snidres and extension is None:
         extension = "_snid.h5"
     elif extension is None:
         extension = ".ascii"
@@ -283,16 +348,28 @@
     if extension is not None:
         glob_format += f"{extension}"
 
     specfiles = glob(os.path.join(IDR_PATH, "spectra", glob_format))
     datafile = pandas.DataFrame(specfiles, columns=["fullpath"])
     datafile["basename"] = datafile["fullpath"].str.split(
         "/", expand=True).iloc[:, -1]
-
-    return pandas.concat([datafile, parse_filename(datafile["basename"], snidres=snidres)], axis=1)
+    
+    specfile = pandas.concat([datafile, parse_filename(datafile["basename"], snidres=snidres)], axis=1)
+    
+    if add_phase:
+        from astropy.time import Time
+        if data is None:
+            from .sample import get_sample
+            data = get_sample().data
+            
+        specfile["dateiso"] = Time(np.asarray(specfile["date"].apply(lambda x: f"{x[:4]}-{x[4:6]}-{x[6:]}"), dtype=str), format="iso").mjd
+        specfile = specfile.join(data["t0"], on="ztfname")
+        specfile["phase"] = specfile.pop("dateiso")-specfile.pop("t0")
+        
+    return specfile
 
 
 def parse_filename(file_s, snidres=False):
     """ file or list of files.
     Returns
     -------
     Serie if single file, DataFrame otherwise
```

### Comparing `ztfidr-0.7.9/ztfidr/lightcurve.py` & `ztfidr-0.8.1/ztfidr/lightcurve.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     # --------- #
     def load_salt2param(self):
         """ """
         targetname = self.targetname
         if targetname is None:
             warnings.warn("Unknown targetname (=None) ; use manually set_salt2param()")
             return None
+        
         from .salt2 import get_target_salt2param
         salt2param = get_target_salt2param(targetname)
         self.set_salt2param(salt2param)
         
     # --------- #
     #  SETTER   #
     # --------- #
@@ -119,15 +120,15 @@
         return get_saltmodel(**self.salt2param.rename({"redshift":"z"}
                                                      )[["z","t0","x0","x1","c",
                                                         "mwebv"]].to_dict()
                             )
     def get_lcdata(self, zp=None, in_mjdrange=None,
                        min_detection=None,
                        filters=None,
-                       flagout=[1,2,4,8,256]):
+                       flagout=[1,2,4,8,16]):
         """ 
         filters: [string, None or list]
             list of filters 
             - None/'*' or 'all': no filter selection/
             - string: just this filter (e.g. 'p48g')
             - list of string: just these filters (e.g. ['p48g','p48r'])
 
@@ -143,14 +144,15 @@
             64: fieldid>879: Recommended IPAC cut 
             128: moonilf>0.5: Recommended IPAC cut 
             256: has_baseline>1: Has a valid baseline correction 
             512: airmass>2: Recommended IPAC cut 
             1024: flux/flux_err>=5: Nominal detection
 
         """
+        from .utils import flux_to_mag
 
         if flagout in ["all","any","*"]:
             data = self.data[self.data["flag"]==0]
             
         if flagout in ["all","any","*"]:
             data = self.data[self.data["flag"]==0]
         elif flagout is None:
@@ -168,18 +170,21 @@
 
             
         flux  = data["flux"] * coef
         error = data["flux_err"] * coef
         detection = flux/error
             
         
-        lcdata = data[["mjd","mag","mag_err","filter","field_id","x_pos","y_pos", "flag","mag_lim"]]
-        additional = pandas.DataFrame(np.asarray([zp, flux,error, detection]).T,
+        lcdata = data[["mjd","mag","mag_err","filter","field_id","x_pos","y_pos", "flag"]]
+        additional = pandas.DataFrame(np.asarray([zp, flux, error, detection]).T,
                                          columns=["zp", "flux", "error", "detection"],
                                          index=lcdata.index)
+        
+        additional["mag_lim"], _ = flux_to_mag(error*5, None, zp=zp)
+        
         lcdata = pandas.merge(lcdata, additional, left_index=True, right_index=True)
 #        lcdata.loc["zp",:] = zp
 #        lcdata["flux"] = flux
 #        lcdata["error"] = error
 #        lcdata["detection"] = detection
         lcdata["filter"] = lcdata["filter"].replace("ztfg","p48g").replace("ztfr","p48r").replace("ztfi","p48i")
```

### Comparing `ztfidr-0.7.9/ztfidr/linefitter.py` & `ztfidr-0.8.1/ztfidr/linefitter.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.7.9/ztfidr/salt2.py` & `ztfidr-0.8.1/ztfidr/salt2.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.7.9/ztfidr/sample.py` & `ztfidr-0.8.1/ztfidr/sample.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,32 +7,39 @@
         
 def get_sample(**kwargs):
     """ Short to to Sample.load() """
     return Sample.load(**kwargs)
 
 
 class Sample():
+
+    NON_IA_CLASSIFICATIONS = ["nonia","ib/c","unclear","confusing"]
     
     def __init__(self, data=None):
         """ """
         self.set_data(data)
     
     @classmethod
-    def load(cls, redshift_range=None, target_list=None, has_spectra=True):
+    def load(cls, redshift_range=None, target_list=None, has_spectra=True,
+                 rm_nonia=False):
         """ Load a Sample instance building it from io.get_targets_data() """
         data = io.get_targets_data()
+        
         if redshift_range is not None:
             data = data[data["redshift"].between(*redshift_range)]
 
         if target_list is not None:
             data = data.loc[target_list]
 
         if has_spectra:
-            specfile = io.get_spectra_datafile()
+            specfile = io.get_spectra_datafile(data=data)
             data = data[data.index.isin(specfile["ztfname"])]
+
+        if rm_nonia:
+            data = data[~data["classification"].isin(cls.NON_IA_CLASSIFICATIONS)]
             
         return cls(data=data)
 
     # ------- #
     # LOADER  #
     # ------- #
     def load_hostdata(self):
@@ -121,15 +128,19 @@
     # SETTER  #
     # ------- #
     def set_data(self, data):
         """ attach to this instance the target data. 
         = Most likely you should not use this method directly. =
         use sample = Sample.load()
         """
-        data["t0day"] = data["t0"].astype("int")
+        try:
+            data["t0day"] = data["t0"].astype("int")
+        except:
+            data["t0day"] = data["t0"]
+            
         self._data = data
 
     def set_hostdata(self, hostdata):
         """ attach to this instance the host data.
         = Most likely you should not use this method directly. =
         use sample.load_hostdata() or simply 
         sample.hostdata that automatically load this corrent hostdata.
@@ -270,14 +281,28 @@
 
         # Additional Query
         if query:
             data = data.query(query)
             
         return data
 
+    def get_ianorm(self, incl_snia=False):
+        """ get the list targets that are ia-norm or ia(-norm) (or sn ia if incl_snia=True)
+        
+        Returns
+        -------
+        array
+            list of targetname (data.index)
+        """
+        classifications = ["ia-norm","ia(-norm)"]
+        if incl_snia:
+            classifications += ["sn ia"]
+            
+        return np.asarray(self.data[self.data["classification"].isin(classifications)].index)
+    
     # Target | High level
     def get_target(self, name):
         """ """
         from . import target
         lightcurve = self.get_target_lightcurve(name)
         spectra = self.get_target_spectra(name, as_spectra=False)
         meta = self.data.loc[name]
@@ -296,34 +321,34 @@
         return spectroscopy.Spectrum.from_name(name, **kwargs)
 
     # Extra
     def get_goodcoverage_targets(self,
                                      n_early_bands=">=2",
                                      n_late_bands=">=2",
                                        n_points=">=7",
-                                       premax_range=[-15,0],
-                                       postmax_range=[0,30],
-                                       phase_range=[-15,30],
+                                       premax_range=[-20,0],
+                                       postmax_range=[0,40],
+                                       phase_range=[-20,30],
                                        **kwargs):
         """ kwargs should have the same format as the n_early_point='>=2' for instance.
         None means no constrain, like n_bands=None means 'n_bands' is not considered.
         """
         query = {**dict(n_early_bands=n_early_bands, n_late_bands=n_late_bands,
                         n_points=n_points),
                  **kwargs}
         df_query = " and ".join([f"{k}{v}" for k,v in query.items() if v is not None])
         phase_coverage = self.get_phase_coverage(premax_range=premax_range,
                                                  postmax_range=postmax_range,
                                                  phase_range=phase_range)
         return phase_coverage.query(df_query).index.astype("string")
 
     
-    def get_phase_coverage(self,premax_range=[-15,0],
-                                postmax_range=[0,30],
-                                phase_range=[-15,30], min_det_perband=1):
+    def get_phase_coverage(self,premax_range=[-20,0],
+                                postmax_range=[0,40],
+                                phase_range=[-20,40], min_det_perband=1):
         """ """        
         # All
         phases = self.phase_df[self.phase_df.between(*phase_range)].reset_index().rename({"level_0":"name"},axis=1)
         n_points = phases.groupby(["name"]).size().to_frame("n_points")
         n_bands = (phases.groupby(["name", "filter"]).size()>=min_det_perband
                         ).groupby(level=[0]).sum().to_frame("n_bands")
         # Pre-Max
@@ -603,14 +628,163 @@
         [ax.spines[which].set_visible(False) for which in clearwhich]
 
     #        ax.set_title("ZTF-1 Ia Statistics")
         ax.set_ylabel("Number of Type Ia Supernovae")
         ax.set_ylim(bottom=0)
         ax.tick_params("y", labelsize="small")
         return fig
+
+
+    def show_npoints_distribution_perband(self, phase_coverage=[-20, 40],
+                                                ax=None, clearaxes=True,
+                                          add_pantheon=True):
+        """ """
+        phase_cov = self.get_phase_coverage( premax_range=[phase_coverage[0], 0],
+                                               postmax_range=[0, phase_coverage[1]],
+                                               phase_range=phase_coverage,)
+
+
+        from matplotlib.colors import to_rgba
+        if ax is None:
+            import matplotlib.pyplot as plt
+            fig = plt.figure(figsize=[7, 4.5])
+            axb = fig.add_axes([0.08, 0.15, 0.87, 0.35])
+            axt = fig.add_axes([0.08, 0.6, 0.87, 0.35])
+
+        else:
+            fig = ax.figure
+            axb, axt = fig.axew
+
+        prop = dict(bins=np.logspace(0,3, 15), density=False, log=False)
+
+        # -------------
+        weights = np.ones(len(phase_cov))*1
+        axt.hist(phase_cov["n_early_points_p48g"]+phase_cov["n_late_points_p48g"], histtype="step", 
+                fill=True, 
+                edgecolor=to_rgba("tab:green", 1), lw=1., ls="--",
+                facecolor=to_rgba("tab:green", 0.05), 
+                label=f"ztf:g", weights=weights,
+                zorder=2, **prop)
+
+        axt.hist(phase_cov["n_early_points_p48r"]+phase_cov["n_late_points_p48r"], histtype="step", 
+                fill=True, 
+                edgecolor=to_rgba("tab:red", 1), lw=1., ls="-",
+                facecolor=to_rgba("tab:red", 0.05), 
+                label=f"ztf:r",weights=weights,
+                zorder=3, **prop)
+
+        axt.hist(phase_cov["n_early_points_p48i"]+phase_cov["n_late_points_p48i"], histtype="step", 
+                fill=True, 
+                edgecolor=to_rgba("tab:orange", 1), lw=1., ls=":",
+                facecolor=to_rgba("tab:orange", 0.05), 
+                label=f"ztf:i",weights=weights,
+                zorder=5, **prop)
+
+
+        # --------------
+        weights = np.ones(len(phase_cov))*1
+
+        axb.hist(phase_cov["n_points"], histtype="step", color="k", lw=1.5,
+                label=f"any phase",
+                weights=weights,
+                zorder=5, **prop)
+
+        axb.hist(phase_cov["n_early_points"], histtype="step", 
+                fill=True, 
+                edgecolor=to_rgba("0.5", 1), lw=1., ls="-",
+                facecolor=to_rgba("0.5", 0.), 
+                label="pre-max",
+                weights=weights,            
+                zorder=3, **prop)
+
+        axb.hist(phase_cov["n_late_points"], histtype="step", 
+                fill=True, 
+                edgecolor=to_rgba("0.5", 1), lw=0., 
+                facecolor=to_rgba("0.5", 0.3), 
+                label="post-max",
+                weights=weights,
+                zorder=4, **prop)
+
+        # --------------
+
+        axb.set_xlabel("number of detected point", fontsize="large")
+        axb.set_xscale("log")
+        axt.set_xscale("log")
+
+        if clearaxes:
+            clearwhich = ["left","right","top"] # "bottom"
+            for ax in [axb, axt]:
+                [ax.spines[which].set_visible(False) for which in clearwhich]
+                ax.tick_params(axis="y", labelsize="small", 
+                           labelcolor="0.5", color="0.5")
+
+        axt.legend(fontsize="medium", frameon=False)#, loc="upper left")
+        axb.legend(fontsize="medium", frameon=False)
+
+        axt.set_xlim(*axb.get_xlim())
+        return fig
+
+
+    def show_firstdet_distributions(self, ax=None, restrict_to=[-25,60]):
+        """ """
+        phases = self.phase_df[self.phase_df.between(*restrict_to)]
+        goodlc = self.get_goodcoverage_targets()
+
+        from matplotlib.colors import to_rgba
+        if ax is None:
+            import matplotlib.pyplot as plt
+            fig = plt.figure(figsize=[7, 2.5])
+            ax = fig.add_axes([0.08, 0.1, 0.87, 0.8])
+        else:
+            fig = ax.figure
+
+        first_det_per_band = phases.groupby(level=[0,1]).min()
+        first_det = first_det_per_band.unstack().min(axis=1)
+
+        prop = dict(range=[-21,30], bins=50, histtype="step", fill=True)
+
+        # ---- Any band
+
+        _ = ax.hist(first_det, facecolor="None", zorder=5,
+                    color="k", label="all Type Ia", **prop)
+
+        _ = ax.hist(first_det.loc[goodlc], zorder=4,
+                    facecolor="0.7", lw=0,
+                     label="good sampling", **prop)
+        # ---- Per filter
+
+        #ax.legend(frameon=False)
+
+        for band, color, label in zip(["p48g","p48r","p48i"],
+                              ["tab:green","tab:red","tab:orange"],
+                              ["ztf:g","ztf:r","ztf:i"]):
+            band_fdet = first_det_per_band.xs(band, level=1)
+            band_fdet_good = band_fdet.loc[band_fdet.index.isin(goodlc)]
+
+
+            _ = ax.hist(band_fdet_good, 
+                        facecolor=to_rgba(color, 0.0), #zorder=2,
+                        edgecolor=color,
+                        weights = np.ones(len(band_fdet_good))*-1, 
+                        label=label, **prop)
+
+        ax.spines["bottom"].set_position(('data',0))
+        ax.spines["bottom"].set_zorder(10)
+
+        clearwhich = ["left","right","top"] # "bottom"
+        [ax.spines[which].set_visible(False) for which in clearwhich]
+        ax.tick_params(axis="y", labelsize="small", 
+                   labelcolor="0.5", color="0.5")
+        ax.tick_params(axis="x", pad=2, zorder=10)
+        ax.set_xlabel("First detection phase [days]", loc="right")
+
+
+        #ax.legend(["all", "good"], frameon=False)
+        ax.legend(frameon=False, ncol=3)
+        return fig
         
     # =============== #
     #   Properties    #
     # =============== #
     @property
     def data(self):
         """ """
```

### Comparing `ztfidr-0.7.9/ztfidr/script.py` & `ztfidr-0.8.1/ztfidr/script.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.7.9/ztfidr/snid.py` & `ztfidr-0.8.1/ztfidr/snid.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.7.9/ztfidr/spectroscopy.py` & `ztfidr-0.8.1/ztfidr/spectroscopy.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,53 @@
 
 def get_target_spectra(name, load_snidres=True, **kwargs):
     """ load the lightcurve object for the given target. """
     return np.atleast_1d(Spectrum.from_name(name, load_snidres=load_snidres,
                                             **kwargs)
                         )
 
+
+def get_heliocentric_correction(ra, dec, time, site, tformat=None):
+    """ get the observer frame to helio centric correction (in km/s) 
+    
+    See astropy.coordinates.SkyCoord.radial_velocity_correction
+    from https://docs.astropy.org/en/stable/api/astropy.coordinates.SkyCoord.html
+
+    Parameters
+    ----------
+    ra, dec: float or array
+        coordinates in degree
+
+    time: float or array
+        when the observation was taken. Inputs astropy.time.Time
+
+    tformat: str
+        format of the input time (goes to format option of astropy.time.Time)
+
+    site: str
+        observatory location, e.g. 'palomar'. 
+        goes to astropy's EarthLocation.of_site(site)
+
+    Returns
+    -------
+    float or array
+        heliocentric correction in km/s
+    """
+    from astropy.time import Time
+    from astropy.coordinates import SkyCoord, EarthLocation
+    
+    observatory = EarthLocation.of_site(site)
+    sc = SkyCoord(ra, dec, unit="deg")
+    obstime = Time(time, format=tformat)
+    heliocorr = sc.radial_velocity_correction(kind="heliocentric", obstime=obstime, location=observatory).to("km/s").value
+    return heliocorr
+
+
+
+
 def read_spectrum(file_, sep=None):
     """ """
     data = open(file_).read().splitlines()
     try:
         header = pandas.DataFrame([d.replace("#","").replace(":"," ").replace("=","").split()[:2] for d in data 
                                    if (d.startswith("#") or "=" in d or ":" in d) and len(d.split())>=2],
                               columns=["keys", "values"]).set_index("keys")["values"]
```

### Comparing `ztfidr-0.7.9/ztfidr/target.py` & `ztfidr-0.8.1/ztfidr/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,30 +95,29 @@
                       "subtype": "unclear",
                       "p(subtype|type)":np.NaN
                      }
         return pandas.Series(typing)[['type', 'subtype', 'p(type)', 'p(subtype|type)']]
         return df_types
 
     def fit_snid(self, delta_phase=5, lbda_range=[4000, 8000],
-                       redshift_source=['host_cat', 'override', 'ha_nii'],
-                       set_it=True,
+                     redshift=None, set_it=True, use_phase=True,
                      **kwargs):
         """ fit SNID constraining redshift and phase """
 
         # Redshift input
-        redshift, source = self.get_redshift()
-        if redshift_source is None or source not in redshift_source:
-            redshift = None
-
         # Phase
         snidres = []
         for spec_ in np.atleast_1d(self.spectra):
-            phase = spec_.get_phase( self.meta["t0"] )
+            if use_phase:
+                phase = spec_.get_phase( self.meta["t0"] )
+            else:
+                phase = None
+                
             snidres_ = spec_.fit_snid(phase=phase, redshift=redshift,
-                                          delta_phase=delta_phase, lbda_range=lbda_range)
+                                      delta_phase=delta_phase, lbda_range=lbda_range)
             if set_it:
                 spec_.set_snidresult(snidres_)
             
             snidres.append(snidres_)
             
         return snidres[0] if not self.has_multiple_spectra() else snidres
```

### Comparing `ztfidr-0.7.9/ztfidr/typing.py` & `ztfidr-0.8.1/ztfidr/typing.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,70 +25,116 @@
     if len(typings)  == 1:
         return typings[0]
     
     ltypings = list(typings)
     ltypings.sort(key = lambda i: sort_favored.index(i))
     return ltypings[0]
 
+def get_specs_to_rm():
+    """ get the list of spectra flaged as 'to remove' in the typingapp """
+    report = Reports()
+    rmspec_serie = report.data[(report.data["value"].str.startswith("spec:rm")) &
+                               (~report.data["value"].str.contains("none_left"))]
+    rmspecs = np.asarray(rmspec_serie["value"].str.replace("spec:rm:","").values, dtype=str)
+    return rmspecs
 
 
+
+def merge_classifications(line):
+    """ """
+    # First arbiter
+    if line.arbiter_classification is not np.NaN:
+        return line.arbiter_classification, 'arbiter'
+    # Second master    
+    elif line.master_classification not in ["unclear", "None"]:
+        return line.master_classification, 'master'
+    # Final, auto    
+    return line.auto_classification, "auto"
+
 def parse_classification(line, 
                          min_review=2,
                          min_autotyping=3, 
                          min_generic_typing=3,
                          unclear_limit=0.5,
                          to_unclear_limit=0.75,
                          min_classifications_to_unclear=6,
-                         verbose=False):
+                         verbose=False, add_origin=False, skipsave=False):
     """ """
     classification = "confusing"
+
     if verbose:
         print(line)
         print(line["typing"])
         print("unclear" in line["typing"])
+        
     # not enough review, pass
     if line.nreviews <= min_review: # not enough
         if verbose:
             print("not enough classification")
         classification = "None"
+        level = 0
         
+    # Level 1
     # easy, all the same 
     elif line.ntypes == 1 and line.ntypings[0] >= min_autotyping:
         if verbose:
             print("all the same")
         classification =  line.typing[0]
-
+        level = 1
     # special save for ia-norm cases.
-        
+
+    # Level 2    
     # enough for generic, let's see if it's sufficient.        
     elif line.nreviews >= min_generic_typing:
         if verbose:
             print("enough for generic review")
+            
         # go back to the easy-case
         if "ia-norm" in line.typing and np.all([k in ["ia-norm", "sn ia", "unclear"] for k in line.typing]) \
           and line.ntypings[ list(line.typing).index("ia-norm") ] >= min_autotyping:
             classification = "ia-norm"
             
         # It looks like a Ia ir Ia-norm
         elif np.all([k in ["ia-norm", "sn ia"] for k in line.typing]):
-            classification = "ia_or_ianorm"
+            classification = "ia(-norm)"
             
         # Typing ok, Sub-tyiping not            
         elif np.all(['ia' in k and "not ia" not in k for k in line.typing]):
-            classification = "ia"
+            classification = "ia(-?)"
             
         # all non-ia ?
-        elif np.all([k in Classifications._NONIA_CASES for k in line.typing]):
+        elif np.all([k in Classifications.NONIA_KEY for k in line.typing]):
             classification = "nonia"
+            
         else:
             classification = "confusing"
+
+        level = 2
+    else:
+        level = -1
+
+
+    # Level 3            
+    # saving unclears if possible
+    # try to save remaining confusing cases
+    if classification == "ia(-?)" and not skipsave:
+        # remove generic cases
+        new_line = clear_line(line.copy(), ["unclear", "sn ia"])
+        classification, _ = parse_classification(new_line, skipsave=True)
+        # Could not be saved:
+        if classification in ["None", "unclear", "confusing","ia(-?)"]:
+            classification = "ia(-?)"
+        else:
+            if verbose:
+                print(f"ia(-?) classification became {classification}")
             
+    # Level 3            
     # saving unclears if possible
     # try to save remaining confusing cases
-    if classification == "confusing" and "unclear" in line["typing"]:
+    elif classification == "confusing" and "unclear" in line["typing"]:
         
         if verbose:
             print("trying to save confusing cases")
             print("unclear" in line["typing"])
             
         info = dict(zip(line["typing"],line["ntypings"]))
         n_unclears = info["unclear"] 
@@ -100,43 +146,86 @@
             print(f"fraction of confusing: {f_unclear}" )
             
         # more than 4 classification agreed when unclear discarded.
         if f_unclear <= unclear_limit and n_not >=min_generic_typing:
             if verbose:
                 print(f"saving this case" )
 
-            new_line = clear_unclear(line.copy())
-            classification = parse_classification(new_line)
+            new_line = clear_line(line.copy())
+            classification, _ = parse_classification(new_line)
 
         # At least 6 classification and more than 4 (if to_unclear_limit==0.75) are 'unclear'
         elif f_unclear >= to_unclear_limit and n_classifications >= min_classifications_to_unclear:
             if verbose:
                 print(f"saving this case as 'unclear' ")
             classification = "unclear"
         elif n_not <= min_review:
             if verbose:
                 print(f"saving this case as 'None' ")
             classification = "None"
             
         if verbose:
             print(f"cannot save this case ( {f_unclear} > {to_unclear_limit} & {n_classifications}>{n_classifications}")
 
-    return classification
+        level = 3
+
+    # Back to saving the rest:
+    if classification == "None":
+        if line.nreviews >= 2:
+            # 2 unclears or more
+            if np.all([k in ["unclear"] for k in line.typing]):
+                classification = "unclear"
+                if verbose:
+                    print(f"saving None to {classification}")
+                
+            else:
+                line = clear_line(line, "unclear")
+                # still have 2 or more entries
+                if line.nreviews >= 2:
+                    # No ?
+                    # let's remove the unclear then, and let's see:
+                    line = clear_line(line, "unclear")
+                    # All the same
+                    if line.ntypes == 1:
+                        classification =  line.typing[0]
+                        if verbose:
+                            print(f"saving None to {classification}")
+                
+                    elif np.all([k in ["ia-norm", "sn ia"] for k in line.typing]):
+                        classification = "ia(-norm)"
+                        if verbose:                        
+                            print(f"saving None to {classification}")
+                
+                    elif np.all([k in ["unclear"] for k in line.typing]):
+                        classification = "unclear"
+                        if verbose:                        
+                            print(f"saving None to {classification}")
+                
+                    elif np.all(['ia' in k and "not ia" not in k for k in line.typing]):
+                        classification = "ia(-?)"
+                        if verbose:
+                            print(f"saving None to {classification}")
+                
+    return classification, level
 
 
-def clear_unclear(line):
+def clear_line(line, rm_value="unclear"):
     """ remove the 'unclear' component from the given typing row """
     typing = list(line.typing)
-    if "unclear" not in typing:
-        return line # nothing to do
+#    if "unclear" not in typing:
+#        return line # nothing to do
     
     ntypings = list(line.ntypings)
-    index_unclear = typing.index("unclear")
-    typing.pop(index_unclear)
-    ntypings.pop(index_unclear)
+    for value in np.atleast_1d(rm_value):
+        if value not in typing:
+            continue
+        index_unclear = typing.index(value)
+        typing.pop(index_unclear)
+        ntypings.pop(index_unclear)
+        
     return pandas.Series({"typing": typing,
                           "ntypings": ntypings,
                           "ntypes": len(ntypings),
                           "nreviews": np.sum(ntypings)})
 
 
 class _DBApp_():
@@ -188,114 +277,144 @@
 class Reports( _DBApp_ ):
     _DB_NAME = "Classifications"
     
     def load(self):
         """ """
         self._data = self.data_from_db(sql="where kind='report'")
 
+    @classmethod
+    def get_arbiters(cls, prefix="arbiter_"):
+        """ """
+        report = cls()
+        dataarbiter = report.data[ report.data["value"].str.startswith("arbiter") ].copy()
+        dataarbiter[f"{prefix}classification"] = dataarbiter["value"].str.replace("arbiter:","")
+        a = dataarbiter["arbiter_classification"
+                       ].str.replace("^ia","ia-", regex=True
+                            ).replace("gal","nonia",regex=False
+                            ).replace("snia","sn ia",regex=False
+                            ).replace("notia","nonia",regex=False
+                            ).replace("ibc","ib/c",regex=False) # self consistency
+        a[a=="ia-"] = "sn ia"
+        dataarbiter["arbiter_classification"] = a.copy()
+        
+        return dataarbiter
+        
+    
 # =================== #
 #                     #
 #  CLASSIFICATIONS    #
 #                     #
 # =================== #
 class Classifications( _DBApp_ ):
     _DB_NAME = "Classifications"
-    _NONIA_CASES = ["not ia", "ii","ib/c","gal","other"]
-
+    
     MASTER_USER = ["jesper", "Joel Johansson", "Kate Maguire",
                    "Mathew Smith", "Umut", "Georgios Dimitriadis"]
 
+    NONIA_KEY = ["not ia", "ii","ib/c","gal","other", "nonia"]
+    IA_PEC_KEY = ["ia-91bg","ia-91t","ia-other"]
+    CLASSIFIED_KEY = ["ia-norm", "ia-pec", "ia(-?)", "sn ia", "ia(-norm)"]
+    
 
-    CLASSIFIED_KEY = ["ia-norm", "ia-pec", "ia", "sn ia", "ia_or_ianorm"]
-    IA_PEC = ["ia-91bg","ia-91t","ia-other"]
+    def __init__(self, in_targetlist=None):
+        """ """
+        _ = super().__init__()
         
+        if in_targetlist is not None:
+            self._data = self._data[self._data["target_name"].isin(in_targetlist)]
+            self._targetlist = self.data["target_name"].unique()
+        else:
+            self._targetlist = io.get_masterlist()
+            
+    
     def load(self):
         """ """
         self._data = self.data_from_db(sql="where kind='typing'")
         self._data["value"] = self._data["value"].str.strip().str.lower()
 
     def load_sample(self):
         """ """
         from . import get_sample
         self._sample = get_sample()
 
-    def store_typing(self, **kwargs):
+    def get_typing(self, **kwargs):
         """ """
         if "classification" not in self.data:
             self.load_classification(**kwargs)
             
         data = self.get_classification_df()
         classification = self.data.groupby("target_name").first()["classification"]
         data = data.join(classification)
+        return data
+    
+    def store_typing(self, **kwargs):
+        """ """
+        data = self.get_typing(**kwargs)
         return data.to_csv( io.get_target_typing(False), sep=" ")
         
 
-    def load_classification(self, min_review=2,
+    def load_classification(self, **kwargs):
+        """ """
+        classifications = self.get_classification(**kwargs)
+        self._data = self.data.join(classifications, on="target_name", how="outer")
+        
+    def get_classification(self, min_review=2,
                                   min_autotyping=3,
                                   min_generic_typing=3,
                                 # Master keys
                                   min_review_master=1,
                                   min_autotyping_master=2,
                                   min_generic_typing_master=3):
         """ """
-        self._load_classification(min_review=min_review, min_autotyping=min_autotyping,
-                                  min_generic_typing=min_generic_typing)
-        # master
-        master = self.get_masterclassification(False)
-        master._load_classification(min_review=min_review_master, min_autotyping=min_autotyping_master,
-                                  min_generic_typing=min_generic_typing_master)
-        
-        # master successful classifications
-        mdata = master.data[~master.data["classification"].isin(["None","confusing"])
-                            ].groupby("target_name").first()["classification"]
-        mdata.name = "master_classification"
-
+        # All auto | default
+        auto_data = self._get_classification(prefix="auto_",
+                                                 min_review=2, min_autotyping=3, min_generic_typing=3)
+
+        # Masters
+        master = self.get_masterclassification(incl_unclear=False) # do not consider unclear's input
+        master_data = master._get_classification(prefix="master_",
+                                                      min_review=min_review_master, min_autotyping=min_autotyping_master,
+                                                      min_generic_typing=min_generic_typing_master)
+        # do not consider master's None or confusing. Only final classification
+        master_data = master_data[~master_data["master_classification"].isin(["None","confusing"])]
 
         # Arbiter
-        report = Reports()
-        dataarbiter = report.data[report.data["value"].str.startswith("arbiter")].copy()
-        dataarbiter["arbiter_classification"] = dataarbiter["value"].str.replace("arbiter:","")
-        a = dataarbiter["arbiter_classification"].str.replace("^ia","ia-", regex=True).replace("gal","nonia",regex=False)
-        a[a=="ia-"] = "ia"
-        dataarbiter["arbiter_classification"] = a.copy()
-        # cleaning naming conventio
-        # This has target_name as index
-        adata = dataarbiter.groupby("target_name")["arbiter_classification"].first() # early issue, all agree, tested
-        
+        arbiter_data = Reports.get_arbiters(prefix="arbiter_").groupby("target_name").last()[["arbiter_classification"]] # [[ to get a dataframe
+        # - force in data list
+        arbiter_data = arbiter_data.loc[ arbiter_data.index.isin(self.target_list) ]
+
         #
-        # merging
+        # Now let's join
         #
-        data = self.data.set_index("target_name") # target_name as index
-        datamerged = data.join(mdata).join(adata).reset_index()
-        datamerged["auto_classification"] = datamerged["classification"]
-        # merge master
-        mclassified = datamerged[~datamerged["master_classification"].isna()]["master_classification"]
-        datamerged.loc[mclassified.index, "classification"] = mclassified
+        # - Default
+        cdata = pandas.DataFrame(auto_data["auto_classification"].values, index=auto_data.index, columns=["classification"])
+        cdata["class_origin"] = "auto"
+        cdata = cdata.join(auto_data)
 
-        # merge arbiter
-        aclassified = datamerged[~datamerged["arbiter_classification"].isna()]["arbiter_classification"]
-        datamerged.loc[aclassified.index, "classification"] = aclassified
+        # make sure it is full master list
         
-        self._data = datamerged
+        # - add master
+        cdata.loc[master_data.index, "classification"] = master_data["master_classification"]
+        cdata.loc[master_data.index, "class_origin"] = "master"
+        cdata = cdata.join(master_data)
+
+        # - add arbiter
+        cdata.loc[arbiter_data.index, "classification"] = arbiter_data["arbiter_classification"]
+        cdata.loc[arbiter_data.index, "class_origin"] = "arbiter"
+        cdata = cdata.join(arbiter_data)
+
+        return cdata
         
         
-    def _load_classification(self, **kwargs):
+    def _get_classification(self, prefix="", **kwargs):
         # Normal
         class_df = self.get_classification_df()
-        class_df["classification"] = class_df.apply(parse_classification, axis=1,
-                                                    **kwargs)
-
-        # are you reloading ?
-        if "classification" in self.data:
-            _ = self.data.pop("classification")
-            
-        self._data = self.data.set_index("target_name").join(class_df["classification"]).reset_index()
-
-
-        
+        d_ = pandas.DataFrame(class_df.apply(parse_classification, axis=1, **kwargs).to_list(),
+                                columns=[f"{prefix}classification",f"{prefix}clevel"], index=class_df.index)
+        return d_.reindex(list(self.target_list))
     # -------- #
     # GETTER   #
     # -------- #
     def get_masterclassification(self, incl_unclear=True):
         """ """
         this = self.__class__()
         MASTER_ID = _Users_().data.set_index("name").loc[self.MASTER_USER]["id"].values
@@ -396,15 +515,15 @@
     
     def get_of_types(self, types):
         """ get entry associated to the given type (lower case) """
         return 
                          
     def get_nonia(self, incl_unclear=False):
         """ """
-        list_to_get = self._NONIA_CASES.copy()
+        list_to_get = self.NONIA_KEY.copy()
         if incl_unclear:
             list_to_get+="unclear"
             
         return self.data[self.data["value"].isin(list_to_get)]
 
     def get_classification_df(self):
         """ """
@@ -418,46 +537,47 @@
     
     # -------- #
     # PLOTTER  #
     # -------- #
     def show_classification_stats(self, explode = 0.1,
                                   based_on = "classification", 
                                   redshift_range = None, dataprop = {},
+                                  startangle_main=90, startangle_sub=0,
                                   **kwargs):
         """ """
         import matplotlib.pyplot as plt
         
         prop_general = {**dict(wedgeprops=dict(width=1, edgecolor='0.7', linewidth=0.2)), 
                 **kwargs}
 
 
         class_stat = self.get_classification_stats( based_on, redshift_range=redshift_range,
                                                     **dataprop)
 
-        class_stat["ia-pec"] = class_stat[self.IA_PEC].sum()
-        class_stat["classified"] = class_stat[self.CLASSIFIED_KEY].sum()
-        class_stat["non ia"] = class_stat[[k for k in self._NONIA_CASES if k in class_stat]].sum()
-
+        class_stat["ia-pec"] = class_stat[self.IA_PEC_KEY].sum()
+        class_stat["Type Ia"] = class_stat[self.CLASSIFIED_KEY].sum()
+        class_stat["non ia"] = class_stat[[k for k in self.NONIA_KEY if k in class_stat]].sum()
+        print(class_stat["non ia"])
         # showing plots
 
 
         fig = plt.figure(figsize=[9,4])
         ax_main = fig.add_axes([0.05,0.15,0.4,0.8])
         ax_sub = fig.add_axes([0.52,0.15,0.4,0.8])
 
         # -> Main plot
-        to_show = ["None","confusing", "unclear", "classified", "non ia"]
+        to_show = ["None","confusing", "unclear", "Type Ia", "non ia"]
         data_show = class_stat[to_show]
         if type(explode) == float:
             explode = np.full_like(data_show.values, explode, dtype="float")
 
         colors = ["w","0.8", plt.cm.bone(0.3),  plt.cm.bone(0.7),
                   "tab:brown"]
         prop = {**dict(colors=colors, explode=explode, autopct='%.0f%%', 
-                       startangle=90), **prop_general}
+                       startangle=startangle_main), **prop_general}
 
         # PLOTTING
         _ = ax_main.pie(data_show.values, labels=data_show.index, **prop)
 
         ax_main.text(0.5, -0.15, f"{np.sum(data_show.values)} Supernovae", 
                      transform=ax_main.transAxes,
                      fontsize="large", ha="center", va="bottom")
@@ -466,20 +586,20 @@
         to_show = self.CLASSIFIED_KEY
         data_show = class_stat[to_show]
         if type(explode) == float:
             explode = np.full_like(data_show.values, explode, dtype="float")
 
         colors = ["tab:blue", "tab:orange", "wheat", "lavender", "lightsteelblue"]
         prop = {**dict(colors=colors, explode=explode, autopct='%.0f%%', 
-                       startangle=0), **prop_general}
+                       startangle=startangle_sub), **prop_general}
 
         # PLOTTING
         _ = ax_sub.pie(data_show.values, labels=data_show.index, **prop)
 
-        ax_sub.text(0.5, -0.15, f"{np.sum(data_show.values)} Supernovae", 
+        ax_sub.text(0.5, -0.15, f"{np.sum(data_show.values)} Type Ia Supernovae", 
                     transform=ax_sub.transAxes,
                     fontsize="large", ha="center", va="bottom")
 
         return fig
 
     
     def show_classifications(self, ax=None, fig=None, 
@@ -518,14 +638,18 @@
     def sample(self):
         """ """
         if not hasattr(self, "_sample"):
             self.load_sample()
             
         return self._sample
 
+    @property
+    def target_list(self):
+        """ """
+        return self._targetlist
     
     @property
     def types(self):
         """ list of all possible types"""
         return self.data["value"].unique()
 
     @property
```

