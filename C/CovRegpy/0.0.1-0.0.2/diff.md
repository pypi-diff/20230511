# Comparing `tmp/CovRegpy-0.0.1.tar.gz` & `tmp/CovRegpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/CovRegpy-0.0.1.tar", last modified: Mon Jan 16 22:58:05 2023, max compression
+gzip compressed data, was "dist/CovRegpy-0.0.2.tar", last modified: Thu May 11 12:40:21 2023, max compression
```

## Comparing `CovRegpy-0.0.1.tar` & `CovRegpy-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 cole      (1000) cole      (1000)        0 2023-01-16 22:58:05.000000 CovRegpy-0.0.1/
-drwxrwxr-x   0 cole      (1000) cole      (1000)        0 2023-01-16 22:58:05.000000 CovRegpy-0.0.1/CovRegpy/
--rw-rw-r--   0 cole      (1000) cole      (1000)    11301 2023-01-15 16:34:29.000000 CovRegpy-0.0.1/CovRegpy/CovRegpy_DCC.py
--rw-rw-r--   0 cole      (1000) cole      (1000)    14929 2023-01-06 00:11:55.000000 CovRegpy-0.0.1/CovRegpy/CovRegpy_IFF.py
--rw-rw-r--   0 cole      (1000) cole      (1000)     1842 2023-01-06 13:04:38.000000 CovRegpy-0.0.1/CovRegpy/CovRegpy_PCA.py
--rw-rw-r--   0 cole      (1000) cole      (1000)    39398 2023-01-14 21:00:35.000000 CovRegpy-0.0.1/CovRegpy/CovRegpy_RCR.py
--rw-rw-r--   0 cole      (1000) cole      (1000)    12503 2023-01-06 17:20:36.000000 CovRegpy-0.0.1/CovRegpy/CovRegpy_RPP.py
--rw-rw-r--   0 cole      (1000) cole      (1000)    14864 2023-01-06 21:46:07.000000 CovRegpy-0.0.1/CovRegpy/CovRegpy_SSA.py
--rw-rw-r--   0 cole      (1000) cole      (1000)    22139 2023-01-14 18:31:35.000000 CovRegpy-0.0.1/CovRegpy/CovRegpy_SSD.py
--rw-rw-r--   0 cole      (1000) cole      (1000)    18388 2023-01-12 19:20:33.000000 CovRegpy-0.0.1/CovRegpy/CovRegpy_X11.py
--rw-rw-r--   0 cole      (1000) cole      (1000)     6215 2023-01-05 23:33:20.000000 CovRegpy-0.0.1/CovRegpy/CovRegpy_forecasting.py
--rw-rw-r--   0 cole      (1000) cole      (1000)    11270 2023-01-06 13:00:23.000000 CovRegpy-0.0.1/CovRegpy/CovRegpy_measures.py
--rw-rw-r--   0 cole      (1000) cole      (1000)    11245 2023-01-06 18:07:39.000000 CovRegpy-0.0.1/CovRegpy/CovRegpy_sharpe.py
--rw-rw-r--   0 cole      (1000) cole      (1000)    21073 2023-01-14 17:42:02.000000 CovRegpy-0.0.1/CovRegpy/CovRegpy_utilities.py
--rw-rw-r--   0 cole      (1000) cole      (1000)      164 2023-01-16 22:31:48.000000 CovRegpy-0.0.1/CovRegpy/__init__.py
-drwxrwxr-x   0 cole      (1000) cole      (1000)        0 2023-01-16 22:58:05.000000 CovRegpy-0.0.1/CovRegpy.egg-info/
--rw-rw-r--   0 cole      (1000) cole      (1000)     1322 2023-01-16 22:58:05.000000 CovRegpy-0.0.1/CovRegpy.egg-info/PKG-INFO
--rw-rw-r--   0 cole      (1000) cole      (1000)      510 2023-01-16 22:58:05.000000 CovRegpy-0.0.1/CovRegpy.egg-info/SOURCES.txt
--rw-rw-r--   0 cole      (1000) cole      (1000)        1 2023-01-16 22:58:05.000000 CovRegpy-0.0.1/CovRegpy.egg-info/dependency_links.txt
--rw-rw-r--   0 cole      (1000) cole      (1000)       96 2023-01-16 22:58:05.000000 CovRegpy-0.0.1/CovRegpy.egg-info/requires.txt
--rw-rw-r--   0 cole      (1000) cole      (1000)        9 2023-01-16 22:58:05.000000 CovRegpy-0.0.1/CovRegpy.egg-info/top_level.txt
--rw-rw-r--   0 cole      (1000) cole      (1000)     1322 2023-01-16 22:58:05.000000 CovRegpy-0.0.1/PKG-INFO
--rw-rw-r--   0 cole      (1000) cole      (1000)       38 2023-01-16 22:58:05.000000 CovRegpy-0.0.1/setup.cfg
--rw-rw-r--   0 cole      (1000) cole      (1000)     1639 2023-01-16 22:48:45.000000 CovRegpy-0.0.1/setup.py
+drwxrwxr-x   0 cole      (1000) cole      (1000)        0 2023-05-11 12:40:21.000000 CovRegpy-0.0.2/
+drwxrwxr-x   0 cole      (1000) cole      (1000)        0 2023-05-11 12:40:21.000000 CovRegpy-0.0.2/CovRegpy/
+-rw-rw-r--   0 cole      (1000) cole      (1000)    11301 2023-01-15 16:34:29.000000 CovRegpy-0.0.2/CovRegpy/CovRegpy_DCC.py
+-rw-rw-r--   0 cole      (1000) cole      (1000)    14941 2023-02-13 17:33:16.000000 CovRegpy-0.0.2/CovRegpy/CovRegpy_IFF.py
+-rw-rw-r--   0 cole      (1000) cole      (1000)     1842 2023-01-06 13:04:38.000000 CovRegpy-0.0.2/CovRegpy/CovRegpy_PCA.py
+-rw-rw-r--   0 cole      (1000) cole      (1000)    39406 2023-05-10 17:49:11.000000 CovRegpy-0.0.2/CovRegpy/CovRegpy_RCR.py
+-rw-rw-r--   0 cole      (1000) cole      (1000)    12503 2023-01-06 17:20:36.000000 CovRegpy-0.0.2/CovRegpy/CovRegpy_RPP.py
+-rw-rw-r--   0 cole      (1000) cole      (1000)    14864 2023-01-06 21:46:07.000000 CovRegpy-0.0.2/CovRegpy/CovRegpy_SSA.py
+-rw-rw-r--   0 cole      (1000) cole      (1000)    22139 2023-01-14 18:31:35.000000 CovRegpy-0.0.2/CovRegpy/CovRegpy_SSD.py
+-rw-rw-r--   0 cole      (1000) cole      (1000)    18388 2023-01-12 19:20:33.000000 CovRegpy-0.0.2/CovRegpy/CovRegpy_X11.py
+-rw-rw-r--   0 cole      (1000) cole      (1000)     6215 2023-01-05 23:33:20.000000 CovRegpy-0.0.2/CovRegpy/CovRegpy_forecasting.py
+-rw-rw-r--   0 cole      (1000) cole      (1000)    11298 2023-03-07 21:20:19.000000 CovRegpy-0.0.2/CovRegpy/CovRegpy_measures.py
+-rw-rw-r--   0 cole      (1000) cole      (1000)    11245 2023-01-06 18:07:39.000000 CovRegpy-0.0.2/CovRegpy/CovRegpy_sharpe.py
+-rw-rw-r--   0 cole      (1000) cole      (1000)    21073 2023-01-14 17:42:02.000000 CovRegpy-0.0.2/CovRegpy/CovRegpy_utilities.py
+-rw-rw-r--   0 cole      (1000) cole      (1000)      164 2023-01-16 22:31:48.000000 CovRegpy-0.0.2/CovRegpy/__init__.py
+drwxrwxr-x   0 cole      (1000) cole      (1000)        0 2023-05-11 12:40:21.000000 CovRegpy-0.0.2/CovRegpy.egg-info/
+-rw-rw-r--   0 cole      (1000) cole      (1000)     1287 2023-05-11 12:40:21.000000 CovRegpy-0.0.2/CovRegpy.egg-info/PKG-INFO
+-rw-rw-r--   0 cole      (1000) cole      (1000)      518 2023-05-11 12:40:21.000000 CovRegpy-0.0.2/CovRegpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 cole      (1000) cole      (1000)        1 2023-05-11 12:40:21.000000 CovRegpy-0.0.2/CovRegpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 cole      (1000) cole      (1000)       96 2023-05-11 12:40:21.000000 CovRegpy-0.0.2/CovRegpy.egg-info/requires.txt
+-rw-rw-r--   0 cole      (1000) cole      (1000)        9 2023-05-11 12:40:21.000000 CovRegpy-0.0.2/CovRegpy.egg-info/top_level.txt
+-rw-rw-r--   0 cole      (1000) cole      (1000)      629 2023-05-11 12:10:51.000000 CovRegpy-0.0.2/LICENSE
+-rw-rw-r--   0 cole      (1000) cole      (1000)     1287 2023-05-11 12:40:21.000000 CovRegpy-0.0.2/PKG-INFO
+-rw-rw-r--   0 cole      (1000) cole      (1000)       38 2023-05-11 12:40:21.000000 CovRegpy-0.0.2/setup.cfg
+-rw-rw-r--   0 cole      (1000) cole      (1000)     1612 2023-05-11 12:38:45.000000 CovRegpy-0.0.2/setup.py
```

### Comparing `CovRegpy-0.0.1/CovRegpy/CovRegpy_DCC.py` & `CovRegpy-0.0.2/CovRegpy/CovRegpy_DCC.py`

 * *Files identical despite different names*

### Comparing `CovRegpy-0.0.1/CovRegpy/CovRegpy_IFF.py` & `CovRegpy-0.0.2/CovRegpy/CovRegpy_IFF.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,15 +224,15 @@
                                               np.vstack((time, emd[1][int(comp + 1), :])),
                                               np.vstack((time[:-1], emd[2][int(comp + 1), :])),
                                               max_frequency=7, which_imfs=[1], plot=False)
                 ax.pcolormesh(x_hs, y, np.abs(z), cmap='gist_rainbow', vmin=0, vmax=np.abs(z).max())
                 plt.xticks([0, np.pi, 2 * np.pi, 3 * np.pi, 4 * np.pi],
                            ['0', r'$\pi$', r'$2\pi$', r'$3\pi$', r'$4\pi$'])
                 # plt.legend(loc='upper left')
-                plt.savefig('aas_figures/iff_ht.png')
+                plt.savefig('../aas_figures/iff_ht.png')
                 plt.show()
                 ax = plt.subplot(111)
                 plt.gcf().subplots_adjust(bottom=0.15)
                 plt.title('Instantaneous Frequency Fit and Forecast', fontsize=16)
                 plt.scatter(time[-fit_window:], full_freq[-fit_window:],
                             label=textwrap.fill('Instantaneous frequency', 15))
                 plt.scatter(forecast_time, freq_forecast, label=textwrap.fill('Forecast instantaneous frequency', 15))
@@ -241,15 +241,15 @@
                          label=textwrap.fill('Linear regression', 12))
                 plt.xticks([3 * np.pi, 4 * np.pi, 5 * np.pi, 6 * np.pi],
                            [r'$3\pi$', r'$4\pi$', r'$5\pi$', r'$6\pi$'])
                 plt.ylim(-0.5, 8.5)
                 box_0 = ax.get_position()
                 ax.set_position([box_0.x0 - 0.04, box_0.y0, box_0.width * 0.90, box_0.height])
                 ax.legend(loc='center left', bbox_to_anchor=(1, 0.5), fontsize=8)
-                plt.savefig('aas_figures/iff_freq.png')
+                plt.savefig('../aas_figures/iff_freq.png')
                 plt.show()
                 ax = plt.subplot(111)
                 plt.gcf().subplots_adjust(bottom=0.15)
                 plt.title('Instantaneous Amplitude Fit and Forecast', fontsize=16)
                 plt.scatter(time[-fit_window:], full_amp[-fit_window:],
                             label=textwrap.fill('Instantaneous amplitude', 15))
                 plt.scatter(forecast_time, amp_forecast, label=textwrap.fill('Forecast instantaneous amplitude', 15))
@@ -257,27 +257,27 @@
                          np.append(amp_linear, amp_forecast), 'r-',
                          label=textwrap.fill('Linear regression', 12))
                 plt.xticks([3 * np.pi, 4 * np.pi, 5 * np.pi, 6 * np.pi],
                            [r'$3\pi$', r'$4\pi$', r'$5\pi$', r'$6\pi$'])
                 box_0 = ax.get_position()
                 ax.set_position([box_0.x0 - 0.04, box_0.y0, box_0.width * 0.92, box_0.height])
                 ax.legend(loc='center left', bbox_to_anchor=(1, 0.5), fontsize=8)
-                plt.savefig('aas_figures/iff_amp.png')
+                plt.savefig('../aas_figures/iff_amp.png')
                 plt.show()
                 ax = plt.subplot(111)
                 plt.gcf().subplots_adjust(bottom=0.15)
                 plt.title('Unfitted Instantaneous Frequency Forecast', fontsize=16)
                 plt.plot(time, emd[0][int(comp + 1), :], label=textwrap.fill('Time series', 12))
                 plt.plot(forecast_time, imf_forecast, 'k-', label=textwrap.fill('Unfitted time series forecast', 12))
                 plt.xticks([0, np.pi, 2 * np.pi, 3 * np.pi, 4 * np.pi, 5 * np.pi, 6 * np.pi],
                            ['0', r'$\pi$', r'$2\pi$', r'$3\pi$', r'$4\pi$', r'$5\pi$', r'$6\pi$'])
                 box_0 = ax.get_position()
                 ax.set_position([box_0.x0 - 0.04, box_0.y0, box_0.width * 0.94, box_0.height])
                 ax.legend(loc='center left', bbox_to_anchor=(1, 0.5), fontsize=8)
-                plt.savefig('aas_figures/iff_unfit.png')
+                plt.savefig('../aas_figures/iff_unfit.png')
                 plt.show()
 
         try:
             imf_forecast_mat = np.vstack((imf_forecast.reshape(1, -1), imf_forecast_mat.reshape(1, -1)))
         except:
             imf_forecast_mat = imf_forecast.copy()
```

### Comparing `CovRegpy-0.0.1/CovRegpy/CovRegpy_PCA.py` & `CovRegpy-0.0.2/CovRegpy/CovRegpy_PCA.py`

 * *Files identical despite different names*

### Comparing `CovRegpy-0.0.1/CovRegpy/CovRegpy_RCR.py` & `CovRegpy-0.0.2/CovRegpy/CovRegpy_RCR.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,15 +323,15 @@
     except:
         try:
             const = np.matmul(np.linalg.lstsq(Psi.astype(np.float64), B.T.astype(np.float64), rcond=None)[0], x)
         except:
             const = np.matmul(np.linalg.lstsq(Psi.astype(np.float64).dot(Psi.astype(np.float64).T),
                                               Psi.astype(np.float64).dot(B.T.astype(np.float64)), rcond=None)[0], x)
 
-    v = (1 + (x * np.matmul(B, const)).sum(0)) ** (-1)
+    v = np.abs((1 + (x * np.matmul(B, const)).sum(0)) ** (-1))
     m = v * sum(errors * const)
 
     return m.astype(np.float64), v.astype(np.float64)
 
 
 # define covariance regression function with mean given
```

### Comparing `CovRegpy-0.0.1/CovRegpy/CovRegpy_RPP.py` & `CovRegpy-0.0.2/CovRegpy/CovRegpy_RPP.py`

 * *Files identical despite different names*

### Comparing `CovRegpy-0.0.1/CovRegpy/CovRegpy_SSA.py` & `CovRegpy-0.0.2/CovRegpy/CovRegpy_SSA.py`

 * *Files identical despite different names*

### Comparing `CovRegpy-0.0.1/CovRegpy/CovRegpy_SSD.py` & `CovRegpy-0.0.2/CovRegpy/CovRegpy_SSD.py`

 * *Files identical despite different names*

### Comparing `CovRegpy-0.0.1/CovRegpy/CovRegpy_X11.py` & `CovRegpy-0.0.2/CovRegpy/CovRegpy_X11.py`

 * *Files identical despite different names*

### Comparing `CovRegpy-0.0.1/CovRegpy/CovRegpy_forecasting.py` & `CovRegpy-0.0.2/CovRegpy/CovRegpy_forecasting.py`

 * *Files identical despite different names*

### Comparing `CovRegpy-0.0.1/CovRegpy/CovRegpy_measures.py` & `CovRegpy-0.0.2/CovRegpy/CovRegpy_measures.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         Vector containing mean of portfolio daily returns using specified window.
 
     Notes
     -----
 
     """
     portfolio_returns = portfolio_return(weights, all_returns)
-    mean_returns = np.zeros(int(np.shape(weights)[1] - window))
+    mean_returns = np.zeros(int(np.shape(weights)[1] - window + 1))
     for col in range(len(mean_returns)):
         mean_returns[col] = np.mean(portfolio_returns[col:int(col + window)])
 
     return mean_returns
 
 
 def variance_return(weights, all_returns, window):
@@ -95,15 +95,15 @@
         Vector containing variance of portfolio daily returns using specified window.
 
     Notes
     -----
 
     """
     portfolio_returns = portfolio_return(weights, all_returns)
-    variance_returns = np.zeros(int(np.shape(weights)[1] - window))
+    variance_returns = np.zeros(int(np.shape(weights)[1] - window + 1))
     for col in range(len(variance_returns)):
         variance_returns[col] = np.var(portfolio_returns[col:int(col + window)])
 
     return variance_returns
 
 
 def value_at_risk_return(weights, all_returns, window):
@@ -127,15 +127,15 @@
         Vector containing value-at-risk of portfolio daily returns using specified window.
 
     Notes
     -----
 
     """
     portfolio_returns = portfolio_return(weights, all_returns)
-    value_at_risk_returns = np.zeros(int(np.shape(weights)[1] - window))
+    value_at_risk_returns = np.zeros(int(np.shape(weights)[1] - window + 1))
     for col in range(len(value_at_risk_returns)):
         value_at_risk_returns[col] = np.quantile(portfolio_returns[col:int(col + window)], 0.05)
 
     return value_at_risk_returns
 
 
 def max_draw_down_return(weights, all_returns, window):
@@ -159,15 +159,15 @@
         Vector containing maximum drawdown of portfolio daily returns using specified window.
 
     Notes
     -----
 
     """
     portfolio_returns = portfolio_return(weights, all_returns)
-    max_draw_down_returns = np.zeros(int(np.shape(weights)[1] - window))
+    max_draw_down_returns = np.zeros(int(np.shape(weights)[1] - window + 1))
     for col in range(len(max_draw_down_returns)):
         max_draw_down_returns[col] = (np.min(portfolio_returns[col:int(col + window)]) -
                                       np.max(portfolio_returns[col:int(col + window)])) / np.max(
             portfolio_returns[col:int(col + window)])
 
     return max_draw_down_returns
 
@@ -193,15 +193,15 @@
         Vector containing omega ratio of portfolio daily returns using specified window.
 
     Notes
     -----
 
     """
     portfolio_returns = portfolio_return(weights, all_returns)
-    omega_ratio_returns = np.zeros(int(np.shape(weights)[1] - window))
+    omega_ratio_returns = np.zeros(int(np.shape(weights)[1] - window + 1))
     for col in range(len(omega_ratio_returns)):
         omega_ratio_returns[col] = np.mean(portfolio_returns[col:int(col + window)] *
                                            (portfolio_returns[col:int(col + window)] > 0)) / \
                                    np.mean(-portfolio_returns[col:int(col + window)] *
                                            (portfolio_returns[col:int(col + window)] <= 0))
 
     return omega_ratio_returns
@@ -231,15 +231,15 @@
         Vector containing Sortino ratio of portfolio daily returns using specified window.
 
     Notes
     -----
 
     """
     portfolio_returns = portfolio_return(weights, all_returns)
-    sortino_ratio_returns = np.zeros(int(np.shape(weights)[1] - window))
+    sortino_ratio_returns = np.zeros(int(np.shape(weights)[1] - window + 1))
     for col in range(len(sortino_ratio_returns)):
         sortino_ratio_returns[col] = (np.mean(portfolio_returns[col:int(col + window)]) - risk_free) / \
                                      np.std(portfolio_returns[col:int(col + window)] *
                                             (portfolio_returns[col:int(col + window)] < 0))
 
     return sortino_ratio_returns
 
@@ -268,15 +268,15 @@
         Vector containing Sharpe ratio of portfolio daily returns using specified window.
 
     Notes
     -----
 
     """
     portfolio_returns = portfolio_return(weights, all_returns)
-    sharpe_ratio_returns = np.zeros(int(np.shape(weights)[1] - window))
+    sharpe_ratio_returns = np.zeros(int(np.shape(weights)[1] - window + 1))
     for col in range(len(sharpe_ratio_returns)):
         sharpe_ratio_returns[col] = (np.mean(portfolio_returns[col:int(col + window)]) - risk_free) / \
                                      np.std(portfolio_returns[col:int(col + window)])
 
     return sharpe_ratio_returns
```

### Comparing `CovRegpy-0.0.1/CovRegpy/CovRegpy_sharpe.py` & `CovRegpy-0.0.2/CovRegpy/CovRegpy_sharpe.py`

 * *Files identical despite different names*

### Comparing `CovRegpy-0.0.1/CovRegpy/CovRegpy_utilities.py` & `CovRegpy-0.0.2/CovRegpy/CovRegpy_utilities.py`

 * *Files identical despite different names*

### Comparing `CovRegpy-0.0.1/CovRegpy.egg-info/PKG-INFO` & `CovRegpy-0.0.2/CovRegpy.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: CovRegpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Regularised covariance regression software project based on Hoff and Niu (2012).
 Home-page: https://github.com/Cole-vJ/CovRegpy.git
+Download-URL: https://github.com/Cole-vJ/CovRegpy/archive/refs/tags/0.0.2.tar.gz
 Author: Cole van Jaarsveldt
 Author-email: colevj0303@gmail.com
-License: gpl-3.0
-Download-URL: https://github.com/Cole-vJ/CovRegpy/archive/refs/tags/0.0.1.tar.gz
-Description: Regularised Covariance regression software project based on Hoff and Niu (2012). This package was developed out of research performed by Cole van Jaarsveldt, Gareth W. Peters, Matthew Ames, and Mike Chantler. This package was built entirely using Python 3.7.0 - Python guarantees backwards compatibility which should ensure that this software package functions as expected on all future Python versions.
+License: custom
 Keywords: Portfolio Optimisation,Regularised Covariance Regression (RCR),Empirical Mode Decomposition (EMD),Singular Spectrum Analysis (SSA),Singular Spectrum Decomposition (SSD),X11,Implicit Factors,Risk Premia Parity,Risk Parity,Long\Short Equity
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: Free for non-commercial use
 Classifier: Programming Language :: Python :: 3.7
+License-File: LICENSE
+
+Regularised Covariance regression software project based on Hoff and Niu (2012). This package was developed out of research performed by Cole van Jaarsveldt, Gareth W. Peters, Matthew Ames, and Mike Chantler. This package was built entirely using Python 3.7.0 - Python guarantees backwards compatibility which should ensure that this software package functions as expected on all future Python versions.
```

### Comparing `CovRegpy-0.0.1/PKG-INFO` & `CovRegpy-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: CovRegpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Regularised covariance regression software project based on Hoff and Niu (2012).
 Home-page: https://github.com/Cole-vJ/CovRegpy.git
+Download-URL: https://github.com/Cole-vJ/CovRegpy/archive/refs/tags/0.0.2.tar.gz
 Author: Cole van Jaarsveldt
 Author-email: colevj0303@gmail.com
-License: gpl-3.0
-Download-URL: https://github.com/Cole-vJ/CovRegpy/archive/refs/tags/0.0.1.tar.gz
-Description: Regularised Covariance regression software project based on Hoff and Niu (2012). This package was developed out of research performed by Cole van Jaarsveldt, Gareth W. Peters, Matthew Ames, and Mike Chantler. This package was built entirely using Python 3.7.0 - Python guarantees backwards compatibility which should ensure that this software package functions as expected on all future Python versions.
+License: custom
 Keywords: Portfolio Optimisation,Regularised Covariance Regression (RCR),Empirical Mode Decomposition (EMD),Singular Spectrum Analysis (SSA),Singular Spectrum Decomposition (SSD),X11,Implicit Factors,Risk Premia Parity,Risk Parity,Long\Short Equity
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: Free for non-commercial use
 Classifier: Programming Language :: Python :: 3.7
+License-File: LICENSE
+
+Regularised Covariance regression software project based on Hoff and Niu (2012). This package was developed out of research performed by Cole van Jaarsveldt, Gareth W. Peters, Matthew Ames, and Mike Chantler. This package was built entirely using Python 3.7.0 - Python guarantees backwards compatibility which should ensure that this software package functions as expected on all future Python versions.
```

### Comparing `CovRegpy-0.0.1/setup.py` & `CovRegpy-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
 from setuptools import setup
 
 setup(
   name = 'CovRegpy',
   packages = ['CovRegpy'],
-  version = '0.0.1',
-  license='gpl-3.0',
+  version = '0.0.2',
+  license='custom',
   description = 'Regularised covariance regression software project based on Hoff and Niu (2012).',
   long_description = 'Regularised Covariance regression software project based on Hoff and Niu (2012). This package was developed out of research performed by Cole van Jaarsveldt, Gareth W. Peters, Matthew Ames, and Mike Chantler. This package was built entirely using Python 3.7.0 - Python guarantees backwards compatibility which should ensure that this software package functions as expected on all future Python versions.',
   author = 'Cole van Jaarsveldt',
   author_email = 'colevj0303@gmail.com',
   url = 'https://github.com/Cole-vJ/CovRegpy.git',
-  download_url = 'https://github.com/Cole-vJ/CovRegpy/archive/refs/tags/0.0.1.tar.gz',
+  download_url = 'https://github.com/Cole-vJ/CovRegpy/archive/refs/tags/0.0.2.tar.gz',
   keywords = ['Portfolio Optimisation', 'Regularised Covariance Regression (RCR)', 'Empirical Mode Decomposition (EMD)', 'Singular Spectrum Analysis (SSA)', 'Singular Spectrum Decomposition (SSD)', 'X11', 'Implicit Factors', 'Risk Premia Parity', 'Risk Parity', 'Long\Short Equity'],
   install_requires=[
           'numpy',
           'seaborn',
 	  'group-lasso',
 	  'AdvEMDpy',
 	  'pandas',
@@ -25,11 +25,11 @@
 	  'arch',
   	  'notebook',
       ],
   classifiers=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
-    'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
+    'License :: Free for non-commercial use',
     'Programming Language :: Python :: 3.7',
   ],
 )
```

