# Comparing `tmp/triplify_csv-0.3.0.tar.gz` & `tmp/triplify_csv-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triplify_csv-0.3.0.tar", max compression
+gzip compressed data, was "triplify_csv-0.4.0.tar", max compression
```

## Comparing `triplify_csv-0.3.0.tar` & `triplify_csv-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1526 2023-04-03 19:59:17.539697 triplify_csv-0.3.0/LICENSE
--rw-r--r--   0        0        0     7467 2023-05-07 09:13:43.889593 triplify_csv-0.3.0/README.md
--rw-r--r--   0        0        0      568 2023-05-07 09:36:22.549551 triplify_csv-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-03 19:59:17.546697 triplify_csv-0.3.0/triplify_csv/__init__.py
--rwxr-xr-x   0        0        0    17765 2023-04-30 07:29:04.624548 triplify_csv-0.3.0/triplify_csv/triplify_csv.py
--rw-r--r--   0        0        0     8264 1970-01-01 00:00:00.000000 triplify_csv-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1526 2023-04-03 19:59:17.539697 triplify_csv-0.4.0/LICENSE
+-rw-r--r--   0        0        0     7905 2023-05-11 07:35:24.158330 triplify_csv-0.4.0/README.md
+-rw-r--r--   0        0        0      568 2023-05-11 07:37:35.982325 triplify_csv-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-03 19:59:17.546697 triplify_csv-0.4.0/triplify_csv/__init__.py
+-rwxr-xr-x   0        0        0    18065 2023-05-10 17:33:25.481276 triplify_csv-0.4.0/triplify_csv/triplify_csv.py
+-rw-r--r--   0        0        0     8702 1970-01-01 00:00:00.000000 triplify_csv-0.4.0/PKG-INFO
```

### Comparing `triplify_csv-0.3.0/LICENSE` & `triplify_csv-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `triplify_csv-0.3.0/README.md` & `triplify_csv-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -159,8 +159,14 @@
 	    foaf:name "Joe Bloggs" .
 	
 	<http://example.com/Contact/30/Mr%20Bun> a foaf:Person ;
 	    ex:id 30 ;
 	    foaf:interest "https://en.m.wikipedia.org/wiki/Spam\_(food)" ;
 	    foaf:name "Mr Bun" .
 
- 
+If you wanted this serialised to json-ld format instead you could use the following command ...
+
+```
+triplify_csv -m 'contactsmap.ttl' -c 'Contacts.csv' -o 'contactstriples.json' -f 'json-ld'
+```
+
+ triplify_csv uses rdflib and can output to all the serialisation formats that [rdflib](https://pypi.org/project/rdflib/) provides. (See also 'format' [here](https://rdflib.readthedocs.io/en/stable/apidocs/rdflib.html#rdflib.Graph.serialize))
```

### Comparing `triplify_csv-0.3.0/pyproject.toml` & `triplify_csv-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "triplify_csv"
-version = "0.3.0"
+version = "0.4.0"
 description = "A tool to generate triples from CSV files according to a configuration file."
 authors = ["Adrian Atley"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/AAtley/triplify_csv"
 
 [tool.poetry.dependencies]
```

### Comparing `triplify_csv-0.3.0/triplify_csv/triplify_csv.py` & `triplify_csv-0.4.0/triplify_csv/triplify_csv.py`

 * *Files 3% similar despite different names*

```diff
@@ -482,30 +482,33 @@
               default=",")
 @click.option("--encoding", "-e",
               help="The input CSV's file encoding. Defaults to 'utf-8'.",
               default="utf-8")
 @click.option("--dateformat", "-d",
               help="If you have dates in your CSV files this describes the format they are in. See 'strptime format codes'. Defaults to '%Y-%m-%d', for example 2022-01-31.",     
               default="%Y-%m-%d")
-def process(mapfile, csvfile, outfile, separator=',', encoding='utf-8', dateformat='%Y-%m-%d'):
+@click.option("--format", "-f",
+              help='One of the inbuilt serialisation formats that RDFLIB supports, one of "xml", "n3", "turtle", "nt", "pretty-xml", "trix", "trig", "nquads", "json-ld" or "hext". Defaults to "n3".',     
+              default="n3")              
+def process(mapfile, csvfile, outfile, separator=',', encoding='utf-8', dateformat='%Y-%m-%d', format='n3'):
 	""" Generates triples or n-quads in outfile from one or more CSV files according to the configuration in the Triples Map configuration file. """
 	csvfiles = list(csvfile)
 	if not sys.stdin.isatty():
 		csvfiles.extend(list(sys.stdin))
 		
 	s = Rml()
 	
 	# take option defaults or those entered
 	options = CsvOptions(encoding = encoding, delimiter = separator, dateformat = dateformat)
 	
 	# load one rml and 1 or more csvs
 	s.loadFile(mapfile, csvfiles, options)
 	s.create_triples()
 	try:
-	    s.write_file(outfile)
+	    s.write_file(outfile, format)
 	except Exception as err:
 	    print("Error outputting graph: {0}".format(err))
 	    raise
 	for e in s.errors:
 		print(e)
```

### Comparing `triplify_csv-0.3.0/PKG-INFO` & `triplify_csv-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triplify-csv
-Version: 0.3.0
+Version: 0.4.0
 Summary: A tool to generate triples from CSV files according to a configuration file.
 Home-page: https://github.com/AAtley/triplify_csv
 License: BSD-3-Clause
 Author: Adrian Atley
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -179,8 +179,14 @@
 	    foaf:name "Joe Bloggs" .
 	
 	<http://example.com/Contact/30/Mr%20Bun> a foaf:Person ;
 	    ex:id 30 ;
 	    foaf:interest "https://en.m.wikipedia.org/wiki/Spam\_(food)" ;
 	    foaf:name "Mr Bun" .
 
- 
+If you wanted this serialised to json-ld format instead you could use the following command ...
+
+```
+triplify_csv -m 'contactsmap.ttl' -c 'Contacts.csv' -o 'contactstriples.json' -f 'json-ld'
+```
+
+ triplify_csv uses rdflib and can output to all the serialisation formats that [rdflib](https://pypi.org/project/rdflib/) provides. (See also 'format' [here](https://rdflib.readthedocs.io/en/stable/apidocs/rdflib.html#rdflib.Graph.serialize))
```

