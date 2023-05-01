# Comparing `tmp/module_qc_analysis_tools-1.3.1rc3.tar.gz` & `tmp/module_qc_analysis_tools-1.3.1rc4.tar.gz`

## Comparing `module_qc_analysis_tools-1.3.1rc3.tar` & `module_qc_analysis_tools-1.3.1rc4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/.flake8
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/.gitmodules
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/tbump.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/__init__.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/_version.py
--rw-r--r--   0        0        0     8794 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py
--rw-r--r--   0        0        0    17806 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py
--rw-r--r--   0        0        0    11067 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py
--rw-r--r--   0        0        0     9559 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/IV_MEASURE.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py
--rw-r--r--   0        0        0     9228 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py
--rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py
--rw-r--r--   0        0        0    23808 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/SLDO.py
--rw-r--r--   0        0        0     9657 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/TUNING.py
--rw-r--r--   0        0        0    11972 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/__init__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/__main__.py
--rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/globals.py
--rwxr-xr-x   0        0        0     8167 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/load_yarr_scans.py
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/main.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/overwrite_config.py
--rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/update_chip_config.py
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/data/analysis_cuts.json
--rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/data/pixel_classification.json
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/data/schema/info_schema.json
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/data/schema/input_yarr_schema.json
--rw-r--r--   0        0        0    21307 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/utils/analysis.py
--rw-r--r--   0        0        0    11368 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/utils/classification.py
--rw-r--r--   0        0        0    34380 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/utils/misc.py
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/tests/test_cli.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/tests/test_package.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/LICENSE
--rw-r--r--   0        0        0    21444 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/README.md
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/pyproject.toml
--rw-r--r--   0        0        0    23571 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc3/PKG-INFO
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/.flake8
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/.gitmodules
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/tbump.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/__init__.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/_version.py
+-rw-r--r--   0        0        0    10062 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py
+-rw-r--r--   0        0        0    18774 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py
+-rw-r--r--   0        0        0    12036 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py
+-rw-r--r--   0        0        0     9548 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/IV_MEASURE.py
+-rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py
+-rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py
+-rw-r--r--   0        0        0     8710 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py
+-rw-r--r--   0        0        0    24858 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/SLDO.py
+-rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/TUNING.py
+-rw-r--r--   0        0        0    12915 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py
+-rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/__init__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/__main__.py
+-rw-r--r--   0        0        0     6023 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/globals.py
+-rwxr-xr-x   0        0        0     8167 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/load_yarr_scans.py
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/main.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/overwrite_config.py
+-rw-r--r--   0        0        0     8646 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/update_chip_config.py
+-rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/data/analysis_cuts.json
+-rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/data/pixel_classification.json
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/data/schema/info_schema.json
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/data/schema/input_yarr_schema.json
+-rw-r--r--   0        0        0    25523 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/utils/analysis.py
+-rw-r--r--   0        0        0    12471 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/utils/classification.py
+-rw-r--r--   0        0        0    34039 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/utils/misc.py
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/tests/test_cli.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/tests/test_package.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/LICENSE
+-rw-r--r--   0        0        0    21574 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/README.md
+-rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/pyproject.toml
+-rw-r--r--   0        0        0    23698 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc4/PKG-INFO
```

### Comparing `module_qc_analysis_tools-1.3.1rc3/.gitlab-ci.yml` & `module_qc_analysis_tools-1.3.1rc4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc3/.pre-commit-config.yaml` & `module_qc_analysis_tools-1.3.1rc4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc3/tbump.toml` & `module_qc_analysis_tools-1.3.1rc4/tbump.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2231 2e33 2e31 7263 3322 0a0a  t = "1.3.1rc3"..
+00000010: 7420 3d20 2231 2e33 2e31 7263 3422 0a0a  t = "1.3.1rc4"..
 00000020: 2320 4578 616d 706c 6520 6f66 2061 2073  # Example of a s
 00000030: 656d 7665 7220 7265 6765 7870 2e0a 2320  emver regexp..# 
 00000040: 4d61 6b65 2073 7572 6520 7468 6973 206d  Make sure this m
 00000050: 6174 6368 6573 2063 7572 7265 6e74 5f76  atches current_v
 00000060: 6572 7369 6f6e 2062 6566 6f72 650a 2320  ersion before.# 
 00000070: 7573 696e 6720 7462 756d 700a 7265 6765  using tbump.rege
 00000080: 7820 3d20 2727 270a 2020 283f 503c 6d61  x = '''.  (?P<ma
@@ -15,15 +15,15 @@
 000000e0: 290a 2020 293f 0a20 2027 2727 0a0a 5b67  ).  )?.  '''..[g
 000000f0: 6974 5d0a 2320 5468 6520 6375 7272 656e  it].# The curren
 00000100: 7420 7665 7273 696f 6e20 7769 6c6c 2067  t version will g
 00000110: 6574 2075 7064 6174 6564 2077 6865 6e20  et updated when 
 00000120: 7462 756d 7020 6973 2072 756e 0a6d 6573  tbump is run.mes
 00000130: 7361 6765 5f74 656d 706c 6174 6520 3d20  sage_template = 
 00000140: 2242 756d 7020 7665 7273 696f 6e3a 2031  "Bump version: 1
-00000150: 2e33 2e31 7263 3320 e286 9220 7b6e 6577  .3.1rc3 ... {new
+00000150: 2e33 2e31 7263 3420 e286 9220 7b6e 6577  .3.1rc4 ... {new
 00000160: 5f76 6572 7369 6f6e 7d22 0a74 6167 5f74  _version}".tag_t
 00000170: 656d 706c 6174 6520 3d20 2276 7b6e 6577  emplate = "v{new
 00000180: 5f76 6572 7369 6f6e 7d22 0a0a 2320 466f  _version}"..# Fo
 00000190: 7220 6561 6368 2066 696c 6520 746f 2070  r each file to p
 000001a0: 6174 6368 2c20 6164 6420 6120 5b5b 6669  atch, add a [[fi
 000001b0: 6c65 5d5d 2063 6f6e 6669 670a 2320 7365  le]] config.# se
 000001c0: 6374 696f 6e20 636f 6e74 6169 6e69 6e67  ction containing
```

### Comparing `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py` & `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,262 +1,256 @@
 from __future__ import annotations
 
 import logging
 from datetime import datetime
 from pathlib import Path
 
-import matplotlib.pyplot as plt
 import numpy as np
 import typer
 from module_qc_data_tools import (
+    convert_serial_to_name,
     get_layer_from_sn,
-    load_json,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 
 from module_qc_analysis_tools import __version__
 from module_qc_analysis_tools.cli.globals import (
     CONTEXT_SETTINGS,
     OPTIONS,
-    FitMethod,
     LogLevel,
 )
 from module_qc_analysis_tools.utils.analysis import (
     check_layer,
+    get_layer,
     perform_qc_analysis,
-    submit_results,
+    print_result_summary,
+)
+from module_qc_analysis_tools.utils.classification import (
+    check_input_yarr_config,
+    check_input_yarr_data,
+    classify_pixels,
+    count_pixels,
+    format_pixel_input,
+    print_pixel_classification,
+    read_json,
 )
 from module_qc_analysis_tools.utils.misc import (
-    DataExtractor,
-    JsonChecker,
     bcolors,
-    get_inputs,
     get_qc_config,
-    get_time_stamp,
-    linear_fit,
-    linear_fit_np,
 )
 
 app = typer.Typer(context_settings=CONTEXT_SETTINGS)
 
+log = logging.getLogger("analysis")
+
 
 @app.command()
 def main(
-    input_meas: Path = OPTIONS["input_meas"],
-    base_output_dir: Path = OPTIONS["output_dir"],
+    input_yarr: Path = OPTIONS["input_yarr_config"],
     qc_criteria_path: Path = OPTIONS["qc_criteria"],
-    input_layer: str = OPTIONS["layer"],
+    pixel_classification_path: Path = OPTIONS["pixel_classification"],
+    base_output_dir: Path = OPTIONS["output_dir"],
     permodule: bool = OPTIONS["permodule"],
-    submit: bool = OPTIONS["submit"],
-    site: str = OPTIONS["site"],
-    fit_method: FitMethod = OPTIONS["fit_method"],
+    input_layer: str = OPTIONS["layer"],
     verbosity: LogLevel = OPTIONS["verbosity"],
 ):
-    log = logging.getLogger(__name__)
-    log.setLevel(verbosity.value)
-
-    if submit and site == "":
-        log.error(
-            bcolors.ERROR
-            + "You have supplied the --submit option without specifying --site (testing site). Please specify your testing site if you would like to submit these results"
-            + bcolors.ENDC
-        )
-        return
-
-    log.info("")
-    log.info(" ===============================================")
-    log.info(" \tPerforming ADC calibration analysis")
-    log.info(" ===============================================")
-    log.info("")
-
     test_type = Path(__file__).stem
+    qc_config = get_qc_config(qc_criteria_path, test_type)
 
     time_start = datetime.now().strftime("%Y-%m-%d_%H%M%S")
     output_dir = base_output_dir.joinpath(test_type).joinpath(f"{time_start}")
     output_dir.mkdir(parents=True, exist_ok=False)
 
-    allinputs = get_inputs(input_meas, test_type)
-    qc_config = get_qc_config(qc_criteria_path, test_type)
+    log.setLevel(verbosity.value)
+    log.addHandler(logging.FileHandler(f"{output_dir}/output.log"))
+
+    log.info("")
+    log.info(" ====================================================")
+    log.info(" \tPerforming pixel failure analysis")
+    log.info(" ====================================================")
+    log.info("")
+
+    input_data = read_json(input_yarr)
+    check_input_yarr_config(input_data, path=input_yarr)
+    datadir = input_data["datadir"]
+    module_sn = input_data["module"]["serialNumber"]
+    layer = get_layer_from_sn(module_sn)
+
+    if input_layer == "Unknown":
+        try:
+            layer = get_layer_from_sn(module_sn)
+        except Exception:
+            log.error(bcolors.WARNING + " Something went wrong." + bcolors.ENDC)
+    else:
+        log.warning(
+            bcolors.WARNING
+            + " Overwriting default layer config {} with manual input {}!".format(
+                get_layer_from_sn(module_sn), input_layer
+            )
+            + bcolors.ENDC
+        )
+        layer = input_layer
+    check_layer(layer)
+
+    pixel_classification = read_json(pixel_classification_path)
+    if not pixel_classification.get(test_type):
+        log.error(
+            bcolors.BADRED
+            + f"Pixel failure selection for {test_type} not found in {pixel_classification_path}! Please check. "
+            + bcolors.ENDC
+        )
+        raise RuntimeError()
 
     alloutput = []
-    timestamps = []
-    for filename in sorted(allinputs):
-        log.info("")
-        log.info(f" Loading {filename}")
-        meas_timestamp = get_time_stamp(filename)
-        inputDFs = load_json(filename)
-        log.debug(
-            f" There are results from {len(inputDFs)} chip(s) stored in this file"
+    for c in input_data["chip"]:
+        chipSN = c["serialNumber"]
+        chipName = convert_serial_to_name(chipSN)
+        filepaths = c["filepaths"]
+        results = {}
+        skip_chip = False
+
+        # Initialize array to track pixel failures
+        pix_fail = np.zeros(153600, dtype=np.uint16)
+
+        # Initialize int to track which classifications have been checked
+        record_fail = 0
+
+        log.debug(f"Performing pixel failure analysis on chip {c['serialNumber']}")
+
+        """ Prepare output json file """
+        outputDF = outputDataFrame()
+        outputDF.set_test_type(test_type)
+        outputDF.set_serial_num(chipSN)
+        data = qcDataFrame()
+        data.add_property(
+            "ANALYSIS_VERSION",
+            __version__,
         )
-        for inputDF in inputDFs:
-            """Check file integrity"""
-            checker = JsonChecker(inputDF, test_type)
-
-            try:
-                checker.check()
-            except BaseException as exc:
-                log.exception(exc)
-                log.warning(
-                    bcolors.WARNING
-                    + " JsonChecker check not passed, skipping this input."
-                    + bcolors.ENDC
-                )
-                continue
-            else:
-                log.debug(" JsonChecker check passed!")
-                pass
+        data.add_meta_data("QC_LAYER", layer)
 
-            """  Get info  """
-            qcframe = inputDF.get_results()
-            metadata = qcframe.get_meta_data()
-
-            if input_layer == "Unknown":
-                try:
-                    layer = get_layer_from_sn(metadata.get("ModuleSN"))
-                except Exception:
-                    log.error(bcolors.WARNING + " Something went wrong." + bcolors.ENDC)
-            else:
-                log.warning(
-                    bcolors.WARNING
-                    + " Overwriting default layer config {} with manual input {}!".format(
-                        get_layer_from_sn(metadata.get("ModuleSN")), input_layer
+        # Loop through pixel failure tests from config file
+        for test_name, params in pixel_classification.get(test_type).items():
+            log.debug(f"Performing {test_name}")
+
+            test_input = params.get("input")
+            test_method = params.get("method")
+            test_params = params.get("params")
+
+            # Get layer-specific params if necessary
+            if type(test_params) is dict:
+                layer_name = get_layer(layer)
+                layer_bounds = test_params.get(layer_name)
+                if not layer_bounds:
+                    log.error(
+                        bcolors.ERROR
+                        + f" QC selections for {test_name} and {layer_name} do not exist - please check! Skipping."
+                        + bcolors.ENDC
                     )
-                    + bcolors.ENDC
-                )
-                layer = input_layer
-            check_layer(layer)
+                    continue
+                test_params = layer_bounds
 
-            try:
-                chipname = metadata.get("Name")
-                log.debug(f" Found chip name = {chipname} from chip config")
-            except Exception:
-                log.warning(
+            # Check if we have data for that test
+            if test_input not in filepaths.keys():
+                log.info(
                     bcolors.WARNING
-                    + "Chip name not found in input from {filename}, skipping."
+                    + f"YARR data for {test_name} not found in {input_yarr} ({test_input}). PIXEL_FAILURE_ANALYSIS cannot be performed on this chip. Exiting."
                     + bcolors.ENDC
                 )
-                continue
+                skip_chip = True
+                break
 
-            """  Calculate quanties   """
-            # Vmux conversion is embedded.
-            extractor = DataExtractor(inputDF, test_type)
-            calculated_data = extractor.calculate()
-
-            """        Plotting       """
-            x_key = "ADC_Vmux8"
-            x = calculated_data.pop(x_key)
-            y_key = "VcalMed"
-
-            value = calculated_data.get(y_key)
-            if fit_method.value == "root":
-                p1, p0 = linear_fit(x["Values"], value["Values"])
-            if fit_method.value == "numpy":
-                p1, p0 = linear_fit_np(x["Values"], value["Values"])
-            # Convert from V to mV
-            p1mv = p1 * 1000
-            p0mv = p0 * 1000
-            fig, ax1 = plt.subplots()
-            ax1.plot(
-                x["Values"],
-                value["Values"],
-                "o",
-                label="Measured data",
-                markersize=10,
-            )
-            x_line = np.linspace(x["Values"][0], x["Values"][-1], 100)
-            ax1.plot(x_line, p1 * x_line + p0, "r--", label="Fitted line")
-            ax1.text(
-                x["Values"][0],
-                0.75 * value["Values"][-1],
-                f"y = {p1:.4e} * x + {p0:.4e}",
-            )
-            ax1.set_xlabel(f"{x_key}[{x['Unit']}]")
-            ax1.set_ylabel(f"{y_key}[{value['Unit']}]")
-            ax1.set_title(chipname)
-            ax1.legend()
-            outfile = output_dir.joinpath(f"{chipname}.png")
-            log.info(f" Saving {outfile}")
-            fig.savefig(f"{outfile}")
-
-            # Load values to dictionary for QC analysis
-            results = {}
-            results.update({"ADC_CALIBRATION_SLOPE": round(p1mv, 3)})
-            results.update({"ADC_CALIBRATION_OFFSET": round(p0mv, 3)})
-
-            # Perform QC analysis
-            passes_qc = perform_qc_analysis(
-                test_type, qc_config, layer, results, verbosity.value
-            )
-            if passes_qc == -1:
-                log.error(
-                    bcolors.ERROR
-                    + f" QC analysis for {chipname} was NOT successful. Please fix and re-run. Continuing to next chip.."
-                    + bcolors.ENDC
-                )
-                continue
-            log.info("")
-            if passes_qc:
-                log.info(
-                    f" Chip {chipname} passes QC? "
-                    + bcolors.OKGREEN
-                    + f"{passes_qc}"
-                    + bcolors.ENDC
-                )
+            # Read input YARR scan
+            input_data_path = datadir + "/" + filepaths[test_input]
+            input_data = read_json(Path(input_data_path))
+            check_input_yarr_data(input_data, path=input_data_path)
+
+            pix_data, pix_index = format_pixel_input(input_data.get("Data"))
+
+            # Calculate relevant quantities
+            if test_method == "mean":
+                if "TDAC" not in test_name:
+                    pix_data = pix_data[pix_data > 0]
+                results.update({"PIXEL_FAILURE_" + test_name: np.mean(pix_data)})
+            elif test_method == "rms":
+                if "TDAC" not in test_name:
+                    pix_data = pix_data[pix_data > 0]
+                results.update({"PIXEL_FAILURE_" + test_name: np.std(pix_data)})
             else:
-                log.info(
-                    f" Chip {chipname} passes QC? "
-                    + bcolors.BADRED
-                    + f"{passes_qc}"
-                    + bcolors.ENDC
+                log.debug(f"Classifying pixels failing {test_name}")
+                pix_fail, record_fail = classify_pixels(
+                    pix_data, pix_fail, record_fail, test_name, test_method, test_params
                 )
-            log.info("")
+                if np.isscalar(pix_fail):
+                    continue
 
-            """ Output a json file """
-            outputDF = outputDataFrame()
-            outputDF.set_test_type(test_type)
-            data = qcDataFrame()
-            data._meta_data.update(metadata)
-            data.add_property(
-                "ANALYSIS_VERSION",
-                __version__,
+        if skip_chip:
+            continue
+
+        chiplog = logging.FileHandler(f"{output_dir}/{chipName}.log")
+        log.addHandler(chiplog)
+        test_names = pixel_classification.get(test_type).keys()
+        failure_summary = count_pixels(pix_fail, record_fail, test_names)
+        for fname, nfail in failure_summary.items():
+            data.add_parameter(
+                "PIXEL_FAILURE_" + fname, round(nfail.get("dependent"), 3)
             )
-            data.add_meta_data(
-                "MEASUREMENT_VERSION",
-                qcframe.get_properties().get(test_type + "_MEASUREMENT_VERSION"),
+
+        print_pixel_classification(failure_summary, test_type, output_dir, chipName)
+        total_electrically_failing = list(failure_summary.values())[-1].get(
+            "integrated"
+        )
+        results.update({"ELECTRICALLY_FAILED": total_electrically_failing})
+        data.add_parameter(
+            "PIXEL_FAILURE_ELECTRICALLY_FAILED", total_electrically_failing
+        )
+
+        passes_qc, summary = perform_qc_analysis(test_type, qc_config, layer, results)
+        print_result_summary(summary, test_type, output_dir, chipName)
+        if passes_qc == -1:
+            log.error(
+                bcolors.ERROR
+                + f" QC analysis for {chipName} was NOT successful. Please fix and re-run. Continuing to next chip.."
+                + bcolors.ENDC
             )
-            data.add_meta_data("QC_LAYER", layer)
-            for key, value in results.items():
-                data.add_parameter(key, value)
-            outputDF.set_results(data)
-            outputDF.set_pass_flag(passes_qc)
-            if submit:
-                submit_results(
-                    outputDF.to_dict(True),
-                    time_start,
-                    site,
-                    output_dir.joinpath("submit.txt"),
-                    layer,
-                )
-            if permodule:
-                alloutput += [outputDF.to_dict(True)]
-                timestamps += [meas_timestamp]
-            else:
-                outfile = output_dir.joinpath(f"{chipname}.json")
-                log.info(f" Saving output of analysis to: {outfile}")
-                save_dict_list(outfile, [outputDF.to_dict(True)])
-    if permodule:
-        # Only store results from same timestamp into same file
-        dfs = np.array(alloutput)
-        tss = np.array(timestamps)
-        for x in np.unique(tss):
-            outfile = output_dir.joinpath("module.json")
-            log.info(f" Saving output of analysis to: {outfile}")
-            save_dict_list(
-                outfile,
-                dfs[tss == x].tolist(),
+            continue
+        log.info("")
+        if passes_qc:
+            log.info(
+                f" Chip {chipName} passes QC? "
+                + bcolors.OKGREEN
+                + f"{passes_qc}"
+                + bcolors.ENDC
             )
+        else:
+            log.info(
+                f" Chip {chipName} passes QC? "
+                + bcolors.BADRED
+                + f"{passes_qc}"
+                + bcolors.ENDC
+            )
+        log.info("")
+        log.removeHandler(chiplog)
+        chiplog.close()
+
+        outputDF.set_results(data)
+        outputDF.set_pass_flag(passes_qc)
+
+        if permodule:
+            alloutput += [outputDF.to_dict(True)]
+        else:
+            outfile = output_dir.joinpath(f"{chipName}.json")
+            log.info(f" Saving output of analysis to: {outfile}")
+            save_dict_list(outfile, [outputDF.to_dict(True)])
+
+    if permodule:
+        outfile = output_dir.joinpath("module.json")
+        log.info(f" Saving output of analysis to: {outfile}")
+        save_dict_list(
+            outfile,
+            alloutput,
+        )
 
 
 if __name__ == "__main__":
     typer.run(main)
```

### Comparing `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py` & `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     OPTIONS,
     FitMethod,
     LogLevel,
 )
 from module_qc_analysis_tools.utils.analysis import (
     check_layer,
     perform_qc_analysis,
+    print_result_summary,
     submit_results,
 )
 from module_qc_analysis_tools.utils.misc import (
     DataExtractor,
     JsonChecker,
     bcolors,
     get_inputs,
@@ -38,15 +39,15 @@
     getVmuxMap,
     linear_fit,
     linear_fit_np,
 )
 
 app = typer.Typer(context_settings=CONTEXT_SETTINGS)
 
-log = logging.getLogger(__name__)
+log = logging.getLogger("analysis")
 
 EMPTY_VAL = -1
 
 
 def get_NtcCalPar(metadata):
     # Read NTC parameters from metadata in the chip config.
     if "NtcCalPar" in metadata:
@@ -191,37 +192,33 @@
     input_layer: str = OPTIONS["layer"],
     permodule: bool = OPTIONS["permodule"],
     submit: bool = OPTIONS["submit"],
     site: str = OPTIONS["site"],
     fit_method: FitMethod = OPTIONS["fit_method"],
     verbosity: LogLevel = OPTIONS["verbosity"],
 ):
+    test_type = Path(__file__).stem
+    time_start = datetime.now().strftime("%Y-%m-%d_%H%M%S")
+
+    output_dir = base_output_dir.joinpath(test_type).joinpath(f"{time_start}")
+    output_dir.mkdir(parents=True, exist_ok=False)
+
     log.setLevel(verbosity.value)
+    log.addHandler(logging.FileHandler(f"{output_dir}/output.log"))
 
-    if submit and site == "":
-        log.error(
-            bcolors.ERROR
-            + "You have supplied the --submit option without specifying --site (testing site). Please specify your testing site if you would like to submit these results"
-            + bcolors.ENDC
-        )
-        return
+    # Turn off matplotlib DEBUG messages
+    plt.set_loglevel(level="warning")
 
     log.info("")
     log.info(" ===============================================")
     log.info(" \tPerforming Analog Readback analysis")
     log.info(" ===============================================")
     log.info("")
 
-    test_type = Path(__file__).stem
-    time_start = datetime.now().strftime("%Y-%m-%d_%H%M%S")
-
-    output_dir = base_output_dir.joinpath(test_type).joinpath(f"{time_start}")
-    output_dir.mkdir(parents=True, exist_ok=False)
-
-    allinputs = get_inputs(input_meas, test_type)
+    allinputs = get_inputs(input_meas)
     qc_config = get_qc_config(qc_criteria_path, test_type)
 
     alloutput = []
     timestamps = []
 
     alloutput_int_biases = []
     timestamps_int_biases = []
@@ -286,26 +283,48 @@
                 log.warning(
                     bcolors.WARNING
                     + "Chip name not found in input from {filename}, skipping."
                     + bcolors.ENDC
                 )
                 continue
 
+            institution = metadata.get("Institution")
+            if site != "" and institution != "":
+                log.warning(
+                    bcolors.WARNING
+                    + " Overwriting default institution {} with manual input {}!".format(
+                        institution, site
+                    )
+                    + bcolors.ENDC
+                )
+                institution = site
+            elif site != "":
+                institution = site
+
+            if institution == "":
+                log.error(
+                    bcolors.ERROR
+                    + "No institution found. Please specify your testing site either in the measurement data or specify with the --site option. "
+                    + bcolors.ENDC
+                )
+                return
+
             # Create an output DF for each chip
             if chipname not in data:
                 data[chipname] = qcDataFrame()
                 data[chipname].add_property(
                     "ANALYSIS_VERSION",
                     __version__,
                 )
                 data[chipname].add_meta_data(
                     "MEASUREMENT_VERSION",
                     qcframe.get_properties().get(test_type + "_MEASUREMENT_VERSION"),
                 )
                 data[chipname].add_meta_data("QC_LAYER", layer)
+                data[chipname].add_meta_data("INSTITUTION", institution)
                 data[chipname]._meta_data.update(metadata)
                 int_biases[chipname] = {}
 
             """  Calculate quanties   """
             # Vmux conversion is embedded.
             extractor = DataExtractor(inputDF, test_type)
             calculated_data = extractor.calculate()
@@ -405,21 +424,23 @@
         """ Output a json file """
         for key, df in data.items():
             outputDF = outputDataFrame()
             outputDF.set_test_type(test_type)
             outputDF.set_results(df)
 
             # Perform QC analysis
-            passes_qc = perform_qc_analysis(
+            chiplog = logging.FileHandler(f"{output_dir}/{chipname}.log")
+            log.addHandler(chiplog)
+            passes_qc, summary = perform_qc_analysis(
                 test_type,
                 qc_config,
                 layer,
                 results.get(key),
-                verbosity.value,
             )
+            print_result_summary(summary, test_type, output_dir, chipname)
             if passes_qc == -1:
                 log.error(
                     bcolors.ERROR
                     + f" QC analysis for {key} was NOT successful. Please fix and re-run. Continuing to next chip.."
                     + bcolors.ENDC
                 )
                 continue
@@ -435,20 +456,23 @@
                 log.info(
                     f" Chip {key} passes QC? "
                     + bcolors.BADRED
                     + f"{passes_qc}"
                     + bcolors.ENDC
                 )
             log.info("")
+            log.removeHandler(chiplog)
+            chiplog.close()
+
             outputDF.set_pass_flag(passes_qc)
             if submit:
                 submit_results(
                     outputDF.to_dict(True),
                     time_start,
-                    site,
+                    institution,
                     output_dir.joinpath("submit.txt"),
                     layer,
                 )
 
             if permodule:
                 alloutput += [outputDF.to_dict(True)]
                 timestamps += [meas_timestamp]
```

### Comparing `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py` & `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 )
 
 from module_qc_analysis_tools import __version__
 from module_qc_analysis_tools.cli.globals import CONTEXT_SETTINGS, OPTIONS, LogLevel
 from module_qc_analysis_tools.utils.analysis import (
     check_layer,
     perform_qc_analysis,
+    print_result_summary,
     submit_results,
 )
 from module_qc_analysis_tools.utils.misc import (
     DataExtractor,
     JsonChecker,
     bcolors,
     get_inputs,
@@ -41,38 +42,34 @@
     qc_criteria_path: Path = OPTIONS["qc_criteria"],
     input_layer: str = OPTIONS["layer"],
     permodule: bool = OPTIONS["permodule"],
     submit: bool = OPTIONS["submit"],
     site: str = OPTIONS["site"],
     verbosity: LogLevel = OPTIONS["verbosity"],
 ):
-    log = logging.getLogger(__name__)
+    test_type = Path(__file__).stem
+
+    time_start = datetime.now().strftime("%Y-%m-%d_%H%M%S")
+    output_dir = base_output_dir.joinpath(test_type).joinpath(f"{time_start}")
+    output_dir.mkdir(parents=True, exist_ok=False)
+
+    log = logging.getLogger("analysis")
     log.setLevel(verbosity.value)
+    log.addHandler(logging.FileHandler(f"{output_dir}/output.log"))
 
-    if submit and site == "":
-        log.error(
-            bcolors.ERROR
-            + "You have supplied the --submit option without specifying --site (testing site). Please specify your testing site if you would like to submit these results"
-            + bcolors.ENDC
-        )
-        return
+    # Turn off matplotlib DEBUG messages
+    plt.set_loglevel(level="warning")
 
     log.info("")
     log.info(" ===================================================")
     log.info(" \tPerforming Injection Capacitance analysis")
     log.info(" ===================================================")
     log.info("")
 
-    test_type = Path(__file__).stem
-
-    time_start = datetime.now().strftime("%Y-%m-%d_%H%M%S")
-    output_dir = base_output_dir.joinpath(test_type).joinpath(f"{time_start}")
-    output_dir.mkdir(parents=True, exist_ok=False)
-
-    allinputs = get_inputs(input_meas, test_type)
+    allinputs = get_inputs(input_meas)
     qc_config = get_qc_config(qc_criteria_path, test_type)
 
     alloutput = []
     timestamps = []
     for filename in allinputs:
         log.info("")
         log.info(f" Loading {filename}")
@@ -128,14 +125,35 @@
                 log.warning(
                     bcolors.WARNING
                     + "Chip name not found in input from {filename}, skipping."
                     + bcolors.ENDC
                 )
                 continue
 
+            institution = metadata.get("Institution")
+            if site != "" and institution != "":
+                log.warning(
+                    bcolors.WARNING
+                    + " Overwriting default institution {} with manual input {}!".format(
+                        institution, site
+                    )
+                    + bcolors.ENDC
+                )
+                institution = site
+            elif site != "":
+                institution = site
+
+            if institution == "":
+                log.error(
+                    bcolors.ERROR
+                    + "No institution found. Please specify your testing site either in the measurement data or specify with the --site option. "
+                    + bcolors.ENDC
+                )
+                return
+
             """  Calculate quanties   """
             # Vmux conversion is embedded.
             extractor = DataExtractor(inputDF, f"{test_type}")
             calculated_data = extractor.calculate()
 
             """        Plotting       """
             CapMeas = calculated_data.get("CapMeas").get("Values")
@@ -227,17 +245,20 @@
             plt.close()
 
             # Load values to dictionary for QC analysis
             results = {}
             results.update({"INJ_CAPACITANCE": avgCpix})
 
             # Perform QC analysis
-            passes_qc = perform_qc_analysis(
-                test_type, qc_config, layer, results, verbosity.value
+            chiplog = logging.FileHandler(f"{output_dir}/{chipname}.log")
+            log.addHandler(chiplog)
+            passes_qc, summary = perform_qc_analysis(
+                test_type, qc_config, layer, results
             )
+            print_result_summary(summary, test_type, output_dir, chipname)
 
             if passes_qc == -1:
                 log.error(
                     bcolors.ERROR
                     + f" QC analysis for {chipname} was NOT successful. Please fix and re-run. Continuing to next chip.."
                     + bcolors.ENDC
                 )
@@ -254,14 +275,16 @@
                 log.info(
                     f" Chip {chipname} passes QC? "
                     + bcolors.BADRED
                     + f"{passes_qc}"
                     + bcolors.ENDC
                 )
             log.info("")
+            log.removeHandler(chiplog)
+            chiplog.close()
 
             """ Information for output json file """
             tmpoutput = {}
 
             tmpoutput["INJ_CAPACITANCE"] = round(avgCpix, 3)
             tmpoutput["Metadata"] = metadata
             tmpoutput["passes_qc"] = passes_qc
@@ -281,27 +304,28 @@
                 __version__,
             )
             data.add_meta_data(
                 "MEASUREMENT_VERSION",
                 qcframe.get_properties().get(test_type + "_MEASUREMENT_VERSION"),
             )
             data.add_meta_data("QC_LAYER", layer)
+            data.add_meta_data("INSTITUTION", institution)
             data._meta_data.update(chip["Metadata"])
             chip.pop("Metadata")
             if outputDF._passed is not False:
                 outputDF.set_pass_flag(chip["passes_qc"])
             chip.pop("passes_qc")
             for result in chip:
                 data.add_parameter(result, chip[result])
             outputDF.set_results(data)
             if submit:
                 submit_results(
                     outputDF.to_dict(True),
                     time_start,
-                    site,
+                    institution,
                     output_dir.joinpath("submit.txt"),
                     layer,
                 )
             if permodule:
                 alloutput += [outputDF.to_dict(True)]
                 timestamps += [meas_timestamp]
             else:
```

### Comparing `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/IV_MEASURE.py` & `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/IV_MEASURE.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     test_type = Path(__file__).stem
 
     time_start = round(datetime.timestamp(datetime.now()))
     output_dir = base_output_dir.joinpath(test_type).joinpath(f"{time_start}")
     output_dir.mkdir(parents=True, exist_ok=False)
 
-    allinputs = get_inputs(input_meas, test_type)
+    allinputs = get_inputs(input_meas)
     # qc_config = get_qc_config(qc_criteria_path, test_type)
 
     # alloutput = []
     # timestamps = []
     for filename in sorted(allinputs):
         log.info("")
         log.info(f" Loading {filename}")
```

### Comparing `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py` & `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     test_type = Path(__file__).stem
 
     time_start = round(datetime.timestamp(datetime.now()))
     output_dir = base_output_dir.joinpath(test_type).joinpath(f"{time_start}")
     output_dir.mkdir(parents=True, exist_ok=False)
 
-    allinputs = get_inputs(input_meas, test_type)
+    allinputs = get_inputs(input_meas)
     # qc_config = get_qc_config(qc_criteria_path, test_type)
 
     # alloutput = []
     # timestamps = []
     for filename in sorted(allinputs):
         log.info("")
         log.info(f" Loading {filename}")
```

### Comparing `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py` & `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,18 @@
 from module_qc_analysis_tools import __version__
 from module_qc_analysis_tools.cli.globals import (
     CONTEXT_SETTINGS,
     OPTIONS,
     LogLevel,
 )
 from module_qc_analysis_tools.utils.analysis import (
+    check_layer,
     get_layer,
     perform_qc_analysis,
+    print_result_summary,
 )
 from module_qc_analysis_tools.utils.classification import (
     check_input_yarr_config,
     check_input_yarr_data,
     classify_pixels,
     count_pixels,
     format_pixel_input,
@@ -36,46 +38,63 @@
 from module_qc_analysis_tools.utils.misc import (
     bcolors,
     get_qc_config,
 )
 
 app = typer.Typer(context_settings=CONTEXT_SETTINGS)
 
-log = logging.getLogger()
+log = logging.getLogger("analysis")
 
 
 @app.command()
 def main(
     input_yarr: Path = OPTIONS["input_yarr_config"],
     qc_criteria_path: Path = OPTIONS["qc_criteria"],
     pixel_classification_path: Path = OPTIONS["pixel_classification"],
     base_output_dir: Path = OPTIONS["output_dir"],
     permodule: bool = OPTIONS["permodule"],
+    input_layer: str = OPTIONS["layer"],
     verbosity: LogLevel = OPTIONS["verbosity"],
 ):
-    log.setLevel(verbosity.value)
-
     test_type = Path(__file__).stem
     qc_config = get_qc_config(qc_criteria_path, test_type)
 
+    time_start = datetime.now().strftime("%Y-%m-%d_%H%M%S")
+    output_dir = base_output_dir.joinpath(test_type).joinpath(f"{time_start}")
+    output_dir.mkdir(parents=True, exist_ok=False)
+
+    log.setLevel(verbosity.value)
+    log.addHandler(logging.FileHandler(f"{output_dir}/output.log"))
+
     log.info("")
     log.info(" ====================================================")
     log.info(" \tPerforming minimum health test analysis")
     log.info(" ====================================================")
     log.info("")
 
-    time_start = datetime.now().strftime("%Y-%m-%d_%H%M%S")
-    output_dir = base_output_dir.joinpath(test_type).joinpath(f"{time_start}")
-    output_dir.mkdir(parents=True, exist_ok=False)
-
     input_data = read_json(input_yarr)
     check_input_yarr_config(input_data, path=input_yarr)
     datadir = input_data["datadir"]
     module_sn = input_data["module"]["serialNumber"]
-    layer = get_layer_from_sn(module_sn)
+
+    if input_layer == "Unknown":
+        try:
+            layer = get_layer_from_sn(module_sn)
+        except Exception:
+            log.error(bcolors.WARNING + " Something went wrong." + bcolors.ENDC)
+    else:
+        log.warning(
+            bcolors.WARNING
+            + " Overwriting default layer config {} with manual input {}!".format(
+                get_layer_from_sn(module_sn), input_layer
+            )
+            + bcolors.ENDC
+        )
+        layer = input_layer
+    check_layer(layer)
 
     pixel_classification = read_json(pixel_classification_path)
 
     if not pixel_classification.get(test_type):
         log.error(
             bcolors.BADRED
             + f"Pixel failure selection for {test_type} not found in {pixel_classification_path}! Please check. "
@@ -170,20 +189,22 @@
                 )
                 if np.isscalar(pix_fail):
                     continue
 
         if skip_chip:
             continue
 
+        chiplog = logging.FileHandler(f"{output_dir}/{chipName}.log")
+        log.addHandler(chiplog)
         test_names = pixel_classification.get(test_type).keys()
         failure_summary = count_pixels(pix_fail, record_fail, test_names)
         for fname, nfail in failure_summary.items():
             data.add_parameter("MIN_HEALTH_" + fname, round(nfail.get("dependent"), 3))
 
-        print_pixel_classification(failure_summary)
+        print_pixel_classification(failure_summary, test_type, output_dir, chipName)
 
         try:
             results.update(
                 {
                     "BAD_ANALOG_INTEGRATED": failure_summary.get("BAD_ANALOG").get(
                         "integrated"
                     )
@@ -221,17 +242,16 @@
         except Exception:
             log.warning(
                 bcolors.WARNING
                 + "Problem getting HIGH_ENC results from failure summary"
                 + bcolors.ENDC
             )
 
-        passes_qc = perform_qc_analysis(
-            test_type, qc_config, layer, results, verbosity.value
-        )
+        passes_qc, summary = perform_qc_analysis(test_type, qc_config, layer, results)
+        print_result_summary(summary, test_type, output_dir, chipName)
         if passes_qc == -1:
             log.error(
                 bcolors.ERROR
                 + f" QC analysis for {chipName} was NOT successful. Please fix and re-run. Continuing to next chip.."
                 + bcolors.ENDC
             )
             continue
@@ -247,14 +267,16 @@
             log.info(
                 f" Chip {chipName} passes QC? "
                 + bcolors.BADRED
                 + f"{passes_qc}"
                 + bcolors.ENDC
             )
         log.info("")
+        log.removeHandler(chiplog)
+        chiplog.close()
 
         outputDF.set_results(data)
         outputDF.set_pass_flag(passes_qc)
 
         if permodule:
             alloutput += [outputDF.to_dict(True)]
         else:
```

### Comparing `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py` & `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/TUNING.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,103 +17,114 @@
 from module_qc_analysis_tools import __version__
 from module_qc_analysis_tools.cli.globals import (
     CONTEXT_SETTINGS,
     OPTIONS,
     LogLevel,
 )
 from module_qc_analysis_tools.utils.analysis import (
+    check_layer,
     get_layer,
     perform_qc_analysis,
+    print_result_summary,
 )
 from module_qc_analysis_tools.utils.classification import (
     check_input_yarr_config,
     check_input_yarr_data,
     classify_pixels,
     count_pixels,
+    format_config_input,
     format_pixel_input,
-    print_pixel_classification,
     read_json,
 )
 from module_qc_analysis_tools.utils.misc import (
     bcolors,
     get_qc_config,
 )
 
 app = typer.Typer(context_settings=CONTEXT_SETTINGS)
 
-log = logging.getLogger()
+log = logging.getLogger("analysis")
 
 
 @app.command()
 def main(
     input_yarr: Path = OPTIONS["input_yarr_config"],
     qc_criteria_path: Path = OPTIONS["qc_criteria"],
     pixel_classification_path: Path = OPTIONS["pixel_classification"],
     base_output_dir: Path = OPTIONS["output_dir"],
     permodule: bool = OPTIONS["permodule"],
+    input_layer: str = OPTIONS["layer"],
     verbosity: LogLevel = OPTIONS["verbosity"],
 ):
-    log.setLevel(verbosity.value)
-
     test_type = Path(__file__).stem
-    qc_config = get_qc_config(qc_criteria_path, test_type)
+    qc_config_untuned = get_qc_config(qc_criteria_path, test_type + "_UNTUNED")
+    qc_config_tuned = get_qc_config(qc_criteria_path, test_type + "_TUNED")
+
+    time_start = datetime.now().strftime("%Y-%m-%d_%H%M%S")
+    output_dir = base_output_dir.joinpath(test_type).joinpath(f"{time_start}")
+    output_dir.mkdir(parents=True, exist_ok=False)
+
+    log.setLevel(verbosity.value)
+    log.addHandler(logging.FileHandler(f"{output_dir}/output.log"))
 
     log.info("")
     log.info(" ====================================================")
-    log.info(" \tPerforming minimum health test analysis")
+    log.info(" \tPerforming tuning analysis")
     log.info(" ====================================================")
     log.info("")
 
-    time_start = datetime.now().strftime("%Y-%m-%d_%H%M%S")
-    output_dir = base_output_dir.joinpath(test_type).joinpath(f"{time_start}")
-    output_dir.mkdir(parents=True, exist_ok=False)
-
     input_data = read_json(input_yarr)
     check_input_yarr_config(input_data, path=input_yarr)
     datadir = input_data["datadir"]
     module_sn = input_data["module"]["serialNumber"]
     layer = get_layer_from_sn(module_sn)
 
+    if input_layer == "Unknown":
+        try:
+            layer = get_layer_from_sn(module_sn)
+        except Exception:
+            log.error(bcolors.WARNING + " Something went wrong." + bcolors.ENDC)
+    else:
+        log.warning(
+            bcolors.WARNING
+            + " Overwriting default layer config {} with manual input {}!".format(
+                get_layer_from_sn(module_sn), input_layer
+            )
+            + bcolors.ENDC
+        )
+        layer = input_layer
+    check_layer(layer)
+
     pixel_classification = read_json(pixel_classification_path)
     if not pixel_classification.get(test_type):
         log.error(
             bcolors.BADRED
             + f"Pixel failure selection for {test_type} not found in {pixel_classification_path}! Please check. "
             + bcolors.ENDC
         )
         raise RuntimeError()
 
     alloutput = []
     for c in input_data["chip"]:
         chipSN = c["serialNumber"]
         chipName = convert_serial_to_name(chipSN)
         filepaths = c["filepaths"]
-        results = {}
+        results_tuned = {}
+        results_untuned = {}
         skip_chip = False
 
         # Initialize array to track pixel failures
-        pix_fail = np.zeros(153600, dtype=np.uint16)
+        pix_fail_tuned = np.zeros(153600, dtype=np.uint16)
+        pix_fail_untuned = np.zeros(153600, dtype=np.uint16)
 
         # Initialize int to track which classifications have been checked
-        record_fail = 0
+        record_fail_tuned = 0
+        record_fail_untuned = 0
 
-        log.debug(
-            f"Performing minimum health test analysis on chip {c['serialNumber']}"
-        )
-
-        """ Prepare output json file """
-        outputDF = outputDataFrame()
-        outputDF.set_test_type(test_type)
-        outputDF.set_serial_num(chipSN)
-        data = qcDataFrame()
-        data.add_property(
-            "ANALYSIS_VERSION",
-            __version__,
-        )
-        data.add_meta_data("QC_LAYER", layer)
+        log.debug(f"Performing tuning test analysis on chip {c['serialNumber']}")
 
         # Loop through pixel failure tests from config file
         for test_name, params in pixel_classification.get(test_type).items():
             log.debug(f"Performing {test_name}")
 
             test_input = params.get("input")
             test_method = params.get("method")
@@ -132,66 +143,123 @@
                     continue
                 test_params = layer_bounds
 
             # Check if we have data for that test
             if test_input not in filepaths.keys():
                 log.info(
                     bcolors.WARNING
-                    + f"YARR data for {test_name} not found in {input_yarr} ({test_input}). PIXEL_FAILURE_ANALYSIS cannot be performed on this chip. Exiting."
+                    + f"YARR data for {test_name} not found in {input_yarr} ({test_input}). TUNING cannot be performed on this chip. Exiting."
                     + bcolors.ENDC
                 )
                 skip_chip = True
                 break
 
             # Read input YARR scan
             input_data_path = datadir + "/" + filepaths[test_input]
             input_data = read_json(Path(input_data_path))
-            check_input_yarr_data(input_data, path=input_data_path)
 
-            pix_data, pix_index = format_pixel_input(input_data.get("Data"))
+            if "TDAC" in test_name:
+                check_input_yarr_data(input_data, input_data_path, config=True)
+                pix_data, pix_index = format_config_input(
+                    input_data.get("RD53B").get("PixelConfig")
+                )
+            else:
+                check_input_yarr_data(input_data, input_data_path, config=False)
+                pix_data, pix_index = format_pixel_input(input_data.get("Data"))
 
             # Calculate relevant quantities
             if test_method == "mean":
                 if "TDAC" not in test_name:
                     pix_data = pix_data[pix_data > 0]
-                results.update({"PIXEL_FAILURE_" + test_name: np.mean(pix_data)})
+                if "UNTUNED" in test_name:
+                    results_untuned.update({test_name: np.mean(pix_data)})
+                else:
+                    results_tuned.update({test_name: np.mean(pix_data)})
+
             elif test_method == "rms":
                 if "TDAC" not in test_name:
                     pix_data = pix_data[pix_data > 0]
-                results.update({"PIXEL_FAILURE_" + test_name: np.std(pix_data)})
+                if "UNTUNED" in test_name:
+                    results_untuned.update({test_name: np.std(pix_data)})
+                else:
+                    results_tuned.update({test_name: np.std(pix_data)})
+
+            elif test_method == "percentile":
+                if "TDAC" not in test_name:
+                    pix_data = pix_data[pix_data > 0]
+                bound = (100 - test_params[0]) / 2.0
+                lower, upper = np.percentile(pix_data, [bound, 100 - bound])
+                if "UNTUNED" in test_name:
+                    results_untuned.update({test_name + "_LOW": lower})
+                    results_untuned.update({test_name + "_HIGH": upper})
+                else:
+                    results_tuned.update({test_name + "_LOW": lower})
+                    results_tuned.update({test_name + "_HIGH": upper})
             else:
                 log.debug(f"Classifying pixels failing {test_name}")
-                pix_fail, record_fail = classify_pixels(
-                    pix_data, pix_fail, record_fail, test_name, test_method, test_params
-                )
-                if np.isscalar(pix_fail):
-                    continue
+                if test_name == "TUNED_THRESHOLD_FAILED_FITS":
+                    pix_fail_tuned, record_fail_tuned = classify_pixels(
+                        pix_data,
+                        pix_fail_tuned,
+                        record_fail_tuned,
+                        "THRESHOLD_FAILED_FITS",
+                        test_method,
+                        test_params,
+                    )
+                    if np.isscalar(pix_fail_tuned):
+                        continue
+                elif test_name == "UNTUNED_THRESHOLD_FAILED_FITS":
+                    pix_fail_untuned, record_fail_untuned = classify_pixels(
+                        pix_data,
+                        pix_fail_untuned,
+                        record_fail_untuned,
+                        "THRESHOLD_FAILED_FITS",
+                        test_method,
+                        test_params,
+                    )
+                    if np.isscalar(pix_fail_untuned):
+                        continue
+                else:
+                    log.error("TUNING not equipped to test for {test_name}. Please fix")
+                    raise RuntimeError()
 
         if skip_chip:
             continue
 
-        test_names = pixel_classification.get(test_type).keys()
-        failure_summary = count_pixels(pix_fail, record_fail, test_names)
-        for fname, nfail in failure_summary.items():
-            data.add_parameter(
-                "PIXEL_FAILURE_" + fname, round(nfail.get("dependent"), 3)
-            )
+        chiplog = logging.FileHandler(f"{output_dir}/{chipName}.log")
+        log.addHandler(chiplog)
+        failure_summary_tuned = count_pixels(
+            pix_fail_tuned, record_fail_tuned, ["THRESHOLD_FAILED_FITS"]
+        )
+        results_tuned.update(
+            {
+                "TUNED_THRESHOLD_FAILED_FITS": failure_summary_tuned.get(
+                    "THRESHOLD_FAILED_FITS"
+                ).get("independent")
+            }
+        )
 
-        print_pixel_classification(failure_summary)
-        total_electrically_failing = list(failure_summary.values())[-1].get(
-            "integrated"
+        failure_summary_untuned = count_pixels(
+            pix_fail_untuned, record_fail_untuned, ["THRESHOLD_FAILED_FITS"]
         )
-        results.update({"ELECTRICALLY_FAILED": total_electrically_failing})
-        data.add_parameter(
-            "PIXEL_FAILURE_ELECTRICALLY_FAILED", total_electrically_failing
+        results_untuned.update(
+            {
+                "UNTUNED_THRESHOLD_FAILED_FITS": failure_summary_untuned.get(
+                    "THRESHOLD_FAILED_FITS"
+                ).get("independent")
+            }
         )
 
-        passes_qc = perform_qc_analysis(
-            test_type, qc_config, layer, results, verbosity.value
+        passes_qc, summary = perform_qc_analysis(
+            test_type, qc_config_untuned, layer, results_untuned
+        )
+        passes_qc, summary = perform_qc_analysis(
+            test_type, qc_config_tuned, layer, results_tuned
         )
+        print_result_summary(summary, test_type, output_dir, chipName)
         if passes_qc == -1:
             log.error(
                 bcolors.ERROR
                 + f" QC analysis for {chipName} was NOT successful. Please fix and re-run. Continuing to next chip.."
                 + bcolors.ENDC
             )
             continue
@@ -207,14 +275,32 @@
             log.info(
                 f" Chip {chipName} passes QC? "
                 + bcolors.BADRED
                 + f"{passes_qc}"
                 + bcolors.ENDC
             )
         log.info("")
+        log.removeHandler(chiplog)
+        chiplog.close()
+
+        """ Output a json file """
+        outputDF = outputDataFrame()
+        outputDF.set_test_type(test_type)
+        outputDF.set_serial_num(chipSN)
+        data = qcDataFrame()
+        data.add_property(
+            "ANALYSIS_VERSION",
+            __version__,
+        )
+        data.add_meta_data("QC_LAYER", layer)
+        # Add all parameters used in QC selection
+        for key, value in results_untuned.items():
+            data.add_parameter("TUNING_" + key, round(value, 3))
+        for key, value in results_tuned.items():
+            data.add_parameter("TUNING_" + key, round(value, 3))
 
         outputDF.set_results(data)
         outputDF.set_pass_flag(passes_qc)
 
         if permodule:
             alloutput += [outputDF.to_dict(True)]
         else:
```

### Comparing `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/SLDO.py` & `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/SLDO.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     check_layer,
     get_n_chips,
     get_nominal_current,
     get_nominal_RextA,
     get_nominal_RextD,
     get_nominal_Voffs,
     perform_qc_analysis,
+    print_result_summary,
     submit_results,
 )
 from module_qc_analysis_tools.utils.misc import (
     DataExtractor,
     JsonChecker,
     bcolors,
     get_inputs,
@@ -51,45 +52,41 @@
     input_meas: Path = OPTIONS["input_meas"],
     base_output_dir: Path = OPTIONS["output_dir"],
     qc_criteria_path: Path = OPTIONS["qc_criteria"],
     input_layer: str = OPTIONS["layer"],
     permodule: bool = OPTIONS["permodule"],
     submit: bool = OPTIONS["submit"],
     site: str = OPTIONS["site"],
-    nChips: int = OPTIONS["nchips"],
+    nChipsInput: int = OPTIONS["nchips"],
     fit_method: FitMethod = OPTIONS["fit_method"],
     verbosity: LogLevel = OPTIONS["verbosity"],
     lp_enable: bool = OPTIONS["lp_enable"],
 ):
-    log = logging.getLogger(__name__)
+    test_type = Path(__file__).stem
+
+    allinputs = get_inputs(input_meas)
+    qc_config = get_qc_config(qc_criteria_path, test_type)
+
+    time_start = datetime.now().strftime("%Y-%m-%d_%H%M%S")
+    output_dir = base_output_dir.joinpath(test_type).joinpath(f"{time_start}")
+    output_dir.mkdir(parents=True, exist_ok=False)
+
+    log = logging.getLogger("analysis")
     log.setLevel(verbosity.value)
+    log.addHandler(logging.FileHandler(f"{output_dir}/output.log"))
 
-    if submit and site == "":
-        log.error(
-            bcolors.ERROR
-            + "You have supplied the --submit option without specifying --site (testing site). Please specify your testing site if you would like to submit these results"
-            + bcolors.ENDC
-        )
-        return
+    # Turn off matplotlib DEBUG messages
+    plt.set_loglevel(level="warning")
 
     log.info("")
     log.info(" =======================================")
     log.info(" \tPerforming SLDO analysis")
     log.info(" =======================================")
     log.info("")
 
-    test_type = Path(__file__).stem
-
-    allinputs = get_inputs(input_meas, test_type)
-    qc_config = get_qc_config(qc_criteria_path, test_type)
-
-    time_start = datetime.now().strftime("%Y-%m-%d_%H%M%S")
-    output_dir = base_output_dir.joinpath(test_type).joinpath(f"{time_start}")
-    output_dir.mkdir(parents=True, exist_ok=False)
-
     alloutput = []
     timestamps = []
     for filename in sorted(allinputs):
         log.info("")
         log.info(f" Loading {filename}")
         meas_timestamp = get_time_stamp(filename)
         inputDFs = load_json(filename)
@@ -134,24 +131,25 @@
                 )
                 layer = input_layer
             check_layer(layer)
 
             # SLDO parameters
             RextA = get_nominal_RextA(layer)
             RextD = get_nominal_RextD(layer)
-            if nChips == 0:
+            if nChipsInput == 0:
                 nChips = get_n_chips(layer)
-            else:
+            elif nChips != get_n_chips(layer):
                 log.warning(
                     bcolors.WARNING
                     + " Overwriting default number of chips ({}) with manual input ({})!".format(
-                        get_n_chips(layer), nChips
+                        get_n_chips(layer), nChipsInput
                     )
                     + bcolors.ENDC
                 )
+                nChips = nChipsInput
 
             try:
                 kShuntA = (
                     metadata.get("ChipConfigs")
                     .get("RD53B")
                     .get("Parameter")
                     .get("KShuntA")
@@ -188,14 +186,35 @@
                 log.error(
                     bcolors.ERROR
                     + f" Chip name not found in input from {filename}, skipping."
                     + bcolors.ENDC
                 )
                 continue
 
+            institution = metadata.get("Institution")
+            if site != "" and institution != "":
+                log.warning(
+                    bcolors.WARNING
+                    + " Overwriting default institution {} with manual input {}!".format(
+                        institution, site
+                    )
+                    + bcolors.ENDC
+                )
+                institution = site
+            elif site != "":
+                institution = site
+
+            if institution == "":
+                log.error(
+                    bcolors.ERROR
+                    + "No institution found. Please specify your testing site either in the measurement data or specify with the --site option. "
+                    + bcolors.ENDC
+                )
+                return
+
             R_eff = 1.0 / ((kShuntA / RextA) + (kShuntD / RextD)) / nChips
 
             Vofs = get_nominal_Voffs(layer, lp_enable)
 
             p = np.poly1d([R_eff, Vofs])
             p1 = np.poly1d([R_eff, 0])
 
@@ -574,17 +593,20 @@
             results.update({"SLDO_IINA": SLDO_IINA})
             results.update({"SLDO_IIND": SLDO_IIND})
             results.update({"SLDO_IREF": SLDO_IREF})
             results.update({"SLDO_ISHUNTA": SLDO_ISHUNTA})
             results.update({"SLDO_ISHUNTD": SLDO_ISHUNTD})
 
             # Perform QC analysis
-            passes_qc = perform_qc_analysis(
-                test_type, qc_config, layer, results, verbosity.value
+            chiplog = logging.FileHandler(f"{output_dir}/{chipname}.log")
+            log.addHandler(chiplog)
+            passes_qc, summary = perform_qc_analysis(
+                test_type, qc_config, layer, results
             )
+            print_result_summary(summary, test_type, output_dir, chipname)
             if passes_qc == -1:
                 log.error(
                     bcolors.ERROR
                     + f" QC analysis for {chipname} was NOT successful. Please fix and re-run. Continuing to next chip.."
                     + bcolors.ENDC
                 )
                 continue
@@ -600,14 +622,16 @@
                 log.info(
                     f" Chip {chipname} passes QC? "
                     + bcolors.BADRED
                     + f"{passes_qc}"
                     + bcolors.ENDC
                 )
             log.info("")
+            log.removeHandler(chiplog)
+            chiplog.close()
 
             """ Output a json file """
             outputDF = outputDataFrame()
             outputDF.set_test_type(test_type)
             data = qcDataFrame()
             data._meta_data.update(metadata)
             data.add_property(
@@ -615,14 +639,15 @@
                 __version__,
             )
             data.add_meta_data(
                 "MEASUREMENT_VERSION",
                 qcframe.get_properties().get(test_type + "_MEASUREMENT_VERSION"),
             )
             data.add_meta_data("QC_LAYER", layer)
+            data.add_meta_data("INSTITUTION", institution)
 
             # Add all values used in QC selection to output file
             for key, value in results.items():
                 data.add_parameter(key, round(value, 4))
 
             # Calculate additional values for output file only
             analog_overhead = calculated_data["IshuntA"]["Values"][idx] / (
@@ -643,15 +668,15 @@
 
             outputDF.set_results(data)
             outputDF.set_pass_flag(passes_qc)
             if submit:
                 submit_results(
                     outputDF.to_dict(True),
                     time_start,
-                    site,
+                    institution,
                     output_dir.joinpath("submit.txt"),
                     layer,
                 )
             if permodule:
                 alloutput += [outputDF.to_dict(True)]
                 timestamps += [meas_timestamp]
             else:
```

### Comparing `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py` & `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     OPTIONS,
     FitMethod,
     LogLevel,
 )
 from module_qc_analysis_tools.utils.analysis import (
     check_layer,
     perform_qc_analysis,
+    print_result_summary,
     submit_results,
 )
 from module_qc_analysis_tools.utils.misc import (
     DataExtractor,
     JsonChecker,
     bcolors,
     get_inputs,
@@ -49,38 +50,34 @@
     input_layer: str = OPTIONS["layer"],
     permodule: bool = OPTIONS["permodule"],
     submit: bool = OPTIONS["submit"],
     site: str = OPTIONS["site"],
     fit_method: FitMethod = OPTIONS["fit_method"],
     verbosity: LogLevel = OPTIONS["verbosity"],
 ):
-    log = logging.getLogger(__name__)
+    test_type = Path(__file__).stem
+
+    time_start = datetime.now().strftime("%Y-%m-%d_%H%M%S")
+    output_dir = base_output_dir.joinpath(test_type).joinpath(f"{time_start}")
+    output_dir.mkdir(parents=True, exist_ok=False)
+
+    log = logging.getLogger("analysis")
     log.setLevel(verbosity.value)
+    log.addHandler(logging.FileHandler(f"{output_dir}/output.log"))
 
-    if submit and site == "":
-        log.error(
-            bcolors.ERROR
-            + "You have supplied the --submit option without specifying --site (testing site). Please specify your testing site if you would like to submit these results"
-            + bcolors.ENDC
-        )
-        return
+    # Turn off matplotlib DEBUG messages
+    plt.set_loglevel(level="warning")
 
     log.info("")
     log.info(" ==========================================")
     log.info(" \tPerforming VCAL calibration analysis")
     log.info(" ==========================================")
     log.info("")
 
-    test_type = Path(__file__).stem
-
-    time_start = datetime.now().strftime("%Y-%m-%d_%H%M%S")
-    output_dir = base_output_dir.joinpath(test_type).joinpath(f"{time_start}")
-    output_dir.mkdir(parents=True, exist_ok=False)
-
-    allinputs = get_inputs(input_meas, test_type)
+    allinputs = get_inputs(input_meas)
     qc_config = get_qc_config(qc_criteria_path, test_type)
 
     alloutput = []
     timestamps = []
     for filename in allinputs:
         log.info("")
         log.info(f" Loading {filename}")
@@ -150,14 +147,35 @@
                 log.warning(
                     bcolors.WARNING
                     + "Chip name not found in input from {filename}, skipping."
                     + bcolors.ENDC
                 )
                 continue
 
+            institution = metadata.get("Institution")
+            if site != "" and institution != "":
+                log.warning(
+                    bcolors.WARNING
+                    + " Overwriting default institution {} with manual input {}!".format(
+                        institution, site
+                    )
+                    + bcolors.ENDC
+                )
+                institution = site
+            elif site != "":
+                institution = site
+
+            if institution == "":
+                log.error(
+                    bcolors.ERROR
+                    + "No institution found. Please specify your testing site either in the measurement data or specify with the --site option. "
+                    + bcolors.ENDC
+                )
+                return
+
             """  Calculate quanties   """
             # Vmux conversion is embedded.
             extractor = DataExtractor(inputDF, test_type)
             calculated_data = extractor.calculate()
 
             """        Plotting       """
             # task specific - for Vcal Calibration x and y needs to be determined for plotting.
@@ -250,21 +268,23 @@
                         + f" Results from VCAL_{subtest}_SLOPE test not found. Unable to perform QC analysis on VCAL_{subtest}_SLOPE_SMALL_RANGE"
                         + bcolors.ENDC
                     )
                     results.get(key).pop(f"VCAL_{subtest}_SLOPE_SMALL_RANGE")
 
                 results.get(key).pop(f"VCAL_{subtest}_OFFSET_SMALL_RANGE", "")
 
-            passes_qc = perform_qc_analysis(
+            chiplog = logging.FileHandler(f"{output_dir}/{key}.log")
+            log.addHandler(chiplog)
+            passes_qc, summary = perform_qc_analysis(
                 test_type,
                 qc_config,
                 layer,
                 results.get(key),
-                verbosity.value,
             )
+            print_result_summary(summary, test_type, output_dir, key)
             if passes_qc == -1:
                 log.error(
                     bcolors.ERROR
                     + f" QC analysis for {key} was NOT successful. Please fix and re-run. Continuing to next chip.."
                     + bcolors.ENDC
                 )
                 continue
@@ -280,37 +300,40 @@
                 log.info(
                     f" Chip {key} passes QC? "
                     + bcolors.BADRED
                     + f"{passes_qc}"
                     + bcolors.ENDC
                 )
             log.info("")
+            log.removeHandler(chiplog)
+            chiplog.close()
 
             outputDF = outputDataFrame()
             test_type = Path(__file__).stem
             outputDF.set_test_type(test_type)
             data = qcDataFrame()
             data.add_property(
                 "ANALYSIS_VERSION",
                 __version__,
             )
             data.add_meta_data("MEASUREMENT_VERSION", chip["MEASUREMENT_VERSION"])
             chip.pop("MEASUREMENT_VERSION")
             data.add_meta_data("QC_LAYER", layer)
+            data.add_meta_data("INSTITUTION", institution)
             data._meta_data.update(chip["Metadata"])
             chip.pop("Metadata")
             for param in chip:
                 data.add_parameter(param, round(chip[param], 4))
             outputDF.set_results(data)
             outputDF.set_pass_flag(passes_qc)
             if submit:
                 submit_results(
                     outputDF.to_dict(True),
                     time_start,
-                    site,
+                    institution,
                     output_dir.joinpath("submit.txt"),
                     layer,
                 )
             if permodule:
                 alloutput += [outputDF.to_dict(True)]
                 timestamps += [meas_timestamp]
             else:
```

### Comparing `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py` & `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     test_type = Path(__file__).stem
 
     time_start = round(datetime.timestamp(datetime.now()))
     output_dir = base_output_dir.joinpath(test_type).joinpath(f"{time_start}")
     output_dir.mkdir(parents=True, exist_ok=False)
 
-    allinputs = get_inputs(input_meas, test_type)
+    allinputs = get_inputs(input_meas)
     # qc_config = get_qc_config(qc_criteria_path, test_type)
 
     # alloutput = []
     # timestamps = []
     for filename in sorted(allinputs):
         log.info("")
         log.info(f" Loading {filename}")
```

### Comparing `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/globals.py` & `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/globals.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/load_yarr_scans.py` & `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/load_yarr_scans.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/main.py` & `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/overwrite_config.py` & `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/overwrite_config.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/cli/update_chip_config.py` & `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/cli/update_chip_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,24 +38,18 @@
         self.all_test_types = [
             "ADC_CALIBRATION",
             "ANALOG_READBACK",
             "VCAL_CALIBRATION",
             "INJECTION_CAPACITANCE",
         ]
         self.config_chip_name = ""
-        self.in_files = get_inputs(self.in_path, self.get_test_type())
-        self.config_files = get_inputs(self.config_path, self.get_test_type(), True)
+        self.in_files = get_inputs(self.in_path)
+        self.config_files = get_inputs(self.config_path)
         self.override = override
 
-    def get_test_type(self):
-        for test_type in self.all_test_types:
-            if test_type in str(self.in_path):
-                return test_type
-        return None
-
     def reset_stack(self):
         self.stack = []
 
     def set_ADCcalPar(self, in_file, config_file):
         # Set the calibrated ADC parameters from the analysis.
         ADC_CALIBRATION_SLOPE = float(lookup(in_file, "ADC_CALIBRATION_SLOPE"))
         ADC_CALIBRATION_OFFSET = float(lookup(in_file, "ADC_CALIBRATION_OFFSET"))
@@ -129,16 +123,18 @@
                 found_chip = False
                 with in_file.open() as jsonFile:
                     in_file_data = json.load(jsonFile)
                 for chip_data in in_file_data:
                     # Check if chip name matched
                     in_chip_serial = lookup(chip_data, "serialNumber")
                     if in_chip_serial is None:
-                        msg = f"Chip {self.config_chip_name} not found in the input files! Please check the input files."
-                        raise KeyError(msg)
+                        log.warning(
+                            f"Chip {self.config_chip_name} not found in the input files! Please check the input files."
+                        )
+                        continue
                     if in_chip_serial != config_chip_serial:
                         log.debug(
                             f"Chip {self.config_chip_name} not found in config. Checking the next chip."
                         )
                     else:
                         found_chip = True
                         in_chip_passqc = lookup(chip_data, "passed")
@@ -152,38 +148,42 @@
                                 )
                             else:
                                 log.warning(
                                     "Will not update parameters. Re-run with --override if you would like to update the chip configuration even if the chip failed QC"
                                 )
                                 continue
 
-                        test_type = self.get_test_type()
+                        test_type = lookup(chip_data, "testType")
                         if test_type == "ADC_CALIBRATION":
                             self.set_ADCcalPar(chip_data, config_file)
                         elif test_type == "ANALOG_READBACK":
                             self.set_trim(chip_data, config_file)
                         elif test_type == "VCAL_CALIBRATION":
                             self.set_VcalPar(chip_data, config_file)
                         elif test_type == "INJECTION_CAPACITANCE":
                             self.set_InjCap(chip_data, config_file)
                         else:
-                            msg = f"No test type found in the input directory {self.input_path}! Please check the input path."
-                            raise KeyError(msg)
+                            log.warning(
+                                f"No test type {test_type} found in the input directory {self.in_path}. Skipping."
+                            )
+                            continue
                         break
                 if found_chip:
                     break
             with config_file.open() as jsonFile:
                 config_file_data = json.load(jsonFile)
 
             out_file = self.in_path.joinpath(f"{config_file.name}.after")
             with out_file.open("w") as fp:
                 json.dump(config_file_data, fp, indent=4)
             if not found_chip:
-                msg = f"Chip {self.config_chip_name} with serial number {config_chip_serial} not found! Please check the input files."
-                raise KeyError(msg)
+                log.warning(
+                    f"Chip {self.config_chip_name} with serial number {config_chip_serial} not found! The corresponding config will not be updated."
+                )
+                continue
 
 
 app = typer.Typer(context_settings=CONTEXT_SETTINGS)
 
 
 @app.command()
 def main(
```

### Comparing `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/data/analysis_cuts.json` & `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/data/analysis_cuts.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7272727272727273%*

 * *Differences: {"'TUNING_TUNED'": "OrderedDict([('TUNED_THRESHOLD_MEAN', OrderedDict([('LZero', [900, 1100]), "*

 * *                   "('LOne', [1350, 1650]), ('LTwo', [1350, 1650])])), ('TUNED_THRESHOLD_SIGMA', "*

 * *                   "[0, 50]), ('TUNED_TDAC_MEAN', [-1, 1]), ('TUNED_TDAC_SIGMA', [8.5, 12.5]), "*

 * *                   "('TUNED_TOT_MEAN', [6, 8]), ('TUNED_TOT_SIGMA', [0, 1])])",*

 * * "'TUNING_UNTUNED'": "OrderedDict([('UNTUNED_THRESHOLD_MEAN', [1700, 2700]), "*

 * *                     "('UNTUNED_THRESHOLD_FAILED_FITS', [0,  […]*

```diff
@@ -308,15 +308,15 @@
             ],
             "LZero": [
                 1.09,
                 1.11
             ]
         }
     },
-    "TUNING": {
+    "TUNING_TUNED": {
         "TUNED_TDAC_MEAN": [
             -1,
             1
         ],
         "TUNED_TDAC_SIGMA": [
             8.5,
             12.5
@@ -342,15 +342,17 @@
         "TUNED_TOT_MEAN": [
             6,
             8
         ],
         "TUNED_TOT_SIGMA": [
             0,
             1
-        ],
+        ]
+    },
+    "TUNING_UNTUNED": {
         "UNTUNED_THRESHOLD_FAILED_FITS": [
             0,
             1536
         ],
         "UNTUNED_THRESHOLD_MEAN": [
             1700,
             2700
```

### Comparing `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/data/pixel_classification.json` & `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/data/pixel_classification.json`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/data/schema/info_schema.json` & `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/data/schema/info_schema.json`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json` & `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/utils/analysis.py` & `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/utils/analysis.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
 import logging
 import sys
 from pathlib import Path
 
+import matplotlib.pyplot as plt
 import numpy as np
 
 from module_qc_analysis_tools.utils.misc import bcolors, getImuxMap, getVmuxMap
 
-log = logging.getLogger(__name__)
-log.setLevel("INFO")
+log = logging.getLogger("analysis")
 
 
 def format_text():
     return " {:^30}: {:^20}: {:^20}: {:^5}"
 
 
 def format_text_short():
@@ -127,19 +127,19 @@
     for key, value in mydict.items():
         if val == value:
             return key
     return -1
 
 
 def perform_qc_analysis_AR_NOMINAL_SETTINGS(
-    _test_type, qc_config, _layer_name, results, verbosity="INFO"
+    _test_type, qc_config, _layer_name, results
 ):
-    log.setLevel(verbosity)
     # QC analysis for AR_NOMINAL_SETTINGS
 
+    cell_text = np.empty(0)
     passes_qc_overall = True
     VmuxMap = getVmuxMap()
     ImuxMap = getImuxMap()
     if len(VmuxMap.keys()) + len(ImuxMap.keys()) != len(results):
         log.error(
             bcolors.ERROR
             + " Number of entries in AR_NOMINAL_SETTINGS results does not match number of entries in VmuxMap and ImuxMap - there should be one entry for every Vmux and Imux in those maps. Please fix and re-run!"
@@ -175,36 +175,54 @@
 
         if (results[index] < lower_bound) or (results[index] > upper_bound):
             passes_qc_test = False
         if passes_qc_test:
             print_output_pass(key, results[index], lower_bound, upper_bound)
         else:
             print_output_fail(key, results[index], lower_bound, upper_bound)
+
+        cell_text = np.append(
+            cell_text,
+            [
+                key,
+                round(results[index], 4),
+                f"[{lower_bound}, {upper_bound}]",
+                passes_qc_test,
+            ],
+        )
+
         passes_qc_overall = passes_qc_overall and passes_qc_test
 
-    return passes_qc_overall
+    return passes_qc_overall, cell_text
 
 
-def perform_qc_analysis_AR_VDD_Trim(
-    _test_type, qc_config, _layer_name, results, key, verbosity="INFO"
-):
-    log.setLevel(verbosity)
+def perform_qc_analysis_AR_VDD_Trim(_test_type, qc_config, _layer_name, results, key):
     # QC analysis for VDDA_VS_TRIM and VDDD_VS_TRIM
     pass_vdd_vs_trim_test = True
 
+    cell_text = np.empty(0)
     # Fist VDD value must satisfy requirements
     tmp_pass_qc = True
     lower_bound_vdd = qc_config.get("VDD_TRIM_0")[0]
     upper_bound_vdd = qc_config.get("VDD_TRIM_0")[1]
     if (results[0] < lower_bound_vdd) or (results[0] > upper_bound_vdd):
         tmp_pass_qc = False
     if tmp_pass_qc:
         print_output_pass(f"{key}_0", results[0], lower_bound_vdd, upper_bound_vdd)
     else:
         print_output_fail(f"{key}_0", results[0], lower_bound_vdd, upper_bound_vdd)
+    cell_text = np.append(
+        cell_text,
+        [
+            f"{key}_0",
+            round(results[0], 4),
+            f"[{lower_bound_vdd}, {upper_bound_vdd}]",
+            tmp_pass_qc,
+        ],
+    )
     pass_vdd_vs_trim_test = pass_vdd_vs_trim_test and tmp_pass_qc
 
     # The trim step size (change in voltage per DAC step) must satisfy requirements
     VDD_dV_list = np.diff(np.array(results))
     lower_bound_dv = qc_config.get("VDD_step_size")[0]
     upper_bound_dv = qc_config.get("VDD_step_size")[1]
     dV_fail = (VDD_dV_list < lower_bound_dv) | (VDD_dV_list > upper_bound_dv)
@@ -215,70 +233,80 @@
             print_output_pass(
                 f"{key}_{i+1}_STEP_SIZE", VDD_dV_list[i], lower_bound_dv, upper_bound_dv
             )
         else:
             print_output_fail(
                 f"{key}_{i+1}_STEP_SIZE", VDD_dV_list[i], lower_bound_dv, upper_bound_dv
             )
+        cell_text = np.append(
+            cell_text,
+            [
+                f"{key}_{i+1}_STEP_SIZE",
+                round(VDD_dV_list[i], 4),
+                f"[{lower_bound_dv}, {upper_bound_dv}]",
+                tmp_pass_qc,
+            ],
+        )
 
-    return pass_vdd_vs_trim_test
+    return pass_vdd_vs_trim_test, cell_text
 
 
-def perform_qc_analysis(test_type, qc_config, layer_name, results, verbosity="INFO"):
-    log.setLevel(verbosity)
+def perform_qc_analysis(test_type, qc_selections, layer_name, results):
     log.info("")
     log.info("Performing QC analysis!")
     log.info("")
 
-    qc_selections = qc_config[test_type]
     check_qc_selections = qc_selections.copy()
 
     check_layer(layer_name)
     layer = get_layer(layer_name)
 
     passes_qc_overall = True
     txt = format_text()
     log.info(txt.format("Parameter", "Analysis result", "QC criteria", "Pass"))
     log.info(
         "--------------------------------------------------------------------------------------"
     )
 
+    # Setup arrays for plotting
+    cell_text = np.empty(0)
+
     for key in results:
         if not qc_selections.get(key):
             log.debug(
                 bcolors.WARNING
                 + f" Selection for {key} not found in QC file! Skipping."
                 + bcolors.ENDC
             )
             print_output_neutral(key, results.get(key))
             continue
         check_qc_selections.pop(key)
 
         # Handle AR_NOMINAL_SETTINGS in completely different function, for now...
         if key == "AR_NOMINAL_SETTINGS":
-            passes_qc_test = perform_qc_analysis_AR_NOMINAL_SETTINGS(
+            passes_qc_test, new_cell_text = perform_qc_analysis_AR_NOMINAL_SETTINGS(
                 test_type,
                 qc_selections.get(key),
                 layer_name,
                 results.get(key),
-                verbosity,
             )
+            cell_text = np.append(cell_text, new_cell_text)
             passes_qc_overall = passes_qc_overall and passes_qc_test
             continue
 
         # Handle AR_VDDA_VS_TRIM and AR_VDD_VS_TRIM separately
         if ("AR_VDDA_VS_TRIM" in key) or ("AR_VDDD_VS_TRIM" in key):
-            passes_qc_test = perform_qc_analysis_AR_VDD_Trim(
+            passes_qc_test, new_cell_text = perform_qc_analysis_AR_VDD_Trim(
                 test_type,
                 qc_selections.get(key),
                 layer_name,
                 results.get(key),
                 key,
-                verbosity,
             )
+            cell_text = np.append(cell_text, new_cell_text)
             passes_qc_overall = passes_qc_overall and passes_qc_test
             continue
 
         log.debug(f" QC selections for {key}: {qc_selections.get(key)}")
         if type(qc_selections.get(key)) is list:
             if len(qc_selections.get(key)) != 2:
                 log.error(
@@ -305,27 +333,128 @@
         if (results.get(key) < lower_bound) or (results.get(key) > upper_bound):
             passes_qc_test = False
         if passes_qc_test:
             print_output_pass(key, results.get(key), lower_bound, upper_bound)
         else:
             print_output_fail(key, results.get(key), lower_bound, upper_bound)
         passes_qc_overall = passes_qc_overall and passes_qc_test
+
+        cell_text = np.append(
+            cell_text,
+            [
+                key,
+                round(results.get(key), 4),
+                f"[{lower_bound}, {upper_bound}]",
+                passes_qc_test,
+            ],
+        )
     if len(check_qc_selections) > 0:
         for key in check_qc_selections:
             log.error(
                 bcolors.ERROR
                 + f" Parameter from chip for QC selection of {key} was not passed to analysis - please fix!"
                 + bcolors.ENDC
             )
         passes_qc_overall = False
     log.info(
         "--------------------------------------------------------------------------------------"
     )
 
-    return passes_qc_overall
+    return passes_qc_overall, cell_text
+
+
+def print_result_summary(cell_text, test_type, outputdir, chipname):
+    # Turn off matplotlib DEBUG messages
+    plt.set_loglevel(level="warning")
+
+    cell_text = cell_text.reshape(-1, 4)
+    nrows, ncols = cell_text.shape
+    cellColours = np.empty(0)
+    for r in range(0, nrows):
+        if cell_text[r][3] == "True":
+            cellColours = np.append(cellColours, ["lightgreen"] * 4)
+        else:
+            cellColours = np.append(cellColours, ["lightcoral"] * 4)
+    cellColours = cellColours.reshape(-1, 4)
+    colLabels = np.array(["Parameter", "Analysis result", "QC criteria", "Pass"])
+    colWidths = [1.2, 0.4, 0.5, 0.3]
+
+    if test_type == "ANALOG_READBACK":
+        cell_text1 = cell_text[0:33, :]
+        cellColours1 = cellColours[:33, :]
+        nrows, ncols = cell_text1.shape
+        fig, ax = plt.subplots(figsize=(6.4, 1.5 + nrows * 0.5))
+        table = ax.table(
+            cellText=cell_text1,
+            colLabels=colLabels,
+            loc="upper center",
+            cellLoc="center",
+            colWidths=colWidths,
+            cellColours=cellColours1,
+        )
+        format_result_summary(fig, ax, table, chipname, test_type, outputdir, "1")
+
+        cell_text2 = cell_text[33:49, :]
+        cellColours2 = cellColours[33:49, :]
+        nrows, ncols = cell_text2.shape
+        fig, ax = plt.subplots(figsize=(6.4, 1.5 + nrows * 0.5))
+        table = ax.table(
+            cellText=cell_text2,
+            colLabels=colLabels,
+            loc="upper center",
+            cellLoc="center",
+            colWidths=colWidths,
+            cellColours=cellColours2,
+        )
+        format_result_summary(fig, ax, table, chipname, test_type, outputdir, "2")
+
+        cell_text3 = cell_text[49:, :]
+        cellColours3 = cellColours[49:, :]
+        nrows, ncols = cell_text3.shape
+        fig, ax = plt.subplots(figsize=(6.4, 1.5 + nrows * 0.5))
+        table = ax.table(
+            cellText=cell_text3,
+            colLabels=colLabels,
+            loc="upper center",
+            cellLoc="center",
+            colWidths=colWidths,
+            cellColours=cellColours3,
+        )
+        format_result_summary(fig, ax, table, chipname, test_type, outputdir, "3")
+
+    else:
+        fig, ax = plt.subplots(figsize=(6.4, 1.5 + nrows * 0.5))
+        table = ax.table(
+            cellText=cell_text,
+            colLabels=colLabels,
+            loc="upper center",
+            cellLoc="center",
+            colWidths=colWidths,
+            cellColours=cellColours,
+        )
+        format_result_summary(fig, ax, table, chipname, test_type, outputdir)
+
+
+def format_result_summary(fig, ax, table, chipname, test_type, outputdir, label=""):
+    fig.patch.set_visible(False)
+    ax.axis("off")
+    ax.axis("tight")
+    table.scale(1, 3)
+    ax.set_title(f"{test_type} for {chipname}", fontsize=15)
+    table.auto_set_font_size(False)
+    table.set_fontsize(15)
+    plt.savefig(
+        outputdir.joinpath(f"{chipname}_summary{label}.png"),
+        bbox_inches="tight",
+        dpi=100,
+        transparent=False,
+        edgecolor="white",
+    )
+    log.info("Saving " + str(outputdir.joinpath(f"{chipname}_summary{label}.png")))
+    plt.close()
 
 
 def submit_results(
     outputDF, timestamp, site="Unspecified", outputfile="submit.txt", layer="Unknown"
 ):
     results = outputDF.get("results")
```

### Comparing `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/utils/classification.py` & `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/utils/classification.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from __future__ import annotations
 
 import json
 import logging
 from pathlib import Path
 
 import jsonschema
+import matplotlib.pyplot as plt
 import numpy as np
 from jsonschema import validate
 
 from module_qc_analysis_tools import data
 from module_qc_analysis_tools.utils.misc import bcolors
 
-log = logging.getLogger(__name__)
-log.setLevel("INFO")
+log = logging.getLogger("analysis")
 
 
 def format_text_short():
     return " {:^30}: {:^20}"
 
 
 testbit_map = {
@@ -331,20 +331,49 @@
     record = set_bit(record, fail_bit)
     for f in failures:
         pix_fail[f] = set_bit(fail[f], fail_bit)
 
     return pix_fail, record
 
 
-def print_pixel_classification(failure_summary):
+def print_pixel_classification(failure_summary, test_type, outputdir, chipname):
     txt = format_text_short()
     log.info(txt.format("Classification", "Number of pixels"))
     log.info("------------------------------------------------------------------")
+    counts = []
+    binlabels = []
     for criteria, failures in failure_summary.items():
-        log.info(txt.format(criteria, round(failures.get("dependent"), 3)))
+        log.info(txt.format(criteria, failures.get("dependent")))
+        counts += [failures.get("dependent")]
+        binlabels += [criteria.replace("_", "\n")]
     log.info("------------------------------------------------------------------")
     log.info(
         txt.format(
             "TOTAL FAILING", list(failure_summary.values())[-1].get("integrated")
         )
     )
+    counts += [list(failure_summary.values())[-1].get("integrated")]
+    binlabels += ["TOTAL\nFAILING"]
     log.info("------------------------------------------------------------------")
+
+    # Turn off matplotlib DEBUG messages
+    plt.set_loglevel(level="warning")
+
+    fig, ax = plt.subplots()
+    ax.set_title(f"{chipname} ({test_type})")
+    plt.stairs(counts, range(len(counts) + 1), fill=True, color="cornflowerblue")
+    ax.set_ylim(0, max(counts) + max(counts) / 10)
+
+    # Label bins
+    plt.xticks([x + 0.5 for x in range(len(counts))], labels=binlabels, rotation=0)
+    ax.set_ylabel("Number of pixels")
+
+    # Print bin contents
+    for i in range(0, len(counts)):
+        if counts[i] > 0:
+            plt.text(i + 0.5, counts[i] + max(counts) / 60, counts[i], ha="center")
+
+    fig.tight_layout()
+    plt.subplots_adjust(bottom=0.3)
+    plt.savefig(outputdir.joinpath(f"{chipname}_classification.png"))
+    log.info("Saving " + str(outputdir.joinpath(f"{chipname}_classification.png")))
+    plt.close()
```

### Comparing `module_qc_analysis_tools-1.3.1rc3/src/module_qc_analysis_tools/utils/misc.py` & `module_qc_analysis_tools-1.3.1rc4/src/module_qc_analysis_tools/utils/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1070,27 +1070,20 @@
         p0 (float): the offset of the fitted line
     """
     A = np.vstack([x, np.ones(len(x))]).T
     p1, p0 = np.linalg.lstsq(A, y, rcond=None)[0]
     return p1, p0
 
 
-def get_inputs(input_meas: Path, test_type: str, isConfig=False) -> list[Path]:
+def get_inputs(input_meas: Path) -> list[Path]:
     # Figure out if input if single file or directory
     allinputs = []
     if input_meas.is_file():
         allinputs = [input_meas]
     elif input_meas.is_dir():
-        if (test_type not in str(input_meas)) and (not isConfig):
-            log.error(
-                bcolors.ERROR
-                + f"The input path {input_meas} does not include the test type {test_type}. Please check the input path."
-                + bcolors.ENDC
-            )
-            raise FileNotFoundError()
         allinputs = sorted(input_meas.glob("*.json"))
         if not allinputs:
             log.error(
                 bcolors.ERROR
                 + f"No input json files in `{input_meas}` are found! Please check the input path."
                 + bcolors.ENDC
             )
@@ -1130,15 +1123,15 @@
         log.error(
             bcolors.ERROR
             + f" QC criteria for {test_type} not found in {qc_criteria_path} - please fix! Exiting."
             + bcolors.ENDC
         )
         raise FileNotFoundError()
 
-    return qc_config
+    return qc_config.get(test_type)
 
 
 def lookup(input_dict, search_key, stack=None):
     # recursion to look up the desired key in a dict and record the path
     for k, v in input_dict.items():
         if k == search_key:
             return v
```

### Comparing `module_qc_analysis_tools-1.3.1rc3/tests/test_cli.py` & `module_qc_analysis_tools-1.3.1rc4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc3/.gitignore` & `module_qc_analysis_tools-1.3.1rc4/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc3/LICENSE` & `module_qc_analysis_tools-1.3.1rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc3/README.md` & `module_qc_analysis_tools-1.3.1rc4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# module-qc-analysis-tools v1.3.1rc3
+# module-qc-analysis-tools v1.3.1rc4
 
 A general python tool for running ITkPixV1.1 module QC test analysis. An
 overview of the steps in the module QC procedure is documented in the
 [Electrical specification and QC procedures for ITkPixV1.1 modules](https://gitlab.cern.ch/atlas-itk/pixel/module/itkpix-electrical-qc/)
 document and in
 [this spreadsheet](https://docs.google.com/spreadsheets/d/1qGzrCl4iD9362RwKlstZASbhphV_qTXPeBC-VSttfgE/edit#gid=989740987).
 The analysis scripts in this repository require input files with measurement
@@ -69,15 +69,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-analysis-tools==1.3.1rc3
+python -m pip install -U pip module-qc-analysis-tools==1.3.1rc4
 ```
 
 Note that users should use the latest python version (check python version via
 `python3 -V`). Python3.7 is the minimum requirement for developers. See
 [For Developer](#for-developer) section.
 
 ## Scripts
@@ -99,16 +99,15 @@
   -i INPUT_MEAS, --input-meas INPUT_MEAS
                         path to the input measurement file or directory containing input measurement files.
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         output directory
   -q QC_CRITERIA, --qc-criteria QC_CRITERIA
                         path to json file with QC selection criteria (default: $(module-qc-analysis-tools --prefix)/analysis_cuts.json)
   -l LAYER, --layer LAYER
-                        Layer of module, used for applying correct QC criteria settings. Options: L0, L1, L2
-                        (default)
+                        Layer of module, used for applying correct QC criteria settings. Default setting uses information from production database. Options: L0, L1, L2.
   --permodule           Store results in one file per module (default: one file per chip)
   -f {root,numpy}, --fit-method {root,numpy}
                         fitting method
   -v VERBOSITY, --verbosity VERBOSITY
                         Log level [options: DEBUG, INFO (default), WARNING, ERROR]
 ```
 
@@ -133,16 +132,15 @@
   -i INPUT_MEAS, --input-meas INPUT_MEAS
                         path to the input measurement file or directory containing input measurement files.
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         output directory
   -q QC_CRITERIA, --qc-criteria QC_CRITERIA
                         path to json file with QC selection criteria (default: $(module-qc-analysis-tools --prefix)/analysis_cuts.json)
   -l LAYER, --layer LAYER
-                        Layer of module, used for applying correct QC criteria settings. Options: L0, L1, L2
-                        (default)
+                        Layer of module, used for applying correct QC criteria settings. Default setting uses information from production database. Options: L0, L1, L2.
   --permodule           Store results in one file per module (default: one file per chip)
   -f {root,numpy}, --fit-method {root,numpy}
                         fitting method
   -v VERBOSITY, --verbosity VERBOSITY
                         Log level [options: DEBUG, INFO (default), WARNING, ERROR]
   --verbose             verbose mode
 
@@ -167,16 +165,15 @@
   -i INPUT_MEAS, --input-meas INPUT_MEAS
                         path to the input measurement file or directory containing input measurement files.
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         output directory
   -q QC_CRITERIA, --qc-criteria QC_CRITERIA
                         path to json file with QC selection criteria (default: $(module-qc-analysis-tools --prefix)/analysis_cuts.json)
   -l LAYER, --layer LAYER
-                        Layer of module, used for applying correct QC criteria settings. Options: L0, L1, L2
-                        (default)
+                        Layer of module, used for applying correct QC criteria settings. Default setting uses information from production database. Options: L0, L1, L2.
   --permodule           Store results in one file per module (default: one file per chip)
   -n NCHIPS, --nChips NCHIPS
                         Number of chips powered in parallel (e.g. 4 for a quad module, 3 for a triplet, 1 for an
                         SCC.)
   -f {root,numpy}, --fit-method {root,numpy}
                         fitting method
   -v VERBOSITY, --verbosity VERBOSITY
@@ -204,16 +201,15 @@
   -i INPUT_MEAS, --input-meas INPUT_MEAS
                         path to the input measurement file or directory containing input measurement files.
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         output directory
   -q QC_CRITERIA, --qc-criteria QC_CRITERIA
                         path to json file with QC selection criteria (default: $(module-qc-analysis-tools --prefix)/analysis_cuts.json)
   -l LAYER, --layer LAYER
-                        Layer of module, used for applying correct QC criteria settings. Options: L0, L1, L2
-                        (default)
+                        Layer of module, used for applying correct QC criteria settings. Default setting uses information from production database. Options: L0, L1, L2.
   --permodule           Store results in one file per module (default: one file per chip)
   -f {root,numpy}, --fit-method {root,numpy}
                         fitting method
   -v VERBOSITY, --verbosity VERBOSITY
                         Log level [options: DEBUG, INFO (default), WARNING, ERROR]
 ```
 
@@ -237,16 +233,15 @@
   -i INPUT_MEAS, --input-meas INPUT_MEAS
                         path to the input measurement file or directory containing input measurement files.
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         output directory
   -q QC_CRITERIA, --qc-criteria QC_CRITERIA
                         path to json file with QC selection criteria (default: $(module-qc-analysis-tools --prefix)/analysis_cuts.json)
   -l LAYER, --layer LAYER
-                        Layer of module, used for applying correct QC criteria settings. Options: L0, L1, L2
-                        (default)
+                        Layer of module, used for applying correct QC criteria settings. Default setting uses information from production database. Options: L0, L1, L2.
   --permodule           Store results in one file per module (default: one file per chip)
   -v VERBOSITY, --verbosity VERBOSITY
                         Log level [options: DEBUG, INFO (default), WARNING, ERROR]
 ```
 
 </details>
```

### Comparing `module_qc_analysis_tools-1.3.1rc3/pyproject.toml` & `module_qc_analysis_tools-1.3.1rc4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 description = "Module qc analysis tools"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
 dependencies = [
     "numpy",
     "matplotlib",
-    "module-qc-data-tools >= 1.0.5rc0",
+    "module-qc-data-tools >= 1.0.6",
     "typer",
     "importlib_resources>=1.4.0; python_version < '3.9'",  # for resources
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `module_qc_analysis_tools-1.3.1rc3/PKG-INFO` & `module_qc_analysis_tools-1.3.1rc4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-qc-analysis-tools
-Version: 1.3.1rc3
+Version: 1.3.1rc4
 Summary: Module qc analysis tools
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools/-/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools
 Author-email: Jay Chan <jay.chan@cern.ch>
 Maintainer-email: Giordon Stark <gstark@cern.ch>
 License: Copyright (c) 2018 The Python Packaging Authority
@@ -29,20 +29,20 @@
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: importlib-resources>=1.4.0; python_version < '3.9'
 Requires-Dist: matplotlib
-Requires-Dist: module-qc-data-tools>=1.0.5rc0
+Requires-Dist: module-qc-data-tools>=1.0.6
 Requires-Dist: numpy
 Requires-Dist: typer
 Description-Content-Type: text/markdown
 
-# module-qc-analysis-tools v1.3.1rc3
+# module-qc-analysis-tools v1.3.1rc4
 
 A general python tool for running ITkPixV1.1 module QC test analysis. An
 overview of the steps in the module QC procedure is documented in the
 [Electrical specification and QC procedures for ITkPixV1.1 modules](https://gitlab.cern.ch/atlas-itk/pixel/module/itkpix-electrical-qc/)
 document and in
 [this spreadsheet](https://docs.google.com/spreadsheets/d/1qGzrCl4iD9362RwKlstZASbhphV_qTXPeBC-VSttfgE/edit#gid=989740987).
 The analysis scripts in this repository require input files with measurement
@@ -109,15 +109,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-analysis-tools==1.3.1rc3
+python -m pip install -U pip module-qc-analysis-tools==1.3.1rc4
 ```
 
 Note that users should use the latest python version (check python version via
 `python3 -V`). Python3.7 is the minimum requirement for developers. See
 [For Developer](#for-developer) section.
 
 ## Scripts
@@ -139,16 +139,15 @@
   -i INPUT_MEAS, --input-meas INPUT_MEAS
                         path to the input measurement file or directory containing input measurement files.
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         output directory
   -q QC_CRITERIA, --qc-criteria QC_CRITERIA
                         path to json file with QC selection criteria (default: $(module-qc-analysis-tools --prefix)/analysis_cuts.json)
   -l LAYER, --layer LAYER
-                        Layer of module, used for applying correct QC criteria settings. Options: L0, L1, L2
-                        (default)
+                        Layer of module, used for applying correct QC criteria settings. Default setting uses information from production database. Options: L0, L1, L2.
   --permodule           Store results in one file per module (default: one file per chip)
   -f {root,numpy}, --fit-method {root,numpy}
                         fitting method
   -v VERBOSITY, --verbosity VERBOSITY
                         Log level [options: DEBUG, INFO (default), WARNING, ERROR]
 ```
 
@@ -173,16 +172,15 @@
   -i INPUT_MEAS, --input-meas INPUT_MEAS
                         path to the input measurement file or directory containing input measurement files.
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         output directory
   -q QC_CRITERIA, --qc-criteria QC_CRITERIA
                         path to json file with QC selection criteria (default: $(module-qc-analysis-tools --prefix)/analysis_cuts.json)
   -l LAYER, --layer LAYER
-                        Layer of module, used for applying correct QC criteria settings. Options: L0, L1, L2
-                        (default)
+                        Layer of module, used for applying correct QC criteria settings. Default setting uses information from production database. Options: L0, L1, L2.
   --permodule           Store results in one file per module (default: one file per chip)
   -f {root,numpy}, --fit-method {root,numpy}
                         fitting method
   -v VERBOSITY, --verbosity VERBOSITY
                         Log level [options: DEBUG, INFO (default), WARNING, ERROR]
   --verbose             verbose mode
 
@@ -207,16 +205,15 @@
   -i INPUT_MEAS, --input-meas INPUT_MEAS
                         path to the input measurement file or directory containing input measurement files.
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         output directory
   -q QC_CRITERIA, --qc-criteria QC_CRITERIA
                         path to json file with QC selection criteria (default: $(module-qc-analysis-tools --prefix)/analysis_cuts.json)
   -l LAYER, --layer LAYER
-                        Layer of module, used for applying correct QC criteria settings. Options: L0, L1, L2
-                        (default)
+                        Layer of module, used for applying correct QC criteria settings. Default setting uses information from production database. Options: L0, L1, L2.
   --permodule           Store results in one file per module (default: one file per chip)
   -n NCHIPS, --nChips NCHIPS
                         Number of chips powered in parallel (e.g. 4 for a quad module, 3 for a triplet, 1 for an
                         SCC.)
   -f {root,numpy}, --fit-method {root,numpy}
                         fitting method
   -v VERBOSITY, --verbosity VERBOSITY
@@ -244,16 +241,15 @@
   -i INPUT_MEAS, --input-meas INPUT_MEAS
                         path to the input measurement file or directory containing input measurement files.
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         output directory
   -q QC_CRITERIA, --qc-criteria QC_CRITERIA
                         path to json file with QC selection criteria (default: $(module-qc-analysis-tools --prefix)/analysis_cuts.json)
   -l LAYER, --layer LAYER
-                        Layer of module, used for applying correct QC criteria settings. Options: L0, L1, L2
-                        (default)
+                        Layer of module, used for applying correct QC criteria settings. Default setting uses information from production database. Options: L0, L1, L2.
   --permodule           Store results in one file per module (default: one file per chip)
   -f {root,numpy}, --fit-method {root,numpy}
                         fitting method
   -v VERBOSITY, --verbosity VERBOSITY
                         Log level [options: DEBUG, INFO (default), WARNING, ERROR]
 ```
 
@@ -277,16 +273,15 @@
   -i INPUT_MEAS, --input-meas INPUT_MEAS
                         path to the input measurement file or directory containing input measurement files.
   -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         output directory
   -q QC_CRITERIA, --qc-criteria QC_CRITERIA
                         path to json file with QC selection criteria (default: $(module-qc-analysis-tools --prefix)/analysis_cuts.json)
   -l LAYER, --layer LAYER
-                        Layer of module, used for applying correct QC criteria settings. Options: L0, L1, L2
-                        (default)
+                        Layer of module, used for applying correct QC criteria settings. Default setting uses information from production database. Options: L0, L1, L2.
   --permodule           Store results in one file per module (default: one file per chip)
   -v VERBOSITY, --verbosity VERBOSITY
                         Log level [options: DEBUG, INFO (default), WARNING, ERROR]
 ```
 
 </details>
```

