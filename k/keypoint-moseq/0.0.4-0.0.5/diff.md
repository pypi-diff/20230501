# Comparing `tmp/keypoint-moseq-0.0.4.tar.gz` & `tmp/keypoint-moseq-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keypoint-moseq-0.0.4.tar", last modified: Tue Apr 25 13:08:41 2023, max compression
+gzip compressed data, was "keypoint-moseq-0.0.5.tar", last modified: Mon May  1 16:41:52 2023, max compression
```

## Comparing `keypoint-moseq-0.0.4.tar` & `keypoint-moseq-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-25 13:08:41.336174 keypoint-moseq-0.0.4/
--rw-r--r--   0 calebweinreb   (501) staff       (20)     8355 2023-04-19 14:03:24.000000 keypoint-moseq-0.0.4/LICENSE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-04-19 14:03:24.000000 keypoint-moseq-0.0.4/NOTICE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-04-25 13:08:41.336442 keypoint-moseq-0.0.4/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1394 2023-04-23 11:46:01.000000 keypoint-moseq-0.0.4/README.md
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-25 13:08:41.333438 keypoint-moseq-0.0.4/keypoint_moseq/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      784 2023-04-25 13:04:51.000000 keypoint-moseq-0.0.4/keypoint_moseq/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    28353 2023-04-21 10:40:06.000000 keypoint-moseq-0.0.4/keypoint_moseq/analysis.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    17686 2023-04-19 14:03:24.000000 keypoint-moseq-0.0.4/keypoint_moseq/calibration.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    17163 2023-04-25 13:04:51.000000 keypoint-moseq-0.0.4/keypoint_moseq/fitting.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    32788 2023-04-23 11:46:01.000000 keypoint-moseq-0.0.4/keypoint_moseq/io.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    26851 2023-04-23 11:46:01.000000 keypoint-moseq-0.0.4/keypoint_moseq/util.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    66369 2023-04-25 13:04:51.000000 keypoint-moseq-0.0.4/keypoint_moseq/viz.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-04-25 13:08:41.335715 keypoint-moseq-0.0.4/keypoint_moseq.egg-info/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-04-25 13:08:41.000000 keypoint-moseq-0.0.4/keypoint_moseq.egg-info/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)      414 2023-04-25 13:08:41.000000 keypoint-moseq-0.0.4/keypoint_moseq.egg-info/SOURCES.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-04-25 13:08:41.000000 keypoint-moseq-0.0.4/keypoint_moseq.egg-info/dependency_links.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)      136 2023-04-25 13:08:41.000000 keypoint-moseq-0.0.4/keypoint_moseq.egg-info/requires.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2023-04-25 13:08:41.000000 keypoint-moseq-0.0.4/keypoint_moseq.egg-info/top_level.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       79 2023-04-25 13:08:41.337339 keypoint-moseq-0.0.4/setup.cfg
--rw-r--r--   0 calebweinreb   (501) staff       (20)      830 2023-04-25 13:07:50.000000 keypoint-moseq-0.0.4/setup.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-01 16:41:52.685750 keypoint-moseq-0.0.5/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     8355 2023-04-19 14:03:24.000000 keypoint-moseq-0.0.5/LICENSE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-04-19 14:03:24.000000 keypoint-moseq-0.0.5/NOTICE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-05-01 16:41:52.686016 keypoint-moseq-0.0.5/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1394 2023-04-23 11:46:01.000000 keypoint-moseq-0.0.5/README.md
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-01 16:41:52.664846 keypoint-moseq-0.0.5/keypoint_moseq/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      784 2023-04-25 13:04:51.000000 keypoint-moseq-0.0.5/keypoint_moseq/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    28353 2023-04-21 10:40:06.000000 keypoint-moseq-0.0.5/keypoint_moseq/analysis.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    17652 2023-05-01 16:41:29.000000 keypoint-moseq-0.0.5/keypoint_moseq/calibration.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    17495 2023-05-01 16:41:29.000000 keypoint-moseq-0.0.5/keypoint_moseq/fitting.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    32459 2023-05-01 16:41:29.000000 keypoint-moseq-0.0.5/keypoint_moseq/io.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    26681 2023-05-01 16:41:29.000000 keypoint-moseq-0.0.5/keypoint_moseq/util.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    66580 2023-05-01 16:41:29.000000 keypoint-moseq-0.0.5/keypoint_moseq/viz.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-01 16:41:52.685314 keypoint-moseq-0.0.5/keypoint_moseq.egg-info/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-05-01 16:41:52.000000 keypoint-moseq-0.0.5/keypoint_moseq.egg-info/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      414 2023-05-01 16:41:52.000000 keypoint-moseq-0.0.5/keypoint_moseq.egg-info/SOURCES.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-05-01 16:41:52.000000 keypoint-moseq-0.0.5/keypoint_moseq.egg-info/dependency_links.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      136 2023-05-01 16:41:52.000000 keypoint-moseq-0.0.5/keypoint_moseq.egg-info/requires.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2023-05-01 16:41:52.000000 keypoint-moseq-0.0.5/keypoint_moseq.egg-info/top_level.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       79 2023-05-01 16:41:52.686939 keypoint-moseq-0.0.5/setup.cfg
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      830 2023-05-01 16:41:29.000000 keypoint-moseq-0.0.5/setup.py
```

### Comparing `keypoint-moseq-0.0.4/LICENSE.md` & `keypoint-moseq-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.0.4/NOTICE.md` & `keypoint-moseq-0.0.5/NOTICE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.0.4/README.md` & `keypoint-moseq-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.0.4/keypoint_moseq/__init__.py` & `keypoint-moseq-0.0.5/keypoint_moseq/__init__.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.0.4/keypoint_moseq/analysis.py` & `keypoint-moseq-0.0.5/keypoint_moseq/analysis.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.0.4/keypoint_moseq/calibration.py` & `keypoint-moseq-0.0.5/keypoint_moseq/calibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     Parameters
     ----------
     confidences: dict
         Keypoint detection confidences for a collection of sessions 
 
     bodyparts: list
-        Label for each keypoint represented in ``confidences``
+        Label for each keypoint represented in `confidences`
 
     use_bodyparts: list
         Ordered subset of keypoint labels to be used for modeling
 
     num_bins: int, default=10
         Number of bins to use for enriching low-confidence keypoint
         detections. Confidence values for all used keypoints are 
@@ -89,15 +89,15 @@
 
     video_extension: str, default=None
         Preferred video extension (passed to :py:func:`keypoint_moseq.util.find_matching_videos`)
 
     Returns
     -------
     sample_keys: dict
-        Dictionary mapping elements from ``sample_keys`` to the
+        Dictionary mapping elements from `sample_keys` to the
         corresponding videos frames.
 
     """
     keys = sorted(set([k[0] for k in sample_keys]))
     videos = find_matching_videos(keys,video_dir)
     key_to_video = dict(zip(keys,videos))
     readers = {key: OpenCVReader(video) for key,video in zip(keys,videos)}
@@ -108,15 +108,15 @@
 def load_annotations(project_dir):
     """
     Reload saved calibration annotations.
 
     Parameters
     ----------
     project_dir: str
-        Load annotations from ``{project_dir}/error_annotations.csv``
+        Load annotations from `{project_dir}/error_annotations.csv`
 
     Returns
     -------
     annotations: dict
         Dictionary mapping sample keys to annotated keypoint 
         coordinates. (See :py:func:`keypoint_moseq.calibration.sample_error_frames` 
         for format of sample keys)
@@ -134,15 +134,15 @@
 def save_annotations(project_dir, annotations): 
     """
     Save calibration annotations to a csv file
 
     Parameters
     ----------
     project_dir: str
-        Save annotations to ``{project_dir}/error_annotations.csv`` 
+        Save annotations to `{project_dir}/error_annotations.csv` 
 
     annotations: dict
         Dictionary mapping sample keys to annotated keypoint 
         coordinates. (See :py:func:`keypoint_moseq.calibration.sample_error_frames` 
         for format of sample keys)
     """
     output = ['key,frame,bodypart,x,y']
@@ -155,18 +155,18 @@
 def save_params(project_dir, estimator):
     """
     Save config parameters learned via calibration
 
     Parameters
     ----------
     project_dir: str
-        Save parameters ``{project_dir}/config.yml`` 
+        Save parameters `{project_dir}/config.yml` 
 
     estimator: :py:func:`holoviews.streams.Stream`
-        Stream object with fields ``conf_threshold``, ``slope``, ``intercept``
+        Stream object with fields `conf_threshold`, `slope`, `intercept`
     """
     update_config(project_dir, 
                   conf_threshold=float(estimator.conf_threshold),
                   slope=float(estimator.slope), 
                   intercept=float(estimator.intercept))
 
 
@@ -370,15 +370,15 @@
     """
     Perform manual annotation to calibrate the relationship between
     keypoint error and neural network confidence. 
 
     This function creates a widget for interactive annotation in a 
     jupyter notebook. Users mark correct keypoint locations for a 
     sequence of frames, and a regression line is fit to the 
-    ``log(confidence), log(error)`` pairs obtained through annotation.
+    `log(confidence), log(error)` pairs obtained through annotation.
     The regression coefficients are used during modeling to set a 
     prior on the noise level for each keypoint on each frame. 
 
     Follow these steps to use the widget:
         - After executing this function, a widget should appear with a 
           video frame in the center.
         - Annotate the labeled bodypart in each frame by left-clicking 
@@ -387,42 +387,42 @@
           annotate additional frames.
         - Each annotation adds a point to the right-hand scatter plot. 
           Continue until the regression line stabilizes.
         - At any point, adjust the confidence threshold by clicking on 
           the scatter plot. The confidence threshold is used to define 
           outlier keypoints for PCA and model initialization.
         - Use the "save" button to store your annotations to disk and 
-          save ``slope``, ``intercept``, and ``confidence_threshold``
+          save `slope`, `intercept`, and `confidence_threshold`
           to the config.
 
 
     Parameters
     ----------
     project_dir: str
-        Project directory. Must contain a ``config.yml`` file.
+        Project directory. Must contain a `config.yml` file.
 
     coordinates: dict
         Keypoint coordinates for a collection of sessions. Values
         must be numpy arrays of shape (T,K,D) where K is the number
         of keypoints and D={2 or 3}. Keys can be any unique str,
-        but must start with the name of a videofile in ``video_dir``. 
+        but must start with the name of a videofile in `video_dir`. 
 
     confidences: dict
         Nonnegative confidence values for the keypoints in 
-        ``coordinates`` as numpy arrays of shape (T,K).
+        `coordinates` as numpy arrays of shape (T,K).
 
     bodyparts: list
-        Label for each keypoint represented in ``coordinates``
+        Label for each keypoint represented in `coordinates`
 
     use_bodyparts: list
         Ordered subset of keypoint labels to be used for modeling
 
     video_dir: str
         Path to directory containing videos. Each video should
-        correspond to a key in ``coordinates``. The key must
+        correspond to a key in `coordinates`. The key must
         contain the videoname as a prefix. 
 
     video_extension: str, default=None
         Preferred video extension (used in :py:func:`keypoint_moseq.util.find_matching_videos`)
 
     conf_pseudocount: float, default=0.001
         Pseudocount added to confidence values to avoid log(0) errors.
```

### Comparing `keypoint-moseq-0.0.4/keypoint_moseq/fitting.py` & `keypoint-moseq-0.0.5/keypoint_moseq/fitting.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,38 +26,40 @@
     if include_states: 
         model_snapshot['states'] = jax.device_get(model['states'])
         
     history[iteration] = model_snapshot
     return history
 
 
-def _wrapped_resample(data, model, **resample_options):
+def _wrapped_resample(data, model, pbar=None, **resample_options):
     try: 
         resample_model(data, **model, **resample_options)
     except KeyboardInterrupt: 
         print('Early termination of fitting: user interruption')
         raise StopResampling()
 
     any_nans, nan_info, messages = check_for_nans(model)
     
     if any_nans:
-        print('Early termination of fitting: NaNs encountered')
-        for msg in messages: print('  - {}'.format(msg))
-        print('\nFor additional information, see https://keypoint-moseq.readthedocs.io/en/latest/troubleshooting.html#nans-during-fitting')
+        if pbar is not None: pbar.close()
+        warning_text = ['\nEarly termination of fitting: NaNs encountered']
+        for msg in messages: warning_text.append('  - {}'.format(msg))
+        warning_text.append('\nFor additional information, see https://keypoint-moseq.readthedocs.io/en/latest/troubleshooting.html#nans-during-fitting')
+        warnings.warn('\n'.join(warning_text))
         raise StopResampling()
     
     return model
 
 
 def fit_model(model,
               data,
               labels,
               start_iter=0,
               history=None,
-              verbose=True,
+              verbose=False,
               num_iters=50,
               ar_only=False,
               name=None,
               project_dir=None,
               save_data=True,
               save_states=True,
               save_history=True,
@@ -101,132 +103,134 @@
         If True, print the model's progress during fitting.
 
     num_iters : int, default=50
         Number of Gibbs sampling iterations to run.
 
     ar_only : bool, default=False
         If True, fit an AR-HMM model using the latent trajectory
-        defined by ``model['states']['x']`` (see 
+        defined by `model['states']['x']` (see 
         :py:func:`jax_moseq.models.arhmm.resample_model`).
         Otherwise fit a full keypoint-SLDS model
         (see :py:func:`jax_moseq.models.keypoint_slds.resample_model`)
 
     name : str, default=None
         Name of the model. If None, rhe model is named using the current
         date and time.
 
     project_dir : str, default=None
-        Project directory; required if ``save_every_n_iters>0`` or
-        ``save_progress_figs=True``.
+        Project directory; required if `save_every_n_iters>0` or
+        `save_progress_figs=True`.
 
     save_data : bool, default=True
         If True, include the data in the checkpoint.
 
     save_states : bool, default=True
         If True, include the model's states in the checkpoint.
 
     save_history : bool, default=True
         If True, include the model's history in the checkpoint.
 
     save_every_n_iters : int, default=10
-        Save a checkpoint every ``save_every_n_iters``
+        Save a checkpoint every `save_every_n_iters`
 
     history_every_n_iters : int, default=10
-        Update the model's history every ``history_every_n_iters``. E.g.,
-        if ``history_every_n_iters=10``, the history will contain snapshots 
-        from iterations 0, 10, 20, etc. If ``history_every_n_iters=0``, no
+        Update the model's history every `history_every_n_iters`. E.g.,
+        if `history_every_n_iters=10`, the history will contain snapshots 
+        from iterations 0, 10, 20, etc. If `history_every_n_iters=0`, no
         history is saved.
 
     states_in_history : bool, default=True
         If True, include the model's states in the history.
 
     plot_every_n_iters : int, default=10
-        Plot the model's progress every ``plot_every_n_iters``. If 
-        ``plot_every_n_iters=0``, no plots are generated.
+        Plot the model's progress every `plot_every_n_iters`. If 
+        `plot_every_n_iters=0`, no plots are generated.
 
     save_progress_figs : bool, default=True
         If True, save the progress plots to disk.
         
     Returns
     -------
     model : dict
         Model dictionary containing states, parameters, hyperparameters,
         noise prior, and random seed.
 
     history : dict
         Snapshots of the model over the course of fitting, represented as
         a dictionary with keys corresponding to the iteration number and
-        values corresponding to copies of the ``model`` dictionary.
+        values corresponding to copies of the `model` dictionary.
 
     name : str
         Name of the model.
     """
     if save_every_n_iters>0 or save_progress_figs:
         assert project_dir, fill(
             'To save checkpoints or progress plots during fitting, provide '
-            'a ``project_dir``. Otherwise set ``save_every_n_iters=0`` and '
-            '``save_progress_figs=False``')
+            'a `project_dir`. Otherwise set `save_every_n_iters=0` and '
+            '`save_progress_figs=False`')
         if name is None: 
             name = str(datetime.now().strftime('%Y_%m_%d-%H_%M_%S'))
         savedir = os.path.join(project_dir,name)
         if not os.path.exists(savedir): os.makedirs(savedir)
         print(fill(f'Outputs will be saved to {savedir}'))
 
     if history is None: history = {}
 
-    for iteration in tqdm.trange(start_iter, num_iters+1):
-        if history_every_n_iters>0 and (iteration%history_every_n_iters)==0:
-            history = _update_history(history, iteration, model, 
-                                     include_states=states_in_history)
-            
-        if plot_every_n_iters>0 and (iteration%plot_every_n_iters)==0:
-            plot_progress(model, data, history, iteration, name=name, 
-                          savefig=save_progress_figs, project_dir=project_dir)
-
-        if save_every_n_iters>0 and (iteration%save_every_n_iters)==0:
-            save_checkpoint(model, data, history, labels, iteration, name=name,
-                            project_dir=project_dir,save_history=save_history, 
-                            save_states=save_states, save_data=save_data)
-            
-        try: model = _wrapped_resample(
-            data, model, ar_only=ar_only, verbose=verbose)
-        except StopResampling: break
-
+    with tqdm.trange(start_iter, num_iters+1) as pbar:
+        for iteration in pbar:
+            if history_every_n_iters>0 and (iteration%history_every_n_iters)==0:
+                history = _update_history(history, iteration, model, 
+                                        include_states=states_in_history)
+                
+            if plot_every_n_iters>0 and (iteration%plot_every_n_iters)==0:
+                plot_progress(model, data, history, iteration, name=name, 
+                            savefig=save_progress_figs, project_dir=project_dir)
+
+            if save_every_n_iters>0 and (iteration%save_every_n_iters)==0:
+                save_checkpoint(model, data, history, labels, iteration, name=name,
+                                project_dir=project_dir,save_history=save_history, 
+                                save_states=save_states, save_data=save_data)
+                
+            try: model = _wrapped_resample(
+                data, model, pbar=pbar, ar_only=ar_only, verbose=verbose)
+            except StopResampling: break
 
     return model, history, name
     
     
-def resume_fitting(*, params, hypparams, labels, iteration, mask,
+def resume_fitting(*, params, hypparams, labels, iteration, mask, num_iters,
                    Y, conf, seed, noise_prior=None, states=None, **kwargs):
     """Resume fitting a model from a checkpoint."""
     
+    num_iters = num_iters + iteration
     data = jax.device_put({'Y':Y, 'mask':mask, 'conf':conf})    
     model = init_model(data, states, params, hypparams,
                        noise_prior, seed, **kwargs)
 
-    return fit_model(model, data, labels, start_iter=iteration+1, **kwargs)
+    return fit_model(model, data, labels, start_iter=iteration+1, 
+                     num_iters=num_iters, **kwargs)
 
 
 def apply_model(*, params, coordinates, confidences=None, num_iters=5, 
                 use_saved_states=True, states=None, mask=None, labels=None, 
                 noise_prior=None, ar_only=False, save_results=True, verbose=False,
                 project_dir=None, name=None, results_path=None, **kwargs): 
     """
     Apply a model to data.
 
     There are two scenarios for applying this function:
         - The model is being applied to the same data it was fit to.
             This would useful if the the data was chunked into segments
             to allow parallelization during fitting. In this case,
-            set ``use_saved_states=True`` and provide ``states``.
+            set `use_saved_states=True` and provide `states`.
         - The model is being applied to new data. In this case,
-            set ``use_saved_states=False``.
+            set `use_saved_states=False`.
 
-    Model outputs are saved to disk as a .h5 file, either at ``results_path``
-    if it is specified, or at ``{project_dir}/{name}/results.h5`` if it is not.
+    Model outputs are saved to disk as a .h5 file, either at `results_path`
+    if it is specified, or at `{project_dir}/{name}/results.h5` if it is not.
     If a .h5 file with the given path already exists, the outputs will be added
     to it. The results have the following structure::
 
         results.h5
         ├──session_name1
         │  ├──syllables             # model state sequence (z), shape=(T,)
         │  ├──syllables_reindexed   # states reindexed by frequency, shape=(T,)
@@ -251,76 +255,76 @@
 
     num_iters : int, default=5
         Number of iterations to run the model. We recommend 5 iterations
         for data the model has already been fit to, and a higher number
         (e.g. 10-20) for new data.
 
     use_saved_states : bool, default=True
-        If True, and ``states`` is provided, the model will be initialized
+        If True, and `states` is provided, the model will be initialized
         with the saved states. 
 
     states : dict, default=None
         Dictionary of saved states. 
 
     mask: ndarray, default=None
-        Binary mask indicating areas of padding in ``states``
+        Binary mask indicating areas of padding in `states`
         (see :py:func:`keypoint_moseq.util.batch`).
 
     labels: list
-        Row labels ``states``
+        Row labels `states`
         (see :py:func:`keypoint_moseq.util.batch`).
 
     noise_prior : ndarray, default=None
         Prior on the noise for each observation. Should be the same shape
-        as ``states['s']``.
+        as `states['s']`.
 
     ar_only : bool, default=False
         See :py:func:`keypoint_moseq.fitting.fit_model`.
 
     save_results : bool, default=True
         If True, the model outputs will be saved to disk.
 
     verbose : bool, default=False
         Whether to print progress updates.
 
     project_dir : str, default=None
-        Path to the project directory. Required if ``save_results=True``
-        and ``results_path=None``.
+        Path to the project directory. Required if `save_results=True`
+        and `results_path=None`.
 
     name : str, default=None
-        Name of the model. Required if ``save_results=True``
-        and ``results_path=None``.
+        Name of the model. Required if `save_results=True`
+        and `results_path=None`.
 
     results_path : str, default=None
         Optional path for saving model outputs.
 
     Returns
     -------
     results_dict : dict
         Dictionary of model outputs with the same structure as the
-        results ``.h5`` file.
+        results `.h5` file.
     """
     
     kwargs['seg_length'] = None # dont separate the data into segments
     
     data, new_labels = format_data(
         coordinates, confidences=confidences, **kwargs)
     session_names = [key for key,start,end in new_labels]
 
     if save_results:
         if results_path is None: 
             assert project_dir is not None and name is not None, fill(
-                'The ``save_results`` option requires either a ``results_path`` '
-                'or the ``project_dir`` and ``name`` arguments')
+                'The `save_results` option requires either a `results_path` '
+                'or the `project_dir` and `name` arguments')
             results_path = os.path.join(project_dir,name,'results.h5')
      
     if use_saved_states:
         assert not (states is None or mask is None or labels is None), fill(
-            'The ``use_saved_states`` option requires the additional '
-            'arguments ``states``, ``mask`` and ``labels``')   
+            'The `use_saved_states` option requires the additional '
+            'arguments `states`, `mask` and `labels`')   
         
         if noise_prior is not None:
             noise_prior = batch(unbatch(noise_prior, labels), keys=session_names)[0]
             noise_prior = np.where(data['mask'][...,None], noise_prior, 1) 
             
         new_states = {}
         for k,v in jax.device_get(states).items():
@@ -333,18 +337,20 @@
     else: 
         states = None
         noise_prior = None
     
     model = init_model(data, states, params, noise_prior=noise_prior, verbose=verbose, **kwargs)
     
     if num_iters>0:
-        for iteration in tqdm.trange(num_iters, desc='Applying model'):
-            try: model = _wrapped_resample(
-                    data, model, ar_only=ar_only, states_only=True, verbose=verbose)
-            except StopResampling: break
+        with tqdm.trange(num_iters, desc='Applying model') as pbar:
+            for iteration in pbar:
+                try: model = _wrapped_resample(
+                        data, model, pbar=pbar, ar_only=ar_only, 
+                        states_only=True, verbose=verbose)
+                except StopResampling: break
 
 
     nlags = model['hypparams']['ar_hypparams']['nlags']
     states = jax.device_get(model['states'])                     
     estimated_coords = jax.device_get(estimate_coordinates(
         **model['states'], **model['params'], **data))
     z_reindexed = reindex_by_frequency(states['z'], np.array(data['mask']))
@@ -368,15 +374,15 @@
 
 
 def revert(checkpoint, iteration):
     """
     Revert a checkpoint to an earlier iteration.
 
     The checkpoint will revert to latest iteration stored in the 
-    fitting history that is less than or equal to ``iteration``.
+    fitting history that is less than or equal to `iteration`.
     The model parameters, seed, and iteration number will be updated
     accordingly. The fitting history will be truncated to remove
     all iterations after the reverted iteration.
 
     Parameters
     ----------
     checkpoint : dict
@@ -412,15 +418,15 @@
     
     
 def update_hypparams(model_dict, **kwargs):
     """
     Edit the hyperparameters of a model.
 
     Hyperparameters are stored as a nested dictionary in the
-    ``hypparams`` key of the model dictionary. This function
+    `hypparams` key of the model dictionary. This function
     allows the user to update the hyperparameters of a model
     by passing in keyword arguments with the same name as the
     hyperparameter. The hyperparameter will be updated if it
     is a scalar value.
 
     Parameters
     ----------
```

### Comparing `keypoint-moseq-0.0.4/keypoint_moseq/io.py` & `keypoint-moseq-0.0.5/keypoint_moseq/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,37 +20,35 @@
 from keypoint_moseq.util import (
     reindex_by_bodyparts, 
     list_files_with_exts, 
     interpolate_keypoints,
 )
 
 
-
-
 def _build_yaml(sections, comments):
     text_blocks = []
     for title,data in sections:
         centered_title = f' {title} '.center(50, '=')
         text_blocks.append(f"\n\n{'#'}{centered_title}{'#'}")
         for key,value in data.items():
             text = yaml.dump({key:value}).strip('\n')
             if key in comments: text = f"\n{'#'} {comments[key]}\n{text}"
             text_blocks.append(text)
     return '\n'.join(text_blocks)
         
 
 def generate_config(project_dir, **kwargs):
     """
-    Generate a ``config.yml`` file with project settings. Default 
-    settings will be used unless overriden by a keywork argument.
+    Generate a `config.yml` file with project settings. Default 
+    settings will be used unless overriden by a keyword argument.
     
     Parameters
     ----------
     project_dir: str 
-        A file ``config.yml`` will be generated in this directory.
+        A file `config.yml` will be generated in this directory.
     
     kwargs
         Custom project settings.  
     """
     
     def _update_dict(new, original):
         return {k:new[k] if k in new else v for k,v in original.items()} 
@@ -131,22 +129,22 @@
                           
         
 def check_config_validity(config):
     """
     Check if the config is valid.
 
     To be valid, the config must satisfy the following criteria:
-        - All the elements of ``config["use_bodyparts"]`` are 
-          also in ``config["bodyparts"]`` 
-        - All the elements of ``config["anterior_bodyparts"]`` are
-          also in ``config["bodyparts"]`` 
-        - All the elements of ``config["anterior_bodyparts"]`` are
-          also in ``config["bodyparts"]`` 
-        - For each pair in ``config["skeleton"]``, both elements 
-          also in ``config["bodyparts"]`` 
+        - All the elements of `config["use_bodyparts"]` are 
+          also in `config["bodyparts"]` 
+        - All the elements of `config["anterior_bodyparts"]` are
+          also in `config["bodyparts"]` 
+        - All the elements of `config["anterior_bodyparts"]` are
+          also in `config["bodyparts"]` 
+        - For each pair in `config["skeleton"]`, both elements 
+          also in `config["bodyparts"]` 
 
     Parameters
     ----------
     config: dict 
 
     Returns
     -------
@@ -196,19 +194,19 @@
         Directory containing the config file
         
     check_if_valid: bool, default=True
         Check if the config is valid using 
         :py:func:`keypoint_moseq.io.check_config_validity`
         
     build_indexes: bool, default=True
-        Add keys ``"anterior_idxs"`` and ``"posterior_idxs"`` to the 
+        Add keys `"anterior_idxs"` and `"posterior_idxs"` to the 
         config. Each maps to a jax array indexing the elements of 
-        ``config["anterior_bodyparts"]`` and 
-        ``config["posterior_bodyparts"]`` by their order in 
-        ``config["use_bodyparts"]``
+        `config["anterior_bodyparts"]` and 
+        `config["posterior_bodyparts"]` by their order in 
+        `config["use_bodyparts"]`
 
     Returns
     -------
     config: dict
     """
     config_path = os.path.join(project_dir,'config.yml')
     
@@ -219,34 +217,37 @@
         check_config_validity(config)
         
     if build_indexes:
         config['anterior_idxs'] = jnp.array(
             [config['use_bodyparts'].index(bp) for bp in config['anterior_bodyparts']])
         config['posterior_idxs'] = jnp.array(
             [config['use_bodyparts'].index(bp) for bp in config['posterior_bodyparts']])
+    
+    if not 'skeleton' in config or config['skeleton'] is None:
+        config['skeleton'] = []
         
     return config
 
 def update_config(project_dir, **kwargs):
     """
-    Update the config file stored at ``project_dir/config.yml``.
+    Update the config file stored at `project_dir/config.yml`.
      
     Use keyword arguments to update key/value pairs in the config.
     To update model hyperparameters, just use the name of the 
     hyperparameter as the keyword argument. 
 
     Examples
     --------
-    To update ``video_dir`` to ``/path/to/videos``::
+    To update `video_dir` to `/path/to/videos`::
 
       >>> update_config(project_dir, video_dir='/path/to/videos')
       >>> print(load_config(project_dir)['video_dir'])
       /path/to/videos
 
-    To update ``trans_hypparams['kappa']`` to ``100``::
+    To update `trans_hypparams['kappa']` to `100`::
 
       >>> update_config(project_dir, kappa=100)
       >>> print(load_config(project_dir)['trans_hypparams']['kappa'])
       100
     """
     config = load_config(project_dir, check_if_valid=False, build_indexes=False)
     config.update(kwargs)
@@ -264,27 +265,27 @@
     Parameters
     ----------
     project_dir: str 
         Path to the project directory (relative or absolute)
         
     deeplabcut_config: str, default=None
         Path to a deeplabcut config file. Relevant settings, including
-        ``'bodyparts'``, ``'skeleton'``, ``'use_bodyparts'``, and 
-        ``'video_dir'`` will be imported from the deeplabcut config and 
+        `'bodyparts'`, `'skeleton'`, `'use_bodyparts'`, and 
+        `'video_dir'` will be imported from the deeplabcut config and 
         used to initialize the keypoint MoSeq config. (overrided by kwargs). 
 
     sleap_file: str, default=None
         Path to a sleap hdf5 file for one of the recordings to be modeled. 
-        Relevant settings, including ``'bodyparts'``, ``'skeleton'``, 
-        and ``'use_bodyparts'`` will be imported from the sleap file and used 
+        Relevant settings, including `'bodyparts'`, `'skeleton'`, 
+        and `'use_bodyparts'` will be imported from the sleap file and used 
         to initialize the keypoint MoSeq config. (overrided by kwargs). 
         
     overwrite: bool, default=False
         Overwrite any config.yml that already exists at the path
-        ``{project_dir}/config.yml``
+        `{project_dir}/config.yml`
         
     options
         Used to initialize config file. Overrides default settings
     """
 
     if os.path.exists(project_dir) and not overwrite:
         print(fill(
@@ -338,75 +339,75 @@
     """
     Format keypoint coordinates and confidences for inference.
 
     Data are transformed as follows:
         1. Coordinates and confidences are each merged into a single 
            array using :py:func:`keypoint_moseq.util.batch`. 
         2. The keypoints axis is reindexed according to the order
-           of elements in ``use_bodyparts`` with respect to their 
-           initial orer in ``bodyparts``.
-        3. Uniform noise proportional to ``added_noise_level`` is
+           of elements in `use_bodyparts` with respect to their 
+           initial orer in `bodyparts`.
+        3. Uniform noise proportional to `added_noise_level` is
            added to the keypoint coordinates to prevent degenerate
            solutions during fitting. 
-        4. Keypoint confidences are augmented by ``conf_pseudocount``.
+        4. Keypoint confidences are augmented by `conf_pseudocount`.
         5. Wherever NaNs occur in the coordinates, they are replaced
            by values imputed using linear interpolation, and the
-           corresponding confidences are set to ``conf_pseudocount``.
+           corresponding confidences are set to `conf_pseudocount`.
     
     Parameters
     ----------
     coordinates: dict
         Keypoint coordinates for a collection of sessions. Values
         must be numpy arrays of shape (T,K,D) where K is the number
         of keypoints and D={2 or 3}. 
         
     confidences: dict, default=None
         Nonnegative confidence values for the keypoints in 
-        ``coordinates`` as numpy arrays of shape (T,K).
+        `coordinates` as numpy arrays of shape (T,K).
         
     keys: list of str, default=None
         (See :py:func:`keypoint_moseq.util.batch`)
         
     seg_length: int default=None
         (See :py:func:`keypoint_moseq.util.batch`)
         
     bodyparts: list, default=None
-        Label for each keypoint represented in ``coordinates``. Required
-        to reindex coordinates and confidences according to ``use_bodyparts``.
+        Label for each keypoint represented in `coordinates`. Required
+        to reindex coordinates and confidences according to `use_bodyparts`.
 
     use_bodyparts: list, default=None
         Ordered subset of keypoint labels to be used for modeling.
-        If ``use_bodyparts=None``, then all keypoints are used.
+        If `use_bodyparts=None`, then all keypoints are used.
 
     conf_pseudocount: float, default=1e-3
         Pseudocount used to augment keypoint confidences.
     
     seg_length: int, default=None
-        Length of each segment. If ``seg_length=None``, a length is 
+        Length of each segment. If `seg_length=None`, a length is 
         chosen so that no time-series are broken into multiple segments.
         
     Returns
     -------
     data: dict with the following items
     
         Y: jax array with shape (n_segs, seg_length, K, D)
             Keypoint coordinates from all sessions broken into 
             fixed-length segments.
             
         conf: jax array with shape (n_segs, seg_length, K)
             Confidences from all sessions broken into fixed-length 
-            segments. If no input is provided for ``confidences``, 
-            then ``data["conf"]=None``.
+            segments. If no input is provided for `confidences`, 
+            then `data["conf"]=None`.
         
         mask: jax array with shape (n_segs, seg_length)
             Binary array where 0 indicates areas of padding 
             (see :py:func:`keypoint_moseq.util.batch`).
             
     labels: list of tuples (object, int, int)
-        Label for each row of ``Y`` and ``conf`` 
+        Label for each row of `Y` and `conf` 
         (see :py:func:`keypoint_moseq.util.batch`).
     """    
     if keys is None: 
         keys = sorted(coordinates.keys()) 
 
     if any(['/' in key for key in keys]): 
         warnings.warn(fill(
@@ -419,21 +420,21 @@
     if bodyparts is not None and use_bodyparts is not None:
         coordinates = reindex_by_bodyparts(coordinates, bodyparts, use_bodyparts)
         confidences = reindex_by_bodyparts(confidences, bodyparts, use_bodyparts)
 
     for key in keys:
         outliers = np.isnan(coordinates[key]).any(-1)
         coordinates[key] = interpolate_keypoints(coordinates[key], outliers)
-        confidences[key] = np.where(outliers, 0, confidences[key])
+        confidences[key] = np.where(outliers, 0, np.nan_to_num(confidences[key]))
 
     Y,mask,labels = batch(coordinates, seg_length=seg_length, keys=keys)
     Y = Y.astype(float)
 
     conf = batch(confidences, seg_length=seg_length, keys=keys)[0]
-    if np.nanmin(conf) < 0: 
+    if np.min(conf) < 0: 
         conf = np.maximum(conf,0) 
         warnings.warn(fill(
             'Negative confidence values are not allowed and will be set to 0.'))
     conf = conf + conf_pseudocount
   
     if added_noise_level>0: 
         Y += np.random.uniform(-added_noise_level,added_noise_level,Y.shape)
@@ -441,16 +442,16 @@
     return jax.device_put({'mask':mask, 'Y':Y, 'conf':conf}), labels
 
 
 def save_pca(pca, project_dir, pca_path=None):
     """
     Save a PCA model to disk.
 
-    The model is saved to ``pca_path`` or else to 
-    ``{project_dir}/pca.p``.
+    The model is saved to `pca_path` or else to 
+    `{project_dir}/pca.p`.
     
     Parameters
     ----------
     pca: :py:class:`sklearn.decomposition.PCA`
     project_dir: str
     pca_path: str, default=None
     """
@@ -458,16 +459,16 @@
         pca_path = os.path.join(project_dir,'pca.p')
     joblib.dump(pca, pca_path)
     
 def load_pca(project_dir, pca_path=None):
     """
     Load a PCA model from disk.
 
-    The model is loaded from ``pca_path`` or else from 
-    ``{project_dir}/pca.p``.
+    The model is loaded from `pca_path` or else from 
+    `{project_dir}/pca.p`.
 
     Parameters
     ----------
     project_dir: str
     pca_path: str, default=None
 
     Returns
@@ -519,47 +520,47 @@
     return load_checkpoint(path=path), name
 
 
 def load_checkpoint(project_dir=None, name=None, path=None):
     """
     Load model fitting checkpoint.
 
-    The checkpoint path can be specified directly via ``path``.
-    Othewise is assumed to be ``{project_dir}/<name>/checkpoint.p``.
+    The checkpoint path can be specified directly via `path`.
+    Othewise is assumed to be `{project_dir}/<name>/checkpoint.p`.
 
     Parameters
     ----------
     project_dir: str, default=None
     name: str, default=None
     path: str, default=None
 
     Returns
     -------
     checkpoint: dict
         See :py:func:`keypoint_moseq.io.save_checkpoint`
     """
     if path is None: 
         assert project_dir is not None and name is not None, fill(
-            '``name`` and ``project_dir`` are required if no ``path`` is given.')
+            '`name` and `project_dir` are required if no `path` is given.')
         path = os.path.join(project_dir,name,'checkpoint.p')
     return joblib.load(path)
 
 
 def save_checkpoint(model, data, history, labels, iteration, 
                     path=None, name=None, project_dir=None,
                     save_history=True, save_states=True, save_data=True):
     """
     Save a checkpoint during model fitting.
 
     A single checkpoint file contains model snapshots from the full history
     of model fitting. To restart fitting from an iteration earlier than the
-    last iteration, use :py:func:`keypoint_moseq.fitting.revert``.
+    last iteration, use :py:func:`keypoint_moseq.fitting.revert`.
 
-    The checkpoint path can be specified directly via ``path``.
-    Otherwise is assumed to be ``{project_dir}/<name>/checkpoint.p``. See
+    The checkpoint path can be specified directly via `path`.
+    Otherwise is assumed to be `{project_dir}/<name>/checkpoint.p`. See
     :py:func:`keypoint_moseq.fitting.fit_model` for a more detailed
     description of the checkpoint contents.
 
     Parameters
     ----------
     model: dict, history: dict
         See :py:func:`keypoint_moseq.fitting.fit_model`
@@ -567,45 +568,45 @@
     data: dict, labels: list of tuples
         See :py:func:`keypoint_moseq.io.format_data`
 
     iteration: int
         Current iteration of model fitting
 
     save_history: bool, default=True
-        Whether to include ``history`` in the checkpoint
+        Whether to include `history` in the checkpoint
 
     save_states: bool, default=True
-        Whether to include ``states`` in the checkpoint
+        Whether to include `states` in the checkpoint
 
     save_data: bool, default=True
-        Whether to include ``Y``, ``conf``, and ``mask`` in the checkpoint
+        Whether to include `Y`, `conf`, and `mask` in the checkpoint
     
     project_dir: str, default=None
-        Project directory; used in conjunction with ``name`` to determine
-        the checkpoint path if ``path`` is not specified.
+        Project directory; used in conjunction with `name` to determine
+        the checkpoint path if `path` is not specified.
 
     name: str, default=None
-        Model name; used in conjunction with ``project_dir`` to determine
-        the checkpoint path if ``path`` is not specified.
+        Model name; used in conjunction with `project_dir` to determine
+        the checkpoint path if `path` is not specified.
 
     path: str, default=None
         Checkpoint path; if not specified, the checkpoint path is determined
-        from ``project_dir`` and ``name``.
+        from `project_dir` and `name`.
 
 
     Returns
     -------
     checkpoint: dict
-        Dictionary containing ``history``, ``labels`` and ``name`` as 
-        well as the key/value pairs from ``model`` and ``data``.
+        Dictionary containing `history`, `labels` and `name` as 
+        well as the key/value pairs from `model` and `data`.
     """
     
     if path is None: 
         assert project_dir is not None and name is not None, fill(
-            '``name`` and ``project_dir`` are required if no ``path`` is given.')
+            '`name` and `project_dir` are required if no `path` is given.')
         path = os.path.join(project_dir,name,'checkpoint.p')
 
     dirname = os.path.dirname(path)
     if not os.path.exists(dirname): 
         print(fill(f'Creating the directory {dirname}'))
         os.makedirs(dirname)
     
@@ -634,98 +635,94 @@
     return save_dict
 
     
 def load_results(project_dir=None, name=None, path=None):
     """
     Load the results from a modeled dataset.
 
-    The results path can be specified directly via ``path``. Otherwise
-    it is assumed to be ``{project_dir}/<name>/results.h5``.
+    The results path can be specified directly via `path`. Otherwise
+    it is assumed to be `{project_dir}/<name>/results.h5`.
     
     Parameters
     ----------
     project_dir: str, default=None
     name: str, default=None
     path: str, default=None
 
     Returns
     -------
     results: dict
         See :py:func:`keypoint_moseq.fitting.apply_model`
     """
     if path is None: 
         assert project_dir is not None and name is not None, fill(
-            '``name`` and ``project_dir`` are required if no ``path`` is given.')
+            '`name` and `project_dir` are required if no `path` is given.')
         path = os.path.join(project_dir,name,'results.h5')
     return load_hdf5(path)
 
 
 def _name_from_path(filepath, path_in_name, path_sep):
     """
     Create a name from a filepath. Either return the name of the file
     (with the extension removed) or return the full filepath, where the
-    path separators are replaced with ``path_sep``.
+    path separators are replaced with `path_sep`.
     """
     filepath = os.path.splitext(filepath)[0]
     if path_in_name:
         return filepath.replace(os.path.sep, path_sep)
     else:
         return os.path.basename(filepath)
 
 
 def load_deeplabcut_results(filepath_pattern, recursive=True, path_sep='-',
                             path_in_name=False, return_bodyparts=False):
     """
     Load tracking results from deeplabcut csv or hdf5 files.
 
-    Deeplabcut outputs tracking results in csv and/or hdf5 format. This
-    function tries to load all files ending in ``.csv`` ``.h5`` or ``.hdf5``,
-    unless a specific extension is specified by the ``extension`` argument.
-   
     Parameters
     ----------
     filepath_pattern: str or list of str
         Filepath pattern for a set of deeplabcut csv or hdf5 files, 
         or a list of such patterns. Filepath patterns can be:
 
-            - single file (e.g. ``/path/to/file.csv``) 
-            - single directory (e.g. ``/path/to/dir/``)
-            - set of files (e.g. ``/path/to/fileprefix*``)
-            - set of directories (e.g. ``/path/to/dirprefix*``)
+            - single file (e.g. `/path/to/file.csv`) 
+            - single directory (e.g. `/path/to/dir/`)
+            - set of files (e.g. `/path/to/fileprefix*`)
+            - set of directories (e.g. `/path/to/dirprefix*`)
 
     recursive: bool, default=True
         Whether to search recursively for deeplabcut csv or hdf5 files.
 
     path_in_name: bool, default=False
         Whether to name the tracking results from each file by the path
         to the file (True) or just the filename (False). If True, the
-        ``path_sep`` argument is used to separate the path components.
+        `path_sep` argument is used to separate the path components.
         
     path_sep: str, default='-'
-        Separator to use when ``path_in_name`` is True. For example,
-        if ``path_sep`` is ``'-'``, then the tracking results from the
-        file ``/path/to/file.csv`` will be named ``path-to-file``. Using
-        ``'/'`` as the separator is discouraged, as it will cause problems
+        Separator to use when `path_in_name` is True. For example,
+        if `path_sep` is `'-'`, then the tracking results from the
+        file `/path/to/file.csv` will be named `path-to-file`. Using
+        `'/'` as the separator is discouraged, as it will cause problems
         saving/loading the modeling results to/from hdf5 files.
 
     return_bodyparts: bool, default=False
         Whether to return a list of bodypart names.
 
     Returns
     -------
     coordinates: dict
         Dictionary mapping filenames to keypoint coordinates as ndarrays
         of shape (n_frames, n_bodyparts, 2)
 
     confidences: dict
-        Dictionary mapping filenames to ``likelihood`` scores as ndarrays
+        Dictionary mapping filenames to `likelihood` scores as ndarrays
         of shape (n_frames, n_bodyparts)
 
     bodyparts: list of str
-        List of bodypart names. Only returned if ``return_bodyparts`` is True.
+        List of bodypart names. Only returned if `return_bodyparts` is True.
     """
     filepaths = list_files_with_exts(
         filepath_pattern, ['.csv','.h5','.hdf5'], recursive=recursive)
     assert len(filepaths)>0, fill(
         f'No deeplabcut csv or hdf5 files found for {filepath_pattern}')
 
     coordinates,confidences = {},{}
@@ -755,50 +752,50 @@
 
     Parameters
     ----------
     filepath_pattern: str, default=None
         Filepath pattern for a set of sleap hdf5 files, or a list of 
         such patterns. Filepath patterns can be:
 
-            - single file (e.g. ``/path/to/file.csv``) 
-            - single directory (e.g. ``/path/to/dir/``)
-            - set of files (e.g. ``/path/to/fileprefix*``)
-            - set of directories (e.g. ``/path/to/dirprefix*``)
+            - single file (e.g. `/path/to/file.csv`) 
+            - single directory (e.g. `/path/to/dir/`)
+            - set of files (e.g. `/path/to/fileprefix*`)
+            - set of directories (e.g. `/path/to/dirprefix*`)
 
     recursive: bool, default=True
         Whether to search recursively for sleap hdf5 files.
 
     path_in_name: bool, default=False
         Whether to name the tracking results from each file by the path
         to the file (True) or just the filename (False). If True, the
-        ``path_sep`` argument is used to separate the path components.
+        `path_sep` argument is used to separate the path components.
         
     path_sep: str, default='-'
-        Separator to use when ``path_in_name`` is True. For example,
-        if ``path_sep`` is ``'-'``, then the tracking results from the
-        file ``/path/to/file.csv`` will be named ``path-to-file``. Using
-        ``'/'`` as the separator is discouraged, as it will cause problems
+        Separator to use when `path_in_name` is True. For example,
+        if `path_sep` is `'-'`, then the tracking results from the
+        file `/path/to/file.csv` will be named `path-to-file`. Using
+        `'/'` as the separator is discouraged, as it will cause problems
         saving/loading the modeling results to/from hdf5 files.
 
     
     return_bodyparts: bool, default=False
         Whether to return a list of bodypart names.
 
     Returns
     -------
     coordinates: dict
         Dictionary mapping filenames to keypoint coordinates as ndarrays
         of shape (n_frames, n_bodyparts, 2)
 
     confidences: dict
-        Dictionary mapping filenames to ``likelihood`` scores as ndarrays
+        Dictionary mapping filenames to `likelihood` scores as ndarrays
         of shape (n_frames, n_bodyparts)
 
     bodyparts: list of str
-        List of bodypart names. Only returned if ``return_bodyparts`` is True.
+        List of bodypart names. Only returned if `return_bodyparts` is True.
     """
     filepaths = list_files_with_exts(
         filepath_pattern, ['.h5','.hdf5'], recursive=recursive)
     assert len(filepaths)>0, fill(
         f'No sleap hdf5 files found for {filepath_pattern}.')
 
     coordinates,confidences = {},{}
```

### Comparing `keypoint-moseq-0.0.4/keypoint_moseq/util.py` & `keypoint-moseq-0.0.5/keypoint_moseq/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 
     Parameters
     ----------
     stateseqs: ndarray
         Batch of state sequences where the last dim indexes time 
 
     mask: ndarray
-        Binary indicator for which elements of ``stateseqs`` are valid,
+        Binary indicator for which elements of `stateseqs` are valid,
         e.g. when state sequences of different lengths have been padded
-        and stacked together in ``stateseqs``
+        and stacked together in `stateseqs`
 
     Returns
     -------
     frequency: ndarray, shape (max(stateseqs)+1,)
         The frequency of each syllable (not run-length encoded)
 
     durations: ndarray
@@ -76,17 +76,17 @@
     ----------
     stateseqs: dict or ndarray, shape (..., t)
         Dictionary mapping names to 1d arrays, or a single
         multi-dimensional array representing a batch of state sequences
         where the last dim indexes time
 
     mask: ndarray, shape (..., >=t), default=None
-        Binary indicator for which elements of ``stateseqs`` are valid,
+        Binary indicator for which elements of `stateseqs` are valid,
         e.g. when state sequences of different lengths have been padded.
-        If ``mask`` contains more time-points than ``stateseqs``, the
+        If `mask` contains more time-points than `stateseqs`, the
         initial extra time-points will be ignored.
 
     Returns
     -------
     stateseqs_flat: ndarray
         1d array containing all state sequences 
     """
@@ -137,15 +137,15 @@
 
     Parameters
     ----------
     stateseqs: dict or ndarray of shape (..., t)
     mask: ndarray of shape (..., >=t), default=None
     num_states: int, default=None
         Number of different states. If None, the number of states will
-        be set to ``max(stateseqs)+1``.
+        be set to `max(stateseqs)+1`.
 
     Returns
     -------
     frequencies: 1d array
         Proportion of frames in each state across all state sequences
 
     Examples
@@ -172,15 +172,15 @@
     ----------
     stateseqs: dict or ndarray of shape (..., t)
     mask: ndarray of shape (..., >=t), default=None
 
     Returns
     -------
     stateseqs_reindexed: ndarray
-        The reindexed state sequences in the same format as ``stateseqs``
+        The reindexed state sequences in the same format as `stateseqs`
     """
     frequency = get_frequencies(stateseqs, mask=mask)
     o = np.argsort(np.argsort(frequency)[::-1])
     if isinstance(stateseqs, dict):
         stateseqs_reindexed = {k: o[seq] for k,seq in stateseqs.items()}
     else: stateseqs_reindexed = o[stateseqs]
     return stateseqs_reindexed
@@ -195,16 +195,15 @@
     ----------
     filepath_pattern : str or list
         A filepath pattern or a list thereof. Filepath patterns can be
         be a single file, a directory, or a path with wildcards (e.g.,
         '/path/to/dir/prefix*').
 
     ext_list : list of str
-        A list of file extensions to search for, including the dot 
-        (e.g., '.txt').
+        A list of file extensions to search for.
 
     recursive : bool, default=True
         Whether to search for files recursively.
 
     Returns
     -------
     list
@@ -213,35 +212,34 @@
     if isinstance(filepath_pattern, list):
         matches = []
         for fp in filepath_pattern:
             matches += list_files_with_exts(fp, ext_list, recursive=recursive)
         return sorted(set(matches))
     
     else:
-        # make sure extensions all start with "." and include uppercase versions
-        ext_list = ['.'+ext.strip('.') for ext in ext_list]
-        ext_list += [ext.upper() for ext in ext_list]
+        # make sure extensions all start with "." and are lowercase
+        ext_list = ['.'+ext.strip('.').lower() for ext in ext_list]
         
         # find all matches (recursively)
         matches = glob.glob(filepath_pattern)
         if recursive:
             for match in list(matches):
                 matches += glob.glob(os.path.join(match, '**'), recursive=True)
 
         # filter matches by extension
-        matches = [match for match in matches if os.path.splitext(match)[1] in ext_list]
+        matches = [match for match in matches if os.path.splitext(match)[1].lower() in ext_list]
         return matches
     
 
 def find_matching_videos(keys, video_dir, as_dict=False, recursive=True, 
                          session_name_suffix='', video_extension=None):
     """
     Find video files for a set of session names. The filename of each
     video is assumed to be a prefix within the session name, i.e. the
-    session name has the form ``{video_name}{more_text}``. If more than 
+    session name has the form `{video_name}{more_text}`. If more than 
     one video matches a session name, the longest match will be used. 
     For example given the following video directory::
 
         video_dir
         ├─ videoname1.avi
         └─ videoname2.avi
  
@@ -250,15 +248,15 @@
         >>> keys = ['videoname1blahblah','videoname2yadayada']
         >>> find_matching_videos(keys, video_dir, as_dict=True)
 
         {'videoname1blahblah': 'video_dir/videoname1.avi',
          'videoname2blahblah': 'video_dir/videoname2.avi'}
 
     A suffix can also be specified, in which case the session name 
-    is assumed to have the form ``{video_name}{suffix}{more_text}``.
+    is assumed to have the form `{video_name}{suffix}{more_text}`.
  
     Parameters
     -------
     keys: iterable
         Session names (as strings)
 
     video_dir: str
@@ -375,17 +373,17 @@
     return centroids, headings
 
 
 def get_syllable_instances(stateseqs, min_duration=3, pre=30, post=60,
                            min_frequency=0, min_instances=0):
     """
     Map each syllable to a list of instances when it occured. Only 
-    include instances that meet the criteria specified by ``pre``, 
-    ``post``, and ``min_duration``. Only include syllables that meet the
-    criteria specified by ``min_frequency`` and ``min_instances``. 
+    include instances that meet the criteria specified by `pre`, 
+    `post`, and `min_duration`. Only include syllables that meet the
+    criteria specified by `min_frequency` and `min_instances`. 
 
     Parameters
     -------
     stateseqs: dict {str : 1d array}
         Dictionary mapping names to syllable sequences
 
     min_duration: int, default=3
@@ -408,15 +406,15 @@
         inclusion of a syllable
 
     Returns
     -------
     syllable_instances: dict
         Dictionary mapping each syllable to a list of instances. Each
         instance is a tuple (name,start,end) representing subsequence
-        ``stateseqs[name][start:end]``.
+        `stateseqs[name][start:end]`.
     """
     num_syllables = int(max(map(max,stateseqs.values()))+1)
     syllable_instances = [[] for syllable in range(num_syllables)]
     
     for key,stateseq in stateseqs.items():
         transitions = np.nonzero(stateseq[1:] != stateseq[:-1])[0]+1
         starts = np.insert(transitions,0,0)
@@ -442,15 +440,15 @@
 
     skeleton: list
         Pairs of bodypart names as tuples (bodypart1,bodypart2)
 
     Returns
     -------
     edges: list
-        Pairs of indexes representing the enties of ``skeleton``
+        Pairs of indexes representing the enties of `skeleton`
     """
     edges = []
     for bp1,bp2 in skeleton:
         if bp1 in use_bodyparts and bp2 in use_bodyparts:
             edges.append([use_bodyparts.index(bp1),use_bodyparts.index(bp2)])
     return edges
 
@@ -462,42 +460,42 @@
     Parameters
     -------
     data: dict or ndarray
         A single array of keypoint coordinates or a dict mapping from 
         names to arrays of keypoint coordinates
 
     bodyparts: list
-        Label for each keypoint represented in ``data``
+        Label for each keypoint represented in `data`
 
     use_bodyparts: list
         Ordered subset of keypoint labels
 
     axis: int, default=1
-        The axis in ``data`` that represents keypoints. It is required
-        that ``data.shape[axis]==len(bodyparts)``. 
+        The axis in `data` that represents keypoints. It is required
+        that `data.shape[axis]==len(bodyparts)`. 
 
     Returns
     -------
     reindexed_data: ndarray or dict
-        Keypoint coordinates in the same form as ``data`` with
+        Keypoint coordinates in the same form as `data` with
         reindexing applied
     """
     ix = np.array([bodyparts.index(bp) for bp in use_bodyparts])
     if isinstance(data, np.ndarray): return np.take(data, ix, axis)
     else: return {k: np.take(v, ix, axis) for k,v in data.items()}
 
 
 def get_trajectories(syllable_instances, coordinates, pre=0, post=None, 
                      centroids=None, headings=None, filter_size=9):
     """
     Extract keypoint trajectories for a collection of syllable instances. 
     
     If centroids and headings are provided, each trajectory
     is transformed into the ego-centric reference frame from the moment 
-    of syllable onset. When ``post`` is not None, trajectories will 
+    of syllable onset. When `post` is not None, trajectories will 
     all terminate a fixed number of frames after syllable onset. 
 
     Parameters
     -------
     syllable_instances: list
         List of syllable instances, where each instance is a tuple of 
         the form (name,start,end)
@@ -506,34 +504,34 @@
         Dictionary mapping names to coordinates, formatted as ndarrays
         with shape (num_frames, num_keypoints, d)
 
     pre: int, default=0
         Number of frames to include before syllable onset
 
     post: int, defualt=None
-        Determines the length of the trajectory. When ``post=None``,
+        Determines the length of the trajectory. When `post=None`,
         the trajectory terminates at the end of the syllable instance.
         Otherwise the trajectory terminates at a fixed number of frames
-        after syllable (where the number is determined by ``post``).
+        after syllable (where the number is determined by `post`).
 
     centroids: dict, default=None
-        Dictionary with the same keys as ``coordinates`` mapping each
+        Dictionary with the same keys as `coordinates` mapping each
         name to an ndarray with shape (num_frames, d)
 
     headings: dict, default=None
-        Dictionary with the same keys as ``coordinates`` mapping each
+        Dictionary with the same keys as `coordinates` mapping each
         name to a 1d array of heading angles in radians
 
     filter_size: int, default=9
-        Size of median filter applied to ``centroids`` and ``headings``
+        Size of median filter applied to `centroids` and `headings`
 
     Returns
     -------
     trajectories: list
-        List or array of trajectories (a list is used when ``post=None``, 
+        List or array of trajectories (a list is used when `post=None`, 
         else an array)
     """
     if centroids is not None and headings is not None:
         centroids,headings = filter_centroids_headings(
             centroids, headings, filter_size=filter_size)
         
     if post is None:
@@ -576,48 +574,48 @@
           function is computed in trajectory space and compared to the 
           overall density across all syllables. An exemplar instance
           that maximizes this ratio is chosen for each syllable, and
           its nearest neighbors are randomly sampled. 
 
     pca_samples: int, default=50000
         Number of trajectories to sample when fitting a PCA model for 
-        density estimation (used when ``mode='density'``)
+        density estimation (used when `mode='density'`)
 
     pca_dim: int, default=4
         Number of principal components to use for density estimation
-        (used when ``mode='density'``)
+        (used when `mode='density'`)
 
     n_neighbors: int, defualt=50
         Number of neighbors to use for density estimation and for 
         sampling the neighbors of the examplar syllable instance
-        (used when ``mode='density'``)
+        (used when `mode='density'`)
 
     coordinates, pre, pos, centroids, heading, filter_size
         Passed to :py:func:`keypoint_moseq.util.get_trajectories`
 
     Returns
     -------
     sampled_instances: dict
-        Dictionary in the same format as ``syllable_instances`` 
+        Dictionary in the same format as `syllable_instances` 
         mapping each syllable to a list of sampled instances.
     """
     assert mode in ['random','density']
     assert all([len(v)>=num_samples for v in syllable_instances.values()])
     assert n_neighbors>=num_samples
 
     if mode=='random':
         sampled_instances = {syllable: [instances[i] for i in np.random.choice(
             len(instances), num_samples, replace=False
         )] for syllable,instances in syllable_instances.items()}
         return sampled_instances
     
     elif mode=='density':
         assert not (coordinates is None or headings is None or centroids is None), fill(
-            '``coordinates``, ``headings`` and ``centroids`` are required when '
-            '``mode == "density"``')
+            '`coordinates`, `headings` and `centroids` are required when '
+            '`mode == "density"`')
 
         for key in coordinates.keys():
             outliers = np.isnan(coordinates[key]).any(-1)
             coordinates[key] = interpolate_keypoints(coordinates[key], outliers)
 
         trajectories = {syllable: get_trajectories(
             instances, coordinates, pre=pre, post=post, 
@@ -696,15 +694,15 @@
     coordinates : ndarray of shape (num_frames, num_keypoints, dim)
         Keypoint observations.
     outliers : ndarray of shape (num_frames, num_keypoints)
         Binary indicator whose true entries are outlier points.
         
     Returns
     -------
-    interpolated_coordinates : ndarray with same shape as ``coordinates``
+    interpolated_coordinates : ndarray with same shape as `coordinates`
         Keypoint observations with outliers imputed.
     """  
     interpolated_coordinates = np.zeros_like(coordinates)
     for i in range(coordinates.shape[1]):
         interpolated_coordinates[:,i,:] = interpolate_along_axis(
             np.arange(coordinates.shape[0]),
             np.nonzero(~outliers[:,i])[0],
@@ -713,15 +711,15 @@
 
 
 
 def filtered_derivative(Y_flat, ksize, axis=0):
     """
     Compute the filtered derivative of a signal along a given axis.
 
-    When ``ksize=3``, for example, the filtered derivative is
+    When `ksize=3`, for example, the filtered derivative is
 
     .. math::
 
         \dot{y_t} = \frac{1}{3}( x_{t+3}+x_{t+2}+x_{t+1}-x_{t-1}-x_{t-2}-x_{t-3})
 
     Parameters
     ----------
```

### Comparing `keypoint-moseq-0.0.4/keypoint_moseq/viz.py` & `keypoint-moseq-0.0.5/keypoint_moseq/viz.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 import warnings
 import logging
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.ndimage import gaussian_filter1d
 from vidio.read import OpenCVReader
 from textwrap import fill
+plt.rcParams['figure.dpi'] = 100
 
 from keypoint_moseq.util import (
     get_edges, get_durations, get_frequencies, reindex_by_bodyparts,
     find_matching_videos, get_syllable_instances, sample_instances,
     filter_centroids_headings, get_trajectories, interpolate_keypoints,
     interpolate_along_axis
 )
 from keypoint_moseq.io import load_results
 from jax_moseq.models.keypoint_slds import center_embedding
 
 # simple warning formatting
-plt.rcParams['figure.dpi'] = 100
 warnings.formatwarning = lambda msg, *a: str(msg)
 
 # suppress warnings from imageio
 logging.getLogger().setLevel(logging.ERROR)
 
 
 
@@ -75,18 +75,18 @@
     Parameters
     ----------
     pca : :py:func:`sklearn.decomposition.PCA`
         Fitted PCA model
 
     savefig : bool, True
         Whether to save the figure to a file. If true, the figure is 
-        saved to ``{project_dir}/pca_scree.pdf``.
+        saved to `{project_dir}/pca_scree.pdf`.
 
     project_dir : str, default=None
-        Path to the project directory. Required if ``savefig`` is True.
+        Path to the project directory. Required if `savefig` is True.
 
     fig_size : tuple, (2.5,2)
         Size of the figure in inches.
 
     Returns 
     -------
     fig : :py:class:`matplotlib.figure.Figure`
@@ -98,15 +98,15 @@
     plt.ylabel('Explained variance')
     plt.gcf().set_size_inches(fig_size)
     plt.grid()
     plt.tight_layout()
     
     if savefig:
         assert project_dir is not None, fill(
-            'The ``savefig`` option requires a ``project_dir``')
+            'The `savefig` option requires a `project_dir`')
         plt.savefig(os.path.join(project_dir,'pca_scree.pdf'))
     plt.show()
     return fig
           
 def plot_pcs(pca, *, use_bodyparts, skeleton, keypoint_colormap='autumn',
              savefig=True, project_dir=None, scale=1, plot_n_pcs=10, 
              axis_size=(2,1.5), ncols=5, node_size=30.0, linewidth=2.0, **kwargs):
@@ -130,19 +130,19 @@
         pair of bodypart names.
 
     keypoint_colormap : str
         Name of a matplotlib colormap to use for coloring the keypoints.
 
     savefig : bool, True
         Whether to save the figure to a file. If true, the figure is
-        saved to ``{project_dir}/pcs-{xy/xz/yz}.pdf`` (``xz`` and ``yz``
+        saved to `{project_dir}/pcs-{xy/xz/yz}.pdf` (`xz` and `yz`
         are only included for 3D data).
 
     project_dir : str, default=None
-        Path to the project directory. Required if ``savefig`` is True.
+        Path to the project directory. Required if `savefig` is True.
 
     scale : float, default=0.5
         Scale factor for the perturbation of the mean pose.
 
     plot_n_pcs : int, default=10
         Number of PCs to plot. 
 
@@ -194,46 +194,46 @@
             ax.axis('off')
         
         fig.set_size_inches((axis_size[0]*ncols, axis_size[1]*nrows))
         plt.tight_layout()
         
         if savefig:
             assert project_dir is not None, fill(
-                'The ``savefig`` option requires a ``project_dir``')
+                'The `savefig` option requires a `project_dir`')
             plt.savefig(os.path.join(project_dir,f'pcs-{name}.pdf'))
         plt.show()
         
 
 def plot_syllable_frequencies(results=None, path=None, project_dir=None, 
                               name=None, use_reindexed=True, minlength=10,
                               min_frequency=0.005):
     """
     Plot a histogram showing the frequency of each syllable.
     
     Caller must provide a results dictionary, a path to a results .h5,
     or a project directory and model name, in which case the results are
-    loaded from ``{project_dir}/{name}/results.h5``.
+    loaded from `{project_dir}/{name}/results.h5`.
 
     Parameters
     ----------
     results : dict, default=None
         Dictionary containing modeling results for a dataset (see
         :py:func:`keypoint_moseq.fitting.apply_model`)
 
     name: str, default=None
-        Name of the model. Required to load results if ``results`` is 
-        None and ``path`` is None. 
+        Name of the model. Required to load results if `results` is 
+        None and `path` is None. 
         
     project_dir: str, default=None
-        Project directory. Required to load results if ``results`` is 
-        None and ``path`` is None. 
+        Project directory. Required to load results if `results` is 
+        None and `path` is None. 
 
     path: str, default=None
         Path to a results file. If None, results will be loaded from
-        ``{project_dir}/{name}/results.h5``.
+        `{project_dir}/{name}/results.h5`.
 
     use_reindexed: bool, default=True
         Whether to use label syllables by their frequency rank (True) or
         or their original label (False). When reindexing, "0"  represents
         the most frequent syllable).
 
     minlength: int, default=10
@@ -273,33 +273,33 @@
                                name=None, use_reindexed=True, lim=None,
                                num_bins=30, fps=None):
     """
     Plot a histogram showing the frequency of each syllable.
     
     Caller must provide a results dictionary, a path to a results .h5,
     or a project directory and model name, in which case the results are
-    loaded from ``{project_dir}/{name}/results.h5``.
+    loaded from `{project_dir}/{name}/results.h5`.
 
     Parameters
     ----------
     results : dict, default=None
         Dictionary containing modeling results for a dataset (see
         :py:func:`keypoint_moseq.fitting.apply_model`)
 
     name: str, default=None
-        Name of the model. Required to load results if ``results`` is 
-        None and ``path`` is None. 
+        Name of the model. Required to load results if `results` is 
+        None and `path` is None. 
         
     project_dir: str, default=None
-        Project directory. Required to load results if ``results`` is 
-        None and ``path`` is None. 
+        Project directory. Required to load results if `results` is 
+        None and `path` is None. 
 
     path: str, default=None
         Path to a results file. If None, results will be loaded from
-        ``{project_dir}/{name}/results.h5``.
+        `{project_dir}/{name}/results.h5`.
 
     lim: tuple, default=None
         x-axis limits as a pair of ints (in units of frames). If None,
         the limits are set to (0, 95th-percentile).
 
     num_bins: int, default=30
         Number of bins in the histogram.
@@ -363,29 +363,29 @@
         - State sequence history
             The state sequence across iterations in a random window 
             (a new window is selected each time the progress is plotted). 
 
     Parameters
     ----------
     model : dict
-        Model dictionary containing ``states``
+        Model dictionary containing `states`
 
     data : dict
-        Data dictionary containing ``mask``
+        Data dictionary containing `mask`
 
     history : dict
         Dictionary mapping iteration number to saved model dictionaries
 
     iteration : int
         Current iteration of model fitting
 
     savefig : bool, default=True
         Whether to save the figure to a file. If true, the figure is
-        either saved to ``path`` or, to ``{project_dir}/{name}-progress.pdf``
-        if ``path`` is None.
+        either saved to `path` or, to `{project_dir}/{name}-progress.pdf`
+        if `path` is None.
 
     fig_size : tuple of float, default=None
         Size of the figure in inches. 
         
     seq_length : int, default=600
         Length of the state sequence history plot.
 
@@ -470,16 +470,16 @@
     fig.suptitle(title)        
     fig.set_size_inches(fig_size)
     plt.tight_layout()
     
     if savefig:
         if path is None:
             assert name is not None and project_dir is not None, fill(
-                'The ``savefig`` option requires either a ``path`` '
-                'or a ``name`` and ``project_dir``')
+                'The `savefig` option requires either a `path` '
+                'or a `name` and `project_dir`')
             path = os.path.join(project_dir,name,'fitting_progress.pdf')
         plt.savefig(path)  
     plt.show()
 
     return fig,axs
 
     
@@ -541,33 +541,33 @@
     Grid movies show many instances of a syllable. Each instance
     contains a snippet of a video, centered on the animal and synchronized
     to the onset of the syllable. A dot appears at syllable onset and 
     disappears at syllable offset.
 
     Parameters
     ----------
-    instances: list of tuples ``(key, start, end)``
+    instances: list of tuples `(key, start, end)`
         List of syllable instances to include in the grid movie,
         where each instance is specified as a tuple with the video 
         name, start frame and end frame. The list must have length
-        ``rows*cols``. The video names must also be keys in ``videos``.
+        `rows*cols`. The video names must also be keys in `videos`.
         
     rows: int, cols : int
         Number of rows and columns in the grid movie grid
     
     videos: dict
         Dictionary mapping video names to video readers. Frames from
-        each reader should be accessible via ``__getitem__(int or slice)``
+        each reader should be accessible via `__getitem__(int or slice)`
 
     centroids: dict
-        Dictionary mapping video names to arrays of shape ``(n_frames, 2)``
+        Dictionary mapping video names to arrays of shape `(n_frames, 2)`
         with the x,y coordinates of animal centroid on each frame
 
     headings: dict
-        Dictionary mapping video names to arrays of shape ``(n_frames,)``
+        Dictionary mapping video names to arrays of shape `(n_frames,)`
         with the heading of the animal on each frame (in radians)
 
     dot_color: tuple of ints, default=(255,255,255)
         RGB color of the dot indicating syllable onset and offset
 
     dot_radius: int, default=4
         Radius of the dot indicating syllable onset and offset
@@ -581,36 +581,36 @@
 
     post: int, default=60
         Number of frames after syllable onset to include in the movie
 
     coordinates: dict, default=None
         Dictionary mapping session names to keypoint coordinates as 
         ndarrays of shape (n_frames, n_bodyparts, 2). Required when
-        ``overlay_trajectory=True``
+        `overlay_trajectory=True`
 
     overlay_trajectory: bool, default=False
         Whether to overlay trajectory of keypoints on the grid movie. 
-        If True, ``coordinates`` must be provided.
+        If True, `coordinates` must be provided.
 
     overlay_options: dict, default={}
         Dictionary of options for overlaying trajectory (see
         :py:func:`keypoint_moseq.viz.overlay_trajectory_on_video`).
 
     plot_options: dict, default={}
         Dictionary of options for overlaying trajectory (see 
         :py:func:`keypoint_moseq.viz.overlay_keypoints_on_image`).
 
     Returns
     -------
-    frames: array of shape ``(rows, cols, post+pre, window_size, window_size, 3)``
+    frames: array of shape `(rows, cols, post+pre, window_size, window_size, 3)`
         Array of frames in the grid movie
     """
     if overlay_trajectory:
         assert coordinates is not None, fill(
-            '``coordinates`` must be provided if ``overlay_trajectory`` is True')
+            '`coordinates` must be provided if `overlay_trajectory` is True')
 
         trajectories = get_trajectories(
             instances, coordinates, pre=pre, post=post, 
             centroids=centroids, headings=headings)
             
     tiles = []
     for i,(key,start,end) in enumerate(instances):
@@ -643,18 +643,18 @@
     """
     Generate grid movies for a modeled dataset.
 
     Grid movies show many instances of a syllable and are useful in
     figuring out what behavior the syllable captures 
     (see :py:func:`keypoint_moseq.viz.grid_movie`). This method
     generates a grid movie for each syllable that is used sufficiently
-    often (i.e. has at least ``rows*cols`` instances with duration
-    of at least ``min_duration`` and an overall frequency of at least
-    ``min_frequency``). The grid movies are saved to ``output_dir`` if 
-    specified, or else to ``{project_dir}/{name}/grid_movies``.
+    often (i.e. has at least `rows*cols` instances with duration
+    of at least `min_duration` and an overall frequency of at least
+    `min_frequency`). The grid movies are saved to `output_dir` if 
+    specified, or else to `{project_dir}/{name}/grid_movies`.
 
     Parameters
     ----------
     results: dict, default=None
         Dictionary containing modeling results for a dataset (see
         :py:func:`keypoint_moseq.fitting.apply_model`). Must have
         the format::
@@ -665,49 +665,49 @@
                     'syllables_reindexed':    array of shape (n_frames,),
                     'centroid':               array of shape (n_frames, dim),
                     'heading' :               array of shape (n_frames,), 
                 },
                 ...  
             }
             
-        - ``syllables`` is required if ``use_reindexed=False``
-        - ``syllables_reindexed`` is required if ``use_reindexed=True``
-        - ``centroid`` is always required
-        - ``heading`` is always required
+        - `syllables` is required if `use_reindexed=False`
+        - `syllables_reindexed` is required if `use_reindexed=True`
+        - `centroid` is always required
+        - `heading` is always required
 
-        If ``results=None``, results will be loaded using either 
-        ``results_path`` or  ``project_dir`` and ``name``.
+        If `results=None`, results will be loaded using either 
+        `results_path` or  `project_dir` and `name`.
 
     output_dir: str, default=None
         Directory where grid movies should be saved. If None, grid
-        movies will be saved to ``{project_dir}/{name}/grid_movies``.
+        movies will be saved to `{project_dir}/{name}/grid_movies`.
 
     name: str, default=None
-        Name of the model. Required to load results if ``results`` is 
-        None and ``results_path`` is None. Required to save grid movies 
-        if ``output_dir`` is None.
+        Name of the model. Required to load results if `results` is 
+        None and `results_path` is None. Required to save grid movies 
+        if `output_dir` is None.
         
     project_dir: str, default=None
-        Project directory. Required to load results if ``results`` is 
-        None and ``results_path`` is None. Required to save grid movies 
-        if ``output_dir`` is None.
+        Project directory. Required to load results if `results` is 
+        None and `results_path` is None. Required to save grid movies 
+        if `output_dir` is None.
 
     results_path: str, default=None
         Path to a results file. If None, results will be loaded from
-        ``{project_dir}/{name}/results.h5``.
+        `{project_dir}/{name}/results.h5`.
 
     video_dir: str, default=None
         Directory containing videos of the modeled data (see 
         :py:func:`keypoint_moseq.io.find_matching_videos`). If None,
-        a dictionary of ``video_paths`` must be provided.
+        a dictionary of `video_paths` must be provided.
 
     video_paths: dict, default=None
         Dictionary mapping session names to video paths. The session 
-        names must correspond to keys in ``results['syllables']``. If
-        None, a ``video_dir`` must be provided.
+        names must correspond to keys in `results['syllables']`. If
+        None, a `video_dir` must be provided.
 
     filter_size: int, default=9
         Size of the median filter applied to centroids and headings
 
     min_frequency: float, default=0.005
         Minimum frequency of a syllable to be included in the grid movies.
 
@@ -723,35 +723,35 @@
     sampling_options: dict, default={}
         Dictionary of options for sampling syllable instances (see
         :py:func:`keypoint_moseq.util.sample_instances`).
     
     coordinates: dict, default=None
         Dictionary mapping session names to keypoint coordinates as 
         ndarrays of shape (n_frames, n_bodyparts, 2). Required when
-        ``overlay_trajectory=True``, and for density-based sampling 
-        (i.e. when ``sampling_options['mode']=='density'``; see 
+        `overlay_trajectory=True`, and for density-based sampling 
+        (i.e. when `sampling_options['mode']=='density'`; see 
         :py:func:`keypoint_moseq.util.sample_instances`).
 
     bodyparts: list of str, default=None
-        List of bodypart names in ``coordinates``. Required when 
-        ``coordinates`` is provided and bodyparts were reindexed 
+        List of bodypart names in `coordinates`. Required when 
+        `coordinates` is provided and bodyparts were reindexed 
         for modeling. 
 
     use_bodyparts: list of str, default=None
         Ordered list of bodyparts used for modeling. Required when 
-        ``coordinates`` is provided and bodyparts were reindexed 
+        `coordinates` is provided and bodyparts were reindexed 
         for modeling. 
 
     skeleton : list, default=[]
         List of edges that define the skeleton, where each edge is a
         pair of bodypart names or a pair of indexes.
 
     overlay_trajectory: bool, default=False
         Whether to overlay trajectory of keypoints on the grid movie. 
-        If True, ``coordinates`` must be provided.
+        If True, `coordinates` must be provided.
 
     overlay_options: dict, default={}
         Dictionary of options for overlaying trajectory (see
         :py:func:`keypoint_moseq.viz.overlay_trajectory_on_video`).
 
     plot_options: dict, default={}
         Dictionary of options for overlaying trajectory (see 
@@ -764,24 +764,24 @@
     rows, cols, pre, post, dot_radius, dot_color, window_size
         See :py:func:`keypoint_moseq.viz.grid_movie`
 
     video_extension: str, default=None
         Preferred video extension (passed to :py:func:`keypoint_moseq.util.find_matching_videos`)
     """
     assert (video_dir is not None) or (video_paths is not None), fill(
-        'You must provide either ``video_dir`` or ``video_paths``') 
+        'You must provide either `video_dir` or `video_paths`') 
 
     if overlay_trajectory:
         assert coordinates is not None, fill(
-            '``coordinates`` must be provided if ``overlay_trajectory`` is True')     
+            '`coordinates` must be provided if `overlay_trajectory` is True')     
     
     if output_dir is None:
         assert project_dir is not None and name is not None, fill(
-            'Either specify the ``output_dir`` where grid movies should '
-            'be saved or include a ``project_dir`` and ``name``')
+            'Either specify the `output_dir` where grid movies should '
+            'be saved or include a `project_dir` and `name`')
         output_dir = os.path.join(project_dir,name, 'grid_movies')
     if not os.path.exists(output_dir): os.makedirs(output_dir)
     print(f'Writing grid movies to {output_dir}')
     
     if not (bodyparts is None or use_bodyparts is None or coordinates is None):
         coordinates = reindex_by_bodyparts(coordinates, bodyparts, use_bodyparts)
 
@@ -819,15 +819,15 @@
     centroids,headings = filter_centroids_headings(
         centroids, headings, filter_size=filter_size)
     
     if len(skeleton)>0 and overlay_trajectory: 
         if isinstance(skeleton[0][0],str):
             assert use_bodyparts is not None, fill(
                 'If skeleton edges are specified using bodypart names, '
-                '``use_bodyparts`` must be specified')
+                '`use_bodyparts` must be specified')
             plot_options['edges'] = get_edges(use_bodyparts, skeleton)
         else: plot_options['edges'] = skeleton
     
     for syllable,instances in tqdm.tqdm(
         sampled_instances.items(), desc='Generating grid movies'):
         
         frames = grid_movie(
@@ -843,37 +843,37 @@
         
 def get_limits(coordinates, pctl=1, blocksize=None,
                left=0.2, right=0.2, top=0.2, bottom=0.2):
     """
     Get axis limits based on the coordinates of all keypoints.
 
     For each axis, limits are determined using the percentiles
-    ``pctl`` and ``100-pctl`` and then padded by ``padding``.
+    `pctl` and `100-pctl` and then padded by `padding`.
 
     Parameters
     ----------
     coordinates: ndarray or dict
         Coordinates as an ndarray of shape (..., 2), or a dict
         with values that are ndarrays of shape (..., 2).
 
     pctl: float, default=1
         Percentile to use for determining the axis limits.
 
     blocksize: int, default=None
         Axis limits are cast to integers and padded so that the width
-        and height are multiples of ``blocksize``. This is useful
+        and height are multiples of `blocksize`. This is useful
         when they are used for generating cropped images for a video. 
         
     left, right, top, bottom: float, default=0.1
         Fraction of the axis range to pad on each side.
 
     Returns
     -------
     lims: ndarray of shape (2,dim)
-        Axis limits, in the format ``[[xmin,ymin,...],[xmax,ymax,...]]``.
+        Axis limits, in the format `[[xmin,ymin,...],[xmax,ymax,...]]`.
     """
     if isinstance(coordinates, dict):
         X = np.concatenate(list(coordinates.values())).reshape(-1,2)
     else:
         X = coordinates.reshape(-1,2)
 
     xmin,ymin = np.nanpercentile(X, pctl, axis=0)
@@ -929,22 +929,22 @@
 
     edges: list of tuples, default=[]
         List of edges, where each edge is a tuple of two integers
 
     lims: ndarray
         Axis limits used for all the trajectory plots. The limits 
         should be provided as an array of shape (2,2) with the format
-        ``[[xmin,ymin],[xmax,ymax]]``.
+        `[[xmin,ymin],[xmax,ymax]]`.
 
     n_cols: int, default=4
         Number of columns in the figure (used when plotting multiple
         trajectories).
 
     invert: bool, default=False
-        Determines the background color of the figure. If ``True``,
+        Determines the background color of the figure. If `True`,
         the background will be black.
 
     keypoint_colormap : str or list
         Name of a matplotlib colormap or a list of colors as (r,b,g) 
         tuples in the same order as as the keypoints.
 
     node_size: int, default=50
@@ -959,20 +959,20 @@
     num_timesteps: int, default=10
         Number of timesteps to plot for each trajectory. The pose 
         at each timestep is determined by linearly interpolating
         between the keypoints.
 
     plot_width: int, default=4
         Width of each trajectory plot in inches. The height  is 
-        determined by the aspect ratio of ``lims``. The final figure 
-        width is ``fig_width * min(n_cols, len(X))``.
+        determined by the aspect ratio of `lims`. The final figure 
+        width is `fig_width * min(n_cols, len(X))`.
 
     overlap: tuple of float, default=(0.2,0)
         Amount of overlap between each trajectory plot as a tuple 
-        with the format ``(x_overlap, y_overlap)``. The values should
+        with the format `(x_overlap, y_overlap)`. The values should
         be between 0 and 1.
         
     return_rasters: bool, default=False
         Rasterize the matplotlib canvas after plotting each step of
         the trajecory. This is used to generate an animated video/gif
         of the trajectory. 
 
@@ -1067,23 +1067,23 @@
     """
     Generate trajectory plots for a modeled dataset.
 
     Each trajectory plot shows a sequence of poses along the average
     trajectory through latent space associated with a given syllable.
     A separate figure (and gif, optionally) is saved for each syllable, 
     along with a single figure showing all syllables in a grid. The 
-    plots are saved to ``{output_dir}`` if it is provided, otherwise 
-    they are saved to ``{project_dir}/{name}/trajectory_plots``.
+    plots are saved to `{output_dir}` if it is provided, otherwise 
+    they are saved to `{project_dir}/{name}/trajectory_plots`.
 
     Parameters
     ----------
     coordinates : dict, default=None
         Dictionary mapping session names to keypoint coordinates as 
         ndarrays of shape (n_frames, n_bodyparts, 2). Required if
-        ``use_estimated_coords=False``.
+        `use_estimated_coords=False`.
 
     results: dict, default=None
         Dictionary containing modeling results for a dataset (see
         :py:func:`keypoint_moseq.fitting.apply_model`). Must have
         the format::
 
             {
@@ -1093,40 +1093,40 @@
                     'syllables_reindexed':    array of shape (n_frames,),
                     'centroid':               array of shape (n_frames, dim),
                     'heading' :               array of shape (n_frames,), 
                 },
                 ...  
             }
             
-        - ``syllables`` is required if ``use_reindexed=False``
-        - ``syllables_reindexed`` is required if ``use_reindexed=True``
-        - ``centroid`` is always required
-        - ``heading`` is always required
-        - ``estimated_coordinates`` is required if ``use_estimated_coords=True``
+        - `syllables` is required if `use_reindexed=False`
+        - `syllables_reindexed` is required if `use_reindexed=True`
+        - `centroid` is always required
+        - `heading` is always required
+        - `estimated_coordinates` is required if `use_estimated_coords=True`
 
-        If ``results=None``, results will be loaded using either 
-        ``results_path`` or  ``project_dir`` and ``name``.
+        If `results=None`, results will be loaded using either 
+        `results_path` or  `project_dir` and `name`.
 
     output_dir: str, default=None
         Directory where trajectory plots should be saved. If None, 
-        plots will be saved to ``{project_dir}/{name}/trajectory_plots``.
+        plots will be saved to `{project_dir}/{name}/trajectory_plots`.
 
     name: str, default=None
-        Name of the model. Required to load results if ``results`` is 
-        None and ``results_path`` is None. Required to save trajectory
-        plots if ``output_dir`` is None.
+        Name of the model. Required to load results if `results` is 
+        None and `results_path` is None. Required to save trajectory
+        plots if `output_dir` is None.
 
     project_dir: str, default=None
-       Project directory. Required to load results if ``results`` is 
-        None and ``results_path`` is None. Required to save trajectory
-        plots if ``output_dir`` is None.
+       Project directory. Required to load results if `results` is 
+        None and `results_path` is None. Required to save trajectory
+        plots if `output_dir` is None.
 
     results_path: str, default=None
         Path to a results file. If None, results will be loaded from
-        ``{project_dir}/{name}/results.h5``.
+        `{project_dir}/{name}/results.h5`.
 
     pre: int, default=5, post: int, default=15
         Defines the temporal window around syllable onset for 
         computing the average trajectory. Note that the window is 
         independent of the actual duration of the syllable.
 
     min_frequency: float, default=0.005
@@ -1138,28 +1138,28 @@
 
     use_reindexed: bool, default=True
         Whether to use label syllables by their frequency rank (True) or
         or their original label (False). When reindexing, "0"  represents
         the most frequent syllable).
 
     bodyparts: list of str, default=None
-        List of bodypart names in ``coordinates``. 
+        List of bodypart names in `coordinates`. 
 
     use_bodyparts: list of str, default=None
         Ordered list of bodyparts to include in trajectory plot.
         If None, all bodyparts will be included.
 
     skeleton : list, default=[]
         List of edges that define the skeleton, where each edge is a
         pair of bodypart names or a pair of indexes.
 
     num_samples: int, default=40
         Number of samples to used to compute the average trajectory.
-        Also used to set ``n_neighbors`` when sampling syllable instances
-        in ``density`` mode. 
+        Also used to set `n_neighbors` when sampling syllable instances
+        in `density` mode. 
 
     keypoint_colormap : str
         Name of a matplotlib colormap to use for coloring the keypoints.
 
     plot_options: dict, default={}
         Dictionary of options for trajectory plots (see
         :py:func:`keypoint_moseq.util.plot_trajectories`).
@@ -1181,26 +1181,26 @@
         Whether to save an animated gif of the trajectory plots.
         
     save_mp4s: bool, default=False
         Whether to save videos of the trajectory plots as .mp4 files
         
     fps: int, default=30
         Framerate of the videos from which keypoints were derived.
-        Used to set the framerate of gifs when ``save_gif=True``.
+        Used to set the framerate of gifs when `save_gif=True`.
         
     projection_planes: list (subset of ['xy', 'yz', 'xz']), default=['xy','xz']
         For 3D data, defines the 2D plane(s) on which to project keypoint 
         coordinates. A separate plot will be saved for each plane with 
         the name of the plane (e.g. 'xy') as a suffix. This argument is 
         ignored for 2D data.
     """
     if output_dir is None:
         assert project_dir is not None and name is not None, fill(
-            'Either specify the ``output_dir`` where trajectory plots '
-            'should be saved or include a ``project_dir`` and ``name``')
+            'Either specify the `output_dir` where trajectory plots '
+            'should be saved or include a `project_dir` and `name`')
         output_dir = os.path.join(project_dir,name, 'trajectory_plots')
     if not os.path.exists(output_dir): os.makedirs(output_dir)
     print(f'Saving trajectory plots to {output_dir}')
         
     if results is None: results = load_results(
         name=name, project_dir=project_dir, path=results_path)
 
@@ -1237,15 +1237,15 @@
         ) for syllable,instances in sampled_instances.items()}
 
     edges = []
     if len(skeleton)>0: 
         if isinstance(skeleton[0][0],str):
             assert use_bodyparts is not None, fill(
                 'If skeleton edges are specified using bodypart names, '
-                '``use_bodyparts`` must be specified')
+                '`use_bodyparts` must be specified')
             edges = get_edges(use_bodyparts, skeleton)
         else: edges = skeleton
 
     syllables = sorted(trajectories.keys())
     titles = [f'Syllable {syllable}' for syllable in syllables]
     Xs = np.nanmean(np.array([trajectories[syllable] for syllable in syllables]),axis=1)  
     
@@ -1273,17 +1273,17 @@
                     return_rasters=(save_gifs or save_mp4s),
                     **plot_options)
 
                 plt.savefig(os.path.join(output_dir, f'{title}{suffix}.pdf'))
                 plt.close(fig=fig)
 
                 if save_gifs:
-                    use_fps = len(rasters)/(pre+post)*fps
+                    frame_duration = int(1000 * (pre+post) / len(rasters) / fps)
                     path = os.path.join(output_dir, f'{title}{suffix}.gif')
-                    imageio.mimsave(path, rasters, fps=use_fps)
+                    imageio.mimsave(path, rasters, duration=frame_duration)
                 if save_mp4s:
                     use_fps = len(rasters)/(pre+post)*fps
                     path = os.path.join(output_dir, f'{title}{suffix}.mp4')
                     write_video_clip(rasters, path, fps=use_fps)
                     
 
         # grid plot
@@ -1292,27 +1292,27 @@
             return_rasters=(save_gifs or save_mp4s),
             **plot_options)
 
         plt.savefig(os.path.join(output_dir, f'all_trajectories{suffix}.pdf'))
         plt.show()
 
         if save_gifs:
-            use_fps = len(rasters)/(pre+post)*fps
+            frame_duration = int(1000 * (pre+post) / len(rasters) / fps)
             path = os.path.join(output_dir, f'all_trajectories{suffix}.gif')
-            imageio.mimsave(path, rasters, fps=use_fps)
+            imageio.mimsave(path, rasters, duration=frame_duration)
         if save_mp4s:
             use_fps = len(rasters)/(pre+post)*fps
             path = os.path.join(output_dir, f'all_trajectories{suffix}.mp4')
             write_video_clip(rasters, path, fps=use_fps)
 
 
 
 def overlay_keypoints_on_image(
     image, coordinates, edges=[], keypoint_colormap='autumn',
-    node_size=3, line_width=2, copy=False, opacity=1.0):
+    node_size=2, line_width=1, copy=False, opacity=1.0):
     """
     Overlay keypoints on an image.
 
     Parameters
     ----------
     image: ndarray of shape (height, width, 3)
         Image to overlay keypoints on.
@@ -1368,15 +1368,15 @@
     if opacity<1.0:
         image = cv2.addWeighted(image, 1-opacity, canvas, opacity, 0)
     return image
 
 
 def overlay_trajectory_on_video(
         frames, trajectory, smoothing_kernel=1, highlight=None, 
-        min_opacity=0.2, max_opacity=1, num_ghosts=10, interval=2, 
+        min_opacity=0.2, max_opacity=1, num_ghosts=5, interval=2, 
         plot_options={}):
     
     """
     Overlay a trajectory of keypoints on a video.
     """
     if smoothing_kernel > 0:
         trajectory = gaussian_filter1d(trajectory, smoothing_kernel, axis=0)
@@ -1411,23 +1411,23 @@
         Array of keypoint coordinates.
 
     skeleton: list of tuples, default=[]
         List of edges that define the skeleton, where each edge is a
         pair of bodypart names or a pair of indexes.
 
     bodyparts: list of str, default=None
-        List of bodypart names in ``coordinates``. Required if
-        ``skeleton`` is defined using bodypart names.
+        List of bodypart names in `coordinates`. Required if
+        `skeleton` is defined using bodypart names.
 
     use_bodyparts: list of str, default=None
         Subset of bodyparts to plot. If None, all bodyparts are plotted.
 
     output_path: str, default=None
         Path to save the video. If None, the video is saved to
-        ``video_path`` with the suffix ``_keypoints``.
+        `video_path` with the suffix `_keypoints`.
 
     show_frame_numbers: bool, default=True
         Whether to overlay the frame number in the video.
 
     text_color: tuple of int, default=(255,255,255)
         Color for the frame number overlay.
 
@@ -1489,34 +1489,37 @@
                 writer.append_data(image)
 
 
 
 
 
 def crowd_movie(
-    instances, coordinates, lims, pre=30, post=60,
+    instances, coordinates, centroids, lims, pre=30, post=60,
     edges=[], plot_options={}):
     """
     Generate a crowd movie.
 
     Crowd movies show many instances of a syllable by animating
     their keypoint trajectories in a common coordinate system.
     The trajectories are synchronized to syllable onset. The opacity 
     of each instance increases at syllable onset and decreases at
     syllable offset.
 
     Parameters
     ----------
-    instances: list of tuples ``(key, start, end)``
+    instances: list of tuples `(key, start, end)`
         List of syllable instances to include in the grid movie,
         where each instance is specified as a tuple with the session
         name, start frame and end frame. 
     
-    coordinates: dict of ndarray of shape (num_frames, num_keypoints, dim)
+    coordinates: dict of ndarrays of shape (num_frames, num_keypoints, dim)
         Dictionary of keypoint coordinates, where each key is a session name.
+        
+    centroids: dict of ndarrays of shape (num_frames, dim)
+        Dictionary of animal centroids, where each key is a session name.
 
     lims: array of shape (2, dim)
         Axis limits for plotting keypoints in the crowd movies. 
 
     pre: int, default=30
         Number of frames before syllable onset to include in the movie
 
@@ -1525,37 +1528,39 @@
 
     plot_options: dict, default={}
         Dictionary of options for rendering keypoints in the crowd
         movies (see :py:func:`keypoint_moseq.util.overlay_keypoints_on_image`).
 
     Returns
     -------
-    frames: array of shape ``(post+pre, height, width, 3)``
-        Array of frames in the grid movie. ``width`` and 
-        ``height`` are determined by ``lims``.
+    frames: array of shape `(post+pre, height, width, 3)`
+        Array of frames in the grid movie. `width` and 
+        `height` are determined by `lims`.
     """
     dim = coordinates[instances[0][0]].shape[2]
     if dim == 3: warnings.warn(fill(
         'Crowd movies are only supported for 2D keypoints. '
         'Only the X and Y coordinates will be used.'))
 
     h, w = (lims[1]-lims[0]).astype(int)
     frames = np.zeros((post+pre, w, h, 3), dtype=np.uint8)
 
     for key, start, end in instances:
         xy = coordinates[key][start-pre:start+post,:,:2]
-        xy = (np.clip(xy, *lims[:,:2]) - lims[0,:2])
+        xy = np.clip(xy, *lims[:,:2]) - lims[0,:2]
         frames = overlay_trajectory_on_video(
             frames, xy, plot_options=plot_options)
 
         dot_radius=5
         dot_color=(255,255,255)
-        centroids = gaussian_filter1d(xy.mean(1),1,axis=0)
+        cen = centroids[key][start-pre:start+post,:2]
+        cen = gaussian_filter1d(cen,1,axis=0)
+        cen = np.clip(cen, *lims[:,:2]) - lims[0,:2]
         for i in range(pre, min(end-start+pre,pre+post)):
-            pos = (int(centroids[i,0]),int(centroids[i,1]))
+            pos = (int(cen[i,0]),int(cen[i,1]))
             frames[i] = cv2.circle(frames[i], pos, dot_radius, dot_color, -1, cv2.LINE_AA)
 
     return frames
 
 
 def generate_crowd_movies(
     coordinates, results=None, output_dir=None, name=None, 
@@ -1568,25 +1573,25 @@
     """
     Generate crowd movies for a modeled dataset.
 
     Crowd movies show many instances of a syllable and are useful in
     figuring out what behavior the syllable captures 
     (see :py:func:`keypoint_moseq.viz.crowd_movie`). This method
     generates a crowd movie for each syllable that is used sufficiently
-    often (i.e. has at least ``num_instances`` instances with duration
-    of at least ``min_duration`` and an overall frequency of at least
-    ``min_frequency``). The crowd movies are saved to ``output_dir`` if 
-    specified, or else to ``{project_dir}/{name}/crowd_movies``.
+    often (i.e. has at least `num_instances` instances with duration
+    of at least `min_duration` and an overall frequency of at least
+    `min_frequency`). The crowd movies are saved to `output_dir` if 
+    specified, or else to `{project_dir}/{name}/crowd_movies`.
 
     Parameters
     ----------
     coordinates: dict, default=None
         Dictionary mapping session names to keypoint coordinates as 
         ndarrays of shape (n_frames, n_bodyparts, 2). Required if
-        ``use_estimated_coords=False``.
+        `use_estimated_coords=False`.
 
     results: dict, default=None
         Dictionary containing modeling results for a dataset (see
         :py:func:`keypoint_moseq.fitting.apply_model`). Must have
         the format::
 
             {
@@ -1596,41 +1601,41 @@
                     'syllables_reindexed':    array of shape (n_frames,),
                     'centroid':               array of shape (n_frames, dim),
                     'heading' :               array of shape (n_frames,), 
                 },
                 ...  
             }
             
-        - ``syllables`` is required if ``use_reindexed=False``
-        - ``syllables_reindexed`` is required if ``use_reindexed=True``
-        - ``centroid`` is required if the sampling mode is 'density'
-        - ``heading`` is required if the sampling mode is 'density'
-        - ``estimated_coordinates`` is required if ``use_estimated_coords=True``
+        - `syllables` is required if `use_reindexed=False`
+        - `syllables_reindexed` is required if `use_reindexed=True`
+        - `centroid` is required if the sampling mode is 'density'
+        - `heading` is required if the sampling mode is 'density'
+        - `estimated_coordinates` is required if `use_estimated_coords=True`
         
 
-        If ``results=None``, results will be loaded using either 
-        ``results_path`` or  ``project_dir`` and ``name``.
+        If `results=None`, results will be loaded using either 
+        `results_path` or  `project_dir` and `name`.
 
     output_dir: str, default=None
         Directory where crowd movies should be saved. If None, 
-        movies will be saved to ``{project_dir}/{name}/crowd_movies``.
+        movies will be saved to `{project_dir}/{name}/crowd_movies`.
 
     name: str, default=None
-        Name of the model. Required to load results if ``results`` is 
-        None and ``results_path`` is None. Required to save crowd
-        movies if ``output_dir`` is None.
+        Name of the model. Required to load results if `results` is 
+        None and `results_path` is None. Required to save crowd
+        movies if `output_dir` is None.
 
     project_dir: str, default=None
-        Project directory. Required to load results if ``results`` is 
-        None and ``results_path`` is None. Required to save crowd
-        movies if ``output_dir`` is None.
+        Project directory. Required to load results if `results` is 
+        None and `results_path` is None. Required to save crowd
+        movies if `output_dir` is None.
 
     results_path: str, default=None
         Path to a results file. If None, results will be loaded from
-        ``{project_dir}/{name}/results.h5``.
+        `{project_dir}/{name}/results.h5`.
 
     num_instances: int, default=15
         Number of syllable instances per crowd movie.
 
     min_frequency: float, default=0.005
         Minimum frequency of a syllable to be included in the crowd movies.
 
@@ -1640,15 +1645,15 @@
 
     use_reindexed: bool, default=True
         Whether to use label syllables by their frequency rank (True) or
         or their original label (False). When reindexing, "0"  represents
         the most frequent syllable).
 
     bodyparts: list of str, default=None
-        List of bodypart names in ``coordinates``. 
+        List of bodypart names in `coordinates`. 
 
     use_bodyparts: list of str, default=None
         Ordered list of bodyparts to include in the crowd
         movies. If None, all bodyparts will be included.
         
     skeleton: list, default=[]
         List of edges that define the skeleton, where each edge is a
@@ -1658,15 +1663,15 @@
         Name of a matplotlib colormap to use for coloring the keypoints.
         
     fps: int, default=30
         Frames per second of the crowd movies.
 
     limits: array, default=None
         Axis limits for plotting keypoints in the crowd movies. If None,
-        limits will be inferred automatically from ``coordinates``.
+        limits will be inferred automatically from `coordinates`.
         
     plot_options: dict, default={}
         Dictionary of options for rendering keypoints in the crowd
         movies (see :py:func:`keypoint_moseq.util.overlay_keypoints_on_image`).
         
     sampling_options: dict, default={}
         Dictionary of options for sampling syllable instances (see
@@ -1674,16 +1679,16 @@
 
     quality: int, default=7
         Quality of the crowd movies. Higher values result in higher
         quality movies but larger file sizes.
     """    
     if output_dir is None:
         assert project_dir is not None and name is not None, fill(
-            'Either specify the ``output_dir`` where crowd movies should '
-            'be saved or include a ``project_dir`` and ``name``')
+            'Either specify the `output_dir` where crowd movies should '
+            'be saved or include a `project_dir` and `name`')
         output_dir = os.path.join(project_dir,name, 'crowd_movies')
     if not os.path.exists(output_dir): os.makedirs(output_dir)
     print(f'Writing crowd movies to {output_dir}')
 
     if results is None: results = load_results(
         name=name, project_dir=project_dir, path=results_path)
         
@@ -1695,27 +1700,32 @@
     syllable_key = 'syllables' + ('_reindexed' if use_reindexed else '')
     syllables = {k:v[syllable_key] for k,v in results.items()}
     plot_options.update({'keypoint_colormap':keypoint_colormap})
 
     if limits is None: 
         limits = get_limits(coordinates, blocksize=16)
 
-    centroids,headings = None,None
     k = list(results.keys())[0]
-    if 'centroid' in results[k]:
-        centroids = {k:v['centroid'] for k,v in results.items()}
     if 'heading' in results[k]:
         headings = {k:v['heading'] for k,v in results.items()}
+    else: headings = None
+        
+    if 'centroid' in results[k]:
+        centroids = {k:v['centroid'] for k,v in results.items()}
+    else:
+        outliers = np.any(np.isnan(coordinates), axis=2)
+        interpolated_coordinates = interpolate_keypoints(coordinates, outliers)
+        centroids = {k:v.mean(1) for k,v in interpolated_coordinates.items()}
 
     edges = []
     if len(skeleton)>0: 
         if isinstance(skeleton[0][0],str):
             assert use_bodyparts is not None, fill(
                 'If skeleton edges are specified using bodypart names, '
-                '``use_bodyparts`` must be specified')
+                '`use_bodyparts` must be specified')
             edges = get_edges(use_bodyparts, skeleton)
         else: edges = skeleton
 
     syllable_instances = get_syllable_instances(
         syllables, pre=pre, post=post, min_duration=min_duration,
         min_frequency=min_frequency, min_instances=num_instances)
     
@@ -1730,13 +1740,13 @@
         syllable_instances, num_instances, coordinates=coordinates, 
         centroids=centroids, headings=headings, **sampling_options)
 
     for syllable,instances in tqdm.tqdm(
         sampled_instances.items(), desc='Generating crowd movies'):
         
         frames = crowd_movie(
-            instances, coordinates, pre=pre, post=post,
+            instances, coordinates, centroids, pre=pre, post=post,
             edges=edges, lims=limits, plot_options=plot_options)
 
         path = os.path.join(output_dir, f'syllable{syllable}.mp4')
         write_video_clip(frames, path, fps=fps, quality=quality)
```

### Comparing `keypoint-moseq-0.0.4/setup.py` & `keypoint-moseq-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='keypoint-moseq',
-    version='0.0.4',
+    version='0.0.5',
     author='Caleb Weinreb',
     author_email='calebsw@gmail.com',
     include_package_data=True,
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent'
```

