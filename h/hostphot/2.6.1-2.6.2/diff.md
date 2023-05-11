# Comparing `tmp/hostphot-2.6.1.tar.gz` & `tmp/hostphot-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hostphot-2.6.1.tar", last modified: Tue May  9 01:58:27 2023, max compression
+gzip compressed data, was "hostphot-2.6.2.tar", last modified: Thu May 11 03:15:08 2023, max compression
```

## Comparing `hostphot-2.6.1.tar` & `hostphot-2.6.2.tar`

### file list

```diff
@@ -1,330 +1,330 @@
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-09 01:58:27.747313 hostphot-2.6.1/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1065 2022-05-31 09:22:42.000000 hostphot-2.6.1/LICENSE
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       53 2022-05-31 09:22:42.000000 hostphot-2.6.1/MANIFEST.in
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9027 2023-05-09 01:58:27.747313 hostphot-2.6.1/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     8495 2023-05-09 01:48:52.000000 hostphot-2.6.1/README.md
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      187 2022-05-31 09:22:42.000000 hostphot-2.6.1/pyproject.toml
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      184 2023-04-28 09:57:11.000000 hostphot-2.6.1/requirements.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-05-09 01:58:27.747313 hostphot-2.6.1/setup.cfg
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1251 2023-04-28 09:57:11.000000 hostphot-2.6.1/setup.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-09 01:58:27.683313 hostphot-2.6.1/src/
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-09 01:58:27.687313 hostphot-2.6.1/src/hostphot/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      412 2022-08-30 07:45:59.000000 hostphot-2.6.1/src/hostphot/__init__.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      123 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/_constants.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       47 2023-05-08 10:28:52.000000 hostphot-2.6.1/src/hostphot/_version.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1762 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/coadd.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    45990 2023-05-09 01:57:23.000000 hostphot-2.6.1/src/hostphot/cutouts.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6006 2023-05-05 10:39:56.000000 hostphot-2.6.1/src/hostphot/dust.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-09 01:58:27.687313 hostphot-2.6.1/src/hostphot/filters/
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-09 01:58:27.687313 hostphot-2.6.1/src/hostphot/filters/2MASS/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1218 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/filters/2MASS/2MASS_H.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2247 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/filters/2MASS/2MASS_J.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1596 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/filters/2MASS/2MASS_Ks.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/filters/2MASS/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1549 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/filters/AAA_README
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-09 01:58:27.691313 hostphot-2.6.1/src/hostphot/filters/DES/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       53 2022-05-31 09:22:42.000000 hostphot-2.6.1/src/hostphot/filters/DES/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3387 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/filters/DES/DES_Y.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4281 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/filters/DES/DES_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4515 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/filters/DES/DES_i.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4516 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/filters/DES/DES_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4338 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/filters/DES/DES_z.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-09 01:58:27.691313 hostphot-2.6.1/src/hostphot/filters/GALEX/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/filters/GALEX/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6777 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/filters/GALEX/GALEX_FUV.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18911 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/filters/GALEX/GALEX_NUV.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-09 01:58:27.691313 hostphot-2.6.1/src/hostphot/filters/HST/
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-09 01:58:27.699313 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    23838 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F435W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    32416 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F475W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4110 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F502N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    15624 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F550M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    31966 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F555W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    43735 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F606W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    29858 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F625W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5234 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F658N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3236 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F660N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    37258 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F775W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   103143 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F814W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    53451 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F850LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7990 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F892N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21666 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR1016N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9107 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR388N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9858 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR423N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    36616 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR459M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    10646 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR462N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11519 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR505N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12578 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR551N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13680 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR601N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    53850 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR647M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    14675 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR656N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    15873 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR716N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    17289 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR782N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18750 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR853N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    61170 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR914M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19635 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR931N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1264 2023-05-05 10:39:56.000000 hostphot-2.6.1/src/hostphot/filters/HST/IR_err.txt
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-09 01:58:27.699313 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9747 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F090M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2486 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F095N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2874 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F097N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3264 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F108N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12445 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24500 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3077 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F113N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    33411 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F140W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13978 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F145M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21021 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F160W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4877 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F164N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11680 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F165M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5199 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F166N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12148 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F170M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6879 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F187N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7831 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F190N.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-09 01:58:27.703313 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24275 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F110W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20849 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F160W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12018 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F165M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18588 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F171M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    17947 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F180M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6506 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    41358 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5506 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F190N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21662 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F204M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    30947 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F205W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20965 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F207M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11516 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F212N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7894 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F215N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7479 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F216N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    30813 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F222M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26323 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F237M.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-09 01:58:27.707313 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3240 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F108N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24427 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F110W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3363 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F113N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    35249 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F150W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20994 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F160W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4858 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F164N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4820 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F166N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    43711 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F175W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6876 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F187N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5510 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F190N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7212 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F196N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9291 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F200N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11541 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F212N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7906 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F215N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    30812 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F222M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13019 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F240M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3503 2023-05-05 10:39:56.000000 hostphot-2.6.1/src/hostphot/filters/HST/UVIS1_err.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3503 2023-05-05 10:39:56.000000 hostphot-2.6.1/src/hostphot/filters/HST/UVIS2_err.txt
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-09 01:58:27.711313 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     8959 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F098M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9826 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F105W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21512 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F110W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    22426 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F125W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4121 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F126N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5064 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F127M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6580 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F128N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3261 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F130N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3792 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F132N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5421 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F139M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13977 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F140W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6752 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F153M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    10046 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F160W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4738 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F164N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6887 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F167N.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-09 01:58:27.723313 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   156254 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F200LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21978 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F218W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    29976 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F225W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21591 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F275W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7558 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F280N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    56436 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F300X.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    15547 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F336W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19356 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F343N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   146819 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F350LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4504 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F373N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9638 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26406 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7035 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F395N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9314 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F410M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18697 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F438W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9833 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F467M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3637 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F469N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    32782 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    72677 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475X.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5098 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F487N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5804 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F502N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    38578 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F547M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    63538 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F555W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    97333 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F600LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    51442 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F606W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21890 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F621M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    34917 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F625W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4204 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F631N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3675 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F645N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2150 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F656N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11299 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F657N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3236 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F658N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11865 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F665N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11991 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F673N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13792 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F680N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20007 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F689M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19898 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F763M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    36590 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F775W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    54378 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F814W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    33733 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F845M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    57316 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F850LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12497 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F953N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13422 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ232N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13900 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ243N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21137 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ378N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6727 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ387N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    39729 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ422M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11393 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ436N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1548 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ437N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    22828 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ492N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26635 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ508N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4658 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ575N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19283 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ619N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20492 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ634N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4687 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ672N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4387 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ674N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24973 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ727N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    25138 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ750N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2950 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ889N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2948 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ906N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3346 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ924N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3461 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ937N.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-09 01:58:27.739313 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   156503 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F200LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20752 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F218W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    29190 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F225W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21479 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F275W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7566 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F280N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    55542 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F300X.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    15542 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F336W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19332 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F343N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   147032 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F350LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4495 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F373N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9640 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26441 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7031 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F395N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9300 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F410M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18727 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F438W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9871 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F467M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3641 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F469N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    32751 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    72732 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475X.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5104 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F487N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5798 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F502N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    38608 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F547M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    63493 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F555W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    97494 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F600LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    51384 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F606W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21858 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F621M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    34960 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F625W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4209 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F631N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3686 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F645N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2154 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F656N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11309 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F657N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3233 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F658N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11857 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F665N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11991 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F673N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13805 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F680N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20019 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F689M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19919 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F763M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    36600 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F775W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    54473 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F814W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    33739 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F845M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    57507 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F850LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12507 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F953N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13422 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ232N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13900 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ243N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21137 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ378N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6727 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ387N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    39729 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ422M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11393 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ436N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1548 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ437N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    22828 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ492N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26635 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ508N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4658 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ575N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19283 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ619N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20492 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ634N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4687 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ672N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4387 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ674N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24973 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ727N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    25138 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ750N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2950 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ889N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2948 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ906N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3346 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ924N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3461 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ937N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2012 2023-05-05 10:39:56.000000 hostphot-2.6.1/src/hostphot/filters/HST/ir_aper_corrections.csv
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18667 2023-05-05 10:39:56.000000 hostphot-2.6.1/src/hostphot/filters/HST/wfc3uvis1_aper_007_syn.csv
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18635 2023-05-05 10:39:56.000000 hostphot-2.6.1/src/hostphot/filters/HST/wfc3uvis2_aper_007_syn.csv
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-09 01:58:27.739313 hostphot-2.6.1/src/hostphot/filters/LegacySurvey/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2281 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/filters/LegacySurvey/BASS_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3180 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/filters/LegacySurvey/BASS_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21743 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/filters/LegacySurvey/DECAM_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21744 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/filters/LegacySurvey/DECAM_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21744 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/filters/LegacySurvey/DECAM_z.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7028 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/filters/LegacySurvey/MzLS_z.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      300 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/filters/LegacySurvey/README.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4275 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/filters/LegacySurvey/init_BASS_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5840 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/filters/LegacySurvey/init_BASS_r.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-09 01:58:27.739313 hostphot-2.6.1/src/hostphot/filters/PS1/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      136 2022-05-31 09:22:42.000000 hostphot-2.6.1/src/hostphot/filters/PS1/AAA_README.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3717 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/filters/PS1/PS1_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3759 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/filters/PS1/PS1_i.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3885 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/filters/PS1/PS1_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4385 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/filters/PS1/PS1_y.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3486 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/filters/PS1/PS1_z.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-09 01:58:27.739313 hostphot-2.6.1/src/hostphot/filters/SDSS/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       72 2022-05-31 09:22:42.000000 hostphot-2.6.1/src/hostphot/filters/SDSS/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1414 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/filters/SDSS/SDSS_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1260 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/filters/SDSS/SDSS_i.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1176 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/filters/SDSS/SDSS_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4718 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/filters/SDSS/SDSS_u.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2509 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/filters/SDSS/SDSS_z.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-09 01:58:27.743313 hostphot-2.6.1/src/hostphot/filters/Spitzer/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      189 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/filters/Spitzer/README.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     8211 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.1.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     8421 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.2.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6531 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.3.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7375 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.4.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2816 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/filters/Spitzer/Spitzer_MIPS.1.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-09 01:58:27.743313 hostphot-2.6.1/src/hostphot/filters/VISTA/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       84 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/filters/VISTA/README.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    39168 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/filters/VISTA/VISTA_H.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    50048 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/filters/VISTA/VISTA_J.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    41344 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/filters/VISTA/VISTA_Ks.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    46341 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/filters/VISTA/VISTA_Y.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   176418 2022-11-14 14:06:00.000000 hostphot-2.6.1/src/hostphot/filters/VISTA/VISTA_Z.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-09 01:58:27.743313 hostphot-2.6.1/src/hostphot/filters/WISE/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/filters/WISE/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2961 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/WISE/WISE_W1.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3528 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/WISE/WISE_W2.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24404 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/WISE/WISE_W3.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19734 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/filters/WISE/WISE_W4.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      739 2023-04-24 13:20:08.000000 hostphot-2.6.1/src/hostphot/filters/config.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    22899 2023-05-05 10:39:56.000000 hostphot-2.6.1/src/hostphot/global_photometry.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2494 2022-07-28 14:32:41.000000 hostphot-2.6.1/src/hostphot/image_cleaning.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12319 2023-04-25 09:34:42.000000 hostphot-2.6.1/src/hostphot/image_masking.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12493 2023-04-25 09:34:42.000000 hostphot-2.6.1/src/hostphot/interactive_aperture.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13261 2023-05-05 10:39:56.000000 hostphot-2.6.1/src/hostphot/local_photometry.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     8326 2023-04-25 09:34:42.000000 hostphot-2.6.1/src/hostphot/objects_detect.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    10706 2022-08-15 08:03:30.000000 hostphot-2.6.1/src/hostphot/rgb_images.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    30137 2023-05-05 10:39:56.000000 hostphot-2.6.1/src/hostphot/utils.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-09 01:58:27.687313 hostphot-2.6.1/src/hostphot.egg-info/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9027 2023-05-09 01:58:27.000000 hostphot-2.6.1/src/hostphot.egg-info/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    14942 2023-05-09 01:58:27.000000 hostphot-2.6.1/src/hostphot.egg-info/SOURCES.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-05-09 01:58:27.000000 hostphot-2.6.1/src/hostphot.egg-info/dependency_links.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      187 2023-05-09 01:58:27.000000 hostphot-2.6.1/src/hostphot.egg-info/requires.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        9 2023-05-09 01:58:27.000000 hostphot-2.6.1/src/hostphot.egg-info/top_level.txt
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-09 01:58:27.747313 hostphot-2.6.1/tests/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2771 2023-04-25 09:34:42.000000 hostphot-2.6.1/tests/test_cutouts.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1073 2023-04-28 09:57:11.000000 hostphot-2.6.1/tests/test_global_phot.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      460 2022-07-28 14:32:41.000000 hostphot-2.6.1/tests/test_interactivity.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1088 2023-04-28 09:57:11.000000 hostphot-2.6.1/tests/test_local_phot.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1095 2022-07-28 14:32:41.000000 hostphot-2.6.1/tests/test_preprocessing.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      860 2023-04-25 09:34:42.000000 hostphot-2.6.1/tests/test_rgb_images.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 03:15:08.076763 hostphot-2.6.2/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1065 2022-05-31 09:22:42.000000 hostphot-2.6.2/LICENSE
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       53 2022-05-31 09:22:42.000000 hostphot-2.6.2/MANIFEST.in
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9235 2023-05-11 03:15:08.076763 hostphot-2.6.2/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8703 2023-05-11 02:29:33.000000 hostphot-2.6.2/README.md
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      187 2022-05-31 09:22:42.000000 hostphot-2.6.2/pyproject.toml
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      190 2023-05-11 02:29:33.000000 hostphot-2.6.2/requirements.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-05-11 03:15:08.076763 hostphot-2.6.2/setup.cfg
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1251 2023-04-28 09:57:11.000000 hostphot-2.6.2/setup.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 03:15:08.024766 hostphot-2.6.2/src/
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 03:15:08.028766 hostphot-2.6.2/src/hostphot/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      412 2022-08-30 07:45:59.000000 hostphot-2.6.2/src/hostphot/__init__.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      123 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/_constants.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       47 2023-05-11 02:29:33.000000 hostphot-2.6.2/src/hostphot/_version.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1762 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/coadd.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    45897 2023-05-11 02:29:33.000000 hostphot-2.6.2/src/hostphot/cutouts.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6006 2023-05-05 10:39:56.000000 hostphot-2.6.2/src/hostphot/dust.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 03:15:08.028766 hostphot-2.6.2/src/hostphot/filters/
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 03:15:08.028766 hostphot-2.6.2/src/hostphot/filters/2MASS/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1218 2022-07-28 14:32:41.000000 hostphot-2.6.2/src/hostphot/filters/2MASS/2MASS_H.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2247 2022-07-28 14:32:41.000000 hostphot-2.6.2/src/hostphot/filters/2MASS/2MASS_J.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1596 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/filters/2MASS/2MASS_Ks.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.6.2/src/hostphot/filters/2MASS/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1549 2022-07-28 14:32:41.000000 hostphot-2.6.2/src/hostphot/filters/AAA_README
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 03:15:08.028766 hostphot-2.6.2/src/hostphot/filters/DES/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       53 2022-05-31 09:22:42.000000 hostphot-2.6.2/src/hostphot/filters/DES/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3387 2022-07-28 14:32:41.000000 hostphot-2.6.2/src/hostphot/filters/DES/DES_Y.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4281 2022-07-28 14:32:41.000000 hostphot-2.6.2/src/hostphot/filters/DES/DES_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4515 2022-07-28 14:32:41.000000 hostphot-2.6.2/src/hostphot/filters/DES/DES_i.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4516 2022-07-28 14:32:41.000000 hostphot-2.6.2/src/hostphot/filters/DES/DES_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4338 2022-07-28 14:32:41.000000 hostphot-2.6.2/src/hostphot/filters/DES/DES_z.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 03:15:08.028766 hostphot-2.6.2/src/hostphot/filters/GALEX/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.6.2/src/hostphot/filters/GALEX/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6777 2022-07-28 14:32:41.000000 hostphot-2.6.2/src/hostphot/filters/GALEX/GALEX_FUV.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18911 2022-07-28 14:32:41.000000 hostphot-2.6.2/src/hostphot/filters/GALEX/GALEX_NUV.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 03:15:08.028766 hostphot-2.6.2/src/hostphot/filters/HST/
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 03:15:08.036765 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    23838 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F435W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    32416 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F475W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4110 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F502N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    15624 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F550M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    31966 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F555W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    43735 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F606W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    29858 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F625W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5234 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F658N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3236 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F660N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    37258 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F775W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   103143 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F814W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    53451 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F850LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7990 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F892N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21666 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR1016N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9107 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR388N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9858 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR423N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    36616 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR459M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    10646 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR462N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11519 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR505N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12578 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR551N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13680 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR601N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    53850 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR647M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    14675 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR656N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    15873 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR716N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    17289 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR782N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18750 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR853N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    61170 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR914M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19635 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR931N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1264 2023-05-05 10:39:56.000000 hostphot-2.6.2/src/hostphot/filters/HST/IR_err.txt
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 03:15:08.040765 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9747 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F090M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2486 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F095N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2874 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F097N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3264 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F108N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12445 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24500 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3077 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F113N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    33411 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F140W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13978 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F145M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21021 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F160W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4877 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F164N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11680 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F165M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5199 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F166N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12148 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F170M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6879 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F187N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7831 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F190N.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 03:15:08.040765 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24275 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F110W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20849 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F160W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12018 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F165M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18588 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F171M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    17947 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F180M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6506 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    41358 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5506 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F190N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21662 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F204M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    30947 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F205W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20965 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F207M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11516 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F212N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7894 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F215N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7479 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F216N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    30813 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F222M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26323 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F237M.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 03:15:08.044765 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3240 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F108N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24427 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F110W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3363 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F113N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    35249 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F150W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20994 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F160W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4858 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F164N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4820 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F166N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    43711 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F175W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6876 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F187N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5510 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F190N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7212 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F196N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9291 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F200N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11541 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F212N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7906 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F215N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    30812 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F222M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13019 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F240M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3503 2023-05-05 10:39:56.000000 hostphot-2.6.2/src/hostphot/filters/HST/UVIS1_err.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3503 2023-05-05 10:39:56.000000 hostphot-2.6.2/src/hostphot/filters/HST/UVIS2_err.txt
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 03:15:08.048765 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8959 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F098M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9826 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F105W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21512 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F110W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    22426 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F125W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4121 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F126N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5064 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F127M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6580 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F128N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3261 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F130N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3792 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F132N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5421 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F139M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13977 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F140W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6752 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F153M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    10046 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F160W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4738 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F164N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6887 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F167N.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 03:15:08.060764 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   156254 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F200LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21978 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F218W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    29976 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F225W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21591 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F275W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7558 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F280N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    56436 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F300X.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    15547 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F336W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19356 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F343N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   146819 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F350LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4504 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F373N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9638 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26406 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7035 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F395N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9314 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F410M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18697 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F438W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9833 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F467M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3637 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F469N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    32782 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    72677 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475X.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5098 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F487N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5804 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F502N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    38578 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F547M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    63538 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F555W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    97333 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F600LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    51442 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F606W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21890 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F621M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    34917 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F625W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4204 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F631N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3675 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F645N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2150 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F656N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11299 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F657N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3236 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F658N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11865 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F665N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11991 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F673N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13792 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F680N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20007 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F689M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19898 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F763M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    36590 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F775W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    54378 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F814W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    33733 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F845M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    57316 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F850LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12497 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F953N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13422 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ232N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13900 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ243N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21137 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ378N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6727 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ387N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    39729 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ422M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11393 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ436N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1548 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ437N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    22828 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ492N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26635 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ508N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4658 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ575N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19283 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ619N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20492 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ634N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4687 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ672N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4387 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ674N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24973 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ727N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    25138 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ750N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2950 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ889N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2948 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ906N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3346 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ924N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3461 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ937N.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 03:15:08.072764 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   156503 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F200LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20752 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F218W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    29190 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F225W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21479 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F275W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7566 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F280N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    55542 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F300X.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    15542 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F336W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19332 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F343N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   147032 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F350LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4495 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F373N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9640 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26441 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7031 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F395N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9300 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F410M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18727 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F438W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9871 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F467M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3641 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F469N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    32751 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    72732 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475X.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5104 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F487N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5798 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F502N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    38608 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F547M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    63493 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F555W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    97494 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F600LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    51384 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F606W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21858 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F621M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    34960 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F625W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4209 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F631N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3686 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F645N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2154 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F656N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11309 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F657N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3233 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F658N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11857 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F665N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11991 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F673N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13805 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F680N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20019 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F689M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19919 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F763M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    36600 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F775W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    54473 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F814W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    33739 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F845M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    57507 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F850LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12507 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F953N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13422 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ232N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13900 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ243N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21137 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ378N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6727 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ387N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    39729 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ422M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11393 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ436N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1548 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ437N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    22828 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ492N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26635 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ508N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4658 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ575N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19283 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ619N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20492 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ634N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4687 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ672N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4387 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ674N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24973 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ727N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    25138 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ750N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2950 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ889N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2948 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ906N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3346 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ924N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3461 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ937N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2012 2023-05-05 10:39:56.000000 hostphot-2.6.2/src/hostphot/filters/HST/ir_aper_corrections.csv
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18667 2023-05-05 10:39:56.000000 hostphot-2.6.2/src/hostphot/filters/HST/wfc3uvis1_aper_007_syn.csv
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18635 2023-05-05 10:39:56.000000 hostphot-2.6.2/src/hostphot/filters/HST/wfc3uvis2_aper_007_syn.csv
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 03:15:08.072764 hostphot-2.6.2/src/hostphot/filters/LegacySurvey/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2281 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/filters/LegacySurvey/BASS_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3180 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/filters/LegacySurvey/BASS_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21743 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/filters/LegacySurvey/DECAM_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21744 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/filters/LegacySurvey/DECAM_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21744 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/filters/LegacySurvey/DECAM_z.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7028 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/filters/LegacySurvey/MzLS_z.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      300 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/filters/LegacySurvey/README.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4275 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/filters/LegacySurvey/init_BASS_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5840 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/filters/LegacySurvey/init_BASS_r.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 03:15:08.072764 hostphot-2.6.2/src/hostphot/filters/PS1/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      136 2022-05-31 09:22:42.000000 hostphot-2.6.2/src/hostphot/filters/PS1/AAA_README.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3717 2022-07-28 14:32:41.000000 hostphot-2.6.2/src/hostphot/filters/PS1/PS1_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3759 2022-07-28 14:32:41.000000 hostphot-2.6.2/src/hostphot/filters/PS1/PS1_i.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3885 2022-07-28 14:32:41.000000 hostphot-2.6.2/src/hostphot/filters/PS1/PS1_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4385 2022-07-28 14:32:41.000000 hostphot-2.6.2/src/hostphot/filters/PS1/PS1_y.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3486 2022-07-28 14:32:41.000000 hostphot-2.6.2/src/hostphot/filters/PS1/PS1_z.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 03:15:08.072764 hostphot-2.6.2/src/hostphot/filters/SDSS/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       72 2022-05-31 09:22:42.000000 hostphot-2.6.2/src/hostphot/filters/SDSS/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1414 2022-07-28 14:32:41.000000 hostphot-2.6.2/src/hostphot/filters/SDSS/SDSS_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1260 2022-07-28 14:32:41.000000 hostphot-2.6.2/src/hostphot/filters/SDSS/SDSS_i.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1176 2022-07-28 14:32:41.000000 hostphot-2.6.2/src/hostphot/filters/SDSS/SDSS_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4718 2022-07-28 14:32:41.000000 hostphot-2.6.2/src/hostphot/filters/SDSS/SDSS_u.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2509 2022-07-28 14:32:41.000000 hostphot-2.6.2/src/hostphot/filters/SDSS/SDSS_z.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 03:15:08.076763 hostphot-2.6.2/src/hostphot/filters/Spitzer/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      189 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/filters/Spitzer/README.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8211 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/filters/Spitzer/Spitzer_IRAC.1.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8421 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/filters/Spitzer/Spitzer_IRAC.2.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6531 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/filters/Spitzer/Spitzer_IRAC.3.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7375 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/filters/Spitzer/Spitzer_IRAC.4.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2816 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/filters/Spitzer/Spitzer_MIPS.1.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 03:15:08.076763 hostphot-2.6.2/src/hostphot/filters/VISTA/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       84 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/filters/VISTA/README.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    39168 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/filters/VISTA/VISTA_H.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    50048 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/filters/VISTA/VISTA_J.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    41344 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/filters/VISTA/VISTA_Ks.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    46341 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/filters/VISTA/VISTA_Y.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   176418 2022-11-14 14:06:00.000000 hostphot-2.6.2/src/hostphot/filters/VISTA/VISTA_Z.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 03:15:08.076763 hostphot-2.6.2/src/hostphot/filters/WISE/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.6.2/src/hostphot/filters/WISE/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2961 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/WISE/WISE_W1.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3528 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/WISE/WISE_W2.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24404 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/WISE/WISE_W3.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19734 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/filters/WISE/WISE_W4.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      739 2023-04-24 13:20:08.000000 hostphot-2.6.2/src/hostphot/filters/config.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    22763 2023-05-11 02:29:33.000000 hostphot-2.6.2/src/hostphot/global_photometry.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2488 2023-05-11 02:29:33.000000 hostphot-2.6.2/src/hostphot/image_cleaning.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12653 2023-05-11 02:29:33.000000 hostphot-2.6.2/src/hostphot/image_masking.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12493 2023-04-25 09:34:42.000000 hostphot-2.6.2/src/hostphot/interactive_aperture.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13859 2023-05-11 02:29:33.000000 hostphot-2.6.2/src/hostphot/local_photometry.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9169 2023-05-11 02:29:33.000000 hostphot-2.6.2/src/hostphot/objects_detect.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    10706 2022-08-15 08:03:30.000000 hostphot-2.6.2/src/hostphot/rgb_images.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    30163 2023-05-11 02:29:33.000000 hostphot-2.6.2/src/hostphot/utils.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 03:15:08.028766 hostphot-2.6.2/src/hostphot.egg-info/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9235 2023-05-11 03:15:08.000000 hostphot-2.6.2/src/hostphot.egg-info/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    14942 2023-05-11 03:15:08.000000 hostphot-2.6.2/src/hostphot.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-05-11 03:15:08.000000 hostphot-2.6.2/src/hostphot.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      193 2023-05-11 03:15:08.000000 hostphot-2.6.2/src/hostphot.egg-info/requires.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        9 2023-05-11 03:15:08.000000 hostphot-2.6.2/src/hostphot.egg-info/top_level.txt
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-11 03:15:08.076763 hostphot-2.6.2/tests/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2771 2023-04-25 09:34:42.000000 hostphot-2.6.2/tests/test_cutouts.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1074 2023-05-11 02:29:33.000000 hostphot-2.6.2/tests/test_global_phot.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      460 2022-07-28 14:32:41.000000 hostphot-2.6.2/tests/test_interactivity.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1089 2023-05-11 02:29:33.000000 hostphot-2.6.2/tests/test_local_phot.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1095 2022-07-28 14:32:41.000000 hostphot-2.6.2/tests/test_preprocessing.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      861 2023-05-11 02:29:33.000000 hostphot-2.6.2/tests/test_rgb_images.py
```

### Comparing `hostphot-2.6.1/LICENSE` & `hostphot-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/PKG-INFO` & `hostphot-2.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hostphot
-Version: 2.6.1
+Version: 2.6.2
 Summary: Global and local photometry of galaxies hosting supernovae or other transients
 Home-page: https://github.com/temuller/hostphot
 Author: Tomás Enrique Müller-Bravo and Lluís Galbany
 Author-email: t.e.muller-bravo@ice.csic.es
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -192,14 +192,18 @@
   number = {76}, 
   pages = {4508},  
   journal = {Journal of Open Source Software} 
 } 
 ```
 
 ## What's new!
+v2.6.2
+* Prettier plots (now using `aplpy`), but also more informative!
+* Scale of the apertures for the masks is now a parameter (`r`) 
+* Raise exception is now `True` by default when calculating photometry
 v2.6.1
 * 2MASS cutouts improved (picking largest image)
 v2.6.0:
 * HST (WFC3 only - pseudo-trial) included
 * 2MASS cutouts fixed (it now downloads the image closest to the given coordinates)
 v2.5.1:
 * Using sfdmap2 instead of sfdmap to avoid issues with numpy version (requires Python>=3.9)
```

### Comparing `hostphot-2.6.1/README.md` & `hostphot-2.6.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -177,14 +177,18 @@
   number = {76}, 
   pages = {4508},  
   journal = {Journal of Open Source Software} 
 } 
 ```
 
 ## What's new!
+v2.6.2
+* Prettier plots (now using `aplpy`), but also more informative!
+* Scale of the apertures for the masks is now a parameter (`r`) 
+* Raise exception is now `True` by default when calculating photometry
 v2.6.1
 * 2MASS cutouts improved (picking largest image)
 v2.6.0:
 * HST (WFC3 only - pseudo-trial) included
 * 2MASS cutouts fixed (it now downloads the image closest to the given coordinates)
 v2.5.1:
 * Using sfdmap2 instead of sfdmap to avoid issues with numpy version (requires Python>=3.9)
```

### Comparing `hostphot-2.6.1/setup.py` & `hostphot-2.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/coadd.py` & `hostphot-2.6.2/src/hostphot/coadd.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/cutouts.py` & `hostphot-2.6.2/src/hostphot/cutouts.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import pyvo  # 2MASS
 from pyvo.dal import sia  # DES, DELVE
 from astroquery.sdss import SDSS
 from astroquery.skyview import SkyView  # other surveys
 from astroquery.mast import Observations  # for GALEX
 
 from astroquery.esa.hubble import ESAHubble
+
 esahubble = ESAHubble()
 
 from reproject import reproject_interp
 
 from hostphot._constants import workdir
 from hostphot.utils import (
     get_survey_filters,
@@ -339,23 +340,30 @@
         size_arcsec = size.to(u.arcsec)
 
     pixel_scale = survey_pixel_scale(survey)
     size_pixels = int(size_arcsec.value / pixel_scale)
 
     coords = SkyCoord(ra=ra * u.degree, dec=dec * u.degree)
     for radius in np.arange(1, 60, 1):
-        ids = SDSS.query_region(coords, radius=radius * u.arcsec, data_release=dr)
+        ids = SDSS.query_region(
+            coords, radius=radius * u.arcsec, data_release=dr
+        )
         if ids is not None:
             break
 
     if ids is None:
         return None
 
     # get the pointing closest to the given coordinates
-    coords_imgs = SkyCoord(ra=ids["ra"].value, dec=ids["dec"].value, unit=(u.degree, u.degree), frame="icrs")
+    coords_imgs = SkyCoord(
+        ra=ids["ra"].value,
+        dec=ids["dec"].value,
+        unit=(u.degree, u.degree),
+        frame="icrs",
+    )
     separation = coords.separation(coords_imgs).value
 
     pointing_id = np.argmin(separation)
     ids2remove = list(np.arange(len(separation)))
     del ids2remove[pointing_id]
     ids.remove_rows(ids2remove)
 
@@ -472,15 +480,20 @@
                     pass
 
             # calculate the separation of the galaxy to the image center
             separations = []
             for hdu in hdu_list:
                 ra_img = float(hdu[0].header["RA_CENT"])
                 dec_img = float(hdu[0].header["DEC_CENT"])
-                coords_img = SkyCoord(ra=ra_img, dec=dec_img, unit=(u.degree, u.degree), frame="icrs")
+                coords_img = SkyCoord(
+                    ra=ra_img,
+                    dec=dec_img,
+                    unit=(u.degree, u.degree),
+                    frame="icrs",
+                )
                 separation = coords.separation(coords_img).value
                 separations.append(separation)
 
             # get the image with the galaxy closest to the center
             if len(separations) != 0:
                 id_file = np.argmin(separations)
                 hdu = hdu_list[id_file]
@@ -762,25 +775,28 @@
                 n_zeros = 3 - len(str(scanno))
                 scanno = n_zeros * "0" + str(scanno)
 
                 tile_url = os.path.join(f"{ordate}{hemisphere}", f"s{scanno}")
                 fits_url = os.path.join("image", f"{fname}.gz")
                 params_url = f"center={ra},{dec}&size={size_degree}degree&gzip=0"  # center and size of the image
 
-                url = os.path.join(base_url, tile_url, fits_url + "?" + params_url)
+                url = os.path.join(
+                    base_url, tile_url, fits_url + "?" + params_url
+                )
                 hdu = fits.open(url)
                 ny, nx = hdu[0].data.shape
-                sizes.append(nx*ny)
+                sizes.append(nx * ny)
                 tmp_hdu_list.append(hdu)
 
             i = np.argmax(sizes)
             hdu_list.append(tmp_hdu_list[i])
-            
+
     return hdu_list
 
+
 # Legacy Survey
 def get_LegacySurvey_images(ra, dec, size=3, filters=None, version="dr10"):
     """Gets Legacy Survey fits images for the given coordinates and
     filters.
 
     Parameters
     ----------
@@ -825,15 +841,15 @@
     # assuming order grz of the filters
     for i, filt in enumerate(filters):
         data = master_hdu[0].data[i]
         hdu = fits.PrimaryHDU(data=data, header=header)
         hdu_list.append(hdu)
 
     return hdu_list
-    
+
 
 # Spitzer
 def get_Spitzer_images(ra, dec, size=3, filters=None):
     """Gets Spitzer fits images for the given coordinates and
     filters.
 
     Parameters
@@ -1019,38 +1035,39 @@
     Parameters
     ----------
     hdu : Header Data Unit.
         HST FITS image.
     """
     # get WCS
     with warnings.catch_warnings():
-            warnings.simplefilter("ignore", AstropyWarning)
-            for i in range(1, len(hdu)-1):
-                try:
-                    img_wcs = wcs.WCS(hdu[i].header)
-                except:
-                    continue
+        warnings.simplefilter("ignore", AstropyWarning)
+        for i in range(1, len(hdu) - 1):
+            try:
+                img_wcs = wcs.WCS(hdu[i].header)
+            except:
+                continue
     hdu[0].header.update(img_wcs.to_header())
-    hdu[0].header['PHOTFLAM'] = hdu[1].header['PHOTFLAM']
-    hdu[0].header['PHOTPLAM'] = hdu[1].header['PHOTPLAM']
+    hdu[0].header["PHOTFLAM"] = hdu[1].header["PHOTFLAM"]
+    hdu[0].header["PHOTPLAM"] = hdu[1].header["PHOTPLAM"]
     hdu[0].data = hdu[1].data
 
     # add zeropoints
     # https://www.stsci.edu/hst/instrumentation/acs/data-analysis/zeropoints
     photflam = hdu[0].header["PHOTFLAM"]
     photplam = hdu[0].header["PHOTPLAM"]
     hdu[0].header["MAGZP"] = (
         -2.5 * np.log10(photflam) - 5 * np.log10(photplam) - 2.408
     )
 
+
 def set_HST_image(file, filt, name):
     """Moves a previously downloaded HST image into the work directory.
 
     The image's header is updated with the necessary keywords to obtain
-    photometry and is also moved under the objects directory inside the 
+    photometry and is also moved under the objects directory inside the
     work directory.
 
     HST images take very long to download, so the user might prefer to
     download the images manually and then use this function to include
     the image into the workflow.
 
     Parameters
@@ -1065,17 +1082,18 @@
     check_work_dir(workdir)
     obj_dir = os.path.join(workdir, name)
     if not os.path.isdir(obj_dir):
         os.mkdir(obj_dir)
 
     hdu = fits.open(file)
     update_HST_header(hdu)
-    outfile = os.path.join(obj_dir, f'HST_{filt}.fits')
+    outfile = os.path.join(obj_dir, f"HST_{filt}.fits")
     hdu.writeto(outfile, overwrite=True)
 
+
 def get_HST_images(ra, dec, size=3, filt=None):
     """Downloads a set of HST fits images for a given set
     of coordinates and filters using the MAST archive.
 
     Parameters
     ----------
     ra: str or float
@@ -1094,21 +1112,21 @@
         `None` is returned if no image is found.
     """
     global esahubble
     esahubble.get_status_messages()
     check_HST_filters(filt)
 
     # separate the instrument name from the actual filter
-    split_filt = filt.split('_')
-    if len(split_filt)==2:
+    split_filt = filt.split("_")
+    if len(split_filt) == 2:
         filt = split_filt[-1]
         instrument = split_filt[0]
-    elif len(split_filt)==3:
+    elif len(split_filt) == 3:
         filt = split_filt[-1]
-        instrument = f'{split_filt[0]}/{split_filt[1]}'
+        instrument = f"{split_filt[0]}/{split_filt[1]}"
     else:
         raise ValueError(f"Incorrect filter name: {filt}")
 
     if isinstance(size, (float, int)):
         size_arcsec = (size * u.arcmin).to(u.arcsec)
     else:
         size_arcsec = size.to(u.arcsec)
@@ -1117,81 +1135,89 @@
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", AstropyWarning)
         coords = SkyCoord(
             ra=ra, dec=dec, unit=(u.degree, u.degree), frame="icrs"
         )
 
     version = None
-    if version=='HLA':
+    if version == "HLA":
         # This does not seem to be faster
-        fov = 0.2   # field-of-view win degrees
+        fov = 0.2  # field-of-view win degrees
         access_url = " https://hla.stsci.edu/cgi-bin/hlaSIAP.cgi"
         svc = sia.SIAService(access_url)
         imgs_table = svc.search(
             (ra, dec), (fov / np.cos(dec * np.pi / 180), fov), verbosity=2
         )
 
         obs_df = pd.DataFrame(imgs_table)
-        obs_df = obs_df[obs_df.Mode=='IMAGE']
-        obs_df = obs_df[obs_df.Format.str.endswith('fits')]
-        obs_df = obs_df[obs_df.Detector==instrument]
-        obs_df = obs_df[obs_df.Spectral_Elt==filt]
-        obs_df = obs_df[obs_df.ExpTime==obs_df.ExpTime.max()]
-        
+        obs_df = obs_df[obs_df.Mode == "IMAGE"]
+        obs_df = obs_df[obs_df.Format.str.endswith("fits")]
+        obs_df = obs_df[obs_df.Detector == instrument]
+        obs_df = obs_df[obs_df.Spectral_Elt == filt]
+        obs_df = obs_df[obs_df.ExpTime == obs_df.ExpTime.max()]
+
         hdu = fits.open(obs_df.URL.values[0])
     else:
-        result = esahubble.cone_search_criteria(radius=3,
-                                                coordinates=coords,
-                                                calibration_level='PRODUCT',
-                                                data_product_type = 'image',
-                                                instrument_name = instrument,
-                                                filters = filt,
-                                                async_job = True,
-                                            )
-        
+        result = esahubble.cone_search_criteria(
+            radius=3,
+            coordinates=coords,
+            calibration_level="PRODUCT",
+            data_product_type="image",
+            instrument_name=instrument,
+            filters=filt,
+            async_job=True,
+        )
+
         obs_df = result.to_pandas()
-        obs_df = obs_df[obs_df['filter']==filt]
+        obs_df = obs_df[obs_df["filter"] == filt]
         # get only exposures shorter than one hour
-        obs_df = obs_df[obs_df.exposure_duration<3600]  
-        obs_df.sort_values(by=['exposure_duration'], 
-                        ascending=False, inplace=True) 
+        obs_df = obs_df[obs_df.exposure_duration < 3600]
+        obs_df.sort_values(
+            by=["exposure_duration"], ascending=False, inplace=True
+        )
 
-        print('Looking for HST images...')
-        filename = f'HST_tmp_{ra}_{dec}'  # the extension is added below
+        print("Looking for HST images...")
+        filename = f"HST_tmp_{ra}_{dec}"  # the extension is added below
         for obs_id in obs_df.observation_id:
             try:
-                esahubble.download_product(observation_id=obs_id, 
-                                        product_type="SCIENCE", 
-                                        calibration_level="PRODUCT", 
-                                        filename=filename)
+                esahubble.download_product(
+                    observation_id=obs_id,
+                    product_type="SCIENCE",
+                    calibration_level="PRODUCT",
+                    filename=filename,
+                )
                 break
             except:
                 pass
 
-        temp_file = f'{filename}.fits.gz'
+        temp_file = f"{filename}.fits.gz"
         if os.path.isfile(temp_file) is False:
             return None
-        
-        temp_dir = filename # same name as the extension-less file above
-        with zipfile.ZipFile(temp_file, 'r') as zip_ref:
+
+        temp_dir = filename  # same name as the extension-less file above
+        with zipfile.ZipFile(temp_file, "r") as zip_ref:
             zip_ref.extractall(temp_dir)
-            fits_file = [file for file in glob.glob(f'{temp_dir}/**', recursive=True) 
-                        if file.endswith('.gz')][0]
+            fits_file = [
+                file
+                for file in glob.glob(f"{temp_dir}/**", recursive=True)
+                if file.endswith(".gz")
+            ][0]
 
-        hdu = fits.open(fits_file)    
+        hdu = fits.open(fits_file)
 
         # remove the temporary files and directory
-        os.remove(temp_file) 
+        os.remove(temp_file)
         shutil.rmtree(temp_dir, ignore_errors=True)
 
     update_HST_header(hdu)
     hdu_list = [hdu]
-    
+
     return hdu_list
 
+
 def get_HST_images_OLD(ra, dec, size=3, filt=None, instrument=None):
     """Downloads a set of HST fits images for a given set
     of coordinates and filters using the MAST archive.
 
     Parameters
     ----------
     ra: str or float
@@ -1275,15 +1301,15 @@
     )
     hdu_list = [hdu]
 
     # remove directory created by MAST download
     shutil.rmtree("mastDownload", ignore_errors=True)
 
     # HST images can be large so need to be trimmed
-    pixel_scale = survey_pixel_scale('HST')
+    pixel_scale = survey_pixel_scale("HST")
     size_pixels = int(size_arcsec / pixel_scale)
     pos = SkyCoord(ra=ra * u.degree, dec=dec * u.degree)
 
     for hdu in hdu_list:
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", AstropyWarning)
             img_wcs = wcs.WCS(hdu[0].header)
@@ -1404,15 +1430,15 @@
         hdu_list = get_Spitzer_images(ra, dec, size, filters)
     elif survey == "VISTA":
         hdu_list = get_VISTA_images(ra, dec, size, filters, version)
     else:
         raise ValueError(
             "The given survey is not properly added to HostPhot..."
         )
-    
+
     if filters is None:
         filters = get_survey_filters(survey)
 
     if hdu_list:
         for hdu, filt in zip(hdu_list, filters):
             if hdu is None:
                 continue  # skip missing filter/image
```

### Comparing `hostphot-2.6.1/src/hostphot/dust.py` & `hostphot-2.6.2/src/hostphot/dust.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/2MASS/2MASS_H.dat` & `hostphot-2.6.2/src/hostphot/filters/2MASS/2MASS_H.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/2MASS/2MASS_J.dat` & `hostphot-2.6.2/src/hostphot/filters/2MASS/2MASS_J.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/2MASS/2MASS_Ks.dat` & `hostphot-2.6.2/src/hostphot/filters/2MASS/2MASS_Ks.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/AAA_README` & `hostphot-2.6.2/src/hostphot/filters/AAA_README`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/DES/DES_Y.dat` & `hostphot-2.6.2/src/hostphot/filters/DES/DES_Y.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/DES/DES_g.dat` & `hostphot-2.6.2/src/hostphot/filters/DES/DES_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/DES/DES_i.dat` & `hostphot-2.6.2/src/hostphot/filters/DES/DES_i.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/DES/DES_r.dat` & `hostphot-2.6.2/src/hostphot/filters/DES/DES_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/DES/DES_z.dat` & `hostphot-2.6.2/src/hostphot/filters/DES/DES_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/GALEX/GALEX_FUV.dat` & `hostphot-2.6.2/src/hostphot/filters/GALEX/GALEX_FUV.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/GALEX/GALEX_NUV.dat` & `hostphot-2.6.2/src/hostphot/filters/GALEX/GALEX_NUV.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F435W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F435W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F475W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F475W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F502N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F502N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F550M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F550M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F555W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F555W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F606W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F606W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F625W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F625W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F658N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F658N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F660N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F660N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F775W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F775W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F814W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F814W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F850LP.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F850LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F892N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F892N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR1016N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR1016N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR388N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR388N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR423N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR423N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR459M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR459M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR462N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR462N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR505N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR505N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR551N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR551N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR601N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR601N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR647M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR647M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR656N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR656N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR716N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR716N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR782N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR782N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR853N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR853N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR914M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR914M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR931N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR931N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/IR_err.txt` & `hostphot-2.6.2/src/hostphot/filters/HST/IR_err.txt`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F090M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F090M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F095N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F095N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F097N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F097N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F108N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F108N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F113N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F113N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F140W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F140W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F145M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F145M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F160W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F160W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F164N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F164N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F165M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F165M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F166N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F166N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F170M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F170M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F187N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F187N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F190N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS1/NICMOS1_F190N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F110W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F110W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F160W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F160W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F165M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F165M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F171M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F171M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F180M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F180M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F190N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F190N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F204M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F204M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F205W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F205W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F207M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F207M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F212N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F212N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F215N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F215N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F216N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F216N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F222M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F222M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F237M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS2/NICMOS2_F237M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F108N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F108N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F110W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F110W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F113N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F113N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F150W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F150W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F160W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F160W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F164N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F164N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F166N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F166N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F175W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F175W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F187N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F187N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F190N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F190N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F196N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F196N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F200N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F200N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F212N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F212N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F215N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F215N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F222M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F222M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F240M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/NICMOS3/NICMOS3_F240M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/UVIS1_err.txt` & `hostphot-2.6.2/src/hostphot/filters/HST/UVIS1_err.txt`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/UVIS2_err.txt` & `hostphot-2.6.2/src/hostphot/filters/HST/UVIS2_err.txt`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F098M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F098M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F105W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F105W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F110W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F110W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F125W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F125W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F126N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F126N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F127M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F127M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F128N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F128N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F130N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F130N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F132N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F132N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F139M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F139M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F140W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F140W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F153M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F153M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F160W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F160W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F164N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F164N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F167N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F167N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F200LP.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F200LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F218W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F218W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F225W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F225W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F275W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F275W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F280N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F280N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F300X.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F300X.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F336W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F336W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F343N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F343N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F350LP.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F350LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F373N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F373N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F395N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F395N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F410M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F410M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F438W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F438W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F467M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F467M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F469N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F469N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475X.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475X.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F487N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F487N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F502N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F502N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F547M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F547M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F555W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F555W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F600LP.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F600LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F606W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F606W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F621M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F621M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F625W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F625W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F631N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F631N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F645N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F645N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F656N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F656N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F657N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F657N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F658N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F658N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F665N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F665N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F673N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F673N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F680N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F680N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F689M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F689M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F763M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F763M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F775W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F775W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F814W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F814W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F845M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F845M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F850LP.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F850LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F953N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F953N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ232N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ232N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ243N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ243N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ378N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ378N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ387N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ387N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ422M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ422M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ436N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ436N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ437N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ437N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ492N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ492N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ508N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ508N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ575N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ575N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ619N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ619N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ634N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ634N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ672N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ672N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ674N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ674N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ727N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ727N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ750N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ750N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ889N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ889N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ906N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ906N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ924N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ924N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ937N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ937N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F200LP.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F200LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F218W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F218W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F225W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F225W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F275W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F275W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F280N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F280N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F300X.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F300X.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F336W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F336W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F343N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F343N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F350LP.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F350LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F373N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F373N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F395N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F395N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F410M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F410M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F438W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F438W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F467M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F467M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F469N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F469N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475X.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475X.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F487N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F487N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F502N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F502N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F547M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F547M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F555W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F555W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F600LP.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F600LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F606W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F606W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F621M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F621M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F625W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F625W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F631N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F631N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F645N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F645N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F656N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F656N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F657N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F657N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F658N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F658N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F665N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F665N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F673N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F673N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F680N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F680N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F689M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F689M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F763M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F763M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F775W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F775W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F814W.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F814W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F845M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F845M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F850LP.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F850LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F953N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F953N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ232N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ232N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ243N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ243N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ378N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ378N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ387N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ387N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ422M.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ422M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ436N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ436N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ437N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ437N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ492N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ492N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ508N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ508N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ575N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ575N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ619N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ619N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ634N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ634N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ672N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ672N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ674N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ674N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ727N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ727N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ750N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ750N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ889N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ889N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ906N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ906N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ924N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ924N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ937N.dat` & `hostphot-2.6.2/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ937N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/ir_aper_corrections.csv` & `hostphot-2.6.2/src/hostphot/filters/HST/ir_aper_corrections.csv`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/wfc3uvis1_aper_007_syn.csv` & `hostphot-2.6.2/src/hostphot/filters/HST/wfc3uvis1_aper_007_syn.csv`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/HST/wfc3uvis2_aper_007_syn.csv` & `hostphot-2.6.2/src/hostphot/filters/HST/wfc3uvis2_aper_007_syn.csv`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/LegacySurvey/BASS_g.dat` & `hostphot-2.6.2/src/hostphot/filters/LegacySurvey/BASS_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/LegacySurvey/BASS_r.dat` & `hostphot-2.6.2/src/hostphot/filters/LegacySurvey/BASS_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/LegacySurvey/DECAM_g.dat` & `hostphot-2.6.2/src/hostphot/filters/LegacySurvey/DECAM_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/LegacySurvey/DECAM_r.dat` & `hostphot-2.6.2/src/hostphot/filters/LegacySurvey/DECAM_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/LegacySurvey/DECAM_z.dat` & `hostphot-2.6.2/src/hostphot/filters/LegacySurvey/DECAM_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/LegacySurvey/MzLS_z.dat` & `hostphot-2.6.2/src/hostphot/filters/LegacySurvey/MzLS_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/LegacySurvey/init_BASS_g.dat` & `hostphot-2.6.2/src/hostphot/filters/LegacySurvey/init_BASS_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/LegacySurvey/init_BASS_r.dat` & `hostphot-2.6.2/src/hostphot/filters/LegacySurvey/init_BASS_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/PS1/PS1_g.dat` & `hostphot-2.6.2/src/hostphot/filters/PS1/PS1_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/PS1/PS1_i.dat` & `hostphot-2.6.2/src/hostphot/filters/PS1/PS1_i.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/PS1/PS1_r.dat` & `hostphot-2.6.2/src/hostphot/filters/PS1/PS1_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/PS1/PS1_y.dat` & `hostphot-2.6.2/src/hostphot/filters/PS1/PS1_y.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/PS1/PS1_z.dat` & `hostphot-2.6.2/src/hostphot/filters/PS1/PS1_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/SDSS/SDSS_g.dat` & `hostphot-2.6.2/src/hostphot/filters/SDSS/SDSS_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/SDSS/SDSS_i.dat` & `hostphot-2.6.2/src/hostphot/filters/SDSS/SDSS_i.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/SDSS/SDSS_r.dat` & `hostphot-2.6.2/src/hostphot/filters/SDSS/SDSS_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/SDSS/SDSS_u.dat` & `hostphot-2.6.2/src/hostphot/filters/SDSS/SDSS_u.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/SDSS/SDSS_z.dat` & `hostphot-2.6.2/src/hostphot/filters/SDSS/SDSS_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.1.dat` & `hostphot-2.6.2/src/hostphot/filters/Spitzer/Spitzer_IRAC.1.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.2.dat` & `hostphot-2.6.2/src/hostphot/filters/Spitzer/Spitzer_IRAC.2.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.3.dat` & `hostphot-2.6.2/src/hostphot/filters/Spitzer/Spitzer_IRAC.3.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.4.dat` & `hostphot-2.6.2/src/hostphot/filters/Spitzer/Spitzer_IRAC.4.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/Spitzer/Spitzer_MIPS.1.dat` & `hostphot-2.6.2/src/hostphot/filters/Spitzer/Spitzer_MIPS.1.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/VISTA/VISTA_H.dat` & `hostphot-2.6.2/src/hostphot/filters/VISTA/VISTA_H.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/VISTA/VISTA_J.dat` & `hostphot-2.6.2/src/hostphot/filters/VISTA/VISTA_J.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/VISTA/VISTA_Ks.dat` & `hostphot-2.6.2/src/hostphot/filters/VISTA/VISTA_Ks.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/VISTA/VISTA_Y.dat` & `hostphot-2.6.2/src/hostphot/filters/VISTA/VISTA_Y.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/VISTA/VISTA_Z.dat` & `hostphot-2.6.2/src/hostphot/filters/VISTA/VISTA_Z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/WISE/WISE_W1.dat` & `hostphot-2.6.2/src/hostphot/filters/WISE/WISE_W1.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/WISE/WISE_W2.dat` & `hostphot-2.6.2/src/hostphot/filters/WISE/WISE_W2.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/WISE/WISE_W3.dat` & `hostphot-2.6.2/src/hostphot/filters/WISE/WISE_W3.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/WISE/WISE_W4.dat` & `hostphot-2.6.2/src/hostphot/filters/WISE/WISE_W4.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/filters/config.txt` & `hostphot-2.6.2/src/hostphot/filters/config.txt`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/global_photometry.py` & `hostphot-2.6.2/src/hostphot/global_photometry.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,46 +66,32 @@
     Returns
     -------
     flux: array
         Kron flux.
     flux_err: array
         Kron flux error.
     """
-    r_min = 1.75  # minimum diameter = 3.5
-
-    if kronrad * np.sqrt(objects["a"] * objects["b"]) < r_min:
-        print(f"Warning: using circular photometry")
-        flux, flux_err, _ = sep.sum_circle(
-            data,
-            objects["x"],
-            objects["y"],
-            r_min,
-            err=err,
-            subpix=5,
-            gain=1.0,
-        )
-    else:
-        # theta must be in the range [-pi/2, pi/2] for sep.sum_ellipse()
-        if objects["theta"] > np.pi / 2:
-            objects["theta"] -= np.pi
-        elif objects["theta"] < -np.pi / 2:
-            objects["theta"] += np.pi
-
-        flux, flux_err, _ = sep.sum_ellipse(
-            data,
-            objects["x"],
-            objects["y"],
-            objects["a"],
-            objects["b"],
-            objects["theta"],
-            scale * kronrad,
-            err=err,
-            subpix=5,
-            gain=gain,
-        )
+    # theta must be in the range [-pi/2, pi/2] for sep.sum_ellipse()
+    if objects["theta"] > np.pi / 2:
+        objects["theta"] -= np.pi
+    elif objects["theta"] < -np.pi / 2:
+        objects["theta"] += np.pi
+
+    flux, flux_err, _ = sep.sum_ellipse(
+        data,
+        objects["x"],
+        objects["y"],
+        objects["a"],
+        objects["b"],
+        objects["theta"],
+        scale * kronrad,
+        err=err,
+        subpix=5,
+        gain=gain,
+    )
 
     return flux, flux_err
 
 
 def optimize_kron_flux(data, err, gain, objects, eps=0.0001):
     """Optimizes the Kron flux by iteration over different values.
     The stop condition is met when the change in flux is less that ``eps``.
@@ -260,19 +246,19 @@
         suffix = "masked_"
     else:
         suffix = ""
     if isinstance(filt, list):
         filt = "".join(f for f in filt)
     fits_file = os.path.join(obj_dir, f"{suffix}{survey}_{filt}.fits")
 
-    img = fits.open(fits_file)
-    img = remove_nan(img)
+    hdu = fits.open(fits_file)
+    hdu = remove_nan(hdu)
 
-    header = img[0].header
-    data = img[0].data
+    header = hdu[0].header
+    data = hdu[0].data
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", AstropyWarning)
         img_wcs = wcs.WCS(header, naxis=2)
 
     data = data.astype(np.float64)
     bkg = sep.Background(data)
     bkg_rms = bkg.globalrms
@@ -305,16 +291,25 @@
             gal_obj["b"],
             gal_obj["theta"],
             6.0,
         )
 
     if save_plots is True:
         outfile = os.path.join(obj_dir, f"global_{survey}_{filt}.jpg")
+        title = f"{name}: {survey}-${filt}$"
         plot_detected_objects(
-            data_sub, gal_obj, scale * kronrad, img_wcs, ra, dec, outfile
+            hdu,
+            gal_obj,
+            scale * kronrad,
+            ra,
+            dec,
+            host_ra,
+            host_dec,
+            title,
+            outfile,
         )
 
     if survey == "DES":
         flip = True
     else:
         flip = False
 
@@ -416,19 +411,19 @@
     obj_dir = os.path.join(workdir, name)
     if use_mask:
         suffix = "masked_"
     else:
         suffix = ""
     fits_file = os.path.join(obj_dir, f"{suffix}{survey}_{filt}.fits")
 
-    img = fits.open(fits_file)
-    img = remove_nan(img)
+    hdu = fits.open(fits_file)
+    hdu = remove_nan(hdu)
 
-    header = img[0].header
-    data = img[0].data
+    header = hdu[0].header
+    data = hdu[0].data
     gain = get_image_gain(header, survey)
 
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", AstropyWarning)
         img_wcs = wcs.WCS(header, naxis=2)
 
     data = data.astype(np.float64)
@@ -508,16 +503,25 @@
 
     if correct_extinction is True:
         A_ext = calc_extinction(filt, survey, host_ra, host_dec)
         mag -= A_ext
 
     if save_plots is True:
         outfile = os.path.join(obj_dir, f"global_{survey}_{filt}.jpg")
+        title = f"{name}: {survey}-${filt}$"
         plot_detected_objects(
-            data_sub, gal_obj, scale * kronrad, img_wcs, ra, dec, outfile
+            hdu,
+            gal_obj,
+            scale * kronrad,
+            ra,
+            dec,
+            host_ra,
+            host_dec,
+            title,
+            outfile,
         )
 
     return mag, mag_err, flux, flux_err
 
 
 def multi_band_phot(
     name,
@@ -535,15 +539,15 @@
     common_aperture=True,
     coadd_filters="riz",
     optimize_kronrad=True,
     eps=0.0001,
     gal_dist_thresh=-1,
     save_plots=True,
     save_results=True,
-    raise_exception=False,
+    raise_exception=True,
 ):
     """Calculates multi-band aperture photometry of the host galaxy
     for an object.
 
     Parameters
     ----------
     name: str
@@ -595,15 +599,15 @@
         the galaxy is considered as not found and a warning is printed. If a non-positive value
         is given, the threshold is considered as infinite, i.e. the closest detected object is
         considered as the galaxy (default option).
     save_plots: bool, default ``True``
         If ``True``, the mask and galaxy aperture figures are saved.
     save_results: bool, default ``True``
         If ``True``, the magnitudes are saved into a csv file.
-    raise_exception: bool, default ``False``
+    raise_exception: bool, default ``True``
         If ``True``, an exception is raised if the photometry fails for any filter.
 
     Returns
     -------
     results_dict: dict
         Dictionary with the object's photometry and other info.
 
@@ -616,20 +620,20 @@
     >>> results = gp.multi_band_phot(name, host_ra, host_dec,
                             survey=survey, ra=ra, dec=dec,
                             use_mask=True, common_aperture=True,
                             coadd_filters='riz', save_plots=True)
     """
     check_survey_validity(survey)
     if filters is None:
-        if survey=='HST':
+        if survey == "HST":
             raise ValueError("For HST, the filter needs to be specified!")
         filters = get_survey_filters(survey)
     else:
         check_filters_validity(filters, survey)
-    if survey=='HST':
+    if survey == "HST":
         filters = [filters]
 
     results_dict = {
         "name": name,
         "host_ra": host_ra,
         "host_dec": host_dec,
         "survey": survey,
```

### Comparing `hostphot-2.6.1/src/hostphot/image_cleaning.py` & `hostphot-2.6.2/src/hostphot/image_cleaning.py`

 * *Files 15% similar despite different names*

```diff
@@ -39,30 +39,30 @@
         header["COMMENT"] = "= Trimmed fits file (hostphot)"
         fits_file[0].header = header
         trimmed_fits_files.append(fits_file)
 
     return trimmed_fits_files
 
 
-def remove_nan(image):
+def remove_nan(hdu):
     """Remove columns and/or rows which have all NaN values.
     The WCS is updated accordingly.
 
     Parameters
     ----------
-    image: fits image
+    image: Header Data Unit
         Fits image with header and data.
 
     Returns
     -------
-    trimmed_image: fits image
+    trimmed_hdu: Header Data Unit
         Trimmed image.
     """
-    header = image[0].header
-    data = image[0].data
+    header = hdu[0].header
+    data = hdu[0].data
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", AstropyWarning)
         img_wcs = wcs.WCS(header, naxis=2)
 
     mask = ~np.all(np.isnan(data), axis=0)
     x_size = np.sum(np.ones_like(data[0])[mask])
     x_pos = np.median(np.arange(data.shape[1])[mask])
@@ -78,12 +78,12 @@
         (y_size, x_size),  # has to be (ny, nx)
         wcs=img_wcs,
         copy=True,
     )
     header.update(trimmed_data.wcs.to_header())
     header["COMMENT"] = "= Trimmed fits file (hostphot)"
 
-    trimmed_image = image.copy()
-    trimmed_image[0].data = trimmed_data.data
-    trimmed_image[0].header = header
+    trimmed_hdu = hdu.copy()
+    trimmed_hdu[0].data = trimmed_data.data
+    trimmed_hdu[0].header = header
 
-    return trimmed_image
+    return trimmed_hdu
```

### Comparing `hostphot-2.6.1/src/hostphot/image_masking.py` & `hostphot-2.6.2/src/hostphot/image_masking.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import os
 import pickle
 import numpy as np
+from copy import deepcopy
 import matplotlib.pyplot as plt
 from matplotlib.patches import Ellipse
+import aplpy
+
+font = "GFS Artemisia"
+plt.rcParams["mathtext.fontset"] = "cm"
 
 import sep
 from astropy.io import fits
-from astropy import wcs, units as u
-from astropy.coordinates import SkyCoord, concatenate
+from astropy import wcs
+from astropy.coordinates import concatenate
 from astropy.convolution import (
     Gaussian2DKernel,
     convolve_fft,
     interpolate_replace_nans,
 )
 
 from hostphot._constants import workdir
@@ -20,37 +25,35 @@
     extract_objects,
     find_gaia_objects,
     find_catalog_objects,
     cross_match,
 )
 from hostphot.utils import (
     check_survey_validity,
-    pixel2pixel,
-    update_axislabels,
-    survey_pixel_scale,
     bkg_surveys,
     adapt_aperture,
+    suppress_stdout,
 )
 
 import warnings
 from astropy.utils.exceptions import AstropyWarning
 
 
 # ----------------------------------------
-def mask_image(data, objects, r=5, sigma=20):
+def mask_image(data, objects, r=6, sigma=20):
     """Masks objects in an image (2D array) by convolving it with
     a 2D Gaussian kernel.
 
     Parameters
     ----------
     data: ndarray
         Image data.
     objects: array
         Objects extracted with :func:`sep.extract()`.
-    r: float, default ``5``
+    r: float, default ``6``
         Scale of the semi-mayor and semi-minor axes
         of the ellipse of the `objects`.
     sigma: float, default ``20``
         Standard deviation in pixel units of the 2D Gaussian kernel
         used to convolve the image.
 
     Returns
@@ -86,22 +89,23 @@
     filt,
     survey,
     ra=None,
     dec=None,
     bkg_sub=None,
     threshold=15,
     sigma=8,
+    r=6,
     crossmatch=False,
     gal_dist_thresh=-1,
     extract_params=False,
     common_params=None,
     save_plots=True,
     save_mask_params=True,
 ):
-    """Calculates the aperture parameters for common aperture.
+    """Calculates the aperture parameters to mask detected sources.
 
     Parameters
     ----------
     name: str
         Name of the object to find the path of the fits file.
     host_ra: float
         Host-galaxy right ascension in degrees.
@@ -120,14 +124,19 @@
         the images that need it get background subtracted (WISE, 2MASS and
         VISTA).
     threshold: float, default `15`
         Threshold used by :func:`sep.extract()` to extract objects.
     sigma: float, default ``8``
         Standard deviation in pixel units of the 2D Gaussian kernel
         used to convolve the image.
+    r: float, default ``6``
+        Scale of the aperture size for the sources to be masked.
+    crossmatch: bool, default ``False``
+        If ``True``, the detected objects are cross-matched with a
+        Gaia catalog.
     crossmatch: bool, default ``False``
         If ``True``, the detected objects are cross-matched with a
         Gaia catalog.
     gal_dist_thresh: float, default ``-1``.
         Distance in arcsec to crossmatch the galaxy coordinates with a detected object,
         where the object nearest to the galaxy position is considered as the galaxy (within
         the given threshold). If no objects are found within the given distance threshold,
@@ -159,19 +168,19 @@
     """
     check_survey_validity(survey)
     if isinstance(filt, list):
         filt = "".join(f for f in filt)
 
     obj_dir = os.path.join(workdir, name)
     fits_file = os.path.join(obj_dir, f"{survey}_{filt}.fits")
-    img = fits.open(fits_file)
-    img = remove_nan(img)
+    hdu = fits.open(fits_file)
+    hdu = remove_nan(hdu)
 
-    header = img[0].header
-    data = img[0].data
+    header = hdu[0].header
+    data = hdu[0].data
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", AstropyWarning)
         img_wcs = wcs.WCS(header, naxis=2)
 
     data = data.astype(np.float64)
     bkg = sep.Background(data)
     bkg_rms = bkg.globalrms
@@ -212,31 +221,34 @@
             flip_ = False
         else:
             flip_ = True
 
         gal_obj = adapt_aperture(gal_obj, master_img_wcs, img_wcs, flip_)
         nogal_objs = adapt_aperture(nogal_objs, master_img_wcs, img_wcs, flip_)
 
-    masked_data = mask_image(data_sub, nogal_objs, sigma=sigma)
-    img[0].data = masked_data
+    masked_data = mask_image(data_sub, nogal_objs, r=r, sigma=sigma)
+    masked_hdu = deepcopy(hdu)
+    masked_hdu[0].data = masked_data
     outfile = os.path.join(obj_dir, f"masked_{survey}_{filt}.fits")
-    img.writeto(outfile, overwrite=True)
+    masked_hdu.writeto(outfile, overwrite=True)
 
     if save_plots:
         outfile = os.path.join(obj_dir, f"masked_{survey}_{filt}.jpg")
+        title = f"{name}: {survey}-${filt}$"
         plot_masked_image(
-            data_sub,
-            masked_data,
+            hdu,
+            masked_hdu,
             nogal_objs,
-            img_wcs,
             gal_obj,
+            r,
             host_ra,
             host_dec,
             ra,
             dec,
+            title,
             outfile,
         )
 
     if survey == "DES":
         flip = True
     else:
         flip = False
@@ -250,23 +262,24 @@
             pickle.dump(mask_parameters, fp, protocol=4)
 
     if extract_params:
         return gal_obj, nogal_objs, img_wcs, flip
 
 
 def plot_masked_image(
-    data,
-    masked_data,
+    hdu,
+    masked_hdu,
     objects,
-    img_wcs,
     gal_obj=None,
+    r=6,
     host_ra=None,
     host_dec=None,
     ra=None,
     dec=None,
+    title=None,
     outfile=None,
 ):
     """Plots the masked image together with the original image and
     the detected objects.
 
     Parameters
     ----------
@@ -276,134 +289,135 @@
          Masked image data.
     objects: array
         Objects extracted with :func:`sep.extract()`.
     img_wcs: WCS
         Image's WCS.
     gal_obj: array, default ``None``
         Galaxy object.
+    r: float, default ``6``
+        Scale of the aperture size for the masked sources.
     host_ra: float, default ``None``
        Right ascension of the galaxy, in degrees. Used for plotting the position of the galaxy.
     host_dec: float, default ``None``
        Declination of the galaxy, in degrees. Used for plotting the position of the galaxy.
     ra: float, default ``None``
        Right ascension of an object, in degrees. Used for plotting the position of the object.
     dec: float, default ``None``
        Declination of an object, in degrees. Used for plotting the position of the object.
+    title: str, default ``None``
+        Title of the image
     outfile: str, default ``None``
         If given, path where to save the output figure.
     """
-    r = 4  # scale
-    m, s = np.nanmean(data), np.nanstd(data)
-
-    fig = plt.figure(figsize=(24, 10))
-    ax0 = plt.subplot(131, projection=img_wcs)
-    ax1 = plt.subplot(132, projection=img_wcs)
-    ax2 = plt.subplot(133, projection=img_wcs)
-    axes = [ax0, ax1, ax2]
-
-    for ax in axes:
-        update_axislabels(ax)
-        ax.imshow(
-            data,
-            interpolation="nearest",
-            cmap="gray",
-            vmin=m - s,
-            vmax=m + s,
-            origin="lower",
-        )
-    for ax in axes[1:]:
-        ax.coords[1].set_axislabel("")
-        ax.coords[1].set_ticklabel_visible(False)
-
-    for i in range(len(objects)):
-        e = Ellipse(
-            xy=(objects["x"][i], objects["y"][i]),
-            width=2.5 * r * objects["a"][i],
-            height=2.5 * r * objects["b"][i],
-            angle=objects["theta"][i] * 180.0 / np.pi,
-        )
-        e.set_facecolor("none")
-        e.set_edgecolor("red")
-        e.set_linewidth(1.5)
-        ax1.add_artist(e)
-
-    # plot galaxy pseudo-aperture
-    if gal_obj is not None:
-        e = Ellipse(
-            xy=(gal_obj["x"][0], gal_obj["y"][0]),
-            width=2.5 * r * gal_obj["a"][0],
-            height=2.5 * r * gal_obj["b"][0],
-            angle=gal_obj["theta"][0] * 180.0 / np.pi,
-        )
-        e.set_facecolor("none")
-        e.set_edgecolor("red")
-        e.set_linestyle("dotted")
-        e.set_linewidth(3)
-        ax1.add_artist(e)
-
-        ax1.scatter(
-            gal_obj["x"][0],
-            gal_obj["y"][0],
-            marker="x",
-            s=140,
-            c="r",
-            label="Identified galaxy center",
-        )
-
-    ax2.imshow(
-        masked_data,
-        interpolation="nearest",
-        cmap="gray",
-        vmin=m - s,
-        vmax=m + s,
-        origin="lower",
+    figure = plt.figure(figsize=(30, 12))
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore", AstropyWarning)
+        fig1 = aplpy.FITSFigure(hdu, figure=figure, subplot=(1, 3, 1))
+        fig2 = aplpy.FITSFigure(hdu, figure=figure, subplot=(1, 3, 2))
+        fig3 = aplpy.FITSFigure(masked_hdu, figure=figure, subplot=(1, 3, 3))
+
+    fig2.tick_labels.hide_y()
+    fig2.axis_labels.hide_y()
+    fig3.tick_labels.set_yposition("right")
+    fig3.axis_labels.set_yposition("right")
+
+    figures = [fig1, fig2, fig3]
+    titles = ["Initial Image", "Detected Sources", "Masked Image"]
+    for i, fig in enumerate(figures):
+        fig.set_theme("publication")
+        fig.set_title(titles[i], **{"family": font, "size": 24})
+        with suppress_stdout():
+            fig.show_grayscale(stretch="arcsinh")
+
+        # ticks
+        fig.tick_labels.set_font(**{"family": font, "size": 18})
+        fig.tick_labels.set_xformat("dd.dd")
+        fig.tick_labels.set_yformat("dd.dd")
+        fig.ticks.set_length(6)
+
+        fig.axis_labels.set_font(**{"family": font, "size": 18})
+
+    # galaxy markers
+    fig2.show_markers(
+        host_ra,
+        host_dec,
+        edgecolor="k",
+        facecolor="r",
+        alpha=0.7,
+        marker="P",
+        s=200,
+        label="Given galaxy",
+    )
+    fig2.show_markers(
+        gal_obj["x"][0],
+        gal_obj["y"][0],
+        edgecolor="k",
+        facecolor="r",
+        alpha=0.7,
+        marker="X",
+        s=200,
+        label="Identified galaxy",
+        coords_frame="pixel",
+    )
+    # galaxy pseudo-aperture
+    fig2.show_ellipses(
+        gal_obj["x"][0],
+        gal_obj["y"][0],
+        2 * r * gal_obj["a"][0],
+        2 * r * gal_obj["b"][0],
+        gal_obj["theta"][0] * 180.0 / np.pi,
+        coords_frame="pixel",
+        linewidth=3,
+        edgecolor="r",
     )
 
-    ax0.set_title("Initial Image", fontsize=24)
-    ax1.set_title("Detected Objects", fontsize=24)
-    ax2.set_title("Masked Image", fontsize=24)
-
-    # plot SN position
-    if (host_ra is not None) and (host_dec is not None):
-        coord = SkyCoord(
-            ra=host_ra, dec=host_dec, unit=(u.degree, u.degree), frame="icrs"
-        )
-        x, y = img_wcs.world_to_pixel(coord)
-        for ax in axes[1:]:
-            ax.scatter(
-                x,
-                y,
-                marker="P",
-                s=140,
-                c="r",
-                edgecolor="gold",
-                label="Galaxy position",
-            )
+    # other sources markers
+    fig2.show_ellipses(
+        objects["x"],
+        objects["y"],
+        2 * r * objects["a"],
+        2 * r * objects["b"],
+        gal_obj["theta"] * 180.0 / np.pi,
+        coords_frame="pixel",
+        linewidth=2,
+        edgecolor="orangered",
+        linestyle="dotted",
+    )
 
-    # plot SN position
+    # SN marker
     if (ra is not None) and (dec is not None):
-        coord = SkyCoord(
-            ra=ra, dec=dec, unit=(u.degree, u.degree), frame="icrs"
-        )
-        x, y = img_wcs.world_to_pixel(coord)
-        for ax in axes[1:]:
-            ax.scatter(
-                x,
-                y,
+        for fig in figures[1:]:
+            fig.show_markers(
+                ra,
+                dec,
+                edgecolor="k",
+                facecolor="aqua",
                 marker="*",
                 s=200,
-                c="g",
-                edgecolor="gold",
-                label="SN position",
+                label="SN",
             )
 
-    axes[1].legend(ncol=2, fontsize=14)
+    fig2.ax.legend(
+        fancybox=True, framealpha=1, prop={"size": 20, "family": font}
+    )
+
+    # title
+    length = len(title) - 2
+    text = fig1.ax.text(
+        0.022 * length,
+        0.06,
+        title,
+        fontsize=28,
+        horizontalalignment="center",
+        verticalalignment="center",
+        transform=fig1.ax.transAxes,
+        font=font,
+    )
+    text.set_bbox(
+        dict(facecolor="white", edgecolor="white", alpha=0.9, boxstyle="round")
+    )
+
     if outfile:
-        basename = os.path.basename(outfile)
-        title = os.path.splitext(basename)[0]
-        title = "-".join(part for part in title.split("_"))
-        fig.suptitle(title, fontsize=28)
-        plt.tight_layout()
         plt.savefig(outfile, bbox_inches="tight")
-        plt.close(fig)
+        plt.close(figure)
     else:
         plt.show()
```

### Comparing `hostphot-2.6.1/src/hostphot/interactive_aperture.py` & `hostphot-2.6.2/src/hostphot/interactive_aperture.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/local_photometry.py` & `hostphot-2.6.2/src/hostphot/local_photometry.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 #
 # Some parts of this notebook are based on https://github.com/djones1040/PS1_surface_brightness/blob/master/Surface%20Brightness%20Tutorial.ipynb and codes from Lluís Galbany
 
 import os
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
+import aplpy
+
+font = "GFS Artemisia"
+plt.rcParams["mathtext.fontset"] = "cm"
 
 import sep
 from photutils.aperture import aperture_photometry, CircularAperture
 
 from astropy.io import fits
 from astropy import units as u, wcs
 from astropy.cosmology import FlatLambdaCDM
@@ -31,16 +35,16 @@
     get_survey_filters,
     check_survey_validity,
     check_filters_validity,
     calc_sky_unc,
     get_image_exptime,
     survey_pixel_scale,
     check_work_dir,
-    update_axislabels,
     magnitude_calculation,
+    suppress_stdout,
     bkg_surveys,
 )
 from hostphot.image_cleaning import remove_nan
 from hostphot.dust import calc_extinction
 
 import warnings
 from astropy.utils.exceptions import AstropyWarning
@@ -118,61 +122,78 @@
     ap_results = aperture_photometry(data, aperture, error=error)
     raw_flux = ap_results["aperture_sum"][0]
     raw_flux_err = ap_results["aperture_sum_err"][0]
 
     return raw_flux, raw_flux_err
 
 
-def plot_aperture(data, px, py, radius_pix, img_wcs, outfile=None):
+def plot_aperture(hdu, px, py, radius_pix, title, outfile=None):
     """Plots the aperture for the given parameters.
 
     Parameters
     ----------
     data: ndarray
         Data of an image.
     px: float
         X-axis center of the aperture in pixels.
     py: float
         Y-axis center of the aperture in pixels.
     radius_pix: float
         Aperture radius in pixels.
     img_wcs: WCS
         Image's WCS.
+    title: str
+        Title of the figure.
     outfile: str, default ``None``
         If given, path where to save the output figure.
     """
-    m, s = np.nanmean(data), np.nanstd(data)
 
-    fig = plt.figure(figsize=(10, 10))
-    ax = plt.subplot(projection=img_wcs)
-    update_axislabels(ax)
-    ax.scatter(px, py, marker="*", s=140, c="g", edgecolor="gold")
-
-    im = ax.imshow(
-        data,
-        interpolation="nearest",
-        cmap="gray",
-        vmin=m - s,
-        vmax=m + s,
-        origin="lower",
+    figure = plt.figure(figsize=(10, 10))
+    title, label = title.split("|")
+
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore", AstropyWarning)
+        fig = aplpy.FITSFigure(hdu, figure=figure)
+
+    with suppress_stdout():
+        fig.show_grayscale(stretch="arcsinh")
+
+    # plot SN and aperture
+    fig.show_markers(
+        px,
+        py,
+        edgecolor="k",
+        facecolor="aqua",
+        marker="*",
+        s=200,
+        label="SN",
+        coords_frame="pixel",
     )
+    fig.show_circles(
+        px, py, radius_pix, coords_frame="pixel", linewidth=2, edgecolor="r"
+    )
+    fig.show_lines([], [], color="r", lw=3, label=label)  # for the legend only
 
-    circle = plt.Circle(
-        (px, py), radius_pix, color="r", fill=False, linewidth=1.5
+    # ticks
+    fig.tick_labels.set_font(**{"family": font, "size": 18})
+    fig.tick_labels.set_xformat("dd.dd")
+    fig.tick_labels.set_yformat("dd.dd")
+    fig.ticks.set_length(6)
+
+    fig.axis_labels.set_font(**{"family": font, "size": 18})
+
+    fig.set_title(title, **{"family": font, "size": 24})
+    fig.set_theme("publication")
+    fig.ax.legend(
+        fancybox=True, framealpha=1, prop={"size": 20, "family": font}
     )
-    ax.add_patch(circle)
 
     if outfile:
-        basename = os.path.basename(outfile)
-        title = os.path.splitext(basename)[0]
-        title = "-".join(part for part in title.split("_"))
-        fig.suptitle(title, fontsize=28)
-        plt.tight_layout()
         plt.savefig(outfile, bbox_inches="tight")
-        plt.close(fig)
+        plt.close(figure)
     else:
         plt.show()
 
 
 def photometry(
     name,
     ra,
@@ -234,19 +255,19 @@
     obj_dir = os.path.join(workdir, name)
     if use_mask:
         suffix = "masked_"
     else:
         suffix = ""
     fits_file = os.path.join(obj_dir, f"{suffix}{survey}_{filt}.fits")
 
-    img = fits.open(fits_file)
-    img = remove_nan(img)
+    hdu = fits.open(fits_file)
+    hdu = remove_nan(hdu)
 
-    header = img[0].header
-    data = img[0].data
+    header = hdu[0].header
+    data = hdu[0].data
     exptime = get_image_exptime(header, survey)
 
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", AstropyWarning)
         img_wcs = wcs.WCS(header, naxis=2)
 
     data = data.astype(np.float64)
@@ -297,15 +318,16 @@
         fluxes.append(flux)
         fluxes_err.append(flux_err)
 
         if save_plots:
             outfile = os.path.join(
                 obj_dir, f"local_{survey}_{filt}_{ap_radius}kpc.jpg"
             )
-            plot_aperture(data_sub, px, py, radius_pix, img_wcs, outfile)
+            title = f"{name}: {survey}-${filt}$|r$={ap_radius}$ kpc @ $z={z}$"
+            plot_aperture(hdu, px, py, radius_pix, title, outfile)
 
     return mags, mags_err, fluxes, fluxes_err
 
 
 def multi_band_phot(
     name,
     ra,
@@ -315,15 +337,15 @@
     survey="PS1",
     ap_radii=1,
     bkg_sub=None,
     use_mask=True,
     correct_extinction=True,
     save_plots=True,
     save_results=True,
-    raise_exception=False,
+    raise_exception=True,
 ):
     """Calculates the local aperture photometry for multiple filters.
 
     Parameters
     ----------
     name: str
         Name of the object to find the path of the fits file.
@@ -351,15 +373,15 @@
     correct_extinction: bool, default `True`
         If `True`, corrects for Milky-Way extinction using the recalibrated dust maps
         by Schlafly & Finkbeiner (2011) and the extinction law from Fitzpatrick (1999).
     save_plots: bool, default ``True``
         If ``True``, the figure with the aperture is saved.
     save_results: bool, default ``True``
         If ``True``, the magnitudes are saved into a csv file.
-    raise_exception: bool, default ``False``
+    raise_exception: bool, default ``True``
         If ``True``, an exception is raised if the photometry fails for any filter.
 
     Returns
     -------
     results_dict: dict
         Dictionary with the object's photometry and other info.
 
@@ -372,34 +394,34 @@
     >>> survey = 'PS1'
     >>> results = lp.multi_band_phot(name, ra, dec, z,
                             survey=survey, ap_radii=ap_radii,
                             use_mask=True, save_plots=True)
     """
     check_survey_validity(survey)
     if filters is None:
-        if survey=='HST':
+        if survey == "HST":
             raise ValueError("For HST, the filter needs to be specified!")
         filters = get_survey_filters(survey)
     else:
         check_filters_validity(filters, survey)
-    if survey=='HST':
+    if survey == "HST":
         filters = [filters]
 
     # turn float into a list
     if isinstance(ap_radii, (float, int)):
         ap_radii = [ap_radii]
 
     results_dict = {
         "name": name,
         "ra": ra,
         "dec": dec,
         "redshift": z,
         "survey": survey,
     }
-    
+
     for filt in filters:
         try:
             mags, mags_err, fluxes, fluxes_err = photometry(
                 name,
                 ra,
                 dec,
                 z,
```

### Comparing `hostphot-2.6.1/src/hostphot/objects_detect.py` & `hostphot-2.6.2/src/hostphot/objects_detect.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 import os
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.patches import Ellipse
+import aplpy
+
+font = "GFS Artemisia"
+plt.rcParams["mathtext.fontset"] = "cm"
 
 import sep
 from astroquery.gaia import Gaia
 from astroquery.mast import Catalogs
 from astropy import units as u
 from astropy.coordinates import SkyCoord
 
-from hostphot.utils import update_axislabels
+from hostphot.utils import suppress_stdout
+
+import warnings
+from astropy.utils.exceptions import AstropyWarning
 
 
 def extract_objects(
-    data, err, host_ra, host_dec, threshold, img_wcs, dist_thresh=-1
+    data, bkg, host_ra, host_dec, threshold, img_wcs, dist_thresh=-1
 ):
     """Extracts objects and their ellipse parameters. The function :func:`sep.extract()`
     is used.
 
     If there is no detected object within a distance of ``dist_thresh`` from the galaxy
     coordinates, it means that the galaxy was not correctly identified.
 
     Parameters
     ----------
     data: ndarray
         Image data.
-    err: 2D array
-        Background error of the image.
+    bkg: 2D array
+        Background level of the image.
     host_ra: float
         Host-galaxy Right ascension of the galaxy in degrees.
     host_dec: float
         Host-galaxy Declination of the galaxy in degrees.
     threshold: float
         Source with flux above ``threshold*bkg_rms`` are extracted.
         See :func:`sep.extract()` for more information.
@@ -51,23 +58,22 @@
     -------
     gal_obj: numpy array
         Galaxy object extracted.
     nogal_objs: numpy array
         All objects extracted except for the galaxy.
     """
     # extract objects with Source Extractor
-    objects = sep.extract(data, threshold, err=err)
+    objects = sep.extract(data, threshold, err=bkg)
 
+    host_coords = SkyCoord(
+        ra=host_ra, dec=host_dec, unit=(u.degree, u.degree), frame="icrs"
+    )
     objs_coords = img_wcs.pixel_to_world(objects["x"], objects["y"])
-    objs_ra, objs_dec = objs_coords.ra.value, objs_coords.dec.value
-    dist = np.sqrt(
-        (objs_ra - host_ra) ** 2 * (np.cos(host_dec * np.pi / 180) ** 2)
-        + (objs_dec - host_dec) ** 2
-    )  # in degrees
-    dist_arcsec = dist * 3600
+    distances = host_coords.separation(objs_coords).to(u.arcsec)
+    dist_arcsec = distances.value
 
     if dist_thresh <= 0.0:
         dist_thresh = np.inf
 
     if any(dist_arcsec <= dist_thresh):
         gal_id = np.argmin(dist_arcsec)
         gal_obj = objects[gal_id : gal_id + 1]
@@ -102,17 +108,18 @@
     """
     Gaia.MAIN_GAIA_TABLE = "gaiaedr3.gaia_source"
     Gaia.ROW_LIMIT = -1
     coord = SkyCoord(ra=ra, dec=dec, unit=(u.degree, u.degree), frame="icrs")
     width = u.Quantity(rad, u.deg)
     height = u.Quantity(rad, u.deg)
     try:
-        gaia_cat = Gaia.query_object_async(
-            coordinate=coord, width=width, height=height
-        )
+        with suppress_stdout():
+            gaia_cat = Gaia.query_object_async(
+                coordinate=coord, width=width, height=height
+            )
     except Exception as exc:
         print(exc)
         print("No objects found with Gaia DR3, switching to DR2")
         Gaia.MAIN_GAIA_TABLE = "gaiadr2.gaia_source"
         gaia_cat = Gaia.query_object_async(
             coordinate=coord, width=width, height=height
         )
@@ -195,15 +202,23 @@
 
     objs = objects.take(objs_id)
 
     return objs
 
 
 def plot_detected_objects(
-    data, objects, scale, img_wcs, ra=None, dec=None, outfile=None
+    hdu,
+    objects,
+    scale,
+    ra=None,
+    dec=None,
+    host_ra=None,
+    host_dec=None,
+    title=None,
+    outfile=None,
 ):
     """Plots the objects extracted with :func:`sep.extract()``.
 
     Parameters
     ----------
     data: ndarray
         Data of an image.
@@ -213,55 +228,78 @@
         Scale of the ellipse's semi-mayor and semi-minor axes.
     img_wcs: WCS
         Image's WCS.
     ra: float, default ``None``
        Right ascension of an object, in degrees. Used for plotting the position of the object.
     dec: float, default ``None``
        Declination of an object, in degrees. Used for plotting the position of the object.
+    host_ra: float, default ``None``
+       Right ascension of a galaxy.
+    host_dec: float, default ``None``
+       Declination of a galaxy.
+    title: str, default ``None``
+        Title of the image.
     outfile: str, default ``None``
         If given, path where to save the output figure.
     """
-    m, s = np.nanmean(data), np.nanstd(data)
+    figure = plt.figure(figsize=(10, 10))
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore", AstropyWarning)
+        fig = aplpy.FITSFigure(hdu, figure=figure)
 
-    fig = plt.figure(figsize=(10, 10))
-    ax = plt.subplot(projection=img_wcs)
-    update_axislabels(ax)
-
-    im = ax.imshow(
-        data,
-        interpolation="nearest",
-        cmap="gray",
-        vmin=m - s,
-        vmax=m + s,
-        origin="lower",
-    )
+    with suppress_stdout():
+        fig.show_grayscale(stretch="arcsinh")
 
-    e = Ellipse(
-        xy=(objects["x"][0], objects["y"][0]),
-        width=2 * scale * objects["a"][0],
-        height=2 * scale * objects["b"][0],
-        angle=objects["theta"][0] * 180.0 / np.pi,
-    )
-
-    e.set_facecolor("none")
-    e.set_edgecolor("red")
-    e.set_linewidth(1.5)
-    ax.add_artist(e)
-
-    # plot SN position
+    # plot SN marker
     if (ra is not None) and (dec is not None):
-        coord = SkyCoord(
-            ra=ra, dec=dec, unit=(u.degree, u.degree), frame="icrs"
+        fig.show_markers(
+            ra,
+            dec,
+            edgecolor="k",
+            facecolor="aqua",
+            marker="*",
+            s=200,
+            label="SN",
+        )
+
+    # plot galaxy marker and aperture
+    if (host_ra is not None) and (host_dec is not None):
+        fig.show_markers(
+            host_ra,
+            host_dec,
+            edgecolor="k",
+            facecolor="r",
+            alpha=0.7,
+            marker="P",
+            s=200,
+            label="Galaxy position",
         )
-        px, py = img_wcs.world_to_pixel(coord)
-        ax.scatter(px, py, marker="*", s=200, c="g", edgecolor="gold")
+    fig.show_ellipses(
+        objects["x"][0],
+        objects["y"][0],
+        2 * scale * objects["a"][0],
+        2 * scale * objects["b"][0],
+        objects["theta"][0] * 180.0 / np.pi,
+        coords_frame="pixel",
+        linewidth=3,
+        edgecolor="r",
+    )
+
+    # ticks
+    fig.tick_labels.set_font(**{"family": font, "size": 18})
+    fig.tick_labels.set_xformat("dd.dd")
+    fig.tick_labels.set_yformat("dd.dd")
+    fig.ticks.set_length(6)
+
+    fig.axis_labels.set_font(**{"family": font, "size": 18})
+
+    fig.set_title(title, **{"family": font, "size": 24})
+    fig.set_theme("publication")
+    fig.ax.legend(
+        fancybox=True, framealpha=1, prop={"size": 20, "family": font}
+    )
 
     if outfile:
-        basename = os.path.basename(outfile)
-        title = os.path.splitext(basename)[0]
-        title = "-".join(part for part in title.split("_"))
-        fig.suptitle(title, fontsize=28)
-        plt.tight_layout()
         plt.savefig(outfile, bbox_inches="tight")
-        plt.close(fig)
+        plt.close(figure)
     else:
         plt.show()
```

### Comparing `hostphot-2.6.1/src/hostphot/rgb_images.py` & `hostphot-2.6.2/src/hostphot/rgb_images.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/src/hostphot/utils.py` & `hostphot-2.6.2/src/hostphot/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 import os
+import sys
 import glob
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 
+import aplpy
+from contextlib import contextmanager
+
+font = "GFS Artemisia"
+plt.rcParams["mathtext.fontset"] = "cm"
+
 from astropy import wcs
 from astropy.io import fits
 from astropy.stats import sigma_clipped_stats
 from photutils.utils import calc_total_error
 from photutils.aperture import EllipticalAperture
 
 import warnings
@@ -16,15 +23,16 @@
 import hostphot
 
 hostphot_path = hostphot.__path__[0]
 config_file = os.path.join(hostphot_path, "filters", "config.txt")
 config_df = pd.read_csv(config_file, delim_whitespace=True)
 
 # surveys that need background subtraction
-bkg_surveys = ['2MASS', 'WISE', 'VISTA']
+bkg_surveys = ["2MASS", "WISE", "VISTA"]
+
 
 def calc_sky_unc(image, exptime):
     """Calculates the uncertainty of the image from the
     sky standard deviation, sigma-clipped STD.
 
     Parameters
     ----------
@@ -78,15 +86,15 @@
     Returns
     -------
     filters: str
         Filters for the given survey.
     """
     check_survey_validity(survey)
 
-    if survey=='HST':
+    if survey == "HST":
         # For HST, the filter needs to be specified
         return None
 
     global config_df
     survey_df = config_df[config_df.survey == survey]
     filters = survey_df.filters.values[0]
 
@@ -122,20 +130,20 @@
 
     if zps == "header":
         return zps
 
     if "," in zps:
         zps = zps.split(",")
         zp_dict = {filt: float(zp) for filt, zp in zip(filters, zps)}
-    elif survey=='SDSS':
+    elif survey == "SDSS":
         # SDSS zero-points are not exactly in AB:
         # https://www.sdss4.org/dr12/algorithms/fluxcal/#SDSStoAB
         zp_dict = {filt: float(zps) for filt in filters}
-        zp_dict['u'] -= 0.04
-        zp_dict['z'] += 0.02
+        zp_dict["u"] -= 0.04
+        zp_dict["z"] += 0.02
     else:
         zp_dict = {filt: float(zps) for filt in filters}
 
     return zp_dict
 
 
 def get_image_gain(header, survey):
@@ -178,16 +186,16 @@
             gain *= header["EFCONV"]  # convert DN/s to MJy/sr
         elif header["INSTRUME"] == "MIPS":
             # Table 2.4 of MIPS Instrument Handbook
             gain = 5.0
     elif survey == "VISTA":
         # use median from http://casu.ast.cam.ac.uk/surveys-projects/vista/technical/vista-gain
         gain = 4.19
-    elif survey=='HST':
-        gain = header['CCDGAIN']
+    elif survey == "HST":
+        gain = header["CCDGAIN"]
     else:
         gain = 1.0
 
     return gain
 
 
 def get_image_readnoise(header, survey):
@@ -233,17 +241,17 @@
         elif header["INSTRUME"] == "MIPS":
             # Table 2.4 of MIPS Instrument Handbook
             readnoise = 40.0
     elif survey == "VISTA":
         # very rough average for all filters in
         # http://casu.ast.cam.ac.uk/surveys-projects/vista/technical/vista-gain
         readnoise = 24.0
-    elif survey=='HST':
+    elif survey == "HST":
         # tipically 0.0
-        readnoise = header['PCTERNOI']
+        readnoise = header["PCTERNOI"]
     else:
         readnoise = 0.0
 
     return readnoise
 
 
 def get_image_exptime(header, survey):
@@ -296,45 +304,52 @@
 
     Returns
     -------
     correction: float
         Aperture correction (encircled energy fraction).
     """
     # split instrument and filter
-    filt_split = filt.split('_')
+    filt_split = filt.split("_")
     filt = filt_split[-1]
     instrument = filt_split[-2]
 
-    if instrument=='UVIS':
-        instrument = header['APERTURE']
+    if instrument == "UVIS":
+        instrument = header["APERTURE"]
 
     # assuming circular aperture
     # for an ellipse, this would take the average of the axes
-    ap_radius = np.sqrt(ap_area/np.pi)
+    ap_radius = np.sqrt(ap_area / np.pi)
 
     # get correction curve
-    ac_files = glob.glob(os.path.join(hostphot_path, 'filters/HST/*'))
-    ac_file = [file for file in ac_files 
-               if f'{instrument.lower()}_aper' in file][0]
+    ac_files = glob.glob(os.path.join(hostphot_path, "filters/HST/*"))
+    ac_file = [
+        file for file in ac_files if f"{instrument.lower()}_aper" in file
+    ][0]
     ac_df = pd.read_csv(ac_file)
 
     # linear interpolation of the aperture correction
-    apertures = np.array([float(col.replace('APER#', '')) for col in ac_df.columns 
-                          if col.startswith('AP')])
-    ap_corr = ac_df[ac_df.FILTER==filt].values[0][2:].astype(float)
+    apertures = np.array(
+        [
+            float(col.replace("APER#", ""))
+            for col in ac_df.columns
+            if col.startswith("AP")
+        ]
+    )
+    ap_corr = ac_df[ac_df.FILTER == filt].values[0][2:].astype(float)
 
     cont_apertures = np.arange(0, 9, 0.01)
     cont_ap_corr = np.interp(cont_apertures, apertures, ap_corr)
 
     # get the closest value
-    ind = np.argmin(np.abs(cont_apertures-ap_radius))
+    ind = np.argmin(np.abs(cont_apertures - ap_radius))
     correction = cont_ap_corr[ind]
 
     return correction
 
+
 def magnitude_calculation(
     flux,
     flux_err,
     survey,
     filt=None,
     ap_area=0.0,
     header=None,
@@ -385,19 +400,19 @@
         survey,
         filt,
         ap_area,
         header,
         bkg_rms,
     )
 
-    if survey == 'HST':
+    if survey == "HST":
         # HST needs and aperture correction for the flux
         # see, e.g. https://www.stsci.edu/hst/instrumentation/acs/data-analysis/aperture-corrections
         ap_corr = correct_HST_aperture(filt, ap_area, header)
-        flux = flux*ap_corr
+        flux = flux * ap_corr
 
     mag = -2.5 * np.log10(flux) + zp
 
     return mag, mag_err, flux, flux_err
 
 
 def get_HST_err(filt, header):
@@ -414,35 +429,36 @@
     -------
     flux_err: float
         Error on PHOTFLAM.
     mag_err: float
         Magnitude error on PHOTFLAM.
     """
     # split instrument and filter
-    filt_split = filt.split('_')
+    filt_split = filt.split("_")
     filt = filt_split[-1]
     instrument = filt_split[-2]
 
-    if instrument=='UVIS':
+    if instrument == "UVIS":
         # APERTURE usually point to UVIS2
-        instrument = header['APERTURE']
+        instrument = header["APERTURE"]
 
     # get uncertainty file
-    err_file = os.path.join(hostphot_path, 
-                            'filters/HST/', 
-                            f'{instrument}_err.txt')
+    err_file = os.path.join(
+        hostphot_path, "filters/HST/", f"{instrument}_err.txt"
+    )
     err_df = pd.read_csv(err_file, delim_whitespace=True)
-    filt_err_df = err_df[err_df.Filter==filt]
+    filt_err_df = err_df[err_df.Filter == filt]
 
     flux = filt_err_df.PHOTFLAM.values[0]
     flux_err = filt_err_df.ERR_PHOTFLAM.values[0]
     mag_err = np.abs(2.5 * flux_err / (flux * np.log(10)))
-    
+
     return flux_err, mag_err
 
+
 def uncertainty_calculation(
     flux, flux_err, survey, filt=None, ap_area=0.0, header=None, bkg_rms=0.0
 ):
     """Calculates the uncertainty propagation.
 
     Parameters
     ----------
@@ -469,27 +485,27 @@
         Total uncertainty in flux units.
     """
     exptime = get_image_exptime(header, survey)
     gain = get_image_gain(header, survey)
     readnoise = get_image_readnoise(header, survey)
 
     mag_err = 2.5 / np.log(10) * flux_err / flux
-    
+
     if survey in ["PS1", "DES", "LegacySurvey", "Spitzer", "VISTA"]:
         if survey == "Spitzer":
             flux /= header["EFCONV"]  # conv. factor (MJy/sr)/(DN/s)
         # 1.0857 = 2.5/ln(10)
         extra_err = (
             1.0857 * np.sqrt(ap_area * (readnoise**2) + flux / gain) / flux
         )
         mag_err = np.sqrt(mag_err**2 + extra_err**2)
 
         extra_flux_err = np.sqrt(ap_area * (readnoise**2) + flux / gain)
         flux_err = np.sqrt(flux_err**2 + extra_flux_err**2)
-    
+
     if survey == "DES":
         # see the photometry section in https://des.ncsa.illinois.edu/releases/dr1/dr1-docs/quality
         # statistical uncertainties on the AB magnitud system zeropoints
         unc_dict = {
             "g": 2.6e-3,
             "r": 2.9e-3,
             "i": 3.4e-3,
@@ -506,32 +522,32 @@
             "i": 5e-3,
             "z": 6e-3,
             "Y": 5e-3,
         }
         extra_err = unc_dict[filt]
         mag_err = np.sqrt(mag_err**2 + extra_err**2)
 
-        extra_flux_err = np.abs(flux*0.4*np.log(10)*extra_err)
-        flux_err = np.sqrt(flux_err ** 2 + extra_flux_err ** 2)
+        extra_flux_err = np.abs(flux * 0.4 * np.log(10) * extra_err)
+        flux_err = np.sqrt(flux_err**2 + extra_flux_err**2)
 
     elif survey == "PS1":
         # add floor systematic error from:
         # https://iopscience.iop.org/article/10.3847/1538-4365/abb82a/pdf
         unc_dict = {
             "g": 14e-3,
             "r": 14e-3,
             "i": 15e-3,
             "z": 15e-3,
             "y": 18e-3,
         }
         floor_err = unc_dict[filt]
-        mag_err = np.sqrt(mag_err ** 2 + floor_err ** 2)
+        mag_err = np.sqrt(mag_err**2 + floor_err**2)
 
         extra_flux_err = np.abs(flux * 0.4 * np.log(10) * floor_err)
-        flux_err = np.sqrt(flux_err ** 2 + extra_flux_err ** 2)
+        flux_err = np.sqrt(flux_err**2 + extra_flux_err**2)
 
     elif survey == "SDSS":
         # https://data.sdss.org/datamodel/files/BOSS_PHOTOOBJ/frames/RERUN/RUN/CAMCOL/frame.html
         camcol = header["CAMCOL"]
         run = header["RUN"]
 
         gain_dict = {
@@ -586,43 +602,47 @@
             if camcol == 5:
                 dark_variance = 2.1025
 
         extra_err = 1.0857 * np.sqrt(dark_variance + flux / gain) / flux
         mag_err = np.sqrt(mag_err**2 + extra_err**2)
 
         extra_flux_err = np.sqrt(dark_variance + flux / gain)
-        flux_err = np.sqrt(flux_err ** 2 + extra_flux_err ** 2)
+        flux_err = np.sqrt(flux_err**2 + extra_flux_err**2)
 
     elif survey == "GALEX":
         # https://asd.gsfc.nasa.gov/archive/galex/FAQ/counts_background.html
         CPS = flux
         if filt == "FUV":
             uv_err = -2.5 * (
                 np.log10(CPS)
                 - np.log10(
                     CPS
                     + (CPS * exptime + (0.050 * CPS * exptime) ** 2) ** 0.5
                     / exptime
                 )
             )
-            flux_uv_err = np.sqrt(CPS*exptime + (0.050 * CPS * exptime)**2)/exptime
+            flux_uv_err = (
+                np.sqrt(CPS * exptime + (0.050 * CPS * exptime) ** 2) / exptime
+            )
         elif filt == "NUV":
             uv_err = -2.5 * (
                 np.log10(CPS)
                 - np.log10(
                     CPS
                     + (CPS * exptime + (0.027 * CPS * exptime) ** 2) ** 0.5
                     / exptime
                 )
             )
-            flux_uv_err = np.sqrt(CPS * exptime + (0.027 * CPS * exptime) ** 2) / exptime
+            flux_uv_err = (
+                np.sqrt(CPS * exptime + (0.027 * CPS * exptime) ** 2) / exptime
+            )
 
         mag_err = np.sqrt(mag_err**2 + uv_err**2)
 
-        flux_err = np.sqrt(flux_err ** 2 + flux_uv_err ** 2)
+        flux_err = np.sqrt(flux_err**2 + flux_uv_err**2)
 
     elif survey == "2MASS":
         # see: https://wise2.ipac.caltech.edu/staff/jarrett/2mass/3chan/noise/
         S = flux
         N_c = 6  # number of coadd pixels
         k_z = 1.7  # kernel smoothing factor
         n_f = ap_area  # number of frame pixels in the aperture; aprox. as aperture area
@@ -633,16 +653,16 @@
             S / (gain * N_c)
             + n_c * (2 * k_z * sigma_c) ** 2
             + (n_c * 0.024 * sigma_c) ** 2
         )
 
         mag_err = 1.0857 / SNR
 
-        extra_flux_err = flux/SNR
-        flux_err = np.sqrt(flux_err ** 2 + extra_flux_err ** 2)
+        extra_flux_err = flux / SNR
+        flux_err = np.sqrt(flux_err**2 + extra_flux_err**2)
 
     elif "WISE" in survey:
         # see: https://wise2.ipac.caltech.edu/docs/release/allsky/expsup/sec2_3f.html
         # see Table 5 of
         # https://wise2.ipac.caltech.edu/docs/release/allsky/expsup/sec4_4c.html#wpro
         # correction assumed to be 0 mags as PSF fitting is not used.
         m_apcor = 0.0
@@ -665,48 +685,48 @@
             * F_corr
             * (flux_err**2 + k * (N_A**2) / N_B * bkg_rms**2)
             + sigma_conf**2
         )
 
         mag_err = np.sqrt(1.179 * sigma_src**2 / F_src**2)
 
-        flux_err = f_apcor ** 2
+        flux_err = f_apcor**2
 
         # add uncertainty from the ZP
-        if survey=="unWISE":
+        if survey == "unWISE":
             # These values are the same for all Atlas Images of a given band...
             # see: https://wise2.ipac.caltech.edu/docs/release/allsky/expsup/sec2_3f.html
-            unc_dict = {'W1':0.006, 'W2':0.007, 'W3':0.012, 'W4':0.012}
+            unc_dict = {"W1": 0.006, "W2": 0.007, "W3": 0.012, "W4": 0.012}
             zp_unc = unc_dict[filt]
-        elif survey=="WISE":
+        elif survey == "WISE":
             zp_unc = header["MAGZPUNC"]
 
         mag_err = np.sqrt(mag_err**2 + zp_unc**2)
 
         extra_flux_err = np.abs(flux * 0.4 * np.log(10) * zp_unc)
-        flux_err = np.sqrt(flux_err ** 2 + extra_flux_err ** 2)
+        flux_err = np.sqrt(flux_err**2 + extra_flux_err**2)
 
     elif survey == "LegacySurvey":
         # already added at the beginning
         pass
     elif survey == "Spitzer":
         # already added at the beginning
         pass
     elif survey == "VISTA":
         # add uncertainty from the ZP
         zp_unc = header["MAGZRR"]
         mag_err = np.sqrt(mag_err**2 + zp_unc**2)
 
         extra_flux_err = np.abs(flux * 0.4 * np.log(10) * zp_unc)
-        flux_err = np.sqrt(flux_err ** 2 + extra_flux_err ** 2)
+        flux_err = np.sqrt(flux_err**2 + extra_flux_err**2)
     elif survey == "HST":
         flux_zp_unc, zp_unc = get_HST_err(filt, header)
 
         mag_err = np.sqrt(mag_err**2 + zp_unc**2)
-        flux_err = np.sqrt(flux_err ** 2 + flux_zp_unc ** 2)
+        flux_err = np.sqrt(flux_err**2 + flux_zp_unc**2)
     else:
         raise Exception(
             f"Survey {survey} has not been added for error propagation."
         )
 
     return mag_err, flux_err
 
@@ -759,49 +779,52 @@
     Parameters
     ----------
     filters: str or list
         Filters to use, e,g, ``griz``.
     survey: str
         Survey name: e.g. ``PS1``, ``GALEX``.
     """
-    if survey=='HST':
+    if survey == "HST":
         check_HST_filters(filters)
 
     else:
         valid_filters = get_survey_filters(survey)
 
         for filt in filters:
             message = (
                 f"filter '{filt}' is not a valid option for "
                 f"'{survey}' survey ({valid_filters})"
             )
             assert filt in valid_filters, message
 
+
 def check_HST_filters(filt):
     """Check whether the given filter is whithin the valid
     options for HST.
 
     Parameters
     ----------
-    filt: str 
+    filt: str
         Filter to use, e,g, ``WFC3_UVIS_F225W``.
-    """        
+    """
     if filt is None:
         raise ValueError(f"'{filt}' is not a valid HST filter.")
-    
+
     # For UVIS, only the filters of UVIS1 are used as the
     # detector 2 is scaled to match detector 1
-    if 'UVIS' in filt:
-        filt = filt.replace('UVIS', 'UVIS1')
+    if "UVIS" in filt:
+        filt = filt.replace("UVIS", "UVIS1")
 
     hostphot_path = hostphot.__path__[0]
     hst_file = glob.glob(os.path.join(hostphot_path, "filters/HST/*/*"))
-    hst_filters = [os.path.basename(file).split('.')[0] for file in hst_file]
+    hst_filters = [os.path.basename(file).split(".")[0] for file in hst_file]
 
-    assert filt in hst_filters, f"Not a valid HST filter ({filt}): {hst_filters}"
+    assert (
+        filt in hst_filters
+    ), f"Not a valid HST filter ({filt}): {hst_filters}"
 
 
 def extract_filter(filt, survey, version=None):
     """Extracts the transmission function for the filter.
 
     Parameters
     ----------
@@ -818,15 +841,15 @@
     -------
     wave: array
         Wavelength range of the filter.
     transmission: array
         Transmission function.
     """
     check_survey_validity(survey)
-    if survey=='HST':
+    if survey == "HST":
         check_filters_validity(filt, survey)
     else:
         check_filters_validity([filt], survey)
 
     if "WISE" in survey:
         survey = "WISE"  # for unWISE to use the same filters as WISE
 
@@ -835,27 +858,27 @@
     # Assume DECaLS filters below 32 degrees and BASS+MzLS above
     # https://www.legacysurvey.org/status/
     if survey == "LegacySurvey":
         if version == "BASS+MzLS":
             if filt == "z":
                 filt_file = os.path.join(filters_path, f"MzLS_z.dat")
             else:
-                filt_file = os.path.join(filters_path, f"BASS_{filt}.dat")       
+                filt_file = os.path.join(filters_path, f"BASS_{filt}.dat")
         elif version == "DECam":
             filt_file = os.path.join(filters_path, f"DECAM_{filt}.dat")
 
     elif survey == "HST":
-        if 'UVIS' in filt:
+        if "UVIS" in filt:
             # Usually UVIS2 is used, but there is no large difference
-            filt = filt.replace('UVIS', 'UVIS2')
-        hst_files = glob.glob(os.path.join(filters_path, '*/*'))
+            filt = filt.replace("UVIS", "UVIS2")
+        hst_files = glob.glob(os.path.join(filters_path, "*/*"))
         filt_file = [file for file in hst_files if filt in file][0]
     else:
         filt_file = os.path.join(filters_path, f"{survey}_{filt}.dat")
-    
+
     wave, transmission = np.loadtxt(filt_file).T
 
     return wave, transmission
 
 
 def integrate_filter(
     spectrum_wave,
@@ -894,14 +917,15 @@
         spectrum_flux * interp_response * spectrum_wave, spectrum_wave
     )
     int2 = np.trapz(filter_response * filter_wave, filter_wave)
     flux_filter = int1 / int2
 
     return flux_filter
 
+
 def adapt_aperture(objects, img_wcs, img_wcs2, flip=False):
     """Changes the aperture parameters to consider differences
     in WCS between surveys.
 
     The values of ``center``, ``a`` and ``b`` should in pixel
     units. DES images are flipped, so these need to be corrected
     with ``theta -> -theta``, i.e. using ``flip=True``.
@@ -911,42 +935,44 @@
     objects: ndarray
         Objects with apertures.
     img_wcs: ~wcs.WCS
         WCS of the image from where the objects were extracted.
     img_wcs2: ~wcs.WCS
         WCS used to adapt the apertures.
     flip: bool, default ``False``
-        Whether to flip the orientation of the aperture. Only 
+        Whether to flip the orientation of the aperture. Only
         used for DES images.
 
     Returns
     -------
     objects_: ndarray
         Objects with adapted apertures.
     """
     objects_ = objects.copy()  # avoid modifying the intial objects
     for obj in objects_:
-        center = (obj['x'], obj['y'])
-        apertures = EllipticalAperture(center, obj['a'],
-                                       obj['b'], obj['theta'])
+        center = (obj["x"], obj["y"])
+        apertures = EllipticalAperture(
+            center, obj["a"], obj["b"], obj["theta"]
+        )
         sky_apertures = apertures.to_sky(img_wcs)
 
         new_apertures = sky_apertures.to_pixel(img_wcs2)
         new_center = new_apertures.positions
-        obj['x'], obj['y'] = new_center
-        obj['a'] = new_apertures.a
-        obj['b'] = new_apertures.b
-        obj['theta'] = new_apertures.theta
+        obj["x"], obj["y"] = new_center
+        obj["a"] = new_apertures.a
+        obj["b"] = new_apertures.b
+        obj["theta"] = new_apertures.theta
 
         if flip is True:
             # flip aperture orientation
-            obj['theta'] *= -1
+            obj["theta"] *= -1
 
     return objects_
 
+
 def check_work_dir(wokrdir):
     """Checks if the working directory exists. If it
     does not, one is created.
 
     Parameters
     ----------
     wokrdir: str
@@ -977,53 +1003,46 @@
     ----------
     fits_file: str or HDU.
         Path to fits file.
     ext: int
         Extension index.
     """
     if isinstance(fits_file, str):
-        hdu = fits.open(fits_file)
         title = os.path.splitext(os.path.basename(fits_file))[0]
     else:
-        hdu = fits_file
         title = None
-    header = hdu[ext].header
-    data = hdu[ext].data
 
+    figure = plt.figure(figsize=(10, 10))
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", AstropyWarning)
-        img_wcs = wcs.WCS(header, naxis=2)
+        fig = aplpy.FITSFigure(fits_file, hdu=ext, figure=figure)
 
-    m, s = np.nanmean(data), np.nanstd(data)
+    with suppress_stdout():
+        fig.show_grayscale(stretch="arcsinh")
+
+    # ticks
+    fig.tick_labels.set_font(**{"family": font, "size": 18})
+    fig.tick_labels.set_xformat("dd.dd")
+    fig.tick_labels.set_yformat("dd.dd")
+    fig.ticks.set_length(6)
+
+    fig.axis_labels.set_font(**{"family": font, "size": 18})
+
+    fig.set_title(title, **{"family": font, "size": 24})
+    fig.set_theme("publication")
 
-    fig = plt.figure(figsize=(10, 10))
-    ax = plt.subplot(projection=img_wcs)
-    ax.set_title(title, fontsize=18)
-    update_axislabels(ax)
-
-    im = ax.imshow(
-        data,
-        interpolation="nearest",
-        cmap="gray",
-        vmin=m - s,
-        vmax=m + s,
-        origin="lower",
-    )
-    
     plt.show()
 
 
-def update_axislabels(ax):
-    """Updates the labels and ticks of a plot.
+@contextmanager
+def suppress_stdout():
+    """Suppresses annoying outputs.
 
-    Parameters
-    ----------
-    ax: `.axes.SubplotBase`.
-        The axis of a subplot.
+    Useful with astroquery and aplpy packages.
     """
-    for i in range(2):
-        ax.coords[i].set_ticklabel(size=16)
-        if i == 0:
-            ax.coords[i].set_axislabel("RA (J2000)", fontsize=20)
-        else:
-            ax.coords[i].set_axislabel("Dec (J2000)", fontsize=20)
-            # ax.coords[i].set_ticklabel(rotation=65)
+    with open(os.devnull, "w") as devnull:
+        old_stdout = sys.stdout
+        sys.stdout = devnull
+        try:
+            yield
+        finally:
+            sys.stdout = old_stdout
```

### Comparing `hostphot-2.6.1/src/hostphot.egg-info/PKG-INFO` & `hostphot-2.6.2/src/hostphot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hostphot
-Version: 2.6.1
+Version: 2.6.2
 Summary: Global and local photometry of galaxies hosting supernovae or other transients
 Home-page: https://github.com/temuller/hostphot
 Author: Tomás Enrique Müller-Bravo and Lluís Galbany
 Author-email: t.e.muller-bravo@ice.csic.es
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -192,14 +192,18 @@
   number = {76}, 
   pages = {4508},  
   journal = {Journal of Open Source Software} 
 } 
 ```
 
 ## What's new!
+v2.6.2
+* Prettier plots (now using `aplpy`), but also more informative!
+* Scale of the apertures for the masks is now a parameter (`r`) 
+* Raise exception is now `True` by default when calculating photometry
 v2.6.1
 * 2MASS cutouts improved (picking largest image)
 v2.6.0:
 * HST (WFC3 only - pseudo-trial) included
 * 2MASS cutouts fixed (it now downloads the image closest to the given coordinates)
 v2.5.1:
 * Using sfdmap2 instead of sfdmap to avoid issues with numpy version (requires Python>=3.9)
```

### Comparing `hostphot-2.6.1/src/hostphot.egg-info/SOURCES.txt` & `hostphot-2.6.2/src/hostphot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/tests/test_cutouts.py` & `hostphot-2.6.2/tests/test_cutouts.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/tests/test_global_phot.py` & `hostphot-2.6.2/tests/test_global_phot.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             host_ra,
             host_dec,
             survey=survey,
             use_mask=False,
             common_aperture=False,
             optimize_kronrad=True,
             save_plots=True,
-            raise_exception=True
+            raise_exception=True,
         )
         mags = [phot[filt] for filt in "griz"]
         # griz SIMBAD reference magnitudes of the host galaxy of SN 2002fk
         ref_mags = [12.155, 11.508, 11.205, 10.979]
 
         err_msg = (
             "Large difference between calculated and reference magnitudes"
```

### Comparing `hostphot-2.6.1/tests/test_local_phot.py` & `hostphot-2.6.2/tests/test_local_phot.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             dec,
             z,
             survey="PS1",
             filters="grizy",
             ap_radii=ap_radii,
             use_mask=False,
             save_plots=True,
-            raise_exception=True
+            raise_exception=True,
         )
         mags = [phot[filt] for filt in ["g_4", "r_4", "i_4", "z_4"]]
         # pre-calculated magnitudes
         ref_mags = [12.26, 11.89, 11.72, 11.57]
 
         err_msg = (
             "Large difference between calculated and reference magnitudes"
```

### Comparing `hostphot-2.6.1/tests/test_preprocessing.py` & `hostphot-2.6.2/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.6.1/tests/test_rgb_images.py` & `hostphot-2.6.2/tests/test_rgb_images.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,14 @@
         for scaling in ["linear", "sqrt", "log", "asinh"]:
             create_RGB_image(images_dir=images_dir, scaling=scaling)
 
     def test_get_PS1_RGB_image(self):
         ra, dec = 50.527333, -15.400056
         get_PS1_RGB_image("PS1.jpg", ra=ra, dec=dec)
 
-    #def test_get_SDSS_RGB_image(self):
+    # def test_get_SDSS_RGB_image(self):
     #    ra, dec = 50.527333, -15.400056
     #    get_SDSS_RGB_image("SDSS.jpg", ra=ra, dec=dec)
 
 
 if __name__ == "__main__":
     unittest.main()
```

