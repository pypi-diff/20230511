# Comparing `tmp/freepaths-1.2.1.tar.gz` & `tmp/freepaths-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freepaths-1.2.1.tar", last modified: Thu Feb  2 08:18:46 2023, max compression
+gzip compressed data, was "freepaths-1.3.tar", last modified: Thu May 11 08:56:37 2023, max compression
```

## Comparing `freepaths-1.2.1.tar` & `freepaths-1.3.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-02-02 08:18:45.000000 freepaths-1.2.1/
--rw-r--r--   0 r         (1000) r         (1000)     5597 2023-02-02 08:18:46.000000 freepaths-1.2.1/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)     4839 2023-02-02 07:39:23.000000 freepaths-1.2.1/README.md
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-02-02 08:18:45.000000 freepaths-1.2.1/freepaths/
--rw-r--r--   0 r         (1000) r         (1000)      871 2023-02-02 07:27:43.000000 freepaths-1.2.1/freepaths/__main__.py
--rw-r--r--   0 r         (1000) r         (1000)     3102 2023-02-02 07:21:25.000000 freepaths-1.2.1/freepaths/animation.py
--rw-r--r--   0 r         (1000) r         (1000)     6040 2023-02-02 07:21:34.000000 freepaths-1.2.1/freepaths/config.py
--rw-r--r--   0 r         (1000) r         (1000)     8000 2023-01-25 07:44:50.000000 freepaths-1.2.1/freepaths/data.py
--rw-r--r--   0 r         (1000) r         (1000)     2455 2023-02-02 07:18:16.000000 freepaths-1.2.1/freepaths/default_config.py
--rw-r--r--   0 r         (1000) r         (1000)     2650 2023-02-01 09:15:48.000000 freepaths-1.2.1/freepaths/flight.py
--rw-r--r--   0 r         (1000) r         (1000)     4392 2023-02-02 08:16:31.000000 freepaths-1.2.1/freepaths/main_mfp_sampling.py
--rw-r--r--   0 r         (1000) r         (1000)     3390 2023-02-02 08:16:00.000000 freepaths-1.2.1/freepaths/main_tracing.py
--rw-r--r--   0 r         (1000) r         (1000)     8647 2023-01-25 08:49:48.000000 freepaths-1.2.1/freepaths/maps.py
--rw-r--r--   0 r         (1000) r         (1000)     3797 2023-01-25 08:49:48.000000 freepaths-1.2.1/freepaths/materials.py
--rw-r--r--   0 r         (1000) r         (1000)      733 2023-01-24 09:26:17.000000 freepaths-1.2.1/freepaths/move.py
--rw-r--r--   0 r         (1000) r         (1000)      457 2023-01-26 04:13:24.000000 freepaths-1.2.1/freepaths/options.py
--rw-r--r--   0 r         (1000) r         (1000)     4837 2023-01-25 08:49:48.000000 freepaths-1.2.1/freepaths/output_info.py
--rw-r--r--   0 r         (1000) r         (1000)    14806 2023-02-01 11:04:45.000000 freepaths-1.2.1/freepaths/output_plots.py
--rw-r--r--   0 r         (1000) r         (1000)     7754 2023-01-26 05:12:52.000000 freepaths-1.2.1/freepaths/phonon.py
--rw-r--r--   0 r         (1000) r         (1000)      580 2023-01-24 09:16:58.000000 freepaths-1.2.1/freepaths/progress.py
--rw-r--r--   0 r         (1000) r         (1000)     2312 2023-02-01 09:16:26.000000 freepaths-1.2.1/freepaths/run_phonon.py
--rw-r--r--   0 r         (1000) r         (1000)    23457 2023-01-26 05:12:54.000000 freepaths-1.2.1/freepaths/scattering.py
--rw-r--r--   0 r         (1000) r         (1000)     1550 2023-01-25 08:51:17.000000 freepaths-1.2.1/freepaths/scattering_types.py
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-02-02 08:18:45.000000 freepaths-1.2.1/freepaths.egg-info/
--rw-r--r--   0 r         (1000) r         (1000)     5597 2023-02-02 08:18:46.000000 freepaths-1.2.1/freepaths.egg-info/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)      672 2023-02-02 08:18:46.000000 freepaths-1.2.1/freepaths.egg-info/SOURCES.txt
--rw-r--r--   0 r         (1000) r         (1000)        1 2023-02-02 08:18:46.000000 freepaths-1.2.1/freepaths.egg-info/dependency_links.txt
--rw-r--r--   0 r         (1000) r         (1000)       53 2023-02-02 08:18:46.000000 freepaths-1.2.1/freepaths.egg-info/entry_points.txt
--rw-r--r--   0 r         (1000) r         (1000)       31 2023-02-02 08:18:46.000000 freepaths-1.2.1/freepaths.egg-info/requires.txt
--rw-r--r--   0 r         (1000) r         (1000)       10 2023-02-02 08:18:46.000000 freepaths-1.2.1/freepaths.egg-info/top_level.txt
--rw-r--r--   0 r         (1000) r         (1000)       91 2022-11-27 00:35:48.000000 freepaths-1.2.1/pyproject.toml
--rw-r--r--   0 r         (1000) r         (1000)       38 2023-02-02 08:18:46.000000 freepaths-1.2.1/setup.cfg
--rw-r--r--   0 r         (1000) r         (1000)     1439 2023-02-01 12:39:12.000000 freepaths-1.2.1/setup.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-11 08:56:37.149307 freepaths-1.3/
+-rw-r--r--   0 r         (1000) r         (1000)     5298 2023-05-11 08:56:37.149307 freepaths-1.3/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)     4542 2023-02-22 13:18:35.000000 freepaths-1.3/README.md
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-11 08:56:37.149307 freepaths-1.3/freepaths/
+-rw-r--r--   0 r         (1000) r         (1000)      869 2023-05-11 07:21:33.000000 freepaths-1.3/freepaths/__main__.py
+-rw-r--r--   0 r         (1000) r         (1000)     3677 2023-05-11 08:30:00.000000 freepaths-1.3/freepaths/animation.py
+-rw-r--r--   0 r         (1000) r         (1000)     8051 2023-05-11 07:22:21.000000 freepaths-1.3/freepaths/config.py
+-rw-r--r--   0 r         (1000) r         (1000)     8022 2023-05-11 07:22:40.000000 freepaths-1.3/freepaths/data.py
+-rw-r--r--   0 r         (1000) r         (1000)     2747 2023-05-11 07:15:01.000000 freepaths-1.3/freepaths/default_config.py
+-rw-r--r--   0 r         (1000) r         (1000)     2650 2023-02-01 09:15:48.000000 freepaths-1.3/freepaths/flight.py
+-rw-r--r--   0 r         (1000) r         (1000)     4366 2023-02-03 02:30:26.000000 freepaths-1.3/freepaths/main_mfp_sampling.py
+-rw-r--r--   0 r         (1000) r         (1000)     3330 2023-05-11 07:20:52.000000 freepaths-1.3/freepaths/main_tracing.py
+-rw-r--r--   0 r         (1000) r         (1000)     8647 2023-01-25 08:49:48.000000 freepaths-1.3/freepaths/maps.py
+-rw-r--r--   0 r         (1000) r         (1000)     3797 2023-01-25 08:49:48.000000 freepaths-1.3/freepaths/materials.py
+-rw-r--r--   0 r         (1000) r         (1000)      733 2023-01-24 09:26:17.000000 freepaths-1.3/freepaths/move.py
+-rw-r--r--   0 r         (1000) r         (1000)      663 2023-05-11 06:25:40.000000 freepaths-1.3/freepaths/options.py
+-rw-r--r--   0 r         (1000) r         (1000)     4837 2023-01-25 08:49:48.000000 freepaths-1.3/freepaths/output_info.py
+-rw-r--r--   0 r         (1000) r         (1000)    15058 2023-05-11 06:36:24.000000 freepaths-1.3/freepaths/output_plots.py
+-rw-r--r--   0 r         (1000) r         (1000)     2348 2023-02-03 08:43:58.000000 freepaths-1.3/freepaths/output_structure.py
+-rw-r--r--   0 r         (1000) r         (1000)     8569 2023-05-11 06:25:46.000000 freepaths-1.3/freepaths/phonon.py
+-rw-r--r--   0 r         (1000) r         (1000)      580 2023-01-24 09:16:58.000000 freepaths-1.3/freepaths/progress.py
+-rw-r--r--   0 r         (1000) r         (1000)     2312 2023-05-11 06:31:01.000000 freepaths-1.3/freepaths/run_phonon.py
+-rw-r--r--   0 r         (1000) r         (1000)    27604 2023-05-11 06:25:47.000000 freepaths-1.3/freepaths/scattering.py
+-rw-r--r--   0 r         (1000) r         (1000)     1550 2023-01-25 08:51:17.000000 freepaths-1.3/freepaths/scattering_types.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-05-11 08:56:37.149307 freepaths-1.3/freepaths.egg-info/
+-rw-r--r--   0 r         (1000) r         (1000)     5298 2023-05-11 08:56:37.000000 freepaths-1.3/freepaths.egg-info/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)      702 2023-05-11 08:56:37.000000 freepaths-1.3/freepaths.egg-info/SOURCES.txt
+-rw-r--r--   0 r         (1000) r         (1000)        1 2023-05-11 08:56:37.000000 freepaths-1.3/freepaths.egg-info/dependency_links.txt
+-rw-r--r--   0 r         (1000) r         (1000)       53 2023-05-11 08:56:37.000000 freepaths-1.3/freepaths.egg-info/entry_points.txt
+-rw-r--r--   0 r         (1000) r         (1000)       31 2023-05-11 08:56:37.000000 freepaths-1.3/freepaths.egg-info/requires.txt
+-rw-r--r--   0 r         (1000) r         (1000)       10 2023-05-11 08:56:37.000000 freepaths-1.3/freepaths.egg-info/top_level.txt
+-rw-r--r--   0 r         (1000) r         (1000)       91 2022-11-27 00:35:48.000000 freepaths-1.3/pyproject.toml
+-rw-r--r--   0 r         (1000) r         (1000)       38 2023-05-11 08:56:37.149307 freepaths-1.3/setup.cfg
+-rw-r--r--   0 r         (1000) r         (1000)     1439 2023-02-03 05:40:49.000000 freepaths-1.3/setup.py
```

### Comparing `freepaths-1.2.1/PKG-INFO` & `freepaths-1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freepaths
-Version: 1.2.1
+Version: 1.3
 Summary: Phonon Monte Carlo simulator
 Home-page: https://github.com/anufrievroman/freepaths
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -17,48 +17,45 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 
 # FreePATHS - Free Phonon And THermal Simulator
 
-This Monte Carlo algorithm simulates trajectories of phonons in 3D models of nanostructures, which consists of a box with holes or pillars of various shapes. The algorithm outputs phonon trajectories, heat fluxes, temperature maps and profiles, the thermal conductivity, scattering maps and statistics and other information. See [the wiki pages](https://github.com/anufrievroman/Monte-Carlo/wiki/General-algorithm-flow) for the details of the simulation.
+This Monte Carlo algorithm simulates trajectories of phonons in 3D models of nanostructures, which consists of a box with holes or pillars of various shapes. The algorithm outputs phonon trajectories, heat fluxes, temperature maps and profiles, the thermal conductivity, scattering maps and statistics and other information. See [documentation](https://anufrievroman.gitbook.io/freepaths/) for the details of the simulation.
 
 ![Screenshot](https://github.com/anufrievroman/Monte-Carlo/blob/master/screenshot.png)
 
 
 ## Installation
 
-FreePATHS requires python 3. On Linux and MacOS, it is probably already installed. On Windows, you may choose to install [Anaconda](https://www.anaconda.com) package, which will install everything for you.
-
-Install the package from PyPi repository by entering this command into a terminal or a python console:
+[Installation is detailed in documentation](https://anufrievroman.gitbook.io/freepaths/installation). In short, install the package from PyPi repository by entering this command into a terminal or a python console:
 
 `pip install --upgrade freepaths`
 
-For more details about installation, see [this wiki page](https://github.com/anufrievroman/freepaths/wiki/Installation).
 
 ## Usage
 
 FreePATHS is a command line application, so it runs inside Linux, MacOS, or Windows terminal. It takes an input file from the user, which contains all the settings, and outputs the results in a new folder.
 
 There are two modes of using the program. Main mode traces a large number of phonons through a structure and collects statistics about their paths. The MFP sampling mode measures phonon mean free paths using a small number of phonons and calculates the thermal conductivity by integrating phonon dispersion. 
 
 ### Demo
 
-First, if you simply run `freepaths` without specifying an input file, the program will run a demo simulation.
+If you simply run `freepaths` without specifying an input file, the program will run a demo simulation.
 
 ### Main mode
 
 In the main mode, the program traces large number of phonons through a structure and calculates various statistical distributions and maps. In this mode, the thermal conductivity will be calculated via Fourier law. Note that the thermal conductivity will be correct only in the absence of holes.
 
 Run the program as:
 
 `freepaths your_input_file.py`
 
-See [wiki page](https://github.com/anufrievroman/freepaths/wiki/Creating-input-files) for explanations about creating your own input files. In the [examples](https://github.com/anufrievroman/freepaths/tree/master/examples) folder, you will find examples of various input files. Try using one of them, for instance as:
+See [documentation](https://anufrievroman.gitbook.io/freepaths/examples) for explanations about creating your own input files. In the [examples](https://github.com/anufrievroman/freepaths/tree/master/examples) folder, you will find examples of various input files. Try using one of them, for instance as:
 
 `freepaths simple_nanowire.py`
 
 After the simulation, see the results in a newly created **Results** folder.
 
 
 ### MFP sampling mode
@@ -68,21 +65,21 @@
 `freepaths -s simple_nanowire.py`
 
 The calculated thermal conductivity will be output in the terminal. However, other statistical quantities and plots will still be calculated and output in the `Results` folder.
 
 
 ## Troubleshooting
 
-- [Troubles with installation](https://github.com/anufrievroman/freepaths/wiki/Installation)
-- [Troubles with usage](https://github.com/anufrievroman/freepaths/wiki/Usage)
+- [Troubles with installation](https://anufrievroman.gitbook.io/freepaths/installation)
+- [Troubles with usage](https://anufrievroman.gitbook.io/freepaths/usage)
 
 
 ## Disclaimer
 
-The code is still in development and provided as is. It likely contains bugs or might be inappropriate for your research. It is your responsibility to understand the underlying physics, test the code, and verify that all the equations and the code are correct. See [the wiki pages](https://github.com/anufrievroman/Monte-Carlo/wiki/General-algorithm-flow) and the references below for more details on the code.
+The code is still in development and provided as is. It likely contains bugs or might be inappropriate for your research. It is your responsibility to understand the underlying physics, test the code, and verify that all the equations and the code are correct. See [documentation](https://anufrievroman.gitbook.io/freepaths/algorithm) and the references below for more details on the code.
 
 
 ## References and acknowledgments
 
 The code has been developed by [Roman Anufriev](https://anufrievroman.com) in [Nomura lab](https://www.nlab.iis.u-tokyo.ac.jp/index-e.html) at the University of Tokyo in 2018-2022.
 If you would like to use this code for your research, please see the disclaimer above and consider citing the papers below, if it is appropriate.
 Details of the code and examples of the output can be found in the following papers:
```

### Comparing `freepaths-1.2.1/README.md` & `freepaths-1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 # FreePATHS - Free Phonon And THermal Simulator
 
-This Monte Carlo algorithm simulates trajectories of phonons in 3D models of nanostructures, which consists of a box with holes or pillars of various shapes. The algorithm outputs phonon trajectories, heat fluxes, temperature maps and profiles, the thermal conductivity, scattering maps and statistics and other information. See [the wiki pages](https://github.com/anufrievroman/Monte-Carlo/wiki/General-algorithm-flow) for the details of the simulation.
+This Monte Carlo algorithm simulates trajectories of phonons in 3D models of nanostructures, which consists of a box with holes or pillars of various shapes. The algorithm outputs phonon trajectories, heat fluxes, temperature maps and profiles, the thermal conductivity, scattering maps and statistics and other information. See [documentation](https://anufrievroman.gitbook.io/freepaths/) for the details of the simulation.
 
 ![Screenshot](https://github.com/anufrievroman/Monte-Carlo/blob/master/screenshot.png)
 
 
 ## Installation
 
-FreePATHS requires python 3. On Linux and MacOS, it is probably already installed. On Windows, you may choose to install [Anaconda](https://www.anaconda.com) package, which will install everything for you.
-
-Install the package from PyPi repository by entering this command into a terminal or a python console:
+[Installation is detailed in documentation](https://anufrievroman.gitbook.io/freepaths/installation). In short, install the package from PyPi repository by entering this command into a terminal or a python console:
 
 `pip install --upgrade freepaths`
 
-For more details about installation, see [this wiki page](https://github.com/anufrievroman/freepaths/wiki/Installation).
 
 ## Usage
 
 FreePATHS is a command line application, so it runs inside Linux, MacOS, or Windows terminal. It takes an input file from the user, which contains all the settings, and outputs the results in a new folder.
 
 There are two modes of using the program. Main mode traces a large number of phonons through a structure and collects statistics about their paths. The MFP sampling mode measures phonon mean free paths using a small number of phonons and calculates the thermal conductivity by integrating phonon dispersion. 
 
 ### Demo
 
-First, if you simply run `freepaths` without specifying an input file, the program will run a demo simulation.
+If you simply run `freepaths` without specifying an input file, the program will run a demo simulation.
 
 ### Main mode
 
 In the main mode, the program traces large number of phonons through a structure and calculates various statistical distributions and maps. In this mode, the thermal conductivity will be calculated via Fourier law. Note that the thermal conductivity will be correct only in the absence of holes.
 
 Run the program as:
 
 `freepaths your_input_file.py`
 
-See [wiki page](https://github.com/anufrievroman/freepaths/wiki/Creating-input-files) for explanations about creating your own input files. In the [examples](https://github.com/anufrievroman/freepaths/tree/master/examples) folder, you will find examples of various input files. Try using one of them, for instance as:
+See [documentation](https://anufrievroman.gitbook.io/freepaths/examples) for explanations about creating your own input files. In the [examples](https://github.com/anufrievroman/freepaths/tree/master/examples) folder, you will find examples of various input files. Try using one of them, for instance as:
 
 `freepaths simple_nanowire.py`
 
 After the simulation, see the results in a newly created **Results** folder.
 
 
 ### MFP sampling mode
@@ -47,21 +44,21 @@
 `freepaths -s simple_nanowire.py`
 
 The calculated thermal conductivity will be output in the terminal. However, other statistical quantities and plots will still be calculated and output in the `Results` folder.
 
 
 ## Troubleshooting
 
-- [Troubles with installation](https://github.com/anufrievroman/freepaths/wiki/Installation)
-- [Troubles with usage](https://github.com/anufrievroman/freepaths/wiki/Usage)
+- [Troubles with installation](https://anufrievroman.gitbook.io/freepaths/installation)
+- [Troubles with usage](https://anufrievroman.gitbook.io/freepaths/usage)
 
 
 ## Disclaimer
 
-The code is still in development and provided as is. It likely contains bugs or might be inappropriate for your research. It is your responsibility to understand the underlying physics, test the code, and verify that all the equations and the code are correct. See [the wiki pages](https://github.com/anufrievroman/Monte-Carlo/wiki/General-algorithm-flow) and the references below for more details on the code.
+The code is still in development and provided as is. It likely contains bugs or might be inappropriate for your research. It is your responsibility to understand the underlying physics, test the code, and verify that all the equations and the code are correct. See [documentation](https://anufrievroman.gitbook.io/freepaths/algorithm) and the references below for more details on the code.
 
 
 ## References and acknowledgments
 
 The code has been developed by [Roman Anufriev](https://anufrievroman.com) in [Nomura lab](https://www.nlab.iis.u-tokyo.ac.jp/index-e.html) at the University of Tokyo in 2018-2022.
 If you would like to use this code for your research, please see the disclaimer above and consider citing the papers below, if it is appropriate.
 Details of the code and examples of the output can be found in the following papers:
```

### Comparing `freepaths-1.2.1/freepaths/__main__.py` & `freepaths-1.3/freepaths/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """FreePATHS - Free Phonon and THermal Simulator"""
 
 import argparse
 
 import freepaths.main_tracing
 import freepaths.main_mfp_sampling
 
-__version__ = "1.2.1"
+__version__ = "1.3"
 
 # Parse user arguments:
 parser = argparse.ArgumentParser(
                 prog = 'FreePATHS',
                 description = 'Monte Carlo simulator',
-                epilog = 'For more information, visit: https://github.com/anufrievroman/freepaths'
+                epilog = 'For more information, visit: https://anufrievroman.gitbook.io/freepaths'
                 )
 parser.add_argument('input_file', nargs='?', default=None, help='The input file')
 parser.add_argument("-s", "--sampling", help="Run in MFP sampling mode", action="store_true")
 args = parser.parse_args()
 
 
 def run():
```

### Comparing `freepaths-1.2.1/freepaths/animation.py` & `freepaths-1.3/freepaths/animation.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,81 +4,103 @@
 import os
 import shutil
 import imageio
 import numpy as np
 import matplotlib.pyplot as plt
 
 from freepaths.config import cf
+from freepaths.output_structure import draw_structure
 
 
 def generate_frames_xy():
     """Generate animation frames with phonon paths"""
 
     data = np.genfromtxt("Data/Phonon paths.csv",
                          unpack=False,
                          delimiter=',',
                          skip_header=1,
                          encoding='utf-8')
 
-
     # Create XY plots for each timestep where all phonon shown at the same time:
     number_of_steps = np.shape(data)[0]
     number_of_phonons = np.shape(data)[1]//3
+
     for step in range(1, number_of_steps):
         fig, ax = plt.subplots()
+
+        # Draw the structure:
+        patches = draw_structure(cf)
+        for patch in patches:
+            ax.add_patch(patch)
+
+        # Draw the paths:
         for phonon_num in range(number_of_phonons):
             x_coords = np.trim_zeros(data[:, 3 * phonon_num], trim='b')
             y_coords = np.trim_zeros(data[:, 3 * phonon_num + 1], trim='b')
             ax.plot(x_coords[:step], y_coords[:step], linewidth=0.5)
-        ax.set_xlabel('X (μm)', fontsize=12)
-        ax.set_ylabel('Y (μm)', fontsize=12)
+
+        # Plot settings:
         ax.set_xlim([-0.55*cf.width*1e6, 0.55*cf.width*1e6])
         ax.set_ylim([0, cf.length*1e6])
-        ax.tick_params(axis="y",direction="out")
-        ax.tick_params(axis="x",direction="out")
         ax.set_aspect('equal')
+        ax.axis('off')
+        for spine in ['top', 'right', 'left', 'bottom']:
+            ax.spines[spine].set_visible(False)
         fig.savefig(f"Frames/frame_{step:0>6}.png", dpi=600, bbox_inches="tight")
         plt.close(fig)
 
+        # Progress:
+        sys.stdout.write(f"\rAnimation: {step}/{number_of_steps - 1} frames")
+
     # Create XY plots for each step for each phonon one by one:
     # cmap = plt.get_cmap("tab10")
     # frame_number = 0
     # number_of_phonons = np.shape(data)[1]//3
     # for phonon_num in range(number_of_phonons):
         # x_coords = np.trim_zeros(data[:, 3 * phonon_num], trim='b')
         # y_coords = np.trim_zeros(data[:, 3 * phonon_num + 1], trim='b')
         # steps = np.shape(x_coords)[0]
         # for step in range(1, steps):
             # fig, ax = plt.subplots()
             # ax.plot(x_coords[:step], y_coords[:step], color=cmap(phonon_num), linewidth=0.5)
-            # ax.set_xlabel('X (μm)', fontsize=12)
-            # ax.set_ylabel('Y (μm)', fontsize=12)
+            # ax.axis('off')
+            # for spine in ['top', 'right', 'left', 'bottom']:
+                # ax.spines[spine].set_visible(False)
             # ax.set_xlim([-0.55*cf.width*1e6, 0.55*cf.width*1e6])
             # ax.set_ylim([0, cf.length*1e6])
-            # ax.tick_params(axis="y",direction="out")
-            # ax.tick_params(axis="x",direction="out")
             # ax.set_aspect('equal')
             # fig.savefig(f"Frames/frame_{frame_number:0>6}.png", dpi=600, bbox_inches="tight")
             # plt.close(fig)
             # frame_number += 1
 
 
 def generate_animation_xy():
     """Generate animation of phonon path in XY plane"""
+    sys.stdout.write(f"\rAnimation: creating animation file")
     images = []
     filenames = os.listdir("Frames/")
     for filename in filenames:
         images.append(imageio.imread(f"Frames/{filename}"))
-    imageio.mimsave("Animated paths XY.gif", images)
+
+    # Create a GIF file:
+    imageio.mimsave("Animated paths XY.gif", images,
+                    fps=cf.output_animation_fps, subrectangles=True)
+
+    # Create an MP4 file:
+    # writer = imageio.get_writer('Animated paths XY.mp4', fps=cf.output_animation_fps)
+
+    # for im in images:
+        # writer.append_data(imageio.imread(im))
+    # writer.close()
 
 
 def delete_frames():
     """Delete frames after creating the animation"""
     folder_path = "Frames/"
     shutil.rmtree(folder_path)
 
 
 def create_animation():
     """Main function that creates the animation"""
     generate_frames_xy()
     generate_animation_xy()
-    delete_frames()
+    # delete_frames()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `freepaths-1.2.1/freepaths/config.py` & `freepaths-1.3/freepaths/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-"""Module that reads the user input file, privides default values, and converts the variables into enums"""
+"""Module that reads the user input file, provides default values, and converts the variables into enums"""
 
 import sys
 import argparse
 
 from freepaths.options import Materials, Distributions, Positions
 
 # Import a default input file:
 from freepaths.default_config import *
 
 
 # Parse user arguments:
-WEBSITE = 'https://github.com/anufrievroman/freepaths'
+WEBSITE = 'https://anufrievroman.gitbook.io/freepaths'
 parser = argparse.ArgumentParser(prog='FreePATHS', description='Monte Carlo simulator',
                                  epilog=f'For more information, visit: {WEBSITE}')
 parser.add_argument('input_file', nargs='?', default=None, help='The input file')
 parser.add_argument("-s", "--sampling", help="Run in MFP sampling mode", action="store_true")
 args = parser.parse_args()
 
 
 # If a file is provided, overwrite the default values:
 if args.input_file:
-    exec(open(args.input_file).read(), globals())
+    exec(open(args.input_file, encoding='utf-8').read(), globals())
 else:
-    print("You didn't provide any input file, so we run a demo simulation:\n")
+    print("You didn't provide any input file, so let's run a demo simulation!\n")
 
 
 class Config:
     """Class that contains all the settings for the simulation"""
 
     def __init__(self):
         """Initiate all the parameters from global variables"""
@@ -37,19 +37,23 @@
         self.number_of_timesteps = NUMBER_OF_TIMESTEPS
         self.number_of_nodes = NUMBER_OF_NODES
         self.timestep = TIMESTEP
         self.temp = T
         self.plots_in_terminal = PLOTS_IN_TERMINAL
         self.output_scattering_map = OUTPUT_SCATTERING_MAP
         self.output_raw_thermal_map = OUTPUT_RAW_THERMAL_MAP
-        self.output_path_animation = OUTPUT_PATH_ANIMATION
         self.output_trajectories_of_first = OUTPUT_TRAJECTORIES_OF_FIRST
+        self.output_structure_color = OUTPUT_STRUCTURE_COLOR
         self.number_of_length_segments = NUMBER_OF_LENGTH_SEGMENTS
         self.hot_side_angle_distribution = HOT_SIDE_ANGLE_DISTRIBUTION
 
+        # Animation:
+        self.output_path_animation = OUTPUT_PATH_ANIMATION
+        self.output_animation_fps = OUTPUT_ANIMATION_FPS
+
         # Map & profiles parameters:
         self.number_of_pixels_x = NUMBER_OF_PIXELS_X
         self.number_of_pixels_y = NUMBER_OF_PIXELS_Y
         self.number_of_timeframes = NUMBER_OF_TIMEFRAMES
 
         # Material parameters:
         self.media = MEDIA
@@ -60,18 +64,23 @@
         self.use_gray_approximation_mfp = USE_GRAY_APPROXIMATION_MFP
         self.gray_approximation_mfp = GRAY_APPROXIMATION_MFP
 
         # System dimensions:
         self.thickness = THICKNESS
         self.width = WIDTH
         self.length = LENGTH
+        self.include_right_sidewall = INCLUDE_RIGHT_SIDEWALL
+        self.include_left_sidewall = INCLUDE_LEFT_SIDEWALL
+        self.include_top_sidewall = INCLUDE_TOP_SIDEWALL
+        self.include_bottom_sidewall = INCLUDE_BOTTOM_SIDEWALL
 
         # Hot and cold sides:
         self.frequency_detector_size = FREQUENCY_DETECTOR_SIZE
         self.cold_side_position = COLD_SIDE_POSITION
+        self.hot_side_position = HOT_SIDE_POSITION
         self.hot_side_x = HOT_SIDE_X
         self.hot_side_y = HOT_SIDE_Y
         self.hot_side_width_x = HOT_SIDE_WIDTH_X
         self.hot_side_width_y = HOT_SIDE_WIDTH_Y
 
         # Roughness:
         self.side_wall_roughness = SIDE_WALL_ROUGHNESS
@@ -103,53 +112,87 @@
 
         # Pillar array parameters [m]
         self.include_pillars = INCLUDE_PILLARS
         self.pillar_coordinates = PILLAR_COORDINATES
         self.pillar_height = PILLAR_HEIGHT
         self.pillar_wall_angle = PILLAR_WALL_ANGLE
 
+
     def convert_to_enums(self):
         """Convert some user generated parameters into enums"""
-        if self.hot_side_angle_distribution in ["random", "lambert", "directional", "uniform"]:
+
+        # Distributions:
+        valid_distributions =[member.name.lower() for member in Distributions]
+        if self.hot_side_angle_distribution in valid_distributions:
             self.hot_side_angle_distribution = Distributions[self.hot_side_angle_distribution.upper()]
         else:
-            print("ERROR: Parameter HOT_SIDE_ANGLE_DISTRIBUTION is not set correctly.\n")
+            print("ERROR: Parameter HOT_SIDE_ANGLE_DISTRIBUTION is not set correctly.")
+            print("HOT_SIDE_ANGLE_DISTRIBUTION should be one of the following:")
+            print(*valid_distributions, sep = ", ")
             sys.exit()
 
-        if self.media in ["Si", "SiC", "Diamond", "AlN"]:
+        # Materials:
+        valid_materials = [member.name for member in Materials]
+        if self.media in valid_materials:
             self.media = Materials[self.media]
         else:
-            print(f"ERROR: Material {self.media} is not in the database.\n")
+            print(f"ERROR: Material {self.media} is not in the database.")
+            print("MEDIA should be one of the following:")
+            print(*valid_materials, sep = ", ")
             sys.exit()
 
-        if self.cold_side_position in ["top", "top_and_right", "top_and_bottom", "right"]:
+        # Positions:
+        valid_positions = [member.name.lower() for member in Positions]
+        if self.cold_side_position in valid_positions:
             self.cold_side_position = Positions[self.cold_side_position.upper()]
         else:
-            print("ERROR: Parameter COLD_SIDE_POSITION is not set correctly.\n")
+            print("ERROR: Parameter COLD_SIDE_POSITION is not set correctly.")
+            print("COLD_SIDE_POSITION should be one of the following:")
+            print(*valid_positions, sep = ", ")
+            sys.exit()
+
+        if self.hot_side_position in valid_positions:
+            self.hot_side_position = Positions[self.hot_side_position.upper()]
+        else:
+            print("ERROR: Parameter HOT_SIDE_POSITION is not set correctly.")
+            print("HOT_SIDE_POSITION should be one of the following:")
+            print(*valid_positions, sep = ", ")
             sys.exit()
 
+
     def check_parameter_validity(self):
-        """Check if some parameteres are valid"""
+        """Check if various parameters are valid"""
         if self.number_of_phonons < self.output_trajectories_of_first:
-            print("ERROR: Parameter OUTPUT_TRAJECTORIES_OF_FIRST exceeds NUMBER_OF_PHONONS.\n")
-            sys.exit()
+            self.output_trajectories_of_first = self.number_of_phonons
+            print("WARNING: Parameter OUTPUT_TRAJECTORIES_OF_FIRST exceeded NUMBER_OF_PHONONS.\n")
 
         if self.hot_side_y > self.length:
-            print("ERROR: Parameter HOT_SIDE_Y exceeds LENGHT.\n")
-            sys.exit()
+            self.hot_side_y = self.length
+            print("WARNING: Parameter HOT_SIDE_Y exceeded LENGHT.\n")
 
         if self.hot_side_y < 0:
-            print("ERROR: Parameter HOT_SIDE_Y is negative.\n")
-            sys.exit()
+            self.hot_side_y = 0
+            print("WARNING: Parameter HOT_SIDE_Y was negative.\n")
 
         if self.hot_side_y - self.hot_side_width_y / 2 < 0:
-            print("ERROR: Parameter HOT_SIDE_WIDTH_Y is too large.\n")
-            sys.exit()
+            self.hot_side_width_y = self.hot_side_y * 2
+            print("WARNING: Parameter HOT_SIDE_WIDTH_Y was too large.\n")
+
+        if self.hot_side_x > self.width/2:
+            self.hot_side_x = 0
+            print("WARNING: Parameter HOT_SIDE_X was larger than WIDTH.\n")
 
         if self.hot_side_width_x > self.width:
-            print("ERROR: Parameter HOT_SIDE_WIDTH_X exceeds WIDTH.\n")
+            self.hot_side_width_x = self.width
+            print("WARNING: Parameter HOT_SIDE_WIDTH_X exceeds WIDTH.\n")
+
+        if self.cold_side_position == self.hot_side_position:
+            print(f"ERROR: Hot and cold sides are set at {self.cold_side_position}.")
             sys.exit()
 
+        if self.output_path_animation and self.number_of_timesteps > 5000:
+            print("WARNING: NUMBER_OF_TIMESTEPS is rather large for animation.\n")
+
 
 cf = Config()
 cf.convert_to_enums()
 cf.check_parameter_validity()
```

### Comparing `freepaths-1.2.1/freepaths/data.py` & `freepaths-1.3/freepaths/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,25 +74,25 @@
 
 
 class ScatteringData:
     """Statistics of phonon scattering events"""
 
     def __init__(self):
         """Initialize arrays according to the number of segments"""
-        self.wall_diffuse = np.zeros(cf.number_of_length_segments)
-        self.wall_specular = np.zeros(cf.number_of_length_segments)
-        self.top_diffuse = np.zeros(cf.number_of_length_segments)
-        self.top_specular = np.zeros(cf.number_of_length_segments)
-        self.hole_diffuse = np.zeros(cf.number_of_length_segments)
-        self.hole_specular = np.zeros(cf.number_of_length_segments)
-        self.pillar_diffuse = np.zeros(cf.number_of_length_segments)
-        self.pillar_specular = np.zeros(cf.number_of_length_segments)
-        self.hot_side = np.zeros(cf.number_of_length_segments)
-        self.internal = np.zeros(cf.number_of_length_segments)
-        self.total = np.zeros(cf.number_of_length_segments)
+        self.wall_diffuse = np.zeros(cf.number_of_length_segments+1)
+        self.wall_specular = np.zeros(cf.number_of_length_segments+1)
+        self.top_diffuse = np.zeros(cf.number_of_length_segments+1)
+        self.top_specular = np.zeros(cf.number_of_length_segments+1)
+        self.hole_diffuse = np.zeros(cf.number_of_length_segments+1)
+        self.hole_specular = np.zeros(cf.number_of_length_segments+1)
+        self.pillar_diffuse = np.zeros(cf.number_of_length_segments+1)
+        self.pillar_specular = np.zeros(cf.number_of_length_segments+1)
+        self.hot_side = np.zeros(cf.number_of_length_segments+1)
+        self.internal = np.zeros(cf.number_of_length_segments+1)
+        self.total = np.zeros(cf.number_of_length_segments+1)
 
     def save_scattering_events(self, y, scattering_types):
         """Analyze types of scattering at the current timestep and add it to the statistics"""
 
         # Calculate in which length segment (starting from zero) we are:
         segment = int(y // (cf.length / cf.number_of_length_segments))
         self.total[segment] += 1
```

### Comparing `freepaths-1.2.1/freepaths/default_config.py` & `freepaths-1.3/freepaths/default_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,18 +8,22 @@
 NUMBER_OF_TIMESTEPS            = 60000
 NUMBER_OF_NODES                = 400
 TIMESTEP                       = 2e-12
 T                              = 300
 PLOTS_IN_TERMINAL              = False
 OUTPUT_SCATTERING_MAP          = False
 OUTPUT_RAW_THERMAL_MAP         = True
-OUTPUT_PATH_ANIMATION          = False
 OUTPUT_TRAJECTORIES_OF_FIRST   = 10
+OUTPUT_STRUCTURE_COLOR         = "#F0F0F0"
 NUMBER_OF_LENGTH_SEGMENTS      = 10
-HOT_SIDE_ANGLE_DISTRIBUTION    = "random"
+HOT_SIDE_ANGLE_DISTRIBUTION    = "random_up"
+
+# Animation:
+OUTPUT_PATH_ANIMATION          = False
+OUTPUT_ANIMATION_FPS           = 24
 
 # Map & profiles parameters:
 NUMBER_OF_PIXELS_X             = 100
 NUMBER_OF_PIXELS_Y             = 100
 NUMBER_OF_TIMEFRAMES           = 5
 
 # Material parameters:
@@ -31,18 +35,23 @@
 USE_GRAY_APPROXIMATION_MFP     = False
 GRAY_APPROXIMATION_MFP         = None
 
 # System dimensions [m]:
 THICKNESS                      = 150e-9
 WIDTH                          = 500e-9
 LENGTH                         = 2200e-9
+INCLUDE_RIGHT_SIDEWALL         = True
+INCLUDE_LEFT_SIDEWALL          = True
+INCLUDE_TOP_SIDEWALL           = False
+INCLUDE_BOTTOM_SIDEWALL        = False
 
 # Hot and cold sides [m]:
 FREQUENCY_DETECTOR_SIZE        = WIDTH
 COLD_SIDE_POSITION             = 'top'
+HOT_SIDE_POSITION              = 'bottom'
 HOT_SIDE_X                     = 0
 HOT_SIDE_WIDTH_X               = WIDTH
 HOT_SIDE_Y                     = 0
 HOT_SIDE_WIDTH_Y               = 0
 
 # Roughness [m]:
 SIDE_WALL_ROUGHNESS            = 2e-9
```

### Comparing `freepaths-1.2.1/freepaths/flight.py` & `freepaths-1.3/freepaths/flight.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.2.1/freepaths/main_mfp_sampling.py` & `freepaths-1.3/freepaths/main_mfp_sampling.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 import scipy
 import math
 
 # Modules:
 from freepaths.animation import create_animation
 from freepaths.config import cf
 from freepaths.run_phonon import run_phonon
-from freepaths.phonon import Phonon, Polarization
+from freepaths.phonon import Phonon
 from freepaths.flight import Flight
 from freepaths.data import ScatteringData, GeneralData, SegmentData, PathData
 from freepaths.progress import Progress
 from freepaths.materials import Material
 from freepaths.maps import ScatteringMap, ThermalMaps
 from freepaths.output_info import output_general_information, output_scattering_information
 from freepaths.output_plots import plot_data
+from freepaths.options import Polarizations
 
 
 def main(input_file):
     """This is the main function, which integrates phonon dispersion to get thermal conductivity"""
 
     print(f'Mean free path sampling of {cf.output_folder_name}')
     start_time = time.time()
@@ -36,15 +37,15 @@
     path_stats = PathData()
     scatter_maps = ScatteringMap()
     thermal_maps = ThermalMaps()
 
     thermal_conductivity = 0
 
     # For each polarization branch:
-    for polarization in [Polarization.LA, Polarization.TA, Polarization.TA]:
+    for polarization in [Polarizations.LA, Polarizations.TA, Polarizations.TA]:
         sys.stdout.write(f"\rIntegrating {polarization.name} branch.\n")
 
         # For each phonon:
         for index in range(cf.number_of_phonons):
 
             # Wave vector:
             k_vector = (material.dispersion[index+1, 0] + material.dispersion[index, 0]) / 2
@@ -91,15 +92,14 @@
     segment_stats.write_into_files()
     thermal_maps.write_into_files()
     scatter_maps.write_into_files()
     path_stats.write_into_files()
 
     # Generate animation of phonon paths:
     if cf.output_path_animation:
-        sys.stdout.write("\rGenerating path animation...")
         create_animation()
 
     # Analyze and plot the data:
     sys.stdout.write("\rAnalyzing the data...")
     plot_data()
 
     # Output general information:
```

### Comparing `freepaths-1.2.1/freepaths/main_tracing.py` & `freepaths-1.3/freepaths/main_tracing.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,15 +74,14 @@
     segment_stats.write_into_files()
     thermal_maps.write_into_files()
     scatter_maps.write_into_files()
     path_stats.write_into_files()
 
     # Generate animation of phonon paths:
     if cf.output_path_animation:
-        sys.stdout.write("\rGenerating path animation...")
         create_animation()
 
     # Analyze and plot the data:
     sys.stdout.write("\rAnalyzing the data...")
     plot_data()
 
     # Output general information:
```

### Comparing `freepaths-1.2.1/freepaths/maps.py` & `freepaths-1.3/freepaths/maps.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.2.1/freepaths/materials.py` & `freepaths-1.3/freepaths/materials.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.2.1/freepaths/move.py` & `freepaths-1.3/freepaths/move.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.2.1/freepaths/output_info.py` & `freepaths-1.3/freepaths/output_info.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.2.1/freepaths/output_plots.py` & `freepaths-1.3/freepaths/output_plots.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Module that calculates and outputs vaious plots and distributions from the saved files"""
 
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.colors import LogNorm
+from matplotlib.patches import Rectangle, Circle
 
 from freepaths.config import cf
+from freepaths.output_structure import draw_structure
 import matplotlib.pyplot as plt
 
 # Style of the plots:
 plt.rcParams['font.family'] = "Arial"
 plt.rcParams['axes.titlesize'] = 12
 plt.rcParams['axes.labelsize'] = 12
 plt.rcParams['lines.linewidth'] = 1.0
@@ -64,15 +66,15 @@
     """Plot distribution of angles"""
     angle_distributions = angle_distribution_calculation()
     fig, ax = plt.subplots()
     ax.plot(angle_distributions[:, 0], angle_distributions[:, 1], 'b')
     ax.plot(angle_distributions[:, 0], angle_distributions[:, 2], 'r')
     ax.set_xlabel('Angle (degree)', fontsize=12)
     ax.set_ylabel('Number of phonons', fontsize=12)
-    ax.legend(["At hot side", "At cold side"])
+    ax.legend(["At cold side", "At hot side"])
     fig.savefig("Distribution of angles.pdf", dpi=300, format='pdf', bbox_inches="tight")
     if cf.plots_in_terminal: plt.show()
     np.savetxt('Data/Distribution of angles.csv', angle_distributions, fmt='%1.3e', delimiter=",")
 
 
 def plot_free_path_distribution():
     """Plot distribution of free path"""
@@ -231,18 +233,27 @@
 def plot_trajectories():
     """Plot the phonon trajectories"""
 
     data = np.genfromtxt("Data/Phonon paths.csv", unpack=False, delimiter=',', skip_header=1, encoding='utf-8')
 
     # Create XY plot:
     fig, ax = plt.subplots()
+
+    # Draw structures:
+    patches = draw_structure(cf)
+    for patch in patches:
+        ax.add_patch(patch)
+
+    # Draw paths:
     for index in range(cf.output_trajectories_of_first):
         x_coordinates = np.trim_zeros(data[:, 3 * index], trim='b')
         y_coordinates = np.trim_zeros(data[:, 3 * index + 1], trim='b')
         ax.plot(x_coordinates, y_coordinates, linewidth=0.2)
+
+    # Set labels:
     ax.set_xlabel('X (μm)', fontsize=12)
     ax.set_ylabel('Y (μm)', fontsize=12)
     ax.set_aspect('equal', 'datalim')
     fig.savefig("Phonon paths XY.pdf", dpi=600, format='pdf', bbox_inches="tight")
     if cf.plots_in_terminal: plt.show()
 
     # Create YZ plot:
@@ -293,23 +304,23 @@
     header = header1 + header2 + header3
     data = np.vstack((segments, all_scattering_rates)).T
     np.savetxt(filename, data, fmt='%1.2e', delimiter=",", header=header)
 
 
 def plot_data():
     """Create plots of various distributions"""
+    plot_trajectories()
     plot_angle_distribution()
     plot_free_path_distribution()
     plot_frequency_distribution()
     plot_wavelength_distribution()
     plot_travel_time_distribution()
     plot_detected_frequency_distribution()
     plot_velocity_distribution()
     plot_time_in_segments()
     plot_thermal_conductivity()
     plot_temperature_profile()
     plot_heat_flux_profile()
     plot_thermal_map()
-    plot_trajectories()
     plot_scattering_statistics()
     if cf.output_scattering_map:
         plot_scattering_map()
```

### Comparing `freepaths-1.2.1/freepaths/phonon.py` & `freepaths-1.3/freepaths/phonon.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,24 +4,18 @@
 from random import random, choice
 from numpy import sign
 from scipy.constants import k, hbar
 import numpy as np
 import enum
 
 from freepaths.config import cf
-from freepaths.options import Distributions, Materials, Positions
+from freepaths.options import Distributions, Materials, Positions, Polarizations
 import freepaths.move
 
 
-class Polarization(enum.Enum):
-    """Possible polarizations of phonon"""
-    LA = 1
-    TA = 2
-
-
 class Phonon:
     """A phonon particle with various physical properties"""
 
     def __init__(self, material, polarization=None, phonon_number=None):
         """Initialize a phonon by assigning coordinates and other properties"""
         self.polarization = polarization
         self.phonon_number = phonon_number
@@ -52,38 +46,54 @@
 
     @property
     def is_in_system(self):
         """Checks if the phonon at this timestep did not reach the cold side.
         Depending on where we set the cold side, we check if phonon crossed that line"""
         small_offset = 10e-9
         if cf.cold_side_position == Positions.TOP:
-            return cf.length > self.y
+            return self.y < cf.length
+        if cf.cold_side_position == Positions.BOTTOM:
+            return self.y > 0
         if cf.cold_side_position == Positions.RIGHT:
-            return (self.y < cf.length - 1.1e-6) or (self.y > cf.length - 1.1e-6 and self.x < cf.width / 2.0 - small_offset)
-        if cf.cold_side_position == Positions.TOP_AND_RIGHT:
-            return (self.y < 1.0e-6) or (1.0e-6 < self.y < cf.length and self.x < cf.width / 2.0 - small_offset)
-        if cf.cold_side_position == Positions.TOP_AND_BOTTOM:
-            return cf.length > self.y > 0
+            # return (self.y < cf.length - 1.1e-6) or (self.y > cf.length - 1.1e-6 and self.x < cf.width / 2.0 - small_offset)
+            return self.x < cf.width / 2.0
+        if cf.cold_side_position == Positions.LEFT:
+            # return (self.y < cf.length - 1.1e-6) or (self.y > cf.length - 1.1e-6 and self.x < cf.width / 2.0 - small_offset)
+            return self.x > - cf.width / 2.0
+        # if cf.cold_side_position == Positions.TOP_AND_RIGHT:
+            # return (self.y < 1.0e-6) or (1.0e-6 < self.y < cf.length and self.x < cf.width / 2.0 - small_offset)
+        # if cf.cold_side_position == Positions.TOP_AND_BOTTOM:
+            # return cf.length > self.y > 0
         raise ValueError('Specified "cold_side" is not valid. Only TOP, RIGHT, TOP_AND_RIGH, TOP_AND_BOTTOM')
 
     def assign_polarization(self):
         """Assign branch of phonon dispersion"""
-        self.polarization = choice([Polarization.TA, Polarization.TA, Polarization.LA])
+        self.polarization = choice([Polarizations.TA, Polarizations.TA, Polarizations.LA])
 
     def assign_coordinates(self):
         """Assign initial coordinates at the hot side"""
         self.x = cf.hot_side_x + 0.49 * cf.hot_side_width_x * (2 * random() - 1)
         self.y = cf.hot_side_y + 0.49 * cf.hot_side_width_y * (2 * random() - 1)
         self.z = 0.49 * cf.thickness * (2 * random() - 1)
 
     def assign_angles(self):
         """Depending on angle distribution, assign angles"""
-        if cf.hot_side_angle_distribution == Distributions.RANDOM:
+        if cf.hot_side_angle_distribution == Distributions.RANDOM_UP:
             self.theta = -pi/2 + pi*random()
             self.phi = asin(2*random() - 1)
+        if cf.hot_side_angle_distribution == Distributions.RANDOM_DOWN:
+            rand_sign = sign((2*random() - 1))
+            self.theta = rand_sign*(pi/2 + pi/2*random())
+            self.phi = asin(2*random() - 1)
+        if cf.hot_side_angle_distribution == Distributions.RANDOM_RIGHT:
+            self.theta = pi*random()
+            self.phi = asin(2*random() - 1)
+        if cf.hot_side_angle_distribution == Distributions.RANDOM_LEFT:
+            self.theta = - pi*random()
+            self.phi = asin(2*random() - 1)
         if cf.hot_side_angle_distribution == Distributions.DIRECTIONAL:
             self.theta = 0
             self.phi = -pi/2 + pi*random()
         if cf.hot_side_angle_distribution == Distributions.LAMBERT:
             self.theta = asin(2*random() - 1)
             self.phi = asin((asin(2*random() - 1))/(pi/2))
         if cf.hot_side_angle_distribution == Distributions.UNIFORM:
@@ -114,15 +124,15 @@
             # We take the normalized distribution at this frequency and draw a random number,
             # If the random number is lower than the distribution, we accept this frequency
             if random() < plank_distribution/plank_distribution_max and self.f < max(material.dispersion[:, 1]):
                 break
 
     def assign_speed(self, material):
         """Calculate group velocity dw/dk according to the frequency and polarization"""
-        if self.polarization == Polarization.TA and self.f < max(material.dispersion[:,2]):
+        if self.polarization == Polarizations.TA and self.f < max(material.dispersion[:,2]):
             point_num = abs((np.abs(material.dispersion[:, 2] - self.f)).argmin() - 1)
             d_w = 2*pi*abs(material.dispersion[point_num+1, 2] - material.dispersion[point_num, 2])
         else:
             point_num = abs((np.abs(material.dispersion[:, 1] - self.f)).argmin() - 1)
             d_w = 2*pi*abs(material.dispersion[point_num+1, 1] - material.dispersion[point_num, 1])
         d_k = abs(material.dispersion[point_num+1, 0] - material.dispersion[point_num, 0])
         self.speed = d_w/d_k
```

### Comparing `freepaths-1.2.1/freepaths/progress.py` & `freepaths-1.3/freepaths/progress.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.2.1/freepaths/run_phonon.py` & `freepaths-1.3/freepaths/run_phonon.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.2.1/freepaths/scattering.py` & `freepaths-1.3/freepaths/scattering.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from math import pi, cos, sin, tan, exp, sqrt, atan, asin, acos
 from random import random
 from numpy import sign
 
 from freepaths.config import cf
 from freepaths.move import move
 from freepaths.scattering_types import Scattering
+from freepaths.options import Positions
 
 
 def specularity(angle, roughness, wavelength):
     """Calculate probability of specular scattering with Soffer's equation"""
     return exp(-16 * pi**2 * roughness**2 * ((cos(angle))**2) / wavelength**2)
 
 
@@ -21,18 +22,23 @@
         ph.theta = -pi + random()*2*pi
         ph.phi = asin(2*random() - 1)
         scattering_types.internal = Scattering.DIFFUSE
 
 
 def reinitialization(ph, scattering_types):
     """Re-thermalize phonon if it comes back to the hot side"""
-    _, y, _ = move(ph, cf.timestep)
+    x, y, _ = move(ph, cf.timestep)
 
-    # If phonon returns to the staring line y = 0, generate it again:
-    if y < 0:
+    # If phonon returns to the hot side, generate it again:
+    if (
+        (cf.hot_side_position == Positions.BOTTOM and y < 0) or
+        (cf.hot_side_position == Positions.TOP and y > cf.length) or
+        (cf.hot_side_position == Positions.RIGHT and x > cf.width/2) or
+        (cf.hot_side_position == Positions.LEFT and x < -cf.width/2)
+        ):
         ph.assign_angles()
         scattering_types.hot_side = Scattering.DIFFUSE
 
 
 def top_parabola_scattering(ph, scattering_types):
     """Scattering on top parabolic boundary"""
     x, y, z = move(ph, cf.timestep)
@@ -360,20 +366,20 @@
 def no_new_scattering(ph):
     """Check if new angles do not immediately lead to new top/bottom or sidewall scattering.
     This is necessary to prevent phonons leaving the structure boundaries."""
     x, y, z = move(ph, cf.timestep)
     return True if (abs(z) < cf.thickness / 2 and abs(x) < cf.width / 2 and y > 0) else False
 
 
-def side_wall_scattering(ph, scattering_types):
-    """Check if the phonon hits a side wall and output new vector"""
+def scattering_on_right_sidewall(ph, scattering_types):
+    """Check if the phonon hits right side wall and output new vector"""
     x, y, z = move(ph, cf.timestep)
 
     # If phonon is beyond the side wall:
-    if abs(x) > cf.width/2:
+    if x > cf.width/2:
 
         # Calculate angle to the surface and specular scattering probability:
         a = acos(cos(ph.phi)*sin(abs(ph.theta))) # Angle to the surface
         p = specularity(a, cf.side_wall_roughness, ph.wavelength)
 
         # Specular scattering:
         if random() < p:
@@ -396,14 +402,115 @@
                 ph.phi = asin((asin(2*random() - 1))/(pi/2))
 
                 # Accept the angles if they do not cause new scattering:
                 if no_new_scattering(ph):
                     break
 
 
+def scattering_on_left_sidewall(ph, scattering_types):
+    """Check if the phonon hits left side wall and output new vector"""
+    x, y, z = move(ph, cf.timestep)
+
+    # If phonon is beyond the side wall:
+    if x < -cf.width/2:
+
+        # Calculate angle to the surface and specular scattering probability:
+        a = acos(cos(ph.phi)*sin(abs(ph.theta))) # Angle to the surface
+        p = specularity(a, cf.side_wall_roughness, ph.wavelength)
+
+        # Specular scattering:
+        if random() < p:
+            scattering_types.walls = Scattering.SPECULAR
+            ph.theta = - ph.theta
+
+        # Diffuse scattering:
+        else:
+            scattering_types.walls = Scattering.DIFFUSE
+            attempt = 0
+            while attempt < 10:
+                attempt += 1
+
+                # Random distribution:
+                # theta = -sign(x)*pi+sign(x)*pi*random()
+                # phi = asin(2*random() - 1)
+
+                # Lambert cosine distribution:
+                ph.theta = -sign(x)*pi/2 + asin(2*random() - 1)
+                ph.phi = asin((asin(2*random() - 1))/(pi/2))
+
+                # Accept the angles if they do not cause new scattering:
+                if no_new_scattering(ph):
+                    break
+
+
+def scattering_on_top_sidewall(ph, scattering_types):
+    """Check if the phonon hits top side wall and output new vector"""
+    x, y, z = move(ph, cf.timestep)
+
+    # If phonon is beyond the side wall:
+    if y > cf.length:
+
+        # Calculate angle to the surface and specular scattering probability:
+        a = acos(cos(ph.phi)*cos(ph.theta))
+        p = specularity(a, cf.hole_roughness, ph.wavelength)
+
+        # Specular scattering:
+        if random() < p:
+            scattering_types.holes = Scattering.SPECULAR
+            ph.theta = sign(ph.theta)*pi - ph.theta
+
+        # Diffuse scattering:
+        else:
+            scattering_types.holes = Scattering.DIFFUSE
+            attempt = 0
+            while attempt < 10:
+                attempt += 1
+
+                # Lambert cosine distribution:
+                rand_sign = sign((2*random() - 1))
+                ph.theta = rand_sign*pi/2 + rand_sign*acos(random())
+                ph.phi = asin((asin(2*random() - 1))/(pi/2))
+
+                # Accept the angles only if they do not immediately cause new scattering:
+                if no_new_scattering(ph):
+                    break
+
+
+def scattering_on_bottom_sidewall(ph, scattering_types):
+    """Check if the phonon hits bottom side wall and output new vector"""
+    x, y, z = move(ph, cf.timestep)
+
+    # If phonon is beyond the side wall:
+    if y < 0.0:
+
+        # Calculate angle to the surface and specular scattering probability:
+        a = acos(cos(ph.phi)*cos(ph.theta))
+        p = specularity(a, cf.hole_roughness, ph.wavelength)
+
+        # Specular scattering:
+        if random() < p:
+            scattering_types.holes = Scattering.SPECULAR
+            ph.theta = sign(ph.theta)*pi - ph.theta
+
+        # Diffuse scattering:
+        else:
+            scattering_types.holes = Scattering.DIFFUSE
+            attempt = 0
+            while attempt < 10:
+                attempt += 1
+
+                # Lambert cosine distribution:
+                ph.theta = asin(2*random() - 1)
+                ph.phi = asin((asin(2*random() - 1))/(pi/2))
+
+                # Accept the angles only if they do not immediately cause new scattering:
+                if no_new_scattering(ph):
+                    break
+
+
 def top_scattering(ph, scattering_types):
     """Check if the phonon hits the top surface and output new vector"""
     x, y, z = move(ph, cf.timestep)
 
     # If phonon is above the top surface, scattering happens:
     if z > cf.thickness/2:
 
@@ -522,15 +629,22 @@
         top_scattering(ph, scattering_types)
 
     # Scattering on bottom surface:
     if scattering_types.top_bottom is None:
         bottom_scattering(ph, scattering_types)
 
     # Scattering on sidewalls:
-    side_wall_scattering(ph, scattering_types)
+    if cf.include_right_sidewall:
+        scattering_on_right_sidewall(ph, scattering_types)
+    if cf.include_left_sidewall:
+        scattering_on_left_sidewall(ph, scattering_types)
+    if cf.include_top_sidewall:
+        scattering_on_top_sidewall(ph, scattering_types)
+    if cf.include_bottom_sidewall:
+        scattering_on_bottom_sidewall(ph, scattering_types)
 
     # Scattering on parabolic walls:
     if cf.include_top_parabola:
         top_parabola_scattering(ph, scattering_types)
     if cf.include_bottom_parabola:
         bottom_parabola_scattering(ph, scattering_types)
 
@@ -561,14 +675,16 @@
                 Ly = cf.rectangular_hole_side_y * (cf.hole_coordinates[i, 2] + 1)
                 scattering_on_triangle_up_holes(ph, x0, y0, Lx, Ly, scattering_types, x, y, z)
 
             elif cf.hole_shapes[i] == "triangle_down":
                 Lx = cf.rectangular_hole_side_x * (cf.hole_coordinates[i, 2] + 1)
                 Ly = cf.rectangular_hole_side_y * (cf.hole_coordinates[i, 2] + 1)
                 scattering_on_triangle_down_holes(ph, x0, y0, Lx, Ly, scattering_types, x, y, z)
+            else:
+                pass
 
             # If there was any scattering, then no need to check other holes:
             if scattering_types.holes is not None:
                 break
 
     # Scattering on pillars:
     if cf.include_pillars:
```

### Comparing `freepaths-1.2.1/freepaths/scattering_types.py` & `freepaths-1.3/freepaths/scattering_types.py`

 * *Files identical despite different names*

### Comparing `freepaths-1.2.1/freepaths.egg-info/PKG-INFO` & `freepaths-1.3/freepaths.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freepaths
-Version: 1.2.1
+Version: 1.3
 Summary: Phonon Monte Carlo simulator
 Home-page: https://github.com/anufrievroman/freepaths
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -17,48 +17,45 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 
 # FreePATHS - Free Phonon And THermal Simulator
 
-This Monte Carlo algorithm simulates trajectories of phonons in 3D models of nanostructures, which consists of a box with holes or pillars of various shapes. The algorithm outputs phonon trajectories, heat fluxes, temperature maps and profiles, the thermal conductivity, scattering maps and statistics and other information. See [the wiki pages](https://github.com/anufrievroman/Monte-Carlo/wiki/General-algorithm-flow) for the details of the simulation.
+This Monte Carlo algorithm simulates trajectories of phonons in 3D models of nanostructures, which consists of a box with holes or pillars of various shapes. The algorithm outputs phonon trajectories, heat fluxes, temperature maps and profiles, the thermal conductivity, scattering maps and statistics and other information. See [documentation](https://anufrievroman.gitbook.io/freepaths/) for the details of the simulation.
 
 ![Screenshot](https://github.com/anufrievroman/Monte-Carlo/blob/master/screenshot.png)
 
 
 ## Installation
 
-FreePATHS requires python 3. On Linux and MacOS, it is probably already installed. On Windows, you may choose to install [Anaconda](https://www.anaconda.com) package, which will install everything for you.
-
-Install the package from PyPi repository by entering this command into a terminal or a python console:
+[Installation is detailed in documentation](https://anufrievroman.gitbook.io/freepaths/installation). In short, install the package from PyPi repository by entering this command into a terminal or a python console:
 
 `pip install --upgrade freepaths`
 
-For more details about installation, see [this wiki page](https://github.com/anufrievroman/freepaths/wiki/Installation).
 
 ## Usage
 
 FreePATHS is a command line application, so it runs inside Linux, MacOS, or Windows terminal. It takes an input file from the user, which contains all the settings, and outputs the results in a new folder.
 
 There are two modes of using the program. Main mode traces a large number of phonons through a structure and collects statistics about their paths. The MFP sampling mode measures phonon mean free paths using a small number of phonons and calculates the thermal conductivity by integrating phonon dispersion. 
 
 ### Demo
 
-First, if you simply run `freepaths` without specifying an input file, the program will run a demo simulation.
+If you simply run `freepaths` without specifying an input file, the program will run a demo simulation.
 
 ### Main mode
 
 In the main mode, the program traces large number of phonons through a structure and calculates various statistical distributions and maps. In this mode, the thermal conductivity will be calculated via Fourier law. Note that the thermal conductivity will be correct only in the absence of holes.
 
 Run the program as:
 
 `freepaths your_input_file.py`
 
-See [wiki page](https://github.com/anufrievroman/freepaths/wiki/Creating-input-files) for explanations about creating your own input files. In the [examples](https://github.com/anufrievroman/freepaths/tree/master/examples) folder, you will find examples of various input files. Try using one of them, for instance as:
+See [documentation](https://anufrievroman.gitbook.io/freepaths/examples) for explanations about creating your own input files. In the [examples](https://github.com/anufrievroman/freepaths/tree/master/examples) folder, you will find examples of various input files. Try using one of them, for instance as:
 
 `freepaths simple_nanowire.py`
 
 After the simulation, see the results in a newly created **Results** folder.
 
 
 ### MFP sampling mode
@@ -68,21 +65,21 @@
 `freepaths -s simple_nanowire.py`
 
 The calculated thermal conductivity will be output in the terminal. However, other statistical quantities and plots will still be calculated and output in the `Results` folder.
 
 
 ## Troubleshooting
 
-- [Troubles with installation](https://github.com/anufrievroman/freepaths/wiki/Installation)
-- [Troubles with usage](https://github.com/anufrievroman/freepaths/wiki/Usage)
+- [Troubles with installation](https://anufrievroman.gitbook.io/freepaths/installation)
+- [Troubles with usage](https://anufrievroman.gitbook.io/freepaths/usage)
 
 
 ## Disclaimer
 
-The code is still in development and provided as is. It likely contains bugs or might be inappropriate for your research. It is your responsibility to understand the underlying physics, test the code, and verify that all the equations and the code are correct. See [the wiki pages](https://github.com/anufrievroman/Monte-Carlo/wiki/General-algorithm-flow) and the references below for more details on the code.
+The code is still in development and provided as is. It likely contains bugs or might be inappropriate for your research. It is your responsibility to understand the underlying physics, test the code, and verify that all the equations and the code are correct. See [documentation](https://anufrievroman.gitbook.io/freepaths/algorithm) and the references below for more details on the code.
 
 
 ## References and acknowledgments
 
 The code has been developed by [Roman Anufriev](https://anufrievroman.com) in [Nomura lab](https://www.nlab.iis.u-tokyo.ac.jp/index-e.html) at the University of Tokyo in 2018-2022.
 If you would like to use this code for your research, please see the disclaimer above and consider citing the papers below, if it is appropriate.
 Details of the code and examples of the output can be found in the following papers:
```

### Comparing `freepaths-1.2.1/freepaths.egg-info/SOURCES.txt` & `freepaths-1.3/freepaths.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 freepaths/main_tracing.py
 freepaths/maps.py
 freepaths/materials.py
 freepaths/move.py
 freepaths/options.py
 freepaths/output_info.py
 freepaths/output_plots.py
+freepaths/output_structure.py
 freepaths/phonon.py
 freepaths/progress.py
 freepaths/run_phonon.py
 freepaths/scattering.py
 freepaths/scattering_types.py
 freepaths.egg-info/PKG-INFO
 freepaths.egg-info/SOURCES.txt
```

### Comparing `freepaths-1.2.1/setup.py` & `freepaths-1.3/setup.py`

 * *Files identical despite different names*

