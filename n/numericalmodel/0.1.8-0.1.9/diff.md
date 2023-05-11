# Comparing `tmp/numericalmodel-0.1.8.tar.gz` & `tmp/numericalmodel-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/numericalmodel-0.1.8.tar", last modified: Fri Oct 13 12:56:57 2017, max compression
+gzip compressed data, was "dist/numericalmodel-0.1.9.tar", last modified: Fri Oct 13 16:07:20 2017, max compression
```

## Comparing `numericalmodel-0.1.8.tar` & `numericalmodel-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-13 12:56:57.000000 numericalmodel-0.1.8/
--rwxrwxrwx   0 root         (0) root         (0)     1203 2017-10-13 12:56:21.000000 numericalmodel-0.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-13 12:56:57.000000 numericalmodel-0.1.8/numericalmodel.egg-info/
--rw-r--r--   0 root         (0) root         (0)       40 2017-10-13 12:56:57.000000 numericalmodel-0.1.8/numericalmodel.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2017-10-13 12:56:57.000000 numericalmodel-0.1.8/numericalmodel.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2017-10-13 12:56:57.000000 numericalmodel-0.1.8/numericalmodel.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2498 2017-10-13 12:56:57.000000 numericalmodel-0.1.8/numericalmodel.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      495 2017-10-13 12:56:57.000000 numericalmodel-0.1.8/numericalmodel.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)     1557 2017-10-13 12:56:21.000000 numericalmodel-0.1.8/README.rst
--rw-r--r--   0 root         (0) root         (0)       59 2017-10-13 12:56:57.000000 numericalmodel-0.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2498 2017-10-13 12:56:57.000000 numericalmodel-0.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    35141 2017-10-13 12:56:21.000000 numericalmodel-0.1.8/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-13 12:56:57.000000 numericalmodel-0.1.8/numericalmodel/
--rw-rw-rw-   0 root         (0) root         (0)     8862 2017-10-13 12:56:21.000000 numericalmodel-0.1.8/numericalmodel/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    22645 2017-10-13 12:56:21.000000 numericalmodel-0.1.8/numericalmodel/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     9232 2017-10-13 12:56:21.000000 numericalmodel-0.1.8/numericalmodel/equations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-13 12:56:57.000000 numericalmodel-0.1.8/numericalmodel/gui/
--rw-rw-rw-   0 root         (0) root         (0)    49570 2017-10-13 12:56:21.000000 numericalmodel-0.1.8/numericalmodel/gui/gui.glade
--rw-rw-rw-   0 root         (0) root         (0)    34032 2017-10-13 12:56:21.000000 numericalmodel-0.1.8/numericalmodel/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    33653 2017-10-13 12:56:21.000000 numericalmodel-0.1.8/numericalmodel/numericalschemes.py
--rw-rw-rw-   0 root         (0) root         (0)    11623 2017-10-13 12:56:21.000000 numericalmodel-0.1.8/numericalmodel/numericalmodel.py
--rw-rw-rw-   0 root         (0) root         (0)     6177 2017-10-13 12:56:21.000000 numericalmodel-0.1.8/numericalmodel/genericmodel.py
--rw-rw-rw-   0 root         (0) root         (0)      326 2017-10-13 12:56:21.000000 numericalmodel-0.1.8/numericalmodel/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       61 2017-10-13 12:56:21.000000 numericalmodel-0.1.8/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-13 16:07:20.000000 numericalmodel-0.1.9/
+-rwxrwxrwx   0 root         (0) root         (0)     1203 2017-10-13 16:06:43.000000 numericalmodel-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-13 16:07:20.000000 numericalmodel-0.1.9/numericalmodel.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       40 2017-10-13 16:07:19.000000 numericalmodel-0.1.9/numericalmodel.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2017-10-13 16:07:19.000000 numericalmodel-0.1.9/numericalmodel.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2017-10-13 16:07:19.000000 numericalmodel-0.1.9/numericalmodel.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2498 2017-10-13 16:07:19.000000 numericalmodel-0.1.9/numericalmodel.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      495 2017-10-13 16:07:20.000000 numericalmodel-0.1.9/numericalmodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2017-10-13 16:06:43.000000 numericalmodel-0.1.9/README.rst
+-rw-r--r--   0 root         (0) root         (0)       59 2017-10-13 16:07:20.000000 numericalmodel-0.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2498 2017-10-13 16:07:20.000000 numericalmodel-0.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    35141 2017-10-13 16:06:43.000000 numericalmodel-0.1.9/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-13 16:07:20.000000 numericalmodel-0.1.9/numericalmodel/
+-rw-rw-rw-   0 root         (0) root         (0)     8862 2017-10-13 16:06:43.000000 numericalmodel-0.1.9/numericalmodel/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    22645 2017-10-13 16:06:43.000000 numericalmodel-0.1.9/numericalmodel/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     9232 2017-10-13 16:06:43.000000 numericalmodel-0.1.9/numericalmodel/equations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2017-10-13 16:07:20.000000 numericalmodel-0.1.9/numericalmodel/gui/
+-rw-rw-rw-   0 root         (0) root         (0)    54540 2017-10-13 16:06:43.000000 numericalmodel-0.1.9/numericalmodel/gui/gui.glade
+-rw-rw-rw-   0 root         (0) root         (0)    39414 2017-10-13 16:06:43.000000 numericalmodel-0.1.9/numericalmodel/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    33653 2017-10-13 16:06:43.000000 numericalmodel-0.1.9/numericalmodel/numericalschemes.py
+-rw-rw-rw-   0 root         (0) root         (0)    11623 2017-10-13 16:06:43.000000 numericalmodel-0.1.9/numericalmodel/numericalmodel.py
+-rw-rw-rw-   0 root         (0) root         (0)     6177 2017-10-13 16:06:43.000000 numericalmodel-0.1.9/numericalmodel/genericmodel.py
+-rw-rw-rw-   0 root         (0) root         (0)      326 2017-10-13 16:06:43.000000 numericalmodel-0.1.9/numericalmodel/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       61 2017-10-13 16:06:43.000000 numericalmodel-0.1.9/MANIFEST.in
```

### Comparing `numericalmodel-0.1.8/setup.py` & `numericalmodel-0.1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # System modules
 import os
 from setuptools import setup, find_packages
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 def read_file(filename):
     with open(filename) as f:
         return f.read()
 
 # run setup
 # take metadata from setup.cfg
```

### Comparing `numericalmodel-0.1.8/numericalmodel.egg-info/PKG-INFO` & `numericalmodel-0.1.9/numericalmodel.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: numericalmodel
-Version: 0.1.8
+Version: 0.1.9
 Summary: abstract classes to set up and run a numerical model
 Home-page: https://gitlab.com/nobodyinperson/python3-numericalmodel
 Author: Yann Büchau
 Author-email: yann.buechau@web.de
 License: GPLv3
 Description: python3-numericalmodel 
         ======================
```

### Comparing `numericalmodel-0.1.8/README.rst` & `numericalmodel-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `numericalmodel-0.1.8/PKG-INFO` & `numericalmodel-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: numericalmodel
-Version: 0.1.8
+Version: 0.1.9
 Summary: abstract classes to set up and run a numerical model
 Home-page: https://gitlab.com/nobodyinperson/python3-numericalmodel
 Author: Yann Büchau
 Author-email: yann.buechau@web.de
 License: GPLv3
 Description: python3-numericalmodel 
         ======================
```

### Comparing `numericalmodel-0.1.8/LICENSE` & `numericalmodel-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `numericalmodel-0.1.8/numericalmodel/utils.py` & `numericalmodel-0.1.9/numericalmodel/utils.py`

 * *Files identical despite different names*

### Comparing `numericalmodel-0.1.8/numericalmodel/interfaces.py` & `numericalmodel-0.1.9/numericalmodel/interfaces.py`

 * *Files identical despite different names*

### Comparing `numericalmodel-0.1.8/numericalmodel/equations.py` & `numericalmodel-0.1.9/numericalmodel/equations.py`

 * *Files identical despite different names*

### Comparing `numericalmodel-0.1.8/numericalmodel/gui/gui.glade` & `numericalmodel-0.1.9/numericalmodel/gui/gui.glade`

 * *Files 2% similar despite different names*

#### Comparing `numericalmodel-0.1.8/numericalmodel/gui/gui.glade` & `numericalmodel-0.1.9/numericalmodel/gui/gui.glade`

```diff
@@ -648,14 +648,73 @@
                                           </object>
                                           <packing>
                                             <property name="expand">False</property>
                                             <property name="fill">True</property>
                                             <property name="position">1</property>
                                           </packing>
                                         </child>
+                                        <child>
+                                          <object class="GtkCheckButton" id="settings_plot_scatterplot_checkbutton">
+                                            <property name="label" translatable="yes">use scatterplots</property>
+                                            <property name="use_action_appearance">False</property>
+                                            <property name="related_action">app.refresh</property>
+                                            <property name="visible">True</property>
+                                            <property name="can_focus">True</property>
+                                            <property name="receives_default">False</property>
+                                            <property name="tooltip_text" translatable="yes">use scatterplots for values with the same unit</property>
+                                            <property name="xalign">0</property>
+                                            <property name="draw_indicator">True</property>
+                                            <signal name="toggled" handler="ShowHideScatterOptions" swapped="no"/>
+                                          </object>
+                                          <packing>
+                                            <property name="expand">False</property>
+                                            <property name="fill">True</property>
+                                            <property name="position">2</property>
+                                          </packing>
+                                        </child>
+                                        <child>
+                                          <object class="GtkCheckButton" id="settings_plot_show_identity_checkbutton">
+                                            <property name="label" translatable="yes">show identity line</property>
+                                            <property name="use_action_appearance">False</property>
+                                            <property name="related_action">app.refresh</property>
+                                            <property name="visible">True</property>
+                                            <property name="sensitive">False</property>
+                                            <property name="can_focus">True</property>
+                                            <property name="receives_default">False</property>
+                                            <property name="no_show_all">True</property>
+                                            <property name="tooltip_text" translatable="yes">show an identity line</property>
+                                            <property name="halign">start</property>
+                                            <property name="xalign">0</property>
+                                            <property name="draw_indicator">True</property>
+                                          </object>
+                                          <packing>
+                                            <property name="expand">False</property>
+                                            <property name="fill">True</property>
+                                            <property name="position">3</property>
+                                          </packing>
+                                        </child>
+                                        <child>
+                                          <object class="GtkCheckButton" id="settings_plot_equal_axes_checkbutton">
+                                            <property name="label" translatable="yes">same aspect ratio for x/y-axis</property>
+                                            <property name="use_action_appearance">False</property>
+                                            <property name="related_action">app.refresh</property>
+                                            <property name="visible">True</property>
+                                            <property name="sensitive">False</property>
+                                            <property name="can_focus">True</property>
+                                            <property name="receives_default">False</property>
+                                            <property name="no_show_all">True</property>
+                                            <property name="xalign">0</property>
+                                            <property name="draw_indicator">True</property>
+                                          </object>
+                                          <packing>
+                                            <property name="expand">False</property>
+                                            <property name="fill">True</property>
+                                            <property name="position">4</property>
+                                          </packing>
+                                        </child>
                                       </object>
                                     </child>
                                     <child type="label">
                                       <object class="GtkLabel" id="settings_plot_expander_label">
                                         <property name="visible">True</property>
                                         <property name="can_focus">False</property>
                                         <property name="label">Settings</property>
```

### Comparing `numericalmodel-0.1.8/numericalmodel/gui/__init__.py` & `numericalmodel-0.1.9/numericalmodel/gui/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -371,24 +371,35 @@
                 )
 
         for sig in signals: # loop over all signals
             GLib.idle_add( # 'execute'
                 install_glib_handler, sig, # add a handler for this signal
                 priority = GLib.PRIORITY_HIGH  )
 
-    def plot_interfacevalues(self, interfacevalues, figure, times = None):
+    def plot_interfacevalues(self, interfacevalues, figure, times = None,
+        scatter = False, consistent_colors = False, equal_axes = False,
+        identity_line = False):
         """
         Plot an :any:`InterfaceValue` onto a given Figure
 
         Args:
             interfacevalues (list): the :any:`InterfaceValue` s to plot
             figure (matplotlib.figure.Figure): the
                 :any:`matplotlib.figure.Figure` to plot onto
             times (numpy.ndarray, optional): Times to plot. If left unspecified,
                 plot the times that are available.
+            scatter (bool, optional): Use scatterplots where possible? Defaults
+                to ``False``.
+            consistent_colors (bool, optional): Use consistent colors for all
+                plots, i.e. determine the color from the :any:`InterfaceValue`
+                's metadata? Defaults to ``False``.
+            identity_line (bool, optional): If ``scatter`` is ``True``, draw an
+                identity line? Defaults to ``False``.
+            equal_axes (bool, optional): If ``scatter`` is ``True``, use an
+                aspect ratio of ``1:1`` for the x/y-axis? Defaults to ``False``.
         """
         # delete all old axes
         for ax in figure.axes:
             figure.delaxes(ax)
         units = {}
         for interfacevalue in interfacevalues:
             try:
@@ -403,68 +414,138 @@
         i = 1
         axes = {}
         timeunit = "s"
         for unit,ivlist in sorted(units.items()):
             try:
                 axes[unit]
             except KeyError:
-                try:
-                    axes[unit] = figure.add_subplot(len(units),1,len(units)-i+1,
-                        sharex=xaxis_shared)
-                except NameError:
-                    axes[unit] = figure.add_subplot(len(units),1,len(units)-i+1)
-                    xaxis_shared = axes[unit]
-            ax = axes[unit]
-            for iv in ivlist:
-                if times is None:
-                    x = iv.times
-                    y = iv.values
+                if scatter:
+                    axes[unit] = figure.add_subplot(len(units),1,
+                            len(units)-i+1)
                 else:
-                    oneday = 24 * 60 * 60
-                    onehour = 60 * 60
-                    oneminute = 60
-                    if max(times) > oneday:
-                        x = times / oneday
-                        timeunit = "d"
-                    elif max(times) > onehour:
-                        x = times / onehour
-                        timeunit = "h"
-                    elif max(times) > oneminute:
-                        x = times / oneminute
-                        timeunit = "min"
+                    try:
+                        axes[unit] = figure.add_subplot(len(units),1,
+                            len(units)-i+1, sharex=xaxis_shared)
+                    except NameError:
+                        axes[unit] = figure.add_subplot(len(units),1,
+                            len(units)-i+1)
+                        xaxis_shared = axes[unit]
+            ax = axes[unit]
+            plot_kwargs_all = { "linewidth":2, "zorder":5 }
+            if scatter:
+                if len(ivlist) == 1:
+                    # 1-1 scatterplot
+                    plot_kwargs = plot_kwargs_all.copy()
+                    iv = ivlist[0]
+                    plot_kwargs.update(
+                        {"label":"{} ({}) vs. itself".format(iv.name,iv.id)})
+                    if consistent_colors:
+                        plot_kwargs.update(
+                            {"color":string2color(iv.name+iv.id)})
+                    if times is None:
+                        times = iv.times
+                    ax.scatter(iv(times),iv(times),**plot_kwargs)
+                    ax.set_xlabel("{} [{}]".format(iv.id,iv.unit))
+                    ax.set_ylabel("{} [{}]".format(iv.id,iv.unit))
+                elif len(ivlist) == 2:
+                    # ordinary scatterplot
+                    plot_kwargs = plot_kwargs_all.copy()
+                    iv1, iv2 = ivlist
+                    if times is None:
+                        times = np.union1d(iv1.times,iv2.times)
+                    plot_kwargs.update(
+                        {"label":"{} ({}) vs. {} ({})".format(
+                            iv1.name,iv1.id,iv2.name,iv2.id)})
+                    if consistent_colors:
+                        plot_kwargs.update(
+                            {"color":string2color(iv1.name+iv1.id)})
+                    ax.scatter(iv1(times),iv2(times),**plot_kwargs)
+                    ax.set_xlabel("{} [{}]".format(iv1.id,iv1.unit))
+                    ax.set_ylabel("{} [{}]".format(iv2.id,iv2.unit))
+                elif len(ivlist) > 2:
+                    if times is None:
+                        times = np.array([])
+                        for v in ivlist:
+                            times = np.union1d(times,v.times)
+                    for iv in ivlist:
+                        plot_kwargs = plot_kwargs_all.copy()
+                        if consistent_colors:
+                            plot_kwargs.update(
+                                {"color":string2color(iv.name+iv.id)})
+                        # stacked scatterplot
+                        try:
+                            main_iv
+                            plot_kwargs.update({"label":"{} ({}) vs. {} ({})"\
+                                .format(main_iv.name,main_iv.id,iv.name,iv.id)})
+                            ax.scatter(main_iv(times),iv(times),**plot_kwargs)
+                            ax.set_xlabel("{} [{}]".format(
+                                main_iv.id,main_iv.unit))
+                            ax.set_ylabel("[{}]".format(main_iv.unit))
+                        except NameError:
+                            main_iv = iv
+                if equal_axes:
+                    ax.set_aspect("equal","datalim")
+                if identity_line:
+                    xl,xu = ax.get_xlim()
+                    yl,yu = ax.get_ylim()
+                    plot_kwargs = plot_kwargs_all.copy()
+                    plot_kwargs.update({"zorder":10,"c":"k","linestyle":"--",
+                        "label":"identity"})
+                    low,high = min(xl,yl), max(xu,yu)
+                    ax.plot([low,high],[low,high],**plot_kwargs)
+            else:
+                for iv in ivlist:
+                    plot_kwargs = plot_kwargs_all.copy()
+                    if times is None:
+                        x = iv.times
+                        y = iv.values
                     else:
-                        x = times
-                    y = iv(times)
-
-                plot_kwargs = {
-                    "label":"{} ({})".format(iv.name,iv.id),
-                    "linewidth":2,
-                    "zorder":5
-                    }
-                if self["settings_plot_consistent_colors_checkbutton"]\
-                    .get_active():
-                    plot_kwargs.update({"color":string2color(iv.name+iv.id)})
-                if np.array(x).size > 1:
-                    plot_kwargs.update({ "drawstyle":interp2drawstyle.get(
-                            iv.interpolation,"steps-post"),})
-                    ax.plot( x,y, **plot_kwargs)
-                else:
-                    ax.scatter( x,y, **plot_kwargs)
-            ax.set_ylabel("[{}]".format(unit))
+                        oneday = 24 * 60 * 60
+                        onehour = 60 * 60
+                        oneminute = 60
+                        if max(times) > oneday:
+                            x = times / oneday
+                            timeunit = "d"
+                        elif max(times) > onehour:
+                            x = times / onehour
+                            timeunit = "h"
+                        elif max(times) > oneminute:
+                            x = times / oneminute
+                            timeunit = "min"
+                        else:
+                            x = times
+                        y = iv(times)
+
+                    plot_kwargs.update(
+                        {"label":"{} ({})".format(iv.name,iv.id)})
+                    if consistent_colors:
+                        plot_kwargs.update(
+                            {"color":string2color(iv.name+iv.id)})
+                    if np.array(x).size > 1:
+                        plot_kwargs.update({ "drawstyle":interp2drawstyle.get(
+                                iv.interpolation,"steps-post"),})
+                        ax.plot( x,y, **plot_kwargs)
+                    else:
+                        ax.scatter( x,y, **plot_kwargs)
+                ax.set_ylabel("[{}]".format(unit))
             ax.tick_params(direction="in")
             ax.grid(zorder=0)
             ax.legend(fontsize="small")
             i += 1
 
         for unit,ax in axes.items():
-            if ax == xaxis_shared:
-                ax.set_xlabel("time [{}]".format(timeunit))
-            else:
+            try:
+                if ax == xaxis_shared:
+                    ax.set_xlabel("time [{}]".format(timeunit))
+                else:
+                    ax.tick_params(bottom=True,left=True,top=True,
+                        right=True,labelbottom=False,)
+            except NameError:
                 ax.tick_params(bottom=True,left=True,top=True,
-                    right=True,labelbottom=False,)
+                    right=True,labelbottom=True,)
         figure.canvas.draw()
 
     def apply_data_from_settings(self,*args,**kwargs):
         """
         Read the data from the settings and feed it into the model
         """
         self.add_status("settings","Applying new data settings...")
@@ -533,14 +614,26 @@
         plot_interfacevalues_kwargs = {}
         if self["settings_plot_usevariabletime_checkbutton"].get_active():
             all_times = np.array([])
             for v in self.model.variables.elements:
                 all_times = np.union1d(all_times,v.times)
             plot_interfacevalues_kwargs["times"] = all_times
 
+        if self["settings_plot_consistent_colors_checkbutton"].get_active():
+            plot_interfacevalues_kwargs["consistent_colors"] = True
+  
+        if self["settings_plot_scatterplot_checkbutton"].get_active():
+            plot_interfacevalues_kwargs["scatter"] = True
+
+        if self["settings_plot_equal_axes_checkbutton"].get_active():
+            plot_interfacevalues_kwargs["equal_axes"] = True
+
+        if self["settings_plot_show_identity_checkbutton"].get_active():
+            plot_interfacevalues_kwargs["identity_line"] = True
+
         for tab,content in self.figures_content.items():
             current_tab = self["plot_notebook"].get_current_page()
             current_box = self["plot_notebook"].get_nth_page(current_tab)
             if self["plot_{}_box".format(tab)] == current_box:
                 self.add_status("plot","Plotting...",important=True)
                 interfacevalues = []
                 for modelpart,ivs in content.items():
@@ -602,19 +695,27 @@
                 label = self["plot_{}_notebook_label".format(attr)]
                 italictext = re.sub(
                     string=label.get_text(),
                     pattern=r"^(?:<b><i>)?([^<]+)(?:</i></b>)?$",
                     repl=r"\1")
                 label.set_markup(italictext)
             self.figures_content = None
+        def show_hide_scatter_options(widget, *args, **kwargs):
+            if self["settings_plot_scatterplot_checkbutton"].get_active():
+                sen = True
+            else:
+                sen = False
+            self["settings_plot_show_identity_checkbutton"].set_sensitive(sen)
+            self["settings_plot_equal_axes_checkbutton"].set_sensitive(sen)
         # connect signals
         self.handlers = {
             "CloseApplication": self.quit,
             "Integrate": self.integrate,
             "UpdatePlot": self.update_current_plot,
+            "ShowHideScatterOptions": show_hide_scatter_options,
             "ResetParams": reset_params,
             "ResetForcing": reset_forcing,
             "ResetVariables": reset_variables,
             "ResetObservations": reset_observations,
             "ResetPlots": reset_plots,
             "FeedModel": feedmodel,
             }
```

### Comparing `numericalmodel-0.1.8/numericalmodel/numericalschemes.py` & `numericalmodel-0.1.9/numericalmodel/numericalschemes.py`

 * *Files identical despite different names*

### Comparing `numericalmodel-0.1.8/numericalmodel/numericalmodel.py` & `numericalmodel-0.1.9/numericalmodel/numericalmodel.py`

 * *Files identical despite different names*

### Comparing `numericalmodel-0.1.8/numericalmodel/genericmodel.py` & `numericalmodel-0.1.9/numericalmodel/genericmodel.py`

 * *Files identical despite different names*

