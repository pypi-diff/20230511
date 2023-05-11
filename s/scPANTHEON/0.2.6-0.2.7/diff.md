# Comparing `tmp/scPANTHEON-0.2.6.tar.gz` & `tmp/scPANTHEON-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scPANTHEON-0.2.6.tar", last modified: Mon May  8 07:40:55 2023, max compression
+gzip compressed data, was "scPANTHEON-0.2.7.tar", last modified: Thu May 11 09:25:12 2023, max compression
```

## Comparing `scPANTHEON-0.2.6.tar` & `scPANTHEON-0.2.7.tar`

### file list

```diff
@@ -1,57 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.930051 scPANTHEON-0.2.6/
--rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0      261 2023-05-08 07:40:55.930051 scPANTHEON-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.878797 scPANTHEON-0.2.6/scPANTHEON.egg-info/
--rw-rw-rw-   0        0        0      261 2023-05-08 07:40:55.000000 scPANTHEON-0.2.6/scPANTHEON.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1721 2023-05-08 07:40:55.000000 scPANTHEON-0.2.6/scPANTHEON.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 07:40:55.000000 scPANTHEON-0.2.6/scPANTHEON.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-08 07:40:55.000000 scPANTHEON-0.2.6/scPANTHEON.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      100 2023-05-08 07:40:55.000000 scPANTHEON-0.2.6/scPANTHEON.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-08 07:40:55.000000 scPANTHEON-0.2.6/scPANTHEON.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.891432 scPANTHEON-0.2.6/scpantheon/
--rw-rw-rw-   0        0        0        0 2023-02-09 07:28:42.000000 scPANTHEON-0.2.6/scpantheon/__init__.py
--rw-rw-rw-   0        0        0     2323 2023-05-08 07:38:57.000000 scPANTHEON-0.2.6/scpantheon/bokeh_qt.py
--rw-rw-rw-   0        0        0     4162 2023-05-08 07:39:20.000000 scPANTHEON-0.2.6/scpantheon/data_qt.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.865349 scPANTHEON-0.2.6/scpantheon/extension/
-drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.893955 scPANTHEON-0.2.6/scpantheon/extension/Change_Color/
-drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.897305 scPANTHEON-0.2.6/scpantheon/extension/Change_Color/__pycache__/
--rw-rw-rw-   0        0        0     1691 2023-02-09 07:28:42.000000 scPANTHEON-0.2.6/scpantheon/extension/Change_Color/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     2286 2023-02-24 01:11:07.000000 scPANTHEON-0.2.6/scpantheon/extension/Change_Color/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     1776 2023-02-24 01:10:45.000000 scPANTHEON-0.2.6/scpantheon/extension/Change_Color/module.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.899307 scPANTHEON-0.2.6/scpantheon/extension/Check_Histogram/
-drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.901308 scPANTHEON-0.2.6/scpantheon/extension/Check_Histogram/__pycache__/
--rw-rw-rw-   0        0        0     4005 2023-03-16 11:08:13.000000 scPANTHEON-0.2.6/scpantheon/extension/Check_Histogram/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     4034 2023-03-11 03:04:00.000000 scPANTHEON-0.2.6/scpantheon/extension/Check_Histogram/module.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.903392 scPANTHEON-0.2.6/scpantheon/extension/Clustering_with_Scanpy/
-drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.906055 scPANTHEON-0.2.6/scpantheon/extension/Clustering_with_Scanpy/__pycache__/
--rw-rw-rw-   0        0        0     2896 2023-02-09 07:28:42.000000 scPANTHEON-0.2.6/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     3643 2023-02-23 14:39:59.000000 scPANTHEON-0.2.6/scpantheon/extension/Clustering_with_Scanpy/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     3181 2023-02-23 14:21:27.000000 scPANTHEON-0.2.6/scpantheon/extension/Clustering_with_Scanpy/module.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.908061 scPANTHEON-0.2.6/scpantheon/extension/Differential_Expression_Analysis/
-drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.911568 scPANTHEON-0.2.6/scpantheon/extension/Differential_Expression_Analysis/__pycache__/
--rw-rw-rw-   0        0        0     4423 2023-02-09 07:28:42.000000 scPANTHEON-0.2.6/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     5499 2023-02-23 14:40:38.000000 scPANTHEON-0.2.6/scpantheon/extension/Differential_Expression_Analysis/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     5496 2023-02-23 14:24:26.000000 scPANTHEON-0.2.6/scpantheon/extension/Differential_Expression_Analysis/module.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.913088 scPANTHEON-0.2.6/scpantheon/extension/Find_Marker_Gene/
-drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.917184 scPANTHEON-0.2.6/scpantheon/extension/Find_Marker_Gene/__pycache__/
--rw-rw-rw-   0        0        0     3786 2023-02-09 07:28:42.000000 scPANTHEON-0.2.6/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     4688 2023-02-23 14:40:47.000000 scPANTHEON-0.2.6/scpantheon/extension/Find_Marker_Gene/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     4694 2023-02-23 14:26:51.000000 scPANTHEON-0.2.6/scpantheon/extension/Find_Marker_Gene/module.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.919282 scPANTHEON-0.2.6/scpantheon/extension/Preprocessing_with_Scanpy/
-drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.922539 scPANTHEON-0.2.6/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/
--rw-rw-rw-   0        0        0     5877 2023-02-09 07:28:42.000000 scPANTHEON-0.2.6/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     5883 2023-02-17 13:16:06.000000 scPANTHEON-0.2.6/scpantheon/extension/Preprocessing_with_Scanpy/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0     7872 2023-02-23 14:33:09.000000 scPANTHEON-0.2.6/scpantheon/extension/Preprocessing_with_Scanpy/module.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.924942 scPANTHEON-0.2.6/scpantheon/extension/TOMAS/
-drwxrwxrwx   0        0        0        0 2023-05-08 07:40:55.928035 scPANTHEON-0.2.6/scpantheon/extension/TOMAS/__pycache__/
--rw-rw-rw-   0        0        0     7544 2023-02-09 07:28:42.000000 scPANTHEON-0.2.6/scpantheon/extension/TOMAS/__pycache__/module.cpython-38.pyc
--rw-rw-rw-   0        0        0     9069 2023-02-23 14:40:54.000000 scPANTHEON-0.2.6/scpantheon/extension/TOMAS/__pycache__/module.cpython-39.pyc
--rw-rw-rw-   0        0        0    10919 2023-02-23 14:39:22.000000 scPANTHEON-0.2.6/scpantheon/extension/TOMAS/module.py
--rw-rw-rw-   0        0        0     1162 2023-05-08 06:41:40.000000 scPANTHEON-0.2.6/scpantheon/main.py
--rw-rw-rw-   0        0        0     5627 2023-05-08 06:44:29.000000 scPANTHEON-0.2.6/scpantheon/qt.py
--rw-rw-rw-   0        0        0      401 2023-02-09 07:28:42.000000 scPANTHEON-0.2.6/scpantheon/run.py
--rw-rw-rw-   0        0        0    59203 2023-04-20 04:56:28.000000 scPANTHEON-0.2.6/scpantheon/source.py
--rw-rw-rw-   0        0        0      634 2023-02-09 07:28:42.000000 scPANTHEON-0.2.6/scpantheon/transform.py
--rw-rw-rw-   0        0        0       42 2023-05-08 07:40:55.931554 scPANTHEON-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1084 2023-05-08 06:46:02.000000 scPANTHEON-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:25:12.987231 scPANTHEON-0.2.7/
+-rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      261 2023-05-11 09:25:12.987231 scPANTHEON-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 09:25:12.973437 scPANTHEON-0.2.7/scPANTHEON.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-05-11 09:25:12.000000 scPANTHEON-0.2.7/scPANTHEON.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-05-11 09:25:12.000000 scPANTHEON-0.2.7/scPANTHEON.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 09:25:12.000000 scPANTHEON-0.2.7/scPANTHEON.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-11 09:25:12.000000 scPANTHEON-0.2.7/scPANTHEON.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      100 2023-05-11 09:25:12.000000 scPANTHEON-0.2.7/scPANTHEON.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-11 09:25:12.000000 scPANTHEON-0.2.7/scPANTHEON.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 09:25:12.985653 scPANTHEON-0.2.7/scpantheon/
+-rw-rw-rw-   0        0        0        0 2023-02-09 07:28:42.000000 scPANTHEON-0.2.7/scpantheon/__init__.py
+-rw-rw-rw-   0        0        0     2323 2023-05-08 07:38:57.000000 scPANTHEON-0.2.7/scpantheon/bokeh_qt.py
+-rw-rw-rw-   0        0        0     4162 2023-05-08 07:39:20.000000 scPANTHEON-0.2.7/scpantheon/data_qt.py
+-rw-rw-rw-   0        0        0     1162 2023-05-08 06:41:40.000000 scPANTHEON-0.2.7/scpantheon/main.py
+-rw-rw-rw-   0        0        0     5627 2023-05-08 06:44:29.000000 scPANTHEON-0.2.7/scpantheon/qt.py
+-rw-rw-rw-   0        0        0      401 2023-02-09 07:28:42.000000 scPANTHEON-0.2.7/scpantheon/run.py
+-rw-rw-rw-   0        0        0    59652 2023-05-11 09:24:08.000000 scPANTHEON-0.2.7/scpantheon/source.py
+-rw-rw-rw-   0        0        0      634 2023-02-09 07:28:42.000000 scPANTHEON-0.2.7/scpantheon/transform.py
+-rw-rw-rw-   0        0        0       42 2023-05-11 09:25:12.988234 scPANTHEON-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1084 2023-05-11 09:25:10.000000 scPANTHEON-0.2.7/setup.py
```

### Comparing `scPANTHEON-0.2.6/scpantheon/bokeh_qt.py` & `scPANTHEON-0.2.7/scpantheon/bokeh_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.6/scpantheon/data_qt.py` & `scPANTHEON-0.2.7/scpantheon/data_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.6/scpantheon/main.py` & `scPANTHEON-0.2.7/scpantheon/main.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.6/scpantheon/qt.py` & `scPANTHEON-0.2.7/scpantheon/qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.6/scpantheon/source.py` & `scPANTHEON-0.2.7/scpantheon/source.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,17 +27,16 @@
 
 TOOLTIPS = [
         ("(x,y)", "($x, $y)"),
         ("color", "@color"),
 ]
 class FlowPlot:
     global data_file
-    def __init__(self, data=None, pdata=None, color_map=None, x_init_idx = 0, y_init_idx = 1, allow_select = True, select_color_change = True, main_plot = None,title=None): # - legend=None
+    def __init__(self, data=None, color_map=None, x_init_idx = 0, y_init_idx = 1, allow_select = True, select_color_change = True, main_plot = None,title=None): # - legend=None
         self.adata = data
-        self.pdata = pdata
         self.data_df = self.adata.to_df()
         self.data_log = np.log1p(self.data_df)    
         # For real-valued input, log1p is accurate also for x so small that 1 + x == 1 in floating-point accuracy.
         self.label_existed, view_existed = False, False
         # personalized
         try:
             group_list = list(self.adata.uns['category_dict'].keys()) 
@@ -290,27 +289,32 @@
         self.s_x.completions = column_list
         self.s_y.completions = column_list
 
         print(column_list)
 
     def save_profile(self):
         self.button_disabled()
-        def next_save():
+        def next_save(self):
             path = 'result/'
-            self.adata.write(path+'result.h5ad')
-            self.adata.obs.to_csv(path+'cluster.csv')
+            try:
+                self.adata.write(path+'result.h5ad') 
+                self.adata.obs.to_csv(path+'cluster.csv')
+            except:
+                os.makedirs(path)
+                self.adata.write(path+'result.h5ad') # ??
+                self.adata.obs.to_csv(path+'cluster.csv')
             # for cate in list(self.adata.uns['category_dict'].keys()):
             #     self.adata.obs[cate].to_csv(path+'%s.csv'%cate)
             #adata.uns['category_dict']('cluster name.csv') 
             self.button_abled()
-        curdoc().add_next_tick_callback(next_save)
+        curdoc().add_next_tick_callback(lambda : next_save(self))
 
     def tag_func(self, selector, effector, attr, plot):
         self.button_disabled()
-        def tag():
+        def tag(self, selector, effector, attr, plot):
             axis = getattr(plot, attr + "axis")
             old_name = axis.axis_label
             print('axis_label=====', axis.axis_label)
             data = pandas.DataFrame(self.source.data) 
             if plot.xaxis.axis_label != plot.yaxis.axis_label:           
                 data.drop(labels=old_name, axis=1, inplace=True)
             axis.axis_label = selector.value
@@ -327,199 +331,200 @@
                 data.loc[:,selector.value] = pandas.Series(list(self.data_log[selector.value]), index=data.index) 
             
             data.drop(labels='index', axis=1, inplace=True)
             print(data)
             self.source.data = data
             setattr(effector, attr, selector.value)
             self.button_abled()
-        curdoc().add_next_tick_callback(tag)
+        curdoc().add_next_tick_callback(lambda : tag(self, selector, effector, attr, plot))
 
     # Log
     def log_cb(self):
         self.button_disabled()
-        def log():
+        def log(self):
             data = pandas.DataFrame(self.source.data) 
             data.drop(labels='index', axis=1, inplace=True)
             axis_label = data.columns
             names = []
             for name in axis_label:
                 if name not in ['color', 'hl_gene']:
                     names = names + [name]
                     if self.log_axis.active == []:
                         data[name] = pandas.DataFrame(list(self.data_df[name]), index=data.index) 
                     else:
                         data[name] = pandas.DataFrame(list(self.data_log[name]), index=data.index) 
             self.source.data = data
             self.button_abled()
-        curdoc().add_next_tick_callback(log)
+        curdoc().add_next_tick_callback(lambda : log(self))
 
     # Callback of colorpicker(selection), update the selected dots with picked color
     def select_color_func(self):
         self.button_disabled()
-        def select():
+        def select(self):
             self.cur_color = self.color_selection.color
             self.r.selection_glyph.fill_color = self.cur_color
             # Just to trigger plot update 
             self.source.data["color"] = self.source.data["color"]
             print('now color',self.r.selection_glyph.fill_color)
             self.button_abled()
-        curdoc().add_next_tick_callback(select)
+        curdoc().add_next_tick_callback(lambda : select(self))
 
     # Show all, gate, and remove function
     def gate_func(self):
         self.button_disabled()
-        def next_gate():
+        def next_gate(self):
             if len(self.view.filters) != 0:
                 indices = list(set(self.source.selected.indices)&set(self.view.filters[0].indices))
             else:
                 indices = self.source.selected.indices
             self.view.filters = [IndexFilter(indices)]
             self.button_abled()
-        curdoc().add_next_tick_callback(next_gate)
+        curdoc().add_next_tick_callback(lambda : next_gate(self))
 
     def remove_func(self):
         self.button_disabled()
-        def next_remove():
+        def next_remove(self):
             if len(self.view.filters) == 0:
                 self.view.filters = [IndexFilter(np.object_(range(self.data_df.shape[0])))]
             remain_indices = [x for x in self.view.filters[0].indices if x not in self.source.selected.indices]
             self.view.filters = [IndexFilter(remain_indices)]
             self.button_abled()
-        curdoc().add_next_tick_callback(next_remove)
+        curdoc().add_next_tick_callback(lambda : next_remove)
 
     def showall_func(self):
         self.button_disabled()
         def next_showall():
             self.view.filters = list([])
             self.button_abled()
-        curdoc().add_next_tick_callback(next_showall)
+        curdoc().add_next_tick_callback(lambda : next_showall(self))
 
     # Show the saved color of dots
     def correct_func(self):
         self.source.selected.indices = []
 
 
     # Select class group
     def choose_cat(self):
         self.button_disabled()
-        def cat():
+        def cat(self):
             try: 
                 self.adata.uns['category_dict'][self.group.value]['class_name'][0]
                 self.update_checkbox()
                 print(self.adata.uns['category_dict'][self.group.value])
                 self.class_checkbox.active = [0]
                 self.show_color()
             except:
                 self.class_checkbox.labels = ['Unassigned: color=grey, cell_nums=' + str(self.data_df.shape[0])]
                 self.class_checkbox.active = []
             #self.text_color()
             self.button_abled()
-        curdoc().add_next_tick_callback(cat)
+        curdoc().add_next_tick_callback(lambda : cat(self))
 
     # New Category
     def new_category(self):
         self.button_disabled()
-        def next_category():
+        def next_category(self):
             if self.group_name.value == '':
                 marker = str(self.p.xaxis.axis_label) + '+' + str(self.p.yaxis.axis_label)
             else:
                 marker = self.group_name.value
             self.adata.uns['category_dict'][marker] = pandas.DataFrame(columns=['class_name','color','cell_num'])
             self.adata.obs[marker] = pandas.Series(index=self.data_df.index,dtype=object)
             self.group.options = list(self.adata.uns['category_dict'].keys())
             self.group.value = marker
             self.group_name.value = ''
             #print('new group',self.group.value, marker,self.group.options, '=')
             self.button_abled()
-        curdoc().add_next_tick_callback(next_category)
+        curdoc().add_next_tick_callback(lambda : next_category(self))
 
     # Rename category
     def edit_category(self):   
         self.button_disabled()
-        def next_edit():
+        def next_edit(self):
             old_name = self.group.value
             new_name = self.group_name.value
             self.adata.obs[new_name] = self.adata.obs.pop(old_name)
             self.adata.uns['category_dict'][new_name] = self.adata.uns['category_dict'].pop(old_name)
             self.group.options = list(self.adata.uns['category_dict'].keys())
             self.group.value = new_name
             print(self.adata.uns['category_dict'])
             self.button_abled()
-        curdoc().add_next_tick_callback(next_edit)
+        curdoc().add_next_tick_callback(lambda : next_edit(self))
 
     # Delete category
     def del_category(self):
         self.button_disabled()
-        def next_del():
+        def next_del(self):
             del self.adata.uns['category_dict'][self.group.value]   
             del self.adata.obs[self.group.value]
             self.group.options = list(self.adata.uns['category_dict'].keys())
             if len(self.group.options) == 0:
                 self.group.value = ''
             else:
                 self.group.value = self.group.options[0]
             self.button_abled()
-        curdoc().add_next_tick_callback(next_del)
+        curdoc().add_next_tick_callback(lambda : next_del(self))
 
     #### Class Callback Function #####
     # Update the label of class checkbox
     def update_checkbox(self):
         self.button_disabled()
-        def updata():
+        def updata(self):
             cate = self.group.value
             group_list = self.adata.uns['category_dict'][cate]['class_name']
             #print('=====', group_list[0],group_list[1])
             cls_label = []
             num = 0
-            for i in range(self.adata.uns['category_dict'][cate].shape[0]):
+            # for i in range(self.adata.uns['category_dict'][cate].shape[0]):
+            for i in range(len(group_list)):
                 class_name = group_list[i]
                 cell_num = len(self.data_df[self.adata.obs[cate]==group_list[i]])       
                 s = str(class_name) +  ': cell_nums=' + str(cell_num)
                 cls_label = np.append(cls_label,s)
                 num = num + cell_num
             cls_label = np.append(cls_label,str('Unassigned: color=grey, cell_nums=' + str(self.data_df.shape[0]-num))) 
             self.class_checkbox.labels = list(cls_label)
             #self.text_color()
             self.button_abled()
-        curdoc().add_next_tick_callback(updata)
+        curdoc().add_next_tick_callback(lambda : updata(self))
 
     def show_checked(self):
         self.button_disabled()
-        def next_show():
+        def next_show(self):
             group = self.group.value
             group_list = self.adata.uns['category_dict'][group]['class_name']
             #source.selected.indices = temp[temp[cat_opt.value]==str(self.class_checkbox.active[0])].index
             self.source.selected.indices = list(self.adata.obs[self.adata.obs[group].isin(list(group_list[i] for i in self.class_checkbox.active))]['ind'])
             self.show_color()
             self.button_abled()
-            curdoc().add_next_tick_callback(next_show)
+        curdoc().add_next_tick_callback(lambda : next_show(self))
 
     # Show color on checkbox
     def text_color(self):
         self.button_disabled()
-        def next_text():
+        def next_text(self):
             color_js = ''
             try:
                 length = len(self.adata.uns['category_dict'][self.group.value]['color']) 
                 for i in range(length):
                     color_js = color_js + self.adata.uns['category_dict'][self.group.value]['color'][i] + ' '
                 self.para_color.text = color_js + color_list[18]
             except:
                 length = 1
                 #color_js = [color_list[18]]
                 self.para_color.text = str(color_list[18])
             self.trigger_color.text = self.trigger_color.text + '1'
             #print('CALL',color_js)
             self.button_abled()
-        curdoc().add_next_tick_callback(next_text)
+        curdoc().add_next_tick_callback(lambda : next_text(self))
 
     # Save change of classes
     def save_class(self, cate, class_name, color, n):
         self.button_disabled()
-        def save():
+        def save(self, cate):
             if n == 0:
                 ind = len(self.class_checkbox.labels)-1
             else:
                 ind = self.class_checkbox.active[0]  
             class_label = list(self.adata.obs[cate])
             group_list = self.adata.uns['category_dict'][cate]['class_name']
             print(group_list)
@@ -531,39 +536,39 @@
             cate = self.group.value
             self.update_checkbox()
             self.class_checkbox.active = [ind]
             self.show_color()
             self.correct_func()
             #self.text_color()
             self.button_disabled()
-        curdoc().add_next_tick_callback(save)
+        curdoc().add_next_tick_callback(lambda : save(self, cate))
 
     # New Class
     def add_entry(self):
         self.button_disabled()
-        def next_add_entry():
+        def next_add_entry(self):
             xaxis = str(self.p.xaxis.axis_label)
             yaxis = str(self.p.yaxis.axis_label)
             #if str(cat_opt.value) != xaxis+'+'+yaxis and str(cat_opt.value) != yaxis+'+'+xaxis:
             if self.group.value == ' ':
                 print(str(self.group.value),xaxis+'+'+yaxis)
                 #self.class_checkbox.labels = ['no cluster: color=' + color_list[18] + ', cell_nums=' + str(self.data_df.shape[0])]
                 self.new_category()       
             cell_num = len(self.source.selected.indices)
             print('add cluster',self.group.value)
             self.adata.uns['category_dict'][self.group.value].loc[len(self.adata.uns['category_dict'][self.group.value])] = {'class_name':self.class_name.value,'color':self.cur_color,'cell_num':cell_num}
             self.save_class(self.group.value, self.class_name.value, self.cur_color, 0)
             self.class_name.value = ''
             self.button_abled()
-        curdoc().add_next_tick_callback(next_add_entry)
+        curdoc().add_next_tick_callback(lambda : next_add_entry(self))
 
     # Merge checked classes
     def merge(self):
         self.button_disabled()
-        def next_merge():
+        def next_merge(self):
             group = self.group.value
             if self.class_name.value == '':
                 toclass = self.adata.uns['category_dict'][group]['class_name'][self.class_checkbox.active[0]]
                 color = self.adata.uns['category_dict'][group]['color'][self.class_checkbox.active[0]]
             else:
                 toclass = self.class_name.value
                 color = self.cur_color
@@ -591,20 +596,20 @@
             del_list2 = del_list2 + [tt]
             self.class_checkbox.labels = del_list2
             self.class_checkbox.active = []
             col_list = [color if self.source.data['color'][i] in checked_color else self.source.data['color'][i] for i in range(self.data_df.shape[0])]
             self.source.data['color'] = col_list
             # self.text_color()
             self.button_abled()
-        curdoc().add_next_tick_callback(next_merge)
+        curdoc().add_next_tick_callback(lambda : next_merge(self))
 
     # Delete Class
     def del_class(self):
         self.button_disabled()
-        def next_del_claass():
+        def next_del_claass(self):
             group = self.group.value
             cluster_list = self.adata.uns['category_dict'][group]['class_name']
             self.adata.obs.loc[self.adata.obs[group].isin([cluster_list[i] for i in self.class_checkbox.active]),group] = np.nan
             checked_color = [self.adata.uns['category_dict'][group].loc[i,'color'] for i in self.class_checkbox.active]
             self.adata.uns['category_dict'][group].drop(index=self.class_checkbox.active,inplace=True)
             
             del_list2 = self.class_checkbox.labels
@@ -614,15 +619,15 @@
             self.class_checkbox.labels = del_list2
             self.class_checkbox.active = []
             self.adata.uns['category_dict'][group] = pandas.DataFrame(self.adata.uns['category_dict'][group], index=list(range(self.adata.uns['category_dict'][group].shape[0])))
             col_list = [color_list[18] if self.source.data['color'][i] in checked_color else self.source.data['color'][i] for i in range(self.data_df.shape[0])]
             self.source.data['color'] = col_list
             # self.text_color()
             self.button_abled()
-        curdoc().add_next_tick_callback(next_del_claass)
+        curdoc().add_next_tick_callback(lambda : next_del_claass(self))
 
     # Rename class
     def rename(self):
         ind = self.class_checkbox.active[0]
         print('rename ind:',ind)
         cell_num = self.adata.uns['category_dict'][self.group.value]['cell_num'][ind]
 
@@ -639,88 +644,88 @@
         self.class_checkbox.labels = labels
 
         #self.text_color()
 
     # Add dots to cluster
     def save_cls_button(self):
         self.button_disabled()
-        def next_save():
+        def next_save(self):
             class_name = self.adata.uns['category_dict'][self.group.value]['class_name'][self.class_checkbox.active[0]]
             color = self.adata.uns['category_dict'][self.group.value]['color'][self.class_checkbox.active[0]]
             cell_num = len(self.source.selected.indices)
             self.save_class(self.group.value, class_name, color, cell_num)
             print(self.adata.uns['category_dict'][self.group.value])
             self.button_abled()
-        curdoc().add_next_tick_callback(next_save)
+        curdoc().add_next_tick_callback(lambda : next_save(self))
 
     # Remove dots from cluster
     def remove_dot(self):
         self.button_disabled()
-        def next_remove():
+        def next_remove(self):
             cl_label = self.adata.obs[self.group.value]
             checked_list = list(self.adata.uns['category_dict'][self.group.value].loc[[j for j in self.class_checkbox.active],'class_name'])
             print(checked_list)
             for i in self.source.selected.indices:
                 if cl_label[i] in checked_list:
                     cl_label[i] = np.nan
             self.adata.obs[self.group.value] = cl_label
             self.update_checkbox()
             self.show_color()
             self.button_abled()
-        curdoc().add_next_tick_callback(next_remove)
+        curdoc().add_next_tick_callback(lambda : next_remove(self))
 
     # Update class
     def update_clus(self):
         self.button_disabled()
-        def next_update():
+        def next_update(self):
             ind = self.class_checkbox.active[0]
             #adata.obs[adata.obs[cat_opt.value]==str(ind)].loc[cat_opt.value] = pandas.Series(index=[0],dtype=object)[0]
             cl_label = self.adata.obs[self.group.value]
             group_list = self.adata.uns['category_dict'][self.group.value]['class_name']
             cl_label[self.adata.obs[self.group.value]==group_list[ind]] = np.NAN
             for i in self.source.selected.indices:
                 cl_label[i] = group_list[ind]
             self.adata.obs[self.group.value] = cl_label
             self.update_checkbox()
             self.show_color()
             #self.text_color()
             self.button_abled()
-        curdoc().add_next_tick_callback(next_update)
+        curdoc().add_next_tick_callback(lambda : next_update(self))
 
     # change color of class
     def change_color(self):
         self.button_disabled()
-        def next_color():
+        def next_color(self):
             color_l = self.source.data['color']
             self.show_checked()
             for i in self.source.selected.indices:
                 color_l[i] = self.cur_color
             self.source.data['color'] = color_l
             self.adata.uns['category_dict'][self.group.value]['color'][[i for i in self.class_checkbox.active]] = self.cur_color
             self.text_color()
             #print(hide.value,now_color)
             self.button_abled()
-        curdoc().add_next_tick_callback(next_color)
+        curdoc().add_next_tick_callback(lambda : next_color(self))
 
     #### Highly variable gene functions #####
     def show_colorbar(self, marker):
         self.button_disabled()
-        def show():
+        def show(self, marker):
             if marker:
                 updated_color = self.data_df.loc[:,self.ct_marker.value]
             else:
                 updated_color = self.data_df.loc[:,self.hl_input.value]
             updated_color = (updated_color-min(updated_color))*(self.hl_bar_map.high - self.hl_bar_map.low)/(max(updated_color)-min(updated_color))
             self.source.data["hl_gene"] = list(updated_color) 
             self.button_abled()
-        curdoc().add_next_tick_callback(show)
+        curdoc().add_next_tick_callback(lambda : show(self, marker))
     
     def hl_filter(self):
         self.button_disabled()
-        def h1():
+        def h1(self):
             if self.view.filters == []:
                 filter_list = list(range(self.data_df.shape[0]))
             else:
                 print(self.view.filters)
                 filter_list = list(self.view.filters[0].indices)
             if self.hl_filt.value == 'Gene Expression >':
                 index_list = list(self.adata.obs[self.data_df[self.hl_input.value] > float(self.hl_filt_num.value)]['ind'])
@@ -730,81 +735,80 @@
                 index_list = list(self.adata.obs[self.data_df[self.hl_input.value] == float(self.hl_filt_num.value)]['ind'])
             index_list = set(index_list)&set(filter_list)
             self.source.selected.indices = list(index_list)
             #new_r = show_colorbar()
             self.r.selection_glyph = Circle(fill_alpha=1,fill_color='Black')
             #print(self.source.selected.indices)
             self.button_abled()
-        curdoc().add_next_tick_callback(h1)
+        curdoc().add_next_tick_callback(lambda : h1(self))
 
     def marker_choice(self):
         self.button_abled()
-        def marker():
+        def marker(self):
             print('filename change: ',self.marker_file.filename)
             if True:
                 marker = pandas.read_csv('data/' + self.marker_file.filename)
 
                 cell_type = list(set(marker['cell_type']))
                 print(cell_type)
                 self.cell_type.options = ['No cell type'] + cell_type
                 self.cell_type.value = cell_type[0]
                 #self.change_marker_ct()
             else:
                 print('PROBLEM')
                 attention = Div(text='No marker gene list found!')
                 curdoc().add_root(attention)
             self.button_abled()
-        curdoc().add_next_tick_callback(marker)
+        curdoc().add_next_tick_callback(lambda : marker(self))
 
     def change_marker_ct(self):
         self.button_disabled()
-        def ct():
+        def ct(self):
             cell_type = self.cell_type.value
             marker = pandas.read_csv('data/' + self.marker_file.filename)
             print('+++++++marker gene')
             marker_list = list(marker[marker['cell_type']==cell_type].loc[:,'marker_gene'])
             self.ct_marker.options = marker_list
             self.ct_marker.value = marker_list[0]
             self.button_abled()
-        curdoc().add_next_tick_callback(ct)
+        curdoc().add_next_tick_callback(lambda : ct(self))
 
 
     def change_select(self, main_plot):
         main_plot.source.selected.indices = self.source.selected.indices
 
     def change_view(self,main_plot):
         self.button_disabled()
-        def view():
+        def view(self,main_plot):
             self.source.data = dict(main_plot.source.data)
             self.adata = main_plot.adata
-            self.pdata = main_plot.pdata
             self.data_df = main_plot.data_df
             self.r.glyph.x = main_plot.r.glyph.x
             self.r.glyph.y = main_plot.r.glyph.y
             self.p.xaxis.axis_label = main_plot.p.xaxis.axis_label
             self.p.yaxis.axis_label = main_plot.p.yaxis.axis_label
             self.view.filters = main_plot.view.filters
             self.button_abled()
-        curdoc().add_next_tick_callback(view)
+        curdoc().add_next_tick_callback(lambda : view(self,main_plot))
 
     #### Other Functions ####
     # Show color of category
     def show_color(self):
         self.button_disabled()
-        def color():
+        def color(self):
             col_list = [color_list[18] for i in range(self.data_df.shape[0])]
             #print(col_list)
             for i in range(len(self.adata.uns['category_dict'][self.group.value])):
                 #print(self.adata.obs.columns)
                 inds = list(self.adata.obs[self.adata.obs[self.group.value]==self.adata.uns['category_dict'][self.group.value]['class_name'][i]]['ind'])
                 color = self.adata.uns['category_dict'][self.group.value]['color'][i]
                 col_list = [color if j in inds else col_list[j] for j in range(len(col_list))] 
             self.source.data['color'] = col_list
             self.button_abled()
-        curdoc().add_next_tick_callback(color)
+        curdoc().add_next_tick_callback(lambda : color(self))
 
 class data_trans():
     def __init__(self,
                  x_label,
                  data_color,
                  selected_color,
                  checked_class,
@@ -821,26 +825,25 @@
         self.showing_indices = showing_indices
 
 
 
 
 class CreateTool:
     
-    def __init__(self,adata,pdata):
+    def __init__(self,adata):
         self.adata = adata
-        self.pdata = pdata
         self.hl_gene_map = log_cmap('hl_gene', cc.kbc[::-1], low=1, high=20) # color log map
 
     def set_function(self, effector, attr, value):
         setattr(effector, attr, value)
         
     def base_tool(self):        
         # module_checkbox = CheckboxGroup(labels=load_options(),active=[],name='modules_checkbox') 
         module_select = Select(title='Choose Functions to Add:', options=load_options(), value='', name='modules_select') 
-        Figure = FlowPlot(data=self.adata, pdata=self.pdata, color_map='color')
+        Figure = FlowPlot(data=self.adata, color_map='color')
 
         layout=row(column(Figure.p, Figure.show_gene_list, Figure.show_plot, Figure.para_color, Figure.trigger_color, module_select), # module_checkbox added
             column(Figure.choose_panel,Figure.s_x, Figure.s_y, Figure.log_axis, Figure.color_selection, Figure.gate_button, Figure.remove_button, Figure.showall_button, Figure.export_button),
             column(Figure.group, Figure.group_name, Figure.create_group, Figure.rename_group, Figure.delete_group,
              Figure.class_name, Figure.new_class, Figure.checkbox_color, Figure.class_checkbox),
             column(Figure.show_selected_class, Figure.add_to, Figure.remove_from, Figure.update_class,
              Figure.rename_class,  Figure.merge_class, Figure.delete_class))
@@ -848,15 +851,15 @@
         # attr refers to the changed attribute’s name, and old and new refer to the previous and updated values of the attribute
         # module_checkbox.on_change('active', lambda attr, old, new: load_module(list(module_checkbox.active))) 
         # active: The list of indices of selected check boxes.
         module_select.on_change('value', lambda attr, old, new: load_module(module_select.value)) 
         return Figure, layout
     
     def highlight_gene(self, main_plot):
-        hl_figure = FlowPlot(data=self.adata, pdata=self.pdata, color_map=self.hl_gene_map, main_plot=main_plot,title='Highlight Gene Plot') # input main_plot
+        hl_figure = FlowPlot(data=self.adata, color_map=self.hl_gene_map, main_plot=main_plot,title='Highlight Gene Plot') # input main_plot
         #hl_figure.p.visible = False
         #hl_figure.marker_choice()
         layout = row(hl_figure.p, 
                  column(hl_figure.marker_file, hl_figure.cell_type, hl_figure.ct_marker, hl_figure.show_marker, hl_figure.hl_input, hl_figure.hl_button, 
                  row(hl_figure.hl_filt, hl_figure.hl_filt_num),hl_figure.hl_filt_button,hl_figure.hl_comfirm))
 
         return hl_figure, layout
@@ -905,18 +908,14 @@
         self.Figure.view.filters = [IndexFilter(d['showing_indices'])]
         print(len(self.Figure.view.filters[0].indices))
     
     def get_anndata(self):
         adata = self.Figure.adata.copy()
         return adata
 
-    def get_pandata(self):
-        pdata = self.Figure.pdata.copy()
-        return pdata
-    
     def set_anndata(self, adata):
         self.Figure.adata = adata
         data_df = self.Figure.data_df
         data_log = self.Figure.data_log
         if len(data_df.index) != len(self.Figure.adata.obs_names):
             indices = list(set(data_df.index) - set(self.Figure.adata.obs_names))
             data_df.drop(index=indices, axis=0, inplace=True)
@@ -1158,36 +1157,33 @@
     print('===loading finished=====')
     filename = os.path.split(data_file)[1]      
     def load():
         global Main_plot
         filetype = os.path.splitext(filename)[-1][1:] # split the filename and the type
                                                       # [-1] means the last tuple: the type 
         if filetype == 'csv':
-            adata = anndata.read_csv(data_file) 
-            pdata = pandas.read_csv(data_file, index_col=0)
+            adata = sc.read_csv(data_file) 
             print('csv')
         elif filetype == 'h5ad':
-            adata = anndata.read(data_file)
-            pdata = pandas.read(data_file, index_col=0)
+            adata = sc.read_h5ad(data_file)
             print('h5ad')
         elif filetype == 'mtx':
             adata = sc.read_10x_mtx(
                 'data/hg19/',  # the directory with the `.mtx` file
                 var_names='gene_symbols',                # use gene symbols for the variable names (variables-axis index)
                 cache=True)                              # write a cache file for faster subsequent reading
-            pdata = adata
         print(data_file)
         # Figure, layout
-        mainplot, panel1 = CreateTool(adata=adata,pdata=pdata).base_tool() # Mainplot: figure, layout
+        mainplot, panel1 = CreateTool(adata=adata).base_tool() # Mainplot: figure, layout
         print('===mainplot finished=====')
         Main_plot = mainplot
         # Highlight Gene Figure,
-        hl_figure, panel2 = CreateTool(adata=adata,pdata=pdata).highlight_gene(mainplot)
+        hl_figure, panel2 = CreateTool(adata=adata).highlight_gene(mainplot)
         print('====highlight finished=====')
-        tab = CreateTool(adata,pdata).multi_panel([mainplot,hl_figure], [panel1,panel2], ['Main View', 'Highlight Gene'], update_view=True)
+        tab = CreateTool(adata).multi_panel([mainplot,hl_figure], [panel1,panel2], ['Main View', 'Highlight Gene'], update_view=True)
         print('====tab====')
         curdoc().remove_root(loading_remind)
         curdoc().add_root(tab)
         print('===finish===')
 
     curdoc().add_next_tick_callback(load)
```

### Comparing `scPANTHEON-0.2.6/scpantheon/transform.py` & `scPANTHEON-0.2.7/scpantheon/transform.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.6/setup.py` & `scPANTHEON-0.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 # python setup.py sdist bdist_wheel
 # python -m twine upload dist/*
 
 setup(
     name='scPANTHEON',# 需要打包的名字,即本模块要发布的名字
-    version='0.2.6',#版本
+    version='0.2.7',#版本
     description='A graphical interface for single cell analysis.', # 简要描述
     packages=['scpantheon'],   #  需要打包的模块
     author='xinzhu', # 作者名
     author_email='xinzhu.jiang@sjtu.edu.cn',   # 作者邮件
     url='https://github.com/xinzhu-email/Pantheon', # 项目地址,一般是代码托管的网站
     install_requires=['bokeh==2.4.3','pandas','anndata','colorcet','scanpy','numpy','PyQt5','PyQtWebEngine',
                         'appdirs==1.4.4'], # 依赖包,如果没有,可以不要
```

