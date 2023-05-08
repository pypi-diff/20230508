# Comparing `tmp/z4d-certified-devices-2.56.tar.gz` & `tmp/z4d-certified-devices-2.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z4d-certified-devices-2.56.tar", last modified: Mon May  1 16:56:40 2023, max compression
+gzip compressed data, was "z4d-certified-devices-2.57.tar", last modified: Mon May  8 19:42:18 2023, max compression
```

## Comparing `z4d-certified-devices-2.56.tar` & `z4d-certified-devices-2.57.tar`

### file list

```diff
@@ -1,520 +1,521 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.586126 z4d-certified-devices-2.56/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    36120 2023-05-01 16:56:40.586126 z4d-certified-devices-2.56/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-01 16:56:40.586126 z4d-certified-devices-2.56/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.518127 z4d-certified-devices-2.56/z4d_certified_devices/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.522127 z4d-certified-devices-2.56/z4d_certified_devices/Certified/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.522127 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Adeo/
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Adeo/LDSENK02F.json
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Adeo/LDSENK10.json
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Adeo/LXEK-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Adeo/LXEK-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Adeo/LXEK-7.json
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Adeo/ZBEK-14.json
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Adeo/ZBEK-3.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.522127 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Aotec/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Aotec/WG001-Z01.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.526126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Bitron/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Bitron/90201021A.json
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Bitron/90201021B.json
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Bitron/90201024.json
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Bitron/AV201021B.json
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Bitron/AV201024A.json
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Bitron/AV201029A.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.526126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/CLEODE/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/CLEODE/ZHUM.json
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/CLEODE/ZMOVE.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/CLEODE/ZPLUG.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.534126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CAC221.json
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CCB432.json
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CDWS312.json
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CKF204.json
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CKF205.json
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CMS323.json
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CPB206.json
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CPC321.json
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CPR412-E.json
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CPR412.json
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CSAC451-E.json
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CSAC451-WTC-E.json
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CSLC601-D-E.json
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CSLC601-E.json
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CSLC631-3.json
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CSP403.json
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CTHS317ET.json
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/Dual_Relay_Module.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.534126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Danalock/
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Danalock/V3-BTZB.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.534126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Danfoss/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Danfoss/RV001.json
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Danfoss/eT093WRG.json
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Danfoss/eT093WRO.json
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Danfoss/eTRV0100.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.534126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Develco/
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Develco/HESZB120.json
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Develco/HMSZB-110.json
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Develco/MOSZB-140.json
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Develco/SMSZB-120.json
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Develco/SPLZB-131.json
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Develco/SPLZB-132.json
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Develco/ZHEMI101.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.538126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/ENKI-LEXMAN/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-7.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.538126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Eurotronics/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Eurotronics/SPZB0001.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.538126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-B-004P.json
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-B-007Z.json
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008Z.json
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008ZS.json
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007-2ID.json
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007.json
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008.json
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008S.json
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008Z.json
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-C-009.json
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-D-003Z.json
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-FL-004TZS.json
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-MC-001.json
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-S-007ZS.json
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GLEDOPTO.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.546126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/COSensor-EF-3.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/COSensor-EM.json
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/COSensor-N.json
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/CO_V15.json
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/CO_YDLV10.json
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/GASSensor-EF-3.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/GAS_V15.json
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/RC-EF-3.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/RC-EM.json
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/SMOK_V16.json
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/SMOK_YDLV10.json
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/SRHMP-I1.json
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/SceneSwitch-EM-3.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/SmartPlug.json
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/SmokeSensor-EF-3.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/SmokeSensor-EM.json
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/SmokeSensor-N-3.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/SmokeSensor-N.json
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/TS0216.json
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/WarningDevice-EF-3.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/WarningDevice.json
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/WaterSensor-EF-3.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.554126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 30x90.json
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 60x60.json
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/FYRTUR block-out roller blind.json
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/KADRILJ roller blind.json
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/Remote Control N2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/STARKVIND Air purifier.json
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/STOFTMOLN ceilingwall lamp WW24.json
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 10W.json
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 30W.json
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI SHORTCUT Button.json
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Signal Repeater.json
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E12 WS opal 400lm.json
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 W opch 400lm.json
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS 470lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 400lm.json
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 600lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS clear 950lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS opal 980lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS 806lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS opal 600lm.json
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 W opal 1000lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 806lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 950lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 1000lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 950lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 980lm.json
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW 806lm.json
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW clear 250lm.json
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 opal 1000lm.json
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 W 400lm.json
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WS 400lm.json
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WW 400lm.json
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI control outlet.json
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI motion sensor.json
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI onoff switch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI openclose remote.json
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI remote control.json
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI transformer 10W.json
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI wireless dimmer.json
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE14WScandleopal470lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbGU10WS345lm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/VINDSTYRKA.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.554126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/INNR/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/INNR/OSL 130 C.json
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/INNR/RB 248 T.json
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/INNR/RB 285 C.json
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/INNR/SP 120.json
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/INNR/SP 220.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.554126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Idinio/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Idinio/Dimmer-Switch-ZB3.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.554126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Iluminize/
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Iluminize/511.201.json
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Iluminize/5120.1200.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.554126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Konke/
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Konke/3AFE140103020000.json
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Konke/3AFE14010402000D.json
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Konke/3AFE170100510001.json
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Konke/3AFE220103020000.json
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Konke/3AFE28010402000D.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.554126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LIVOLO/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LIVOLO/TI0001.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.554126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LS-Deutschland-GmbH/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LS-Deutschland-GmbH/Emotion.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.562126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.airmonitor.acn01.json
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.aq1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.json
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.aq1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral1.json
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.light.aqcn02.json
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.lock.v1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.magnet.acn001.json
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.motion.ac01.json
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.motion.ac02.json
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.plug.json
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.plug.maeu01.json
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.plug.mmeu01.json
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.relay.c2acn01.json
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn01.json
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn02.json
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b1acn01.json
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn01.json
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn02.json
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01-bulb.json
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01.json
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b28ac1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01-bulb.json
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01.json
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01-bulb.json
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01.json
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.router.json
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sen_ill.mgl01.json
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sens.json
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw1.json
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw2.json
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.aqgl01.json
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.json
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_ht.json
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.acn001.json
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.aq2.json
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.json
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.aq2.json
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.json
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_natgas.json
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.acn03.json
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.json
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq2.json
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq3.json
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.json
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_wleak.aq1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.switch.b1lacn02.json
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.switch.b2lacn02.json
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.switch.b2lc04.json
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.switch.l1aeu1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.switch.l2aeu1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.switch.n1aeu1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.vibration.aq1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.weather.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.562126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Cable outlet.json
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Connected outlet.json
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/DIN power consumption module.json
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Dimmer switch wo neutral.json
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Double gangs remote switch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Micromodule switch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Mobile outlet.json
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Remote motion sensor.json
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Remote switch Wake up Sleep.json
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Remote switch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Remote toggle switch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Shutter switch with neutral.json
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Shutters central remote switch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Teleruptor.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.562126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Lixee/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Lixee/WS2812_light_controller.json
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-mono.json
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-tri.json
--rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono-prod.json
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono.json
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri-prod.json
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri.json
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Lixee/ZLinky_TIC.json
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Lixee/Zigate-Router.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.562126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Nexturn/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Nexturn/VOC_Sensor.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.562126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Nodon/
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20.json
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20_PRO.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.566126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/OSRAM/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/OSRAM/CLA60 TW OSRAM.json
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/OSRAM/Classic A60 W clear - LIGHTIFY.json
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/OSRAM/LEDVANCE DIM.json
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Indoor Flex RGBW.json
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Outdoor Flex RGBW.json
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/OSRAM/Lightify Switch Mini.json
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/OSRAM/PAR16 50 TW.json
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/OSRAM/Plug 01.json
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/OSRAM/Plug Z3.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.566126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Orvibo/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Orvibo/396483ce8b3f4e0d8e9d79079a35a420.json
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Orvibo/3c4e4fc81ed442efaf69353effcdfc5f.json
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Orvibo/50938c4c3c0b4049923cd5afbc151bde.json
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Orvibo/82c167c95ed746cdbd21d6817f72c593.json
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Orvibo/898ca74409a740b28d5841661e72268d.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.566126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/BDP3001.json
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/Dimmablelight.json
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/EcoDim-Zigbee 3.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/FB56-ZCW08KU1.1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB1.6.json
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB2.1.json
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/FNB56-ZSW01LX2.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/FNB56-ZSW02LX2.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/Lamp_01.json
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/NUET56-DL27LX1.1.json
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/SA-003-Zigbee.json
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/VMS_ADUROLIGHT.json
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/ZB-CL01.json
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/ZB-CT01.json
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/ZB-ONOFFPlug-D0005.json
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/ZB-SW01.json
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/ZB-SW02.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.570126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/AC201A.json
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/AC211.json
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/AC221.json
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/CB432.json
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/DWS312-E.json
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/DWS312.json
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/KF204.json
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/KF205.json
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/PB206.json
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/PC321.json
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/PIR323-A.json
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/PIR323.json
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/PR412.json
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/THS317-ET.json
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/THS317.json
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/VBS308.json
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/WSP402.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.570126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/440400982841.json
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/440400982842.json
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/929003052501_01.json
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/929003052501_02.json
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/929003053301_01.json
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/929003053301_02.json
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LCA001.json
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LCT001.json
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LCT003.json
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LCT007.json
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LCT010.json
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LCT015.json
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LCT024.json
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LLC010.json
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LOM002.json
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LOM008.json
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LST002.json
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LTA001.json
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LTC001.json
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LTG002.json
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LTW001.json
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LTW004.json
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LTW013.json
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LWA001.json
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LWA009.json
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LWB006.json
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LWB010.json
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/ROM001.json
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/RWL021.json
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/SML001.json
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/SML002.json
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/SML003.json
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/SML004.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.574126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Profalux/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Profalux/BSO-Profalux.json
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Profalux/MAI-ZTS.json
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Profalux/MOT-C1Z06C.json
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Profalux/MOT-C1Z06F.json
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Profalux/Telecommande-Profalux.json
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Profalux/Volet-Profalux.json
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Profalux/VoletBSO-Profalux.json
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.574126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Robb-Smarrt/
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Robb-Smarrt/ROB_200-017-0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.574126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/SALUS/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/SALUS/SPE600.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.574126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Samotech/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Samotech/SM309.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.574126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/1GANGSHUTTER1.json
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/CCT592011_AS.json
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/EH-ZB-BMS.json
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/EH-ZB-HACT.json
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/EH-ZB-LMACT.json
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/EH-ZB-RTS.json
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD-V2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD.json
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/EH-ZB-VACT.json
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/NHPBSHUTTER1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/PUCKDIMMER1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/PUCKSHUTTER1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/PUCKSWITCH1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/Wiser2-Thermostat.json
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/iTRV.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.574126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/SmartThings/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/SmartThings/outletv4.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.578126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sonoff/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sonoff/01MINIZB.json
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sonoff/66666.json
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sonoff/BASICZBR3.json
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sonoff/DONGLE-E_R.json
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sonoff/DS-01.json
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sonoff/DS01.json
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sonoff/MS01.json
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sonoff/MSO1.json
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sonoff/S26R2ZB.json
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sonoff/SNZB-02D.json
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sonoff/TH01.json
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sonoff/WB-01.json
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sonoff/WB01.json
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sonoff/ZBMINI-L.json
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sonoff/ZBMINI-L2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.578126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sunricher/
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sunricher/ZG2858A.json
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sunricher/ZG9101SAC-HP.json
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sunricher/ZGRC-KEY-013.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.578126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/TDURM0D01/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/TDURM0D01/ZBT-Remote-ALL-RGBW.json
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/TDURM0D01/tint-ExtendedColor.json
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/TDURM0D01/tint-Remote-white.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.578126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/TUYATEC/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/TUYATEC/RH3001.json
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/TUYATEC/RH3040.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.586126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0001.json
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0002.json
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0002_relay_switch.json
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0003-QS-Zigbee-S05-LN.json
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0003.json
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0003_relay_switch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_excgg5kb.json
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_u3oupgdy.json
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0011.json
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0012.json
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0013.json
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0041.json
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0042.json
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0043.json
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0044.json
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0046.json
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS004F-_TZ3000_xabckq1v.json
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS004F.json
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0112.json
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0115.json
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS011F-2Gang-switches.json
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS011F-_TZ3000_zmy1waw6.json
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS011F-din.json
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS011F-multiprise.json
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS011F-plug.json
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS011F.json
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0121.json
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_mxzo5rhf.json
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_qaaysllp.json
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0201.json
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0202-_TZ3210_jijr1sss.json
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0202.json
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0203.json
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0205.json
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0207-extender.json
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0207-waterleak.json
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0211.json
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0215A-secure-remote.json
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0215A-sos.json
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0222.json
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0302.json
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0502A.json
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0505A.json
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0505B.json
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-2Gangs-dimmer.json
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-2Gangs-switch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-Clamp-Meter.json
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-Energy.json
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-Parkside-Watering-Timer.json
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-SmartAir.json
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-Solar-Siren.json
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_b6wax7g0.json
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_chyvmhay.json
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_dzuqwsyg.json
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_nklqjk62.json
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_t1blo2bj.json
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-curtain.json
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-dimmer.json
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-eTRV.json
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-eTRV1.json
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-eTRV2.json
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-eTRV3.json
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-eTRV5.json
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-eTRV6.json
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-motion.json
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-radar.json
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-sirene.json
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-smoke.json
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-switch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-temphumi-2.json
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-temphumi.json
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-thermostat.json
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS1001.json
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS110E-_QS-Zigbee-D02-TRIAC-LN.json
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS110E-_TZ3210_weaqkhab.json
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS110F-_TYZB01_qezuin6k.json
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS110F-_TZ3000_ktuoyvt5.json
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Blind.json
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Vanne.json
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi.json
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_8kzqqzu4.json
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_dph3rpss.json
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_femsaaua.json
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_fvhunhxb.json
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_zirycpws.json
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TY0202.json
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/fvq6avy.json
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/ivfvd7h.json
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/kud7u2l.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.586126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Woolley/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Woolley/SA-029-1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.586126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Ynoa/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Ynoa/ZBT-CCTLight-A0001.json
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Ynoa/ZBT-CCTLight-GU100001.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.586126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Ysrai/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Ysrai/ZB-CL01.json
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Ysrai/ZB-CT01.json
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Ysrai/ZB-DL01.json
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Ysrai/ZB-SW01.json
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Ysrai/ZB-SW02.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.586126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Zehnder/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Zehnder/TAFFETAS2 D1.00P1.01Z1.00.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.586126 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Zemismart/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/Certified/Zemismart/LXN56-DC27LX1.1.json
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-01 16:56:29.000000 z4d-certified-devices-2.56/z4d_certified_devices/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:56:40.518127 z4d-certified-devices-2.56/z4d_certified_devices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36120 2023-05-01 16:56:40.000000 z4d-certified-devices-2.56/z4d_certified_devices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27476 2023-05-01 16:56:40.000000 z4d-certified-devices-2.56/z4d_certified_devices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:56:40.000000 z4d-certified-devices-2.56/z4d_certified_devices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-01 16:56:40.000000 z4d-certified-devices-2.56/z4d_certified_devices.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:56:40.000000 z4d-certified-devices-2.56/z4d_certified_devices.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.664714 z4d-certified-devices-2.57/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    36120 2023-05-08 19:42:18.668714 z4d-certified-devices-2.57/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-08 19:42:18.668714 z4d-certified-devices-2.57/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.560715 z4d-certified-devices-2.57/z4d_certified_devices/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.564715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.564715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Adeo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Adeo/LDSENK02F.json
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Adeo/LDSENK10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Adeo/LXEK-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Adeo/LXEK-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Adeo/LXEK-7.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Adeo/ZBEK-14.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Adeo/ZBEK-3.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.564715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Aotec/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Aotec/WG001-Z01.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.568715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Bitron/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Bitron/90201021A.json
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Bitron/90201021B.json
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Bitron/90201024.json
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Bitron/AV201021B.json
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Bitron/AV201024A.json
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Bitron/AV201029A.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.568715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/CLEODE/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/CLEODE/ZHUM.json
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/CLEODE/ZMOVE.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/CLEODE/ZPLUG.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.572715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CAC221.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CCB432.json
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CDWS312.json
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CKF204.json
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CKF205.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CMS323.json
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CPB206.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CPC321.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CPR412-E.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CPR412.json
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CSAC451-E.json
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CSAC451-WTC-E.json
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CSLC601-D-E.json
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CSLC601-E.json
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CSLC631-3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CSP403.json
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CTHS317ET.json
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/Dual_Relay_Module.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.572715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Danalock/
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Danalock/V3-BTZB.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.572715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Danfoss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Danfoss/RV001.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Danfoss/eT093WRG.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Danfoss/eT093WRO.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Danfoss/eTRV0100.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.572715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Develco/
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Develco/HESZB120.json
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Develco/HMSZB-110.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Develco/MOSZB-140.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Develco/SMSZB-120.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Develco/SPLZB-131.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Develco/SPLZB-132.json
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Develco/ZHEMI101.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.576715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/ENKI-LEXMAN/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-7.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.576715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Eurotronics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Eurotronics/SPZB0001.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.576715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-B-004P.json
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-B-007Z.json
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008Z.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008ZS.json
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007-2ID.json
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007.json
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008.json
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008S.json
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008Z.json
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-C-009.json
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-D-003Z.json
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-FL-004TZS.json
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-MC-001.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-S-007ZS.json
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GLEDOPTO.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.584715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/COSensor-EF-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/COSensor-EM.json
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/COSensor-N.json
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/CO_V15.json
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/CO_YDLV10.json
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/GASSensor-EF-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/GAS_V15.json
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/RC-EF-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/RC-EM.json
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/SMOK_V16.json
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/SMOK_YDLV10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/SRHMP-I1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/SceneSwitch-EM-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/SmartPlug.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/SmokeSensor-EF-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/SmokeSensor-EM.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/SmokeSensor-N-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/SmokeSensor-N.json
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/TS0216.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/WarningDevice-EF-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/WarningDevice.json
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/WaterSensor-EF-3.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.592715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 30x90.json
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 60x60.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/FYRTUR block-out roller blind.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/KADRILJ roller blind.json
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/Remote Control N2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/STARKVIND Air purifier.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/STOFTMOLN ceilingwall lamp WW24.json
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 10W.json
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 30W.json
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI SHORTCUT Button.json
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Signal Repeater.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E12 WS opal 400lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 W opch 400lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS 470lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 400lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 600lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS clear 950lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS opal 980lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS 806lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS opal 600lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 W opal 1000lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 806lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 950lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 1000lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 950lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 980lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW 806lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW clear 250lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 opal 1000lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 W 400lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WS 400lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WW 400lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI control outlet.json
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI motion sensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI onoff switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI openclose remote.json
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI remote control.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI transformer 10W.json
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI wireless dimmer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE14WScandleopal470lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbGU10WS345lm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/VINDSTYRKA.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.592715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/INNR/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/INNR/OSL 130 C.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/INNR/RB 248 T.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/INNR/RB 285 C.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/INNR/SP 120.json
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/INNR/SP 220.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.592715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Idinio/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Idinio/Dimmer-Switch-ZB3.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.596715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Iluminize/
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Iluminize/511.201.json
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Iluminize/5120.1200.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.596715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Konke/
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Konke/3AFE140103020000.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Konke/3AFE14010402000D.json
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Konke/3AFE170100510001.json
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Konke/3AFE220103020000.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Konke/3AFE28010402000D.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.596715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LIVOLO/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LIVOLO/TI0001.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.596715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LS-Deutschland-GmbH/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LS-Deutschland-GmbH/Emotion.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.608715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.airmonitor.acn01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.aq1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.aq1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.light.aqcn02.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.lock.v1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.magnet.acn001.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.motion.ac01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.motion.ac02.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.plug.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.plug.maeu01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.plug.mmeu01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.relay.c2acn01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn02.json
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b1acn01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn02.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01-bulb.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b28ac1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01-bulb.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01-bulb.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.router.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sen_ill.mgl01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sens.json
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.aqgl01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.json
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_ht.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.acn001.json
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.aq2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.aq2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.json
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_natgas.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.acn03.json
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.json
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_wleak.aq1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.switch.b1lacn02.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.switch.b2lacn02.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.switch.b2lc04.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.switch.l1aeu1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.switch.l2aeu1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.switch.n1aeu1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.vibration.aq1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.weather.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.612715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Cable outlet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Connected outlet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/DIN power consumption module.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Dimmer switch wo neutral.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Double gangs remote switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Micromodule switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Mobile outlet.json
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Remote motion sensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Remote switch Wake up Sleep.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Remote switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Remote toggle switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Shutter switch with neutral.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Shutters central remote switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Teleruptor.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.612715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Lixee/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Lixee/WS2812_light_controller.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-mono.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-tri.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono-prod.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri-prod.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Lixee/ZLinky_TIC.json
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Lixee/Zigate-Router.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.612715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Nexturn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Nexturn/VOC_Sensor.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.616715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Nodon/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20_PRO.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.616715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/OSRAM/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/OSRAM/CLA60 TW OSRAM.json
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/OSRAM/Classic A60 W clear - LIGHTIFY.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/OSRAM/LEDVANCE DIM.json
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Indoor Flex RGBW.json
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Outdoor Flex RGBW.json
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/OSRAM/Lightify Switch Mini.json
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/OSRAM/PAR16 50 TW.json
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/OSRAM/Plug 01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/OSRAM/Plug Z3.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.616715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Orvibo/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Orvibo/396483ce8b3f4e0d8e9d79079a35a420.json
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Orvibo/3c4e4fc81ed442efaf69353effcdfc5f.json
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Orvibo/50938c4c3c0b4049923cd5afbc151bde.json
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Orvibo/82c167c95ed746cdbd21d6817f72c593.json
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Orvibo/898ca74409a740b28d5841661e72268d.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.620715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/BDP3001.json
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/Dimmablelight.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/EcoDim-Zigbee 3.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/FB56-ZCW08KU1.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB1.6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB2.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/FNB56-ZSW01LX2.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/FNB56-ZSW02LX2.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/Lamp_01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/NUET56-DL27LX1.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/SA-003-Zigbee.json
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/VMS_ADUROLIGHT.json
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/ZB-CL01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/ZB-CT01.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/ZB-ONOFFPlug-D0005.json
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/ZB-SW01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/ZB-SW02.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.624715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/AC201A.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/AC211.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/AC221.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/CB432.json
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/DWS312-E.json
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/DWS312.json
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/KF204.json
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/KF205.json
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/PB206.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/PC321.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/PIR323-A.json
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/PIR323.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/PR412.json
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/THS317-ET.json
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/THS317.json
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/VBS308.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/WSP402.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.632715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/440400982841.json
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/440400982842.json
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/929003052501_01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/929003052501_02.json
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/929003053301_01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/929003053301_02.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LCA001.json
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LCT001.json
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LCT003.json
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LCT007.json
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LCT010.json
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LCT015.json
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LCT024.json
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LLC010.json
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LOM002.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LOM008.json
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LST002.json
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LTA001.json
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LTC001.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LTG002.json
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LTW001.json
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LTW004.json
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LTW013.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LWA001.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LWA009.json
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LWB006.json
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LWB010.json
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/ROM001.json
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/RWL021.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/SML001.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/SML002.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/SML003.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/SML004.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.632715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Profalux/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Profalux/BSO-Profalux.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Profalux/MAI-ZTS.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Profalux/MOT-C1Z06C.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Profalux/MOT-C1Z06F.json
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Profalux/Telecommande-Profalux.json
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Profalux/Volet-Profalux.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Profalux/VoletBSO-Profalux.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.632715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Robb-Smarrt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Robb-Smarrt/ROB_200-017-0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.636715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/SALUS/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/SALUS/SPE600.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.636715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Samotech/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Samotech/SM309.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.640715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/1GANGSHUTTER1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/CCT592011_AS.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/EH-ZB-BMS.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/EH-ZB-HACT.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/EH-ZB-LMACT.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/EH-ZB-RTS.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD-V2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/EH-ZB-VACT.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/NHPBSHUTTER1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/PUCKDIMMER1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/PUCKSHUTTER1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/PUCKSWITCH1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/Wiser2-Thermostat.json
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/iTRV.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.640715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/SmartThings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/SmartThings/outletv4.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.640715 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sonoff/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sonoff/01MINIZB.json
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sonoff/66666.json
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sonoff/BASICZBR3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sonoff/DONGLE-E_R.json
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sonoff/DS-01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sonoff/DS01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sonoff/MS01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sonoff/MSO1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sonoff/S26R2ZB.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sonoff/SNZB-02D.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sonoff/TH01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sonoff/WB-01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sonoff/WB01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sonoff/ZBMINI-L.json
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sonoff/ZBMINI-L2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.644714 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sunricher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sunricher/ZG2858A.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sunricher/ZG9101SAC-HP.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sunricher/ZGRC-KEY-013.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.644714 z4d-certified-devices-2.57/z4d_certified_devices/Certified/TDURM0D01/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/TDURM0D01/ZBT-Remote-ALL-RGBW.json
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/TDURM0D01/tint-ExtendedColor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/TDURM0D01/tint-Remote-white.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.644714 z4d-certified-devices-2.57/z4d_certified_devices/Certified/TUYATEC/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/TUYATEC/RH3001.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/TUYATEC/RH3040.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.664714 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0001.json
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0002.json
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0002_relay_switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0003-QS-Zigbee-S05-LN.json
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0003.json
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0003_relay_switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_excgg5kb.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_u3oupgdy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0011.json
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0012.json
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0013.json
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0041.json
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0042.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0043.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0044.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0046.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS004F-_TZ3000_xabckq1v.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS004F.json
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0112.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0115.json
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS011F-2Gang-switches.json
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS011F-_TZ3000_zmy1waw6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS011F-din.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS011F-multiprise.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS011F-plug.json
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS011F.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0121.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_mxzo5rhf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_qaaysllp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0201.json
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0202-_TZ3210_jijr1sss.json
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0202.json
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0203.json
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0205.json
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0207-extender.json
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0207-waterleak.json
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0211.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0215A-secure-remote.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0215A-sos.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0219.json
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0222.json
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0302.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0502A.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0505A.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0505B.json
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-2Gangs-dimmer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-2Gangs-switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-Clamp-Meter.json
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-Energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-Parkside-Watering-Timer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-SmartAir.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-Solar-Siren.json
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_b6wax7g0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_chyvmhay.json
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_dzuqwsyg.json
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_nklqjk62.json
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_t1blo2bj.json
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-curtain.json
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-dimmer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-eTRV.json
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-eTRV1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-eTRV2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-eTRV3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-eTRV5.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-eTRV6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-motion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-radar.json
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-sirene.json
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-smoke.json
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-switch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-temphumi-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-temphumi.json
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-thermostat.json
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS1001.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS110E-_QS-Zigbee-D02-TRIAC-LN.json
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS110E-_TZ3210_weaqkhab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS110F-_TYZB01_qezuin6k.json
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS110F-_TZ3000_ktuoyvt5.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Blind.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Vanne.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_8kzqqzu4.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_dph3rpss.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_femsaaua.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_fvhunhxb.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_zirycpws.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TY0202.json
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/fvq6avy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/ivfvd7h.json
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/kud7u2l.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.664714 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Woolley/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Woolley/SA-029-1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.664714 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Ynoa/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Ynoa/ZBT-CCTLight-A0001.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Ynoa/ZBT-CCTLight-GU100001.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.664714 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Ysrai/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Ysrai/ZB-CL01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Ysrai/ZB-CT01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Ysrai/ZB-DL01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Ysrai/ZB-SW01.json
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Ysrai/ZB-SW02.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.664714 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Zehnder/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Zehnder/TAFFETAS2 D1.00P1.01Z1.00.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.664714 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Zemismart/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/Certified/Zemismart/LXN56-DC27LX1.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-08 19:42:07.000000 z4d-certified-devices-2.57/z4d_certified_devices/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:42:18.564715 z4d-certified-devices-2.57/z4d_certified_devices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36120 2023-05-08 19:42:18.000000 z4d-certified-devices-2.57/z4d_certified_devices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27525 2023-05-08 19:42:18.000000 z4d-certified-devices-2.57/z4d_certified_devices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:42:18.000000 z4d-certified-devices-2.57/z4d_certified_devices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 19:42:18.000000 z4d-certified-devices-2.57/z4d_certified_devices.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:42:18.000000 z4d-certified-devices-2.57/z4d_certified_devices.egg-info/zip-safe
```

### Comparing `z4d-certified-devices-2.56/LICENSE.txt` & `z4d-certified-devices-2.57/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/PKG-INFO` & `z4d-certified-devices-2.57/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z4d-certified-devices
-Version: 2.56
+Version: 2.57
 Summary: "Certified devices for Zigbee for Domoticz plugin"
 Home-page: https://github.com/zigbeefordomoticz/z4d-certified-devices
 Author: "Patrick Pichon"
 Author-email: "patrick@pichon.me"
 License: "GPL-3.0"
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `z4d-certified-devices-2.56/README.md` & `z4d-certified-devices-2.57/README.md`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/setup.cfg` & `z4d-certified-devices-2.57/setup.cfg`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Adeo/LDSENK02F.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Adeo/LDSENK02F.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Adeo/LDSENK10.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Adeo/LDSENK10.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Adeo/LXEK-1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Adeo/LXEK-1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Adeo/LXEK-2.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Adeo/LXEK-2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Adeo/LXEK-7.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Adeo/LXEK-7.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Adeo/ZBEK-14.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Adeo/ZBEK-14.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Adeo/ZBEK-3.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Adeo/ZBEK-3.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Aotec/WG001-Z01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Aotec/WG001-Z01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Bitron/90201021A.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Bitron/90201021A.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Bitron/AV201024A.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Bitron/AV201024A.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Bitron/AV201029A.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Bitron/AV201029A.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/CLEODE/ZHUM.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/CLEODE/ZHUM.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/CLEODE/ZMOVE.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/CLEODE/ZMOVE.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/CLEODE/ZPLUG.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/CLEODE/ZPLUG.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CAC221.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CAC221.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CCB432.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CCB432.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CDWS312.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CDWS312.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CKF205.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CKF205.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CMS323.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CMS323.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CPC321.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CPC321.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CPR412-E.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CPR412-E.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CPR412.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CPR412.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CSAC451-E.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CSAC451-E.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CSAC451-WTC-E.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CSAC451-WTC-E.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CSLC601-D-E.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CSLC601-D-E.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CSLC601-E.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CSLC601-E.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CSLC631-3.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CSLC631-3.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CSP403.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CSP403.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/CTHS317ET.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/CTHS317ET.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Casa.ia/Dual_Relay_Module.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Casa.ia/Dual_Relay_Module.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Danalock/V3-BTZB.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Danalock/V3-BTZB.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Danfoss/RV001.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Danfoss/RV001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Danfoss/eT093WRG.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Danfoss/eT093WRG.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Danfoss/eT093WRO.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Danfoss/eT093WRO.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Danfoss/eTRV0100.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Danfoss/eTRV0100.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Develco/HESZB120.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Develco/HESZB120.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Develco/HMSZB-110.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Develco/HMSZB-110.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Develco/MOSZB-140.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Develco/MOSZB-140.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Develco/SMSZB-120.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Develco/SMSZB-120.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Develco/SPLZB-131.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Develco/SPLZB-131.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Develco/SPLZB-132.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Develco/SPLZB-132.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Develco/ZHEMI101.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Develco/ZHEMI101.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-2.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-7.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-7.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Eurotronics/SPZB0001.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Eurotronics/SPZB0001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-B-004P.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-B-004P.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-B-007Z.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-B-007Z.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008Z.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008Z.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008ZS.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008ZS.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007-2ID.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007-2ID.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008S.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008S.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008Z.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008Z.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-C-009.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-C-009.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-D-003Z.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-D-003Z.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-FL-004TZS.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-FL-004TZS.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-MC-001.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-MC-001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GL-S-007ZS.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GL-S-007ZS.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/GLEDOPTO/GLEDOPTO.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/GLEDOPTO/GLEDOPTO.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/COSensor-EM.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/COSensor-EM.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/GASSensor-EF-3.0.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/GASSensor-EF-3.0.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/RC-EF-3.0.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/RC-EF-3.0.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/RC-EM.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/RC-EM.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/SRHMP-I1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/SRHMP-I1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/SceneSwitch-EM-3.0.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/SceneSwitch-EM-3.0.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/SmartPlug.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/SmartPlug.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/SmokeSensor-EM.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/SmokeSensor-EM.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/TS0216.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/TS0216.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/WarningDevice-EF-3.0.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/WarningDevice-EF-3.0.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/WarningDevice.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/WarningDevice.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Heiman/WaterSensor-EF-3.0.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Heiman/WaterSensor-EF-3.0.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 30x90.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 30x90.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 60x60.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 60x60.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/FYRTUR block-out roller blind.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/FYRTUR block-out roller blind.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/KADRILJ roller blind.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/KADRILJ roller blind.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/Remote Control N2.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/Remote Control N2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/STARKVIND Air purifier.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/STARKVIND Air purifier.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/STOFTMOLN ceilingwall lamp WW24.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/STOFTMOLN ceilingwall lamp WW24.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 10W.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 10W.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 30W.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 30W.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI SHORTCUT Button.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI SHORTCUT Button.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Signal Repeater.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Signal Repeater.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E12 WS opal 400lm.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E12 WS opal 400lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 W opch 400lm.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 W opch 400lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS 470lm.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS 470lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 400lm.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 400lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 600lm.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 600lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS clear 950lm.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS clear 950lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS opal 980lm.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS opal 980lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS 806lm.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS 806lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS opal 600lm.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS opal 600lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 W opal 1000lm.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 W opal 1000lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 806lm.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 806lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 950lm.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 950lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 1000lm.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 1000lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 950lm.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 950lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 980lm.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 980lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW 806lm.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW 806lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW clear 250lm.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW clear 250lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 opal 1000lm.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 opal 1000lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 W 400lm.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 W 400lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WS 400lm.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WS 400lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WW 400lm.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WW 400lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI control outlet.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI control outlet.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI motion sensor.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI motion sensor.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI onoff switch.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI onoff switch.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI openclose remote.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI openclose remote.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI remote control.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI remote control.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI transformer 10W.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI transformer 10W.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE14WScandleopal470lm.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE14WScandleopal470lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbGU10WS345lm.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbGU10WS345lm.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/IKEA_TRADFRI/VINDSTYRKA.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/IKEA_TRADFRI/VINDSTYRKA.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/INNR/OSL 130 C.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/INNR/OSL 130 C.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/INNR/RB 248 T.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/INNR/RB 248 T.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/INNR/RB 285 C.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/INNR/RB 285 C.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/INNR/SP 120.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/INNR/SP 120.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/INNR/SP 220.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/INNR/SP 220.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Idinio/Dimmer-Switch-ZB3.0.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Idinio/Dimmer-Switch-ZB3.0.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Iluminize/511.201.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Iluminize/511.201.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Iluminize/5120.1200.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Iluminize/5120.1200.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Konke/3AFE140103020000.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Konke/3AFE140103020000.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Konke/3AFE14010402000D.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Konke/3AFE14010402000D.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Konke/3AFE170100510001.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Konke/3AFE170100510001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Konke/3AFE220103020000.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Konke/3AFE220103020000.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Konke/3AFE28010402000D.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Konke/3AFE28010402000D.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LIVOLO/TI0001.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LIVOLO/TI0001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LS-Deutschland-GmbH/Emotion.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LS-Deutschland-GmbH/Emotion.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.airmonitor.acn01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.airmonitor.acn01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.aq1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.aq1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.aq1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.aq1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral2.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.light.aqcn02.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.light.aqcn02.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.lock.v1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.lock.v1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.magnet.acn001.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.magnet.acn001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.motion.ac01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.motion.ac01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.motion.ac02.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.motion.ac02.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.plug.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.plug.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.plug.maeu01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.plug.maeu01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.plug.mmeu01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.plug.mmeu01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.relay.c2acn01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.relay.c2acn01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn02.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn02.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b1acn01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b1acn01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn02.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn02.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01-bulb.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01-bulb.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b28ac1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b28ac1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01-bulb.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01-bulb.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01-bulb.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01-bulb.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.router.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.router.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sen_ill.mgl01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sen_ill.mgl01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sens.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sens.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw2.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.aqgl01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.aqgl01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_ht.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_ht.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.acn001.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.acn001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.aq2.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.aq2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.aq2.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.aq2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_natgas.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_natgas.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.acn03.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.acn03.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq2.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq3.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq3.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.sensor_wleak.aq1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.sensor_wleak.aq1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.switch.b1lacn02.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.switch.b1lacn02.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.switch.b2lacn02.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.switch.b2lacn02.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.switch.b2lc04.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.switch.b2lc04.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.switch.l1aeu1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.switch.l1aeu1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.switch.l2aeu1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.switch.l2aeu1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.switch.n1aeu1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.switch.n1aeu1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.vibration.aq1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.vibration.aq1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/LUMI/lumi.weather.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/LUMI/lumi.weather.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Cable outlet.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Cable outlet.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Connected outlet.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Connected outlet.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/DIN power consumption module.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/DIN power consumption module.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Dimmer switch wo neutral.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Dimmer switch wo neutral.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Double gangs remote switch.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Double gangs remote switch.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Micromodule switch.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Micromodule switch.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Mobile outlet.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Mobile outlet.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Remote motion sensor.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Remote motion sensor.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Remote switch Wake up Sleep.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Remote switch Wake up Sleep.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Remote switch.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Remote switch.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Remote toggle switch.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Remote toggle switch.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Shutter switch with neutral.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Shutter switch with neutral.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Shutters central remote switch.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Shutters central remote switch.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Legrand/Teleruptor.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Legrand/Teleruptor.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Lixee/WS2812_light_controller.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Lixee/WS2812_light_controller.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-mono.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-mono.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-tri.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-tri.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono-prod.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono-prod.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri-prod.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri-prod.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Lixee/ZLinky_TIC.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Lixee/ZLinky_TIC.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Lixee/Zigate-Router.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Lixee/Zigate-Router.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Nexturn/VOC_Sensor.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Nexturn/VOC_Sensor.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20_PRO.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20_PRO.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/OSRAM/CLA60 TW OSRAM.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/OSRAM/CLA60 TW OSRAM.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/OSRAM/Classic A60 W clear - LIGHTIFY.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/OSRAM/Classic A60 W clear - LIGHTIFY.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/OSRAM/LEDVANCE DIM.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/OSRAM/LEDVANCE DIM.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Indoor Flex RGBW.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Indoor Flex RGBW.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Outdoor Flex RGBW.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Outdoor Flex RGBW.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/OSRAM/Lightify Switch Mini.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/OSRAM/Lightify Switch Mini.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/OSRAM/PAR16 50 TW.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/OSRAM/PAR16 50 TW.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/OSRAM/Plug 01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/OSRAM/Plug 01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/OSRAM/Plug Z3.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/OSRAM/Plug Z3.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Orvibo/396483ce8b3f4e0d8e9d79079a35a420.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Orvibo/396483ce8b3f4e0d8e9d79079a35a420.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Orvibo/50938c4c3c0b4049923cd5afbc151bde.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Orvibo/50938c4c3c0b4049923cd5afbc151bde.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Orvibo/82c167c95ed746cdbd21d6817f72c593.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Orvibo/82c167c95ed746cdbd21d6817f72c593.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Orvibo/898ca74409a740b28d5841661e72268d.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Orvibo/898ca74409a740b28d5841661e72268d.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/BDP3001.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/BDP3001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/Dimmablelight.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/Dimmablelight.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/EcoDim-Zigbee 3.0.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/EcoDim-Zigbee 3.0.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB1.6.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB1.6.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB2.1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB2.1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/FNB56-ZSW01LX2.0.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/FNB56-ZSW01LX2.0.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/FNB56-ZSW02LX2.0.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/FNB56-ZSW02LX2.0.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/Lamp_01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/Lamp_01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/NUET56-DL27LX1.1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/NUET56-DL27LX1.1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/VMS_ADUROLIGHT.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/VMS_ADUROLIGHT.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/ZB-CL01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/ZB-CL01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/ZB-CT01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/ZB-CT01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/ZB-ONOFFPlug-D0005.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/ZB-ONOFFPlug-D0005.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Others/ZB-SW02.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Others/ZB-SW02.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/AC201A.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/AC201A.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/AC211.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/AC211.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/AC221.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/AC221.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/CB432.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/CB432.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/DWS312-E.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/DWS312-E.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/KF205.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/KF205.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/PC321.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/PC321.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/PIR323-A.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/PIR323-A.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/PIR323.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/PIR323.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/PR412.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/PR412.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/THS317-ET.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/THS317-ET.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Owon/WSP402.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Owon/WSP402.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/440400982841.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/440400982841.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/440400982842.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/440400982842.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/929003052501_01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/929003052501_01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/929003052501_02.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/929003052501_02.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/929003053301_01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/929003053301_01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/929003053301_02.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/929003053301_02.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LCA001.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LCA001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LCT001.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LCT001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LCT003.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LCT003.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LCT007.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LCT007.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LCT010.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LCT010.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LCT015.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LCT015.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LCT024.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LCT024.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LLC010.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LLC010.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LOM008.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LOM008.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LST002.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LST002.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LTA001.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LTA001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LTC001.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LTC001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LTG002.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LTG002.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LTW001.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LTW001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LTW004.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LTW004.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LTW013.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LTW013.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LWA001.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LWA001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LWA009.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LWA009.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LWB006.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LWB006.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/LWB010.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/LWB010.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/ROM001.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/ROM001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/RWL021.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/RWL021.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/SML001.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/SML001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/SML002.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/SML002.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/SML003.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/SML003.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Philips/SML004.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Philips/SML004.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Profalux/BSO-Profalux.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Profalux/BSO-Profalux.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Profalux/MAI-ZTS.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Profalux/MAI-ZTS.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Profalux/MOT-C1Z06C.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Profalux/MOT-C1Z06C.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Profalux/MOT-C1Z06F.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Profalux/MOT-C1Z06F.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Profalux/Telecommande-Profalux.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Profalux/Telecommande-Profalux.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Profalux/Volet-Profalux.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Profalux/Volet-Profalux.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Profalux/VoletBSO-Profalux.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Profalux/VoletBSO-Profalux.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/README.md` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/README.md`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Robb-Smarrt/ROB_200-017-0.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Robb-Smarrt/ROB_200-017-0.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/SALUS/SPE600.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/SALUS/SPE600.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Samotech/SM309.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Samotech/SM309.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/1GANGSHUTTER1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/1GANGSHUTTER1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/CCT592011_AS.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/CCT592011_AS.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/EH-ZB-BMS.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/EH-ZB-BMS.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/EH-ZB-HACT.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/EH-ZB-HACT.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/EH-ZB-LMACT.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/EH-ZB-LMACT.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/EH-ZB-RTS.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/EH-ZB-RTS.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD-V2.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD-V2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/EH-ZB-VACT.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/EH-ZB-VACT.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/NHPBSHUTTER1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/NHPBSHUTTER1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/PUCKDIMMER1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/PUCKDIMMER1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/PUCKSHUTTER1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/PUCKSHUTTER1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/PUCKSWITCH1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/PUCKSWITCH1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET2.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/Wiser2-Thermostat.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/Wiser2-Thermostat.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Schneider/iTRV.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Schneider/iTRV.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/SmartThings/outletv4.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/SmartThings/outletv4.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sonoff/01MINIZB.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sonoff/01MINIZB.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sonoff/66666.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sonoff/66666.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sonoff/S26R2ZB.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sonoff/S26R2ZB.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sonoff/SNZB-02D.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sonoff/SNZB-02D.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sonoff/TH01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sonoff/TH01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sonoff/ZBMINI-L2.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sonoff/ZBMINI-L2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sunricher/ZG2858A.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sunricher/ZG2858A.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sunricher/ZG9101SAC-HP.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sunricher/ZG9101SAC-HP.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Sunricher/ZGRC-KEY-013.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Sunricher/ZGRC-KEY-013.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/TDURM0D01/ZBT-Remote-ALL-RGBW.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/TDURM0D01/ZBT-Remote-ALL-RGBW.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/TDURM0D01/tint-ExtendedColor.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/TDURM0D01/tint-ExtendedColor.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/TDURM0D01/tint-Remote-white.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/TDURM0D01/tint-Remote-white.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/TUYATEC/RH3040.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/TUYATEC/RH3040.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0001.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0002.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0002.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0002_relay_switch.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0002_relay_switch.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0003.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0003.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0003_relay_switch.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0003_relay_switch.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_excgg5kb.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_excgg5kb.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_u3oupgdy.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_u3oupgdy.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0011.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0011.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0012.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0012.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0013.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0013.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0041.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0041.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0042.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0042.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0043.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0043.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0044.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0044.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0046.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0046.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS004F-_TZ3000_xabckq1v.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS004F-_TZ3000_xabckq1v.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS004F.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS004F.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0112.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0112.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0115.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0115.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS011F-2Gang-switches.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS011F-2Gang-switches.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS011F-_TZ3000_zmy1waw6.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS011F-_TZ3000_zmy1waw6.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS011F-din.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS011F-din.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS011F-multiprise.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS011F-multiprise.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS011F-plug.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS011F-plug.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS011F.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS011F.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0121.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0121.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_mxzo5rhf.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_mxzo5rhf.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_qaaysllp.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_qaaysllp.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0202-_TZ3210_jijr1sss.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0202-_TZ3210_jijr1sss.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0202.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0202.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0207-extender.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0207-extender.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0207-waterleak.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0207-waterleak.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0215A-secure-remote.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0215A-secure-remote.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0215A-sos.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0215A-sos.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0222.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0222.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0302.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0302.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0502A.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0502A.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0505A.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0505A.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0505B.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0505B.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-2Gangs-dimmer.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-2Gangs-dimmer.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-Clamp-Meter.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-Clamp-Meter.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-Energy.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-Energy.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-Parkside-Watering-Timer.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-Parkside-Watering-Timer.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-Solar-Siren.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-Solar-Siren.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_b6wax7g0.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_b6wax7g0.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_dzuqwsyg.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_dzuqwsyg.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_nklqjk62.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_nklqjk62.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_t1blo2bj.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_t1blo2bj.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-dimmer.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-dimmer.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-eTRV5.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-eTRV5.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-eTRV6.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-eTRV6.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-motion.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-motion.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-radar.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-radar.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-sirene.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-sirene.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-temphumi-2.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-temphumi-2.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-temphumi.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-temphumi.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS0601-thermostat.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS0601-thermostat.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS1001.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS1001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS110E-_QS-Zigbee-D02-TRIAC-LN.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS110E-_QS-Zigbee-D02-TRIAC-LN.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS110E-_TZ3210_weaqkhab.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS110E-_TZ3210_weaqkhab.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS110F-_TYZB01_qezuin6k.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS110F-_TYZB01_qezuin6k.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS110F-_TZ3000_ktuoyvt5.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS110F-_TZ3000_ktuoyvt5.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Blind.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Blind.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Vanne.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Vanne.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_8kzqqzu4.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_8kzqqzu4.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_dph3rpss.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_dph3rpss.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_femsaaua.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_femsaaua.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_fvhunhxb.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_fvhunhxb.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_zirycpws.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_zirycpws.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Tuya/TY0202.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Tuya/TY0202.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Woolley/SA-029-1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Woolley/SA-029-1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Ynoa/ZBT-CCTLight-A0001.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Ynoa/ZBT-CCTLight-A0001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Ynoa/ZBT-CCTLight-GU100001.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Ynoa/ZBT-CCTLight-GU100001.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Ysrai/ZB-CL01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Ysrai/ZB-CL01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Ysrai/ZB-CT01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Ysrai/ZB-CT01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Ysrai/ZB-DL01.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Ysrai/ZB-DL01.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Ysrai/ZB-SW02.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Ysrai/ZB-SW02.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Zehnder/TAFFETAS2 D1.00P1.01Z1.00.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Zehnder/TAFFETAS2 D1.00P1.01Z1.00.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/Certified/Zemismart/LXN56-DC27LX1.1.json` & `z4d-certified-devices-2.57/z4d_certified_devices/Certified/Zemismart/LXN56-DC27LX1.1.json`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices/__init__.py` & `z4d-certified-devices-2.57/z4d_certified_devices/__init__.py`

 * *Files identical despite different names*

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices.egg-info/PKG-INFO` & `z4d-certified-devices-2.57/z4d_certified_devices.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z4d-certified-devices
-Version: 2.56
+Version: 2.57
 Summary: "Certified devices for Zigbee for Domoticz plugin"
 Home-page: https://github.com/zigbeefordomoticz/z4d-certified-devices
 Author: "Patrick Pichon"
 Author-email: "patrick@pichon.me"
 License: "GPL-3.0"
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `z4d-certified-devices-2.56/z4d_certified_devices.egg-info/SOURCES.txt` & `z4d-certified-devices-2.57/z4d_certified_devices.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -404,14 +404,15 @@
 z4d_certified_devices/Certified/Tuya/TS0203.json
 z4d_certified_devices/Certified/Tuya/TS0205.json
 z4d_certified_devices/Certified/Tuya/TS0207-extender.json
 z4d_certified_devices/Certified/Tuya/TS0207-waterleak.json
 z4d_certified_devices/Certified/Tuya/TS0211.json
 z4d_certified_devices/Certified/Tuya/TS0215A-secure-remote.json
 z4d_certified_devices/Certified/Tuya/TS0215A-sos.json
+z4d_certified_devices/Certified/Tuya/TS0219.json
 z4d_certified_devices/Certified/Tuya/TS0222.json
 z4d_certified_devices/Certified/Tuya/TS0302.json
 z4d_certified_devices/Certified/Tuya/TS0502A.json
 z4d_certified_devices/Certified/Tuya/TS0505A.json
 z4d_certified_devices/Certified/Tuya/TS0505B.json
 z4d_certified_devices/Certified/Tuya/TS0601-2Gangs-dimmer.json
 z4d_certified_devices/Certified/Tuya/TS0601-2Gangs-switch.json
```

