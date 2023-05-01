# Comparing `tmp/kiwigrad-0.24.tar.gz` & `tmp/kiwigrad-0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwigrad-0.24.tar", last modified: Sat Apr 29 14:38:56 2023, max compression
+gzip compressed data, was "kiwigrad-0.25.tar", last modified: Mon May  1 12:20:28 2023, max compression
```

## Comparing `kiwigrad-0.24.tar` & `kiwigrad-0.25.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-29 14:38:56.063179 kiwigrad-0.24/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.24/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       22 2023-04-08 12:11:45.000000 kiwigrad-0.24/MANIFEST.in
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2148 2023-04-29 14:38:56.062742 kiwigrad-0.24/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1672 2023-04-28 23:23:14.000000 kiwigrad-0.24/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-29 14:38:56.060564 kiwigrad-0.24/kiwigrad/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      253 2023-04-29 00:16:46.000000 kiwigrad-0.24/kiwigrad/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     9999 2023-04-29 14:37:23.000000 kiwigrad-0.24/kiwigrad/engine.c
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4222 2023-04-09 13:04:30.000000 kiwigrad-0.24/kiwigrad/engine.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1235 2023-04-27 13:43:11.000000 kiwigrad-0.24/kiwigrad/layers.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3246 2023-04-27 13:42:56.000000 kiwigrad-0.24/kiwigrad/neurons.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1566 2023-04-27 13:42:45.000000 kiwigrad-0.24/kiwigrad/nn.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      144 2023-04-19 20:29:26.000000 kiwigrad-0.24/kiwigrad/skeleton.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-29 14:38:56.061845 kiwigrad-0.24/kiwigrad.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2148 2023-04-29 14:38:55.000000 kiwigrad-0.24/kiwigrad.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      312 2023-04-29 14:38:55.000000 kiwigrad-0.24/kiwigrad.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-29 14:38:55.000000 kiwigrad-0.24/kiwigrad.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-29 14:38:55.000000 kiwigrad-0.24/kiwigrad.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-29 14:38:56.063274 kiwigrad-0.24/setup.cfg
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      942 2023-04-29 00:16:42.000000 kiwigrad-0.24/setup.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-29 14:38:56.062155 kiwigrad-0.24/test/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      618 2023-04-27 14:12:42.000000 kiwigrad-0.24/test/test.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-01 12:20:28.547208 kiwigrad-0.25/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.25/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2128 2023-05-01 12:20:28.546861 kiwigrad-0.25/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1652 2023-04-29 16:01:59.000000 kiwigrad-0.25/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-01 12:20:28.542939 kiwigrad-0.25/kiwigrad/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      253 2023-05-01 11:23:27.000000 kiwigrad-0.25/kiwigrad/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    10349 2023-05-01 12:19:55.000000 kiwigrad-0.25/kiwigrad/engine.c
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4222 2023-04-09 13:04:30.000000 kiwigrad-0.25/kiwigrad/engine.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1235 2023-04-27 13:43:11.000000 kiwigrad-0.25/kiwigrad/layers.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3246 2023-04-27 13:42:56.000000 kiwigrad-0.25/kiwigrad/neurons.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1566 2023-04-27 13:42:45.000000 kiwigrad-0.25/kiwigrad/nn.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      144 2023-04-19 20:29:26.000000 kiwigrad-0.25/kiwigrad/skeleton.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-01 12:20:28.545355 kiwigrad-0.25/kiwigrad.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2128 2023-05-01 12:20:28.000000 kiwigrad-0.25/kiwigrad.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      306 2023-05-01 12:20:28.000000 kiwigrad-0.25/kiwigrad.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-05-01 12:20:28.000000 kiwigrad-0.25/kiwigrad.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-05-01 12:20:28.000000 kiwigrad-0.25/kiwigrad.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-05-01 12:20:28.547317 kiwigrad-0.25/setup.cfg
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      942 2023-05-01 11:23:23.000000 kiwigrad-0.25/setup.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-05-01 12:20:28.545828 kiwigrad-0.25/test/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1075 2023-05-01 10:14:41.000000 kiwigrad-0.25/test/test_value.py
```

### Comparing `kiwigrad-0.24/LICENSE` & `kiwigrad-0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.24/PKG-INFO` & `kiwigrad-0.25/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwigrad
-Version: 0.24
+Version: 0.25
 Summary: Mini deep learning framework
 Home-page: https://github.com/marcosalvalaggio/kiwigrad
 Author: Marco Salvalaggio
 Author-email: mar.salvalaggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -65,9 +65,8 @@
 
 model = PotNet()
 ```
 
 ## TODOS
 
 * Include the activation functions tanh in the Value object.
-* Fix pow function.
```

### Comparing `kiwigrad-0.24/README.md` & `kiwigrad-0.25/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -48,9 +48,8 @@
         super().__init__(layers=layers)
 
 model = PotNet()
 ```
 
 ## TODOS
 
-* Include the activation functions tanh in the Value object.
-* Fix pow function.
+* Include the activation functions tanh in the Value object.
```

### Comparing `kiwigrad-0.24/kiwigrad/engine.c` & `kiwigrad-0.25/kiwigrad/engine.c`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 typedef struct {
   PyObject_HEAD
   double data;
   double grad;
   double oa;
   PyObject *prev;
+  PyObject *op;
   int func_idx;
   PyObject *tmp;
   List *topology;
   int visited;
 } Value;
 
 typedef struct _Node {
@@ -40,14 +41,15 @@
   Value *value = (Value *)Value_Type.tp_alloc(&Value_Type, 0);
   if (value) {
     value->grad = 0.0;
     value->visited = 0;
     value->data = data;
     value->oa = 0.0;
     value->prev = PyTuple_New(0);
+    value->op = Py_None;
     value->topology = NULL;
     value->tmp = Py_None;
     value->func_idx = -1;
   }
   return (PyObject *)value;
 }
 
@@ -179,36 +181,39 @@
   if (((Value *)self)->data < 0.0) {
     value->data = 0.0;
   } else {
     value->data = ((Value *)self)->data;
   }
   value->grad = 0.0;
   value->prev = PyTuple_Pack(1, self);
+  value->op = PyUnicode_FromString("relu");
   value->func_idx = 3;
   return (PyObject *)value;
 }
 
 static PyObject * Value_sigmoid(PyObject *self) {
   Value *value = (Value *)Value_Type.tp_alloc(&Value_Type, 0);
   double x = ((Value *)self)->data;
   double t = 1 / (1 + exp(-x));
   value->data = t;
   value->grad = 0.0;
   value->prev = PyTuple_Pack(1, self);
+  value->op = PyUnicode_FromString("sigmoid");
   value->func_idx = 4;
   return (PyObject *)value;
 }
 
 static PyObject * Value_log(PyObject *self) {
   Value *value = (Value *)Value_Type.tp_alloc(&Value_Type, 0);
   double x = ((Value *)self)->data;
   double t = log(x);
   value->data = t;
   value->grad = 0.0;
   value->prev = PyTuple_Pack(1, self);
+  value->op = PyUnicode_FromString("log");
   value->func_idx = 5;
   return (PyObject *)value;
 }
 
 
 static void list_append(List *list, PyObject *value) {
   Node *node = malloc(sizeof(Node));
@@ -272,42 +277,46 @@
     {"backward", (PyCFunction)backward, METH_NOARGS, "Backward"},
     {NULL}  /* Sentinel */
 };
 
 static PyMemberDef Value_members[] = {
    {"data", T_DOUBLE, offsetof(Value, data), 0, "Data"},
    {"grad", T_DOUBLE, offsetof(Value, grad), 0, "Gradient of the Object"},
-   // {"prev", T_OBJECT_EX, offsetof(Value, prev), 0, "Children"}, // DEBUG
+   {"_prev", T_OBJECT, offsetof(Value, prev), 0, "Children"}, // DEBUG
+   {"_op", T_OBJECT, offsetof(Value, op), 0, "Label"},
    {NULL}
   };
 
 PyObject * pyvalue_add(PyObject *self, PyObject *other) {
   Value *value = (Value *)Value_Type.tp_alloc(&Value_Type, 0);
   value->data = ((Value *)self)->data + ((Value *)other)->data;
   value->grad = 0.0;
   value->prev = PyTuple_Pack(2, self, other);
+  value->op = PyUnicode_FromString("+");
   value->func_idx = 0;
   return (PyObject *)value;
 }
 
 PyObject * pyvalue_mul(PyObject *self, PyObject *other) {
   Value *value = (Value *)Value_Type.tp_alloc(&Value_Type, 0);
   value->data = ((Value *)self)->data * ((Value *)other)->data;
   value->grad = 0.0;
   value->prev = PyTuple_Pack(2, self, other);
+  value->op = PyUnicode_FromString("*");
   value->func_idx = 1;
   return (PyObject *)value;
 }
 
 PyObject * pyvalue_pow(PyObject *self, PyObject *other, PyObject *arg) {
   Value *value = (Value *)Value_Type.tp_alloc(&Value_Type, 0);
   value->data = pow(((Value *)self)->data, PyFloat_AsDouble(other));
   value->grad = 0.0;
   value->prev = PyTuple_Pack(1, self);
   value->oa = PyFloat_AsDouble(other);
+  value->op = PyUnicode_FromString("pow");
   //value->tmp = other;
   value->func_idx = 2;
   return (PyObject *)value;
 }
 
 PyObject * pyvalue_negative(PyObject *self) {
   PyObject *other = (PyObject *)Value_Type.tp_alloc(&Value_Type, 0);
```

### Comparing `kiwigrad-0.24/kiwigrad/engine.py` & `kiwigrad-0.25/kiwigrad/engine.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.24/kiwigrad/layers.py` & `kiwigrad-0.25/kiwigrad/layers.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.24/kiwigrad/neurons.py` & `kiwigrad-0.25/kiwigrad/neurons.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.24/kiwigrad/nn.py` & `kiwigrad-0.25/kiwigrad/nn.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.24/kiwigrad.egg-info/PKG-INFO` & `kiwigrad-0.25/kiwigrad.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwigrad
-Version: 0.24
+Version: 0.25
 Summary: Mini deep learning framework
 Home-page: https://github.com/marcosalvalaggio/kiwigrad
 Author: Marco Salvalaggio
 Author-email: mar.salvalaggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -65,9 +65,8 @@
 
 model = PotNet()
 ```
 
 ## TODOS
 
 * Include the activation functions tanh in the Value object.
-* Fix pow function.
```

### Comparing `kiwigrad-0.24/setup.py` & `kiwigrad-0.25/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools.extension import Extension
 
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='kiwigrad',
-      version='0.24',
+      version='0.25',
       description='Mini deep learning framework',
       author='Marco Salvalaggio',
       author_email='mar.salvalaggio@gmail.com',
       license='MIT',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/marcosalvalaggio/kiwigrad',
```

