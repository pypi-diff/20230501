# Comparing `tmp/NewareNDA-2023.4.14-py3-none-any.whl.zip` & `tmp/NewareNDA-2023.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 6276 bytes, number of entries: 9
--rw-rw-r--  2.0 unx     7403 b- defN 23-Apr-14 13:45 NewareNDA/NewareNDA.py
--rw-rw-r--  2.0 unx       61 b- defN 22-Sep-06 14:02 NewareNDA/__init__.py
--rw-rw-r--  2.0 unx       28 b- defN 23-Apr-14 13:47 NewareNDA/version.py
--rwxrwxr-x  2.0 unx     1189 b- defN 23-Apr-14 14:03 NewareNDA-2023.4.14.data/scripts/NewareNDA-cli.py
--rw-rw-r--  2.0 unx     1488 b- defN 23-Apr-14 14:03 NewareNDA-2023.4.14.dist-info/LICENSE
--rw-rw-r--  2.0 unx      919 b- defN 23-Apr-14 14:03 NewareNDA-2023.4.14.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-14 14:03 NewareNDA-2023.4.14.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Apr-14 14:03 NewareNDA-2023.4.14.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      751 b- defN 23-Apr-14 14:03 NewareNDA-2023.4.14.dist-info/RECORD
-9 files, 11941 bytes uncompressed, 4968 bytes compressed:  58.4%
+Zip file size: 8208 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx     7215 b- defN 23-May-01 14:45 NewareNDA/NewareNDA.py
+-rw-rw-r--  2.0 unx     4637 b- defN 23-Apr-28 21:34 NewareNDA/NewareNDAx.py
+-rw-rw-r--  2.0 unx       61 b- defN 23-Apr-28 21:30 NewareNDA/__init__.py
+-rw-rw-r--  2.0 unx       28 b- defN 23-May-01 14:48 NewareNDA/version.py
+-rwxrwxr-x  2.0 unx     1189 b- defN 23-May-01 14:49 NewareNDA-2023.5.1.data/scripts/NewareNDA-cli.py
+-rw-rw-r--  2.0 unx     1488 b- defN 23-May-01 14:49 NewareNDA-2023.5.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1052 b- defN 23-May-01 14:49 NewareNDA-2023.5.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-01 14:49 NewareNDA-2023.5.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-May-01 14:49 NewareNDA-2023.5.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      826 b- defN 23-May-01 14:49 NewareNDA-2023.5.1.dist-info/RECORD
+10 files, 16598 bytes uncompressed, 6790 bytes compressed:  59.1%
```

## zipnote {}

```diff
@@ -1,28 +1,31 @@
 Filename: NewareNDA/NewareNDA.py
 Comment: 
 
+Filename: NewareNDA/NewareNDAx.py
+Comment: 
+
 Filename: NewareNDA/__init__.py
 Comment: 
 
 Filename: NewareNDA/version.py
 Comment: 
 
-Filename: NewareNDA-2023.4.14.data/scripts/NewareNDA-cli.py
+Filename: NewareNDA-2023.5.1.data/scripts/NewareNDA-cli.py
 Comment: 
 
-Filename: NewareNDA-2023.4.14.dist-info/LICENSE
+Filename: NewareNDA-2023.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: NewareNDA-2023.4.14.dist-info/METADATA
+Filename: NewareNDA-2023.5.1.dist-info/METADATA
 Comment: 
 
-Filename: NewareNDA-2023.4.14.dist-info/WHEEL
+Filename: NewareNDA-2023.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: NewareNDA-2023.4.14.dist-info/top_level.txt
+Filename: NewareNDA-2023.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: NewareNDA-2023.4.14.dist-info/RECORD
+Filename: NewareNDA-2023.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## NewareNDA/NewareNDA.py

```diff
@@ -131,31 +131,31 @@
                     aux.append(_aux_bytes_to_list(bytes))
 
     # Create DataFrame and sort by Index
     df = pd.DataFrame(output, columns=rec_columns)
     df.dropna(inplace=True)
     df.drop_duplicates(inplace=True)
 
-    if not df.Index.is_monotonic_increasing:
+    if not df['Index'].is_monotonic_increasing:
         df.sort_values('Index', inplace=True)
 
     df.reset_index(drop=True, inplace=True)
 
     # Join temperature data
     aux_df = pd.DataFrame(aux, columns=aux_columns)
     aux_df.drop_duplicates(inplace=True)
     if not aux_df.empty:
         pvt_df = aux_df.pivot(index='Index', columns='Aux', values='T')
         for k in pvt_df.keys():
             pvt_df.rename(columns={k: f"T{k}"}, inplace=True)
         df = df.join(pvt_df, on='Index')
 
     # Postprocessing
-    df.Step = _count_changes(df.Step)
-    df.Cycle = _generate_cycle_number(df)
+    df['Step'] = _count_changes(df['Step'])
+    df['Cycle'] = _generate_cycle_number(df)
     df = df.astype(dtype=dtype_dict)
 
     return df
 
 
 def _valid_record(bytes):
     """Helper function to identify a valid record"""
@@ -173,25 +173,18 @@
     [Status, Jump, Time] = struct.unpack('<BBQ', bytes[12:22])
     [Voltage, Current] = struct.unpack('<ii', bytes[22:30])
     [Charge_capacity, Discharge_capacity] = struct.unpack('<qq', bytes[38:54])
     [Charge_energy, Discharge_energy] = struct.unpack('<qq', bytes[54:70])
     [Y, M, D, h, m, s] = struct.unpack('<HBBBBB', bytes[70:77])
     [Range] = struct.unpack('<i', bytes[78:82])
 
-    # Index should not be zero
-    if Index == 0:
+    # Index and should not be zero
+    if Index == 0 or Status == 0:
         return []
 
-    # Convert date to datetime. Try Unix timestamp on failure.
-    try:
-        Date = datetime(Y, M, D, h, m, s)
-    except ValueError:
-        [Timestamp] = struct.unpack('<Q', bytes[70:78])
-        Date = datetime.fromtimestamp(Timestamp)
-
     multiplier = multiplier_dict[Range]
 
     # Create a dictionary for the record
     list = [
         Index,
         Cycle + 1,
         Step,
@@ -199,15 +192,15 @@
         Time/1000,
         Voltage/10000,
         Current*multiplier,
         Charge_capacity*multiplier/3600,
         Discharge_capacity*multiplier/3600,
         Charge_energy*multiplier/3600,
         Discharge_energy*multiplier/3600,
-        Date
+        datetime(Y, M, D, h, m, s)
     ]
     return list
 
 
 def _aux_bytes_to_list(bytes):
     """Helper function for intepreting auxiliary records"""
     [Aux, Index] = struct.unpack('<BI', bytes[1:6])
@@ -219,21 +212,21 @@
 def _generate_cycle_number(df):
     """
     Generate a cycle number to match Neware. A new cycle starts with a charge
     step after there has previously been a discharge.
     """
 
     # Identify the beginning of charge steps
-    chg = (df.Status == 'CCCV_Chg') | (df.Status == 'CC_Chg')
+    chg = (df['Status'] == 'CCCV_Chg') | (df['Status'] == 'CC_Chg')
     chg = (chg - chg.shift()).clip(0)
     chg.iat[0] = 1
 
     # Convert to numpy arrays
     chg = chg.values
-    status = df.Status.values
+    status = df['Status'].values
 
     # Increment the cycle at a charge step after there has been a discharge
     cyc = 1
     dchg = False
     for n in range(len(chg)):
         if chg[n] & dchg:
             cyc += 1
```

## NewareNDA/version.py

```diff
@@ -1 +1 @@
-__version__ = 'v2023.04.14'
+__version__ = 'v2023.05.01'
```

## Comparing `NewareNDA-2023.4.14.data/scripts/NewareNDA-cli.py` & `NewareNDA-2023.5.1.data/scripts/NewareNDA-cli.py`

 * *Files identical despite different names*

## Comparing `NewareNDA-2023.4.14.dist-info/LICENSE` & `NewareNDA-2023.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `NewareNDA-2023.4.14.dist-info/METADATA` & `NewareNDA-2023.5.1.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewareNDA
-Version: 2023.4.14
+Version: 2023.5.1
 Summary: Neware nda binary file reader.
 Home-page: https://github.com/Solid-Energy-Systems/NewareNDA
 Author: Daniel Cogswell
 Author-email: danielcogswell@ses.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
@@ -14,20 +14,26 @@
 
 # NewareNDA
 
 © 2023 Copyright SES AI
 <br>Author: Daniel Cogswell
 <br>Email: danielcogswell@ses.ai
 
-Python module and Bash command line tool for reading and converting Neware .nda battery cycling files.
+Python module and command line tool for reading and converting Neware .nda battery cycling files.
 
 # Installation
+To install from the PyPi package repository:
+```
+pip install NewareNDA
+```
+
+To install from source, clone this repository and run:
 ```
 cd NewareNDA
-pip install .
+pip install NewareNDA
 ```
 
 # Usage
 ```
 import NewareNDA
 df = NewareNDA.read('filename.nda')
 ```
```

## Comparing `NewareNDA-2023.4.14.dist-info/RECORD` & `NewareNDA-2023.5.1.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-NewareNDA/NewareNDA.py,sha256=ROuoZ2hcHEAKBpueQhRTcsSYpeR0oA9jVoBCfgYv5xk,7403
+NewareNDA/NewareNDA.py,sha256=Mzg6R_qg_6InxeydFyNMFa24CVN6YbM4dJR8dnyBGCU,7215
+NewareNDA/NewareNDAx.py,sha256=TL6EMS76SvDkAc2B9JaUhzdWo6a6POmJq-ua0oNQKZU,4637
 NewareNDA/__init__.py,sha256=HcIL21PU-NmBDfuzsk6zzOsoq_GIgFwU86JYhHUUxVY,61
-NewareNDA/version.py,sha256=LrufNtHNcWr2xPkf2tZ2uoA4oWKI-847_Z2cSdiIz0Q,28
-NewareNDA-2023.4.14.data/scripts/NewareNDA-cli.py,sha256=lKzHAUSqfmxorAo-qRKZikdgW6B-kJ-ePq3YVdR5qno,1189
-NewareNDA-2023.4.14.dist-info/LICENSE,sha256=AGY-bfMClgUyCBsA_w4IMlP5G018QfjCPfSGgHOrF3Y,1488
-NewareNDA-2023.4.14.dist-info/METADATA,sha256=M4xT88AaEa2C4lD0j8nyiNi-RAKjtCvtgZ9NlaLGueE,919
-NewareNDA-2023.4.14.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-NewareNDA-2023.4.14.dist-info/top_level.txt,sha256=TrIpR_dGmBO9hgO5ZtJ2_09-dx4Q1x3iieFIJ2ZbIa4,10
-NewareNDA-2023.4.14.dist-info/RECORD,,
+NewareNDA/version.py,sha256=5PsANnDwbRVkUHbbIV-xjcAuiNJ1oLG-3-6mqc_KMr8,28
+NewareNDA-2023.5.1.data/scripts/NewareNDA-cli.py,sha256=lKzHAUSqfmxorAo-qRKZikdgW6B-kJ-ePq3YVdR5qno,1189
+NewareNDA-2023.5.1.dist-info/LICENSE,sha256=AGY-bfMClgUyCBsA_w4IMlP5G018QfjCPfSGgHOrF3Y,1488
+NewareNDA-2023.5.1.dist-info/METADATA,sha256=XSlZ1piBTLMECWbIgewW6sKRIaKn2EDDglptNGpPjd8,1052
+NewareNDA-2023.5.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+NewareNDA-2023.5.1.dist-info/top_level.txt,sha256=TrIpR_dGmBO9hgO5ZtJ2_09-dx4Q1x3iieFIJ2ZbIa4,10
+NewareNDA-2023.5.1.dist-info/RECORD,,
```

