# Comparing `tmp/ebmdatalab-0.0.8.tar.gz` & `tmp/ebmdatalab-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebmdatalab-0.0.8.tar", last modified: Tue Mar  5 14:50:24 2019, max compression
+gzip compressed data, was "ebmdatalab-0.0.9.tar", last modified: Wed Mar 20 11:37:37 2019, max compression
```

## Comparing `ebmdatalab-0.0.8.tar` & `ebmdatalab-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       89 2019-02-13 07:49:30.908874 ebmdatalab-0.0.8/.gitignore
--rw-r--r--   0        0        0     1055 2019-02-01 08:54:06.667773 ebmdatalab-0.0.8/LICENSE
--rw-r--r--   0        0        0      981 2019-03-05 08:31:11.614717 ebmdatalab-0.0.8/README.md
--rw-r--r--   0        0        0       75 2019-03-05 14:48:40.290509 ebmdatalab-0.0.8/ebmdatalab/__init__.py
--rw-r--r--   0        0        0     1722 2019-03-05 14:47:28.286351 ebmdatalab-0.0.8/ebmdatalab/bq.py
--rw-r--r--   0        0        0     4175 2019-03-05 14:22:42.515947 ebmdatalab-0.0.8/ebmdatalab/charts.py
--rw-r--r--   0        0        0    13485 2019-02-01 12:10:13.656335 ebmdatalab-0.0.8/ebmdatalab/data/ccg_for_map.csv
--rw-r--r--   0        0        0  1779062 2019-03-04 18:35:57.420315 ebmdatalab-0.0.8/ebmdatalab/data/ccgs.json
--rw-r--r--   0        0        0   568311 2019-03-05 13:18:15.556191 ebmdatalab-0.0.8/ebmdatalab/data/ccgs_cartogram.json
--rw-r--r--   0        0        0     2515 2019-03-05 13:22:59.962055 ebmdatalab-0.0.8/ebmdatalab/maps.py
--rw-r--r--   0        0        0      853 2019-02-01 16:47:34.038068 ebmdatalab-0.0.8/ebmdatalab/stats.py
--rw-r--r--   0        0        0     2526 2019-03-05 14:43:09.746060 ebmdatalab-0.0.8/ebmdatalab/test_bq.py
--rw-r--r--   0        0        0      850 2019-02-01 18:55:21.151984 ebmdatalab-0.0.8/ebmdatalab/test_charts.py
--rw-r--r--   0        0        0      486 2019-02-01 16:47:34.042068 ebmdatalab-0.0.8/ebmdatalab/test_maps.py
--rw-r--r--   0        0        0      994 2019-02-01 16:47:34.042068 ebmdatalab-0.0.8/ebmdatalab/test_stats.py
--rw-r--r--   0        0        0  1180320 2019-03-04 18:35:57.272314 ebmdatalab-0.0.8/examples/ccg_list_size.json
--rw-r--r--   0        0        0   295042 2019-03-05 13:23:04.166083 ebmdatalab-0.0.8/examples/charts.ipynb
--rw-r--r--   0        0        0     1908 2019-03-05 13:23:04.178083 ebmdatalab-0.0.8/examples/charts.py
--rw-r--r--   0        0        0     3272 2019-03-04 18:39:38.626100 ebmdatalab-0.0.8/examples/stats.ipynb
--rw-r--r--   0        0        0      683 2019-03-04 18:39:38.634101 ebmdatalab-0.0.8/examples/stats.py
--rw-r--r--   0        0        0      490 2019-03-04 18:41:05.174800 ebmdatalab-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 ebmdatalab-0.0.8/setup.py
--rw-r--r--   0        0        0      219 1970-01-01 00:00:00.000000 ebmdatalab-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       89 2019-02-13 07:49:30.908874 ebmdatalab-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1055 2019-02-01 08:54:06.667773 ebmdatalab-0.0.9/LICENSE
+-rw-r--r--   0        0        0      981 2019-03-05 08:31:11.614717 ebmdatalab-0.0.9/README.md
+-rw-r--r--   0        0        0       75 2019-03-20 11:37:25.756258 ebmdatalab-0.0.9/ebmdatalab/__init__.py
+-rw-r--r--   0        0        0     1722 2019-03-05 14:47:28.286351 ebmdatalab-0.0.9/ebmdatalab/bq.py
+-rw-r--r--   0        0        0     4171 2019-03-20 11:36:22.647684 ebmdatalab-0.0.9/ebmdatalab/charts.py
+-rw-r--r--   0        0        0    13485 2019-02-01 12:10:13.656335 ebmdatalab-0.0.9/ebmdatalab/data/ccg_for_map.csv
+-rw-r--r--   0        0        0  1779062 2019-03-04 18:35:57.420315 ebmdatalab-0.0.9/ebmdatalab/data/ccgs.json
+-rw-r--r--   0        0        0   568311 2019-03-05 13:18:15.556191 ebmdatalab-0.0.9/ebmdatalab/data/ccgs_cartogram.json
+-rw-r--r--   0        0        0     2515 2019-03-05 13:22:59.962055 ebmdatalab-0.0.9/ebmdatalab/maps.py
+-rw-r--r--   0        0        0      853 2019-02-01 16:47:34.038068 ebmdatalab-0.0.9/ebmdatalab/stats.py
+-rw-r--r--   0        0        0     2526 2019-03-05 14:43:09.746060 ebmdatalab-0.0.9/ebmdatalab/test_bq.py
+-rw-r--r--   0        0        0      850 2019-02-01 18:55:21.151984 ebmdatalab-0.0.9/ebmdatalab/test_charts.py
+-rw-r--r--   0        0        0      486 2019-02-01 16:47:34.042068 ebmdatalab-0.0.9/ebmdatalab/test_maps.py
+-rw-r--r--   0        0        0      994 2019-02-01 16:47:34.042068 ebmdatalab-0.0.9/ebmdatalab/test_stats.py
+-rw-r--r--   0        0        0  1180320 2019-03-04 18:35:57.272314 ebmdatalab-0.0.9/examples/ccg_list_size.json
+-rw-r--r--   0        0        0   295042 2019-03-05 13:23:04.166083 ebmdatalab-0.0.9/examples/charts.ipynb
+-rw-r--r--   0        0        0     1908 2019-03-05 13:23:04.178083 ebmdatalab-0.0.9/examples/charts.py
+-rw-r--r--   0        0        0     3272 2019-03-04 18:39:38.626100 ebmdatalab-0.0.9/examples/stats.ipynb
+-rw-r--r--   0        0        0      683 2019-03-04 18:39:38.634101 ebmdatalab-0.0.9/examples/stats.py
+-rw-r--r--   0        0        0      490 2019-03-04 18:41:05.174800 ebmdatalab-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 ebmdatalab-0.0.9/setup.py
+-rw-r--r--   0        0        0      219 1970-01-01 00:00:00.000000 ebmdatalab-0.0.9/PKG-INFO
```

### Comparing `ebmdatalab-0.0.8/LICENSE` & `ebmdatalab-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ebmdatalab-0.0.8/README.md` & `ebmdatalab-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ebmdatalab-0.0.8/ebmdatalab/bq.py` & `ebmdatalab-0.0.9/ebmdatalab/bq.py`

 * *Files identical despite different names*

### Comparing `ebmdatalab-0.0.8/ebmdatalab/charts.py` & `ebmdatalab-0.0.9/ebmdatalab/charts.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             linewidth=style['linewidth'],
             color=style['color'],
             label=label)
     ax.set_ylabel(ylabel, size=15, alpha=0.6)
     if title:
         ax.set_title(title, size=18)
     # set ymax across all subplots as largest value across dataset
-    ax.set_ylim([0, 100*df[column].max()*1.05])
+    ax.set_ylim([0, df[column].max()*1.05])
     ax.tick_params(labelsize=12)
     ax.set_xlim([df[period_column].min(), df[period_column].max()]) # set x axis range as full date range
 
     plt.setp(ax.xaxis.get_majorticklabels(), rotation=90)
     ax.xaxis.set_major_formatter(matplotlib.dates.DateFormatter('%B %Y'))
     if show_legend:
         ax.legend(
```

### Comparing `ebmdatalab-0.0.8/ebmdatalab/data/ccg_for_map.csv` & `ebmdatalab-0.0.9/ebmdatalab/data/ccg_for_map.csv`

 * *Files identical despite different names*

### Comparing `ebmdatalab-0.0.8/ebmdatalab/data/ccgs.json` & `ebmdatalab-0.0.9/ebmdatalab/data/ccgs.json`

 * *Files identical despite different names*

### Comparing `ebmdatalab-0.0.8/ebmdatalab/data/ccgs_cartogram.json` & `ebmdatalab-0.0.9/ebmdatalab/data/ccgs_cartogram.json`

 * *Files identical despite different names*

### Comparing `ebmdatalab-0.0.8/ebmdatalab/maps.py` & `ebmdatalab-0.0.9/ebmdatalab/maps.py`

 * *Files identical despite different names*

### Comparing `ebmdatalab-0.0.8/ebmdatalab/stats.py` & `ebmdatalab-0.0.9/ebmdatalab/stats.py`

 * *Files identical despite different names*

### Comparing `ebmdatalab-0.0.8/ebmdatalab/test_bq.py` & `ebmdatalab-0.0.9/ebmdatalab/test_bq.py`

 * *Files identical despite different names*

### Comparing `ebmdatalab-0.0.8/ebmdatalab/test_charts.py` & `ebmdatalab-0.0.9/ebmdatalab/test_charts.py`

 * *Files identical despite different names*

### Comparing `ebmdatalab-0.0.8/ebmdatalab/test_stats.py` & `ebmdatalab-0.0.9/ebmdatalab/test_stats.py`

 * *Files identical despite different names*

### Comparing `ebmdatalab-0.0.8/examples/ccg_list_size.json` & `ebmdatalab-0.0.9/examples/ccg_list_size.json`

 * *Files identical despite different names*

### Comparing `ebmdatalab-0.0.8/examples/charts.ipynb` & `ebmdatalab-0.0.9/examples/charts.ipynb`

 * *Files identical despite different names*

### Comparing `ebmdatalab-0.0.8/examples/charts.py` & `ebmdatalab-0.0.9/examples/charts.py`

 * *Files identical despite different names*

### Comparing `ebmdatalab-0.0.8/examples/stats.ipynb` & `ebmdatalab-0.0.9/examples/stats.ipynb`

 * *Files identical despite different names*

### Comparing `ebmdatalab-0.0.8/examples/stats.py` & `ebmdatalab-0.0.9/examples/stats.py`

 * *Files identical despite different names*

### Comparing `ebmdatalab-0.0.8/setup.py` & `ebmdatalab-0.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 install_requires = \
 ['statsmodels', 'pandas', 'pandas-gbq', 'geopandas', 'descartes']
 
 extras_require = \
 {'test': ['pytest >=2.7.3']}
 
 setup(name='ebmdatalab',
-      version='0.0.8',
+      version='0.0.9',
       description='Package for ebmdatalab jupyter notebook stuff',
       author='EBM DataLab',
       author_email='tech@ebmdatalab.net',
       url='https://github.com/ebmdatalab/datalab-pandas',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

