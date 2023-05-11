# Comparing `tmp/bambooai-0.1.1.tar.gz` & `tmp/bambooai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambooai-0.1.1.tar", last modified: Tue May  9 12:58:14 2023, max compression
+gzip compressed data, was "bambooai-0.1.2.tar", last modified: Wed May 10 12:54:14 2023, max compression
```

## Comparing `bambooai-0.1.1.tar` & `bambooai-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 12:58:14.028590 bambooai-0.1.1/
--rw-rw-rw-   0        0        0     5507 2023-05-09 12:58:14.028590 bambooai-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5015 2023-05-09 08:27:19.000000 bambooai-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 12:58:13.997590 bambooai-0.1.1/bambooai/
--rw-rw-rw-   0        0        0       30 2023-05-07 07:18:22.000000 bambooai-0.1.1/bambooai/__init__.py
--rw-rw-rw-   0        0        0     7741 2023-05-09 12:51:42.000000 bambooai-0.1.1/bambooai/bambooai.py
-drwxrwxrwx   0        0        0        0 2023-05-09 12:58:14.026589 bambooai-0.1.1/bambooai.egg-info/
--rw-rw-rw-   0        0        0     5507 2023-05-09 12:58:13.000000 bambooai-0.1.1/bambooai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-05-09 12:58:13.000000 bambooai-0.1.1/bambooai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 12:58:13.000000 bambooai-0.1.1/bambooai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-09 12:58:13.000000 bambooai-0.1.1/bambooai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-09 12:58:13.000000 bambooai-0.1.1/bambooai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 12:58:14.029589 bambooai-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      676 2023-05-09 12:54:11.000000 bambooai-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:54:14.956787 bambooai-0.1.2/
+-rw-rw-rw-   0        0        0     5719 2023-05-10 12:54:14.956479 bambooai-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5221 2023-05-10 12:51:46.000000 bambooai-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 12:54:14.948585 bambooai-0.1.2/bambooai/
+-rw-rw-rw-   0        0        0       30 2023-05-07 07:18:22.000000 bambooai-0.1.2/bambooai/__init__.py
+-rw-rw-rw-   0        0        0     9150 2023-05-10 12:25:26.000000 bambooai-0.1.2/bambooai/bambooai.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:54:14.953932 bambooai-0.1.2/bambooai.egg-info/
+-rw-rw-rw-   0        0        0     5719 2023-05-10 12:54:14.000000 bambooai-0.1.2/bambooai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-05-10 12:54:14.000000 bambooai-0.1.2/bambooai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 12:54:14.000000 bambooai-0.1.2/bambooai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-10 12:54:14.000000 bambooai-0.1.2/bambooai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-10 12:54:14.000000 bambooai-0.1.2/bambooai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 12:54:14.957695 bambooai-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      676 2023-05-10 12:48:21.000000 bambooai-0.1.2/setup.py
```

### Comparing `bambooai-0.1.1/PKG-INFO` & `bambooai-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambooai
-Version: 0.1.1
+Version: 0.1.2
 Summary: A lightweight library for working with pandas dataframes using natural language queries
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,20 @@
 
 ## Objective
 
 The BambooAI library is a user-friendly tool designed to make data analysis more accessible to non-programmers. Utilizing the power of Large Language Models (LLM), BambooAI can comprehend your questions about a dataset and automatically generate and execute the appropriate Python code for both analysis and plotting. Users can effortlessly gain valuable insights from their data without writing complex code or mastering advanced programming techniques. With BambooAI, simply input your dataset, ask questions in plain English, and receive answers along with relevant out of the box visualizations if asked for to help you better understand your data.
 
 My aim was to keep the code base under 150 lines of actual code (not counting comments and blanks) to ensure easy comprehension and clarity for users of various skill levels. By maintaining a concise code base, I strived to create an accessible and straightforward tool that streamlines the process of data analysis and visualization. This approach not only makes it easier for developers and users to understand the library's inner workings but also fosters efficient implementation and customization, catering to a diverse audience and their unique needs.
 
+## Preview
+
+Try it out in Google Colab:
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1grKtqKD4u8cVGMoVv__umci4F7IU14vU?usp=sharing)
+
 ## How it works
 
 - User starts BambooAI
 - BambooAI checks if a question is provided
   - If a question is given programmatically, it gets processed and the assistant exits after the execution
   - If no question is provided programaticaly, BambooAI prompts the user for one and enters a loop of questions and answers, remembering the conversation history
     - Sends each question to the OpenAI API LLM along with the conversation history
```

### Comparing `bambooai-0.1.1/README.md` & `bambooai-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 
 ## Objective
 
 The BambooAI library is a user-friendly tool designed to make data analysis more accessible to non-programmers. Utilizing the power of Large Language Models (LLM), BambooAI can comprehend your questions about a dataset and automatically generate and execute the appropriate Python code for both analysis and plotting. Users can effortlessly gain valuable insights from their data without writing complex code or mastering advanced programming techniques. With BambooAI, simply input your dataset, ask questions in plain English, and receive answers along with relevant out of the box visualizations if asked for to help you better understand your data.
 
 My aim was to keep the code base under 150 lines of actual code (not counting comments and blanks) to ensure easy comprehension and clarity for users of various skill levels. By maintaining a concise code base, I strived to create an accessible and straightforward tool that streamlines the process of data analysis and visualization. This approach not only makes it easier for developers and users to understand the library's inner workings but also fosters efficient implementation and customization, catering to a diverse audience and their unique needs.
 
+## Preview
+
+Try it out in Google Colab:
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1grKtqKD4u8cVGMoVv__umci4F7IU14vU?usp=sharing)
+
 ## How it works
 
 - User starts BambooAI
 - BambooAI checks if a question is provided
   - If a question is given programmatically, it gets processed and the assistant exits after the execution
   - If no question is provided programaticaly, BambooAI prompts the user for one and enters a loop of questions and answers, remembering the conversation history
     - Sends each question to the OpenAI API LLM along with the conversation history
```

### Comparing `bambooai-0.1.1/bambooai/bambooai.py` & `bambooai-0.1.2/bambooai/bambooai.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,484 +1,572 @@
 00000000: 0d0a 696d 706f 7274 206f 730d 0a69 6d70  ..import os..imp
 00000010: 6f72 7420 7265 0d0a 696d 706f 7274 2073  ort re..import s
-00000020: 7973 0d0a 696d 706f 7274 2069 6f0d 0a69  ys..import io..i
-00000030: 6d70 6f72 7420 7469 6d65 0d0a 696d 706f  mport time..impo
-00000040: 7274 206f 7065 6e61 690d 0a69 6d70 6f72  rt openai..impor
-00000050: 7420 7061 6e64 6173 2061 7320 7064 0d0a  t pandas as pd..
-00000060: 6672 6f6d 2074 6572 6d63 6f6c 6f72 2069  from termcolor i
-00000070: 6d70 6f72 7420 636f 6c6f 7265 640d 0a0d  mport colored...
-00000080: 0a63 6c61 7373 2042 616d 626f 6f41 493a  .class BambooAI:
-00000090: 0d0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-000000a0: 5f5f 2873 656c 662c 2064 663a 2070 642e  __(self, df: pd.
-000000b0: 4461 7461 4672 616d 652c 206c 6c6d 3a20  DataFrame, llm: 
-000000c0: 7374 7220 3d20 2767 7074 2d33 2e35 2d74  str = 'gpt-3.5-t
-000000d0: 7572 626f 2729 3a0d 0a0d 0a20 2020 2020  urbo'):....     
-000000e0: 2020 2073 656c 662e 4150 495f 4b45 5920     self.API_KEY 
-000000f0: 3d20 6f73 2e65 6e76 6972 6f6e 2e67 6574  = os.environ.get
-00000100: 2827 4f50 454e 4149 5f41 5049 5f4b 4559  ('OPENAI_API_KEY
-00000110: 2729 0d0a 2020 2020 2020 2020 7365 6c66  ')..        self
-00000120: 2e4d 4158 5f45 5252 4f52 5f43 4f52 5245  .MAX_ERROR_CORRE
-00000130: 4354 494f 4e53 203d 2033 0d0a 0d0a 2020  CTIONS = 3....  
-00000140: 2020 2020 2020 7365 6c66 2e64 6620 3d20        self.df = 
-00000150: 6466 0d0a 2020 2020 2020 2020 7365 6c66  df..        self
-00000160: 2e64 665f 6865 6164 203d 2064 662e 6865  .df_head = df.he
-00000170: 6164 2831 290d 0a20 2020 200d 0a20 2020  ad(1)..    ..   
-00000180: 2020 2020 2073 656c 662e 6c6c 6d20 3d20       self.llm = 
-00000190: 6c6c 6d0d 0a0d 0a20 2020 2020 2020 2073  llm....        s
-000001a0: 656c 662e 7461 736b 203d 2022 2222 0d0a  elf.task = """..
-000001b0: 2020 2020 2020 2020 5468 6572 6520 6973          There is
-000001c0: 2061 2070 616e 6461 7320 6461 7461 6672   a pandas datafr
-000001d0: 616d 652e 0d0a 2020 2020 2020 2020 5468  ame...        Th
-000001e0: 6520 6e61 6d65 206f 6620 7468 6520 6461  e name of the da
-000001f0: 7461 6672 616d 6520 6973 2060 6466 602e  taframe is `df`.
-00000200: 0d0a 2020 2020 2020 2020 5468 6973 2069  ..        This i
-00000210: 7320 7468 6520 7265 7375 6c74 206f 6620  s the result of 
-00000220: 6070 7269 6e74 2864 662e 6865 6164 2831  `print(df.head(1
-00000230: 2929 603a 0d0a 2020 2020 2020 2020 7b7d  ))`:..        {}
-00000240: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
-00000250: 7572 6e20 7468 6520 7079 7468 6f6e 2063  urn the python c
-00000260: 6f64 6520 7468 6174 2070 7269 6e74 7320  ode that prints 
-00000270: 6f75 7420 7468 6520 616e 7377 6572 2074  out the answer t
-00000280: 6f20 7468 6520 666f 6c6c 6f77 696e 6720  o the following 
-00000290: 7175 6573 7469 6f6e 203a 207b 7d2e 200d  question : {}. .
-000002a0: 0a20 2020 2020 2020 2050 7265 6669 7820  .        Prefix 
-000002b0: 7468 6520 7079 7468 6f6e 2063 6f64 6520  the python code 
-000002c0: 7769 7468 203c 636f 6465 3e20 616e 6420  with <code> and 
-000002d0: 7375 6666 6978 2074 6865 2063 6f64 6520  suffix the code 
-000002e0: 7769 7468 203c 2f63 6f64 653e 202e 0d0a  with </code> ...
-000002f0: 2020 2020 2020 2020 2222 220d 0a0d 0a20          """.... 
-00000300: 2020 2020 2020 2073 656c 662e 6572 726f         self.erro
-00000310: 725f 636f 7272 6563 745f 7461 736b 203d  r_correct_task =
-00000320: 2022 2222 0d0a 2020 2020 2020 2020 5468   """..        Th
-00000330: 6520 636f 6465 2079 6f75 2070 726f 7669  e code you provi
-00000340: 6465 6420 7265 7375 6c74 6564 2069 6e20  ded resulted in 
-00000350: 616e 2065 7272 6f72 2e0d 0a20 2020 2020  an error...     
-00000360: 2020 2054 6865 2065 7272 6f72 206d 6573     The error mes
-00000370: 7361 6765 2069 733a 207b 7d2e 0d0a 2020  sage is: {}...  
-00000380: 2020 2020 2020 5468 6520 636f 6465 2079        The code y
-00000390: 6f75 2070 726f 7669 6465 6420 6973 3a20  ou provided is: 
-000003a0: 7b7d 2e0d 0a20 2020 2020 2020 2054 6865  {}...        The
-000003b0: 2071 7565 7374 696f 6e20 7761 733a 207b   question was: {
-000003c0: 7d2e 0d0a 2020 2020 2020 2020 5265 7475  }...        Retu
-000003d0: 726e 2061 2063 6f72 7265 6374 6564 2070  rn a corrected p
-000003e0: 7974 686f 6e20 636f 6465 2074 6861 7420  ython code that 
-000003f0: 6669 7865 7320 7468 6520 6572 726f 722e  fixes the error.
-00000400: 0d0a 2020 2020 2020 2020 5072 6566 6978  ..        Prefix
-00000410: 2074 6865 2070 7974 686f 6e20 636f 6465   the python code
-00000420: 2077 6974 6820 3c63 6f64 653e 2061 6e64   with <code> and
-00000430: 2073 7566 6669 7820 7468 6520 636f 6465   suffix the code
-00000440: 2077 6974 6820 3c2f 636f 6465 3e2e 0d0a   with </code>...
-00000450: 2020 2020 2020 2020 2222 220d 0a0d 0a20          """.... 
-00000460: 2020 2020 2020 206f 7065 6e61 692e 6170         openai.ap
-00000470: 695f 6b65 7920 3d20 7365 6c66 2e41 5049  i_key = self.API
-00000480: 5f4b 4559 0d0a 2020 2020 2020 2020 7365  _KEY..        se
-00000490: 6c66 2e74 6f74 616c 5f74 6f6b 656e 735f  lf.total_tokens_
-000004a0: 7573 6564 203d 205b 5d0d 0a0d 0a20 2020  used = []....   
-000004b0: 2020 2020 2023 2070 7269 6e74 2074 6865       # print the
-000004c0: 206d 6f64 656c 206e 616d 6520 696e 2072   model name in r
-000004d0: 6564 0d0a 2020 2020 2020 2020 7072 696e  ed..        prin
-000004e0: 7428 636f 6c6f 7265 6428 225c 6e55 7369  t(colored("\nUsi
-000004f0: 6e67 204d 6f64 656c 3a20 7b7d 222e 666f  ng Model: {}".fo
-00000500: 726d 6174 286c 6c6d 292c 2022 7265 6422  rmat(llm), "red"
-00000510: 2929 0d0a 0d0a 2020 2020 6465 6620 6c6c  ))....    def ll
-00000520: 6d5f 6361 6c6c 2873 656c 662c 206d 6573  m_call(self, mes
-00000530: 7361 6765 733a 2073 7472 2c20 7465 6d70  sages: str, temp
-00000540: 6572 6174 7572 653a 2066 6c6f 6174 203d  erature: float =
-00000550: 2030 2c20 6d61 785f 746f 6b65 6e73 3a20   0, max_tokens: 
-00000560: 696e 7420 3d20 3130 3030 293a 0d0a 2020  int = 1000):..  
-00000570: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-00000580: 206f 7065 6e61 692e 4368 6174 436f 6d70   openai.ChatComp
-00000590: 6c65 7469 6f6e 2e63 7265 6174 6528 0d0a  letion.create(..
-000005a0: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-000005b0: 6c3d 7365 6c66 2e6c 6c6d 2c0d 0a20 2020  l=self.llm,..   
-000005c0: 2020 2020 2020 2020 206d 6573 7361 6765           message
-000005d0: 733d 6d65 7373 6167 6573 2c0d 0a20 2020  s=messages,..   
-000005e0: 2020 2020 2020 2020 2074 656d 7065 7261           tempera
-000005f0: 7475 7265 3d74 656d 7065 7261 7475 7265  ture=temperature
-00000600: 2c0d 0a20 2020 2020 2020 2020 2020 206d  ,..            m
-00000610: 6178 5f74 6f6b 656e 733d 6d61 785f 746f  ax_tokens=max_to
-00000620: 6b65 6e73 2c0d 0a20 2020 2020 2020 2029  kens,..        )
-00000630: 0d0a 0d0a 2020 2020 2020 2020 636f 6e74  ....        cont
-00000640: 656e 7420 3d20 7265 7370 6f6e 7365 2e63  ent = response.c
-00000650: 686f 6963 6573 5b30 5d2e 6d65 7373 6167  hoices[0].messag
-00000660: 652e 636f 6e74 656e 742e 7374 7269 7028  e.content.strip(
-00000670: 290d 0a20 2020 2020 2020 2074 6f6b 656e  )..        token
-00000680: 735f 7573 6564 203d 2072 6573 706f 6e73  s_used = respons
-00000690: 652e 7573 6167 652e 746f 7461 6c5f 746f  e.usage.total_to
-000006a0: 6b65 6e73 0d0a 0d0a 2020 2020 2020 2020  kens....        
-000006b0: 7265 7475 726e 2063 6f6e 7465 6e74 2c20  return content, 
-000006c0: 746f 6b65 6e73 5f75 7365 640d 0a20 2020  tokens_used..   
-000006d0: 200d 0a20 2020 2023 2046 756e 6374 696f   ..    # Functio
-000006e0: 6e20 746f 2073 616e 6974 697a 6520 7468  n to sanitize th
-000006f0: 6520 6f75 7470 7574 2066 726f 6d20 7468  e output from th
-00000700: 6520 4c4c 4d0d 0a20 2020 2064 6566 205f  e LLM..    def _
-00000710: 6578 7472 6163 745f 636f 6465 2873 656c  extract_code(sel
-00000720: 662c 7265 7370 6f6e 7365 3a20 7374 722c  f,response: str,
-00000730: 2073 6570 6172 6174 6f72 3a20 7374 7220   separator: str 
-00000740: 3d20 2260 6060 2229 202d 3e20 7374 723a  = "```") -> str:
-00000750: 0d0a 0d0a 2020 2020 2020 2020 2320 4465  ....        # De
-00000760: 6669 6e65 2061 2062 6c61 636b 6c69 7374  fine a blacklist
-00000770: 206f 6620 5079 7468 6f6e 206b 6579 776f   of Python keywo
-00000780: 7264 7320 616e 6420 6675 6e63 7469 6f6e  rds and function
-00000790: 7320 7468 6174 2061 7265 206e 6f74 2061  s that are not a
-000007a0: 6c6c 6f77 6564 0d0a 2020 2020 2020 2020  llowed..        
-000007b0: 626c 6163 6b6c 6973 7420 3d20 5b27 6f73  blacklist = ['os
-000007c0: 272c 2773 7562 7072 6f63 6573 7327 2c27  ','subprocess','
-000007d0: 7379 7327 2c27 6576 616c 272c 2765 7865  sys','eval','exe
-000007e0: 6327 2c27 6669 6c65 272c 276f 7065 6e27  c','file','open'
-000007f0: 2c27 736f 636b 6574 272c 2775 726c 6c69  ,'socket','urlli
-00000800: 6227 5d0d 0a0d 0a20 2020 2020 2020 2023  b']....        #
-00000810: 2053 6574 2074 6865 2069 6e69 7469 616c   Set the initial
-00000820: 2076 616c 7565 206f 6620 636f 6465 2074   value of code t
-00000830: 6f20 7468 6520 7265 7370 6f6e 7365 0d0a  o the response..
-00000840: 2020 2020 2020 2020 636f 6465 203d 2072          code = r
-00000850: 6573 706f 6e73 650d 0a0d 0a20 2020 2020  esponse....     
-00000860: 2020 2023 2049 6620 7468 6520 7265 7370     # If the resp
-00000870: 6f6e 7365 2063 6f6e 7461 696e 7320 7468  onse contains th
-00000880: 6520 7365 7061 7261 746f 722c 2065 7874  e separator, ext
-00000890: 7261 6374 2074 6865 2063 6f64 6520 626c  ract the code bl
-000008a0: 6f63 6b20 6265 7477 6565 6e20 7468 6520  ock between the 
-000008b0: 7365 7061 7261 746f 7273 0d0a 2020 2020  separators..    
-000008c0: 2020 2020 6966 206c 656e 2872 6573 706f      if len(respo
-000008d0: 6e73 652e 7370 6c69 7428 7365 7061 7261  nse.split(separa
-000008e0: 746f 7229 2920 3e20 313a 0d0a 2020 2020  tor)) > 1:..    
-000008f0: 2020 2020 2020 2020 636f 6465 203d 2072          code = r
-00000900: 6573 706f 6e73 652e 7370 6c69 7428 7365  esponse.split(se
-00000910: 7061 7261 746f 7229 5b31 5d0d 0a0d 0a20  parator)[1].... 
-00000920: 2020 2020 2020 2023 2053 6561 7263 6820         # Search 
-00000930: 666f 7220 6120 7061 7474 6572 6e20 6265  for a pattern be
-00000940: 7477 6565 6e20 3c63 6f64 653e 2061 6e64  tween <code> and
-00000950: 203c 2f63 6f64 653e 2069 6e20 7468 6520   </code> in the 
-00000960: 6578 7472 6163 7465 6420 636f 6465 0d0a  extracted code..
-00000970: 2020 2020 2020 2020 6d61 7463 6820 3d20          match = 
-00000980: 7265 2e73 6561 7263 6828 7222 3c63 6f64  re.search(r"<cod
-00000990: 653e 282e 2a29 3c2f 636f 6465 3e22 2c20  e>(.*)</code>", 
-000009a0: 636f 6465 2c20 7265 2e44 4f54 414c 4c29  code, re.DOTALL)
-000009b0: 0d0a 2020 2020 2020 2020 6966 206d 6174  ..        if mat
-000009c0: 6368 3a0d 0a20 2020 2020 2020 2020 2020  ch:..           
-000009d0: 2023 2049 6620 6120 6d61 7463 6820 6973   # If a match is
-000009e0: 2066 6f75 6e64 2c20 6578 7472 6163 7420   found, extract 
-000009f0: 7468 6520 636f 6465 2062 6574 7765 656e  the code between
-00000a00: 203c 636f 6465 3e20 616e 6420 3c2f 636f   <code> and </co
-00000a10: 6465 3e0d 0a20 2020 2020 2020 2020 2020  de>..           
-00000a20: 2063 6f64 6520 3d20 6d61 7463 682e 6772   code = match.gr
-00000a30: 6f75 7028 3129 0d0a 2020 2020 2020 2020  oup(1)..        
-00000a40: 2020 2020 2320 5265 6d6f 7665 2074 6865      # Remove the
-00000a50: 2022 7079 7468 6f6e 2220 6f72 2022 7079   "python" or "py
-00000a60: 2220 7072 6566 6978 2069 6620 7072 6573  " prefix if pres
-00000a70: 656e 740d 0a20 2020 2020 2020 2020 2020  ent..           
-00000a80: 2069 6620 7265 2e6d 6174 6368 2872 225e   if re.match(r"^
-00000a90: 2870 7974 686f 6e7c 7079 2922 2c20 636f  (python|py)", co
-00000aa0: 6465 293a 0d0a 2020 2020 2020 2020 2020  de):..          
-00000ab0: 2020 2020 2020 636f 6465 203d 2072 652e        code = re.
-00000ac0: 7375 6228 7222 5e28 7079 7468 6f6e 7c70  sub(r"^(python|p
-00000ad0: 7929 222c 2022 222c 2063 6f64 6529 0d0a  y)", "", code)..
-00000ae0: 0d0a 2020 2020 2020 2020 2320 4966 2074  ..        # If t
-00000af0: 6865 2063 6f64 6520 6973 2062 6574 7765  he code is betwe
-00000b00: 656e 2073 696e 676c 6520 6261 636b 7469  en single backti
-00000b10: 636b 732c 2065 7874 7261 6374 2074 6865  cks, extract the
-00000b20: 2063 6f64 6520 6265 7477 6565 6e20 7468   code between th
-00000b30: 656d 0d0a 2020 2020 2020 2020 6966 2072  em..        if r
-00000b40: 652e 6d61 7463 6828 7222 5e60 2e2a 6024  e.match(r"^`.*`$
-00000b50: 222c 2063 6f64 6529 3a0d 0a20 2020 2020  ", code):..     
-00000b60: 2020 2020 2020 2063 6f64 6520 3d20 7265         code = re
-00000b70: 2e73 7562 2872 225e 6028 2e2a 2960 2422  .sub(r"^`(.*)`$"
-00000b80: 2c20 7222 5c31 222c 2063 6f64 6529 0d0a  , r"\1", code)..
-00000b90: 0d0a 2020 2020 2020 2020 2320 5265 6d6f  ..        # Remo
-00000ba0: 7665 2061 6e79 2069 6e73 7461 6e63 6573  ve any instances
-00000bb0: 206f 6620 2264 6620 3d20 7064 2e72 6561   of "df = pd.rea
-00000bc0: 645f 6373 7628 2766 696c 656e 616d 652e  d_csv('filename.
-00000bd0: 6373 7627 2922 2066 726f 6d20 7468 6520  csv')" from the 
-00000be0: 636f 6465 0d0a 2020 2020 2020 2020 636f  code..        co
-00000bf0: 6465 203d 2072 652e 7375 6228 7222 6466  de = re.sub(r"df
-00000c00: 5c73 2a3d 5c73 2a70 645c 2e72 6561 645f  \s*=\s*pd\.read_
-00000c10: 6373 765c 2827 2e2a 3f27 5c29 222c 2022  csv\('.*?'\)", "
-00000c20: 222c 2063 6f64 6529 0d0a 2020 2020 2020  ", code)..      
-00000c30: 2020 0d0a 2020 2020 2020 2020 2320 5265    ..        # Re
-00000c40: 6d6f 7665 2061 6e79 206f 6363 7572 7265  move any occurre
-00000c50: 6e63 6573 206f 6620 6466 203d 2070 642e  nces of df = pd.
-00000c60: 4461 7461 4672 616d 6528 2920 7769 7468  DataFrame() with
-00000c70: 2061 6e79 206e 756d 6265 7220 6f66 2063   any number of c
-00000c80: 6861 7261 6374 6572 7320 696e 7369 6465  haracters inside
-00000c90: 2074 6865 2070 6172 656e 7468 6573 6573   the parentheses
-00000ca0: 2e0d 0a20 2020 2020 2020 2063 6f64 6520  ...        code 
-00000cb0: 3d20 7265 2e73 7562 2872 2264 665c 732a  = re.sub(r"df\s*
-00000cc0: 3d5c 732a 7064 5c2e 4461 7461 4672 616d  =\s*pd\.DataFram
-00000cd0: 655c 282e 2a3f 5c29 222c 2022 222c 2063  e\(.*?\)", "", c
-00000ce0: 6f64 6529 0d0a 0d0a 2020 2020 2020 2020  ode)....        
-00000cf0: 2320 4465 6669 6e65 2074 6865 2072 6567  # Define the reg
-00000d00: 756c 6172 2065 7870 7265 7373 696f 6e20  ular expression 
-00000d10: 7061 7474 6572 6e20 746f 206d 6174 6368  pattern to match
-00000d20: 2074 6865 2062 6c61 636b 6c69 7374 2069   the blacklist i
-00000d30: 7465 6d73 0d0a 2020 2020 2020 2020 7061  tems..        pa
-00000d40: 7474 6572 6e20 3d20 7222 5e28 2e2a 5c62  ttern = r"^(.*\b
-00000d50: 2822 202b 2022 7c22 2e6a 6f69 6e28 626c  (" + "|".join(bl
-00000d60: 6163 6b6c 6973 7429 202b 2072 2229 5c62  acklist) + r")\b
-00000d70: 2e2a 2924 220d 0a0d 0a20 2020 2020 2020  .*)$"....       
-00000d80: 2023 2052 6570 6c61 6365 2074 6865 2062   # Replace the b
-00000d90: 6c61 636b 6c69 7374 2069 7465 6d73 2077  lacklist items w
-00000da0: 6974 6820 636f 6d6d 656e 7473 0d0a 2020  ith comments..  
-00000db0: 2020 2020 2020 636f 6465 203d 2072 652e        code = re.
-00000dc0: 7375 6228 7061 7474 6572 6e2c 2072 2223  sub(pattern, r"#
-00000dd0: 206e 6f74 2061 6c6c 6f77 6564 205c 3122   not allowed \1"
-00000de0: 2c20 636f 6465 2c20 666c 6167 733d 7265  , code, flags=re
-00000df0: 2e4d 554c 5449 4c49 4e45 290d 0a0d 0a20  .MULTILINE).... 
-00000e00: 2020 2020 2020 2023 2052 6574 7572 6e20         # Return 
-00000e10: 7468 6520 636c 6561 6e65 6420 616e 6420  the cleaned and 
-00000e20: 6578 7472 6163 7465 6420 636f 6465 0d0a  extracted code..
-00000e30: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-00000e40: 6f64 652e 7374 7269 7028 290d 0a0d 0a20  ode.strip().... 
-00000e50: 2020 2064 6566 2070 645f 6167 656e 745f     def pd_agent_
-00000e60: 636f 6e76 6572 7365 2873 656c 662c 2071  converse(self, q
-00000e70: 7565 7374 696f 6e3d 4e6f 6e65 293a 0d0a  uestion=None):..
-00000e80: 2020 2020 2020 2020 2320 496e 6974 6961          # Initia
-00000e90: 6c69 7a65 2074 6865 206d 6573 7361 6765  lize the message
-00000ea0: 7320 6c69 7374 2077 6974 6820 6120 7379  s list with a sy
-00000eb0: 7374 656d 206d 6573 7361 6765 2063 6f6e  stem message con
-00000ec0: 7461 696e 696e 6720 7468 6520 7461 736b  taining the task
-00000ed0: 2070 726f 6d70 740d 0a20 2020 2020 2020   prompt..       
-00000ee0: 206d 6573 7361 6765 7320 3d20 5b7b 2272   messages = [{"r
-00000ef0: 6f6c 6522 3a20 2273 7973 7465 6d22 2c20  ole": "system", 
-00000f00: 2263 6f6e 7465 6e74 223a 2073 656c 662e  "content": self.
-00000f10: 7461 736b 2e66 6f72 6d61 7428 7365 6c66  task.format(self
-00000f20: 2e64 665f 6865 6164 2c20 2222 297d 5d0d  .df_head, "")}].
-00000f30: 0a0d 0a20 2020 2020 2020 2023 2049 6620  ...        # If 
-00000f40: 6120 7175 6573 7469 6f6e 2069 7320 7072  a question is pr
-00000f50: 6f76 6964 6564 2c20 736b 6970 2074 6865  ovided, skip the
-00000f60: 2069 6e70 7574 2070 726f 6d70 740d 0a20   input prompt.. 
-00000f70: 2020 2020 2020 2069 6620 7175 6573 7469         if questi
-00000f80: 6f6e 2069 7320 6e6f 7420 4e6f 6e65 3a0d  on is not None:.
-00000f90: 0a20 2020 2020 2020 2020 2020 2061 6e73  .            ans
-00000fa0: 7765 7220 3d20 7365 6c66 2e70 645f 6167  wer = self.pd_ag
-00000fb0: 656e 7428 7175 6573 7469 6f6e 2c20 6d65  ent(question, me
-00000fc0: 7373 6167 6573 2c20 7365 6c66 2e64 6629  ssages, self.df)
-00000fd0: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-00000fe0: 696e 7428 636f 6c6f 7265 6428 225c 6e41  int(colored("\nA
-00000ff0: 6e73 7765 723a 5c6e 7b7d 222e 666f 726d  nswer:\n{}".form
-00001000: 6174 2861 6e73 7765 7229 2c20 2267 7265  at(answer), "gre
-00001010: 656e 2229 290d 0a20 2020 2020 2020 2020  en"))..         
-00001020: 2020 2072 6574 7572 6e0d 0a0d 0a20 2020     return....   
-00001030: 2020 2020 2023 2053 7461 7274 2061 6e20       # Start an 
-00001040: 696e 6669 6e69 7465 206c 6f6f 7020 746f  infinite loop to
-00001050: 206b 6565 7020 6173 6b69 6e67 2074 6865   keep asking the
-00001060: 2075 7365 7220 666f 7220 7175 6573 7469   user for questi
-00001070: 6f6e 730d 0a20 2020 2020 2020 2077 6869  ons..        whi
-00001080: 6c65 2054 7275 653a 0d0a 2020 2020 2020  le True:..      
-00001090: 2020 2020 2020 2320 5072 6f6d 7074 2074        # Prompt t
-000010a0: 6865 2075 7365 7220 746f 2065 6e74 6572  he user to enter
-000010b0: 2061 2071 7565 7374 696f 6e20 6f72 2074   a question or t
-000010c0: 7970 6520 2765 7869 7427 2074 6f20 7175  ype 'exit' to qu
-000010d0: 6974 0d0a 2020 2020 2020 2020 2020 2020  it..            
-000010e0: 7175 6573 7469 6f6e 203d 2069 6e70 7574  question = input
-000010f0: 2863 6f6c 6f72 6564 2822 456e 7465 7220  (colored("Enter 
-00001100: 796f 7572 2071 7565 7374 696f 6e20 6f72  your question or
-00001110: 2074 7970 6520 2765 7869 7427 2074 6f20   type 'exit' to 
-00001120: 7175 6974 3a20 222c 2022 6379 616e 2229  quit: ", "cyan")
-00001130: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00001140: 2023 2049 6620 7468 6520 7573 6572 2074   # If the user t
-00001150: 7970 6573 2027 6578 6974 272c 2062 7265  ypes 'exit', bre
-00001160: 616b 206f 7574 206f 6620 7468 6520 6c6f  ak out of the lo
-00001170: 6f70 0d0a 2020 2020 2020 2020 2020 2020  op..            
-00001180: 6966 2071 7565 7374 696f 6e2e 7374 7269  if question.stri
-00001190: 7028 292e 6c6f 7765 7228 2920 3d3d 2027  p().lower() == '
-000011a0: 6578 6974 273a 0d0a 2020 2020 2020 2020  exit':..        
-000011b0: 2020 2020 2020 2020 6272 6561 6b0d 0a0d          break...
-000011c0: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
-000011d0: 616c 6c20 7468 6520 7064 5f61 6765 6e74  all the pd_agent
-000011e0: 206d 6574 686f 6420 7769 7468 2074 6865   method with the
-000011f0: 2075 7365 7227 7320 7175 6573 7469 6f6e   user's question
-00001200: 2c20 7468 6520 6d65 7373 6167 6573 206c  , the messages l
-00001210: 6973 742c 2061 6e64 2074 6865 2064 6174  ist, and the dat
-00001220: 6166 7261 6d65 0d0a 2020 2020 2020 2020  aframe..        
-00001230: 2020 2020 616e 7377 6572 203d 2073 656c      answer = sel
-00001240: 662e 7064 5f61 6765 6e74 2871 7565 7374  f.pd_agent(quest
-00001250: 696f 6e2c 206d 6573 7361 6765 732c 2073  ion, messages, s
-00001260: 656c 662e 6466 290d 0a0d 0a20 2020 2020  elf.df)....     
-00001270: 2020 2020 2020 2023 2050 7269 6e74 2074         # Print t
-00001280: 6865 2061 6e73 7765 7220 7265 7475 726e  he answer return
-00001290: 6564 2062 7920 7468 6520 7064 5f61 6765  ed by the pd_age
-000012a0: 6e74 206d 6574 686f 640d 0a20 2020 2020  nt method..     
-000012b0: 2020 2020 2020 2070 7269 6e74 2863 6f6c         print(col
-000012c0: 6f72 6564 2822 5c6e 416e 7377 6572 3a5c  ored("\nAnswer:\
-000012d0: 6e7b 7d22 2e66 6f72 6d61 7428 616e 7377  n{}".format(answ
-000012e0: 6572 292c 2022 6772 6565 6e22 2929 0d0a  er), "green"))..
-000012f0: 0d0a 0d0a 2020 2020 6465 6620 7064 5f61  ....    def pd_a
-00001300: 6765 6e74 2873 656c 662c 2071 7565 7374  gent(self, quest
-00001310: 696f 6e2c 206d 6573 7361 6765 732c 2064  ion, messages, d
-00001320: 663d 4e6f 6e65 293a 0d0a 2020 2020 2020  f=None):..      
-00001330: 2020 2320 4164 6420 6120 7573 6572 206d    # Add a user m
-00001340: 6573 7361 6765 2077 6974 6820 7468 6520  essage with the 
-00001350: 7570 6461 7465 6420 7461 736b 2070 726f  updated task pro
-00001360: 6d70 7420 746f 2074 6865 206d 6573 7361  mpt to the messa
-00001370: 6765 7320 6c69 7374 0d0a 2020 2020 2020  ges list..      
-00001380: 2020 6d65 7373 6167 6573 2e61 7070 656e    messages.appen
-00001390: 6428 7b22 726f 6c65 223a 2022 7573 6572  d({"role": "user
-000013a0: 222c 2022 636f 6e74 656e 7422 3a20 7365  ", "content": se
-000013b0: 6c66 2e74 6173 6b2e 666f 726d 6174 2873  lf.task.format(s
-000013c0: 656c 662e 6466 5f68 6561 642c 2071 7565  elf.df_head, que
-000013d0: 7374 696f 6e29 7d29 0d0a 0d0a 2020 2020  stion)})....    
-000013e0: 2020 2020 2320 4361 6c6c 2074 6865 204f      # Call the O
-000013f0: 7065 6e41 4920 4150 4920 616e 6420 6861  penAI API and ha
-00001400: 6e64 6c65 2072 6174 6520 6c69 6d69 7420  ndle rate limit 
-00001410: 6572 726f 7273 0d0a 2020 2020 2020 2020  errors..        
-00001420: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-00001430: 2020 636f 6465 2c20 746f 6b65 6e73 5f75    code, tokens_u
-00001440: 7365 6420 3d20 7365 6c66 2e6c 6c6d 5f63  sed = self.llm_c
-00001450: 616c 6c28 6d65 7373 6167 6573 290d 0a20  all(messages).. 
-00001460: 2020 2020 2020 2065 7863 6570 7420 6f70         except op
-00001470: 656e 6169 2e65 7272 6f72 2e52 6174 654c  enai.error.RateL
-00001480: 696d 6974 4572 726f 723a 0d0a 2020 2020  imitError:..    
-00001490: 2020 2020 2020 2020 7072 696e 7428 0d0a          print(..
-000014a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014b0: 2254 6865 204f 7065 6e41 4920 4150 4920  "The OpenAI API 
-000014c0: 7261 7465 206c 696d 6974 2068 6173 2062  rate limit has b
-000014d0: 6565 6e20 6578 6365 6564 6564 2e20 5761  een exceeded. Wa
-000014e0: 6974 696e 6720 3130 2073 6563 6f6e 6473  iting 10 seconds
-000014f0: 2061 6e64 2074 7279 696e 6720 6167 6169   and trying agai
-00001500: 6e2e 220d 0a20 2020 2020 2020 2020 2020  n."..           
-00001510: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-00001520: 7469 6d65 2e73 6c65 6570 2831 3029 0d0a  time.sleep(10)..
-00001530: 2020 2020 2020 2020 2020 2020 636f 6465              code
-00001540: 2c20 746f 6b65 6e73 5f75 7365 6420 3d20  , tokens_used = 
-00001550: 7365 6c66 2e6c 6c6d 5f63 616c 6c28 6d65  self.llm_call(me
-00001560: 7373 6167 6573 290d 0a0d 0a20 2020 2020  ssages)....     
-00001570: 2020 2023 2045 7874 7261 6374 2074 6865     # Extract the
-00001580: 2063 6f64 6520 6672 6f6d 2074 6865 2041   code from the A
-00001590: 5049 2072 6573 706f 6e73 650d 0a20 2020  PI response..   
-000015a0: 2020 2020 2063 6f64 6520 3d20 7365 6c66       code = self
-000015b0: 2e5f 6578 7472 6163 745f 636f 6465 2863  ._extract_code(c
-000015c0: 6f64 6529 0d0a 0d0a 2020 2020 2020 2020  ode)....        
-000015d0: 2320 5570 6461 7465 2074 6865 2074 6f74  # Update the tot
-000015e0: 616c 2074 6f6b 656e 7320 7573 6564 0d0a  al tokens used..
-000015f0: 2020 2020 2020 2020 7365 6c66 2e74 6f74          self.tot
-00001600: 616c 5f74 6f6b 656e 735f 7573 6564 2e61  al_tokens_used.a
-00001610: 7070 656e 6428 746f 6b65 6e73 5f75 7365  ppend(tokens_use
-00001620: 6429 0d0a 2020 2020 2020 2020 746f 7461  d)..        tota
-00001630: 6c5f 746f 6b65 6e73 5f75 7365 645f 7375  l_tokens_used_su
-00001640: 6d20 3d20 7375 6d28 7365 6c66 2e74 6f74  m = sum(self.tot
-00001650: 616c 5f74 6f6b 656e 735f 7573 6564 290d  al_tokens_used).
-00001660: 0a0d 0a20 2020 2020 2020 2023 2052 6564  ...        # Red
-00001670: 6972 6563 7420 7374 616e 6461 7264 206f  irect standard o
-00001680: 7574 7075 7420 746f 2061 2053 7472 696e  utput to a Strin
-00001690: 6749 4f20 6275 6666 6572 0d0a 2020 2020  gIO buffer..    
-000016a0: 2020 2020 6f75 7470 7574 203d 2069 6f2e      output = io.
-000016b0: 5374 7269 6e67 494f 2829 0d0a 2020 2020  StringIO()..    
-000016c0: 2020 2020 7379 732e 7374 646f 7574 203d      sys.stdout =
-000016d0: 206f 7574 7075 740d 0a0d 0a20 2020 2020   output....     
-000016e0: 2020 2023 2049 6e69 7469 616c 697a 6520     # Initialize 
-000016f0: 6572 726f 7220 636f 7272 6563 7469 6f6e  error correction
-00001700: 2063 6f75 6e74 6572 0d0a 2020 2020 2020   counter..      
-00001710: 2020 6572 726f 725f 636f 7272 6563 7469    error_correcti
-00001720: 6f6e 7320 3d20 300d 0a0d 0a20 2020 2020  ons = 0....     
-00001730: 2020 2023 2054 7279 2074 6f20 6578 6563     # Try to exec
-00001740: 7574 6520 7468 6520 636f 6465 2061 6e64  ute the code and
-00001750: 2068 616e 646c 6520 6572 726f 7273 0d0a   handle errors..
-00001760: 2020 2020 2020 2020 7768 696c 6520 6572          while er
-00001770: 726f 725f 636f 7272 6563 7469 6f6e 7320  ror_corrections 
-00001780: 3c20 7365 6c66 2e4d 4158 5f45 5252 4f52  < self.MAX_ERROR
-00001790: 5f43 4f52 5245 4354 494f 4e53 3a0d 0a20  _CORRECTIONS:.. 
-000017a0: 2020 2020 2020 2020 2020 2074 7279 3a0d             try:.
-000017b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000017c0: 206d 6573 7361 6765 732e 6170 7065 6e64   messages.append
-000017d0: 287b 2272 6f6c 6522 3a20 2261 7373 6973  ({"role": "assis
-000017e0: 7461 6e74 222c 2022 636f 6e74 656e 7422  tant", "content"
-000017f0: 3a20 636f 6465 7d29 0d0a 2020 2020 2020  : code})..      
-00001800: 2020 2020 2020 2020 2020 6578 6563 2863            exec(c
-00001810: 6f64 6529 0d0a 2020 2020 2020 2020 2020  ode)..          
-00001820: 2020 2020 2020 6272 6561 6b0d 0a20 2020        break..   
-00001830: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-00001840: 4578 6365 7074 696f 6e20 6173 2065 3a0d  Exception as e:.
-00001850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001860: 2023 2049 6e63 7265 6d65 6e74 2074 6865   # Increment the
-00001870: 2065 7272 6f72 2063 6f72 7265 6374 696f   error correctio
-00001880: 6e20 636f 756e 7465 7220 616e 6420 7570  n counter and up
-00001890: 6461 7465 2074 6865 206d 6573 7361 6765  date the message
-000018a0: 7320 6c69 7374 2077 6974 6820 7468 6520  s list with the 
-000018b0: 6572 726f 720d 0a20 2020 2020 2020 2020  error..         
-000018c0: 2020 2020 2020 2065 7272 6f72 5f63 6f72         error_cor
-000018d0: 7265 6374 696f 6e73 202b 3d20 310d 0a20  rections += 1.. 
-000018e0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000018f0: 6573 7361 6765 732e 6170 7065 6e64 287b  essages.append({
-00001900: 2272 6f6c 6522 3a20 2275 7365 7222 2c20  "role": "user", 
-00001910: 2263 6f6e 7465 6e74 223a 2073 656c 662e  "content": self.
-00001920: 6572 726f 725f 636f 7272 6563 745f 7461  error_correct_ta
-00001930: 736b 2e66 6f72 6d61 7428 652c 2063 6f64  sk.format(e, cod
-00001940: 652c 2071 7565 7374 696f 6e29 7d29 0d0a  e, question)})..
-00001950: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001960: 2020 2320 4174 7465 6d70 7420 746f 2063    # Attempt to c
-00001970: 6f72 7265 6374 2074 6865 2063 6f64 6520  orrect the code 
-00001980: 616e 6420 6861 6e64 6c65 2072 6174 6520  and handle rate 
-00001990: 6c69 6d69 7420 6572 726f 7273 0d0a 2020  limit errors..  
-000019a0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-000019b0: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-000019c0: 2020 2020 2020 2020 636f 6465 2c20 746f          code, to
-000019d0: 6b65 6e73 5f75 7365 6420 3d20 7365 6c66  kens_used = self
-000019e0: 2e6c 6c6d 5f63 616c 6c28 6d65 7373 6167  .llm_call(messag
-000019f0: 6573 290d 0a20 2020 2020 2020 2020 2020  es)..           
-00001a00: 2020 2020 2020 2020 2063 6f64 6520 3d20           code = 
-00001a10: 7365 6c66 2e5f 6578 7472 6163 745f 636f  self._extract_co
-00001a20: 6465 2863 6f64 6529 0d0a 2020 2020 2020  de(code)..      
-00001a30: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00001a40: 6c66 2e74 6f74 616c 5f74 6f6b 656e 735f  lf.total_tokens_
-00001a50: 7573 6564 2e61 7070 656e 6428 746f 6b65  used.append(toke
-00001a60: 6e73 5f75 7365 6429 0d0a 2020 2020 2020  ns_used)..      
-00001a70: 2020 2020 2020 2020 2020 2020 2020 746f                to
-00001a80: 7461 6c5f 746f 6b65 6e73 5f75 7365 645f  tal_tokens_used_
-00001a90: 7375 6d20 3d20 7375 6d28 7365 6c66 2e74  sum = sum(self.t
-00001aa0: 6f74 616c 5f74 6f6b 656e 735f 7573 6564  otal_tokens_used
-00001ab0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00001ac0: 2020 2065 7863 6570 7420 6f70 656e 6169     except openai
-00001ad0: 2e65 7272 6f72 2e52 6174 654c 696d 6974  .error.RateLimit
-00001ae0: 4572 726f 723a 0d0a 2020 2020 2020 2020  Error:..        
-00001af0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00001b00: 7428 0d0a 2020 2020 2020 2020 2020 2020  t(..            
-00001b10: 2020 2020 2020 2020 2020 2020 2254 6865              "The
-00001b20: 204f 7065 6e41 4920 4150 4920 7261 7465   OpenAI API rate
-00001b30: 206c 696d 6974 2068 6173 2062 6565 6e20   limit has been 
-00001b40: 6578 6365 6564 6564 2e20 5761 6974 696e  exceeded. Waitin
-00001b50: 6720 3130 2073 6563 6f6e 6473 2061 6e64  g 10 seconds and
-00001b60: 2074 7279 696e 6720 6167 6169 6e2e 220d   trying again.".
-00001b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001b80: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00001b90: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-00001ba0: 2e73 6c65 6570 2831 3029 0d0a 2020 2020  .sleep(10)..    
-00001bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bc0: 636f 6465 2c20 746f 6b65 6e73 5f75 7365  code, tokens_use
-00001bd0: 6420 3d20 7365 6c66 2e6c 6c6d 5f63 616c  d = self.llm_cal
-00001be0: 6c28 6d65 7373 6167 6573 290d 0a20 2020  l(messages)..   
-00001bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c00: 2063 6f64 6520 3d20 7365 6c66 2e5f 6578   code = self._ex
-00001c10: 7472 6163 745f 636f 6465 2863 6f64 6529  tract_code(code)
-00001c20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001c30: 2020 2020 2020 7365 6c66 2e74 6f74 616c        self.total
-00001c40: 5f74 6f6b 656e 735f 7573 6564 2e61 7070  _tokens_used.app
-00001c50: 656e 6428 746f 6b65 6e73 5f75 7365 6429  end(tokens_used)
-00001c60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001c70: 2020 2020 2020 746f 7461 6c5f 746f 6b65        total_toke
-00001c80: 6e73 5f75 7365 645f 7375 6d20 3d20 7375  ns_used_sum = su
-00001c90: 6d28 7365 6c66 2e74 6f74 616c 5f74 6f6b  m(self.total_tok
-00001ca0: 656e 735f 7573 6564 290d 0a0d 0a20 2020  ens_used)....   
-00001cb0: 2020 2020 2023 2050 7269 6e74 2074 6865       # Print the
-00001cc0: 2067 656e 6572 6174 6564 2063 6f64 650d   generated code.
-00001cd0: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
-00001ce0: 5c6e 436f 6465 3a5c 6e7b 7d22 2e66 6f72  \nCode:\n{}".for
-00001cf0: 6d61 7428 636f 6465 2929 0d0a 0d0a 2020  mat(code))....  
-00001d00: 2020 2020 2020 2320 5265 7374 6f72 6520        # Restore 
-00001d10: 7374 616e 6461 7264 206f 7574 7075 740d  standard output.
-00001d20: 0a20 2020 2020 2020 2073 7973 2e73 7464  .        sys.std
-00001d30: 6f75 7420 3d20 7379 732e 5f5f 7374 646f  out = sys.__stdo
-00001d40: 7574 5f5f 0d0a 0d0a 2020 2020 2020 2020  ut__....        
-00001d50: 2320 5072 696e 7420 7468 6520 746f 7461  # Print the tota
-00001d60: 6c20 746f 6b65 6e73 2075 7365 640d 0a20  l tokens used.. 
-00001d70: 2020 2020 2020 2070 7269 6e74 2863 6f6c         print(col
-00001d80: 6f72 6564 2822 5c6e 546f 7461 6c20 746f  ored("\nTotal to
-00001d90: 6b65 6e73 2075 7365 643a 7b7d 222e 666f  kens used:{}".fo
-00001da0: 726d 6174 2874 6f74 616c 5f74 6f6b 656e  rmat(total_token
-00001db0: 735f 7573 6564 5f73 756d 292c 2022 7965  s_used_sum), "ye
-00001dc0: 6c6c 6f77 2229 290d 0a0d 0a20 2020 2020  llow"))....     
-00001dd0: 2020 2023 2047 6574 2074 6865 206f 7574     # Get the out
-00001de0: 7075 7420 6672 6f6d 2074 6865 2065 7865  put from the exe
-00001df0: 6375 7465 6420 636f 6465 0d0a 2020 2020  cuted code..    
-00001e00: 2020 2020 616e 7377 6572 203d 206f 7574      answer = out
-00001e10: 7075 742e 6765 7476 616c 7565 2829 0d0a  put.getvalue()..
-00001e20: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00001e30: 2061 6e73 7765 720d 0a20 2020 20          answer..    
+00000020: 7973 0d0a 6672 6f6d 2063 6f6e 7465 7874  ys..from context
+00000030: 6c69 6220 696d 706f 7274 2072 6564 6972  lib import redir
+00000040: 6563 745f 7374 646f 7574 0d0a 696d 706f  ect_stdout..impo
+00000050: 7274 2069 6f0d 0a69 6d70 6f72 7420 7469  rt io..import ti
+00000060: 6d65 0d0a 696d 706f 7274 206f 7065 6e61  me..import opena
+00000070: 690d 0a69 6d70 6f72 7420 7061 6e64 6173  i..import pandas
+00000080: 2061 7320 7064 0d0a 6672 6f6d 2074 6572   as pd..from ter
+00000090: 6d63 6f6c 6f72 2069 6d70 6f72 7420 636f  mcolor import co
+000000a0: 6c6f 7265 642c 2063 7072 696e 740d 0a66  lored, cprint..f
+000000b0: 726f 6d20 4950 7974 686f 6e2e 6469 7370  rom IPython.disp
+000000c0: 6c61 7920 696d 706f 7274 2064 6973 706c  lay import displ
+000000d0: 6179 2c20 4854 4d4c 0d0a 0d0a 636c 6173  ay, HTML....clas
+000000e0: 7320 4261 6d62 6f6f 4149 3a0d 0a20 2020  s BambooAI:..   
+000000f0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00000100: 6c66 2c20 6466 3a20 7064 2e44 6174 6146  lf, df: pd.DataF
+00000110: 7261 6d65 2c20 6c6c 6d3a 2073 7472 203d  rame, llm: str =
+00000120: 2027 6770 742d 332e 352d 7475 7262 6f27   'gpt-3.5-turbo'
+00000130: 293a 0d0a 0d0a 2020 2020 2020 2020 7365  ):....        se
+00000140: 6c66 2e41 5049 5f4b 4559 203d 206f 732e  lf.API_KEY = os.
+00000150: 656e 7669 726f 6e2e 6765 7428 274f 5045  environ.get('OPE
+00000160: 4e41 495f 4150 495f 4b45 5927 290d 0a20  NAI_API_KEY').. 
+00000170: 2020 2020 2020 2073 656c 662e 4d41 585f         self.MAX_
+00000180: 4552 524f 525f 434f 5252 4543 5449 4f4e  ERROR_CORRECTION
+00000190: 5320 3d20 330d 0a0d 0a20 2020 2020 2020  S = 3....       
+000001a0: 2073 656c 662e 6466 203d 2064 660d 0a20   self.df = df.. 
+000001b0: 2020 2020 2020 2073 656c 662e 6466 5f68         self.df_h
+000001c0: 6561 6420 3d20 6466 2e68 6561 6428 3129  ead = df.head(1)
+000001d0: 0d0a 2020 2020 0d0a 2020 2020 2020 2020  ..    ..        
+000001e0: 7365 6c66 2e6c 6c6d 203d 206c 6c6d 0d0a  self.llm = llm..
+000001f0: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
+00000200: 6173 6b20 3d20 2222 220d 0a20 2020 2020  ask = """..     
+00000210: 2020 2054 6865 7265 2069 7320 6120 7061     There is a pa
+00000220: 6e64 6173 2064 6174 6166 7261 6d65 2e0d  ndas dataframe..
+00000230: 0a20 2020 2020 2020 2054 6865 206e 616d  .        The nam
+00000240: 6520 6f66 2074 6865 2064 6174 6166 7261  e of the datafra
+00000250: 6d65 2069 7320 6064 6660 2e0d 0a20 2020  me is `df`...   
+00000260: 2020 2020 2054 6869 7320 6973 2074 6865       This is the
+00000270: 2072 6573 756c 7420 6f66 2060 7072 696e   result of `prin
+00000280: 7428 6466 2e68 6561 6428 3129 2960 3a0d  t(df.head(1))`:.
+00000290: 0a20 2020 2020 2020 207b 7d2e 0d0a 0d0a  .        {}.....
+000002a0: 2020 2020 2020 2020 5265 7475 726e 2074          Return t
+000002b0: 6865 2070 7974 686f 6e20 636f 6465 2074  he python code t
+000002c0: 6861 7420 7072 696e 7473 206f 7574 2074  hat prints out t
+000002d0: 6865 2061 6e73 7765 7220 746f 2074 6865  he answer to the
+000002e0: 2066 6f6c 6c6f 7769 6e67 2071 7565 7374   following quest
+000002f0: 696f 6e20 3a20 7b7d 2e20 0d0a 2020 2020  ion : {}. ..    
+00000300: 2020 2020 5072 6566 6978 2074 6865 2070      Prefix the p
+00000310: 7974 686f 6e20 636f 6465 2077 6974 6820  ython code with 
+00000320: 3c63 6f64 653e 2061 6e64 2073 7566 6669  <code> and suffi
+00000330: 7820 7468 6520 636f 6465 2077 6974 6820  x the code with 
+00000340: 3c2f 636f 6465 3e20 2e0d 0a20 2020 2020  </code> ...     
+00000350: 2020 2022 2222 0d0a 0d0a 2020 2020 2020     """....      
+00000360: 2020 7365 6c66 2e65 7272 6f72 5f63 6f72    self.error_cor
+00000370: 7265 6374 5f74 6173 6b20 3d20 2222 220d  rect_task = """.
+00000380: 0a20 2020 2020 2020 2054 6865 2063 6f64  .        The cod
+00000390: 6520 796f 7520 7072 6f76 6964 6564 2072  e you provided r
+000003a0: 6573 756c 7465 6420 696e 2061 6e20 6572  esulted in an er
+000003b0: 726f 722e 0d0a 2020 2020 2020 2020 5468  ror...        Th
+000003c0: 6520 6572 726f 7220 6d65 7373 6167 6520  e error message 
+000003d0: 6973 3a20 7b7d 2e0d 0a20 2020 2020 2020  is: {}...       
+000003e0: 2054 6865 2063 6f64 6520 796f 7520 7072   The code you pr
+000003f0: 6f76 6964 6564 2069 733a 207b 7d2e 0d0a  ovided is: {}...
+00000400: 2020 2020 2020 2020 5468 6520 7175 6573          The ques
+00000410: 7469 6f6e 2077 6173 3a20 7b7d 2e0d 0a20  tion was: {}... 
+00000420: 2020 2020 2020 2052 6574 7572 6e20 6120         Return a 
+00000430: 636f 7272 6563 7465 6420 7079 7468 6f6e  corrected python
+00000440: 2063 6f64 6520 7468 6174 2066 6978 6573   code that fixes
+00000450: 2074 6865 2065 7272 6f72 2e0d 0a20 2020   the error...   
+00000460: 2020 2020 2050 7265 6669 7820 7468 6520       Prefix the 
+00000470: 7079 7468 6f6e 2063 6f64 6520 7769 7468  python code with
+00000480: 203c 636f 6465 3e20 616e 6420 7375 6666   <code> and suff
+00000490: 6978 2074 6865 2063 6f64 6520 7769 7468  ix the code with
+000004a0: 203c 2f63 6f64 653e 2e0d 0a20 2020 2020   </code>...     
+000004b0: 2020 2022 2222 0d0a 0d0a 2020 2020 2020     """....      
+000004c0: 2020 6f70 656e 6169 2e61 7069 5f6b 6579    openai.api_key
+000004d0: 203d 2073 656c 662e 4150 495f 4b45 590d   = self.API_KEY.
+000004e0: 0a20 2020 2020 2020 2073 656c 662e 746f  .        self.to
+000004f0: 7461 6c5f 746f 6b65 6e73 5f75 7365 6420  tal_tokens_used 
+00000500: 3d20 5b5d 0d0a 0d0a 2020 2020 2020 2020  = []....        
+00000510: 2320 7072 696e 7420 7468 6520 6d6f 6465  # print the mode
+00000520: 6c20 6e61 6d65 2069 6e20 7265 640d 0a20  l name in red.. 
+00000530: 2020 2020 2020 2070 7269 6e74 2863 6f6c         print(col
+00000540: 6f72 6564 2822 5c6e 5573 696e 6720 4d6f  ored("\nUsing Mo
+00000550: 6465 6c3a 207b 7d22 2e66 6f72 6d61 7428  del: {}".format(
+00000560: 6c6c 6d29 2c20 2272 6564 2229 290d 0a0d  llm), "red"))...
+00000570: 0a20 2020 2064 6566 206c 6c6d 5f63 616c  .    def llm_cal
+00000580: 6c28 7365 6c66 2c20 6d65 7373 6167 6573  l(self, messages
+00000590: 3a20 7374 722c 2074 656d 7065 7261 7475  : str, temperatu
+000005a0: 7265 3a20 666c 6f61 7420 3d20 302c 206d  re: float = 0, m
+000005b0: 6178 5f74 6f6b 656e 733a 2069 6e74 203d  ax_tokens: int =
+000005c0: 2031 3030 3029 3a0d 0a20 2020 2020 2020   1000):..       
+000005d0: 2072 6573 706f 6e73 6520 3d20 6f70 656e   response = open
+000005e0: 6169 2e43 6861 7443 6f6d 706c 6574 696f  ai.ChatCompletio
+000005f0: 6e2e 6372 6561 7465 280d 0a20 2020 2020  n.create(..     
+00000600: 2020 2020 2020 206d 6f64 656c 3d73 656c         model=sel
+00000610: 662e 6c6c 6d2c 0d0a 2020 2020 2020 2020  f.llm,..        
+00000620: 2020 2020 6d65 7373 6167 6573 3d6d 6573      messages=mes
+00000630: 7361 6765 732c 0d0a 2020 2020 2020 2020  sages,..        
+00000640: 2020 2020 7465 6d70 6572 6174 7572 653d      temperature=
+00000650: 7465 6d70 6572 6174 7572 652c 0d0a 2020  temperature,..  
+00000660: 2020 2020 2020 2020 2020 6d61 785f 746f            max_to
+00000670: 6b65 6e73 3d6d 6178 5f74 6f6b 656e 732c  kens=max_tokens,
+00000680: 0d0a 2020 2020 2020 2020 290d 0a0d 0a20  ..        ).... 
+00000690: 2020 2020 2020 2063 6f6e 7465 6e74 203d         content =
+000006a0: 2072 6573 706f 6e73 652e 6368 6f69 6365   response.choice
+000006b0: 735b 305d 2e6d 6573 7361 6765 2e63 6f6e  s[0].message.con
+000006c0: 7465 6e74 2e73 7472 6970 2829 0d0a 2020  tent.strip()..  
+000006d0: 2020 2020 2020 746f 6b65 6e73 5f75 7365        tokens_use
+000006e0: 6420 3d20 7265 7370 6f6e 7365 2e75 7361  d = response.usa
+000006f0: 6765 2e74 6f74 616c 5f74 6f6b 656e 730d  ge.total_tokens.
+00000700: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+00000710: 6e20 636f 6e74 656e 742c 2074 6f6b 656e  n content, token
+00000720: 735f 7573 6564 0d0a 2020 2020 0d0a 2020  s_used..    ..  
+00000730: 2020 2320 4675 6e63 7469 6f6e 2074 6f20    # Function to 
+00000740: 7361 6e69 7469 7a65 2074 6865 206f 7574  sanitize the out
+00000750: 7075 7420 6672 6f6d 2074 6865 204c 4c4d  put from the LLM
+00000760: 0d0a 2020 2020 6465 6620 5f65 7874 7261  ..    def _extra
+00000770: 6374 5f63 6f64 6528 7365 6c66 2c72 6573  ct_code(self,res
+00000780: 706f 6e73 653a 2073 7472 2c20 7365 7061  ponse: str, sepa
+00000790: 7261 746f 723a 2073 7472 203d 2022 6060  rator: str = "``
+000007a0: 6022 2920 2d3e 2073 7472 3a0d 0a0d 0a20  `") -> str:.... 
+000007b0: 2020 2020 2020 2023 2044 6566 696e 6520         # Define 
+000007c0: 6120 626c 6163 6b6c 6973 7420 6f66 2050  a blacklist of P
+000007d0: 7974 686f 6e20 6b65 7977 6f72 6473 2061  ython keywords a
+000007e0: 6e64 2066 756e 6374 696f 6e73 2074 6861  nd functions tha
+000007f0: 7420 6172 6520 6e6f 7420 616c 6c6f 7765  t are not allowe
+00000800: 640d 0a20 2020 2020 2020 2062 6c61 636b  d..        black
+00000810: 6c69 7374 203d 205b 276f 7327 2c27 7375  list = ['os','su
+00000820: 6270 726f 6365 7373 272c 2773 7973 272c  bprocess','sys',
+00000830: 2765 7661 6c27 2c27 6578 6563 272c 2766  'eval','exec','f
+00000840: 696c 6527 2c27 6f70 656e 272c 2773 6f63  ile','open','soc
+00000850: 6b65 7427 2c27 7572 6c6c 6962 272c 0d0a  ket','urllib',..
+00000860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000870: 2020 2020 2773 6875 7469 6c27 2c27 7069      'shutil','pi
+00000880: 636b 6c65 272c 2763 7479 7065 7327 2c27  ckle','ctypes','
+00000890: 6d75 6c74 6970 726f 6365 7373 696e 6727  multiprocessing'
+000008a0: 2c27 7465 6d70 6669 6c65 272c 2767 6c6f  ,'tempfile','glo
+000008b0: 6227 2c27 636f 6465 272c 2770 7479 272c  b','code','pty',
+000008c0: 2763 6f6d 6d61 6e64 7327 2c0d 0a20 2020  'commands',..   
+000008d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008e0: 2027 7265 7175 6573 7473 272c 2763 6769   'requests','cgi
+000008f0: 272c 2763 6769 7462 272c 2778 6d6c 2e65  ','cgitb','xml.e
+00000900: 7472 6565 2e45 6c65 6d65 6e74 5472 6565  tree.ElementTree
+00000910: 272c 2762 7569 6c74 696e 7327 0d0a 2020  ','builtins'..  
+00000920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000930: 2020 5d0d 0a0d 0a20 2020 2020 2020 2023    ]....        #
+00000940: 2053 6574 2074 6865 2069 6e69 7469 616c   Set the initial
+00000950: 2076 616c 7565 206f 6620 636f 6465 2074   value of code t
+00000960: 6f20 7468 6520 7265 7370 6f6e 7365 0d0a  o the response..
+00000970: 2020 2020 2020 2020 636f 6465 203d 2072          code = r
+00000980: 6573 706f 6e73 650d 0a0d 0a20 2020 2020  esponse....     
+00000990: 2020 2023 2049 6620 7468 6520 7265 7370     # If the resp
+000009a0: 6f6e 7365 2063 6f6e 7461 696e 7320 7468  onse contains th
+000009b0: 6520 7365 7061 7261 746f 722c 2065 7874  e separator, ext
+000009c0: 7261 6374 2074 6865 2063 6f64 6520 626c  ract the code bl
+000009d0: 6f63 6b20 6265 7477 6565 6e20 7468 6520  ock between the 
+000009e0: 7365 7061 7261 746f 7273 0d0a 2020 2020  separators..    
+000009f0: 2020 2020 6966 206c 656e 2872 6573 706f      if len(respo
+00000a00: 6e73 652e 7370 6c69 7428 7365 7061 7261  nse.split(separa
+00000a10: 746f 7229 2920 3e20 313a 0d0a 2020 2020  tor)) > 1:..    
+00000a20: 2020 2020 2020 2020 636f 6465 203d 2072          code = r
+00000a30: 6573 706f 6e73 652e 7370 6c69 7428 7365  esponse.split(se
+00000a40: 7061 7261 746f 7229 5b31 5d0d 0a0d 0a20  parator)[1].... 
+00000a50: 2020 2020 2020 2023 2053 6561 7263 6820         # Search 
+00000a60: 666f 7220 6120 7061 7474 6572 6e20 6265  for a pattern be
+00000a70: 7477 6565 6e20 3c63 6f64 653e 2061 6e64  tween <code> and
+00000a80: 203c 2f63 6f64 653e 2069 6e20 7468 6520   </code> in the 
+00000a90: 6578 7472 6163 7465 6420 636f 6465 0d0a  extracted code..
+00000aa0: 2020 2020 2020 2020 6d61 7463 6820 3d20          match = 
+00000ab0: 7265 2e73 6561 7263 6828 7222 3c63 6f64  re.search(r"<cod
+00000ac0: 653e 282e 2a29 3c2f 636f 6465 3e22 2c20  e>(.*)</code>", 
+00000ad0: 636f 6465 2c20 7265 2e44 4f54 414c 4c29  code, re.DOTALL)
+00000ae0: 0d0a 2020 2020 2020 2020 6966 206d 6174  ..        if mat
+00000af0: 6368 3a0d 0a20 2020 2020 2020 2020 2020  ch:..           
+00000b00: 2023 2049 6620 6120 6d61 7463 6820 6973   # If a match is
+00000b10: 2066 6f75 6e64 2c20 6578 7472 6163 7420   found, extract 
+00000b20: 7468 6520 636f 6465 2062 6574 7765 656e  the code between
+00000b30: 203c 636f 6465 3e20 616e 6420 3c2f 636f   <code> and </co
+00000b40: 6465 3e0d 0a20 2020 2020 2020 2020 2020  de>..           
+00000b50: 2063 6f64 6520 3d20 6d61 7463 682e 6772   code = match.gr
+00000b60: 6f75 7028 3129 0d0a 2020 2020 2020 2020  oup(1)..        
+00000b70: 2020 2020 2320 5265 6d6f 7665 2074 6865      # Remove the
+00000b80: 2022 7079 7468 6f6e 2220 6f72 2022 7079   "python" or "py
+00000b90: 2220 7072 6566 6978 2069 6620 7072 6573  " prefix if pres
+00000ba0: 656e 740d 0a20 2020 2020 2020 2020 2020  ent..           
+00000bb0: 2069 6620 7265 2e6d 6174 6368 2872 225e   if re.match(r"^
+00000bc0: 2870 7974 686f 6e7c 7079 2922 2c20 636f  (python|py)", co
+00000bd0: 6465 293a 0d0a 2020 2020 2020 2020 2020  de):..          
+00000be0: 2020 2020 2020 636f 6465 203d 2072 652e        code = re.
+00000bf0: 7375 6228 7222 5e28 7079 7468 6f6e 7c70  sub(r"^(python|p
+00000c00: 7929 222c 2022 222c 2063 6f64 6529 0d0a  y)", "", code)..
+00000c10: 0d0a 2020 2020 2020 2020 2320 4966 2074  ..        # If t
+00000c20: 6865 2063 6f64 6520 6973 2062 6574 7765  he code is betwe
+00000c30: 656e 2073 696e 676c 6520 6261 636b 7469  en single backti
+00000c40: 636b 732c 2065 7874 7261 6374 2074 6865  cks, extract the
+00000c50: 2063 6f64 6520 6265 7477 6565 6e20 7468   code between th
+00000c60: 656d 0d0a 2020 2020 2020 2020 6966 2072  em..        if r
+00000c70: 652e 6d61 7463 6828 7222 5e60 2e2a 6024  e.match(r"^`.*`$
+00000c80: 222c 2063 6f64 6529 3a0d 0a20 2020 2020  ", code):..     
+00000c90: 2020 2020 2020 2063 6f64 6520 3d20 7265         code = re
+00000ca0: 2e73 7562 2872 225e 6028 2e2a 2960 2422  .sub(r"^`(.*)`$"
+00000cb0: 2c20 7222 5c31 222c 2063 6f64 6529 0d0a  , r"\1", code)..
+00000cc0: 0d0a 2020 2020 2020 2020 2320 5265 6d6f  ..        # Remo
+00000cd0: 7665 2061 6e79 2069 6e73 7461 6e63 6573  ve any instances
+00000ce0: 206f 6620 2264 6620 3d20 7064 2e72 6561   of "df = pd.rea
+00000cf0: 645f 6373 7628 2766 696c 656e 616d 652e  d_csv('filename.
+00000d00: 6373 7627 2922 2066 726f 6d20 7468 6520  csv')" from the 
+00000d10: 636f 6465 0d0a 2020 2020 2020 2020 636f  code..        co
+00000d20: 6465 203d 2072 652e 7375 6228 7222 6466  de = re.sub(r"df
+00000d30: 5c73 2a3d 5c73 2a70 645c 2e72 6561 645f  \s*=\s*pd\.read_
+00000d40: 6373 765c 2827 2e2a 3f27 5c29 222c 2022  csv\('.*?'\)", "
+00000d50: 222c 2063 6f64 6529 0d0a 2020 2020 2020  ", code)..      
+00000d60: 2020 0d0a 2020 2020 2020 2020 2320 5265    ..        # Re
+00000d70: 6d6f 7665 2061 6e79 206f 6363 7572 7265  move any occurre
+00000d80: 6e63 6573 206f 6620 6466 203d 2070 642e  nces of df = pd.
+00000d90: 4461 7461 4672 616d 6528 2920 7769 7468  DataFrame() with
+00000da0: 2061 6e79 206e 756d 6265 7220 6f66 2063   any number of c
+00000db0: 6861 7261 6374 6572 7320 696e 7369 6465  haracters inside
+00000dc0: 2074 6865 2070 6172 656e 7468 6573 6573   the parentheses
+00000dd0: 2e0d 0a20 2020 2020 2020 2063 6f64 6520  ...        code 
+00000de0: 3d20 7265 2e73 7562 2872 2264 665c 732a  = re.sub(r"df\s*
+00000df0: 3d5c 732a 7064 5c2e 4461 7461 4672 616d  =\s*pd\.DataFram
+00000e00: 655c 282e 2a3f 5c29 222c 2022 222c 2063  e\(.*?\)", "", c
+00000e10: 6f64 6529 0d0a 0d0a 2020 2020 2020 2020  ode)....        
+00000e20: 2320 4465 6669 6e65 2074 6865 2072 6567  # Define the reg
+00000e30: 756c 6172 2065 7870 7265 7373 696f 6e20  ular expression 
+00000e40: 7061 7474 6572 6e20 746f 206d 6174 6368  pattern to match
+00000e50: 2074 6865 2062 6c61 636b 6c69 7374 2069   the blacklist i
+00000e60: 7465 6d73 0d0a 2020 2020 2020 2020 7061  tems..        pa
+00000e70: 7474 6572 6e20 3d20 7222 5e28 2e2a 5c62  ttern = r"^(.*\b
+00000e80: 2822 202b 2022 7c22 2e6a 6f69 6e28 626c  (" + "|".join(bl
+00000e90: 6163 6b6c 6973 7429 202b 2072 2229 5c62  acklist) + r")\b
+00000ea0: 2e2a 2924 220d 0a0d 0a20 2020 2020 2020  .*)$"....       
+00000eb0: 2023 2052 6570 6c61 6365 2074 6865 2062   # Replace the b
+00000ec0: 6c61 636b 6c69 7374 2069 7465 6d73 2077  lacklist items w
+00000ed0: 6974 6820 636f 6d6d 656e 7473 0d0a 2020  ith comments..  
+00000ee0: 2020 2020 2020 636f 6465 203d 2072 652e        code = re.
+00000ef0: 7375 6228 7061 7474 6572 6e2c 2072 2223  sub(pattern, r"#
+00000f00: 206e 6f74 2061 6c6c 6f77 6564 205c 3122   not allowed \1"
+00000f10: 2c20 636f 6465 2c20 666c 6167 733d 7265  , code, flags=re
+00000f20: 2e4d 554c 5449 4c49 4e45 290d 0a0d 0a20  .MULTILINE).... 
+00000f30: 2020 2020 2020 2023 2052 6574 7572 6e20         # Return 
+00000f40: 7468 6520 636c 6561 6e65 6420 616e 6420  the cleaned and 
+00000f50: 6578 7472 6163 7465 6420 636f 6465 0d0a  extracted code..
+00000f60: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+00000f70: 6f64 652e 7374 7269 7028 290d 0a0d 0a0d  ode.strip().....
+00000f80: 0a20 2020 2064 6566 2070 645f 6167 656e  .    def pd_agen
+00000f90: 745f 636f 6e76 6572 7365 2873 656c 662c  t_converse(self,
+00000fa0: 2071 7565 7374 696f 6e3d 4e6f 6e65 293a   question=None):
+00000fb0: 0d0a 2020 2020 2020 2020 2320 496e 6974  ..        # Init
+00000fc0: 6961 6c69 7a65 2074 6865 206d 6573 7361  ialize the messa
+00000fd0: 6765 7320 6c69 7374 2077 6974 6820 6120  ges list with a 
+00000fe0: 7379 7374 656d 206d 6573 7361 6765 2063  system message c
+00000ff0: 6f6e 7461 696e 696e 6720 7468 6520 7461  ontaining the ta
+00001000: 736b 2070 726f 6d70 740d 0a20 2020 2020  sk prompt..     
+00001010: 2020 206d 6573 7361 6765 7320 3d20 5b7b     messages = [{
+00001020: 2272 6f6c 6522 3a20 2273 7973 7465 6d22  "role": "system"
+00001030: 2c20 2263 6f6e 7465 6e74 223a 2073 656c  , "content": sel
+00001040: 662e 7461 736b 2e66 6f72 6d61 7428 7365  f.task.format(se
+00001050: 6c66 2e64 665f 6865 6164 2c20 2222 297d  lf.df_head, "")}
+00001060: 5d0d 0a0d 0a20 2020 2020 2020 2023 2046  ]....        # F
+00001070: 756e 6374 696f 6e20 746f 2064 6973 706c  unction to displ
+00001080: 6179 2072 6573 756c 7473 206e 6963 656c  ay results nicel
+00001090: 790d 0a20 2020 2020 2020 2064 6566 2064  y..        def d
+000010a0: 6973 706c 6179 5f72 6573 756c 7473 2861  isplay_results(a
+000010b0: 6e73 7765 722c 2063 6f64 652c 2074 6f74  nswer, code, tot
+000010c0: 616c 5f74 6f6b 656e 735f 7573 6564 5f73  al_tokens_used_s
+000010d0: 756d 293a 0d0a 2020 2020 2020 2020 2020  um):..          
+000010e0: 2020 6966 2027 6970 796b 6572 6e65 6c27    if 'ipykernel'
+000010f0: 2069 6e20 7379 732e 6d6f 6475 6c65 733a   in sys.modules:
+00001100: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001110: 2020 2320 4a75 7079 7465 7220 6e6f 7465    # Jupyter note
+00001120: 626f 6f6b 206f 7220 6970 7974 686f 6e0d  book or ipython.
+00001130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001140: 2064 6973 706c 6179 2848 544d 4c28 6627   display(HTML(f'
+00001150: 3c70 3e3c 6220 7374 796c 653d 2263 6f6c  <p><b style="col
+00001160: 6f72 3a67 7265 656e 3b22 3e41 6e73 7765  or:green;">Answe
+00001170: 723a 3c2f 623e 3c62 723e 3c73 7061 6e20  r:</b><br><span 
+00001180: 7374 796c 653d 2263 6f6c 6f72 3a67 7265  style="color:gre
+00001190: 656e 3b22 3e7b 616e 7377 6572 7d3c 2f73  en;">{answer}</s
+000011a0: 7061 6e3e 3c2f 703e 3c62 723e 2729 290d  pan></p><br>')).
+000011b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000011c0: 2064 6973 706c 6179 2848 544d 4c28 6627   display(HTML(f'
+000011d0: 3c70 3e3c 6220 7374 796c 653d 2263 6f6c  <p><b style="col
+000011e0: 6f72 3a67 7265 656e 3b22 3e43 6f64 653a  or:green;">Code:
+000011f0: 3c2f 623e 3c62 723e 3c73 7061 6e20 7374  </b><br><span st
+00001200: 796c 653d 2263 6f6c 6f72 3a67 7265 656e  yle="color:green
+00001210: 3b22 3e7b 636f 6465 7d3c 2f73 7061 6e3e  ;">{code}</span>
+00001220: 3c2f 703e 3c62 723e 2729 290d 0a20 2020  </p><br>'))..   
+00001230: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+00001240: 706c 6179 2848 544d 4c28 6627 3c70 3e3c  play(HTML(f'<p><
+00001250: 6220 7374 796c 653d 2263 6f6c 6f72 3a67  b style="color:g
+00001260: 7265 656e 3b22 3e54 6f74 616c 2054 6f6b  reen;">Total Tok
+00001270: 656e 7320 5573 6564 3a3c 2f62 3e3c 6272  ens Used:</b><br
+00001280: 3e3c 7370 616e 2073 7479 6c65 3d22 636f  ><span style="co
+00001290: 6c6f 723a 6772 6565 6e3b 223e 7b74 6f74  lor:green;">{tot
+000012a0: 616c 5f74 6f6b 656e 735f 7573 6564 5f73  al_tokens_used_s
+000012b0: 756d 7d3c 2f73 7061 6e3e 3c2f 703e 3c62  um}</span></p><b
+000012c0: 723e 2729 290d 0a20 2020 2020 2020 2020  r>'))..         
+000012d0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+000012e0: 2020 2020 2020 2020 2020 2320 4f74 6865            # Othe
+000012f0: 7220 656e 7669 726f 6e6d 656e 7420 286c  r environment (l
+00001300: 696b 6520 7465 726d 696e 616c 290d 0a20  ike terminal).. 
+00001310: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00001320: 7072 696e 7428 6622 5c6e 416e 7377 6572  print(f"\nAnswer
+00001330: 3a5c 6e7b 616e 7377 6572 7d5c 6e22 2c20  :\n{answer}\n", 
+00001340: 2767 7265 656e 272c 2061 7474 7273 3d5b  'green', attrs=[
+00001350: 2762 6f6c 6427 5d29 0d0a 2020 2020 2020  'bold'])..      
+00001360: 2020 2020 2020 2020 2020 6370 7269 6e74            cprint
+00001370: 2866 2243 6f64 653a 5c6e 7b63 6f64 657d  (f"Code:\n{code}
+00001380: 5c6e 222c 2027 6772 6565 6e27 2c20 6174  \n", 'green', at
+00001390: 7472 733d 5b27 626f 6c64 275d 290d 0a20  trs=['bold']).. 
+000013a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000013b0: 7072 696e 7428 6622 546f 7461 6c20 746f  print(f"Total to
+000013c0: 6b65 6e73 2075 7365 643a 5c6e 7b74 6f74  kens used:\n{tot
+000013d0: 616c 5f74 6f6b 656e 735f 7573 6564 5f73  al_tokens_used_s
+000013e0: 756d 7d5c 6e22 2c20 2779 656c 6c6f 7727  um}\n", 'yellow'
+000013f0: 2c20 6174 7472 733d 5b27 626f 6c64 275d  , attrs=['bold']
+00001400: 290d 0a0d 0a20 2020 2020 2020 2023 2049  )....        # I
+00001410: 6620 6120 7175 6573 7469 6f6e 2069 7320  f a question is 
+00001420: 7072 6f76 6964 6564 2c20 736b 6970 2074  provided, skip t
+00001430: 6865 2069 6e70 7574 2070 726f 6d70 740d  he input prompt.
+00001440: 0a20 2020 2020 2020 2069 6620 7175 6573  .        if ques
+00001450: 7469 6f6e 2069 7320 6e6f 7420 4e6f 6e65  tion is not None
+00001460: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
+00001470: 2043 616c 6c20 7468 6520 7064 5f61 6765   Call the pd_age
+00001480: 6e74 206d 6574 686f 6420 7769 7468 2074  nt method with t
+00001490: 6865 2075 7365 7227 7320 7175 6573 7469  he user's questi
+000014a0: 6f6e 2c20 7468 6520 6d65 7373 6167 6573  on, the messages
+000014b0: 206c 6973 742c 2061 6e64 2074 6865 2064   list, and the d
+000014c0: 6174 6166 7261 6d65 0d0a 2020 2020 2020  ataframe..      
+000014d0: 2020 2020 2020 616e 7377 6572 2c20 636f        answer, co
+000014e0: 6465 2c20 746f 7461 6c5f 746f 6b65 6e73  de, total_tokens
+000014f0: 5f75 7365 645f 7375 6d20 3d20 7365 6c66  _used_sum = self
+00001500: 2e70 645f 6167 656e 7428 7175 6573 7469  .pd_agent(questi
+00001510: 6f6e 2c20 6d65 7373 6167 6573 2c20 7365  on, messages, se
+00001520: 6c66 2e64 6629 0d0a 2020 2020 2020 2020  lf.df)..        
+00001530: 2020 2020 6469 7370 6c61 795f 7265 7375      display_resu
+00001540: 6c74 7328 616e 7377 6572 2c20 636f 6465  lts(answer, code
+00001550: 2c20 746f 7461 6c5f 746f 6b65 6e73 5f75  , total_tokens_u
+00001560: 7365 645f 7375 6d29 0d0a 2020 2020 2020  sed_sum)..      
+00001570: 2020 2020 2020 7265 7475 726e 0d0a 0d0a        return....
+00001580: 2020 2020 2020 2020 2320 5374 6172 7420          # Start 
+00001590: 616e 2069 6e66 696e 6974 6520 6c6f 6f70  an infinite loop
+000015a0: 2074 6f20 6b65 6570 2061 736b 696e 6720   to keep asking 
+000015b0: 7468 6520 7573 6572 2066 6f72 2071 7565  the user for que
+000015c0: 7374 696f 6e73 0d0a 2020 2020 2020 2020  stions..        
+000015d0: 7768 696c 6520 5472 7565 3a0d 0a20 2020  while True:..   
+000015e0: 2020 2020 2020 2020 2023 2050 726f 6d70           # Promp
+000015f0: 7420 7468 6520 7573 6572 2074 6f20 656e  t the user to en
+00001600: 7465 7220 6120 7175 6573 7469 6f6e 206f  ter a question o
+00001610: 7220 7479 7065 2027 6578 6974 2720 746f  r type 'exit' to
+00001620: 2071 7569 740d 0a20 2020 2020 2020 2020   quit..         
+00001630: 2020 2069 6620 2769 7079 6b65 726e 656c     if 'ipykernel
+00001640: 2720 696e 2073 7973 2e6d 6f64 756c 6573  ' in sys.modules
+00001650: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00001660: 2020 2064 6973 706c 6179 2848 544d 4c28     display(HTML(
+00001670: 273c 6220 7374 796c 653d 2263 6f6c 6f72  '<b style="color
+00001680: 3a62 6c75 653b 223e 456e 7465 7220 796f  :blue;">Enter yo
+00001690: 7572 2071 7565 7374 696f 6e20 6f72 2074  ur question or t
+000016a0: 7970 6520 5c27 6578 6974 5c27 2074 6f20  ype \'exit\' to 
+000016b0: 7175 6974 3a3c 2f62 3e27 2929 0d0a 2020  quit:</b>'))..  
+000016c0: 2020 2020 2020 2020 2020 2020 2020 7175                qu
+000016d0: 6573 7469 6f6e 203d 2069 6e70 7574 2829  estion = input()
+000016e0: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+000016f0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00001700: 2020 2020 2063 7072 696e 7428 225c 6e45       cprint("\nE
+00001710: 6e74 6572 2079 6f75 7220 7175 6573 7469  nter your questi
+00001720: 6f6e 206f 7220 7479 7065 2027 6578 6974  on or type 'exit
+00001730: 2720 746f 2071 7569 743a 222c 2027 626c  ' to quit:", 'bl
+00001740: 7565 272c 2061 7474 7273 3d5b 2762 6f6c  ue', attrs=['bol
+00001750: 6427 5d29 0d0a 2020 2020 2020 2020 2020  d'])..          
+00001760: 2020 2020 2020 7175 6573 7469 6f6e 203d        question =
+00001770: 2069 6e70 7574 2829 0d0a 0d0a 2020 2020   input()....    
+00001780: 2020 2020 2020 2020 2320 4966 2074 6865          # If the
+00001790: 2075 7365 7220 7479 7065 7320 2765 7869   user types 'exi
+000017a0: 7427 2c20 6272 6561 6b20 6f75 7420 6f66  t', break out of
+000017b0: 2074 6865 206c 6f6f 700d 0a20 2020 2020   the loop..     
+000017c0: 2020 2020 2020 2069 6620 7175 6573 7469         if questi
+000017d0: 6f6e 2e73 7472 6970 2829 2e6c 6f77 6572  on.strip().lower
+000017e0: 2829 203d 3d20 2765 7869 7427 3a0d 0a20  () == 'exit':.. 
+000017f0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00001800: 7265 616b 0d0a 0d0a 2020 2020 2020 2020  reak....        
+00001810: 2020 2020 2320 4361 6c6c 2074 6865 2070      # Call the p
+00001820: 645f 6167 656e 7420 6d65 7468 6f64 2077  d_agent method w
+00001830: 6974 6820 7468 6520 7573 6572 2773 2071  ith the user's q
+00001840: 7565 7374 696f 6e2c 2074 6865 206d 6573  uestion, the mes
+00001850: 7361 6765 7320 6c69 7374 2c20 616e 6420  sages list, and 
+00001860: 7468 6520 6461 7461 6672 616d 650d 0a20  the dataframe.. 
+00001870: 2020 2020 2020 2020 2020 2061 6e73 7765             answe
+00001880: 722c 2063 6f64 652c 2074 6f74 616c 5f74  r, code, total_t
+00001890: 6f6b 656e 735f 7573 6564 5f73 756d 203d  okens_used_sum =
+000018a0: 2073 656c 662e 7064 5f61 6765 6e74 2871   self.pd_agent(q
+000018b0: 7565 7374 696f 6e2c 206d 6573 7361 6765  uestion, message
+000018c0: 732c 2073 656c 662e 6466 290d 0a20 2020  s, self.df)..   
+000018d0: 2020 2020 2020 2020 2064 6973 706c 6179           display
+000018e0: 5f72 6573 756c 7473 2861 6e73 7765 722c  _results(answer,
+000018f0: 2063 6f64 652c 2074 6f74 616c 5f74 6f6b   code, total_tok
+00001900: 656e 735f 7573 6564 5f73 756d 290d 0a0d  ens_used_sum)...
+00001910: 0a20 2020 2064 6566 2070 645f 6167 656e  .    def pd_agen
+00001920: 7428 7365 6c66 2c20 7175 6573 7469 6f6e  t(self, question
+00001930: 2c20 6d65 7373 6167 6573 2c20 6466 3d4e  , messages, df=N
+00001940: 6f6e 6529 3a0d 0a20 2020 2020 2020 2023  one):..        #
+00001950: 2041 6464 2061 2075 7365 7220 6d65 7373   Add a user mess
+00001960: 6167 6520 7769 7468 2074 6865 2075 7064  age with the upd
+00001970: 6174 6564 2074 6173 6b20 7072 6f6d 7074  ated task prompt
+00001980: 2074 6f20 7468 6520 6d65 7373 6167 6573   to the messages
+00001990: 206c 6973 740d 0a20 2020 2020 2020 206d   list..        m
+000019a0: 6573 7361 6765 732e 6170 7065 6e64 287b  essages.append({
+000019b0: 2272 6f6c 6522 3a20 2275 7365 7222 2c20  "role": "user", 
+000019c0: 2263 6f6e 7465 6e74 223a 2073 656c 662e  "content": self.
+000019d0: 7461 736b 2e66 6f72 6d61 7428 7365 6c66  task.format(self
+000019e0: 2e64 665f 6865 6164 2c20 7175 6573 7469  .df_head, questi
+000019f0: 6f6e 297d 290d 0a0d 0a20 2020 2020 2020  on)})....       
+00001a00: 2023 2043 616c 6c20 7468 6520 4f70 656e   # Call the Open
+00001a10: 4149 2041 5049 2061 6e64 2068 616e 646c  AI API and handl
+00001a20: 6520 7261 7465 206c 696d 6974 2065 7272  e rate limit err
+00001a30: 6f72 730d 0a20 2020 2020 2020 2074 7279  ors..        try
+00001a40: 3a0d 0a20 2020 2020 2020 2020 2020 2063  :..            c
+00001a50: 6f64 652c 2074 6f6b 656e 735f 7573 6564  ode, tokens_used
+00001a60: 203d 2073 656c 662e 6c6c 6d5f 6361 6c6c   = self.llm_call
+00001a70: 286d 6573 7361 6765 7329 0d0a 2020 2020  (messages)..    
+00001a80: 2020 2020 6578 6365 7074 206f 7065 6e61      except opena
+00001a90: 692e 6572 726f 722e 5261 7465 4c69 6d69  i.error.RateLimi
+00001aa0: 7445 7272 6f72 3a0d 0a20 2020 2020 2020  tError:..       
+00001ab0: 2020 2020 2070 7269 6e74 280d 0a20 2020       print(..   
+00001ac0: 2020 2020 2020 2020 2020 2020 2022 5468               "Th
+00001ad0: 6520 4f70 656e 4149 2041 5049 2072 6174  e OpenAI API rat
+00001ae0: 6520 6c69 6d69 7420 6861 7320 6265 656e  e limit has been
+00001af0: 2065 7863 6565 6465 642e 2057 6169 7469   exceeded. Waiti
+00001b00: 6e67 2031 3020 7365 636f 6e64 7320 616e  ng 10 seconds an
+00001b10: 6420 7472 7969 6e67 2061 6761 696e 2e22  d trying again."
+00001b20: 0d0a 2020 2020 2020 2020 2020 2020 290d  ..            ).
+00001b30: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
+00001b40: 652e 736c 6565 7028 3130 290d 0a20 2020  e.sleep(10)..   
+00001b50: 2020 2020 2020 2020 2063 6f64 652c 2074           code, t
+00001b60: 6f6b 656e 735f 7573 6564 203d 2073 656c  okens_used = sel
+00001b70: 662e 6c6c 6d5f 6361 6c6c 286d 6573 7361  f.llm_call(messa
+00001b80: 6765 7329 0d0a 0d0a 2020 2020 2020 2020  ges)....        
+00001b90: 2320 4578 7472 6163 7420 7468 6520 636f  # Extract the co
+00001ba0: 6465 2066 726f 6d20 7468 6520 4150 4920  de from the API 
+00001bb0: 7265 7370 6f6e 7365 0d0a 2020 2020 2020  response..      
+00001bc0: 2020 636f 6465 203d 2073 656c 662e 5f65    code = self._e
+00001bd0: 7874 7261 6374 5f63 6f64 6528 636f 6465  xtract_code(code
+00001be0: 290d 0a0d 0a20 2020 2020 2020 2023 2055  )....        # U
+00001bf0: 7064 6174 6520 7468 6520 746f 7461 6c20  pdate the total 
+00001c00: 746f 6b65 6e73 2075 7365 640d 0a20 2020  tokens used..   
+00001c10: 2020 2020 2073 656c 662e 746f 7461 6c5f       self.total_
+00001c20: 746f 6b65 6e73 5f75 7365 642e 6170 7065  tokens_used.appe
+00001c30: 6e64 2874 6f6b 656e 735f 7573 6564 290d  nd(tokens_used).
+00001c40: 0a20 2020 2020 2020 2074 6f74 616c 5f74  .        total_t
+00001c50: 6f6b 656e 735f 7573 6564 5f73 756d 203d  okens_used_sum =
+00001c60: 2073 756d 2873 656c 662e 746f 7461 6c5f   sum(self.total_
+00001c70: 746f 6b65 6e73 5f75 7365 6429 0d0a 0d0a  tokens_used)....
+00001c80: 2020 2020 2020 2020 2320 496e 6974 6961          # Initia
+00001c90: 6c69 7a65 2065 7272 6f72 2063 6f72 7265  lize error corre
+00001ca0: 6374 696f 6e20 636f 756e 7465 720d 0a20  ction counter.. 
+00001cb0: 2020 2020 2020 2065 7272 6f72 5f63 6f72         error_cor
+00001cc0: 7265 6374 696f 6e73 203d 2030 0d0a 0d0a  rections = 0....
+00001cd0: 2020 2020 2020 2020 2320 5265 6469 7265          # Redire
+00001ce0: 6374 2073 7461 6e64 6172 6420 6f75 7470  ct standard outp
+00001cf0: 7574 2074 6f20 6120 5374 7269 6e67 494f  ut to a StringIO
+00001d00: 2062 7566 6665 720d 0a20 2020 2020 2020   buffer..       
+00001d10: 2077 6974 6820 7265 6469 7265 6374 5f73   with redirect_s
+00001d20: 7464 6f75 7428 696f 2e53 7472 696e 6749  tdout(io.StringI
+00001d30: 4f28 2929 2061 7320 6f75 7470 7574 3a0d  O()) as output:.
+00001d40: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
+00001d50: 7279 2074 6f20 6578 6563 7574 6520 7468  ry to execute th
+00001d60: 6520 636f 6465 2061 6e64 2068 616e 646c  e code and handl
+00001d70: 6520 6572 726f 7273 0d0a 2020 2020 2020  e errors..      
+00001d80: 2020 2020 2020 7768 696c 6520 6572 726f        while erro
+00001d90: 725f 636f 7272 6563 7469 6f6e 7320 3c20  r_corrections < 
+00001da0: 7365 6c66 2e4d 4158 5f45 5252 4f52 5f43  self.MAX_ERROR_C
+00001db0: 4f52 5245 4354 494f 4e53 3a0d 0a20 2020  ORRECTIONS:..   
+00001dc0: 2020 2020 2020 2020 2020 2020 2074 7279               try
+00001dd0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00001de0: 2020 2020 2020 206d 6573 7361 6765 732e         messages.
+00001df0: 6170 7065 6e64 287b 2272 6f6c 6522 3a20  append({"role": 
+00001e00: 2261 7373 6973 7461 6e74 222c 2022 636f  "assistant", "co
+00001e10: 6e74 656e 7422 3a20 636f 6465 7d29 0d0a  ntent": code})..
+00001e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e30: 2020 2020 6578 6563 2863 6f64 6529 0d0a      exec(code)..
+00001e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e50: 2020 2020 6272 6561 6b0d 0a20 2020 2020      break..     
+00001e60: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00001e70: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00001e80: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00001e90: 2020 2020 2020 2023 2049 6e63 7265 6d65         # Increme
+00001ea0: 6e74 2074 6865 2065 7272 6f72 2063 6f72  nt the error cor
+00001eb0: 7265 6374 696f 6e20 636f 756e 7465 7220  rection counter 
+00001ec0: 616e 6420 7570 6461 7465 2074 6865 206d  and update the m
+00001ed0: 6573 7361 6765 7320 6c69 7374 2077 6974  essages list wit
+00001ee0: 6820 7468 6520 6572 726f 720d 0a20 2020  h the error..   
+00001ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f00: 2065 7272 6f72 5f63 6f72 7265 6374 696f   error_correctio
+00001f10: 6e73 202b 3d20 310d 0a20 2020 2020 2020  ns += 1..       
+00001f20: 2020 2020 2020 2020 2020 2020 206d 6573               mes
+00001f30: 7361 6765 732e 6170 7065 6e64 287b 2272  sages.append({"r
+00001f40: 6f6c 6522 3a20 2275 7365 7222 2c20 2263  ole": "user", "c
+00001f50: 6f6e 7465 6e74 223a 2073 656c 662e 6572  ontent": self.er
+00001f60: 726f 725f 636f 7272 6563 745f 7461 736b  ror_correct_task
+00001f70: 2e66 6f72 6d61 7428 652c 2063 6f64 652c  .format(e, code,
+00001f80: 2071 7565 7374 696f 6e29 7d29 0d0a 0d0a   question)})....
+00001f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fa0: 2020 2020 2320 4174 7465 6d70 7420 746f      # Attempt to
+00001fb0: 2063 6f72 7265 6374 2074 6865 2063 6f64   correct the cod
+00001fc0: 6520 616e 6420 6861 6e64 6c65 2072 6174  e and handle rat
+00001fd0: 6520 6c69 6d69 7420 6572 726f 7273 0d0a  e limit errors..
+00001fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ff0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00002000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002010: 2020 636f 6465 2c20 746f 6b65 6e73 5f75    code, tokens_u
+00002020: 7365 6420 3d20 7365 6c66 2e6c 6c6d 5f63  sed = self.llm_c
+00002030: 616c 6c28 6d65 7373 6167 6573 290d 0a20  all(messages).. 
+00002040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002050: 2020 2020 2020 2063 6f64 6520 3d20 7365         code = se
+00002060: 6c66 2e5f 6578 7472 6163 745f 636f 6465  lf._extract_code
+00002070: 2863 6f64 6529 0d0a 2020 2020 2020 2020  (code)..        
+00002080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002090: 7365 6c66 2e74 6f74 616c 5f74 6f6b 656e  self.total_token
+000020a0: 735f 7573 6564 2e61 7070 656e 6428 746f  s_used.append(to
+000020b0: 6b65 6e73 5f75 7365 6429 0d0a 2020 2020  kens_used)..    
+000020c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020d0: 2020 2020 746f 7461 6c5f 746f 6b65 6e73      total_tokens
+000020e0: 5f75 7365 645f 7375 6d20 3d20 7375 6d28  _used_sum = sum(
+000020f0: 7365 6c66 2e74 6f74 616c 5f74 6f6b 656e  self.total_token
+00002100: 735f 7573 6564 290d 0a20 2020 2020 2020  s_used)..       
+00002110: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+00002120: 6570 7420 6f70 656e 6169 2e65 7272 6f72  ept openai.error
+00002130: 2e52 6174 654c 696d 6974 4572 726f 723a  .RateLimitError:
+00002140: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002150: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00002160: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002170: 2020 2020 2020 2020 2020 2020 2020 2254                "T
+00002180: 6865 204f 7065 6e41 4920 4150 4920 7261  he OpenAI API ra
+00002190: 7465 206c 696d 6974 2068 6173 2062 6565  te limit has bee
+000021a0: 6e20 6578 6365 6564 6564 2e20 5761 6974  n exceeded. Wait
+000021b0: 696e 6720 3130 2073 6563 6f6e 6473 2061  ing 10 seconds a
+000021c0: 6e64 2074 7279 696e 6720 6167 6169 6e2e  nd trying again.
+000021d0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+000021e0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+000021f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002200: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
+00002210: 2831 3029 0d0a 2020 2020 2020 2020 2020  (10)..          
+00002220: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00002230: 6465 2c20 746f 6b65 6e73 5f75 7365 6420  de, tokens_used 
+00002240: 3d20 7365 6c66 2e6c 6c6d 5f63 616c 6c28  = self.llm_call(
+00002250: 6d65 7373 6167 6573 290d 0a20 2020 2020  messages)..     
+00002260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002270: 2020 2063 6f64 6520 3d20 7365 6c66 2e5f     code = self._
+00002280: 6578 7472 6163 745f 636f 6465 2863 6f64  extract_code(cod
+00002290: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+000022a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000022b0: 2e74 6f74 616c 5f74 6f6b 656e 735f 7573  .total_tokens_us
+000022c0: 6564 2e61 7070 656e 6428 746f 6b65 6e73  ed.append(tokens
+000022d0: 5f75 7365 6429 0d0a 2020 2020 2020 2020  _used)..        
+000022e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022f0: 746f 7461 6c5f 746f 6b65 6e73 5f75 7365  total_tokens_use
+00002300: 645f 7375 6d20 3d20 7375 6d28 7365 6c66  d_sum = sum(self
+00002310: 2e74 6f74 616c 5f74 6f6b 656e 735f 7573  .total_tokens_us
+00002320: 6564 290d 0a0d 0a20 2020 2020 2020 2023  ed)....        #
+00002330: 2047 6574 2074 6865 206f 7574 7075 7420   Get the output 
+00002340: 6672 6f6d 2074 6865 2065 7865 6375 7465  from the execute
+00002350: 6420 636f 6465 0d0a 2020 2020 2020 2020  d code..        
+00002360: 616e 7377 6572 203d 206f 7574 7075 742e  answer = output.
+00002370: 6765 7476 616c 7565 2829 0d0a 0d0a 2020  getvalue()....  
+00002380: 2020 2020 2020 7265 7475 726e 2061 6e73        return ans
+00002390: 7765 722c 2063 6f64 652c 2074 6f74 616c  wer, code, total
+000023a0: 5f74 6f6b 656e 735f 7573 6564 5f73 756d  _tokens_used_sum
+000023b0: 0d0a 2020 2020 0d0a 0d0a 2020 2020       ..    ....
```

### Comparing `bambooai-0.1.1/bambooai.egg-info/PKG-INFO` & `bambooai-0.1.2/bambooai.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambooai
-Version: 0.1.1
+Version: 0.1.2
 Summary: A lightweight library for working with pandas dataframes using natural language queries
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,20 @@
 
 ## Objective
 
 The BambooAI library is a user-friendly tool designed to make data analysis more accessible to non-programmers. Utilizing the power of Large Language Models (LLM), BambooAI can comprehend your questions about a dataset and automatically generate and execute the appropriate Python code for both analysis and plotting. Users can effortlessly gain valuable insights from their data without writing complex code or mastering advanced programming techniques. With BambooAI, simply input your dataset, ask questions in plain English, and receive answers along with relevant out of the box visualizations if asked for to help you better understand your data.
 
 My aim was to keep the code base under 150 lines of actual code (not counting comments and blanks) to ensure easy comprehension and clarity for users of various skill levels. By maintaining a concise code base, I strived to create an accessible and straightforward tool that streamlines the process of data analysis and visualization. This approach not only makes it easier for developers and users to understand the library's inner workings but also fosters efficient implementation and customization, catering to a diverse audience and their unique needs.
 
+## Preview
+
+Try it out in Google Colab:
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1grKtqKD4u8cVGMoVv__umci4F7IU14vU?usp=sharing)
+
 ## How it works
 
 - User starts BambooAI
 - BambooAI checks if a question is provided
   - If a question is given programmatically, it gets processed and the assistant exits after the execution
   - If no question is provided programaticaly, BambooAI prompts the user for one and enters a loop of questions and answers, remembering the conversation history
     - Sends each question to the OpenAI API LLM along with the conversation history
```

### Comparing `bambooai-0.1.1/setup.py` & `bambooai-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='bambooai',
-    version='0.1.1',
+    version='0.1.2',
     description='A lightweight library for working with pandas dataframes using natural language queries',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         'openai',
         'pandas',
```

