# Comparing `tmp/pizurscan-0.1.1.tar.gz` & `tmp/pizurscan-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pizurscan-0.1.1.tar", last modified: Mon May  1 10:14:53 2023, max compression
+gzip compressed data, was "pizurscan-0.1.2.tar", last modified: Mon May  1 12:03:50 2023, max compression
```

## Comparing `pizurscan-0.1.1.tar` & `pizurscan-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 10:14:53.605965 pizurscan-0.1.1/
--rw-rw-rw-   0        0        0     1775 2023-05-01 10:14:53.604951 pizurscan-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1036 2023-05-01 07:49:26.000000 pizurscan-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 10:14:53.598667 pizurscan-0.1.1/pizurscan/
--rw-rw-rw-   0        0        0     5568 2023-05-01 06:55:20.000000 pizurscan-0.1.1/pizurscan/InputProcessor.py
--rw-rw-rw-   0        0        0     3997 2023-05-01 06:55:20.000000 pizurscan-0.1.1/pizurscan/OutputProcessor.py
--rw-rw-rw-   0        0        0     5430 2023-05-01 06:55:20.000000 pizurscan-0.1.1/pizurscan/PI_commands.py
--rw-rw-rw-   0        0        0     3620 2023-05-01 06:55:20.000000 pizurscan-0.1.1/pizurscan/Scanners.py
--rw-rw-rw-   0        0        0        0 2023-05-01 07:04:31.000000 pizurscan-0.1.1/pizurscan/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 10:14:53.603930 pizurscan-0.1.1/pizurscan.egg-info/
--rw-rw-rw-   0        0        0     1775 2023-05-01 10:14:53.000000 pizurscan-0.1.1/pizurscan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-05-01 10:14:53.000000 pizurscan-0.1.1/pizurscan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 10:14:53.000000 pizurscan-0.1.1/pizurscan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-01 10:14:53.000000 pizurscan-0.1.1/pizurscan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-01 10:14:53.000000 pizurscan-0.1.1/pizurscan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 10:14:53.605965 pizurscan-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1278 2023-05-01 09:46:15.000000 pizurscan-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:50.171589 pizurscan-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-01 12:03:50.171589 pizurscan-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-01 12:03:35.000000 pizurscan-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:50.171589 pizurscan-0.1.2/pizurscan/
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-05-01 12:03:35.000000 pizurscan-0.1.2/pizurscan/InputProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-01 12:03:35.000000 pizurscan-0.1.2/pizurscan/OutputProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-05-01 12:03:35.000000 pizurscan-0.1.2/pizurscan/PI_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-01 12:03:35.000000 pizurscan-0.1.2/pizurscan/Scanners.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:35.000000 pizurscan-0.1.2/pizurscan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:50.171589 pizurscan-0.1.2/pizurscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-01 12:03:50.000000 pizurscan-0.1.2/pizurscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-01 12:03:50.000000 pizurscan-0.1.2/pizurscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 12:03:50.000000 pizurscan-0.1.2/pizurscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-01 12:03:50.000000 pizurscan-0.1.2/pizurscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 12:03:50.000000 pizurscan-0.1.2/pizurscan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 12:03:50.171589 pizurscan-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-01 12:03:35.000000 pizurscan-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:03:50.171589 pizurscan-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    23152 2023-05-01 12:03:35.000000 pizurscan-0.1.2/tests/testclasses.py
```

### Comparing `pizurscan-0.1.1/PKG-INFO` & `pizurscan-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
-Name: pizurscan
-Version: 0.1.1
-Summary: Library to interface PI controllers and Zurich lock-in
-Home-page: https://pizur-scanner.readthedocs.io/
-Author: Giacomo Rizzi
-Author-email: rizzigiacomo@pm.me
-License: MIT
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-
-# pizur-scanner
-A library to execute one-dimensional continuous and discrete spatial scan with PI (Physik Intrumente) stepper motor and axis in combination with a lock-in Zurich implifier. In particular, with this library three main applications can be covered:
-- Input processing: input parameters for the axis scan, such as the scan edges and the step size, are processed to return the parameters to be inserted into the DAQ (data acquisition) of the Zurich lock-in. 
-- Scan execution: a connection with the PI controller that controls the stepper motor (and thus the motion of the axis) is established. A 1D continuous/discrete scan can be executed based on the scan parameters. 
-- Output Processing: as Input Processing stage sets the parameters of the DAQ acquisition of the Zurich instrument, post processing of the output Zurich data is performed in this last stage. Output data are "cleaned" from redundancy and the output file is eventually made of two columns; position and acquired signal, in a one-to-one relationship.  
+Metadata-Version: 2.1
+Name: pizurscan
+Version: 0.1.2
+Summary: Library to interface PI controllers and Zurich lock-in
+Home-page: https://pizur-scanner.readthedocs.io/
+Author: Giacomo Rizzi
+Author-email: rizzigiacomo@pm.me
+License: MIT
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+
+# pizur-scanner
+A library to execute one-dimensional continuous and discrete spatial scan with PI (Physik Intrumente) stepper motor and axis in combination with a lock-in Zurich implifier. In particular, with this library three main applications can be covered:
+- Input processing: input parameters for the axis scan, such as the scan edges and the step size, are processed to return the parameters to be inserted into the DAQ (data acquisition) of the Zurich lock-in. 
+- Scan execution: a connection with the PI controller that controls the stepper motor (and thus the motion of the axis) is established. A 1D continuous/discrete scan can be executed based on the scan parameters. 
+- Output Processing: as Input Processing stage sets the parameters of the DAQ acquisition of the Zurich instrument, post processing of the output Zurich data is performed in this last stage. Output data are "cleaned" from redundancy and the output file is eventually made of two columns; position and acquired signal, in a one-to-one relationship.
```

### Comparing `pizurscan-0.1.1/README.md` & `pizurscan-0.1.2/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,5 +1,5 @@
-# pizur-scanner
-A library to execute one-dimensional continuous and discrete spatial scan with PI (Physik Intrumente) stepper motor and axis in combination with a lock-in Zurich implifier. In particular, with this library three main applications can be covered:
-- Input processing: input parameters for the axis scan, such as the scan edges and the step size, are processed to return the parameters to be inserted into the DAQ (data acquisition) of the Zurich lock-in. 
-- Scan execution: a connection with the PI controller that controls the stepper motor (and thus the motion of the axis) is established. A 1D continuous/discrete scan can be executed based on the scan parameters. 
+# pizur-scanner
+A library to execute one-dimensional continuous and discrete spatial scan with PI (Physik Intrumente) stepper motor and axis in combination with a lock-in Zurich implifier. In particular, with this library three main applications can be covered:
+- Input processing: input parameters for the axis scan, such as the scan edges and the step size, are processed to return the parameters to be inserted into the DAQ (data acquisition) of the Zurich lock-in. 
+- Scan execution: a connection with the PI controller that controls the stepper motor (and thus the motion of the axis) is established. A 1D continuous/discrete scan can be executed based on the scan parameters. 
 - Output Processing: as Input Processing stage sets the parameters of the DAQ acquisition of the Zurich instrument, post processing of the output Zurich data is performed in this last stage. Output data are "cleaned" from redundancy and the output file is eventually made of two columns; position and acquired signal, in a one-to-one relationship.
```

### Comparing `pizurscan-0.1.1/pizurscan/OutputProcessor.py` & `pizurscan-0.1.2/pizurscan/OutputProcessor.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-import numpy as np 
-
-class OutputProcessor():
-
-    def __init__(self,filename,scan_pars,daq_pars):
-        """
-        Initialize an OutputProcessor object with the given filename, scan parameters, and DAQ parameters.
-
-        Args:
-        - filename (str): the name of the file containing the output data
-        - scan_pars (dict): a dictionary containing the scan parameters
-        - daq_pars (dict): a dictionary containing the DAQ parameters
-
-        Attributes:
-        - scan_pars (dict): a dictionary containing the scan parameters
-        - filename (str): the name of the file containing the output data
-        - daq_pars (dict): a dictionary containing the DAQ parameters
-        - N_rows (int): the number of rows in the DAQ data
-        - N_cols (int): the number of columns in the DAQ data
-        """
-        self.scan_pars = scan_pars
-        self.filename = filename
-        self.N_rows = daq_pars["daq_rows"]
-        self.N_cols = daq_pars["daq_columns"]
-
-    def get_raw_data(self):
-        """
-        Read raw data from the outputfile and return the third column, containing the values of the measured signal.
-
-        Returns:
-        - raw_data (ndarray): a NumPy array containing the third column of the input file
-        """
-        raw_data = np.genfromtxt(self.filename,skip_header = 1, delimiter = ";")
-        return raw_data[:,2] # third column contains all the data in a column     
-    
-    def evaluate_averaged_data(self,raw_data): 
-        """
-        Average the input data in case of a 1D discrete scan. Raw data is divided ini chunck of dimension N_cols, 
-        over which an average is performed. Output avg_data is in one to one relation with the spatial coordinates.
-
-        Args:
-        - raw_data (ndarray): a NumPy array containing the raw data
-
-        Returns:
-        - avg_data (ndarray): a NumPy array containing the averaged data
-        """
-        avg_data = np.empty(self.N_rows)
-        for row in range(self.N_rows):
-            avg_data[row] = np.mean(raw_data[row*self.N_cols:(row + 1)*self.N_cols])
-        return avg_data
-    
-    def evaluate_target_positions(self,scanedges,stepsize):
-        """
-        Evaluate the partition of the target points for a 1D scan.
-
-        Args:
-        - scanedges (list): a list containing the start and end positions of the scan
-        - stepsize (float): the step size of the scan
-
-        Returns:
-        - targets (ndarray): a NumPy array containing the target positions
-        """
-        # calculate targets points
-        Npoints = int(abs((scanedges[1]-scanedges[0]))/stepsize) + 1
-        return np.linspace(scanedges[0],scanedges[1],Npoints,endpoint=  True)
-
-    def save_data_file(self,targets,avg_data):         
-        """
-        Save the cleaned 1D data to a file named "cleaned_1D_data.txt".
-
-        Args:
-        - targets (ndarray): a NumPy array containing the target positions
-        - avg_data (ndarray): a NumPy array containing the averaged data
-        """
-        out_name = "cleaned_1D_data.txt"
-        out_file = np.column_stack((targets,avg_data))
-        np.savetxt(out_name, out_file, fmt = "%10.6f", delimiter = ",")
-
-    def save_processed_data(self):
-        """
-        Process the 1D data, averaging it if necessary (discrete scan), and save it to a file named "cleaned_1D_data.txt".
-        """
-        # get targets position
-        scanedges = self.scan_pars["scan_edges"]
-        stepsize = self.scan_pars["stepsize"]
-        targets = self.evaluate_target_positions(scanedges,stepsize)  
-        # get out_data
-        raw_data = self.get_raw_data()
-        if (self.scan_pars["type"] == "discrete"):
-            out_data = self.evaluate_averaged_data(raw_data, )
-        else: 
-            out_data = raw_data
-        # save data
-        self.save_data_file(targets,out_data)
-
-            
-        
-               
-        
-        
-
-
-    
-
+import numpy as np 
+
+class OutputProcessor():
+
+    def __init__(self,filename,scan_pars,daq_pars):
+        """
+        Initialize an OutputProcessor object with the given filename, scan parameters, and DAQ parameters.
+
+        Args:
+        - filename (str): the name of the file containing the output data
+        - scan_pars (dict): a dictionary containing the scan parameters
+        - daq_pars (dict): a dictionary containing the DAQ parameters
+
+        Attributes:
+        - scan_pars (dict): a dictionary containing the scan parameters
+        - filename (str): the name of the file containing the output data
+        - daq_pars (dict): a dictionary containing the DAQ parameters
+        - N_rows (int): the number of rows in the DAQ data
+        - N_cols (int): the number of columns in the DAQ data
+        """
+        self.scan_pars = scan_pars
+        self.filename = filename
+        self.N_rows = daq_pars["daq_rows"]
+        self.N_cols = daq_pars["daq_columns"]
+
+    def get_raw_data(self):
+        """
+        Read raw data from the outputfile and return the third column, containing the values of the measured signal.
+
+        Returns:
+        - raw_data (ndarray): a NumPy array containing the third column of the input file
+        """
+        raw_data = np.genfromtxt(self.filename,skip_header = 1, delimiter = ";")
+        return raw_data[:,2] # third column contains all the data in a column     
+    
+    def evaluate_averaged_data(self,raw_data): 
+        """
+        Average the input data in case of a 1D discrete scan. Raw data is divided ini chunck of dimension N_cols, 
+        over which an average is performed. Output avg_data is in one to one relation with the spatial coordinates.
+
+        Args:
+        - raw_data (ndarray): a NumPy array containing the raw data
+
+        Returns:
+        - avg_data (ndarray): a NumPy array containing the averaged data
+        """
+        avg_data = np.empty(self.N_rows)
+        for row in range(self.N_rows):
+            avg_data[row] = np.mean(raw_data[row*self.N_cols:(row + 1)*self.N_cols])
+        return avg_data
+    
+    def evaluate_target_positions(self,scanedges,stepsize):
+        """
+        Evaluate the partition of the target points for a 1D scan.
+
+        Args:
+        - scanedges (list): a list containing the start and end positions of the scan
+        - stepsize (float): the step size of the scan
+
+        Returns:
+        - targets (ndarray): a NumPy array containing the target positions
+        """
+        # calculate targets points
+        Npoints = int(abs((scanedges[1]-scanedges[0]))/stepsize) + 1
+        return np.linspace(scanedges[0],scanedges[1],Npoints,endpoint=  True)
+
+    def save_data_file(self,targets,avg_data):         
+        """
+        Save the cleaned 1D data to a file named "cleaned_1D_data.txt".
+
+        Args:
+        - targets (ndarray): a NumPy array containing the target positions
+        - avg_data (ndarray): a NumPy array containing the averaged data
+        """
+        out_name = "cleaned_1D_data.txt"
+        out_file = np.column_stack((targets,avg_data))
+        np.savetxt(out_name, out_file, fmt = "%10.6f", delimiter = ",")
+
+    def save_processed_data(self):
+        """
+        Process the 1D data, averaging it if necessary (discrete scan), and save it to a file named "cleaned_1D_data.txt".
+        """
+        # get targets position
+        scanedges = self.scan_pars["scan_edges"]
+        stepsize = self.scan_pars["stepsize"]
+        targets = self.evaluate_target_positions(scanedges,stepsize)  
+        # get out_data
+        raw_data = self.get_raw_data()
+        if (self.scan_pars["type"] == "discrete"):
+            out_data = self.evaluate_averaged_data(raw_data, )
+        else: 
+            out_data = raw_data
+        # save data
+        self.save_data_file(targets,out_data)
+
+            
+        
+               
+        
+        
+
+
+    
+
```

### Comparing `pizurscan-0.1.1/pizurscan/PI_commands.py` & `pizurscan-0.1.2/pizurscan/PI_commands.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,169 +1,169 @@
-from pipython import GCSDevice, pitools, GCS2Commands
-
-class Stepper:
-    """Represents an axis connected to a PI controller.
-
-    This class provides methods for connecting to and controlling the axis, 
-    including referencing the stage to a known position, moving the stage, 
-    querying the position, and configuring the output trigger.
-
-    Parameters
-    ----------
-    controller_ID : str
-        The ID of the PI controller to connect to.
-    axis_ID : str
-        The ID of the axis to control.
-
-    Attributes
-    ----------
-    pidevice : GCSDevice
-        The underlying PI device object.
-    controller_ID : str
-        The ID of the PI controller this axis is connected to.
-    axis_ID : str
-        The ID of this axis.
-    """
-
-    def __init__(self, controller_id, axis_id):
-        """Initializes the StepperChain class.
-
-        Parameters:
-        ----------
-        controller_id (str): The ID of the controller.
-        axis_id (int): The ID of the axis.
-        """
-        self.controller_id = controller_id
-        self.pidevice = GCSDevice(devname=self.controller_id)
-        self.axis_id = axis_id
-    
-    def usb_plugged_devices(self):
-        """
-        Returns a list with the devices plugged through USB.
-        
-        Returns:
-        --------
-        A list object with the indeces of the connected devices
-        """
-        return self.pidevice.EnumerateUSB(mask=self.controller_id)
-    
-    def connect_pidevice(self):
-        """
-        Activates an I/O interface to select the device of interest among the plugged ones.
-        Accepts a user input with the index of the device to interest and connects to it.
-        """
-        devices = self.usb_plugged_devices()
-        if not devices:
-            raise Exception("There are no plugged devices! Please connect at least one device.")
-        for i, device in enumerate(devices):
-            print('Number ---- Device')
-            print(f'{i}      ----  {device}')
-        # I/O for device selection
-        item = int(input('Input the index of the device to connect: '))
-        self.pidevice.ConnectUSB(devices[item])
-        pitools.startup(self.pidevice, self.axis_id)
-        
-    def move_stage_to_ref(self, refmode):
-        """
-        Moves the selected controller towards the reference position.
-        
-        Parameters
-        ----------
-        refmode : str
-            String defining the referencing position.
-        """
-        if refmode == 'FNL':
-            print("Moving stage towards negative edge...")
-            self.pidevice.FNL()
-        elif refmode == 'FPL':
-            print("Moving stage towards positive edge...")
-            self.pidevice.FPL()
-        pitools.waitontarget(self.pidevice)
-        print(f"Stage: {GCS2Commands.qCST(self.pidevice)['1']} successfully referenced.")
-    
-    def get_curr_pos(self):
-        """
-        Returns the current position of the axis
-        
-        Returns
-        --------
-        A float object with the current position of the stage
-
-        """
-        return self.pidevice.qPOS('1')
-
-    def set_velocity(self,velocity):
-        """ 
-        Set the velocity of motion in the ROM of the controller
-        
-        Parameters
-        ----------
-        velocity : float
-            Float defining the velocity of motion
-        """
-        self.pidevice.VEL('1',velocity)
-
-    def set_acceleration(self,acceleration):
-        """ 
-        Set the acceleration of motion in the ROM of the controller
-        
-        Parameters
-        ----------
-        acceleration : float
-            Float defining the acceleration of motion
-        """
-        self.pidevice.ACC('1',acceleration)
-        
-    def get_velocity(self):
-        """ 
-        Get and returns the velocity of the device
-        
-        Returns
-        ----------
-        velocity : float
-            Float defining the velocity of motion
-        """
-        velocity = GCS2Commands.qVEL(self.pidevice)['1']
-        return velocity
-
-    def get_acceleration(self):
-        """
-        Gets and returns the acceleration of the device
-               
-        Returns
-        --------
-        A float object defining the acceleration of motion
-        """
-        acceleration = GCS2Commands.qACC(self.pidevice)['1']
-        return acceleration
-
-        
-    def move_stage_to_target(self,target):
-        """ 
-        Moves the device to target position
-        
-        Parameters
-        ----------
-        target : float
-            Float defining the target position
-        """
-        self.pidevice.MOV(self.pidevice.axes,target)
-        pitools.waitontarget(self.pidevice)
-
-    def configure_out_trigger(self, trigger_type):
-        """Configures and sets the output trigger for a given axis.
-        
-        Parameters
-        ----------
-        trigger_type : int
-            Type of trigger to be output (6 == in Motion, 1 = Line trigger).
-        """
-        self.pidevice.CTO(1, 2, 1)
-        self.pidevice.CTO(1, 3, trigger_type)
-        # enable trigger output with the configuration defined above
-        self.pidevice.TRO(1, True)
-        
-    def close_connection(self):
-        """
-        Close the connection and reset the axis property
-        """
+from pipython import GCSDevice, pitools, GCS2Commands
+
+class Stepper:
+    """Represents an axis connected to a PI controller.
+
+    This class provides methods for connecting to and controlling the axis, 
+    including referencing the stage to a known position, moving the stage, 
+    querying the position, and configuring the output trigger.
+
+    Parameters
+    ----------
+    controller_ID : str
+        The ID of the PI controller to connect to.
+    axis_ID : str
+        The ID of the axis to control.
+
+    Attributes
+    ----------
+    pidevice : GCSDevice
+        The underlying PI device object.
+    controller_ID : str
+        The ID of the PI controller this axis is connected to.
+    axis_ID : str
+        The ID of this axis.
+    """
+
+    def __init__(self, controller_id, axis_id):
+        """Initializes the StepperChain class.
+
+        Parameters:
+        ----------
+        controller_id (str): The ID of the controller.
+        axis_id (int): The ID of the axis.
+        """
+        self.controller_id = controller_id
+        self.pidevice = GCSDevice(devname=self.controller_id)
+        self.axis_id = axis_id
+    
+    def usb_plugged_devices(self):
+        """
+        Returns a list with the devices plugged through USB.
+        
+        Returns:
+        --------
+        A list object with the indeces of the connected devices
+        """
+        return self.pidevice.EnumerateUSB(mask=self.controller_id)
+    
+    def connect_pidevice(self):
+        """
+        Activates an I/O interface to select the device of interest among the plugged ones.
+        Accepts a user input with the index of the device to interest and connects to it.
+        """
+        devices = self.usb_plugged_devices()
+        if not devices:
+            raise Exception("There are no plugged devices! Please connect at least one device.")
+        for i, device in enumerate(devices):
+            print('Number ---- Device')
+            print(f'{i}      ----  {device}')
+        # I/O for device selection
+        item = int(input('Input the index of the device to connect: '))
+        self.pidevice.ConnectUSB(devices[item])
+        pitools.startup(self.pidevice, self.axis_id)
+        
+    def move_stage_to_ref(self, refmode):
+        """
+        Moves the selected controller towards the reference position.
+        
+        Parameters
+        ----------
+        refmode : str
+            String defining the referencing position.
+        """
+        if refmode == 'FNL':
+            print("Moving stage towards negative edge...")
+            self.pidevice.FNL()
+        elif refmode == 'FPL':
+            print("Moving stage towards positive edge...")
+            self.pidevice.FPL()
+        pitools.waitontarget(self.pidevice)
+        print(f"Stage: {GCS2Commands.qCST(self.pidevice)['1']} successfully referenced.")
+    
+    def get_curr_pos(self):
+        """
+        Returns the current position of the axis
+        
+        Returns
+        --------
+        A float object with the current position of the stage
+
+        """
+        return self.pidevice.qPOS('1')
+
+    def set_velocity(self,velocity):
+        """ 
+        Set the velocity of motion in the ROM of the controller
+        
+        Parameters
+        ----------
+        velocity : float
+            Float defining the velocity of motion
+        """
+        self.pidevice.VEL('1',velocity)
+
+    def set_acceleration(self,acceleration):
+        """ 
+        Set the acceleration of motion in the ROM of the controller
+        
+        Parameters
+        ----------
+        acceleration : float
+            Float defining the acceleration of motion
+        """
+        self.pidevice.ACC('1',acceleration)
+        
+    def get_velocity(self):
+        """ 
+        Get and returns the velocity of the device
+        
+        Returns
+        ----------
+        velocity : float
+            Float defining the velocity of motion
+        """
+        velocity = GCS2Commands.qVEL(self.pidevice)['1']
+        return velocity
+
+    def get_acceleration(self):
+        """
+        Gets and returns the acceleration of the device
+               
+        Returns
+        --------
+        A float object defining the acceleration of motion
+        """
+        acceleration = GCS2Commands.qACC(self.pidevice)['1']
+        return acceleration
+
+        
+    def move_stage_to_target(self,target):
+        """ 
+        Moves the device to target position
+        
+        Parameters
+        ----------
+        target : float
+            Float defining the target position
+        """
+        self.pidevice.MOV(self.pidevice.axes,target)
+        pitools.waitontarget(self.pidevice)
+
+    def configure_out_trigger(self, trigger_type):
+        """Configures and sets the output trigger for a given axis.
+        
+        Parameters
+        ----------
+        trigger_type : int
+            Type of trigger to be output (6 == in Motion, 1 = Line trigger).
+        """
+        self.pidevice.CTO(1, 2, 1)
+        self.pidevice.CTO(1, 3, trigger_type)
+        # enable trigger output with the configuration defined above
+        self.pidevice.TRO(1, True)
+        
+    def close_connection(self):
+        """
+        Close the connection and reset the axis property
+        """
         self.pidevice.CloseConnection()
```

### Comparing `pizurscan-0.1.1/pizurscan/Scanners.py` & `pizurscan-0.1.2/pizurscan/Scanners.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,89 +1,88 @@
-from PI_commands import Stepper
-import numpy as np
-
-class Scan1D:
-    """A class to perform 1D continuous or discrete scans without the need to understand the 
-    lower level class Stepper 
-    """
-    def __init__(self,InPars):
-        """
-        Initialize Scan1D object with input parameters.
-
-        Args:
-            InPars (dict): Dictionary of input parameters containing the following keys:
-                - pi (dict): Dictionary of PI device information.
-                - scan_pars (dict): Dictionary of scan parameters containing the following keys:
-                    - scan_edges (tuple): Tuple of start and end positions of the scan.
-                    - stepsize (float): Step size of the scan.
-                    - velocity (float): Velocity of the scan.
-                    - acceleration (float): Acceleration of the scan.
-        """
-        self.PI = InPars["pi"]        
-        self.scan_pars = InPars["scan_pars"]
-        self.scan_edges = self.scan_pars["scan_edges"]
-        self.stepsize = self.scan_pars["stepsize"]
-        # evaluate target positions for the 1D scan
-        self.targets = self.evaluate_target_positions()
-        self.stepper = Stepper(self.PI["ID"],self.PI["stage_ID"]) 
-
-    def evaluate_target_positions(self):
-        """
-        Evaluate the partition of the target points for a 1D scan.
-
-        Returns:
-            numpy.ndarray: Array of target positions.
-        """
-        Npoints = int(abs(self.scan_edges[1]-self.scan_edges[0])/self.stepsize) + 1
-        return np.linspace(self.scan_edges[0],self.scan_edges[1],Npoints,endpoint=  True)
-
-    def connect_stepper(self):
-        """
-        Connect to the the PI device through a user-interface I/O.
-        """
-        self.stepper.connect_pidevice()
-    
-    def setup_motion_stepper(self):
-        """
-        Store input velocity and acceleration in the ROM of the device
-        """
-        self.stepper.set_velocity(self.scan_pars["velocity"])
-        self.stepper.set_acceleration(self.scan_pars["acceleration"])
-
-    def init_stepper_scan(self):
-        """ 
-        Setup the 1D scan in four steps:
-                        - acceleration and velocity are set to default values for quick refering and motion 
-                        - stage is moved to reference, either positive or negative depending on the input refmode
-                        - stage is moved to the first target point
-                        - output trigger is selected and activated
-        """
-        # high default values to obtain a quick referencing 
-        self.stepper.set_velocity(10)
-        self.stepper.set_acceleration(20)
-    
-        self.stepper.move_stage_to_ref(self.PI["refmode"])
-        self.stepper.move_stage_to_target(self.targets[0])
-        trigtype = self.PI["trig_type"]
-        self.stepper.configure_out_trigger(trigger_type=trigtype)
-
-    def execute_discrete_scan(self):
-        """
-        Execute the 1D discrete scan by moving the axis on all the target positions.
-
-        Returns:
-            list: List of current positions.
-        """
-        cur_pos = []
-        for target in self.targets:
-            self.stepper.move_stage_to_target(target)        
-            print("Position: ", target)
-            cur_pos.append(self.stepper.get_curr_pos())
-        return cur_pos
-
-    
-    def execute_continuous_scan(self):
-        """
-        Execute the continuous scan by moving the axis to the last position.
-        """
-        self.stepper.move_stage_to_target(self.targets[-1])        
+from PI_commands import Stepper
+import numpy as np
+
+class Scan1D:
+    """A class to perform 1D continuous or discrete scans without the need to understand the 
+    lower level class Stepper 
+    """
+    def __init__(self,InPars):
+        """
+        Initialize Scan1D object with input parameters.
+
+        Args:
+            InPars (dict): Dictionary of input parameters containing the following keys:
+                - pi (dict): Dictionary of PI device information.
+                - scan_pars (dict): Dictionary of scan parameters containing the following keys:
+                    - scan_edges (tuple): Tuple of start and end positions of the scan.
+                    - stepsize (float): Step size of the scan.
+                    - velocity (float): Velocity of the scan.
+                    - acceleration (float): Acceleration of the scan.
+        """
+        self.PI = InPars["pi"]        
+        self.scan_pars = InPars["scan_pars"]
+        self.scan_edges = self.scan_pars["scan_edges"]
+        self.stepsize = self.scan_pars["stepsize"]
+        self.targets = self.evaluate_target_positions()
+        self.stepper = Stepper(self.PI["ID"],self.PI["stage_ID"]) 
+
+    def evaluate_target_positions(self):
+        """
+        Evaluate the partition of the target points for a 1D scan.
+
+        Returns:
+            numpy.ndarray: Array of target positions.
+        """
+        Npoints = int(abs(self.scan_edges[1]-self.scan_edges[0])/self.stepsize) + 1
+        return np.linspace(self.scan_edges[0],self.scan_edges[1],Npoints,endpoint=  True)
+
+    def connect_stepper(self):
+        """
+        Connect to the the PI device through a user-interface I/O.
+        """
+        self.stepper.connect_pidevice()
+    
+    def setup_motion_stepper(self):
+        """
+        Store input velocity and acceleration in the ROM of the device
+        """
+        self.stepper.set_velocity(self.scan_pars["velocity"])
+        self.stepper.set_acceleration(self.scan_pars["acceleration"])
+
+    def init_stepper_scan(self):
+        """ 
+        Setup the 1D scan in four steps:
+                        - acceleration and velocity are set to default values for quick refering and motion 
+                        - stage is moved to reference, either positive or negative depending on the input refmode
+                        - stage is moved to the first target point
+                        - output trigger is selected and activated
+        """
+        # high default values to obtain a quick referencing 
+        self.stepper.set_velocity(10)
+        self.stepper.set_acceleration(20)
+    
+        self.stepper.move_stage_to_ref(self.PI["refmode"])
+        self.stepper.move_stage_to_target(self.targets[0])
+        trigtype = self.PI["trig_type"]
+        self.stepper.configure_out_trigger(trigger_type=trigtype)
+
+    def execute_discrete_scan(self):
+        """
+        Execute the 1D discrete scan by moving the axis on all the target positions.
+
+        Returns:
+            list: List of current positions.
+        """
+        cur_pos = []
+        for target in self.targets:
+            self.stepper.move_stage_to_target(target)        
+            print("Position: ", target)
+            cur_pos.append(self.stepper.get_curr_pos())
+        return cur_pos
+
+    
+    def execute_continuous_scan(self):
+        """
+        Execute the continuous scan by moving the axis to the last position.
+        """
+        self.stepper.move_stage_to_target(self.targets[-1])
```

### Comparing `pizurscan-0.1.1/pizurscan.egg-info/PKG-INFO` & `pizurscan-0.1.2/pizurscan.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
-Name: pizurscan
-Version: 0.1.1
-Summary: Library to interface PI controllers and Zurich lock-in
-Home-page: https://pizur-scanner.readthedocs.io/
-Author: Giacomo Rizzi
-Author-email: rizzigiacomo@pm.me
-License: MIT
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-
-# pizur-scanner
-A library to execute one-dimensional continuous and discrete spatial scan with PI (Physik Intrumente) stepper motor and axis in combination with a lock-in Zurich implifier. In particular, with this library three main applications can be covered:
-- Input processing: input parameters for the axis scan, such as the scan edges and the step size, are processed to return the parameters to be inserted into the DAQ (data acquisition) of the Zurich lock-in. 
-- Scan execution: a connection with the PI controller that controls the stepper motor (and thus the motion of the axis) is established. A 1D continuous/discrete scan can be executed based on the scan parameters. 
-- Output Processing: as Input Processing stage sets the parameters of the DAQ acquisition of the Zurich instrument, post processing of the output Zurich data is performed in this last stage. Output data are "cleaned" from redundancy and the output file is eventually made of two columns; position and acquired signal, in a one-to-one relationship.  
+Metadata-Version: 2.1
+Name: pizurscan
+Version: 0.1.2
+Summary: Library to interface PI controllers and Zurich lock-in
+Home-page: https://pizur-scanner.readthedocs.io/
+Author: Giacomo Rizzi
+Author-email: rizzigiacomo@pm.me
+License: MIT
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+
+# pizur-scanner
+A library to execute one-dimensional continuous and discrete spatial scan with PI (Physik Intrumente) stepper motor and axis in combination with a lock-in Zurich implifier. In particular, with this library three main applications can be covered:
+- Input processing: input parameters for the axis scan, such as the scan edges and the step size, are processed to return the parameters to be inserted into the DAQ (data acquisition) of the Zurich lock-in. 
+- Scan execution: a connection with the PI controller that controls the stepper motor (and thus the motion of the axis) is established. A 1D continuous/discrete scan can be executed based on the scan parameters. 
+- Output Processing: as Input Processing stage sets the parameters of the DAQ acquisition of the Zurich instrument, post processing of the output Zurich data is performed in this last stage. Output data are "cleaned" from redundancy and the output file is eventually made of two columns; position and acquired signal, in a one-to-one relationship.
```

