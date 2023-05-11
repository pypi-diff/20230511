# Comparing `tmp/Pydule-3.3.1.tar.gz` & `tmp/Pydule-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pydule-3.3.1.tar", last modified: Fri May  5 02:17:53 2023, max compression
+gzip compressed data, was "Pydule-3.3.2.tar", last modified: Wed May 10 16:27:41 2023, max compression
```

## Comparing `Pydule-3.3.1.tar` & `Pydule-3.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 02:17:53.116360 Pydule-3.3.1/
--rw-rw-rw-   0        0        0     2452 2023-05-05 02:17:53.085102 Pydule-3.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1649 2023-05-04 14:22:20.000000 Pydule-3.3.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 02:17:53.116360 Pydule-3.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1427 2023-05-05 02:14:36.000000 Pydule-3.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 02:17:53.022621 Pydule-3.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-05 02:17:53.085102 Pydule-3.3.1/src/Pydule.egg-info/
--rw-rw-rw-   0        0        0     2452 2023-05-05 02:17:51.000000 Pydule-3.3.1/src/Pydule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-05-05 02:17:51.000000 Pydule-3.3.1/src/Pydule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 02:17:51.000000 Pydule-3.3.1/src/Pydule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      181 2023-05-05 02:17:51.000000 Pydule-3.3.1/src/Pydule.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 02:17:51.000000 Pydule-3.3.1/src/Pydule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12486 2023-05-05 02:15:21.000000 Pydule-3.3.1/src/Pydule.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:27:41.453933 Pydule-3.3.2/
+-rw-rw-rw-   0        0        0     2448 2023-05-10 16:27:41.445361 Pydule-3.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1699 2023-05-10 15:01:16.000000 Pydule-3.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-10 16:27:41.453933 Pydule-3.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1403 2023-05-10 16:22:27.000000 Pydule-3.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:27:41.385505 Pydule-3.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 16:27:41.434187 Pydule-3.3.2/src/Pydule.egg-info/
+-rw-rw-rw-   0        0        0     2448 2023-05-10 16:27:40.000000 Pydule-3.3.2/src/Pydule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-05-10 16:27:40.000000 Pydule-3.3.2/src/Pydule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 16:27:40.000000 Pydule-3.3.2/src/Pydule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2023-05-10 16:27:40.000000 Pydule-3.3.2/src/Pydule.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-10 16:27:40.000000 Pydule-3.3.2/src/Pydule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12750 2023-05-10 16:19:47.000000 Pydule-3.3.2/src/Pydule.py
```

### Comparing `Pydule-3.3.1/PKG-INFO` & `Pydule-3.3.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Pydule
-Version: 3.3.1
-Summary: Access ChatGPT,Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..
+Version: 3.3.2
+Summary: Access ChatGPT,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..
 Author: D.Tamil Mutharasan
 Keywords: python,PyDule,Module,Pydule,pydule,matrix,qrcode,youtube,weather,list,tuple,set,dictionary,clear,color,pick_color,open,app,search,play,mp3,song,restart,system,shutdown,date,time,text_to_speech,text,speech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,14 @@
 
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)                 
 [![Python 3.6](https://img.shields.io/badge/python-3.10.7-blue.svg)](https://www.python.org/downloads/release/python-3107/)   
 
 ## Functionality of Pydule
 
 - Access ChatGPT
-- Download Mp3 or Mp4 From Youtube
 - Encode and Decode a String
 - Record Screen,Internal Audio and Microphone
 - Seperate String
 - Swap Dictionary's Key to Values and Values to Key
 - Insert Elements in Tuple & String
 - Generate Qrcode
 - Copy Text
@@ -59,14 +58,20 @@
 # to Swap Dictionary
 d={1:2,2:3,3:4}
 print(py.swapdict(d))
 
 # to Encode String
 string,Key=py.codestr('Hello World')
 
+# to Code the String
+x,y=py.codestr('Hi') #This Converts Hi to @^&-+*^+^=##&*
+
+# to Decode the String
+print(py.dcodestr(x,py.swapdict(y)))
+
 # to Decode String
 print(py.dcodestr(string,swapdict(key)))
 
 # to Create Qrcode
 text,filename='Hello World','Hello.png'
 py.cqrcode(text,filename)
 
@@ -75,13 +80,10 @@
 
 # to Open Calculator
 py.openapp('calculator')
 
 # to Copy Text
 py.copytext('Hello World')
 
-# to Download Youtube Audio
-py.ytmp3('YOUR LINK HERE')
-
-# to Download Youtube Video with Audio
-py.ytmp4('YOUR LINK HERE')
+# to Access ChatGPT
+print(py.ChatGPT('Hi There','Your API Key'))
   ```
```

### Comparing `Pydule-3.3.1/README.md` & `Pydule-3.3.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)                 
 [![Python 3.6](https://img.shields.io/badge/python-3.10.7-blue.svg)](https://www.python.org/downloads/release/python-3107/)   
 
 ## Functionality of Pydule
 
 - Access ChatGPT
-- Download Mp3 or Mp4 From Youtube
 - Encode and Decode a String
 - Record Screen,Internal Audio and Microphone
 - Seperate String
 - Swap Dictionary's Key to Values and Values to Key
 - Insert Elements in Tuple & String
 - Generate Qrcode
 - Copy Text
@@ -45,14 +44,20 @@
 # to Swap Dictionary
 d={1:2,2:3,3:4}
 print(py.swapdict(d))
 
 # to Encode String
 string,Key=py.codestr('Hello World')
 
+# to Code the String
+x,y=py.codestr('Hi') #This Converts Hi to @^&-+*^+^=##&*
+
+# to Decode the String
+print(py.dcodestr(x,py.swapdict(y)))
+
 # to Decode String
 print(py.dcodestr(string,swapdict(key)))
 
 # to Create Qrcode
 text,filename='Hello World','Hello.png'
 py.cqrcode(text,filename)
 
@@ -61,13 +66,10 @@
 
 # to Open Calculator
 py.openapp('calculator')
 
 # to Copy Text
 py.copytext('Hello World')
 
-# to Download Youtube Audio
-py.ytmp3('YOUR LINK HERE')
-
-# to Download Youtube Video with Audio
-py.ytmp4('YOUR LINK HERE')
+# to Access ChatGPT
+print(py.ChatGPT('Hi There','Your API Key'))
   ```
```

### Comparing `Pydule-3.3.1/setup.py` & `Pydule-3.3.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import setuptools
 
 with open('README.md','r') as fh:
 	long_description = fh.read()
 
 setup(
 	name='Pydule',
-	version='3.3.1',
-	description="Access ChatGPT,Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..",
+	version='3.3.2',
+	description="Access ChatGPT,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..",
 	author='D.Tamil Mutharasan',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	packages=setuptools.find_packages(),
 	keywords=['python','PyDule','Module','Pydule','pydule','matrix','qrcode','youtube','weather','list','tuple','set','dictionary','clear','color','pick_color','open','app','search','play','mp3','song','restart','system','shutdown','date','time','text_to_speech','text','speech'],
 	classifiers=[
 		"Programming Language :: Python :: 3",
@@ -29,20 +29,21 @@
 		'pywhatkit',
 		'playsound',
 		'datetime',
 		'requests',
 		'AppOpener',
 		'deep_translator',
 		'qrcode',
-		'pytube',
 		'numpy',
 		'pyperclip',
 		'soundfile',
 		'soundcard',
 		'pyautogui',
 		'pyaudio',
 		'wave',
 		'opencv-python',
-		'openai'
+		'openai',
+		'phonenumbers',
+		'SpeechRecognition'
 	]
 
 )
```

### Comparing `Pydule-3.3.1/src/Pydule.egg-info/PKG-INFO` & `Pydule-3.3.2/src/Pydule.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Pydule
-Version: 3.3.1
-Summary: Access ChatGPT,Download Audio From Youtube Video or Video with Audio,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..
+Version: 3.3.2
+Summary: Access ChatGPT,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..
 Author: D.Tamil Mutharasan
 Keywords: python,PyDule,Module,Pydule,pydule,matrix,qrcode,youtube,weather,list,tuple,set,dictionary,clear,color,pick_color,open,app,search,play,mp3,song,restart,system,shutdown,date,time,text_to_speech,text,speech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,14 @@
 
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)                 
 [![Python 3.6](https://img.shields.io/badge/python-3.10.7-blue.svg)](https://www.python.org/downloads/release/python-3107/)   
 
 ## Functionality of Pydule
 
 - Access ChatGPT
-- Download Mp3 or Mp4 From Youtube
 - Encode and Decode a String
 - Record Screen,Internal Audio and Microphone
 - Seperate String
 - Swap Dictionary's Key to Values and Values to Key
 - Insert Elements in Tuple & String
 - Generate Qrcode
 - Copy Text
@@ -59,14 +58,20 @@
 # to Swap Dictionary
 d={1:2,2:3,3:4}
 print(py.swapdict(d))
 
 # to Encode String
 string,Key=py.codestr('Hello World')
 
+# to Code the String
+x,y=py.codestr('Hi') #This Converts Hi to @^&-+*^+^=##&*
+
+# to Decode the String
+print(py.dcodestr(x,py.swapdict(y)))
+
 # to Decode String
 print(py.dcodestr(string,swapdict(key)))
 
 # to Create Qrcode
 text,filename='Hello World','Hello.png'
 py.cqrcode(text,filename)
 
@@ -75,13 +80,10 @@
 
 # to Open Calculator
 py.openapp('calculator')
 
 # to Copy Text
 py.copytext('Hello World')
 
-# to Download Youtube Audio
-py.ytmp3('YOUR LINK HERE')
-
-# to Download Youtube Video with Audio
-py.ytmp4('YOUR LINK HERE')
+# to Access ChatGPT
+print(py.ChatGPT('Hi There','Your API Key'))
   ```
```

### Comparing `Pydule-3.3.1/src/Pydule.py` & `Pydule-3.3.2/src/Pydule.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,46 @@
 
 err='\n \U0000274C Something Went Wrong \U0000274C\n'
 
 def openapp(appname):
 	from AppOpener import open
 	open(appname)
 
+def screenshot(sec=0):
+	import pyautogui
+	import time as t
+	import datetime
+
+	t.sleep(sec)
+
+	myScreenshot = pyautogui.screenshot()
+
+	fname="Pydule Screen Shot-" + str(datetime.datetime.now().strftime("%Y-%m-%d-%H-%M-%S")) + ".png"
+
+	myScreenshot.save(fname)
+
+def SpeechtoText(string=''):
+	if isinstance(string,str):
+		import speech_recognition as sr
+
+		r = sr.Recognizer()
+
+		mic = sr.Microphone()
+
+		with mic as source:
+		    print(string,end='')
+		    audio = r.listen(source)
+
+		try:
+		    return r.recognize_google(audio)
+		except:
+		    print(err)
+	else:
+		print(err)	    
+
 def recintaudio(sec):
 	if isinstance(sec,int):
 		if sec>0:
 			import soundcard as sc
 			import soundfile as sf
 			import datetime
 
@@ -144,20 +176,18 @@
 	for i in string:
 		s+=d[i]
 	for i in d:
 		n=ord(i)
 		e[n]=d[i]	
 	return s,e
 
-def ChatGPT(prompt,path,engine="text-davinci-003",max_tokens=1024,temperature=0.7):
+def ChatGPT(prompt,api_key,engine="text-davinci-003",max_tokens=1024,temperature=0.7):
 	import openai
 
-	file=open(path,'r')
-
-	openai.api_key = file.read()
+	openai.api_key = api_key
 
 	completions = openai.Completion.create(engine=engine,prompt=prompt,max_tokens=max_tokens,n=1,stop=None,temperature=temperature)
 
 	return completions.choices[0].text.strip()
 
 def wjson(data,path):
 	import json
@@ -223,15 +253,15 @@
 				else:
 					new+=j
 		return new
 	else:
 		print(err)			
 
 def functions():
-	l=['ChatGPT(<content>)','recintaudio(<seconds>)','recmic(<seconds>)','recscreen()','mulmatrix(<matrix a>,<matrix b>)','codestr(<str>)','dcodestr(<str>,<dict>)','swapdict(<dict>)','sepstr(<str>)','wjson(<dict>,<path>)','deljsonele(<path>)','upjson(<path>)','copytext(<text_to_copy>)','translate(<sentence>,<language>)','ytmp4(<youtube_link>)','ytmp3(<youtube_link>)','cqrcode(<link>)','summatrix(<matrix a>,<matrix b>)','submatrix(<matrix a>,<matrix b>)','intuple(<tuple>,<index>,<new_element>)','instr(<str>,<index>,<new_element>)','reSet(<old_set>,<new_element>,<old_element>)','reStr(<old_str>,<index>,<new_str>)','reDict(<old_dict>,<old_key>,<new_key>)','reList(<old_list>,<index>,<new_element>)','reTuple(<old_tuple>,<index>,<new_element>)','clist(<length_of_the_list>)','ctuple(<length_of_the_tuple>)','cdict(<length_of_the_dict>)','cset(<length_of_the_set>)','pickcolor()','search(<content>)','playsong(<path>)','restart_system()','shutdown_system()','datetoday()','timenow()','say(<content>)','openfile(<path>)','weathernow(<city_name>)','setvoice(<number_between 0 to 2>)','voicerate(<any_number>)']
+	l=['tracklocation(<phone_number>)','num(<numbers>)','screenshot(<seconds>)','SpeechtoText(<str>)','ChatGPT(<content>,<api>)','recintaudio(<seconds>)','recmic(<seconds>)','recscreen()','mulmatrix(<matrix a>,<matrix b>)','codestr(<str>)','dcodestr(<str>,<dict>)','swapdict(<dict>)','sepstr(<str>)','wjson(<dict>,<path>)','deljsonele(<path>)','upjson(<path>)','copytext(<text_to_copy>)','translate(<sentence>,<language>)','cqrcode(<link>)','summatrix(<matrix a>,<matrix b>)','submatrix(<matrix a>,<matrix b>)','intuple(<tuple>,<index>,<new_element>)','instr(<str>,<index>,<new_element>)','reSet(<old_set>,<new_element>,<old_element>)','reStr(<old_str>,<index>,<new_str>)','reDict(<old_dict>,<old_key>,<new_key>)','reList(<old_list>,<index>,<new_element>)','reTuple(<old_tuple>,<index>,<new_element>)','clist(<length_of_the_list>)','ctuple(<length_of_the_tuple>)','cdict(<length_of_the_dict>)','cset(<length_of_the_set>)','pickcolor()','search(<content>)','playsong(<path>)','restart_system()','shutdown_system()','datetoday()','timenow()','say(<content>)','openfile(<path>)','weathernow(<city_name>)','setvoice(<number_between 0 to 2>)','voicerate(<any_number>)']
 	print('Available Functions : \n')
 	for i in l:
 		print(f'\t{i}')
 
 def summatrix(x,y):
 	import numpy as np
 	result = np.array(x) + np.array(y)
@@ -254,31 +284,14 @@
 	else:
 		print(err)
 
 def translate(content,language):
 	from deep_translator import GoogleTranslator
 	translated = GoogleTranslator(source='auto', target=language.lower()).translate(content)
 	return translated
-
-def ytmp4(link):
-	from pytube import YouTube
-	yt = YouTube(link)
-	stream = yt.streams.get_highest_resolution()
-	stream.download()
-	print('\n\U0001F3AC Video Saved Successfully \U00002714\n')
-	
-def ytmp3(link):
-	from pytube import YouTube
-	yt = YouTube(link)
-	video = yt.streams.filter(only_audio=True).first()
-	ofile = video.download(output_path=".")
-	b, ext = os.path.splitext(ofile)
-	file = b + '.mp3'
-	os.rename(ofile, file)
-	print('\n\U0001F3B6 Audio Saved Successfully \U00002714\n')
 	
 def cqrcode(data,filename):
 	import qrcode
 	img = qrcode.make(data)
 	img.save(filename)
 	print('\nQrcode Saved Successfully \U00002714\n')
 	
@@ -373,23 +386,17 @@
 
 def copytext(string):
 	import pyperclip
 	pyperclip.copy(string)
 	spam=pyperclip.paste()
 
 def pickcolor():
-	root=tk.Tk()
-	root.geometry('250x100')
-	root.title('Color Picker')
-	def n():
-		c=colorchooser.askcolor(title='Pydule Color Picker \U00002714')
-		copytext('\''+str(c[-1])+'\'')
-		print(f'Choosen Color ({c[-1]}) is Copied \U00002714')
-	b=tk.Button(root,text='Pick Color',command=n).pack()
-	root.mainloop()				
+	c=colorchooser.askcolor(title='Pydule Color Picker \U00002714')
+	copytext('\''+str(c[-1])+'\'')
+	print(f'Choosen Color ({c[-1]}) is Copied \U00002714')
 	
 def search(content):
 	import pywhatkit as kt
 	kt.search(content)	
 	print('\nSearching \U0001F50E...\n')		
 	
 def playsong(song_path):
@@ -418,32 +425,47 @@
 	engine.say(content)
 	engine.runAndWait()  
 	
 def openfile(path):
 	os.startfile(path)
 
 def weathernow(place):
-	import requests
-	from bs4 import BeautifulSoup
-	headers = {
-		'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3'}
-
-	def weather(city,place):
-		city = city.replace(" ", "+")
-		res = requests.get(
-			f'https://www.google.com/search?q={city}&oq={city}&aqs=chrome.0.35i39l2j0l4j46j69i60.6128j1j7&sourceid=chrome&ie=UTF-8', headers=headers)
-		soup = BeautifulSoup(res.text, 'html.parser')
-		location = soup.select('#wob_loc')[0].getText().strip()
-		time = soup.select('#wob_dts')[0].getText().strip()
-		info = soup.select('#wob_dc')[0].getText().strip()
-		weather = soup.select('#wob_tm')[0].getText().strip()
-		details=['City Name : '+place,info,weather+'°C']
-		return details
-	city = place+" weather"
-	return weather(city,place)
+	if isinstance(place,str):
+		import requests
+		from bs4 import BeautifulSoup
+		headers = {
+			'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3'}
+
+		def weather(city,place):
+			city = city.replace(" ", "+")
+			res = requests.get(
+				f'https://www.google.com/search?q={city}&oq={city}&aqs=chrome.0.35i39l2j0l4j46j69i60.6128j1j7&sourceid=chrome&ie=UTF-8', headers=headers)
+			soup = BeautifulSoup(res.text, 'html.parser')
+			time = soup.select('#wob_dts')[0].getText().strip()
+			info = soup.select('#wob_dc')[0].getText().strip()
+			weather = soup.select('#wob_tm')[0].getText().strip()
+			details=['City Name : '+place,info,weather+'°C']
+			return details
+		city = place+" weather"
+		return weather(city,place)
+	else:
+		print(err)	
+
+def tracklocation(string):
+	if isinstance(string,str) and len(string)==13:
+		import phonenumbers
+		from phonenumbers import geocoder
+
+		number = phonenumbers.parse(string)
+
+		location = geocoder.description_for_number(number, "en")
+
+		return location
+	else:
+		print(err)	
 
 def setvoice(num):
 	voices=engine.getProperty('voices')
 	engine.setProperty('voice',voices[num].id)	
 
 def voicerate(num):
 	engine.setProperty('rate',num)
```

