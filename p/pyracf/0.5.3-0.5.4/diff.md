# Comparing `tmp/pyracf-0.5.3.tar.gz` & `tmp/pyracf-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyracf-0.5.3.tar", last modified: Mon Mar 27 14:56:38 2023, max compression
+gzip compressed data, was "pyracf-0.5.4.tar", last modified: Mon May  1 20:21:10 2023, max compression
```

## Comparing `pyracf-0.5.3.tar` & `pyracf-0.5.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-03-27 14:56:38.639737 pyracf-0.5.3/
--rw-rw-r--   0 henri     (1000) henri     (1000)     1071 2022-04-10 14:57:24.000000 pyracf-0.5.3/LICENSE
--rw-rw-r--   0 henri     (1000) henri     (1000)      172 2022-04-04 21:07:37.000000 pyracf-0.5.3/MANIFEST.in
--rw-rw-r--   0 henri     (1000) henri     (1000)     6592 2023-03-27 14:56:38.639737 pyracf-0.5.3/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)     6079 2023-03-26 14:05:05.000000 pyracf-0.5.3/README.md
--rw-rw-r--   0 henri     (1000) henri     (1000)       38 2023-03-27 14:56:38.639737 pyracf-0.5.3/setup.cfg
--rw-rw-r--   0 henri     (1000) henri     (1000)      930 2023-03-27 14:56:22.000000 pyracf-0.5.3/setup.py
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-03-27 14:56:38.635738 pyracf-0.5.3/src/
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-03-27 14:56:38.635738 pyracf-0.5.3/src/pyracf/
--rw-rw-r--   0 henri     (1000) henri     (1000)    28682 2023-03-27 14:56:25.000000 pyracf-0.5.3/src/pyracf/__init__.py
--rw-rw-r--   0 henri     (1000) henri     (1000)   123027 2022-11-28 14:18:15.000000 pyracf-0.5.3/src/pyracf/offsets.json
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-03-27 14:56:38.639737 pyracf-0.5.3/src/pyracf.egg-info/
--rw-rw-r--   0 henri     (1000) henri     (1000)     6592 2023-03-27 14:56:38.000000 pyracf-0.5.3/src/pyracf.egg-info/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)      254 2023-03-27 14:56:38.000000 pyracf-0.5.3/src/pyracf.egg-info/SOURCES.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        1 2023-03-27 14:56:38.000000 pyracf-0.5.3/src/pyracf.egg-info/dependency_links.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)       24 2023-03-27 14:56:38.000000 pyracf-0.5.3/src/pyracf.egg-info/requires.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        7 2023-03-27 14:56:38.000000 pyracf-0.5.3/src/pyracf.egg-info/top_level.txt
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-01 20:21:10.419753 pyracf-0.5.4/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2023-05-01 20:17:28.000000 pyracf-0.5.4/LICENSE
+-rw-rw-r--   0 henri     (1000) henri     (1000)      172 2022-04-04 21:07:37.000000 pyracf-0.5.4/MANIFEST.in
+-rw-rw-r--   0 henri     (1000) henri     (1000)     6604 2023-05-01 20:21:10.419753 pyracf-0.5.4/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)     6079 2023-03-26 14:05:05.000000 pyracf-0.5.4/README.md
+-rw-rw-r--   0 henri     (1000) henri     (1000)       38 2023-05-01 20:21:10.419753 pyracf-0.5.4/setup.cfg
+-rw-rw-r--   0 henri     (1000) henri     (1000)      961 2023-05-01 20:21:04.000000 pyracf-0.5.4/setup.py
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-01 20:21:10.415753 pyracf-0.5.4/src/
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-01 20:21:10.415753 pyracf-0.5.4/src/pyracf/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    33323 2023-05-01 20:17:28.000000 pyracf-0.5.4/src/pyracf/__init__.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)   125683 2023-05-01 20:17:28.000000 pyracf-0.5.4/src/pyracf/offsets.json
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-01 20:21:10.419753 pyracf-0.5.4/src/pyracf.egg-info/
+-rw-rw-r--   0 henri     (1000) henri     (1000)     6604 2023-05-01 20:21:10.000000 pyracf-0.5.4/src/pyracf.egg-info/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)      254 2023-05-01 20:21:10.000000 pyracf-0.5.4/src/pyracf.egg-info/SOURCES.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        1 2023-05-01 20:21:10.000000 pyracf-0.5.4/src/pyracf.egg-info/dependency_links.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)       32 2023-05-01 20:21:10.000000 pyracf-0.5.4/src/pyracf.egg-info/requires.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        7 2023-05-01 20:21:10.000000 pyracf-0.5.4/src/pyracf.egg-info/top_level.txt
```

### Comparing `pyracf-0.5.3/PKG-INFO` & `pyracf-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.5.3
+Version: 0.5.4
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyracf
```

### Comparing `pyracf-0.5.3/README.md` & `pyracf-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pyracf-0.5.3/setup.py` & `pyracf-0.5.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyracf",
-    version="0.5.3",
+    version="0.5.4",
     author="Wizard of z/OS",
     author_email="wizard@zdevops.com",
     description="Parsing IRRDBU00 unloads in panda dataframes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wizardofzos/pyracf",
     project_urls={
         "Bug Tracker": "https://github.com/wizardofzos/pyracf/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     include_package_data=True,
     install_requires=[
         'wheel',
         'pandas',
-        'xlsxwriter'
+        'xlsxwriter',
+        'anytree'
     ],
     python_requires=">=3.6",
 )
```

### Comparing `pyracf-0.5.3/src/pyracf/__init__.py` & `pyracf-0.5.4/src/pyracf/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,15 +47,17 @@
     DSBD_RECORDTYPE    = '0400'
     DSCACC_RECORDTYPE  = '0402'
     DSACC_RECORDTYPE   = '0404'
 
     GRBD_RECORDTYPE    = '0500'
     GRMEM_RECORDTYPE   = '0503'
     GRACC_RECORDTYPE   = '0505'
+    GRCACC_RECORDTYPE  = '0507'
 
+    _ownertree          = None
 
 
     def __init__(self, irrdbu00=None, pickles=None, prefix=''):
 
         self._state = self.STATE_INIT
 
         with importlib.resources.open_text("pyracf", "offsets.json") as file:
@@ -90,15 +92,16 @@
                     'USTSO': ['_userTSO','0220'],
                     'USOMVS': ['_userOMVS','0270'],
                     'DSBD': ['_datasets','0400'],
                     'DSCACC': ['_datasetPermit','0402'],
                     'DSACC': ['_datasetAccess','0404'],
                     'GRBD': ['_generics','0500'],
                     'GRMEM': ['_genericMembers','0503'],
-                    'GRACC': ['_genericAccess','0505']
+                    'GRACC': ['_genericAccess','0505'],
+                    'GRCACC': ['_genericConditionalAccess','0507']
                 }
                 exec(f'self.{lookup[recordtype][0]} = pd.read_pickle("{pickle}")')
                 exec(f'self._records["{lookup[recordtype][1]}"] = ' + "{}")
                 exec(f'self._records["{lookup[recordtype][1]}"]["seen"] = len(self.{lookup[recordtype][0]})')
                 exec(f'self._records["{lookup[recordtype][1]}"]["parsed"] = len(self.{lookup[recordtype][0]})')
                 exec(f'self._unloadlines += len(self.{lookup[recordtype][0]})')
             self._state = self.STATE_READY
@@ -153,14 +156,15 @@
             self.DSBD  = []
             self.DSACC  = []
             self.DSCACC = []
             self.DSDFP  = []
             self.GRBD  = []
             self.GRTVOL  = []
             self.GRACC  = []
+            self.GRCACC = []
             self.GRMEM = []
             self.CERTN  = []
 
     @property
     def status(self):
         seen = 0
         parsed = 0
@@ -193,15 +197,15 @@
 
     def findOffsets(self, recordType):
         for offset in self._offsets:
             if self._offsets[offset]['record-type'] == recordType:
                 return json.loads(json.dumps(self._offsets[offset]))
         return False
 
-    def parse_fancycli(self, recordtypes=[GPBD_RECORDTYPE, GPSGRP_RECORDTYPE, GPMEM_RECORDTYPE, GPOMVS_RECORDTYPE, USBD_RECORDTYPE, USCON_RECORDTYPE, '0220', USOMVS_RECORDTYPE, '0400', DSCACC_RECORDTYPE, DSACC_RECORDTYPE, GRBD_RECORDTYPE, GRACC_RECORDTYPE], save_pickles=False, prefix=''):
+    def parse_fancycli(self, recordtypes=[GPBD_RECORDTYPE, GPSGRP_RECORDTYPE, GPMEM_RECORDTYPE, GPOMVS_RECORDTYPE, USBD_RECORDTYPE, USGCON_RECORDTYPE ,USCON_RECORDTYPE, USTSO_RECORDTYPE, USOMVS_RECORDTYPE, DSBD_RECORDTYPE, DSACC_RECORDTYPE, GRBD_RECORDTYPE, GRACC_RECORDTYPE], save_pickles=False, prefix=''):
         print(f'{datetime.now().strftime("%y-%m-%d %H:%M:%S")} - parsing {self._irrdbu00}')
         self.parse(recordtypes=recordtypes)
         print(f'{datetime.now().strftime("%y-%m-%d %H:%M:%S")} - selected recordtypes: {",".join(recordtypes)}')
         while self._state != self.STATE_READY:
             progress =  math.floor(((sum(r['seen'] for r in self._records.values() if r)) / self._unloadlines) * 63)
             pct = (progress/63) * 100 # not as strange as it seems:)
             done = progress * '▉'
@@ -213,21 +217,21 @@
         for r in recordtypes:
             print(f'{datetime.now().strftime("%y-%m-%d %H:%M:%S")} - recordtype {r} -> {self._records[r]["parsed"]} records parsed')
         print(f'{datetime.now().strftime("%y-%m-%d %H:%M:%S")} - total parse time: {(self._stoptime - self._starttime).total_seconds()} seconds')
         if save_pickles:
             self.save_pickles(path=save_pickles,prefix=prefix)
             print(f'{datetime.now().strftime("%y-%m-%d %H:%M:%S")} - Pickle files saved to {save_pickles}')
 
-    def parse(self, recordtypes=[GPBD_RECORDTYPE, GPSGRP_RECORDTYPE, GPMEM_RECORDTYPE, GPOMVS_RECORDTYPE, USBD_RECORDTYPE, USGCON_RECORDTYPE , USINSTD_RECORDTYPE, USCON_RECORDTYPE, USTSO_RECORDTYPE, USOMVS_RECORDTYPE, DSBD_RECORDTYPE, DSCACC_RECORDTYPE, DSACC_RECORDTYPE, GRBD_RECORDTYPE, GRACC_RECORDTYPE]):
+    def parse(self, recordtypes=[GPBD_RECORDTYPE, GPSGRP_RECORDTYPE, GPMEM_RECORDTYPE, GPOMVS_RECORDTYPE, USBD_RECORDTYPE, USGCON_RECORDTYPE, USCON_RECORDTYPE, USTSO_RECORDTYPE, USOMVS_RECORDTYPE, DSBD_RECORDTYPE, DSACC_RECORDTYPE, GRBD_RECORDTYPE, GRACC_RECORDTYPE]):
         self._starttime = datetime.now()
         pt = threading.Thread(target=self.parse_t,args=(recordtypes,))
         pt.start()
         return True
 
-    def parse_t(self, thingswewant=[GPBD_RECORDTYPE, GPSGRP_RECORDTYPE, GPMEM_RECORDTYPE, GPOMVS_RECORDTYPE, USBD_RECORDTYPE, USGCON_RECORDTYPE , USINSTD_RECORDTYPE, USCON_RECORDTYPE, USTSO_RECORDTYPE, USOMVS_RECORDTYPE, DSBD_RECORDTYPE, DSCACC_RECORDTYPE, DSACC_RECORDTYPE, GRBD_RECORDTYPE, GRACC_RECORDTYPE]):
+    def parse_t(self, thingswewant=[GPBD_RECORDTYPE, GPSGRP_RECORDTYPE, GPMEM_RECORDTYPE, GPOMVS_RECORDTYPE, USBD_RECORDTYPE, USGCON_RECORDTYPE, USCON_RECORDTYPE, USTSO_RECORDTYPE, USOMVS_RECORDTYPE, DSBD_RECORDTYPE, DSACC_RECORDTYPE, GRBD_RECORDTYPE, GRACC_RECORDTYPE]):
         # TODO: make this multiple threads (per record-type?)
         self._state = self.STATE_PARSING
         self.THREAD_COUNT += 1
         # TODO: Complete all record-types. Fix offsets.json !
         with open(self._irrdbu00, 'r', encoding="utf-8", errors="replace") as infile:
             for line in infile:
                 r = line[:4]
@@ -275,15 +279,17 @@
                         if r == self.DSACC_RECORDTYPE:
                             self.DSACC.append(irrmodel)  
                         if r == self.GRBD_RECORDTYPE: 
                             self.GRBD.append(irrmodel)
                         if r == self.GRMEM_RECORDTYPE:
                             self.GRMEM.append(irrmodel)                            
                         if r == self.GRACC_RECORDTYPE:
-                            self.GRACC.append(irrmodel)       
+                            self.GRACC.append(irrmodel)    
+                        if r == self.GRCACC_RECORDTYPE:
+                            self.GRCACC.append(irrmodel)   
                     self._records[r]['parsed'] += 1
         # all models parsed :)
 
         if self.GPBD_RECORDTYPE in thingswewant:
             self._groups = pd.DataFrame.from_dict(self.GPBD)
         if self.GPSGRP_RECORDTYPE in thingswewant:
             self._subgroups = pd.DataFrame.from_dict(self.GPSGRP)
@@ -311,14 +317,16 @@
             self._datasetAccess = pd.DataFrame.from_dict(self.DSACC)
         if self.GRBD_RECORDTYPE in thingswewant:
             self._generics = pd.DataFrame.from_dict(self.GRBD)
         if self.GRMEM_RECORDTYPE in thingswewant:
             self._genericMembers = pd.DataFrame.from_dict(self.GRMEM)
         if self.GRACC_RECORDTYPE in thingswewant:
             self._genericAccess = pd.DataFrame.from_dict(self.GRACC)
+        if self.GRCACC_RECORDTYPE in thingswewant:
+            self._genericConditionalAccess = pd.DataFrame.from_dict(self.GRCACC)
         
         self.THREAD_COUNT -= 1
         if self.THREAD_COUNT == 0:
             self._state = self.STATE_READY         
             self._stoptime = datetime.now()
         return True
 
@@ -368,14 +376,16 @@
             self.save_pickle(df=self._datasetAccess, dfname='DSACC', path=path, prefix=prefix)
         if len(self.GRBD) > 0:
             self.save_pickle(df=self._generics, dfname='GRBD', path=path, prefix=prefix)
         if len(self.GRMEM) > 0:
             self.save_pickle(df=self._genericMembers, dfname='GRMEM', path=path, prefix=prefix)
         if len(self.GRACC) > 0:
             self.save_pickle(df=self._genericAccess, dfname='GRACC', path=path, prefix=prefix)
+        if len(self.GRCACC) > 0:
+            self.save_pickle(df=self._genericConditionalAccess, dfname='GRCACC', path=path, prefix=prefix)
 
     @property
     def users(self):
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
         try:
             return self._users
@@ -483,14 +493,20 @@
     @property
     def genericAccess(self, query=None):
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
         return self._genericAccess
     
     @property
+    def genericConditionalAccess(self):
+        if self._state != self.STATE_READY:
+            raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
+        return self._genericConditionalAccess
+    
+    @property
     def userOMVS(self, query=None):
         if self._state != self.STATE_READY:
             raise StoopidException('Not done parsing yet! (PEBKAM/ID-10T error)')
         return self._userOMVS
 
     @property
     def groupOMVS(self, query=None):
@@ -642,9 +658,95 @@
                         centry = rdict.get(i,None)
                         if centry:
                             value = shared_strings[centry.string]
                             worksheet.write(j, i, value, accessLevelFormats[value])
 
         writer.save()   
 
+    def ownertree(self):
+        if self._ownertree != None:
+            return self._ownertree
+        else:
+            # get all owners... (group or user)
+            self._ownertree = {}
+            owners = self.groups.groupby('GPBD_OWNER_ID')
+            for owner in owners.groups.keys():
+                if owner not in self._ownertree:
+                    self._ownertree[owner] = []
+                    for group in owners.get_group(owner)['GPBD_NAME'].values:
+                        self._ownertree[owner].append(group)
+            # now we gotta condense it :)
+            return self._ownertree
+            for supgrp in self._ownertree:
+                for subgrp in self._ownertree[supgrp]:
+                    if subgrp in self._ownertree.values:
+                        self._ownertree[supgrp].remove(subgrp)
+                        self._ownertree[supgrp].append(self._ownertree[subgrp])
+
+
+            return self._ownertree
+
+
+
+
+    
+    def getdatsetrisk(self, profile=''):
+        '''This will produce a dict as follows:
+      
+        '''
+        try:
+            if self._records[self.GPBD_RECORDTYPE]['parsed'] == 0 or self._records[self.USCON_RECORDTYPE]['parsed'] == 0 or self._records[self.USBD_RECORDTYPE]['parsed'] == 0 or self._records[self.DSACC_RECORDTYPE]['parsed'] == 0 or  self._records[self.DSBD_RECORDTYPE]['parsed'] == 0:
+                raise StoopidException("Need to parse DSACC and DSBD first...")
+        except:
+            raise StoopidException("Need to parse DSACC, USCON, USBD, GPBD and DSBD first...")
+        
+        d = self.datasets.loc[self.datasets.DSBD_NAME==profile]
+        if len(d) == 0:
+            raise Exception('Profile not here...')
+        
+        owner = d['DSBD_OWNER_ID'].values[0]
+        accesslist = {}
+        accessmanagers = {}
+        dsacc = self.datasetAccess.groupby('DSACC_NAME')
+        peraccess = dsacc.get_group(profile).groupby('DSACC_ACCESS')
+        for access in ['NONE','EXECUTE','READ','UPDATE','CONTROL','ALTER']:
+            accesslist[access] = []
+            accessmanagers[access] = []
+            if access in peraccess.groups.keys():
+                a = peraccess.get_group(access)['DSACC_AUTH_ID'].values
+                for id in a:
+                    if len(self.user(id)) == 1:
+                        accesslist[access].append(id)
+                    else:
+                        if len(self.group(id)) == 1:
+                            g = self.connectData.loc[self.connectData.USCON_GRP_ID==id]
+                            for user,grp_special in g[['USCON_NAME','USCON_GRP_SPECIAL']].values:
+                                accesslist[access].append(user)
+                                # But suppose this user is group_special here?
+                                if grp_special=='YES':
+                                    accessmanagers[access].append(user)
+                            # And wait a minute... this groups owner, can also add people to the group?
+                            gowner = self.group(id)['GPBD_OWNER_ID'].values[0]
+                            if len(self.user(gowner)) == 1:
+                                accessmanagers[access].append(gowner)
+                            else:
+                                gg = self.connectData.loc[self.connectData.USCON_GRP_ID==gowner]
+                                for user,grp_special in gg[['USCON_NAME','USCON_GRP_SPECIAL']].values:
+                                    if grp_special=='YES':
+                                        accessmanagers[access].append(user)
+                # clean up doubles...
+            accessmanagers[access] = list(set(accessmanagers[access]))
+            accesslist[access] = list(set(accesslist[access]))
+
+        y = {
+            'owner': owner,
+            'accessmanagers': accessmanagers,
+            'uacc': d['DSBD_UACC'].values[0],
+            'permits': accesslist
+        }
+
+
+        return y
+
 class IRRDBU(RACF):
-    pass
+    pass
+
```

### Comparing `pyracf-0.5.3/src/pyracf/offsets.json` & `pyracf-0.5.4/src/pyracf/offsets.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9795918367346939%*

 * *Differences: {"'general-resource-conditional-access-record'": "OrderedDict([('record-type', '0507'), "*

 * *                                                 "('ref-url', "*

 * *                                                 "'https://www.ibm.com/docs/en/zos/2.2.0?topic=utility-general-resource-record-formats'), "*

 * *                                                 "('offsets', [OrderedDict([('field-desc', 'Record "*

 * *                                                 'type of the General Resources Conditional Access '*

 * *                 […]*

```diff
@@ -848,14 +848,90 @@
                 "start": "2312",
                 "type": "Char"
             }
         ],
         "record-type": "1560",
         "ref-url": "http://www.redbooks.ibm.com/iea/pdf/zOS_V2R1_RACF_Database_Unload_of_Certificate_DNs.pdf"
     },
+    "general-resource-conditional-access-record": {
+        "offsets": [
+            {
+                "end": "4",
+                "field-desc": "Record type of the General Resources Conditional Access record (0507).",
+                "field-name": "GRCACC_RECORD_TYPE",
+                "start": "1",
+                "type": "Int"
+            },
+            {
+                "end": "251",
+                "field-desc": "General resource name as taken from the profile name.",
+                "field-name": "GRCACC_NAME",
+                "start": "6",
+                "type": "Char"
+            },
+            {
+                "end": "260",
+                "field-desc": "Name of the class to which the general resource profile belongs.",
+                "field-name": "GRACC_CLASS_NAME",
+                "start": "253",
+                "type": "Char"
+            },
+            {
+                "end": "269",
+                "field-desc": "The type of conditional access checking that is being performed. Valid values are CONSOLE, TERMINAL, JESINPUT, SYSID, APPCPORT, SERVAUTH, PROGRAM, and CRITERIA.",
+                "field-name": "GRCACC_CATYPE",
+                "start": "262",
+                "type": "Char"
+            },
+            {
+                "end": "278",
+                "field-desc": "The name of a conditional access element which is permitted access.",
+                "field-name": "GRCACC_CANAME",
+                "start": "271",
+                "type": "Char"
+            },
+            {
+                "end": "287",
+                "field-desc": "The user ID or group name which has authority to the general resource.",
+                "field-name": "GRCACC_AUTH_ID",
+                "start": "280",
+                "type": "Char"
+            },
+            {
+                "end": "296",
+                "field-desc": "The authority of the conditional access element/user combination. Valid values are NONE, READ, UPDATE, CONTROL, and ALTER.",
+                "field-name": "GRCACC_AUTH_ID",
+                "start": "289",
+                "type": "Char"
+            },
+            {
+                "end": "302",
+                "field-desc": "The number of times that the general resource was accessed.",
+                "field-name": "GRCACC_ACCESS_CNT",
+                "start": "298",
+                "type": "Int"
+            },
+            {
+                "end": "311",
+                "field-desc": "The network name when GRCACC_CATYPE is APPCPORT.",
+                "field-name": "GRCACC_NET_ID",
+                "start": "304",
+                "type": "Char"
+            },
+            {
+                "end": "556",
+                "field-desc": "Access criteria or SERVAUTH IP data.",
+                "field-name": "GRCACC_CACRITERIA",
+                "start": "313",
+                "type": "Char"
+            }
+        ],
+        "record-type": "0507",
+        "ref-url": "https://www.ibm.com/docs/en/zos/2.2.0?topic=utility-general-resource-record-formats"
+    },
     "general-resource-members-record": {
         "offsets": [
             {
                 "end": "4",
                 "field-desc": "Record type of the General Resource Members record (0503).",
                 "field-name": "GRMEM_RECORD_TYPE",
                 "start": "1",
```

### Comparing `pyracf-0.5.3/src/pyracf.egg-info/PKG-INFO` & `pyracf-0.5.4/src/pyracf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.5.3
+Version: 0.5.4
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyracf
```

