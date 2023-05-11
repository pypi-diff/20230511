# Comparing `tmp/datoso-0.2.7.tar.gz` & `tmp/datoso-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso-0.2.7.tar", last modified: Mon May  8 22:55:35 2023, max compression
+gzip compressed data, was "datoso-0.2.8.tar", last modified: Thu May 11 18:52:32 2023, max compression
```

## Comparing `datoso-0.2.7.tar` & `datoso-0.2.8.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.167677 datoso-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-08 22:55:23.000000 datoso-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-08 22:55:23.000000 datoso-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-08 22:55:35.167677 datoso-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-08 22:55:23.000000 datoso-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-08 22:55:23.000000 datoso-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-08 22:55:35.171677 datoso-0.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.159677 datoso-0.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.163677 datoso-0.2.7/src/datoso/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18809 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.167677 datoso-0.2.7/src/datoso/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/actions/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.167677 datoso-0.2.7/src/datoso/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/commands/doctor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/commands/seed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.167677 datoso-0.2.7/src/datoso/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/configuration/folder_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/configuration/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.167677 datoso-0.2.7/src/datoso/database/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.167677 datoso-0.2.7/src/datoso/database/models/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/database/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/database/models/datfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.167677 datoso-0.2.7/src/datoso/database/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/database/seeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/database/seeds/dat_repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/database/seeds/dat_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/datoso.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.167677 datoso-0.2.7/src/datoso/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/helpers/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/helpers/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.167677 datoso-0.2.7/src/datoso/repositories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/repositories/dat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/repositories/dedupe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.167677 datoso-0.2.7/src/datoso/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/seeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/seeds/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/seeds/unknown_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/seeds.txt
--rw-r--r--   0 runner    (1001) docker     (123)    42230 2023-05-08 22:55:23.000000 datoso-0.2.7/src/datoso/systems.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:55:35.167677 datoso-0.2.7/src/datoso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-08 22:55:35.000000 datoso-0.2.7/src/datoso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-08 22:55:35.000000 datoso-0.2.7/src/datoso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 22:55:35.000000 datoso-0.2.7/src/datoso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-08 22:55:35.000000 datoso-0.2.7/src/datoso.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-08 22:55:35.000000 datoso-0.2.7/src/datoso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 22:55:35.000000 datoso-0.2.7/src/datoso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:52:32.375929 datoso-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-11 18:52:18.000000 datoso-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-11 18:52:18.000000 datoso-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-11 18:52:32.375929 datoso-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-11 18:52:18.000000 datoso-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-11 18:52:18.000000 datoso-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-11 18:52:32.375929 datoso-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:52:32.367929 datoso-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:52:32.371929 datoso-0.2.8/src/datoso/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19183 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:52:32.371929 datoso-0.2.8/src/datoso/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/actions/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:52:32.371929 datoso-0.2.8/src/datoso/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/commands/doctor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/commands/seed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:52:32.375929 datoso-0.2.8/src/datoso/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/configuration/folder_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/configuration/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:52:32.375929 datoso-0.2.8/src/datoso/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:52:32.375929 datoso-0.2.8/src/datoso/database/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/database/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/database/models/datfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:52:32.375929 datoso-0.2.8/src/datoso/database/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/database/seeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/database/seeds/dat_repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/database/seeds/dat_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/datoso.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:52:32.375929 datoso-0.2.8/src/datoso/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/helpers/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/helpers/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:52:32.375929 datoso-0.2.8/src/datoso/repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/repositories/dat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/repositories/dedupe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:52:32.375929 datoso-0.2.8/src/datoso/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/seeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/seeds/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/seeds/unknown_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/seeds.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    42230 2023-05-11 18:52:18.000000 datoso-0.2.8/src/datoso/systems.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:52:32.371929 datoso-0.2.8/src/datoso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-11 18:52:32.000000 datoso-0.2.8/src/datoso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-11 18:52:32.000000 datoso-0.2.8/src/datoso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:52:32.000000 datoso-0.2.8/src/datoso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-11 18:52:32.000000 datoso-0.2.8/src/datoso.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-11 18:52:32.000000 datoso-0.2.8/src/datoso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 18:52:32.000000 datoso-0.2.8/src/datoso.egg-info/top_level.txt
```

### Comparing `datoso-0.2.7/LICENSE` & `datoso-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso-0.2.7/PKG-INFO` & `datoso-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso
 Keywords: emulators,roms
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `datoso-0.2.7/README.md` & `datoso-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `datoso-0.2.7/pyproject.toml` & `datoso-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datoso-0.2.7/src/datoso/__main__.py` & `datoso-0.2.8/src/datoso/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,27 +304,35 @@
             args.seed = seed
             command_seed(args)
         sys.exit(0)
     seed = Seed(name=args.seed)
     if getattr(args, 'details', False):
         command_seed_details(args)
     if getattr(args, 'fetch', False):
-        print(f'Fetching seed {Bcolors.OKGREEN}{args.seed}{Bcolors.ENDC}')
+        message = f'{Bcolors.OKCYAN}Fetching seed {Bcolors.OKGREEN}{args.seed}{Bcolors.ENDC}'
+        print('='*(len(message)-14))
+        print(message)
+        print('='*(len(message)-14))
         if seed.fetch():
             print(f'Errors fetching {Bcolors.FAIL}{args.seed}{Bcolors.ENDC}')
             print('Please enable logs for more information or use -v parameter')
             command_doctor(args)
+            sys.exit(1)
+        print(f'{Bcolors.OKBLUE}Finished fetching {Bcolors.OKGREEN}{args.seed}{Bcolors.ENDC}')
     if getattr(args, 'process', False):
-        print('=======================')
-        print(f'{Bcolors.OKCYAN}Processing seed {Bcolors.OKGREEN}{args.seed}{Bcolors.ENDC}')
-        print('=======================')
+        message = f'{Bcolors.OKCYAN}Processing seed {Bcolors.OKGREEN}{args.seed}{Bcolors.ENDC}'
+        print('='*(len(message)-14))
+        print(message)
+        print('='*(len(message)-14))
         if seed.process_dats(fltr=getattr(args, 'filter', None)):
             print(f'Errors processing {Bcolors.FAIL}{args.seed}{Bcolors.ENDC}')
             print('Please enable logs for more information or use -v parameter')
             command_doctor(args)
+            sys.exit(1)
+        print(f'{Bcolors.OKBLUE}Finished processing {Bcolors.OKGREEN}{args.seed}{Bcolors.ENDC}')
 
 
 def command_config_save(args) -> None:
     """ Save config to file """
     config_file = os.path.expanduser('~/.datosorc') if args.directory == '~' else os.path.join(os.getcwd(), '.datosorc')
     with open(config_file, 'w', encoding='utf-8') as file:
         config.write(file)
```

### Comparing `datoso-0.2.7/src/datoso/actions/processor.py` & `datoso-0.2.8/src/datoso/actions/processor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.7/src/datoso/commands/doctor.py` & `datoso-0.2.8/src/datoso/commands/doctor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.7/src/datoso/commands/seed.py` & `datoso-0.2.8/src/datoso/commands/seed.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,8 +80,7 @@
                 if output and not config.getboolean('COMMAND', 'Quiet', fallback=False):
                     line += str(output)+' '
                     print(output, end=' ', flush=True)
                 if output or config.getboolean('COMMAND', 'Verbose', fallback=False):
                     line = ''
                     print(line)
         delete_line(line)
-        print(f'{Bcolors.OKBLUE}Finished processing {Bcolors.OKGREEN}{self.name}{Bcolors.ENDC}')
```

### Comparing `datoso-0.2.7/src/datoso/configuration/folder_helper.py` & `datoso-0.2.8/src/datoso/configuration/folder_helper.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.7/src/datoso/configuration/logger.py` & `datoso-0.2.8/src/datoso/configuration/logger.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.7/src/datoso/database/__init__.py` & `datoso-0.2.8/src/datoso/database/__init__.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.7/src/datoso/database/models/datfile.py` & `datoso-0.2.8/src/datoso/database/models/datfile.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.7/src/datoso/database/seeds/dat_repos.py` & `datoso-0.2.8/src/datoso/database/seeds/dat_repos.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.7/src/datoso/database/seeds/dat_rules.py` & `datoso-0.2.8/src/datoso/database/seeds/dat_rules.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.7/src/datoso/datoso.ini` & `datoso-0.2.8/src/datoso/datoso.ini`

 * *Files identical despite different names*

### Comparing `datoso-0.2.7/src/datoso/helpers/__init__.py` & `datoso-0.2.8/src/datoso/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.7/src/datoso/helpers/executor.py` & `datoso-0.2.8/src/datoso/helpers/executor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.7/src/datoso/helpers/plugins.py` & `datoso-0.2.8/src/datoso/helpers/plugins.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.7/src/datoso/repositories/dat.py` & `datoso-0.2.8/src/datoso/repositories/dat.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,32 +102,41 @@
     header = None
     merged_roms = []
 
     def load(self) -> None:
         """ Load the data from a XML file. """
         with open(self.file, encoding='utf-8') as fild:
             self.data = xmltodict.parse(fild.read())
-            self.header = self.data['datafile']['header']
-            self.name = self.header['name'] if 'name' in self.header else None
-            self.full_name = self.header['description'] if 'description' in self.header else None
-            self.date = self.header['date'] if 'date' in self.header else None
-            self.homepage = self.header['homepage'] if 'homepage' in self.header and self.header['homepage'] and 'insert' not in self.header['homepage'] else None
-            self.url = self.header['url'] if 'url' in self.header and self.header['url'] and 'insert' not in self.header['url'] else None
-            self.author = self.header['author'] if 'author' in self.header and self.header['author'] and 'insert' not in self.header['author'] else None
-            self.email = self.header['email'] if 'email' in self.header and self.header['email'] and 'insert' not in self.header['email'] else None
+            self.detect_main_key()
+            self.header = self.data[self.main_key].get('header', {})
+            if self.header:
+                self.name = self.header['name'] if 'name' in self.header else None
+                self.full_name = self.header['description'] if 'description' in self.header else None
+                self.date = self.header['date'] if 'date' in self.header else None
+                self.homepage = self.header['homepage'] if 'homepage' in self.header and self.header['homepage'] and 'insert' not in self.header['homepage'] else None
+                self.url = self.header['url'] if 'url' in self.header and self.header['url'] and 'insert' not in self.header['url'] else None
+                self.author = self.header['author'] if 'author' in self.header and self.header['author'] and 'insert' not in self.header['author'] else None
+                self.email = self.header['email'] if 'email' in self.header and self.header['email'] and 'insert' not in self.header['email'] else None
+            else:
+                self.name = self.data[self.main_key].get('@name')
+                self.full_name = self.data[self.main_key].get('@description')
             self.detect_game_key()
 
     def save(self) -> None:
         """ Save the data to a XML file. """
         with open(self.file, 'w', encoding='utf-8') as fild:
             fild.write(xmltodict.unparse(self.data, pretty=True))
 
+    def detect_main_key(self) -> str:
+        """ Detect the main key for the dat file. """
+        self.main_key = next(iter(self.data))
+
     def detect_game_key(self) -> str:
         """ Get the game key. """
-        for key in self.data['datafile']:
+        for key in self.data[self.main_key]:
             if key != 'header' and not key.startswith('@'):
                 self.game_key = key
                 break
 
     def parse_rom(self, rom: dict) -> dict:
         """ Standarize the rom. """
         parsed_rom = {}
@@ -142,27 +151,27 @@
         """ Add a rom to the dat file. """
         self.shas.add_rom(self.parse_rom(rom))
 
     def get_rom_shas(self) -> None:
         """ Get the shas for the roms and creates an index. """
         self.shas = HashesIndex()
 
-        for game in self.data['datafile'][self.game_key]:
+        for game in self.data[self.main_key][self.game_key]:
             if 'rom' not in game:
                 continue
             if not isinstance(game['rom'], list):
                 self.add_rom(game['rom'])
             else:
                 for rom in game['rom']:
                     self.add_rom(rom)
 
     def merge_with(self, parent: DatFile) -> None:
         """ Merge the dat file with the parent. """
         parent.get_rom_shas()
-        for game in self.data['datafile'][self.game_key]:
+        for game in self.data[self.main_key][self.game_key]:
             if 'rom' not in game:
                 continue
             if not isinstance(game['rom'], list):
                 if parent.shas.has_rom(self.parse_rom(game['rom'])):
                     self.merged_roms.append(self.parse_rom(game['rom']))
                     del game['rom']
             else:
@@ -170,18 +179,18 @@
                 for rom in game['rom']:
                     if not parent.shas.has_rom(self.parse_rom(rom)):
                         new_roms.append(rom)
                     else:
                         self.merged_roms.append(self.parse_rom(rom))
                 game['rom'] = new_roms
         new_games = []
-        for game in self.data['datafile'][self.game_key]:
+        for game in self.data[self.main_key][self.game_key]:
             if 'rom' in game:
                 new_games.append(game)
-        self.data['datafile'][self.game_key] = new_games
+        self.data[self.main_key][self.game_key] = new_games
 
     def get_name(self) -> str:
         """ Get the name of the dat file. """
         if not self.name:
             self.load()
         return self.name
 
@@ -270,15 +279,15 @@
             self.header = self.read_block(block)
 
             while next_block:
                 block, next_block = self.get_next_block(next_block)
                 self.games.append(self.read_block(block))
 
         self.data = {
-            'datafile': {
+            self.main_key: {
                 'header':  self.header,
                 'game': self.games
             }
         }
         self.name = self.header['name']
         self.full_name = self.header['description']
 
@@ -294,15 +303,15 @@
 
     def load(self) -> None:
         """ Load the data from a ClrMamePro file. """
         self.games = []
         self.header = self.get_header()
 
         self.data = {
-            'datafile': {
+            self.main_key: {
                 'header':  self.header,
                 'game': self.games
             }
         }
         self.name = self.header['name']
         self.full_name = self.header['description']
 
@@ -320,15 +329,15 @@
                 self.games.append({ 'rom': { '@name': file } })
 
         self.name = os.path.basename(self.file)
 
         self.header = self.get_header()
 
         self.data = {
-            'datafile': {
+            self.main_key: {
                 'header':  self.header,
                 'game': self.games
             }
         }
         self.name = self.header['name']
         self.full_name = self.header['description']
```

### Comparing `datoso-0.2.7/src/datoso/repositories/dedupe.py` & `datoso-0.2.8/src/datoso/repositories/dedupe.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.7/src/datoso/seeds/unknown_seed.py` & `datoso-0.2.8/src/datoso/seeds/unknown_seed.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.7/src/datoso/seeds.txt` & `datoso-0.2.8/src/datoso/seeds.txt`

 * *Files identical despite different names*

### Comparing `datoso-0.2.7/src/datoso/systems.json` & `datoso-0.2.8/src/datoso/systems.json`

 * *Files identical despite different names*

### Comparing `datoso-0.2.7/src/datoso.egg-info/PKG-INFO` & `datoso-0.2.8/src/datoso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso
 Keywords: emulators,roms
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `datoso-0.2.7/src/datoso.egg-info/SOURCES.txt` & `datoso-0.2.8/src/datoso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datoso-0.2.7/src/datoso.egg-info/requires.txt` & `datoso-0.2.8/src/datoso.egg-info/requires.txt`

 * *Files identical despite different names*

