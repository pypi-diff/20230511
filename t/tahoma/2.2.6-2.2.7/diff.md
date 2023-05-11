# Comparing `tmp/tahoma-2.2.6.tar.gz` & `tmp/tahoma-2.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahoma-2.2.6.tar", last modified: Sun May  7 16:50:58 2023, max compression
+gzip compressed data, was "tahoma-2.2.7.tar", last modified: Thu May 11 16:50:17 2023, max compression
```

## Comparing `tahoma-2.2.6.tar` & `tahoma-2.2.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-07 16:50:58.616933 tahoma-2.2.6/
--rwxrwx---   0 neptune   (1000) neptune   (1000)     1070 2023-02-18 00:22:37.000000 tahoma-2.2.6/LICENSE
--rwxrwx---   0 neptune   (1000) neptune   (1000)      142 2023-02-21 14:35:21.000000 tahoma-2.2.6/MANIFEST.in
--rwxrwx---   0 neptune   (1000) neptune   (1000)     6437 2023-05-07 16:50:58.617046 tahoma-2.2.6/PKG-INFO
--rwxrwx---   0 neptune   (1000) neptune   (1000)     5775 2023-05-07 16:40:31.000000 tahoma-2.2.6/PYPI_README.md
--rwxrwx---   0 neptune   (1000) neptune   (1000)     5753 2023-05-04 11:36:20.000000 tahoma-2.2.6/README.md
--rwxrwx---   0 neptune   (1000) neptune   (1000)     1201 2023-02-21 21:29:00.000000 tahoma-2.2.6/pyproject.toml
--rwxrwx---   0 neptune   (1000) neptune   (1000)       41 2023-02-21 17:24:01.000000 tahoma-2.2.6/requirements.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       38 2023-05-07 16:50:58.617379 tahoma-2.2.6/setup.cfg
--rwxrwx---   0 neptune   (1000) neptune   (1000)      125 2023-02-15 20:31:23.000000 tahoma-2.2.6/setup.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-07 16:50:58.611462 tahoma-2.2.6/tahoma/
--rwxrwx---   0 neptune   (1000) neptune   (1000)      134 2023-02-21 18:24:33.000000 tahoma-2.2.6/tahoma/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)       22 2023-05-07 16:41:10.000000 tahoma-2.2.6/tahoma/__version__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)     6121 2023-05-07 16:43:55.000000 tahoma-2.2.6/tahoma/get_devices_url.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-07 16:50:58.615305 tahoma-2.2.6/tahoma/icons/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.6/tahoma/icons/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)    21160 2023-02-15 08:39:56.000000 tahoma-2.2.6/tahoma/icons/connected_house.png
--rwxrwx---   0 neptune   (1000) neptune   (1000)    29722 2023-02-15 17:48:11.000000 tahoma-2.2.6/tahoma/icons/water heater.png
--rwxrwx---   0 neptune   (1000) neptune   (1000)    38624 2023-05-07 16:50:10.000000 tahoma-2.2.6/tahoma/tahoma.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-07 16:50:58.615824 tahoma-2.2.6/tahoma/temp/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:32:54.000000 tahoma-2.2.6/tahoma/temp/__init__.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-07 16:50:58.616627 tahoma-2.2.6/tahoma/test/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.6/tahoma/test/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2021-07-13 15:25:04.000000 tahoma-2.2.6/tahoma/test/test.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-07 16:50:58.613891 tahoma-2.2.6/tahoma.egg-info/
--rwxrwx---   0 neptune   (1000) neptune   (1000)     6437 2023-05-07 16:50:58.000000 tahoma-2.2.6/tahoma.egg-info/PKG-INFO
--rwxrwx---   0 neptune   (1000) neptune   (1000)      517 2023-05-07 16:50:58.000000 tahoma-2.2.6/tahoma.egg-info/SOURCES.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)        1 2023-05-07 16:50:58.000000 tahoma-2.2.6/tahoma.egg-info/dependency_links.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       46 2023-05-07 16:50:58.000000 tahoma-2.2.6/tahoma.egg-info/entry_points.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       41 2023-05-07 16:50:58.000000 tahoma-2.2.6/tahoma.egg-info/requires.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)        7 2023-05-07 16:50:58.000000 tahoma-2.2.6/tahoma.egg-info/top_level.txt
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-11 16:50:17.397825 tahoma-2.2.7/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     1070 2023-02-18 00:22:37.000000 tahoma-2.2.7/LICENSE
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      142 2023-02-21 14:35:21.000000 tahoma-2.2.7/MANIFEST.in
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     7051 2023-05-11 16:50:17.398305 tahoma-2.2.7/PKG-INFO
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     6389 2023-05-11 16:26:57.000000 tahoma-2.2.7/PYPI_README.md
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     6389 2023-05-11 16:26:53.000000 tahoma-2.2.7/README.md
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     1201 2023-02-21 21:29:00.000000 tahoma-2.2.7/pyproject.toml
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       41 2023-02-21 17:24:01.000000 tahoma-2.2.7/requirements.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       38 2023-05-11 16:50:17.399292 tahoma-2.2.7/setup.cfg
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      125 2023-02-15 20:31:23.000000 tahoma-2.2.7/setup.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-11 16:50:17.391061 tahoma-2.2.7/tahoma/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      134 2023-02-21 18:24:33.000000 tahoma-2.2.7/tahoma/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       22 2023-05-11 16:27:42.000000 tahoma-2.2.7/tahoma/__version__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    11266 2023-05-11 16:31:18.000000 tahoma-2.2.7/tahoma/get_devices_url.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-11 16:50:17.395556 tahoma-2.2.7/tahoma/icons/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.7/tahoma/icons/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    21160 2023-02-15 08:39:56.000000 tahoma-2.2.7/tahoma/icons/connected_house.png
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    29722 2023-02-15 17:48:11.000000 tahoma-2.2.7/tahoma/icons/water heater.png
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    42780 2023-05-11 16:43:54.000000 tahoma-2.2.7/tahoma/tahoma.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-11 16:50:17.396186 tahoma-2.2.7/tahoma/temp/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:32:54.000000 tahoma-2.2.7/tahoma/temp/__init__.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-11 16:50:17.397337 tahoma-2.2.7/tahoma/test/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.7/tahoma/test/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2021-07-13 15:25:04.000000 tahoma-2.2.7/tahoma/test/test.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-11 16:50:17.393964 tahoma-2.2.7/tahoma.egg-info/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     7051 2023-05-11 16:50:17.000000 tahoma-2.2.7/tahoma.egg-info/PKG-INFO
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      517 2023-05-11 16:50:17.000000 tahoma-2.2.7/tahoma.egg-info/SOURCES.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        1 2023-05-11 16:50:17.000000 tahoma-2.2.7/tahoma.egg-info/dependency_links.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       46 2023-05-11 16:50:17.000000 tahoma-2.2.7/tahoma.egg-info/entry_points.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       41 2023-05-11 16:50:17.000000 tahoma-2.2.7/tahoma.egg-info/requires.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        7 2023-05-11 16:50:17.000000 tahoma-2.2.7/tahoma.egg-info/top_level.txt
```

### Comparing `tahoma-2.2.6/LICENSE` & `tahoma-2.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.6/PKG-INFO` & `tahoma-2.2.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoma
-Version: 2.2.6
+Version: 2.2.7
 Summary: This is a very easy API for controlling Somfy Tahoma's devices written in Python3, thanks to the pyoverkiz API. You just need a three-word input to control a device
 Author-email: Pzim-devdata <contact@pzim.fr>
 Project-URL: Homepage, https://github.com/pzim-devdata/tahoma
 Project-URL: Bug Tracker, https://github.com/pzim-devdata/tahoma/issues
 Keywords: tahoma,somfy,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -101,25 +101,39 @@
 or
 - C:\foler\of\tahoma\tahoma.exe -g
 
 3. And now, you are ready to use tahoma :
 
 
 # Usage : 
+
 `tahoma [ACTION] [CATEGORY] [NAME]`
 
 
 For instance : `tahoma open shutter kitchen` or `tahoma ouvrir volet cuisine`
 
 You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
 
 You can also run many commands during the same process without restarting tahoma ;
 
 For instance : `tahoma arm alarm garden close shutter room6 confort heater dining off plug office 25 sunscreen kitchen launch scene morning`
 
+Exemples :
+
+- tahoma open shutter kitchen
+- tahoma 25 sunscreen Velux3 (You can close a shutter or a sunscreen to a specifique level. Here it will close to 25% )
+- tahoma get sensor ['Luminace sensor garden'] (Just for sensors : you can use the full name of the device with [''] )
+- tahoma on plug office
+- tahoma get sensor door
+- tahoma arm alarm garden
+- confort heater dining
+- tahoma get sensor ['heater dining room']
+- tahoma launch scene morning
+- tahoma arm alarm garden open shutter room6 confort heater dining off plug office 25 sunscreen kitchen launch scene morning get sensor ['heater dining room']
+
 
 # But first you need to retrieve your PERSONALS commands :
 
 
 ## Get a list of all possibles [ACTIONS] for each [CATEGORIES] : 
 
 Open a terminal and type :
```

### Comparing `tahoma-2.2.6/PYPI_README.md` & `tahoma-2.2.7/PYPI_README.md`

 * *Files 5% similar despite different names*

```diff
@@ -86,25 +86,39 @@
 or
 - C:\foler\of\tahoma\tahoma.exe -g
 
 3. And now, you are ready to use tahoma :
 
 
 # Usage : 
+
 `tahoma [ACTION] [CATEGORY] [NAME]`
 
 
 For instance : `tahoma open shutter kitchen` or `tahoma ouvrir volet cuisine`
 
 You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
 
 You can also run many commands during the same process without restarting tahoma ;
 
 For instance : `tahoma arm alarm garden close shutter room6 confort heater dining off plug office 25 sunscreen kitchen launch scene morning`
 
+Exemples :
+
+- tahoma open shutter kitchen
+- tahoma 25 sunscreen Velux3 (You can close a shutter or a sunscreen to a specifique level. Here it will close to 25% )
+- tahoma get sensor ['Luminace sensor garden'] (Just for sensors : you can use the full name of the device with [''] )
+- tahoma on plug office
+- tahoma get sensor door
+- tahoma arm alarm garden
+- confort heater dining
+- tahoma get sensor ['heater dining room']
+- tahoma launch scene morning
+- tahoma arm alarm garden open shutter room6 confort heater dining off plug office 25 sunscreen kitchen launch scene morning get sensor ['heater dining room']
+
 
 # But first you need to retrieve your PERSONALS commands :
 
 
 ## Get a list of all possibles [ACTIONS] for each [CATEGORIES] : 
 
 Open a terminal and type :
```

### Comparing `tahoma-2.2.6/README.md` & `tahoma-2.2.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -86,24 +86,39 @@
 or
 - C:\foler\of\tahoma\tahoma.exe -g
 
 3. And now, you are ready to use tahoma :
 
 
 # Usage : 
+
 `tahoma [ACTION] [CATEGORY] [NAME]`
 
 
 For instance : `tahoma open shutter kitchen` or `tahoma ouvrir volet cuisine`
 
 You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
 
 You can also run many commands during the same process without restarting tahoma ;
 
-For instance : `tahoma arm alarm garden open shutter kitchen close shutter room6 confort heater dining off plug office 25 sunscreen kitchen`
+For instance : `tahoma arm alarm garden close shutter room6 confort heater dining off plug office 25 sunscreen kitchen launch scene morning`
+
+Exemples :
+
+- tahoma open shutter kitchen
+- tahoma 25 sunscreen Velux3 (You can close a shutter or a sunscreen to a specifique level. Here it will close to 25% )
+- tahoma get sensor ['Luminace sensor garden'] (Just for sensors : you can use the full name of the device with [''] )
+- tahoma on plug office
+- tahoma get sensor door
+- tahoma arm alarm garden
+- confort heater dining
+- tahoma get sensor ['heater dining room']
+- tahoma launch scene morning
+- tahoma arm alarm garden open shutter room6 confort heater dining off plug office 25 sunscreen kitchen launch scene morning get sensor ['heater dining room']
+
 
 # But first you need to retrieve your PERSONALS commands :
 
 
 ## Get a list of all possibles [ACTIONS] for each [CATEGORIES] : 
 
 Open a terminal and type :
@@ -164,15 +179,15 @@
 
 
 By doing this, instead of taping `python3 '/place/of/the/folder/tahoma/tahoma.py open shutter kitchen'`,
 
  you will be able to directly tape in the terminal : `tahoma open shutter kitchen`.
 
 
-Then execute tahoma just like this : `tahoma arm alarm garden open shutter kitchen close shutter room6 confort heater dining off plug office` and that's all !
+Then execute tahoma just like this : `tahoma arm alarm garden close shutter room6 confort heater dining off plug office 25 sunscreen kitchen launch scene morning` and that's all !
 
 
 
 
 
 
 For :
```

### Comparing `tahoma-2.2.6/pyproject.toml` & `tahoma-2.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.6/tahoma/icons/connected_house.png` & `tahoma-2.2.7/tahoma/icons/connected_house.png`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.6/tahoma/icons/water heater.png` & `tahoma-2.2.7/tahoma/icons/water heater.png`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.6/tahoma/tahoma.py` & `tahoma-2.2.7/tahoma/tahoma.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,40 +18,41 @@
 from pyoverkiz.const import SUPPORTED_SERVERS
 from pyoverkiz.client import OverkizClient
 from pyoverkiz.enums import OverkizCommand
 from pyoverkiz.models import Command
 from pyoverkiz.models import Scenario
 from tahoma import __version__
 
-
 def main():
-    version ='tahoma - Version '+ str(__version__.__version__)+' - by @pzim-devdata'
+    version ='tahoma - portable Version '+ str(__version__.__version__)+' - by @pzim-devdata'
 
     icon_app = os.path.dirname(os.path.abspath(__file__))+'/icons/connected_house.png'
     icon_chauffe_eau=os.path.dirname(os.path.abspath(__file__))+'/icons/water heater.png'
 
     passwd_file = os.path.dirname(os.path.abspath(__file__))+'/temp/identifier_file.txt'
 
     list_of_tahoma_devices = os.path.dirname(os.path.abspath(__file__))+'/temp/list_of_tahoma_devices.txt'
     list_of_tahoma_shutters = os.path.dirname(os.path.abspath(__file__))+'/temp/shutters.txt'
     list_of_tahoma_heaters = os.path.dirname(os.path.abspath(__file__))+'/temp/heaters.txt'
     list_of_tahoma_alarms = os.path.dirname(os.path.abspath(__file__))+'/temp/alarms.txt'
     list_of_tahoma_spotalarms = os.path.dirname(os.path.abspath(__file__))+'/temp/spotalarms.txt'
     list_of_tahoma_plugs = os.path.dirname(os.path.abspath(__file__))+'/temp/plugs.txt'
     list_of_tahoma_sunscreens = os.path.dirname(os.path.abspath(__file__))+'/temp/sunscreens.txt'
     list_of_tahoma_scenes = os.path.dirname(os.path.abspath(__file__))+'/temp/scenarios.txt'
+    list_of_tahoma_sensors = os.path.dirname(os.path.abspath(__file__))+'/temp/sensors.txt'
+    list_of_tahoma_states = os.path.dirname(os.path.abspath(__file__))+'/temp/states.txt'
 
     notification_consent = os.path.dirname(os.path.abspath(__file__))+'/temp/consent_notification.txt'
 
     server_choosen =  os.path.dirname(os.path.abspath(__file__))+'/temp/server_choosen.txt'
 
-    list_categories = ['shutter','spotalarm','plug','alarm','heater','sunscreen','scene']
-    list_categories_french = ['volet','spotalarme','prise','alarme','chauffage','rideau','scenario']
-    list_actions = ['[open,close,stop,my,NUMBER]','[on,off]','[on,off]','[arm,disarm,partial,arm_night,arm_away]','[comfort,comfort-1,comfort-2,eco,off]','[open,close,stop,my,NUMBER]','[on,activate,launch,execute]']
-    list_actions_french = ['[ouvrir,fermer,stop,my,NOMBRE]','[allumer,eteindre]','[allumer,eteindre]','[activer,desactiver,partiel,activer_nuit,activer_parti]','[confort,confort-1,confort-2,eco,eteindre]','[ouvrir,fermer,stop,my,NOMBRE]','[lancer,activer,executer]']
+    list_categories = ['shutter','spotalarm','plug','alarm','heater','sunscreen','scene','sensor']
+    list_categories_french = ['volet','spotalarme','prise','alarme','chauffage','rideau','scenario','capteur']
+    list_actions = ['[open,close,stop,my,NUMBER]','[on,off]','[on,off]','[arm,disarm,partial,arm_night,arm_away]','[comfort,comfort-1,comfort-2,eco,off]','[open,close,stop,my,NUMBER]','[on,activate,launch,execute]','[get,get_state,get_position,get_lumens,get_temperature]']
+    list_actions_french = ['[ouvrir,fermer,stop,my,NOMBRE]','[allumer,eteindre]','[allumer,eteindre]','[activer,desactiver,partiel,activer_nuit,activer_parti]','[confort,confort-1,confort-2,eco,eteindre]','[ouvrir,fermer,stop,my,NOMBRE]','[lancer,activer,executer]','[obtenir,etat,position,luminosite,temperature]']
 
     try :
         f = open(notification_consent, 'r')
         notification = f.read()
         f.close()
     except FileNotFoundError:
         notification = 'n'
@@ -62,33 +63,35 @@
         f.close()
     except FileNotFoundError:
         serverchoice = "somfy_europe"
 
     def info():
         print( "" )
         print( "      ***************************************************************      " )
-        print( "------*     "+version+"     *-------" )
+        print( "------*     Tahoma version : "+version+"     *-------" )
         print( "      ***************************************************************        " )
         print( "              sudo python3 -m pip install tahoma-pzim -U" )
         print( "                   https://pypi.org/project/tahoma/" )
         print( "                 https://github.com/pzim-devdata/tahoma" )
         print( "                          contact@pzim.fr" )
         print( "" )
         print( " USAGE : tahoma [ACTION] [CATEGORY] [NAME]" )
         print( "")
         print( " - List of possible ACTIONS : \n "+str(list_actions) )
         print( " - Liste des ACTIONS possibles : \n "+str(list_actions_french) )
         print( "" )
         print( " - List of possible CATEGORIES : \n "+str(list_categories) )
         print( " - Liste des CATEGORIES possibles : \n "+str(list_categories_french) )
         print( "" )
-        print( " - List of available NAMES : tahoma --list-names \n - Liste des NOMS possibles : tahoma --list-names-french \n You must provide a part of the name you have assigned to the device in the Tahoma App. \n It must be a single and unic word, not taken by another device of the same category !\n For instance if you have two devices called <Alarm 1> and <Alarm 2> you will need to choose <2> as device [NAME] for <Alarm 2> and not <Alarm>).\n See tahoma --list or tahoma --help for info")
+        print( " - List of available NAMES : tahoma --list-names \n - Liste des NOMS possibles : tahoma --list-names-french \n You must provide a part of the name you have assigned to the device in the Tahoma App. \n It must be a single and unic word, not taken by another device of the same category !\n For instance if you have two devices called <Alarm 1> and <Alarm 2> you will need to choose <2> as device [NAME] for <Alarm 2> and not <Alarm>).\n See tahoma --list or tahoma --help for info\nJust for sensors, you can use the full <NAME> : Use square brackets AND quotation mark : ['<NAME>'] . \nFor exemple if you want to use the <NAME> <Heater Room 6> the syntax should be : ['Heater Room 6'].")
         print( "" )
-        print( "                  You must provide at least 3 arguments" )
-        print( "         For instance : python3 tahoma open shutter kitchen or python3 tahoma 25 shutter kitchen" )
+        print( " You must provide at least 3 arguments" )
+        print( " For instance : python3 tahoma open shutter kitchen")
+        print( "\n You can close a shutter or a sunscreen to a specific level (IO protocols only)")
+        print( " For instance :python3 tahoma 25 shutter kitchen. It will open the shutter to 75% or close it to 25%" )
         print( "" )
         print( " You can also provide, as many as you wish, orders on the same line." ) 
         print( " Tahoma will execute all orders one by one on the same process ;-)" )
         print( " For instance : tahoma open shutter kitchen arm alarm garden on plug room wait train garestation " )
         print( "" )
         print( " FIRST you must configure login and password : sudo tahoma -c " )
         print( " It will be stored there : \n "+passwd_file )
@@ -216,15 +219,15 @@
     for arg in sys.argv :
         if arg == '-lc' or arg == '--list-categories' :
             print( "tahoma can control this type of devices's categories :\n"+str(list_categories))
             exit()
 
     for arg in sys.argv :
         if arg == '-lcf' or arg == '--list-categories-french' :
-            print( "tahoma peut controler ce type de categories d'équipements :\n"+str(list_categories))
+            print( "tahoma peut controler ce type de categories d'équipements :\n"+str(list_categories_french))
             exit()
 
     for arg in sys.argv :
         if arg == '-ln' or arg == '--list-names' :
             print("\nExecute tahoma --getlist before this command for being sure to have a complete list of installed devices")
             for category in list_categories :
                 try:
@@ -304,30 +307,31 @@
 
     parser.add_argument("action")
     parser.add_argument("category")
     parser.add_argument("name")
     parser.add_argument("suite", nargs='*')
 
     args = parser.parse_args()
-    print(f'Input action(s) : {args.action} {args.category} {args.name} '+' '.join(args.suite) )
+#    print(f'Input action(s) : {args.action} {args.category} {args.name} '+' '.join(args.suite) )
 
     if args.password:
         PASSWORD = (f'{args.password}')
     if args.username:
         USERNAME = (f'{args.username}')
 
     def remove_accent(old):
         new = old.lower()
         new = re.sub(r'[àáâãäå]', 'a', new)
         new = re.sub(r'[èéêë]', 'e', new)
         new = re.sub(r'[ìíîï]', 'i', new)
         new = re.sub(r'[òóôõö]', 'o', new)
         new = re.sub(r'[ùúûü]', 'u', new)
+        new = re.sub(r'[ç]', 'c', new)
         return new
-        
+
     ##########################PARAMETERING FUNCTION
 
     j=0
     for i in range(-1,int(len(args.suite)/3)) :
         if i == -1 :
             action = args.action
             category=args.category
@@ -587,34 +591,86 @@
             
             #fonction = Command(OverkizCommand.SET_HEATING_LEVEL,['comfort'])
             #exec_id = await client.execute_scenario(device_url)
 
             str1 = " "
             print("Output action : "+remove_accent(action).lower()+" "+remove_accent(category)+" "+str1.join(good_name)+ " \nwith url : "+str1.join(url))
 
+        ##########################SENSORS_STATES
+
+        elif remove_accent(category) == 'sensor' or remove_accent(category) == 'capteur':
+            command_state=[]
+            f = open(list_of_tahoma_states, 'r')
+            content = f.read()
+            f.close()
+            time.sleep(1)
+            try:
+                master_list = content.split("\n")
+                master_list.remove('')
+            except ValueError:
+                print("\nDid you downloaded the list of Tahoma's sensors ?.\nExecute tahoma --getlist \nFor more info execute tahoma -h or tahoma --info")
+                exit()
+            for i in master_list :
+                bad_name.append(i.split(",")[0])
+                if len(name.split())>1 :
+                    if remove_accent(i.split(",")[0]) == remove_accent(str(name)) or remove_accent(str(name)).replace('[','').replace(']','') == remove_accent(i.split(",")[0]) :
+                        url.append(i.split(",")[1])
+                        too_many_urls.append(i.split(",")[0])
+                        good_name.append(i.split(",")[0])
+                        command_state.append(i.split(",")[3])
+                elif str(name).startswith("[") :
+                    if '['+remove_accent(i.split(",")[0])+']' == remove_accent(str(name)) or remove_accent(str(name)).replace('[','').replace(']','') == remove_accent(i.split(",")[0]) :
+                        url.append(i.split(",")[1])
+                        too_many_urls.append(i.split(",")[0])
+                        good_name.append(i.split(",")[0])
+                        command_state.append(i.split(",")[3])
+                else :
+                    if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
+                         url.append(i.split(",")[1])
+                         too_many_urls.append(i.split(",")[0])
+                         good_name.append(i.split(",")[0])
+                         command_state.append(i.split(",")[3])
+
+            if len(url)== 0 :
+                print("There is no match. The <NAME> you gave is not exact or it's impossible to retrieve the state of '"+args.name+"'. \nPerhaps because it's RTS protocol and not IO. \n\nHere are supported devices : "+str(bad_name)+" \n\nChoose a UNIQUE part of word from this supported devices as <NAME> argument or if you want to indicate the exact <NAME> use square brackets AND quotation mark : ['<NAME>'] . \nFor exemple if you want to use the <NAME> <Heater Room 6> the syntax should be : ['Heater Room 6']. \n\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
+                exit()
+
+#            command_state=[]
+#            time.sleep(1)
+#            for i in master_list :
+#                if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
+#                     command_state.append(i.split(",")[3])
+
         ##########################
 
         else :
             print( "\nThe <CATEGORY> you have entered doesn't exist.\nChoose one of this category : "+str(list_categories)+"\nUse tahoma --help-categories or tahoma --list-categories for info")
 
 
     ##########################MAIN FUNCTION
 
         try:
             async def main() -> None:
                 async with OverkizClient(USERNAME, PASSWORD, SUPPORTED_SERVERS[serverchoice]) as client:
                     await client.login()
                     try :
+                        j=0
                         for device_url in url :
                             try :
                                 exec_id = await client.execute_command( device_url, fonction )
                             except : pass
                             try :
                                 exec_id = await client.execute_scenario(device_url)
                             except : pass
+                            try:
+                                get_state = await client.get_state(device_url)
+                                state_function=str(command_state[j]).replace("['","").replace("']","")
+                                print('The '+str(good_name[j])+' is '+str(eval(state_function)))
+                                j=j+1
+                            except :pass 
                     except Exception as e:
                         print(e) 
                         try:
                             if notification.lower() == 'y'or notification.lower() == 'yes':
                                 os.system("notify-send -i "+icon_app+" -t 150000 Tahoma "+"'Program failed. Here is the error message :\n\n "+str(e)+"'")
                         except:pass
                         exit()
```

### Comparing `tahoma-2.2.6/tahoma.egg-info/PKG-INFO` & `tahoma-2.2.7/tahoma.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoma
-Version: 2.2.6
+Version: 2.2.7
 Summary: This is a very easy API for controlling Somfy Tahoma's devices written in Python3, thanks to the pyoverkiz API. You just need a three-word input to control a device
 Author-email: Pzim-devdata <contact@pzim.fr>
 Project-URL: Homepage, https://github.com/pzim-devdata/tahoma
 Project-URL: Bug Tracker, https://github.com/pzim-devdata/tahoma/issues
 Keywords: tahoma,somfy,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -101,25 +101,39 @@
 or
 - C:\foler\of\tahoma\tahoma.exe -g
 
 3. And now, you are ready to use tahoma :
 
 
 # Usage : 
+
 `tahoma [ACTION] [CATEGORY] [NAME]`
 
 
 For instance : `tahoma open shutter kitchen` or `tahoma ouvrir volet cuisine`
 
 You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
 
 You can also run many commands during the same process without restarting tahoma ;
 
 For instance : `tahoma arm alarm garden close shutter room6 confort heater dining off plug office 25 sunscreen kitchen launch scene morning`
 
+Exemples :
+
+- tahoma open shutter kitchen
+- tahoma 25 sunscreen Velux3 (You can close a shutter or a sunscreen to a specifique level. Here it will close to 25% )
+- tahoma get sensor ['Luminace sensor garden'] (Just for sensors : you can use the full name of the device with [''] )
+- tahoma on plug office
+- tahoma get sensor door
+- tahoma arm alarm garden
+- confort heater dining
+- tahoma get sensor ['heater dining room']
+- tahoma launch scene morning
+- tahoma arm alarm garden open shutter room6 confort heater dining off plug office 25 sunscreen kitchen launch scene morning get sensor ['heater dining room']
+
 
 # But first you need to retrieve your PERSONALS commands :
 
 
 ## Get a list of all possibles [ACTIONS] for each [CATEGORIES] : 
 
 Open a terminal and type :
```

### Comparing `tahoma-2.2.6/tahoma.egg-info/SOURCES.txt` & `tahoma-2.2.7/tahoma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

