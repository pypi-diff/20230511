# Comparing `tmp/aac_datasets-0.3.1.tar.gz` & `tmp/aac_datasets-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aac_datasets-0.3.1.tar", last modified: Mon Oct 31 09:57:48 2022, max compression
+gzip compressed data, was "aac_datasets-0.3.2.tar", last modified: Mon Jan 30 13:48:38 2023, max compression
```

## Comparing `aac_datasets-0.3.1.tar` & `aac_datasets-0.3.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2022-10-31 09:57:48.835198 aac_datasets-0.3.1/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1081 2022-06-03 12:09:27.000000 aac_datasets-0.3.1/LICENSE
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       76 2022-10-31 09:56:50.000000 aac_datasets-0.3.1/MANIFEST.in
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5745 2022-10-31 09:57:48.835198 aac_datasets-0.3.1/PKG-INFO
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4969 2022-10-31 09:56:50.000000 aac_datasets-0.3.1/README.md
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2022-10-31 09:57:48.831198 aac_datasets-0.3.1/docs/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2921 2022-08-30 10:15:41.000000 aac_datasets-0.3.1/docs/conf.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1331 2022-10-31 09:57:48.835198 aac_datasets-0.3.1/setup.cfg
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      117 2022-06-03 12:09:27.000000 aac_datasets-0.3.1/setup.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2022-10-31 09:57:48.831198 aac_datasets-0.3.1/src/
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2022-10-31 09:57:48.831198 aac_datasets-0.3.1/src/aac_datasets/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      425 2022-10-31 09:56:50.000000 aac_datasets-0.3.1/src/aac_datasets/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      559 2022-09-28 09:57:04.000000 aac_datasets-0.3.1/src/aac_datasets/__main__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3266 2022-09-28 09:57:04.000000 aac_datasets-0.3.1/src/aac_datasets/check.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2022-10-31 09:57:48.831198 aac_datasets-0.3.1/src/aac_datasets/datasets/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      340 2022-08-30 10:15:41.000000 aac_datasets-0.3.1/src/aac_datasets/datasets/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    28537 2022-10-31 09:56:50.000000 aac_datasets-0.3.1/src/aac_datasets/datasets/audiocaps.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    29662 2022-10-31 09:56:50.000000 aac_datasets-0.3.1/src/aac_datasets/datasets/clotho.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    26130 2022-10-31 09:56:50.000000 aac_datasets-0.3.1/src/aac_datasets/datasets/macs.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6852 2022-09-28 09:57:04.000000 aac_datasets-0.3.1/src/aac_datasets/download.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      956 2022-09-28 09:57:04.000000 aac_datasets-0.3.1/src/aac_datasets/info.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2022-10-31 09:57:48.831198 aac_datasets-0.3.1/src/aac_datasets/utils/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      126 2022-09-28 09:57:04.000000 aac_datasets-0.3.1/src/aac_datasets/utils/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4162 2022-09-28 09:57:04.000000 aac_datasets-0.3.1/src/aac_datasets/utils/collate.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2206 2022-10-31 09:57:30.000000 aac_datasets-0.3.1/src/aac_datasets/utils.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      946 2022-10-31 09:57:30.000000 aac_datasets-0.3.1/src/aac_datasets/version.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2022-10-31 09:57:48.835198 aac_datasets-0.3.1/src/aac_datasets.egg-info/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5745 2022-10-31 09:57:48.000000 aac_datasets-0.3.1/src/aac_datasets.egg-info/PKG-INFO
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1100 2022-10-31 09:57:48.000000 aac_datasets-0.3.1/src/aac_datasets.egg-info/SOURCES.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        1 2022-10-31 09:57:48.000000 aac_datasets-0.3.1/src/aac_datasets.egg-info/dependency_links.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      239 2022-10-31 09:57:48.000000 aac_datasets-0.3.1/src/aac_datasets.egg-info/entry_points.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      165 2022-10-31 09:57:48.000000 aac_datasets-0.3.1/src/aac_datasets.egg-info/requires.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       13 2022-10-31 09:57:48.000000 aac_datasets-0.3.1/src/aac_datasets.egg-info/top_level.txt
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-01-30 13:48:38.884543 aac_datasets-0.3.2/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1081 2022-06-03 12:09:27.000000 aac_datasets-0.3.2/LICENSE
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       76 2022-10-31 09:56:50.000000 aac_datasets-0.3.2/MANIFEST.in
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5854 2023-01-30 13:48:38.884543 aac_datasets-0.3.2/PKG-INFO
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5098 2023-01-30 13:48:13.000000 aac_datasets-0.3.2/README.md
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-01-30 13:48:38.880543 aac_datasets-0.3.2/docs/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3153 2023-01-30 13:48:13.000000 aac_datasets-0.3.2/docs/conf.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1331 2023-01-30 13:48:38.884543 aac_datasets-0.3.2/setup.cfg
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      117 2022-06-03 12:09:27.000000 aac_datasets-0.3.2/setup.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-01-30 13:48:38.880543 aac_datasets-0.3.2/src/
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-01-30 13:48:38.880543 aac_datasets-0.3.2/src/aac_datasets/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      425 2023-01-30 13:48:13.000000 aac_datasets-0.3.2/src/aac_datasets/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      559 2022-09-28 09:57:04.000000 aac_datasets-0.3.2/src/aac_datasets/__main__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3266 2022-09-28 09:57:04.000000 aac_datasets-0.3.2/src/aac_datasets/check.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-01-30 13:48:38.880543 aac_datasets-0.3.2/src/aac_datasets/datasets/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      340 2022-08-30 10:15:41.000000 aac_datasets-0.3.2/src/aac_datasets/datasets/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    29285 2023-01-30 13:48:13.000000 aac_datasets-0.3.2/src/aac_datasets/datasets/audiocaps.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    30031 2023-01-30 13:48:13.000000 aac_datasets-0.3.2/src/aac_datasets/datasets/clotho.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    26435 2023-01-30 13:48:13.000000 aac_datasets-0.3.2/src/aac_datasets/datasets/macs.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6852 2022-09-28 09:57:04.000000 aac_datasets-0.3.2/src/aac_datasets/download.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      956 2022-09-28 09:57:04.000000 aac_datasets-0.3.2/src/aac_datasets/info.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-01-30 13:48:38.880543 aac_datasets-0.3.2/src/aac_datasets/utils/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      126 2022-09-28 09:57:04.000000 aac_datasets-0.3.2/src/aac_datasets/utils/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4170 2023-01-30 13:48:13.000000 aac_datasets-0.3.2/src/aac_datasets/utils/collate.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2206 2023-01-30 13:47:59.000000 aac_datasets-0.3.2/src/aac_datasets/utils.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      946 2023-01-30 13:47:59.000000 aac_datasets-0.3.2/src/aac_datasets/version.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2023-01-30 13:48:38.884543 aac_datasets-0.3.2/src/aac_datasets.egg-info/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5854 2023-01-30 13:48:38.000000 aac_datasets-0.3.2/src/aac_datasets.egg-info/PKG-INFO
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1100 2023-01-30 13:48:38.000000 aac_datasets-0.3.2/src/aac_datasets.egg-info/SOURCES.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        1 2023-01-30 13:48:38.000000 aac_datasets-0.3.2/src/aac_datasets.egg-info/dependency_links.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      238 2023-01-30 13:48:38.000000 aac_datasets-0.3.2/src/aac_datasets.egg-info/entry_points.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      165 2023-01-30 13:48:38.000000 aac_datasets-0.3.2/src/aac_datasets.egg-info/requires.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       13 2023-01-30 13:48:38.000000 aac_datasets-0.3.2/src/aac_datasets.egg-info/top_level.txt
```

### Comparing `aac_datasets-0.3.1/LICENSE` & `aac_datasets-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aac_datasets-0.3.1/PKG-INFO` & `aac_datasets-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: aac_datasets
-Version: 0.3.1
+Version: 0.3.2
 Summary: Audio Captioning datasets for Pytorch.
 Home-page: https://pypi.org/project/aac-datasets/
 Author: Etienne Labbé (Labbeti)
 License: MIT
 Project-URL: Documentation, https://aac-datasets.readthedocs.io/
 Project-URL: Source, https://github.com/Labbeti/aac-datasets
 Project-URL: PyPI, https://pypi.org/project/aac-datasets/
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <!-- # -*- coding: utf-8 -*- -->
 
 <div align="center">
 
-# Audio Captioning datasets for Pytorch
+# Audio Captioning datasets for PyTorch
 
 <a href="https://www.python.org/"><img alt="Python" src="https://img.shields.io/badge/-Python 3.8+-blue?style=for-the-badge&logo=python&logoColor=white"></a>
-<a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/-PyTorch 1.10.1-ee4c2c?style=for-the-badge&logo=pytorch&logoColor=white"></a>
+<a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/-PyTorch 1.10.1+-ee4c2c?style=for-the-badge&logo=pytorch&logoColor=white"></a>
 <a href="https://black.readthedocs.io/en/stable/"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-black.svg?style=for-the-badge&labelColor=gray"></a>
-<a href="https://github.com/Labbeti/aac-datasets/actions"><img alt="Build" src="https://img.shields.io/github/workflow/status/Labbeti/aac-datasets/Python%20package%20using%20Pip/main?style=for-the-badge&logo=github"></a>
+<a href="https://github.com/Labbeti/aac-datasets/actions"><img alt="Build" src="https://img.shields.io/github/actions/workflow/status/Labbeti/aac-datasets/python-package-pip.yaml?branch=main&style=for-the-badge&logo=github"></a>
 
-Audio Captioning unofficial datasets source code for **AudioCaps** [[1]](#audiocaps), **Clotho** [[2]](#clotho), and **MACS** [[3]](#macs), designed for Pytorch.
+Audio Captioning unofficial datasets source code for **AudioCaps** [[1]](#audiocaps), **Clotho** [[2]](#clotho), and **MACS** [[3]](#macs), designed for PyTorch.
 
 </div>
 
 ## Installation
 ```bash
 pip install aac-datasets
 ```
@@ -42,34 +41,34 @@
 ## Examples
 
 ### Create Clotho dataset
 
 ```python
 from aac_datasets import Clotho
 
-dataset = Clotho(root=".", subset="dev", download=True)
+dataset = Clotho(root=".", download=True)
 item = dataset[0]
 audio, captions = item["audio"], item["captions"]
 # audio: Tensor of shape (n_channels=1, audio_max_size)
-# captions: list of str captions
+# captions: list of str
 ```
 
-### Build Pytorch dataloader with Clotho
+### Build PyTorch dataloader with Clotho
 
 ```python
 from torch.utils.data.dataloader import DataLoader
 from aac_datasets import Clotho
 from aac_datasets.utils import BasicCollate
 
 dataset = Clotho(root=".", download=True)
 dataloader = DataLoader(dataset, batch_size=4, collate_fn=BasicCollate())
 
 for batch in dataloader:
-    # batch["audio"]: list of Tensor of shape (n_channels, audio_size)
-    # batch["captions"]: list of list of str
+    # batch["audio"]: list of 4 tensors of shape (n_channels, audio_size)
+    # batch["captions"]: list of 4 lists of str
     ...
 ```
 
 ## Datasets stats
 Here is the statistics for each dataset :
 
 | | AudioCaps | Clotho | MACS |
@@ -85,15 +84,15 @@
 |:---:|:---:|:---:|:---:|
 | Nb audios | 49838 | 3840 | 3930 |
 | Total audio duration | 136.6h<sup>1</sup> | 24.0h | 10.9h |
 | Audio duration range | 0.5-10s | 15-30s | 10s |
 | Nb captions per audio | 1 | 5 | 2-5 |
 | Nb captions | 49838 | 19195 | 17275 |
 | Total nb words<sup>2</sup> | 402482 | 217362 | 160006 |
-| Nb words range<sup>2</sup> | 2-52 | 8-20 | 5-40 |
+| Sentence size<sup>2</sup> | 2-52 | 8-20 | 5-40 |
 
 <sup>1</sup> This duration is estimated on the total duration of 46230/49838 files of 126.7h.
 
 <sup>2</sup> The sentences are cleaned (lowercase+remove punctuation) and tokenized using the spacy tokenizer to count the words.
 
 ## Requirements
 ### Python packages
@@ -116,19 +115,26 @@
 ```python
 from aac_datasets import AudioCaps
 AudioCaps.FFMPEG_PATH = "/my/path/to/ffmpeg"
 AudioCaps.YOUTUBE_DL_PATH = "/my/path/to/youtube_dl"
 dataset = AudioCaps(root=".", download=True)
 ```
 
-## Command line download
+## Download datasets
 To download a dataset, you can use `download=True` argument in dataset construction.
+
 However, if you want to download datasets separately, you can also use the following command :
 ```bash
-python -m aac_datasets.download --root "./data" clotho --version "v2.1"
+aac-datasets-download --root "." clotho --subsets "dev"
+```
+Or use the corresponding function in the code :
+```python
+from aac_datasets.download import download_clotho
+
+download_clotho(root=".", subsets=["dev"])
 ```
 
 ## References
 #### AudioCaps
 [1] C. D. Kim, B. Kim, H. Lee, and G. Kim, “Audiocaps: Generating captions for audios in the wild,” in NAACL-HLT, 2019. Available: https://aclanthology.org/N19-1011/
 
 #### Clotho
@@ -141,20 +147,18 @@
 If you use this software, please consider cite it as below :
 
 ```
 @software{
     Labbe_aac-datasets_2022,
     author = {Labbé, Etienne},
     license = {MIT},
-    month = {6},
+    month = {01},
     title = {{aac-datasets}},
     url = {https://github.com/Labbeti/aac-datasets/},
-    version = {0.3.1},
-    year = {2022}
+    version = {0.3.2},
+    year = {2023}
 }
 ```
 
 ## Contact
 Maintainer:
 - Etienne Labbé "Labbeti": labbeti.pub@gmail.com
-
-
```

#### html2text {}

```diff
@@ -1,66 +1,67 @@
-Metadata-Version: 2.1 Name: aac_datasets Version: 0.3.1 Summary: Audio
+Metadata-Version: 2.1 Name: aac_datasets Version: 0.3.2 Summary: Audio
 Captioning datasets for Pytorch. Home-page: https://pypi.org/project/aac-
 datasets/ Author: Etienne LabbÃ© (Labbeti) License: MIT Project-URL:
 Documentation, https://aac-datasets.readthedocs.io/ Project-URL: Source, https:
 //github.com/Labbeti/aac-datasets Project-URL: PyPI, https://pypi.org/project/
-aac-datasets/ Platform: UNKNOWN Classifier: Intended Audience :: Science/
-Research Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3.8 Classifier: Topic :: Scientific/
-Engineering Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Requires-Python: >=3.8 Description-Content-Type: text/markdown
-Provides-Extra: dev License-File: LICENSE
-# Audio Captioning datasets for Pytorch [Python] [PyTorch] [Code_style:_black]
+aac-datasets/ Classifier: Intended Audience :: Science/Research Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3.8 Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.7
+Description-Content-Type: text/markdown Provides-Extra: dev License-File:
+LICENSE
+# Audio Captioning datasets for PyTorch [Python] [PyTorch] [Code_style:_black]
  [Build] Audio Captioning unofficial datasets source code for **AudioCaps** [
     [1]](#audiocaps), **Clotho** [[2]](#clotho), and **MACS** [[3]](#macs),
-                             designed for Pytorch.
+                             designed for PyTorch.
 ## Installation ```bash pip install aac-datasets ``` ## Examples ### Create
 Clotho dataset ```python from aac_datasets import Clotho dataset = Clotho
-(root=".", subset="dev", download=True) item = dataset[0] audio, captions =
-item["audio"], item["captions"] # audio: Tensor of shape (n_channels=1,
-audio_max_size) # captions: list of str captions ``` ### Build Pytorch
-dataloader with Clotho ```python from torch.utils.data.dataloader import
-DataLoader from aac_datasets import Clotho from aac_datasets.utils import
-BasicCollate dataset = Clotho(root=".", download=True) dataloader = DataLoader
-(dataset, batch_size=4, collate_fn=BasicCollate()) for batch in dataloader: #
-batch["audio"]: list of Tensor of shape (n_channels, audio_size) # batch
-["captions"]: list of list of str ... ``` ## Datasets stats Here is the
-statistics for each dataset : | | AudioCaps | Clotho | MACS | |:---:|:---:|:--
--:|:---:| | Subset(s) | train, val, test | dev, val, eval, test, analysis |
-full | | Sample rate | 32000 | 44100 | 48000 | | Estimated size | 43GB | 27GB |
-13GB | | Audio source | AudioSet (youtube) | Freesound | TAU Urban Acoustic
-Scenes 2019 | Here is the **train** subset statistics for each dataset : | |
-AudioCaps/train | Clotho/dev | MACS/full | |:---:|:---:|:---:|:---:| | Nb
-audios | 49838 | 3840 | 3930 | | Total audio duration | 136.6h1 | 24.0h | 10.9h
-| | Audio duration range | 0.5-10s | 15-30s | 10s | | Nb captions per audio | 1
-| 5 | 2-5 | | Nb captions | 49838 | 19195 | 17275 | | Total nb words2 | 402482
-| 217362 | 160006 | | Nb words range2 | 2-52 | 8-20 | 5-40 | 1 This duration is
-estimated on the total duration of 46230/49838 files of 126.7h. 2 The sentences
-are cleaned (lowercase+remove punctuation) and tokenized using the spacy
-tokenizer to count the words. ## Requirements ### Python packages The
-requirements are automatically installed when using pip on this repository. ```
-torch >= 1.10.1 torchaudio >= 0.10.1 py7zr >= 0.17.2 pyyaml >= 6.0 tqdm >=
-4.64.0 ``` ### External requirements (AudioCaps only) The external requirements
-needed to download **AudioCaps** are **ffmpeg** and **youtube-dl**. These two
-programs can be download on Ubuntu using `sudo apt install ffmpeg youtube-dl`.
-You can also override their paths for AudioCaps: ```python from aac_datasets
-import AudioCaps AudioCaps.FFMPEG_PATH = "/my/path/to/ffmpeg"
-AudioCaps.YOUTUBE_DL_PATH = "/my/path/to/youtube_dl" dataset = AudioCaps
-(root=".", download=True) ``` ## Command line download To download a dataset,
-you can use `download=True` argument in dataset construction. However, if you
-want to download datasets separately, you can also use the following command :
-```bash python -m aac_datasets.download --root "./data" clotho --version "v2.1"
-``` ## References #### AudioCaps [1] C. D. Kim, B. Kim, H. Lee, and G. Kim,
-âAudiocaps: Generating captions for audios in the wild,â in NAACL-HLT,
-2019. Available: https://aclanthology.org/N19-1011/ #### Clotho [2] K. Drossos,
-S. Lipping, and T. Virtanen, âClotho: An Audio Captioning Dataset,â arXiv:
-1910.09387 [cs, eess], Oct. 2019, Available: http://arxiv.org/abs/1910.09387
-#### MACS [3] F. Font, A. Mesaros, D. P. W. Ellis, E. Fonseca, M. Fuentes, and
-B. Elizalde, Proceedings of the 6th Workshop on Detection and Classication of
-Acoustic Scenes and Events (DCASE 2021). Barcelona, Spain: Music Technology
-Group - Universitat Pompeu Fabra, Nov. 2021. Available: https://doi.org/
-10.5281/zenodo.5770113 ## Cite the aac-datasets package If you use this
-software, please consider cite it as below : ``` @software{ Labbe_aac-
-datasets_2022, author = {LabbÃ©, Etienne}, license = {MIT}, month = {6}, title
-= {{aac-datasets}}, url = {https://github.com/Labbeti/aac-datasets/}, version =
-{0.3.1}, year = {2022} } ``` ## Contact Maintainer: - Etienne LabbÃ© "Labbeti":
-labbeti.pub@gmail.com
+(root=".", download=True) item = dataset[0] audio, captions = item["audio"],
+item["captions"] # audio: Tensor of shape (n_channels=1, audio_max_size) #
+captions: list of str ``` ### Build PyTorch dataloader with Clotho ```python
+from torch.utils.data.dataloader import DataLoader from aac_datasets import
+Clotho from aac_datasets.utils import BasicCollate dataset = Clotho(root=".",
+download=True) dataloader = DataLoader(dataset, batch_size=4,
+collate_fn=BasicCollate()) for batch in dataloader: # batch["audio"]: list of 4
+tensors of shape (n_channels, audio_size) # batch["captions"]: list of 4 lists
+of str ... ``` ## Datasets stats Here is the statistics for each dataset : | |
+AudioCaps | Clotho | MACS | |:---:|:---:|:---:|:---:| | Subset(s) | train, val,
+test | dev, val, eval, test, analysis | full | | Sample rate | 32000 | 44100 |
+48000 | | Estimated size | 43GB | 27GB | 13GB | | Audio source | AudioSet
+(youtube) | Freesound | TAU Urban Acoustic Scenes 2019 | Here is the **train**
+subset statistics for each dataset : | | AudioCaps/train | Clotho/dev | MACS/
+full | |:---:|:---:|:---:|:---:| | Nb audios | 49838 | 3840 | 3930 | | Total
+audio duration | 136.6h1 | 24.0h | 10.9h | | Audio duration range | 0.5-10s |
+15-30s | 10s | | Nb captions per audio | 1 | 5 | 2-5 | | Nb captions | 49838 |
+19195 | 17275 | | Total nb words2 | 402482 | 217362 | 160006 | | Sentence size2
+| 2-52 | 8-20 | 5-40 | 1 This duration is estimated on the total duration of
+46230/49838 files of 126.7h. 2 The sentences are cleaned (lowercase+remove
+punctuation) and tokenized using the spacy tokenizer to count the words. ##
+Requirements ### Python packages The requirements are automatically installed
+when using pip on this repository. ``` torch >= 1.10.1 torchaudio >= 0.10.1
+py7zr >= 0.17.2 pyyaml >= 6.0 tqdm >= 4.64.0 ``` ### External requirements
+(AudioCaps only) The external requirements needed to download **AudioCaps** are
+**ffmpeg** and **youtube-dl**. These two programs can be download on Ubuntu
+using `sudo apt install ffmpeg youtube-dl`. You can also override their paths
+for AudioCaps: ```python from aac_datasets import AudioCaps
+AudioCaps.FFMPEG_PATH = "/my/path/to/ffmpeg" AudioCaps.YOUTUBE_DL_PATH = "/my/
+path/to/youtube_dl" dataset = AudioCaps(root=".", download=True) ``` ##
+Download datasets To download a dataset, you can use `download=True` argument
+in dataset construction. However, if you want to download datasets separately,
+you can also use the following command : ```bash aac-datasets-download --root
+"." clotho --subsets "dev" ``` Or use the corresponding function in the code :
+```python from aac_datasets.download import download_clotho download_clotho
+(root=".", subsets=["dev"]) ``` ## References #### AudioCaps [1] C. D. Kim, B.
+Kim, H. Lee, and G. Kim, âAudiocaps: Generating captions for audios in the
+wild,â in NAACL-HLT, 2019. Available: https://aclanthology.org/N19-1011/ ####
+Clotho [2] K. Drossos, S. Lipping, and T. Virtanen, âClotho: An Audio
+Captioning Dataset,â arXiv:1910.09387 [cs, eess], Oct. 2019, Available: http:
+//arxiv.org/abs/1910.09387 #### MACS [3] F. Font, A. Mesaros, D. P. W. Ellis,
+E. Fonseca, M. Fuentes, and B. Elizalde, Proceedings of the 6th Workshop on
+Detection and Classication of Acoustic Scenes and Events (DCASE 2021).
+Barcelona, Spain: Music Technology Group - Universitat Pompeu Fabra, Nov. 2021.
+Available: https://doi.org/10.5281/zenodo.5770113 ## Cite the aac-datasets
+package If you use this software, please consider cite it as below : ```
+@software{ Labbe_aac-datasets_2022, author = {LabbÃ©, Etienne}, license =
+{MIT}, month = {01}, title = {{aac-datasets}}, url = {https://github.com/
+Labbeti/aac-datasets/}, version = {0.3.2}, year = {2023} } ``` ## Contact
+Maintainer: - Etienne LabbÃ© "Labbeti": labbeti.pub@gmail.com
```

### Comparing `aac_datasets-0.3.1/README.md` & `aac_datasets-0.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 <!-- # -*- coding: utf-8 -*- -->
 
 <div align="center">
 
-# Audio Captioning datasets for Pytorch
+# Audio Captioning datasets for PyTorch
 
 <a href="https://www.python.org/"><img alt="Python" src="https://img.shields.io/badge/-Python 3.8+-blue?style=for-the-badge&logo=python&logoColor=white"></a>
-<a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/-PyTorch 1.10.1-ee4c2c?style=for-the-badge&logo=pytorch&logoColor=white"></a>
+<a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/-PyTorch 1.10.1+-ee4c2c?style=for-the-badge&logo=pytorch&logoColor=white"></a>
 <a href="https://black.readthedocs.io/en/stable/"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-black.svg?style=for-the-badge&labelColor=gray"></a>
-<a href="https://github.com/Labbeti/aac-datasets/actions"><img alt="Build" src="https://img.shields.io/github/workflow/status/Labbeti/aac-datasets/Python%20package%20using%20Pip/main?style=for-the-badge&logo=github"></a>
+<a href="https://github.com/Labbeti/aac-datasets/actions"><img alt="Build" src="https://img.shields.io/github/actions/workflow/status/Labbeti/aac-datasets/python-package-pip.yaml?branch=main&style=for-the-badge&logo=github"></a>
 
-Audio Captioning unofficial datasets source code for **AudioCaps** [[1]](#audiocaps), **Clotho** [[2]](#clotho), and **MACS** [[3]](#macs), designed for Pytorch.
+Audio Captioning unofficial datasets source code for **AudioCaps** [[1]](#audiocaps), **Clotho** [[2]](#clotho), and **MACS** [[3]](#macs), designed for PyTorch.
 
 </div>
 
 ## Installation
 ```bash
 pip install aac-datasets
 ```
@@ -21,34 +21,34 @@
 ## Examples
 
 ### Create Clotho dataset
 
 ```python
 from aac_datasets import Clotho
 
-dataset = Clotho(root=".", subset="dev", download=True)
+dataset = Clotho(root=".", download=True)
 item = dataset[0]
 audio, captions = item["audio"], item["captions"]
 # audio: Tensor of shape (n_channels=1, audio_max_size)
-# captions: list of str captions
+# captions: list of str
 ```
 
-### Build Pytorch dataloader with Clotho
+### Build PyTorch dataloader with Clotho
 
 ```python
 from torch.utils.data.dataloader import DataLoader
 from aac_datasets import Clotho
 from aac_datasets.utils import BasicCollate
 
 dataset = Clotho(root=".", download=True)
 dataloader = DataLoader(dataset, batch_size=4, collate_fn=BasicCollate())
 
 for batch in dataloader:
-    # batch["audio"]: list of Tensor of shape (n_channels, audio_size)
-    # batch["captions"]: list of list of str
+    # batch["audio"]: list of 4 tensors of shape (n_channels, audio_size)
+    # batch["captions"]: list of 4 lists of str
     ...
 ```
 
 ## Datasets stats
 Here is the statistics for each dataset :
 
 | | AudioCaps | Clotho | MACS |
@@ -64,15 +64,15 @@
 |:---:|:---:|:---:|:---:|
 | Nb audios | 49838 | 3840 | 3930 |
 | Total audio duration | 136.6h<sup>1</sup> | 24.0h | 10.9h |
 | Audio duration range | 0.5-10s | 15-30s | 10s |
 | Nb captions per audio | 1 | 5 | 2-5 |
 | Nb captions | 49838 | 19195 | 17275 |
 | Total nb words<sup>2</sup> | 402482 | 217362 | 160006 |
-| Nb words range<sup>2</sup> | 2-52 | 8-20 | 5-40 |
+| Sentence size<sup>2</sup> | 2-52 | 8-20 | 5-40 |
 
 <sup>1</sup> This duration is estimated on the total duration of 46230/49838 files of 126.7h.
 
 <sup>2</sup> The sentences are cleaned (lowercase+remove punctuation) and tokenized using the spacy tokenizer to count the words.
 
 ## Requirements
 ### Python packages
@@ -95,19 +95,26 @@
 ```python
 from aac_datasets import AudioCaps
 AudioCaps.FFMPEG_PATH = "/my/path/to/ffmpeg"
 AudioCaps.YOUTUBE_DL_PATH = "/my/path/to/youtube_dl"
 dataset = AudioCaps(root=".", download=True)
 ```
 
-## Command line download
+## Download datasets
 To download a dataset, you can use `download=True` argument in dataset construction.
+
 However, if you want to download datasets separately, you can also use the following command :
 ```bash
-python -m aac_datasets.download --root "./data" clotho --version "v2.1"
+aac-datasets-download --root "." clotho --subsets "dev"
+```
+Or use the corresponding function in the code :
+```python
+from aac_datasets.download import download_clotho
+
+download_clotho(root=".", subsets=["dev"])
 ```
 
 ## References
 #### AudioCaps
 [1] C. D. Kim, B. Kim, H. Lee, and G. Kim, “Audiocaps: Generating captions for audios in the wild,” in NAACL-HLT, 2019. Available: https://aclanthology.org/N19-1011/
 
 #### Clotho
@@ -120,18 +127,18 @@
 If you use this software, please consider cite it as below :
 
 ```
 @software{
     Labbe_aac-datasets_2022,
     author = {Labbé, Etienne},
     license = {MIT},
-    month = {6},
+    month = {01},
     title = {{aac-datasets}},
     url = {https://github.com/Labbeti/aac-datasets/},
-    version = {0.3.1},
-    year = {2022}
+    version = {0.3.2},
+    year = {2023}
 }
 ```
 
 ## Contact
 Maintainer:
 - Etienne Labbé "Labbeti": labbeti.pub@gmail.com
```

#### html2text {}

```diff
@@ -1,55 +1,56 @@
-# Audio Captioning datasets for Pytorch [Python] [PyTorch] [Code_style:_black]
+# Audio Captioning datasets for PyTorch [Python] [PyTorch] [Code_style:_black]
  [Build] Audio Captioning unofficial datasets source code for **AudioCaps** [
     [1]](#audiocaps), **Clotho** [[2]](#clotho), and **MACS** [[3]](#macs),
-                             designed for Pytorch.
+                             designed for PyTorch.
 ## Installation ```bash pip install aac-datasets ``` ## Examples ### Create
 Clotho dataset ```python from aac_datasets import Clotho dataset = Clotho
-(root=".", subset="dev", download=True) item = dataset[0] audio, captions =
-item["audio"], item["captions"] # audio: Tensor of shape (n_channels=1,
-audio_max_size) # captions: list of str captions ``` ### Build Pytorch
-dataloader with Clotho ```python from torch.utils.data.dataloader import
-DataLoader from aac_datasets import Clotho from aac_datasets.utils import
-BasicCollate dataset = Clotho(root=".", download=True) dataloader = DataLoader
-(dataset, batch_size=4, collate_fn=BasicCollate()) for batch in dataloader: #
-batch["audio"]: list of Tensor of shape (n_channels, audio_size) # batch
-["captions"]: list of list of str ... ``` ## Datasets stats Here is the
-statistics for each dataset : | | AudioCaps | Clotho | MACS | |:---:|:---:|:--
--:|:---:| | Subset(s) | train, val, test | dev, val, eval, test, analysis |
-full | | Sample rate | 32000 | 44100 | 48000 | | Estimated size | 43GB | 27GB |
-13GB | | Audio source | AudioSet (youtube) | Freesound | TAU Urban Acoustic
-Scenes 2019 | Here is the **train** subset statistics for each dataset : | |
-AudioCaps/train | Clotho/dev | MACS/full | |:---:|:---:|:---:|:---:| | Nb
-audios | 49838 | 3840 | 3930 | | Total audio duration | 136.6h1 | 24.0h | 10.9h
-| | Audio duration range | 0.5-10s | 15-30s | 10s | | Nb captions per audio | 1
-| 5 | 2-5 | | Nb captions | 49838 | 19195 | 17275 | | Total nb words2 | 402482
-| 217362 | 160006 | | Nb words range2 | 2-52 | 8-20 | 5-40 | 1 This duration is
-estimated on the total duration of 46230/49838 files of 126.7h. 2 The sentences
-are cleaned (lowercase+remove punctuation) and tokenized using the spacy
-tokenizer to count the words. ## Requirements ### Python packages The
-requirements are automatically installed when using pip on this repository. ```
-torch >= 1.10.1 torchaudio >= 0.10.1 py7zr >= 0.17.2 pyyaml >= 6.0 tqdm >=
-4.64.0 ``` ### External requirements (AudioCaps only) The external requirements
-needed to download **AudioCaps** are **ffmpeg** and **youtube-dl**. These two
-programs can be download on Ubuntu using `sudo apt install ffmpeg youtube-dl`.
-You can also override their paths for AudioCaps: ```python from aac_datasets
-import AudioCaps AudioCaps.FFMPEG_PATH = "/my/path/to/ffmpeg"
-AudioCaps.YOUTUBE_DL_PATH = "/my/path/to/youtube_dl" dataset = AudioCaps
-(root=".", download=True) ``` ## Command line download To download a dataset,
-you can use `download=True` argument in dataset construction. However, if you
-want to download datasets separately, you can also use the following command :
-```bash python -m aac_datasets.download --root "./data" clotho --version "v2.1"
-``` ## References #### AudioCaps [1] C. D. Kim, B. Kim, H. Lee, and G. Kim,
-âAudiocaps: Generating captions for audios in the wild,â in NAACL-HLT,
-2019. Available: https://aclanthology.org/N19-1011/ #### Clotho [2] K. Drossos,
-S. Lipping, and T. Virtanen, âClotho: An Audio Captioning Dataset,â arXiv:
-1910.09387 [cs, eess], Oct. 2019, Available: http://arxiv.org/abs/1910.09387
-#### MACS [3] F. Font, A. Mesaros, D. P. W. Ellis, E. Fonseca, M. Fuentes, and
-B. Elizalde, Proceedings of the 6th Workshop on Detection and Classication of
-Acoustic Scenes and Events (DCASE 2021). Barcelona, Spain: Music Technology
-Group - Universitat Pompeu Fabra, Nov. 2021. Available: https://doi.org/
-10.5281/zenodo.5770113 ## Cite the aac-datasets package If you use this
-software, please consider cite it as below : ``` @software{ Labbe_aac-
-datasets_2022, author = {LabbÃ©, Etienne}, license = {MIT}, month = {6}, title
-= {{aac-datasets}}, url = {https://github.com/Labbeti/aac-datasets/}, version =
-{0.3.1}, year = {2022} } ``` ## Contact Maintainer: - Etienne LabbÃ© "Labbeti":
-labbeti.pub@gmail.com
+(root=".", download=True) item = dataset[0] audio, captions = item["audio"],
+item["captions"] # audio: Tensor of shape (n_channels=1, audio_max_size) #
+captions: list of str ``` ### Build PyTorch dataloader with Clotho ```python
+from torch.utils.data.dataloader import DataLoader from aac_datasets import
+Clotho from aac_datasets.utils import BasicCollate dataset = Clotho(root=".",
+download=True) dataloader = DataLoader(dataset, batch_size=4,
+collate_fn=BasicCollate()) for batch in dataloader: # batch["audio"]: list of 4
+tensors of shape (n_channels, audio_size) # batch["captions"]: list of 4 lists
+of str ... ``` ## Datasets stats Here is the statistics for each dataset : | |
+AudioCaps | Clotho | MACS | |:---:|:---:|:---:|:---:| | Subset(s) | train, val,
+test | dev, val, eval, test, analysis | full | | Sample rate | 32000 | 44100 |
+48000 | | Estimated size | 43GB | 27GB | 13GB | | Audio source | AudioSet
+(youtube) | Freesound | TAU Urban Acoustic Scenes 2019 | Here is the **train**
+subset statistics for each dataset : | | AudioCaps/train | Clotho/dev | MACS/
+full | |:---:|:---:|:---:|:---:| | Nb audios | 49838 | 3840 | 3930 | | Total
+audio duration | 136.6h1 | 24.0h | 10.9h | | Audio duration range | 0.5-10s |
+15-30s | 10s | | Nb captions per audio | 1 | 5 | 2-5 | | Nb captions | 49838 |
+19195 | 17275 | | Total nb words2 | 402482 | 217362 | 160006 | | Sentence size2
+| 2-52 | 8-20 | 5-40 | 1 This duration is estimated on the total duration of
+46230/49838 files of 126.7h. 2 The sentences are cleaned (lowercase+remove
+punctuation) and tokenized using the spacy tokenizer to count the words. ##
+Requirements ### Python packages The requirements are automatically installed
+when using pip on this repository. ``` torch >= 1.10.1 torchaudio >= 0.10.1
+py7zr >= 0.17.2 pyyaml >= 6.0 tqdm >= 4.64.0 ``` ### External requirements
+(AudioCaps only) The external requirements needed to download **AudioCaps** are
+**ffmpeg** and **youtube-dl**. These two programs can be download on Ubuntu
+using `sudo apt install ffmpeg youtube-dl`. You can also override their paths
+for AudioCaps: ```python from aac_datasets import AudioCaps
+AudioCaps.FFMPEG_PATH = "/my/path/to/ffmpeg" AudioCaps.YOUTUBE_DL_PATH = "/my/
+path/to/youtube_dl" dataset = AudioCaps(root=".", download=True) ``` ##
+Download datasets To download a dataset, you can use `download=True` argument
+in dataset construction. However, if you want to download datasets separately,
+you can also use the following command : ```bash aac-datasets-download --root
+"." clotho --subsets "dev" ``` Or use the corresponding function in the code :
+```python from aac_datasets.download import download_clotho download_clotho
+(root=".", subsets=["dev"]) ``` ## References #### AudioCaps [1] C. D. Kim, B.
+Kim, H. Lee, and G. Kim, âAudiocaps: Generating captions for audios in the
+wild,â in NAACL-HLT, 2019. Available: https://aclanthology.org/N19-1011/ ####
+Clotho [2] K. Drossos, S. Lipping, and T. Virtanen, âClotho: An Audio
+Captioning Dataset,â arXiv:1910.09387 [cs, eess], Oct. 2019, Available: http:
+//arxiv.org/abs/1910.09387 #### MACS [3] F. Font, A. Mesaros, D. P. W. Ellis,
+E. Fonseca, M. Fuentes, and B. Elizalde, Proceedings of the 6th Workshop on
+Detection and Classication of Acoustic Scenes and Events (DCASE 2021).
+Barcelona, Spain: Music Technology Group - Universitat Pompeu Fabra, Nov. 2021.
+Available: https://doi.org/10.5281/zenodo.5770113 ## Cite the aac-datasets
+package If you use this software, please consider cite it as below : ```
+@software{ Labbe_aac-datasets_2022, author = {LabbÃ©, Etienne}, license =
+{MIT}, month = {01}, title = {{aac-datasets}}, url = {https://github.com/
+Labbeti/aac-datasets/}, version = {0.3.2}, year = {2023} } ``` ## Contact
+Maintainer: - Etienne LabbÃ© "Labbeti": labbeti.pub@gmail.com
```

### Comparing `aac_datasets-0.3.1/docs/conf.py` & `aac_datasets-0.3.2/docs/conf.py`

 * *Files 15% similar despite different names*

```diff
@@ -62,15 +62,22 @@
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = "sphinx_rtd_theme"
+html_theme = "press"
+
+html_theme_options = {
+    "external_links": [
+        ("Github", "https://github.com/Labbeti/aac-datasets"),
+        ("PyPI", "https://pypi.org/project/aac-datasets/"),
+    ],
+}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 
@@ -82,8 +89,9 @@
 todo_include_todos = True
 
 add_module_names = False
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/", None),
     "torch": ("https://pytorch.org/docs/master/", None),
+    "torchaudio": ("https://pytorch.org/audio/stable/", None),
 }
```

### Comparing `aac_datasets-0.3.1/setup.cfg` & `aac_datasets-0.3.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 url = https://pypi.org/project/aac-datasets/
 version = attr: aac_datasets.__version__
 
 [options]
 packages = find:
 package_dir = 
 	=src
-python_requires = >= 3.8
+python_requires = >= 3.7
 install_requires = 
 	torch>=1.10.1
 	torchaudio>=0.10.1
 	py7zr>=0.17.2
 	pyyaml>=6.0
 	tqdm>=4.64.0
```

### Comparing `aac_datasets-0.3.1/src/aac_datasets/__main__.py` & `aac_datasets-0.3.2/src/aac_datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `aac_datasets-0.3.1/src/aac_datasets/check.py` & `aac_datasets-0.3.2/src/aac_datasets/check.py`

 * *Files identical despite different names*

### Comparing `aac_datasets-0.3.1/src/aac_datasets/datasets/audiocaps.py` & `aac_datasets-0.3.2/src/aac_datasets/datasets/audiocaps.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import os.path as osp
 import subprocess
 import sys
 import time
 
 from dataclasses import dataclass, field, fields
-from functools import cached_property
+from functools import lru_cache
 from subprocess import CalledProcessError
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
 
 import torch
 import torchaudio
 import tqdm
 
@@ -42,15 +42,15 @@
     audiocaps_ids: List[int] = field(default_factory=list)
     start_time: int = -1
     tags: List[int] = field(default_factory=list)
     youtube_id: str = "unknown"
 
 
 class AudioCaps(Dataset[Dict[str, Any]]):
-    r"""Unofficial AudioCaps pytorch dataset.
+    r"""Unofficial AudioCaps PyTorch dataset.
 
     Subsets available are 'train', 'val' and 'test'.
 
     Audio is a waveform tensor of shape (1, n_times) of 10 seconds max, sampled at 32KHz.
     Target is a list of strings containing the captions.
     The 'train' subset has only 1 caption per sample and 'val' and 'test' have 5 captions.
 
@@ -84,14 +84,15 @@
     AUDIO_N_CHANNELS = 1
     CAPTION_MAX_LENGTH = 52
     CAPTION_MIN_LENGTH = 2
     CAPTIONS_PER_AUDIO = {"train": 1, "val": 5, "test": 5}
     DNAME_LOG = "logs"
     FFMPEG_PATH: str = "ffmpeg"
     FORCE_PREPARE_DATA: bool = False
+    N_AUDIOSET_CLASSES: int = 527
     REDIRECT_LOG = False
     SAMPLE_RATE = 32000
     SUBSETS = ("train", "val", "test")
     VERIFY_FILES = False
     YOUTUBE_DL_PATH: str = "youtube-dl"
 
     # Initialization
@@ -125,55 +126,55 @@
             defaults to True.
         :param with_tags: If True, load the tags from AudioSet dataset.
             Note: tags needs to be downloaded with download=True & with_tags=True before being used.
             defaults to False.
         """
         if subset not in AudioCaps.SUBSETS:
             raise ValueError(
-                f"Invalid argument {subset=} for AudioCaps. (expected one of {AudioCaps.SUBSETS})"
+                f"Invalid argument subset={subset} for AudioCaps. (expected one of {AudioCaps.SUBSETS})"
             )
 
         super().__init__()
         # Attributes
-        self.__root = root
-        self.__subset = subset
-        self.__download = download
-        self.__transform = transform
-        self.__flat_captions = flat_captions
-        self.__verbose = verbose
-        self.__exclude_removed_audio = exclude_removed_audio
-        self.__with_tags = with_tags
+        self._root = root
+        self._subset = subset
+        self._download = download
+        self._transform = transform
+        self._flat_captions = flat_captions
+        self._verbose = verbose
+        self._exclude_removed_audio = exclude_removed_audio
+        self._with_tags = with_tags
 
         # Data to load
-        self.__all_items: Dict[str, List[Any]] = {}
-        self.__loaded = False
-        self.__index_to_tagname: List[str] = []
+        self._all_items: Dict[str, List[Any]] = {}
+        self._loaded = False
+        self._index_to_tagname: List[str] = []
 
-        if self.__download:
+        if self._download:
             self.__prepare_data()
         self.__load_data()
 
     # Properties
     @property
     def column_names(self) -> List[str]:
         """The name of each column of the dataset."""
         return [field.name for field in fields(AudioCapsItem)]
 
     @property
     def index_to_tagname(self) -> List[str]:
         """AudioSet ordered list of tag names. Returns an empty list if `with_tags` is False."""
-        return self.__index_to_tagname
+        return self._index_to_tagname
 
     @property
     def info(self) -> Dict[str, Any]:
         """Return the global dataset info."""
         return {
             "dataset": "audiocaps",
-            "subset": self.__subset,
-            "with_tags": self.__with_tags,
+            "subset": self._subset,
+            "with_tags": self._with_tags,
         }
 
     @property
     def shape(self) -> Tuple[int, ...]:
         """The shape of the AudioCaps dataset."""
         return len(self), len(self.column_names)
 
@@ -193,43 +194,48 @@
             idx = slice(None)
         if column is None:
             column = self.column_names
 
         if not isinstance(column, str) and isinstance(column, Iterable):
             return {column_i: self.at(idx, column_i) for column_i in column}
 
-        if isinstance(idx, (int, slice)) and column in self.__all_items.keys():
-            return self.__all_items[column][idx]
+        if isinstance(idx, (int, slice)) and column in self._all_items.keys():
+            return self._all_items[column][idx]
 
         if isinstance(idx, slice):
             idx = range(len(self))[idx]
 
         if isinstance(idx, Iterable):
+            idx = list(idx)
+            if not all(isinstance(idx_i, int) for idx_i in idx):
+                raise TypeError(
+                    f"Invalid input type for idx={idx}. (expected Iterable[int], not Iterable[{idx.__class__.__name__}])"
+                )
             return [self.at(idx_i, column) for idx_i in idx]
 
         if column == "audio":
             fpath = self.at(idx, "fpath")
-            if not self.__all_items["is_on_disk"][idx]:
+            if not self._all_items["is_on_disk"][idx]:
                 return torch.empty((0,))
             audio, sr = torchaudio.load(fpath)  # type: ignore
 
             # Sanity check
             if audio.nelement() == 0:
                 raise RuntimeError(
-                    f"Invalid audio number of elements in {fpath}. (expected {audio.nelement()=} > 0)"
+                    f"Invalid audio number of elements in '{fpath}'. (expected audio.nelements()={audio.nelement()} > 0)"
                 )
             if sr != self.SAMPLE_RATE:
                 raise RuntimeError(
-                    f"Invalid sample rate in {fpath}. (expected {self.SAMPLE_RATE} but found {sr=})"
+                    f"Invalid sample rate in '{fpath}'. (expected {self.SAMPLE_RATE} but found sr={sr})"
                 )
             return audio
 
         elif column == "audio_metadata":
             fpath = self.at(idx, "fpath")
-            if not self.__all_items["is_on_disk"][idx]:
+            if not self._all_items["is_on_disk"][idx]:
                 return None
             audio_metadata = torchaudio.info(fpath)  # type: ignore
             return audio_metadata
 
         elif column == "dataset":
             return "audiocaps"
 
@@ -256,31 +262,31 @@
         elif column == "sr":
             audio_metadata = self.at(idx, "audio_metadata")
             if audio_metadata is None:
                 return -1
             return audio_metadata.sample_rate
 
         elif column == "subset":
-            return self.__subset
+            return self._subset
 
         else:
             raise ValueError(
-                f"Invalid argument {column=} at {idx=}. (expected one of {tuple(self.column_names)})"
+                f"Invalid argument column={column} at idx={idx}. (expected one of {tuple(self.column_names)})"
             )
 
     def is_loaded(self) -> bool:
         """Returns True if the dataset is loaded."""
-        return self.__loaded
+        return self._loaded
 
     def set_transform(
         self,
         transform: Optional[Callable[[Dict[str, Any]], Any]],
     ) -> None:
         """Set the transform applied to each row."""
-        self.__transform = transform
+        self._transform = transform
 
     # Magic methods
     def __getitem__(
         self,
         idx: Any,
     ) -> Dict[str, Any]:
         if (
@@ -289,26 +295,39 @@
             and (isinstance(idx[1], (str, Iterable)) or idx[1] is None)
         ):
             idx, column = idx
         else:
             column = None
 
         item = self.at(idx, column)
-        if self.__transform is not None:
-            item = self.__transform(item)
+        if self._transform is not None:
+            item = self._transform(item)
         return item
 
     def __len__(self) -> int:
         """
         :return: The number of items in the dataset.
         """
-        return len(self.__all_items["captions"])
+        return len(self._all_items["captions"])
 
     def __repr__(self) -> str:
-        return f"AudioCaps(size={len(self)}, subset={self.__subset}, num_columns={len(self.column_names)}, with_tags={self.__with_tags})"
+        return f"AudioCaps(size={len(self)}, subset={self._subset}, num_columns={len(self.column_names)}, with_tags={self._with_tags})"
+
+    # Public class methods
+    @classmethod
+    def load_class_labels_indices(cls, root: str) -> List[Dict[str, str]]:
+        class_labels_indices_fpath = osp.join(
+            root,
+            f"AUDIOCAPS_{AudioCaps.SAMPLE_RATE}Hz",
+            AUDIOSET_LINKS["class_labels_indices"]["fname"],
+        )
+        with open(class_labels_indices_fpath, "r") as file:
+            reader = csv.DictReader(file)
+            audioset_classes_data = list(reader)
+        return audioset_classes_data
 
     # Private methods
     def __check_file(self, fpath: str) -> bool:
         try:
             audio, sr = torchaudio.load(fpath)  # type: ignore
         except RuntimeError:
             message = f'Found file "{fpath}" already downloaded but it is invalid (cannot load). It will be removed.'
@@ -323,63 +342,63 @@
         if sr != self.SAMPLE_RATE:
             message = f'Found file "{fpath}" already downloaded but it is invalid (invalid sr={sr} != {self.SAMPLE_RATE}). It will be removed.'
             logger.error(message)
             return False
 
         return True
 
-    @cached_property
+    @property
+    @lru_cache()
     def __dpath_audio_subset(self) -> str:
         return osp.join(
             self.__dpath_data,
             "audio",
-            self.__subset,
+            self._subset,
         )
 
-    @cached_property
+    @property
+    @lru_cache()
     def __dpath_data(self) -> str:
-        return osp.join(self.__root, f"AUDIOCAPS_{AudioCaps.SAMPLE_RATE}Hz")
+        return osp.join(self._root, f"AUDIOCAPS_{AudioCaps.SAMPLE_RATE}Hz")
 
     def __is_prepared(self) -> bool:
-        links = AUDIOCAPS_LINKS[self.__subset]
+        links = AUDIOCAPS_LINKS[self._subset]
         captions_fname = links["captions"]["fname"]
         captions_fpath = osp.join(self.__dpath_data, captions_fname)
         return osp.isdir(self.__dpath_audio_subset) and osp.isfile(captions_fpath)
 
     def __load_data(self) -> None:
         if not self.__is_prepared():
             raise RuntimeError(
-                f"Cannot load data: audiocaps_{self.__subset} is not prepared in data root={self.__root}. Please use download=True in dataset constructor."
+                f"Cannot load data: audiocaps_{self._subset} is not prepared in data root={self._root}. Please use download=True in dataset constructor."
             )
 
-        links = AUDIOCAPS_LINKS[self.__subset]
+        links = AUDIOCAPS_LINKS[self._subset]
 
         captions_fname = links["captions"]["fname"]
         captions_fpath = osp.join(self.__dpath_data, captions_fname)
         with open(captions_fpath, "r") as file:
             reader = csv.DictReader(file)
             captions_data = list(reader)
 
-        if self.__with_tags:
+        if self._with_tags:
             class_labels_indices_fpath = osp.join(
                 self.__dpath_data, AUDIOSET_LINKS["class_labels_indices"]["fname"]
             )
             unbal_tags_fpath = osp.join(
                 self.__dpath_data, AUDIOSET_LINKS["unbalanced"]["fname"]
             )
 
             if not all(map(osp.isfile, (class_labels_indices_fpath, unbal_tags_fpath))):
                 raise FileNotFoundError(
                     f"Cannot load tags without tags files '{osp.basename(class_labels_indices_fpath)}' and '{osp.basename(unbal_tags_fpath)}'."
                     f"Please use download=True and with_tags=True in dataset constructor."
                 )
 
-            with open(class_labels_indices_fpath, "r") as file:
-                reader = csv.DictReader(file)
-                audioset_classes_data = list(reader)
+            audioset_classes_data = AudioCaps.load_class_labels_indices(self._root)
 
             with open(unbal_tags_fpath, "r") as file:
                 fieldnames = ("YTID", "start_seconds", "end_seconds", "positive_labels")
                 reader = csv.DictReader(
                     file, fieldnames, skipinitialspace=True, strict=True
                 )
                 # Skip the comments
@@ -392,15 +411,15 @@
 
         # Build global mappings
         fnames_dic = dict.fromkeys(
             f"{line['youtube_id']}_{line['start_time']}.{self.AUDIO_FILE_EXTENSION}"
             for line in captions_data
         )
         audio_fnames_on_disk = dict.fromkeys(os.listdir(self.__dpath_audio_subset))
-        if self.__exclude_removed_audio:
+        if self._exclude_removed_audio:
             fnames_lst = [
                 fname for fname in fnames_dic if fname in audio_fnames_on_disk
             ]
             is_on_disk_lst = [True for _ in range(len(fnames_lst))]
         else:
             fnames_lst = list(fnames_dic)
             is_on_disk_lst = [fname in audio_fnames_on_disk for fname in fnames_lst]
@@ -416,25 +435,25 @@
             mid_to_tag_name[line["mid"]] = line["display_name"]
             tag_name_to_index[line["display_name"]] = int(line["index"])
 
         classes_indexes = list(tag_name_to_index.values())
         assert len(classes_indexes) == 0 or classes_indexes == list(
             range(classes_indexes[-1] + 1)
         )
-        self.__index_to_tagname = list(tag_name_to_index.keys())
+        self._index_to_tagname = list(tag_name_to_index.keys())
 
         # Process each field into a single structure
         all_caps_dic: Dict[str, List[Any]] = {
             key: [None for _ in range(dataset_size)]
             for key in ("audiocaps_ids", "youtube_id", "start_time", "captions")
         }
         for line in tqdm.tqdm(
             captions_data,
-            disable=self.__verbose <= 0,
-            desc=f"Loading AudioCaps ({self.__subset}) captions...",
+            disable=self._verbose <= 0,
+            desc=f"Loading AudioCaps ({self._subset}) captions...",
         ):
             # audiocap_id, youtube_id, start_time, caption
             audiocap_id = line["audiocap_id"]
             youtube_id = line["youtube_id"]
             start_time = line["start_time"]
             caption = line["caption"]
 
@@ -455,15 +474,15 @@
                     all_caps_dic["captions"][idx].append(caption)
 
         # Load tags from audioset data
         all_tags_lst = [[] for _ in range(dataset_size)]
 
         for line in tqdm.tqdm(
             unbal_tags_data,
-            disable=self.__verbose <= 0,
+            disable=self._verbose <= 0,
             desc="Loading AudioSet tags...",
         ):
             # keys: YTID, start_seconds, end_seconds, positive_labels
             youtube_id = line["YTID"]
             # Note : In audioset, start_time is a string repr of a float value, audiocaps it is a string repr of an integer
             start_time = int(float(line["start_seconds"]))
             fname = f"{youtube_id}_{start_time}.{self.AUDIO_FILE_EXTENSION}"
@@ -476,42 +495,43 @@
                 idx = fname_to_idx[fname]
                 all_tags_lst[idx] = tags_indexes
 
         all_items = {
             "fname": fnames_lst,
             "tags": all_tags_lst,
             "is_on_disk": is_on_disk_lst,
-        } | all_caps_dic
+        }
+        all_items.update(all_caps_dic)
 
         # Convert audiocaps_ids and start_time to ints
         all_items["audiocaps_ids"] = [
             list(map(int, item)) for item in all_items["audiocaps_ids"]
         ]
         all_items["start_time"] = list(map(int, all_items["start_time"]))
 
-        if self.__flat_captions and self.CAPTIONS_PER_AUDIO[self.__subset] > 1:
+        if self._flat_captions and self.CAPTIONS_PER_AUDIO[self._subset] > 1:
             all_infos_unfolded = {key: [] for key in all_items.keys()}
 
             for i, captions in enumerate(all_items["captions"]):
                 for caption in captions:
                     for key in all_items.keys():
                         all_infos_unfolded[key].append(all_items[key][i])
                     all_infos_unfolded["captions"] = [caption]
 
             all_items = all_infos_unfolded
 
-        self.__all_items = all_items
-        self.__loaded = True
+        self._all_items = all_items
+        self._loaded = True
 
-        if self.__verbose >= 1:
+        if self._verbose >= 1:
             logger.info(f"{repr(self)} has been loaded. (len={len(self)})")
 
     def __prepare_data(self) -> None:
-        if not osp.isdir(self.__root):
-            raise RuntimeError(f"Cannot find root directory '{self.__root}'.")
+        if not osp.isdir(self._root):
+            raise RuntimeError(f"Cannot find root directory '{self._root}'.")
 
         try:
             subprocess.check_call(
                 [self.YOUTUBE_DL_PATH, "--help"],
                 stdout=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL,
             )
@@ -530,46 +550,46 @@
         except (CalledProcessError, PermissionError, FileNotFoundError) as err:
             logger.error(f"Cannot use ffmpeg path '{self.FFMPEG_PATH}'. ({err})")
             raise err
 
         if self.__is_prepared() and not self.FORCE_PREPARE_DATA:
             return None
 
-        links = AUDIOCAPS_LINKS[self.__subset]
+        links = AUDIOCAPS_LINKS[self._subset]
         captions_fname = links["captions"]["fname"]
         captions_fpath = osp.join(self.__dpath_data, captions_fname)
 
         os.makedirs(self.__dpath_audio_subset, exist_ok=True)
 
         if not osp.isfile(captions_fpath):
             url = links["captions"]["url"]
-            download_url_to_file(url, captions_fpath, progress=self.__verbose >= 1)
+            download_url_to_file(url, captions_fpath, progress=self._verbose >= 1)
 
         start = time.perf_counter()
         with open(captions_fpath, "r") as file:
             n_samples = len(file.readlines())
 
-        if self.__verbose >= 1:
+        if self._verbose >= 1:
             log_dpath = osp.join(self.__dpath_data, self.DNAME_LOG)
             if not osp.isdir(log_dpath):
                 os.makedirs(log_dpath)
 
             if self.REDIRECT_LOG:
                 logging.basicConfig(
-                    filename=osp.join(log_dpath, f"preparation_{self.__subset}.txt"),
+                    filename=osp.join(log_dpath, f"preparation_{self._subset}.txt"),
                     filemode="w",
                     level=logging.INFO,
                     force=True,
                 )
-            logger.info(f"Start downloading files for {self.__subset} AudioCaps split.")
+            logger.info(f"Start downloading files for {self._subset} AudioCaps split.")
 
         with open(captions_fpath, "r") as file:
             # Download audio files
             reader = csv.DictReader(file)
-            if self.__verbose >= 1:
+            if self._verbose >= 1:
                 reader = tqdm.tqdm(reader, total=n_samples)
 
             n_download_ok, n_download_err, n_already_ok, n_already_err = 0, 0, 0, 0
             for line in reader:
                 # Keys: audiocap_id, youtube_id, start_time, caption
                 audiocap_id, youtube_id, start_time = [
                     line[key] for key in ("audiocap_id", "youtube_id", "start_time")
@@ -594,69 +614,69 @@
                         youtube_dl_path=self.YOUTUBE_DL_PATH,
                         ffmpeg_path=self.FFMPEG_PATH,
                         n_channels=self.AUDIO_N_CHANNELS,
                     )
                     if success:
                         valid_file = self.__check_file(fpath)
                         if valid_file:
-                            if self.__verbose >= 2:
+                            if self._verbose >= 2:
                                 logger.debug(
                                     f'[{audiocap_id:6s}] File "{youtube_id}" has been downloaded and verified.'
                                 )
                             n_download_ok += 1
                         else:
-                            if self.__verbose >= 1:
+                            if self._verbose >= 1:
                                 logger.warning(
                                     f'[{audiocap_id:6s}] File "{youtube_id}" has been downloaded but it is not valid and it will be removed.'
                                 )
                             os.remove(fpath)
                             n_download_err += 1
                     else:
                         logger.error(
                             f'[{audiocap_id:6s}] Cannot extract audio from "{youtube_id}".'
                         )
                         n_download_err += 1
 
                 elif self.VERIFY_FILES:
                     valid_file = self.__check_file(fpath)
                     if valid_file:
-                        if self.__verbose >= 2:
+                        if self._verbose >= 2:
                             logger.debug(
                                 f'[{audiocap_id:6s}] File "{youtube_id}" is already downloaded and has been verified.'
                             )
                         n_already_ok += 1
                     else:
-                        if self.__verbose >= 1:
+                        if self._verbose >= 1:
                             logger.warning(
                                 f'[{audiocap_id:6s}] File "{youtube_id}" is already downloaded but it is not valid and will be removed.'
                             )
                         os.remove(fpath)
                         n_already_err += 1
                 else:
-                    if self.__verbose >= 2:
+                    if self._verbose >= 2:
                         logger.debug(
-                            f'[{audiocap_id:6s}] File "{youtube_id}" is already downloaded but it is not verified due to {self.VERIFY_FILES=}.'
+                            f'[{audiocap_id:6s}] File "{youtube_id}" is already downloaded but it is not verified due to self.VERIFY_FILES={self.VERIFY_FILES}.'
                         )
                     n_already_ok += 1
 
-        if self.__with_tags:
+        if self._with_tags:
             for key in ("class_labels_indices", "unbalanced"):
                 infos = AUDIOSET_LINKS[key]
                 url = infos["url"]
                 fname = infos["fname"]
                 fpath = osp.join(self.__dpath_data, fname)
                 if not osp.isfile(fpath):
-                    if self.__verbose >= 1:
+                    if self._verbose >= 1:
                         logger.info(f"Downloading file '{fname}'...")
-                    download_url_to_file(url, fpath, progress=self.__verbose >= 1)
+                    download_url_to_file(url, fpath, progress=self._verbose >= 1)
 
-        if self.__verbose >= 1:
+        if self._verbose >= 1:
             duration = int(time.perf_counter() - start)
             logger.info(
-                f'Download and preparation of AudioCaps for subset "{self.__subset}" done in {duration}s. '
+                f'Download and preparation of AudioCaps for subset "{self._subset}" done in {duration}s. '
             )
             logger.info(f"- {n_download_ok} downloads success,")
             logger.info(f"- {n_download_err} downloads failed,")
             logger.info(f"- {n_already_ok} already downloaded,")
             logger.info(f"- {n_already_err} already downloaded errors,")
             logger.info(f"- {n_samples} total samples.")
```

### Comparing `aac_datasets-0.3.1/src/aac_datasets/datasets/clotho.py` & `aac_datasets-0.3.2/src/aac_datasets/datasets/clotho.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import copy
 import csv
 import logging
 import os
 import os.path as osp
 
 from dataclasses import dataclass, field, fields
-from functools import cached_property
+from functools import lru_cache
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
 from zipfile import ZipFile
 
 import torch
 import torchaudio
 
 from py7zr import SevenZipFile
@@ -250,15 +250,15 @@
     "manufacturer",
     "license",
 )
 
 
 class Clotho(Dataset[Dict[str, Any]]):
     r"""
-    Unofficial Clotho pytorch dataset.
+    Unofficial Clotho PyTorch dataset.
     Subsets available are 'train', 'val', 'eval', 'test' and 'analysis'.
 
     Audio are waveform sounds of 15 to 30 seconds, sampled at 44100 Hz.
     Target is a list of 5 different sentences strings describing an audio sample.
     The maximal number of words in captions is 20.
 
     Clotho V1 Paper : https://arxiv.org/pdf/1910.09387.pdf
@@ -332,55 +332,56 @@
         :param verbose: Verbose level to use. Can be 0 or 1.
             defaults to 0.
         :param version: The version of the dataset. Can be one of :attr:`~Clotho.VERSIONS`.
             defaults to 'v2.1'.
         """
         if version not in Clotho.VERSIONS:
             raise ValueError(
-                f"Invalid Clotho argument {version=}. Must be one of {Clotho.VERSIONS}."
+                f"Invalid Clotho argument version={version}. Must be one of {Clotho.VERSIONS}."
             )
 
-        if subset not in CLOTHO_LINKS[version].keys():
+        subsets = tuple(CLOTHO_LINKS[version].keys())
+        if subset not in subsets:
             raise ValueError(
-                f"Invalid Clotho argument {subset=} for {version=}. Must be one of {tuple(CLOTHO_LINKS[version].keys())}."
+                f"Invalid Clotho argument subset={subset} for version={version}. Must be one of {subsets}."
             )
 
         super().__init__()
-        self.__root = root
-        self.__subset = subset
-        self.__download = download
-        self.__transform = transform
-        self.__flat_captions = flat_captions
-        self.__version = version
-        self.__verbose = verbose
+        self._root = root
+        self._subset = subset
+        self._download = download
+        self._transform = transform
+        self._flat_captions = flat_captions
+        self._version = version
+        self._verbose = verbose
 
-        self.__all_items = {}
-        self.__loaded = False
+        self._all_items = {}
+        self._loaded = False
 
-        if self.__download:
+        if self._download:
             self.__prepare_data()
         self.__load_data()
 
     # Properties
     @property
     def column_names(self) -> List[str]:
         """The name of each column of the dataset."""
         return [
             field_.name
             for field_ in fields(ClothoItem)
-            if field_.name in self.__all_items or field_.name not in METADATA_KEYS
+            if field_.name in self._all_items or field_.name not in METADATA_KEYS
         ]
 
     @property
     def info(self) -> Dict[str, Any]:
         """Return the global dataset info."""
         return {
             "dataset": "clotho",
-            "subset": self.__subset,
-            "version": self.__version,
+            "subset": self._subset,
+            "version": self._version,
         }
 
     @property
     def shape(self) -> Tuple[int, ...]:
         """The shape of the Clotho dataset."""
         return len(self), len(self.column_names)
 
@@ -400,35 +401,40 @@
             idx = slice(None)
         if column is None:
             column = self.column_names
 
         if not isinstance(column, str) and isinstance(column, Iterable):
             return {column_i: self.at(idx, column_i) for column_i in column}
 
-        if isinstance(idx, (int, slice)) and column in self.__all_items.keys():
-            return self.__all_items[column][idx]
+        if isinstance(idx, (int, slice)) and column in self._all_items.keys():
+            return self._all_items[column][idx]
 
         if isinstance(idx, slice):
             idx = range(len(self))[idx]
 
         if isinstance(idx, Iterable):
+            idx = list(idx)
+            if not all(isinstance(idx_i, int) for idx_i in idx):
+                raise TypeError(
+                    f"Invalid input type for idx={idx}. (expected Iterable[int], not Iterable[{idx.__class__.__name__}])"
+                )
             return [self.at(idx_i, column) for idx_i in idx]
 
         if column == "audio":
             fpath = self.at(idx, "fpath")
             audio, sr = torchaudio.load(fpath)  # type: ignore
 
             # Sanity check
             if audio.nelement() == 0:
                 raise RuntimeError(
-                    f"Invalid audio number of elements in {fpath}. (expected {audio.nelement()=} > 0)"
+                    f"Invalid audio number of elements in {fpath}. (expected audio.nelement()={audio.nelement()} > 0)"
                 )
             if sr != self.SAMPLE_RATE:
                 raise RuntimeError(
-                    f"Invalid sample rate in {fpath}. (expected {self.SAMPLE_RATE} but found {sr=})"
+                    f"Invalid sample rate in {fpath}. (expected {self.SAMPLE_RATE} but found sr={sr})"
                 )
             return audio
 
         elif column == "audio_metadata":
             fpath = self.at(idx, "fpath")
             audio_metadata = torchaudio.info(fpath)  # type: ignore
             return audio_metadata
@@ -453,31 +459,31 @@
             return audio_metadata.num_frames
 
         elif column == "sr":
             audio_metadata = self.at(idx, "audio_metadata")
             return audio_metadata.sample_rate
 
         elif column == "subset":
-            return self.__subset
+            return self._subset
 
         else:
             raise ValueError(
-                f"Invalid argument {column=} at {idx=}. (expected one of {tuple(self.column_names)})"
+                f"Invalid argument column={column} at idx={idx}. (expected one of {tuple(self.column_names)})"
             )
 
     def is_loaded(self) -> bool:
         """Returns True if the dataset is loaded."""
-        return self.__loaded
+        return self._loaded
 
     def set_transform(
         self,
         transform: Optional[Callable[[Dict[str, Any]], Any]],
     ) -> None:
         """Set the transform applied to each row."""
-        self.__transform = transform
+        self._transform = transform
 
     # Magic methods
     def __getitem__(
         self,
         idx: Any,
     ) -> Dict[str, Any]:
         if (
@@ -486,75 +492,80 @@
             and (isinstance(idx[1], (str, Iterable)) or idx[1] is None)
         ):
             idx, column = idx
         else:
             column = None
 
         item = self.at(idx, column)
-        if self.__transform is not None:
-            item = self.__transform(item)
+        if self._transform is not None:
+            item = self._transform(item)
         return item
 
     def __len__(self) -> int:
         """
         :return: The number of items in the dataset.
         """
-        return len(self.__all_items["captions"])
+        return len(self._all_items["captions"])
 
     def __repr__(self) -> str:
-        return f"Clotho(size={len(self)}, subset={self.__subset}, num_columns={len(self.column_names)}, version={self.__version})"
+        return f"Clotho(size={len(self)}, subset={self._subset}, num_columns={len(self.column_names)}, version={self._version})"
 
     # Private methods
-    @cached_property
+    @property
+    @lru_cache()
     def __dpath_archives(self) -> str:
         return osp.join(self.__dpath_data, "archives")
 
-    @cached_property
+    @property
+    @lru_cache()
     def __dpath_audio(self) -> str:
         return osp.join(self.__dpath_data, "clotho_audio_files")
 
-    @cached_property
+    @property
+    @lru_cache()
     def __dpath_audio_subset(self) -> str:
         return osp.join(
             self.__dpath_data,
             "clotho_audio_files",
-            CLOTHO_AUDIO_DNAMES[self.__subset],
+            CLOTHO_AUDIO_DNAMES[self._subset],
         )
 
-    @cached_property
+    @property
+    @lru_cache()
     def __dpath_csv(self) -> str:
         return osp.join(self.__dpath_data, "clotho_csv_files")
 
-    @cached_property
+    @property
+    @lru_cache()
     def __dpath_data(self) -> str:
-        return osp.join(self.__root, f"CLOTHO_{self.__version}")
+        return osp.join(self._root, f"CLOTHO_{self._version}")
 
     def __is_prepared(self) -> bool:
         if not all(map(osp.isdir, (self.__dpath_audio_subset, self.__dpath_csv))):
             return False
 
-        if Clotho.CAPTIONS_PER_AUDIO[self.__subset] == 0:
+        if Clotho.CAPTIONS_PER_AUDIO[self._subset] == 0:
             return True
 
-        links = CLOTHO_LINKS[self.__version][self.__subset]
+        links = CLOTHO_LINKS[self._version][self._subset]
         captions_fname = links["captions"]["fname"]
         captions_fpath = osp.join(self.__dpath_csv, captions_fname)
         with open(captions_fpath, "r") as file:
             reader = csv.DictReader(file)
             lines = list(reader)
         return len(lines) == len(os.listdir(self.__dpath_audio_subset))
 
     def __load_data(self) -> None:
         if not self.__is_prepared():
             raise RuntimeError(
-                f"Cannot load data: clotho_{self.__subset} is not prepared in data root={self.__root}. Please use download=True in dataset constructor."
+                f"Cannot load data: clotho_{self._subset} is not prepared in data root={self._root}. Please use download=True in dataset constructor."
             )
 
         # Read fpath of .wav audio files
-        links = CLOTHO_LINKS[self.__version][self.__subset]
+        links = CLOTHO_LINKS[self._version][self._subset]
         dpath_audio_subset = self.__dpath_audio_subset
 
         if not osp.isdir(dpath_audio_subset):
             raise RuntimeError(f'Cannot find directory "{dpath_audio_subset}".')
 
         # Read Clotho files
         if "captions" in links.keys():
@@ -569,21 +580,21 @@
             captions_data = []
 
         if "metadata" in links.keys():
             metadata_fname = links["metadata"]["fname"]
             metadata_fpath = osp.join(self.__dpath_csv, metadata_fname)
 
             # Keys: file_name, keywords, sound_id, sound_link, start_end_samples, manufacturer, license
-            if self.__version in ("v2", "v2.1"):
+            if self._version in ("v2", "v2.1"):
                 encoding = "ISO-8859-1"
             else:
                 encoding = None
 
             with open(metadata_fpath, "r", encoding=encoding) as file:
-                delimiter = ";" if self.__subset == "test" else ","
+                delimiter = ";" if self._subset == "test" else ","
                 reader = csv.DictReader(file, delimiter=delimiter)
                 metadata = list(reader)
         else:
             metadata = []
 
         if "captions" in links.keys():
             # note: "dev", "val", "eval"
@@ -615,63 +626,64 @@
         all_metadata_dic: Dict[str, List[Any]] = {
             key: [None for _ in range(dataset_size)] for key in subset_metadata_keys
         }
         for line in metadata:
             fname = line["file_name"]
             if fname not in fname_to_idx:
                 raise KeyError(
-                    f"Cannot find metadata {fname=} in captions file. (subset={self.__subset})"
+                    f"Cannot find metadata fname={fname} in captions file. (subset={self._subset})"
                 )
             idx = fname_to_idx[fname]
             for key in subset_metadata_keys:
                 # The test subset does not have keywords in metadata, but has sound_id, sound_link, etc.
                 if key in line:
                     all_metadata_dic[key][idx] = line[key]
 
         all_items = {
             "fname": fnames_lst,
             "captions": all_captions_lst,
-        } | all_metadata_dic
+        }
+        all_items.update(all_metadata_dic)
 
         if "keywords" in all_items:
             # Split keywords into list[str]
             all_items["keywords"] = [
                 keywords.split(";") if keywords is not None else []
                 for keywords in all_items["keywords"]
             ]
 
-        if self.__flat_captions and self.CAPTIONS_PER_AUDIO[self.__subset] > 1:
+        if self._flat_captions and self.CAPTIONS_PER_AUDIO[self._subset] > 1:
             all_infos_unfolded = {key: [] for key in all_items.keys()}
 
             for i, captions in enumerate(all_items["captions"]):
                 for caption in captions:
                     for key in all_items.keys():
                         all_infos_unfolded[key].append(all_items[key][i])
                     all_infos_unfolded["captions"] = [caption]
 
             all_items = all_infos_unfolded
 
-        self.__all_items = all_items
-        self.__loaded = True
+        self._all_items = all_items
+        self._loaded = True
 
-        if self.__verbose >= 1:
+        if self._verbose >= 1:
             logger.info(f"{repr(self)} has been loaded. (len={len(self)})")
 
     def __prepare_data(self) -> None:
-        if not osp.isdir(self.__root):
-            raise RuntimeError(f"Cannot find root directory '{self.__root}'.")
+        if not osp.isdir(self._root):
+            raise RuntimeError(f"Cannot find root directory '{self._root}'.")
 
         os.makedirs(self.__dpath_archives, exist_ok=True)
         os.makedirs(self.__dpath_audio, exist_ok=True)
         os.makedirs(self.__dpath_csv, exist_ok=True)
 
-        if self.__verbose >= 1:
-            logger.info(f"Start to download files for clotho_{self.__subset}...")
+        if self._verbose >= 1:
+            logger.info(f"Start to download files for clotho_{self._subset}...")
 
-        links = copy.deepcopy(CLOTHO_LINKS[self.__version][self.__subset])
+        links = copy.deepcopy(CLOTHO_LINKS[self._version][self._subset])
         extensions = ("7z", "csv", "zip")
 
         # Download csv and 7z files
         for file_info in links.values():
             fname, url, hash_value = (
                 file_info["fname"],
                 file_info["url"],
@@ -681,46 +693,46 @@
 
             if extension in ("7z", "zip"):
                 dpath = self.__dpath_archives
             elif extension == "csv":
                 dpath = self.__dpath_csv
             else:
                 raise RuntimeError(
-                    f"Found invalid {extension=}. Must be one of {extensions}."
+                    f"Found invalid extension={extension}. Must be one of {extensions}."
                 )
 
             fpath = osp.join(dpath, fname)
             if not osp.isfile(fpath) or self.FORCE_PREPARE_DATA:
-                if self.__verbose >= 1:
-                    logger.info(f"Download and check file '{fname}' from {url=}...")
+                if self._verbose >= 1:
+                    logger.info(f"Download and check file '{fname}' from url={url}...")
 
                 download_url_to_file(
                     url,
                     fpath,
-                    progress=self.__verbose >= 1,
+                    progress=self._verbose >= 1,
                 )
 
-            elif self.__verbose >= 1:
-                logger.info(f"File {fname=} is already extracted.")
+            elif self._verbose >= 1:
+                logger.info(f"File fname={fname} is already extracted.")
 
             with open(fpath, "rb") as file:
                 valid = validate_file(file, hash_value, hash_type="md5")
             if not valid:
                 raise RuntimeError(f"Invalid checksum for file {fname}.")
 
         # Extract audio files from archives
         for file_info in links.values():
             fname = file_info["fname"]
             extension = fname.split(".")[-1]
 
             if extension in ("7z", "zip"):
                 fpath = osp.join(self.__dpath_archives, fname)
 
-                if self.__verbose >= 1:
-                    logger.info(f"Extract archive file {fname=}...")
+                if self._verbose >= 1:
+                    logger.info(f"Extract archive file fname={fname}...")
 
                 if extension == "7z":
                     archive_file = SevenZipFile(fpath)
                     compressed_fnames = [
                         osp.basename(fname) for fname in archive_file.getnames()
                     ]
                 elif extension == "zip":
@@ -731,15 +743,15 @@
                 else:
                     raise RuntimeError(f"Invalid extension '{extension}'.")
 
                 # Ignore dir name from archive file
                 compressed_fnames = [
                     fname
                     for fname in compressed_fnames
-                    if fname not in ("", CLOTHO_AUDIO_DNAMES[self.__subset])
+                    if fname not in ("", CLOTHO_AUDIO_DNAMES[self._subset])
                 ]
                 extracted_fnames = (
                     os.listdir(self.__dpath_audio_subset)
                     if osp.isdir(self.__dpath_audio_subset)
                     else []
                 )
 
@@ -756,25 +768,25 @@
                 archive_file.close()
 
             elif extension == "csv":
                 pass
 
             else:
                 logger.error(
-                    f"Found unexpected {extension=} for downloaded file '{fname}'. Expected one of {extensions}."
+                    f"Found unexpected extension={extension} for downloaded file '{fname}'. Expected one of {extensions}."
                 )
 
         if self.CLEAN_ARCHIVES:
             for file_info in links.values():
                 fname = file_info["fname"]
                 extension = fname.split(".")[-1]
 
                 if extension in ("7z", "zip"):
                     fpath = osp.join(self.__dpath_audio, fname)
-                    if self.__verbose >= 1:
+                    if self._verbose >= 1:
                         logger.info(f"Removing archive file {osp.basename(fpath)}...")
                     os.remove(fpath)
 
 
 CLOTHO_AUDIO_DNAMES = {
     "dev": "development",
     "eval": "evaluation",
```

### Comparing `aac_datasets-0.3.1/src/aac_datasets/datasets/macs.py` & `aac_datasets-0.3.2/src/aac_datasets/datasets/macs.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import logging
 import os
 import os.path as osp
 import shutil
 import zipfile
 
 from dataclasses import dataclass, field, fields
-from functools import cached_property
+from functools import lru_cache
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
 
 import torch
 import torchaudio
 import yaml
 
 from torch import Tensor
@@ -43,15 +43,15 @@
     competences: List[float] = field(default_factory=list)
     identifier: str = "unknown"
     scene_label: str = "unknown"
     tags: List[List[str]] = field(default_factory=list)
 
 
 class MACS(Dataset[Dict[str, Any]]):
-    r"""Unofficial MACS pytorch dataset.
+    r"""Unofficial MACS PyTorch dataset.
 
     .. code-block:: text
         :caption: Dataset folder tree
 
         {root}
         └── MACS
             ├── audio
@@ -103,45 +103,45 @@
         :param flat_captions: If True, map captions to audio instead of audio to caption.
             defaults to True.
         :param verbose: Verbose level to use. Can be 0 or 1.
             defaults to 0.
         """
         if subset not in self.SUBSETS:
             raise ValueError(
-                f"Invalid argument {subset=} for MACS. (expected one of {self.SUBSETS})"
+                f"Invalid argument subset={subset} for MACS. (expected one of {self.SUBSETS})"
             )
 
         super().__init__()
-        self.__root = root
-        self.__subset = subset
-        self.__download = download
-        self.__transform = transform
-        self.__flat_captions = flat_captions
-        self.__verbose = verbose
-
-        self.__annotator_id_to_competence = {}
-        self.__all_items = {}
-        self.__loaded = False
+        self._root = root
+        self._subset = subset
+        self._download = download
+        self._transform = transform
+        self._flat_captions = flat_captions
+        self._verbose = verbose
+
+        self._annotator_id_to_competence = {}
+        self._all_items = {}
+        self._loaded = False
 
-        if self.__download:
+        if self._download:
             self.__prepare_data()
         self.__load_data()
 
     # Properties
     @property
     def column_names(self) -> List[str]:
         """The name of each column of the dataset."""
         return [field.name for field in fields(MACSItem)]
 
     @property
     def info(self) -> Dict[str, Any]:
         """Return the global dataset info."""
         return {
             "dataset": "macs",
-            "subset": self.__subset,
+            "subset": self._subset,
         }
 
     @property
     def shape(self) -> Tuple[int, ...]:
         """The shape of the MACS dataset."""
         return len(self), len(self.column_names)
 
@@ -161,35 +161,40 @@
             idx = slice(None)
         if column is None:
             column = self.column_names
 
         if not isinstance(column, str) and isinstance(column, Iterable):
             return {column_i: self.at(idx, column_i) for column_i in column}
 
-        if isinstance(idx, (int, slice)) and column in self.__all_items.keys():
-            return self.__all_items[column][idx]
+        if isinstance(idx, (int, slice)) and column in self._all_items.keys():
+            return self._all_items[column][idx]
 
         if isinstance(idx, slice):
             idx = range(len(self))[idx]
 
         if isinstance(idx, Iterable):
+            idx = list(idx)
+            if not all(isinstance(idx_i, int) for idx_i in idx):
+                raise TypeError(
+                    f"Invalid input type for idx={idx}. (expected Iterable[int], not Iterable[{idx.__class__.__name__}])"
+                )
             return [self.at(idx_i, column) for idx_i in idx]
 
         if column == "audio":
             fpath = self.at(idx, "fpath")
             audio, sr = torchaudio.load(fpath)  # type: ignore
 
             # Sanity check
             if audio.nelement() == 0:
                 raise RuntimeError(
-                    f"Invalid audio number of elements in {fpath}. (expected {audio.nelement()=} > 0)"
+                    f"Invalid audio number of elements in {fpath}. (expected audio.nelement()={audio.nelement()} > 0)"
                 )
             if sr != self.SAMPLE_RATE:
                 raise RuntimeError(
-                    f"Invalid sample rate in {fpath}. (expected {self.SAMPLE_RATE} but found {sr=})"
+                    f"Invalid sample rate in {fpath}. (expected {self.SAMPLE_RATE} but found sr={sr})"
                 )
             return audio
 
         elif column == "audio_metadata":
             fpath = self.at(idx, "fpath")
             audio_metadata = torchaudio.info(fpath)  # type: ignore
             return audio_metadata
@@ -219,40 +224,40 @@
             return audio_metadata.num_frames
 
         elif column == "sr":
             audio_metadata = self.at(idx, "audio_metadata")
             return audio_metadata.sample_rate
 
         elif column == "subset":
-            return self.__subset
+            return self._subset
 
         else:
             raise ValueError(
-                f"Invalid argument {column=} at {idx=}. (expected one of {tuple(self.column_names)})"
+                f"Invalid argument column={column} at idx={idx}. (expected one of {tuple(self.column_names)})"
             )
 
     def get_annotator_id_to_competence_dict(self) -> Dict[int, float]:
         """Get annotator to competence dictionary."""
         # Note : copy to prevent any changes on this attribute
-        return copy.deepcopy(self.__annotator_id_to_competence)
+        return copy.deepcopy(self._annotator_id_to_competence)
 
     def get_competence(self, annotator_id: int) -> float:
         """Get competence value for a specific annotator id."""
-        return self.__annotator_id_to_competence[annotator_id]
+        return self._annotator_id_to_competence[annotator_id]
 
     def is_loaded(self) -> bool:
         """Returns True if the dataset is loaded."""
-        return self.__loaded
+        return self._loaded
 
     def set_transform(
         self,
         transform: Optional[Callable[[Dict[str, Any]], Any]],
     ) -> None:
         """Set the transform applied to each row."""
-        self.__transform = transform
+        self._transform = transform
 
     # Magic methods
     def __getitem__(
         self,
         idx: Any,
     ) -> Dict[str, Any]:
         if (
@@ -261,38 +266,42 @@
             and (isinstance(idx[1], (str, Iterable)) or idx[1] is None)
         ):
             idx, column = idx
         else:
             column = None
 
         item = self.at(idx, column)
-        if self.__transform is not None:
-            item = self.__transform(item)
+        if self._transform is not None:
+            item = self._transform(item)
         return item
 
     def __len__(self) -> int:
-        return len(self.__all_items["captions"])
+        return len(self._all_items["captions"])
 
     def __repr__(self) -> str:
-        return f"MACS(size={len(self)}, subset={self.__subset}, num_columns={len(self.column_names)})"
+        return f"MACS(size={len(self)}, subset={self._subset}, num_columns={len(self.column_names)})"
 
     # Private methods
-    @cached_property
+    @property
+    @lru_cache()
     def __dpath_archives(self) -> str:
         return osp.join(self.__dpath_data, "archives")
 
-    @cached_property
+    @property
+    @lru_cache()
     def __dpath_audio(self) -> str:
         return osp.join(self.__dpath_data, "audio")
 
-    @cached_property
+    @property
+    @lru_cache()
     def __dpath_data(self) -> str:
-        return osp.join(self.__root, "MACS")
+        return osp.join(self._root, "MACS")
 
-    @cached_property
+    @property
+    @lru_cache()
     def __dpath_tau_meta(self) -> str:
         return osp.join(self.__dpath_data, "tau_meta")
 
     def __is_prepared(self) -> bool:
         if not osp.isdir(self.__dpath_audio):
             return False
         captions_fpath = osp.join(self.__dpath_data, MACS_FILES["captions"]["fname"])
@@ -304,40 +313,40 @@
         data = data["files"]
         fnames = os.listdir(self.__dpath_audio)
         return len(data) == len(fnames)
 
     def __load_data(self) -> None:
         if not self.__is_prepared():
             raise RuntimeError(
-                f"Cannot load data: macs is not prepared in data root={self.__root}. Please use download=True in dataset constructor."
+                f"Cannot load data: macs is not prepared in data root={self._root}. Please use download=True in dataset constructor."
             )
 
         # Read data files
         captions_fname = MACS_FILES["captions"]["fname"]
         captions_fpath = osp.join(self.__dpath_data, captions_fname)
-        if self.__verbose >= 2:
+        if self._verbose >= 2:
             logger.debug(f"Reading captions file {captions_fname}...")
 
         with open(captions_fpath, "r") as file:
             caps_data = yaml.safe_load(file)
 
         tau_meta_fname = "meta.csv"
         tau_meta_fpath = osp.join(self.__dpath_tau_meta, tau_meta_fname)
-        if self.__verbose >= 2:
+        if self._verbose >= 2:
             logger.debug(
                 f"Reading Tau Urban acoustic scene meta file {tau_meta_fname}..."
             )
 
         with open(tau_meta_fpath, "r") as file:
             reader = csv.DictReader(file, delimiter="\t")
             tau_tags_data = list(reader)
 
         competence_fname = "MACS_competence.csv"
         competence_fpath = osp.join(self.__dpath_data, competence_fname)
-        if self.__verbose >= 2:
+        if self._verbose >= 2:
             logger.debug(f"Reading file {competence_fname}...")
 
         with open(competence_fpath, "r") as file:
             reader = csv.DictReader(file, delimiter="\t")
             competences_data = list(reader)
 
         # Store MACS data
@@ -363,26 +372,27 @@
         annotator_id_to_competence = {
             int(annotator["annotator_id"]): float(annotator["competence"])
             for annotator in competences_data
         }
 
         # Store TAU Urban acoustic scenes data
         tau_additional_keys = ("scene_label", "identifier")
-        all_items |= {
-            key: [None for _ in range(dataset_size)] for key in tau_additional_keys
-        }
+        all_items.update(
+            {key: [None for _ in range(dataset_size)] for key in tau_additional_keys}
+        )
+
         tau_meta_fpath = osp.join(self.__dpath_tau_meta, "meta.csv")
         for tau_tags in tau_tags_data:
             fname = osp.basename(tau_tags["filename"])
             if fname in fname_to_idx:
                 idx = fname_to_idx[fname]
                 for key in tau_additional_keys:
                     all_items[key][idx] = tau_tags[key]
 
-        if self.__flat_captions and self.MIN_CAPTIONS_PER_AUDIO[self.__subset] > 1:
+        if self._flat_captions and self.MIN_CAPTIONS_PER_AUDIO[self._subset] > 1:
             all_infos_unfolded = {key: [] for key in all_items.keys()}
 
             for i, captions in enumerate(all_items["captions"]):
                 for caption in captions:
                     for key in all_items.keys():
                         all_infos_unfolded[key].append(all_items[key][i])
                     all_infos_unfolded["captions"] = [caption]
@@ -393,44 +403,44 @@
         assert all(
             all(value is not None for value in all_items[key])
             for key in tau_additional_keys
         )
         assert all(len(values) == dataset_size for values in all_items.values())
 
         # Set attributes
-        self.__all_items = all_items
-        self.__annotator_id_to_competence = annotator_id_to_competence
-        self.__loaded = True
+        self._all_items = all_items
+        self._annotator_id_to_competence = annotator_id_to_competence
+        self._loaded = True
 
-        if self.__verbose >= 1:
+        if self._verbose >= 1:
             logger.info(f"{repr(self)} has been loaded. (len={len(self)})")
 
     def __prepare_data(self) -> None:
-        if not osp.isdir(self.__root):
-            raise RuntimeError(f"Cannot find root directory '{self.__root}'.")
+        if not osp.isdir(self._root):
+            raise RuntimeError(f"Cannot find root directory '{self._root}'.")
 
         os.makedirs(self.__dpath_archives, exist_ok=True)
         os.makedirs(self.__dpath_audio, exist_ok=True)
         os.makedirs(self.__dpath_tau_meta, exist_ok=True)
 
         # Download MACS specific files
         for file_info in MACS_FILES.values():
             dpath = self.__dpath_data
             fname = file_info["fname"]
             fpath = osp.join(dpath, fname)
 
             if not osp.isfile(fpath) or self.FORCE_PREPARE_DATA:
-                if self.__verbose >= 1:
+                if self._verbose >= 1:
                     logger.info(f"Downloading captions file '{fname}'...")
 
                 url = file_info["url"]
                 download_url_to_file(
                     url,
                     fpath,
-                    progress=self.__verbose >= 1,
+                    progress=self._verbose >= 1,
                 )
 
             hash_value = file_info["hash_value"]
             with open(fpath, "rb") as file:
                 valid = validate_file(file, hash_value, hash_type="md5")
             if not valid:
                 raise RuntimeError(f"Invalid checksum for file {fname}.")
@@ -443,41 +453,41 @@
         # Download TAU Urban Sound audio archives files
         for i, file_info in enumerate(MACS_ARCHIVES_FILES.values()):
             dpath = self.__dpath_archives
             zip_fname = file_info["fname"]
             zip_fpath = osp.join(dpath, zip_fname)
 
             if not osp.isfile(zip_fpath) or self.FORCE_PREPARE_DATA:
-                if self.__verbose >= 1:
+                if self._verbose >= 1:
                     logger.info(
                         f"Downloading audio zip file '{zip_fpath}'... ({i+1}/{len(MACS_ARCHIVES_FILES)})"
                     )
 
                 url = file_info["url"]
                 download_url_to_file(
                     url,
                     zip_fpath,
-                    progress=self.__verbose >= 1,
+                    progress=self._verbose >= 1,
                 )
 
             hash_value = file_info["hash_value"]
             with open(zip_fpath, "rb") as file:
                 valid = validate_file(file, hash_value, hash_type="md5")
             if not valid:
                 raise RuntimeError(f"Invalid checksum for file {zip_fname}.")
 
         # Extract files from TAU Urban Sound archives
         macs_fnames = dict.fromkeys(data["filename"] for data in captions_data)
         for i, (name, file_info) in enumerate(MACS_ARCHIVES_FILES.items()):
             zip_fname = file_info["fname"]
             zip_fpath = osp.join(self.__dpath_archives, zip_fname)
 
-            if self.__verbose >= 2:
+            if self._verbose >= 2:
                 logger.debug(
-                    f"Check to extract TAU Urban acoustic scenes archive {zip_fname=}..."
+                    f"Check to extract TAU Urban acoustic scenes archive zip_fname={zip_fname}..."
                 )
 
             is_audio_archive = name.startswith("audio")
             target_dpath = (
                 self.__dpath_audio if is_audio_archive else self.__dpath_tau_meta
             )
 
@@ -488,37 +498,37 @@
                     # Extract member if file if in captions yaml file and if the audio file is not already downloaded
                     if (
                         (osp.basename(member) in macs_fnames or not is_audio_archive)
                         and not osp.isfile(osp.join(target_dpath, osp.basename(member)))
                     )
                 ]
 
-                if self.__verbose >= 1:
+                if self._verbose >= 1:
                     logger.info(
                         f"Extracting {len(members_to_extract)}/{len(file.namelist())} audio files from ZIP file '{zip_fname}'... ({i+1}/{len(MACS_ARCHIVES_FILES)})"
                     )
 
                 if len(members_to_extract) > 0:
                     file.extractall(self.__dpath_archives, members_to_extract)
                     for member in members_to_extract:
                         extracted_fpath = osp.join(self.__dpath_archives, member)
                         target_fpath = osp.join(target_dpath, osp.basename(member))
                         shutil.move(extracted_fpath, target_fpath)
 
         if self.CLEAN_ARCHIVES:
-            if self.__verbose >= 1:
+            if self._verbose >= 1:
                 logger.info(f"Removing archives files in {self.__dpath_archives}...")
             shutil.rmtree(self.__dpath_archives, ignore_errors=True)
 
         audio_fnames = [
             name for name in os.listdir(self.__dpath_audio) if name.endswith(".wav")
         ]
         assert len(audio_fnames) == len(macs_fnames)
 
-        if self.__verbose >= 1:
+        if self._verbose >= 1:
             logger.info(
                 f"{len(audio_fnames)} audio files has been prepared for MACS dataset."
             )
 
 
 # MACS-specific files links.
 MACS_FILES = {
```

### Comparing `aac_datasets-0.3.1/src/aac_datasets/download.py` & `aac_datasets-0.3.2/src/aac_datasets/download.py`

 * *Files identical despite different names*

### Comparing `aac_datasets-0.3.1/src/aac_datasets/info.py` & `aac_datasets-0.3.2/src/aac_datasets/info.py`

 * *Files identical despite different names*

### Comparing `aac_datasets-0.3.1/src/aac_datasets/utils/collate.py` & `aac_datasets-0.3.2/src/aac_datasets/utils/collate.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,10 +113,10 @@
     if key_mode == "same":
         if not all(keys == set(item.keys()) for item in lst[1:]):
             raise ValueError("Invalid keys for batch.")
     elif key_mode == "intersect":
         for item in lst[1:]:
             keys = keys.intersection(item.keys())
     else:
-        raise ValueError(f"Invalid argument {key_mode=}.")
+        raise ValueError(f"Invalid argument key_mode={key_mode}.")
 
     return {key: [item[key] for item in lst] for key in keys}
```

### Comparing `aac_datasets-0.3.1/src/aac_datasets/utils.py` & `aac_datasets-0.3.2/src/aac_datasets/utils.py`

 * *Files identical despite different names*

### Comparing `aac_datasets-0.3.1/src/aac_datasets/version.py` & `aac_datasets-0.3.2/src/aac_datasets/version.py`

 * *Files identical despite different names*

### Comparing `aac_datasets-0.3.1/src/aac_datasets.egg-info/PKG-INFO` & `aac_datasets-0.3.2/src/aac_datasets.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: aac-datasets
-Version: 0.3.1
+Version: 0.3.2
 Summary: Audio Captioning datasets for Pytorch.
 Home-page: https://pypi.org/project/aac-datasets/
 Author: Etienne Labbé (Labbeti)
 License: MIT
 Project-URL: Documentation, https://aac-datasets.readthedocs.io/
 Project-URL: Source, https://github.com/Labbeti/aac-datasets
 Project-URL: PyPI, https://pypi.org/project/aac-datasets/
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <!-- # -*- coding: utf-8 -*- -->
 
 <div align="center">
 
-# Audio Captioning datasets for Pytorch
+# Audio Captioning datasets for PyTorch
 
 <a href="https://www.python.org/"><img alt="Python" src="https://img.shields.io/badge/-Python 3.8+-blue?style=for-the-badge&logo=python&logoColor=white"></a>
-<a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/-PyTorch 1.10.1-ee4c2c?style=for-the-badge&logo=pytorch&logoColor=white"></a>
+<a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/-PyTorch 1.10.1+-ee4c2c?style=for-the-badge&logo=pytorch&logoColor=white"></a>
 <a href="https://black.readthedocs.io/en/stable/"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-black.svg?style=for-the-badge&labelColor=gray"></a>
-<a href="https://github.com/Labbeti/aac-datasets/actions"><img alt="Build" src="https://img.shields.io/github/workflow/status/Labbeti/aac-datasets/Python%20package%20using%20Pip/main?style=for-the-badge&logo=github"></a>
+<a href="https://github.com/Labbeti/aac-datasets/actions"><img alt="Build" src="https://img.shields.io/github/actions/workflow/status/Labbeti/aac-datasets/python-package-pip.yaml?branch=main&style=for-the-badge&logo=github"></a>
 
-Audio Captioning unofficial datasets source code for **AudioCaps** [[1]](#audiocaps), **Clotho** [[2]](#clotho), and **MACS** [[3]](#macs), designed for Pytorch.
+Audio Captioning unofficial datasets source code for **AudioCaps** [[1]](#audiocaps), **Clotho** [[2]](#clotho), and **MACS** [[3]](#macs), designed for PyTorch.
 
 </div>
 
 ## Installation
 ```bash
 pip install aac-datasets
 ```
@@ -42,34 +41,34 @@
 ## Examples
 
 ### Create Clotho dataset
 
 ```python
 from aac_datasets import Clotho
 
-dataset = Clotho(root=".", subset="dev", download=True)
+dataset = Clotho(root=".", download=True)
 item = dataset[0]
 audio, captions = item["audio"], item["captions"]
 # audio: Tensor of shape (n_channels=1, audio_max_size)
-# captions: list of str captions
+# captions: list of str
 ```
 
-### Build Pytorch dataloader with Clotho
+### Build PyTorch dataloader with Clotho
 
 ```python
 from torch.utils.data.dataloader import DataLoader
 from aac_datasets import Clotho
 from aac_datasets.utils import BasicCollate
 
 dataset = Clotho(root=".", download=True)
 dataloader = DataLoader(dataset, batch_size=4, collate_fn=BasicCollate())
 
 for batch in dataloader:
-    # batch["audio"]: list of Tensor of shape (n_channels, audio_size)
-    # batch["captions"]: list of list of str
+    # batch["audio"]: list of 4 tensors of shape (n_channels, audio_size)
+    # batch["captions"]: list of 4 lists of str
     ...
 ```
 
 ## Datasets stats
 Here is the statistics for each dataset :
 
 | | AudioCaps | Clotho | MACS |
@@ -85,15 +84,15 @@
 |:---:|:---:|:---:|:---:|
 | Nb audios | 49838 | 3840 | 3930 |
 | Total audio duration | 136.6h<sup>1</sup> | 24.0h | 10.9h |
 | Audio duration range | 0.5-10s | 15-30s | 10s |
 | Nb captions per audio | 1 | 5 | 2-5 |
 | Nb captions | 49838 | 19195 | 17275 |
 | Total nb words<sup>2</sup> | 402482 | 217362 | 160006 |
-| Nb words range<sup>2</sup> | 2-52 | 8-20 | 5-40 |
+| Sentence size<sup>2</sup> | 2-52 | 8-20 | 5-40 |
 
 <sup>1</sup> This duration is estimated on the total duration of 46230/49838 files of 126.7h.
 
 <sup>2</sup> The sentences are cleaned (lowercase+remove punctuation) and tokenized using the spacy tokenizer to count the words.
 
 ## Requirements
 ### Python packages
@@ -116,19 +115,26 @@
 ```python
 from aac_datasets import AudioCaps
 AudioCaps.FFMPEG_PATH = "/my/path/to/ffmpeg"
 AudioCaps.YOUTUBE_DL_PATH = "/my/path/to/youtube_dl"
 dataset = AudioCaps(root=".", download=True)
 ```
 
-## Command line download
+## Download datasets
 To download a dataset, you can use `download=True` argument in dataset construction.
+
 However, if you want to download datasets separately, you can also use the following command :
 ```bash
-python -m aac_datasets.download --root "./data" clotho --version "v2.1"
+aac-datasets-download --root "." clotho --subsets "dev"
+```
+Or use the corresponding function in the code :
+```python
+from aac_datasets.download import download_clotho
+
+download_clotho(root=".", subsets=["dev"])
 ```
 
 ## References
 #### AudioCaps
 [1] C. D. Kim, B. Kim, H. Lee, and G. Kim, “Audiocaps: Generating captions for audios in the wild,” in NAACL-HLT, 2019. Available: https://aclanthology.org/N19-1011/
 
 #### Clotho
@@ -141,20 +147,18 @@
 If you use this software, please consider cite it as below :
 
 ```
 @software{
     Labbe_aac-datasets_2022,
     author = {Labbé, Etienne},
     license = {MIT},
-    month = {6},
+    month = {01},
     title = {{aac-datasets}},
     url = {https://github.com/Labbeti/aac-datasets/},
-    version = {0.3.1},
-    year = {2022}
+    version = {0.3.2},
+    year = {2023}
 }
 ```
 
 ## Contact
 Maintainer:
 - Etienne Labbé "Labbeti": labbeti.pub@gmail.com
-
-
```

#### html2text {}

```diff
@@ -1,66 +1,67 @@
-Metadata-Version: 2.1 Name: aac-datasets Version: 0.3.1 Summary: Audio
+Metadata-Version: 2.1 Name: aac-datasets Version: 0.3.2 Summary: Audio
 Captioning datasets for Pytorch. Home-page: https://pypi.org/project/aac-
 datasets/ Author: Etienne LabbÃ© (Labbeti) License: MIT Project-URL:
 Documentation, https://aac-datasets.readthedocs.io/ Project-URL: Source, https:
 //github.com/Labbeti/aac-datasets Project-URL: PyPI, https://pypi.org/project/
-aac-datasets/ Platform: UNKNOWN Classifier: Intended Audience :: Science/
-Research Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3.8 Classifier: Topic :: Scientific/
-Engineering Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Requires-Python: >=3.8 Description-Content-Type: text/markdown
-Provides-Extra: dev License-File: LICENSE
-# Audio Captioning datasets for Pytorch [Python] [PyTorch] [Code_style:_black]
+aac-datasets/ Classifier: Intended Audience :: Science/Research Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3.8 Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.7
+Description-Content-Type: text/markdown Provides-Extra: dev License-File:
+LICENSE
+# Audio Captioning datasets for PyTorch [Python] [PyTorch] [Code_style:_black]
  [Build] Audio Captioning unofficial datasets source code for **AudioCaps** [
     [1]](#audiocaps), **Clotho** [[2]](#clotho), and **MACS** [[3]](#macs),
-                             designed for Pytorch.
+                             designed for PyTorch.
 ## Installation ```bash pip install aac-datasets ``` ## Examples ### Create
 Clotho dataset ```python from aac_datasets import Clotho dataset = Clotho
-(root=".", subset="dev", download=True) item = dataset[0] audio, captions =
-item["audio"], item["captions"] # audio: Tensor of shape (n_channels=1,
-audio_max_size) # captions: list of str captions ``` ### Build Pytorch
-dataloader with Clotho ```python from torch.utils.data.dataloader import
-DataLoader from aac_datasets import Clotho from aac_datasets.utils import
-BasicCollate dataset = Clotho(root=".", download=True) dataloader = DataLoader
-(dataset, batch_size=4, collate_fn=BasicCollate()) for batch in dataloader: #
-batch["audio"]: list of Tensor of shape (n_channels, audio_size) # batch
-["captions"]: list of list of str ... ``` ## Datasets stats Here is the
-statistics for each dataset : | | AudioCaps | Clotho | MACS | |:---:|:---:|:--
--:|:---:| | Subset(s) | train, val, test | dev, val, eval, test, analysis |
-full | | Sample rate | 32000 | 44100 | 48000 | | Estimated size | 43GB | 27GB |
-13GB | | Audio source | AudioSet (youtube) | Freesound | TAU Urban Acoustic
-Scenes 2019 | Here is the **train** subset statistics for each dataset : | |
-AudioCaps/train | Clotho/dev | MACS/full | |:---:|:---:|:---:|:---:| | Nb
-audios | 49838 | 3840 | 3930 | | Total audio duration | 136.6h1 | 24.0h | 10.9h
-| | Audio duration range | 0.5-10s | 15-30s | 10s | | Nb captions per audio | 1
-| 5 | 2-5 | | Nb captions | 49838 | 19195 | 17275 | | Total nb words2 | 402482
-| 217362 | 160006 | | Nb words range2 | 2-52 | 8-20 | 5-40 | 1 This duration is
-estimated on the total duration of 46230/49838 files of 126.7h. 2 The sentences
-are cleaned (lowercase+remove punctuation) and tokenized using the spacy
-tokenizer to count the words. ## Requirements ### Python packages The
-requirements are automatically installed when using pip on this repository. ```
-torch >= 1.10.1 torchaudio >= 0.10.1 py7zr >= 0.17.2 pyyaml >= 6.0 tqdm >=
-4.64.0 ``` ### External requirements (AudioCaps only) The external requirements
-needed to download **AudioCaps** are **ffmpeg** and **youtube-dl**. These two
-programs can be download on Ubuntu using `sudo apt install ffmpeg youtube-dl`.
-You can also override their paths for AudioCaps: ```python from aac_datasets
-import AudioCaps AudioCaps.FFMPEG_PATH = "/my/path/to/ffmpeg"
-AudioCaps.YOUTUBE_DL_PATH = "/my/path/to/youtube_dl" dataset = AudioCaps
-(root=".", download=True) ``` ## Command line download To download a dataset,
-you can use `download=True` argument in dataset construction. However, if you
-want to download datasets separately, you can also use the following command :
-```bash python -m aac_datasets.download --root "./data" clotho --version "v2.1"
-``` ## References #### AudioCaps [1] C. D. Kim, B. Kim, H. Lee, and G. Kim,
-âAudiocaps: Generating captions for audios in the wild,â in NAACL-HLT,
-2019. Available: https://aclanthology.org/N19-1011/ #### Clotho [2] K. Drossos,
-S. Lipping, and T. Virtanen, âClotho: An Audio Captioning Dataset,â arXiv:
-1910.09387 [cs, eess], Oct. 2019, Available: http://arxiv.org/abs/1910.09387
-#### MACS [3] F. Font, A. Mesaros, D. P. W. Ellis, E. Fonseca, M. Fuentes, and
-B. Elizalde, Proceedings of the 6th Workshop on Detection and Classication of
-Acoustic Scenes and Events (DCASE 2021). Barcelona, Spain: Music Technology
-Group - Universitat Pompeu Fabra, Nov. 2021. Available: https://doi.org/
-10.5281/zenodo.5770113 ## Cite the aac-datasets package If you use this
-software, please consider cite it as below : ``` @software{ Labbe_aac-
-datasets_2022, author = {LabbÃ©, Etienne}, license = {MIT}, month = {6}, title
-= {{aac-datasets}}, url = {https://github.com/Labbeti/aac-datasets/}, version =
-{0.3.1}, year = {2022} } ``` ## Contact Maintainer: - Etienne LabbÃ© "Labbeti":
-labbeti.pub@gmail.com
+(root=".", download=True) item = dataset[0] audio, captions = item["audio"],
+item["captions"] # audio: Tensor of shape (n_channels=1, audio_max_size) #
+captions: list of str ``` ### Build PyTorch dataloader with Clotho ```python
+from torch.utils.data.dataloader import DataLoader from aac_datasets import
+Clotho from aac_datasets.utils import BasicCollate dataset = Clotho(root=".",
+download=True) dataloader = DataLoader(dataset, batch_size=4,
+collate_fn=BasicCollate()) for batch in dataloader: # batch["audio"]: list of 4
+tensors of shape (n_channels, audio_size) # batch["captions"]: list of 4 lists
+of str ... ``` ## Datasets stats Here is the statistics for each dataset : | |
+AudioCaps | Clotho | MACS | |:---:|:---:|:---:|:---:| | Subset(s) | train, val,
+test | dev, val, eval, test, analysis | full | | Sample rate | 32000 | 44100 |
+48000 | | Estimated size | 43GB | 27GB | 13GB | | Audio source | AudioSet
+(youtube) | Freesound | TAU Urban Acoustic Scenes 2019 | Here is the **train**
+subset statistics for each dataset : | | AudioCaps/train | Clotho/dev | MACS/
+full | |:---:|:---:|:---:|:---:| | Nb audios | 49838 | 3840 | 3930 | | Total
+audio duration | 136.6h1 | 24.0h | 10.9h | | Audio duration range | 0.5-10s |
+15-30s | 10s | | Nb captions per audio | 1 | 5 | 2-5 | | Nb captions | 49838 |
+19195 | 17275 | | Total nb words2 | 402482 | 217362 | 160006 | | Sentence size2
+| 2-52 | 8-20 | 5-40 | 1 This duration is estimated on the total duration of
+46230/49838 files of 126.7h. 2 The sentences are cleaned (lowercase+remove
+punctuation) and tokenized using the spacy tokenizer to count the words. ##
+Requirements ### Python packages The requirements are automatically installed
+when using pip on this repository. ``` torch >= 1.10.1 torchaudio >= 0.10.1
+py7zr >= 0.17.2 pyyaml >= 6.0 tqdm >= 4.64.0 ``` ### External requirements
+(AudioCaps only) The external requirements needed to download **AudioCaps** are
+**ffmpeg** and **youtube-dl**. These two programs can be download on Ubuntu
+using `sudo apt install ffmpeg youtube-dl`. You can also override their paths
+for AudioCaps: ```python from aac_datasets import AudioCaps
+AudioCaps.FFMPEG_PATH = "/my/path/to/ffmpeg" AudioCaps.YOUTUBE_DL_PATH = "/my/
+path/to/youtube_dl" dataset = AudioCaps(root=".", download=True) ``` ##
+Download datasets To download a dataset, you can use `download=True` argument
+in dataset construction. However, if you want to download datasets separately,
+you can also use the following command : ```bash aac-datasets-download --root
+"." clotho --subsets "dev" ``` Or use the corresponding function in the code :
+```python from aac_datasets.download import download_clotho download_clotho
+(root=".", subsets=["dev"]) ``` ## References #### AudioCaps [1] C. D. Kim, B.
+Kim, H. Lee, and G. Kim, âAudiocaps: Generating captions for audios in the
+wild,â in NAACL-HLT, 2019. Available: https://aclanthology.org/N19-1011/ ####
+Clotho [2] K. Drossos, S. Lipping, and T. Virtanen, âClotho: An Audio
+Captioning Dataset,â arXiv:1910.09387 [cs, eess], Oct. 2019, Available: http:
+//arxiv.org/abs/1910.09387 #### MACS [3] F. Font, A. Mesaros, D. P. W. Ellis,
+E. Fonseca, M. Fuentes, and B. Elizalde, Proceedings of the 6th Workshop on
+Detection and Classication of Acoustic Scenes and Events (DCASE 2021).
+Barcelona, Spain: Music Technology Group - Universitat Pompeu Fabra, Nov. 2021.
+Available: https://doi.org/10.5281/zenodo.5770113 ## Cite the aac-datasets
+package If you use this software, please consider cite it as below : ```
+@software{ Labbe_aac-datasets_2022, author = {LabbÃ©, Etienne}, license =
+{MIT}, month = {01}, title = {{aac-datasets}}, url = {https://github.com/
+Labbeti/aac-datasets/}, version = {0.3.2}, year = {2023} } ``` ## Contact
+Maintainer: - Etienne LabbÃ© "Labbeti": labbeti.pub@gmail.com
```

### Comparing `aac_datasets-0.3.1/src/aac_datasets.egg-info/SOURCES.txt` & `aac_datasets-0.3.2/src/aac_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

