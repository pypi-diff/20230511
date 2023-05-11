# Comparing `tmp/OpenGeode_Inspector-3.0.3-cp39-cp39-win_amd64.whl.zip` & `tmp/OpenGeode_Inspector-3.0.4-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 262745 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      175 b- defN 23-May-03 09:50 opengeode_inspector/__init__.py
--rw-rw-rw-  2.0 fat      271 b- defN 23-May-03 09:50 opengeode_inspector/inspector.py
--rw-rw-rw-  2.0 fat   436736 b- defN 23-May-03 09:52 opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll
--rw-rw-rw-  2.0 fat   451072 b- defN 23-May-03 09:52 opengeode_inspector/bin/opengeode_inspector_py_inspector.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     5481 b- defN 23-May-03 09:52 OpenGeode_Inspector-3.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-03 09:52 OpenGeode_Inspector-3.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-May-03 09:52 OpenGeode_Inspector-3.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      772 b- defN 23-May-03 09:52 OpenGeode_Inspector-3.0.3.dist-info/RECORD
-8 files, 894627 bytes uncompressed, 261373 bytes compressed:  70.8%
+Zip file size: 262749 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      175 b- defN 23-May-11 08:13 opengeode_inspector/__init__.py
+-rw-rw-rw-  2.0 fat      271 b- defN 23-May-11 08:13 opengeode_inspector/inspector.py
+-rw-rw-rw-  2.0 fat   436736 b- defN 23-May-11 08:14 opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll
+-rw-rw-rw-  2.0 fat   451072 b- defN 23-May-11 08:14 opengeode_inspector/bin/opengeode_inspector_py_inspector.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     5481 b- defN 23-May-11 08:14 OpenGeode_Inspector-3.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-11 08:14 OpenGeode_Inspector-3.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-May-11 08:14 OpenGeode_Inspector-3.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      772 b- defN 23-May-11 08:14 OpenGeode_Inspector-3.0.4.dist-info/RECORD
+8 files, 894627 bytes uncompressed, 261377 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll
 Comment: 
 
 Filename: opengeode_inspector/bin/opengeode_inspector_py_inspector.cp39-win_amd64.pyd
 Comment: 
 
-Filename: OpenGeode_Inspector-3.0.3.dist-info/METADATA
+Filename: OpenGeode_Inspector-3.0.4.dist-info/METADATA
 Comment: 
 
-Filename: OpenGeode_Inspector-3.0.3.dist-info/WHEEL
+Filename: OpenGeode_Inspector-3.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: OpenGeode_Inspector-3.0.3.dist-info/top_level.txt
+Filename: OpenGeode_Inspector-3.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: OpenGeode_Inspector-3.0.3.dist-info/RECORD
+Filename: OpenGeode_Inspector-3.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180049210
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May  3 09:51:31 2023
+Time/Date		Thu May 11 08:13:46 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		000000000004b800
 SizeOfInitializedData	000000000001ee00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000049210
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		0006f000
 SizeOfHeaders		00000400
-CheckSum		00079e1d
+CheckSum		00077085
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -238,16 +238,16 @@
 
  000636e0	000639c8 00000000 00000000 000675c0 0004d1b8
 
 	DLL Name: OpenGeode_geometry.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	66cc4	  301  ??1?$NNSearch@$01@geode@@QEAA@XZ
 	6755c	   42  ??$point_triangle_position@$02@geode@@YA?AW4Position@0@AEBV?$Point@$02@0@AEBV?$Triangle@$02@0@@Z
-	674b2	  643  ?vertices@?$GenericSegment@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$02@geode@@QEBAAEBV?$array@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$01@std@@XZ
-	67408	  642  ?vertices@?$GenericSegment@V?$reference_wrapper@$$CBV?$Point@$01@geode@@@std@@$01@geode@@QEBAAEBV?$array@V?$reference_wrapper@$$CBV?$Point@$01@geode@@@std@@$01@std@@XZ
+	674b2	  646  ?vertices@?$GenericSegment@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$02@geode@@QEBAAEBV?$array@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$01@std@@XZ
+	67408	  645  ?vertices@?$GenericSegment@V?$reference_wrapper@$$CBV?$Point@$01@geode@@@std@@$01@geode@@QEBAAEBV?$array@V?$reference_wrapper@$$CBV?$Point@$01@geode@@@std@@$01@std@@XZ
 	673d0	  512  ?intersects@?$BoundingBox@$01@geode@@QEBA_NAEBV12@@Z
 	67398	  515  ?intersects@?$BoundingBox@$02@geode@@QEBA_NAEBV12@@Z
 	67362	  532  ?mapping_morton@Impl@?$AABBTree@$01@geode@@QEBAII@Z
 	6731e	  550  ?node@Impl@?$AABBTree@$01@geode@@QEBAAEBV?$BoundingBox@$01@3@I@Z
 	672d0	  504  ?get_recursive_iterators@Impl@?$AABBTree@$01@geode@@SA?AUIterator@123@III@Z
 	672a0	  518  ?is_leaf@Impl@?$AABBTree@$01@geode@@SA_NII@Z
 	6726a	  533  ?mapping_morton@Impl@?$AABBTree@$02@geode@@QEBAII@Z
@@ -255,19 +255,19 @@
 	671d8	  505  ?get_recursive_iterators@Impl@?$AABBTree@$02@geode@@SA?AUIterator@123@III@Z
 	671a8	  519  ?is_leaf@Impl@?$AABBTree@$02@geode@@SA_NII@Z
 	6717c	  542  ?nb_bboxes@?$AABBTree@$01@geode@@QEBAIXZ
 	67158	  296  ??1?$AABBTree@$01@geode@@QEAA@XZ
 	6712c	  543  ?nb_bboxes@?$AABBTree@$02@geode@@QEBAIXZ
 	67108	  297  ??1?$AABBTree@$02@geode@@QEAA@XZ
 	670d2	  248  ??0?$Segment@$02@geode@@QEAA@AEBV?$Point@$02@1@0@Z
-	67026	  649  ?vertices@?$GenericTriangle@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$02@geode@@QEBAAEBV?$array@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$02@std@@XZ
+	67026	  652  ?vertices@?$GenericTriangle@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$02@geode@@QEBAAEBV?$array@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$02@std@@XZ
 	66fc2	   41  ??$point_triangle_position@$01@geode@@YA?AW4Position@0@AEBV?$Point@$01@0@AEBV?$Triangle@$01@0@@Z
 	66f8c	  244  ??0?$Segment@$01@geode@@QEAA@AEBV?$Point@$01@1@0@Z
-	66f04	  614  ?segment_triangle_intersection_detection@geode@@YA?AU?$pair@W4Position@geode@@W412@@std@@AEBV?$Segment@$02@1@AEBV?$Triangle@$02@1@@Z
-	66e92	  611  ?segment_segment_intersection_detection@geode@@YA?AU?$pair@W4Position@geode@@W412@@std@@AEBV?$Segment@$01@1@0@Z
+	66f04	  616  ?segment_triangle_intersection_detection@geode@@YA?AU?$pair@W4Position@geode@@W412@@std@@AEBV?$Segment@$02@1@AEBV?$Triangle@$02@1@@Z
+	66e92	  613  ?segment_segment_intersection_detection@geode@@YA?AU?$pair@W4Position@geode@@W412@@std@@AEBV?$Segment@$01@1@0@Z
 	66e54	   26  ??$point_point_distance@$02@geode@@YANAEBV?$Point@$02@0@0@Z
 	66e16	   25  ??$point_point_distance@$01@geode@@YANAEBV?$Point@$01@0@0@Z
 	66dc8	  479  ?colocated_index_mapping@?$NNSearch@$02@geode@@QEBA?AUColocatedInfo@12@N@Z
 	66da4	  302  ??1?$NNSearch@$02@geode@@QEAA@XZ
 	66d36	  176  ??0?$NNSearch@$02@geode@@QEAA@V?$vector@V?$Point@$02@geode@@V?$allocator@V?$Point@$02@geode@@@std@@@std@@@Z
 	66ce8	  478  ?colocated_index_mapping@?$NNSearch@$01@geode@@QEBA?AUColocatedInfo@12@N@Z
 	66c56	  174  ??0?$NNSearch@$01@geode@@QEAA@V?$vector@V?$Point@$01@geode@@V?$allocator@V?$Point@$01@geode@@@std@@@std@@@Z
@@ -13208,23 +13208,23 @@
 	  11580: 00 00 19 00 3f 3f 24 70 6f 69 6e 74 5f 70 6f 69
 	  11590: 6e 74 5f 64 69 73 74 61 6e 63 65 40 24 30 31 40
 	  115a0: 67 65 6f 64 65 40 40 59 41 4e 41 45 42 56 3f 24
 	  115b0: 50 6f 69 6e 74 40 24 30 31 40 30 40 30 40 5a 00
 	  115c0: 1a 00 3f 3f 24 70 6f 69 6e 74 5f 70 6f 69 6e 74
 	  115d0: 5f 64 69 73 74 61 6e 63 65 40 24 30 32 40 67 65
 	  115e0: 6f 64 65 40 40 59 41 4e 41 45 42 56 3f 24 50 6f
-	  115f0: 69 6e 74 40 24 30 32 40 30 40 30 40 5a 00 63 02
+	  115f0: 69 6e 74 40 24 30 32 40 30 40 30 40 5a 00 65 02
 	  11600: 3f 73 65 67 6d 65 6e 74 5f 73 65 67 6d 65 6e 74
 	  11610: 5f 69 6e 74 65 72 73 65 63 74 69 6f 6e 5f 64 65
 	  11620: 74 65 63 74 69 6f 6e 40 67 65 6f 64 65 40 40 59
 	  11630: 41 3f 41 55 3f 24 70 61 69 72 40 57 34 50 6f 73
 	  11640: 69 74 69 6f 6e 40 67 65 6f 64 65 40 40 57 34 31
 	  11650: 32 40 40 73 74 64 40 40 41 45 42 56 3f 24 53 65
 	  11660: 67 6d 65 6e 74 40 24 30 31 40 31 40 30 40 5a 00
-	  11670: 66 02 3f 73 65 67 6d 65 6e 74 5f 74 72 69 61 6e
+	  11670: 68 02 3f 73 65 67 6d 65 6e 74 5f 74 72 69 61 6e
 	  11680: 67 6c 65 5f 69 6e 74 65 72 73 65 63 74 69 6f 6e
 	  11690: 5f 64 65 74 65 63 74 69 6f 6e 40 67 65 6f 64 65
 	  116a0: 40 40 59 41 3f 41 55 3f 24 70 61 69 72 40 57 34
 	  116b0: 50 6f 73 69 74 69 6f 6e 40 67 65 6f 64 65 40 40
 	  116c0: 57 34 31 32 40 40 73 74 64 40 40 41 45 42 56 3f
 	  116d0: 24 53 65 67 6d 65 6e 74 40 24 30 32 40 31 40 41
 	  116e0: 45 42 56 3f 24 54 72 69 61 6e 67 6c 65 40 24 30
@@ -13234,15 +13234,15 @@
 	  11720: 6e 74 40 24 30 31 40 31 40 30 40 5a 00 00 29 00
 	  11730: 3f 3f 24 70 6f 69 6e 74 5f 74 72 69 61 6e 67 6c
 	  11740: 65 5f 70 6f 73 69 74 69 6f 6e 40 24 30 31 40 67
 	  11750: 65 6f 64 65 40 40 59 41 3f 41 57 34 50 6f 73 69
 	  11760: 74 69 6f 6e 40 30 40 41 45 42 56 3f 24 50 6f 69
 	  11770: 6e 74 40 24 30 31 40 30 40 41 45 42 56 3f 24 54
 	  11780: 72 69 61 6e 67 6c 65 40 24 30 31 40 30 40 40 5a
-	  11790: 00 00 89 02 3f 76 65 72 74 69 63 65 73 40 3f 24
+	  11790: 00 00 8c 02 3f 76 65 72 74 69 63 65 73 40 3f 24
 	  117a0: 47 65 6e 65 72 69 63 54 72 69 61 6e 67 6c 65 40
 	  117b0: 56 3f 24 72 65 66 65 72 65 6e 63 65 5f 77 72 61
 	  117c0: 70 70 65 72 40 24 24 43 42 56 3f 24 50 6f 69 6e
 	  117d0: 74 40 24 30 32 40 67 65 6f 64 65 40 40 40 73 74
 	  117e0: 64 40 40 24 30 32 40 67 65 6f 64 65 40 40 51 45
 	  117f0: 42 41 41 45 42 56 3f 24 61 72 72 61 79 40 56 3f
 	  11800: 24 72 65 66 65 72 65 6e 63 65 5f 77 72 61 70 70
@@ -13296,25 +13296,25 @@
 	  11b00: 49 40 5a 00 03 02 3f 69 6e 74 65 72 73 65 63 74
 	  11b10: 73 40 3f 24 42 6f 75 6e 64 69 6e 67 42 6f 78 40
 	  11b20: 24 30 32 40 67 65 6f 64 65 40 40 51 45 42 41 5f
 	  11b30: 4e 41 45 42 56 31 32 40 40 5a 00 00 00 02 3f 69
 	  11b40: 6e 74 65 72 73 65 63 74 73 40 3f 24 42 6f 75 6e
 	  11b50: 64 69 6e 67 42 6f 78 40 24 30 31 40 67 65 6f 64
 	  11b60: 65 40 40 51 45 42 41 5f 4e 41 45 42 56 31 32 40
-	  11b70: 40 5a 00 00 82 02 3f 76 65 72 74 69 63 65 73 40
+	  11b70: 40 5a 00 00 85 02 3f 76 65 72 74 69 63 65 73 40
 	  11b80: 3f 24 47 65 6e 65 72 69 63 53 65 67 6d 65 6e 74
 	  11b90: 40 56 3f 24 72 65 66 65 72 65 6e 63 65 5f 77 72
 	  11ba0: 61 70 70 65 72 40 24 24 43 42 56 3f 24 50 6f 69
 	  11bb0: 6e 74 40 24 30 31 40 67 65 6f 64 65 40 40 40 73
 	  11bc0: 74 64 40 40 24 30 31 40 67 65 6f 64 65 40 40 51
 	  11bd0: 45 42 41 41 45 42 56 3f 24 61 72 72 61 79 40 56
 	  11be0: 3f 24 72 65 66 65 72 65 6e 63 65 5f 77 72 61 70
 	  11bf0: 70 65 72 40 24 24 43 42 56 3f 24 50 6f 69 6e 74
 	  11c00: 40 24 30 31 40 67 65 6f 64 65 40 40 40 73 74 64
-	  11c10: 40 40 24 30 31 40 73 74 64 40 40 58 5a 00 83 02
+	  11c10: 40 40 24 30 31 40 73 74 64 40 40 58 5a 00 86 02
 	  11c20: 3f 76 65 72 74 69 63 65 73 40 3f 24 47 65 6e 65
 	  11c30: 72 69 63 53 65 67 6d 65 6e 74 40 56 3f 24 72 65
 	  11c40: 66 65 72 65 6e 63 65 5f 77 72 61 70 70 65 72 40
 	  11c50: 24 24 43 42 56 3f 24 50 6f 69 6e 74 40 24 30 32
 	  11c60: 40 67 65 6f 64 65 40 40 40 73 74 64 40 40 24 30
 	  11c70: 32 40 67 65 6f 64 65 40 40 51 45 42 41 41 45 42
 	  11c80: 56 3f 24 61 72 72 61 79 40 56 3f 24 72 65 66 65
@@ -49620,19 +49620,19 @@
    180021898:	mov    %rdi,0x20(%rsp)
    18002189d:	mov    %rbx,%r8
    1800218a0:	lea    0x48(%rsp),%rdx
    1800218a5:	lea    0x60(%rsp),%rcx
    1800218aa:	call   0x180021090
    1800218af:	test   %al,%al
    1800218b1:	jne    0x1800218d1
-   1800218b3:	mov    %rbp,%r9
+   1800218b3:	mov    %rbx,%r9
    1800218b6:	mov    %rdi,0x20(%rsp)
-   1800218bb:	mov    %rbx,%r8
-   1800218be:	lea    0x48(%rsp),%rdx
-   1800218c3:	lea    0x60(%rsp),%rcx
+   1800218bb:	mov    %rbp,%r8
+   1800218be:	lea    0x60(%rsp),%rdx
+   1800218c3:	lea    0x48(%rsp),%rcx
    1800218c8:	call   0x180021090
    1800218cd:	test   %al,%al
    1800218cf:	je     0x180021881
    1800218d1:	mov    $0x1,%al
    1800218d3:	mov    0x78(%rsp),%rcx
    1800218d8:	xor    %rsp,%rcx
    1800218db:	call   0x180048ed0
@@ -100922,17 +100922,17 @@
    18004f01a:	(bad)
    18004f01b:	addb   $0x0,(%rcx)
    18004f01e:	add    %al,(%rax)
    18004f020:	rclb   0x18006(%rsi)
    18004f026:	add    %al,(%rax)
    18004f028:	add    %al,(%rax)
    18004f02a:	add    %al,(%rax)
-   18004f02c:	movabs %eax,0xd0000000064522e
-   18004f035:	add    %al,(%rax)
-   18004f037:	add    %ch,%ah
+   18004f02c:	mov    $0x645ca3,%edx
+   18004f031:	add    %al,(%rax)
+   18004f033:	add    %cl,-0x14000000(%rip)        # 0x16c04f039
    18004f039:	add    (%rax),%al
    18004f03b:	add    %bl,-0x16e3fffc(,%rdi,8)
    18004f042:	add    $0x0,%al
 	...
    18004f050:	cmp    %al,(%rcx)
 	...
    18004f0a6:	add    %al,(%rax)
@@ -143090,15 +143090,15 @@
    180066e7e:	rex.X push %rsi
    180066e80:	(bad)
    180066e81:	and    $0x50,%al
    180066e83:	outsl  %ds:(%rsi),(%dx)
    180066e84:	imul   $0x32302440,0x74(%rsi),%ebp
    180066e8b:	rex xor %al,0x30(%rax)
    180066e8f:	rex pop %rdx
-   180066e91:	add    %ah,0x2(%rbx)
+   180066e91:	add    %ah,0x2(%rbp)
    180066e94:	(bad)
    180066e95:	jae    0x180066efc
    180066e97:	insl   (%dx),%es:(%edi)
    180066e99:	outsb  %gs:(%rsi),(%dx)
    180066e9b:	je     0x180066efc
    180066e9d:	jae    0x180066f04
    180066e9f:	insl   (%dx),%es:(%edi)
@@ -143141,15 +143141,15 @@
    180066ef1:	and    $0x53,%al
    180066ef3:	gs insl (%dx),%es:(%edi)
    180066ef6:	outsb  %gs:(%rsi),(%dx)
    180066ef8:	je     0x180066f3a
    180066efa:	and    $0x30,%al
    180066efc:	xor    %eax,0x31(%rax)
    180066eff:	rex xor %al,0x5a(%rax)
-   180066f03:	add    %ah,0x2(%rsi)
+   180066f03:	add    %ch,0x2(%rax)
    180066f06:	(bad)
    180066f07:	jae    0x180066f6e
    180066f09:	insl   (%dx),%es:(%edi)
    180066f0b:	outsb  %gs:(%rsi),(%dx)
    180066f0d:	je     0x180066f6e
    180066f0f:	je     0x180066f83
    180066f11:	imul   $0x5f656c67,0x6e(%rcx),%esp
@@ -143280,15 +143280,15 @@
    180067017:	outsb  %ds:(%rsi),(%dx)
    180067018:	insb   (%dx),%es:(%edi)
    18006701a:	gs rex and $0x30,%al
    18006701e:	xor    %eax,0x30(%rax)
    180067021:	rex
    180067022:	rex pop %rdx
    180067024:	add    %al,(%rax)
-   180067026:	mov    %eax,(%rdx)
+   180067026:	mov    %es,(%rdx)
    180067028:	(bad)
    180067029:	jbe    0x180067090
    18006702b:	jb     0x1800670a1
    18006702d:	imul   $0x243f4073,0x65(%rbx),%esp
    180067034:	rex.RXB
    180067035:	outsb  %gs:(%rsi),(%dx)
    180067037:	gs jb  0x1800670a3
@@ -143763,16 +143763,16 @@
    1800673fd:	rex.B
    1800673fe:	rex.RB
    1800673ff:	rex.X push %rsi
    180067401:	xor    %esi,(%rdx)
    180067403:	rex
    180067404:	rex pop %rdx
    180067406:	add    %al,(%rax)
-   180067408:	(bad)
-   180067409:	add    (%rdi),%bh
+   180067408:	test   %eax,(%rdx)
+   18006740a:	(bad)
    18006740b:	jbe    0x180067472
    18006740d:	jb     0x180067483
    18006740f:	imul   $0x243f4073,0x65(%rbx),%esp
    180067416:	rex.RXB
    180067417:	outsb  %gs:(%rsi),(%dx)
    180067419:	gs jb  0x180067485
    18006741c:	movsxd 0x65(%rbx),%edx
@@ -143843,15 +143843,15 @@
    1800674a3:	fs rex
    1800674a5:	rex and $0x30,%al
    1800674a8:	xor    %eax,0x73(%rax)
    1800674ab:	je     0x180067511
    1800674ad:	rex
    1800674ae:	rex pop %rax
    1800674b0:	pop    %rdx
-   1800674b1:	add    %al,0x65763f02(%rbx)
+   1800674b1:	add    %al,0x65763f02(%rsi)
    1800674b7:	jb     0x18006752d
    1800674b9:	imul   $0x243f4073,0x65(%rbx),%esp
    1800674c0:	rex.RXB
    1800674c1:	outsb  %gs:(%rsi),(%dx)
    1800674c3:	gs jb  0x18006752f
    1800674c6:	movsxd 0x65(%rbx),%edx
    1800674c9:	insl   (%dx),%es:(%edi)
```

## Comparing `OpenGeode_Inspector-3.0.3.dist-info/METADATA` & `OpenGeode_Inspector-3.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: OpenGeode-Inspector
-Version: 3.0.3
+Version: 3.0.4
 Summary: Open source framework for inspecting the validity of geometric models
 Home-page: https://github.com/Geode-solutions/OpenGeode-Inspector
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: opengeode-core (==14.*,>=14.0.13)
+Requires-Dist: opengeode-core (==14.*,>=14.0.16)
 Requires-Dist: opengeode-geosciences (==7.*,>=7.0.6)
-Requires-Dist: opengeode-geosciencesio (==4.*,>=4.1.1)
+Requires-Dist: opengeode-geosciencesio (==4.*,>=4.1.2)
 Requires-Dist: opengeode-io (==6.*,>=6.0.4)
 
 <h1 align="center">OpenGeode-Inspector<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">OpenGeode module for inspecting meshes and models</h3>
 
 
 <p align="center">
```

### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: OpenGeode-Inspector Version: 3.0.3 Summary: Open
+Metadata-Version: 2.1 Name: OpenGeode-Inspector Version: 3.0.4 Summary: Open
 source framework for inspecting the validity of geometric models Home-page:
 https://github.com/Geode-solutions/OpenGeode-Inspector Author: Geode-solutions
 Author-email: contact@geode-solutions.com License: MIT Platform: UNKNOWN
 Description-Content-Type: text/markdown Requires-Dist: opengeode-core
-(==14.*,>=14.0.13) Requires-Dist: opengeode-geosciences (==7.*,>=7.0.6)
-Requires-Dist: opengeode-geosciencesio (==4.*,>=4.1.1) Requires-Dist:
+(==14.*,>=14.0.16) Requires-Dist: opengeode-geosciences (==7.*,>=7.0.6)
+Requires-Dist: opengeode-geosciencesio (==4.*,>=4.1.2) Requires-Dist:
 opengeode-io (==6.*,>=6.0.4)
               ****** OpenGeode-Inspectorby Geode-solutions ******
           **** OpenGeode module for inspecting meshes and models ****
           [Build Status] [Deploy Status] [Coverage Status] [Version]
              [Windows support] [Ubuntu support] [Red Hat support]
       [Language] [License] [Semantic-release] [Slack_invite] [DOI] --- ##
  Introduction OpenGeode-Inspector is a module of [OpenGeode] providing ways of
```

## Comparing `OpenGeode_Inspector-3.0.3.dist-info/RECORD` & `OpenGeode_Inspector-3.0.4.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 opengeode_inspector/__init__.py,sha256=PxQ3SsdhF6R2_6Gj0-wVDgy1a-veIjTQApBSB7X5b2U,175
 opengeode_inspector/inspector.py,sha256=gouwVrJtM8c0PoZuR6t9cbtvdpJhrgk_Lvm9PTj-Tws,271
-opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll,sha256=ozd6Kmm6wh50sgERRcSFVqXXYRjlUD6Yi5RKN2Jra2E,436736
-opengeode_inspector/bin/opengeode_inspector_py_inspector.cp39-win_amd64.pyd,sha256=PD_APmJqd2ubKAaJNJ_RcIPHZaSst00owDznLg6aZIY,451072
-OpenGeode_Inspector-3.0.3.dist-info/METADATA,sha256=vF-dQMLKnj4PQW0SL8oEKQ6Jip1cZQVTCzBkP_XudqY,5481
-OpenGeode_Inspector-3.0.3.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-OpenGeode_Inspector-3.0.3.dist-info/top_level.txt,sha256=HB6mBr33nBKSATXRcJ4Yof7xiFcQAnhw3pFzWTv8zso,20
-OpenGeode_Inspector-3.0.3.dist-info/RECORD,,
+opengeode_inspector/bin/OpenGeode-Inspector_inspector.dll,sha256=mwBa-sk7Z01L4Fvji0Gczarh6R6I5sLxDjS-f65rDk8,436736
+opengeode_inspector/bin/opengeode_inspector_py_inspector.cp39-win_amd64.pyd,sha256=lo-lUJTvUk8QIhNn7VC7fltFKusOFk3Wz9540D1lDoE,451072
+OpenGeode_Inspector-3.0.4.dist-info/METADATA,sha256=qpmSKDHa0gbtjXZwvM8VTu323RB1Sk71E6g3USC7SgM,5481
+OpenGeode_Inspector-3.0.4.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+OpenGeode_Inspector-3.0.4.dist-info/top_level.txt,sha256=HB6mBr33nBKSATXRcJ4Yof7xiFcQAnhw3pFzWTv8zso,20
+OpenGeode_Inspector-3.0.4.dist-info/RECORD,,
```

