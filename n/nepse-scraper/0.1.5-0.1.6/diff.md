# Comparing `tmp/nepse_scraper-0.1.5.tar.gz` & `tmp/nepse_scraper-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nepse_scraper-0.1.5.tar", last modified: Wed May  3 11:29:14 2023, max compression
+gzip compressed data, was "nepse_scraper-0.1.6.tar", last modified: Thu May 11 02:05:59 2023, max compression
```

## Comparing `nepse_scraper-0.1.5.tar` & `nepse_scraper-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 11:29:14.969710 nepse_scraper-0.1.5/
--rw-rw-rw-   0        0        0     1085 2023-05-03 09:07:21.000000 nepse_scraper-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0     3186 2023-05-03 11:29:14.969710 nepse_scraper-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2510 2023-05-03 11:26:57.000000 nepse_scraper-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 11:29:14.923796 nepse_scraper-0.1.5/nepse_scraper/
--rw-rw-rw-   0        0        0    25306 2023-05-03 11:01:38.000000 nepse_scraper-0.1.5/nepse_scraper/Scraper.py
--rw-rw-rw-   0        0        0       50 2023-05-03 06:38:36.000000 nepse_scraper-0.1.5/nepse_scraper/__init__.py
--rw-rw-rw-   0        0        0     1717 2023-05-03 11:26:30.000000 nepse_scraper-0.1.5/nepse_scraper/apis.py
--rw-rw-rw-   0        0        0     5032 2023-05-01 16:07:59.000000 nepse_scraper-0.1.5/nepse_scraper/nepse.wasm
-drwxrwxrwx   0        0        0        0 2023-05-03 11:29:14.967702 nepse_scraper-0.1.5/nepse_scraper.egg-info/
--rw-rw-rw-   0        0        0     3186 2023-05-03 11:29:14.000000 nepse_scraper-0.1.5/nepse_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-05-03 11:29:14.000000 nepse_scraper-0.1.5/nepse_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 11:29:14.000000 nepse_scraper-0.1.5/nepse_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-05-03 11:29:14.000000 nepse_scraper-0.1.5/nepse_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-03 11:29:14.000000 nepse_scraper-0.1.5/nepse_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-03 11:29:14.972247 nepse_scraper-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1182 2023-05-03 11:27:45.000000 nepse_scraper-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 02:05:59.391182 nepse_scraper-0.1.6/
+-rw-rw-rw-   0        0        0     1085 2023-05-03 09:07:21.000000 nepse_scraper-0.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     2879 2023-05-11 02:05:59.391182 nepse_scraper-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2203 2023-05-10 16:47:44.000000 nepse_scraper-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 02:05:59.357246 nepse_scraper-0.1.6/nepse_scraper/
+-rw-rw-rw-   0        0        0    25906 2023-05-11 01:51:35.000000 nepse_scraper-0.1.6/nepse_scraper/Scraper.py
+-rw-rw-rw-   0        0        0       50 2023-05-10 16:47:44.000000 nepse_scraper-0.1.6/nepse_scraper/__init__.py
+-rw-rw-rw-   0        0        0     1717 2023-05-03 11:26:30.000000 nepse_scraper-0.1.6/nepse_scraper/apis.py
+-rw-rw-rw-   0        0        0     5032 2023-05-01 16:07:59.000000 nepse_scraper-0.1.6/nepse_scraper/nepse.wasm
+drwxrwxrwx   0        0        0        0 2023-05-11 02:05:59.389182 nepse_scraper-0.1.6/nepse_scraper.egg-info/
+-rw-rw-rw-   0        0        0     2879 2023-05-11 02:05:59.000000 nepse_scraper-0.1.6/nepse_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-05-11 02:05:59.000000 nepse_scraper-0.1.6/nepse_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 02:05:59.000000 nepse_scraper-0.1.6/nepse_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-05-11 02:05:59.000000 nepse_scraper-0.1.6/nepse_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-11 02:05:59.000000 nepse_scraper-0.1.6/nepse_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-11 02:05:59.393608 nepse_scraper-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1182 2023-05-11 02:04:25.000000 nepse_scraper-0.1.6/setup.py
```

### Comparing `nepse_scraper-0.1.5/LICENSE.txt` & `nepse_scraper-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nepse_scraper-0.1.5/PKG-INFO` & `nepse_scraper-0.1.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 Metadata-Version: 2.1
 Name: nepse_scraper
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python Scraper for Nepse
 Home-page: https://github.com/polymorphisma/nepse_scraper/
-Download-URL: https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.5.tar.gz
+Download-URL: https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.6.tar.gz
 Author: Shrawan Sunar
 Author-email: shrawansunar.6@gmail.com
 Keywords: python,nepse data,nepse scraper
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# _NEPSE_SCRAPER_
+# Nepse scraper
+> Python module that provides convenient access to the Nepal Stock Exchange (NEPSE) API, enabling developers and analysts to retrieve stock market data and improve investment decisions.
 
-Welcome to **nepse_scraper**, the Python module that provides easy access to the Nepal Stock Exchange (NEPSE) API. With just a few lines of code, you can retrieve today's stock prices, market summary, head indices and etc to help you make better investment decisions. The code is well-documented and organized, making it easy to understand and modify for your specific use case.
+# Table of content
+- [Introduction](#introduction)
+- [Features](#features)
+- [Installation](#installation)
+  - [Using Pip](#using-pip)
+- [Usage](#usage)
+- [Documentation](/docs/index.md)
+- [License](#license)
 
-But that's not all! With the power of Python libraries such as **pandas**, you can quickly process the retrieved data and convert it into your desired format.
+## Introduction
+Welcome to **nepse_scraper**, the Python module that provides easy access to the Nepal Stock Exchange (NEPSE) API. With just a few lines of code, you can retrieve today's stock prices, market summary, head indices and etc to help you make better investment decisions. The code is well-documented and organized, making it easy to understand and modify for your specific use case.
 
 **nepse_scraper** is open-source, which means you can contribute and improve the code by adding new functions to retrieve additional data, enhancing existing functions with more options, or improving the error handling and exception handling to make it more robust. Your contributions can help make **nepse_scraper** even more useful for developers and analysts who work with data from the Nepal Stock Exchange.
 
 So what are you waiting for? Try out **nepse_scraper** and see how it can simplify your stock market analysis and investment strategies.
 
 
 ## Features
@@ -48,61 +57,29 @@
 
 ## Installation
 
 ### Using Pip
 ```
 pip install nepse-scraper
 ```
-### Cloning 
-
-```
-git clone git@github.com:polymorphisma/nepse_scraper.git
-```
-#### Downloading Dependencies
-```
-pip install -r requirements.txt
-```
-
-_or_ 
 
-```
-pip install requests urllib3 wasmtime retrying
-```
 
 ## Usage
 ```py
 from nepse_scraper import Request_module
 
 # create object from Request_module class
 request_obj = Request_module()
 
 # getting today's price from nepse
 today_price = request_obj.get_today_price()
 print(today_price)
-```
 
+# "Please refer to the documentation for more detailed usage instructions."
+```
 
-## All Methods
-- get_news()
-- get_head_indices() 
-- get_market_summary()
-- get_sectorwise_summary()
-- get_today_price() 
-- is_trading_day()
-- get_top_gainer() 
-- get_top_loser() 
-- get_top_trade() 
-- get_top_transaction()
-- get_top_turnover() 
-- get_today_market_summary()
-- get_security_detail()
-- get_marketcap()
-- get_trading_average()
-- get_sector_detail()
-- get_live_stock()
-- is_market_open()
 
 ## License
 
 MIT
 
 **Free Software, Hell Yeah!**
```

### Comparing `nepse_scraper-0.1.5/README.md` & `nepse_scraper-0.1.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,21 @@
-# _NEPSE_SCRAPER_
+# Nepse scraper
+> Python module that provides convenient access to the Nepal Stock Exchange (NEPSE) API, enabling developers and analysts to retrieve stock market data and improve investment decisions.
 
-Welcome to **nepse_scraper**, the Python module that provides easy access to the Nepal Stock Exchange (NEPSE) API. With just a few lines of code, you can retrieve today's stock prices, market summary, head indices and etc to help you make better investment decisions. The code is well-documented and organized, making it easy to understand and modify for your specific use case.
+# Table of content
+- [Introduction](#introduction)
+- [Features](#features)
+- [Installation](#installation)
+  - [Using Pip](#using-pip)
+- [Usage](#usage)
+- [Documentation](/docs/index.md)
+- [License](#license)
 
-But that's not all! With the power of Python libraries such as **pandas**, you can quickly process the retrieved data and convert it into your desired format.
+## Introduction
+Welcome to **nepse_scraper**, the Python module that provides easy access to the Nepal Stock Exchange (NEPSE) API. With just a few lines of code, you can retrieve today's stock prices, market summary, head indices and etc to help you make better investment decisions. The code is well-documented and organized, making it easy to understand and modify for your specific use case.
 
 **nepse_scraper** is open-source, which means you can contribute and improve the code by adding new functions to retrieve additional data, enhancing existing functions with more options, or improving the error handling and exception handling to make it more robust. Your contributions can help make **nepse_scraper** even more useful for developers and analysts who work with data from the Nepal Stock Exchange.
 
 So what are you waiting for? Try out **nepse_scraper** and see how it can simplify your stock market analysis and investment strategies.
 
 
 ## Features
@@ -31,61 +40,29 @@
 
 ## Installation
 
 ### Using Pip
 ```
 pip install nepse-scraper
 ```
-### Cloning 
-
-```
-git clone git@github.com:polymorphisma/nepse_scraper.git
-```
-#### Downloading Dependencies
-```
-pip install -r requirements.txt
-```
-
-_or_ 
 
-```
-pip install requests urllib3 wasmtime retrying
-```
 
 ## Usage
 ```py
 from nepse_scraper import Request_module
 
 # create object from Request_module class
 request_obj = Request_module()
 
 # getting today's price from nepse
 today_price = request_obj.get_today_price()
 print(today_price)
-```
 
+# "Please refer to the documentation for more detailed usage instructions."
+```
 
-## All Methods
-- get_news()
-- get_head_indices() 
-- get_market_summary()
-- get_sectorwise_summary()
-- get_today_price() 
-- is_trading_day()
-- get_top_gainer() 
-- get_top_loser() 
-- get_top_trade() 
-- get_top_transaction()
-- get_top_turnover() 
-- get_today_market_summary()
-- get_security_detail()
-- get_marketcap()
-- get_trading_average()
-- get_sector_detail()
-- get_live_stock()
-- is_market_open()
 
 ## License
 
 MIT
 
 **Free Software, Hell Yeah!**
```

### Comparing `nepse_scraper-0.1.5/nepse_scraper/Scraper.py` & `nepse_scraper-0.1.6/nepse_scraper/Scraper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,600 +1,600 @@
-import requests
-from datetime import datetime, date
-from urllib3.exceptions import InsecureRequestWarning
-from urllib3 import disable_warnings
-import time
-from wasmtime import Store,Module,Instance
-import json
-import os
-
-import pkg_resources
-WASM_FILE = pkg_resources.resource_filename(__name__, 'nepse.wasm')
-
-
-# WASM_FILE = r'nepse.wasm'
-from .apis import api_dict
-
-ROOT_URL = 'https://www.nepalstock.com.np'
-
-class TokenParser():
-    def __init__(self):
-        self.store = Store()
-        module = Module.from_file(self.store.engine, WASM_FILE)
-        instance = Instance(self.store,module,[])
-
-        self.cdx = instance.exports(self.store)["cdx"]
-        self.rdx = instance.exports(self.store)["rdx"]
-        self.bdx = instance.exports(self.store)["bdx"]
-        self.ndx = instance.exports(self.store)["ndx"]
-        self.mdx = instance.exports(self.store)["mdx"]
-        
-
-    def parse_token_response(self, token_response):
-        n = self.cdx(self.store,token_response['salt1'], token_response['salt2'], token_response['salt3'], token_response['salt4'], token_response['salt5'])
-        l = self.rdx(self.store,token_response['salt1'], token_response['salt2'], token_response['salt4'], token_response['salt3'], token_response['salt5'])
-        o = self.bdx(self.store,token_response['salt1'], token_response['salt2'], token_response['salt4'], token_response['salt3'], token_response['salt5'])
-        p = self.ndx(self.store,token_response['salt1'], token_response['salt2'], token_response['salt4'], token_response['salt3'], token_response['salt5'])
-        q = self.mdx(self.store,token_response['salt1'], token_response['salt2'], token_response['salt4'], token_response['salt3'], token_response['salt5'])
-        
-        i = self.cdx(self.store,token_response['salt2'], token_response['salt1'], token_response['salt3'], token_response['salt5'], token_response['salt4'])
-        r = self.rdx(self.store,token_response['salt2'], token_response['salt1'], token_response['salt3'], token_response['salt4'], token_response['salt5'])
-        s = self.bdx(self.store,token_response['salt2'], token_response['salt1'], token_response['salt4'], token_response['salt3'], token_response['salt5'])
-        t = self.ndx(self.store,token_response['salt2'], token_response['salt1'], token_response['salt4'], token_response['salt3'], token_response['salt5'])
-        u = self.mdx(self.store,token_response['salt2'], token_response['salt1'], token_response['salt4'], token_response['salt3'], token_response['salt5'])
-
-        access_token  = token_response['accessToken']
-        refresh_token = token_response['refreshToken']
-        
-        parsed_access_token = access_token[0:n] + access_token[n+1:l] + access_token[l+1:o] + access_token[o+1:p] + access_token[p+1:q] + access_token[q+1:]
-        parsed_refresh_token = refresh_token[0:i] + refresh_token[i+1:r] + refresh_token[r+1:s] + refresh_token[s+1:t] + refresh_token[t+1:u] + refresh_token[u+1:]
-        
-        return (parsed_access_token, parsed_refresh_token)
-
-class PayloadParser():
-    def __init__(self):
-        self.dummyData = [147, 117, 239, 143, 157, 312, 161, 612, 512, 804, 411, 527, 170, 511, 421, 667, 764, 621, 301, 106, 133, 793, 411, 511, 312, 423, 344, 346, 653, 758, 342, 222, 236, 811, 711, 611, 122, 447, 128, 199, 183, 135, 489, 703, 800, 745, 152, 863, 134, 211, 142, 564, 375, 793, 212, 153, 138, 153, 648, 611, 151, 649, 318, 143, 117, 756, 119, 141, 717, 113, 112, 146, 162, 660, 693, 261, 362, 354, 251, 641, 157, 178, 631, 192, 734, 445, 192, 883, 187, 122, 591, 731, 852, 384, 565, 596, 451, 772, 624, 691]
-        self.url = ROOT_URL + api_dict["marketopen_api"]["api"]
-        self.method = api_dict["marketopen_api"]['method']
-        self.payload = {}
-        self.headers = {
-            "authority": "www.nepalstock.com.np",
-            "accept": "application/json, text/plain, */*",
-            "accept-language": "en-US,en;q=0.5",
-            "referer": "https://www.nepalstock.com.np",
-            "sec-ch-ua": '"Not_A Brand";v="99", "Brave";v="109", "Chromium";v="109"',
-            "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": '"Windows"',
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "cors",
-            "sec-fetch-site": "same-origin",
-            "sec-gpc": "1",
-            "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36",
-        }
-
-    def return_payload(self, access_token_value, which=None):
-        headers = {'Authorization': f'Salter {access_token_value[0]}', **self.headers}
-        
-        response = requests.request(self.method, self.url, headers=headers, data=self.payload, verify=False)
-        given_id = json.loads(response.content)["id"]
-        
-        today = datetime.now().day
-        
-        payload_id = self.dummyData[given_id] + given_id + 2 * today
-
-        if which == 'stock-live':
-            return payload_id
-
-        if which == 'sector-live':
-            if payload_id % 10 < 5:
-                index_value = 3
-            else:
-                index_value = 1
-        else:
-            if payload_id % 10 < 5:
-                index_value = 1
-            else:
-                index_value = 3
-
-        payload_id = payload_id + access_token_value[1].get(f"salt{index_value+1}") *  today - access_token_value[1].get(f"salt{index_value}")
-
-        return payload_id
-
-class Nepse:
-    """
-    this is the main class which gets the data from nepse
-    
-    Paramaters:
-        optional str: date_value
-            which date data you want(only works for todays date to exact one year before time period)
-            
-    """
-    def __init__(self):
-        self.parser_obj = PayloadParser()
-        self.token_parser= TokenParser()
-
-        self.token_url = ROOT_URL + api_dict['authenticate_api']['api'] 
-        self.token_method = api_dict['authenticate_api']['method'] 
-
-        self.headers = {
-            'Host': 'www.nepalstock.com.np',
-            'User-Agent': 'Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:89.0) Gecko/20100101 Firefox/89.0',
-            'Accept': 'application/json, text/plain, */*',
-            'Accept-Language': 'en-US,en;q=0.5',
-            'Accept-Encoding': 'gzip, deflate, br',
-            'Connection': 'keep-alive',
-            'Referer': 'https://www.nepalstock.com.np/',
-            'Pragma': 'no-cache',
-            'Cache-Control': 'no-cache',
-            'TE': 'Trailers',
-        }
-
-    def request_api(self, url, access_token, method='GET', which_payload = None, querystring = None, payload=None):
-        """
-        this method/fucnion returns the data form requested url in json format
-        
-        Parameters
-            str: url
-                url of the api you want to get data from
-                
-            str: access_token
-                this can be generated from get_valid_token() function(only works if given get_valid_token() generated token)
-                
-            str: Method
-                this is optional can pass 'POST', 'GET'
-        Returns
-            json: what
-                returns the json file accured after requsting to the api
-        """
-        headers = {'Authorization': f'Salter {access_token[0]}', **self.headers}
-
-        if payload == None:
-            payload = {'id': self.parser_obj.return_payload(access_token, which=which_payload)}
-
-        # Send the request with the given parameters
-        try:
-            response = requests.request(
-                method=method,
-                url=url,
-                headers=headers,
-                json=payload,
-                params=querystring,
-                verify=False
-            )
-            # shranavyawan
-            response.raise_for_status()  # Raise an exception if the response status code is not successful
-            return response
-        
-        except Exception as exp:
-            raise ValueError(f"Error sending request: {exp}")
-        
-
-    def get_valid_token(self):
-        """
-        IMP
-        
-        this function is used to generate the access token to by pass authantication of the nepalstock.com.np
-        
-        Parameters
-            None
-        Returns
-            str: acess_token
-        """
-        header = self.headers
-        disable_warnings(InsecureRequestWarning)
-
-        token_response = requests.request(self.token_method, self.token_url, headers=header, verify=False).json()
-        for salt_index in range(1, 6):
-            token_response[f'salt{salt_index}'] = int(token_response[f'salt{salt_index}'])
-     
-        return [self.token_parser.parse_token_response(token_response)[0], token_response]
-    
-    def return_data(self, url, access_token, method='GET', which_payload=None,  querystring = None, payload=None):
-        return self.request_api(method=method, url = url, access_token = access_token, which_payload=which_payload, querystring=querystring, payload=payload)
-
-from retrying import retry
-
-class Request_module:
-    
-    SLEEP_TIME = 3000 # -> wait time for every failed request(in milisecond)
-
-    def __init__(self) -> None:
-        self.nepse_obj = Nepse()
-        self.desired_status = 200
-
-
-    @retry(wait_fixed = SLEEP_TIME)
-    def call_nepse_function(self, url, method,  querystring=None, payload=None):
-        try:
-            access_token = self.nepse_obj.get_valid_token()
-            response = self.nepse_obj.return_data(url, access_token=access_token, method=method, querystring=querystring, payload=payload)
-
-            if response.status_code != self.desired_status:
-                raise ValueError('Unexpected status code: {}'.format(response.status_code))
-            # print(response.json())
-            return response.json()
-        
-        except Exception as exp:
-            raise ValueError('Unexpected Error: {}'.format(exp))
-        
-    def is_trading_day(self) -> bool:
-        """
-        Check if today is a trading day on the Nepal Stock Exchange (NEPSE).
-
-        This method queries the NEPSE API to determine if today is a trading day or not.
-        If today is a trading day, it returns True, otherwise it returns False.
-
-        Returns:
-            bool: True if today is a trading day, False otherwise.
-        """
-        api = ROOT_URL + api_dict['marketopen_api']['api']
-        method = api_dict['marketopen_api']['method']
-
-        response = self.call_nepse_function(url=api, method=method)
-
-        date_ = response['asOf'].split('T')[0]
-
-        if date_ != str(date.today()):
-            return False
-        
-        return True
-    
-    def is_market_open(self) -> bool:
-        """
-        Check if today is a trading day on the Nepal Stock Exchange (NEPSE).
-
-        This method queries the NEPSE API to determine if today is a trading day or not.
-        If today is a trading day, it returns True, otherwise it returns False.
-
-        Returns:
-            bool: True if today is a trading day, False otherwise.
-        """
-
-        api = ROOT_URL + api_dict['marketopen_api']['api']
-        method = api_dict['marketopen_api']['method']
-
-        response = self.call_nepse_function(url=api, method=method)
-
-        isOpen = response['isOpen']
-
-        if isOpen != 'OPEN':
-            return False
-        
-        return True
-
-    def get_today_price(self, date_ : str = None) -> json:
-        """
-        Get today's trading data for from Nepal Stock Exchange (NEPSE).
-
-        This method queries the NEPSE API to retrieve the trading data for the current date or a specified date.
-        The data is returned as a json response.
-
-        Args:
-            date_ (str, optional): The date for which trading data should be retrieved in "YYYY-MM-DD" format. Defaults to None,
-                which retrieves data for the current date.(Date should be from today to one year prior)
-
-        Returns:
-            json: A json response returned by NEPSE API.
-
-        Raises:
-            ValueError: If the date string is not in the "YYYY-MM-DD" format.
-        """
-        api = ROOT_URL + api_dict['today_price_api']['api']
-        method = api_dict['today_price_api']['method']
-
-        querystring = {"page":"0","size":"500","businessDate":date_}
-
-        return self.call_nepse_function(url=api, method=method, querystring=querystring)
-    
-    def get_head_indices(self) -> dict:
-        """
-        Retrieve the head indices data from the Nepal Stock Exchange (NEPSE).
-
-        This method reads the head indices file located at paths.headindices_path and queries the NEPSE API to retrieve
-        data. The data is returned as a dictionary containing index as keys and the corresponding index data as values.
-
-        Returns:
-            dict: A dictionary containing the latest data for each head index, with index as keys and response as a value.
-        """
-        api = ROOT_URL + api_dict['head_indices_api']['api']
-        print(api)
-        method = api_dict['head_indices_api']['method']
-
-        querystring = {"page":"0","size":"500"}
-
-        dicts = {}
-
-        sector_index = self._get_sector_index()
-        
-        for val in sector_index:
-            dicts[val['id']] = self.call_nepse_function(url=api + '/' + str(val['id']), method=method, querystring=querystring)
-
-        return dicts
-    
-    def get_sectorwise_summary(self, date_ : str =None) -> json:
-        """
-        Retrieve the sector-wise summary from a given business date from the Nepal Stock Exchange (NEPSE).
-
-        This method queries the NEPSE API to retrieve the sector-wise summary for a given business date.
-        If no date is specified, the default behavior is to retrieve the sector-wise summary for the current business date.
-        The sector-wise summary is returned as a json response from NEPSE API.
-
-        Args:
-            date_ (str, optional): The business date for which to retrieve the sector-wise summary, in YYYY-MM-DD format.
-                Defaults to None, in which case the sector-wise summary for all the data avialable on {nepalstock.com.np}.
-
-        Returns:
-            json: A json response returned by NEPSE API.
-        """
-
-        api = ROOT_URL + api_dict['sectorwise_summary_api']['api']
-        method = api_dict['sectorwise_summary_api']['method']
-
-        querystring = {"page":"0","size":"500","businessDate":date_}
-
-        return self.call_nepse_function(url=api, method=method, querystring=querystring)
-
-    def get_market_summary(self, date_ : str = None) -> json:
-        """
-        Retrieve the market summary from a given business date from the Nepal Stock Exchange (NEPSE).
-
-        This method queries the NEPSE API to retrieve the market summary for a given business date.
-        If no date is specified, the default behavior is to retrieve the market summary for the current business date.
-        The market summary is returned as a dictionary with various statistics as keys and corresponding values.
-
-        Args:
-            date_ (str, optional): The business date for which to retrieve the market summary, in YYYY-MM-DD format.
-            Defaults to None, in which case the market summary for the current business date is retrieved.
-
-        Returns:
-            json: A json response returned by NEPSE API.
-        """
-        api = ROOT_URL + api_dict['market_summary_history_api']['api']
-        method = api_dict['market_summary_history_api']['method']
-
-        querystring = {"page":"0","size":"500","businessDate":date_}
-
-        return self.call_nepse_function(url=api, method=method, querystring=querystring)
-    
-    def get_news(self) -> json:
-        """
-        Retrieve the latest news and announcements from the Nepal Stock Exchange (NEPSE).
-
-        This method queries the NEPSE API to retrieve the latest news and announcements regarding listed companies.
-        The news and announcements are returned as a json.
-
-        Returns:
-            json: A json response returned by NEPSE API.
-        """
-        api = ROOT_URL + api_dict['disclosure']['api']
-        method = api_dict['disclosure']['method']
-
-        return self.call_nepse_function(url=api, method=method)
-    
-    def get_top_gainer(self) -> json:
-        """
-        Retrieve the all the gains of ticker in terms of share price from the Nepal Stock Exchange (NEPSE).
-
-        This method queries the NEPSE API to retrieve the all the gains of ticker in terms of share price.
-        The all the gains of ticker are returned as a json.
-
-        Returns:
-            json: A json response returned by NEPSE API.
-        """
-        api = ROOT_URL + api_dict['top_gainer']['api']
-        method = api_dict['top_gainer']['method']
-
-
-        return self.call_nepse_function(url=api, method=method)
-    
-    def get_top_loser(self) -> json:
-        """
-        Retrieve the all the loser of ticker in terms of share price from the Nepal Stock Exchange (NEPSE).
-
-        This method queries the NEPSE API to retrieve the all the loser of ticker in terms of share price.
-        The all the loser of ticker are returned as a json.
-
-        Returns:
-            json: A json response returned by NEPSE API.
-        """
-        api = ROOT_URL + api_dict['top_loser']['api']
-        method = api_dict['top_loser']['method']
-
-        return self.call_nepse_function(url=api, method=method)
-    
-    def get_top_turnover(self) -> json:
-        """
-        Retrieve the all the turnover of ticker in terms of share price from the Nepal Stock Exchange (NEPSE).
-
-        This method queries the NEPSE API to retrieve the all the turnover of ticker in terms of share price.
-        The all the turnover of ticker are returned as a json.
-
-        Returns:
-            json: A json response returned by NEPSE API.
-        """
-        api = ROOT_URL + api_dict['top_turnover']['api']
-        method = api_dict['top_turnover']['method']
-
-
-        return self.call_nepse_function(url=api, method=method)
-
-    def get_top_trade(self) -> json:
-        """
-        Retrieve the all the trade of ticker in terms of share price from the Nepal Stock Exchange (NEPSE).
-
-        This method queries the NEPSE API to retrieve the all the trade of ticker in terms of share price.
-        The all the trade of ticker are returned as a json.
-
-        Returns:
-            json: A json response returned by NEPSE API.
-        """
-        api = ROOT_URL + api_dict['top_trade']['api']
-        method = api_dict['top_trade']['method']
-
-        return self.call_nepse_function(url=api, method=method)
-
-    def get_top_transaction(self) -> json:
-        """
-        Retrieve the all the transaction of ticker in terms of share price from the Nepal Stock Exchange (NEPSE).
-
-        This method queries the NEPSE API to retrieve the all the transaction of ticker in terms of share price.
-        The all the transaction of ticker are returned as a json.
-
-        Returns:
-            json: A json response returned by NEPSE API.
-        """
-        api = ROOT_URL + api_dict['top_transaction']['api']
-        method = api_dict['top_transaction']['method']
-
-        return self.call_nepse_function(url=api, method=method)
-    
-    def get_today_market_summary(self) -> json:
-
-        """
-        Retrieve today's market summary from the Nepal Stock Exchange (NEPSE).
-
-        This method queries the NEPSE API to retrieve today's market summary, which includes information
-        such as the current NEPSE index value, trading volume, and the number of transactions.
-
-        Returns:
-            json: A json response returned by NEPSE API.
-        """
-        api = ROOT_URL + api_dict['market_summary_api']['api']
-        method = api_dict['market_summary_api']['method']
-
-        return self.call_nepse_function(url=api, method=method)
-
-    def get_security_detail(self) -> json:
-        """
-        Retrieve security detail information from the Nepal Stock Exchange (NEPSE).
-
-        This method queries the NEPSE API to retrieve security detail information, which includes the
-        names and codes of all listed securities on the NEPSE, along with their market prices and other
-        relevant data.
-
-        Returns:
-            json: A json response returned by NEPSE API.
-        """
-        api = ROOT_URL + api_dict['security_api']['api']
-        method = api_dict['security_api']['method']
-
-        return self.call_nepse_function(url=api, method=method)
-    
-    def get_marketcap(self) -> json:
-        """
-        Retrieve market capitalization data from the Nepal Stock Exchange (NEPSE).
-
-        This method queries the NEPSE API to retrieve market capitalization data for all listed securities
-        on the NEPSE.
-
-        Returns:
-            json: A json response returned by NEPSE API.
-        """
-        api = ROOT_URL + api_dict['marketcap_api']['api']
-        method = api_dict['marketcap_api']['method']
-
-        return self.call_nepse_function(url=api, method=method)
-    
-
-    def get_trading_average(self, date_ : str = None, n_days : int =120) -> json:
-        """
-        Retrieve the trading average for the specified number of days ending on the given date (or today if date is not
-        specified).
-
-        Args:
-            date_: A string representing the date (in YYYY-MM-DD format) for which to retrieve the trading average. If
-                not specified, the method will retrieve the trading average for today.
-            n_days: An integer representing the number of days to include in the trading average calculation. The default
-                value is 120.
-        Returns:
-            json: A json response returned by NEPSE API.
-        Raises:
-            ValueError: If n_days is less than or equal to zero.
-        """
-        if n_days < 1 or n_days > 180:
-            raise ValueError(r"n_days must be between 1 and 180")
-        
-        api = ROOT_URL + api_dict['trading_average_api']['api']
-        method = api_dict['trading_average_api']['method']
-
-        querystring = {"page":"0","size":"500","businessDate":date_,"nDays":n_days}
-
-        return self.call_nepse_function(url=api, method=method, querystring=querystring)
-    
-    def get_broker(self, member_name : str= "", contact_person : str ="", contact_number : str = "", member_code : str ="", province_id : int = 0, district_id : int = 0, municipality_id : int= 0):
-        """
-        Get broker information from NEPSE.
-
-        Args:
-            member_name (str, optional): The name of the broker member. Defaults to "".
-            contact_person (str, optional): The contact person name of the broker. Defaults to "".
-            contact_number (str, optional): The contact number of the broker. Defaults to "".
-            member_code (str, optional): The code of the broker member. Defaults to "".
-            province_id (int, optional): The ID of the province where the broker is located. Defaults to 0.
-            district_id (int, optional): The ID of the district where the broker is located. Defaults to 0.
-            municipality_id (int, optional): The ID of the municipality where the broker is located. Defaults to 0.
-
-        Returns:
-            json: A json response returned by NEPSE API.
-        """
-        api = ROOT_URL + api_dict['broker_api']['api']
-        method = api_dict['broker_api']['method']
-        querystring = {"page":"0","size":"500"}
-
-
-        payload = {
-            "memberName": member_name,
-            "contactPerson": contact_person,
-            "contactNumber": contact_number,
-            "memberCode": member_code,
-            "provinceId": province_id,
-            "districtId": district_id,
-            "municipalityId": municipality_id
-        }
-
-        return self.call_nepse_function(url=api, method=method, querystring=querystring, payload=payload)
-    
-    def get_sector_detail(self):
-        """
-        Retrieve details of all sectors listed in the NEPSE.
-
-        Returns:
-            json: A json response returned by NEPSE API.
-        """
-        api = ROOT_URL + api_dict['sector_api']['api']
-        method = api_dict['sector_api']['method']
-        querystring = {"page":"0","size":"500"}
-
-        return self.call_nepse_function(url=api, method=method, querystring=querystring)
-    
-    def _get_sector_index(self):
-        """
-        Retrieve idnex of all sectors listed in the NEPSE.
-
-        Returns:
-            json: A json response returned by NEPSE API.
-        """
-        api = ROOT_URL + api_dict['sector_index_api']['api']
-        method = api_dict['sector_index_api']['method']
-        querystring = {"page":"0","size":"500"}
-
-        return self.call_nepse_function(url=api, method=method, querystring=querystring)
-    
-    def get_live_stock(self):
-        if not(self.is_market_open()):
-            raise ValueError('Market Already closed')
-        
-        api = ROOT_URL + api_dict['stock_live_api']['api']
-        method = api_dict['stock_live_api']['method']
-
-        return self.call_nepse_function(url=api, method=method, payload='stock-live')
-    
-
-    # # incomplete pyload not working
-    # def get_nepse_live(self):
-    #     if not(self.is_market_open()):
-    #         raise ValueError('Market Already closed')
-
-    #     api = ROOT_URL + api_dict['nepse_live_api']['api']
-    #     method = api_dict['nepse_live_api']['method']
-
-    #     return self.call_nepse_function(url=api, method=method, payload='sector-live')
+import requests
+from datetime import datetime, date
+from urllib3.exceptions import InsecureRequestWarning
+from urllib3 import disable_warnings
+import time
+from wasmtime import Store,Module,Instance
+import json
+import os
+
+import pkg_resources
+WASM_FILE = pkg_resources.resource_filename(__name__, 'nepse.wasm')
+
+
+# WASM_FILE = r'nepse.wasm'
+from .apis import api_dict
+
+ROOT_URL = 'https://www.nepalstock.com.np'
+
+class TokenParser():
+    def __init__(self):
+        self.store = Store()
+        module = Module.from_file(self.store.engine, WASM_FILE)
+        instance = Instance(self.store,module,[])
+
+        self.cdx = instance.exports(self.store)["cdx"]
+        self.rdx = instance.exports(self.store)["rdx"]
+        self.bdx = instance.exports(self.store)["bdx"]
+        self.ndx = instance.exports(self.store)["ndx"]
+        self.mdx = instance.exports(self.store)["mdx"]
+        
+
+    def parse_token_response(self, token_response):
+        n = self.cdx(self.store,token_response['salt1'], token_response['salt2'], token_response['salt3'], token_response['salt4'], token_response['salt5'])
+        l = self.rdx(self.store,token_response['salt1'], token_response['salt2'], token_response['salt4'], token_response['salt3'], token_response['salt5'])
+        o = self.bdx(self.store,token_response['salt1'], token_response['salt2'], token_response['salt4'], token_response['salt3'], token_response['salt5'])
+        p = self.ndx(self.store,token_response['salt1'], token_response['salt2'], token_response['salt4'], token_response['salt3'], token_response['salt5'])
+        q = self.mdx(self.store,token_response['salt1'], token_response['salt2'], token_response['salt4'], token_response['salt3'], token_response['salt5'])
+        
+        i = self.cdx(self.store,token_response['salt2'], token_response['salt1'], token_response['salt3'], token_response['salt5'], token_response['salt4'])
+        r = self.rdx(self.store,token_response['salt2'], token_response['salt1'], token_response['salt3'], token_response['salt4'], token_response['salt5'])
+        s = self.bdx(self.store,token_response['salt2'], token_response['salt1'], token_response['salt4'], token_response['salt3'], token_response['salt5'])
+        t = self.ndx(self.store,token_response['salt2'], token_response['salt1'], token_response['salt4'], token_response['salt3'], token_response['salt5'])
+        u = self.mdx(self.store,token_response['salt2'], token_response['salt1'], token_response['salt4'], token_response['salt3'], token_response['salt5'])
+
+        access_token  = token_response['accessToken']
+        refresh_token = token_response['refreshToken']
+        
+        parsed_access_token = access_token[0:n] + access_token[n+1:l] + access_token[l+1:o] + access_token[o+1:p] + access_token[p+1:q] + access_token[q+1:]
+        parsed_refresh_token = refresh_token[0:i] + refresh_token[i+1:r] + refresh_token[r+1:s] + refresh_token[s+1:t] + refresh_token[t+1:u] + refresh_token[u+1:]
+        
+        return (parsed_access_token, parsed_refresh_token)
+
+class PayloadParser():
+    def __init__(self):
+        self.dummyData = [147, 117, 239, 143, 157, 312, 161, 612, 512, 804, 411, 527, 170, 511, 421, 667, 764, 621, 301, 106, 133, 793, 411, 511, 312, 423, 344, 346, 653, 758, 342, 222, 236, 811, 711, 611, 122, 447, 128, 199, 183, 135, 489, 703, 800, 745, 152, 863, 134, 211, 142, 564, 375, 793, 212, 153, 138, 153, 648, 611, 151, 649, 318, 143, 117, 756, 119, 141, 717, 113, 112, 146, 162, 660, 693, 261, 362, 354, 251, 641, 157, 178, 631, 192, 734, 445, 192, 883, 187, 122, 591, 731, 852, 384, 565, 596, 451, 772, 624, 691]
+        self.url = ROOT_URL + api_dict["marketopen_api"]["api"]
+        self.method = api_dict["marketopen_api"]['method']
+        self.payload = {}
+        self.headers = {
+            "authority": "www.nepalstock.com.np",
+            "accept": "application/json, text/plain, */*",
+            "accept-language": "en-US,en;q=0.5",
+            "referer": "https://www.nepalstock.com.np",
+            "sec-ch-ua": '"Not_A Brand";v="99", "Brave";v="109", "Chromium";v="109"',
+            "sec-ch-ua-mobile": "?0",
+            "sec-ch-ua-platform": '"Windows"',
+            "sec-fetch-dest": "empty",
+            "sec-fetch-mode": "cors",
+            "sec-fetch-site": "same-origin",
+            "sec-gpc": "1",
+            "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36",
+        }
+
+    def return_payload(self, access_token_value, which=None):
+        headers = {'Authorization': f'Salter {access_token_value[0]}', **self.headers}
+        
+        response = requests.request(self.method, self.url, headers=headers, data=self.payload, verify=False)
+        given_id = json.loads(response.content)["id"]
+        
+        today = datetime.now().day
+        
+        payload_id = self.dummyData[given_id] + given_id + 2 * today
+
+        if which == 'stock-live':
+            return payload_id
+
+        if which == 'sector-live':
+            if payload_id % 10 < 5:
+                index_value = 3
+            else:
+                index_value = 1
+        else:
+            if payload_id % 10 < 5:
+                index_value = 1
+            else:
+                index_value = 3
+
+        payload_id = payload_id + access_token_value[1].get(f"salt{index_value+1}") *  today - access_token_value[1].get(f"salt{index_value}")
+
+        return payload_id
+
+class Nepse:
+    """
+    this is the main class which gets the data from nepse
+    
+    Paramaters:
+        optional str: date_value
+            which date data you want(only works for todays date to exact one year before time period)
+            
+    """
+    def __init__(self):
+        self.parser_obj = PayloadParser()
+        self.token_parser= TokenParser()
+
+        self.token_url = ROOT_URL + api_dict['authenticate_api']['api'] 
+        self.token_method = api_dict['authenticate_api']['method'] 
+
+        self.headers = {
+            'Host': 'www.nepalstock.com.np',
+            'User-Agent': 'Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:89.0) Gecko/20100101 Firefox/89.0',
+            'Accept': 'application/json, text/plain, */*',
+            'Accept-Language': 'en-US,en;q=0.5',
+            'Accept-Encoding': 'gzip, deflate, br',
+            'Connection': 'keep-alive',
+            'Referer': 'https://www.nepalstock.com.np/',
+            'Pragma': 'no-cache',
+            'Cache-Control': 'no-cache',
+            'TE': 'Trailers',
+        }
+
+    def request_api(self, url, access_token, method='GET', which_payload = None, querystring = None, payload=None):
+        """
+        this method/fucnion returns the data form requested url in json format
+        
+        Parameters
+            str: url
+                url of the api you want to get data from
+                
+            str: access_token
+                this can be generated from get_valid_token() function(only works if given get_valid_token() generated token)
+                
+            str: Method
+                this is optional can pass 'POST', 'GET'
+        Returns
+            json: what
+                returns the json file accured after requsting to the api
+        """
+        headers = {'Authorization': f'Salter {access_token[0]}', **self.headers}
+
+        if payload == None:
+            payload = {'id': self.parser_obj.return_payload(access_token, which=which_payload)}
+
+        # Send the request with the given parameters
+        try:
+            response = requests.request(
+                method=method,
+                url=url,
+                headers=headers,
+                json=payload,
+                params=querystring,
+                verify=False
+            )
+            # shranavyawan
+            response.raise_for_status()  # Raise an exception if the response status code is not successful
+            return response
+        
+        except Exception as exp:
+            raise ValueError(f"Error sending request: {exp}")
+        
+
+    def get_valid_token(self):
+        """
+        IMP
+        
+        this function is used to generate the access token to by pass authantication of the nepalstock.com.np
+        
+        Parameters
+            None
+        Returns
+            str: acess_token
+        """
+        header = self.headers
+        disable_warnings(InsecureRequestWarning)
+
+        token_response = requests.request(self.token_method, self.token_url, headers=header, verify=False).json()
+        for salt_index in range(1, 6):
+            token_response[f'salt{salt_index}'] = int(token_response[f'salt{salt_index}'])
+     
+        return [self.token_parser.parse_token_response(token_response)[0], token_response]
+    
+    def return_data(self, url, access_token, method='GET', which_payload=None,  querystring = None, payload=None):
+        return self.request_api(method=method, url = url, access_token = access_token, which_payload=which_payload, querystring=querystring, payload=payload)
+
+from retrying import retry
+
+class Request_module:
+    
+    SLEEP_TIME = 3000 # -> wait time for every failed request(in milisecond)
+
+    def __init__(self) -> None:
+        self.nepse_obj = Nepse()
+        self.desired_status = 200
+
+
+    @retry(wait_fixed = SLEEP_TIME)
+    def call_nepse_function(self, url, method,  querystring=None, payload=None):
+        try:
+            access_token = self.nepse_obj.get_valid_token()
+            response = self.nepse_obj.return_data(url, access_token=access_token, method=method, querystring=querystring, payload=payload)
+
+            if response.status_code != self.desired_status:
+                raise ValueError('Unexpected status code: {}'.format(response.status_code))
+            # print(response.json())
+            return response.json()
+        
+        except Exception as exp:
+            raise ValueError('Unexpected Error: {}'.format(exp))
+        
+    def is_trading_day(self) -> bool:
+        """
+        Check if today is a trading day on the Nepal Stock Exchange (NEPSE).
+
+        This method queries the NEPSE API to determine if today is a trading day or not.
+        If today is a trading day, it returns True, otherwise it returns False.
+
+        Returns:
+            bool: True if today is a trading day, False otherwise.
+        """
+        api = ROOT_URL + api_dict['marketopen_api']['api']
+        method = api_dict['marketopen_api']['method']
+
+        response = self.call_nepse_function(url=api, method=method)
+
+        date_ = response['asOf'].split('T')[0]
+
+        if date_ != str(date.today()):
+            return False
+        
+        return True
+    
+    def is_market_open(self) -> bool:
+        """
+        Check if today is a trading day on the Nepal Stock Exchange (NEPSE).
+
+        This method queries the NEPSE API to determine if today is a trading day or not.
+        If today is a trading day, it returns True, otherwise it returns False.
+
+        Returns:
+            bool: True if today is a trading day, False otherwise.
+        """
+
+        api = ROOT_URL + api_dict['marketopen_api']['api']
+        method = api_dict['marketopen_api']['method']
+
+        response = self.call_nepse_function(url=api, method=method)
+
+        isOpen = response['isOpen']
+
+        if isOpen != 'OPEN':
+            return False
+        
+        return True
+
+    def get_today_price(self, date_ : str = None) -> json:
+        """
+        Get today's trading data for from Nepal Stock Exchange (NEPSE).
+
+        This method queries the NEPSE API to retrieve the trading data for the current date or a specified date.
+        The data is returned as a json response.
+
+        Args:
+            date_ (str, optional): The date for which trading data should be retrieved in "YYYY-MM-DD" format. Defaults to None,
+                which retrieves data for the current date.(Date should be from today to one year prior)
+
+        Returns:
+            json: A json response returned by NEPSE API.
+
+        Raises:
+            ValueError: If the date string is not in the "YYYY-MM-DD" format.
+        """
+        api = ROOT_URL + api_dict['today_price_api']['api']
+        method = api_dict['today_price_api']['method']
+
+        querystring = {"page":"0","size":"500","businessDate":date_}
+
+        return self.call_nepse_function(url=api, method=method, querystring=querystring)
+    
+    def get_head_indices(self) -> dict:
+        """
+        Retrieve the head indices data from the Nepal Stock Exchange (NEPSE).
+
+        This method reads the head indices file located at paths.headindices_path and queries the NEPSE API to retrieve
+        data. The data is returned as a dictionary containing index as keys and the corresponding index data as values.
+
+        Returns:
+            dict: A dictionary containing the latest data for each head index, with index as keys and response as a value.
+        """
+        api = ROOT_URL + api_dict['head_indices_api']['api']
+        print(api)
+        method = api_dict['head_indices_api']['method']
+
+        querystring = {"page":"0","size":"500"}
+
+        dicts = {}
+
+        sector_index = self._get_sector_index()
+        
+        for val in sector_index:
+            dicts[val['id']] = self.call_nepse_function(url=api + '/' + str(val['id']), method=method, querystring=querystring)
+
+        return dicts
+    
+    def get_sectorwise_summary(self, date_ : str =None) -> json:
+        """
+        Retrieve the sector-wise summary from a given business date from the Nepal Stock Exchange (NEPSE).
+
+        This method queries the NEPSE API to retrieve the sector-wise summary for a given business date.
+        If no date is specified, the default behavior is to retrieve the sector-wise summary for the current business date.
+        The sector-wise summary is returned as a json response from NEPSE API.
+
+        Args:
+            date_ (str, optional): The business date for which to retrieve the sector-wise summary, in YYYY-MM-DD format.
+                Defaults to None, in which case the sector-wise summary for all the data avialable on {nepalstock.com.np}.
+
+        Returns:
+            json: A json response returned by NEPSE API.
+        """
+
+        api = ROOT_URL + api_dict['sectorwise_summary_api']['api']
+        method = api_dict['sectorwise_summary_api']['method']
+
+        querystring = {"page":"0","size":"500","businessDate":date_}
+
+        return self.call_nepse_function(url=api, method=method, querystring=querystring)
+
+    def get_market_summary(self, date_ : str = None) -> json:
+        """
+        Retrieve the market summary from a given business date from the Nepal Stock Exchange (NEPSE).
+
+        This method queries the NEPSE API to retrieve the market summary for a given business date.
+        If no date is specified, the default behavior is to retrieve the market summary for the current business date.
+        The market summary is returned as a dictionary with various statistics as keys and corresponding values.
+
+        Args:
+            date_ (str, optional): The business date for which to retrieve the market summary, in YYYY-MM-DD format.
+            Defaults to None, in which case the market summary for the current business date is retrieved.
+
+        Returns:
+            json: A json response returned by NEPSE API.
+        """
+        api = ROOT_URL + api_dict['market_summary_history_api']['api']
+        method = api_dict['market_summary_history_api']['method']
+
+        querystring = {"page":"0","size":"500","businessDate":date_}
+
+        return self.call_nepse_function(url=api, method=method, querystring=querystring)
+    
+    def get_news(self) -> json:
+        """
+        Retrieve the latest news and announcements from the Nepal Stock Exchange (NEPSE).
+
+        This method queries the NEPSE API to retrieve the latest news and announcements regarding listed companies.
+        The news and announcements are returned as a json.
+
+        Returns:
+            json: A json response returned by NEPSE API.
+        """
+        api = ROOT_URL + api_dict['disclosure']['api']
+        method = api_dict['disclosure']['method']
+
+        return self.call_nepse_function(url=api, method=method)
+    
+    def get_top_gainer(self) -> json:
+        """
+        Retrieve the all the gains of ticker in terms of share price from the Nepal Stock Exchange (NEPSE).
+
+        This method queries the NEPSE API to retrieve the all the gains of ticker in terms of share price.
+        The all the gains of ticker are returned as a json.
+
+        Returns:
+            json: A json response returned by NEPSE API.
+        """
+        api = ROOT_URL + api_dict['top_gainer']['api']
+        method = api_dict['top_gainer']['method']
+
+
+        return self.call_nepse_function(url=api, method=method)
+    
+    def get_top_loser(self) -> json:
+        """
+        Retrieve the all the loser of ticker in terms of share price from the Nepal Stock Exchange (NEPSE).
+
+        This method queries the NEPSE API to retrieve the all the loser of ticker in terms of share price.
+        The all the loser of ticker are returned as a json.
+
+        Returns:
+            json: A json response returned by NEPSE API.
+        """
+        api = ROOT_URL + api_dict['top_loser']['api']
+        method = api_dict['top_loser']['method']
+
+        return self.call_nepse_function(url=api, method=method)
+    
+    def get_top_turnover(self) -> json:
+        """
+        Retrieve the all the turnover of ticker in terms of share price from the Nepal Stock Exchange (NEPSE).
+
+        This method queries the NEPSE API to retrieve the all the turnover of ticker in terms of share price.
+        The all the turnover of ticker are returned as a json.
+
+        Returns:
+            json: A json response returned by NEPSE API.
+        """
+        api = ROOT_URL + api_dict['top_turnover']['api']
+        method = api_dict['top_turnover']['method']
+
+
+        return self.call_nepse_function(url=api, method=method)
+
+    def get_top_trade(self) -> json:
+        """
+        Retrieve the all the trade of ticker in terms of share price from the Nepal Stock Exchange (NEPSE).
+
+        This method queries the NEPSE API to retrieve the all the trade of ticker in terms of share price.
+        The all the trade of ticker are returned as a json.
+
+        Returns:
+            json: A json response returned by NEPSE API.
+        """
+        api = ROOT_URL + api_dict['top_trade']['api']
+        method = api_dict['top_trade']['method']
+
+        return self.call_nepse_function(url=api, method=method)
+
+    def get_top_transaction(self) -> json:
+        """
+        Retrieve the all the transaction of ticker in terms of share price from the Nepal Stock Exchange (NEPSE).
+
+        This method queries the NEPSE API to retrieve the all the transaction of ticker in terms of share price.
+        The all the transaction of ticker are returned as a json.
+
+        Returns:
+            json: A json response returned by NEPSE API.
+        """
+        api = ROOT_URL + api_dict['top_transaction']['api']
+        method = api_dict['top_transaction']['method']
+
+        return self.call_nepse_function(url=api, method=method)
+    
+    def get_today_market_summary(self) -> json:
+
+        """
+        Retrieve today's market summary from the Nepal Stock Exchange (NEPSE).
+
+        This method queries the NEPSE API to retrieve today's market summary, which includes information
+        such as the current NEPSE index value, trading volume, and the number of transactions.
+
+        Returns:
+            json: A json response returned by NEPSE API.
+        """
+        api = ROOT_URL + api_dict['market_summary_api']['api']
+        method = api_dict['market_summary_api']['method']
+
+        return self.call_nepse_function(url=api, method=method)
+
+    def get_security_detail(self) -> json:
+        """
+        Retrieve security detail information from the Nepal Stock Exchange (NEPSE).
+
+        This method queries the NEPSE API to retrieve security detail information, which includes the
+        names and codes of all listed securities on the NEPSE, along with their market prices and other
+        relevant data.
+
+        Returns:
+            json: A json response returned by NEPSE API.
+        """
+        api = ROOT_URL + api_dict['security_api']['api']
+        method = api_dict['security_api']['method']
+
+        return self.call_nepse_function(url=api, method=method)
+    
+    def get_marketcap(self) -> json:
+        """
+        Retrieve market capitalization data from the Nepal Stock Exchange (NEPSE).
+
+        This method queries the NEPSE API to retrieve market capitalization data for all listed securities
+        on the NEPSE.
+
+        Returns:
+            json: A json response returned by NEPSE API.
+        """
+        api = ROOT_URL + api_dict['marketcap_api']['api']
+        method = api_dict['marketcap_api']['method']
+
+        return self.call_nepse_function(url=api, method=method)
+    
+
+    def get_trading_average(self, date_ : str = None, n_days : int =120) -> json:
+        """
+        Retrieve the trading average for the specified number of days ending on the given date (or today if date is not
+        specified).
+
+        Args:
+            date_: A string representing the date (in YYYY-MM-DD format) for which to retrieve the trading average. If
+                not specified, the method will retrieve the trading average for today.
+            n_days: An integer representing the number of days to include in the trading average calculation. The default
+                value is 120.
+        Returns:
+            json: A json response returned by NEPSE API.
+        Raises:
+            ValueError: If n_days is less than or equal to zero.
+        """
+        if n_days < 1 or n_days > 180:
+            raise ValueError(r"n_days must be between 1 and 180")
+        
+        api = ROOT_URL + api_dict['trading_average_api']['api']
+        method = api_dict['trading_average_api']['method']
+
+        querystring = {"page":"0","size":"500","businessDate":date_,"nDays":n_days}
+
+        return self.call_nepse_function(url=api, method=method, querystring=querystring)
+    
+    def get_broker(self, member_name : str= "", contact_person : str ="", contact_number : str = "", member_code : str ="", province_id : int = 0, district_id : int = 0, municipality_id : int= 0):
+        """
+        Get broker information from NEPSE.
+
+        Args:
+            member_name (str, optional): The name of the broker member. Defaults to "".
+            contact_person (str, optional): The contact person name of the broker. Defaults to "".
+            contact_number (str, optional): The contact number of the broker. Defaults to "".
+            member_code (str, optional): The code of the broker member. Defaults to "".
+            province_id (int, optional): The ID of the province where the broker is located. Defaults to 0.
+            district_id (int, optional): The ID of the district where the broker is located. Defaults to 0.
+            municipality_id (int, optional): The ID of the municipality where the broker is located. Defaults to 0.
+
+        Returns:
+            json: A json response returned by NEPSE API.
+        """
+        api = ROOT_URL + api_dict['broker_api']['api']
+        method = api_dict['broker_api']['method']
+        querystring = {"page":"0","size":"500"}
+
+        payload = {
+            "memberName": member_name,
+            "contactPerson": contact_person,
+            "contactNumber": contact_number,
+            "memberCode": member_code,
+            "provinceId": province_id,
+            "districtId": district_id,
+            "municipalityId": municipality_id
+        }
+
+        return self.call_nepse_function(url=api, method=method, querystring=querystring, payload=payload)
+    
+    def get_sector_detail(self):
+        """
+        Retrieve details of all sectors listed in the NEPSE.
+        Returns:
+            json: A json response returned by NEPSE API.
+        """
+        api = ROOT_URL + api_dict['sector_api']['api']
+        method = api_dict['sector_api']['method']
+        querystring = {"page":"0","size":"500"}
+
+        return self.call_nepse_function(url=api, method=method, querystring=querystring)
+    
+    def _get_sector_index(self):
+        """
+        Retrieve index of all sectors listed in the NEPSE.
+
+        Returns:
+            json: A json response returned by NEPSE API.
+        """
+        api = ROOT_URL + api_dict['sector_index_api']['api']
+        method = api_dict['sector_index_api']['method']
+        querystring = {"page":"0","size":"500"}
+
+        return self.call_nepse_function(url=api, method=method, querystring=querystring)
+    
+    def get_live_stock(self):
+        if not(self.is_market_open()):
+            raise ValueError('Market Already closed')
+        
+        api = ROOT_URL + api_dict['stock_live_api']['api']
+        method = api_dict['stock_live_api']['method']
+
+        return self.call_nepse_function(url=api, method=method, payload='stock-live')
+    
+
+    # # incomplete pyload not working
+    # def get_nepse_live(self):
+    #     if not(self.is_market_open()):
+    #         raise ValueError('Market Already closed')
+
+    #     api = ROOT_URL + api_dict['nepse_live_api']['api']
+    #     method = api_dict['nepse_live_api']['method']
+
+    #     return self.call_nepse_function(url=api, method=method, payload='sector-live')
+
+
```

### Comparing `nepse_scraper-0.1.5/nepse_scraper/apis.py` & `nepse_scraper-0.1.6/nepse_scraper/apis.py`

 * *Files identical despite different names*

### Comparing `nepse_scraper-0.1.5/nepse_scraper/nepse.wasm` & `nepse_scraper-0.1.6/nepse_scraper/nepse.wasm`

 * *Files identical despite different names*

### Comparing `nepse_scraper-0.1.5/nepse_scraper.egg-info/PKG-INFO` & `nepse_scraper-0.1.6/nepse_scraper.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 Metadata-Version: 2.1
 Name: nepse-scraper
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python Scraper for Nepse
 Home-page: https://github.com/polymorphisma/nepse_scraper/
-Download-URL: https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.5.tar.gz
+Download-URL: https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.6.tar.gz
 Author: Shrawan Sunar
 Author-email: shrawansunar.6@gmail.com
 Keywords: python,nepse data,nepse scraper
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# _NEPSE_SCRAPER_
+# Nepse scraper
+> Python module that provides convenient access to the Nepal Stock Exchange (NEPSE) API, enabling developers and analysts to retrieve stock market data and improve investment decisions.
 
-Welcome to **nepse_scraper**, the Python module that provides easy access to the Nepal Stock Exchange (NEPSE) API. With just a few lines of code, you can retrieve today's stock prices, market summary, head indices and etc to help you make better investment decisions. The code is well-documented and organized, making it easy to understand and modify for your specific use case.
+# Table of content
+- [Introduction](#introduction)
+- [Features](#features)
+- [Installation](#installation)
+  - [Using Pip](#using-pip)
+- [Usage](#usage)
+- [Documentation](/docs/index.md)
+- [License](#license)
 
-But that's not all! With the power of Python libraries such as **pandas**, you can quickly process the retrieved data and convert it into your desired format.
+## Introduction
+Welcome to **nepse_scraper**, the Python module that provides easy access to the Nepal Stock Exchange (NEPSE) API. With just a few lines of code, you can retrieve today's stock prices, market summary, head indices and etc to help you make better investment decisions. The code is well-documented and organized, making it easy to understand and modify for your specific use case.
 
 **nepse_scraper** is open-source, which means you can contribute and improve the code by adding new functions to retrieve additional data, enhancing existing functions with more options, or improving the error handling and exception handling to make it more robust. Your contributions can help make **nepse_scraper** even more useful for developers and analysts who work with data from the Nepal Stock Exchange.
 
 So what are you waiting for? Try out **nepse_scraper** and see how it can simplify your stock market analysis and investment strategies.
 
 
 ## Features
@@ -48,61 +57,29 @@
 
 ## Installation
 
 ### Using Pip
 ```
 pip install nepse-scraper
 ```
-### Cloning 
-
-```
-git clone git@github.com:polymorphisma/nepse_scraper.git
-```
-#### Downloading Dependencies
-```
-pip install -r requirements.txt
-```
-
-_or_ 
 
-```
-pip install requests urllib3 wasmtime retrying
-```
 
 ## Usage
 ```py
 from nepse_scraper import Request_module
 
 # create object from Request_module class
 request_obj = Request_module()
 
 # getting today's price from nepse
 today_price = request_obj.get_today_price()
 print(today_price)
-```
 
+# "Please refer to the documentation for more detailed usage instructions."
+```
 
-## All Methods
-- get_news()
-- get_head_indices() 
-- get_market_summary()
-- get_sectorwise_summary()
-- get_today_price() 
-- is_trading_day()
-- get_top_gainer() 
-- get_top_loser() 
-- get_top_trade() 
-- get_top_transaction()
-- get_top_turnover() 
-- get_today_market_summary()
-- get_security_detail()
-- get_marketcap()
-- get_trading_average()
-- get_sector_detail()
-- get_live_stock()
-- is_market_open()
 
 ## License
 
 MIT
 
 **Free Software, Hell Yeah!**
```

### Comparing `nepse_scraper-0.1.5/setup.py` & `nepse_scraper-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from os import path
 
 current_dir = path.abspath(path.dirname(__file__))
 
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 DESCRIPTION = 'Python Scraper for Nepse'
 
 with open(path.join(current_dir, 'README.md'), encoding='utf-8') as f:
     LONG_DESCRIPTION = f.read()
 
 # Setting up
 setup(
@@ -19,15 +19,15 @@
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     url='https://github.com/polymorphisma/nepse_scraper/',  
     install_requires=['requests','urllib3','wasmtime', 'retrying'],
     keywords=['python', 'nepse data', 'nepse scraper'],
-    download_url="https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.5.tar.gz",
+    download_url="https://github.com/polymorphisma/nepse_scraper/archive/refs/tags/v_01.6.tar.gz",
     classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
   ],
```

