# Comparing `tmp/engawa-0.1.4.tar.gz` & `tmp/engawa-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "engawa-0.1.4.tar", max compression
+gzip compressed data, was "engawa-0.1.5.tar", max compression
```

## Comparing `engawa-0.1.4.tar` & `engawa-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0      703 2023-01-09 18:20:49.237625 engawa-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-01-02 14:17:41.407366 engawa-0.1.4/engawa/__init__.py
--rw-r--r--   0        0        0      221 2023-01-09 18:20:31.363960 engawa-0.1.4/engawa/cli.py
--rw-r--r--   0        0        0     7810 2023-01-03 13:41:40.949180 engawa-0.1.4/engawa/data_collator.py
--rw-r--r--   0        0        0     1555 2023-01-09 16:45:27.520496 engawa-0.1.4/engawa/data_loader.py
--rw-r--r--   0        0        0     1632 2023-01-05 18:32:23.907195 engawa-0.1.4/engawa/misc/did_it_learn_anything.py
--rw-r--r--   0        0        0     3028 2023-01-09 15:36:58.495915 engawa-0.1.4/engawa/model.py
--rw-r--r--   0        0        0     2043 2023-01-09 16:27:22.695337 engawa-0.1.4/engawa/tokenizer.py
--rw-r--r--   0        0        0     4049 2023-01-09 16:28:40.766597 engawa-0.1.4/engawa/train.py
--rw-r--r--   0        0        0      629 2023-01-09 18:21:01.928473 engawa-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1681 1970-01-01 00:00:00.000000 engawa-0.1.4/setup.py
--rw-r--r--   0        0        0     1380 1970-01-01 00:00:00.000000 engawa-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      787 2023-03-28 12:54:29.775929 engawa-0.1.5/README.md
+-rw-r--r--   0        0        0      221 2023-04-12 10:42:17.169919 engawa-0.1.5/engawa/.null-ls_883731_cli.py
+-rw-r--r--   0        0        0     4049 2023-03-28 13:49:48.391129 engawa-0.1.5/engawa/.null-ls_893613_train.py
+-rw-r--r--   0        0        0        0 2023-01-02 14:17:41.407366 engawa-0.1.5/engawa/__init__.py
+-rw-r--r--   0        0        0      175 2023-05-11 09:37:24.419967 engawa-0.1.5/engawa/cli.py
+-rw-r--r--   0        0        0     7810 2023-01-03 13:41:40.949180 engawa-0.1.5/engawa/data_collator.py
+-rw-r--r--   0        0        0     1555 2023-01-09 16:45:27.520496 engawa-0.1.5/engawa/data_loader.py
+-rw-r--r--   0        0        0     1632 2023-01-05 18:32:23.907195 engawa-0.1.5/engawa/misc/did_it_learn_anything.py
+-rw-r--r--   0        0        0     3028 2023-01-09 15:36:58.495915 engawa-0.1.5/engawa/model.py
+-rw-r--r--   0        0        0     1982 2023-05-11 09:22:23.116015 engawa-0.1.5/engawa/tokenizer.py
+-rw-r--r--   0        0        0     3172 2023-05-11 09:37:38.747918 engawa-0.1.5/engawa/train.py
+-rw-r--r--   0        0        0      661 2023-05-11 09:39:04.688700 engawa-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1799 1970-01-01 00:00:00.000000 engawa-0.1.5/setup.py
+-rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 engawa-0.1.5/PKG-INFO
```

### Comparing `engawa-0.1.4/README.md` & `engawa-0.1.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # engawa
 
+<img align="center" src="img/logo.jpg" width="200" height="200" />
+
 **NOT YET FULLY TESTED**
 
 A simple implementation to pre-train BART from scratch with your own corpus.
 
 
 # Usage
 
@@ -23,12 +25,16 @@
 # Checkout other options by
 engawa train-tokenizer --help
 ```
 
 ## Pre-train BART
 
 ```bash
-engawa train-model --tokenizer-file /path/to/tokenizer.json --train-file /path/to/train.txt --val-file /path/to/val.txt --default-root-dir /path/to/save/things
+engawa train-model \
+  --tokenizer-file /path/to/tokenizer.json \
+  --train-file /path/to/train.txt \
+  --val-file /path/to/val.txt \
+  --default-root-dir /path/to/save/things
 
 # Checkout other options by
 engawa train-model --help
 ```
```

### Comparing `engawa-0.1.4/engawa/data_collator.py` & `engawa-0.1.5/engawa/data_collator.py`

 * *Files identical despite different names*

### Comparing `engawa-0.1.4/engawa/data_loader.py` & `engawa-0.1.5/engawa/data_loader.py`

 * *Files identical despite different names*

### Comparing `engawa-0.1.4/engawa/misc/did_it_learn_anything.py` & `engawa-0.1.5/engawa/misc/did_it_learn_anything.py`

 * *Files identical despite different names*

### Comparing `engawa-0.1.4/engawa/model.py` & `engawa-0.1.5/engawa/model.py`

 * *Files identical despite different names*

### Comparing `engawa-0.1.4/engawa/tokenizer.py` & `engawa-0.1.5/engawa/tokenizer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
+from typing import Annotated
 
-import click
+import typer
 from tokenizers import (Tokenizer, decoders, models, pre_tokenizers,
                         processors, trainers)
 
 BOS = "<s>"
 EOS = "</s>"
 UNK = "<unk>"
 PAD = "<pad>"
@@ -26,34 +27,27 @@
                 yield text_batch
                 text_batch = []
                 cnt = 0
             text_batch.append(line)
             cnt += 1
 
 
-@click.command()
-@click.option(
-    "--data-path", type=str, required=True, help="Path to a training text file."
-)
-@click.option(
-    "--save-dir", type=str, required=True, help="Dir to save trianed tokenizer."
-)
-@click.option(
-    "--batch-size",
-    type=int,
-    default=32,
-    help="Batch size for building tokenizer, smaller value for limited resourced situation but takes more time.",
-)
-@click.option(
-    "--vocab-size",
-    type=int,
-    default=50000,
-    help="Number of unique tokens in the vocabulary.",
-)
-def train_tokenizer(data_path: str, save_dir: str, batch_size: int, vocab_size: int):
+def train_tokenizer(
+    data_path: Annotated[str, typer.Option(help="Path to a training text file.")],
+    save_dir: Annotated[str, typer.Option(help="Dir to save trianed tokenizer.")],
+    batch_size: Annotated[
+        int,
+        typer.Option(
+            help="Batch size for building tokenizer, smaller value for limited resourced situation but takes more time."
+        ),
+    ] = 32,
+    vocab_size: Annotated[
+        int, typer.Option(help="Number of unique tokens in the vocabulary.")
+    ] = 50000,
+):
     tokenizer = Tokenizer(models.BPE())
     tokenizer.pre_tokenizer = pre_tokenizers.ByteLevel(add_prefix_space=False)
     tokenizer.decoder = decoders.ByteLevel()
 
     # Set the training hyperparameters
     trainer = trainers.BpeTrainer(
         vocab_size=vocab_size,
```

### Comparing `engawa-0.1.4/engawa/train.py` & `engawa-0.1.5/engawa/.null-ls_893613_train.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 @click.option("--seed", type=int, required=False, default=10)
 @click.option("--bs", type=int, required=False, default=32)
 @click.option("--max-length", type=int, required=False, default=1024)
 @click.option("--lr", type=float, required=False, default=0.0004)
 @click.option("--weight-decay", type=float, required=False, default=0.01)
 @click.option("--num-warmup-steps", type=int, required=False, default=10000)
 @click.option("--mask-ratio", type=float, required=False, default=0.3)
-@click.option("--poisson_lambda", type=float, required=False, default=3.5)
+@click.option("--poisson-lambda", type=float, required=False, default=3.5)
 def train_model(
     tokenizer_file: str,
     train_file: str,
     val_file: str,
     default_root_dir: str,
     ckpt_path: str,
     wandb_proj_name: str,
```

### Comparing `engawa-0.1.4/setup.py` & `engawa-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,24 +12,25 @@
  'datasets>=2.8.0,<3.0.0',
  'nltk>=3.8,<4.0',
  'pytorch-lightning>=1.8.6,<2.0.0',
  'sentencepiece>=0.1.97,<0.2.0',
  'sienna>=0.1.5,<0.2.0',
  'tokenizers>=0.13.2,<0.14.0',
  'transformers>=4.25.1,<5.0.0',
+ 'typer>=0.9.0,<0.10.0',
  'wandb>=0.13.7,<0.14.0']
 
 entry_points = \
-{'console_scripts': ['engawa = engawa.cli:main']}
+{'console_scripts': ['engawa = engawa.cli:app']}
 
 setup_kwargs = {
     'name': 'engawa',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': '',
-    'long_description': '# engawa\n\n**NOT YET FULLY TESTED**\n\nA simple implementation to pre-train BART from scratch with your own corpus.\n\n\n# Usage\n\nSoon, I will make this pip-installable with CLI commands but at the moment, you need to run it as a repository.\n\n## Installation\n\n```bash\npip install engawa\n```\n\n## Build tokenizer\n\n```bash\nengawa train-tokenizer --data-path /path/to/train.txt --save-dir /path/to/save\n\n# Checkout other options by\nengawa train-tokenizer --help\n```\n\n## Pre-train BART\n\n```bash\nengawa train-model --tokenizer-file /path/to/tokenizer.json --train-file /path/to/train.txt --val-file /path/to/val.txt --default-root-dir /path/to/save/things\n\n# Checkout other options by\nengawa train-model --help\n```\n',
+    'long_description': '# engawa\n\n<img align="center" src="img/logo.jpg" width="200" height="200" />\n\n**NOT YET FULLY TESTED**\n\nA simple implementation to pre-train BART from scratch with your own corpus.\n\n\n# Usage\n\nSoon, I will make this pip-installable with CLI commands but at the moment, you need to run it as a repository.\n\n## Installation\n\n```bash\npip install engawa\n```\n\n## Build tokenizer\n\n```bash\nengawa train-tokenizer --data-path /path/to/train.txt --save-dir /path/to/save\n\n# Checkout other options by\nengawa train-tokenizer --help\n```\n\n## Pre-train BART\n\n```bash\nengawa train-model \\\n  --tokenizer-file /path/to/tokenizer.json \\\n  --train-file /path/to/train.txt \\\n  --val-file /path/to/val.txt \\\n  --default-root-dir /path/to/save/things\n\n# Checkout other options by\nengawa train-model --help\n```\n',
     'author': 'sobamchan',
     'author_email': 'oh.sore.sore.soutarou@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `engawa-0.1.4/PKG-INFO` & `engawa-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: engawa
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: sobamchan
 Author-email: oh.sore.sore.soutarou@gmail.com
 Requires-Python: >=3.10.8,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: datasets (>=2.8.0,<3.0.0)
 Requires-Dist: nltk (>=3.8,<4.0)
 Requires-Dist: pytorch-lightning (>=1.8.6,<2.0.0)
 Requires-Dist: sentencepiece (>=0.1.97,<0.2.0)
 Requires-Dist: sienna (>=0.1.5,<0.2.0)
 Requires-Dist: tokenizers (>=0.13.2,<0.14.0)
 Requires-Dist: transformers (>=4.25.1,<5.0.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: wandb (>=0.13.7,<0.14.0)
 Description-Content-Type: text/markdown
 
 # engawa
 
+<img align="center" src="img/logo.jpg" width="200" height="200" />
+
 **NOT YET FULLY TESTED**
 
 A simple implementation to pre-train BART from scratch with your own corpus.
 
 
 # Usage
 
@@ -43,13 +46,17 @@
 # Checkout other options by
 engawa train-tokenizer --help
 ```
 
 ## Pre-train BART
 
 ```bash
-engawa train-model --tokenizer-file /path/to/tokenizer.json --train-file /path/to/train.txt --val-file /path/to/val.txt --default-root-dir /path/to/save/things
+engawa train-model \
+  --tokenizer-file /path/to/tokenizer.json \
+  --train-file /path/to/train.txt \
+  --val-file /path/to/val.txt \
+  --default-root-dir /path/to/save/things
 
 # Checkout other options by
 engawa train-model --help
 ```
```

