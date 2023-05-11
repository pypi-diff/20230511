# Comparing `tmp/glue-small-multiples-1.1.1.tar.gz` & `tmp/glue-small-multiples-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue-small-multiples-1.1.1.tar", last modified: Fri Mar 24 02:40:17 2023, max compression
+gzip compressed data, was "glue-small-multiples-1.1.2.tar", last modified: Thu May 11 13:39:04 2023, max compression
```

## Comparing `glue-small-multiples-1.1.1.tar` & `glue-small-multiples-1.1.2.tar`

### file list

```diff
@@ -1,51 +1,35 @@
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-24 02:40:17.122531 glue-small-multiples-1.1.1/
--rw-r--r--   0 jfoster    (501) staff       (20)     1820 2022-07-25 18:38:05.000000 glue-small-multiples-1.1.1/.gitignore
--rw-r--r--   0 jfoster    (501) staff       (20)      229 2023-03-24 02:38:18.000000 glue-small-multiples-1.1.1/CHANGES.md
--rw-r--r--   0 jfoster    (501) staff       (20)     1023 2023-03-24 02:40:17.122659 glue-small-multiples-1.1.1/PKG-INFO
--rw-r--r--   0 jfoster    (501) staff       (20)      259 2023-03-24 02:33:19.000000 glue-small-multiples-1.1.1/README.md
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-24 02:40:17.112494 glue-small-multiples-1.1.1/glue_small_multiples/
--rw-r--r--   0 jfoster    (501) staff       (20)      145 2022-07-14 18:45:57.000000 glue-small-multiples-1.1.1/glue_small_multiples/__init__.py
--rw-r--r--   0 jfoster    (501) staff       (20)    16789 2023-03-24 02:34:02.000000 glue-small-multiples-1.1.1/glue_small_multiples/layer_artist.py
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-24 02:40:17.119330 glue-small-multiples-1.1.1/glue_small_multiples/qt/
--rw-r--r--   0 jfoster    (501) staff       (20)        0 2022-07-14 18:45:57.000000 glue-small-multiples-1.1.1/glue_small_multiples/qt/__init__.py
--rw-r--r--   0 jfoster    (501) staff       (20)    10367 2022-09-14 14:36:06.000000 glue-small-multiples-1.1.1/glue_small_multiples/qt/layer_style_editor.py
--rw-r--r--   0 jfoster    (501) staff       (20)    31829 2021-07-29 13:32:17.000000 glue-small-multiples-1.1.1/glue_small_multiples/qt/layer_style_editor.ui
--rw-r--r--   0 jfoster    (501) staff       (20)      643 2022-09-14 14:35:59.000000 glue-small-multiples-1.1.1/glue_small_multiples/qt/options_widget.py
--rw-r--r--   0 jfoster    (501) staff       (20)    11435 2022-10-07 20:17:52.000000 glue-small-multiples-1.1.1/glue_small_multiples/qt/options_widget.ui
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-24 02:40:17.121789 glue-small-multiples-1.1.1/glue_small_multiples/qt/tests/
--rw-r--r--   0 jfoster    (501) staff       (20)        0 2022-08-02 19:50:55.000000 glue-small-multiples-1.1.1/glue_small_multiples/qt/tests/__init__.py
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-24 02:40:17.122276 glue-small-multiples-1.1.1/glue_small_multiples/qt/tests/data/
--rw-r--r--   0 jfoster    (501) staff       (20)    16046 2022-08-02 19:50:55.000000 glue-small-multiples-1.1.1/glue_small_multiples/qt/tests/data/penguins.csv
--rw-r--r--   0 jfoster    (501) staff       (20)     2562 2022-09-16 20:07:13.000000 glue-small-multiples-1.1.1/glue_small_multiples/qt/tests/echo_selection_none.py
--rw-r--r--   0 jfoster    (501) staff       (20)     1272 2022-09-19 14:08:39.000000 glue-small-multiples-1.1.1/glue_small_multiples/qt/tests/run_example.py
--rw-r--r--   0 jfoster    (501) staff       (20)    11631 2022-10-07 15:25:43.000000 glue-small-multiples-1.1.1/glue_small_multiples/qt/tests/session.glu
--rw-r--r--   0 jfoster    (501) staff       (20)     3070 2022-10-07 18:14:45.000000 glue-small-multiples-1.1.1/glue_small_multiples/qt/tests/test_axes.py
--rw-r--r--   0 jfoster    (501) staff       (20)     6886 2022-10-25 01:44:38.000000 glue-small-multiples-1.1.1/glue_small_multiples/qt/tests/test_data_viewer.py
--rw-r--r--   0 jfoster    (501) staff       (20)     2562 2022-10-07 18:14:45.000000 glue-small-multiples-1.1.1/glue_small_multiples/qt/tests/test_save_restore.py
--rw-r--r--   0 jfoster    (501) staff       (20)    12146 2022-10-12 20:03:29.000000 glue-small-multiples-1.1.1/glue_small_multiples/qt/viewer.py
--rw-r--r--   0 jfoster    (501) staff       (20)    36975 2022-10-08 18:38:10.000000 glue-small-multiples-1.1.1/glue_small_multiples/session.glu
--rw-r--r--   0 jfoster    (501) staff       (20)    12287 2022-10-25 01:44:38.000000 glue-small-multiples-1.1.1/glue_small_multiples/state.py
--rw-r--r--   0 jfoster    (501) staff       (20)    26178 2022-10-08 17:47:10.000000 glue-small-multiples-1.1.1/glue_small_multiples/test1.glu
--rw-r--r--   0 jfoster    (501) staff       (20)    36804 2022-10-08 17:55:26.000000 glue-small-multiples-1.1.1/glue_small_multiples/test2.glu
--rw-r--r--   0 jfoster    (501) staff       (20)    36393 2022-10-08 18:03:11.000000 glue-small-multiples-1.1.1/glue_small_multiples/test3.glu
--rw-r--r--   0 jfoster    (501) staff       (20)    75705 2022-10-08 18:04:23.000000 glue-small-multiples-1.1.1/glue_small_multiples/test4.glu
--rw-r--r--   0 jfoster    (501) staff       (20)    94376 2022-10-08 18:06:47.000000 glue-small-multiples-1.1.1/glue_small_multiples/test5.glu
--rw-r--r--   0 jfoster    (501) staff       (20)    94267 2022-10-08 18:07:39.000000 glue-small-multiples-1.1.1/glue_small_multiples/test6.glu
--rw-r--r--   0 jfoster    (501) staff       (20)   136474 2022-10-08 18:12:09.000000 glue-small-multiples-1.1.1/glue_small_multiples/test7.glu
--rw-r--r--   0 jfoster    (501) staff       (20)    46623 2022-10-08 18:30:23.000000 glue-small-multiples-1.1.1/glue_small_multiples/test8.glu
--rw-r--r--   0 jfoster    (501) staff       (20)    37146 2022-10-08 20:27:48.000000 glue-small-multiples-1.1.1/glue_small_multiples/test9.glu
--rw-r--r--   0 jfoster    (501) staff       (20)    26058 2022-10-08 20:26:34.000000 glue-small-multiples-1.1.1/glue_small_multiples/test_diff_gene_exp.glu
--rw-r--r--   0 jfoster    (501) staff       (20)    11285 2022-10-25 01:35:33.000000 glue-small-multiples-1.1.1/glue_small_multiples/test_penguins_cmap.glu
--rw-r--r--   0 jfoster    (501) staff       (20)    75796 2022-10-12 20:05:25.000000 glue-small-multiples-1.1.1/glue_small_multiples/toolbar_test_session.glu
--rw-r--r--   0 jfoster    (501) staff       (20)     1127 2022-07-14 19:22:36.000000 glue-small-multiples-1.1.1/glue_small_multiples/utils.py
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-03-24 02:40:17.114991 glue-small-multiples-1.1.1/glue_small_multiples.egg-info/
--rw-r--r--   0 jfoster    (501) staff       (20)     1023 2023-03-24 02:40:17.000000 glue-small-multiples-1.1.1/glue_small_multiples.egg-info/PKG-INFO
--rw-r--r--   0 jfoster    (501) staff       (20)     1570 2023-03-24 02:40:17.000000 glue-small-multiples-1.1.1/glue_small_multiples.egg-info/SOURCES.txt
--rw-r--r--   0 jfoster    (501) staff       (20)        1 2023-03-24 02:40:17.000000 glue-small-multiples-1.1.1/glue_small_multiples.egg-info/dependency_links.txt
--rw-r--r--   0 jfoster    (501) staff       (20)       65 2023-03-24 02:40:17.000000 glue-small-multiples-1.1.1/glue_small_multiples.egg-info/entry_points.txt
--rw-r--r--   0 jfoster    (501) staff       (20)        1 2022-07-14 18:37:34.000000 glue-small-multiples-1.1.1/glue_small_multiples.egg-info/not-zip-safe
--rw-r--r--   0 jfoster    (501) staff       (20)       47 2023-03-24 02:40:17.000000 glue-small-multiples-1.1.1/glue_small_multiples.egg-info/requires.txt
--rw-r--r--   0 jfoster    (501) staff       (20)       21 2023-03-24 02:40:17.000000 glue-small-multiples-1.1.1/glue_small_multiples.egg-info/top_level.txt
--rw-r--r--   0 jfoster    (501) staff       (20)      149 2023-03-24 02:40:04.000000 glue-small-multiples-1.1.1/pyproject.toml
--rw-r--r--   0 jfoster    (501) staff       (20)     1074 2023-03-24 02:40:17.123032 glue-small-multiples-1.1.1/setup.cfg
--rw-r--r--   0 jfoster    (501) staff       (20)      397 2022-10-07 17:28:26.000000 glue-small-multiples-1.1.1/setup.py
+drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-05-11 13:39:04.696155 glue-small-multiples-1.1.2/
+-rw-r--r--   0 jfoster    (501) staff       (20)     1820 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/.gitignore
+-rw-r--r--   0 jfoster    (501) staff       (20)      229 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/CHANGES.md
+-rw-r--r--   0 jfoster    (501) staff       (20)     1023 2023-05-11 13:39:04.696248 glue-small-multiples-1.1.2/PKG-INFO
+-rw-r--r--   0 jfoster    (501) staff       (20)      259 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/README.md
+drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-05-11 13:39:04.693801 glue-small-multiples-1.1.2/glue_small_multiples/
+-rw-r--r--   0 jfoster    (501) staff       (20)      145 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/__init__.py
+-rw-r--r--   0 jfoster    (501) staff       (20)    16789 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/layer_artist.py
+drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-05-11 13:39:04.695490 glue-small-multiples-1.1.2/glue_small_multiples/qt/
+-rw-r--r--   0 jfoster    (501) staff       (20)        0 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/qt/__init__.py
+-rw-r--r--   0 jfoster    (501) staff       (20)    10367 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/qt/layer_style_editor.py
+-rw-r--r--   0 jfoster    (501) staff       (20)    31901 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/qt/layer_style_editor.ui
+-rw-r--r--   0 jfoster    (501) staff       (20)      643 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/qt/options_widget.py
+-rw-r--r--   0 jfoster    (501) staff       (20)    11451 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/qt/options_widget.ui
+drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-05-11 13:39:04.695945 glue-small-multiples-1.1.2/glue_small_multiples/qt/tests/
+-rw-r--r--   0 jfoster    (501) staff       (20)        0 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/qt/tests/__init__.py
+drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-05-11 13:39:04.696056 glue-small-multiples-1.1.2/glue_small_multiples/qt/tests/data/
+-rw-r--r--   0 jfoster    (501) staff       (20)    16046 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/qt/tests/data/penguins.csv
+-rw-r--r--   0 jfoster    (501) staff       (20)     3070 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/qt/tests/test_axes.py
+-rw-r--r--   0 jfoster    (501) staff       (20)     6886 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/qt/tests/test_data_viewer.py
+-rw-r--r--   0 jfoster    (501) staff       (20)     2562 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/qt/tests/test_save_restore.py
+-rw-r--r--   0 jfoster    (501) staff       (20)    12146 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/qt/viewer.py
+-rw-r--r--   0 jfoster    (501) staff       (20)    12287 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/state.py
+-rw-r--r--   0 jfoster    (501) staff       (20)     1127 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/glue_small_multiples/utils.py
+drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-05-11 13:39:04.694715 glue-small-multiples-1.1.2/glue_small_multiples.egg-info/
+-rw-r--r--   0 jfoster    (501) staff       (20)     1023 2023-05-11 13:39:04.000000 glue-small-multiples-1.1.2/glue_small_multiples.egg-info/PKG-INFO
+-rw-r--r--   0 jfoster    (501) staff       (20)      984 2023-05-11 13:39:04.000000 glue-small-multiples-1.1.2/glue_small_multiples.egg-info/SOURCES.txt
+-rw-r--r--   0 jfoster    (501) staff       (20)        1 2023-05-11 13:39:04.000000 glue-small-multiples-1.1.2/glue_small_multiples.egg-info/dependency_links.txt
+-rw-r--r--   0 jfoster    (501) staff       (20)       65 2023-05-11 13:39:04.000000 glue-small-multiples-1.1.2/glue_small_multiples.egg-info/entry_points.txt
+-rw-r--r--   0 jfoster    (501) staff       (20)        1 2023-05-11 13:39:04.000000 glue-small-multiples-1.1.2/glue_small_multiples.egg-info/not-zip-safe
+-rw-r--r--   0 jfoster    (501) staff       (20)       47 2023-05-11 13:39:04.000000 glue-small-multiples-1.1.2/glue_small_multiples.egg-info/requires.txt
+-rw-r--r--   0 jfoster    (501) staff       (20)       21 2023-05-11 13:39:04.000000 glue-small-multiples-1.1.2/glue_small_multiples.egg-info/top_level.txt
+-rw-r--r--   0 jfoster    (501) staff       (20)      149 2023-05-11 13:34:45.000000 glue-small-multiples-1.1.2/pyproject.toml
+-rw-r--r--   0 jfoster    (501) staff       (20)     1074 2023-05-11 13:39:04.696574 glue-small-multiples-1.1.2/setup.cfg
+-rw-r--r--   0 jfoster    (501) staff       (20)      397 2023-05-11 13:32:46.000000 glue-small-multiples-1.1.2/setup.py
```

### Comparing `glue-small-multiples-1.1.1/.gitignore` & `glue-small-multiples-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `glue-small-multiples-1.1.1/PKG-INFO` & `glue-small-multiples-1.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-small-multiples
-Version: 1.1.1
+Version: 1.1.2
 Summary: A viewer for small multiples
 Home-page: https://www.gluesolutions.io
 Author: glue solutions, inc.
 Author-email: jfoster@gluesolutions.io
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `glue-small-multiples-1.1.1/glue_small_multiples/layer_artist.py` & `glue-small-multiples-1.1.2/glue_small_multiples/layer_artist.py`

 * *Files identical despite different names*

### Comparing `glue-small-multiples-1.1.1/glue_small_multiples/qt/layer_style_editor.py` & `glue-small-multiples-1.1.2/glue_small_multiples/qt/layer_style_editor.py`

 * *Files identical despite different names*

### Comparing `glue-small-multiples-1.1.1/glue_small_multiples/qt/layer_style_editor.ui` & `glue-small-multiples-1.1.2/glue_small_multiples/qt/layer_style_editor.ui`

 * *Files 1% similar despite different names*

#### Comparing `glue-small-multiples-1.1.1/glue_small_multiples/qt/layer_style_editor.ui` & `glue-small-multiples-1.1.2/glue_small_multiples/qt/layer_style_editor.ui`

```diff
@@ -127,15 +127,15 @@
                     </size>
                   </property>
                 </spacer>
               </item>
               <item row="2" column="1" colspan="3">
                 <widget class="QComboBox" name="combosel_cmap_att">
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                 </widget>
               </item>
               <item row="0" column="1">
                 <widget class="QComboBox" name="combosel_cmap_mode">
                   <property name="maximumSize">
                     <size>
@@ -224,15 +224,15 @@
                   <property name="sizePolicy">
                     <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
                       <horstretch>0</horstretch>
                       <verstretch>0</verstretch>
                     </sizepolicy>
                   </property>
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                 </widget>
               </item>
             </layout>
           </widget>
           <widget class="QWidget" name="tab_2">
             <attribute name="title">
@@ -262,15 +262,15 @@
                   <property name="maximumSize">
                     <size>
                       <width>120</width>
                       <height>16777215</height>
                     </size>
                   </property>
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                 </widget>
               </item>
               <item row="0" column="0">
                 <widget class="QLabel" name="label">
                   <property name="font">
                     <font>
@@ -467,15 +467,15 @@
               </item>
               <item row="2" column="3">
                 <widget class="QSpinBox" name="value_size"/>
               </item>
               <item row="4" column="1" colspan="3">
                 <widget class="QComboBox" name="combosel_size_att">
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                 </widget>
               </item>
               <item row="0" column="1" colspan="3">
                 <widget class="QCheckBox" name="bool_markers_visible">
                   <property name="text">
                     <string/>
@@ -510,15 +510,15 @@
                   <property name="maximumSize">
                     <size>
                       <width>16777215</width>
                       <height>16777215</height>
                     </size>
                   </property>
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                 </widget>
               </item>
               <item row="9" column="0">
                 <widget class="QLabel" name="label_contrast">
                   <property name="font">
                     <font>
@@ -730,22 +730,22 @@
                     </size>
                   </property>
                 </spacer>
               </item>
               <item row="2" column="4">
                 <widget class="QComboBox" name="combosel_yerr_att">
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                 </widget>
               </item>
               <item row="1" column="4">
                 <widget class="QComboBox" name="combosel_xerr_att">
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                 </widget>
               </item>
               <item row="1" column="2">
                 <widget class="QCheckBox" name="bool_xerr_visible">
                   <property name="text">
                     <string/>
@@ -829,15 +829,15 @@
                     <string>Show arrow</string>
                   </property>
                 </widget>
               </item>
               <item row="3" column="1">
                 <widget class="QComboBox" name="combosel_vx_att">
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                 </widget>
               </item>
               <item row="1" column="0">
                 <widget class="QLabel" name="label_3">
                   <property name="font">
                     <font>
@@ -852,15 +852,15 @@
                     <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
                   </property>
                 </widget>
               </item>
               <item row="4" column="1">
                 <widget class="QComboBox" name="combosel_vy_att">
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                 </widget>
               </item>
               <item row="3" column="0">
                 <widget class="QLabel" name="label_vector_x">
                   <property name="font">
                     <font>
```

### Comparing `glue-small-multiples-1.1.1/glue_small_multiples/qt/options_widget.py` & `glue-small-multiples-1.1.2/glue_small_multiples/qt/options_widget.py`

 * *Files identical despite different names*

### Comparing `glue-small-multiples-1.1.1/glue_small_multiples/qt/options_widget.ui` & `glue-small-multiples-1.1.2/glue_small_multiples/qt/options_widget.ui`

 * *Files 1% similar despite different names*

#### Comparing `glue-small-multiples-1.1.1/glue_small_multiples/qt/options_widget.ui` & `glue-small-multiples-1.1.2/glue_small_multiples/qt/options_widget.ui`

```diff
@@ -66,15 +66,15 @@
                     <string>x axis</string>
                   </property>
                 </widget>
               </item>
               <item row="0" column="2">
                 <widget class="QComboBox" name="combosel_x_att">
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                 </widget>
               </item>
               <item row="0" column="3">
                 <widget class="QToolButton" name="bool_x_log_">
                   <property name="text">
                     <string>log</string>
@@ -96,15 +96,15 @@
                     <string>y axis</string>
                   </property>
                 </widget>
               </item>
               <item row="1" column="2">
                 <widget class="QComboBox" name="combosel_y_att">
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                 </widget>
               </item>
               <item row="1" column="3">
                 <widget class="QToolButton" name="bool_y_log_">
                   <property name="text">
                     <string>log</string>
```

### Comparing `glue-small-multiples-1.1.1/glue_small_multiples/qt/tests/data/penguins.csv` & `glue-small-multiples-1.1.2/glue_small_multiples/qt/tests/data/penguins.csv`

 * *Files identical despite different names*

### Comparing `glue-small-multiples-1.1.1/glue_small_multiples/qt/tests/test_axes.py` & `glue-small-multiples-1.1.2/glue_small_multiples/qt/tests/test_axes.py`

 * *Files identical despite different names*

### Comparing `glue-small-multiples-1.1.1/glue_small_multiples/qt/tests/test_data_viewer.py` & `glue-small-multiples-1.1.2/glue_small_multiples/qt/tests/test_data_viewer.py`

 * *Files identical despite different names*

### Comparing `glue-small-multiples-1.1.1/glue_small_multiples/qt/tests/test_save_restore.py` & `glue-small-multiples-1.1.2/glue_small_multiples/qt/tests/test_save_restore.py`

 * *Files identical despite different names*

### Comparing `glue-small-multiples-1.1.1/glue_small_multiples/qt/viewer.py` & `glue-small-multiples-1.1.2/glue_small_multiples/qt/viewer.py`

 * *Files identical despite different names*

### Comparing `glue-small-multiples-1.1.1/glue_small_multiples/state.py` & `glue-small-multiples-1.1.2/glue_small_multiples/state.py`

 * *Files identical despite different names*

### Comparing `glue-small-multiples-1.1.1/glue_small_multiples/utils.py` & `glue-small-multiples-1.1.2/glue_small_multiples/utils.py`

 * *Files identical despite different names*

### Comparing `glue-small-multiples-1.1.1/glue_small_multiples.egg-info/PKG-INFO` & `glue-small-multiples-1.1.2/glue_small_multiples.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-small-multiples
-Version: 1.1.1
+Version: 1.1.2
 Summary: A viewer for small multiples
 Home-page: https://www.gluesolutions.io
 Author: glue solutions, inc.
 Author-email: jfoster@gluesolutions.io
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `glue-small-multiples-1.1.1/setup.cfg` & `glue-small-multiples-1.1.2/setup.cfg`

 * *Files identical despite different names*

