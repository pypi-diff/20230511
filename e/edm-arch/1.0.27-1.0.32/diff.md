# Comparing `tmp/edm-arch-1.0.27.tar.gz` & `tmp/edm-arch-1.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\mcpherro\Local\Source\Python3\edmpy\dist\tmp9ymjtm39\edm-arch-1.0.27.tar", last modified: Thu Aug 11 12:19:56 2022, max compression
+gzip compressed data, was "edm-arch-1.0.32.tar", last modified: Wed May 10 12:38:48 2023, max compression
```

## Comparing `edm-arch-1.0.27.tar` & `edm-arch-1.0.32.tar`

### file list

```diff
@@ -1,29 +1,35 @@
-drwxrwxrwx   0        0        0        0 2022-08-11 12:19:56.627935 edm-arch-1.0.27/
--rw-rw-rw-   0        0        0     1096 2022-06-07 20:35:30.000000 edm-arch-1.0.27/LICENSE
--rw-rw-rw-   0        0        0     5737 2022-08-11 12:19:56.627935 edm-arch-1.0.27/PKG-INFO
--rw-rw-rw-   0        0        0     4843 2022-08-10 12:19:35.000000 edm-arch-1.0.27/README.md
--rw-rw-rw-   0        0        0      522 2022-06-10 11:27:08.000000 edm-arch-1.0.27/pyproject.toml
--rw-rw-rw-   0        0        0     1221 2022-08-11 12:19:56.641936 edm-arch-1.0.27/setup.cfg
--rw-rw-rw-   0        0        0       73 2022-06-16 14:04:21.000000 edm-arch-1.0.27/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-11 12:19:56.217903 edm-arch-1.0.27/src/
-drwxrwxrwx   0        0        0        0 2022-08-11 12:19:56.538934 edm-arch-1.0.27/src/edm_arch.egg-info/
--rw-rw-rw-   0        0        0     5737 2022-08-11 12:19:56.000000 edm-arch-1.0.27/src/edm_arch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      542 2022-08-11 12:19:56.000000 edm-arch-1.0.27/src/edm_arch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-11 12:19:56.000000 edm-arch-1.0.27/src/edm_arch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-06-22 11:44:30.000000 edm-arch-1.0.27/src/edm_arch.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      132 2022-08-11 12:19:56.000000 edm-arch-1.0.27/src/edm_arch.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-08-11 12:19:56.000000 edm-arch-1.0.27/src/edm_arch.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-08-11 12:19:56.568935 edm-arch-1.0.27/src/edmpy/
--rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm-arch-1.0.27/src/edmpy/__init__.py
--rw-rw-rw-   0        0        0       79 2022-06-21 13:54:13.000000 edm-arch-1.0.27/src/edmpy/__main__.py
--rw-rw-rw-   0        0        0    12982 2022-06-21 11:24:51.000000 edm-arch-1.0.27/src/edmpy/edm.kv
--rw-rw-rw-   0        0        0   180410 2022-08-11 12:14:51.000000 edm-arch-1.0.27/src/edmpy/edm.py
-drwxrwxrwx   0        0        0        0 2022-08-11 12:19:56.622935 edm-arch-1.0.27/src/edmpy/lib/
--rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm-arch-1.0.27/src/edmpy/lib/__init__.py
--rw-rw-rw-   0        0        0     4209 2022-06-20 13:52:19.000000 edm-arch-1.0.27/src/edmpy/lib/blockdata.py
--rw-rw-rw-   0        0        0     4285 2022-06-20 13:52:32.000000 edm-arch-1.0.27/src/edmpy/lib/colorscheme.py
--rw-rw-rw-   0        0        0     2125 2022-06-28 14:51:41.000000 edm-arch-1.0.27/src/edmpy/lib/constants.py
--rw-rw-rw-   0        0        0     3856 2022-06-30 11:59:18.000000 edm-arch-1.0.27/src/edmpy/lib/dbs.py
--rw-rw-rw-   0        0        0   112189 2022-08-07 16:29:38.000000 edm-arch-1.0.27/src/edmpy/lib/e5_widgets.py
--rw-rw-rw-   0        0        0     1772 2022-06-08 15:04:53.000000 edm-arch-1.0.27/src/edmpy/lib/misc.py
--rw-rw-rw-   0        0        0        0 2022-06-07 20:43:53.000000 edm-arch-1.0.27/src/edmpy/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-10 12:38:48.137064 edm-arch-1.0.32/
+-rw-rw-rw-   0        0        0     1096 2022-06-07 20:35:30.000000 edm-arch-1.0.32/LICENSE
+-rw-rw-rw-   0        0        0    16069 2023-05-10 12:38:48.138031 edm-arch-1.0.32/PKG-INFO
+-rw-rw-rw-   0        0        0    15175 2023-05-08 09:53:16.000000 edm-arch-1.0.32/README.md
+-rw-rw-rw-   0        0        0      522 2022-06-10 11:27:08.000000 edm-arch-1.0.32/pyproject.toml
+-rw-rw-rw-   0        0        0     1255 2023-05-10 12:38:48.140033 edm-arch-1.0.32/setup.cfg
+-rw-rw-rw-   0        0        0       73 2022-06-16 14:04:21.000000 edm-arch-1.0.32/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:38:48.087197 edm-arch-1.0.32/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 12:38:48.108031 edm-arch-1.0.32/src/edm_arch.egg-info/
+-rw-rw-rw-   0        0        0    16069 2023-05-10 12:38:48.000000 edm-arch-1.0.32/src/edm_arch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      658 2023-05-10 12:38:48.000000 edm-arch-1.0.32/src/edm_arch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 12:38:48.000000 edm-arch-1.0.32/src/edm_arch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-06-22 11:44:30.000000 edm-arch-1.0.32/src/edm_arch.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      162 2023-05-10 12:38:48.000000 edm-arch-1.0.32/src/edm_arch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-10 12:38:48.000000 edm-arch-1.0.32/src/edm_arch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 12:38:48.125026 edm-arch-1.0.32/src/edmpy/
+-rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm-arch-1.0.32/src/edmpy/__init__.py
+-rw-rw-rw-   0        0        0       79 2022-06-21 13:54:13.000000 edm-arch-1.0.32/src/edmpy/__main__.py
+-rw-rw-rw-   0        0        0    28026 2023-05-08 09:53:16.000000 edm-arch-1.0.32/src/edmpy/cfg.py
+-rw-rw-rw-   0        0        0       18 2023-03-08 09:12:03.000000 edm-arch-1.0.32/src/edmpy/constants.py
+-rw-rw-rw-   0        0        0     5289 2023-05-08 09:53:16.000000 edm-arch-1.0.32/src/edmpy/db.py
+-rw-rw-rw-   0        0        0    13461 2023-05-08 09:53:16.000000 edm-arch-1.0.32/src/edmpy/edm.kv
+-rw-rw-rw-   0        0        0   122722 2023-05-10 12:35:53.000000 edm-arch-1.0.32/src/edmpy/edm.py
+-rw-rw-rw-   0        0        0     5691 2023-05-08 09:53:16.000000 edm-arch-1.0.32/src/edmpy/geo.py
+-rw-rw-rw-   0        0        0     2496 2023-05-08 09:53:16.000000 edm-arch-1.0.32/src/edmpy/ini.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:38:48.135030 edm-arch-1.0.32/src/edmpy/lib/
+-rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm-arch-1.0.32/src/edmpy/lib/__init__.py
+-rw-rw-rw-   0        0        0     4214 2023-05-08 09:53:16.000000 edm-arch-1.0.32/src/edmpy/lib/blockdata.py
+-rw-rw-rw-   0        0        0     4332 2023-05-08 09:53:16.000000 edm-arch-1.0.32/src/edmpy/lib/colorscheme.py
+-rw-rw-rw-   0        0        0     2334 2023-05-08 09:53:16.000000 edm-arch-1.0.32/src/edmpy/lib/constants.py
+-rw-rw-rw-   0        0        0     4035 2023-03-08 08:56:31.000000 edm-arch-1.0.32/src/edmpy/lib/dbs.py
+-rw-rw-rw-   0        0        0   175935 2023-05-10 12:05:08.000000 edm-arch-1.0.32/src/edmpy/lib/e5_widgets.py
+-rw-rw-rw-   0        0        0     1792 2023-05-08 09:53:16.000000 edm-arch-1.0.32/src/edmpy/lib/misc.py
+-rw-rw-rw-   0        0        0        0 2022-06-07 20:43:53.000000 edm-arch-1.0.32/src/edmpy/py.typed
+-rw-rw-rw-   0        0        0    44643 2023-05-10 12:13:46.000000 edm-arch-1.0.32/src/edmpy/totalstation.py
```

### Comparing `edm-arch-1.0.27/LICENSE` & `edm-arch-1.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.27/pyproject.toml` & `edm-arch-1.0.32/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.27/setup.cfg` & `edm-arch-1.0.32/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 646d 2d61 7263 680d 0a64 6573   = edm-arch..des
 00000020: 6372 6970 7469 6f6e 203d 2054 6f74 616c  cription = Total
 00000030: 2073 7461 7469 6f6e 7320 666f 7220 6172   stations for ar
 00000040: 6368 6165 6f6c 6f67 6973 7473 0d0a 7665  chaeologists..ve
-00000050: 7273 696f 6e20 3d20 312e 302e 3237 0d0a  rsion = 1.0.27..
+00000050: 7273 696f 6e20 3d20 312e 302e 3332 0d0a  rsion = 1.0.32..
 00000060: 6175 7468 6f72 203d 2053 6861 6e6e 6f6e  author = Shannon
 00000070: 2050 2e20 4d63 5068 6572 726f 6e0d 0a61   P. McPherron..a
 00000080: 7574 686f 725f 656d 6169 6c20 3d20 6d63  uthor_email = mc
 00000090: 7068 6572 726f 6e40 6576 612e 6d70 672e  pherron@eva.mpg.
 000000a0: 6465 0d0a 6c6f 6e67 5f64 6573 6372 6970  de..long_descrip
 000000b0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 000000c0: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
@@ -51,27 +51,29 @@
 00000320: 200d 0a09 6564 6d70 790d 0a09 6564 6d70   ...edmpy...edmp
 00000330: 792e 6c69 620d 0a69 6e73 7461 6c6c 5f72  y.lib..install_r
 00000340: 6571 7569 7265 7320 3d20 0d0a 096b 6976  equires = ...kiv
 00000350: 793e 3d32 0d0a 0974 696e 7964 623e 3d34  y>=2...tinydb>=4
 00000360: 0d0a 0970 7973 6572 6961 6c3e 3d33 2e35  ...pyserial>=3.5
 00000370: 0d0a 0961 6e67 6c65 733e 3d32 0d0a 0970  ...angles>=2...p
 00000380: 7965 6e63 6861 6e74 3e3d 332e 322e 320d  yenchant>=3.2.2.
-00000390: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
-000003a0: 203d 203e 3d33 2e36 0d0a 7061 636b 6167   = >=3.6..packag
-000003b0: 655f 6469 7220 3d20 0d0a 093d 7372 630d  e_dir = ...=src.
-000003c0: 0a7a 6970 5f73 6166 6520 3d20 6e6f 0d0a  .zip_safe = no..
-000003d0: 0d0a 5b6f 7074 696f 6e73 2e65 7874 7261  ..[options.extra
-000003e0: 735f 7265 7175 6972 655d 0d0a 7465 7374  s_require]..test
-000003f0: 696e 6720 3d20 0d0a 0970 7974 6573 743e  ing = ...pytest>
-00000400: 3d36 2e30 0d0a 0970 7974 6573 742d 636f  =6.0...pytest-co
-00000410: 763e 3d32 2e30 0d0a 096d 7970 793e 3d30  v>=2.0...mypy>=0
-00000420: 2e39 3130 0d0a 0966 6c61 6b65 383e 3d33  .910...flake8>=3
-00000430: 2e39 0d0a 0974 6f78 3e3d 332e 3234 0d0a  .9...tox>=3.24..
-00000440: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
-00000450: 6765 5f64 6174 615d 0d0a 6564 6d70 7920  ge_data]..edmpy 
-00000460: 3d20 0d0a 0970 792e 7479 7065 640d 0a09  = ...py.typed...
-00000470: 2a2e 6b76 0d0a 0d0a 5b66 6c61 6b65 385d  *.kv....[flake8]
-00000480: 0d0a 6d61 782d 6c69 6e65 2d6c 656e 6774  ..max-line-lengt
-00000490: 6820 3d20 3136 300d 0a0d 0a5b 6567 675f  h = 160....[egg_
-000004a0: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-000004b0: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-000004c0: 300d 0a0d 0a                             0....
+00000390: 0a09 6170 7064 6174 613e 3d32 2e32 0d0a  ..appdata>=2.2..
+000003a0: 0972 6571 7565 7374 733e 3d32 2e32 382e  .requests>=2.28.
+000003b0: 310d 0a70 7974 686f 6e5f 7265 7175 6972  1..python_requir
+000003c0: 6573 203d 203e 3d33 2e36 0d0a 7061 636b  es = >=3.6..pack
+000003d0: 6167 655f 6469 7220 3d20 0d0a 093d 7372  age_dir = ...=sr
+000003e0: 630d 0a7a 6970 5f73 6166 6520 3d20 6e6f  c..zip_safe = no
+000003f0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 7874  ....[options.ext
+00000400: 7261 735f 7265 7175 6972 655d 0d0a 7465  ras_require]..te
+00000410: 7374 696e 6720 3d20 0d0a 0970 7974 6573  sting = ...pytes
+00000420: 743e 3d36 2e30 0d0a 0970 7974 6573 742d  t>=6.0...pytest-
+00000430: 636f 763e 3d32 2e30 0d0a 096d 7970 793e  cov>=2.0...mypy>
+00000440: 3d30 2e39 3130 0d0a 0966 6c61 6b65 383e  =0.910...flake8>
+00000450: 3d33 2e39 0d0a 0974 6f78 3e3d 332e 3234  =3.9...tox>=3.24
+00000460: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
+00000470: 6b61 6765 5f64 6174 615d 0d0a 6564 6d70  kage_data]..edmp
+00000480: 7920 3d20 0d0a 0970 792e 7479 7065 640d  y = ...py.typed.
+00000490: 0a09 2a2e 6b76 0d0a 0d0a 5b66 6c61 6b65  ..*.kv....[flake
+000004a0: 385d 0d0a 6d61 782d 6c69 6e65 2d6c 656e  8]..max-line-len
+000004b0: 6774 6820 3d20 3136 300d 0a0d 0a5b 6567  gth = 160....[eg
+000004c0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+000004d0: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+000004e0: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `edm-arch-1.0.27/src/edm_arch.egg-info/SOURCES.txt` & `edm-arch-1.0.32/src/edm_arch.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -7,17 +7,23 @@
 src/edm_arch.egg-info/SOURCES.txt
 src/edm_arch.egg-info/dependency_links.txt
 src/edm_arch.egg-info/not-zip-safe
 src/edm_arch.egg-info/requires.txt
 src/edm_arch.egg-info/top_level.txt
 src/edmpy/__init__.py
 src/edmpy/__main__.py
+src/edmpy/cfg.py
+src/edmpy/constants.py
+src/edmpy/db.py
 src/edmpy/edm.kv
 src/edmpy/edm.py
+src/edmpy/geo.py
+src/edmpy/ini.py
 src/edmpy/py.typed
+src/edmpy/totalstation.py
 src/edmpy/lib/__init__.py
 src/edmpy/lib/blockdata.py
 src/edmpy/lib/colorscheme.py
 src/edmpy/lib/constants.py
 src/edmpy/lib/dbs.py
 src/edmpy/lib/e5_widgets.py
 src/edmpy/lib/misc.py
```

### Comparing `edm-arch-1.0.27/src/edmpy/edm.kv` & `edm-arch-1.0.32/src/edmpy/edm.kv`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,18 @@
                         on_press: app.root.current = 'CFGScreen'
                         color: SUBMENU_COLOR
                     ActionButton:
                         text: 'INI'
                         on_press: app.root.current = 'INIScreen'
                         color: SUBMENU_COLOR
                     ActionButton:
+                        text: 'JSON'
+                        on_press: app.root.current = 'JSONScreen'
+                        color: SUBMENU_COLOR
+                    ActionButton:
                         text: 'About'
                         on_press: app.root.current = 'AboutScreen'
                         color: SUBMENU_COLOR
                 ActionGroup:
                     text: 'Delete'
                     color: SUBMENU_COLOR
                     background_color: (.5, .5, .5, 1)
@@ -135,14 +139,18 @@
                         text: 'Verify Station'
                         on_press: app.root.current = 'VerifyStationScreen'
                         color: SUBMENU_COLOR
                     ActionButton:
                         text: 'Record Datums'
                         on_press: app.root.current = 'RecordDatumsScreen'
                         color: SUBMENU_COLOR
+                    ActionButton:
+                        text: 'Options'
+                        on_press: app.root.current = 'OptionsScreen'
+                        color: SUBMENU_COLOR
                 ActionGroup:
                     text: 'File'
                     color: SUBMENU_COLOR
                     background_color: (.5, .5, .5, 1)
                     background_normal: ''
                     ActionButton:
                         text: 'Default CFG'
@@ -169,15 +177,14 @@
                     ActionButton:
                         text: 'Exit'
                         #on_release: app.stop()
                         on_release: root.exit_program()
                         color: SUBMENU_COLOR
 
 
-
 <e5_LoadDialog>:
     BoxLayout:
         size: root.size
         pos: root.pos
         orientation: "vertical"
         TextInput:
             size_hint: 1, None
@@ -192,27 +199,29 @@
             path: root.start_path
         BoxLayout:
             size_hint_y: None
             spacing: 5
             padding: 5
             Button:
                 text: "Cancel"
+                font_size: root.font_size
                 on_release: root.cancel()
                 color: root.button_color
                 background_color: root.button_background
                 background_normal: ''
             Button:
                 text: "Open"
+                font_size: root.font_size
                 on_release: root.load(filechooser.path, filechooser.selection)
                 color: root.button_color
                 background_color: root.button_background
                 background_normal: ''
 
 
-#region code from https://github.com/MichaelStott/DataframeGUIKivy/blob/master/dfguik.py
+#region code based on https://github.com/MichaelStott/DataframeGUIKivy/blob/master/dfguik.py
 
 <DataGridHeaderCell>:
     size_hint: (None, None)
     text_size: self.size
     halign: "center"
     valign: "middle"
     height: '30dp'
@@ -223,47 +232,50 @@
         Color:
             rgba: 0.165, 0.165, 0.165, 1
         Rectangle:
             pos: self.pos
             size: self.size
     on_release: root.parent.parent.parent.parent._generate_table(self.text)
 
+
 <DataGridTableHeader>:
     header: header
     bar_width: 0
     do_scroll: False
     size_hint: (1, None)
     effect_cls: "ScrollEffect"
     height: '30dp'
     GridLayout:
         id: header
         rows: 1
         size_hint: (None, None)
         width: self.minimum_width
         height: self.minimum_height
 
+
 <DataGridScrollCell>:
     canvas.before:
         #Color:
         #    rgba: root.datagrid_odd if root.is_even else root.datagrid_even
         Rectangle:
             pos: self.pos
             size: self.size
     text: root.text
     id: root.id
     on_press: root.callback(root.key, root.field, root.db)
-    background_color: root.datagrid_odd if root.is_even else root.datagrid_even
+    background_color: root.datagrid_even if root.is_even else root.datagrid_odd
     halign: "center"
     valign: "middle"
     # This setting determines if text wraps in the grid cell box
     text_size: self.size
     size_hint: 1, 1
     #height: 60
     #width: 400
 
+
 <DataGridTableData>:
     rgrid: rgrid
     scroll_type: ['bars', 'content']
     bar_color: [0.2, 0.7, 0.9, 1]
     bar_inactive_color: [0.2, 0.7, 0.9, .5]
     do_scroll_x: True
     do_scroll_y: True
@@ -273,14 +285,15 @@
         id: rgrid
         rows: root.nrows
         cols: root.ncols
         size_hint: (None, None)
         width: self.minimum_width
         height: self.minimum_height
 
+
 <DataGridWidget>:
     panel1: data_frame_panel
     panel2: edit_panel
     panel3: delete_panel
     panel4: addnew_panel
     do_default_tab: False
     TabbedPanelItem:
@@ -308,17 +321,19 @@
         DataGridAddNewPanel:
             id: addnew_panel
     TabbedPanelItem:
         text: 'Close'
         on_release: root.close_panels()
         background_normal: ''
 
+
 <DataGridGridPanel>:
 #    orientation: 'vertical'
 
+
 <DataGridAddNewPanel>:
     addnew_list: addnew_list
 #    orientation: 'vertical'
     ScrollView:
         do_scroll_x: False
         do_scroll_y: True
         size_hint: 1, 1
@@ -330,26 +345,27 @@
             cols:1
             row_default_height: '35dp'
             row_force_default: True
             size_hint_y: None
 
 <DataGridCasePanel>:
     edit_list: edit_list
-#    orientation: 'vertical'
+    orientation: 'vertical'
     ScrollView:
         do_scroll_x: False
         do_scroll_y: True
         size_hint: 1, 1
         scroll_timeout: 150
         GridLayout:
             id: edit_list
             padding: "10sp"
             spacing: "5sp"
             cols:1
             row_default_height: '35dp'
             row_force_default: True
             size_hint_y: None
 
+
 <DataGridDeletePanel>:
 #    orientation: 'vertical'
 
 #endregion end code from https://github.com/MichaelStott/DataframeGUIKivy/blob/master/dfguik.py
```

### Comparing `edm-arch-1.0.27/src/edmpy/edm.py` & `edm-arch-1.0.32/src/edmpy/lib/e5_widgets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,3803 +1,3583 @@
-# To do for next version
-#   Better prism update in prism field
-#   Do unitchecking after doing an offset shot on suffix 0 points
-#   On import, integers (like Suffix) are being converted to float values
-
-# Changes version 1.0.21
-#   Tweaked the default CFG to carry unit and increment ID
-#   Changed how increment works a bit (should work properly now)
-#   Disabled multitouch to disable red dot on right mouse click
-#   Check to see if mdf or sdf file is specified (from EDMWin and EDM-Mobile).
-#       Correct to json and give warning
-#   Check to see if json file can be found
-#       If not, new empty file is created and warning given
-#   Prism height - whether menu or manual - carries between shots
-#   Prism height menu - works better with keyboard (enter key and arrow keys)
-#   A number of issues with using the program before opening a CFG fixed
-
-# Changes to version 1.0.26
-#   Changed the way saving works on editing last points
-#   Better setting focus on editing last points
-
-# EDM by Shannon McPherron
-#
-#   This is an alpha release.  I am still working on bugs and I am still implementing some features.
-#   It should be backwards compatible with EDM-Mobile and EDMWin (but there are still some issues).
-
-#   A text field can be linked to another table. [future feature]
-#   Think through making a field link to a database table (unique value is a table record)
-
-# ToDo NewPlot
-#   Read JSON file
-
-# ToDo More Longterm
-#   Add bluetooth communications
-
-# Bugs
-#   when you delete records one by one, the last one does not show as deleted (even though it is)
-#   could make menus work better with keyboard (at least with tab)
-#   there is no error checking on duplicates in datagrid edits
-#   when editing pole height after shot, offer to update Z
-
-__version__ = '1.0.27'
-__date__ = 'August, 2022'
-__program__ = 'EDM'
-__DEFAULT_FIELDS__ = ['X', 'Y', 'Z', 'SLOPED', 'VANGLE', 'HANGLE', 'STATIONX', 'STATIONY', 'STATIONZ', 'LOCALX', 'LOCALY', 'LOCALZ', 'DATE', 'PRISM', 'ID']
-__BUTTONS__ = 13
-__LASTCOMPORT__ = 16
-from edmpy.lib.constants import __SPLASH_HELP__
-
-# Region Imports
-from kivy.config import Config
-
 from kivy.core.clipboard import Clipboard
-from kivy.graphics import Color, Rectangle
-from kivy.app import App
-from kivy.factory import Factory
-from kivy.uix.popup import Popup
-from kivy.uix.screenmanager import ScreenManager, Screen
-from kivy.uix.boxlayout import BoxLayout
-from kivy.uix.spinner import Spinner
+from kivy.clock import Clock
 from kivy.uix.textinput import TextInput
-from kivy.uix.gridlayout import GridLayout
-from kivy.properties import ObjectProperty
 from kivy.uix.label import Label
 from kivy.uix.scrollview import ScrollView
-from kivy.clock import Clock
-from kivy import __version__ as __kivy_version__
+from kivy.uix.tabbedpanel import TabbedPanel
+from kivy.core.window import Window
+from kivy.uix.button import Button
+from kivy.uix.popup import Popup
+from kivy.uix.gridlayout import GridLayout
+from kivy.uix.boxlayout import BoxLayout
+from kivy.uix.screenmanager import Screen
+from kivy.uix.filechooser import FileChooserListView
+from kivy.uix.recycleview import RecycleView
+from kivy.properties import ObjectProperty, NumericProperty, StringProperty, BooleanProperty
+from kivy.uix.floatlayout import FloatLayout
+from kivy.uix.switch import Switch
+from kivy.uix.slider import Slider
+from kivy.uix.behaviors.focus import FocusBehavior
+from kivy.uix.spinner import Spinner, SpinnerOption
+from kivy.uix.progressbar import ProgressBar
 
-# The explicit mention of this package here
-# triggers its inclusions in the pyinstaller spec file.
-# It is needed for the filechooser widget.
-# The TimeZoneInfo is just to avoid a flake8 error.
-try:
-    import win32timezone
-    win32timezone.TimeZoneInfo.local()
-except ModuleNotFoundError:
-    pass
+from decimal import DivisionByZero
 
+import ntpath
 import os
-import random
+from shutil import copyfile
 from datetime import datetime
-import csv
-from math import sqrt
-from math import pi
-from math import cos
-from math import sin
-from math import acos
+from tinydb import Query, where
+import re
+import requests
+import json
+import urllib
+from threading import Thread
+from appdata import AppDataPaths
 
-from typing import List, Dict
+from lib.constants import __SPLASH_HELP__
+from lib.constants import APP_NAME
+from lib.colorscheme import ColorScheme, make_rgb, BLACK, WHITE, GOOGLE_COLORS, MIDDLE_GREY, DARK_GREY
+from lib.misc import platform_name, locate_file
 
-import re
-import string
-from platform import python_version
 
-import logging
+SCROLLBAR_WIDTH = 5
+TEXTBOX_HEIGHT = 30
 
-# My libraries for this project
-from edmpy.lib.blockdata import blockdata
-from edmpy.lib.dbs import dbs
-from edmpy.lib.e5_widgets import e5_label, e5_button, e5_MessageBox, e5_DatagridScreen, e5_RecordEditScreen, e5_side_by_side_buttons, e5_textinput, e5_scrollview_label
-from edmpy.lib.e5_widgets import edm_manual, DataGridTextBox, width_calculator, e5_SaveDialog, e5_LoadDialog, e5_PopUpMenu, e5_MainScreen, e5_InfoScreen
-from edmpy.lib.e5_widgets import e5_LogScreen, e5_CFGScreen, e5_INIScreen, e5_SettingsScreen, e5_scrollview_menu, DataGridMenuList, SpinnerOptions
-from edmpy.lib.e5_widgets import DataGridLabelAndField
-from edmpy.lib.colorscheme import ColorScheme
-from edmpy.lib.misc import restore_window_size_position, filename_only, platform_name
-
-# The database - pure Python
-from tinydb import TinyDB, Query, where
-from tinydb import __version__ as __tinydb_version__
 
-# from plyer import gps
-# from plyer import __version__ as __plyer_version__
+def width_calculator(fraction_size = .8, maximum_width = 800):
+    if Window.size[0] * fraction_size > maximum_width:
+        return maximum_width / Window.size[0]
+    else:
+        return fraction_size
 
-# from plyer import __version__ as __plyer_version__
-__plyer_version__ = 'None'
 
-# endregion
+def height_calculator(desired_size):
+    ratio = desired_size / Window.size[1]
+    if ratio > .9:
+        ratio = .9
+    return ratio
 
-from angles import r2d, d2r, deci2sexa, Angle
 
-import serial
+def set_color(popup, colors):
+    if not popup:
+        return colors.text_color if colors else make_rgb(BLACK)
+    else:
+        return colors.popup_text_color if colors else make_rgb(WHITE)
 
-if os.name == 'nt':  # sys.platform == 'win32':
-    from serial.tools.list_ports_windows import comports
-elif os.name == 'posix':
-    from serial.tools.list_ports_posix import comports
-# ~ elif os.name == 'java':
-else:
-    raise ImportError("Sorry: no implementation for your platform ('{}') available".format(os.name))
 
-# Region Data Classes
+class SpinnerOptions(SpinnerOption):
+    def __init__(self, **kwargs):
+        super(SpinnerOptions, self).__init__(**kwargs)
 
 
-class point:
-    def __init__(self, x = None, y = None, z = None):
-        self.x = x
-        self.y = y
-        self.z = z
+class e5_PopUpMenu(Popup):
+    def __init__(self, title, menu_list, message = '', menu_selected = '', call_back = None, colors = None, **kwargs):
+        super(e5_PopUpMenu, self).__init__(**kwargs)
 
-    def __str__(self):
-        return(f'X : {round(self.x, 3)}, Y : {round(self.y, 3)}, Z : {round(self.z, 3)}')
+        pop_content = GridLayout(cols = 1, size_hint_y = 1, spacing = 5, padding = 5)
 
-    def __repr__(self):
-        return(f'X : {round(self.x, 3)}, Y : {round(self.y, 3)}, Z : {round(self.z, 3)}')
+        ncols = int(Window.width / 200)
+        ncols = max(1, ncols)
 
-    def __eq__(self, other):
-        if isinstance(other, self.__class__):
-            return self.x == other.x and self.y == other.y and self.x == other.z
-        else:
-            return False
+        if message:
+            label = e5_scrollview_label(message, popup = True, colors = colors)
+            label.size_hint = (1, .2)
+            pop_content.add_widget(label)
 
-    def __ne__(self, other):
-        return not self.__eq__(other)
+        menu = e5_scrollview_menu(menu_list, menu_selected,
+                                                 widget_id = 'menu',
+                                                 call_back = [call_back],
+                                                 ncols = ncols,
+                                                 colors = colors)
+        pop_content.add_widget(menu)
+        menu.make_scroll_menu_item_visible()
 
-    def is_none(self):
-        return(self.x is None and self.y is None and self.y is None)
+        pop_content.add_widget(e5_button('Back', selected = True,
+                                                 call_back = self.dismiss,
+                                                 colors = colors))
 
-    def round(self):
-        self.x = round(self.x, 3)
-        self.y = round(self.y, 3)
-        self.z = round(self.z, 3)
-        return(self)
-
-
-class datum:
-    def __init__(self, name = None, x = None, y = None, z = None, notes = ''):
-        self.name = name if name else None
-        self.x = x
-        self.y = y
-        self.z = z
-        self.notes = notes
-
-    def as_point(self):
-        return(point(self.x, self.y, self.z))
-
-    def __str__(self):
-        return(f'Datum: {self.name} of X : {round(self.x, 3)}, Y : {round(self.y, 3)}, Z : {round(self.z, 3)}')
-
-    def __repr__(self):
-        return(f'Datum: {self.name} of X : {round(self.x, 3)}, Y : {round(self.y, 3)}, Z : {round(self.z, 3)}')
-
-    def __eq__(self, other):
-        if isinstance(other, self.__class__):
-            return self.x == other.x and self.y == other.y and self.x == other.z and self.name == other.name and self.notes == other.notes
-        else:
-            return False
+        self.content = pop_content
+        self.title = title
+        self.size_hint = (.9, .9)
+        self.auto_dismiss = True
 
-    def __ne__(self, other):
-        return not self.__eq__(other)
 
-    def is_none(self):
-        return(self.name is None and self.x is None and self.y is None and self.z is None and self.notes == '')
+class db_filter(Popup):
 
+    def __init__(self, default_field = '', fields = [], call_back = None, colors = None, **kwargs):
+        super(db_filter, self).__init__(**kwargs)
 
-class prism:
-    def __init__(self, name = None, height = None, offset = None):
-        self.name = name
-        self.height = height
-        self.offset = offset
+        spinner_dropdown_button = SpinnerOptions
+        spinner_dropdown_button.font_size = colors.button_font_size.replace("sp", '') if colors.button_font_size else None
+        spinner_dropdown_button.background_color = (0, 0, 0, 1)
 
-    def __str__(self):
-        return(f'Prism {self.name} with hieght of {round(self.height, 3)} and offset of {round(self.offset, 3)}')
+        pop_content = GridLayout(cols = 1, spacing = 5, padding = 5)
+        field_value = GridLayout(cols = 2, spacing = 5, padding = 5)
+        self.fields_dropdown = Spinner(text = default_field, values = fields,
+                                        size_hint = (.5, None),
+                                        option_cls = spinner_dropdown_button)
+        field_value.add_widget(self.fields_dropdown)
+        field_value_right = GridLayout(cols = 1, spacing = 5, padding = 5)
+        field_value_right.add_widget(e5_label('Select a field and enter a\nvalue to match in this field.', size_hint = (1, .2), halign = 'left', popup = True))
+        self.value_input = e5_textinput(size_hint = (0.75, None), id = 'value', write_tab = False)
+        self.value_input.bind(minimum_height = self.value_input.setter('height'))
+        field_value_right.add_widget(self.value_input)
+        field_value.add_widget(field_value_right)
+        pop_content.add_widget(field_value)
+        buttons = e5_side_by_side_buttons(text = ['Back', 'Apply'],
+                                            button_height = None,
+                                            id = ['back', 'apply'],
+                                            selected = [True, True],
+                                            call_back = [self.dismiss, call_back],
+                                            colors = colors)
+        pop_content.add_widget(buttons)
+        self.content = pop_content
+        self.title = 'Filter dataset'
+        self.size_hint = (.9, .38)
+
+
+class edm_manual(Popup):
+
+    def __init__(self, type = "Manual XYZ", call_back = None, colors = None, **kwargs):
+        super(edm_manual, self).__init__(**kwargs)
+
+        pop_content = GridLayout(cols = 1, spacing = 5, padding = 5)
+        if type == "Manual XYZ":
+            input = DataGridLabelAndField(col = 'X', colors = colors, popup = True)
+            input.txt.bind(on_text_validate = self.next_field)
+            self.xcoord = input.txt
+            pop_content.add_widget(input)
+            input = DataGridLabelAndField(col = 'Y', colors = colors, popup = True)
+            input.txt.bind(on_text_validate = self.next_field)
+            self.ycoord = input.txt
+            pop_content.add_widget(input)
+            input = DataGridLabelAndField(col = 'Z', colors = colors, popup = True)
+            input.txt.bind(on_text_validate = self.next_field)
+            self.zcoord = input.txt
+            pop_content.add_widget(input)
+            self.hangle = None
+            self.vangle = None
+            self.sloped = None
+        else:
+            input = DataGridLabelAndField(col = 'Horizontal angle', colors = colors, popup = True)
+            input.txt.bind(on_text_validate = self.next_field)
+            self.hangle = input.txt
+            pop_content.add_widget(input)
+            input = DataGridLabelAndField(col = 'Vertical angle', colors = colors, popup = True)
+            input.txt.bind(on_text_validate = self.next_field)
+            self.vangle = input.txt
+            pop_content.add_widget(input)
+            input = DataGridLabelAndField(col = 'Slope distance', colors = colors, popup = True)
+            input.txt.bind(on_text_validate = self.next_field)
+            self.sloped = input.txt
+            pop_content.add_widget(input)
+            self.xcoord = None
+            self.ycoord = None
+            self.zcoord = None
+        buttons = e5_side_by_side_buttons(text = ['Cancel', 'Next'],
+                                            button_height = None,
+                                            id = ['cancel', 'next'],
+                                            selected = [True, True],
+                                            call_back = [self.dismiss, call_back],
+                                            colors = colors)
+        self.call_back = call_back
+        pop_content.add_widget(buttons)
+        self.content = pop_content
+        self.title = 'Manual Input'
+        self.size_hint = (.9, height_calculator(280))
+        self.auto_dismiss = True
+
+    def on_open(self):
+        if self.xcoord is not None:
+            self.xcoord.focus = True
+        elif self.hangle is not None:
+            self.hangle.focus = True
+
+    def next_field(self, instance):
+        if instance.id in ['Slope distance', 'Z']:
+            self.call_back(instance)
+        instance.get_focus_next().focus = True
+
+
+class e5_textinput_without_clear(TextInput):
+    id = ObjectProperty('')
+    text_length = ObjectProperty(0)
 
-    def __repr__(self):
-        return(f'Prism {self.name} with hieght of {round(self.height, 3)} and offset of {round(self.offset, 3)}')
+    def __init__(self, **kwargs):
+        super(e5_textinput_without_clear, self).__init__(**kwargs)
+        if 'id' in kwargs:
+            self.id = kwargs.get('id')
+            if self.id in ['X', 'Y', 'Z', 'PRISM', 'SLOPED', 'STATIONX', 'STATIONY', 'STATIONZ', 'LOCALX', 'LOCALY', 'LOCALZ'] and APP_NAME == 'EDM':
+                self.bind(on_text_validate = self.do_coordinate_math)
+        if 'text_length' in kwargs:
+            self.text_length = kwargs.get('text_length')
+
+    def do_coordinate_math(self, instance):
+        if instance.text:
+            try:
+                self.text = str(eval(instance.text))
+            except (DivisionByZero, NameError, SyntaxError):
+                pass
 
-    def __eq__(self, other):
-        if isinstance(other, self.__class__):
-            return self.name == other.name and self.height == other.height and self.offset == other.offset
+    def insert_text(self, substring, from_undo=False):
+        if self.text_length:
+            s = '' if len(self.text) > self.text_length else substring
         else:
-            return False
+            s = substring
+        return super().insert_text(s, from_undo = from_undo)
 
-    def __ne__(self, other):
-        return not self.__eq__(other)
 
-    def is_none(self):
-        return(self.name is None and self.height is None and self.offset is None)
+class e5_textinput(GridLayout):
 
-    def valid(self):
-        if self.name == '':
-            return('A name field is required.')
-        if len(self.name) > 20:
-            return('A prism name should be 20 characters or less.')
-        if self.height == '':
-            return('A prism height is required.')
-        if float(self.height) > 10:
-            return('Prism height looks too large.  Prism heights are in meters.')
-        if self.offset == '':
-            self.offset == 0.0
-        if float(self.offset) > .2:
-            return('Prism offset looks to be too large.  Prism offsets are expressed in meters.')
-        return(True)
-
-
-class unit:
-    def __init__(self, name = None, minx = None, miny = None, maxx = None, maxy = None, centerx = None, centery = None, radius = None):
-        self.name = name
-        self.minx = minx
-        self.miny = miny
-        self.maxx = maxx
-        self.maxy = maxy
-        self.radius = radius
-        self.centerx = centerx
-        self.centery = centery
-
-    def __str__(self):
-        if not self.radius:
-            return(f'Unit {self.name} with limits ({self.minx},{self.miny})-({self.maxx},{self.maxy})')
-        else:
-            return(f'Unit {self.name} centered on ({self.centerx},{self.centery}) with a radius of {self.radius}')
-
-    def __repr__(self):
-        if not self.radius:
-            return(f'Unit {self.name} with limits ({self.minx},{self.miny})-({self.maxx},{self.maxy})')
-        else:
-            return(f'Unit {self.name} centered on ({self.centerx},{self.centery}) with a radius of {self.radius}')
-
-    def __eq__(self, other):
-        if isinstance(other, self.__class__):
-            return (self.name == other.name and self.minx == other.minx and self.miny == other.miny and self.maxx == other.maxx and self.maxy == other.maxy and self.centerx == other.centerx and self.centery == other.centery and self.radius == other.radius)
+    def __init__(self, **kwargs):
+        super(e5_textinput, self).__init__()
+
+        self.cols = 2
+        self.spacing = 0
+        self.size_hint = (1, None)
+        self.height = TEXTBOX_HEIGHT
+
+        self.textbox = e5_textinput_without_clear(**kwargs, height = 30)
+        # self.textbox.bind(text = self.update_text)
+        # self.text = self.textbox.text
+        self.add_widget(self.textbox)
+
+        self.clear_button = Button(text = 'X', width = TEXTBOX_HEIGHT,
+                                    size_hint=(None, None), height = TEXTBOX_HEIGHT,
+                                    background_normal = '',
+                                    background_color = (.2, .2, .2, 1),
+                                    on_press = self.clear_text_box)
+        self.add_widget(self.clear_button)
+
+    # def update_text(self, instance, value):
+    #     self.text = instance.text
+
+    def clear_text_box(self, instance):
+        self.textbox.text = ''
+
+
+class e5_label(Label):
+    id = ObjectProperty('')
+
+    def __init__(self, text, popup = False, colors = None, label_height = None, **kwargs):
+        super(e5_label, self).__init__(**kwargs)
+        self.text = text
+        self.color = set_color(popup, colors)
+        if colors:
+            if colors.text_font_size:
+                self.font_size = colors.text_font_size
+        if label_height is None:
+            self.bind(size = self.setter('text_size'))
+        # else:
+        #     self.height = label_height
+        self.height = 30 if label_height is None else label_height
+        self.valign = 'center'
+
+
+class e5_label_wrapped(e5_label):
+    def __init__(self, text, popup = False, colors = None, **kwargs):
+        super(e5_label_wrapped, self).__init__(text, popup = False, colors = None, **kwargs)
+        self.size_hint = (1, None)
+        self.bind(width = lambda *x: self.setter('text_size')(self, (self.width, None)),
+                                texture_size=lambda *x: self.setter('height')(self, self.texture_size[1]))
+
+
+class e5_side_by_side_buttons(GridLayout):
+    def __init__(self, text,
+                    id = ['', ''], selected = [False, False],
+                    call_back = [None, None], button_height = None, colors = None, **kwargs):
+        super(e5_side_by_side_buttons, self).__init__(**kwargs)
+        self.cols = len(id)
+        self.spacing = 5
+        self.size_hint_y = button_height
+        # self.height = button_height
+        for i in range(len(id)):
+            self.add_widget(e5_button(text[i],
+                            id = id[i],
+                            selected = selected[i], call_back = call_back[i],
+                            button_height = button_height, colors = colors))
+
+
+class e5_button(FocusBehavior, Button):
+    id = ObjectProperty('')
+
+    def __init__(self, text,
+                    id = '',
+                    selected = False, call_back = None, on_focus = None,
+                    button_height = None, colors = None, **kwargs):
+        super(e5_button, self).__init__(**kwargs)
+        self.colors = colors
+        self.text = text
+        self.size_hint_y = button_height
+        self.id = id
+        if colors:
+            if colors.button_font_size:
+                self.font_size = colors.button_font_size
+        self.color = colors.button_color if colors else make_rgb(WHITE)
+        if colors:
+            self.background_color = colors.button_background if selected else colors.optionbutton_background
         else:
-            return False
+            self.background_color = make_rgb(GOOGLE_COLORS['light blue'][2 if selected else 0])
+        if call_back:
+            self.bind(on_press = call_back)
+        self.background_normal = ''
+        self.call_back = call_back
 
-    def __ne__(self, other):
-        return not self.__eq__(other)
+    def on_focus(self, instance, value, *largs):
+        if self.background_color and self.colors:
+            self.background_color = self.colors.button_background if self.focus else self.colors.optionbutton_background
 
-    def is_none(self):
-        return(self.name is None and self.minx is None and self.miny is None and self.maxx is None and self.maxy is None and self.radius is None and self.centerx is None and self.centery is None)
 
-    def is_valid(self):
-        if self.name == '' or self.name is None:
-            return('A name field is required.')
-        if len(self.name) > 20:
-            return('A unit name should be 20 characters or less.')
-        if self.minx is not None and self.maxx is not None:
-            if self.minx >= self.maxx:
-                return('The unit X2 coordinate must be larger than the X1 coordinate.')
-        if self.miny is not None and self.maxy is not None:
-            if self.miny >= self.maxy:
-                return('The unit Y2 coordinate must be larger than the Y1 coordinate.')
-        return(True)
-
-
-class DB(dbs):
-    MAX_FIELDS = 30
-    db = None
-    filename = None
-    db_name = 'points'
-    new_data = {}  # type: Dict[str, bool]
-
-    def __init__(self, filename = ''):
-        self.filename = filename
-        if self.filename:
-            self.db = TinyDB(self.filename)
+class e5_scrollview_menu(ScrollView):
+    id = ObjectProperty(None)
+    scrollbox = ObjectProperty(None)
+    menu_selected_widget = None
 
-    def open(self, filename):
-        try:
-            if self.valid_format(filename):
-                self.db = TinyDB(filename)
-                self.filename = filename
-                self.prisms = self.db.table('prisms')
-                self.new_data['prisms'] = True
-                self.units = self.db.table('units')
-                self.new_data['units'] = True
-                self.datums = self.db.table('datums')
-                self.new_data['datums'] = True
-                logger = logging.getLogger(__name__)
-                logger.info('Database ' + filename + ' opened.')
-                return(True)
-            else:
-                return(False)
-        except FileNotFoundError:
-            return(False)
+    def __init__(self, menu_list, menu_selected, widget_id = '', call_back = [None], ncols = 1, colors = None, **kwargs):
+        super(e5_scrollview_menu, self).__init__(**kwargs)
+        self.colors = colors
+        self.scrollbox = GridLayout(cols = ncols,
+                                    size_hint_y = None,
+                                    spacing = 5)
+        self.scrollbox.bind(minimum_height = self.scrollbox.setter('height'))
 
-    def create_defaults(self):
-        pass
+        self.menu_selected_widget = None
+        if menu_list:
+            if len(call_back) == 1:
+                call_back = call_back * len(menu_list)
+            for menu_item in menu_list:
+                menu_button = e5_button(menu_item, menu_item,
+                                        selected = (menu_item == menu_selected),
+                                        call_back = call_back[menu_list.index(menu_item)],
+                                        colors = colors)
+                menu_button.halign = 'center'
+                menu_button.bind(size = self.set_text_width)
+                self.scrollbox.add_widget(menu_button)
+                if menu_item == menu_selected:
+                    self.menu_selected_widget = menu_button
+        else:
+            self.scrollbox.add_widget(Button(text = '',
+                                             background_normal = ''))
+        self.size_hint = (1, 1)
+        self.id = widget_id + '_scroll'
+        self.add_widget(self.scrollbox)
 
-    def get_unitid(self, unitid):
-        unit, id = unitid.split('-')
-        p = self.db.search((where('unit') == unit) & (where('id') == id)) if self.db else None
-        if p:
-            return(p)
-        else:
-            return(None)
-
-    def get_datum(self, name = None):
-        p = self.get_by_name('datums', name)
-        return(datum(p['NAME'] if 'NAME' in p.keys() else None,
-                        float(p['X']) if 'X' in p.keys() else None,
-                        float(p['Y']) if 'Y' in p.keys() else None,
-                        float(p['Z']) if 'Z' in p.keys() else None,
-                        p['NOTES'] if 'NOTES' in p.keys() else ''))
-
-    def get_unit(self, name):
-        p = self.get_by_name('units', name)
-        return(unit(name = p['NAME'] if 'NAME' in p.keys() else None,
-                    minx = float(p['MINX']) if 'MINX' in p.keys() else None,
-                    miny = float(p['MINY']) if 'MINY' in p.keys() else None,
-                    maxx = float(p['MAXX']) if 'MAXX' in p.keys() else None,
-                    maxy = float(p['MAXY']) if 'MAXY' in p.keys() else None,
-                    centerx = float(p['CENTERX']) if 'CENTERX' in p.keys() else None,
-                    centery = float(p['CENTERY']) if 'CENTERY' in p.keys() else None,
-                    radius = float(p['RADIUS']) if 'RADIUS' in p.keys() else None))
-
-    def get_prism(self, name):
-        p = self.get_by_name('prisms', name)
-        return(prism(p['NAME'] if 'NAME' in p.keys() else None,
-                        float(p['HEIGHT']) if 'HEIGHT' in p.keys() else None,
-                        float(p['OFFSET']) if 'OFFSET' in p.keys() else None))
-
-    def get_by_name(self, table = None, name = None):
-        if table is not None and name is not None and self.db is not None:
-            item = Query()
-            p = self.db.table(table).search(item.NAME.matches('^' + name + '$', flags = re.IGNORECASE))
-            if p != []:
-                return(p[0])
-        return({})
-
-    def delete_unit(self, name = None):
-        return(self.delete_by_name('units', name))
-
-    def delete_prism(self, name = None):
-        return(self.delete_by_name('prisms', name))
-
-    def delete_datum(self, name = None):
-        return(self.delete_by_name('datums', name))
-
-    def delete_by_name(self, table = None, name = None):
-        if name is not None and table is not None and self.db is not None:
-            item = Query()
-            self.db.table(table).remove(item.NAME.matches('^' + name + '$', flags = re.IGNORECASE))
-            return(True)
-        return(False)
+    def set_text_width(self, instance, value):
+        instance.text_size = (instance.width, None)
 
-    def unit_ids(self):
-        return([row['UNIT'] + '-' + row['ID'] for row in self.db.table(self.table)] if self.db is not None else [])
+    def scroll_menu_clear_selected(self):
+        if self.menu_selected_widget:
+            self.menu_selected_widget.background_color = self.colors.optionbutton_background
+            self.menu_selected_widget = None
+
+    def scroll_menu_get_selected(self):
+        return self.menu_selected_widget
+
+    def scroll_menu_set_selected(self, text):
+        self.scroll_menu_clear_selected()
+        for widget in self.scrollbox.children:
+            if widget.text == text:
+                widget.background_color = self.colors.button_background
+                self.menu_selected_widget = widget
+                break
+
+    def scroll_menu_list(self):
+        menu_list = []
+        for widget in self.scrollbox.children:
+            menu_list.append(widget.text)
+        menu_list.reverse()
+        return menu_list
+        # return([widget.text for widget in self.scroll_menu.children])
+
+    def make_scroll_menu_item_visible(self):
+        if self.menu_selected_widget is not None:
+            self.scroll_to(self.menu_selected_widget)
+
+    def move_scroll_menu_item(self, ascii_code):
+        menu_list = self.scroll_menu_list()
+        if self.menu_selected_widget is not None:
+            index_no = menu_list.index(self.menu_selected_widget.text)
+        else:
+            index_no = 0
+
+        if index_no >= 0:
+            new_index = -1
+            if ascii_code == 279:
+                new_index = len(menu_list) - 1
+            elif ascii_code == 278:
+                new_index = 0
+            elif ascii_code == 273:  # Up
+                new_index = max([index_no - self.children[0].cols, 0])
+            elif ascii_code == 276:
+                new_index = max([index_no - 1, 0])
+            elif ascii_code == 274:  # Down
+                new_index = min([index_no + self.children[0].cols, len(menu_list) - 1])
+            elif ascii_code == 275:
+                new_index = min([index_no + 1, len(menu_list) - 1])
+            if new_index >= 0:
+                self.scroll_menu_set_selected(menu_list[new_index])
+                self.make_scroll_menu_item_visible()
+                # if self.get_widget_by_id('field_data'):
+                #    self.get_widget_by_id('field_data').text = menu_list[new_index]
+
+    def scroll_menu_char_match(self, match_str):
+        menu_list = self.scroll_menu_list()
+        if menu_list:
+            index_no = menu_list.index(self.scroll_menu_get_selected().text)
+
+            new_index = (index_no + 1) % len(menu_list)
+            while not new_index == index_no:
+                if menu_list[new_index].upper()[0] == match_str.upper():
+                    self.scroll_menu_set_selected(menu_list[new_index])
+                    self.make_scroll_menu_item_visible()
+                    break
+                else:
+                    new_index = (new_index + 1) % len(menu_list)
+                    # need new logic to auto select when only one case is available
 
-    def names(self, table_name):
-        return([row['NAME'] for row in self.db.table(table_name) if 'NAME' in row] if self.db is not None and table_name is not None else [])
 
-    def export_csv(self):
-        pass
+class e5_scrollview_label(ScrollView):
+    id = ObjectProperty(None)
 
-    def delete_record(self):
-        pass
+    def __init__(self, text, widget_id = '', popup = False, colors = None, **kwargs):
+        super(e5_scrollview_label, self).__init__(**kwargs)
+        self.colors = colors if colors else ColorScheme()
+        self.text = text
+        scrollbox = GridLayout(cols = 1,
+                                size_hint_y = None,
+                                spacing = 5)
+        scrollbox.bind(minimum_height = scrollbox.setter('height'))
+
+        self.scrolling_label = e5_label(text = self.text, markup = True,
+                                        size_hint_y = None,
+                                        color = self.colors.text_color if not popup else self.colors.popup_text_color,
+                                        id = widget_id + '_label', popup = popup,
+                                        text_size = (self.width, None))
+        if colors is not None:
+            if colors.text_font_size:
+                self.scrolling_label.font_size = colors.text_font_size
+
+        self.scrolling_label.bind(texture_size=lambda instance, value: setattr(instance, 'height', value[1]))
+        self.scrolling_label.bind(width=lambda instance, value: setattr(instance, 'text_size', (value * .95, None)))
+
+        # info.bind(texture_size=lambda *x: info.setter('height')(info, info.texture_size[1]))
+        scrollbox.add_widget(self.scrolling_label)
+
+        self.bar_width = SCROLLBAR_WIDTH
+        self.size_hint = (1, 1)
+        self.id = widget_id + '_scroll'
+        self.add_widget(scrollbox)
 
-    def add_record(self):
-        pass
 
-    def distance(self, p1, a_unit):
-        return(sqrt((p1.x - a_unit.centerx)**2 + (p1.y - a_unit.centery)**2))
+class e5_MainScreen(Screen):
 
-    def point_in_unit(self, xyz = None):
-        if xyz.x is not None and xyz.y is not None:
-            for unitname in self.names('units'):
-                a_unit = self.get_unit(unitname)
-                if a_unit.is_valid() is True:
-                    if a_unit.minx is not None and a_unit.miny is not None and a_unit.maxx is not None and a_unit.maxy is not None:
-                        if xyz.x <= a_unit.maxx and xyz.x >= a_unit.minx and xyz.y <= a_unit.maxy and xyz.y >= a_unit.miny:
-                            return(a_unit.name)
-                    elif a_unit.centerx is not None and a_unit.centery is not None and not a_unit.radius == 0.0:
-                        if self.distance(xyz, a_unit) <= a_unit.radius:
-                            return(a_unit.name)
-        return(None)
-
-    def get_link_fields(self, name = None, value = None):
-        if name is not None and value is not None and self.db is not None:
-            q = Query()
-            r = self.db.table(name).search(q[name].matches('^' + value + '$', re.IGNORECASE))
-            if r != []:
-                return(r[0])
-        return(None)
-
-
-class INI(blockdata):
-
-    def __init__(self, filename = ''):
-        if filename == '':
-            filename = __program__ + '.ini'
-        self.filename = filename
-        self.incremental_backups = False
-        self.backup_interval = 0
-        self.first_time = True
-        self.debug = False
-
-    def open(self, filename = ''):
-        if filename:
-            self.filename = filename
-        self.blocks = self.read_blocks()
-        self.first_time = (self.blocks == [])
-        self.is_valid()
-        self.incremental_backups = self.get_value(__program__, 'IncrementalBackups').upper() == 'TRUE'
-        self.backup_interval = int(self.get_value(__program__, 'BackupInterval'))
-        self.debug = self.get_value(__program__, 'Debug').upper() == 'TRUE'
-
-    def is_valid(self):
-        for field_option in ['DARKMODE', 'INCREMENTALBACKUPS']:
-            if self.get_value(__program__, field_option):
-                if self.get_value(__program__, field_option).upper() == 'YES':
-                    self.update_value(__program__, field_option, 'TRUE')
-            else:
-                self.update_value(__program__, field_option, 'FALSE')
+    popup = ObjectProperty(None)
+    popup_open = False
+    event = ObjectProperty(None)
+    widget_with_focus = ObjectProperty(None)
+    text_color = (0, 0, 0, 1)
+    title = APP_NAME
+    app_paths = AppDataPaths(APP_NAME)
 
-        if self.get_value(__program__, "BACKUPINTERVAL"):
-            try:
-                test = int(self.get_value(__program__, "BACKUPINTERVAL"))
-                if test < 0:
-                    test = 0
-                elif test > 200:
-                    test = 200
-                self.update_value(__program__, 'BACKUPINTERVAL', test)
-            except ValueError:
-                self.update_value(__program__, 'BACKUPINTERVAL', 0)
-        else:
-            self.update_value(__program__, 'BACKUPINTERVAL', 0)
+    def setup_program(self):
+        warnings, errors = [], []
+        self.ini.open(self.app_paths.config_path)
+        if not self.ini.first_time:
+            if self.ini.get_value(APP_NAME, 'ColorScheme'):
+                self.colors.set_to(self.ini.get_value(APP_NAME, 'ColorScheme'))
+            if self.ini.get_value(APP_NAME, 'DarkMode').upper() == 'TRUE':
+                self.colors.darkmode = True
+            else:
+                self.colors.darkmode = False
+
+            if self.ini.get_value(APP_NAME, 'ButtonFontSize'):
+                self.colors.button_font_size = (self.ini.get_value(APP_NAME, 'ButtonFontSize'))
+            if self.ini.get_value(APP_NAME, 'TextFontSize'):
+                self.colors.text_font_size = (self.ini.get_value(APP_NAME, 'TextFontSize'))
+
+            if self.ini.get_value(APP_NAME, "CFG"):
+                has_errors, errors = self.cfg.open(self.ini.get_value(APP_NAME, "CFG"))
+                if self.cfg.filename and not has_errors:
+                    warnings, errors = self.open_db()
+            self.ini.update(self.colors, self.cfg)
+            self.ini.save()
+        self.colors.set_colormode()
+        self.colors.need_redraw = False
+        return warnings, errors
+
+    def get_path(self):
+        if self.ini.get_value(APP_NAME, "CFG"):
+            return ntpath.split(self.ini.get_value(APP_NAME, "CFG"))[0]
+        else:
+            return os.getcwd()
+
+    def get_files(self, fpath, exts = None):
+        files = []
+        for (dirpath, dirnames, filenames) in os.walk(fpath):
+            files.extend(filenames)
+            break
+        if exts:
+            return [filename for filename in files if filename.upper().endswith(exts.upper())]
+        else:
+            return files
+
+    def open_db(self):
+        warnings = []
+        errors = []
+        database = locate_file(self.cfg.get_value(APP_NAME, 'DATABASE'), self.cfg.path)
+        if not database:
+            database = os.path.split(self.cfg.filename)[1]
+            if "." in database:
+                database = database.split('.')[0]
+            database = os.path.join(self.cfg.path, database + '.json')
+            warning = f"Could not locate the data file {self.cfg.get_value(APP_NAME, 'DATABASE')} as specified in the CFG file.  "
+            warning += 'EDM looked in the specified location and also in '
+            warning += f'in the same folder as the CFG file {self.cfg.path}.  A new empty data file was created as {database}.  '
+            warning += 'If this is not correct, leave the program and alter the CFG file '
+            warning += "and/or move the data file to the correct location."
+            warnings.append(warning)
+        if database.lower().endswith('.mdb') or database.lower().endswith('.sdf'):
+            database = database[:-4] + '.json'
+            warning = 'EDM does not accept the mdb and sdf data files that were used with EDMWin and EDM-Mobile.  '
+            warning += f'A new, empty json format file has been opened in this case.  The filename is {database}.  '
+            warning += 'JSON files are human readable ASCII files.  To move your data from the old format to this program, '
+            warning += 'follow the directions found on the EDM GitHub site '
+            warning += 'https://github.com/surf3s/EDM/tree/master/Import_from_EDM-Mobile or https://github.com/surf3s/EDM/tree/master/Import_from_EDMWin.  '
+            warning += 'Basically you need to create csv files that can be imported into this program.  '
+            warning += 'EDM-Mobile will create them for you.  With EDMWin you need to create them youself.  '
+            warning += 'Alternatively, you can hand enter items like datums, units, and prisms using the various menu options under Edit.'
+            warnings.append(warning)
+        if not self.data.valid_format(database):
+            error = f'The file {database} does not load as a valid json file.  If the wrong file has been loaded, edit the CFG file to point to the '
+            error += 'correct database.  If the file is the correct one, then it appears that it has become corrupted.  Open the file in any text '
+            error += 'editor and assess the situation.  A json file is a human readable file format, and you should be able to see your data.  '
+            error += 'If you need more help fixing the problem, you can contact me.'
+            errors.append(error)
+        else:
+            self.data.open(database)
+            if self.cfg.get_value(APP_NAME, 'TABLE'):
+                self.data.table = self.cfg.get_value(APP_NAME, 'TABLE')
+            else:
+                self.data.table = '_default'
+            self.cfg.update_value(APP_NAME, 'DATABASE', self.data.filename)
+            self.cfg.update_value(APP_NAME, 'TABLE', self.data.table)
+            self.cfg.save()
+            self.data.new_data[self.data.table] = True
+        return (warnings, errors)
 
-    def update(self, colors, cfg):
-        self.update_value(__program__, 'CFG', cfg.filename)
-        self.update_value(__program__, 'ColorScheme', colors.color_scheme)
-        self.update_value(__program__, 'ButtonFontSize', colors.button_font_size)
-        self.update_value(__program__, 'TextFontSize', colors.text_font_size)
-        self.update_value(__program__, 'DarkMode', 'TRUE' if colors.darkmode else 'FALSE')
-        self.update_value(__program__, 'IncrementalBackups', self.incremental_backups)
-        self.update_value(__program__, 'BackupInterval', self.backup_interval)
-        self.save()
-
-    def save(self):
-        self.write_blocks()
-
-    def status(self):
-        txt = '\nThe INI file is %s.\n' % self.filename
-        return(txt)
-
-
-class CFG(blockdata):
-
-    class field:
-        name = ''
-        inputtype = ''
-        prompt = ''
-        length = 0
-        menu = []  # type: List[str]
-        increment = False
-        required = False
-        carry = False
-        unique = False
-        link_fields = []  # type: List[str]
-
-        def __init__(self, name):
-            self.name = name
-
-    def __init__(self, filename = ''):
-        self.initialize()
-        if filename:
-            self.filename = filename
-
-    def initialize(self):
-        self.blocks = []
-        self.filename = ""
-        self.path = ""
-        self.current_field = None
-        self.current_record = {}
-        self.BOF = True
-        self.EOF = False
-        self.has_errors = False
-        self.has_warnings = False
-        self.key_field = None   # not implimented yet
-        self.description = ''   # not implimented yet
-        self.gps = False
-        self.link_fields = []   # I think this is a holdover.  Linked fields are not associated with a particular field
-        self.errors = []
-        self.unique_together = []
-
-    def open(self, filename = ''):
-        if filename:
-            self.filename = filename
-        return(self.load())
-
-    def validate_datafield(self, data_to_insert, data_table):
-        # This just validates one field (e.g. when an existing record is edit)
-        if data_to_insert and data_table and len(data_to_insert) == 1:
-            for field, value in data_to_insert.items():
-                f = self.get(field)
-                if f.required and str(value).strip() == "":
-                    error_message = f'\nThe field {field} is set to unique or required.  Enter a value to save this record.'
-                    return(error_message)
-                if f.inputtype == 'NUMERIC':
-                    try:
-                        float(value)
-                    except ValueError:
-                        error_message = f'\nThe field {field} requires a valid number.  Correct to save this record.'
-                        return(error_message)
-                if f.unique:
-                    result = data_table.search(where(field) == value)
-                    if result:
-                        error_message = f'\nThe field {field} is set to unique and the value {value} already exists for this field in this data table.'
-                        return(error_message)
-        return(True)
-
-    def validate_datarecord(self, data_to_insert, data_table):
-        # This validates one record (e.g. one a record is about to be inserted)
-        for field in self.fields():
-            f = self.get(field)
-            if f.required:
-                if field in data_to_insert.keys():
-                    if data_to_insert[field].strip() == '':
-                        error_message = f'\nThe field {field} is set to unique or required.  Enter a value to save this record.'
-                        return(error_message)
-                else:
-                    error_message = f'\nThe field {field} is set to unique or required.  Enter a value to save this record.'
-                    return(error_message)
-            if f.inputtype == 'NUMERIC':
-                if field in data_to_insert.keys():
-                    try:
-                        float(data_to_insert[field])
-                    except ValueError:
-                        error_message = f'\nThe field {field} requires a valid number.  Correct to save this record.'
-                        return(error_message)
-            if f.unique:
-                if field in data_to_insert.keys():
-                    result = data_table.search(where(field) == data_to_insert[field])
-                    if result:
-                        error_message = f'\nThe field {field} is set to unique and the value {data_to_insert[field]} already exists for this field in this data table.'
-                        return(error_message)
-                else:
-                    error_message = f'\nThe field {field} is set to unique and a value was not provided for this field.  Unique fields require a value.'
-                    return(error_message)
+    def warnings_and_errors_popup(self, warnings, errors):
+        message_txt = '\n'
+        message_txt += ',\n\n'.join(['Warning: ' + warning for warning in warnings])
+        message_txt += ',\n\n'.join(['Error: ' + error for error in errors])
+        return e5_MessageBox('Warnings and errors', message_txt, colors = self.colors)
 
-        # TODO test to see if it is units, prisms or datums
-        # TODO create a unit, prism or datum from the dictionary using *data_to_insert
-        # TODO run the validator in whichever
-        # TODO and return results
-        return(True)
-
-    def get(self, field_name):
-        f = self.field(field_name)
-        f.inputtype = self.get_value(field_name, 'TYPE').upper()
-        f.prompt = self.get_value(field_name, 'PROMPT')
-        f.length = self.get_value(field_name, 'LENGTH')
-        menulist = self.get_value(field_name, 'MENU')
-        if menulist:
-            f.menu = self.get_value(field_name, 'MENU').split(",")
-        link_fields = self.get_value(field_name, 'LINKED')
-        if link_fields:
-            f.link_fields = link_fields.upper().split(",")
-        f.carry = self.get_value(field_name, 'CARRY').upper() == 'TRUE'
-        f.required = self.get_value(field_name, 'REQUIRED').upper() == 'TRUE'
-        f.increment = self.get_value(field_name, 'INCREMENT').upper() == 'TRUE'
-        f.unique = self.get_value(field_name, 'UNIQUE').upper() == 'TRUE'
-        if f.unique:
-            f.required = True
-        return(f)
-
-    def put(self, field_name, f):
-        self.update_value(field_name, 'PROMPT', f.prompt)
-        self.update_value(field_name, 'LENGTH', f.length)
-        self.update_value(field_name, 'TYPE', f.inputtype)
-
-    def fields(self):
-        field_names = self.names()
-        del_fields = ['EDM', 'TIME']
-        for n in range(1, __BUTTONS__):
-            del_fields.append('BUTTON%s' % n)
-        for del_field in del_fields:
-            if del_field in field_names:
-                field_names.remove(del_field)
-        return(field_names)
-
-    def clean_menu(self, menulist):
-        menulist = [item.strip() for item in menulist]
-        menulist = list(filter(('').__ne__, menulist))
-        return(menulist)
-
-    def build_prism(self):
-        self.update_value('NAME', 'Prompt', 'Name :')
-        self.update_value('NAME', 'Type', 'Text')
-        self.update_value('NAME', 'Length', 20)
-        self.update_value('NAME', 'UNIQUE', 'TRUE')
-        self.update_value('NAME', 'REQUIRED', 'TRUE')
-
-        self.update_value('HEIGHT', 'Prompt', 'Height :')
-        self.update_value('HEIGHT', 'Type', 'Numeric')
-        self.update_value('HEIGHT', 'REQUIRED', 'TRUE')
-
-        self.update_value('OFFSET', 'Prompt', 'Offset :')
-        self.update_value('OFFSET', 'Type', 'Numeric')
-
-    def build_unit(self):
-        self.update_value('NAME', 'Prompt', 'Name :')
-        self.update_value('NAME', 'Type', 'Text')
-        self.update_value('NAME', 'Length', 20)
-        self.update_value('NAME', 'UNIQUE', 'TRUE')
-        self.update_value('NAME', 'REQUIRED', 'TRUE')
-
-        self.update_value('MINX', 'Prompt', 'X Minimum :')
-        self.update_value('MINX', 'Type', 'Numeric')
-
-        self.update_value('MINY', 'Prompt', 'Y Minimum :')
-        self.update_value('MINY', 'Type', 'Numeric')
-
-        self.update_value('MAXX', 'Prompt', 'X Maximum :')
-        self.update_value('MAXX', 'Type', 'Numeric')
-
-        self.update_value('MAXY', 'Prompt', 'Y Maximum :')
-        self.update_value('MAXY', 'Type', 'Numeric')
-
-        self.update_value('RADIUS', 'Prompt', 'or enter a Radius :')
-        self.update_value('RADIUS', 'Type', 'Text')
-        self.update_value('RADIUS', 'Length', 20)
-
-        self.update_value('CENTERX', 'Prompt', 'and a Center X :')
-        self.update_value('CENTERX', 'Type', 'Numeric')
-
-        self.update_value('CENTERY', 'Prompt', 'and Center Y :')
-        self.update_value('CENTERY', 'Type', 'Numeric')
-
-    def build_datum(self):
-        self.update_value('NAME', 'Prompt', 'Name :')
-        self.update_value('NAME', 'Type', 'Text')
-        self.update_value('NAME', 'Length', 20)
-        self.update_value('NAME', 'UNIQUE', 'TRUE')
-        self.update_value('NAME', 'REQUIRED', 'TRUE')
-
-        self.update_value('X', 'Prompt', 'X :')
-        self.update_value('X', 'Type', 'Numeric')
-        self.update_value('X', 'REQUIRED', 'TRUE')
-
-        self.update_value('Y', 'Prompt', 'Y :')
-        self.update_value('Y', 'Type', 'Numeric')
-        self.update_value('Y', 'REQUIRED', 'TRUE')
-
-        self.update_value('Z', 'Prompt', 'Z :')
-        self.update_value('Z', 'Type', 'Numeric')
-        self.update_value('Z', 'REQUIRED', 'TRUE')
-
-        self.update_value('NOTES', 'Prompt', 'Note :')
-        self.update_value('NOTES', 'Type', 'Note')
-
-    def build_default(self):
-        self.update_value('UNIT', 'Prompt', 'Unit :')
-        self.update_value('UNIT', 'Type', 'Text')
-        self.update_value('UNIT', 'Length', 6)
-        self.update_value('UNIT', 'REQUIRED', 'TRUE')
-        self.update_value('UNIT', 'CARRY', 'TRUE')
-
-        self.update_value('ID', 'Prompt', 'ID :')
-        self.update_value('ID', 'Type', 'Text')
-        self.update_value('ID', 'Length', 6)
-        self.update_value('ID', 'REQUIRED', 'TRUE')
-        self.update_value('ID', 'INCREMENT', 'TRUE')
-
-        self.update_value('SUFFIX', 'Prompt', 'Suffix :')
-        self.update_value('SUFFIX', 'Type', 'Numeric')
-        self.update_value('SUFFIX', 'REQUIRED', 'TRUE')
-
-        self.update_value('LEVEL', 'Prompt', 'Level :')
-        self.update_value('LEVEL', 'Type', 'Menu')
-        self.update_value('LEVEL', 'Length', 20)
-        self.update_value('LEVEL', 'REQUIRED', 'TRUE')
-
-        self.update_value('CODE', 'Prompt', 'Code :')
-        self.update_value('CODE', 'Type', 'Menu')
-        self.update_value('CODE', 'Length', 20)
-        self.update_value('CODE', 'REQUIRED', 'TRUE')
-
-        self.update_value('EXCAVATOR', 'Prompt', 'Excavator :')
-        self.update_value('EXCAVATOR', 'Type', 'Menu')
-        self.update_value('EXCAVATOR', 'Length', 20)
-
-        self.update_value('PRISM', 'Prompt', 'Prism :')
-        self.update_value('PRISM', 'Type', 'Numeric')
-
-        self.update_value('X', 'Prompt', 'X :')
-        self.update_value('X', 'Type', 'Numeric')
-        self.update_value('X', 'REQUIRED', 'TRUE')
-
-        self.update_value('Y', 'Prompt', 'Y :')
-        self.update_value('Y', 'Type', 'Numeric')
-        self.update_value('Y', 'REQUIRED', 'TRUE')
-
-        self.update_value('Z', 'Prompt', 'Z :')
-        self.update_value('Z', 'Type', 'Numeric')
-        self.update_value('Z', 'REQUIRED', 'TRUE')
-
-        self.update_value('DATE', 'Prompt', 'Date :')
-        self.update_value('DATE', 'Type', 'Text')
-        self.update_value('DATE', 'Length', 24)
-
-        self.update_value('HANGLE', 'Prompt', 'H-angle :')
-        self.update_value('HANGLE', 'Type', 'Numeric')
-        self.update_value('HANGLE', 'REQUIRED', 'TRUE')
-
-        self.update_value('VANGLE', 'Prompt', 'V-angle :')
-        self.update_value('VANGLE', 'Type', 'Numeric')
-        self.update_value('VANGLE', 'REQUIRED', 'TRUE')
-
-        self.update_value('SLOPED', 'Prompt', 'Slope Dist. :')
-        self.update_value('SLOPED', 'Type', 'Numeric')
-        self.update_value('SLOPED', 'REQUIRED', 'TRUE')
-
-        self.update_value('EDM', 'UNIQUE_TOGETHER', 'UNIT,ID,SUFFIX')
-        self.unique_together = ['UNIT', 'ID', 'SUFFIX']
-
-    def validate(self):
-
-        self.errors = []
-        self.has_errors = False
-        self.has_warnings = False
-        field_names = self.fields()
-        self.link_fields = []
-        bad_characters = r' !@#$%^&*()?/\{}<.,.|+=~`-'
-
-        # This is a legacy issue.  Linked fields are now listed with each field.
-        unit_fields = self.get_value('EDM', 'UNITFIELDS')
-        if unit_fields:
-            unit_fields = unit_fields.upper().split(',')
-            unit_fields.remove('UNIT')
-            unit_fields = ','.join(unit_fields)
-            self.update_value('UNIT', 'LINKED', unit_fields)
-            self.delete_key('EDM', 'UNITFIELDS')
-
-        table_name = self.get_value('EDM', 'TABLE')
-        if table_name:
-            if any((c in set(bad_characters)) for c in table_name):
-                self.errors.append(f"Error: The table name {table_name} has non-standard characters in it that cause a problem in JSON files.  Do not use any of these '{bad_characters}' characters.  Change the name before collecting data.")
-                self.has_errors = True
-
-        unique_together = self.get_value('EDM', 'UNIQUE_TOGETHER')
-        if unique_together:
-            no_errors = True
-            for field_name in unique_together.split(','):
-                if field_name not in field_names:
-                    self.errors.append(f"Error: The field '{field_name}' is listed in UNIQUE_TOGETHER but does not appear as a field in the CFG file.")
-                    self.has_errors = True
-                    no_errors = False
-                    break
-            if no_errors:
-                self.unique_together = unique_together.split(',')
+    def show_popup_message(self, dt):
+        self.event.cancel()
+        if self.cfg.has_errors or self.cfg.has_warnings:
+            if self.cfg.has_errors:
+                message_text = f'\nThe following errors were found in the configuration file {self.cfg.filename} '\
+                               'and must be corrected before data entry can begin.\n\n'
+                self.cfg.filename = ''
+                title = 'CFG File Errors'
+            elif self.cfg.has_warnings:
+                self.cfg.has_warnings = False
+                message_text = '\nThough data collection can start, there are the following warnings in '\
+                                    f'the configuration file {self.cfg.filename}.\n\n'
+                title = 'Warnings'
+            message_text = message_text + '\n\n'.join(self.cfg.errors)
+        else:
+            title = APP_NAME
+            message_text = __SPLASH_HELP__
+        self.popup = e5_MessageBox(title, message_text, call_back = self.close_popup, colors = self.colors)
+        self.popup.open()
+        self.popup_open = True
+
+    def get_widget_by_id(self, id):
+        for widget in self.walk():
+            if hasattr(widget, 'id'):
+                if widget.id == id:
+                    return widget
+        return None
+
+    def get_info(self):
+        if self.cfg.current_field.infofile:
+            fname = os.path.join(self.cfg.path, self.cfg.current_field.infofile)
+            if os.path.exists(fname):
+                try:
+                    with open(fname, 'r') as f:
+                        return f.read()
+                except OSError:
+                    return f'Could not open file {fname}.'
             else:
-                self.unique_together = []
+                return f'The file {fname} does not exist.'
         else:
-            if 'UNIT' in field_names and 'ID' in field_names and 'SUFFIX' in field_names:
-                self.update_value('EDM', 'UNIQUE_TOGETHER', 'UNIT,ID,SUFFIX')
-                self.unique_together = ['UNIT', 'ID', 'SUFFIX']
-            if 'ID' in field_names and 'SUFFIX' in field_names:
-                self.update_value('EDM', 'UNIQUE_TOGETHER', 'ID,SUFFIX')
-                self.unique_together = ['ID', 'SUFFIX']
-
-        for field_name in field_names:
-            if any((c in set(bad_characters)) for c in field_name):
-                self.errors.append(f"Error: The field name '{field_name}' has non-standard characters in it that cause a problem in JSON files.  Do not use any of these '{bad_characters}' characters.  Change the name before collecting data.")
-                self.has_errors = True
-            f = self.get(field_name)
-            if f.prompt == '':
-                f.prompt = field_name
-            f.inputtype = f.inputtype.upper()
-            if field_name in ['UNIT', 'ID', 'SUFFIX', 'X', 'Y', 'Z']:
-                self.update_value(field_name, 'REQUIRED', 'TRUE')
-            if field_name == 'ID':
-                self.update_value(field_name, 'INCREMENT', 'TRUE')
-            if f.link_fields:
-                self.link_fields.append(field_name)
-                # uppercase the link fields
-                for link_field_name in f.link_fields:
-                    if link_field_name not in field_names:
-                        self.errors.append(f"Error: The field {field_name} is set to link to {link_field_name} but the field {link_field_name} does not exist in the CFG.")
-                        self.has_errors = True
-            self.put(field_name, f)
-
-            for field_option in ['UNIQUE', 'CARRY', 'INCREMENT', 'REQUIRED', 'SORTED']:
-                if self.get_value(field_name, field_option):
-                    if self.get_value(field_name, field_option).upper() == 'YES':
-                        self.update_value(field_name, field_option, 'TRUE')
-
-        # Every CFG should have a unique together so that duplicates can be avoided
-        if self.unique_together == []:
-            for field_name in field_names:
-                f = self.get(field_name)
-                if f.unique is True:
-                    self.unique_together = [f.name]
-                    if 'SUFFIX' in field_names:
-                        self.unique_together.append('SUFFIX')
-                    self.update_value('EDM', 'UNIQUE_TOGETHER', ','.join(self.unique_together))
-                    break
+            return self.cfg.current_field.info
 
-        if self.unique_together == []:
-            self.errors.append('Every CFG file should contain at least one field or a set of fields that together are unique.  Normally, this will be something like Unit, ID and Suffix together.  Set this value by either setting one field to UNIQUE=TRUE or by adding a UNIQUE_TOGETHER line in the EDM block of the CFG file (e.g. something like UNIQUE_TOGETHER=UNIT,ID,SUFFIX).')
-            self.has_errors = True
-
-        return(self.has_errors)
-
-    def save(self):
-        self.write_blocks()
-
-    def load(self, filename = ''):
-        if filename:
-            self.filename = filename
-        self.path = os.path.split(self.filename)[0]
-
-        self.blocks = []
-        if os.path.isfile(self.filename):
-            self.blocks = self.read_blocks()
-            errors = self.validate()
-            if errors is False:     # This is bad.  Errors returned are not dealt with when starting program
-                self.save()
-            else:
-                return(errors)
-        else:
-            self.filename = 'default.cfg'
-            self.build_default()
-        logger = logging.getLogger(__name__)
-        logger.info('CFG ' + self.filename + ' opened.')
-
-    def status(self):
-        txt = '\nCFG file is %s\n' % self.filename
-        return(txt)
-
-    def write_csvs(self, filename, table):
-        # This routine could be shortened with Python libraries, however,
-        # It is written this way to ensure a proper CSV even if users
-        # change their CFG part way through data collection
-        # (meaning that the CFG and the JSON datafile do not perfectly match)
-        try:
-            cfg_fields = self.fields()
-            f = open(filename, 'w')
-            csv_row = ''
-            for fieldname in cfg_fields:
-                csv_row += ',"%s"' % fieldname if csv_row else '"%s"' % fieldname
-            f.write(csv_row + '\n')
-            for row in table:
-                csv_row = ''
-                for fieldname in cfg_fields:
-                    if fieldname in row.keys():
-                        if row[fieldname] is not None:
-                            if self.get(fieldname).inputtype in ['NUMERIC', 'INSTRUMENT']:
-                                csv_row += ',%s' % row[fieldname] if csv_row else "%s" % row[fieldname]
-                            else:
-                                csv_row += ',"%s"' % row[fieldname] if csv_row else '"%s"' % row[fieldname]
-                        else:
-                            if self.get(fieldname).inputtype in ['NUMERIC', 'INSTRUMENT']:
-                                if csv_row:
-                                    csv_row = csv_row + ','     # Not sure this works if there is an entirely empty row of numeric values
-                            else:
-                                if csv_row:
-                                    csv_row = csv_row + ',""'
-                                else:
-                                    csv_row = '""'
-                    else:
-                        if self.get(fieldname).inputtype in ['NUMERIC', 'INSTRUMENT']:
-                            if csv_row:
-                                csv_row = csv_row + ','     # Not sure this works if there is an entirely empty row of numeric values
-                        else:
-                            if csv_row:
-                                csv_row = csv_row + ',""'
-                            else:
-                                csv_row = '""'
-                f.write(csv_row + '\n')
-            f.close()
-            return(None)
-        except OSError:
-            return('\nCould not write data to %s.' % (filename))
+    def save_window_location(self):
+        self.ini.update_value(APP_NAME, 'ScreenTop', max(Window.top, 0))
+        self.ini.update_value(APP_NAME, 'ScreenLeft', max(Window.left, 0))
+        self.ini.update_value(APP_NAME, 'ScreenWidth', Window.size[0])
+        self.ini.update_value(APP_NAME, 'ScreenHeight', Window.size[1])
+        self.ini.save()
 
-    def write_geojson(self, filename, table):
-        try:
-            cfg_fields = self.fields()
-            basename = os.path.basename(filename)
-            basename = os.path.splitext(basename)[0]
-            f = open(filename, 'w')
-            geojson_header = '{\n'
-            geojson_header += '"type": "FeatureCollection",\n'
-            geojson_header += '"name": "%s",\n' % basename
-            geojson_header += '"features": [\n'
-            f.write(geojson_header)
-            row_comma = ''
-            for row in table:
-                geojson_row = row_comma + '{ "type": "Feature", "properties": {'
-                comma = ' '
-                for fieldname in cfg_fields:
-                    if fieldname in row.keys():
-                        if row[fieldname] != '':
-                            geojson_row += comma + '"%s": ' % fieldname
-                            if self.get(fieldname).inputtype in ['NUMERIC', 'INSTRUMENT']:
-                                geojson_row += '%s' % row[fieldname]
-                            else:
-                                geojson_row += '"%s"' % row[fieldname]
-                            comma = ', '
-                geojson_row += ' },\n'
-                geojson_row += '"geometry": { "type": "Point", "coordinates": [ '
-                geojson_row += '%s , %s' % self.get_XY(row)
-                geojson_row += '] } }'
-                f.write(geojson_row)
-                row_comma = ',\n'
-            f.write('\n]\n}')
-            f.close()
-            return(None)
-        except:
-            return('\nCould not write data to %s.' % (filename))
-
-    def get_XY(self, row):
-        cfg_fields = self.fields()
-        if 'X' in cfg_fields and 'Y' in cfg_fields:
-            return((row['X'], row['Y']))
-        elif 'LATITUDE' in cfg_fields and 'LONGITUDE' in cfg_fields:
-            return((row['LONGITUDE'], row['LATITUDE']))
-        elif self.gps_field(row):
-            gps_data = self.gps_to_dict(self.gps_field(row))
-            return((gps_data['Lon'], gps_data['Lat']))
-        else:
-            return((0, 0))
-
-    def gps_field(self, row):
-        for fieldname in self.fields():
-            field = self.get(fieldname)
-            if field.inputtype in ['GPS']:
-                return(row[fieldname])
-        return('')
-
-    def gps_to_dict(self, delimited_data):
-        dict_data = {}
-        for item in delimited_data.split(','):
-            dict_item = item.split('=')
-            dict_data[dict_item[0].strip()] = dict_item[1].strip()
-        return(dict_data)
+    def open_popup(self):
+        self.popup_open = False
+        self.popup.open()
+
+    def dismiss_popup(self, *args):
+        self.popup_open = False
+        if self.popup:
+            self.popup.dismiss()
+        if self.parent:
+            self.parent.current = 'MainScreen'
+
+    def save_record(self):
+        valid = self.cfg.validate_current_record()
+        if valid:
+            if self.data.save(self.cfg.current_record):
+                self.make_backup()
+            else:
+                pass
+        else:
+            self.popup = e5_MessageBox('Save Error', valid, call_back = self.close_popup, colors = self.colors)
+            self.popup.open()
+            self.popup_open = True
+
+    def make_backup(self):
+        if self.ini.backup_interval > 0:
+            try:
+                record_counter = int(self.cfg.get_value(APP_NAME, 'RECORDS UNTIL BACKUP')) \
+                    if self.cfg.get_value(APP_NAME, 'RECORDS UNTIL BACKUP') else self.ini.backup_interval
+                record_counter -= 1
+                if record_counter <= 0:
+                    backup_path, backup_file = os.path.split(self.data.filename)
+                    backup_file, backup_file_ext = backup_file.split('.')
+                    backup_file += self.datetime_stamp() if self.ini.incremental_backups else '_backup'
+                    backup_file += "." + backup_file_ext
+                    backup_file = os.path.join(backup_path, backup_file)
+                    copyfile(self.data.filename, backup_file)
+                    record_counter = self.ini.backup_interval
+                self.cfg.update_value(APP_NAME, 'RECORDS UNTIL BACKUP', str(record_counter))
+            except OSError:
+                self.popup = e5_MessageBox('Backup Error', "\n An error occurred while attempting to make a backup.  "
+                                            "Check the backup settings and that the disk has enough space for a backup.",
+                                            call_back = self.close_popup, colors = self.colors)
+                self.popup.open()
+                self.popup_open = True
 
+    def date_stamp(self):
+        date_stamp = '%s' % datetime.now().replace(microsecond=0)
+        date_stamp = date_stamp.split(' ')[0]
+        date_stamp = date_stamp.replace('-', '_')
+        return '_' + date_stamp
+
+    def datetime_stamp(self):
+        time_stamp = '%s' % datetime.now().replace(microsecond=0)
+        time_stamp = time_stamp.replace('-', '_')
+        time_stamp = time_stamp.replace(' ', '_')
+        time_stamp = time_stamp.replace(':', '_')
+        return '_' + time_stamp
 
-class totalstation(object):
+    def close_popup(self, value):
+        self.popup.dismiss()
+        self.popup_open = False
+        self.event = Clock.schedule_once(self.set_focus, 1)
 
-    popup = ObjectProperty(None)
-    popup_open = False
-    # rotate_source = []
-    # rotate_destination = []
+    def set_focus(self, value):
+        self.widget_with_focus.focus = True
 
-    def __init__(self, make = None, model = None):
-        self.make = make if make else 'Manual XYZ'
-        self.model = model
-        self.communication = 'Serial'
-        self.comport = 'COM1'
-        self.baudrate = '1200'
-        self.parity = 'EVEN'
-        self.databits = 7
-        self.stopbits = 1
-        self.comport_settings = ''
-        self.serialcom = serial.Serial()
-        self.input_string = ''
-        self.output_string = ''
-        self.port_open = False
-        self.location = point(0, 0, 0)
-        self.xyz = point()
-        self.prism_constant = 0.0
-        self.hangle = None              # Decimal degrees
-        self.vangle = None              # Decimal degrees
-        self.sloped = 0.0
-        self.suffix = 0
-        self.prism = prism()
-        self.xyz_global = point()
-        self.rotate_local = []
-        self.rotate_global = []
-        self.last_setup_type = ''
-        self.shot_type = ''
-        self.event = None
-        self.io = ''
-        self.open()
-
-    def text_to_point(self, txt):
-        if len(txt.split(',')) == 3:
-            x, y, z = txt.split(',')
-            try:
-                return(point(float(x), float(y), float(z)))
-            except Exception:
-                return(None)
-        else:
-            return(None)
-
-    def setup(self, ini, data):
-        if ini.get_value(__program__, 'STATION'):
-            self.make = ini.get_value(__program__, 'STATION')
-        if ini.get_value(__program__, 'COMMUNICATIONS'):
-            self.communication = ini.get_value(__program__, 'COMMUNICATIONS')
-        if ini.get_value(__program__, 'COMPORT'):
-            self.comport = ini.get_value(__program__, 'COMPORT')
-        if ini.get_value(__program__, 'BAUDRATE'):
-            self.baudrate = ini.get_value(__program__, 'BAUDRATE')
-        if ini.get_value(__program__, 'PARITY'):
-            self.parity = ini.get_value(__program__, 'PARITY')
-        if ini.get_value(__program__, 'DATABITS'):
-            self.databits = ini.get_value(__program__, 'DATABITS')
-        if ini.get_value(__program__, 'STOPBITS'):
-            self.stopbits = ini.get_value(__program__, 'STOPBITS')
-
-        self.last_setup_type = ini.get_value('SETUPS', 'LASTSETUP_TYPE')
-
-        if ini.get_value('SETUPS', '3DATUM_SHIFT_LOCAL_1'):
-            point1 = self.text_to_point(ini.get_value('SETUPS', '3DATUM_SHIFT_LOCAL_1'))
-            point2 = self.text_to_point(ini.get_value('SETUPS', '3DATUM_SHIFT_LOCAL_2'))
-            point3 = self.text_to_point(ini.get_value('SETUPS', '3DATUM_SHIFT_LOCAL_3'))
-            if point1 is not None and point2 is not None and point3 is not None:
-                self.rotate_local = [point1, point2, point3]
-        if ini.get_value('SETUPS', '3DATUM_SHIFT_GLOBAL_1'):
-            point1 = data.get_datum(ini.get_value('SETUPS', '3DATUM_SHIFT_GLOBAL_1'))
-            point2 = data.get_datum(ini.get_value('SETUPS', '3DATUM_SHIFT_GLOBAL_2'))
-            point3 = data.get_datum(ini.get_value('SETUPS', '3DATUM_SHIFT_GLOBAL_3'))
-            if point1 is not None and point2 is not None and point3 is not None:
-                self.rotate_global = [point1.as_point(), point2.as_point(), point3.as_point()]
-
-    def status(self):
-        txt = '\nTotal Station:\n'
-        txt += '  Make is %s\n' % self.make
-        if self.make not in ['Microscribe']:
-            txt += '  Communication type is %s\n' % self.communication
-            txt += '  COM Port is %s\n' % self.comport
-            txt += '  Com settings are %s, %s, %s, %s\n' % (self.baudrate, self.parity, self.databits, self.stopbits)
-            if self.serialcom.is_open:
-                txt += 'COM Port is open\n'
-            else:
-                txt += 'COM port is closed\n'
-            txt += '  Station was initialized with %s\n' % self.last_setup_type
-            txt += '  Station X : %s\n' % self.location.x
-            txt += '  Station Y : %s\n' % self.location.y
-            txt += '  Station Z : %s\n' % self.location.z
-        else:
-            if self.last_setup_type:
-                txt += '  Station was initialized with %s\n' % self.last_setup_type
-                n = 1
-                for coordinates in self.rotate_local:
-                    txt += '    Datum %s locally is %s, %s, %s\n' % (n, coordinates.x, coordinates.y, coordinates.z)
-                    n += 1
-                n = 1
-                for coordinates in self.rotate_global:
-                    txt += '    Datum %s globally is %s, %s, %s\n' % (n, coordinates.x, coordinates.y, coordinates.z)
-                    n += 1
-        return(txt)
-
-    def prism_adjust(self):
-        if self.prism.height is not None:
-            if self.xyz.z is not None:
-                self.xyz.z = round(self.xyz.z - self.prism.height, 3)
-            if self.xyz_global.z is not None:
-                self.xyz_global.z = round(self.xyz_global.z - self.prism.height, 3)
-
-    def angle_between_points(self, p1, p2):
-        return self.angle_between_xy_pairs(p1.x, p1.y, p2.x, p2.y)
-
-    def angle_between_xy_pairs(self, x1, y1, x2, y2):
-        # angle is from xy1 to xy2
-        # result is in decimal degrees
-        # angle is clockwise survey angle with positive y = 90
-
-        # Subtract point 1 from 2 to make 2 relative to the origin
-        p = self.subtract_points(point(x2, y2, 0), point(x1, y1, 0))
-
-        # Get the angle between the Y axis and this point
-        cos_of_angle = self.dot_product(point(0, 1, 0), self.normalize_vector(p))
-        angle = r2d(acos(cos_of_angle))
-
-        if p.x < 0:
-            angle = 360 - angle
-
-        return(angle)
-
-    def parseangle(self, hangle):
-        hangle = str(hangle)
-        if hangle.find("."):
-            angle = int(hangle)
-            minutes = 0
-            seconds = 0
-        else:
-            hangle = hangle + "0000"
-            angle = hangle.split(".")[0]
-            minutes = hangle.split(".")[1][0:2]
-            seconds = hangle.split(".")[1][2:4]
-
-        return([angle, minutes, seconds])
-
-    def point_pretty(self, point):
-        return(f'X: {round(point.x, 3)}\nY: {round(point.y, 3)}\nZ: {round(point.z, 3)}')
-
-    def decimal_degrees_to_dddmmss(self, angle):
-        if angle is not None:
-            sexa = deci2sexa(angle)
-            return(f'{sexa[1]}.{sexa[2]}{sexa[3]}')
-        else:
-            return('')
-
-    def decimal_degrees_to_sexa_pretty(self, angle):
-        if angle is not None:
-            sexa = deci2sexa(angle)
-            return(f'{sexa[1]}° {sexa[2]}\" {sexa[3]}\'')
-        else:
-            return('')
-
-    def vhd_to_sexa_pretty_compact(self):
-        return(f"hangle : {self.decimal_degrees_to_sexa_pretty(self.hangle)}, vangle : {self.decimal_degrees_to_sexa_pretty(self.vangle)}, sloped : {round(self.sloped, 3) if self.sloped else ''}")
-
-    def add_points(self, p1, p2):
-        return point(p1.x + p2.x, p1.y + p2.y, p1.z + p2.z)
-
-    def subtract_points(self, p1, p2):
-        return point(p1.x - p2.x, p1.y - p2.y, p1.z - p2.z)
-
-    def hash(self, hashlen = 5):
-        hash = ""
-        for a in range(0, hashlen):
-            hash += random.choice(string.ascii_uppercase)
-        return(hash)
-
-    def set_horizontal_angle(self, angle):
-        if self.make == 'TOPCON':
-            self.set_horizontal_angle_topcon(angle)
-        elif self.make in ['WILD', 'Leica']:
-            self.set_horizontal_angle_leica(angle)
-        elif self.make == 'SOKKIA':
-            self.set_horizontal_angle_sokkia(angle)
-        elif self.make == 'Simulate':
-            pass
-        elif self.make in ['Manual XYZ', 'Manual VHD']:
-            pass
-
-    def set_horizontal_angle_nikon(self, angle):
-        # need to send to station in format dddmmss
-        self.send("!HAN" + angle.encode())
-        # delay(1)
-        self.clear_com()
-
-    def launch_point_simulate(self):
-        # Put the points into one of two units
-        if random.uniform(0, 1) > 0.5:
-            self.xyz = point(round(random.uniform(1000, 1001), 3),
-                                round(random.uniform(1000, 1001), 3),
-                                round(random.uniform(0, 1), 3))
-        else:
-            self.xyz = point(round(random.uniform(2000, 2001), 3),
-                                round(random.uniform(2000, 2001), 3),
-                                round(random.uniform(0, 1), 3))
-        self.make_global()
-        self.vhd_from_xyz()
-
-    def take_shot(self):
-
-        self.clear_xyz()
-        self.clear_com()
-
-        if self.make == 'TOPCON':
-            self.launch_point_topcon()
-
-        elif self.make in ['WILD', 'Leica']:
-            self.launch_point_leica()
-
-        elif self.make == "SOKKIA":
-            self.launch_point_sokkia()
-
-        elif self.make == 'Simulate':
-            self.launch_point_simulate()
-
-        else:
-            pass
-
-    def fetch_point(self):
-        if self.make in ['WILD', 'Leica']:
-            self.fetch_point_leica()
-
-    def vhd_from_xyz(self):
-        self.hangle = self.angle_between_xy_pairs(self.location.x, self.location.y, self.xyz.x, self.xyz.y)
-        level_distance = sqrt((self.xyz.x - self.location.x)**2 + (self.xyz.y - self.location.y)**2)
-        self.sloped = self.distance(self.location, self.xyz)
-        self.vangle = self.angle_between_xy_pairs(0, 0, level_distance, self.xyz.z)
-
-    def make_global(self):
-        if self.xyz.x is not None and self.xyz.y is not None and self.xyz.z is not None:
-            if self.make == 'Microscribe':
-                if len(self.rotate_local) == 3 and len(self.rotate_global) == 3:
-                    self.xyz_global = self.rotate_point(self.xyz)
-                else:
-                    self.xyz_global = self.xyz
-                self.round_xyz()
+    def show_delete_last_object(self):
+        last_record = self.data.last_record()
+        if last_record:
+            message_text = '\n Delete the following records?\n\n'
+            if 'UNIT' in last_record.keys() and 'ID' in last_record.keys():
+                unit = last_record["UNIT"]
+                idno = last_record["ID"]
+                a_record = Query()
+                records_to_delete = self.data.db.table(self.data.table).search(a_record.UNIT.matches('^' + unit + '$', flags = re.IGNORECASE) and a_record.ID.matches('^' + idno + '$', flags = re.IGNORECASE))
+                for record in records_to_delete:
+                    for field in self.cfg.fields():
+                        if field in record:
+                            message_text += "%s : %s \n" % (field, record[field])
+                    message_text += '\n\n'
+                self.popup = e5_MessageBox('Delete last object', message_text, response_type = "YESNO",
+                                            call_back = [self.delete_last_object, self.close_popup],
+                                            colors = self.colors)
             else:
-                if self.location.x is not None and self.location.y is not None and self.location.z is not None:
-                    self.xyz_global = point(self.xyz.x + self.location.x,
-                                            self.xyz.y + self.location.y,
-                                            self.xyz.z + self.location.z,)
-                else:
-                    self.xyz_global = self.xyz
+                self.popup = e5_MessageBox('Delete last object',
+                                            '\n For now, this option requires a field called UNIT and another called ID.',
+                                            call_back = self.close_popup,
+                                            colors = self.colors)
+        else:
+            self.popup = e5_MessageBox('Delete last object', '\n No records in table to delete.',
+                                        call_back = self.close_popup,
+                                        colors = self.colors)
+        self.popup.open()
+        self.popup_open = True
+
+    def delete_last_object(self, value):
+        last_record = self.data.last_record()
+        unit = last_record["UNIT"]
+        idno = last_record["ID"]
+        a_record = Query()
+        records_to_delete = self.data.db.table(self.data.table).search(a_record.UNIT.matches('^' + unit + '$', flags = re.IGNORECASE) and a_record.ID.matches('^' + idno + '$', flags = re.IGNORECASE))
+        for record in records_to_delete:
+            self.data.delete(record.doc_id)
+        self.data.new_data[self.data.table] = True
+        self.close_popup(value)
+
+    def show_delete_last_record(self):
+        last_record = self.data.last_record()
+        if last_record:
+            message_text = '\n'
+            for field in self.cfg.fields():
+                if field in last_record:
+                    message_text += "%s : %s \n" % (field, last_record[field])
+            self.popup = e5_MessageBox('Delete Last Record', message_text, response_type = "YESNO",
+                                        call_back = [self.delete_last_record, self.close_popup],
+                                        colors = self.colors)
+        else:
+            self.popup = e5_MessageBox('Delete Last Record', '\n No records in table to delete.',
+                                        call_back = self.close_popup,
+                                        colors = self.colors)
+        self.popup.open()
+        self.popup_open = True
 
-    def round_xyz(self):
-        if self.xyz_global.x is not None:
-            self.xyz_global = self.round_point(self.xyz_global)
+    def delete_last_record(self, value):
+        last_record = self.data.last_record()
+        self.data.delete(last_record.doc_id)
+        self.data.new_data[self.data.table] = True
+        self.close_popup(value)
+
+    def show_delete_all_records(self, table_name = None):
+        if not table_name:
+            message_text = '\n You are asking to delete all of the records in the current database table. Are you sure you want to do this?'
+            self.delete_table = self.data.table
+        else:
+            message_text = f'\n You are asking to delete all of the records in the {table_name} table. Are you sure you want to do this?'
+            self.delete_table = table_name
+        self.popup = e5_MessageBox('Delete All Records', message_text, response_type = "YESNO",
+                                    call_back = [self.delete_all_records1, self.close_popup],
+                                    colors = self.colors)
+        self.popup.open()
+        self.popup_open = True
 
-        if self.xyz.x is not None:
-            self.xyz = self.round_point(self.xyz)
+    def delete_all_records1(self, value):
+        self.popup.dismiss()
+        self.popup_open = False
+        message_text = f'\nThis is your last chance.  All records in the {self.delete_table} table will be deleted when you press Yes.'
+        self.popup = e5_MessageBox('Delete All Records', message_text, response_type = "YESNO",
+                                    call_back = [self.delete_all_records2, self.close_popup],
+                                    colors = self.colors)
+        self.popup.open()
+        self.popup_open = True
 
-    def round_point(self, p):
-        return(point(round(p.x, 3), round(p.y, 3), round(p.z, 3)))
+    def delete_all_records2(self, value):
+        self.data.delete_all(self.delete_table)
+        self.data.new_data[self.data.table] = True
+        self.popup.dismiss()
+        self.popup_open = False
+        if APP_NAME == 'EDM':
+            self.update_info_label()
 
-    def clear_xyz(self):
-        self.xyz = point()
-        self.xyz_global = point()
+    def show_save_csvs(self, *args):
+        if self.cfg.filename and self.data.filename:
+            self.csv_data_type = args[0].id.lower() if len(args) > 0 else self.data.table
+            filename = ntpath.split(self.cfg.filename)[1].split(".")[0]
+            filename = filename + "_" + self.csv_data_type + self.date_stamp() + '.csv'
+            content = e5_SaveDialog(filename = filename,
+                                    start_path = self.cfg.path,
+                                    save = self.save_csvs,
+                                    cancel = self.dismiss_popup)
+            self.popup = Popup(title = "Export CSV file",
+                                content = content,
+                                size_hint = (0.9, 0.9))
+        else:
+            self.popup = e5_MessageBox('E5', '\n Open a CFG before exporting to CSV',
+                                        call_back = self.dismiss_popup,
+                                        colors = self.colors)
+        self.popup.open()
+        self.popup_open = True
 
-    def parse_nez(self):
-        pass
+    def save_csvs(self, instance):
 
-    def comport_nos(self):
-        ports = self.list_comports()
-        return(list([port[0]['port'] for port in ports]))
-
-    def list_comports(self):
-        ports = []
-        for n, (port, desc, hwid) in enumerate(sorted(comports()), 1):
-            ports.append([{'port': port, 'desc': desc}])
-        return(ports)
-
-    def clear_io(self):
-        self.io = ''
-
-    def trim_io(self, length = 1024):
-        self.io = self.io[:length]
-
-    def add_to_io(self, data):
-        self.io = self.io + data
-        self.trim_io()
-
-    def data_waiting(self):
-        if self.serialcom.is_open:
-            if self.serialcom.in_waiting > 0:
-                return(True)
-        return(False)
-
-    def send(self, data):
-        if self.serialcom.is_open:
-            self.serialcom.write(data)
-            self.add_to_io('Sent -> ' + data.decode())
-            # print(data)
-            # sleep(0.1)
-
-    def receive(self):
-        if self.serialcom.is_open:
-            data = self.serialcom.read_until().decode()
-            # data = self.serialcom.readline().decode()
-            if data:
-                if self.event is not None:  # This is for Topcon where the COM has to be monitored
-                    self.event.cancel()
-                    self.event = None
-                self.add_to_io('Received <- ' + data)
-            return(data)
-
-    def close(self):
-        if self.serialcom.is_open:
-            self.serialcom.close()
-            self.clear_io()
-
-    def open(self):
-        self.close()
-        if self.baudrate and self.comport and self.parity and self.databits and self.stopbits:
-            if self.comport in self.comport_nos():
-                self.serialcom.port = self.comport
-                self.serialcom.baudrate = int(self.baudrate)
-                if self.parity == 'Even':
-                    self.serialcom.parity = serial.PARITY_EVEN
-                elif self.parity == 'Odd':
-                    self.serialcom.parity = serial.PARITY_ODD
-                elif self.parity == 'None':
-                    self.serialcom.parity = serial.PARITY_NONE
-                self.serialcom.stopbits = int(self.stopbits)
-                self.serialcom.bytesize = int(self.databits)
-                self.serialcom.timeout = 30
-                try:
-                    self.serialcom.open()
-                    self.clear_io()
-                    return(True)
-                except OSError:
-                    pass
-        return(False)
+        filename = os.path.join(self.popup.content.filesaver.path, self.popup.content.filename)
 
-    def settings_pretty(self):
-        if self.baudrate and self.comport and self.parity and self.databits and self.stopbits:
-            return(f"{self.comport}:{self.baudrate},{self.parity},{self.databits},{self.stopbits}")
-        else:
-            return("Incomplete Settings")
-
-    def clear_com(self):
-        if self.serialcom.is_open:
-            self.serialcom.reset_input_buffer()
-            self.serialcom.reset_output_buffer()
-
-    def distance(self, p1, p2):
-        return(sqrt((p1.x - p2.x)**2 + (p1.y - p2.y)**2 + (p1.z - p2.z)**2))
-
-    def dms_to_decdeg(self, angle):
-        angle = str(angle)
-        degrees = int(angle.split(".")[0])
-        minutes = int(angle.split(".")[1][0:2])
-        seconds = int(angle.split(".")[1][2:])
-        return(degrees + minutes / 60.0 + seconds / 3600.0)
-
-    def decdeg_to_radians(self, angle):
-        return(angle / 360.0 * (2.0 * pi))
-
-    def vhd_to_xyz(self):
-        if self.vangle is not None and self.hangle is not None and self.sloped is not None:
-            # angle_decdeg = self.dms_to_decdeg(self.vangle)
-            z = self.sloped * cos(self.decdeg_to_radians(self.vangle))
-            actual_distance = sqrt(self.sloped**2 - z**2)
-
-            # angle_decdeg = self.dms_to_decdeg(self.hangle)
-            angle_decdeg = 450 - self.hangle
-            x = cos(self.decdeg_to_radians(angle_decdeg)) * actual_distance
-            y = sin(self.decdeg_to_radians(angle_decdeg)) * actual_distance
-            self.xyz = point(x, y, z)
-
-    # The following functions are needed by the rotation function at the end of this list.
-    # Note too that all of the dependent routines are self written
-    # rather than pulled from existing libraries (like numpy) to avoid dependencies.  Dependencies make porting to
-    # Apple and Android more difficult.
-    def dot_product(self, a, b):
-        return(a.x * b.x + a.y * b.y + a.z * b.z)
-
-    def normalize_vector(self, a):
-        if sqrt(self.dot_product(a, a)) == 0:
-            return(a)
-        else:
-            return(self.scale_vector(1 / sqrt(self.dot_product(a, a)), a))
-
-    def vector_subtract(self, p2, p1):
-        return(point(p2.x - p1.x, p2.y - p1.y, p2.z - p1.z))
-
-    def surface_normal(self, a):
-        u = self.vector_subtract(a[1], a[0])
-        v = self.vector_subtract(a[2], a[0])
-        return(self.normalize_vector(self.cross_product(u, v)))
-
-    def vector_magnitude(self, a):
-        return(sqrt(self.dot_product(a, a)))
-
-    def cross_product(self, v1, v2):
-        return(point(v1.y * v2.z - v1.z * v2.y,
-                        v1.z * v2.x - v1.x * v2.z,
-                        v1.x * v2.y - v1.y * v2.x))
-
-    def scale_vector(self, scalar, a):
-        return(point(scalar * a.x,
-                        scalar * a.y,
-                        scalar * a.z))
-
-    def empty_matrix(self):
-        return([[0.0 for x in range(3)] for y in range(3)])
-
-    def identity_matrix(self):
-        i = self.empty_matrix()
-        for n in range(3):
-            i[n][n] = 1.0
-        return(i)
-
-    def matrix_product(self, a, b):
-        result = self.empty_matrix()
-        for row in range(3):
-            for col in range(3):
-                for index in range(3):
-                    result[row][col] = result[row][col] + a[row][index] * b[index][col]
-        return(result)
-
-    def scale_matrix(self, scalar, m):
-        result = self.empty_matrix()
-        for row in range(3):
-            for col in range(3):
-                result[row][col] = scalar * m[row][col]
-        return(result)
-
-    def matrix_add(self, m1, m2):
-        result = self.empty_matrix()
-        for row in range(3):
-            for col in range(3):
-                result[row][col] = m1[row][col] + m2[row][col]
-        return(result)
-
-    def translate_point(self, translation, p):
-        return(point(p.x + translation.x,
-                        p.y + translation.y,
-                        p.z + translation.z))
-
-    def rotate_point_2d(self, local_vector, global_vector, p):
-        # local coodinate system and global coordinate system vectors that will be made to align with each other.
-        # p is a point to be rotated along with this vector alignment.
-        # This is in essence a 2D rotation in the plane formed by the two vectors and around the perpendicular to this plane.
-        # (Two vectors have the origin in common and thus make three points altogether and this is a plane)
-        # (The surface normal is the rotation axis and the angle of rotation is the angle between the two vectors in this plane)
-
-        i = self.identity_matrix()
-
-        v = self.cross_product(local_vector, global_vector)
-        s = self.vector_magnitude(v)
-        c = self.dot_product(local_vector, global_vector)
-
-        vx = self.empty_matrix()
-        vx[0][0] = 0.0
-        vx[0][1] = -1.0 * v.z
-        vx[0][2] = v.y
-
-        vx[1][0] = v.z
-        vx[1][1] = 0.0
-        vx[1][2] = -1.0 * v.x
-
-        vx[2][0] = -1.0 * v.y
-        vx[2][1] = v.x
-        vx[2][2] = 0.0
-
-        v2x = self.scale_matrix(1 / (1 + c), self.matrix_product(vx, vx))
-
-        # Now create the rotation matrix by adding these components
-        r = self.matrix_add(self.matrix_add(i, vx), v2x)
-
-        # Now do the rotation by multiplying this rotation matrix by the individual points (or vectors)
-        return(point((p.x * r[0][0]) + (p.y * r[1][0]) + (p.z * r[2][0]),
-                        (p.x * r[0][1]) + (p.y * r[1][1]) + (p.z * r[2][1]),
-                        (p.x * r[0][2]) + (p.y * r[1][2]) + (p.z * r[2][2])))
-
-    def rotate_point_2d_2(self, rotation_vector, local_vector, global_vector, p):
-        # local coodinate system and global coordinate system vectors that will be made to align with each other.
-        # p is a point to be rotated along with this vector alignment.
-        # This is in essence a 2D rotation in the plane formed by the two vectors and around the perpendicular to this plane.
-        # (Two vectors have the origin in common and thus make three points altogether and this is a plane)
-        # (The surface normal is the rotation axis and the angle of rotation is the angle between the two vectors in this plane)
-
-        i = self.identity_matrix()
-
-        v = rotation_vector
-        s = self.vector_magnitude(v)
-        c = self.dot_product(local_vector, global_vector)
-
-        vx = self.empty_matrix()
-        vx[0][0] = 0.0
-        vx[0][1] = -1.0 * v.z
-        vx[0][2] = v.y
-
-        vx[1][0] = v.z
-        vx[1][1] = 0.0
-        vx[1][2] = -1.0 * v.x
-
-        vx[2][0] = -1.0 * v.y
-        vx[2][1] = v.x
-        vx[2][2] = 0.0
-
-        v2x = self.scale_matrix(1 / (1 + c), self.matrix_product(vx, vx))
-
-        # Now create the rotation matrix by adding these components
-        r = self.matrix_add(self.matrix_add(i, vx), v2x)
-
-        # Now do the rotation by multiplying this rotation matrix by the individual points (or vectors)
-        return(point((p.x * r[0][0]) + (p.y * r[1][0]) + (p.z * r[2][0]),
-                        (p.x * r[0][1]) + (p.y * r[1][1]) + (p.z * r[2][1]),
-                        (p.x * r[0][2]) + (p.y * r[1][2]) + (p.z * r[2][2])))
-
-    # This routine takes two sets of datums (local and global) and converts a newly recorded point
-    # from the local coordinate system (e.g. Microscribe) to the global coordinate system.
-    # It does this by performing a rotation around first one leg and then another of the triangle formed by the datums.
-    # It is written to be readable.  Much efficiency could be gained but as points are only rotated as recorded,
-    # the routine does not need to be fast.  Note too that all of the dependent routines are self written
-    # rather than pulled from existing libraries (like numpy) to avoid dependencies.  Dependencies make porting to
-    # Apple and Android more difficult.
-
-    def rotate_point(self, p = None):
-        # p is a point to be rotated
-
-        if p is None:
-            p = self.xyz
-
-        if len(self.rotate_local) == 3 and len(self.rotate_global) == 3 and p:
-            rotated_local = []
-
-            # Shift point to relative to the origin
-            p = self.vector_subtract(p, self.rotate_local[0])
-
-            # Shift local set relative to origin
-            local = []
-            local.append(point(0, 0, 0))
-            local.append(self.vector_subtract(self.rotate_local[1], self.rotate_local[0]))
-            local.append(self.vector_subtract(self.rotate_local[2], self.rotate_local[0]))
-
-            # First line up one side of the triangle formed by the three datum points
-            local_vector = self.normalize_vector(local[1])
-            global_vector = self.normalize_vector(self.vector_subtract(self.rotate_global[1], self.rotate_global[0]))
-            p_out = self.rotate_point_2d(global_vector, local_vector, p)
-
-            # Put the local datums in this new space as well
-            rotated_local.append(self.rotate_point_2d(global_vector, local_vector, local[0]))
-            rotated_local.append(self.rotate_point_2d(global_vector, local_vector, local[1]))
-            rotated_local.append(self.rotate_point_2d(global_vector, local_vector, local[2]))
-
-            # Now line up on the other side of the triangle formed by the three datum points
-            # by computing the surface normal of each and rotating on the first already rotated side
-            local_datums_normal = self.normalize_vector(self.cross_product(self.normalize_vector(rotated_local[1]),
-                                                        self.normalize_vector(rotated_local[2])))
-            global_datums_normal = self.normalize_vector(self.cross_product(self.normalize_vector(self.vector_subtract(self.rotate_global[1], self.rotate_global[0])),
-                                                                            self.normalize_vector(self.vector_subtract(self.rotate_global[2], self.rotate_global[0]))))
-            p_out2 = self.rotate_point_2d(global_datums_normal, local_datums_normal, p_out)
-
-            # Finish the rotation for the local datums as well (not strictly needed for points 2 and 3)
-            rotated_local[0] = self.rotate_point_2d(global_vector, local_vector, rotated_local[0])
-            rotated_local[1] = self.rotate_point_2d(global_vector, local_vector, rotated_local[1])
-            rotated_local[2] = self.rotate_point_2d(global_vector, local_vector, rotated_local[2])
-
-            # Now align the starting points of each grid systems by shifting the first datum points onto each other
-            result = self.translate_point(self.rotate_global[0], p_out2)
-
-            return(result)
-
-        else:
-            return(None)
-
-    def rotate_initialize(self, local_datums, global_datums):
-        # local and global datums are two lists of three corresponding points in the two grid systems
-
-        self.rotate_local = local_datums
-        self.rotate_global = global_datums
-
-    # Function specific to Topcon #
-
-    def launch_point_topcon(self):
-        self.send("Z34")   # Slope angle mode
-        self.receive()
-        # delay(0.5)
-
-        self.send("C")     # Take the shot
-        self.receive()
-        # delay(0.5)
-        self.event1 = Clock.schedule_interval(self.check_receive_buffer, .2)
-
-    def check_receive_buffer(self):
-        # need code here to check for a completed shot
-        # and then acknowledge back
-        pass
+        self.popup.dismiss()
 
-    def make_bcc_topcon(self, itext):
-        # Dim b As Integer = 0
-        # Dim i As Integer
-        # Dim q As Integer
-        # Dim b1 As Integer
-        # Dim b2 As Integer
-
-        b = 0
-        for i in range(0, len(itext)):
-            # q = asc(itext[i:i+1])
-            # b1 = q and (Not b) # this is not at all ready
-            # b2 = b and (Not q)
-            # b = b1 or b2
-            pass
-
-        bcc = "000" + str(b).strip()
-        return(bcc[-3])
-
-    def set_horizontal_angle_topcon(self, angle):
-        # angle should be in dddmmss
-        self.send("J+" + angle + "d")
-        self.receive()
-        # delay(1)
-        self.clear_com()
-
-    def initialize_topcon(self):
-        self.send("ST0")
-
-    # end Topcon
-
-    # Sokkia functions
-
-    def launch_point_sokkia(self):
-        self.send(chr(17).encode())
-
-    def set_horizontal_angle_sokkia(self, angle):
-        # need to send to station in format ddd.mmss
-        set_angle_command = "/Dc " + angle + "\r\n"
-        self.send(set_angle_command.encode())
-        # delay(5)
-        self.clear_com()
-
-    def fetch_point_sokkia(self):
-        self.pnt = self.receive()
-        if self.pnt:
-            self.parce_sokkia()
-            self.vhd_to_xyz()
-
-    def parce_sokkia(self):
-        if self.pnt:
-            vhd = self.pnt.strip().split(" ")
-            if len(vhd) == 3:
-                try:
-                    self.sloped = float(vhd[0]) / 1000.0
-                except ValueError:
-                    self.sloped = None
-            if vhd[1][0] != 'E':
-                self.vangle = Angle(f'{vhd[1][:3]}d{vhd[1][3:5]}m{vhd[1][5:7]}').d
-            else:
-                self.vangle = None
-            if vhd[2][0] != 'E':
-                self.hangle = Angle(f'{vhd[1][:3]}d{vhd[1][3:5]}m{vhd[1][5:7]}').d
-            else:
-                self.hangle = None
+        if APP_NAME == 'EDM' and self.csv_data_type != 'points':
+            router = {'datums': self.cfg_datums, 'units': self.cfg_units, 'prisms': self.cfg_prisms}
+            response = router[self.csv_data_type].write_csvs(filename, self.data.db.table(self.csv_data_type))
+        else:
+            table = self.data.db.table(self.data.table)
+            response = self.cfg.write_csvs(filename, table)
+
+        if not response:
+            response = f'\n The table {self.csv_data_type} was successfully written as the file {filename}.'
+        self.popup = e5_MessageBox('CSV Export', response, call_back = self.close_popup, colors = self.colors)
+        self.popup.open()
+        self.popup_open = True
 
-    def initialize_sokkia(self):
-        pass
+    def show_save_geojson(self):
+        if self.cfg.filename and self.data.filename:
+            geojson_compatible = 0
+            for fieldname in self.cfg.fields():
+                if fieldname in ['X', 'Y', 'Z']:
+                    geojson_compatible += 1
+                elif fieldname in ['LATITUDE', 'LONGITUDE', 'ELEVATION']:
+                    geojson_compatible += 1
+                else:
+                    field = self.cfg.get(fieldname)
+                    if field.inputtype in ['GPS']:
+                        geojson_compatible = 2
+                if geojson_compatible > 1:
+                    break
+            if geojson_compatible:
+                filename = ntpath.split(self.cfg.filename)[1].split(".")[0]
+                filename = filename + '_' + self.data.table + '.geojson'
+
+                content = e5_SaveDialog(filename = filename,
+                                        start_path = self.cfg.path,
+                                        save = self.save_geojson,
+                                        cancel = self.dismiss_popup,
+                                        colors = self.colors)
+                self.popup = Popup(title = "Export geoJSON file",
+                                    content = content,
+                                    size_hint = (0.9, 0.9))
+            else:
+                self.popup = e5_MessageBox('E5',
+                                            '\nA geoJSON file requires a GPS type field or fields named XY(Z) or Latitude, '
+                                            'Longitude and optionally Elevation.',
+                                            call_back = self.dismiss_popup,
+                                            colors = self.colors)
+        else:
+            self.popup = e5_MessageBox('E5', '\nOpen a CFG before exporting to geoJSON.',
+                                        call_back = self.dismiss_popup,
+                                        colors = self.colors)
+        self.popup.open()
+        self.popup_open = True
 
-    # end Sokkia
+    def save_geojson(self, path):
+        filename = os.path.join(self.popup.content.filesaver.path, self.popup.content.filename)
 
-    # Leica functions ###
+        self.popup.dismiss()
+        self.popup = Popup(title = "Export geoJSON file",
+                            content = DataGridLabelAndProgressBar(col = 'Progress...', popup = True,
+                                                                  colors = self.colors, orientation = 'vertical'),
+                                                                  size_hint = (.6, .15))
+        self.popup.open()
+        self.popup_open = True
 
-    def pad_dms_leica(self, angle):
-        degrees = ('000' + angle.split('.')[0])[-3:]
-        minutes_seconds = (angle.split('.')[1] + '0000')[0:4]
-        return(degrees + minutes_seconds)
-
-    def set_horizontal_angle_leica(self, angle):
-        # function expects angle as ddd.mmss input
-        # but decimal seconds are possible
-        if angle.count('.') == 0:
-            angle = angle + '.0000'
-        elif angle.count('.') == 2:
-            dms = angle.split('.')
-            ms = '0000' + str(round(float(dms[1] + '.' + dms[2])))
-            ms = ms[-4:]
-            angle = str(dms[0] + '.' + ms)
-        set_angle_command = "PUT/21...4+%s0 \r\n" % self.pad_dms_leica(angle)
-        self.send(set_angle_command.encode())
-        return(self.receive())
-
-    def launch_point_leica(self):
-        self.send(b"GET/M/WI21/WI22/WI31/WI51\r\n")
-
-    def fetch_point_leica(self):
-        self.pnt = self.receive()
-        if self.pnt:
-            self.parce_leica()
-            self.vhd_to_xyz()
-
-    def parce_leica(self):
-        if self.pnt:
-            if self.pnt.startswith('*'):
-                self.pnt = self.pnt[1:]
-            for component in self.pnt.split(' '):
-                if component.startswith('21.'):
-                    data = component[6:]
-                    self.hangle = Angle(f'{data[:-5]}d{data[-5:-3]}m{data[-3:-1]}.{data[-1]}').d
-                elif component.startswith('22.'):
-                    data = component[6:]
-                    self.vangle = Angle(f'{data[:-5]}d{data[-5:-3]}m{data[-3:-1]}.{data[-1]}').d
-                elif component.startswith('31.'):
-                    try:
-                        self.sloped = float(component[6:]) / 1000.0
-                    except ValueError:
-                        self.sloped = None
-                elif component.startswith('51.'):
-                    try:
-                        self.prism_constant = float(component[-4:]) / 1000.0
-                    except ValueError:
-                        self.prism_constant = None
-
-    def initialize_leica(self):
-        self.send("SET/41/0")
-        acknow1 = self.receive()
-        self.send("SET/149/2")
-        acknow2 = self.receive()
-        return(acknow1 + acknow2)
-    # ## Leica functions ###
+        self.popup.status = "Working..."
+        self.popup.filename = filename
+        self.upload_thread = Thread(target = self.cfg.write_geojson, args = (filename, self.data.db.table(self.data.table), self.popup))
+        self.upload_thread.start()
+
+        self.event = Clock.schedule_interval(self.check_file_conversion, 0.5)
+
+    def check_file_conversion(self, dt):
+        if self.popup.status != 'Working...':
+            response = self.popup.status
+            if not response:
+                response = f'\n The table {self.data.table} was successfully written as geoJSON to the file {self.popup.filename}.'
+            self.popup.dismiss()
+            self.popup = e5_MessageBox('geoJSON Export', response, call_back = self.close_popup, colors = self.colors)
+            self.popup.open()
+            self.popup_open = True
+            return False
 
-    # ## Leica geocom functions ###
-    def initialize_geocom(self):
-        pass
 
-    def set_horizontal_angle_geocom(self, angle):
-        # function expects angle as ddd.mmss as input
-        # %R1Q,2113:HzOrientation[double]
-        output = "%R1Q,2113:{:10.8f}".format(self.decdeg_to_radians(self.dms_to_decdeg(angle)))
-        errorcode = self.send(output)
-        returncode = self.receive()
-
-    def record_point_geocom(self):
-        self.clear_com()
-        self.send("%R1Q,2008:1,1")          # Use the defaults with 1 and 1
-        errorcode = self.receive()
-        if not errorcode:
-            # %R1Q,2108:WaitTime[long],Mode[long]
-            # Waittime is in ms
-            # Mode 1 = automatic
-            self.clear_com()
-            self.send("%R1Q,2108:10000,1")  # Wait for the measurements and return the angles + sloped
-            result = self.receive()
-        self.clear_com()
-        self.send("%R1Q,2008:3,1")          # Empty the measurement buffer as a precaution
-        returncode = self.receive()
-    # ## Leica geocom functions ###
+class e5_gridlayout(GridLayout):
+    id = ObjectProperty(None)
+
+    def __init__(self, **kwargs):
+        super(e5_gridlayout, self).__init__(**kwargs)
 
-# endregion
 
+class e5_SettingsScreen(Screen):
 
-class ComTestScreen(Screen):
-    def __init__(self, station = None, cfg = None, colors = None, **kwargs):
-        super(ComTestScreen, self).__init__(**kwargs)
+    buttons = []
+    labels = []
 
+    def __init__(self, cfg = None, ini = None, colors = None, **kwargs):
+        super(e5_SettingsScreen, self).__init__(**kwargs)
         self.colors = colors if colors else ColorScheme()
-        self.station = station
+        self.ini = ini
         self.cfg = cfg
 
-        self.clear_widgets()
-        self.layout = GridLayout(cols = 1,
-                                 spacing = 5,
-                                 size_hint_x = width_calculator(.9, 400),
-                                 size_hint_y = .9,
-                                 pos_hint = {'center_x': .5, 'center_y': .5})
-        self.add_widget(self.layout)
-        self.build_screen()
-
-    def current_settings_pretty(self):
-        txt = 'The current settings are:\n' + self.station.make + '\n' + self.station.settings_pretty()
-        txt += '\nThe COM port is '
-        txt += 'Open' if self.station.serialcom.is_open else 'Close'
-        return(txt)
-
     def on_enter(self):
-        sm.get_screen('StationConfigurationScreen').call_back = 'MainScreen'
-        self.current_settings.text = self.current_settings_pretty()
-        self.station.clear_io()
-        self.event = Clock.schedule_interval(self.check_io, .2)
-
-    def check_io(self, dt):
-        if self.station.data_waiting():
-            self.station.receive()
-        if self.station.io != '' and self.station.io != self.io.scrolling_label.text:
-            self.io.scrolling_label.text = self.station.io
+        self.build_screen()
 
     def build_screen(self):
+        self.clear_widgets()
+        layout = GridLayout(cols = 1,
+                            # size_hint_x = width_calculator(.9, 600),
+                            size_hint_y = 1,
+                            spacing = 5,
+                            padding = 5,
+                            pos_hint = {'center_x': .5, 'center_y': .5})
+        layout.bind(minimum_height = layout.setter('height'))
+
+        darkmode = GridLayout(cols = 2, size_hint_y = .1, spacing = 5, padding = 5)
+        darkmode_label = e5_label('Dark Mode', colors = self.colors)
+        self.labels.append(darkmode_label)
+        darkmode.add_widget(darkmode_label)
+        darkmode_switch = Switch(active = self.colors.darkmode)
+        darkmode_switch.bind(active = self.darkmode)
+        darkmode.add_widget(darkmode_switch)
+        layout.add_widget(darkmode)
+
+        colorscheme = GridLayout(cols = 2, size_hint_y = .6, spacing = 5, padding = 5)
+        colorscheme_label = e5_label('Color Scheme', colors = self.colors)
+        self.labels.append(colorscheme_label)
+        colorscheme.add_widget(colorscheme_label)
+        colorscheme.add_widget(e5_scrollview_menu(self.colors.color_names(),
+                                                  menu_selected = '',
+                                                  colors = self.colors,
+                                                  call_back = [self.color_scheme_selected]))
+        temp = ColorScheme()
+        for widget in colorscheme.walk():
+            if hasattr(widget, 'id'):
+                if widget.id in self.colors.color_names():
+                    temp.set_to(widget.text)
+                    widget.background_color = temp.button_background
+                    widget.height = 40
+                    self.buttons.append(widget)
+        layout.add_widget(colorscheme)
 
-        self.settings = GridLayout(cols = 2, spacing = 5, padding = 5, size_hint = (.2, None))
-        self.current_settings = e5_label(self.current_settings_pretty(), colors = self.colors, size_hint = (0.75, None))
-        self.settings.add_widget(self.current_settings)
-        self.change_settings = e5_button("Change Settings", call_back = self.settings_change, colors = self.colors)
-        self.settings.add_widget(self.change_settings)
-        self.layout.add_widget(self.settings)
-
-        self.horizontal_angle = GridLayout(cols = 2, spacing = 5, padding = 5, size_hint = (.2, None))
-        self.leftside = GridLayout(cols = 1, spacing = 5, padding = 5)
-        self.leftside.add_widget(e5_label('Enter angle as ddd.mmss', colors = self.colors))
-        self.hangle_input = e5_textinput(write_tab = False)
-        self.hangle_input.bind(minimum_height = self.hangle_input.setter('height'))
-        self.leftside.add_widget(self.hangle_input)
-        self.horizontal_angle.add_widget(self.leftside)
-        self.set_angle = e5_button("Set H-angle", call_back = self.set_hangle, colors = self.colors)
-        self.horizontal_angle.add_widget(self.set_angle)
-        self.layout.add_widget(self.horizontal_angle)
-
-        self.record = GridLayout(cols = 1, spacing = 5, padding = 5, size_hint = (.2, None))
-        self.measure = e5_button("Record Point", call_back = self.record_point, colors = self.colors)
-        self.record.add_widget(self.measure)
-        self.layout.add_widget(self.record)
-
-        self.io = e5_scrollview_label('Set an angle or record a point and the communication to the station will appear here.  If nothing is received at all, then it might be a COM port number issue.  If what is received is unreadable, then there is a problem with the speed, parity, data bits, and stop bits.  If everything looks fine, but the angle does not change or a point is not taken, then likely Shannon needs to have a look.  Email the results here to him.', popup = False, colors = self.colors)
-        self.layout.add_widget(self.io)
-
-        self.layout.add_widget(e5_side_by_side_buttons(text = ['Clear', 'Copy', 'Close'],
-                                                        id = ['clear', 'copy', 'close'],
-                                                        call_back = [self.clear_io, self.copy_io, self.close],
-                                                        selected = [False, False, False],
-                                                        colors = self.colors))
-
-    def clear_io(self, instance):
-        self.station.clear_io()
-        self.io.scrolling_label.text = ''
-
-    def copy_io(self, instance):
-        Clipboard.copy(self.io.scrolling_label.text)
-
-    def set_hangle(self, instance):
-        if self.hangle_input.text:
-            self.station.set_horizontal_angle(self.hangle_input.text)
-            # self.io.scrolling_label.text = self.station.io
+        backups = GridLayout(cols = 2, size_hint_y = .2, spacing = 5, padding = 5)
+        self.backup_label = e5_label(f'Auto-backup after\n{self.ini.backup_interval} records.',
+                                        colors = self.colors)
+        self.labels.append(self.backup_label)
+        backups.add_widget(self.backup_label)
+        slide = Slider(min = 0, max = 200, step = 5,
+                        value = self.ini.backup_interval,
+                        orientation = 'horizontal',
+                        value_track = True,
+                        value_track_color = self.colors.button_background)
+        backups.add_widget(slide)
+        slide.bind(value = self.update_backup_interval)
+
+        incremental_backup_label = e5_label('Use incremental\nbackups?', colors = self.colors)
+        self.labels.append(incremental_backup_label)
+        backups.add_widget(incremental_backup_label)
+        backups_switch = Switch(active = self.ini.incremental_backups)
+        backups_switch.bind(active = self.incremental_backups)
+        backups.add_widget(backups_switch)
+        layout.add_widget(backups)
+
+        text_font_size = GridLayout(cols = 2, size_hint_y = .1, spacing = 5, padding = 5)
+        text_font_size_value = int(self.colors.text_font_size.replace("sp", '')) if self.colors.text_font_size else 12
+        self.text_font_size_label = e5_label('Text font size is %s' % text_font_size_value,
+                                                id = 'label_font_size',
+                                                colors = self.colors)
+        self.labels.append(self.text_font_size_label)
+        text_font_size.add_widget(self.text_font_size_label)
+        text_font_slide = Slider(min = 12, max = 26, step = 1, value = text_font_size_value,
+                                    orientation = 'horizontal',
+                                    value_track = True, value_track_color = self.colors.button_background)
+        text_font_size.add_widget(text_font_slide)
+        text_font_slide.bind(value = self.update_text_font_size)
+        layout.add_widget(text_font_size)
+
+        button_font_size = GridLayout(cols = 2, size_hint_y = .1, spacing = 5, padding = 5)
+        button_font_size_value = int(self.colors.button_font_size.replace("sp", '')) if self.colors.button_font_size else 12
+        self.button_font_size_label = e5_label('Button font size is %s' % button_font_size_value,
+                                                id = 'label_font_size',
+                                                colors = self.colors)
+        self.labels.append(self.button_font_size_label)
+        button_font_size.add_widget(self.button_font_size_label)
+        button_font_slide = Slider(min = 12, max = 26, step = 1, value = button_font_size_value,
+                                    orientation = 'horizontal',
+                                    value_track = True, value_track_color = self.colors.button_background)
+        button_font_size.add_widget(button_font_slide)
+        button_font_slide.bind(value = self.update_button_font_size)
+        layout.add_widget(button_font_size)
+
+        settings_layout = GridLayout(cols = 1,
+                                        size_hint_max_x = 400,
+                                        size_hint_y = 1,
+                                        spacing = 5, padding = 5,
+                                        pos_hint = {'center_x': .5, 'center_y': .5})
+        scrollview = ScrollView(size_hint = (1, 1),
+                                 bar_width = SCROLLBAR_WIDTH)
+        scrollview.add_widget(layout)
+        settings_layout.add_widget(scrollview)
+
+        self.back_button = e5_button('Back', selected = True,
+                                             call_back = self.go_back,
+                                             colors = self.colors)
+        self.buttons.append(self.back_button)
+        settings_layout.add_widget(self.back_button)
+        self.add_widget(settings_layout)
+
+    def update_text_font_size(self, intance, value):
+        self.text_font_size_label.text = 'Text font size is %s' % int(value)
+        self.colors.text_font_size = '%ssp' % value
+        self.refresh_screen()
+
+    def update_button_font_size(self, intance, value):
+        self.button_font_size_label.text = 'Button font size is %s' % int(value)
+        self.colors.button_font_size = '%ssp' % value
+        self.refresh_screen()
+
+    def update_backup_interval(self, instance, value):
+        self.ini.backup_interval = int(value)
+        self.backup_label.text = 'Auto-backup after\nevery %s\nrecords entered.' % self.ini.backup_interval
+
+    def incremental_backups(self, instance, value):
+        self.ini.incremental_backups = value
+
+    def darkmode(self, instance, value):
+        self.colors.darkmode = value
+        self.colors.set_colormode()
+        self.build_screen()
 
-    def settings_change(self, instance):
-        sm.get_screen('StationConfigurationScreen').call_back = 'ComTestScreen'
-        self.event.cancel()
-        self.parent.current = 'StationConfigurationScreen'
+    def color_scheme_selected(self, instance):
+        self.colors.set_to(instance.text)
+        self.back_button.background_color = self.colors.button_background
+        self.back_button.color = self.colors.button_color
 
-    def record_point(self, instance):
-        self.station.take_shot()
+    def refresh_screen(self):
+        for widget in self.buttons:
+            widget.font_size = self.colors.button_font_size
+        for widget in self.labels:
+            widget.font_size = self.colors.text_font_size
 
-    def close(self, instance):
-        self.event.cancel()
+    def go_back(self, instance):
+        self.ini.update(self.colors, self.cfg)
         self.parent.current = 'MainScreen'
 
 
-class MainScreen(e5_MainScreen):
+class e5_InfoScreen(Screen):
+    content = ObjectProperty(None)
+    back_button = ObjectProperty(None)
 
-    popup = ObjectProperty(None)
-    popup_open = False
-    text_color = (0, 0, 0, 1)
-    title = __program__
+    def __init__(self, colors = None, **kwargs):
+        super(e5_InfoScreen, self).__init__(**kwargs)
+        self.colors = colors if colors else ColorScheme()
+        layout = GridLayout(cols = 1, size_hint_y = 1, spacing = 5, padding = 5)
+        layout.add_widget(e5_scrollview_label(text = '', widget_id = 'content', colors = self.colors))
+        layout.add_widget(e5_side_by_side_buttons(['Back', 'Copy'],
+                                                    id = ['back_button', 'copy_button'],
+                                                    selected = [False, False],
+                                                    call_back = [self.go_back, self.copy],
+                                                    colors = self.colors))
+        self.add_widget(layout)
+        for widget in self.walk():
+            if hasattr(widget, 'id'):
+                if widget.id == 'content_label':
+                    self.content = widget
+                if widget.id == 'back_button':
+                    self.back_button = widget
 
-    def __init__(self, user_data_dir, **kwargs):
-        super(MainScreen, self).__init__(**kwargs)
+    def go_back(self, *args):
+        self.parent.current = 'MainScreen'
 
-        self.user_data_dir = user_data_dir
-        self.setup_logger()
+    def copy(self, instance):
+        Clipboard.copy(self.content.text)
 
-        self.colors = ColorScheme()
-        self.ini = INI()
-        self.cfg = CFG()
-        self.data = DB()
-
-        self.warnings, self.errors = self.setup_program()
-
-        self.station = totalstation(self.ini.get_value(__program__, 'STATION'))
-        self.station.setup(self.ini, self.data)
-        self.station.open()
-
-        self.cfg_datums = CFG()
-        self.cfg_datums.build_datum()
-        self.cfg_prisms = CFG()
-        self.cfg_prisms.build_prism()
-        self.cfg_units = CFG()
-        self.cfg_units.build_unit()
-
-        self.layout = BoxLayout(orientation = 'vertical',
-                                size_hint_y = .9,
-                                size_hint_x = .8,
-                                pos_hint={'center_x': .5},
-                                padding = 20,
-                                spacing = 20)
-        self.build_mainscreen()
-        self.add_widget(self.layout)
-        self.add_screens()
-        restore_window_size_position(__program__, self.ini)
 
-    def on_enter(self, *args):
-        if self.warnings or self.errors:
-            self.popup = self.warnings_and_errors_popup(self.warnings, self.errors)
-            self.popup.open()
-            self.errors, self.warnings = [], []
-        elif self.ini.first_time:
-            self.popup = e5_MessageBox('Welcome to EDM', __SPLASH_HELP__)
-            self.popup.open()
-            self.ini.first_time = False
+class e5_JSONScreen(e5_InfoScreen):
 
-    def setup_logger(self):
-        logger = logging.getLogger(__name__)
-        logger.setLevel(logging.INFO)
-        formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s', datefmt = '%Y-%m-%d %H:%M:%S')
-        fh = logging.FileHandler(os.path.join(self.user_data_dir, __program__ + '.log'))
-        fh.setLevel(logging.INFO)
-        fh.setFormatter(formatter)
-        logger.addHandler(fh)
-        logger.info(__program__ + ' started, logger initialized, and application built.')
-
-    def add_screens(self):
-        sm.add_widget(EditLastRecordScreen(name = 'EditLastRecordScreen',
-                                            colors = self.colors,
-                                            data = self.data,
-                                            doc_id = None,
-                                            e5_cfg = self.cfg))
-
-        sm.add_widget(VerifyStationScreen(name = 'VerifyStationScreen',
-                                            id = 'verify_station',
-                                            data = self.data,
-                                            station = self.station,
-                                            colors = self.colors,
-                                            ini = self.ini))
-
-        sm.add_widget(RecordDatumsScreen(name = 'RecordDatumsScreen',
-                                            data = self.data,
-                                            station = self.station,
-                                            colors = self.colors,
-                                            ini = self.ini))
-
-        sm.add_widget(EditPointScreen(name = 'EditPointScreen',
-                                            colors = self.colors,
-                                            data = self.data,
-                                            # data_table = self.data.table,
-                                            doc_id = None,
-                                            e5_cfg = self.cfg,
-                                            one_record_only = True))
-
-        sm.add_widget(EditPointsScreen(name = 'EditPointsScreen',
-                                            colors = self.colors,
-                                            main_data = self.data,
-                                            main_tablename = self.data.table,
-                                            main_cfg = self.cfg))
-
-        sm.add_widget(EditPointsScreen(name = 'EditDatumsScreen',
-                                            colors = self.colors,
-                                            main_data = self.data,
-                                            main_tablename = 'datums',
-                                            main_cfg = self.cfg_datums,
-                                            addnew = True))
-
-        sm.add_widget(EditPointsScreen(name = 'EditPrismsScreen',
-                                            colors = self.colors,
-                                            main_data = self.data,
-                                            main_tablename = 'prisms',
-                                            main_cfg = self.cfg_prisms,
-                                            addnew = True))
-
-        sm.add_widget(EditPointsScreen(name = 'EditUnitsScreen',
-                                            colors = self.colors,
-                                            main_data = self.data,
-                                            main_tablename = 'units',
-                                            main_cfg = self.cfg_units,
-                                            addnew = True))
-
-        sm.add_widget(StatusScreen(name = 'StatusScreen',
-                                            colors = self.colors,
-                                            cfg = self.cfg,
-                                            ini = self.ini,
-                                            data = self.data,
-                                            station = self.station))
-
-        sm.add_widget(e5_LogScreen(name = 'LogScreen',
-                                            colors = self.colors,
-                                            logger = logging.getLogger(__name__)))
-
-        sm.add_widget(e5_CFGScreen(name = 'CFGScreen',
-                                            colors = self.colors,
-                                            cfg = self.cfg))
-
-        sm.add_widget(e5_INIScreen(name = 'INIScreen',
-                                            colors = self.colors,
-                                            ini = self.ini))
+    def __init__(self, data = None, **kwargs):
+        super(e5_JSONScreen, self).__init__(**kwargs)
+        self.data = data
 
-        sm.add_widget(AboutScreen(name = 'AboutScreen',
-                                            colors = self.colors))
+    def on_pre_enter(self):
+        self.content.text = 'The last 150 lines:\n\n'
+        with open(self.data.filename, 'r') as f:
+            content = f.readlines()
+        # self.content.text += ''.join(list(reversed(content))[0:150])
+        self.content.text += ''.join(list(content)[-150:])
+        self.content.color = self.colors.text_color
+        self.back_button.background_color = self.colors.button_background
+        self.back_button.color = self.colors.button_color
 
-        sm.add_widget(StationConfigurationScreen(name = 'StationConfigurationScreen',
-                                                    station = self.station,
-                                                    ini = self.ini,
-                                                    colors = self.colors))
 
-        sm.add_widget(InitializeStationScreen(name = 'InitializeStationScreen',
-                                                    data = self.data,
-                                                    station = self.station,
-                                                    ini = self.ini,
-                                                    colors = self.colors))
+class e5_LogScreen(e5_InfoScreen):
 
-        sm.add_widget(e5_SettingsScreen(name = 'EDMSettingsScreen',
-                                        colors = self.colors,
-                                        ini = self.ini,
-                                        cfg = self.cfg))
+    def __init__(self, logger = None, **kwargs):
+        super(e5_LogScreen, self).__init__(**kwargs)
+        self.logger = logger
 
-        sm.add_widget(ComTestScreen(name = 'ComTestScreen',
-                                        colors = self.colors,
-                                        station = self.station,
-                                        cfg = self.cfg))
+    def on_pre_enter(self):
+        self.content.text = 'The last 150 lines:\n\n'
+        try:
+            with open(self.logger.handlers[0].baseFilename, 'r') as f:
+                content = f.readlines()
+            self.content.text += ''.join(list(reversed(content))[0:150])
+        except AttributeError:
+            self.content.text = '\nThe logger has not been initialized.'
+        except OSError:
+            self.content.text = "\nAn error occurred when reading the log file '%s'." % (self.logger.handlers[0].baseFilename)
+        self.content.color = self.colors.text_color
+        self.back_button.background_color = self.colors.button_background
+        self.back_button.color = self.colors.button_color
 
-    def reset_screens(self):
-        for screen in sm.screens[:]:
-            if screen.name != 'MainScreen':
-                sm.remove_widget(screen)
-        self.add_screens()
 
-    def build_mainscreen(self):
+class e5_INIScreen(e5_InfoScreen):
 
-        if platform_name() == 'Android':
-            size_hints = {'info': .13,
-                            'option_buttons': .8 - .13 - .2,
-                            'shot_buttons': .2}
-        else:
-            size_hints = {'info': .13,
-                            'option_buttons': .8 - .13 - .2,
-                            'shot_buttons': .2}
-
-        self.layout.clear_widgets()
-
-        self.info = e5_label(text = 'EDM',
-                                size_hint = (1, size_hints['info']),
-                                color = self.colors.text_color,
-                                id = 'lastshot',
-                                halign = 'center')
-        if self.colors:
-            if self.colors.text_font_size:
-                self.info.font_size = self.colors.text_font_size
-        self.layout.add_widget(self.info)
-        self.info.bind(texture_size = self.info.setter('size'))
-        self.info.bind(size_hint_min_x = self.info.setter('width'))
-
-        # grid = GridLayout(cols = 3, spacing = 10)
-        scroll_content = BoxLayout(orientation = 'horizontal',
-                                    size_hint = (1, size_hints['option_buttons']),
-                                    spacing = 20)
-        self.layout.add_widget(scroll_content)
-
-        button_count = 0
-        button_text = []
-        button_selected = []
-        for button_no in range(1, __BUTTONS__):
-            if self.cfg.get_value('BUTTON' + str(button_no), 'TITLE'):
-                button_text.append(self.cfg.get_value('BUTTON' + str(button_no), 'TITLE'))
-                button_selected.append(False)
-                button_count += 1
-
-        if button_count > 0:
-            self.scroll_menu = e5_scrollview_menu(button_text,
-                                                        menu_selected = button_selected,
-                                                        widget_id = 'buttons',
-                                                        call_back = [self.take_shot],
-                                                        ncols = 3,
-                                                        colors = self.colors)
-            scroll_content.add_widget(self.scroll_menu)
-
-        # if button_count % 3 !=0:
-        #    button_empty = Button(text = '', size_hint_y = None, id = '',
-        #                    color = self.colors.window_background,
-        #                    background_color = self.colors.window_background,
-        #                    background_normal = '')
-        #    scroll_content.add_widget(button_empty)
-
-        # if button_count % 3 == 2:
-        #    scroll_content.add_widget(button_empty)
-
-        # self.layout.add_widget(scroll_content)
-
-        shot_buttons = GridLayout(cols = 3, size_hint = (1, size_hints['shot_buttons']), spacing = 20)
-
-        shot_buttons.add_widget(e5_button(text = 'Record',
-                                            id = 'record',
-                                            colors = self.colors, call_back = self.take_shot, selected = True))
-
-        shot_buttons.add_widget(e5_button(text = 'Continue',
-                                            id = 'continue',
-                                            colors = self.colors, call_back = self.take_shot, selected = True))
-
-        shot_buttons.add_widget(e5_button(text = 'Measure',
-                                            id = 'measure',
-                                            colors = self.colors, call_back = self.take_shot, selected = True))
+    def __init__(self, ini = None, **kwargs):
+        super(e5_INIScreen, self).__init__(**kwargs)
+        self.ini = ini
 
-        self.layout.add_widget(shot_buttons)
+    def on_pre_enter(self):
+        with open(self.ini.filename, 'r') as f:
+            self.content.text = f.read()
+        self.content.color = self.colors.text_color
+        self.back_button.background_color = self.colors.button_background
+        self.back_button.color = self.colors.button_color
 
-        self.update_title()
 
-        if self.cfg.filename:
-            if self.cfg.has_warnings or self.cfg.has_errors:
-                self.event = Clock.schedule_once(self.show_popup_message, 1)
+class e5_CFGScreen(e5_InfoScreen):
 
-    def update_title(self):
-        for widget in self.walk():
-            if hasattr(widget, 'action_previous'):
-                widget.action_previous.title = 'EDM'
-                if self.cfg is not None:
-                    if self.cfg.filename:
-                        widget.action_previous.title = filename_only(self.cfg.filename)
-
-    def message_open_cfg_first(self):
-        message = '\nBefore you can do this, you need to open a CFG file (see option under File menu).  Opening a CFG file will also open your database. '
-        message += 'If you do not have a CFG file already, you can use a default one (see option under File menu).  Later you can alter the default CFG to '
-        message += 'add additional options specific to your work.'
-        return(e5_MessageBox('EDM', message))
-
-    def ready_to_use(self):
-        return(self.cfg is not None and self.data.filename != '')
-
-    def take_shot(self, instance):
-        if not self.ready_to_use() and instance.id != 'measure':
-            self.popup = self.message_open_cfg_first()
-        else:
-            self.station.shot_type = instance.id
-            self.station.clear_xyz()
-            if self.station.make == 'Microscribe':
-                self.popup = DataGridTextBox(title = 'EDM', text = '<Microscribe>',
-                                                label = 'Waiting on...',
-                                                button_text = ['Cancel', 'Next'],
-                                                call_back = self.have_shot,
-                                                colors = self.colors)
-            elif self.station.make in ['Manual XYZ', 'Manual VHD']:
-                self.popup = edm_manual(type = self.station.make, call_back = self.have_shot_manual, colors = self.colors)
-            else:
-                self.station.take_shot()
-                self.popup = self.get_prism_height()
-        self.popup.open()
+    def __init__(self, cfg = None, **kwargs):
+        super(e5_CFGScreen, self).__init__(**kwargs)
+        self.cfg = cfg
 
-    def have_shot_manual(self, instance):
-        # check that next was pressed and get values
-        if self.popup.xcoord and self.popup.ycoord and self.popup.zcoord:
-            p = self.station.text_to_point(f'{self.popup.xcoord.text},{self.popup.ycoord.text},{self.popup.zcoord.text}')
-            if p:
-                self.station.xyz = p
-                self.station.make_global()
-                self.station.vhd_from_xyz()
-        elif self.popup.hangle and self.popup.vangle and self.popup.sloped:
+    def on_pre_enter(self):
+        if self.cfg.filename:
             try:
-                self.station.hangle = float(self.popup.hangle.text)
-                self.station.vangle = float(self.popup.vangle.text)
-                self.station.sloped = float(self.popup.sloped.text)
-            except ValueError:
-                self.station.xyz = point()
-            self.station.vhd_to_xyz()
-            self.station.make_global()
-        self.station.pnt = None
-        self.popup.dismiss()
-        if self.station.xyz.x is None or self.station.xyz.y is None or self.station.xyz.z is None:
-            self.popup = e5_MessageBox('Recording error', '\nInvalid value(s) were given.  Point not recorded.', call_back = self.close_popup)
+                with open(self.cfg.filename, 'r') as f:
+                    self.content.text = f.read()
+            except OSError:
+                self.content.text = "There was an error reading from the CFG file '%s'" % self.cfg.filename
         else:
-            self.popup = self.get_prism_height()
-        self.popup.open()
-        self.popup_open = True
+            self.content.text = '\nOpen a CFG file before trying to view it.'
+        self.content.color = self.colors.text_color
+        self.back_button.background_color = self.colors.button_background
+        self.back_button.color = self.colors.button_color
 
-    def get_prism_height(self):
-        prism_names = self.data.names('prisms')
-        if len(prism_names) > 0:
-            return(DataGridMenuList(title = "Select or Enter a Prism Height",
-                                            menu_list = prism_names,
-                                            menu_selected = self.station.prism.name,
-                                            call_back = self.have_shot,
-                                            colors = self.colors))
-        else:
-            return(DataGridTextBox(title = 'Enter a Prism Height',
-                                        text = str(self.station.prism.height) if self.station.prism.height else '0',
-                                        call_back = self.have_shot,
-                                        button_text = ['Back', 'Next'],
-                                        colors = self.colors))
-
-    def have_shot(self, instance):
-        if self.station.make == 'Microscribe':
-            result = self.popup.result
-            if result:
-                p = self.station.text_to_point(result)
-                if p:
-                    p.x = p.x / 1000.0
-                    p.y = p.y / 1000.0
-                    p.z = p.z / 1000.0
-                    self.station.xyz = p
-                    self.station.make_global()
-        else:
-            prism_name = instance.text
-            if prism_name == 'Add' or prism_name == 'Next':
-                try:
-                    self.station.prism = prism(None, float(self.popup.txt.text), None)
-                except ValueError:
-                    self.station.prism = prism()
-            else:
-                self.station.prism = self.data.get_prism(prism_name)
-            if self.station.prism.height is None:
-                self.popup.dismiss()
-                self.popup = e5_MessageBox('Error', '\nInvalid prism height provided.  Shot not recorded.', call_back = self.close_popup)
-                self.popup.open()
-                self.popup_open = True
-                return
-            else:
-                if self.station.make in ['Leica']:
-                    self.station.fetch_point()
-                    self.station.make_global()
-                elif self.station.make in ['Simulate']:
-                    self.station.pnt = None
-                elif self.station.make in ['Manual XYZ', 'Manual VHD']:
-                    self.station.pnt = None
-                self.station.prism_adjust()
-        self.popup.dismiss()
 
-        if self.station.xyz.x is not None and self.station.xyz.y is not None and self.station.xyz.z is not None:
-            if self.station.shot_type == 'measure':
-                txt = f'\nCoordinates:\n  X:  {self.station.xyz_global.x:.3f}\n  Y:  {self.station.xyz_global.y:.3f}\n  Z:  {self.station.xyz_global.z:.3f}'
-                unitname = self.data.point_in_unit(self.station.xyz_global)
-                if unitname:
-                    txt += f'\n\nThe point is in unit {unitname}.'
-                if self.station.make != 'Microscribe':
-                    txt += f'\n\nMeasurement Data:\n  Horizontal angle:  {self.station.decimal_degrees_to_sexa_pretty(self.station.hangle)}\n  Vertical angle:  {self.station.decimal_degrees_to_sexa_pretty(self.station.vangle)}\n  Slope distance:  {self.station.sloped:.3f}'
-                    txt += f'\n  X:  {self.station.xyz.x:.3f}\n  Y:  {self.station.xyz.y:.3f}\n  Z:  {self.station.xyz.z:.3f}'
-                    txt += f'\n\nStation coordinates:\n  X:  {self.station.location.x:.3f}\n  Y:  {self.station.location.y:.3f}\n  Z:  {self.station.location.z:.3f}'
-                    if self.station.prism_constant:
-                        txt += f'\n\nPrism constant :  {self.station.prism_constant} m'
-                    if self.station.pnt:
-                        txt += f'\n\nData stream:\n  {self.station.pnt}'
-                self.popup = e5_MessageBox('Measurement', txt,
-                                            response_type = "OK",
-                                            call_back = self.close_popup,
-                                            colors = self.colors)
-                self.popup.open()
-            else:
-                self.add_point_record()
-                # TODO self.station.prism = self.data.prisms.get(value.text).height
-                if self.data.db is not None:
-                    self.data.db.table(self.data.table).on_save = self.on_save
-                    self.data.db.table(self.data.table).on_cancel = self.on_cancel
-                self.parent.current = 'EditPointScreen'
-        else:
-            self.popup = e5_MessageBox(title = 'Error', message = '\nPointed not recorded.')
+class e5_LoadDialog(FloatLayout):
+    start_path = ObjectProperty(None)
+    load = ObjectProperty(None)
+    cancel = ObjectProperty(None)
+    button_color = ObjectProperty(None)
+    button_background = ObjectProperty(None)
+    filters = ObjectProperty(['*.cfg', '*.CFG'])
+    font_size = ObjectProperty(None)
+
+
+class e5_SaveDialog(BoxLayout):
+    save = ObjectProperty(None)
+    cancel = ObjectProperty(None)
+    start_path = ObjectProperty(None)
+    filename = ObjectProperty(None)
+    path = ObjectProperty(None)
+
+    def __init__(self, colors = None, **kwargs):
+        super(e5_SaveDialog, self).__init__(**kwargs)
+        self.colors = colors if colors else ColorScheme()
+
+        content = BoxLayout(orientation = 'vertical', padding = 5, spacing = 5)
+        self.pathlabel = e5_textinput(text = self.start_path, background_color = (0, 0, 0, 0), foreground_color = (1, 1, 1, .8), size_hint = (1, None))
+        self.pathlabel.bind(minimum_height = self.pathlabel.setter('height'))
+        content.add_widget(self.pathlabel)
+        self.filesaver = FileChooserListView(path = self.start_path)
+        self.filesaver.bind(selection = self.path_selected)
+        self.filesaver.bind(path = self.path_changed)
+        content.add_widget(self.filesaver)
+
+        self.txt = TextInput(text = self.filename,
+                                multiline = False,
+                                size_hint = (1, None))
+        #                        id = 'filename')
+        self.txt.bind(text = self.update_filename)
+        self.txt.bind(minimum_height = self.txt.setter('height'))
+        content.add_widget(self.txt)
+
+        content.add_widget(e5_side_by_side_buttons(text = ['Cancel', 'Save'],
+                                                    id = ['cancel', 'save'],
+                                                    call_back = [self.cancel, self.does_file_exist],
+                                                    selected = [True, True],
+                                                    colors = self.colors))
+
+        self.add_widget(content)
+        self.path = self.start_path
+
+    def update_filename(self, instance, value):
+        self.filename = value
+
+    def path_changed(self, instance, value):
+        self.path = instance.path
+        self.pathlabel.text = instance.path
+
+    def path_selected(self, instance, value):
+        self.path = instance.path
+        self.txt.text = ntpath.split(value[0])[1] if value else ''
+
+    def does_file_exist(self, instance):
+        filename = os.path.join(self.path, self.filename)
+        if os.path.isfile(filename):
+            self.popup = e5_MessageBox('Overwrite existing file?', '\n You are about to overwrite an existing file - %s.\n\n Continue?' % filename,
+                                        response_type = "YESNO",
+                                        call_back = [self.overwrite_file, self.close_popup],
+                                        colors = self.colors)
             self.popup.open()
+        else:
+            self.save(self)
 
-    def on_save(self):
-        self.log_the_shot()
-        self.update_info_label()
-        self.make_backup()
-        self.check_for_duplicate_xyz()
-        return([])
-
-    def log_the_shot(self):
-        logger = logging.getLogger(__name__)
-        logger.info(f'{self.get_last_squid()} {self.station.vhd_to_sexa_pretty_compact()} with prism height {self.station.prism.height} from {self.station.location} ')
-
-    def on_cancel(self):
-        if self.data.db is not None:
-            last_record = self.data.db.table(self.data.table).all()[-1]
-            if last_record != []:
-                self.data.db.table(self.data.table).remove(doc_ids = [last_record.doc_id])
-
-    def get_last_squid(self):
-        unit = self.get_last_value('UNIT')
-        idno = self.get_last_value('ID')
-        suffix = self.get_last_value('SUFFIX')
-        if unit is not None and idno is not None and suffix is not None:
-            return(f'{unit}-{idno}({suffix})')
-        else:
-            return('')
-
-    def update_info_label(self):
-        last_squid = self.get_last_squid()
-        self.info.text = last_squid if last_squid else 'EDM'
-
-    def check_for_duplicate_xyz(self):
-        if self.station.make == 'Microscribe' and self.data.db is not None:
-            if len(self.data.db.table(self.data.table)) > 1:
-                last_record = self.data.db.table(self.data.table).all()[-1]
-                next_to_last_record = self.data.db.table(self.data.table).all()[-2]
-                if 'X' in last_record.keys() and 'Y' in last_record.keys() and 'Z' in last_record.keys():
-                    if last_record['X'] == next_to_last_record['X'] and last_record['Y'] == next_to_last_record['Y'] and last_record['Z'] == next_to_last_record['Z']:
-                        self.popup = e5_MessageBox(title = 'Warning', message = f"\nThe last two recorded points have the exact same XYZ coordinates ({last_record['X']}, {last_record['Y']}, {last_record['Z']}).  Verify that the Microscribe is still properly recording points (green light is on).  If the red light is on, you need to re-initialize (Setup - Initialize Station) and re-shoot the last two points.")
-                        self.popup.open()
+    def overwrite_file(self, instance):
+        self.popup.dismiss()
+        self.save(instance)
 
     def close_popup(self, instance):
         self.popup.dismiss()
 
-    def save_default_cfg(self):
-        content = e5_SaveDialog(filename = '',
-                                start_path = self.cfg.path,
-                                save = self.save_default,
-                                cancel = self.dismiss_popup)
-        self.popup = Popup(title = "Create a new default CFG file",
-                            content = content,
-                            size_hint = (0.9, 0.9))
-        self.popup.open()
-        self.popup_open = True
 
-    def save_default(self, *args):
-        path = self.popup.content.filesaver.path
-        filename = self.popup.content.filename
-        if '.cfg' not in filename.lower():
-            filename = filename + '.cfg'
-        self.cfg.initialize()
-        self.cfg.build_default()
-        self.ini.update_value(__program__, 'CFG', os.path.join(path, filename))
-        self.cfg.update_value(__program__, 'DATABASE', os.path.join(path, filename.split('.')[0] + '.json'))
-        self.cfg.update_value(__program__, 'TABLE', filename.split('.')[0])
-        self.data.open(os.path.join(path, filename.split('.')[0] + '.json'))
-        self.open_db()
-        self.set_new_data_to_true()
-        self.cfg.filename = os.path.join(path, filename)
-        self.cfg.save()
-        self.ini.update(self.colors, self.cfg)
-        self.dismiss_popup()
-        self.build_mainscreen()
-        self.reset_screens()
-
-    def set_new_data_to_true(self, table_name = None):
-        if table_name is None:
-            self.data.new_data['prisms'] = True
-            self.data.new_data['units'] = True
-            self.data.new_data['datums'] = True
-            self.data.new_data[self.data.table] = True
-        else:
-            self.data.new_data[table_name] = True
+class e5_RecordEditScreen(Screen):
 
-    def show_load_cfg(self):
-        if self.cfg.filename and self.cfg.path:
-            start_path = self.cfg.path
-        else:
-            start_path = self.ini.get_value(__program__, 'APP_PATH')
-        if not os.path.exists(start_path):
-            start_path = os.path.abspath(os.path.dirname(__file__))
-        content = e5_LoadDialog(load = self.load_cfg,
-                                cancel = self.dismiss_popup,
-                                start_path = start_path,
-                                button_color = self.colors.button_color,
-                                button_background = self.colors.button_background)
-        self.popup = Popup(title = "Load CFG file", content = content,
-                            size_hint = (0.9, 0.9))
-        self.popup.open()
+    can_update_data_table = False
+    first_field_widget = ObjectProperty(None)
 
-    def load_cfg(self, path, filename):
-        warnings, errors = [], []
-        self.data.close()
-        self.dismiss_popup()
-        self.cfg.load(os.path.join(path, filename[0]))
-        if self.cfg.filename:
-            warnings, errors = self.open_db()
-            if errors == []:
-                self.set_new_data_to_true()
-        self.ini.update(self.colors, self.cfg)
-        self.build_mainscreen()
-        self.reset_screens()
-        if warnings or errors:
-            self.popup = self.warnings_and_errors_popup(warnings, errors)
-            self.popup.open()
+    def __init__(self, data = None,
+                        doc_id = None,
+                        e5_cfg = None,
+                        colors = None,
+                        one_record_only = False,
+                        **kwargs):
+        super(e5_RecordEditScreen, self).__init__(**kwargs)
+        self.colors = colors if colors is not None else ColorScheme()
+        self.e5_cfg = e5_cfg
+        self.data = data
+        self.doc_id = doc_id
+        self.one_record_only = one_record_only
+        self.can_update_data_table = False
+        self.layout = GridLayout(cols = 1,
+                                 size_hint_y = .9,
+                                 size_hint_x = width_calculator(.9, 600),
+                                 spacing = 5,
+                                 padding = 5,
+                                 pos_hint={'center_x': .5, 'center_y': .5})
+        if self.one_record_only:
+            self.record_counter_label = None
+        else:
+            self.record_counter_label = e5_label('Record counter', size_hint = (1, .08), halign = 'center')
+            self.layout.add_widget(self.record_counter_label)
+        self.data_fields = GridLayout(cols = 1, size_hint_y = None, spacing = 5, padding = 5)
+        self.make_empty_frame()
+        scroll = ScrollView(size_hint = (1, 1))
+        scroll.add_widget(self.data_fields)
+        self.layout.add_widget(scroll)
+        if not self.one_record_only:
+            self.layout.add_widget(e5_side_by_side_buttons(text = ['First', 'Previous', 'Next', 'Last'],
+                                                            id = ['first', 'previous', 'next', 'last'],
+                                                            call_back = [self.first_record, self.previous_record,
+                                                                         self.next_record, self.last_record],
+                                                            selected = [True, True, True, True],
+                                                            colors = self.colors))
+            back_and_filter = e5_side_by_side_buttons(text = ['Back', 'Save', 'Filter'],
+                                                            id = ['back', 'save', 'filter'],
+                                                            call_back = [self.call_back, self.save_record, self.filter],
+                                                            selected = [True, True, True],
+                                                            colors = self.colors)
+            self.filter_button = back_and_filter.children[0]
+            self.layout.add_widget(back_and_filter)
+        else:
+            self.layout.add_widget(e5_side_by_side_buttons(text = ['Cancel', 'Save'],
+                                                            id = ['cancel', 'save'],
+                                                            call_back = [self.cancel_record, self.save_record_and_exit],
+                                                            selected = [True, True],
+                                                            colors = self.colors))
 
-    def reset_screen_defaults(self):
-        sm.get_screen('EditPointScreen').e5_cfg = self.cfg
-        sm.get_screen('EditPointScreen').data_table = self.data.table
-        sm.get_screen('EditPointScreen').data = self.data
-        sm.get_screen('EditLastRecordScreen').data_table = self.data.table
-
-    def show_import_csv(self):
-        if not self.ready_to_use():
-            self.popup = self.message_open_cfg_first()
-        else:
-            instructions = 'EDM can import data from EDM-Mobile, EDMWin, EDM itself, or user prepared data files.  The two import formats are CSV and JSON.  CSV files should have a csv or txt extension.  JSON files should have a json extension.'
-            instructions += ' See our web site for more information on exporting data from EDM-Mobile and EDMWin.  The JSON option is for easy importing from EDM data files.'
-            instructions += ' Importing points from JSON files is not yet available. IMPORT: Imported data will overwrite existing data in the case of duplicates.'
-            self.popup = e5_PopUpMenu(title = "Load which kind of data", message = instructions,
-                                            menu_list = ['Points', 'Datums', 'Prisms', 'Units'],
-                                            menu_selected = '',
-                                            call_back = self.select_csv_file,
-                                            colors = self.colors)
-        self.popup.open()
+        self.add_widget(self.layout)
+        self.filter_field = 'Unit-ID'
+        self.loading = True
 
-    def show_csv_datatype(self):
-        if not self.ready_to_use():
-            self.popup = self.message_open_cfg_first()
-        else:
-            self.popup = e5_PopUpMenu(title = "Export which kind of data", message = '',
-                                            menu_list = ['Points', 'Datums', 'Prisms', 'Units'],
-                                            menu_selected = '',
-                                            call_back = self.show_save_csvs,
-                                            colors = self.colors)
-        self.popup.open()
+    def on_pre_enter(self):
+        self.loading = True
+        if self.data.table is not None and self.e5_cfg is not None:
+            self.reset_doc_ids()
+            self.doc_id = self.doc_ids[-1] if self.doc_ids else None
+        else:
+            self.doc_ids = []
+            self.doc_id = None
+        self.put_data_in_frame()
 
-    def select_csv_file(self, instance):
-        self.csv_data_type = instance.text
-        self.popup.dismiss()
-        if self.cfg.filename and self.cfg.path:
-            start_path = self.cfg.path
+    def on_enter(self):
+        if self.first_field_widget:
+            self.first_field_widget.focus = True
+        self.loading = False
+        self.changes_made = False
+
+    def on_leave(self):
+        # This helps insure that saving on lost focus works properly
+        # There is an issue this addresses with building the screens
+        # at startup.
+        self.loading = True
+
+    def reset_doc_ids(self):
+        self.doc_ids = [r.doc_id for r in self.data.db.table(self.data.table).all()] if self.data.db is not None else []
+
+    def filter(self, instance):
+        if instance.text == 'Clear Filter':
+            instance.text = 'Filter'
+            self.reset_doc_ids()
+            self.last_record(None)
+            # self.update_record_counter_label()
         else:
-            start_path = self.ini.get_value('EDM', 'APP_PATH')
-        content = e5_LoadDialog(load = self.load_csv,
-                                cancel = self.dismiss_popup,
-                                start_path = start_path,
-                                button_color = self.colors.button_color,
-                                button_background = self.colors.button_background,
-                                filters = ['*.csv', '*.CSV', '*.txt', '*.TXT', '*.json', '*.JSON'])
-        self.popup = Popup(title = "Select CSV or JSON file to import from",
-                            content = content,
-                            size_hint = (0.9, 0.9))
-        self.popup.open()
-
-    def read_csv_file(self, full_filename):
-        data = []
-        with open(full_filename, newline='') as csvfile:
-            reader = csv.DictReader(csvfile, quoting = csv.QUOTE_NONNUMERIC)
-            for row in reader:
-                data.append(row)
-        fields = [field.upper() for field in reader.fieldnames]
-        return(fields, data)
+            self.popup = db_filter(default_field = self.filter_field, fields = ['doc_id', 'Unit-ID'] + self.e5_cfg.fields(),
+                                    colors = self.colors, call_back = self.apply_filter)
+            self.popup.open()
 
-    def read_json_table(self, full_filename, data_type):
-        data = []
-        if data_type.upper() in ['DATUMS', 'UNITS', 'PRISMS']:
-            data = TinyDB(full_filename).table(data_type.lower()).all()
-        fields = data[0].keys() if data else []
-        return(fields, data)
-
-    def check_import_fields_against_cfg_fields(self, fields):
-        cfg_fields = self.cfg.fields()
-        missing_fields = [field for field in fields if field not in cfg_fields]
-        missing_fields = [field for field in missing_fields if field not in ['RECNO', 'TIME']]
-        if missing_fields:
-            return(f"The following field(s) are present in the import data but not in the current CFG: {', '.join(missing_fields)}. Importing these data could cause the loss of data.  Please add these missing fields to the CFG before importing these data.")
+    def get_matching_doc_ids(self, filter_field, filter_value):
+        matches = []
+        if filter_field == 'doc_id':
+            matches = self.data.db.table(self.data.table).get(doc_id = filter_value)
+        elif filter_field == 'Unit-ID':
+            for record in self.data.db.table(self.data.table):
+                if "UNIT" in record.keys() and "ID" in record.keys():
+                    if f"{str(record['UNIT']).lower()}-{str(record['ID']).lower()}" == filter_value.lower():
+                        matches.append(record.doc_id)
         else:
-            return("")
-
-    def get_unique_key(self, data_record):
-        unique_key = []
-        for field in self.cfg.unique_together:
-            unique_key.append("%s" % data_record[field])
-        return(",".join(unique_key))
-
-    def check_unique_together(self, data_record):
-        if self.data.db is not None:
-            if self.cfg.unique_together and len(self.data.db.table(self.data.table)) > 1:
-                unique_key = self.get_unique_key(data_record)
-                for doc_id in self.data.doc_ids():
-                    if unique_key == self.get_unique_key(self.data.db.table(self.data.table).get(doc_id = doc_id)):
-                        return(doc_id)
-        return('')
-
-    def error_check_import(self, fields):
-        errors = ''
-        if self.csv_data_type == 'Datums':
-            if len(fields) < 4:
-                errors = f'\nThese data seem to have fewer than four fields.  To import datums requires a Name, X, Y, and Z field.  If this is a CSV file, the first row in the file should contain these field names separated by commas.  The fieldnames read were {fields}.'
-            if 'X' not in fields or 'Y' not in fields or 'Z' not in fields or 'NAME' not in fields:
-                errors = f'\nIf these data are coming from a CSV file, the first row must list the field names (comma delimited) and must include a field called Name, X, Y and Z.  The fields read were {fields}.'
-        if self.csv_data_type == 'Prisms':
-            if len(fields) < 2:
-                errors = f'\nThese data seem to have fewer than two fields.  To import prisms requires a Name and height and optionally an offset field.  If this is a csv file, the first row in the file should contain these field names separated by commas.  The fieldnames read were {fields}.'
-            if 'NAME' not in fields or 'HEIGHT' not in fields:
-                errors = f'\nIf these data are coming from a CSV file, the first row must list the field names (comma delimited) and must include a field called Name and Height.  The fields read were {fields}.'
-        if self.csv_data_type == 'Units':
-            if len(fields) < 5:
-                errors = f'\nThese data seem to have fewer than five fields.  To import units requires a Unit, Minx, Miny, Maxx, Maxy field.  If this is a CSV file, the first row in the file should contain these field names separated by commas.  The fieldnames read were {fields}.'
-            if 'UNIT' not in fields or 'MINX' not in fields or 'MINY' not in fields or 'MAXX' not in fields or 'MAXY' not in fields:
-                errors = f'\nIf these data are coming from a CSV file, the first row must list the field names (comma delimited) and must include at least fields called Unit, Minx, Miny, Maxx, Maxy.  The fields read were {fields}.'
-        if self.csv_data_type == 'Points':
-            errors = self.check_import_fields_against_cfg_fields(fields)
-        return(errors)
-
-    def build_hash_unique_ids(self):
-        hash = {}
-        if self.data.db is not None:
             for record in self.data.db.table(self.data.table):
-                hash[self.get_unique_key(record)] = record.doc_id
-        return(hash)
+                if str(record[filter_field]).lower() == filter_value.lower():
+                    matches.append(record.doc_id)
+        return matches
+
+    def apply_filter(self, instance):
+        self.filter_field = self.popup.fields_dropdown.text
+        filter_value = self.popup.value_input.text
+        if filter_value and self.filter_field:
+            self.doc_ids = self.get_matching_doc_ids(self.filter_field, filter_value)
+            if self.doc_ids:
+                self.first_record(None)
+            else:
+                self.clear_the_frame()
+                self.doc_id = None
+                self.update_record_counter_label()
+            self.filter_button.text = 'Clear Filter'
+        else:
+            self.filter_button.text = 'Filter'
+        self.popup.dismiss()
 
-    def import_these(self, data):
-        record_count = 0
-        replacements = 0
-        hash_unique_ids = self.build_hash_unique_ids()
-        if self.data.db is not None:
-            for item in data:
-                insert_record = {}
-                for key, value in item.items():
-                    if key.upper() == "UNIT" and self.csv_data_type == "Units":
-                        insert_record['NAME'] = value
-                    elif key.upper() == "DATE" and "TIME" in item:
-                        insert_record['DATE'] = value + " " + item['TIME']
-                    else:
-                        insert_record[key.upper()] = value
-                if self.csv_data_type in ['Datums', 'Prisms', 'Units']:
-                    if insert_record['NAME'].strip():
-                        if len(self.data.get_by_name(self.csv_data_type.lower(), insert_record['NAME'])) > 0:
-                            self.data.delete_by_name(self.csv_data_type.lower(), insert_record['NAME'])
-                            replacements += 1
-                        self.data.db.table(self.csv_data_type.lower()).insert(insert_record)
-                if self.csv_data_type == 'Points':
-                    new_docid = self.data.db.table(self.data.table).insert(insert_record)
-                    hash_key = self.get_unique_key(insert_record)
-                    if hash_key in hash_unique_ids:
-                        duplicate_doc_id = hash_unique_ids[hash_key]
-                        self.data.db.table(self.data.table).remove(doc_ids = [duplicate_doc_id])
-                        replacements += 1
-                    hash_unique_ids[hash_key] = new_docid
-                record_count += 1
-        return((record_count, replacements))
-
-    def load_csv(self, path, filename):
-        # TODO This routine does not properly import Units.  The unitfields need to be put into a separate table
-        # TODO Need to write the routine to import actual data
-        full_filename = os.path.join(path, filename[0])
-        self.dismiss_popup()
-
-        if '.csv' in full_filename.lower() or '.txt' in full_filename.lower():
-            fields, data = self.read_csv_file(full_filename)
-        else:
-            fields, data = self.read_json_table(full_filename, self.csv_data_type)
-
-        errors = self.error_check_import(fields)
-
-        if not errors:
-            record_count, replacements = self.import_these(data)
-
-        if errors:
-            message = errors
-        else:
-            if replacements == 0:
-                message = '%s %s successfully imported.' % (record_count, self.csv_data_type)
-            else:
-                message = '%s %s successfully imported.  Of these, %s updated an existing record.' % (record_count, self.csv_data_type, replacements)
-
-        self.popup = e5_MessageBox('CSV Import', message,
-                                    response_type = "OK",
-                                    call_back = self.close_popup,
+    def make_empty_frame(self):
+        self.data_fields.bind(minimum_height = self.data_fields.setter('height'))
+        self.data_fields.clear_widgets()
+        fields = self.e5_cfg.fields()
+        self.first_field_widget = None
+        if fields:
+            first_field = True
+            for col in fields:
+                field_type = self.e5_cfg.get_value(col, 'TYPE')
+                field_length = self.e5_cfg.get_value(col, 'LENGTH')
+                field_length = int(field_length) if self.is_numeric(field_length) else 0
+                widget = DataGridLabelAndField(col = col, prompt = self.e5_cfg.get_value(col, 'PROMPT'),
+                                                colors = self.colors, note_field = (field_type == 'NOTE'),
+                                                text_length = field_length)
+                self.data_fields.add_widget(widget)
+                if first_field:
+                    if field_type not in ['MENU', 'BOOLEAN']:
+                        self.first_field_widget = widget.txt
+                    first_field = False
+
+    def leave_record_without_save(self, instance):
+        self.changes_made = False
+        self.close_popup(None)
+        self.continue_on_with(None)
+
+    def ask_about_saving(self):
+        self.popup = e5_MessageBox('Leave without saving', '\nLeave this record without saving changes?',
+                                    response_type = "YESNO",
+                                    call_back = [self.leave_record_without_save, self.close_popup],
                                     colors = self.colors)
-        self.open_popup()
-        return(errors)
+        self.popup.open()
 
-    def add_point_record(self):
-        new_record = {}
-        new_record = self.fill_default_fields(new_record)
-        if self.station.shot_type != 'continue':
-            new_record = self.find_unit_and_fill_fields(new_record)
-            new_record = self.fill_carry_fields(new_record)
-            new_record = self.fill_link_fields(new_record)
-            new_record = self.do_increments(new_record)
-            new_record['SUFFIX'] = 0
-            new_record = self.fill_button_defaults(new_record)
-        else:
-            new_record = self.fill_empty_with_last(new_record)
-            new_record['SUFFIX'] = int(self.get_last_value('SUFFIX')) + 1
+    def first_record(self, value):
+        if self.doc_ids:
+            if self.changes_made:
+                self.continue_on_with = self.first_record
+                self.ask_about_saving()
+            else:
+                self.doc_id = self.doc_ids[0]
+                self.put_data_in_frame()
+
+    def previous_record(self, value):
+        if self.doc_ids:
+            if self.changes_made:
+                self.continue_on_with = self.previous_record
+                self.ask_about_saving()
+            else:
+                current = self.doc_ids.index(self.doc_id)
+                new = max(current - 1, 0)
+                self.doc_id = self.doc_ids[new]
+                self.put_data_in_frame()
+
+    def next_record(self, value):
+        if self.doc_ids:
+            if self.changes_made:
+                self.continue_on_with = self.next_record
+                self.ask_about_saving()
+            else:
+                current = self.doc_ids.index(self.doc_id)
+                new = min(current + 1, len(self.doc_ids) - 1)
+                self.doc_id = self.doc_ids[new]
+                self.put_data_in_frame()
+
+    def last_record(self, value):
+        if self.doc_ids:
+            if self.changes_made:
+                self.continue_on_with = self.last_record
+                self.ask_about_saving()
+            else:
+                self.doc_id = self.doc_ids[-1]
+                self.put_data_in_frame()
+
+    def update_record_counter_label(self):
+        if self.record_counter_label:
+            if self.doc_id:
+                current = self.doc_ids.index(self.doc_id) + 1
+                self.record_counter_label.text = f'Viewing record {current} of {len(self.doc_ids)} (doc_id={self.doc_id})'
+            else:
+                self.record_counter_label.text = 'No matching records'
+
+    def clear_the_frame(self):
+        self.can_update_data_table = False
+        if self.e5_cfg:
+            fields = self.e5_cfg.fields()
+            for widget in self.layout.walk():
+                if hasattr(widget, 'id'):
+                    if widget.id in fields:
+                        widget.text = ''
+
+    def put_data_in_frame(self):
+        self.clear_the_frame()
+        if self.doc_id and self.data.table and self.e5_cfg:
+            data_record = self.data.db.table(self.data.table).get(doc_id = self.doc_id)
+            if data_record:
+                for field in self.e5_cfg.fields():
+                    for widget in self.layout.walk():
+                        if hasattr(widget, 'id'):
+                            if widget.id == field:
+                                widget.text = '%s' % data_record[field] if field in data_record.keys() else ''
+                                widget.bind(text = self.flag_changes_made)
+                                widget.bind(on_text_validate = self.check_for_prism_change)
+                                if widget.id == "PRISM":
+                                    widget.bind(focus = self.show_prisms)
+                                else:
+                                    widget.bind(focus = self.show_menu)
+                                break
+        self.can_update_data_table = True
+        self.update_record_counter_label()
+        self.changes_made = False
+
+    def check_for_prism_change(self, instance):
+        if instance.id == 'PRISM':
+            if not self.is_numeric(instance.text) and instance.text != '':
+                self.popup = e5_MessageBox('Invalid entry',
+                                            '\nPrism height must be a valid number.',
+                                            response_type = "OK",
+                                            call_back = self.close_popup,
+                                            colors = self.colors)
+                self.popup.open()
+                return
+            prism_height_new = float(instance.text) if self.is_numeric(instance.text) else 0.0
+            if prism_height_new != self.prism_height_old:
+                z = self.get_widget_by_id(self, 'Z')
+                if z:
+                    z_old = float(z.text)
+                    self.z_new = z_old + self.prism_height_old - prism_height_new
+                    message = f"\nUpdate the Z as well from {round(z_old, 3)} to {round(self.z_new, 3)}?"
+                    self.popup = e5_MessageBox('Update', message,
+                                                    response_type = "YESNO",
+                                                    call_back = [self.update_z, self.close_popup],
+                                                    colors = self.colors)
+                    self.popup.open()
+
+    def flag_changes_made(self, instance, value):
+        self.changes_made = True
+
+    def check_numeric(self, instance, value):
+        cfg_field = self.e5_cfg.get(instance.id)
+        if cfg_field.inputtype in ['NUMERIC', 'INSTRUMENT']:
+            if not self.is_numeric(value):
+                return [f'{instance.id} is listed as a numeric field in the CFG file but the value {value} is not a valid number.']
+            else:
+                return []
+        else:
+            return []
+
+    def update_db(self, *args):
+        if self.doc_id and self.data.table and self.e5_cfg and self.can_update_data_table:
+            update = {}
+            for field in self.e5_cfg.fields():
+                for widget in self.layout.walk():
+                    if hasattr(widget, 'id'):
+                        if widget.id == field:
+                            if self.e5_cfg.save_as_numeric_field(field):
+                                if '.' in widget.text:
+                                    update[widget.id] = float(widget.text)
+                                else:
+                                    update[widget.id] = int(widget.text)
+                            else:
+                                update[widget.id] = widget.text
+                            break
+            self.data.db.table(self.data.table).update(update, doc_ids = [self.doc_id])
+            self.data.new_data[self.data.table] = True
+            self.changes_made = False
 
-        self.data.db.table(self.data.table).insert(new_record)
+    def refresh_linked_fields(self, fieldname, value):
+        field = self.e5_cfg.get(fieldname)
+        if field.link_fields:
+            linkfields = self.data.get_link_fields(fieldname, value)
+            if linkfields:
+                for widget in self.layout.walk():
+                    if hasattr(widget, 'id'):
+                        if widget.id in linkfields.keys() and widget.id != fieldname:
+                            widget.text = linkfields[widget.id]
+                            widget_field = self.e5_cfg.get(widget.id)
+                            if widget_field.increment:
+                                try:
+                                    widget.text = str(int(widget.text) + 1)
+                                except ValueError:
+                                    pass
+                            # self.update_db(widget, widget.text)
+
+    def check_required_fields(self):
+        save_errors = []
+        for field_name in self.e5_cfg.fields():
+            field = self.e5_cfg.get(field_name)
+            if field.required:
+                for widget in self.layout.walk():
+                    if hasattr(widget, 'id'):
+                        if widget.id == field_name:
+                            if widget.text == '':
+                                save_errors.append('The field %s requires a value.' % field_name)
+        return save_errors
+
+    def convert_widgets_to_record(self):
+        data_record = {}
+        for field_name in self.e5_cfg.fields():
+            for widget in self.layout.walk():
+                if hasattr(widget, 'id'):
+                    if widget.id == field_name:
+                        data_record[field_name] = widget.text
+        return data_record
 
-    def fill_empty_with_last(self, new_record):
-        for field in self.cfg.fields():
-            field_data = self.get_last_value(field)
-            if field_data is not None:
-                if field not in new_record.keys():
-                    new_record[field] = self.get_last_value(field)
-                elif new_record[field] == '':
-                    new_record[field] = self.get_last_value(field)
-        return(new_record)
-
-    def fill_button_defaults(self, new_record):
-        for button_no in range(1, __BUTTONS__):
-            button = self.cfg.get_block('BUTTON' + str(button_no))
-            if button:
-                if 'TITLE' in button.keys():
-                    if button['TITLE'] == self.station.shot_type:
-                        fieldnames = self.cfg.fields()
-                        for button_default in button:
-                            if button_default in fieldnames:
-                                if button[button_default].upper() == 'ALPHA':
-                                    # TODO Should be calibrated to the length of this field
-                                    new_record[button_default] = self.station.hash()
-                                else:
-                                    new_record[button_default] = button[button_default]
-        return(new_record)
+    def get_unique_key(self, data_record):
+        unique_key = []
+        for field in self.e5_cfg.unique_together:
+            unique_key.append("%s" % data_record[field] if field in data_record else '')
+        return ",".join(unique_key)
+
+    def check_unique_together(self):
+        save_errors = []
+        if self.e5_cfg.unique_together and len(self.data.db.table(self.data.table)) > 1:
+            doc_ids = self.data.doc_ids()
+            unique_key = self.get_unique_key(self.convert_widgets_to_record())
+            for doc_id in doc_ids[0:-1]:
+                if unique_key == self.get_unique_key(self.data.db.table(self.data.table).get(doc_id = doc_id)):
+                    save_errors.append("Based on the unique together field(s) %s, this record's unique key of %s duplicates the record with a doc_id of %s." %
+                                        (",".join(self.e5_cfg.unique_together), unique_key, doc_id))
+                    break
+        return save_errors
 
-    def do_increments(self, new_record):
-        fieldnames = self.cfg.fields()
-        for fieldname in fieldnames:
-            field = self.cfg.get(fieldname)
-            if field.increment:
-                try:
-                    new_record[fieldname] = int(new_record[fieldname]) + 1 if fieldname in new_record.keys() else int(self.get_last_value(fieldname)) + 1
-                except (ValueError, TypeError):
-                    pass
-        return(new_record)
+    def check_numeric_fields(self):
+        save_errors = []
+        for field_name in self.e5_cfg.fields():
+            field = self.e5_cfg.get(field_name)
+            if field.inputtype in ['NUMERIC', 'INSTRUMENT']:
+                for widget in self.layout.walk():
+                    if hasattr(widget, 'id'):
+                        if widget.id == field_name:
+                            if not self.is_numeric(widget.text) and widget.text != '':
+                                save_errors.append('The field %s is marked as numeric but the value entered is not a valid number.' % field_name)
+        return save_errors
+
+    def check_bad_characters(self):
+        save_errors = []
+        for field_name in self.e5_cfg.fields():
+            for widget in self.layout.walk():
+                if hasattr(widget, 'id'):
+                    if widget.id == field_name:
+                        if "\"" in widget.text:
+                            save_errors.append(f'The field {field_name} contains characters that are not recommended in a data file.  These include \" and \\.')
+        return save_errors
+
+    def no_errors_before_save(self):
+        save_errors = self.check_required_fields()
+        save_errors += self.check_unique_together()
+        save_errors += self.check_numeric_fields()
+        save_errors += self.check_bad_characters()
+        if hasattr(self.data.db.table(self.data.table), 'on_save') and save_errors == []:
+            save_errors += self.data.db.table(self.data.table).on_save()
+        if save_errors:
+            self.popup = e5_MessageBox('Save errors',
+                                        '\nCorrect the following errors:\n  ' + '\n  '.join(save_errors),
+                                        response_type = "OK",
+                                        call_back = self.close_popup,
+                                        colors = self.colors)
+            self.popup.open()
+            return False
+        return True
 
-    def fill_carry_fields(self, new_record):
-        fieldnames = self.cfg.fields()
-        for fieldname in fieldnames:
-            if fieldname not in __DEFAULT_FIELDS__ and fieldname not in new_record.keys():
-                field = self.cfg.get(fieldname)
-                if field.carry:
-                    carry_value = self.get_last_value(fieldname)
-                    if carry_value:
-                        new_record[fieldname] = carry_value
-        return(new_record)
-
-    def fill_link_fields(self, new_record):
-        fieldnames = self.cfg.fields()
-        for fieldname in fieldnames:
-            if fieldname not in __DEFAULT_FIELDS__:
-                field = self.cfg.get(fieldname)
-                if field.link_fields:
-                    if fieldname in new_record.keys():
-                        linkfields = self.data.get_link_fields(fieldname, new_record[fieldname])
-                        if linkfields:
-                            for link_fieldname in linkfields.keys():
-                                new_record[link_fieldname] = linkfields[link_fieldname]
-        return(new_record)
-
-    def find_unit_and_fill_fields(self, new_record):
-        fields = self.cfg.fields()
-        unitname = self.data.point_in_unit(self.station.xyz_global)
-        if unitname and "UNIT" in fields:
-            new_record['UNIT'] = unitname
-            unitfields = self.data.get_link_fields('UNIT', unitname)
-            if unitfields:
-                for field in unitfields.keys():
-                    new_record[field] = unitfields[field]
-        return(new_record)
-
-    def fill_default_fields(self, new_record):
-        fields = self.cfg.fields()
-        for field in fields:
-            if field == 'X':
-                new_record['X'] = self.station.xyz_global.x
-            elif field == 'Y':
-                new_record['Y'] = self.station.xyz_global.y
-            elif field == 'Z':
-                new_record['Z'] = self.station.xyz_global.z
-            elif field == 'SLOPED':
-                new_record['SLOPED'] = self.station.sloped
-            elif field == 'HANGLE':
-                new_record['HANGLE'] = self.station.hangle
-            elif field == 'VANGLE':
-                new_record['VANGLE'] = self.station.vangle
-            elif field == 'STATIONX':
-                new_record['STATIONX'] = self.station.location.x
-            elif field == 'STATIONY':
-                new_record['STATIONY'] = self.station.location.y
-            elif field == 'STATIONZ':
-                new_record['STATIONZ'] = self.station.location.z
-            elif field == 'LOCALX':
-                new_record['LOCALX'] = self.station.xyz.x
-            elif field == 'LOCALY':
-                new_record['LOCALY'] = self.station.xyz.y
-            elif field == 'LOCALZ':
-                new_record['LOCALZ'] = self.station.xyz.z
-            elif field == 'PRISM':
-                new_record['PRISM'] = self.station.prism.height if self.station.prism else 0.0
-            elif field == 'DATE':
-                new_record['DATE'] = '%s' % datetime.now().replace(microsecond=0)
-        return(new_record)
-
-    def get_last_value(self, field_name):
-        if self.data.db is not None:
-            if len(self.data.db.table(self.data.table)) > 0:
-                last_record = self.data.db.table(self.data.table).all()[-1]
-                if last_record != []:
-                    if field_name in last_record.keys():
-                        return(last_record[field_name])
-        return(None)
-
-    def exit_program(self):
-        logger = logging.getLogger(__name__)
-        logger.info(__program__ + ' exited.')
-        self.save_window_location()
-        App.get_running_app().stop()
+    def save_record(self, instance):
+        if self.no_errors_before_save():
+            self.update_db()
+            self.update_link_fields()
+
+    def save_record_and_exit(self, instance):
+        if self.no_errors_before_save():
+            self.update_db()
+            self.update_link_fields()
+            self.go_mainscreen()
 
+    def close_popup(self, instance):
+        self.popup.dismiss()
 
-class RecordDatumsScreen(Screen):
+    def update_link_fields(self):
+        if hasattr(self.e5_cfg, 'link_fields'):
+            for field_name in self.e5_cfg.link_fields:
+                cfg_field = self.e5_cfg.get(field_name)
+                for widget in self.layout.walk():
+                    if hasattr(widget, 'id'):
+                        if widget.id == field_name:
+                            q = Query()
+                            db_rec = self.data.db.table(field_name).search(q[field_name].matches('^' + widget.text + '$', re.IGNORECASE))
+                            if db_rec == []:
+                                self.data.db.table(field_name).insert({field_name: widget.text})
+                                db_rec = self.data.db.table(field_name).search(where(field_name) == widget.text)
+                            for link_field_name in cfg_field.link_fields:
+                                for widget in self.layout.walk():
+                                    if hasattr(widget, 'id'):
+                                        if widget.id == link_field_name:
+                                            if (widget.id == 'ID' and self.is_numeric(widget.text)) or widget.id != 'ID':
+                                                update = {link_field_name: widget.text}
+                                                self.data.db.table(field_name).update(update, doc_ids = [db_rec[0].doc_id])
 
-    def __init__(self, data = None, station = None, ini = None, colors = None, **kwargs):
-        super(RecordDatumsScreen, self).__init__(**kwargs)
+    def is_numeric(self, value):
+        try:
+            float(value)
+            return True
+        except ValueError:
+            return False
 
-        self.colors = colors if colors else ColorScheme()
-        self.station = station
-        self.data = data
-        self.ini = ini
+    def cancel_record(self, instance):
+        if hasattr(self.data.db.table(self.data.table), 'on_cancel'):
+            self.data.db.table(self.data.table).on_cancel()
+        self.parent.current = 'MainScreen'
 
-        self.content = BoxLayout(orientation = 'vertical',
-                                    size_hint_y = .9,
-                                    size_hint_x = width_calculator(.9, 400),
-                                    pos_hint={'center_x': .5},
-                                    padding = 20,
-                                    spacing = 20)
-        self.add_widget(self.content)
-
-        self.content.add_widget(e5_label('Provide a name and notes (optional), then record and save.', colors = self.colors))
-
-        self.datum_name = DataGridLabelAndField('Name', colors = self.colors)
-        self.content.add_widget(self.datum_name)
-        self.datum_notes = DataGridLabelAndField('Notes', colors = self.colors)
-        self.content.add_widget(self.datum_notes)
-
-        self.recorder = datum_recorder('Record datum', station = self.station,
-                                        colors = self.colors, setup_type = 'record_new', data = self.data)
-        self.content.add_widget(self.recorder)
-
-        self.results = e5_label('', colors = self.colors)
-        self.content.add_widget(self.results)
-
-        self.content.add_widget(e5_side_by_side_buttons(text = ['Back', 'Save'],
-                                                        id = ['cancel', 'save'],
-                                                        call_back = [self.cancel, self.check_for_duplicate],
-                                                        selected = [False, False],
-                                                        colors = self.colors))
-
-    def check_for_duplicate(self, instance):
-        if self.data.get_datum(self.datum_name.txt.text).name is not None:
-            message = '\nOverwrite existing datum %s?' % self.datum_name.txt.text
-            self.popup = e5_MessageBox('Overwrite?', message,
-                                        response_type = "YESNO",
-                                        call_back = [self.delete_and_save, self.close_popup],
-                                        colors = self.colors)
-            self.popup.open()
-        elif self.datum_name.txt.text == "":
-            self.popup = e5_MessageBox('Error', '\nProvide a datum name before saving.', colors = self.colors)
-            self.popup.open()
-        else:
-            self.save_datum()
+    def show_menu(self, instance, ValueError):
+        if instance.focus and not self.loading:
+            cfg_field = self.e5_cfg.get(instance.id)
+            if cfg_field:
+                self.popup_field_widget = instance
+                if cfg_field.inputtype in ['MENU', 'BOOLEAN']:
+                    text_length = int(cfg_field.length) if self.is_numeric(cfg_field.length) else 0
+                    self.popup = DataGridMenuList(cfg_field.prompt if cfg_field.prompt else instance.id, cfg_field.menu,
+                                                    instance.text, self.menu_selection,
+                                                    colors = self.colors, text_length = text_length)
+                    self.popup.open()
+                    self.popup_scrollmenu = self.get_widget_by_id(self.popup, 'menu_scroll')
+                    self.popup_textbox = self.get_widget_by_id(self.popup, 'new_item')
+                    self.popup_addbutton = self.get_widget_by_id(self.popup, 'add_button')
+        elif not instance.focus and not self.loading:
+            self.refresh_linked_fields(instance.id, instance.text)
 
-    def delete_and_save(self, instance):
+    def menu_selection(self, instance):
         self.popup.dismiss()
-        self.data.delete_datum(self.datum_name.txt.text)
-        self.save_datum()
+        self.popup_field_widget.text = instance.text if not instance.id == 'add_button' else self.popup_textbox.text
+        self.refresh_linked_fields(instance.id, instance.text)
+        if instance.id == 'add_button' and self.popup_field_widget.text.strip() != '':
+            field = self.e5_cfg.get(self.popup_field_widget.id)
+            if self.popup_field_widget.text not in field.menu:
+                field.menu.append(self.popup_field_widget.text)
+                self.e5_cfg.update_value(field.name, 'MENU', ','.join(field.menu))
+                self.e5_cfg.save()
+        self.popup_field_widget = None
+        self.popup_scrollmenu = None
+
+    def find_prism_match(self, value):
+        if self.is_numeric(value):
+            for prism_name in self.data.names('prisms'):
+                prism = self.data.get_prism(prism_name)
+                if prism.height == float(value):
+                    return prism_name
+        return ''
+
+    def show_prisms(self, instance, ValueError):
+        if instance.focus and not self.loading:
+            self.prism_height_old = float(instance.text) if self.is_numeric(instance.text) else 0.0
+            prism_names = self.data.names('prisms')
+            if len(prism_names) > 0:
+                default_prism = self.find_prism_match(instance.text)
+                self.popup_field_widget = instance
+                self.popup = DataGridMenuList(title = "Select or Enter a Prism Height",
+                                                menu_list = prism_names,
+                                                menu_selected = default_prism,
+                                                call_back = self.offer_to_adjust_z,
+                                                colors = self.colors)
+                self.popup.open()
+                self.popup_scrollmenu = self.get_widget_by_id(self.popup, 'menu_scroll')
+                self.popup_textbox = self.get_widget_by_id(self.popup, 'new_item')
+                self.popup_addbutton = self.get_widget_by_id(self.popup, 'add_button')
 
-    def save_datum(self):
-        error_message = ''
-        if self.datum_name.txt.text == '':
-            error_message = '\nProvide a datum name.'
-        if self.recorder.result.xyz_global.x is None or self.recorder.result.xyz_global.y is None or self.recorder.result.xyz_global.z is None:
-            error_message = '\nThe point was not properly recorded.  Try again.'
-        if error_message == '':
-            insert_record = {}
-            insert_record['NAME'] = self.datum_name.txt.text
-            insert_record['NOTES'] = self.datum_notes.txt.text
-            insert_record['X'] = str(round(self.recorder.result.xyz_global.x, 3))
-            insert_record['Y'] = str(round(self.recorder.result.xyz_global.y, 3))
-            insert_record['Z'] = str(round(self.recorder.result.xyz_global.z, 3))
-            self.data.db.table('datums').insert(insert_record)
-            self.datum_name.txt.text = ''
-            self.datum_notes.txt.text = ''
-            self.recorder.result.text = ''
-            self.recorder.result.xyz = None
-            self.recorder.result.xyz_global = None
-            self.data.new_data['datums'] = True
+    def offer_to_adjust_z(self, instance):
+        self.popup.dismiss()
+        if instance.id == 'add_button':
+            if self.is_numeric(self.popup_textbox.text):
+                self.popup_field_widget.text = self.popup_textbox.text
+            else:
+                return
         else:
-            self.popup = e5_MessageBox('Error', error_message, colors = self.colors)
+            prism = self.data.get_prism(instance.text)
+            self.popup_field_widget.text = str(prism.height)
+        prism_height_new = float(self.popup_field_widget.text)
+        z = self.get_widget_by_id(self, 'Z')
+        if z:
+            z_old = float(z.text)
+            self.z_new = z_old + self.prism_height_old - prism_height_new
+            message = f"\nUpdate the Z as well from {round(z_old, 3)} to {round(self.z_new, 3)}?"
+            self.popup = e5_MessageBox('Update', message,
+                                            response_type = "YESNO",
+                                            call_back = [self.update_z, self.close_popup],
+                                            colors = self.colors)
             self.popup.open()
 
-    def close_popup(self, instance):
+    def update_z(self, instance):
+        z = self.get_widget_by_id(self, 'Z')
+        prism = self.get_widget_by_id(self, 'PRISM')
+        if z and prism:
+            z.text = str(round(self.z_new, 3))
         self.popup.dismiss()
 
-    def cancel(self, instance):
+    def get_widget_by_id(self, start = None, id = ''):
+        if not start:
+            start = self
+        for widget in start.walk():
+            if hasattr(widget, 'id'):
+                if widget.id == id:
+                    return widget
+        return None
+
+    def call_back(self, value):
+        if self.changes_made:
+            self.popup = e5_MessageBox('Leave without saving', '\nLeave this record without saving changes?',
+                                        response_type = "YESNO",
+                                        call_back = [self.back_without_save, self.close_popup],
+                                        colors = self.colors)
+            self.popup.open()
+        else:
+            self.go_mainscreen()
+
+    def back_without_save(self, instance):
+        self.close_popup(instance)
+        self.go_mainscreen()
+
+    def go_mainscreen(self, *args):
         self.parent.current = 'MainScreen'
 
 
-class VerifyStationScreen(Screen):
-    id = ObjectProperty(None)
+class e5_DatagridScreen(Screen):
 
-    def __init__(self, data = None, station = None, ini = None, colors = None, **kwargs):
-        super(VerifyStationScreen, self).__init__(**kwargs)
+    datagrid = ObjectProperty(None)
 
+    def __init__(self, main_data = None, main_tablename = '_default', main_cfg = None, colors = None, addnew = False, **kwargs):
+        super(e5_DatagridScreen, self).__init__(**kwargs)
         self.colors = colors if colors else ColorScheme()
-        self.station = station
-        self.data = data
-        self.ini = ini
 
-        self.content = BoxLayout(orientation = 'vertical',
-                                    size_hint_y = .9,
-                                    size_hint_x = .8,
-                                    pos_hint={'center_x': .5},
-                                    padding = 20,
-                                    spacing = 20)
-        self.add_widget(self.content)
-
-        # self.content.add_widget(e5_label('Select a datum to use as verification and record it.', colors = self.colors))
-
-        self.datum1 = datum_selector(text = 'Select\nverification\ndatum',
-                                            data = self.data,
-                                            colors = self.colors,
-                                            default_datum = self.data.get_datum(self.ini.get_value('SETUPS', 'VERIFICATION')))
-        self.content.add_widget(self.datum1)
-
-        self.recorder = datum_recorder('Record\nverification\ndatum', station = self.station,
-                                        colors = self.colors, setup_type = 'verify',
-                                        on_record = self.compute_error, data = self.data)
-        self.content.add_widget(self.recorder)
-
-        self.results = e5_label('', colors = self.colors)
-        self.content.add_widget(self.results)
-
-        self.back_button = e5_button(text = 'Back', size_hint_y = None,
-                                        size_hint_x = 1,
-                                        id = 'cancel',
-                                        colors = self.colors, selected = True)
-        self.content.add_widget(self.back_button)
-        self.back_button.bind(on_press = self.close_screen)
-
-    def compute_error(self):
-        if self.datum1.datum:
-            error = self.station.round_point(self.station.vector_subtract(self.datum1.datum, self.recorder.result.xyz_global))
-            self.results.text = '\n  X error: %s\n  Y error: %s\n  Z error: %s' % (error.x, error.y, error.z)
-        else:
-            self.results.text = "Select the name of the verification datum before recording the datum."
-
-    def close_screen(self, instance):
-        if self.datum1.datum:
-            self.ini.update_value('SETUPS', 'VERIFICATION', self.datum1.datum.name)
-            self.ini.save()
-        self.parent.current = 'MainScreen'
+        if platform_name() == 'Android':
+            self.colors.datagrid_font_size = "11sp"
 
+        self.e5_data = main_data
+        self.e5_cfg = main_cfg
+        self.tablename = main_tablename
 
-class record_button(e5_button):
+        self.datagrid = DataGridWidget(data = main_data.db.table(main_tablename) if self.e5_data.db is not None and main_tablename else None,
+                                        cfg = self.e5_cfg,
+                                        colors = self.colors,
+                                        addnew = addnew)
+        self.add_widget(self.datagrid)
+        if main_data.db is not None:
+            if main_data.db.tables:
+                self.datagrid.data = main_data.db.table(main_tablename)
+                self.datagrid.fields = main_cfg
 
-    popup = ObjectProperty(None)
-    datum_name = None
+    def on_pre_enter(self):
+        if self.e5_data is not None:
+            if self.tablename in self.e5_data.new_data:
+                if self.e5_data.new_data[self.tablename]:
+                    self.datagrid.data = self.e5_data.db.table(self.tablename)
+                    self.datagrid.fields = self.e5_cfg
+                    self.datagrid.reload_data()
+                    self.e5_data.new_data[self.tablename] = False
 
-    def __init__(self, station = None, result_label = None, setup_type = None, on_record = None, datum1 = None, datum2 = None, datum3 = None, data = None, **kwargs):
-        super(record_button, self).__init__(**kwargs)
-        # self.colors = colors if colors is not None else ColorScheme()
-        self.station = station
-        self.bind(on_press = self.record_datum)
-        self.result_label = result_label
-        self.setup_type = setup_type
-        self.on_record = on_record
-        self.datum1 = datum1
-        self.datum2 = datum2
-        self.datum3 = datum3
-        self.data = data
-        self.default_prism = prism()
+    def on_enter(self):
+        Window.bind(on_key_down = self._on_keyboard_down)
+        if self.datagrid:
+            self.datagrid.switch_to(self.datagrid.tab_list[len(self.datagrid.tab_list) - 1])
+
+    def _on_keyboard_down(self, *args):
+        ascii_code = args[1]
+        # print(ascii_code)
+        # text_str = args[3]
+        if ascii_code in [273, 274, 275, 276, 278, 279]:
+            if self.datagrid.popup_scrollmenu:
+                self.datagrid.popup_scrollmenu.move_scroll_menu_item(ascii_code)
+            return False
+        elif ascii_code == 13 and (self.datagrid.popup_scrollmenu or self.datagrid.popup_textbox):
+            if self.datagrid.popup_textbox.focus:
+                self.datagrid.popup_addbutton.trigger_action(0)
+            elif self.datagrid.popup_scrollmenu:
+                self.datagrid.popup_scrollmenu.menu_selected_widget.trigger_action(0)
+        elif ascii_code == 13:
+            return False
+        elif ascii_code == 8:
+            return False
+        elif ascii_code == 27 and (self.datagrid.popup_scrollmenu or self.datagrid.popup_textbox):
+            self.datagrid.popup_scrollmenu = None
+            self.datagrid.popup_textbox = None
+            self.datagrid.popup.dismiss()
+        elif ascii_code in [97, 120, 118, 275, 276, 304, 122, 114, 127]:
+            return False
+        # TODO On key down, see if there is a current record,
+        # get the next record in the db,
+        # and then try to fire the highlight record stuff
+        return True
+
+    def on_leave(self):
+        Window.unbind(on_key_down = self._on_keyboard_down)
+
+
+class e5_MessageBox(Popup):
+    def __init__(self, title, message,
+                    response_type = 'OK',
+                    response_text = None,
+                    call_back = None,
+                    colors = None, **kwargs):
+        super(e5_MessageBox, self).__init__(**kwargs)
+        self.widget_with_focus = None
+        self.colors = colors
+        self.title = title
+        self.response_type = response_type
+        self.response_text = response_text
+        self.call_back = call_back if call_back else self.dismiss
+        self.content = self.build_contents(message)
+        self.size_hint = (.8, .8)
+        self.size = (400, 400)
+        self.auto_dismiss = False
+
+    def build_contents(self, message):
+        contents = GridLayout(cols = 1, spacing = 5)
+        self.txt = e5_scrollview_label(message, popup = True, colors = self.colors)
+        contents.add_widget(self.txt)
+        if self.response_type == 'OK':
+            self.widget_with_focus = e5_button('OK',
+                                                call_back = self.call_back,
+                                                selected = True,
+                                                button_height = .2,
+                                                colors = self.colors)
+            self.widget_with_focus.bind(on_key_up = self.keystroke)
+            contents.add_widget(self.widget_with_focus)
+        elif self.response_type == 'CANCEL':
+            contents.add_widget(e5_button('CANCEL',
+                                                call_back = self.call_back,
+                                                selected = True,
+                                                button_height = .2,
+                                                colors = self.colors))
+        elif self.response_type == 'YESNO':
+            contents.add_widget(e5_side_by_side_buttons(text = ['Yes', 'No'],
+                                                                call_back = self.call_back,
+                                                                selected = [False, False],
+                                                                button_height = .2,
+                                                                colors = self.colors))
+        elif self.response_type == 'YESNOCANCEL':
+            contents.add_widget(e5_side_by_side_buttons(text = ['Yes', 'No', 'Cancel'],
+                                                                call_back = self.call_back,
+                                                                selected = [True, True, True],
+                                                                button_height = .2,
+                                                                colors = self.colors))
+        else:
+            contents.add_widget(e5_side_by_side_buttons(text = self.response_text,
+                                                                call_back = self.call_back,
+                                                                selected = [True, True],
+                                                                button_height = .2,
+                                                                colors = self.colors))
+        return contents
+
+    def refresh_text(self, text):
+        self.content = self.build_contents(text)
+
+    def on_open(self):
+        if self.widget_with_focus:
+            self.widget_with_focus.focus = True
+        Window.bind(on_key_up = self.keystroke)
+
+    def on_dismiss(self):
+        Window.unbind(on_key_up = self.keystroke)
+
+    def keystroke(self, key, scancode, codepoint):
+        if scancode == 13 and self.widget_with_focus:
+            self.widget_with_focus.trigger_action()
 
-    def record_datum(self, instance):
-        self.set_angle()
 
-    def get_angle(self):
-        if self.id == 'datum1':
-            if self.setup_type == 'Over a datum + Record a datum':
-                return(self.station.angle_between_points(self.datum1.datum, self.datum2.datum))
-            elif self.setup_type == 'Record two datums':
-                return(0)
-        else:
-            return(None)
-
-    def set_angle(self):
-        angle = self.get_angle()
-        if angle is not None:
-            if self.station.make in ['Manual XYZ', 'Manual VHD']:
-                self.popup = e5_MessageBox('Set horizonal angle', f'\nAim at {self.datum1.datum.name} and set the horizontal angle to {self.station.decimal_degrees_to_sexastr(angle)}.',
-                                            call_back = self.now_take_shot, colors = self.colors)
-                self.popup.open()
-            elif self.station.make == 'Leica':
-                self.station.set_horizontal_angle_leica(self.station.decimal_degrees_to_dddmmss(angle))
-                self.station.take_shot()
-                self.popup = self.get_prism_height()
-                self.popup.open()
-        else:
-            if self.station.make in ['Microscribe', 'Manual XYZ', 'Manual VHD']:
-                self.wait_for_shot()
-            else:
-                self.station.take_shot()
-                self.popup = self.get_prism_height()
-                self.popup.open()
+class DataUploadScreen(Screen):
 
-    def now_take_shot(self, instance):
-        self.popup.dismiss()
-        self.station.take_shot()
-        self.wait_for_shot()
+    def __init__(self, data = None, cfg = None, colors = None, url = None, username = None, password = None, **kwargs):
+        super(DataUploadScreen, self).__init__(**kwargs)
 
-    def wait_for_shot(self):
-        if self.station.make == 'Microscribe':
-            # self.popup = DataGridTextBox(title = self.text + '.  Waiting on Microscribe...', button_text = ['Cancel', 'Next'], call_back = self.microscribe)
-            self.popup = DataGridTextBox(title = 'EDM',
-                                            label = self.text + '.  Waiting on...',
-                                            text = '<Microscribe>',
-                                            button_text = ['Cancel', 'Next'],
-                                            call_back = self.microscribe,
-                                            colors = self.colors)
-            self.popup.open()
-        elif self.station.make in ['Manual XYZ', 'Manual VHD']:
-            self.popup = edm_manual(call_back = self.have_shot_manual, colors = self.colors)
-            self.popup.open()
+        self.data = data
+        self.cfg = cfg
+        self.colors = colors if colors is not None else ColorScheme()
+        self.height = 1
+        self.layout = GridLayout(cols = 1,
+                                 size_hint_y = .9,
+                                 size_hint_x = width_calculator(.9, 600),
+                                 spacing = 5,
+                                 padding = 5,
+                                 pos_hint={'center_x': .5, 'center_y': .5})
+        self.scroll = ScrollView(size_hint = (1, 1))
+        self.scroll_grid = GridLayout(cols = 1,
+                                        spacing = 5,
+                                        padding = 5,
+                                        size_hint_y = None)
+        instructions = 'Here the data are uploaded to an online database repository like OSA.  '
+        instructions += 'The URL of the repository and your credentials are needed.  '
+        instructions += 'You also need the database and table names for the online repository.  '
+        instructions += 'If you select overwrite, all data for existing matching records in the '
+        instructions += 'online repository will be overwritten with the data here.  Normally you '
+        instructions += 'do not want to do this, but if you are making changes here to already '
+        instructions += 'uploaded data, you may want to select this option. '
+        instructions += 'A local backup of your JSON datafile is made before the upload.  '
+        instructions += 'Select Delete to remove the data here after the upload (this is good practice).'
+        self.scroll_grid.add_widget(e5_label_wrapped(text = instructions, colors = self.colors))
+        self.url = DataGridLabelAndField(col = 'URL', colors = self.colors)
+        if url:
+            self.url.txt.text = url
+        self.scroll_grid.add_widget(self.url)
+        self.username = DataGridLabelAndField(col = 'Username', colors = self.colors)
+        if username:
+            self.username.txt.text = username
+        self.scroll_grid.add_widget(self.username)
+        self.password = DataGridLabelAndField(col = 'Password', colors = self.colors)
+        password = ''
+        if password:
+            self.password.txt.text = password
+        self.password.txt.password = True
+        self.scroll_grid.add_widget(self.password)
+        self.dbname = DataGridLabelAndField(col = 'Database name', colors = self.colors)
+        self.scroll_grid.add_widget(self.dbname)
+        self.tablename = DataGridLabelAndField(col = 'Table name', colors = self.colors)
+        self.scroll_grid.add_widget(self.tablename)
+        self.overwrite = DataGridLabelAndToggle(col = 'Overwrite existing records?')
+        self.scroll_grid.add_widget(self.overwrite)
+        self.deleteafter = DataGridLabelAndToggle(col = 'Delete uploaded/updated?')
+        self.scroll_grid.add_widget(self.deleteafter)
+        self.progress = DataGridLabelAndProgressBar(col = 'Progress\n')
+        self.scroll_grid.add_widget(self.progress)
+        self.scroll_grid.add_widget(e5_side_by_side_buttons(text = ['Back', 'Test', 'Upload'],
+                                                            id = ['back', 'test', 'upload'],
+                                                            call_back = [self.back, self.test, self. upload],
+                                                            selected = [False, False, False],
+                                                            colors = self.colors))
+        self.scroll.add_widget(self.scroll_grid)
+        self.layout.add_widget(self.scroll)
+        self.add_widget(self.layout)
 
-    def have_shot_manual(self, instance):
-        # check that next was pressed and get values
-        p = self.station.text_to_point(f'{self.popup.xcoord.text},{self.popup.ycoord.text},{self.popup.zcoord.text}')
-        if p:
-            self.station.xyz = p
-            self.station.make_global()
-            self.station.vhd_from_xyz()
-        else:
-            self.station.hangle = self.popup.hangle.text if isinstance(self.popup.hangle.text, int) or isinstance(self.popup.hangle.text, float) else ''
-            self.station.vangle = self.popup.vangle.text if isinstance(self.popup.vangle.text, int) or isinstance(self.popup.vangle.text, float) else ''
-            self.station.sloped = self.popup.sloped.text if isinstance(self.popup.sloped.text, int) or isinstance(self.popup.sloped.text, float) else ''
-            self.station.vhd_to_xyz()
-        self.popup.dismiss()
-        self.popup = self.get_prism_height()
-        self.popup.open()
+        self.upload_thread = None
+        self.test_thread = None
 
-    def get_prism_height(self):
-        prism_names = self.data.names('prisms') if self.data else []
-        if len(prism_names) > 0:
-            return(DataGridMenuList(title = "Select or Enter a Prism Height",
-                                            menu_list = prism_names,
-                                            menu_selected = self.default_prism.name if self.default_prism.name else '',
-                                            call_back = self.have_shot))
-        else:
-            return(DataGridTextBox(title = 'Enter a Prism Height',
-                                        text = str(self.default_prism.height) if self.default_prism.height else '',
-                                        call_back = self.have_shot,
-                                        button_text = ['Back', 'Next']))
+    def on_pre_enter(self):
+        database = self.cfg.get_value(APP_NAME, 'ONLINE_DATABASE')
+        if database:
+            self.dbname.txt.text = database
+
+        table = self.cfg.get_value(APP_NAME, 'ONLINE_TABLE')
+        if table:
+            self.tablename.txt.text = table
+
+        username = self.cfg.get_value(APP_NAME, 'ONLINE_USERNAME')
+        if username:
+            self.username.txt.text = username
+
+        url = self.cfg.get_value(APP_NAME, 'ONLINE_URL')
+        if url:
+            self.url.txt.text = url
+
+    def back(self, instance):
+        if self.dbname.txt.text:
+            self.cfg.update_value(APP_NAME, 'ONLINE_DATABASE', self.dbname.txt.text)
 
-    def microscribe(self, instance):
-        result = self.popup.result
-        self.popup.dismiss()
-        if result:
-            error = True
-            try:
-                if len(result.split(',')) == 3:
-                    x, y, z = result.split(',')
-                    x = round(float(x) / 1000, 3)
-                    y = round(float(y) / 1000, 3)
-                    z = round(float(z) / 1000, 3)
-                    self.station.xyz = point(x, y, z)
-                    if self.setup_type == 'verify' or self.setup_type == 'record_new':
-                        self.station.make_global()
-                    else:
-                        self.station.round_xyz()
-                    self.have_shot()
-                    error = False
-            except ValueError:
-                pass
-            if error:
-                self.popup = e5_MessageBox(title = 'Error', message = '\nData not formatted correctly.  EDM expects three floating point numbers separated by commas.',
-                                            colors = self.colors)
-                self.popup.open()
+        if self.tablename.txt.text:
+            self.cfg.update_value(APP_NAME, 'ONLINE_TABLE', self.tablename.txt.text)
 
-    def have_shot(self, instance = None):
-        self.popup.dismiss()
-        # prism_height = instance.text if not instance.id == 'add_button' else self.popup_textbox.text
-        if self.station.make in ['Leica']:
-            self.station.fetch_point()
-            self.station.make_global()
-
-        if instance:
-            prism_name = instance.text
-            if prism_name == 'Add' or prism_name == 'Next':
-                try:
-                    self.station.prism = prism(None, float(self.popup.txt.text), None)
-                except ValueError:
-                    self.station.prism = prism()
-            else:
-                self.station.prism = self.data.get_prism(prism_name)
-        else:
-            self.station.prism = prism(None, 0.0, None)
-        # try:
-        #    if instance:
-        #        self.station.prism = self.data.get_prism(instance.txt)
-        #    else:
-        #        self.station.prism = prism(None, float(self.popup.result), None)
-        # except ValueError:
-        #    self.station.prism = prism(None, 0.0, None)
-        self.default_prism = self.station.prism
-        self.station.prism_adjust()
-        if self.station.xyz.x is not None and self.station.xyz.y is not None and self.station.xyz.z is not None:
-            if self.setup_type == 'verify' or self.setup_type == 'record_new':
-                self.result_label.text = self.station.point_pretty(self.station.xyz_global)
-            else:
-                self.result_label.text = self.station.point_pretty(self.station.xyz)
-            self.result_label.xyz = self.station.xyz
-            self.result_label.xyz_global = self.station.xyz_global
-            if self.on_record is not None:
-                self.on_record()
-        else:
-            self.result_label.text = 'Recording error.'
-            self.result_label.xyz = None
-            self.result_label.xyz_global = None
-
-
-class record_result(e5_label):
-    xyz = point()
-    xyz_global = point()
-
-
-class datum_recorder(GridLayout):
-
-    def __init__(self, text = '', datum_no = 1, station = None,
-                        colors = None, setup_type = None,
-                        on_record = None, datum1 = None, datum2 = None, datum3 = None,
-                        data = None, **kwargs):
-        super(datum_recorder, self).__init__(**kwargs)
-        self.padding = 10
-        self.spacing = 10
-        self.colors = colors if colors is not None else ColorScheme()
-        self.station = station
-        self.cols = 2
-        self.results = []
-        self.buttons = []
-        self.size_hint_y = None
-        self.result = record_result('', colors = self.colors)
-        self.button = record_button(text = text if text else 'Record datum %s' % (datum_no),
-                                    selected = True,
-                                    id = 'datum%s' % (datum_no),
-                                    colors = self.colors,
-                                    station = self.station,
-                                    result_label = self.result,
-                                    setup_type = setup_type,
-                                    on_record = on_record,
-                                    datum1 = datum1,
-                                    datum2 = datum2,
-                                    datum3 = datum3,
-                                    data = data)
-        self.add_widget(self.button)
-        self.add_widget(self.result)
+        if self.username.txt.text:
+            self.cfg.update_value(APP_NAME, 'ONLINE_USERNAME', self.username.txt.text)
 
+        if self.url.txt.text:
+            self.cfg.update_value(APP_NAME, 'ONLINE_URL', self.url.txt.text)
 
-class datum_selector(GridLayout):
+        self.cfg.save()
+        self.parent.current = 'MainScreen'
 
-    datum = None
-    popup = ObjectProperty(None)
-    popup_open = False
+    def connected_to_internet(self):
+        try:
+            # This is hardwired to OSA but it could be anything on the internet
+            urllib.request.urlopen('https://www.oldstoneage.com')
+            return True
+        except (urllib.error.HTTPError, urllib.error.URLError):
+            return False
 
-    def __init__(self, text = '',
-                        data = None, colors = None, default_datum = None,
-                        call_back = None,
-                        id = None,
-                        **kwargs):
-        super(datum_selector, self).__init__(**kwargs)
-        # self.orientation = 'horizontal'
-        self.padding = 10
-        self.spacing = 10
-        self.cols = 2
-        self.colors = colors
-        self.data = data
-        self.datum = default_datum
-        self.call_back = call_back
-        self.size_hint_y = None
-        self.add_widget(e5_button(text = text,
-                                    selected = True,
-                                    call_back = self.show_select_datum,
-                                    colors = self.colors))
-        if self.datum is not None:
-            self.result = e5_label('Datum: %s\nX: %s\nY: %s\nZ: %s' % (self.datum.name,
-                                                                        self.datum.x,
-                                                                        self.datum.y,
-                                                                        self.datum.z), colors = self.colors)
-        else:
-            self.result = e5_label('Datum:\nX:\nY:\nZ:', colors = self.colors)
-        self.add_widget(self.result)
-
-    def show_select_datum(self, instance):
-        self.popup = DataGridMenuList(title = "Datum",
-                                        menu_list = self.data.names('datums'),
-                                        menu_selected = '',
-                                        call_back = self.datum_selected,
-                                        colors = self.colors)
-        self.popup.open()
+    def get_auth_token(self, route):
+        try:
+            if not route['username'] or not route['password']:
+                return (False, 'A username and password must be provided')
+            response = requests.post(route['url'] + 'get-token/', data = {'username': route['username'], 'password': route['password']})
+            if not response.ok:
+                return (False, response.reason)
+            return (True, json.loads(response.text))
+        except urllib.error.HTTPError as e:
+            return (False, e.code)
+        except urllib.error.URLError as e:
+            return (False, e.reason)
+        except Exception as inst:
+            return (False, str(inst))
 
-    def datum_selected(self, instance):
-        self.popup.dismiss()
-        self.datum = self.data.get_datum(instance.text)
-        if self.datum:
-            self.result.text = 'Datum: %s\nX: %s\nY: %s\nZ: %s' % (self.datum.name,
-                                                                    self.datum.x,
-                                                                    self.datum.y,
-                                                                    self.datum.z)
-            if self.call_back:
-                self.call_back(self)
+    def connected_to_rest(self, route):
+        try:
+            if not route['api']:
+                return (False, 'Username and Password authentication not yet coded')
+            response = requests.get(route['url'] + 'connected/', headers = {'Authorization': f"Token {route['api']}"})
+            if response.status_code == 401:
+                return (False, response.reason)
+            return (True, json.loads(response.text))
+        except urllib.error.HTTPError as e:
+            return (False, e.code)
+        except urllib.error.URLError as e:
+            return (False, e.reason)
+        except Exception as inst:
+            return (False, str(inst))
+
+    def get_structure(self, route):
+        response = requests.get(f"{route['url']}structure/{route['database']}/{route['table']}/",
+                                headers = {'Authorization': f"Token {route['api']}"})
+        try:
+            return json.loads(response.text)
+        except ValueError:
+            return ''
+
+    def get_details(self, route, detail_keys):
+        if route['type'] == 'Standard':
+            response = requests.get(f"{route['url']}{route['database']}/{route['table']}{detail_keys}/",
+                                        headers = {'Authorization': f"Token {route['api']}"})
+        else:
+            response = requests.get(f"{route['url']}{route['database']}/{route['table']}/detail{detail_keys}/",
+                                    headers = {'Authorization': f"Token {route['api']}"})
+        return json.loads(response.text)
+
+    def replace_keyfields(self, route, record, unique_together, structure):
+        new_record = record.copy()
+        for field in record.keys():
+            if structure[field]['type'] == 'ForeignKey' and field != 'squid':
+                second_route = route.copy()
+                second_route['table'] = field
+                detail = '/' + record[field]
+                response = self.get_details(second_route, detail)
+                if 'id' in response:
+                    new_record[field] = response['id']
+        return new_record
+
+    def fix_numeric_fields(self, record, structure):
+        new_record = record.copy()
+        for field in record.keys():
+            if structure[field]['type'] in ['IntegerField', 'FloatField'] and record[field] == "":
+                new_record[field] = None
+        return new_record
+
+    def remove_non_e5_cfg_fields(self, record, cfg_fields):
+        delete_list = []
+        cfg_fields_lower = [field.lower() for field in cfg_fields]
+        for key in record.keys():
+            if key.lower() not in cfg_fields_lower:
+                delete_list.append(key)
+        if delete_list:
+            for key in delete_list:
+                record.pop(key, None)
+        return record
+
+    def unique_together_as_url(self, route, record, unique_together, structure):
+        details = []
+        for field in unique_together:
+            if structure[field]['type'] == 'ForeignKey' and field != 'squid':
+                second_route = route.copy()
+                second_route['table'] = field
+                detail = '/' + record[field]
+                response = self.get_details(second_route, detail)
+                if 'id' in response:
+                    details.append(str(response['id']))
+                else:
+                    details.append('None')
+            else:
+                details.append(record[field])
+        # detail = [record[field] if field in record.keys() else '' for field in unique_together]
+        return '/' + '/'.join([detail if detail != '' else 'None' for detail in details])
+
+    def unique_together_as_humanreadable(self, record, unique_together):
+        detail = [str(record[field]) if field in record.keys() else '' for field in unique_together]
+        return '-'.join(detail)
+
+    def record_already_exists(self, route, record, unique_together, structure):
+        detail = self.unique_together_as_url(route, record, unique_together, structure)
+        response = self.get_details(route, detail)
+        if response == {}:
+            return 'Lookup error.'
+        if 'detail' in response.keys():
+            if response['detail'] == 'Not found.':
+                return False
+        return response
+
+    def is_numeric(self, value):
+        if value is None:
+            return True
+        else:
+            try:
+                float(value)
+                return True
+            except (ValueError, TypeError):
+                return False
+
+    def is_integer(self, value):
+        if value is None:
+            return True
         else:
-            self.result.text = 'Search error'
+            try:
+                int(value)
+                return True
+            except ValueError:
+                return False
 
+    def get_route(self):
+        return {'url': self.url.txt.text, 'api': '',
+                    'username': self.username.txt.text, 'password': self.password.txt.text,
+                    'database': self.dbname.txt.text.lower(), 'table': self.tablename.txt.text.lower()}
+
+    def check_connection_issues(self, route):
+        if not self.connected_to_internet():
+            return ('Could not establish an internet connection to www.oldstoneage.com.  Check that you are connected to the internet.', route)
+        if not route['url']:
+            return ('Provide a URL to the base address of the API for this database (e.g. https://www.oldstoneage.com/api/).', route)
+        if not route['api'] and (not route['username'] or not route['password']):
+            return ('Provide either an API key or a username and password.', route)
+        connected, status = self.get_auth_token(route)
+        if not connected:
+            return ('Username or password is invalid.  Or URL is invalid.  The URL should look something like https://www.oldstoneage.com/api/', route)
+        route['api'] = status['token']
+        connected, status = self.connected_to_rest(route)
+        if not connected:
+            return ("Could not connect to the URL provided above with those credentials.  "
+                        "This URL should look something like https://www.oldstoneage.com/api/ but modified for your database.  "
+                        f"The exact error message was '{status}'.", route)
+        if not self.dbname.txt.text or not self.tablename.txt.text:
+            return ('Provide a database and table name.', route)
+        route['type'] = status['type']
+        return ('', route)
+
+    def check_for_cfg_fields_not_online(self, structure):
+        online_fields = [field.lower() for field, value in structure.items() if field not in ['pk', 'unique_together']]
+        missing_fields = []
+        for field in self.cfg.fields():
+            if field.lower() not in online_fields:
+                missing_fields.append(field)
 
-class setups(ScrollView):
+        if missing_fields:
+            return (f"The following fields are in the CFG but not in the online database: {', '.join(missing_fields)}.\n\n"
+                    "Data cannot be transfered until this is fixed.")
+        else:
+            return ''
 
-    id = ObjectProperty(None)
-    popup = ObjectProperty(None)
-    popup_open = False
-    recorder = []
+    def parse_error(self, record, unique_together, error):
+        error_message = self.unique_together_as_humanreadable(record, unique_together) + ' - '
+        for field, value in error.items():
+            if field in record.keys():
+                error_message += f"{record[field]} in {field} - {' '.join(value)}\n"
+            else:
+                error_message += f"{field} - {' '.join(value)}\n"
+        return error_message
+
+    def clean_the_record(self, record, structure):
+        for field, value in record.items():
+            if field in structure.keys():
+                field_online_structure = structure[field]
+                if field_online_structure['type'] == 'BooleanField':
+                    if value.lower() in ['yes', 'true']:
+                        record[field] = True
+                    elif value.lower() in ['no', 'false']:
+                        record[field] = False
+                    elif value.lower() in ['na', 'n/a', '']:
+                        record[field] = None
+        return record
+
+    def update_upload_progress(self, dt):
+        if self.upload_thread is not None:
+            if self.progress.label.text == 'Done\n':
+                if self.error_message:
+                    fails = list(dict.fromkeys(self.fails))
+                    self.popup = e5_MessageBox('Data Upload',
+                                                f"\n{self.additions} records were added. {len(self.overwrites)} were updated.  {len(self.fails)} records "
+                                                    f"could not be added or updated.\n\nThese are the reported errors:\n{self.error_message}\nAnd these are "
+                                                    f"the affected records:\n{', '.join(fails)}",
+                                                call_back = self.close_popup)
+                else:
+                    self.popup = e5_MessageBox('Data Upload',
+                                                f'\n{self.additions} records were added. {len(self.overwrites)} were updated.',
+                                                call_back = self.close_popup)
+                self.popup.open()
+                self.event.cancel()
+                self.progress.bar.value = 0
 
-    def __init__(self, setup_type, data = None, ini = None, station = None, colors = None, **kwargs):
-        super(setups, self).__init__(**kwargs)
+    def update_test_progress(self, dt):
+        if self.test_thread is not None:
+            if self.progress.label.text == 'Done\n':
+                if not self.error_message:
+                    if len(self.overwrites) > 0:
+                        self.overwrites = list(dict.fromkeys(self.overwrites))
+                        self.popup = e5_MessageBox('Data Upload Test',
+                                                    f"\nTest results.  A data upload would add {self.additions} records and modify {len(self.overwrites)} records.\n\n\The modified records would be {', '.join(self.overwrites)}",
+                                                    call_back = self.close_popup)
+                    else:
+                        self.popup = e5_MessageBox('Data Upload Test',
+                                                    f"\nTest results.  A data upload would add {self.additions} records and "
+                                                        f"modify {len(self.overwrites)} records.",
+                                                    call_back = self.close_popup)
+                else:
+                    if len(self.fails) > 0:
+                        self.fails = list(dict.fromkeys(self.fails))
+                        self.popup = e5_MessageBox('Data Upload Test',
+                                                    f"\nA data upload would add {self.additions} records, modify {len(self.overwrites)} records.  However, the upload test produced errors.  Here first is a descripion of the errors:\n{self.error_message}.\n\n\Here is a list of the problem cases:\n{', '.join(self.fails)}",
+                                                    call_back = self.close_popup)
+                    else:
+                        self.popup = e5_MessageBox('Data Upload Test',
+                                                    f'\n{self.error_message}',
+                                                    call_back = self.close_popup)
+                self.popup.open()
+                self.event.cancel()
+                self.progress.bar.value = 0
 
-        self.colors = colors if colors is not None else ColorScheme()
-        self.data = data
-        self.station = station
-        self.ini = ini
-        self.recorder = []
-        self.bar_width = 10
+    def do_upload_of_edm_data(self):
+        self.overwrites = []
+        self.additions = 0
+        self.fails = []
+        route = self.get_route()
+
+        #  TODO this is just to remove a flakeer8 error
+        structure = ''
+
+        self.progress.label.text = 'Checking connection\n'
+        self.error_message, route = self.check_connection_issues(route)
+        if self.error_message:
+            self.progress.label.text = 'Done\n'
+            return
+
+        self.progress.label.text = 'Retrieving structure\n'
+        route['table'] = 'xyz'
+        xyz_structure = self.get_structure(route)
+        if not xyz_structure:
+            self.error_message = 'Something went wrong that should not have.  Could not retreive structure of the xyz table from website.'
+            self.progress.label.text = 'Done\n'
+            return
+
+        route['table'] = 'context'
+        context_structure = self.get_structure(route)
+        if not context_structure:
+            self.error_message = 'Something went wrong that should not have.  Could not retreive structure of the context table from website.'
+            self.progress.label.text = 'Done\n'
+            return
+
+        self.error_message = self.check_for_cfg_fields_not_online(xyz_structure + context_structure)
+        if self.error_message:
+            self.progress.label.text = 'Done\n'
+            return
+
+        unique_together_xyz = ['unit', 'id', 'suffix']
+        # unique_together_context = ['unit', 'id']
+        # unique_keys = {}
+        self.error_message = ''
+        n_records = len(self.data.db.table(self.data.table))
+        record_counter = 0
+        to_delete = []
+        for record in self.data.db.table(self.data.table).all():
+            record_copy = record.copy()
+            doc_id = record_copy.doc_id
+            record_copy = {k.lower(): v for k, v in record_copy.items()}
+            record_copy = self.remove_non_e5_cfg_fields(record_copy, self.cfg.fields())
+            record_copy = self.clean_the_record(record_copy, xyz_structure)
+            record_copy = self.clean_the_record(record_copy, context_structure)
+            record_copy = self.fix_numeric_fields(record_copy, xyz_structure)
+            record_copy = self.fix_numeric_fields(record_copy, context_structure)
+
+            record_counter += 1
+            self.progress.label.text = f'Uploading {self.unique_together_as_humanreadable(record_copy, unique_together_xyz)}\n'
+            self.progress.bar.value = record_counter / n_records
+
+            online_record = self.record_already_exists(route, record_copy, self.cfg.unique_together, structure)
+            if online_record == 'Lookup error':
+                self.error_message += f"\n\nRecord {self.unique_together_as_humanreadable(record_copy, self.cfg.unique_together)} - "\
+                                      "Unable to test whether this record already exists."
+                self.fails.append(self.unique_together_as_humanreadable(record_copy, self.cfg.unique_together))
+            elif online_record and self.overwrite.check.active:
+                if route['type'] == 'Standard':
+                    url = f"{route['url']}{route['database']}/{route['table']}/{online_record['squid']}/"
+                else:
+                    url = f"{route['url']}{route['database']}/{route['table']}/update/{online_record['id']}/"
+                record_copy['id'] = online_record['id']
+                record_copy = self.replace_keyfields(route, record_copy, self.cfg.unique_together, structure)
+                record_copy = self.fix_numeric_fields(record_copy, structure)
+                record_copy = self.remove_non_e5_cfg_fields(record_copy, self.cfg.fields())
+                response = requests.patch(url, data = record_copy, headers = {'Authorization': f"Token {route['api']}"})
+                if response.status_code == 400:
+                    self.error_message += self.parse_error(record_copy, self.cfg.unique_together, json.loads(response.text))
+                    self.fails.append(self.unique_together_as_humanreadable(record_copy, self.cfg.unique_together))
+                elif response.status_code == 500:
+                    self.error_message += f'{self.unique_together_as_humanreadable(record_copy, self.cfg.unique_together)} - {response.reason}'
+                    self.fails.append(self.unique_together_as_humanreadable(record_copy, self.cfg.unique_together))
+                elif response.reason == 'OK':
+                    self.overwrites.append(self.unique_together_as_humanreadable(record_copy, self.cfg.unique_together))
+                    if self.deleteafter.check.active:
+                        to_delete.append(doc_id)
+                else:
+                    self.error_message += f'{self.unique_together_as_humanreadable(record_copy, self.cfg.unique_together)} - \
+                                            Unexpected response - {response.reason}'
+            elif not online_record:
+                record_copy = self.replace_keyfields(route, record_copy, self.cfg.unique_together, structure)
+                record_copy = self.fix_numeric_fields(record_copy, structure)
+                record_copy = self.remove_non_e5_cfg_fields(record_copy, self.cfg.fields())
+                if route['type'] == 'Standard':
+                    url = f"{route['url']}{route['database']}/{route['table']}/"
+                else:
+                    url = f"{route['url']}{route['database']}/{route['table']}/create/"
+                response = requests.post(url, data = record_copy, headers = {'Authorization': f"Token {route['api']}"})
+                if response.status_code == 400:
+                    self.error_message += self.parse_error(record_copy, self.cfg.unique_together, json.loads(response.text))
+                    self.fails.append(self.unique_together_as_humanreadable(record_copy, self.cfg.unique_together))
+                elif response.status_code == 500:
+                    self.error_message += f'{self.unique_together_as_humanreadable(record_copy, self.cfg.unique_together)} - {response.reason}'
+                    self.fails.append(self.unique_together_as_humanreadable(record_copy, self.cfg.unique_together))
+                elif response.reason == 'Created' or response.reason == 'OK':
+                    self.additions += 1
+                    if self.deleteafter.check.active:
+                        to_delete.append(doc_id)
+                else:
+                    self.error_message += f'{self.unique_together_as_humanreadable(record_copy, self.cfg.unique_together)} - '\
+                                            'Unexpected response - {response.reason}\n'
+            else:
+                self.error_message += f'{self.unique_together_as_humanreadable(record_copy, self.cfg.unique_together)} - '\
+                                        'Record already exists and overwrite set to false.\n'
 
-        self.scrollbox = GridLayout(cols = 1,
-                                    size_hint = (1, None),
-                                    spacing = 5)
-        self.scrollbox.bind(minimum_height = self.scrollbox.setter('height'))
+        if self.deleteafter.check.active:
+            self.progress.label.text = 'Deleting uploaded and updated records\n\n'
+            self.data.db.table(self.data.table).remove(doc_ids = to_delete)
+        self.progress.label.text = 'Done\n'
+        return
+
+    def do_upload(self):
+        self.overwrites = []
+        self.additions = 0
+        self.fails = []
+        route = self.get_route()
+        self.progress.bar.value = 0
+
+        self.progress.label.text = 'Checking connection\n'
+        self.error_message, route = self.check_connection_issues(route)
+        if self.error_message:
+            self.progress.label.text = 'Done\n'
+            return
+
+        self.progress.label.text = 'Retrieving structure\n'
+        structure = self.get_structure(route)
+        if not structure:
+            self.error_message = 'Something went wrong that should not have.  Could not retreive structure of the data table from website.  '\
+                                    'Make sure the name of the database and the name of the table are correct.'
+            self.progress.label.text = 'Done\n'
+            return
+
+        self.error_message = self.check_for_cfg_fields_not_online(structure)
+        if self.error_message:
+            self.progress.label.text = 'Done\n'
+            return
+
+        unique_together = structure['unique_together'][0]
+        self.error_message = ''
+        n_records = len(self.data.db.table(self.data.table))
+        record_counter = 0
+        to_delete = []
+        for record in self.data.db.table(self.data.table).all():
+            doc_id = record.doc_id
+            record = {k.lower(): v for k, v in record.items()}
+            record = self.clean_the_record(record, structure)
+
+            record_counter += 1
+            self.progress.label.text = f'Uploading {self.unique_together_as_humanreadable(record, unique_together)}\n'
+            self.progress.bar.value = record_counter / n_records
+
+            online_record = self.record_already_exists(route, record, unique_together, structure)
+            if online_record == 'Lookup error':
+                self.error_message += f"\n\nRecord {self.unique_together_as_humanreadable(record, unique_together)} - "\
+                                        "Unable to test whether this record already exists."
+                self.fails.append(self.unique_together_as_humanreadable(record, unique_together))
+            elif online_record and self.overwrite.check.active:
+                if route['type'] == 'Standard':
+                    url = f"{route['url']}{route['database']}/{route['table']}/{online_record['squid']}/"
+                else:
+                    url = f"{route['url']}{route['database']}/{route['table']}/update/{online_record['id']}/"
+                record['id'] = online_record['id']
+                record = self.replace_keyfields(route, record, unique_together, structure)
+                record = self.fix_numeric_fields(record, structure)
+                record = self.remove_non_e5_cfg_fields(record, self.cfg.fields())
+                response = requests.patch(url, data = record, headers = {'Authorization': f"Token {route['api']}"})
+                if response.status_code == 400:
+                    self.error_message += self.parse_error(record, unique_together, json.loads(response.text))
+                    self.fails.append(self.unique_together_as_humanreadable(record, unique_together))
+                elif response.status_code == 500:
+                    self.error_message += f'{self.unique_together_as_humanreadable(record, unique_together)} - {response.reason}'
+                    self.fails.append(self.unique_together_as_humanreadable(record, unique_together))
+                elif response.reason == 'OK':
+                    self.overwrites.append(self.unique_together_as_humanreadable(record, unique_together))
+                    if self.deleteafter.check.active:
+                        to_delete.append(doc_id)
+                else:
+                    self.error_message += f'{self.unique_together_as_humanreadable(record, unique_together)} - Unexpected response - {response.reason}'
+            elif not online_record:
+                record = self.replace_keyfields(route, record, unique_together, structure)
+                record = self.fix_numeric_fields(record, structure)
+                record = self.remove_non_e5_cfg_fields(record, self.cfg.fields())
+                if route['type'] == 'Standard':
+                    url = f"{route['url']}{route['database']}/{route['table']}/"
+                else:
+                    url = f"{route['url']}{route['database']}/{route['table']}/create/"
+                response = requests.post(url, data = record, headers = {'Authorization': f"Token {route['api']}"})
+                if response.status_code == 400:
+                    self.error_message += self.parse_error(record, unique_together, json.loads(response.text))
+                    self.fails.append(self.unique_together_as_humanreadable(record, unique_together))
+                elif response.status_code == 500:
+                    self.error_message += f'{self.unique_together_as_humanreadable(record, unique_together)} - {response.reason}'
+                    self.fails.append(self.unique_together_as_humanreadable(record, unique_together))
+                elif response.reason == 'Created' or response.reason == 'OK':
+                    self.additions += 1
+                    if self.deleteafter.check.active:
+                        to_delete.append(doc_id)
+                else:
+                    self.error_message += f'{self.unique_together_as_humanreadable(record, unique_together)} - Unexpected response - {response.reason}\n'
+            else:
+                self.error_message += f'{self.unique_together_as_humanreadable(record, unique_together)} - Record already exists and overwrite set to false.\n'
 
-        instructions = Label(color = self.colors.text_color, size_hint_y = None)
+        if self.deleteafter.check.active:
+            self.progress.label.text = 'Deleting uploaded and updated records\n\n'
+            self.data.db.table(self.data.table).remove(doc_ids = to_delete)
+        self.progress.label.text = 'Done\n'
+        return
+
+    def duplicate_check(self, route, record, unique_together, structure):
+        already_in_db = self.record_already_exists(route, record, unique_together, structure)
+        if already_in_db == 'Lookup error.':
+            self.error_message += f"\n\nRecord {self.unique_together_as_humanreadable(record, unique_together)} - "\
+                                    "Unable to test whether this record already exists."
+            self.fails.append(self.unique_together_as_humanreadable(record, unique_together))
+        elif already_in_db and self.overwrite.check.active:
+            self.overwrites.append(self.unique_together_as_humanreadable(record, unique_together))
+        elif already_in_db and not self.overwrite.check.active:
+            self.error_message += f"\n\nRecord {self.unique_together_as_humanreadable(record, unique_together)} - "\
+                                    "Already exists but overwrite is set to False."
+            self.fails.append(self.unique_together_as_humanreadable(record, unique_together))
+        else:
+            self.additions += 1
+
+    def field_check(self, record, structure, unique_together):
+        for field, value in record.items():
+            if field not in structure:
+                self.error_message += f'\n\nRecord {self.unique_together_as_humanreadable(record, unique_together)} - '\
+                                        'the field {field} is in datafile but not in the online database.'
+                self.fails.append(self.unique_together_as_humanreadable(record, unique_together))
+                continue
+            field_online_structure = structure[field]
+            if field_online_structure['type'] == 'CharField':
+                if len(record[field]) > field_online_structure['length']:
+                    self.error_message += f"\n\nRecord {self.unique_together_as_humanreadable(record, unique_together)} - "\
+                                            f"{record[field]} in {field} exceeds the valid field length. Maximum length is {field_online_structure['length']}.  "\
+                                            f"Actual length is {len(record[field])}."
+                    self.fails.append(self.unique_together_as_humanreadable(record, unique_together))
+            elif field_online_structure['type'] == 'FloatField':
+                if not self.is_numeric(record[field]):
+                    self.error_message += f'\n\nRecord {self.unique_together_as_humanreadable(record, unique_together)} - '\
+                                            f'the value {record[field]} for {field} must be numeric.'
+                    self.fails.append(self.unique_together_as_humanreadable(record, unique_together))
+            elif field_online_structure['type'] == 'IntegerField':
+                if not self.is_integer(record[field]):
+                    self.error_message += f'\n\nRecord {self.unique_together_as_humanreadable(record, unique_together)} - '\
+                                            f'the value {record[field]} for {field} must be an integer.'
+                    self.fails.append(self.unique_together_as_humanreadable(record, unique_together))
+            elif field_online_structure['type'] == 'DateTimeField':
+                pass
+            elif field_online_structure['type'] == 'BooleanField':
+                if record[field] not in [True, False, None]:
+                    self.error_message += f'\n\nRecord {self.unique_together_as_humanreadable(record, unique_together)} - '\
+                                            f'the value {record[field]} for {field} must be True or False.'
+                    self.fails.append(self.unique_together_as_humanreadable(record, unique_together))
+            elif field_online_structure['type'] == 'ForeignKey':
+                pass    # TODO look up in related table
+
+    def do_test_of_edm_data(self):
+
+        self.overwrites = []
+        self.additions = 0
+        self.fails = []
+        route = self.get_route()
+
+        self.progress.label.text = 'Checking connection\n'
+        self.error_message, route = self.check_connection_issues(route)
+        if self.error_message:
+            self.progress.label.text = 'Done\n'
+            return
+
+        self.progress.label.text = 'Retrieving structure\n'
+        route['table'] = 'xyz'
+        xyz_structure = self.get_structure(route)
+        if not xyz_structure:
+            self.error_message = 'Something went wrong that should not have.  Could not retreive structure of the xyz table from website.'
+            self.progress.label.text = 'Done\n'
+            return
+
+        route['table'] = 'context'
+        context_structure = self.get_structure(route)
+        if not context_structure:
+            self.error_message = 'Something went wrong that should not have.  Could not retreive structure of the context table from website.'
+            self.progress.label.text = 'Done\n'
+            return
+
+        self.error_message = self.check_for_cfg_fields_not_online(xyz_structure + context_structure)
+        if self.error_message:
+            self.progress.label.text = 'Done\n'
+            return
+
+        unique_together_xyz = ['unit', 'id', 'suffix']
+        unique_together_context = ['unit', 'id']
+        unique_keys = {}
+        self.error_message = ''
+        n_records = len(self.data.db.table(self.data.table))
+        record_counter = 0
+        for record in self.data.db.table(self.data.table).all():
+            record_copy = record.copy()
+            record_copy = {k.lower(): v for k, v in record_copy.items()}
+            record_copy = self.remove_non_e5_cfg_fields(record_copy, self.cfg.fields())
+            record_copy = self.clean_the_record(record_copy, xyz_structure)
+            record_copy = self.clean_the_record(record_copy, context_structure)
+            record_copy = self.fix_numeric_fields(record_copy, xyz_structure)
+            record_copy = self.fix_numeric_fields(record_copy, context_structure)
+
+            record_counter += 1
+            self.progress.label.text = f'Testing upload of {self.unique_together_as_humanreadable(record_copy, unique_together_xyz)}\n'
+            self.progress.bar.value = record_counter / n_records
+
+            route['table'] = 'context'
+            self.duplicate_check(route, record_copy, unique_together_context, context_structure)
+            route['table'] = 'xyz'
+            self.duplicate_check(route, record_copy, unique_together_xyz, xyz_structure)
+
+            if self.unique_together_as_humanreadable(record_copy, unique_together_xyz) not in unique_keys.keys():
+                unique_keys[self.unique_together_as_humanreadable(record_copy, unique_together_xyz)] = 1
+            else:
+                unique_keys[self.unique_together_as_humanreadable(record_copy, unique_together_xyz)] += 1
+
+            self.field_check(record_copy, xyz_structure + context_structure, unique_together_xyz)
+
+        if len(unique_keys) != record_counter:
+            self.error_message += "\n\nWARNING: The following records are duplicated in the data file.  "\
+                                  "When they are transfered they will overwrite each other: "\
+                                  f"{', '.join([item for item, value in unique_keys.items() if value > 1])}"
+
+        self.progress.label.text = 'Done\n'
+        return
+
+    def do_test(self):
+        self.overwrites = []
+        self.additions = 0
+        self.fails = []
+        route = self.get_route()
+
+        self.progress.label.text = 'Checking connection\n'
+        self.error_message, route = self.check_connection_issues(route)
+        if self.error_message:
+            self.progress.label.text = 'Done\n'
+            return
+
+        self.progress.label.text = 'Retrieving structure\n'
+        structure = self.get_structure(route)
+        if not structure:
+            self.error_message = 'Something went wrong that should not have.  Could not retreive structure of the data table from website.'
+            self.progress.label.text = 'Done\n'
+            return
+
+        self.error_message = self.check_for_cfg_fields_not_online(structure)
+        if self.error_message:
+            self.progress.label.text = 'Done\n'
+            return
+
+        unique_together = structure['unique_together'][0]
+        unique_keys = {}
+        self.error_message = ''
+        n_records = len(self.data.db.table(self.data.table))
+        record_counter = 0
+        for record in self.data.db.table(self.data.table).all():
+            record = {k.lower(): v for k, v in record.items()}
+            record = self.clean_the_record(record, structure)
+
+            record_counter += 1
+            self.progress.label.text = f'Uploading {self.unique_together_as_humanreadable(record, unique_together)}\n'
+            self.progress.bar.value = record_counter / n_records
+
+            already_in_db = self.record_already_exists(route, record, unique_together, structure)
+            if already_in_db == 'Lookup error.':
+                self.error_message += f"\n\nRecord {self.unique_together_as_humanreadable(record, unique_together)} - "\
+                                      "Unable to test whether this record already exists."
+                self.fails.append(self.unique_together_as_humanreadable(record, unique_together))
+            elif already_in_db and self.overwrite.check.active:
+                self.overwrites.append(self.unique_together_as_humanreadable(record, unique_together))
+            elif already_in_db and not self.overwrite.check.active:
+                self.error_message += f"\n\nRecord {self.unique_together_as_humanreadable(record, unique_together)} - "\
+                                      "Already exists but overwrite is set to False."
+                self.fails.append(self.unique_together_as_humanreadable(record, unique_together))
+            else:
+                self.additions += 1
+
+            if self.unique_together_as_humanreadable(record, unique_together) not in unique_keys.keys():
+                unique_keys[self.unique_together_as_humanreadable(record, unique_together)] = 1
+            else:
+                unique_keys[self.unique_together_as_humanreadable(record, unique_together)] += 1
+
+            record = self.remove_non_e5_cfg_fields(record, self.cfg.fields())
+            record = self.fix_numeric_fields(record, structure)
+
+            for field, value in record.items():
+                if field not in structure:
+                    self.error_message += f'\n\nRecord {self.unique_together_as_humanreadable(record, unique_together)} - '\
+                                          f'the field {field} is in datafile but not in the online database.'
+                    self.fails.append(self.unique_together_as_humanreadable(record, unique_together))
+                    continue
+                field_online_structure = structure[field]
+                if field_online_structure['type'] == 'CharField':
+                    if len(record[field]) > field_online_structure['length']:
+                        self.error_message += f"\n\nRecord {self.unique_together_as_humanreadable(record, unique_together)} - "\
+                                              f"{record[field]} in {field} exceeds the valid field length. "\
+                                              f"Maximum length is {field_online_structure['length']}.  Actual length is {len(record[field])}."
+                        self.fails.append(self.unique_together_as_humanreadable(record, unique_together))
+                elif field_online_structure['type'] == 'FloatField':
+                    if not self.is_numeric(record[field]):
+                        self.error_message += f'\n\nRecord {self.unique_together_as_humanreadable(record, unique_together)} - '\
+                                              f'the value {record[field]} for {field} must be numeric.'
+                        self.fails.append(self.unique_together_as_humanreadable(record, unique_together))
+                elif field_online_structure['type'] == 'IntegerField':
+                    if not self.is_integer(record[field]):
+                        self.error_message += f'\n\nRecord {self.unique_together_as_humanreadable(record, unique_together)} - '\
+                                              f'the value {record[field]} for {field} must be an integer.'
+                        self.fails.append(self.unique_together_as_humanreadable(record, unique_together))
+                elif field_online_structure['type'] == 'DateTimeField':
+                    pass
+                elif field_online_structure['type'] == 'BooleanField':
+                    if record[field] not in [True, False, None]:
+                        self.error_message += f'\n\nRecord {self.unique_together_as_humanreadable(record, unique_together)} - '\
+                                              f'the value {record[field]} for {field} must be True or False.'
+                        self.fails.append(self.unique_together_as_humanreadable(record, unique_together))
+                elif field_online_structure['type'] == 'ForeignKey':
+                    pass    # TODO look up in related table
+
+        if len(unique_keys) != record_counter:
+            self.error_message += f"\n\nWARNING: The following records are duplicated in the data file.  "\
+                                  "When they are transfered they will overwrite each other: "\
+                                  f"{', '.join([item for item, value in unique_keys.items() if value > 1])}"
+
+        self.progress.label.text = 'Done\n'
+        return
+
+    def test(self, instance):
+        self.event = Clock.schedule_interval(self.update_test_progress, 0.5)
+        self.test_thread = Thread(target = self.do_test)
+        self.test_thread.start()
+
+    def upload(self, instance):
+        # backup the data file
+        self.event = Clock.schedule_interval(self.update_upload_progress, 0.5)
+        self.upload_thread = Thread(target = self.do_upload)
+        self.upload_thread.start()
 
-        if setup_type == "Horizontal Angle Only":
-            instructions.text = '\nEnter the horizontal angle to uploaded to the station.'
-            self.scrollbox.add_widget(instructions)
-
-            content1 = GridLayout(cols = 2, padding = 10, size_hint_y = None)
-            content1.add_widget(e5_label('Angle (use ddd.mmss)'))
-            self.hangle = TextInput(text = '', multiline = False,
-                                    size_hint_max_y = 30)
-            content1.add_widget(self.hangle)
-            self.scrollbox.add_widget(content1)
-
-            content2 = GridLayout(cols = 1, padding = 10, size_hint_y = None)
-            content2.add_widget(e5_button(text = 'Upload angle', selected = True, call_back = self.set_hangle, colors = self.colors))
-            self.scrollbox.add_widget(content2)
-
-        elif setup_type == "Over a datum":
-            instructions.text = '\nUse this option when the station is setup over a known point and you can measure the station height or to set the station location directly (with no station height).  Note this option assumes the horizontal angle is already correct or will be otherwise set.'
-            self.scrollbox.add_widget(instructions)
-
-            self.over_datum = datum_selector(text = 'Select a datum',
-                                                data = self.data,
-                                                colors = self.colors,
-                                                default_datum = self.data.get_datum(self.ini.get_value('SETUPS', 'OVERDATUM')))
-            self.scrollbox.add_widget(self.over_datum)
-
-            content2 = GridLayout(cols = 2, padding = 10, size_hint_y = None)
-            content2.add_widget(e5_label('Station height (optional)'))
-            self.station_height = TextInput(text = '', multiline = False,
-                                            size_hint_max_y = 30)
-            content2.add_widget(self.station_height)
-            self.scrollbox.add_widget(content2)
-
-        elif setup_type == "Over a datum + Record a datum":
-            instructions.text = "\nSelect the datum under the station and a datum to recorded.  EDM will automatically set the correct horizontal angle and compute the station's XYZ coordinates."
-            self.scrollbox.add_widget(instructions)
-
-            self.datum1 = datum_selector(text = 'Select datum\nunder the\nstation',
-                                                data = self.data,
-                                                colors = self.colors,
-                                                default_datum = self.data.get_datum(self.ini.get_value('SETUPS', 'OVERDATUM')))
-            self.scrollbox.add_widget(self.datum1)
-
-            self.datum2 = datum_selector(text = 'Select datum\nto record',
-                                                data = self.data,
-                                                colors = self.colors,
-                                                default_datum = self.data.get_datum(self.ini.get_value('SETUPS', 'RECORDDATUM')),
-                                                call_back = self.datum1_selected)
-            self.scrollbox.add_widget(self.datum2)
-
-            datum_name = self.data.get_datum(self.ini.get_value('SETUPS', 'RECORDDATUM'))
-            datum_name = f'Record\n{datum_name.name}' if datum_name else 'Record datum 1'
-            self.recorder.append(datum_recorder(datum_name, station = self.station, colors = self.colors,
-                                                setup_type = setup_type, datum1 = self.datum1, datum2 = self.datum2,
-                                                data = self.data))
-            self.scrollbox.add_widget(self.recorder[0])
-
-        elif setup_type == "Record two datums":
-            instructions.text = "\nSelect two datums to record. EDM will use triangulation to compute the station's XYZ coordinates.  Always record datum one first and then datum two.  When you record datum one, the horizontal angle will be set to 0.0.  When you accept the setup, the horizontal angle will be reset correctly on datum 2."
-            self.scrollbox.add_widget(instructions)
-
-            self.datum1 = datum_selector(text = 'Select\ndatum\none',
-                                                data = self.data,
-                                                colors = self.colors,
-                                                default_datum = self.data.get_datum(self.ini.get_value('SETUPS', '2DATUMS_DATUM_1')),
-                                                call_back = self.datum1_selected)
-            self.scrollbox.add_widget(self.datum1)
-
-            self.datum2 = datum_selector(text = 'Select\ndatum\ntwo',
-                                                data = self.data,
-                                                colors = self.colors,
-                                                default_datum = self.data.get_datum(self.ini.get_value('SETUPS', '2DATUMS_DATUM_2')),
-                                                call_back = self.datum2_selected)
-            self.scrollbox.add_widget(self.datum2)
-
-            for n in range(2):
-                datum_name = self.data.get_datum(self.ini.get_value('SETUPS', '2DATUMS_DATUM_%s' % (n + 1)))
-                datum_name = f'Record\n{datum_name.name}' if datum_name else f'Record datum {n + 1}'
-                self.recorder.append(datum_recorder(datum_name, datum_no = n + 1, station = station, colors = colors,
-                                                    setup_type = setup_type, datum1 = self.datum1, datum2 = self.datum2, data = self.data))
-                self.scrollbox.add_widget(self.recorder[n])
-
-        elif setup_type == "Three datum shift":
-            instructions.text = "\nThis option is designed to let one grid be rotated into another and is best for when a block of sediment is being excavated in a lab.  It requires three datums points."
-            self.scrollbox.add_widget(instructions)
-
-            self.datum1 = datum_selector(text = 'Select datum 1',
-                                                data = self.data,
-                                                colors = self.colors,
-                                                default_datum = self.data.get_datum(self.ini.get_value('SETUPS', '3DATUM_SHIFT_GLOBAL_1')),
-                                                call_back = self.datum1_selected)
-            self.scrollbox.add_widget(self.datum1)
-
-            self.datum2 = datum_selector(text = 'Select datum 2',
-                                                data = self.data,
-                                                colors = self.colors,
-                                                default_datum = self.data.get_datum(self.ini.get_value('SETUPS', '3DATUM_SHIFT_GLOBAL_2')),
-                                                call_back = self.datum2_selected)
-            self.scrollbox.add_widget(self.datum2)
-
-            self.datum3 = datum_selector(text = 'Select datum 3',
-                                                data = self.data,
-                                                colors = self.colors,
-                                                default_datum = self.data.get_datum(self.ini.get_value('SETUPS', '3DATUM_SHIFT_GLOBAL_3')),
-                                                call_back = self.datum3_selected)
-            self.scrollbox.add_widget(self.datum3)
-
-            for n in range(3):
-                datum_name = self.data.get_datum(self.ini.get_value('SETUPS', '3DATUM_SHIFT_GLOBAL_%s' % (n + 1)))
-                datum_name = f'Record {datum_name.name}' if datum_name else f'Record datum {n + 1}'
-                self.recorder.append(datum_recorder(datum_name, datum_no = n + 1, station = station,
-                                                                colors = self.colors, setup_type = setup_type))
-                self.scrollbox.add_widget(self.recorder[n])
-
-        instructions.bind(texture_size = lambda instance, value: setattr(instance, 'height', value[1]))
-        instructions.bind(width = lambda instance, value: setattr(instance, 'text_size', (value * .95, None)))
-
-        self.size_hint = (1, .9)
-        # self.size = (Window.width, Window.height / 2)
-        self.id = 'setup_scroll'
-        self.add_widget(self.scrollbox)
+    def close_popup(self, instance):
+        self.popup.dismiss()
 
-        def draw_background(widget, prop):
-            with widget.canvas.before:
-                Color(0.8, 0.8, 0.8, 1)
-                Rectangle(size=self.size, pos=self.pos)
 
-        # self.bind(size = draw_background)
-        # self.bind(pos = draw_background)
+# region Data Grid
+# Code from https://github.com/MichaelStott/DataframeGUIKivy/blob/master/dfguik.py
 
-    def datum1_selected(self, instance):
-        self.recorder[0].children[1].text = 'Record ' + instance.datum.name
-        self.recorder[0].children[1].datum_name = instance.datum.name
+class DataGridMenuList(Popup):
 
-    def datum2_selected(self, instance):
-        self.recorder[1].children[1].text = 'Record ' + instance.datum.name
-        self.recorder[1].children[1].datum_name = instance.datum.name
+    def __init__(self, title, menu_list, menu_selected = '', call_back = None, colors = None, text_length = 0, **kwargs):
+        super(DataGridMenuList, self).__init__(**kwargs)
 
-    def datum3_selected(self, instance):
-        self.recorder[2].children[1].text = 'Record ' + instance.datum.name
-        self.recorder[2].children[1].datum_name = instance.datum.name
+        pop_content = GridLayout(cols = 1, size_hint_y = 1, spacing = 5, padding = 5)
+
+        new_item = GridLayout(cols = 2, spacing = 5, size_hint_y = None)
+        new_item_left = GridLayout(cols = 1, spacing = 5, size_hint_y = None)
+        if menu_list:
+            new_item_instructions_text = 'Enter a new menu item and press add or select from the menu below.  New menu items are saved in the CFG.'
+        else:
+            new_item_instructions_text = 'Enter a new menu item and press add.  New menu items are saved in the CFG.'
+        new_item_instructions = e5_label(new_item_instructions_text, popup = True, text_size = (self.width * 2, None))
+        new_item_left.add_widget(new_item_instructions)
+        self.txt = e5_textinput(id = 'new_item', size_hint_y = None, text_length = text_length)
+        self.txt.bind(minimum_height = self.txt.setter('height'))
+        if colors:
+            if colors.text_font_size:
+                self.txt.font_size = colors.text_font_size
+        new_item_left.add_widget(self.txt)
+        new_item.add_widget(new_item_left)
+        self.add_button = e5_button('Add',
+                                    id = 'add_button',
+                                    selected = True,
+                                    call_back = call_back,
+                                    button_height = .15,
+                                    colors = colors)
+        new_item.add_widget(self.add_button)
+        # new_item.bind(minimum_height = new_item.setter('height'))
+        pop_content.add_widget(new_item)
+
+        ncols = max(int(Window.width / 200), 1)
+
+        self.menu = None
+        if menu_list:
+            self.menu = e5_scrollview_menu(menu_list, menu_selected,
+                                                    widget_id = 'menu',
+                                                    call_back = [call_back],
+                                                    ncols = ncols,
+                                                    colors = colors)
+            pop_content.add_widget(self.menu)
+            self.menu.make_scroll_menu_item_visible()
+
+        pop_content.add_widget(e5_button('Back', selected = True,
+                                                 call_back = self.dismiss,
+                                                 colors = colors))
+
+        self.content = pop_content
+
+        self.title = title
+        self.size_hint = (.9, .9 if menu_list else .33)
+        self.auto_dismiss = True
+        self.call_back = call_back
 
-    def set_hangle(self, instance):
-        if self.hangle:
-            self.station.set_horizontal_angle(self.hangle.text)
-            logger = logging.getLogger(__name__)
-            logger.info(f'Horizontal angle set to {self.hangle.text}')
+    def on_open(self):
+        self.txt.textbox.focus = True
+        self.txt.textbox.select_all()
+        Window.bind(on_key_down = self._on_keyboard_down)
+
+    def _on_keyboard_down(self, *args):
+        ascii_code = args[1]
+        if ascii_code == 13 and self.txt.textbox.focus and self.txt.textbox.text != "":
+            self.call_back(self.add_button)
+        elif ascii_code == 13:
+            if self.menu:
+                if self.menu.scroll_menu_get_selected():
+                    self.call_back(self.menu.scroll_menu_get_selected())
+        elif self.menu:
+            self.menu.move_scroll_menu_item(ascii_code)
 
+    def on_dismiss(self):
+        Window.unbind(on_key_down = self._on_keyboard_down)
 
-class InitializeStationScreen(Screen):
 
-    def __init__(self, data = None, station = None, ini = None, colors = None, **kwargs):
-        super(InitializeStationScreen, self).__init__(**kwargs)
+class DataGridTextInput(e5_textinput):
 
-        self.colors = colors if colors else ColorScheme()
-        self.station = station
-        self.data = data
-        self.ini = ini
+    id = ObjectProperty(None)
 
-        lastsetup_type = self.ini.get_value('SETUPS', 'LASTSETUP_TYPE')
-        self.setup = lastsetup_type if lastsetup_type else 'Horizontal Angle Only'
+    def __init__(self, call_back = None, **kwargs):
+        super(DataGridTextInput, self).__init__(**kwargs)
+        self.call_back = call_back
 
-        self.content = BoxLayout(orientation = 'vertical',
-                                    size_hint_y = .9,
-                                    # size_hint_x = width_calculator(.9, 200),
-                                    pos_hint = {'center_x': .5, 'center_y': .5},
-                                    padding = 5,
-                                    spacing = 5)
-        self.add_widget(self.content)
+    def keyboard_on_key_up(self, window, keycode):
+        # print(keycode)
+        return super(DataGridTextInput, self).keyboard_on_key_up(window, keycode)
 
-        setup_type_box = GridLayout(cols = 2,
-                                    # size_hint = (width_calculator(.9, 400), None),
-                                    size_hint_y = None,
-                                    pos_hint = {'center_x': .5, 'center_y': .5})
 
-        spinner_dropdown_button = SpinnerOptions
-        spinner_dropdown_button.font_size = colors.button_font_size.replace("sp", '') if colors.button_font_size else None
-        spinner_dropdown_button.background_color = (0, 0, 0, 1)
+class DataGridTextBox(Popup):
 
-        self.setup_type = Spinner(text = self.setup,
-                                    values=["Horizontal Angle Only",
-                                            "Over a datum",
-                                            "Over a datum + Record a datum",
-                                            "Record two datums",
-                                            "Three datum shift"],
-                                    # pos_hint = {'center_x': .5, 'center_y': .5}
-                                    size_hint = (.5, None),
-                                    option_cls = spinner_dropdown_button)
-        if colors.button_font_size:
-            self.setup_type.font_size = colors.button_font_size
-        setup_type_box.add_widget(self.setup_type)
-        self.setup_type.bind(text = self.rebuild)
-        self.content.add_widget(setup_type_box)
-
-        self.scroll_content = BoxLayout(orientation = 'vertical',
-                                        size_hint = (1, .9),
-                                        spacing = 5, padding = 5)
+    result = ObjectProperty(None)
+    save_button = ObjectProperty(None)
 
-        self.content.add_widget(self.scroll_content)
+    def __init__(self, title, label = None, text = '', multiline = False, call_back = None,
+                        button_text = ['Back', 'Save'], colors = None, text_length = 0, **kwargs):
+        super(DataGridTextBox, self).__init__(**kwargs)
+        self.colors = colors if colors else ColorScheme()
+        content = GridLayout(cols = 1, spacing = 5, padding = 10)
+        if label:
+            # e5_label(text = col, id = '__label', colors = colors)
+            # content.add_widget(Label(text = label, text_size = (None, 30)))
+            content.add_widget(e5_label(text = label, colors = self.colors, popup = True))
+        self.txt = DataGridTextInput(text = text, size_hint_y = None,
+                                        text_length = text_length,
+                                        # height = 30 if not multiline else 90,
+                                        multiline = multiline, id = 'new_item')
+        if self.colors:
+            if self.colors.text_font_size:
+                self.txt.font_size = self.colors.text_font_size
+            if not multiline:
+                if self.colors.text_font_size:
+                    self.txt.height = int(self.colors.text_font_size.replace('sp', '')) * 1.8
+        self.result = text
+        self.txt.textbox.bind(text = self.update)
+        self.txt.textbox.bind(on_text_validate = self.accept_value)
+        content.add_widget(self.txt)
+        buttons = e5_side_by_side_buttons(button_text,
+                                            button_height = None,
+                                            id = [title, 'add_button'],
+                                            selected = [True, True],
+                                            call_back = [self.dismiss, call_back],
+                                            colors = self.colors)
+        self.save_button = buttons.children[0]
+        content.add_widget(buttons)
+        self.title = title
+        self.content = content
+        if not multiline:
+            self.size_hint = (width_calculator(.8, 800), .35 if label is None else .5)
+        else:
+            self.size_hint = (width_calculator(.8, 800), .45 if label is None else .6)
+        self.auto_dismiss = True
+
+        self.event = Clock.schedule_once(self.set_focus, .35)
+
+    def set_focus(self, instance):
+        self.txt.textbox.focus = True
+        self.txt.textbox.select_all()
+
+    def on_open(self):
+        self.txt.textbox.focus = True
+        self.txt.textbox.select_all()
+
+    def update(self, instance, value):
+        self.result = value
+
+    def accept_value(self, instance):
+        self.save_button.trigger_action(0)
+
+
+class DataGridHeaderCell(Button):
+    def __init__(self, text, colors, **kwargs):
+        super(DataGridHeaderCell, self).__init__(**kwargs)
+        self.background_color = colors.button_background
+        self.background_color = DARK_GREY
+        self.background_normal = ''
+        self.color = make_rgb(WHITE)
+        self.text = text
+        if colors.datagrid_font_size:
+            self.font_size = colors.datagrid_font_size
+
+
+class DataGridTableHeader(ScrollView):
+    """Fixed table header that scrolls x with the data table"""
+    header = ObjectProperty(None)
+
+    def __init__(self, titles = None, colors = None, *args, **kwargs):
+        super(DataGridTableHeader, self).__init__(*args, **kwargs)
+
+        for title in titles:
+            self.header.add_widget(DataGridHeaderCell(title, colors))
+
+
+class DataGridScrollCell(Button):
+    text = StringProperty(None)
+    is_even = BooleanProperty(None)
+    # datagrid_even = ListProperty(None)
+    # datagrid_odd = ListProperty(None)
+    datagrid_even = [189.0 / 255, 189.0 / 255, 189.0 / 255, 1]
+    datagrid_odd = [224.0 / 255, 224.0 / 255, 224.0 / 255, 1]
 
-        self.setup_widgets = setups(self.setup_type.text,
-                                    data = self.data,
-                                    ini = self.ini,
-                                    station = self.station,
-                                    colors = self.colors)
-        self.scroll_content.add_widget(self.setup_widgets)
+    def __init__(self, **kwargs):
+        super(DataGridScrollCell, self).__init__(**kwargs)
+        self.background_normal = ''
 
-        self.content.add_widget(e5_side_by_side_buttons(text = ['Back', 'Accept Setup'],
-                                                        id = ['back', 'accept'],
-                                                        call_back = [self.go_back, self.accept_setup],
-                                                        selected = [True, True],
-                                                        colors = self.colors))
-
-    def rebuild(self, instance, value):
-        self.setup = value
-        self.scroll_content.clear_widgets()
-        self.setup_widgets = setups(self.setup_type.text,
-                                                data = self.data,
-                                                ini = self.ini,
-                                                station = self.station,
-                                                colors = self.colors)
-        self.scroll_content.add_widget(self.setup_widgets)
 
-    def go_back(self, instance):
-        self.ini.update_value(__program__, 'LASTSETUP_TYPE', self.setup_type.text)
-        self.parent.current = 'MainScreen'
+class DataGridTableData(RecycleView):
+    nrows = NumericProperty(None)
+    ncols = NumericProperty(None)
+    rgrid = ObjectProperty(None)
 
-    def accept_setup(self, instance):
+    datagrid_doc_id = None
+    datagrid_background_color = None
+    # datagrid_widget_row = []
 
-        self.new_station = point()
-        self.foresight = None
-        txt = ''
-        error_message = ''
-
-        if self.setup_type.text == 'Horizontal Angle Only':
-            if self.station.location.is_none() is True:
-                txt = '\nThe location of the station has not been set.'
-            else:
-                txt = f'\nThe location of the station is at {str(self.station.location)}.  All measured points will be relative to that point and the horizontal angle uploaded here.'
-
-        elif self.setup_type.text == 'Over a datum':
-            if self.setup_widgets.over_datum.datum is None:
-                error_message = '\nSelect the datum under the total station and optionally provide the station height.'
-            else:
-                station_height = float(self.setup_widgets.station_height.text) if self.setup_widgets.station_height.text else 0
-                self.new_station = self.setup_widgets.over_datum.datum
-                self.new_station.z += station_height
-                txt = '\nSet the station coordinates to\nX : %s\nY : %s\nZ : %s' % (self.new_station.x, self.new_station.y, self.new_station.z)
-
-        elif self.setup_type.text == 'Over a datum + Record a datum':
-            if self.setup_widgets.datum1.datum is None or self.setup_widgets.datum2.datum is None:
-                error_message = '\nSelect the datum under the total station and a datum to record.'
-            elif self.setup_widgets.datum1.datum == self.setup_widgets.datum2.datum:
-                error_message = '\nSelect two different datums.'
-            elif self.station.subtract_points(self.setup_widgets.datum1.datum, self.setup_widgets.datum2.datum) == point(0, 0, 0):
-                error_message = '\nSelect two different datums with different coordinates.'
-            elif self.setup_widgets.recorder[0].result.xyz is None:
-                error_message = '\nRecord the datum before accepting the setup.'
-            else:
-                self.new_station = self.station.subtract_points(self.setup_widgets.datum2.datum, self.setup_widgets.recorder[0].result.xyz).round()
-                datum2 = self.station.add_points(self.setup_widgets.datum1.datum, self.setup_widgets.recorder[0].result.xyz).round()
-                station_error = self.station.subtract_points(self.setup_widgets.datum2.datum, datum2).round()
-                txt = f'\n{self.setup_widgets.datum2.datum.name} recorded as \nX : {datum2.x}\nY : {datum2.y}\nZ : {datum2.z}\n'
-                txt += f'\nThe error in this measurement is \nX : {station_error.x}\nY : {station_error.y}\nZ : {station_error.z}\n'
-                txt += '(Note that Z will be off by the station height in most setups)\n'
-                txt += f'\nIf the setup as measured is accepted, the new station coordinates will be \nX : {self.new_station.x}\nY : {self.new_station.y}\nZ : {self.new_station.z}'
-
-        elif self.setup_type.text == 'Record two datums':
-            if self.setup_widgets.datum1.datum is None or self.setup_widgets.datum2.datum is None:
-                error_message = '\nSelect two datums to record.'
-            elif self.setup_widgets.datum1.datum == self.setup_widgets.datum2.datum:
-                error_message = '\nSelect two different datums.'
-            elif self.station.subtract_points(self.setup_widgets.datum1.datum, self.setup_widgets.datum2.datum) == point(0, 0, 0):
-                error_message = '\nSelect two different datums with different coordinates.'
-            elif self.setup_widgets.recorder[0].result.xyz.is_none() or self.setup_widgets.recorder[1].result.xyz.is_none():
-                error_message = '\nRecord each datum.  It is important that the first datum is recorded and then the second and not the other way around.  Note that before the first datum is recorded, a horizontal angle of 0.0000 will be uploaded.'
-            else:
-                measured_distance = self.station.distance(self.setup_widgets.recorder[0].result.xyz, self.setup_widgets.recorder[1].result.xyz)
-                actual_distance = self.station.distance(self.setup_widgets.datum1.datum.as_point(), self.setup_widgets.datum2.datum.as_point())
-                error_distance = abs(measured_distance - actual_distance)
-
-                # The following code is ported from EDM-Mobile (and EDMWin).
-                # I can't remember exactly how this works, but it does work.
-                # And I remember the hot, weekend day at Carsac when Harold
-                # and I first figured out how to do this.
-
-                # Workout what the measured angle would be from datum1 to datum2
-                y = -1 * self.setup_widgets.recorder[0].result.xyz.y
-                y = y + self.setup_widgets.recorder[1].result.xyz.y
-                p = point(self.setup_widgets.recorder[1].result.xyz.x, y, 0)
-                measured_angle = self.station.angle_between_points(point(0, 0, 0), p)
-
-                # Calculate the actual angle between datum1 and datum2
-                defined_angle = self.station.angle_between_points(self.setup_widgets.datum1.datum.as_point(), self.setup_widgets.datum2.datum.as_point())
-
-                # get the difference between these two angles
-                angle_difference = defined_angle - measured_angle
-
-                # Based on this, compute the new datum.
-                self.new_station = point(round(-1 * self.setup_widgets.recorder[0].result.xyz.y * sin(d2r(angle_difference)) + self.setup_widgets.datum1.datum.x, 3),
-                                            round(-1 * self.setup_widgets.recorder[0].result.xyz.y * cos(d2r(angle_difference)) + self.setup_widgets.datum1.datum.y, 3),
-                                            round(((self.setup_widgets.datum1.datum.z - self.setup_widgets.recorder[0].result.xyz.z) + (self.setup_widgets.datum2.datum.z - self.setup_widgets.recorder[1].result.xyz.z)) / 2, 3))
-
-                # Workout what angle needs to be uploaded to the station
-                self.foresight = self.station.angle_between_points(self.new_station, self.setup_widgets.datum2.datum.as_point())
-                txt = f'\nThe measured distance between {self.setup_widgets.datum1.datum.name} and {self.setup_widgets.datum2.datum.name} was {round(measured_distance, 3)} m.  The distance based on the datum definitions should be {round(actual_distance, 3)} m.  The error is {round(error_distance, 3)} m.\n'
-                txt += f'\nIf the setup as measured is accepted, the new station coordinates will be \nX : {self.new_station.x}\nY : {self.new_station.y}\nZ : {self.new_station.z}\n'
-                txt += f'\nAn angle of {self.station.decimal_degrees_to_sexa_pretty(self.foresight)} will be uploaded (do not turn the station until this angle is set).'
-                self.foresight = self.station.decimal_degrees_to_dddmmss(self.foresight)
-
-        elif self.setup_type.text == 'Three datum shift':
-            if self.setup_widgets.datum1.datum is None or self.setup_widgets.datum2.datum is None or self.setup_widgets.datum3.datum is None:
-                error_message = '\nSelect three datums to record.'
-            elif self.setup_widgets.recorder[0].result.xyz is None or self.setup_widgets.recorder[1].result.xyz is None or self.setup_widgets.recorder[2].result.xyz is None:
-                error_message = '\nRecord each datum.'
-            else:
-                dist_12_measured = self.station.distance(self.setup_widgets.recorder[0].result.xyz, self.setup_widgets.recorder[1].result.xyz)
-                dist_12_datums = self.station.distance(self.setup_widgets.datum1.datum.as_point(), self.setup_widgets.datum2.datum.as_point())
-                dist_12_error = round(abs(dist_12_measured - dist_12_datums), 3)
-
-                dist_23_measured = self.station.distance(self.setup_widgets.recorder[1].result.xyz, self.setup_widgets.recorder[2].result.xyz)
-                dist_23_datums = self.station.distance(self.setup_widgets.datum2.datum.as_point(), self.setup_widgets.datum3.datum.as_point())
-                dist_23_error = round(abs(dist_23_measured - dist_23_datums), 3)
-
-                dist_13_measured = self.station.distance(self.setup_widgets.recorder[0].result.xyz, self.setup_widgets.recorder[2].result.xyz)
-                dist_13_datums = self.station.distance(self.setup_widgets.datum1.datum.as_point(), self.setup_widgets.datum3.datum.as_point())
-                dist_13_error = round(abs(dist_13_measured - dist_13_datums), 3)
-
-                # should also include a mean error by averaging everything
-
-                txt = '\nThe following errors are noted.  The actual distance between datums 1 and 2 is %s and the measured distance was %s.  ' % (round(dist_12_datums, 3), round(dist_12_measured, 3))
-                txt += 'The actual distance between datums 2 and 3 is %s and the measured distance was %s.  ' % (round(dist_23_datums, 3), round(dist_23_measured, 3))
-                txt += 'The actual distance between datums 1 and 3 is %s and the measured distance was %s.  ' % (round(dist_13_datums, 3), round(dist_13_measured, 3))
-                txt += '\n\nThis corresponds to errors of %s, %s, and %s, respectively.' % (dist_12_error, dist_23_error, dist_13_error)
+    datatable_widget = None
 
-        if not self.new_station.is_none() or txt:
-            self.popup = e5_MessageBox('Accept setup?', txt,
-                                        response_type = "YESNO",
-                                        call_back = [self.set_and_close, self.close_popup],
-                                        colors = self.colors)
-        else:
-            self.popup = e5_MessageBox('Error', error_message,
-                                        colors = self.colors)
+    popup = ObjectProperty(None)
 
-        self.popup.open()
+    def __init__(self, list_dicts=[], column_names = None, tb = None, e5_cfg = None, colors = None, *args, **kwargs):
+        self.nrows = len(list_dicts) if len(list_dicts) != 1 else 2
+        self.ncols = len(column_names)
+        self.id = 'datatable'
+        self.colors = colors if colors else ColorScheme()
+        self.e5_cfg = e5_cfg
 
-    def close_popup(self, instance):
-        self.popup.dismiss()
+        super(DataGridTableData, self).__init__(*args, **kwargs)
 
-    def set_and_close(self, instance):
-        if self.setup_type:
+        self.data = []
+        black = make_rgb(BLACK)
+        if len(list_dicts) == 1:
+            # This is a hack to deal with a Kivy but where the grid does not display if there is
+            # only one row.  So the solution is to insert a dummy row.
+            for column in column_names:
+                self.data.append({'text': '',
+                                    'is_even': False,
+                                    'callback': self.editcell,
+                                    'key': 0,
+                                    'field': column,
+                                    'db': tb,
+                                    'id': 'datacell',
+                                    'datagrid_even': self.colors.datagrid_even,
+                                    'datagrid_odd': self.colors.datagrid_odd,
+                                    'color': black})
+        for i, ord_dict in enumerate(list_dicts):
+            is_even = i % 2 == 0
+            for column in column_names:
+                value = ord_dict[column] if column in ord_dict.keys() else ''
+                content = {'text': value,
+                            'is_even': is_even,
+                            'callback': self.editcell,
+                            'key': ord_dict['doc_id'],
+                            'field': column,
+                            'db': tb,
+                            'id': 'datacell',
+                            'datagrid_even': self.colors.datagrid_even,
+                            'datagrid_odd': self.colors.datagrid_odd,
+                            'color': black}
+                if self.colors.datagrid_font_size:
+                    content['font_size'] = self.colors.datagrid_font_size
+                self.data.append(content)
 
-            logger = logging.getLogger(__name__)
+    def is_numeric(self, value):
+        try:
+            float(value)
+            return True
+        except ValueError:
+            return False
 
-            if self.setup_type.text == 'Horizontal Angle Only':
-                pass
+    def clear_highlight_row(self):
+        if self.datagrid_doc_id:
+            for record in self.data:
+                record['background_color'] = self.colors.datagrid_even if record['is_even'] else self.colors.datagrid_odd
+            self.refresh_from_data()
+            self.datagrid_doc_id = ''
+
+    def set_highlight_row(self):
+        for record in self.data:
+            if record['key'] == self.datagrid_doc_id:
+                record['background_color'] = self.colors.optionbutton_background
+        self.refresh_from_data()
+
+    # def get_editcell_row(self, key):
+    #    row_widgets = []
+    #    for widget in self.walk():
+    #        if hasattr(widget, 'id'):
+    #            if widget.id == 'datacell':
+    #                if widget.key == key:
+    #                    row_widgets.append(widget)
+    #    return(row_widgets)
 
-            elif self.setup_type.text == 'Over a datum':
-                self.ini.update_value('SETUPS', 'OVERDATUM', self.setup_widgets.over_datum.datum.name)
-                logger.info(f'Setup over {self.setup_widgets.over_datum.datum}')
-
-            elif self.setup_type.text == 'Over a datum + Record a datum':
-                self.ini.update_value('SETUPS', 'OVERDATUM', self.setup_widgets.datum1.datum.name)
-                self.ini.update_value('SETUPS', 'RECORDDATUM', self.setup_widgets.datum2.datum.name)
-                logger.info(f'Setup over {self.setup_widgets.datum1.datum} and recorded {self.setup_widgets.datum2.datum}')
-
-            elif self.setup_type.text == 'Record two datums':
-                self.ini.update_value('SETUPS', '2DATUMS_DATUM_1', self.setup_widgets.datum1.datum.name)
-                self.ini.update_value('SETUPS', '2DATUMS_DATUM_2', self.setup_widgets.datum2.datum.name)
-                logger.info(f'Setup 2-point using {self.setup_widgets.datum1.datum} and {self.setup_widgets.datum2.datum}')
-
-            elif self.setup_type.text == 'Three datum shift':
-                self.station.rotate_local = [self.setup_widgets.recorder[0].result.xyz,
-                                                self.setup_widgets.recorder[1].result.xyz,
-                                                self.setup_widgets.recorder[2].result.xyz]
-                self.station.rotate_global = [self.setup_widgets.datum1.datum.as_point(),
-                                                    self.setup_widgets.datum2.datum.as_point(),
-                                                    self.setup_widgets.datum3.datum.as_point()]
-                self.ini.update_value('SETUPS', '3DATUM_SHIFT_LOCAL_1', '%s,%s,%s' % (self.setup_widgets.recorder[0].result.xyz.x,
-                                                                                            self.setup_widgets.recorder[0].result.xyz.y,
-                                                                                            self.setup_widgets.recorder[0].result.xyz.z))
-                self.ini.update_value('SETUPS', '3DATUM_SHIFT_LOCAL_2', '%s,%s,%s' % (self.setup_widgets.recorder[1].result.xyz.x,
-                                                                                            self.setup_widgets.recorder[1].result.xyz.y,
-                                                                                            self.setup_widgets.recorder[1].result.xyz.z))
-                self.ini.update_value('SETUPS', '3DATUM_SHIFT_LOCAL_3', '%s,%s,%s' % (self.setup_widgets.recorder[2].result.xyz.x,
-                                                                                            self.setup_widgets.recorder[2].result.xyz.y,
-                                                                                            self.setup_widgets.recorder[2].result.xyz.z))
-                self.ini.update_value('SETUPS', '3DATUM_SHIFT_GLOBAL_1', self.setup_widgets.datum1.datum.name)
-                self.ini.update_value('SETUPS', '3DATUM_SHIFT_GLOBAL_2', self.setup_widgets.datum2.datum.name)
-                self.ini.update_value('SETUPS', '3DATUM_SHIFT_GLOBAL_3', self.setup_widgets.datum3.datum.name)
-                logger.info(f'Setup 3 datum shift using {self.setup_widgets.datum1.datum}, {self.setup_widgets.datum2.datum}, and {self.setup_widgets.datum3.datum}')
-                logger.info(f'Recorded values were respectively {self.setup_widgets.recorder[0].result.xyz}, {self.setup_widgets.recorder[1].result.xyz}, and {self.setup_widgets.recorder[2].result.xyz}')
+    def get_editcell(self, key, field):
+        for widget in self.walk():
+            if hasattr(widget, 'id'):
+                if widget.id == 'datacell':
+                    if widget.field == field and widget.key == key:
+                        return widget
+        return None
+
+    def editcell(self, key, field, db):
+        # self.key = key
+        if field == 'doc_id' and self.datagrid_doc_id == key:
+            self.clear_highlight_row()
+            return
+        self.clear_highlight_row()
+        self.datagrid_doc_id = key
+        editcell_widget = self.get_editcell(key, field)
+        self.datagrid_background_color = editcell_widget.background_color
+        self.set_highlight_row()
+        self.field = field
+        self.tb = db
+        cfg_field = self.e5_cfg.get(field)
+        self.inputtype = cfg_field.inputtype.upper()
+        text_length = int(cfg_field.length) if self.is_numeric(cfg_field.length) else 0
+        if self.inputtype in ['MENU', 'BOOLEAN']:
+            self.popup = DataGridMenuList(field, cfg_field.menu,
+                                            editcell_widget.text, self.menu_selection,
+                                            self.colors, text_length = text_length)
+            self.popup.open()
+        elif self.inputtype in ['TEXT', 'NUMERIC', 'NOTE']:
+            self.popup = DataGridTextBox(title = field, text = editcell_widget.text,
+                                            multiline = self.inputtype == 'NOTE',
+                                            call_back = self.menu_selection,
+                                            colors = self.colors, text_length = text_length)
+            self.popup.open()
+        self.datatable_widget.popup_scrollmenu = self.datatable_widget.get_widget_by_id(self.popup, 'menu_scroll')
+        self.datatable_widget.popup_textbox = self.datatable_widget.get_widget_by_id(self.popup, 'new_item')
+        self.datatable_widget.popup_addbutton = self.datatable_widget.get_widget_by_id(self.popup, 'add_button')
+        self.datatable_widget.popup = self.popup
 
+    def menu_selection(self, instance):
         self.popup.dismiss()
-        if self.foresight:
-            self.station.set_horizontal_angle(self.foresight)
-            logger.info(f'Horizontal angle set to {self.foresight}')
-        if self.new_station.is_none() is False:
-            self.station.location = self.new_station
-            logger.info('Station location set to ' + str(self.station.location))
-        self.ini.update_value('SETUPS', 'LASTSETUP_TYPE', self.setup_type.text)
-        self.ini.save()
-        self.parent.current = 'MainScreen'
+        if self.field in ['HANGLE', 'VANGLE'] and APP_NAME == 'EDM':
+            new_data = {self.field: self.datatable_widget.popup_textbox.text}
+        elif self.inputtype in ['MENU', 'BOOLEAN']:
+            new_data = {self.field: instance.text if not instance.text == 'Add' else self.datatable_widget.popup_textbox.text}
+        elif self.inputtype == 'NUMERIC':
+            if self.field in ['X', 'Y', 'Z', 'PRISM', 'SLOPED', 'STATIONX', 'STATIONY', 'STATIONZ', 'LOCALX', 'LOCALY', 'LOCALZ'] and APP_NAME == 'EDM':
+                try:
+                    self.datatable_widget.popup_textbox.text = str(eval(self.datatable_widget.popup_textbox.text))
+                except (DivisionByZero, NameError, SyntaxError):
+                    pass
+            try:
+                if '.' in self.datatable_widget.popup_textbox.text:
+                    new_data = {self.field: float(self.datatable_widget.popup_textbox.text)}
+                else:
+                    new_data = {self.field: int(self.datatable_widget.popup_textbox.text)}
+            except ValueError:
+                new_data = {self.field: self.datatable_widget.popup_textbox.text}
+        else:
+            new_data = {self.field: self.datatable_widget.popup_textbox.text}
+        is_valid = self.e5_cfg.validate_datafield(new_data, self.tb)
+        if is_valid is True:
+            self.tb.update(new_data, doc_ids = [int(self.datagrid_doc_id)])
+            self.update_recycle_data(self.datagrid_doc_id, self.field, new_data[self.field])
+            # for widget in self.walk():
+            #    if hasattr(widget, 'id'):
+            #        if widget.id == 'datacell':
+            #            if widget.key == self.datagrid_doc_id and widget.field == self.field:
+            #                widget.text = str(new_data[self.field])
+            self.datatable_widget.popup_scrollmenu = None
+            self.datatable_widget.popup_textbox = None
+        else:
+            self.popup = e5_MessageBox('Data error', is_valid)
+            self.popup.open()
 
+    def update_recycle_data(self, doc_id, field, value):
+        for record in self.data:
+            if record['key'] == doc_id and record['field'] == field:
+                record['text'] = str(value)
+                self.refresh_from_data()
+                break
 
-class EditLastRecordScreen(e5_RecordEditScreen):
-    pass
 
+class DataGridTable(BoxLayout):
 
-class EditPointScreen(e5_RecordEditScreen):
-    pass
+    def __init__(self, list_dicts=[], column_names = None, tb = None, e5_cfg = None, colors = None, *args, **kwargs):
 
+        super(DataGridTable, self).__init__(*args, **kwargs)
+        self.orientation = "vertical"
 
-class EditDatumScreen(Screen):
-    pass
+        self.header = DataGridTableHeader(column_names, colors)
+        self.table_data = DataGridTableData(list_dicts = list_dicts, column_names = column_names,
+                                            tb = tb, e5_cfg = e5_cfg, colors = colors)
 
+        self.table_data.fbind('scroll_x', self.scroll_with_header)
 
-class EditPointsScreen(e5_DatagridScreen):
-    pass
+        self.add_widget(self.header)
+        self.add_widget(self.table_data)
 
+    def scroll_with_header(self, obj, value):
+        self.header.scroll_x = value
 
-class EditPrismsScreen(e5_DatagridScreen):
-    pass
 
+class DataGridGridPanel(BoxLayout):
 
-class EditUnitsScreen(e5_DatagridScreen):
-    pass
+    def populate_data(self, tb, tb_fields, colors = None):
+        if tb is not None and tb_fields is not None:
+            self.colors = colors if colors else ColorScheme()
+            self.tb = tb
+            self.sort_key = None
+            self.column_names = ['doc_id'] + tb_fields.fields()
+            self.tb_fields = tb_fields
+            self._generate_table()
 
+    def _generate_table(self, sort_key = None, disabled = None):
+        self.clear_widgets()
+        data = []
+        table_fields = self.tb_fields.fields()
+        for tb_row in self.tb:
+            reformatted_row = {}
+            reformatted_row['doc_id'] = str(tb_row.doc_id)
+            for field in table_fields:
+                reformatted_row[field] = str(tb_row[field]) if field in tb_row else ''
+            data.append(reformatted_row)
+        data = sorted(data, key=lambda k: int(k['doc_id']), reverse = True)
+        self.recycleview_box = DataGridTable(list_dicts = data, column_names = self.column_names,
+                                                tb = self.tb, e5_cfg = self.tb_fields, colors = self.colors)
+        self.add_widget(self.recycleview_box)
+
+
+class DataGridCasePanel(BoxLayout):
+
+    changed = False
+    id = 'datagridcase'
+
+    def populate(self, data, fields, colors = None, call_back = None, revert = None):
+        if data is not None and fields is not None:
+            self.colors = colors if colors else ColorScheme()
+            self.edit_list.bind(minimum_height = self.edit_list.setter('height'))
+            self.edit_list.clear_widgets()
+            for col in fields.fields():
+                label_and_text = DataGridLabelAndField(col = col, prompt = fields.get(col).prompt, colors = self.colors)
+                label_and_text.txt.textbox.bind(on_text_validate = self.next_field)
+                self.edit_list.add_widget(label_and_text)
+                label_and_text.txt.textbox.bind(text = self.changes)
+            self.add_widget(e5_side_by_side_buttons(text = ['Revert', 'Save'],
+                                                    call_back = [revert, call_back],
+                                                    colors = self.colors))
+        self.changed = False
 
-class EditDatumsScreen(e5_DatagridScreen):
-    pass
+    def next_field(self, instance):
+        pass
 
+    def changes(self, instance, value):
+        self.changed = True
 
-class station_setting(GridLayout):
-    label = ObjectProperty(None)
-    spinner = ObjectProperty(None)
-    id = ObjectProperty(None)
-    comport_to_test = None
-    valid_comports = []
 
-    def __init__(self, label_text = '', spinner_values = (), default = '',
-                        id = None, call_back = None, colors = None, station = None, **kwargs):
-        super(station_setting, self).__init__(**kwargs)
+class DataGridLabelAndProgressBar(BoxLayout):
 
-        self.station = station
-        self.id = id
-        self.cols = 2
-        self.pos_hint = {'center_x': .5},
-        self.colors = colors
-        self.label = e5_label(text = label_text, colors = colors)
+    def __init__(self, col, active = False, colors = None, popup = False, **kwargs):
+        super(DataGridLabelAndProgressBar, self).__init__(**kwargs)
+        self.colors = colors if colors is not None else ColorScheme()
+        self.size_hint = (0.9, None)
+        self.bind(minimum_height = self.setter('height'))
+        self.spacing = 10
+        self.label = e5_label(text = col, id = '__label', colors = self.colors, popup = popup, size_hint_y = None, halign = 'center')
+        self.label.bind(texture_size = self.label.setter('size'))
+        self.bar = ProgressBar(max = 1)
+        self.bar.height = 50
         self.add_widget(self.label)
+        self.add_widget(self.bar)
 
-        # Create a default dropdown button and then modify its properties
-        # For some reason, the usual font size specification doesn't work here and sp has to be removed
-        spinner_dropdown_button = SpinnerOptions
-        spinner_dropdown_button.font_size = colors.button_font_size.replace("sp", '') if colors.button_font_size else None
-        spinner_dropdown_button.background_color = (0, 0, 0, 1)
-
-        self.spinner = Spinner(text = default if default is not None else '',
-                                values = spinner_values,
-                                font_size = colors.button_font_size if colors.button_font_size else None,
-                                option_cls = spinner_dropdown_button)
-        if label_text == 'Port Number':
-            comport = GridLayout(cols = 2, spacing = 5)
-            comport.bind(minimum_height = comport.setter('height'))
-            comport.add_widget(self.spinner)
-            comport.add_widget(e5_button('Scan', colors = colors, call_back = self.scanner))
-            self.add_widget(comport)
-        else:
-            self.add_widget(self.spinner)
-        if call_back:
-            self.spinner.bind(text = call_back)
 
-    def scanner(self, instance):
-        if self.station:
-            ports = self.station.list_comports()
-            text = 'Available ports:\n\n'
-            for port in ports:
-                text += '%s - %s\n' % (port[0]['port'], port[0]['desc'])
-            self.spinner.values = list([port[0]['port'] for port in ports])
-            self.popup = e5_MessageBox('COM Ports', text,
-                                        response_type = "OK",
-                                        call_back = self.close_popup_comports,
-                                        colors = self.colors)
-            self.popup.open()
-            self.popup_open = True
-        else:
-            self.event1 = Clock.schedule_once(self.show_popup_message, .2)
-            self.event2 = Clock.schedule_interval(self.check_comports, .2)
-
-    def show_popup_message(self, dt):
-        self.popup = e5_MessageBox('COM Ports', '\nLooking for valid COM ports...This can take several seconds...And the Cancel button might appear non-responsive...',
-                                    response_type = "CANCEL",
-                                    call_back = self.close_popup,
-                                    colors = self.colors)
-        self.popup.open()
-        self.popup_open = True
+class DataGridLabelAndToggle(BoxLayout):
 
-    def close_popup(self, value):
-        self.popup.dismiss()
-        self.popup_open = False
-        self.event2.cancel()
-        self.comport_to_test = None
+    def __init__(self, col, active = False, colors = None, popup = False, **kwargs):
+        super(DataGridLabelAndToggle, self).__init__(**kwargs)
+        self.colors = colors if colors is not None else ColorScheme()
+        self.size_hint = (0.9, None)
+        self.bind(minimum_height = self.setter('height'))
+        self.spacing = 10
+        label = e5_label(text = col, id = '__label', colors = self.colors, popup = popup)
+        label.bind(texture_size = label.setter('size'))
+        self.check = Switch(active = active, size_hint = (0.75, None))
+        self.check.height = 30
+        self.add_widget(label)
+        self.add_widget(self.check)
 
-    def close_popup_comports(self, value):
-        self.popup.dismiss()
-        self.popup_open = False
 
-    def comportIsUsable(self, portName):
-        try:
-            ser = serial.Serial(port = portName)
-            ser.close()
-            return portName
-        except:
-            return None
-
-    def check_comports(self, dt):
-        if self.comport_to_test is None:
-            self.comport_to_test = 0
-            self.valid_comports = []
-        self.comport_to_test += 1
-        if self.comport_to_test > __LASTCOMPORT__:
-            self.spinner.values = list(filter(None.__ne__, self.valid_comports))
-            self.event2.cancel()
-            self.close_popup(None)
-            self.comport_to_test = None
-        else:
-            self.valid_comports.append(self.comportIsUsable("COM%s" % self.comport_to_test))
-
-    def comports(self):
-        return list(filter(None.__ne__, [self.comportIsUsable("COM%s" % comno) for comno in range(1, __LASTCOMPORT__ + 1)]))
+class DataGridLabelAndField(BoxLayout):
 
+    popup = ObjectProperty(None)
+    sorted_result = None
 
-class StationConfigurationScreen(Screen):
+    def __init__(self, col, colors, prompt = '', note_field = False, popup = False, text_length = 0, height = None, **kwargs):
+        super(DataGridLabelAndField, self).__init__(**kwargs)
+        self.update_db = False
+        self.widget_type = 'data'
+        if not note_field:
+            if colors:
+                if colors.text_font_size:
+                    self.height = int(colors.text_font_size.replace('sp', '')) * 1.9
+        self.size_hint = (0.9, None)
+        self.bind(minimum_height = self.setter('height'))
+        self.spacing = 10
+        label = e5_label(text = prompt if prompt else col, id = '__label',
+                            colors = colors, popup = popup, size_hint_y = None,
+                            halign = 'right', label_height = height)
+        label.bind(texture_size = label.setter('size'))
+        self.txt = e5_textinput(multiline = note_field,
+                                size_hint = (0.75, None),
+                                id = col,
+                                # size_hint_y = 1,
+                                text_length = text_length,
+                                write_tab = False)
+        self.txt.bind(minimum_height = self.txt.setter('height'))
+        if colors:
+            if colors.text_font_size:
+                self.txt.font_size = colors.text_font_size
+        self.add_widget(label)
+        self.add_widget(self.txt)
 
-    def __init__(self, station = None, ini = None, colors = None, **kwargs):
-        super(StationConfigurationScreen, self).__init__(**kwargs)
 
-        self.station = station
-        self.colors = colors
-        self.ini = ini
-        self.call_back = 'MainScreen'
+class DataGridDeletePanel(GridLayout):
 
-    def on_enter(self):
+    def populate(self, message = None, call_back = None, colors = None):
+        self.colors = colors if colors else ColorScheme()
         self.clear_widgets()
-        self.layout = GridLayout(cols = 1,
-                                 spacing = 5,
-                                 size_hint_x = width_calculator(.9, 400),
-                                 size_hint_y = .9,
-                                 pos_hint = {'center_x': .5, 'center_y': .5})
-        self.add_widget(self.layout)
-        self.build_screen()
-
-    def build_screen(self):
-        self.station_type = station_setting(label_text = 'Station type',
-                                            spinner_values = ("Leica", "Wild", "Topcon", "Sokkia", "Microscribe", "Manual XYZ", "Manual VHD", "Simulate"),
-                                            call_back = self.toggle_buttons,
-                                            id = 'station_type',
-                                            colors = self.colors,
-                                            default = self.ini.get_value(__program__, 'STATION'))
-        self.layout.add_widget(self.station_type)
-
-        self.communications = station_setting(label_text = 'Communications',
-                                                spinner_values = ("Serial", "Bluetooth"),
-                                                # call_back = self.update_ini,
-                                                id = 'communications',
-                                                colors = self.colors,
-                                                default = self.ini.get_value(__program__, 'COMMUNICATIONS'))
-        self.layout.add_widget(self.communications)
-
-        self.comports = station_setting(label_text = 'Port Number',
-                                            spinner_values = [],
-                                            # call_back = self.update_ini,
-                                            id = 'comport',
-                                            colors = self.colors, station = self.station,
-                                            default = self.ini.get_value(__program__, 'COMPORT'))
-        self.layout.add_widget(self.comports)
-
-        self.baud_rate = station_setting(label_text = 'Baud rate',
-                                            spinner_values = ("1200", "2400", "4800", "9600", "14400", "19200"),
-                                            # call_back = self.update_ini,
-                                            id = 'baudrate',
-                                            colors = self.colors,
-                                            default = self.ini.get_value(__program__, 'BAUDRATE'))
-        self.layout.add_widget(self.baud_rate)
-
-        self.parity = station_setting(label_text = 'Parity',
-                                            spinner_values = ("Even", "Odd", "None"),
-                                            # call_back = self.update_ini,
-                                            id = 'parity',
-                                            colors = self.colors,
-                                            default = self.ini.get_value(__program__, 'PARITY'))
-        self.layout.add_widget(self.parity)
-
-        self.data_bits = station_setting(label_text = 'Databits',
-                                            spinner_values = ("7", "8"),
-                                            # call_back = self.update_ini,
-                                            id = 'databits',
-                                            colors = self.colors,
-                                            default = self.ini.get_value(__program__, 'DATABITS'))
-        self.layout.add_widget(self.data_bits)
-
-        self.stop_bits = station_setting(label_text = 'Stopbits',
-                                            spinner_values = ("0", "1", "2"),
-                                            # call_back = self.update_ini,
-                                            id = 'stopbits',
-                                            colors = self.colors,
-                                            default = self.ini.get_value(__program__, 'STOPBITS'))
-        self.layout.add_widget(self.stop_bits)
-
-        self.buttons = e5_side_by_side_buttons(text = ['Back', 'Set'],
-                                                id = ['Back', 'Set'],
-                                                selected = [True, False],
-                                                call_back = [self.close_screen, self.update_ini],
-                                                colors = self.colors)
-        self.layout.add_widget(self.buttons)
-        self.toggle_buttons(None, None)
-        self.changes = False
-
-    def toggle_buttons(self, instance, value):
-        disabled = self.station_type.spinner.text in ['Simulate', 'Microscribe']
-        self.stop_bits.spinner.disabled = disabled
-        self.parity.spinner.disabled = disabled
-        self.data_bits.spinner.disabled = disabled
-        self.baud_rate.spinner.disabled = disabled
-        self.comports.spinner.disabled = disabled
-        self.communications.spinner.disabled = disabled
-
-    def update_ini(self, instance):
-        self.station.make = self.station_type.spinner.text
-        self.ini.update_value(__program__, 'STATION', self.station_type.spinner.text)
-
-        self.station.stopbits = self.stop_bits.spinner.text
-        self.ini.update_value(__program__, 'STOPBITS', self.stop_bits.spinner.text)
-
-        self.station.baudrate = self.baud_rate.spinner.text
-        self.ini.update_value(__program__, 'BAUDRATE', self.baud_rate.spinner.text)
-
-        self.station.databits = self.data_bits.spinner.text
-        self.ini.update_value(__program__, 'DATABITS', self.data_bits.spinner.text)
-
-        self.station.comport = self.comports.spinner.text
-        self.ini.update_value(__program__, 'COMPORT', self.comports.spinner.text)
-
-        self.station.parity = self.parity.spinner.text
-        self.ini.update_value(__program__, 'PARITY', self.parity.spinner.text)
-
-        self.station.communications = self.communications.spinner.text
-        self.ini.update_value(__program__, 'COMMUNICATIONS', self.communications.spinner.text)
+        self.cols = 1
+        self.spacing = 5
+        if message is not None:
+            self.add_widget(e5_scrollview_label(message, popup = False, colors = self.colors))
+            self.add_widget(e5_button('Delete',
+                                        id = 'delete',
+                                        selected = True,
+                                        call_back = call_back, colors = self.colors))
+        else:
+            self.add_widget(e5_scrollview_label('\nHighlight a record in the grid view (data tab) by clicking on its doc_id, '
+                                                'and then delete that record here.',
+                                                popup = False, colors = self.colors))
+
+
+class DataGridAddNewPanel(GridLayout):
+
+    def populate(self, data, fields, colors = None, addnew = False, call_back = None):
+        if data is not None and fields is not None:
+            self.colors = colors if colors else ColorScheme()
+            self.cols = 1
+            if addnew:
+                self.addnew_list.bind(minimum_height = self.addnew_list.setter('height'))
+                self.addnew_list.clear_widgets()
+                for col in fields.fields():
+                    label_and_text = DataGridLabelAndField(col = col, colors = self.colors)
+                    label_and_text.txt.bind(on_text_validate = self.next_field)
+                    self.addnew_list.add_widget(label_and_text)
+                self.button = e5_button('Add record',
+                                            id = 'addnew',
+                                            selected = False,
+                                            call_back = call_back, colors = self.colors)
+                self.add_widget(self.button)
+                self.call_back = call_back
+            else:
+                self.clear_widgets()
+                if APP_NAME == 'EDM':
+                    self.add_widget(e5_scrollview_label('\nAdding records in this way is not enabled for the main points table but is enabled '
+                                                        'for datums, units and prisms.',
+                                                        popup = False, colors = self.colors))
+                else:
+                    self.add_widget(e5_scrollview_label('\nAdding records in this way is not enabled in E5 because it would bipass conditions '
+                                                        'and error checking (but it is enabled in EDM which is why it appears in this list of tabs).',
+                                                        popup = False, colors = self.colors))
 
-        self.ini.save()
-        self.station.open()
-        self.close_screen(None)
+    def next_field(self, instance):
+        if instance.get_focus_next() == self.button:
+            if self.call_back:
+                self.call_back(instance)
+                instance.get_focus_next().get_focus_next().focus = True
+        else:
+            instance.get_focus_next().focus = True
 
-    def close_screen(self, value):
-        self.parent.current = self.call_back
 
-# Region Help Screens
+class DataGridWidget(TabbedPanel):
+    data = ObjectProperty(None)
+    fields = ObjectProperty(None)
+    colors = ObjectProperty(None)
 
+    popup = None
+    popup_open = False
+    popup_scrollmenu = None
+    popup_addbutton = None
+    popup_textbox = None
+    popup_field_widget = None
+
+    def __init__(self, data = None, cfg = None, colors = None, addnew = False, **kwargs):
+        super(DataGridWidget, self).__init__(**kwargs)
+
+        self.addnew = addnew
+
+        if data is not None:
+            self.data = data
+        if cfg is not None:
+            self.fields = cfg
+            self.cfg = cfg
 
-class AboutScreen(e5_InfoScreen):
-    def on_pre_enter(self):
-        self.content.text = '\n\nEDM by Shannon P. McPherron\n\nVersion ' + __version__ + ' Alpha\nApple Pie\n\n'
-        self.content.text += 'Built using Python 3.8, Kivy 2.0 and TinyDB 4.0\n\n'
-        self.content.text += 'An OldStoneAge.Com Production\n\n' + __date__
-        self.content.halign = 'center'
-        self.content.valign = 'middle'
-        self.content.color = self.colors.text_color
-        self.back_button.background_color = self.colors.button_background
-        self.back_button.color = self.colors.button_color
+        self.colors = colors if colors else ColorScheme()
+        self.color = self.colors.text_color
+        self.background_color = self.colors.window_background
+        self.background_image = ''
+
+        if data is not None and self.fields is not None:
+            self.populate_panels()
+
+        # if not addnew:
+        #    self.tab_list.remove(self.get_tab_by_name('Add New'))
+
+        for tab in self.tab_list:
+            tab.color = make_rgb(WHITE)
+            tab.background_color = MIDDLE_GREY
+            if self.colors.datagrid_font_size:
+                tab.font_size = self.colors.datagrid_font_size
+
+    def record_count(self):
+        datatable = self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable')
+        return datatable.nrows if datatable else 0
+
+    def reload_data(self):
+        # This next conditional is to avoid an exception in unit testing
+        if hasattr(self, 'panel1'):
+            self.panel1.populate_data(tb = self.data, tb_fields = self.cfg, colors = self.colors)
+            if self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable'):
+                self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable').datatable_widget = self
+        # self.populate_panels()
+
+    # def load_data(self, data, fields):
+    #    self.data = data
+    #    self.fields = fields
+    #    self.populate_panels()
+
+    def populate_panels(self):
+        # This next conditional is to avoid an exception in unit testing
+        if hasattr(self, 'panel1'):
+            self.panel1.populate_data(tb = self.data, tb_fields = self.cfg, colors = self.colors)
+            self.panel2.populate(data = self.data, fields = self.fields, colors = self.colors,
+                                    call_back = self.save_record, revert = self.load_record)
+            self.panel3.populate(colors = self.colors)
+            self.panel4.populate(addnew = self.addnew,
+                                    data = self.data,
+                                    fields = self.fields,
+                                    colors = self.colors,
+                                    call_back = self.addnew_record)
+            if self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable'):
+                self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable').datatable_widget = self
+
+    def open_panel1(self):
+        self.check_changes()
+        if self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable'):
+            self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable').datatable_widget = self
+        self.panel1.children[0].children[0].refresh_from_data()
+
+    def open_panel2(self):
+        datatable = self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable')
+        if datatable is not None:
+            if datatable.datagrid_doc_id is not None and datatable.datagrid_doc_id != '':
+                data_record = self.data.get(doc_id = int(datatable.datagrid_doc_id))
+                for widget in self.panel2.walk():
+                    if hasattr(widget, 'id'):
+                        if widget.id in self.fields.fields():
+                            widget.text = str(data_record[widget.id]) if widget.id in data_record else ''
+                            widget.bind(focus = self.show_menu)
+            else:
+                cfg_fields = self.fields.fields()
+                for widget in self.panel2.walk():
+                    if hasattr(widget, 'id'):
+                        if widget.id in cfg_fields:
+                            widget.text = ''
+            self.get_widget_by_id(self.panel2, 'datagridcase').changed = False
+
+    def open_panel3(self):
+        self.check_changes()
+        datatable = self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable')
+        if datatable is not None:
+            if datatable.datagrid_doc_id:
+                data_record = self.data.get(doc_id = int(datatable.datagrid_doc_id))
+                if data_record:
+                    serialize_record = '\nDelete this record?\n\n'
+                    for field in self.fields.fields():
+                        if field in data_record.keys():
+                            serialize_record += field + f" : {data_record[field]}\n"
+                    self.panel3.populate(message = serialize_record,
+                                            call_back = self.confirm_delete_record,
+                                            colors = self.colors)
 
+    def open_panel4(self):
+        self.check_changes()
+        if self.fields is not None:
+            cfg_fields = self.fields.fields()
+            # TODO this seems like a bug - not sure why edit_panel is being cleared here
+            for widget in self.ids.edit_panel.children[0].walk():
+                if hasattr(widget, 'id'):
+                    if widget.id in cfg_fields:
+                        widget.text = ''
+
+    def show_menu(self, instance, value):
+        if instance.focus:
+            cfg_field = self.fields.get(instance.id)
+            if cfg_field:
+                self.popup_field_widget = instance
+                if cfg_field.inputtype in ['MENU', 'BOOLEAN']:
+                    self.popup = DataGridMenuList(instance.id, cfg_field.menu,
+                                                    instance.text, self.menu_selection, colors = self.colors)
+                    self.popup.open()
+                    self.popup_scrollmenu = self.get_widget_by_id(self.popup, 'menu_scroll')
+                    self.popup_textbox = self.get_widget_by_id(self.popup, 'new_item')
+                    self.popup_addbutton = self.get_widget_by_id(self.popup, 'add_button')
 
-class StatusScreen(e5_InfoScreen):
+    def menu_selection(self, instance):
+        self.popup.dismiss()
+        self.popup_field_widget.text = instance.text if not instance.id == 'add_button' else self.popup_textbox.text
+        self.popup_field_widget = None
+        self.popup_scrollmenu = None
+
+    def check_changes(self):
+        if self.get_widget_by_id(self.panel2, 'datagridcase').changed:
+            self.open_popup(e5_MessageBox('Save changes?', '\nSave the changes made to this record?',
+                                            response_type = 'YESNO',
+                                            call_back = [self.save_record, self.save_record_not],
+                                            colors = self.colors))
 
-    def __init__(self, data = None, ini = None, cfg = None, station = None, **kwargs):
-        super(StatusScreen, self).__init__(**kwargs)
-        self.data = data
-        self.ini = ini
-        self.cfg = cfg
-        self.station = station
+    def clear_addnew(self):
+        cfg_fields = self.fields.fields()
+        for widget in self.ids.addnew_panel.children[1].walk():
+            if hasattr(widget, 'id'):
+                if widget.id in cfg_fields:
+                    if widget.text:
+                        widget.text = ''
+
+    def load_record(self, instance):
+        datatable = self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable')
+        if datatable is not None:
+            if datatable.datagrid_doc_id is not None and datatable.datagrid_doc_id != '':
+                data_record = self.data.get(doc_id = int(datatable.datagrid_doc_id))
+                self.load_record_into_widgets(self.panel2, data_record)
+
+    def load_record_into_widgets(self, root, record):
+        for widget in root.walk():
+            if hasattr(widget, 'id'):
+                if widget.id in self.fields.fields():
+                    if widget.id in record.keys():
+                        widget.text = record[widget.id]
+                    else:
+                        widget.text = ''
 
-    def on_pre_enter(self):
-        txt = self.data.status() if self.data else 'A data file has not been initialized or opened.\n\n'
-        txt += self.cfg.status() if self.cfg else 'A CFG is not open.\n\n'
-        txt += self.ini.status() if self.ini else 'An INI file is not available.\n\n'
-        txt += self.station.status() if self.station else 'Total station information is not available.\n\n'
-        txt += '\nThe default user path is %s.\n' % self.ini.get_value(__program__, "APP_PATH")
-        logger = logging.getLogger(__name__)
-        txt += f'\nThe log is written to {logger.handlers[0].baseFilename}\n'
-        txt += '\nThe operating system is %s.\n' % platform_name()
-        txt += '\nPython build is %s.\n' % (python_version())
-        txt += '\nLibraries installed include Kivy %s and TinyDB %s.\n' % (__kivy_version__, __tinydb_version__)
-        txt += '\nEDM was tested and distributed most recently on Python 3.8.1, Kivy 2.0.0 and TinyDB 4.4.0.\n'
-        self.content.text = txt
-        self.content.color = self.colors.text_color
-        self.back_button.background_color = self.colors.button_background
-        self.back_button.color = self.colors.button_color
+    def build_record_from_widgets(self, root):
+        new_record = {}
+        cfg_fields = self.fields.fields()
+        for widget in root.walk():
+            if hasattr(widget, 'id'):
+                if widget.id in cfg_fields:
+                    if widget.text:
+                        if self.cfg.save_as_numeric_field(widget.id):
+                            if '.' in widget.text:
+                                new_record[widget.id] = float(widget.text)
+                            else:
+                                new_record[widget.id] = int(widget.text)
+                        else:
+                            new_record[widget.id] = widget.text
+        return new_record
 
-# endregion
+    def strip_strings_from_number_fields(self, new_record):
+        for field, value in new_record.items():
+            f = self.cfg.get(field)
+            if f.inputtype == 'NUMERIC':
+                try:
+                    new_record[field] = float(value)
+                except ValueError:
+                    pass
+        return new_record
 
-# sm = ScreenManager(id = 'screen_manager')
+    def addnew_record(self, instance):
+        new_record = self.build_record_from_widgets(self.ids.addnew_panel.children[1])
+        valid_data = self.cfg.validate_datarecord(new_record, self.data)
+        if valid_data is True:
+            self.data.insert(self.strip_strings_from_number_fields(new_record))
+            self.data.new_data = True  # TODO Needs to reference parent
+            self.panel1.populate_data(tb = self.data, tb_fields = self.fields, colors = self.colors)
+            self.clear_addnew()
+        else:
+            self.popup = e5_MessageBox("Save error", valid_data, call_back = self.close_popup)
+            self.popup.open()
+            self.popup_open = True
 
+    def save_record(self, instance):
+        datatable = self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable')
+        if datatable is not None:
+            new_record = self.build_record_from_widgets(self.panel2)
+            valid_data = self.cfg.validate_datarecord(new_record, self.data)
+            if valid_data is True:
+                unique_error = self.check_unique_together(int(datatable.datagrid_doc_id), new_record)
+                if unique_error == '':
+                    self.data.update(new_record, doc_ids = [int(datatable.datagrid_doc_id)])
+                    self.get_widget_by_id(self.panel2, 'datagridcase').changed = False
+                    self.update_datagrid_record(datatable.datagrid_doc_id, new_record)
+                    self.data.new_data = True  # TODO Needs to reference parent
+                    self.close_popup(None)
+                else:
+                    self.open_popup(e5_MessageBox("Save error", unique_error, call_back = self.close_popup))
+            else:
+                self.open_popup(e5_MessageBox("Save error", valid_data, call_back = self.close_popup))
 
-sm = ScreenManager()
+    def save_record_not(self, instance):
+        self.get_widget_by_id(self.panel2, 'datagridcase').changed = False
+        self.close_popup(None)
 
+    def get_field_type(self, fieldname):
+        f = self.cfg.get(fieldname)
+        return f.inputtype
 
-class EDMApp(App):
+    def get_unique_key(self, data_record):
+        unique_key = []
+        for field in self.cfg.unique_together:
+            unique_key.append("%s" % data_record[field] if field in data_record else '')
+        return ",".join(unique_key)
 
-    def __init__(self, **kwargs):
-        super(EDMApp, self).__init__(**kwargs)
+    def check_unique_together(self, current_doc_id, new_record):
+        unique_error = ''
+        if self.cfg.unique_together and len(self.data) > 1:
+            unique_key = self.get_unique_key(new_record)
+            for record in self.data.all():
+                if record.doc_id != current_doc_id:
+                    if unique_key == self.get_unique_key(record):
+                        unique_error = f'Based on the unique together field(s) {",".join(self.cfg.unique_together)}, '\
+                                        f'this record\'s unique key of {unique_key} duplicates another record.  This is not allowed.'
+                        break
+        return unique_error
+
+    def update_datagrid_record(self, doc_id, new_record):
+        datatable = self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable')
+        for record in datatable.data:
+            if record['key'] == doc_id and record['field'] in new_record.keys():
+                record['text'] = str(new_record[record['field']])
+        self.get_tab_by_name('Data').content.recycleview_box.table_data.refresh_from_data()
+
+    def update_datagrid_field(self, doc_id, field, value):
+        datatable = self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable')
+        for record in datatable.data:
+            if record['key'] == doc_id and record['field'] == field:
+                record['text'] = str(value)
+                self.get_tab_by_name('Data').content.recycleview_box.table_data.refresh_from_data()
+                break
+
+    def confirm_delete_record(self, instance):
+        self.popup = e5_MessageBox('Delete record', '\nAre you sure you want to delete this record?',
+                                    response_type = "YESNO",
+                                    call_back = [self.delete_record, self.close_popup],
+                                    colors = self.colors)
+        self.popup.open()
+        self.popup_open = True
 
-        if platform_name() != 'Android':
-            self.app_path = os.path.abspath(os.path.dirname(__file__))
-        else:
-            self.app_path = self.user_data_dir
+    def delete_record(self, value):
+        self.close_popup(value)
+        datatable = self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable')
+        if datatable is not None:
+            doc_id = int(datatable.datagrid_doc_id)
+            self.data.remove(doc_ids = [doc_id])
+            datatable.datagrid_doc_id = None
+            # datatable.datagrid_widget_row = None
+            self.reload_data()
+            self.panel3.populate(colors = self.colors)
+            self.switch_to(self.get_tab_by_name('Data'))
 
-    def build(self):
-        sm.add_widget(MainScreen(user_data_dir = self.app_path, name = 'MainScreen'))
-        sm.current = 'MainScreen'
-        # Window.borderless = True
-        self.title = __program__ + " " + __version__
-        return(sm)
+    def open_popup(self, content):
+        self.popup = content
+        self.popup.open()
+        self.popup_open = True
 
+    def close_popup(self, value):
+        if self.popup:
+            self.popup.dismiss()
+        self.popup_open = False
 
-Factory.register(__program__, cls = EDMApp)
+    # repeats code above - could be put into a general functions package
+    def get_widget_by_id(self, start = None, id = ''):
+        start_here = self if start is None else start
+        for widget in start_here.walk():
+            if hasattr(widget, 'id'):
+                if widget.id == id:
+                    return widget
+        return None
+
+    def get_tab_by_name(self, text = ''):
+        for tab in self.tab_list:
+            if tab.text == text:
+                return tab
+        return None
+
+    def close_panels(self):
+        self.check_changes()
+        self.parent.parent.current = 'MainScreen'
 
+    def cancel(self):
+        pass
 
-if __name__ == '__main__':
-    Config.set('input', 'mouse', 'mouse,multitouch_on_demand')      # Removes red dot
-    EDMApp().run()
+# End code from https://github.com/MichaelStott/DataframeGUIKivy/blob/master/dfguik.py
+# endregion
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `edm-arch-1.0.27/src/edmpy/lib/blockdata.py` & `edm-arch-1.0.32/src/edmpy/lib/blockdata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # To Do
 #   Consider implications of not writing the block data after each update
 
 import logging
 import os
-from edmpy.lib.constants import __program__
+
+from lib.constants import APP_NAME
 
 
 class blockdata:
 
     filename = ''
     blocks = []
 
@@ -16,29 +17,29 @@
         for block in self.blocks:
             if block['BLOCKNAME'] == blockname.upper():
                 block_exists = True
                 if (varname.upper() in block.keys()) and append:
                     block[varname.upper()] = [block[varname.upper()], vardata]
                 else:
                     block[varname.upper()] = vardata
-                return(True)
+                return True
         if not block_exists:
             temp = {}
             temp['BLOCKNAME'] = blockname.upper()
             temp[varname.upper()] = vardata
             self.blocks.append(temp)
-            return(True)
-        return(False)
+            return True
+        return False
 
     def get_block(self, blockname):
         if self.blocks:
             for block in self.blocks:
                 if block['BLOCKNAME'] == blockname.upper():
-                    return(block)
-        return('')
+                    return block
+        return ''
 
     def read_blocks(self):
         self.blocks = []
         try:
             if os.path.isfile(self.filename):
                 with open(self.filename) as f:
                     for line in f:
@@ -54,35 +55,35 @@
                 f = open(self.filename, mode = 'w')
                 f.close()
         except Exception as ex:
             template = "An exception of type {0} occurred. Arguments:\n{1!r}"
             message = template.format(type(ex).__name__, ex.args)
             logging.exception(message)
             print(message)
-        return(self.blocks)
+        return self.blocks
 
     def names(self):
         name_list = []
         for block in self.blocks:
             name_list.append(block['BLOCKNAME'])
-        return(name_list)
+        return name_list
 
     def fields(self):
-        field_names = [field for field in self.names() if field not in [__program__]]
-        return(field_names)
+        field_names = [field for field in self.names() if field not in [APP_NAME]]
+        return field_names
 
     def get_value(self, blockname, varname):
         if self.blocks:
             for block in self.blocks:
                 if block['BLOCKNAME'] == blockname.upper():
                     if varname.upper() in block.keys():
-                        return(block[varname.upper()])
+                        return block[varname.upper()]
                     else:
-                        return('')
-        return('')
+                        return ''
+        return ''
 
     def delete_key(self, blockname, key):
         for block in self.blocks:
             if block['BLOCKNAME'] == blockname.upper():
                 block.pop(key)
                 return
 
@@ -98,22 +99,22 @@
                 block[new_key] = block.pop(old_key)
                 return
 
     def write_blocks(self):
         try:
             with open(self.filename, mode = 'w') as f:
                 for block in self.blocks:
-                    f.write("[%s]\n" % block['BLOCKNAME'])
+                    f.write(f"[{block['BLOCKNAME']}]\n")
                     for item in block.keys():
                         if not item == 'BLOCKNAME' and not item[:2] == "__":
-                            if block[item]:
-                                f.write(item + "=%s\n" % block[item])
+                            if block[item] != '' and block[item] is not None:
+                                f.write(f"{item}={block[item]}\n")
                     f.write("\n")
-            return(True)
+            return True
         except OSError:
-            return(False)
+            return False
 
     def save(self):
         self.write_blocks()
 
     def __len__(self):
-        return(len(self.blocks))
+        return len(self.blocks)
```

### Comparing `edm-arch-1.0.27/src/edmpy/lib/colorscheme.py` & `edm-arch-1.0.32/src/edmpy/lib/colorscheme.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from kivy.core.window import Window
-from edmpy.lib.misc import platform_name
+from lib.misc import platform_name
 
 BLACK = 0x000000
 WHITE = 0xFFFFFF
+MIDDLE_GREY = (.5, .5, .5, 1)
+DARK_GREY = (.2, .2, .2, 1)
 
 # Color from Google material design
 # https://material.io/design/color/the-color-system.html#tools-for-picking-colors
 GOOGLE_COLORS = {'red': [0xFF8A80, BLACK, 0xFF1744, WHITE],
                                 'pink': [0xFF80AB, BLACK, 0xF50057, WHITE],
                                 'purple': [0xEA80FC, BLACK, 0xD500F9, WHITE],
                                 'deep purple': [0xB388FF, BLACK, 0x651FFF, WHITE],
@@ -22,18 +24,18 @@
                                 'amber': [0xFFE57F, BLACK, 0xFFC400, BLACK],
                                 'orange': [0xFFD180, BLACK, 0xFF9100, BLACK],
                                 'deep orange': [0xFF9E80, BLACK, 0xFF3D00, WHITE],
                                 'brown': [0x8D6E63, WHITE, 0x6D4C41, WHITE]}
 
 
 def make_rgb(hex_color):
-    return([((hex_color >> 16) & 0xFF) / 255.0,
+    return [((hex_color >> 16) & 0xFF) / 255.0,
             ((hex_color >> 8) & 0xFF) / 255.0,
             (hex_color & 0xFF) / 255.0,
-            1])
+            1]
 
 
 class ColorScheme:
 
     def __init__(self, color_name = 'light blue'):
 
         if platform_name() == 'Android':
@@ -87,19 +89,19 @@
         self.need_redraw = True
         self.window_background = (1, 1, 1, 1)
         self.text_color = (0, 0, 0, 1)
         self.darkmode = False
         Window.clearcolor = self.window_background
 
     def color_names(self):
-        return(list(self.valid_colors.keys()))
+        return list(self.valid_colors.keys())
 
     def set_to(self, name):
         self.need_redraw = True
         if name in self.valid_colors:
             self.optionbutton_background = make_rgb(self.valid_colors[name][0])
             self.optionbutton_color = make_rgb(self.valid_colors[name][1])
             self.button_background = make_rgb(self.valid_colors[name][2])
             self.button_color = make_rgb(self.valid_colors[name][3])
             self.color_scheme = name
         else:
-            return('Error: %s is not a valid color scheme.' % (name))
+            return f'Error: {name} is not a valid color scheme.'
```

### Comparing `edm-arch-1.0.27/src/edmpy/lib/constants.py` & `edm-arch-1.0.32/src/edmpy/lib/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,26 @@
+'''
+As the lib folder is shared between EDM and E5, I place here the only things that are specific to each program.
+In this way I can copy the other library code between programs without modifying it.
+'''
+
 __SPLASH_HELP__ = "\nEDM is a rewrite of the EDMWin and EDM-Mobile programs that Harold Dibble and I wrote for "
 __SPLASH_HELP__ += "using total stations on archaeological sites.  The basic idea is to provide archaeologists with "
 __SPLASH_HELP__ += "a tool that makes it easy to setup a grid on a site and piece provenience artifacts. Over time, "
 __SPLASH_HELP__ += "because of changes in hardware and operating systems, the above mentioned programs are at risk "
 __SPLASH_HELP__ += "of no longer working.\n\n"
 __SPLASH_HELP__ += "This rewrite is in Python and uses libraires designed to make it work across Windows, Linux and "
-__SPLASH_HELP__ += "MacOS.  The interface is also designed specifically for touch screens, but I am also strivin to "
+__SPLASH_HELP__ += "MacOS.  The interface is also designed specifically for touch screens, but I am also striving to "
 __SPLASH_HELP__ += "make it work well with keyboards too.  Fast, efficient and error-free are the goals.\n\n"
 __SPLASH_HELP__ += "EDM uses configuration files that let you specify what kinds of fields you want to record with "
 __SPLASH_HELP__ += "each point.  This is one of the main features of the program.  It also makes it easy to create "
 __SPLASH_HELP__ += "menus to speed data entry and reduce errors.  This new program will read the previous CFG files. "
 __SPLASH_HELP__ += "However, it will not read the previous data files.  To move data from those data files into this "
 __SPLASH_HELP__ += "program, see the instructions on the GitHub web site - https://github.com/surf3s/EDM.\n\n"
 __SPLASH_HELP__ += "This program is also open access.  My goal is to bring this tool to as many archaeologists as "
 __SPLASH_HELP__ += "possible.  If you want to help me or you need help with the program, please contact me.\n\n"
 __SPLASH_HELP__ += "Before you can start recording data points, you will need to open a previouus CFG file, create one, "
 __SPLASH_HELP__ += "or use the default one provided here (see option in File menu).  Then you will need to configure "
 __SPLASH_HELP__ += "your total station and test the connection (see options in Setup menu) or you can simulate a total station "
 __SPLASH_HELP__ += "or use manual entry."
 
-__program__ = 'EDM'
+APP_NAME = 'EDM'
```

### Comparing `edm-arch-1.0.27/src/edmpy/lib/dbs.py` & `edm-arch-1.0.32/src/edmpy/lib/dbs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 from tinydb import TinyDB, where
 from typing import Dict
 import json
 from os import path
 
 
-class dbs:
+class dbs():
 
     db = None
     filename = None
     db_name = 'data'
     table = '_default'
     new_data = {}  # type: Dict[str, bool]
 
-    def __init__(self, filename = None):
+    def __init__(self, filename = None, **kwargs):
         if filename:
             self.filename = filename
+            return self.open(self.filename)
 
     def open(self, filename = ''):
         if filename:
             self.filename = filename
-        try:
-            self.db = TinyDB(self.filename)
-            self.new_data[self.table] = True
-        except FileNotFoundError:
-            self.db = None
-            self.filename = ''
+            try:
+                self.db = TinyDB(self.filename, sort_keys = True, indent = 4, separators = (',', ': '))
+                self.new_data[self.table] = True
+                return True
+            except FileNotFoundError:
+                self.db = None
+                self.filename = ''
+        return False
 
     def valid_format(self, filename):
         try:
             if path.getsize(filename) == 0:
-                return(True)
+                return True
             with open(filename) as f:
                 json.load(f)
             return True
         except ValueError:
             return False
         except FileNotFoundError:
             return True
@@ -58,34 +61,34 @@
                     txt += "The current table is '%s'.\n" % self.table
                 else:
                     txt += 'There are no tables in this data file.\n'
             else:
                 txt += 'The data file is empty or has not been initialized.\n'
         else:
             txt = '\nA data file has not been opened.\n'
-        return(txt)
+        return txt
 
     def fields(self, tablename = ''):
         fieldnames = []
         for row in self.db.table(tablename if tablename else self.table):
             for fieldname in row.keys():
                 if fieldname not in fieldnames:
                     fieldnames.append(fieldname)
-        return(fieldnames)
+        return fieldnames
 
     def save(self, data_record):
         self.db.table(self.table).insert(data_record)
         self.new_data[self.table] = True
-        return(True)
+        return True
 
     # def __len__(self):
     #    return(len(self.db) if self.db else 0)
 
     def names(self, fieldname):
-        return([row[fieldname] for row in self.db.table(self.table)])
+        return [row[fieldname] for row in self.db.table(self.table)]
 
     def replace(self, data_record):
         pass
 
     def duplicate(self, data_record):
         pass
 
@@ -100,20 +103,20 @@
             else:
                 self.db.table(table_name).truncate()
 
     def get_unitid(self, name):
         unit, idno = name.split('-')
         p = self.db.table(self.table).search((where('unit') == unit.strip()) & (where('id') == idno.strip()))
         if p:
-            return(p)
+            return p
         else:
-            return(None)
+            return None
 
     def last_record(self):
         try:
             last = self.db.table(self.table).all()[-1]
         except (IndexError, AttributeError):
             last = None
-        return(last)
+        return last
 
     def doc_ids(self):
-        return([r.doc_id for r in self.db.table(self.table).all()])
+        return [r.doc_id for r in self.db.table(self.table).all()]
```

### Comparing `edm-arch-1.0.27/src/edmpy/lib/e5_widgets.py` & `edm-arch-1.0.32/src/edmpy/edm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,2405 +1,2405 @@
-from decimal import DivisionByZero
+"""
+EDM by Shannon McPherron
+
+  This is now beta release.  I am still working on bugs and I am still implementing some features.
+  It should be backwards compatible with EDM-Mobile and EDMWin (but there are still some issues).
+
+Changes for Version 1.0.30
+  Added and debugged Topcon stations
+  Added and debugged Leica and Leica GeoCom stations
+  Stopped program from exiting when escape is pressed
+  Fixed default locations for ini, log, and data
+  Program remembers last size and location of the screen
+  Repeat button added to measure screen
+  Flag to not prompt for prism each point added to options screen
+  Misc. prism height issues addressed
+  X box added to text boxes to help clearing values on touchscreen computers
+  Prism menu added to edit record with update of Z on prism height change
+  Improved text sizing in buttons to include word wrapping and dynamic sizing
+  Improved the default CFG and carry and increment issues
+  Fixed button font size on open dialog
+  Length checking implemented (length in CFG is enforced during data entry)
+  Prompt values (from CFG when provided) are used in Edit last record and New Record instead of the field name
+  Empty entries in MENUs are removed
+  Better error trapping of mistakes in the CFG
+  First shot on empty data table put 1 in increment fields
+  Fields shown in CFG order on delete record in gridview
+  Can do offsets in the datagrid using +-
+  Added save and revert buttons to case saving in datagrid (i.e. no longer saves immediately)
+  Basic editing shortcuts (like cntl-c etc.) work in text boxes
+
+Changes for Version 1.0.31
+  BlueTooth tested with Leica GeoCom stations
+  UI fixes
+  Tested with 1000 records in DB
+  Made JSON files better formatted so that they are more human readable
+  Made geoJSON files work with QGIS (points and lines are separate layers)
+  Substantial refactoring of Python classes and file structure
+
+Changes for Version 1.0.31
+  Fixed issue with numeric values saved as text in JSON after initial save
+  Added Help JSON to view raw data in JSON file
+
+Changes for Version 1.0.32
+  Fixing issues with GeoCom and station setup
+  
+Bugs/To Do
+  could make menus work better with keyboard (at least with tab)
+  there is no error checking on duplicates in datagrid edits
+  Do unitchecking after doing an offset shot on suffix 0 points
+  On import, integers (like Suffix) are being converted to float values
+  Good way to get random hash IDs
+  Offer to change Z when prism changes in datagrid edit cases
+  Thoroughly test unit checking
+  Thoroughly test setups (with and without prism)
+  Add home/end page up/page down and control home/control end to datagrid movement
+  *** Keeping checking edit/save issues
+  *** Program asks for save record in all points even when having saved already
+  Add move to top or bottom in Help JSON and others (like Log file)
+  Check what gets logged
+"""
+
+
+from kivy.config import Config
 from kivy.core.clipboard import Clipboard
-from kivy.clock import Clock
-from kivy.uix.textinput import TextInput
-from kivy.uix.label import Label
-from kivy.uix.scrollview import ScrollView
-from kivy.uix.tabbedpanel import TabbedPanel
-from kivy.core.window import Window
-from kivy.uix.button import Button
+from kivy.graphics import Color, Rectangle
+from kivy.app import App
+from kivy.factory import Factory
 from kivy.uix.popup import Popup
-from kivy.uix.gridlayout import GridLayout
+from kivy.uix.screenmanager import ScreenManager, Screen
 from kivy.uix.boxlayout import BoxLayout
-from kivy.uix.screenmanager import Screen
-from kivy.uix.filechooser import FileChooserListView
-from kivy.uix.recycleview import RecycleView
-from kivy.properties import ObjectProperty, NumericProperty, StringProperty, BooleanProperty
-from kivy.uix.floatlayout import FloatLayout
+from kivy.uix.spinner import Spinner
+from kivy.uix.gridlayout import GridLayout
+from kivy.properties import ObjectProperty
+from kivy.uix.label import Label
+from kivy.uix.scrollview import ScrollView
+from kivy.clock import Clock
 from kivy.uix.switch import Switch
-from kivy.uix.slider import Slider
-from kivy.uix.behaviors.focus import FocusBehavior
-from kivy.uix.spinner import Spinner, SpinnerOption
-
-from edmpy.lib.constants import __SPLASH_HELP__
-from edmpy.lib.colorscheme import ColorScheme, make_rgb, BLACK, WHITE, GOOGLE_COLORS
-from edmpy.lib.misc import platform_name, locate_file
-import ntpath
+from kivy import __version__ as __kivy_version__
+
 import os
-from shutil import copyfile
 from datetime import datetime
-from tinydb import Query, where
-import re
-
-SCROLLBAR_WIDTH = 5
-__program__ = 'EDM'
-
-
-def width_calculator(fraction_size = .8, maximum_width = 800):
-    if Window.size[0] * fraction_size > maximum_width:
-        return(maximum_width / Window.size[0])
-    else:
-        return(fraction_size)
+import csv
+from math import cos
+from math import sin
+from platform import python_version
+import logging
+from appdata import AppDataPaths
+
+# My libraries for this project
+from lib.e5_widgets import e5_label, e5_button, e5_MessageBox, e5_DatagridScreen, e5_RecordEditScreen, e5_side_by_side_buttons, e5_textinput
+from lib.e5_widgets import edm_manual, DataGridTextBox, e5_SaveDialog, e5_LoadDialog, e5_PopUpMenu, e5_MainScreen, e5_InfoScreen, e5_scrollview_label
+from lib.e5_widgets import e5_LogScreen, e5_CFGScreen, e5_INIScreen, e5_SettingsScreen, e5_scrollview_menu, DataGridMenuList, SpinnerOptions
+from lib.e5_widgets import e5_JSONScreen, DataGridLabelAndField
+from lib.colorscheme import ColorScheme
+from lib.misc import restore_window_size_position, filename_only, platform_name
+
+from geo import point, prism
+from db import DB
+from ini import INI
+from cfg import CFG
+from totalstation import totalstation
+from constants import APP_NAME
+from lib.constants import __SPLASH_HELP__
+
+# The database - pure Python
+from tinydb import TinyDB
+from tinydb import __version__ as __tinydb_version__
+
+# from plyer import gps
+# from plyer import __version__ as __plyer_version__
+
+# from plyer import __version__ as __plyer_version__
+__plyer_version__ = 'None'
+
+from angles import d2r
+
+import serial
+import requests
+import serial.tools.list_ports_windows
+
+"""
+The explicit mention of this package here
+triggers its inclusions in the pyinstaller spec file.
+It is needed for the filechooser widget.
+The TimeZoneInfo is just to avoid a flake8 error.
+"""
+try:
+    import win32timezone
+    win32timezone.TimeZoneInfo.local()
+except ModuleNotFoundError:
+    pass
+
+VERSION = '1.0.32'
+PRODUCTION_DATE = 'May, 2023'
+__DEFAULT_FIELDS__ = ['X', 'Y', 'Z', 'SLOPED', 'VANGLE', 'HANGLE', 'STATIONX', 'STATIONY', 'STATIONZ', 'LOCALX', 'LOCALY', 'LOCALZ', 'DATE', 'PRISM', 'ID']
+__BUTTONS__ = 13
+__LASTCOMPORT__ = 16
+MAX_SCREEN_WIDTH = 400
 
 
-def height_calculator(desired_size):
-    ratio = desired_size / Window.size[1]
-    if ratio > .9:
-        ratio = .9
-    return(ratio)
+class MainScreen(e5_MainScreen):
 
+    event = None
 
-def set_color(popup, colors):
-    if not popup:
-        return(colors.text_color if colors else make_rgb(BLACK))
-    else:
-        return(colors.popup_text_color if colors else make_rgb(WHITE))
-
-
-class SpinnerOptions(SpinnerOption):
     def __init__(self, **kwargs):
-        super(SpinnerOptions, self).__init__(**kwargs)
-
-
-class e5_PopUpMenu(Popup):
-    def __init__(self, title, menu_list, message = '', menu_selected = '', call_back = None, colors = None, **kwargs):
-        super(e5_PopUpMenu, self).__init__(**kwargs)
-
-        pop_content = GridLayout(cols = 1, size_hint_y = 1, spacing = 5, padding = 5)
-
-        ncols = int(Window.width / 200)
-        if ncols < 1:
-            ncols = 1
-
-        if message:
-            label = e5_scrollview_label(message, popup = True, colors = colors)
-            label.size_hint = (1, .2)
-            pop_content.add_widget(label)
-
-        menu = e5_scrollview_menu(menu_list, menu_selected,
-                                                 widget_id = 'menu',
-                                                 call_back = [call_back],
-                                                 ncols = ncols,
-                                                 colors = colors)
-        pop_content.add_widget(menu)
-        menu.make_scroll_menu_item_visible()
+        super(MainScreen, self).__init__(**kwargs)
 
-        pop_content.add_widget(e5_button('Back', selected = True,
-                                                 call_back = self.dismiss,
-                                                 colors = colors))
-
-        self.content = pop_content
-        self.title = title
-        self.size_hint = (.9, .9)
-        self.auto_dismiss = True
+        self.setup_logger()
 
+        self.colors = ColorScheme()
+        self.ini = INI()
+        self.cfg = CFG()
+        self.data = DB()
+
+        self.warnings, self.errors = self.setup_program()
+
+        self.station = totalstation(self.ini.get_value(APP_NAME, 'STATION'))
+        self.station.setup(self.ini, self.data)
+        self.station.open()
+        if self.station.error_message:
+            self.warnings.append(self.station.error_message)
+
+        self.cfg_datums = CFG()
+        self.cfg_datums.build_datum()
+        self.cfg_prisms = CFG()
+        self.cfg_prisms.build_prism()
+        self.cfg_units = CFG()
+        self.cfg_units.build_unit()
+
+        self.layout = BoxLayout(orientation = 'vertical',
+                                size_hint_y = .9,
+                                size_hint_x = .8,
+                                pos_hint={'center_x': .5},
+                                padding = 20,
+                                spacing = 20)
+        self.build_mainscreen()
+        self.add_widget(self.layout)
+        self.add_screens()
+        restore_window_size_position(APP_NAME, self.ini)
 
-class db_filter(Popup):
+    def on_enter(self, *args):
+        if self.warnings or self.errors:
+            self.popup = self.warnings_and_errors_popup(self.warnings, self.errors)
+            self.popup.open()
+            self.errors, self.warnings = [], []
+        elif self.ini.first_time:
+            self.popup = e5_MessageBox('Welcome to EDM', __SPLASH_HELP__)
+            self.popup.open()
+            self.ini.first_time = False
+        self.update_info_label()
 
-    def __init__(self, default_field = '', fields = [], call_back = None, colors = None, **kwargs):
-        super(db_filter, self).__init__(**kwargs)
+    def setup_logger(self):
+        logger = logging.getLogger(__name__)
+        logger.setLevel(logging.INFO)
+        formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s', datefmt = '%Y-%m-%d %H:%M:%S')
+        fh = logging.FileHandler(self.app_paths.log_file_path)
+        fh.setLevel(logging.INFO)
+        fh.setFormatter(formatter)
+        logger.addHandler(fh)
+        logger.info(APP_NAME + ' started, logger initialized, and application built.')
+
+    def add_screens(self):
+        sm.add_widget(EditLastRecordScreen(name = 'EditLastRecordScreen',
+                                            colors = self.colors,
+                                            data = self.data,
+                                            doc_id = None,
+                                            e5_cfg = self.cfg))
+
+        sm.add_widget(VerifyStationScreen(name = 'VerifyStationScreen',
+                                            id = 'verify_station',
+                                            data = self.data,
+                                            station = self.station,
+                                            colors = self.colors,
+                                            ini = self.ini))
+
+        sm.add_widget(RecordDatumsScreen(name = 'RecordDatumsScreen',
+                                            data = self.data,
+                                            station = self.station,
+                                            colors = self.colors,
+                                            ini = self.ini))
+
+        sm.add_widget(EditPointScreen(name = 'EditPointScreen',
+                                            colors = self.colors,
+                                            data = self.data,
+                                            # data_table = self.data.table,
+                                            doc_id = None,
+                                            e5_cfg = self.cfg,
+                                            one_record_only = True))
+
+        sm.add_widget(EditPointsScreen(name = 'EditPointsScreen',
+                                            colors = self.colors,
+                                            main_data = self.data,
+                                            main_tablename = self.data.table,
+                                            main_cfg = self.cfg))
+
+        sm.add_widget(EditPointsScreen(name = 'EditDatumsScreen',
+                                            colors = self.colors,
+                                            main_data = self.data,
+                                            main_tablename = 'datums',
+                                            main_cfg = self.cfg_datums,
+                                            addnew = True))
+
+        sm.add_widget(EditPointsScreen(name = 'EditPrismsScreen',
+                                            colors = self.colors,
+                                            main_data = self.data,
+                                            main_tablename = 'prisms',
+                                            main_cfg = self.cfg_prisms,
+                                            addnew = True))
+
+        sm.add_widget(EditPointsScreen(name = 'EditUnitsScreen',
+                                            colors = self.colors,
+                                            main_data = self.data,
+                                            main_tablename = 'units',
+                                            main_cfg = self.cfg_units,
+                                            addnew = True))
+
+        sm.add_widget(StatusScreen(name = 'StatusScreen',
+                                            colors = self.colors,
+                                            cfg = self.cfg,
+                                            ini = self.ini,
+                                            data = self.data,
+                                            station = self.station))
+
+        sm.add_widget(e5_LogScreen(name = 'LogScreen', colors = self.colors, logger = logging.getLogger(__name__)))
+
+        sm.add_widget(e5_CFGScreen(name = 'CFGScreen', colors = self.colors, cfg = self.cfg))
+
+        sm.add_widget(e5_INIScreen(name = 'INIScreen', colors = self.colors, ini = self.ini))
+
+        sm.add_widget(e5_JSONScreen(name = 'JSONScreen', colors = self.colors, data = self.data))
+
+        sm.add_widget(AboutScreen(name = 'AboutScreen', colors = self.colors))
+
+        sm.add_widget(StationConfigurationScreen(name = 'StationConfigurationScreen',
+                                                    station = self.station,
+                                                    ini = self.ini,
+                                                    colors = self.colors))
 
-        spinner_dropdown_button = SpinnerOptions
-        spinner_dropdown_button.font_size = colors.button_font_size.replace("sp", '') if colors.button_font_size else None
-        spinner_dropdown_button.background_color = (0, 0, 0, 1)
+        sm.add_widget(InitializeStationScreen(name = 'InitializeStationScreen',
+                                                    data = self.data,
+                                                    station = self.station,
+                                                    ini = self.ini,
+                                                    colors = self.colors))
 
-        pop_content = GridLayout(cols = 1, spacing = 5, padding = 5)
-        field_value = GridLayout(cols = 2, spacing = 5, padding = 5)
-        self.fields_dropdown = Spinner(text = default_field, values = fields,
-                                        size_hint = (.5, None),
-                                        option_cls = spinner_dropdown_button)
-        field_value.add_widget(self.fields_dropdown)
-        field_value_right = GridLayout(cols = 1, spacing = 5, padding = 5)
-        field_value_right.add_widget(e5_label('Select a field and enter a\nvalue to match in this field.', size_hint = (1, .2), halign = 'left', popup = True))
-        self.value_input = e5_textinput(size_hint = (0.75, None), id = 'value', write_tab = False)
-        self.value_input.bind(minimum_height = self.value_input.setter('height'))
-        field_value_right.add_widget(self.value_input)
-        field_value.add_widget(field_value_right)
-        pop_content.add_widget(field_value)
-        buttons = e5_side_by_side_buttons(text = ['Back', 'Apply'],
-                                            button_height = None,
-                                            id = ['back', 'apply'],
-                                            selected = [True, True],
-                                            call_back = [self.dismiss, call_back],
-                                            colors = colors)
-        pop_content.add_widget(buttons)
-        self.content = pop_content
-        self.title = 'Filter dataset'
-        self.size_hint = (.9, .38)
-
-
-class edm_manual(Popup):
-
-    def __init__(self, type = "Manual XYZ", call_back = None, colors = None, **kwargs):
-        super(edm_manual, self).__init__(**kwargs)
-
-        pop_content = GridLayout(cols = 1, spacing = 5, padding = 5)
-        if type == "Manual XYZ":
-            input = DataGridLabelAndField(col = 'X', colors = colors, popup = True)
-            input.txt.bind(on_text_validate = self.next_field)
-            self.xcoord = input.txt
-            pop_content.add_widget(input)
-            input = DataGridLabelAndField(col = 'Y', colors = colors, popup = True)
-            input.txt.bind(on_text_validate = self.next_field)
-            self.ycoord = input.txt
-            pop_content.add_widget(input)
-            input = DataGridLabelAndField(col = 'Z', colors = colors, popup = True)
-            input.txt.bind(on_text_validate = self.next_field)
-            self.zcoord = input.txt
-            pop_content.add_widget(input)
-            self.hangle = None
-            self.vangle = None
-            self.sloped = None
-        else:
-            input = DataGridLabelAndField(col = 'Horizontal angle', colors = colors, popup = True)
-            input.txt.bind(on_text_validate = self.next_field)
-            self.hangle = input.txt
-            pop_content.add_widget(input)
-            input = DataGridLabelAndField(col = 'Vertical angle', colors = colors, popup = True)
-            input.txt.bind(on_text_validate = self.next_field)
-            self.vangle = input.txt
-            pop_content.add_widget(input)
-            input = DataGridLabelAndField(col = 'Slope distance', colors = colors, popup = True)
-            input.txt.bind(on_text_validate = self.next_field)
-            self.sloped = input.txt
-            pop_content.add_widget(input)
-            self.xcoord = None
-            self.ycoord = None
-            self.zcoord = None
-        buttons = e5_side_by_side_buttons(text = ['Cancel', 'Next'],
-                                            button_height = None,
-                                            id = ['cancel', 'next'],
-                                            selected = [True, True],
-                                            call_back = [self.dismiss, call_back],
-                                            colors = colors)
-        self.call_back = call_back
-        pop_content.add_widget(buttons)
-        self.content = pop_content
-        self.title = 'Manual Input'
-        self.size_hint = (.9, height_calculator(280))
-        self.auto_dismiss = True
-
-    def on_open(self):
-        if self.xcoord is not None:
-            self.xcoord.focus = True
-        elif self.hangle is not None:
-            self.hangle.focus = True
-
-    def next_field(self, instance):
-        if instance.id in ['Slope distance', 'Z']:
-            self.call_back(instance)
-        instance.get_focus_next().focus = True
+        sm.add_widget(e5_SettingsScreen(name = 'EDMSettingsScreen',
+                                        colors = self.colors,
+                                        ini = self.ini,
+                                        cfg = self.cfg))
 
+        sm.add_widget(ComTestScreen(name = 'ComTestScreen',
+                                        colors = self.colors,
+                                        station = self.station,
+                                        cfg = self.cfg))
 
-class e5_textinput(TextInput):
-    id = ObjectProperty('')
+        sm.add_widget(OptionsScreen(name = 'OptionsScreen',
+                                        colors = self.colors,
+                                        station = self.station,
+                                        cfg = self.cfg))
 
-    def __init__(self, **kwargs):
-        super(e5_textinput, self).__init__(**kwargs)
-        if 'id' in kwargs:
-            self.id = kwargs.get('id')
-            if self.id in ['X', 'Y', 'Z'] and __program__ == 'EDM':
-                self.bind(on_text_validate = self.do_coordinate_math)
+    def reset_screens(self):
+        for screen in sm.screens[:]:
+            if screen.name != 'MainScreen':
+                sm.remove_widget(screen)
+        self.add_screens()
 
-    def do_coordinate_math(self, instance):
-        if instance.text:
-            try:
-                self.text = str(eval(instance.text))
-            except (DivisionByZero, NameError):
-                pass
+    def build_mainscreen(self):
 
+        if platform_name() == 'Android':
+            size_hints = {'info': .13,
+                            'option_buttons': .8 - .13 - .2,
+                            'shot_buttons': .2}
+        else:
+            size_hints = {'info': .13,
+                            'option_buttons': .8 - .13 - .2,
+                            'shot_buttons': .2}
+
+        self.layout.clear_widgets()
+
+        self.info = e5_label(text = 'EDM',
+                                size_hint = (1, size_hints['info']),
+                                color = self.colors.text_color,
+                                id = 'lastshot',
+                                halign = 'center')
+        if self.colors:
+            if self.colors.text_font_size:
+                self.info.font_size = self.colors.text_font_size
+        self.layout.add_widget(self.info)
+        self.info.bind(texture_size = self.info.setter('size'))
+        self.info.bind(size_hint_min_x = self.info.setter('width'))
+
+        # grid = GridLayout(cols = 3, spacing = 10)
+        scroll_content = BoxLayout(orientation = 'horizontal',
+                                    size_hint = (1, size_hints['option_buttons']),
+                                    spacing = 20)
+        self.layout.add_widget(scroll_content)
+
+        button_count = 0
+        button_text = []
+        button_selected = []
+        for button_no in range(1, __BUTTONS__):
+            title = self.cfg.get_value(f'BUTTON{button_no}', 'TITLE')
+            if title:
+                button_text.append(title)
+                button_selected.append(False)
+                button_count += 1
+
+        if button_count > 0:
+            self.scroll_menu = e5_scrollview_menu(button_text,
+                                                        menu_selected = button_selected,
+                                                        widget_id = 'buttons',
+                                                        call_back = [self.take_shot],
+                                                        ncols = 3,
+                                                        colors = self.colors)
+            scroll_content.add_widget(self.scroll_menu)
+
+        # if button_count % 3 !=0:
+        #    button_empty = Button(text = '', size_hint_y = None, id = '',
+        #                    color = self.colors.window_background,
+        #                    background_color = self.colors.window_background,
+        #                    background_normal = '')
+        #    scroll_content.add_widget(button_empty)
+
+        # if button_count % 3 == 2:
+        #    scroll_content.add_widget(button_empty)
+
+        # self.layout.add_widget(scroll_content)
+
+        shot_buttons = GridLayout(cols = 3, size_hint = (1, size_hints['shot_buttons']), spacing = 20)
+
+        shot_buttons.add_widget(e5_button(text = 'Record', id = 'record',
+                                            colors = self.colors, call_back = self.take_shot, selected = True))
+
+        shot_buttons.add_widget(e5_button(text = 'Continue', id = 'continue',
+                                            colors = self.colors, call_back = self.take_shot, selected = True))
+
+        self.measure_button = e5_button(text = 'Measure', id = 'measure',
+                                            colors = self.colors, call_back = self.take_shot, selected = True)
+        shot_buttons.add_widget(self.measure_button)
+
+        self.layout.add_widget(shot_buttons)
+
+        self.update_title()
+
+        # if self.cfg.filename:
+        #     if self.cfg.has_warnings or self.cfg.has_errors:
+        #         self.event = Clock.schedule_once(self.show_popup_message, 1)
 
-class e5_label(Label):
-    id = ObjectProperty('')
+    def update_title(self):
+        for widget in self.walk():
+            if hasattr(widget, 'action_previous'):
+                widget.action_previous.title = 'EDM'
+                if self.cfg is not None:
+                    if self.cfg.filename:
+                        widget.action_previous.title = filename_only(self.cfg.filename)
+
+    def message_open_cfg_first(self):
+        message = '\nBefore you can do this, you need to open a CFG file (see option under File menu).  Opening a CFG file will also open your database. '
+        message += 'If you do not have a CFG file already, you can use a default one (see option under File menu).  Later you can alter the default CFG to '
+        message += 'add additional options specific to your work.'
+        return e5_MessageBox('EDM', message)
+
+    def ready_to_use(self):
+        return self.cfg is not None and self.data.filename != ''
+
+    def take_shot(self, instance):
+        if not self.ready_to_use() and instance.id != 'measure':
+            self.popup = self.message_open_cfg_first()
+            self.popup.open()
+            return
 
-    def __init__(self, text, popup = False, colors = None, **kwargs):
-        super(e5_label, self).__init__(**kwargs)
-        self.text = text
-        self.color = set_color(popup, colors)
-        if colors:
-            if colors.text_font_size:
-                self.font_size = colors.text_font_size
-
-
-class e5_label_wrapped(e5_label):
-    def __init__(self, text, popup = False, colors = None, **kwargs):
-        super(e5_label_wrapped, self).__init__(text, popup = False, colors = None, **kwargs)
-        self.size_hint = (1, None)
-        self.bind(width=lambda *x: self.setter('text_size')(self, (self.width, None)),
-                                texture_size=lambda *x: self.setter('height')(self, self.texture_size[1]))
-
-
-class e5_side_by_side_buttons(GridLayout):
-    def __init__(self, text,
-                    id = ['', ''], selected = [False, False],
-                    call_back = [None, None], button_height = None, colors = None, **kwargs):
-        super(e5_side_by_side_buttons, self).__init__(**kwargs)
-        self.cols = len(id)
-        self.spacing = 5
-        self.size_hint_y = button_height
-        # self.height = button_height
-        for i in range(len(id)):
-            self.add_widget(e5_button(text[i],
-                            id = id[i],
-                            selected = selected[i], call_back = call_back[i],
-                            button_height = button_height, colors = colors))
-
-
-class e5_button(FocusBehavior, Button):
-    id = ObjectProperty('')
-
-    def __init__(self, text,
-                    id = '',
-                    selected = False, call_back = None, on_focus = None,
-                    button_height = None, colors = None, **kwargs):
-        super(e5_button, self).__init__(**kwargs)
-        self.colors = colors
-        self.text = text
-        self.size_hint_y = button_height
-        self.id = id
-        if colors:
-            if colors.button_font_size:
-                self.font_size = colors.button_font_size
-        self.color = colors.button_color if colors else make_rgb(WHITE)
-        if colors:
-            self.background_color = colors.button_background if selected else colors.optionbutton_background
+        self.station.shot_type = instance.id
+        self.station.clear_xyz()
+        if self.station.make == 'Microscribe':
+            self.popup = DataGridTextBox(title = 'EDM', text = '<Microscribe>',
+                                            label = 'Waiting on...',
+                                            button_text = ['Cancel', 'Next'],
+                                            call_back = self.have_shot,
+                                            colors = self.colors)
+            self.popup.open()
+        elif self.station.make in ['Manual XYZ', 'Manual VHD']:
+            self.popup = edm_manual(type = self.station.make, call_back = self.have_shot_manual, colors = self.colors)
+            self.popup.open()
         else:
-            self.background_color = make_rgb(GOOGLE_COLORS['light blue'][2 if selected else 0])
-        if call_back:
-            self.bind(on_press = call_back)
-        self.background_normal = ''
-        self.call_back = call_back
-
-    def on_focus(self, instance, value, *largs):
-        if self.background_color and self.colors:
-            self.background_color = self.colors.button_background if self.focus else self.colors.optionbutton_background
-
-
-class e5_scrollview_menu(ScrollView):
-    id = ObjectProperty(None)
-    scrollbox = ObjectProperty(None)
-    menu_selected_widget = None
-
-    def __init__(self, menu_list, menu_selected, widget_id = '', call_back = [None], ncols = 1, colors = None, **kwargs):
-        super(e5_scrollview_menu, self).__init__(**kwargs)
-        self.colors = colors
-        self.scrollbox = GridLayout(cols = ncols,
-                                    size_hint_y = None,
-                                    spacing = 5)
-        self.scrollbox.bind(minimum_height = self.scrollbox.setter('height'))
-
-        self.menu_selected_widget = None
-        if menu_list:
-            if len(call_back) == 1:
-                call_back = call_back * len(menu_list)
-            for menu_item in menu_list:
-                menu_button = e5_button(menu_item, menu_item,
-                                        selected = (menu_item == menu_selected),
-                                        call_back = call_back[menu_list.index(menu_item)], colors = colors)
-                self.scrollbox.add_widget(menu_button)
-                if menu_item == menu_selected:
-                    self.menu_selected_widget = menu_button
-        else:
-            self.scrollbox.add_widget(Button(text = '',
-                                             background_normal = ''))
-        self.size_hint = (1, 1)
-        self.id = widget_id + '_scroll'
-        self.add_widget(self.scrollbox)
-
-    def scroll_menu_clear_selected(self):
-        if self.menu_selected_widget:
-            self.menu_selected_widget.background_color = self.colors.optionbutton_background
-            self.menu_selected_widget = None
-
-    def scroll_menu_get_selected(self):
-        return(self.menu_selected_widget)
-
-    def scroll_menu_set_selected(self, text):
-        self.scroll_menu_clear_selected()
-        for widget in self.scrollbox.children:
-            if widget.text == text:
-                widget.background_color = self.colors.button_background
-                self.menu_selected_widget = widget
-                break
-
-    def scroll_menu_list(self):
-        menu_list = []
-        for widget in self.scrollbox.children:
-            menu_list.append(widget.text)
-        menu_list.reverse()
-        return(menu_list)
-        # return([widget.text for widget in self.scroll_menu.children])
-
-    def make_scroll_menu_item_visible(self):
-        if self.menu_selected_widget is not None:
-            self.scroll_to(self.menu_selected_widget)
-
-    def move_scroll_menu_item(self, ascii_code):
-        menu_list = self.scroll_menu_list()
-        if self.menu_selected_widget is not None:
-            index_no = menu_list.index(self.menu_selected_widget.text)
-        else:
-            index_no = 0
-
-        if index_no >= 0:
-            new_index = -1
-            if ascii_code == 279:
-                new_index = len(menu_list) - 1
-            elif ascii_code == 278:
-                new_index = 0
-            elif ascii_code == 273:  # Up
-                new_index = max([index_no - self.children[0].cols, 0])
-            elif ascii_code == 276:
-                new_index = max([index_no - 1, 0])
-            elif ascii_code == 274:  # Down
-                new_index = min([index_no + self.children[0].cols, len(menu_list) - 1])
-            elif ascii_code == 275:
-                new_index = min([index_no + 1, len(menu_list) - 1])
-            if new_index >= 0:
-                self.scroll_menu_set_selected(menu_list[new_index])
-                self.make_scroll_menu_item_visible()
-                # if self.get_widget_by_id('field_data'):
-                #    self.get_widget_by_id('field_data').text = menu_list[new_index]
-
-    def scroll_menu_char_match(self, match_str):
-        menu_list = self.scroll_menu_list()
-        if menu_list:
-            index_no = menu_list.index(self.scroll_menu_get_selected().text)
-
-            new_index = (index_no + 1) % len(menu_list)
-            while not new_index == index_no:
-                if menu_list[new_index].upper()[0] == match_str.upper():
-                    self.scroll_menu_set_selected(menu_list[new_index])
-                    self.make_scroll_menu_item_visible()
-                    break
-                else:
-                    new_index = (new_index + 1) % len(menu_list)
-                    # need new logic to auto select when only one case is available
-
-
-class e5_scrollview_label(ScrollView):
-    id = ObjectProperty(None)
-
-    def __init__(self, text, widget_id = '', popup = False, colors = None, **kwargs):
-        super(e5_scrollview_label, self).__init__(**kwargs)
-        self.colors = colors if colors else ColorScheme()
-        self.text = text
-        scrollbox = GridLayout(cols = 1,
-                                size_hint_y = None,
-                                spacing = 5)
-        scrollbox.bind(minimum_height = scrollbox.setter('height'))
-
-        self.scrolling_label = e5_label(text = self.text, markup = True,
-                                        size_hint_y = None,
-                                        color = self.colors.text_color if not popup else self.colors.popup_text_color,
-                                        id = widget_id + '_label', popup = popup,
-                                        text_size = (self.width, None))
-        if colors is not None:
-            if colors.text_font_size:
-                self.scrolling_label.font_size = colors.text_font_size
-
-        self.scrolling_label.bind(texture_size=lambda instance, value: setattr(instance, 'height', value[1]))
-        self.scrolling_label.bind(width=lambda instance, value: setattr(instance, 'text_size', (value * .95, None)))
-
-        # info.bind(texture_size=lambda *x: info.setter('height')(info, info.texture_size[1]))
-        scrollbox.add_widget(self.scrolling_label)
-
-        self.bar_width = SCROLLBAR_WIDTH
-        self.size_hint = (1, 1)
-        self.id = widget_id + '_scroll'
-        self.add_widget(scrollbox)
-
-
-class e5_MainScreen(Screen):
-
-    popup = ObjectProperty(None)
-    popup_open = False
-    event = ObjectProperty(None)
-    widget_with_focus = ObjectProperty(None)
-    text_color = (0, 0, 0, 1)
-
-    def setup_program(self):
-        warnings, errors = [], []
-        self.ini.open(os.path.join(self.user_data_dir, __program__ + '.ini'))
-        if not self.ini.first_time:
-            if self.ini.get_value(__program__, 'ColorScheme'):
-                self.colors.set_to(self.ini.get_value(__program__, 'ColorScheme'))
-            if self.ini.get_value(__program__, 'DarkMode').upper() == 'TRUE':
-                self.colors.darkmode = True
+            self.station.take_shot()
+            if self.station.prism_prompt:
+                self.popup = self.get_prism_height()
+                self.popup.open()
             else:
-                self.colors.darkmode = False
+                self.have_shot(instance)
 
-            if self.ini.get_value(__program__, 'ButtonFontSize'):
-                self.colors.button_font_size = (self.ini.get_value(__program__, 'ButtonFontSize'))
-            if self.ini.get_value(__program__, 'TextFontSize'):
-                self.colors.text_font_size = (self.ini.get_value(__program__, 'TextFontSize'))
-
-            if self.ini.get_value(__program__, "CFG"):
-                self.cfg.open(self.ini.get_value(__program__, "CFG"))
-                if self.cfg.filename:
-                    warnings, errors = self.open_db()
-            self.ini.update(self.colors, self.cfg)
-            self.ini.save()
-        self.colors.set_colormode()
-        self.colors.need_redraw = False
-        self.ini.update_value(__program__, 'APP_PATH', os.path.abspath(os.path.dirname(__file__)) if platform_name() == 'Windows' else self.user_data_dir)
-        return(warnings, errors)
-
-    def get_path(self):
-        if self.ini.get_value(__program__, "CFG"):
-            return(ntpath.split(self.ini.get_value(__program__, "CFG"))[0])
-        else:
-            return(os.getcwd())
-
-    def get_files(self, fpath, exts = None):
-        files = []
-        for (dirpath, dirnames, filenames) in os.walk(fpath):
-            files.extend(filenames)
-            break
-        if exts:
-            return([filename for filename in files if filename.upper().endswith(exts.upper())])
-        else:
-            return(files)
-
-    def open_db(self):
-        warnings = []
-        errors = []
-        database = locate_file(self.cfg.get_value(__program__, 'DATABASE'), self.cfg.path)
-        if not database:
-            database = os.path.split(self.cfg.filename)[1]
-            if "." in database:
-                database = database.split('.')[0]
-            database = os.path.join(self.cfg.path, database + '.json')
-            warning = f"Could not locate the data file {self.cfg.get_value(__program__, 'DATABASE')} as specified in the CFG file.  EDM looked in the specified location and also in "
-            warning += f"in the same folder as the CFG file {self.cfg.path}.  A new empty data file was created as {database}.  If this is not correct, leave the program and alter the CFG file "
-            warning += "and/or move the data file to the correct location."
-            warnings.append(warning)
-        if database.lower().endswith('.mdb') or database.lower().endswith('.sdf'):
-            database = database[:-4] + '.json'
-            warning = 'EDM does not accept the mdb and sdf data files that were used with EDMWin and EDM-Mobile.  A new, empty json format file has been opened in this case.  '
-            warning += f'The filename is {database}.  '
-            warning += 'JSON files are human readable ASCII files.  To move your data from the old format to this program, follow the directions found on the EDM GitHub site '
-            warning += 'https://github.com/surf3s/EDM/tree/master/Import_from_EDM-Mobile or https://github.com/surf3s/EDM/tree/master/Import_from_EDMWin.  Basically you need to '
-            warning += 'create csv files that can be imported into this program.  EDM-Mobile will create them for you.  With EDMWin you need to create them youself.  '
-            warning += 'Alternatively, you can hand enter items like datums, units, and prisms using the various menu options under Edit.'
-            warnings.append(warning)
-        if not self.data.valid_format(database):
-            error = f'The file {database} does not load as a valid json file.  If the wrong file has been loaded, edit the CFG file to point to the correct database.  If the file is '
-            error += 'the correct one, then it appears that it has become corrupted.  Open the file in any text editor and assess the situation.  A json file is a human readable '
-            error += 'file format, and you should be able to see your data.  If you need more help fixing the problem, you can contact me.'
-            errors.append(error)
-        else:
-            self.data.open(database)
-            if self.cfg.get_value(__program__, 'TABLE'):
-                self.data.table = self.cfg.get_value(__program__, 'TABLE')
+    def have_shot_manual(self, instance):
+        # check that next was pressed and get values
+        if self.popup.xcoord and self.popup.ycoord and self.popup.zcoord:
+            p = self.station.text_to_point(f'{self.popup.xcoord.textbox.text},{self.popup.ycoord.textbox.text},{self.popup.zcoord.textbox.text}')
+            if p:
+                self.station.xyz = p
+                self.station.make_global()
+                self.station.vhd_from_xyz()
+        elif self.popup.hangle and self.popup.vangle and self.popup.sloped:
+            try:
+                self.station.hangle = float(self.popup.hangle.text)
+                self.station.vangle = float(self.popup.vangle.text)
+                self.station.sloped = float(self.popup.sloped.text)
+            except ValueError:
+                self.station.xyz = point()
+            self.station.vhd_to_xyz()
+            self.station.make_global()
+        self.station.pnt = None
+        self.popup.dismiss()
+        if self.station.xyz.x is None or self.station.xyz.y is None or self.station.xyz.z is None:
+            self.popup = e5_MessageBox('Recording error', '\nInvalid value(s) were given.  Point not recorded.', call_back = self.close_popup)
+            self.popup.open()
+            self.popup_open = True
+        else:
+            if self.station.prism_prompt:
+                self.popup = self.get_prism_height()
+                self.popup.open()
+                self.popup_open = True
             else:
-                self.data.table = '_default'
-            self.cfg.update_value(__program__, 'DATABASE', self.data.filename)
-            self.cfg.update_value(__program__, 'TABLE', self.data.table)
-            self.cfg.save()
-            self.data.new_data[self.data.table] = True
-        return((warnings, errors))
-
-    def warnings_and_errors_popup(self, warnings, errors):
-        message_txt = '\n'
-        message_txt += ',\n\n'.join(['Warning: ' + warning for warning in warnings])
-        message_txt += ',\n\n'.join(['Error: ' + error for error in errors])
-        return(e5_MessageBox('Warnings and errors', message_txt, colors = self.colors))
-
-    def show_popup_message(self, dt):
-        self.event.cancel()
-        if self.cfg.has_errors or self.cfg.has_warnings:
-            if self.cfg.has_errors:
-                message_text = '\nThe following errors were found in the configuration file %s and must be corrected before data entry can begin.\n\n' % self.cfg.filename
-                self.cfg.filename = ''
-                title = 'CFG File Errors'
-            elif self.cfg.has_warnings:
-                self.cfg.has_warnings = False
-                message_text = '\nThough data collection can start, there are the following warnings in the configuration file %s.\n\n' % self.cfg.filename
-                title = 'Warnings'
-            message_text = message_text + '\n\n'.join(self.cfg.errors)
-        else:
-            title = __program__
-            message_text = __SPLASH_HELP__
-        self.popup = e5_MessageBox(title, message_text, call_back = self.close_popup, colors = self.colors)
-        self.popup.open()
-        self.popup_open = True
+                self.have_shot(instance)
 
-    def get_widget_by_id(self, id):
-        for widget in self.walk():
-            if hasattr(widget, 'id'):
-                if widget.id == id:
-                    return(widget)
-        return(None)
-
-    def get_info(self):
-        if self.cfg.current_field.infofile:
-            fname = os.path.join(self.cfg.path, self.cfg.current_field.infofile)
-            if os.path.exists(fname):
-                try:
-                    with open(fname, 'r') as f:
-                        return(f.read())
-                except OSError:
-                    return('Could not open file %s.' % fname)
-            else:
-                return('The file %s does not exist.' % fname)
+    def get_prism_height(self):
+        prism_names = self.data.names('prisms')
+        if len(prism_names) > 0:
+            return DataGridMenuList(title = "Select or Enter a Prism Height",
+                                            menu_list = prism_names,
+                                            menu_selected = self.station.prism.name,
+                                            call_back = self.have_shot,
+                                            colors = self.colors)
         else:
-            return(self.cfg.current_field.info)
-
-    def save_window_location(self):
-        self.ini.update_value(__program__, 'ScreenTop', Window.top)
-        self.ini.update_value(__program__, 'ScreenLeft', Window.left)
-        self.ini.update_value(__program__, 'ScreenWidth', Window.size[0])
-        self.ini.update_value(__program__, 'ScreenHeight', Window.size[1])
-        self.ini.save()
-
-    def open_popup(self):
-        self.popup_open = False
-        self.popup.open()
-
-    def dismiss_popup(self, *args):
-        self.popup_open = False
-        if self.popup:
-            self.popup.dismiss()
-        if self.parent:
-            self.parent.current = 'MainScreen'
+            return DataGridTextBox(title = 'Enter a Prism Height',
+                                        text = str(self.station.prism.height) if self.station.prism.height else '0',
+                                        call_back = self.have_shot,
+                                        button_text = ['Back', 'Next'],
+                                        colors = self.colors)
 
-    def save_record(self):
-        valid = self.cfg.validate_current_record()
-        if valid:
-            if self.data.save(self.cfg.current_record):
-                self.make_backup()
+    def have_shot(self, instance):
+        if self.station.make == 'Microscribe':
+            result = self.popup.result
+            if result:
+                p = self.station.text_to_point(result)
+                if p:
+                    self.station.xyz = self.station.mm_to_meters(p)
+                    self.station.make_global()
+        else:
+            if self.station.prism_prompt:
+                prism_name = instance.text
+                if prism_name == 'Add' or prism_name == 'Next':
+                    try:
+                        self.station.prism = prism(None, float(self.popup.txt.textbox.text), None)
+                    except ValueError:
+                        self.station.prism = prism()
+                else:
+                    self.station.prism = self.data.get_prism(prism_name)
             else:
-                pass
-        else:
-            self.popup = e5_MessageBox('Save Error', valid, call_back = self.close_popup, colors = self.colors)
-            self.popup.open()
-            self.popup_open = True
-
-    def make_backup(self):
-        if self.ini.backup_interval > 0:
-            try:
-                record_counter = int(self.cfg.get_value(__program__, 'RECORDS UNTIL BACKUP')) if self.cfg.get_value(__program__, 'RECORDS UNTIL BACKUP') else self.ini.backup_interval
-                record_counter -= 1
-                if record_counter <= 0:
-                    backup_path, backup_file = os.path.split(self.data.filename)
-                    backup_file, backup_file_ext = backup_file.split('.')
-                    backup_file += self.datetime_stamp() if self.ini.incremental_backups else '_backup'
-                    backup_file += "." + backup_file_ext
-                    backup_file = os.path.join(backup_path, backup_file)
-                    copyfile(self.data.filename, backup_file)
-                    record_counter = self.ini.backup_interval
-                self.cfg.update_value(__program__, 'RECORDS UNTIL BACKUP', str(record_counter))
-            except OSError:
-                self.popup = e5_MessageBox('Backup Error', "\nAn error occurred while attempting to make a backup.  Check the backup settings and that the disk has enough space for a backup.",
-                                            call_back = self.close_popup, colors = self.colors)
+                self.station.prism = prism(None, 0.0, None)
+            if self.station.prism.height is None:
+                self.popup.dismiss()
+                self.popup = e5_MessageBox('Error', '\nInvalid prism height provided.  Shot not recorded.', call_back = self.close_popup)
                 self.popup.open()
                 self.popup_open = True
+                return
+            if self.station.make in ['Manual XYZ', 'Manual VHD', 'Simulate']:
+                self.station.prism_adjust()
+        if self.popup:
+            self.popup.dismiss()
 
-    def date_stamp(self):
-        date_stamp = '%s' % datetime.now().replace(microsecond=0)
-        date_stamp = date_stamp.split(' ')[0]
-        date_stamp = date_stamp.replace('-', '_')
-        return('_' + date_stamp)
-
-    def datetime_stamp(self):
-        time_stamp = '%s' % datetime.now().replace(microsecond=0)
-        time_stamp = time_stamp.replace('-', '_')
-        time_stamp = time_stamp.replace(' ', '_')
-        time_stamp = time_stamp.replace(':', '_')
-        return('_' + time_stamp)
+        if self.station.shot_type == 'measure':
+            self.popup = e5_MessageBox('Measurement',
+                                        self.make_x_shot_summary(),
+                                        response_type = "Other",
+                                        response_text = ['Close', 'Repeat'],
+                                        call_back = [self.cancel_x_shot, self.record_another_x_shot],
+                                        colors = self.colors)
+            if self.station.make not in ['Manual XYZ', 'Manual VHD', 'Simulate', '']:
+                self.event = Clock.schedule_interval(self.check_for_station_response_x_shot, .1)
+            self.popup.open()
+        else:
+            self.add_point_record()
+            if self.data.db is not None:
+                self.data.db.table(self.data.table).on_save = self.on_save
+                self.data.db.table(self.data.table).on_cancel = self.on_cancel
+            self.parent.current = 'EditPointScreen'
+            self.event = Clock.schedule_interval(self.check_for_station_response_edit_record, .1)
 
-    def close_popup(self, value):
+    def cancel_x_shot(self, instance):
         self.popup.dismiss()
-        self.popup_open = False
-        self.event = Clock.schedule_once(self.set_focus, 1)
+        if self.event:
+            self.event.cancel()
+            self.station.cancel()
+
+    def check_for_station_response_edit_record(self, dt):
+        if self.station.data_waiting():
+            if self.station.make in ['Leica']:
+                self.station.fetch_point()
+            elif self.station.make in ['Leica GeoCom']:
+                self.station.fetch_point_leica_geocom()
+            elif self.station.make in ['Topcon']:
+                self.station.fetch_point_topcon()
+            if self.station.response:
+                self.station.make_global()
+                self.station.prism_adjust()
+                sm.get_screen('EditPointScreen').reset_defaults_from_recorded_point(self.station)
+                self.event.cancel()
+
+    def check_for_station_response_x_shot(self, dt):
+        if self.station.data_waiting():
+            if self.station.make in ['Leica']:
+                self.station.fetch_point()
+            elif self.station.make in ['Leica GeoCom']:
+                self.station.fetch_point_leica_geocom()
+            elif self.station.make in ['Topcon']:
+                self.station.fetch_point_topcon()
+            if self.station.response:
+                self.station.make_global()
+                self.station.prism_adjust()
+                self.popup.refresh_text(self.make_x_shot_summary())
+                if not self.station.xyz.is_none():
+                    self.event.cancel()
+
+    def make_x_shot_summary(self):
+        if self.station.xyz.is_none():
+            return '\n  Waiting....'
+
+        txt = f'\nCoordinates:\n  X:  {self.station.xyz_global.x:.3f}\n  Y:  {self.station.xyz_global.y:.3f}\n  Z:  {self.station.xyz_global.z:.3f}'
+        unitname = self.data.point_in_unit(self.station.xyz_global)
+        if unitname:
+            txt += f'\n\nThe point is in unit {unitname}.'
+        if self.station.make != 'Microscribe':
+            txt += f'\n\nMeasurement Data:\n  Horizontal angle:  {self.station.decimal_degrees_to_sexa_pretty(self.station.hangle)}\n  ' \
+                   f'Vertical angle:  {self.station.decimal_degrees_to_sexa_pretty(self.station.vangle)}\n  ' \
+                   f'Slope distance:  {self.station.sloped:.3f}'
+            txt += f'\n  X:  {self.station.xyz.x:.3f}\n  Y:  {self.station.xyz.y:.3f}\n  Z:  {self.station.xyz.z:.3f}'
+            txt += f'\n\nStation coordinates:\n  X:  {self.station.location.x:.3f}\n  Y:  {self.station.location.y:.3f}\n  Z:  {self.station.location.z:.3f}'
+            if self.station.prism_constant:
+                txt += f'\n\nPrism constant :  {self.station.prism_constant} m'
+            if self.station.received:
+                txt += f'\n\nData stream:\n  {self.station.received}'
+            if self.station.error_code != 0:
+                txt += f'\n{self.station.error_message}'
+        return txt
+
+    def record_another_x_shot(self, instance):
+        if self.station.make in ['Manual XYZ', 'Manual VHD', 'Simulate', 'Microscribe']:
+            self.close_popup(instance)
+            self.take_shot(self.measure_button)
+        else:
+            self.station.take_shot()
+            self.popup.refresh_text('\n  Waiting...')
+            self.event = Clock.schedule_interval(self.check_for_station_response_x_shot, .1)
+
+    def on_save(self):
+        self.log_the_shot()
+        self.update_info_label()
+        self.make_backup()
+        self.check_for_duplicate_xyz()
+        return []
+
+    def log_the_shot(self):
+        logger = logging.getLogger(__name__)
+        logger.info(f'{self.get_last_squid()} {self.station.vhd_to_sexa_pretty_compact()} with prism height {self.station.prism.height} '
+                        'from {self.station.location} ')
+
+    def on_cancel(self):
+        if self.data.db is not None:
+            last_record = self.data.db.table(self.data.table).all()[-1]
+            if last_record != []:
+                self.data.db.table(self.data.table).remove(doc_ids = [last_record.doc_id])
+
+    def get_last_squid(self):
+        unit = self.get_last_value('UNIT')
+        idno = self.get_last_value('ID')
+        suffix = self.get_last_value('SUFFIX')
+        return f'{unit}-{idno}({suffix})' if all(item is not None for item in [unit, idno, suffix]) else ''
+
+    def update_info_label(self):
+        last_squid = self.get_last_squid()
+        self.info.text = last_squid if last_squid else 'EDM'
+
+    def same_coordinates(record1, record2):
+        return record1['X'] == record2['X'] and record1['Y'] == record2['Y'] and record1['Z'] == record2['Z']
+
+    def check_for_duplicate_xyz(self):
+        if self.station.make == 'Microscribe' and self.data.db is not None:
+            if len(self.data.db.table(self.data.table)) > 1:
+                last_record = self.data.db.table(self.data.table).all()[-1]
+                next_to_last_record = self.data.db.table(self.data.table).all()[-2]
+                if all(field in last_record.keys() for field in ['X', 'Y', 'Z']):
+                    if self.same_coordinates(last_record, next_to_last_record):
+                        self.popup = e5_MessageBox(title = 'Warning',
+                                                    message = "\nThe last two recorded points have the exact same XYZ "
+                                                        f"coordinates ({last_record['X']}, {last_record['Y']}, {last_record['Z']}).  "
+                                                        "Verify that the Microscribe is still properly recording points (green light is on).  "
+                                                        "If the red light is on, you need to re-initialize (Setup - Initialize Station) and "
+                                                        "re-shoot the last two points.")
+                        self.popup.open()
 
-    def set_focus(self, value):
-        self.widget_with_focus.focus = True
+    def close_popup(self, instance):
+        self.popup.dismiss()
 
-    def show_delete_last_object(self):
-        last_record = self.data.last_record()
-        if last_record:
-            message_text = '\nDelete the following records?\n\n'
-            if 'UNIT' in last_record.keys() and 'ID' in last_record.keys():
-                unit = last_record["UNIT"]
-                idno = last_record["ID"]
-                a_record = Query()
-                records_to_delete = self.data.db.table(self.data.table).search(a_record.UNIT.matches('^' + unit + '$', flags = re.IGNORECASE) and a_record.ID.matches('^' + idno + '$', flags = re.IGNORECASE))
-                for record in records_to_delete:
-                    for field in self.cfg.fields():
-                        if field in record:
-                            message_text += "%s : %s \n" % (field, record[field])
-                    message_text += '\n\n'
-                self.popup = e5_MessageBox('Delete last object', message_text, response_type = "YESNO",
-                                            call_back = [self.delete_last_object, self.close_popup],
-                                            colors = self.colors)
-            else:
-                self.popup = e5_MessageBox('Delete last object', '\nFor now, this option requires a field called UNIT and another called ID.',
-                                            call_back = self.close_popup,
-                                            colors = self.colors)
-        else:
-            self.popup = e5_MessageBox('Delete last object', '\nNo records in table to delete.',
-                                        call_back = self.close_popup,
-                                        colors = self.colors)
+    def save_default_cfg(self):
+        content = e5_SaveDialog(filename = '',
+                                start_path = self.cfg.path,
+                                save = self.save_default,
+                                cancel = self.dismiss_popup)
+        self.popup = Popup(title = "Create a new default CFG file",
+                            content = content,
+                            size_hint = (0.9, 0.9))
         self.popup.open()
         self.popup_open = True
 
-    def delete_last_object(self, value):
-        last_record = self.data.last_record()
-        unit = last_record["UNIT"]
-        idno = last_record["ID"]
-        a_record = Query()
-        records_to_delete = self.data.db.table(self.data.table).search(a_record.UNIT.matches('^' + unit + '$', flags = re.IGNORECASE) and a_record.ID.matches('^' + idno + '$', flags = re.IGNORECASE))
-        for record in records_to_delete:
-            self.data.delete(record.doc_id)
-        self.data.new_data[self.data.table] = True
-        self.close_popup(value)
-
-    def show_delete_last_record(self):
-        last_record = self.data.last_record()
-        if last_record:
-            message_text = '\n'
-            for field in self.cfg.fields():
-                if field in last_record:
-                    message_text += "%s : %s \n" % (field, last_record[field])
-            self.popup = e5_MessageBox('Delete Last Record', message_text, response_type = "YESNO",
-                                        call_back = [self.delete_last_record, self.close_popup],
-                                        colors = self.colors)
+    def save_default(self, *args):
+        path = self.popup.content.filesaver.path
+        filename = self.popup.content.filename
+        if '.cfg' not in filename.lower():
+            filename = filename + '.cfg'
+        self.cfg.initialize()
+        self.cfg.build_default()
+        self.ini.update_value(APP_NAME, 'CFG', os.path.join(path, filename))
+        self.cfg.update_value(APP_NAME, 'DATABASE', os.path.join(path, filename.split('.')[0] + '.json'))
+        self.cfg.update_value(APP_NAME, 'TABLE', filename.split('.')[0])
+        self.data.open(os.path.join(path, filename.split('.')[0] + '.json'))
+        self.open_db()
+        self.set_new_data_to_true()
+        self.cfg.filename = os.path.join(path, filename)
+        self.cfg.save()
+        self.ini.update(self.colors, self.cfg)
+        self.dismiss_popup()
+        self.build_mainscreen()
+        self.reset_screens()
+
+    def set_new_data_to_true(self, table_name = None):
+        if table_name is None:
+            self.data.new_data['prisms'] = True
+            self.data.new_data['units'] = True
+            self.data.new_data['datums'] = True
+            self.data.new_data[self.data.table] = True
         else:
-            self.popup = e5_MessageBox('Delete Last Record', '\nNo records in table to delete.',
-                                        call_back = self.close_popup,
-                                        colors = self.colors)
-        self.popup.open()
-        self.popup_open = True
+            self.data.new_data[table_name] = True
 
-    def delete_last_record(self, value):
-        last_record = self.data.last_record()
-        self.data.delete(last_record.doc_id)
-        self.data.new_data[self.data.table] = True
-        self.close_popup(value)
-
-    def show_delete_all_records(self, table_name = None):
-        if not table_name:
-            message_text = '\nYou are asking to delete all of the records in the current database table. Are you sure you want to do this?'
-            self.delete_table = self.data.table
-        else:
-            message_text = '\nYou are asking to delete all of the records in the %s table. Are you sure you want to do this?' % table_name
-            self.delete_table = table_name
-        self.popup = e5_MessageBox('Delete All Records', message_text, response_type = "YESNO",
-                                    call_back = [self.delete_all_records1, self.close_popup],
-                                    colors = self.colors)
+    def show_load_cfg(self):
+        start_path = self.cfg.path if self.cfg.path else self.app_paths.app_data_path
+        if not os.path.exists(start_path):
+            start_path = os.path.abspath(os.path.dirname(__file__))
+        content = e5_LoadDialog(load = self.load_cfg,
+                                cancel = self.dismiss_popup,
+                                start_path = start_path,
+                                button_color = self.colors.button_color,
+                                button_background = self.colors.button_background,
+                                font_size = self.colors.button_font_size)
+        self.popup = Popup(title = "Load CFG file",
+                            content = content,
+                            size_hint = (0.9, 0.9))
         self.popup.open()
-        self.popup_open = True
 
-    def delete_all_records1(self, value):
-        self.close_popup(value)
-        message_text = '\nThis is your last chance.  All records in the %s table will be deleted when you press Yes.' % self.delete_table
-        self.popup = e5_MessageBox('Delete All Records', message_text, response_type = "YESNO",
-                                    call_back = [self.delete_all_records2, self.close_popup],
-                                    colors = self.colors)
-        self.popup.open()
-        self.popup_open = True
+    def load_cfg(self, path, filename):
+        warnings, errors = [], []
+        self.data.close()
+        self.dismiss_popup()
+        self.cfg.load(os.path.join(path, filename[0]))
+        if self.cfg.filename:
+            warnings, errors = self.open_db()
+            if errors == []:
+                self.set_new_data_to_true()
+        self.ini.update(self.colors, self.cfg)
+        self.build_mainscreen()
+        self.reset_screens()
+        if warnings or errors:
+            self.popup = self.warnings_and_errors_popup(warnings, errors)
+            self.popup.open()
 
-    def delete_all_records2(self, value):
-        self.data.delete_all(self.delete_table)
-        self.data.new_data[self.data.table] = True
-        self.close_popup(value)
-
-    def show_save_csvs(self, *args):
-        if self.cfg.filename and self.data.filename:
-            if len(args) > 0:
-                self.csv_data_type = args[0].id.lower()
-            else:
-                self.csv_data_type = self.data.table
-            filename = ntpath.split(self.cfg.filename)[1].split(".")[0]
-            filename = filename + "_" + self.csv_data_type + self.date_stamp() + '.csv'
-            content = e5_SaveDialog(filename = filename,
-                                    start_path = self.cfg.path,
-                                    save = self.save_csvs,
-                                    cancel = self.dismiss_popup)
-            self.popup = Popup(title = "Export CSV file",
-                                content = content,
-                                size_hint = (0.9, 0.9))
-        else:
-            self.popup = e5_MessageBox('E5', '\nOpen a CFG before exporting to CSV',
-                                        call_back = self.dismiss_popup,
+    def reset_screen_defaults(self):
+        sm.get_screen('EditPointScreen').e5_cfg = self.cfg
+        sm.get_screen('EditPointScreen').data_table = self.data.table
+        sm.get_screen('EditPointScreen').data = self.data
+        sm.get_screen('EditLastRecordScreen').data_table = self.data.table
+
+    def show_import_csv(self):
+        if not self.ready_to_use():
+            self.popup = self.message_open_cfg_first()
+        else:
+            instructions = 'EDM can import data from EDM-Mobile, EDMWin, EDM itself, or user prepared data files.'
+            instructions += '  The two import formats are CSV and JSON.'
+            instructions += '  CSV files should have a csv or txt extension.  JSON files should have a json extension.'
+            instructions += '  See our web site for more information on exporting data from EDM-Mobile and EDMWin.'
+            instructions += '  The JSON option is for easy importing from EDM data files.'
+            instructions += '  Importing points from JSON files is not yet available.'
+            instructions += '  IMPORT: Imported data will overwrite existing data in the case of duplicates.'
+            self.popup = e5_PopUpMenu(title = "Load which kind of data", message = instructions,
+                                        menu_list = ['Points', 'Datums', 'Prisms', 'Units'],
+                                        menu_selected = '',
+                                        call_back = self.select_csv_file,
                                         colors = self.colors)
         self.popup.open()
-        self.popup_open = True
 
-    def save_csvs(self, instance):
-
-        path = self.popup.content.filesaver.path
-        filename = self.popup.content.filename
+    def show_csv_datatype(self):
+        if not self.ready_to_use():
+            self.popup = self.message_open_cfg_first()
+        else:
+            self.popup = e5_PopUpMenu(title = "Export which kind of data", message = '',
+                                            menu_list = ['Points', 'Datums', 'Prisms', 'Units'],
+                                            menu_selected = '',
+                                            call_back = self.show_save_csvs,
+                                            colors = self.colors)
+        self.popup.open()
 
+    def select_csv_file(self, instance):
+        self.csv_data_type = instance.text
         self.popup.dismiss()
+        start_path = self.cfg.path if self.cfg.path else self.app_paths.app_data_path
+        content = e5_LoadDialog(load = self.load_csv,
+                                cancel = self.dismiss_popup,
+                                start_path = start_path,
+                                button_color = self.colors.button_color,
+                                button_background = self.colors.button_background,
+                                filters = ['*.csv', '*.CSV', '*.txt', '*.TXT', '*.json', '*.JSON'])
+        self.popup = Popup(title = "Select CSV or JSON file to import from",
+                            content = content,
+                            size_hint = (0.9, 0.9))
+        self.popup.open()
 
-        filename = os.path.join(path, filename)
+    def read_csv_file(self, full_filename):
+        data = []
+        with open(full_filename, newline='') as csvfile:
+            reader = csv.DictReader(csvfile, quoting = csv.QUOTE_NONNUMERIC)
+            for row in reader:
+                data.append(row)
+        fields = [field.upper() for field in reader.fieldnames]
+        return fields, data
 
-        if __program__ == 'EDM' and self.csv_data_type != 'points':
-            table = self.data.db.table(self.csv_data_type)
-            if self.csv_data_type == 'datums':
-                errors = self.cfg_datums.write_csvs(filename, table)
-            if self.csv_data_type == 'units':
-                errors = self.cfg_units.write_csvs(filename, table)
-            if self.csv_data_type == 'prisms':
-                errors = self.cfg_prisms.write_csvs(filename, table)
+    def read_json_table(self, full_filename, data_type):
+        data = []
+        if data_type.upper() in ['DATUMS', 'UNITS', 'PRISMS']:
+            data = TinyDB(full_filename).table(data_type.lower()).all()
+        fields = data[0].keys() if data else []
+        return fields, data
+
+    def check_import_fields_against_cfg_fields(self, fields):
+        cfg_fields = self.cfg.fields()
+        missing_fields = [field for field in fields if field not in cfg_fields]
+        missing_fields = [field for field in missing_fields if field not in ['RECNO', 'TIME']]
+        if missing_fields:
+            return (f"The following field(s) are present in the import data but not in the current CFG: {', '.join(missing_fields)}. "
+                    "Importing these data could cause the loss of data.  Please add these missing fields to the CFG before importing "
+                    "these data.")
         else:
-            table = self.data.db.table(self.data.table)
-            errors = self.cfg.write_csvs(filename, table)
+            return ""
 
-        title = 'CSV Export'
-        if errors:
-            self.popup = e5_MessageBox(title, errors, call_back = self.close_popup, colors = self.colors)
-        else:
-            self.popup = e5_MessageBox(title, '\nThe table %s was successfully written as the file %s.' % (self.csv_data_type, filename),
-                                        call_back = self.close_popup, colors = self.colors)
-        self.popup.open()
-        self.popup_open = True
+    def get_unique_key(self, data_record):
+        unique_key = []
+        for field in self.cfg.unique_together:
+            unique_key.append("%s" % data_record[field])
+        return ",".join(unique_key)
+
+    def check_unique_together(self, data_record):
+        if self.data.db is not None:
+            if self.cfg.unique_together and len(self.data.db.table(self.data.table)) > 1:
+                unique_key = self.get_unique_key(data_record)
+                for doc_id in self.data.doc_ids():
+                    if unique_key == self.get_unique_key(self.data.db.table(self.data.table).get(doc_id = doc_id)):
+                        return doc_id
+        return ''
+
+    def error_check_import(self, fields):
+        errors = ''
+        if self.csv_data_type == 'Datums':
+            if len(fields) < 4:
+                errors = '\nThese data seem to have fewer than four fields.  To import datums requires a Name, X, Y, and Z field.  '\
+                         'If this is a CSV file, the first row in the file should contain these field names separated by commas.  '\
+                         f'The fieldnames read were {fields}.'
+            if 'X' not in fields or 'Y' not in fields or 'Z' not in fields or 'NAME' not in fields:
+                errors = '\nIf these data are coming from a CSV file, the first row must list the field names (comma delimited) and '\
+                         f'must include a field called Name, X, Y and Z.  The fields read were {fields}.'
+        if self.csv_data_type == 'Prisms':
+            if len(fields) < 2:
+                errors = '\nThese data seem to have fewer than two fields.  To import prisms requires a Name and height and optionally '\
+                         'an offset field.  If this is a csv file, the first row in the file should contain these field names separated '\
+                         f'by commas.  The fieldnames read were {fields}.'
+            if 'NAME' not in fields or 'HEIGHT' not in fields:
+                errors = '\nIf these data are coming from a CSV file, the first row must list the field names (comma delimited) and must '\
+                         f'include a field called Name and Height.  The fields read were {fields}.'
+        if self.csv_data_type == 'Units':
+            if len(fields) < 5:
+                errors = '\nThese data seem to have fewer than five fields.  To import units requires a Unit, Minx, Miny, Maxx, Maxy field.  '\
+                         'If this is a CSV file, the first row in the file should contain these field names separated by commas.  '\
+                         f'The fieldnames read were {fields}.'
+            if 'UNIT' not in fields or 'MINX' not in fields or 'MINY' not in fields or 'MAXX' not in fields or 'MAXY' not in fields:
+                errors = '\nIf these data are coming from a CSV file, the first row must list the field names (comma delimited) and '\
+                         f'must include at least fields called Unit, Minx, Miny, Maxx, Maxy.  The fields read were {fields}.'
+        if self.csv_data_type == 'Points':
+            errors = self.check_import_fields_against_cfg_fields(fields)
+        return errors
+
+    def build_hash_unique_ids(self):
+        hash = {}
+        if self.data.db is not None:
+            for record in self.data.db.table(self.data.table):
+                hash[self.get_unique_key(record)] = record.doc_id
+        return hash
 
-    def show_save_geojson(self):
-        if self.cfg.filename and self.data.filename:
-            geojson_compatible = 0
-            for fieldname in self.cfg.fields():
-                if fieldname in ['X', 'Y', 'Z']:
-                    geojson_compatible += 1
-                elif fieldname in ['LATITUDE', 'LONGITUDE', 'ELEVATION']:
-                    geojson_compatible += 1
-                else:
-                    field = self.cfg.get(fieldname)
-                    if field.inputtype in ['GPS']:
-                        geojson_compatible = 2
-                if geojson_compatible > 1:
-                    break
-            if geojson_compatible:
-                filename = ntpath.split(self.cfg.filename)[1].split(".")[0]
-                filename = filename + '_' + self.data.table + '.geojson'
-
-                content = e5_SaveDialog(filename = filename,
-                                        start_path = self.cfg.path,
-                                        save = self.save_geojson,
-                                        cancel = self.dismiss_popup)
-                self.popup = Popup(title = "Export geoJSON file",
-                                    content = content,
-                                    size_hint = (0.9, 0.9))
-            else:
-                self.popup = e5_MessageBox('E5', '\nA geoJSON file requires a GPS type field or fields named XY(Z) or Latitude, Longitude and optionally Elevation.',
-                                            call_back = self.dismiss_popup,
-                                            colors = self.colors)
+    def import_these(self, data):
+        record_count = 0
+        replacements = 0
+        hash_unique_ids = self.build_hash_unique_ids()
+        if self.data.db is not None:
+            for item in data:
+                insert_record = {}
+                for key, value in item.items():
+                    if key.upper() == "UNIT" and self.csv_data_type == "Units":
+                        insert_record['NAME'] = value
+                    elif key.upper() == "DATE" and "TIME" in item:
+                        insert_record['DATE'] = value + " " + item['TIME']
+                    else:
+                        insert_record[key.upper()] = value
+                if self.csv_data_type in ['Datums', 'Prisms', 'Units']:
+                    if insert_record['NAME'].strip():
+                        if len(self.data.get_by_name(self.csv_data_type.lower(), insert_record['NAME'])) > 0:
+                            self.data.delete_by_name(self.csv_data_type.lower(), insert_record['NAME'])
+                            replacements += 1
+                        self.data.db.table(self.csv_data_type.lower()).insert(insert_record)
+                if self.csv_data_type == 'Points':
+                    new_docid = self.data.db.table(self.data.table).insert(insert_record)
+                    hash_key = self.get_unique_key(insert_record)
+                    if hash_key in hash_unique_ids:
+                        duplicate_doc_id = hash_unique_ids[hash_key]
+                        self.data.db.table(self.data.table).remove(doc_ids = [duplicate_doc_id])
+                        replacements += 1
+                    hash_unique_ids[hash_key] = new_docid
+                record_count += 1
+        return (record_count, replacements)
+
+    def load_csv(self, path, filename):
+        # TODO This routine does not properly import Units.  The unitfields need to be put into a separate table
+        # TODO Need to write the routine to import actual data
+        full_filename = os.path.join(path, filename[0])
+        self.dismiss_popup()
+
+        if '.csv' in full_filename.lower() or '.txt' in full_filename.lower():
+            fields, data = self.read_csv_file(full_filename)
         else:
-            self.popup = e5_MessageBox('E5', '\nOpen a CFG before exporting to geoJSON.',
-                                        call_back = self.dismiss_popup,
-                                        colors = self.colors)
-        self.popup.open()
-        self.popup_open = True
-
-    def save_geojson(self, path):
-        path = self.popup.content.filesaver.path
-        filename = self.popup.content.filename
-
-        self.popup.dismiss()
+            fields, data = self.read_json_table(full_filename, self.csv_data_type)
 
-        filename = os.path.join(path, filename)
+        errors = self.error_check_import(fields)
 
-        table = self.data.db.table(self.data.table)
+        if not errors:
+            record_count, replacements = self.import_these(data)
 
-        errors = self.cfg.write_geojson(filename, table)
-        title = 'geoJSON Export'
         if errors:
-            self.popup = e5_MessageBox(title, errors, call_back = self.close_popup, colors = self.colors)
+            message = errors
         else:
-            self.popup = e5_MessageBox(title, '\nThe table %s was successfully written as geoJSON to the file %s.' % (self.data.table, filename),
-                                        call_back = self.close_popup, colors = self.colors)
-        self.popup.open()
-        self.popup_open = True
+            if replacements == 0:
+                message = '%s %s successfully imported.' % (record_count, self.csv_data_type)
+            else:
+                message = '%s %s successfully imported.  Of these, %s updated an existing record.' % (record_count, self.csv_data_type, replacements)
 
+        self.popup = e5_MessageBox('CSV Import', message,
+                                    response_type = "OK",
+                                    call_back = self.close_popup,
+                                    colors = self.colors)
+        self.open_popup()
+        return errors
 
-class e5_gridlayout(GridLayout):
-    id = ObjectProperty(None)
+    def add_point_record(self):
+        new_record = {}
+        new_record = self.fill_default_fields(new_record)
+        if self.station.shot_type != 'continue':
+            new_record = self.find_unit_and_fill_fields(new_record)
+            new_record = self.fill_carry_fields(new_record)
+            new_record = self.fill_link_fields(new_record)
+            new_record = self.do_increments(new_record)
+            new_record['SUFFIX'] = 0
+            new_record = self.fill_button_defaults(new_record)
+        else:
+            new_record = self.fill_empty_with_last(new_record)
+            new_record['SUFFIX'] = int(self.get_last_value('SUFFIX')) + 1
+
+        self.data.db.table(self.data.table).insert(new_record)
+
+    def fill_empty_with_last(self, new_record):
+        for field in self.cfg.fields():
+            field_data = self.get_last_value(field)
+            if field_data is not None:
+                if field not in new_record.keys():
+                    new_record[field] = self.get_last_value(field)
+                elif new_record[field] == '':
+                    new_record[field] = self.get_last_value(field)
+        return new_record
+
+    def fill_button_defaults(self, new_record):
+        for button_no in range(1, __BUTTONS__):
+            button = self.cfg.get_block(f'BUTTON{button_no}')
+            if button:
+                if 'TITLE' in button.keys():
+                    if button['TITLE'] == self.station.shot_type:
+                        fieldnames = self.cfg.fields()
+                        for button_default in button:
+                            if button_default in fieldnames:
+                                if button[button_default].upper() == 'ALPHA':
+                                    # TODO Should be calibrated to the length of this field
+                                    new_record[button_default] = self.station.hash()
+                                else:
+                                    new_record[button_default] = button[button_default]
+        return new_record
+
+    def do_increments(self, new_record):
+        fieldnames = self.cfg.fields()
+        for fieldname in fieldnames:
+            field = self.cfg.get(fieldname)
+            if field.increment:
+                try:
+                    if fieldname in new_record.keys():
+                        new_record[fieldname] = int(new_record[fieldname]) + 1
+                    elif self.get_last_numeric_value(fieldname):
+                        new_record[fieldname] = int(self.get_last_value(fieldname)) + 1
+                    else:
+                        new_record[fieldname] = '1'
+                except (ValueError, TypeError):
+                    pass
+        return new_record
 
-    def __init__(self, **kwargs):
-        super(e5_gridlayout, self).__init__(**kwargs)
+    def fill_carry_fields(self, new_record):
+        fieldnames = self.cfg.fields()
+        for fieldname in fieldnames:
+            if fieldname not in __DEFAULT_FIELDS__:
+                field = self.cfg.get(fieldname)
+                if field.carry:
+                    carry_value = self.get_last_value(fieldname)
+                    if carry_value:
+                        new_record[fieldname] = carry_value
+        return new_record
+
+    def fill_link_fields(self, new_record):
+        fieldnames = self.cfg.fields()
+        for fieldname in fieldnames:
+            if fieldname not in __DEFAULT_FIELDS__:
+                field = self.cfg.get(fieldname)
+                if field.link_fields:
+                    if fieldname in new_record.keys():
+                        linkfields = self.data.get_link_fields(fieldname, new_record[fieldname])
+                        if linkfields:
+                            for link_fieldname in linkfields.keys():
+                                new_record[link_fieldname] = linkfields[link_fieldname]
+        return new_record
+
+    def find_unit_and_fill_fields(self, new_record):
+        fields = self.cfg.fields()
+        unitname = self.data.point_in_unit(self.station.xyz_global)
+        if unitname and "UNIT" in fields:
+            new_record['UNIT'] = unitname
+            unitfields = self.data.get_link_fields('UNIT', unitname)
+            if unitfields:
+                for field in unitfields.keys():
+                    new_record[field] = unitfields[field]
+        return new_record
+
+    def fill_default_fields(self, new_record):
+        fields = self.cfg.fields()
+        for field in fields:
+            value = self.station.format_widget_value(field)
+            if value != '':
+                new_record[field] = value
+            if field == 'DATE':
+                new_record['DATE'] = f'{datetime.now().replace(microsecond=0)}'
+        return new_record
+
+    def get_last_value(self, field_name):
+        if self.data.db is not None:
+            if len(self.data.db.table(self.data.table)) > 0:
+                last_record = self.data.db.table(self.data.table).all()[-1]
+                if last_record != []:
+                    if field_name in last_record.keys():
+                        return last_record[field_name]
+        return None
+
+    def get_last_numeric_value(self, field_name):
+        if self.data.db is not None:
+            if len(self.data.db.table(self.data.table)) > 0:
+                for record in reversed(self.data.db.table(self.data.table).all()):
+                    if record != []:
+                        if field_name in record.keys():
+                            if self.is_numeric(record[field_name]):
+                                return record[field_name]
+        return None
 
+    def is_numeric(self, value):
+        try:
+            float(value)
+            return True
+        except ValueError:
+            return False
+
+    def exit_program(self):
+        logger = logging.getLogger(__name__)
+        logger.info(APP_NAME + ' exited.')
+        self.save_window_location()
+        App.get_running_app().stop()
 
-class e5_SettingsScreen(Screen):
 
-    def __init__(self, cfg = None, ini = None, colors = None, **kwargs):
-        super(e5_SettingsScreen, self).__init__(**kwargs)
+class OptionsScreen(Screen):
+    def __init__(self, station = None, cfg = None, colors = None, **kwargs):
+        super(OptionsScreen, self).__init__(**kwargs)
+
         self.colors = colors if colors else ColorScheme()
-        self.ini = ini
+        self.station = station
         self.cfg = cfg
 
-    def on_enter(self):
+        self.clear_widgets()
+        self.layout = GridLayout(cols = 1,
+                                    spacing = 5, padding = 5,
+                                    size_hint_max_x = MAX_SCREEN_WIDTH,
+                                    size_hint_y = 1,
+                                    pos_hint = {'center_x': .5, 'center_y': .5})
+        self.add_widget(self.layout)
         self.build_screen()
 
     def build_screen(self):
-        self.clear_widgets()
-        layout = GridLayout(cols = 1,
-                            # size_hint_x = width_calculator(.9, 600),
-                            # size_hint_y = .9,
-                            spacing = 5,
-                            padding = 5,
-                            pos_hint = {'center_x': .5, 'center_y': .5})
-        layout.bind(minimum_height = layout.setter('height'))
-
-        darkmode = GridLayout(cols = 2, size_hint_y = .1, spacing = 5, padding = 5)
-        darkmode.add_widget(e5_label('Dark Mode', colors = self.colors))
-        darkmode_switch = Switch(active = self.colors.darkmode)
-        darkmode_switch.bind(active = self.darkmode)
-        darkmode.add_widget(darkmode_switch)
-        layout.add_widget(darkmode)
-
-        colorscheme = GridLayout(cols = 2, size_hint_y = .6, spacing = 5, padding = 5)
-        colorscheme.add_widget(e5_label('Color Scheme', colors = self.colors))
-        colorscheme.add_widget(e5_scrollview_menu(self.colors.color_names(),
-                                                  menu_selected = '',
-                                                  colors = self.colors,
-                                                  call_back = [self.color_scheme_selected]))
-        temp = ColorScheme()
-        for widget in colorscheme.walk():
-            if hasattr(widget, 'id'):
-                if widget.id in self.colors.color_names():
-                    temp.set_to(widget.text)
-                    widget.background_color = temp.button_background
-        layout.add_widget(colorscheme)
-
-        backups = GridLayout(cols = 2, size_hint_y = .3, spacing = 5, padding = 5)
-        self.backup_label = e5_label(f'Auto-backup after\n{self.ini.backup_interval} records.',
-                                        colors = self.colors)
-        backups.add_widget(self.backup_label)
-        slide = Slider(min = 0, max = 200, step = 5,
-                        value = self.ini.backup_interval,
-                        orientation = 'horizontal',
-                        value_track = True,
-                        value_track_color = self.colors.button_background)
-        backups.add_widget(slide)
-        slide.bind(value = self.update_backup_interval)
-        backups.add_widget(e5_label('Use incremental\nbackups?', colors = self.colors))
-        backups_switch = Switch(active = self.ini.incremental_backups)
-        backups_switch.bind(active = self.incremental_backups)
-        backups.add_widget(backups_switch)
-        layout.add_widget(backups)
-
-        text_font_size = GridLayout(cols = 2, size_hint_y = .3, spacing = 5, padding = 5)
-        if self.colors.text_font_size:
-            text_font_size_value = int(self.colors.text_font_size.replace("sp", ''))
-        else:
-            text_font_size_value = 12
-        self.text_font_size_label = e5_label('Text font size is %s' % text_font_size_value,
-                                                id = 'label_font_size',
-                                                colors = self.colors)
-        text_font_size.add_widget(self.text_font_size_label)
-        text_font_slide = Slider(min = 12, max = 26, step = 1, value = text_font_size_value,
-                                    orientation = 'horizontal',
-                                    value_track = True, value_track_color = self.colors.button_background)
-        text_font_size.add_widget(text_font_slide)
-        text_font_slide.bind(value = self.update_text_font_size)
-        layout.add_widget(text_font_size)
-
-        button_font_size = GridLayout(cols = 2, size_hint_y = .3, spacing = 5, padding = 5)
-        if self.colors.button_font_size:
-            button_font_size_value = int(self.colors.button_font_size.replace("sp", ''))
-        else:
-            button_font_size_value = 12
-        self.button_font_size_label = e5_label('Button font size is %s' % button_font_size_value,
-                                                id = 'label_font_size',
-                                                colors = self.colors)
-        button_font_size.add_widget(self.button_font_size_label)
-        button_font_slide = Slider(min = 12, max = 26, step = 1, value = button_font_size_value,
-                                    orientation = 'horizontal',
-                                    value_track = True, value_track_color = self.colors.button_background)
-        button_font_size.add_widget(button_font_slide)
-        button_font_slide.bind(value = self.update_button_font_size)
-        layout.add_widget(button_font_size)
-
-        settings_layout = GridLayout(cols = 1,
-                                        size_hint_x = width_calculator(.9, 400),
-                                        size_hint_y = .9,
-                                        spacing = 5,
-                                        pos_hint = {'center_x': .5, 'center_y': .5})
-        scrollview = ScrollView(size_hint = (1, 1),
-                                 bar_width = SCROLLBAR_WIDTH)
-        scrollview.add_widget(layout)
-        settings_layout.add_widget(scrollview)
+        prism = GridLayout(cols = 2, size_hint_y = .1, spacing = 5, padding = 5)
+        prism.add_widget(e5_label('Prompt for prism height after each point', colors = self.colors))
+        prism_switch = Switch(active = self.station.prism_prompt)
+        prism_switch.bind(active = self.prism_prompt)
+        prism.add_widget(prism_switch)
+        self.layout.add_widget(prism)
 
         self.back_button = e5_button('Back', selected = True,
                                              call_back = self.go_back,
-                                             colors = self.colors,
-                                             size_hint_x = width_calculator(.9, 600))
-        settings_layout.add_widget(self.back_button)
-        self.add_widget(settings_layout)
-
-    def update_text_font_size(self, intance, value):
-        self.text_font_size_label.text = 'Text font size is %s' % int(value)
-        self.colors.text_font_size = '%ssp' % value
-        self.build_screen()
-
-    def update_button_font_size(self, intance, value):
-        self.button_font_size_label.text = 'Button font size is %s' % int(value)
-        self.colors.button_font_size = '%ssp' % value
-        self.build_screen()
-
-    def update_backup_interval(self, instance, value):
-        self.ini.backup_interval = int(value)
-        self.backup_label.text = 'Auto-backup after\nevery %s\nrecords entered.' % self.ini.backup_interval
-
-    def incremental_backups(self, instance, value):
-        self.ini.incremental_backups = value
-
-    def darkmode(self, instance, value):
-        self.colors.darkmode = value
-        self.colors.set_colormode()
-        self.build_screen()
+                                             colors = self.colors)
+        self.layout.add_widget(self.back_button)
 
-    def color_scheme_selected(self, instance):
-        self.colors.set_to(instance.text)
-        self.back_button.background_color = self.colors.button_background
-        self.back_button.color = self.colors.button_color
+    def prism_prompt(self, instance, value):
+        self.station.prism_prompt = value
 
     def go_back(self, instance):
-        self.ini.update(self.colors, self.cfg)
         self.parent.current = 'MainScreen'
 
 
-class e5_InfoScreen(Screen):
-    content = ObjectProperty(None)
-    back_button = ObjectProperty(None)
+class ComTestScreen(Screen):
+    def __init__(self, station = None, cfg = None, colors = None, **kwargs):
+        super(ComTestScreen, self).__init__(**kwargs)
 
-    def __init__(self, colors = None, **kwargs):
-        super(e5_InfoScreen, self).__init__(**kwargs)
         self.colors = colors if colors else ColorScheme()
-        layout = GridLayout(cols = 1, size_hint_y = 1, spacing = 5, padding = 5)
-        layout.add_widget(e5_scrollview_label(text = '', widget_id = 'content', colors = self.colors))
-        layout.add_widget(e5_side_by_side_buttons(['Back', 'Copy'],
-                                                    id = ['back_button', 'copy_button'],
-                                                    selected = [False, False],
-                                                    call_back = [self.go_back, self.copy],
-                                                    colors = self.colors))
-        self.add_widget(layout)
-        for widget in self.walk():
-            if hasattr(widget, 'id'):
-                if widget.id == 'content_label':
-                    self.content = widget
-                if widget.id == 'back_button':
-                    self.back_button = widget
+        self.station = station
+        self.cfg = cfg
 
-    def go_back(self, *args):
-        self.parent.current = 'MainScreen'
+        self.clear_widgets()
+        self.layout = GridLayout(cols = 1,
+                                    spacing = 5, padding = 5,
+                                    size_hint_max_x = MAX_SCREEN_WIDTH,
+                                    size_hint_y = 1,
+                                    pos_hint = {'center_x': .5, 'center_y': .5})
+        self.add_widget(self.layout)
+        self.build_screen()
 
-    def copy(self, instance):
-        Clipboard.copy(self.content.text)
+    def current_settings_pretty(self):
+        txt = f'Current settings:\n{self.station.make}\n{self.station.settings_pretty()}'
+        txt += '\nCOM port is '
+        txt += 'Open' if self.station.serialcom.is_open else 'Close'
+        return txt
 
+    def on_enter(self):
+        sm.get_screen('StationConfigurationScreen').call_back = 'MainScreen'
+        self.current_settings.text = self.current_settings_pretty()
+        self.station.clear_io()
+        self.event = Clock.schedule_interval(self.check_io, .2)
+
+    def check_io(self, dt):
+        if self.station.data_waiting():
+            self.station.receive()
+        if self.station.io != '' and self.station.io != self.io.scrolling_label.text:
+            '''This is a hack to work around an issue I had when changing the content of 
+            a scrollbox label.  It wouldn't let me go beyond the size of the original content.
+            So now I remove it and  rebuild it.
+            '''
+            self.layout.remove_widget(self.io)
+            self.layout.remove_widget(self.buttons)
+            self.io = e5_scrollview_label(self.station.io, popup = False, colors = self.colors)
+            self.layout.add_widget(self.io)
+            self.layout.add_widget(self.buttons)
 
-class e5_LogScreen(e5_InfoScreen):
+    def build_screen(self):
+        self.settings = GridLayout(cols = 2, spacing = 5, padding = 5, size_hint = (.2, None))
+        self.current_settings = e5_label(self.current_settings_pretty(), colors = self.colors)
+        self.settings.add_widget(self.current_settings)
+        self.change_settings = e5_button("Change Settings", call_back = self.settings_change, colors = self.colors)
+        self.settings.add_widget(self.change_settings)
+        self.layout.add_widget(self.settings)
+
+        self.horizontal_angle = GridLayout(cols = 2, spacing = 5, padding = 5, size_hint = (.2, None))
+        self.leftside = GridLayout(cols = 1, spacing = 5, padding = 5)
+        self.leftside.add_widget(e5_label('Enter angle as ddd.mmss', colors = self.colors))
+        self.hangle_input = e5_textinput(write_tab = False)
+        self.hangle_input.bind(minimum_height = self.hangle_input.setter('height'))
+        self.leftside.add_widget(self.hangle_input)
+        self.horizontal_angle.add_widget(self.leftside)
+        self.set_angle = e5_button("Set H-angle", call_back = self.set_hangle, colors = self.colors)
+        self.horizontal_angle.add_widget(self.set_angle)
+        self.layout.add_widget(self.horizontal_angle)
+
+        self.record = GridLayout(cols = 1, spacing = 5, padding = 5, size_hint = (.2, None))
+        self.measure = e5_button("Record Point", call_back = self.record_point, colors = self.colors)
+        self.record.add_widget(self.measure)
+        self.layout.add_widget(self.record)
+
+        self.io = e5_scrollview_label('Set an angle or record a point and the communication to the station will appear here.  '
+                                        'If nothing is received at all, then it might be a COM port number issue.  '
+                                        'If what is received is unreadable, then there is a problem with the speed, parity, data bits, and stop bits.  '
+                                        'If everything looks fine, but the angle does not change or a point is not taken, '
+                                        'then likely Shannon needs to have a look.  '
+                                        'Email the results here to him.', popup = False, colors = self.colors)
+        self.layout.add_widget(self.io)
+
+        self.buttons = e5_side_by_side_buttons(text = ['Back', 'Clear', 'Copy'],
+                                                        id = ['back', 'clear', 'copy'],
+                                                        call_back = [self.close, self.clear_io, self.copy_io],
+                                                        selected = [False, False, False],
+                                                        colors = self.colors)
+        self.layout.add_widget(self.buttons)
+
+    def clear_io(self, instance):
+        self.station.clear_io()
+        self.station.clear_serial_buffers()
+        self.io.scrolling_label.text = ''
+
+    def copy_io(self, instance):
+        Clipboard.copy(self.io.scrolling_label.text)
+
+    def set_hangle(self, instance):
+        if self.hangle_input.textbox.text:
+            self.station.set_horizontal_angle(self.hangle_input.textbox.text)
+            # self.io.scrolling_label.text = self.station.io
 
-    def __init__(self, logger = None, **kwargs):
-        super(e5_LogScreen, self).__init__(**kwargs)
-        self.logger = logger
+    def settings_change(self, instance):
+        sm.get_screen('StationConfigurationScreen').call_back = 'ComTestScreen'
+        self.event.cancel()
+        self.parent.current = 'StationConfigurationScreen'
 
-    def on_pre_enter(self):
-        self.content.text = 'The last 150 lines:\n\n'
-        try:
-            with open(self.logger.handlers[0].baseFilename, 'r') as f:
-                content = f.readlines()
-            self.content.text += ''.join(list(reversed(content))[0:150])
-        except AttributeError:
-            self.content.text = '\nThe logger has not been initialized.'
-        except OSError:
-            self.content.text = "\nAn error occurred when reading the log file '%s'." % (self.logger.handlers[0].baseFilename)
-        self.content.color = self.colors.text_color
-        self.back_button.background_color = self.colors.button_background
-        self.back_button.color = self.colors.button_color
+    def record_point(self, instance):
+        self.station.stop_and_clear_geocom()
+        self.station.take_shot()
 
+    def close(self, instance):
+        self.event.cancel()
+        self.parent.current = 'MainScreen'
 
-class e5_INIScreen(e5_InfoScreen):
 
-    def __init__(self, ini = None, **kwargs):
-        super(e5_INIScreen, self).__init__(**kwargs)
-        self.ini = ini
+class RecordDatumsScreen(Screen):
 
-    def on_pre_enter(self):
-        with open(self.ini.filename, 'r') as f:
-            self.content.text = f.read()
-        self.content.color = self.colors.text_color
-        self.back_button.background_color = self.colors.button_background
-        self.back_button.color = self.colors.button_color
+    def __init__(self, data = None, station = None, ini = None, colors = None, **kwargs):
+        super(RecordDatumsScreen, self).__init__(**kwargs)
 
+        self.colors = colors if colors else ColorScheme()
+        self.station = station
+        self.data = data
+        self.ini = ini
 
-class e5_CFGScreen(e5_InfoScreen):
+        self.content = BoxLayout(orientation = 'vertical',
+                                    size_hint_y = 1,
+                                    size_hint_max_x = 400,
+                                    pos_hint = {'center_x': .5},
+                                    padding = 5,
+                                    spacing = 20)
+        self.add_widget(self.content)
+
+        self.content.add_widget(e5_label('Provide a name and notes (optional), then record and save.', colors = self.colors))
+
+        self.datum_name = DataGridLabelAndField('Name', colors = self.colors)
+        self.content.add_widget(self.datum_name)
+        self.datum_notes = DataGridLabelAndField('Notes', colors = self.colors)
+        self.content.add_widget(self.datum_notes)
+
+        self.recorder = datum_recorder('Record datum', station = self.station,
+                                        colors = self.colors, setup_type = 'record_new', data = self.data)
+        self.content.add_widget(self.recorder)
+
+        self.results = e5_label('', colors = self.colors)
+        self.content.add_widget(self.results)
+
+        self.content.add_widget(e5_side_by_side_buttons(text = ['Back', 'Save'],
+                                                        id = ['cancel', 'save'],
+                                                        call_back = [self.cancel, self.check_for_duplicate],
+                                                        selected = [False, False],
+                                                        colors = self.colors))
+
+    def check_for_duplicate(self, instance):
+        if self.data.get_datum(self.datum_name.txt.textbox.text).name is not None:
+            message = '\nOverwrite existing datum %s?' % self.datum_name.txt.textbox.text
+            self.popup = e5_MessageBox('Overwrite?', message,
+                                        response_type = "YESNO",
+                                        call_back = [self.delete_and_save, self.close_popup],
+                                        colors = self.colors)
+            self.popup.open()
+        elif self.datum_name.txt.textbox.text == "":
+            self.popup = e5_MessageBox('Error', '\nProvide a datum name before saving.', colors = self.colors)
+            self.popup.open()
+        else:
+            self.save_datum()
 
-    def __init__(self, cfg = None, **kwargs):
-        super(e5_CFGScreen, self).__init__(**kwargs)
-        self.cfg = cfg
+    def delete_and_save(self, instance):
+        self.popup.dismiss()
+        self.data.delete_datum(self.datum_name.txt.texbox.text)
+        self.save_datum()
 
-    def on_pre_enter(self):
-        if self.cfg.filename:
-            try:
-                with open(self.cfg.filename, 'r') as f:
-                    self.content.text = f.read()
-            except OSError:
-                self.content.text = "There was an error reading from the CFG file '%s'" % self.cfg.filename
-        else:
-            self.content.text = '\nOpen a CFG file before trying to view it.'
-        self.content.color = self.colors.text_color
-        self.back_button.background_color = self.colors.button_background
-        self.back_button.color = self.colors.button_color
+    def save_datum(self):
+        error_message = ''
+        if self.datum_name.txt.textbox.text == '':
+            error_message = '\nProvide a datum name.'
+        if self.recorder.result.xyz_global.x is None or self.recorder.result.xyz_global.y is None or self.recorder.result.xyz_global.z is None:
+            error_message = '\nThe point was not properly recorded.  Try again.'
+        if error_message != '':
+            self.popup = e5_MessageBox('Error', error_message, colors = self.colors)
+            self.popup.open()
+            return
 
+        insert_record = {}
+        insert_record['NAME'] = self.datum_name.txt.textbox.text
+        insert_record['NOTES'] = self.datum_notes.txt.textbox.text
+        insert_record['X'] = str(round(self.recorder.result.xyz_global.x, 3))
+        insert_record['Y'] = str(round(self.recorder.result.xyz_global.y, 3))
+        insert_record['Z'] = str(round(self.recorder.result.xyz_global.z, 3))
+        self.data.db.table('datums').insert(insert_record)
+        self.datum_name.txt.textbox.text = ''
+        self.datum_notes.txt.textbox.text = ''
+        self.recorder.result.text = ''
+        self.recorder.result.xyz = None
+        self.recorder.result.xyz_global = None
+        self.data.new_data['datums'] = True
+
+    def close_popup(self, instance):
+        self.popup.dismiss()
 
-class e5_LoadDialog(FloatLayout):
-    start_path = ObjectProperty(None)
-    load = ObjectProperty(None)
-    cancel = ObjectProperty(None)
-    button_color = ObjectProperty(None)
-    button_background = ObjectProperty(None)
-    filters = ObjectProperty(['*.cfg', '*.CFG'])
-
-
-class e5_SaveDialog(BoxLayout):
-    save = ObjectProperty(None)
-    cancel = ObjectProperty(None)
-    start_path = ObjectProperty(None)
-    filename = ObjectProperty(None)
-    path = ObjectProperty(None)
+    def cancel(self, instance):
+        self.parent.current = 'MainScreen'
 
-    def __init__(self, colors = None, **kwargs):
-        super(e5_SaveDialog, self).__init__(**kwargs)
-        self.colors = colors if colors else ColorScheme()
 
-        content = BoxLayout(orientation = 'vertical', padding = 5, spacing = 5)
-        self.pathlabel = e5_textinput(text = self.start_path, background_color = (0, 0, 0, 0), foreground_color = (1, 1, 1, .8), size_hint = (1, None))
-        self.pathlabel.bind(minimum_height = self.pathlabel.setter('height'))
-        content.add_widget(self.pathlabel)
-        self.filesaver = FileChooserListView(path = self.start_path)
-        self.filesaver.bind(selection = self.path_selected)
-        self.filesaver.bind(path = self.path_changed)
-        content.add_widget(self.filesaver)
-
-        self.txt = TextInput(text = self.filename,
-                                multiline = False,
-                                size_hint = (1, None))
-        #                        id = 'filename')
-        self.txt.bind(text = self.update_filename)
-        self.txt.bind(minimum_height = self.txt.setter('height'))
-        content.add_widget(self.txt)
-
-        content.add_widget(e5_side_by_side_buttons(text = ['Cancel', 'Save'],
-                                                    id = ['cancel', 'save'],
-                                                    call_back = [self.cancel, self.does_file_exist],
-                                                    selected = [True, True],
-                                                    colors = self.colors))
+class VerifyStationScreen(Screen):
+    id = ObjectProperty(None)
 
-        self.add_widget(content)
-        self.path = self.start_path
+    def __init__(self, data = None, station = None, ini = None, colors = None, **kwargs):
+        super(VerifyStationScreen, self).__init__(**kwargs)
 
-    def update_filename(self, instance, value):
-        self.filename = value
+        self.colors = colors if colors else ColorScheme()
+        self.station = station
+        self.data = data
+        self.ini = ini
 
-    def path_changed(self, instance, value):
-        self.path = instance.path
-        self.pathlabel.text = instance.path
-
-    def path_selected(self, instance, value):
-        self.path = instance.path
-        self.txt.text = ntpath.split(value[0])[1] if value else ''
-
-    def does_file_exist(self, instance):
-        filename = os.path.join(self.path, self.filename)
-        if os.path.isfile(filename):
-            self.popup = e5_MessageBox('Overwrite existing file?', '\nYou are about to overwrite an existing file - %s.\nContinue?' % filename,
-                                        response_type = "YESNO",
-                                        call_back = [self.overwrite_file, self.close_popup],
-                                        colors = self.colors)
+        self.content = BoxLayout(orientation = 'vertical',
+                                    size_hint_y = 1,
+                                    size_hint_max_x = 400,
+                                    pos_hint={'center_x': .5},
+                                    padding = 5,
+                                    spacing = 20)
+        self.add_widget(self.content)
+
+        # self.content.add_widget(e5_label('Select a datum to use as verification and record it.', colors = self.colors))
+
+        self.datum1 = datum_selector(text = 'Select\nverification\ndatum',
+                                            data = self.data,
+                                            colors = self.colors,
+                                            default_datum = self.data.get_datum(self.ini.get_value('SETUPS', 'VERIFICATION')))
+        self.content.add_widget(self.datum1)
+
+        self.recorder = datum_recorder('Record\nverification\ndatum', station = self.station,
+                                        colors = self.colors, setup_type = 'verify',
+                                        on_record = self.compute_error, data = self.data)
+        self.content.add_widget(self.recorder)
+
+        self.results = e5_label('', colors = self.colors)
+        self.content.add_widget(self.results)
+
+        self.back_button = e5_button(text = 'Back', size_hint_y = None,
+                                        size_hint_x = 1,
+                                        id = 'cancel',
+                                        colors = self.colors, selected = False)
+        self.content.add_widget(self.back_button)
+        self.back_button.bind(on_press = self.close_screen)
+
+    def on_enter(self, *args):
+        if len(self.data.names('datums')) == 0:
+            self.popup = e5_MessageBox('Datums', '\nBefore you can use this option, you need to define some datums.  '
+                                                    'Go to the menu Edit Datums or to Setup Record Datums to add datums.',
+                                        call_back = self.close_popup)
             self.popup.open()
-        else:
-            self.save(self)
+        return super().on_enter(*args)
 
-    def overwrite_file(self, instance):
-        self.popup.dismiss()
-        self.save(instance)
+    def compute_error(self):
+        if not self.datum1.datum.is_none():
+            error = self.station.round_point(self.station.vector_subtract(self.datum1.datum, self.recorder.result.xyz_global))
+            self.results.text = f'\n  X error: {error.x}\n  Y error: {error.y}\n  Z error: {error.z}'
+        else:
+            self.results.text = "Select the name of the verification datum before recording the datum."
 
     def close_popup(self, instance):
         self.popup.dismiss()
+        self.close_screen(instance)
 
+    def close_screen(self, instance):
+        if not self.datum1.datum.is_none():
+            self.ini.update_value('SETUPS', 'VERIFICATION', self.datum1.datum.name)
+            self.ini.save()
+        self.parent.current = 'MainScreen'
 
-class e5_RecordEditScreen(Screen):
-
-    can_update_data_table = False
-    first_field_widget = ObjectProperty(None)
 
-    def __init__(self, data = None,
-                        doc_id = None,
-                        e5_cfg = None,
-                        colors = None,
-                        one_record_only = False,
-                        **kwargs):
-        super(e5_RecordEditScreen, self).__init__(**kwargs)
-        self.colors = colors if colors is not None else ColorScheme()
-        self.e5_cfg = e5_cfg
-        self.data = data
-        self.doc_id = doc_id
-        self.one_record_only = one_record_only
-        self.can_update_data_table = False
-        self.layout = GridLayout(cols = 1,
-                                 size_hint_y = .9,
-                                 size_hint_x = width_calculator(.9, 600),
-                                 spacing = 5,
-                                 padding = 5,
-                                 pos_hint={'center_x': .5, 'center_y': .5})
-        if self.one_record_only:
-            self.record_counter_label = None
-        else:
-            self.record_counter_label = e5_label('Record counter', size_hint = (1, .08), halign = 'center')
-            self.layout.add_widget(self.record_counter_label)
-        self.data_fields = GridLayout(cols = 1, size_hint_y = None, spacing = 5, padding = 5)
-        self.make_empty_frame()
-        scroll = ScrollView(size_hint = (1, 1))
-        scroll.add_widget(self.data_fields)
-        self.layout.add_widget(scroll)
-        if not self.one_record_only:
-            self.layout.add_widget(e5_side_by_side_buttons(text = ['First', 'Previous', 'Next', 'Last'],
-                                                            id = ['first', 'previous', 'next', 'last'],
-                                                            call_back = [self.first_record, self.previous_record,
-                                                                         self.next_record, self.last_record],
-                                                            selected = [True, True, True, True],
-                                                            colors = self.colors))
-            back_and_filter = e5_side_by_side_buttons(text = ['Back', 'Filter'],
-                                                            id = ['back', 'filter'],
-                                                            call_back = [self.call_back, self.filter],
-                                                            selected = [True, True],
-                                                            colors = self.colors)
-            self.filter_button = back_and_filter.children[0]
-            self.layout.add_widget(back_and_filter)
-        else:
-            self.layout.add_widget(e5_side_by_side_buttons(text = ['Save', 'Cancel'],
-                                                            id = ['save', 'cancel'],
-                                                            call_back = [self.save_record, self.cancel_record],
-                                                            selected = [True, True],
-                                                            colors = self.colors))
+class record_button(e5_button):
 
-        self.add_widget(self.layout)
-        self.filter_field = 'Unit-ID'
-        self.loading = True
+    popup = ObjectProperty(None)
+    datum_name = None
 
-    def on_pre_enter(self):
-        self.loading = True
-        if self.data.table is not None and self.e5_cfg is not None:
-            self.reset_doc_ids()
-            self.doc_id = self.doc_ids[-1] if self.doc_ids else None
-        else:
-            self.doc_ids = []
-            self.doc_id = None
-        self.put_data_in_frame()
+    def __init__(self, station = None, result_label = None, setup_type = None, on_record = None,
+                        datum1 = None, datum2 = None, datum3 = None, data = None, **kwargs):
+        super(record_button, self).__init__(**kwargs)
+        # self.colors = colors if colors is not None else ColorScheme()
+        self.station = station
+        self.bind(on_press = self.record_datum)
+        self.result_label = result_label
+        self.setup_type = setup_type
+        self.on_record = on_record
+        self.datum1 = datum1
+        self.datum2 = datum2
+        self.datum3 = datum3
+        self.data = data
+        self.default_prism = prism()
 
-    def on_enter(self):
-        if self.first_field_widget:
-            self.first_field_widget.focus = True
-        self.loading = False
-
-    def on_leave(self):
-        # This helps insure that saving on lost focus works properly
-        # There is an issue this addresses with building the screens
-        # at startup.
-        self.loading = True
-
-    def reset_doc_ids(self):
-        self.doc_ids = [r.doc_id for r in self.data.db.table(self.data.table).all()] if self.data.db is not None else []
-
-    def filter(self, instance):
-        if instance.text == 'Clear Filter':
-            instance.text = 'Filter'
-            self.reset_doc_ids()
-            self.last_record(None)
-            # self.update_record_counter_label()
-        else:
-            self.popup = db_filter(default_field = self.filter_field, fields = ['doc_id', 'Unit-ID'] + self.e5_cfg.fields(),
-                                    colors = self.colors, call_back = self.apply_filter)
-            self.popup.open()
+    def record_datum(self, instance):
+        self.set_angle()
 
-    def get_matching_doc_ids(self, filter_field, filter_value):
-        matches = []
-        if filter_field == 'doc_id':
-            matches = self.data.db.table(self.data.table).get(doc_id = filter_value)
-        elif filter_field == 'Unit-ID':
-            for record in self.data.db.table(self.data.table):
-                if "UNIT" in record.keys() and "ID" in record.keys():
-                    if f"{str(record['UNIT']).lower()}-{str(record['ID']).lower()}" == filter_value.lower():
-                        matches.append(record.doc_id)
+    def get_angle(self):
+        if self.id == 'datum1':
+            if self.setup_type == 'Over a datum + Record a datum':
+                if self.datum1.datum.is_none() or self.datum2.datum.is_none():
+                    return None
+                else:
+                    return self.station.angle_between_points(self.datum1.datum, self.datum2.datum)
+            elif self.setup_type == 'Record two datums':
+                return 0
+        else:
+            return None
+
+    def set_angle(self):
+        angle = self.get_angle()
+        if angle is not None:
+            if self.station.make in ['Manual XYZ', 'Manual VHD']:
+                self.popup = e5_MessageBox('Set horizonal angle',
+                                            f'\nAim at {self.datum1.datum.name} and set the horizontal angle '
+                                                'to {self.station.decimal_degrees_to_sexastr(angle)}.',
+                                            call_back = self.now_take_shot, colors = self.colors)
+                self.popup.open()
+            elif self.station.make in ['Leica', 'Wild', 'Leica GeoCom', 'Sokkia', 'Topcon']:
+                self.popup = self.get_prism_height()
+                self.popup.open()
+                self.station.set_horizontal_angle(self.station.decimal_degrees_to_dddmmss(angle))
+                self.station.take_shot()
         else:
-            for record in self.data.db.table(self.data.table):
-                if str(record[filter_field]).lower() == filter_value.lower():
-                    matches.append(record.doc_id)
-        return(matches)
-
-    def apply_filter(self, instance):
-        self.filter_field = self.popup.fields_dropdown.text
-        filter_value = self.popup.value_input.text
-        if filter_value and self.filter_field:
-            self.doc_ids = self.get_matching_doc_ids(self.filter_field, filter_value)
-            if self.doc_ids:
-                self.first_record(None)
+            if self.station.make in ['Microscribe', 'Manual XYZ', 'Manual VHD']:
+                self.wait_for_shot()
             else:
-                self.clear_the_frame()
-                self.doc_id = None
-                self.update_record_counter_label()
-            self.filter_button.text = 'Clear Filter'
-        else:
-            self.filter_button.text = 'Filter'
-        self.popup.dismiss()
+                self.popup = self.get_prism_height()
+                self.popup.open()
+                self.station.take_shot()
 
-    def make_empty_frame(self):
-        self.data_fields.bind(minimum_height = self.data_fields.setter('height'))
-        self.data_fields.clear_widgets()
-        fields = self.e5_cfg.fields()
-        self.first_field_widget = None
-        if fields:
-            first_field = True
-            for col in fields:
-                field_type = self.e5_cfg.get_value(col, 'TYPE')
-                widget = DataGridLabelAndField(col = col, colors = self.colors, note_field = (field_type == 'NOTE'))
-                self.data_fields.add_widget(widget)
-                if first_field:
-                    if field_type not in ['MENU', 'BOOLEAN']:
-                        self.first_field_widget = widget.txt
-                    first_field = False
-
-    def first_record(self, value):
-        if self.doc_ids:
-            self.doc_id = self.doc_ids[0]
-            self.put_data_in_frame()
-
-    def previous_record(self, value):
-        if self.doc_ids:
-            current = self.doc_ids.index(self.doc_id)
-            new = max(current - 1, 0)
-            self.doc_id = self.doc_ids[new]
-            self.put_data_in_frame()
-
-    def next_record(self, value):
-        if self.doc_ids:
-            current = self.doc_ids.index(self.doc_id)
-            new = min(current + 1, len(self.doc_ids) - 1)
-            self.doc_id = self.doc_ids[new]
-            self.put_data_in_frame()
-
-    def last_record(self, value):
-        if self.doc_ids:
-            self.doc_id = self.doc_ids[-1]
-            self.put_data_in_frame()
-
-    def update_record_counter_label(self):
-        if self.record_counter_label:
-            if self.doc_id:
-                current = self.doc_ids.index(self.doc_id) + 1
-                self.record_counter_label.text = f'Viewing record {current} of {len(self.doc_ids)} (doc_id={self.doc_id})'
-            else:
-                self.record_counter_label.text = 'No matching records'
+    def now_take_shot(self, instance):
+        self.popup.dismiss()
+        self.station.take_shot()
+        self.wait_for_shot()
 
-    def clear_the_frame(self):
-        self.can_update_data_table = False
-        if self.e5_cfg:
-            fields = self.e5_cfg.fields()
-            for widget in self.layout.walk():
-                if hasattr(widget, 'id'):
-                    if widget.id in fields:
-                        widget.text = ''
-
-    def put_data_in_frame(self):
-        self.clear_the_frame()
-        if self.doc_id and self.data.table and self.e5_cfg:
-            data_record = self.data.db.table(self.data.table).get(doc_id = self.doc_id)
-            if data_record:
-                for field in self.e5_cfg.fields():
-                    for widget in self.layout.walk():
-                        if hasattr(widget, 'id'):
-                            if widget.id == field:
-                                widget.text = '%s' % data_record[field] if field in data_record.keys() else ''
-                                # widget.bind(text = self.update_db)
-                                widget.bind(focus = self.show_menu)
-                                break
-        self.can_update_data_table = True
-        self.update_record_counter_label()
-
-    def check_numeric(self, instance, value):
-        cfg_field = self.e5_cfg.get(instance.id)
-        if cfg_field.inputtype in ['NUMERIC', 'INSTRUMENT']:
-            if not self.is_numeric(value):
-                return([f'{instance.id} is listed as a numeric field in the CFG file but the value {value} is not a valid number.'])
-            else:
-                return([])
-        else:
-            return([])
+    def wait_for_shot(self):
+        if self.station.make == 'Microscribe':
+            # self.popup = DataGridTextBox(title = self.text + '.  Waiting on Microscribe...', button_text = ['Cancel', 'Next'], call_back = self.microscribe)
+            self.popup = DataGridTextBox(title = 'EDM',
+                                            label = self.text + '.  Waiting on...',
+                                            text = '<Microscribe>',
+                                            button_text = ['Cancel', 'Next'],
+                                            call_back = self.microscribe,
+                                            colors = self.colors)
+            self.popup.open()
+        elif self.station.make in ['Manual XYZ', 'Manual VHD']:
+            self.popup = edm_manual(call_back = self.have_shot_manual, colors = self.colors)
+            self.popup.open()
 
-    def update_db(self, instance, value):
-        if self.data.table and self.can_update_data_table:
-            update = {instance.id: value}
-            self.data.db.table(self.data.table).update(update, doc_ids = [self.doc_id])
-            self.refresh_linked_fields(instance.id, value)
-            self.data.new_data[self.data.table] = True
+    def have_shot_manual(self, instance):
+        # check that next was pressed and get values
+        p = self.station.text_to_point(f'{self.popup.xcoord.text},{self.popup.ycoord.text},{self.popup.zcoord.text}')
+        if p:
+            self.station.xyz = p
+            self.station.make_global()
+            self.station.vhd_from_xyz()
+        else:
+            self.station.hangle = self.popup.hangle.text if isinstance(self.popup.hangle.text, int) or isinstance(self.popup.hangle.text, float) else ''
+            self.station.vangle = self.popup.vangle.text if isinstance(self.popup.vangle.text, int) or isinstance(self.popup.vangle.text, float) else ''
+            self.station.sloped = self.popup.sloped.text if isinstance(self.popup.sloped.text, int) or isinstance(self.popup.sloped.text, float) else ''
+            self.station.vhd_to_xyz()
+        self.popup.dismiss()
+        self.popup = self.get_prism_height()
+        self.popup.open()
 
-    def refresh_linked_fields(self, fieldname, value):
-        field = self.e5_cfg.get(fieldname)
-        if field.link_fields:
-            linkfields = self.data.get_link_fields(fieldname, value)
-            if linkfields:
-                for widget in self.layout.walk():
-                    if hasattr(widget, 'id'):
-                        if widget.id in linkfields.keys() and widget.id != fieldname:
-                            widget.text = linkfields[widget.id]
-                            widget_field = self.e5_cfg.get(widget.id)
-                            if widget_field.increment:
-                                try:
-                                    widget.text = str(int(widget.text) + 1)
-                                except ValueError:
-                                    pass
-
-    def check_required_fields(self):
-        save_errors = []
-        for field_name in self.e5_cfg.fields():
-            field = self.e5_cfg.get(field_name)
-            if field.required:
-                for widget in self.layout.walk():
-                    if hasattr(widget, 'id'):
-                        if widget.id == field_name:
-                            if widget.text == '':
-                                save_errors.append('The field %s requires a value.' % field_name)
-        return(save_errors)
+    def get_prism_height(self):
+        prism_names = self.data.names('prisms') if self.data else []
+        if len(prism_names) > 0:
+            return DataGridMenuList(title = "Select or Enter a Prism Height",
+                                        menu_list = prism_names,
+                                        menu_selected = self.default_prism.name if self.default_prism.name else '',
+                                        call_back = self.have_shot)
+        else:
+            return DataGridTextBox(title = 'Enter a Prism Height',
+                                        text = str(self.default_prism.height) if self.default_prism.height else '',
+                                        call_back = self.have_shot,
+                                        button_text = ['Back', 'Next'])
 
-    def get_unique_key(self, doc_id):
-        unique_key = []
-        data_record = self.data.db.table(self.data.table).get(doc_id = doc_id)
-        for field in self.e5_cfg.unique_together:
-            unique_key.append("%s" % data_record[field] if field in data_record else '')
-        return(",".join(unique_key))
-
-    def check_unique_together(self):
-        save_errors = []
-        if self.e5_cfg.unique_together and len(self.data.db.table(self.data.table)) > 1:
-            doc_ids = self.data.doc_ids()
-            unique_key = self.get_unique_key(doc_ids[-1])
-            for doc_id in doc_ids[0:-1]:
-                if unique_key == self.get_unique_key(doc_id):
-                    save_errors.append("Based on the unique together field(s) %s, this record's unique key of %s duplicates the record with a doc_id of %s." %
-                                        (",".join(self.e5_cfg.unique_together), unique_key, doc_id))
-                    break
-        return(save_errors)
-
-    def check_numeric_fields(self):
-        save_errors = []
-        for field_name in self.e5_cfg.fields():
-            field = self.e5_cfg.get(field_name)
-            if field.inputtype in ['NUMERIC', 'INSTRUMENT']:
-                for widget in self.layout.walk():
-                    if hasattr(widget, 'id'):
-                        if widget.id == field_name:
-                            if not self.is_numeric(widget.text) and widget.text != '':
-                                save_errors.append('The field %s is marked as numeric but the value entered is not a valid number.' % field_name)
-        return(save_errors)
-
-    def check_bad_characters(self):
-        save_errors = []
-        for field_name in self.e5_cfg.fields():
-            for widget in self.layout.walk():
-                if hasattr(widget, 'id'):
-                    if widget.id == field_name:
-                        if "\"" in widget.text:
-                            save_errors.append('The field %s contains characters that are not recommended in a data file.  These include \" and \\.' % field_name)
-        return(save_errors)
-
-    def save_record(self, instance):
-        save_errors = self.check_required_fields()
-        save_errors += self.check_unique_together()
-        save_errors += self.check_numeric_fields()
-        save_errors += self.check_bad_characters()
-        if hasattr(self.data.db.table(self.data.table), 'on_save') and save_errors == []:
-            save_errors += self.data.db.table(self.data.table).on_save()
-        if not save_errors:
-            self.update_link_fields()
-            self.data.new_data[self.data.table] = True
-            self.parent.current = 'MainScreen'
-        else:
-            self.popup = e5_MessageBox('Save errors',
-                                        '\nCorrect the following errors:\n  ' + '\n  '.join(save_errors),
-                                        response_type = "OK",
-                                        call_back = self.close_popup,
+    def microscribe(self, instance):
+        result = self.popup.result
+        self.popup.dismiss()
+        p = self.station.text_to_point(result)
+        if not p:
+            self.popup = e5_MessageBox(title = 'Error',
+                                        message = '\n Data not formatted correctly.  EDM expects three floating point numbers separated by commas.',
                                         colors = self.colors)
             self.popup.open()
+            return
+        self.station.xyz = self.station.mm_to_meters(p)
+        if self.setup_type == 'verify' or self.setup_type == 'record_new':
+            self.station.make_global()
+        else:
+            self.station.round_xyz()
+        self.have_shot()
 
-    def close_popup(self, instance):
+    def have_shot(self, instance = None):
         self.popup.dismiss()
+        # prism_height = instance.text if not instance.id == 'add_button' else self.popup_textbox.text
+        # if self.station.make in ['Leica', 'Leica GeoCom']:
+        #     self.station.fetch_point()
+        #     self.station.make_global()
+
+        if instance:
+            prism_name = instance.text
+            if prism_name == 'Add' or prism_name == 'Next':
+                try:
+                    self.station.prism = prism(None, float(self.popup.txt.textbox.text), None)
+                except ValueError:
+                    self.station.prism = prism()
+            else:
+                self.station.prism = self.data.get_prism(prism_name)
+        else:
+            self.station.prism = prism(None, 0.0, None)
+        # try:
+        #    if instance:
+        #        self.station.prism = self.data.get_prism(instance.txt)
+        #    else:
+        #        self.station.prism = prism(None, float(self.popup.result), None)
+        # except ValueError:
+        #    self.station.prism = prism(None, 0.0, None)
+        self.default_prism = self.station.prism
+
+        self.event = Clock.schedule_interval(self.check_for_station_response, .1)
+
+    def check_for_station_response(self, dt):
+        if self.station.data_waiting():
+            if self.station.make in ['Leica']:
+                self.station.fetch_point()
+            elif self.station.make in ['Leica GeoCom']:
+                self.station.fetch_point_leica_geocom()
+            elif self.station.make in ['Topcon']:
+                self.station.fetch_point_topcon()
+            if self.station.response:
+                self.station.prism_adjust()
+                if self.station.xyz.x is not None and self.station.xyz.y is not None and self.station.xyz.z is not None:
+                    self.station.make_global()
+                    if self.setup_type == 'verify' or self.setup_type == 'record_new':
+                        self.result_label.text = self.station.point_pretty(self.station.xyz_global)
+                    else:
+                        self.result_label.text = self.station.point_pretty(self.station.xyz)
+                    self.result_label.xyz = self.station.xyz
+                    self.result_label.xyz_global = self.station.xyz_global
+                    if self.on_record is not None:
+                        self.on_record()
+                else:
+                    self.result_label.text = 'Recording error.'
+                    self.result_label.xyz = None
+                    self.result_label.xyz_global = None
+                self.event.cancel()
 
-    def update_link_fields(self):
-        if hasattr(self.e5_cfg, 'link_fields'):
-            for field_name in self.e5_cfg.link_fields:
-                cfg_field = self.e5_cfg.get(field_name)
-                for widget in self.layout.walk():
-                    if hasattr(widget, 'id'):
-                        if widget.id == field_name:
-                            q = Query()
-                            db_rec = self.data.db.table(field_name).search(q[field_name].matches('^' + widget.text + '$', re.IGNORECASE))
-                            if db_rec == []:
-                                self.data.db.table(field_name).insert({field_name: widget.text})
-                                db_rec = self.data.db.table(field_name).search(where(field_name) == widget.text)
-                            for link_field_name in cfg_field.link_fields:
-                                for widget in self.layout.walk():
-                                    if hasattr(widget, 'id'):
-                                        if widget.id == link_field_name:
-                                            if (widget.id == 'ID' and self.is_numeric(widget.text)) or widget.id != 'ID':
-                                                update = {link_field_name: widget.text}
-                                                self.data.db.table(field_name).update(update, doc_ids = [db_rec[0].doc_id])
 
-    def is_numeric(self, value):
-        try:
-            float(value)
-            return(True)
-        except ValueError:
-            return(False)
+class record_result(e5_label):
+    xyz = point()
+    xyz_global = point()
 
-    def cancel_record(self, instance):
-        if hasattr(self.data.db.table(self.data.table), 'on_cancel'):
-            self.data.db.table(self.data.table).on_cancel()
-        self.parent.current = 'MainScreen'
 
-    def show_menu(self, instance, ValueError):
-        if instance.focus and not self.loading:
-            cfg_field = self.e5_cfg.get(instance.id)
-            if cfg_field:
-                self.popup_field_widget = instance
-                if cfg_field.inputtype in ['MENU', 'BOOLEAN']:
-                    self.popup = DataGridMenuList(instance.id, cfg_field.menu,
-                                                    instance.text, self.menu_selection, colors = self.colors)
-                    self.popup.open()
-                    self.popup_scrollmenu = self.get_widget_by_id(self.popup, 'menu_scroll')
-                    self.popup_textbox = self.get_widget_by_id(self.popup, 'new_item')
-                    self.popup_addbutton = self.get_widget_by_id(self.popup, 'add_button')
-        elif not instance.focus and not self.loading:
-            self.update_db(instance, instance.text)
+class datum_recorder(GridLayout):
 
-    def menu_selection(self, instance):
-        self.popup.dismiss()
-        self.popup_field_widget.text = instance.text if not instance.id == 'add_button' else self.popup_textbox.text
-        self.update_db(self.popup_field_widget, self.popup_field_widget.text)
-        if instance.id == 'add_button' and self.popup_field_widget.text.strip() != '':
-            field = self.e5_cfg.get(self.popup_field_widget.id)
-            if self.popup_field_widget.text not in field.menu:
-                field.menu.append(self.popup_field_widget.text)
-                self.e5_cfg.update_value(self.popup_field_widget.id, 'MENU', ','.join(field.menu))
-                self.e5_cfg.save()
-        self.popup_field_widget = None
-        self.popup_scrollmenu = None
-
-    def get_widget_by_id(self, start = None, id = ''):
-        if not start:
-            start = self
-        for widget in start.walk():
-            if hasattr(widget, 'id'):
-                if widget.id == id:
-                    return(widget)
-        return(None)
+    def __init__(self, text = '', datum_no = 1, station = None,
+                        colors = None, setup_type = None,
+                        on_record = None, datum1 = None, datum2 = None, datum3 = None,
+                        data = None, **kwargs):
+        super(datum_recorder, self).__init__(**kwargs)
+        self.padding = 10
+        self.spacing = 10
+        self.colors = colors if colors is not None else ColorScheme()
+        self.station = station
+        self.cols = 2
+        self.results = []
+        self.buttons = []
+        self.size_hint_y = None
+        self.result = record_result('', colors = self.colors, label_height = 100)
+        self.button = record_button(text = text if text else 'Record datum %s' % (datum_no),
+                                    selected = True,
+                                    id = 'datum%s' % (datum_no),
+                                    colors = self.colors,
+                                    station = self.station,
+                                    result_label = self.result,
+                                    setup_type = setup_type,
+                                    on_record = on_record,
+                                    datum1 = datum1,
+                                    datum2 = datum2,
+                                    datum3 = datum3,
+                                    data = data)
+        self.add_widget(self.button)
+        self.add_widget(self.result)
 
-    def call_back(self, value):
-        self.parent.current = 'MainScreen'
 
+class datum_selector(GridLayout):
 
-class e5_DatagridScreen(Screen):
+    datum = None
+    popup = ObjectProperty(None)
+    popup_open = False
 
-    datagrid = ObjectProperty(None)
+    def __init__(self, text = '',
+                        data = None, colors = None, default_datum = None,
+                        call_back = None,
+                        id = None,
+                        **kwargs):
+        super(datum_selector, self).__init__(**kwargs)
+        # self.orientation = 'horizontal'
+        self.padding = 10
+        self.spacing = 10
+        self.cols = 2
+        self.colors = colors
+        self.data = data
+        self.datum = default_datum
+        self.call_back = call_back
+        self.size_hint_y = None
+        self.add_widget(e5_button(text = text,
+                                    selected = True,
+                                    call_back = self.show_select_datum,
+                                    colors = self.colors))
+        if not self.datum.is_none():
+            self.result = e5_label(f'Datum: {self.datum.name}\nX: {self.datum.x}\nY: {self.datum.y}\nZ: {self.datum.z}',
+                                    colors = self.colors, label_height = 100)
+        else:
+            self.result = e5_label('Datum:\nX:\nY:\nZ:', colors = self.colors)
+        self.add_widget(self.result)
+
+    def show_select_datum(self, instance):
+        self.popup = DataGridMenuList(title = "Datum",
+                                        menu_list = self.data.names('datums'),
+                                        menu_selected = '',
+                                        call_back = self.datum_selected,
+                                        colors = self.colors)
+        self.popup.open()
 
-    def __init__(self, main_data = None, main_tablename = '_default', main_cfg = None, colors = None, addnew = False, **kwargs):
-        super(e5_DatagridScreen, self).__init__(**kwargs)
-        self.colors = colors if colors else ColorScheme()
+    def datum_selected(self, instance):
+        self.popup.dismiss()
+        self.datum = self.data.get_datum(instance.text)
+        if not self.datum.is_none():
+            self.result.text = f'Datum: {self.datum.name}\nX: {self.datum.x}\nY: {self.datum.y}\nZ: {self.datum.z}'
+            if self.call_back:
+                self.call_back(self)
+        else:
+            self.result.text = 'Search error'
 
-        if platform_name() == 'Android':
-            self.colors.datagrid_font_size = "11sp"
 
-        self.e5_data = main_data
-        self.e5_cfg = main_cfg
-        self.tablename = main_tablename
+class setups(ScrollView):
 
-        self.datagrid = DataGridWidget(data = main_data.db.table(main_tablename) if self.e5_data.db is not None and main_tablename else None,
-                                        cfg = self.e5_cfg,
-                                        colors = self.colors,
-                                        addnew = addnew)
-        self.add_widget(self.datagrid)
-        if main_data.db is not None:
-            if main_data.db.tables:
-                self.datagrid.data = main_data.db.table(main_tablename)
-                self.datagrid.fields = main_cfg
+    id = ObjectProperty(None)
+    popup = ObjectProperty(None)
+    popup_open = False
+    recorder = []
 
-    def on_pre_enter(self):
-        if self.e5_data is not None:
-            if self.tablename in self.e5_data.new_data:
-                if self.e5_data.new_data[self.tablename]:
-                    self.datagrid.data = self.e5_data.db.table(self.tablename)
-                    self.datagrid.fields = self.e5_cfg
-                    self.datagrid.reload_data()
-                    self.e5_data.new_data[self.tablename] = False
+    def __init__(self, setup_type, data = None, ini = None, station = None, colors = None, **kwargs):
+        super(setups, self).__init__(**kwargs)
 
-    def on_enter(self):
-        Window.bind(on_key_down = self._on_keyboard_down)
-        if self.datagrid:
-            self.datagrid.switch_to(self.datagrid.tab_list[len(self.datagrid.tab_list) - 1])
-
-    def _on_keyboard_down(self, *args):
-        ascii_code = args[1]
-        # text_str = args[3]
-        if ascii_code in [273, 274, 275, 276, 278, 279] and self.datagrid.popup_scrollmenu:
-            self.datagrid.popup_scrollmenu.move_scroll_menu_item(ascii_code)
-            return False
-        elif ascii_code == 13 and (self.datagrid.popup_scrollmenu or self.datagrid.popup_textbox):
-            if self.datagrid.popup_textbox.focus:
-                self.datagrid.popup_addbutton.trigger_action(0)
-            elif self.datagrid.popup_scrollmenu:
-                self.datagrid.popup_scrollmenu.menu_selected_widget.trigger_action(0)
-        elif ascii_code == 13:
-            return False
-        elif ascii_code == 8:
-            return False
-        elif ascii_code == 27 and (self.datagrid.popup_scrollmenu or self.datagrid.popup_textbox):
-            self.datagrid.popup_scrollmenu = None
-            self.datagrid.popup_textbox = None
-            self.datagrid.popup.dismiss()
-        # TODO On key down, see if there is a current record,
-        # get the next record in the db,
-        # and then try to fire the highlight record stuff
-        return True
-
-    def on_leave(self):
-        Window.unbind(on_key_down = self._on_keyboard_down)
-
-
-class e5_MessageBox(Popup):
-    def __init__(self, title, message,
-                    response_type = 'OK',
-                    response_text = None,
-                    call_back = None,
-                    colors = None, **kwargs):
-        super(e5_MessageBox, self).__init__(**kwargs)
-        self.widget_with_focus = None
-        popup_contents = GridLayout(cols = 1, spacing = 5)
-        popup_contents.add_widget(e5_scrollview_label(message, popup = True, colors = colors))
-        if not call_back:
-            call_back = self.dismiss
-        if response_type == 'OK':
-            self.widget_with_focus = e5_button('OK',
-                                                call_back = call_back,
-                                                selected = True,
-                                                button_height = .2,
-                                                colors = colors)
-            self.widget_with_focus.bind(on_key_up = self.keystroke)
-            popup_contents.add_widget(self.widget_with_focus)
-        elif response_type == 'CANCEL':
-            popup_contents.add_widget(e5_button('CANCEL',
-                                                call_back = call_back,
-                                                selected = True,
-                                                button_height = .2,
-                                                colors = colors))
-        elif response_type == 'YESNO':
-            popup_contents.add_widget(e5_side_by_side_buttons(text = ['Yes', 'No'],
-                                                                call_back = call_back,
-                                                                selected = [False, False],
-                                                                button_height = .2,
-                                                                colors = colors))
-        elif response_type == 'YESNOCANCEL':
-            popup_contents.add_widget(e5_side_by_side_buttons(text = ['Yes', 'No', 'Cancel'],
-                                                                call_back = call_back,
-                                                                selected = [True, True, True],
-                                                                button_height = .2,
-                                                                colors = colors))
-        else:
-            popup_contents.add_widget(e5_side_by_side_buttons(text = response_text,
-                                                                call_back = call_back,
-                                                                selected = [True, True],
-                                                                button_height = .2,
-                                                                colors = colors))
-
-        self.title = title
-        self.content = popup_contents
-        self.size_hint = (.8, .8)
-        self.size = (400, 400)
-        self.auto_dismiss = False
-
-    def on_open(self):
-        if self.widget_with_focus:
-            self.widget_with_focus.focus = True
-        Window.bind(on_key_up = self.keystroke)
-
-    def on_dismiss(self):
-        Window.unbind(on_key_up = self.keystroke)
-
-    def keystroke(self, key, scancode, codepoint):
-        if scancode == 13 and self.widget_with_focus:
-            self.widget_with_focus.trigger_action()
-
-
-# region Data Grid
-# Code from https://github.com/MichaelStott/DataframeGUIKivy/blob/master/dfguik.py
-
-class DataGridMenuList(Popup):
-
-    def __init__(self, title, menu_list, menu_selected = '', call_back = None, colors = None, **kwargs):
-        super(DataGridMenuList, self).__init__(**kwargs)
-
-        pop_content = GridLayout(cols = 1, size_hint_y = 1, spacing = 5, padding = 5)
-
-        new_item = GridLayout(cols = 2, spacing = 5, size_hint_y = None)
-        new_item_left = GridLayout(cols = 1, spacing = 5, size_hint_y = None)
-        if menu_list:
-            new_item_instructions_text = 'Enter a new menu item and press add or select from the menu below.  New menu items are saved in the CFG.'
-        else:
-            new_item_instructions_text = 'Enter a new menu item and press add.  New menu items are saved in the CFG.'
-        new_item_instructions = e5_label(new_item_instructions_text, popup = True, text_size = (self.width * 2, None))
-        new_item_left.add_widget(new_item_instructions)
-        self.txt = e5_textinput(id = 'new_item', size_hint_y = None)
-        self.txt.bind(minimum_height = self.txt.setter('height'))
-        if colors:
-            if colors.text_font_size:
-                self.txt.font_size = colors.text_font_size
-        new_item_left.add_widget(self.txt)
-        new_item.add_widget(new_item_left)
-        self.add_button = e5_button('Add',
-                                    id = 'add_button',
-                                    selected = True,
-                                    call_back = call_back,
-                                    button_height = .15,
-                                    colors = colors)
-        new_item.add_widget(self.add_button)
-        # new_item.bind(minimum_height = new_item.setter('height'))
-        pop_content.add_widget(new_item)
-
-        ncols = int(Window.width / 200)
-        if ncols < 1:
-            ncols = 1
-
-        self.menu = None
-        if menu_list:
-            self.menu = e5_scrollview_menu(menu_list, menu_selected,
-                                                    widget_id = 'menu',
-                                                    call_back = [call_back],
-                                                    ncols = ncols,
-                                                    colors = colors)
-            pop_content.add_widget(self.menu)
-            self.menu.make_scroll_menu_item_visible()
-
-        pop_content.add_widget(e5_button('Back', selected = True,
-                                                 call_back = self.dismiss,
-                                                 colors = colors))
-
-        self.content = pop_content
-
-        self.title = title
-        self.size_hint = (.9, .9 if menu_list else .33)
-        self.auto_dismiss = True
-        self.call_back = call_back
+        self.colors = colors if colors is not None else ColorScheme()
+        self.data = data
+        self.station = station
+        self.ini = ini
+        self.recorder = []
+        self.bar_width = 10
 
-    def on_open(self):
-        self.txt.focus = True
-        self.txt.select_all()
-        Window.bind(on_key_down = self._on_keyboard_down)
-
-    def _on_keyboard_down(self, *args):
-        ascii_code = args[1]
-        if ascii_code == 13 and self.txt.focus and self.txt.text != "":
-            self.call_back(self.add_button)
-        elif ascii_code == 13:
-            if self.menu:
-                if self.menu.scroll_menu_get_selected():
-                    self.call_back(self.menu.scroll_menu_get_selected())
-        elif self.menu:
-            self.menu.move_scroll_menu_item(ascii_code)
+        self.scrollbox = GridLayout(cols = 1,
+                                    size_hint = (1, None),
+                                    spacing = 5)
+        self.scrollbox.bind(minimum_height = self.scrollbox.setter('height'))
 
-    def on_dismiss(self):
-        Window.unbind(on_key_down = self._on_keyboard_down)
+        instructions = Label(color = self.colors.text_color,
+                             size_hint_y = None,
+                             font_size = self.colors.text_font_size if self.colors.text_font_size else 12)
+
+        if setup_type == "Horizontal Angle Only":
+            instructions.text = '\nEnter the horizontal angle to uploaded to the station.'
+            self.scrollbox.add_widget(instructions)
+
+            # content1 = GridLayout(cols = 2, padding = 10, size_hint_y = None)
+            # content1.add_widget(e5_label('Angle (ddd.mmss)', colors = self.colors))
+            # self.hangle = e5_textinput(text = '', multiline = False)
+            # content1.add_widget(self.hangle)
+            # self.scrollbox.add_widget(content1)
+
+            widget = DataGridLabelAndField(col = '', prompt = 'Angle (ddd.mmss)',
+                                            colors = self.colors,
+                                            text_length = 8, padding = 5)
+            self.hangle = widget.txt.textbox
+            self.scrollbox.add_widget(widget)
+
+            content2 = GridLayout(cols = 1, padding = 5, size_hint_y = None)
+            content2.add_widget(e5_button(text = 'Upload angle', selected = True,
+                                call_back = self.set_hangle, colors = self.colors))
+            self.scrollbox.add_widget(content2)
+
+        elif setup_type == "Over a datum":
+            instructions.text = '\nUse this option when the station is setup over a known point and you can measure the station height '\
+                                'or to set the station location directly (with no station height).  Note this option assumes the horizontal '\
+                                'angle is already correct or will be otherwise set.'
+            self.scrollbox.add_widget(instructions)
+
+            self.over_datum = datum_selector(text = 'Select a datum',
+                                                data = self.data,
+                                                colors = self.colors,
+                                                default_datum = self.data.get_datum(self.ini.get_value('SETUPS', 'OVERDATUM')))
+            self.scrollbox.add_widget(self.over_datum)
+
+            # content2 = GridLayout(cols = 2, padding = 10, size_hint_y = None)
+            # content2.add_widget(e5_label('Station height (optional)'))
+            # self.station_height = TextInput(text = '', multiline = False,
+            #                                 size_hint_max_y = 30)
+
+            widget = DataGridLabelAndField(col = '', prompt = 'Height (optional)',
+                                            colors = self.colors,
+                                            text_length = 8, padding = 5, spacing = 20)
+            self.station_height = widget.txt.textbox
+            # content2.add_widget(self.station_height)
+
+            self.scrollbox.add_widget(widget)
+
+        elif setup_type == "Over a datum + Record a datum":
+            instructions.text = "\nSelect the datum under the station and a datum to recorded.  "\
+                                "EDM will automatically set the correct horizontal angle and compute the station's XYZ coordinates."
+            self.scrollbox.add_widget(instructions)
+
+            self.datum1 = datum_selector(text = 'Select datum\nunder the\nstation',
+                                                data = self.data,
+                                                colors = self.colors,
+                                                default_datum = self.data.get_datum(self.ini.get_value('SETUPS', 'OVERDATUM')))
+            self.scrollbox.add_widget(self.datum1)
+
+            self.datum2 = datum_selector(text = 'Select datum\nto record',
+                                                data = self.data,
+                                                colors = self.colors,
+                                                default_datum = self.data.get_datum(self.ini.get_value('SETUPS', 'RECORDDATUM')),
+                                                call_back = self.datum1_selected)
+            self.scrollbox.add_widget(self.datum2)
+
+            datum_name = self.data.get_datum(self.ini.get_value('SETUPS', 'RECORDDATUM'))
+            datum_name = f'Record\n{datum_name.name}' if datum_name else 'Record datum 1'
+            self.recorder.append(datum_recorder(datum_name, station = self.station, colors = self.colors,
+                                                setup_type = setup_type, datum1 = self.datum1, datum2 = self.datum2,
+                                                data = self.data))
+            self.scrollbox.add_widget(self.recorder[0])
+
+        elif setup_type == "Record two datums":
+            instructions.text = "\nSelect two datums to record. EDM will use triangulation to compute the station's XYZ coordinates.  "\
+                                "Always record datum one first and then datum two.  When you record datum one, the horizontal angle will "\
+                                "be set to 0.0.  When you accept the setup, the horizontal angle will be reset correctly on datum 2."
+            self.scrollbox.add_widget(instructions)
+
+            self.datum1 = datum_selector(text = 'Select\ndatum\none',
+                                                data = self.data,
+                                                colors = self.colors,
+                                                default_datum = self.data.get_datum(self.ini.get_value('SETUPS', '2DATUMS_DATUM_1')),
+                                                call_back = self.datum1_selected)
+            self.scrollbox.add_widget(self.datum1)
+
+            self.datum2 = datum_selector(text = 'Select\ndatum\ntwo',
+                                                data = self.data,
+                                                colors = self.colors,
+                                                default_datum = self.data.get_datum(self.ini.get_value('SETUPS', '2DATUMS_DATUM_2')),
+                                                call_back = self.datum2_selected)
+            self.scrollbox.add_widget(self.datum2)
+
+            for n in range(2):
+                datum_name = self.data.get_datum(self.ini.get_value('SETUPS', '2DATUMS_DATUM_%s' % (n + 1)))
+                datum_name = f'Record\n{datum_name.name}' if datum_name else f'Record datum {n + 1}'
+                self.recorder.append(datum_recorder(datum_name, datum_no = n + 1, station = station, colors = colors,
+                                                    setup_type = setup_type, datum1 = self.datum1, datum2 = self.datum2, data = self.data))
+                self.scrollbox.add_widget(self.recorder[n])
+
+        elif setup_type == "Three datum shift":
+            instructions.text = "\nThis option is designed to let one grid be rotated into another and is best for when a block of "\
+                                "sediment is being excavated in a lab.  It requires three datums points."
+            self.scrollbox.add_widget(instructions)
+
+            self.datum1 = datum_selector(text = 'Select datum 1',
+                                                data = self.data,
+                                                colors = self.colors,
+                                                default_datum = self.data.get_datum(self.ini.get_value('SETUPS', '3DATUM_SHIFT_GLOBAL_1')),
+                                                call_back = self.datum1_selected)
+            self.scrollbox.add_widget(self.datum1)
+
+            self.datum2 = datum_selector(text = 'Select datum 2',
+                                                data = self.data,
+                                                colors = self.colors,
+                                                default_datum = self.data.get_datum(self.ini.get_value('SETUPS', '3DATUM_SHIFT_GLOBAL_2')),
+                                                call_back = self.datum2_selected)
+            self.scrollbox.add_widget(self.datum2)
+
+            self.datum3 = datum_selector(text = 'Select datum 3',
+                                                data = self.data,
+                                                colors = self.colors,
+                                                default_datum = self.data.get_datum(self.ini.get_value('SETUPS', '3DATUM_SHIFT_GLOBAL_3')),
+                                                call_back = self.datum3_selected)
+            self.scrollbox.add_widget(self.datum3)
+
+            for n in range(3):
+                datum_name = self.data.get_datum(self.ini.get_value('SETUPS', '3DATUM_SHIFT_GLOBAL_%s' % (n + 1)))
+                datum_name = f'Record {datum_name.name}' if datum_name else f'Record datum {n + 1}'
+                self.recorder.append(datum_recorder(datum_name, datum_no = n + 1, station = station,
+                                                                colors = self.colors, setup_type = setup_type))
+                self.scrollbox.add_widget(self.recorder[n])
+
+        instructions.bind(texture_size = lambda instance, value: setattr(instance, 'height', value[1]))
+        instructions.bind(width = lambda instance, value: setattr(instance, 'text_size', (value * .95, None)))
+
+        self.size_hint = (1, .9)
+        # self.size = (Window.width, Window.height / 2)
+        self.id = 'setup_scroll'
+        self.add_widget(self.scrollbox)
 
+        def draw_background(widget, prop):
+            with widget.canvas.before:
+                Color(0.8, 0.8, 0.8, 1)
+                Rectangle(size=self.size, pos=self.pos)
 
-class DataGridTextInput(TextInput):
+        # self.bind(size = draw_background)
+        # self.bind(pos = draw_background)
 
-    id = ObjectProperty(None)
+    def datum1_selected(self, instance):
+        self.recorder[0].children[1].text = 'Record ' + instance.datum.name
+        self.recorder[0].children[1].datum_name = instance.datum.name
 
-    def __init__(self, call_back = None, **kwargs):
-        super(DataGridTextInput, self).__init__(**kwargs)
-        self.call_back = call_back
+    def datum2_selected(self, instance):
+        self.recorder[1].children[1].text = 'Record ' + instance.datum.name
+        self.recorder[1].children[1].datum_name = instance.datum.name
 
-    def keyboard_on_key_up(self, window, keycode):
-        # print(keycode)
-        return super(DataGridTextInput, self).keyboard_on_key_up(window, keycode)
+    def datum3_selected(self, instance):
+        self.recorder[2].children[1].text = 'Record ' + instance.datum.name
+        self.recorder[2].children[1].datum_name = instance.datum.name
 
+    def set_hangle(self, instance):
+        if self.hangle:
+            self.station.set_horizontal_angle(self.hangle.text)
+            logger = logging.getLogger(__name__)
+            logger.info(f'Horizontal angle set to {self.hangle.text}')
 
-class DataGridTextBox(Popup):
 
-    result = ObjectProperty(None)
-    save_button = ObjectProperty(None)
+class InitializeStationScreen(Screen):
 
-    def __init__(self, title, label = None, text = '', multiline = False, call_back = None,
-                        button_text = ['Back', 'Save'], colors = None, **kwargs):
-        super(DataGridTextBox, self).__init__(**kwargs)
-        self.colors = colors if colors else ColorScheme()
-        content = GridLayout(cols = 1, spacing = 5, padding = 10)
-        if label:
-            # e5_label(text = col, id = '__label', colors = colors)
-            # content.add_widget(Label(text = label, text_size = (None, 30)))
-            content.add_widget(e5_label(text = label, colors = self.colors, popup = True))
-        self.txt = DataGridTextInput(text = text, size_hint_y = None, height = 30 if not multiline else 90,
-                                        multiline = multiline, id = 'new_item')
-        if self.colors:
-            if self.colors.text_font_size:
-                self.txt.font_size = self.colors.text_font_size
-            if not multiline:
-                if self.colors.text_font_size:
-                    self.txt.height = int(self.colors.text_font_size.replace('sp', '')) * 1.8
-        self.result = text
-        self.txt.bind(text = self.update)
-        self.txt.bind(on_text_validate = self.accept_value)
-        content.add_widget(self.txt)
-        buttons = e5_side_by_side_buttons(button_text,
-                                            button_height = None,
-                                            id = [title, 'add_button'],
-                                            selected = [True, True],
-                                            call_back = [self.dismiss, call_back],
-                                            colors = self.colors)
-        self.save_button = buttons.children[0]
-        content.add_widget(buttons)
-        self.title = title
-        self.content = content
-        if not multiline:
-            self.size_hint = (width_calculator(.8, 800), .35 if label is None else .5)
-        else:
-            self.size_hint = (width_calculator(.8, 800), .45 if label is None else .6)
-        self.auto_dismiss = True
-
-        self.event = Clock.schedule_once(self.set_focus, .35)
-
-    def set_focus(self, instance):
-        self.txt.focus = True
-        self.txt.select_all()
-
-    def on_open(self):
-        self.txt.focus = True
-        self.txt.select_all()
-
-    def update(self, instance, value):
-        self.result = value
-
-    def accept_value(self, instance):
-        self.save_button.trigger_action(0)
-
-
-class DataGridHeaderCell(Button):
-    def __init__(self, text, colors, **kwargs):
-        super(DataGridHeaderCell, self).__init__(**kwargs)
-        self.background_color = colors.button_background
-        self.background_normal = ''
-        self.color = colors.button_color
-        self.text = text
-        if colors.datagrid_font_size:
-            self.font_size = colors.datagrid_font_size
-
-
-class DataGridTableHeader(ScrollView):
-    """Fixed table header that scrolls x with the data table"""
-    header = ObjectProperty(None)
-
-    def __init__(self, titles = None, colors = None, *args, **kwargs):
-        super(DataGridTableHeader, self).__init__(*args, **kwargs)
-
-        for title in titles:
-            self.header.add_widget(DataGridHeaderCell(title, colors))
-
-
-class DataGridScrollCell(Button):
-    text = StringProperty(None)
-    is_even = BooleanProperty(None)
-    # datagrid_even = ListProperty(None)
-    # datagrid_odd = ListProperty(None)
-    datagrid_even = [189.0 / 255, 189.0 / 255, 189.0 / 255, 1]
-    datagrid_odd = [224.0 / 255, 224.0 / 255, 224.0 / 255, 1]
-
-    def __init__(self, **kwargs):
-        super(DataGridScrollCell, self).__init__(**kwargs)
-        self.background_normal = ''
+    def __init__(self, data = None, station = None, ini = None, colors = None, **kwargs):
+        super(InitializeStationScreen, self).__init__(**kwargs)
 
+        self.colors = colors if colors else ColorScheme()
+        self.station = station
+        self.data = data
+        self.ini = ini
 
-class DataGridTableData(RecycleView):
-    nrows = NumericProperty(None)
-    ncols = NumericProperty(None)
-    rgrid = ObjectProperty(None)
+        lastsetup_type = self.ini.get_value('SETUPS', 'LASTSETUP_TYPE')
+        self.setup = lastsetup_type if lastsetup_type else 'Horizontal Angle Only'
 
-    datagrid_doc_id = None
-    datagrid_background_color = None
-    # datagrid_widget_row = []
+        self.content = BoxLayout(orientation = 'vertical',
+                                    size_hint_y = 1,
+                                    size_hint_max_x = MAX_SCREEN_WIDTH,
+                                    pos_hint = {'center_x': .5, 'center_y': .5},
+                                    padding = 5,
+                                    spacing = 5)
+        self.add_widget(self.content)
 
-    datatable_widget = None
+        setup_type_box = GridLayout(cols = 2,
+                                    size_hint_y = None,
+                                    pos_hint = {'center_x': .5, 'center_y': .5})
 
-    popup = ObjectProperty(None)
+        spinner_dropdown_button = SpinnerOptions
+        spinner_dropdown_button.font_size = colors.button_font_size.replace("sp", '') if colors.button_font_size else None
+        spinner_dropdown_button.background_color = (0, 0, 0, 1)
 
-    def __init__(self, list_dicts=[], column_names = None, tb = None, e5_cfg = None, colors = None, *args, **kwargs):
-        self.nrows = len(list_dicts) if len(list_dicts) != 1 else 2
-        self.ncols = len(column_names)
-        self.id = 'datatable'
-        self.colors = colors if colors else ColorScheme()
-        self.e5_cfg = e5_cfg
+        self.setup_type = Spinner(text = self.setup,
+                                    values=["Horizontal Angle Only",
+                                            "Over a datum",
+                                            "Over a datum + Record a datum",
+                                            "Record two datums",
+                                            "Three datum shift"],
+                                    option_cls = spinner_dropdown_button)
+        if colors.button_font_size:
+            self.setup_type.font_size = colors.button_font_size
+        setup_type_box.add_widget(self.setup_type)
+        self.setup_type.bind(text = self.rebuild)
+        self.content.add_widget(setup_type_box)
+
+        self.scroll_content = BoxLayout(orientation = 'vertical',
+                                        size_hint = (1, .9),
+                                        spacing = 5, padding = 5)
 
-        super(DataGridTableData, self).__init__(*args, **kwargs)
+        self.content.add_widget(self.scroll_content)
 
-        self.data = []
-        black = make_rgb(BLACK)
-        if len(list_dicts) == 1:
-            # This is a hack to deal with a Kivy but where the grid does not display if there is
-            # only one row.  So the solution is to insert a dummy row.
-            for column in column_names:
-                self.data.append({'text': '',
-                                    'is_even': False,
-                                    'callback': self.editcell,
-                                    'key': 0,
-                                    'field': column,
-                                    'db': tb,
-                                    'id': 'datacell',
-                                    'datagrid_even': self.colors.datagrid_even,
-                                    'datagrid_odd': self.colors.datagrid_odd,
-                                    'color': black})
-        for i, ord_dict in enumerate(list_dicts):
-            is_even = i % 2 == 0
-            for column in column_names:
-                value = ord_dict[column] if column in ord_dict.keys() else ''
-                content = {'text': value,
-                            'is_even': is_even,
-                            'callback': self.editcell,
-                            'key': ord_dict['doc_id'],
-                            'field': column,
-                            'db': tb,
-                            'id': 'datacell',
-                            'datagrid_even': self.colors.datagrid_even,
-                            'datagrid_odd': self.colors.datagrid_odd,
-                            'color': black}
-                if self.colors.datagrid_font_size:
-                    content['font_size'] = self.colors.datagrid_font_size
-                self.data.append(content)
-
-    def clear_highlight_row(self):
-        if self.datagrid_doc_id:
-            for record in self.data:
-                if record['key'] == self.datagrid_doc_id:
-                    if 'background_color' in record:
-                        del record['background_color']
-            self.refresh_from_data()
-            # for widget in self.get_editcell_row(self.datagrid_doc_id):
-            #    widget.background_color = self.datagrid_background_color
-            self.datagrid_doc_id = ''
-            # self.datagrid_widget_row = []
-
-    def set_highlight_row(self):
-        # if self.datagrid_doc_id:
-        #    widget_row = self.get_editcell_row(self.datagrid_doc_id)
-        #    for widget in widget_row:
-        #        widget.background_color = self.colors.optionbutton_background
-        #   self.datagrid_widget_row = widget_row
-        for record in self.data:
-            if record['key'] == self.datagrid_doc_id:
-                record['background_color'] = self.colors.optionbutton_background
-        self.refresh_from_data()
-
-    # def get_editcell_row(self, key):
-    #    row_widgets = []
-    #    for widget in self.walk():
-    #        if hasattr(widget, 'id'):
-    #            if widget.id == 'datacell':
-    #                if widget.key == key:
-    #                    row_widgets.append(widget)
-    #    return(row_widgets)
+        self.setup_widgets = setups(self.setup_type.text,
+                                    data = self.data,
+                                    ini = self.ini,
+                                    station = self.station,
+                                    colors = self.colors)
+        self.scroll_content.add_widget(self.setup_widgets)
 
-    def get_editcell(self, key, field):
-        for widget in self.walk():
-            if hasattr(widget, 'id'):
-                if widget.id == 'datacell':
-                    if widget.field == field and widget.key == key:
-                        return(widget)
-        return(None)
-
-    def editcell(self, key, field, db):
-        # self.key = key
-        if field == 'doc_id' and self.datagrid_doc_id == key:
-            self.clear_highlight_row()
-            return
-        self.clear_highlight_row()
-        self.datagrid_doc_id = key
-        editcell_widget = self.get_editcell(key, field)
-        self.datagrid_background_color = editcell_widget.background_color
-        self.set_highlight_row()
-        self.field = field
-        self.tb = db
-        cfg_field = self.e5_cfg.get(field)
-        self.inputtype = cfg_field.inputtype.upper()
-        if self.inputtype in ['MENU', 'BOOLEAN']:
-            self.popup = DataGridMenuList(field, cfg_field.menu, editcell_widget.text, self.menu_selection, self.colors)
-            self.popup.open()
-        if self.inputtype in ['TEXT', 'NUMERIC', 'NOTE']:
-            self.popup = DataGridTextBox(title = field, text = editcell_widget.text,
-                                            multiline = self.inputtype == 'NOTE',
-                                            call_back = self.menu_selection,
-                                            colors = self.colors)
-            self.popup.open()
-        self.datatable_widget.popup_scrollmenu = self.datatable_widget.get_widget_by_id(self.popup, 'menu_scroll')
-        self.datatable_widget.popup_textbox = self.datatable_widget.get_widget_by_id(self.popup, 'new_item')
-        self.datatable_widget.popup_addbutton = self.datatable_widget.get_widget_by_id(self.popup, 'add_button')
-        self.datatable_widget.popup = self.popup
+        self.content.add_widget(e5_side_by_side_buttons(text = ['Back', 'Accept Setup'],
+                                                        id = ['back', 'accept'],
+                                                        call_back = [self.go_back, self.accept_setup],
+                                                        selected = [False, False],
+                                                        colors = self.colors))
+
+    def rebuild(self, instance, value):
+        self.setup = value
+        self.scroll_content.clear_widgets()
+        self.setup_widgets = setups(self.setup_type.text,
+                                                data = self.data,
+                                                ini = self.ini,
+                                                station = self.station,
+                                                colors = self.colors)
+        self.scroll_content.add_widget(self.setup_widgets)
+        if value not in ['Horizontal Angle Only']:
+            if len(self.data.names('datums')) == 0:
+                self.popup = e5_MessageBox('Datums', '\nBefore you can use this option, you need to define some datums.  '
+                                                    'Go to the menu Edit Datums or to Setup Record Datums to add datums.',
+                                            call_back = self.close_popup)
+                self.popup.open()
 
-    def menu_selection(self, instance):
-        self.popup.dismiss()
-        if self.inputtype in ['MENU', 'BOOLEAN']:
-            new_data = {self.field: instance.text if not instance.text == 'Add' else self.datatable_widget.popup_textbox.text}
-        elif self.inputtype == 'NUMERIC':
-            try:
-                if '.' in self.datatable_widget.popup_textbox.text:
-                    new_data = {self.field: float(self.datatable_widget.popup_textbox.text)}
-                else:
-                    new_data = {self.field: int(self.datatable_widget.popup_textbox.text)}
-            except ValueError:
-                new_data = {self.field: self.datatable_widget.popup_textbox.text}
-        else:
-            new_data = {self.field: self.datatable_widget.popup_textbox.text}
-        is_valid = self.e5_cfg.validate_datafield(new_data, self.tb)
-        if is_valid is True:
-            self.tb.update(new_data, doc_ids = [int(self.datagrid_doc_id)])
-            self.update_recycle_data(self.datagrid_doc_id, self.field, new_data[self.field])
-            # for widget in self.walk():
-            #    if hasattr(widget, 'id'):
-            #        if widget.id == 'datacell':
-            #            if widget.key == self.datagrid_doc_id and widget.field == self.field:
-            #                widget.text = str(new_data[self.field])
-            self.datatable_widget.popup_scrollmenu = None
-            self.datatable_widget.popup_textbox = None
-        else:
-            self.popup = e5_MessageBox('Data error', is_valid)
-            self.popup.open()
+    def go_back(self, instance):
+        self.ini.update_value(APP_NAME, 'LASTSETUP_TYPE', self.setup_type.text)
+        self.parent.current = 'MainScreen'
 
-    def update_recycle_data(self, doc_id, field, value):
-        for record in self.data:
-            if record['key'] == doc_id and record['field'] == field:
-                record['text'] = str(value)
-                self.refresh_from_data()
-                break
+    def accept_setup(self, instance):
 
+        self.new_station = point()
+        self.foresight = None
+        txt = ''
+        error_message = ''
+
+        if self.setup_type.text == 'Horizontal Angle Only':
+            if self.station.location.is_none() is True:
+                txt = '\nThe location of the station has not been set.'
+            else:
+                txt = f'\nThe location of the station is at {str(self.station.location)}.  '\
+                      'All measured points will be relative to that point and the horizontal angle uploaded here.'
 
-class DataGridTable(BoxLayout):
+        elif self.setup_type.text == 'Over a datum':
+            if self.setup_widgets.over_datum.datum is None:
+                error_message = '\nSelect the datum under the total station and optionally provide the station height.'
+            else:
+                station_height = float(self.setup_widgets.station_height.text) if self.setup_widgets.station_height.text else 0
+                self.new_station = self.setup_widgets.over_datum.datum
+                self.new_station.z += station_height
+                txt = f'\nSet the station coordinates to\nX : {self.new_station.x}\nY : {self.new_station.y}\nZ : {self.new_station.z}'
+
+        elif self.setup_type.text == 'Over a datum + Record a datum':
+            if self.setup_widgets.datum1.datum is None or self.setup_widgets.datum2.datum is None:
+                error_message = '\nSelect the datum under the total station and a datum to record.'
+            elif self.setup_widgets.datum1.datum == self.setup_widgets.datum2.datum:
+                error_message = '\nSelect two different datums.'
+            elif self.station.subtract_points(self.setup_widgets.datum1.datum, self.setup_widgets.datum2.datum) == point(0, 0, 0):
+                error_message = '\nSelect two different datums with different coordinates.'
+            elif self.setup_widgets.recorder[0].result.xyz is None:
+                error_message = '\nRecord the datum before accepting the setup.'
+            else:
+                self.new_station = self.station.subtract_points(self.setup_widgets.datum2.datum, self.setup_widgets.recorder[0].result.xyz).round()
+                datum2 = self.station.add_points(self.setup_widgets.datum1.datum, self.setup_widgets.recorder[0].result.xyz).round()
+                station_error = self.station.subtract_points(self.setup_widgets.datum2.datum, datum2).round()
+                txt = f'\n{self.setup_widgets.datum2.datum.name} recorded as \nX : {datum2.x}\nY : {datum2.y}\nZ : {datum2.z}\n'
+                txt += f'\nThe error in this measurement is \nX : {station_error.x}\nY : {station_error.y}\nZ : {station_error.z}\n'
+                txt += '(Note that Z will be off by the station height in most setups)\n'
+                txt += '\nIf the setup as measured is accepted, the new station coordinates will be \n'\
+                        f'X : {self.new_station.x}\nY : {self.new_station.y}\nZ : {self.new_station.z}'
+
+        elif self.setup_type.text == 'Record two datums':
+            if self.setup_widgets.datum1.datum is None or self.setup_widgets.datum2.datum is None:
+                error_message = '\nSelect two datums to record.'
+            elif self.setup_widgets.datum1.datum == self.setup_widgets.datum2.datum:
+                error_message = '\nSelect two different datums.'
+            elif self.station.subtract_points(self.setup_widgets.datum1.datum, self.setup_widgets.datum2.datum) == point(0, 0, 0):
+                error_message = '\nSelect two different datums with different coordinates.'
+            elif self.setup_widgets.recorder[0].result.xyz.is_none() or self.setup_widgets.recorder[1].result.xyz.is_none():
+                error_message = '\nRecord each datum.  It is important that the first datum is recorded and then the second and not the other way around.  '\
+                                'Note that before the first datum is recorded, a horizontal angle of 0.0000 will be uploaded.'
+            else:
+                measured_distance = self.station.distance(self.setup_widgets.recorder[0].result.xyz, self.setup_widgets.recorder[1].result.xyz)
+                actual_distance = self.station.distance(self.setup_widgets.datum1.datum.as_point(), self.setup_widgets.datum2.datum.as_point())
+                error_distance = abs(measured_distance - actual_distance)
+
+                # The following code is ported from EDM-Mobile (and EDMWin).
+                # I can't remember exactly how this works, but it does work.
+                # And I remember the hot, weekend day at Carsac when Harold
+                # and I first figured out how to do this.
+
+                # Workout what the measured angle would be from datum1 to datum2
+                y = -1 * self.setup_widgets.recorder[0].result.xyz.y
+                y = y + self.setup_widgets.recorder[1].result.xyz.y
+                p = point(self.setup_widgets.recorder[1].result.xyz.x, y, 0)
+                measured_angle = self.station.angle_between_points(point(0, 0, 0), p)
+
+                # Calculate the actual angle between datum1 and datum2
+                defined_angle = self.station.angle_between_points(self.setup_widgets.datum1.datum.as_point(), self.setup_widgets.datum2.datum.as_point())
+
+                # get the difference between these two angles
+                angle_difference = defined_angle - measured_angle
+
+                # Based on this, compute the new datum.
+                x = round(-1 * self.setup_widgets.recorder[0].result.xyz.y * sin(d2r(angle_difference)) + self.setup_widgets.datum1.datum.x, 3)
+                y = round(-1 * self.setup_widgets.recorder[0].result.xyz.y * cos(d2r(angle_difference)) + self.setup_widgets.datum1.datum.y, 3)
+                z = round(((self.setup_widgets.datum1.datum.z - self.setup_widgets.recorder[0].result.xyz.z) + (
+                    self.setup_widgets.datum2.datum.z - self.setup_widgets.recorder[1].result.xyz.z)) / 2, 3)
+                self.new_station = point(x, y, z)
+
+                # Workout what angle needs to be uploaded to the station
+                self.foresight = self.station.angle_between_points(self.new_station, self.setup_widgets.datum2.datum.as_point())
+                txt = f'\nThe measured distance between {self.setup_widgets.datum1.datum.name} and {self.setup_widgets.datum2.datum.name} '\
+                      f'was {round(measured_distance, 3)} m.  The distance based on the datum definitions should be {round(actual_distance, 3)} m.  '\
+                      f'The error is {round(error_distance, 3)} m.\n'
+                txt += '\nIf the setup as measured is accepted, the new station coordinates will be \n'\
+                       f'X : {self.new_station.x}\nY : {self.new_station.y}\nZ : {self.new_station.z}\n'
+                txt += f'\nAn angle of {self.station.decimal_degrees_to_sexa_pretty(self.foresight)} '\
+                        'will be uploaded (do not turn the station until this angle is set).'
+                self.foresight = self.station.decimal_degrees_to_dddmmss(self.foresight)
+
+        elif self.setup_type.text == 'Three datum shift':
+            if self.setup_widgets.datum1.datum.is_none() or \
+                self.setup_widgets.datum2.datum.is_none() or \
+                    self.setup_widgets.datum3.datum.is_none():
+                error_message = '\nSelect three datums to record.'
+            elif self.setup_widgets.recorder[0].result.xyz is None or \
+                    self.setup_widgets.recorder[1].result.xyz is None or \
+                        self.setup_widgets.recorder[2].result.xyz is None:
+                error_message = '\nRecord each datum.'
+            else:
+                dist_12_measured = self.station.distance(self.setup_widgets.recorder[0].result.xyz, self.setup_widgets.recorder[1].result.xyz)
+                dist_12_datums = self.station.distance(self.setup_widgets.datum1.datum.as_point(), self.setup_widgets.datum2.datum.as_point())
+                dist_12_error = round(abs(dist_12_measured - dist_12_datums), 3)
+
+                dist_23_measured = self.station.distance(self.setup_widgets.recorder[1].result.xyz, self.setup_widgets.recorder[2].result.xyz)
+                dist_23_datums = self.station.distance(self.setup_widgets.datum2.datum.as_point(), self.setup_widgets.datum3.datum.as_point())
+                dist_23_error = round(abs(dist_23_measured - dist_23_datums), 3)
+
+                dist_13_measured = self.station.distance(self.setup_widgets.recorder[0].result.xyz, self.setup_widgets.recorder[2].result.xyz)
+                dist_13_datums = self.station.distance(self.setup_widgets.datum1.datum.as_point(), self.setup_widgets.datum3.datum.as_point())
+                dist_13_error = round(abs(dist_13_measured - dist_13_datums), 3)
+
+                # should also include a mean error by averaging everything
+
+                txt = f'\nThe following errors are noted.  The actual distance between datums 1 and 2 is {round(dist_12_datums, 3)} and '
+                txt += f'the measured distance was {round(dist_12_measured, 3)}.  '
+                txt += f'The actual distance between datums 2 and 3 is {round(dist_23_datums, 3)} and the measured distance was {round(dist_23_measured, 3)}.  '
+                txt += f'The actual distance between datums 1 and 3 is {round(dist_13_datums, 3)} and the measured distance was {round(dist_13_measured, 3)}.  '
+                txt += f'\n\nThis corresponds to errors of {dist_12_error}, {dist_23_error}, and {dist_13_error}, respectively.'
 
-    def __init__(self, list_dicts=[], column_names = None, tb = None, e5_cfg = None, colors = None, *args, **kwargs):
+        if not self.new_station.is_none() or txt:
+            self.popup = e5_MessageBox('Accept setup?', txt,
+                                        response_type = "YESNO",
+                                        call_back = [self.set_and_close, self.close_popup],
+                                        colors = self.colors)
+        else:
+            self.popup = e5_MessageBox('Error', error_message,
+                                        colors = self.colors)
 
-        super(DataGridTable, self).__init__(*args, **kwargs)
-        self.orientation = "vertical"
+        self.popup.open()
 
-        self.header = DataGridTableHeader(column_names, colors)
-        self.table_data = DataGridTableData(list_dicts = list_dicts, column_names = column_names,
-                                            tb = tb, e5_cfg = e5_cfg, colors = colors)
+    def close_popup(self, instance):
+        self.popup.dismiss()
 
-        self.table_data.fbind('scroll_x', self.scroll_with_header)
+    def set_and_close(self, instance):
+        if self.setup_type:
 
-        self.add_widget(self.header)
-        self.add_widget(self.table_data)
+            logger = logging.getLogger(__name__)
 
-    def scroll_with_header(self, obj, value):
-        self.header.scroll_x = value
+            if self.setup_type.text == 'Horizontal Angle Only':
+                pass
 
+            elif self.setup_type.text == 'Over a datum':
+                self.ini.update_value('SETUPS', 'OVERDATUM', self.setup_widgets.over_datum.datum.name)
+                logger.info(f'Setup over {self.setup_widgets.over_datum.datum}')
+
+            elif self.setup_type.text == 'Over a datum + Record a datum':
+                self.ini.update_value('SETUPS', 'OVERDATUM', self.setup_widgets.datum1.datum.name)
+                self.ini.update_value('SETUPS', 'RECORDDATUM', self.setup_widgets.datum2.datum.name)
+                logger.info(f'Setup over {self.setup_widgets.datum1.datum} and recorded {self.setup_widgets.datum2.datum}')
+
+            elif self.setup_type.text == 'Record two datums':
+                self.ini.update_value('SETUPS', '2DATUMS_DATUM_1', self.setup_widgets.datum1.datum.name)
+                self.ini.update_value('SETUPS', '2DATUMS_DATUM_2', self.setup_widgets.datum2.datum.name)
+                logger.info(f'Setup 2-point using {self.setup_widgets.datum1.datum} and {self.setup_widgets.datum2.datum}')
+
+            elif self.setup_type.text == 'Three datum shift':
+                self.station.rotate_local = [self.setup_widgets.recorder[0].result.xyz,
+                                                self.setup_widgets.recorder[1].result.xyz,
+                                                self.setup_widgets.recorder[2].result.xyz]
+                self.station.rotate_global = [self.setup_widgets.datum1.datum.as_point(),
+                                                    self.setup_widgets.datum2.datum.as_point(),
+                                                    self.setup_widgets.datum3.datum.as_point()]
+                self.ini.update_value('SETUPS', '3DATUM_SHIFT_LOCAL_1', '%s,%s,%s' % (self.setup_widgets.recorder[0].result.xyz.x,
+                                                                                            self.setup_widgets.recorder[0].result.xyz.y,
+                                                                                            self.setup_widgets.recorder[0].result.xyz.z))
+                self.ini.update_value('SETUPS', '3DATUM_SHIFT_LOCAL_2', '%s,%s,%s' % (self.setup_widgets.recorder[1].result.xyz.x,
+                                                                                            self.setup_widgets.recorder[1].result.xyz.y,
+                                                                                            self.setup_widgets.recorder[1].result.xyz.z))
+                self.ini.update_value('SETUPS', '3DATUM_SHIFT_LOCAL_3', '%s,%s,%s' % (self.setup_widgets.recorder[2].result.xyz.x,
+                                                                                            self.setup_widgets.recorder[2].result.xyz.y,
+                                                                                            self.setup_widgets.recorder[2].result.xyz.z))
+                self.ini.update_value('SETUPS', '3DATUM_SHIFT_GLOBAL_1', self.setup_widgets.datum1.datum.name)
+                self.ini.update_value('SETUPS', '3DATUM_SHIFT_GLOBAL_2', self.setup_widgets.datum2.datum.name)
+                self.ini.update_value('SETUPS', '3DATUM_SHIFT_GLOBAL_3', self.setup_widgets.datum3.datum.name)
+                logger.info(f'Setup 3 datum shift using {self.setup_widgets.datum1.datum}, {self.setup_widgets.datum2.datum}, and \
+                                {self.setup_widgets.datum3.datum}')
+                logger.info(f'Recorded values were respectively {self.setup_widgets.recorder[0].result.xyz}, {self.setup_widgets.recorder[1].result.xyz}, and \
+                                {self.setup_widgets.recorder[2].result.xyz}')
 
-class DataGridGridPanel(BoxLayout):
+        self.popup.dismiss()
+        if self.foresight:
+            self.station.set_horizontal_angle(self.foresight)
+            logger.info(f'Horizontal angle set to {self.foresight}')
+        if self.new_station.is_none() is False:
+            self.station.location = self.new_station
+            logger.info('Station location set to ' + str(self.station.location))
+        self.ini.update_value('SETUPS', 'LASTSETUP_TYPE', self.setup_type.text)
+        self.ini.save()
+        self.parent.current = 'MainScreen'
 
-    def populate_data(self, tb, tb_fields, colors = None):
-        if tb is not None and tb_fields is not None:
-            self.colors = colors if colors else ColorScheme()
-            self.tb = tb
-            self.sort_key = None
-            self.column_names = ['doc_id'] + tb_fields.fields()
-            self.tb_fields = tb_fields
-            self._generate_table()
 
-    def _generate_table(self, sort_key = None, disabled = None):
-        self.clear_widgets()
-        data = []
-        for tb_row in self.tb:
-            reformatted_row = {}
-            reformatted_row['doc_id'] = str(tb_row.doc_id)
-            for field in self.tb_fields.fields():
-                reformatted_row[field] = str(tb_row[field]) if field in tb_row else ''
-            data.append(reformatted_row)
-        data = sorted(data, key=lambda k: int(k['doc_id']), reverse = True)
-        self.recycleview_box = DataGridTable(list_dicts = data, column_names = self.column_names,
-                                                tb = self.tb, e5_cfg = self.tb_fields, colors = self.colors)
-        self.add_widget(self.recycleview_box)
-
-
-class DataGridCasePanel(BoxLayout):
-
-    def populate(self, data, fields, colors = None):
-        if data is not None and fields is not None:
-            self.colors = colors if colors else ColorScheme()
-            self.edit_list.bind(minimum_height = self.edit_list.setter('height'))
-            self.edit_list.clear_widgets()
-            for col in fields.fields():
-                label_and_text = DataGridLabelAndField(col = col, colors = self.colors)
-                label_and_text.txt.bind(on_text_validate = self.next_field)
-                self.edit_list.add_widget(label_and_text)
+class EditLastRecordScreen(e5_RecordEditScreen):
+    pass
 
-    def next_field(self, instance):
-        pass
 
+class EditPointScreen(e5_RecordEditScreen):
 
-class DataGridLabelAndToggle(BoxLayout):
+    def reset_defaults_from_recorded_point(self, station):
+        for widget in self.layout.walk():
+            if hasattr(widget, 'id'):
+                value = station.format_widget_value(widget.id)
+                if value != '':
+                    widget.text = str(value)
 
-    def __init__(self, col, active = False, colors = None, popup = False, **kwargs):
-        super(DataGridLabelAndToggle, self).__init__(**kwargs)
-        self.colors = colors if colors is not None else ColorScheme()
-        self.size_hint = (0.9, None)
-        self.bind(minimum_height = self.setter('height'))
-        self.spacing = 10
-        label = e5_label(text = col, id = '__label', colors = self.colors, popup = popup)
-        label.bind(texture_size = label.setter('size'))
-        self.check = Switch(active = active, size_hint = (0.75, None))
-        self.add_widget(label)
-        self.add_widget(self.check)
 
+class EditDatumScreen(Screen):
+    pass
 
-class DataGridLabelAndField(BoxLayout):
 
-    popup = ObjectProperty(None)
-    sorted_result = None
+class EditPointsScreen(e5_DatagridScreen):
+    pass
 
-    def __init__(self, col, colors, note_field = False, popup = False, **kwargs):
-        super(DataGridLabelAndField, self).__init__(**kwargs)
-        self.update_db = False
-        self.widget_type = 'data'
-        if not note_field:
-            if colors:
-                if colors.text_font_size:
-                    self.height = int(colors.text_font_size.replace('sp', '')) * 1.9
-        self.size_hint = (0.9, None)
-        self.bind(minimum_height = self.setter('height'))
-        self.spacing = 10
-        label = e5_label(text = col, id = '__label', colors = colors, popup = popup, size_hint_y = None)
-        label.bind(texture_size=label.setter('size'))
-        self.txt = e5_textinput(multiline = note_field,
-                                size_hint = (0.75, None),
-                                id = col,
-                                # size_hint_y = 1,
-                                write_tab = False)
-        self.txt.bind(minimum_height = self.txt.setter('height'))
-        if colors:
-            if colors.text_font_size:
-                self.txt.font_size = colors.text_font_size
-        self.add_widget(label)
-        self.add_widget(self.txt)
 
+class EditPrismsScreen(e5_DatagridScreen):
+    pass
 
-class DataGridDeletePanel(GridLayout):
 
-    def populate(self, message = None, call_back = None, colors = None):
-        self.colors = colors if colors else ColorScheme()
-        self.clear_widgets()
-        self.cols = 1
-        self.spacing = 5
-        if message is not None:
-            self.add_widget(e5_scrollview_label(message, popup = False, colors = self.colors))
-            self.add_widget(e5_button('Delete',
-                                        id = 'delete',
-                                        selected = True,
-                                        call_back = call_back, colors = self.colors))
-        else:
-            self.add_widget(e5_scrollview_label('\nHighlight a record in the grid view (data tab) by clicking on its doc_id, and then delete that record here.',
-                                                 popup = False, colors = self.colors))
-
-
-class DataGridAddNewPanel(GridLayout):
-
-    def populate(self, data, fields, colors = None, addnew = False, call_back = None):
-        if data is not None and fields is not None:
-            self.colors = colors if colors else ColorScheme()
-            self.cols = 1
-            if addnew:
-                self.addnew_list.bind(minimum_height = self.addnew_list.setter('height'))
-                self.addnew_list.clear_widgets()
-                for col in fields.fields():
-                    label_and_text = DataGridLabelAndField(col = col, colors = self.colors)
-                    label_and_text.txt.bind(on_text_validate = self.next_field)
-                    self.addnew_list.add_widget(label_and_text)
-                self.button = e5_button('Add record',
-                                            id = 'addnew',
-                                            selected = False,
-                                            call_back = call_back, colors = self.colors)
-                self.add_widget(self.button)
-                self.call_back = call_back
-            else:
-                self.clear_widgets()
-                if __program__ == 'EDM':
-                    self.add_widget(e5_scrollview_label('\nAdding records in this way is not enabled for the main points table but is enabled for datums, units and prisms.',
-                                                        popup = False, colors = self.colors))
-                else:
-                    self.add_widget(e5_scrollview_label('\nAdding records in this way is not enabled in E5 because it would bipass conditions and error checking (but it is enabled in EDM which is why it appears in this list of tabs).',
-                                                        popup = False, colors = self.colors))
+class EditUnitsScreen(e5_DatagridScreen):
+    pass
 
-    def next_field(self, instance):
-        if instance.get_focus_next() == self.button:
-            if self.call_back:
-                self.call_back(instance)
-                instance.get_focus_next().get_focus_next().focus = True
-        else:
-            instance.get_focus_next().focus = True
 
+class EditDatumsScreen(e5_DatagridScreen):
+    pass
 
-class DataGridWidget(TabbedPanel):
-    data = ObjectProperty(None)
-    fields = ObjectProperty(None)
-    colors = ObjectProperty(None)
-
-    popup = None
-    popup_scrollmenu = None
-    popup_addbutton = None
-    popup_textbox = None
-    popup_field_widget = None
-
-    def __init__(self, data = None, cfg = None, colors = None, addnew = False, **kwargs):
-        super(DataGridWidget, self).__init__(**kwargs)
-        self.textboxes_will_update_db = False
-
-        self.addnew = addnew
-
-        if data is not None:
-            self.data = data
-        if cfg is not None:
-            self.fields = cfg
-            self.cfg = cfg
 
-        self.colors = colors if colors else ColorScheme()
-        self.color = self.colors.text_color
-        self.background_color = self.colors.window_background
-        self.background_image = ''
-
-        if data is not None and self.fields is not None:
-            self.populate_panels()
-
-        # if not addnew:
-        #    self.tab_list.remove(self.get_tab_by_name('Add New'))
-
-        for tab in self.tab_list:
-            tab.color = self.colors.button_color
-            tab.background_color = self.colors.button_background
-            if self.colors.datagrid_font_size:
-                tab.font_size = self.colors.datagrid_font_size
-
-    def record_count(self):
-        datatable = self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable')
-        return(datatable.nrows if datatable else 0)
-
-    def reload_data(self):
-        # This next conditional is to avoid an exception in unit testing
-        if hasattr(self, 'panel1'):
-            self.panel1.populate_data(tb = self.data, tb_fields = self.cfg, colors = self.colors)
-            if self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable'):
-                self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable').datatable_widget = self
-        # self.populate_panels()
-
-    # def load_data(self, data, fields):
-    #    self.data = data
-    #    self.fields = fields
-    #    self.populate_panels()
-
-    def populate_panels(self):
-        # This next conditional is to avoid an exception in unit testing
-        if hasattr(self, 'panel1'):
-            self.panel1.populate_data(tb = self.data, tb_fields = self.cfg, colors = self.colors)
-            self.panel2.populate(data = self.data, fields = self.fields, colors = self.colors)
-            self.panel3.populate(colors = self.colors)
-            self.panel4.populate(addnew = self.addnew,
-                                    data = self.data,
-                                    fields = self.fields,
-                                    colors = self.colors,
-                                    call_back = self.addnew_record)
-            if self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable'):
-                self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable').datatable_widget = self
-
-    def open_panel1(self):
-        if self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable'):
-            self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable').datatable_widget = self
-        self.textboxes_will_update_db = False
-
-    def open_panel2(self):
-        datatable = self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable')
-        if datatable is not None:
-            if datatable.datagrid_doc_id is not None and datatable.datagrid_doc_id != '':
-                data_record = self.data.get(doc_id = int(datatable.datagrid_doc_id))
-                for widget in self.ids.edit_panel.children[0].walk():
-                    if hasattr(widget, 'id'):
-                        if widget.id in self.fields.fields():
-                            widget.text = str(data_record[widget.id]) if widget.id in data_record else ''
-                            widget.bind(text = self.update_db)
-                            widget.bind(focus = self.show_menu)
-                self.textboxes_will_update_db = True
-            else:
-                cfg_fields = self.fields.fields()
-                for widget in self.ids.edit_panel.children[0].walk():
-                    if hasattr(widget, 'id'):
-                        if widget.id in cfg_fields:
-                            widget.text = ''
-                self.textboxes_will_update_db = False
-
-    def open_panel3(self):
-        datatable = self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable')
-        if datatable is not None:
-            if datatable.datagrid_doc_id:
-                data_record = self.data.get(doc_id = int(datatable.datagrid_doc_id))
-                if data_record:
-                    serialize_record = '\nDelete this record?\n\n'
-                    for field in data_record:
-                        serialize_record += field + " : %s\n" % data_record[field]
-                    self.panel3.populate(message = serialize_record,
-                                            call_back = self.delete_record1,
-                                            colors = self.colors)
+class station_setting(GridLayout):
+    label = ObjectProperty(None)
+    spinner = ObjectProperty(None)
+    id = ObjectProperty(None)
+    comport_to_test = None
+    valid_comports = []
 
-    def open_panel4(self):
-        if self.fields is not None:
-            self.textboxes_will_update_db = False
-            cfg_fields = self.fields.fields()
-            # TODO this seems like a bug - not sure why edit_panel is being cleared here
-            for widget in self.ids.edit_panel.children[0].walk():
-                if hasattr(widget, 'id'):
-                    if widget.id in cfg_fields:
-                        widget.text = ''
-
-    def show_menu(self, instance, value):
-        if instance.focus:
-            cfg_field = self.fields.get(instance.id)
-            if cfg_field:
-                self.popup_field_widget = instance
-                if cfg_field.inputtype in ['MENU', 'BOOLEAN']:
-                    self.popup = DataGridMenuList(instance.id, cfg_field.menu,
-                                                    instance.text, self.menu_selection, colors = self.colors)
-                    self.popup.open()
-                    self.popup_scrollmenu = self.get_widget_by_id(self.popup, 'menu_scroll')
-                    self.popup_textbox = self.get_widget_by_id(self.popup, 'new_item')
-                    self.popup_addbutton = self.get_widget_by_id(self.popup, 'add_button')
+    def __init__(self, label_text = '', spinner_values = (), default = '',
+                        id = None, call_back = None, colors = None, station = None, **kwargs):
+        super(station_setting, self).__init__(**kwargs)
 
-    def menu_selection(self, instance):
-        self.popup.dismiss()
-        self.popup_field_widget.text = instance.text if not instance.id == 'add_button' else self.popup_textbox.text
-        self.popup_field_widget = None
-        self.popup_scrollmenu = None
-
-    def clear_addnew(self):
-        cfg_fields = self.fields.fields()
-        for widget in self.ids.addnew_panel.children[1].walk():
-            if hasattr(widget, 'id'):
-                if widget.id in cfg_fields:
-                    if widget.text:
-                        widget.text = ''
+        self.station = station
+        self.id = id
+        self.cols = 2
+        self.pos_hint = {'center_x': .5},
+        self.colors = colors
+        self.label = e5_label(text = label_text, colors = colors)
+        self.add_widget(self.label)
 
-    def build_record_from_addnew(self):
-        new_record = {}
-        cfg_fields = self.fields.fields()
-        for widget in self.ids.addnew_panel.children[1].walk():
-            if hasattr(widget, 'id'):
-                if widget.id in cfg_fields:
-                    if widget.text:
-                        new_record[widget.id] = widget.text
-        return(new_record)
-
-    def strip_strings_from_number_fields(self, new_record):
-        for field, value in new_record.items():
-            f = self.cfg.get(field)
-            if f.inputtype == 'NUMERIC':
-                try:
-                    new_record[field] = float(value)
-                except ValueError:
-                    pass
-        return(new_record)
+        # Create a default dropdown button and then modify its properties
+        # For some reason, the usual font size specification doesn't work here and sp has to be removed
+        spinner_dropdown_button = SpinnerOptions
+        spinner_dropdown_button.font_size = colors.button_font_size.replace("sp", '') if colors.button_font_size else None
+        spinner_dropdown_button.background_color = (0, 0, 0, 1)
 
-    def addnew_record(self, instance):
-        new_record = self.build_record_from_addnew()
-        valid_data = self.cfg.validate_datarecord(new_record, self.data)
-        if valid_data is True:
-            self.data.insert(self.strip_strings_from_number_fields(new_record))
-            self.data.new_data = True  # TODO Needs to reference parent
-            self.panel1.populate_data(tb = self.data, tb_fields = self.fields, colors = self.colors)
-            self.clear_addnew()
+        self.spinner = Spinner(text = default if default is not None else '',
+                                values = spinner_values,
+                                font_size = colors.button_font_size if colors.button_font_size else None,
+                                option_cls = spinner_dropdown_button)
+        if label_text == 'Port Number':
+            comport = GridLayout(cols = 2, spacing = 5)
+            comport.bind(minimum_height = comport.setter('height'))
+            comport.add_widget(self.spinner)
+            scan_button = e5_button('Scan', colors = colors, call_back = self.scanner, button_height = comport.height)
+            comport.add_widget(scan_button)
+            self.add_widget(comport)
         else:
-            self.popup = e5_MessageBox("Save error", valid_data, call_back = self.close_popup)
+            self.add_widget(self.spinner)
+        if call_back:
+            self.spinner.bind(text = call_back)
+
+    def scanner(self, instance):
+        if self.station:
+            ports = self.station.list_comports()
+            text = 'Available ports:\n\n'
+            for port in ports:
+                text += f"{port[0]['port']} - {port[0]['desc'][0:port[0]['desc'].find('(') - 1]}\n"
+            self.spinner.values = list([port[0]['port'] for port in ports])
+            self.popup = e5_MessageBox('COM Ports', text,
+                                        response_type = "OK",
+                                        call_back = self.close_popup_comports,
+                                        colors = self.colors)
             self.popup.open()
             self.popup_open = True
+        else:
+            self.event1 = Clock.schedule_once(self.show_popup_message, .2)
+            self.event2 = Clock.schedule_interval(self.check_comports, .2)
 
-    def get_field_type(self, fieldname):
-        f = self.cfg.get(fieldname)
-        return(f.inputtype)
-
-    def update_db(self, instance, value):
-        if self.textboxes_will_update_db:
-            datatable = self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable')
-            if datatable is not None:
-                if self.get_field_type(instance.id) == 'NUMERIC':
-                    try:
-                        if '.' in value:
-                            update = {instance.id: float(value)}
-                        else:
-                            update = {instance.id: int(value)}
-                    except ValueError:
-                        update = {instance.id: value}
-                else:
-                    update = {instance.id: value}
-                is_valid = self.cfg.validate_datafield(update, self.data)
-                if is_valid is True:
-                    self.data.update(update, doc_ids = [int(datatable.datagrid_doc_id)])
-                    self.update_datagrid(datatable.datagrid_doc_id, instance.id, value)
-                    # for widget in datatable.datagrid_widget_row:
-                    #     if widget.field == instance.id and widget.key == datatable.datagrid_doc_id:
-                    #         widget.text = str(value)
-                    #         break
-
-    def update_datagrid(self, doc_id, field, value):
-        datatable = self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable')
-        for record in datatable.data:
-            if record['key'] == doc_id and record['field'] == field:
-                record['text'] = str(value)
-                self.get_tab_by_name('Data').content.recycleview_box.table_data.refresh_from_data()
-                break
-
-    def delete_record1(self, instance):
-        self.popup = e5_MessageBox('Delete record', '\nAre you sure you want to delete this record?',
-                                    response_type = "YESNO",
-                                    call_back = [self.delete_record2, self.close_popup],
+    def show_popup_message(self, dt):
+        self.popup = e5_MessageBox('COM Ports', '\nLooking for valid COM ports...This can take several seconds...'
+                                                    'And the Cancel button might appear non-responsive...',
+                                    response_type = "CANCEL",
+                                    call_back = self.close_popup,
                                     colors = self.colors)
         self.popup.open()
         self.popup_open = True
 
-    def delete_record2(self, value):
-        self.close_popup(value)
-        datatable = self.get_widget_by_id(self.get_tab_by_name('Data').content, 'datatable')
-        if datatable is not None:
-            doc_id = int(datatable.datagrid_doc_id)
-            self.data.remove(doc_ids = [doc_id])
-            datatable.datagrid_doc_id = None
-            # datatable.datagrid_widget_row = None
-            self.reload_data()
-            self.panel3.populate(colors = self.colors)
-            self.switch_to(self.get_tab_by_name('Data'))
-
     def close_popup(self, value):
         self.popup.dismiss()
         self.popup_open = False
+        self.event2.cancel()
+        self.comport_to_test = None
+
+    def close_popup_comports(self, value):
+        self.popup.dismiss()
+        self.popup_open = False
+
+    def comportIsUsable(self, portName):
+        try:
+            ser = serial.Serial(port = portName)
+            ser.close()
+            return portName
+        except:
+            return None
+
+    def check_comports(self, dt):
+        if self.comport_to_test is None:
+            self.comport_to_test = 0
+            self.valid_comports = []
+        self.comport_to_test += 1
+        if self.comport_to_test > __LASTCOMPORT__:
+            self.spinner.values = list(filter(None.__ne__, self.valid_comports))
+            self.event2.cancel()
+            self.close_popup(None)
+            self.comport_to_test = None
+        else:
+            self.valid_comports.append(self.comportIsUsable(f"COM{self.comport_to_test}"))
+
+    def comports(self):
+        return list(filter(None.__ne__, [self.comportIsUsable(f"COM{comno}") for comno in range(1, __LASTCOMPORT__ + 1)]))
+
+
+class StationConfigurationScreen(Screen):
+
+    def __init__(self, station = None, ini = None, colors = None, **kwargs):
+        super(StationConfigurationScreen, self).__init__(**kwargs)
+
+        self.station = station
+        self.colors = colors
+        self.ini = ini
+        self.call_back = 'MainScreen'
+
+    def on_enter(self):
+        self.clear_widgets()
+        self.layout = GridLayout(cols = 1,
+                                    spacing = 5, padding = 5,
+                                    size_hint_max_x = MAX_SCREEN_WIDTH,
+                                    size_hint_y = 1,
+                                    pos_hint = {'center_x': .5, 'center_y': .5})
+        self.add_widget(self.layout)
+        self.build_screen()
+
+    def build_screen(self):
+        self.station_type = station_setting(label_text = 'Station type',
+                                            spinner_values = ("Leica", "Leica GeoCom", "Wild", "Topcon", "Sokkia", "Microscribe",
+                                                                "Manual XYZ", "Manual VHD", "Simulate"),
+                                            call_back = self.toggle_buttons,
+                                            id = 'station_type',
+                                            colors = self.colors,
+                                            default = self.ini.get_value(APP_NAME, 'STATION'))
+        self.layout.add_widget(self.station_type)
+
+        self.communications = station_setting(label_text = 'Communications',
+                                                spinner_values = ("Serial", "Bluetooth"),
+                                                # call_back = self.update_ini,
+                                                id = 'communications',
+                                                colors = self.colors,
+                                                default = self.ini.get_value(APP_NAME, 'COMMUNICATIONS'))
+        self.layout.add_widget(self.communications)
+
+        self.comports = station_setting(label_text = 'Port Number',
+                                            spinner_values = [f'COM{n + 1}' for n in range(20)],
+                                            # call_back = self.update_ini,
+                                            id = 'comport',
+                                            colors = self.colors, station = self.station,
+                                            default = self.ini.get_value(APP_NAME, 'COMPORT'))
+        self.layout.add_widget(self.comports)
+
+        self.baud_rate = station_setting(label_text = 'Baud rate',
+                                            spinner_values = ("1200", "2400", "4800", "9600", "14400", "19200", "115200"),
+                                            # call_back = self.update_ini,
+                                            id = 'baudrate',
+                                            colors = self.colors,
+                                            default = self.ini.get_value(APP_NAME, 'BAUDRATE'))
+        self.layout.add_widget(self.baud_rate)
+
+        self.parity = station_setting(label_text = 'Parity',
+                                            spinner_values = ("Even", "Odd", "None"),
+                                            # call_back = self.update_ini,
+                                            id = 'parity',
+                                            colors = self.colors,
+                                            default = self.ini.get_value(APP_NAME, 'PARITY'))
+        self.layout.add_widget(self.parity)
+
+        self.data_bits = station_setting(label_text = 'Databits',
+                                            spinner_values = ("7", "8"),
+                                            # call_back = self.update_ini,
+                                            id = 'databits',
+                                            colors = self.colors,
+                                            default = self.ini.get_value(APP_NAME, 'DATABITS'))
+        self.layout.add_widget(self.data_bits)
+
+        self.stop_bits = station_setting(label_text = 'Stopbits',
+                                            spinner_values = ("0", "1", "2"),
+                                            # call_back = self.update_ini,
+                                            id = 'stopbits',
+                                            colors = self.colors,
+                                            default = self.ini.get_value(APP_NAME, 'STOPBITS'))
+        self.layout.add_widget(self.stop_bits)
+
+        self.buttons = e5_side_by_side_buttons(text = ['Back', 'Set'],
+                                                id = ['Back', 'Set'],
+                                                selected = [True, False],
+                                                call_back = [self.close_screen, self.update_ini],
+                                                colors = self.colors)
+        self.layout.add_widget(self.buttons)
+        self.toggle_buttons(None, None)
+        self.changes = False
+
+    def toggle_buttons(self, instance, value):
+        disabled = self.station_type.spinner.text in ['Simulate', 'Microscribe']
+        self.stop_bits.spinner.disabled = disabled
+        self.parity.spinner.disabled = disabled
+        self.data_bits.spinner.disabled = disabled
+        self.baud_rate.spinner.disabled = disabled
+        self.comports.spinner.disabled = disabled
+        self.communications.spinner.disabled = disabled
+
+    def update_ini(self, instance):
+        self.station.make = self.station_type.spinner.text
+        self.ini.update_value(APP_NAME, 'STATION', self.station_type.spinner.text)
+
+        self.station.stopbits = self.stop_bits.spinner.text
+        self.ini.update_value(APP_NAME, 'STOPBITS', self.stop_bits.spinner.text)
+
+        self.station.baudrate = self.baud_rate.spinner.text
+        self.ini.update_value(APP_NAME, 'BAUDRATE', self.baud_rate.spinner.text)
+
+        self.station.databits = self.data_bits.spinner.text
+        self.ini.update_value(APP_NAME, 'DATABITS', self.data_bits.spinner.text)
+
+        self.station.comport = self.comports.spinner.text
+        self.ini.update_value(APP_NAME, 'COMPORT', self.comports.spinner.text)
+
+        self.station.parity = self.parity.spinner.text
+        self.ini.update_value(APP_NAME, 'PARITY', self.parity.spinner.text)
+
+        self.station.communication = self.communications.spinner.text
+        self.ini.update_value(APP_NAME, 'COMMUNICATIONS', self.communications.spinner.text)
+
+        self.ini.save()
+        success = self.station.open()
+        if success != '':
+            self.popup = e5_MessageBox('Error', success)
+            self.popup.open()
+        else:
+            self.close_screen(None)
+
+    def close_screen(self, value):
+        self.parent.current = self.call_back
+
+
+class AboutScreen(e5_InfoScreen):
+    def on_pre_enter(self):
+        self.content.text = '\n\nEDM by Shannon P. McPherron\n\nVersion ' + VERSION + ' Beta\nBlueberry Pie\n\n'
+        self.content.text += f'Built using Python 3.8, Kivy {__kivy_version__} and TinyDB {__tinydb_version__}\n\n'
+        self.content.text += 'An OldStoneAge.Com Production\n\n' + PRODUCTION_DATE
+        self.content.halign = 'center'
+        self.content.valign = 'middle'
+        self.content.color = self.colors.text_color
+        self.back_button.background_color = self.colors.button_background
+        self.back_button.color = self.colors.button_color
+
+
+class StatusScreen(e5_InfoScreen):
+
+    def __init__(self, data = None, ini = None, cfg = None, station = None, **kwargs):
+        super(StatusScreen, self).__init__(**kwargs)
+        self.data = data
+        self.ini = ini
+        self.cfg = cfg
+        self.station = station
+
+    def on_pre_enter(self):
+        app_paths = AppDataPaths(APP_NAME)
+        txt = self.data.status() if self.data else 'A data file has not been initialized or opened.\n\n'
+        txt += self.cfg.status() if self.cfg else 'A CFG is not open.\n\n'
+        txt += self.ini.status() if self.ini else 'An INI file is not available.\n\n'
+        txt += self.station.status() if self.station else 'Total station information is not available.\n\n'
+        txt += f'\nThe default user path is {app_paths.app_data_path}.\n'
+        logger = logging.getLogger(__name__)
+        txt += f'\nThe log is written to {logger.handlers[0].baseFilename}\n'
+        txt += f'\nThe operating system is {platform_name()}.\n'
+        txt += f'\nPython build is {python_version()}.\n'
+        txt += f'\nLibraries installed include Kivy {__kivy_version__} and TinyDB {__tinydb_version__}.\n'
+        txt += '\nEDM was tested and distributed most recently on Python 3.8.1, Kivy 2.0.0 and TinyDB 4.4.0.\n'
+        self.content.text = txt
+        self.content.color = self.colors.text_color
+        self.back_button.background_color = self.colors.button_background
+        self.back_button.color = self.colors.button_color
+
+
+sm = ScreenManager()
+
+
+class EDMApp(App):
+
+    def __init__(self, **kwargs):
+        super(EDMApp, self).__init__(**kwargs)
+
+        self.app_paths = AppDataPaths(APP_NAME)
+        self.app_paths.setup()
+
+    def build(self):
+        sm.add_widget(MainScreen(name = 'MainScreen'))
+        sm.current = 'MainScreen'
+        self.title = APP_NAME + " " + VERSION
+        return sm
 
-    # repeats code above - could be put into a general functions package
-    def get_widget_by_id(self, start = None, id = ''):
-        start_here = self if start is None else start
-        for widget in start_here.walk():
-            if hasattr(widget, 'id'):
-                if widget.id == id:
-                    return(widget)
-        return(None)
-
-    def get_tab_by_name(self, text = ''):
-        for tab in self.tab_list:
-            if tab.text == text:
-                return(tab)
-        return(None)
 
-    def close_panels(self):
-        self.parent.parent.current = 'MainScreen'
+Factory.register(APP_NAME, cls = EDMApp)
 
-    def cancel(self):
-        pass
 
-# End code from https://github.com/MichaelStott/DataframeGUIKivy/blob/master/dfguik.py
-# endregion
+if __name__ == '__main__':
+    Config.set('input', 'mouse', 'mouse,multitouch_on_demand')      # Removes red dot
+    Config.set('kivy', 'exit_on_escape', '0')
+    EDMApp().run()
```

### Comparing `edm-arch-1.0.27/src/edmpy/lib/misc.py` & `edm-arch-1.0.32/src/edmpy/lib/misc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 from os import path
 from kivy.utils import platform
 from kivy.core.window import Window
 
-# See if the file as given can be found.
-# If not, try to find it in the same folder as the CFG file.
-# This can happen when a CFG and associated files are copied to a
-# new folder or computer or device.
-
 
 def locate_file(filename, cfg_path = None):
+    '''
+    See if the file as given can be found.
+    If not, try to find it in the same folder as the CFG file.
+    This can happen when a CFG and associated files are copied to a
+    new folder or computer or device.
+    '''
     if path.isfile(filename):
-        return(filename)
+        return filename
     if cfg_path:
         p, f = path.split(filename)
         if path.isfile(path.join(cfg_path, f)):
-            return(path.join(cfg_path, f))
-    return('')
+            return path.join(cfg_path, f)
+    return ''
 
 
 def filename_only(filename = None):
     if filename:
         p, f = path.split(filename)
-        return(f)
+        return f
     else:
-        return('')
+        return ''
 
 
 def platform_name():
-    return(['Windows', 'Linux', 'Android', 'MacOSX', 'IOS', 'Unknown'][['win', 'linux', 'android', 'macosx', 'ios', 'unknown'].index(platform)])
+    return (['Windows', 'Linux', 'Android', 'MacOSX', 'IOS', 'Unknown'][['win', 'linux', 'android', 'macosx', 'ios', 'unknown'].index(platform)])
 
 
 def restore_window_size_position(main_name, main_ini):
     Window.minimum_width = 450
     Window.minimum_height = 450
     if main_ini.get_value(main_name, "SCREENTOP"):
         temp = max(int(main_ini.get_value(main_name, "SCREENTOP")), 0)
```

