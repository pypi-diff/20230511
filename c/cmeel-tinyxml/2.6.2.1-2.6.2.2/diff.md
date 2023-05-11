# Comparing `tmp/cmeel_tinyxml-2.6.2.1-4-py3-none-musllinux_1_1_x86_64.whl.zip` & `tmp/cmeel_tinyxml-2.6.2.2-0-py3-none-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 63060 bytes, number of entries: 11
--rw-r--r--  2.0 unx     8198 b- defN 23-May-03 13:46 cmeel.prefix/include/tinystr.h
--rw-r--r--  2.0 unx    64834 b- defN 23-May-03 13:46 cmeel.prefix/include/tinyxml.h
--rwxr-xr-x  2.0 unx   116496 b- defN 23-May-03 13:47 cmeel.prefix/lib/libtinyxml.so
--rw-r--r--  2.0 unx      977 b- defN 23-May-03 13:47 cmeel.prefix/lib/cmake/tinyxml/tinyxmlConfig.cmake
--rw-r--r--  2.0 unx     2762 b- defN 23-May-03 13:47 cmeel.prefix/lib/cmake/tinyxml/tinyxmlConfigVersion.cmake
--rw-r--r--  2.0 unx      839 b- defN 23-May-03 13:47 cmeel.prefix/lib/cmake/tinyxml/tinyxmlTargets-release.cmake
--rw-r--r--  2.0 unx     3947 b- defN 23-May-03 13:47 cmeel.prefix/lib/cmake/tinyxml/tinyxmlTargets.cmake
--rw-r--r--  2.0 unx      389 b- defN 23-May-03 13:47 cmeel_tinyxml-2.6.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx      111 b- defN 23-May-03 13:47 cmeel_tinyxml-2.6.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 13:47 cmeel_tinyxml-2.6.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1036 b- defN 23-May-03 13:47 cmeel_tinyxml-2.6.2.1.dist-info/RECORD
-11 files, 199589 bytes uncompressed, 61268 bytes compressed:  69.3%
+Zip file size: 55495 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     8198 b- defN 23-May-11 08:31 cmeel.prefix/include/tinystr.h
+-rw-r--r--  2.0 unx    64834 b- defN 23-May-11 08:31 cmeel.prefix/include/tinyxml.h
+-rwxr-xr-x  2.0 unx   129005 b- defN 23-May-11 08:33 cmeel.prefix/lib/libtinyxml.dylib
+-rw-r--r--  2.0 unx      977 b- defN 23-May-11 08:33 cmeel.prefix/lib/cmake/tinyxml/tinyxmlConfig.cmake
+-rw-r--r--  2.0 unx     2762 b- defN 23-May-11 08:33 cmeel.prefix/lib/cmake/tinyxml/tinyxmlConfigVersion.cmake
+-rw-r--r--  2.0 unx      855 b- defN 23-May-11 08:33 cmeel.prefix/lib/cmake/tinyxml/tinyxmlTargets-release.cmake
+-rw-r--r--  2.0 unx     3947 b- defN 23-May-11 08:33 cmeel.prefix/lib/cmake/tinyxml/tinyxmlTargets.cmake
+-rw-r--r--  2.0 unx      389 b- defN 23-May-11 08:33 cmeel_tinyxml-2.6.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-May-11 08:33 cmeel_tinyxml-2.6.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        0 b- defN 23-May-11 08:33 cmeel_tinyxml-2.6.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1039 b- defN 23-May-11 08:33 cmeel_tinyxml-2.6.2.2.dist-info/RECORD
+11 files, 212114 bytes uncompressed, 53697 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -1,34 +1,34 @@
 Filename: cmeel.prefix/include/tinystr.h
 Comment: 
 
 Filename: cmeel.prefix/include/tinyxml.h
 Comment: 
 
-Filename: cmeel.prefix/lib/libtinyxml.so
+Filename: cmeel.prefix/lib/libtinyxml.dylib
 Comment: 
 
 Filename: cmeel.prefix/lib/cmake/tinyxml/tinyxmlConfig.cmake
 Comment: 
 
 Filename: cmeel.prefix/lib/cmake/tinyxml/tinyxmlConfigVersion.cmake
 Comment: 
 
 Filename: cmeel.prefix/lib/cmake/tinyxml/tinyxmlTargets-release.cmake
 Comment: 
 
 Filename: cmeel.prefix/lib/cmake/tinyxml/tinyxmlTargets.cmake
 Comment: 
 
-Filename: cmeel_tinyxml-2.6.2.1.dist-info/METADATA
+Filename: cmeel_tinyxml-2.6.2.2.dist-info/METADATA
 Comment: 
 
-Filename: cmeel_tinyxml-2.6.2.1.dist-info/WHEEL
+Filename: cmeel_tinyxml-2.6.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: cmeel_tinyxml-2.6.2.1.dist-info/top_level.txt
+Filename: cmeel_tinyxml-2.6.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: cmeel_tinyxml-2.6.2.1.dist-info/RECORD
+Filename: cmeel_tinyxml-2.6.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cmeel.prefix/lib/cmake/tinyxml/tinyxmlTargets-release.cmake

```diff
@@ -4,16 +4,16 @@
 
 # Commands may need to know the format version.
 set(CMAKE_IMPORT_FILE_VERSION 1)
 
 # Import target "cmeel::tinyxml" for configuration "Release"
 set_property(TARGET cmeel::tinyxml APPEND PROPERTY IMPORTED_CONFIGURATIONS RELEASE)
 set_target_properties(cmeel::tinyxml PROPERTIES
-  IMPORTED_LOCATION_RELEASE "${_IMPORT_PREFIX}/lib/libtinyxml.so"
-  IMPORTED_SONAME_RELEASE "libtinyxml.so"
+  IMPORTED_LOCATION_RELEASE "${_IMPORT_PREFIX}/lib/libtinyxml.dylib"
+  IMPORTED_SONAME_RELEASE "@rpath/libtinyxml.dylib"
   )
 
 list(APPEND _cmake_import_check_targets cmeel::tinyxml )
-list(APPEND _cmake_import_check_files_for_cmeel::tinyxml "${_IMPORT_PREFIX}/lib/libtinyxml.so" )
+list(APPEND _cmake_import_check_files_for_cmeel::tinyxml "${_IMPORT_PREFIX}/lib/libtinyxml.dylib" )
 
 # Commands beyond this point should not need to know the version.
 set(CMAKE_IMPORT_FILE_VERSION)
```

## Comparing `cmeel_tinyxml-2.6.2.1.dist-info/RECORD` & `cmeel_tinyxml-2.6.2.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 cmeel.prefix/include/tinystr.h,sha256=cY4F0ArkDS6r1ojGS5gPpAQZrOfBLZaFxxCIjK8QLdU,8198
 cmeel.prefix/include/tinyxml.h,sha256=SS6_yWyihfpj9QIl2UiD-rcHdik8Ms08ZpUJaqbMdK4,64834
-cmeel.prefix/lib/libtinyxml.so,sha256=VHWqkb7VmKOvPmsG5HU2xOHKuHl8p9X12T1xpb-mX6Q,116496
+cmeel.prefix/lib/libtinyxml.dylib,sha256=ucvO7UySCVKY6fORcPuw8fXUmHUWQslwjU2rD5eBuSA,129005
 cmeel.prefix/lib/cmake/tinyxml/tinyxmlConfig.cmake,sha256=8UTTX8xp-a63aHKGu4llc0lZQrCxoET7MvFtSadPCQ8,977
 cmeel.prefix/lib/cmake/tinyxml/tinyxmlConfigVersion.cmake,sha256=RK8xbZkVKX-auS7N_aazNrNXYwboUhC_47cWw-b-v-c,2762
-cmeel.prefix/lib/cmake/tinyxml/tinyxmlTargets-release.cmake,sha256=2Gpsr58sAW7Uo6N1Id98ffaFl6wxlReC9TXXst3WPP8,839
+cmeel.prefix/lib/cmake/tinyxml/tinyxmlTargets-release.cmake,sha256=JUgwxZb6oSE-MgfGpuS5fai4sA0D7V6xs_G7tD2GFmc,855
 cmeel.prefix/lib/cmake/tinyxml/tinyxmlTargets.cmake,sha256=NaTseO70MssYbHmYraF1zior6DPM2vLJRL47LJ8tdLY,3947
-cmeel_tinyxml-2.6.2.1.dist-info/METADATA,sha256=Dwr9GfBsOJqpGrC2v15Qgh9q_5UbKG95fGFEuoRsG98,389
-cmeel_tinyxml-2.6.2.1.dist-info/WHEEL,sha256=pddIQTs2KsDTVS_JRcHntOedsyyPYi5Z2ruU71ZPEDg,111
-cmeel_tinyxml-2.6.2.1.dist-info/top_level.txt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cmeel_tinyxml-2.6.2.1.dist-info/RECORD,,
+cmeel_tinyxml-2.6.2.2.dist-info/METADATA,sha256=kf-2BKrumsoRCZJG6IP3t7zPmJ07A0767ejgHYUxR1A,389
+cmeel_tinyxml-2.6.2.2.dist-info/WHEEL,sha256=fQEGWmDGMVdwxh3c-Q1An6NDSnLDemHsQiF6sYhq5pM,108
+cmeel_tinyxml-2.6.2.2.dist-info/top_level.txt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+cmeel_tinyxml-2.6.2.2.dist-info/RECORD,,
```

