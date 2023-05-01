# Comparing `tmp/synapgrad-0.2.9-py3-none-any.whl.zip` & `tmp/synapgrad-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 28868 bytes, number of entries: 21
+Zip file size: 29510 bytes, number of entries: 21
 -rw-rw-rw-  2.0 fat       72 b- defN 23-Apr-08 18:28 synapgrad/__init__.py
--rw-rw-rw-  2.0 fat    30875 b- defN 23-Apr-21 09:11 synapgrad/engine.py
--rw-rw-rw-  2.0 fat      420 b- defN 23-Apr-21 10:37 synapgrad/nn/__init__.py
+-rw-rw-rw-  2.0 fat    30938 b- defN 23-May-01 14:04 synapgrad/engine.py
+-rw-rw-rw-  2.0 fat      442 b- defN 23-May-01 13:33 synapgrad/nn/__init__.py
 -rw-rw-rw-  2.0 fat     3538 b- defN 23-Apr-20 01:42 synapgrad/nn/activations.py
 -rw-rw-rw-  2.0 fat     7831 b- defN 23-Apr-19 17:14 synapgrad/nn/functional.py
 -rw-rw-rw-  2.0 fat     2879 b- defN 23-Apr-20 12:52 synapgrad/nn/initializations.py
--rw-rw-rw-  2.0 fat    13895 b- defN 23-Apr-21 10:27 synapgrad/nn/layers.py
+-rw-rw-rw-  2.0 fat    17780 b- defN 23-May-01 13:30 synapgrad/nn/layers.py
 -rw-rw-rw-  2.0 fat     6809 b- defN 23-Apr-20 01:41 synapgrad/nn/losses.py
 -rw-rw-rw-  2.0 fat     2654 b- defN 23-Apr-19 20:19 synapgrad/nn/modules.py
--rw-rw-rw-  2.0 fat      997 b- defN 23-Apr-20 12:59 synapgrad/nn/neurons.py
+-rw-rw-rw-  2.0 fat      989 b- defN 23-May-01 11:50 synapgrad/nn/neurons.py
 -rw-rw-rw-  2.0 fat       46 b- defN 23-Apr-08 14:30 synapgrad/optim/__init__.py
 -rw-rw-rw-  2.0 fat     5293 b- defN 23-Apr-20 01:43 synapgrad/optim/optimizers.py
 -rw-rw-rw-  2.0 fat      154 b- defN 23-Apr-11 17:18 synapgrad/utils/__init__.py
 -rw-rw-rw-  2.0 fat     3403 b- defN 23-Apr-11 18:19 synapgrad/utils/data.py
 -rw-rw-rw-  2.0 fat     1345 b- defN 23-Apr-21 08:50 synapgrad/utils/graph.py
 -rw-rw-rw-  2.0 fat    10586 b- defN 23-Apr-12 12:20 synapgrad/utils/train.py
--rw-rw-rw-  2.0 fat     1088 b- defN 23-Apr-21 11:09 synapgrad-0.2.9.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4488 b- defN 23-Apr-21 11:09 synapgrad-0.2.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-21 11:09 synapgrad-0.2.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-21 11:09 synapgrad-0.2.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1696 b- defN 23-Apr-21 11:09 synapgrad-0.2.9.dist-info/RECORD
-21 files, 98171 bytes uncompressed, 26128 bytes compressed:  73.4%
+-rw-rw-rw-  2.0 fat     1088 b- defN 23-May-01 14:44 synapgrad-0.3.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4664 b- defN 23-May-01 14:44 synapgrad-0.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-01 14:44 synapgrad-0.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-May-01 14:44 synapgrad-0.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1696 b- defN 23-May-01 14:44 synapgrad-0.3.0.dist-info/RECORD
+21 files, 102309 bytes uncompressed, 26770 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: synapgrad/utils/graph.py
 Comment: 
 
 Filename: synapgrad/utils/train.py
 Comment: 
 
-Filename: synapgrad-0.2.9.dist-info/LICENSE
+Filename: synapgrad-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: synapgrad-0.2.9.dist-info/METADATA
+Filename: synapgrad-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: synapgrad-0.2.9.dist-info/WHEEL
+Filename: synapgrad-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: synapgrad-0.2.9.dist-info/top_level.txt
+Filename: synapgrad-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: synapgrad-0.2.9.dist-info/RECORD
+Filename: synapgrad-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## synapgrad/engine.py

```diff
@@ -696,14 +696,17 @@
         self._retain_grad = True
         
     def numpy(self) -> np.ndarray:
         if self.requires_grad:
             raise RuntimeError("Can't call numpy() on Tensor that requires grad. Use tensor.detach().numpy() instead")
         return self.data
     
+    def numel(self) -> int:
+        return self.data.size
+    
     def item(self) -> float:
         squeezed = self.data.squeeze()
         if len(squeezed.shape) > 0:
             raise ValueError("only one element tensors can be converted to Python scalars")
         
         return squeezed
         
@@ -792,15 +795,15 @@
             self._current_idx += 1
             return val
     
     def __len__(self) -> int:
         return len(self.data)
     
     def __neg__(self) -> 'Tensor': # -self
-        return self * -1
+        return self * -1.0
 
     def __radd__(self, other) -> 'Tensor': # other + self
         return self + other
 
     def __sub__(self, other) -> 'Tensor': # self - other
         return self + (-other)
 
@@ -834,13 +837,13 @@
         if self.requires_grad:
             string += f", req_grad={self.requires_grad}"
             
         if self._operation is not None:
             string += f", op={self._operation}"
             
         if self._name is not None:
-            string += f", name={self._operation}"
+            string += f", name={self._name}"
             
             
         string += f", dtype={self.dtype})"
             
         return string
```

## synapgrad/nn/__init__.py

```diff
@@ -1,8 +1,8 @@
 
 from .modules import Module, Sequential
 from .neurons import Neuron
-from .layers import Linear, Flatten, Unfold, Fold, Conv2d, MaxPool2d, Dropout# , BatchNorm2d
+from .layers import Linear, Flatten, Unfold, Fold, Conv2d, MaxPool2d, Dropout, BatchNorm, BatchNorm1d, BatchNorm2d
 from .losses import Loss, MSELoss, CrossEntropyLoss, NLLLoss, BCELoss, BCEWithLogitsLoss
 from .activations import relu_fn, ReLU, Tanh, tanh_fn, sigmoid_fn, Sigmoid, softmax_fn, Softmax, LogSoftmax
 from . import functional
 from . import initializations
```

## synapgrad/nn/layers.py

```diff
@@ -10,26 +10,26 @@
     def __init__(self, input_size:int, output_size:int, weight_init_method='he_normal'):
         super().__init__()
         self.input_size = input_size
         self.output_size = output_size
         
         self.weight_init_method = weight_init_method
         weight_values = init_weights((output_size, input_size), weight_init_method).astype(np.float32)
-        self.weights = Tensor(weight_values, requires_grad=True)
+        self.weight = Tensor(weight_values, requires_grad=True)
         self.bias = Tensor(np.zeros((output_size,), dtype=np.float32), requires_grad=True)
         
     def forward(self, x:Tensor) -> Tensor:
         assert x.shape[1] == self.input_size, f"Expected input size '{self.input_size}' but received '{x.shape[1]}'"
 
-        out = (x @ self.weights.transpose(0,-1)) + self.bias
+        out = (x @ self.weight.transpose(0,-1)) + self.bias
         
         return out
     
     def parameters(self) -> list[Tensor]:
-        return [self.weights, self.bias]
+        return [self.weight, self.bias]
     
     def __repr__(self) -> str:
         return f"Linear(input_size={self.input_size}, neurons={len(self.output_size)})"
 
 
 class Flatten(nn.Module):
     
@@ -219,128 +219,207 @@
         self.stride = stride
         self.stride = stride
         self.padding = padding
         self.dilation = dilation
         
         self.weight_init_method = weight_init_method
         weight_values = init_weights((out_channels, in_channels, *kernel_size), weight_init_method).astype(np.float32)
-        self.weights = Tensor(weight_values, requires_grad=True)
+        self.weight = Tensor(weight_values, requires_grad=True)
         self.bias = Tensor(np.zeros((out_channels,), dtype=np.float32), requires_grad=True)
     
     def forward(self, x: Tensor) -> Tensor:
         N, C, H, W = x.shape
         lH = int(np.floor((H + 2 * self.padding[0] - self.dilation[0] * (self.kernel_size[0] - 1) - 1) / self.stride[0] + 1))
         lW = int(np.floor((W + 2 * self.padding[1] - self.dilation[1] * (self.kernel_size[1] - 1) - 1) / self.stride[1] + 1))
         
         unfolded = Unfold(kernel_size=self.kernel_size, stride=self.stride, dilation=self.dilation,
                            padding=self.padding, pad_value=0)(x)
         
-        weights = self.weights.view(self.weights.shape[0], -1).transpose(0,1) 
-        mult = unfolded.transpose(1,2) @ weights
+        weight = self.weight.view(self.weight.shape[0], -1).transpose(0,1) 
+        mult = unfolded.transpose(1,2) @ weight
         convolved = (mult) + self.bias
         out = convolved.transpose(1,2).view(N, self.out_channels, lH, lW)
 
         return out
         
     def parameters(self) -> list['Tensor']:
-        return [self.weights, self.bias]
+        return [self.weight, self.bias]
     
     def __repr__(self) -> str:
         return (f"Conv2d(in_channels={self.in_channels}, out_channels={self.out_channels}, " + 
                 f"kernel_size={self.kernel_size}, stride={self.stride}, padding={self.padding}, " + 
                 f"dilation={self.dilation}")
     
-    
-class BatchNorm2d(nn.Module):
-    """
-    TODO: This layer is not working properly yet
+
+class Dropout(nn.Module):
+    """ 
     Reference:
-        https://pytorch.org/docs/stable/generated/torch.nn.BatchNorm2d.html
-    """
+        https://pytorch.org/docs/stable/generated/torch.nn.Dropout.html
     
-    def __init__(self, num_features:int, eps:float=1e-5, momentum:float=0.1, affine:bool=True,
-                 track_running_stats:bool=True) -> None:
-        """
-        Computes the batchnorm2d of a 4-dimensional tensor and its gradient.
+    """
 
-        Arguments:
-        x: tensor of shape (N, C, H, W) representing a batch of images.
-        gamma: tensor of shape (C,) representing the normalization scale.
-        beta: tensor of shape (C,) representing the normalization bias.
-        eps: small constant to avoid division by zero in variance computation.
-        momentum: exponential moving average factor for the mean and variance.
-        track_running_stats: 
-        """
+    def __init__(self, p=0.5, inplace=False) -> None:
+        super().__init__()
+        self.p = p
+        self.inplace = inplace
+        
+    def forward(self, x: Tensor) -> Tensor:
+        if not self.training: return x
+        random_data = np.random.rand(*x.shape)
+        random_data = np.where(random_data <= self.p, 0, 1)
+        if self.p < 1:
+            random_data = random_data / (1-self.p) # scale data
+        random_t = Tensor(random_data)
+        
+        return x*random_t
+    
+    
+class BatchNorm(nn.Module):
+    
+    def __init__(self, mode:str, num_features:int, eps:float=1e-5, momentum:float=0.1, affine:bool=True,
+                 track_running_stats:bool=True, dtype=None) -> None:
         super().__init__()
         self.num_features = num_features
         self.eps = eps
         self.momentum = momentum
         self.affine = affine
         self.track_running_stats = track_running_stats
         
-        self.running_mean = None
-        self.running_var = None
+        valid_modes = ['1d', '2d']
+        
+        if mode not in valid_modes:
+            raise ValueError(f"'{mode}' is not a valid mode, expected one of {valid_modes}")
+        self.mode = mode
+        
+        if dtype is None:
+            dtype = np.float32
+        
+        if self.track_running_stats:
+            self.running_mean = Tensor(np.zeros(num_features, dtype=dtype))
+            self.running_var = Tensor(np.ones(num_features, dtype=dtype))
+        else:
+            self.running_mean = None
+            self.running_var = None
         
         if affine:
-            self.gamma = Tensor(np.ones(num_features), requires_grad=True, dtype=np.float32, name="gamma")
-            self.beta = Tensor(np.zeros(num_features), requires_grad=True, dtype=np.float32, name="beta")
-            
-            
+            # gamma
+            self.weight = Tensor(np.ones(num_features), requires_grad=True, dtype=dtype, name="gamma")
+            # beta
+            self.bias = Tensor(np.zeros(num_features), requires_grad=True, dtype=dtype, name="beta")
+                
     def forward(self, x: Tensor) -> Tensor:
-        N, C, H, W = x.shape
-        num_examples = N*H*W
+        if self.mode == '2d':
+            if len(x.shape) == 4:
+                N, C, H, W = x.shape
+                n = N*H*W # num_samples
+                dims = (0,2,3)
+                view_shape = (1,C,1,1)
+            else: raise RuntimeError(f"Expected 4D tensor, but got {len(x.shape)}D")
+        elif self.mode == '1d':
+            if len(x.shape) == 3:
+                N, C, L = x.shape
+                n = N*L # num_samples
+                dims = (0,2)
+                view_shape = (1,C,1)
+            elif len(x.shape) == 2:
+                N, C = x.shape
+                n = N # num_samples
+                dims = (0,)
+                view_shape = (1,C)
+            else: raise RuntimeError(f"Expected 2D or 3D tensor, but got {len(x.shape)}D")
         assert C == self.num_features, f"Expected {self.num_features} channels, got {C}."
-        # Compute the mean of each channel
-        mu = x.mean(dim=(0,2,3), keepdims=True)
-
-        # Compute the variance of each channel
-        var = ((x - mu)**2).mean(dim=(0,2,3), keepdims=True)
-        std = (var + self.eps).sqrt()
-
-        # Update the running average of mean and variance
-        if self.track_running_stats:
-            if self.running_mean is None:
-                self.running_mean = mu
-            else:
-                self.running_mean = (self.momentum * self.running_mean + (1 - self.momentum) * mu)
+        
+        if self.training or not self.track_running_stats:
+            # Compute the mean of each channel
+            mu = x.mean(dim=dims, keepdims=True)
+            # Compute the variance of each channel
+            var_sum = ((x-mu)**2).sum(dim=dims, keepdims=True)
+            var = var_sum / n
+            std = (var + self.eps).sqrt()
             
-            if self.running_var is None:
-                self.running_var = var
-            else:
-                self.running_var = (self.momentum * self.running_var + (1 - self.momentum) * var)
-
-        # Normalize the input tensor
-        x_norm = (x - mu) / std
+            # Normalize the input tensor
+            x_norm = (x - mu) / std
+            
+            # Update the running average of mean and variance
+            if self.training and self.track_running_stats:
+                r_mu = (self.momentum * mu.data.reshape(-1) + (1 - self.momentum) * self.running_mean.data)
+                self.running_mean = Tensor(r_mu)
+                
+                unbiased_var = var_sum.data.reshape(-1) / (n - 1)
+                r_var = (self.momentum * unbiased_var + (1 - self.momentum) * self.running_var.data)
+                self.running_var = Tensor(r_var.squeeze())
+        else:
+            x_norm = (x - self.running_mean.view(*view_shape)) / (self.running_var.view(*view_shape) + self.eps).sqrt()
 
         # Scale and shift the normalization
         if self.affine:
-            out = self.gamma.view(1,C,1,1) * x_norm + self.beta.view(1,C,1,1)
+            out = self.weight.view(*view_shape) * x_norm + self.bias.view(*view_shape)
         else:
             out = x_norm
         
         return out
 
     def parameters(self) -> list[Tensor]:
-        return [self.gamma, self.beta] if self.affine else []    
-    
+        return [self.weight, self.bias] if self.affine else []
 
-class Dropout(nn.Module):
-    """ 
+
+class BatchNorm1d(BatchNorm):
+    """
     Reference:
-        https://pytorch.org/docs/stable/generated/torch.nn.Dropout.html
+        https://pytorch.org/docs/stable/generated/torch.nn.BatchNorm1d.html
+    """
+    
+    def __init__(self, num_features:int, eps:float=1e-5, momentum:float=0.1, affine:bool=True,
+                 track_running_stats:bool=True, dtype=None) -> None:
+        """
+        Computes the batchnorm of a 2 or 3 dimensional tensor (N, C) or (N, C, L) 
+
+        Arguments:
+        num_features (int): C from an expected input size (N, C) or (N, C, L).
+        eps (float): small constant to avoid division by zero in variance computation.
+        momentum (float): the value used for the running_mean and running_var computation.
+            Can be set to None for cumulative moving average (i.e. simple average).
+            Default: 0.1.
+        affine (bool): a boolean value that when set to True, this module has 
+            learnable affine parameters. Default: True
+        track_running_stats (bool): a boolean value that when set to True, this module 
+            tracks the running mean and variance, and when set to False, this 
+            module does not track such statistics, and initializes statistics buffers
+            running_mean and running_var as None. When these buffers are None, this 
+            module always uses batch statistics. in both training and eval modes. 
+            Default: True
+        """
+        super().__init__('1d', num_features, eps, momentum, affine, track_running_stats, dtype)
+
     
+class BatchNorm2d(BatchNorm):
+    """
+    Reference:
+        https://pytorch.org/docs/stable/generated/torch.nn.BatchNorm2d.html
     """
     
-    def __init__(self, p=0.5, inplace=False) -> None:
-        super().__init__()
-        self.p = p
-        self.inplace = inplace
+    def __init__(self, num_features:int, eps:float=1e-5, momentum:float=0.1, affine:bool=True,
+                 track_running_stats:bool=True, dtype=None) -> None:
+        """
+        Computes the batchnorm of a 4-dimensional tensor (N, C, H, W) 
+
+        Arguments:
+        num_features (int): C from an expected input size (N, C, H, W).
+        eps (float): small constant to avoid division by zero in variance computation.
+        momentum (float): the value used for the running_mean and running_var computation.
+            Can be set to None for cumulative moving average (i.e. simple average).
+            Default: 0.1.
+        affine (bool): a boolean value that when set to True, this module has 
+            learnable affine parameters. Default: True
+        track_running_stats (bool): a boolean value that when set to True, this module 
+            tracks the running mean and variance, and when set to False, this 
+            module does not track such statistics, and initializes statistics buffers
+            running_mean and running_var as None. When these buffers are None, this 
+            module always uses batch statistics. in both training and eval modes. 
+            Default: True
+        """
+        super().__init__('2d', num_features, eps, momentum, affine, track_running_stats, dtype)
         
-    def forward(self, x: Tensor) -> Tensor:
-        if not self.training: return x
-        random_data = np.random.rand(*x.shape)
-        random_data = np.where(random_data <= self.p, 0, 1)
-        if self.p < 1:
-            random_data = random_data / (1-self.p) # scale data
-        random_t = Tensor(random_data)
         
-        return x*random_t
+
+        
+
```

## synapgrad/nn/neurons.py

```diff
@@ -1,29 +1,28 @@
 import numpy as np
 from .. import Tensor, nn
 from .initializations import init_weights
 
 
-
 class Neuron(nn.Module):
     
     def __init__(self, inputs:int, weight_init_method='he_normal') -> None:
         self.inputs = inputs
         
         # Randomly initialize weights and bias
         self.weight_init_method = weight_init_method
         weight_values = init_weights((1, inputs), weight_init_method).astype(np.float32)
-        self.weights = Tensor(weight_values, requires_grad=True)
+        self.weight = Tensor(weight_values, requires_grad=True)
         self.bias = Tensor([0], requires_grad=True)
     
     def forward(self, x:Tensor) -> Tensor:
-        assert x[0].matches_shape(self.weights[0]), f"Expected input size '{self.weights[0].shape}' but received '{x[0].shape}'"
+        assert x[0].matches_shape(self.weight[0]), f"Expected input size '{self.weight[0].shape}' but received '{x[0].shape}'"
 
-        out = (x @ self.weights.transpose(0,-1)) + self.bias
+        out = (x @ self.weight.transpose(0,-1)) + self.bias
     
         return out
 
     def parameters(self):
-        return [self.weights, self.bias]
+        return [self.weight, self.bias]
 
     def __repr__(self) -> str:
-        return f"Neuron(weights={self.weights}, bias={self.bias})"
+        return f"Neuron(weights={self.weight}, bias={self.bias})"
```

## Comparing `synapgrad-0.2.9.dist-info/LICENSE` & `synapgrad-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `synapgrad-0.2.9.dist-info/METADATA` & `synapgrad-0.3.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapgrad
-Version: 0.2.9
+Version: 0.3.0
 Summary: An autograd Tensor-based engine with a deep learning library built on top of it made from scratch
 Home-page: https://github.com/pgmesa/synapgrad
 Author: Pablo García Mesa
 Author-email: pgmesa.sm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
@@ -79,22 +79,23 @@
 Example 1 (synapgrad MLP solution)     |  Example 2 and 3
 :-------------------------:|:-------------------------:
 ![Image 1](/assets/example_moons.png) | ![Image 2](/assets/example_mnist.png) 
 
 ## Comparisons with other frameworks
 In order to see the efficiency of synapgrad, it is compared with other existing engines (in this case torch and micrograd).
 
-
 | Training Example | synapgrad | torch | micrograd |
 |     :---:        |  :---:  |  :---:  |   :---:   |  
 | 1 | 1.7 s | 1.5 s | 1 min 43 s |
-| 2 | 52 s | 31 s | - |
-| 3 |  16 min 7 s  |  1 min 52 s  | - |
+| 2 | 2 min 30 s | 53 s | - |
+| 3 |  25 min 10 s  |  2 min 5 s  | - |
+| 2 (without batchnorm) | 52 s |  31 s | - |
+| 3 (without batchnorm) |  16 min 7 s  |  1 min 52 s  | - |
 
-As it can be seen, pytorch is much better optimized for convolutional operations.
+As can be observed, conv2d and batchnorm are currently much more optimized in Pytorch. I will attempt to optimize these layers in a future version.
 
 ## Graph Visualization
 In the `examples/trace_graph.ipynb` notebook there is an example of how to display the graph that synapgrad creates in the background as operations are chained.
 
 ```python
 import synapgrad
 from synapgrad import nn, utils
```

## Comparing `synapgrad-0.2.9.dist-info/RECORD` & `synapgrad-0.3.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 synapgrad/__init__.py,sha256=rzU1koPmJ4_LyMdxWzho4Qd-qWUqh16aKSgmF5HBOEw,72
-synapgrad/engine.py,sha256=UFwd5mIN1oYTGKGwNlRdd6cbYc4wJYWGXVd19hiMjY0,30875
-synapgrad/nn/__init__.py,sha256=I-NOoUsUEoYP7VlN8IB2BnCGkF3Xruj7X7Dk_BnF4FU,420
+synapgrad/engine.py,sha256=fttCUYh5ZLB5uJ6MzvCp63aPQpW_P7OeZKtrXVL_664,30938
+synapgrad/nn/__init__.py,sha256=kJVBFgfaX-9Rsg0QDV3lKjPaRNuWVn2RgCkb-mAvXhM,442
 synapgrad/nn/activations.py,sha256=TEUzX6IvnYlnWkmCyLQMxTDENH-cukG8R0R26ikV5QA,3538
 synapgrad/nn/functional.py,sha256=jICas3UKdjRsxh4xZBTl4nNMfswrrEmqRoOKzu4Qgjw,7831
 synapgrad/nn/initializations.py,sha256=WjgU7KfSQh_aMXBXrj5KOyaz6C3y-tPbmsodFiu6uRc,2879
-synapgrad/nn/layers.py,sha256=d5NGI0WbJtI1Z6BZH2laoqpuLwsr62FYixz6vWLj5jI,13895
+synapgrad/nn/layers.py,sha256=OOSg5Dcz3O3RHFGztODfv6aXjWOXUcMW9JWL8jCycZU,17780
 synapgrad/nn/losses.py,sha256=N7uLz_ILdv_LQ_MGLH3xCfyC9FPyEWz7zVO51Di0XJY,6809
 synapgrad/nn/modules.py,sha256=y_F6iUE5t0rlXGwvOtsSVttqgJ3OPMkdx5MbDxceVYc,2654
-synapgrad/nn/neurons.py,sha256=_sTmji8gninDkOEqxHL6Q8av7CIu9mK2m9Olz0FG98E,997
+synapgrad/nn/neurons.py,sha256=oQNtsfpAE-CYymK45Wz-ORsuiOzk6CAg5ZcCLYnjl6A,989
 synapgrad/optim/__init__.py,sha256=8X56jD7Dcyw-Hdux1K7_YK9_oc3BuNPk9YwC7gSNWaE,46
 synapgrad/optim/optimizers.py,sha256=Y5ryseve_Virrpsl2ynSt2npq2O0-kyIj_Tj0jfKko0,5293
 synapgrad/utils/__init__.py,sha256=eCwZrBr9yWO92hufOIWwAFhwrA_JuMCsmHeDL7PSAtE,154
 synapgrad/utils/data.py,sha256=cwSsVZwEbB6BU9tWrf5aIeZo9u5KNgar7rVYa6WV328,3403
 synapgrad/utils/graph.py,sha256=FOkPCSYcmOaoPRhdoXweUQRvoxH0n3x4nASGLr7HQjw,1345
 synapgrad/utils/train.py,sha256=V3j4iqSW9sjSfIz9bski95Ni25KuYzIAkjqD4o3-Tjg,10586
-synapgrad-0.2.9.dist-info/LICENSE,sha256=tILw81bLBHb_8uhiXZAlAo5QrlyMSCJH33lb7GYpz6E,1088
-synapgrad-0.2.9.dist-info/METADATA,sha256=XeHTUuOhPvWrceJLtuFqH5yPCqe5pBw_M7WaHyAzuU8,4488
-synapgrad-0.2.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-synapgrad-0.2.9.dist-info/top_level.txt,sha256=D7_rcC0S5ytl1AFRAo5c73mZggZB-Z_zm_GNIGe0QgM,10
-synapgrad-0.2.9.dist-info/RECORD,,
+synapgrad-0.3.0.dist-info/LICENSE,sha256=tILw81bLBHb_8uhiXZAlAo5QrlyMSCJH33lb7GYpz6E,1088
+synapgrad-0.3.0.dist-info/METADATA,sha256=xo0yor_rizRPwrTbqEkbeyd291m40qqxZNIpQOKzoNw,4664
+synapgrad-0.3.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+synapgrad-0.3.0.dist-info/top_level.txt,sha256=D7_rcC0S5ytl1AFRAo5c73mZggZB-Z_zm_GNIGe0QgM,10
+synapgrad-0.3.0.dist-info/RECORD,,
```

