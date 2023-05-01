# Comparing `tmp/limes_x-1.0.1-py3-none-any.whl.zip` & `tmp/limes_x-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 35670 bytes, number of entries: 21
+Zip file size: 35742 bytes, number of entries: 21
 -rw-rw-r--  2.0 unx      220 b- defN 23-Apr-19 01:42 limes_x/__init__.py
 -rw-rw-r--  2.0 unx       69 b- defN 23-Apr-19 01:42 limes_x/constants.py
 -rw-rw-r--  2.0 unx     2864 b- defN 23-Apr-19 01:42 limes_x/telemetry.py
--rw-rw-r--  2.0 unx    38931 b- defN 23-Apr-19 01:42 limes_x/workflow.py
+-rw-rw-r--  2.0 unx    38931 b- defN 23-Apr-30 09:08 limes_x/workflow.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-19 01:42 limes_x/common/__init__.py
 -rw-rw-r--  2.0 unx     8098 b- defN 23-Apr-19 01:42 limes_x/common/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-19 01:42 limes_x/environments/__init__.py
 -rw-rw-r--  2.0 unx     1202 b- defN 23-Apr-19 01:42 limes_x/environments/_setup.py
--rw-rw-r--  2.0 unx     6015 b- defN 23-Apr-27 17:28 limes_x/environments/hpc.py
+-rw-rw-r--  2.0 unx     6151 b- defN 23-May-01 01:12 limes_x/environments/hpc.py
 -rw-rw-r--  2.0 unx     3654 b- defN 23-Apr-19 01:42 limes_x/environments/local.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-19 01:42 limes_x/execution/__init__.py
 -rw-rw-r--  2.0 unx     2814 b- defN 23-Apr-19 01:42 limes_x/execution/comms.py
--rw-rw-r--  2.0 unx     9436 b- defN 23-Apr-19 01:42 limes_x/execution/executors.py
+-rw-rw-r--  2.0 unx     9506 b- defN 23-Apr-29 08:02 limes_x/execution/executors.py
 -rw-rw-r--  2.0 unx     5105 b- defN 23-Apr-19 01:42 limes_x/execution/instances.py
 -rw-rw-r--  2.0 unx    14052 b- defN 23-Apr-19 01:42 limes_x/execution/modules.py
 -rw-rw-r--  2.0 unx     4419 b- defN 23-Apr-19 01:42 limes_x/execution/solver.py
 -rw-rw-r--  2.0 unx      677 b- defN 23-Apr-19 01:42 limes_x/execution/template_module_definition.py
--rw-rw-r--  2.0 unx     9991 b- defN 23-Apr-27 17:29 limes_x-1.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-27 17:29 limes_x-1.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Apr-27 17:29 limes_x-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1717 b- defN 23-Apr-27 17:29 limes_x-1.0.1.dist-info/RECORD
-21 files, 109364 bytes uncompressed, 32872 bytes compressed:  69.9%
+-rw-rw-r--  2.0 unx     9991 b- defN 23-May-01 17:09 limes_x-1.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-01 17:09 limes_x-1.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-May-01 17:09 limes_x-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1717 b- defN 23-May-01 17:09 limes_x-1.0.2.dist-info/RECORD
+21 files, 109570 bytes uncompressed, 32944 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -45,20 +45,20 @@
 
 Filename: limes_x/execution/solver.py
 Comment: 
 
 Filename: limes_x/execution/template_module_definition.py
 Comment: 
 
-Filename: limes_x-1.0.1.dist-info/METADATA
+Filename: limes_x-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: limes_x-1.0.1.dist-info/WHEEL
+Filename: limes_x-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: limes_x-1.0.1.dist-info/top_level.txt
+Filename: limes_x-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: limes_x-1.0.1.dist-info/RECORD
+Filename: limes_x-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## limes_x/environments/hpc.py

```diff
@@ -44,15 +44,15 @@
         if s.endswith('\n'): s = s[:-1]
         line = f'{_timestamp()} {s}'
         if not is_child: log.append(line)
         with open(realtime_log, 'a') as f:
             if not is_child: f.write(line+NEWLINE)
 
     def _shell(cmd: str, is_child: bool):
-        cmd = cmd.replace("  ", "")
+        cmd = " ".join([tok for tok in cmd.split(" ") if tok != ""])
         lines = cmd.split('\n')
         ts = _timestamp()
         cmd_history.append(f"{ts}")
         for line in lines:
             line = line.strip()
             if line == "": continue
             cmd_history.append(f"{' '*(len(ts))}{line}")
@@ -145,27 +145,29 @@
             """, is_child=False)
         _shell("""\
             echo "---- final workspace:"
             ls | xargs -I {} sh -c "echo {}/ && ls -lh {}"
             echo "---- done!"
         """, is_child=False)
     else:
-        _shell('echo "terminating due to missing requirement', is_child=False)
+        _shell('echo "terminating due to missing requirement"', is_child=False)
 
     result_json = 'result.json'
     result_path = RELATIVE_OUTPUT_PATH.joinpath(result_json)
     def _get_result_json():
         if result_path.exists():
             with open(result_path) as j:
                 try:
                     return json.load(j)
                 except json.JSONDecodeError:
                     return {}
         else:
             return {}
 
+    # todo: consolidate shell def with local
+    # todo: get exectutor cmd,out,err and use with local
     res = _get_result_json()
     res['hpc-wrapper_commands'] = cmd_history
     res['hpc-wrapper_out'] = out_log
     res['hpc-wrapper_err'] = err_log
     with open(WORKSPACE.joinpath(RELATIVE_OUTPUT_PATH).joinpath(result_json), 'w') as outj:
         json.dump(res, outj, indent=4)
```

## limes_x/execution/executors.py

```diff
@@ -29,14 +29,17 @@
         c.output_folder = Path(instance.GetFolderName())
         c.params = params.Copy()
         c.ref = instance.step.location.joinpath(ComputeModule.LIB_FOLDER)
         c.manifest = dict((Item(k), [ii.value for ii in v] if isinstance(v, list) else v.value) for k, v in self.instance.inputs.items())
         if _save: c.Save(workspace)
         self.context = c
 
+    def SaveContext(self):
+        self.context.Save(self.workspace)
+
     def Shell(self, cmd: str):
         err_log = []
         pr = lambda s: print(s, end="")
         code=LiveShell(cmd, echo_cmd=False, onErr=lambda s: err_log.append(s), onOut=pr if self._verbose else lambda s: None)
         return code==0, "".join(err_log)
 
 ExecutionHandler = Callable[[Job], tuple[bool, str]]
```

## Comparing `limes_x-1.0.1.dist-info/METADATA` & `limes_x-1.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limes-x
-Version: 1.0.1
+Version: 1.0.2
 Summary: declarative workflow automation
 Home-page: https://github.com/hallamlab/limes-x
 Author: Tony Liu
 Author-email: contacttonyliu@gmail.com
 Project-URL: Bug Tracker, https://github.com/hallamlab/limes-x/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

## Comparing `limes_x-1.0.1.dist-info/RECORD` & `limes_x-1.0.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 limes_x/constants.py,sha256=yugKKsslkE48FwDWtzqkZ8EUK4XLX_NEh9cccmm_1IM,69
 limes_x/telemetry.py,sha256=6hUE1nxxKkPUGUNq0KlIbHQqa3pSqA0zZSjb57Wyngc,2864
 limes_x/workflow.py,sha256=taAErdX4P017ay4y8CJoeg9f43okaXjtlpSVpbnMBPU,38931
 limes_x/common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 limes_x/common/utils.py,sha256=83ayvyp9oieN9CFF9VNxjQQwK06EWzqXKaLDjhGqC_c,8098
 limes_x/environments/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 limes_x/environments/_setup.py,sha256=rI9gTVt2VMXfeAsuxkTx3ucBp5kd_K-Z6xbJqybzEvg,1202
-limes_x/environments/hpc.py,sha256=MKU6R8hJ7fhqd5Mx3TXQzJCQCLBMhY5Wd33bygAnB04,6015
+limes_x/environments/hpc.py,sha256=vNbqopLFFrk8AXfKeLgPNlgRPEl-fQMxFNLi-sJBR44,6151
 limes_x/environments/local.py,sha256=MF_-1XB4hiFUI9_0fhXCRrMshFSlc5hyO1rG1B35kik,3654
 limes_x/execution/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 limes_x/execution/comms.py,sha256=Yx_cIyvzuA7h_iKU4R3fyd1LvsKZzZx-NsVZh_MXHE4,2814
-limes_x/execution/executors.py,sha256=6O7uZqyAqFLS-lmQifanKc_8CUKPTFHACL0yDrYiQlY,9436
+limes_x/execution/executors.py,sha256=XQDQdbrahymtWE7xVqRMUudg-lu-lCcv2_yZSbSiE_I,9506
 limes_x/execution/instances.py,sha256=lT32W3nNSOrfovSNEl7ARY8Yt4SkhkA-1NjWUhBvOds,5105
 limes_x/execution/modules.py,sha256=AIEY-xyIDUhrQvw7qxJChTwXNTEtydKjrxHZCd4woWs,14052
 limes_x/execution/solver.py,sha256=y9XNSlZscAHxizN57PZTMphHw1PVWjFnEfHyrGN7SFU,4419
 limes_x/execution/template_module_definition.py,sha256=RxW4KsU1-iEScq_Y5GIafSfeXnQQeYGYr9FC9AZ8-VQ,677
-limes_x-1.0.1.dist-info/METADATA,sha256=TP1mWoyP9Uv5yUOoaIMInZZeVv5pyXbg2sTSJhDRnY4,9991
-limes_x-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-limes_x-1.0.1.dist-info/top_level.txt,sha256=r9RGajCrNNSpim7JI2bx3UHGzgXw2vRLTNuxMRwPRNQ,8
-limes_x-1.0.1.dist-info/RECORD,,
+limes_x-1.0.2.dist-info/METADATA,sha256=1dM-4hli2KX_-9iXYqBEMte70A6eg4B5mQoB6365ON8,9991
+limes_x-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+limes_x-1.0.2.dist-info/top_level.txt,sha256=r9RGajCrNNSpim7JI2bx3UHGzgXw2vRLTNuxMRwPRNQ,8
+limes_x-1.0.2.dist-info/RECORD,,
```

