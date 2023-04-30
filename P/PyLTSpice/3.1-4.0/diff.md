# Comparing `tmp/PyLTSpice-3.1.tar.gz` & `tmp/PyLTSpice-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\sandbox\PyLTSpice_GitHub_nunobrum\dist\.tmp-ifxk38c3\PyLTSpice-3.1.tar", last modified: Sun Jan 22 22:21:54 2023, max compression
+gzip compressed data, was "C:\sandbox\PySpice\dist\.tmp-dascasfp\PyLTSpice-4.0.tar", last modified: Sun Apr 30 22:32:38 2023, max compression
```

## Comparing `PyLTSpice-3.1.tar` & `PyLTSpice-4.0.tar`

### file list

```diff
@@ -1,31 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-01-22 22:21:54.185546 PyLTSpice-3.1/
--rw-rw-rw-   0        0        0    35823 2019-05-13 20:30:20.000000 PyLTSpice-3.1/LICENSE
--rw-rw-rw-   0        0        0    54895 2023-01-22 22:21:54.185546 PyLTSpice-3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-01-22 22:21:54.175572 PyLTSpice-3.1/PyLTSpice/
--rw-rw-rw-   0        0        0     9083 2023-01-06 15:27:38.000000 PyLTSpice-3.1/PyLTSpice/Histogram.py
--rw-rw-rw-   0        0        0      347 2023-01-02 18:18:52.000000 PyLTSpice-3.1/PyLTSpice/LTSpiceBatch.py
--rw-rw-rw-   0        0        0      329 2023-01-02 18:18:52.000000 PyLTSpice-3.1/PyLTSpice/LTSpice_RawRead.py
--rw-rw-rw-   0        0        0      328 2023-01-02 18:18:52.000000 PyLTSpice-3.1/PyLTSpice/LTSpice_RawWrite.py
--rw-rw-rw-   0        0        0    32325 2023-01-06 15:27:38.000000 PyLTSpice-3.1/PyLTSpice/LTSteps.py
--rw-rw-rw-   0        0        0     6040 2023-01-06 15:27:38.000000 PyLTSpice-3.1/PyLTSpice/SemiDevOpReader.py
--rw-rw-rw-   0        0        0    44721 2023-01-18 08:02:16.000000 PyLTSpice-3.1/PyLTSpice/SpiceEditor.py
--rw-rw-rw-   0        0        0      225 2023-01-02 18:18:52.000000 PyLTSpice-3.1/PyLTSpice/__init__.py
--rw-rw-rw-   0        0        0     2576 2023-01-06 15:27:38.000000 PyLTSpice-3.1/PyLTSpice/detect_encoding.py
--rw-rw-rw-   0        0        0    14072 2023-01-06 15:27:38.000000 PyLTSpice-3.1/PyLTSpice/raw_classes.py
--rw-rw-rw-   0        0        0    30662 2023-01-22 21:25:10.000000 PyLTSpice-3.1/PyLTSpice/raw_read.py
--rw-rw-rw-   0        0        0    20346 2023-01-06 15:27:38.000000 PyLTSpice-3.1/PyLTSpice/raw_write.py
--rw-rw-rw-   0        0        0     4808 2023-01-06 15:27:38.000000 PyLTSpice-3.1/PyLTSpice/sim_analysis.py
--rw-rw-rw-   0        0        0    21706 2023-01-22 22:06:13.000000 PyLTSpice-3.1/PyLTSpice/sim_batch.py
--rw-rw-rw-   0        0        0     7373 2023-01-06 15:27:38.000000 PyLTSpice-3.1/PyLTSpice/sim_stepping.py
--rw-rw-rw-   0        0        0    10037 2023-01-22 21:59:00.000000 PyLTSpice-3.1/PyLTSpice/simulator.py
--rw-rw-rw-   0        0        0    11563 2023-01-06 15:27:38.000000 PyLTSpice-3.1/PyLTSpice/sweep_iterators.py
-drwxrwxrwx   0        0        0        0 2023-01-22 22:21:54.183584 PyLTSpice-3.1/PyLTSpice.egg-info/
--rw-rw-rw-   0        0        0    54895 2023-01-22 22:21:54.000000 PyLTSpice-3.1/PyLTSpice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2023-01-22 22:21:54.000000 PyLTSpice-3.1/PyLTSpice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-22 22:21:54.000000 PyLTSpice-3.1/PyLTSpice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-01-22 22:21:54.000000 PyLTSpice-3.1/PyLTSpice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-01-22 22:21:54.000000 PyLTSpice-3.1/PyLTSpice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13047 2023-01-22 22:14:30.000000 PyLTSpice-3.1/README.md
--rw-rw-rw-   0        0        0      714 2023-01-22 22:04:06.000000 PyLTSpice-3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-22 22:21:54.186541 PyLTSpice-3.1/setup.cfg
--rw-rw-rw-   0        0        0     1179 2023-01-02 18:18:52.000000 PyLTSpice-3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-30 22:32:37.998312 PyLTSpice-4.0/
+-rw-rw-rw-   0        0        0    35823 2022-12-04 12:18:59.000000 PyLTSpice-4.0/LICENSE
+-rw-rw-rw-   0        0        0    56547 2023-04-30 22:32:37.997314 PyLTSpice-4.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-30 22:32:37.935480 PyLTSpice-4.0/PyLTSpice/
+drwxrwxrwx   0        0        0        0 2023-04-30 22:32:37.948445 PyLTSpice-4.0/PyLTSpice/PyLTSpice.egg-info/
+-rw-rw-rw-   0        0        0    56547 2023-04-30 22:32:37.000000 PyLTSpice-4.0/PyLTSpice/PyLTSpice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1122 2023-04-30 22:32:37.000000 PyLTSpice-4.0/PyLTSpice/PyLTSpice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-30 22:32:37.000000 PyLTSpice-4.0/PyLTSpice/PyLTSpice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      159 2023-04-30 22:32:37.000000 PyLTSpice-4.0/PyLTSpice/PyLTSpice.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-04-30 22:32:37.000000 PyLTSpice-4.0/PyLTSpice/PyLTSpice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-04-30 22:32:37.000000 PyLTSpice-4.0/PyLTSpice/PyLTSpice.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-30 22:32:37.955426 PyLTSpice-4.0/PyLTSpice/client_server/
+-rw-rw-rw-   0        0        0        0 2023-04-08 17:08:22.000000 PyLTSpice-4.0/PyLTSpice/client_server/__init__.py
+-rw-rw-rw-   0        0        0     8400 2023-04-19 21:29:58.000000 PyLTSpice-4.0/PyLTSpice/client_server/sim_client.py
+-rw-rw-rw-   0        0        0     5427 2023-04-23 11:45:04.000000 PyLTSpice-4.0/PyLTSpice/client_server/sim_server.py
+-rw-rw-rw-   0        0        0     4737 2023-04-23 11:45:04.000000 PyLTSpice-4.0/PyLTSpice/client_server/srv_sim_runner.py
+drwxrwxrwx   0        0        0        0 2023-04-30 22:32:37.959417 PyLTSpice-4.0/PyLTSpice/log/
+-rw-rw-rw-   0        0        0        0 2023-04-08 22:49:34.000000 PyLTSpice-4.0/PyLTSpice/log/__init__.py
+-rw-rw-rw-   0        0        0    29860 2023-02-23 16:46:29.000000 PyLTSpice-4.0/PyLTSpice/log/ltsteps.py
+-rw-rw-rw-   0        0        0     6047 2023-04-30 22:25:50.000000 PyLTSpice-4.0/PyLTSpice/log/semi_dev_op_reader.py
+drwxrwxrwx   0        0        0        0 2023-04-30 22:32:37.966398 PyLTSpice-4.0/PyLTSpice/raw/
+-rw-rw-rw-   0        0        0        0 2023-04-08 22:49:18.000000 PyLTSpice-4.0/PyLTSpice/raw/__init__.py
+-rw-rw-rw-   0        0        0    14667 2023-04-30 20:34:58.000000 PyLTSpice-4.0/PyLTSpice/raw/raw_classes.py
+-rw-rw-rw-   0        0        0     5609 2023-04-30 17:57:03.000000 PyLTSpice-4.0/PyLTSpice/raw/raw_convert.py
+-rw-rw-rw-   0        0        0    39972 2023-04-30 22:25:50.000000 PyLTSpice-4.0/PyLTSpice/raw/raw_read.py
+-rw-rw-rw-   0        0        0    16752 2023-04-30 22:29:26.000000 PyLTSpice-4.0/PyLTSpice/raw/raw_write.py
+drwxrwxrwx   0        0        0        0 2023-04-30 22:32:37.989336 PyLTSpice-4.0/PyLTSpice/sim/
+-rw-rw-rw-   0        0        0        0 2023-02-12 22:11:29.000000 PyLTSpice-4.0/PyLTSpice/sim/__init__.py
+-rw-rw-rw-   0        0        0     8568 2023-04-30 18:47:14.000000 PyLTSpice-4.0/PyLTSpice/sim/ltspice_simulator.py
+-rw-rw-rw-   0        0        0     4636 2023-04-26 20:04:46.000000 PyLTSpice-4.0/PyLTSpice/sim/ngspice_simulator.py
+-rw-rw-rw-   0        0        0     1505 2023-04-23 16:20:26.000000 PyLTSpice-4.0/PyLTSpice/sim/process_callback.py
+-rw-rw-rw-   0        0        0     6059 2023-04-23 21:06:11.000000 PyLTSpice-4.0/PyLTSpice/sim/run_task.py
+-rw-rw-rw-   0        0        0     4809 2023-04-26 21:05:36.000000 PyLTSpice-4.0/PyLTSpice/sim/sim_analysis.py
+-rw-rw-rw-   0        0        0    10749 2023-04-23 14:18:49.000000 PyLTSpice-4.0/PyLTSpice/sim/sim_batch.py
+-rw-rw-rw-   0        0        0    23686 2023-04-30 18:47:14.000000 PyLTSpice-4.0/PyLTSpice/sim/sim_runner.py
+-rw-rw-rw-   0        0        0     9221 2023-04-26 21:05:36.000000 PyLTSpice-4.0/PyLTSpice/sim/sim_stepping.py
+-rw-rw-rw-   0        0        0     4652 2023-04-08 19:00:33.000000 PyLTSpice-4.0/PyLTSpice/sim/simulator.py
+-rw-rw-rw-   0        0        0    46608 2023-04-30 22:25:50.000000 PyLTSpice-4.0/PyLTSpice/sim/spice_editor.py
+-rw-rw-rw-   0        0        0     7384 2023-04-07 13:28:50.000000 PyLTSpice-4.0/PyLTSpice/sim/xyce_simulator.py
+drwxrwxrwx   0        0        0        0 2023-04-30 22:32:37.993327 PyLTSpice-4.0/PyLTSpice/utils/
+-rw-rw-rw-   0        0        0     2678 2023-04-29 18:03:58.000000 PyLTSpice-4.0/PyLTSpice/utils/detect_encoding.py
+-rw-rw-rw-   0        0        0    11563 2023-01-15 18:28:54.000000 PyLTSpice-4.0/PyLTSpice/utils/sweep_iterators.py
+-rw-rw-rw-   0        0        0    14768 2023-04-30 22:25:50.000000 PyLTSpice-4.0/README.md
+-rw-rw-rw-   0        0        0     1179 2023-04-30 18:15:46.000000 PyLTSpice-4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-30 22:32:37.999311 PyLTSpice-4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-30 22:32:37.995320 PyLTSpice-4.0/tests/
+-rw-rw-rw-   0        0        0      801 2023-04-23 17:09:47.000000 PyLTSpice-4.0/tests/test_ltsteps.py
```

### Comparing `PyLTSpice-3.1/LICENSE` & `PyLTSpice-4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyLTSpice-3.1/PKG-INFO` & `PyLTSpice-4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: PyLTSpice
-Version: 3.1
+Version: 4.0
 Summary: A set of tools to Automate LTSpice simulations
-Home-page: https://github.com/nunobrum/PyLTSpice
-Author: Nuno Brum
 Author-email: Nuno Brum <me@nunobrum.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -692,68 +690,74 @@
 # README #
 
 PyLTSpice is a toolchain of python utilities design to interact with LTSpice and NGSpice Electronic Simulator.
 
 ## What is contained in this repository ##
 
 * __LTSteps.py__
-An utility that extracts from LTSpice output files data, and formats it for import in a spreadsheet, such like Excel or Calc.
+  An utility that extracts from LTSpice output files data, and formats it for import in a spreadsheet, such like Excel
+  or Calc.
 
 * __raw_read.py__
-A pure python class that serves to read raw files into a python class.
+  A pure python class that serves to read raw files into a python class.
 
 * __raw_write.py__
-A class to write RAW files that can be read by LTSpice Wave Application.
+  A class to write RAW files that can be read by LTSpice Wave Application.
 
 * __Histogram.py__
-A python script that uses numpy and matplotlib to create an histogram and calculate the sigma deviations. This is useful for Monte-Carlo analysis.
+  A python script that uses numpy and matplotlib to create an histogram and calculate the sigma deviations. This is
+  useful for Monte-Carlo analysis.
 
 * __sim_batch.py__
-This is a script to launch Spice Simulations. This is useful because:
+  This is a script to launch Spice Simulations. This is useful because:
 
     - Can overcome the limitation of only stepping 3 parameters
     - Different types of simulations .TRAN .AC .NOISE can be run in a single batch
     - The RAW Files are smaller and easier to treat
     - When used with the RawRead.py and LTSteps.py, validation of the circuit can be done automatically.
     - Different models can be simulated in a single batch, by using the following instructions:
-        - `set_element_model('D1', '1N4148') # Replaces the Diode D1 with the model 1N4148 `  
-        - `set_component_value('R2', '33k') # Replaces the value of R2 by 33k`  
-        - `set_parameters(run=1, TEMP=80) # Creates or updates the netlist to have .PARAM run=1 or .PARAM TEMP=80`  
-        - `add_instructions(".STEP run -1 1023 1", ".dc V1 -5 5") `  
-        - `remove_instruction(".STEP run -1 1023 1")  # Removes previously added instruction`  
-        - `reset_netlist() # Resets all edits done to the netlist.`  
+        - `set_element_model('D1', '1N4148') # Replaces the Diode D1 with the model 1N4148 `
+        - `set_component_value('R2', '33k') # Replaces the value of R2 by 33k`
+        - `set_parameters(run=1, TEMP=80) # Creates or updates the netlist to have .PARAM run=1 or .PARAM TEMP=80`
+        - `add_instructions(".STEP run -1 1023 1", ".dc V1 -5 5") `
+        - `remove_instruction(".STEP run -1 1023 1")  # Removes previously added instruction`
+        - `reset_netlist() # Resets all edits done to the netlist.`
 
-    Note: It was only tested with Windows based installations.
+  Note: It was only tested with Windows based installations.
 
 ## How to Install ##
-`pip install PyLTSpice `  
+
+`pip install PyLTSpice `
 
 ### Updating PyLTSpice ###
- `pip install --upgrade PyLTSpice `  
+
+`pip install --upgrade PyLTSpice `
 
 ### Using GITHub ###
 
- `git clone https://github.com/nunobrum/PyLTSpice.git `  
+`git clone https://github.com/nunobrum/PyLTSpice.git `
 
 If using this method it would be good to add the path where you cloned the site to python path.
 
- `import sys `  
- `sys.path.append(<path to PyLTSpice>) `  
+`import sys `  
+`sys.path.append(<path to PyLTSpice>) `
 
 ## How to use ##
 
 Here follows a quick outlook on how to use each of the tools.
 
 More comprehensive documentation can be found in https://pyltspice.readthedocs.io/en/latest/
 
 ## LICENSE ##
+
 GNU V3 License
 (refer to the LICENSE file)
 
 ### raw_read.py ###
+
 The example below reads the data from a Spice Simulation called
 "TRAN - STEP.raw" and displays all steps of the "I(R1)" trace in a matplotlib plot
 
  ```python
 from PyLTSpice import RawRead
 
 from matplotlib import pyplot as plt
@@ -764,97 +768,107 @@
 print(LTR.get_raw_property())
 
 IR1 = LTR.get_trace("I(R1)")
 x = LTR.get_trace('time')  # Gets the time axis
 steps = LTR.get_steps()
 for step in range(len(steps)):
     # print(steps[step])
-    plt.plot(x.get_time_axis(step), IR1.get_wave(step), label=steps[step])
+    plt.plot(x.get_wave(step), IR1.get_wave(step), label=steps[step])
 
 plt.legend()  # order a legend
 plt.show()
  ```   
 
 ### raw_write.py ###
-The following example writes a RAW file with a 3 milliseconds transient simulation sine with a
-10kHz and a cosine with 9.997kHz
+
+The following example writes a RAW file with a 3 milliseconds transient simulation sine with a 10kHz and a cosine with
+9.997kHz
+
  ```python
 import numpy as np
 from PyLTSpice import Trace, RawWrite
 
-LW = RawWrite()
+LW = RawWrite(fastacces=False)
 tx = Trace('time', np.arange(0.0, 3e-3, 997E-11))
 vy = Trace('N001', np.sin(2 * np.pi * tx.data * 10000))
 vz = Trace('N002', np.cos(2 * np.pi * tx.data * 9970))
 LW.add_trace(tx)
 LW.add_trace(vy)
 LW.add_trace(vz)
-LW.save("teste_w.raw")
-
+LW.save("teste_snippet1.raw")
  ```   
 
-
 ### sim_batch.py ###
-This module is used to launch LTSPice simulations. Results then can be processed with either the RawRead
-or with the LTSteps module to read the log file which can contain .MEAS results.
 
-The script will firstly invoke the LTSpice in command line to generate a netlist, and then this netlist can be
-updated directly by the script, in order to change component values, parameters or simulation commands.
+This module is used to launch LTSPice simulations. Results then can be processed with either the RawRead or with the
+LTSteps module to read the log file which can contain .MEAS results.
+
+The script will firstly invoke the LTSpice in command line to generate a netlist, and then this netlist can be updated
+directly by the script, in order to change component values, parameters or simulation commands.
 
 Here follows an example of operation.
 
 ```python
-import os
-from PyLTSpice import SimCommander
-
-def processing_data(raw_file, log_file):
-    print("Handling the simulation data of %s, log file %s" % (raw_file, log_file))
+from PyLTSpice import SimRunner
+from PyLTSpice import SpiceEditor
 
 # select spice model
-LTC = SimCommander("Batch_Test.asc")
+LTC = SimRunner(output_folder='./temp')
+LTC.create_netlist('Batch_Test.asc')
+netlist = SpiceEditor('Batch_Test.net')
 # set default arguments
-LTC.set_parameters(res=0, cap=100e-6)
-LTC.set_component_value('R2', '2k')
-LTC.set_component_value('R1', '4k')
-LTC.set_element_model('V3', "SINE(0 1 3k 0 0 0)")
-# define simulation
-LTC.add_instructions(
-    "; Simulation settings",
-    ".param run = 0"
+netlist.set_parameters(res=0, cap=100e-6)
+netlist.set_component_value('R2', '2k')  # Modifying the value of a resistor
+netlist.set_component_value('R1', '4k')
+netlist.set_element_model('V3', "SINE(0 1 3k 0 0 0)")  # Modifying the
+netlist.set_component_value('XU1:C2', 20e-12)  # modifying a define simulation
+netlist.add_instructions(
+        "; Simulation settings",
+        ".param run = 0"
 )
 
 for opamp in ('AD712', 'AD820'):
-    LTC.set_element_model('XU1', opamp)
+    netlist.set_element_model('XU1', opamp)
     for supply_voltage in (5, 10, 15):
-        LTC.set_component_value('V1', supply_voltage)
-        LTC.set_component_value('V2', -supply_voltage)
-        # overriding he automatic netlist naming
-        run_netlist_file = "{}_{}_{}.net".format(LTC.circuit_radic, opamp, supply_voltage)
-        LTC.run(run_filename=run_netlist_file, callback=processing_data)
-
-
-LTC.reset_netlist()
-LTC.add_instructions(
-    "; Simulation settings",
-    ".ac dec 30 10 1Meg",
-    ".meas AC Gain MAX mag(V(out)) ; find the peak response and call it ""Gain""",
-    ".meas AC Fcut TRIG mag(V(out))=Gain/sqrt(2) FALL=last"
+        netlist.set_component_value('V1', supply_voltage)
+        netlist.set_component_value('V2', -supply_voltage)
+        print("simulating OpAmp", opamp, "Voltage", supply_voltage)
+        LTC.run(netlist)
+
+for raw, log in LTC:
+    print("Raw file: %s, Log file: %s" % (raw, log))
+    # do something with the data
+    # raw_data = RawRead(raw)
+    # log_data = LTSteps(log)
+    # ...
+
+netlist.reset_netlist()
+netlist.add_instructions(
+        "; Simulation settings",
+        ".ac dec 30 10 1Meg",
+        ".meas AC Gain MAX mag(V(out)) ; find the peak response and call it ""Gain""",
+        ".meas AC Fcut TRIG mag(V(out))=Gain/sqrt(2) FALL=last"
 )
 
-LTC.run()
-LTC.wait_completion()
+# Sim Statistics
+print('Successful/Total Simulations: ' + str(LTC.okSim) + '/' + str(LTC.runno))
+
+enter = input("Press enter to delete created files")
+if enter == '':
+    LTC.file_cleanup()
 
 # Sim Statistics
 print('Successful/Total Simulations: ' + str(LTC.okSim) + '/' + str(LTC.runno))
 ```
 
 ### LTSteps.py ###
-This module defines a class that can be used to parse LTSpice log files where the information about .STEP information is written.
-There are two possible usages of this module, either programmatically by importing the module and then accessing data through the
-class as exemplified here:
+
+This module defines a class that can be used to parse LTSpice log files where the information about .STEP information is
+written. There are two possible usages of this module, either programmatically by importing the module and then
+accessing data through the class as exemplified here:
 
 ```python
 from PyLTSpice.LTSteps import LTSpiceLogReader
 
 data = LTSpiceLogReader("Batch_Test_AD820_15.log")
 
 print("Number of steps  :", data.step_count)
@@ -869,22 +883,24 @@
     print(' '.join([f"{data[step][i]:15}" for step in step_names]), end='')  # Print steps names with no new line
     print(' '.join([f"{data[name][i]:15}" for name in meas_names]), end='\n')  # Print Header
 
 print("Total number of measures found :", data.measure_count)
 ```
 
 The second possibility is to use the module directly on the command line
- `python -m PyLTSpice.LTSteps <filename> `
- The <filename> can be either be a log file (.log), a data export file (.txt) or a measurement output file (.meas)
- This will process all the data and export it automatically into a text file with the extension (tlog, tsv, tmeas)
- where the data read is formatted into a more convenient tab separated format.
- In case the <logfile> is not provided, the script will scan the directory and process the newest log, txt or out file found.
+`python -m PyLTSpice.LTSteps <filename> `
+The <filename> can be either be a log file (.log), a data export file (.txt) or a measurement output file (.meas)
+This will process all the data and export it automatically into a text file with the extension (tlog, tsv, tmeas)
+where the data read is formatted into a more convenient tab separated format. In case the <logfile> is not provided, the
+script will scan the directory and process the newest log, txt or out file found.
 
 ### Histogram.py ###
+
 This module uses the data inside on the filename to produce an histogram image.
+
  ```
 Usage: Histogram.py [options] LOG_FILE TRACE
 
 Options:
   --version             show program's version number and exit
   -h, --help            show this help message and exit
   -s SIGMA, --sigma=SIGMA
@@ -904,129 +920,161 @@
                         Range of the X axis to use for the histogram in the
                         form min:max. Example: -r -1:1
   -C, --clipboard       If the data from the clipboard is to be used.
   -i IMAGEFILE, --image=IMAGEFILE
                         Name of the image File. extension 'png'    
  ```
 
+### rawconvert.py ###
+
+A tool to convert .raw files into csv or Excel files.
+
+```
+Usage: raw_convert.py [options] <rawfile> <trace_list>
+
+Options:
+  --version             show program's version number and exit
+  -h, --help            show this help message and exit
+  -o FILE, --output=FILE
+                        Output file name. Use .csv for CSV output, .xlsx for
+                        Excel output
+  -c, --clipboard       Output to clipboard
+  -v, --verbose         Verbose output
+  -s SEPARATOR, --sep=SEPARATOR
+                        Value separator for CSV output. Default: "\t" <TAB>
+                        Example: -d ";"
+
+
+```
+
 ### SemiDevOpReader.py ###
-This module is used to read from LTSpice log files Semiconductor Devices Operating Point Information.
-A more detailed documentation is directly included in the source file docstrings.
+
+This module is used to read from LTSpice log files Semiconductor Devices Operating Point Information. A more detailed
+documentation is directly included in the source file docstrings.
 
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
-* Version 3.1\
-Supporting the new improved LTspice version from ADI. \
-Adding the get_wave() directly to the RawRead Class.
+
+* Version 4.0.0\
+  Separating the SimCommander into two separate classes, one for the spice netlist editing (SpiceEditor) and another for
+  the simulation execution (SimRunner).\
+  Implementing simulation server to allow for remote simulation execution and the respective client.\
+  Supporting Wiggler element in the new LTSpiceXVII.\
+  Renaming all files into lowercase.\
+  Creating Error classes for better error handling.\
+  Adding support for other simulators (ex: ngspice) where the simulator is defined by a class. This
+  support class needs to be a subclass of the abstract class Simulator.\
+  Enormous improvement in the documentation of the code.  
 
 * Version 3.0\
-Eliminating the LTSpice prefixes from files and classes.\
-Adopting the lowercase convention for filenames.
+  Eliminating the LTSpice prefixes from files and classes.\
+  Adopting the lowercase convention for filenames.
 
 * Version 2.3.1\
-Bug fix on the parameter replacement
+  Bug fix on the parameter replacement
 
 * Version 2.3\
-Supporting the creation of RAW Noise Analysis\
-Bug Fixes (See GitHub Log) 
+  Supporting the creation of RAW Noise Analysis\
+  Bug Fixes (See GitHub Log)
 
 * Version 2.2\
-Making numpy as an requirement and eliminating all code that avoided the use of numpy\
-Using new packaging tool\
-Fixes on the LTSpice_RawWrite\
-Fixes in the handling of stepped operating point simulations 
+  Making numpy as an requirement and eliminating all code that avoided the use of numpy\
+  Using new packaging tool\
+  Fixes on the LTSpice_RawWrite\
+  Fixes in the handling of stepped operating point simulations
 
 * Version 2.1\
-Adopting minimum python version 3.7\
-Starting to use unit tests to validate all modules and improving testbenches\
-Compatibility with NGSpice\
-Avoiding the use of setup.py as per PEP517 and PEP518\
-Bug Fixes (See GitHub log for more information)\
-Improvements on the management of stepped data in the LTSpice_RawRead.py
+  Adopting minimum python version 3.7\
+  Starting to use unit tests to validate all modules and improving testbenches\
+  Compatibility with NGSpice\
+  Avoiding the use of setup.py as per PEP517 and PEP518\
+  Bug Fixes (See GitHub log for more information)\
+  Improvements on the management of stepped data in the LTSpice_RawRead.py
 
 * Version 2.0.2\
-Improvements on Encoding detection
+  Improvements on Encoding detection
 
 * Version 2.0\
-International Support using the correct encoding when loading log files.\
-Code Optimizations on the LTSpice_RawReader that allow faster data loading.\
-Improving the functionality on the LTSpice_RawWriter.py\
-Adding support to editing components inside subcircuits (.subckt)\
-Supporting resistors with Model Definitions\
-Fixing problem with LTSpiceLogReader that would return messed up data\
-Fixing problem with replacing the file extension in certain names\
-Correcting problem with deprecations on the numpy functions used by the Histogram.py\
-Adding back the README.md that somehow was deleted
+  International Support using the correct encoding when loading log files.\
+  Code Optimizations on the LTSpice_RawReader that allow faster data loading.\
+  Improving the functionality on the LTSpice_RawWriter.py\
+  Adding support to editing components inside subcircuits (.subckt)\
+  Supporting resistors with Model Definitions\
+  Fixing problem with LTSpiceLogReader that would return messed up data\
+  Fixing problem with replacing the file extension in certain names\
+  Correcting problem with deprecations on the numpy functions used by the Histogram.py\
+  Adding back the README.md that somehow was deleted
 
 * Version 1.9\
-Adding support for µ character in the SpiceEditor.\
-Adding get_component_floatvalue() method in the netlist manipulating class that handles the conversion of 
-  numeric fields into a float. This function takes into account the engineering qualifiers 'k' for kilos, 'm' or milis, 
+  Adding support for µ character in the SpiceEditor.\
+  Adding get_component_floatvalue() method in the netlist manipulating class that handles the conversion of numeric
+  fields into a float. This function takes into account the engineering qualifiers 'k' for kilos, 'm' or milis,
   'u' or 'µ' for microns, 'n' for nanos, 'f' for femtos and 'Meg' for Megas.
 
 * Version 1.8\
-Uniforming License reference across files and improvements on the documentation\
-An enormous and wholehearted thanks to Logan Herrera (lpherr) <logan.herrera.github@gmail.com> for the improvements in the documentation.\
-Bugfix on the add_LTspiceRunCmdLineSwitches() ; Supporting .param name value format\
-Allowing the LTSpiceRawRead to proceed when the log file can't be found or when there are problems reading it.
+  Uniforming License reference across files and improvements on the documentation\
+  An enormous and wholehearted thanks to Logan Herrera (lpherr) <logan.herrera.github@gmail.com> for the improvements in
+  the documentation.\
+  Bugfix on the add_LTspiceRunCmdLineSwitches() ; Supporting .param name value format\
+  Allowing the LTSpiceRawRead to proceed when the log file can't be found or when there are problems reading it.
 * Version 1.7\
-Running in Linux under wine is now possible
+  Running in Linux under wine is now possible
 
 * Version 1.6\
-Adding LTSpice_RawWrite. Adding documentation.
+  Adding LTSpice_RawWrite. Adding documentation.
 
 * Version 1.5\
-Small fixes and improvements on the class usage. No added features
+  Small fixes and improvements on the class usage. No added features
 
 * Version 1.4 \
-Adding the LTSpice_SemiDevOpReader module\
-Re-enabling the Histogram functions which where disabled by mistake.
+  Adding the LTSpice_SemiDevOpReader module\
+  Re-enabling the Histogram functions which where disabled by mistake.
 
 * Version 1.3 \
-Bug fixes on the SpiceEditor Class
+  Bug fixes on the SpiceEditor Class
 
 * Version 1.2 \
-README.md:
-Adding link to readthedocs documentation\
-All files:
-Comprehensive documentation on how to use each module
+  README.md:
+  Adding link to readthedocs documentation\
+  All files:
+  Comprehensive documentation on how to use each module
 
 * Version 1.1\
-README.md:
-Updated the description\
-LTSpiceBatch.py:
-Corrected the name of the returned raw file.\
-Added comments throughout the code and cleanup
+  README.md:
+  Updated the description\
+  LTSpiceBatch.py:
+  Corrected the name of the returned raw file.\
+  Added comments throughout the code and cleanup
 
 * Version 1.0\
-LTSpiceBatch.py:
-Implemented an new approach (NOT BACKWARDS COMPATIBLE), that avoids the usage of the sim_settings.inc file.
-And allows to modify not only parameters, but also models and even the simulation commands.\
-LTSpice_RawRead.py:
-Added the get_time_axis method to the RawRead class to avoid the problems with negative values on
-time axis, when 2nd order compression is enabled in LTSpice.\
-LTSteps.py:
-Modified the LTSteps so it can also read measurements on log files without any steps done.
+  LTSpiceBatch.py:
+  Implemented an new approach (NOT BACKWARDS COMPATIBLE), that avoids the usage of the sim_settings.inc file. And allows
+  to modify not only parameters, but also models and even the simulation commands.\
+  LTSpice_RawRead.py:
+  Added the get_time_axis method to the RawRead class to avoid the problems with negative values on time axis, when 2nd
+  order compression is enabled in LTSpice.\
+  LTSteps.py:
+  Modified the LTSteps so it can also read measurements on log files without any steps done.
 
 
 * Version 0.6\
-Histogram.py now has an option to make the histogram directly from values stored in the clipboard
+  Histogram.py now has an option to make the histogram directly from values stored in the clipboard
 
 * Version 0.5\
-The LTSpice_RawReader.py now uses the struc.unpack function for a faster execution
+  The LTSpice_RawReader.py now uses the struc.unpack function for a faster execution
 
 * Version 0.4\
-Added LTSpiceBatch.py to the collection of tools
+  Added LTSpiceBatch.py to the collection of tools
 
 * Version 0.3\
-A version of LTSteps that can be imported to use in a higher level script 
+  A version of LTSteps that can be imported to use in a higher level script
 
 * Version 0.2\
-Adding LTSteps.py and Histogram.py
+  Adding LTSteps.py and Histogram.py
 
 * Version 0.1 \
-First commit to the bitbucket repository.
+  First commit to the bitbucket repository.
```

### Comparing `PyLTSpice-3.1/PyLTSpice/LTSteps.py` & `PyLTSpice-4.0/PyLTSpice/log/ltsteps.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,17 @@
 #!/usr/bin/env python
 # coding=utf-8
 
 # -------------------------------------------------------------------------------
-#    ____        _   _____ ____        _
-#   |  _ \ _   _| | |_   _/ ___| _ __ (_) ___ ___
-#   | |_) | | | | |   | | \___ \| '_ \| |/ __/ _ \
-#   |  __/| |_| | |___| |  ___) | |_) | | (_|  __/
-#   |_|    \__, |_____|_| |____/| .__/|_|\___\___|
-#          |___/                |_|
-#
-# Name:        LTSteps.py
+# Name:        ltsteps.py
 # Purpose:     Process LTSpice output files and align data for usage in a spread-
 #              sheet tool such as Excel, or Calc.
 #
 # Author:      Nuno Brum (nuno.brum@gmail.com)
 #
-# Created:     19-05-2014
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
 
 """
 This module allows to process data generated by LTSpice during simulation. There are three types of files that are
 handled by this module.
 
@@ -80,53 +72,49 @@
 as one of the columns.
 
 If `<path_to_filename>` argument is ommited, the script will automatically search for the newest .log/.txt/.mout file
 and use it.
 
 """
 __author__ = "Nuno Canto Brum <me@nunobrum.com>"
-__copyright__ = "Copyright 2017, Fribourg Switzerland"
+__copyright__ = "Copyright 2023, Fribourg Switzerland"
 
 import math
 import re
-import os
-import sys
 from collections import OrderedDict
 from typing import Union, Iterable, List
-from .detect_encoding import detect_encoding
-
-if __name__ == "__main__":
-    def message(*strs):
-        for string in strs:
-            print(string)
-else:
-    def message(*strs):
-        pass
+from ..utils.detect_encoding import detect_encoding
 
 
 class LTComplex(object):
     """
     Class to represent complex numbers as exported by LTSpice
     """
     complex_match = re.compile(r"\((?P<mag>[^dB]*)(dB)?,(?P<ph>.*)°\)")
 
     def __init__(self, strvalue):
         a = self.complex_match.match(strvalue)
         if a:
             self.mag = float(a.group('mag'))
             self.ph = float(a.group('ph'))
+            self.unit = 'dB' if len(a.groups()) == 3 else ''
         else:
             raise ValueError("Invalid complex value format")
 
     def to_complex(self):
         ph = self.ph / 180 * math.pi
-        return complex(self.mag * math.cos(ph), self.mag * math.sin(ph))
+        if self.unit == '':
+            mag = self.mag
+        else:
+            mag = 10**(self.mag/20)  # Typically, we are working in voltages
+
+        return complex(mag * math.cos(ph), mag * math.sin(ph))
 
     def __str__(self):
-        return f"{self.mag},{self.ph}"
+        return f"{self.mag}{self.unit},{self.ph}°"
 
 
 def try_convert_value(value: Union[str, int, float]) -> Union[int, float, str]:
     """
     Tries to convert the string into an integer and if it fails, tries to convert to a float, if it fails, then returns the
     value as string.
 
@@ -199,33 +187,33 @@
     go_header = True
     run_no = 0  # Just to avoid warning, this is later overridden by the step information
     param_values = ""  # Just to avoid warning, this is later overridden by the step information
     regx = re.compile(r"Step Information: ([\w=\d\. -]+) +\(Run: (\d*)/\d*\)\n")
     for line in fin:
         if line.startswith("Step Information:"):
             match = regx.match(line)
-            # message(line, end="")
+            # print(line, end="")
             if match:
-                # message(match.groups())
+                # print(match.groups())
                 step, run_no = match.groups()
-                # message(step, line, end="")
+                # print(step, line, end="")
                 params = []
                 for param in step.split():
                     params.append(param.split('=')[1])
                 param_values = "\t".join(params)
 
                 if go_header:
                     header_keys = []
                     for param in step.split():
                         header_keys.append(param.split('=')[0])
                     param_header = "\t".join(header_keys)
                     fout.write("Run\t%s\t%s" % (param_header, headers))
-                    message("Run\t%s\t%s" % (param_header, headers))
+                    print("Run\t%s\t%s" % (param_header, headers))
                     go_header = False
-                    # message("%s\t%s"% (run_no, param_values))
+                    # print("%s\t%s"% (run_no, param_values))
         else:
             fout.write("%s\t%s\t%s" % (run_no, param_values, line))
 
     fin.close()
     fout.close()
 
 
@@ -263,19 +251,19 @@
         curr_dic = {}
         self.dataset = {}
 
         regx = re.compile(r"Step Information: ([\w=\d\. -]+) +\(Run: (\d*)/\d*\)\n")
         for line in fin:
             if line.startswith("Step Information:"):
                 match = regx.match(line)
-                # message(line, end="")
+                # print(line, end="")
                 if match:
-                    # message(match.groups())
+                    # print(match.groups())
                     step, run_no = match.groups()
-                    # message(step, line, end="")
+                    # print(step, line, end="")
                     curr_dic['runno'] = run_no
                     for param in step.split():
                         key, value = param.split('=')
                         curr_dic[key] = try_convert_value(value)
 
                     if go_header:
                         go_header = False  # This is executed only once
@@ -344,15 +332,15 @@
         # gain: vout_rms/vin_rms=1.99809 => Parameter
         # vout1m: v(out)=-0.0186257 at 0.001 => Point
         # fcutac=8.18166e+006 FROM 1.81834e+006 TO 1e+007 => AC Find Computation
         regx = re.compile(
                 r"^(?P<name>\w+)(:\s+.*)?=(?P<value>[\d\.E+\-\(\)dB,°]+)(( FROM (?P<from>[\d\.E+-]*) TO (?P<to>[\d\.E+-]*))|( at (?P<at>[\d\.E+-]*)))?",
                 re.IGNORECASE)
 
-        message("Processing LOG file", log_filename)
+        print("Processing LOG file", log_filename)
         with open(log_filename, 'r', encoding=self.encoding) as fin:
             line = fin.readline()
 
             while line:
                 if line.startswith("N-Period"):
                     import pandas as pd
                     # Read number of periods
@@ -426,15 +414,15 @@
                         period_dict[waveform] = []
                         waveform_list = period_dict[waveform]
 
                     # Add the data to the list
                     waveform_list.append(data_dict)
 
                 if line.startswith(".step"):
-                    # message(line)
+                    # print(line)
                     self.step_count += 1
                     tokens = line.strip('\r\n').split(' ')
                     for tok in tokens[1:]:
                         lhs, rhs = tok.split("=")
                         # Try to convert to int or float
                         rhs = try_convert_value(rhs)
 
@@ -461,38 +449,39 @@
                             measurements = [match.group('value'), match.group('from'), match.group('to')]
                         elif match.group('at'):
                             headers = [dataname, dataname + "_at"]
                             measurements = [match.group('value'), match.group('at')]
                         else:
                             headers = [dataname]
                             measurements = [match.group('value')]
-
+                        self.measure_count += 1
                         for k, title in enumerate(headers):
                             self.dataset[title] = [
                                 try_convert_value(measurements[k])]  # need to be a list for compatibility
                 line = fin.readline()
 
-            # message("Reading Measurements")
+            # print("Reading Measurements")
             dataname = None
 
             headers = []  # Initializing an empty parameters
             measurements = []
             while line:
                 line = line.strip('\r\n')
                 if line.startswith("Measurement: "):
                     if dataname:  # If previous measurement was saved
                         # store the info
                         if len(measurements):
-                            message("Storing Measurement %s (count %d)" % (dataname, len(measurements)))
+                            print("Storing Measurement %s (count %d)" % (dataname, len(measurements)))
+                            self.measure_count += len(measurements)
                             for k, title in enumerate(headers):
                                 self.dataset[title] = [line[k] for line in measurements]
                         headers = []
                         measurements = []
                     dataname = line[13:]  # text which is after "Measurement: ". len("Measurement: ") -> 13
-                    message("Reading Measurement %s" % line[13:])
+                    print("Reading Measurement %s" % line[13:])
                 else:
                     tokens = line.split("\t")
                     if len(tokens) >= 2:
                         try:
                             int(tokens[0])  # This instruction only serves to trigger the exception
                             meas = tokens[1:]  # [float(x) for x in tokens[1:]]
                             measurements.append(try_convert_values(meas))
@@ -501,26 +490,28 @@
                             if len(tokens) >= 3 and (tokens[2] == "FROM" or tokens[2] == 'at'):
                                 tokens[2] = dataname + '_' + tokens[2]
                             if len(tokens) >= 4 and tokens[3] == "TO":
                                 tokens[3] = dataname + "_TO"
                             headers = [dataname] + tokens[2:]
                             measurements = []
                     else:
-                        message("->", line)
+                        print("->", line)
 
                 line = fin.readline()  # advance to the next line
 
             # storing the last data into the dataset
-            message("Storing Measurement %s" % dataname)
+            if dataname:
+                print("Storing Measurement %s (count %d)" % (dataname, len(measurements)))
             if len(measurements):
+                self.measure_count += len(measurements)
                 for k, title in enumerate(headers):
                     self.dataset[title] = [line[k] for line in measurements]
 
-            message("%d measurements" % len(self.dataset))
-            message("Identified %d steps, read %d measurements" % (self.step_count, self.measure_count))
+            print("%d measurements" % len(self.dataset))
+            print("Identified %d steps, read %d measurements" % (self.step_count, self.measure_count))
 
     def __getitem__(self, key):
         """
         __getitem__ implements
         :key: step or measurement name
         :return: step or measurement set
         :rtype: List[float]
@@ -581,15 +572,15 @@
         """
         Returns the names of the measurements read from the log file.
         :return: List of measurement names.
         :rtype: list of str
         """
         return self.dataset.keys()
 
-    def get_measure_value(self, measure: str, step: int = None) -> Union[float, int, str, complex]:
+    def get_measure_value(self, measure: str, step: int = None) -> Union[float, int, str, LTComplex]:
         """
         Returns a measure value on a given step.
 
         :param measure: name of the measurement to get
         :type measure: str
         :param step: optional step number if the simulation has no steps.
         :type step: int
@@ -631,25 +622,25 @@
                 self.dataset[param + '_ph'] = [v.ph for v in self.dataset[param]]
 
     def export_data(self, export_file: str, append_with_line_prefix=None):
         """
         Exports the measurement information to a tab separated value (.tsv) format. If step data is found, it is
         included in the exported file.
 
-        When using export data together with sim_batch.py classes, it may be helpful to append data to an existing
+        When using export data together with SpiceBatch.py classes, it may be helpful to append data to an existing
         file. For this purpose, the user can user the append_with_line_prefix argument to indicate that an append should
         be done. And in this case, the user must provide a string that will identify the LTSpice batch run.
 
         :param export_file: path to the file containing the information
         :type export_file: str
         :param append_with_line_prefix: user information to be written in the file in case an append is to be made.
         :type append_with_line_prefix: str
         :return: Nothing
         """
-        # message(tokens)
+        # print(tokens)
         if append_with_line_prefix is None:
             mode = 'w'  # rewrites the file
         else:
             mode = 'a'  # Appends an existing file
 
         if len(self.dataset) == 0:
             print("Empty data set. Exiting without writing file.")
@@ -680,70 +671,7 @@
                     for x in tok:
                         fout.write(f'\t{x}')
                 else:
                     fout.write(f'\t{tok}')
             fout.write('\n')
 
         fout.close()
-
-
-if __name__ == "__main__":
-
-    def valid_extension(filename):
-        return filename.endswith('.txt') or filename.endswith('.log') or filename.endswith('.mout')
-
-
-    if len(sys.argv) > 1:
-        filename = sys.argv[1]
-        if not valid_extension(filename):
-            print("Invalid extension in filename '%s'" % filename)
-            print("This tool only supports the following extensions :'.txt','.log','.mout'")
-            exit(-1)
-    else:
-        filename = None
-        newer_date = 0
-        for f in os.listdir():
-            date = os.path.getmtime(f)
-            if date > newer_date and valid_extension(f):
-                newer_date = date
-                filename = f
-    if filename is None:
-        print("File not found")
-        print("This tool only supports the following extensions :'.txt','.log','.mout'")
-        exit(-1)
-
-    fname_out = None
-    if filename.endswith('.txt'):
-        fname_out = filename[:-len('txt')] + 'tsv'
-    elif filename.endswith('.log'):
-        fname_out = filename[:-len('log')] + 'tlog'
-    elif filename.endswith('.mout'):
-        fname_out = filename[:-len('mout')] + 'tmout'
-    else:
-        print("Error in file type")
-        print("This tool only supports the following extensions :'.txt','.log','.mout'")
-        exit(-1)
-
-    if fname_out is not None:
-        print("Processing File %s" % filename)
-        print("Creating File %s" % fname_out)
-        if filename.endswith('txt'):
-            print("Processing Data File")
-            reformat_LTSpice_export(filename, fname_out)
-        elif filename.endswith("log"):
-            data = LTSpiceLogReader(filename)
-            data.split_complex_values_on_datasets()
-            data.export_data(fname_out)
-        elif filename.endswith(".mout"):
-            log_file = filename[:len('mout')] + 'log'
-            if os.path.exists(log_file):
-                steps = LTSpiceLogReader(log_file, read_measures=False)
-                data = LTSpiceLogReader(filename, step_set=steps.stepset)
-                data.stepset = steps.stepset
-            else:
-                # just reformats
-                data = LTSpiceLogReader(filename)
-            data.split_complex_values_on_datasets()
-            data.export_data(fname_out)
-            data.export_data(fname_out)
-
-    # input("Press Enter to Continue")
```

### Comparing `PyLTSpice-3.1/PyLTSpice/SemiDevOpReader.py` & `PyLTSpice-4.0/PyLTSpice/log/semi_dev_op_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # -------------------------------------------------------------------------------
 
 """
 Implements a parser for extracting Semiconductor Devices Operating Points from an LTSpice log file.
 """
 
 import re
-from .detect_encoding import detect_encoding
+from ..utils.detect_encoding import detect_encoding
 
 
 def opLogReader(filename: str) -> dict:
     """
     This function is exclusively dedicated to retrieving operation point parameters of Semiconductor Devices. This is
     handled separately from the main LogReader class because of its specialization and therefore not judged to be
     of interest to the typical LTSpice user making board level simulations.
```

### Comparing `PyLTSpice-3.1/PyLTSpice/SpiceEditor.py` & `PyLTSpice-4.0/PyLTSpice/sim/spice_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,36 +5,36 @@
 #    ____        _   _____ ____        _
 #   |  _ \ _   _| | |_   _/ ___| _ __ (_) ___ ___
 #   | |_) | | | | |   | | \___ \| '_ \| |/ __/ _ \
 #   |  __/| |_| | |___| |  ___) | |_) | | (_|  __/
 #   |_|    \__, |_____|_| |____/| .__/|_|\___\___|
 #          |___/                |_|
 #
-# Name:        SpiceEditor.py
+# Name:        spice_editor.py
 # Purpose:     Class made to update Generic Spice Netlists
 #
 # Author:      Nuno Brum (nuno.brum@gmail.com)
 #
-# Created:     30-08-2020
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
 import os
+from pathlib import Path
 import traceback
 import re
 import logging
 from math import log, floor
-from typing import Union, Optional, List
-from .detect_encoding import detect_encoding
+from typing import Union, List, Callable, Any
+from ..utils.detect_encoding import detect_encoding
 
 __author__ = "Nuno Canto Brum <nuno.brum@gmail.com>"
 __copyright__ = "Copyright 2021, Fribourg Switzerland"
 
 END_LINE_TERM = '\n'  #: This controls the end of line terminator used
 SUBCIRCUIT_DIVIDER = ':'  #: This controls the Subcircuit divider when setting component values inside subcircuits.
-                          # Ex: Editor.set_component
+                          # Ex: Editor.set_component_value('XU1:R1', '1k')
 
 # A Spice netlist can only have one of the instructions below, otherwise an error will be raised
 UNIQUE_SIMULATION_DOT_INSTRUCTIONS = ('.AC', '.DC', '.TRAN', '.NOISE', '.DC', '.TF')
 
 SPICE_DOT_INSTRUCTIONS = (
     '.BACKANNO',
     '.END',
@@ -66,15 +66,14 @@
 )
 
 REPLACE_REGXES = {
     'A': r"",  # Special Functions, Parameter substitution not supported
     'B': r"^(?P<designator>B§?[VI]?\w+)(?P<nodes>(\s+\S+){2})\s+(?P<value>.*)$",  # Behavioral source
     'C': r"^(?P<designator>C§?\w+)(?P<nodes>(\s+\S+){2})(?P<model>\s+\w+)?\s+(?P<value>({)?(?(6).*}|([0-9\.E+-]+(Meg|[kmuµnpf])?F?))).*$",  # Capacitor
     'D': r"^(?P<designator>D§?\w+)(?P<nodes>(\s+\S+){2})\s+(?P<value>\w+).*$",  # Diode
-    'I': r"^(?P<designator>I§?\w+)(?P<nodes>(\s+\S+){2})\s+(?P<value>.*)$",  # Current Source
     'E': r"^(?P<designator>E§?\w+)(?P<nodes>(\s+\S+){2,4})\s+(?P<value>.*)$",  # Voltage Dependent Voltage Source
                                                         # this only supports changing gain values
     'F': r"^(?P<designator>F§?\w+)(?P<nodes>(\s+\S+){2})\s+(?P<value>.*)$",  # Current Dependent Current Source
                                                         # This implementation replaces everything after the 2 first nets
     'G': r"^(?P<designator>G§?\w+)(?P<nodes>(\s+\S+){2,4})\s+(?P<value>.*)$",  # Voltage Dependent Current Source
                                                         # This only supports changing gain values
     'H': r"^(?P<designator>H§?\w+)(?P<nodes>(\s+\S+){2})\s+(?P<value>.*)$",  # Voltage Dependent Current Source
@@ -91,29 +90,32 @@
     'S': r"^(?P<designator>S§?\w+)(?P<nodes>(\s+\S+){4})\s+(?P<value>.*)$",  # Voltage Controlled Switch
     'T': r"^(?P<designator>T§?\w+)(?P<nodes>(\s+\S+){4})\s+(?P<value>.*)$",  # Lossless Transmission
     'U': r"^(?P<designator>U§?\w+)(?P<nodes>(\s+\S+){3})\s+(?P<value>.*)$",  # Uniform RC-line
     'V': r"^(?P<designator>V§?\w+)(?P<nodes>(\s+\S+){2})\s+(?P<value>.*)$",  # Voltage Source
                                                         # This implementation replaces everything after the 2 first nets
     'W': r"^(?P<designator>W§?\w+)(?P<nodes>(\s+\S+){2})\s+(?P<value>.*)$",  # Current Controlled Switch
                                                         # This implementation replaces everything after the 2 first nets
-    'X': r"^(?P<designator>X§?\w+)(?P<nodes>(\s+\S+){1,99}?)\s+(?P<value>\w+)(\s+params:)?(?P<params>(\s+\w+\s*=\s*[\d\w{}()\-\+\*/]+)*)\s*\\?$",  # Sub-circuit, Parameter substitution not supported
+    'X': r"^(?P<designator>X§?\w+)(?P<nodes>(\s+\S+){1,99}?)\s+(?P<value>\w+)(\s+params:)?(?P<params>(\s+\w+\s*=\s*[\d\w\{\}\(\)\-\+\*/]+)*)\s*\\?$",  # Sub-circuit, Parameter substitution not supported
     'Z': r"^(?P<designator>Z§?\w+)(?P<nodes>(\s+\S+){3})\s+(?P<value>\w+).*$",  # MESFET and IBGT. TODO: Parameters substitution not supported
+    '@': r"^(?P<designator>@§?\d+)(?P<nodes>(\s+\S+){2})\s?(?P<params>(.*)*)$",  # Frequency Noise Analysis (FRA) wiggler
+    # pattern = r'^@(\d+)\s+(\w+)\s+(\w+)(?:\s+delay=(\d+\w+))?(?:\s+fstart=(\d+\w+))?(?:\s+fend=(\d+\w+))?(?:\s+oct=(\d+))?(?:\s+fcoarse=(\d+\w+))?(?:\s+nmax=(\d+\w+))?\s+(\d+)\s+(\d+\w+)\s+(\d+)(?:\s+pp0=(\d+\.\d+))?(?:\s+pp1=(\d+\.\d+))?(?:\s+f0=(\d+\w+))?(?:\s+f1=(\d+\w+))?(?:\s+tavgmin=(\d+\w+))?(?:\s+tsettle=(\d+\w+))?(?:\s+acmag=(\d+))?$'
 }
 
 
 PARAM_REGEX = r"(?<= )(?P<replace>%s(\s*=\s*)(?P<value>[\w\*\/\.\+\-\/\*\{\}\(\)\t ]*))(?<!\s)($|\s+)(?!\s*=)"
 SUBCKT_CLAUSE_FIND = r"^.SUBCKT\s+"
 
 # Code Optimization objects, avoiding repeated compilation of regular expressions
 component_replace_regexs = {prefix: re.compile(pattern, re.IGNORECASE) for prefix, pattern in REPLACE_REGXES.items()}
 subcircuit_regex = re.compile(r"^.SUBCKT\s+(?P<name>\w+)", re.IGNORECASE)
 lib_inc_regex = re.compile(r"^\.(LIB|INC)\s+(.*)$", re.IGNORECASE)
 
 LibSearchPaths = []
 
+
 def format_eng(value) -> str:
     """
     Helper function for formating value with the SI qualifiers.  That is, it will use
 
         * p for pico (10E-12)
         * n for nano (10E-9)
         * u for micro (10E-6)
@@ -241,33 +243,43 @@
     cmd = get_line_command(instruction)
     return cmd in UNIQUE_SIMULATION_DOT_INSTRUCTIONS
 
 
 class ComponentNotFoundError(Exception):
     """Component Not Found Error"""
 
+
 class ParameterNotFoundError(Exception):
     """ParameterNotFound Error"""
     def __init__(self, parameter):
         super().__init__(f'Parameter "{parameter}" not found')
 
+
 class UnrecognizedSyntaxError(Exception):
     """Line doesn't match expected Spice syntax"""
     def __init__(self, line, regex):
         super().__init__(f'Line: "{line}" doesn\'t match regular expression "{regex}"')
 
 
+class MissingExpectedClauseError(Exception):
+    """Missing expected clause in Spice netlist"""
+
+
+
 class SpiceCircuit(object):
     """
     The Spice Circuit represents subcircuits within a SPICE circuit and since subcircuits can have subcircuits inside
-    them, it serves as base for the top level netlist.
-    This hierchical approach helps to encapsulate and protect parameters and components from a edits made a a higher
+    them, it serves as base for the top level netlist. See class SpiceEditor
+    This hierarchical approach helps to encapsulate and protect parameters and components from edits made at a higher
     level.
-    The information is stored in a python list, each line of the SPICE netlist is an item of the list. A Subcircuit
-    is represented as a SpiceCircuit object.
+
+    The netlist information is stored in a list, each element of the list corresponds to a SPICE instruction.
+    If an instruction spawns more than a line with the '+' operator, it is contained in the same element.
+
+    This class serves as subclass to the SpiceEditor class.
     """
 
     def __init__(self):
         self.subcircuits = {}
         self.netlist = []
         self.logger = logging.getLogger("SpiceCircuit")
 
@@ -334,15 +346,15 @@
             if cmd == command:
                 match = search_expression.search(line)
                 if match:
                     return line_no, match
             line_no += 1
         return -1, None  # If it fails, it returns an invalid line number and No match
 
-    def _get_subcircuit(self, instance_name: str) -> 'SubCircuit':
+    def _get_subcircuit(self, instance_name: str) -> 'SpiceCircuit':
         """Internal function. Do not use."""
         global LibSearchPaths
         if SUBCIRCUIT_DIVIDER in instance_name:
             subcircuit_ref, sub_subcircuits = instance_name.split(SUBCIRCUIT_DIVIDER, 1)
         else:
             subcircuit_ref = instance_name
 
@@ -398,15 +410,14 @@
                 return sub_circuit._get_subcircuit(sub_subcircuits)
             else:
                 return sub_circuit
         else:
             # The search was not successful
             raise ComponentNotFoundError(f'Subcircuit "{subcircuit_name}" not found')
 
-
     def _set_model_and_value(self, component, value):
         """Internal function. Do not use."""
         prefix = component[0]  # Using the first letter of the component to identify what is it
         regex = component_replace_regexs.get(prefix, None)  # Obtain RegX to make the update
 
         if regex is None:
             print("Component must start with one of these letters:\n", ','.join(REPLACE_REGXES.keys()))
@@ -442,15 +453,20 @@
         clone.netlist.insert(0, "***** SpiceEditor Manipulated this subcircuit ****" + END_LINE_TERM)
         clone.netlist.append("***** ENDS SpiceEditor ****" + END_LINE_TERM)
         new_name = kwargs.get('new_name', None)
         if new_name:  # If it is different from None
             clone.setname(new_name)
         return clone
 
-    def name(self):
+    def name(self) -> str:
+        """
+        Returns the name of the Sub-Circuit -> str.
+
+        :rtype: str
+        """
         if len(self.netlist):
             for line in self.netlist:
                 m = subcircuit_regex.search(line)
                 if m:
                     return m.group('name')
             else:
                 raise RuntimeError("Unable to find .SUBCKT clause in subcircuit")
@@ -477,25 +493,25 @@
                     # Replacing the name in the SUBCKT Clause
                     start = m.start('name')
                     end = m.end('name')
                     self.netlist[line_no] = line[:start] + new_name + line[end:]
                     break
                 line_no += 1
             else:
-                raise UnrecognizedSyntaxError("Unable to find .SUBCKT clause in subcircuit")
+                raise MissingExpectedClauseError("Unable to find .SUBCKT clause in subcircuit")
 
             # This second loop finds the .ENDS clause
             while line_no < lines:
                 line = self.netlist[line_no]
                 if get_line_command(line) == '.ENDS':
                     self.netlist[line_no] = '.ENDS ' + new_name + END_LINE_TERM
                     break
                 line_no += 1
             else:
-                raise UnrecognizedSyntaxError("Unable to find .SUBCKT clause in subcircuit")
+                raise MissingExpectedClauseError("Unable to find .SUBCKT clause in subcircuit")
         else:
             # Avoiding exception by creating an empty subcircuit
             self.netlist.app("* SpiceEditor Created this subcircuit")
             self.netlist.append('.SUBCKT %s%s' % (new_name, END_LINE_TERM))
             self.netlist.append('.ENDS %s%s' % (new_name, END_LINE_TERM))
         
     def get_component_info(self, component) -> dict:
@@ -519,15 +535,15 @@
 
         line_no = self._getline_startingwith(component)
         line = self.netlist[line_no]
         m = regex.match(line)
         if m is None:
             error_msg = 'Unsupported line "{}"\nExpected format is "{}"'.format(line, REPLACE_REGXES[prefix])
             self.logger.error(error_msg)
-            raise UnrecognizedSyntaxError(error_msg)
+            raise UnrecognizedSyntaxError(line, REPLACE_REGXES[prefix])
 
         info = m.groupdict()
         info['line'] = line_no  # adding the line number to the component information
         return info
 
     def get_parameter(self, param: str) -> str:
         """
@@ -793,31 +809,37 @@
                 if match:
                     nodes = match.group('nodes').split()  # This separates by all space characters including \t
                     for node in nodes:
                         if node not in circuit_nodes:
                             circuit_nodes.append(node)
         return circuit_nodes
 
+
 class SpiceEditor(SpiceCircuit):
     """
     This class implements interfaces to manipulate SPICE netlist files. The class doesn't update the netlist file
     itself. After implementing the modifications the user should call the "write_netlist" method to write a new
     netlist file.
+
     :param netlist_file: Name of the .NET file to parse
-    :type netlist_file: str
+    :type netlist_file: str or Path
     :param encoding: Forcing the encoding to be used on the circuit netlile read. Defaults to 'autodetect' which will
-    call a function that tries to detect the encoding automatically. This however is not 100% fool proof.
+        call a function that tries to detect the encoding automatically. This however is not 100% fool proof.
     :type encoding: str, optional
     """
-    def __init__(self, netlist_file, encoding='autodetect'):
+    def __init__(self, netlist_file: Union[str, Path], encoding='autodetect'):
         super().__init__()
-        self.netlist_file = netlist_file
+        self.netlist_file = Path(netlist_file)
+        if self.netlist_file.suffix == '.asc':
+            from .ltspice_simulator import LTspice
+
+            self.netlist_file = LTspice.create_netlist(self.netlist_file)
         self.modified_subcircuits = {}
         if encoding == 'autodetect':
-            self.encoding = detect_encoding(netlist_file, '*')  # Normally the file will start with a '*'
+            self.encoding = detect_encoding(self.netlist_file, '*')  # Normally the file will start with a '*'
         else:
             self.encoding = encoding
         self.reset_netlist()
 
     def _set_model_and_value(self, component, value):
         prefix = component[0]  # Using the first letter of the component to identify what is it
         if prefix == 'X' and SUBCIRCUIT_DIVIDER in component:  # Relaces a component inside of a subciruit
@@ -880,99 +902,105 @@
             # Insert before backanno instruction
             try:
                 line = self.netlist.index('.backanno\n')  # TODO: Improve this. END of line termination could be differnt and case as well
             except ValueError:
                 line = len(self.netlist) - 2  # This is where typically the .backanno instruction is
             self.netlist.insert(line, instruction)
 
-    def add_instructions(self, *instructions)->None:
+    def add_instructions(self, *instructions) -> None:
         """Adds a list of instructions to the SPICE NETLIST.
         Example:
         ::
 
             LTC.add_instructions(
                 ".STEP run -1 1023 1",
                 ".dc V1 -5 5"
             )
 
         :param instructions: Argument list of instructions to add
-        :type instructions: list
+        :type instructions: argument list
         :returns: Nothing
         """
         for instruction in instructions:
             self.add_instruction(instruction)
 
     def remove_instruction(self, instruction)->None:
         """Usage a previously added instructions.
         Example: ::
 
             LTC.remove_instruction(".STEP run -1 1023 1")
 
-        :param instructions The list of instructions to remove. Each instruction is of the type 'str'
+        This only works if the instruction exactly matches the line on the netlist. This means that space characters,
+        and upper case and lower case differences will not match the line.
+
+        :param instruction: The list of instructions to remove. Each instruction is of the type 'str'
         :type instruction: str
         :returns: Nothing
-        TODO: This only works with a full line instruction. Make it more inteligent so it recognizes .models, .param
-        and .subckt
         """
+        # TODO: Make it more inteligent so it recognizes .models, .param
+        #  and .subckt
         # Because the netlist is stored containing the end of line terminations and because they are added when they
         # they are added to the netlist.
         if not instruction.endswith(END_LINE_TERM):
             instruction += END_LINE_TERM
 
         self.netlist.remove(instruction)
 
-    def write_netlist(self, run_netlist_file: str)->None:
+    def write_netlist(self, run_netlist_file: 'Path') -> None:
         """
         Writes the netlist will all the requested updates into a file named <run_netlist_file>.
+
         :param run_netlist_file: File name of the netlist file.
-        :type run_netlist_file: str
-        :return Nothing
+        :type run_netlist_file: Path
+        :returns: Nothing
         """
-        f = open(run_netlist_file, 'w', encoding=self.encoding)
-        lines = iter(self.netlist)
-        for line in lines:
-            if isinstance(line, SpiceCircuit):
-                line._write_lines(f)
-            else:
-                # Writes the modified subcircuits at the end just before the .END clause
-                if line.upper().startswith(".END"):
-                    # write here the modified subcircuits
-                    for sub in self.modified_subcircuits.values():
-                        sub._write_lines(f)
-                f.write(line)
-        f.close()
+        with run_netlist_file.open('w', encoding=self.encoding) as f:
+            lines = iter(self.netlist)
+            for line in lines:
+                if isinstance(line, SpiceCircuit):
+                    line._write_lines(f)
+                else:
+                    # Writes the modified subcircuits at the end just before the .END clause
+                    if line.upper().startswith(".END"):
+                        # write here the modified subcircuits
+                        for sub in self.modified_subcircuits.values():
+                            sub._write_lines(f)
+                    f.write(line)
 
     def reset_netlist(self) -> None:
         """
         Removes all previous edits done to the netlist, i.e. resets it to the original state.
 
         :returns: Nothing
         """
         self.netlist.clear()
         self.modified_subcircuits.clear()
-        if os.path.exists(self.netlist_file):
-            with open(self.netlist_file, 'r', encoding=self.encoding, errors='replace') as f:
+        if self.netlist_file.exists():
+            with self.netlist_file.open('r', encoding=self.encoding, errors='replace') as f:
                 lines = iter(f)  # Creates an iterator object to consume the file
                 finished = self._add_lines(lines)
                 if not finished:
                     raise SyntaxError("Netlist with missing .END or .ENDS statements")
                 else:
                     for remainig_lines in lines:
                         print("Ignoring %s" % remainig_lines)
         else:
             self.logger.error("Netlist file not found")
 
     @staticmethod
-    def find_subckt_in_lib(library, subckt_name) -> 'SpiceEditor':
+    def find_subckt_in_lib(library, subckt_name) -> Union['SpiceCircuit', None]:
         """
-        Finds returns a Subckt from a library file
+        Finds returns a Subckt from a library file.
 
         :param library: path to the library to search
         :type library: str
         :param subckt_name: Subcircuit to search for
+        :type subckt_name: str
+        :return: Returns a SpiceCircuit instance with the subcircuit found or None if not found
+        :rtype: SpiceCircuit
         """
         # 0. Setup things
         reg_subckt = re.compile(SUBCKT_CLAUSE_FIND + subckt_name, re.IGNORECASE)
         # 1. Find Encoding
         encoding = detect_encoding(library)
         #  2. scan the file
         with open(library, encoding=encoding) as lib:
@@ -981,17 +1009,29 @@
                 if search:
                     sub_circuit = SpiceCircuit()
                     sub_circuit.netlist.append(line)
                     # Advance to the next non nested .ENDS
                     finished = sub_circuit._add_lines(lib)
                     if finished:
                         return sub_circuit
-        #  3. Return an instance of SpiceEditor
+        #  3. Return an instance of SpiceCircuit
         return None
 
+    def run(self, wait_resource: bool = True,
+            callback: Callable[[str, str], Any] = None, timeout: float = 600, run_filename: str = None, simulator=None):
+        """
+        *(Deprecated)*
+
+        Convenience function for maintaining legacy with legacy code.
+        """
+        from .sim_runner import SimRunner
+        Sim = SimRunner()
+        return Sim.run(self, wait_resource=wait_resource, callback=callback, timeout=timeout, run_filename=run_filename)
+
+
 if __name__ == '__main__':
     E = SpiceEditor(os.path.abspath('..\\tests\\PI_Filter_resampled.net'))
     E.add_instruction(".nodeset V(N001)=0")
     E.write_netlist('..\\tests\\PI_Filter_resampled_mod.net')
     E = SpiceEditor('..\\tests\\Editor_Test.net')
     print("Circuit Nodes", E.get_all_nodes())
     E.add_library_search_paths([r"C:\SVN\Electronic_Libraries\LTSpice\lib"])
```

### Comparing `PyLTSpice-3.1/PyLTSpice/detect_encoding.py` & `PyLTSpice-4.0/PyLTSpice/utils/detect_encoding.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# coding=utf-8
 #!/usr/bin/env python
+# coding=utf-8
 
 # -------------------------------------------------------------------------------
 #    ____        _   _____ ____        _
 #   |  _ \ _   _| | |_   _/ ___| _ __ (_) ___ ___
 #   | |_) | | | | |   | | \___ \| '_ \| |/ __/ _ \
 #   |  __/| |_| | |___| |  ___) | |_) | | (_|  __/
 #   |_|    \__, |_____|_| |____/| .__/|_|\___\___|
@@ -22,15 +22,15 @@
 Not using other known unicode detection libraries because we don't need something so complicated. LTSpice only supports
 for the time being a reduced set of encodings.
 """
 from pathlib import Path
 from typing import Union
 
 
-def detect_encoding(file_path, expected_str: Union[str, Path] = '') -> str:
+def detect_encoding(file_path: Union[str, Path], expected_str: str = '') -> str:
     """
     Simple strategy to detect file encoding.  If an expected_str is given the function will scan through the possible
     encodings and return a match.
     If an expected string is not given, it will use the second character is null, high chances are that this file has an
     'utf_16_le' encoding, otherwise it is assuming that it is 'utf-8'.
     :param file_path: path to the filename
     :type file_path: str
@@ -53,8 +53,11 @@
                     # File did not start with expected string
                     # Try again with a different encoding (This is unlikely to resolve the issue)
                     continue
             if encoding == 'utf-8' and lines[0][1] == '\x00':
                 continue
             return encoding
     else:
-        raise UnicodeError(f"Unable to detect log file encoding, or expected string ""{expected_str}"" not found")
+        if expected_str:
+            raise UnicodeError(f"Expected string \"{expected_str}\" not found in file:{file_path}")
+        else:
+            raise UnicodeError(f"Unable to detect log file encoding")
```

### Comparing `PyLTSpice-3.1/PyLTSpice/raw_classes.py` & `PyLTSpice-4.0/PyLTSpice/raw/raw_classes.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,24 +13,26 @@
 # Purpose:     Implements helper classes that contain
 #
 # Author:      Nuno Brum (nuno.brum@gmail.com)
 #
 # Created:     19-06-2022
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
-
+"""
+Defines base classes for the RAW file data structures.
+"""
 import numpy as np
 from numpy import zeros, complex128, float32, float64
 from binascii import b2a_hex
 from typing import Union, List
 
 
 class DataSet(object):
     """
-    This is the base class for storing all traces inside of a RAW file. Returned by the get_trace() or by the get_axis()
+    This is the base class for storing all traces of a RAW file. Returned by the get_trace() or by the get_axis()
     methods.
     Normally the user doesn't have to be aware of this class. It is only used internally to encapsulate the different
     implementations of the wave population.
     Data can be retrieved directly by using the [] operator.
     If numpy is available, the numpy vector can be retrieved by using the get_wave() method.
     The parameter whattype defines what is the trace representing in the simulation, Voltage, Current a Time or
     Frequency.
@@ -60,18 +62,24 @@
         else:
             data = [b2a_hex(value) for value in self.data]
             return "name:'%s'\ntype:'%s'\nlen:%d\n%s" % (self.name, self.whattype, len(self.data), str(data))
 
     def __len__(self):
         return len(self.data)
 
-    def get_wave(self):
+    def __iter__(self):
+        return iter(self.data)
+
+    def __getitem__(self, item):
+        return self.data[item]
+
+    def get_wave(self) -> np.array:
         """
         :return: Internal data array
-        :rtype: list or numpy.array
+        :rtype: numpy.array
         """
         return self.data
 
 
 class Axis(DataSet):
     """This class is used to represent the horizontal axis like on a Transient or DC Sweep Simulation. It derives from
     the DataSet and defines additional methods that are specific for X axis.
@@ -102,15 +110,15 @@
                 # print(k, i, self.data[i], self.data[i+1])
                 self.step_offsets[k] = i
                 k += 1
             i += 1
 
         if k != len(self.step_info):
             raise SpiceReadException("The file a different number of steps than expected.\n" +
-                                       "Expecting %d got %d" % (len(self.step_offsets), k))
+                                     "Expecting %d got %d" % (len(self.step_offsets), k))
 
     def step_offset(self, step: int):
         """
         In Stepped RAW files, several simulations runs are stored in the same RAW file. This function returns the
         offset within the binary stream where each step starts.
 
         :param step: Number of the step within the RAW file
@@ -125,65 +133,68 @@
                 return 0
         else:
             if step >= len(self.step_offsets):
                 return len(self.data)
             else:
                 return self.step_offsets[step]
 
-    def get_wave(self, step: int = 0):
+    def get_wave(self, step: int = 0) -> np.array:
         """
-        Returns an the vector containing the wave values. If numpy is installed, data is returned as a numpy array.
+        Returns a vector containing the wave values. If numpy is installed, data is returned as a numpy array.
         If not, the wave is returned as a list of floats.
 
         If stepped data is present in the array, the user should specify which step is to be returned. Failing to do so,
         will return all available steps concatenated together.
 
         :param step: Optional step in stepped data raw files.
         :type step: int
         :return: The trace values
-        :rtype: list[float] or numpy.array
+        :rtype: numpy.array
         """
-        # print(self.data)
-        # print('step offset %d' % self.step_offset(step))
-        # print(self.data[self.step_offset(step):self.step_offset(step + 1)])
         if step == 0:
-            return self.data[:self.step_offset(1)]
+            wave = self.data[:self.step_offset(1)]
+        else:
+            wave = self.data[self.step_offset(step):self.step_offset(step + 1)]
+        if self.name == 'time':  # This is a bug in LTSpice, where the time axis values are sometimes negative
+            return np.abs(wave)
         else:
-            return self.data[self.step_offset(step):self.step_offset(step + 1)]
+            return wave
 
     def get_time_axis(self, step: int = 0):
         """
+        **Deprecated**. Use get_wave() instead.
+
         Returns the time axis raw data. Please note that the time axis may not have a constant time step. LTSpice will
         increase the time-step in simulation phases where there aren't value changes, and decrease time step in
         the parts where more time accuracy is needed.
 
         :param step: Optional step number if reading a raw file with stepped data.
         :type step: int
         :return: time axis
-        :rtype: list[float] or numpy.array
+        :rtype: numpy.array
         """
         assert self.name == 'time', \
             "This function is only applicable to transient analysis, where a bug exists on the time signal"
-        return np.abs(self.get_wave(step))
+        return self.get_wave(step)
 
-    def get_point(self, n, step: int = 0):
+    def get_point(self, n, step: int = 0) -> Union[float, complex]:
         """
         Get a point from the dataset
         :param n: position on the vector
         :type n:int
         :param step: step index
         :type step: int
         :returns: Value of the data point
         :rtype: float or complex
         """
         return self.data[n + self.step_offset(step)]
 
-    def __getitem__(self, item):
+    def __getitem__(self, item) -> Union[float, complex]:
         """This is only here for compatibility with previous code. """
-        assert self.step_info is None, "Indexing should not be used with stepped data. Use get_point"
+        assert self.step_info is None, "Indexing should not be used with stepped data. Use get_point or get_wave"
         return self.data.__getitem__(item)
 
     def get_position(self, t, step: int = 0) -> Union[int, float]:
         """
         Returns the position of a point in the axis. If the point doesn't exist, an interpolation is done between the
         two closest points.
         For example, if the point requested is 1.0001ms and the closest points that exist in the axis are t[100]=1ms and
@@ -222,28 +233,32 @@
 
     def __len__(self):
         if self.step_info is None:
             return len(self.data)
         else:
             return self.get_len()
 
+    def __iter__(self):
+        assert self.step_info is None, "Iteration can't be used with stepped data. Use get_wave() method."
+        return self.data.__iter__()
+
 
-class Trace(DataSet):
+class TraceRead(DataSet):
     """This class is used to represent a trace. It derives from DataSet and implements the additional methods to
     support STEPed simulations.
     This class is constructed by the get_trace() command.
     Data can be accessed through the [] and len() operators, or by the get_wave() method.
     If numpy is available the get_wave() method will return a numpy array.
     """
 
     def __init__(self, name, whattype, datalen, axis, numerical_type='real'):
         super().__init__(name, whattype, datalen, numerical_type)
         self.axis = axis
 
-    def get_point(self, n: int, step: int = 0):
+    def get_point(self, n: int, step: int = 0) -> Union[float, complex]:
         """
         Implementation of the [] operator.
 
         :param n: item in the array
         :type n: int
         :param step: Optional step number
         :type step: int
@@ -254,44 +269,44 @@
             if n != 0:
                 return self.data[n]
             else:
                 return self.data[step]  # This is for the case of stepped operation point simulation.
         else:
             return self.data[self.axis.step_offset(step) + n]
 
-    def __getitem__(self, item):
+    def __getitem__(self, item) -> Union[float, complex]:
         """This is only here for compatibility with previous code. """
         assert self.axis is None or self.axis.step_info is None, \
             "Indexing should not be used with stepped data. Use get_point() method"
         return self.data.__getitem__(item)
 
-    def get_wave(self, step: int = 0):
+    def get_wave(self, step: int = 0) -> np.array:
         """
         Returns the data contained in this object. For stepped simulations an argument must be passed specifying the
         step number. If no steps exist, the argument must be left blank.
         To know whether stepped data exist, the user can use the get_raw_property('Flags') method.
 
         If numpy is available the get_wave() method will return a numpy array.
 
         :param step: To be used when stepped data exist on the RAW file.
         :type step: int
         :return: a List or numpy array (if installed) containing the data contained in this object.
-        :rtype: list or numpy.array
+        :rtype: numpy.array
         """
         # print('step size %d' % step)
         # print(self.data[self.axis.step_offset(step):self.axis.step_offset(step + 1)])
         if self.axis is None:
             return super().get_wave()
         else:
             if step == 0:
                 return self.data[:self.axis.step_offset(1)]
             else:
                 return self.data[self.axis.step_offset(step):self.axis.step_offset(step + 1)]
 
-    def get_point_at(self, t, step: int = 0):
+    def get_point_at(self, t, step: int = 0) -> Union[float, complex]:
         """
         Get a point from the trace at the point specified by the /t/ argument.
         If the point doesn't exist on the axis, the data is interpolated using a linear regression between the two
         adjacent points.
         :param t: point in the axis where to find the point.
         :type t: float, float32(numpy) or float64(numpy)
         :param step: step index
@@ -319,15 +334,18 @@
         :type step: int
         :return: The number of data points
         :rtype: int
         """
         return self.axis.step_offset(step + 1)
 
     def __len__(self):
-        """This is only here for compatibility with previous code. """
+        """
+        **Deprecated**
+        This is only here for compatibility with previous code.
+        """
         assert self.axis is None or self.axis.step_info is None, \
             "len() should not be used with stepped data. Use get_len() method passing the step index"
         return len(self.data)
 
 
 class DummyTrace(object):
     """Dummy Trace for bypassing traces while reading"""
@@ -336,8 +354,9 @@
         """Base Class for both Axis and Trace Classes.
         Defines the common operations between both."""
         self.name = name
         self.whattype = whattype
 
 
 class SpiceReadException(Exception):
-    """Custom class for exception handling"""
+    """Custom class for exception handling"""
+    ...
```

### Comparing `PyLTSpice-3.1/PyLTSpice/raw_read.py` & `PyLTSpice-4.0/PyLTSpice/raw/raw_read.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,20 +6,19 @@
 #   |  _ \ _   _| | |_   _/ ___| _ __ (_) ___ ___
 #   | |_) | | | | |   | | \___ \| '_ \| |/ __/ _ \
 #   |  __/| |_| | |___| |  ___) | |_) | | (_|  __/
 #   |_|    \__, |_____|_| |____/| .__/|_|\___\___|
 #          |___/                |_|
 #
 # Name:        raw_read.py
-# Purpose:     Process LTSpice output files and align data for usage in a spread-
-#              sheet tool such as Excel, or Calc.
+# Purpose:     Process LTSpice output files and align data for usage in a spreadsheet
+#              tool such as Excel, or Calc.
 #
 # Author:      Nuno Brum (nuno.brum@gmail.com)
 #
-# Created:     19-06-2022
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
 
 """
 This module reads data from an LTSpice RAW file.
 The main class object is the RawRead which is initialized with the filename of the RAW file to be processed.
 The object wil read the file and construct a structure of objects which can be used to access the data inside the
@@ -48,16 +47,16 @@
                        * DC transfer characteristic
                        * AC Analysis
                        * Transient Analysis
                        * Noise Spectral Density - (V/Hz½ or A/Hz½)
                        * Transfer Function
 
    + Flags:          => Flags that are used in this plot. The simulation can have any combination of these flags.
-                      * "real" -> The traces in the raw file contain real values. As for exmple on a TRAN simulation.
-                      * "complex" -> Traces in the raw file contain complex values. As for exmple on an AC simulation.
+                      * "real" -> The traces in the raw file contain real values. As for example on a TRAN simulation.
+                      * "complex" -> Traces in the raw file contain complex values. As for example on an AC simulation.
                       * "forward" -> Tells whether the simulation has more than one point. DC transfer
                         characteristic, AC Analysis, Transient Analysis or Noise Spectral Density have the forward flag.
                         Operating Point and Transfer Function don't have this flag activated.
                       * "log" -> The preferred plot view of this data is logarithmic.
                       * "stepped" -> The simulation had .STEP primitives.
                       * "FastAccess" -> Order of the data is changed to speed up access. See Binary section for details.
 
@@ -73,16 +72,16 @@
 
    + Variables:      => a list of variable, one per line as described below
 
    + Binary:         => Start of the binary section. See section below for details.
 
 Variables List
 --------------
-The variable list contains the list of measurements saved in the raw file. The order of the variables defines how they are
-stored in the binary section. The format is one variable per line, using the following format:
+The variable list contains the list of measurements saved in the raw file. The order of the variables defines how they
+are stored in the binary section. The format is one variable per line, using the following format:
 
 <tab><ordinal number><tab><measurement><tab><type of measurement>
 
 Here is an example:
 
 .. code-block:: text
 
@@ -122,15 +121,15 @@
      <timestamp 2><trace1 2><trace2 2><trace3 2>...<traceN 2>
 
      ...
 
      <timestamp T><trace1 T><trace2 T><trace3 T>...<traceN T>
      
 Depending on the type of simulation the type of data changes.
-On TRAN simulations the timestamp is always stored as 8 bytes float (double) and trace values as a 4 bytes (single).
+On TRAN simulations the timestamp is always stored as 8 bytes float (double) and trace values as 4 bytes (single).
 On AC simulations the data is stored in complex format, which includes a real part and an imaginary part, each with 8
 bytes.
 The way we determine the size of the data is dividing the total block size by the number of points, then taking only
 the integer part.
 
 Fast Access
 -----------
@@ -177,18 +176,18 @@
     LTR = RawRead("some_random_file.raw")  # Reads the RAW file contents from file
 
     print(LTR.get_trace_names())  # Prints the contents of the RAW file. The result is a list, and print formats it.
     print(LTR.get_raw_property())  # Prints all the properties found in the Header section.
 
     plt.figure()  # Creates the canvas for plotting
 
-    vin = LTR.get_trace('V(in)')  # Get's the trace data. If Numpy is installed, then it comes in numpy array format.
-    vout = LTR.get_trace('V(out)') # Get's the second trace.
+    vin = LTR.get_trace('V(in)')  # Gets the trace data. If Numpy is installed, then it comes in numpy array format.
+    vout = LTR.get_trace('V(out)') # Gets the second trace.
 
-    steps = LTR.get_steps()  # Get's the step information. Returns a list of step numbers, ex: [0,1,2...]. If no steps
+    steps = LTR.get_steps()  # Gets the step information. Returns a list of step numbers, ex: [0,1,2...]. If no steps
                              # are present on the RAW file, returns only one step : [0] .
 
     fig, (ax1, ax2) = plt.subplots(2, 1, sharex=True)  # Creates the two subplots. One on top of the other.
 
     for ax in (ax1, ax2):  # Crates a grid on all the plots.
         ax.grid(True)
 
@@ -208,27 +207,27 @@
 __author__ = "Nuno Canto Brum <nuno.brum@gmail.com>"
 __copyright__ = "Copyright 2022, Fribourg Switzerland"
 
 import os
 
 from collections import OrderedDict
 from struct import unpack
-from typing import Union, List, Tuple
+from typing import Union, List, Tuple, Dict
 from pathlib import Path
 
-from .raw_classes import Axis, Trace, DummyTrace, SpiceReadException
-from .detect_encoding import detect_encoding
+from .raw_classes import Axis, TraceRead, DummyTrace, SpiceReadException
+from ..utils.detect_encoding import detect_encoding
 
 import numpy as np
 from numpy import zeros, complex128, float32, float64, frombuffer, angle
 
 
 def read_float64(f):
     """
-    Reads a 64 bit float value, normally associated with the plot X axis.
+    Reads a 64-bit float value, normally associated with the plot X axis.
     The codification is done as follows:
 
     =====  === === === ===   === === === ===
     bit#   7   6   5   4     3   2   1   0
     =====  === === === ===   === === === ===
     Byte7  SGM SGE E9  E8    E7  E6  E5  E4
     Byte6  E3  E2  E1  E0    M51 M50 M49 M48
@@ -353,14 +352,15 @@
     ACCEPTED_PLOTNAMES = (
         'AC Analysis',
         'DC transfer characteristic',
         'Operating Point',
         'Transient Analysis',
         'Transfer Function',
         'Noise Spectral Density',
+        'Frequency Response Analysis',
     )
 
     def __init__(self, raw_filename: str, traces_to_read: Union[str, List[str], Tuple[str], None] = '*', **kwargs):
         self.verbose = kwargs.get('verbose', True)
         raw_filename = Path(raw_filename)
         if traces_to_read is not None:
             assert isinstance(traces_to_read, (str, list, tuple)), "traces_to_read must be a string, a list or None"
@@ -376,21 +376,20 @@
         elif ch.decode(encoding='utf_16_le') == 'Tit':
             self.encoding = 'utf_16_le'
             sz_enc = 2
             line = 'Tit'
         else:
             raise RuntimeError("Unrecognized encoding")
         if self.verbose:
-            print("Reading file with encoding ", self.encoding)
+            print("Reading the file with encoding ", self.encoding)
         # Storing the filename as part of the dictionary
         self.raw_params = OrderedDict(Filename=raw_filename)  # Initializing the dict that contains all raw file info
         self.backannotations = []  # Storing backannotations
         header = []
         binary_start = 6
-        line = ""
         while True:
             ch = raw_file.read(sz_enc).decode(encoding=self.encoding)
             binary_start += sz_enc
             if ch == '\n':
                 if self.encoding == 'utf_8':  # must remove the \r
                     line = line.rstrip('\r')
                 header.append(line)
@@ -427,18 +426,18 @@
                     axis_numerical_type = 'double'
                 else:
                     axis_numerical_type = numerical_type
                 self.axis = Axis(name, var_type, self.nPoints, axis_numerical_type)
                 trace = self.axis
             elif (traces_to_read == "*") or (name in traces_to_read):
                 if has_axis:  # Reads data
-                    trace = Trace(name, var_type, self.nPoints, self.axis, numerical_type)
+                    trace = TraceRead(name, var_type, self.nPoints, self.axis, numerical_type)
                 else:
                     # If an Operation Point or Transfer Function, only one point per step
-                    trace = Trace(name, var_type, self.nPoints, None, 'real')
+                    trace = TraceRead(name, var_type, self.nPoints, None, 'real')
             else:
                 trace = DummyTrace(name, var_type)
 
             self._traces.append(trace)
             ivar += 1
 
         if traces_to_read is None or len(self._traces) == 0:
@@ -447,15 +446,17 @@
             return
 
         if kwargs.get("headeronly", False):
             raw_file.close()
             return
 
         if self.verbose:
-            print("File contains {} traces, reading {}".format(ivar, len(self._traces)))
+            print("File contains {} traces, reading {}".format(ivar,
+                                                               len([trace for trace in self._traces
+                                                                    if not isinstance(trace, DummyTrace)])))
 
         if self.raw_type == "Binary:":
             # Will start the reading of binary values
             # But first check whether how data is stored.
             self.block_size = (raw_file_size - binary_start) // self.nPoints
             self.data_size = self.block_size // self.nVariables
 
@@ -520,20 +521,20 @@
             # Will start the reading of ASCII Values
             for point in range(self.nPoints):
                 first_var = True
                 for var in self._traces:
                     line = raw_file.readline().decode(encoding=self.encoding, errors='ignore')
                     if first_var:
                         first_var = False
-                        spoint = line.split("\t", 1)[0]
+                        s_point = line.split("\t", 1)[0]
 
-                        if point != int(spoint):
+                        if point != int(s_point):
                             print("Error Reading File")
                             break
-                        value = line[len(spoint):-1]
+                        value = line[len(s_point):-1]
                     else:
                         value = line[:-1]
                     if not isinstance(var, DummyTrace):
                         var.data[point] = float(value)
         else:
             raw_file.close()
             raise SpiceReadException("Unsupported RAW File. ""%s""" % self.raw_type)
@@ -556,30 +557,30 @@
         if "stepped" in self.raw_params["Flags"]:
             try:
                 self._load_step_information(raw_filename)
             except SpiceReadException:
                 print("LOG file not found or problems happened while reading it. Auto-detecting steps")
                 if has_axis:
                     number_of_steps = 0
-                    for v in self.axis:
-                        if v == self.axis[0]:
+                    for v in self.axis.data:
+                        if v == self.axis.data[0]:
                             number_of_steps += 1
                 else:
                     number_of_steps = self.nPoints
-                self.steps = [{'run': i+1} for i in range(number_of_steps)]
+                self.steps = [{'run': i + 1} for i in range(number_of_steps)]
 
             if self.steps is not None:
                 if has_axis:
                     # Individual access to the Trace Classes, this information is stored in the Axis
                     # which is always in position 0
                     self._traces[0]._set_steps(self.steps)
 
     def get_raw_property(self, property_name=None):
         """
-        Get a property. By default it returns all properties defined in the RAW file.
+        Get a property. By default, it returns all properties defined in the RAW file.
 
         :param property_name: name of the property to retrieve.
         :type property_name: str
         :returns: Property object
         :rtype: str
         :raises: ValueError if the property doesn't exist
         """
@@ -588,15 +589,15 @@
         elif property_name in self.raw_params.keys():
             return self.raw_params[property_name]
         else:
             raise ValueError("Invalid property. Use %s" % str(self.raw_params.keys()))
 
     def get_trace_names(self):
         """
-        Returns a list of exiting trace names inside of the RAW file.
+        Returns a list of exiting trace names of the RAW file.
 
         :return: trace names
         :rtype: list[str]
         """
         return [trace.name for trace in self._traces]
 
     def get_trace(self, trace_ref: Union[str, int]):
@@ -607,15 +608,15 @@
         :type trace_ref: str or int
         :return: An object containing the requested trace
         :rtype: DataSet subclass
         :raises IndexError: When a trace is not found
         """
         if isinstance(trace_ref, str):
             for trace in self._traces:
-                if trace_ref.upper() == trace.name.upper():  # The trace names are case insensitive
+                if trace_ref.upper() == trace.name.upper():  # The trace names are case-insensitive
                     # assert isinstance(trace, DataSet)
                     return trace
             raise IndexError(f"{self} doesn't contain trace \"{trace_ref}\"\n"
                              f"Valid traces are {[trc.name for trc in self._traces]}")
         else:
             return self._traces[trace_ref]
 
@@ -650,30 +651,28 @@
         :param step: Step number
         :type step: int
         :returns: Array with the X axis
         :rtype: list[float] or numpy.array
         """
         if self.axis:
             axis = self.get_trace(0)
-            if axis.whattype == 'time':
-                return axis.get_time_axis(step)
-            else:
-                return axis.get_wave(step)
+            assert isinstance(axis, Axis), "This RAW file does not have an axis."
+            return axis.get_wave(step)
         else:
             raise RuntimeError("This RAW file does not have an axis.")
 
     def get_len(self, step: int = 0) -> int:
         """
         Returns the length of the data at the give step index.
         :param step: Optional parameter the step index.
         :type step: int
         :return: The number of data points
         :rtype: int
         """
-        return self.axis.get_len(step) 
+        return self.axis.get_len(step)
 
     def _load_step_information(self, filename: Path):
         # Find the extension of the file
         if not filename.suffix == ".raw":
             raise SpiceReadException("Invalid Filename. The file should end with '.raw'")
         logfile = filename.with_suffix(".log")
         try:
@@ -688,15 +687,15 @@
             if line.startswith(".step"):
                 step_dict = {}
                 for tok in line[6:-1].split(' '):
                     key, value = tok.split('=')
                     try:
                         # Tries to convert to float for backward compatibility
                         value = float(value)
-                    except:
+                    except ValueError:
                         pass
                         # Leave value as a string to accommodate cases like temperature steps.
                         # Temperature steps have the form '.step temp=25°C'
                     step_dict[key] = value
                 if self.steps is None:
                     self.steps = [step_dict]
                 else:
@@ -721,15 +720,15 @@
          key-value arguments in which the key correspond to a stepped parameter or source name, and the value is the
          stepped value.
 
         :return: The steps that match the query
         :rtype: list[int]
         """
         if self.steps is None:
-            return [0]  # returns an single step
+            return [0]  # returns a single step
         else:
             if len(kwargs) > 0:
                 ret_steps = []  # Initializing an empty array
                 i = 0
                 for step_dict in self.steps:
                     for key in kwargs:
                         ll = step_dict.get(key, None)
@@ -740,18 +739,251 @@
                     else:
                         ret_steps.append(i)  # All the step parameters match
                     i += 1
                 return ret_steps
             else:
                 return range(len(self.steps))  # Returns all the steps
 
+    def export(self, columns: list = None, step: Union[int, List[int]] = -1, **kwargs) -> Dict[str, list]:
+        """
+        Returns a native python class structure with the requested trace data and steps.
+        It consists of an ordered dictionary where the columns are the keys and the values are lists with the data.
+
+        This function is used by the export functions.
+
+        :param step: Step number to retrieve. If not given, it will return all steps
+        :type step: int
+        :param columns: List of traces to use as columns. Default is all traces
+        :type columns: list
+        :param kwargs: Additional arguments to pass to the pandas.DataFrame constructor
+        :type kwargs: **dict
+        :return: A pandas DataFrame
+        :rtype: pandas.DataFrame
+        """
+        if columns is None:
+            columns = self.get_trace_names()  # if no columns are given, use all traces
+        else:
+            if self.axis and self.axis.name not in columns:  # If axis is not in the list, add it
+                columns.insert(0, self.axis.name)
+
+        if isinstance(step, list):
+            steps_to_read = step  # If a list of steps is given, use it
+        elif step == -1:
+            steps_to_read = self.get_steps(**kwargs)  # If no step is given, read all steps
+        else:
+            steps_to_read = [step]  # If a single step is given, pass it as a list
+
+        step_columns = []
+        if len(step_columns) > 1:
+            for step_dict in self.steps[0]:
+                for key in step_dict:
+                    step_columns.append(key)
+        data = OrderedDict()
+        # Create the headers with the column names and empty lists
+        for col in columns:
+            data[col] = []
+        for col in step_columns:
+            data[col] = []
+        # Read the data
+        for step in steps_to_read:
+            for col in columns:
+                data[col] += list(self.get_wave(col, step))
+            for col in step_columns:
+                data[col] += [self.steps[step][col]] * len(data[columns[0]])
+        return data
+
+    def to_dataframe(self, columns: list = None, step: Union[int, List[int]] = -1, **kwargs):
+        """
+        Returns a pandas DataFrame with the requested data.
+
+        :param step: Step number to retrieve. If not given, it
+        :type step: int
+        :param columns: List of traces to use as columns. Default is all traces
+        :type columns: list
+        :param kwargs: Additional arguments to pass to the pandas.DataFrame constructor
+        :type kwargs: **dict
+        :return: A pandas DataFrame
+        :rtype: pandas.DataFrame
+        """
+        try:
+            import pandas as pd
+        except ImportError:
+            raise ImportError("The 'pandas' module is required to use this function.\n"
+                              "Use 'pip install pandas' to install it.")
+        data = self.export(columns=columns, step=step, **kwargs)
+        return pd.DataFrame(data, **kwargs)
+
+    def to_csv(self, filename: Union[str, Path], columns: list = None, step: Union[int, List[int]] = -1,
+               separator=',', **kwargs):
+        """
+        Saves the data to a CSV file.
+
+        :param filename: Name of the file to save the data to
+        :type filename: str
+        :param columns: List of traces to use as columns. Default is all traces
+        :type columns: list
+        :param step: Step number to retrieve. If not given, it
+        :type step: int
+        :param separator: separator to use in the CSV file
+        :type separator: str
+        :param kwargs: Additional arguments to pass to the pandas.DataFrame.to_csv function
+        :type kwargs: **dict
+        """
+        try:
+            import pandas as pd
+        except ImportError:
+            use_pandas = False
+        else:
+            use_pandas = True
+
+        if use_pandas:
+            df = self.to_dataframe(columns=columns, step=step)
+            df.to_csv(filename, sep=separator, **kwargs)
+        else:
+            # Export to CSV using python built-in functions
+            data = self.export(columns=columns, step=step)
+            with open(filename, 'w') as f:
+                f.write(separator.join(data.keys()) + '\n')
+                for i in range(len(data[columns[0]])):
+                    f.write(separator.join([str(data[col][i]) for col in data.keys()]) + '\n')
+
+    def to_excel(self, filename: Union[str, Path], columns: list = None, step: Union[int, List[int]] = -1,
+                 **kwargs):
+        """
+        Saves the data to an Excel file.
+        :param filename: Name of the file to save the data to
+        :type filename: str
+        :param columns: List of traces to use as columns. Default is all traces
+        :type columns: list
+        :param step: Step number to retrieve. If not given, it
+        :type step: int
+        :param kwargs: Additional arguments to pass to the pandas.DataFrame.to_excel function
+        :type kwargs: **dict
+        """
+        try:
+            import pandas as pd
+        except ImportError:
+            raise ImportError("The 'pandas' module is required to use this function.\n"
+                              "Use 'pip install pandas' to install it.")
+        df = self.to_dataframe(columns=columns, step=step)
+        df.to_excel(filename, **kwargs)
+
 
 # Backward compatibility naming
 LTSpiceRawRead = RawRead
 
-# if __name__ == "__main__":
+
+def main():
+    """Uses matplotlib to plot the data in the raw file"""
+    import sys
+    import matplotlib.pyplot as plt
+    import os
+    from os.path import split as path_split
+    from os.path import join as path_join
+    from numpy import abs as mag
+
+    def what_to_units(whattype):
+        """Determines the unit to display on the plot Y axis"""
+        if 'voltage' in whattype:
+            return 'V'
+        if 'current' in whattype:
+            return 'A'
+
+    directory = os.getcwd()
+
+    if len(sys.argv) > 1:
+        raw_filename = sys.argv[1]
+        trace_names = sys.argv[2:]
+        if len(trace_names) == 0:
+            trace_names = '*'
+    else:
+        test_directory = path_join(path_split(directory)[0], 'tests')
+        filename = 'DC sweep.raw'
+        # filename = 'tran.raw'
+        # filename = 'tran - step.raw'
+        # filename = 'ac.raw'
+        # filename = 'AC - STEP.raw'
+        # filename = 'PI_Filter_tf.raw'
+        # filename = 'DC op point - STEP_1.raw'
+        # filename = 'Noise.raw'
+        filename = "test2_gs_000.raw"
+        trace_names = ("run", "V(out)", "V(err)")
+        # trace_names = '*' # 'V(out)',
+        raw_filename = path_join(test_directory, filename)
+
+    LTR = RawRead(raw_filename, trace_names, verbose=True)
+    for param, value in LTR.raw_params.items():
+        print("{}: {}{}".format(param, " " * (20 - len(param)), str(value).strip()))
+
+    if trace_names == '*':
+        print("Reading all the traces in the raw file")
+        trace_names = LTR.get_trace_names()
+
+    traces = [LTR.get_trace(trace) for trace in trace_names]
+    if LTR.axis is not None:
+        steps_data = LTR.get_steps()
+    else:
+        steps_data = [0]
+    print("Steps read are :", list(steps_data))
+
+    if 'complex' in LTR.flags:
+        n_axis = len(traces) * 2
+    else:
+        n_axis = len(traces)
+
+    fig, axis_set = plt.subplots(n_axis, 1, sharex='all')
+    write_labels = True
+
+    for i, trace in enumerate(traces):
+        if 'complex' in LTR.flags:
+            axis_set = axis_set[2 * i: 2 * i + 2]  # Returns two axis
+        else:
+            if n_axis == 1:
+                axis_set = [axis_set]  # Needs to return a list
+            else:
+                axis_set = axis_set[i:i + 1]  # Returns just one axis but enclosed in a list
+        magnitude = True
+        for ax in axis_set:
+            ax.grid(True)
+            if 'log' in LTR.flags:
+                ax.set_xscale('log')
+            for step_i in steps_data:
+                if LTR.axis:
+                    x = LTR.get_axis(step_i)
+                else:
+                    x = np.arange(LTR.nPoints)
+                y = traces[i].get_wave(step_i)
+                if 'complex' in LTR.flags:
+                    x = mag(x)
+                    if magnitude:
+                        ax.set_yscale('log')
+                        y = mag(y)
+                    else:
+                        y = angle(y, deg=True)
+                if write_labels:
+                    ax.plot(x, y, label=str(steps_data[step_i]))
+                else:
+                    ax.plot(x, y)
+            write_labels = False
+
+            if 'complex' in LTR.flags:
+                if magnitude:
+                    title = f"{trace.name} Mag [db{what_to_units(trace.whattype)}]"
+                    magnitude = False
+                else:
+                    title = f"{trace.name} Phase [deg]"
+            else:
+                title = f"{trace.name} [{what_to_units(trace.whattype)}]"
+            ax.set_title(title)
+
+    plt.figlegend()
+    plt.show()
+'''
+'''
 # out = open("RAW_TEST_out_test1.txt", 'w')
 #
 # for step in LTR.get_steps():
 #     for x in range(len(LTR[0].data)):
 #         out.write("%s, %e, %e\n" % (step, LTR[0].data[x], LTR[2].data[x]))
 # out.close()
+if __name__ == "__main__":
+    main()
```

### Comparing `PyLTSpice-3.1/PyLTSpice/sim_analysis.py` & `PyLTSpice-4.0/PyLTSpice/sim/sim_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # Created:     23-12-2016
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
 
 from collections import OrderedDict
 from typing import Iterable
 from .sim_batch import SimCommander
-from .SpiceEditor import ComponentNotFoundError
+from .spice_editor import ComponentNotFoundError
 
 
 class SimAnalysis(object):
     """
     Base class for making Monte-Carlo, Extreme Value Analysis (EVA) or Failure Mode and Effects Analysis.
     As a base class, a certain number of assertions must be made on the simulation results that will make the pass/fail.
```

### Comparing `PyLTSpice-3.1/PyLTSpice/sim_batch.py` & `PyLTSpice-4.0/PyLTSpice/sim/sim_runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 #    ____        _   _____ ____        _
 #   |  _ \ _   _| | |_   _/ ___| _ __ (_) ___ ___
 #   | |_) | | | | |   | | \___ \| '_ \| |/ __/ _ \
 #   |  __/| |_| | |___| |  ___) | |_) | | (_|  __/
 #   |_|    \__, |_____|_| |____/| .__/|_|\___\___|
 #          |___/                |_|
 #
-# Name:        sim_batch.py
-# Purpose:     Tool used to launch LTSpice simulation in batch mode. Netlsts can
-#              be updated by user instructions
+# Name:        sim_runner.py
+# Purpose:     Tool used to launch LTSpice simulation in batch mode.
 #
 # Author:      Nuno Brum (nuno.brum@gmail.com)
 #
 # Created:     23-12-2016
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
 """
@@ -36,15 +35,15 @@
 
     LTC.wait_completion()  # Waits for the LTSpice simulations to complete
 
     print("Total Simulations: {}".format(LTC.runno))
     print("Successful Simulations: {}".format(LTC.okSim))
     print("Failed Simulations: {}".format(LTC.failSim))
 
-The first line will create an python class instance that represents the LTSpice file or netlist that is to be
+The first line will create a python class instance that represents the LTSpice file or netlist that is to be
 simulated. This object implements methods that are used to manipulate the spice netlist. For example, the method
 set_parameters() will set or update existing parameters defined in the netlist. The method set_component_value() is
 used to update existing component values or models.
 
 ---------------
 Multiprocessing
 ---------------
@@ -91,401 +90,446 @@
 
 The callback function is optional. If  no callback function is given, the thread is terminated just after the
 simulation is finished.
 """
 __author__ = "Nuno Canto Brum <nuno.brum@gmail.com>"
 __copyright__ = "Copyright 2020, Fribourg Switzerland"
 
+__all__ = ['SimRunner']
+
 import logging
 import os
-import pathlib
-import threading
-import time
-import traceback
-from time import sleep
-from typing import Callable, Union, Any, Tuple
-from warnings import warn
-
-from .SpiceEditor import SpiceEditor
-from .simulator import clock_function, Simulator
+import shutil
+from pathlib import Path
+from time import sleep, thread_time as clock
+
+from typing import Callable, Union, Any, Type
+
+from .process_callback import ProcessCallback
+from ..sim.run_task import RunTask
+from ..sim.simulator import Simulator
+from ..sim.spice_editor import SpiceEditor
 
 END_LINE_TERM = '\n'
 
-logging.basicConfig(filename='SpiceBatch.log', level=logging.INFO)
-
-
-
-
-class RunTask(threading.Thread):
-    """This is an internal Class and should not be used directly by the User."""
-
-    def __init__(self, simulator: Simulator,  run_no, netlist_file: str, callback: Callable[[str, str], Any], timeout=None, verbose=True):
-        self.verbose = verbose
-        self.timeout = timeout  # Thanks to Daniel Phili for implementing this
-
-        threading.Thread.__init__(self)
-        self.setName("sim%d" % run_no)
-        self.simulator = simulator
-        self.run_no = run_no
-        self.netlist_file = netlist_file
-        self.callback = callback
-        self.retcode = -1  # Signals an error by default
-        self.raw_file = None
-        self.log_file = None
-
-    def run(self):
-        # Setting up
-        logger = logging.getLogger("sim%d" % self.run_no)
-        logger.setLevel(logging.INFO)
-
-        # Running the Simulation
-
-        self.start_time = clock_function()
-        if self.verbose:
-            print(time.asctime(), ": Starting simulation %d" % self.run_no)
-
-        # start execution
-        self.retcode = self.simulator.run(self.netlist_file, self.timeout)
-
-        # print simulation time
-        sim_time = time.strftime("%H:%M:%S", time.gmtime(clock_function() - self.start_time))
-        netlist_radic, extension = os.path.splitext(self.netlist_file)
-        self.log_file = netlist_radic + '.log'
-
-        # Cleanup everything
-        if self.retcode == 0:
-            # simulation successful
-            logger.info("Simulation Successful. Time elapsed: %s" % sim_time)
-            if self.verbose:
-                print(time.asctime() + ": Simulation Successful. Time elapsed %s:%s" % (sim_time, END_LINE_TERM))
 
-            self.raw_file = netlist_radic + '.raw'
+# logging.basicConfig(filename='SpiceBatch.log', level=logging.INFO)
 
-            if os.path.exists(self.raw_file) and os.path.exists(self.log_file):
-                if self.callback:
-                    if self.verbose:
-                        print("Calling the callback function")
-                    try:
-                        self.callback(self.raw_file, self.log_file)
-                    except Exception as err:
-                        error = traceback.format_tb(err)
-                        logger.error(error)
-                else:
-                    if self.verbose:
-                        print('No Callback')
-            else:
-                logger.error("Simulation Raw file or Log file were not found")
-        else:
-            # simulation failed
 
-            logger.warning(time.asctime() + ": Simulation Failed. Time elapsed %s:%s" % (sim_time, END_LINE_TERM))
-            if os.path.exists(self.log_file):
-                old_log_file = self.log_file
-                self.log_file = netlist_radic + '.fail'
-                os.rename(old_log_file, self.log_file)
-
-    def wait_results(self) -> Tuple[str, str]:
-        """
-        Waits for the completion of the task and returns a tuple with the raw and log files.
-        :returns: Tupple with the path to the raw file and the path to the log file
-        :rtype: tuple(str, str)
-        """
-        while self.is_alive() or self.retcode == -1:
-            sleep(0.1)
-        if self.retcode == 0:  # All finished OK
-            return self.raw_file, self.log_file
-        else:
-            return '', ''
+class SimRunnerTimeoutError(TimeoutError):
+    """Timeout Error class"""
+    ...
 
 
-class SimCommander(SpiceEditor):
+class SimRunner(object):
     """
     The SimCommander class implements all the methods required for launching batches of LTSpice simulations.
     It takes a parameter the path to the LTSpice .asc file to be simulated, or directly the .net file.
     If an .asc file is given, the class will try to generate the respective .net file by calling LTspice with
     the --netlist option
+    :raises FileNotFoundError: When the file is not found  /!\\ This will be changed
 
-    :param circuit_file: Path to the circuit to simulate. It can be either a .asc or a .net file
-    :type circuit_file: str
     :param parallel_sims: Defines the number of parallel simulations that can be executed at the same time. Ideally this
                           number should be aligned to the number of CPUs (processor cores) available on the machine.
     :type parallel_sims: int, optional
     :param timeout: Timeout parameter as specified on the os subprocess.run() function
     :type timeout: float, optional
     :param verbose: If True, it enables a richer printout of the program execution.
     :type verbose: bool, optional
-    :param encoding: Forcing the encoding to be used on the circuit netlile read. Defaults to 'autodetect' which will
-                     call a function that tries to detect the encoding automatically. This however is not 100% fool
-                     proof.
-    :type encoding: str, optional
+    :param output_folder: specifying which directory shall be used for simulation files (raw and log files).
+    :param output_folder: str
     :param simulator: Forcing a given simulator executable.
     :type simulator: str or Simulator, optional
+
     """
 
-    def __init__(self, circuit_file: str, parallel_sims: int = 4, timeout=None, verbose=True, encoding='autodetect',
-                 simulator=None):
+    def __init__(self, parallel_sims: int = 4, timeout=None, verbose=True, output_folder: str = None, simulator=None):
         """
         Class Constructor. It serves to start batches of simulations.
         See Class documentation for more information.
         """
-
+        self.workfiles = []
         self.verbose = verbose
         self.timeout = timeout
+        self.cmdline_switches = []
 
-        self.file_path = os.path.dirname(circuit_file)
-        if self.file_path == '':
-            self.file_path = os.path.abspath(os.curdir)
-        self.file_name, file_ext = os.path.splitext(os.path.basename(circuit_file))
-        self.circuit_radic = os.path.join(self.file_path, self.file_name)
+        if output_folder:
+            self.output_folder = Path(output_folder)  # If not None converts to Path() object
+            if not self.output_folder.exists():
+                self.output_folder.mkdir()
+        else:
+            self.output_folder = None
 
         self.parallel_sims = parallel_sims
-        self.threads = []
+        self.sim_tasks = []
+        # Create another logger for the SimRunner class
 
         # master_log_filename = self.circuit_radic + '.masterlog' TODO: create the JSON or YAML file
-        self.logger = logging.getLogger("SimCommander")
+        self.logger = logging.getLogger("SimRunner")
         self.logger.setLevel(logging.INFO)
-        # TODO redirect this logger to a file.
+        # redirect this logger to a file.
+        self.logger.addHandler(logging.FileHandler('SimRunner.log', mode='w'))
+        # if verbose is true, all log messages are also printed to the console
+        if verbose:
+            self.logger.addHandler(logging.StreamHandler())
+        self.logger.info("SimRunner started")
 
         self.runno = 0  # number of total runs
         self.failSim = 0  # number of failed simulations
-        self.okSim = 0  # number of succesfull completed simulations
+        self.okSim = 0  # number of successful completed simulations
         # self.failParam = []  # collects for later user investigation of failed parameter sets
 
         # Gets a simulator.
         if simulator is None:
-            self.simulator = Simulator.get_default_simulator()
-        elif isinstance(simulator, Simulator):
+            from ..sim.ltspice_simulator import LTspice  # Used for defaults
+            self.simulator = LTspice
+        elif issubclass(simulator, Simulator):
             self.simulator = simulator
-        elif isinstance(simulator, (str, pathlib.Path)):
+        elif isinstance(simulator, (str, Path)):
             self.simulator = Simulator.create_from(simulator)
         else:
-            raise TypeError("Invalid simulator type. Either use a string with the ")
-
-        if file_ext == '.asc':
-            netlist_file = self.circuit_radic + '.net'
-            if self.verbose:
-                print("Creating Netlist")
-            retcode = self.simulator.create_netlist(circuit_file)
-            if retcode == 0 and os.path.exists(netlist_file):
-                if self.verbose:
-                    print("The Netlist was successfully created")
-            else:
-                if self.verbose:
-                    print("Unable to create the Netlist from %s" % circuit_file)
-                netlist_file = None
-        elif os.path.exists(circuit_file):
-            netlist_file = circuit_file
-        else:
-            netlist_file = None
-            if self.verbose:
-                print("Unable to find the Netlist: %s" % circuit_file)
-
-        super(SimCommander, self).__init__(netlist_file, encoding=encoding)
-        self.reset_netlist()
-        if len(self.netlist) == 0:
-            self.logger.error("Unable to create Netlist")
+            raise TypeError("Invalid simulator type.")
 
     def __del__(self):
         """Class Destructor : Closes Everything"""
-        self.logger.debug("Waiting for all spawned threads to finish.")
-        self.wait_completion()  # TODO: Kill all pending simulations
+        self.logger.debug("Waiting for all spawned sim_tasks to finish.")
+        self.wait_completion(abort_all_on_timeout=True)  # Kill all pending simulations
         self.logger.debug("Exiting SimCommander")
 
-    def setLTspiceRunCommand(self, spice_tool: Union[str, Simulator]) -> None:
+    def set_run_command(self, spice_tool: Union[str, Simulator]) -> None:
         """
-        Manually setting the LTSpice run command.
+        Manually setting the LTSpice run command
 
         :param spice_tool: String containing the path to the spice tool to be used, or alternatively the Simulator
-                           object.
+            object.
         :type spice_tool: str or Simulator
         :return: Nothing
         :rtype: None
         """
         if isinstance(spice_tool, str):
             self.simulator = Simulator.create_from(spice_tool)
         elif isinstance(spice_tool, Simulator):
             self.simulator = spice_tool
         else:
             raise TypeError("Expecting str or Simulator objects")
 
-    def add_LTspiceRunCmdLineSwitches(self, *args) -> None:
+    def SetRunCommand(self, spice_tool: Union[str, Simulator]) -> None:
+        """
+        *(Deprecated)*
+        Use set_run_command() method.
+        """
+        self.set_run_command(spice_tool)
+
+    def clear_command_line_switches(self):
+        """Clear all the command line switches added previously"""
+        self.cmdline_switches.clear()
+
+    def add_command_line_switch(self, switch, path=''):
         """
         Used to add an extra command line argument such as -I<path> to add symbol search path or -FastAccess
         to convert the raw file into Fast Access.
-        The arguments is a list of strings as is defined in the LTSpice command line documentation.
+        The argument is a string as is defined in the LTSpice command line documentation.
 
-        :param args: list of strings
-            A list of command line switches such as "-ascii" for generating a raw file in text format or "-alt" for
-            setting the solver to alternate. See Command Line Switches information on LTSpice help file.
-        :type args: list[str]
+        :param switch: switch to be added.
+        :type switch: str:  A command line switch such as "-ascii" for generating a raw file in text format or
+            "-alt" for setting the solver to alternate. See Command Line Switches information on LTSpice help file.
+        :param path: path to the file related to the switch being given.
+        :type path: str, optional
         :returns: Nothing
         """
-        self.simulator.add_command_line_switche(*args)
+        self.cmdline_switches.append(switch)
+        if path is not None:
+            self.cmdline_switches.append(path)
+
+    def _on_output_folder(self, afile):
+        if self.output_folder:
+            return self.output_folder / afile
+        else:
+            return Path(afile)
+
+    def _to_output_folder(self, afile: Path, *, copy: bool, new_name: str = ''):
+        if self.output_folder:
+            if new_name:
+                ddst = self.output_folder / new_name
+            else:
+                ddst = self.output_folder
+
+            if copy:
+                dest = shutil.copy(afile, ddst)
+            else:
+                dest = shutil.move(afile, ddst)
+            return Path(dest)
+        else:
+            if new_name:
+                dest = shutil.copy(afile, afile.parent / new_name)
+                return Path(dest)
+            else:
+                return afile
+
+    def _run_file_name(self, netlist):
+        if not isinstance(netlist, Path):
+            netlist = Path(netlist)
+        return "%s_%i.net" % (netlist.stem, self.runno)
+
+    def create_netlist(self, asc_file: Union[str, Path]):
+        """Creates a .net from an .asc using the LTSpice -netlist command line"""
+        if not isinstance(asc_file, Path):
+            asc_file = Path(asc_file)
+        if asc_file.suffix == '.asc':
+            if self.verbose:
+                self.logger.info("Creating Netlist")
+            return self.simulator.create_netlist(asc_file)
+        else:
+            self.logger.info("Unable to create the Netlist from %s" % asc_file)
+            return None
+
+    def _prepare_sim(self, netlist: Union[str, Path, SpiceEditor], run_filename: str):
+        """Internal function"""
+        # update number of simulation
+        self.runno += 1  # Incrementing internal simulation number
+        # Harmonize the netlist into a Path object pointing to a netlist file on the right output folder
+        if isinstance(netlist, SpiceEditor):
+            if run_filename is None:
+                run_filename = self._run_file_name(netlist.netlist_file)
 
-    def run(self, run_filename: str = None, wait_resource: bool = True,
-            callback: Callable[[str, str], Any] = None, timeout: float = 600) -> RunTask:
+            # Calculates the path where to store the new netlist.
+            run_netlist_file = self._on_output_folder(run_filename).with_suffix('.net')
+            netlist.write_netlist(run_netlist_file)
+
+        elif isinstance(netlist, (Path, str)):
+            if run_filename is None:
+                run_filename = self._run_file_name(netlist)
+            if isinstance(netlist, str):
+                netlist = Path(netlist)
+            run_netlist_file = self._to_output_folder(netlist, copy=True, new_name=run_filename)
+        else:
+            raise TypeError("'netlist' parameter shall be a SpiceEditor, pathlib.Path or a plain str")
+
+        self.workfiles.append(run_netlist_file)
+        return run_netlist_file
+
+    def run(self, netlist: Union[str, Path, SpiceEditor], *, wait_resource: bool = True,
+            callback: Union[Type[ProcessCallback], Callable[[Path, Path], Any]] = None, switches=None,
+            timeout: float = 600, run_filename: str = None) -> Union[RunTask, None]:
         """
         Executes a simulation run with the conditions set by the user.
         Conditions are set by the set_parameter, set_component_value or add_instruction functions.
 
-        :param run_filename:
+        :param netlist:
             The name of the netlist can be optionally overridden if the user wants to have a better control of how the
             simulations files are generated.
-        :type run_filename: str, optional
+        :type netlist: SpiceEditor or a path to the file
         :param wait_resource:
             Setting this parameter to False will force the simulation to start immediately, irrespective of the number
             of simulations already active.
-            By default the SimCommander class uses only four processors. This number can be overridden by setting
+            By default, the SimCommander class uses only four processors. This number can be overridden by setting
             the parameter ´parallel_sims´ to a different number.
             If there are more than ´parallel_sims´ simulations being done, the new one will be placed on hold till one
             of the other simulations are finished.
         :type wait_resource: bool, optional
         :param callback:
             The user can optionally give a callback function for when the simulation finishes so that processing can
-            be done immediately.
-        :type: callback: function(raw_file, log_file), optional
+            be done immediately. The callback function must receive two input parameters that correspond the raw and
+            log files created by the simulation. The argument type is of the type pathlib.Path
+        :type: callback: function(raw_file: Path, log_file: Path), optional
+        :param switches: Command line switches override
+        :type switches: list
         :param timeout: Timeout to be used in waiting for resources. Default time is 600 seconds, i.e. 10 minutes.
         :type timeout: float, optional
-
+        :param run_filename: Name to be used for the log and raw file.
+        :type run_filename: str or Path
         :returns: The task object of type RunTask
         """
-        # decide sim required
-        if self.netlist is not None:
-            # update number of simulation
-            self.runno += 1  # Using internal simulation number in case a run_id is not supplied
-
-            # Write the new settings
-            if run_filename is None:
-                run_netlist_file = "%s_%i.net" % (self.circuit_radic, self.runno)
-            else:
-                run_netlist_file = run_filename
+        if switches is None:
+            switches = []
+        run_netlist_file = self._prepare_sim(netlist, run_filename)
+
+        t0 = clock()  # Store the time for timeout calculation
+        while clock() - t0 < timeout:
+            cmdline_switches = switches or self.cmdline_switches  # If switches are passed, they override the ones
+            # inside the class.
+
+            if (wait_resource is False) or (self.active_threads() < self.parallel_sims):
+                t = RunTask(self.simulator, self.runno, run_netlist_file, callback, cmdline_switches,
+                            timeout=self.timeout, verbose=self.verbose)
+                self.sim_tasks.append(t)
+                t.start()
+                sleep(0.01)  # Give slack for the thread to start
+                return t  # Returns the task object
+            sleep(0.1)  # Give Time for other simulations to end
+        else:
+            self.logger.error("Timeout waiting for resources for simulation %d" % self.runno)
+            if self.verbose:
+                self.logger.info("Timeout on launching simulation %d." % self.runno)
+            return None
 
-            self.write_netlist(run_netlist_file)
-            t0 = time.perf_counter()  # Store the time for timeout calculation
-            while time.perf_counter() - t0 < timeout:
-                self.updated_stats()  # purge ended tasks
-
-                if (wait_resource is False) or (len(self.threads) < self.parallel_sims):
-                    t = RunTask(self.simulator, self.runno, run_netlist_file, callback,
-                                timeout=self.timeout, verbose=self.verbose)
-                    self.threads.append(t)
-                    t.start()
-                    sleep(0.01)  # Give slack for the thread to start
-                    return t  # Returns the task number
-                sleep(0.1)  # Give Time for other simulations to end
-            else:
-                self.logger.error("Timeout waiting for resources for simulation %d" % self.runno)
-                if self.verbose:
-                    print("Timeout on launching simulation %d." % self.runno)
+    def run_now(self, netlist: Union[str, Path, SpiceEditor], *, switches=None, run_filename: str = None) -> (str, str):
+        """
+        Executes a simulation run with the conditions set by the user.
+        Conditions are set by the set_parameter, set_component_value or add_instruction functions.
 
-        else:
-            # no simulation required
-            raise UserWarning('skipping simulation ' + str(self.runno))
+        :param netlist:
+            The name of the netlist can be optionally overridden if the user wants to have a better control of how the
+            simulations files are generated.
+        :type netlist: SpiceEditor or a path to the file
+        :param switches: Command line switches override
+        :type switches: list
+        :param run_filename: Name to be used for the log and raw file.
+        :type run_filename: str or Path
+        :returns: the raw and log filenames
+        """
+        if switches is None:
+            switches = []
+        run_netlist_file = self._prepare_sim(netlist, run_filename)
+
+        cmdline_switches = switches or self.cmdline_switches  # If switches are passed, they override the ones inside
+
+        # the class.
+
+        def dummy_callback(raw, log):
+            """Dummy call back that does nothing"""
+            return None
+
+        t = RunTask(self.simulator, self.runno, run_netlist_file, dummy_callback, cmdline_switches,
+                    timeout=self.timeout, verbose=self.verbose)
+        t.start()
+        sleep(0.01)  # Give slack for the thread to start
+        while t.is_alive():
+            sleep(0.1)  # Waits for the task to terminate
+
+        return t.raw_file, t.log_file  # Returns the raw and log file
+
+    def active_threads(self):
+        """Returns the number of active sim_tasks"""
+        count = 0
+        for t in self.sim_tasks:
+            if t.is_alive():
+                count += 1
+        return count
 
-    def updated_stats(self):
+    def updated_stats(self, release_tasks: bool = True):
         """
         This function updates the OK/Fail statistics and releases finished RunTask objects from memory.
 
+        :param release_tasks: Boolean indicating whether the tasks are to be released.
+        :type release_tasks: bool
         :returns: Nothing
         """
         i = 0
-        while i < len(self.threads):
-            if self.threads[i].is_alive():
+        while i < len(self.sim_tasks):
+            if self.sim_tasks[i].is_alive():
                 i += 1
             else:
-                if self.threads[i].retcode == 0:
+                if self.sim_tasks[i].retcode == 0:
                     self.okSim += 1
                 else:
                     # simulation failed
                     self.failSim += 1
-                del self.threads[i]
+                if release_tasks:
+                    task = self.sim_tasks.pop(i)
+                    task.join()
 
-    @staticmethod
-    def kill_all_ltspice():
+    def kill_all_ltspice(self):
         """Function to terminate LTSpice in windows"""
-        simulator = Simulator.get_default_simulator()
-        simulator.kill_all()
+        simulator = Simulator
+        process_name = simulator.process_name
+        import psutil
+        for proc in psutil.process_iter():
+            # check whether the process name matches
+
+            if proc.name() == process_name:
+                self.logger.info("killing ngspice", proc.pid)
+                proc.kill()
 
     def wait_completion(self, timeout=None, abort_all_on_timeout=False) -> bool:
         """
         This function will wait for the execution of all scheduled simulations to complete.
 
         :param timeout: Cancels the wait after the number of seconds specified by the timeout.
             This timeout is reset everytime that a simulation is completed. The difference between this timeout and the
-            one defined in the SimCommander instance, is that the later is implemented by the subprocess class, and the
-            this timeout just cancels the wait.
+            one defined in the SimRunner instance, is that the latter is implemented by the subprocess class, and
+            this one just cancels the wait.
         :type timeout: int
         :param abort_all_on_timeout: attempts to stop all LTSpice processes if timeout is expired.
         :type abort_all_on_timeout: bool
         :returns: True if all simulations were executed successfully
         :rtype: bool
         """
         self.updated_stats()
         timeout_counter = 0
         sim_counters = (self.okSim, self.failSim)
 
-        while len(self.threads) > 0:
+        while len(self.sim_tasks) > 0:
             sleep(1)
             self.updated_stats()
             if timeout is not None:
                 if sim_counters == (self.okSim, self.failSim):
                     timeout_counter += 1
-                    print(timeout_counter, "timeout counter")
+                    self.logger.info(timeout_counter, "timeout counter")
                 else:
                     timeout_counter = 0
 
                 if timeout_counter > timeout:
                     if abort_all_on_timeout:
                         self.kill_all_ltspice()
                     return False
 
         return self.failSim == 0
 
-
-if __name__ == "__main__":
-    # get script absolute path
-    meAbsPath = os.path.dirname(os.path.realpath(__file__))
-    meAbsPath, _ = os.path.split(meAbsPath)
-    # select spice model
-    LTC = SimCommander(meAbsPath + "\\test_files\\testfile.asc")
-    # set default arguments
-    LTC.set_parameters(res=0.001, cap=100e-6)
-    # define simulation
-    LTC.add_instructions(
-            "; Simulation settings",
-            # [".STEP PARAM Rmotor LIST 21 28"],
-            ".TRAN 3m",
-            # ".step param run 1 2 1"
-    )
-    # do parameter sweep
-    for res in range(5):
-        # LTC.runs_to_do = range(2)
-        LTC.set_parameters(ANA=res)
-        raw, log = LTC.run()
-        print("Raw file '%s' | Log File '%s'" % (raw, log))
-    # Sim Statistics
-    print('Successful/Total Simulations: ' + str(LTC.okSim) + '/' + str(LTC.runno))
-
-
-    def callback_function(raw_file, log_file):
-        print("Handling the simulation data of %s, log file %s" % (raw_file, log_file))
-
-
-    LTC = SimCommander(meAbsPath + "\\test_files\\testfile.asc", parallel_sims=1)
-    tstart = 0
-    for tstop in (2, 5, 8, 10):
-        tduration = tstop - tstart
-        LTC.add_instruction(".tran {}".format(tduration), )
-        if tstart != 0:
-            LTC.add_instruction(".loadbias {}".format(bias_file))
-            # Put here your parameter modifications
-            # LTC.set_parameters(param1=1, param2=2, param3=3)
-        bias_file = "sim_loadbias_%d.txt" % tstop
-        LTC.add_instruction(".savebias {} internal time={}".format(bias_file, tduration))
-        tstart = tstop
-        LTC.run(callback=callback_function)
-
-    LTC.reset_netlist()
-    LTC.add_instruction('.ac dec 40 1m 1G')
-    LTC.set_component_value('V1', 'AC 1 0')
-    LTC.run(callback=callback_function)
-    LTC.wait_completion()
+    def file_cleanup(self):
+        """
+        Will delete all log and raw files that were created by the script. This should only be executed at the end
+        of data processing.
+        """
+        self.updated_stats()
+        while len(self.workfiles):
+            workfile = self.workfiles.pop(0)
+            if workfile.suffix == '.net':
+                # Delete the log file if exists
+                logfile = workfile.with_suffix('.log')
+                if logfile.exists():
+                    self.logger.info("Deleting..." + logfile.name)
+                    logfile.unlink()
+                # Delete the raw file if exists
+                rawfile = workfile.with_suffix('.raw')
+                if rawfile.exists():
+                    self.logger.info("Deleting..." + rawfile.name)
+                    rawfile.unlink()
+
+                # Delete the op.raw file if exists
+                oprawfile = workfile.with_suffix('.op.raw')
+                if oprawfile.exists():
+                    self.logger.info("Deleting..." + oprawfile.name)
+                    oprawfile.unlink()
+
+            # Delete the file
+            self.logger.info("Deleting..." + workfile.name)
+            workfile.unlink()
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        t0 = clock()
+        while True:
+            i = 0
+            while i < len(self.sim_tasks):
+                if self.sim_tasks[i].is_alive():
+                    i += 1
+                else:
+                    if self.sim_tasks[i].retcode == 0:
+                        self.okSim += 1
+                    else:
+                        # simulation failed
+                        self.failSim += 1
+                    task = self.sim_tasks.pop(i)
+                    ret = task.get_results()
+                    task.join()
+                    return ret
+
+            if i == 0:
+                # when there aren't any pending jobs left, exit the iterator
+                raise StopIteration
+
+            sleep(0.2)  # Go asleep for a sec
+            if self.timeout and ((clock() - t0) > self.timeout):
+                raise SimRunnerTimeoutError(f"Exceeded {self.timeout} seconds waiting for tasks to finish")
```

### Comparing `PyLTSpice-3.1/PyLTSpice/sim_stepping.py` & `PyLTSpice-4.0/PyLTSpice/sim/xyce_simulator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,159 +1,135 @@
 #!/usr/bin/env python
+# coding=utf-8
 
 # -------------------------------------------------------------------------------
 #    ____        _   _____ ____        _
 #   |  _ \ _   _| | |_   _/ ___| _ __ (_) ___ ___
 #   | |_) | | | | |   | | \___ \| '_ \| |/ __/ _ \
 #   |  __/| |_| | |___| |  ___) | |_) | | (_|  __/
 #   |_|    \__, |_____|_| |____/| .__/|_|\___\___|
 #          |___/                |_|
 #
-# Name:        sim_stepping.py
-# Purpose:     Spice Simulation Library intended to automate the exploring of
-#              design corners, try different models and different parameter
-#              settings.
+# Name:        xyce_simulator.py
+# Purpose:     Tool used to launch NGspice simulations in batch mode.
 #
 # Author:      Nuno Brum (nuno.brum@gmail.com)
 #
-# Created:     31-07-2020
+# Created:     14-03-2023
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
 
-__author__ = "Nuno Canto Brum <nuno.brum@gmail.com>"
-__copyright__ = "Copyright 2017, Fribourg Switzerland"
+import logging
+import sys
+import os
+
+from pathlib import Path
+from typing import Union
+
+from .simulator import Simulator, run_function
+
+
+class XyceSimulator(Simulator):
+    """Stores the simulator location and command line options and runs simulations."""
+    spice_exe = ["C:/Program Files/Xyce 7.6 NORAD/bin/xyce.exe"]
+    process_name = "XVIIx64.exe"
+    xyce_args = {
+        '-b'                : ['-b'],  # batch mode flag for spice compatibility (ignored)
+        '-h'                : ['-h'],  # print usage and exit
+        '-v'                : ['-v'],  # print version info and exit
+        '-capabilities'     : ['-capabilities'],  # print compiled-in options and exit
+        '-license'          : ['-license'],  # print license and exit
+        '-param'            : ['-param', '<param_options>'],
+        # [device [level [<inst|mod>]]] print a terse summary of model and/or device parameters
+        '-doc'              : ['-doc', '<param_options>'],
+        # [device [level [<inst|mod>]]] output latex tables of model and device parameters to files
+        '-doc_cat'          : ['-doc_cat', '<param_options>'],
+        # [device [level [<inst|mod>]]] output latex tables of model and device parameters to files
+        '-count'            : ['-count'],  # device count without netlist syntax or topology check
+        '-syntax'           : ['-syntax'],  # check netlist syntax and exit
+        '-norun'            : ['-norun'],  # netlist syntax and topology and exit
+        '-namesfile'        : ['-namesfile', '<path>'],  # output internal names file to <path> and exit
+        '-noise_names_file' : ['-noise_names_file', '<path>'],  # output noise source names file to <path> and exit
+        '-quiet'            : ['-quiet'],  # suppress some of the simulation-progress messages sent to stdout
+        '-jacobian_test'    : ['-jacobian_test'],  # jacobian matrix diagnostic
+        '-hspice-ext'       : ['-hspice-ext', '<hsext_options>'],
+        # apply hspice compatibility features during parsing.  option=all applies them all
+        '-redefined_params' : ['-redefined_params', '<redef_param_option>'],
+        # set option for redefined .params as ignore (use last), usefirst, warn or error
+        '-subckt_multiplier': ['-subckt_multiplier', '<truefalse_option>'],
+        # set option to true(default) or false to apply implicit subcircuit multipliers
+        '-delim'            : ['-delim', '<delim_option>'],  # <TAB|COMMA|string>   set the output file field delimiter
+        '-o'                : ['-o', '<basename>'],  # <basename> for the output file(s)
+        '-l'                : ['-l', '<path>'],  # place the log output into <path>, "cout" to log to stdout
+        '-per-processor'    : ['-per-processor'],  # create log file for each processor, add .<n>.<r> to log path
+        '-remeasure'        : ['-remeasure', '<path>'],
+        # [existing Xyce output file] recompute .measure() results with existing data
+        '-nox'              : ['-nox', 'onoff_option'],  # <on|off>               NOX nonlinear solver usage
+        '-linsolv'          : ['-linsolv', '<solver>'],  # <solver>           force usage of specific linear solver
+        '-maxord'           : ['-maxord', '<int_option>'],  # <1..5>              maximum time integration order
+        '-max'              : ['-max', '<int_option>'],  # -warnings <#>           maximum number of warning messages
+        '-prf'              : ['-prf', '<path>'],  # <param file name>      specify a file with simulation parameters
+        '-rsf'              : ['-rsf', '<path>'],  # specify a file to save simulation responses functions.
+        '-r'                : ['-r', '<path>'],  # <file>   generate a rawfile named <file> in binary format
+        '-a'                : ['-a', '<path>'],  # use with -r <file> to output in ascii format
+        '-randseed'         : ['-randseed', '<int_option>'],
+        # <number>          seed random number generator used by expressions and sampling methods
+    }
 
-from typing import Callable, Any
-from typing import Iterable
-from .sim_batch import SimCommander
-
-
-class StepInfo(object):
-    def __init__(self, what: str, elem: str, iterable: Iterable):
-        self.what = what
-        self.elem = elem
-        self.iter = iterable
-
-    def __len__(self):
-        return len(list(self.iter))
-
-    def __str__(self):
-        return f"Iteration on {self.what} {self.elem} : {self.iter}"
-
-
-class SimStepper(SimCommander):
-
-    def __init__(self, spice_file: str, parallel_sims=4, renaming_mask=None):
-        """This class is intended to be used for simulations with many parameter sweeps. This provides a more user-
-        friendly interface than the SimCommander class when there are many parameters to be found. Using the
-        SimCommander class a loop needs to be added for each dimension of the simulations.
-        A typical usage would be as follows:
-        ```
-        LTC = SimCommander("my_circuit.asc")
-        for dmodel in ("BAT54", "BAT46WJ")
-            LTC.set_element_model("D1", model)  # Sets the Diode D1 model
-            for res_value1 in sweep(2.2, 2,4, 0.2):  # Steps from 2.2 to 2.4 with 0.2 increments
-                LTC.set_component_value('R1', res_value1)  # Updates the resistor R1 value to be 3.3k
-                for temperature in sweep(0, 80, 20):  # Makes temperature step from 0 to 80 degrees in 20 degree steps
-                    LTC.set_parameters(temp=80)  # Sets the simulation temperature to be 80 degrees
-                    for res_value2 in (10, 25, 32):
-                        LTC.set_component_value('R2', res_value2)  # Updates the resistor R2 value to be 3.3k
-                        LTC.run()
-
-        LTC.wait_completion()  # Waits for the LTSpice simulations to complete
-        ```
-
-        With SimStepper the same thing can be done as follows, resulting in a more cleaner code.
-
-        ```
-        Stepper = SimStepper("my_circuit.asc")
-        Stepper.add_model_sweep('D1', "BAT54", "BAT46WJ")
-        Stepper.add_component_sweep('R1', sweep(2.2, 2,4, 0.2))  # Steps from 2.2 to 2.4 with 0.2 increments
-        Stepper.add_parameter_sweep('temp', sweep(0, 80, 20))  # Makes temperature step from 0 to 80 degrees in 20
-                                                               # degree steps
-        Stepper.add_component_sweep('R2', (10, 25, 32)) #  Updates the resistor R2 value to be 3.3k
-        Stepper.run_all()
-
-        ```
-
-        Another advantage of using SimStepper is that it can optionally use the .SAVEBIAS in the first simulation and
-        then use the .LOADBIAS command at the subsequent ones to speed up the simulation times.
+    @classmethod
+    def valid_switch(cls, switch, parameter='') -> list:
         """
-        SimCommander.__init__(self, spice_file, parallel_sims)
-        self.iter_list = []
+        Validates a command line switch. The following options are available for Xyce:
 
-    def add_param_sweep(self, param: str, iterable: Iterable):
-        """Adds a dimension to the simulation, where the param is swept."""
-        self.iter_list.append(StepInfo("param", param, iterable))
-
-    def add_value_sweep(self, comp: str, iterable: Iterable):
-        """Adds a dimension to the simulation, where a component value is swept."""
-        # The next line raises an ComponentNotFoundError if the component doesn't exist
-        _ = self.get_component_value(comp)
-        self.iter_list.append(StepInfo("component", comp, iterable))
-
-    def add_model_sweep(self, comp: str, iterable: Iterable):
-        """Adds a dimension to the simulation, where a component model is swept."""
-        # The next line raises an ComponentNotFoundError if the component doesn't exist
-        _ = self.get_component_value(comp)
-        self.iter_list.append(StepInfo("model", comp, iterable))
-
-    def total_number_of_simulations(self):
-        """Returns the total number of simulations foreseen."""
-        total = 1
-        for step in self.iter_list:
-            l = len(step)
-            if l:
-                total *= l
+        :param switch: switch to be added. If the switch is not on the list above, it should be correctly formatted with
+            the preceding '-' switch
+        :type switch: str
+        :param parameter: parameter for the switch
+        :type parameter: str, optional
+        :return: the correct formatting for the switch
+        :rtype: list
+        """
+        ret = []  # This is an empty switch
+        if switch in cls.xyce_args:
+            switch_list = cls.xyce_args[switch]
+            if len(switch_list) == 2:
+                param_token = switch_list[1]
+                if param_token == '<path>':
+                    ret = [switch_list[0], parameter]
+                elif param_token == '<param_options>':
+                    # Check for [device [level [<inst|mod>]]] syntax ??
+                    ret = [switch_list[0], parameter]
+                elif param_token == '<hsext_options>':
+                    ret = [switch_list[0], parameter]
+                elif param_token == '<redef_param_option>':
+                    if parameter in ('ignore', 'uselast', 'usefirst', 'warn', 'error'):
+                        ret = [switch_list[0], parameter]
+                elif param_token == '<truefalse_option>':
+                    if parameter.lower() in ('true', 'false'):
+                        ret = [switch_list[0], parameter]
+                elif param_token == '<delim_option>':
+                    ret = [switch_list[0], parameter]
+                elif param_token == '<onoff_option>':
+                    if parameter.lower() in ('on', 'off'):
+                        ret = [switch_list[0], parameter]
+                elif param_token == '<int_option>':
+                    try:
+                        int(parameter)
+                    except ValueError:
+                        pass
+                    else:
+                        ret = [switch_list[0], parameter]
+                else:
+                    print(f"Invalid parameter {parameter} for switch '{switch}'")
             else:
-                print(step, " is empty")
-        return total
+                ret = switch_list
+        else:
+            print(f"Invalid Switch {switch}")
+        return ret
+
+    @classmethod
+    def run(cls, netlist_file, cmd_line_switches, timeout):
+        cmd_run = cls.spice_exe + cmd_line_switches + [netlist_file]
+        # start execution
+        return run_function(cmd_run, timeout=timeout)
 
-    def run_all(self, callback: Callable[[str, str], Any] = None, use_loadbias='Auto'):
-        assert use_loadbias in ('Auto', 'Yes', 'No'), "use_loadbias argument must be 'Auto', 'Yes' or 'No'"
-        if (use_loadbias == 'Auto' and self.total_number_of_simulations() > 10) or use_loadbias == 'Yes':
-            # It will choose to use .SAVEBIAS/.LOADBIAS if the number of simulaitons is higher than 10
-            # TODO: Make a first simulation and storing the bias
-            pass
-        iter_no = 0
-        iterators = [iter(step.iter) for step in self.iter_list]
-        while True:
-            while 0 <= iter_no < len(self.iter_list):
-                try:
-                    value = iterators[iter_no].__next__()
-                except StopIteration:
-                    iterators[iter_no] = iter(self.iter_list[iter_no].iter)
-                    iter_no -= 1
-                    continue
-                if self.iter_list[iter_no].what == 'param':
-                    self.set_parameter(self.iter_list[iter_no].elem, value)
-                elif self.iter_list[iter_no].what == 'component':
-                    self.set_component_value(self.iter_list[iter_no].elem, value)
-                elif self.iter_list[iter_no].what == 'model':
-                    self.set_element_model(self.iter_list[iter_no].elem, value)
-                else:
-                    # TODO: develop other types of sweeps EX: add .STEP instruction
-                    raise ValueError("Not Supported sweep")
-                iter_no += 1
-            if iter_no < 0:
-                break
-            # TODO: Implement the renaming Mask, so the output filename is written according to user instructions
-            SimCommander.run(self, callback=callback)  # Like this a recursion is avoided
-            iter_no = len(self.iter_list) - 1  # Resets the counter to start next iteration
-        # Now waits for the simulations to end
-        self.wait_completion()
-
-    def run(self):
-        """Rather uses run_all instead"""
-        self.run_all()
-
-
-if __name__ == "__main__":
-    from PyLTSpice.sweep_iterators import *
-
-    test = SimStepper("..\\tests\\DC sweep.asc")
-    test.verbose = True
-    test.add_param_sweep("res", [10, 11, 9])
-    test.add_value_sweep("R1", sweep_log(0.1, 10))
-    test.add_model_sweep("D1", ("model1", "model2"))
-    test.run_all()
```

### Comparing `PyLTSpice-3.1/PyLTSpice/simulator.py` & `PyLTSpice-4.0/PyLTSpice/sim/ltspice_simulator.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,47 +5,68 @@
 #    ____        _   _____ ____        _
 #   |  _ \ _   _| | |_   _/ ___| _ __ (_) ___ ___
 #   | |_) | | | | |   | | \___ \| '_ \| |/ __/ _ \
 #   |  __/| |_| | |___| |  ___) | |_) | | (_|  __/
 #   |_|    \__, |_____|_| |____/| .__/|_|\___\___|
 #          |___/                |_|
 #
-# Name:        simulator.py
-# Purpose:     Represents a Simulator tool and it's command line options
+# Name:        ltspice_simulator.py
+# Purpose:     Represents a LTspice tool and it's command line options
 #
 # Author:      Nuno Brum (nuno.brum@gmail.com)
 #
 # Created:     23-12-2016
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
+import logging
 import sys
 import os
-import subprocess
-import time
-from pathlib import Path
-
-if sys.version_info.major >= 3 and sys.version_info.minor >= 6:
-    clock_function = time.process_time
-
-
-    def run_function(command, timeout=None):
-        result = subprocess.run(command, timeout=timeout)
-        return result.returncode
-else:
-    clock_function = time.clock
 
+from pathlib import Path
+from typing import Union
 
-    def run_function(command, timeout=None):
-        return subprocess.call(command, timeout=timeout)
+from .simulator import Simulator, run_function
 
 
-class Simulator(object):
+class LTspice(Simulator):
     """Stores the simulator location and command line options and is responsible for generating netlists and running
     simulations."""
 
+    """Searches on the any usual locations for a simulator"""
+    if sys.platform == "linux":
+        if os.environ.get('LTSPICEFOLDER') is not None:
+            spice_exe = ["wine", os.environ['LTSPICEFOLDER'] + "/XVIIx64.exe"]
+        else:
+            spice_exe = ["wine",
+                           os.path.expanduser("~") + "/.wine/drive_c/Program Files/LTC/LTspiceXVII/XVIIx64.exe"]
+        process_name = "XVIIx64.exe"
+    elif sys.platform == "darwin":
+        spice_exe = ['/Applications/LTspice.app/Contents/MacOS/LTspice']
+        process_name = "XVIIx64"
+    else:  # Windows
+        for exe in (  # Placed in order of preference. The first to be found will be used.
+                os.path.expanduser(r"~\AppData\Local\Programs\ADI\LTspice\LTspice.exe"),
+                r"C:\Program Files\ADI\LTspice\LTspice.exe",
+                r"C:\Program Files\LTC\LTspiceXVII\XVIIx64.exe",
+                r"C:\Program Files (x86)\LTC\LTspiceIV\scad3.exe",  # Legacy LTspice IV
+        ):
+            if os.path.exists(exe):
+                print(f"Using LTspice installed in : '{exe}' ")
+                spice_exe = [exe]
+                break
+        else:
+            spice_exe = []
+            print("================== ALERT! ====================")
+            print("Unable to find a LTSpice executable.")
+            print("A specific location of the LTSPICE can be set")
+            print("using the create_from(<location>) class method")
+            print("==============================================")
+
+        process_name = "XVIIx64.exe"
+
     ltspice_args = {
         'alt' : ['-alt'],  # Set solver to Alternate.
         'ascii'     : ['-ascii'],  # Use ASCII.raw files. Seriously degrades program performance.
         # 'batch': ['-b <path>'], # Used by run command: Run in batch mode.E.g. "ltspice.exe-b deck.cir" will leave the data infile deck.raw
         'big'       : ['-big'],  # Start as a maximized window.
         'encrypt'   : ['-encrypt'],
         # Encrypt a model library.For 3rd parties wishing to allow people to use libraries without
@@ -70,97 +91,37 @@
         'SOI'       : ['-SOI'],  # Allow MOSFET's to have up to 7 nodes even in subcircuit expansion.
         'sync'      : ['-sync'],  # Update component libraries
         'uninstall' : ['-uninstall'],  # Please don't. Executes one step of the uninstallation process.
 
     }
 
     @classmethod
-    def get_default_simulator(cls):
-        if sys.platform == "linux":
-            if os.environ.get('LTSPICEFOLDER') is not None:
-                LTspice_exe = ["wine", os.environ['LTSPICEFOLDER'] + "/XVIIx64.exe"]
-            else:
-                LTspice_exe = ["wine",
-                               os.path.expanduser("~") + "/.wine/drive_c/Program Files/LTC/LTspiceXVII/XVIIx64.exe"]
-            process_name = "XVIIx64.exe"
-        elif sys.platform == "darwin":
-            LTspice_exe = ['/Applications/LTspice.app/Contents/MacOS/LTspice']
-            process_name = "XVIIx64"
-        else:  # Windows
-            for exe in (  # Placed in order of preference. The first to be found will be used.
-                    os.path.expanduser(r"~\AppData\Local\Programs\ADI\LTspice\LTspice.exe"),
-                    r"C:\Program Files\ADI\LTspice\LTspice.exe",
-                    r"C:\Program Files\LTC\LTspiceXVII\XVIIx64.exe",
-                    r"C:\Program Files (x86)\LTC\LTspiceIV\scad3.exe",  # Legacy LTspice IV
-            ):
-                if os.path.exists(exe):
-                    print(f"Using LTspice installed in : '{exe}' ")
-                    LTspice_exe = [exe]
-                    _, process_name = os.path.split(exe)
-                    break
-            else:
-                raise FileNotFoundError("A suitable exe file was not found. Please locate the spice simulator "
-                                        "executable and pass it to the SimCommander object by using the 'simulator'"
-                                        "parameter.")
-        return cls(LTspice_exe, process_name)
-
-    @classmethod
-    def create_from(cls, path_to_exe):
+    def valid_switch(cls, switch, path='') -> list:
         """
-        Creates a simulator class from a path to the simulator executable
-        :param path_to_exe:
-        :type path_to_exe: pathlib.Path or str
-        :return: a class instance representing the Spice simulator
-        :rtype: Simulator
-        """
-        plib_path_to_exe = Path(path_to_exe)
-        if plib_path_to_exe.exists():
-            if sys.platform == 'darwin':
-                process_name = plib_path_to_exe.stem
-            else:
-                process_name = plib_path_to_exe.name
-            return cls([plib_path_to_exe.as_posix()], process_name)
-        else:
-            raise FileNotFoundError(f"Provided exe file was not found '{path_to_exe}'")
-
-    def __init__(self, spice_exe, process_name):
-        if not isinstance(spice_exe, list):
-            raise TypeError("spice_exe must be a list of strings that can be passed into the subprocess call")
-
-        self.spice_exe = spice_exe
-        self.cmdline_switches = []
-        self.process_name = process_name
-
-    def clear_command_line_switches(self):
-        """Clear all the command line switches added previously"""
-        self.cmdline_switches.clear()
-
-    def add_command_line_switch(self, switch, path=''):
-        """
-        Adds a command line switch to the spice tool command line call. The following options are available for LTSpice:
+        Validates a command line switch. The following options are available for LTSpice:
 
             * 'alt' : Set solver to Alternate.
 
             * 'ascii'     : Use ASCII.raw files. Seriously degrades program performance.
 
             * 'encrypt'   : Encrypt a model library.For 3rd parties wishing to allow people to use libraries without
-            revealing implementation details. Not used by AnalogDevices models.
+                            revealing implementation details. Not used by AnalogDevices models.
 
             * 'fastaccess': Batch conversion of a binary.rawfile to Fast Access format.
 
-            * 'FixUpSchematicFonts'  : Convert the font size field of very old user - authored schematic text to the
-            modern default.
+            * 'FixUpSchematicFonts' : Convert the font size field of very old user - authored schematic text to the
+                                    modern default.
 
             * 'FixUpSymbolFonts' : Convert the font size field of very old user - authored symbols to the modern
-            default. See Changelog.txt for application hints.
+                default. See Changelog.txt for application hints.
 
             * 'ini <path>' : Specify an .ini file to use other than %APPDATA%\LTspice.ini
 
             * 'I<path>' : Specify a path to insert in the symbol and file search paths. Must be the last specified
-            option.
+                option.
 
             * 'netlist'   :  Batch conversion of a schematic to a netlist.
 
             * 'normal'    :  Set solver to Normal.
 
             * 'PCBnetlist':  Batch conversion of a schematic to a PCB format netlist.
 
@@ -168,48 +129,50 @@
 
             * 'sync'      : Update component libraries
 
             * 'uninstall' :  Executes one step of the uninstallation process. Please don't.
 
 
         :param switch: switch to be added. If the switch is not on the list above, it should be correctly formatted with
-        the preceeding '-' switch
-        :type switch:
+                       the preceding '-' switch
+        :type switch: str
         :param path: path to the file related to the switch being given.
         :type path: str, optional
-        :return:
-        :rtype:
+        :return: Nothing
+        :rtype: None
         """
-        if switch in self.ltspice_args:
-            switches = self.ltspice_args[switch]
-            switches = [switch.replace('{path}', path) for switch in switches]
-            self.cmdline_switches.extend(switches)
+        if switch in cls.ltspice_args:
+            switches = cls.ltspice_args[switch]
+            switches = [switch.replace('<path>', path) for switch in switches]
+            return switches
         else:
-            self.cmdline_switches.append(switch)
-            if path is not None:
-                self.cmdline_switches.append(path)
+            raise ValueError("Invalid switch for class ")
 
-    def run(self, netlist_file, timeout):
+    @classmethod
+    def run(cls, netlist_file, cmd_line_switches, timeout):
         if sys.platform == 'darwin':
-            cmd_run = self.spice_exe + ['-b'] + [netlist_file] + self.cmdline_switches
+            cmd_run = cls.spice_exe + ['-b'] + [netlist_file] + cmd_line_switches
         else:
-            cmd_run = self.spice_exe + ['-Run'] + ['-b'] + [netlist_file] + self.cmdline_switches
+            cmd_run = cls.spice_exe + ['-Run'] + ['-b'] + [netlist_file] + cmd_line_switches
         # start execution
         return run_function(cmd_run, timeout=timeout)
 
-    def create_netlist(self, circuit_file):
+    @classmethod
+    def create_netlist(cls, circuit_file: Union[str, Path]) -> Path:
         # prepare instructions, two stages used to enable edits on the netlist w/o open GUI
         # see: https://www.mikrocontroller.net/topic/480647?goto=5965300#5965300
-
+        circuit_file = Path(circuit_file)
         if sys.platform == 'darwin':
             NotImplementedError("In this platform LTSpice doesn't have netlist generation capabilities")
-        cmd_netlist = self.spice_exe + ['-netlist'] + [circuit_file]
-        return run_function(cmd_netlist)
-
-    def kill_all(self):
-        import psutil
-        for proc in psutil.process_iter():
-            # check whether the process name matches
-
-            if proc.name() == self.process_name:
-                print("killing ltspice", proc.pid)
-                proc.kill()
+        cmd_netlist = cls.spice_exe + ['-netlist'] + [circuit_file.as_posix()]
+        # print(f'Creating netlist file from "{circuit_file}"', end='...')
+        error = run_function(cmd_netlist)
+
+        if error == 0:
+            netlist = circuit_file.with_suffix('.net')
+            if netlist.exists():
+                print("OK")
+                return netlist
+        msg = "Failed to create netlist"
+        # print(msg)
+        logging.error(msg)
+        raise RuntimeError(msg)
```

### Comparing `PyLTSpice-3.1/PyLTSpice/sweep_iterators.py` & `PyLTSpice-4.0/PyLTSpice/utils/sweep_iterators.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-3.1/PyLTSpice.egg-info/PKG-INFO` & `PyLTSpice-4.0/PyLTSpice/PyLTSpice.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: PyLTSpice
-Version: 3.1
+Version: 4.0
 Summary: A set of tools to Automate LTSpice simulations
-Home-page: https://github.com/nunobrum/PyLTSpice
-Author: Nuno Brum
 Author-email: Nuno Brum <me@nunobrum.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -692,68 +690,74 @@
 # README #
 
 PyLTSpice is a toolchain of python utilities design to interact with LTSpice and NGSpice Electronic Simulator.
 
 ## What is contained in this repository ##
 
 * __LTSteps.py__
-An utility that extracts from LTSpice output files data, and formats it for import in a spreadsheet, such like Excel or Calc.
+  An utility that extracts from LTSpice output files data, and formats it for import in a spreadsheet, such like Excel
+  or Calc.
 
 * __raw_read.py__
-A pure python class that serves to read raw files into a python class.
+  A pure python class that serves to read raw files into a python class.
 
 * __raw_write.py__
-A class to write RAW files that can be read by LTSpice Wave Application.
+  A class to write RAW files that can be read by LTSpice Wave Application.
 
 * __Histogram.py__
-A python script that uses numpy and matplotlib to create an histogram and calculate the sigma deviations. This is useful for Monte-Carlo analysis.
+  A python script that uses numpy and matplotlib to create an histogram and calculate the sigma deviations. This is
+  useful for Monte-Carlo analysis.
 
 * __sim_batch.py__
-This is a script to launch Spice Simulations. This is useful because:
+  This is a script to launch Spice Simulations. This is useful because:
 
     - Can overcome the limitation of only stepping 3 parameters
     - Different types of simulations .TRAN .AC .NOISE can be run in a single batch
     - The RAW Files are smaller and easier to treat
     - When used with the RawRead.py and LTSteps.py, validation of the circuit can be done automatically.
     - Different models can be simulated in a single batch, by using the following instructions:
-        - `set_element_model('D1', '1N4148') # Replaces the Diode D1 with the model 1N4148 `  
-        - `set_component_value('R2', '33k') # Replaces the value of R2 by 33k`  
-        - `set_parameters(run=1, TEMP=80) # Creates or updates the netlist to have .PARAM run=1 or .PARAM TEMP=80`  
-        - `add_instructions(".STEP run -1 1023 1", ".dc V1 -5 5") `  
-        - `remove_instruction(".STEP run -1 1023 1")  # Removes previously added instruction`  
-        - `reset_netlist() # Resets all edits done to the netlist.`  
+        - `set_element_model('D1', '1N4148') # Replaces the Diode D1 with the model 1N4148 `
+        - `set_component_value('R2', '33k') # Replaces the value of R2 by 33k`
+        - `set_parameters(run=1, TEMP=80) # Creates or updates the netlist to have .PARAM run=1 or .PARAM TEMP=80`
+        - `add_instructions(".STEP run -1 1023 1", ".dc V1 -5 5") `
+        - `remove_instruction(".STEP run -1 1023 1")  # Removes previously added instruction`
+        - `reset_netlist() # Resets all edits done to the netlist.`
 
-    Note: It was only tested with Windows based installations.
+  Note: It was only tested with Windows based installations.
 
 ## How to Install ##
-`pip install PyLTSpice `  
+
+`pip install PyLTSpice `
 
 ### Updating PyLTSpice ###
- `pip install --upgrade PyLTSpice `  
+
+`pip install --upgrade PyLTSpice `
 
 ### Using GITHub ###
 
- `git clone https://github.com/nunobrum/PyLTSpice.git `  
+`git clone https://github.com/nunobrum/PyLTSpice.git `
 
 If using this method it would be good to add the path where you cloned the site to python path.
 
- `import sys `  
- `sys.path.append(<path to PyLTSpice>) `  
+`import sys `  
+`sys.path.append(<path to PyLTSpice>) `
 
 ## How to use ##
 
 Here follows a quick outlook on how to use each of the tools.
 
 More comprehensive documentation can be found in https://pyltspice.readthedocs.io/en/latest/
 
 ## LICENSE ##
+
 GNU V3 License
 (refer to the LICENSE file)
 
 ### raw_read.py ###
+
 The example below reads the data from a Spice Simulation called
 "TRAN - STEP.raw" and displays all steps of the "I(R1)" trace in a matplotlib plot
 
  ```python
 from PyLTSpice import RawRead
 
 from matplotlib import pyplot as plt
@@ -764,97 +768,107 @@
 print(LTR.get_raw_property())
 
 IR1 = LTR.get_trace("I(R1)")
 x = LTR.get_trace('time')  # Gets the time axis
 steps = LTR.get_steps()
 for step in range(len(steps)):
     # print(steps[step])
-    plt.plot(x.get_time_axis(step), IR1.get_wave(step), label=steps[step])
+    plt.plot(x.get_wave(step), IR1.get_wave(step), label=steps[step])
 
 plt.legend()  # order a legend
 plt.show()
  ```   
 
 ### raw_write.py ###
-The following example writes a RAW file with a 3 milliseconds transient simulation sine with a
-10kHz and a cosine with 9.997kHz
+
+The following example writes a RAW file with a 3 milliseconds transient simulation sine with a 10kHz and a cosine with
+9.997kHz
+
  ```python
 import numpy as np
 from PyLTSpice import Trace, RawWrite
 
-LW = RawWrite()
+LW = RawWrite(fastacces=False)
 tx = Trace('time', np.arange(0.0, 3e-3, 997E-11))
 vy = Trace('N001', np.sin(2 * np.pi * tx.data * 10000))
 vz = Trace('N002', np.cos(2 * np.pi * tx.data * 9970))
 LW.add_trace(tx)
 LW.add_trace(vy)
 LW.add_trace(vz)
-LW.save("teste_w.raw")
-
+LW.save("teste_snippet1.raw")
  ```   
 
-
 ### sim_batch.py ###
-This module is used to launch LTSPice simulations. Results then can be processed with either the RawRead
-or with the LTSteps module to read the log file which can contain .MEAS results.
 
-The script will firstly invoke the LTSpice in command line to generate a netlist, and then this netlist can be
-updated directly by the script, in order to change component values, parameters or simulation commands.
+This module is used to launch LTSPice simulations. Results then can be processed with either the RawRead or with the
+LTSteps module to read the log file which can contain .MEAS results.
+
+The script will firstly invoke the LTSpice in command line to generate a netlist, and then this netlist can be updated
+directly by the script, in order to change component values, parameters or simulation commands.
 
 Here follows an example of operation.
 
 ```python
-import os
-from PyLTSpice import SimCommander
-
-def processing_data(raw_file, log_file):
-    print("Handling the simulation data of %s, log file %s" % (raw_file, log_file))
+from PyLTSpice import SimRunner
+from PyLTSpice import SpiceEditor
 
 # select spice model
-LTC = SimCommander("Batch_Test.asc")
+LTC = SimRunner(output_folder='./temp')
+LTC.create_netlist('Batch_Test.asc')
+netlist = SpiceEditor('Batch_Test.net')
 # set default arguments
-LTC.set_parameters(res=0, cap=100e-6)
-LTC.set_component_value('R2', '2k')
-LTC.set_component_value('R1', '4k')
-LTC.set_element_model('V3', "SINE(0 1 3k 0 0 0)")
-# define simulation
-LTC.add_instructions(
-    "; Simulation settings",
-    ".param run = 0"
+netlist.set_parameters(res=0, cap=100e-6)
+netlist.set_component_value('R2', '2k')  # Modifying the value of a resistor
+netlist.set_component_value('R1', '4k')
+netlist.set_element_model('V3', "SINE(0 1 3k 0 0 0)")  # Modifying the
+netlist.set_component_value('XU1:C2', 20e-12)  # modifying a define simulation
+netlist.add_instructions(
+        "; Simulation settings",
+        ".param run = 0"
 )
 
 for opamp in ('AD712', 'AD820'):
-    LTC.set_element_model('XU1', opamp)
+    netlist.set_element_model('XU1', opamp)
     for supply_voltage in (5, 10, 15):
-        LTC.set_component_value('V1', supply_voltage)
-        LTC.set_component_value('V2', -supply_voltage)
-        # overriding he automatic netlist naming
-        run_netlist_file = "{}_{}_{}.net".format(LTC.circuit_radic, opamp, supply_voltage)
-        LTC.run(run_filename=run_netlist_file, callback=processing_data)
-
-
-LTC.reset_netlist()
-LTC.add_instructions(
-    "; Simulation settings",
-    ".ac dec 30 10 1Meg",
-    ".meas AC Gain MAX mag(V(out)) ; find the peak response and call it ""Gain""",
-    ".meas AC Fcut TRIG mag(V(out))=Gain/sqrt(2) FALL=last"
+        netlist.set_component_value('V1', supply_voltage)
+        netlist.set_component_value('V2', -supply_voltage)
+        print("simulating OpAmp", opamp, "Voltage", supply_voltage)
+        LTC.run(netlist)
+
+for raw, log in LTC:
+    print("Raw file: %s, Log file: %s" % (raw, log))
+    # do something with the data
+    # raw_data = RawRead(raw)
+    # log_data = LTSteps(log)
+    # ...
+
+netlist.reset_netlist()
+netlist.add_instructions(
+        "; Simulation settings",
+        ".ac dec 30 10 1Meg",
+        ".meas AC Gain MAX mag(V(out)) ; find the peak response and call it ""Gain""",
+        ".meas AC Fcut TRIG mag(V(out))=Gain/sqrt(2) FALL=last"
 )
 
-LTC.run()
-LTC.wait_completion()
+# Sim Statistics
+print('Successful/Total Simulations: ' + str(LTC.okSim) + '/' + str(LTC.runno))
+
+enter = input("Press enter to delete created files")
+if enter == '':
+    LTC.file_cleanup()
 
 # Sim Statistics
 print('Successful/Total Simulations: ' + str(LTC.okSim) + '/' + str(LTC.runno))
 ```
 
 ### LTSteps.py ###
-This module defines a class that can be used to parse LTSpice log files where the information about .STEP information is written.
-There are two possible usages of this module, either programmatically by importing the module and then accessing data through the
-class as exemplified here:
+
+This module defines a class that can be used to parse LTSpice log files where the information about .STEP information is
+written. There are two possible usages of this module, either programmatically by importing the module and then
+accessing data through the class as exemplified here:
 
 ```python
 from PyLTSpice.LTSteps import LTSpiceLogReader
 
 data = LTSpiceLogReader("Batch_Test_AD820_15.log")
 
 print("Number of steps  :", data.step_count)
@@ -869,22 +883,24 @@
     print(' '.join([f"{data[step][i]:15}" for step in step_names]), end='')  # Print steps names with no new line
     print(' '.join([f"{data[name][i]:15}" for name in meas_names]), end='\n')  # Print Header
 
 print("Total number of measures found :", data.measure_count)
 ```
 
 The second possibility is to use the module directly on the command line
- `python -m PyLTSpice.LTSteps <filename> `
- The <filename> can be either be a log file (.log), a data export file (.txt) or a measurement output file (.meas)
- This will process all the data and export it automatically into a text file with the extension (tlog, tsv, tmeas)
- where the data read is formatted into a more convenient tab separated format.
- In case the <logfile> is not provided, the script will scan the directory and process the newest log, txt or out file found.
+`python -m PyLTSpice.LTSteps <filename> `
+The <filename> can be either be a log file (.log), a data export file (.txt) or a measurement output file (.meas)
+This will process all the data and export it automatically into a text file with the extension (tlog, tsv, tmeas)
+where the data read is formatted into a more convenient tab separated format. In case the <logfile> is not provided, the
+script will scan the directory and process the newest log, txt or out file found.
 
 ### Histogram.py ###
+
 This module uses the data inside on the filename to produce an histogram image.
+
  ```
 Usage: Histogram.py [options] LOG_FILE TRACE
 
 Options:
   --version             show program's version number and exit
   -h, --help            show this help message and exit
   -s SIGMA, --sigma=SIGMA
@@ -904,129 +920,161 @@
                         Range of the X axis to use for the histogram in the
                         form min:max. Example: -r -1:1
   -C, --clipboard       If the data from the clipboard is to be used.
   -i IMAGEFILE, --image=IMAGEFILE
                         Name of the image File. extension 'png'    
  ```
 
+### rawconvert.py ###
+
+A tool to convert .raw files into csv or Excel files.
+
+```
+Usage: raw_convert.py [options] <rawfile> <trace_list>
+
+Options:
+  --version             show program's version number and exit
+  -h, --help            show this help message and exit
+  -o FILE, --output=FILE
+                        Output file name. Use .csv for CSV output, .xlsx for
+                        Excel output
+  -c, --clipboard       Output to clipboard
+  -v, --verbose         Verbose output
+  -s SEPARATOR, --sep=SEPARATOR
+                        Value separator for CSV output. Default: "\t" <TAB>
+                        Example: -d ";"
+
+
+```
+
 ### SemiDevOpReader.py ###
-This module is used to read from LTSpice log files Semiconductor Devices Operating Point Information.
-A more detailed documentation is directly included in the source file docstrings.
+
+This module is used to read from LTSpice log files Semiconductor Devices Operating Point Information. A more detailed
+documentation is directly included in the source file docstrings.
 
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
-* Version 3.1\
-Supporting the new improved LTspice version from ADI. \
-Adding the get_wave() directly to the RawRead Class.
+
+* Version 4.0.0\
+  Separating the SimCommander into two separate classes, one for the spice netlist editing (SpiceEditor) and another for
+  the simulation execution (SimRunner).\
+  Implementing simulation server to allow for remote simulation execution and the respective client.\
+  Supporting Wiggler element in the new LTSpiceXVII.\
+  Renaming all files into lowercase.\
+  Creating Error classes for better error handling.\
+  Adding support for other simulators (ex: ngspice) where the simulator is defined by a class. This
+  support class needs to be a subclass of the abstract class Simulator.\
+  Enormous improvement in the documentation of the code.  
 
 * Version 3.0\
-Eliminating the LTSpice prefixes from files and classes.\
-Adopting the lowercase convention for filenames.
+  Eliminating the LTSpice prefixes from files and classes.\
+  Adopting the lowercase convention for filenames.
 
 * Version 2.3.1\
-Bug fix on the parameter replacement
+  Bug fix on the parameter replacement
 
 * Version 2.3\
-Supporting the creation of RAW Noise Analysis\
-Bug Fixes (See GitHub Log) 
+  Supporting the creation of RAW Noise Analysis\
+  Bug Fixes (See GitHub Log)
 
 * Version 2.2\
-Making numpy as an requirement and eliminating all code that avoided the use of numpy\
-Using new packaging tool\
-Fixes on the LTSpice_RawWrite\
-Fixes in the handling of stepped operating point simulations 
+  Making numpy as an requirement and eliminating all code that avoided the use of numpy\
+  Using new packaging tool\
+  Fixes on the LTSpice_RawWrite\
+  Fixes in the handling of stepped operating point simulations
 
 * Version 2.1\
-Adopting minimum python version 3.7\
-Starting to use unit tests to validate all modules and improving testbenches\
-Compatibility with NGSpice\
-Avoiding the use of setup.py as per PEP517 and PEP518\
-Bug Fixes (See GitHub log for more information)\
-Improvements on the management of stepped data in the LTSpice_RawRead.py
+  Adopting minimum python version 3.7\
+  Starting to use unit tests to validate all modules and improving testbenches\
+  Compatibility with NGSpice\
+  Avoiding the use of setup.py as per PEP517 and PEP518\
+  Bug Fixes (See GitHub log for more information)\
+  Improvements on the management of stepped data in the LTSpice_RawRead.py
 
 * Version 2.0.2\
-Improvements on Encoding detection
+  Improvements on Encoding detection
 
 * Version 2.0\
-International Support using the correct encoding when loading log files.\
-Code Optimizations on the LTSpice_RawReader that allow faster data loading.\
-Improving the functionality on the LTSpice_RawWriter.py\
-Adding support to editing components inside subcircuits (.subckt)\
-Supporting resistors with Model Definitions\
-Fixing problem with LTSpiceLogReader that would return messed up data\
-Fixing problem with replacing the file extension in certain names\
-Correcting problem with deprecations on the numpy functions used by the Histogram.py\
-Adding back the README.md that somehow was deleted
+  International Support using the correct encoding when loading log files.\
+  Code Optimizations on the LTSpice_RawReader that allow faster data loading.\
+  Improving the functionality on the LTSpice_RawWriter.py\
+  Adding support to editing components inside subcircuits (.subckt)\
+  Supporting resistors with Model Definitions\
+  Fixing problem with LTSpiceLogReader that would return messed up data\
+  Fixing problem with replacing the file extension in certain names\
+  Correcting problem with deprecations on the numpy functions used by the Histogram.py\
+  Adding back the README.md that somehow was deleted
 
 * Version 1.9\
-Adding support for µ character in the SpiceEditor.\
-Adding get_component_floatvalue() method in the netlist manipulating class that handles the conversion of 
-  numeric fields into a float. This function takes into account the engineering qualifiers 'k' for kilos, 'm' or milis, 
+  Adding support for µ character in the SpiceEditor.\
+  Adding get_component_floatvalue() method in the netlist manipulating class that handles the conversion of numeric
+  fields into a float. This function takes into account the engineering qualifiers 'k' for kilos, 'm' or milis,
   'u' or 'µ' for microns, 'n' for nanos, 'f' for femtos and 'Meg' for Megas.
 
 * Version 1.8\
-Uniforming License reference across files and improvements on the documentation\
-An enormous and wholehearted thanks to Logan Herrera (lpherr) <logan.herrera.github@gmail.com> for the improvements in the documentation.\
-Bugfix on the add_LTspiceRunCmdLineSwitches() ; Supporting .param name value format\
-Allowing the LTSpiceRawRead to proceed when the log file can't be found or when there are problems reading it.
+  Uniforming License reference across files and improvements on the documentation\
+  An enormous and wholehearted thanks to Logan Herrera (lpherr) <logan.herrera.github@gmail.com> for the improvements in
+  the documentation.\
+  Bugfix on the add_LTspiceRunCmdLineSwitches() ; Supporting .param name value format\
+  Allowing the LTSpiceRawRead to proceed when the log file can't be found or when there are problems reading it.
 * Version 1.7\
-Running in Linux under wine is now possible
+  Running in Linux under wine is now possible
 
 * Version 1.6\
-Adding LTSpice_RawWrite. Adding documentation.
+  Adding LTSpice_RawWrite. Adding documentation.
 
 * Version 1.5\
-Small fixes and improvements on the class usage. No added features
+  Small fixes and improvements on the class usage. No added features
 
 * Version 1.4 \
-Adding the LTSpice_SemiDevOpReader module\
-Re-enabling the Histogram functions which where disabled by mistake.
+  Adding the LTSpice_SemiDevOpReader module\
+  Re-enabling the Histogram functions which where disabled by mistake.
 
 * Version 1.3 \
-Bug fixes on the SpiceEditor Class
+  Bug fixes on the SpiceEditor Class
 
 * Version 1.2 \
-README.md:
-Adding link to readthedocs documentation\
-All files:
-Comprehensive documentation on how to use each module
+  README.md:
+  Adding link to readthedocs documentation\
+  All files:
+  Comprehensive documentation on how to use each module
 
 * Version 1.1\
-README.md:
-Updated the description\
-LTSpiceBatch.py:
-Corrected the name of the returned raw file.\
-Added comments throughout the code and cleanup
+  README.md:
+  Updated the description\
+  LTSpiceBatch.py:
+  Corrected the name of the returned raw file.\
+  Added comments throughout the code and cleanup
 
 * Version 1.0\
-LTSpiceBatch.py:
-Implemented an new approach (NOT BACKWARDS COMPATIBLE), that avoids the usage of the sim_settings.inc file.
-And allows to modify not only parameters, but also models and even the simulation commands.\
-LTSpice_RawRead.py:
-Added the get_time_axis method to the RawRead class to avoid the problems with negative values on
-time axis, when 2nd order compression is enabled in LTSpice.\
-LTSteps.py:
-Modified the LTSteps so it can also read measurements on log files without any steps done.
+  LTSpiceBatch.py:
+  Implemented an new approach (NOT BACKWARDS COMPATIBLE), that avoids the usage of the sim_settings.inc file. And allows
+  to modify not only parameters, but also models and even the simulation commands.\
+  LTSpice_RawRead.py:
+  Added the get_time_axis method to the RawRead class to avoid the problems with negative values on time axis, when 2nd
+  order compression is enabled in LTSpice.\
+  LTSteps.py:
+  Modified the LTSteps so it can also read measurements on log files without any steps done.
 
 
 * Version 0.6\
-Histogram.py now has an option to make the histogram directly from values stored in the clipboard
+  Histogram.py now has an option to make the histogram directly from values stored in the clipboard
 
 * Version 0.5\
-The LTSpice_RawReader.py now uses the struc.unpack function for a faster execution
+  The LTSpice_RawReader.py now uses the struc.unpack function for a faster execution
 
 * Version 0.4\
-Added LTSpiceBatch.py to the collection of tools
+  Added LTSpiceBatch.py to the collection of tools
 
 * Version 0.3\
-A version of LTSteps that can be imported to use in a higher level script 
+  A version of LTSteps that can be imported to use in a higher level script
 
 * Version 0.2\
-Adding LTSteps.py and Histogram.py
+  Adding LTSteps.py and Histogram.py
 
 * Version 0.1 \
-First commit to the bitbucket repository.
+  First commit to the bitbucket repository.
```

### Comparing `PyLTSpice-3.1/README.md` & `PyLTSpice-4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,74 @@
 # README #
 
 PyLTSpice is a toolchain of python utilities design to interact with LTSpice and NGSpice Electronic Simulator.
 
 ## What is contained in this repository ##
 
 * __LTSteps.py__
-An utility that extracts from LTSpice output files data, and formats it for import in a spreadsheet, such like Excel or Calc.
+  An utility that extracts from LTSpice output files data, and formats it for import in a spreadsheet, such like Excel
+  or Calc.
 
 * __raw_read.py__
-A pure python class that serves to read raw files into a python class.
+  A pure python class that serves to read raw files into a python class.
 
 * __raw_write.py__
-A class to write RAW files that can be read by LTSpice Wave Application.
+  A class to write RAW files that can be read by LTSpice Wave Application.
 
 * __Histogram.py__
-A python script that uses numpy and matplotlib to create an histogram and calculate the sigma deviations. This is useful for Monte-Carlo analysis.
+  A python script that uses numpy and matplotlib to create an histogram and calculate the sigma deviations. This is
+  useful for Monte-Carlo analysis.
 
 * __sim_batch.py__
-This is a script to launch Spice Simulations. This is useful because:
+  This is a script to launch Spice Simulations. This is useful because:
 
     - Can overcome the limitation of only stepping 3 parameters
     - Different types of simulations .TRAN .AC .NOISE can be run in a single batch
     - The RAW Files are smaller and easier to treat
     - When used with the RawRead.py and LTSteps.py, validation of the circuit can be done automatically.
     - Different models can be simulated in a single batch, by using the following instructions:
-        - `set_element_model('D1', '1N4148') # Replaces the Diode D1 with the model 1N4148 `  
-        - `set_component_value('R2', '33k') # Replaces the value of R2 by 33k`  
-        - `set_parameters(run=1, TEMP=80) # Creates or updates the netlist to have .PARAM run=1 or .PARAM TEMP=80`  
-        - `add_instructions(".STEP run -1 1023 1", ".dc V1 -5 5") `  
-        - `remove_instruction(".STEP run -1 1023 1")  # Removes previously added instruction`  
-        - `reset_netlist() # Resets all edits done to the netlist.`  
+        - `set_element_model('D1', '1N4148') # Replaces the Diode D1 with the model 1N4148 `
+        - `set_component_value('R2', '33k') # Replaces the value of R2 by 33k`
+        - `set_parameters(run=1, TEMP=80) # Creates or updates the netlist to have .PARAM run=1 or .PARAM TEMP=80`
+        - `add_instructions(".STEP run -1 1023 1", ".dc V1 -5 5") `
+        - `remove_instruction(".STEP run -1 1023 1")  # Removes previously added instruction`
+        - `reset_netlist() # Resets all edits done to the netlist.`
 
-    Note: It was only tested with Windows based installations.
+  Note: It was only tested with Windows based installations.
 
 ## How to Install ##
-`pip install PyLTSpice `  
+
+`pip install PyLTSpice `
 
 ### Updating PyLTSpice ###
- `pip install --upgrade PyLTSpice `  
+
+`pip install --upgrade PyLTSpice `
 
 ### Using GITHub ###
 
- `git clone https://github.com/nunobrum/PyLTSpice.git `  
+`git clone https://github.com/nunobrum/PyLTSpice.git `
 
 If using this method it would be good to add the path where you cloned the site to python path.
 
- `import sys `  
- `sys.path.append(<path to PyLTSpice>) `  
+`import sys `  
+`sys.path.append(<path to PyLTSpice>) `
 
 ## How to use ##
 
 Here follows a quick outlook on how to use each of the tools.
 
 More comprehensive documentation can be found in https://pyltspice.readthedocs.io/en/latest/
 
 ## LICENSE ##
+
 GNU V3 License
 (refer to the LICENSE file)
 
 ### raw_read.py ###
+
 The example below reads the data from a Spice Simulation called
 "TRAN - STEP.raw" and displays all steps of the "I(R1)" trace in a matplotlib plot
 
  ```python
 from PyLTSpice import RawRead
 
 from matplotlib import pyplot as plt
@@ -73,97 +79,107 @@
 print(LTR.get_raw_property())
 
 IR1 = LTR.get_trace("I(R1)")
 x = LTR.get_trace('time')  # Gets the time axis
 steps = LTR.get_steps()
 for step in range(len(steps)):
     # print(steps[step])
-    plt.plot(x.get_time_axis(step), IR1.get_wave(step), label=steps[step])
+    plt.plot(x.get_wave(step), IR1.get_wave(step), label=steps[step])
 
 plt.legend()  # order a legend
 plt.show()
  ```   
 
 ### raw_write.py ###
-The following example writes a RAW file with a 3 milliseconds transient simulation sine with a
-10kHz and a cosine with 9.997kHz
+
+The following example writes a RAW file with a 3 milliseconds transient simulation sine with a 10kHz and a cosine with
+9.997kHz
+
  ```python
 import numpy as np
 from PyLTSpice import Trace, RawWrite
 
-LW = RawWrite()
+LW = RawWrite(fastacces=False)
 tx = Trace('time', np.arange(0.0, 3e-3, 997E-11))
 vy = Trace('N001', np.sin(2 * np.pi * tx.data * 10000))
 vz = Trace('N002', np.cos(2 * np.pi * tx.data * 9970))
 LW.add_trace(tx)
 LW.add_trace(vy)
 LW.add_trace(vz)
-LW.save("teste_w.raw")
-
+LW.save("teste_snippet1.raw")
  ```   
 
-
 ### sim_batch.py ###
-This module is used to launch LTSPice simulations. Results then can be processed with either the RawRead
-or with the LTSteps module to read the log file which can contain .MEAS results.
 
-The script will firstly invoke the LTSpice in command line to generate a netlist, and then this netlist can be
-updated directly by the script, in order to change component values, parameters or simulation commands.
+This module is used to launch LTSPice simulations. Results then can be processed with either the RawRead or with the
+LTSteps module to read the log file which can contain .MEAS results.
+
+The script will firstly invoke the LTSpice in command line to generate a netlist, and then this netlist can be updated
+directly by the script, in order to change component values, parameters or simulation commands.
 
 Here follows an example of operation.
 
 ```python
-import os
-from PyLTSpice import SimCommander
-
-def processing_data(raw_file, log_file):
-    print("Handling the simulation data of %s, log file %s" % (raw_file, log_file))
+from PyLTSpice import SimRunner
+from PyLTSpice import SpiceEditor
 
 # select spice model
-LTC = SimCommander("Batch_Test.asc")
+LTC = SimRunner(output_folder='./temp')
+LTC.create_netlist('Batch_Test.asc')
+netlist = SpiceEditor('Batch_Test.net')
 # set default arguments
-LTC.set_parameters(res=0, cap=100e-6)
-LTC.set_component_value('R2', '2k')
-LTC.set_component_value('R1', '4k')
-LTC.set_element_model('V3', "SINE(0 1 3k 0 0 0)")
-# define simulation
-LTC.add_instructions(
-    "; Simulation settings",
-    ".param run = 0"
+netlist.set_parameters(res=0, cap=100e-6)
+netlist.set_component_value('R2', '2k')  # Modifying the value of a resistor
+netlist.set_component_value('R1', '4k')
+netlist.set_element_model('V3', "SINE(0 1 3k 0 0 0)")  # Modifying the
+netlist.set_component_value('XU1:C2', 20e-12)  # modifying a define simulation
+netlist.add_instructions(
+        "; Simulation settings",
+        ".param run = 0"
 )
 
 for opamp in ('AD712', 'AD820'):
-    LTC.set_element_model('XU1', opamp)
+    netlist.set_element_model('XU1', opamp)
     for supply_voltage in (5, 10, 15):
-        LTC.set_component_value('V1', supply_voltage)
-        LTC.set_component_value('V2', -supply_voltage)
-        # overriding he automatic netlist naming
-        run_netlist_file = "{}_{}_{}.net".format(LTC.circuit_radic, opamp, supply_voltage)
-        LTC.run(run_filename=run_netlist_file, callback=processing_data)
-
-
-LTC.reset_netlist()
-LTC.add_instructions(
-    "; Simulation settings",
-    ".ac dec 30 10 1Meg",
-    ".meas AC Gain MAX mag(V(out)) ; find the peak response and call it ""Gain""",
-    ".meas AC Fcut TRIG mag(V(out))=Gain/sqrt(2) FALL=last"
+        netlist.set_component_value('V1', supply_voltage)
+        netlist.set_component_value('V2', -supply_voltage)
+        print("simulating OpAmp", opamp, "Voltage", supply_voltage)
+        LTC.run(netlist)
+
+for raw, log in LTC:
+    print("Raw file: %s, Log file: %s" % (raw, log))
+    # do something with the data
+    # raw_data = RawRead(raw)
+    # log_data = LTSteps(log)
+    # ...
+
+netlist.reset_netlist()
+netlist.add_instructions(
+        "; Simulation settings",
+        ".ac dec 30 10 1Meg",
+        ".meas AC Gain MAX mag(V(out)) ; find the peak response and call it ""Gain""",
+        ".meas AC Fcut TRIG mag(V(out))=Gain/sqrt(2) FALL=last"
 )
 
-LTC.run()
-LTC.wait_completion()
+# Sim Statistics
+print('Successful/Total Simulations: ' + str(LTC.okSim) + '/' + str(LTC.runno))
+
+enter = input("Press enter to delete created files")
+if enter == '':
+    LTC.file_cleanup()
 
 # Sim Statistics
 print('Successful/Total Simulations: ' + str(LTC.okSim) + '/' + str(LTC.runno))
 ```
 
 ### LTSteps.py ###
-This module defines a class that can be used to parse LTSpice log files where the information about .STEP information is written.
-There are two possible usages of this module, either programmatically by importing the module and then accessing data through the
-class as exemplified here:
+
+This module defines a class that can be used to parse LTSpice log files where the information about .STEP information is
+written. There are two possible usages of this module, either programmatically by importing the module and then
+accessing data through the class as exemplified here:
 
 ```python
 from PyLTSpice.LTSteps import LTSpiceLogReader
 
 data = LTSpiceLogReader("Batch_Test_AD820_15.log")
 
 print("Number of steps  :", data.step_count)
@@ -178,22 +194,24 @@
     print(' '.join([f"{data[step][i]:15}" for step in step_names]), end='')  # Print steps names with no new line
     print(' '.join([f"{data[name][i]:15}" for name in meas_names]), end='\n')  # Print Header
 
 print("Total number of measures found :", data.measure_count)
 ```
 
 The second possibility is to use the module directly on the command line
- `python -m PyLTSpice.LTSteps <filename> `
- The <filename> can be either be a log file (.log), a data export file (.txt) or a measurement output file (.meas)
- This will process all the data and export it automatically into a text file with the extension (tlog, tsv, tmeas)
- where the data read is formatted into a more convenient tab separated format.
- In case the <logfile> is not provided, the script will scan the directory and process the newest log, txt or out file found.
+`python -m PyLTSpice.LTSteps <filename> `
+The <filename> can be either be a log file (.log), a data export file (.txt) or a measurement output file (.meas)
+This will process all the data and export it automatically into a text file with the extension (tlog, tsv, tmeas)
+where the data read is formatted into a more convenient tab separated format. In case the <logfile> is not provided, the
+script will scan the directory and process the newest log, txt or out file found.
 
 ### Histogram.py ###
+
 This module uses the data inside on the filename to produce an histogram image.
+
  ```
 Usage: Histogram.py [options] LOG_FILE TRACE
 
 Options:
   --version             show program's version number and exit
   -h, --help            show this help message and exit
   -s SIGMA, --sigma=SIGMA
@@ -213,129 +231,161 @@
                         Range of the X axis to use for the histogram in the
                         form min:max. Example: -r -1:1
   -C, --clipboard       If the data from the clipboard is to be used.
   -i IMAGEFILE, --image=IMAGEFILE
                         Name of the image File. extension 'png'    
  ```
 
+### rawconvert.py ###
+
+A tool to convert .raw files into csv or Excel files.
+
+```
+Usage: raw_convert.py [options] <rawfile> <trace_list>
+
+Options:
+  --version             show program's version number and exit
+  -h, --help            show this help message and exit
+  -o FILE, --output=FILE
+                        Output file name. Use .csv for CSV output, .xlsx for
+                        Excel output
+  -c, --clipboard       Output to clipboard
+  -v, --verbose         Verbose output
+  -s SEPARATOR, --sep=SEPARATOR
+                        Value separator for CSV output. Default: "\t" <TAB>
+                        Example: -d ";"
+
+
+```
+
 ### SemiDevOpReader.py ###
-This module is used to read from LTSpice log files Semiconductor Devices Operating Point Information.
-A more detailed documentation is directly included in the source file docstrings.
+
+This module is used to read from LTSpice log files Semiconductor Devices Operating Point Information. A more detailed
+documentation is directly included in the source file docstrings.
 
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
-* Version 3.1\
-Supporting the new improved LTspice version from ADI. \
-Adding the get_wave() directly to the RawRead Class.
+
+* Version 4.0.0\
+  Separating the SimCommander into two separate classes, one for the spice netlist editing (SpiceEditor) and another for
+  the simulation execution (SimRunner).\
+  Implementing simulation server to allow for remote simulation execution and the respective client.\
+  Supporting Wiggler element in the new LTSpiceXVII.\
+  Renaming all files into lowercase.\
+  Creating Error classes for better error handling.\
+  Adding support for other simulators (ex: ngspice) where the simulator is defined by a class. This
+  support class needs to be a subclass of the abstract class Simulator.\
+  Enormous improvement in the documentation of the code.  
 
 * Version 3.0\
-Eliminating the LTSpice prefixes from files and classes.\
-Adopting the lowercase convention for filenames.
+  Eliminating the LTSpice prefixes from files and classes.\
+  Adopting the lowercase convention for filenames.
 
 * Version 2.3.1\
-Bug fix on the parameter replacement
+  Bug fix on the parameter replacement
 
 * Version 2.3\
-Supporting the creation of RAW Noise Analysis\
-Bug Fixes (See GitHub Log) 
+  Supporting the creation of RAW Noise Analysis\
+  Bug Fixes (See GitHub Log)
 
 * Version 2.2\
-Making numpy as an requirement and eliminating all code that avoided the use of numpy\
-Using new packaging tool\
-Fixes on the LTSpice_RawWrite\
-Fixes in the handling of stepped operating point simulations 
+  Making numpy as an requirement and eliminating all code that avoided the use of numpy\
+  Using new packaging tool\
+  Fixes on the LTSpice_RawWrite\
+  Fixes in the handling of stepped operating point simulations
 
 * Version 2.1\
-Adopting minimum python version 3.7\
-Starting to use unit tests to validate all modules and improving testbenches\
-Compatibility with NGSpice\
-Avoiding the use of setup.py as per PEP517 and PEP518\
-Bug Fixes (See GitHub log for more information)\
-Improvements on the management of stepped data in the LTSpice_RawRead.py
+  Adopting minimum python version 3.7\
+  Starting to use unit tests to validate all modules and improving testbenches\
+  Compatibility with NGSpice\
+  Avoiding the use of setup.py as per PEP517 and PEP518\
+  Bug Fixes (See GitHub log for more information)\
+  Improvements on the management of stepped data in the LTSpice_RawRead.py
 
 * Version 2.0.2\
-Improvements on Encoding detection
+  Improvements on Encoding detection
 
 * Version 2.0\
-International Support using the correct encoding when loading log files.\
-Code Optimizations on the LTSpice_RawReader that allow faster data loading.\
-Improving the functionality on the LTSpice_RawWriter.py\
-Adding support to editing components inside subcircuits (.subckt)\
-Supporting resistors with Model Definitions\
-Fixing problem with LTSpiceLogReader that would return messed up data\
-Fixing problem with replacing the file extension in certain names\
-Correcting problem with deprecations on the numpy functions used by the Histogram.py\
-Adding back the README.md that somehow was deleted
+  International Support using the correct encoding when loading log files.\
+  Code Optimizations on the LTSpice_RawReader that allow faster data loading.\
+  Improving the functionality on the LTSpice_RawWriter.py\
+  Adding support to editing components inside subcircuits (.subckt)\
+  Supporting resistors with Model Definitions\
+  Fixing problem with LTSpiceLogReader that would return messed up data\
+  Fixing problem with replacing the file extension in certain names\
+  Correcting problem with deprecations on the numpy functions used by the Histogram.py\
+  Adding back the README.md that somehow was deleted
 
 * Version 1.9\
-Adding support for µ character in the SpiceEditor.\
-Adding get_component_floatvalue() method in the netlist manipulating class that handles the conversion of 
-  numeric fields into a float. This function takes into account the engineering qualifiers 'k' for kilos, 'm' or milis, 
+  Adding support for µ character in the SpiceEditor.\
+  Adding get_component_floatvalue() method in the netlist manipulating class that handles the conversion of numeric
+  fields into a float. This function takes into account the engineering qualifiers 'k' for kilos, 'm' or milis,
   'u' or 'µ' for microns, 'n' for nanos, 'f' for femtos and 'Meg' for Megas.
 
 * Version 1.8\
-Uniforming License reference across files and improvements on the documentation\
-An enormous and wholehearted thanks to Logan Herrera (lpherr) <logan.herrera.github@gmail.com> for the improvements in the documentation.\
-Bugfix on the add_LTspiceRunCmdLineSwitches() ; Supporting .param name value format\
-Allowing the LTSpiceRawRead to proceed when the log file can't be found or when there are problems reading it.
+  Uniforming License reference across files and improvements on the documentation\
+  An enormous and wholehearted thanks to Logan Herrera (lpherr) <logan.herrera.github@gmail.com> for the improvements in
+  the documentation.\
+  Bugfix on the add_LTspiceRunCmdLineSwitches() ; Supporting .param name value format\
+  Allowing the LTSpiceRawRead to proceed when the log file can't be found or when there are problems reading it.
 * Version 1.7\
-Running in Linux under wine is now possible
+  Running in Linux under wine is now possible
 
 * Version 1.6\
-Adding LTSpice_RawWrite. Adding documentation.
+  Adding LTSpice_RawWrite. Adding documentation.
 
 * Version 1.5\
-Small fixes and improvements on the class usage. No added features
+  Small fixes and improvements on the class usage. No added features
 
 * Version 1.4 \
-Adding the LTSpice_SemiDevOpReader module\
-Re-enabling the Histogram functions which where disabled by mistake.
+  Adding the LTSpice_SemiDevOpReader module\
+  Re-enabling the Histogram functions which where disabled by mistake.
 
 * Version 1.3 \
-Bug fixes on the SpiceEditor Class
+  Bug fixes on the SpiceEditor Class
 
 * Version 1.2 \
-README.md:
-Adding link to readthedocs documentation\
-All files:
-Comprehensive documentation on how to use each module
+  README.md:
+  Adding link to readthedocs documentation\
+  All files:
+  Comprehensive documentation on how to use each module
 
 * Version 1.1\
-README.md:
-Updated the description\
-LTSpiceBatch.py:
-Corrected the name of the returned raw file.\
-Added comments throughout the code and cleanup
+  README.md:
+  Updated the description\
+  LTSpiceBatch.py:
+  Corrected the name of the returned raw file.\
+  Added comments throughout the code and cleanup
 
 * Version 1.0\
-LTSpiceBatch.py:
-Implemented an new approach (NOT BACKWARDS COMPATIBLE), that avoids the usage of the sim_settings.inc file.
-And allows to modify not only parameters, but also models and even the simulation commands.\
-LTSpice_RawRead.py:
-Added the get_time_axis method to the RawRead class to avoid the problems with negative values on
-time axis, when 2nd order compression is enabled in LTSpice.\
-LTSteps.py:
-Modified the LTSteps so it can also read measurements on log files without any steps done.
+  LTSpiceBatch.py:
+  Implemented an new approach (NOT BACKWARDS COMPATIBLE), that avoids the usage of the sim_settings.inc file. And allows
+  to modify not only parameters, but also models and even the simulation commands.\
+  LTSpice_RawRead.py:
+  Added the get_time_axis method to the RawRead class to avoid the problems with negative values on time axis, when 2nd
+  order compression is enabled in LTSpice.\
+  LTSteps.py:
+  Modified the LTSteps so it can also read measurements on log files without any steps done.
 
 
 * Version 0.6\
-Histogram.py now has an option to make the histogram directly from values stored in the clipboard
+  Histogram.py now has an option to make the histogram directly from values stored in the clipboard
 
 * Version 0.5\
-The LTSpice_RawReader.py now uses the struc.unpack function for a faster execution
+  The LTSpice_RawReader.py now uses the struc.unpack function for a faster execution
 
 * Version 0.4\
-Added LTSpiceBatch.py to the collection of tools
+  Added LTSpiceBatch.py to the collection of tools
 
 * Version 0.3\
-A version of LTSteps that can be imported to use in a higher level script 
+  A version of LTSteps that can be imported to use in a higher level script
 
 * Version 0.2\
-Adding LTSteps.py and Histogram.py
+  Adding LTSteps.py and Histogram.py
 
 * Version 0.1 \
-First commit to the bitbucket repository.
+  First commit to the bitbucket repository.
```

