# Comparing `tmp/popv-0.2.1.tar.gz` & `tmp/popv-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popv-0.2.1.tar", max compression
+gzip compressed data, was "popv-0.2.2.tar", max compression
```

## Comparing `popv-0.2.1.tar` & `popv-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1067 2023-01-27 08:23:56.770098 popv-0.2.1/LICENSE
--rw-r--r--   0        0        0     6513 2023-05-10 14:11:33.843003 popv-0.2.1/README.md
--rw-r--r--   0        0        0      730 2023-02-04 09:31:22.143889 popv-0.2.1/popv/__init__.py
--rw-r--r--   0        0        0     2926 2023-02-04 09:31:22.143889 popv-0.2.1/popv/_settings.py
--rw-r--r--   0        0        0     4953 2023-05-09 13:10:44.633839 popv-0.2.1/popv/_utils.py
--rw-r--r--   0        0        0      475 2023-02-04 09:31:22.143889 popv-0.2.1/popv/algorithms/__init__.py
--rw-r--r--   0        0        0     3895 2023-05-09 15:13:49.394527 popv-0.2.1/popv/algorithms/_bbknn.py
--rw-r--r--   0        0        0     2744 2023-02-17 07:50:33.768775 popv-0.2.1/popv/algorithms/_celltypist.py
--rw-r--r--   0        0        0     7494 2023-05-09 14:08:51.333824 popv-0.2.1/popv/algorithms/_onclass.py
--rw-r--r--   0        0        0     2958 2023-03-23 00:34:48.123721 popv-0.2.1/popv/algorithms/_rf.py
--rw-r--r--   0        0        0     3229 2023-02-17 07:50:33.768775 popv-0.2.1/popv/algorithms/_scaffold_algorithm.py
--rw-r--r--   0        0        0     3525 2023-02-17 07:50:33.768775 popv-0.2.1/popv/algorithms/_scanorama.py
--rw-r--r--   0        0        0     7460 2023-02-04 09:31:22.147889 popv-0.2.1/popv/algorithms/_scanvi.py
--rw-r--r--   0        0        0     6697 2023-03-23 00:17:40.248214 popv-0.2.1/popv/algorithms/_scvi.py
--rw-r--r--   0        0        0     3063 2023-02-04 09:31:22.147889 popv-0.2.1/popv/algorithms/_svm.py
--rw-r--r--   0        0        0    10981 2023-03-11 22:16:34.706423 popv-0.2.1/popv/annotation.py
--rw-r--r--   0        0        0    16716 2023-05-09 14:08:51.417825 popv-0.2.1/popv/preprocessing.py
--rw-r--r--   0        0        0     2643 2023-05-09 14:08:51.273823 popv-0.2.1/popv/reproducibility/_accuracy.py
--rw-r--r--   0        0        0    12900 2023-05-09 14:08:51.445825 popv-0.2.1/popv/reproducibility/_alluvial.py
--rwxr-xr-x   0        0        0     8997 2023-03-12 06:52:28.135061 popv-0.2.1/popv/visualization.py
--rw-r--r--   0        0        0     2448 2023-05-10 17:11:44.678104 popv-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     8205 1970-01-01 00:00:00.000000 popv-0.2.1/setup.py
--rw-r--r--   0        0        0     8999 1970-01-01 00:00:00.000000 popv-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-01-27 08:23:56.770098 popv-0.2.2/LICENSE
+-rw-r--r--   0        0        0     6301 2023-05-11 05:02:47.119626 popv-0.2.2/README.md
+-rw-r--r--   0        0        0      730 2023-02-04 09:31:22.143889 popv-0.2.2/popv/__init__.py
+-rw-r--r--   0        0        0     2926 2023-02-04 09:31:22.143889 popv-0.2.2/popv/_settings.py
+-rw-r--r--   0        0        0     4953 2023-05-09 13:10:44.633839 popv-0.2.2/popv/_utils.py
+-rw-r--r--   0        0        0      475 2023-02-04 09:31:22.143889 popv-0.2.2/popv/algorithms/__init__.py
+-rw-r--r--   0        0        0     3895 2023-05-09 15:13:49.394527 popv-0.2.2/popv/algorithms/_bbknn.py
+-rw-r--r--   0        0        0     2744 2023-02-17 07:50:33.768775 popv-0.2.2/popv/algorithms/_celltypist.py
+-rw-r--r--   0        0        0     7494 2023-05-09 14:08:51.333824 popv-0.2.2/popv/algorithms/_onclass.py
+-rw-r--r--   0        0        0     2958 2023-03-23 00:34:48.123721 popv-0.2.2/popv/algorithms/_rf.py
+-rw-r--r--   0        0        0     3229 2023-02-17 07:50:33.768775 popv-0.2.2/popv/algorithms/_scaffold_algorithm.py
+-rw-r--r--   0        0        0     3525 2023-02-17 07:50:33.768775 popv-0.2.2/popv/algorithms/_scanorama.py
+-rw-r--r--   0        0        0     7460 2023-02-04 09:31:22.147889 popv-0.2.2/popv/algorithms/_scanvi.py
+-rw-r--r--   0        0        0     6697 2023-03-23 00:17:40.248214 popv-0.2.2/popv/algorithms/_scvi.py
+-rw-r--r--   0        0        0     3063 2023-02-04 09:31:22.147889 popv-0.2.2/popv/algorithms/_svm.py
+-rw-r--r--   0        0        0    10981 2023-03-11 22:16:34.706423 popv-0.2.2/popv/annotation.py
+-rw-r--r--   0        0        0    16716 2023-05-09 14:08:51.417825 popv-0.2.2/popv/preprocessing.py
+-rw-r--r--   0        0        0     2643 2023-05-09 14:08:51.273823 popv-0.2.2/popv/reproducibility/_accuracy.py
+-rw-r--r--   0        0        0    12900 2023-05-09 14:08:51.445825 popv-0.2.2/popv/reproducibility/_alluvial.py
+-rwxr-xr-x   0        0        0     8997 2023-03-12 06:52:28.135061 popv-0.2.2/popv/visualization.py
+-rw-r--r--   0        0        0     4650 2023-05-11 05:38:18.737545 popv-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     7991 1970-01-01 00:00:00.000000 popv-0.2.2/setup.py
+-rw-r--r--   0        0        0     8787 1970-01-01 00:00:00.000000 popv-0.2.2/PKG-INFO
```

### Comparing `popv-0.2.1/LICENSE` & `popv-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `popv-0.2.1/README.md` & `popv-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 [![Stars](https://img.shields.io/github/stars/yoseflab/popv?logo=GitHub&color=yellow)](https://github.com/YosefLab/popv/stargazers)
 [![PyPI](https://img.shields.io/pypi/v/popv.svg)](https://pypi.org/project/popv)
-![Build Status](https://github.com/yoseflab/popv/workflows/popv/badge.svg)
-[![Coverage](https://codecov.io/gh/yoseflab/popv/branch/master/graph/badge.svg)](https://codecov.io/gh/YosefLab/popv)
+[![PopV](https://github.com/YosefLab/PopV/actions/workflows/test.yml/badge.svg)](https://github.com/YosefLab/PopV/actions/workflows/test.yml)
+[![Coverage](https://codecov.io/gh/YosefLab/popv/branch/main/graph/badge.svg?token=KuSsL5q3l7)](https://codecov.io/gh/YosefLab/popv)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![Downloads](https://pepy.tech/badge/popv)](https://pepy.tech/project/popv)
 
 # PopV
 
 PopV uses popular vote of a variety of cell-type transfer tools to classify cell-types in a query dataset based on a test dataset.
 Using this variety of algorithms, we compute the agreement between those algorithms and use this agreement to predict which cell-types are with a high likelihood the same cell-types observed in the reference.
@@ -54,16 +54,14 @@
 
     conda create -n yourenv python=3.8
     conda activate yourenv
     pip install git+https://github.com/czbiohub/PopV
 
 ## Example notebook
 
-We deposited an example notebook in Google Colab:
+We provide an example notebook in Google Colab:
 
 -   [Tutorial demonstrating use of Tabula sapiens as a reference](tabula_sapiens_tutorial.ipynb)
 
 This notebook will guide you through annotating a dataset based on the annotated [Tabula sapiens reference](https://tabula-sapiens-portal.ds.czbiohub.org) and demonstrates how to run annotation on your own query dataset. This notebook requires that all cells are annotated based on a cell ontology. We strongly encourage the use of a common cell ontology, see also [Osumi-Sutherland et al](https://www.nature.com/articles/s41556-021-00787-7). Using a cell ontology is a requirement to run OnClass as a prediction algorithm.
 
-However, for other organisms than human no ontology exists. We therefore allow running PopV without using a cell ontology. A second notebook highlighting using PopV without an existing ontology is currently planned and will be released here.
-
-Memory requirements exceed the free limit in Colab and we recommend a Pro access to run the notebook.
+We allow running PopV without using a cell ontology.
```

### Comparing `popv-0.2.1/popv/__init__.py` & `popv-0.2.2/popv/__init__.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.1/popv/_settings.py` & `popv-0.2.2/popv/_settings.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.1/popv/_utils.py` & `popv-0.2.2/popv/_utils.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.1/popv/algorithms/_bbknn.py` & `popv-0.2.2/popv/algorithms/_bbknn.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.1/popv/algorithms/_celltypist.py` & `popv-0.2.2/popv/algorithms/_celltypist.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.1/popv/algorithms/_onclass.py` & `popv-0.2.2/popv/algorithms/_onclass.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.1/popv/algorithms/_rf.py` & `popv-0.2.2/popv/algorithms/_rf.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.1/popv/algorithms/_scaffold_algorithm.py` & `popv-0.2.2/popv/algorithms/_scaffold_algorithm.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.1/popv/algorithms/_scanorama.py` & `popv-0.2.2/popv/algorithms/_scanorama.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.1/popv/algorithms/_scanvi.py` & `popv-0.2.2/popv/algorithms/_scanvi.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.1/popv/algorithms/_scvi.py` & `popv-0.2.2/popv/algorithms/_scvi.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.1/popv/algorithms/_svm.py` & `popv-0.2.2/popv/algorithms/_svm.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.1/popv/annotation.py` & `popv-0.2.2/popv/annotation.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.1/popv/preprocessing.py` & `popv-0.2.2/popv/preprocessing.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.1/popv/reproducibility/_accuracy.py` & `popv-0.2.2/popv/reproducibility/_accuracy.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.1/popv/reproducibility/_alluvial.py` & `popv-0.2.2/popv/reproducibility/_alluvial.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.1/popv/visualization.py` & `popv-0.2.2/popv/visualization.py`

 * *Files identical despite different names*

### Comparing `popv-0.2.1/setup.py` & `popv-0.2.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'gdown>=4.6.0,<5.0.0',
  'grpcio>=1.51.1,<2.0.0',
  'h5py>=3.7.0,<4.0.0',
  'huggingface-hub==0.11.1',
  'imgkit==1.2.2',
  'importlib-metadata==4.2.0',
  'ipywidgets',
- 'numpy>1.21.5',
+ 'numpy>1.23.5',
  'obonet>=1.0,<2.0',
  'onclass>=1.2,<2.0',
  'pandas>=1.4',
  'rich>=9.1.0',
  'scanorama>=1.7.3,<2.0.0',
  'scanpy>=1.9.1,<2.0.0',
  'scikit-learn>0.21.2,<1.0',
@@ -44,17 +44,17 @@
          'nbconvert>=5.4.0',
          'nbformat>=4.4.0',
          'pre-commit>=2.7.1',
          'pytest>=4.4']}
 
 setup_kwargs = {
     'name': 'popv',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Automatic annotation of single cell data using a labelled reference dataset including various methods and giving certainty across those methods.',
-    'long_description': '\n[![Stars](https://img.shields.io/github/stars/yoseflab/popv?logo=GitHub&color=yellow)](https://github.com/YosefLab/popv/stargazers)\n[![PyPI](https://img.shields.io/pypi/v/popv.svg)](https://pypi.org/project/popv)\n![Build Status](https://github.com/yoseflab/popv/workflows/popv/badge.svg)\n[![Coverage](https://codecov.io/gh/yoseflab/popv/branch/master/graph/badge.svg)](https://codecov.io/gh/YosefLab/popv)\n[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)\n[![Downloads](https://pepy.tech/badge/popv)](https://pepy.tech/project/popv)\n\n# PopV\n\nPopV uses popular vote of a variety of cell-type transfer tools to classify cell-types in a query dataset based on a test dataset.\nUsing this variety of algorithms, we compute the agreement between those algorithms and use this agreement to predict which cell-types are with a high likelihood the same cell-types observed in the reference.\n\n## Algorithms\n\nCurrently implemented algorithms are:\n\n-   K-nearest neighbor classification after dataset integration with [BBKNN](https://github.com/Teichlab/bbknn)\n-   K-nearest neighbor classification after dataset integration with [SCANORAMA](https://github.com/brianhie/scanorama)\n-   K-nearest neighbor classification after dataset integration with [scVI](https://github.com/scverse/scvi-tools)\n-   Random forest classification\n-   Support vector machine classification\n-   [OnClass](https://github.com/wangshenguiuc/OnClass) cell type classification\n-   [scANVI](https://github.com/scverse/scvi-tools) label transfer\n-   [Celltypist](https://www.celltypist.org) cell type classification\n\nAll algorithms are implemented as a class in [popv/algorithms](popv/algorithms/__init__.py).\nTo implement a new method, a class has to have several methods:\n\n-   algorithm.compute_integration: Computes dataset integration to yield an integrated latent space.\n-   algorithm.predict: Computes cell-type labels based on the specific classifier.\n-   algorithm.compute_embedding: Computes UMAP embedding of previously computed integrated latent space.\n\nWe highlight the implementation of a new classifier in a [scaffold](popv/algorithms/_scaffold.py). Adding a new class with those methods will automatically tell PopV to include this class into its classifiers and will use the new classifier as another expert.\n\nAll algorithms that allow for pre-training are pre-trained. This excludes by design BBKNN and SCANORAMA as both construct a new embedding space. Pretrained models are stored on (Zenodo)[https://zenodo.org/record/7580707] and are automatically downloaded in the Colab notebook linked below. We encourage pre-training models when implementing new classes.\n\nAll input parameters are defined during initial call to [Process_Query](popv/preprocessing.py) and are stored in the unstructured field of the generated AnnData object. PopV has three levels of prediction complexities:\n\n-   retrain will train all classifiers from scratch. For 50k cells this takes up to an hour of computing time using a GPU.\n-   inference will use pretrained classifiers to annotate query as well as reference cells and construct a joint embedding using all integration methods from above. For 50k cells this takes in our hands up to half an hour of computing time using a GPU.\n-   fast will use only methods with pretrained classifiers to annotate only query cells. For 50k cells this takes 5 minutes without a GPU (without UMAP embedding).\n\nA user-defined selection of classification algorithms can be defined when calling [annotate_data](popv/annotation.py). Additionally advanced users can define here non-standard parameters for the integration methods as well as the classifiers.\n\n## Output\n\nPopV will output a cell-type classification for each of the used classifiers, as well as the majority vote across all classifiers. Additionally, PopV uses the ontology to go through the full ontology descendants for the OnClass prediction (disabled in fast mode). This method will be further described when PopV is published. PopV additionally outputs a score, which counts the number of classifiers that agreed upon the PopV prediction. This can be seen as the certainty that the current prediction is correct for every single cell in the query data. We generally found disagreement of a single expert to be still highly reliable while disagreement of more than 2 classifiers signifies less reliable results. The aim of PopV is not to fully annotate a data set but to highlight cells that potentially benefit from further manual careful annotation.\nAdditionally, PopV outputs UMAP embeddings of all integrated latent spaces if _compute_embedding==True_ in [Process_Query](popv/preprocessing.py) and computes certainties for every used classifier if _return_probabilities==True_ in [Process_Query](popv/preprocessing.py).\n\n## Installation\n\nWe suggest using a package manager like conda or mamba to install the package. OnClass files for annotation based on Tabula sapiens are deposited in popv/ontology. We use [Cell Ontology](https://obofoundry.org/ontology/cl.html) as an ontology throughout our experiments. PopV will automatically look for the ontology in this folder. If you want to provide your user-edited ontology, we will provide notebooks to create the Natural Language Model used in OnClass for this user-defined ontology.\n\n    conda create -n yourenv python=3.8\n    conda activate yourenv\n    pip install git+https://github.com/czbiohub/PopV\n\n## Example notebook\n\nWe deposited an example notebook in Google Colab:\n\n-   [Tutorial demonstrating use of Tabula sapiens as a reference](tabula_sapiens_tutorial.ipynb)\n\nThis notebook will guide you through annotating a dataset based on the annotated [Tabula sapiens reference](https://tabula-sapiens-portal.ds.czbiohub.org) and demonstrates how to run annotation on your own query dataset. This notebook requires that all cells are annotated based on a cell ontology. We strongly encourage the use of a common cell ontology, see also [Osumi-Sutherland et al](https://www.nature.com/articles/s41556-021-00787-7). Using a cell ontology is a requirement to run OnClass as a prediction algorithm.\n\nHowever, for other organisms than human no ontology exists. We therefore allow running PopV without using a cell ontology. A second notebook highlighting using PopV without an existing ontology is currently planned and will be released here.\n\nMemory requirements exceed the free limit in Colab and we recommend a Pro access to run the notebook.\n',
+    'long_description': '\n[![Stars](https://img.shields.io/github/stars/yoseflab/popv?logo=GitHub&color=yellow)](https://github.com/YosefLab/popv/stargazers)\n[![PyPI](https://img.shields.io/pypi/v/popv.svg)](https://pypi.org/project/popv)\n[![PopV](https://github.com/YosefLab/PopV/actions/workflows/test.yml/badge.svg)](https://github.com/YosefLab/PopV/actions/workflows/test.yml)\n[![Coverage](https://codecov.io/gh/YosefLab/popv/branch/main/graph/badge.svg?token=KuSsL5q3l7)](https://codecov.io/gh/YosefLab/popv)\n[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)\n[![Downloads](https://pepy.tech/badge/popv)](https://pepy.tech/project/popv)\n\n# PopV\n\nPopV uses popular vote of a variety of cell-type transfer tools to classify cell-types in a query dataset based on a test dataset.\nUsing this variety of algorithms, we compute the agreement between those algorithms and use this agreement to predict which cell-types are with a high likelihood the same cell-types observed in the reference.\n\n## Algorithms\n\nCurrently implemented algorithms are:\n\n-   K-nearest neighbor classification after dataset integration with [BBKNN](https://github.com/Teichlab/bbknn)\n-   K-nearest neighbor classification after dataset integration with [SCANORAMA](https://github.com/brianhie/scanorama)\n-   K-nearest neighbor classification after dataset integration with [scVI](https://github.com/scverse/scvi-tools)\n-   Random forest classification\n-   Support vector machine classification\n-   [OnClass](https://github.com/wangshenguiuc/OnClass) cell type classification\n-   [scANVI](https://github.com/scverse/scvi-tools) label transfer\n-   [Celltypist](https://www.celltypist.org) cell type classification\n\nAll algorithms are implemented as a class in [popv/algorithms](popv/algorithms/__init__.py).\nTo implement a new method, a class has to have several methods:\n\n-   algorithm.compute_integration: Computes dataset integration to yield an integrated latent space.\n-   algorithm.predict: Computes cell-type labels based on the specific classifier.\n-   algorithm.compute_embedding: Computes UMAP embedding of previously computed integrated latent space.\n\nWe highlight the implementation of a new classifier in a [scaffold](popv/algorithms/_scaffold.py). Adding a new class with those methods will automatically tell PopV to include this class into its classifiers and will use the new classifier as another expert.\n\nAll algorithms that allow for pre-training are pre-trained. This excludes by design BBKNN and SCANORAMA as both construct a new embedding space. Pretrained models are stored on (Zenodo)[https://zenodo.org/record/7580707] and are automatically downloaded in the Colab notebook linked below. We encourage pre-training models when implementing new classes.\n\nAll input parameters are defined during initial call to [Process_Query](popv/preprocessing.py) and are stored in the unstructured field of the generated AnnData object. PopV has three levels of prediction complexities:\n\n-   retrain will train all classifiers from scratch. For 50k cells this takes up to an hour of computing time using a GPU.\n-   inference will use pretrained classifiers to annotate query as well as reference cells and construct a joint embedding using all integration methods from above. For 50k cells this takes in our hands up to half an hour of computing time using a GPU.\n-   fast will use only methods with pretrained classifiers to annotate only query cells. For 50k cells this takes 5 minutes without a GPU (without UMAP embedding).\n\nA user-defined selection of classification algorithms can be defined when calling [annotate_data](popv/annotation.py). Additionally advanced users can define here non-standard parameters for the integration methods as well as the classifiers.\n\n## Output\n\nPopV will output a cell-type classification for each of the used classifiers, as well as the majority vote across all classifiers. Additionally, PopV uses the ontology to go through the full ontology descendants for the OnClass prediction (disabled in fast mode). This method will be further described when PopV is published. PopV additionally outputs a score, which counts the number of classifiers that agreed upon the PopV prediction. This can be seen as the certainty that the current prediction is correct for every single cell in the query data. We generally found disagreement of a single expert to be still highly reliable while disagreement of more than 2 classifiers signifies less reliable results. The aim of PopV is not to fully annotate a data set but to highlight cells that potentially benefit from further manual careful annotation.\nAdditionally, PopV outputs UMAP embeddings of all integrated latent spaces if _compute_embedding==True_ in [Process_Query](popv/preprocessing.py) and computes certainties for every used classifier if _return_probabilities==True_ in [Process_Query](popv/preprocessing.py).\n\n## Installation\n\nWe suggest using a package manager like conda or mamba to install the package. OnClass files for annotation based on Tabula sapiens are deposited in popv/ontology. We use [Cell Ontology](https://obofoundry.org/ontology/cl.html) as an ontology throughout our experiments. PopV will automatically look for the ontology in this folder. If you want to provide your user-edited ontology, we will provide notebooks to create the Natural Language Model used in OnClass for this user-defined ontology.\n\n    conda create -n yourenv python=3.8\n    conda activate yourenv\n    pip install git+https://github.com/czbiohub/PopV\n\n## Example notebook\n\nWe provide an example notebook in Google Colab:\n\n-   [Tutorial demonstrating use of Tabula sapiens as a reference](tabula_sapiens_tutorial.ipynb)\n\nThis notebook will guide you through annotating a dataset based on the annotated [Tabula sapiens reference](https://tabula-sapiens-portal.ds.czbiohub.org) and demonstrates how to run annotation on your own query dataset. This notebook requires that all cells are annotated based on a cell ontology. We strongly encourage the use of a common cell ontology, see also [Osumi-Sutherland et al](https://www.nature.com/articles/s41556-021-00787-7). Using a cell ontology is a requirement to run OnClass as a prediction algorithm.\n\nWe allow running PopV without using a cell ontology.\n',
     'author': 'Galen Xing',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `popv-0.2.1/PKG-INFO` & `popv-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popv
-Version: 0.2.1
+Version: 0.2.2
 Summary: Automatic annotation of single cell data using a labelled reference dataset including various methods and giving certainty across those methods.
 License: BSD-3-Clause
 Author: Galen Xing
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -36,15 +36,15 @@
 Requires-Dist: ipywidgets
 Requires-Dist: isort (>=5.7) ; extra == "dev"
 Requires-Dist: jupyter (>=1.0) ; extra == "dev"
 Requires-Dist: nbconvert (>=5.4.0) ; extra == "dev"
 Requires-Dist: nbformat (>=4.4.0) ; extra == "dev"
 Requires-Dist: nbsphinx
 Requires-Dist: nbsphinx-link
-Requires-Dist: numpy (>1.21.5)
+Requires-Dist: numpy (>1.23.5)
 Requires-Dist: obonet (>=1.0,<2.0)
 Requires-Dist: onclass (>=1.2,<2.0)
 Requires-Dist: pandas (>=1.4)
 Requires-Dist: pre-commit (>=2.7.1) ; extra == "dev"
 Requires-Dist: pytest (>=4.4) ; extra == "dev"
 Requires-Dist: rich (>=9.1.0)
 Requires-Dist: scanorama (>=1.7.3,<2.0.0)
@@ -58,16 +58,16 @@
 Requires-Dist: transformers (>=4.25.1,<5.0.0)
 Requires-Dist: typing-extensions (==4.2.0)
 Description-Content-Type: text/markdown
 
 
 [![Stars](https://img.shields.io/github/stars/yoseflab/popv?logo=GitHub&color=yellow)](https://github.com/YosefLab/popv/stargazers)
 [![PyPI](https://img.shields.io/pypi/v/popv.svg)](https://pypi.org/project/popv)
-![Build Status](https://github.com/yoseflab/popv/workflows/popv/badge.svg)
-[![Coverage](https://codecov.io/gh/yoseflab/popv/branch/master/graph/badge.svg)](https://codecov.io/gh/YosefLab/popv)
+[![PopV](https://github.com/YosefLab/PopV/actions/workflows/test.yml/badge.svg)](https://github.com/YosefLab/PopV/actions/workflows/test.yml)
+[![Coverage](https://codecov.io/gh/YosefLab/popv/branch/main/graph/badge.svg?token=KuSsL5q3l7)](https://codecov.io/gh/YosefLab/popv)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![Downloads](https://pepy.tech/badge/popv)](https://pepy.tech/project/popv)
 
 # PopV
 
 PopV uses popular vote of a variety of cell-type transfer tools to classify cell-types in a query dataset based on a test dataset.
 Using this variety of algorithms, we compute the agreement between those algorithms and use this agreement to predict which cell-types are with a high likelihood the same cell-types observed in the reference.
@@ -115,17 +115,15 @@
 
     conda create -n yourenv python=3.8
     conda activate yourenv
     pip install git+https://github.com/czbiohub/PopV
 
 ## Example notebook
 
-We deposited an example notebook in Google Colab:
+We provide an example notebook in Google Colab:
 
 -   [Tutorial demonstrating use of Tabula sapiens as a reference](tabula_sapiens_tutorial.ipynb)
 
 This notebook will guide you through annotating a dataset based on the annotated [Tabula sapiens reference](https://tabula-sapiens-portal.ds.czbiohub.org) and demonstrates how to run annotation on your own query dataset. This notebook requires that all cells are annotated based on a cell ontology. We strongly encourage the use of a common cell ontology, see also [Osumi-Sutherland et al](https://www.nature.com/articles/s41556-021-00787-7). Using a cell ontology is a requirement to run OnClass as a prediction algorithm.
 
-However, for other organisms than human no ontology exists. We therefore allow running PopV without using a cell ontology. A second notebook highlighting using PopV without an existing ontology is currently planned and will be released here.
-
-Memory requirements exceed the free limit in Colab and we recommend a Pro access to run the notebook.
+We allow running PopV without using a cell ontology.
```

