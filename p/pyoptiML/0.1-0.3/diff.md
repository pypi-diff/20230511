# Comparing `tmp/pyoptiML-0.1.tar.gz` & `tmp/pyoptiML-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoptiML-0.1.tar", last modified: Mon Apr 17 10:03:44 2023, max compression
+gzip compressed data, was "pyoptiML-0.3.tar", last modified: Thu May 11 14:38:06 2023, max compression
```

## Comparing `pyoptiML-0.1.tar` & `pyoptiML-0.3.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 10:03:44.580558 pyoptiML-0.1/
--rw-rw-rw-   0        0        0     1094 2023-04-01 08:26:40.000000 pyoptiML-0.1/LICENSE
--rw-rw-rw-   0        0        0     3817 2023-04-17 10:03:44.581554 pyoptiML-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3120 2023-04-17 09:15:45.000000 pyoptiML-0.1/README.md
--rw-rw-rw-   0        0        0      697 2023-04-17 10:03:44.593671 pyoptiML-0.1/setup.cfg
--rw-rw-rw-   0        0        0      812 2023-04-17 09:44:11.000000 pyoptiML-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 10:03:44.268336 pyoptiML-0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 10:03:44.497273 pyoptiML-0.1/src/optiML/
--rw-rw-rw-   0        0        0        0 2023-04-01 08:33:14.000000 pyoptiML-0.1/src/optiML/__init__.py
--rw-rw-rw-   0        0        0     1786 2023-04-17 04:54:10.000000 pyoptiML-0.1/src/optiML/import_file.py
--rw-rw-rw-   0        0        0     8370 2023-04-06 09:26:41.000000 pyoptiML-0.1/src/optiML/preprocessing_data.py
--rw-rw-rw-   0        0        0      308 2023-04-06 09:26:50.000000 pyoptiML-0.1/src/optiML/pyoptiml.py
--rw-rw-rw-   0        0        0     1706 2023-04-06 09:27:07.000000 pyoptiML-0.1/src/optiML/savefile.py
--rw-rw-rw-   0        0        0      966 2023-04-06 09:07:00.000000 pyoptiML-0.1/src/optiML/testing.py
--rw-rw-rw-   0        0        0     6294 2023-04-06 09:28:10.000000 pyoptiML-0.1/src/optiML/trainingtesting.py
-drwxrwxrwx   0        0        0        0 2023-04-17 10:03:44.577567 pyoptiML-0.1/src/pyoptiML.egg-info/
--rw-rw-rw-   0        0        0     3817 2023-04-17 10:03:44.000000 pyoptiML-0.1/src/pyoptiML.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2023-04-17 10:03:44.000000 pyoptiML-0.1/src/pyoptiML.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 10:03:44.000000 pyoptiML-0.1/src/pyoptiML.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      172 2023-04-17 10:03:44.000000 pyoptiML-0.1/src/pyoptiML.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-17 10:03:44.000000 pyoptiML-0.1/src/pyoptiML.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:38:06.725080 pyoptiML-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-11 14:37:46.000000 pyoptiML-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-11 14:38:06.725080 pyoptiML-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-11 14:37:46.000000 pyoptiML-0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-11 14:37:46.000000 pyoptiML-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-11 14:38:06.725080 pyoptiML-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-11 14:37:46.000000 pyoptiML-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:38:06.717080 pyoptiML-0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:38:06.721080 pyoptiML-0.3/src/optiML/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 14:37:46.000000 pyoptiML-0.3/src/optiML/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-11 14:37:46.000000 pyoptiML-0.3/src/optiML/import_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-05-11 14:37:46.000000 pyoptiML-0.3/src/optiML/preprocessing_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-11 14:37:46.000000 pyoptiML-0.3/src/optiML/preprocessing_data_expert_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-11 14:37:46.000000 pyoptiML-0.3/src/optiML/pyoptiml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-11 14:37:46.000000 pyoptiML-0.3/src/optiML/savefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-11 14:37:46.000000 pyoptiML-0.3/src/optiML/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-05-11 14:37:46.000000 pyoptiML-0.3/src/optiML/trainingtesting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:38:06.721080 pyoptiML-0.3/src/pyoptiML.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-11 14:38:06.000000 pyoptiML-0.3/src/pyoptiML.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-11 14:38:06.000000 pyoptiML-0.3/src/pyoptiML.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:38:06.000000 pyoptiML-0.3/src/pyoptiML.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-11 14:38:06.000000 pyoptiML-0.3/src/pyoptiML.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 14:38:06.000000 pyoptiML-0.3/src/pyoptiML.egg-info/top_level.txt
```

### Comparing `pyoptiML-0.1/LICENSE` & `pyoptiML-0.3/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 alex-christopher
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 alex-christopher
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pyoptiML-0.1/PKG-INFO` & `pyoptiML-0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,69 +1,68 @@
-Metadata-Version: 2.1
-Name: pyoptiML
-Version: 0.1
-Summary: A Machine Learning package for generating model
-Home-page: https://github.com/alex-christopher/pyoptiML
-Author: alex-christopher
-Author-email: alexchristopher154@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/alex-christopher/pyoptiML/issues
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: testing
-License-File: LICENSE
-
-# pyoptiML
-This is a package that is developed to automate all the process of Machine Learning to prepare a optimal model on its own
-
-# What is it?
-automate_ml is a Python package that provides fast model generation for any dataset that contains numerical values in them. It aims to help everyone to create model on their own without most knowledge about Machine Learning and how it works. This package runs on its own and suggest the best algorithm to choose to fit the data that has been processed. 
-
-# Main Features
-Things that automate_ml does:
-1. Importing the data - is way easier now, you can just select the file from the path not to copy the path and paste them to make them run.
-2. Preprocessing - It fills the nan values / NA values /  empty values on its own not with mean median or mode alternatively it uses prediction algorithm to predict the missing values. 
-Reasons : 
-Rather than filling with mean, median or mode values this could help to fill the empty values more accurately.
-Model with the best accuracy will be used to fill the nan values and so the accuracy increases in filling the missing values
-3. Saving - Saving the files is the most important feature that has been processed. This package asks for yes or no kinda questions to save train data, test data, standardized data and even the model everything will be saved in a new folder that is created from where the data has been selected.
-4. Handled outliers with the help of IQR (Interquaratile Range)
-5. Numerical data are stored in csv files
-6. Models are stored in the same folder so we can just load them to test the accuraccy and can be shared
-7. Testing - After the model has been saved it also asks for testing to the user. So here user can just enter the values and the model predicts the output ie the target feature the model is trained with
-8. It shows the total time taken to execute the whole process
-9. This package intracts with the user so it can be more comfortable than coding and creating a model out of it
-
-# Where to get it
-
-The source code is currently hosted on Github at : https://github.com/alex-christopher/pyoptiML
-
-pip install 
-
-# Dependencies
-1. Numpy
-2. Pandas
-3. Scikit-learn
-
-These are the very basic libraries that are needed for machine learning and this package is built with all these to reduce the work that is done by the users
-
-# License
-
-# Documentation
-The official documentation is hosted an PyData.org : 
-
-# Contributing to automate_ml
-
-All contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcomed.
-
-Or maybe through using pandas you have an idea of your own or are looking for something in the documentation and thinking ‘this can be improved’...you can do something about it!
-
-# Features to improve
-1. Used only 4-5 libraries without hyperparameter tuning for the final model generation.
-2. Works only for regression problems 
-3. Works under progress for classification problems
-4. Auto code generation for all the steps or all the progess that the user has done has to be generated on its own 
+Metadata-Version: 2.1
+Name: pyoptiML
+Version: 0.3
+Summary: A Machine Learning package for generating model
+Home-page: https://github.com/alex-christopher/pyoptiML
+Author: alex-christopher
+Author-email: alexchristopher154@gmail.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/alex-christopher/pyoptiML/issues
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Provides-Extra: testing
+License-File: LICENSE
+
+# pyoptiML
+This is a package that is developed to automate all the process of Machine Learning to prepare a optimal model on its own
+
+# What is it?
+automate_ml is a Python package that provides fast model generation for any dataset that contains numerical values in them. It aims to help everyone to create model on their own without most knowledge about Machine Learning and how it works. This package runs on its own and suggest the best algorithm to choose to fit the data that has been processed. 
+
+# Main Features
+Things that automate_ml does:
+1. Importing the data - is way easier now, you can just select the file from the path not to copy the path and paste them to make them run.
+2. Preprocessing - It fills the nan values / NA values /  empty values on its own not with mean median or mode alternatively it uses prediction algorithm to predict the missing values. 
+Reasons : 
+Rather than filling with mean, median or mode values this could help to fill the empty values more accurately.
+Model with the best accuracy will be used to fill the nan values and so the accuracy increases in filling the missing values
+3. Saving - Saving the files is the most important feature that has been processed. This package asks for yes or no kinda questions to save train data, test data, standardized data and even the model everything will be saved in a new folder that is created from where the data has been selected.
+4. Handled outliers with the help of IQR (Interquaratile Range)
+5. Numerical data are stored in csv files
+6. Models are stored in the same folder so we can just load them to test the accuraccy and can be shared
+7. Testing - After the model has been saved it also asks for testing to the user. So here user can just enter the values and the model predicts the output ie the target feature the model is trained with
+8. It shows the total time taken to execute the whole process
+9. This package intracts with the user so it can be more comfortable than coding and creating a model out of it
+
+# Where to get it
+
+The source code is currently hosted on Github at : https://github.com/alex-christopher/pyoptiML
+
+pip install 
+
+# Dependencies
+1. Numpy
+2. Pandas
+3. Scikit-learn
+
+These are the very basic libraries that are needed for machine learning and this package is built with all these to reduce the work that is done by the users
+
+# License
+
+# Documentation
+The official documentation is hosted an PyData.org : 
+
+# Contributing to automate_ml
+
+All contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcomed.
+
+Or maybe through using pandas you have an idea of your own or are looking for something in the documentation and thinking ‘this can be improved’...you can do something about it!
+
+# Features to improve
+1. Used only 4-5 libraries without hyperparameter tuning for the final model generation.
+2. Works only for regression problems 
+3. Works under progress for classification problems
+4. Auto code generation for all the steps or all the progess that the user has done has to be generated on its own
```

### Comparing `pyoptiML-0.1/README.md` & `pyoptiML-0.3/README.md`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-# pyoptiML
-This is a package that is developed to automate all the process of Machine Learning to prepare a optimal model on its own
-
-# What is it?
-automate_ml is a Python package that provides fast model generation for any dataset that contains numerical values in them. It aims to help everyone to create model on their own without most knowledge about Machine Learning and how it works. This package runs on its own and suggest the best algorithm to choose to fit the data that has been processed. 
-
-# Main Features
-Things that automate_ml does:
-1. Importing the data - is way easier now, you can just select the file from the path not to copy the path and paste them to make them run.
-2. Preprocessing - It fills the nan values / NA values /  empty values on its own not with mean median or mode alternatively it uses prediction algorithm to predict the missing values. 
-Reasons : 
-Rather than filling with mean, median or mode values this could help to fill the empty values more accurately.
-Model with the best accuracy will be used to fill the nan values and so the accuracy increases in filling the missing values
-3. Saving - Saving the files is the most important feature that has been processed. This package asks for yes or no kinda questions to save train data, test data, standardized data and even the model everything will be saved in a new folder that is created from where the data has been selected.
-4. Handled outliers with the help of IQR (Interquaratile Range)
-5. Numerical data are stored in csv files
-6. Models are stored in the same folder so we can just load them to test the accuraccy and can be shared
-7. Testing - After the model has been saved it also asks for testing to the user. So here user can just enter the values and the model predicts the output ie the target feature the model is trained with
-8. It shows the total time taken to execute the whole process
-9. This package intracts with the user so it can be more comfortable than coding and creating a model out of it
-
-# Where to get it
-
-The source code is currently hosted on Github at : https://github.com/alex-christopher/pyoptiML
-
-pip install 
-
-# Dependencies
-1. Numpy
-2. Pandas
-3. Scikit-learn
-
-These are the very basic libraries that are needed for machine learning and this package is built with all these to reduce the work that is done by the users
-
-# License
-
-# Documentation
-The official documentation is hosted an PyData.org : 
-
-# Contributing to automate_ml
-
-All contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcomed.
-
-Or maybe through using pandas you have an idea of your own or are looking for something in the documentation and thinking ‘this can be improved’...you can do something about it!
-
-# Features to improve
-1. Used only 4-5 libraries without hyperparameter tuning for the final model generation.
-2. Works only for regression problems 
-3. Works under progress for classification problems
-4. Auto code generation for all the steps or all the progess that the user has done has to be generated on its own 
+# pyoptiML
+This is a package that is developed to automate all the process of Machine Learning to prepare a optimal model on its own
+
+# What is it?
+automate_ml is a Python package that provides fast model generation for any dataset that contains numerical values in them. It aims to help everyone to create model on their own without most knowledge about Machine Learning and how it works. This package runs on its own and suggest the best algorithm to choose to fit the data that has been processed. 
+
+# Main Features
+Things that automate_ml does:
+1. Importing the data - is way easier now, you can just select the file from the path not to copy the path and paste them to make them run.
+2. Preprocessing - It fills the nan values / NA values /  empty values on its own not with mean median or mode alternatively it uses prediction algorithm to predict the missing values. 
+Reasons : 
+Rather than filling with mean, median or mode values this could help to fill the empty values more accurately.
+Model with the best accuracy will be used to fill the nan values and so the accuracy increases in filling the missing values
+3. Saving - Saving the files is the most important feature that has been processed. This package asks for yes or no kinda questions to save train data, test data, standardized data and even the model everything will be saved in a new folder that is created from where the data has been selected.
+4. Handled outliers with the help of IQR (Interquaratile Range)
+5. Numerical data are stored in csv files
+6. Models are stored in the same folder so we can just load them to test the accuraccy and can be shared
+7. Testing - After the model has been saved it also asks for testing to the user. So here user can just enter the values and the model predicts the output ie the target feature the model is trained with
+8. It shows the total time taken to execute the whole process
+9. This package intracts with the user so it can be more comfortable than coding and creating a model out of it
+
+# Where to get it
+
+The source code is currently hosted on Github at : https://github.com/alex-christopher/pyoptiML
+
+pip install 
+
+# Dependencies
+1. Numpy
+2. Pandas
+3. Scikit-learn
+
+These are the very basic libraries that are needed for machine learning and this package is built with all these to reduce the work that is done by the users
+
+# License
+
+# Documentation
+The official documentation is hosted an PyData.org : 
+
+# Contributing to automate_ml
+
+All contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcomed.
+
+Or maybe through using pandas you have an idea of your own or are looking for something in the documentation and thinking ‘this can be improved’...you can do something about it!
+
+# Features to improve
+1. Used only 4-5 libraries without hyperparameter tuning for the final model generation.
+2. Works only for regression problems 
+3. Works under progress for classification problems
+4. Auto code generation for all the steps or all the progess that the user has done has to be generated on its own
```

### Comparing `pyoptiML-0.1/src/optiML/preprocessing_data.py` & `pyoptiML-0.3/src/optiML/preprocessing_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,208 +1,256 @@
-import traceback
-
-import pandas as pd
-import numpy as np
-
-from import_file import data_loading
-
-from sklearn.model_selection import train_test_split
-from sklearn.ensemble import GradientBoostingRegressor
-from sklearn.metrics import r2_score, mean_squared_error
-
-
-class preprocessing_data:
-    def __init__(self):
-        self.dc = data_loading()
-        self.df, self.file_path = self.dc.import_data()
-        self.print = self.dc.print_def
-
-    '''def find_datatype(self):
-        try:
-            if self.df:
-                self.print("PRINTING DATATYPES")
-                # print(self.df.dtypes)
-                float_vals = self.df.select_dtypes(include=['float'])
-                int_vals = self.df.select_dtypes(include=['int'])
-                # print(int_vals)
-                return int_vals, float_vals
-
-
-        except Exception as e:
-            print("Error occurred in find_datatype function", e)'''
-
-    def missing_value_data(self):
-        # int_vals, float_vals = self.find_datatype()
-        try:
-            self.null_columns = self.df.columns[self.df.isna().any()]
-            if not self.null_columns.empty:
-                for i in self.null_columns:
-                    # print("NO OF MISSING VALUES : ", sum_of_missing_values)
-                    print("No of missing values in '{}' : ".format(i), self.df[i].isna().sum())
-
-            else:
-                print("NO NULL VALUES")
-        except Exception as e:
-            print("Missing value function", e)
-
-    def categorical_to_numerical(self):
-        try:
-            categorical_cols = self.df.select_dtypes(include='object')
-            numerical_cols = self.df.select_dtypes(exclude='object')
-
-            if not categorical_cols.empty:
-                self.cat_cols = pd.get_dummies(categorical_cols)
-                # self.cat_cols = self.cat_cols.replace({0 : 1, 1 : 2, np.nan : 0})
-                print(self.cat_cols)
-            else:
-                return self.df
-
-            self.df = pd.concat([numerical_cols, self.cat_cols], axis=1)
-            print(self.df)
-        except Exception as e:
-            print("ERROR IN CATEGORICAL TO NUMERICAL", e)
-
-    def cols_with_more_than_one_missing_values(self):
-        try:
-            counter = 0
-            self.df = self.df.reset_index(drop=True)
-            for i in range(len(self.df.index - 1)):
-                '''print(self.df.index)
-                print(len(self.df.values))
-                print(i)'''
-                c = self.df.iloc[i].isna().values.sum()
-                if c > 1:
-                    self.df = self.df.dropna(thresh=self.df.shape[1] - 1, axis=0)
-                    counter += 1
-                    return self.df
-
-            print(self.df)
-            # print("PLSSSSSSSS", self.new_df)
-            print("COUNTER : ", counter)
-            print("DATA WITH MORE THAN ONE MISSING COLUMN HAS BEEN DROPPED")
-            print("NO OF ROWS DROPPED : ", counter)
-            print("NO OF ROWS REMAINING : ", len(self.df.values) - counter)
-            print("NEW DF \n", self.df)
-            return self.df
-        except Exception as e:
-            print("ERROR IN COLS WITH MORE THAN ONE MISSING VALUE", e)
-
-    def save_visualization(self):
-        pass
-
-    def splitting_data(self):
-        try:
-            # int_vals, float_vals = self.find_datatype()
-            target = []
-            self.df = self.cols_with_more_than_one_missing_values()
-
-            self.categorical_to_numerical()
-            self.missing_value_data()
-            for cols in self.null_columns:
-
-                target.append(cols)
-                print("TARGET : ", target)
-                training_data = self.df.dropna(axis=0)
-                print("TRAINING DATAAAAAAAAA : \n", training_data)
-                testing_data = self.df.drop(training_data.index)
-                print("TESTING DATAAAAA : \n", testing_data)
-
-                x_train = training_data.drop(target, axis=1)
-                print("X TRAIN : \n", x_train)
-                y_train = training_data[target]
-                print("Y TRAIN : \n", y_train)
-
-                # print("XTRAIN : \n", x_train, "\nYTRAIN : \n", y_train)
-                # print("TRAINING DATA\n", training_data)
-                # print("TESTING DATA\n", testing_data)
-
-                x_val_train, x_val_test, y_val_train, y_val_test = train_test_split(x_train, y_train,
-                                                                                    test_size=0.3, random_state=42)
-
-                print("X_val_train : \n", x_val_train, "X_val_test : \n", x_val_test)
-                print("Y_val_train : \n", y_val_train, "Y_val_test : \n", y_val_test)
-                print(x_val_train.shape)
-                print(x_val_test.shape)
-
-                x_test = testing_data.drop(target, axis=1)
-                x_test = x_test.dropna(axis=0)
-                y_test = testing_data[target].loc[x_test.index]
-                print("X_TEST : \n", x_test, "\nY_TEST\n", y_test)
-
-                '''lr = LinearRegression()
-                rid = Ridge()
-
-                model_name = f'{target}_model'
-
-                model_name = rid.fit(x_val_train, y_val_train)
-                prediction = model_name.predict(x_val_test)
-
-                R2_score = r2_score(y_val_test, prediction)
-                mse = mean_squared_error(y_val_test, prediction)
-                print("R2 Score for validation dataset : ", R2_score)
-                print("MEAN SQUARED ERROR for validation dataset : ", mse)'''
-
-                '''HistGrad = HistGradientBoostingRegressor()
-                modelHGB = HistGrad.fit(x_val_train, y_val_train.values.ravel())
-                pred = modelHGB.predict(x_val_test)
-                R2_score = r2_score(y_val_test, pred)
-                mse = mean_squared_error(y_val_test, pred)
-                print(pred)
-                print("R2 : ", R2_score)
-                print("MSE : ", mse)'''
-
-                GradBoost = GradientBoostingRegressor(loss='squared_error',
-                                                      learning_rate=0.1,
-                                                      n_estimators=100,
-                                                      random_state=42)
-                modelGBR = GradBoost.fit(x_val_train, y_val_train.values.ravel())
-                GBR_Pred = modelGBR.predict(x_val_test)
-                R2_score = r2_score(y_val_test, GBR_Pred)
-                mse = mean_squared_error(y_val_test, GBR_Pred)
-                print("R2 : ", R2_score, "\nGBR : ", GBR_Pred, "\nMSE : ", mse)
-
-                if R2_score > 0.8:
-                    print("MODEL FITTED WELL AND GOOD")
-                elif 0.5 > R2_score < 0.8:
-                    print("MODEL FITTED GOOD")
-
-                self.print(f"FILLING MISSING VALUES IN COLUMN {cols}")
-
-                missing_value_prediction = modelGBR.predict(x_test)
-                c = self.df[target].loc[0][0]
-                print(c)
-
-                number_of_decimal_values = str(c)[::-1].find('.')
-                print(number_of_decimal_values)
-
-                print("MISSING VALUE TO BE REPLACED : ", missing_value_prediction)
-
-                print(y_test)
-                print(y_test.index)
-
-                print("NEW Y TEST \n", self.df)
-                print(f"{target} null values : ", self.df.isna().sum())
-
-                print(type(missing_value_prediction))
-
-                # predicted_series_1d = round(missing_value_prediction, 2)
-
-                i = 0
-                for j in y_test.index:
-                    print("BEFORE UPDATION \n", testing_data)
-                    testing_data.loc[[j], target] = np.round(missing_value_prediction[i], number_of_decimal_values)
-                    print("AFTER UPDATION\n", testing_data)
-                    i = i + 1
-
-                self.df = pd.concat([training_data, testing_data], axis=0)
-
-                print("PRINT ALL", self.df)
-
-                target = []
-
-                self.cols_with_more_than_one_missing_values()
-
-            return self.df, self.file_path
-
-        except Exception as e:
-            traceback.print_exc()
-            print("Splitting data function", e)
+import traceback
+
+import pandas as pd
+import numpy as np
+
+from import_file import data_loading
+
+from sklearn.model_selection import train_test_split
+from sklearn.ensemble import GradientBoostingRegressor
+from sklearn.metrics import r2_score, mean_squared_error
+
+
+class Standard_preprocessing_data:
+    def __init__(self):
+        self.dc = data_loading()
+        self.df, self.file_path = self.dc.import_data()
+        self.print = self.dc.print_def
+
+    '''def find_datatype(self):
+        try:
+            if self.df:
+                self.print("PRINTING DATATYPES")
+                # print(self.df.dtypes)
+                float_vals = self.df.select_dtypes(include=['float'])
+                int_vals = self.df.select_dtypes(include=['int'])
+                # print(int_vals)
+                return int_vals, float_vals
+
+
+        except Exception as e:
+            print("Error occurred in find_datatype function", e)'''
+
+    def missing_value_data(self):
+        """
+        This function gets the number of missing values in the every column
+        :return: Missing values
+        """
+        # int_vals, float_vals = self.find_datatype()
+        try:
+            self.null_columns = self.df.columns[self.df.isna().any()]
+            if not self.null_columns.empty:
+                for i in self.null_columns:
+                    # print("NO OF MISSING VALUES : ", sum_of_missing_values)
+                    print("No of missing values in '{}' : ".format(i), self.df[i].isna().sum())
+
+            else:
+                print("NO NULL VALUES")
+        except Exception as e:
+            print("Missing value function", e)
+
+    def categorical_to_numerical(self):
+        """
+        This function converts all the categorical features into numerical features by creating dummies
+        :return:
+        """
+        try:
+            categorical_cols = self.df.select_dtypes(include='object')
+            numerical_cols = self.df.select_dtypes(exclude='object')
+
+            if not categorical_cols.empty:
+                self.cat_cols = pd.get_dummies(categorical_cols)
+                # self.cat_cols = self.cat_cols.replace({0 : 1, 1 : 2, np.nan : 0})
+                print(self.cat_cols)
+            else:
+                return self.df
+
+            self.df = pd.concat([numerical_cols, self.cat_cols], axis=1)
+            print(self.df)
+        except Exception as e:
+            print("ERROR IN CATEGORICAL TO NUMERICAL", e)
+
+    def cols_with_more_than_one_missing_values(self):
+        """
+        This function drops all the rows that contains more than one missing values considering the worst case scenario
+        :return: New dataframe self.df
+        """
+        try:
+            counter = 0
+            self.df = self.df.reset_index(drop=True)
+            for i in range(len(self.df.index - 1)):
+                '''print(self.df.index)
+                print(len(self.df.values))
+                print(i)'''
+                c = self.df.iloc[i].isna().values.sum()
+                if c > 1:
+                    self.df = self.df.dropna(thresh=self.df.shape[1] - 1, axis=0)
+                    counter += 1
+                    return self.df
+
+            print(self.df)
+            # print("PLSSSSSSSS", self.new_df)
+            print("COUNTER : ", counter)
+            print("DATA WITH MORE THAN ONE MISSING COLUMN HAS BEEN DROPPED")
+            print("NO OF ROWS DROPPED : ", counter)
+            print("NO OF ROWS REMAINING : ", len(self.df.values) - counter)
+            print("NEW DF \n", self.df)
+            return self.df
+        except Exception as e:
+            print("ERROR IN COLS WITH MORE THAN ONE MISSING VALUE", e)
+
+    def save_visualization(self):
+        pass
+
+    def splitting_data(self):
+        """
+        This function splits all the data as training and testing to fill the NA values
+        The NA values are considered as the testing data and the model is prepared with XGBoost Regressor to fill in the values
+        :return: New Dataframe self.df, File path from where the data is fetched self.file_path
+        """
+        try:
+            # int_vals, float_vals = self.find_datatype()
+            target = []
+            self.df = self.cols_with_more_than_one_missing_values()
+
+            self.categorical_to_numerical()
+            self.missing_value_data()
+            for cols in self.null_columns:
+
+                target.append(cols)
+                print("TARGET : ", target)
+                training_data = self.df.dropna(axis=0)
+                print("TRAINING DATAAAAAAAAA : \n", training_data)
+                testing_data = self.df.drop(training_data.index)
+                print("TESTING DATAAAAA : \n", testing_data)
+
+                x_train = training_data.drop(target, axis=1)
+                print("X TRAIN : \n", x_train)
+                y_train = training_data[target]
+                print("Y TRAIN : \n", y_train)
+
+                # print("XTRAIN : \n", x_train, "\nYTRAIN : \n", y_train)
+                # print("TRAINING DATA\n", training_data)
+                # print("TESTING DATA\n", testing_data)
+
+                x_val_train, x_val_test, y_val_train, y_val_test = train_test_split(x_train, y_train,
+                                                                                    test_size=0.3, random_state=42)
+
+                print("X_val_train : \n", x_val_train, "X_val_test : \n", x_val_test)
+                print("Y_val_train : \n", y_val_train, "Y_val_test : \n", y_val_test)
+                print(x_val_train.shape)
+                print(x_val_test.shape)
+
+                x_test = testing_data.drop(target, axis=1)
+                x_test = x_test.dropna(axis=0)
+                y_test = testing_data[target].loc[x_test.index]
+                print("X_TEST : \n", x_test, "\nY_TEST\n", y_test)
+
+                '''lr = LinearRegression()
+                rid = Ridge()
+
+                model_name = f'{target}_model'
+
+                model_name = rid.fit(x_val_train, y_val_train)
+                prediction = model_name.predict(x_val_test)
+
+                R2_score = r2_score(y_val_test, prediction)
+                mse = mean_squared_error(y_val_test, prediction)
+                print("R2 Score for validation dataset : ", R2_score)
+                print("MEAN SQUARED ERROR for validation dataset : ", mse)'''
+
+                '''HistGrad = HistGradientBoostingRegressor()
+                modelHGB = HistGrad.fit(x_val_train, y_val_train.values.ravel())
+                pred = modelHGB.predict(x_val_test)
+                R2_score = r2_score(y_val_test, pred)
+                mse = mean_squared_error(y_val_test, pred)
+                print(pred)
+                print("R2 : ", R2_score)
+                print("MSE : ", mse)'''
+
+                GradBoost = GradientBoostingRegressor(loss='squared_error',
+                                                      learning_rate=0.1,
+                                                      n_estimators=100,
+                                                      random_state=42)
+                modelGBR = GradBoost.fit(x_val_train, y_val_train.values.ravel())
+                GBR_Pred = modelGBR.predict(x_val_test)
+                R2_score = r2_score(y_val_test, GBR_Pred)
+                mse = mean_squared_error(y_val_test, GBR_Pred)
+                print("R2 : ", R2_score, "\nGBR : ", GBR_Pred, "\nMSE : ", mse)
+
+                if R2_score > 0.8:
+                    print("MODEL FITTED WELL AND GOOD")
+                elif 0.5 > R2_score < 0.8:
+                    print("MODEL FITTED GOOD")
+
+                self.print(f"FILLING MISSING VALUES IN COLUMN {cols}")
+
+                missing_value_prediction = modelGBR.predict(x_test)
+                c = self.df[target].loc[0][0]
+                print(c)
+
+                number_of_decimal_values = str(c)[::-1].find('.')
+                print(number_of_decimal_values)
+
+                print("MISSING VALUE TO BE REPLACED : ", missing_value_prediction)
+
+                print(y_test)
+                print(y_test.index)
+
+                print("NEW Y TEST \n", self.df)
+                print(f"{target} null values : ", self.df.isna().sum())
+
+                print(type(missing_value_prediction))
+
+                # predicted_series_1d = round(missing_value_prediction, 2)
+
+                i = 0
+                for j in y_test.index:
+                    print("BEFORE UPDATION \n", testing_data)
+                    testing_data.loc[[j], target] = np.round(missing_value_prediction[i], number_of_decimal_values)
+                    print("AFTER UPDATION\n", testing_data)
+                    i = i + 1
+
+                self.df = pd.concat([training_data, testing_data], axis=0)
+
+                print("PRINT ALL", self.df)
+
+                target = []
+
+                self.cols_with_more_than_one_missing_values()
+
+            return self.df, self.file_path
+
+        except Exception as e:
+            traceback.print_exc()
+            print("Splitting data function", e)
+
+class Expert_preprocessing_data:
+    def __int__(self):
+        self.dc = data_loading()
+        self.df, self.file_path = self.dc.import_data()
+        self.print = self.dc.print_def
+    def find_datatypes(self, data):
+        try:
+            if data:
+                float_values = data.select_dtypes(include=["float"])
+                integer_values = data.select_dtypes(include=["int"])
+                date_pattern = r'\d{4}-\d{2}-\d{2}'
+                return float_values, integer_values
+        finally:
+            print("Segregated with datatypes")
+
+    def fill_missing_values(self):
+        missing_vals = ["Mean", "Median", "Mode", "Prediction", "Drop Missing value"]
+        for i in missing_vals:
+            print(i)
+        while True:
+            missing_vals_input = str(input("Enter the method to fill the missing values : "))
+            if missing_vals_input in missing_vals:
+                if missing_vals.lower() == "mean":
+                    for i in self.df.columns:
+                        self.df[i].fillna(method="mean", inplace=True)
+
+
+
+
+
```

### Comparing `pyoptiML-0.1/src/optiML/savefile.py` & `pyoptiML-0.3/src/optiML/savefile.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-import os
-from preprocessing_data import preprocessing_data
-import pickle
-
-
-class savefileas:
-    def __init__(self):
-        pre = preprocessing_data()
-        self.df, self.file_path = pre.splitting_data()
-
-    def fixing_file_path(self):
-        save_option = str(input("Do you like to save the updated dataframe in .csv format? [y/n] : "))
-        if save_option.lower()[0] == 'y':
-            print(self.file_path)
-            folder_path = os.path.split(self.file_path)[0]
-            folder_name = os.path.split(self.file_path)[1]
-
-            i = 0
-            while True:
-                if i == 0:
-                    complete_path = os.path.join(folder_path, folder_name)
-                else:
-                    complete_path = os.path.join(folder_path, f'{folder_name}({i})')
-                if not os.path.exists(complete_path):
-                    os.mkdir(complete_path)
-                    break
-                i += 1
-
-            # os.mkdir(complete_path)
-            csv_path = f'Preprocessed_{folder_name}.csv'
-            print(csv_path)
-
-            os.chdir(complete_path)
-            self.df.to_csv(csv_path, index=False)
-            print("SAVED")
-            return self.df, complete_path
-        else:
-            print("FILE NOT SAVED")
-        return self.df, None
-
-    def save_model(self, model, model_name):
-        save_option = str(input("Do you like to save the model? [y/n] : "))
-        if save_option.lower() == 'y':
-            pickle.dump(model, open(self.file_path / f"{model_name}.pkl"), "wb")
-            print(f"MODEL SAVED IN {self.file_path}")
-        else:
-            print("MODEL NOT SAVED")
-        return
+import os
+from preprocessing_data import Standard_preprocessing_data
+import pickle
+
+
+class savefileas:
+    def __init__(self):
+        pre = Standard_preprocessing_data()
+        self.df, self.file_path = pre.splitting_data()
+
+    def fixing_file_path(self):
+        save_option = str(input("Do you like to save the updated dataframe in .csv format? [y/n] : "))
+        if save_option.lower()[0] == 'y':
+            print(self.file_path)
+            folder_path = os.path.split(self.file_path)[0]
+            folder_name = os.path.split(self.file_path)[1]
+
+            i = 0
+            while True:
+                if i == 0:
+                    complete_path = os.path.join(folder_path, folder_name)
+                else:
+                    complete_path = os.path.join(folder_path, f'{folder_name}({i})')
+                if not os.path.exists(complete_path):
+                    os.mkdir(complete_path)
+                    break
+                i += 1
+
+            # os.mkdir(complete_path)
+            csv_path = f'Preprocessed_{folder_name}.csv'
+            print(csv_path)
+
+            os.chdir(complete_path)
+            self.df.to_csv(csv_path, index=False)
+            print("SAVED")
+            return self.df, complete_path
+        else:
+            print("FILE NOT SAVED")
+        return self.df, None
+
+    def save_model(self, model, model_name):
+        save_option = str(input("Do you like to save the model? [y/n] : "))
+        if save_option.lower() == 'y':
+            pickle.dump(model, open(self.file_path / f"{model_name}.pkl"), "wb")
+            print(f"MODEL SAVED IN {self.file_path}")
+        else:
+            print("MODEL NOT SAVED")
+        return
```

### Comparing `pyoptiML-0.1/src/optiML/testing.py` & `pyoptiML-0.3/src/optiML/testing.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from trainingtesting import model_creation
-import pickle
-
-
-class testing_module:
-
-    def __init__(self):
-        model = model_creation()
-        self.df = model.treating_outliers()
-        self.x, self.y, self.generated_model, self.target = model.final_model_generation()
-
-    def testing_user_input(self):
-        try:
-            test_input = str(input("Do you like to test your model [y/n] : "))
-            if test_input.lower()[0] == 'y':
-                append_values = []
-                for i in self.x.columns:
-                    values = float(input(f"Enter the value for {i} : "))
-                    append_values.append(values)
-
-                load_model = pickle.load(open(self.generated_model, 'rb'))
-                pred = load_model.predict([append_values])
-                print("Predicted output : ", pred[0])
-            else:
-                print("THANK YOU")
-        finally:
-            print("MODEL EXECUTED")
+from trainingtesting import model_creation
+import pickle
+
+
+class testing_module:
+
+    def __init__(self):
+        model = model_creation()
+        self.df = model.treating_outliers()
+        self.x, self.y, self.generated_model, self.target = model.final_model_generation()
+
+    def testing_user_input(self):
+        try:
+            test_input = str(input("Do you like to test your model [y/n] : "))
+            if test_input.lower()[0] == 'y':
+                append_values = []
+                for i in self.x.columns:
+                    values = float(input(f"Enter the value for {i} : "))
+                    append_values.append(values)
+
+                load_model = pickle.load(open(self.generated_model, 'rb'))
+                pred = load_model.predict([append_values])
+                print("Predicted output : ", pred[0])
+            else:
+                print("THANK YOU")
+        finally:
+            print("MODEL EXECUTED")
```

### Comparing `pyoptiML-0.1/src/optiML/trainingtesting.py` & `pyoptiML-0.3/src/optiML/trainingtesting.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,163 +1,188 @@
-import sys
-
-import numpy as np
-import pandas as pd
-import os
-import matplotlib.pyplot as plt
-
-from savefile import savefileas
-
-from sklearn.preprocessing import StandardScaler
-from sklearn.model_selection import train_test_split
-from sklearn.metrics import mean_squared_error, r2_score
-
-from sklearn.linear_model import LinearRegression, Ridge, Lasso, ElasticNet
-
-from sklearn.ensemble import GradientBoostingRegressor
-
-import pickle
-
-sc = StandardScaler()
-
-
-class model_creation:
-    def __init__(self):
-        self.save = savefileas()
-        self.df, self.path = self.save.fixing_file_path()
-
-    def new_save(self, process, data, file_format):
-        self.save_file = str(input(f"Do you like to save the {process} as {file_format} file? [y/n] : "))
-        if self.save_file.lower()[0] == 'y':
-            folder_name = os.path.split(self.path)[1]
-            if file_format == ".csv":
-                file_name = f'{process}_{folder_name}{file_format}'
-                print(file_name)
-                os.chdir(self.path)
-                data.to_csv(file_name, index=False)
-                print(f'{process} saved')
-
-            elif file_format == ".pkl":
-                self.model_file_name = f'{process}_{folder_name}{file_format}'
-                pickle.dump(data, open(self.model_file_name, 'wb'))
-                print('MODEL IS BEING SAVED...')
-                print("MODEL SAVED")
-
-            elif file_format == ".jpg":
-                plt.imsave(f'{process}_{data}{file_format}', data)
-            else:
-                print("FILE NOT SAVED")
-                sys.exit()
-        else:
-            print("FILE NOT SAVED")
-
-    def visualization(self, column, process):
-        hist = plt.hist(self.df[column])
-        plt.imsave(f'Before_Outliers{column}.jpg', hist)
-        box = plt.box(self.df[column])
-        self.new_save(process, box, ".jpg")
-
-    def treating_outliers(self):
-        try:
-            for i in self.df.columns:
-                Q1 = self.df[i].quantile(.25)
-                Q3 = self.df[i].quantile(.75)
-                IQR = Q3 - Q1
-                lower = Q1 - 1.5 * IQR
-                upper = Q3 + 1.5 * IQR
-                print(f"LOWER LIMIT FOR {i} : ", round(lower, 2))
-                print(f"UPPER LIMIT FOR {i} : ", round(upper, 2))
-
-                self.df[i] = np.where(self.df[i] > upper, upper,
-                                      np.where(self.df[i] < lower, lower, self.df[i]))
-            return self.df
-        except Exception as e:
-            print("ERROR IN REMOVING OUTLIERS", e)
-
-    def train_test_split_(self):
-        # self.df = self.treating_outliers()
-        for i in self.df.columns:
-            print(i)
-        while True:
-            target = input("Select the target column : ")
-            if target in self.df.columns:
-                x = self.df.drop(target, axis=1)
-                y = self.df[target]
-                self.x_train, self.x_test, self.y_train, self.y_test = train_test_split(x, y, test_size=0.3,
-                                                                                        random_state=42)
-                print("Test size is set to 0.3 by default")
-                training_data = pd.concat([self.x_train, self.y_train], axis=1)
-                train_data = pd.DataFrame(training_data)
-                testing_data = pd.concat([self.x_test, self.y_test], axis=1)
-                test_data = pd.DataFrame(testing_data)
-                self.new_save("Train values", train_data, ".csv")
-                # print("Train data saved")
-                self.new_save("Test values", test_data, ".csv")
-                # print("Test data saved")
-                break
-            else:
-                print("Enter the appropriate column name")
-
-        return x, y, target
-
-    def standardization(self):
-        self.df = sc.fit_transform(self.df)
-        standard = pd.DataFrame(self.df)
-        self.new_save("Standardized", standard, ".csv")
-
-    def validation_model_generation(self):
-
-        self.standardization()
-        x_train = sc.fit_transform(self.x_train)
-        x_test = sc.transform(self.x_test)
-
-        GradBoost = GradientBoostingRegressor(loss='squared_error',
-                                              learning_rate=0.1,
-                                              n_estimators=100,
-                                              random_state=42)
-        LinearReg = LinearRegression()
-        RidgeReg = Ridge()
-        ElasticNetReg = ElasticNet()
-        LassoReg = Lasso()
-
-        models = [GradBoost,
-                  LinearReg,
-                  RidgeReg,
-                  ElasticNetReg,
-                  LassoReg]
-
-        r2 = []
-        mse_ = []
-
-        for model in models:
-            modelGBR = model.fit(x_train, self.y_train.values.ravel())
-            Prediction = modelGBR.predict(x_test)
-            R2_score = r2_score(self.y_test, Prediction)
-            r2.append(R2_score)
-            mse = mean_squared_error(self.y_test, Prediction)
-            mse_.append(mse)
-            print(f"{model}")
-            print("R2 : ", R2_score, "\nMSE : ", mse)
-        model_selection = ['Gradient Boosting Regressor',
-                           'Linear Regression',
-                           'Ridge Regression',
-                           'Elastic Net Regression',
-                           'Lasso Regression']
-        greatest_index = r2.index(max(r2))
-        best_model = models[greatest_index]
-        suggest_model = model_selection[greatest_index]
-        print("BEST MODEL : ", suggest_model)
-        return greatest_index, best_model
-
-    def final_model_generation(self):
-        try:
-            x, y, target = self.train_test_split_()
-            index_values, validation = self.validation_model_generation()
-
-            new_model = validation.fit(x, y.values.ravel())
-            self.new_save("Model", new_model, ".pkl")
-            if self.save_file.lower() == 'y':
-                return x, y, self.model_file_name, target
-            else:
-                return x, y, new_model, target
-        except Exception as e:
-            print("ERROR AT MODEL GENERATION", e)
+import sys
+
+import numpy as np
+import pandas as pd
+import os
+import matplotlib.pyplot as plt
+
+from savefile import savefileas
+
+from sklearn.preprocessing import StandardScaler
+from sklearn.model_selection import train_test_split
+from sklearn.metrics import mean_squared_error, r2_score
+
+from sklearn.linear_model import LinearRegression, Ridge, Lasso, ElasticNet
+
+from sklearn.ensemble import GradientBoostingRegressor
+
+import pickle
+
+sc = StandardScaler()
+
+
+class model_creation:
+    def __init__(self):
+        self.save = savefileas()
+        self.df, self.path = self.save.fixing_file_path()
+
+    def new_save(self, process, data, file_format):
+        '''
+        This function in general is used to save the file or data in a particular format
+        :param process: Standardization, testing, training etc.
+        :param data: The data that has to be saved
+        :param file_format: pkl format for models and csv for numerical data and jpg for visualization
+        :return:
+        '''
+        self.save_file = str(input(f"Do you like to save the {process} as {file_format} file? [y/n] : "))
+        if self.save_file.lower()[0] == 'y':
+            folder_name = os.path.split(self.path)[1]
+            if file_format == ".csv":
+                file_name = f'{process}_{folder_name}{file_format}'
+                print(file_name)
+                os.chdir(self.path)
+                data.to_csv(file_name, index=False)
+                print(f'{process} saved')
+
+            elif file_format == ".pkl":
+                self.model_file_name = f'{process}_{folder_name}{file_format}'
+                pickle.dump(data, open(self.model_file_name, 'wb'))
+                print('MODEL IS BEING SAVED...')
+                print("MODEL SAVED")
+
+            elif file_format == ".jpg":
+                plt.imsave(f'{process}_{data}{file_format}', data)
+            else:
+                print("FILE NOT SAVED")
+                sys.exit()
+        else:
+            print("FILE NOT SAVED")
+
+    def visualization(self, column, process):
+        hist = plt.hist(self.df[column])
+        plt.imsave(f'Before_Outliers{column}.jpg', hist)
+        box = plt.box(self.df[column])
+        self.new_save(process, box, ".jpg")
+
+    def treating_outliers(self):
+        '''
+        This function treats the outliers with Interquaratile range 25% for the minimum value and 75% for maximum value
+        :return: self.df The updated new dataframe
+        '''
+        try:
+            for i in self.df.columns:
+                Q1 = self.df[i].quantile(.25)
+                Q3 = self.df[i].quantile(.75)
+                IQR = Q3 - Q1
+                lower = Q1 - 1.5 * IQR
+                upper = Q3 + 1.5 * IQR
+                print(f"LOWER LIMIT FOR {i} : ", round(lower, 2))
+                print(f"UPPER LIMIT FOR {i} : ", round(upper, 2))
+
+                self.df[i] = np.where(self.df[i] > upper, upper,
+                                      np.where(self.df[i] < lower, lower, self.df[i]))
+            return self.df
+        except Exception as e:
+            print("ERROR IN REMOVING OUTLIERS", e)
+
+    def train_test_split_(self):
+        """
+        This function in splits the data for training and testing
+        :return: New updated dataframe self.df
+        """
+        # self.df = self.treating_outliers()
+        for i in self.df.columns:
+            print(i)
+        while True:
+            target = input("Select the target column : ")
+            if target in self.df.columns:
+                x = self.df.drop(target, axis=1)
+                y = self.df[target]
+                self.x_train, self.x_test, self.y_train, self.y_test = train_test_split(x, y, test_size=0.3,
+                                                                                        random_state=42)
+                print("Test size is set to 0.3 by default")
+                training_data = pd.concat([self.x_train, self.y_train], axis=1)
+                train_data = pd.DataFrame(training_data)
+                testing_data = pd.concat([self.x_test, self.y_test], axis=1)
+                test_data = pd.DataFrame(testing_data)
+                self.new_save("Train values", train_data, ".csv")
+                # print("Train data saved")
+                self.new_save("Test values", test_data, ".csv")
+                # print("Test data saved")
+                break
+            else:
+                print("Enter the appropriate column name")
+
+        return x, y, target
+
+    def standardization(self):
+        self.df = sc.fit_transform(self.df)
+        standard = pd.DataFrame(self.df)
+        self.new_save("Standardized", standard, ".csv")
+
+    def validation_model_generation(self):
+        """
+        This function creates a validation model that can be used to check which model fits well and that can be suggested to the user
+        :return: Least MSE value as the greatest index and model as the best model will be suggested
+        """
+        self.standardization()
+        x_train = sc.fit_transform(self.x_train)
+        x_test = sc.transform(self.x_test)
+
+        GradBoost = GradientBoostingRegressor(loss='squared_error',
+                                              learning_rate=0.1,
+                                              n_estimators=100,
+                                              random_state=42)
+        LinearReg = LinearRegression()
+        RidgeReg = Ridge()
+        ElasticNetReg = ElasticNet()
+        LassoReg = Lasso()
+
+        models = [GradBoost,
+                  LinearReg,
+                  RidgeReg,
+                  ElasticNetReg,
+                  LassoReg]
+
+        r2 = []
+        mse_ = []
+
+        for model in models:
+            modelGBR = model.fit(x_train, self.y_train.values.ravel())
+            Prediction = modelGBR.predict(x_test)
+            R2_score = r2_score(self.y_test, Prediction)
+            r2.append(R2_score)
+            mse = mean_squared_error(self.y_test, Prediction)
+            mse_.append(mse)
+            print(f"{model}")
+            print("R2 : ", R2_score, "\nMSE : ", mse)
+        model_selection = ['Gradient Boosting Regressor',
+                           'Linear Regression',
+                           'Ridge Regression',
+                           'Elastic Net Regression',
+                           'Lasso Regression']
+        greatest_index = r2.index(max(r2))
+        best_model = models[greatest_index]
+        suggest_model = model_selection[greatest_index]
+        print("BEST MODEL : ", suggest_model)
+        return greatest_index, best_model
+
+    def final_model_generation(self):
+        """
+        This function will generate the real model that can be reused
+        :return:  x values as x
+                  y values as y
+                  model as model_file_name
+                  target as target for cross checking purposes
+        """
+        try:
+            x, y, target = self.train_test_split_()
+            index_values, validation = self.validation_model_generation()
+
+            new_model = validation.fit(x, y.values.ravel())
+            self.new_save("Model", new_model, ".pkl")
+            if self.save_file.lower() == 'y':
+                return x, y, self.model_file_name, target
+            else:
+                return x, y, new_model, target
+        except Exception as e:
+            print("ERROR AT MODEL GENERATION", e)
```

### Comparing `pyoptiML-0.1/src/pyoptiML.egg-info/PKG-INFO` & `pyoptiML-0.3/src/pyoptiML.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,69 +1,68 @@
-Metadata-Version: 2.1
-Name: pyoptiML
-Version: 0.1
-Summary: A Machine Learning package for generating model
-Home-page: https://github.com/alex-christopher/pyoptiML
-Author: alex-christopher
-Author-email: alexchristopher154@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/alex-christopher/pyoptiML/issues
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: testing
-License-File: LICENSE
-
-# pyoptiML
-This is a package that is developed to automate all the process of Machine Learning to prepare a optimal model on its own
-
-# What is it?
-automate_ml is a Python package that provides fast model generation for any dataset that contains numerical values in them. It aims to help everyone to create model on their own without most knowledge about Machine Learning and how it works. This package runs on its own and suggest the best algorithm to choose to fit the data that has been processed. 
-
-# Main Features
-Things that automate_ml does:
-1. Importing the data - is way easier now, you can just select the file from the path not to copy the path and paste them to make them run.
-2. Preprocessing - It fills the nan values / NA values /  empty values on its own not with mean median or mode alternatively it uses prediction algorithm to predict the missing values. 
-Reasons : 
-Rather than filling with mean, median or mode values this could help to fill the empty values more accurately.
-Model with the best accuracy will be used to fill the nan values and so the accuracy increases in filling the missing values
-3. Saving - Saving the files is the most important feature that has been processed. This package asks for yes or no kinda questions to save train data, test data, standardized data and even the model everything will be saved in a new folder that is created from where the data has been selected.
-4. Handled outliers with the help of IQR (Interquaratile Range)
-5. Numerical data are stored in csv files
-6. Models are stored in the same folder so we can just load them to test the accuraccy and can be shared
-7. Testing - After the model has been saved it also asks for testing to the user. So here user can just enter the values and the model predicts the output ie the target feature the model is trained with
-8. It shows the total time taken to execute the whole process
-9. This package intracts with the user so it can be more comfortable than coding and creating a model out of it
-
-# Where to get it
-
-The source code is currently hosted on Github at : https://github.com/alex-christopher/pyoptiML
-
-pip install 
-
-# Dependencies
-1. Numpy
-2. Pandas
-3. Scikit-learn
-
-These are the very basic libraries that are needed for machine learning and this package is built with all these to reduce the work that is done by the users
-
-# License
-
-# Documentation
-The official documentation is hosted an PyData.org : 
-
-# Contributing to automate_ml
-
-All contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcomed.
-
-Or maybe through using pandas you have an idea of your own or are looking for something in the documentation and thinking ‘this can be improved’...you can do something about it!
-
-# Features to improve
-1. Used only 4-5 libraries without hyperparameter tuning for the final model generation.
-2. Works only for regression problems 
-3. Works under progress for classification problems
-4. Auto code generation for all the steps or all the progess that the user has done has to be generated on its own 
+Metadata-Version: 2.1
+Name: pyoptiML
+Version: 0.3
+Summary: A Machine Learning package for generating model
+Home-page: https://github.com/alex-christopher/pyoptiML
+Author: alex-christopher
+Author-email: alexchristopher154@gmail.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/alex-christopher/pyoptiML/issues
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Provides-Extra: testing
+License-File: LICENSE
+
+# pyoptiML
+This is a package that is developed to automate all the process of Machine Learning to prepare a optimal model on its own
+
+# What is it?
+automate_ml is a Python package that provides fast model generation for any dataset that contains numerical values in them. It aims to help everyone to create model on their own without most knowledge about Machine Learning and how it works. This package runs on its own and suggest the best algorithm to choose to fit the data that has been processed. 
+
+# Main Features
+Things that automate_ml does:
+1. Importing the data - is way easier now, you can just select the file from the path not to copy the path and paste them to make them run.
+2. Preprocessing - It fills the nan values / NA values /  empty values on its own not with mean median or mode alternatively it uses prediction algorithm to predict the missing values. 
+Reasons : 
+Rather than filling with mean, median or mode values this could help to fill the empty values more accurately.
+Model with the best accuracy will be used to fill the nan values and so the accuracy increases in filling the missing values
+3. Saving - Saving the files is the most important feature that has been processed. This package asks for yes or no kinda questions to save train data, test data, standardized data and even the model everything will be saved in a new folder that is created from where the data has been selected.
+4. Handled outliers with the help of IQR (Interquaratile Range)
+5. Numerical data are stored in csv files
+6. Models are stored in the same folder so we can just load them to test the accuraccy and can be shared
+7. Testing - After the model has been saved it also asks for testing to the user. So here user can just enter the values and the model predicts the output ie the target feature the model is trained with
+8. It shows the total time taken to execute the whole process
+9. This package intracts with the user so it can be more comfortable than coding and creating a model out of it
+
+# Where to get it
+
+The source code is currently hosted on Github at : https://github.com/alex-christopher/pyoptiML
+
+pip install 
+
+# Dependencies
+1. Numpy
+2. Pandas
+3. Scikit-learn
+
+These are the very basic libraries that are needed for machine learning and this package is built with all these to reduce the work that is done by the users
+
+# License
+
+# Documentation
+The official documentation is hosted an PyData.org : 
+
+# Contributing to automate_ml
+
+All contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcomed.
+
+Or maybe through using pandas you have an idea of your own or are looking for something in the documentation and thinking ‘this can be improved’...you can do something about it!
+
+# Features to improve
+1. Used only 4-5 libraries without hyperparameter tuning for the final model generation.
+2. Works only for regression problems 
+3. Works under progress for classification problems
+4. Auto code generation for all the steps or all the progess that the user has done has to be generated on its own
```

