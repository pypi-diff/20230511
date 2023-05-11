# Comparing `tmp/fdcalls-1.2-py3-none-any.whl.zip` & `tmp/fdcalls-1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4616 bytes, number of entries: 7
+Zip file size: 4874 bytes, number of entries: 7
 -rw-r--r--  2.0 unx        0 b- defN 23-May-08 12:39 fdcalls/__init__.py
--rw-r--r--  2.0 unx    15534 b- defN 23-May-08 13:05 fdcalls/fdcalls.py
--rw-r--r--  2.0 unx      274 b- defN 23-May-09 11:28 fdcalls-1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-09 11:28 fdcalls-1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 23-May-09 11:28 fdcalls-1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-May-09 11:28 fdcalls-1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      530 b- defN 23-May-09 11:28 fdcalls-1.2.dist-info/RECORD
-7 files, 16488 bytes uncompressed, 3672 bytes compressed:  77.7%
+-rw-r--r--  2.0 unx    16413 b- defN 23-May-11 09:19 fdcalls/fdcalls.py
+-rw-r--r--  2.0 unx      274 b- defN 23-May-11 09:48 fdcalls-1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-11 09:48 fdcalls-1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-May-11 09:48 fdcalls-1.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-May-11 09:48 fdcalls-1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      530 b- defN 23-May-11 09:48 fdcalls-1.3.dist-info/RECORD
+7 files, 17367 bytes uncompressed, 3930 bytes compressed:  77.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: fdcalls/__init__.py
 Comment: 
 
 Filename: fdcalls/fdcalls.py
 Comment: 
 
-Filename: fdcalls-1.2.dist-info/METADATA
+Filename: fdcalls-1.3.dist-info/METADATA
 Comment: 
 
-Filename: fdcalls-1.2.dist-info/WHEEL
+Filename: fdcalls-1.3.dist-info/WHEEL
 Comment: 
 
-Filename: fdcalls-1.2.dist-info/entry_points.txt
+Filename: fdcalls-1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: fdcalls-1.2.dist-info/top_level.txt
+Filename: fdcalls-1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: fdcalls-1.2.dist-info/RECORD
+Filename: fdcalls-1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fdcalls/fdcalls.py

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import sys
+import json
 import r2pipe
 import argparse
 import subprocess
 
 
 dangerous_functions = ['sym.imp.system', 'sym.imp.popen', 'sym.imp.execve']
 command_injection_addr = []
@@ -49,15 +50,15 @@
 
          .o88o.       .o8                      oooo  oooo           
          888 `"      "888                      `888  `888           
         o888oo   .oooo888   .ooooo.   .oooo.    888   888   .oooo.o 
          888    d88' `888  d88' `"Y8 `P  )88b   888   888  d88(  "8 
          888    888   888  888        .oP"888   888   888  `"Y88b.  
          888    888   888  888   .o8 d8(  888   888   888  o.  )88b 
-        o888o   `Y8bod88P" `Y8bod8P' `Y888""8o o888o o888o 8""888P'   author:fxc  version:1.2
+        o888o   `Y8bod88P" `Y8bod8P' `Y888""8o o888o o888o 8""888P'
                                                             
     """)
 
 def add_colour(string, colour = 'white'):
     if colour == 'red':
         return f'\033[1;31m{string}\033[0m'
     elif colour == 'yellow':
@@ -72,139 +73,178 @@
 # Obtain the relative path of the file
 def get_path_by_filename(filename, file_system_path):
     output = subprocess.check_output(['find', file_system_path, '-name', filename]).decode('utf-8')
     for line in output.split('\n'):
         return line
 
 # Obtain relevant dynamic link library names
-def get_dynamic_libraries(target_file_path, file_system_path):
+def get_dynamic_libraries(r2fd, file_system_path):
+    '''
     output = subprocess.check_output(['readelf', '-d', target_file_path]).decode('utf-8')
     libraries = []
     for line in output.split('\n'):
         if 'Shared library' in line:
             library = line.split('[')[-1].split(']')[0]
             library = get_path_by_filename(library, file_system_path)
             libraries.append(library)
+    '''
+    libraries = []
+    libs = r2fd.cmdj('ilj')
+    for lib in libs:
+        library = get_path_by_filename(lib, file_system_path)
+        libraries.append(library)
+
     return libraries
 
 # Obtain function names in target file
 def get_function_names(r2fd, mode):
     function_names = []
     function_name = ''
     functions = r2fd.cmdj('aflj')
     if mode == 0:
         for function in functions:
-            #print(function)
+            # print(function)
             if 'sym.imp' in function['name']:
                 function_name = function['name']
-                #print(function_name)
+                # print(function_name)
                 function_names.append(function_name) 
     else:
         for function in functions:
-            #print(function)
+            # print(function)
             if 'sym.imp' not in function['name']:
                 function_name = function['name']
-                #print(function_name)
+                # print(function_name)
                 function_names.append(function_name) 
     return function_names
 
+# start r2 analysis
 def r2_start_analysis(filepath):
     r2fd = r2pipe.open(filepath)
     r2fd.cmd('aaa')
      
     return r2fd
 
+# get architecture of binary
+def get_architecture(r2fd):
+    info = json.loads(r2fd.cmd('iIj'))
+    return info["arch"]
+
 # Obtain the function called internally from the function
+'''
+for example:
+    int FunA(){
+        system(...);
+        printf(...);
+    }
+    we will get:
+    function_called_functions[A] = ['system', 'printf']
+
+    differnet arch may be a little difference while coding
+'''
 def get_functions_called(r2fd, filename, arch):
 
     function_called_functions = {}
     functions = []
     function_name = ''
     length = 0
     
     if arch == 'arm':
         for fun in functions_self_defined[filename]:
-            #print(fun)
+            # print(fun)
             functions = []
             disassembly = r2fd.cmd(f'pdf @ {fun} 2>/dev/null')
             for line in disassembly.split('\n'):
                 function_name = ''
                 if 'sym' in line:
-                    #print(line)
+                    # print(line)
                     line1 = line[line.rfind('sym'):]
                     if line1.find(' ') != -1:
                         length = line1.find(' ')
                     else:
                         length = len(line1)
-                    #print(length)
-                    #print(line[line.find('sym'):line.find('sym')+length])
+                    # print(length)
+                    # print(line[line.find('sym'):line.find('sym')+length])
                     function_name = line[line.find('sym'):line.find('sym')+length]
                 elif 'fcn' in line:
-                    #print(line)
+                    # print(line)
                     line1 = line[line.find('fcn'):]
                     if line1.find(' ') != -1:
                         length = line1.find(' ')
                     else:
                         length = len(line1)
-                    #print(length)
-                    #print(line[line.find('fcn'):line.find('fcn')+length])
+                    # print(length)
+                    # print(line[line.find('fcn'):line.find('fcn')+length])
                     function_name = line[line.find('fcn'):line.find('fcn')+length]
                 if function_name != '' and function_name!=fun and function_name not in functions:
                     functions.append(function_name)
             function_called_functions[fun] = functions
-            #print(function_called_functions[fun])
-        #print(function_called_functions)
+            # print(function_called_functions[fun])
+        # print(function_called_functions)
     if arch == 'mips':
         for fun in functions_self_defined[filename]:
-            #print(fun)
+            # print(fun)
             functions = []
             disassembly = r2fd.cmd(f'pdf @ {fun} 2>/dev/null')
             for line in disassembly.split('\n'):
                 function_name = ''
                 if 'sym' in line and 'XREF' not in line:
-                    #print(line)
+                    # print(line)
                     line1 = line[line.rfind('sym'):]
                     if line1.find(' ') != -1:
                         length = line1.find(' ')
                     else:
                         length = len(line1)
-                    #print(length)
-                    #print(line[line.find('sym'):line.find('sym')+length])
+                    # print(length)
+                    # print(line[line.find('sym'):line.find('sym')+length])
                     function_name = line[line.find('sym'):line.find('sym')+length]
                 elif 'fcn' in line and 'XREF' not in line:
-                    #print(line)
+                    # print(line)
                     line1 = line[line.find('fcn'):]
                     if line1.find(' ') != -1:
                         length = line1.find(' ')
                     else:
                         length = len(line1)
-                    #print(length)
-                    #print(line[line.find('fcn'):line.find('fcn')+length])
+                    # print(length)
+                    # print(line[line.find('fcn'):line.find('fcn')+length])
                     function_name = line[line.find('fcn'):line.find('fcn')+length]
                 if function_name != '' and function_name!=fun and function_name not in functions:
                     functions.append(function_name)
             function_called_functions[fun] = functions
-            #print(function_called_functions[fun])
-        #print(function_called_functions)
+            # print(function_called_functions[fun])
+        # print(function_called_functions)
     return function_called_functions
 
 # Obtaining a dangerous function call chain
+'''
+for example:
+    int FunA(){
+        FunB();
+        puts(...);
+    }
+    int FunB(){
+        system(...);
+        printf(...);
+    }
+    we will get:
+    dangerous_fun[A] = ['FunB', 'system']
+    dangerous_fun[B] = ['system']
+'''
 def get_dangerous_chains(dangerous_fun, pre_fun):
     dangerous_fun = [dangerous_fun]
     
     dangerous_fun+= dangerous_functions_chain[pre_fun]
     return dangerous_fun
     
 
 def find_command_injection(r2fd, filename):
     cmdinjection = []
     banned_funcs = []
 
     for fun in functions_self_defined[filename]:
-        #print(fun)
+        # print(fun)
         disassembly = r2fd.cmd(f'pdf @ {fun} 2>/dev/null')
         for line in disassembly.split('\n'):
             for func in dangerous_functions:
                 func_chain = ''
                 if func in line and fun != func:
                     addr = line[line.find('0x'):line.find('0x')+10]
                     cnt = 0    
@@ -233,20 +273,20 @@
                             func_chain+= add_colour(function_to_library[s], 'cyan')
                             func_chain+= '] '
                             func_chain+= add_colour(s, 'yellow')
                             cnt+= 1
                         else:
                             func_chain+= add_colour(f, 'yellow')
                             cnt+= 1
-                    #print(func_chain)
+                    # print(func_chain)
                     cmdinjection.append(func_chain)
 
-                    #print(fun + f'({addr}) ->' + func)
-                    #print(dangerous_functions_chain[func])
-                    #print(line)
+                    # print(fun + f'({addr}) ->' + func)
+                    # print(dangerous_functions_chain[func])
+                    # print(line)
     return cmdinjection
 
 # Add the filename before the functionname
 def add_filename_to_function(filename, functionname):
     if 'sym.imp' in functionname:
         return functionname
     else:
@@ -258,82 +298,80 @@
         if 'sym.imp' in fun:
             fun = fun.replace('sym.imp', 'sym')
             if fun in function_to_library.keys():
             	print('[' + add_colour(function_to_library[fun], 'cyan') + '] ' + add_colour(fun, 'yellow'))
 
 def main():
     parser = argparse.ArgumentParser(description="fdcalls to help analysis")
-    parser.add_argument('-p', '--path', type=str, default='', help='path to target binary')
-    parser.add_argument('-f', '--file_system_path', type=str, default='', help='path to file path')
-    parser.add_argument('-a', '--arch', type=str, default='', help='arch of target binary')
+    parser.version = "1.3"
+
+    parser.add_argument('-b', '--target_binary_path', type=str, default='', help='path to target binary')
+    parser.add_argument('-d', '--file_system_directory_path', type=str, default='', help='path to firmware file system directory')
     parser.add_argument('-l', '--level', type=int, default=0, help='level of analysis')
+    parser.add_argument('-v', action='version', help='print the version and exit')
     args = parser.parse_args()
 
-    target_filepath = args.path
-    file_system_path = args.file_system_path
-    architecture = args.arch
+    target_filepath = args.target_binary_path
+    file_system_path = args.file_system_directory_path
     level = args.level
     
-    if target_filepath == ''or architecture == '':
-        print('./dcalls.py -p [path/to/target_binary] -f [path/to/file_system_dir] -a [arch] -l [level=0]')
+    if target_filepath == '':
+        print('./dcalls.py -b [path/to/target_binary] -d [path/to/file_system_dir] -a [arch] -l [level=0]')
         exit(0)
     
     init()
-    
-    print("[*] Collecting libraries ...")
-    dynamic_libraries[target_filepath] = get_dynamic_libraries(target_filepath, file_system_path)
+
+    print("[*] Collecting and analysing binaries ...")
+    r2_fd[target_filepath] = r2_start_analysis(target_filepath)
+    dynamic_libraries[target_filepath] = get_dynamic_libraries(r2_fd[target_filepath], file_system_path)
     for f in dynamic_libraries[target_filepath]:
-        if f not in all_used_dynamic_libraries:
-            all_used_dynamic_libraries.append(f)
-        dynamic_libraries[f] = get_dynamic_libraries(f, file_system_path)
+        r2_fd[f] = r2_start_analysis(f)
+        all_used_dynamic_libraries.append(f)
+        dynamic_libraries[f] = get_dynamic_libraries(r2_fd[f], file_system_path)
         for lib in dynamic_libraries[f]:
             if lib not in all_used_dynamic_libraries:
                 all_used_dynamic_libraries.append(lib)
-        #print(f + "=> ", end = '')
-        #print(get_dynamic_libraries(f, file_system_path))
-
-    for f in all_used_dynamic_libraries:
-        if f not in dynamic_libraries.keys():
-            dynamic_libraries[f] = get_dynamic_libraries(f, file_system_path)
-            #print(f + "=> ", end = '')
-            #print(get_dynamic_libraries(f, file_system_path))
-    #print(all_used_dynamic_libraries)
-    print("[+] Get libraries success")
+        # print(f + "=> ", end = '')
+        # print(get_dynamic_libraries(r2_fd[f], file_system_path))
     
-    print("[*] Analysis elf and libraries ...")
-    r2_fd[target_filepath] = r2_start_analysis(target_filepath)
     for f in all_used_dynamic_libraries:
-        r2_fd[f] = r2_start_analysis(f)
-    print("[+] Finish analysis  ")
-    
-    
+        if f not in dynamic_libraries.keys():
+            r2_fd[f] = r2_start_analysis(f)
+            dynamic_libraries[f] = get_dynamic_libraries(r2_fd[f], file_system_path)
+            # print(f + "=> ", end = '')
+            # print(get_dynamic_libraries(r2_fd[f], file_system_path))
+    # print(all_used_dynamic_libraries)
+    architecture = get_architecture(r2_fd[target_filepath])
+    print("[+] Collect and analyse success")
+
     print("[*] Identifying functions in elf and libraries ...")
     functions_other_defined[target_filepath] = get_function_names(r2_fd[target_filepath], 0)
     for f in all_used_dynamic_libraries:
         functions_other_defined[f] = get_function_names(r2_fd[f], 0)
-    #print(functions_other_defined)
+    # print(functions_other_defined)
     
     functions_self_defined[target_filepath] = get_function_names(r2_fd[target_filepath], 1)
     for lib in all_used_dynamic_libraries:
         functions_self_defined[lib] = get_function_names(r2_fd[lib], 1)
         for fun in functions_self_defined[lib]:
             function_to_library[fun] = lib
-    #print(functions_self_defined['./bin/pucfu'])
-    #print(functions_self_defined)
-    #print(function_to_library)
+    # print(functions_self_defined['./bin/pucfu'])
+    # print(functions_self_defined)
+    # print(function_to_library)
     print("[+] Identifying functions success")
     
     print("[*] Enumerateing call paths in libraries ...")
     for lib in all_used_dynamic_libraries:
         libraries_called_functions[lib] = get_functions_called(r2_fd[lib] ,lib, architecture)
-        #print(lib)
-        #print(get_functions_called(r2_fd[lib] ,lib, architecture))
-    #print(libraries_called_functions)
+        # print(lib)
+        # print(get_functions_called(r2_fd[lib] ,lib, architecture))
+    # print(libraries_called_functions)
     print("[+] Enumerateing call paths in libraries success")
 
+    # Search dangerous functions and add them to dangerous_functions
     print("[*] Searching for dangerous functions in libraries ...")
     dangerous_functions_now_len = len(dangerous_functions)
     dangerous_functions_old_len = 0
     while(dangerous_functions_now_len > dangerous_functions_old_len):
         for lib in libraries_called_functions.keys():
             for fun in libraries_called_functions[lib].keys():
                 if 'sym' in fun:
@@ -353,24 +391,23 @@
                         if add_filename_to_function(lib, called_fun) in dangerous_functions and func not in dangerous_functions:
                             dangerous_functions.append(func)
                             dangerous_functions_chain[func] = get_dangerous_chains(func, add_filename_to_function(lib, called_fun))
                             break
 
         dangerous_functions_old_len = dangerous_functions_now_len
         dangerous_functions_now_len = len(dangerous_functions)
-    #print(dangerous_functions)
-    #print(dangerous_functions_chain)
+    # print(dangerous_functions)
+    # print(dangerous_functions_chain)
     print("[*] Searching dangerous functions finish")
 
     print("[*] Searching dangerous called in binary ...")
     command_injection_addr = find_command_injection(r2_fd[target_filepath], target_filepath)
+    # print results
     for s in command_injection_addr:
         print(s)
     print("[+] fdcalls finish")
     
     if level:
         show_more_dangerous_function()
 
 if __name__ == '__main__':
     main()
-    
-
```

