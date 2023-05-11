# Comparing `tmp/loristrck-1.5.6.tar.gz` & `tmp/loristrck-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loristrck-1.5.6.tar", last modified: Tue May  9 15:00:09 2023, max compression
+gzip compressed data, was "loristrck-1.5.7.tar", last modified: Thu May 11 20:28:10 2023, max compression
```

## Comparing `loristrck-1.5.6.tar` & `loristrck-1.5.7.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-09 15:00:09.553993 loristrck-1.5.6/
--rwxrwxr-x   0 em        (1000) em        (1000)     1681 2021-11-25 01:27:49.000000 loristrck-1.5.6/LICENSE
--rw-rw-r--   0 em        (1000) em        (1000)      296 2021-11-25 01:27:49.000000 loristrck-1.5.6/MANIFEST.in
--rw-rw-r--   0 em        (1000) em        (1000)     2231 2023-05-09 15:00:09.554993 loristrck-1.5.6/PKG-INFO
--rwxrwxr-x   0 em        (1000) em        (1000)     1822 2023-04-26 15:20:52.000000 loristrck-1.5.6/README.rst
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-09 15:00:09.448994 loristrck-1.5.6/bin/
--rwxrwxr-x   0 em        (1000) em        (1000)     3225 2023-01-21 19:17:25.000000 loristrck-1.5.6/bin/loristrck_analyze
--rwxrwxr-x   0 em        (1000) em        (1000)     3798 2023-04-19 22:30:16.000000 loristrck-1.5.6/bin/loristrck_chord
--rwxrwxr-x   0 em        (1000) em        (1000)     4213 2021-11-25 01:27:49.000000 loristrck-1.5.6/bin/loristrck_pack
--rwxrwxr-x   0 em        (1000) em        (1000)     3203 2021-11-25 01:34:31.000000 loristrck-1.5.6/bin/loristrck_synth
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-09 15:00:09.453994 loristrck-1.5.6/loristrck/
--rwxrwxr-x   0 em        (1000) em        (1000)      344 2021-11-25 01:27:49.000000 loristrck-1.5.6/loristrck/__init__.py
--rw-rw-r--   0 em        (1000) em        (1000)  1267772 2023-01-21 17:51:56.000000 loristrck-1.5.6/loristrck/_core.cpp
--rw-rw-r--   0 em        (1000) em        (1000)     2010 2023-05-09 14:59:22.000000 loristrck-1.5.6/loristrck/_core.pyi
--rwxrwxr-x   0 em        (1000) em        (1000)    26341 2021-11-25 01:27:49.000000 loristrck-1.5.6/loristrck/_core.pyx
--rw-rw-r--   0 em        (1000) em        (1000)       74 2021-11-25 01:27:49.000000 loristrck-1.5.6/loristrck/common.py
--rwxrwxr-x   0 em        (1000) em        (1000)     6041 2021-11-25 01:27:49.000000 loristrck-1.5.6/loristrck/lorisdefs.pxd
--rw-rw-r--   0 em        (1000) em        (1000)     4288 2021-11-25 01:27:49.000000 loristrck-1.5.6/loristrck/play.py
--rwxrwxr-x   0 em        (1000) em        (1000)     1960 2021-11-25 01:27:49.000000 loristrck-1.5.6/loristrck/plot.py
--rw-rw-r--   0 em        (1000) em        (1000)        0 2023-05-06 10:27:47.000000 loristrck-1.5.6/loristrck/py.typed
--rwxrwxr-x   0 em        (1000) em        (1000)    55251 2023-05-09 10:31:56.000000 loristrck-1.5.6/loristrck/util.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-09 15:00:09.455994 loristrck-1.5.6/loristrck.egg-info/
--rw-rw-r--   0 em        (1000) em        (1000)     2231 2023-05-09 15:00:09.000000 loristrck-1.5.6/loristrck.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)     4117 2023-05-09 15:00:09.000000 loristrck-1.5.6/loristrck.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2023-05-09 15:00:09.000000 loristrck-1.5.6/loristrck.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)       43 2023-05-09 15:00:09.000000 loristrck-1.5.6/loristrck.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)       10 2023-05-09 15:00:09.000000 loristrck-1.5.6/loristrck.egg-info/top_level.txt
--rw-r--r--   0 em        (1000) em        (1000)      117 2023-02-26 12:26:54.000000 loristrck-1.5.6/pyproject.toml
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-09 15:00:09.455994 loristrck-1.5.6/scripts/
--rwxrwxr-x   0 em        (1000) em        (1000)     4010 2021-11-25 01:27:49.000000 loristrck-1.5.6/scripts/prepare_windows_build.py
--rw-rw-r--   0 em        (1000) em        (1000)      964 2021-11-25 01:27:49.000000 loristrck-1.5.6/scripts/windows-build-wheely.py
--rwxrwxr-x   0 em        (1000) em        (1000)       67 2023-05-09 15:00:09.556993 loristrck-1.5.6/setup.cfg
--rwxrwxr-x   0 em        (1000) em        (1000)     5227 2023-05-09 14:59:36.000000 loristrck-1.5.6/setup.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-09 15:00:09.445994 loristrck-1.5.6/src/
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-09 15:00:09.465994 loristrck-1.5.6/src/loris/
--rwxrwxr-x   0 em        (1000) em        (1000)      177 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/AUTHORS
--rwxrwxr-x   0 em        (1000) em        (1000)    17982 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/COPYING
--rwxrwxr-x   0 em        (1000) em        (1000)     7831 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/INSTALL
--rwxrwxr-x   0 em        (1000) em        (1000)     1455 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/Makefile.am
--rwxrwxr-x   0 em        (1000) em        (1000)    24527 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/Makefile.in
--rwxrwxr-x   0 em        (1000) em        (1000)    32377 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/NEWS
--rwxrwxr-x   0 em        (1000) em        (1000)     2914 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/README
--rwxrwxr-x   0 em        (1000) em        (1000)      793 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/THANKS
--rwxrwxr-x   0 em        (1000) em        (1000)   280777 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/aclocal.m4
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-09 15:00:09.471994 loristrck-1.5.6/src/loris/config/
--rwxrwxr-x   0 em        (1000) em        (1000)     3707 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/config/compile
--rwxrwxr-x   0 em        (1000) em        (1000)    44941 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/config/config.guess
--rwxrwxr-x   0 em        (1000) em        (1000)    34423 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/config/config.sub
--rwxrwxr-x   0 em        (1000) em        (1000)    18615 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/config/depcomp
--rwxrwxr-x   0 em        (1000) em        (1000)    13663 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/config/install-sh
--rwxrwxr-x   0 em        (1000) em        (1000)   199705 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/config/ltmain.sh
--rwxrwxr-x   0 em        (1000) em        (1000)    11419 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/config/missing
--rwxrwxr-x   0 em        (1000) em        (1000)     4189 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/config/py-compile
--rwxrwxr-x   0 em        (1000) em        (1000)     3379 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/config.h.in
--rwxrwxr-x   0 em        (1000) em        (1000)   850178 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/configure
--rwxrwxr-x   0 em        (1000) em        (1000)    14378 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/configure.ac
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-09 15:00:09.478994 loristrck-1.5.6/src/loris/csound/
--rwxrwxr-x   0 em        (1000) em        (1000)     1124 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/csound/Makefile.am
--rwxrwxr-x   0 em        (1000) em        (1000)    19007 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/csound/Makefile.in
--rwxrwxr-x   0 em        (1000) em        (1000)     4338 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/csound/README
--rwxrwxr-x   0 em        (1000) em        (1000)    36541 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/csound/lorisgens4.C
--rwxrwxr-x   0 em        (1000) em        (1000)     2842 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/csound/lorisgens4.h
--rwxrwxr-x   0 em        (1000) em        (1000)    37239 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/csound/lorisgens5.C
--rwxrwxr-x   0 em        (1000) em        (1000)     2839 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/csound/lorisgens5.h
--rwxrwxr-x   0 em        (1000) em        (1000)     2567 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/csound/tryit.csd
--rwxrwxr-x   0 em        (1000) em        (1000)     3409 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/csound/trymorph.csd
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-09 15:00:09.548993 loristrck-1.5.6/src/loris/src/
--rwxrwxr-x   0 em        (1000) em        (1000)    29321 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/AiffData.C
--rwxrwxr-x   0 em        (1000) em        (1000)    11816 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/AiffData.h
--rwxrwxr-x   0 em        (1000) em        (1000)    18754 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/AiffFile.C
--rwxrwxr-x   0 em        (1000) em        (1000)    15921 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/AiffFile.h
--rwxrwxr-x   0 em        (1000) em        (1000)    50936 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Analyzer.C
--rwxrwxr-x   0 em        (1000) em        (1000)    27787 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Analyzer.h
--rwxrwxr-x   0 em        (1000) em        (1000)    10512 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/AssociateBandwidth.C
--rwxrwxr-x   0 em        (1000) em        (1000)     3701 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/AssociateBandwidth.h
--rwxrwxr-x   0 em        (1000) em        (1000)     3887 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/BigEndian.C
--rwxrwxr-x   0 em        (1000) em        (1000)     1687 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/BigEndian.h
--rwxrwxr-x   0 em        (1000) em        (1000)     3643 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Breakpoint.C
--rwxrwxr-x   0 em        (1000) em        (1000)     4414 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Breakpoint.h
--rwxrwxr-x   0 em        (1000) em        (1000)     1501 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/BreakpointEnvelope.h
--rwxrwxr-x   0 em        (1000) em        (1000)     2685 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/BreakpointUtils.C
--rwxrwxr-x   0 em        (1000) em        (1000)     7352 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/BreakpointUtils.h
--rwxrwxr-x   0 em        (1000) em        (1000)    23042 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Channelizer.C
--rwxrwxr-x   0 em        (1000) em        (1000)    24426 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Channelizer.h
--rwxrwxr-x   0 em        (1000) em        (1000)     6399 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Collator.C
--rwxrwxr-x   0 em        (1000) em        (1000)    14556 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Collator.h
--rwxrwxr-x   0 em        (1000) em        (1000)     9497 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Dilator.C
--rwxrwxr-x   0 em        (1000) em        (1000)    15529 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Dilator.h
--rwxrwxr-x   0 em        (1000) em        (1000)    17254 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Distiller.C
--rwxrwxr-x   0 em        (1000) em        (1000)    15125 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Distiller.h
--rwxrwxr-x   0 em        (1000) em        (1000)     1583 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Envelope.C
--rwxrwxr-x   0 em        (1000) em        (1000)     4642 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Envelope.h
--rwxrwxr-x   0 em        (1000) em        (1000)     1630 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Exception.h
--rwxrwxr-x   0 em        (1000) em        (1000)    22934 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/F0Estimate.C
--rwxrwxr-x   0 em        (1000) em        (1000)     5213 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/F0Estimate.h
--rwxrwxr-x   0 em        (1000) em        (1000)     6538 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Filter.C
--rwxrwxr-x   0 em        (1000) em        (1000)     9426 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Filter.h
--rwxrwxr-x   0 em        (1000) em        (1000)    19699 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/FourierTransform.C
--rwxrwxr-x   0 em        (1000) em        (1000)     8265 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/FourierTransform.h
--rwxrwxr-x   0 em        (1000) em        (1000)     9407 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/FrequencyReference.C
--rwxrwxr-x   0 em        (1000) em        (1000)     4797 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/FrequencyReference.h
--rwxrwxr-x   0 em        (1000) em        (1000)    25411 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Fundamental.C
--rwxrwxr-x   0 em        (1000) em        (1000)    32674 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Fundamental.h
--rwxrwxr-x   0 em        (1000) em        (1000)     5544 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Harmonifier.C
--rwxrwxr-x   0 em        (1000) em        (1000)    17270 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Harmonifier.h
--rwxrwxr-x   0 em        (1000) em        (1000)    14749 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/ImportLemur.C
--rwxrwxr-x   0 em        (1000) em        (1000)     2509 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/ImportLemur.h
--rwxrwxr-x   0 em        (1000) em        (1000)     8267 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/KaiserWindow.C
--rwxrwxr-x   0 em        (1000) em        (1000)     4295 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/KaiserWindow.h
--rwxrwxr-x   0 em        (1000) em        (1000)     5837 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/LinearEnvelope.C
--rwxrwxr-x   0 em        (1000) em        (1000)     9103 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/LinearEnvelope.h
--rwxrwxr-x   0 em        (1000) em        (1000)     3029 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/LorisExceptions.C
--rwxrwxr-x   0 em        (1000) em        (1000)    11388 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/LorisExceptions.h
--rwxrwxr-x   0 em        (1000) em        (1000)     3610 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Makefile.am
--rwxrwxr-x   0 em        (1000) em        (1000)    78206 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Makefile.in
--rwxrwxr-x   0 em        (1000) em        (1000)     5172 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Marker.C
--rwxrwxr-x   0 em        (1000) em        (1000)     5714 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Marker.h
--rwxrwxr-x   0 em        (1000) em        (1000)    60117 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Morpher.C
--rwxrwxr-x   0 em        (1000) em        (1000)    27813 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Morpher.h
--rwxrwxr-x   0 em        (1000) em        (1000)     5823 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/NoiseGenerator.C
--rwxrwxr-x   0 em        (1000) em        (1000)     2811 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/NoiseGenerator.h
--rwxrwxr-x   0 em        (1000) em        (1000)     5527 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Notifier.C
--rwxrwxr-x   0 em        (1000) em        (1000)     4213 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Notifier.h
--rwxrwxr-x   0 em        (1000) em        (1000)     9369 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Oscillator.C
--rwxrwxr-x   0 em        (1000) em        (1000)     5207 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Oscillator.h
--rwxrwxr-x   0 em        (1000) em        (1000)    26751 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Partial.C
--rwxrwxr-x   0 em        (1000) em        (1000)    29096 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Partial.h
--rwxrwxr-x   0 em        (1000) em        (1000)    11661 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/PartialBuilder.C
--rwxrwxr-x   0 em        (1000) em        (1000)     4995 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/PartialBuilder.h
--rwxrwxr-x   0 em        (1000) em        (1000)     2227 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/PartialList.h
--rwxrwxr-x   0 em        (1000) em        (1000)     3927 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/PartialPtrs.h
--rwxrwxr-x   0 em        (1000) em        (1000)    19776 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/PartialUtils.C
--rwxrwxr-x   0 em        (1000) em        (1000)    42918 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/PartialUtils.h
--rwxrwxr-x   0 em        (1000) em        (1000)      241 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/README
--rwxrwxr-x   0 em        (1000) em        (1000)    26232 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/ReassignedSpectrum.C
--rwxrwxr-x   0 em        (1000) em        (1000)     8941 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/ReassignedSpectrum.h
--rwxrwxr-x   0 em        (1000) em        (1000)    14071 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Resampler.C
--rwxrwxr-x   0 em        (1000) em        (1000)    18608 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Resampler.h
--rwxrwxr-x   0 em        (1000) em        (1000)    65946 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/SdifFile.C
--rwxrwxr-x   0 em        (1000) em        (1000)     9333 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/SdifFile.h
--rwxrwxr-x   0 em        (1000) em        (1000)     7824 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Sieve.C
--rwxrwxr-x   0 em        (1000) em        (1000)    10648 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Sieve.h
--rwxrwxr-x   0 em        (1000) em        (1000)    48034 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/SpcFile.C
--rwxrwxr-x   0 em        (1000) em        (1000)    14527 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/SpcFile.h
--rwxrwxr-x   0 em        (1000) em        (1000)     8152 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/SpectralPeakSelector.C
--rwxrwxr-x   0 em        (1000) em        (1000)     2917 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/SpectralPeakSelector.h
--rwxrwxr-x   0 em        (1000) em        (1000)     3351 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/SpectralPeaks.h
--rwxrwxr-x   0 em        (1000) em        (1000)    11444 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/SpectralSurface.C
--rwxrwxr-x   0 em        (1000) em        (1000)    13760 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/SpectralSurface.h
--rwxrwxr-x   0 em        (1000) em        (1000)    19549 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Synthesizer.C
--rwxrwxr-x   0 em        (1000) em        (1000)    15051 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/Synthesizer.h
--rwxrwxr-x   0 em        (1000) em        (1000)    89575 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/fftsg.c
--rwxrwxr-x   0 em        (1000) em        (1000)    42072 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/loris.h.in
--rwxrwxr-x   0 em        (1000) em        (1000)    27092 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/lorisAnalyzer_pi.C
--rwxrwxr-x   0 em        (1000) em        (1000)     6365 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/lorisBpEnvelope_pi.C
--rwxrwxr-x   0 em        (1000) em        (1000)     3919 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/lorisException_pi.C
--rwxrwxr-x   0 em        (1000) em        (1000)     3061 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/lorisException_pi.h
--rwxrwxr-x   0 em        (1000) em        (1000)    33540 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/lorisNonObj_pi.C
--rwxrwxr-x   0 em        (1000) em        (1000)    21648 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/lorisPartialList_pi.C
--rwxrwxr-x   0 em        (1000) em        (1000)    31391 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/lorisUtilities_pi.C
--rwxrwxr-x   0 em        (1000) em        (1000)    17960 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/phasefix.C
--rwxrwxr-x   0 em        (1000) em        (1000)     9508 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/src/phasefix.h
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-09 15:00:09.551993 loristrck-1.5.6/src/loris/win/
--rwxrwxr-x   0 em        (1000) em        (1000)    25018 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/win/Loris_MorphTest.vcproj
--rwxrwxr-x   0 em        (1000) em        (1000)    16896 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/win/Loris_PythonModule.vcproj
--rwxrwxr-x   0 em        (1000) em        (1000)     3775 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/win/config.h
--rwxrwxr-x   0 em        (1000) em        (1000)    42007 2021-11-25 01:27:49.000000 loristrck-1.5.6/src/loris/win/loris.h
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-09 15:00:09.553993 loristrck-1.5.6/test/
--rw-r--r--   0 em        (1000) em        (1000)      817 2023-01-21 18:34:16.000000 loristrck-1.5.6/test/test-analysis.py
--rw-r--r--   0 em        (1000) em        (1000)      680 2023-01-21 18:45:08.000000 loristrck-1.5.6/test/test-fade.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-11 20:28:10.225128 loristrck-1.5.7/
+-rwxrwxr-x   0 em        (1000) em        (1000)     1681 2021-11-25 01:27:49.000000 loristrck-1.5.7/LICENSE
+-rw-rw-r--   0 em        (1000) em        (1000)      296 2021-11-25 01:27:49.000000 loristrck-1.5.7/MANIFEST.in
+-rw-rw-r--   0 em        (1000) em        (1000)     2231 2023-05-11 20:28:10.225128 loristrck-1.5.7/PKG-INFO
+-rwxrwxr-x   0 em        (1000) em        (1000)     1822 2023-04-26 15:20:52.000000 loristrck-1.5.7/README.rst
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-11 20:28:10.128128 loristrck-1.5.7/bin/
+-rwxrwxr-x   0 em        (1000) em        (1000)     3225 2023-01-21 19:17:25.000000 loristrck-1.5.7/bin/loristrck_analyze
+-rwxrwxr-x   0 em        (1000) em        (1000)     3798 2023-04-19 22:30:16.000000 loristrck-1.5.7/bin/loristrck_chord
+-rwxrwxr-x   0 em        (1000) em        (1000)     4213 2021-11-25 01:27:49.000000 loristrck-1.5.7/bin/loristrck_pack
+-rwxrwxr-x   0 em        (1000) em        (1000)     3203 2021-11-25 01:34:31.000000 loristrck-1.5.7/bin/loristrck_synth
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-11 20:28:10.137128 loristrck-1.5.7/loristrck/
+-rwxrwxr-x   0 em        (1000) em        (1000)      344 2021-11-25 01:27:49.000000 loristrck-1.5.7/loristrck/__init__.py
+-rw-rw-r--   0 em        (1000) em        (1000)  1267772 2023-01-21 17:51:56.000000 loristrck-1.5.7/loristrck/_core.cpp
+-rw-rw-r--   0 em        (1000) em        (1000)     2010 2023-05-09 14:59:22.000000 loristrck-1.5.7/loristrck/_core.pyi
+-rwxrwxr-x   0 em        (1000) em        (1000)    26341 2021-11-25 01:27:49.000000 loristrck-1.5.7/loristrck/_core.pyx
+-rw-rw-r--   0 em        (1000) em        (1000)       74 2021-11-25 01:27:49.000000 loristrck-1.5.7/loristrck/common.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     6041 2021-11-25 01:27:49.000000 loristrck-1.5.7/loristrck/lorisdefs.pxd
+-rw-rw-r--   0 em        (1000) em        (1000)     4288 2021-11-25 01:27:49.000000 loristrck-1.5.7/loristrck/play.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     1960 2021-11-25 01:27:49.000000 loristrck-1.5.7/loristrck/plot.py
+-rw-rw-r--   0 em        (1000) em        (1000)        0 2023-05-06 10:27:47.000000 loristrck-1.5.7/loristrck/py.typed
+-rwxrwxr-x   0 em        (1000) em        (1000)    55474 2023-05-11 19:36:31.000000 loristrck-1.5.7/loristrck/util.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-11 20:28:10.138128 loristrck-1.5.7/loristrck.egg-info/
+-rw-rw-r--   0 em        (1000) em        (1000)     2231 2023-05-11 20:28:10.000000 loristrck-1.5.7/loristrck.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)     4117 2023-05-11 20:28:10.000000 loristrck-1.5.7/loristrck.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2023-05-11 20:28:10.000000 loristrck-1.5.7/loristrck.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       43 2023-05-11 20:28:10.000000 loristrck-1.5.7/loristrck.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       10 2023-05-11 20:28:10.000000 loristrck-1.5.7/loristrck.egg-info/top_level.txt
+-rw-r--r--   0 em        (1000) em        (1000)      117 2023-02-26 12:26:54.000000 loristrck-1.5.7/pyproject.toml
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-11 20:28:10.139128 loristrck-1.5.7/scripts/
+-rwxrwxr-x   0 em        (1000) em        (1000)     4010 2021-11-25 01:27:49.000000 loristrck-1.5.7/scripts/prepare_windows_build.py
+-rw-rw-r--   0 em        (1000) em        (1000)      964 2021-11-25 01:27:49.000000 loristrck-1.5.7/scripts/windows-build-wheely.py
+-rwxrwxr-x   0 em        (1000) em        (1000)       67 2023-05-11 20:28:10.225128 loristrck-1.5.7/setup.cfg
+-rwxrwxr-x   0 em        (1000) em        (1000)     5227 2023-05-11 20:27:16.000000 loristrck-1.5.7/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-11 20:28:10.126128 loristrck-1.5.7/src/
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-11 20:28:10.151128 loristrck-1.5.7/src/loris/
+-rwxrwxr-x   0 em        (1000) em        (1000)      177 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/AUTHORS
+-rwxrwxr-x   0 em        (1000) em        (1000)    17982 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/COPYING
+-rwxrwxr-x   0 em        (1000) em        (1000)     7831 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/INSTALL
+-rwxrwxr-x   0 em        (1000) em        (1000)     1455 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/Makefile.am
+-rwxrwxr-x   0 em        (1000) em        (1000)    24527 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/Makefile.in
+-rwxrwxr-x   0 em        (1000) em        (1000)    32377 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/NEWS
+-rwxrwxr-x   0 em        (1000) em        (1000)     2914 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/README
+-rwxrwxr-x   0 em        (1000) em        (1000)      793 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/THANKS
+-rwxrwxr-x   0 em        (1000) em        (1000)   280777 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/aclocal.m4
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-11 20:28:10.158128 loristrck-1.5.7/src/loris/config/
+-rwxrwxr-x   0 em        (1000) em        (1000)     3707 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/config/compile
+-rwxrwxr-x   0 em        (1000) em        (1000)    44941 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/config/config.guess
+-rwxrwxr-x   0 em        (1000) em        (1000)    34423 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/config/config.sub
+-rwxrwxr-x   0 em        (1000) em        (1000)    18615 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/config/depcomp
+-rwxrwxr-x   0 em        (1000) em        (1000)    13663 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/config/install-sh
+-rwxrwxr-x   0 em        (1000) em        (1000)   199705 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/config/ltmain.sh
+-rwxrwxr-x   0 em        (1000) em        (1000)    11419 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/config/missing
+-rwxrwxr-x   0 em        (1000) em        (1000)     4189 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/config/py-compile
+-rwxrwxr-x   0 em        (1000) em        (1000)     3379 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/config.h.in
+-rwxrwxr-x   0 em        (1000) em        (1000)   850178 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/configure
+-rwxrwxr-x   0 em        (1000) em        (1000)    14378 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/configure.ac
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-11 20:28:10.163128 loristrck-1.5.7/src/loris/csound/
+-rwxrwxr-x   0 em        (1000) em        (1000)     1124 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/csound/Makefile.am
+-rwxrwxr-x   0 em        (1000) em        (1000)    19007 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/csound/Makefile.in
+-rwxrwxr-x   0 em        (1000) em        (1000)     4338 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/csound/README
+-rwxrwxr-x   0 em        (1000) em        (1000)    36541 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/csound/lorisgens4.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     2842 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/csound/lorisgens4.h
+-rwxrwxr-x   0 em        (1000) em        (1000)    37239 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/csound/lorisgens5.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     2839 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/csound/lorisgens5.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     2567 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/csound/tryit.csd
+-rwxrwxr-x   0 em        (1000) em        (1000)     3409 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/csound/trymorph.csd
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-11 20:28:10.219128 loristrck-1.5.7/src/loris/src/
+-rwxrwxr-x   0 em        (1000) em        (1000)    29321 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/AiffData.C
+-rwxrwxr-x   0 em        (1000) em        (1000)    11816 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/AiffData.h
+-rwxrwxr-x   0 em        (1000) em        (1000)    18754 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/AiffFile.C
+-rwxrwxr-x   0 em        (1000) em        (1000)    15921 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/AiffFile.h
+-rwxrwxr-x   0 em        (1000) em        (1000)    50936 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Analyzer.C
+-rwxrwxr-x   0 em        (1000) em        (1000)    27787 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Analyzer.h
+-rwxrwxr-x   0 em        (1000) em        (1000)    10512 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/AssociateBandwidth.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     3701 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/AssociateBandwidth.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     3887 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/BigEndian.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     1687 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/BigEndian.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     3643 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Breakpoint.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     4414 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Breakpoint.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     1501 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/BreakpointEnvelope.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     2685 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/BreakpointUtils.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     7352 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/BreakpointUtils.h
+-rwxrwxr-x   0 em        (1000) em        (1000)    23042 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Channelizer.C
+-rwxrwxr-x   0 em        (1000) em        (1000)    24426 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Channelizer.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     6399 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Collator.C
+-rwxrwxr-x   0 em        (1000) em        (1000)    14556 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Collator.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     9497 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Dilator.C
+-rwxrwxr-x   0 em        (1000) em        (1000)    15529 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Dilator.h
+-rwxrwxr-x   0 em        (1000) em        (1000)    17254 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Distiller.C
+-rwxrwxr-x   0 em        (1000) em        (1000)    15125 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Distiller.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     1583 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Envelope.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     4642 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Envelope.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     1630 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Exception.h
+-rwxrwxr-x   0 em        (1000) em        (1000)    22934 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/F0Estimate.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     5213 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/F0Estimate.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     6538 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Filter.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     9426 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Filter.h
+-rwxrwxr-x   0 em        (1000) em        (1000)    19699 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/FourierTransform.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     8265 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/FourierTransform.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     9407 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/FrequencyReference.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     4797 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/FrequencyReference.h
+-rwxrwxr-x   0 em        (1000) em        (1000)    25411 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Fundamental.C
+-rwxrwxr-x   0 em        (1000) em        (1000)    32674 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Fundamental.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     5544 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Harmonifier.C
+-rwxrwxr-x   0 em        (1000) em        (1000)    17270 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Harmonifier.h
+-rwxrwxr-x   0 em        (1000) em        (1000)    14749 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/ImportLemur.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     2509 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/ImportLemur.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     8267 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/KaiserWindow.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     4295 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/KaiserWindow.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     5837 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/LinearEnvelope.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     9103 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/LinearEnvelope.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     3029 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/LorisExceptions.C
+-rwxrwxr-x   0 em        (1000) em        (1000)    11388 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/LorisExceptions.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     3610 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Makefile.am
+-rwxrwxr-x   0 em        (1000) em        (1000)    78206 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Makefile.in
+-rwxrwxr-x   0 em        (1000) em        (1000)     5172 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Marker.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     5714 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Marker.h
+-rwxrwxr-x   0 em        (1000) em        (1000)    60117 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Morpher.C
+-rwxrwxr-x   0 em        (1000) em        (1000)    27813 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Morpher.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     5823 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/NoiseGenerator.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     2811 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/NoiseGenerator.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     5527 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Notifier.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     4213 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Notifier.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     9369 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Oscillator.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     5207 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Oscillator.h
+-rwxrwxr-x   0 em        (1000) em        (1000)    26751 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Partial.C
+-rwxrwxr-x   0 em        (1000) em        (1000)    29096 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Partial.h
+-rwxrwxr-x   0 em        (1000) em        (1000)    11661 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/PartialBuilder.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     4995 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/PartialBuilder.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     2227 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/PartialList.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     3927 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/PartialPtrs.h
+-rwxrwxr-x   0 em        (1000) em        (1000)    19776 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/PartialUtils.C
+-rwxrwxr-x   0 em        (1000) em        (1000)    42918 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/PartialUtils.h
+-rwxrwxr-x   0 em        (1000) em        (1000)      241 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/README
+-rwxrwxr-x   0 em        (1000) em        (1000)    26232 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/ReassignedSpectrum.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     8941 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/ReassignedSpectrum.h
+-rwxrwxr-x   0 em        (1000) em        (1000)    14071 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Resampler.C
+-rwxrwxr-x   0 em        (1000) em        (1000)    18608 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Resampler.h
+-rwxrwxr-x   0 em        (1000) em        (1000)    65946 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/SdifFile.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     9333 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/SdifFile.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     7824 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Sieve.C
+-rwxrwxr-x   0 em        (1000) em        (1000)    10648 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Sieve.h
+-rwxrwxr-x   0 em        (1000) em        (1000)    48034 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/SpcFile.C
+-rwxrwxr-x   0 em        (1000) em        (1000)    14527 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/SpcFile.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     8152 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/SpectralPeakSelector.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     2917 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/SpectralPeakSelector.h
+-rwxrwxr-x   0 em        (1000) em        (1000)     3351 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/SpectralPeaks.h
+-rwxrwxr-x   0 em        (1000) em        (1000)    11444 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/SpectralSurface.C
+-rwxrwxr-x   0 em        (1000) em        (1000)    13760 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/SpectralSurface.h
+-rwxrwxr-x   0 em        (1000) em        (1000)    19549 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Synthesizer.C
+-rwxrwxr-x   0 em        (1000) em        (1000)    15051 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/Synthesizer.h
+-rwxrwxr-x   0 em        (1000) em        (1000)    89575 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/fftsg.c
+-rwxrwxr-x   0 em        (1000) em        (1000)    42072 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/loris.h.in
+-rwxrwxr-x   0 em        (1000) em        (1000)    27092 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/lorisAnalyzer_pi.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     6365 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/lorisBpEnvelope_pi.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     3919 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/lorisException_pi.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     3061 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/lorisException_pi.h
+-rwxrwxr-x   0 em        (1000) em        (1000)    33540 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/lorisNonObj_pi.C
+-rwxrwxr-x   0 em        (1000) em        (1000)    21648 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/lorisPartialList_pi.C
+-rwxrwxr-x   0 em        (1000) em        (1000)    31391 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/lorisUtilities_pi.C
+-rwxrwxr-x   0 em        (1000) em        (1000)    17960 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/phasefix.C
+-rwxrwxr-x   0 em        (1000) em        (1000)     9508 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/src/phasefix.h
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-11 20:28:10.223128 loristrck-1.5.7/src/loris/win/
+-rwxrwxr-x   0 em        (1000) em        (1000)    25018 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/win/Loris_MorphTest.vcproj
+-rwxrwxr-x   0 em        (1000) em        (1000)    16896 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/win/Loris_PythonModule.vcproj
+-rwxrwxr-x   0 em        (1000) em        (1000)     3775 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/win/config.h
+-rwxrwxr-x   0 em        (1000) em        (1000)    42007 2021-11-25 01:27:49.000000 loristrck-1.5.7/src/loris/win/loris.h
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-11 20:28:10.224128 loristrck-1.5.7/test/
+-rw-r--r--   0 em        (1000) em        (1000)      817 2023-01-21 18:34:16.000000 loristrck-1.5.7/test/test-analysis.py
+-rw-r--r--   0 em        (1000) em        (1000)      680 2023-01-21 18:45:08.000000 loristrck-1.5.7/test/test-fade.py
```

### Comparing `loristrck-1.5.6/LICENSE` & `loristrck-1.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/PKG-INFO` & `loristrck-1.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loristrck
-Version: 1.5.6
+Version: 1.5.7
 Summary: A wrapper around the partial-tracking library Loris
 Home-page: https://github.com/gesellkammer/loristrck
 Download-URL: https://github.com/gesellkammer/loristrck
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: GPL
 Platform: Linux
```

### Comparing `loristrck-1.5.6/README.rst` & `loristrck-1.5.7/README.rst`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/bin/loristrck_analyze` & `loristrck-1.5.7/bin/loristrck_analyze`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/bin/loristrck_chord` & `loristrck-1.5.7/bin/loristrck_chord`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/bin/loristrck_pack` & `loristrck-1.5.7/bin/loristrck_pack`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/bin/loristrck_synth` & `loristrck-1.5.7/bin/loristrck_synth`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/loristrck/_core.cpp` & `loristrck-1.5.7/loristrck/_core.cpp`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/loristrck/_core.pyi` & `loristrck-1.5.7/loristrck/_core.pyi`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/loristrck/_core.pyx` & `loristrck-1.5.7/loristrck/_core.pyx`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/loristrck/lorisdefs.pxd` & `loristrck-1.5.7/loristrck/lorisdefs.pxd`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/loristrck/play.py` & `loristrck-1.5.7/loristrck/play.py`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/loristrck/plot.py` & `loristrck-1.5.7/loristrck/plot.py`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/loristrck/util.py` & `loristrck-1.5.7/loristrck/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 """
 from __future__ import annotations
 import os
 import numpy as np
 import numpyx as npx
 import importlib
-import soundfile
 import logging
 import math
 import sys
 
 from . import _core
 
 logger = logging.getLogger("loristrck")
@@ -821,14 +820,15 @@
 
     assert bits in (32, 64)
     if fmt is None:
         fmt = os.path.splitext(outfile)[1][1:].lower()
 
     assert fmt in ('wav', 'aif')
     subtype = 'FLOAT' if bits == 32 else 'DOUBLE'
+    import soundfile
     return soundfile.SoundFile(outfile, mode="w", samplerate=sr, channels=channels,
                                format=fmt, subtype=subtype)
 
 
 def wavwrite(outfile: str, samples: np.ndarray, sr=44100, bits=32) -> None:
     """
     Write samples to a wav-file (see also sndwrite) as float32 or float64
@@ -841,15 +841,15 @@
     """
     f = _wavwriter(outfile, sr=sr, bits=bits, channels=_numchannels(samples))
     f.write(samples)
     f.close()
 
 
 def partials_save_matrix(partials: list[np.ndarray],
-                         outfile: str,
+                         outfile: str = '',
                          dt: float = None,
                          gapfactor=3.,
                          maxtracks=0,
                          maxactive=0
                          ) -> tuple[list[np.ndarray], np.ndarray]:
     """
     Packs short partials into longer partials and saves the result as a matrix
@@ -869,15 +869,15 @@
         partials: a list of numpy 2D-arrays, each representing a partial
         dt: sampling period to sample the packed partials. If not given,
             it will be estimated with sensible defaults. To have more control
             over this stage, you can call estimate_sampling_interval yourself.
             At the cost of oversampling, a good value can be ksmps/sr, which results
             in 64/44100 = 0.0014 secs for typical values
         outfile: path to save the sampled partials. Supported formats: `.mtx`, `.npy`
-            (See matrix_save for more information)
+            (See matrix_save for more information). If not given, the matrix is not saved
         gapfactor: partials are packed with a gap = dt * gapfactor.
             It should be at least 2. A gap is a minimal amount of silence
             between the partials to allow for a fade out and fade in
         maxtracks: Partials are packed in tracks and represented as a 2D matrix where
             each track is a row. If filesize and save/load time are a concern,
             a max. value for the amount of tracks can be given here, with the
             consequence that partials might be left out if there are no available
@@ -893,15 +893,20 @@
     """
     if dt is None:
         dt = estimate_sampling_interval(partials)
     assert all(isinstance(p, np.ndarray) for p in partials)
     gap = dt*gapfactor
     tracks, rest = pack(partials, gap=gap, maxtracks=maxtracks)
     mtx = partials_sample(tracks, dt=dt, maxactive=maxactive)
-    matrix_save(mtx, outfile, bits=32, metadata={'dt': dt, 'numTracks': len(tracks), 'gap': gap, 'maxActive': maxactive})
+    if outfile:
+        metadata = {'dt': dt, 
+                    'numTracks': len(tracks), 
+                    'gap': gap, 
+                    'maxActive': maxactive}
+        matrix_save(mtx, outfile, bits=32, metadata=metadata)
     return tracks, mtx
 
 
 def _numchannels(samples: np.ndarray) -> int:
     return 1 if samples.ndim == 1 else samples.shape[1]
 
 
@@ -916,14 +921,15 @@
         contiguous: If True, it is ensured that the returned array 
             is contiguous. This should be set to True if the samples are to be
             passed to `analyze`, which expects a contiguous array
 
     Returns:
         a tuple (samples:np.ndarray, sr:int)
     """
+    import soundfile
     samples, sr = soundfile.read(path)
     if contiguous:
         samples = np.ascontiguousarray(samples)
     return samples, sr
 
 
 def sndreadmono(path: str, chan: int = 0, contiguous=True
@@ -939,14 +945,15 @@
         contiguous: If True, it is ensured that the returned array 
             is contiguous. This should be set to True if the samples are to be
             passed to `analyze`, which expects a contiguous array
 
     Returns:
         a tuple (samples:np.ndarray, sr:int)
     """
+    import soundfile
     samples, sr = soundfile.read(path)
     if _numchannels(samples) > 1:
         samples = samples[:, chan]
     if contiguous:
         samples = np.ascontiguousarray(samples)
     return samples, sr
 
@@ -960,14 +967,16 @@
         sr: samplerate
         path: the outfile to write the samples to (the extension will determine the format)
         encoding: the encoding of the samples. If None, a default is used, according to
             the extension of the outfile given. Otherwise, a string 'floatXX' or 'pcmXX'
             is expected, where XX represent the bits per sample (15, 24, 32, 64 for pcm,
             32 or 64 for float). Not all encodings are supported by all formats.
     """
+    import soundfile
+
     if isinstance(encoding, str):
         encoding = encoding[:-2], int(encoding[-2:])
     elif encoding is None:
         ext = os.path.splitext(path)[1].lower()
         encoding = {
             '.wav':'float32',
             '.aif':'float32',
```

### Comparing `loristrck-1.5.6/loristrck.egg-info/PKG-INFO` & `loristrck-1.5.7/loristrck.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loristrck
-Version: 1.5.6
+Version: 1.5.7
 Summary: A wrapper around the partial-tracking library Loris
 Home-page: https://github.com/gesellkammer/loristrck
 Download-URL: https://github.com/gesellkammer/loristrck
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: GPL
 Platform: Linux
```

### Comparing `loristrck-1.5.6/loristrck.egg-info/SOURCES.txt` & `loristrck-1.5.7/loristrck.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/scripts/prepare_windows_build.py` & `loristrck-1.5.7/scripts/prepare_windows_build.py`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/scripts/windows-build-wheely.py` & `loristrck-1.5.7/scripts/windows-build-wheely.py`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/setup.py` & `loristrck-1.5.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
 import glob
 from setuptools import setup, Extension
 import shutil
 
-VERSION = '1.5.6'
+VERSION = '1.5.7'
 
 class get_numpy_include(str):
     def __str__(self):
         import numpy
         return numpy.get_include()
 
 # -----------------------------------------------------------------------------
```

### Comparing `loristrck-1.5.6/src/loris/COPYING` & `loristrck-1.5.7/src/loris/COPYING`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/INSTALL` & `loristrck-1.5.7/src/loris/INSTALL`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/Makefile.am` & `loristrck-1.5.7/src/loris/Makefile.am`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/Makefile.in` & `loristrck-1.5.7/src/loris/Makefile.in`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/NEWS` & `loristrck-1.5.7/src/loris/NEWS`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/README` & `loristrck-1.5.7/src/loris/README`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/THANKS` & `loristrck-1.5.7/src/loris/THANKS`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/aclocal.m4` & `loristrck-1.5.7/src/loris/aclocal.m4`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/config/compile` & `loristrck-1.5.7/src/loris/config/compile`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/config/config.guess` & `loristrck-1.5.7/src/loris/config/config.guess`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/config/config.sub` & `loristrck-1.5.7/src/loris/config/config.sub`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/config/depcomp` & `loristrck-1.5.7/src/loris/config/depcomp`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/config/install-sh` & `loristrck-1.5.7/src/loris/config/install-sh`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/config/ltmain.sh` & `loristrck-1.5.7/src/loris/config/ltmain.sh`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/config/missing` & `loristrck-1.5.7/src/loris/config/missing`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/config/py-compile` & `loristrck-1.5.7/src/loris/config/py-compile`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/config.h.in` & `loristrck-1.5.7/src/loris/config.h.in`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/configure` & `loristrck-1.5.7/src/loris/configure`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/configure.ac` & `loristrck-1.5.7/src/loris/configure.ac`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/csound/Makefile.am` & `loristrck-1.5.7/src/loris/csound/Makefile.am`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/csound/Makefile.in` & `loristrck-1.5.7/src/loris/csound/Makefile.in`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/csound/README` & `loristrck-1.5.7/src/loris/csound/README`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/csound/lorisgens4.C` & `loristrck-1.5.7/src/loris/csound/lorisgens4.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/csound/lorisgens4.h` & `loristrck-1.5.7/src/loris/csound/lorisgens4.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/csound/lorisgens5.C` & `loristrck-1.5.7/src/loris/csound/lorisgens5.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/csound/lorisgens5.h` & `loristrck-1.5.7/src/loris/csound/lorisgens5.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/csound/tryit.csd` & `loristrck-1.5.7/src/loris/csound/tryit.csd`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/csound/trymorph.csd` & `loristrck-1.5.7/src/loris/csound/trymorph.csd`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/AiffData.C` & `loristrck-1.5.7/src/loris/src/AiffData.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/AiffData.h` & `loristrck-1.5.7/src/loris/src/AiffData.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/AiffFile.C` & `loristrck-1.5.7/src/loris/src/AiffFile.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/AiffFile.h` & `loristrck-1.5.7/src/loris/src/AiffFile.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Analyzer.C` & `loristrck-1.5.7/src/loris/src/Analyzer.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Analyzer.h` & `loristrck-1.5.7/src/loris/src/Analyzer.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/AssociateBandwidth.C` & `loristrck-1.5.7/src/loris/src/AssociateBandwidth.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/AssociateBandwidth.h` & `loristrck-1.5.7/src/loris/src/AssociateBandwidth.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/BigEndian.C` & `loristrck-1.5.7/src/loris/src/BigEndian.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/BigEndian.h` & `loristrck-1.5.7/src/loris/src/BigEndian.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Breakpoint.C` & `loristrck-1.5.7/src/loris/src/Breakpoint.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Breakpoint.h` & `loristrck-1.5.7/src/loris/src/Breakpoint.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/BreakpointEnvelope.h` & `loristrck-1.5.7/src/loris/src/BreakpointEnvelope.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/BreakpointUtils.C` & `loristrck-1.5.7/src/loris/src/BreakpointUtils.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/BreakpointUtils.h` & `loristrck-1.5.7/src/loris/src/BreakpointUtils.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Channelizer.C` & `loristrck-1.5.7/src/loris/src/Channelizer.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Channelizer.h` & `loristrck-1.5.7/src/loris/src/Channelizer.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Collator.C` & `loristrck-1.5.7/src/loris/src/Collator.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Collator.h` & `loristrck-1.5.7/src/loris/src/Collator.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Dilator.C` & `loristrck-1.5.7/src/loris/src/Dilator.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Dilator.h` & `loristrck-1.5.7/src/loris/src/Dilator.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Distiller.C` & `loristrck-1.5.7/src/loris/src/Distiller.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Distiller.h` & `loristrck-1.5.7/src/loris/src/Distiller.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Envelope.C` & `loristrck-1.5.7/src/loris/src/Envelope.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Envelope.h` & `loristrck-1.5.7/src/loris/src/Envelope.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Exception.h` & `loristrck-1.5.7/src/loris/src/Exception.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/F0Estimate.C` & `loristrck-1.5.7/src/loris/src/F0Estimate.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/F0Estimate.h` & `loristrck-1.5.7/src/loris/src/F0Estimate.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Filter.C` & `loristrck-1.5.7/src/loris/src/Filter.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Filter.h` & `loristrck-1.5.7/src/loris/src/Filter.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/FourierTransform.C` & `loristrck-1.5.7/src/loris/src/FourierTransform.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/FourierTransform.h` & `loristrck-1.5.7/src/loris/src/FourierTransform.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/FrequencyReference.C` & `loristrck-1.5.7/src/loris/src/FrequencyReference.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/FrequencyReference.h` & `loristrck-1.5.7/src/loris/src/FrequencyReference.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Fundamental.C` & `loristrck-1.5.7/src/loris/src/Fundamental.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Fundamental.h` & `loristrck-1.5.7/src/loris/src/Fundamental.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Harmonifier.C` & `loristrck-1.5.7/src/loris/src/Harmonifier.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Harmonifier.h` & `loristrck-1.5.7/src/loris/src/Harmonifier.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/ImportLemur.C` & `loristrck-1.5.7/src/loris/src/ImportLemur.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/ImportLemur.h` & `loristrck-1.5.7/src/loris/src/ImportLemur.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/KaiserWindow.C` & `loristrck-1.5.7/src/loris/src/KaiserWindow.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/KaiserWindow.h` & `loristrck-1.5.7/src/loris/src/KaiserWindow.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/LinearEnvelope.C` & `loristrck-1.5.7/src/loris/src/LinearEnvelope.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/LinearEnvelope.h` & `loristrck-1.5.7/src/loris/src/LinearEnvelope.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/LorisExceptions.C` & `loristrck-1.5.7/src/loris/src/LorisExceptions.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/LorisExceptions.h` & `loristrck-1.5.7/src/loris/src/LorisExceptions.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Makefile.am` & `loristrck-1.5.7/src/loris/src/Makefile.am`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Makefile.in` & `loristrck-1.5.7/src/loris/src/Makefile.in`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Marker.C` & `loristrck-1.5.7/src/loris/src/Marker.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Marker.h` & `loristrck-1.5.7/src/loris/src/Marker.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Morpher.C` & `loristrck-1.5.7/src/loris/src/Morpher.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Morpher.h` & `loristrck-1.5.7/src/loris/src/Morpher.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/NoiseGenerator.C` & `loristrck-1.5.7/src/loris/src/NoiseGenerator.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/NoiseGenerator.h` & `loristrck-1.5.7/src/loris/src/NoiseGenerator.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Notifier.C` & `loristrck-1.5.7/src/loris/src/Notifier.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Notifier.h` & `loristrck-1.5.7/src/loris/src/Notifier.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Oscillator.C` & `loristrck-1.5.7/src/loris/src/Oscillator.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Oscillator.h` & `loristrck-1.5.7/src/loris/src/Oscillator.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Partial.C` & `loristrck-1.5.7/src/loris/src/Partial.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Partial.h` & `loristrck-1.5.7/src/loris/src/Partial.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/PartialBuilder.C` & `loristrck-1.5.7/src/loris/src/PartialBuilder.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/PartialBuilder.h` & `loristrck-1.5.7/src/loris/src/PartialBuilder.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/PartialList.h` & `loristrck-1.5.7/src/loris/src/PartialList.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/PartialPtrs.h` & `loristrck-1.5.7/src/loris/src/PartialPtrs.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/PartialUtils.C` & `loristrck-1.5.7/src/loris/src/PartialUtils.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/PartialUtils.h` & `loristrck-1.5.7/src/loris/src/PartialUtils.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/ReassignedSpectrum.C` & `loristrck-1.5.7/src/loris/src/ReassignedSpectrum.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/ReassignedSpectrum.h` & `loristrck-1.5.7/src/loris/src/ReassignedSpectrum.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Resampler.C` & `loristrck-1.5.7/src/loris/src/Resampler.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Resampler.h` & `loristrck-1.5.7/src/loris/src/Resampler.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/SdifFile.C` & `loristrck-1.5.7/src/loris/src/SdifFile.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/SdifFile.h` & `loristrck-1.5.7/src/loris/src/SdifFile.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Sieve.C` & `loristrck-1.5.7/src/loris/src/Sieve.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Sieve.h` & `loristrck-1.5.7/src/loris/src/Sieve.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/SpcFile.C` & `loristrck-1.5.7/src/loris/src/SpcFile.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/SpcFile.h` & `loristrck-1.5.7/src/loris/src/SpcFile.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/SpectralPeakSelector.C` & `loristrck-1.5.7/src/loris/src/SpectralPeakSelector.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/SpectralPeakSelector.h` & `loristrck-1.5.7/src/loris/src/SpectralPeakSelector.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/SpectralPeaks.h` & `loristrck-1.5.7/src/loris/src/SpectralPeaks.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/SpectralSurface.C` & `loristrck-1.5.7/src/loris/src/SpectralSurface.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/SpectralSurface.h` & `loristrck-1.5.7/src/loris/src/SpectralSurface.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Synthesizer.C` & `loristrck-1.5.7/src/loris/src/Synthesizer.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/Synthesizer.h` & `loristrck-1.5.7/src/loris/src/Synthesizer.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/fftsg.c` & `loristrck-1.5.7/src/loris/src/fftsg.c`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/loris.h.in` & `loristrck-1.5.7/src/loris/src/loris.h.in`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/lorisAnalyzer_pi.C` & `loristrck-1.5.7/src/loris/src/lorisAnalyzer_pi.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/lorisBpEnvelope_pi.C` & `loristrck-1.5.7/src/loris/src/lorisBpEnvelope_pi.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/lorisException_pi.C` & `loristrck-1.5.7/src/loris/src/lorisException_pi.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/lorisException_pi.h` & `loristrck-1.5.7/src/loris/src/lorisException_pi.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/lorisNonObj_pi.C` & `loristrck-1.5.7/src/loris/src/lorisNonObj_pi.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/lorisPartialList_pi.C` & `loristrck-1.5.7/src/loris/src/lorisPartialList_pi.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/lorisUtilities_pi.C` & `loristrck-1.5.7/src/loris/src/lorisUtilities_pi.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/phasefix.C` & `loristrck-1.5.7/src/loris/src/phasefix.C`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/src/phasefix.h` & `loristrck-1.5.7/src/loris/src/phasefix.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/win/Loris_MorphTest.vcproj` & `loristrck-1.5.7/src/loris/win/Loris_MorphTest.vcproj`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/win/Loris_PythonModule.vcproj` & `loristrck-1.5.7/src/loris/win/Loris_PythonModule.vcproj`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/win/config.h` & `loristrck-1.5.7/src/loris/win/config.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/src/loris/win/loris.h` & `loristrck-1.5.7/src/loris/win/loris.h`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/test/test-analysis.py` & `loristrck-1.5.7/test/test-analysis.py`

 * *Files identical despite different names*

### Comparing `loristrck-1.5.6/test/test-fade.py` & `loristrck-1.5.7/test/test-fade.py`

 * *Files identical despite different names*

