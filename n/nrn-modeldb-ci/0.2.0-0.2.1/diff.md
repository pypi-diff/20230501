# Comparing `tmp/nrn-modeldb-ci-0.2.0.tar.gz` & `tmp/nrn-modeldb-ci-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrn-modeldb-ci-0.2.0.tar", last modified: Thu Dec 15 13:56:16 2022, max compression
+gzip compressed data, was "nrn-modeldb-ci-0.2.1.tar", last modified: Mon May  1 07:37:47 2023, max compression
```

## Comparing `nrn-modeldb-ci-0.2.0.tar` & `nrn-modeldb-ci-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:56:16.802948 nrn-modeldb-ci-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:56:16.798948 nrn-modeldb-ci-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:56:16.798948 nrn-modeldb-ci-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2022-12-15 13:55:43.000000 nrn-modeldb-ci-0.2.0/.github/workflows/nrn-modeldb-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2022-12-15 13:55:43.000000 nrn-modeldb-ci-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2022-12-15 13:55:43.000000 nrn-modeldb-ci-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10597 2022-12-15 13:56:16.802948 nrn-modeldb-ci-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10275 2022-12-15 13:55:43.000000 nrn-modeldb-ci-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:56:16.802948 nrn-modeldb-ci-0.2.0/modeldb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-15 13:55:43.000000 nrn-modeldb-ci-0.2.0/modeldb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2022-12-15 13:55:43.000000 nrn-modeldb-ci-0.2.0/modeldb/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2022-12-15 13:55:43.000000 nrn-modeldb-ci-0.2.0/modeldb/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2022-12-15 13:55:43.000000 nrn-modeldb-ci-0.2.0/modeldb/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2022-12-15 13:55:43.000000 nrn-modeldb-ci-0.2.0/modeldb/hocscripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    20368 2022-12-15 13:55:43.000000 nrn-modeldb-ci-0.2.0/modeldb/modeldb-run.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2022-12-15 13:55:43.000000 nrn-modeldb-ci-0.2.0/modeldb/modeldb.py
--rw-r--r--   0 runner    (1001) docker     (123)    16045 2022-12-15 13:55:43.000000 nrn-modeldb-ci-0.2.0/modeldb/modelrun.py
--rw-r--r--   0 runner    (1001) docker     (123)     8826 2022-12-15 13:55:43.000000 nrn-modeldb-ci-0.2.0/modeldb/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2022-12-15 13:55:43.000000 nrn-modeldb-ci-0.2.0/modeldb/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2022-12-15 13:55:43.000000 nrn-modeldb-ci-0.2.0/modeldb/showgout.hoc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:56:16.802948 nrn-modeldb-ci-0.2.0/modeldb/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2022-12-15 13:55:43.000000 nrn-modeldb-ci-0.2.0/modeldb/templates/diffreport.html
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2022-12-15 13:55:43.000000 nrn-modeldb-ci-0.2.0/modeldb/templates/report.html
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2022-12-15 13:55:43.000000 nrn-modeldb-ci-0.2.0/modeldb/templates/runtimes.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 13:56:16.802948 nrn-modeldb-ci-0.2.0/nrn_modeldb_ci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10597 2022-12-15 13:56:16.000000 nrn-modeldb-ci-0.2.0/nrn_modeldb_ci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      653 2022-12-15 13:56:16.000000 nrn-modeldb-ci-0.2.0/nrn_modeldb_ci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 13:56:16.000000 nrn-modeldb-ci-0.2.0/nrn_modeldb_ci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2022-12-15 13:56:16.000000 nrn-modeldb-ci-0.2.0/nrn_modeldb_ci.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2022-12-15 13:56:16.000000 nrn-modeldb-ci-0.2.0/nrn_modeldb_ci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-15 13:56:16.000000 nrn-modeldb-ci-0.2.0/nrn_modeldb_ci.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-15 13:56:16.802948 nrn-modeldb-ci-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2022-12-15 13:55:43.000000 nrn-modeldb-ci-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:37:47.252365 nrn-modeldb-ci-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:37:47.248365 nrn-modeldb-ci-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:37:47.248365 nrn-modeldb-ci-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/.github/workflows/nrn-modeldb-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-05-01 07:37:47.252365 nrn-modeldb-ci-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:37:47.248365 nrn-modeldb-ci-0.2.1/modeldb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/hocscripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26146 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/modeldb-run.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/modeldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16932 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/modelrun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/showgout.hoc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:37:47.248365 nrn-modeldb-ci-0.2.1/modeldb/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/templates/diffreport.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/templates/report.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/modeldb/templates/runtimes.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:37:47.252365 nrn-modeldb-ci-0.2.1/nrn_modeldb_ci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-05-01 07:37:47.000000 nrn-modeldb-ci-0.2.1/nrn_modeldb_ci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-01 07:37:47.000000 nrn-modeldb-ci-0.2.1/nrn_modeldb_ci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 07:37:47.000000 nrn-modeldb-ci-0.2.1/nrn_modeldb_ci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-01 07:37:47.000000 nrn-modeldb-ci-0.2.1/nrn_modeldb_ci.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-01 07:37:47.000000 nrn-modeldb-ci-0.2.1/nrn_modeldb_ci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 07:37:47.000000 nrn-modeldb-ci-0.2.1/nrn_modeldb_ci.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 07:37:47.252365 nrn-modeldb-ci-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-01 07:37:34.000000 nrn-modeldb-ci-0.2.1/setup.py
```

### Comparing `nrn-modeldb-ci-0.2.0/.github/workflows/nrn-modeldb-ci.yaml` & `nrn-modeldb-ci-0.2.1/.github/workflows/nrn-modeldb-ci.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -109,29 +109,40 @@
         #   22203   -> skip: true
         #   156120  -> several model directories
         #   97868   -> failed nrnivmodl
         #   146030  -> curate_patterns
         #   244679  -> no entry in modeldb-run.yaml
         #   rest:   -> currently yielding differences in the pipeline
         echo 'MODELS_TO_RUN=64195 22203 156120 51781 97868 22203 97756 97917 105507 136803 138379 138382 146030 244679 251881' >> $GITHUB_ENV
+
+        # parse PR description for models to run
+       
+        parse_models=$(gh pr view $PR_URL --json body -q '.body | capture("(MODELS_TO_RUN=)(?<models>\\d+( \\d+)*)")')
+        if [ ! -z "$parse_models" ]; then
+          echo "MODELS_TO_RUN=$(echo $parse_models | jq -r .models)" >> $GITHUB_ENV
+        fi
+      
       if: github.event_name == 'pull_request' && inputs.repo == ''
+      env:
+        PR_URL: ${{ github.event.pull_request.html_url }}
+        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
     - name: Install dependencies and project
       id: install-deps
       run: |
         set
         # Set up Xvfb
         sudo apt-get install xvfb
         sudo /usr/bin/Xvfb $DISPLAY -screen 0 1600x1200x24 -noreset -nolock -shmem &  # run in bg
         # Install python dependencies
         python -m pip install --upgrade pip
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
         #Install project in editable mode
         python -m pip install -e .
-        echo "::set-output name=date::$(date -u "+%Y%m")"
+        echo "date=$(date -u "+%Y%m")" >> $GITHUB_OUTPUT
     
     - name: Cache ModelDB models
       id: cache-models
       uses: actions/cache@v3
       with:
         path: |
           cache
@@ -147,15 +158,22 @@
         # Install NEURON V1
         if [[ -d "${DROP_DIR_V1}" ]]; then
           python -m pip install --user --find-links ${DROP_DIR_V1} neuron-nightly
         else
           python -m pip install $NEURON_V1
         fi
         nrn_ver=`python -c "from neuron import __version__ as nrn_ver; print(nrn_ver)"`
-        runmodels --virtual --workdir=$nrn_ver $MODELS_TO_RUN
+        ps uxf # debug
+        runmodels --gout --workdir=$nrn_ver $MODELS_TO_RUN
+        # Filter out the gout data before generating HTML reports. The HTML
+        # diff uses the original gout files on disk anyway. Compress the large
+        # JSON file including gout data for inclusion in the artifacts
+        mv ${nrn_ver}.json ${nrn_ver}-full.json
+        jq -r 'del(.[].gout)' ${nrn_ver}-full.json > ${nrn_ver}.json
+        xz ${nrn_ver}-full.json
         report2html ${nrn_ver}.json
         if [[ -d "${DROP_DIR_V1}" ]]; then
           python -m pip uninstall --yes neuron-nightly==${nrn_ver}
         else
           python -m pip uninstall --yes $NEURON_V1
         fi
         
@@ -167,27 +185,35 @@
         # Install NEURON V2
         if [[ -d "${DROP_DIR_V2}" ]]; then
           python -m pip install --user --find-links ${DROP_DIR_V2} neuron-nightly
         else
           python -m pip install $NEURON_V2
         fi
         nrn_ver=`python -c "from neuron import __version__ as nrn_ver; print(nrn_ver)"`
-        runmodels --virtual --workdir=$nrn_ver $MODELS_TO_RUN
+        ps uxf # debug
+        runmodels --gout --workdir=$nrn_ver $MODELS_TO_RUN
+        # Filter out the gout data before generating HTML reports. The HTML
+        # diff uses the original gout files on disk anyway. Compress the large
+        # JSON file including gout data for inclusion in the artifacts
+        mv ${nrn_ver}.json ${nrn_ver}-full.json
+        jq -r 'del(.[].gout)' ${nrn_ver}-full.json > ${nrn_ver}.json
+        xz ${nrn_ver}-full.json
         report2html ${nrn_ver}.json
         if [[ -d "${DROP_DIR_V2}" ]]; then
           python -m pip uninstall --yes neuron-nightly==${nrn_ver}
         else
           python -m pip uninstall --yes $NEURON_V2
         fi
         echo "nrn2_ver=$nrn_ver" >> $GITHUB_ENV
 
     - name: diffreports2html ${{ env.nrn1_ver }}.json <-> ${{ env.nrn2_ver }}.json
       if: env.NEURON_V1 != env.NEURON_V2
       run: |
         diffreports2html ${nrn1_ver}.json ${nrn2_ver}.json
 
     - uses: actions/upload-artifact@v3
+      if: ${{ always() }}
       with:
         name: ${{ env.nrn1_ver }}-vs-${{ env.nrn2_ver }}
         path: |
-          ./*.json
+          ./*.json.xz
           ./*.html
```

### Comparing `nrn-modeldb-ci-0.2.0/.github/workflows/python-publish.yml` & `nrn-modeldb-ci-0.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nrn-modeldb-ci-0.2.0/LICENSE.txt` & `nrn-modeldb-ci-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nrn-modeldb-ci-0.2.0/PKG-INFO` & `nrn-modeldb-ci-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrn-modeldb-ci
-Version: 0.2.0
+Version: 0.2.1
 Summary: NEURON ModelDB CI tools
 Home-page: https://github.com/neuronsimulator/nrn-modeldb-ci
 Author: EPFL Blue Brain Project & Yale
 Author-email: alexandru.savulescu@epfl.ch
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `nrn-modeldb-ci-0.2.0/README.md` & `nrn-modeldb-ci-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nrn-modeldb-ci-0.2.0/modeldb/commands.py` & `nrn-modeldb-ci-0.2.1/modeldb/commands.py`

 * *Files 21% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         sys.exit(1)
 
     mrm = ModelRunManager(working_dir, gout=gout, clean=clean, norun=norun, inplace=inplace)
     model_list = model_ids if model_ids else None
 
     if virtual:
         from pyvirtualdisplay import Display
-        with Display(manage_global_env=False) as _:
+        with Display(manage_global_env=True, visible=False) as _:
             mrm.run_models(model_list)
     else:
         mrm.run_models(model_list)
 
 
 def getmodels(args=None):
     """getmodels
@@ -174,15 +174,15 @@
 
     json_report = options.pop("<json_report>")
 
     file_loader = FileSystemLoader(os.path.join(Path(__file__).parent.resolve(), 'templates'))
     env = Environment(loader=file_loader)
     template = env.get_template('report.html')
 
-    report_filename = os.path.join(os.path.splitext(json_report)[0] + '.html')
+    report_filename = os.path.join(os.path.splitext(os.path.basename(json_report))[0] + '.html')
     print('Writing {} ...'.format(report_filename))
     with open(report_filename, 'w') as fh, open(json_report, 'r+') as jr:
         fh.write(template.render(
             title="{} : nr-modeldb-ci HTML report".format(json_report),
             json_report=json.load(jr),
         ))
     print('Done.')
@@ -212,20 +212,21 @@
     json_report2 = options.pop("<json_report2>")
 
     file_loader = FileSystemLoader(os.path.join(Path(__file__).parent.resolve(), 'templates'))
     env = Environment(loader=file_loader)
     template = env.get_template('diffreport.html')
     runtime_template = env.get_template('runtimes.html')
 
-    report_title = '{}-vs-{}'.format(os.path.splitext(json_report1)[0],
-                                     os.path.splitext(json_report2)[0])
+
+    report_title = '{}-vs-{}'.format( os.path.splitext(os.path.basename(json_report1))[0],
+                                      os.path.splitext(os.path.basename(json_report2))[0] )
     report_filename = os.path.join(Path(json_report1).resolve().parent, report_title + '.html')
     runtime_report_title = 'Runtimes ' + report_title
     runtime_report_filename = os.path.join(Path(json_report1).resolve().parent, "runtimes-" + report_title + '.html')
-    diff_dict, gout_dict,runtime_dict, v1, v2 = diff_reports(json_report1, json_report2)
+    diff_dict, gout_dict, runtime_dict, stats_dict, v1, v2 = diff_reports(json_report1, json_report2)
 
     print('Writing {} ...'.format(report_filename))
     with open(report_filename, 'w') as fh:
         fh.write(template.render(
             title="{}".format(report_title),
             diff_dict=diff_dict,
             gout_dict=gout_dict),
@@ -236,8 +237,58 @@
         fh.write(runtime_template.render(
             title="{}".format(runtime_report_title),
             runtime_dict=runtime_dict,
             stats={"stats":diff_dict['0']},
             v1=v1,
             v2=v2),
     )
-    print('Done.')
+    print('Done.')
+    # Return a useful status code
+    code = 0
+    if len(diff_dict) > 1:
+        assert "0" in diff_dict  # summary info; not a real diff
+        print("FAILURE: stdout diffs in {}".format(set(diff_dict.keys()) - {"0"}))
+        code = 1
+    if len(gout_dict) > 1:
+        assert "0" in gout_dict  # summary info; not a real diff
+        print("FAILURE: gout diffs in {}".format(set(diff_dict.keys()) - {"0"}))
+        code = 1
+    total_failures = sum(
+        version_stats["Failed models"]["Count"] for version_stats in stats_dict.values()
+    )
+    if total_failures > 0:
+        print(
+            "FAILURE: there were {} failed model builds across {} versions of NEURON".format(
+                total_failures, len(stats_dict)
+            )
+        )
+        code = 1
+    total_runtime_failures = sum(
+        version_stats["Failed runs"]["Count"] for version_stats in stats_dict.values()
+    )
+    if total_runtime_failures > 0:
+        print(
+            "FAILURE: there were {} failed model runs across {} versions of NEURON".format(
+                total_runtime_failures, len(stats_dict)
+            )
+        )
+        code = 1
+    # These are not expected to be different between the two NEURON versions tested
+    assert (
+        len(
+            {
+                version_stats["Skipped runs"]["Count"]
+                for version_stats in stats_dict.values()
+            }
+        )
+        == 1
+    )
+    assert (
+        len(
+            {
+                version_stats["Total nof models run"]
+                for version_stats in stats_dict.values()
+            }
+        )
+        == 1
+    )
+    return code
```

### Comparing `nrn-modeldb-ci-0.2.0/modeldb/config.py` & `nrn-modeldb-ci-0.2.1/modeldb/config.py`

 * *Files identical despite different names*

### Comparing `nrn-modeldb-ci-0.2.0/modeldb/hocscripts.py` & `nrn-modeldb-ci-0.2.1/modeldb/hocscripts.py`

 * *Files identical despite different names*

### Comparing `nrn-modeldb-ci-0.2.0/modeldb/modeldb.py` & `nrn-modeldb-ci-0.2.1/modeldb/modeldb.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,23 +35,28 @@
             zipfile.write(base64.standard_b64decode(url["file_content"]))
 
         if "github" in model_run_info:
             # This means we should try to replace the version of the model that
             # we downloaded from the ModelDB API just above with a version from
             # GitHub
             github = model_run_info["github"]
+            organisation = "ModelDBRepository"
+            suffix = "" # default branch
             if github == "default":
-                suffix = ""
+                pass
             elif github.startswith("pull/"):
                 pr_number = int(github[5:])
                 suffix = "/pull/{}/head".format(pr_number)
+            elif github.startswith('/'):
+                # /org implies that we use the default branch from org/model_id
+                organisation = github[1:]
             else:
                 raise Exception("Invalid value for github key: {}".format(github))
-            github_url = "https://api.github.com/repos/ModelDBRepository/{model_id}/zipball{suffix}".format(
-                model_id=model_id, suffix=suffix
+            github_url = "https://api.github.com/repos/{organisation}/{model_id}/zipball{suffix}".format(
+                model_id=model_id, organisation=organisation, suffix=suffix
             )
             # Replace the local file `model_zip_uri` with the zip file we
             # downloaded from `github_url`
             num_attempts = 3
             status_codes = []
             for _ in range(num_attempts):
                 github_response = requests.get(github_url)
```

### Comparing `nrn-modeldb-ci-0.2.0/modeldb/modelrun.py` & `nrn-modeldb-ci-0.2.1/modeldb/modelrun.py`

 * *Files 8% similar despite different names*

```diff
@@ -95,17 +95,20 @@
     return logstr.replace(model.model_dir, '%model_dir%') if len(model.model_dir) else logstr
 
 
 def append_log(model, model_sink, text):
     model_sink.extend(curate_log_string(model, text).split('\n'))
 
 
-def run_commands(model, cmds, work_dir=None):
+def run_commands(model, cmds, env={}, work_dir=None):
+    full_env = os.environ
+    full_env.update(env)
     out, _ = subprocess.Popen(
             cmds,
+            env=full_env,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
             universal_newlines=True,
             cwd=model.model_dir if work_dir is None else work_dir,
         ).communicate()
 
     model.logs.extend(curate_log_string(model, out).split('\n'))
@@ -130,15 +133,29 @@
 
 def clean_model_dir(model):
     # delete x86_64 folder
     run_commands(model, ["/bin/sh", "-c", "rm -rf ./{}/".format(platform.machine())], work_dir=model.run_info["start_dir"])
 
 
 def compile_mods(model, mods):
-    run_commands(model, ["nrnivmodl"] + mods, work_dir=model.run_info["start_dir"])
+    # Unfortunately nrnivmodl doesn't have an option to steer how much build
+    # parallellism it tries to do, it just hardcodes `make -j 4`. Because we
+    # parallelise over models, at a higher level, we want to remove this
+    # internal parallelism from nrnivmodl. In the CI we install NEURON using
+    # pip from precompiled wheels, and the real nrnivmodl is hidden behind
+    # an extra layer of wrappers. This makes it inconvenient to change the
+    # hardcoded value. Instead, we try to achieve the same effect using Make's
+    # environment variables. --max-load 0.0 should ban >1 job being launched if
+    # the system load is larger than zero.
+    run_commands(
+        model,
+        ["nrnivmodl"] + mods,
+        env={"MAKEFLAGS": " --max-load 0.0"},
+        work_dir=model.run_info["start_dir"],
+    )
 
 
 def build_driver_hoc(model):
     model.run_info["driver"] = os.path.join(model.model_dir, "driver.hoc")
 
     with open(model.run_info["driver"], "w") as drv:
         drv.write(driver_hoc_header.format(model_dir=model.model_dir))
@@ -188,24 +205,26 @@
 
 def prepare_model(model):
     # unzip model from cache
     with zipfile.ZipFile(
             os.path.join(MODELS_ZIP_DIR, str(model.id) + ".zip"), "r"
     ) as zip_ref:
         model_dir = os.path.join(
-            model.working_dir, os.path.dirname(zip_ref.infolist()[0].filename)
+            model.working_dir,
+            str(model.id),
+            os.path.dirname(zip_ref.infolist()[0].filename),
         )
-        model_run_info_file = os.path.join(model_dir, str(model.id) + '.yaml')
+        model_run_info_file = os.path.join(model_dir, str(model.id) + ".yaml")
         if model._inplace and os.path.isfile(model_run_info_file):
             with open(model_run_info_file) as run_info_file:
                 model["run_info"] = yaml.load(run_info_file, yaml.Loader)
         else:
             if model._clean and is_dir_non_empty(model_dir):
                 shutil.rmtree(model_dir)
-            zip_ref.extractall(model.working_dir)
+            zip_ref.extractall(os.path.join(model.working_dir, str(model.id)))
 
             # set model_dir
             model.run_info["model_dir"] = model_dir
 
             # write driver.hoc
             build_driver_hoc(model)
```

### Comparing `nrn-modeldb-ci-0.2.0/modeldb/progressbar.py` & `nrn-modeldb-ci-0.2.1/modeldb/progressbar.py`

 * *Files identical despite different names*

### Comparing `nrn-modeldb-ci-0.2.0/modeldb/report.py` & `nrn-modeldb-ci-0.2.1/modeldb/report.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,47 @@
-import numpy as np
 import json
 import re
 import difflib
 import logging
 import os
+import shlex
 import subprocess
 from .modeldb import ModelDB
 from pygments import highlight
 from pygments.lexers import DiffLexer
 from pygments.formatters import HtmlFormatter
 
 
 mdb = ModelDB()
 
+
 def curate_run_data(run_data, model=None):
     curated_data = run_data
-
+    
     regex_dict = {
         # /../nrniv: Assignment to modern physical constant FARADAY	<-> ./x86_64/special: Assignment to modern physical constant FARADAY
         "^/.*?/nrniv:": "%neuron-executable%:",
         "^\\./x86_64/special:": "%neuron-executable%:",
         # nrniv: unable to open font "*helvetica-medium-r-normal*--14*", using "fixed" <-> special: unableto open font "*helvetica-medium-r-normal*--14*", using "fixed"
         "^nrniv:": "%neuron-executable%:",
         "^special:": "%neuron-executable%:",
-        "(Mon|Tue|Wed|Thu|Fri|Sat|Sun) (Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec) \d+ \d+:\d+:\d+ [A-Z]+ \d+": "%date_command%",
+        "(Mon|Tue|Wed|Thu|Fri|Sat|Sun) (Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)\s+\d+\s+\d+:\d+:\d+ [A-Z\s]+ \d+": "%date_command%",
         "total run time [0-9\.]+": "total run time %run_time%",
         "(^.*distutils.*$)": "",
+        "/.*?/lib/python.*/site-packages/" : "%python-site-packages%",
     }
-
+    
     for model_specific_substitution in mdb.run_instr.get(model, {}).get("curate_patterns", []):
         regex_dict[model_specific_substitution["pattern"]] = model_specific_substitution["repl"]
 
     for regex_key, regex_value in regex_dict.items():
         updated_data = []
+        pattern = re.compile(regex_key)
         for line in curated_data:
-            new_line, number_of_subs = re.subn(regex_key, regex_value, line)
+            new_line, number_of_subs = pattern.subn(regex_value, line)
             if number_of_subs:
                 logging.debug("{} matched {} time(s)".format(regex_key, number_of_subs))
                 logging.debug("{} -> {}".format(line, new_line))
             # if we are replacing a full line with an empty string, don't add it to the curated data
             if new_line:
                 updated_data.append(new_line)
         curated_data = updated_data
@@ -54,25 +57,33 @@
     with open(report1_json, 'r+') as f, open(report2_json, 'r+') as f2:
         data_a = json.load(f)
         data_b = json.load(f2)
 
         hd = difflib.HtmlDiff()
         v1 = data_a["0"]["NEURON version"]
         v2 = data_b["0"]["NEURON version"]
-        diff_dict["0"] = hd.make_table(json.dumps(data_a["0"], indent='\t').split('\n'),
-                                             json.dumps(data_b["0"], indent='\t').split('\n')).replace("\n", "")
+        diff_dict["0"] = hd.make_table(
+            json.dumps(data_a["0"], indent="\t").split("\n"),
+            json.dumps(data_b["0"], indent="\t").split("\n"),
+        ).replace("\n", "")
+        stats_dict = {v1: data_a["0"]["Stats"], v2: data_b["0"]["Stats"]}
         for k in data_a.keys():
             if int(k) == 0:
                 continue  # skip info key
-
+            if k not in data_b:
+                ud_empty = difflib.unified_diff(data_a[k]["nrn_run"], ["Accession number {} not found in report2".format(k)])
+                diff_dict[k] = highlight('\n'.join(ud_empty), DiffLexer(), HtmlFormatter(linenos=True, cssclass="colorful", full=True))
+                continue            
             curated_a = curate_run_data(data_a[k]["nrn_run"], model=int(k))
             curated_b = curate_run_data(data_b[k]["nrn_run"], model=int(k))
+            start_dir_a = data_a[k]["run_info"]["start_dir"] if "run_info" in data_a[k] and "start_dir" in data_a[k]["run_info"] else "unknown"
+            start_dir_b = data_b[k]["run_info"]["start_dir"] if "run_info" in data_b[k] and "start_dir" in data_b[k]["run_info"] else "unknown"
             if curated_a != curated_b:
-                ud = difflib.unified_diff(curated_a, curated_b,  fromfile=data_a[k]["run_info"]["start_dir"],
-                                             tofile=data_b[k]["run_info"]["start_dir"])
+                ud = difflib.unified_diff(curated_a, curated_b,  fromfile=start_dir_a,
+                                             tofile=start_dir_b)
                 diff_dict[k] = highlight('\n'.join(ud), DiffLexer(), HtmlFormatter(linenos=True, cssclass="colorful", full=True))
                 
             def _speedup(a, b):
                 dict = {}
                 dict["v1"] = a
                 dict["v2"] = b
                 # compute slowdown/speedup relative to runtime_b (negative means slowdown)
@@ -90,14 +101,16 @@
                         runtime_dict[k][runkey] = _speedup(data_a[k]["run_times"][runkey], data_b[k]["run_times"][runkey])
                 
                 # compare gout
                 gout_a_file = os.path.join(data_a[k]["run_info"]["start_dir"], "gout")
                 gout_b_file = os.path.join(data_b[k]["run_info"]["start_dir"], "gout")
                 # gout may be missing in one of the paths. `diff -N` treats non-existent files as empty.
                 if os.path.isfile(gout_a_file) or os.path.isfile(gout_b_file):
-                    diff_out = subprocess.getoutput("diff -uN {} {} | head -n 30".format(gout_a_file, gout_b_file))
+                    diff_out = subprocess.getoutput(
+                        "diff -uN --speed-large-files {} {} | head -n 30".format(
+                            shlex.quote(gout_a_file), shlex.quote(gout_b_file)
+                        )
+                    )
                     if diff_out:
                         gout_dict[k] = highlight(diff_out, DiffLexer(), HtmlFormatter(linenos=True, cssclass="colorful", full=True))
 
-    return diff_dict, gout_dict, runtime_dict, v1, v2
-
-
+    return diff_dict, gout_dict, runtime_dict, stats_dict, v1, v2
```

### Comparing `nrn-modeldb-ci-0.2.0/modeldb/showgout.hoc` & `nrn-modeldb-ci-0.2.1/modeldb/showgout.hoc`

 * *Files identical despite different names*

### Comparing `nrn-modeldb-ci-0.2.0/modeldb/templates/diffreport.html` & `nrn-modeldb-ci-0.2.1/modeldb/templates/diffreport.html`

 * *Files identical despite different names*

### Comparing `nrn-modeldb-ci-0.2.0/modeldb/templates/report.html` & `nrn-modeldb-ci-0.2.1/modeldb/templates/report.html`

 * *Files identical despite different names*

### Comparing `nrn-modeldb-ci-0.2.0/modeldb/templates/runtimes.html` & `nrn-modeldb-ci-0.2.1/modeldb/templates/runtimes.html`

 * *Files identical despite different names*

### Comparing `nrn-modeldb-ci-0.2.0/nrn_modeldb_ci.egg-info/PKG-INFO` & `nrn-modeldb-ci-0.2.1/nrn_modeldb_ci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrn-modeldb-ci
-Version: 0.2.0
+Version: 0.2.1
 Summary: NEURON ModelDB CI tools
 Home-page: https://github.com/neuronsimulator/nrn-modeldb-ci
 Author: EPFL Blue Brain Project & Yale
 Author-email: alexandru.savulescu@epfl.ch
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `nrn-modeldb-ci-0.2.0/nrn_modeldb_ci.egg-info/SOURCES.txt` & `nrn-modeldb-ci-0.2.1/nrn_modeldb_ci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nrn-modeldb-ci-0.2.0/setup.py` & `nrn-modeldb-ci-0.2.1/setup.py`

 * *Files identical despite different names*

