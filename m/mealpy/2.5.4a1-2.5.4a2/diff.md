# Comparing `tmp/mealpy-2.5.4a1.tar.gz` & `tmp/mealpy-2.5.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mealpy-2.5.4a1.tar", last modified: Fri May  5 08:41:36 2023, max compression
+gzip compressed data, was "mealpy-2.5.4a2.tar", last modified: Mon May  8 09:26:07 2023, max compression
```

## Comparing `mealpy-2.5.4a1.tar` & `mealpy-2.5.4a2.tar`

### file list

```diff
@@ -1,177 +1,176 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.563960 mealpy-2.5.4a1/
--rw-r--r--   0 runner    (1001) docker     (123)    57633 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    90608 2023-05-05 08:41:36.563960 mealpy-2.5.4a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    88069 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.543960 mealpy-2.5.4a1/mealpy/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.543960 mealpy-2.5.4a1/mealpy/bio_based/
--rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/BBO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/BBOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/BMO.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/EOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/IWO.py
--rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/SBO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/SMA.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/SOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/SOS.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/TPO.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/TSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    11744 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/VCS.py
--rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/WHO.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/bio_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.547960 mealpy-2.5.4a1/mealpy/evolutionary_based/
--rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/evolutionary_based/CRO.py
--rw-r--r--   0 runner    (1001) docker     (123)    40520 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/evolutionary_based/DE.py
--rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/evolutionary_based/EP.py
--rw-r--r--   0 runner    (1001) docker     (123)    16955 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/evolutionary_based/ES.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/evolutionary_based/FPA.py
--rw-r--r--   0 runner    (1001) docker     (123)    38686 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/evolutionary_based/GA.py
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/evolutionary_based/MA.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/evolutionary_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.547960 mealpy-2.5.4a1/mealpy/human_based/
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/BRO.py
--rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/BSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/CA.py
--rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/CHIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    14812 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/FBIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    12588 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/GSKA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/HBO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/HCO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/ICA.py
--rw-r--r--   0 runner    (1001) docker     (123)    11696 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/ILA.py
--rw-r--r--   0 runner    (1001) docker     (123)    12285 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/LCO.py
--rw-r--r--   0 runner    (1001) docker     (123)    17806 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/QSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/SARO.py
--rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/SPBO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/SSDO.py
--rw-r--r--   0 runner    (1001) docker     (123)    13823 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/TLO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/TOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/WarSO.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/human_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.551960 mealpy-2.5.4a1/mealpy/math_based/
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/AOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/CEM.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/CGO.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/CircleSA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/GBO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/HC.py
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/INFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/PSS.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/RUN.py
--rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/SCA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/SHIO.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/math_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/multitask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.551960 mealpy-2.5.4a1/mealpy/music_based/
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/music_based/HS.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/music_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32769 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.551960 mealpy-2.5.4a1/mealpy/physics_based/
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/ASO.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/ArchOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/CDO.py
--rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/EFO.py
--rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/EO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/EVO.py
--rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/FLA.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/HGSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/MVO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/NRO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/RIME.py
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/SA.py
--rw-r--r--   0 runner    (1001) docker     (123)    20823 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/TWO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/WDO.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/physics_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.559960 mealpy-2.5.4a1/mealpy/swarm_based/
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/ABC.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/ACOR.py
--rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/AGTO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/ALO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/AO.py
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/ARO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/AVOA.py
--rw-r--r--   0 runner    (1001) docker     (123)    15447 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/BA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/BES.py
--rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/BFO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10607 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/BSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    17152 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/BeesA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/COA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/CSA.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/CSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/CoatiOA.py
--rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/DMOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/DO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/EHO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/ESOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/FA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/FFA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/FFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/FOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/FOX.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/GJO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/GOA.py
--rw-r--r--   0 runner    (1001) docker     (123)    19661 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/GTO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/GWO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/HBA.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/HGS.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/HHO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/JA.py
--rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/MFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/MGO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/MPA.py
--rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/MRFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/MSA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/NGO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/NMRA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/OOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/PFA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/POA.py
--rw-r--r--   0 runner    (1001) docker     (123)    27340 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/PSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/SCSO.py
--rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/SFO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/SHO.py
--rw-r--r--   0 runner    (1001) docker     (123)    14771 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/SLO.py
--rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/SRSR.py
--rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/SSA.py
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/SSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/SSpiderA.py
--rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/SSpiderO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/STO.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/SeaHO.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/ServalOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/TDO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/TSO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/WOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/WaOA.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/ZOA.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/swarm_based/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.559960 mealpy-2.5.4a1/mealpy/system_based/
--rw-r--r--   0 runner    (1001) docker     (123)    28103 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/system_based/AEO.py
--rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/system_based/GCO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/system_based/WCA.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/system_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.563960 mealpy-2.5.4a1/mealpy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/utils/history.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/utils/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/utils/termination.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.563960 mealpy-2.5.4a1/mealpy/utils/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/utils/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/mealpy/utils/visualize/linechart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.543960 mealpy-2.5.4a1/mealpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    90608 2023-05-05 08:41:36.000000 mealpy-2.5.4a1/mealpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-05 08:41:36.000000 mealpy-2.5.4a1/mealpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:41:36.000000 mealpy-2.5.4a1/mealpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-05 08:41:36.000000 mealpy-2.5.4a1/mealpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 08:41:36.000000 mealpy-2.5.4a1/mealpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 08:41:36.563960 mealpy-2.5.4a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:41:36.563960 mealpy-2.5.4a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/tests/test_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-05 08:39:15.000000 mealpy-2.5.4a1/tests/test_tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.389421 mealpy-2.5.4a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    58037 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    90608 2023-05-08 09:26:07.389421 mealpy-2.5.4a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    88069 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.369420 mealpy-2.5.4a2/mealpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.369420 mealpy-2.5.4a2/mealpy/bio_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/BBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/BBOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/BMO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/EOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/IWO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/SBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/SMA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/SOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/SOS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/TPO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/TSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/VCS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/WHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/bio_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.373420 mealpy-2.5.4a2/mealpy/evolutionary_based/
+-rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/evolutionary_based/CRO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40520 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/evolutionary_based/DE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/evolutionary_based/EP.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16955 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/evolutionary_based/ES.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/evolutionary_based/FPA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38686 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/evolutionary_based/GA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/evolutionary_based/MA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/evolutionary_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.373420 mealpy-2.5.4a2/mealpy/human_based/
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/BRO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12441 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/BSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/CA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/CHIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/FBIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12588 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/GSKA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/HBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/HCO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/ICA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12285 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/LCO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17806 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/QSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/SARO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/SPBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/SSDO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13823 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/TLO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/TOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/WarSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/human_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.377420 mealpy-2.5.4a2/mealpy/math_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/AOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/CEM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/CGO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/CircleSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/GBO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/HC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/INFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/PSS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/RUN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13376 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/SCA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/SHIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/math_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/multitask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.377420 mealpy-2.5.4a2/mealpy/music_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/music_based/HS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/music_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33893 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.377420 mealpy-2.5.4a2/mealpy/physics_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/ASO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/ArchOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/CDO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11475 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/EFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/EO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/EVO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/FLA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/HGSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/MVO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/NRO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/RIME.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/SA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20823 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/TWO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/WDO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/physics_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.385421 mealpy-2.5.4a2/mealpy/swarm_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/ABC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/ACOR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/AGTO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/ALO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/AO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/ARO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/AVOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15447 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/BA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/BES.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/BFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10607 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/BSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17152 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/BeesA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/COA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/CSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/CSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/CoatiOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10548 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/DMOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/DO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/EHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/ESOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/FA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/FFA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/FFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/FOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/FOX.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/GJO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/GOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19661 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/GTO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/GWO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/HBA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/HGS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/HHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/JA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/MFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/MGO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/MPA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/MRFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/MSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/NGO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/NMRA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/OOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/PFA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/POA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27073 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/PSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/SCSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/SFO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/SHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14504 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/SLO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14226 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/SRSR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/SSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/SSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/SSpiderA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/SSpiderO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/STO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/SeaHO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/ServalOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/TDO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/TSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/WOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/WaOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/ZOA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/swarm_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.385421 mealpy-2.5.4a2/mealpy/system_based/
+-rw-r--r--   0 runner    (1001) docker     (123)    28103 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/system_based/AEO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/system_based/GCO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/system_based/WCA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/system_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.389421 mealpy-2.5.4a2/mealpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/utils/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/utils/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/utils/termination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.389421 mealpy-2.5.4a2/mealpy/utils/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/utils/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/mealpy/utils/visualize/linechart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.369420 mealpy-2.5.4a2/mealpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    90608 2023-05-08 09:26:07.000000 mealpy-2.5.4a2/mealpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-08 09:26:07.000000 mealpy-2.5.4a2/mealpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:26:07.000000 mealpy-2.5.4a2/mealpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 09:26:07.000000 mealpy-2.5.4a2/mealpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 09:26:07.000000 mealpy-2.5.4a2/mealpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 09:26:07.389421 mealpy-2.5.4a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:26:07.389421 mealpy-2.5.4a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/tests/test_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-08 09:23:50.000000 mealpy-2.5.4a2/tests/test_tuner.py
```

### Comparing `mealpy-2.5.4a1/ChangeLog.md` & `mealpy-2.5.4a2/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,19 @@
 
 
 # Version 2.5.4
 
 ### Update
 + Update the parameter's order in Tuner class  
 + Update the saving's bug when using Termination in Multitask
-
++ Remove ILA optimizer 
++ Rename "amend_position()" definition in some algorithms to "bounded_position()".
++ Add a "amend_position()" function in Optimizer class. This function will call two functions.
+  + bounded_position() from optimizer. This means for optimizer level (get in valid range of position)
+  + amend_position() from problem. This means for problem level (transform to the correct solution)
 
 
 
 # Version 2.5.3
 
 ### Update 
 + Fix bug in roulette-wheel-selection in Optimizer
```

### Comparing `mealpy-2.5.4a1/LICENSE` & `mealpy-2.5.4a2/LICENSE`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/PKG-INFO` & `mealpy-2.5.4a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mealpy
-Version: 2.5.4a1
+Version: 2.5.4a2
 Summary: MEALPY: An Open-source Library for Latest Meta-heuristic Algorithms in Python
 Home-page: https://github.com/thieu1995/mealpy
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mealpy.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/mealpy
```

### Comparing `mealpy-2.5.4a1/README.md` & `mealpy-2.5.4a2/README.md`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/__init__.py` & `mealpy-2.5.4a2/mealpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # >>>
 # >>> ## Run the algorithm
 # >>> model = PSO.C_PSO(epoch=5, pop_size=50, name="C-PSO")
 # >>> best_position, best_fitness = model.solve(problem)
 # >>> print(f"Best solution: {best_position}, Best fitness: {best_fitness}")
 
 
-__version__ = "2.5.4-alpha.1"
+__version__ = "2.5.4-alpha.2"
 
 from .bio_based import (BBO, BBOA, BMO, EOA, IWO, SBO, SMA, SOA, SOS, TPO, TSA, VCS, WHO)
 from .evolutionary_based import (CRO, DE, EP, ES, FPA, GA, MA)
 from .human_based import (BRO, BSO, CA, CHIO, FBIO, GSKA, HBO, HCO, ICA, LCO, QSA, SARO, SPBO, SSDO, TLO, TOA, WarSO)
 from .math_based import (AOA, CEM, CGO, CircleSA, GBO, HC, INFO, PSS, RUN, SCA, SHIO)
 from .physics_based import (ArchOA, ASO, CDO, EFO, EO, EVO, FLA, HGSO, MVO, NRO, RIME, SA, TWO, WDO)
 from .swarm_based import (ABC, ACOR, AGTO, ALO, AO, ARO, AVOA, BA, BeesA, BES, BFO, BSA, COA, CoatiOA, CSA, CSO,
```

### Comparing `mealpy-2.5.4a1/mealpy/bio_based/BBO.py` & `mealpy-2.5.4a2/mealpy/bio_based/BBO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/bio_based/BBOA.py` & `mealpy-2.5.4a2/mealpy/bio_based/BBOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/bio_based/BMO.py` & `mealpy-2.5.4a2/mealpy/bio_based/BMO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/bio_based/EOA.py` & `mealpy-2.5.4a2/mealpy/bio_based/EOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/bio_based/IWO.py` & `mealpy-2.5.4a2/mealpy/bio_based/IWO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/bio_based/SBO.py` & `mealpy-2.5.4a2/mealpy/bio_based/SBO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/bio_based/SMA.py` & `mealpy-2.5.4a2/mealpy/bio_based/SMA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/bio_based/SOA.py` & `mealpy-2.5.4a2/mealpy/bio_based/SOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/bio_based/SOS.py` & `mealpy-2.5.4a2/mealpy/bio_based/SOS.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/bio_based/TPO.py` & `mealpy-2.5.4a2/mealpy/bio_based/TPO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/bio_based/TSA.py` & `mealpy-2.5.4a2/mealpy/bio_based/TSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/bio_based/VCS.py` & `mealpy-2.5.4a2/mealpy/bio_based/VCS.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,24 +188,15 @@
             epoch (int): maximum number of iterations, default = 10000
             pop_size (int): number of population size, default = 100
             lamda (float): Number of the best will keep, default = 0.5
             sigma (float): Weight factor, default = 1.5
         """
         super().__init__(epoch, pop_size, lamda, sigma, **kwargs)
 
-    def amend_position(self, position=None, lb=None, ub=None):
-        """
-        Args:
-            position: vector position (location) of the solution.
-            lb: list of lower bound values
-            ub: list of upper bound values
-
-        Returns:
-            Amended position (make the position is in bound)
-        """
+    def bounded_position(self, position=None, lb=None, ub=None):
         condition = np.logical_and(lb <= position, position <= ub)
         random_pos = np.random.uniform(lb, ub)
         return np.where(condition, position, random_pos)
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
```

### Comparing `mealpy-2.5.4a1/mealpy/bio_based/WHO.py` & `mealpy-2.5.4a2/mealpy/bio_based/WHO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/evolutionary_based/CRO.py` & `mealpy-2.5.4a2/mealpy/evolutionary_based/CRO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/evolutionary_based/DE.py` & `mealpy-2.5.4a2/mealpy/evolutionary_based/DE.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/evolutionary_based/EP.py` & `mealpy-2.5.4a2/mealpy/evolutionary_based/EP.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/evolutionary_based/ES.py` & `mealpy-2.5.4a2/mealpy/evolutionary_based/ES.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/evolutionary_based/FPA.py` & `mealpy-2.5.4a2/mealpy/evolutionary_based/FPA.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,24 +60,15 @@
         self.epoch = self.validator.check_int("epoch", epoch, [1, 100000])
         self.pop_size = self.validator.check_int("pop_size", pop_size, [10, 10000])
         self.p_s = self.validator.check_float("p_s", p_s, (0, 1.0))
         self.levy_multiplier = self.validator.check_float("levy_multiplier", levy_multiplier, (-10000, 10000))
         self.set_parameters(["epoch", "pop_size", "p_s", "levy_multiplier"])
         self.sort_flag = False
 
-    def amend_position(self, position=None, lb=None, ub=None):
-        """
-        Args:
-            position: vector position (location) of the solution.
-            lb: list of lower bound values
-            ub: list of upper bound values
-
-        Returns:
-            Amended position (make the position is in bound)
-        """
+    def bounded_position(self, position=None, lb=None, ub=None):
         condition = np.logical_and(lb <= position, position <= ub)
         random_pos = np.random.uniform(lb, ub)
         return np.where(condition, position, random_pos)
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
```

### Comparing `mealpy-2.5.4a1/mealpy/evolutionary_based/GA.py` & `mealpy-2.5.4a2/mealpy/evolutionary_based/GA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/evolutionary_based/MA.py` & `mealpy-2.5.4a2/mealpy/evolutionary_based/MA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/human_based/BRO.py` & `mealpy-2.5.4a2/mealpy/human_based/BRO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/human_based/BSO.py` & `mealpy-2.5.4a2/mealpy/human_based/BSO.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,24 +202,15 @@
             p4 (float): probability
             slope (int): changing logsig() function's slope (k: in the paper)
         """
         super().__init__(epoch, pop_size, m_clusters, p1, p2, p3, p4, **kwargs)
         self.slope = self.validator.check_int("slope", slope, [10, 50])
         self.set_parameters(["epoch", "pop_size", "m_clusters", "p1", "p2", "p3", "p4", "slope"])
 
-    def amend_position(self, position=None, lb=None, ub=None):
-        """
-        Args:
-            position: vector position (location) of the solution.
-            lb: list of lower bound values
-            ub: list of upper bound values
-
-        Returns:
-            Amended position (make the position is in bound)
-        """
+    def bounded_position(self, position=None, lb=None, ub=None):
         rand_pos = np.random.uniform(lb, ub)
         condition = np.logical_and(lb <= position, position <= ub)
         return np.where(condition, position, rand_pos)
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
```

### Comparing `mealpy-2.5.4a1/mealpy/human_based/CA.py` & `mealpy-2.5.4a2/mealpy/human_based/CA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/human_based/CHIO.py` & `mealpy-2.5.4a2/mealpy/human_based/CHIO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/human_based/FBIO.py` & `mealpy-2.5.4a2/mealpy/human_based/FBIO.py`

 * *Files 5% similar despite different names*

```diff
@@ -181,27 +181,15 @@
         """
         Args:
             epoch (int): maximum number of iterations, default = 10000
             pop_size (int): number of population size, default = 100
         """
         super().__init__(epoch, pop_size, **kwargs)
 
-    def amend_position(self, position=None, lb=None, ub=None):
-        """
-        Depend on what kind of problem are we trying to solve, there will be an different amend_position
-        function to rebound the position of agent into the valid range.
-
-        Args:
-            position: vector position (location) of the solution.
-            lb: list of lower bound values
-            ub: list of upper bound values
-
-        Returns:
-            Amended position (make the position is in bound)
-        """
+    def bounded_position(self, position=None, lb=None, ub=None):
         rand_pos = np.random.uniform(lb, ub)
         condition = np.logical_and(lb <= position, position <= ub)
         return np.where(condition, position, rand_pos)
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
```

### Comparing `mealpy-2.5.4a1/mealpy/human_based/GSKA.py` & `mealpy-2.5.4a2/mealpy/human_based/GSKA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/human_based/HBO.py` & `mealpy-2.5.4a2/mealpy/human_based/HBO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/human_based/HCO.py` & `mealpy-2.5.4a2/mealpy/human_based/HCO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/human_based/ICA.py` & `mealpy-2.5.4a2/mealpy/human_based/ICA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/human_based/LCO.py` & `mealpy-2.5.4a2/mealpy/human_based/LCO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/human_based/QSA.py` & `mealpy-2.5.4a2/mealpy/human_based/QSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/human_based/SARO.py` & `mealpy-2.5.4a2/mealpy/human_based/SARO.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,27 +62,15 @@
 
     def initialization(self):
         if self.pop is None:
             self.pop = self.create_population(2 * self.pop_size)
         else:
             self.pop = self.pop + self.create_population(self.pop_size)
 
-    def amend_position(self, position=None, lb=None, ub=None):
-        """
-        Depend on what kind of problem are we trying to solve, there will be an different amend_position
-        function to rebound the position of agent into the valid range.
-
-        Args:
-            position: vector position (location) of the solution.
-            lb: list of lower bound values
-            ub: list of upper bound values
-
-        Returns:
-            Amended position (make the position is in bound)
-        """
+    def bounded_position(self, position=None, lb=None, ub=None):
         condition = np.logical_and(lb <= position, position <= ub)
         rand_pos = np.random.uniform(lb, ub)
         return np.where(condition, position, rand_pos)
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
```

### Comparing `mealpy-2.5.4a1/mealpy/human_based/SPBO.py` & `mealpy-2.5.4a2/mealpy/human_based/SPBO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/human_based/SSDO.py` & `mealpy-2.5.4a2/mealpy/human_based/SSDO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/human_based/TLO.py` & `mealpy-2.5.4a2/mealpy/human_based/TLO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/human_based/TOA.py` & `mealpy-2.5.4a2/mealpy/human_based/TOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/human_based/WarSO.py` & `mealpy-2.5.4a2/mealpy/human_based/WarSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/math_based/AOA.py` & `mealpy-2.5.4a2/mealpy/math_based/AOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/math_based/CEM.py` & `mealpy-2.5.4a2/mealpy/math_based/CEM.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/math_based/CGO.py` & `mealpy-2.5.4a2/mealpy/math_based/CGO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/math_based/CircleSA.py` & `mealpy-2.5.4a2/mealpy/math_based/CircleSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/math_based/GBO.py` & `mealpy-2.5.4a2/mealpy/math_based/GBO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/math_based/HC.py` & `mealpy-2.5.4a2/mealpy/math_based/HC.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/math_based/INFO.py` & `mealpy-2.5.4a2/mealpy/math_based/INFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/math_based/PSS.py` & `mealpy-2.5.4a2/mealpy/math_based/PSS.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/math_based/RUN.py` & `mealpy-2.5.4a2/mealpy/math_based/RUN.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/math_based/SCA.py` & `mealpy-2.5.4a2/mealpy/math_based/SCA.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,27 +121,15 @@
         Args:
             epoch (int): maximum number of iterations, default = 10000
             pop_size (int): number of population size, default = 100
         """
         super().__init__(epoch, pop_size, **kwargs)
         self.sort_flag = False
 
-    def amend_position(self, position=None, lb=None, ub=None):
-        """
-        Depend on what kind of problem are we trying to solve, there will be an different amend_position
-        function to rebound the position of agent into the valid range.
-
-        Args:
-            position: vector position (location) of the solution.
-            lb: list of lower bound values
-            ub: list of upper bound values
-
-        Returns:
-            Amended position (make the position is in bound)
-        """
+    def bounded_position(self, position=None, lb=None, ub=None):
         return np.where(np.logical_and(lb <= position, position <= ub), position, np.random.uniform(lb, ub))
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
 
         Args:
@@ -270,15 +258,15 @@
         if pos is None:
             pos = self.generate_position(lb, ub)
         position = self.amend_position(pos, lb, ub)
         target = self.get_target_wrapper(position)
         q_table = QTable(n_states=9, n_actions=9)
         return [position, target, q_table]
 
-    def amend_position(self, position=None, lb=None, ub=None):
+    def bounded_position(self, position=None, lb=None, ub=None):
         return np.where(np.logical_and(lb <= position, position <= ub), position, np.random.uniform(lb, ub))
 
     def density__(self, pop):
         agents = np.array([agent[self.ID_POS] for agent in pop])
         # calculate the mean of each dimension of the agents
         Y = np.mean(agents, axis=0)
         # calculate the longest diagonal length L
```

### Comparing `mealpy-2.5.4a1/mealpy/math_based/SHIO.py` & `mealpy-2.5.4a2/mealpy/math_based/SHIO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/multitask.py` & `mealpy-2.5.4a2/mealpy/multitask.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/music_based/HS.py` & `mealpy-2.5.4a2/mealpy/music_based/HS.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/optimizer.py` & `mealpy-2.5.4a2/mealpy/optimizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -188,17 +188,48 @@
         position = self.amend_position(pos, lb, ub)
         target = self.get_target_wrapper(position)
         return [position, target]
 
     def evolve(self, epoch):
         pass
 
+    def bounded_position(self, position=None, lb=None, ub=None):
+        """
+        This is default function in most algorithms. Otherwise, there will be an overridden function
+        in child of Optimizer class for this function.
+
+        Args:
+            position: vector position (location) of the solution.
+            lb: list of lower bound values
+            ub: list of upper bound values
+
+        Returns:
+            Bounded position (make the position is in bound)
+        """
+        return np.clip(position, lb, ub)
+
+    def amend_position(self, position=None, lb=None, ub=None):
+        """
+        This function will call two functions:
+            + self.bounded_position(): Get the valid position by the Optimizer
+            + self.problem.amend_position(): Amend the position by the problem
+
+        Args:
+            position: vector position (location) of the solution.
+            lb: list of lower bound values
+            ub: list of upper bound values
+
+        Returns:
+            Amended position (make the position is in bound)
+        """
+        pos = self.bounded_position(position, lb, ub)
+        return self.problem.amend_position(pos, lb, ub)
+
     def check_problem(self, problem):
         self.problem = problem if isinstance(problem, Problem) else Problem(**problem)
-        self.amend_position = self.problem.amend_position
         self.generate_position = self.problem.generate_position
         self.logger = Logger(self.problem.log_to, log_file=self.problem.log_file).create_logger(name=f"{self.__module__}.{self.__class__.__name__}")
         self.logger.info(self.problem.msg)
         self.history = History(log_to=self.problem.log_to, log_file=self.problem.log_file)
         self.pop, self.g_best, self.g_worst = None, None, None
 
     def check_mode_and_workers(self, mode, n_workers):
```

### Comparing `mealpy-2.5.4a1/mealpy/physics_based/ASO.py` & `mealpy-2.5.4a2/mealpy/physics_based/ASO.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,24 +82,15 @@
             pos = self.generate_position(lb, ub)
         position = self.amend_position(pos, lb, ub)
         target = self.get_target_wrapper(position)
         velocity = self.generate_position(lb, ub)
         mass = 0.0
         return [position, target, velocity, mass]
 
-    def amend_position(self, position=None, lb=None, ub=None):
-        """
-        Args:
-            position: vector position (location) of the solution.
-            lb: list of lower bound values
-            ub: list of upper bound values
-
-        Returns:
-            Amended position (make the position is in bound)
-        """
+    def bounded_position(self, position=None, lb=None, ub=None):
         condition = np.logical_and(lb <= position, position <= ub)
         rand_pos = np.random.uniform(lb, ub)
         return np.where(condition, position, rand_pos)
 
     def update_mass__(self, population):
         list_fit = np.array([agent[self.ID_TAR][self.ID_FIT] for agent in population])
         list_fit = np.exp(-(list_fit - np.max(list_fit)) / (np.max(list_fit) - np.min(list_fit) + self.EPSILON))
```

### Comparing `mealpy-2.5.4a1/mealpy/physics_based/ArchOA.py` & `mealpy-2.5.4a2/mealpy/physics_based/ArchOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/physics_based/CDO.py` & `mealpy-2.5.4a2/mealpy/physics_based/CDO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/physics_based/EFO.py` & `mealpy-2.5.4a2/mealpy/physics_based/EFO.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,27 +159,15 @@
             ps_rate (float): default = 0.85    Like crossover parameter in GA
             p_field (float): default = 0.1     portion of population, positive field
             n_field (float): default = 0.45    portion of population, negative field
         """
         super().__init__(epoch, pop_size, r_rate, ps_rate, p_field, n_field, **kwargs)
         self.support_parallel_modes = False
 
-    def amend_position(self, position=None, lb=None, ub=None):
-        """
-        Depend on what kind of problem are we trying to solve, there will be an different amend_position
-        function to rebound the position of agent into the valid range.
-
-        Args:
-            position: vector position (location) of the solution.
-            lb: list of lower bound values
-            ub: list of upper bound values
-
-        Returns:
-            Amended position (make the position is in bound)
-        """
+    def bounded_position(self, position=None, lb=None, ub=None):
         return np.where(np.logical_and(lb <= position, position <= ub), position, np.random.uniform(lb, ub))
 
     def initialization(self):
         # %random vectors (this is to increase the calculation speed instead of determining the random values in each
         # iteration we allocate them in the beginning before algorithm start
         self.r_index1 = np.random.randint(0, int(self.pop_size * self.p_field), (self.problem.n_dims, self.epoch))
         # random particles from positive field
```

### Comparing `mealpy-2.5.4a1/mealpy/physics_based/EO.py` & `mealpy-2.5.4a2/mealpy/physics_based/EO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/physics_based/EVO.py` & `mealpy-2.5.4a2/mealpy/physics_based/EVO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/physics_based/FLA.py` & `mealpy-2.5.4a2/mealpy/physics_based/FLA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/physics_based/HGSO.py` & `mealpy-2.5.4a2/mealpy/physics_based/HGSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/physics_based/MVO.py` & `mealpy-2.5.4a2/mealpy/physics_based/MVO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/physics_based/NRO.py` & `mealpy-2.5.4a2/mealpy/physics_based/NRO.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,27 +55,15 @@
         """
         super().__init__(**kwargs)
         self.epoch = self.validator.check_int("epoch", epoch, [1, 100000])
         self.pop_size = self.validator.check_int("pop_size", pop_size, [10, 10000])
         self.set_parameters(["epoch", "pop_size"])
         self.sort_flag = False
 
-    def amend_position(self, position=None, lb=None, ub=None):
-        """
-        Depend on what kind of problem are we trying to solve, there will be an different amend_position
-        function to rebound the position of agent into the valid range.
-
-        Args:
-            position: vector position (location) of the solution.
-            lb: list of lower bound values
-            ub: list of upper bound values
-
-        Returns:
-            Amended position (make the position is in bound)
-        """
+    def bounded_position(self, position=None, lb=None, ub=None):
         rand_pos = np.random.uniform(lb, ub)
         condition = np.logical_and(lb <= position, position <= ub)
         return np.where(condition, position, rand_pos)
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
```

### Comparing `mealpy-2.5.4a1/mealpy/physics_based/RIME.py` & `mealpy-2.5.4a2/mealpy/physics_based/RIME.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/physics_based/SA.py` & `mealpy-2.5.4a2/mealpy/physics_based/SA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/physics_based/TWO.py` & `mealpy-2.5.4a2/mealpy/physics_based/TWO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/physics_based/WDO.py` & `mealpy-2.5.4a2/mealpy/physics_based/WDO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/ABC.py` & `mealpy-2.5.4a2/mealpy/swarm_based/ABC.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/ACOR.py` & `mealpy-2.5.4a2/mealpy/swarm_based/ACOR.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/AGTO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/AGTO.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         super().__init__(**kwargs)
         self.epoch = self.validator.check_int("epoch", epoch, [1, 100000])
         self.pop_size = self.validator.check_int("pop_size", pop_size, [10, 10000])
         self.pp = self.validator.check_float("p1", pp, (0, 1))      # p in the paper
         self.set_parameters(["epoch", "pop_size", "pp"])
         self.sort_flag = False
 
-    def amend_position(self, position=None, lb=None, ub=None):
+    def bounded_position(self, position=None, lb=None, ub=None):
         condition = np.logical_and(lb <= position, position <= ub)
         random_pos = np.random.uniform(lb, ub)
         return np.where(condition, position, random_pos)
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
```

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/ALO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/ALO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/AO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/AO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/ARO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/ARO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/AVOA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/AVOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/BA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/BA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/BES.py` & `mealpy-2.5.4a2/mealpy/swarm_based/BES.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/BFO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/BFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/BSA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/BSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/BeesA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/BeesA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/COA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/COA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/CSA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/CSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/CSO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/CSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/CoatiOA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/CoatiOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/DMOA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/DMOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/DO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/DO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/EHO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/EHO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/ESOA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/ESOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/FA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/FA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/FFA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/FFA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/FFO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/FFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/FOA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/FOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/FOX.py` & `mealpy-2.5.4a2/mealpy/swarm_based/FOX.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/GJO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/GJO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/GOA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/GOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/GTO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/GTO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/GWO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/GWO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/HBA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/HBA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/HGS.py` & `mealpy-2.5.4a2/mealpy/swarm_based/HGS.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/HHO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/HHO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/JA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/JA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/MFO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/MFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/MGO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/MGO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/MPA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/MPA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/MRFO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/MRFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/MSA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/MSA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/NGO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/NGO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/NMRA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/NMRA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/OOA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/OOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/PFA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/PFA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/POA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/POA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/PSO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/PSO.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,24 +91,15 @@
         position = self.amend_position(pos, lb, ub)
         target = self.get_target_wrapper(position)
         velocity = np.random.uniform(self.v_min, self.v_max)
         local_pos = deepcopy(position)
         local_fit = deepcopy(target)
         return [position, target, velocity, local_pos, local_fit]
 
-    def amend_position(self, position=None, lb=None, ub=None):
-        """
-        Args:
-            position: vector position (location) of the solution.
-            lb: list of lower bound values
-            ub: list of upper bound values
-
-        Returns:
-            Amended position (make the position is in bound)
-        """
+    def bounded_position(self, position=None, lb=None, ub=None):
         condition = np.logical_and(lb <= position, position <= ub)
         pos_rand = np.random.uniform(lb, ub)
         return np.where(condition, position, pos_rand)
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
```

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/SCSO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/SCSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/SFO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/SFO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/SHO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/SHO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/SLO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/SLO.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,24 +55,15 @@
         """
         super().__init__(**kwargs)
         self.epoch = self.validator.check_int("epoch", epoch, [1, 100000])
         self.pop_size = self.validator.check_int("pop_size", pop_size, [10, 10000])
         self.set_parameters(["epoch", "pop_size"])
         self.sort_flag = False
 
-    def amend_position(self, position=None, lb=None, ub=None):
-        """
-        Args:
-            position: vector position (location) of the solution.
-            lb: list of lower bound values
-            ub: list of upper bound values
-
-        Returns:
-            Amended position (make the position is in bound)
-        """
+    def bounded_position(self, position=None, lb=None, ub=None):
         condition = np.logical_and(lb <= position, position <= ub)
         pos_rand = np.random.uniform(lb, ub)
         return np.where(condition, position, pos_rand)
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
```

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/SRSR.py` & `mealpy-2.5.4a2/mealpy/swarm_based/SRSR.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/SSA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/SSA.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,24 +68,15 @@
         self.PD = self.validator.check_float("PD", PD, (0, 1.0))
         self.SD = self.validator.check_float("SD", SD, (0, 1.0))
         self.set_parameters(["epoch", "pop_size", "ST", "PD", "SD"])
         self.n1 = int(self.PD * self.pop_size)
         self.n2 = int(self.SD * self.pop_size)
         self.sort_flag = True
 
-    def amend_position(self, position=None, lb=None, ub=None):
-        """
-        Args:
-            position: vector position (location) of the solution.
-            lb: list of lower bound values
-            ub: list of upper bound values
-
-        Returns:
-            Amended position (make the position is in bound)
-        """
+    def bounded_position(self, position=None, lb=None, ub=None):
         condition = np.logical_and(lb <= position, position <= ub)
         pos_rand = np.random.uniform(lb, ub)
         return np.where(condition, position, pos_rand)
 
     def evolve(self, epoch):
         """
         The main operations (equations) of algorithm. Inherit from Optimizer class
```

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/SSO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/SSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/SSpiderA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/SSpiderA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/SSpiderO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/SSpiderO.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,27 +95,15 @@
         if pos is None:
             pos = self.generate_position(lb, ub)
         position = self.amend_position(pos, lb, ub)
         target = self.get_target_wrapper(position)
         weight = 0.0
         return [position, target, weight]
 
-    def amend_position(self, position=None, lb=None, ub=None):
-        """
-        Depend on what kind of problem are we trying to solve, there will be an different amend_position
-        function to rebound the position of agent into the valid range.
-
-        Args:
-            position: vector position (location) of the solution.
-            lb: list of lower bound values
-            ub: list of upper bound values
-
-        Returns:
-            Amended position (make the position is in bound)
-        """
+    def bounded_position(self, position=None, lb=None, ub=None):
         return np.where(np.logical_and(lb <= position, position <= ub), position, np.random.uniform(lb, ub))
 
     def move_females__(self, epoch=None):
         scale_distance = np.sum(self.problem.ub - self.problem.lb)
         pop = self.pop_females + self.pop_males
         # Start looking for any stronger vibration
         for i in range(0, self.n_f):  # Move the females
```

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/STO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/STO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/SeaHO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/SeaHO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/ServalOA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/ServalOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/TDO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/TDO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/TSO.py` & `mealpy-2.5.4a2/mealpy/swarm_based/TSO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/WOA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/WOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/WaOA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/WaOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/swarm_based/ZOA.py` & `mealpy-2.5.4a2/mealpy/swarm_based/ZOA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/system_based/AEO.py` & `mealpy-2.5.4a2/mealpy/system_based/AEO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/system_based/GCO.py` & `mealpy-2.5.4a2/mealpy/system_based/GCO.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/system_based/WCA.py` & `mealpy-2.5.4a2/mealpy/system_based/WCA.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/tuner.py` & `mealpy-2.5.4a2/mealpy/tuner.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/utils/history.py` & `mealpy-2.5.4a2/mealpy/utils/history.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/utils/io.py` & `mealpy-2.5.4a2/mealpy/utils/io.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/utils/logger.py` & `mealpy-2.5.4a2/mealpy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/utils/problem.py` & `mealpy-2.5.4a2/mealpy/utils/problem.py`

 * *Files 5% similar despite different names*

```diff
@@ -180,21 +180,20 @@
         Returns:
             np.array: the position (the solution for the problem)
         """
         return np.random.uniform(lb, ub)
 
     def amend_position(self, position=None, lb=None, ub=None):
         """
-        This is default function in most algorithms. Otherwise, there will be an overridden function
-        in child of Optimizer class for this function. Depend on what kind of problem are we trying to solve,
-        there will be a different amend_position function to rebound the position of agent into the valid range.
+        The goal is to transform the solution into the right format corresponding to the problem.
+        For example, with discrete problems, floating-point numbers must be converted to integers
+        to ensure the solution is in the correct format.
 
         Args:
             position: vector position (location) of the solution.
             lb: list of lower bound values
             ub: list of upper bound values
 
         Returns:
-            Amended position (make the position is in bound)
+            Amended position (make the right format of the solution)
         """
-        # return np.maximum(self.problem.lb, np.minimum(self.problem.ub, position))
-        return np.clip(position, lb, ub)
+        return position
```

### Comparing `mealpy-2.5.4a1/mealpy/utils/termination.py` & `mealpy-2.5.4a2/mealpy/utils/termination.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/utils/validator.py` & `mealpy-2.5.4a2/mealpy/utils/validator.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy/utils/visualize/linechart.py` & `mealpy-2.5.4a2/mealpy/utils/visualize/linechart.py`

 * *Files identical despite different names*

### Comparing `mealpy-2.5.4a1/mealpy.egg-info/PKG-INFO` & `mealpy-2.5.4a2/mealpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mealpy
-Version: 2.5.4a1
+Version: 2.5.4a2
 Summary: MEALPY: An Open-source Library for Latest Meta-heuristic Algorithms in Python
 Home-page: https://github.com/thieu1995/mealpy
 Author: Thieu
 Author-email: nguyenthieu2102@gmail.com
 License: GPLv3
 Project-URL: Documentation, https://mealpy.readthedocs.io/
 Project-URL: Source Code, https://github.com/thieu1995/mealpy
```

### Comparing `mealpy-2.5.4a1/mealpy.egg-info/SOURCES.txt` & `mealpy-2.5.4a2/mealpy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 mealpy/human_based/CA.py
 mealpy/human_based/CHIO.py
 mealpy/human_based/FBIO.py
 mealpy/human_based/GSKA.py
 mealpy/human_based/HBO.py
 mealpy/human_based/HCO.py
 mealpy/human_based/ICA.py
-mealpy/human_based/ILA.py
 mealpy/human_based/LCO.py
 mealpy/human_based/QSA.py
 mealpy/human_based/SARO.py
 mealpy/human_based/SPBO.py
 mealpy/human_based/SSDO.py
 mealpy/human_based/TLO.py
 mealpy/human_based/TOA.py
```

### Comparing `mealpy-2.5.4a1/setup.py` & `mealpy-2.5.4a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with open('README.md', encoding='utf-8') as f:
         README = f.read()
     return README
 
 
 setup(
     name="mealpy",
-    version="2.5.4-alpha.1",
+    version="2.5.4-alpha.2",
     author="Thieu",
     author_email="nguyenthieu2102@gmail.com",
     description="MEALPY: An Open-source Library for Latest Meta-heuristic Algorithms in Python",
     long_description=readme(),
     long_description_content_type="text/markdown",
     keywords=["optimization", "metaheuristics", "MHA", "mathematical optimization", "nature-inspired algorithms",
               "evolutionary computation", "soft computing", "population-based algorithms",
```

### Comparing `mealpy-2.5.4a1/tests/test_optimizer.py` & `mealpy-2.5.4a2/tests/test_optimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,26 +20,25 @@
         "lb": [-10, -10, -10, -10, -10],
         "ub": [10, 10, 10, 10, 10],
         "minmax": "min",
         "log_to": None,
     }
     model = Optimizer()
     model.problem = Problem(**problem)
-    model.amend_position = model.problem.amend_position
     model.generate_position = model.problem.generate_position
     return model
 
 
 def test_amend_position(model):
     LB = model.problem.lb
     UB = model.problem.ub
     pos = np.array([-15.4, 100, 0.4, -9, 7])
     pos = model.amend_position(pos, LB, UB)
-    comparison = (pos == np.array([-10, 10, 0.4, -9, 7]))
-    assert comparison.all()
+    print(pos)
+    assert np.all(pos == np.array([-10, 10, 0.4, -9, 7]))
 
 
 def test_get_target_wrapper(model):
     pos = np.array([1, 2, 0, 2, 1])
     target = model.get_target_wrapper(pos)
     fit = np.sum(pos ** 2)
     assert target[model.ID_FIT] == fit
```

### Comparing `mealpy-2.5.4a1/tests/test_tuner.py` & `mealpy-2.5.4a2/tests/test_tuner.py`

 * *Files identical despite different names*

