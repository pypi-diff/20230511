# Comparing `tmp/launchpy-0.4.0.post3.tar.gz` & `tmp/launchpy-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launchpy-0.4.0.post3.tar", last modified: Wed Jan 25 12:01:17 2023, max compression
+gzip compressed data, was "launchpy-0.4.1.tar", last modified: Thu May 11 13:29:15 2023, max compression
```

## Comparing `launchpy-0.4.0.post3.tar` & `launchpy-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-01-25 12:01:17.441313 launchpy-0.4.0.post3/
--rw-rw-rw-   0        0        0    35823 2021-10-20 19:49:46.000000 launchpy-0.4.0.post3/LICENSE
--rw-rw-rw-   0        0        0      858 2023-01-25 12:01:17.440317 launchpy-0.4.0.post3/PKG-INFO
--rw-rw-rw-   0        0        0     1290 2022-11-09 18:49:02.000000 launchpy-0.4.0.post3/README.md
-drwxrwxrwx   0        0        0        0 2023-01-25 12:01:17.425357 launchpy-0.4.0.post3/launchpy/
--rw-rw-rw-   0        0        0      268 2022-11-08 13:23:21.000000 launchpy-0.4.0.post3/launchpy/__init__.py
--rw-rw-rw-   0        0        0       23 2023-01-25 08:54:56.000000 launchpy-0.4.0.post3/launchpy/__version__.py
--rw-rw-rw-   0        0        0    14165 2022-11-15 15:33:26.000000 launchpy-0.4.0.post3/launchpy/admin.py
--rw-rw-rw-   0        0        0      712 2021-11-08 18:47:00.000000 launchpy-0.4.0.post3/launchpy/config.py
--rw-rw-rw-   0        0        0     6823 2022-11-08 13:20:12.000000 launchpy-0.4.0.post3/launchpy/configs.py
--rw-rw-rw-   0        0        0    11497 2021-10-20 19:49:47.000000 launchpy-0.4.0.post3/launchpy/connector.py
--rw-rw-rw-   0        0        0    29268 2022-11-23 09:43:28.000000 launchpy-0.4.0.post3/launchpy/launchpy.py
--rw-rw-rw-   0        0        0    16796 2023-01-25 08:51:08.000000 launchpy-0.4.0.post3/launchpy/library.py
--rw-rw-rw-   0        0        0    74185 2023-01-18 11:01:23.000000 launchpy-0.4.0.post3/launchpy/property.py
--rw-rw-rw-   0        0        0    20655 2023-01-11 19:42:54.000000 launchpy-0.4.0.post3/launchpy/synchronizer.py
-drwxrwxrwx   0        0        0        0 2023-01-25 12:01:17.437324 launchpy-0.4.0.post3/launchpy.egg-info/
--rw-rw-rw-   0        0        0      858 2023-01-25 12:01:17.000000 launchpy-0.4.0.post3/launchpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-01-25 12:01:17.000000 launchpy-0.4.0.post3/launchpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-25 12:01:17.000000 launchpy-0.4.0.post3/launchpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-01-25 12:01:17.000000 launchpy-0.4.0.post3/launchpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-01-25 12:01:17.000000 launchpy-0.4.0.post3/launchpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-25 12:01:17.442311 launchpy-0.4.0.post3/setup.cfg
--rw-rw-rw-   0        0        0     1754 2021-10-20 19:49:47.000000 launchpy-0.4.0.post3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 13:29:15.256854 launchpy-0.4.1/
+-rw-rw-rw-   0        0        0    35823 2021-10-20 19:49:46.000000 launchpy-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0      852 2023-05-11 13:29:15.255857 launchpy-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1290 2022-11-09 18:49:02.000000 launchpy-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 13:29:15.217959 launchpy-0.4.1/launchpy/
+-rw-rw-rw-   0        0        0      268 2022-11-08 13:23:21.000000 launchpy-0.4.1/launchpy/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-05-11 13:26:59.000000 launchpy-0.4.1/launchpy/__version__.py
+-rw-rw-rw-   0        0        0    14165 2023-05-10 17:31:08.000000 launchpy-0.4.1/launchpy/admin.py
+-rw-rw-rw-   0        0        0      712 2021-11-08 18:47:00.000000 launchpy-0.4.1/launchpy/config.py
+-rw-rw-rw-   0        0        0     6823 2022-11-08 13:20:12.000000 launchpy-0.4.1/launchpy/configs.py
+-rw-rw-rw-   0        0        0    11497 2021-10-20 19:49:47.000000 launchpy-0.4.1/launchpy/connector.py
+-rw-rw-rw-   0        0        0    29268 2023-05-10 17:31:00.000000 launchpy-0.4.1/launchpy/launchpy.py
+-rw-rw-rw-   0        0        0    16796 2023-05-10 17:30:51.000000 launchpy-0.4.1/launchpy/library.py
+-rw-rw-rw-   0        0        0    74941 2023-05-10 17:30:38.000000 launchpy-0.4.1/launchpy/property.py
+-rw-rw-rw-   0        0        0    25209 2023-05-11 12:16:25.000000 launchpy-0.4.1/launchpy/synchronizer.py
+drwxrwxrwx   0        0        0        0 2023-05-11 13:29:15.251868 launchpy-0.4.1/launchpy.egg-info/
+-rw-rw-rw-   0        0        0      852 2023-05-11 13:29:15.000000 launchpy-0.4.1/launchpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-05-11 13:29:15.000000 launchpy-0.4.1/launchpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 13:29:15.000000 launchpy-0.4.1/launchpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-11 13:29:15.000000 launchpy-0.4.1/launchpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-11 13:29:15.000000 launchpy-0.4.1/launchpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 13:29:15.257851 launchpy-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1754 2021-10-20 19:49:47.000000 launchpy-0.4.1/setup.py
```

### Comparing `launchpy-0.4.0.post3/LICENSE` & `launchpy-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.0.post3/PKG-INFO` & `launchpy-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launchpy
-Version: 0.4.0.post3
+Version: 0.4.1
 Summary: Python wrapper around the Adobe Experience Launch API.
 Home-page: https://github.com/pitchmuc/launchpy
 Author: Julien Piccini
 Author-email: piccini.julien@gmail.com
 Keywords: adobe,Launch,API,python,Tag Manager
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `launchpy-0.4.0.post3/README.md` & `launchpy-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.0.post3/launchpy/admin.py` & `launchpy-0.4.1/launchpy/admin.py`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.0.post3/launchpy/config.py` & `launchpy-0.4.1/launchpy/config.py`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.0.post3/launchpy/configs.py` & `launchpy-0.4.1/launchpy/configs.py`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.0.post3/launchpy/connector.py` & `launchpy-0.4.1/launchpy/connector.py`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.0.post3/launchpy/launchpy.py` & `launchpy-0.4.1/launchpy/launchpy.py`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.0.post3/launchpy/library.py` & `launchpy-0.4.1/launchpy/library.py`

 * *Files identical despite different names*

### Comparing `launchpy-0.4.0.post3/launchpy/property.py` & `launchpy-0.4.1/launchpy/property.py`

 * *Files 1% similar despite different names*

```diff
@@ -409,14 +409,16 @@
         Argument:
             dataElementId : REQUIRED : a Data Element ID
         """
         if dataElementId is None:
             raise ValueError('Require a Data Element ID')
         path = f"/data_elements/{dataElementId}"
         res = self.connector.getData(self.endpoint+path)
+        if 'data' in res.keys():
+            return res['data']
         return res
 
     def searchDataElements(self, name: str = None, enabled: bool = None, published: bool = None, dirty: bool = None, **kwargs)->object:
         """
         Returns the rules searched through the different operator. One argument is required in order to return a result. 
         Arguments: 
             name : OPTIONAL : string of what is searched (used as "contains")
@@ -910,27 +912,29 @@
         }
         path = f"/data_elements/{dataElement_id}"
         dataElements = self.connector.patchData(
             self.endpoint+path, data=obj)
         data = dataElements
         return data
 
-    def getRule(self, rule_id: str=None)->object:
+    def getRule(self, rule_id: str=None)->dict:
         """
         Update the rule based on elements passed in attr_dict. 
         arguments: 
             rule_id : REQUIRED : Rule ID
             attr_dict : REQUIRED : dictionary that will be passed to Launch for update
         documentation : https://developer.adobelaunch.com/api/reference/1.0/rules/update/
         """
         if rule_id is None:
             raise ValueError('Require a rule ID')
         path = f'/rules/{rule_id}'
         rule = self.connector.getData(
             self.endpoint+path)
+        if 'data' in rule.keys():
+            return rule['data']
         return rule
 
     def updateRule(self, rule_id: str, attr_dict: dict)->dict:
         """
         Update the rule based on elements passed in attr_dict. 
         arguments: 
             rule_id : REQUIRED : Rule ID
@@ -1004,15 +1008,15 @@
             myRCsettings['customSetup']['source'] = myCode
         myNewSettings = json.dumps(myRCsettings)
         obj = {"settings": myNewSettings}
         res = self.updateRuleComponent(rc_id=rc_id, attr_dict=obj)
         return res
 
 
-    def updateDataElement(self, dataElement_id: str, attr_dict: object, **kwargs)->object:
+    def updateDataElement(self, dataElement_id: str, attr_dict: object, **kwargs)->dict:
         """
         Update the data element information based on the information provided.
         arguments: 
             dataElement_id : REQUIRED : Data Element ID
             attr_dict : REQUIRED : dictionary that will be passed to Launch for update
         """
         obj = {
@@ -1027,15 +1031,29 @@
             self.endpoint+path, data=obj)
         try:
             data = dataElements['data']
         except:
             data = dataElements
         return data
 
-    def updateEnvironment(self, name: str, env_id: str, **kwargs)->object:
+    def updateDataElementCode(self,dataElementId:str=None,code:str=None)->dict:
+        """
+        Update a data element custom code by passing the data element ID and the code as strng you want to upload.
+        Arguments:
+            dataElementId : REQUIRED : The data element ID
+            code : REQUIED : The code stringify
+        """
+        de = self.getDataElement(dataElementId)
+        attr = deepcopy(de['attributes'])
+        attr['settings'] = json.dumps({'source' : code})
+        print(json.dumps(attr,indent=2))
+        newDE = self.updateDataElement(dataElementId,attr)
+        return newDE
+
+    def updateEnvironment(self, name: str, env_id: str, **kwargs)->dict:
         """
         Update an environment. Note :only support name change.
         Arguments:
             name : REQUIRED : name of your environment
             env_id : REQUIRED : The environement id.
         documentation : https://developer.adobelaunch.com/api/reference/1.0/environments/create/
         """
```

### Comparing `launchpy-0.4.0.post3/launchpy/synchronizer.py` & `launchpy-0.4.1/launchpy/synchronizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-import re
+import re,json
 # Non standard libraries
 from .admin import Admin
 from .property import Property
 from .library import Library
 from .launchpy import Translator, copySettings
+from collections import defaultdict
+from copy import deepcopy
 
 class Synchronizer:
     """
     The synchronizer class provides an abstaction layer for synchronizing the rule components and the data elements.
     It combined the usage of elements provided by the launchpy library: 
     - Property class
     - Translator class
     - copySetting method
     - extensionInfo method
     - RulesInfo method
     It takes 2 arguments, the base property (template) where all information will be fetched from. The target properties where the element will be copied to.
     It requires that you have imported a configuration file.
     """
 
-    def __init__(self,base:str=None,targets:list=None)->None:
+    def __init__(self,base:str=None,targets:list=None,**kwargs)->None:
         """
         Instantiating the Synchronizer taking 2 parameters, base property name, target property list.
         Arguments:
             base : REQUIRED : The name of your base/template property
             targets : REQUIRED : The list of property names that you want to sync with.
+        possible kwargs:
+            dynamicRuleComponent: A data element name that contains rule for synchronization on the property.
         """
         tmp_admin = Admin()
         cid = tmp_admin.getCompanyId()
         properties = tmp_admin.getProperties(cid)
         base_property = [prop for prop in properties if prop['attributes']['name'] == base]
         if len(base_property) ==0:
             raise KeyError("The base property name has not been found in your account")
@@ -36,14 +40,28 @@
         self.base["api"] = Property(base_property[0])
         self.base['rules'] = self.base['api'].getRules()
         self.base['dataElements'] = self.base['api'].getDataElements()
         self.base['extensions'] = self.base['api'].getExtensions()
         self.translator = Translator()
         self.translator.setBaseExtensions(self.base['extensions'],self.base['name'])
         self.translator.setBaseRules(self.base['rules'],self.base['name'])
+        self.dict_config = {}
+        if kwargs.get("dynamicRuleComponent",None) is not None:
+            configRules = [de for de in self.base['dataElements'] if de['attributes']['name'] == kwargs.get("dynamicRuleComponent",None)]
+            if len(configRules)==1:
+                configRules = configRules[0]
+            else:
+                raise ValueError("The dynamicRuleComponent is using a value that does not match any data element.")
+            codeConfig:list = json.loads(json.loads(configRules['attributes']['settings'])['source'])## list expected from the code
+            for rule in codeConfig:
+                self.dict_config[rule['targetProperties']] = {'inclComponents':[],'exclComponents':[]}
+                if 'inclComponents' in rule.keys():
+                    self.dict_config[rule['targetProperties']]['inclComponents'] += rule['inclComponents']
+                if 'exclComponents' in rule.keys():
+                    self.dict_config[rule['targetProperties']]['exclComponents'] += rule['exclComponents']
         self.targets = {}
         for target in targets:
             tmp_target = [prop for prop in properties if prop['attributes']['name'] == target]
             if len(tmp_target) == 0:
                 raise KeyError(f"The target property : {target} cannot be found. Please, fix it")
             self.targets[target] = {'api' : Property(tmp_target[0]),'name':target}
             self.targets[target]['rules'] = self.targets[target]['api'].getRules()
@@ -51,20 +69,34 @@
             self.targets[target]['dataElements'] = self.targets[target]['api'].getDataElements()
             self.targets[target]['libraryStack'] = {'dataElements':[],'rules':[]}
             self.translator.extendExtensions(self.targets[target]['extensions'],self.targets[target]['name'])
             if len(self.targets[target]['rules']) > 0:
                 self.translator.extendRules(self.targets[target]['rules'],self.targets[target]['name'])
             else:
                 self.translator.rules[self.targets[target]['name']] = None
+        self.target_configs = {}
+        if len(self.dict_config)>0: ## verify that there are rules
+            for rule in self.dict_config.keys():
+                for target in self.targets.keys():
+                    if re.search(rule,target) is not None:
+                        if target in self.target_configs.keys():
+                            self.target_configs[target]['exclComponents'] += deepcopy(self.dict_config[rule]['exclComponents'])
+                            self.target_configs[target]['inclComponents'] += deepcopy(self.dict_config[rule]['inclComponents'])
+                        else:
+                            self.target_configs[target] = {
+                                'exclComponents': deepcopy(self.dict_config[rule]['exclComponents']),
+                                'inclComponents': deepcopy(self.dict_config[rule]['inclComponents'])
+                            }
 
-    def syncComponent(self,componentName:str=None,componentId:str=None,publishedVersion:bool=False)->None:
+    def syncComponent(self,componentName:str=None,componentId:str=None,publishedVersion:bool=False,**kwargs)->None:
         """
         Synchronize a component from the base property to the different target properties.
         It will detect the component with the same name in target properties.
         It will delete the components related objects (ruleComponents, data element code) in the target property and push the template version.
+        If you uploaded a dynamicRuleComponent data element config during the init method, any element that are not sync because of the exclComponentList will return a dict: {componentName:False} 
         Arguments:
             componentName : REQUIRED : the name of the component to sync
             componentID : REQUIRED : the id of the component to sync
             publishedVersion : OPTIONAL : if you want to take the version that has been published
         """
         if componentName is None and componentId is None:
             raise ValueError('Require a component Name of a component ID')
@@ -111,122 +143,142 @@
             cmp_baseDict['component'] = publishedVersion
             cmp_baseDict['copy'] = copySettings(publishedVersion)
         ## handling the data element
         if cmp_baseDict['component']['type'] == 'data_elements':
             latestCompVersion = self.base['api'].getDataElement(cmp_baseDict['id']).get('data',cmp_baseDict['component'])
             cmp_baseDict = {'id':latestCompVersion['id'],'name':latestCompVersion['attributes']['name'],'component':latestCompVersion,'copy':copySettings(latestCompVersion)}
             for target in list(self.targets.keys()):
-                translatedComponent = self.translator.translate(target,data_element=cmp_baseDict['copy'])
-                ## if it does not exist
-                if cmp_baseDict['name'] not in [de['attributes']['name'] for de in self.targets[target]['dataElements']]:
-                    comp = self.targets[target]['api'].createDataElement(
-                        name=cmp_baseDict['name'],
-                        descriptor= translatedComponent['descriptor'],
-                        settings=translatedComponent['settings'],
-                        extension=translatedComponent['extension'],
-                        storage_duration = translatedComponent["storage_duration"],
-                        force_lower_case = translatedComponent["force_lower_case"],
-                        clean_text = translatedComponent["clean_text"],
-                        default_value= translatedComponent["default_value"]
-                        )
-                    if cmp_baseDict['component']['attributes']['enabled'] != comp['attributes']['enabled']:
-                        updateDE = self.targets[target]['api'].updateDataElement(
-                            dataElement_id=comp['id'],
-                            attr_dict=translatedComponent)
-                    self.targets[target]['libraryStack']['dataElements'].append(comp)
-                    self.targets[target]['dataElements'].append(comp)
-                else:
-                    index,old_component = [(index,de) for index,de in enumerate(self.targets[target]['dataElements']) if de['attributes']['name'] == cmp_baseDict['name']][0]
-                    attributes = {
-                        "name" : translatedComponent['name'],
-                        "enabled" : translatedComponent["enabled"],
-                        "delegate_descriptor_id" : translatedComponent["descriptor"],
-                        "storage_duration" : translatedComponent["storage_duration"],
-                        "force_lower_case" : translatedComponent["force_lower_case"],
-                        "clean_text" : translatedComponent["clean_text"],
-                        "settings" : translatedComponent["settings"],
-                        "default_value": translatedComponent["default_value"]
-                    }
-                    comp = self.targets[target]['api'].updateDataElement(
-                        dataElement_id=old_component['id'],
-                        attr_dict=attributes,
-                        )
-                    del self.targets[target]['dataElements'][index]
-                    self.targets[target]['dataElements'].append(comp)
-                    self.targets[target]['libraryStack']['dataElements'].append(comp)
+                flagAllowList = False
+                ## check if the component is in the exclComponentList
+                if any([bool(re.search(key,cmp_baseDict['name'])) for key in self.target_configs.get(target,{}).get('exclComponents',[])]):
+                    return {cmp_baseDict['name']:False}
+                ## if there is an allow list for that property
+                if len(self.target_configs.get(target,{}).get('inclComponents',[]))>0:
+                    if any([bool(re.search(key,cmp_baseDict['name'])) for key in self.target_configs.get(target,{}).get('inclComponents',[])]):
+                        flagAllowList = True
+                ## if there is no allow list for that property, or no match in the list of target properties, or component was allow
+                if len(self.target_configs.get(target,{}).get('inclComponents',[]))==0 or flagAllowList:
+                    translatedComponent = self.translator.translate(target,data_element=cmp_baseDict['copy'])
+                    ## if it does not exist
+                    if cmp_baseDict['name'] not in [de['attributes']['name'] for de in self.targets[target]['dataElements']]:
+                        comp = self.targets[target]['api'].createDataElement(
+                            name=cmp_baseDict['name'],
+                            descriptor= translatedComponent['descriptor'],
+                            settings=translatedComponent['settings'],
+                            extension=translatedComponent['extension'],
+                            storage_duration = translatedComponent["storage_duration"],
+                            force_lower_case = translatedComponent["force_lower_case"],
+                            clean_text = translatedComponent["clean_text"],
+                            default_value= translatedComponent["default_value"]
+                            )
+                        if cmp_baseDict['component']['attributes']['enabled'] != comp['attributes']['enabled']:
+                            updateDE = self.targets[target]['api'].updateDataElement(
+                                dataElement_id=comp['id'],
+                                attr_dict=translatedComponent)
+                        self.targets[target]['libraryStack']['dataElements'].append(comp)
+                        self.targets[target]['dataElements'].append(comp)
+                    else:
+                        index,old_component = [(index,de) for index,de in enumerate(self.targets[target]['dataElements']) if de['attributes']['name'] == cmp_baseDict['name']][0]
+                        attributes = {
+                            "name" : translatedComponent['name'],
+                            "enabled" : translatedComponent["enabled"],
+                            "delegate_descriptor_id" : translatedComponent["descriptor"],
+                            "storage_duration" : translatedComponent["storage_duration"],
+                            "force_lower_case" : translatedComponent["force_lower_case"],
+                            "clean_text" : translatedComponent["clean_text"],
+                            "settings" : translatedComponent["settings"],
+                            "default_value": translatedComponent["default_value"]
+                        }
+                        comp = self.targets[target]['api'].updateDataElement(
+                            dataElement_id=old_component['id'],
+                            attr_dict=attributes,
+                            )
+                        del self.targets[target]['dataElements'][index]
+                        self.targets[target]['dataElements'].append(comp)
+                        self.targets[target]['libraryStack']['dataElements'].append(comp)
         ## Rules part
         if cmp_baseDict['component']['type'] == 'rules':
             latestCompVersion = self.base['api'].getRule(cmp_baseDict['id']).get('data',cmp_baseDict['component'])
             cmp_baseDict = {'id':latestCompVersion['id'],'name':latestCompVersion['attributes']['name'],'component':latestCompVersion,'copy':copySettings(latestCompVersion)}
             ## fetching all rule components associated with a rule.
             rcsLink = cmp_baseDict['component'].get('relationships',{}).get('rule_components',{}).get('links',{}).get('related')
             resResource = self.base['api'].getRessource(rcsLink)
             template_ruleComponents:list = resResource['data']
             for rc in template_ruleComponents:
                 rc['rule_name'] = cmp_baseDict['name']
                 rc['rule_id'] = cmp_baseDict['id']
             for target in list(self.targets.keys()):
-                ## if rule does not exist
-                if cmp_baseDict['name'] not in [rule['attributes']['name'] for rule in self.targets[target]['rules']]:
-                    targetRule = self.targets[target]['api'].createRule(
-                        name=cmp_baseDict['name']
-                        )
-                    targetRuleId = targetRule['id']
-                    self.translator.extendTargetRules(ruleName=cmp_baseDict['name'],ruleId=targetRuleId,property_name=target)
-                    self.targets[target]['rules'].append(targetRule)
-                    index = len(self.targets[target]['rules'])-1
-                    self.targets[target]['libraryStack']['rules'].append(targetRule)
-                    for rc in template_ruleComponents:
-                        translatedComponent = self.translator.translate(target,rule_component=copySettings(rc))
-                        translatedComponent['rule_setting']['data'][0]['id'] = targetRuleId
-                        targetRuleComponent = self.targets[target]['api'].createRuleComponent(
-                            name=translatedComponent['name'],
-                            settings = translatedComponent['settings'],
-                            descriptor = translatedComponent['descriptor'],
-                            extension_infos = translatedComponent['extension'],
-                            rule_infos = translatedComponent['rule_setting'],
-                            rule_order=translatedComponent['rule_order'],
-                            order=translatedComponent['order'],
-                            negate=translatedComponent['negate'],
-                            delay_next=translatedComponent['delay_next'],
-                            timeout=translatedComponent['timeout'],
-                        )
-                else: ## if a rule exist with the same name
-                    index, targetRule = [(index,rule) for index, rule in enumerate(self.targets[target]['rules']) if rule['attributes']['name'] == cmp_baseDict['name']][0]
-                    self.targets[target]['libraryStack']['rules'].append(targetRule)
-                    targetRuleId = targetRule['id']
-                    rcsLinkTarget = targetRule.get('relationships',{}).get('rule_components',{}).get('links',{}).get('related')
-                    resResource = self.targets[target]['api'].getRessource(rcsLinkTarget)
-                    old_components:list = resResource['data']
-                    ## deleting the old version of rule component
-                    if len(old_components)>0:
-                        for component in old_components:
-                            self.targets[target]['api'].deleteRuleComponent(component['id'])
-                    ## creating the new version of the old version
-                    for rc in template_ruleComponents:
-                        translatedComponent = self.translator.translate(target,rule_component=copySettings(rc))
-                        translatedComponent['rule_setting']['data'][0]['id'] = targetRuleId
-                        targetRuleComponent = self.targets[target]['api'].createRuleComponent(
-                            name=translatedComponent['name'],
-                            settings = translatedComponent['settings'],
-                            descriptor = translatedComponent['descriptor'],
-                            extension_infos = translatedComponent['extension'],
-                            rule_infos = translatedComponent['rule_setting'],
-                            rule_order=translatedComponent['rule_order'],
-                            order=translatedComponent['order'],
-                            negate=translatedComponent['negate'],
-                            delay_next=translatedComponent['delay_next'],
-                            timeout=translatedComponent['timeout'],
-                        )
-                ## updating rule attribute if difference between base and target
-                if cmp_baseDict['component']['attributes']['enabled'] != targetRule['attributes']['enabled']:
-                    baseRuleAttr = copySettings(cmp_baseDict['component'])
-                    targetRule = self.targets[target]['api'].updateRule(rule_id=targetRuleId,attr_dict=baseRuleAttr) ## keeping in a var for debug
-                    del self.targets[target]['rules'][index]
-                    self.targets[target]['rules'].append(targetRule)
+                flagAllowList = False
+                ## check if the component is in the exclComponentList
+                if any([bool(re.search(key,cmp_baseDict['name'])) for key in self.target_configs.get(target,{}).get('exclComponents',[])]):
+                    return {cmp_baseDict['name']:False}
+                ## if there is an allow list for that property
+                if len(self.target_configs.get(target,{}).get('inclComponents',[]))>0:
+                    if any([bool(re.search(key,cmp_baseDict['name'])) for key in self.target_configs.get(target,{}).get('inclComponents',[])]):
+                        flagAllowList = True
+                ## if there is no allow list for that property, or no match in the list of target properties, or component was allow
+                if len(self.target_configs.get(target,{}).get('inclComponents',[]))==0 or flagAllowList:
+                    ## if rule does not exist
+                    if cmp_baseDict['name'] not in [rule['attributes']['name'] for rule in self.targets[target]['rules']]:
+                        targetRule = self.targets[target]['api'].createRule(
+                            name=cmp_baseDict['name']
+                            )
+                        targetRuleId = targetRule['id']
+                        self.translator.extendTargetRules(ruleName=cmp_baseDict['name'],ruleId=targetRuleId,property_name=target)
+                        self.targets[target]['rules'].append(targetRule)
+                        index = len(self.targets[target]['rules'])-1
+                        self.targets[target]['libraryStack']['rules'].append(targetRule)
+                        for rc in template_ruleComponents:
+                            translatedComponent = self.translator.translate(target,rule_component=copySettings(rc))
+                            translatedComponent['rule_setting']['data'][0]['id'] = targetRuleId
+                            targetRuleComponent = self.targets[target]['api'].createRuleComponent(
+                                name=translatedComponent['name'],
+                                settings = translatedComponent['settings'],
+                                descriptor = translatedComponent['descriptor'],
+                                extension_infos = translatedComponent['extension'],
+                                rule_infos = translatedComponent['rule_setting'],
+                                rule_order=translatedComponent['rule_order'],
+                                order=translatedComponent['order'],
+                                negate=translatedComponent['negate'],
+                                delay_next=translatedComponent['delay_next'],
+                                timeout=translatedComponent['timeout'],
+                            )
+                    else: ## if a rule exist with the same name
+                        index, targetRule = [(index,rule) for index, rule in enumerate(self.targets[target]['rules']) if rule['attributes']['name'] == cmp_baseDict['name']][0]
+                        self.targets[target]['libraryStack']['rules'].append(targetRule)
+                        targetRuleId = targetRule['id']
+                        rcsLinkTarget = targetRule.get('relationships',{}).get('rule_components',{}).get('links',{}).get('related')
+                        resResource = self.targets[target]['api'].getRessource(rcsLinkTarget)
+                        old_components:list = resResource['data']
+                        ## deleting the old version of rule component
+                        if len(old_components)>0:
+                            for component in old_components:
+                                self.targets[target]['api'].deleteRuleComponent(component['id'])
+                        ## creating the new version of the old version
+                        for rc in template_ruleComponents:
+                            translatedComponent = self.translator.translate(target,rule_component=copySettings(rc))
+                            translatedComponent['rule_setting']['data'][0]['id'] = targetRuleId
+                            targetRuleComponent = self.targets[target]['api'].createRuleComponent(
+                                name=translatedComponent['name'],
+                                settings = translatedComponent['settings'],
+                                descriptor = translatedComponent['descriptor'],
+                                extension_infos = translatedComponent['extension'],
+                                rule_infos = translatedComponent['rule_setting'],
+                                rule_order=translatedComponent['rule_order'],
+                                order=translatedComponent['order'],
+                                negate=translatedComponent['negate'],
+                                delay_next=translatedComponent['delay_next'],
+                                timeout=translatedComponent['timeout'],
+                            )
+                    ## updating rule attribute if difference between base and target
+                    if cmp_baseDict['component']['attributes']['enabled'] != targetRule['attributes']['enabled']:
+                        baseRuleAttr = copySettings(cmp_baseDict['component'])
+                        targetRule = self.targets[target]['api'].updateRule(rule_id=targetRuleId,attr_dict=baseRuleAttr) ## keeping in a var for debug
+                        del self.targets[target]['rules'][index]
+                        self.targets[target]['rules'].append(targetRule)
 
     def syncComponents(self,componentsName:list=None,componentsId:list=None,publishedVersion:bool=False)->None:
         """
         Sync multiple components by looping through the list of name passed.
         Arguments:
             componentsName : REQUIRED : The list of component names to sync
             componentsId : REQUIRED : The list of component ID to sync
```

### Comparing `launchpy-0.4.0.post3/launchpy.egg-info/PKG-INFO` & `launchpy-0.4.1/launchpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launchpy
-Version: 0.4.0.post3
+Version: 0.4.1
 Summary: Python wrapper around the Adobe Experience Launch API.
 Home-page: https://github.com/pitchmuc/launchpy
 Author: Julien Piccini
 Author-email: piccini.julien@gmail.com
 Keywords: adobe,Launch,API,python,Tag Manager
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `launchpy-0.4.0.post3/setup.py` & `launchpy-0.4.1/setup.py`

 * *Files identical despite different names*

