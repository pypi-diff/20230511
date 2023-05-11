# Comparing `tmp/alacorder-80.3.7.tar.gz` & `tmp/alacorder-80.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.3.7.tar", max compression
+gzip compressed data, was "alacorder-80.3.8.tar", max compression
```

## Comparing `alacorder-80.3.7.tar` & `alacorder-80.3.8.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.3.7/LICENSE
--rw-r--r--   0        0        0     6538 2023-05-09 14:42:24.077836 alacorder-80.3.7/README.md
--rw-r--r--   0        0        0      697 2023-05-10 22:46:53.867967 alacorder-80.3.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.3.7/src/alacorder/__init__.py
--rw-r--r--   0        0        0   210898 2023-05-10 22:45:11.591026 alacorder-80.3.7/src/alacorder/__main__.py
--rw-r--r--   0        0        0   210898 2023-05-10 22:45:05.975144 alacorder-80.3.7/src/alacorder/alac.py
--rw-r--r--   0        0        0     7467 1970-01-01 00:00:00.000000 alacorder-80.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.3.8/LICENSE
+-rw-r--r--   0        0        0     6538 2023-05-09 14:42:24.077836 alacorder-80.3.8/README.md
+-rw-r--r--   0        0        0      697 2023-05-11 16:52:50.223899 alacorder-80.3.8/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-11 16:53:19.663002 alacorder-80.3.8/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.3.8/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   210937 2023-05-11 16:52:36.878159 alacorder-80.3.8/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   210937 2023-05-11 16:52:14.477544 alacorder-80.3.8/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7467 1970-01-01 00:00:00.000000 alacorder-80.3.8/PKG-INFO
```

### Comparing `alacorder-80.3.7/LICENSE` & `alacorder-80.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.3.7/README.md` & `alacorder-80.3.8/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.3.7/pyproject.toml` & `alacorder-80.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.3.7"
+version = "80.3.8"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.3.7/src/alacorder/__main__.py` & `alacorder-80.3.8/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.3.7"
+version = "80.3.8"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
 from datetime import datetime
+from random import sample
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.chrome.options import Options
 
 
 #   #   #   #                LOGS                #   #   #   #
@@ -432,16 +433,14 @@
     cID="",
     uID="",
     pwd="",
     qmax=0,
     qskip=0,
     pairs=None,
     vrr_summary=False,
-    charges_summary=False,
-    convictions_summary=False,
     append=False,
     window=None,
     force=False,
     no_update=False,
     now=False,
 ):
     """
@@ -462,16 +461,14 @@
         cID (str, optional): Customer ID on Alacourt.com
         uID (str, optional): User ID on Alacourt.com
         pwd (str, optional): Password on Alacourt.com
         qmax (int, optional): Maximum queries to conduct on Alacourt.com
         qskip (int, optional): Skip entries at top of query file
         pairs (str, optional): Path to AIS / Unique ID pairs for grouped table functions
         vrr_summary (bool, optional): Create voting rights summary from pairs
-        charges_summary (bool, optional): Create charges summary from pairs
-        convictions_summary (bool, optional): Create convictions summary from pairs
         append (bool, optional): Append one archive to another
         window (None, optional): PySimpleGUI window element
         force (bool, optional): Do not raise exceptions
         no_update (bool, optional): Do not mark input query when fetching cases
         now (bool, optional): Start Alacorder upon successful configuration
     """
     return cf(
@@ -489,16 +486,14 @@
         cID=cID,
         uID=uID,
         pwd=pwd,
         qmax=qmax,
         qskip=qskip,
         pairs=pairs,
         vrr_summary=vrr_summary,
-        charges_summary=charges_summary,
-        convictions_summary=convictions_summary,
         append=append,
         window=window,
         force=force,
         no_update=no_update,
         now=now,
     )
 
@@ -516,18 +511,17 @@
     no_write=False,
     fetch=False,
     cID="",
     uID="",
     pwd="",
     qmax=0,
     qskip=0,
+    criminal_only=False,
     pairs=None,
     vrr_summary=False,
-    charges_summary=False,
-    convictions_summary=False,
     append=False,
     window=None,
     force=False,
     no_update=False,
     now=False,
 ):
     """
@@ -544,50 +538,49 @@
         debug (bool, optional): Print verbose logs to console for developers
         overwrite (bool, optional): Overwrite existing files at output path
         no_write (bool, optional): Do not export to output path
         fetch (bool, optional): Retrieve case detail PDFs from Alacourt.com
         cID (str, optional): Customer ID on Alacourt.com
         uID (str, optional): User ID on Alacourt.com
         pwd (str, optional): Password on Alacourt.com
+        criminal_only (bool): Only fetch criminal cases
         qmax (int, optional): Maximum queries to conduct on Alacourt.com
         qskip (int, optional): Skip entries at top of query file
         pairs (str, optional): Path to AIS / Unique ID pairs for grouped table functions
         vrr_summary (bool, optional): Create voting rights summary from pairs
-        charges_summary (bool, optional): Create charges summary from pairs
-        convictions_summary (bool, optional): Create convictions summary from pairs
         append (bool, optional): Append one archive to another
-        window (None, optional): PySimpleGUI window element
+        window (None, optional): PySimpleGUI Window element
         force (bool, optional): Do not raise exceptions
         no_update (bool, optional): Do not mark input query when fetching cases
         now (bool, optional): Start Alacorder upon successful configuration
     """
     good = True
     outputs = None if no_write else outputs
     no_write = True if outputs == None else no_write
     found = 0
 
     if debug:
         sys.tracebacklimit = 10
         pl.Config.set_verbose(True)
         pl.Config.set_tbl_rows(100)
     else:
-        sys.tracebacklimit = 2
+        sys.tracebacklimit = 0
         pl.Config.set_verbose(False)
 
     # raise overwrite error
     if no_write:
         outputext = "none"
         existing_output = False
     elif os.path.isdir(outputs):
         outputext = "directory"
         existing_output = False
     elif os.path.isfile(outputs):
         if not overwrite and not append:
             error(
-                "Error: Existing file at output path.\nRepeat in overwrite mode to continue.",
+                "Existing file at output path. Repeat in overwrite mode.",
                 cf={"WINDOW": window, "FORCE": force},
             )
         outputext = os.path.splitext(outputs)[1]
         existing_output = True
     else:
         outputext = os.path.splitext(str(outputs))[1]
         existing_output = False
@@ -619,15 +612,15 @@
         ".parquet",
         ".json",
         ".csv",
         "none",
         "directory",
     ):
         error(
-            "Error: File extension not supported.\nRepeat with .xls, .xlsx, .parquet, .csv, or .json.",
+            "File extension not supported.\nRepeat with .xls, .xlsx, .parquet, .csv, or .json.",
             cf={"WINDOW": window, "FORCE": force},
         )
 
     if (  # raise no table selection
         support_multitable == False
         and archive == False
         and fetch == False
@@ -712,15 +705,18 @@
         error("Failed to determine input type.", cf={"WINDOW": window, "FORCE": force})
 
     if count == 0:
         count = found
     if count > found:
         count = found
     if found > count:
-        queue = queue[0:count]
+        if isinstance(queue, pl.dataframe.frame.DataFrame):
+            queue = queue.sample(count)
+        elif isinstance(queue, list):
+            queue = sample(queue, count)
 
     out = {
         "QUEUE": queue,
         "INPUTS": inputs,
         "NEEDTEXT": bool(not is_full_text),
         "INPUT_TYPE": itype,
         "FOUND": found,
@@ -730,22 +726,21 @@
         "SUPPORT_MULTITABLE": support_multitable,
         "SUPPORT_SINGLETABLE": support_singletable,
         "SUPPORT_ARCHIVE": support_archive,
         "TABLE": table,
         "ARCHIVE": archive,
         "PAIRS": pairs,
         "VRR_SUMMARY": vrr_summary,
-        "CHARGES_SUMMARY": charges_summary,
-        "CONVICTIONS_SUMMARY": convictions_summary,
         "APPEND": append,
         "NO_UPDATE": no_update,
         "FETCH": fetch,
         "ALA_CUSTOMER_ID": cID,
         "ALA_USER_ID": uID,
         "ALA_PASSWORD": pwd,
+        "CRIMINAL_ONLY": criminal_only,
         "FETCH_SKIP": qskip,
         "FETCH_MAX": qmax,
         "LOG": log,
         "NO_WRITE": no_write,
         "NO_PROMPT": no_prompt,
         "OVERWRITE": overwrite,
         "EXISTING_OUTPUT": existing_output,
@@ -984,20 +979,14 @@
         return ft
     elif cf["ARCHIVE"] == True:
         ar = archive(cf)
         return ar
     elif cf["VRR_SUMMARY"] == True and cf["PAIRS"]:
         vr = vrr_summary(cf)
         return vr
-    elif cf["CHARGES_SUMMARY"] == True and cf["PAIRS"]:
-        ch = charges_summary(cf)
-        return ch
-    elif cf["CONVICTIONS_SUMMARY"] == True and cf["PAIRS"]:
-        conv = convictions_summary(cf)
-        return cf
     elif (
         cf["TABLE"].lower() in ("charges", "disposition", "filing")
         and cf["SUPPORT_SINGLETABLE"]
     ):
         ch = charges(cf)
         return ch
     elif cf["TABLE"].lower() in ("cases", "caseinfo") and cf["SUPPORT_SINGLETABLE"]:
@@ -1100,31 +1089,31 @@
     if cf and inpath == "":
         inpath = cf["INPUTS"]
 
     if cf and outpath == "":
         outpath = cf["OUTPUT_PATH"]
 
     if not os.path.isfile(inpath) and not os.path.isfile(outpath):
-        error("Error: Invalid path.", cf=cf)
+        error("Invalid path.", cf=cf)
 
     inarc = read(inpath)
     outarc = read(outpath)
 
     try:
         inarc = inarc.select("AllPagesText", "Path", "Timestamp")
         outarc = outarc.select("AllPagesText", "Path", "Timestamp")
     except:
         try:
             dlog(inarc, outarc, cf=conf)
-            print("Warning: Could not find column Timestamp in archive.")
+            print("Warning! Could not find column Timestamp in archive.")
             inarc = inarc.select("AllPagesText", "Path")
             outarc = outarc.select("AllPagesText", "Path")
         except:
             dlog(inarc, outarc, cf=conf)
-            print("Warning: Could not find column Path in archive.")
+            print("Warning! Could not find column Path in archive.")
             inarc = inarc.select("AllPagesText")
             outarc = outarc.select("AllPagesText")
 
     out = pl.concat([inarc, outarc])
 
     if window:
         window.write_event_value("COMPLETE-AA", True)
@@ -3151,14 +3140,15 @@
     querypath="",
     dirpath="",
     cID="",
     uID="",
     pwd="",
     qmax=0,
     qskip=0,
+    criminal_only=False,
     cf=None,
     no_update=False,
     debug=False,
     window=None,
 ):
     """
     Fetch case PDFs from Alacourt.com.
@@ -3178,23 +3168,25 @@
         querypath = cf["INPUTS"]
         dirpath = cf["OUTPUT_PATH"]
         cID = cf["ALA_CUSTOMER_ID"]
         uID = cf["ALA_USER_ID"]
         pwd = cf["ALA_PASSWORD"]
         qmax = cf["FETCH_MAX"]
         qskip = cf["FETCH_SKIP"]
+        criminal_only = cf["CRIMINAL_ONLY"]
     else:
         cf = {
             "INPUTS": querypath,
             "OUTPUT_PATH": dirpath,
             "ALA_CUSTOMER_ID": cID,
             "ALA_USER_ID": uID,
             "ALA_PASSWORD": pwd,
             "FETCH_MAX": qmax,
             "FETCH_SKIP": qskip,
+            "CRIMINAL_ONLY": criminal_only,
         }
 
     query = read_query(cf["INPUTS"], qmax=qmax, qskip=qskip)
 
     # start browser and authenticate
     opt = webdriver.ChromeOptions()
     opt.add_experimental_option(
@@ -3223,24 +3215,25 @@
             ssn=r["TEMP_SSN"],
             dob=r["TEMP_DOB"],
             county=r["TEMP_COUNTY"],
             division=r["TEMP_DIVISION"],
             case_year=r["TEMP_CASE_YEAR"],
             filed_before=r["TEMP_FILED_BEFORE"],
             filed_after=r["TEMP_FILED_AFTER"],
+            criminal_only=criminal_only,
             window=window,
         )
 
         if len(results) > 0:
             print(
                 f"#{i+1}/{query.shape[0]} {query[i, 'TEMP_NAME']} ({len(results)} records returned)"
             )
             if window:
                 window.write_event_value("PROGRESS-TEXT", 0)
-                window.write_event_value("PROGRESS-TEXT-TOTAL", 100)
+                window.write_event_value("PROGRESS-TEXT-TOTAL", len(results))
                 for x, url in enumerate(results):
                     window.write_event_value("PROGRESS-TEXT", x + 1)
                     downloadPDF(driver, url)
             else:
                 for x, url in enumerate(tqdm(results)):
                     downloadPDF(driver, url)
             query[i, "CASES_FOUND"] = len(results)
@@ -3297,14 +3290,15 @@
     case_year="",
     filed_before="",
     filed_after="",
     debug=False,
     cID="",
     uID="",
     pwd="",
+    criminal_only=False,
     window=None,
 ):
     """
     Collect PDFs via SJIS Party Search Form from Alacourt.com
     Returns list of URLs for downloadPDF() to download
 
     Args:
@@ -3327,90 +3321,100 @@
              "MC - MUNICIPAL-CRIMINAL"
              "TP - MUNICIPAL-PARKING"
              "SM - SMALL CLAIMS"
              "TR - TRAFFIC"
         case_year (str, optional): YYYY
         filed_before (str, optional): M/DD/YYYY
         filed_after (str, optional): M/DD/YYYY
+        cID (str): Customer ID on Alacourt.com
+        uID (str): User ID on Alacourt.com
+        pwd (str): Password on Alacourt.com
+        criminal_only (bool, optional): Only search criminal cases
         debug (bool, optional): Print detailed logs.
-        cID (str, optional): Customer ID on Alacourt.com
-        uID (str, optional): User ID on Alacourt.com
-        pwd (str, optional): Password on Alacourt.com
 
     Returns:
         List[str] of URLs to PDF
     """
 
     if "frmIndexSearchForm" not in driver.current_url:
         driver.get("https://v2.alacourt.com/frmIndexSearchForm.aspx")
 
-    driver.implicitly_wait(5)
-
+    driver.implicitly_wait(2)
     has_window = False if window == "None" else True
 
     # connection error
     try:
         party_name_box = driver.find_element(
             by=By.NAME, value="ctl00$ContentPlaceHolder1$txtName"
         )
     except selenium.common.exceptions.NoSuchElementException:
-        if debug:
-            print(
-                """NoSuchElementException on alac.py 2173: party_name_box = driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$txtName")"""
-            )
+        dlog(
+            """NoSuchElementException on `party_name_box = driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$txtName")`""",
+            cf=debug,
+        )
         if driver.current_url == "https://v2.alacourt.com/frmlogin.aspx":
-            time.sleep(10)
+            time.sleep(2)
             login(driver, cID=cID, uID=uID, pwd=pwd)
             driver.implicitly_wait(1)
         driver.get("https:v2.alacourt.com/frmIndexSearchForm.aspx")
         print("Successfully connected and logged into Alacourt!")
 
     # field search
+
+    # name
     if name != "":
         party_name_box.send_keys(name)
+    # ssn
     if ssn != "":
         ssn_box = driver.find_element(
             by=By.NAME, value="ctl00$ContentPlaceHolder1$txtSSN"
         )
         ssn_box.send_keys(ssn)
+    # dob
     if dob != "":
         date_of_birth_box = driver.find_element(
             by=By.NAME, value="ctl00$ContentPlaceHolder1$txtDOB"
         )
         date_of_birth_box.send_keys(dob)
-    if party_type != "":
-        party_type_select = driver.find_element(
-            by=By.NAME, value="ctl00$ContentPlaceHolder1$rdlPartyType"
-        )
-        pts = Select(party_type_select)
-        if party_type == "plaintiffs":
-            pts.select_by_visible_text("Plaintiffs")
-        if party_type == "defendants":
-            pts.select_by_visible_text("Defendants")
-        if party_type == "all":
-            pts.select_by_visible_text("ALL")
-
-    if county != "":
-        county_select = driver.find_element(
-            by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlCounties"
-        )
-        scounty = Select(county_select)
-        scounty.select_by_visible_text(county)
-    if division != "":
-        division_select = driver.find_element(
-            by=By.NAME, value="ctl00$ContentPlaceHolder1$UcddlDivisions1$ddlDivision"
-        )
-        sdivision = Select(division_select)
-        sdivision.select_by_visible_text(division)
-    if case_year != "":
+    # party type
+    if party_type == "Plaintiffs":
+        driver.find_element(
+            by=By.ID, value="ContentPlaceHolder1_rdlPartyType_0"
+        ).click()
+    if party_type == "Defendants":
+        driver.find_element(
+            by=By.ID, value="ContentPlaceHolder1_rdlPartyType_1"
+        ).click()
+    if party_type == "ALL":
+        driver.find_element(
+            by=By.ID, value="ContentPlaceHolder1_rdlPartyType_2"
+        ).click()
+    # division
+    if division == "" and not criminal_only:
+        division = "All Divisions"
+    if criminal_only:
+        division = "Criminal Only"
+    division_select = driver.find_element(
+        by=By.ID, value="ContentPlaceHolder1_UcddlDivisions1_ddlDivision"
+    )
+    sdivision = Select(division_select)
+    sdivision.select_by_visible_text(division)
+    if county == "":
+        county = "Statewide Search"
+    county_select = driver.find_element(
+        by=By.ID, value="ContentPlaceHolder1_ddlCounties"
+    )
+    scounty = Select(county_select)
+    scounty.select_by_visible_text(county)
+    if case_year != "" and case_year != None:
         case_year_select = driver.find_element(
             by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlCaseYear"
         )
         scase_year = Select(case_year_select)
-        scase_year.select_by_visible_text(case_year)
+        scase_year.select_by_visible_text(str(case_year))
     no_records_select = driver.find_element(
         by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlNumberOfRecords"
     )
     sno_records = Select(no_records_select)
     sno_records.select_by_visible_text("1000")
     if filed_before != "":
         filed_before_box = driver.find_element(
@@ -3420,15 +3424,14 @@
     if filed_after != "":
         filed_after_box = driver.find_element(
             by=By.NAME, value="ctl00$ContentPlaceHolder1$txtTo"
         )
         filed_after_box.send_keys(filed_after)
 
     driver.implicitly_wait(1)
-
     # submit search
     search_button = driver.find_element(by=By.ID, value="searchButton")
 
     driver.implicitly_wait(1)
     try:
         search_button.click()
     except:
@@ -3723,42 +3726,43 @@
                 button_text="New Query",
                 button_color=("white", "black"),
                 k="NEWQUERY",
                 enable_events=True,
             ),
         ],
         [
-            sg.Text("Output Path: "),
+            sg.Text("Output Directory: "),
             sg.InputText(
                 tooltip="PDF download destination folder",
-                size=[29, 10],
+                size=[26, 10],
                 key="SQ-OUTPUTPATH",
             ),
             sg.FolderBrowse(
                 button_text="Select Folder", button_color=("white", "black")
             ),
         ],
         [
             sg.Text("Max queries: "),
             sg.Input(key="SQ-MAX", default_text="0", size=[5, 1]),
             sg.Text("Skip from top: "),
             sg.Input(key="SQ-SKIP", default_text="0", size=[5, 1]),
+            sg.Checkbox(key="SQ-CRIMINALONLY", text="Criminal Only"),
         ],
         [sg.Text("Alacourt.com Credentials", font=BODY_FONT)],
         [
-            sg.Text("Customer ID:"),
-            sg.Input(key="SQ-CUSTOMERID", size=(13, 1)),
+            sg.Text("Customer ID: "),
+            sg.Input(key="SQ-CUSTOMERID", size=(16, 1)),
         ],
         [
             sg.Text("User ID:"),
-            sg.Input(key="SQ-USERID", size=(13, 1)),
+            sg.Input(key="SQ-USERID", size=(20, 1)),
         ],
         [
-            sg.Text("Password:"),
-            sg.InputText(key="SQ-PASSWORD", password_char="*", size=(15, 1)),
+            sg.Text("Password: "),
+            sg.InputText(key="SQ-PASSWORD", password_char="*", size=(18, 1)),
         ],
         [
             sg.Button(
                 "Start Query",
                 key="SQ",
                 button_color=("white", "black"),
                 pad=(10, 10),
@@ -3798,27 +3802,26 @@
             sg.InputText(
                 tooltip="Output archive file path (.parquet, .json, .csv)",
                 size=[39, 1],
                 key="MA-OUTPUTPATH",
             ),
         ],
         [
-            sg.Text("Skip Cases From: "),
+            sg.Text("Skip Cases From:  "),
             sg.Input(
                 tooltip="Skip all input cases found in PDF directory or archive (.parquet, .json, .csv)",
                 key="MA-SKIP",
-                size=[24, 1],
+                size=[36, 1],
                 pad=(0, 10),
             ),
         ],
         [
             sg.Text("Max cases: "),
             sg.Input(key="MA-COUNT", default_text="0", size=[5, 1]),
             sg.Checkbox("Allow Overwrite", default=True, key="MA-OVERWRITE"),
-            sg.Checkbox("Try to Append", key="MA-APPEND", default=False),
         ],
         [
             sg.Button(
                 "Make Archive",
                 button_color=("white", "black"),
                 key="MA",
                 enable_events=True,
@@ -3871,22 +3874,22 @@
                 bind_return_key=True,
             )
         ],
     ]  # "AA"
     sum_layout = [
         [
             sg.Text(
-                """Pair cases by AIS number to create a\npaired summary table.""",
+                """Pair cases by AIS number to create a\npaired voting rights summary table.""",
                 font=HEADER_FONT,
                 pad=(5, 5),
             )
         ],
         [
             sg.Text(
-                """To make a voting rights summary table, start by creating an AIS / Unique ID\npair template, fill the template with AIS numbers or another\nidentifier to match names in common, then enter the template path and\ncase input path below.""",
+                """To make a voting rights summary table, start by creating an AIS / Unique ID\npair template, fill the template with AIS numbers or another identifier\nto match names in common, then enter the template path and case\ninput path below.""",
                 pad=(5, 5),
             )
         ],
         [
             sg.Text("Input Path:  "),
             sg.InputText(
                 tooltip="PDF Directory or full text archive (.parquet, .json, .csv)",
@@ -3912,14 +3915,15 @@
             sg.InputText(
                 tooltip="PDF Directory or full text archive (.parquet, .json, .csv)",
                 size=[40, 10],
                 key="SUM-OUTPUTPATH",
                 focus=True,
             ),
         ],
+        [sg.Checkbox("Allow Overwrite", default=True, key="SUM-OVERWRITE")],
         [
             sg.Button(
                 "Create Summary",
                 key="SUM",
                 button_color=("white", "black"),
                 pad=(10, 10),
                 disabled_button_color=("grey", "black"),
@@ -3938,15 +3942,15 @@
         [
             sg.Text(
                 """Alacorder processes case detail PDFs and case text archives into data\ntables suitable for research purposes. Enter PDF directory or case text\narchive path and output file path (.xlsx, .xls, .csv, .json) to begin. CSV\nand JSON support single table selection only.""",
                 pad=(5, 5),
             )
         ],
         [
-            sg.Text("Input Path: "),
+            sg.Text("Input Path:  "),
             sg.InputText(
                 tooltip="PDF directory or full text archive (.parquet, .json, .csv)",
                 size=[28, 10],
                 key="TB-INPUTPATH",
                 focus=True,
             ),
             sg.FolderBrowse(
@@ -4006,15 +4010,15 @@
                 """Rename case PDFs in directory to\ncase numbers.""",
                 font=HEADER_FONT,
                 pad=(5, 5),
             )
         ],
         [
             sg.Text(
-                """To rename each PDF case in a directory to its case number, enter the\ndirectory path below and click start. Some devices may require a\nreboot or reindex to reflect updated file names.""",
+                """To rename each PDF case in a directory to its case number, enter the\ndirectory path below and click start. Some devices may require a\nreboot or reindex to reflect updated file names. Duplicate cases will\nbe removed.""",
                 pad=(5, 5),
             )
         ],
         [
             sg.Text("Directory: "),
             sg.InputText(
                 tooltip="PDF Directory",
@@ -4156,29 +4160,29 @@
         elif event == "MT":
             cf = set(
                 window["SUM-INPUTPATH"].get(),
                 window["SUM-PAIRS"].get(),
                 pairs=window["SUM-PAIRS"].get(),
                 log=True,
                 no_write=False,
-                overwrite=True,
+                overwrite=window["SUM-OVERWRITE"].get(),
                 window=window,
             )
             thread = threading.Thread(target=pairs, args=[cf], daemon=True).start()
             print("Creating AIS / Unique ID pairs template...")
             window["MT"].update(disabled=True)
         elif event == "SUM":
             cf = set(
                 window["SUM-INPUTPATH"].get(),
                 window["SUM-OUTPUTPATH"].get(),
                 pairs=window["SUM-PAIRS"].get(),
                 vrr_summary=True,
                 log=True,
                 no_write=False,
-                overwrite=True,
+                overwrite=window["SUM-OVERWRITE"].get(),
                 window=window,
             )
             print("Making voting rights summary table...")
             thread = threading.Thread(
                 target=vrr_summary, args=[cf], daemon=True
             ).start()
             window["SUM"].update(disabled=True)
@@ -4235,15 +4239,14 @@
                 cf = set(
                     window["MA-INPUTPATH"].get(),
                     window["MA-OUTPUTPATH"].get(),
                     count=count,
                     archive=True,
                     log=True,
                     overwrite=window["MA-OVERWRITE"].get(),
-                    append=window["MA-APPEND"].get(),
                     no_prompt=True,
                     window=window,
                 )
             except:
                 sg.popup("Check configuration and try again.")
                 window["MA"].update(disabled=False)
                 continue
@@ -4259,14 +4262,15 @@
             continue
         elif event == "SQ":
             if (
                 window["SQ-INPUTPATH"].get() == ""
                 or window["SQ-OUTPUTPATH"].get() == ""
             ):
                 sg.popup("Check configuration and try again.")
+                continue
             try:
                 pwd = window["SQ-PASSWORD"].get()
                 try:
                     sq_max = int(window["SQ-MAX"].get().strip())
                     sq_skip = int(window["SQ-SKIP"].get().strip())
                 except:
                     sq_max = 0
@@ -4278,14 +4282,15 @@
                         window["SQ-INPUTPATH"].get(),
                         window["SQ-OUTPUTPATH"].get(),
                         window["SQ-CUSTOMERID"].get(),
                         window["SQ-USERID"].get(),
                         pwd,
                         sq_max,
                         sq_skip,
+                        window["SQ-CRIMINALONLY"].get(),
                         None,
                         False,
                         False,
                         window,
                     ),
                     daemon=True,
                 ).start()
@@ -4439,14 +4444,21 @@
     "pwd",
     required=True,
     prompt="Alacourt Password",
     help="Password on Alacourt.com",
     hide_input=True,
 )
 @click.option(
+    "--criminal-only",
+    "-criminal",
+    is_flag=True,
+    default=False,
+    help="Only search criminal cases",
+)
+@click.option(
     "--max",
     "-max",
     "qmax",
     required=False,
     type=int,
     help="Maximum queries to conduct on Alacourt.com",
     default=0,
@@ -4470,37 +4482,41 @@
 )
 @click.option(
     "--debug",
     is_flag=True,
     default=False,
     help="Print detailed runtime information to console",
 )
-def _cli_fetch(querypath, path, cID, uID, pwd, qmax, qskip, no_update, debug):
+def _cli_fetch(
+    querypath, path, cID, uID, pwd, qmax, qskip, no_update, criminal_only, debug
+):
     """
     Fetch case PDFs from Alacourt.com.
     Args:
         querypath (str): Path to query table/spreadsheet (.xls, .xlsx)
         path (str): Path to PDF output directory
         cID (str): Customer ID on Alacourt.com
         uID (str): User ID on Alacourt.com
         pwd (str): Password on Alacourt.com
         qmax (int): Maximum queries to conduct on Alacourt.com
         qskip (int): Skip entries at top of query file
         no_update (bool): Do not update query template after completion
+        criminal_only (bool): Only search criminal cases
         debug (bool): Print detailed runtime information to console
     """
     fetch(
         querypath=querypath,
         dirpath=path,
         cID=cID,
         uID=uID,
         pwd=pwd,
         qmax=qmax,
         qskip=qskip,
         no_update=no_update,
+        criminal_only=criminal_only,
         debug=debug,
     )
 
 
 @main.command(name="multi", help="Export all data tables to .xls/.xlsx")
 @click.option(
     "--input-path",
@@ -5567,21 +5583,14 @@
     "-o",
     default=False,
     help="Overwrite existing files at output path",
     is_flag=True,
     show_default=False,
 )
 @click.option(
-    "--append",
-    "-a",
-    default=False,
-    is_flag=True,
-    help="Attempt to append to existing file at output path",
-)
-@click.option(
     "--no-log",
     default=False,
     is_flag=True,
     help="Do not print logs to console",
 )
 @click.option(
     "--no-prompt",
@@ -5592,30 +5601,30 @@
 @click.option(
     "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
 @click.version_option(
     package_name=name.lower(), prog_name=name.upper(), message="%(prog)s %(version)s"
 )
 def _cli_archive(
-    input_path, output_path, count, overwrite, append, no_log, no_prompt, debug
+    input_path, output_path, count, overwrite, no_log, no_prompt, debug
 ):
     """
     Write a full text archive from a directory of case detail PDFs.
 
     Args:
         input_path (str): PDF directory or archive input
         output_path (str): Path to archive output
         count (int): Total cases to pull from input
         overwrite (bool): Overwrite existing files at output path
-        append (bool): Attempt to append to existing file at output path
         no_write (bool): Do not export to output path
         no_prompt (bool): Skip user input / confirmation prompts
         debug (bool): Print verbose logs to console for developers
     """
     log = not no_log
+    sys.tracebacklimit = 0
     cf = set(
         input_path,
         output_path,
         archive=True,
         count=count,
         overwrite=overwrite,
         no_write=False,
@@ -5634,15 +5643,15 @@
     "--input-path",
     "-in",
     "input_path",
     required=True,
     type=click.Path(),
     prompt="PDF directory",
 )
-def cli_rename(input_path):
+def _cli_rename(input_path):
     c = cf(input_path, log=True)
     rename_pdfs(c)
 
 
 @main.command(
     name="pair",
     help="Create blank AIS / unique pairing template",
```

### Comparing `alacorder-80.3.7/src/alacorder/alac.py` & `alacorder-80.3.8/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.3.7"
+version = "80.3.8"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
 from datetime import datetime
+from random import sample
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import Select
 from selenium.webdriver.chrome.options import Options
 
 
 #   #   #   #                LOGS                #   #   #   #
@@ -432,16 +433,14 @@
     cID="",
     uID="",
     pwd="",
     qmax=0,
     qskip=0,
     pairs=None,
     vrr_summary=False,
-    charges_summary=False,
-    convictions_summary=False,
     append=False,
     window=None,
     force=False,
     no_update=False,
     now=False,
 ):
     """
@@ -462,16 +461,14 @@
         cID (str, optional): Customer ID on Alacourt.com
         uID (str, optional): User ID on Alacourt.com
         pwd (str, optional): Password on Alacourt.com
         qmax (int, optional): Maximum queries to conduct on Alacourt.com
         qskip (int, optional): Skip entries at top of query file
         pairs (str, optional): Path to AIS / Unique ID pairs for grouped table functions
         vrr_summary (bool, optional): Create voting rights summary from pairs
-        charges_summary (bool, optional): Create charges summary from pairs
-        convictions_summary (bool, optional): Create convictions summary from pairs
         append (bool, optional): Append one archive to another
         window (None, optional): PySimpleGUI window element
         force (bool, optional): Do not raise exceptions
         no_update (bool, optional): Do not mark input query when fetching cases
         now (bool, optional): Start Alacorder upon successful configuration
     """
     return cf(
@@ -489,16 +486,14 @@
         cID=cID,
         uID=uID,
         pwd=pwd,
         qmax=qmax,
         qskip=qskip,
         pairs=pairs,
         vrr_summary=vrr_summary,
-        charges_summary=charges_summary,
-        convictions_summary=convictions_summary,
         append=append,
         window=window,
         force=force,
         no_update=no_update,
         now=now,
     )
 
@@ -516,18 +511,17 @@
     no_write=False,
     fetch=False,
     cID="",
     uID="",
     pwd="",
     qmax=0,
     qskip=0,
+    criminal_only=False,
     pairs=None,
     vrr_summary=False,
-    charges_summary=False,
-    convictions_summary=False,
     append=False,
     window=None,
     force=False,
     no_update=False,
     now=False,
 ):
     """
@@ -544,50 +538,49 @@
         debug (bool, optional): Print verbose logs to console for developers
         overwrite (bool, optional): Overwrite existing files at output path
         no_write (bool, optional): Do not export to output path
         fetch (bool, optional): Retrieve case detail PDFs from Alacourt.com
         cID (str, optional): Customer ID on Alacourt.com
         uID (str, optional): User ID on Alacourt.com
         pwd (str, optional): Password on Alacourt.com
+        criminal_only (bool): Only fetch criminal cases
         qmax (int, optional): Maximum queries to conduct on Alacourt.com
         qskip (int, optional): Skip entries at top of query file
         pairs (str, optional): Path to AIS / Unique ID pairs for grouped table functions
         vrr_summary (bool, optional): Create voting rights summary from pairs
-        charges_summary (bool, optional): Create charges summary from pairs
-        convictions_summary (bool, optional): Create convictions summary from pairs
         append (bool, optional): Append one archive to another
-        window (None, optional): PySimpleGUI window element
+        window (None, optional): PySimpleGUI Window element
         force (bool, optional): Do not raise exceptions
         no_update (bool, optional): Do not mark input query when fetching cases
         now (bool, optional): Start Alacorder upon successful configuration
     """
     good = True
     outputs = None if no_write else outputs
     no_write = True if outputs == None else no_write
     found = 0
 
     if debug:
         sys.tracebacklimit = 10
         pl.Config.set_verbose(True)
         pl.Config.set_tbl_rows(100)
     else:
-        sys.tracebacklimit = 2
+        sys.tracebacklimit = 0
         pl.Config.set_verbose(False)
 
     # raise overwrite error
     if no_write:
         outputext = "none"
         existing_output = False
     elif os.path.isdir(outputs):
         outputext = "directory"
         existing_output = False
     elif os.path.isfile(outputs):
         if not overwrite and not append:
             error(
-                "Error: Existing file at output path.\nRepeat in overwrite mode to continue.",
+                "Existing file at output path. Repeat in overwrite mode.",
                 cf={"WINDOW": window, "FORCE": force},
             )
         outputext = os.path.splitext(outputs)[1]
         existing_output = True
     else:
         outputext = os.path.splitext(str(outputs))[1]
         existing_output = False
@@ -619,15 +612,15 @@
         ".parquet",
         ".json",
         ".csv",
         "none",
         "directory",
     ):
         error(
-            "Error: File extension not supported.\nRepeat with .xls, .xlsx, .parquet, .csv, or .json.",
+            "File extension not supported.\nRepeat with .xls, .xlsx, .parquet, .csv, or .json.",
             cf={"WINDOW": window, "FORCE": force},
         )
 
     if (  # raise no table selection
         support_multitable == False
         and archive == False
         and fetch == False
@@ -712,15 +705,18 @@
         error("Failed to determine input type.", cf={"WINDOW": window, "FORCE": force})
 
     if count == 0:
         count = found
     if count > found:
         count = found
     if found > count:
-        queue = queue[0:count]
+        if isinstance(queue, pl.dataframe.frame.DataFrame):
+            queue = queue.sample(count)
+        elif isinstance(queue, list):
+            queue = sample(queue, count)
 
     out = {
         "QUEUE": queue,
         "INPUTS": inputs,
         "NEEDTEXT": bool(not is_full_text),
         "INPUT_TYPE": itype,
         "FOUND": found,
@@ -730,22 +726,21 @@
         "SUPPORT_MULTITABLE": support_multitable,
         "SUPPORT_SINGLETABLE": support_singletable,
         "SUPPORT_ARCHIVE": support_archive,
         "TABLE": table,
         "ARCHIVE": archive,
         "PAIRS": pairs,
         "VRR_SUMMARY": vrr_summary,
-        "CHARGES_SUMMARY": charges_summary,
-        "CONVICTIONS_SUMMARY": convictions_summary,
         "APPEND": append,
         "NO_UPDATE": no_update,
         "FETCH": fetch,
         "ALA_CUSTOMER_ID": cID,
         "ALA_USER_ID": uID,
         "ALA_PASSWORD": pwd,
+        "CRIMINAL_ONLY": criminal_only,
         "FETCH_SKIP": qskip,
         "FETCH_MAX": qmax,
         "LOG": log,
         "NO_WRITE": no_write,
         "NO_PROMPT": no_prompt,
         "OVERWRITE": overwrite,
         "EXISTING_OUTPUT": existing_output,
@@ -984,20 +979,14 @@
         return ft
     elif cf["ARCHIVE"] == True:
         ar = archive(cf)
         return ar
     elif cf["VRR_SUMMARY"] == True and cf["PAIRS"]:
         vr = vrr_summary(cf)
         return vr
-    elif cf["CHARGES_SUMMARY"] == True and cf["PAIRS"]:
-        ch = charges_summary(cf)
-        return ch
-    elif cf["CONVICTIONS_SUMMARY"] == True and cf["PAIRS"]:
-        conv = convictions_summary(cf)
-        return cf
     elif (
         cf["TABLE"].lower() in ("charges", "disposition", "filing")
         and cf["SUPPORT_SINGLETABLE"]
     ):
         ch = charges(cf)
         return ch
     elif cf["TABLE"].lower() in ("cases", "caseinfo") and cf["SUPPORT_SINGLETABLE"]:
@@ -1100,31 +1089,31 @@
     if cf and inpath == "":
         inpath = cf["INPUTS"]
 
     if cf and outpath == "":
         outpath = cf["OUTPUT_PATH"]
 
     if not os.path.isfile(inpath) and not os.path.isfile(outpath):
-        error("Error: Invalid path.", cf=cf)
+        error("Invalid path.", cf=cf)
 
     inarc = read(inpath)
     outarc = read(outpath)
 
     try:
         inarc = inarc.select("AllPagesText", "Path", "Timestamp")
         outarc = outarc.select("AllPagesText", "Path", "Timestamp")
     except:
         try:
             dlog(inarc, outarc, cf=conf)
-            print("Warning: Could not find column Timestamp in archive.")
+            print("Warning! Could not find column Timestamp in archive.")
             inarc = inarc.select("AllPagesText", "Path")
             outarc = outarc.select("AllPagesText", "Path")
         except:
             dlog(inarc, outarc, cf=conf)
-            print("Warning: Could not find column Path in archive.")
+            print("Warning! Could not find column Path in archive.")
             inarc = inarc.select("AllPagesText")
             outarc = outarc.select("AllPagesText")
 
     out = pl.concat([inarc, outarc])
 
     if window:
         window.write_event_value("COMPLETE-AA", True)
@@ -3151,14 +3140,15 @@
     querypath="",
     dirpath="",
     cID="",
     uID="",
     pwd="",
     qmax=0,
     qskip=0,
+    criminal_only=False,
     cf=None,
     no_update=False,
     debug=False,
     window=None,
 ):
     """
     Fetch case PDFs from Alacourt.com.
@@ -3178,23 +3168,25 @@
         querypath = cf["INPUTS"]
         dirpath = cf["OUTPUT_PATH"]
         cID = cf["ALA_CUSTOMER_ID"]
         uID = cf["ALA_USER_ID"]
         pwd = cf["ALA_PASSWORD"]
         qmax = cf["FETCH_MAX"]
         qskip = cf["FETCH_SKIP"]
+        criminal_only = cf["CRIMINAL_ONLY"]
     else:
         cf = {
             "INPUTS": querypath,
             "OUTPUT_PATH": dirpath,
             "ALA_CUSTOMER_ID": cID,
             "ALA_USER_ID": uID,
             "ALA_PASSWORD": pwd,
             "FETCH_MAX": qmax,
             "FETCH_SKIP": qskip,
+            "CRIMINAL_ONLY": criminal_only,
         }
 
     query = read_query(cf["INPUTS"], qmax=qmax, qskip=qskip)
 
     # start browser and authenticate
     opt = webdriver.ChromeOptions()
     opt.add_experimental_option(
@@ -3223,24 +3215,25 @@
             ssn=r["TEMP_SSN"],
             dob=r["TEMP_DOB"],
             county=r["TEMP_COUNTY"],
             division=r["TEMP_DIVISION"],
             case_year=r["TEMP_CASE_YEAR"],
             filed_before=r["TEMP_FILED_BEFORE"],
             filed_after=r["TEMP_FILED_AFTER"],
+            criminal_only=criminal_only,
             window=window,
         )
 
         if len(results) > 0:
             print(
                 f"#{i+1}/{query.shape[0]} {query[i, 'TEMP_NAME']} ({len(results)} records returned)"
             )
             if window:
                 window.write_event_value("PROGRESS-TEXT", 0)
-                window.write_event_value("PROGRESS-TEXT-TOTAL", 100)
+                window.write_event_value("PROGRESS-TEXT-TOTAL", len(results))
                 for x, url in enumerate(results):
                     window.write_event_value("PROGRESS-TEXT", x + 1)
                     downloadPDF(driver, url)
             else:
                 for x, url in enumerate(tqdm(results)):
                     downloadPDF(driver, url)
             query[i, "CASES_FOUND"] = len(results)
@@ -3297,14 +3290,15 @@
     case_year="",
     filed_before="",
     filed_after="",
     debug=False,
     cID="",
     uID="",
     pwd="",
+    criminal_only=False,
     window=None,
 ):
     """
     Collect PDFs via SJIS Party Search Form from Alacourt.com
     Returns list of URLs for downloadPDF() to download
 
     Args:
@@ -3327,90 +3321,100 @@
              "MC - MUNICIPAL-CRIMINAL"
              "TP - MUNICIPAL-PARKING"
              "SM - SMALL CLAIMS"
              "TR - TRAFFIC"
         case_year (str, optional): YYYY
         filed_before (str, optional): M/DD/YYYY
         filed_after (str, optional): M/DD/YYYY
+        cID (str): Customer ID on Alacourt.com
+        uID (str): User ID on Alacourt.com
+        pwd (str): Password on Alacourt.com
+        criminal_only (bool, optional): Only search criminal cases
         debug (bool, optional): Print detailed logs.
-        cID (str, optional): Customer ID on Alacourt.com
-        uID (str, optional): User ID on Alacourt.com
-        pwd (str, optional): Password on Alacourt.com
 
     Returns:
         List[str] of URLs to PDF
     """
 
     if "frmIndexSearchForm" not in driver.current_url:
         driver.get("https://v2.alacourt.com/frmIndexSearchForm.aspx")
 
-    driver.implicitly_wait(5)
-
+    driver.implicitly_wait(2)
     has_window = False if window == "None" else True
 
     # connection error
     try:
         party_name_box = driver.find_element(
             by=By.NAME, value="ctl00$ContentPlaceHolder1$txtName"
         )
     except selenium.common.exceptions.NoSuchElementException:
-        if debug:
-            print(
-                """NoSuchElementException on alac.py 2173: party_name_box = driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$txtName")"""
-            )
+        dlog(
+            """NoSuchElementException on `party_name_box = driver.find_element(by=By.NAME, value="ctl00$ContentPlaceHolder1$txtName")`""",
+            cf=debug,
+        )
         if driver.current_url == "https://v2.alacourt.com/frmlogin.aspx":
-            time.sleep(10)
+            time.sleep(2)
             login(driver, cID=cID, uID=uID, pwd=pwd)
             driver.implicitly_wait(1)
         driver.get("https:v2.alacourt.com/frmIndexSearchForm.aspx")
         print("Successfully connected and logged into Alacourt!")
 
     # field search
+
+    # name
     if name != "":
         party_name_box.send_keys(name)
+    # ssn
     if ssn != "":
         ssn_box = driver.find_element(
             by=By.NAME, value="ctl00$ContentPlaceHolder1$txtSSN"
         )
         ssn_box.send_keys(ssn)
+    # dob
     if dob != "":
         date_of_birth_box = driver.find_element(
             by=By.NAME, value="ctl00$ContentPlaceHolder1$txtDOB"
         )
         date_of_birth_box.send_keys(dob)
-    if party_type != "":
-        party_type_select = driver.find_element(
-            by=By.NAME, value="ctl00$ContentPlaceHolder1$rdlPartyType"
-        )
-        pts = Select(party_type_select)
-        if party_type == "plaintiffs":
-            pts.select_by_visible_text("Plaintiffs")
-        if party_type == "defendants":
-            pts.select_by_visible_text("Defendants")
-        if party_type == "all":
-            pts.select_by_visible_text("ALL")
-
-    if county != "":
-        county_select = driver.find_element(
-            by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlCounties"
-        )
-        scounty = Select(county_select)
-        scounty.select_by_visible_text(county)
-    if division != "":
-        division_select = driver.find_element(
-            by=By.NAME, value="ctl00$ContentPlaceHolder1$UcddlDivisions1$ddlDivision"
-        )
-        sdivision = Select(division_select)
-        sdivision.select_by_visible_text(division)
-    if case_year != "":
+    # party type
+    if party_type == "Plaintiffs":
+        driver.find_element(
+            by=By.ID, value="ContentPlaceHolder1_rdlPartyType_0"
+        ).click()
+    if party_type == "Defendants":
+        driver.find_element(
+            by=By.ID, value="ContentPlaceHolder1_rdlPartyType_1"
+        ).click()
+    if party_type == "ALL":
+        driver.find_element(
+            by=By.ID, value="ContentPlaceHolder1_rdlPartyType_2"
+        ).click()
+    # division
+    if division == "" and not criminal_only:
+        division = "All Divisions"
+    if criminal_only:
+        division = "Criminal Only"
+    division_select = driver.find_element(
+        by=By.ID, value="ContentPlaceHolder1_UcddlDivisions1_ddlDivision"
+    )
+    sdivision = Select(division_select)
+    sdivision.select_by_visible_text(division)
+    if county == "":
+        county = "Statewide Search"
+    county_select = driver.find_element(
+        by=By.ID, value="ContentPlaceHolder1_ddlCounties"
+    )
+    scounty = Select(county_select)
+    scounty.select_by_visible_text(county)
+    if case_year != "" and case_year != None:
         case_year_select = driver.find_element(
             by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlCaseYear"
         )
         scase_year = Select(case_year_select)
-        scase_year.select_by_visible_text(case_year)
+        scase_year.select_by_visible_text(str(case_year))
     no_records_select = driver.find_element(
         by=By.NAME, value="ctl00$ContentPlaceHolder1$ddlNumberOfRecords"
     )
     sno_records = Select(no_records_select)
     sno_records.select_by_visible_text("1000")
     if filed_before != "":
         filed_before_box = driver.find_element(
@@ -3420,15 +3424,14 @@
     if filed_after != "":
         filed_after_box = driver.find_element(
             by=By.NAME, value="ctl00$ContentPlaceHolder1$txtTo"
         )
         filed_after_box.send_keys(filed_after)
 
     driver.implicitly_wait(1)
-
     # submit search
     search_button = driver.find_element(by=By.ID, value="searchButton")
 
     driver.implicitly_wait(1)
     try:
         search_button.click()
     except:
@@ -3723,42 +3726,43 @@
                 button_text="New Query",
                 button_color=("white", "black"),
                 k="NEWQUERY",
                 enable_events=True,
             ),
         ],
         [
-            sg.Text("Output Path: "),
+            sg.Text("Output Directory: "),
             sg.InputText(
                 tooltip="PDF download destination folder",
-                size=[29, 10],
+                size=[26, 10],
                 key="SQ-OUTPUTPATH",
             ),
             sg.FolderBrowse(
                 button_text="Select Folder", button_color=("white", "black")
             ),
         ],
         [
             sg.Text("Max queries: "),
             sg.Input(key="SQ-MAX", default_text="0", size=[5, 1]),
             sg.Text("Skip from top: "),
             sg.Input(key="SQ-SKIP", default_text="0", size=[5, 1]),
+            sg.Checkbox(key="SQ-CRIMINALONLY", text="Criminal Only"),
         ],
         [sg.Text("Alacourt.com Credentials", font=BODY_FONT)],
         [
-            sg.Text("Customer ID:"),
-            sg.Input(key="SQ-CUSTOMERID", size=(13, 1)),
+            sg.Text("Customer ID: "),
+            sg.Input(key="SQ-CUSTOMERID", size=(16, 1)),
         ],
         [
             sg.Text("User ID:"),
-            sg.Input(key="SQ-USERID", size=(13, 1)),
+            sg.Input(key="SQ-USERID", size=(20, 1)),
         ],
         [
-            sg.Text("Password:"),
-            sg.InputText(key="SQ-PASSWORD", password_char="*", size=(15, 1)),
+            sg.Text("Password: "),
+            sg.InputText(key="SQ-PASSWORD", password_char="*", size=(18, 1)),
         ],
         [
             sg.Button(
                 "Start Query",
                 key="SQ",
                 button_color=("white", "black"),
                 pad=(10, 10),
@@ -3798,27 +3802,26 @@
             sg.InputText(
                 tooltip="Output archive file path (.parquet, .json, .csv)",
                 size=[39, 1],
                 key="MA-OUTPUTPATH",
             ),
         ],
         [
-            sg.Text("Skip Cases From: "),
+            sg.Text("Skip Cases From:  "),
             sg.Input(
                 tooltip="Skip all input cases found in PDF directory or archive (.parquet, .json, .csv)",
                 key="MA-SKIP",
-                size=[24, 1],
+                size=[36, 1],
                 pad=(0, 10),
             ),
         ],
         [
             sg.Text("Max cases: "),
             sg.Input(key="MA-COUNT", default_text="0", size=[5, 1]),
             sg.Checkbox("Allow Overwrite", default=True, key="MA-OVERWRITE"),
-            sg.Checkbox("Try to Append", key="MA-APPEND", default=False),
         ],
         [
             sg.Button(
                 "Make Archive",
                 button_color=("white", "black"),
                 key="MA",
                 enable_events=True,
@@ -3871,22 +3874,22 @@
                 bind_return_key=True,
             )
         ],
     ]  # "AA"
     sum_layout = [
         [
             sg.Text(
-                """Pair cases by AIS number to create a\npaired summary table.""",
+                """Pair cases by AIS number to create a\npaired voting rights summary table.""",
                 font=HEADER_FONT,
                 pad=(5, 5),
             )
         ],
         [
             sg.Text(
-                """To make a voting rights summary table, start by creating an AIS / Unique ID\npair template, fill the template with AIS numbers or another\nidentifier to match names in common, then enter the template path and\ncase input path below.""",
+                """To make a voting rights summary table, start by creating an AIS / Unique ID\npair template, fill the template with AIS numbers or another identifier\nto match names in common, then enter the template path and case\ninput path below.""",
                 pad=(5, 5),
             )
         ],
         [
             sg.Text("Input Path:  "),
             sg.InputText(
                 tooltip="PDF Directory or full text archive (.parquet, .json, .csv)",
@@ -3912,14 +3915,15 @@
             sg.InputText(
                 tooltip="PDF Directory or full text archive (.parquet, .json, .csv)",
                 size=[40, 10],
                 key="SUM-OUTPUTPATH",
                 focus=True,
             ),
         ],
+        [sg.Checkbox("Allow Overwrite", default=True, key="SUM-OVERWRITE")],
         [
             sg.Button(
                 "Create Summary",
                 key="SUM",
                 button_color=("white", "black"),
                 pad=(10, 10),
                 disabled_button_color=("grey", "black"),
@@ -3938,15 +3942,15 @@
         [
             sg.Text(
                 """Alacorder processes case detail PDFs and case text archives into data\ntables suitable for research purposes. Enter PDF directory or case text\narchive path and output file path (.xlsx, .xls, .csv, .json) to begin. CSV\nand JSON support single table selection only.""",
                 pad=(5, 5),
             )
         ],
         [
-            sg.Text("Input Path: "),
+            sg.Text("Input Path:  "),
             sg.InputText(
                 tooltip="PDF directory or full text archive (.parquet, .json, .csv)",
                 size=[28, 10],
                 key="TB-INPUTPATH",
                 focus=True,
             ),
             sg.FolderBrowse(
@@ -4006,15 +4010,15 @@
                 """Rename case PDFs in directory to\ncase numbers.""",
                 font=HEADER_FONT,
                 pad=(5, 5),
             )
         ],
         [
             sg.Text(
-                """To rename each PDF case in a directory to its case number, enter the\ndirectory path below and click start. Some devices may require a\nreboot or reindex to reflect updated file names.""",
+                """To rename each PDF case in a directory to its case number, enter the\ndirectory path below and click start. Some devices may require a\nreboot or reindex to reflect updated file names. Duplicate cases will\nbe removed.""",
                 pad=(5, 5),
             )
         ],
         [
             sg.Text("Directory: "),
             sg.InputText(
                 tooltip="PDF Directory",
@@ -4156,29 +4160,29 @@
         elif event == "MT":
             cf = set(
                 window["SUM-INPUTPATH"].get(),
                 window["SUM-PAIRS"].get(),
                 pairs=window["SUM-PAIRS"].get(),
                 log=True,
                 no_write=False,
-                overwrite=True,
+                overwrite=window["SUM-OVERWRITE"].get(),
                 window=window,
             )
             thread = threading.Thread(target=pairs, args=[cf], daemon=True).start()
             print("Creating AIS / Unique ID pairs template...")
             window["MT"].update(disabled=True)
         elif event == "SUM":
             cf = set(
                 window["SUM-INPUTPATH"].get(),
                 window["SUM-OUTPUTPATH"].get(),
                 pairs=window["SUM-PAIRS"].get(),
                 vrr_summary=True,
                 log=True,
                 no_write=False,
-                overwrite=True,
+                overwrite=window["SUM-OVERWRITE"].get(),
                 window=window,
             )
             print("Making voting rights summary table...")
             thread = threading.Thread(
                 target=vrr_summary, args=[cf], daemon=True
             ).start()
             window["SUM"].update(disabled=True)
@@ -4235,15 +4239,14 @@
                 cf = set(
                     window["MA-INPUTPATH"].get(),
                     window["MA-OUTPUTPATH"].get(),
                     count=count,
                     archive=True,
                     log=True,
                     overwrite=window["MA-OVERWRITE"].get(),
-                    append=window["MA-APPEND"].get(),
                     no_prompt=True,
                     window=window,
                 )
             except:
                 sg.popup("Check configuration and try again.")
                 window["MA"].update(disabled=False)
                 continue
@@ -4259,14 +4262,15 @@
             continue
         elif event == "SQ":
             if (
                 window["SQ-INPUTPATH"].get() == ""
                 or window["SQ-OUTPUTPATH"].get() == ""
             ):
                 sg.popup("Check configuration and try again.")
+                continue
             try:
                 pwd = window["SQ-PASSWORD"].get()
                 try:
                     sq_max = int(window["SQ-MAX"].get().strip())
                     sq_skip = int(window["SQ-SKIP"].get().strip())
                 except:
                     sq_max = 0
@@ -4278,14 +4282,15 @@
                         window["SQ-INPUTPATH"].get(),
                         window["SQ-OUTPUTPATH"].get(),
                         window["SQ-CUSTOMERID"].get(),
                         window["SQ-USERID"].get(),
                         pwd,
                         sq_max,
                         sq_skip,
+                        window["SQ-CRIMINALONLY"].get(),
                         None,
                         False,
                         False,
                         window,
                     ),
                     daemon=True,
                 ).start()
@@ -4439,14 +4444,21 @@
     "pwd",
     required=True,
     prompt="Alacourt Password",
     help="Password on Alacourt.com",
     hide_input=True,
 )
 @click.option(
+    "--criminal-only",
+    "-criminal",
+    is_flag=True,
+    default=False,
+    help="Only search criminal cases",
+)
+@click.option(
     "--max",
     "-max",
     "qmax",
     required=False,
     type=int,
     help="Maximum queries to conduct on Alacourt.com",
     default=0,
@@ -4470,37 +4482,41 @@
 )
 @click.option(
     "--debug",
     is_flag=True,
     default=False,
     help="Print detailed runtime information to console",
 )
-def _cli_fetch(querypath, path, cID, uID, pwd, qmax, qskip, no_update, debug):
+def _cli_fetch(
+    querypath, path, cID, uID, pwd, qmax, qskip, no_update, criminal_only, debug
+):
     """
     Fetch case PDFs from Alacourt.com.
     Args:
         querypath (str): Path to query table/spreadsheet (.xls, .xlsx)
         path (str): Path to PDF output directory
         cID (str): Customer ID on Alacourt.com
         uID (str): User ID on Alacourt.com
         pwd (str): Password on Alacourt.com
         qmax (int): Maximum queries to conduct on Alacourt.com
         qskip (int): Skip entries at top of query file
         no_update (bool): Do not update query template after completion
+        criminal_only (bool): Only search criminal cases
         debug (bool): Print detailed runtime information to console
     """
     fetch(
         querypath=querypath,
         dirpath=path,
         cID=cID,
         uID=uID,
         pwd=pwd,
         qmax=qmax,
         qskip=qskip,
         no_update=no_update,
+        criminal_only=criminal_only,
         debug=debug,
     )
 
 
 @main.command(name="multi", help="Export all data tables to .xls/.xlsx")
 @click.option(
     "--input-path",
@@ -5567,21 +5583,14 @@
     "-o",
     default=False,
     help="Overwrite existing files at output path",
     is_flag=True,
     show_default=False,
 )
 @click.option(
-    "--append",
-    "-a",
-    default=False,
-    is_flag=True,
-    help="Attempt to append to existing file at output path",
-)
-@click.option(
     "--no-log",
     default=False,
     is_flag=True,
     help="Do not print logs to console",
 )
 @click.option(
     "--no-prompt",
@@ -5592,30 +5601,30 @@
 @click.option(
     "--debug", default=False, is_flag=True, help="Print verbose logs to console"
 )
 @click.version_option(
     package_name=name.lower(), prog_name=name.upper(), message="%(prog)s %(version)s"
 )
 def _cli_archive(
-    input_path, output_path, count, overwrite, append, no_log, no_prompt, debug
+    input_path, output_path, count, overwrite, no_log, no_prompt, debug
 ):
     """
     Write a full text archive from a directory of case detail PDFs.
 
     Args:
         input_path (str): PDF directory or archive input
         output_path (str): Path to archive output
         count (int): Total cases to pull from input
         overwrite (bool): Overwrite existing files at output path
-        append (bool): Attempt to append to existing file at output path
         no_write (bool): Do not export to output path
         no_prompt (bool): Skip user input / confirmation prompts
         debug (bool): Print verbose logs to console for developers
     """
     log = not no_log
+    sys.tracebacklimit = 0
     cf = set(
         input_path,
         output_path,
         archive=True,
         count=count,
         overwrite=overwrite,
         no_write=False,
@@ -5634,15 +5643,15 @@
     "--input-path",
     "-in",
     "input_path",
     required=True,
     type=click.Path(),
     prompt="PDF directory",
 )
-def cli_rename(input_path):
+def _cli_rename(input_path):
     c = cf(input_path, log=True)
     rename_pdfs(c)
 
 
 @main.command(
     name="pair",
     help="Create blank AIS / unique pairing template",
```

### Comparing `alacorder-80.3.7/PKG-INFO` & `alacorder-80.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.3.7
+Version: 80.3.8
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

