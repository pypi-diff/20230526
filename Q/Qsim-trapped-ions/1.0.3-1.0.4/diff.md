# Comparing `tmp/Qsim_trapped_ions-1.0.3.tar.gz` & `tmp/Qsim_trapped_ions-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Qsim_trapped_ions-1.0.3.tar", last modified: Tue May 23 09:42:13 2023, max compression
+gzip compressed data, was "Qsim_trapped_ions-1.0.4.tar", last modified: Fri May 26 06:12:07 2023, max compression
```

## Comparing `Qsim_trapped_ions-1.0.3.tar` & `Qsim_trapped_ions-1.0.4.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 09:42:13.112881 Qsim_trapped_ions-1.0.3/
--rw-rw-rw-   0        0        0     4285 2023-05-23 09:42:13.112881 Qsim_trapped_ions-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-23 09:42:13.071872 Qsim_trapped_ions-1.0.3/Qsim/
-drwxrwxrwx   0        0        0        0 2023-05-23 09:42:13.078008 Qsim_trapped_ions-1.0.3/Qsim/ion_chain/
--rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.3/Qsim/ion_chain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:42:13.081009 Qsim_trapped_ions-1.0.3/Qsim/ion_chain/eigendiagram/
--rw-rw-rw-   0        0        0     7825 2023-04-22 20:45:12.000000 Qsim_trapped_ions-1.0.3/Qsim/ion_chain/eigendiagram/exci_diagram.py
--rw-rw-rw-   0        0        0      111 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.3/Qsim/ion_chain/eigendiagram/init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:42:13.085010 Qsim_trapped_ions-1.0.3/Qsim/ion_chain/interaction/
--rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.3/Qsim/ion_chain/interaction/__init__.py
--rw-rw-rw-   0        0        0     2853 2023-03-27 05:10:36.000000 Qsim_trapped_ions-1.0.3/Qsim/ion_chain/interaction/pure_spin.py
--rw-rw-rw-   0        0        0     7440 2023-02-19 21:26:44.000000 Qsim_trapped_ions-1.0.3/Qsim/ion_chain/interaction/spin_phonon.py
--rw-rw-rw-   0        0        0    30482 2023-05-23 08:53:03.000000 Qsim_trapped_ions-1.0.3/Qsim/ion_chain/ion_system.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:42:13.088831 Qsim_trapped_ions-1.0.3/Qsim/ion_chain/ising/
--rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.3/Qsim/ion_chain/ising/__init__.py
--rw-rw-rw-   0        0        0     1569 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.3/Qsim/ion_chain/ising/ising_c.py
--rw-rw-rw-   0        0        0     4045 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.3/Qsim/ion_chain/ising/ising_ps.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:42:13.099390 Qsim_trapped_ions-1.0.3/Qsim/ion_chain/transfer/
--rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.3/Qsim/ion_chain/transfer/__init__.py
--rw-rw-rw-   0        0        0    15712 2023-03-07 21:30:48.000000 Qsim_trapped_ions-1.0.3/Qsim/ion_chain/transfer/anharmonic_transfer - 副本.py
--rw-rw-rw-   0        0        0    15800 2023-03-08 00:56:56.000000 Qsim_trapped_ions-1.0.3/Qsim/ion_chain/transfer/anharmonic_transfer.py
--rw-rw-rw-   0        0        0     3037 2023-02-20 05:11:39.000000 Qsim_trapped_ions-1.0.3/Qsim/ion_chain/transfer/chaos.py
--rw-rw-rw-   0        0        0     3063 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.3/Qsim/ion_chain/transfer/elec_transfer.py
--rw-rw-rw-   0        0        0    13991 2023-03-05 19:12:10.000000 Qsim_trapped_ions-1.0.3/Qsim/ion_chain/transfer/exci_operators.py
--rw-rw-rw-   0        0        0     4323 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.3/Qsim/ion_chain/transfer/exci_transfer.py
--rw-rw-rw-   0        0        0     5700 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.3/Qsim/ion_chain/transfer/multi_core.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:42:13.104277 Qsim_trapped_ions-1.0.3/Qsim/operator/
--rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.3/Qsim/operator/__init__.py
--rw-rw-rw-   0        0        0     7121 2023-03-05 17:06:10.000000 Qsim_trapped_ions-1.0.3/Qsim/operator/phonon.py
--rw-rw-rw-   0        0        0     6429 2023-02-27 23:34:30.000000 Qsim_trapped_ions-1.0.3/Qsim/operator/spin.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:42:13.110876 Qsim_trapped_ions-1.0.3/Qsim_trapped_ions.egg-info/
--rw-rw-rw-   0        0        0     4285 2023-05-23 09:42:12.000000 Qsim_trapped_ions-1.0.3/Qsim_trapped_ions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      986 2023-05-23 09:42:13.000000 Qsim_trapped_ions-1.0.3/Qsim_trapped_ions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 09:42:12.000000 Qsim_trapped_ions-1.0.3/Qsim_trapped_ions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-23 09:42:12.000000 Qsim_trapped_ions-1.0.3/Qsim_trapped_ions.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-23 09:42:12.000000 Qsim_trapped_ions-1.0.3/Qsim_trapped_ions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4035 2023-05-23 09:08:47.000000 Qsim_trapped_ions-1.0.3/README.rst
--rw-rw-rw-   0        0        0       42 2023-05-23 09:42:13.112881 Qsim_trapped_ions-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1216 2023-05-23 09:42:02.000000 Qsim_trapped_ions-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:12:07.780077 Qsim_trapped_ions-1.0.4/
+-rw-rw-rw-   0        0        0     4294 2023-05-26 06:12:07.779072 Qsim_trapped_ions-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-26 06:12:07.737583 Qsim_trapped_ions-1.0.4/Qsim/
+drwxrwxrwx   0        0        0        0 2023-05-26 06:12:07.741596 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/
+-rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:12:07.744907 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/eigendiagram/
+-rw-rw-rw-   0        0        0     7825 2023-04-22 20:45:12.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/eigendiagram/exci_diagram.py
+-rw-rw-rw-   0        0        0      111 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/eigendiagram/init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:12:07.749440 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/interaction/
+-rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/interaction/__init__.py
+-rw-rw-rw-   0        0        0     2853 2023-03-27 05:10:36.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/interaction/pure_spin.py
+-rw-rw-rw-   0        0        0     7440 2023-02-19 21:26:44.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/interaction/spin_phonon.py
+-rw-rw-rw-   0        0        0    30412 2023-05-26 06:01:34.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/ion_system.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:12:07.753600 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/ising/
+-rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/ising/__init__.py
+-rw-rw-rw-   0        0        0     1569 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/ising/ising_c.py
+-rw-rw-rw-   0        0        0     4045 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/ising/ising_ps.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:12:07.765197 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/
+-rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/__init__.py
+-rw-rw-rw-   0        0        0    15712 2023-03-07 21:30:48.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/anharmonic_transfer - 副本.py
+-rw-rw-rw-   0        0        0    15800 2023-03-08 00:56:56.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/anharmonic_transfer.py
+-rw-rw-rw-   0        0        0     3037 2023-02-20 05:11:39.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/chaos.py
+-rw-rw-rw-   0        0        0     3063 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/elec_transfer.py
+-rw-rw-rw-   0        0        0    13991 2023-03-05 19:12:10.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/exci_operators.py
+-rw-rw-rw-   0        0        0     4323 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/exci_transfer.py
+-rw-rw-rw-   0        0        0     5700 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/multi_core.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:12:07.768714 Qsim_trapped_ions-1.0.4/Qsim/operator/
+-rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.4/Qsim/operator/__init__.py
+-rw-rw-rw-   0        0        0     7121 2023-03-05 17:06:10.000000 Qsim_trapped_ions-1.0.4/Qsim/operator/phonon.py
+-rw-rw-rw-   0        0        0     6429 2023-02-27 23:34:30.000000 Qsim_trapped_ions-1.0.4/Qsim/operator/spin.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:12:07.776047 Qsim_trapped_ions-1.0.4/Qsim_trapped_ions.egg-info/
+-rw-rw-rw-   0        0        0     4294 2023-05-26 06:12:07.000000 Qsim_trapped_ions-1.0.4/Qsim_trapped_ions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      988 2023-05-26 06:12:07.000000 Qsim_trapped_ions-1.0.4/Qsim_trapped_ions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 06:12:07.000000 Qsim_trapped_ions-1.0.4/Qsim_trapped_ions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-26 06:12:07.000000 Qsim_trapped_ions-1.0.4/Qsim_trapped_ions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-26 06:12:07.000000 Qsim_trapped_ions-1.0.4/Qsim_trapped_ions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 06:12:07.780077 Qsim_trapped_ions-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1207 2023-05-26 05:56:05.000000 Qsim_trapped_ions-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:12:07.778069 Qsim_trapped_ions-1.0.4/test/
+-rw-rw-rw-   0        0        0      147 2023-05-26 03:52:59.000000 Qsim_trapped_ions-1.0.4/test/test.py
```

### Comparing `Qsim_trapped_ions-1.0.3/PKG-INFO` & `Qsim_trapped_ions-1.0.4/Qsim_trapped_ions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: Qsim_trapped_ions
-Version: 1.0.3
+Name: Qsim-trapped-ions
+Version: 1.0.4
 Summary: Numerical simulation of trapped ion quantum dynamics
 Home-page: https://github.com/TrappedIonRice/Open-Quantum-system-simulation
-Author: mjz
+Author: Mingjian Zhu
 Author-email: mz40@rice.edu
 
 # Open-Quantum-system-simulation
 package: ion_chain
 
 dependence pakcage: Qutip
```

### Comparing `Qsim_trapped_ions-1.0.3/Qsim/ion_chain/eigendiagram/exci_diagram.py` & `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/eigendiagram/exci_diagram.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.3/Qsim/ion_chain/interaction/pure_spin.py` & `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/interaction/pure_spin.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.3/Qsim/ion_chain/interaction/spin_phonon.py` & `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/interaction/spin_phonon.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.3/Qsim/ion_chain/ion_system.py` & `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/ion_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # -*- coding: utf-8 -*-
 """
 Created on Wed Jun  1 15:47:46 2022
-
 @author: zhumj
 A class that contains basic physical and computational parameters of 1-D N ion system with 1 laser drive
 """
 
 import matplotlib.pyplot as plt
 import numpy as np
 from qutip import *
@@ -29,15 +28,14 @@
         input frequency, in Hz, kHz, or MHz
     unit : str
         specify the unit, can be 'hz', 'khz', 'mhz'
     Returns
     -------
     f_out : float
         output radial frequency, unit of 2pi Hz
-
     '''
     factor = {'hz':0,'khz':3,'mhz':6}
     f_out = 2*np.pi * f*10**(factor[unit])
     return f_out
 '''
 subfunction
 '''
@@ -116,52 +114,46 @@
     '''
     compute the length scale of the system, in SI
     input(fz)
     Parameters
     ----------
     fz : flaot
         axial frequency of the ion trap, [MHz]
-
     Returns
     -------
     float, unit of m
-
     '''
     return (qe**2/ (4*np.pi * eps0 * MYb171 * fr_conv(fz,'mhz')**2))**(1/3)
 def eta(f):
     '''
     Compute single ion Lamb-Dicke parameter for vibrational eigenmode correspond to
     eigenfrequency f
     input(f)
     Parameters
     ----------
     f : float
        eigenfrequency [MHz]
-
     Returns
     -------
     float, unit SI
-
     '''
     return Dk * X0(f) 
 def Omega(fs,fx):
     '''
     Compute side band rabi-rate
     Input(fs,fx)
     Parameters
     ----------
     fs : float
         sideband rabi frequency, [kHz]
     fx : float
         transverse frequency of the ion trap, [MHz]
-
     Returns
     -------
     float, unit [2pi Hz]
-
     '''
     return fr_conv(fs,'khz') / eta(fx)  
 def summary():
     '''
     give a summary of all functions and classes defined in this module
     '''
     print('Class:')
@@ -237,15 +229,14 @@
     coolant = [2] #index of coolant
     df_laser = 1 #vibrational degree of freedom coupled to the laser, 0 for axial, 1 for radial
     laser_couple = [0,1] #ion index that couples to the laser, for instance [0,1] means couple to ion 0, 1
     delta_ref = 0 #reference frequency index, 0 for com frequency
     def list_para(self):
         '''
         list basic physical parameters of the system
-
         '''
         Coup_dic = {0:'Axial', 1:'Transverse (Radial)'}
         freqdic = {'0':'COM freq','1':'tilt freq','2':'rock freq'}
         print('________________________________________________________________')
         print('********************Setup of the Trap************************')
         print('number of ions', self.N)
         print('axial COM (Confining) frequency ',np.round(self.fz,2),' [MHz]')
@@ -269,15 +260,14 @@
         print('corresonding phonon space cutoff ', self.pcut)
         print('spin phase phis',np.round(self.phase*180/np.pi,2))
         print('(input in rad but displayed in degs)')
         print('cooling rate ', np.round(self.gamma,2)," [kHz]") 
     def check_phonon(self):
         '''
         Check the consistency in set up of phonon space
-
         '''
         print('_____________________________________________________________')
         print('Checking phonon space setup')
         checker = 1
         if (len(self.pcut)==len(self.active_phonon)):
             for i in range(len(self.pcut)):
                 if len(self.pcut[i]) != len(self.active_phonon[i]):
@@ -288,29 +278,27 @@
             print('Inconsistency between active phonon space and assigned phonon cutoff')
         else:
             print('consistent')
         print('_____________________________________________________________')    
     def df_spin(self):
         '''
         number of spin degree of freedom to be considered
-
         '''
         return len(self.laser_couple)
     def df_phonon(self):
         '''
         output parameteres to construct phonon space
         Returns
         -------
         ph_space : list 
             the first element is the number of degree of freedoms considered.
             the second second element is list in which each element is the 
             number of phonon space to be considered for a specfic degreea of freedom
             for instance [2, [3, 3]] means 2 degreee of freedom to be considered
             and 3 phonon spaces for each degree of freedom
-
         '''
         ph_space = [len(self.active_phonon)]
         ph_N  = []
         for ph_i in range(len(self.active_phonon)):
             ph_N.append(len(self.active_phonon[ph_i]))
         ph_space.append(ph_N)
         return ph_space
@@ -400,34 +388,30 @@
         plt.legend()
     def alpha(self):
         '''
         compute anisotropy coefficient of the trap
         Returns
         -------
         float, unit of 1
-
         '''
         return (self.fz/self.fx)**2 
     def l0(self):
         '''
         compute the chracteristic length scale of the system
-
         Returns
         -------
         float, unit of m
         '''
         return lc(self.fz)
     def Equi_posi(self):
         '''
         compute the equilibrium position of 1-D ion-chain
-
         Returns
         -------
         np array object, each index a equilibirum position
-
         '''
         return E_position(self.N,self.fz,False,0) 
     def Amatrix(self):
         #compute the tensor A which determines the axial oscillation
         #fz, axial frequency of the ion trap
         eposition = E_position(self.N, self.fz,False,0) 
         Amat = np.zeros((self.N,self.N))
@@ -440,20 +424,18 @@
         #fx, transverse frequency of the ion trap
         Amat = self.Amatrix()
         Tmat = (0.5+(self.fx/self.fz)**2) * np.identity(self.N) - 0.5*Amat
         return Tmat
     def C(self,m,n,p):
         '''
         Compute the anharmonic tensor in the classical Lagrangian 
-
         Parameters
         ----------
         m, n, p : int
         python index from 0~N-1
-
         Returns
         -------
         float
         tensor element m, n, p
         '''
         if (m==n) and (n==p):
             Cmnp = 0
@@ -478,15 +460,14 @@
         '''
         Compute the anharmonic tensor for mode-mode coupling   
         
         Parameters
         ----------
         p0, q, r : int
         python index from 0~N-1
-
         Returns
         -------
         float
         tensor element p, q, r
         '''
         #implement the summation over 3 index
         Dpqr = 0
@@ -504,24 +485,21 @@
                 for n0 in range(N0):
                     nterm = self.C(l,m0,n0) * Amat[p0,l] * Amat[q,m0] * Amat[r,n0]
                     Dpqr = Dpqr + nterm
         return Dpqr 
     def plot_D(self,non_zero=True):
         '''
         Plot absolute value of anharmonic coefficients D_mnp
-
         Parameters
         ----------
         non_zero: bool 
             default is True, if True, only plot non-zero coefficeints     
-
         Returns
         -------
         None.
-
         '''
         Dplot = {}
         for i in range(self.N ):
             for j in range(self.N):
                 for k in range(self.N ):
                     Dvalue = np.abs(self.D(i,j,k))
                     if non_zero:
@@ -537,15 +515,14 @@
         plt.yticks(fontsize = 13)  
         plt.xlabel('Mode index mnp: m,n for radial, p for axial',fontsize = 13)
         plt.grid()       
         plt.show()
     def ah_freq(self,mode_index,ftype):
         '''
         compute the oscillating frequency of the anharmonic term m n p
-
         Parameters
         ----------
         m : int
             index of radial mode 1
         n : int
             index of radial mode
         p : int
@@ -553,37 +530,33 @@
         ftype: int
             determines the type of frequency to be computed
             0 for -
             1 for +
         Returns
         -------
         frequency in kHz
-
         '''
         [m,n,p] = mode_index
         efaxial = self.Axialfreq()*self.fz*1000
         efradial = self.Transfreq()*self.fz*1000
         if ftype==0:
             f_ah = efradial[m]-efradial[n]-efaxial[p]
         else:
             f_ah = efradial[m]+efradial[n]-efaxial[p]
         return f_ah 
     def plot_ah_freq(self,non_zero=True):
         '''
         Plot absolute value of anharmonic coupling freq
-
         Parameters
         ----------
         non_zero: bool 
             default is True, if True, only plot non-zero coefficeints     
-
         Returns
         -------
         None.
-
         '''
         afplot1 = {}; afplot2 = {}
         #compute axial, radial freq
         efaxial = self.Axialfreq()*self.fz*1000
         efradial = self.Transfreq()*self.fz*1000
         for i in range(self.N ):
             for j in range(self.N):
@@ -638,48 +611,44 @@
         '''
         compute the eigenmodes of axial oscillation 
         Returns
         -------
         np array object that represents N by N matrix, each row is an axial eigenmode
         The eigenmode are arranged in an increasing order of eigenvalues, such that the first 
         one correpond to COM mode
-
         '''
         e_val,e_array = np.linalg.eig(self.Amatrix())
         order = np.argsort(e_val)
         return (np.transpose(e_array))[order]
     def Transfreq(self):
         '''
         compute the eigenvalue of transverse eigenmode matrix, multiply by fz to get real frequency [MHz]
         Returns
         -------
         np array object, each index is an eigenvalue for Transverse(Radial) mode [unit of 1]
         The eigenvalues are arranged in an decreasing order, such that the first 
         one correpond to COM mode frequency
-
         '''
         e_val = np.linalg.eig(self.Tmatrix())[0]
         order = np.argsort(e_val)
         e_val = e_val[order][::-1]
         #check if the matrix is positive-definite
         if np.min(e_val) < 0:
             print("Negtive transverse frequency, the system is unstable")
             return np.sqrt(e_val+0j)
         else:
             return np.sqrt(e_val)
     def Transmode(self):
         '''
         compute the eigenmode of transverse oscillation
-
         Returns
         -------
         np array object that represents N by N matrix, each row is an Transverse (Radial) eigenmode
         The eigenmode are arranged in an decreasing order of eigenvalues, such that the first 
         one correpond to COM mode
-
         '''
         e_val, e_array= np.linalg.eig(self.Tmatrix())
         order = np.argsort(e_val)[::-1]
         return np.transpose(e_array)[order]    
     def wmlist(self):
         '''
         compute axial , transverse eigenfrequencies of the system
@@ -728,15 +697,14 @@
         Compute the laser-ion coupling strength between ion i and mode m
         Parameters
         ----------
         i : int
             ion index
         m : int
             eigenmode index
-
         Returns
         -------
         g : float
             [2pi kHz]
         '''
         
         if self.df_laser == 0:
@@ -763,36 +731,33 @@
     def epsilon(self):
         '''
         Compute the anharmonic coefficient epsilon = sqrt(hbar/(2 m fz)/(4l))
         -------
         Returns
         -------
         float unit of 1
-
         '''
         sigma0 = np.sqrt(0.5*h / (MYb171*fr_conv(self.fz,'mhz')))
         return  sigma0 / (4*self.l0())
     def ah_couple(self, mode_index,real_unit=False):
         '''
         Compute the anharmonic coupling strength for index m , n, p
-
         Parameters
         ----------
         mode_index: list of python index [m n p]
         m,n for transverse modes, p for axial mode
         real_unit: bool
             default as False
             if True, compute coefficients in unit of kHz
             if false, compute coefficients in unit of fz
         Returns
         -------
         float, anharmonic coupling strength, [unit 1]
         multiply fz to get coupling strength in Hz
         or real frequency in kHz
-
         '''
         [m,n,p] = mode_index
         tfreq = (self.Transfreq())**2; afreq = (self.Axialfreq())**2
         freq_factor = (tfreq[m]*tfreq[n]*afreq[p])**0.25
         if real_unit:
             ah_coef = self.fz*1000*(-3*self.epsilon()*self.D(m,n,p)/freq_factor)
         else:
```

### Comparing `Qsim_trapped_ions-1.0.3/Qsim/ion_chain/ising/ising_c.py` & `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/ising/ising_c.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.3/Qsim/ion_chain/ising/ising_ps.py` & `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/ising/ising_ps.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.3/Qsim/ion_chain/transfer/anharmonic_transfer - 副本.py` & `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/anharmonic_transfer - 副本.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.3/Qsim/ion_chain/transfer/anharmonic_transfer.py` & `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/anharmonic_transfer.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.3/Qsim/ion_chain/transfer/chaos.py` & `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/chaos.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.3/Qsim/ion_chain/transfer/elec_transfer.py` & `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/elec_transfer.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.3/Qsim/ion_chain/transfer/exci_operators.py` & `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/exci_operators.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.3/Qsim/ion_chain/transfer/exci_transfer.py` & `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/exci_transfer.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.3/Qsim/ion_chain/transfer/multi_core.py` & `Qsim_trapped_ions-1.0.4/Qsim/ion_chain/transfer/multi_core.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.3/Qsim/operator/phonon.py` & `Qsim_trapped_ions-1.0.4/Qsim/operator/phonon.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.3/Qsim/operator/spin.py` & `Qsim_trapped_ions-1.0.4/Qsim/operator/spin.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.3/Qsim_trapped_ions.egg-info/PKG-INFO` & `Qsim_trapped_ions-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: Qsim-trapped-ions
-Version: 1.0.3
+Name: Qsim_trapped_ions
+Version: 1.0.4
 Summary: Numerical simulation of trapped ion quantum dynamics
 Home-page: https://github.com/TrappedIonRice/Open-Quantum-system-simulation
-Author: mjz
+Author: Mingjian Zhu
 Author-email: mz40@rice.edu
 
 # Open-Quantum-system-simulation
 package: ion_chain
 
 dependence pakcage: Qutip
```

### Comparing `Qsim_trapped_ions-1.0.3/Qsim_trapped_ions.egg-info/SOURCES.txt` & `Qsim_trapped_ions-1.0.4/Qsim_trapped_ions.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-README.rst
 setup.py
 Qsim/ion_chain/__init__.py
 Qsim/ion_chain/ion_system.py
 Qsim/ion_chain/eigendiagram/exci_diagram.py
 Qsim/ion_chain/eigendiagram/init__.py
 Qsim/ion_chain/interaction/__init__.py
 Qsim/ion_chain/interaction/pure_spin.py
@@ -21,8 +20,9 @@
 Qsim/operator/__init__.py
 Qsim/operator/phonon.py
 Qsim/operator/spin.py
 Qsim_trapped_ions.egg-info/PKG-INFO
 Qsim_trapped_ions.egg-info/SOURCES.txt
 Qsim_trapped_ions.egg-info/dependency_links.txt
 Qsim_trapped_ions.egg-info/requires.txt
-Qsim_trapped_ions.egg-info/top_level.txt
+Qsim_trapped_ions.egg-info/top_level.txt
+test/test.py
```

### Comparing `Qsim_trapped_ions-1.0.3/setup.py` & `Qsim_trapped_ions-1.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 
 @author: zhumj
 """
 
 from setuptools import setup
 
 def readme_file():
-    with open("C:\\Users\\zhumj\\.ipython\README.rst") as rf:
+    with open(".\\Qsim\\README.rst") as rf:
         return rf.read()
     
 setup(name = 'Qsim_trapped_ions', 
-      version = '1.0.3', 
+      version = '1.0.4', 
       description = 'Numerical simulation of trapped ion quantum dynamics',
       package_dir = {
             'Qsim': 'Qsim',
             'Qsim.ion_chain': 'Qsim/ion_chain',
             'Qsim.operator': 'Qsim/operator',
             'Qsim.ion_chain.eigendiagram': 'Qsim/ion_chain/eigendiagram',
             'Qsim.ion_chain.interaction': 'Qsim/ion_chain/interaction',
             'Qsim.ion_chain.ising': 'Qsim/ion_chain/ising',
             'Qsim.ion_chain.transfer': 'Qsim/ion_chain/transfer',},
       install_requires=[
           'qutip'],
       packages = ['Qsim.ion_chain','Qsim.operator','Qsim.ion_chain.eigendiagram','Qsim.ion_chain.interaction',
                   'Qsim.ion_chain.ising', 'Qsim.ion_chain.transfer',],
-      author = 'mjz',
+      author = 'Mingjian Zhu',
       author_email='mz40@rice.edu',
       long_description = readme_file(),
       url = 'https://github.com/TrappedIonRice/Open-Quantum-system-simulation')
```

