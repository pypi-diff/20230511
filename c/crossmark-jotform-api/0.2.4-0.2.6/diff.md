# Comparing `tmp/crossmark-jotform-api-0.2.4.tar.gz` & `tmp/crossmark-jotform-api-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossmark-jotform-api-0.2.4.tar", last modified: Tue May  2 04:07:45 2023, max compression
+gzip compressed data, was "crossmark-jotform-api-0.2.6.tar", last modified: Wed May 10 22:12:26 2023, max compression
```

## Comparing `crossmark-jotform-api-0.2.4.tar` & `crossmark-jotform-api-0.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 04:07:45.124176 crossmark-jotform-api-0.2.4/
--rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     2446 2023-05-02 04:07:45.123178 crossmark-jotform-api-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      546 2023-05-02 04:06:48.000000 crossmark-jotform-api-0.2.4/README.md
--rw-rw-rw-   0        0        0      789 2023-05-02 04:06:56.000000 crossmark-jotform-api-0.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 04:07:45.125140 crossmark-jotform-api-0.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-02 04:07:45.105141 crossmark-jotform-api-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 04:07:45.111141 crossmark-jotform-api-0.2.4/src/crossmark_jotform_api/
--rw-rw-rw-   0        0        0    12786 2023-05-02 04:01:53.000000 crossmark-jotform-api-0.2.4/src/crossmark_jotform_api/jotForm.py
-drwxrwxrwx   0        0        0        0 2023-05-02 04:07:45.121142 crossmark-jotform-api-0.2.4/src/crossmark_jotform_api.egg-info/
--rw-rw-rw-   0        0        0     2446 2023-05-02 04:07:45.000000 crossmark-jotform-api-0.2.4/src/crossmark_jotform_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-02 04:07:45.000000 crossmark-jotform-api-0.2.4/src/crossmark_jotform_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 04:07:45.000000 crossmark-jotform-api-0.2.4/src/crossmark_jotform_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-02 04:07:45.000000 crossmark-jotform-api-0.2.4/src/crossmark_jotform_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 22:12:26.448674 crossmark-jotform-api-0.2.6/
+-rw-rw-rw-   0        0        0     1091 2023-02-01 01:57:52.000000 crossmark-jotform-api-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0     2446 2023-05-10 22:12:26.447677 crossmark-jotform-api-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      546 2023-05-10 22:11:10.000000 crossmark-jotform-api-0.2.6/README.md
+-rw-rw-rw-   0        0        0      789 2023-05-10 22:10:43.000000 crossmark-jotform-api-0.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 22:12:26.448674 crossmark-jotform-api-0.2.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 22:12:26.430680 crossmark-jotform-api-0.2.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 22:12:26.436674 crossmark-jotform-api-0.2.6/src/crossmark_jotform_api/
+-rw-rw-rw-   0        0        0    13153 2023-05-10 22:10:29.000000 crossmark-jotform-api-0.2.6/src/crossmark_jotform_api/jotForm.py
+drwxrwxrwx   0        0        0        0 2023-05-10 22:12:26.445676 crossmark-jotform-api-0.2.6/src/crossmark_jotform_api.egg-info/
+-rw-rw-rw-   0        0        0     2446 2023-05-10 22:12:26.000000 crossmark-jotform-api-0.2.6/src/crossmark_jotform_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-10 22:12:26.000000 crossmark-jotform-api-0.2.6/src/crossmark_jotform_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 22:12:26.000000 crossmark-jotform-api-0.2.6/src/crossmark_jotform_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-10 22:12:26.000000 crossmark-jotform-api-0.2.6/src/crossmark_jotform_api.egg-info/top_level.txt
```

### Comparing `crossmark-jotform-api-0.2.4/LICENSE` & `crossmark-jotform-api-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `crossmark-jotform-api-0.2.4/PKG-INFO` & `crossmark-jotform-api-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.2.4
+Version: 0.2.6
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `crossmark-jotform-api-0.2.4/README.md` & `crossmark-jotform-api-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `crossmark-jotform-api-0.2.4/pyproject.toml` & `crossmark-jotform-api-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","requests>=2.22.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crossmark-jotform-api"
-version = "0.2.4"
+version = "0.2.6"
 authors = [
   { name="Renas Mirkan Kilic", email="mirkanbaba1@gmail.com" },
 ]
 description = "Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `crossmark-jotform-api-0.2.4/src/crossmark_jotform_api/jotForm.py` & `crossmark-jotform-api-0.2.6/src/crossmark_jotform_api/jotForm.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,24 +25,27 @@
         if self.debug:
             print(text)
 
     def __set_get_submission_data(self, submissions):
         submissions_dict = {}
         for i in submissions:
             submissions_dict[i["id"]] = JotFormSubmission(i)
-        # sorted_tuples = sorted(submissions_dict.items(), key=lambda x: x[1].id, reverse=True)
-        # submissions_dict = dict(sorted_tuples)
         return submissions_dict
 
     def get_submission_ids(self):
         return self.submission_ids
 
-    def set_submission_ids(self):
+    def __set_submissions_and_ids(self):
+        """This function sets the submission memory. It is used for easier for loop for submissions. 
+        It is called in the constructor, and time to time in other functions"""
+        self.submission_ids = set()
+        self.submissions = []
         for key, value in self.submission_data.items():
             self.submission_ids.add(value.id)
+            self.submissions.append(value.to_dict())
 
     def set_submission_count(self):
         self.submission_count = len(self.submission_ids)
 
     def get_submission_data(self):
         self.update()
         return self.submission_data
@@ -114,14 +117,18 @@
     def update_submission_answer(self, submission_id, answer_id, answer):
         self.update()
         query = f'submission[{answer_id}]={answer}'
         url = f"https://api.jotform.com/submission/{submission_id}?apiKey={self.api_key}&{query}"
         response = requests.request("POST", url, timeout=self.timeout)
         if response.status_code == 200:
             self.submission_data[submission_id].set_answer(answer_id, answer)
+            for submission in self.submissions:
+                if submission['id'] == submission_id:
+                    submission['answers'][answer_id] = answer
+                    break
             return True
         else:
             return False
 
     def set_url_param(self, key, value):
         value = str(value)
         if key in self.url:
@@ -154,15 +161,15 @@
             self.set_url_param(
                 "offset", self.data['resultSet']['offset'] + count)
             return self.set_data()
         self.set_global_data()
 
     def set_global_data(self):
         self._sort_submission_data_by_id()
-        self.set_submission_ids()
+        self.__set_submissions_and_ids()
         self.set_submission_count()
         self.set_url_param("offset", "0")
 
     def request_submission_by_case_id(self, case_id):
         '''
             Requests the submission by case id
             this function is used when the submission is not in the submission data
```

### Comparing `crossmark-jotform-api-0.2.4/src/crossmark_jotform_api.egg-info/PKG-INFO` & `crossmark-jotform-api-0.2.6/src/crossmark_jotform_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossmark-jotform-api
-Version: 0.2.4
+Version: 0.2.6
 Summary: Jotform api integration dedicated for server usage which limits calls and calling form only if there is a new submission
 Author-email: Renas Mirkan Kilic <mirkanbaba1@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

