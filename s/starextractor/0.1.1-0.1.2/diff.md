# Comparing `tmp/starextractor-0.1.1-py3-none-any.whl.zip` & `tmp/starextractor-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8649 bytes, number of entries: 9
+Zip file size: 8711 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      564 b- defN 23-Apr-05 03:18 starextractor/__init__.py
--rw-r--r--  2.0 unx     5108 b- defN 23-Apr-05 08:45 starextractor/classes.py
--rw-r--r--  2.0 unx     3752 b- defN 23-Apr-05 08:43 starextractor/image.py
+-rw-r--r--  2.0 unx     5068 b- defN 23-May-11 09:19 starextractor/classes.py
+-rw-r--r--  2.0 unx     3814 b- defN 23-May-11 09:11 starextractor/image.py
 -rw-r--r--  2.0 unx     2937 b- defN 23-Apr-05 07:44 starextractor/plot.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Apr-05 09:24 starextractor-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4117 b- defN 23-Apr-05 09:24 starextractor-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-05 09:24 starextractor-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-05 09:24 starextractor-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      735 b- defN 23-Apr-05 09:24 starextractor-0.1.1.dist-info/RECORD
-9 files, 18387 bytes uncompressed, 7381 bytes compressed:  59.9%
+-rw-r--r--  2.0 unx     1068 b- defN 23-May-11 15:07 starextractor-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4278 b- defN 23-May-11 15:07 starextractor-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-11 15:07 starextractor-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-May-11 15:07 starextractor-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      735 b- defN 23-May-11 15:07 starextractor-0.1.2.dist-info/RECORD
+9 files, 18570 bytes uncompressed, 7443 bytes compressed:  59.9%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: starextractor/image.py
 Comment: 
 
 Filename: starextractor/plot.py
 Comment: 
 
-Filename: starextractor-0.1.1.dist-info/LICENSE
+Filename: starextractor-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: starextractor-0.1.1.dist-info/METADATA
+Filename: starextractor-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: starextractor-0.1.1.dist-info/WHEEL
+Filename: starextractor-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: starextractor-0.1.1.dist-info/top_level.txt
+Filename: starextractor-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: starextractor-0.1.1.dist-info/RECORD
+Filename: starextractor-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## starextractor/classes.py

```diff
@@ -1,10 +1,10 @@
 from photutils.aperture import CircularAperture,aperture_photometry
 
-from .image import read_image,centroid
+from .image import read_image,source_extract
 from .plot import show_image
 
 class AstroImage(object):
     """
     Class AstroImage
     """    
 
@@ -38,57 +38,57 @@
         """    
         image_raw = read_image(imagefile)
         res = image_raw.shape
         info = {'image_raw':image_raw,'res':res}
 
         return AstroImage(info)  
 
-    def find_centroid(self,max_control_points=50,fwhm=12,mask=False):
+    def find_source(self,max_control_points=60,fwhm=12,mask=False):
         """
         Search for star spots in an image, extracting their centroids and doing photometry.
 
         Usage: 
         >>> from sourceextractor import AstroImage
         >>> imagefile = 'obs/fits/img_00000.fits' # imagefile = 'obs/bmp/img_00000.bmp'
         >>> image = AstroImage.read_image(imagefile)
-        >>> centroids = image.find_centroid(imagefile,mask=True)
+        >>> sources = image.find_source(imagefile,mask=True)
 
         Parameters:    
-        max_control_points -> [int,optional,default=50] Maximum number of centroids to extract
+        max_control_points -> [int,optional,default=50] Maximum number of sources to extract
         fwhm -> [float,optional,default=15] Priori Full-width half-maximum (FWHM) of the Gaussian kernel in units of pixels used in DAOStarFinder
         mask -> [bool,optional,default=False] A True value indicates the edge area of an image is masked. Masked pixels are ignored when searching for stars.
         Outputs:
-        centroids -> instance of class Centroid with its attributes as follows:
-            xy_centroids -> [2d array of float] Cartesian pixel coordinates of the star centroids
-            _offset -> [array of float] Cartesian coordinates of the center of the image
+        sources -> Instance of class Source with its attributes as follows:
+            xy_centroids -> [2d array of float] Pixel coordinates of the star centroids
+            _offset -> [array of float] Pixel coordinates of the center of the image
             _image_raw -> [2d array of float] raw grayscale image
             _image -> [2d array of float] signal, i.e. subtracting the background gray value from the raw grayscale image
             _apertures -> A circular aperture defined in pixel coordinates.
             brightness -> [array of float]  Brightness(Grayvalues) of star spots
             snr -> [array of float] Signal Noise Ratio(SNR) of star spots
             mask_rectangle -> [None or tuple] If None, then no mask rectangle is generated; Else, a rectangle defined by the bottom left corner point, width and height is generated
         """
         image_raw = self.image_raw
-        # Search for star spots in an image and extract their centroids
-        xy_centroids,_offset,_image,_bkg_rms,_mask_rectangle = centroid(image_raw,max_control_points,fwhm,mask)
+        # Search for star spots in an image and extract them
+        xy_centroids,_offset,_image,_bkg_rms,_mask_rectangle = source_extract(image_raw,max_control_points,fwhm,mask)
 
         # Do photometry
         _apertures = CircularAperture(xy_centroids, r=fwhm)
         phot_table = aperture_photometry(_image, _apertures) 
         noise_table = aperture_photometry(_bkg_rms, _apertures)
 
         brightness = phot_table['aperture_sum'].value
         noise = noise_table['aperture_sum'].value
         snr = brightness/noise # Signal Noise Ratio
 
         dict_values = xy_centroids,_offset,image_raw,_image,_apertures,brightness,snr,_mask_rectangle
         dict_keys = 'xy','_offset','image_raw','_image','_apertures','brightness','snr','_mask_rectangle'
         info = dict(zip(dict_keys, dict_values))
 
-        return Centroid(info)      
+        return Source(info)      
 
     def show_image(self,fig_out=None):
         """
         Show raw image
 
         Parameters:
         fig_out -> [str,optional,default=None] In not None, save the output image to a file defined by fig_out
@@ -96,37 +96,36 @@
         """
         if fig_out is None:
             show_image(self.image_raw,origin='lower') 
         else:    
             plot_kwargs = {'figname':fig_out}
             show_image(self.image_raw,origin='lower',**plot_kwargs)         
 
-class Centroid(object):
+class Source(object):
     """
-    Class Centroids
+    Class Source
     """
     
     def __init__(self,info):  
 
         self.info = info
 
         for key in info.keys():
             setattr(self, key, info[key])
 
     def __repr__(self):
     
-        return 'instance of class Centroid'
+        return 'Instance of class Source'
 
     def show_image(self,fig_out=None):
         """
-        Show raw image with star spots marked
-
-        Parameters:
-        fig_out -> [str,optional,default=None] In not None, save the image to a file defined by fig_out
+        Show raw image with stars marked
 
+        Inputs:
+            fig_out -> [str,optional,default=None] In not None, save the image to a file defined by fig_out
         """
         if fig_out is None:
             plot_kwargs = {'mark':(self._apertures,'blue')}
         else:
             plot_kwargs = {'mark':(self._apertures,'blue'),'figname':fig_out}
         show_image(self.image_raw,origin='lower',mask_rectangle=self._mask_rectangle,**plot_kwargs)
```

## starextractor/image.py

```diff
@@ -6,58 +6,56 @@
 from PIL import Image
 
 def read_image(imagefile):
     """
     Read an astronomical image captured by cameras in fits format or in generic image format.
 
     Usage:
-    >>> imagefile = 'obs/fits/img_00000.fits' # imagefile = 'obs/bmp/img_00000.bmp'
-    >>> image_raw = read_image(imagefile)
+        >>> imagefile = 'obs/fits/img_00000.fits' # imagefile = 'obs/bmp/img_00000.bmp'
+        >>> image_raw = read_image(imagefile)
 
     Inputs:
-    imagefile -> [str] image filename
+        imagefile -> [str] image filename
 
     Outputs:
-    image_raw -> [2d array of float] raw grayscale image with origin at bottom left corner point
+        image_raw -> [2d array of float] raw grayscale image with origin at bottom left corner point
     """
     if imagefile.split('.')[1] in ['fits','fit']: # Load an astronomical image in format of fits
         unit_list = fits.open(imagefile)
         image_raw = unit_list[0].data.astype(float) 
     else:
         image_raw = Image.open(imagefile).convert('L') # Load an astronomical image in generic image format
         image_raw = np.asarray(image_raw)
     # convert origin from top left to bottom left
     image_raw = image_raw[::-1] 
 
     return image_raw
     
 
-def centroid(image_raw,max_control_points=50,fwhm=12,mask=False):
+def source_extract(image_raw,max_control_points=60,fwhm=12,mask=False):
     """
     Search for star spots in an image, extracting their centroids and doing photometry.
 
     Usage: 
-    >>> imagefile = 'obs/fits/img_00000.fits' # imagefile = 'obs/bmp/img_00000.bmp'
-    >>> image_raw = read_image(imagefile)
-    >>> xy_centroids,offset,image,bkg_rms,mask_rectangle = centroid(image_raw)
+        >>> imagefile = 'obs/fits/img_00000.fits' # imagefile = 'obs/bmp/img_00000.bmp'
+        >>> image_raw = read_image(imagefile)
+        >>> xy_centroids,offset,image,bkg_rms,mask_rectangle = source_extract(image_raw)
     
     Inputs:
-    image_raw -> [2d array of float] raw grayscale image with origin at bottom left corner point
-
-    Parameters:    
-    max_control_points -> [int,optional,default=50] Maximum number of centroids to extract
-    fwhm -> [float,optional,default=15] Full-width half-maximum (FWHM) of the Gaussian kernel in units of pixels used in DAOStarFinder
-    mask -> [bool,optional,default=False] A True value indicates the edge area of an image is masked. Masked pixels are ignored when searching for stars.
+        image_raw -> [2d array of float] raw grayscale image with origin at bottom left corner point  
+        max_control_points -> [int,optional,default=50] Maximum number of sources to extract
+        fwhm -> [float,optional,default=15] Full-width half-maximum (FWHM) of the Gaussian kernel in units of pixels used in DAOStarFinder
+        mask -> [bool,optional,default=False] A True value indicates the edge area of an image is masked. Masked pixels are ignored when searching for stars.
 
     Outputs:
-    xy_centroids -> [2d array of float] Cartesian pixel coordinates of the star centroids
-    offset -> [array of float] Cartesian coordinates of the center of the image
-    image -> [2d array of float] signal, i.e. subtracting the background gray value from the raw grayscale image
-    bkg_rms -> [2d array of float] background noise
-    mask_rectangle -> [None or tuple] If None, then no mask rectangle is generated; Else, a rectangle defined by the bottom left corner point, width and height is generated
+        xy_centroids -> [2d array of float] Cartesian pixel coordinates of the centroids of star spots
+        offset -> [array of float] Cartesian coordinates of the center of the image
+        image -> [2d array of float] signal, i.e. subtracting the background gray value from the raw grayscale image
+        bkg_rms -> [2d array of float] background noise
+        mask_rectangle -> [None or tuple] If None, then no mask rectangle is generated; Else, a rectangle defined by the bottom left corner point, width and height is generated
     """
 
     # Calculate the offset of the image center from the origin
     yc, xc = image_raw.shape
     offset = np.array([xc/2,yc/2]) - 0.5
             
     # Deaverage the image
@@ -76,13 +74,13 @@
         width,height = xc//2,yc//2
         mask_rectangle = ([lb,bb],width,height)
         mask_region[bb:ub, lb:rb] = False
     else:
         mask_region = None
         mask_rectangle = None
             
-    # Search for star spots and extract their centroids
+    # Extract star spots and estimate their centroids
     daofind = DAOStarFinder(fwhm=fwhm,threshold=5*bkg_sigma,brightest=max_control_points) 
     star_spots = daofind(image,mask=mask_region)  
     xy_centroids = np.transpose((star_spots['xcentroid'], star_spots['ycentroid']))
 
     return xy_centroids,offset,image,bkg_rms,mask_rectangle
```

## Comparing `starextractor-0.1.1.dist-info/LICENSE` & `starextractor-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `starextractor-0.1.1.dist-info/METADATA` & `starextractor-0.1.2.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starextractor
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package to extract stars from an astronomical image
 Home-page: https://github.com/lcx366/STAREXTRACTOR
 Author: Chunxiao Li
 Author-email: lcx366@126.com
 License: MIT
 Keywords: source extract,stars
 Classifier: Development Status :: 4 - Beta
@@ -25,79 +25,82 @@
 # Welcome to the STAREXTRACTOR package
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/starextractor.svg)](https://pypi.python.org/pypi/starextractor/) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/starextractor.svg)](https://pypi.python.org/pypi/starextractor/) [![PyPI status](https://img.shields.io/pypi/status/starextractor.svg)](https://pypi.python.org/pypi/starextractor/) [![GitHub contributors](https://img.shields.io/github/contributors/lcx366/STAREXTRACTOR.svg)](https://GitHub.com/lcx366/STAREXTRACTOR/graphs/contributors/) [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/lcx366/STAREXTRACTOR/graphs/commit-activity) [![GitHub license](https://img.shields.io/github/license/lcx366/STAREXTRACTOR.svg)](https://github.com/lcx366/STAREXTRACTOR/blob/master/LICENSE) [![Documentation Status](https://readthedocs.org/projects/starextractor/badge/?version=latest)](http://starextractor.readthedocs.io/?badge=latest) [![Build Status](https://travis-ci.org/lcx366/starextractor.svg?branch=master)](https://travis-ci.org/lcx366/starextractor)
 
 This package is an archive of scientific routines for data processing related to the source extraction from an astronomical image.
 Currently, operations on source extraction include:
 
-1. Read an astronomical image captured by cameras in fits format or in generic image format;
-2. Search for stars, extract their centroids and do photometry using `photutils`;
-3. Show raw image with star marked;
+1. Read an astronomical image in `.fits` format or in generic image format, such as `.bmp`;
+2. Extract the centroid coordinates of the star spots and do photometry using `photutils`;
+3. Show raw image with star spots marked;
 
 ## How to Install
 
-On Linux, macOS and Windows architectures, the binary wheels can be installed using pip by executing one of the following commands:
+On Linux, macOS and Windows architectures, the binary wheels can be installed using `pip` by executing one of the following commands:
 
 ```
 pip install starextractor
 pip install starextractor --upgrade # to upgrade a pre-existing installation
 ```
 
 ## How to use
 
 ### Read an astronomical image
 
-Images can be in `.fits` format or in generic image format, such as `.bmp`
+Images can be in `.fits` format or in generic image format, such as `.bmp`.
 
 ```python
 >>> from starextractor import AstroImage
 >>> imagefile = 'obs/fits/img_00000.fits' #imagefile = 'obs/bmp/img_00000.bmp'
 >>> image = AstroImage.read_image(imagefile)
 ```
 
-Output the raw grayscale image with origin at bottom(the first row) left corner point.
+Print the raw grayscale image with the origin at the center of the bottom(the first row of array) left pixel.
 
 ```python
->>> rawimage = image.rawimage
->>> print(image.raw_image,image.res) # image resolution
+>>> print(image.image_raw,image.res) # original grayscale image and its resolution
 ```
 
-Show raw image
+### Show the raw image
 
 ```python
 >>> image.show_image()
 >>> #image.show_image('figs/raw_image.png') # save image to a file
 ```
 
 <p align="middle">
   <img src="readme_figs/image_raw.png" width="500" />
 </p>
 
-#### Search for stars, extract their centroids and do photometry
+### Extract the centroid coordinates of the star spots and do photometry
 
-Estimate the centroids coordinates, brightness(sum of grayvalue within an aperture),  and SNR of star spots.
+Estimate the centroids coordinates, brightness(sum of gray value within an aperture),  and SNR of star spots.
 
 ```python
->>> centroids = image.find_centroid(fwhm=12,max_control_points=50,mask=True)
->>> print(centroids.xy,centroids.brightness,centroids.snr)
+>>> sources = image.find_source(fwhm=12,max_control_points=50,mask=True)
+>>> print(sources.xy,sources.brightness,sources.snr)
 ```
 
-Show raw image
+### Show the raw image
 
 ```python
->>> centroids.show_image()
->>> #centroids.show_image('figs/centroids.png') # save image to a file
+>>> sources.show_image()
+>>> #sources.show_image('figs/sources.png') # save image to a file
 ```
 
 <p align="middle">
   <img src="readme_figs/centroids.png" width="500" />
 </p>
 
 ## Change log
 
+- **0.1.2 — May 11,  2023**
+  
+  - The class `Centriod` is *deprecated*, and the class `Source` is used instead
+
 - **0.1.0 — Apr 5,  2023**
   
   - The ***starextractor*** package was released.
 
 ## Reference
 
 - [photutils](https://photutils.readthedocs.io/en/stable/index.html)
```

## Comparing `starextractor-0.1.1.dist-info/RECORD` & `starextractor-0.1.2.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 starextractor/__init__.py,sha256=CI2mxua1zYm0gwTkzBbIc1vxZ_MhdKyfVEp5Qsfv8gM,564
-starextractor/classes.py,sha256=sgPKs5r-Kg9sH8JlBXcaY8tJATS5eDUwt8xTvm_3IEU,5108
-starextractor/image.py,sha256=9-Z29XdzehYd7442ikOZv-v_CVkUW920dHO_Ab5_R80,3752
+starextractor/classes.py,sha256=VhIWWFB_xHOWLkBsthjbxylEL_OmQoEL6rG9yjVrOE0,5068
+starextractor/image.py,sha256=5WiKMycAwULNO44WOpJZs51IL6LogOb6n80R_G_HqTM,3814
 starextractor/plot.py,sha256=Dllpov4H72BOlZjhSLpwbmw9E2fKa5jXXFSNQNIKg-c,2937
-starextractor-0.1.1.dist-info/LICENSE,sha256=1mo8gGwn9nEfzoruoWYAD1ttN40DofMYGQNef1rsytY,1068
-starextractor-0.1.1.dist-info/METADATA,sha256=rWOOWqUlLkeRZhAaZXo8VI4y6YegZ4o_Y5iTlLTkKOc,4117
-starextractor-0.1.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-starextractor-0.1.1.dist-info/top_level.txt,sha256=QBc6fvT33gTCfADa-aXjDX7yfBqb8twQR3BQjM5cwls,14
-starextractor-0.1.1.dist-info/RECORD,,
+starextractor-0.1.2.dist-info/LICENSE,sha256=1mo8gGwn9nEfzoruoWYAD1ttN40DofMYGQNef1rsytY,1068
+starextractor-0.1.2.dist-info/METADATA,sha256=_aRodrc_L4DNb3rYDYpURW5QoF3asII2xKtjFT7EpVk,4278
+starextractor-0.1.2.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+starextractor-0.1.2.dist-info/top_level.txt,sha256=QBc6fvT33gTCfADa-aXjDX7yfBqb8twQR3BQjM5cwls,14
+starextractor-0.1.2.dist-info/RECORD,,
```

