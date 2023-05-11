# Comparing `tmp/hyd-0.1.3.tar.gz` & `tmp/hyd-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyd-0.1.3.tar", max compression
+gzip compressed data, was "hyd-0.1.4.tar", max compression
```

## Comparing `hyd-0.1.3.tar` & `hyd-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1063 2022-12-07 14:08:19.737464 hyd-0.1.3/LICENSE
--rw-r--r--   0        0        0      103 2022-12-07 14:08:19.737576 hyd-0.1.3/README.md
--rw-r--r--   0        0        0     3826 2023-03-07 12:13:29.545689 hyd-0.1.3/hyd/HaukursYouTubeDownloader.py
--rw-r--r--   0        0        0      385 2023-03-07 12:24:17.738645 hyd-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      584 1970-01-01 00:00:00.000000 hyd-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2022-12-07 14:08:19.737464 hyd-0.1.4/LICENSE
+-rw-r--r--   0        0        0      103 2022-12-07 14:08:19.737576 hyd-0.1.4/README.md
+-rw-r--r--   0        0        0     3866 2023-05-11 08:37:42.319477 hyd-0.1.4/hyd/HaukursYouTubeDownloader.py
+-rw-r--r--   0        0        0      385 2023-05-11 08:38:00.313976 hyd-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      584 1970-01-01 00:00:00.000000 hyd-0.1.4/PKG-INFO
```

### Comparing `hyd-0.1.3/LICENSE` & `hyd-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hyd-0.1.3/hyd/HaukursYouTubeDownloader.py` & `hyd-0.1.4/hyd/HaukursYouTubeDownloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,15 +93,15 @@
             popup.mainloop()
         except:
             error = Tk()
             error.title("Download Failed :/")
             error.geometry("350x125")
             error.resizable(False, False)
             error.configure(bg="#222222")
-            errorLabel = Label(error, text="Download Failed :/ \n Please check your internet connection.",  fg="#EDEDED", bg="#222222")
+            errorLabel = Label(error, text="Download Failed :/ \n Please check your internet connection \n Maybe try updating your pip packages.",  fg="#EDEDED", bg="#222222")
             errorLabel.place(relx=0.5, rely=0.25, anchor=CENTER)
             error.mainloop()
             
     window.mainloop()
 if __name__ == '__main__':
     main()
```

### Comparing `hyd-0.1.3/PKG-INFO` & `hyd-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyd
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 License: MIT
 Author: haukurlogi
 Author-email: haukurlogi2008@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

