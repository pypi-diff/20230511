# Comparing `tmp/addict-tracking-changes-0.1.1.tar.gz` & `tmp/addict-tracking-changes-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "addict-tracking-changes-0.1.1.tar", last modified: Tue Feb 28 06:29:34 2023, max compression
+gzip compressed data, was "addict-tracking-changes-1.0.0.tar", last modified: Thu May 11 10:04:20 2023, max compression
```

## Comparing `addict-tracking-changes-0.1.1.tar` & `addict-tracking-changes-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,33 @@
--rw-r--r--   0        0        0     1836 2023-02-28 06:28:18.757491 addict-tracking-changes-0.1.1/.gitignore
--rw-r--r--   0        0        0     1070 2022-11-29 03:20:21.000000 addict-tracking-changes-0.1.1/LICENSE
--rw-r--r--   0        0        0      282 2023-02-28 06:21:14.531735 addict-tracking-changes-0.1.1/Pipfile
--rw-r--r--   0        0        0    35082 2023-02-28 06:23:40.850259 addict-tracking-changes-0.1.1/Pipfile.lock
--rw-r--r--   0        0        0     3829 2022-12-03 13:38:01.000000 addict-tracking-changes-0.1.1/README.md
--rw-r--r--   0        0        0     3726 2022-12-03 13:37:34.000000 addict-tracking-changes-0.1.1/docs/README.md
--rw-r--r--   0        0        0     1430 2022-12-02 18:42:15.000000 addict-tracking-changes-0.1.1/docs/main_doc.md
--rw-r--r--   0        0        0      408 2022-12-03 11:14:35.000000 addict-tracking-changes-0.1.1/mkdocs.yml
--rw-r--r--   0        0        0      723 2023-02-28 03:47:56.458718 addict-tracking-changes-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      201 2023-02-28 06:29:30.406773 addict-tracking-changes-0.1.1/src/addict_tracking_changes/__init__.py
--rw-r--r--   0        0        0     9197 2022-12-03 11:14:35.000000 addict-tracking-changes-0.1.1/src/addict_tracking_changes/addict.py
--rw-r--r--   0        0        0     6481 2023-01-14 18:17:02.578076 addict-tracking-changes-0.1.1/tests/addict_test.py
--rw-r--r--   0        0        0     4331 1970-01-01 00:00:00.000000 addict-tracking-changes-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      141 2023-05-11 09:44:16.829627 addict-tracking-changes-1.0.0/.flake8
+-rw-r--r--   0        0        0     1886 2023-05-11 09:44:16.829627 addict-tracking-changes-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1070 2022-11-29 03:20:21.000000 addict-tracking-changes-1.0.0/LICENSE
+-rw-r--r--   0        0        0      325 2023-05-11 09:44:16.859627 addict-tracking-changes-1.0.0/Pipfile
+-rw-r--r--   0        0        0    41152 2023-05-11 09:44:16.859627 addict-tracking-changes-1.0.0/Pipfile.lock
+-rw-r--r--   0        0        0     5078 2023-05-11 09:44:16.809627 addict-tracking-changes-1.0.0/README.md
+-rw-r--r--   0        0        0     1146 2023-05-11 09:44:16.859627 addict-tracking-changes-1.0.0/badge_coverage.svg
+-rw-r--r--   0        0        0     1177 2023-05-11 09:44:16.859627 addict-tracking-changes-1.0.0/badge_flake8.svg
+-rw-r--r--   0        0        0     1115 2023-05-11 09:44:16.859627 addict-tracking-changes-1.0.0/badge_tests.svg
+-rw-r--r--   0        0        0      634 2023-05-11 09:44:16.829627 addict-tracking-changes-1.0.0/docs/Makefile
+-rw-r--r--   0        0        0     5873 2023-05-11 09:44:16.839627 addict-tracking-changes-1.0.0/docs/addict.rst
+-rw-r--r--   0        0        0     1950 2023-05-11 09:44:16.829627 addict-tracking-changes-1.0.0/docs/conf.py
+-rw-r--r--   0        0        0      503 2023-05-11 09:44:16.829627 addict-tracking-changes-1.0.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-05-11 09:44:16.829627 addict-tracking-changes-1.0.0/docs/make.bat
+-rw-r--r--   0        0        0     1116 2023-05-11 09:44:16.829627 addict-tracking-changes-1.0.0/docs/usage.rst
+-rw-r--r--   0        0        0      408 2023-05-11 09:44:16.789627 addict-tracking-changes-1.0.0/mkdocs.yml
+-rw-r--r--   0        0        0     3544 2023-05-11 09:44:16.859627 addict-tracking-changes-1.0.0/noxfile.py
+-rw-r--r--   0        0        0      723 2023-05-11 09:44:16.799627 addict-tracking-changes-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2245 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.0/reports/flake8/back.svg
+-rw-r--r--   0        0        0     2666 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.0/reports/flake8/file.svg
+-rw-r--r--   0        0        0     7400 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.0/reports/flake8/flake8stats.txt
+-rw-r--r--   0        0        0     1109 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.0/reports/flake8/index.html
+-rw-r--r--   0        0        0     3669 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.0/reports/flake8/src.addict_tracking_changes.__init__.report.html
+-rw-r--r--   0        0        0     8223 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.0/reports/flake8/src.addict_tracking_changes.__init__.source.html
+-rw-r--r--   0        0        0     2999 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.0/reports/flake8/src.addict_tracking_changes.addict.report.html
+-rw-r--r--   0        0        0    89377 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.0/reports/flake8/src.addict_tracking_changes.addict.source.html
+-rw-r--r--   0        0        0     7273 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.0/reports/flake8/styles.css
+-rw-r--r--   0        0        0     4565 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.0/reports/junit/junit.xml
+-rw-r--r--   0        0        0     1471 2023-05-11 09:44:16.849627 addict-tracking-changes-1.0.0/src/addict_tracking_changes/__init__.py
+-rw-r--r--   0        0        0    13290 2023-05-11 09:44:16.849627 addict-tracking-changes-1.0.0/src/addict_tracking_changes/addict.py
+-rw-r--r--   0        0        0     1115 2023-05-11 09:44:16.869627 addict-tracking-changes-1.0.0/tests-badge.svg
+-rw-r--r--   0        0        0    14497 2023-05-11 09:44:16.849627 addict-tracking-changes-1.0.0/tests/addict_test.py
+-rw-r--r--   0        0        0     5580 1970-01-01 00:00:00.000000 addict-tracking-changes-1.0.0/PKG-INFO
```

### Comparing `addict-tracking-changes-0.1.1/.gitignore` & `addict-tracking-changes-1.0.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# emacs
+*.*~
+*~
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
@@ -67,14 +71,18 @@
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
 docs/_build/
+docs/_templates/
+docs/_static/
+
+
 
 # PyBuilder
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
```

### Comparing `addict-tracking-changes-0.1.1/LICENSE` & `addict-tracking-changes-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-0.1.1/Pipfile.lock` & `addict-tracking-changes-1.0.0/Pipfile.lock`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.690372085048011%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'d95420feb7d28652f8e93d836dd0af58b65e5caeb675c7a1de8f97f0ef7876ef'}}",*

 * * "'default'": "{replace: OrderedDict([('dpath', OrderedDict([('hashes', "*

 * *              "['sha256:559edcbfc806ca2f9ad9e63566f22e5d41c000e4215bbce9dbf1ca4c859f5e0b', "*

 * *              "'sha256:ccd964db839baad4aa820612b4b8731b09f40a245d401b723156ce4ef45b22b7']), "*

 * *              "('index', 'pypi'), ('version', '==2.1.5')]))])}",*

 * * "'develop'": "{'black': {'hashes': "*

 * *              "['sha256:06410 […]*

```diff
@@ -1,284 +1,278 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "0175c35291fc34d7d7c5c10ed5fa23059f5f3b4b65ab7795aa0c9d0d3204990e"
+            "sha256": "d95420feb7d28652f8e93d836dd0af58b65e5caeb675c7a1de8f97f0ef7876ef"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.11"
         },
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
         ]
     },
     "default": {
-        "addict-tracking-changes": {
-            "editable": true,
-            "path": "."
+        "dpath": {
+            "hashes": [
+                "sha256:559edcbfc806ca2f9ad9e63566f22e5d41c000e4215bbce9dbf1ca4c859f5e0b",
+                "sha256:ccd964db839baad4aa820612b4b8731b09f40a245d401b723156ce4ef45b22b7"
+            ],
+            "index": "pypi",
+            "version": "==2.1.5"
         }
     },
     "develop": {
-        "anyio": {
+        "alabaster": {
             "hashes": [
-                "sha256:25ea0d673ae30af41a0c442f81cf3b38c7e79fdc7b60335a4c14e05eb0947421",
-                "sha256:fbbe32bd270d2a2ef3ed1c5d45041250284e31fc0a4df4a5a6071842051a51e3"
+                "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
+                "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
             ],
-            "markers": "python_full_version >= '3.6.2'",
-            "version": "==3.6.2"
+            "markers": "python_version >= '3.6'",
+            "version": "==0.7.13"
         },
-        "attrs": {
+        "argcomplete": {
             "hashes": [
-                "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836",
-                "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"
+                "sha256:b9ca96448e14fa459d7450a4ab5a22bbf9cee4ba7adddf03e65c398b5daeea28",
+                "sha256:e36fd646839933cbec7941c662ecb65338248667358dd3d968405a4506a60d9b"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==22.2.0"
+            "version": "==3.0.8"
+        },
+        "babel": {
+            "hashes": [
+                "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
+                "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==2.12.1"
+        },
+        "beautifulsoup4": {
+            "hashes": [
+                "sha256:492bbc69dca35d12daac71c4db1bfff0c876c00ef4a2ffacce226d4638eb72da",
+                "sha256:bd2520ca0d9d7d12694a53d44ac482d181b4ec1888909b035a3dbf40d0f57d4a"
+            ],
+            "markers": "python_full_version >= '3.6.0'",
+            "version": "==4.12.2"
         },
         "black": {
             "hashes": [
-                "sha256:0052dba51dec07ed029ed61b18183942043e00008ec65d5028814afaab9a22fd",
-                "sha256:0680d4380db3719ebcfb2613f34e86c8e6d15ffeabcf8ec59355c5e7b85bb555",
-                "sha256:121ca7f10b4a01fd99951234abdbd97728e1240be89fde18480ffac16503d481",
-                "sha256:162e37d49e93bd6eb6f1afc3e17a3d23a823042530c37c3c42eeeaf026f38468",
-                "sha256:2a951cc83ab535d248c89f300eccbd625e80ab880fbcfb5ac8afb5f01a258ac9",
-                "sha256:2bf649fda611c8550ca9d7592b69f0637218c2369b7744694c5e4902873b2f3a",
-                "sha256:382998821f58e5c8238d3166c492139573325287820963d2f7de4d518bd76958",
-                "sha256:49f7b39e30f326a34b5c9a4213213a6b221d7ae9d58ec70df1c4a307cf2a1580",
-                "sha256:57c18c5165c1dbe291d5306e53fb3988122890e57bd9b3dcb75f967f13411a26",
-                "sha256:7a0f701d314cfa0896b9001df70a530eb2472babb76086344e688829efd97d32",
-                "sha256:8178318cb74f98bc571eef19068f6ab5613b3e59d4f47771582f04e175570ed8",
-                "sha256:8b70eb40a78dfac24842458476135f9b99ab952dd3f2dab738c1881a9b38b753",
-                "sha256:9880d7d419bb7e709b37e28deb5e68a49227713b623c72b2b931028ea65f619b",
-                "sha256:9afd3f493666a0cd8f8df9a0200c6359ac53940cbde049dcb1a7eb6ee2dd7074",
-                "sha256:a29650759a6a0944e7cca036674655c2f0f63806ddecc45ed40b7b8aa314b651",
-                "sha256:a436e7881d33acaf2536c46a454bb964a50eff59b21b51c6ccf5a40601fbef24",
-                "sha256:a59db0a2094d2259c554676403fa2fac3473ccf1354c1c63eccf7ae65aac8ab6",
-                "sha256:a8471939da5e824b891b25751955be52ee7f8a30a916d570a5ba8e0f2eb2ecad",
-                "sha256:b0bd97bea8903f5a2ba7219257a44e3f1f9d00073d6cc1add68f0beec69692ac",
-                "sha256:b6a92a41ee34b883b359998f0c8e6eb8e99803aa8bf3123bf2b2e6fec505a221",
-                "sha256:bb460c8561c8c1bec7824ecbc3ce085eb50005883a6203dcfb0122e95797ee06",
-                "sha256:bfffba28dc52a58f04492181392ee380e95262af14ee01d4bc7bb1b1c6ca8d27",
-                "sha256:c1c476bc7b7d021321e7d93dc2cbd78ce103b84d5a4cf97ed535fbc0d6660648",
-                "sha256:c91dfc2c2a4e50df0026f88d2215e166616e0c80e86004d0003ece0488db2739",
-                "sha256:e6663f91b6feca5d06f2ccd49a10f254f9298cc1f7f49c46e498a0771b507104"
+                "sha256:064101748afa12ad2291c2b91c960be28b817c0c7eaa35bec09cc63aa56493c5",
+                "sha256:0945e13506be58bf7db93ee5853243eb368ace1c08a24c65ce108986eac65915",
+                "sha256:11c410f71b876f961d1de77b9699ad19f939094c3a677323f43d7a29855fe326",
+                "sha256:1c7b8d606e728a41ea1ccbd7264677e494e87cf630e399262ced92d4a8dac940",
+                "sha256:1d06691f1eb8de91cd1b322f21e3bfc9efe0c7ca1f0e1eb1db44ea367dff656b",
+                "sha256:3238f2aacf827d18d26db07524e44741233ae09a584273aa059066d644ca7b30",
+                "sha256:32daa9783106c28815d05b724238e30718f34155653d4d6e125dc7daec8e260c",
+                "sha256:35d1381d7a22cc5b2be2f72c7dfdae4072a3336060635718cc7e1ede24221d6c",
+                "sha256:3a150542a204124ed00683f0db1f5cf1c2aaaa9cc3495b7a3b5976fb136090ab",
+                "sha256:48f9d345675bb7fbc3dd85821b12487e1b9a75242028adad0333ce36ed2a6d27",
+                "sha256:50cb33cac881766a5cd9913e10ff75b1e8eb71babf4c7104f2e9c52da1fb7de2",
+                "sha256:562bd3a70495facf56814293149e51aa1be9931567474993c7942ff7d3533961",
+                "sha256:67de8d0c209eb5b330cce2469503de11bca4085880d62f1628bd9972cc3366b9",
+                "sha256:6b39abdfb402002b8a7d030ccc85cf5afff64ee90fa4c5aebc531e3ad0175ddb",
+                "sha256:6f3c333ea1dd6771b2d3777482429864f8e258899f6ff05826c3a4fcc5ce3f70",
+                "sha256:714290490c18fb0126baa0fca0a54ee795f7502b44177e1ce7624ba1c00f2331",
+                "sha256:7c3eb7cea23904399866c55826b31c1f55bbcd3890ce22ff70466b907b6775c2",
+                "sha256:92c543f6854c28a3c7f39f4d9b7694f9a6eb9d3c5e2ece488c327b6e7ea9b266",
+                "sha256:a6f6886c9869d4daae2d1715ce34a19bbc4b95006d20ed785ca00fa03cba312d",
+                "sha256:a8a968125d0a6a404842fa1bf0b349a568634f856aa08ffaff40ae0dfa52e7c6",
+                "sha256:c7ab5790333c448903c4b721b59c0d80b11fe5e9803d8703e84dcb8da56fec1b",
+                "sha256:e114420bf26b90d4b9daa597351337762b63039752bdf72bf361364c1aa05925",
+                "sha256:e198cf27888ad6f4ff331ca1c48ffc038848ea9f031a3b40ba36aced7e22f2c8",
+                "sha256:ec751418022185b0c1bb7d7736e6933d40bbb14c14a0abcf9123d1b159f98dd4",
+                "sha256:f0bd2f4a58d6666500542b26354978218a9babcdc972722f4bf90779524515f3"
             ],
             "index": "pypi",
-            "version": "==23.1.0"
+            "version": "==23.3.0"
         },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
-        "cffi": {
+        "charset-normalizer": {
             "hashes": [
-                "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
-                "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
-                "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
-                "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
-                "sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405",
-                "sha256:198caafb44239b60e252492445da556afafc7d1e3ab7a1fb3f0584ef6d742375",
-                "sha256:1e74c6b51a9ed6589199c787bf5f9875612ca4a8a0785fb2d4a84429badaf22a",
-                "sha256:2012c72d854c2d03e45d06ae57f40d78e5770d252f195b93f581acf3ba44496e",
-                "sha256:21157295583fe8943475029ed5abdcf71eb3911894724e360acff1d61c1d54bc",
-                "sha256:2470043b93ff09bf8fb1d46d1cb756ce6132c54826661a32d4e4d132e1977adf",
-                "sha256:285d29981935eb726a4399badae8f0ffdff4f5050eaa6d0cfc3f64b857b77185",
-                "sha256:30d78fbc8ebf9c92c9b7823ee18eb92f2e6ef79b45ac84db507f52fbe3ec4497",
-                "sha256:320dab6e7cb2eacdf0e658569d2575c4dad258c0fcc794f46215e1e39f90f2c3",
-                "sha256:33ab79603146aace82c2427da5ca6e58f2b3f2fb5da893ceac0c42218a40be35",
-                "sha256:3548db281cd7d2561c9ad9984681c95f7b0e38881201e157833a2342c30d5e8c",
-                "sha256:3799aecf2e17cf585d977b780ce79ff0dc9b78d799fc694221ce814c2c19db83",
-                "sha256:39d39875251ca8f612b6f33e6b1195af86d1b3e60086068be9cc053aa4376e21",
-                "sha256:3b926aa83d1edb5aa5b427b4053dc420ec295a08e40911296b9eb1b6170f6cca",
-                "sha256:3bcde07039e586f91b45c88f8583ea7cf7a0770df3a1649627bf598332cb6984",
-                "sha256:3d08afd128ddaa624a48cf2b859afef385b720bb4b43df214f85616922e6a5ac",
-                "sha256:3eb6971dcff08619f8d91607cfc726518b6fa2a9eba42856be181c6d0d9515fd",
-                "sha256:40f4774f5a9d4f5e344f31a32b5096977b5d48560c5592e2f3d2c4374bd543ee",
-                "sha256:4289fc34b2f5316fbb762d75362931e351941fa95fa18789191b33fc4cf9504a",
-                "sha256:470c103ae716238bbe698d67ad020e1db9d9dba34fa5a899b5e21577e6d52ed2",
-                "sha256:4f2c9f67e9821cad2e5f480bc8d83b8742896f1242dba247911072d4fa94c192",
-                "sha256:50a74364d85fd319352182ef59c5c790484a336f6db772c1a9231f1c3ed0cbd7",
-                "sha256:54a2db7b78338edd780e7ef7f9f6c442500fb0d41a5a4ea24fff1c929d5af585",
-                "sha256:5635bd9cb9731e6d4a1132a498dd34f764034a8ce60cef4f5319c0541159392f",
-                "sha256:59c0b02d0a6c384d453fece7566d1c7e6b7bae4fc5874ef2ef46d56776d61c9e",
-                "sha256:5d598b938678ebf3c67377cdd45e09d431369c3b1a5b331058c338e201f12b27",
-                "sha256:5df2768244d19ab7f60546d0c7c63ce1581f7af8b5de3eb3004b9b6fc8a9f84b",
-                "sha256:5ef34d190326c3b1f822a5b7a45f6c4535e2f47ed06fec77d3d799c450b2651e",
-                "sha256:6975a3fac6bc83c4a65c9f9fcab9e47019a11d3d2cf7f3c0d03431bf145a941e",
-                "sha256:6c9a799e985904922a4d207a94eae35c78ebae90e128f0c4e521ce339396be9d",
-                "sha256:70df4e3b545a17496c9b3f41f5115e69a4f2e77e94e1d2a8e1070bc0c38c8a3c",
-                "sha256:7473e861101c9e72452f9bf8acb984947aa1661a7704553a9f6e4baa5ba64415",
-                "sha256:8102eaf27e1e448db915d08afa8b41d6c7ca7a04b7d73af6514df10a3e74bd82",
-                "sha256:87c450779d0914f2861b8526e035c5e6da0a3199d8f1add1a665e1cbc6fc6d02",
-                "sha256:8b7ee99e510d7b66cdb6c593f21c043c248537a32e0bedf02e01e9553a172314",
-                "sha256:91fc98adde3d7881af9b59ed0294046f3806221863722ba7d8d120c575314325",
-                "sha256:94411f22c3985acaec6f83c6df553f2dbe17b698cc7f8ae751ff2237d96b9e3c",
-                "sha256:98d85c6a2bef81588d9227dde12db8a7f47f639f4a17c9ae08e773aa9c697bf3",
-                "sha256:9ad5db27f9cabae298d151c85cf2bad1d359a1b9c686a275df03385758e2f914",
-                "sha256:a0b71b1b8fbf2b96e41c4d990244165e2c9be83d54962a9a1d118fd8657d2045",
-                "sha256:a0f100c8912c114ff53e1202d0078b425bee3649ae34d7b070e9697f93c5d52d",
-                "sha256:a591fe9e525846e4d154205572a029f653ada1a78b93697f3b5a8f1f2bc055b9",
-                "sha256:a5c84c68147988265e60416b57fc83425a78058853509c1b0629c180094904a5",
-                "sha256:a66d3508133af6e8548451b25058d5812812ec3798c886bf38ed24a98216fab2",
-                "sha256:a8c4917bd7ad33e8eb21e9a5bbba979b49d9a97acb3a803092cbc1133e20343c",
-                "sha256:b3bbeb01c2b273cca1e1e0c5df57f12dce9a4dd331b4fa1635b8bec26350bde3",
-                "sha256:cba9d6b9a7d64d4bd46167096fc9d2f835e25d7e4c121fb2ddfc6528fb0413b2",
-                "sha256:cc4d65aeeaa04136a12677d3dd0b1c0c94dc43abac5860ab33cceb42b801c1e8",
-                "sha256:ce4bcc037df4fc5e3d184794f27bdaab018943698f4ca31630bc7f84a7b69c6d",
-                "sha256:cec7d9412a9102bdc577382c3929b337320c4c4c4849f2c5cdd14d7368c5562d",
-                "sha256:d400bfb9a37b1351253cb402671cea7e89bdecc294e8016a707f6d1d8ac934f9",
-                "sha256:d61f4695e6c866a23a21acab0509af1cdfd2c013cf256bbf5b6b5e2695827162",
-                "sha256:db0fbb9c62743ce59a9ff687eb5f4afbe77e5e8403d6697f7446e5f609976f76",
-                "sha256:dd86c085fae2efd48ac91dd7ccffcfc0571387fe1193d33b6394db7ef31fe2a4",
-                "sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e",
-                "sha256:e229a521186c75c8ad9490854fd8bbdd9a0c9aa3a524326b55be83b54d4e0ad9",
-                "sha256:e263d77ee3dd201c3a142934a086a4450861778baaeeb45db4591ef65550b0a6",
-                "sha256:ed9cb427ba5504c1dc15ede7d516b84757c3e3d7868ccc85121d9310d27eed0b",
-                "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01",
-                "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"
+                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
+                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
+                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
+                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
+                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
+                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
+                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
+                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
+                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
+                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
+                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
+                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
+                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
+                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
+                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
+                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
+                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
+                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
+                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
+                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
+                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
+                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
+                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
+                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
+                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
+                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
+                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
+                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
+                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
+                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
+                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
+                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
+                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
+                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
+                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
+                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
+                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
+                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
+                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
+                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
+                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
+                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
+                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
+                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
+                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
+                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
+                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
+                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
+                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
+                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
+                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
+                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
+                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
+                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
+                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
+                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
+                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
+                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
+                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
+                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
+                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
+                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
+                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
+                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
+                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
+                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
+                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
+                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
+                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
+                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
+                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
+                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
+                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
+                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
+                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "version": "==1.15.1"
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==3.1.0"
         },
-        "charset-normalizer": {
+        "classify-imports": {
             "hashes": [
-                "sha256:00d3ffdaafe92a5dc603cb9bd5111aaa36dfa187c8285c543be562e61b755f6b",
-                "sha256:024e606be3ed92216e2b6952ed859d86b4cfa52cd5bc5f050e7dc28f9b43ec42",
-                "sha256:0298eafff88c99982a4cf66ba2efa1128e4ddaca0b05eec4c456bbc7db691d8d",
-                "sha256:02a51034802cbf38db3f89c66fb5d2ec57e6fe7ef2f4a44d070a593c3688667b",
-                "sha256:083c8d17153ecb403e5e1eb76a7ef4babfc2c48d58899c98fcaa04833e7a2f9a",
-                "sha256:0a11e971ed097d24c534c037d298ad32c6ce81a45736d31e0ff0ad37ab437d59",
-                "sha256:0bf2dae5291758b6f84cf923bfaa285632816007db0330002fa1de38bfcb7154",
-                "sha256:0c0a590235ccd933d9892c627dec5bc7511ce6ad6c1011fdf5b11363022746c1",
-                "sha256:0f438ae3532723fb6ead77e7c604be7c8374094ef4ee2c5e03a3a17f1fca256c",
-                "sha256:109487860ef6a328f3eec66f2bf78b0b72400280d8f8ea05f69c51644ba6521a",
-                "sha256:11b53acf2411c3b09e6af37e4b9005cba376c872503c8f28218c7243582df45d",
-                "sha256:12db3b2c533c23ab812c2b25934f60383361f8a376ae272665f8e48b88e8e1c6",
-                "sha256:14e76c0f23218b8f46c4d87018ca2e441535aed3632ca134b10239dfb6dadd6b",
-                "sha256:16a8663d6e281208d78806dbe14ee9903715361cf81f6d4309944e4d1e59ac5b",
-                "sha256:292d5e8ba896bbfd6334b096e34bffb56161c81408d6d036a7dfa6929cff8783",
-                "sha256:2c03cc56021a4bd59be889c2b9257dae13bf55041a3372d3295416f86b295fb5",
-                "sha256:2e396d70bc4ef5325b72b593a72c8979999aa52fb8bcf03f701c1b03e1166918",
-                "sha256:2edb64ee7bf1ed524a1da60cdcd2e1f6e2b4f66ef7c077680739f1641f62f555",
-                "sha256:31a9ddf4718d10ae04d9b18801bd776693487cbb57d74cc3458a7673f6f34639",
-                "sha256:356541bf4381fa35856dafa6a965916e54bed415ad8a24ee6de6e37deccf2786",
-                "sha256:358a7c4cb8ba9b46c453b1dd8d9e431452d5249072e4f56cfda3149f6ab1405e",
-                "sha256:37f8febc8ec50c14f3ec9637505f28e58d4f66752207ea177c1d67df25da5aed",
-                "sha256:39049da0ffb96c8cbb65cbf5c5f3ca3168990adf3551bd1dee10c48fce8ae820",
-                "sha256:39cf9ed17fe3b1bc81f33c9ceb6ce67683ee7526e65fde1447c772afc54a1bb8",
-                "sha256:3ae1de54a77dc0d6d5fcf623290af4266412a7c4be0b1ff7444394f03f5c54e3",
-                "sha256:3b590df687e3c5ee0deef9fc8c547d81986d9a1b56073d82de008744452d6541",
-                "sha256:3e45867f1f2ab0711d60c6c71746ac53537f1684baa699f4f668d4c6f6ce8e14",
-                "sha256:3fc1c4a2ffd64890aebdb3f97e1278b0cc72579a08ca4de8cd2c04799a3a22be",
-                "sha256:4457ea6774b5611f4bed5eaa5df55f70abde42364d498c5134b7ef4c6958e20e",
-                "sha256:44ba614de5361b3e5278e1241fda3dc1838deed864b50a10d7ce92983797fa76",
-                "sha256:4a8fcf28c05c1f6d7e177a9a46a1c52798bfe2ad80681d275b10dcf317deaf0b",
-                "sha256:4b0d02d7102dd0f997580b51edc4cebcf2ab6397a7edf89f1c73b586c614272c",
-                "sha256:502218f52498a36d6bf5ea77081844017bf7982cdbe521ad85e64cabee1b608b",
-                "sha256:503e65837c71b875ecdd733877d852adbc465bd82c768a067badd953bf1bc5a3",
-                "sha256:5995f0164fa7df59db4746112fec3f49c461dd6b31b841873443bdb077c13cfc",
-                "sha256:59e5686dd847347e55dffcc191a96622f016bc0ad89105e24c14e0d6305acbc6",
-                "sha256:601f36512f9e28f029d9481bdaf8e89e5148ac5d89cffd3b05cd533eeb423b59",
-                "sha256:608862a7bf6957f2333fc54ab4399e405baad0163dc9f8d99cb236816db169d4",
-                "sha256:62595ab75873d50d57323a91dd03e6966eb79c41fa834b7a1661ed043b2d404d",
-                "sha256:70990b9c51340e4044cfc394a81f614f3f90d41397104d226f21e66de668730d",
-                "sha256:71140351489970dfe5e60fc621ada3e0f41104a5eddaca47a7acb3c1b851d6d3",
-                "sha256:72966d1b297c741541ca8cf1223ff262a6febe52481af742036a0b296e35fa5a",
-                "sha256:74292fc76c905c0ef095fe11e188a32ebd03bc38f3f3e9bcb85e4e6db177b7ea",
-                "sha256:761e8904c07ad053d285670f36dd94e1b6ab7f16ce62b9805c475b7aa1cffde6",
-                "sha256:772b87914ff1152b92a197ef4ea40efe27a378606c39446ded52c8f80f79702e",
-                "sha256:79909e27e8e4fcc9db4addea88aa63f6423ebb171db091fb4373e3312cb6d603",
-                "sha256:7e189e2e1d3ed2f4aebabd2d5b0f931e883676e51c7624826e0a4e5fe8a0bf24",
-                "sha256:7eb33a30d75562222b64f569c642ff3dc6689e09adda43a082208397f016c39a",
-                "sha256:81d6741ab457d14fdedc215516665050f3822d3e56508921cc7239f8c8e66a58",
-                "sha256:8499ca8f4502af841f68135133d8258f7b32a53a1d594aa98cc52013fff55678",
-                "sha256:84c3990934bae40ea69a82034912ffe5a62c60bbf6ec5bc9691419641d7d5c9a",
-                "sha256:87701167f2a5c930b403e9756fab1d31d4d4da52856143b609e30a1ce7160f3c",
-                "sha256:88600c72ef7587fe1708fd242b385b6ed4b8904976d5da0893e31df8b3480cb6",
-                "sha256:8ac7b6a045b814cf0c47f3623d21ebd88b3e8cf216a14790b455ea7ff0135d18",
-                "sha256:8b8af03d2e37866d023ad0ddea594edefc31e827fee64f8de5611a1dbc373174",
-                "sha256:8c7fe7afa480e3e82eed58e0ca89f751cd14d767638e2550c77a92a9e749c317",
-                "sha256:8eade758719add78ec36dc13201483f8e9b5d940329285edcd5f70c0a9edbd7f",
-                "sha256:911d8a40b2bef5b8bbae2e36a0b103f142ac53557ab421dc16ac4aafee6f53dc",
-                "sha256:93ad6d87ac18e2a90b0fe89df7c65263b9a99a0eb98f0a3d2e079f12a0735837",
-                "sha256:95dea361dd73757c6f1c0a1480ac499952c16ac83f7f5f4f84f0658a01b8ef41",
-                "sha256:9ab77acb98eba3fd2a85cd160851816bfce6871d944d885febf012713f06659c",
-                "sha256:9cb3032517f1627cc012dbc80a8ec976ae76d93ea2b5feaa9d2a5b8882597579",
-                "sha256:9cf4e8ad252f7c38dd1f676b46514f92dc0ebeb0db5552f5f403509705e24753",
-                "sha256:9d9153257a3f70d5f69edf2325357251ed20f772b12e593f3b3377b5f78e7ef8",
-                "sha256:a152f5f33d64a6be73f1d30c9cc82dfc73cec6477ec268e7c6e4c7d23c2d2291",
-                "sha256:a16418ecf1329f71df119e8a65f3aa68004a3f9383821edcb20f0702934d8087",
-                "sha256:a60332922359f920193b1d4826953c507a877b523b2395ad7bc716ddd386d866",
-                "sha256:a8d0fc946c784ff7f7c3742310cc8a57c5c6dc31631269876a88b809dbeff3d3",
-                "sha256:ab5de034a886f616a5668aa5d098af2b5385ed70142090e2a31bcbd0af0fdb3d",
-                "sha256:c22d3fe05ce11d3671297dc8973267daa0f938b93ec716e12e0f6dee81591dc1",
-                "sha256:c2ac1b08635a8cd4e0cbeaf6f5e922085908d48eb05d44c5ae9eabab148512ca",
-                "sha256:c512accbd6ff0270939b9ac214b84fb5ada5f0409c44298361b2f5e13f9aed9e",
-                "sha256:c75ffc45f25324e68ab238cb4b5c0a38cd1c3d7f1fb1f72b5541de469e2247db",
-                "sha256:c95a03c79bbe30eec3ec2b7f076074f4281526724c8685a42872974ef4d36b72",
-                "sha256:cadaeaba78750d58d3cc6ac4d1fd867da6fc73c88156b7a3212a3cd4819d679d",
-                "sha256:cd6056167405314a4dc3c173943f11249fa0f1b204f8b51ed4bde1a9cd1834dc",
-                "sha256:db72b07027db150f468fbada4d85b3b2729a3db39178abf5c543b784c1254539",
-                "sha256:df2c707231459e8a4028eabcd3cfc827befd635b3ef72eada84ab13b52e1574d",
-                "sha256:e62164b50f84e20601c1ff8eb55620d2ad25fb81b59e3cd776a1902527a788af",
-                "sha256:e696f0dd336161fca9adbb846875d40752e6eba585843c768935ba5c9960722b",
-                "sha256:eaa379fcd227ca235d04152ca6704c7cb55564116f8bc52545ff357628e10602",
-                "sha256:ebea339af930f8ca5d7a699b921106c6e29c617fe9606fa7baa043c1cdae326f",
-                "sha256:f4c39b0e3eac288fedc2b43055cfc2ca7a60362d0e5e87a637beac5d801ef478",
-                "sha256:f5057856d21e7586765171eac8b9fc3f7d44ef39425f85dbcccb13b3ebea806c",
-                "sha256:f6f45710b4459401609ebebdbcfb34515da4fc2aa886f95107f556ac69a9147e",
-                "sha256:f97e83fa6c25693c7a35de154681fcc257c1c41b38beb0304b9c4d2d9e164479",
-                "sha256:f9d0c5c045a3ca9bedfc35dca8526798eb91a07aa7a2c0fee134c6c6f321cbd7",
-                "sha256:ff6f3db31555657f3163b15a6b7c6938d08df7adbfc9dd13d9d19edad678f1e8"
+                "sha256:7abfb7ea92149b29d046bd34573d247ba6e68cc28100c801eba4af17964fc40e",
+                "sha256:dbbc264b70a470ed8c6c95976a11dfb8b7f63df44ed1af87328bbed2663f5161"
             ],
-            "version": "==3.0.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==4.2.0"
         },
         "click": {
             "hashes": [
                 "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
                 "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==8.1.3"
         },
-        "cryptography": {
+        "colorlog": {
             "hashes": [
-                "sha256:0f8da300b5c8af9f98111ffd512910bc792b4c77392a9523624680f7956a99d4",
-                "sha256:35f7c7d015d474f4011e859e93e789c87d21f6f4880ebdc29896a60403328f1f",
-                "sha256:4789d1e3e257965e960232345002262ede4d094d1a19f4d3b52e48d4d8f3b885",
-                "sha256:5aa67414fcdfa22cf052e640cb5ddc461924a045cacf325cd164e65312d99502",
-                "sha256:5d2d8b87a490bfcd407ed9d49093793d0f75198a35e6eb1a923ce1ee86c62b41",
-                "sha256:6687ef6d0a6497e2b58e7c5b852b53f62142cfa7cd1555795758934da363a965",
-                "sha256:6f8ba7f0328b79f08bdacc3e4e66fb4d7aab0c3584e0bd41328dce5262e26b2e",
-                "sha256:706843b48f9a3f9b9911979761c91541e3d90db1ca905fd63fee540a217698bc",
-                "sha256:807ce09d4434881ca3a7594733669bd834f5b2c6d5c7e36f8c00f691887042ad",
-                "sha256:83e17b26de248c33f3acffb922748151d71827d6021d98c70e6c1a25ddd78505",
-                "sha256:96f1157a7c08b5b189b16b47bc9db2332269d6680a196341bf30046330d15388",
-                "sha256:aec5a6c9864be7df2240c382740fcf3b96928c46604eaa7f3091f58b878c0bb6",
-                "sha256:b0afd054cd42f3d213bf82c629efb1ee5f22eba35bf0eec88ea9ea7304f511a2",
-                "sha256:c5caeb8188c24888c90b5108a441c106f7faa4c4c075a2bcae438c6e8ca73cef",
-                "sha256:ced4e447ae29ca194449a3f1ce132ded8fcab06971ef5f618605aacaa612beac",
-                "sha256:d1f6198ee6d9148405e49887803907fe8962a23e6c6f83ea7d98f1c0de375695",
-                "sha256:e124352fd3db36a9d4a21c1aa27fd5d051e621845cb87fb851c08f4f75ce8be6",
-                "sha256:e422abdec8b5fa8462aa016786680720d78bdce7a30c652b7fadf83a4ba35336",
-                "sha256:ef8b72fa70b348724ff1218267e7f7375b8de4e8194d1636ee60510aae104cd0",
-                "sha256:f0c64d1bd842ca2633e74a1a28033d139368ad959872533b1bab8c80e8240a0c",
-                "sha256:f24077a3b5298a5a06a8e0536e3ea9ec60e4c7ac486755e5fb6e6ea9b3500106",
-                "sha256:fdd188c8a6ef8769f148f88f859884507b954cc64db6b52f66ef199bb9ad660a",
-                "sha256:fe913f20024eb2cb2f323e42a64bdf2911bb9738a15dba7d3cce48151034e3a8"
+                "sha256:0d33ca236784a1ba3ff9c532d4964126d8a2c44f1f0cb1d2b0728196f512f662",
+                "sha256:bd94bd21c1e13fac7bd3153f4bc3a7dc0eb0974b8bc2fdf1a989e474f6e582e5"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==39.0.1"
+            "version": "==6.7.0"
+        },
+        "coverage": {
+            "extras": [
+                "toml"
+            ],
+            "hashes": [
+                "sha256:0342a28617e63ad15d96dca0f7ae9479a37b7d8a295f749c14f3436ea59fdcb3",
+                "sha256:066b44897c493e0dcbc9e6a6d9f8bbb6607ef82367cf6810d387c09f0cd4fe9a",
+                "sha256:10b15394c13544fce02382360cab54e51a9e0fd1bd61ae9ce012c0d1e103c813",
+                "sha256:12580845917b1e59f8a1c2ffa6af6d0908cb39220f3019e36c110c943dc875b0",
+                "sha256:156192e5fd3dbbcb11cd777cc469cf010a294f4c736a2b2c891c77618cb1379a",
+                "sha256:1637253b11a18f453e34013c665d8bf15904c9e3c44fbda34c643fbdc9d452cd",
+                "sha256:292300f76440651529b8ceec283a9370532f4ecba9ad67d120617021bb5ef139",
+                "sha256:30dcaf05adfa69c2a7b9f7dfd9f60bc8e36b282d7ed25c308ef9e114de7fc23b",
+                "sha256:338aa9d9883aaaad53695cb14ccdeb36d4060485bb9388446330bef9c361c252",
+                "sha256:373ea34dca98f2fdb3e5cb33d83b6d801007a8074f992b80311fc589d3e6b790",
+                "sha256:38c0a497a000d50491055805313ed83ddba069353d102ece8aef5d11b5faf045",
+                "sha256:40cc0f91c6cde033da493227797be2826cbf8f388eaa36a0271a97a332bfd7ce",
+                "sha256:4436cc9ba5414c2c998eaedee5343f49c02ca93b21769c5fdfa4f9d799e84200",
+                "sha256:509ecd8334c380000d259dc66feb191dd0a93b21f2453faa75f7f9cdcefc0718",
+                "sha256:5c587f52c81211d4530fa6857884d37f514bcf9453bdeee0ff93eaaf906a5c1b",
+                "sha256:5f3671662dc4b422b15776cdca89c041a6349b4864a43aa2350b6b0b03bbcc7f",
+                "sha256:6599bf92f33ab041e36e06d25890afbdf12078aacfe1f1d08c713906e49a3fe5",
+                "sha256:6e8a95f243d01ba572341c52f89f3acb98a3b6d1d5d830efba86033dd3687ade",
+                "sha256:706ec567267c96717ab9363904d846ec009a48d5f832140b6ad08aad3791b1f5",
+                "sha256:780551e47d62095e088f251f5db428473c26db7829884323e56d9c0c3118791a",
+                "sha256:7ff8f3fb38233035028dbc93715551d81eadc110199e14bbbfa01c5c4a43f8d8",
+                "sha256:828189fcdda99aae0d6bf718ea766b2e715eabc1868670a0a07bf8404bf58c33",
+                "sha256:857abe2fa6a4973f8663e039ead8d22215d31db613ace76e4a98f52ec919068e",
+                "sha256:883123d0bbe1c136f76b56276074b0c79b5817dd4238097ffa64ac67257f4b6c",
+                "sha256:8877d9b437b35a85c18e3c6499b23674684bf690f5d96c1006a1ef61f9fdf0f3",
+                "sha256:8e575a59315a91ccd00c7757127f6b2488c2f914096077c745c2f1ba5b8c0969",
+                "sha256:97072cc90f1009386c8a5b7de9d4fc1a9f91ba5ef2146c55c1f005e7b5c5e068",
+                "sha256:9a22cbb5ede6fade0482111fa7f01115ff04039795d7092ed0db43522431b4f2",
+                "sha256:a063aad9f7b4c9f9da7b2550eae0a582ffc7623dca1c925e50c3fbde7a579771",
+                "sha256:a08c7401d0b24e8c2982f4e307124b671c6736d40d1c39e09d7a8687bddf83ed",
+                "sha256:a0b273fe6dc655b110e8dc89b8ec7f1a778d78c9fd9b4bda7c384c8906072212",
+                "sha256:a2b3b05e22a77bb0ae1a3125126a4e08535961c946b62f30985535ed40e26614",
+                "sha256:a66e055254a26c82aead7ff420d9fa8dc2da10c82679ea850d8feebf11074d88",
+                "sha256:aa387bd7489f3e1787ff82068b295bcaafbf6f79c3dad3cbc82ef88ce3f48ad3",
+                "sha256:ae453f655640157d76209f42c62c64c4d4f2c7f97256d3567e3b439bd5c9b06c",
+                "sha256:b5016e331b75310610c2cf955d9f58a9749943ed5f7b8cfc0bb89c6134ab0a84",
+                "sha256:b9a4ee55174b04f6af539218f9f8083140f61a46eabcaa4234f3c2a452c4ed11",
+                "sha256:bd3b4b8175c1db502adf209d06136c000df4d245105c8839e9d0be71c94aefe1",
+                "sha256:bebea5f5ed41f618797ce3ffb4606c64a5de92e9c3f26d26c2e0aae292f015c1",
+                "sha256:c10fbc8a64aa0f3ed136b0b086b6b577bc64d67d5581acd7cc129af52654384e",
+                "sha256:c2c41c1b1866b670573657d584de413df701f482574bad7e28214a2362cb1fd1",
+                "sha256:cf97ed82ca986e5c637ea286ba2793c85325b30f869bf64d3009ccc1a31ae3fd",
+                "sha256:d1f25ee9de21a39b3a8516f2c5feb8de248f17da7eead089c2e04aa097936b47",
+                "sha256:d2fbc2a127e857d2f8898aaabcc34c37771bf78a4d5e17d3e1f5c30cd0cbc62a",
+                "sha256:dc945064a8783b86fcce9a0a705abd7db2117d95e340df8a4333f00be5efb64c",
+                "sha256:ddc5a54edb653e9e215f75de377354e2455376f416c4378e1d43b08ec50acc31",
+                "sha256:e8834e5f17d89e05697c3c043d3e58a8b19682bf365048837383abfe39adaed5",
+                "sha256:ef9659d1cda9ce9ac9585c045aaa1e59223b143f2407db0eaee0b61a4f266fb6",
+                "sha256:f6f5cab2d7f0c12f8187a376cc6582c477d2df91d63f75341307fcdcb5d60303",
+                "sha256:f81c9b4bd8aa747d417407a7f6f0b1469a43b36a85748145e144ac4e8d303cb5",
+                "sha256:f99ef080288f09ffc687423b8d60978cf3a465d3f404a18d1a05474bd8575a47"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==7.2.5"
+        },
+        "css-html-js-minify": {
+            "hashes": [
+                "sha256:3da9d35ac0db8ca648c1b543e0e801d7ca0bab9e6bfd8418fee59d5ae001727a",
+                "sha256:4704e04a0cd6dd56d61bbfa3bfffc630da6b2284be33519be0b456672e2a2438",
+                "sha256:4a9f11f7e0496f5284d12111f3ba4ff5ff2023d12f15d195c9c48bd97013746c"
+            ],
+            "version": "==2.5.5"
         },
         "distlib": {
             "hashes": [
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
             "version": "==0.3.6"
@@ -287,341 +281,399 @@
             "hashes": [
                 "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6",
                 "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.19"
         },
-        "editables": {
-            "hashes": [
-                "sha256:167524e377358ed1f1374e61c268f0d7a4bf7dbd046c656f7b410cde16161b1a",
-                "sha256:ee686a8db9f5d91da39849f175ffeef094dd0e9c36d6a59a2e8c7f92a3b80020"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==0.3"
-        },
         "filelock": {
             "hashes": [
-                "sha256:7b319f24340b51f55a2bf7a12ac0755a9b03e718311dac567a0f4f7fabd2f5de",
-                "sha256:f58d535af89bb9ad5cd4df046f741f8553a418c01a7856bf0d173bbc9f6bd16d"
+                "sha256:ad98852315c2ab702aeb628412cbf7e95b7ce8c3bf9565670b4eaecf1db370a9",
+                "sha256:fc03ae43288c013d2ea83c8597001b1129db351aad9c57fe2409327916b8e718"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.9.0"
-        },
-        "flit": {
-            "hashes": [
-                "sha256:5ee0f88fd1cfa4160d1a8fa01237e96d06d677ae0403a0bbabbb277cb37c5e9c",
-                "sha256:d0f2a8f4bd45dc794befbf5839ecc0fd3830d65a57bd52b5997542fac5d5e937"
-            ],
-            "index": "pypi",
-            "version": "==3.8.0"
-        },
-        "flit-core": {
-            "hashes": [
-                "sha256:64a29ec845164a6abe1136bf4bc5ae012bdfe758ed42fc7571a9059a7c80bd83",
-                "sha256:b305b30c99526df5e63d6022dd2310a0a941a187bd3884f4c8ef0418df6c39f3"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==3.8.0"
-        },
-        "h11": {
-            "hashes": [
-                "sha256:8f19fbbe99e72420ff35c00b27a34cb9937e902a8b810e2c88300c6f0a3b699d",
-                "sha256:e3fe4ac4b851c468cc8363d500db52c2ead036020723024a109d37346efaa761"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==0.14.0"
-        },
-        "hatch": {
-            "hashes": [
-                "sha256:650e671ba300318e498ef93bbe3b99b32ce14920764fb8753f89993f63eed79a",
-                "sha256:e9b3ceb2d4022c23fffd38aaed97774a6368bfdf0a2a5b67bc88b1577df58e9d"
-            ],
-            "index": "pypi",
-            "version": "==1.6.3"
-        },
-        "hatchling": {
-            "hashes": [
-                "sha256:357d5a5abac0d28e24fa87534efc63f5ba3f9b3306675678049ca4ba9f2a6674",
-                "sha256:f8d275a2cc720735286b7c2e2bc35da05761e6d3695c2fa416550395f10c53c7"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==1.13.0"
-        },
-        "httpcore": {
-            "hashes": [
-                "sha256:c5d6f04e2fc530f39e0c077e6a30caa53f1451096120f1f38b954afd0b17c0cb",
-                "sha256:da1fb708784a938aa084bde4feb8317056c55037247c787bd7e19eb2c2949dc0"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==0.16.3"
-        },
-        "httpx": {
-            "hashes": [
-                "sha256:9818458eb565bb54898ccb9b8b251a28785dd4a55afbc23d0eb410754fe7d0f9",
-                "sha256:a211fcce9b1254ea24f0cd6af9869b3d29aba40154e947d2a07bb499b3e310d6"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==0.23.3"
-        },
-        "hyperlink": {
-            "hashes": [
-                "sha256:427af957daa58bc909471c6c40f74c5450fa123dd093fc53efd2e91d2705a56b",
-                "sha256:e6b14c37ecb73e89c77d78cdb4c2cc8f3fb59a885c5b3f819ff4ed80f25af1b4"
-            ],
-            "version": "==21.0.0"
+            "version": "==3.12.0"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==3.4"
         },
-        "importlib-metadata": {
+        "imagesize": {
             "hashes": [
-                "sha256:7efb448ec9a5e313a57655d35aa54cd3e01b7e1fbcf72dce1bf06119420f5bad",
-                "sha256:e354bedeb60efa6affdcc8ae121b73544a7aa74156d047311948f6d711cd378d"
+                "sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b",
+                "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
             ],
-            "markers": "python_version < '3.12'",
-            "version": "==6.0.0"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==1.4.1"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
-        "jaraco.classes": {
+        "jinja2": {
             "hashes": [
-                "sha256:2353de3288bc6b82120752201c6b1c1a14b058267fa424ed5ce5984e3b922158",
-                "sha256:89559fa5c1d3c34eff6f631ad80bb21f378dbcbb35dd161fd2c6b93f5be2f98a"
+                "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852",
+                "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.2.3"
+            "version": "==3.1.2"
         },
-        "jeepney": {
-            "hashes": [
-                "sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806",
-                "sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755"
-            ],
-            "markers": "sys_platform == 'linux'",
-            "version": "==0.8.0"
-        },
-        "keyring": {
-            "hashes": [
-                "sha256:771ed2a91909389ed6148631de678f82ddc73737d85a927f382a8a1b157898cd",
-                "sha256:ba2e15a9b35e21908d0aaf4e0a47acc52d6ae33444df0da2b49d41a46ef6d678"
+        "lxml": {
+            "hashes": [
+                "sha256:01d36c05f4afb8f7c20fd9ed5badca32a2029b93b1750f571ccc0b142531caf7",
+                "sha256:04876580c050a8c5341d706dd464ff04fd597095cc8c023252566a8826505726",
+                "sha256:05ca3f6abf5cf78fe053da9b1166e062ade3fa5d4f92b4ed688127ea7d7b1d03",
+                "sha256:090c6543d3696cbe15b4ac6e175e576bcc3f1ccfbba970061b7300b0c15a2140",
+                "sha256:0dc313ef231edf866912e9d8f5a042ddab56c752619e92dfd3a2c277e6a7299a",
+                "sha256:0f2b1e0d79180f344ff9f321327b005ca043a50ece8713de61d1cb383fb8ac05",
+                "sha256:13598ecfbd2e86ea7ae45ec28a2a54fb87ee9b9fdb0f6d343297d8e548392c03",
+                "sha256:16efd54337136e8cd72fb9485c368d91d77a47ee2d42b057564aae201257d419",
+                "sha256:1ab8f1f932e8f82355e75dda5413a57612c6ea448069d4fb2e217e9a4bed13d4",
+                "sha256:223f4232855ade399bd409331e6ca70fb5578efef22cf4069a6090acc0f53c0e",
+                "sha256:2455cfaeb7ac70338b3257f41e21f0724f4b5b0c0e7702da67ee6c3640835b67",
+                "sha256:2899456259589aa38bfb018c364d6ae7b53c5c22d8e27d0ec7609c2a1ff78b50",
+                "sha256:2a29ba94d065945944016b6b74e538bdb1751a1db6ffb80c9d3c2e40d6fa9894",
+                "sha256:2a87fa548561d2f4643c99cd13131acb607ddabb70682dcf1dff5f71f781a4bf",
+                "sha256:2e430cd2824f05f2d4f687701144556646bae8f249fd60aa1e4c768ba7018947",
+                "sha256:36c3c175d34652a35475a73762b545f4527aec044910a651d2bf50de9c3352b1",
+                "sha256:3818b8e2c4b5148567e1b09ce739006acfaa44ce3156f8cbbc11062994b8e8dd",
+                "sha256:3ab9fa9d6dc2a7f29d7affdf3edebf6ece6fb28a6d80b14c3b2fb9d39b9322c3",
+                "sha256:3efea981d956a6f7173b4659849f55081867cf897e719f57383698af6f618a92",
+                "sha256:4c8f293f14abc8fd3e8e01c5bd86e6ed0b6ef71936ded5bf10fe7a5efefbaca3",
+                "sha256:5344a43228767f53a9df6e5b253f8cdca7dfc7b7aeae52551958192f56d98457",
+                "sha256:58bfa3aa19ca4c0f28c5dde0ff56c520fbac6f0daf4fac66ed4c8d2fb7f22e74",
+                "sha256:5b4545b8a40478183ac06c073e81a5ce4cf01bf1734962577cf2bb569a5b3bbf",
+                "sha256:5f50a1c177e2fa3ee0667a5ab79fdc6b23086bc8b589d90b93b4bd17eb0e64d1",
+                "sha256:63da2ccc0857c311d764e7d3d90f429c252e83b52d1f8f1d1fe55be26827d1f4",
+                "sha256:6749649eecd6a9871cae297bffa4ee76f90b4504a2a2ab528d9ebe912b101975",
+                "sha256:6804daeb7ef69e7b36f76caddb85cccd63d0c56dedb47555d2fc969e2af6a1a5",
+                "sha256:689bb688a1db722485e4610a503e3e9210dcc20c520b45ac8f7533c837be76fe",
+                "sha256:699a9af7dffaf67deeae27b2112aa06b41c370d5e7633e0ee0aea2e0b6c211f7",
+                "sha256:6b418afe5df18233fc6b6093deb82a32895b6bb0b1155c2cdb05203f583053f1",
+                "sha256:76cf573e5a365e790396a5cc2b909812633409306c6531a6877c59061e42c4f2",
+                "sha256:7b515674acfdcadb0eb5d00d8a709868173acece5cb0be3dd165950cbfdf5409",
+                "sha256:7b770ed79542ed52c519119473898198761d78beb24b107acf3ad65deae61f1f",
+                "sha256:7d2278d59425777cfcb19735018d897ca8303abe67cc735f9f97177ceff8027f",
+                "sha256:7e91ee82f4199af8c43d8158024cbdff3d931df350252288f0d4ce656df7f3b5",
+                "sha256:821b7f59b99551c69c85a6039c65b75f5683bdc63270fec660f75da67469ca24",
+                "sha256:822068f85e12a6e292803e112ab876bc03ed1f03dddb80154c395f891ca6b31e",
+                "sha256:8340225bd5e7a701c0fa98284c849c9b9fc9238abf53a0ebd90900f25d39a4e4",
+                "sha256:85cabf64adec449132e55616e7ca3e1000ab449d1d0f9d7f83146ed5bdcb6d8a",
+                "sha256:880bbbcbe2fca64e2f4d8e04db47bcdf504936fa2b33933efd945e1b429bea8c",
+                "sha256:8d0b4612b66ff5d62d03bcaa043bb018f74dfea51184e53f067e6fdcba4bd8de",
+                "sha256:8e20cb5a47247e383cf4ff523205060991021233ebd6f924bca927fcf25cf86f",
+                "sha256:925073b2fe14ab9b87e73f9a5fde6ce6392da430f3004d8b72cc86f746f5163b",
+                "sha256:998c7c41910666d2976928c38ea96a70d1aa43be6fe502f21a651e17483a43c5",
+                "sha256:9b22c5c66f67ae00c0199f6055705bc3eb3fcb08d03d2ec4059a2b1b25ed48d7",
+                "sha256:9f102706d0ca011de571de32c3247c6476b55bb6bc65a20f682f000b07a4852a",
+                "sha256:a08cff61517ee26cb56f1e949cca38caabe9ea9fbb4b1e10a805dc39844b7d5c",
+                "sha256:a0a336d6d3e8b234a3aae3c674873d8f0e720b76bc1d9416866c41cd9500ffb9",
+                "sha256:a35f8b7fa99f90dd2f5dc5a9fa12332642f087a7641289ca6c40d6e1a2637d8e",
+                "sha256:a38486985ca49cfa574a507e7a2215c0c780fd1778bb6290c21193b7211702ab",
+                "sha256:a5da296eb617d18e497bcf0a5c528f5d3b18dadb3619fbdadf4ed2356ef8d941",
+                "sha256:a6e441a86553c310258aca15d1c05903aaf4965b23f3bc2d55f200804e005ee5",
+                "sha256:a82d05da00a58b8e4c0008edbc8a4b6ec5a4bc1e2ee0fb6ed157cf634ed7fa45",
+                "sha256:ab323679b8b3030000f2be63e22cdeea5b47ee0abd2d6a1dc0c8103ddaa56cd7",
+                "sha256:b1f42b6921d0e81b1bcb5e395bc091a70f41c4d4e55ba99c6da2b31626c44892",
+                "sha256:b23e19989c355ca854276178a0463951a653309fb8e57ce674497f2d9f208746",
+                "sha256:b264171e3143d842ded311b7dccd46ff9ef34247129ff5bf5066123c55c2431c",
+                "sha256:b26a29f0b7fc6f0897f043ca366142d2b609dc60756ee6e4e90b5f762c6adc53",
+                "sha256:b64d891da92e232c36976c80ed7ebb383e3f148489796d8d31a5b6a677825efe",
+                "sha256:b9cc34af337a97d470040f99ba4282f6e6bac88407d021688a5d585e44a23184",
+                "sha256:bc718cd47b765e790eecb74d044cc8d37d58562f6c314ee9484df26276d36a38",
+                "sha256:be7292c55101e22f2a3d4d8913944cbea71eea90792bf914add27454a13905df",
+                "sha256:c83203addf554215463b59f6399835201999b5e48019dc17f182ed5ad87205c9",
+                "sha256:c9ec3eaf616d67db0764b3bb983962b4f385a1f08304fd30c7283954e6a7869b",
+                "sha256:ca34efc80a29351897e18888c71c6aca4a359247c87e0b1c7ada14f0ab0c0fb2",
+                "sha256:ca989b91cf3a3ba28930a9fc1e9aeafc2a395448641df1f387a2d394638943b0",
+                "sha256:d02a5399126a53492415d4906ab0ad0375a5456cc05c3fc0fc4ca11771745cda",
+                "sha256:d17bc7c2ccf49c478c5bdd447594e82692c74222698cfc9b5daae7ae7e90743b",
+                "sha256:d5bf6545cd27aaa8a13033ce56354ed9e25ab0e4ac3b5392b763d8d04b08e0c5",
+                "sha256:d6b430a9938a5a5d85fc107d852262ddcd48602c120e3dbb02137c83d212b380",
+                "sha256:da248f93f0418a9e9d94b0080d7ebc407a9a5e6d0b57bb30db9b5cc28de1ad33",
+                "sha256:da4dd7c9c50c059aba52b3524f84d7de956f7fef88f0bafcf4ad7dde94a064e8",
+                "sha256:df0623dcf9668ad0445e0558a21211d4e9a149ea8f5666917c8eeec515f0a6d1",
+                "sha256:e5168986b90a8d1f2f9dc1b841467c74221bd752537b99761a93d2d981e04889",
+                "sha256:efa29c2fe6b4fdd32e8ef81c1528506895eca86e1d8c4657fda04c9b3786ddf9",
+                "sha256:f1496ea22ca2c830cbcbd473de8f114a320da308438ae65abad6bab7867fe38f",
+                "sha256:f49e52d174375a7def9915c9f06ec4e569d235ad428f70751765f48d5926678c"
+            ],
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
+            "version": "==4.9.2"
+        },
+        "markupsafe": {
+            "hashes": [
+                "sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed",
+                "sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc",
+                "sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2",
+                "sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460",
+                "sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7",
+                "sha256:1bea30e9bf331f3fef67e0a3877b2288593c98a21ccb2cf29b74c581a4eb3af0",
+                "sha256:22152d00bf4a9c7c83960521fc558f55a1adbc0631fbb00a9471e097b19d72e1",
+                "sha256:22731d79ed2eb25059ae3df1dfc9cb1546691cc41f4e3130fe6bfbc3ecbbecfa",
+                "sha256:2298c859cfc5463f1b64bd55cb3e602528db6fa0f3cfd568d3605c50678f8f03",
+                "sha256:28057e985dace2f478e042eaa15606c7efccb700797660629da387eb289b9323",
+                "sha256:2e7821bffe00aa6bd07a23913b7f4e01328c3d5cc0b40b36c0bd81d362faeb65",
+                "sha256:2ec4f2d48ae59bbb9d1f9d7efb9236ab81429a764dedca114f5fdabbc3788013",
+                "sha256:340bea174e9761308703ae988e982005aedf427de816d1afe98147668cc03036",
+                "sha256:40627dcf047dadb22cd25ea7ecfe9cbf3bbbad0482ee5920b582f3809c97654f",
+                "sha256:40dfd3fefbef579ee058f139733ac336312663c6706d1163b82b3003fb1925c4",
+                "sha256:4cf06cdc1dda95223e9d2d3c58d3b178aa5dacb35ee7e3bbac10e4e1faacb419",
+                "sha256:50c42830a633fa0cf9e7d27664637532791bfc31c731a87b202d2d8ac40c3ea2",
+                "sha256:55f44b440d491028addb3b88f72207d71eeebfb7b5dbf0643f7c023ae1fba619",
+                "sha256:608e7073dfa9e38a85d38474c082d4281f4ce276ac0010224eaba11e929dd53a",
+                "sha256:63ba06c9941e46fa389d389644e2d8225e0e3e5ebcc4ff1ea8506dce646f8c8a",
+                "sha256:65608c35bfb8a76763f37036547f7adfd09270fbdbf96608be2bead319728fcd",
+                "sha256:665a36ae6f8f20a4676b53224e33d456a6f5a72657d9c83c2aa00765072f31f7",
+                "sha256:6d6607f98fcf17e534162f0709aaad3ab7a96032723d8ac8750ffe17ae5a0666",
+                "sha256:7313ce6a199651c4ed9d7e4cfb4aa56fe923b1adf9af3b420ee14e6d9a73df65",
+                "sha256:7668b52e102d0ed87cb082380a7e2e1e78737ddecdde129acadb0eccc5423859",
+                "sha256:7df70907e00c970c60b9ef2938d894a9381f38e6b9db73c5be35e59d92e06625",
+                "sha256:7e007132af78ea9df29495dbf7b5824cb71648d7133cf7848a2a5dd00d36f9ff",
+                "sha256:835fb5e38fd89328e9c81067fd642b3593c33e1e17e2fdbf77f5676abb14a156",
+                "sha256:8bca7e26c1dd751236cfb0c6c72d4ad61d986e9a41bbf76cb445f69488b2a2bd",
+                "sha256:8db032bf0ce9022a8e41a22598eefc802314e81b879ae093f36ce9ddf39ab1ba",
+                "sha256:99625a92da8229df6d44335e6fcc558a5037dd0a760e11d84be2260e6f37002f",
+                "sha256:9cad97ab29dfc3f0249b483412c85c8ef4766d96cdf9dcf5a1e3caa3f3661cf1",
+                "sha256:a4abaec6ca3ad8660690236d11bfe28dfd707778e2442b45addd2f086d6ef094",
+                "sha256:a6e40afa7f45939ca356f348c8e23048e02cb109ced1eb8420961b2f40fb373a",
+                "sha256:a6f2fcca746e8d5910e18782f976489939d54a91f9411c32051b4aab2bd7c513",
+                "sha256:a806db027852538d2ad7555b203300173dd1b77ba116de92da9afbc3a3be3eed",
+                "sha256:abcabc8c2b26036d62d4c746381a6f7cf60aafcc653198ad678306986b09450d",
+                "sha256:b8526c6d437855442cdd3d87eede9c425c4445ea011ca38d937db299382e6fa3",
+                "sha256:bb06feb762bade6bf3c8b844462274db0c76acc95c52abe8dbed28ae3d44a147",
+                "sha256:c0a33bc9f02c2b17c3ea382f91b4db0e6cde90b63b296422a939886a7a80de1c",
+                "sha256:c4a549890a45f57f1ebf99c067a4ad0cb423a05544accaf2b065246827ed9603",
+                "sha256:ca244fa73f50a800cf8c3ebf7fd93149ec37f5cb9596aa8873ae2c1d23498601",
+                "sha256:cf877ab4ed6e302ec1d04952ca358b381a882fbd9d1b07cccbfd61783561f98a",
+                "sha256:d9d971ec1e79906046aa3ca266de79eac42f1dbf3612a05dc9368125952bd1a1",
+                "sha256:da25303d91526aac3672ee6d49a2f3db2d9502a4a60b55519feb1a4c7714e07d",
+                "sha256:e55e40ff0cc8cc5c07996915ad367fa47da6b3fc091fdadca7f5403239c5fec3",
+                "sha256:f03a532d7dee1bed20bc4884194a16160a2de9ffc6354b3878ec9682bb623c54",
+                "sha256:f1cd098434e83e656abf198f103a8207a8187c0fc110306691a2e94a78d0abb2",
+                "sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6",
+                "sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.13.1"
-        },
-        "markdown-it-py": {
-            "hashes": [
-                "sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30",
-                "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==2.2.0"
-        },
-        "mdurl": {
-            "hashes": [
-                "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8",
-                "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==0.1.2"
-        },
-        "more-itertools": {
-            "hashes": [
-                "sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d",
-                "sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==9.1.0"
+            "version": "==2.1.2"
         },
         "mypy-extensions": {
             "hashes": [
                 "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
                 "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.0"
         },
-        "packaging": {
+        "nox": {
             "hashes": [
-                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
-                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
+                "sha256:0b1adc619c58ab4fa57d6ab2e7823fe47a32e70202f287d78474adcc7bda1891",
+                "sha256:46c0560b0dc609d7d967dc99e22cb463d3c4caf54a5fda735d6c11b5177e3a9f"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==23.0"
+            "index": "pypi",
+            "version": "==2023.4.22"
         },
-        "pathspec": {
+        "packaging": {
             "hashes": [
-                "sha256:3a66eb970cbac598f9e5ccb5b2cf58930cd8e3ed86d393d541eaf2d8b1705229",
-                "sha256:64d338d4e0914e91c1792321e6907b5a593f1ab1851de7fc269557a21b30ebbc"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.11.0"
+            "version": "==23.1"
         },
-        "pexpect": {
+        "pathspec": {
             "hashes": [
-                "sha256:0b48a55dcb3c05f3329815901ea4fc1537514d6ba867a152b581d69ae3710937",
-                "sha256:fc65a43959d153d0114afe13997d439c22823a27cefceb5ff35c2178c6784c0c"
+                "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687",
+                "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"
             ],
-            "version": "==4.8.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==0.11.1"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:8a1228abb1ef82d788f74139988b137e78692984ec7b08eaa6c65f1723af28f9",
-                "sha256:b1d5eb14f221506f50d6604a561f4c5786d9e80355219694a1b244bcd96f4567"
+                "sha256:47692bc24c1958e8b0f13dd727307cff1db103fca36399f457da8e05f222fdc4",
+                "sha256:7954a68d0ba23558d753f73437c55f89027cf8f5108c19844d4b82e5af396335"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.0.0"
+            "version": "==3.5.0"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.0.0"
         },
-        "ptyprocess": {
+        "pygments": {
             "hashes": [
-                "sha256:4b41f3967fce3af57cc7e94b888626c18bf37a083e3651ca8feeb66d492fef35",
-                "sha256:5c5d0a3b48ceee0b48485e0c26037c0acd7d29765ca3fbb5cb3831d347423220"
+                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
+                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
-            "version": "==0.7.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.1"
         },
-        "pycparser": {
+        "pytest": {
             "hashes": [
-                "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
-                "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
+                "sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362",
+                "sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3"
             ],
-            "version": "==2.21"
+            "index": "pypi",
+            "version": "==7.3.1"
         },
-        "pygments": {
+        "pytest-cov": {
             "hashes": [
-                "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297",
-                "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"
+                "sha256:2feb1b751d66a8bd934e5edfa2e961d11309dc37b73b0eabe73b5945fee20f6b",
+                "sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.14.0"
+            "index": "pypi",
+            "version": "==4.0.0"
         },
-        "pyperclip": {
+        "python-afl": {
             "hashes": [
-                "sha256:105254a8b04934f0bc84e9c24eb360a591aaf6535c9def5f29d92af107a9bf57"
+                "sha256:b373196d747266230bbe842edaaad659625363857c8e765505d765d0613f9544"
             ],
-            "version": "==1.8.2"
+            "index": "pypi",
+            "version": "==0.7.3"
         },
-        "pytest": {
+        "python-slugify": {
+            "extras": [
+                "unidecode"
+            ],
             "hashes": [
-                "sha256:c7c6ca206e93355074ae32f7403e8ea12163b1163c976fee7d4d84027c162be5",
-                "sha256:d45e0952f3727241918b8fd0f376f5ff6b301cc0777c6f9a556935c92d8a7d42"
+                "sha256:70ca6ea68fe63ecc8fa4fcf00ae651fc8a5d02d93dcd12ae6d4fc7ca46c4d395",
+                "sha256:ce0d46ddb668b3be82f4ed5e503dbc33dd815d83e2eb6824211310d3fb172a27"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==8.0.1"
+        },
+        "reorder-python-imports": {
+            "hashes": [
+                "sha256:3f9c16e8781f54c944756d0d1eb34a8c863554f7a4eb3693f574fe19b1a29b56",
+                "sha256:49292ed537829a6bece9fb3746fc1bbe98f52643be5de01a4e13680268a5b0ec"
             ],
             "index": "pypi",
-            "version": "==7.2.1"
+            "version": "==3.9.0"
         },
         "requests": {
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294",
+                "sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4'",
-            "version": "==2.28.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.30.0"
         },
-        "rfc3986": {
-            "extras": [
-                "idna2008"
+        "snowballstemmer": {
+            "hashes": [
+                "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
+                "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
+            "version": "==2.2.0"
+        },
+        "soupsieve": {
             "hashes": [
-                "sha256:270aaf10d87d0d4e095063c65bf3ddbc6ee3d0b226328ce21e036f946e421835",
-                "sha256:a86d6e1f5b1dc238b218b012df0aa79409667bb209e58da56d0b94704e712a97"
+                "sha256:1c1bfee6819544a3447586c889157365a27e10d88cde3ad3da0cf0ddf646feb8",
+                "sha256:89d12b2d5dfcd2c9e8c22326da9d9aa9cb3dfab0a83a024f05704076ee8d35ea"
             ],
-            "version": "==1.5.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.4.1"
         },
-        "rich": {
+        "sphinx": {
             "hashes": [
-                "sha256:125d96d20c92b946b983d0d392b84ff945461e5a06d3867e9f9e575f8697b67f",
-                "sha256:8aa57747f3fc3e977684f0176a88e789be314a99f99b43b75d1e9cb5dc6db9e9"
+                "sha256:283c44aa28922bb4223777b44ac0d59af50a279ac7690dfe945bb2b9575dc41b",
+                "sha256:3cfc1c6756ef1b132687b813ec6ea2214cb7a7e5d1dcb2772006cb895a0fa469"
             ],
-            "markers": "python_full_version >= '3.7.0'",
-            "version": "==13.3.1"
+            "markers": "python_version >= '3.8'",
+            "version": "==7.0.0"
         },
-        "secretstorage": {
+        "sphinx-material": {
+            "git": "https://github.com/bashtage/sphinx-material.git",
+            "ref": "ac7444216f4d2a568ff9d7cfe386929537f7344d"
+        },
+        "sphinxcontrib-applehelp": {
             "hashes": [
-                "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
-                "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
+                "sha256:29d341f67fb0f6f586b23ad80e072c8e6ad0b48417db2bde114a4c9746feb228",
+                "sha256:828f867945bbe39817c210a1abfd1bc4895c8b73fcaade56d45357a348a07d7e"
             ],
-            "markers": "sys_platform == 'linux'",
-            "version": "==3.3.3"
+            "markers": "python_version >= '3.8'",
+            "version": "==1.0.4"
         },
-        "shellingham": {
+        "sphinxcontrib-devhelp": {
             "hashes": [
-                "sha256:368bf8c00754fd4f55afb7bbb86e272df77e4dc76ac29dbcbb81a59e9fc15744",
-                "sha256:823bc5fb5c34d60f285b624e7264f4dda254bc803a3774a147bf99c0e3004a28"
+                "sha256:8165223f9a335cc1af7ffe1ed31d2871f325254c0423bc0c4c7cd1c1e4734a2e",
+                "sha256:ff7f1afa7b9642e7060379360a67e9c41e8f3121f2ce9164266f61b9f4b338e4"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==1.5.0.post1"
+            "markers": "python_version >= '3.5'",
+            "version": "==1.0.2"
         },
-        "sniffio": {
+        "sphinxcontrib-htmlhelp": {
             "hashes": [
-                "sha256:e60305c5e5d314f5389259b7f22aaa33d8f7dee49763119234af3755c55b9101",
-                "sha256:eecefdce1e5bbfb7ad2eeaabf7c1eeb404d7757c379bd1f7e5cce9d8bf425384"
+                "sha256:0cbdd302815330058422b98a113195c9249825d681e18f11e8b1f78a2f11efff",
+                "sha256:c38cb46dccf316c79de6e5515e1770414b797162b23cd3d06e67020e1d2a6903"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==1.3.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.0.1"
         },
-        "tomli-w": {
+        "sphinxcontrib-jsmath": {
             "hashes": [
-                "sha256:9f2a07e8be30a0729e533ec968016807069991ae2fd921a78d42f429ae5f4463",
-                "sha256:f463434305e0336248cac9c2dc8076b707d8a12d019dd349f5c1e382dd1ae1b9"
+                "sha256:2ec2eaebfb78f3f2078e73666b1415417a116cc848b72e5172e596c871103178",
+                "sha256:a9925e4a4587247ed2191a22df5f6970656cb8ca2bd6284309578f2153e0c4b8"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==1.0.0"
+            "markers": "python_version >= '3.5'",
+            "version": "==1.0.1"
         },
-        "tomlkit": {
+        "sphinxcontrib-qthelp": {
             "hashes": [
-                "sha256:07de26b0d8cfc18f871aec595fda24d95b08fef89d147caa861939f37230bf4b",
-                "sha256:71b952e5721688937fb02cf9d354dbcf0785066149d2855e44531ebdd2b65d73"
+                "sha256:4c33767ee058b70dba89a6fc5c1892c0d57a54be67ddd3e7875a18d14cba5a72",
+                "sha256:bd9fc24bcb748a8d51fd4ecaade681350aa63009a347a8c14e637895444dfab6"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==0.11.6"
+            "markers": "python_version >= '3.5'",
+            "version": "==1.0.3"
         },
-        "urllib3": {
+        "sphinxcontrib-serializinghtml": {
             "hashes": [
-                "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
-                "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
+                "sha256:352a9a00ae864471d3a7ead8d7d79f5fc0b57e8b3f95e9867eb9eb28999b92fd",
+                "sha256:aa5f6de5dfdf809ef505c4895e51ef5c9eac17d0f287933eb49ec495280b6952"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.14"
+            "markers": "python_version >= '3.5'",
+            "version": "==1.1.5"
         },
-        "userpath": {
+        "text-unidecode": {
             "hashes": [
-                "sha256:04233d2fcfe5cff911c1e4fb7189755640e1524ff87a4b82ab9d6b875fee5787",
-                "sha256:f133b534a8c0b73511fc6fa40be68f070d9474de1b5aada9cded58cdf23fb557"
+                "sha256:1311f10e8b895935241623731c2ba64f4c455287888b18189350b67134a822e8",
+                "sha256:bad6603bb14d279193107714b288be206cac565dfa49aa5b105294dd5c4aab93"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==1.8.0"
+            "version": "==1.3"
         },
-        "virtualenv": {
+        "unidecode": {
             "hashes": [
-                "sha256:37a640ba82ed40b226599c522d411e4be5edb339a0c0de030c0dc7b646d61590",
-                "sha256:54eb59e7352b573aa04d53f80fc9736ed0ad5143af445a1e539aada6eb947dd1"
+                "sha256:547d7c479e4f377b430dd91ac1275d593308dce0fc464fb2ab7d41f82ec653be",
+                "sha256:fed09cf0be8cf415b391642c2a5addfc72194407caee4f98719e40ec2a72b830"
+            ],
+            "version": "==1.3.6"
+        },
+        "urllib3": {
+            "hashes": [
+                "sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc",
+                "sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.19.0"
+            "version": "==2.0.2"
         },
-        "zipp": {
+        "virtualenv": {
             "hashes": [
-                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
-                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
+                "sha256:6abec7670e5802a528357fdc75b26b9f57d5d92f29c5462ba0fbe45feacc685e",
+                "sha256:a85caa554ced0c0afbd0d638e7e2d7b5f92d23478d05d17a76daeac8f279f924"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.15.0"
+            "version": "==20.23.0"
         }
     }
 }
```

### Comparing `addict-tracking-changes-0.1.1/README.md` & `addict-tracking-changes-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -58,19 +58,17 @@
 for changed_path in body.get_changed_history():
     #<work with changed_path>
 
 body.clear_changed_history()
 ```
 
 ### Behaviour when values are instances of container types 
-addict works as expected when the values of keys are simple data types (such as string, int, float, etc.). However, for container types such as dict, list, tuples, etc. the behaviour 
-is somewhat differs. 
+addict works as expected when the values of keys are simple data types (such as string, int, float, etc.). However, for container types such as dict, list, tuples, etc. the behaviour is somewhat differs. 
 
-* dicts 
-are treated as opaque object just like simple data types
+* dicts are treated as opaque object just like simple data types
 
 ```python
 from addict import Dict
 
 mydict = Dict()
 mydict.a.b.c = {'kk': 1}
 mydict.a.b.e = {'dd': 1}
@@ -106,37 +104,46 @@
 /a/b/0,
 /a/b/1/0,
 /a/c/0,
 /a/c/1/0,
 /a/c/1/1/"
 ```
 
-* tuple 
-tuple  behave same as dict
-
-* sets
-sets behave same as dict
-
+* tuple, namedtuple, sets
+tuple  behave same as dict and are treated as opaque data structure
 
 
 ## Known bugs and Caveats
 1. Only tracks  field additions.  Deletions and updates are not tracked. 
 2. freeze doesn't guards against deletions
 3. building dict from another dict as shown in following expression wont' work
 ```python
-cjs_cfg = Dict(x, track_changes=True)
+cjs_cfg = Dict(other_dict, track_changes=True)
 ```
 instead use
 ```python 
 cjs_cfg = Dict(track_changes = True)
-with open("cjs_cfg.pickle", "rb") as fh:
+with open("other_dict.pickle", "rb") as fh:
     x = pickle.load(fh)
 for _ in oj.dictWalker(x):
     oj.dnew(cjs_cfg, _[0], _[1])
 
 ```
 
+## APIs
+| API                                                    | Description                                           |
+|--------------------------------------------------------+-------------------------------------------------------|
+| Dict(*args, **kwargs)                                  | Initializes a new Dict object                         |
+| to_dict(self)                                          | Converts the Dict object to a regular dictionary      |
+| freeze(self, shouldFreeze=True)                        | Freezes the Dict object, making it immutable          |
+| unfreeze(self)                                         | Unfreezes the Dict object, making it mutable again    |
+| get_changed_history(self, prefix="", path_guards=None) | Returns an iterator with the changed history of keys  |
+| clear_changed_history(self)                            | Clears the changed history of the Dict object         |
+| set_tracker(self, track_changes=False)                 | Sets or resets the change tracker for the Dict object |
+|--------------------------------------------------------+-------------------------------------------------------|
+
+
 ### EndNotes
-- Docs (in readthedocs format): https://monallabs-org.github.io/addict-tracking-changes/#introduction
+- Docs (in readthedocs format): https://monallabs-org.github.io/addict-tracking-changes/#introduction, https://webworks.monallabs.in/addict-tracking-changes
 
 - Developed By: webworks.monallabs.in
```

### Comparing `addict-tracking-changes-0.1.1/pyproject.toml` & `addict-tracking-changes-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `addict-tracking-changes-0.1.1/PKG-INFO` & `addict-tracking-changes-1.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: addict-tracking-changes
-Version: 0.1.1
+Version: 1.0.0
 Summary: Addict dictionary enhanced with ability to track changes -- currently only supports field additions
 Maintainer-email: Kabira K <kabira@monallabs.in>
 Description-Content-Type: text/markdown
 Project-URL: Documentation, https://ofjustpy.github.io/addict-tracking-changes/
 Project-URL: Home, https://webworks.monallabs.in/ofjustpy/addict-tracking-changes
 Project-URL: Source, https://github.com/ofjustpy/addict-tracking-changes
 
@@ -68,19 +68,17 @@
 for changed_path in body.get_changed_history():
     #<work with changed_path>
 
 body.clear_changed_history()
 ```
 
 ### Behaviour when values are instances of container types 
-addict works as expected when the values of keys are simple data types (such as string, int, float, etc.). However, for container types such as dict, list, tuples, etc. the behaviour 
-is somewhat differs. 
+addict works as expected when the values of keys are simple data types (such as string, int, float, etc.). However, for container types such as dict, list, tuples, etc. the behaviour is somewhat differs. 
 
-* dicts 
-are treated as opaque object just like simple data types
+* dicts are treated as opaque object just like simple data types
 
 ```python
 from addict import Dict
 
 mydict = Dict()
 mydict.a.b.c = {'kk': 1}
 mydict.a.b.e = {'dd': 1}
@@ -116,38 +114,47 @@
 /a/b/0,
 /a/b/1/0,
 /a/c/0,
 /a/c/1/0,
 /a/c/1/1/"
 ```
 
-* tuple 
-tuple  behave same as dict
-
-* sets
-sets behave same as dict
-
+* tuple, namedtuple, sets
+tuple  behave same as dict and are treated as opaque data structure
 
 
 ## Known bugs and Caveats
 1. Only tracks  field additions.  Deletions and updates are not tracked. 
 2. freeze doesn't guards against deletions
 3. building dict from another dict as shown in following expression wont' work
 ```python
-cjs_cfg = Dict(x, track_changes=True)
+cjs_cfg = Dict(other_dict, track_changes=True)
 ```
 instead use
 ```python 
 cjs_cfg = Dict(track_changes = True)
-with open("cjs_cfg.pickle", "rb") as fh:
+with open("other_dict.pickle", "rb") as fh:
     x = pickle.load(fh)
 for _ in oj.dictWalker(x):
     oj.dnew(cjs_cfg, _[0], _[1])
 
 ```
 
+## APIs
+| API                                                    | Description                                           |
+|--------------------------------------------------------+-------------------------------------------------------|
+| Dict(*args, **kwargs)                                  | Initializes a new Dict object                         |
+| to_dict(self)                                          | Converts the Dict object to a regular dictionary      |
+| freeze(self, shouldFreeze=True)                        | Freezes the Dict object, making it immutable          |
+| unfreeze(self)                                         | Unfreezes the Dict object, making it mutable again    |
+| get_changed_history(self, prefix="", path_guards=None) | Returns an iterator with the changed history of keys  |
+| clear_changed_history(self)                            | Clears the changed history of the Dict object         |
+| set_tracker(self, track_changes=False)                 | Sets or resets the change tracker for the Dict object |
+|--------------------------------------------------------+-------------------------------------------------------|
+
+
 ### EndNotes
-- Docs (in readthedocs format): https://monallabs-org.github.io/addict-tracking-changes/#introduction
+- Docs (in readthedocs format): https://monallabs-org.github.io/addict-tracking-changes/#introduction, https://webworks.monallabs.in/addict-tracking-changes
 
 - Developed By: webworks.monallabs.in
```

