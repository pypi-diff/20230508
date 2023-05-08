# Comparing `tmp/hostphot-2.5.1.tar.gz` & `tmp/hostphot-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hostphot-2.5.1.tar", last modified: Fri Apr 28 10:01:50 2023, max compression
+gzip compressed data, was "hostphot-2.6.0.tar", last modified: Mon May  8 02:32:27 2023, max compression
```

## Comparing `hostphot-2.5.1.tar` & `hostphot-2.6.0.tar`

### file list

```diff
@@ -1,325 +1,330 @@
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-28 10:01:50.075446 hostphot-2.5.1/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1065 2022-05-31 09:22:42.000000 hostphot-2.5.1/LICENSE
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       53 2022-05-31 09:22:42.000000 hostphot-2.5.1/MANIFEST.in
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     8748 2023-04-28 10:01:50.075446 hostphot-2.5.1/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     8216 2023-04-25 09:34:42.000000 hostphot-2.5.1/README.md
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      187 2022-05-31 09:22:42.000000 hostphot-2.5.1/pyproject.toml
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      184 2023-04-28 09:57:11.000000 hostphot-2.5.1/requirements.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-04-28 10:01:50.075446 hostphot-2.5.1/setup.cfg
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1251 2023-04-28 09:57:11.000000 hostphot-2.5.1/setup.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-28 10:01:50.023445 hostphot-2.5.1/src/
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-28 10:01:50.027445 hostphot-2.5.1/src/hostphot/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      412 2022-08-30 07:45:59.000000 hostphot-2.5.1/src/hostphot/__init__.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      123 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/_constants.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       47 2023-04-28 09:57:11.000000 hostphot-2.5.1/src/hostphot/_version.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1762 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/coadd.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    44116 2023-04-25 15:01:12.000000 hostphot-2.5.1/src/hostphot/cutouts.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6163 2023-04-28 09:57:11.000000 hostphot-2.5.1/src/hostphot/dust.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-28 10:01:50.027445 hostphot-2.5.1/src/hostphot/filters/
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-28 10:01:50.027445 hostphot-2.5.1/src/hostphot/filters/2MASS/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1218 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/filters/2MASS/2MASS_H.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2247 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/filters/2MASS/2MASS_J.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1596 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/filters/2MASS/2MASS_Ks.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/filters/2MASS/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1549 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/filters/AAA_README
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-28 10:01:50.027445 hostphot-2.5.1/src/hostphot/filters/DES/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       53 2022-05-31 09:22:42.000000 hostphot-2.5.1/src/hostphot/filters/DES/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3387 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/filters/DES/DES_Y.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4281 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/filters/DES/DES_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4515 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/filters/DES/DES_i.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4516 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/filters/DES/DES_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4338 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/filters/DES/DES_z.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-28 10:01:50.027445 hostphot-2.5.1/src/hostphot/filters/GALEX/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/filters/GALEX/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6777 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/filters/GALEX/GALEX_FUV.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18911 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/filters/GALEX/GALEX_NUV.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-28 10:01:50.031445 hostphot-2.5.1/src/hostphot/filters/HST/
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-28 10:01:50.035446 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    23838 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F435W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    32416 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F475W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4110 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F502N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    15624 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F550M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    31966 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F555W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    43735 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F606W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    29858 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F625W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5234 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F658N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3236 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F660N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    37258 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F775W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   103143 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F814W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    53451 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F850LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7990 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F892N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21666 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR1016N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9107 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR388N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9858 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR423N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    36616 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR459M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    10646 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR462N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11519 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR505N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12578 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR551N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13680 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR601N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    53850 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR647M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    14675 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR656N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    15873 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR716N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    17289 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR782N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18750 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR853N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    61170 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR914M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19635 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR931N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11835 2023-04-25 09:34:42.000000 hostphot-2.5.1/src/hostphot/filters/HST/HST_filters.txt
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-28 10:01:50.039445 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9747 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F090M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2486 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F095N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2874 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F097N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3264 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F108N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12445 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24500 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3077 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F113N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    33411 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F140W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13978 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F145M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21021 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F160W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4877 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F164N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11680 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F165M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5199 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F166N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12148 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F170M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6879 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F187N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7831 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F190N.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-28 10:01:50.039445 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24275 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F110W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20849 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F160W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12018 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F165M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18588 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F171M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    17947 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F180M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6506 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    41358 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5506 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F190N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21662 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F204M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    30947 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F205W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20965 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F207M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11516 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F212N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7894 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F215N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7479 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F216N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    30813 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F222M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26323 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F237M.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-28 10:01:50.043445 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3240 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F108N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24427 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F110W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3363 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F113N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    35249 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F150W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20994 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F160W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4858 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F164N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4820 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F166N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    43711 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F175W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6876 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F187N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5510 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F190N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7212 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F196N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9291 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F200N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11541 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F212N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7906 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F215N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    30812 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F222M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13019 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F240M.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-28 10:01:50.043445 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     8959 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F098M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9826 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F105W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21512 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F110W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    22426 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F125W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4121 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F126N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5064 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F127M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6580 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F128N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3261 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F130N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3792 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F132N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5421 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F139M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13977 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F140W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6752 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F153M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    10046 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F160W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4738 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F164N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6887 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F167N.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-28 10:01:50.059445 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   156254 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F200LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21978 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F218W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    29976 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F225W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21591 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F275W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7558 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F280N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    56436 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F300X.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    15547 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F336W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19356 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F343N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   146819 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F350LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4504 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F373N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9638 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26406 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7035 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F395N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9314 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F410M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18697 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F438W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9833 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F467M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3637 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F469N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    32782 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    72677 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475X.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5098 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F487N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5804 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F502N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    38578 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F547M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    63538 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F555W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    97333 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F600LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    51442 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F606W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21890 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F621M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    34917 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F625W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4204 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F631N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3675 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F645N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2150 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F656N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11299 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F657N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3236 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F658N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11865 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F665N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11991 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F673N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13792 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F680N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20007 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F689M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19898 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F763M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    36590 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F775W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    54378 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F814W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    33733 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F845M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    57316 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F850LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12497 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F953N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13422 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ232N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13900 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ243N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21137 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ378N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6727 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ387N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    39729 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ422M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11393 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ436N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1548 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ437N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    22828 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ492N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26635 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ508N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4658 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ575N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19283 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ619N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20492 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ634N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4687 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ672N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4387 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ674N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24973 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ727N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    25138 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ750N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2950 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ889N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2948 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ906N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3346 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ924N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3461 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ937N.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-28 10:01:50.071446 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   156503 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F200LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20752 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F218W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    29190 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F225W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21479 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F275W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7566 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F280N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    55542 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F300X.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    15542 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F336W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19332 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F343N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   147032 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F350LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4495 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F373N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9640 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26441 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7031 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F395N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9300 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F410M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    18727 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F438W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     9871 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F467M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3641 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F469N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    32751 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    72732 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475X.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5104 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F487N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5798 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F502N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    38608 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F547M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    63493 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F555W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    97494 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F600LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    51384 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F606W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21858 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F621M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    34960 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F625W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4209 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F631N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3686 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F645N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2154 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F656N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11309 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F657N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3233 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F658N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11857 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F665N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11991 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F673N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13805 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F680N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20019 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F689M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19919 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F763M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    36600 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F775W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    54473 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F814W.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    33739 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F845M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    57507 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F850LP.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12507 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F953N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13422 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ232N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13900 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ243N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21137 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ378N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6727 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ387N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    39729 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ422M.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    11393 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ436N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1548 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ437N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    22828 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ492N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    26635 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ508N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4658 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ575N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19283 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ619N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    20492 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ634N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4687 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ672N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4387 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ674N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24973 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ727N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    25138 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ750N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2950 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ889N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2948 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ906N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3346 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ924N.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3461 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ937N.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-28 10:01:50.071446 hostphot-2.5.1/src/hostphot/filters/LegacySurvey/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2281 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/filters/LegacySurvey/BASS_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3180 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/filters/LegacySurvey/BASS_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21743 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/filters/LegacySurvey/DECAM_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21744 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/filters/LegacySurvey/DECAM_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    21744 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/filters/LegacySurvey/DECAM_z.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7028 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/filters/LegacySurvey/MzLS_z.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      300 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/filters/LegacySurvey/README.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4275 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/filters/LegacySurvey/init_BASS_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5840 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/filters/LegacySurvey/init_BASS_r.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-28 10:01:50.071446 hostphot-2.5.1/src/hostphot/filters/PS1/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      136 2022-05-31 09:22:42.000000 hostphot-2.5.1/src/hostphot/filters/PS1/AAA_README.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3717 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/filters/PS1/PS1_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3759 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/filters/PS1/PS1_i.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3885 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/filters/PS1/PS1_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4385 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/filters/PS1/PS1_y.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3486 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/filters/PS1/PS1_z.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-28 10:01:50.071446 hostphot-2.5.1/src/hostphot/filters/SDSS/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       72 2022-05-31 09:22:42.000000 hostphot-2.5.1/src/hostphot/filters/SDSS/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1414 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/filters/SDSS/SDSS_g.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1260 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/filters/SDSS/SDSS_i.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1176 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/filters/SDSS/SDSS_r.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4718 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/filters/SDSS/SDSS_u.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2509 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/filters/SDSS/SDSS_z.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-28 10:01:50.071446 hostphot-2.5.1/src/hostphot/filters/Spitzer/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      189 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/filters/Spitzer/README.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     8211 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.1.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     8421 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.2.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     6531 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.3.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     7375 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.4.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2816 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/filters/Spitzer/Spitzer_MIPS.1.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-28 10:01:50.075446 hostphot-2.5.1/src/hostphot/filters/VISTA/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       84 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/filters/VISTA/README.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    39168 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/filters/VISTA/VISTA_H.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    50048 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/filters/VISTA/VISTA_J.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    41344 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/filters/VISTA/VISTA_Ks.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    46341 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/filters/VISTA/VISTA_Y.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)   176418 2022-11-14 14:06:00.000000 hostphot-2.5.1/src/hostphot/filters/VISTA/VISTA_Z.dat
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-28 10:01:50.075446 hostphot-2.5.1/src/hostphot/filters/WISE/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/filters/WISE/AAA_README
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2961 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/WISE/WISE_W1.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3528 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/WISE/WISE_W2.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    24404 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/WISE/WISE_W3.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    19734 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/filters/WISE/WISE_W4.dat
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      739 2023-04-24 13:20:08.000000 hostphot-2.5.1/src/hostphot/filters/config.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    22688 2023-04-25 09:34:42.000000 hostphot-2.5.1/src/hostphot/global_photometry.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2494 2022-07-28 14:32:41.000000 hostphot-2.5.1/src/hostphot/image_cleaning.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12319 2023-04-25 09:34:42.000000 hostphot-2.5.1/src/hostphot/image_masking.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    12493 2023-04-25 09:34:42.000000 hostphot-2.5.1/src/hostphot/interactive_aperture.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    13116 2023-04-25 09:34:42.000000 hostphot-2.5.1/src/hostphot/local_photometry.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     8326 2023-04-25 09:34:42.000000 hostphot-2.5.1/src/hostphot/objects_detect.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    10706 2022-08-15 08:03:30.000000 hostphot-2.5.1/src/hostphot/rgb_images.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    27890 2023-04-25 09:34:42.000000 hostphot-2.5.1/src/hostphot/utils.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-28 10:01:50.027445 hostphot-2.5.1/src/hostphot.egg-info/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     8748 2023-04-28 10:01:50.000000 hostphot-2.5.1/src/hostphot.egg-info/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)    14716 2023-04-28 10:01:50.000000 hostphot-2.5.1/src/hostphot.egg-info/SOURCES.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-04-28 10:01:50.000000 hostphot-2.5.1/src/hostphot.egg-info/dependency_links.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      187 2023-04-28 10:01:50.000000 hostphot-2.5.1/src/hostphot.egg-info/requires.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        9 2023-04-28 10:01:50.000000 hostphot-2.5.1/src/hostphot.egg-info/top_level.txt
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-04-28 10:01:50.075446 hostphot-2.5.1/tests/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     2771 2023-04-25 09:34:42.000000 hostphot-2.5.1/tests/test_cutouts.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1073 2023-04-28 09:57:11.000000 hostphot-2.5.1/tests/test_global_phot.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      460 2022-07-28 14:32:41.000000 hostphot-2.5.1/tests/test_interactivity.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1088 2023-04-28 09:57:11.000000 hostphot-2.5.1/tests/test_local_phot.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1095 2022-07-28 14:32:41.000000 hostphot-2.5.1/tests/test_preprocessing.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      860 2023-04-25 09:34:42.000000 hostphot-2.5.1/tests/test_rgb_images.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-08 02:32:27.363835 hostphot-2.6.0/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1065 2022-05-31 09:22:42.000000 hostphot-2.6.0/LICENSE
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       53 2022-05-31 09:22:42.000000 hostphot-2.6.0/MANIFEST.in
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8967 2023-05-08 02:32:27.363835 hostphot-2.6.0/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8435 2023-05-05 10:39:56.000000 hostphot-2.6.0/README.md
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      187 2022-05-31 09:22:42.000000 hostphot-2.6.0/pyproject.toml
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      184 2023-04-28 09:57:11.000000 hostphot-2.6.0/requirements.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-05-08 02:32:27.363835 hostphot-2.6.0/setup.cfg
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1251 2023-04-28 09:57:11.000000 hostphot-2.6.0/setup.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-08 02:32:27.295836 hostphot-2.6.0/src/
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-08 02:32:27.299836 hostphot-2.6.0/src/hostphot/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      412 2022-08-30 07:45:59.000000 hostphot-2.6.0/src/hostphot/__init__.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      123 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/_constants.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       47 2023-05-05 10:39:56.000000 hostphot-2.6.0/src/hostphot/_version.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1762 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/coadd.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    45837 2023-05-05 10:39:56.000000 hostphot-2.6.0/src/hostphot/cutouts.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6006 2023-05-05 10:39:56.000000 hostphot-2.6.0/src/hostphot/dust.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-08 02:32:27.299836 hostphot-2.6.0/src/hostphot/filters/
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-08 02:32:27.299836 hostphot-2.6.0/src/hostphot/filters/2MASS/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1218 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/filters/2MASS/2MASS_H.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2247 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/filters/2MASS/2MASS_J.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1596 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/filters/2MASS/2MASS_Ks.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/filters/2MASS/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1549 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/filters/AAA_README
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-08 02:32:27.303836 hostphot-2.6.0/src/hostphot/filters/DES/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       53 2022-05-31 09:22:42.000000 hostphot-2.6.0/src/hostphot/filters/DES/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3387 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/filters/DES/DES_Y.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4281 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/filters/DES/DES_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4515 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/filters/DES/DES_i.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4516 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/filters/DES/DES_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4338 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/filters/DES/DES_z.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-08 02:32:27.303836 hostphot-2.6.0/src/hostphot/filters/GALEX/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/filters/GALEX/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6777 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/filters/GALEX/GALEX_FUV.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18911 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/filters/GALEX/GALEX_NUV.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-08 02:32:27.303836 hostphot-2.6.0/src/hostphot/filters/HST/
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-08 02:32:27.311836 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    23838 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F435W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    32416 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F475W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4110 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F502N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    15624 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F550M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    31966 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F555W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    43735 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F606W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    29858 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F625W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5234 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F658N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3236 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F660N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    37258 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F775W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   103143 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F814W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    53451 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F850LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7990 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F892N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21666 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR1016N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9107 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR388N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9858 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR423N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    36616 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR459M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    10646 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR462N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11519 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR505N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12578 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR551N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13680 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR601N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    53850 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR647M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    14675 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR656N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    15873 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR716N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    17289 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR782N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18750 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR853N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    61170 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR914M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19635 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR931N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1264 2023-05-05 10:39:56.000000 hostphot-2.6.0/src/hostphot/filters/HST/IR_err.txt
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-08 02:32:27.311836 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9747 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F090M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2486 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F095N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2874 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F097N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3264 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F108N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12445 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24500 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3077 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F113N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    33411 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F140W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13978 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F145M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21021 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F160W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4877 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F164N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11680 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F165M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5199 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F166N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12148 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F170M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6879 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F187N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7831 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F190N.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-08 02:32:27.315836 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24275 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F110W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20849 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F160W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12018 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F165M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18588 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F171M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    17947 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F180M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6506 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    41358 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5506 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F190N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21662 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F204M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    30947 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F205W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20965 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F207M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11516 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F212N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7894 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F215N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7479 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F216N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    30813 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F222M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26323 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F237M.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-08 02:32:27.319836 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3240 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F108N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24427 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F110W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3363 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F113N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    35249 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F150W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20994 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F160W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4858 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F164N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4820 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F166N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    43711 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F175W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6876 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F187N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5510 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F190N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7212 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F196N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9291 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F200N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11541 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F212N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7906 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F215N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    30812 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F222M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13019 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F240M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3503 2023-05-05 10:39:56.000000 hostphot-2.6.0/src/hostphot/filters/HST/UVIS1_err.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3503 2023-05-05 10:39:56.000000 hostphot-2.6.0/src/hostphot/filters/HST/UVIS2_err.txt
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-08 02:32:27.323835 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8959 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F098M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9826 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F105W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21512 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F110W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    22426 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F125W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4121 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F126N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5064 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F127M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6580 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F128N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3261 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F130N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3792 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F132N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5421 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F139M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13977 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F140W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6752 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F153M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    10046 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F160W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4738 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F164N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6887 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F167N.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-08 02:32:27.339835 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   156254 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F200LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21978 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F218W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    29976 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F225W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21591 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F275W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7558 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F280N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    56436 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F300X.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    15547 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F336W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19356 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F343N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   146819 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F350LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4504 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F373N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9638 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26406 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7035 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F395N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9314 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F410M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18697 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F438W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9833 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F467M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3637 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F469N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    32782 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    72677 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475X.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5098 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F487N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5804 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F502N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    38578 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F547M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    63538 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F555W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    97333 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F600LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    51442 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F606W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21890 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F621M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    34917 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F625W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4204 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F631N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3675 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F645N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2150 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F656N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11299 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F657N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3236 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F658N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11865 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F665N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11991 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F673N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13792 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F680N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20007 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F689M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19898 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F763M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    36590 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F775W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    54378 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F814W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    33733 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F845M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    57316 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F850LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12497 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F953N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13422 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ232N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13900 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ243N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21137 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ378N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6727 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ387N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    39729 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ422M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11393 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ436N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1548 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ437N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    22828 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ492N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26635 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ508N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4658 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ575N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19283 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ619N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20492 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ634N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4687 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ672N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4387 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ674N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24973 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ727N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    25138 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ750N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2950 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ889N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2948 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ906N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3346 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ924N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3461 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ937N.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-08 02:32:27.355835 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   156503 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F200LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20752 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F218W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    29190 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F225W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21479 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F275W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7566 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F280N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    55542 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F300X.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    15542 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F336W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19332 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F343N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   147032 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F350LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4495 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F373N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9640 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26441 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7031 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F395N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9300 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F410M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18727 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F438W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     9871 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F467M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3641 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F469N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    32751 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    72732 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475X.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5104 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F487N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5798 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F502N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    38608 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F547M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    63493 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F555W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    97494 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F600LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    51384 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F606W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21858 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F621M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    34960 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F625W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4209 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F631N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3686 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F645N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2154 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F656N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11309 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F657N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3233 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F658N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11857 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F665N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11991 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F673N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13805 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F680N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20019 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F689M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19919 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F763M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    36600 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F775W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    54473 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F814W.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    33739 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F845M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    57507 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F850LP.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12507 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F953N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13422 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ232N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13900 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ243N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21137 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ378N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6727 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ387N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    39729 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ422M.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    11393 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ436N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1548 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ437N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    22828 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ492N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    26635 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ508N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4658 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ575N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19283 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ619N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    20492 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ634N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4687 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ672N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4387 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ674N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24973 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ727N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    25138 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ750N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2950 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ889N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2948 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ906N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3346 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ924N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3461 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ937N.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2012 2023-05-05 10:39:56.000000 hostphot-2.6.0/src/hostphot/filters/HST/ir_aper_corrections.csv
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18667 2023-05-05 10:39:56.000000 hostphot-2.6.0/src/hostphot/filters/HST/wfc3uvis1_aper_007_syn.csv
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    18635 2023-05-05 10:39:56.000000 hostphot-2.6.0/src/hostphot/filters/HST/wfc3uvis2_aper_007_syn.csv
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-08 02:32:27.355835 hostphot-2.6.0/src/hostphot/filters/LegacySurvey/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2281 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/filters/LegacySurvey/BASS_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3180 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/filters/LegacySurvey/BASS_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21743 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/filters/LegacySurvey/DECAM_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21744 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/filters/LegacySurvey/DECAM_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    21744 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/filters/LegacySurvey/DECAM_z.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7028 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/filters/LegacySurvey/MzLS_z.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      300 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/filters/LegacySurvey/README.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4275 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/filters/LegacySurvey/init_BASS_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5840 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/filters/LegacySurvey/init_BASS_r.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-08 02:32:27.355835 hostphot-2.6.0/src/hostphot/filters/PS1/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      136 2022-05-31 09:22:42.000000 hostphot-2.6.0/src/hostphot/filters/PS1/AAA_README.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3717 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/filters/PS1/PS1_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3759 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/filters/PS1/PS1_i.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3885 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/filters/PS1/PS1_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4385 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/filters/PS1/PS1_y.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3486 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/filters/PS1/PS1_z.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-08 02:32:27.355835 hostphot-2.6.0/src/hostphot/filters/SDSS/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       72 2022-05-31 09:22:42.000000 hostphot-2.6.0/src/hostphot/filters/SDSS/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1414 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/filters/SDSS/SDSS_g.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1260 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/filters/SDSS/SDSS_i.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1176 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/filters/SDSS/SDSS_r.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     4718 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/filters/SDSS/SDSS_u.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2509 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/filters/SDSS/SDSS_z.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-08 02:32:27.359835 hostphot-2.6.0/src/hostphot/filters/Spitzer/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      189 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/filters/Spitzer/README.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8211 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.1.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8421 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.2.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     6531 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.3.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     7375 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.4.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2816 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/filters/Spitzer/Spitzer_MIPS.1.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-08 02:32:27.359835 hostphot-2.6.0/src/hostphot/filters/VISTA/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       84 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/filters/VISTA/README.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    39168 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/filters/VISTA/VISTA_H.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    50048 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/filters/VISTA/VISTA_J.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    41344 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/filters/VISTA/VISTA_Ks.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    46341 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/filters/VISTA/VISTA_Y.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)   176418 2022-11-14 14:06:00.000000 hostphot-2.6.0/src/hostphot/filters/VISTA/VISTA_Z.dat
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-08 02:32:27.359835 hostphot-2.6.0/src/hostphot/filters/WISE/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/filters/WISE/AAA_README
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2961 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/WISE/WISE_W1.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     3528 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/WISE/WISE_W2.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    24404 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/WISE/WISE_W3.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    19734 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/filters/WISE/WISE_W4.dat
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      739 2023-04-24 13:20:08.000000 hostphot-2.6.0/src/hostphot/filters/config.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    22899 2023-05-05 10:39:56.000000 hostphot-2.6.0/src/hostphot/global_photometry.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2494 2022-07-28 14:32:41.000000 hostphot-2.6.0/src/hostphot/image_cleaning.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12319 2023-04-25 09:34:42.000000 hostphot-2.6.0/src/hostphot/image_masking.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    12493 2023-04-25 09:34:42.000000 hostphot-2.6.0/src/hostphot/interactive_aperture.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    13261 2023-05-05 10:39:56.000000 hostphot-2.6.0/src/hostphot/local_photometry.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8326 2023-04-25 09:34:42.000000 hostphot-2.6.0/src/hostphot/objects_detect.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    10706 2022-08-15 08:03:30.000000 hostphot-2.6.0/src/hostphot/rgb_images.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    30137 2023-05-05 10:39:56.000000 hostphot-2.6.0/src/hostphot/utils.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-08 02:32:27.299836 hostphot-2.6.0/src/hostphot.egg-info/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     8967 2023-05-08 02:32:27.000000 hostphot-2.6.0/src/hostphot.egg-info/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)    14942 2023-05-08 02:32:27.000000 hostphot-2.6.0/src/hostphot.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-05-08 02:32:27.000000 hostphot-2.6.0/src/hostphot.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      187 2023-05-08 02:32:27.000000 hostphot-2.6.0/src/hostphot.egg-info/requires.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        9 2023-05-08 02:32:27.000000 hostphot-2.6.0/src/hostphot.egg-info/top_level.txt
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-08 02:32:27.363835 hostphot-2.6.0/tests/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2771 2023-04-25 09:34:42.000000 hostphot-2.6.0/tests/test_cutouts.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1073 2023-04-28 09:57:11.000000 hostphot-2.6.0/tests/test_global_phot.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      460 2022-07-28 14:32:41.000000 hostphot-2.6.0/tests/test_interactivity.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1088 2023-04-28 09:57:11.000000 hostphot-2.6.0/tests/test_local_phot.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1095 2022-07-28 14:32:41.000000 hostphot-2.6.0/tests/test_preprocessing.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      860 2023-04-25 09:34:42.000000 hostphot-2.6.0/tests/test_rgb_images.py
```

### Comparing `hostphot-2.5.1/LICENSE` & `hostphot-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/PKG-INFO` & `hostphot-2.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hostphot
-Version: 2.5.1
+Version: 2.6.0
 Summary: Global and local photometry of galaxies hosting supernovae or other transients
 Home-page: https://github.com/temuller/hostphot
 Author: Tomás Enrique Müller-Bravo and Lluís Galbany
 Author-email: t.e.muller-bravo@ice.csic.es
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -192,14 +192,19 @@
   number = {76}, 
   pages = {4508},  
   journal = {Journal of Open Source Software} 
 } 
 ```
 
 ## What's new!
+v2.6.0:
+* HST (WFC3 only) included
+* 2MASS cutouts fixed (it now downloads the image closest to the given coordinates)
+v2.5.1:
+* Using sfdmap2 instead of sfdmap to avoid issues with numpy version (requires Python>=3.9)
 v2.5.0:
 * Systematic error floor added to PS1 photometry
 * Added missing uncertainties in the error budget of DES (~5 mmag) 
 * Flux/counts have been added to output photometry
 * GALEX now downloads images with largest exposure time by default
 * Fixed image realignment/orientation between different surveys when using common apertures (for masking and global photometry)
 * Added option to output mask parameters, and also aperture parameters for global photometry
```

### Comparing `hostphot-2.5.1/README.md` & `hostphot-2.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -177,14 +177,19 @@
   number = {76}, 
   pages = {4508},  
   journal = {Journal of Open Source Software} 
 } 
 ```
 
 ## What's new!
+v2.6.0:
+* HST (WFC3 only) included
+* 2MASS cutouts fixed (it now downloads the image closest to the given coordinates)
+v2.5.1:
+* Using sfdmap2 instead of sfdmap to avoid issues with numpy version (requires Python>=3.9)
 v2.5.0:
 * Systematic error floor added to PS1 photometry
 * Added missing uncertainties in the error budget of DES (~5 mmag) 
 * Flux/counts have been added to output photometry
 * GALEX now downloads images with largest exposure time by default
 * Fixed image realignment/orientation between different surveys when using common apertures (for masking and global photometry)
 * Added option to output mask parameters, and also aperture parameters for global photometry
```

### Comparing `hostphot-2.5.1/setup.py` & `hostphot-2.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/coadd.py` & `hostphot-2.6.0/src/hostphot/coadd.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/cutouts.py` & `hostphot-2.6.0/src/hostphot/cutouts.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from hostphot._constants import workdir
 from hostphot.utils import (
     get_survey_filters,
     clean_dir,
     check_work_dir,
     check_survey_validity,
     check_filters_validity,
-    check_HST_inputs,
+    check_HST_filters,
     survey_pixel_scale,
 )
 
 import warnings
 from astropy.utils.exceptions import AstropyWarning
 
 
@@ -337,85 +337,50 @@
         size_arcsec = (size * u.arcmin).to(u.arcsec)
     else:
         size_arcsec = size.to(u.arcsec)
 
     pixel_scale = survey_pixel_scale(survey)
     size_pixels = int(size_arcsec.value / pixel_scale)
 
-    pos = SkyCoord(ra=ra * u.degree, dec=dec * u.degree)
+    coords = SkyCoord(ra=ra * u.degree, dec=dec * u.degree)
     for radius in np.arange(1, 60, 1):
-        ids = SDSS.query_region(pos, radius=radius * u.arcsec, data_release=dr)
+        ids = SDSS.query_region(coords, radius=radius * u.arcsec, data_release=dr)
         if ids is not None:
             break
 
     if ids is None:
         return None
 
-    pointings_ra = ids["ra"].value
-    pointings_dec = ids["dec"].value
-    dist = np.sqrt(
-        (pointings_ra - ra) ** 2 * (np.cos(pointings_dec * np.pi / 180) ** 2)
-        + (pointings_dec - dec) ** 2
-    )
-
     # get the pointing closest to the given coordinates
-    pointing_id = np.argmin(dist)
-    ids2remove = list(np.arange(len(dist)))
+    coords_imgs = SkyCoord(ra=ids["ra"].value, dec=ids["dec"].value, unit=(u.degree, u.degree), frame="icrs")
+    separation = coords.separation(coords_imgs).value
+
+    pointing_id = np.argmin(separation)
+    ids2remove = list(np.arange(len(separation)))
     del ids2remove[pointing_id]
     ids.remove_rows(ids2remove)
 
     # download images here
     hdu_list = SDSS.get_images(matches=ids, band=filters, data_release=dr)
 
     # SDSS images are large so need to be trimmed
     for hdu in hdu_list:
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", AstropyWarning)
             img_wcs = wcs.WCS(hdu[0].header)
 
-        trimmed_data = Cutout2D(hdu[0].data, pos, size_pixels, img_wcs)
+        trimmed_data = Cutout2D(hdu[0].data, coords, size_pixels, img_wcs)
         hdu[0].data = trimmed_data.data
         hdu[0].header.update(trimmed_data.wcs.to_header())
 
     return hdu_list
 
 
 # GALEX
 # ----------------------------------------
-def get_img_dist(host_ra, host_dec, header):
-    """Obtains the distance from the image center
-    to the galaxy position.
-
-    Parameters
-    ----------
-    host_ra: str or float
-        Right ascension of the galaxy in degrees.
-    host_dec: str or float
-        Declination of the galaxy in degrees.
-    header: fits header
-        Header of an image.
-
-    Returns
-    -------
-    dist_from_center: float
-        Distance of from the image center to the galaxy
-        position in pixel units.
-    """
-    # coordinates of the image center
-    img_ra, img_dec = float(header["RA_CENT"]), float(header["DEC_CENT"])
-
-    # distance to the galaxy
-    dist_from_center = np.sqrt(
-        (img_ra - host_ra) ** 2 * (np.cos(img_dec * np.pi / 180) ** 2)
-        + (img_dec - host_dec) ** 2
-    )
-
-    return dist_from_center
-
-
 def get_GALEX_images(ra, dec, size=3, filters=None, version=None):
     """Downloads a set of GALEX fits images for a given set
     of coordinates and filters.
 
     Parameters
     ----------
     ra: str or float
@@ -502,24 +467,26 @@
             for file in files:
                 try:
                     hdu = fits.open(file)
                     hdu_list.append(hdu)
                 except:
                     pass
 
-            # calculate the distance of the galaxy to the image center
-            distances = []
+            # calculate the separation of the galaxy to the image center
+            separations = []
             for hdu in hdu_list:
-                header = hdu[0].header
-                dist_from_center = get_img_dist(ra, dec, header)
-                distances.append(dist_from_center)
+                ra_img = float(hdu[0].header["RA_CENT"])
+                dec_img = float(hdu[0].header["DEC_CENT"])
+                coords_img = SkyCoord(ra=ra_img, dec=dec_img, unit=(u.degree, u.degree), frame="icrs")
+                separation = coords.separation(coords_img).value
+                separations.append(separation)
 
             # get the image with the galaxy closest to the center
-            if len(distances) != 0:
-                id_file = np.argmin(np.array(distances))
+            if len(separations) != 0:
+                id_file = np.argmin(separations)
                 hdu = hdu_list[id_file]
             else:
                 hdu = None
 
             hdu_dict[filt] = hdu
 
     hdu_list = []
@@ -692,15 +659,15 @@
     base_url = "http://unwise.me/cutout_fits?"
     params_url = (
         f"version={version}&ra={ra}&dec={dec}&size={size_pixels}&bands={bands}"
     )
     master_url = base_url + params_url
 
     response = requests.get(master_url, stream=True)
-    target_file = "unWISE_images.tar.gz"  # current directory
+    target_file = f"unWISE_images_{ra}_{dec}.tar.gz"  # current directory
     if response.status_code == 200:
         with open(target_file, "wb") as f:
             f.write(response.raw.read())
 
     hdu_list = []
     with tarfile.open(target_file) as tar_file:
         files_list = tar_file.getnames()
@@ -708,15 +675,17 @@
             for filt in filters:
                 if f"{filt.lower()}-img-m.fits" in fits_file:
                     tar_file.extract(fits_file, ".")
                     hdu = fits.open(fits_file)
                     hdu_list.append(hdu)
                     os.remove(fits_file)
 
-    os.remove(target_file)
+    # sometimes, the file is not downloaded, so let's check if it exists
+    if os.path.isfile(target_file) is True:
+        os.remove(target_file)
 
     return hdu_list
 
 
 # 2MASS
 # ----------------------------------------
 def get_2MASS_images(ra, dec, size=3, filters=None):
@@ -766,275 +735,47 @@
 
         # for more info: https://irsa.ipac.caltech.edu/ibe/docs/twomass/allsky/allsky/#main
         base_url = (
             "https://irsa.ipac.caltech.edu/ibe/data/twomass/allsky/allsky"
         )
 
         hdu_list = []
-        for i, filt in enumerate(filters):
+        for filt in filters:
             if filt == "Ks":
                 filt = "K"
             band_df = twomass_df[twomass_df.band == filt]
             if len(band_df) == 0:
                 # no data for this band:
                 hdu_list.append(None)
                 continue
 
-            fname = band_df.download.values[0].split("=")[-1]
-            hemisphere = band_df.hem.values[0]
-            ordate = band_df.date.values[0]
-            scanno = band_df.scan.values[0]
+            # get image with the image's coordinates closest to the given coordinates
+            coords_imgs = SkyCoord(ra=band_df.center_ra.values, 
+                                   dec=band_df.center_dec.values, unit=(u.degree, u.degree), frame="icrs")
+            separation = coords.separation(coords_imgs).value
+            i = np.argmin(separation)
+
+            fname = band_df.download.values[i].split("=")[-1]
+            hemisphere = band_df.hem.values[i]
+            ordate = band_df.date.values[i]
+            scanno = band_df.scan.values[i]
             # add leading zeros for scanno bellow 100
             n_zeros = 3 - len(str(scanno))
             scanno = n_zeros * "0" + str(scanno)
 
             tile_url = os.path.join(f"{ordate}{hemisphere}", f"s{scanno}")
             fits_url = os.path.join("image", f"{fname}.gz")
             params_url = f"center={ra},{dec}&size={size_degree}degree&gzip=0"  # center and size of the image
 
             url = os.path.join(base_url, tile_url, fits_url + "?" + params_url)
             hdu = fits.open(url)
             hdu_list.append(hdu)
 
     return hdu_list
 
-
-# HST
-# ----------------------------------------
-def updated_HST_header(hdu):
-    """Updates the HST image header with the necessary keywords.
-
-    Parameters
-    ----------
-    hdu : Header Data Unit.
-        HST FITS image.
-    """
-    # get WCS
-    with warnings.catch_warnings():
-            warnings.simplefilter("ignore", AstropyWarning)
-            img_wcs = wcs.WCS(hdu[1].header)
-    hdu[0].header.update(img_wcs.to_header())
-    hdu[0].header['PHOTPLAM'] = hdu[1].header['PHOTPLAM']
-    hdu[0].data = hdu[1].data
-
-    # add zeropoints
-    # https://www.stsci.edu/hst/instrumentation/acs/data-analysis/zeropoints
-    photflam = hdu[0].header["PHOTFLAM"]
-    photplam = hdu[0].header["PHOTFLAM"]
-    hdu[0].header["MAGZP"] = (
-        -2.5 * np.log10(photflam) - 5 * np.log10(photplam) - 2.408
-    )
-
-
-def get_HST_images(ra, dec, size=3, filt=None, instrument=None):
-    """Downloads a set of HST fits images for a given set
-    of coordinates and filters using the MAST archive.
-
-    Parameters
-    ----------
-    ra: str or float
-        Right ascension in degrees.
-    dec: str or float
-        Declination in degrees.
-    size: float or ~astropy.units.Quantity, default ``3``
-        Image size. If a float is given, the units are assumed to be arcmin.
-    filt: str, default ``None``
-        Filter to use.
-    instrument: str, default ``None``
-        Instrument to use.
-
-    Return
-    ------
-    hdu_list: list
-        List with fits image for the given filter.
-        `None` is returned if no image is found.
-    """
-    global esahubble
-    esahubble.get_status_messages()
-    check_HST_inputs(filt, instrument)
-
-    if isinstance(size, (float, int)):
-        size_arcsec = (size * u.arcmin).to(u.arcsec)
-    else:
-        size_arcsec = size.to(u.arcsec)
-    size_arcsec = size_arcsec.value
-
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore", AstropyWarning)
-        coords = SkyCoord(
-            ra=ra, dec=dec, unit=(u.degree, u.degree), frame="icrs"
-        )
-
-    result = esahubble.cone_search_criteria(radius=3,
-                                        #obs_collection=['HST'],
-                                        coordinates=coords,
-                                        calibration_level='PRODUCT',
-                                        data_product_type = 'image',
-                                        instrument_name = instrument,
-                                        filters = filt,
-                                        async_job = True,
-                                       )
-
-    obs_df = result.to_pandas()
-    obs_df = obs_df[obs_df['filter']==filt]
-    # get only exposures shorter than one hour
-    obs_df = obs_df[obs_df.exposure_duration<3600]  
-    obs_df.sort_values(by=['exposure_duration'], 
-                       ascending=False, inplace=True) 
-
-    print('Looking for HST images...')
-    for obs_id in obs_df.observation_id:
-        try:
-            esahubble.download_product(observation_id=obs_id, 
-                                       product_type="SCIENCE", 
-                                       calibration_level="PRODUCT", 
-                                       filename='tmp')
-            break
-        except:
-            pass
-
-    if os.path.isfile('tmp.fits.gz') is False:
-        return None
-    
-    with zipfile.ZipFile('tmp.fits.gz', 'r') as zip_ref:
-        zip_ref.extractall('tmp')
-        fits_file = [file for file in glob.glob('tmp/**', recursive=True) 
-                     if file.endswith('.gz')][0]
-
-    hdu = fits.open(fits_file)
-    updated_HST_header(hdu)
-    
-    hdu_list = [hdu]
-
-    # remove the temporary files
-    os.remove("tmp.fits.gz") 
-    shutil.rmtree("tmp", ignore_errors=True)
-
-    # HST images can be large so need to be trimmed
-    pixel_scale = survey_pixel_scale('HST')
-    size_pixels = int(size_arcsec / pixel_scale)
-
-    for hdu in hdu_list:
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore", AstropyWarning)
-            img_wcs = wcs.WCS(hdu[0].header)
-
-        trimmed_data = Cutout2D(hdu[0].data, coords, size_pixels, img_wcs)
-        hdu[0].data = trimmed_data.data
-        hdu[0].header.update(trimmed_data.wcs.to_header())
-
-    return hdu_list
-
-def get_HST_images_(ra, dec, size=3, filt=None, instrument=None):
-    """Downloads a set of HST fits images for a given set
-    of coordinates and filters using the MAST archive.
-
-    Parameters
-    ----------
-    ra: str or float
-        Right ascension in degrees.
-    dec: str or float
-        Declination in degrees.
-    size: float or ~astropy.units.Quantity, default ``3``
-        Image size. If a float is given, the units are assumed to be arcmin.
-    filt: str, default ``None``
-        Filter to use.
-    instrument: str, default ``None``
-        Instrument to use.
-
-    Return
-    ------
-    hdu_list: list
-        List with fits image for the given filter.
-        `None` is returned if no image is found.
-    """
-    check_HST_inputs(filt, instrument)
-
-    if isinstance(size, (float, int)):
-        size_arcsec = (size * u.arcmin).to(u.arcsec)
-    else:
-        size_arcsec = size.to(u.arcsec)
-    size_arcsec = size_arcsec.value
-
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore", AstropyWarning)
-        coords = SkyCoord(
-            ra=ra, dec=dec, unit=(u.degree, u.degree), frame="icrs"
-        )
-
-    obs_table = Observations.query_region(coords, radius=size)
-    obs_table = obs_table.filled()  # remove masked rows
-    obs_df = obs_table.to_pandas()
-
-    obs_df = obs_df[
-        (obs_df.obs_collection == "HST") | (obs_df.obs_collection == "HLA")
-    ]
-    obs_df = obs_df[obs_df.dataproduct_type == "image"]
-    obs_df = obs_df[obs_df.t_exptime > 15]  # remove short exposures
-
-    # filter by instrument+filter
-    inst = instrument.split("/")[0]
-    # inst_df = obs_df[obs_df.instrument_name==instrument]
-    inst_df = obs_df[obs_df.instrument_name.str.contains(inst)]
-    filt_df = inst_df[inst_df.filters == filt]
-    # just use one image
-    filt_df = filt_df[filt_df.t_exptime == filt_df.t_exptime.max()]
-
-    # get data products
-    data_products = Observations.get_product_list(Table.from_pandas(filt_df))
-    dp_df = data_products.to_pandas()
-    dp_df = dp_df[dp_df.type == "S"]
-    dp_df = dp_df[dp_df.productSubGroupDescription == "FLT"]  # only images
-    # choose first image
-    single_dp_df = dp_df[dp_df.obs_id == dp_df.obs_id.values[0]]
-
-    Observations.download_products(
-        Table.from_pandas(single_dp_df),
-        download_dir=None,
-        cache=False,
-        productType="SCIENCE",
-        extension=["fits"],
-    )
-
-    for path, subdirs, files in os.walk("mastDownload"):
-        for file in files:
-            fits_file = os.path.join(path, file)
-
-    hdu = fits.open(fits_file)
-    hdu[0].data = hdu[1].data
-
-    # add zeropoints
-    # https://www.stsci.edu/hst/instrumentation/acs/data-analysis/zeropoints
-    photflam = hdu[0].header["PHOTFLAM"]
-    photplam = hdu[0].header["PHOTFLAM"]
-    hdu[0].header["MAGZP"] = (
-        -2.5 * np.log10(photflam) - 5 * np.log10(photplam) - 2.408
-    )
-    hdu_list = [hdu]
-
-    # remove directory created by MAST download
-    shutil.rmtree("mastDownload", ignore_errors=True)
-
-    # HST images can be large so need to be trimmed
-    pixel_scale = survey_pixel_scale('HST')
-    size_pixels = int(size_arcsec / pixel_scale)
-    pos = SkyCoord(ra=ra * u.degree, dec=dec * u.degree)
-
-    for hdu in hdu_list:
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore", AstropyWarning)
-            img_wcs = wcs.WCS(hdu[0].header)
-
-        trimmed_data = Cutout2D(hdu[0].data, pos, size_pixels, img_wcs)
-        hdu[0].data = trimmed_data.data
-        hdu[0].header.update(trimmed_data.wcs.to_header())
-
-    return hdu_list
-
-
 # Legacy Survey
 def get_LegacySurvey_images(ra, dec, size=3, filters=None, version="dr10"):
     """Gets Legacy Survey fits images for the given coordinates and
     filters.
 
     Parameters
     ----------
@@ -1261,14 +1002,298 @@
             hdu_list.append(hdu[1])  # extension 1
         else:
             hdu_list.append(None)
 
     return hdu_list
 
 
+# HST
+# ----------------------------------------
+def update_HST_header(hdu):
+    """Updates the HST image header with the necessary keywords.
+
+    Parameters
+    ----------
+    hdu : Header Data Unit.
+        HST FITS image.
+    """
+    # get WCS
+    with warnings.catch_warnings():
+            warnings.simplefilter("ignore", AstropyWarning)
+            for i in range(1, len(hdu)-1):
+                try:
+                    img_wcs = wcs.WCS(hdu[i].header)
+                except:
+                    continue
+    hdu[0].header.update(img_wcs.to_header())
+    hdu[0].header['PHOTFLAM'] = hdu[1].header['PHOTFLAM']
+    hdu[0].header['PHOTPLAM'] = hdu[1].header['PHOTPLAM']
+    hdu[0].data = hdu[1].data
+
+    # add zeropoints
+    # https://www.stsci.edu/hst/instrumentation/acs/data-analysis/zeropoints
+    photflam = hdu[0].header["PHOTFLAM"]
+    photplam = hdu[0].header["PHOTPLAM"]
+    hdu[0].header["MAGZP"] = (
+        -2.5 * np.log10(photflam) - 5 * np.log10(photplam) - 2.408
+    )
+
+def set_HST_image(file, filt, name):
+    """Moves a previously downloaded HST image into the work directory.
+
+    The image's header is updated with the necessary keywords to obtain
+    photometry and is also moved under the objects directory inside the 
+    work directory.
+
+    HST images take very long to download, so the user might prefer to
+    download the images manually and then use this function to include
+    the image into the workflow.
+
+    Parameters
+    ----------
+    file : str
+        HST image to use.
+    filt : str
+        HST filter, e.g. ``WFC3_UVIS_F275W``.
+    name : str
+        Object's name.
+    """
+    check_work_dir(workdir)
+    obj_dir = os.path.join(workdir, name)
+    if not os.path.isdir(obj_dir):
+        os.mkdir(obj_dir)
+
+    hdu = fits.open(file)
+    update_HST_header(hdu)
+    outfile = os.path.join(obj_dir, f'HST_{filt}.fits')
+    hdu.writeto(outfile, overwrite=True)
+
+def get_HST_images(ra, dec, size=3, filt=None):
+    """Downloads a set of HST fits images for a given set
+    of coordinates and filters using the MAST archive.
+
+    Parameters
+    ----------
+    ra: str or float
+        Right ascension in degrees.
+    dec: str or float
+        Declination in degrees.
+    size: float or ~astropy.units.Quantity, default ``3``
+        Image size. If a float is given, the units are assumed to be arcmin.
+    filt: str, default ``None``
+        Filter to use, e.g. ``WFC3_UVIS_F225W``.
+
+    Return
+    ------
+    hdu_list: list
+        List with fits image for the given filter.
+        `None` is returned if no image is found.
+    """
+    global esahubble
+    esahubble.get_status_messages()
+    check_HST_filters(filt)
+
+    # separate the instrument name from the actual filter
+    split_filt = filt.split('_')
+    if len(split_filt)==2:
+        filt = split_filt[-1]
+        instrument = split_filt[0]
+    elif len(split_filt)==3:
+        filt = split_filt[-1]
+        instrument = f'{split_filt[0]}/{split_filt[1]}'
+    else:
+        raise ValueError(f"Incorrect filter name: {filt}")
+
+    if isinstance(size, (float, int)):
+        size_arcsec = (size * u.arcmin).to(u.arcsec)
+    else:
+        size_arcsec = size.to(u.arcsec)
+    size_arcsec = size_arcsec.value
+
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore", AstropyWarning)
+        coords = SkyCoord(
+            ra=ra, dec=dec, unit=(u.degree, u.degree), frame="icrs"
+        )
+
+    version = None
+    if version=='HLA':
+        # This does not seem to be faster
+        fov = 0.2   # field-of-view win degrees
+        access_url = " https://hla.stsci.edu/cgi-bin/hlaSIAP.cgi"
+        svc = sia.SIAService(access_url)
+        imgs_table = svc.search(
+            (ra, dec), (fov / np.cos(dec * np.pi / 180), fov), verbosity=2
+        )
+
+        obs_df = pd.DataFrame(imgs_table)
+        obs_df = obs_df[obs_df.Mode=='IMAGE']
+        obs_df = obs_df[obs_df.Format.str.endswith('fits')]
+        obs_df = obs_df[obs_df.Detector==instrument]
+        obs_df = obs_df[obs_df.Spectral_Elt==filt]
+        obs_df = obs_df[obs_df.ExpTime==obs_df.ExpTime.max()]
+        
+        hdu = fits.open(obs_df.URL.values[0])
+    else:
+        result = esahubble.cone_search_criteria(radius=3,
+                                                coordinates=coords,
+                                                calibration_level='PRODUCT',
+                                                data_product_type = 'image',
+                                                instrument_name = instrument,
+                                                filters = filt,
+                                                async_job = True,
+                                            )
+        
+        obs_df = result.to_pandas()
+        obs_df = obs_df[obs_df['filter']==filt]
+        # get only exposures shorter than one hour
+        obs_df = obs_df[obs_df.exposure_duration<3600]  
+        obs_df.sort_values(by=['exposure_duration'], 
+                        ascending=False, inplace=True) 
+
+        print('Looking for HST images...')
+        filename = f'HST_tmp_{ra}_{dec}'  # the extension is added below
+        for obs_id in obs_df.observation_id:
+            try:
+                esahubble.download_product(observation_id=obs_id, 
+                                        product_type="SCIENCE", 
+                                        calibration_level="PRODUCT", 
+                                        filename=filename)
+                break
+            except:
+                pass
+
+        temp_file = f'{filename}.fits.gz'
+        if os.path.isfile(temp_file) is False:
+            return None
+        
+        temp_dir = filename # same name as the extension-less file above
+        with zipfile.ZipFile(temp_file, 'r') as zip_ref:
+            zip_ref.extractall(temp_dir)
+            fits_file = [file for file in glob.glob(f'{temp_dir}/**', recursive=True) 
+                        if file.endswith('.gz')][0]
+
+        hdu = fits.open(fits_file)    
+
+        # remove the temporary files and directory
+        os.remove(temp_file) 
+        shutil.rmtree(temp_dir, ignore_errors=True)
+
+    update_HST_header(hdu)
+    hdu_list = [hdu]
+    
+    return hdu_list
+
+def get_HST_images_OLD(ra, dec, size=3, filt=None, instrument=None):
+    """Downloads a set of HST fits images for a given set
+    of coordinates and filters using the MAST archive.
+
+    Parameters
+    ----------
+    ra: str or float
+        Right ascension in degrees.
+    dec: str or float
+        Declination in degrees.
+    size: float or ~astropy.units.Quantity, default ``3``
+        Image size. If a float is given, the units are assumed to be arcmin.
+    filt: str, default ``None``
+        Filter to use.
+    instrument: str, default ``None``
+        Instrument to use.
+
+    Return
+    ------
+    hdu_list: list
+        List with fits image for the given filter.
+        `None` is returned if no image is found.
+    """
+    check_HST_filters(filt, instrument)
+
+    if isinstance(size, (float, int)):
+        size_arcsec = (size * u.arcmin).to(u.arcsec)
+    else:
+        size_arcsec = size.to(u.arcsec)
+    size_arcsec = size_arcsec.value
+
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore", AstropyWarning)
+        coords = SkyCoord(
+            ra=ra, dec=dec, unit=(u.degree, u.degree), frame="icrs"
+        )
+
+    obs_table = Observations.query_region(coords, radius=size)
+    obs_table = obs_table.filled()  # remove masked rows
+    obs_df = obs_table.to_pandas()
+
+    obs_df = obs_df[
+        (obs_df.obs_collection == "HST") | (obs_df.obs_collection == "HLA")
+    ]
+    obs_df = obs_df[obs_df.dataproduct_type == "image"]
+    obs_df = obs_df[obs_df.t_exptime > 15]  # remove short exposures
+
+    # filter by instrument+filter
+    inst = instrument.split("/")[0]
+    # inst_df = obs_df[obs_df.instrument_name==instrument]
+    inst_df = obs_df[obs_df.instrument_name.str.contains(inst)]
+    filt_df = inst_df[inst_df.filters == filt]
+    # just use one image
+    filt_df = filt_df[filt_df.t_exptime == filt_df.t_exptime.max()]
+
+    # get data products
+    data_products = Observations.get_product_list(Table.from_pandas(filt_df))
+    dp_df = data_products.to_pandas()
+    dp_df = dp_df[dp_df.type == "S"]
+    dp_df = dp_df[dp_df.productSubGroupDescription == "FLT"]  # only images
+    # choose first image
+    single_dp_df = dp_df[dp_df.obs_id == dp_df.obs_id.values[0]]
+
+    Observations.download_products(
+        Table.from_pandas(single_dp_df),
+        download_dir=None,
+        cache=False,
+        productType="SCIENCE",
+        extension=["fits"],
+    )
+
+    for path, subdirs, files in os.walk("mastDownload"):
+        for file in files:
+            fits_file = os.path.join(path, file)
+
+    hdu = fits.open(fits_file)
+    hdu[0].data = hdu[1].data
+
+    # add zeropoints
+    # https://www.stsci.edu/hst/instrumentation/acs/data-analysis/zeropoints
+    photflam = hdu[0].header["PHOTFLAM"]
+    photplam = hdu[0].header["PHOTFLAM"]
+    hdu[0].header["MAGZP"] = (
+        -2.5 * np.log10(photflam) - 5 * np.log10(photplam) - 2.408
+    )
+    hdu_list = [hdu]
+
+    # remove directory created by MAST download
+    shutil.rmtree("mastDownload", ignore_errors=True)
+
+    # HST images can be large so need to be trimmed
+    pixel_scale = survey_pixel_scale('HST')
+    size_pixels = int(size_arcsec / pixel_scale)
+    pos = SkyCoord(ra=ra * u.degree, dec=dec * u.degree)
+
+    for hdu in hdu_list:
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore", AstropyWarning)
+            img_wcs = wcs.WCS(hdu[0].header)
+
+        trimmed_data = Cutout2D(hdu[0].data, pos, size_pixels, img_wcs)
+        hdu[0].data = trimmed_data.data
+        hdu[0].header.update(trimmed_data.wcs.to_header())
+
+    return hdu_list
+
+
 # Check orientation
 # ------------------
 def match_wcs(fits_files):
     """Matches the WCS of all the images, taking the first ones as
     a reference.
 
     Parameters
@@ -1363,27 +1388,27 @@
     elif survey == "WISE":
         hdu_list = get_WISE_images(ra, dec, size, filters)
     elif survey == "unWISE":
         hdu_list = get_unWISE_images(ra, dec, size, filters, version)
     elif survey == "2MASS":
         hdu_list = get_2MASS_images(ra, dec, size, filters)
     elif survey == "HST":
-        hdu_list = get_HST_images(ra, dec, size, filters, version)
+        hdu_list = get_HST_images(ra, dec, size, filters)
     elif survey == "LegacySurvey":
         hdu_list = get_LegacySurvey_images(ra, dec, size, filters, version)
     elif survey == "Spitzer":
         hdu_list = get_Spitzer_images(ra, dec, size, filters)
     elif survey == "VISTA":
         hdu_list = get_VISTA_images(ra, dec, size, filters, version)
     else:
         raise ValueError(
             "The given survey is not properly added to HostPhot..."
         )
     
-    if filters is None and survey != 'HST':
+    if filters is None:
         filters = get_survey_filters(survey)
 
     if hdu_list:
         for hdu, filt in zip(hdu_list, filters):
             if hdu is None:
                 continue  # skip missing filter/image
```

### Comparing `hostphot-2.5.1/src/hostphot/dust.py` & `hostphot-2.6.0/src/hostphot/dust.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from sfdmap2 import sfdmap
 import extinction
 from astropy.coordinates import SkyCoord
 from astropy import units as u
 
 import hostphot
-from .utils import integrate_filter, get_survey_filters, extract_filters
+from .utils import integrate_filter, extract_filter
 
 import warnings
 
 
 def _download_dustmaps():
     """Downloads the dust maps for extinction calculation if they are not found
     locally.
@@ -73,15 +73,15 @@
         Declination in degrees.
     scaling: float, default ``0.86``
         Calibration of the Milky Way dust maps. Either ``0.86``
         for the Schlafly & Finkbeiner (2011) recalibration or ``1.0`` for the original
         dust map of Schlegel, Fikbeiner & Davis (1998).
     reddening_law: str, default ``fitzpatrick99``
         Reddening law. The options are: ``ccm89`` (Cardelli, Clayton & Mathis 1989),
-        ``odonnell94`` (O’Donnell 1994), ``fitzpatrick99`` (Fitzpatrick 1999), ``calzetti00``
+        ``odonnell94`` (O'Donnell 1994), ``fitzpatrick99`` (Fitzpatrick 1999), ``calzetti00``
         (Calzetti 2000) and ``fm07`` (Fitzpatrick & Massa 2007 with :math:`R_V` = 3.1.)
     dustmaps_dir : str, default ``None``
         Directory where the dust maps of Schlegel, Fikbeiner & Davis (1998) are found.
     r_v : float, default ``3.1``
         Total-to-selective extinction ratio (:math:`R_V`)
     ebv : float, default ``None``
         Colour excess (:math:`E(B-V)`). If given, this is used instead of the dust map value.
@@ -141,43 +141,39 @@
         Declinationin degrees.
     scaling: float, default ``0.86``
         Calibration of the Milky Way dust maps. Either ``0.86``
         for the Schlafly & Finkbeiner (2011) recalibration or ``1.0`` for the original
         dust map of Schlegel, Fikbeiner & Davis (1998).
     reddening_law: str, default ``fitzpatrick99``
         Reddening law. The options are: ``ccm89`` (Cardelli, Clayton & Mathis 1989),
-        ``odonnell94`` (O’Donnell 1994), ``fitzpatrick99`` (Fitzpatrick 1999), ``calzetti00``
+        ``odonnell94`` (O'Donnell 1994), ``fitzpatrick99`` (Fitzpatrick 1999), ``calzetti00``
         (Calzetti 2000) and ``fm07`` (Fitzpatrick & Massa 2007 with :math:`R_V` = 3.1.)
     r_v : float, default ``3.1``
         Total-to-selective extinction ratio (:math:`R_V`)
 
     Returns
     -------
     A_ext : float
         Extinction value in magnitudes.
     """
-    # extract transmission function for the given filter+survey
-    filters = get_survey_filters(survey)
     if survey == "LegacySurvey":
         # https://datalab.noirlab.edu/ls/bass.php
         # declination above ~32 and above the galactic plane
         gal_coords = SkyCoord(
             ra=ra * u.degree, dec=dec * u.degree, frame="icrs"
         )
         if (dec > 32.375) and (gal_coords.b.value > 0):
             version = "BASS+MzLS"
         else:
             version = "DECam"
     else:
         version = None
 
-    filters_dict = extract_filters(filters, survey, version)
-
-    filter_wave = filters_dict[filt]["wave"]
-    filter_response = filters_dict[filt]["transmission"]
+    # extract transmission function for the given filter+survey
+    filter_wave, filter_response = extract_filter(filt, survey, version)
 
     # calculate extinction
     flux = 100
     dereddened_flux = deredden(
         filter_wave, flux, ra, dec, scaling, reddening_law, r_v
     )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hostphot-2.5.1/src/hostphot/filters/2MASS/2MASS_H.dat` & `hostphot-2.6.0/src/hostphot/filters/2MASS/2MASS_H.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/2MASS/2MASS_J.dat` & `hostphot-2.6.0/src/hostphot/filters/2MASS/2MASS_J.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/2MASS/2MASS_Ks.dat` & `hostphot-2.6.0/src/hostphot/filters/2MASS/2MASS_Ks.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/AAA_README` & `hostphot-2.6.0/src/hostphot/filters/AAA_README`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/DES/DES_Y.dat` & `hostphot-2.6.0/src/hostphot/filters/DES/DES_Y.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/DES/DES_g.dat` & `hostphot-2.6.0/src/hostphot/filters/DES/DES_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/DES/DES_i.dat` & `hostphot-2.6.0/src/hostphot/filters/DES/DES_i.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/DES/DES_r.dat` & `hostphot-2.6.0/src/hostphot/filters/DES/DES_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/DES/DES_z.dat` & `hostphot-2.6.0/src/hostphot/filters/DES/DES_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/GALEX/GALEX_FUV.dat` & `hostphot-2.6.0/src/hostphot/filters/GALEX/GALEX_FUV.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/GALEX/GALEX_NUV.dat` & `hostphot-2.6.0/src/hostphot/filters/GALEX/GALEX_NUV.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F435W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F435W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F475W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F475W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F502N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F502N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F550M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F550M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F555W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F555W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F606W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F606W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F625W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F625W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F658N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F658N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F660N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F660N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F775W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F775W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F814W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F814W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F850LP.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F850LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F892N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F892N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR1016N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR1016N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR388N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR388N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR423N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR423N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR459M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR459M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR462N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR462N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR505N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR505N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR551N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR551N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR601N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR601N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR647M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR647M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR656N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR656N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR716N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR716N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR782N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR782N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR853N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR853N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR914M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR914M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR931N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/ACS_WFC/ACS_WFC_FR931N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F090M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F090M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F095N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F095N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F097N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F097N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F108N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F108N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F110W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F113N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F113N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F140W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F140W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F145M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F145M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F160W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F160W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F164N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F164N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F165M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F165M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F166N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F166N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F170M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F170M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F187N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F187N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS1/NICMOS1_F190N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS1/NICMOS1_F190N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F110W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F110W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F160W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F160W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F165M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F165M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F171M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F171M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F180M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F180M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F187W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F190N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F190N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F204M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F204M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F205W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F205W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F207M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F207M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F212N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F212N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F215N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F215N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F216N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F216N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F222M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F222M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS2/NICMOS2_F237M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS2/NICMOS2_F237M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F108N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F108N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F110W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F110W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F113N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F113N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F150W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F150W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F160W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F160W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F164N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F164N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F166N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F166N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F175W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F175W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F187N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F187N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F190N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F190N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F196N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F196N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F200N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F200N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F212N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F212N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F215N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F215N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F222M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F222M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/NICMOS3/NICMOS3_F240M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/NICMOS3/NICMOS3_F240M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F098M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F098M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F105W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F105W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F110W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F110W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F125W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F125W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F126N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F126N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F127M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F127M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F128N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F128N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F130N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F130N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F132N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F132N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F139M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F139M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F140W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F140W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F153M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F153M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F160W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F160W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F164N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F164N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F167N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_IR/WFC3_IR_F167N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F200LP.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F200LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F218W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F218W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F225W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F225W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F275W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F275W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F280N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F280N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F300X.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F300X.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F336W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F336W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F343N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F343N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F350LP.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F350LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F373N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F373N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F390W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F395N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F395N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F410M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F410M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F438W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F438W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F467M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F467M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F469N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F469N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475X.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F475X.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F487N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F487N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F502N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F502N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F547M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F547M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F555W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F555W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F600LP.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F600LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F606W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F606W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F621M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F621M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F625W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F625W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F631N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F631N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F645N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F645N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F656N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F656N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F657N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F657N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F658N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F658N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F665N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F665N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F673N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F673N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F680N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F680N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F689M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F689M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F763M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F763M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F775W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F775W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F814W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F814W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F845M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F845M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F850LP.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F850LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F953N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_F953N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ232N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ232N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ243N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ243N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ378N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ378N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ387N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ387N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ422M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ422M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ436N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ436N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ437N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ437N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ492N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ492N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ508N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ508N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ575N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ575N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ619N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ619N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ634N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ634N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ672N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ672N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ674N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ674N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ727N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ727N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ750N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ750N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ889N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ889N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ906N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ906N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ924N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ924N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ937N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS1/WFC3_UVIS1_FQ937N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F200LP.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F200LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F218W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F218W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F225W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F225W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F275W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F275W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F280N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F280N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F300X.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F300X.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F336W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F336W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F343N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F343N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F350LP.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F350LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F373N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F373N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F390W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F395N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F395N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F410M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F410M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F438W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F438W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F467M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F467M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F469N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F469N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475X.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F475X.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F487N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F487N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F502N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F502N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F547M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F547M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F555W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F555W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F600LP.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F600LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F606W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F606W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F621M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F621M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F625W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F625W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F631N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F631N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F645N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F645N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F656N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F656N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F657N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F657N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F658N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F658N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F665N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F665N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F673N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F673N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F680N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F680N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F689M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F689M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F763M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F763M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F775W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F775W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F814W.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F814W.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F845M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F845M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F850LP.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F850LP.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F953N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_F953N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ232N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ232N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ243N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ243N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ378N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ378N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ387N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ387N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ422M.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ422M.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ436N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ436N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ437N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ437N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ492N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ492N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ508N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ508N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ575N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ575N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ619N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ619N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ634N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ634N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ672N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ672N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ674N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ674N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ727N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ727N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ750N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ750N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ889N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ889N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ906N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ906N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ924N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ924N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ937N.dat` & `hostphot-2.6.0/src/hostphot/filters/HST/WFC3_UVIS2/WFC3_UVIS2_FQ937N.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/LegacySurvey/BASS_g.dat` & `hostphot-2.6.0/src/hostphot/filters/LegacySurvey/BASS_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/LegacySurvey/BASS_r.dat` & `hostphot-2.6.0/src/hostphot/filters/LegacySurvey/BASS_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/LegacySurvey/DECAM_g.dat` & `hostphot-2.6.0/src/hostphot/filters/LegacySurvey/DECAM_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/LegacySurvey/DECAM_r.dat` & `hostphot-2.6.0/src/hostphot/filters/LegacySurvey/DECAM_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/LegacySurvey/DECAM_z.dat` & `hostphot-2.6.0/src/hostphot/filters/LegacySurvey/DECAM_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/LegacySurvey/MzLS_z.dat` & `hostphot-2.6.0/src/hostphot/filters/LegacySurvey/MzLS_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/LegacySurvey/init_BASS_g.dat` & `hostphot-2.6.0/src/hostphot/filters/LegacySurvey/init_BASS_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/LegacySurvey/init_BASS_r.dat` & `hostphot-2.6.0/src/hostphot/filters/LegacySurvey/init_BASS_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/PS1/PS1_g.dat` & `hostphot-2.6.0/src/hostphot/filters/PS1/PS1_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/PS1/PS1_i.dat` & `hostphot-2.6.0/src/hostphot/filters/PS1/PS1_i.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/PS1/PS1_r.dat` & `hostphot-2.6.0/src/hostphot/filters/PS1/PS1_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/PS1/PS1_y.dat` & `hostphot-2.6.0/src/hostphot/filters/PS1/PS1_y.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/PS1/PS1_z.dat` & `hostphot-2.6.0/src/hostphot/filters/PS1/PS1_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/SDSS/SDSS_g.dat` & `hostphot-2.6.0/src/hostphot/filters/SDSS/SDSS_g.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/SDSS/SDSS_i.dat` & `hostphot-2.6.0/src/hostphot/filters/SDSS/SDSS_i.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/SDSS/SDSS_r.dat` & `hostphot-2.6.0/src/hostphot/filters/SDSS/SDSS_r.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/SDSS/SDSS_u.dat` & `hostphot-2.6.0/src/hostphot/filters/SDSS/SDSS_u.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/SDSS/SDSS_z.dat` & `hostphot-2.6.0/src/hostphot/filters/SDSS/SDSS_z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.1.dat` & `hostphot-2.6.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.1.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.2.dat` & `hostphot-2.6.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.2.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.3.dat` & `hostphot-2.6.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.3.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/Spitzer/Spitzer_IRAC.4.dat` & `hostphot-2.6.0/src/hostphot/filters/Spitzer/Spitzer_IRAC.4.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/Spitzer/Spitzer_MIPS.1.dat` & `hostphot-2.6.0/src/hostphot/filters/Spitzer/Spitzer_MIPS.1.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/VISTA/VISTA_H.dat` & `hostphot-2.6.0/src/hostphot/filters/VISTA/VISTA_H.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/VISTA/VISTA_J.dat` & `hostphot-2.6.0/src/hostphot/filters/VISTA/VISTA_J.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/VISTA/VISTA_Ks.dat` & `hostphot-2.6.0/src/hostphot/filters/VISTA/VISTA_Ks.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/VISTA/VISTA_Y.dat` & `hostphot-2.6.0/src/hostphot/filters/VISTA/VISTA_Y.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/VISTA/VISTA_Z.dat` & `hostphot-2.6.0/src/hostphot/filters/VISTA/VISTA_Z.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/WISE/WISE_W1.dat` & `hostphot-2.6.0/src/hostphot/filters/WISE/WISE_W1.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/WISE/WISE_W2.dat` & `hostphot-2.6.0/src/hostphot/filters/WISE/WISE_W2.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/WISE/WISE_W3.dat` & `hostphot-2.6.0/src/hostphot/filters/WISE/WISE_W3.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/WISE/WISE_W4.dat` & `hostphot-2.6.0/src/hostphot/filters/WISE/WISE_W4.dat`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/filters/config.txt` & `hostphot-2.6.0/src/hostphot/filters/config.txt`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/global_photometry.py` & `hostphot-2.6.0/src/hostphot/global_photometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,18 +25,16 @@
 
 from hostphot._constants import workdir
 from hostphot.utils import (
     get_survey_filters,
     check_survey_validity,
     check_filters_validity,
     get_image_gain,
-    pixel2pixel,
     check_work_dir,
     magnitude_calculation,
-    survey_pixel_scale,
     adapt_aperture,
     bkg_surveys,
 )
 from hostphot.objects_detect import extract_objects, plot_detected_objects
 from hostphot.image_cleaning import remove_nan
 from hostphot.dust import calc_extinction
 
@@ -210,16 +208,18 @@
         Filter to use to load the fits file. List is commonly used for coadds.
     survey: str
         Survey to use for the zero-points and pixel scale.
     ra: float, default ``None``
        Right ascension of an object, in degrees. Used for plotting the position of the object.
     dec: float, default ``None``
        Declination of an object, in degrees. Used for plotting the position of the object.
-    bkg_sub: bool, default `False`
-        If `True`, the image gets background subtracted.
+    bkg_sub: bool, default `None`
+        If `True`, the image gets background subtracted. By default, only
+        the images that need it get background subtracted (WISE, 2MASS and
+        VISTA).
     threshold: float, default `10`
         Threshold used by `sep.extract()` to extract objects.
     use_mask: bool, default `True`
         If `True`, the masked fits files are used. These must have
         been created beforehand.
     optimize_kronrad: bool, default `True`
         If `True`, the Kron radius is optimized, increasing the
@@ -492,15 +492,15 @@
             flux, flux_err = kron_flux(
                 data_sub, bkg_rms, gain, gal_obj, kronrad, scale
             )
             flux, flux_err = flux[0], flux_err[0]
 
     ap_area = np.pi * gal_obj["a"][0] * gal_obj["b"][0]
 
-    mag, mag_err, total_flux_err = magnitude_calculation(
+    mag, mag_err, flux, flux_err = magnitude_calculation(
         flux,
         flux_err,
         survey,
         filt,
         ap_area,
         header,
         bkg_rms,
@@ -512,15 +512,15 @@
 
     if save_plots is True:
         outfile = os.path.join(obj_dir, f"global_{survey}_{filt}.jpg")
         plot_detected_objects(
             data_sub, gal_obj, scale * kronrad, img_wcs, ra, dec, outfile
         )
 
-    return mag, mag_err, flux, total_flux_err
+    return mag, mag_err, flux, flux_err
 
 
 def multi_band_phot(
     name,
     host_ra,
     host_dec,
     filters=None,
@@ -616,17 +616,21 @@
     >>> results = gp.multi_band_phot(name, host_ra, host_dec,
                             survey=survey, ra=ra, dec=dec,
                             use_mask=True, common_aperture=True,
                             coadd_filters='riz', save_plots=True)
     """
     check_survey_validity(survey)
     if filters is None:
+        if survey=='HST':
+            raise ValueError("For HST, the filter needs to be specified!")
         filters = get_survey_filters(survey)
     else:
         check_filters_validity(filters, survey)
+    if survey=='HST':
+        filters = [filters]
 
     results_dict = {
         "name": name,
         "host_ra": host_ra,
         "host_dec": host_dec,
         "survey": survey,
     }
```

### Comparing `hostphot-2.5.1/src/hostphot/image_cleaning.py` & `hostphot-2.6.0/src/hostphot/image_cleaning.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/image_masking.py` & `hostphot-2.6.0/src/hostphot/image_masking.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/interactive_aperture.py` & `hostphot-2.6.0/src/hostphot/interactive_aperture.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/local_photometry.py` & `hostphot-2.6.0/src/hostphot/local_photometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,15 +273,15 @@
         radius_pix = radius_arcsec / pixel_scale
 
         flux, flux_err = extract_aperture_flux(
             data_sub, error, px, py, radius_pix
         )
 
         ap_area = 2 * np.pi * (radius_pix**2)
-        mag, mag_err, total_flux_error = magnitude_calculation(
+        mag, mag_err, flux, flux_err = magnitude_calculation(
             flux,
             flux_err,
             survey,
             filt,
             ap_area,
             header,
             bkg_rms,
@@ -291,15 +291,15 @@
         if correct_extinction:
             A_ext = calc_extinction(filt, survey, ra, dec)
             mag -= A_ext
 
         mags.append(mag)
         mags_err.append(mag_err)
         fluxes.append(flux)
-        fluxes_err.append(total_flux_error)
+        fluxes_err.append(flux_err)
 
         if save_plots:
             outfile = os.path.join(
                 obj_dir, f"local_{survey}_{filt}_{ap_radius}kpc.jpg"
             )
             plot_aperture(data_sub, px, py, radius_pix, img_wcs, outfile)
 
@@ -372,30 +372,34 @@
     >>> survey = 'PS1'
     >>> results = lp.multi_band_phot(name, ra, dec, z,
                             survey=survey, ap_radii=ap_radii,
                             use_mask=True, save_plots=True)
     """
     check_survey_validity(survey)
     if filters is None:
+        if survey=='HST':
+            raise ValueError("For HST, the filter needs to be specified!")
         filters = get_survey_filters(survey)
     else:
         check_filters_validity(filters, survey)
+    if survey=='HST':
+        filters = [filters]
 
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

### Comparing `hostphot-2.5.1/src/hostphot/objects_detect.py` & `hostphot-2.6.0/src/hostphot/objects_detect.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/rgb_images.py` & `hostphot-2.6.0/src/hostphot/rgb_images.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/src/hostphot/utils.py` & `hostphot-2.6.0/src/hostphot/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import glob
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 
 from astropy import wcs
 from astropy.io import fits
 from astropy.stats import sigma_clipped_stats
@@ -15,16 +16,15 @@
 import hostphot
 
 hostphot_path = hostphot.__path__[0]
 config_file = os.path.join(hostphot_path, "filters", "config.txt")
 config_df = pd.read_csv(config_file, delim_whitespace=True)
 
 # surveys that need background subtraction
-bkg_surveys = ["2MASS", "WISE", "VISTA"]
-
+bkg_surveys = ['2MASS', 'WISE', 'VISTA']
 
 def calc_sky_unc(image, exptime):
     """Calculates the uncertainty of the image from the
     sky standard deviation, sigma-clipped STD.
 
     Parameters
     ----------
@@ -56,36 +56,40 @@
 def check_survey_validity(survey):
     """Check whether the given survey is whithin the valid
     options.
 
     Parameters
     ----------
     survey: str
-        Survey name: ``PS1``, ``DES``, ``SDSS``, ``GALEX``, ``WISE``, ``2MASS``.
+        Survey name: e.g. ``PS1``, ``GALEX``.
     """
     global config_df
     surveys = list(config_df.survey)
-    assert survey in surveys, f"survey '{survey}' not" f" in {surveys}"
+    assert survey in surveys, f"Survey '{survey}' not in {surveys}"
 
 
 def get_survey_filters(survey):
     """Gets all the valid filters for the given survey.
 
     Parameters
     ----------
     survey: str
-        Survey name: ``PS1``, ``DES``, ``SDSS``, ``GALEX``, ``WISE``, ``2MASS``.
+        Survey name: e.g. ``PS1``, ``GALEX``.
 
     Returns
     -------
     filters: str
         Filters for the given survey.
     """
     check_survey_validity(survey)
 
+    if survey=='HST':
+        # For HST, the filter needs to be specified
+        return None
+
     global config_df
     survey_df = config_df[config_df.survey == survey]
     filters = survey_df.filters.values[0]
 
     if "," in filters:
         filters = filters.split(",")
 
@@ -97,15 +101,15 @@
 
     **Note:** for ``PS1``, an extra :math:`+2.5*np.log10(exptime)`
     needs to be added afterwards.
 
     Parameters
     ----------
     survey: str
-        Survey name: ``PS1``, ``DES``, ``SDSS``, ``GALEX``, ``WISE``, ``2MASS``.
+        Survey name: e.g. ``PS1``, ``GALEX``.
 
     Returns
     -------
     zp_dict: dict or str
         Zero-points for all the filters in the given survey. If the survey zero-point
         is different for each image, the string ``header`` is returned.
     """
@@ -118,20 +122,20 @@
 
     if zps == "header":
         return zps
 
     if "," in zps:
         zps = zps.split(",")
         zp_dict = {filt: float(zp) for filt, zp in zip(filters, zps)}
-    elif survey == "SDSS":
+    elif survey=='SDSS':
         # SDSS zero-points are not exactly in AB:
         # https://www.sdss4.org/dr12/algorithms/fluxcal/#SDSStoAB
         zp_dict = {filt: float(zps) for filt in filters}
-        zp_dict["u"] -= 0.04
-        zp_dict["z"] += 0.02
+        zp_dict['u'] -= 0.04
+        zp_dict['z'] += 0.02
     else:
         zp_dict = {filt: float(zps) for filt in filters}
 
     return zp_dict
 
 
 def get_image_gain(header, survey):
@@ -141,15 +145,15 @@
     as it should already be included.
 
     Parameters
     ----------
     header: fits header
         Header of an image.
     survey: str
-        Survey name: ``PS1``, ``DES``, ``SDSS``, ``GALEX``, ``WISE``, ``2MASS``.
+        Survey name: e.g. ``PS1``, ``GALEX``.
 
     Returns
     -------
     gain: float
         Gain value.
     """
     check_survey_validity(survey)
@@ -174,14 +178,16 @@
             gain *= header["EFCONV"]  # convert DN/s to MJy/sr
         elif header["INSTRUME"] == "MIPS":
             # Table 2.4 of MIPS Instrument Handbook
             gain = 5.0
     elif survey == "VISTA":
         # use median from http://casu.ast.cam.ac.uk/surveys-projects/vista/technical/vista-gain
         gain = 4.19
+    elif survey=='HST':
+        gain = header['CCDGAIN']
     else:
         gain = 1.0
 
     return gain
 
 
 def get_image_readnoise(header, survey):
@@ -192,15 +198,15 @@
     as it should already be included.
 
     Parameters
     ----------
     header: fits header
         Header of an image.
     survey: str
-        Survey name: ``PS1``, ``DES``, ``SDSS``, ``GALEX``, ``WISE``, ``2MASS``.
+        Survey name: e.g. ``PS1``, ``GALEX``.
 
     Returns
     -------
     readnoise: float
         Read noise value.
     """
     check_survey_validity(survey)
@@ -227,37 +233,40 @@
         elif header["INSTRUME"] == "MIPS":
             # Table 2.4 of MIPS Instrument Handbook
             readnoise = 40.0
     elif survey == "VISTA":
         # very rough average for all filters in
         # http://casu.ast.cam.ac.uk/surveys-projects/vista/technical/vista-gain
         readnoise = 24.0
+    elif survey=='HST':
+        # tipically 0.0
+        readnoise = header['PCTERNOI']
     else:
         readnoise = 0.0
 
     return readnoise
 
 
 def get_image_exptime(header, survey):
     """Returns the exposure time from an image's header.
 
     Parameters
     ----------
     header: fits header
         Header of an image.
     survey: str
-        Survey name: ``PS1``, ``DES``, ``SDSS``, ``GALEX``, ``WISE``, ``2MASS``.
+        Survey name: e.g. ``PS1``, ``GALEX``.
 
     Returns
     -------
     exptime: float
         Exposure time in seconds.
     """
     check_survey_validity(survey)
-    if survey in ["PS1", "DES", "GALEX", "VISTA", "Spitzer"]:
+    if survey in ["PS1", "DES", "GALEX", "VISTA", "Spitzer", "HST"]:
         exptime = float(header["EXPTIME"])
     elif survey == "WISE":
         # see: https://wise2.ipac.caltech.edu/docs/release/allsky/
         # and https://wise2.ipac.caltech.edu/docs/release/allsky/expsup/sec1_1.html
         if header["BAND"] in [1, 2]:
             exptime = 7.7
         elif header["BAND"] in [3, 4]:
@@ -269,14 +278,63 @@
         exptime = 900.0  # assumed similar to DES
     else:
         exptime = 1.0
 
     return exptime
 
 
+def correct_HST_aperture(filt, ap_area, header):
+    """Get the aperture correction for the given configuration.
+
+    Parameters
+    ----------
+    filt : str
+        HST filter, e.g. ``WFC3_UVIS_F225W``.
+    ap_area: float
+        Aperture area.
+    header: fits header
+        Header of an image.
+
+    Returns
+    -------
+    correction: float
+        Aperture correction (encircled energy fraction).
+    """
+    # split instrument and filter
+    filt_split = filt.split('_')
+    filt = filt_split[-1]
+    instrument = filt_split[-2]
+
+    if instrument=='UVIS':
+        instrument = header['APERTURE']
+
+    # assuming circular aperture
+    # for an ellipse, this would take the average of the axes
+    ap_radius = np.sqrt(ap_area/np.pi)
+
+    # get correction curve
+    ac_files = glob.glob(os.path.join(hostphot_path, 'filters/HST/*'))
+    ac_file = [file for file in ac_files 
+               if f'{instrument.lower()}_aper' in file][0]
+    ac_df = pd.read_csv(ac_file)
+
+    # linear interpolation of the aperture correction
+    apertures = np.array([float(col.replace('APER#', '')) for col in ac_df.columns 
+                          if col.startswith('AP')])
+    ap_corr = ac_df[ac_df.FILTER==filt].values[0][2:].astype(float)
+
+    cont_apertures = np.arange(0, 9, 0.01)
+    cont_ap_corr = np.interp(cont_apertures, apertures, ap_corr)
+
+    # get the closest value
+    ind = np.argmin(np.abs(cont_apertures-ap_radius))
+    correction = cont_ap_corr[ind]
+
+    return correction
+
 def magnitude_calculation(
     flux,
     flux_err,
     survey,
     filt=None,
     ap_area=0.0,
     header=None,
@@ -285,15 +343,15 @@
     """Calculates the calibrated magnitudes and errors.
 
     Parameters
     ----------
     flux: float
         Aperture flux.
     survey: str
-        Survey name. E.g. ``PS1``, ``DES``, ``SDSS``, ``GALEX``, ``WISE``, etc.
+        Survey name: e.g. ``PS1``, ``GALEX``.
     filt: str, default ``None``
         Survey-specific filter.
     ap_area: float, default ``0.0``
         Aperture area.
     header: fits header, default ``None``
         Header of an image.
     bkg_rms: float, default ``0.0``
@@ -301,92 +359,137 @@
 
     Returns
     -------
     mag: float
         Apparent magnitude.
     mag_err: float
         Apparent magnitude uncertainty.
-    total_flux_error: float
-        Total uncertainty in flux units.
+    flux: float
+        Total flux.
+    flux_error: float
+        Total uncertainty in flux.
     """
+    # get zeropoint
     zp_dict = survey_zp(survey)
     if zp_dict == "header":
         zp = header["MAGZP"]
     else:
         zp = zp_dict[filt]
-
     if survey == "PS1":
         exptime = get_image_exptime(header, survey)
         zp += 2.5 * np.log10(exptime)
 
-    mag = -2.5 * np.log10(flux) + zp
-    mag_err = 2.5 / np.log(10) * flux_err / flux
-
     # error propagation
-    extra_err, total_flux_error = uncertainty_calculation(
+    mag_err, flux_err = uncertainty_calculation(
         flux,
         flux_err,
         survey,
         filt,
         ap_area,
         header,
         bkg_rms,
     )
-    mag_err = np.sqrt(mag_err**2 + extra_err**2)
 
-    return mag, mag_err, total_flux_error
+    if survey == 'HST':
+        # HST needs and aperture correction for the flux
+        # see, e.g. https://www.stsci.edu/hst/instrumentation/acs/data-analysis/aperture-corrections
+        ap_corr = correct_HST_aperture(filt, ap_area, header)
+        flux = flux*ap_corr
+
+    mag = -2.5 * np.log10(flux) + zp
+
+    return mag, mag_err, flux, flux_err
+
+
+def get_HST_err(filt, header):
+    """Obtaines the error propagation from the zeropoint.
+
+    Parameters
+    ----------
+    filt : str
+        HST filter, e.g. ``WFC3_UVIS_F225W``.
+    header: fits header
+        Header of an image.
 
+    Returns
+    -------
+    flux_err: float
+        Error on PHOTFLAM.
+    mag_err: float
+        Magnitude error on PHOTFLAM.
+    """
+    # split instrument and filter
+    filt_split = filt.split('_')
+    filt = filt_split[-1]
+    instrument = filt_split[-2]
+
+    if instrument=='UVIS':
+        # APERTURE usually point to UVIS2
+        instrument = header['APERTURE']
+
+    # get uncertainty file
+    err_file = os.path.join(hostphot_path, 
+                            'filters/HST/', 
+                            f'{instrument}_err.txt')
+    err_df = pd.read_csv(err_file, delim_whitespace=True)
+    filt_err_df = err_df[err_df.Filter==filt]
+
+    flux = filt_err_df.PHOTFLAM.values[0]
+    flux_err = filt_err_df.ERR_PHOTFLAM.values[0]
+    mag_err = np.abs(2.5 * flux_err / (flux * np.log(10)))
+    
+    return flux_err, mag_err
 
 def uncertainty_calculation(
     flux, flux_err, survey, filt=None, ap_area=0.0, header=None, bkg_rms=0.0
 ):
     """Calculates the uncertainty propagation.
 
     Parameters
     ----------
     flux: float
         Aperture flux.
     flux_err: float
         Aperture flux error.
     survey: str
-        Survey name. E.g. ``PS1``, ``DES``, ``SDSS``, ``GALEX``, ``WISE``, etc.
+        Survey name: e.g. ``PS1``, ``GALEX``.
     filt: str, default ``None``
         Survey-specific filter.
     ap_area: float, default ``0.0``
         Aperture area.
     header: fits header, default ``None``
         Header of an image.
     bkg_rms: float, default ``0.0``
         Background noise.
 
     Returns
     -------
     mag_err: float
         Extra uncertainty in magnitudes.
-    total_flux_err: float
+    flux_err: float
         Total uncertainty in flux units.
     """
     exptime = get_image_exptime(header, survey)
     gain = get_image_gain(header, survey)
     readnoise = get_image_readnoise(header, survey)
 
-    mag_err = 0.0
-    total_flux_err = np.copy(flux_err)
+    mag_err = 2.5 / np.log(10) * flux_err / flux
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
-        total_flux_err = np.sqrt(total_flux_err**2 + extra_flux_err**2)
-
+        flux_err = np.sqrt(flux_err**2 + extra_flux_err**2)
+    
     if survey == "DES":
         # see the photometry section in https://des.ncsa.illinois.edu/releases/dr1/dr1-docs/quality
         # statistical uncertainties on the AB magnitud system zeropoints
         unc_dict = {
             "g": 2.6e-3,
             "r": 2.9e-3,
             "i": 3.4e-3,
@@ -403,32 +506,32 @@
             "i": 5e-3,
             "z": 6e-3,
             "Y": 5e-3,
         }
         extra_err = unc_dict[filt]
         mag_err = np.sqrt(mag_err**2 + extra_err**2)
 
-        extra_flux_err = np.abs(flux * 0.4 * np.log(10) * extra_err)
-        total_flux_err = np.sqrt(total_flux_err**2 + extra_flux_err**2)
+        extra_flux_err = np.abs(flux*0.4*np.log(10)*extra_err)
+        flux_err = np.sqrt(flux_err ** 2 + extra_flux_err ** 2)
 
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
-        mag_err = np.sqrt(mag_err**2 + floor_err**2)
+        mag_err = np.sqrt(mag_err ** 2 + floor_err ** 2)
 
         extra_flux_err = np.abs(flux * 0.4 * np.log(10) * floor_err)
-        total_flux_err = np.sqrt(total_flux_err**2 + extra_flux_err**2)
+        flux_err = np.sqrt(flux_err ** 2 + extra_flux_err ** 2)
 
     elif survey == "SDSS":
         # https://data.sdss.org/datamodel/files/BOSS_PHOTOOBJ/frames/RERUN/RUN/CAMCOL/frame.html
         camcol = header["CAMCOL"]
         run = header["RUN"]
 
         gain_dict = {
@@ -483,47 +586,43 @@
             if camcol == 5:
                 dark_variance = 2.1025
 
         extra_err = 1.0857 * np.sqrt(dark_variance + flux / gain) / flux
         mag_err = np.sqrt(mag_err**2 + extra_err**2)
 
         extra_flux_err = np.sqrt(dark_variance + flux / gain)
-        total_flux_err = np.sqrt(total_flux_err**2 + extra_flux_err**2)
+        flux_err = np.sqrt(flux_err ** 2 + extra_flux_err ** 2)
 
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
-            flux_uv_err = (
-                np.sqrt(CPS * exptime + (0.050 * CPS * exptime) ** 2) / exptime
-            )
+            flux_uv_err = np.sqrt(CPS*exptime + (0.050 * CPS * exptime)**2)/exptime
         elif filt == "NUV":
             uv_err = -2.5 * (
                 np.log10(CPS)
                 - np.log10(
                     CPS
                     + (CPS * exptime + (0.027 * CPS * exptime) ** 2) ** 0.5
                     / exptime
                 )
             )
-            flux_uv_err = (
-                np.sqrt(CPS * exptime + (0.027 * CPS * exptime) ** 2) / exptime
-            )
+            flux_uv_err = np.sqrt(CPS * exptime + (0.027 * CPS * exptime) ** 2) / exptime
 
         mag_err = np.sqrt(mag_err**2 + uv_err**2)
 
-        total_flux_err = np.sqrt(total_flux_err**2 + flux_uv_err**2)
+        flux_err = np.sqrt(flux_err ** 2 + flux_uv_err ** 2)
 
     elif survey == "2MASS":
         # see: https://wise2.ipac.caltech.edu/staff/jarrett/2mass/3chan/noise/
         S = flux
         N_c = 6  # number of coadd pixels
         k_z = 1.7  # kernel smoothing factor
         n_f = ap_area  # number of frame pixels in the aperture; aprox. as aperture area
@@ -534,16 +633,16 @@
             S / (gain * N_c)
             + n_c * (2 * k_z * sigma_c) ** 2
             + (n_c * 0.024 * sigma_c) ** 2
         )
 
         mag_err = 1.0857 / SNR
 
-        extra_flux_err = flux / SNR
-        total_flux_err = np.sqrt(total_flux_err**2 + extra_flux_err**2)
+        extra_flux_err = flux/SNR
+        flux_err = np.sqrt(flux_err ** 2 + extra_flux_err ** 2)
 
     elif "WISE" in survey:
         # see: https://wise2.ipac.caltech.edu/docs/release/allsky/expsup/sec2_3f.html
         # see Table 5 of
         # https://wise2.ipac.caltech.edu/docs/release/allsky/expsup/sec4_4c.html#wpro
         # correction assumed to be 0 mags as PSF fitting is not used.
         m_apcor = 0.0
@@ -566,59 +665,63 @@
             * F_corr
             * (flux_err**2 + k * (N_A**2) / N_B * bkg_rms**2)
             + sigma_conf**2
         )
 
         mag_err = np.sqrt(1.179 * sigma_src**2 / F_src**2)
 
-        total_flux_err = f_apcor**2
+        flux_err = f_apcor ** 2
 
         # add uncertainty from the ZP
-        if survey == "unWISE":
+        if survey=="unWISE":
             # These values are the same for all Atlas Images of a given band...
             # see: https://wise2.ipac.caltech.edu/docs/release/allsky/expsup/sec2_3f.html
-            unc_dict = {"W1": 0.006, "W2": 0.007, "W3": 0.012, "W4": 0.012}
+            unc_dict = {'W1':0.006, 'W2':0.007, 'W3':0.012, 'W4':0.012}
             zp_unc = unc_dict[filt]
-        elif survey == "WISE":
+        elif survey=="WISE":
             zp_unc = header["MAGZPUNC"]
 
         mag_err = np.sqrt(mag_err**2 + zp_unc**2)
 
         extra_flux_err = np.abs(flux * 0.4 * np.log(10) * zp_unc)
-        total_flux_err = np.sqrt(total_flux_err**2 + extra_flux_err**2)
+        flux_err = np.sqrt(flux_err ** 2 + extra_flux_err ** 2)
 
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
-        total_flux_err = np.sqrt(total_flux_err**2 + extra_flux_err**2)
+        flux_err = np.sqrt(flux_err ** 2 + extra_flux_err ** 2)
+    elif survey == "HST":
+        flux_zp_unc, zp_unc = get_HST_err(filt, header)
 
+        mag_err = np.sqrt(mag_err**2 + zp_unc**2)
+        flux_err = np.sqrt(flux_err ** 2 + flux_zp_unc ** 2)
     else:
         raise Exception(
             f"Survey {survey} has not been added for error propagation."
         )
 
-    return mag_err, total_flux_err
+    return mag_err, flux_err
 
 
 def survey_pixel_scale(survey, filt=None):
     """Returns the pixel scale for a given survey.
 
     Parameters
     ----------
     survey: str
-        Survey name: ``PS1``, ``DES``, ``SDSS``, ``GALEX``, ``WISE``, ``2MASS``.
+        Survey name: e.g. ``PS1``, ``GALEX``.
     filt: str, default ``None``
         Filter to use by surveys that have different pixel scales
         for different filters (e.g. Spitzer's IRAC and MIPS instruments).
 
     Returns
     -------
     pixel_scale: float
@@ -654,117 +757,108 @@
     options for the given survey.
 
     Parameters
     ----------
     filters: str or list
         Filters to use, e,g, ``griz``.
     survey: str
-        Survey name, e.g. ``PS1``, ``DES`` and ``GALEX``.
+        Survey name: e.g. ``PS1``, ``GALEX``.
     """
-    if filters is not None:
+    if survey=='HST':
+        check_HST_filters(filters)
+
+    else:
         valid_filters = get_survey_filters(survey)
 
         for filt in filters:
             message = (
                 f"filter '{filt}' is not a valid option for "
                 f"'{survey}' survey ({valid_filters})"
             )
             assert filt in valid_filters, message
 
-
-def check_HST_inputs(filt, instrument):
-    """Check whether the given filter and instrument are whithin the valid
+def check_HST_filters(filt):
+    """Check whether the given filter is whithin the valid
     options for HST.
 
     Parameters
     ----------
-    filt: str
-        Filter to use, e,g, ``F225W``.
-    instrument: str
-        Instrument name, e.g. ``WFC3/UVIS1``.
-    """
-    hst_file = os.path.join(hostphot_path, "filters/HST", "HST_filters.txt")
-    valid_instruments, valid_filters = np.loadtxt(hst_file, dtype=str).T
-
-    assert (
-        instrument in valid_instruments
-    ), f"Not a valid HST instrument ({instrument}): {valid_instruments}"
-    assert (
-        filt in valid_filters
-    ), f"Not a valid HST filter ({filt}): {valid_filters}"
-
-    indexes_inst = [i for i, f in enumerate(valid_filters) if f == filt]
-    matched_instruments = valid_instruments[indexes_inst]
-    assert (
-        instrument in matched_instruments
-    ), f"Not a valid HST instrument-filter combination -> {instrument}-{filt}"
+    filt: str 
+        Filter to use, e,g, ``WFC3_UVIS_F225W``.
+    """        
+    if filt is None:
+        raise ValueError(f"'{filt}' is not a valid HST filter.")
+    
+    # For UVIS, only the filters of UVIS1 are used as the
+    # detector 2 is scaled to match detector 1
+    if 'UVIS' in filt:
+        filt = filt.replace('UVIS', 'UVIS1')
+
+    hostphot_path = hostphot.__path__[0]
+    hst_file = glob.glob(os.path.join(hostphot_path, "filters/HST/*/*"))
+    hst_filters = [os.path.basename(file).split('.')[0] for file in hst_file]
 
+    assert filt in hst_filters, f"Not a valid HST filter ({filt}): {hst_filters}"
 
-def extract_filters(filters, survey, version=None):
-    """Extracts transmission functions.
+
+def extract_filter(filt, survey, version=None):
+    """Extracts the transmission function for the filter.
 
     Parameters
     ----------
-    filters: str
-        Filters to extract.
+    filt: str
+        Filter to extract.
     survey: str
         Survey of the filters.
-    version: str
+    version: str, default ``None``
         Version of the filters to use. E.g. for the
         Legacy Survey as it uses DECam for the south
         and BASS+MzLS for the north.
 
     Returns
     -------
-    filters_dict: dict
-        Dictionary with transmission functions
-        and their respective wavelengths.
+    wave: array
+        Wavelength range of the filter.
+    transmission: array
+        Transmission function.
     """
     check_survey_validity(survey)
-    check_filters_validity(filters, survey)
-    filters_dict = {filt: None for filt in filters}
+    if survey=='HST':
+        check_filters_validity(filt, survey)
+    else:
+        check_filters_validity([filt], survey)
 
     if "WISE" in survey:
         survey = "WISE"  # for unWISE to use the same filters as WISE
+
     filters_path = os.path.join(hostphot.__path__[0], "filters", survey)
 
     # Assume DECaLS filters below 32 degrees and BASS+MzLS above
     # https://www.legacysurvey.org/status/
     if survey == "LegacySurvey":
-        filters_path = os.path.join(
-            hostphot.__path__[0], "filters", "LegacySurvey"
-        )
         if version == "BASS+MzLS":
-            for filt in filters:
-                if filt != "z":
-                    filt_file = os.path.join(filters_path, f"BASS_{filt}.dat")
-                else:
-                    filt_file = os.path.join(filters_path, f"MzLS_z.dat")
-                wave, transmission = np.loadtxt(filt_file).T
-                filters_dict[filt] = {
-                    "wave": wave,
-                    "transmission": transmission,
-                }
+            if filt == "z":
+                filt_file = os.path.join(filters_path, f"MzLS_z.dat")
+            else:
+                filt_file = os.path.join(filters_path, f"BASS_{filt}.dat")       
         elif version == "DECam":
-            for filt in filters:
-                filt_file = os.path.join(filters_path, f"DECAM_{filt}.dat")
-                wave, transmission = np.loadtxt(filt_file).T
-                filters_dict[filt] = {
-                    "wave": wave,
-                    "transmission": transmission,
-                }
-
-        return filters_dict
+            filt_file = os.path.join(filters_path, f"DECAM_{filt}.dat")
 
-    for filt in filters:
+    elif survey == "HST":
+        if 'UVIS' in filt:
+            # Usually UVIS2 is used, but there is no large difference
+            filt = filt.replace('UVIS', 'UVIS2')
+        hst_files = glob.glob(os.path.join(filters_path, '*/*'))
+        filt_file = [file for file in hst_files if filt in file][0]
+    else:
         filt_file = os.path.join(filters_path, f"{survey}_{filt}.dat")
-        wave, transmission = np.loadtxt(filt_file).T
-        filters_dict[filt] = {"wave": wave, "transmission": transmission}
+    
+    wave, transmission = np.loadtxt(filt_file).T
 
-    return filters_dict
+    return wave, transmission
 
 
 def integrate_filter(
     spectrum_wave,
     spectrum_flux,
     filter_wave,
     filter_response,
@@ -800,15 +894,14 @@
         spectrum_flux * interp_response * spectrum_wave, spectrum_wave
     )
     int2 = np.trapz(filter_response * filter_wave, filter_wave)
     flux_filter = int1 / int2
 
     return flux_filter
 
-
 def adapt_aperture(objects, img_wcs, img_wcs2, flip=False):
     """Changes the aperture parameters to consider differences
     in WCS between surveys.
 
     The values of ``center``, ``a`` and ``b`` should in pixel
     units. DES images are flipped, so these need to be corrected
     with ``theta -> -theta``, i.e. using ``flip=True``.
@@ -818,44 +911,42 @@
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
-        center = (obj["x"], obj["y"])
-        apertures = EllipticalAperture(
-            center, obj["a"], obj["b"], obj["theta"]
-        )
+        center = (obj['x'], obj['y'])
+        apertures = EllipticalAperture(center, obj['a'],
+                                       obj['b'], obj['theta'])
         sky_apertures = apertures.to_sky(img_wcs)
 
         new_apertures = sky_apertures.to_pixel(img_wcs2)
         new_center = new_apertures.positions
-        obj["x"], obj["y"] = new_center
-        obj["a"] = new_apertures.a
-        obj["b"] = new_apertures.b
-        obj["theta"] = new_apertures.theta
+        obj['x'], obj['y'] = new_center
+        obj['a'] = new_apertures.a
+        obj['b'] = new_apertures.b
+        obj['theta'] = new_apertures.theta
 
         if flip is True:
             # flip aperture orientation
-            obj["theta"] *= -1
+            obj['theta'] *= -1
 
     return objects_
 
-
 def check_work_dir(wokrdir):
     """Checks if the working directory exists. If it
     does not, one is created.
 
     Parameters
     ----------
     wokrdir: str
@@ -913,15 +1004,15 @@
         data,
         interpolation="nearest",
         cmap="gray",
         vmin=m - s,
         vmax=m + s,
         origin="lower",
     )
-
+    
     plt.show()
 
 
 def update_axislabels(ax):
     """Updates the labels and ticks of a plot.
 
     Parameters
```

### Comparing `hostphot-2.5.1/src/hostphot.egg-info/PKG-INFO` & `hostphot-2.6.0/src/hostphot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hostphot
-Version: 2.5.1
+Version: 2.6.0
 Summary: Global and local photometry of galaxies hosting supernovae or other transients
 Home-page: https://github.com/temuller/hostphot
 Author: Tomás Enrique Müller-Bravo and Lluís Galbany
 Author-email: t.e.muller-bravo@ice.csic.es
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -192,14 +192,19 @@
   number = {76}, 
   pages = {4508},  
   journal = {Journal of Open Source Software} 
 } 
 ```
 
 ## What's new!
+v2.6.0:
+* HST (WFC3 only) included
+* 2MASS cutouts fixed (it now downloads the image closest to the given coordinates)
+v2.5.1:
+* Using sfdmap2 instead of sfdmap to avoid issues with numpy version (requires Python>=3.9)
 v2.5.0:
 * Systematic error floor added to PS1 photometry
 * Added missing uncertainties in the error budget of DES (~5 mmag) 
 * Flux/counts have been added to output photometry
 * GALEX now downloads images with largest exposure time by default
 * Fixed image realignment/orientation between different surveys when using common apertures (for masking and global photometry)
 * Added option to output mask parameters, and also aperture parameters for global photometry
```

### Comparing `hostphot-2.5.1/src/hostphot.egg-info/SOURCES.txt` & `hostphot-2.6.0/src/hostphot.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,20 @@
 src/hostphot/filters/DES/DES_g.dat
 src/hostphot/filters/DES/DES_i.dat
 src/hostphot/filters/DES/DES_r.dat
 src/hostphot/filters/DES/DES_z.dat
 src/hostphot/filters/GALEX/AAA_README
 src/hostphot/filters/GALEX/GALEX_FUV.dat
 src/hostphot/filters/GALEX/GALEX_NUV.dat
-src/hostphot/filters/HST/HST_filters.txt
+src/hostphot/filters/HST/IR_err.txt
+src/hostphot/filters/HST/UVIS1_err.txt
+src/hostphot/filters/HST/UVIS2_err.txt
+src/hostphot/filters/HST/ir_aper_corrections.csv
+src/hostphot/filters/HST/wfc3uvis1_aper_007_syn.csv
+src/hostphot/filters/HST/wfc3uvis2_aper_007_syn.csv
 src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F435W.dat
 src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F475W.dat
 src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F502N.dat
 src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F550M.dat
 src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F555W.dat
 src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F606W.dat
 src/hostphot/filters/HST/ACS_WFC/ACS_WFC_F625W.dat
```

### Comparing `hostphot-2.5.1/tests/test_cutouts.py` & `hostphot-2.6.0/tests/test_cutouts.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/tests/test_global_phot.py` & `hostphot-2.6.0/tests/test_global_phot.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/tests/test_local_phot.py` & `hostphot-2.6.0/tests/test_local_phot.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/tests/test_preprocessing.py` & `hostphot-2.6.0/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `hostphot-2.5.1/tests/test_rgb_images.py` & `hostphot-2.6.0/tests/test_rgb_images.py`

 * *Files identical despite different names*

