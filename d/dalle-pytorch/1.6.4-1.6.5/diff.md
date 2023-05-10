# Comparing `tmp/dalle-pytorch-1.6.4.tar.gz` & `tmp/dalle-pytorch-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalle-pytorch-1.6.4.tar", last modified: Mon May 30 18:46:04 2022, max compression
+gzip compressed data, was "dalle-pytorch-1.6.5.tar", last modified: Wed May 10 22:57:23 2023, max compression
```

## Comparing `dalle-pytorch-1.6.4.tar` & `dalle-pytorch-1.6.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 18:46:04.419845 dalle-pytorch-1.6.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-05-30 18:45:54.000000 dalle-pytorch-1.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-30 18:45:54.000000 dalle-pytorch-1.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-05-30 18:46:04.419845 dalle-pytorch-1.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    27842 2022-05-30 18:45:54.000000 dalle-pytorch-1.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 18:46:04.415845 dalle-pytorch-1.6.4/dalle_pytorch/
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-05-30 18:45:54.000000 dalle-pytorch-1.6.4/dalle_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14131 2022-05-30 18:45:54.000000 dalle-pytorch-1.6.4/dalle_pytorch/attention.py
--rw-r--r--   0 runner    (1001) docker     (121)    23073 2022-05-30 18:45:54.000000 dalle-pytorch-1.6.4/dalle_pytorch/dalle_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 18:46:04.415845 dalle-pytorch-1.6.4/dalle_pytorch/data/
--rw-r--r--   0 runner    (1001) docker     (121)  3194984 2022-05-30 18:45:54.000000 dalle-pytorch-1.6.4/dalle_pytorch/data/bpe_simple_vocab_16e6.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 18:46:04.419845 dalle-pytorch-1.6.4/dalle_pytorch/distributed_backends/
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-05-30 18:45:54.000000 dalle-pytorch-1.6.4/dalle_pytorch/distributed_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5987 2022-05-30 18:45:54.000000 dalle-pytorch-1.6.4/dalle_pytorch/distributed_backends/deepspeed_backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     5671 2022-05-30 18:45:54.000000 dalle-pytorch-1.6.4/dalle_pytorch/distributed_backends/distributed_backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     1222 2022-05-30 18:45:54.000000 dalle-pytorch-1.6.4/dalle_pytorch/distributed_backends/dummy_backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     1703 2022-05-30 18:45:54.000000 dalle-pytorch-1.6.4/dalle_pytorch/distributed_backends/horovod_backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     2839 2022-05-30 18:45:54.000000 dalle-pytorch-1.6.4/dalle_pytorch/distributed_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3558 2022-05-30 18:45:54.000000 dalle-pytorch-1.6.4/dalle_pytorch/loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     5390 2022-05-30 18:45:54.000000 dalle-pytorch-1.6.4/dalle_pytorch/reversible.py
--rw-r--r--   0 runner    (1001) docker     (121)     9436 2022-05-30 18:45:54.000000 dalle-pytorch-1.6.4/dalle_pytorch/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)    13131 2022-05-30 18:45:54.000000 dalle-pytorch-1.6.4/dalle_pytorch/transformer.py
--rw-r--r--   0 runner    (1001) docker     (121)     7674 2022-05-30 18:45:54.000000 dalle-pytorch-1.6.4/dalle_pytorch/vae.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-30 18:45:54.000000 dalle-pytorch-1.6.4/dalle_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-30 18:46:04.415845 dalle-pytorch-1.6.4/dalle_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-05-30 18:46:04.000000 dalle-pytorch-1.6.4/dalle_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      807 2022-05-30 18:46:04.000000 dalle-pytorch-1.6.4/dalle_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-30 18:46:04.000000 dalle-pytorch-1.6.4/dalle_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-05-30 18:46:04.000000 dalle-pytorch-1.6.4/dalle_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-05-30 18:46:04.000000 dalle-pytorch-1.6.4/dalle_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-30 18:46:04.419845 dalle-pytorch-1.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1149 2022-05-30 18:45:54.000000 dalle-pytorch-1.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:57:23.613964 dalle-pytorch-1.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-10 22:57:14.000000 dalle-pytorch-1.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 22:57:14.000000 dalle-pytorch-1.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-10 22:57:23.613964 dalle-pytorch-1.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28137 2023-05-10 22:57:14.000000 dalle-pytorch-1.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:57:23.609964 dalle-pytorch-1.6.5/dalle_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-10 22:57:14.000000 dalle-pytorch-1.6.5/dalle_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14131 2023-05-10 22:57:14.000000 dalle-pytorch-1.6.5/dalle_pytorch/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23607 2023-05-10 22:57:14.000000 dalle-pytorch-1.6.5/dalle_pytorch/dalle_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:57:23.609964 dalle-pytorch-1.6.5/dalle_pytorch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  3194984 2023-05-10 22:57:14.000000 dalle-pytorch-1.6.5/dalle_pytorch/data/bpe_simple_vocab_16e6.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:57:23.613964 dalle-pytorch-1.6.5/dalle_pytorch/distributed_backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-10 22:57:14.000000 dalle-pytorch-1.6.5/dalle_pytorch/distributed_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-10 22:57:14.000000 dalle-pytorch-1.6.5/dalle_pytorch/distributed_backends/deepspeed_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-10 22:57:14.000000 dalle-pytorch-1.6.5/dalle_pytorch/distributed_backends/distributed_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-10 22:57:14.000000 dalle-pytorch-1.6.5/dalle_pytorch/distributed_backends/dummy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-10 22:57:14.000000 dalle-pytorch-1.6.5/dalle_pytorch/distributed_backends/horovod_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-10 22:57:14.000000 dalle-pytorch-1.6.5/dalle_pytorch/distributed_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-10 22:57:14.000000 dalle-pytorch-1.6.5/dalle_pytorch/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-05-10 22:57:14.000000 dalle-pytorch-1.6.5/dalle_pytorch/reversible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9436 2023-05-10 22:57:14.000000 dalle-pytorch-1.6.5/dalle_pytorch/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13131 2023-05-10 22:57:14.000000 dalle-pytorch-1.6.5/dalle_pytorch/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-05-10 22:57:14.000000 dalle-pytorch-1.6.5/dalle_pytorch/vae.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 22:57:14.000000 dalle-pytorch-1.6.5/dalle_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:57:23.609964 dalle-pytorch-1.6.5/dalle_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-10 22:57:23.000000 dalle-pytorch-1.6.5/dalle_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-10 22:57:23.000000 dalle-pytorch-1.6.5/dalle_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 22:57:23.000000 dalle-pytorch-1.6.5/dalle_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-10 22:57:23.000000 dalle-pytorch-1.6.5/dalle_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-10 22:57:23.000000 dalle-pytorch-1.6.5/dalle_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 22:57:23.613964 dalle-pytorch-1.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-10 22:57:14.000000 dalle-pytorch-1.6.5/setup.py
```

### Comparing `dalle-pytorch-1.6.4/LICENSE` & `dalle-pytorch-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dalle-pytorch-1.6.4/PKG-INFO` & `dalle-pytorch-1.6.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: dalle-pytorch
-Version: 1.6.4
+Version: 1.6.5
 Summary: DALL-E - Pytorch
 Home-page: https://github.com/lucidrains/dalle-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers,text-to-image
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `dalle-pytorch-1.6.4/README.md` & `dalle-pytorch-1.6.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -747,8 +747,18 @@
 ```bibtex
 @misc{crowson2022,
     author  = {Katherine Crowson},
     url     = {https://twitter.com/RiversHaveWings/status/1478093658716966912}
 }
 ```
 
+```bibtex
+@article{Liu2023BridgingDA,
+    title   = {Bridging Discrete and Backpropagation: Straight-Through and Beyond},
+    author  = {Liyuan Liu and Chengyu Dong and Xiaodong Liu and Bin Yu and Jianfeng Gao},
+    journal = {ArXiv},
+    year    = {2023},
+    volume  = {abs/2304.08612}
+}
+```
+
 *Those who do not want to imitate anything, produce nothing.* - Dali
```

#### html2text {}

```diff
@@ -304,9 +304,12 @@
 Pan and Bo Wen and Yunfeng Liu}, year = {2021}, eprint = {2104.09864},
 archivePrefix = {arXiv}, primaryClass = {cs.CL} } ``` ```bibtex @inproceedings
 {ho2021classifierfree, title = {Classifier-Free Diffusion Guidance}, author =
 {Jonathan Ho and Tim Salimans}, booktitle = {NeurIPS 2021 Workshop on Deep
 Generative Models and Downstream Applications}, year = {2021}, url = {https://
 openreview.net/forum?id=qw8AKxfYbI} } ``` ```bibtex @misc{crowson2022, author =
 {Katherine Crowson}, url = {https://twitter.com/RiversHaveWings/status/
-1478093658716966912} } ``` *Those who do not want to imitate anything, produce
-nothing.* - Dali
+1478093658716966912} } ``` ```bibtex @article{Liu2023BridgingDA, title =
+{Bridging Discrete and Backpropagation: Straight-Through and Beyond}, author =
+{Liyuan Liu and Chengyu Dong and Xiaodong Liu and Bin Yu and Jianfeng Gao},
+journal = {ArXiv}, year = {2023}, volume = {abs/2304.08612} } ``` *Those who do
+not want to imitate anything, produce nothing.* - Dali
```

### Comparing `dalle-pytorch-1.6.4/dalle_pytorch/attention.py` & `dalle-pytorch-1.6.5/dalle_pytorch/attention.py`

 * *Files identical despite different names*

### Comparing `dalle-pytorch-1.6.4/dalle_pytorch/dalle_pytorch.py` & `dalle-pytorch-1.6.5/dalle_pytorch/dalle_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,28 +107,31 @@
         num_layers = 3,
         num_resnet_blocks = 0,
         hidden_dim = 64,
         channels = 3,
         smooth_l1_loss = False,
         temperature = 0.9,
         straight_through = False,
+        reinmax = False,
         kl_div_loss_weight = 0.,
         normalization = ((*((0.5,) * 3), 0), (*((0.5,) * 3), 1))
     ):
         super().__init__()
         assert log2(image_size).is_integer(), 'image size must be a power of 2'
         assert num_layers >= 1, 'number of layers must be greater than or equal to 1'
         has_resblocks = num_resnet_blocks > 0
 
         self.channels = channels
         self.image_size = image_size
         self.num_tokens = num_tokens
         self.num_layers = num_layers
         self.temperature = temperature
         self.straight_through = straight_through
+        self.reinmax = reinmax
+
         self.codebook = nn.Embedding(num_tokens, codebook_dim)
 
         hdim = hidden_dim
 
         enc_chans = [hidden_dim] * num_layers
         dec_chans = list(reversed(enc_chans))
 
@@ -223,16 +226,28 @@
 
         logits = self.encoder(img)
 
         if return_logits:
             return logits # return logits for getting hard image indices for DALL-E training
 
         temp = default(temp, self.temperature)
-        soft_one_hot = F.gumbel_softmax(logits, tau = temp, dim = 1, hard = self.straight_through)
-        sampled = einsum('b n h w, n d -> b d h w', soft_one_hot, self.codebook.weight)
+
+        one_hot = F.gumbel_softmax(logits, tau = temp, dim = 1, hard = self.straight_through)
+
+        if self.straight_through and self.reinmax:
+            # use reinmax for better second-order accuracy - https://arxiv.org/abs/2304.08612
+            # algorithm 2
+            one_hot = one_hot.detach()
+            π0 = logits.softmax(dim = 1)
+            π1 = (one_hot + (logits / temp).softmax(dim = 1)) / 2
+            π1 = ((π1.log() - logits).detach() + logits).softmax(dim = 1)
+            π2 = 2 * π1 - 0.5 * π0
+            one_hot = π2 - π2.detach() + one_hot
+
+        sampled = einsum('b n h w, n d -> b d h w', one_hot, self.codebook.weight)
         out = self.decoder(sampled)
 
         if not return_loss:
             return out
 
         # reconstruction loss
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dalle-pytorch-1.6.4/dalle_pytorch/data/bpe_simple_vocab_16e6.txt` & `dalle-pytorch-1.6.5/dalle_pytorch/data/bpe_simple_vocab_16e6.txt`

 * *Files identical despite different names*

### Comparing `dalle-pytorch-1.6.4/dalle_pytorch/distributed_backends/deepspeed_backend.py` & `dalle-pytorch-1.6.5/dalle_pytorch/distributed_backends/deepspeed_backend.py`

 * *Files identical despite different names*

### Comparing `dalle-pytorch-1.6.4/dalle_pytorch/distributed_backends/distributed_backend.py` & `dalle-pytorch-1.6.5/dalle_pytorch/distributed_backends/distributed_backend.py`

 * *Files identical despite different names*

### Comparing `dalle-pytorch-1.6.4/dalle_pytorch/distributed_backends/dummy_backend.py` & `dalle-pytorch-1.6.5/dalle_pytorch/distributed_backends/dummy_backend.py`

 * *Files identical despite different names*

### Comparing `dalle-pytorch-1.6.4/dalle_pytorch/distributed_backends/horovod_backend.py` & `dalle-pytorch-1.6.5/dalle_pytorch/distributed_backends/horovod_backend.py`

 * *Files identical despite different names*

### Comparing `dalle-pytorch-1.6.4/dalle_pytorch/distributed_utils.py` & `dalle-pytorch-1.6.5/dalle_pytorch/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `dalle-pytorch-1.6.4/dalle_pytorch/loader.py` & `dalle-pytorch-1.6.5/dalle_pytorch/loader.py`

 * *Files identical despite different names*

### Comparing `dalle-pytorch-1.6.4/dalle_pytorch/reversible.py` & `dalle-pytorch-1.6.5/dalle_pytorch/reversible.py`

 * *Files identical despite different names*

### Comparing `dalle-pytorch-1.6.4/dalle_pytorch/tokenizer.py` & `dalle-pytorch-1.6.5/dalle_pytorch/tokenizer.py`

 * *Files identical despite different names*

### Comparing `dalle-pytorch-1.6.4/dalle_pytorch/transformer.py` & `dalle-pytorch-1.6.5/dalle_pytorch/transformer.py`

 * *Files identical despite different names*

### Comparing `dalle-pytorch-1.6.4/dalle_pytorch/vae.py` & `dalle-pytorch-1.6.5/dalle_pytorch/vae.py`

 * *Files identical despite different names*

### Comparing `dalle-pytorch-1.6.4/dalle_pytorch.egg-info/PKG-INFO` & `dalle-pytorch-1.6.5/dalle_pytorch.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: dalle-pytorch
-Version: 1.6.4
+Version: 1.6.5
 Summary: DALL-E - Pytorch
 Home-page: https://github.com/lucidrains/dalle-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers,text-to-image
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `dalle-pytorch-1.6.4/dalle_pytorch.egg-info/SOURCES.txt` & `dalle-pytorch-1.6.5/dalle_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dalle-pytorch-1.6.4/setup.py` & `dalle-pytorch-1.6.5/setup.py`

 * *Files identical despite different names*

