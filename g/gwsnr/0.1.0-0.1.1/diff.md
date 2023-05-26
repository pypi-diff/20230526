# Comparing `tmp/gwsnr-0.1.0.tar.gz` & `tmp/gwsnr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwsnr-0.1.0.tar", last modified: Tue Apr 25 09:35:26 2023, max compression
+gzip compressed data, was "gwsnr-0.1.1.tar", last modified: Fri May 26 14:57:48 2023, max compression
```

## Comparing `gwsnr-0.1.0.tar` & `gwsnr-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-04-25 09:35:26.759885 gwsnr-0.1.0/
--rw-r--r--   0 hemantaph   (501) staff       (20)      210 2023-04-25 09:35:26.759451 gwsnr-0.1.0/PKG-INFO
--rw-r--r--   0 hemantaph   (501) staff       (20)      437 2023-03-08 19:14:30.000000 gwsnr-0.1.0/README.md
-drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-04-25 09:35:26.756717 gwsnr-0.1.0/gwsnr/
--rw-r--r--   0 hemantaph   (501) staff       (20)       26 2023-04-25 06:50:13.000000 gwsnr-0.1.0/gwsnr/__init__.py
--rw-r--r--   0 hemantaph   (501) staff       (20)    54362 2023-04-25 08:46:23.000000 gwsnr-0.1.0/gwsnr/gwsnr.py
--rw-r--r--   0 hemantaph   (501) staff       (20)        0 2023-04-25 06:49:42.000000 gwsnr-0.1.0/gwsnr/pdet.py
-drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-04-25 09:35:26.758943 gwsnr-0.1.0/gwsnr.egg-info/
--rw-r--r--   0 hemantaph   (501) staff       (20)      210 2023-04-25 09:35:26.000000 gwsnr-0.1.0/gwsnr.egg-info/PKG-INFO
--rw-r--r--   0 hemantaph   (501) staff       (20)      209 2023-04-25 09:35:26.000000 gwsnr-0.1.0/gwsnr.egg-info/SOURCES.txt
--rw-r--r--   0 hemantaph   (501) staff       (20)        1 2023-04-25 09:35:26.000000 gwsnr-0.1.0/gwsnr.egg-info/dependency_links.txt
--rw-r--r--   0 hemantaph   (501) staff       (20)       83 2023-04-25 09:35:26.000000 gwsnr-0.1.0/gwsnr.egg-info/requires.txt
--rw-r--r--   0 hemantaph   (501) staff       (20)        6 2023-04-25 09:35:26.000000 gwsnr-0.1.0/gwsnr.egg-info/top_level.txt
--rw-r--r--   0 hemantaph   (501) staff       (20)       38 2023-04-25 09:35:26.759998 gwsnr-0.1.0/setup.cfg
--rw-r--r--   0 hemantaph   (501) staff       (20)      529 2023-04-25 06:43:39.000000 gwsnr-0.1.0/setup.py
+drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-05-26 14:57:48.396352 gwsnr-0.1.1/
+-rw-r--r--   0 hemantaph   (501) staff       (20)      210 2023-05-26 14:57:48.396046 gwsnr-0.1.1/PKG-INFO
+-rw-r--r--   0 hemantaph   (501) staff       (20)      437 2023-03-08 19:14:30.000000 gwsnr-0.1.1/README.md
+drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-05-26 14:57:48.393845 gwsnr-0.1.1/gwsnr/
+-rw-r--r--   0 hemantaph   (501) staff       (20)       26 2023-04-25 06:50:13.000000 gwsnr-0.1.1/gwsnr/__init__.py
+-rw-r--r--   0 hemantaph   (501) staff       (20)    51383 2023-05-26 14:30:24.000000 gwsnr-0.1.1/gwsnr/gwsnr.py
+-rw-r--r--   0 hemantaph   (501) staff       (20)        0 2023-04-25 06:49:42.000000 gwsnr-0.1.1/gwsnr/pdet.py
+drwxr-xr-x   0 hemantaph   (501) staff       (20)        0 2023-05-26 14:57:48.395578 gwsnr-0.1.1/gwsnr.egg-info/
+-rw-r--r--   0 hemantaph   (501) staff       (20)      210 2023-05-26 14:57:48.000000 gwsnr-0.1.1/gwsnr.egg-info/PKG-INFO
+-rw-r--r--   0 hemantaph   (501) staff       (20)      209 2023-05-26 14:57:48.000000 gwsnr-0.1.1/gwsnr.egg-info/SOURCES.txt
+-rw-r--r--   0 hemantaph   (501) staff       (20)        1 2023-05-26 14:57:48.000000 gwsnr-0.1.1/gwsnr.egg-info/dependency_links.txt
+-rw-r--r--   0 hemantaph   (501) staff       (20)       83 2023-05-26 14:57:48.000000 gwsnr-0.1.1/gwsnr.egg-info/requires.txt
+-rw-r--r--   0 hemantaph   (501) staff       (20)        6 2023-05-26 14:57:48.000000 gwsnr-0.1.1/gwsnr.egg-info/top_level.txt
+-rw-r--r--   0 hemantaph   (501) staff       (20)       38 2023-05-26 14:57:48.396422 gwsnr-0.1.1/setup.cfg
+-rw-r--r--   0 hemantaph   (501) staff       (20)      529 2023-05-26 14:56:11.000000 gwsnr-0.1.1/setup.py
```

### Comparing `gwsnr-0.1.0/gwsnr/gwsnr.py` & `gwsnr-0.1.1/gwsnr/gwsnr.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # note: setting mtot_min and mtot_max is important.
 # mtot_min=219. is accordance to minimum_frequency = 20
 # __init__ paramters are important don't to change for a particular analysis
 # they are detector and waveform dependent parameters
 # at f_min==10Hz: mtot_max=439.6 
 import numpy as np
 import bilby
-from pycbc.detector import Detector
+#from pycbc.detector import Detector
 from scipy.stats import norm
 from scipy.interpolate import interp1d
 from gwpy.timeseries import TimeSeries
 from scipy.optimize import fsolve
 from multiprocessing import Pool
 import pycbc.psd
 from tqdm import tqdm
@@ -41,15 +41,15 @@
     ####################################################
     #                                                  #
     #             Class initialization                 #
     #                                                  #
     ####################################################
     def __init__(self, npool=int(4), mtot_min=2., mtot_max=439.6, nsamples_mtot=100, nsamples_mass_ratio=50, \
                  sampling_frequency=4096.,\
-                 waveform_approximant = 'TaylorF2', minimum_frequency = 20., \
+                 waveform_approximant = 'IMRPhenomD', minimum_frequency = 20., \
                  snr_type = 'interpolation', waveform_inspiral_must_be_above_fmin=False, psds=False, psd_file=False):
         
         '''
         Initialized parameters and functions
         snr_half_scaled() : function for finding (f/PSD) integration in the limit [f_min,f_max]
         list_of_detectors :  list of detector initials, e.g. L1 for Livingston
         f_min : minimum frequency for the detector
@@ -87,14 +87,15 @@
         self.sampling_frequency   = sampling_frequency
         self.waveform_approximant = waveform_approximant
         self.f_min                = minimum_frequency
         self.waveform_type        = self.waveform_classifier(waveform_approximant)
         self.snr_type             = snr_type
         self.waveform_inspiral_must_be_above_fmin = waveform_inspiral_must_be_above_fmin
         self.psd_file             = psd_file
+        
         # pre-initialized half scaled snr with search sort
         # self.halfSNR values are initialized
         #print('waveform_type=',self.waveform_type)
         
         
         if psds==False:
             print("psds not given. Choosing bilby's default psds")
@@ -106,15 +107,17 @@
             self.psds = psds
             self.list_of_detectors    = list(psds.keys())
         else:
             self.psds_default = False
             self.list_of_detectors    = list(psds.keys())
             print("given psds: ",psds)
             self.psds = psds
-            
+        
+        # for Fp, Fc calculation
+        self.ifos = ifos = bilby.gw.detector.InterferometerList(self.list_of_detectors)
             
         if snr_type == 'interpolation':
             
             # creating interpolator_pickle directory to store scipy inter
             path = './interpolator_pickle'
             if not os.path.exists(path):
                 os.makedirs(path)
@@ -285,59 +288,53 @@
                                         np.array([ra]).reshape(-1)*np.ones(size), \
                                         np.array([dec]).reshape(-1)*np.ones(size)
         
         Mc = ( (mass_1*mass_2)**(3/5) )/( (mass_1+mass_2)**(1/5) )
         mtot = mass_1+mass_2
         luminosity_distance = luminosity_distance
         
-        '''
-        # dealing with mtot array
-        # mtot > mtot_max will be have snr = 0.
-        snr_half_scaled = np.zeros(size) # for mtot > mtot_max, set zero value will not change later
-        idx2 = np.array(np.where(self.mtot_max>=mtot)).reshape(-1).tolist() # record index with mtot values less than mtot_max
-        # getting simple snr_half_scaled values for interpolation
-        halfSNR_interpolator = self.halfSNR
-        '''
         snr_half_scaled = np.zeros(size)
-        approx_duration = self.findchirp_chirptime(mass_1, mass_2, self.f_min)
         # select only those that have inspiral part above f_min
         if self.waveform_inspiral_must_be_above_fmin==True:
+            approx_duration = self.findchirp_chirptime(mass_1, mass_2, self.f_min)
             idx2 = approx_duration>0.
         else:
             idx2 = np.full(size,True)
             
         idx2 = idx2&(mtot>=self.mtot_min)&(mtot<=self.mtot_max)
         
         # getting simple snr_half_scaled values for interpolation
         halfSNR_interpolator = self.halfSNR
         
         A1 = Mc**(5./6.)
-        ci_2 = np.cos(iota)**2
-        ci_param = ((1+np.cos(iota)**2)/2)**2
+        ci_2 = np.cos(theta_jn)**2
+        ci_param = ((1+np.cos(theta_jn)**2)/2)**2
         detectors = self.list_of_detectors
         
         opt_snr = {'opt_snr_net': 0}
 
         idx_ratio = np.searchsorted(self.ratio, mass_2/mass_1)
         idx_tracker = np.arange(size)
         idx_tracker = idx_tracker[idx2]
         #self.idx_ratio = idx_ratio 
         # loop wrt detectors
-        i = 0
-        for det in detectors:
+        for i in range(len(detectors)):
+            det = detectors[i]
             # calculation of snr_half_scaled for particular detector at the required mtot
             for j in idx_tracker:
                 snr_half_scaled[j] = halfSNR_interpolator[idx_ratio[j],i](mtot[j]) # i is iterator wrt detectors
-
-            Fp, Fc = Detector(det).antenna_pattern(ra, dec, psi, geocent_time)
-            Deff1 = luminosity_distance/np.sqrt( Fp**2*ci_param + Fc**2*ci_2 )
+            
+            Deff1 = np.zeros(size)
+            for k in range(len(ra)):
+                Fp = self.ifos[i].antenna_response(ra[k], dec[k], geocent_time[k], psi[k], 'plus')
+                Fc = self.ifos[i].antenna_response(ra[k], dec[k], geocent_time[k], psi[k], 'cross')
+                Deff1[k] = luminosity_distance[k]/np.sqrt( Fp**2*ci_param[k] + Fc**2*ci_2[k] )
 
             opt_snr[det] = (A1/Deff1)*snr_half_scaled
             opt_snr['opt_snr_net'] += opt_snr[det]**2
-            i+=1
 
         opt_snr['opt_snr_net'] = np.sqrt(opt_snr['opt_snr_net'])
         self.stored_snrs = opt_snr # this stored snrs can be use for Pdet calculation
         
         # saving as json file
         if jsonFile:
             parameters_dict = {'mass_1':mass_1, 'mass_2':mass_2, 'luminosity_distance':luminosity_distance, 'theta_jn':theta_jn, 'psi':psi, 'phase':phase, 'ra':ra, 'dec':dec, 'geocent_time':geocent_time,}
@@ -354,69 +351,14 @@
         return( opt_snr )
     
     ####################################################
     #                                                  #
     #   half_snr vs mtot table for interpolation       #
     #                                                  #
     ####################################################
-    def snr_correction_func(self):
-        '''
-        '''
-        mtot_min = self.mtot_min
-        mtot_max = self.mtot_max
-        nsamples = self.nsamples
-        detectors = self.list_of_detectors
-        f_min = self.f_min
-
-        # geocent_time cannot be array here
-        # this geocent_time is only to get halfScaledSNR
-        geocent_time_ = 1246527224.169434 # random time from O3
-    
-        iota_, ra_, dec_, psi_, phase_ = 0.,0.,0.,0.,0.
-        luminosity_distance_ = 100.
-        
-        ratio = self.ratio
-        correction_ = np.zeros((len(ratio),len(detectors)),dtype=object)
-        i = 0
-        for q in tqdm(ratio, desc="interpolation for extra snr correction", total=len(ratio), ncols= 100):
-            
-            mass_ratio = q
-            if self.waveform_inspiral_must_be_above_fmin==True:
-                func = lambda x: self.findchirp_chirptime(x/(1+mass_ratio),x/(1+mass_ratio)*mass_ratio, f_min)
-                mtot_max = fsolve(func, 150)[0] # to make sure that chirptime is not negative, TaylorF2 might need this
-            
-            mtot_table = np.sort(np.random.uniform(mtot_min,  mtot_max, nsamples-2)).tolist()
-            mtot_table = np.array([mtot_min]+mtot_table+[mtot_max])
-            mass_1_ = np.round(mtot_table/(1+q),5)
-            mass_1_[0] = mass_1_[0]+0.00001
-            mass_1_[-1] = mass_1_[-1]-0.00001
-            mass_2_ = np.round(mass_1_*q,5)
-            ######## calling bilby_snr ########
-            bilby_snr = self.compute_bilby_snr_(mass_1=mass_1_, mass_2=mass_2_, luminosity_distance=luminosity_distance_, \
-                                                    theta_jn=iota_, psi=psi_, ra=ra_, dec=dec_,verbose=False, jsonFile=False)  
-            
-            interpolation_snr = self.snr_with_interpolation(mass_1=mass_1_, mass_2=mass_2_, luminosity_distance=luminosity_distance_, \
-                                                iota=iota_, psi=psi_, ra=ra_, dec=dec_, jsonFile=False)
-            
-            ######## filling in interpolation table for different detectors ########
-            j = 0
-            for det in detectors:
-                correction_[i,j] = interp1d( mtot_table, abs(interpolation_snr[det]-bilby_snr[det]), kind = 'cubic')
-                j+=1
-            i+=1
-        self.snr_correction = correction_
-        
-        return None
-    
-    
-    ####################################################
-    #                                                  #
-    #   half_snr vs mtot table for interpolation       #
-    #                                                  #
-    ####################################################
     def __init_halfScaled(self):
         '''
         Function for finding (f/PSD) integration in the limit [f_min,f_max]
         f_min is already initialized
         f_max is taken as 'last stable orbit frequency' is a function of mtot
         __init_halfScaled(self) will initialize the interpolator (scipy cubic spline) as self.halfSNR
         -----------------
@@ -440,30 +382,14 @@
         except ValueError:
             print('Error: mass too low')
         
         C = 299792458.
         G = 6.67408*1e-11
         Mo = 1.989*1e30
         f_min = self.f_min
-        '''
-        # mtot_max_propose from f_min
-        mtot_max_propose = (C**3)/( G*Mo*f_min*np.pi*6**(3/2) )
-        
-        if mtot_max_propose<mtot_max:
-            warnings.warn\
-                (f'\n Mtot_max={mtot_max} given here is smaller than Mtot_max set by \
-                f_min={f_min}, \n new Mtot_max={mtot_max_propose}. \n If you want higher Mtot_max, set f_min lower \
-                (e.g. f_min=10Hz, but not lesser than 10Hz)')
-            mtot_max = mtot_max_propose
-            self.mtot_max = mtot_max
-        
-        #mtot_table = np.sort(mtot_min+mtot_max-np.geomspace(mtot_min,  mtot_max, nsamples))
-        #mtot_table = np.geomspace(mtot_min,  mtot_max, nsamples)
-        mtot_table = np.linspace(mtot_min,  mtot_max, nsamples)
-        '''
 
         # geocent_time cannot be array here
         # this geocent_time is only to get halfScaledSNR
         geocent_time_ = 1246527224.169434 # random time from O3
     
         iota_, ra_, dec_, psi_, phase_ = 0.,0.,0.,0.,0.
         luminosity_distance_ = 100.
@@ -492,22 +418,22 @@
             {'opt_snr_net': array([156.53268655, 243.00092419, 292.10396943]),
              'L1': array([132.08275995, 205.04492349, 246.47822334]),
              'H1': array([ 84.00372897, 130.40716432, 156.75845871])}
             '''
 
             A2 = mchirp**(5./6.)
             ######## filling in interpolation table for different detectors ########
-            j = 0
-            for det in detectors:
-                Fp, Fc = Detector(det).antenna_pattern(ra_, dec_, psi_, geocent_time_)
+            for j in range(len(detectors)):
+                Fp = self.ifos[j].antenna_response(ra_, dec_, geocent_time_, psi_, 'plus')
+                Fc = self.ifos[j].antenna_response(ra_, dec_, geocent_time_, psi_, 'cross')
                 Deff2 = luminosity_distance_/np.sqrt(Fp**2*((1+np.cos(iota_)**2)/2)**2+Fc**2*np.cos(iota_)**2 )
 
-                snrHalf_[i,j] = interp1d( mtot_table, (Deff2/A2)*opt_snr_unscaled[det], kind = 'cubic')
-                j+=1
-            i+=1
+                snrHalf_[i,j] = interp1d( mtot_table, (Deff2/A2)*opt_snr_unscaled[detectors[j]], kind = 'cubic')
+                
+            i+=1 # iterator over mass_ratio
             
         # 2D array size: n_detectors X nsamples np.concatenate((a, b), axis=0)
         # snrHalf_det['mtot'] = mtot_table
         #print(snrHalf_det)
         self.halfSNR = snrHalf_
         
         # save halfSNR interpolation values
@@ -829,30 +755,32 @@
         f_array = waveform_generator.frequency_array
         idx = (f_array>=f_min)&(f_array<=f_max)
         h_plus  = polas['plus'][idx]
         h_cross = polas['cross'][idx]
             
         SNRs_list = []
         NetSNR      = 0.
+        # detectors = self.list_of_detectors
         list_of_detectors = params[15:].tolist()
         psds_arrays = params[14]
-        for ifo in list_of_detectors:
+        for i in range(len(list_of_detectors)):
             # need to compute the inner product for
-            p_array = psds_arrays[ifo].get_power_spectral_density_array(f_array)[idx]
+            p_array = psds_arrays[list_of_detectors[i]].get_power_spectral_density_array(f_array)[idx]
             idx2 = (p_array!=0.) & (p_array!=np.inf)
             hp_inner_hp = bilby.gw.utils.noise_weighted_inner_product(h_plus[idx2],
                                                                            h_plus[idx2],
                                                                            p_array[idx2],
                                                                            waveform_generator.duration)
             hc_inner_hc = bilby.gw.utils.noise_weighted_inner_product(h_cross[idx2],
                                                                            h_cross[idx2],
                                                                            p_array[idx2],
                                                                            waveform_generator.duration)
             # make an ifo object to get the antenna pattern
-            Fp, Fc = Detector(ifo).antenna_pattern(parameters['ra'],parameters['dec'],parameters['psi'],parameters['geocent_time'])
+            Fp = self.ifos[i].antenna_response(parameters['ra'],parameters['dec'], parameters['geocent_time'], parameters['psi'], 'plus')
+            Fc = self.ifos[i].antenna_response(parameters['ra'],parameters['dec'], parameters['geocent_time'], parameters['psi'], 'cross')
 
             snrs_sq = abs((Fp**2)*hp_inner_hp + (Fc**2)*hc_inner_hc)
 
             SNRs_list.append(np.sqrt(snrs_sq))
             NetSNR += snrs_sq
 
         SNRs_list.append(np.sqrt(NetSNR))
@@ -901,28 +829,29 @@
                                                         waveform_arguments = waveform_arguments)
         polas = waveform_generator.frequency_domain_strain(parameters = parameters)
 
         SNRs_list = []
         NetSNR      = 0.
         list_of_detectors = params[15:].tolist()
         psds_arrays = params[14]
-        for ifo in list_of_detectors:
+        for i in range(len(list_of_detectors)):
             # need to compute the inner product for
-            p_array = psds_arrays[ifo].get_power_spectral_density_array(waveform_generator.frequency_array)
+            p_array = psds_arrays[list_of_detectors[i]].get_power_spectral_density_array(waveform_generator.frequency_array)
             idx2 = (p_array!=0.) & (p_array!=np.inf)
             hp_inner_hp = bilby.gw.utils.noise_weighted_inner_product(polas['plus'][idx2],
                                                                            polas['plus'][idx2],
                                                                            p_array[idx2],
                                                                            waveform_generator.duration)
             hc_inner_hc = bilby.gw.utils.noise_weighted_inner_product(polas['cross'][idx2],
                                                                            polas['cross'][idx2],
                                                                            p_array[idx2],
                                                                            waveform_generator.duration)
             # make an ifo object to get the antenna pattern
-            Fp, Fc = Detector(ifo).antenna_pattern(parameters['ra'],parameters['dec'],parameters['psi'],parameters['geocent_time'])
+            Fp = self.ifos[i].antenna_response(parameters['ra'],parameters['dec'], parameters['geocent_time'], parameters['psi'], 'plus')
+            Fc = self.ifos[i].antenna_response(parameters['ra'],parameters['dec'], parameters['geocent_time'], parameters['psi'], 'cross')
 
             snrs_sq = abs((Fp**2)*hp_inner_hp + (Fc**2)*hc_inner_hc)
 
             SNRs_list.append(np.sqrt(snrs_sq))
             NetSNR += snrs_sq
 
         SNRs_list.append(np.sqrt(NetSNR))
```

### Comparing `gwsnr-0.1.0/setup.py` & `gwsnr-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 setup(name='gwsnr',
-      version='0.1.0',
+      version='0.1.1',
       description='Fast SNR interpolator',
       author='Hemantakumar, Otto',
       license="MIT",
       author_email='hemantaphurailatpam@gmail.com',
       url='https://github.com/hemantaph/gwsnr',
       packages=find_packages(),
       install_requires=[
```

