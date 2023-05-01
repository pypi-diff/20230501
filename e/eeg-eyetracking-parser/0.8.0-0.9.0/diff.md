# Comparing `tmp/eeg_eyetracking_parser-0.8.0.tar.gz` & `tmp/eeg_eyetracking_parser-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eeg_eyetracking_parser-0.8.0.tar", last modified: Mon Sep 26 08:45:57 2022, max compression
+gzip compressed data, was "eeg_eyetracking_parser-0.9.0.tar", last modified: Thu Oct  6 10:31:54 2022, max compression
```

## Comparing `eeg_eyetracking_parser-0.8.0.tar` & `eeg_eyetracking_parser-0.9.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      461 2022-09-26 08:45:46.320306 eeg_eyetracking_parser-0.8.0/eeg_eyetracking_parser/__init__.py
--rw-r--r--   0        0        0     4367 2022-09-26 08:45:46.324306 eeg_eyetracking_parser-0.8.0/eeg_eyetracking_parser/_custom_epochs.py
--rw-r--r--   0        0        0     3587 2022-09-26 08:45:46.324306 eeg_eyetracking_parser-0.8.0/eeg_eyetracking_parser/_data2bids.py
--rw-r--r--   0        0        0    14034 2022-09-26 08:45:46.324306 eeg_eyetracking_parser-0.8.0/eeg_eyetracking_parser/_eeg_preprocessing.py
--rw-r--r--   0        0        0    20590 2022-09-26 08:45:46.324306 eeg_eyetracking_parser-0.8.0/eeg_eyetracking_parser/_parsing.py
--rw-r--r--   0        0        0     2176 2022-09-26 08:45:46.324306 eeg_eyetracking_parser-0.8.0/eeg_eyetracking_parser/_triggers.py
--rw-r--r--   0        0        0    18897 2022-09-26 08:45:46.324306 eeg_eyetracking_parser-0.8.0/eeg_eyetracking_parser/braindecode_utils.py
--rw-r--r--   0        0        0      903 2022-09-26 08:45:46.324306 eeg_eyetracking_parser-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    14241 2022-09-26 08:45:46.324306 eeg_eyetracking_parser-0.8.0/readme.md
--rw-r--r--   0        0        0    14991 1970-01-01 00:00:00.000000 eeg_eyetracking_parser-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      483 2022-10-06 10:31:44.868044 eeg_eyetracking_parser-0.9.0/eeg_eyetracking_parser/__init__.py
+-rw-r--r--   0        0        0     5665 2022-10-06 10:31:44.868044 eeg_eyetracking_parser-0.9.0/eeg_eyetracking_parser/_custom_epochs.py
+-rw-r--r--   0        0        0     3587 2022-10-06 10:31:44.868044 eeg_eyetracking_parser-0.9.0/eeg_eyetracking_parser/_data2bids.py
+-rw-r--r--   0        0        0    14034 2022-10-06 10:31:44.868044 eeg_eyetracking_parser-0.9.0/eeg_eyetracking_parser/_eeg_preprocessing.py
+-rw-r--r--   0        0        0    20608 2022-10-06 10:31:44.868044 eeg_eyetracking_parser-0.9.0/eeg_eyetracking_parser/_parsing.py
+-rw-r--r--   0        0        0     2562 2022-10-06 10:31:44.868044 eeg_eyetracking_parser-0.9.0/eeg_eyetracking_parser/_time_frequency.py
+-rw-r--r--   0        0        0     2176 2022-10-06 10:31:44.868044 eeg_eyetracking_parser-0.9.0/eeg_eyetracking_parser/_triggers.py
+-rw-r--r--   0        0        0    20248 2022-10-06 10:31:44.868044 eeg_eyetracking_parser-0.9.0/eeg_eyetracking_parser/braindecode_utils.py
+-rw-r--r--   0        0        0      903 2022-10-06 10:31:44.868044 eeg_eyetracking_parser-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    14287 2022-10-06 10:31:44.868044 eeg_eyetracking_parser-0.9.0/readme.md
+-rw-r--r--   0        0        0    15037 1970-01-01 00:00:00.000000 eeg_eyetracking_parser-0.9.0/PKG-INFO
```

### Comparing `eeg_eyetracking_parser-0.8.0/eeg_eyetracking_parser/_data2bids.py` & `eeg_eyetracking_parser-0.9.0/eeg_eyetracking_parser/_data2bids.py`

 * *Files identical despite different names*

### Comparing `eeg_eyetracking_parser-0.8.0/eeg_eyetracking_parser/_eeg_preprocessing.py` & `eeg_eyetracking_parser-0.9.0/eeg_eyetracking_parser/_eeg_preprocessing.py`

 * *Files identical despite different names*

### Comparing `eeg_eyetracking_parser-0.8.0/eeg_eyetracking_parser/_parsing.py` & `eeg_eyetracking_parser-0.9.0/eeg_eyetracking_parser/_parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 from . import _eeg_preprocessing as epp
 
 logger = logging.getLogger('eeg_eyetracking_parser')
 
 
 @fnc.memoize(persistent=True)
 def read_subject(subject_nr, folder='data/', trigger_parser=None,
-                 eeg_margin=30, min_sacc_dur=10, min_sacc_size=30,
+                 eeg_margin=30, min_sacc_dur=10, min_sacc_size=100,
                  min_blink_dur=10, blink_annotation='BLINK',
                  saccade_annotation='SACCADE', eeg_preprocessing=True,
                  save_preprocessing_output=True, plot_preprocessing=True,
                  eye_kwargs={}, downsample_data_kwargs={},
                  drop_unused_channels_kwargs={}, 
                  rereference_channels_kwargs={}, create_eog_channels_kwargs={},
-                 set_montage_kwargs={}, annotate_emg_kwargs={}, band_pass_filter_kwargs={},
-                 autodetect_bad_channels_kwargs={}, run_ica_kwargs={},
-                 auto_select_ica_kwargs={}, interpolate_bads_kwargs={}):
+                 set_montage_kwargs={}, annotate_emg_kwargs={},
+                 band_pass_filter_kwargs={}, autodetect_bad_channels_kwargs={},
+                 run_ica_kwargs={}, auto_select_ica_kwargs={},
+                 interpolate_bads_kwargs={}):
     """Reads EEG, eye-tracking, and behavioral data for a single participant.
     This data should be organized according to the BIDS specification.
     
     EEG data is assumed to be in BrainVision data format (`.vhdr`, `.vmrk`,
     `.eeg`). Eye-tracking data is assumed to be in EyeLink data format (`.edf`
     or `.asc`). Behavioral data is assumed to be in `.csv` format.
```

### Comparing `eeg_eyetracking_parser-0.8.0/eeg_eyetracking_parser/_triggers.py` & `eeg_eyetracking_parser-0.9.0/eeg_eyetracking_parser/_triggers.py`

 * *Files identical despite different names*

### Comparing `eeg_eyetracking_parser-0.8.0/eeg_eyetracking_parser/braindecode_utils.py` & `eeg_eyetracking_parser-0.9.0/eeg_eyetracking_parser/braindecode_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,61 +53,67 @@
     epochs_query: str, optional
         A pandas-style query to select trials from the to-be-decoded epoch. The
         default assumes that there is a `practice` column from which we only
         want to have the 'no' values, i.e. that we want exclude practice
         trials.
     epochs: int, optional
         The number of training epochs, i.e. the number of times that the data
-        is fed into the model
+        is fed into the model. This should be at least 2.
     lesions: list of tuple or str
         A list of time windows or electrode names to be set to 0 during
         testing. A separate prediction is made for each lesion. Time windows
         are (start, end) tuples in sample units. Electrode names are strings.
     window_size_samples: int
         The length of the window to sample from the Epochs object. This should
         be slightly shorter than the actual Epochs to allow for jittered
         samples to be taken from the purpose of 'cropped decoding'.
     window_stride_samples: int
         The number of samples to jitter around the window for the purpose of
         cropped decoding.
     n_fold: int
-        The total number of splits (or folds)
+        The total number of splits (or folds). This should be at least 2.
     folder: str
         The folder in which the participant data is stored.
         
     Returns
     -------
     tuple
         A (results, metadata) tuple.
         
-        
         Results is a dict where keys are labels with 'overall' corresponding to
         the overall (unlesioned) test, and the other keys corresponding to the
         lesions as provided by the lesions parameter. Values are confusion
         matrices with shape (n_conditions, n_conditions) where the first
         dimension is the real label, and the second dimension is the predicted
         label.
         
         Metadata is a DataFrame corresponding to the dataset's metadata plus
         two additional columns: braindecode_label is numeric label that encodes
         the to-be-decoded factor, and braindecode_prediction is the predicted
         label. Rows where these two columns match were correctly decoded.
     """
+    if not isinstance(epochs, int) or epochs < 2:
+        raise ValueError('epochs should >= 2')
+    if not isinstance(n_fold, int) or epochs < 2:
+        raise ValueError('n_fold should >= 2')
     dataset, labels, metadata = read_decode_dataset(
         subject_nr, factors, epochs_kwargs, trigger, epochs_query,
         window_size=window_size, window_stride=window_stride, folder=folder)
     n_conditions = len(labels)
     results = {}
     results['overall'] = np.zeros((n_conditions, n_conditions))
     predictions = DataMatrix(length=0)
     for fold in range(n_fold):
         logger.info(f'subject {subject_nr}, fold {fold}')
         train_data, test_data = split_dataset(
-            dataset, fold=fold)
+            dataset, fold=fold, n_fold=n_fold)
         clf = train(train_data, test_data, epochs=epochs)
+        # We can unbalance the data after training to save time and to make the
+        # cell counts match again
+        unbalance_dataset(test_data)
         logger.info('Testing on complete data')
         # We want to know which trial was predicted to have which label. For
         # that reason, we create a datamatrix with true and predicted labels.
         # These are not in the original order, so we also store timestamps
         # so that later we can sort the datamatrix back into the original order
         y_pred = clf.predict(test_data)
         resized_pred = y_pred.copy()
@@ -146,16 +152,15 @@
 def read_decode_dataset(subject_nr, factors, epochs_kwargs, trigger,
                         epochs_query, lesion=None, window_size=200,
                         window_stride=1, folder='data'):
     """Reads a dataset and converts it to a format that is suitable for
     braindecode.
     """
     raw, events, metadata = _read_decode_subject(
-        subject_nr, folder=folder, save_preprocessing_output=False,
-        plot_preprocessing=False)
+        subject_nr, folder=folder, plot_preprocessing=False)
     epochs = mne.Epochs(raw, epoch_trigger(events, trigger),
                         metadata=metadata, **epochs_kwargs)
     epochs = epochs[epochs_query]
     metadata = metadata.query(epochs_query)
     if isinstance(lesion, tuple):
         epochs._data[:, :, lesion[0]:lesion[1]] = 0
     elif isinstance(lesion, str):
@@ -239,15 +244,14 @@
     tuple
         A (training set, test set) tuple
     """
     splitted = dataset.split({
         'train': [i for i in range(len(dataset.datasets)) if i % n_fold != fold],
         'test': [i for i in range(len(dataset.datasets)) if i % n_fold == fold]
     })
-    assert len(splitted['train']) > len(splitted['test'])
     return splitted['train'], splitted['test']
 
 
 def balance_dataset(dataset):
     """Makes sure that a dataset contains an equal number of observations for
     each label by randomly duplicating observations from labels that have too
     few observations. This modifies the dataset in-place.
@@ -263,23 +267,58 @@
             n_codes[code] = 0
         n_codes[code] += 1
     max_count = max(n_codes.values())
     for code, count in n_codes.items():
         n_add = max_count - count
         code_datasets = [d for d in dataset.datasets if d.y[0] == code]
         for i in range(n_add):
-            dataset.datasets.append(
-                copy.deepcopy(random.choice(code_datasets)))
-    # We need to update these property to keep the length of the dataset
-    # consistent, because they are used by the __len__() functions. Not clear
-    # what the different roles of the two different properties is. See also:
-    # https://github.com/pytorch/tnt/blob/master/torchnet/dataset/concatdataset.py
+            copied_dataset = copy.deepcopy(random.choice(code_datasets))
+            copied_dataset._is_balance_copy = True
+            dataset.datasets.append(copied_dataset)
+        if n_add:
+            logger.info(
+                f'adding {n_add} observations to code {code} to balance data')
+    update_dataset_size(dataset)
+
+
+def update_dataset_size(dataset):
+    """This updates properties of the dataset to keep the length consistent,
+    because they are used by the __len__() functions. Not clear what the
+    different roles of the two different properties is. See also:
+    
+    - https://github.com/pytorch/tnt/blob/master/torchnet/dataset/concatdataset.py
+    
+    This modifies the dataset in-place.
+
+    Parameters
+    ----------
+    dataset
+    """
     dataset.cum_sizes = np.cumsum([len(x) for x in dataset.datasets])
     dataset.cumulative_sizes = dataset.cum_sizes
-            
+
+
+def unbalance_dataset(dataset):
+    """Removes copied datasets that were add during balancing of the data. This
+    modifies the dataset in-place.
+
+    Parameters
+    ----------
+    dataset
+    """
+    to_remove = []
+    for d in dataset.datasets:
+        if hasattr(d, '_is_balance_copy') and d._is_balance_copy:
+            to_remove.append(d)
+    if not to_remove:
+        return
+    logger.info(f'removing {len(to_remove)} observations to unbalance data')
+    for d in to_remove:
+        dataset.datasets.remove(d)
+    update_dataset_size(dataset)
 
 def build_dataset(epochs, metadata, factors, window_size_samples,
                   window_stride_samples):
     """Creates a dataset that is suitable for braindecode from an Epochs
     object. This indirectly implements 'cropped decoding' as explained on
     the braindecode website and accompanying paper.
     
@@ -353,15 +392,18 @@
     model = ShallowFBCSPNet(
         n_chans,
         n_classes,
         input_window_samples=input_window_samples,
         final_conv_length='auto',
     )
     if torch.cuda.is_available():
+        logger.info('enabling cuda for gpu acceleration')
         model.cuda()
+    else:
+        logger.info('cuda is not available, not enabling gpu acceleration')
     to_dense_prediction_model(model)
     if test_set is None:
         train_split = None
         callbacks = None
     else:
         train_split = predefined_split(test_set)
         callbacks = [
```

### Comparing `eeg_eyetracking_parser-0.8.0/pyproject.toml` & `eeg_eyetracking_parser-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eeg_eyetracking_parser-0.8.0/readme.md` & `eeg_eyetracking_parser-0.9.0/readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 You can also convert the `PupilEpochs` object to a `SeriesColumn` and plot it that way, for example using `time_series_test.plot()`.
 
 ```python
 from datamatrix import convert as cnv
 import time_series_test as tst
 
 dm = cnv.from_pandas(metadata)
-dm.pupil = eet.epochs_to_series(dm, cue_epoch)
+dm.pupil = eet.epochs_to_series(dm, cue_epoch, baseline_trim=(-2, 2))
 tst.plot(dm, dv='pupil', hue_factor='cue_eccentricity')
 ```
 
 ## Installation
 
 ```
 pip install eeg_eyetracking_parser
@@ -190,29 +190,29 @@
 
 * **_Epochs:_**
 
   An mne.Epochs() object with autorejection applied.
 
 
 
-## <span style="color:purple">epochs\_to\_series</span>_(dm, epochs, baseline\_trim=(-2, 2))_
+## <span style="color:purple">epochs\_to\_series</span>_(dm, epochs, baseline\_trim=None)_
 
-Takes an Epochs or PupilEpochs object and converts it to a DataMatrix
-SeriesColumn. If a baseline has been specified in the epoch, it is applied
-to each row of the series separately. Rows where the mean baseline value
-(z-scored) is not within the range indicated by `baseline_trim` are set to
-`NAN`.
+Takes an Epochs, PupilEpochs, or EpochsTFR object and converts it to a
+DataMatrix SeriesColumn. If a baseline has been specified in the epoch, it
+is applied to each row of the series separately. Rows where the mean
+baseline value (z-scored) is not within the range indicated by
+`baseline_trim` are set to `NAN`.
 
 ### Parameters
 
 * **dm: DataMatrix**
 
   A DataMatrix object to which the series belongs
 
-* **epochs: Epochs or PupilEpochs**
+* **epochs: Epochs, PupilEpochs, or EpochsTFR**
 
   The source object with the epoch data.
 
 * **baseline\_trim: tuple of int, optional**
 
   The range of acceptable baseline values. This refers to z-scores.
 
@@ -249,15 +249,15 @@
 
 An Epochs class for the PupilSize channel. This allows baseline
 correction to be applied to pupil size, even though this channel is not a
 regular data channel.
 
 
 
-## <span style="color:purple">read\_subject</span>_(subject\_nr, folder='data/', trigger\_parser=None, eeg\_margin=30, min\_sacc\_dur=10, min\_sacc\_size=30, min\_blink\_dur=10, blink\_annotation='BLINK', saccade\_annotation='SACCADE', eeg\_preprocessing=True, save\_preprocessing\_output=True, plot\_preprocessing=True, eye\_kwargs={}, downsample\_data\_kwargs={}, drop\_unused\_channels\_kwargs={}, rereference\_channels\_kwargs={}, create\_eog\_channels\_kwargs={}, set\_montage\_kwargs={}, annotate\_emg\_kwargs={}, band\_pass\_filter\_kwargs={}, autodetect\_bad\_channels\_kwargs={}, run\_ica\_kwargs={}, auto\_select\_ica\_kwargs={}, interpolate\_bads\_kwargs={})_
+## <span style="color:purple">read\_subject</span>_(subject\_nr, folder='data/', trigger\_parser=None, eeg\_margin=30, min\_sacc\_dur=10, min\_sacc\_size=100, min\_blink\_dur=10, blink\_annotation='BLINK', saccade\_annotation='SACCADE', eeg\_preprocessing=True, save\_preprocessing\_output=True, plot\_preprocessing=True, eye\_kwargs={}, downsample\_data\_kwargs={}, drop\_unused\_channels\_kwargs={}, rereference\_channels\_kwargs={}, create\_eog\_channels\_kwargs={}, set\_montage\_kwargs={}, annotate\_emg\_kwargs={}, band\_pass\_filter\_kwargs={}, autodetect\_bad\_channels\_kwargs={}, run\_ica\_kwargs={}, auto\_select\_ica\_kwargs={}, interpolate\_bads\_kwargs={})_
 
 Reads EEG, eye-tracking, and behavioral data for a single participant.
 This data should be organized according to the BIDS specification.
 
 EEG data is assumed to be in BrainVision data format (`.vhdr`, `.vmrk`,
 `.eeg`). Eye-tracking data is assumed to be in EyeLink data format (`.edf`
 or `.asc`). Behavioral data is assumed to be in `.csv` format.
@@ -411,7 +411,8 @@
 
   A numpy array with events as expected by mne.Epochs().
 
 ## License
 
 `eeg_eyetracking_parser` is licensed under the [GNU General Public License
 v3](http://www.gnu.org/licenses/gpl-3.0.en.html).
+
```

### Comparing `eeg_eyetracking_parser-0.8.0/PKG-INFO` & `eeg_eyetracking_parser-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eeg_eyetracking_parser
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Python module for reading concurrently recorded EEG and eye-tracking data,
 Author-email: Hermine Berberyan <h.berberyan@rug.nl>, Wouter Kruijne <w.kruijne@rug.nl>, Sebastiaan Mathôt <s.mathot@cogsci.nl>, Ana Vilotjević <a.vilotijevic@rug.nl>
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: python-eyelinkparser
 Requires-Dist: mne
@@ -90,15 +90,15 @@
 You can also convert the `PupilEpochs` object to a `SeriesColumn` and plot it that way, for example using `time_series_test.plot()`.
 
 ```python
 from datamatrix import convert as cnv
 import time_series_test as tst
 
 dm = cnv.from_pandas(metadata)
-dm.pupil = eet.epochs_to_series(dm, cue_epoch)
+dm.pupil = eet.epochs_to_series(dm, cue_epoch, baseline_trim=(-2, 2))
 tst.plot(dm, dv='pupil', hue_factor='cue_eccentricity')
 ```
 
 ## Installation
 
 ```
 pip install eeg_eyetracking_parser
@@ -206,29 +206,29 @@
 
 * **_Epochs:_**
 
   An mne.Epochs() object with autorejection applied.
 
 
 
-## <span style="color:purple">epochs\_to\_series</span>_(dm, epochs, baseline\_trim=(-2, 2))_
+## <span style="color:purple">epochs\_to\_series</span>_(dm, epochs, baseline\_trim=None)_
 
-Takes an Epochs or PupilEpochs object and converts it to a DataMatrix
-SeriesColumn. If a baseline has been specified in the epoch, it is applied
-to each row of the series separately. Rows where the mean baseline value
-(z-scored) is not within the range indicated by `baseline_trim` are set to
-`NAN`.
+Takes an Epochs, PupilEpochs, or EpochsTFR object and converts it to a
+DataMatrix SeriesColumn. If a baseline has been specified in the epoch, it
+is applied to each row of the series separately. Rows where the mean
+baseline value (z-scored) is not within the range indicated by
+`baseline_trim` are set to `NAN`.
 
 ### Parameters
 
 * **dm: DataMatrix**
 
   A DataMatrix object to which the series belongs
 
-* **epochs: Epochs or PupilEpochs**
+* **epochs: Epochs, PupilEpochs, or EpochsTFR**
 
   The source object with the epoch data.
 
 * **baseline\_trim: tuple of int, optional**
 
   The range of acceptable baseline values. This refers to z-scores.
 
@@ -265,15 +265,15 @@
 
 An Epochs class for the PupilSize channel. This allows baseline
 correction to be applied to pupil size, even though this channel is not a
 regular data channel.
 
 
 
-## <span style="color:purple">read\_subject</span>_(subject\_nr, folder='data/', trigger\_parser=None, eeg\_margin=30, min\_sacc\_dur=10, min\_sacc\_size=30, min\_blink\_dur=10, blink\_annotation='BLINK', saccade\_annotation='SACCADE', eeg\_preprocessing=True, save\_preprocessing\_output=True, plot\_preprocessing=True, eye\_kwargs={}, downsample\_data\_kwargs={}, drop\_unused\_channels\_kwargs={}, rereference\_channels\_kwargs={}, create\_eog\_channels\_kwargs={}, set\_montage\_kwargs={}, annotate\_emg\_kwargs={}, band\_pass\_filter\_kwargs={}, autodetect\_bad\_channels\_kwargs={}, run\_ica\_kwargs={}, auto\_select\_ica\_kwargs={}, interpolate\_bads\_kwargs={})_
+## <span style="color:purple">read\_subject</span>_(subject\_nr, folder='data/', trigger\_parser=None, eeg\_margin=30, min\_sacc\_dur=10, min\_sacc\_size=100, min\_blink\_dur=10, blink\_annotation='BLINK', saccade\_annotation='SACCADE', eeg\_preprocessing=True, save\_preprocessing\_output=True, plot\_preprocessing=True, eye\_kwargs={}, downsample\_data\_kwargs={}, drop\_unused\_channels\_kwargs={}, rereference\_channels\_kwargs={}, create\_eog\_channels\_kwargs={}, set\_montage\_kwargs={}, annotate\_emg\_kwargs={}, band\_pass\_filter\_kwargs={}, autodetect\_bad\_channels\_kwargs={}, run\_ica\_kwargs={}, auto\_select\_ica\_kwargs={}, interpolate\_bads\_kwargs={})_
 
 Reads EEG, eye-tracking, and behavioral data for a single participant.
 This data should be organized according to the BIDS specification.
 
 EEG data is assumed to be in BrainVision data format (`.vhdr`, `.vmrk`,
 `.eeg`). Eye-tracking data is assumed to be in EyeLink data format (`.edf`
 or `.asc`). Behavioral data is assumed to be in `.csv` format.
@@ -428,7 +428,8 @@
   A numpy array with events as expected by mne.Epochs().
 
 ## License
 
 `eeg_eyetracking_parser` is licensed under the [GNU General Public License
 v3](http://www.gnu.org/licenses/gpl-3.0.en.html).
 
+
```

