# Comparing `tmp/torchbones-1.0.4.tar.gz` & `tmp/torchbones-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbones-1.0.4.tar", last modified: Fri May 26 19:26:06 2023, max compression
+gzip compressed data, was "torchbones-1.0.5.tar", last modified: Fri May 26 20:19:54 2023, max compression
```

## Comparing `torchbones-1.0.4.tar` & `torchbones-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-26 19:26:06.170776 torchbones-1.0.4/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-26 19:26:06.170776 torchbones-1.0.4/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-05-26 19:26:06.170776 torchbones-1.0.4/setup.cfg
--rw-r--r--   0 oross314  (1000) oross314  (1000)      441 2023-05-26 19:25:56.000000 torchbones-1.0.4/setup.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-26 19:26:06.170776 torchbones-1.0.4/torchbones/
--rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.0.4/torchbones/__init__.py
--rw-r--r--   0 oross314  (1000) oross314  (1000)    14981 2023-05-26 17:39:33.000000 torchbones-1.0.4/torchbones/main.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-26 19:26:06.170776 torchbones-1.0.4/torchbones.egg-info/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-26 19:26:06.000000 torchbones-1.0.4/torchbones.egg-info/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-05-26 19:26:06.000000 torchbones-1.0.4/torchbones.egg-info/SOURCES.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-05-26 19:26:06.000000 torchbones-1.0.4/torchbones.egg-info/dependency_links.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       30 2023-05-26 19:26:06.000000 torchbones-1.0.4/torchbones.egg-info/requires.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-05-26 19:26:06.000000 torchbones-1.0.4/torchbones.egg-info/top_level.txt
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-26 20:19:53.994946 torchbones-1.0.5/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-26 20:19:53.994946 torchbones-1.0.5/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-05-26 20:19:53.994946 torchbones-1.0.5/setup.cfg
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      441 2023-05-26 20:19:03.000000 torchbones-1.0.5/setup.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-26 20:19:53.994946 torchbones-1.0.5/torchbones/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.0.5/torchbones/__init__.py
+-rw-r--r--   0 oross314  (1000) oross314  (1000)    15442 2023-05-26 20:18:52.000000 torchbones-1.0.5/torchbones/main.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-05-26 20:19:53.994946 torchbones-1.0.5/torchbones.egg-info/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      266 2023-05-26 20:19:53.000000 torchbones-1.0.5/torchbones.egg-info/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-05-26 20:19:53.000000 torchbones-1.0.5/torchbones.egg-info/SOURCES.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-05-26 20:19:53.000000 torchbones-1.0.5/torchbones.egg-info/dependency_links.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       30 2023-05-26 20:19:53.000000 torchbones-1.0.5/torchbones.egg-info/requires.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-05-26 20:19:53.000000 torchbones-1.0.5/torchbones.egg-info/top_level.txt
```

### Comparing `torchbones-1.0.4/torchbones/main.py` & `torchbones-1.0.5/torchbones/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import pickle
 import matplotlib.pyplot as plt
 import sys, os
 import warnings
 import math
 import copy 
 
-
+weight_path = 'weights'
+val_file = 'values.p'
 
 class Net(nn.Module):
     def __init__(self, *args):
         super(Net, self).__init__()
         sizes, self.convs, lins, csizes,  dropout, self.resnet, self.activation = args  
         
         if self.resnet:
@@ -85,16 +86,16 @@
         return output
 
     
 class Model:
     def __init__(self, *args, **kwargs):
         self.lins, self.activation, optimizer,  self.batch_size, self.lr, self.indata, self.truth, self.cost =args
         
-        keys = ('convs', 'csizes','lr_decay', 'max_epochs', 'saving', 'run_num', 'new_tar',
-                'lr_min','dropout',  'plot_ev', 'print_ev', 'resnet', 'train_fac', 'cov')
+        keys = ('convs', 'csizes','lr_decay',  'saving', 'run_num', 'new_tar', 'save_weights',
+                'lr_min','dropout',  'plot_ev', 'print_ev', 'resnet', 'train_fac', 'cov', 'check')
         for kwarg in kwargs.keys():
             if kwarg not in keys:
                 raise Exception(kwarg + ' is not a valid key. Valid keys: ', keys )
         
         self.cov = kwargs.get('cov', 1)
         self.convs = kwargs.get('convs', [])
         self.csizes = kwargs.get('csizes', [])
@@ -120,25 +121,32 @@
         self.dropout = kwargs.get('dropout', 0)
         self.net = Net(self.indata.shape[1:], self.convs, self.lins,  self.csizes, self.dropout, 
                              self.resnet, self.activation).double()
         
         self.lr_decay = kwargs.get('lr_decay', 1)
         self.lr_min = kwargs.get('lr_min', 1e-10)
         self.optimizer = optimizer(self.net.parameters(), lr = self.lr)
-        self.max_epochs = kwargs.get('max_epochs', 20)
             
         self.trainerr, self.testerr, self.err, self.epoch, self.loc, self.save_file = [], [], 0, 0, 0, None #just inits
         
         self.saving = kwargs.get('saving', False)
-        
-        self.new_tar = kwargs.get('new_tar', False)
+        self.save_tar = kwargs.get('save_weights', False)
+        if self.save_tar and not os.path.isdir(weight_path):
+            os.makedirs(weight_path)
+        
+        if self.save_tar and not self.saving:
+            raise Exception('Saving must be enabled to save model weights')
+        if self.save and not os.path.exists('values.p'):
+            pickle.dump(self.params(), open('values.p', 'wb'))
+            
         self.run_num = kwargs.get('run_num', None)
-        self.check()
-
-        
+        self.new_tar = kwargs.get('new_tar', False)
+        check = kwargs.get('check', True)
+        if check:
+            self.check()
         if self.run_num:
             vals = pickle.load(open('values.p','rb')).loc[self.run_num]
             self.epoch = vals['epochs']
             self.err = vals['err']
             self.lr = vals['learning rate']
             print('Weights from run ', str(self.run_num), ' loaded.')
         else: self.epoch = 0        
@@ -184,30 +192,30 @@
         if self.run_num and len(same):
             same = list(np.delete(same, np.where(same == self.run_num)))
         if len(same):
             warnings.warn('Run(s) '+ str(same) + ' used the same hyper parameters')
             
         # if saving to a new file, load weights. If continuing run, check that vals match
         if self.new_tar and type(self.run_num)==int:
-            self.net.load_state_dict(torch.load('tars/' + str(self.run_num)+'.tar'))        
+            self.net.load_state_dict(torch.load(weight_path + '/' + str(self.run_num)+'.tar'))        
         elif not self.new_tar and self.run_num:
             if vals.loc[self.run_num][:5].equals(df.loc[self.loc][:5]):
                 self.loc = self.run_num
-                self.net.load_state_dict(torch.load('tars/' + str(self.loc)+'.tar'))   
+                self.net.load_state_dict(torch.load(weight_path + '/' + str(self.loc)+'.tar'))   
             else: raise Exception('Parameters don\'t match')
 
                      
         if not self.loc: 
             self.loc = vals.index[-1] + 1
     
-        if not self.saving:
+        if not self.save_tar:
             self.save_file = None
             print('Not saving')
         else: 
-            self.save_file = 'tars/' + str(self.loc)+'.tar'
+            self.save_file = weight_path + '/' + str(self.loc)+'.tar'
             
     def save(self): 
         torch.save(self.net.state_dict(), self.save_file)
         vals = pickle.load(open('values.p', 'rb'))
         df = self.params()
         if self.loc in vals.index.tolist():
             vals.loc[self.loc] = df.loc[self.loc]
@@ -215,36 +223,34 @@
             vals = vals.append( df)
         pickle.dump(vals, open('values.p', 'wb'))
         
   
         
                 
     def run(self, **kwargs):
-        if self.max_epochs ==self.epoch:
-            print('maximum epoch reached')
         if len(self.trainerr)!=len(self.testerr):
             self.trainerr = self.trainerr[:-1]
         keys = ('lr', 'lr_decay', 'max_epochs', 'saving', 'batch_size', 'lr_min', 'training',)
         for kwarg in kwargs.keys():
             if kwarg not in keys:
                 raise Exception(kwarg + ' is not a valid key. Valid keys: ', keys )
                 
         train, traintruth, traincov, test, testtruth, testcov = self.data
-        self.max_epochs = kwargs.get('max_epochs', self.max_epochs)
+        self.max_epochs = kwargs.get('max_epochs', 20)
         self.lr = kwargs.get('lr', self.lr)
         self.saving = kwargs.get('saving', self.saving)
         self.lr_decay = kwargs.get('lr_decay', self.lr_decay)
         self.batch_size = kwargs.get('batch_size', self.batch_size)
         self.lr_min = kwargs.get('lr_min', self.lr_min)
         training = kwargs.get('training', True)
         self.printev = kwargs.get('print_ev', self.printev)
         self.plotev = kwargs.get('plot_ev', self.plotev)
         e0 = self.epoch
         
-        while self.epoch + e0 < self.max_epochs:
+        while self.epoch - e0 < self.max_epochs:
             shuffle = torch.randperm(len(traintruth)) #shuffle training set
             self.lr = max(self.lr * self.lr_decay, self.lr_min)  #lr decay
             for i in range(round(len(traintruth)/self.batch_size)):
                 self.optimizer.param_groups[0]['lr'] = self.lr
                 where = shuffle[i * self.batch_size:(i + 1) * self.batch_size] #take batch of training set
                 self.output = self.net(train[where])
                 self.truetrain = traintruth[where]
@@ -280,14 +286,16 @@
                 self.checkpoint(t)
                 
             if self.saving:
                 self.save()
             self.epoch += 1
     
     def checkpoint(self, t = 10): 
+        if len(self.trainerr) < t +1:
+            return 0
         if not self.epoch>t:
             #create a checkpoint
             self.oldmodel = copy.deepcopy(self.net.state_dict())#create a checkpoint to return to if training goes off the rails
             self.oldlr = 1*self.lr
             self.countcheck = 0
         elif (self.trainerr[-1]/self.trainerr[-1 - t]>5) or (self.trainerr[-1]!=self.trainerr[-1]):
             #return to checkpoint if necessary
```

