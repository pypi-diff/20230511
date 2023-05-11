# Comparing `tmp/irene_pro-0.0.23.tar.gz` & `tmp/irene_pro-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.23.tar", last modified: Sun May  7 10:59:43 2023, max compression
+gzip compressed data, was "irene_pro-0.0.26.tar", last modified: Thu May 11 09:10:54 2023, max compression
```

## Comparing `irene_pro-0.0.23.tar` & `irene_pro-0.0.26.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 10:59:43.306898 irene_pro-0.0.23/
--rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.23/LICENSE
--rw-rw-rw-   0        0        0     2406 2023-05-07 10:59:43.303902 irene_pro-0.0.23/PKG-INFO
--rw-rw-rw-   0        0        0     1827 2023-05-07 10:49:50.000000 irene_pro-0.0.23/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 10:59:43.274980 irene_pro-0.0.23/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-05-04 07:11:13.000000 irene_pro-0.0.23/irene_pro/__init__.py
--rw-rw-rw-   0        0        0    24162 2023-05-07 10:44:54.000000 irene_pro-0.0.23/irene_pro/gui.py
--rw-rw-rw-   0        0        0    11620 2023-05-01 10:00:44.000000 irene_pro-0.0.23/irene_pro/others.py
-drwxrwxrwx   0        0        0        0 2023-05-07 10:59:43.299914 irene_pro-0.0.23/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     2406 2023-05-07 10:59:43.000000 irene_pro-0.0.23/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-05-07 10:59:43.000000 irene_pro-0.0.23/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 10:59:43.000000 irene_pro-0.0.23/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-05-07 10:59:43.000000 irene_pro-0.0.23/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-07 10:59:43.000000 irene_pro-0.0.23/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 10:59:43.307929 irene_pro-0.0.23/setup.cfg
--rw-rw-rw-   0        0        0     2370 2023-05-07 10:58:51.000000 irene_pro-0.0.23/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:10:54.194740 irene_pro-0.0.26/
+-rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.26/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.26/MANIFEST.in
+-rw-rw-rw-   0        0        0     1280 2023-05-11 09:10:54.191749 irene_pro-0.0.26/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2023-05-11 07:56:46.000000 irene_pro-0.0.26/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 09:10:54.129606 irene_pro-0.0.26/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.26/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     1445 2023-05-11 07:54:52.000000 irene_pro-0.0.26/irene_pro/logic.py
+-rw-rw-rw-   0        0        0    24835 2023-05-11 07:56:04.000000 irene_pro-0.0.26/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-05-11 09:10:54.184766 irene_pro-0.0.26/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1280 2023-05-11 09:10:53.000000 irene_pro-0.0.26/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-11 09:10:53.000000 irene_pro-0.0.26/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 09:10:53.000000 irene_pro-0.0.26/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-11 09:10:53.000000 irene_pro-0.0.26/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-11 09:10:53.000000 irene_pro-0.0.26/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 09:10:54.195737 irene_pro-0.0.26/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-05-11 07:52:27.000000 irene_pro-0.0.26/setup.py
```

### Comparing `irene_pro-0.0.23/irene_pro/gui.py` & `irene_pro-0.0.26/irene_pro/widgets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 
 from tkinter import *
 from tkinter import ttk, filedialog
 import re, random
 from win32api import GetSystemMetrics as ruler
 from math import ceil
 import cv2
+
 from tkcalendar import Calendar
 import ttkthemes
-from others import *
+import numpy as np
 
 s_width = ruler(0)
 s_height = ruler(1)
 
 
 def w(width:float):
     ratio = width / 1366
@@ -397,14 +398,16 @@
             if found_num:
                 text = master['bg'][:master['bg'].index(found_num[0])]
                 num = int(master['bg'][master['bg'].index(found_num[0]):]) - 3
                 self.config(bg = text+str(num))
         except TypeError:
             pass
 
+
+
 class spinbox(ttk.Spinbox):
     def __init__(self, master, **kwargs):
         super().__init__(master =master, **kwargs)
 
 class calendar(Calendar):
     def __init__(self, master, global_date_holder:Variable, date_holder_widget = None, create_toplevel = False, **kw):
         super().__init__(master = master, **kw)
@@ -416,14 +419,16 @@
             self.datetime_fr = lframe(self.master)
             self.datetime_fr.pack(side=RIGHT, padx = w(2))
         else:
             # CREATE TOPLEVEL WINDOW TO HOLD THE CALENDAR AND THE TIME SELECTOR
             self.datetime_fr = Toplevel()
             self.datetime_fr.title("Select time and date")
             self.datetime_fr.geometry(f'{w(250)}x{h(480)}')
+            # self.datetime_fr.resizable(False, False)
+            self.datetime_fr.iconbitmap("images/clock.ico")
             self.datetime_fr.resizable(False, False)
         
         # MAKE CALENDAR
         self.make_cal()
 
     def make_cal(self):
         self.datetime_fr1 = lframe(self.datetime_fr)
@@ -465,15 +470,15 @@
                 h = "0" + h
             if len(m) != 2:
                 m = "0" + m
             if len(s) != 2:
                 s = "0" + s
             final_datetime = data[2] + "-" + data[0] + "-" + data[1] + " " + f"{h}:{m}:{s}"
             # COPY THE SELECTED DATE AND TIME
-            clipboard(data = final_datetime, action = "copy")
+            # clipboard(data = final_datetime, action = "copy")
             # GLOBALIZE SELECTED DATE
             global_date_holder = final_datetime
             
             if self.choosen_date:
                 try:
                     self.choosen_date.delete(0, END)
                     self.choosen_date.insert(END, final_datetime)
@@ -506,98 +511,87 @@
         dir = filedialog.askdirectory()
         if dir_holder:
             dir_holder.delete(0, END)
             dir_holder.insert(END, dir)
         else:
             return dir
 
-# PROGRESSBAR
-class Progress(ttk.Progressbar):
-    def __init__(self, master, max = 100, **kwargs):
-        """max: is the max length to which the progressbar will automatically be destroyed when reached"""
-        super().__init__(master=master)
-        self.master = master
-        self.max = max
-        
-    def step(self, value):
-        import time
-        self['value'] = value
-        self.master.update_idletasks()
-        if value == self.max:
-            self.master.destroy()
-        time.sleep(1)
-
-# ======= SCALE===========================================================
-class scaler(ttk.Scale):
-    def __init__(self, master,start, end, selected_displayer:Label, return_float = True, **kwargs):
-        """selected_displayer: the label to display the selected value from scale
-        return_float: by default, it returns float value, you can return integers but setting to False"""
-        super().__init__(master=master, from_ = start, to=end, **kwargs)
-        
-        self.displayer = selected_displayer
-        self.return_float_value = return_float
-        self.selected_value = None
-        self.config(command=self.display)
-
-    def display(self, value):
-        if not self.return_float_value:
-            value = int(float(value))
-        self.displayer.config(text=value)
-        self.selected_value = value
-    
-    def get_value(self):
-        """get the selected value from the scale so that you can use it in other side"""
-        return self.selected_value
-
-
-def separate(numbers):
-    floating = []
-    new_str = ""
-    float_pos = 0
-    decision = ""
-    sign_negative = ""
-    str_num = str(numbers)
-    listed = [i for i in str_num]
-    original = listed
-
-    try:
-        if "." in str_num:
-            float_pos += original.index(".")
-            decision += "point"
-            floating = listed[float_pos:]
-        if "-" in str_num:
-            listed.remove("-")
-            sign_negative += "negative"
 
-    except Exception:
-        pass
+class Table_gui:
+    def __init__(self, parent):
+        self.rows = 1
+        self.cols = 1
+        self.data = []
+        self.entries = []
+        self.cols_created = []
+
+        # BASE FRAME
+        self.base_frame = frame(parent)
+        self.base_frame.pack(fill = X, expand = True, padx = w(1), pady = h(1), side = LEFT)
+
+        self.btn_frame = frame(self.base_frame)
+        self.btn_frame.pack(side = BOTTOM, fill = X, expand = True, padx = w(1), pady = h(1))
 
-    if decision == "point":
-        listed = listed[:float_pos]
+        self.row = btn(self.btn_frame, text = "add row", command=self.make_row)
+        self.row.pack(side = LEFT, padx = w(1), pady = h(1), fill = X, expand = True)
 
-    if len(listed) > 3 and len(listed) < 7:
-        try:
-            position = len(listed) - 3
-            listed.insert(position, " ")
-        except Exception:
-            pass
+        self.col = btn(self.btn_frame, text = "add column", command= lambda: self.make_column(self.base_frame))
+        self.col.pack(side = LEFT, padx = w(1), pady = h(1), fill = X, expand = True)
+
+        # INITIAL COLUMN AT START
+        self.make_column(self.base_frame)
+    
+    def entry(self, frame:Frame):
+        e = entry(frame)
+        e.bind("<KeyRelease>", lambda e: replace_empty_in_data())
+        e.pack(side = TOP, padx = w(1), pady = h(1), fill = X, expand = True)
+        # TRACK THE ANCHORED ENTRY IN THE LIST OF ENTRIES AND BE ABLE TO REPLACE ITS VALUE IN THE DATA
+        def replace_empty_in_data():
+            found = False
+            for index,row in enumerate(self.entries):
+                for data_index, entry in enumerate(row):
+                    if e == entry:
+                        self.data[index][data_index] = e.get()
+                        found = True
+                # IF THE ENTRY POSITION WAS FOUND, STOP ITERATION FROM CONTINUING BECAUSE THERE IS NO DUPLICATES IN ENTRIES CREATED
+                if found:
+                    break
+            # DISPLAY THE UPDATE DATAFRAME
+            self.make_dynamic_df()
+
+        return e
+    
+    def frame(self, parent):
+        f = frame(parent)
+        f.pack(side = LEFT, padx = w(1), pady = h(1), fill = X, expand = True)
+        return f
+    
+    def make_row(self):
+        """if the row is created the entries are spreaded across the whole columns, so i need to know what the are the available column
+        so that I can spread an entry across the those columns. defautly, the column 1 should be created as I make the instance of the class"""
+        for index,row in enumerate(self.entries):
+            ent = self.entry(self.cols_created[index])
+            #APPEND THIS ENTRY TO THE ENTRIES AVAILABLE FOR ALL THE COLUMBS
+            row.append(ent)
+            # APPEND THE POSITION HOLDER OF THIS COLUMN IN THE DATA
+            self.data[index].append('')
+        self.rows += 1
+
+    def make_column(self, parent):
+        for i in range(self.cols):
+            fr = self.frame(parent)
+            self.cols_created.append(fr)
+            # HOLD VALUES
+            self.data.append([])
+            # HOLD ENTRIES
+            self.entries.append([])
+            for j in range(self.rows):
+                ent = self.entry(fr)
+                self.entries[-1].append(ent)
+                self.data[-1].append('')
+    
+    def final_data(self):
+        # BY NOW, THE DATAFRAME WILL BE BEING DISLPLAY IN THE TERMINAL
+        nd = np.array(self.data)
+        transposed_data = nd.T
+        return transposed_data
 
-    elif len(listed) == 7:
-        listed.insert(1, " ")
-        listed.insert(5, " ")
-
-    elif len(listed) == 8:
-        listed.insert(2, " ")
-        listed.insert(6, " ")
-
-    elif len(listed) == 9:
-        listed.insert(3, " ")
-        listed.insert(7, " ")
-
-    if sign_negative == "negative":
-        new_str += "-"
-    for j in listed:
-        new_str += j
-    if len(floating) > 0:
-        for k in floating:
-            new_str += k
-    return new_str
```

