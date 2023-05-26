# Comparing `tmp/astromulti-1.0.3.tar.gz` & `tmp/astromulti-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astromulti-1.0.3.tar", last modified: Mon Jan  9 11:07:07 2023, max compression
+gzip compressed data, was "astromulti-1.0.4.tar", last modified: Fri May 26 12:22:06 2023, max compression
```

## Comparing `astromulti-1.0.3.tar` & `astromulti-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ro        (1000) ro        (1000)        0 2023-01-09 11:07:07.353984 astromulti-1.0.3/
--rw-r--r--   0 ro        (1000) ro        (1000)     1231 2022-09-29 04:01:38.000000 astromulti-1.0.3/LICENSE
--rw-rw-r--   0 ro        (1000) ro        (1000)     1747 2023-01-09 11:07:07.353984 astromulti-1.0.3/PKG-INFO
--rw-r--r--   0 ro        (1000) ro        (1000)     1297 2023-01-09 11:05:23.000000 astromulti-1.0.3/README.md
--rw-r--r--   0 ro        (1000) ro        (1000)      677 2023-01-09 11:04:29.000000 astromulti-1.0.3/pyproject.toml
--rw-rw-r--   0 ro        (1000) ro        (1000)       38 2023-01-09 11:07:07.353984 astromulti-1.0.3/setup.cfg
-drwxrwxr-x   0 ro        (1000) ro        (1000)        0 2023-01-09 11:07:07.353984 astromulti-1.0.3/src/
-drwxrwxr-x   0 ro        (1000) ro        (1000)        0 2023-01-09 11:07:07.353984 astromulti-1.0.3/src/astromulti/
--rw-r--r--   0 ro        (1000) ro        (1000)        2 2022-09-29 04:01:37.000000 astromulti-1.0.3/src/astromulti/__init__.py
--rw-r--r--   0 ro        (1000) ro        (1000)    37618 2022-12-10 09:04:36.000000 astromulti-1.0.3/src/astromulti/fits_actions.py
--rw-r--r--   0 ro        (1000) ro        (1000)     7811 2022-09-29 04:01:37.000000 astromulti-1.0.3/src/astromulti/linear_fitting.py
--rw-r--r--   0 ro        (1000) ro        (1000)     2437 2022-09-29 04:01:37.000000 astromulti-1.0.3/src/astromulti/new_colormap.py
--rw-r--r--   0 ro        (1000) ro        (1000)     4744 2022-09-29 04:01:37.000000 astromulti-1.0.3/src/astromulti/region_meta.py
--rw-r--r--   0 ro        (1000) ro        (1000)     1630 2022-09-29 04:01:37.000000 astromulti-1.0.3/src/astromulti/simple_funcs.py
-drwxrwxr-x   0 ro        (1000) ro        (1000)        0 2023-01-09 11:07:07.353984 astromulti-1.0.3/src/astromulti.egg-info/
--rw-rw-r--   0 ro        (1000) ro        (1000)     1747 2023-01-09 11:07:07.000000 astromulti-1.0.3/src/astromulti.egg-info/PKG-INFO
--rw-rw-r--   0 ro        (1000) ro        (1000)      367 2023-01-09 11:07:07.000000 astromulti-1.0.3/src/astromulti.egg-info/SOURCES.txt
--rw-rw-r--   0 ro        (1000) ro        (1000)        1 2023-01-09 11:07:07.000000 astromulti-1.0.3/src/astromulti.egg-info/dependency_links.txt
--rw-rw-r--   0 ro        (1000) ro        (1000)       11 2023-01-09 11:07:07.000000 astromulti-1.0.3/src/astromulti.egg-info/top_level.txt
+drwxrwxr-x   0 ro        (1000) ro        (1000)        0 2023-05-26 12:22:06.476145 astromulti-1.0.4/
+-rw-r--r--   0 ro        (1000) ro        (1000)     1231 2022-09-29 04:01:38.000000 astromulti-1.0.4/LICENSE
+-rw-rw-r--   0 ro        (1000) ro        (1000)     1747 2023-05-26 12:22:06.476145 astromulti-1.0.4/PKG-INFO
+-rw-r--r--   0 ro        (1000) ro        (1000)     1297 2023-01-09 11:05:23.000000 astromulti-1.0.4/README.md
+-rw-r--r--   0 ro        (1000) ro        (1000)      677 2023-05-26 11:53:50.000000 astromulti-1.0.4/pyproject.toml
+-rw-rw-r--   0 ro        (1000) ro        (1000)       38 2023-05-26 12:22:06.476145 astromulti-1.0.4/setup.cfg
+drwxrwxr-x   0 ro        (1000) ro        (1000)        0 2023-05-26 12:22:06.476145 astromulti-1.0.4/src/
+drwxrwxr-x   0 ro        (1000) ro        (1000)        0 2023-05-26 12:22:06.476145 astromulti-1.0.4/src/astromulti/
+-rw-r--r--   0 ro        (1000) ro        (1000)        2 2022-09-29 04:01:37.000000 astromulti-1.0.4/src/astromulti/__init__.py
+-rw-r--r--   0 ro        (1000) ro        (1000)    34041 2023-05-26 12:18:33.000000 astromulti-1.0.4/src/astromulti/fits_actions.py
+-rw-r--r--   0 ro        (1000) ro        (1000)     7811 2022-09-29 04:01:37.000000 astromulti-1.0.4/src/astromulti/linear_fitting.py
+-rw-r--r--   0 ro        (1000) ro        (1000)     2441 2023-05-26 12:18:43.000000 astromulti-1.0.4/src/astromulti/new_colormap.py
+-rw-r--r--   0 ro        (1000) ro        (1000)     5023 2023-05-26 12:18:55.000000 astromulti-1.0.4/src/astromulti/region_meta.py
+-rw-r--r--   0 ro        (1000) ro        (1000)     1630 2022-09-29 04:01:37.000000 astromulti-1.0.4/src/astromulti/simple_funcs.py
+drwxrwxr-x   0 ro        (1000) ro        (1000)        0 2023-05-26 12:22:06.476145 astromulti-1.0.4/src/astromulti.egg-info/
+-rw-rw-r--   0 ro        (1000) ro        (1000)     1747 2023-05-26 12:22:06.000000 astromulti-1.0.4/src/astromulti.egg-info/PKG-INFO
+-rw-rw-r--   0 ro        (1000) ro        (1000)      367 2023-05-26 12:22:06.000000 astromulti-1.0.4/src/astromulti.egg-info/SOURCES.txt
+-rw-rw-r--   0 ro        (1000) ro        (1000)        1 2023-05-26 12:22:06.000000 astromulti-1.0.4/src/astromulti.egg-info/dependency_links.txt
+-rw-rw-r--   0 ro        (1000) ro        (1000)       11 2023-05-26 12:22:06.000000 astromulti-1.0.4/src/astromulti.egg-info/top_level.txt
```

### Comparing `astromulti-1.0.3/LICENSE` & `astromulti-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `astromulti-1.0.3/PKG-INFO` & `astromulti-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromulti
-Version: 1.0.3
+Version: 1.0.4
 Summary: A set of functions for analysis of astronomical images
 Author-email: Rohit D <rohitd@proton.me>
 Project-URL: Homepage, https://gitlab.com/drohi/astromulti
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `astromulti-1.0.3/README.md` & `astromulti-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `astromulti-1.0.3/pyproject.toml` & `astromulti-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = [
     "setuptools>=42",
     "regions>=0.5",
     "numpy>=1.18",
-    "astropy>=5.0.1",
+    "astropy>=5.2.2",
     "scipy>=1.5",
     "matplotlib>=3.3",
     "colorspacious>=1.1",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "astromulti"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Rohit D", email="rohitd@proton.me" },
 ]
 description = "A set of functions for analysis of astronomical images"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `astromulti-1.0.3/src/astromulti/fits_actions.py` & `astromulti-1.0.4/src/astromulti/fits_actions.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from astropy.wcs import WCS
 from astropy.nddata import Cutout2D
 from astropy.modeling import models, fitting
 from astropy.convolution import convolve, convolve_fft, Gaussian2DKernel
 from astropy.coordinates import SkyCoord
 from regions import CircleSkyRegion
 
-from .region_meta import get_extent, get_center, rot_PolySkyReg
-from .simple_funcs import s_clip, ask_user, FWHM_to_SD, dimless
-from .linear_fitting import plane_fit
+from region_meta import get_extent, get_center, rot_PolySkyReg
+from simple_funcs import s_clip, ask_user, FWHM_to_SD, dimless
+from linear_fitting import plane_fit
 
 
 def remove_axes_34(infits,outfits):
     # remove degenerate axes if present
     data, hdr = fits.getdata(infits,0,header=True)
     hdr['NAXIS'] = 2
     for cardname in ['NAXIS3','CRVAL3','CTYPE3','CDELT3','CRPIX3','CROTA3','NAXIS4','CRVAL4','CTYPE4','CDELT4','CRPIX4','CROTA4']:
@@ -172,20 +172,20 @@
     targetunit  = targetunit.lower()
 
     if imageunit==targetunit:
         print("Input is already in target units, so, directly writing to output.")
         fits.writeto( outfits,indata,hdr,overwrite=overwr )
         return
 
-    if 'milli' in imageunit or (imageunit=='m'+targetunit):
+    if 'milli' in imageunit.lower():
         indata = indata/1e3
-        newimageunit = imageunit.replace("milli","").replace("m","",1)
-    elif 'micro' in imageunit or (imageunit=='u'+targetunit):
+        newimageunit = imageunit.lower().replace("milli","")
+    elif 'micro' in imageunit.lower():
         indata = indata/1e6
-        newimageunit = imageunit.replace("micro","").replace("u","",1)
+        newimageunit = imageunit.lower().replace("micro","")
     else:
         newimageunit = imageunit
     if newimageunit==targetunit or ("k" in newimageunit and targetunit=="k"):
         print("Only a factor micro/milli different, no T-S conversion needed.")
         hdr['BUNIT'] = targetunit
         fits.writeto( outfits,indata,hdr,overwrite=overwr )
         return
@@ -204,114 +204,77 @@
                 freq = hdr['FREQUE']
                 print("Using frequency info from fits header.")
             except:
                 raise RuntimeError('freq was not given; input fits also has no FREQUE in it!')
         TbyS = ((1*u.Jy/(np.pi*(beamsz*u.degree)**2/4/np.log(2))).to(u.K, equivalencies=u.brightness_temperature(freq*u.Hz))).value
         print('Calculated the following conversion factor: '+str(TbyS))
 
-    if (newimageunit=='k' or newimageunit=='k tb') and targetunit=="jy/beam":
+    if (newimageunit=='k' or newimageunit=='k tb') and targetunit.lower()=="jy/beam":
         hdr['BUNIT'] = 'Jy/beam'
         fits.writeto( outfits,indata/TbyS,hdr,overwrite=overwr )
         return
-    if newimageunit=="jy/beam" and targetunit=='k':
+    if newimageunit.lower()=="jy/beam" and targetunit=='k':
         hdr['BUNIT'] = 'K'
         fits.writeto( outfits,indata*TbyS,hdr,overwrite=overwr )
         return
 
     # if the code reached here, it means something did not work
     print("The image unit is: "+imageunit)
     print("The given target unit is: "+targetunit)
     print("Target units must be only 'Jy/beam' or 'K'")
     raise RuntimeError("Something wrong with the units.")
 
 
 def regioncut( fitsfile, ds9reg=None, units=True ):
     '''
     Extracts data from a single fits file and also gives its units.
-    The data is returned in the same shape as input, except the coordinate axes of course.
+    Input must be only 2D (only coordinates) or 3D (+velocity/frequency).
+    Output also corresponds to the input.
         Along the coordinates, it takes a 2D shape rather than the mask shape.
         Values outside the mask are converted to NaN.
     '''
 
     # data and details from the fits files
     im_I1, h1 = fits.getdata(fitsfile,0,header=True)
     wcshdr1   = WCS(h1)
+    if len(np.shape(im_I1))>3:
+        raise RuntimeError('Input FITS file must have only 2 or 3 dimensions!')
 
-    # get axis indices of GLON/RA and GLAT/DEC, and the other axes
-    # _4wcs is for popping axes; _4arr is for array operations
+    # get velcoty axis index
     wcs_axis_names = wcshdr1.axis_type_names
-    for axisname in wcs_axis_names:
-        if 'glon' in axisname.lower() or 'ra' in axisname.lower():
-            l_axis_4wcs = [ yy for yy in range(len(wcs_axis_names)) if wcs_axis_names[yy]==axisname ][0]
-            l_axis_4arr = len(np.shape(im_I1)) - l_axis_4wcs - 1
-        if 'glat' in axisname.lower() or 'dec' in axisname.lower():
-            b_axis_4wcs = [ yy for yy in range(len(wcs_axis_names)) if wcs_axis_names[yy]==axisname ][0]
-            b_axis_4arr = len(np.shape(im_I1)) - b_axis_4wcs - 1
-    o_axes = [ kk for kk in range(len(np.shape(im_I1))) if kk not in [l_axis_4arr,b_axis_4arr] ]
-
-    # if there are planes other than l and b
-    if o_axes!=[]:
-        # we will build a dictionary of all the planes,
-        #   with keys corresponding to indices (no l,b indices of course)
-        # example:
-        #   [l,b]=[2,3]  &  o_axes=[0,1,4]  &  key=(d,e,f)
-        #   =>  we must access image with (d,e,:,:,f)
-        dict_full  = {}                                                         # this dictionary will contain the full data (not cropped yet)
-        mykeys_arr = [ np.arange(np.shape(im_I1)[oo]) for oo in o_axes ]        # a list of arrays, each array has the index number that will be iterated over
-        mykeys_fin = [ aa for aa in itrt.product(*mykeys_arr) ]                 # all the required keys
-        for key in mykeys_fin:                                                  # iterating over each key
-            arrayslicer = [ slice(None) ] * len(np.shape(im_I1))                # we'll use this to slice the cube (start with :,:,:,... )
-            for eachaxis in range(len(np.shape(im_I1))):                        # iterate over each axis
-                if eachaxis not in [l_axis_4arr,b_axis_4arr]:                   # if this axis is either l or b, we don't want to change slice(None)
-                    keyidx = [ oo for oo in o_axes if oo==eachaxis ][0]         # the index (in o_axes) that corresponds to the current axis
-                    arrayslicer[eachaxis] = key[keyidx]                         # finally prepare the slicer
-            dict_full[key] = im_I1[tuple(arrayslicer)]                          # slice the cube and save it in dict_full
+    namesjoined = ''.join(wcs_axis_names).lower()
+    if len(np.shape(im_I1))==3:
+        if 'glon' in namesjoined or 'glat' in namesjoined:
+            velaxis = [ axname for axname in wcs_axis_names if 'glon' not in axname.lower() and 'glat' not in axname.lower() ]
+        if 'dec' in namesjoined:
+            velaxis = [ axname for axname in wcs_axis_names if 'ra'!=axname.lower() and 'dec'!=axname.lower() ]
+        velaxis = [ idx for idx in range(len(wcs_axis_names)) if wcs_axis_names[idx]==velaxis[0] ][0]
+    else:
+        velaxis = None
+
+    # if there's a velocity/frequency axis
+    if velaxis is not None:
         # remember that all planes will have the same WCS, same shape
+        # Pop out the velocity axis in the WCS first and get the mask to apply
         new_wcs = dcp(wcshdr1)                                                  # make a deepcopy before modifying
-        # make a list of unnecessary axes and sort them in reverse (for popping correctly)
-        unnec_axes = [ idx for idx in range(wcshdr1.naxis) if idx!=l_axis_4wcs and idx!=b_axis_4wcs ]
-        unnec_axes = np.sort(unnec_axes)[::-1]
-        for axis2rem in unnec_axes:                                             # drop unnecessary axes
-            new_wcs = new_wcs.dropaxis(axis2rem)
-        # so we have corrected the WCS by dropping the unnecessary axes.
-        # now we will create a new dictionary, this time it will contain cropped data.
-        dict_crpd = {}
+        new_wcs = new_wcs.dropaxis(velaxis)                                     # remove velocity axis
         msk1 = ds9reg.to_pixel(new_wcs).to_mask()                               # mask for the 2D image plane
-        for key in mykeys_fin:                                                  # iterating over each key (just reusing the same old keys)
-            croppeddata = msk1.multiply(dict_full[key],fill_value=np.nan)       # values of 'I' pixels inside the bounding box
-            dict_crpd[key] = np.array( croppeddata )                            # save in the dictionary as an array
-            if (dict_crpd[key]==None).all() == True:                            # raise error if object mask can't be prepared
-                print("Something went wrong at this key: "+str(key))
-                raise RuntimeError('Mask cannot be prepared!')
-                return
-        # OK so we have the cutout data in a dictionary with appropriate keys
-        # now we should arrange it back in original shape
-        fin_shape = np.array(np.shape(im_I1))                                   # first start with original shape
-        new_l_idx = int(l_axis_4wcs<b_axis_4wcs)                                # (l,b) = (0,1) or (1,0) ?
-        new_b_idx = int(l_axis_4wcs>b_axis_4wcs)
-        fin_shape[l_axis_4arr] = np.shape(dict_crpd[key])[new_l_idx]            # put correct value of length along 'l'
-        fin_shape[b_axis_4arr] = np.shape(dict_crpd[key])[new_b_idx]            # put correct value of length along 'b'
-        finaldata = np.zeros(fin_shape) + np.nan                                # initialize the data array to be returned
-        # use arrayslicer part from above
-        for key in mykeys_fin:                                                  # iterating over each key
-            arrayslicer = [ slice(None) ] * len(np.shape(im_I1))                # we'll use this to slice the cube (start with :,:,:,... )
-            for eachaxis in range(len(fin_shape)):                              # iterate over each axis
-                if eachaxis not in [l_axis_4arr,b_axis_4arr]:                   # if this axis is either l or b, we don't want to change slice(None)
-                    keyidx = [ oo for oo in o_axes if oo==eachaxis ][0]         # the index (in o_axes) that corresponds to the current axis
-                    arrayslicer[eachaxis] = key[keyidx]                         # finally prepare the slicer
-            finaldata[tuple(arrayslicer)] = dict_crpd[key]                      # save the data from dictionary to the final array
-        I_vals1 = finaldata
-
-    # if there are no axes other than l and b
-    if o_axes==[]:
+        finaldatalist = []                                                      # initialize a list for the final data
+        for idx in range(wcshdr1.spectral.pixel_shape[0]):                      # iterate over each velocity channel
+            croppeddata = msk1.multiply(im_I1[idx],fill_value=np.nan)           # values of 'I' pixels inside the bounding box
+            finaldatalist.append(croppeddata)
+        I_vals1 = np.dstack(finaldatalist)                                      # convert list to 3D array
+    else:
         msk1    = ds9reg.to_pixel(wcshdr1).to_mask()                            # mask for actual data
         I_vals1 = np.array( msk1.multiply(im_I1,fill_value=np.nan) )            # values of 'I' pixels inside the bounding box
-        if (I_vals1==None).all() == True:                                       # skip if object mask can't be prepared
-            raise RuntimeError('Mask cannot be prepared!')
-            return
+
+    # rasie error if no values can be extracted
+    if (I_vals1==None).all() == True:
+        raise RuntimeError('Mask cannot be prepared!')
+        return
 
     # return according to units
     if units==True:
         try:
             imageuni1 = h1['BUNIT']
             return I_vals1,imageuni1
         except:
@@ -450,17 +413,15 @@
         mask0      = (I_vals1>maskval1) * (I_vals2>maskval2)                # use only pixels that are over the threshold in both images
         I_vals1    = I_vals1[mask0]
         I_vals2    = I_vals2[mask0]
 
     return I_vals1,I_vals2,imageuni2
 
 
-def measure_FD( fitsfile, ds9reg=None,
-                noise='auto', noisereg=None, noiseval=None, s2n=0.0, cal_error=0.1,
-                tpds9reg=None, bgboxsize=None, bgregrotate=15*u.degree ):
+def measure_FD( fitsfile, ds9reg=None, noise='auto', noisereg=None, noiseval=None, s2n=0.0, cal_error=0.1, tpds9reg=None, bgboxsize=None, bgregrotate=15*u.degree ):
     '''
     Measures the flux density (Jy) of an extended object.
     BUNIT in the header must be only jy/beam or K or a factor of it.
     If noise=='semi', noise value will be calculated from the values inside 'noisereg'.
     If noise=='auto', noise value will be calculated from the values inside a large surrounding region.
     If noise=='manual', noiseval will be used.
     Values below s2n will be masked.
@@ -481,14 +442,19 @@
 
     # header info fixes
     try:
         _ = hdr['CDELT1']
     except:
         hdr['CDELT1'] = hdr['CD1_1']
         hdr['CDELT2'] = hdr['CD2_2']
+    try:
+        _ = hdr['BMAJ']
+    except:
+        hdr['BMAJ'] = hdr['RESOL1']
+        hdr['BMIN'] = hdr['RESOL2']
 
     # region for noise estimation
     if noise=='auto':
         noisereg = CircleSkyRegion( get_center(ds9reg), radius=get_extent(ds9reg) )
 
     # some required info
     BAinSqDeg = np.pi * hdr['BMAJ'] * hdr['BMIN'] / ( 4*np.log(2) )             # beam area; square degree
@@ -583,28 +549,37 @@
 
 def smooth_fits( inimage, outimage, beamsize, target, overwr=True ):
     '''
     Given an input fits file and the gaussian beam FWHM,
       the output image will be the result of convolution.
     Currently can only handle circular Gaussian beams (BMIN=BMAJ).
     'beamsize' must be in whatever units the input image BMAJ/BMIN are!
+    If target==True: 'beamsize' will be the final beam.
+    If target==False: image is convolved WITH 'beamsize'.
     '''
     data0, hdr = fits.getdata(inimage,0,header=True)
     if len(np.shape(data0))>2:
         print("Removing degenerate axes before smoothing")
     while len(np.shape(data0))>2:
         data0 = data0[0]
 
     # header info fixes
     try:
         dummy = hdr['CDELT1']
     except:
         hdr['CDELT1'] = hdr['CD1_1']
         hdr['CDELT2'] = hdr['CD2_2']
 
+    # header fix
+    try:
+        _ = hdr['BMAJ']
+    except:
+        hdr['BMAJ'] = hdr['RESOL1']
+        hdr['BMIN'] = hdr['RESOL2']
+
     # if something is wrong, let the user know and stop
     if beamsize < hdr['BMAJ']:
         raise RuntimeError('input beam size is too small')
     if ~np.isclose(hdr['BMAJ'],hdr['BMIN'],rtol=1e-5):
         print( '  beam major axis: ' + str(hdr['BMAJ']) )
         print( '  beam minor axis: ' + str(hdr['BMIN']) )
         ask_user()
@@ -690,29 +665,30 @@
         loreshdr = fits.getheader(loresfile)
         smooth_fits(hiresfile,hinewname,loreshdr['BMAJ'],True)
 
 
 def gauss2Dfit_fits( fitsfile, skyposition, cutsize, calibr_uncert=0.1 ):
     '''
     perform 2D gaussian fitting on a point source.
-    skyposition is made with SkyCoord().
     cutsize is the cutout size over which fitting is performed.
     assumes that the pixels are square shaped.
+    give astropy cutout of a point source and beam FWHM of the data in units of number of pixels
     '''
 
     fitshdu = fits.open(fitsfile)[0]
     fitshdr = fitshdu.header
 
     # header info fixes
     try:
         dummy = fitshdr['CDELT1']
     except:
         fitshdr['CDELT1'] = fitshdr['CD1_1']
         fitshdr['CDELT2'] = fitshdr['CD2_2']
 
+
     fitswcs = WCS(fitshdr)
     fitsdata= fitshdu.data
     cutout  = Cutout2D( fitsdata, skyposition, cutsize, fitswcs )
     beamSTD = FWHM_to_SD( fitshdr['BMAJ']/np.abs(fitshdr['CDELT1']) )
     cutdata = cutout.data
     maxval  = np.nanmax(cutdata)
     initx   = np.where(cutdata==maxval)[0]
@@ -743,14 +719,15 @@
 
 
 
 
 
 
 
+
```

### Comparing `astromulti-1.0.3/src/astromulti/linear_fitting.py` & `astromulti-1.0.4/src/astromulti/linear_fitting.py`

 * *Files identical despite different names*

### Comparing `astromulti-1.0.3/src/astromulti/new_colormap.py` & `astromulti-1.0.4/src/astromulti/new_colormap.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,27 +18,27 @@
     Important things to keep in mind while designing colormaps:
     - grayscale conversion (printing B&W)
     - lightness and perception
     - sequential or diverging or cyclic
     - 'hubble' palette is not recommended for single data images
     '''
     if colors is None:
-        # only palette name is given
+        # i.e., only palette name is given
         if palette=='fire':
             colors = ["black","maroon","yellow","white"]
             nodes  = [  0.0,    0.1,     0.5,    1.0]
         elif palette=='hubble':
             colors = ["black","orange","skyblue","white"]
             nodes  = [  0.0,    0.2,     0.5,    1.0]
         elif palette=='kindlmann':
             colors = ["black","navy","limegreen","yellow","white"]
             nodes  = [  0.0,    0.2,    0.4,        0.7,    1.0]
         else:
             raise RuntimeError('Palette name not recognized.')
-    newcmap1 = LinearSegmentedColormap.from_list("mycmap", list(zip(nodes, colors)))
+    newcmap1 = LinearSegmentedColormap.from_list(palette,list(zip(nodes, colors)))
     if lightnessplotfile:
         rgb = cm.get_cmap(newcmap1)(np.linspace(0.,1.,100))[np.newaxis,:,:3]
         lab = cspace_converter("sRGB1", "CAM02-UCS")(rgb)
         if palette is not None:
             plt.plot(lab[0,:,0],label=palette)
             plt.legend()
         else:
```

### Comparing `astromulti-1.0.3/src/astromulti/region_meta.py` & `astromulti-1.0.4/src/astromulti/region_meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,27 +66,34 @@
     ds9regs = Regions.read( regionfile )
 
     labels = []     # not using list comprehension because printing region details is easier this way
     for rg in range(len(ds9regs)):
         try:
             labels.append(ds9regs[rg].meta['label'])
         except:
-            print("The following region cannot be appended,")
-            print("  likely because no label exists for it.")
-            print("Check your DS9 region file!")
-            print("file: "+regionfile+"; idx: "+rg)
+            try:
+                labels.append(ds9regs[rg].meta['text'])
+            except:
+                print("The following region cannot be appended,")
+                print("  likely because no label exists for it.")
+                print("Check your DS9 region file!")
+                print("file: "+regionfile+"; idx: "+str(rg))
+                raise RuntimeError("No label/text field exists for at least one region!")
 
     duplicates = [ item for item, count in collections.Counter(labels).items() if count > 1 ]
     if not duplicates==[]:
         print(duplicates)
         raise RuntimeError("Duplicates exist! The duplicated labels are printed above for your reference.")
 
     regdict = {}
     for r1 in ds9regs:
-        regdict[r1.meta['label']] = r1
+        try:
+            regdict[r1.meta['label']] = r1
+        except:
+            regdict[r1.meta['text']] = r1
 
     return regdict
 
 
 def rot_PolySkyReg( reg, angl ):
     """
     Rotates 'reg' by the given 'angl'
```

### Comparing `astromulti-1.0.3/src/astromulti/simple_funcs.py` & `astromulti-1.0.4/src/astromulti/simple_funcs.py`

 * *Files identical despite different names*

### Comparing `astromulti-1.0.3/src/astromulti.egg-info/PKG-INFO` & `astromulti-1.0.4/src/astromulti.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromulti
-Version: 1.0.3
+Version: 1.0.4
 Summary: A set of functions for analysis of astronomical images
 Author-email: Rohit D <rohitd@proton.me>
 Project-URL: Homepage, https://gitlab.com/drohi/astromulti
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

