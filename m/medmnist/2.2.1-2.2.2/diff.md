# Comparing `tmp/medmnist-2.2.1.tar.gz` & `tmp/medmnist-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/medmnist-2.2.1.tar", last modified: Sun Apr  2 20:41:50 2023, max compression
+gzip compressed data, was "medmnist-2.2.2.tar", last modified: Thu May 11 20:19:10 2023, max compression
```

## Comparing `medmnist-2.2.1.tar` & `medmnist-2.2.2.tar`

### file list

```diff
@@ -1,29 +1,20 @@
-drwxr-xr-x   0 yangjiancheng   (501) staff       (20)        0 2023-04-02 20:41:50.137298 medmnist-2.2.1/
--rw-r--r--   0 yangjiancheng   (501) staff       (20)     1838 2020-12-04 06:14:24.000000 medmnist-2.2.1/.gitignore
--rw-r--r--   0 yangjiancheng   (501) staff       (20)    11348 2023-04-02 20:38:44.000000 medmnist-2.2.1/LICENSE
--rw-r--r--   0 yangjiancheng   (501) staff       (20)    11971 2023-04-02 20:41:50.136462 medmnist-2.2.1/PKG-INFO
--rw-r--r--   0 yangjiancheng   (501) staff       (20)    10228 2023-04-02 20:40:50.000000 medmnist-2.2.1/README.md
-drwxr-xr-x   0 yangjiancheng   (501) staff       (20)        0 2023-04-02 20:41:50.097843 medmnist-2.2.1/assets/
--rw-r--r--   0 yangjiancheng   (501) staff       (20)   463986 2021-08-22 12:37:13.000000 medmnist-2.2.1/assets/medmnistv1.jpg
--rw-r--r--   0 yangjiancheng   (501) staff       (20)   631019 2023-04-01 17:07:22.000000 medmnist-2.2.1/assets/medmnistv2.jpg
-drwxr-xr-x   0 yangjiancheng   (501) staff       (20)        0 2023-04-02 20:41:50.115219 medmnist-2.2.1/examples/
--rw-r--r--   0 yangjiancheng   (501) staff       (20)     8755 2021-08-22 22:09:52.000000 medmnist-2.2.1/examples/dataset_without_pytorch.py
--rw-r--r--   0 yangjiancheng   (501) staff       (20)  1269363 2022-05-06 14:53:03.000000 medmnist-2.2.1/examples/getting_started.ipynb
--rw-r--r--   0 yangjiancheng   (501) staff       (20)  1253929 2022-05-06 14:53:03.000000 medmnist-2.2.1/examples/getting_started_without_PyTorch.ipynb
-drwxr-xr-x   0 yangjiancheng   (501) staff       (20)        0 2023-04-02 20:41:50.130565 medmnist-2.2.1/medmnist/
--rw-r--r--   0 yangjiancheng   (501) staff       (20)      569 2021-08-22 22:09:53.000000 medmnist-2.2.1/medmnist/__init__.py
--rw-r--r--   0 yangjiancheng   (501) staff       (20)     3268 2021-08-22 22:09:53.000000 medmnist-2.2.1/medmnist/__main__.py
--rw-r--r--   0 yangjiancheng   (501) staff       (20)     7897 2021-08-22 22:09:53.000000 medmnist-2.2.1/medmnist/dataset.py
--rw-r--r--   0 yangjiancheng   (501) staff       (20)     7155 2021-08-22 22:09:53.000000 medmnist-2.2.1/medmnist/evaluator.py
--rw-r--r--   0 yangjiancheng   (501) staff       (20)    22841 2023-04-02 20:39:59.000000 medmnist-2.2.1/medmnist/info.py
--rw-r--r--   0 yangjiancheng   (501) staff       (20)     2501 2023-04-02 20:12:30.000000 medmnist-2.2.1/medmnist/utils.py
-drwxr-xr-x   0 yangjiancheng   (501) staff       (20)        0 2023-04-02 20:41:50.135143 medmnist-2.2.1/medmnist.egg-info/
--rw-r--r--   0 yangjiancheng   (501) staff       (20)    11971 2023-04-02 20:41:49.000000 medmnist-2.2.1/medmnist.egg-info/PKG-INFO
--rw-r--r--   0 yangjiancheng   (501) staff       (20)      517 2023-04-02 20:41:50.000000 medmnist-2.2.1/medmnist.egg-info/SOURCES.txt
--rw-r--r--   0 yangjiancheng   (501) staff       (20)        1 2023-04-02 20:41:49.000000 medmnist-2.2.1/medmnist.egg-info/dependency_links.txt
--rw-r--r--   0 yangjiancheng   (501) staff       (20)       74 2023-04-02 20:41:49.000000 medmnist-2.2.1/medmnist.egg-info/requires.txt
--rw-r--r--   0 yangjiancheng   (501) staff       (20)        9 2023-04-02 20:41:49.000000 medmnist-2.2.1/medmnist.egg-info/top_level.txt
--rw-r--r--   0 yangjiancheng   (501) staff       (20)        1 2023-04-02 20:41:49.000000 medmnist-2.2.1/medmnist.egg-info/zip-safe
--rw-r--r--   0 yangjiancheng   (501) staff       (20)       73 2021-11-22 12:50:28.000000 medmnist-2.2.1/requirements.txt
--rw-r--r--   0 yangjiancheng   (501) staff       (20)       38 2023-04-02 20:41:50.137653 medmnist-2.2.1/setup.cfg
--rw-r--r--   0 yangjiancheng   (501) staff       (20)     1150 2023-04-02 20:39:06.000000 medmnist-2.2.1/setup.py
+drwxr-xr-x   0 jiyang     (502) staff       (20)        0 2023-05-11 20:19:10.498004 medmnist-2.2.2/
+-rw-r--r--   0 jiyang     (502) staff       (20)    11348 2023-05-11 20:14:10.000000 medmnist-2.2.2/LICENSE
+-rw-r--r--   0 jiyang     (502) staff       (20)    10821 2023-05-11 20:19:10.497778 medmnist-2.2.2/PKG-INFO
+-rw-r--r--   0 jiyang     (502) staff       (20)    10294 2023-05-11 20:17:58.000000 medmnist-2.2.2/README.md
+drwxr-xr-x   0 jiyang     (502) staff       (20)        0 2023-05-11 20:19:10.496577 medmnist-2.2.2/medmnist/
+-rw-r--r--   0 jiyang     (502) staff       (20)      569 2022-10-26 12:13:26.000000 medmnist-2.2.2/medmnist/__init__.py
+-rw-r--r--   0 jiyang     (502) staff       (20)     3268 2022-10-26 12:13:26.000000 medmnist-2.2.2/medmnist/__main__.py
+-rw-r--r--   0 jiyang     (502) staff       (20)     7897 2022-10-26 12:13:26.000000 medmnist-2.2.2/medmnist/dataset.py
+-rw-r--r--   0 jiyang     (502) staff       (20)     7155 2022-10-26 12:13:26.000000 medmnist-2.2.2/medmnist/evaluator.py
+-rw-r--r--   0 jiyang     (502) staff       (20)    22841 2023-05-11 20:16:48.000000 medmnist-2.2.2/medmnist/info.py
+-rw-r--r--   0 jiyang     (502) staff       (20)     2501 2023-05-11 20:14:10.000000 medmnist-2.2.2/medmnist/utils.py
+drwxr-xr-x   0 jiyang     (502) staff       (20)        0 2023-05-11 20:19:10.497575 medmnist-2.2.2/medmnist.egg-info/
+-rw-r--r--   0 jiyang     (502) staff       (20)    10821 2023-05-11 20:19:10.000000 medmnist-2.2.2/medmnist.egg-info/PKG-INFO
+-rw-r--r--   0 jiyang     (502) staff       (20)      331 2023-05-11 20:19:10.000000 medmnist-2.2.2/medmnist.egg-info/SOURCES.txt
+-rw-r--r--   0 jiyang     (502) staff       (20)        1 2023-05-11 20:19:10.000000 medmnist-2.2.2/medmnist.egg-info/dependency_links.txt
+-rw-r--r--   0 jiyang     (502) staff       (20)       74 2023-05-11 20:19:10.000000 medmnist-2.2.2/medmnist.egg-info/requires.txt
+-rw-r--r--   0 jiyang     (502) staff       (20)        9 2023-05-11 20:19:10.000000 medmnist-2.2.2/medmnist.egg-info/top_level.txt
+-rw-r--r--   0 jiyang     (502) staff       (20)        1 2023-05-11 20:19:10.000000 medmnist-2.2.2/medmnist.egg-info/zip-safe
+-rw-r--r--   0 jiyang     (502) staff       (20)       38 2023-05-11 20:19:10.498043 medmnist-2.2.2/setup.cfg
+-rw-r--r--   0 jiyang     (502) staff       (20)     1150 2023-05-11 20:14:10.000000 medmnist-2.2.2/setup.py
```

### Comparing `medmnist-2.2.1/LICENSE` & `medmnist-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `medmnist-2.2.1/PKG-INFO` & `medmnist-2.2.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,166 +1,153 @@
-Metadata-Version: 2.1
-Name: medmnist
-Version: 2.2.1
-Summary: MedMNIST: 18 MNIST-like Datasets for 2D and 3D Biomedical Image Classification
-Home-page: https://github.com/MedMNIST/MedMNIST/
-Author: MedMNIST Team
-Author-email: jiancheng.yang@epfl.ch
-License: Apache-2.0 License
-Description: # MedMNIST: [medmnist.com](https://medmnist.github.io/)
-        ## Data ([Zenodo](https://doi.org/10.5281/zenodo.6496656)) | Publication ([Scientific Data](https://doi.org/10.1038/s41597-022-01721-8) / [arXiv](https://arxiv.org/abs/2110.14795)) | MedMNIST v1 ([ISBI'21](https://medmnist.github.io/v1)) 
-        [Jiancheng Yang](https://jiancheng-yang.com/), Rui Shi, [Donglai Wei](https://donglaiw.github.io/), Zequan Liu, Lin Zhao, [Bilian Ke](https://scholar.google.com/citations?user=2cX5y8kAAAAJ&hl=en), [Hanspeter Pfister](https://scholar.google.com/citations?user=VWX-GMAAAAAJ&hl=en), [Bingbing Ni](https://scholar.google.com/citations?user=eUbmKwYAAAAJ)
-        
-        [![](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MedMNIST/MedMNIST/blob/main/examples/getting_started.ipynb)
-        
-        We introduce *MedMNIST v2*, a large-scale MNIST-like collection of standardized biomedical images, including 12 datasets for 2D and 6 datasets for 3D. All images are pre-processed into 28x28 (2D) or 28x28x28 (3D) with the corresponding classification labels, so that no background knowledge is required for users. Covering primary data modalities in biomedical images, MedMNIST v2 is designed to perform classification on lightweight 2D and 3D images with various data scales (from 100 to 100,000) and diverse tasks (binary/multi-class, ordinal regression and multi-label). The resulting dataset, consisting of 708,069 2D images and 9,998 3D images in total, could support numerous research / educational purposes in biomedical image analysis, computer vision and machine learning. We benchmark several baseline methods on MedMNIST v2, including 2D / 3D neural networks and open-source / commercial AutoML tools. 
-        
-        ![MedMNISTv2_overview](https://raw.githubusercontent.com/MedMNIST/MedMNIST/main/assets/medmnistv2.jpg)
-        
-        For more details, please refer to our paper:
-        
-        **MedMNIST v2: A Large-Scale Lightweight Benchmark for 2D and 3D Biomedical Image Classification** ([Scientific Data](https://doi.org/10.1038/s41597-022-01721-8) / [arXiv](https://arxiv.org/abs/2110.14795))
-        
-        or its conference version:
-        
-        **MedMNIST Classification Decathlon: A Lightweight AutoML Benchmark for Medical Image Analysis** ([ISBI'21](https://arxiv.org/abs/2010.14925))
-        
-        # Key Features
-        * ***Diverse***: It covers diverse data modalities, dataset scales (from 100 to 100,000), and tasks (binary/multi-class, multi-label, and ordinal regression). It is as diverse as the VDD and MSD to fairly evaluate the generalizable performance of machine learning algorithms in different settings, but both 2D and 3D biomedical images are provided. 
-        * ***Standardized***: Each sub-dataset is pre-processed into the same format, which requires no background knowledge for users. As an MNIST-like dataset collection to perform classification tasks on small images, it primarily focuses on the machine learning part rather than the end-to-end system. Furthermore, we provide standard train-validation-test splits for all datasets in MedMNIST v2, therefore algorithms could be easily compared. 
-        * ***Lightweight***: The small size of 28×28 (2D) or 28×28×28 (3D) is friendly to evaluate machine learning algorithms. 
-        * ***Educational***: As an interdisciplinary research area, biomedical image analysis is difficult to hand on for researchers from other communities, as it requires background knowledge from computer vision, machine learning, biomedical imaging, and clinical science. Our data with the Creative Commons (CC) License is easy to use for educational purposes.
-        
-        Please note that this dataset is **NOT** intended for clinical use.
-        
-        # Code Structure
-        * [`medmnist/`](medmnist/):
-            * [`dataset.py`](medmnist/dataset.py): PyTorch datasets and dataloaders of MedMNIST.
-            * [`evaluator.py`](medmnist/evaluator.py): Standardized evaluation functions.
-            * [`info.py`](medmnist/info.py): Dataset information `dict` for each subset of MedMNIST.
-        * [`examples/`](examples/):
-            * [`getting_started.ipynb`](examples/getting_started.ipynb): To explore the MedMNIST dataset with jupyter notebook. It is ONLY intended for a quick exploration, i.e., it does not provide full training and evaluation functionalities. 
-            * [`getting_started_without_PyTorch.ipynb`](examples/getting_started_without_PyTorch.ipynb): This notebook provides snippets about how to use MedMNIST data (the `.npz` files) without PyTorch.
-        * [`setup.py`](setup.py): To install `medmnist` as a module.
-        * [EXTERNAL] [`MedMNIST/experiments`](https://github.com/MedMNIST/experiments): training and evaluation scripts to reproduce both 2D and 3D experiments in our paper, including PyTorch, auto-sklearn, AutoKeras and Google AutoML Vision together with their weights ;)
-        
-        # Installation and Requirements
-        Setup the required environments and install `medmnist` as a standard Python package from [PyPI](https://pypi.org/project/medmnist/):
-        
-            pip install medmnist
-        
-        Or install from source:
-        
-            pip install --upgrade git+https://github.com/MedMNIST/MedMNIST.git
-        
-        Check whether you have installed the latest [version](medmnist/info.py):
-        
-            >>> import medmnist
-            >>> print(medmnist.__version__)
-        
-        The code requires only common Python environments for machine learning. Basically, it was tested with
-        * Python 3 (>=3.6)
-        * PyTorch\==1.3.1
-        * numpy\==1.18.5, pandas\==0.25.3, scikit-learn\==0.22.2, Pillow\==8.0.1
-        * fire, scikit-image
-        
-        Higher (or lower) versions should also work (perhaps with minor modifications). 
-        
-        # If you use PyTorch...
-        
-        * Great! Our code is designed to work with PyTorch.
-        
-        * Explore the MedMNIST dataset with jupyter notebook ([`getting_started.ipynb`](examples/getting_started.ipynb)), and train basic neural networks in PyTorch.
-        
-        
-        # If you do not use PyTorch...
-        
-        * Although our code is tested with PyTorch, you are free to parse them with your own code (without PyTorch or even without Python!), as they are only standard NumPy serialization files. It is simple to create a dataset without PyTorch.
-        * Go to [`getting_started_without_PyTorch.ipynb`](examples/getting_started_without_PyTorch.ipynb), which provides snippets about how to use MedMNIST data (the `.npz` files) without PyTorch.
-        * Simply change the super class of `MedMNIST` from `torch.utils.data.Dataset` to `collections.Sequence`, you will get a standard dataset without PyTorch. Check [`dataset_without_pytorch.py`](examples/dataset_without_pytorch.py) for more details.
-        * You still have most functionality of our MedMNIST code ;)
-        
-        # Dataset
-        
-        Please download the dataset(s) via [`Zenodo`](https://doi.org/10.5281/zenodo.6496656). You could also use our code to download automatically by setting `download=True` in [`dataset.py`](medmnist/dataset.py).
-        
-        The MedMNIST dataset contains several subsets. Each subset (e.g., `pathmnist.npz`) is comprised of 6 keys: `train_images`, `train_labels`, `val_images`, `val_labels`, `test_images` and `test_labels`.
-        * `train_images` / `val_images` / `test_images`: `N` × 28 × 28 for 2D gray-scale datasets, `N` × 28 × 28 × 3 for 2D RGB datasets, `N` × 28 × 28 × 28 for 3D datasets. `N` denotes the number of samples.  
-        * `train_labels` / `val_labels` / `test_labels`: `N` x `L`. `N` denotes the number of samples. `L` denotes the number of task labels; for single-label (binary/multi-class) classification, `L=1`, and `{0,1,2,3,..,C}` denotes the category labels (`C=1` for binary); for multi-label classification `L!=1`, e.g., `L=14` for `chestmnist.npz`.
-        
-        # Command Line Tools
-        
-        * List all available datasets:
-            
-                python -m medmnist available
-        
-        * Download all available datasets:
-            
-                python -m medmnist download
-        
-        * Delete all downloaded npz from root:
-        
-                python -m medmnist clean
-        
-        * Print the dataset details given a subset flag:
-        
-                python -m medmnist info --flag=xxxmnist
-        
-        * Save the dataset as standard figure and csv files, which could be used for AutoML tools, e.g., Google AutoML Vision:
-        
-            for 2D datasets:
-        
-                python -m medmnist save --flag=xxxmnist --folder=tmp/ --postfix=png
-                
-            for 3D datasets:
-        
-                python -m medmnist save --flag=xxxmnist3d --folder=tmp/ --postfix=gif
-        
-        * Parse and evaluate a standard result file, refer to [`Evaluator.parse_and_evaluate`](medmnist/evaluator.py) for details.
-        
-                python -m medmnist evaluate --path=folder/{flag}_{split}@{run}.csv
-        
-        # License and Citation
-        
-        The code is under [Apache-2.0 License](./LICENSE).
-        
-        The MedMNIST dataset is licensed under *Creative Commons Attribution 4.0 International* ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)).
-        If you find this project useful in your research, please cite the following papers:
-        
-            Jiancheng Yang, Rui Shi, Donglai Wei, Zequan Liu, Lin Zhao, Bilian Ke, Hanspeter Pfister, Bingbing Ni. Yang, Jiancheng, et al. "MedMNIST v2-A large-scale lightweight benchmark for 2D and 3D biomedical image classification." Scientific Data, 2023.
-        
-            Jiancheng Yang, Rui Shi, Bingbing Ni. "MedMNIST Classification Decathlon: A Lightweight AutoML Benchmark for Medical Image Analysis". IEEE 18th International Symposium on Biomedical Imaging (ISBI), 2021.
-        
-        or using the bibtex:
-        
-            @article{medmnistv2,
-                title={MedMNIST v2-A large-scale lightweight benchmark for 2D and 3D biomedical image classification},
-                author={Yang, Jiancheng and Shi, Rui and Wei, Donglai and Liu, Zequan and Zhao, Lin and Ke, Bilian and Pfister, Hanspeter and Ni, Bingbing},
-                journal={Scientific Data},
-                volume={10},
-                number={1},
-                pages={41},
-                year={2023},
-                publisher={Nature Publishing Group UK London}
-            }
-             
-            @inproceedings{medmnistv1,
-                title={MedMNIST Classification Decathlon: A Lightweight AutoML Benchmark for Medical Image Analysis},
-                author={Yang, Jiancheng and Shi, Rui and Ni, Bingbing},
-                booktitle={IEEE 18th International Symposium on Biomedical Imaging (ISBI)},
-                pages={191--195},
-                year={2021}
-            }
-        
-        Please also cite source data paper(s) of the MedMNIST subset(s) as per the description on the [project page](https://medmnist.github.io/).
-        
-        # Release Notes
-        * `v2.2.1`: PyPI info updated
-        * `v2.2.0`: `montage` method supported for scikit-image>=0.20.0
-        * `v2.1.0`: `NoduleMNIST3D` data error fixed
-        * `v2.0.0`: MedMNIST v2 release
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
+# MedMNIST: [medmnist.com](https://medmnist.github.io/)
+## Data ([Zenodo](https://doi.org/10.5281/zenodo.6496656)) | Publication ([Scientific Data](https://doi.org/10.1038/s41597-022-01721-8) / [arXiv](https://arxiv.org/abs/2110.14795)) | MedMNIST v1 ([ISBI'21](https://medmnist.github.io/v1)) 
+[Jiancheng Yang](https://jiancheng-yang.com/), Rui Shi, [Donglai Wei](https://donglaiw.github.io/), Zequan Liu, Lin Zhao, [Bilian Ke](https://scholar.google.com/citations?user=2cX5y8kAAAAJ&hl=en), [Hanspeter Pfister](https://scholar.google.com/citations?user=VWX-GMAAAAAJ&hl=en), [Bingbing Ni](https://scholar.google.com/citations?user=eUbmKwYAAAAJ)
+
+[![](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MedMNIST/MedMNIST/blob/main/examples/getting_started.ipynb)
+
+We introduce *MedMNIST v2*, a large-scale MNIST-like collection of standardized biomedical images, including 12 datasets for 2D and 6 datasets for 3D. All images are pre-processed into 28x28 (2D) or 28x28x28 (3D) with the corresponding classification labels, so that no background knowledge is required for users. Covering primary data modalities in biomedical images, MedMNIST v2 is designed to perform classification on lightweight 2D and 3D images with various data scales (from 100 to 100,000) and diverse tasks (binary/multi-class, ordinal regression and multi-label). The resulting dataset, consisting of 708,069 2D images and 9,998 3D images in total, could support numerous research / educational purposes in biomedical image analysis, computer vision and machine learning. We benchmark several baseline methods on MedMNIST v2, including 2D / 3D neural networks and open-source / commercial AutoML tools. 
+
+![MedMNISTv2_overview](https://raw.githubusercontent.com/MedMNIST/MedMNIST/main/assets/medmnistv2.jpg)
+
+For more details, please refer to our paper:
+
+**MedMNIST v2: A Large-Scale Lightweight Benchmark for 2D and 3D Biomedical Image Classification** ([Scientific Data](https://doi.org/10.1038/s41597-022-01721-8) / [arXiv](https://arxiv.org/abs/2110.14795))
+
+or its conference version:
+
+**MedMNIST Classification Decathlon: A Lightweight AutoML Benchmark for Medical Image Analysis** ([ISBI'21](https://arxiv.org/abs/2010.14925))
+
+# Key Features
+* ***Diverse***: It covers diverse data modalities, dataset scales (from 100 to 100,000), and tasks (binary/multi-class, multi-label, and ordinal regression). It is as diverse as the VDD and MSD to fairly evaluate the generalizable performance of machine learning algorithms in different settings, but both 2D and 3D biomedical images are provided. 
+* ***Standardized***: Each sub-dataset is pre-processed into the same format, which requires no background knowledge for users. As an MNIST-like dataset collection to perform classification tasks on small images, it primarily focuses on the machine learning part rather than the end-to-end system. Furthermore, we provide standard train-validation-test splits for all datasets in MedMNIST v2, therefore algorithms could be easily compared. 
+* ***Lightweight***: The small size of 28×28 (2D) or 28×28×28 (3D) is friendly to evaluate machine learning algorithms. 
+* ***Educational***: As an interdisciplinary research area, biomedical image analysis is difficult to hand on for researchers from other communities, as it requires background knowledge from computer vision, machine learning, biomedical imaging, and clinical science. Our data with the Creative Commons (CC) License is easy to use for educational purposes.
+
+Please note that this dataset is **NOT** intended for clinical use.
+
+# Code Structure
+* [`medmnist/`](medmnist/):
+    * [`dataset.py`](medmnist/dataset.py): PyTorch datasets and dataloaders of MedMNIST.
+    * [`evaluator.py`](medmnist/evaluator.py): Standardized evaluation functions.
+    * [`info.py`](medmnist/info.py): Dataset information `dict` for each subset of MedMNIST.
+* [`examples/`](examples/):
+    * [`getting_started.ipynb`](examples/getting_started.ipynb): To explore the MedMNIST dataset with jupyter notebook. It is ONLY intended for a quick exploration, i.e., it does not provide full training and evaluation functionalities. 
+    * [`getting_started_without_PyTorch.ipynb`](examples/getting_started_without_PyTorch.ipynb): This notebook provides snippets about how to use MedMNIST data (the `.npz` files) without PyTorch.
+* [`setup.py`](setup.py): To install `medmnist` as a module.
+* [EXTERNAL] [`MedMNIST/experiments`](https://github.com/MedMNIST/experiments): training and evaluation scripts to reproduce both 2D and 3D experiments in our paper, including PyTorch, auto-sklearn, AutoKeras and Google AutoML Vision together with their weights ;)
+
+# Installation and Requirements
+Setup the required environments and install `medmnist` as a standard Python package from [PyPI](https://pypi.org/project/medmnist/):
+
+    pip install medmnist
+
+Or install from source:
+
+    pip install --upgrade git+https://github.com/MedMNIST/MedMNIST.git
+
+Check whether you have installed the latest [version](medmnist/info.py):
+
+    >>> import medmnist
+    >>> print(medmnist.__version__)
+
+The code requires only common Python environments for machine learning. Basically, it was tested with
+* Python 3 (>=3.6)
+* PyTorch\==1.3.1
+* numpy\==1.18.5, pandas\==0.25.3, scikit-learn\==0.22.2, Pillow\==8.0.1
+* fire, scikit-image
+
+Higher (or lower) versions should also work (perhaps with minor modifications). 
+
+# If you use PyTorch...
+
+* Great! Our code is designed to work with PyTorch.
+
+* Explore the MedMNIST dataset with jupyter notebook ([`getting_started.ipynb`](examples/getting_started.ipynb)), and train basic neural networks in PyTorch.
+
+
+# If you do not use PyTorch...
+
+* Although our code is tested with PyTorch, you are free to parse them with your own code (without PyTorch or even without Python!), as they are only standard NumPy serialization files. It is simple to create a dataset without PyTorch.
+* Go to [`getting_started_without_PyTorch.ipynb`](examples/getting_started_without_PyTorch.ipynb), which provides snippets about how to use MedMNIST data (the `.npz` files) without PyTorch.
+* Simply change the super class of `MedMNIST` from `torch.utils.data.Dataset` to `collections.Sequence`, you will get a standard dataset without PyTorch. Check [`dataset_without_pytorch.py`](examples/dataset_without_pytorch.py) for more details.
+* You still have most functionality of our MedMNIST code ;)
+
+# Dataset
+
+Please download the dataset(s) via [`Zenodo`](https://doi.org/10.5281/zenodo.6496656). You could also use our code to download automatically by setting `download=True` in [`dataset.py`](medmnist/dataset.py).
+
+The MedMNIST dataset contains several subsets. Each subset (e.g., `pathmnist.npz`) is comprised of 6 keys: `train_images`, `train_labels`, `val_images`, `val_labels`, `test_images` and `test_labels`.
+* `train_images` / `val_images` / `test_images`: `N` × 28 × 28 for 2D gray-scale datasets, `N` × 28 × 28 × 3 for 2D RGB datasets, `N` × 28 × 28 × 28 for 3D datasets. `N` denotes the number of samples.  
+* `train_labels` / `val_labels` / `test_labels`: `N` x `L`. `N` denotes the number of samples. `L` denotes the number of task labels; for single-label (binary/multi-class) classification, `L=1`, and `{0,1,2,3,..,C}` denotes the category labels (`C=1` for binary); for multi-label classification `L!=1`, e.g., `L=14` for `chestmnist.npz`.
+
+# Command Line Tools
+
+* List all available datasets:
+    
+        python -m medmnist available
+
+* Download all available datasets:
+    
+        python -m medmnist download
+
+* Delete all downloaded npz from root:
+
+        python -m medmnist clean
+
+* Print the dataset details given a subset flag:
+
+        python -m medmnist info --flag=xxxmnist
+
+* Save the dataset as standard figure and csv files, which could be used for AutoML tools, e.g., Google AutoML Vision:
+
+    for 2D datasets:
+
+        python -m medmnist save --flag=xxxmnist --folder=tmp/ --postfix=png
+        
+    for 3D datasets:
+
+        python -m medmnist save --flag=xxxmnist3d --folder=tmp/ --postfix=gif
+
+* Parse and evaluate a standard result file, refer to [`Evaluator.parse_and_evaluate`](medmnist/evaluator.py) for details.
+
+        python -m medmnist evaluate --path=folder/{flag}_{split}@{run}.csv
+
+# License and Citation
+
+The code is under [Apache-2.0 License](./LICENSE).
+
+The MedMNIST dataset is licensed under *Creative Commons Attribution 4.0 International* ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)).
+If you find this project useful in your research, please cite the following papers:
+
+    Jiancheng Yang, Rui Shi, Donglai Wei, Zequan Liu, Lin Zhao, Bilian Ke, Hanspeter Pfister, Bingbing Ni. Yang, Jiancheng, et al. "MedMNIST v2-A large-scale lightweight benchmark for 2D and 3D biomedical image classification." Scientific Data, 2023.
+
+    Jiancheng Yang, Rui Shi, Bingbing Ni. "MedMNIST Classification Decathlon: A Lightweight AutoML Benchmark for Medical Image Analysis". IEEE 18th International Symposium on Biomedical Imaging (ISBI), 2021.
+
+or using the bibtex:
+
+    @article{medmnistv2,
+        title={MedMNIST v2-A large-scale lightweight benchmark for 2D and 3D biomedical image classification},
+        author={Yang, Jiancheng and Shi, Rui and Wei, Donglai and Liu, Zequan and Zhao, Lin and Ke, Bilian and Pfister, Hanspeter and Ni, Bingbing},
+        journal={Scientific Data},
+        volume={10},
+        number={1},
+        pages={41},
+        year={2023},
+        publisher={Nature Publishing Group UK London}
+    }
+     
+    @inproceedings{medmnistv1,
+        title={MedMNIST Classification Decathlon: A Lightweight AutoML Benchmark for Medical Image Analysis},
+        author={Yang, Jiancheng and Shi, Rui and Ni, Bingbing},
+        booktitle={IEEE 18th International Symposium on Biomedical Imaging (ISBI)},
+        pages={191--195},
+        year={2021}
+    }
+
+Please also cite source data paper(s) of the MedMNIST subset(s) as per the description on the [project page](https://medmnist.github.io/).
+
+# Release Notes
+* `v2.2.2`: Python 3.11 `Sequence` from collections.abc supported
+* `v2.2.1`: PyPI info updated
+* `v2.2.0`: `montage` method supported for scikit-image>=0.20.0
+* `v2.1.0`: `NoduleMNIST3D` data error fixed
+* `v2.0.0`: MedMNIST v2 release
```

### Comparing `medmnist-2.2.1/README.md` & `medmnist-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: medmnist
+Version: 2.2.2
+Summary: MedMNIST: 18 MNIST-like Datasets for 2D and 3D Biomedical Image Classification
+Home-page: https://github.com/MedMNIST/MedMNIST/
+Author: MedMNIST Team
+Author-email: jiancheng.yang@epfl.ch
+License: Apache-2.0 License
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # MedMNIST: [medmnist.com](https://medmnist.github.io/)
 ## Data ([Zenodo](https://doi.org/10.5281/zenodo.6496656)) | Publication ([Scientific Data](https://doi.org/10.1038/s41597-022-01721-8) / [arXiv](https://arxiv.org/abs/2110.14795)) | MedMNIST v1 ([ISBI'21](https://medmnist.github.io/v1)) 
 [Jiancheng Yang](https://jiancheng-yang.com/), Rui Shi, [Donglai Wei](https://donglaiw.github.io/), Zequan Liu, Lin Zhao, [Bilian Ke](https://scholar.google.com/citations?user=2cX5y8kAAAAJ&hl=en), [Hanspeter Pfister](https://scholar.google.com/citations?user=VWX-GMAAAAAJ&hl=en), [Bingbing Ni](https://scholar.google.com/citations?user=eUbmKwYAAAAJ)
 
 [![](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MedMNIST/MedMNIST/blob/main/examples/getting_started.ipynb)
 
 We introduce *MedMNIST v2*, a large-scale MNIST-like collection of standardized biomedical images, including 12 datasets for 2D and 6 datasets for 3D. All images are pre-processed into 28x28 (2D) or 28x28x28 (3D) with the corresponding classification labels, so that no background knowledge is required for users. Covering primary data modalities in biomedical images, MedMNIST v2 is designed to perform classification on lightweight 2D and 3D images with various data scales (from 100 to 100,000) and diverse tasks (binary/multi-class, ordinal regression and multi-label). The resulting dataset, consisting of 708,069 2D images and 9,998 3D images in total, could support numerous research / educational purposes in biomedical image analysis, computer vision and machine learning. We benchmark several baseline methods on MedMNIST v2, including 2D / 3D neural networks and open-source / commercial AutoML tools. 
@@ -142,11 +157,12 @@
         pages={191--195},
         year={2021}
     }
 
 Please also cite source data paper(s) of the MedMNIST subset(s) as per the description on the [project page](https://medmnist.github.io/).
 
 # Release Notes
+* `v2.2.2`: Python 3.11 `Sequence` from collections.abc supported
 * `v2.2.1`: PyPI info updated
 * `v2.2.0`: `montage` method supported for scikit-image>=0.20.0
 * `v2.1.0`: `NoduleMNIST3D` data error fixed
-* `v2.0.0`: MedMNIST v2 release
+* `v2.0.0`: MedMNIST v2 release
```

### Comparing `medmnist-2.2.1/examples/dataset_without_pytorch.py` & `medmnist-2.2.2/medmnist/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
-import random
 import numpy as np
-from collections import Sequence
 from PIL import Image
+from torch.utils.data import Dataset
 from medmnist.info import INFO, HOMEPAGE, DEFAULT_ROOT
 
 
-class MedMNIST(Sequence):
+class MedMNIST(Dataset):
 
     flag = ...
 
     def __init__(self,
                  split,
                  transform=None,
                  target_transform=None,
@@ -33,16 +32,16 @@
                                "Please specify and create the `root` directory manually.")
 
         if download:
             self.download()
 
         if not os.path.exists(
                 os.path.join(self.root, "{}.npz".format(self.flag))):
-            raise RuntimeError('Dataset not found.' +
-                               ' You can use download=True to download it')
+            raise RuntimeError('Dataset not found. ' +
+                               ' You can set `download=True` to download it')
 
         npz_file = np.load(os.path.join(self.root, "{}.npz".format(self.flag)))
 
         self.split = split
         self.transform = transform
         self.target_transform = target_transform
         self.as_rgb = as_rgb
@@ -87,23 +86,14 @@
                          filename="{}.npz".format(self.flag),
                          md5=self.info["MD5"])
         except:
             raise RuntimeError('Something went wrong when downloading! ' +
                                'Go to the homepage to download manually. ' +
                                HOMEPAGE)
 
-    @staticmethod
-    def _collate_fn(data):
-        xs = []
-        ys = []
-        for x, y in data:
-            xs.append(np.array(x))
-            ys.append(y)
-        return np.array(xs), np.array(ys)
-
 
 class MedMNIST2D(MedMNIST):
 
     def __getitem__(self, index):
         '''
         return: (without transform/target_transofrm)
             img: PIL.Image
@@ -279,33 +269,7 @@
     flag = "synapsemnist3d"
 
 
 # backward-compatible
 OrganMNISTAxial = OrganAMNIST
 OrganMNISTCoronal = OrganCMNIST
 OrganMNISTSagittal = OrganSMNIST
-
-
-def get_loader(dataset, batch_size):
-    total_size = len(dataset)
-    print('Size', total_size)
-    index_generator = shuffle_iterator(range(total_size))
-    while True:
-        data = []
-        for _ in range(batch_size):
-            idx = next(index_generator)
-            data.append(dataset[idx])
-        yield dataset._collate_fn(data)
-
-
-def shuffle_iterator(iterator):
-    # iterator should have limited size
-    index = list(iterator)
-    total_size = len(index)
-    i = 0
-    random.shuffle(index)
-    while True:
-        yield index[i]
-        i += 1
-        if i >= total_size:
-            i = 0
-            random.shuffle(index)
```

### Comparing `medmnist-2.2.1/medmnist/__init__.py` & `medmnist-2.2.2/medmnist/__init__.py`

 * *Files identical despite different names*

### Comparing `medmnist-2.2.1/medmnist/__main__.py` & `medmnist-2.2.2/medmnist/__main__.py`

 * *Files identical despite different names*

### Comparing `medmnist-2.2.1/medmnist/dataset.py` & `medmnist-2.2.2/medmnist/evaluator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,275 +1,214 @@
 import os
+import warnings
 import numpy as np
-from PIL import Image
-from torch.utils.data import Dataset
-from medmnist.info import INFO, HOMEPAGE, DEFAULT_ROOT
-
-
-class MedMNIST(Dataset):
-
-    flag = ...
-
-    def __init__(self,
-                 split,
-                 transform=None,
-                 target_transform=None,
-                 download=False,
-                 as_rgb=False,
-                 root=DEFAULT_ROOT):
-        ''' dataset
-        :param split: 'train', 'val' or 'test', select subset
-        :param transform: data transformation
-        :param target_transform: target transformation
+import pandas as pd
+from collections import namedtuple
+from sklearn.metrics import roc_auc_score
+from sklearn.metrics import accuracy_score
 
-        '''
+from medmnist.info import INFO, DEFAULT_ROOT
 
-        self.info = INFO[self.flag]
+Metrics = namedtuple("Metrics", ["AUC", "ACC"])
+
+
+class Evaluator:
+    def __init__(self, flag, split, root=DEFAULT_ROOT):
+
+        self.flag = flag
+        self.split = split
 
         if root is not None and os.path.exists(root):
             self.root = root
         else:
             raise RuntimeError("Failed to setup the default `root` directory. " +
                                "Please specify and create the `root` directory manually.")
 
-        if download:
-            self.download()
-
-        if not os.path.exists(
-                os.path.join(self.root, "{}.npz".format(self.flag))):
-            raise RuntimeError('Dataset not found. ' +
-                               ' You can set `download=True` to download it')
-
         npz_file = np.load(os.path.join(self.root, "{}.npz".format(self.flag)))
 
-        self.split = split
-        self.transform = transform
-        self.target_transform = target_transform
-        self.as_rgb = as_rgb
+        self.info = INFO[self.flag]
 
         if self.split == 'train':
-            self.imgs = npz_file['train_images']
             self.labels = npz_file['train_labels']
         elif self.split == 'val':
-            self.imgs = npz_file['val_images']
             self.labels = npz_file['val_labels']
         elif self.split == 'test':
-            self.imgs = npz_file['test_images']
             self.labels = npz_file['test_labels']
         else:
             raise ValueError
 
-    def __len__(self):
-        return self.imgs.shape[0]
-
-    def __repr__(self):
-        '''Adapted from torchvision.ss'''
-        _repr_indent = 4
-        head = f"Dataset {self.__class__.__name__} ({self.flag})"
-        body = [f"Number of datapoints: {self.__len__()}"]
-        body.append(f"Root location: {self.root}")
-        body.append(f"Split: {self.split}")
-        body.append(f"Task: {self.info['task']}")
-        body.append(f"Number of channels: {self.info['n_channels']}")
-        body.append(f"Meaning of labels: {self.info['label']}")
-        body.append(f"Number of samples: {self.info['n_samples']}")
-        body.append(f"Description: {self.info['description']}")
-        body.append(f"License: {self.info['license']}")
-
-        lines = [head] + [" " * _repr_indent + line for line in body]
-        return '\n'.join(lines)
-
-    def download(self):
-        try:
-            from torchvision.datasets.utils import download_url
-            download_url(url=self.info["url"],
-                         root=self.root,
-                         filename="{}.npz".format(self.flag),
-                         md5=self.info["MD5"])
-        except:
-            raise RuntimeError('Something went wrong when downloading! ' +
-                               'Go to the homepage to download manually. ' +
-                               HOMEPAGE)
-
-
-class MedMNIST2D(MedMNIST):
-
-    def __getitem__(self, index):
-        '''
-        return: (without transform/target_transofrm)
-            img: PIL.Image
-            target: np.array of `L` (L=1 for single-label)
-        '''
-        img, target = self.imgs[index], self.labels[index].astype(int)
-        img = Image.fromarray(img)
-
-        if self.as_rgb:
-            img = img.convert('RGB')
-
-        if self.transform is not None:
-            img = self.transform(img)
-
-        if self.target_transform is not None:
-            target = self.target_transform(target)
-
-        return img, target
-
-    def save(self, folder, postfix="png", write_csv=True):
+    def evaluate(self, y_score, save_folder=None, run=None):
+        assert y_score.shape[0] == self.labels.shape[0]
 
-        from medmnist.utils import save2d
-
-        save2d(imgs=self.imgs,
-               labels=self.labels,
-               img_folder=os.path.join(folder, self.flag),
-               split=self.split,
-               postfix=postfix,
-               csv_path=os.path.join(folder, f"{self.flag}.csv") if write_csv else None)
-
-    def montage(self, length=20, replace=False, save_folder=None):
-        from medmnist.utils import montage2d
-
-        n_sel = length * length
-        sel = np.random.choice(self.__len__(), size=n_sel, replace=replace)
-
-        montage_img = montage2d(imgs=self.imgs,
-                                n_channels=self.info['n_channels'],
-                                sel=sel)
+        task = self.info["task"]
+        auc = getAUC(self.labels, y_score, task)
+        acc = getACC(self.labels, y_score, task)
+        metrics = Metrics(auc, acc)
 
         if save_folder is not None:
-            if not os.path.exists(save_folder):
-                os.makedirs(save_folder)
-            montage_img.save(os.path.join(save_folder,
-                                          f"{self.flag}_{self.split}_montage.jpg"))
-
-        return montage_img
+            path = os.path.join(save_folder,
+                                self.get_standard_evaluation_filename(metrics, run))
+            pd.DataFrame(y_score).to_csv(path, header=None)
+        return metrics
+
+    def get_standard_evaluation_filename(self, metrics, run=None):
+        eval_txt = "_".join(
+            [f"[{k}]{v:.3f}" for k, v in zip(metrics._fields, metrics)])
+
+        if run is None:
+            import time
+            run = time.time()
 
+        ret = f"{self.flag}_{self.split}_{eval_txt}@{run}.csv"
+        return ret
 
-class MedMNIST3D(MedMNIST):
-
-    def __getitem__(self, index):
-        '''
-        return: (without transform/target_transofrm)
-            img: an array of 1x28x28x28 or 3x28x28x28 (if `as_RGB=True`), in [0,1]
-            target: np.array of `L` (L=1 for single-label)
+    def get_dummy_prediction(self):
+        '''Return a dummy prediction of correct shape.
         '''
-        img, target = self.imgs[index], self.labels[index].astype(int)
-
-        img = np.stack([img/255.]*(3 if self.as_rgb else 1), axis=0)
-
-        if self.transform is not None:
-            img = self.transform(img)
-
-        if self.target_transform is not None:
-            target = self.target_transform(target)
-
-        return img, target
-
-    def save(self, folder, postfix="gif", write_csv=True):
-        from medmnist.utils import save3d
-
-        assert postfix == "gif"
-
-        save3d(imgs=self.imgs,
-               labels=self.labels,
-               img_folder=os.path.join(folder, self.flag),
-               split=self.split,
-               postfix=postfix,
-               csv_path=os.path.join(folder, f"{self.flag}.csv") if write_csv else None)
-
-    def montage(self, length=20, replace=False, save_folder=None):
-        assert self.info['n_channels'] == 1
-
-        from medmnist.utils import montage3d, save_frames_as_gif
-        n_sel = length * length
-        sel = np.random.choice(self.__len__(), size=n_sel, replace=replace)
-
-        montage_frames = montage3d(imgs=self.imgs,
-                                   n_channels=self.info['n_channels'],
-                                   sel=sel)
-
-        if save_folder is not None:
-            if not os.path.exists(save_folder):
-                os.makedirs(save_folder)
-
-            save_frames_as_gif(montage_frames,
-                               os.path.join(save_folder,
-                                            f"{self.flag}_{self.split}_montage.gif"))
-
-        return montage_frames
-
-
-class PathMNIST(MedMNIST2D):
-    flag = "pathmnist"
-
-
-class OCTMNIST(MedMNIST2D):
-    flag = "octmnist"
-
-
-class PneumoniaMNIST(MedMNIST2D):
-    flag = "pneumoniamnist"
-
-
-class ChestMNIST(MedMNIST2D):
-    flag = "chestmnist"
-
-
-class DermaMNIST(MedMNIST2D):
-    flag = "dermamnist"
-
-
-class RetinaMNIST(MedMNIST2D):
-    flag = "retinamnist"
-
-
-class BreastMNIST(MedMNIST2D):
-    flag = "breastmnist"
-
-
-class BloodMNIST(MedMNIST2D):
-    flag = "bloodmnist"
-
-
-class TissueMNIST(MedMNIST2D):
-    flag = "tissuemnist"
-
-
-class OrganAMNIST(MedMNIST2D):
-    flag = "organamnist"
-
-
-class OrganCMNIST(MedMNIST2D):
-    flag = "organcmnist"
-
-
-class OrganSMNIST(MedMNIST2D):
-    flag = "organsmnist"
-
-
-class OrganMNIST3D(MedMNIST3D):
-    flag = "organmnist3d"
-
-
-class NoduleMNIST3D(MedMNIST3D):
-    flag = "nodulemnist3d"
-
-
-class AdrenalMNIST3D(MedMNIST3D):
-    flag = "adrenalmnist3d"
-
-
-class FractureMNIST3D(MedMNIST3D):
-    flag = "fracturemnist3d"
-
-
-class VesselMNIST3D(MedMNIST3D):
-    flag = "vesselmnist3d"
+        task = self.info["task"]
+        if task == 'multi-class' or task == "ordinal-regression":
+            num_classes = self.labels.max()
+            dummy = np.random.rand(self.labels.shape[0], num_classes)
+            dummy = dummy/dummy.sum(axis=-1, keepdims=True)
+        else:
+            dummy = np.random.rand(*self.labels.shape)
+        return dummy
 
+    @classmethod
+    def parse_and_evaluate(cls, path, run=None):
+        '''Parse and evaluate a standard result file.
+        
+        A standard result file is named as:
+            {flag}_{split}|*|.csv (|*| means anything)
+
+        A standard evaluation file is named as:
+            {flag}_{split}_[AUC]{auc:.3f}_[ACC]{acc:.3f}@{run}.csv
+
+        In result/evaluation file, each line is (dataset index,float prediction).
+
+        For instance,
+        octmnist_test_[AUC]0.672_[ACC]0.892@3.csv
+            0,0.125,0.275,0.5,0.2
+            1,0.5,0.125,0.275,0.2
+        '''
+        folder, filename = os.path.split(path)
+        flag, split_, *_ = filename.split("_")
+        if split_.startswith('train'):
+            split = "train"
+        elif split_.startswith('val'):
+            split = "val"
+        elif split_.startswith('test'):
+            split = "test"
+        else:
+            raise ValueError
 
-class SynapseMNIST3D(MedMNIST3D):
-    flag = "synapsemnist3d"
+        if run is None:
+            assert "@" in filename
+            run = filename.split("@")[-1].split(".")[0]
+
+        evaluator = cls(flag, split)
+
+        df = pd.read_csv(path, index_col=0, header=None)
+        y_score = df.sort_index().values
+
+        metrics = evaluator.evaluate(y_score, folder, run)
+        print(metrics)
+
+        return metrics
+
+
+def getAUC(y_true, y_score, task):
+    '''AUC metric.
+    :param y_true: the ground truth labels, shape: (n_samples, n_labels) or (n_samples,) if n_labels==1
+    :param y_score: the predicted score of each class,
+    shape: (n_samples, n_labels) or (n_samples, n_classes) or (n_samples,) if n_labels==1 or n_classes==1
+    :param task: the task of current dataset
+    '''
+    y_true = y_true.squeeze()
+    y_score = y_score.squeeze()
+
+    if task == 'multi-label, binary-class':
+        auc = 0
+        for i in range(y_score.shape[1]):
+            label_auc = roc_auc_score(y_true[:, i], y_score[:, i])
+            auc += label_auc
+        ret = auc / y_score.shape[1]
+    elif task == 'binary-class':
+        if y_score.ndim == 2:
+            y_score = y_score[:, -1]
+        else:
+            assert y_score.ndim == 1
+        ret = roc_auc_score(y_true, y_score)
+    else:
+        auc = 0
+        for i in range(y_score.shape[1]):
+            y_true_binary = (y_true == i).astype(float)
+            y_score_binary = y_score[:, i]
+            auc += roc_auc_score(y_true_binary, y_score_binary)
+        ret = auc / y_score.shape[1]
+
+    return ret
+
+
+def getACC(y_true, y_score, task, threshold=0.5):
+    '''Accuracy metric.
+    :param y_true: the ground truth labels, shape: (n_samples, n_labels) or (n_samples,) if n_labels==1
+    :param y_score: the predicted score of each class,
+    shape: (n_samples, n_labels) or (n_samples, n_classes) or (n_samples,) if n_labels==1 or n_classes==1
+    :param task: the task of current dataset
+    :param threshold: the threshold for multilabel and binary-class tasks
+    '''
+    y_true = y_true.squeeze()
+    y_score = y_score.squeeze()
+
+    if task == 'multi-label, binary-class':
+        y_pre = y_score > threshold
+        acc = 0
+        for label in range(y_true.shape[1]):
+            label_acc = accuracy_score(y_true[:, label], y_pre[:, label])
+            acc += label_acc
+        ret = acc / y_true.shape[1]
+    elif task == 'binary-class':
+        if y_score.ndim == 2:
+            y_score = y_score[:, -1]
+        else:
+            assert y_score.ndim == 1
+        ret = accuracy_score(y_true, y_score > threshold)
+    else:
+        ret = accuracy_score(y_true, np.argmax(y_score, axis=-1))
+
+    return ret
+
+
+def save_results(y_true, y_score, outputpath):
+    '''Save ground truth and scores
+    :param y_true: the ground truth labels, shape: (n_samples, n_classes) for multi-label, and (n_samples,) for other tasks
+    :param y_score: the predicted score of each class, shape: (n_samples, n_classes)
+    :param outputpath: path to save the result csv
+
+    '''
+
+    warnings.DeprecationWarning("Only kept for backward compatiblility." +
+                                "Please use `Evaluator` API instead. ")
+    idx = []
+
+    idx.append('id')
+
+    for i in range(y_true.shape[1]):
+        idx.append('true_%s' % (i))
+    for i in range(y_score.shape[1]):
+        idx.append('score_%s' % (i))
+
+    df = pd.DataFrame(columns=idx)
+    for id in range(y_score.shape[0]):
+        dic = {}
+        dic['id'] = id
+        for i in range(y_true.shape[1]):
+            dic['true_%s' % (i)] = y_true[id][i]
+        for i in range(y_score.shape[1]):
+            dic['score_%s' % (i)] = y_score[id][i]
 
+        df_insert = pd.DataFrame(dic, index=[0])
+        df = df.append(df_insert, ignore_index=True)
 
-# backward-compatible
-OrganMNISTAxial = OrganAMNIST
-OrganMNISTCoronal = OrganCMNIST
-OrganMNISTSagittal = OrganSMNIST
+    df.to_csv(outputpath, sep=',', index=False,
+              header=True, encoding="utf_8_sig")
```

### Comparing `medmnist-2.2.1/medmnist/info.py` & `medmnist-2.2.2/medmnist/info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.2.1"
+__version__ = "2.2.2"
 
 
 import os
 from os.path import expanduser
 import warnings
```

### Comparing `medmnist-2.2.1/medmnist/utils.py` & `medmnist-2.2.2/medmnist/utils.py`

 * *Files identical despite different names*

### Comparing `medmnist-2.2.1/medmnist.egg-info/PKG-INFO` & `medmnist-2.2.2/medmnist.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,166 +1,168 @@
 Metadata-Version: 2.1
 Name: medmnist
-Version: 2.2.1
+Version: 2.2.2
 Summary: MedMNIST: 18 MNIST-like Datasets for 2D and 3D Biomedical Image Classification
 Home-page: https://github.com/MedMNIST/MedMNIST/
 Author: MedMNIST Team
 Author-email: jiancheng.yang@epfl.ch
 License: Apache-2.0 License
-Description: # MedMNIST: [medmnist.com](https://medmnist.github.io/)
-        ## Data ([Zenodo](https://doi.org/10.5281/zenodo.6496656)) | Publication ([Scientific Data](https://doi.org/10.1038/s41597-022-01721-8) / [arXiv](https://arxiv.org/abs/2110.14795)) | MedMNIST v1 ([ISBI'21](https://medmnist.github.io/v1)) 
-        [Jiancheng Yang](https://jiancheng-yang.com/), Rui Shi, [Donglai Wei](https://donglaiw.github.io/), Zequan Liu, Lin Zhao, [Bilian Ke](https://scholar.google.com/citations?user=2cX5y8kAAAAJ&hl=en), [Hanspeter Pfister](https://scholar.google.com/citations?user=VWX-GMAAAAAJ&hl=en), [Bingbing Ni](https://scholar.google.com/citations?user=eUbmKwYAAAAJ)
-        
-        [![](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MedMNIST/MedMNIST/blob/main/examples/getting_started.ipynb)
-        
-        We introduce *MedMNIST v2*, a large-scale MNIST-like collection of standardized biomedical images, including 12 datasets for 2D and 6 datasets for 3D. All images are pre-processed into 28x28 (2D) or 28x28x28 (3D) with the corresponding classification labels, so that no background knowledge is required for users. Covering primary data modalities in biomedical images, MedMNIST v2 is designed to perform classification on lightweight 2D and 3D images with various data scales (from 100 to 100,000) and diverse tasks (binary/multi-class, ordinal regression and multi-label). The resulting dataset, consisting of 708,069 2D images and 9,998 3D images in total, could support numerous research / educational purposes in biomedical image analysis, computer vision and machine learning. We benchmark several baseline methods on MedMNIST v2, including 2D / 3D neural networks and open-source / commercial AutoML tools. 
-        
-        ![MedMNISTv2_overview](https://raw.githubusercontent.com/MedMNIST/MedMNIST/main/assets/medmnistv2.jpg)
-        
-        For more details, please refer to our paper:
-        
-        **MedMNIST v2: A Large-Scale Lightweight Benchmark for 2D and 3D Biomedical Image Classification** ([Scientific Data](https://doi.org/10.1038/s41597-022-01721-8) / [arXiv](https://arxiv.org/abs/2110.14795))
-        
-        or its conference version:
-        
-        **MedMNIST Classification Decathlon: A Lightweight AutoML Benchmark for Medical Image Analysis** ([ISBI'21](https://arxiv.org/abs/2010.14925))
-        
-        # Key Features
-        * ***Diverse***: It covers diverse data modalities, dataset scales (from 100 to 100,000), and tasks (binary/multi-class, multi-label, and ordinal regression). It is as diverse as the VDD and MSD to fairly evaluate the generalizable performance of machine learning algorithms in different settings, but both 2D and 3D biomedical images are provided. 
-        * ***Standardized***: Each sub-dataset is pre-processed into the same format, which requires no background knowledge for users. As an MNIST-like dataset collection to perform classification tasks on small images, it primarily focuses on the machine learning part rather than the end-to-end system. Furthermore, we provide standard train-validation-test splits for all datasets in MedMNIST v2, therefore algorithms could be easily compared. 
-        * ***Lightweight***: The small size of 28×28 (2D) or 28×28×28 (3D) is friendly to evaluate machine learning algorithms. 
-        * ***Educational***: As an interdisciplinary research area, biomedical image analysis is difficult to hand on for researchers from other communities, as it requires background knowledge from computer vision, machine learning, biomedical imaging, and clinical science. Our data with the Creative Commons (CC) License is easy to use for educational purposes.
-        
-        Please note that this dataset is **NOT** intended for clinical use.
-        
-        # Code Structure
-        * [`medmnist/`](medmnist/):
-            * [`dataset.py`](medmnist/dataset.py): PyTorch datasets and dataloaders of MedMNIST.
-            * [`evaluator.py`](medmnist/evaluator.py): Standardized evaluation functions.
-            * [`info.py`](medmnist/info.py): Dataset information `dict` for each subset of MedMNIST.
-        * [`examples/`](examples/):
-            * [`getting_started.ipynb`](examples/getting_started.ipynb): To explore the MedMNIST dataset with jupyter notebook. It is ONLY intended for a quick exploration, i.e., it does not provide full training and evaluation functionalities. 
-            * [`getting_started_without_PyTorch.ipynb`](examples/getting_started_without_PyTorch.ipynb): This notebook provides snippets about how to use MedMNIST data (the `.npz` files) without PyTorch.
-        * [`setup.py`](setup.py): To install `medmnist` as a module.
-        * [EXTERNAL] [`MedMNIST/experiments`](https://github.com/MedMNIST/experiments): training and evaluation scripts to reproduce both 2D and 3D experiments in our paper, including PyTorch, auto-sklearn, AutoKeras and Google AutoML Vision together with their weights ;)
-        
-        # Installation and Requirements
-        Setup the required environments and install `medmnist` as a standard Python package from [PyPI](https://pypi.org/project/medmnist/):
-        
-            pip install medmnist
-        
-        Or install from source:
-        
-            pip install --upgrade git+https://github.com/MedMNIST/MedMNIST.git
-        
-        Check whether you have installed the latest [version](medmnist/info.py):
-        
-            >>> import medmnist
-            >>> print(medmnist.__version__)
-        
-        The code requires only common Python environments for machine learning. Basically, it was tested with
-        * Python 3 (>=3.6)
-        * PyTorch\==1.3.1
-        * numpy\==1.18.5, pandas\==0.25.3, scikit-learn\==0.22.2, Pillow\==8.0.1
-        * fire, scikit-image
-        
-        Higher (or lower) versions should also work (perhaps with minor modifications). 
-        
-        # If you use PyTorch...
-        
-        * Great! Our code is designed to work with PyTorch.
-        
-        * Explore the MedMNIST dataset with jupyter notebook ([`getting_started.ipynb`](examples/getting_started.ipynb)), and train basic neural networks in PyTorch.
-        
-        
-        # If you do not use PyTorch...
-        
-        * Although our code is tested with PyTorch, you are free to parse them with your own code (without PyTorch or even without Python!), as they are only standard NumPy serialization files. It is simple to create a dataset without PyTorch.
-        * Go to [`getting_started_without_PyTorch.ipynb`](examples/getting_started_without_PyTorch.ipynb), which provides snippets about how to use MedMNIST data (the `.npz` files) without PyTorch.
-        * Simply change the super class of `MedMNIST` from `torch.utils.data.Dataset` to `collections.Sequence`, you will get a standard dataset without PyTorch. Check [`dataset_without_pytorch.py`](examples/dataset_without_pytorch.py) for more details.
-        * You still have most functionality of our MedMNIST code ;)
-        
-        # Dataset
-        
-        Please download the dataset(s) via [`Zenodo`](https://doi.org/10.5281/zenodo.6496656). You could also use our code to download automatically by setting `download=True` in [`dataset.py`](medmnist/dataset.py).
-        
-        The MedMNIST dataset contains several subsets. Each subset (e.g., `pathmnist.npz`) is comprised of 6 keys: `train_images`, `train_labels`, `val_images`, `val_labels`, `test_images` and `test_labels`.
-        * `train_images` / `val_images` / `test_images`: `N` × 28 × 28 for 2D gray-scale datasets, `N` × 28 × 28 × 3 for 2D RGB datasets, `N` × 28 × 28 × 28 for 3D datasets. `N` denotes the number of samples.  
-        * `train_labels` / `val_labels` / `test_labels`: `N` x `L`. `N` denotes the number of samples. `L` denotes the number of task labels; for single-label (binary/multi-class) classification, `L=1`, and `{0,1,2,3,..,C}` denotes the category labels (`C=1` for binary); for multi-label classification `L!=1`, e.g., `L=14` for `chestmnist.npz`.
-        
-        # Command Line Tools
-        
-        * List all available datasets:
-            
-                python -m medmnist available
-        
-        * Download all available datasets:
-            
-                python -m medmnist download
-        
-        * Delete all downloaded npz from root:
-        
-                python -m medmnist clean
-        
-        * Print the dataset details given a subset flag:
-        
-                python -m medmnist info --flag=xxxmnist
-        
-        * Save the dataset as standard figure and csv files, which could be used for AutoML tools, e.g., Google AutoML Vision:
-        
-            for 2D datasets:
-        
-                python -m medmnist save --flag=xxxmnist --folder=tmp/ --postfix=png
-                
-            for 3D datasets:
-        
-                python -m medmnist save --flag=xxxmnist3d --folder=tmp/ --postfix=gif
-        
-        * Parse and evaluate a standard result file, refer to [`Evaluator.parse_and_evaluate`](medmnist/evaluator.py) for details.
-        
-                python -m medmnist evaluate --path=folder/{flag}_{split}@{run}.csv
-        
-        # License and Citation
-        
-        The code is under [Apache-2.0 License](./LICENSE).
-        
-        The MedMNIST dataset is licensed under *Creative Commons Attribution 4.0 International* ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)).
-        If you find this project useful in your research, please cite the following papers:
-        
-            Jiancheng Yang, Rui Shi, Donglai Wei, Zequan Liu, Lin Zhao, Bilian Ke, Hanspeter Pfister, Bingbing Ni. Yang, Jiancheng, et al. "MedMNIST v2-A large-scale lightweight benchmark for 2D and 3D biomedical image classification." Scientific Data, 2023.
-        
-            Jiancheng Yang, Rui Shi, Bingbing Ni. "MedMNIST Classification Decathlon: A Lightweight AutoML Benchmark for Medical Image Analysis". IEEE 18th International Symposium on Biomedical Imaging (ISBI), 2021.
-        
-        or using the bibtex:
-        
-            @article{medmnistv2,
-                title={MedMNIST v2-A large-scale lightweight benchmark for 2D and 3D biomedical image classification},
-                author={Yang, Jiancheng and Shi, Rui and Wei, Donglai and Liu, Zequan and Zhao, Lin and Ke, Bilian and Pfister, Hanspeter and Ni, Bingbing},
-                journal={Scientific Data},
-                volume={10},
-                number={1},
-                pages={41},
-                year={2023},
-                publisher={Nature Publishing Group UK London}
-            }
-             
-            @inproceedings{medmnistv1,
-                title={MedMNIST Classification Decathlon: A Lightweight AutoML Benchmark for Medical Image Analysis},
-                author={Yang, Jiancheng and Shi, Rui and Ni, Bingbing},
-                booktitle={IEEE 18th International Symposium on Biomedical Imaging (ISBI)},
-                pages={191--195},
-                year={2021}
-            }
-        
-        Please also cite source data paper(s) of the MedMNIST subset(s) as per the description on the [project page](https://medmnist.github.io/).
-        
-        # Release Notes
-        * `v2.2.1`: PyPI info updated
-        * `v2.2.0`: `montage` method supported for scikit-image>=0.20.0
-        * `v2.1.0`: `NoduleMNIST3D` data error fixed
-        * `v2.0.0`: MedMNIST v2 release
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# MedMNIST: [medmnist.com](https://medmnist.github.io/)
+## Data ([Zenodo](https://doi.org/10.5281/zenodo.6496656)) | Publication ([Scientific Data](https://doi.org/10.1038/s41597-022-01721-8) / [arXiv](https://arxiv.org/abs/2110.14795)) | MedMNIST v1 ([ISBI'21](https://medmnist.github.io/v1)) 
+[Jiancheng Yang](https://jiancheng-yang.com/), Rui Shi, [Donglai Wei](https://donglaiw.github.io/), Zequan Liu, Lin Zhao, [Bilian Ke](https://scholar.google.com/citations?user=2cX5y8kAAAAJ&hl=en), [Hanspeter Pfister](https://scholar.google.com/citations?user=VWX-GMAAAAAJ&hl=en), [Bingbing Ni](https://scholar.google.com/citations?user=eUbmKwYAAAAJ)
+
+[![](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MedMNIST/MedMNIST/blob/main/examples/getting_started.ipynb)
+
+We introduce *MedMNIST v2*, a large-scale MNIST-like collection of standardized biomedical images, including 12 datasets for 2D and 6 datasets for 3D. All images are pre-processed into 28x28 (2D) or 28x28x28 (3D) with the corresponding classification labels, so that no background knowledge is required for users. Covering primary data modalities in biomedical images, MedMNIST v2 is designed to perform classification on lightweight 2D and 3D images with various data scales (from 100 to 100,000) and diverse tasks (binary/multi-class, ordinal regression and multi-label). The resulting dataset, consisting of 708,069 2D images and 9,998 3D images in total, could support numerous research / educational purposes in biomedical image analysis, computer vision and machine learning. We benchmark several baseline methods on MedMNIST v2, including 2D / 3D neural networks and open-source / commercial AutoML tools. 
+
+![MedMNISTv2_overview](https://raw.githubusercontent.com/MedMNIST/MedMNIST/main/assets/medmnistv2.jpg)
+
+For more details, please refer to our paper:
+
+**MedMNIST v2: A Large-Scale Lightweight Benchmark for 2D and 3D Biomedical Image Classification** ([Scientific Data](https://doi.org/10.1038/s41597-022-01721-8) / [arXiv](https://arxiv.org/abs/2110.14795))
+
+or its conference version:
+
+**MedMNIST Classification Decathlon: A Lightweight AutoML Benchmark for Medical Image Analysis** ([ISBI'21](https://arxiv.org/abs/2010.14925))
+
+# Key Features
+* ***Diverse***: It covers diverse data modalities, dataset scales (from 100 to 100,000), and tasks (binary/multi-class, multi-label, and ordinal regression). It is as diverse as the VDD and MSD to fairly evaluate the generalizable performance of machine learning algorithms in different settings, but both 2D and 3D biomedical images are provided. 
+* ***Standardized***: Each sub-dataset is pre-processed into the same format, which requires no background knowledge for users. As an MNIST-like dataset collection to perform classification tasks on small images, it primarily focuses on the machine learning part rather than the end-to-end system. Furthermore, we provide standard train-validation-test splits for all datasets in MedMNIST v2, therefore algorithms could be easily compared. 
+* ***Lightweight***: The small size of 28×28 (2D) or 28×28×28 (3D) is friendly to evaluate machine learning algorithms. 
+* ***Educational***: As an interdisciplinary research area, biomedical image analysis is difficult to hand on for researchers from other communities, as it requires background knowledge from computer vision, machine learning, biomedical imaging, and clinical science. Our data with the Creative Commons (CC) License is easy to use for educational purposes.
+
+Please note that this dataset is **NOT** intended for clinical use.
+
+# Code Structure
+* [`medmnist/`](medmnist/):
+    * [`dataset.py`](medmnist/dataset.py): PyTorch datasets and dataloaders of MedMNIST.
+    * [`evaluator.py`](medmnist/evaluator.py): Standardized evaluation functions.
+    * [`info.py`](medmnist/info.py): Dataset information `dict` for each subset of MedMNIST.
+* [`examples/`](examples/):
+    * [`getting_started.ipynb`](examples/getting_started.ipynb): To explore the MedMNIST dataset with jupyter notebook. It is ONLY intended for a quick exploration, i.e., it does not provide full training and evaluation functionalities. 
+    * [`getting_started_without_PyTorch.ipynb`](examples/getting_started_without_PyTorch.ipynb): This notebook provides snippets about how to use MedMNIST data (the `.npz` files) without PyTorch.
+* [`setup.py`](setup.py): To install `medmnist` as a module.
+* [EXTERNAL] [`MedMNIST/experiments`](https://github.com/MedMNIST/experiments): training and evaluation scripts to reproduce both 2D and 3D experiments in our paper, including PyTorch, auto-sklearn, AutoKeras and Google AutoML Vision together with their weights ;)
+
+# Installation and Requirements
+Setup the required environments and install `medmnist` as a standard Python package from [PyPI](https://pypi.org/project/medmnist/):
+
+    pip install medmnist
+
+Or install from source:
+
+    pip install --upgrade git+https://github.com/MedMNIST/MedMNIST.git
+
+Check whether you have installed the latest [version](medmnist/info.py):
+
+    >>> import medmnist
+    >>> print(medmnist.__version__)
+
+The code requires only common Python environments for machine learning. Basically, it was tested with
+* Python 3 (>=3.6)
+* PyTorch\==1.3.1
+* numpy\==1.18.5, pandas\==0.25.3, scikit-learn\==0.22.2, Pillow\==8.0.1
+* fire, scikit-image
+
+Higher (or lower) versions should also work (perhaps with minor modifications). 
+
+# If you use PyTorch...
+
+* Great! Our code is designed to work with PyTorch.
+
+* Explore the MedMNIST dataset with jupyter notebook ([`getting_started.ipynb`](examples/getting_started.ipynb)), and train basic neural networks in PyTorch.
+
+
+# If you do not use PyTorch...
+
+* Although our code is tested with PyTorch, you are free to parse them with your own code (without PyTorch or even without Python!), as they are only standard NumPy serialization files. It is simple to create a dataset without PyTorch.
+* Go to [`getting_started_without_PyTorch.ipynb`](examples/getting_started_without_PyTorch.ipynb), which provides snippets about how to use MedMNIST data (the `.npz` files) without PyTorch.
+* Simply change the super class of `MedMNIST` from `torch.utils.data.Dataset` to `collections.Sequence`, you will get a standard dataset without PyTorch. Check [`dataset_without_pytorch.py`](examples/dataset_without_pytorch.py) for more details.
+* You still have most functionality of our MedMNIST code ;)
+
+# Dataset
+
+Please download the dataset(s) via [`Zenodo`](https://doi.org/10.5281/zenodo.6496656). You could also use our code to download automatically by setting `download=True` in [`dataset.py`](medmnist/dataset.py).
+
+The MedMNIST dataset contains several subsets. Each subset (e.g., `pathmnist.npz`) is comprised of 6 keys: `train_images`, `train_labels`, `val_images`, `val_labels`, `test_images` and `test_labels`.
+* `train_images` / `val_images` / `test_images`: `N` × 28 × 28 for 2D gray-scale datasets, `N` × 28 × 28 × 3 for 2D RGB datasets, `N` × 28 × 28 × 28 for 3D datasets. `N` denotes the number of samples.  
+* `train_labels` / `val_labels` / `test_labels`: `N` x `L`. `N` denotes the number of samples. `L` denotes the number of task labels; for single-label (binary/multi-class) classification, `L=1`, and `{0,1,2,3,..,C}` denotes the category labels (`C=1` for binary); for multi-label classification `L!=1`, e.g., `L=14` for `chestmnist.npz`.
+
+# Command Line Tools
+
+* List all available datasets:
+    
+        python -m medmnist available
+
+* Download all available datasets:
+    
+        python -m medmnist download
+
+* Delete all downloaded npz from root:
+
+        python -m medmnist clean
+
+* Print the dataset details given a subset flag:
+
+        python -m medmnist info --flag=xxxmnist
+
+* Save the dataset as standard figure and csv files, which could be used for AutoML tools, e.g., Google AutoML Vision:
+
+    for 2D datasets:
+
+        python -m medmnist save --flag=xxxmnist --folder=tmp/ --postfix=png
+        
+    for 3D datasets:
+
+        python -m medmnist save --flag=xxxmnist3d --folder=tmp/ --postfix=gif
+
+* Parse and evaluate a standard result file, refer to [`Evaluator.parse_and_evaluate`](medmnist/evaluator.py) for details.
+
+        python -m medmnist evaluate --path=folder/{flag}_{split}@{run}.csv
+
+# License and Citation
+
+The code is under [Apache-2.0 License](./LICENSE).
+
+The MedMNIST dataset is licensed under *Creative Commons Attribution 4.0 International* ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)).
+If you find this project useful in your research, please cite the following papers:
+
+    Jiancheng Yang, Rui Shi, Donglai Wei, Zequan Liu, Lin Zhao, Bilian Ke, Hanspeter Pfister, Bingbing Ni. Yang, Jiancheng, et al. "MedMNIST v2-A large-scale lightweight benchmark for 2D and 3D biomedical image classification." Scientific Data, 2023.
+
+    Jiancheng Yang, Rui Shi, Bingbing Ni. "MedMNIST Classification Decathlon: A Lightweight AutoML Benchmark for Medical Image Analysis". IEEE 18th International Symposium on Biomedical Imaging (ISBI), 2021.
+
+or using the bibtex:
+
+    @article{medmnistv2,
+        title={MedMNIST v2-A large-scale lightweight benchmark for 2D and 3D biomedical image classification},
+        author={Yang, Jiancheng and Shi, Rui and Wei, Donglai and Liu, Zequan and Zhao, Lin and Ke, Bilian and Pfister, Hanspeter and Ni, Bingbing},
+        journal={Scientific Data},
+        volume={10},
+        number={1},
+        pages={41},
+        year={2023},
+        publisher={Nature Publishing Group UK London}
+    }
+     
+    @inproceedings{medmnistv1,
+        title={MedMNIST Classification Decathlon: A Lightweight AutoML Benchmark for Medical Image Analysis},
+        author={Yang, Jiancheng and Shi, Rui and Ni, Bingbing},
+        booktitle={IEEE 18th International Symposium on Biomedical Imaging (ISBI)},
+        pages={191--195},
+        year={2021}
+    }
+
+Please also cite source data paper(s) of the MedMNIST subset(s) as per the description on the [project page](https://medmnist.github.io/).
+
+# Release Notes
+* `v2.2.2`: Python 3.11 `Sequence` from collections.abc supported
+* `v2.2.1`: PyPI info updated
+* `v2.2.0`: `montage` method supported for scikit-image>=0.20.0
+* `v2.1.0`: `NoduleMNIST3D` data error fixed
+* `v2.0.0`: MedMNIST v2 release
```

### Comparing `medmnist-2.2.1/setup.py` & `medmnist-2.2.2/setup.py`

 * *Files identical despite different names*

