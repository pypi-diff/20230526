# Comparing `tmp/torch_activation-0.0.1.tar.gz` & `tmp/torch_activation-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_activation-0.0.1.tar", max compression
+gzip compressed data, was "torch_activation-0.1.0.tar", max compression
```

## Comparing `torch_activation-0.0.1.tar` & `torch_activation-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,12 @@
--rw-r--r--   0        0        0     3203 2023-05-23 01:48:14.729010 torch_activation-0.0.1/README.md
--rw-r--r--   0        0        0      449 2023-05-23 01:48:14.729010 torch_activation-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      372 2023-05-23 01:48:14.729010 torch_activation-0.0.1/torch_activation/__init__.py
--rw-r--r--   0        0        0     3363 2023-05-23 01:48:14.729010 torch_activation-0.0.1/torch_activation/glu_family.py
--rw-r--r--   0        0        0     6402 2023-05-23 01:48:14.729010 torch_activation-0.0.1/torch_activation/non_linear.py
--rw-r--r--   0        0        0     4571 2023-05-23 01:48:14.729010 torch_activation-0.0.1/torch_activation/relu_family.py
--rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 torch_activation-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      466 2023-05-26 05:16:22.044757 torch_activation-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2642 2023-05-26 05:15:36.983248 torch_activation-0.1.0/README.md
+-rw-r--r--   0        0        0      546 2023-05-26 05:16:03.785176 torch_activation-0.1.0/torch_activation/__init__.py
+-rw-r--r--   0        0        0     2773 2023-05-26 05:12:46.037659 torch_activation-0.1.0/torch_activation/composite.py
+-rw-r--r--   0        0        0     3492 2023-05-23 01:10:45.441694 torch_activation-0.1.0/torch_activation/glu_family.py
+-rw-r--r--   0        0        0     2613 2023-05-24 04:44:25.674253 torch_activation-0.1.0/torch_activation/lincomb.py
+-rw-r--r--   0        0        0     2531 2023-05-24 04:28:43.623528 torch_activation-0.1.0/torch_activation/non_linear.py
+-rw-r--r--   0        0        0     4774 2023-05-24 04:44:04.736433 torch_activation-0.1.0/torch_activation/relu_family.py
+-rw-r--r--   0        0        0     3681 2023-05-26 05:00:14.812656 torch_activation-0.1.0/torch_activation/trig.py
+-rw-r--r--   0        0        0     2877 2023-05-26 04:49:13.643443 torch_activation-0.1.0/torch_activation/utils.py
+-rw-r--r--   0        0        0     3329 1970-01-01 00:00:00.000000 torch_activation-0.1.0/setup.py
+-rw-r--r--   0        0        0     3298 1970-01-01 00:00:00.000000 torch_activation-0.1.0/PKG-INFO
```

### Comparing `torch_activation-0.0.1/torch_activation/glu_family.py` & `torch_activation-0.1.0/torch_activation/glu_family.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-from torch import Tensor
-
-
-class ReGLU(torch.nn.Module):
-    r"""
-    Applies the GeGLU activation function, defined as:
-
-    :math:`\text{GeGLU}(x) = \text{ReLU} (xW + b) \odot (xV + c)`
-
-    Args:
-        inplace: can optionally do the operation in-place. Default: ``False``
-        size: The size of the last dimension of the input tensor.
-
-    Shape:
-        - Input: :math:`(*)` where :math:`*` means any number of additional dimensions.
-        - Output: :math:`(*)`
-
-    Examples::
-
-        >>> m = ReGLU(20)
-        >>> input = torch.randn(3, 20, 20)
-        >>> output = m(input)
-
-    """
-
-    def __init__(self, size:int):
-        super(ReGLU, self).__init__()
-        self.linear = nn.Linear(size, size*2)
-
-    def forward(self, x) -> Tensor:
-        a, b = self.linear(x).chunk(2, dim=-1)
-        return a * F.relu(b)
-
-
-class GeGLU(torch.nn.Module):
-    r"""
-    Applies the GeGLU activation function, defined as:
-
-    :math:`\text{GeGLU}(x) = \text{GELU} (xW + b) \odot (xV + c)`
-
-    Args:
-        inplace: can optionally do the operation in-place. Default: ``False``
-        size: The size of the last dimension of the input tensor.
-
-    Shape:
-        - Input: :math:`(*)` where :math:`*` means any number of additional dimensions.
-        - Output: :math:`(*)`
-
-    Examples::
-
-        >>> m = GeGLU(20)
-        >>> input = torch.randn(3, 20, 20)
-        >>> output = m(input)
-    """
-
-    def __init__(self, size:int):
-        super(GeGLU, self).__init__()
-        self.linear = nn.Linear(size, size*2)
-
-    def forward(self, x) -> Tensor:
-        a, b = self.linear(x).chunk(2, dim=-1)
-        return a * F.gelu(b)
-
-
-class SwiGLU(torch.nn.Module):
-    r"""
-    Applies the SwiGLU activation function, defined as:
-
-    :math:`\text{SwiGLU}(x) =  \text{Swish} (xW + b) \odot (xV + c)`
-
-    Args:
-        inplace: can optionally do the operation in-place. Default: ``False``
-        size: The size of the last dimension of the input tensor.
-
-    Shape:
-        - Input: :math:`(*)` where :math:`*` means any number of additional dimensions.
-        - Output: :math:`(*)`
-
-    Examples::
-
-        >>> m = SwiGLU(20)
-        >>> input = torch.randn(3, 20, 20)
-        >>> output = m(input)
-    """
-
-    def __init__(self, size:int):
-        super(SwiGLU, self).__init__()
-        self.linear = nn.Linear(size, size*2)
-
-    def forward(self, x) -> Tensor:
-        a, b = self.linear(x).chunk(2, dim=-1)
-        return a * F.silu(b)
-    
-class SeGLU(torch.nn.Module):
-    r"""
-    Applies the SeGLU activation function, defined as:
-
-    :math:`\text{SeGLU}(x) =  \text{SELU} (xW + b) \odot (xV + c)`
-
-    Args:
-        inplace: can optionally do the operation in-place. Default: ``False``
-        size: The size of the last dimension of the input tensor.
-
-    Shape:
-        - Input: :math:`(*)` where :math:`*` means any number of additional dimensions.
-        - Output: :math:`(*)`
-
-    Examples::
-
-        >>> m = SeGLU(20)
-        >>> input = torch.randn(3, 20, 20)
-        >>> output = m(input)
-    """
-
-    def __init__(self, size:int):
-        super(SeGLU, self).__init__()
-        self.linear = nn.Linear(size, size*2)
-
-    def forward(self, x) -> Tensor:
-        a, b = self.linear(x).chunk(2, dim=-1)
-        return a * F.selu(b)
-
-if __name__ == "__main__":
-    pass    
-
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+from torch import Tensor
+
+
+class ReGLU(torch.nn.Module):
+    r"""
+    Applies the GeGLU activation function, defined as:
+
+    :math:`\text{GeGLU}(x) = \text{ReLU} (xW + b) \odot (xV + c)`
+
+    Args:
+        inplace: can optionally do the operation in-place. Default: ``False``
+        size: The size of the last dimension of the input tensor.
+
+    Shape:
+        - Input: :math:`(*)` where :math:`*` means any number of additional dimensions.
+        - Output: :math:`(*)`
+
+    Examples::
+
+        >>> m = ReGLU(20)
+        >>> input = torch.randn(3, 20, 20)
+        >>> output = m(input)
+
+    """
+
+    def __init__(self, size:int):
+        super(ReGLU, self).__init__()
+        self.linear = nn.Linear(size, size*2)
+
+    def forward(self, x) -> Tensor:
+        a, b = self.linear(x).chunk(2, dim=-1)
+        return a * F.relu(b)
+
+
+class GeGLU(torch.nn.Module):
+    r"""
+    Applies the GeGLU activation function, defined as:
+
+    :math:`\text{GeGLU}(x) = \text{GELU} (xW + b) \odot (xV + c)`
+
+    Args:
+        inplace: can optionally do the operation in-place. Default: ``False``
+        size: The size of the last dimension of the input tensor.
+
+    Shape:
+        - Input: :math:`(*)` where :math:`*` means any number of additional dimensions.
+        - Output: :math:`(*)`
+
+    Examples::
+
+        >>> m = GeGLU(20)
+        >>> input = torch.randn(3, 20, 20)
+        >>> output = m(input)
+    """
+
+    def __init__(self, size:int):
+        super(GeGLU, self).__init__()
+        self.linear = nn.Linear(size, size*2)
+
+    def forward(self, x) -> Tensor:
+        a, b = self.linear(x).chunk(2, dim=-1)
+        return a * F.gelu(b)
+
+
+class SwiGLU(torch.nn.Module):
+    r"""
+    Applies the SwiGLU activation function, defined as:
+
+    :math:`\text{SwiGLU}(x) =  \text{Swish} (xW + b) \odot (xV + c)`
+
+    Args:
+        inplace: can optionally do the operation in-place. Default: ``False``
+        size: The size of the last dimension of the input tensor.
+
+    Shape:
+        - Input: :math:`(*)` where :math:`*` means any number of additional dimensions.
+        - Output: :math:`(*)`
+
+    Examples::
+
+        >>> m = SwiGLU(20)
+        >>> input = torch.randn(3, 20, 20)
+        >>> output = m(input)
+    """
+
+    def __init__(self, size:int):
+        super(SwiGLU, self).__init__()
+        self.linear = nn.Linear(size, size*2)
+
+    def forward(self, x) -> Tensor:
+        a, b = self.linear(x).chunk(2, dim=-1)
+        return a * F.silu(b)
+    
+class SeGLU(torch.nn.Module):
+    r"""
+    Applies the SeGLU activation function, defined as:
+
+    :math:`\text{SeGLU}(x) =  \text{SELU} (xW + b) \odot (xV + c)`
+
+    Args:
+        inplace: can optionally do the operation in-place. Default: ``False``
+        size: The size of the last dimension of the input tensor.
+
+    Shape:
+        - Input: :math:`(*)` where :math:`*` means any number of additional dimensions.
+        - Output: :math:`(*)`
+
+    Examples::
+
+        >>> m = SeGLU(20)
+        >>> input = torch.randn(3, 20, 20)
+        >>> output = m(input)
+    """
+
+    def __init__(self, size:int):
+        super(SeGLU, self).__init__()
+        self.linear = nn.Linear(size, size*2)
+
+    def forward(self, x) -> Tensor:
+        a, b = self.linear(x).chunk(2, dim=-1)
+        return a * F.selu(b)
+
+if __name__ == "__main__":
+    pass    
+
```

### Comparing `torch_activation-0.0.1/torch_activation/relu_family.py` & `torch_activation-0.1.0/torch_activation/relu_family.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-from torch import Tensor
-
-
-class ShiLU(nn.Module):
-    r"""
-    Applies the ShiLU activation function:
-
-    :math:`\text{ShiLU}(x) = \alpha * \max(0,x) + \beta`
-
-    Args:
-        alpha : Scaling factor for the positive part of the input. Default: 1.0.
-        beta : Bias term added to the output. Default: 0.0.
-        inplace: can optionally do the operation in-place. Default: ``False``
-
-    Shape:
-        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
-        - Output: :math:`(*)`, same shape as the input.
-        
-    Attributes:
-        alpha : Scaling factor for the positive part of the input. Default: 1.0.
-        beta : Bias term added to the output. Default: 0.0.
-
-    .. image:: ../images/activation_images/ShiLU.png
-
-    Examples::
-    
-        >>> m = ShiLU(alpha=2.0, beta=1.0)
-        >>> x = torch.randn(2)
-        >>> output = m(x)
-
-        >>> m = ShiLU(inplace=True)
-        >>> x = torch.randn(2, 3, 4)
-        >>> m(x)
-    """
-
-    def __init__(self, alpha=1.0, beta=0.0, inplace=False):
-        super().__init__()
-        self.alpha = nn.Parameter(torch.tensor(alpha))
-        self.beta  = nn.Parameter(torch.tensor(beta))
-        self.inplace = inplace
-
-    def forward(self, x):
-        if self.inplace:
-            F.relu_(x)
-            x.mul_(self.alpha)
-            x.add_(self.beta)
-            return x
-        else:    
-            return self.alpha * F.relu(x) + self.beta
-        
-
-class CReLU(nn.Module):
-    r"""
-    Applies the Concatenated Rectified Linear Unit activation function.
-
-    :math:`\text{CReLU}(x) = \max(0,x) \oplus \max(0,-x)`
-
-    Args:
-        dim: Dimension along which to concatenate in the output tensor. Default: 1
-        inplace: can optionally do the operation in-place. Default: ``False``
-
-    Shape:
-        - Input: :math:`(*, C, *)` where :math:`*` means any number of additional dimensions
-        - Output: :math:`(*, 2C, *)`
-
-    .. image:: ../images/activation_images/CReLU.png
-
-    Examples::
-
-        >>> m = nn.CReLU()
-        >>> x = torch.randn(2, 3)
-        >>> output = m(x)
-        
-        >>> m = CReLU(inplace=True)
-        >>> x = torch.randn(2, 3, 4)
-        >>> m(x)
-    """
-    
-    
-    def __init__(self, dim=0):
-        super(CReLU, self).__init__()
-        self.dim = dim
-
-    def forward(self, x):
-        return F.relu(torch.cat((x, -x), dim=self.dim))
-        
-        
-class ReLUN(nn.Module):
-    r"""Applies the element-wise function:
-
-    :math:`\text{ReLUN}(x) = \min(\max(0,x), n)`
-
-    Args:
-        n: Upper bound for the function's output. Default is 1.0.
-        inplace: can optionally do the operation in-place. Default: ``False``
-
-    Shape:
-        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
-        - Output: :math:`(*)`, same shape as the input.
-        
-    Attributes:
-        n: Upper bound for the function's output. Default is 1.0.
-        
-    .. image:: ../images/activation_images/ReLUN.png
-
-    Examples::
-
-        >>> m = nn.ReLUN(n=6.0) # ReLU6
-        >>> x = torch.randn(2)
-        >>> output = m(x)
-        
-        >>> m = nn.ReLUN(inplace=True)
-        >>> x = torch.randn(2)
-        >>> m(x)
-
-    """
-    def __init__(self, n=1.0, inplace=False):
-        super(ReLUN, self).__init__()
-        self.n = nn.Parameter(torch.tensor(n))
-        self.inplace = inplace
-
-    def forward(self, x):
-        if self.inplace:
-            x.clamp_max_(self.n.data)
-            x.relu_()
-            return x
-        else:
-            return torch.clamp(x, 0, self.n.data)
-        
-        
-class SquaredReLU(nn.Module):
-    r"""
-    Applies the element-wise function:
-
-    :math:`\text{SquaredReLU}(x) = \text{ReLU}(x)^2`
-
-    Args:
-        inplace: can optionally do the operation in-place. Default: ``False``
-
-    Shape:
-        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
-        - Output: :math:`(*)`, same shape as the input.
-        
-    .. image:: ../images/activation_images/SquaredReLU.png
-
-    Examples::
-
-        >>> m = nn.SquaredReLU()
-        >>> x = torch.randn(2)
-        >>> output = m(x)
-
-        >>> m = nn.SquaredReLU(inplace=True)
-        >>> x = torch.randn(2)
-        >>> m(x)
-    """
-    
-    
-    def __init__(self, inplace=False):
-        super().__init__()
-        self.inplace = inplace
-
-    def forward(self, x) -> Tensor:
-        if self.inplace:
-            return F.relu_(x).pow_(2)
-        else:
-            return F.relu(x).pow(2)
-    
-    
-if __name__ == '__main__':
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+from torch import Tensor
+
+
+class ShiLU(nn.Module):
+    r"""
+    Applies the ShiLU activation function:
+
+    :math:`\text{ShiLU}(x) = \alpha * \max(0,x) + \beta`
+
+    Args:
+        alpha : Scaling factor for the positive part of the input. Default: 1.0.
+        beta : Bias term added to the output. Default: 0.0.
+        inplace: can optionally do the operation in-place. Default: ``False``
+
+    Shape:
+        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
+        - Output: :math:`(*)`, same shape as the input.
+        
+    Attributes:
+        alpha : Scaling factor for the positive part of the input. Default: 1.0.
+        beta : Bias term added to the output. Default: 0.0.
+
+    .. image:: ../images/activation_images/ShiLU.png
+
+    Examples::
+    
+        >>> m = ShiLU(alpha=2.0, beta=1.0)
+        >>> x = torch.randn(2)
+        >>> output = m(x)
+
+        >>> m = ShiLU(inplace=True)
+        >>> x = torch.randn(2, 3, 4)
+        >>> m(x)
+    """
+
+    def __init__(self, alpha=1.0, beta=0.0, inplace=False):
+        super().__init__()
+        self.alpha = nn.Parameter(torch.tensor(alpha))
+        self.beta  = nn.Parameter(torch.tensor(beta))
+        self.inplace = inplace
+
+    def forward(self, x) -> Tensor:
+        if self.inplace:
+            F.relu_(x)
+            x.mul_(self.alpha)
+            x.add_(self.beta)
+            return x
+        else:    
+            return self.alpha * F.relu(x) + self.beta
+        
+
+class CReLU(nn.Module):
+    r"""
+    Applies the Concatenated Rectified Linear Unit activation function.
+
+    :math:`\text{CReLU}(x) = \max(0,x) \oplus \max(0,-x)`
+
+    Args:
+        dim: Dimension along which to concatenate in the output tensor. Default: 1
+        inplace: can optionally do the operation in-place. Default: ``False``
+
+    Shape:
+        - Input: :math:`(*, C, *)` where :math:`*` means any number of additional dimensions
+        - Output: :math:`(*, 2C, *)`
+
+    .. image:: ../images/activation_images/CReLU.png
+
+    Examples::
+
+        >>> m = nn.CReLU()
+        >>> x = torch.randn(2, 3)
+        >>> output = m(x)
+        
+        >>> m = CReLU(inplace=True)
+        >>> x = torch.randn(2, 3, 4)
+        >>> m(x)
+    """
+    
+    
+    def __init__(self, dim=0):
+        super(CReLU, self).__init__()
+        self.dim = dim
+
+    def forward(self, x) -> Tensor:
+        return F.relu(torch.cat((x, -x), dim=self.dim))
+        
+        
+class ReLUN(nn.Module):
+    r"""Applies the element-wise function:
+
+    :math:`\text{ReLUN}(x) = \min(\max(0,x), n)`
+
+    Args:
+        n: Upper bound for the function's output. Default is 1.0.
+        inplace: can optionally do the operation in-place. Default: ``False``
+
+    Shape:
+        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
+        - Output: :math:`(*)`, same shape as the input.
+        
+    Attributes:
+        n: Upper bound for the function's output. Default is 1.0.
+        
+    .. image:: ../images/activation_images/ReLUN.png
+
+    Examples::
+
+        >>> m = nn.ReLUN(n=6.0) # ReLU6
+        >>> x = torch.randn(2)
+        >>> output = m(x)
+        
+        >>> m = nn.ReLUN(inplace=True)
+        >>> x = torch.randn(2)
+        >>> m(x)
+
+    """
+    def __init__(self, n=1.0, inplace=False):
+        super(ReLUN, self).__init__()
+        self.n = nn.Parameter(torch.tensor(n))
+        self.inplace = inplace
+
+    def forward(self, x) -> Tensor:
+        if self.inplace:
+            x.clamp_max_(self.n.data)
+            x.relu_()
+            return x
+        else:
+            return torch.clamp(x, 0, self.n.data)
+        
+        
+class SquaredReLU(nn.Module):
+    r"""
+    Applies the element-wise function:
+
+    :math:`\text{SquaredReLU}(x) = \text{ReLU}(x)^2`
+
+    Args:
+        inplace: can optionally do the operation in-place. Default: ``False``
+
+    Shape:
+        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
+        - Output: :math:`(*)`, same shape as the input.
+        
+    .. image:: ../images/activation_images/SquaredReLU.png
+
+    Examples::
+
+        >>> m = nn.SquaredReLU()
+        >>> x = torch.randn(2)
+        >>> output = m(x)
+
+        >>> m = nn.SquaredReLU(inplace=True)
+        >>> x = torch.randn(2)
+        >>> m(x)
+    """
+    
+    
+    def __init__(self, inplace=False):
+        super().__init__()
+        self.inplace = inplace
+
+    def forward(self, x) -> Tensor:
+        if self.inplace:
+            return F.relu_(x).pow_(2)
+        else:
+            return F.relu(x).pow(2)
+    
+    
+if __name__ == '__main__':
     pass
```

