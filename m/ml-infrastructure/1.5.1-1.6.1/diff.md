# Comparing `tmp/ml_infrastructure-1.5.1.tar.gz` & `tmp/ml_infrastructure-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_infrastructure-1.5.1.tar", last modified: Sun Apr 16 14:46:08 2023, max compression
+gzip compressed data, was "ml_infrastructure-1.6.1.tar", last modified: Mon May  1 11:22:15 2023, max compression
```

## Comparing `ml_infrastructure-1.5.1.tar` & `ml_infrastructure-1.6.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-04-16 14:46:08.319739 ml_infrastructure-1.5.1/
--rw-rw-r--   0 maple     (1000) maple     (1000)     1067 2023-04-16 13:21:50.000000 ml_infrastructure-1.5.1/LICENSE.rst
--rw-rw-r--   0 maple     (1000) maple     (1000)      581 2023-04-16 14:46:08.319739 ml_infrastructure-1.5.1/PKG-INFO
--rw-rw-r--   0 maple     (1000) maple     (1000)        0 2023-02-25 18:05:38.000000 ml_infrastructure-1.5.1/README.rst
-drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-04-16 14:46:08.315739 ml_infrastructure-1.5.1/ml_infrastructure/
--rw-rw-r--   0 maple     (1000) maple     (1000)      168 2023-02-25 17:41:53.000000 ml_infrastructure-1.5.1/ml_infrastructure/__init__.py
--rw-rw-r--   0 maple     (1000) maple     (1000)     9224 2023-04-15 23:10:23.000000 ml_infrastructure-1.5.1/ml_infrastructure/app.py
--rw-rw-r--   0 maple     (1000) maple     (1000)      180 2022-11-28 03:17:28.000000 ml_infrastructure-1.5.1/ml_infrastructure/data_manager.py
--rw-rw-r--   0 maple     (1000) maple     (1000)     4402 2023-04-16 13:23:13.000000 ml_infrastructure-1.5.1/ml_infrastructure/evaluator.py
--rw-rw-r--   0 maple     (1000) maple     (1000)     3532 2022-11-28 03:17:28.000000 ml_infrastructure-1.5.1/ml_infrastructure/example.py
--rw-rw-r--   0 maple     (1000) maple     (1000)     3924 2023-04-16 14:21:11.000000 ml_infrastructure-1.5.1/ml_infrastructure/manager.py
--rw-rw-r--   0 maple     (1000) maple     (1000)     3300 2023-04-16 13:27:14.000000 ml_infrastructure-1.5.1/ml_infrastructure/model.py
-drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-04-16 14:46:08.319739 ml_infrastructure-1.5.1/ml_infrastructure/templates/
--rw-rw-r--   0 maple     (1000) maple     (1000)      508 2022-11-28 03:17:28.000000 ml_infrastructure-1.5.1/ml_infrastructure/templates/control.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      316 2023-04-15 15:08:42.000000 ml_infrastructure-1.5.1/ml_infrastructure/templates/eval.html
--rw-rw-r--   0 maple     (1000) maple     (1000)     1530 2023-04-16 14:31:42.000000 ml_infrastructure-1.5.1/ml_infrastructure/templates/header.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      138 2023-04-15 15:08:42.000000 ml_infrastructure-1.5.1/ml_infrastructure/templates/index.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      309 2023-04-15 15:08:42.000000 ml_infrastructure-1.5.1/ml_infrastructure/templates/loss.html
--rw-rw-r--   0 maple     (1000) maple     (1000)     1706 2023-04-16 14:31:42.000000 ml_infrastructure-1.5.1/ml_infrastructure/templates/stopForm.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      181 2022-11-28 03:17:28.000000 ml_infrastructure-1.5.1/ml_infrastructure/templates/trainingEval.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      452 2023-02-25 17:15:04.000000 ml_infrastructure-1.5.1/ml_infrastructure/templates/trainingLoss.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      189 2022-11-28 03:17:28.000000 ml_infrastructure-1.5.1/ml_infrastructure/templates/validationEval.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      446 2023-02-25 16:35:50.000000 ml_infrastructure-1.5.1/ml_infrastructure/templates/validationLoss.html
--rw-rw-r--   0 maple     (1000) maple     (1000)     1899 2022-12-13 04:56:19.000000 ml_infrastructure-1.5.1/ml_infrastructure/trainer.py
-drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-04-16 14:46:08.315739 ml_infrastructure-1.5.1/ml_infrastructure.egg-info/
--rw-rw-r--   0 maple     (1000) maple     (1000)      581 2023-04-16 14:46:08.000000 ml_infrastructure-1.5.1/ml_infrastructure.egg-info/PKG-INFO
--rw-rw-r--   0 maple     (1000) maple     (1000)      905 2023-04-16 14:46:08.000000 ml_infrastructure-1.5.1/ml_infrastructure.egg-info/SOURCES.txt
--rw-rw-r--   0 maple     (1000) maple     (1000)        1 2023-04-16 14:46:08.000000 ml_infrastructure-1.5.1/ml_infrastructure.egg-info/dependency_links.txt
--rw-rw-r--   0 maple     (1000) maple     (1000)       46 2023-04-16 14:46:08.000000 ml_infrastructure-1.5.1/ml_infrastructure.egg-info/requires.txt
--rw-rw-r--   0 maple     (1000) maple     (1000)       18 2023-04-16 14:46:08.000000 ml_infrastructure-1.5.1/ml_infrastructure.egg-info/top_level.txt
--rw-rw-r--   0 maple     (1000) maple     (1000)      107 2023-04-16 14:46:08.319739 ml_infrastructure-1.5.1/setup.cfg
--rw-rw-r--   0 maple     (1000) maple     (1000)      987 2023-04-16 14:45:48.000000 ml_infrastructure-1.5.1/setup.py
+drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-05-01 11:22:15.194608 ml_infrastructure-1.6.1/
+-rw-rw-r--   0 maple     (1000) maple     (1000)     1067 2023-04-16 13:21:50.000000 ml_infrastructure-1.6.1/LICENSE.rst
+-rw-rw-r--   0 maple     (1000) maple     (1000)      581 2023-05-01 11:22:15.194608 ml_infrastructure-1.6.1/PKG-INFO
+-rw-rw-r--   0 maple     (1000) maple     (1000)        0 2023-02-25 18:05:38.000000 ml_infrastructure-1.6.1/README.rst
+drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-05-01 11:22:15.190608 ml_infrastructure-1.6.1/ml_infrastructure/
+-rw-rw-r--   0 maple     (1000) maple     (1000)      168 2023-02-25 17:41:53.000000 ml_infrastructure-1.6.1/ml_infrastructure/__init__.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)     9270 2023-04-30 18:29:39.000000 ml_infrastructure-1.6.1/ml_infrastructure/app.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)      180 2022-11-28 03:17:28.000000 ml_infrastructure-1.6.1/ml_infrastructure/data_manager.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)     4799 2023-04-30 18:25:01.000000 ml_infrastructure-1.6.1/ml_infrastructure/evaluator.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)     3532 2022-11-28 03:17:28.000000 ml_infrastructure-1.6.1/ml_infrastructure/example.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)     3924 2023-04-16 14:21:11.000000 ml_infrastructure-1.6.1/ml_infrastructure/manager.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)     3301 2023-04-30 18:13:06.000000 ml_infrastructure-1.6.1/ml_infrastructure/model.py
+drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-05-01 11:22:15.194608 ml_infrastructure-1.6.1/ml_infrastructure/templates/
+-rw-rw-r--   0 maple     (1000) maple     (1000)      508 2022-11-28 03:17:28.000000 ml_infrastructure-1.6.1/ml_infrastructure/templates/control.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      316 2023-04-15 15:08:42.000000 ml_infrastructure-1.6.1/ml_infrastructure/templates/eval.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)     1530 2023-04-16 14:31:42.000000 ml_infrastructure-1.6.1/ml_infrastructure/templates/header.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      138 2023-04-15 15:08:42.000000 ml_infrastructure-1.6.1/ml_infrastructure/templates/index.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      309 2023-04-15 15:08:42.000000 ml_infrastructure-1.6.1/ml_infrastructure/templates/loss.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)     1706 2023-04-16 14:31:42.000000 ml_infrastructure-1.6.1/ml_infrastructure/templates/stopForm.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      181 2022-11-28 03:17:28.000000 ml_infrastructure-1.6.1/ml_infrastructure/templates/trainingEval.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      452 2023-02-25 17:15:04.000000 ml_infrastructure-1.6.1/ml_infrastructure/templates/trainingLoss.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      189 2022-11-28 03:17:28.000000 ml_infrastructure-1.6.1/ml_infrastructure/templates/validationEval.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      446 2023-02-25 16:35:50.000000 ml_infrastructure-1.6.1/ml_infrastructure/templates/validationLoss.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)     2123 2023-04-30 18:36:27.000000 ml_infrastructure-1.6.1/ml_infrastructure/trainer.py
+drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-05-01 11:22:15.190608 ml_infrastructure-1.6.1/ml_infrastructure.egg-info/
+-rw-rw-r--   0 maple     (1000) maple     (1000)      581 2023-05-01 11:22:15.000000 ml_infrastructure-1.6.1/ml_infrastructure.egg-info/PKG-INFO
+-rw-rw-r--   0 maple     (1000) maple     (1000)      905 2023-05-01 11:22:15.000000 ml_infrastructure-1.6.1/ml_infrastructure.egg-info/SOURCES.txt
+-rw-rw-r--   0 maple     (1000) maple     (1000)        1 2023-05-01 11:22:15.000000 ml_infrastructure-1.6.1/ml_infrastructure.egg-info/dependency_links.txt
+-rw-rw-r--   0 maple     (1000) maple     (1000)       46 2023-05-01 11:22:15.000000 ml_infrastructure-1.6.1/ml_infrastructure.egg-info/requires.txt
+-rw-rw-r--   0 maple     (1000) maple     (1000)       18 2023-05-01 11:22:15.000000 ml_infrastructure-1.6.1/ml_infrastructure.egg-info/top_level.txt
+-rw-rw-r--   0 maple     (1000) maple     (1000)      107 2023-05-01 11:22:15.194608 ml_infrastructure-1.6.1/setup.cfg
+-rw-rw-r--   0 maple     (1000) maple     (1000)      987 2023-05-01 11:19:50.000000 ml_infrastructure-1.6.1/setup.py
```

### Comparing `ml_infrastructure-1.5.1/LICENSE.rst` & `ml_infrastructure-1.6.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.5.1/PKG-INFO` & `ml_infrastructure-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_infrastructure
-Version: 1.5.1
+Version: 1.6.1
 Summary: Software infrastructure to for machine learning
 Author: Ada L
 Author-email: the.nostra.tymus@gmail.com
 License: MIT
 Keywords: machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ml_infrastructure-1.5.1/ml_infrastructure/app.py` & `ml_infrastructure-1.6.1/ml_infrastructure/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
     return json.dumps(loss_graph, cls=plotly.utils.PlotlyJSONEncoder)
 
 
 def get_loss_graph_log(mode):
     global performance
     loss_graph = {
         'data': [Scatter(x=performance[key][mode]['index'],
-                         y=np.log10(performance[key][mode]['values']),
+                         y=[np.log10(i) if i != 0 else np.log10(.1e-100) for i in performance[key][mode]['values']],
                          name=key) for key in performance.keys()],
         'layout': {
             'title': f'<b> {mode.capitalize()} Log Loss </b>',
             'yaxis': {
                 'title': "<b> Log Loss </b>"
             },
             'xaxis': {
```

### Comparing `ml_infrastructure-1.5.1/ml_infrastructure/evaluator.py` & `ml_infrastructure-1.6.1/ml_infrastructure/evaluator.py`

 * *Files 16% similar despite different names*

```diff
@@ -88,26 +88,36 @@
     if mode == 'training':
         loader = data_manager.train_loader
     else:
         loader = data_manager.validation_loader
 
     confusion_matrix = np.zeros((len(classes), len(classes)), dtype=int)
 
-    if len(data_manager.classes) == 2:
+    if len(data_manager.classes) <= 2:
         with torch.no_grad():
             for data in loader:
                 inputs, targets = data[0], data[1]
 
                 outputs = model.classify(inputs)
                 predicted = torch.sigmoid(outputs)
                 predicted = predicted.to("cpu")
                 predicted = [1 if x >= .5 else 0 for x in predicted]
                 for pred, true in zip(predicted, targets):
                     confusion_matrix[int(pred), int(true)] += 1
 
+    else:
+        with torch.no_grad():
+            for data in loader:
+                inputs, targets = data[0], data[1]
+                outputs = model.classify(inputs)
+                predicted = torch.argmax(outputs, 1)
+                predicted = predicted.to("cpu")
+                for pred, true in zip(predicted, targets):
+                    confusion_matrix[int(pred), int(true)] += 1
+
     return confusion_matrix
 
 
 @dataclass
 class Evaluator:
     model: any = None
     data_manager: any = None
```

### Comparing `ml_infrastructure-1.5.1/ml_infrastructure/example.py` & `ml_infrastructure-1.6.1/ml_infrastructure/example.py`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.5.1/ml_infrastructure/manager.py` & `ml_infrastructure-1.6.1/ml_infrastructure/manager.py`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.5.1/ml_infrastructure/model.py` & `ml_infrastructure-1.6.1/ml_infrastructure/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         self.verify_save_dir(os.path.join(save_dir, name))
 
     def step(self, inputs, labels):
         inputs = inputs.to(self.device)
         labels = labels.to(self.device)
         self.optimizer.zero_grad()
         outputs = self.net(inputs)
+
         loss = self.criterion(outputs, labels)
         loss.backward()
         self.optimizer.step()
         return loss.item()
 
     def loss(self, inputs, labels):
         inputs = inputs.to(self.device)
```

### Comparing `ml_infrastructure-1.5.1/ml_infrastructure/templates/header.html` & `ml_infrastructure-1.6.1/ml_infrastructure/templates/header.html`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.5.1/ml_infrastructure/templates/stopForm.html` & `ml_infrastructure-1.6.1/ml_infrastructure/templates/stopForm.html`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.5.1/ml_infrastructure/trainer.py` & `ml_infrastructure-1.6.1/ml_infrastructure/trainer.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 @dataclass
 class Trainer:
     model: any = None
     data_manager: any = None
     ip: str = "0.0.0.0"
     port: int = 5000
     epochs: int = 1
+    print_loss: bool = False
 
     def __post_init__(self):
         self.train_loss = list()
         self.val_loss = list()
 
     def train(self):
         train_loader = self.data_manager.train_loader
@@ -24,23 +25,27 @@
         for epoch in range(self.epochs):
             loss = []
             for batch_idx, data_target in enumerate(train_loader):
                 data = data_target[0]
                 target = data_target[1]
                 loss.append(self.model.step(data, target))
             epoch_loss = np.mean(loss)
+            if self.print_loss:
+                print(f"Mean Epoch Training Loss: {epoch_loss}")
             self.train_loss.append(epoch_loss)
             self.send_watcher('loss', 'training', epoch_loss, len(self.train_loss))
             with torch.no_grad():
                 loss = []
                 for data_target in val_loader:
                     data = data_target[0]
                     target = data_target[1]
                     loss.append(self.model.loss(data, target))
             epoch_loss = np.mean(loss)
+            if self.print_loss:
+                print(f"Mean Epoch Validaion Loss: {epoch_loss}")
             self.val_loss.append(epoch_loss)
             self.send_watcher('loss', 'validation', epoch_loss, len(self.val_loss))
 
         return {
             'train_loss': self.train_loss,
             'validation_loss': self.val_loss,
         }
```

### Comparing `ml_infrastructure-1.5.1/ml_infrastructure.egg-info/PKG-INFO` & `ml_infrastructure-1.6.1/ml_infrastructure.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-infrastructure
-Version: 1.5.1
+Version: 1.6.1
 Summary: Software infrastructure to for machine learning
 Author: Ada L
 Author-email: the.nostra.tymus@gmail.com
 License: MIT
 Keywords: machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ml_infrastructure-1.5.1/ml_infrastructure.egg-info/SOURCES.txt` & `ml_infrastructure-1.6.1/ml_infrastructure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.5.1/setup.py` & `ml_infrastructure-1.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = '1.5.1'
+VERSION = '1.6.1'
 DESCRIPTION = 'Software infrastructure to for machine learning'
 LONG_DESCRIPTION = 'Software infrastructure for machine learning projects that makes it easier to manage experiments and log progress'
 
 setup(
     name="ml_infrastructure",
     version=VERSION,
     description=DESCRIPTION,
```

