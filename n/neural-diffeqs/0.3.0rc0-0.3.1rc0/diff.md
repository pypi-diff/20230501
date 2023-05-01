# Comparing `tmp/neural-diffeqs-0.3.0rc0.tar.gz` & `tmp/neural-diffeqs-0.3.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural-diffeqs-0.3.0rc0.tar", last modified: Thu Apr 13 21:24:41 2023, max compression
+gzip compressed data, was "neural-diffeqs-0.3.1rc0.tar", last modified: Mon May  1 16:08:31 2023, max compression
```

## Comparing `neural-diffeqs-0.3.0rc0.tar` & `neural-diffeqs-0.3.1rc0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:24:41.748619 neural-diffeqs-0.3.0rc0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-13 21:24:41.748619 neural-diffeqs-0.3.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:24:41.744619 neural-diffeqs-0.3.0rc0/neural_diffeqs/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/_latent_potential_ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/_latent_potential_sde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/_neural_ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/_neural_sde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/_potential_ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/_potential_sde.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:24:41.748619 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_latent_ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_latent_sde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_neural_diffeq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_neural_ode.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_neural_sde.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_diffeq_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_potential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:24:41.744619 neural-diffeqs-0.3.0rc0/neural_diffeqs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-13 21:24:41.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-13 21:24:41.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:24:41.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-13 21:24:41.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 21:24:41.000000 neural-diffeqs-0.3.0rc0/neural_diffeqs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 21:24:41.748619 neural-diffeqs-0.3.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-13 21:24:32.000000 neural-diffeqs-0.3.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:08:31.623602 neural-diffeqs-0.3.1rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-01 16:08:20.000000 neural-diffeqs-0.3.1rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-01 16:08:31.623602 neural-diffeqs-0.3.1rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-01 16:08:20.000000 neural-diffeqs-0.3.1rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:08:31.619602 neural-diffeqs-0.3.1rc0/neural_diffeqs/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-01 16:08:20.000000 neural-diffeqs-0.3.1rc0/neural_diffeqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-01 16:08:20.000000 neural-diffeqs-0.3.1rc0/neural_diffeqs/_latent_potential_ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-01 16:08:20.000000 neural-diffeqs-0.3.1rc0/neural_diffeqs/_latent_potential_sde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-01 16:08:20.000000 neural-diffeqs-0.3.1rc0/neural_diffeqs/_neural_ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-01 16:08:20.000000 neural-diffeqs-0.3.1rc0/neural_diffeqs/_neural_sde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-01 16:08:20.000000 neural-diffeqs-0.3.1rc0/neural_diffeqs/_potential_ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-01 16:08:20.000000 neural-diffeqs-0.3.1rc0/neural_diffeqs/_potential_sde.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:08:31.623602 neural-diffeqs-0.3.1rc0/neural_diffeqs/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-01 16:08:20.000000 neural-diffeqs-0.3.1rc0/neural_diffeqs/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-01 16:08:20.000000 neural-diffeqs-0.3.1rc0/neural_diffeqs/core/_base_latent_ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-01 16:08:20.000000 neural-diffeqs-0.3.1rc0/neural_diffeqs/core/_base_latent_sde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-01 16:08:20.000000 neural-diffeqs-0.3.1rc0/neural_diffeqs/core/_base_neural_diffeq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-01 16:08:20.000000 neural-diffeqs-0.3.1rc0/neural_diffeqs/core/_base_neural_ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-01 16:08:20.000000 neural-diffeqs-0.3.1rc0/neural_diffeqs/core/_base_neural_sde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-01 16:08:20.000000 neural-diffeqs-0.3.1rc0/neural_diffeqs/core/_diffeq_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-01 16:08:20.000000 neural-diffeqs-0.3.1rc0/neural_diffeqs/core/_potential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:08:31.619602 neural-diffeqs-0.3.1rc0/neural_diffeqs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-01 16:08:31.000000 neural-diffeqs-0.3.1rc0/neural_diffeqs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-01 16:08:31.000000 neural-diffeqs-0.3.1rc0/neural_diffeqs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:08:31.000000 neural-diffeqs-0.3.1rc0/neural_diffeqs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-01 16:08:31.000000 neural-diffeqs-0.3.1rc0/neural_diffeqs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-01 16:08:31.000000 neural-diffeqs-0.3.1rc0/neural_diffeqs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 16:08:31.623602 neural-diffeqs-0.3.1rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-01 16:08:20.000000 neural-diffeqs-0.3.1rc0/setup.py
```

### Comparing `neural-diffeqs-0.3.0rc0/LICENSE` & `neural-diffeqs-0.3.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.3.0rc0/neural_diffeqs/__init__.py` & `neural-diffeqs-0.3.1rc0/neural_diffeqs/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 __module_name__ = "__init__.py"
 __doc__ = """__init__.py module"""
 __author__ = ", ".join(["Michael E. Vinyard"])
 __email__ = ", ".join(["vinyard@g.harvard.edu"])
-__version__ = "0.3.0rc"
+__version__ = "0.3.0"
 
 
 # -- import subpackages: -------------------------------------------------------
 from . import core
 
 
 # -- import modules: -----------------------------------------------------------
```

### Comparing `neural-diffeqs-0.3.0rc0/neural_diffeqs/_latent_potential_ode.py` & `neural-diffeqs-0.3.1rc0/neural_diffeqs/_latent_potential_ode.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 
 # -- Main operational class: ---------------------------------------------------
 class LatentPotentialODE(core.BaseLatentODE):
     DIFFEQ_TYPE = "ODE"
 
     def __init__(
         self,
-        state_size,
+        state_size: int,
+        coef_diff: float = 0,
+        dt: float = 0.1,
         mu_hidden: Union[List[int], int] = [2000, 2000],
         mu_activation: Union[str, List[str]] = "LeakyReLU",
         mu_dropout: Union[float, List[float]] = 0.2,
         mu_bias: bool = True,
         mu_output_bias: bool = True,
         mu_n_augment: int = 0,
         sde_type="ito",
```

### Comparing `neural-diffeqs-0.3.0rc0/neural_diffeqs/_latent_potential_sde.py` & `neural-diffeqs-0.3.1rc0/neural_diffeqs/_latent_potential_sde.py`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.3.0rc0/neural_diffeqs/_neural_ode.py` & `neural-diffeqs-0.3.1rc0/neural_diffeqs/_neural_ode.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 
 
 # -- Main operational class: ---------------------------------------------------
 class NeuralODE(BaseODE):
     DIFFEQ_TYPE = "ODE"
     def __init__(
         self,
-        state_size,
+        state_size: int,
+        dt: float = 0.1,
+        coef_diff: float = 0,
         mu_hidden: Union[List[int], int] = [2000, 2000],
         mu_activation: Union[str, List[str]] = "LeakyReLU",
         mu_dropout: Union[float, List[float]] = 0.2,
         mu_bias: bool = True,
         mu_output_bias: bool = True,
         mu_n_augment: int = 0,
         sde_type="ito",
```

### Comparing `neural-diffeqs-0.3.0rc0/neural_diffeqs/_neural_sde.py` & `neural-diffeqs-0.3.1rc0/neural_diffeqs/_neural_sde.py`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.3.0rc0/neural_diffeqs/_potential_ode.py` & `neural-diffeqs-0.3.1rc0/neural_diffeqs/_potential_ode.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     sde_type = "ito"
     noise_type = "general"
     brownian_dim = 1
         
     def __init__(
         self,
         state_size,
+        dt: float = 0.1,
+        coef_diff: float = 0,
         mu_hidden: Union[List[int], int] = [2000, 2000],
         mu_activation: Union[str, List[str]] = "LeakyReLU",
         mu_dropout: Union[float, List[float]] = 0.2,
         mu_bias: bool = True,
         mu_output_bias: bool = True,
         mu_n_augment: int = 0,
     ):
@@ -43,10 +45,7 @@
         """use-case: output is directly psi (from a potential network)"""
         return torch.autograd.grad(ψ, y, torch.ones_like(ψ), create_graph=True)[0]
 
     def drift(self, y) -> torch.Tensor:
         y = y.requires_grad_()
         ψ = self._potential(y)
         return self._gradient(ψ, y)
-
-    def diffusion(self, y) -> torch.Tensor:
-        return self.sigma(y).view(y.shape[0], y.shape[1], self.brownian_dim)
```

### Comparing `neural-diffeqs-0.3.0rc0/neural_diffeqs/_potential_sde.py` & `neural-diffeqs-0.3.1rc0/neural_diffeqs/_potential_sde.py`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_latent_ode.py` & `neural-diffeqs-0.3.1rc0/neural_diffeqs/core/_base_latent_sde.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,47 +4,50 @@
 from abc import abstractmethod
 
 
 from ._base_neural_diffeq import BaseDiffEq
 from ._diffeq_config import DiffEqConfig
 
 
-class BaseLatentODE(BaseDiffEq):
-    DIFFEQ_TYPE = "ODE"
+class BaseLatentSDE(BaseDiffEq):
+    DIFFEQ_TYPE = "SDE"
 
     def __init__(self, *args, **kwargs):
         super().__init__()
 
         """
         Must call self.__config__(locals()) in the __init__ of theinheriting
         class.
         
+        
         """
 
     def __config__(self, kwargs):
         """Sets up mu and sigma given params"""
 
         self.__parse__(kwargs=kwargs)
 
         self._config_kwargs = ABCParse.function_kwargs(func=DiffEqConfig, kwargs=kwargs)
         configs = DiffEqConfig(**self._config_kwargs)
+
         self.mu = configs.mu
+        self.sigma = configs.sigma
 
     # -- required methods in child classes: ------------------------------------
     @abstractmethod
     def drift(self):
         """Called by self.f"""
         ...
-    
-    def diffusion(self, y):
-        # keep for compatibility with torchsde.sdeint
+
+    @abstractmethod
+    def diffusion(self):
         """Called by self.g"""
-        return torch.zeros([y.shape[0], y.shape[1], self.brownian_dim])
-    
+        ...
+        
     @abstractmethod
     def prior_drift(self):
         """Called by self.h"""
         ...
-
+        
     def h(self, t: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         """Should return the output of self.diffusion"""
         return self.prior_drift(y)
```

### Comparing `neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_latent_sde.py` & `neural-diffeqs-0.3.1rc0/neural_diffeqs/core/_base_latent_ode.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,51 @@
 
 import torch
 import ABCParse
 from abc import abstractmethod
 
 
-from ._base_neural_diffeq import BaseDiffEq
+# from ._base_neural_diffeq import BaseDiffEq
+from ._base_neural_ode import BaseODE
 from ._diffeq_config import DiffEqConfig
 
 
-class BaseLatentSDE(BaseDiffEq):
-    DIFFEQ_TYPE = "SDE"
+class BaseLatentODE(BaseODE):
+    DIFFEQ_TYPE = "ODE"
 
     def __init__(self, *args, **kwargs):
         super().__init__()
 
         """
         Must call self.__config__(locals()) in the __init__ of theinheriting
         class.
         
-        
         """
 
-    def __config__(self, kwargs):
-        """Sets up mu and sigma given params"""
-
-        self.__parse__(kwargs=kwargs)
+#     def __config__(self, kwargs):
+#         """Sets up mu and sigma given params"""
 
-        self._config_kwargs = ABCParse.function_kwargs(func=DiffEqConfig, kwargs=kwargs)
-        configs = DiffEqConfig(**self._config_kwargs)
+#         self.__parse__(kwargs=kwargs)
 
-        self.mu = configs.mu
-        self.sigma = configs.sigma
+#         self._config_kwargs = ABCParse.function_kwargs(func=DiffEqConfig, kwargs=kwargs)
+#         configs = DiffEqConfig(**self._config_kwargs)
+#         self.mu = configs.mu
 
     # -- required methods in child classes: ------------------------------------
     @abstractmethod
     def drift(self):
         """Called by self.f"""
         ...
-
-    @abstractmethod
-    def diffusion(self):
-        """Called by self.g"""
-        ...
-        
+    
+#     def diffusion(self, y):
+#         # keep for compatibility with torchsde.sdeint
+#         """Called by self.g"""
+#         return torch.zeros([y.shape[0], y.shape[1], self.brownian_dim])
+    
     @abstractmethod
     def prior_drift(self):
         """Called by self.h"""
         ...
-        
+
     def h(self, t: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         """Should return the output of self.diffusion"""
         return self.prior_drift(y)
```

### Comparing `neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_neural_diffeq.py` & `neural-diffeqs-0.3.1rc0/neural_diffeqs/core/_base_neural_diffeq.py`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_base_neural_ode.py` & `neural-diffeqs-0.3.1rc0/neural_diffeqs/core/_base_neural_sde.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 
-import torch
 import ABCParse
 from abc import abstractmethod
 
+
 from ._base_neural_diffeq import BaseDiffEq
 from ._diffeq_config import DiffEqConfig
 
-class BaseODE(BaseDiffEq):
-    DIFFEQ_TYPE = "ODE"
+
+class BaseSDE(BaseDiffEq):
+    DIFFEQ_TYPE = "SDE"
 
     def __init__(self, *args, **kwargs):
         super().__init__()
 
         """
         Must call self.__config__(locals()) in the __init__ of theinheriting
         class.
@@ -22,24 +23,21 @@
     def __config__(self, kwargs):
         """Sets up mu and sigma given params"""
 
         self.__parse__(kwargs=kwargs)
 
         self._config_kwargs = ABCParse.function_kwargs(func=DiffEqConfig, kwargs=kwargs)
         configs = DiffEqConfig(**self._config_kwargs)
+
         self.mu = configs.mu
+        self.sigma = configs.sigma
 
     # -- required methods in child classes: ------------------------------------
     @abstractmethod
     def drift(self):
-        """Called by self.f and/or self.forward"""
+        """Called by self.f"""
         ...
-        
-    def forward(self, t: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
-        return self.drift(y)
 
-    def diffusion(self, y):
-        # keep for compatibility with torchsde.sdeint
+    @abstractmethod
+    def diffusion(self):
         """Called by self.g"""
-        return torch.zeros([y.shape[0], y.shape[1], self.brownian_dim])
-        
-    
+        ...
```

### Comparing `neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_diffeq_config.py` & `neural-diffeqs-0.3.1rc0/neural_diffeqs/core/_diffeq_config.py`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.3.0rc0/neural_diffeqs/core/_potential.py` & `neural-diffeqs-0.3.1rc0/neural_diffeqs/core/_potential.py`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.3.0rc0/neural_diffeqs.egg-info/SOURCES.txt` & `neural-diffeqs-0.3.1rc0/neural_diffeqs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neural-diffeqs-0.3.0rc0/setup.py` & `neural-diffeqs-0.3.1rc0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import re
 import os
 import sys
 
 
 setuptools.setup(
     name="neural-diffeqs",
-    version="0.3.0rc0",
-    python_requires=">3.7.0",
+    version="0.3.1rc0",
+    python_requires=">3.9.0",
     author="Michael E. Vinyard",
     author_email="mvinyard@broadinstitute.org",
     url=None,
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="Neural differential equations made easy.",
     packages=setuptools.find_packages(),
@@ -20,13 +20,13 @@
         "numpy==1.22.4",
         "torch>=2.0.0",
         "torch-nets>=0.0.4",
         "torchsde>=0.2.5",
     ],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.9",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
     license="MIT",
 )
```

