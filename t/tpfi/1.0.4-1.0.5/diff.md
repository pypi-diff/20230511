# Comparing `tmp/tpfi-1.0.4.tar.gz` & `tmp/tpfi-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpfi-1.0.4.tar", max compression
+gzip compressed data, was "tpfi-1.0.5.tar", max compression
```

## Comparing `tpfi-1.0.4.tar` & `tpfi-1.0.5.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-05-02 10:27:26.163043 tpfi-1.0.4/LICENSE
--rw-r--r--   0        0        0     2251 2023-05-02 10:27:26.163043 tpfi-1.0.4/README.md
--rw-r--r--   0        0        0      417 2023-05-02 10:27:26.171043 tpfi-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      123 2023-05-02 10:27:26.171043 tpfi-1.0.4/src/tpfi/__init__.py
--rw-r--r--   0        0        0    15351 2023-05-02 10:27:26.171043 tpfi-1.0.4/src/tpfi/tpfi.py
--rw-r--r--   0        0        0     5333 2023-05-02 10:27:26.171043 tpfi-1.0.4/src/tpfi/utils.py
--rw-r--r--   0        0        0     2930 1970-01-01 00:00:00.000000 tpfi-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-11 02:14:49.669951 tpfi-1.0.5/LICENSE
+-rw-r--r--   0        0        0     2271 2023-05-11 02:14:49.925952 tpfi-1.0.5/README.md
+-rw-r--r--   0        0        0      563 2023-05-11 02:14:49.677951 tpfi-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      154 2023-05-11 02:14:49.677951 tpfi-1.0.5/src/tpfi/__init__.py
+-rw-r--r--   0        0        0    15258 2023-05-11 02:14:49.677951 tpfi-1.0.5/src/tpfi/tpfi.py
+-rw-r--r--   0        0        0     5333 2023-05-11 02:14:49.677951 tpfi-1.0.5/src/tpfi/utils.py
+-rw-r--r--   0        0        0       22 2023-05-11 02:14:49.677951 tpfi-1.0.5/src/tpfi/version.py
+-rw-r--r--   0        0        0     2950 1970-01-01 00:00:00.000000 tpfi-1.0.5/PKG-INFO
```

### Comparing `tpfi-1.0.4/LICENSE` & `tpfi-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tpfi-1.0.4/README.md` & `tpfi-1.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -41,18 +41,18 @@
 You can install this package using `pip`:
 ```shell
 pip install tpfi
 ```
 
 ## How to use
 
-See the [example notebook](https://github.com/keyuxing/tpfi/blob/main/examples/tutorial.ipynb) for more details.
+See the [example notebook](https://raw.githubusercontent.com/keyuxing/tpfi/main/examples/tutorial.ipynb) for more details.
 
 ## Contributing
 
 If you would like to contribute to this project, feel free to submit a pull request 
 or open an issue on GitHub. Any suggestion, improvement, or bug report is welcomed.
 
 ## License
 
 This project is licensed under the MIT License - see the 
-[LICENSE](https://github.com/keyuxing/tpfi/blob/main/LICENSE) file for details.
+[LICENSE](https://raw.githubusercontent.com/keyuxing/tpfi/main/LICENSE) file for details.
```

### Comparing `tpfi-1.0.4/src/tpfi/tpfi.py` & `tpfi-1.0.5/src/tpfi/tpfi.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,32 +7,28 @@
 from astropy import units as u
 from astropy.coordinates import SkyCoord
 from astropy.table import QTable, Table
 from astropy.time import Time
 from astropy.visualization import SqrtStretch
 from astropy.visualization.mpl_normalize import imshow_norm
 from astroquery.gaia import Gaia
-from astroquery.simbad import Simbad
 from erfa import ErfaWarning
-from lightkurve import LightkurveWarning, TessTargetPixelFile, KeplerTargetPixelFile
+from lightkurve import KeplerTargetPixelFile, LightkurveWarning, TessTargetPixelFile
 from matplotlib import patches
 from matplotlib import pyplot as plt
 from matplotlib.axes import Axes
 from matplotlib.colorbar import Colorbar
 from matplotlib.offsetbox import AnchoredText
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
 from .utils import add_orientation, add_scalebar, calculate_theta, query_sky_img
 
 Gaia.MAIN_GAIA_TABLE = "gaiadr3.gaia_source"
 Gaia.ROW_LIMIT = -1
 
-CUSTOM_SIMBAD = Simbad()
-CUSTOM_SIMBAD.add_votable_fields("ids")
-
 REF_EPOCH = Time("J2016")
 
 logging.getLogger("astroquery").setLevel(logging.WARNING)
 
 
 def query_nearby_gaia_objects(
     tpf: Union[TessTargetPixelFile, KeplerTargetPixelFile], verbose: bool
@@ -71,15 +67,15 @@
             coords = coords_j2000.apply_space_motion(new_obstime=REF_EPOCH)
     else:
         coords = SkyCoord(ra, dec, frame="icrs")
 
     j = Gaia.cone_search_async(coords, radius, columns=["source_id", "phot_g_mean_mag", "ra", "dec", "pmra", "pmdec"])
     r = j.get_results()
 
-    if not (r["dist"] < 3).any():
+    if not (r["dist"] < 3 / 3600).any():
         if verbose:
             print("Target not found in Gaia DR3")
         return None
     else:
         if verbose:
             print(f"Target Gaia Source DR3 ID: {r[0]['source_id']}")
         return r
@@ -200,14 +196,15 @@
     ax_tpf.invert_xaxis()
 
     if r is None:
         at = AnchoredText("No Gaia DR3 Data", frameon=False, loc="upper left", prop=dict(size=13))
         ax_tpf.add_artist(at)
     else:
         target_gaia_id = r[0]["source_id"]
+        print(r)
         r.sort("phot_g_mean_mag")
         this = np.nonzero(r["source_id"] == target_gaia_id)[0][0]
         magnitude_limit = max(r["phot_g_mean_mag"][0] + 3, mag_limit)
         r = r[r["phot_g_mean_mag"] < magnitude_limit][: max(this + 50, 300)]
 
         qr = QTable([r["ra"].filled(), r["dec"].filled(), r["pmra"].filled(0), r["pmdec"].filled(0)])
         coords_gaia = SkyCoord(
@@ -407,15 +404,15 @@
     percent_array = np.full(4, np.nan)
     for i, tpf in enumerate(tpf_list):
         if tpf is not None:
             percent_array[i] = int(tpf.shape[2] / tpf_list[max_index].shape[2] * 100)
     percent_array = np.nan_to_num(percent_array, nan=np.nanmedian(percent_array))
 
     ax_list = []
-    for i, percent in enumerate(percent_array):
+    for percent in percent_array:
         ax_list.append(divider.append_axes("right", size=f"{percent}%", pad=0.1))
 
     plot_sky(ax, tpf_list[max_index], show_label, verbose)
 
     r = query_nearby_gaia_objects(tpf_list[max_index], verbose=verbose)
     for i, tpf in enumerate(tpf_list):
         if tpf is not None:
```

### Comparing `tpfi-1.0.4/src/tpfi/utils.py` & `tpfi-1.0.5/src/tpfi/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Tuple, Union
 
 import numpy as np
 from astropy import units as u
 from astropy.coordinates import Angle
 from astropy.wcs import Wcsprm
 from astroquery.hips2fits import hips2fits
-from lightkurve import TessTargetPixelFile, KeplerTargetPixelFile
+from lightkurve import KeplerTargetPixelFile, TessTargetPixelFile
 from matplotlib.axes import Axes
 
 
 def calculate_theta(w: Wcsprm) -> Tuple[float, bool]:
     """
     Calculates the rotation angle of TPF according to the wcs in the FITS Header.
```

### Comparing `tpfi-1.0.4/PKG-INFO` & `tpfi-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpfi
-Version: 1.0.4
+Version: 1.0.5
 Summary: Plot identification charts for Kepler, K2 and TESS.
 Home-page: https://github.com/keyuxing/tpfi
 License: MIT
 Author: Keyu Xing
 Author-email: kyxing@mail.bnu.edu.cn
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -60,18 +60,18 @@
 You can install this package using `pip`:
 ```shell
 pip install tpfi
 ```
 
 ## How to use
 
-See the [example notebook](https://github.com/keyuxing/tpfi/blob/main/examples/tutorial.ipynb) for more details.
+See the [example notebook](https://raw.githubusercontent.com/keyuxing/tpfi/main/examples/tutorial.ipynb) for more details.
 
 ## Contributing
 
 If you would like to contribute to this project, feel free to submit a pull request 
 or open an issue on GitHub. Any suggestion, improvement, or bug report is welcomed.
 
 ## License
 
 This project is licensed under the MIT License - see the 
-[LICENSE](https://github.com/keyuxing/tpfi/blob/main/LICENSE) file for details.
+[LICENSE](https://raw.githubusercontent.com/keyuxing/tpfi/main/LICENSE) file for details.
```

