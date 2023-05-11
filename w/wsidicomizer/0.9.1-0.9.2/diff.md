# Comparing `tmp/wsidicomizer-0.9.1.tar.gz` & `tmp/wsidicomizer-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsidicomizer-0.9.1.tar", max compression
+gzip compressed data, was "wsidicomizer-0.9.2.tar", max compression
```

## Comparing `wsidicomizer-0.9.1.tar` & `wsidicomizer-0.9.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1733 2023-04-16 18:01:15.190683 wsidicomizer-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     8205 2023-04-03 13:27:43.536187 wsidicomizer-0.9.1/README.md
--rw-r--r--   0        0        0      921 2023-04-16 18:01:15.195683 wsidicomizer-0.9.1/wsidicomizer/__init__.py
--rw-r--r--   0        0        0    10732 2023-04-03 13:27:43.562194 wsidicomizer-0.9.1/wsidicomizer/cli.py
--rw-r--r--   0        0        0     1197 2023-04-03 06:05:46.207813 wsidicomizer-0.9.1/wsidicomizer/config.py
--rw-r--r--   0        0        0    23475 2023-04-16 18:01:15.243759 wsidicomizer-0.9.1/wsidicomizer/dataset.py
--rw-r--r--   0        0        0     6735 2023-04-16 18:01:15.266942 wsidicomizer-0.9.1/wsidicomizer/dicomizer_source.py
--rw-r--r--   0        0        0     6049 2023-03-31 14:54:00.541987 wsidicomizer-0.9.1/wsidicomizer/encoding.py
--rw-r--r--   0        0        0      789 2023-04-03 13:27:43.575189 wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/__init__.py
--rw-r--r--   0        0        0     2228 2023-04-03 13:27:43.576394 wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/bioformats_cli.py
--rw-r--r--   0        0        0     3913 2023-04-16 18:01:15.299403 wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/bioformats_dicomizer.py
--rw-r--r--   0        0        0     4418 2023-04-03 13:27:43.578184 wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/bioformats_image_data.py
--rw-r--r--   0        0        0    14802 2023-04-08 06:20:09.255055 wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/bioformats_reader.py
--rw-r--r--   0        0        0     5403 2023-04-16 18:01:15.324824 wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/bioformats_source.py
--rw-r--r--   0        0        0      769 2023-04-03 06:08:44.876033 wsidicomizer-0.9.1/wsidicomizer/extras/openslide/__init__.py
--rw-r--r--   0        0        0     2227 2023-04-03 06:08:51.748970 wsidicomizer-0.9.1/wsidicomizer/extras/openslide/openslide.py
--rw-r--r--   0        0        0    16631 2023-04-03 13:27:43.582423 wsidicomizer-0.9.1/wsidicomizer/extras/openslide/openslide_image_data.py
--rw-r--r--   0        0        0     1476 2023-04-03 13:27:43.593514 wsidicomizer-0.9.1/wsidicomizer/extras/openslide/openslide_metadata.py
--rw-r--r--   0        0        0     3787 2023-04-16 18:01:15.353013 wsidicomizer-0.9.1/wsidicomizer/extras/openslide/openslide_source.py
--rw-r--r--   0        0        0     2069 2023-04-03 06:06:15.956751 wsidicomizer-0.9.1/wsidicomizer/image_data.py
--rw-r--r--   0        0        0      860 2023-04-03 13:27:43.595183 wsidicomizer-0.9.1/wsidicomizer/sources/__init__.py
--rw-r--r--   0        0        0      746 2023-03-31 14:54:00.564988 wsidicomizer-0.9.1/wsidicomizer/sources/czi/__init__.py
--rw-r--r--   0        0        0    13161 2023-04-03 13:27:43.605550 wsidicomizer-0.9.1/wsidicomizer/sources/czi/czi_image_data.py
--rw-r--r--   0        0        0     7933 2023-04-16 18:01:15.358822 wsidicomizer-0.9.1/wsidicomizer/sources/czi/czi_metadata.py
--rw-r--r--   0        0        0     2899 2023-04-16 18:01:15.407906 wsidicomizer-0.9.1/wsidicomizer/sources/czi/czi_source.py
--rw-r--r--   0        0        0      771 2023-04-16 18:02:33.046081 wsidicomizer-0.9.1/wsidicomizer/sources/opentile/__init__.py
--rw-r--r--   0        0        0     8756 2023-04-08 06:20:09.243941 wsidicomizer-0.9.1/wsidicomizer/sources/opentile/opentile_image_data.py
--rw-r--r--   0        0        0     3102 2023-04-16 18:01:15.432092 wsidicomizer-0.9.1/wsidicomizer/sources/opentile/opentile_source.py
--rw-r--r--   0        0        0      775 2023-04-03 13:27:43.622220 wsidicomizer-0.9.1/wsidicomizer/sources/tiffslide/__init__.py
--rw-r--r--   0        0        0    15167 2023-04-16 18:01:15.458910 wsidicomizer-0.9.1/wsidicomizer/sources/tiffslide/tiffslide_image_data.py
--rw-r--r--   0        0        0     1443 2023-04-16 18:01:15.485967 wsidicomizer-0.9.1/wsidicomizer/sources/tiffslide/tiffslide_metadata.py
--rw-r--r--   0        0        0     3575 2023-04-16 18:01:15.515906 wsidicomizer-0.9.1/wsidicomizer/sources/tiffslide/tiffslide_source.py
--rw-r--r--   0        0        0     9561 2023-04-16 18:01:15.541906 wsidicomizer-0.9.1/wsidicomizer/wsidicomizer.py
--rw-r--r--   0        0        0     9782 1970-01-01 00:00:00.000000 wsidicomizer-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1733 2023-05-11 13:26:16.759959 wsidicomizer-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     8191 2023-05-11 13:26:16.751696 wsidicomizer-0.9.2/README.md
+-rw-r--r--   0        0        0      921 2023-05-11 13:26:16.764698 wsidicomizer-0.9.2/wsidicomizer/__init__.py
+-rw-r--r--   0        0        0    10732 2023-04-03 13:27:43.562194 wsidicomizer-0.9.2/wsidicomizer/cli.py
+-rw-r--r--   0        0        0     1197 2023-04-03 06:05:46.207813 wsidicomizer-0.9.2/wsidicomizer/config.py
+-rw-r--r--   0        0        0    23475 2023-04-27 11:02:16.094157 wsidicomizer-0.9.2/wsidicomizer/dataset.py
+-rw-r--r--   0        0        0     6735 2023-04-27 11:02:16.096375 wsidicomizer-0.9.2/wsidicomizer/dicomizer_source.py
+-rw-r--r--   0        0        0     6094 2023-05-11 13:26:16.766698 wsidicomizer-0.9.2/wsidicomizer/encoding.py
+-rw-r--r--   0        0        0      789 2023-04-03 13:27:43.575189 wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/__init__.py
+-rw-r--r--   0        0        0     2228 2023-04-03 13:27:43.576394 wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/bioformats_cli.py
+-rw-r--r--   0        0        0     3913 2023-04-27 11:02:16.099286 wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/bioformats_dicomizer.py
+-rw-r--r--   0        0        0     4418 2023-04-03 13:27:43.578184 wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/bioformats_image_data.py
+-rw-r--r--   0        0        0    14802 2023-04-08 06:20:09.255055 wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/bioformats_reader.py
+-rw-r--r--   0        0        0     5403 2023-04-27 11:02:16.100156 wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/bioformats_source.py
+-rw-r--r--   0        0        0      769 2023-04-03 06:08:44.876033 wsidicomizer-0.9.2/wsidicomizer/extras/openslide/__init__.py
+-rw-r--r--   0        0        0     2227 2023-04-03 06:08:51.748970 wsidicomizer-0.9.2/wsidicomizer/extras/openslide/openslide.py
+-rw-r--r--   0        0        0    16631 2023-04-03 13:27:43.582423 wsidicomizer-0.9.2/wsidicomizer/extras/openslide/openslide_image_data.py
+-rw-r--r--   0        0        0     1476 2023-04-03 13:27:43.593514 wsidicomizer-0.9.2/wsidicomizer/extras/openslide/openslide_metadata.py
+-rw-r--r--   0        0        0     3787 2023-04-27 11:02:16.102156 wsidicomizer-0.9.2/wsidicomizer/extras/openslide/openslide_source.py
+-rw-r--r--   0        0        0     2069 2023-04-03 06:06:15.956751 wsidicomizer-0.9.2/wsidicomizer/image_data.py
+-rw-r--r--   0        0        0      860 2023-04-03 13:27:43.595183 wsidicomizer-0.9.2/wsidicomizer/sources/__init__.py
+-rw-r--r--   0        0        0      746 2023-03-31 14:54:00.564988 wsidicomizer-0.9.2/wsidicomizer/sources/czi/__init__.py
+-rw-r--r--   0        0        0    13161 2023-04-03 13:27:43.605550 wsidicomizer-0.9.2/wsidicomizer/sources/czi/czi_image_data.py
+-rw-r--r--   0        0        0     7933 2023-04-27 11:02:16.105158 wsidicomizer-0.9.2/wsidicomizer/sources/czi/czi_metadata.py
+-rw-r--r--   0        0        0     2899 2023-04-27 11:02:16.109161 wsidicomizer-0.9.2/wsidicomizer/sources/czi/czi_source.py
+-rw-r--r--   0        0        0      771 2023-04-16 18:02:33.046081 wsidicomizer-0.9.2/wsidicomizer/sources/opentile/__init__.py
+-rw-r--r--   0        0        0     8756 2023-04-08 06:20:09.243941 wsidicomizer-0.9.2/wsidicomizer/sources/opentile/opentile_image_data.py
+-rw-r--r--   0        0        0     3102 2023-04-27 11:02:16.111155 wsidicomizer-0.9.2/wsidicomizer/sources/opentile/opentile_source.py
+-rw-r--r--   0        0        0      775 2023-04-03 13:27:43.622220 wsidicomizer-0.9.2/wsidicomizer/sources/tiffslide/__init__.py
+-rw-r--r--   0        0        0    15167 2023-04-27 11:02:16.112156 wsidicomizer-0.9.2/wsidicomizer/sources/tiffslide/tiffslide_image_data.py
+-rw-r--r--   0        0        0     1443 2023-04-27 11:02:16.114308 wsidicomizer-0.9.2/wsidicomizer/sources/tiffslide/tiffslide_metadata.py
+-rw-r--r--   0        0        0     3575 2023-04-27 11:02:16.116157 wsidicomizer-0.9.2/wsidicomizer/sources/tiffslide/tiffslide_source.py
+-rw-r--r--   0        0        0     9593 2023-05-11 13:26:16.769358 wsidicomizer-0.9.2/wsidicomizer/wsidicomizer.py
+-rw-r--r--   0        0        0     9768 1970-01-01 00:00:00.000000 wsidicomizer-0.9.2/PKG-INFO
```

### Comparing `wsidicomizer-0.9.1/pyproject.toml` & `wsidicomizer-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wsidicomizer"
-version = "0.9.1"
+version = "0.9.2"
 description = "Tool for reading WSI files from proprietary formats and optionally convert them to to DICOM"
 authors = ["Erik O Gabrielsson <erik.o.gabrielsson@sectra.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/imi-bigpicture/wsidicomizer"
 keywords = ["whole slide image", "digital pathology", "dicom", "converter"]
 classifiers = [
```

### Comparing `wsidicomizer-0.9.1/README.md` & `wsidicomizer-0.9.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -140,28 +140,28 @@
 ## Openslide support
 
 ### Installation
 
 Support for reading images using Openslide c library can optionally be enabled by installing *wsidicomizer* with the `openslide` extra:
 
 ```console
-pip install wsidicomizer --extras openslide
+pip install wsidicomizer[openslide]
 ```
 
 The OpenSlide extra requires the OpenSlide library to be installed separately. Instructions for how to install OpenSlide is avaiable on <https://openslide.org/download/>
 For Windows, you need also need add OpenSlide's bin-folder to the environment variable 'Path'
 
 ## Bioformats support
 
 ### Installation
 
 Support for reading images using Bioformats java library can optionally be enabled by installing *wsidicomizer* with the `bioformats` extra:
 
 ```console
-pip install wsidicomizer --extras bioformats
+pip install wsidicomizer[bioformats]
 ```
 
 The `bioformats` extra enables usage of the `bioformats` module and the `bioformats_wsidicomizer`-cli command. The required Bioformats java library (jar-file) is downloaded automatically when the module is imported using [scyjava](https://github.com/scijava/scyjava).
 
 ### Using
 
 As the Bioformats library is a java library it needs to run in a java virtual machine (JVM). A JVM is started automatically when the `bioformats` module is imported. The JVM can´t be restarted in the same Python inteprenter, and is therfore left running once started. If you want to shutdown the JVM (without closing the Python inteprenter) you can call the shutdown_jvm()-method:
@@ -195,8 +195,8 @@
 
 Our aim is to provide constructive and positive code reviews for all submissions. The project relies on gradual typing and roughly follows PEP8. However, we are not dogmatic. Most important is that the code is easy to read and understand.
 
 ## Acknowledgement
 
 *wsidicomizer*: Copyright 2021 Sectra AB, licensed under Apache 2.0.
 
-This project is part of a project that has received funding from the Innovative Medicines Initiative 2 Joint Undertaking under grant agreement No 945358. This Joint Undertaking receives support from the European Union’s Horizon 2020 research and innovation programme and EFPIA. IMI website: www.imi.europa.eu
+This project is part of a project that has received funding from the Innovative Medicines Initiative 2 Joint Undertaking under grant agreement No 945358. This Joint Undertaking receives support from the European Union’s Horizon 2020 research and innovation programme and EFPIA. IMI website: <www.imi.europa.eu>
```

### Comparing `wsidicomizer-0.9.1/wsidicomizer/__init__.py` & `wsidicomizer-0.9.2/wsidicomizer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
     create_patient_module,
     create_sample,
     create_specimen_module,
     create_study_module,
 )
 from wsidicomizer.wsidicomizer import WsiDicomizer
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
```

### Comparing `wsidicomizer-0.9.1/wsidicomizer/cli.py` & `wsidicomizer-0.9.2/wsidicomizer/cli.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/config.py` & `wsidicomizer-0.9.2/wsidicomizer/config.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/dataset.py` & `wsidicomizer-0.9.2/wsidicomizer/dataset.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/dicomizer_source.py` & `wsidicomizer-0.9.2/wsidicomizer/dicomizer_source.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/encoding.py` & `wsidicomizer-0.9.2/wsidicomizer/encoding.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
     def __init__(self, quality: int = 90, subsampling: Optional[str] = "420") -> None:
         """Creates a JPEG encoder with specified settings.
 
         Parameters
         ----------
         quality: int = 90
-            The encoding quality. To not use higher than 95.
+            The encoding quality. Recommended to not use higher than 95.
         subsampling: Optional[str] = '420'
             Subsampling option. Use '444' for no subsampling, '422' for 2x1
             subsampling, and '420' for 2x2 subsampling.
         """
         self._quality = quality
         if subsampling not in ["444", "422", "420"]:
             raise NotImplementedError(
@@ -139,20 +139,20 @@
 class Jpeg2000Encoder(Encoder):
     def __init__(self, quality: float = 20.0) -> None:
         """Creates a JPEG2000 encoder with specified settings.
 
         Parameters
         ----------
         quality: float = 20.0.
-            The encoding quality as peak signal to noise (PSNR). Use < 1 for
+            The encoding quality as peak signal to noise (PSNR). Use < 1 or > 1000 for
             lossless quality. Up to 60 gives acceptable results.
 
         """
         self._quality = quality
-        if self.quality < 1:
+        if self.quality < 1 or self.quality > 1000:
             self._transfer_syntax = JPEG2000Lossless
         else:
             self._transfer_syntax = JPEG2000
 
     def photometric_interpretation(self, channels: int) -> str:
         if channels == 1:
             return "MONOCRHOME2"
```

### Comparing `wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/__init__.py` & `wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/__init__.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/bioformats_cli.py` & `wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/bioformats_cli.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/bioformats_dicomizer.py` & `wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/bioformats_dicomizer.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/bioformats_image_data.py` & `wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/bioformats_image_data.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/bioformats_reader.py` & `wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/bioformats_reader.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/extras/bioformats/bioformats_source.py` & `wsidicomizer-0.9.2/wsidicomizer/extras/bioformats/bioformats_source.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/extras/openslide/__init__.py` & `wsidicomizer-0.9.2/wsidicomizer/extras/openslide/__init__.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/extras/openslide/openslide.py` & `wsidicomizer-0.9.2/wsidicomizer/extras/openslide/openslide.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/extras/openslide/openslide_image_data.py` & `wsidicomizer-0.9.2/wsidicomizer/extras/openslide/openslide_image_data.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/extras/openslide/openslide_metadata.py` & `wsidicomizer-0.9.2/wsidicomizer/extras/openslide/openslide_metadata.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/extras/openslide/openslide_source.py` & `wsidicomizer-0.9.2/wsidicomizer/extras/openslide/openslide_source.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/image_data.py` & `wsidicomizer-0.9.2/wsidicomizer/image_data.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/sources/__init__.py` & `wsidicomizer-0.9.2/wsidicomizer/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/sources/czi/__init__.py` & `wsidicomizer-0.9.2/wsidicomizer/sources/czi/__init__.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/sources/czi/czi_image_data.py` & `wsidicomizer-0.9.2/wsidicomizer/sources/czi/czi_image_data.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/sources/czi/czi_metadata.py` & `wsidicomizer-0.9.2/wsidicomizer/sources/czi/czi_metadata.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/sources/czi/czi_source.py` & `wsidicomizer-0.9.2/wsidicomizer/sources/czi/czi_source.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/sources/opentile/__init__.py` & `wsidicomizer-0.9.2/wsidicomizer/sources/opentile/__init__.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/sources/opentile/opentile_image_data.py` & `wsidicomizer-0.9.2/wsidicomizer/sources/opentile/opentile_image_data.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/sources/opentile/opentile_source.py` & `wsidicomizer-0.9.2/wsidicomizer/sources/opentile/opentile_source.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/sources/tiffslide/__init__.py` & `wsidicomizer-0.9.2/wsidicomizer/sources/tiffslide/__init__.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/sources/tiffslide/tiffslide_image_data.py` & `wsidicomizer-0.9.2/wsidicomizer/sources/tiffslide/tiffslide_image_data.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/sources/tiffslide/tiffslide_metadata.py` & `wsidicomizer-0.9.2/wsidicomizer/sources/tiffslide/tiffslide_metadata.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/sources/tiffslide/tiffslide_source.py` & `wsidicomizer-0.9.2/wsidicomizer/sources/tiffslide/tiffslide_source.py`

 * *Files identical despite different names*

### Comparing `wsidicomizer-0.9.1/wsidicomizer/wsidicomizer.py` & `wsidicomizer-0.9.2/wsidicomizer/wsidicomizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         modules: Optional[Union[Dataset, Sequence[Dataset]]] = None,
         tile_size: int = 512,
         include_levels: Optional[Sequence[int]] = None,
         include_label: bool = True,
         include_overview: bool = True,
         include_confidential: bool = True,
         encoding_format: str = "jpeg",
-        encoding_quality: int = 90,
+        encoding_quality: float = 90,
         jpeg_subsampling: str = "420",
         label: Optional[Union[PILImage, str, Path]] = None,
         preferred_source: Optional[Type[DicomizerSource]] = None,
         **source_args,
     ) -> WsiDicom:
         """Open data in file in filepath as WsiDicom.
 
@@ -83,17 +83,17 @@
             Include label(s), default true.
         include_overwiew: bool = True
             Include overview(s), default true.
         include_confidential: bool = True
             Include confidential metadata.
         encoding_format: str = 'jpeg'
             Encoding format to use if re-encoding. 'jpeg' or 'jpeg2000'.
-        encoding_quality: int = 90
-            Quality to use if re-encoding. Do not use > 95 for jpeg. Use 100
-            for lossless jpeg2000.
+        encoding_quality: float = 90
+            Quality to use if re-encoding. It is recommended to not use > 95 for jpeg.
+            Use < 1 or > 1000 for lossless jpeg2000.
         jpeg_subsampling: str = '420'
             Subsampling option if using jpeg for re-encoding. Use '444' for
             no subsampling, '422' for 2x1 subsampling, and '420' for 2x2
             subsampling.
         label: Optional[Union[PILImage, str, Path]] = None
             Optional label image to use instead of label found in file.
         preferred_source: Optional[Type[DicomizerSource]] = None
```

### Comparing `wsidicomizer-0.9.1/PKG-INFO` & `wsidicomizer-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsidicomizer
-Version: 0.9.1
+Version: 0.9.2
 Summary: Tool for reading WSI files from proprietary formats and optionally convert them to to DICOM
 Home-page: https://github.com/imi-bigpicture/wsidicomizer
 License: Apache-2.0
 Keywords: whole slide image,digital pathology,dicom,converter
 Author: Erik O Gabrielsson
 Author-email: erik.o.gabrielsson@sectra.com
 Requires-Python: >=3.8,<3.12
@@ -179,28 +179,28 @@
 ## Openslide support
 
 ### Installation
 
 Support for reading images using Openslide c library can optionally be enabled by installing *wsidicomizer* with the `openslide` extra:
 
 ```console
-pip install wsidicomizer --extras openslide
+pip install wsidicomizer[openslide]
 ```
 
 The OpenSlide extra requires the OpenSlide library to be installed separately. Instructions for how to install OpenSlide is avaiable on <https://openslide.org/download/>
 For Windows, you need also need add OpenSlide's bin-folder to the environment variable 'Path'
 
 ## Bioformats support
 
 ### Installation
 
 Support for reading images using Bioformats java library can optionally be enabled by installing *wsidicomizer* with the `bioformats` extra:
 
 ```console
-pip install wsidicomizer --extras bioformats
+pip install wsidicomizer[bioformats]
 ```
 
 The `bioformats` extra enables usage of the `bioformats` module and the `bioformats_wsidicomizer`-cli command. The required Bioformats java library (jar-file) is downloaded automatically when the module is imported using [scyjava](https://github.com/scijava/scyjava).
 
 ### Using
 
 As the Bioformats library is a java library it needs to run in a java virtual machine (JVM). A JVM is started automatically when the `bioformats` module is imported. The JVM can´t be restarted in the same Python inteprenter, and is therfore left running once started. If you want to shutdown the JVM (without closing the Python inteprenter) you can call the shutdown_jvm()-method:
@@ -234,9 +234,9 @@
 
 Our aim is to provide constructive and positive code reviews for all submissions. The project relies on gradual typing and roughly follows PEP8. However, we are not dogmatic. Most important is that the code is easy to read and understand.
 
 ## Acknowledgement
 
 *wsidicomizer*: Copyright 2021 Sectra AB, licensed under Apache 2.0.
 
-This project is part of a project that has received funding from the Innovative Medicines Initiative 2 Joint Undertaking under grant agreement No 945358. This Joint Undertaking receives support from the European Union’s Horizon 2020 research and innovation programme and EFPIA. IMI website: www.imi.europa.eu
+This project is part of a project that has received funding from the Innovative Medicines Initiative 2 Joint Undertaking under grant agreement No 945358. This Joint Undertaking receives support from the European Union’s Horizon 2020 research and innovation programme and EFPIA. IMI website: <www.imi.europa.eu>
```

