# Comparing `tmp/pymatgen-4.7.6.tar.gz` & `tmp/pymatgen-4.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymatgen-4.7.6.tar", last modified: Sun May 14 16:35:25 2017, max compression
+gzip compressed data, was "dist/pymatgen-4.7.7.tar", last modified: Sat May 27 14:41:40 2017, max compression
```

## Comparing `pymatgen-4.7.6.tar` & `pymatgen-4.7.7.tar`

### file list

```diff
@@ -1,397 +1,398 @@
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/
--rw-r--r--   0 shyue      (501) staff       (20)    40248 2017-05-14 16:33:16.000000 pymatgen-4.7.6/CHANGES.rst
--rw-r--r--   0 shyue      (501) staff       (20)     1082 2016-09-25 20:11:02.000000 pymatgen-4.7.6/LICENSE.rst
--rw-r--r--   0 shyue      (501) staff       (20)      219 2016-09-25 20:11:02.000000 pymatgen-4.7.6/MANIFEST.in
--rw-r--r--   0 shyue      (501) staff       (20)    10890 2017-05-14 16:35:25.000000 pymatgen-4.7.6/PKG-INFO
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/
--rw-r--r--   0 shyue      (501) staff       (20)     2418 2017-05-14 16:35:20.000000 pymatgen-4.7.6/pymatgen/__init__.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/alchemy/
--rw-r--r--   0 shyue      (501) staff       (20)      228 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/alchemy/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    11447 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/alchemy/filters.py
--rw-r--r--   0 shyue      (501) staff       (20)    14267 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/alchemy/materials.py
--rw-r--r--   0 shyue      (501) staff       (20)    16735 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/alchemy/transmuters.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/analysis/
--rw-r--r--   0 shyue      (501) staff       (20)      217 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    25361 2017-03-07 21:24:46.000000 pymatgen-4.7.6/pymatgen/analysis/adsorption.py
--rw-r--r--   0 shyue      (501) staff       (20)    21703 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/bond_valence.py
--rw-r--r--   0 shyue      (501) staff       (20)     1240 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/analysis/bonds_jmol_ob.yaml
--rw-r--r--   0 shyue      (501) staff       (20)     1770 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/bvparam_1991.yaml
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/
--rw-r--r--   0 shyue      (501) staff       (20)       26 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/__init__.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/
--rw-r--r--   0 shyue      (501) staff       (20)       26 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    84066 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/chemenv_strategies.py
--rw-r--r--   0 shyue      (501) staff       (20)    51388 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/
--rw-r--r--   0 shyue      (501) staff       (20)       26 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)      511 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/A#2.json
--rw-r--r--   0 shyue      (501) staff       (20)     4980 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/AC#12.json
--rw-r--r--   0 shyue      (501) staff       (20)     2682 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/allcg.txt
--rw-r--r--   0 shyue      (501) staff       (20)     3653 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/BO_1#8.json
--rw-r--r--   0 shyue      (501) staff       (20)     5530 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/BO_2#8.json
--rw-r--r--   0 shyue      (501) staff       (20)     4909 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/BO_3#8.json
--rw-r--r--   0 shyue      (501) staff       (20)     3124 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/BS_1#10.json
--rw-r--r--   0 shyue      (501) staff       (20)    10526 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/BS_2#10.json
--rw-r--r--   0 shyue      (501) staff       (20)     7863 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/C#12.json
--rw-r--r--   0 shyue      (501) staff       (20)     2865 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/C#8.json
--rw-r--r--   0 shyue      (501) staff       (20)      258 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/CO#11.json
--rw-r--r--   0 shyue      (501) staff       (20)      260 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/DD#20.json
--rw-r--r--   0 shyue      (501) staff       (20)     2310 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/DD#8.json
--rw-r--r--   0 shyue      (501) staff       (20)     2378 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/DDPN#8.json
--rw-r--r--   0 shyue      (501) staff       (20)     9900 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/DI#11.json
--rw-r--r--   0 shyue      (501) staff       (20)     3406 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/ET#7.json
--rw-r--r--   0 shyue      (501) staff       (20)     2521 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/FO#7.json
--rw-r--r--   0 shyue      (501) staff       (20)      262 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/H#10.json
--rw-r--r--   0 shyue      (501) staff       (20)     8230 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/H#11.json
--rw-r--r--   0 shyue      (501) staff       (20)     2631 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/HA#12.json
--rw-r--r--   0 shyue      (501) staff       (20)     2999 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/HB#8.json
--rw-r--r--   0 shyue      (501) staff       (20)     1640 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/HD#9.json
--rw-r--r--   0 shyue      (501) staff       (20)     8053 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/HP#12.json
--rw-r--r--   0 shyue      (501) staff       (20)     7469 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/I#12.json
--rw-r--r--   0 shyue      (501) staff       (20)      495 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/L#2.json
--rw-r--r--   0 shyue      (501) staff       (20)     7956 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/MI#10.json
--rw-r--r--   0 shyue      (501) staff       (20)     2916 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/O#6.json
--rw-r--r--   0 shyue      (501) staff       (20)     1204 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/O#6_explicit.json
--rw-r--r--   0 shyue      (501) staff       (20)     7566 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PA#10.json
--rw-r--r--   0 shyue      (501) staff       (20)     2564 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PB#7.json
--rw-r--r--   0 shyue      (501) staff       (20)    12676 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PBP#12.json
--rw-r--r--   0 shyue      (501) staff       (20)    17243 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PCPA#11.json
--rw-r--r--   0 shyue      (501) staff       (20)     3743 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PP#10.json
--rw-r--r--   0 shyue      (501) staff       (20)      999 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PP#5.json
--rw-r--r--   0 shyue      (501) staff       (20)     2353 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PP#6.json
--rw-r--r--   0 shyue      (501) staff       (20)      464 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/S#1.json
--rw-r--r--   0 shyue      (501) staff       (20)      256 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/S#10.json
--rw-r--r--   0 shyue      (501) staff       (20)      260 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/S#12.json
--rw-r--r--   0 shyue      (501) staff       (20)      647 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/S#4.json
--rw-r--r--   0 shyue      (501) staff       (20)      979 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/S#5.json
--rw-r--r--   0 shyue      (501) staff       (20)     3215 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SA#8.json
--rw-r--r--   0 shyue      (501) staff       (20)    12423 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SBSA#10.json
--rw-r--r--   0 shyue      (501) staff       (20)     3574 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SBT#8.json
--rw-r--r--   0 shyue      (501) staff       (20)     2612 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SC#12.json
--rw-r--r--   0 shyue      (501) staff       (20)      970 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SH#11.json
--rw-r--r--   0 shyue      (501) staff       (20)     6312 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SH#13.json
--rw-r--r--   0 shyue      (501) staff       (20)     9708 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SMA#9.json
--rw-r--r--   0 shyue      (501) staff       (20)      708 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SS#4.json
--rw-r--r--   0 shyue      (501) staff       (20)     5992 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SS#9.json
--rw-r--r--   0 shyue      (501) staff       (20)     2829 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/ST#7.json
--rw-r--r--   0 shyue      (501) staff       (20)      780 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SY#4.json
--rw-r--r--   0 shyue      (501) staff       (20)      887 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/T#4.json
--rw-r--r--   0 shyue      (501) staff       (20)      991 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/T#5.json
--rw-r--r--   0 shyue      (501) staff       (20)     2374 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/T#6.json
--rw-r--r--   0 shyue      (501) staff       (20)     8161 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TBSA#10.json
--rw-r--r--   0 shyue      (501) staff       (20)     2008 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TBT#8.json
--rw-r--r--   0 shyue      (501) staff       (20)     6515 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TC#9.json
--rw-r--r--   0 shyue      (501) staff       (20)     4868 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TI#9.json
--rw-r--r--   0 shyue      (501) staff       (20)      625 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TL#3.json
--rw-r--r--   0 shyue      (501) staff       (20)    14523 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TO_1#9.json
--rw-r--r--   0 shyue      (501) staff       (20)     8184 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TO_2#9.json
--rw-r--r--   0 shyue      (501) staff       (20)    10703 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TO_3#9.json
--rw-r--r--   0 shyue      (501) staff       (20)      583 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TS#3.json
--rw-r--r--   0 shyue      (501) staff       (20)     7895 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TT#12.json
--rw-r--r--   0 shyue      (501) staff       (20)     7757 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TT_1#9.json
--rw-r--r--   0 shyue      (501) staff       (20)    12608 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TT_2#9.json
--rw-r--r--   0 shyue      (501) staff       (20)     5258 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TT_3#9.json
--rw-r--r--   0 shyue      (501) staff       (20)      724 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TY#3.json
--rw-r--r--   0 shyue      (501) staff       (20)    75875 2016-10-19 06:56:38.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometry_finder.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/strategy_files/
--rw-r--r--   0 shyue      (501) staff       (20)       26 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/strategy_files/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)      844 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/strategy_files/ImprovedConfidenceCutoffDefaultParameters.json
--rw-r--r--   0 shyue      (501) staff       (20)    79050 2017-01-03 01:28:02.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/structure_environments.py
--rw-r--r--   0 shyue      (501) staff       (20)    36849 2016-12-03 05:41:54.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/voronoi.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/utils/
--rw-r--r--   0 shyue      (501) staff       (20)       26 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/utils/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     8193 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/utils/chemenv_config.py
--rw-r--r--   0 shyue      (501) staff       (20)     3780 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/utils/chemenv_errors.py
--rw-r--r--   0 shyue      (501) staff       (20)    34349 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/utils/coordination_geometry_utils.py
--rw-r--r--   0 shyue      (501) staff       (20)     3527 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/utils/defs_utils.py
--rw-r--r--   0 shyue      (501) staff       (20)     7225 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/utils/func_utils.py
--rw-r--r--   0 shyue      (501) staff       (20)     9465 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/utils/math_utils.py
--rw-r--r--   0 shyue      (501) staff       (20)    15858 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/chemenv/utils/scripts_utils.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/analysis/cost/
--rw-r--r--   0 shyue      (501) staff       (20)      299 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/cost/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     6048 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/cost/cost.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/analysis/defects/
--rw-r--r--   0 shyue      (501) staff       (20)      203 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/defects/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    53295 2017-04-01 23:01:31.000000 pymatgen-4.7.6/pymatgen/analysis/defects/dilute_solution_model.py
--rw-r--r--   0 shyue      (501) staff       (20)     7631 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/defects/ionic_radii.json
--rw-r--r--   0 shyue      (501) staff       (20)    72613 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/analysis/defects/point_defects.py
--rw-r--r--   0 shyue      (501) staff       (20)     1510 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/defects/surf_error.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/analysis/diffraction/
--rw-r--r--   0 shyue      (501) staff       (20)      439 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/diffraction/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     6760 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/diffraction/atomic_scattering_params.json
--rw-r--r--   0 shyue      (501) staff       (20)    14977 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/analysis/diffraction/xrd.py
--rw-r--r--   0 shyue      (501) staff       (20)    35366 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/analysis/diffusion_analyzer.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/analysis/elasticity/
--rw-r--r--   0 shyue      (501) staff       (20)      220 2017-02-02 21:53:25.000000 pymatgen-4.7.6/pymatgen/analysis/elasticity/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    26939 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/analysis/elasticity/elastic.py
--rw-r--r--   0 shyue      (501) staff       (20)    10794 2017-05-11 02:29:31.000000 pymatgen-4.7.6/pymatgen/analysis/elasticity/strain.py
--rw-r--r--   0 shyue      (501) staff       (20)     3571 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/analysis/elasticity/stress.py
--rw-r--r--   0 shyue      (501) staff       (20)    19491 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/analysis/elasticity/tensors.py
--rw-r--r--   0 shyue      (501) staff       (20)     5624 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/energy_models.py
--rw-r--r--   0 shyue      (501) staff       (20)    17394 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/analysis/eos.py
--rw-r--r--   0 shyue      (501) staff       (20)    24382 2017-05-12 04:20:30.000000 pymatgen-4.7.6/pymatgen/analysis/ewald.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/analysis/ferroelectricity/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2017-04-19 12:25:30.000000 pymatgen-4.7.6/pymatgen/analysis/ferroelectricity/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    15811 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/analysis/ferroelectricity/polarization.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/analysis/hhi/
--rw-r--r--   0 shyue      (501) staff       (20)      131 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/hhi/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     3806 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/hhi/hhi.py
--rw-r--r--   0 shyue      (501) staff       (20)    34095 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/icsd_bv.yaml
--rw-r--r--   0 shyue      (501) staff       (20)    25092 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/analysis/molecule_matcher.py
--rw-r--r--   0 shyue      (501) staff       (20)     7931 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/molecule_structure_comparator.py
--rw-r--r--   0 shyue      (501) staff       (20)     4047 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/nmr.py
--rw-r--r--   0 shyue      (501) staff       (20)    18284 2017-03-24 21:58:11.000000 pymatgen-4.7.6/pymatgen/analysis/path_finder.py
--rw-r--r--   0 shyue      (501) staff       (20)     1682 2017-04-01 23:01:31.000000 pymatgen-4.7.6/pymatgen/analysis/piezo.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/analysis/pourbaix/
--rw-r--r--   0 shyue      (501) staff       (20)      108 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/pourbaix/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     9840 2016-12-03 05:41:54.000000 pymatgen-4.7.6/pymatgen/analysis/pourbaix/analyzer.py
--rw-r--r--   0 shyue      (501) staff       (20)    14039 2017-04-01 23:01:31.000000 pymatgen-4.7.6/pymatgen/analysis/pourbaix/entry.py
--rw-r--r--   0 shyue      (501) staff       (20)    17124 2017-04-01 23:01:31.000000 pymatgen-4.7.6/pymatgen/analysis/pourbaix/maker.py
--rw-r--r--   0 shyue      (501) staff       (20)    34827 2017-03-07 21:24:46.000000 pymatgen-4.7.6/pymatgen/analysis/pourbaix/plotter.py
--rw-r--r--   0 shyue      (501) staff       (20)    12109 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/analysis/quasiharmonic.py
--rw-r--r--   0 shyue      (501) staff       (20)    16693 2017-03-07 21:24:46.000000 pymatgen-4.7.6/pymatgen/analysis/reaction_calculator.py
--rw-r--r--   0 shyue      (501) staff       (20)    82945 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/analysis/structure_analyzer.py
--rw-r--r--   0 shyue      (501) staff       (20)    42586 2017-01-16 16:23:39.000000 pymatgen-4.7.6/pymatgen/analysis/structure_matcher.py
--rw-r--r--   0 shyue      (501) staff       (20)    18671 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/substrate_analyzer.py
--rw-r--r--   0 shyue      (501) staff       (20)     3335 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/analysis/thermochemistry.py
--rw-r--r--   0 shyue      (501) staff       (20)    12402 2017-03-07 21:24:46.000000 pymatgen-4.7.6/pymatgen/analysis/transition_state.py
--rw-r--r--   0 shyue      (501) staff       (20)    20227 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/analysis/wulff.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/apps/
--rw-r--r--   0 shyue      (501) staff       (20)      210 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/apps/__init__.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/apps/battery/
--rw-r--r--   0 shyue      (501) staff       (20)      256 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/apps/battery/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     8873 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/apps/battery/analyzer.py
--rw-r--r--   0 shyue      (501) staff       (20)    12215 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/apps/battery/battery_abc.py
--rw-r--r--   0 shyue      (501) staff       (20)    20877 2017-01-16 16:23:39.000000 pymatgen-4.7.6/pymatgen/apps/battery/conversion_battery.py
--rw-r--r--   0 shyue      (501) staff       (20)    20634 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/apps/battery/insertion_battery.py
--rw-r--r--   0 shyue      (501) staff       (20)     3443 2017-03-07 21:24:46.000000 pymatgen-4.7.6/pymatgen/apps/battery/plotter.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/apps/borg/
--rw-r--r--   0 shyue      (501) staff       (20)      229 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/apps/borg/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    17218 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/apps/borg/hive.py
--rw-r--r--   0 shyue      (501) staff       (20)     4998 2017-02-02 21:53:25.000000 pymatgen-4.7.6/pymatgen/apps/borg/queen.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/cli/
--rw-r--r--   0 shyue      (501) staff       (20)      289 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/cli/__init__.py
--rwxr-xr-x   0 shyue      (501) staff       (20)     2148 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/cli/feff_input_generation.py
--rwxr-xr-x   0 shyue      (501) staff       (20)     1996 2017-03-07 21:24:46.000000 pymatgen-4.7.6/pymatgen/cli/feff_plot_cross_section.py
--rwxr-xr-x   0 shyue      (501) staff       (20)     2193 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/cli/feff_plot_dos.py
--rwxr-xr-x   0 shyue      (501) staff       (20)     3347 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/cli/gaussian_analyzer.py
--rw-r--r--   0 shyue      (501) staff       (20)     1341 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/cli/get_environment.py
--rwxr-xr-x   0 shyue      (501) staff       (20)    14089 2017-01-16 16:23:39.000000 pymatgen-4.7.6/pymatgen/cli/pmg.py
--rwxr-xr-x   0 shyue      (501) staff       (20)     4753 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/cli/pmg_analyze.py
--rwxr-xr-x   0 shyue      (501) staff       (20)     6791 2017-01-03 01:28:02.000000 pymatgen-4.7.6/pymatgen/cli/pmg_config.py
--rwxr-xr-x   0 shyue      (501) staff       (20)     2497 2017-03-07 21:24:46.000000 pymatgen-4.7.6/pymatgen/cli/pmg_plot.py
--rwxr-xr-x   0 shyue      (501) staff       (20)     1147 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/cli/pmg_potcar.py
--rw-r--r--   0 shyue      (501) staff       (20)     1907 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/cli/pmg_query.py
--rwxr-xr-x   0 shyue      (501) staff       (20)     3397 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/cli/pmg_structure.py
--rwxr-xr-x   0 shyue      (501) staff       (20)    23839 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/cli/pydii.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/command_line/
--rw-r--r--   0 shyue      (501) staff       (20)      277 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/command_line/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     3605 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/command_line/aconvasp_caller.py
--rw-r--r--   0 shyue      (501) staff       (20)     6078 2017-01-03 01:28:02.000000 pymatgen-4.7.6/pymatgen/command_line/bader_caller.py
--rw-r--r--   0 shyue      (501) staff       (20)    15800 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/command_line/enumlib_caller.py
--rw-r--r--   0 shyue      (501) staff       (20)    26892 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/command_line/gulp_caller.py
--rw-r--r--   0 shyue      (501) staff       (20)     5726 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/command_line/OxideTersoffPotentials
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/core/
--rw-r--r--   0 shyue      (501) staff       (20)      640 2016-11-16 04:40:15.000000 pymatgen-4.7.6/pymatgen/core/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     3408 2017-04-19 12:25:30.000000 pymatgen-4.7.6/pymatgen/core/bond_lengths.json
--rw-r--r--   0 shyue      (501) staff       (20)     3875 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/core/bonds.py
--rw-r--r--   0 shyue      (501) staff       (20)    31944 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/core/composition.py
--rw-r--r--   0 shyue      (501) staff       (20)     2822 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/core/func_groups.json
--rw-r--r--   0 shyue      (501) staff       (20)     7310 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/core/ion.py
--rw-r--r--   0 shyue      (501) staff       (20)    42044 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/core/lattice.py
--rw-r--r--   0 shyue      (501) staff       (20)    58185 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/core/libxc_docs.json
--rw-r--r--   0 shyue      (501) staff       (20)    13121 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/core/libxcfunc.py
--rw-r--r--   0 shyue      (501) staff       (20)    21597 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/core/operations.py
--rw-r--r--   0 shyue      (501) staff       (20)   120293 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/core/periodic_table.json
--rw-r--r--   0 shyue      (501) staff       (20)    37149 2017-03-07 21:24:46.000000 pymatgen-4.7.6/pymatgen/core/periodic_table.py
--rw-r--r--   0 shyue      (501) staff       (20)     1935 2016-12-16 05:48:52.000000 pymatgen-4.7.6/pymatgen/core/physical_constants.py
--rw-r--r--   0 shyue      (501) staff       (20)    18993 2017-03-07 21:24:46.000000 pymatgen-4.7.6/pymatgen/core/sites.py
--rw-r--r--   0 shyue      (501) staff       (20)   124072 2017-05-13 01:33:30.000000 pymatgen-4.7.6/pymatgen/core/structure.py
--rw-r--r--   0 shyue      (501) staff       (20)    44320 2017-03-07 21:24:46.000000 pymatgen-4.7.6/pymatgen/core/surface.py
--rw-r--r--   0 shyue      (501) staff       (20)    27827 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/core/units.py
--rw-r--r--   0 shyue      (501) staff       (20)    10353 2017-03-24 21:58:11.000000 pymatgen-4.7.6/pymatgen/core/xcfunc.py
--rw-r--r--   0 shyue      (501) staff       (20)      695 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/dao.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/electronic_structure/
--rw-r--r--   0 shyue      (501) staff       (20)      189 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/electronic_structure/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    39691 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/electronic_structure/bandstructure.py
--rw-r--r--   0 shyue      (501) staff       (20)    94779 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/electronic_structure/boltztrap.py
--rw-r--r--   0 shyue      (501) staff       (20)    15416 2017-04-19 12:25:30.000000 pymatgen-4.7.6/pymatgen/electronic_structure/core.py
--rw-r--r--   0 shyue      (501) staff       (20)    17289 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/electronic_structure/dos.py
--rw-r--r--   0 shyue      (501) staff       (20)   139126 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/electronic_structure/plotter.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/entries/
--rw-r--r--   0 shyue      (501) staff       (20)      297 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/entries/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    24628 2017-04-06 03:57:47.000000 pymatgen-4.7.6/pymatgen/entries/compatibility.py
--rw-r--r--   0 shyue      (501) staff       (20)     7315 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/entries/computed_entries.py
--rw-r--r--   0 shyue      (501) staff       (20)     5906 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/entries/entry_tools.py
--rw-r--r--   0 shyue      (501) staff       (20)     2795 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/entries/exp_entries.py
--rw-r--r--   0 shyue      (501) staff       (20)     2174 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/entries/MITCompatibility.yaml
--rw-r--r--   0 shyue      (501) staff       (20)     2604 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/entries/MPCompatibility.yaml
--rw-r--r--   0 shyue      (501) staff       (20)     1459 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/entries/post_processors_abc.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/io/
--rw-r--r--   0 shyue      (501) staff       (20)      233 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/__init__.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/io/abinit/
--rw-r--r--   0 shyue      (501) staff       (20)      226 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/abinit/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    19214 2017-03-24 21:58:11.000000 pymatgen-4.7.6/pymatgen/io/abinit/abiinspect.py
--rw-r--r--   0 shyue      (501) staff       (20)    49706 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/io/abinit/abiobjects.py
--rw-r--r--   0 shyue      (501) staff       (20)    29828 2017-04-19 12:25:30.000000 pymatgen-4.7.6/pymatgen/io/abinit/abitimer.py
--rw-r--r--   0 shyue      (501) staff       (20)    17803 2017-03-24 21:58:11.000000 pymatgen-4.7.6/pymatgen/io/abinit/calculations.py
--rw-r--r--   0 shyue      (501) staff       (20)     4991 2017-03-07 21:24:46.000000 pymatgen-4.7.6/pymatgen/io/abinit/db.py
--rw-r--r--   0 shyue      (501) staff       (20)    28225 2016-11-02 22:55:22.000000 pymatgen-4.7.6/pymatgen/io/abinit/events.py
--rw-r--r--   0 shyue      (501) staff       (20)   106450 2017-04-19 12:25:30.000000 pymatgen-4.7.6/pymatgen/io/abinit/flows.py
--rw-r--r--   0 shyue      (501) staff       (20)     7018 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/abinit/helpers.py
--rw-r--r--   0 shyue      (501) staff       (20)    47837 2017-03-24 21:58:11.000000 pymatgen-4.7.6/pymatgen/io/abinit/launcher.py
--rw-r--r--   0 shyue      (501) staff       (20)    10393 2017-03-24 21:58:11.000000 pymatgen-4.7.6/pymatgen/io/abinit/netcdf.py
--rw-r--r--   0 shyue      (501) staff       (20)    38373 2017-03-24 21:58:11.000000 pymatgen-4.7.6/pymatgen/io/abinit/nodes.py
--rw-r--r--   0 shyue      (501) staff       (20)    63356 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/io/abinit/pseudos.py
--rw-r--r--   0 shyue      (501) staff       (20)    79542 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/io/abinit/qadapters.py
--rw-r--r--   0 shyue      (501) staff       (20)    17260 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/abinit/qjobs.py
--rw-r--r--   0 shyue      (501) staff       (20)     3763 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/abinit/qutils.py
--rw-r--r--   0 shyue      (501) staff       (20)     3632 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/abinit/scheduler_error_handlers.py
--rw-r--r--   0 shyue      (501) staff       (20)    14014 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/abinit/scheduler_error_parsers.py
--rw-r--r--   0 shyue      (501) staff       (20)   171911 2017-03-24 21:58:11.000000 pymatgen-4.7.6/pymatgen/io/abinit/tasks.py
--rw-r--r--   0 shyue      (501) staff       (20)    27984 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/io/abinit/utils.py
--rw-r--r--   0 shyue      (501) staff       (20)    56476 2017-03-24 21:58:11.000000 pymatgen-4.7.6/pymatgen/io/abinit/works.py
--rw-r--r--   0 shyue      (501) staff       (20)    12127 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/abinit/wrappers.py
--rw-r--r--   0 shyue      (501) staff       (20)    31523 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/io/adf.py
--rw-r--r--   0 shyue      (501) staff       (20)     2129 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/aiida.py
--rw-r--r--   0 shyue      (501) staff       (20)     1985 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/ase.py
--rw-r--r--   0 shyue      (501) staff       (20)     4995 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/babel.py
--rw-r--r--   0 shyue      (501) staff       (20)    35160 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/io/cif.py
--rw-r--r--   0 shyue      (501) staff       (20)     3039 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/io/cssr.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/io/exciting/
--rw-r--r--   0 shyue      (501) staff       (20)      267 2017-03-07 21:24:46.000000 pymatgen-4.7.6/pymatgen/io/exciting/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    11846 2017-03-07 21:24:46.000000 pymatgen-4.7.6/pymatgen/io/exciting/inputs.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/io/feff/
--rw-r--r--   0 shyue      (501) staff       (20)      311 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/feff/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    32326 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/io/feff/inputs.py
--rw-r--r--   0 shyue      (501) staff       (20)      405 2016-10-19 06:56:38.000000 pymatgen-4.7.6/pymatgen/io/feff/MPELNESSet.yaml
--rw-r--r--   0 shyue      (501) staff       (20)      112 2017-03-07 21:24:46.000000 pymatgen-4.7.6/pymatgen/io/feff/MPEXAFSSet.yaml
--rw-r--r--   0 shyue      (501) staff       (20)      362 2016-10-19 06:56:38.000000 pymatgen-4.7.6/pymatgen/io/feff/MPEXELFSSet.yaml
--rw-r--r--   0 shyue      (501) staff       (20)      161 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/feff/MPXANESSet.yaml
--rw-r--r--   0 shyue      (501) staff       (20)    12025 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/io/feff/outputs.py
--rw-r--r--   0 shyue      (501) staff       (20)    16295 2017-03-07 21:24:46.000000 pymatgen-4.7.6/pymatgen/io/feff/sets.py
--rw-r--r--   0 shyue      (501) staff       (20)    28823 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/io/fiesta.py
--rw-r--r--   0 shyue      (501) staff       (20)    53491 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/io/gaussian.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/io/lammps/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/lammps/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    33053 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/io/lammps/data.py
--rw-r--r--   0 shyue      (501) staff       (20)     3235 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/lammps/force_field.py
--rw-r--r--   0 shyue      (501) staff       (20)     6304 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/lammps/input.py
--rw-r--r--   0 shyue      (501) staff       (20)     1141 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/lammps/NPT.json
--rw-r--r--   0 shyue      (501) staff       (20)     1244 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/lammps/NPT_NVT.json
--rw-r--r--   0 shyue      (501) staff       (20)      908 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/lammps/NVT.json
--rw-r--r--   0 shyue      (501) staff       (20)    16467 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/io/lammps/output.py
--rw-r--r--   0 shyue      (501) staff       (20)     5153 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/lammps/topology.py
--rw-r--r--   0 shyue      (501) staff       (20)    15202 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/lammps/utils.py
--rw-r--r--   0 shyue      (501) staff       (20)    32329 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/io/nwchem.py
--rw-r--r--   0 shyue      (501) staff       (20)     6155 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/io/phonopy.py
--rw-r--r--   0 shyue      (501) staff       (20)     7300 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/io/pwscf.py
--rw-r--r--   0 shyue      (501) staff       (20)    87307 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/io/qchem.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/io/vasp/
--rw-r--r--   0 shyue      (501) staff       (20)      456 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/vasp/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     1456 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/vasp/GWVaspInputSet.yaml
--rw-r--r--   0 shyue      (501) staff       (20)    26739 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/vasp/GWvaspinputsets.py
--rw-r--r--   0 shyue      (501) staff       (20)    71956 2017-05-12 04:29:06.000000 pymatgen-4.7.6/pymatgen/io/vasp/inputs.py
--rw-r--r--   0 shyue      (501) staff       (20)     7374 2017-04-01 23:01:31.000000 pymatgen-4.7.6/pymatgen/io/vasp/MITRelaxSet.yaml
--rw-r--r--   0 shyue      (501) staff       (20)     1331 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/vasp/MPHSERelaxSet.yaml
--rw-r--r--   0 shyue      (501) staff       (20)     2023 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/vasp/MPRelaxSet.yaml
--rw-r--r--   0 shyue      (501) staff       (20)   137250 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/io/vasp/outputs.py
--rw-r--r--   0 shyue      (501) staff       (20)    58726 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/io/vasp/sets.py
--rw-r--r--   0 shyue      (501) staff       (20)     3382 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/io/xcrysden.py
--rw-r--r--   0 shyue      (501) staff       (20)     6272 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/io/xr.py
--rw-r--r--   0 shyue      (501) staff       (20)     3960 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/io/xyz.py
--rw-r--r--   0 shyue      (501) staff       (20)    18986 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/io/zeopp.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/matproj/
--rw-r--r--   0 shyue      (501) staff       (20)      196 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/matproj/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    39592 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/matproj/rest.py
--rw-r--r--   0 shyue      (501) staff       (20)    13495 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/matproj/snl.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/optimization/
--rw-r--r--   0 shyue      (501) staff       (20)      109 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/optimization/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)   901516 2016-10-23 04:19:30.000000 pymatgen-4.7.6/pymatgen/optimization/linear_assignment.c
--rw-r--r--   0 shyue      (501) staff       (20)     8016 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/optimization/linear_assignment.pyx
--rw-r--r--   0 shyue      (501) staff       (20)     8228 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/optimization/linear_assignment_numpy.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/phasediagram/
--rw-r--r--   0 shyue      (501) staff       (20)      410 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/phasediagram/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    19907 2017-04-01 23:01:31.000000 pymatgen-4.7.6/pymatgen/phasediagram/analyzer.py
--rw-r--r--   0 shyue      (501) staff       (20)     9519 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/phasediagram/entries.py
--rw-r--r--   0 shyue      (501) staff       (20)    18276 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/phasediagram/maker.py
--rw-r--r--   0 shyue      (501) staff       (20)    30521 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/phasediagram/plotter.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/phonon/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2017-02-02 21:53:25.000000 pymatgen-4.7.6/pymatgen/phonon/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    18026 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/phonon/bandstructure.py
--rw-r--r--   0 shyue      (501) staff       (20)     5900 2017-02-02 21:53:25.000000 pymatgen-4.7.6/pymatgen/phonon/dos.py
--rw-r--r--   0 shyue      (501) staff       (20)    15693 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/phonon/plotter.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/serializers/
--rw-r--r--   0 shyue      (501) staff       (20)      211 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/serializers/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     1194 2017-03-24 21:58:11.000000 pymatgen-4.7.6/pymatgen/serializers/json_coders.py
--rw-r--r--   0 shyue      (501) staff       (20)     3272 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/serializers/pickle_coders.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/structure_prediction/
--rw-r--r--   0 shyue      (501) staff       (20)      108 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/structure_prediction/__init__.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/structure_prediction/data/
--rw-r--r--   0 shyue      (501) staff       (20)   184884 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/structure_prediction/data/lambda.json
--rw-r--r--   0 shyue      (501) staff       (20)   256410 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/structure_prediction/data/pair_correlation.json
--rw-r--r--   0 shyue      (501) staff       (20)     8996 2017-04-19 12:25:30.000000 pymatgen-4.7.6/pymatgen/structure_prediction/substitution_probability.py
--rw-r--r--   0 shyue      (501) staff       (20)    10618 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/structure_prediction/substitutor.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/symmetry/
--rw-r--r--   0 shyue      (501) staff       (20)      203 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/symmetry/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    54060 2017-05-14 16:30:09.000000 pymatgen-4.7.6/pymatgen/symmetry/analyzer.py
--rw-r--r--   0 shyue      (501) staff       (20)    29835 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/symmetry/bandstructure.py
--rw-r--r--   0 shyue      (501) staff       (20)    18471 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/symmetry/groups.py
--rw-r--r--   0 shyue      (501) staff       (20)     2849 2017-04-01 23:01:31.000000 pymatgen-4.7.6/pymatgen/symmetry/structure.py
--rw-r--r--   0 shyue      (501) staff       (20)    48218 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/symmetry/symm_data.yaml
--rw-r--r--   0 shyue      (501) staff       (20)   422366 2016-10-19 06:56:38.000000 pymatgen-4.7.6/pymatgen/symmetry/symm_ops.json
--rw-r--r--   0 shyue      (501) staff       (20)   443429 2016-10-19 06:56:38.000000 pymatgen-4.7.6/pymatgen/symmetry/symm_ops.yaml
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/transformations/
--rw-r--r--   0 shyue      (501) staff       (20)      256 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/transformations/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    33684 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/transformations/advanced_transformations.py
--rw-r--r--   0 shyue      (501) staff       (20)    11269 2017-04-01 23:01:31.000000 pymatgen-4.7.6/pymatgen/transformations/defect_transformations.py
--rw-r--r--   0 shyue      (501) staff       (20)    20998 2017-02-02 21:53:25.000000 pymatgen-4.7.6/pymatgen/transformations/site_transformations.py
--rw-r--r--   0 shyue      (501) staff       (20)    23008 2017-01-16 16:23:39.000000 pymatgen-4.7.6/pymatgen/transformations/standard_transformations.py
--rw-r--r--   0 shyue      (501) staff       (20)     2734 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/transformations/transformation_abc.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/util/
--rw-r--r--   0 shyue      (501) staff       (20)      309 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/util/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    14863 2017-03-24 21:58:11.000000 pymatgen-4.7.6/pymatgen/util/convergence.py
--rw-r--r--   0 shyue      (501) staff       (20)    15753 2017-04-19 12:25:30.000000 pymatgen-4.7.6/pymatgen/util/coord_utils.py
--rw-r--r--   0 shyue      (501) staff       (20)   992710 2016-12-03 05:41:54.000000 pymatgen-4.7.6/pymatgen/util/coord_utils_cython.c
--rw-r--r--   0 shyue      (501) staff       (20)     8664 2016-12-03 05:41:54.000000 pymatgen-4.7.6/pymatgen/util/coord_utils_cython.pyx
--rw-r--r--   0 shyue      (501) staff       (20)     6016 2017-03-24 21:58:11.000000 pymatgen-4.7.6/pymatgen/util/io_utils.py
--rw-r--r--   0 shyue      (501) staff       (20)     3740 2017-03-07 21:24:46.000000 pymatgen-4.7.6/pymatgen/util/num.py
--rw-r--r--   0 shyue      (501) staff       (20)      181 2017-03-07 21:24:46.000000 pymatgen-4.7.6/pymatgen/util/num_utils.py
--rw-r--r--   0 shyue      (501) staff       (20)    10567 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/util/plotting.py
--rw-r--r--   0 shyue      (501) staff       (20)      196 2017-03-07 21:24:46.000000 pymatgen-4.7.6/pymatgen/util/plotting_utils.py
--rw-r--r--   0 shyue      (501) staff       (20)     3733 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/util/string.py
--rw-r--r--   0 shyue      (501) staff       (20)      190 2017-03-07 21:24:46.000000 pymatgen-4.7.6/pymatgen/util/string_utils.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/util/structures/
--rw-r--r--   0 shyue      (501) staff       (20)     2647 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/util/structures/BaNiO3.json
--rw-r--r--   0 shyue      (501) staff       (20)      524 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/util/structures/CsCl.json
--rw-r--r--   0 shyue      (501) staff       (20)     1183 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/util/structures/Graphite.json
--rw-r--r--   0 shyue      (501) staff       (20)     2239 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/util/structures/K2O2.json
--rw-r--r--   0 shyue      (501) staff       (20)    11142 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/util/structures/Li10GeP2S12.json
--rw-r--r--   0 shyue      (501) staff       (20)     1032 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/util/structures/Li2O.json
--rw-r--r--   0 shyue      (501) staff       (20)     2270 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/util/structures/Li2O2.json
--rw-r--r--   0 shyue      (501) staff       (20)    10384 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/util/structures/Li3V2(PO4)3.json
--rw-r--r--   0 shyue      (501) staff       (20)     6007 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/util/structures/LiFePO4.json
--rw-r--r--   0 shyue      (501) staff       (20)     5871 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/util/structures/NaFePO4.json
--rw-r--r--   0 shyue      (501) staff       (20)      660 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/util/structures/Si.json
--rw-r--r--   0 shyue      (501) staff       (20)     1446 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/util/structures/Sn.json
--rw-r--r--   0 shyue      (501) staff       (20)     1095 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/util/structures/SrTiO3.json
--rw-r--r--   0 shyue      (501) staff       (20)     1641 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/util/structures/TiO2.json
--rw-r--r--   0 shyue      (501) staff       (20)     1007 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/util/structures/VO2.json
--rw-r--r--   0 shyue      (501) staff       (20)     6039 2017-03-07 21:24:46.000000 pymatgen-4.7.6/pymatgen/util/testing.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen/vis/
--rw-r--r--   0 shyue      (501) staff       (20)      211 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/vis/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     4494 2016-09-25 20:11:03.000000 pymatgen-4.7.6/pymatgen/vis/ElementColorSchemes.yaml
--rw-r--r--   0 shyue      (501) staff       (20)     3231 2017-02-02 21:53:25.000000 pymatgen-4.7.6/pymatgen/vis/structure_chemview.py
--rw-r--r--   0 shyue      (501) staff       (20)    47019 2017-05-09 20:42:44.000000 pymatgen-4.7.6/pymatgen/vis/structure_vtk.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-14 16:35:25.000000 pymatgen-4.7.6/pymatgen.egg-info/
--rw-r--r--   0 shyue      (501) staff       (20)        1 2017-05-14 16:35:24.000000 pymatgen-4.7.6/pymatgen.egg-info/dependency_links.txt
--rw-r--r--   0 shyue      (501) staff       (20)      367 2017-05-14 16:35:24.000000 pymatgen-4.7.6/pymatgen.egg-info/entry_points.txt
--rw-r--r--   0 shyue      (501) staff       (20)    10890 2017-05-14 16:35:24.000000 pymatgen-4.7.6/pymatgen.egg-info/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)      345 2017-05-14 16:35:24.000000 pymatgen-4.7.6/pymatgen.egg-info/requires.txt
--rw-r--r--   0 shyue      (501) staff       (20)    16092 2017-05-14 16:35:24.000000 pymatgen-4.7.6/pymatgen.egg-info/SOURCES.txt
--rw-r--r--   0 shyue      (501) staff       (20)        9 2017-05-14 16:35:24.000000 pymatgen-4.7.6/pymatgen.egg-info/top_level.txt
--rw-r--r--   0 shyue      (501) staff       (20)     8265 2017-05-09 20:42:44.000000 pymatgen-4.7.6/README.rst
--rw-r--r--   0 shyue      (501) staff       (20)       95 2017-04-01 23:01:31.000000 pymatgen-4.7.6/requirements-optional.txt
--rw-r--r--   0 shyue      (501) staff       (20)      220 2017-05-12 04:20:30.000000 pymatgen-4.7.6/requirements.txt
--rw-r--r--   0 shyue      (501) staff       (20)      112 2017-05-14 16:35:25.000000 pymatgen-4.7.6/setup.cfg
--rw-r--r--   0 shyue      (501) staff       (20)     5473 2017-05-14 16:35:23.000000 pymatgen-4.7.6/setup.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:40.000000 pymatgen-4.7.7/
+-rw-r--r--   0 shyue      (501) staff       (20)    40367 2017-05-27 14:40:53.000000 pymatgen-4.7.7/CHANGES.rst
+-rw-r--r--   0 shyue      (501) staff       (20)     1082 2016-09-25 20:11:02.000000 pymatgen-4.7.7/LICENSE.rst
+-rw-r--r--   0 shyue      (501) staff       (20)      219 2016-09-25 20:11:02.000000 pymatgen-4.7.7/MANIFEST.in
+-rw-r--r--   0 shyue      (501) staff       (20)    10890 2017-05-27 14:41:40.000000 pymatgen-4.7.7/PKG-INFO
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:38.000000 pymatgen-4.7.7/pymatgen/
+-rw-r--r--   0 shyue      (501) staff       (20)     2773 2017-05-27 14:41:08.000000 pymatgen-4.7.7/pymatgen/__init__.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:38.000000 pymatgen-4.7.7/pymatgen/alchemy/
+-rw-r--r--   0 shyue      (501) staff       (20)      228 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/alchemy/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    11447 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/alchemy/filters.py
+-rw-r--r--   0 shyue      (501) staff       (20)    14267 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/alchemy/materials.py
+-rw-r--r--   0 shyue      (501) staff       (20)    16735 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/alchemy/transmuters.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:39.000000 pymatgen-4.7.7/pymatgen/analysis/
+-rw-r--r--   0 shyue      (501) staff       (20)      217 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    25361 2017-03-07 21:24:46.000000 pymatgen-4.7.7/pymatgen/analysis/adsorption.py
+-rw-r--r--   0 shyue      (501) staff       (20)    21703 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/bond_valence.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1240 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/analysis/bonds_jmol_ob.yaml
+-rw-r--r--   0 shyue      (501) staff       (20)     1770 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/bvparam_1991.yaml
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:39.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/
+-rw-r--r--   0 shyue      (501) staff       (20)       26 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/__init__.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:39.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/
+-rw-r--r--   0 shyue      (501) staff       (20)       26 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    84066 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/chemenv_strategies.py
+-rw-r--r--   0 shyue      (501) staff       (20)    51388 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:39.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/
+-rw-r--r--   0 shyue      (501) staff       (20)       26 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)      511 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/A#2.json
+-rw-r--r--   0 shyue      (501) staff       (20)     4980 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/AC#12.json
+-rw-r--r--   0 shyue      (501) staff       (20)     2682 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/allcg.txt
+-rw-r--r--   0 shyue      (501) staff       (20)     3653 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/BO_1#8.json
+-rw-r--r--   0 shyue      (501) staff       (20)     5530 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/BO_2#8.json
+-rw-r--r--   0 shyue      (501) staff       (20)     4909 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/BO_3#8.json
+-rw-r--r--   0 shyue      (501) staff       (20)     3124 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/BS_1#10.json
+-rw-r--r--   0 shyue      (501) staff       (20)    10526 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/BS_2#10.json
+-rw-r--r--   0 shyue      (501) staff       (20)     7863 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/C#12.json
+-rw-r--r--   0 shyue      (501) staff       (20)     2865 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/C#8.json
+-rw-r--r--   0 shyue      (501) staff       (20)      258 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/CO#11.json
+-rw-r--r--   0 shyue      (501) staff       (20)      260 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/DD#20.json
+-rw-r--r--   0 shyue      (501) staff       (20)     2310 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/DD#8.json
+-rw-r--r--   0 shyue      (501) staff       (20)     2378 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/DDPN#8.json
+-rw-r--r--   0 shyue      (501) staff       (20)     9900 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/DI#11.json
+-rw-r--r--   0 shyue      (501) staff       (20)     3406 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/ET#7.json
+-rw-r--r--   0 shyue      (501) staff       (20)     2521 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/FO#7.json
+-rw-r--r--   0 shyue      (501) staff       (20)      262 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/H#10.json
+-rw-r--r--   0 shyue      (501) staff       (20)     8230 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/H#11.json
+-rw-r--r--   0 shyue      (501) staff       (20)     2631 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/HA#12.json
+-rw-r--r--   0 shyue      (501) staff       (20)     2999 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/HB#8.json
+-rw-r--r--   0 shyue      (501) staff       (20)     1640 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/HD#9.json
+-rw-r--r--   0 shyue      (501) staff       (20)     8053 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/HP#12.json
+-rw-r--r--   0 shyue      (501) staff       (20)     7469 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/I#12.json
+-rw-r--r--   0 shyue      (501) staff       (20)      495 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/L#2.json
+-rw-r--r--   0 shyue      (501) staff       (20)     7956 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/MI#10.json
+-rw-r--r--   0 shyue      (501) staff       (20)     2916 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/O#6.json
+-rw-r--r--   0 shyue      (501) staff       (20)     1204 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/O#6_explicit.json
+-rw-r--r--   0 shyue      (501) staff       (20)     7566 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PA#10.json
+-rw-r--r--   0 shyue      (501) staff       (20)     2564 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PB#7.json
+-rw-r--r--   0 shyue      (501) staff       (20)    12676 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PBP#12.json
+-rw-r--r--   0 shyue      (501) staff       (20)    17243 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PCPA#11.json
+-rw-r--r--   0 shyue      (501) staff       (20)     3743 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PP#10.json
+-rw-r--r--   0 shyue      (501) staff       (20)      999 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PP#5.json
+-rw-r--r--   0 shyue      (501) staff       (20)     2353 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PP#6.json
+-rw-r--r--   0 shyue      (501) staff       (20)      464 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/S#1.json
+-rw-r--r--   0 shyue      (501) staff       (20)      256 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/S#10.json
+-rw-r--r--   0 shyue      (501) staff       (20)      260 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/S#12.json
+-rw-r--r--   0 shyue      (501) staff       (20)      647 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/S#4.json
+-rw-r--r--   0 shyue      (501) staff       (20)      979 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/S#5.json
+-rw-r--r--   0 shyue      (501) staff       (20)     3215 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SA#8.json
+-rw-r--r--   0 shyue      (501) staff       (20)    12423 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SBSA#10.json
+-rw-r--r--   0 shyue      (501) staff       (20)     3574 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SBT#8.json
+-rw-r--r--   0 shyue      (501) staff       (20)     2612 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SC#12.json
+-rw-r--r--   0 shyue      (501) staff       (20)      970 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SH#11.json
+-rw-r--r--   0 shyue      (501) staff       (20)     6312 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SH#13.json
+-rw-r--r--   0 shyue      (501) staff       (20)     9708 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SMA#9.json
+-rw-r--r--   0 shyue      (501) staff       (20)      708 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SS#4.json
+-rw-r--r--   0 shyue      (501) staff       (20)     5992 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SS#9.json
+-rw-r--r--   0 shyue      (501) staff       (20)     2829 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/ST#7.json
+-rw-r--r--   0 shyue      (501) staff       (20)      780 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SY#4.json
+-rw-r--r--   0 shyue      (501) staff       (20)      887 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/T#4.json
+-rw-r--r--   0 shyue      (501) staff       (20)      991 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/T#5.json
+-rw-r--r--   0 shyue      (501) staff       (20)     2374 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/T#6.json
+-rw-r--r--   0 shyue      (501) staff       (20)     8161 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TBSA#10.json
+-rw-r--r--   0 shyue      (501) staff       (20)     2008 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TBT#8.json
+-rw-r--r--   0 shyue      (501) staff       (20)     6515 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TC#9.json
+-rw-r--r--   0 shyue      (501) staff       (20)     4868 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TI#9.json
+-rw-r--r--   0 shyue      (501) staff       (20)      625 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TL#3.json
+-rw-r--r--   0 shyue      (501) staff       (20)    14523 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TO_1#9.json
+-rw-r--r--   0 shyue      (501) staff       (20)     8184 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TO_2#9.json
+-rw-r--r--   0 shyue      (501) staff       (20)    10703 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TO_3#9.json
+-rw-r--r--   0 shyue      (501) staff       (20)      583 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TS#3.json
+-rw-r--r--   0 shyue      (501) staff       (20)     7895 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TT#12.json
+-rw-r--r--   0 shyue      (501) staff       (20)     7757 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TT_1#9.json
+-rw-r--r--   0 shyue      (501) staff       (20)    12608 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TT_2#9.json
+-rw-r--r--   0 shyue      (501) staff       (20)     5258 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TT_3#9.json
+-rw-r--r--   0 shyue      (501) staff       (20)      724 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TY#3.json
+-rw-r--r--   0 shyue      (501) staff       (20)    75875 2016-10-19 06:56:38.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometry_finder.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:39.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/strategy_files/
+-rw-r--r--   0 shyue      (501) staff       (20)       26 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/strategy_files/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)      844 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/strategy_files/ImprovedConfidenceCutoffDefaultParameters.json
+-rw-r--r--   0 shyue      (501) staff       (20)    79050 2017-01-03 01:28:02.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/structure_environments.py
+-rw-r--r--   0 shyue      (501) staff       (20)    36849 2016-12-03 05:41:54.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/voronoi.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:39.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/utils/
+-rw-r--r--   0 shyue      (501) staff       (20)       26 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/utils/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     8193 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/utils/chemenv_config.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3780 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/utils/chemenv_errors.py
+-rw-r--r--   0 shyue      (501) staff       (20)    34349 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/utils/coordination_geometry_utils.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3527 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/utils/defs_utils.py
+-rw-r--r--   0 shyue      (501) staff       (20)     7225 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/utils/func_utils.py
+-rw-r--r--   0 shyue      (501) staff       (20)     9465 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/utils/math_utils.py
+-rw-r--r--   0 shyue      (501) staff       (20)    15858 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/chemenv/utils/scripts_utils.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:39.000000 pymatgen-4.7.7/pymatgen/analysis/cost/
+-rw-r--r--   0 shyue      (501) staff       (20)      299 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/cost/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6048 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/cost/cost.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:39.000000 pymatgen-4.7.7/pymatgen/analysis/defects/
+-rw-r--r--   0 shyue      (501) staff       (20)      203 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/defects/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    53295 2017-04-01 23:01:31.000000 pymatgen-4.7.7/pymatgen/analysis/defects/dilute_solution_model.py
+-rw-r--r--   0 shyue      (501) staff       (20)     7631 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/defects/ionic_radii.json
+-rw-r--r--   0 shyue      (501) staff       (20)    72613 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/analysis/defects/point_defects.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1510 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/defects/surf_error.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:39.000000 pymatgen-4.7.7/pymatgen/analysis/diffraction/
+-rw-r--r--   0 shyue      (501) staff       (20)      439 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/diffraction/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6760 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/diffraction/atomic_scattering_params.json
+-rw-r--r--   0 shyue      (501) staff       (20)    14977 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/analysis/diffraction/xrd.py
+-rw-r--r--   0 shyue      (501) staff       (20)    35366 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/analysis/diffusion_analyzer.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:39.000000 pymatgen-4.7.7/pymatgen/analysis/elasticity/
+-rw-r--r--   0 shyue      (501) staff       (20)      220 2017-02-02 21:53:25.000000 pymatgen-4.7.7/pymatgen/analysis/elasticity/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    26939 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/analysis/elasticity/elastic.py
+-rw-r--r--   0 shyue      (501) staff       (20)    10794 2017-05-14 16:37:00.000000 pymatgen-4.7.7/pymatgen/analysis/elasticity/strain.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3571 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/analysis/elasticity/stress.py
+-rw-r--r--   0 shyue      (501) staff       (20)    19994 2017-05-27 14:38:07.000000 pymatgen-4.7.7/pymatgen/analysis/elasticity/tensors.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5624 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/energy_models.py
+-rw-r--r--   0 shyue      (501) staff       (20)    17394 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/analysis/eos.py
+-rw-r--r--   0 shyue      (501) staff       (20)    24382 2017-05-14 16:37:00.000000 pymatgen-4.7.7/pymatgen/analysis/ewald.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:39.000000 pymatgen-4.7.7/pymatgen/analysis/ferroelectricity/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2017-04-19 12:25:30.000000 pymatgen-4.7.7/pymatgen/analysis/ferroelectricity/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    15811 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/analysis/ferroelectricity/polarization.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:39.000000 pymatgen-4.7.7/pymatgen/analysis/hhi/
+-rw-r--r--   0 shyue      (501) staff       (20)      131 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/hhi/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3806 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/hhi/hhi.py
+-rw-r--r--   0 shyue      (501) staff       (20)    34095 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/icsd_bv.yaml
+-rw-r--r--   0 shyue      (501) staff       (20)    25092 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/analysis/molecule_matcher.py
+-rw-r--r--   0 shyue      (501) staff       (20)     7931 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/molecule_structure_comparator.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4047 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/nmr.py
+-rw-r--r--   0 shyue      (501) staff       (20)    18284 2017-03-24 21:58:11.000000 pymatgen-4.7.7/pymatgen/analysis/path_finder.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1682 2017-04-01 23:01:31.000000 pymatgen-4.7.7/pymatgen/analysis/piezo.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:39.000000 pymatgen-4.7.7/pymatgen/analysis/pourbaix/
+-rw-r--r--   0 shyue      (501) staff       (20)      108 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/pourbaix/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     9840 2016-12-03 05:41:54.000000 pymatgen-4.7.7/pymatgen/analysis/pourbaix/analyzer.py
+-rw-r--r--   0 shyue      (501) staff       (20)    14039 2017-04-01 23:01:31.000000 pymatgen-4.7.7/pymatgen/analysis/pourbaix/entry.py
+-rw-r--r--   0 shyue      (501) staff       (20)    17124 2017-04-01 23:01:31.000000 pymatgen-4.7.7/pymatgen/analysis/pourbaix/maker.py
+-rw-r--r--   0 shyue      (501) staff       (20)    34827 2017-03-07 21:24:46.000000 pymatgen-4.7.7/pymatgen/analysis/pourbaix/plotter.py
+-rw-r--r--   0 shyue      (501) staff       (20)    12109 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/analysis/quasiharmonic.py
+-rw-r--r--   0 shyue      (501) staff       (20)    16693 2017-03-07 21:24:46.000000 pymatgen-4.7.7/pymatgen/analysis/reaction_calculator.py
+-rw-r--r--   0 shyue      (501) staff       (20)    86029 2017-05-23 05:53:16.000000 pymatgen-4.7.7/pymatgen/analysis/structure_analyzer.py
+-rw-r--r--   0 shyue      (501) staff       (20)    42586 2017-01-16 16:23:39.000000 pymatgen-4.7.7/pymatgen/analysis/structure_matcher.py
+-rw-r--r--   0 shyue      (501) staff       (20)    18671 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/substrate_analyzer.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3335 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/analysis/thermochemistry.py
+-rw-r--r--   0 shyue      (501) staff       (20)    12402 2017-03-07 21:24:46.000000 pymatgen-4.7.7/pymatgen/analysis/transition_state.py
+-rw-r--r--   0 shyue      (501) staff       (20)    20227 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/analysis/wulff.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:39.000000 pymatgen-4.7.7/pymatgen/apps/
+-rw-r--r--   0 shyue      (501) staff       (20)      210 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/apps/__init__.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:39.000000 pymatgen-4.7.7/pymatgen/apps/battery/
+-rw-r--r--   0 shyue      (501) staff       (20)      256 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/apps/battery/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     8873 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/apps/battery/analyzer.py
+-rw-r--r--   0 shyue      (501) staff       (20)    12215 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/apps/battery/battery_abc.py
+-rw-r--r--   0 shyue      (501) staff       (20)    20877 2017-01-16 16:23:39.000000 pymatgen-4.7.7/pymatgen/apps/battery/conversion_battery.py
+-rw-r--r--   0 shyue      (501) staff       (20)    20634 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/apps/battery/insertion_battery.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3443 2017-03-07 21:24:46.000000 pymatgen-4.7.7/pymatgen/apps/battery/plotter.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:39.000000 pymatgen-4.7.7/pymatgen/apps/borg/
+-rw-r--r--   0 shyue      (501) staff       (20)      229 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/apps/borg/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    17218 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/apps/borg/hive.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4998 2017-02-02 21:53:25.000000 pymatgen-4.7.7/pymatgen/apps/borg/queen.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:39.000000 pymatgen-4.7.7/pymatgen/cli/
+-rw-r--r--   0 shyue      (501) staff       (20)      289 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/cli/__init__.py
+-rwxr-xr-x   0 shyue      (501) staff       (20)     2148 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/cli/feff_input_generation.py
+-rwxr-xr-x   0 shyue      (501) staff       (20)     1996 2017-03-07 21:24:46.000000 pymatgen-4.7.7/pymatgen/cli/feff_plot_cross_section.py
+-rwxr-xr-x   0 shyue      (501) staff       (20)     2193 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/cli/feff_plot_dos.py
+-rwxr-xr-x   0 shyue      (501) staff       (20)     3347 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/cli/gaussian_analyzer.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1341 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/cli/get_environment.py
+-rwxr-xr-x   0 shyue      (501) staff       (20)    14089 2017-01-16 16:23:39.000000 pymatgen-4.7.7/pymatgen/cli/pmg.py
+-rwxr-xr-x   0 shyue      (501) staff       (20)     4753 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/cli/pmg_analyze.py
+-rwxr-xr-x   0 shyue      (501) staff       (20)     6791 2017-01-03 01:28:02.000000 pymatgen-4.7.7/pymatgen/cli/pmg_config.py
+-rwxr-xr-x   0 shyue      (501) staff       (20)     2497 2017-03-07 21:24:46.000000 pymatgen-4.7.7/pymatgen/cli/pmg_plot.py
+-rwxr-xr-x   0 shyue      (501) staff       (20)     1147 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/cli/pmg_potcar.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1907 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/cli/pmg_query.py
+-rwxr-xr-x   0 shyue      (501) staff       (20)     3397 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/cli/pmg_structure.py
+-rwxr-xr-x   0 shyue      (501) staff       (20)    23839 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/cli/pydii.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:39.000000 pymatgen-4.7.7/pymatgen/command_line/
+-rw-r--r--   0 shyue      (501) staff       (20)      277 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/command_line/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3605 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/command_line/aconvasp_caller.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6078 2017-01-03 01:28:02.000000 pymatgen-4.7.7/pymatgen/command_line/bader_caller.py
+-rw-r--r--   0 shyue      (501) staff       (20)    15800 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/command_line/enumlib_caller.py
+-rw-r--r--   0 shyue      (501) staff       (20)    26892 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/command_line/gulp_caller.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5726 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/command_line/OxideTersoffPotentials
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:39.000000 pymatgen-4.7.7/pymatgen/core/
+-rw-r--r--   0 shyue      (501) staff       (20)      640 2016-11-16 04:40:15.000000 pymatgen-4.7.7/pymatgen/core/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3408 2017-04-19 12:25:30.000000 pymatgen-4.7.7/pymatgen/core/bond_lengths.json
+-rw-r--r--   0 shyue      (501) staff       (20)     3875 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/core/bonds.py
+-rw-r--r--   0 shyue      (501) staff       (20)    31944 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/core/composition.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2822 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/core/func_groups.json
+-rw-r--r--   0 shyue      (501) staff       (20)     7310 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/core/ion.py
+-rw-r--r--   0 shyue      (501) staff       (20)    42044 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/core/lattice.py
+-rw-r--r--   0 shyue      (501) staff       (20)    58185 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/core/libxc_docs.json
+-rw-r--r--   0 shyue      (501) staff       (20)    13121 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/core/libxcfunc.py
+-rw-r--r--   0 shyue      (501) staff       (20)    21597 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/core/operations.py
+-rw-r--r--   0 shyue      (501) staff       (20)   120293 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/core/periodic_table.json
+-rw-r--r--   0 shyue      (501) staff       (20)    37149 2017-03-07 21:24:46.000000 pymatgen-4.7.7/pymatgen/core/periodic_table.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1935 2016-12-16 05:48:52.000000 pymatgen-4.7.7/pymatgen/core/physical_constants.py
+-rw-r--r--   0 shyue      (501) staff       (20)    18993 2017-03-07 21:24:46.000000 pymatgen-4.7.7/pymatgen/core/sites.py
+-rw-r--r--   0 shyue      (501) staff       (20)   129233 2017-05-17 05:02:55.000000 pymatgen-4.7.7/pymatgen/core/structure.py
+-rw-r--r--   0 shyue      (501) staff       (20)    44320 2017-03-07 21:24:46.000000 pymatgen-4.7.7/pymatgen/core/surface.py
+-rw-r--r--   0 shyue      (501) staff       (20)    27827 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/core/units.py
+-rw-r--r--   0 shyue      (501) staff       (20)    10353 2017-03-24 21:58:11.000000 pymatgen-4.7.7/pymatgen/core/xcfunc.py
+-rw-r--r--   0 shyue      (501) staff       (20)      695 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/dao.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:39.000000 pymatgen-4.7.7/pymatgen/electronic_structure/
+-rw-r--r--   0 shyue      (501) staff       (20)      189 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/electronic_structure/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    39691 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/electronic_structure/bandstructure.py
+-rw-r--r--   0 shyue      (501) staff       (20)    95579 2017-05-26 21:05:35.000000 pymatgen-4.7.7/pymatgen/electronic_structure/boltztrap.py
+-rw-r--r--   0 shyue      (501) staff       (20)    15423 2017-05-17 05:02:55.000000 pymatgen-4.7.7/pymatgen/electronic_structure/core.py
+-rw-r--r--   0 shyue      (501) staff       (20)    17289 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/electronic_structure/dos.py
+-rw-r--r--   0 shyue      (501) staff       (20)   161089 2017-05-26 21:06:44.000000 pymatgen-4.7.7/pymatgen/electronic_structure/plotter.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:39.000000 pymatgen-4.7.7/pymatgen/entries/
+-rw-r--r--   0 shyue      (501) staff       (20)      297 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/entries/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    24628 2017-04-06 03:57:47.000000 pymatgen-4.7.7/pymatgen/entries/compatibility.py
+-rw-r--r--   0 shyue      (501) staff       (20)     7315 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/entries/computed_entries.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5906 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/entries/entry_tools.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2795 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/entries/exp_entries.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2174 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/entries/MITCompatibility.yaml
+-rw-r--r--   0 shyue      (501) staff       (20)     2604 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/entries/MPCompatibility.yaml
+-rw-r--r--   0 shyue      (501) staff       (20)     1459 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/entries/post_processors_abc.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:39.000000 pymatgen-4.7.7/pymatgen/io/
+-rw-r--r--   0 shyue      (501) staff       (20)      233 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/__init__.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:40.000000 pymatgen-4.7.7/pymatgen/io/abinit/
+-rw-r--r--   0 shyue      (501) staff       (20)      226 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/abinit/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    19214 2017-03-24 21:58:11.000000 pymatgen-4.7.7/pymatgen/io/abinit/abiinspect.py
+-rw-r--r--   0 shyue      (501) staff       (20)    49706 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/io/abinit/abiobjects.py
+-rw-r--r--   0 shyue      (501) staff       (20)    29828 2017-04-19 12:25:30.000000 pymatgen-4.7.7/pymatgen/io/abinit/abitimer.py
+-rw-r--r--   0 shyue      (501) staff       (20)    17803 2017-03-24 21:58:11.000000 pymatgen-4.7.7/pymatgen/io/abinit/calculations.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4991 2017-03-07 21:24:46.000000 pymatgen-4.7.7/pymatgen/io/abinit/db.py
+-rw-r--r--   0 shyue      (501) staff       (20)    28225 2016-11-02 22:55:22.000000 pymatgen-4.7.7/pymatgen/io/abinit/events.py
+-rw-r--r--   0 shyue      (501) staff       (20)   106450 2017-04-19 12:25:30.000000 pymatgen-4.7.7/pymatgen/io/abinit/flows.py
+-rw-r--r--   0 shyue      (501) staff       (20)     7018 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/abinit/helpers.py
+-rw-r--r--   0 shyue      (501) staff       (20)    47837 2017-03-24 21:58:11.000000 pymatgen-4.7.7/pymatgen/io/abinit/launcher.py
+-rw-r--r--   0 shyue      (501) staff       (20)    10393 2017-03-24 21:58:11.000000 pymatgen-4.7.7/pymatgen/io/abinit/netcdf.py
+-rw-r--r--   0 shyue      (501) staff       (20)    38373 2017-03-24 21:58:11.000000 pymatgen-4.7.7/pymatgen/io/abinit/nodes.py
+-rw-r--r--   0 shyue      (501) staff       (20)    63356 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/io/abinit/pseudos.py
+-rw-r--r--   0 shyue      (501) staff       (20)    79542 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/io/abinit/qadapters.py
+-rw-r--r--   0 shyue      (501) staff       (20)    17260 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/abinit/qjobs.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3763 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/abinit/qutils.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3632 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/abinit/scheduler_error_handlers.py
+-rw-r--r--   0 shyue      (501) staff       (20)    14014 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/abinit/scheduler_error_parsers.py
+-rw-r--r--   0 shyue      (501) staff       (20)   171911 2017-03-24 21:58:11.000000 pymatgen-4.7.7/pymatgen/io/abinit/tasks.py
+-rw-r--r--   0 shyue      (501) staff       (20)    27984 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/io/abinit/utils.py
+-rw-r--r--   0 shyue      (501) staff       (20)    56476 2017-03-24 21:58:11.000000 pymatgen-4.7.7/pymatgen/io/abinit/works.py
+-rw-r--r--   0 shyue      (501) staff       (20)    12127 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/abinit/wrappers.py
+-rw-r--r--   0 shyue      (501) staff       (20)    31523 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/io/adf.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2129 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/aiida.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1985 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/ase.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4995 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/babel.py
+-rw-r--r--   0 shyue      (501) staff       (20)    50443 2017-05-25 20:34:29.000000 pymatgen-4.7.7/pymatgen/io/cif.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3039 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/io/cssr.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:40.000000 pymatgen-4.7.7/pymatgen/io/exciting/
+-rw-r--r--   0 shyue      (501) staff       (20)      267 2017-03-07 21:24:46.000000 pymatgen-4.7.7/pymatgen/io/exciting/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    11846 2017-03-07 21:24:46.000000 pymatgen-4.7.7/pymatgen/io/exciting/inputs.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:40.000000 pymatgen-4.7.7/pymatgen/io/feff/
+-rw-r--r--   0 shyue      (501) staff       (20)      311 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/feff/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    32326 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/io/feff/inputs.py
+-rw-r--r--   0 shyue      (501) staff       (20)      405 2016-10-19 06:56:38.000000 pymatgen-4.7.7/pymatgen/io/feff/MPELNESSet.yaml
+-rw-r--r--   0 shyue      (501) staff       (20)      112 2017-03-07 21:24:46.000000 pymatgen-4.7.7/pymatgen/io/feff/MPEXAFSSet.yaml
+-rw-r--r--   0 shyue      (501) staff       (20)      362 2016-10-19 06:56:38.000000 pymatgen-4.7.7/pymatgen/io/feff/MPEXELFSSet.yaml
+-rw-r--r--   0 shyue      (501) staff       (20)      161 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/feff/MPXANESSet.yaml
+-rw-r--r--   0 shyue      (501) staff       (20)    12025 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/io/feff/outputs.py
+-rw-r--r--   0 shyue      (501) staff       (20)    16295 2017-03-07 21:24:46.000000 pymatgen-4.7.7/pymatgen/io/feff/sets.py
+-rw-r--r--   0 shyue      (501) staff       (20)    28823 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/io/fiesta.py
+-rw-r--r--   0 shyue      (501) staff       (20)    53491 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/io/gaussian.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:40.000000 pymatgen-4.7.7/pymatgen/io/lammps/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/lammps/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    33053 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/io/lammps/data.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3235 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/lammps/force_field.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6304 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/lammps/input.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1141 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/lammps/NPT.json
+-rw-r--r--   0 shyue      (501) staff       (20)     1244 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/lammps/NPT_NVT.json
+-rw-r--r--   0 shyue      (501) staff       (20)      908 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/lammps/NVT.json
+-rw-r--r--   0 shyue      (501) staff       (20)    16467 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/io/lammps/output.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5153 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/lammps/topology.py
+-rw-r--r--   0 shyue      (501) staff       (20)    15202 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/lammps/utils.py
+-rw-r--r--   0 shyue      (501) staff       (20)    32329 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/io/nwchem.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6155 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/io/phonopy.py
+-rw-r--r--   0 shyue      (501) staff       (20)    17277 2017-05-26 21:07:21.000000 pymatgen-4.7.7/pymatgen/io/pwscf.py
+-rw-r--r--   0 shyue      (501) staff       (20)    87307 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/io/qchem.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:40.000000 pymatgen-4.7.7/pymatgen/io/vasp/
+-rw-r--r--   0 shyue      (501) staff       (20)      456 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/vasp/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1456 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/vasp/GWVaspInputSet.yaml
+-rw-r--r--   0 shyue      (501) staff       (20)    26739 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/vasp/GWvaspinputsets.py
+-rw-r--r--   0 shyue      (501) staff       (20)    72033 2017-05-17 02:35:57.000000 pymatgen-4.7.7/pymatgen/io/vasp/inputs.py
+-rw-r--r--   0 shyue      (501) staff       (20)     7374 2017-04-01 23:01:31.000000 pymatgen-4.7.7/pymatgen/io/vasp/MITRelaxSet.yaml
+-rw-r--r--   0 shyue      (501) staff       (20)     1331 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/vasp/MPHSERelaxSet.yaml
+-rw-r--r--   0 shyue      (501) staff       (20)     2023 2017-05-17 02:34:11.000000 pymatgen-4.7.7/pymatgen/io/vasp/MPRelaxSet.yaml
+-rw-r--r--   0 shyue      (501) staff       (20)   137250 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/io/vasp/outputs.py
+-rw-r--r--   0 shyue      (501) staff       (20)    58824 2017-05-17 02:43:06.000000 pymatgen-4.7.7/pymatgen/io/vasp/sets.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3382 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/io/xcrysden.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6272 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/io/xr.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3960 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/io/xyz.py
+-rw-r--r--   0 shyue      (501) staff       (20)    18986 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/io/zeopp.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:40.000000 pymatgen-4.7.7/pymatgen/matproj/
+-rw-r--r--   0 shyue      (501) staff       (20)      196 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/matproj/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    39592 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/matproj/rest.py
+-rw-r--r--   0 shyue      (501) staff       (20)    13687 2017-05-25 20:34:29.000000 pymatgen-4.7.7/pymatgen/matproj/snl.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:40.000000 pymatgen-4.7.7/pymatgen/optimization/
+-rw-r--r--   0 shyue      (501) staff       (20)      109 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/optimization/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)   901516 2016-10-23 04:19:30.000000 pymatgen-4.7.7/pymatgen/optimization/linear_assignment.c
+-rw-r--r--   0 shyue      (501) staff       (20)     8016 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/optimization/linear_assignment.pyx
+-rw-r--r--   0 shyue      (501) staff       (20)     8228 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/optimization/linear_assignment_numpy.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:40.000000 pymatgen-4.7.7/pymatgen/phasediagram/
+-rw-r--r--   0 shyue      (501) staff       (20)      410 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/phasediagram/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    19907 2017-04-01 23:01:31.000000 pymatgen-4.7.7/pymatgen/phasediagram/analyzer.py
+-rw-r--r--   0 shyue      (501) staff       (20)     9519 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/phasediagram/entries.py
+-rw-r--r--   0 shyue      (501) staff       (20)    18276 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/phasediagram/maker.py
+-rw-r--r--   0 shyue      (501) staff       (20)    30521 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/phasediagram/plotter.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:40.000000 pymatgen-4.7.7/pymatgen/phonon/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2017-02-02 21:53:25.000000 pymatgen-4.7.7/pymatgen/phonon/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    18026 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/phonon/bandstructure.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5900 2017-02-02 21:53:25.000000 pymatgen-4.7.7/pymatgen/phonon/dos.py
+-rw-r--r--   0 shyue      (501) staff       (20)    15693 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/phonon/plotter.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:40.000000 pymatgen-4.7.7/pymatgen/serializers/
+-rw-r--r--   0 shyue      (501) staff       (20)      211 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/serializers/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1194 2017-03-24 21:58:11.000000 pymatgen-4.7.7/pymatgen/serializers/json_coders.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3272 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/serializers/pickle_coders.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:40.000000 pymatgen-4.7.7/pymatgen/structure_prediction/
+-rw-r--r--   0 shyue      (501) staff       (20)      108 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/structure_prediction/__init__.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:40.000000 pymatgen-4.7.7/pymatgen/structure_prediction/data/
+-rw-r--r--   0 shyue      (501) staff       (20)   184884 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/structure_prediction/data/lambda.json
+-rw-r--r--   0 shyue      (501) staff       (20)   256410 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/structure_prediction/data/pair_correlation.json
+-rw-r--r--   0 shyue      (501) staff       (20)     8996 2017-04-19 12:25:30.000000 pymatgen-4.7.7/pymatgen/structure_prediction/substitution_probability.py
+-rw-r--r--   0 shyue      (501) staff       (20)    10618 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/structure_prediction/substitutor.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:40.000000 pymatgen-4.7.7/pymatgen/symmetry/
+-rw-r--r--   0 shyue      (501) staff       (20)      203 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/symmetry/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    54060 2017-05-14 16:37:00.000000 pymatgen-4.7.7/pymatgen/symmetry/analyzer.py
+-rw-r--r--   0 shyue      (501) staff       (20)    29835 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/symmetry/bandstructure.py
+-rw-r--r--   0 shyue      (501) staff       (20)    18471 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/symmetry/groups.py
+-rw-r--r--   0 shyue      (501) staff       (20)    23828 2017-05-20 15:04:46.000000 pymatgen-4.7.7/pymatgen/symmetry/maggroups.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2849 2017-04-01 23:01:31.000000 pymatgen-4.7.7/pymatgen/symmetry/structure.py
+-rw-r--r--   0 shyue      (501) staff       (20)    48218 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/symmetry/symm_data.yaml
+-rw-r--r--   0 shyue      (501) staff       (20)   422366 2016-10-19 06:56:38.000000 pymatgen-4.7.7/pymatgen/symmetry/symm_ops.json
+-rw-r--r--   0 shyue      (501) staff       (20)   443429 2016-10-19 06:56:38.000000 pymatgen-4.7.7/pymatgen/symmetry/symm_ops.yaml
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:40.000000 pymatgen-4.7.7/pymatgen/transformations/
+-rw-r--r--   0 shyue      (501) staff       (20)      256 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/transformations/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    33684 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/transformations/advanced_transformations.py
+-rw-r--r--   0 shyue      (501) staff       (20)    11269 2017-04-01 23:01:31.000000 pymatgen-4.7.7/pymatgen/transformations/defect_transformations.py
+-rw-r--r--   0 shyue      (501) staff       (20)    20998 2017-02-02 21:53:25.000000 pymatgen-4.7.7/pymatgen/transformations/site_transformations.py
+-rw-r--r--   0 shyue      (501) staff       (20)    23008 2017-01-16 16:23:39.000000 pymatgen-4.7.7/pymatgen/transformations/standard_transformations.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2734 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/transformations/transformation_abc.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:40.000000 pymatgen-4.7.7/pymatgen/util/
+-rw-r--r--   0 shyue      (501) staff       (20)      309 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/util/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    14863 2017-03-24 21:58:11.000000 pymatgen-4.7.7/pymatgen/util/convergence.py
+-rw-r--r--   0 shyue      (501) staff       (20)    15753 2017-04-19 12:25:30.000000 pymatgen-4.7.7/pymatgen/util/coord_utils.py
+-rw-r--r--   0 shyue      (501) staff       (20)   992710 2016-12-03 05:41:54.000000 pymatgen-4.7.7/pymatgen/util/coord_utils_cython.c
+-rw-r--r--   0 shyue      (501) staff       (20)     8664 2016-12-03 05:41:54.000000 pymatgen-4.7.7/pymatgen/util/coord_utils_cython.pyx
+-rw-r--r--   0 shyue      (501) staff       (20)     6016 2017-03-24 21:58:11.000000 pymatgen-4.7.7/pymatgen/util/io_utils.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3740 2017-03-07 21:24:46.000000 pymatgen-4.7.7/pymatgen/util/num.py
+-rw-r--r--   0 shyue      (501) staff       (20)      181 2017-03-07 21:24:46.000000 pymatgen-4.7.7/pymatgen/util/num_utils.py
+-rw-r--r--   0 shyue      (501) staff       (20)    10567 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/util/plotting.py
+-rw-r--r--   0 shyue      (501) staff       (20)      196 2017-03-07 21:24:46.000000 pymatgen-4.7.7/pymatgen/util/plotting_utils.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3733 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/util/string.py
+-rw-r--r--   0 shyue      (501) staff       (20)      190 2017-03-07 21:24:46.000000 pymatgen-4.7.7/pymatgen/util/string_utils.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:40.000000 pymatgen-4.7.7/pymatgen/util/structures/
+-rw-r--r--   0 shyue      (501) staff       (20)     2647 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/util/structures/BaNiO3.json
+-rw-r--r--   0 shyue      (501) staff       (20)      524 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/util/structures/CsCl.json
+-rw-r--r--   0 shyue      (501) staff       (20)     1183 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/util/structures/Graphite.json
+-rw-r--r--   0 shyue      (501) staff       (20)     2239 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/util/structures/K2O2.json
+-rw-r--r--   0 shyue      (501) staff       (20)    11142 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/util/structures/Li10GeP2S12.json
+-rw-r--r--   0 shyue      (501) staff       (20)     1032 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/util/structures/Li2O.json
+-rw-r--r--   0 shyue      (501) staff       (20)     2270 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/util/structures/Li2O2.json
+-rw-r--r--   0 shyue      (501) staff       (20)    10384 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/util/structures/Li3V2(PO4)3.json
+-rw-r--r--   0 shyue      (501) staff       (20)     6007 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/util/structures/LiFePO4.json
+-rw-r--r--   0 shyue      (501) staff       (20)     5871 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/util/structures/NaFePO4.json
+-rw-r--r--   0 shyue      (501) staff       (20)      660 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/util/structures/Si.json
+-rw-r--r--   0 shyue      (501) staff       (20)     1446 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/util/structures/Sn.json
+-rw-r--r--   0 shyue      (501) staff       (20)     1095 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/util/structures/SrTiO3.json
+-rw-r--r--   0 shyue      (501) staff       (20)     1641 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/util/structures/TiO2.json
+-rw-r--r--   0 shyue      (501) staff       (20)     1007 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/util/structures/VO2.json
+-rw-r--r--   0 shyue      (501) staff       (20)     6039 2017-03-07 21:24:46.000000 pymatgen-4.7.7/pymatgen/util/testing.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:40.000000 pymatgen-4.7.7/pymatgen/vis/
+-rw-r--r--   0 shyue      (501) staff       (20)      211 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/vis/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4494 2016-09-25 20:11:03.000000 pymatgen-4.7.7/pymatgen/vis/ElementColorSchemes.yaml
+-rw-r--r--   0 shyue      (501) staff       (20)     3231 2017-02-02 21:53:25.000000 pymatgen-4.7.7/pymatgen/vis/structure_chemview.py
+-rw-r--r--   0 shyue      (501) staff       (20)    47019 2017-05-09 20:42:44.000000 pymatgen-4.7.7/pymatgen/vis/structure_vtk.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2017-05-27 14:41:38.000000 pymatgen-4.7.7/pymatgen.egg-info/
+-rw-r--r--   0 shyue      (501) staff       (20)        1 2017-05-27 14:41:37.000000 pymatgen-4.7.7/pymatgen.egg-info/dependency_links.txt
+-rw-r--r--   0 shyue      (501) staff       (20)      367 2017-05-27 14:41:37.000000 pymatgen-4.7.7/pymatgen.egg-info/entry_points.txt
+-rw-r--r--   0 shyue      (501) staff       (20)    10890 2017-05-27 14:41:37.000000 pymatgen-4.7.7/pymatgen.egg-info/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)      345 2017-05-27 14:41:37.000000 pymatgen-4.7.7/pymatgen.egg-info/requires.txt
+-rw-r--r--   0 shyue      (501) staff       (20)    16123 2017-05-27 14:41:37.000000 pymatgen-4.7.7/pymatgen.egg-info/SOURCES.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        9 2017-05-27 14:41:37.000000 pymatgen-4.7.7/pymatgen.egg-info/top_level.txt
+-rw-r--r--   0 shyue      (501) staff       (20)     8265 2017-05-09 20:42:44.000000 pymatgen-4.7.7/README.rst
+-rw-r--r--   0 shyue      (501) staff       (20)       95 2017-05-25 20:34:29.000000 pymatgen-4.7.7/requirements-optional.txt
+-rw-r--r--   0 shyue      (501) staff       (20)      220 2017-05-25 20:34:29.000000 pymatgen-4.7.7/requirements.txt
+-rw-r--r--   0 shyue      (501) staff       (20)      112 2017-05-27 14:41:40.000000 pymatgen-4.7.7/setup.cfg
+-rw-r--r--   0 shyue      (501) staff       (20)     5473 2017-05-27 14:41:36.000000 pymatgen-4.7.7/setup.py
```

### Comparing `pymatgen-4.7.6/CHANGES.rst` & `pymatgen-4.7.7/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Change log
 ==========
 
+v4.7.7
+------
+* Magnetic symmetry and CIF support. (Horton)
+* Improved PWSCF Input file generation.
+* Misc bug fixes.
+
 v4.7.6
 ------
 * Fix serious bug in PointGroupAnalyzer that resulted in wrong point groups assigned to non-centered molecules.
 * Useful get_structure_from_mp at the root level for quick retrieval of common structures for analysis.
 * More efficient kpoint grids.
 * Misc bug fixes.
```

### Comparing `pymatgen-4.7.6/LICENSE.rst` & `pymatgen-4.7.7/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/PKG-INFO` & `pymatgen-4.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pymatgen
-Version: 4.7.6
+Version: 4.7.7
 Summary: Python Materials Genomics is a robust materials analysis code that defines core object representations for structures and molecules with support for many electronic structure codes. It is currently the core analysis code powering the Materials Project (https://www.materialsproject.org).
 Home-page: http://www.pymatgen.org
 Author: Shyue Ping Ong
 Author-email: ongsp@eng.ucsd.edu
 License: MIT
 Description: 
         .. image:: https://circleci.com/gh/materialsproject/pymatgen.svg?style=shield&circle-token=:circle-token
```

### Comparing `pymatgen-4.7.6/pymatgen/__init__.py` & `pymatgen-4.7.7/pymatgen/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from __future__ import unicode_literals
 
 import os
+import warnings
+import yaml
 
 __author__ = "Pymatgen Development Team"
 __email__ ="pymatgen@googlegroups.com"
 __maintainer__ = "Shyue Ping Ong"
 __maintainer_email__ ="shyuep@gmail.com"
-__date__ = "May 14 2017"
-__version__ = "4.7.6"
+__date__ = "May 27 2017"
+__version__ = "4.7.7"
 
 
 SETTINGS_FILE = os.path.join(os.path.expanduser("~"), ".pmgrc.yaml")
 
 
 def _load_pmg_settings():
     try:
-        import yaml
         with open(SETTINGS_FILE, "rt") as f:
             d = yaml.load(f)
     except IOError:
         # If there are any errors, default to using environment variables
         # if present.
         d = {}
         for k, v in os.environ.items():
             if k.startswith("PMG_"):
                 d[k] = v
             elif k in ["VASP_PSP_DIR", "MAPI_KEY", "DEFAULT_FUNCTIONAL"]:
                 d["PMG_" + k] = v
     clean_d = {}
     for k, v in d.items():
         if not k.startswith("PMG_"):
-            import warnings
             warnings.warn('With effect from pmg 5.0, all pymatgen settings are'
                           ' prefixed with a "PMG_". E.g., "PMG_VASP_PSP_DIR" '
                           'instead of "VASP_PSP_DIR".')
             clean_d["PMG_" + k] = v
         else:
             clean_d[k] = v
     return clean_d
@@ -56,16 +56,23 @@
     """
     if not SETTINGS.get("PMG_MAPI_KEY"):
         raise RuntimeError("PMG_MAPI_KEY must be set in .pmgrc.yaml to use this "
                            "function.")
 
     from pymatgen.matproj.rest import MPRester
     m = MPRester()
-    return min(m.get_entries(formula, inc_structure=True),
-               key=lambda e: e.energy_per_atom).structure
+    entries = m.get_entries(formula, inc_structure=True)
+    if len(entries) == 0:
+        raise ValueError("No structure with formula %s in Materials Project!" %
+                         formula)
+    elif len(entries) > 1:
+        warnings.warn("%d structures with formula %s found in Materials Project."
+                      "The lowest energy structure will be returned." %
+                      (len(entries), formula))
+    return min(entries, key=lambda e: e.energy_per_atom).structure
 
 
 # Order of imports is important on some systems to avoid
 # failures when loading shared libraries.
 # import spglib
 # from . import optimization, util
 # del(spglib, optimization, util)
```

### Comparing `pymatgen-4.7.6/pymatgen/alchemy/filters.py` & `pymatgen-4.7.7/pymatgen/alchemy/filters.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/alchemy/materials.py` & `pymatgen-4.7.7/pymatgen/alchemy/materials.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/alchemy/transmuters.py` & `pymatgen-4.7.7/pymatgen/alchemy/transmuters.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/adsorption.py` & `pymatgen-4.7.7/pymatgen/analysis/adsorption.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/bond_valence.py` & `pymatgen-4.7.7/pymatgen/analysis/bond_valence.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/bonds_jmol_ob.yaml` & `pymatgen-4.7.7/pymatgen/analysis/bonds_jmol_ob.yaml`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/bvparam_1991.yaml` & `pymatgen-4.7.7/pymatgen/analysis/bvparam_1991.yaml`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/chemenv_strategies.py` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/chemenv_strategies.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries.py` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/AC#12.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/AC#12.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/allcg.txt` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/allcg.txt`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/BO_1#8.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/BO_1#8.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/BO_2#8.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/BO_2#8.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/BO_3#8.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/BO_3#8.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/BS_1#10.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/BS_1#10.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/BS_2#10.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/BS_2#10.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/C#12.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/C#12.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/C#8.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/C#8.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/DD#8.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/DD#8.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/DDPN#8.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/DDPN#8.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/DI#11.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/DI#11.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/ET#7.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/ET#7.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/FO#7.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/FO#7.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/H#11.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/H#11.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/HA#12.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/HA#12.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/HB#8.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/HB#8.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/HD#9.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/HD#9.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/HP#12.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/HP#12.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/I#12.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/I#12.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/MI#10.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/MI#10.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/O#6.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/O#6.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/O#6_explicit.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/O#6_explicit.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PA#10.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PA#10.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PB#7.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PB#7.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PBP#12.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PBP#12.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PCPA#11.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PCPA#11.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PP#10.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PP#10.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PP#5.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PP#5.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PP#6.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/PP#6.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/S#4.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/S#4.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/S#5.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/S#5.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SA#8.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SA#8.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SBSA#10.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SBSA#10.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SBT#8.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SBT#8.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SC#12.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SC#12.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SH#11.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SH#11.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SH#13.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SH#13.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SMA#9.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SMA#9.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SS#4.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SS#4.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SS#9.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SS#9.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/ST#7.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/ST#7.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SY#4.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/SY#4.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/T#4.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/T#4.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/T#5.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/T#5.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/T#6.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/T#6.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TBSA#10.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TBSA#10.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TBT#8.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TBT#8.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TC#9.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TC#9.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TI#9.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TI#9.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TL#3.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TL#3.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TO_1#9.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TO_1#9.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TO_2#9.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TO_2#9.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TO_3#9.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TO_3#9.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TS#3.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TS#3.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TT#12.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TT#12.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TT_1#9.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TT_1#9.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TT_2#9.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TT_2#9.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TT_3#9.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TT_3#9.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TY#3.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometries_files/TY#3.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/coordination_geometry_finder.py` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/coordination_geometry_finder.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/strategy_files/ImprovedConfidenceCutoffDefaultParameters.json` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/strategy_files/ImprovedConfidenceCutoffDefaultParameters.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/structure_environments.py` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/structure_environments.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/coordination_environments/voronoi.py` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/coordination_environments/voronoi.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/utils/chemenv_config.py` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/utils/chemenv_config.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/utils/chemenv_errors.py` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/utils/chemenv_errors.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/utils/coordination_geometry_utils.py` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/utils/coordination_geometry_utils.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/utils/defs_utils.py` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/utils/defs_utils.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/utils/func_utils.py` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/utils/func_utils.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/utils/math_utils.py` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/utils/math_utils.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/chemenv/utils/scripts_utils.py` & `pymatgen-4.7.7/pymatgen/analysis/chemenv/utils/scripts_utils.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/cost/cost.py` & `pymatgen-4.7.7/pymatgen/analysis/cost/cost.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/defects/dilute_solution_model.py` & `pymatgen-4.7.7/pymatgen/analysis/defects/dilute_solution_model.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/defects/ionic_radii.json` & `pymatgen-4.7.7/pymatgen/analysis/defects/ionic_radii.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/defects/point_defects.py` & `pymatgen-4.7.7/pymatgen/analysis/defects/point_defects.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/defects/surf_error.py` & `pymatgen-4.7.7/pymatgen/analysis/defects/surf_error.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/diffraction/atomic_scattering_params.json` & `pymatgen-4.7.7/pymatgen/analysis/diffraction/atomic_scattering_params.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/diffraction/xrd.py` & `pymatgen-4.7.7/pymatgen/analysis/diffraction/xrd.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/diffusion_analyzer.py` & `pymatgen-4.7.7/pymatgen/analysis/diffusion_analyzer.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/elasticity/elastic.py` & `pymatgen-4.7.7/pymatgen/analysis/elasticity/elastic.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/elasticity/strain.py` & `pymatgen-4.7.7/pymatgen/analysis/elasticity/strain.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/elasticity/stress.py` & `pymatgen-4.7.7/pymatgen/analysis/elasticity/stress.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/elasticity/tensors.py` & `pymatgen-4.7.7/pymatgen/analysis/elasticity/tensors.py`

 * *Files 5% similar despite different names*

```diff
@@ -266,23 +266,29 @@
             raise ValueError("Invalid shape for voigt matrix")
         voigt_input = voigt_input / t._vscale
         this_voigt_map = t.get_voigt_dict(rank)
         for ind in this_voigt_map:
             t[ind] = voigt_input[this_voigt_map[ind]]
         return cls(t)
 
-    def convert_to_ieee(self, structure):
+    def convert_to_ieee(self, structure, initial_fit=True):
         """
         Given a structure associated with a tensor, attempts a
         calculation of the tensor in IEEE format according to
         the 1987 IEEE standards.
 
         Args:
             structure (Structure): a structure associated with the
                 tensor to be converted to the IEEE standard
+            initial_fit (bool): flag to indicate whether initial
+                tensor is fit to the symmetry of the structure.
+                Defaults to true. Note that if false, inconsistent
+                results may be obtained due to symmetrically
+                equivalent, but distinct transformations
+                being used in different versions of spglib.
         """
 
         def get_uvec(v):
             """ Gets a unit vector parallel to input vector"""
             l = np.linalg.norm(v)
             if l < 1e-8:
                 return v
@@ -344,15 +350,18 @@
         # IEEE rules: c || x3
         elif xtal_sys == "triclinic":
             rotation = [vec / mag for (mag, vec) in sorted(zip(lengths, vecs))]
             rotation = np.roll(rotation, 2, axis=0)
             rotation[1] = get_uvec(np.cross(rotation[2], rotation[1]))
             rotation[0] = np.cross(rotation[1], rotation[2])
 
-        return self.rotate(rotation, tol=1e-2)
+        result = self.copy()
+        if initial_fit:
+            result = result.fit_to_structure(structure)
+        return result.rotate(rotation, tol=1e-2)
 
 
 class TensorCollection(collections.Sequence):
     """
     A sequence of tensors that can be used for fitting data
     or for having a tensor expansion
     """
```

### Comparing `pymatgen-4.7.6/pymatgen/analysis/energy_models.py` & `pymatgen-4.7.7/pymatgen/analysis/energy_models.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/eos.py` & `pymatgen-4.7.7/pymatgen/analysis/eos.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/ewald.py` & `pymatgen-4.7.7/pymatgen/analysis/ewald.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/ferroelectricity/polarization.py` & `pymatgen-4.7.7/pymatgen/analysis/ferroelectricity/polarization.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/hhi/hhi.py` & `pymatgen-4.7.7/pymatgen/analysis/hhi/hhi.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/icsd_bv.yaml` & `pymatgen-4.7.7/pymatgen/analysis/icsd_bv.yaml`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/molecule_matcher.py` & `pymatgen-4.7.7/pymatgen/analysis/molecule_matcher.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/molecule_structure_comparator.py` & `pymatgen-4.7.7/pymatgen/analysis/molecule_structure_comparator.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/nmr.py` & `pymatgen-4.7.7/pymatgen/analysis/nmr.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/path_finder.py` & `pymatgen-4.7.7/pymatgen/analysis/path_finder.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/piezo.py` & `pymatgen-4.7.7/pymatgen/analysis/piezo.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/pourbaix/analyzer.py` & `pymatgen-4.7.7/pymatgen/analysis/pourbaix/analyzer.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/pourbaix/entry.py` & `pymatgen-4.7.7/pymatgen/analysis/pourbaix/entry.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/pourbaix/maker.py` & `pymatgen-4.7.7/pymatgen/analysis/pourbaix/maker.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/pourbaix/plotter.py` & `pymatgen-4.7.7/pymatgen/analysis/pourbaix/plotter.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/quasiharmonic.py` & `pymatgen-4.7.7/pymatgen/analysis/quasiharmonic.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/reaction_calculator.py` & `pymatgen-4.7.7/pymatgen/analysis/reaction_calculator.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/structure_analyzer.py` & `pymatgen-4.7.7/pymatgen/analysis/structure_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -847,16 +847,16 @@
 class OrderParameters(object):
     """
     This class permits the calculation of various types of local order
     parameters.
     """
 
     __supported_types = (
-            "cn", "lin", "bent", "tet", "oct", "bcc", "q2", "q4", "q6",
-            "reg_tri", "sq", "sq_pyr", "tri_bipyr")
+            "cn", "lin", "bent", "tet", "tetalt", "oct", "octalt", "bcc",
+            "q2", "q4", "q6", "reg_tri", "sq", "sq_pyr", "tri_bipyr")
 
     def __init__(self, types, parameters=None, cutoff=-10.0):
         """
         Create an OrderParameter analyzer instance.
 
         Args:
             types ([string]):
@@ -1019,14 +1019,24 @@
                 else:
                     if loc_parameters[i][0] == 0.0:
                         raise ValueError("Gaussian width for"
                                          " tetrahedral order"
                                          " parameter is zero!")
                     else:
                         tmpparas[i].append(1.0 / loc_parameters[i][0])
+            elif t == "tetalt":
+                if len(loc_parameters[i]) == 0:
+                    tmpparas[i].append(1.0 / 0.0667)
+                else:
+                    if loc_parameters[i][0] == 0.0:
+                        raise ValueError("Gaussian width for"
+                                         " tetrahedral order"
+                                         " parameter is zero!")
+                    else:
+                        tmpparas[i].append(1.0 / loc_parameters[i][0])
             elif t == "oct":
                 if len(loc_parameters[i]) < 4:
                     tmpparas[i].append(8.0 * pi / 9.0)
                     tmpparas[i].append(1.0 / 0.0667)
                     tmpparas[i].append(1.0 / 0.0556)
                     tmpparas[i].append(0.25)
                     tmpparas[i].append(4.0 / 3.0)
@@ -1052,14 +1062,38 @@
                     if loc_parameters[i][3] - 1.0 == 0.0:
                         raise ValueError("Shift constant may not be"
                                          " unity!")
                     if loc_parameters[i][3] < 0.0 or loc_parameters[i][3] > 1.0:
                         warn("Shift constant outside [0,1[.")
                     tmpparas[i].append(loc_parameters[i][3])
                     tmpparas[i].append(1.0 / (1.0 - loc_parameters[i][3]))
+            elif t == "octalt":
+                if len(loc_parameters[i]) < 3:
+                    tmpparas[i].append(8.0 * pi / 9.0)
+                    tmpparas[i].append(1.0 / 0.0667)
+                    tmpparas[i].append(1.0 / 0.0556)
+                else:
+                    if loc_parameters[i][0] <= 0.0 or loc_parameters[i][
+                            0] >= 180.0:
+                        warn("Threshold value for south pole"
+                             " configurations in octahedral order"
+                             " parameter outside ]0,180[")
+                    tmpparas[i].append(loc_parameters[i][0] * pi / 180.0)
+                    if loc_parameters[i][1] == 0.0:
+                        raise ValueError("Gaussian width for south pole"
+                                         " configurations in octahedral"
+                                         " order parameter is zero!")
+                    else:
+                        tmpparas[i].append(1.0 / loc_parameters[i][1])
+                    if loc_parameters[i][2] == 0.0:
+                        raise ValueError("Gaussian width for equatorial"
+                                         " configurations in octahedral"
+                                         " order parameter is zero!")
+                    else:
+                        tmpparas[i].append(1.0 / loc_parameters[i][2])
             elif t == "bcc":
                 if len(loc_parameters[i]) < 2:
                     tmpparas[i].append(8.0 * pi / 9.0)
                     tmpparas[i].append(1.0 / 0.0667)
                 else:
                     if loc_parameters[i][0] <= 0.0 or loc_parameters[i][
                         0] >= 180.0:
@@ -1136,15 +1170,15 @@
 
             # Add here any additional flags to be used during calculation.
             # self._computerijs: compute vectors from centeral atom i
             #                    to any neighbor j.
             # self._computerjks: compute vectors from non-centeral atom j
             #                    to any non-central atom k.
             if t == "tet" or t == "oct" or t == "bcc" or t == "sq_pyr" or \
-                    t == "tri_bipyr":
+                    t == "tri_bipyr" or t == "tetalt" or t == "octalt":
                 self._computerijs = self._geomops = True
             if t == "reg_tri" or t =="sq":
                 self._computerijs = self._computerjks = self._geomops2 = True
             if t == "q2" or t == "q4" or t == "q6":
                 self._computerijs = self._boops = True
             if t == "q2" and self._max_trig_order < 2:
                 self._max_trig_order = 2
@@ -1834,19 +1868,19 @@
                             if t == "lin":
                                 tmp = self._paras[i][0] * (thetak * ipi - 1.0)
                                 ops[i] += exp(-0.5 * tmp * tmp)
                             elif t == "bent":
                                 tmp = self._paras[i][1] * (
                                     thetak * ipi - self._paras[i][0])
                                 ops[i] += exp(-0.5 * tmp * tmp)
-                            elif t == "tet":
+                            elif t == "tet" or t == "tetalt":
                                 tmp = self._paras[i][0] * (
                                     thetak * ipi - tetangoverpi)
                                 gaussthetak[i] = math.exp(-0.5 * tmp * tmp)
-                            elif t == "oct":
+                            elif t == "oct" or t == "octalt":
                                 if thetak >= self._paras[i][0]:
                                     # k is south pole to j
                                     tmp = self._paras[i][1] * (
                                         thetak * ipi - 1.0)
                                     ops[i] += 3.0 * math.exp(-0.5 * tmp * tmp)
                             elif t == "bcc" and j < k:
                                 if thetak >= self._paras[i][0]:
@@ -1885,26 +1919,41 @@
                                     for i, t in enumerate(self._types):
                                         if t == "tet":
                                             tmp = self._paras[i][0] * (
                                                 thetam * ipi - tetangoverpi)
                                             ops[i] += gaussthetak[i] * math.exp(
                                                 -0.5 * tmp * tmp) * math.cos(
                                                 3.0 * phi)
+                                        elif t == "tetalt":
+                                            tmp = self._paras[i][0] * (
+                                                thetam * ipi - tetangoverpi)
+                                            tmp2 = math.cos(1.5 * phi)
+                                            ops[i] += gaussthetak[i] * math.exp(
+                                                -0.5 * tmp * tmp) * tmp2 * tmp2
                                         elif t == "oct":
                                             if thetak < self._paras[i][0] and \
                                                             thetam < \
                                                             self._paras[i][0]:
                                                 tmp = math.cos(2.0 * phi)
                                                 tmp2 = self._paras[i][2] * (
                                                     thetam * ipi - 0.5)
                                                 ops[i] += tmp * tmp * \
                                                           self._paras[i][4] * (
                                                               math.exp(
                                                                   -0.5 * tmp2 * tmp2) - \
                                                               self._paras[i][3])
+                                        elif t == "octalt":
+                                            if thetak < self._paras[i][0] and \
+                                                    thetam < self._paras[i][0]:
+                                                tmp = math.cos(2.0 * phi)
+                                                tmp2 = self._paras[i][2] * (
+                                                        thetam * ipi - 0.5)
+                                                ops[i] += tmp * tmp * \
+                                                        math.exp(
+                                                        -0.5 * tmp2 * tmp2)
                                         elif t == "bcc" and j < k:
                                             if thetak < self._paras[i][0]:
                                                 if thetak > piover2:
                                                     fac = 1.0
                                                 else:
                                                     fac = -1.0
                                                 tmp = (thetam - piover2) / (
@@ -1929,18 +1978,18 @@
             for i, t in enumerate(self._types):
                 if t == "lin":
                     ops[i] = ops[i] / float(nneigh * (
                             nneigh - 1)) if nneigh > 1 else None
                 elif t == "bent":
                     ops[i] = ops[i] / float(nneigh * (
                             nneigh - 1)) if nneigh > 1 else None
-                elif t == "tet":
+                elif t == "tet" or t == "tetalt":
                     ops[i] = ops[i] / float(nneigh * (nneigh - 1) * (
                             nneigh - 2)) if nneigh > 2 else None
-                elif t == "oct":
+                elif t == "oct" or t == "octalt":
                     ops[i] = ops[i] / float(nneigh * (3 + (nneigh - 2) * (
                             nneigh - 3))) if nneigh > 3 else None
                 elif t == "bcc":
                     ops[i] = ops[i] / float(0.5 * float(
                             nneigh * (6 + (nneigh - 2) * (nneigh - 3)))) \
                             if nneigh > 3 else None
                 elif t == "sq_pyr":
```

### Comparing `pymatgen-4.7.6/pymatgen/analysis/structure_matcher.py` & `pymatgen-4.7.7/pymatgen/analysis/structure_matcher.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/substrate_analyzer.py` & `pymatgen-4.7.7/pymatgen/analysis/substrate_analyzer.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/thermochemistry.py` & `pymatgen-4.7.7/pymatgen/analysis/thermochemistry.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/transition_state.py` & `pymatgen-4.7.7/pymatgen/analysis/transition_state.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/analysis/wulff.py` & `pymatgen-4.7.7/pymatgen/analysis/wulff.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/apps/battery/analyzer.py` & `pymatgen-4.7.7/pymatgen/apps/battery/analyzer.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/apps/battery/battery_abc.py` & `pymatgen-4.7.7/pymatgen/apps/battery/battery_abc.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/apps/battery/conversion_battery.py` & `pymatgen-4.7.7/pymatgen/apps/battery/conversion_battery.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/apps/battery/insertion_battery.py` & `pymatgen-4.7.7/pymatgen/apps/battery/insertion_battery.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/apps/battery/plotter.py` & `pymatgen-4.7.7/pymatgen/apps/battery/plotter.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/apps/borg/hive.py` & `pymatgen-4.7.7/pymatgen/apps/borg/hive.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/apps/borg/queen.py` & `pymatgen-4.7.7/pymatgen/apps/borg/queen.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/cli/feff_input_generation.py` & `pymatgen-4.7.7/pymatgen/cli/feff_input_generation.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/cli/feff_plot_cross_section.py` & `pymatgen-4.7.7/pymatgen/cli/feff_plot_cross_section.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/cli/feff_plot_dos.py` & `pymatgen-4.7.7/pymatgen/cli/feff_plot_dos.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/cli/gaussian_analyzer.py` & `pymatgen-4.7.7/pymatgen/cli/gaussian_analyzer.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/cli/get_environment.py` & `pymatgen-4.7.7/pymatgen/cli/get_environment.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/cli/pmg.py` & `pymatgen-4.7.7/pymatgen/cli/pmg.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/cli/pmg_analyze.py` & `pymatgen-4.7.7/pymatgen/cli/pmg_analyze.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/cli/pmg_config.py` & `pymatgen-4.7.7/pymatgen/cli/pmg_config.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/cli/pmg_plot.py` & `pymatgen-4.7.7/pymatgen/cli/pmg_plot.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/cli/pmg_potcar.py` & `pymatgen-4.7.7/pymatgen/cli/pmg_potcar.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/cli/pmg_query.py` & `pymatgen-4.7.7/pymatgen/cli/pmg_query.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/cli/pmg_structure.py` & `pymatgen-4.7.7/pymatgen/cli/pmg_structure.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/cli/pydii.py` & `pymatgen-4.7.7/pymatgen/cli/pydii.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/command_line/aconvasp_caller.py` & `pymatgen-4.7.7/pymatgen/command_line/aconvasp_caller.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/command_line/bader_caller.py` & `pymatgen-4.7.7/pymatgen/command_line/bader_caller.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/command_line/enumlib_caller.py` & `pymatgen-4.7.7/pymatgen/command_line/enumlib_caller.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/command_line/gulp_caller.py` & `pymatgen-4.7.7/pymatgen/command_line/gulp_caller.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/command_line/OxideTersoffPotentials` & `pymatgen-4.7.7/pymatgen/command_line/OxideTersoffPotentials`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/core/__init__.py` & `pymatgen-4.7.7/pymatgen/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/core/bond_lengths.json` & `pymatgen-4.7.7/pymatgen/core/bond_lengths.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/core/bonds.py` & `pymatgen-4.7.7/pymatgen/core/bonds.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/core/composition.py` & `pymatgen-4.7.7/pymatgen/core/composition.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/core/func_groups.json` & `pymatgen-4.7.7/pymatgen/core/func_groups.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/core/ion.py` & `pymatgen-4.7.7/pymatgen/core/ion.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/core/lattice.py` & `pymatgen-4.7.7/pymatgen/core/lattice.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/core/libxc_docs.json` & `pymatgen-4.7.7/pymatgen/core/libxc_docs.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/core/libxcfunc.py` & `pymatgen-4.7.7/pymatgen/core/libxcfunc.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/core/operations.py` & `pymatgen-4.7.7/pymatgen/core/operations.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/core/periodic_table.json` & `pymatgen-4.7.7/pymatgen/core/periodic_table.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/core/periodic_table.py` & `pymatgen-4.7.7/pymatgen/core/periodic_table.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/core/physical_constants.py` & `pymatgen-4.7.7/pymatgen/core/physical_constants.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/core/sites.py` & `pymatgen-4.7.7/pymatgen/core/sites.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/core/structure.py` & `pymatgen-4.7.7/pymatgen/core/structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -528,14 +528,118 @@
             all_sp.extend([sp] * len(cc))
             all_coords.extend(cc)
             for k, v in props.items():
                 all_site_properties[k].extend([v[i]] * len(cc))
 
         return cls(latt, all_sp, all_coords,
                    site_properties=all_site_properties)
+                   
+    @classmethod
+    def from_magnetic_spacegroup(cls, msg, lattice, species, coords, site_properties,
+                                  transform_setting=None, coords_are_cartesian=False, tol=1e-5):
+         """
+         Generate a structure using a magnetic spacegroup. Note that only
+         symmetrically distinct species, coords and magmoms should be provided.]
+         All equivalent sites are generated from the spacegroup operations.
+
+         Args:
+             msg (str/list/:class:`pymatgen.symmetry.maggroups.MagneticSpaceGroup`):
+                 The magnetic spacegroup.
+                 If a string, it will be interpreted as one of the notations
+                 supported by MagneticSymmetryGroup, e.g., "R-3'c" or "Fm'-3'm".
+                 If a list of two ints, it will be interpreted as the number of
+                 the spacegroup in its Belov, Neronova and Smirnova (BNS) setting.
+             lattice (Lattice/3x3 array): The lattice, either as a
+                 :class:`pymatgen.core.lattice.Lattice` or
+                 simply as any 2D array. Each row should correspond to a lattice
+                 vector. E.g., [[10,0,0], [20,10,0], [0,0,30]] specifies a
+                 lattice with lattice vectors [10,0,0], [20,10,0] and [0,0,30].
+                 Note that no attempt is made to check that the lattice is
+                 compatible with the spacegroup specified. This may be
+                 introduced in a future version.
+             species ([Specie]): Sequence of species on each site. Can take in
+                 flexible input, including:
+
+                 i.  A sequence of element / specie specified either as string
+                     symbols, e.g. ["Li", "Fe2+", "P", ...] or atomic numbers,
+                     e.g., (3, 56, ...) or actual Element or Specie objects.
+
+                 ii. List of dict of elements/species and occupancies, e.g.,
+                     [{"Fe" : 0.5, "Mn":0.5}, ...]. This allows the setup of
+                     disordered structures.
+             coords (Nx3 array): list of fractional/cartesian coordinates of
+                 each species.
+             site_properties (dict): Properties associated with the sites as a
+                 dict of sequences, e.g., {"magmom":[5,5,5,5]}. The sequences
+                 have to be the same length as the atomic species and
+                 fractional_coords. Unlike Structure.from_spacegroup(),
+                 this argument is mandatory, since magnetic moment information
+                 has to be included. Note that the *direction* of the supplied
+                 magnetic moment relative to the crystal is important, even if
+                 the resulting structure is used for collinear calculations.
+             coords_are_cartesian (bool): Set to True if you are providing
+                 coordinates in cartesian coordinates. Defaults to False.
+             tol (float): A fractional tolerance to deal with numerical
+                precision issues in determining if orbits are the same.
+         """
+         from pymatgen.electronic_structure.core import Magmom
+         from pymatgen.symmetry.maggroups import MagneticSpaceGroup
+
+         if 'magmom' not in site_properties:
+             raise ValueError('Magnetic moments have to be defined.')
+         else:
+             magmoms = [Magmom(m) for m in site_properties['magmom']]
+
+         if not isinstance(msg, MagneticSpaceGroup):
+             msg = MagneticSpaceGroup(msg)
+
+         if isinstance(lattice, Lattice):
+             latt = lattice
+         else:
+             latt = Lattice(lattice)
+
+         if not msg.is_compatible(latt):
+             raise ValueError(
+                 "Supplied lattice with parameters %s is incompatible with "
+                 "supplied spacegroup %s!" % (latt.lengths_and_angles,
+                                              sgp.symbol)
+             )
+
+         if len(species) != len(coords):
+             raise ValueError(
+                 "Supplied species and coords lengths (%d vs %d) are "
+                 "different!" % (len(species), len(coords))
+             )
+
+         if len(species) != len(magmoms):
+             raise ValueError(
+                 "Supplied species and magmom lengths (%d vs %d) are "
+                 "different!" % (len(species), len(magmoms))
+             )
+
+         frac_coords = coords if not coords_are_cartesian else \
+             lattice.get_fractional_coords(coords)
+
+         all_sp = []
+         all_coords = []
+         all_magmoms = []
+         all_site_properties = collections.defaultdict(list)
+         for i, (sp, c, m) in enumerate(zip(species, frac_coords, magmoms)):
+             cc, mm = msg.get_orbit(c, m, tol=tol)
+             all_sp.extend([sp] * len(cc))
+             all_coords.extend(cc)
+             all_magmoms.extend(mm)
+             for k, v in site_properties.items():
+                 if k != 'magmom':
+                     all_site_properties[k].extend([v[i]] * len(cc))
+
+         all_site_properties['magmom'] = all_magmoms
+
+         return cls(latt, all_sp, all_coords,
+                    site_properties=all_site_properties)
 
     @property
     def distance_matrix(self):
         """
         Returns the distance matrix between all sites in the structure. For
         periodic structures, this should return the nearest image distance.
         """
```

### Comparing `pymatgen-4.7.6/pymatgen/core/surface.py` & `pymatgen-4.7.7/pymatgen/core/surface.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/core/units.py` & `pymatgen-4.7.7/pymatgen/core/units.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/core/xcfunc.py` & `pymatgen-4.7.7/pymatgen/core/xcfunc.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/dao.py` & `pymatgen-4.7.7/pymatgen/dao.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/electronic_structure/bandstructure.py` & `pymatgen-4.7.7/pymatgen/electronic_structure/bandstructure.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/electronic_structure/boltztrap.py` & `pymatgen-4.7.7/pymatgen/electronic_structure/boltztrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1992,39 +1992,51 @@
                                  doping, mu_doping, seebeck_doping,
                                  cond_doping, kappa_doping, hall_doping, dos,
                                  dos_partial, carrier_conc, vol, warning)
 
 
 def read_cube_file(filename):
     with open(filename, 'rt') as f:
-        natoms = 0
-        count_line = 0
-        for line in f:
-            line = line.rstrip("\n")
-            if count_line == 0 and "CUBE" not in line:
-                raise ValueError("CUBE file format not recognized")
-
-            if count_line == 2:
-                tokens = line.split()
-                natoms = int(tokens[0])
-            if count_line == 3:
-                tokens = line.split()
-                n1 = int(tokens[0])
-            elif count_line == 4:
-                tokens = line.split()
-                n2 = int(tokens[0])
-            elif count_line == 5:
-                tokens = line.split()
-                n3 = int(tokens[0])
-            elif count_line > 5:
-                break
-
-            count_line += 1
-
-    energy_data = np.loadtxt(filename, skiprows=natoms + 6).reshape(n1, n2, n3)
+            natoms = 0
+            count_line = 0
+            for line in f:
+                line = line.rstrip("\n")
+                if count_line == 0 and "CUBE" not in line:
+                    raise ValueError("CUBE file format not recognized")
+
+                if count_line == 2:
+                    tokens = line.split()
+                    origin = [float(tokens[i]) for i in range(1,4)]
+                    natoms = int(tokens[0])
+                if count_line == 3:
+                    tokens = line.split()
+                    a1 = [float(tokens[i]) for i in range(1,4)]
+                    n1 = int(tokens[0])
+                elif count_line == 4:
+                    tokens = line.split()
+                    a2 = [float(tokens[i]) for i in range(1,4)]
+                    n2 = int(tokens[0])
+                elif count_line == 5:
+                    tokens = line.split()
+                    a3 = [float(tokens[i]) for i in range(1,4)]
+                    n3 = int(tokens[0])
+                    #kpoints=[[[0 for i in range(0,n1)] for j in range(0,n2)] for l in range(0,n3)]
+                elif count_line > 5:
+                    break
+
+                count_line += 1
+
+    if 'fort.30' in filename:
+        energy_data = np.genfromtxt(filename,skip_header=natoms+6,skip_footer=1)
+        nlines_data = len(energy_data)
+        last_line = np.genfromtxt(filename,skip_header=nlines_data+natoms+6)
+        energy_data = np.append(energy_data.flatten(),last_line).reshape(n1,n2,n3)
+    elif 'boltztrap_BZ.cube' in filename:
+        energy_data = np.loadtxt(filename,skiprows=natoms+6).reshape(n1,n2,n3)
+    
     energy_data /= Energy(1, "eV").to("Ry")
 
     return energy_data
 
 
 def compare_sym_bands(bands_obj, bands_ref_obj, nb=None):
     """
```

### Comparing `pymatgen-4.7.6/pymatgen/electronic_structure/core.py` & `pymatgen-4.7.7/pymatgen/electronic_structure/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -463,15 +463,15 @@
         antiferromagnetic collinear structures without additional
         user intervention.
 
         However, should be used with caution for non-collinear
         structures and might give non-sensical results except in the case
         of only slightly non-collinear structures (e.g. small canting).
         """
-        return self.get_00t_magmom_with_xyz_saxis()[2]
+        return float(self.get_00t_magmom_with_xyz_saxis()[2])
 
     def __str__(self):
         return str(float(self))
 
     def __repr__(self):
         if np.allclose(self.saxis, (0, 0, 1)):
             return 'Magnetic moment {0}'.format(self.moment, self.saxis)
```

### Comparing `pymatgen-4.7.6/pymatgen/electronic_structure/dos.py` & `pymatgen-4.7.7/pymatgen/electronic_structure/dos.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/electronic_structure/plotter.py` & `pymatgen-4.7.7/pymatgen/electronic_structure/plotter.py`

 * *Files 10% similar despite different names*

```diff
@@ -521,17 +521,17 @@
 #                                     tck, der=0)
 #                                  for x in range(1000)], 'r--',
 #                                 linewidth=band_linewidth)
 
         self._maketicks(plt)
 
         # Main X and Y Labels
-        plt.xlabel(r'$\mathrm{Wave\ Vector}$', fontsize=30)
-        ylabel = r'$\mathrm{E\ -\ E_f\ (eV)}$' if zero_to_efermi \
-            else r'$\mathrm{Energy\ (eV)}$'
+        plt.xlabel(r'$\\mathrm{Wave\ Vector}$', fontsize=30)
+        ylabel = r'$\\mathrm{E\ -\ E_f\ (eV)}$' if zero_to_efermi \
+            else r'$\\mathrm{Energy\ (eV)}$'
         plt.ylabel(ylabel, fontsize=30)
 
         # Draw Fermi energy, only if not the zero
         if not zero_to_efermi:
             ef = self._bs.efermi
             plt.axhline(ef, linewidth=2, color='k')
 
@@ -633,42 +633,55 @@
                         tick_labels.append("$" + c.label + "$")
                     else:
                         tick_labels.append(c.label)
                 previous_label = c.label
                 previous_branch = this_branch
         return {'distance': tick_distance, 'label': tick_labels}
 
-    def plot_compare(self, other_plotter):
+    def plot_compare(self, other_plotter, legend=True):
         """
         plot two band structure for comparison. One is in red the other in blue
         (no difference in spins). The two band structures need to be defined
         on the same symmetry lines! and the distance between symmetry lines is
         the one of the band structure used to build the BSPlotter
 
         Args:
             another band structure object defined along the same symmetry lines
 
         Returns:
             a matplotlib object with both band structures
 
         """
         # TODO: add exception if the band structures are not compatible
+        import matplotlib.lines as mlines
         plt = self.get_plot()
         data_orig = self.bs_plot_data()
         data = other_plotter.bs_plot_data()
         band_linewidth = 1
         for i in range(other_plotter._nb_bands):
             for d in range(len(data_orig['distances'])):
                 plt.plot(data_orig['distances'][d],
                          [e[str(Spin.up)][i] for e in data['energy']][d],
-                         'r-', linewidth=band_linewidth)
-        if other_plotter._bs.is_spin_polarized:
-            plt.plot(data_orig['distances'],
-                     [e for e in data['energy'][i][str(Spin.down)]],
-                     'r-', linewidth=band_linewidth)
+                         'c-', linewidth=band_linewidth)
+                if other_plotter._bs.is_spin_polarized:
+                    plt.plot(data_orig['distances'][d],
+                             [e[str(Spin.down)][i] for e in data['energy']][d],
+                             'm--', linewidth=band_linewidth)
+        if legend:
+            handles = [mlines.Line2D([], [], linewidth=2,
+                                     color='b', label='bs 1 up'),
+                       mlines.Line2D([], [], linewidth=2,
+                                     color='r', label='bs 1 down', linestyle="--"),
+                       mlines.Line2D([], [], linewidth=2,
+                                     color='c', label='bs 2 up'),
+                       mlines.Line2D([], [], linewidth=2,
+                                     color='m', linestyle="--",
+                                     label='bs 2 down')]
+
+            plt.legend(handles=handles)
         return plt
 
     def plot_brillouin(self):
         """
         plot the Brillouin zone
         """
 
@@ -2510,14 +2523,513 @@
             plt.xlim(xlim)
         plt.ylabel("ZT", fontsize=30.0)
         plt.xlabel("E-E$_f$ (eV)", fontsize=30.0)
         plt.xticks(fontsize=25)
         plt.yticks(fontsize=25)
         return plt
 
+    def plot_seebeck_temp(self, doping='all', output='average'):
+        """
+        Plot the Seebeck coefficient in function of temperature for different 
+        doping levels.
+
+        Args:
+            dopings: the default 'all' plots all the doping levels in the analyzer.
+                     Specify a list of doping levels if you want to plot only some.
+            output: with 'average' you get an average of the three directions
+                    with 'eigs' you get all the three directions.
+        Returns:
+            a matplotlib object
+        """
+
+        import matplotlib.pyplot as plt
+        if output == 'average':
+            sbk = self._bz.get_seebeck(output='average')
+        elif output == 'eigs':
+            sbk = self._bz.get_seebeck(output='eigs')
+            
+        plt.figure(figsize=(22,14))
+        tlist = np.sort(sbk['n'].keys())
+        doping = self._bz.doping['n'] if doping == 'all' else doping
+        for i,dt in enumerate(['n','p']):
+            plt.subplot(121+i)
+            for dop in doping:
+                d = self._bz.doping[dt].index(dop)
+                sbk_temp =[]
+                for temp in tlist:
+                    sbk_temp.append(sbk[dt][temp][d])
+                if output == 'average':
+                    plt.plot(tlist,sbk_temp,marker='s',label=str(dop)+' $cm^{-3}$')
+                elif output == 'eigs':
+                    for xyz in range(3):
+                        plt.plot(tlist,zip(*sbk_temp)[xyz],marker='s',
+                                 label=str(xyz)+' '+str(dop)+' $cm^{-3}$')
+            plt.title(dt+'-type',fontsize=20)
+            if i == 0:
+                plt.ylabel("Seebeck \n coefficient  ($\\mu$V/K)", fontsize=30.0)
+            plt.xlabel('Temperature (K)', fontsize=30.0)
+
+            p = 'lower right' if i == 0 else ''
+            plt.legend(loc=p,fontsize=15)
+            plt.grid()
+            plt.xticks(fontsize=25)
+            plt.yticks(fontsize=25)
+        
+        plt.tight_layout()
+
+        return plt
+
+    def plot_conductivity_temp(self, doping='all', output='average', relaxation_time=1e-14):
+        """
+        Plot the conductivity in function of temperature for different doping levels.
+
+        Args:
+            dopings: the default 'all' plots all the doping levels in the analyzer.
+                     Specify a list of doping levels if you want to plot only some.
+            output: with 'average' you get an average of the three directions
+                    with 'eigs' you get all the three directions.
+            relaxation_time: specify a constant relaxation time value
+        
+        Returns:
+            a matplotlib object
+        """
+        import matplotlib.pyplot as plt
+        import matplotlib.ticker as mtick
+        
+        if output == 'average':
+            cond = self._bz.get_conductivity(relaxation_time=relaxation_time,output='average')
+        elif output == 'eigs':
+            cond = self._bz.get_conductivity(relaxation_time=relaxation_time,output='eigs')
+            
+        plt.figure(figsize=(22,14))
+        tlist = np.sort(cond['n'].keys())
+        doping = self._bz.doping['n'] if doping == 'all' else doping
+        for i,dt in enumerate(['n','p']):
+            plt.subplot(121+i)
+            for dop in doping:
+                d = self._bz.doping[dt].index(dop)
+                cond_temp =[]
+                for temp in tlist:
+                    cond_temp.append(cond[dt][temp][d])
+                if output == 'average':
+                    plt.plot(tlist,cond_temp,marker='s',label=str(dop)+' $cm^{-3}$')
+                elif output == 'eigs':
+                    for xyz in range(3):
+                        plt.plot(tlist,zip(*cond_temp)[xyz],marker='s',
+                                 label=str(xyz)+' '+str(dop)+' $cm^{-3}$')
+            plt.title(dt+'-type',fontsize=20)
+            if i == 0:
+                plt.ylabel("conductivity $\sigma$ (1/($\\Omega$ m))", fontsize=30.0)
+            plt.xlabel('Temperature (K)', fontsize=30.0)
+
+            p = '' # 'lower right' if i == 0 else ''
+            plt.legend(loc=p,fontsize=15)
+            plt.grid()
+            plt.xticks(fontsize=25)
+            plt.yticks(fontsize=25)
+            plt.ticklabel_format(style='sci', axis='y', scilimits=(0,0))
+            
+        plt.tight_layout()
+
+        return plt
+
+    def plot_power_factor_temp(self, doping='all', output='average', relaxation_time=1e-14):
+        """
+        Plot the Power Factor in function of temperature for different doping levels.
+
+        Args:
+            dopings: the default 'all' plots all the doping levels in the analyzer.
+                     Specify a list of doping levels if you want to plot only some.
+            output: with 'average' you get an average of the three directions
+                    with 'eigs' you get all the three directions.
+            relaxation_time: specify a constant relaxation time value
+        
+        Returns:
+            a matplotlib object
+        """
+        
+        import matplotlib.pyplot as plt
+        if output == 'average':
+            pf = self._bz.get_power_factor(relaxation_time=relaxation_time,output='average')
+        elif output == 'eigs':
+            pf = self._bz.get_power_factor(relaxation_time=relaxation_time,output='eigs')
+            
+        plt.figure(figsize=(22,14))
+        tlist = np.sort(pf['n'].keys())
+        doping = self._bz.doping['n'] if doping == 'all' else doping
+        for i,dt in enumerate(['n','p']):
+            plt.subplot(121+i)
+            for dop in doping:
+                d = self._bz.doping[dt].index(dop)
+                pf_temp =[]
+                for temp in tlist:
+                    pf_temp.append(pf[dt][temp][d])
+                if output == 'average':
+                    plt.plot(tlist,pf_temp,marker='s',label=str(dop)+' $cm^{-3}$')
+                elif output == 'eigs':
+                    for xyz in range(3):
+                        plt.plot(tlist,zip(*pf_temp)[xyz],marker='s',
+                                 label=str(xyz)+' '+str(dop)+' $cm^{-3}$')
+            plt.title(dt+'-type',fontsize=20)
+            if i == 0:
+                plt.ylabel("Power Factor ($\\mu$W/(mK$^2$))", fontsize=30.0)
+            plt.xlabel('Temperature (K)', fontsize=30.0)
+
+            p = '' #'lower right' if i == 0 else ''
+            plt.legend(loc=p,fontsize=15)
+            plt.grid()
+            plt.xticks(fontsize=25)
+            plt.yticks(fontsize=25)
+            plt.ticklabel_format(style='sci', axis='y', scilimits=(0,0))
+            
+        plt.tight_layout()
+        return plt
+
+    def plot_zt_temp(self, doping='all', output='average', relaxation_time=1e-14):
+        """
+        Plot the figure of merit zT in function of temperature for different doping levels.
+
+        Args:
+            dopings: the default 'all' plots all the doping levels in the analyzer.
+                     Specify a list of doping levels if you want to plot only some.
+            output: with 'average' you get an average of the three directions
+                    with 'eigs' you get all the three directions.
+            relaxation_time: specify a constant relaxation time value
+        
+        Returns:
+            a matplotlib object
+        """
+        
+        import matplotlib.pyplot as plt
+        if output == 'average':
+            zt = self._bz.get_zt(relaxation_time=relaxation_time,output='average')
+        elif output == 'eigs':
+            zt = self._bz.get_zt(relaxation_time=relaxation_time,output='eigs')
+            
+        plt.figure(figsize=(22,14))
+        tlist = np.sort(zt['n'].keys())
+        doping = self._bz.doping['n'] if doping == 'all' else doping
+        for i,dt in enumerate(['n','p']):
+            plt.subplot(121+i)
+            for dop in doping:
+                d = self._bz.doping[dt].index(dop)
+                zt_temp =[]
+                for temp in tlist:
+                    zt_temp.append(zt[dt][temp][d])
+                if output == 'average':
+                    plt.plot(tlist,zt_temp,marker='s',label=str(dop)+' $cm^{-3}$')
+                elif output == 'eigs':
+                    for xyz in range(3):
+                        plt.plot(tlist,zip(*zt_temp)[xyz],marker='s',
+                                 label=str(xyz)+' '+str(dop)+' $cm^{-3}$')
+            plt.title(dt+'-type',fontsize=20)
+            if i == 0:
+                plt.ylabel("zT", fontsize=30.0)
+            plt.xlabel('Temperature (K)', fontsize=30.0)
+
+            p = '' #'lower right' if i == 0 else ''
+            plt.legend(loc=p,fontsize=15)
+            plt.grid()
+            plt.xticks(fontsize=25)
+            plt.yticks(fontsize=25)
+        
+        plt.tight_layout()
+        return plt
+    
+    def plot_eff_mass_temp(self, doping='all', output='average'):
+        """
+        Plot the average effective mass in function of temperature 
+        for different doping levels.
+
+        Args:
+            dopings: the default 'all' plots all the doping levels in the analyzer.
+                     Specify a list of doping levels if you want to plot only some.
+            output: with 'average' you get an average of the three directions
+                    with 'eigs' you get all the three directions.
+
+        Returns:
+            a matplotlib object
+        """
+        
+        import matplotlib.pyplot as plt
+        if output == 'average':
+            em = self._bz.get_average_eff_mass(output='average')
+        elif output == 'eigs':
+            em = self._bz.get_average_eff_mass(output='eigs')
+            
+        plt.figure(figsize=(22,14))
+        tlist = np.sort(em['n'].keys())
+        doping = self._bz.doping['n'] if doping == 'all' else doping
+        for i,dt in enumerate(['n','p']):
+            plt.subplot(121+i)
+            for dop in doping:
+                d = self._bz.doping[dt].index(dop)
+                em_temp =[]
+                for temp in tlist:
+                    em_temp.append(em[dt][temp][d])
+                if output == 'average':
+                    plt.plot(tlist,em_temp,marker='s',label=str(dop)+' $cm^{-3}$')
+                elif output == 'eigs':
+                    for xyz in range(3):
+                        plt.plot(tlist,zip(*em_temp)[xyz],marker='s',
+                                 label=str(xyz)+' '+str(dop)+' $cm^{-3}$')
+            plt.title(dt+'-type',fontsize=20)
+            if i == 0:
+                plt.ylabel("Effective mass (m$_e$)", fontsize=30.0)
+            plt.xlabel('Temperature (K)', fontsize=30.0)
+
+            p = '' #'lower right' if i == 0 else ''
+            plt.legend(loc=p,fontsize=15)
+            plt.grid()
+            plt.xticks(fontsize=25)
+            plt.yticks(fontsize=25)
+            
+        plt.tight_layout()
+        return plt
+
+    
+    def plot_seebeck_dop(self, temps='all', output='average'):
+        """
+        Plot the Seebeck in function of doping levels for different temperatures.
+
+        Args:
+            temps: the default 'all' plots all the temperatures in the analyzer.
+                   Specify a list of temperatures if you want to plot only some.
+            output: with 'average' you get an average of the three directions
+                    with 'eigs' you get all the three directions.
+
+        Returns:
+            a matplotlib object
+        """        
+
+        import matplotlib.pyplot as plt
+        if output == 'average':
+            sbk = self._bz.get_seebeck(output='average')
+        elif output == 'eigs':
+            sbk = self._bz.get_seebeck(output='eigs')
+        
+        tlist = np.sort(sbk['n'].keys()) if temps=='all' else temps
+        plt.figure(figsize=(22,14))
+        for i,dt in enumerate(['n','p']):
+            plt.subplot(121+i)
+            for temp in tlist:
+                if output == 'eigs':
+                    for xyz in range(3):
+                        plt.semilogx(self._bz.doping[dt],zip(*sbk[dt][temp])[xyz],
+                                     marker='s',label=str(xyz)+' '+str(temp)+' K')
+                elif output == 'average':
+                    plt.semilogx(self._bz.doping[dt],sbk[dt][temp],
+                                 marker='s',label=str(temp)+' K')
+            plt.title(dt+'-type',fontsize=20)
+            if i == 0:
+                plt.ylabel("Seebeck coefficient ($\\mu$V/K)", fontsize=30.0)
+            plt.xlabel('Doping concentration (cm$^{-3}$)', fontsize=30.0)
+
+            p = 'lower right' if i == 0 else ''
+            plt.legend(loc=p,fontsize=15)
+            plt.grid()
+            plt.xticks(fontsize=25)
+            plt.yticks(fontsize=25)
+        
+        plt.tight_layout()
+        
+        return plt
+        
+
+    def plot_conductivity_dop(self, temps='all', output='average', relaxation_time=1e-14):
+        """
+        Plot the conductivity in function of doping levels for different temperatures.
+
+        Args:
+            temps: the default 'all' plots all the temperatures in the analyzer.
+                   Specify a list of temperatures if you want to plot only some.
+            output: with 'average' you get an average of the three directions
+                    with 'eigs' you get all the three directions.
+            relaxation_time: specify a constant relaxation time value
+        
+        Returns:
+            a matplotlib object
+        """        
+        import matplotlib.pyplot as plt
+        if output == 'average':
+            cond = self._bz.get_conductivity(relaxation_time=relaxation_time,output='average')
+        elif output == 'eigs':
+            cond = self._bz.get_conductivity(relaxation_time=relaxation_time,output='eigs')
+        
+        tlist = np.sort(cond['n'].keys()) if temps=='all' else temps
+        plt.figure(figsize=(22,14))
+        for i,dt in enumerate(['n','p']):
+            plt.subplot(121+i)
+            for temp in tlist:
+                if output == 'eigs':
+                    for xyz in range(3):
+                        plt.semilogx(self._bz.doping[dt],zip(*cond[dt][temp])[xyz],
+                                     marker='s',label=str(xyz)+' '+str(temp)+' K')
+                elif output == 'average':
+                    plt.semilogx(self._bz.doping[dt],cond[dt][temp],
+                                 marker='s',label=str(temp)+' K')
+            plt.title(dt+'-type',fontsize=20)
+            if i == 0:
+                plt.ylabel("conductivity $\sigma$ (1/($\\Omega$ m))", fontsize=30.0)
+            plt.xlabel('Doping concentration ($cm^{-3}$)', fontsize=30.0)
+            plt.ticklabel_format(style='sci', axis='y', scilimits=(0,0))
+            plt.legend(fontsize=15)
+            plt.grid()
+            plt.xticks(fontsize=25)
+            plt.yticks(fontsize=25)
+        
+        plt.tight_layout()
+        
+        return plt
+
+    def plot_power_factor_dop(self, temps='all', output='average', relaxation_time=1e-14):
+        """
+        Plot the Power Factor in function of doping levels for different temperatures.
+
+        Args:
+            temps: the default 'all' plots all the temperatures in the analyzer.
+                   Specify a list of temperatures if you want to plot only some.
+            output: with 'average' you get an average of the three directions
+                    with 'eigs' you get all the three directions.
+            relaxation_time: specify a constant relaxation time value
+        
+        Returns:
+            a matplotlib object
+        """        
+        import matplotlib.pyplot as plt
+        if output == 'average':
+            pf = self._bz.get_power_factor(relaxation_time=relaxation_time,output='average')
+        elif output == 'eigs':
+            pf = self._bz.get_power_factor(relaxation_time=relaxation_time,output='eigs')
+        
+        tlist = np.sort(pf['n'].keys()) if temps=='all' else temps
+        plt.figure(figsize=(22,14))
+        for i,dt in enumerate(['n','p']):
+            plt.subplot(121+i)
+            for temp in tlist:
+                if output == 'eigs':
+                    for xyz in range(3):
+                        plt.semilogx(self._bz.doping[dt],zip(*pf[dt][temp])[xyz],
+                                     marker='s',label=str(xyz)+' '+str(temp)+' K')
+                elif output == 'average':
+                    plt.semilogx(self._bz.doping[dt],pf[dt][temp],
+                                 marker='s',label=str(temp)+' K')
+            plt.title(dt+'-type',fontsize=20)
+            if i == 0:
+                plt.ylabel("Power Factor  ($\\mu$W/(mK$^2$))", fontsize=30.0)
+            plt.xlabel('Doping concentration ($cm^{-3}$)', fontsize=30.0)
+            plt.ticklabel_format(style='sci', axis='y', scilimits=(0,0))
+            p = '' #'lower right' if i == 0 else ''
+            plt.legend(loc=p,fontsize=15)
+            plt.grid()
+            plt.xticks(fontsize=25)
+            plt.yticks(fontsize=25)
+        
+        plt.tight_layout()
+        
+        return plt
+
+
+    def plot_zt_dop(self, temps='all', output='average', relaxation_time=1e-14):
+        """
+        Plot the figure of merit zT in function of doping levels for different temperatures.
+
+        Args:
+            temps: the default 'all' plots all the temperatures in the analyzer.
+                   Specify a list of temperatures if you want to plot only some.
+            output: with 'average' you get an average of the three directions
+                    with 'eigs' you get all the three directions.
+            relaxation_time: specify a constant relaxation time value
+        
+        Returns:
+            a matplotlib object
+        """        
+        import matplotlib.pyplot as plt
+        if output == 'average':
+            zt = self._bz.get_zt(relaxation_time=relaxation_time,output='average')
+        elif output == 'eigs':
+            zt = self._bz.get_zt(relaxation_time=relaxation_time,output='eigs')
+        
+        tlist = np.sort(zt['n'].keys()) if temps=='all' else temps
+        plt.figure(figsize=(22,14))
+        for i,dt in enumerate(['n','p']):
+            plt.subplot(121+i)
+            for temp in tlist:
+                if output == 'eigs':
+                    for xyz in range(3):
+                        plt.semilogx(self._bz.doping[dt],zip(*zt[dt][temp])[xyz],
+                                     marker='s',label=str(xyz)+' '+str(temp)+' K')
+                elif output == 'average':
+                    plt.semilogx(self._bz.doping[dt],zt[dt][temp],
+                                 marker='s',label=str(temp)+' K')
+            plt.title(dt+'-type',fontsize=20)
+            if i == 0:
+                plt.ylabel("zT", fontsize=30.0)
+            plt.xlabel('Doping concentration ($cm^{-3}$)', fontsize=30.0)
+
+            p = 'lower right' if i == 0 else ''
+            plt.legend(loc=p,fontsize=15)
+            plt.grid()
+            plt.xticks(fontsize=25)
+            plt.yticks(fontsize=25)
+        
+        plt.tight_layout()
+        
+        return plt
+
+    def plot_eff_mass_dop(self, temps='all', output='average'):
+        """
+        Plot the average effective mass in function of doping levels 
+        for different temperatures.
+
+        Args:
+            temps: the default 'all' plots all the temperatures in the analyzer.
+                   Specify a list of temperatures if you want to plot only some.
+            output: with 'average' you get an average of the three directions
+                    with 'eigs' you get all the three directions.
+            relaxation_time: specify a constant relaxation time value
+        
+        Returns:
+            a matplotlib object
+        """
+        
+        import matplotlib.pyplot as plt
+        if output == 'average':
+            em = self._bz.get_average_eff_mass(output='average')
+        elif output == 'eigs':
+            em = self._bz.get_average_eff_mass(output='eigs')
+        
+        tlist = np.sort(em['n'].keys()) if temps=='all' else temps
+        plt.figure(figsize=(22,14))
+        for i,dt in enumerate(['n','p']):
+            plt.subplot(121+i)
+            for temp in tlist:
+                if output == 'eigs':
+                    for xyz in range(3):
+                        plt.semilogx(self._bz.doping[dt],zip(*em[dt][temp])[xyz],
+                                     marker='s',label=str(xyz)+' '+str(temp)+' K')
+                elif output == 'average':
+                    plt.semilogx(self._bz.doping[dt],em[dt][temp],
+                                 marker='s',label=str(temp)+' K')
+            plt.title(dt+'-type',fontsize=20)
+            if i == 0:
+                plt.ylabel("Effective mass (m$_e$)", fontsize=30.0)
+            plt.xlabel('Doping concentration ($cm^{-3}$)', fontsize=30.0)
+
+            p = 'lower right' if i == 0 else ''
+            plt.legend(loc=p,fontsize=15)
+            plt.grid()
+            plt.xticks(fontsize=25)
+            plt.yticks(fontsize=25)
+        
+        plt.tight_layout()
+        
+        return plt
+
+
     def plot_dos(self, sigma=0.05):
         """
         plot dos
 
         Args:
             sigma: a smearing
 
@@ -2999,15 +3511,16 @@
 
     ax.set_aspect('equal')
     ax.axis("off")
 
     return fig
 
 
-def plot_ellipsoid(hessian, center, lattice=None, rescale=1.0, ax=None, coords_are_cartesian=False, **kwargs):
+def plot_ellipsoid(hessian, center, lattice=None, rescale=1.0, ax=None, 
+                   coords_are_cartesian=False, arrows = False, **kwargs):
     """
     Plots a 3D ellipsoid rappresenting the Hessian matrix in input.
     Useful to get a graphical visualization of the effective mass
     of a band in a single k-point.
     
     Args:
         hessian: the Hessian matrix
@@ -3056,9 +3569,18 @@
     for i in range(len(x)):
         for j in range(len(x)):
             [x[i, j], y[i, j], z[i, j]] = np.dot([x[i, j], y[i, j], z[i, j]], rotation)*rescale + center
 
     # add the ellipsoid to the current axes
     ax, fig, plt = get_ax3d_fig_plt(ax)
     ax.plot_wireframe(x, y, z,  **kwargs)
+    
+    if arrows:
+        color=('b','g','r')
+        em=np.zeros((3,3))
+        for i in range(3):
+            em[i,:] = rotation[i,:]/np.linalg.norm(rotation[i,:])
+        for i in range(3):
+            ax.quiver3D(center[0],center[1],center[2],em[i,0],em[i,1],em[i,2],pivot='tail',
+                        arrow_length_ratio=0.2,length=radii[i]*rescale,color=color[i])
 
     return fig, ax
```

### Comparing `pymatgen-4.7.6/pymatgen/entries/compatibility.py` & `pymatgen-4.7.7/pymatgen/entries/compatibility.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/entries/computed_entries.py` & `pymatgen-4.7.7/pymatgen/entries/computed_entries.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/entries/entry_tools.py` & `pymatgen-4.7.7/pymatgen/entries/entry_tools.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/entries/exp_entries.py` & `pymatgen-4.7.7/pymatgen/entries/exp_entries.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/entries/MITCompatibility.yaml` & `pymatgen-4.7.7/pymatgen/entries/MITCompatibility.yaml`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/entries/MPCompatibility.yaml` & `pymatgen-4.7.7/pymatgen/entries/MPCompatibility.yaml`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/entries/post_processors_abc.py` & `pymatgen-4.7.7/pymatgen/entries/post_processors_abc.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/abinit/abiinspect.py` & `pymatgen-4.7.7/pymatgen/io/abinit/abiinspect.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/abinit/abiobjects.py` & `pymatgen-4.7.7/pymatgen/io/abinit/abiobjects.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/abinit/abitimer.py` & `pymatgen-4.7.7/pymatgen/io/abinit/abitimer.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/abinit/calculations.py` & `pymatgen-4.7.7/pymatgen/io/abinit/calculations.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/abinit/db.py` & `pymatgen-4.7.7/pymatgen/io/abinit/db.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/abinit/events.py` & `pymatgen-4.7.7/pymatgen/io/abinit/events.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/abinit/flows.py` & `pymatgen-4.7.7/pymatgen/io/abinit/flows.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/abinit/helpers.py` & `pymatgen-4.7.7/pymatgen/io/abinit/helpers.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/abinit/launcher.py` & `pymatgen-4.7.7/pymatgen/io/abinit/launcher.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/abinit/netcdf.py` & `pymatgen-4.7.7/pymatgen/io/abinit/netcdf.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/abinit/nodes.py` & `pymatgen-4.7.7/pymatgen/io/abinit/nodes.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/abinit/pseudos.py` & `pymatgen-4.7.7/pymatgen/io/abinit/pseudos.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/abinit/qadapters.py` & `pymatgen-4.7.7/pymatgen/io/abinit/qadapters.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/abinit/qjobs.py` & `pymatgen-4.7.7/pymatgen/io/abinit/qjobs.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/abinit/qutils.py` & `pymatgen-4.7.7/pymatgen/io/abinit/qutils.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/abinit/scheduler_error_handlers.py` & `pymatgen-4.7.7/pymatgen/io/abinit/scheduler_error_handlers.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/abinit/scheduler_error_parsers.py` & `pymatgen-4.7.7/pymatgen/io/abinit/scheduler_error_parsers.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/abinit/tasks.py` & `pymatgen-4.7.7/pymatgen/io/abinit/tasks.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/abinit/utils.py` & `pymatgen-4.7.7/pymatgen/io/abinit/utils.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/abinit/works.py` & `pymatgen-4.7.7/pymatgen/io/abinit/works.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/abinit/wrappers.py` & `pymatgen-4.7.7/pymatgen/io/abinit/wrappers.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/adf.py` & `pymatgen-4.7.7/pymatgen/io/adf.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/aiida.py` & `pymatgen-4.7.7/pymatgen/io/aiida.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/ase.py` & `pymatgen-4.7.7/pymatgen/io/ase.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/babel.py` & `pymatgen-4.7.7/pymatgen/io/babel.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/cif.py` & `pymatgen-4.7.7/pymatgen/matproj/rest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,880 +1,956 @@
 # coding: utf-8
 # Copyright (c) Pymatgen Development Team.
 # Distributed under the terms of the MIT License.
 
-from __future__ import division, unicode_literals, print_function
+from __future__ import division, unicode_literals
 
-import math
+import itertools
+import json
 import re
-import os
-import textwrap
 import warnings
-from collections import OrderedDict, deque
 
-import six
-from six.moves import zip, cStringIO
+from monty.json import MontyDecoder, MontyEncoder
+from six import string_types
+
+from pymatgen import SETTINGS
 
-import numpy as np
-from functools import partial
-try:
-    from inspect import getfullargspec as getargspec
-except ImportError:
-    from inspect import getargspec
-from itertools import groupby
-from pymatgen.core.periodic_table import Element, Specie, get_el_sp, DummySpecie
-from monty.io import zopen
-from pymatgen.util.coord_utils import in_coord_list_pbc, pbc_diff, \
-    find_in_coord_list_pbc
-from monty.string import remove_non_ascii
-from pymatgen.core.lattice import Lattice
-from pymatgen.core.structure import Structure
 from pymatgen.core.composition import Composition
-from pymatgen.core.operations import SymmOp
-from pymatgen.symmetry.groups import SpaceGroup, SYMM_DATA
-from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
+from pymatgen.core.periodic_table import Element
+from pymatgen.core.structure import Structure
+
+from pymatgen.entries.computed_entries import ComputedEntry, \
+    ComputedStructureEntry
+from pymatgen.entries.exp_entries import ExpEntry
+
 
 """
-Wrapper classes for Cif input and output from Structures.
+This module provides classes to interface with the Materials Project REST
+API v2 to enable the creation of data structures and pymatgen objects using
+Materials Project data.
+
+To make use of the Materials API, you need to be a registered user of the
+Materials Project, and obtain an API key by going to your dashboard at
+https://www.materialsproject.org/dashboard.
 """
 
-__author__ = "Shyue Ping Ong, Will Richards"
-__copyright__ = "Copyright 2011, The Materials Project"
-__version__ = "3.0"
+__author__ = "Shyue Ping Ong, Shreyas Cholia"
+__credits__ = "Anubhav Jain"
+__copyright__ = "Copyright 2012, The Materials Project"
+__version__ = "1.0"
 __maintainer__ = "Shyue Ping Ong"
 __email__ = "shyuep@gmail.com"
-__status__ = "Production"
-__date__ = "Sep 23, 2011"
+__date__ = "Feb 22, 2013"
+
 
-sub_spgrp = partial(re.sub, r"[\s_]", "")
+class MPRester(object):
+    """
+    A class to conveniently interface with the Materials Project REST
+    interface. The recommended way to use MPRester is with the "with" context
+    manager to ensure that sessions are properly closed after usage::
 
-space_groups = {sub_spgrp(k): k
-                for k in SYMM_DATA['space_group_encoding'].keys()}
+        with MPRester("API_KEY") as m:
+            do_something
 
-space_groups.update({sub_spgrp(k): k
-                     for k in SYMM_DATA['space_group_encoding'].keys()})
-
-_COD_DATA = None
-
-
-def _get_cod_data():
-    global _COD_DATA
-    if _COD_DATA is None:
-        import pymatgen
-        with open(os.path.join(pymatgen.symmetry.__path__[0],
-                               "symm_ops.json")) \
-                as f:
-            import json
-            _COD_DATA = json.load(f)
-
-    return _COD_DATA
-
-
-class CifBlock(object):
-    maxlen = 70  # not quite 80 so we can deal with semicolons and things
-
-    def __init__(self, data, loops, header):
-        """
-        Object for storing cif data. All data is stored in a single dictionary.
-        Data inside loops are stored in lists in the data dictionary, and
-        information on which keys are grouped together are stored in the loops
-        attribute.
-
-        Args:
-            data: dict or OrderedDict of data to go into the cif. Values should
-                    be convertible to string, or lists of these if the key is
-                    in a loop
-            loops: list of lists of keys, grouped by which loop they should
-                    appear in
-            header: name of the block (appears after the data_ on the first
-                line)
-        """
-        self.loops = loops
-        self.data = data
-        # AJ says: CIF Block names cannot be more than 75 characters or you
-        # get an Exception
-        self.header = header[:74]
-
-    def __eq__(self, other):
-        return self.loops == other.loops \
-               and self.data == other.data \
-               and self.header == other.header
-
-    def __getitem__(self, key):
-        return self.data[key]
-
-    def __str__(self):
-        """
-        Returns the cif string for the data block
-        """
-        s = ["data_{}".format(self.header)]
-        keys = self.data.keys()
-        written = []
-        for k in keys:
-            if k in written:
-                continue
-            for l in self.loops:
-                # search for a corresponding loop
-                if k in l:
-                    s.append(self._loop_to_string(l))
-                    written.extend(l)
-                    break
-            if k not in written:
-                # k didn't belong to a loop
-                v = self._format_field(self.data[k])
-                if len(k) + len(v) + 3 < self.maxlen:
-                    s.append("{}   {}".format(k, v))
-                else:
-                    s.extend([k, v])
-        return "\n".join(s)
+    MPRester uses the "requests" package, which provides for HTTP connection
+    pooling. All connections are made via https for security.
+
+    .. note::
+
+        The Materials Project recently switched to using string ids with a
+        "mp-" prefix for greater flexibility going forward. The MPRester
+        should still work as intended if you provide the proper string ids.
+
+    Args:
+        api_key (str): A String API key for accessing the MaterialsProject
+            REST interface. Please obtain your API key at
+            https://www.materialsproject.org/dashboard. If this is None,
+            the code will check if there is a "PMG_MAPI_KEY" setting.
+            If so, it will use that environment variable. This makes
+            easier for heavy users to simply add this environment variable to
+            their setups and MPRester can then be called without any arguments.
+        endpoint (str): Url of endpoint to access the MaterialsProject REST
+            interface. Defaults to the standard Materials Project REST
+            address, but can be changed to other urls implementing a similar
+            interface.
+    """
+
+    supported_properties = ("energy", "energy_per_atom", "volume",
+                            "formation_energy_per_atom", "nsites",
+                            "unit_cell_formula", "pretty_formula",
+                            "is_hubbard", "elements", "nelements",
+                            "e_above_hull", "hubbards", "is_compatible",
+                            "spacegroup", "task_ids", "band_gap", "density",
+                            "icsd_id", "icsd_ids", "cif", "total_magnetization",
+                            "material_id", "oxide_type", "tags", "elasticity")
+
+    supported_task_properties = ("energy", "energy_per_atom", "volume",
+                                 "formation_energy_per_atom", "nsites",
+                                 "unit_cell_formula", "pretty_formula",
+                                 "is_hubbard",
+                                 "elements", "nelements", "e_above_hull",
+                                 "hubbards",
+                                 "is_compatible", "spacegroup",
+                                 "band_gap", "density", "icsd_id", "cif")
+
+    def __init__(self, api_key=None,
+                 endpoint="https://www.materialsproject.org/rest/v2"):
+        if api_key is not None:
+            self.api_key = api_key
+        else:
+            self.api_key = SETTINGS.get("PMG_MAPI_KEY", "")
+        self.preamble = endpoint
+        import requests
+        try:
+            from pybtex import __version__
+        except ImportError:
+            warnings.warn("If you query for structure data encoded using MP's "
+                          "Structure Notation Language (SNL) format and you use "
+                          "`mp_decode=True` (the default) for MPRester queries, "
+                          "you should install dependencies via "
+                          "`pip install pymatgen[matproj.snl]`.")
+        self.session = requests.Session()
+        self.session.headers = {"x-api-key": self.api_key}
+
+    def __enter__(self):
+        """
+        Support for "with" context.
+        """
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        """
+        Support for "with" context.
+        """
+        self.session.close()
 
-    def _loop_to_string(self, loop):
-        s = "loop_"
-        for l in loop:
-            s += '\n ' + l
-        for fields in zip(*[self.data[k] for k in loop]):
-            line = "\n"
-            for val in map(self._format_field, fields):
-                if val[0] == ";":
-                    s += line + "\n" + val
-                    line = "\n"
-                elif len(line) + len(val) + 2 < self.maxlen:
-                    line += "  " + val
+    def _make_request(self, sub_url, payload=None, method="GET",
+                      mp_decode=True):
+        response = None
+        url = self.preamble + sub_url
+        try:
+            if method == "POST":
+                response = self.session.post(url, data=payload, verify=True)
+            else:
+                response = self.session.get(url, params=payload, verify=True)
+            if response.status_code in [200, 400]:
+                if mp_decode:
+                    data = json.loads(response.text, cls=MontyDecoder)
                 else:
-                    s += line
-                    line = '\n  ' + val
-            s += line
-        return s
-
-    def _format_field(self, v):
-        v = v.__str__().strip()
-        if len(v) > self.maxlen:
-            return ';\n' + textwrap.fill(v, self.maxlen) + '\n;'
-        # add quotes if necessary
-        if v == '':
-            return '""'
-        if (" " in v or v[0] == "_") \
-                and not (v[0] == "'" and v[-1] == "'") \
-                and not (v[0] == '"' and v[-1] == '"'):
-            if "'" in v:
-                q = '"'
+                    data = json.loads(response.text)
+                if data["valid_response"]:
+                    if data.get("warning"):
+                        warnings.warn(data["warning"])
+                    return data["response"]
+                else:
+                    raise MPRestError(data["error"])
+
+            raise MPRestError("REST query returned with error status code {}"
+                              .format(response.status_code))
+
+        except Exception as ex:
+            msg = "{}. Content: {}".format(str(ex), response.content)\
+                if hasattr(response, "content") else str(ex)
+            raise MPRestError(msg)
+
+    def get_materials_id_from_task_id(self, task_id):
+        """
+        Returns a new MP materials id from a task id (which can be
+        equivalent to an old materials id)
+
+        Args:
+            task_id (str): A task id.
+
+        Returns:
+            materials_id (str)
+        """
+        return self._make_request("/materials/mid_from_tid/%s" % task_id)
+
+    def get_materials_id_references(self, material_id):
+        """
+        Returns all references for a materials id.
+
+        Args:
+            material_id (str): A material id.
+
+        Returns:
+            BibTeX (str)
+        """
+        return self._make_request("/materials/%s/refs" % material_id)
+
+    def get_data(self, chemsys_formula_id, data_type="vasp", prop=""):
+        """
+        Flexible method to get any data using the Materials Project REST
+        interface. Generally used by other methods for more specific queries.
+
+        Format of REST return is *always* a list of dict (regardless of the
+        number of pieces of data returned. The general format is as follows:
+
+        [{"material_id": material_id, "property_name" : value}, ...]
+
+        Args:
+            chemsys_formula_id (str): A chemical system (e.g., Li-Fe-O),
+                or formula (e.g., Fe2O3) or materials_id (e.g., mp-1234).
+            data_type (str): Type of data to return. Currently can either be
+                "vasp" or "exp".
+            prop (str): Property to be obtained. Should be one of the
+                MPRester.supported_task_properties. Leave as empty string for a
+                general list of useful properties.
+        """
+        sub_url = "/materials/%s/%s" % (chemsys_formula_id, data_type)
+        if prop:
+            sub_url += "/" + prop
+        return self._make_request(sub_url)
+
+    def get_task_data(self, chemsys_formula_id, prop=""):
+        """
+        Flexible method to get any data using the Materials Project REST
+        interface. Generally used by other methods for more specific queries.
+        Unlike the :func:`get_data`_, this method queries the task collection
+        for specific run information.
+
+        Format of REST return is *always* a list of dict (regardless of the
+        number of pieces of data returned. The general format is as follows:
+
+        [{"material_id": material_id, "property_name" : value}, ...]
+
+        Args:
+            chemsys_formula_id (str): A chemical system (e.g., Li-Fe-O),
+                or formula (e.g., Fe2O3) or materials_id (e.g., mp-1234).
+            prop (str): Property to be obtained. Should be one of the
+                MPRester.supported_properties. Leave as empty string for a
+                general list of useful properties.
+        """
+        sub_url = "/tasks/%s" % chemsys_formula_id
+        if prop:
+            sub_url += "/" + prop
+        return self._make_request(sub_url)
+
+    def get_structures(self, chemsys_formula_id, final=True):
+        """
+        Get a list of Structures corresponding to a chemical system, formula,
+        or materials_id.
+
+        Args:
+            chemsys_formula_id (str): A chemical system (e.g., Li-Fe-O),
+                or formula (e.g., Fe2O3) or materials_id (e.g., mp-1234).
+            final (bool): Whether to get the final structure, or the initial
+                (pre-relaxation) structure. Defaults to True.
+
+        Returns:
+            List of Structure objects.
+        """
+        prop = "final_structure" if final else "initial_structure"
+        data = self.get_data(chemsys_formula_id, prop=prop)
+        return [d[prop] for d in data]
+
+    def find_structure(self, filename_or_structure):
+        """
+        Finds matching structures on the Materials Project site.
+
+        Args:
+            filename_or_structure: filename or Structure object
+
+        Returns:
+            A list of matching structures.
+
+        Raises:
+            MPRestError
+        """
+        try:
+            if isinstance(filename_or_structure, string_types):
+                s = Structure.from_file(filename_or_structure)
+            elif isinstance(filename_or_structure, Structure):
+                s = filename_or_structure
             else:
-                q = "'"
-            v = q + v + q
-        return v
-
-    @classmethod
-    def _process_string(cls, string):
-        # remove comments
-        string = re.sub(r"(\s|^)#.*$", "", string, flags=re.MULTILINE)
-        # remove empty lines
-        string = re.sub(r"^\s*\n", "", string, flags=re.MULTILINE)
-        # remove non_ascii
-        string = remove_non_ascii(string)
-
-        # since line breaks in .cif files are mostly meaningless,
-        # break up into a stream of tokens to parse, rejoining multiline
-        # strings (between semicolons)
-        q = deque()
-        multiline = False
-        ml = []
-        # this regex splits on spaces, except when in quotes.
-        # starting quotes must not be preceded by non-whitespace
-        # (these get eaten by the first expression)
-        # ending quotes must not be followed by non-whitespace
-        p = re.compile(r'''([^'"\s][\S]*)|'(.*?)'(?!\S)|"(.*?)"(?!\S)''')
-        for l in string.splitlines():
-            if multiline:
-                if l.startswith(";"):
-                    multiline = False
-                    q.append(('', '', '', ' '.join(ml)))
-                    ml = []
-                    l = l[1:].strip()
+                raise MPRestError("Provide filename or Structure object.")
+            payload = {'structure': json.dumps(s.as_dict(), cls=MontyEncoder)}
+            response = self.session.post(
+                '{}/find_structure'.format(self.preamble), data=payload
+            )
+            if response.status_code in [200, 400]:
+                resp = json.loads(response.text, cls=MontyDecoder)
+                if resp['valid_response']:
+                    return resp['response']
                 else:
-                    ml.append(l)
-                    continue
-            if l.startswith(";"):
-                multiline = True
-                ml.append(l[1:].strip())
+                    raise MPRestError(resp["error"])
+            raise MPRestError("REST error with status code {} and error {}"
+                              .format(response.status_code, response.text))
+        except Exception as ex:
+            raise MPRestError(str(ex))
+
+    def get_entries(self, chemsys_formula_id_criteria, compatible_only=True,
+                    inc_structure=None, property_data=None):
+        """
+        Get a list of ComputedEntries or ComputedStructureEntries corresponding
+        to a chemical system, formula, or materials_id or full criteria.
+
+        Args:
+            chemsys_formula_id_criteria (str/dict): A chemical system
+                (e.g., Li-Fe-O), or formula (e.g., Fe2O3) or materials_id
+                (e.g., mp-1234) or full Mongo-style dict criteria.
+            compatible_only (bool): Whether to return only "compatible"
+                entries. Compatible entries are entries that have been
+                processed using the MaterialsProjectCompatibility class,
+                which performs adjustments to allow mixing of GGA and GGA+U
+                calculations for more accurate phase diagrams and reaction
+                energies.
+            inc_structure (str): If None, entries returned are
+                ComputedEntries. If inc_structure="final",
+                ComputedStructureEntries with final structures are returned.
+                Otherwise, ComputedStructureEntries with initial structures
+                are returned.
+            property_data (list): Specify additional properties to include in
+                entry.data. If None, no data. Should be a subset of
+                supported_properties.
+
+        Returns:
+            List of ComputedEntry or ComputedStructureEntry objects.
+        """
+        # TODO: This is a very hackish way of doing this. It should be fixed
+        # on the REST end.
+        params = ["run_type", "is_hubbard", "pseudo_potential", "hubbards",
+                  "potcar_symbols"]
+        if compatible_only:
+            props = ["energy", "unit_cell_formula", "task_id"] + params
+            if property_data:
+                props += property_data
+            if inc_structure:
+                if inc_structure == "final":
+                    props.append("structure")
+                else:
+                    props.append("initial_structure")
+
+            if not isinstance(chemsys_formula_id_criteria, dict):
+                criteria = MPRester.parse_criteria(chemsys_formula_id_criteria)
             else:
-                for s in p.findall(l):
-                    # s is tuple. location of the data in the tuple
-                    # depends on whether it was quoted in the input
-                    q.append(s)
-        return q
-
-    @classmethod
-    def from_string(cls, string):
-        q = cls._process_string(string)
-        header = q.popleft()[0][5:]
-        data = OrderedDict()
-        loops = []
-        while q:
-            s = q.popleft()
-            # cif keys aren't in quotes, so show up in s[0]
-            if s[0] == "_eof":
-                break
-            if s[0].startswith("_"):
-                data[s[0]] = "".join(q.popleft())
-            elif s[0].startswith("loop_"):
-                columns = []
-                items = []
-                while q:
-                    s = q[0]
-                    if s[0].startswith("loop_") or not s[0].startswith("_"):
-                        break
-                    columns.append("".join(q.popleft()))
-                    data[columns[-1]] = []
-                while q:
-                    s = q[0]
-                    if s[0].startswith("loop_") or s[0].startswith("_"):
-                        break
-                    items.append("".join(q.popleft()))
-                n = len(items) // len(columns)
-                assert len(items) % n == 0
-                loops.append(columns)
-                for k, v in zip(columns * n, items):
-                    data[k].append(v.strip())
-            elif "".join(s).strip() != "":
-                warnings.warn("Possible error in cif format"
-                              " error at {}".format("".join(s).strip()))
-        return cls(data, loops, header)
+                criteria = chemsys_formula_id_criteria
 
+            data = self.query(criteria, props)
 
-class CifFile(object):
-    """
-    Reads and parses CifBlocks from a .cif file
-    """
+            entries = []
+            for d in data:
+                d["potcar_symbols"] = [
+                    "%s %s" % (d["pseudo_potential"]["functional"], l)
+                    for l in d["pseudo_potential"]["labels"]]
+                data = {k: d[k] for k in property_data} if property_data else None
+                if not inc_structure:
+                    e = ComputedEntry(d["unit_cell_formula"], d["energy"],
+                                      parameters={k: d[k] for k in params},
+                                      data=data,
+                                      entry_id=d["task_id"])
+
+                else:
+                    s = d["structure"] if inc_structure == "final" else d[
+                        "initial_structure"]
+                    e = ComputedStructureEntry(
+                        s, d["energy"],
+                        parameters={k: d[k] for k in params},
+                        data=data,
+                        entry_id=d["task_id"])
+                entries.append(e)
+            from pymatgen.entries.compatibility import \
+                MaterialsProjectCompatibility
+            entries = MaterialsProjectCompatibility().process_entries(entries)
+        else:
+            entries = []
+            for d in self.get_data(chemsys_formula_id_criteria,
+                                   prop="task_ids"):
+                for i in d["task_ids"]:
+                    e = self.get_task_data(i, prop="entry")
+                    e = e[0]["entry"]
+                    if inc_structure:
+                        s = self.get_task_data(i,
+                                               prop="structure")[0]["structure"]
+                        e = ComputedStructureEntry(
+                            s, e.energy, e.correction, e.parameters, e.data,
+                            e.entry_id)
+                    entries.append(e)
+
+        return entries
 
-    def __init__(self, data, orig_string=None, comment=None):
+    def get_structure_by_material_id(self, material_id, final=True):
         """
+        Get a Structure corresponding to a material_id.
+
         Args:
-            data (OrderedDict): Of CifBlock objects.å
-            orig_string (str): The original cif string.
-            comment (str): Comment string.
-        """
-        self.data = data
-        self.orig_string = orig_string
-        self.comment = comment or "# generated using pymatgen"
-
-    def __str__(self):
-        s = ["%s" % v for v in self.data.values()]
-        return self.comment + "\n" + "\n".join(s) + "\n"
-
-    @classmethod
-    def from_string(cls, string):
-        d = OrderedDict()
-        for x in re.split(r"^\s*data_", "x\n" + string,
-                          flags=re.MULTILINE | re.DOTALL)[1:]:
-
-            # Skip over Cif block that contains powder diffraction data.
-            # Some elements in this block were missing from CIF files in Springer materials/Pauling file DBs.
-            # This block anyway does not contain any structure information, and CifParser was also not parsing it.
-            if 'powder_pattern' in re.split(r"\n", x, 1)[0]:
-                continue
-            c = CifBlock.from_string("data_" + x)
-            d[c.header] = c
-        return cls(d, string)
-
-    @classmethod
-    def from_file(cls, filename):
-        with zopen(filename, "rt") as f:
-            return cls.from_string(f.read())
+            material_id (str): Materials Project material_id (a string,
+                e.g., mp-1234).
+            final (bool): Whether to get the final structure, or the initial
+                (pre-relaxation) structure. Defaults to True.
 
+        Returns:
+            Structure object.
+        """
+        prop = "final_structure" if final else "initial_structure"
+        data = self.get_data(material_id, prop=prop)
+        return data[0][prop]
 
-class CifParser(object):
-    """
-    Parses a cif file
+    def get_entry_by_material_id(self, material_id, compatible_only=True,
+                                 inc_structure=None, property_data=None):
+        """
+        Get a ComputedEntry corresponding to a material_id.
 
-    Args:
-        filename (str): Cif filename. bzipped or gzipped cifs are fine too.
-        occupancy_tolerance (float): If total occupancy of a site is between 1
-            and occupancy_tolerance, the occupancies will be scaled down to 1.
-        site_tolerance (float): This tolerance is used to determine if two
-            sites are sitting in the same position, in which case they will be
-            combined to a single disordered site. Defaults to 1e-4.
-    """
+        Args:
+            material_id (str): Materials Project material_id (a string,
+                e.g., mp-1234).
+            compatible_only (bool): Whether to return only "compatible"
+                entries. Compatible entries are entries that have been
+                processed using the MaterialsProjectCompatibility class,
+                which performs adjustments to allow mixing of GGA and GGA+U
+                calculations for more accurate phase diagrams and reaction
+                energies.
+            inc_structure (str): If None, entries returned are
+                ComputedEntries. If inc_structure="final",
+                ComputedStructureEntries with final structures are returned.
+                Otherwise, ComputedStructureEntries with initial structures
+                are returned.
+            property_data (list): Specify additional properties to include in
+                entry.data. If None, no data. Should be a subset of
+                supported_properties.
 
-    def __init__(self, filename, occupancy_tolerance=1., site_tolerance=1e-4):
-        self._occupancy_tolerance = occupancy_tolerance
-        self._site_tolerance = site_tolerance
-        if isinstance(filename, six.string_types):
-            self._cif = CifFile.from_file(filename)
-        else:
-            self._cif = CifFile.from_string(filename.read())
+        Returns:
+            ComputedEntry or ComputedStructureEntry object.
+        """
+        data = self.get_entries(material_id, compatible_only=compatible_only,
+                                inc_structure=inc_structure, property_data=property_data)
+        return data[0]
 
-    @staticmethod
-    def from_string(cif_string, occupancy_tolerance=1.):
+    def get_dos_by_material_id(self, material_id):
         """
-        Creates a CifParser from a string.
+        Get a Dos corresponding to a material_id.
 
         Args:
-            cif_string (str): String representation of a CIF.
-            occupancy_tolerance (float): If total occupancy of a site is
-                between 1 and occupancy_tolerance, the occupancies will be
-                scaled down to 1.
+            material_id (str): Materials Project material_id (a string,
+                e.g., mp-1234).
 
         Returns:
-            CifParser
+            A Dos object.
         """
-        stream = cStringIO(cif_string)
-        return CifParser(stream, occupancy_tolerance)
+        data = self.get_data(material_id, prop="dos")
+        return data[0]["dos"]
 
-    def _unique_coords(self, coords_in):
+    def get_bandstructure_by_material_id(self, material_id):
         """
-        Generate unique coordinates using coord and symmetry positions.
+        Get a BandStructure corresponding to a material_id.
+
+        Args:
+            material_id (str): Materials Project material_id (an int).
+
+        Returns:
+            A BandStructure object.
         """
-        coords = []
-        for tmp_coord in coords_in:
-            for op in self.symmetry_operations:
-                coord = op.operate(tmp_coord)
-                coord = np.array([i - math.floor(i) for i in coord])
-                if not in_coord_list_pbc(coords, coord,
-                                         atol=self._site_tolerance):
-                    coords.append(coord)
-        return coords
+        data = self.get_data(material_id, prop="bandstructure")
+        return data[0]["bandstructure"]
 
-    def get_lattice(self, data, length_strings=("a", "b", "c"),
-                    angle_strings=("alpha", "beta", "gamma"),
-                    lattice_type=None):
+    def get_entries_in_chemsys(self, elements, compatible_only=True,
+                               inc_structure=None, property_data=None):
         """
-        Generate the lattice from the provided lattice parameters. In
-        the absence of all six lattice parameters, the crystal system
-        and necessary parameters are parsed
+        Helper method to get a list of ComputedEntries in a chemical system.
+        For example, elements = ["Li", "Fe", "O"] will return a list of all
+        entries in the Li-Fe-O chemical system, i.e., all LixOy,
+        FexOy, LixFey, LixFeyOz, Li, Fe and O phases. Extremely useful for
+        creating phase diagrams of entire chemical systems.
+
+        Args:
+            elements ([str]): List of element symbols, e.g., ["Li", "Fe",
+                "O"].
+            compatible_only (bool): Whether to return only "compatible"
+                entries. Compatible entries are entries that have been
+                processed using the MaterialsProjectCompatibility class,
+                which performs adjustments to allow mixing of GGA and GGA+U
+                calculations for more accurate phase diagrams and reaction
+                energies.
+            inc_structure (str): If None, entries returned are
+                ComputedEntries. If inc_structure="final",
+                ComputedStructureEntries with final structures are returned.
+                Otherwise, ComputedStructureEntries with initial structures
+                are returned.
+            property_data (list): Specify additional properties to include in
+                entry.data. If None, no data. Should be a subset of
+                supported_properties.
+
+        Returns:
+            List of ComputedEntries.
         """
-        try:
+        entries = []
+        for i in range(len(elements)):
+            for els in itertools.combinations(elements, i + 1):
+                entries.extend(
+                    self.get_entries(
+                        "-".join(els), compatible_only=compatible_only,
+                        inc_structure=inc_structure,
+                        property_data=property_data))
+        return entries
 
-            lengths = [str2float(data["_cell_length_" + i])
-                       for i in length_strings]
-            angles = [str2float(data["_cell_angle_" + i])
-                      for i in angle_strings]
-            if not lattice_type:
-                return Lattice.from_lengths_and_angles(lengths, angles)
+    def get_exp_thermo_data(self, formula):
+        """
+        Get a list of ThermoData objects associated with a formula using the
+        Materials Project REST interface.
 
-            else:
-                return getattr(Lattice, lattice_type)(*(lengths + angles))
+        Args:
+            formula (str): A formula to search for.
 
-        except KeyError:
-            # Missing Key search for cell setting
-            for lattice_lable in ["_symmetry_cell_setting",
-                                  "_space_group_crystal_system"]:
-                if data.data.get(lattice_lable):
-                    lattice_type = data.data.get(lattice_lable).lower()
-                    try:
-
-                        required_args = getargspec(
-                            getattr(Lattice, lattice_type)).args
-
-                        lengths = (l for l in length_strings
-                                   if l in required_args)
-                        angles = (a for a in angle_strings
-                                  if a in required_args)
-                        return self.get_lattice(data, lengths, angles,
-                                                lattice_type=lattice_type)
-                    except AttributeError as exc:
-                        warnings.warn(exc)
+        Returns:
+            List of ThermoData objects.
+        """
+        return self.get_data(formula, data_type="exp")
 
-                else:
-                    return None
+    def get_exp_entry(self, formula):
+        """
+        Returns an ExpEntry object, which is the experimental equivalent of a
+        ComputedEntry and can be used for analyses using experimental data.
+
+        Args:
+            formula (str): A formula to search for.
 
-    def get_symops(self, data):
+        Returns:
+            An ExpEntry object.
         """
-        In order to generate symmetry equivalent positions, the symmetry
-        operations are parsed. If the symops are not present, the space
-        group symbol is parsed, and symops are generated.
-        """
-        symops = []
-        for symmetry_label in ["_symmetry_equiv_pos_as_xyz",
-                               "_symmetry_equiv_pos_as_xyz_",
-                               "_space_group_symop_operation_xyz",
-                               "_space_group_symop_operation_xyz_"]:
-            if data.data.get(symmetry_label):
-                xyz = data.data.get(symmetry_label)
-                if isinstance(xyz, six.string_types):
-                    warnings.warn("A 1-line symmetry op P1 CIF is detected!")
-                    xyz = [xyz]
-                try:
-                    symops = [SymmOp.from_xyz_string(s)
-                              for s in xyz]
-                    break
-                except ValueError:
-                    continue
-        if not symops:
-            # Try to parse symbol
-            for symmetry_label in ["_symmetry_space_group_name_H-M",
-                                   "_symmetry_space_group_name_H_M",
-                                   "_symmetry_space_group_name_H-M_",
-                                   "_symmetry_space_group_name_H_M_",
-                                   "_space_group_name_Hall",
-                                   "_space_group_name_Hall_",
-                                   "_space_group_name_H-M_alt",
-                                   "_space_group_name_H-M_alt_",
-                                   "_symmetry_space_group_name_hall",
-                                   "_symmetry_space_group_name_hall_",
-                                   "_symmetry_space_group_name_h-m",
-                                   "_symmetry_space_group_name_h-m_"]:
-                sg = data.data.get(symmetry_label)
-
-                if sg:
-                    sg = sub_spgrp(sg)
-                    try:
-                        spg = space_groups.get(sg)
-                        if spg:
-                            symops = SpaceGroup(spg).symmetry_ops
-                            warnings.warn(
-                                "No _symmetry_equiv_pos_as_xyz type key found. "
-                                "Spacegroup from %s used." % symmetry_label)
-                            break
-                    except ValueError:
-                        # Ignore any errors
-                        pass
-
-                    try:
-                        for d in _get_cod_data():
-                            if sg == re.sub(r"\s+", "",
-                                            d["hermann_mauguin"]) :
-                                xyz = d["symops"]
-                                symops = [SymmOp.from_xyz_string(s)
-                                          for s in xyz]
-                                warnings.warn(
-                                    "No _symmetry_equiv_pos_as_xyz type key found. "
-                                    "Spacegroup from %s used." % symmetry_label)
-                                break
-                    except Exception as ex:
-                        continue
-
-                    if symops:
-                        break
-        if not symops:
-            # Try to parse International number
-            for symmetry_label in ["_space_group_IT_number",
-                                   "_space_group_IT_number_",
-                                   "_symmetry_Int_Tables_number",
-                                   "_symmetry_Int_Tables_number_"]:
-                if data.data.get(symmetry_label):
-                    try:
-                        i = int(str2float(data.data.get(symmetry_label)))
-                        symops = SpaceGroup.from_int_number(i).symmetry_ops
-                        break
-                    except ValueError:
-                        continue
-
-        if not symops:
-            warnings.warn("No _symmetry_equiv_pos_as_xyz type key found. "
-                          "Defaulting to P1.")
-            symops = [SymmOp.from_xyz_string(s) for s in ['x', 'y', 'z']]
 
-        return symops
+        return ExpEntry(Composition(formula),
+                        self.get_exp_thermo_data(formula))
 
-    def parse_oxi_states(self, data):
+    def query(self, criteria, properties, mp_decode=True):
         """
-        Parse oxidation states from data dictionary
+        Performs an advanced query, which is a Mongo-like syntax for directly
+        querying the Materials Project database via the query rest interface.
+        Please refer to the Materials Project REST wiki
+        https://materialsproject.org/wiki/index.php/The_Materials_API#query
+        on the query language and supported criteria and properties.
+        Essentially, any supported properties within MPRester should be
+        supported in query.
+
+        Query allows an advanced developer to perform queries which are
+        otherwise too cumbersome to perform using the standard convenience
+        methods.
+
+        It is highly recommended that you consult the Materials API
+        documentation at http://bit.ly/materialsapi, which provides a
+        comprehensive explanation of the document schema used in the
+        Materials Project and how best to query for the relevant information
+        you need.
+
+        Args:
+            criteria (str/dict): Criteria of the query as a string or
+                mongo-style dict.
+
+                If string, it supports a powerful but simple string criteria.
+                E.g., "Fe2O3" means search for materials with reduced_formula
+                Fe2O3. Wild cards are also supported. E.g., "\\*2O" means get
+                all materials whose formula can be formed as \\*2O, e.g.,
+                Li2O, K2O, etc.
+
+                Other syntax examples:
+                mp-1234: Interpreted as a Materials ID.
+                Fe2O3 or \\*2O3: Interpreted as reduced formulas.
+                Li-Fe-O or \\*-Fe-O: Interpreted as chemical systems.
+
+                You can mix and match with spaces, which are interpreted as
+                "OR". E.g. "mp-1234 FeO" means query for all compounds with
+                reduced formula FeO or with materials_id mp-1234.
+
+                Using a full dict syntax, even more powerful queries can be
+                constructed. For example, {"elements":{"$in":["Li",
+                "Na", "K"], "$all": ["O"]}, "nelements":2} selects all Li, Na
+                and K oxides. {"band_gap": {"$gt": 1}} selects all materials
+                with band gaps greater than 1 eV.
+            properties (list): Properties to request for as a list. For
+                example, ["formula", "formation_energy_per_atom"] returns
+                the formula and formation energy per atom.
+            mp_decode (bool): Whether to do a decoding to a Pymatgen object
+                where possible. In some cases, it might be useful to just get
+                the raw python dict, i.e., set to False.
+
+        Returns:
+            List of results. E.g.,
+            [{u'formula': {u'O': 1, u'Li': 2.0}},
+            {u'formula': {u'Na': 2.0, u'O': 2.0}},
+            {u'formula': {u'K': 1, u'O': 3.0}},
+            ...]
+        """
+        if not isinstance(criteria, dict):
+            criteria = MPRester.parse_criteria(criteria)
+        payload = {"criteria": json.dumps(criteria),
+                   "properties": json.dumps(properties)}
+        return self._make_request("/query", payload=payload, method="POST",
+                                  mp_decode=mp_decode)
+
+    def submit_structures(self, structures, authors, projects=None,
+                          references='', remarks=None, data=None,
+                          histories=None, created_at=None):
+        """
+        Submits a list of structures to the Materials Project as SNL files.
+        The argument list mirrors the arguments for the StructureNL object,
+        except that a list of structures with the same metadata is used as an
+        input.
+
+        .. note::
+
+            As of now, this MP REST feature is open only to a select group of
+            users. Opening up submissions to all users is being planned for
+            the future.
+
+        Args:
+            structures: A list of Structure objects
+            authors (list): List of {"name":'', "email":''} dicts,
+                *list* of Strings as 'John Doe <johndoe@gmail.com>',
+                or a single String with commas separating authors
+            projects ([str]): List of Strings ['Project A', 'Project B'].
+                This applies to all structures.
+            references (str): A String in BibTeX format. Again, this applies to
+                all structures.
+            remarks ([str]): List of Strings ['Remark A', 'Remark B']
+            data ([dict]): A list of free form dict. Namespaced at the root
+                level with an underscore, e.g. {"_materialsproject":<custom
+                data>}. The length of data should be the same as the list of
+                structures if not None.
+            histories: List of list of dicts - [[{'name':'', 'url':'',
+                'description':{}}], ...] The length of histories should be the
+                same as the list of structures if not None.
+            created_at (datetime): A datetime object
+
+        Returns:
+            A list of inserted submission ids.
+        """
+        from pymatgen.matproj.snl import StructureNL
+        snl_list = StructureNL.from_structures(structures, authors, projects,
+                                               references, remarks, data,
+                                               histories, created_at)
+        self.submit_snl(snl_list)
+
+    def submit_snl(self, snl):
+        """
+        Submits a list of StructureNL to the Materials Project site.
+
+        .. note::
+
+            As of now, this MP REST feature is open only to a select group of
+            users. Opening up submissions to all users is being planned for
+            the future.
+
+        Args:
+            snl (StructureNL/[StructureNL]): A single StructureNL, or a list
+            of StructureNL objects
+
+        Returns:
+            A list of inserted submission ids.
+
+        Raises:
+            MPRestError
         """
         try:
-            oxi_states = {
-                data["_atom_type_symbol"][i]:
-                    str2float(data["_atom_type_oxidation_number"][i])
-                for i in range(len(data["_atom_type_symbol"]))}
-            # attempt to strip oxidation state from _atom_type_symbol
-            # in case the label does not contain an oxidation state
-            for i, symbol in enumerate(data["_atom_type_symbol"]):
-                oxi_states[re.sub(r"\d?[\+,\-]?$", "", symbol)] = \
-                    str2float(data["_atom_type_oxidation_number"][i])
-
-        except (ValueError, KeyError):
-            oxi_states = None
-        return oxi_states
-
-    def _get_structure(self, data, primitive):
-        """
-        Generate structure from part of the cif.
-        """
-        def parse_symbol(sym):
-            # Common representations for elements/water in cif files
-            # TODO: fix inconsistent handling of water
-            special = {"D": "D", "Hw": "H", "Ow": "O", "Wat": "O",
-                       "wat": "O", "OH": "", "OH2": ""}
-            m = re.findall(r"w?[A-Z][a-z]*", sym)
-            if m and m != "?":
-                if sym in special:
-                    v = special[sym]
+            snl = snl if isinstance(snl, list) else [snl]
+            jsondata = [s.as_dict() for s in snl]
+            payload = {"snl": json.dumps(jsondata, cls=MontyEncoder)}
+            response = self.session.post("{}/snl/submit".format(self.preamble),
+                                         data=payload)
+            if response.status_code in [200, 400]:
+                resp = json.loads(response.text, cls=MontyDecoder)
+                if resp["valid_response"]:
+                    if resp.get("warning"):
+                        warnings.warn(resp["warning"])
+                    return resp['inserted_ids']
                 else:
-                    v = special.get(m[0], m[0])
-                if len(m) > 1 or (m[0] in special):
-                    warnings.warn("{} parsed as {}".format(sym, v))
-                return v
-
-        lattice = self.get_lattice(data)
-        self.symmetry_operations = self.get_symops(data)
-        oxi_states = self.parse_oxi_states(data)
-
-        coord_to_species = OrderedDict()
-
-        def get_matching_coord(coord):
-            keys = list(coord_to_species.keys())
-            coords = np.array(keys)
-            for op in self.symmetry_operations:
-                c = op.operate(coord)
-                inds = find_in_coord_list_pbc(coords, c, atol=self._site_tolerance)
-                # cant use if inds, because python is dumb and np.array([0]) evaluates
-                # to False
-                if len(inds):
-                    return keys[inds[0]]
-            return False
-
-        ############################################################
-        """
-        This part of the code deals with handling formats of data as found in
-        CIF files extracted from the Springer Materials/Pauling File
-        databases, and that are different from standard ICSD formats.
-        """
-
-        # Check to see if "_atom_site_type_symbol" exists, as some test CIFs do
-        # not contain this key.
-        if "_atom_site_type_symbol" in data.data.keys():
-
-            # Keep a track of which data row needs to be removed.
-            # Example of a row: Nb,Zr '0.8Nb + 0.2Zr' .2a .m-3m 0 0 0 1 14
-            # 'rhombic dodecahedron, Nb<sub>14</sub>'
-            # Without this code, the above row in a structure would be parsed
-            # as an ordered site with only Nb (since
-            # CifParser would try to parse the first two characters of the
-            # label "Nb,Zr") and occupancy=1.
-            # However, this site is meant to be a disordered site with 0.8 of
-            # Nb and 0.2 of Zr.
-            idxs_to_remove = []
-
-            for idx, el_row in enumerate(data["_atom_site_label"]):
-
-                # CIF files from the Springer Materials/Pauling File have
-                # switched the label and symbol. Thus, in the
-                # above shown example row, '0.8Nb + 0.2Zr' is the symbol.
-                # Below, we split the strings on ' + ' to
-                # check if the length (or number of elements) in the label and
-                # symbol are equal.
-                if len(data["_atom_site_type_symbol"][idx].split(' + ')) > \
-                        len(data["_atom_site_label"][idx].split(' + ')):
-
-                    # Dictionary to hold extracted elements and occupancies
-                    els_occu = {}
-
-                    # parse symbol to get element names and occupancy and store
-                    # in "els_occu"
-                    symbol_str = data["_atom_site_type_symbol"][idx]
-                    symbol_str_lst = symbol_str.split(' + ')
-                    for elocc_idx in range(len(symbol_str_lst)):
-                        # Remove any bracketed items in the string
-                        symbol_str_lst[elocc_idx] = re.sub(r'\([0-9]*\)', '',
-                            symbol_str_lst[elocc_idx].strip())
-
-                        # Extract element name and its occupancy from the
-                        # string, and store it as a
-                        # key-value pair in "els_occ".
-                        els_occu[str(re.findall(r'\D+', symbol_str_lst[
-                            elocc_idx].strip())[1]).replace('<sup>', '')] = \
-                            float('0' + re.findall(r'\.?\d+', symbol_str_lst[
-                                elocc_idx].strip())[1])
-
-                    x = str2float(data["_atom_site_fract_x"][idx])
-                    y = str2float(data["_atom_site_fract_y"][idx])
-                    z = str2float(data["_atom_site_fract_z"][idx])
-
-                    coord = (x, y, z)
-                    # Add each partially occupied element on the site coordinate
-                    for et in els_occu:
-                        match = get_matching_coord(coord)
-                        if not match:
-                            coord_to_species[coord] = Composition(
-                                {parse_symbol(et): els_occu[parse_symbol(et)]})
-                        else:
-                            coord_to_species[match] += {
-                                parse_symbol(et): els_occu[parse_symbol(et)]}
-                    idxs_to_remove.append(idx)
-
-            # Remove the original row by iterating over all keys in the CIF
-            # data looking for lists, which indicates
-            # multiple data items, one for each row, and remove items from the
-            # list that corresponds to the removed row,
-            # so that it's not processed by the rest of this function (which
-            # would result in an error).
-            for cif_key in data.data:
-                if type(data.data[cif_key]) == list:
-                    for id in sorted(idxs_to_remove, reverse=True):
-                        del data.data[cif_key][id]
-
-        ############################################################
-        for i in range(len(data["_atom_site_label"])):
-            try:
-                # If site type symbol exists, use it. Otherwise, we use the
-                # label.
-                symbol = parse_symbol(data["_atom_site_type_symbol"][i])
-            except KeyError:
-                symbol = parse_symbol(data["_atom_site_label"][i])
-            if not symbol:
-                continue
-
-            if oxi_states is not None:
-                o_s = oxi_states.get(symbol, 0)
-                # use _atom_site_type_symbol if possible for oxidation state
-                if "_atom_site_type_symbol" in data.data.keys():
-                    oxi_symbol = data["_atom_site_type_symbol"][i]
-                    o_s = oxi_states.get(oxi_symbol, o_s)
-                try:
-                    el = Specie(symbol, o_s)
-                except:
-                    el = DummySpecie(symbol, o_s)
-            else:
-                el = get_el_sp(symbol)
+                    raise MPRestError(resp["error"])
 
-            x = str2float(data["_atom_site_fract_x"][i])
-            y = str2float(data["_atom_site_fract_y"][i])
-            z = str2float(data["_atom_site_fract_z"][i])
-
-            try:
-                occu = str2float(data["_atom_site_occupancy"][i])
-            except (KeyError, ValueError):
-                occu = 1
-
-            if occu > 0:
-                coord = (x, y, z)
-                match = get_matching_coord(coord)
-                if not match:
-                    coord_to_species[coord] = Composition({el: occu})
-                else:
-                    coord_to_species[match] += {el: occu}
+            raise MPRestError("REST error with status code {} and error {}"
+                              .format(response.status_code, response.text))
 
-        sum_occu = [sum(c.values()) for c in coord_to_species.values()]
-        if any([o > 1 for o in sum_occu]):
-            warnings.warn("Some occupancies (%s) sum to > 1! If they are within "
-                          "the tolerance, they will be rescaled." % str(sum_occu))
+        except Exception as ex:
+            raise MPRestError(str(ex))
 
-        allspecies = []
-        allcoords = []
+    def delete_snl(self, snl_ids):
+        """
+        Delete earlier submitted SNLs.
 
-        if coord_to_species.items():
-            for species, group in groupby(
-                    sorted(list(coord_to_species.items()), key=lambda x: x[1]),
-                    key=lambda x: x[1]):
-                tmp_coords = [site[0] for site in group]
+        .. note::
 
-                coords = self._unique_coords(tmp_coords)
+            As of now, this MP REST feature is open only to a select group of
+            users. Opening up submissions to all users is being planned for
+            the future.
 
-                allcoords.extend(coords)
-                allspecies.extend(len(coords) * [species])
+        Args:
+            snl_ids: List of SNL ids.
 
-            # rescale occupancies if necessary
-            for i, species in enumerate(allspecies):
-                totaloccu = sum(species.values())
-                if 1 < totaloccu <= self._occupancy_tolerance:
-                    allspecies[i] = species / totaloccu
+        Raises:
+            MPRestError
+        """
+        try:
+            payload = {"ids": json.dumps(snl_ids)}
+            response = self.session.post(
+                "{}/snl/delete".format(self.preamble), data=payload)
+
+            if response.status_code in [200, 400]:
+                resp = json.loads(response.text, cls=MontyDecoder)
+                if resp["valid_response"]:
+                    if resp.get("warning"):
+                        warnings.warn(resp["warning"])
+                    return resp
+                else:
+                    raise MPRestError(resp["error"])
 
-        if allspecies and len(allspecies) == len(allcoords):
-            struct = Structure(lattice, allspecies, allcoords)
-            struct = struct.get_sorted_structure()
+            raise MPRestError("REST error with status code {} and error {}"
+                              .format(response.status_code, response.text))
 
-            if primitive:
-                struct = struct.get_primitive_structure()
-                struct = struct.get_reduced_structure()
-            return struct
+        except Exception as ex:
+            raise MPRestError(str(ex))
 
-    def get_structures(self, primitive=True):
+    def query_snl(self, criteria):
         """
-        Return list of structures in CIF file. primitive boolean sets whether a
-        conventional cell structure or primitive cell structure is returned.
+        Query for submitted SNLs.
+
+        .. note::
+
+            As of now, this MP REST feature is open only to a select group of
+            users. Opening up submissions to all users is being planned for
+            the future.
 
         Args:
-            primitive (bool): Set to False to return conventional unit cells.
-                Defaults to True.
+            criteria (dict): Query criteria.
 
         Returns:
-            List of Structures.
+            A dict, with a list of submitted SNLs in the "response" key.
+
+        Raises:
+            MPRestError
         """
-        structures = []
-        for d in self._cif.data.values():
-            try:
-                s = self._get_structure(d, primitive)
-                if s:
-                    structures.append(s)
-            except (KeyError, ValueError) as exc:
-                # Warn the user (Errors should never pass silently)
-                # A user reported a problem with cif files produced by Avogadro
-                # in which the atomic coordinates are in Cartesian coords.
-                warnings.warn(str(exc))
-        if len(structures) == 0:
-            raise ValueError("Invalid cif file with no structures!")
-        return structures
-
-    def as_dict(self):
-        d = OrderedDict()
-        for k, v in self._cif.data.items():
-            d[k] = {}
-            for k2, v2 in v.data.items():
-                d[k][k2] = v2
-        return d
+        try:
+            payload = {"criteria": json.dumps(criteria)}
+            response = self.session.post("{}/snl/query".format(self.preamble),
+                                         data=payload)
+            if response.status_code in [200, 400]:
+                resp = json.loads(response.text)
+                if resp["valid_response"]:
+                    if resp.get("warning"):
+                        warnings.warn(resp["warning"])
+                    return resp["response"]
+                else:
+                    raise MPRestError(resp["error"])
 
+            raise MPRestError("REST error with status code {} and error {}"
+                              .format(response.status_code, response.text))
 
-class CifWriter(object):
-    """
-    A wrapper around CifFile to write CIF files from pymatgen structures.
+        except Exception as ex:
+            raise MPRestError(str(ex))
 
-    Args:
-        struct (Structure): structure to write
-        symprec (float): If not none, finds the symmetry of the structure
-            and writes the cif with symmetry information. Passes symprec
-            to the SpacegroupAnalyzer
-    """
+    def submit_vasp_directory(self, rootdir, authors, projects=None,
+                              references='', remarks=None, master_data=None,
+                              master_history=None, created_at=None,
+                              ncpus=None):
+        """
+        Assimilates all vasp run directories beneath a particular
+        directory using BorgQueen to obtain structures, and then submits thhem
+        to the Materials Project as SNL files. VASP related meta data like
+        initial structure and final energies are automatically incorporated.
 
-    def __init__(self, struct, symprec=None):
-        format_str = "{:.8f}"
+        .. note::
 
-        block = OrderedDict()
-        loops = []
-        spacegroup = ("P 1", 1)
-        if symprec is not None:
-            sf = SpacegroupAnalyzer(struct, symprec)
-            spacegroup = (sf.get_space_group_symbol(),
-                          sf.get_space_group_number())
-            # Needs the refined struture when using symprec. This converts
-            # primitive to conventional structures, the standard for CIF.
-            struct = sf.get_refined_structure()
-
-        latt = struct.lattice
-        comp = struct.composition
-        no_oxi_comp = comp.element_composition
-        block["_symmetry_space_group_name_H-M"] = spacegroup[0]
-        for cell_attr in ['a', 'b', 'c']:
-            block["_cell_length_" + cell_attr] = format_str.format(
-                getattr(latt, cell_attr))
-        for cell_attr in ['alpha', 'beta', 'gamma']:
-            block["_cell_angle_" + cell_attr] = format_str.format(
-                getattr(latt, cell_attr))
-        block["_symmetry_Int_Tables_number"] = spacegroup[1]
-        block["_chemical_formula_structural"] = no_oxi_comp.reduced_formula
-        block["_chemical_formula_sum"] = no_oxi_comp.formula
-        block["_cell_volume"] = latt.volume.__str__()
-
-        reduced_comp, fu = no_oxi_comp.get_reduced_composition_and_factor()
-        block["_cell_formula_units_Z"] = str(int(fu))
-
-        if symprec is None:
-            block["_symmetry_equiv_pos_site_id"] = ["1"]
-            block["_symmetry_equiv_pos_as_xyz"] = ["x, y, z"]
-        else:
-            sf = SpacegroupAnalyzer(struct, symprec)
+            As of now, this MP REST feature is open only to a select group of
+            users. Opening up submissions to all users is being planned for
+            the future.
 
-            symmops = []
-            for op in sf.get_symmetry_operations():
-                v = op.translation_vector
-                symmops.append(SymmOp.from_rotation_and_translation(
-                    op.rotation_matrix, v))
-
-            ops = [op.as_xyz_string() for op in symmops]
-            block["_symmetry_equiv_pos_site_id"] = \
-                ["%d" % i for i in range(1, len(ops) + 1)]
-            block["_symmetry_equiv_pos_as_xyz"] = ops
+        Args:
+            rootdir (str): Rootdir to start assimilating VASP runs from.
+            authors: *List* of {"name":'', "email":''} dicts,
+                *list* of Strings as 'John Doe <johndoe@gmail.com>',
+                or a single String with commas separating authors. The same
+                list of authors should apply to all runs.
+            projects ([str]): List of Strings ['Project A', 'Project B'].
+                This applies to all structures.
+            references (str): A String in BibTeX format. Again, this applies to
+                all structures.
+            remarks ([str]): List of Strings ['Remark A', 'Remark B']
+            master_data (dict): A free form dict. Namespaced at the root
+                level with an underscore, e.g. {"_materialsproject":<custom
+                data>}. This data is added to all structures detected in the
+                directory, in addition to other vasp data on a per structure
+                basis.
+            master_history: A master history to be added to all entries.
+            created_at (datetime): A datetime object
+            ncpus (int): Number of cpus to use in using BorgQueen to
+                assimilate. Defaults to None, which means serial.
+        """
+        from pymatgen.apps.borg.hive import VaspToComputedEntryDrone
+        from pymatgen.apps.borg.queen import BorgQueen
+        drone = VaspToComputedEntryDrone(inc_structure=True,
+                                         data=["filename",
+                                               "initial_structure"])
+        queen = BorgQueen(drone, number_of_drones=ncpus)
+        queen.parallel_assimilate(rootdir)
 
-        loops.append(["_symmetry_equiv_pos_site_id",
-                      "_symmetry_equiv_pos_as_xyz"])
+        structures = []
+        metadata = []
+        histories = []
+        for e in queen.get_data():
+            structures.append(e.structure)
+            m = {
+                "_vasp": {
+                    "parameters": e.parameters,
+                    "final_energy": e.energy,
+                    "final_energy_per_atom": e.energy_per_atom,
+                    "initial_structure": e.data["initial_structure"].as_dict()
+                }
+            }
+            if "history" in e.parameters:
+                histories.append(e.parameters["history"])
+            if master_data is not None:
+                m.update(master_data)
+            metadata.append(m)
+        if master_history is not None:
+            histories = master_history * len(structures)
+
+        return self.submit_structures(
+            structures, authors, projects=projects, references=references,
+            remarks=remarks, data=metadata, histories=histories,
+            created_at=created_at)
 
-        contains_oxidation = True
+    def get_stability(self, entries):
+        """
+        Returns the stability of all entries.
+        """
         try:
-            symbol_to_oxinum = OrderedDict([
-                                               (el.__str__(),
-                                                float(el.oxi_state))
-                                               for el in sorted(comp.elements)])
-        except AttributeError:
-            symbol_to_oxinum = OrderedDict([(el.symbol, 0) for el in
-                                            sorted(comp.elements)])
-            contains_oxidation = False
-        if contains_oxidation:
-            block["_atom_type_symbol"] = symbol_to_oxinum.keys()
-            block["_atom_type_oxidation_number"] = symbol_to_oxinum.values()
-            loops.append(["_atom_type_symbol", "_atom_type_oxidation_number"])
-
-        atom_site_type_symbol = []
-        atom_site_symmetry_multiplicity = []
-        atom_site_fract_x = []
-        atom_site_fract_y = []
-        atom_site_fract_z = []
-        atom_site_label = []
-        atom_site_occupancy = []
-        count = 1
-        if symprec is None:
-            for site in struct:
-                for sp, occu in sorted(site.species_and_occu.items()):
-                    atom_site_type_symbol.append(sp.__str__())
-                    atom_site_symmetry_multiplicity.append("1")
-                    atom_site_fract_x.append("{0:f}".format(site.a))
-                    atom_site_fract_y.append("{0:f}".format(site.b))
-                    atom_site_fract_z.append("{0:f}".format(site.c))
-                    atom_site_label.append("{}{}".format(sp.symbol, count))
-                    atom_site_occupancy.append(occu.__str__())
-                    count += 1
-        else:
-            # The following just presents a deterministic ordering.
-            unique_sites = [
-                (sorted(sites, key=lambda s: tuple([abs(x) for x in
-                                                    s.frac_coords]))[0],
-                 len(sites))
-                for sites in sf.get_symmetrized_structure().equivalent_sites
-                ]
-            for site, mult in sorted(
-                    unique_sites,
-                    key=lambda t: (t[0].species_and_occu.average_electroneg,
-                                   -t[1], t[0].a, t[0].b, t[0].c)):
-                for sp, occu in site.species_and_occu.items():
-                    atom_site_type_symbol.append(sp.__str__())
-                    atom_site_symmetry_multiplicity.append("%d" % mult)
-                    atom_site_fract_x.append("{0:f}".format(site.a))
-                    atom_site_fract_y.append("{0:f}".format(site.b))
-                    atom_site_fract_z.append("{0:f}".format(site.c))
-                    atom_site_label.append("{}{}".format(sp.symbol, count))
-                    atom_site_occupancy.append(occu.__str__())
-                    count += 1
-
-        block["_atom_site_type_symbol"] = atom_site_type_symbol
-        block["_atom_site_label"] = atom_site_label
-        block["_atom_site_symmetry_multiplicity"] = \
-            atom_site_symmetry_multiplicity
-        block["_atom_site_fract_x"] = atom_site_fract_x
-        block["_atom_site_fract_y"] = atom_site_fract_y
-        block["_atom_site_fract_z"] = atom_site_fract_z
-        block["_atom_site_occupancy"] = atom_site_occupancy
-        loops.append(["_atom_site_type_symbol",
-                      "_atom_site_label",
-                      "_atom_site_symmetry_multiplicity",
-                      "_atom_site_fract_x",
-                      "_atom_site_fract_y",
-                      "_atom_site_fract_z",
-                      "_atom_site_occupancy"])
-        d = OrderedDict()
-        d[comp.reduced_formula] = CifBlock(block, loops, comp.reduced_formula)
-        self._cf = CifFile(d)
-
-    def __str__(self):
-        """
-        Returns the cif as a string.
-        """
-        return self._cf.__str__()
-
-    def write_file(self, filename):
+            payload = {"entries": json.dumps(entries, cls=MontyEncoder)}
+            response = self.session.post("{}/phase_diagram/calculate_stability"
+                                         .format(self.preamble), data=payload)
+            if response.status_code in [200, 400]:
+                resp = json.loads(response.text, cls=MontyDecoder)
+                if resp["valid_response"]:
+                    if resp.get("warning"):
+                        warnings.warn(resp["warning"])
+                    return resp["response"]
+                else:
+                    raise MPRestError(resp["error"])
+            raise MPRestError("REST error with status code {} and error {}"
+                              .format(response.status_code, response.text))
+        except Exception as ex:
+            raise MPRestError(str(ex))
+
+    def get_reaction(self, reactants, products):
+        """
+        Gets a reaction from the Materials Project.
+
+        Args:
+            reactants ([str]): List of formulas
+            products ([str]): List of formulas
+
+        Returns:
+            rxn
+        """
+        return self._make_request("/reaction",
+                                  payload={"reactants[]": reactants,
+                                           "products[]": products}, mp_decode=False)
+
+    def get_substrates(self, material_id, number=50, orient=None):
+        """
+        Get a substrate list for a material id. The list is in order of
+        increasing elastic energy if a elastic tensor is available for
+        the material_id. Otherwise the list is in order of increasing
+        matching area.
+
+        Args:
+            material_id (str): Materials Project material_id, e.g. 'mp-123'.
+            orient (list) : substrate orientation to look for
+            number (int) : number of substrates to return;
+                n=0 returns all available matches
+        Returns:
+            list of dicts with substrate matches
+        """
+        req = "/materials/{}/substrates?n={}".format(material_id, number)
+        if orient:
+            req += "&orient={}".format(" ".join(map(str, orient)))
+        return self._make_request(req)
+
+    def get_all_substrates(self):
+        """
+        Gets the list of all possible substrates considered in the
+        Materials Project substrate database
+
+        Returns:
+            list of material_ids corresponding to possible substrates
         """
-        Write the cif file.
+
+        return self._make_request("/materials/all_substrate_ids")
+
+    @staticmethod
+    def parse_criteria(criteria_string):
         """
-        with zopen(filename, "wt") as f:
-            f.write(self.__str__())
+        Parses a powerful and simple string criteria and generates a proper
+        mongo syntax criteria.
 
+        Args:
+            criteria_string (str): A string representing a search criteria.
+                Also supports wild cards. E.g.,
+                something like "*2O" gets converted to
+                {'pretty_formula': {'$in': [u'B2O', u'Xe2O', u"Li2O", ...]}}
+
+                Other syntax examples:
+                    mp-1234: Interpreted as a Materials ID.
+                    Fe2O3 or *2O3: Interpreted as reduced formulas.
+                    Li-Fe-O or *-Fe-O: Interpreted as chemical systems.
+
+                You can mix and match with spaces, which are interpreted as
+                "OR". E.g., "mp-1234 FeO" means query for all compounds with
+                reduced formula FeO or with materials_id mp-1234.
 
-def str2float(text):
+        Returns:
+            A mongo query dict.
+        """
+        toks = criteria_string.split()
+
+        def parse_sym(sym):
+            if sym == "*":
+                return [el.symbol for el in Element]
+            else:
+                m = re.match(r"\{(.*)\}", sym)
+                if m:
+                    return [s.strip() for s in m.group(1).split(",")]
+                else:
+                    return [sym]
+
+        def parse_tok(t):
+            if re.match(r"\w+-\d+", t):
+                return {"task_id": t}
+            elif "-" in t:
+                elements = [parse_sym(sym) for sym in t.split("-")]
+                chemsyss = []
+                for cs in itertools.product(*elements):
+                    if len(set(cs)) == len(cs):
+                        # Check for valid symbols
+                        cs = [Element(s).symbol for s in cs]
+                        chemsyss.append("-".join(sorted(cs)))
+                return {"chemsys": {"$in": chemsyss}}
+            else:
+                all_formulas = set()
+                explicit_els = []
+                wild_card_els = []
+                for sym in re.findall(
+                        r"(\*[\.\d]*|\{.*\}[\.\d]*|[A-Z][a-z]*)[\.\d]*", t):
+                    if ("*" in sym) or ("{" in sym):
+                        wild_card_els.append(sym)
+                    else:
+                        m = re.match(r"([A-Z][a-z]*)[\.\d]*", sym)
+                        explicit_els.append(m.group(1))
+                nelements = len(wild_card_els) + len(set(explicit_els))
+                parts = re.split(r"(\*|\{.*\})", t)
+                parts = [parse_sym(s) for s in parts if s != ""]
+                for f in itertools.product(*parts):
+                    c = Composition("".join(f))
+                    if len(c) == nelements:
+                        # Check for valid Elements in keys.
+                        for e in c.keys():
+                            Element(e.symbol)
+                        all_formulas.add(c.reduced_formula)
+                return {"pretty_formula": {"$in": list(all_formulas)}}
+
+        if len(toks) == 1:
+            return parse_tok(toks[0])
+        else:
+            return {"$or": list(map(parse_tok, toks))}
+
+
+class MPRestError(Exception):
     """
-    Remove uncertainty brackets from strings and return the float.
+    Exception class for MPRestAdaptor.
+    Raised when the query has problems, e.g., bad query format.
     """
-
-    try:
-        return float(re.sub(r"\(.+\)", "", text))
-    except TypeError:
-        if isinstance(text, list) and len(text) == 1:
-            return float(re.sub(r"\(.+\)", "", text[0]))
-    except ValueError as ex:
-        if text.strip() == ".":
-            return 0
-        raise ex
+    pass
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pymatgen-4.7.6/pymatgen/io/cssr.py` & `pymatgen-4.7.7/pymatgen/io/cssr.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/exciting/inputs.py` & `pymatgen-4.7.7/pymatgen/io/exciting/inputs.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/feff/inputs.py` & `pymatgen-4.7.7/pymatgen/io/feff/inputs.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/feff/outputs.py` & `pymatgen-4.7.7/pymatgen/io/feff/outputs.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/feff/sets.py` & `pymatgen-4.7.7/pymatgen/io/feff/sets.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/fiesta.py` & `pymatgen-4.7.7/pymatgen/io/fiesta.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/gaussian.py` & `pymatgen-4.7.7/pymatgen/io/gaussian.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/lammps/data.py` & `pymatgen-4.7.7/pymatgen/io/lammps/data.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/lammps/force_field.py` & `pymatgen-4.7.7/pymatgen/io/lammps/force_field.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/lammps/input.py` & `pymatgen-4.7.7/pymatgen/io/lammps/input.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/lammps/NPT.json` & `pymatgen-4.7.7/pymatgen/io/lammps/NPT.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/lammps/NPT_NVT.json` & `pymatgen-4.7.7/pymatgen/io/lammps/NPT_NVT.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/lammps/NVT.json` & `pymatgen-4.7.7/pymatgen/io/lammps/NVT.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/lammps/output.py` & `pymatgen-4.7.7/pymatgen/io/lammps/output.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/lammps/topology.py` & `pymatgen-4.7.7/pymatgen/io/lammps/topology.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/lammps/utils.py` & `pymatgen-4.7.7/pymatgen/io/lammps/utils.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/nwchem.py` & `pymatgen-4.7.7/pymatgen/io/nwchem.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/phonopy.py` & `pymatgen-4.7.7/pymatgen/io/phonopy.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/pwscf.py` & `pymatgen-4.7.7/pymatgen/io/xr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,187 +1,164 @@
 # coding: utf-8
 # Copyright (c) Pymatgen Development Team.
 # Distributed under the terms of the MIT License.
 
 from __future__ import division, unicode_literals
 
-import six
-
-from monty.re import regrep
-from collections import defaultdict
-
 """
-This module implements input and output processing from PWSCF.
+This module provides input and output mechanisms
+for the xr file format, which is a modified CSSR
+file format and, for example, used in GULP.
+In particular, the module makes it easy
+to remove shell positions from relaxations
+that employed core-shell models.
 """
 
-__author__ = "Shyue Ping Ong"
-__copyright__ = "Copyright 2012, The Materials Virtual Lab"
+
+__author__ = "Nils Edvin Richard Zimmermann"
+__copyright__ = "Copyright 2016, The Materials Project"
 __version__ = "0.1"
-__maintainer__ = "Shyue Ping Ong"
-__email__ = "ongsp@ucsd.edu"
-__date__ = "3/27/15"
+__maintainer__ = "Nils Edvin Richard Zimmermann"
+__email__ = "nils.e.r.zimmermann@gmail.com"
+__date__ = "June 23, 2016"
 
+import re
 
-class PWInput(object):
-    """
-    Base input file class. Right now, only supports no symmetry and is
-    very basic.
+from six.moves import map
+import numpy as np
+
+from monty.io import zopen
+from math import fabs
+from pymatgen.core.lattice import Lattice
+from pymatgen.core.structure import Structure
+
+class Xr(object):
     """
+    Basic object for working with xr files.
 
-    def __init__(self, structure, pseudo, control=None, system=None,
-                 electrons=None, ions=None, cell=None, kpoints_mode="automatic",
-                 kpoints_grid=(1, 1, 1),kpoints_shift=(0, 0, 0)):
-        """
-        Initializes a PWSCF input file.
+    Args:
+        structure (Structure/IStructure): Structure object to create the
+                Xr object.
+    """
 
-        Args:
-            structure (Structure): Input structure
-            pseudo (dict): A dict of the pseudopotentials to use.
-            control (dict): Control parameters. Refer to official PWSCF doc
-                on supported parameters. Default to {"calculation": "scf"}
-            system (dict): System parameters. Refer to official PWSCF doc
-                on supported parameters. Default to None, which means {}.
-            electrons (dict): Electron parameters. Refer to official PWSCF doc
-                on supported parameters. Default to None, which means {}.
-            ions (dict): Ions parameters. Refer to official PWSCF doc
-                on supported parameters. Default to None, which means {}.
-            cell (dict): Cell parameters. Refer to official PWSCF doc
-                on supported parameters. Default to None, which means {}.
-            kpoints_mode (str): Kpoints generation mode. Default to automatic.
-            kpoints_grid (sequence): The kpoint grid. Default to (1, 1, 1).
-            kpoints_shift (sequence): The shift for the kpoints. Defaults to
-                (0, 0, 0).
-        """
+    def __init__(self, structure):
+        if not structure.is_ordered:
+            raise ValueError("Xr file can only be constructed from ordered "
+                             "structure")
         self.structure = structure
-        sections = {}
-        sections["control"] = control or {"calculation": "scf"}
-        sections["system"] = system or {}
-        sections["electrons"] = electrons or {}
-        sections["ions"] = ions or {}
-        sections["cell"] = cell or {}
-        for species in self.structure.composition.keys():
-            if species.symbol not in pseudo:
-                raise PWInputError("Missing %s in pseudo specification!")
-        self.pseudo = pseudo
-        self.sections = sections
-        self.kpoints_mode = kpoints_mode
-        self.kpoints_grid = kpoints_grid
-        self.kpoints_shift = kpoints_shift
 
     def __str__(self):
-        out = []
-        def to_str(v):
-            if isinstance(v, six.string_types):
-                return "'%s'" % v
-            return v
-        for k1 in ["control", "system", "electrons", "ions", "cell"]:
-            v1 = self.sections[k1]
-            out.append("&%s" % k1.upper())
-            sub = []
-            for k2 in sorted(v1.keys()):
-                sub.append("  %s = %s" % (k2, to_str(v1[k2])))
-            if k1 == "system":
-                sub.append("  ibrav = 0")
-                sub.append("  nat = %d" % len(self.structure))
-                sub.append("  ntyp = %d" % len(self.structure.composition))
-            sub.append("/")
-            out.append(",\n".join(sub))
-
-        out.append("ATOMIC_SPECIES")
-        for k, v in self.structure.composition.items():
-            out.append("  %s %.4f %s" % (k.symbol, k.atomic_mass,
-                                         self.pseudo[k.symbol]))
-        out.append("ATOMIC_POSITIONS crystal")
-        for site in self.structure:
-            out.append("  %s %.6f %.6f %.6f" % (site.specie.symbol, site.a,
-                                                site.b, site.c))
-        out.append("K_POINTS %s" % self.kpoints_mode)
-        kpt_str = ["%s" % i for i in self.kpoints_grid]
-        kpt_str.extend(["%s" % i for i in self.kpoints_shift])
-        out.append("  %s" % " ".join(kpt_str))
-        out.append("CELL_PARAMETERS angstrom")
-        for vec in self.structure.lattice.matrix:
-            out.append("  %f %f %f" % (vec[0], vec[1], vec[2]))
-        return "\n".join(out)
+        output = ["pymatgen   {:.4f} {:.4f} {:.4f}"
+                  .format(*self.structure.lattice.abc),
+                  "{:.3f} {:.3f} {:.3f}"
+                  .format(*self.structure.lattice.angles),
+                  "{} 0".format(len(self.structure)),
+                  "0 {}".format(self.structure.formula)]
+        # There are actually 10 more fields per site
+        # in a typical xr file from GULP, for example.
+        for i, site in enumerate(self.structure.sites):
+            output.append("{} {} {:.4f} {:.4f} {:.4f}"
+                          .format(i + 1, site.specie, site.x, site.y, site.z))
+        mat = self.structure.lattice.matrix
+        for i in range(2):
+            for j in range(3):
+                output.append("{:.4f} {:.4f} {:.4f}".format(
+                        mat[j][0], mat[j][1], mat[j][2]))
+        return "\n".join(output)
 
     def write_file(self, filename):
         """
-        Write the PWSCF input file.
+        Write out an xr file.
 
         Args:
-            filename (str): The string filename to output to.
+            filename (str): name of the file to write to.
         """
-        with open(filename, "w") as f:
-            f.write(self.__str__())
-
-
-class PWInputError(BaseException):
-    pass
+        with zopen(filename, 'wt') as f:
+            f.write(str(self) + "\n")
 
+    @staticmethod
+    def from_string(string, use_cores=True, thresh=1.e-4):
+        """
+        Creates an Xr object from a string representation.
 
-class PWOutput(object):
-
-    patterns = {
-        "energies": r'total energy\s+=\s+([\d\.\-]+)\sRy',
-        "ecut": r'kinetic\-energy cutoff\s+=\s+([\d\.\-]+)\s+Ry',
-        "lattice_type": r'bravais\-lattice index\s+=\s+(\d+)',
-        "celldm1": r"celldm\(1\)=\s+([\d\.]+)\s",
-        "celldm2": r"celldm\(2\)=\s+([\d\.]+)\s",
-        "celldm3": r"celldm\(3\)=\s+([\d\.]+)\s",
-        "celldm4": r"celldm\(4\)=\s+([\d\.]+)\s",
-        "celldm5": r"celldm\(5\)=\s+([\d\.]+)\s",
-        "celldm6": r"celldm\(6\)=\s+([\d\.]+)\s",
-        "nkpts": r"number of k points=\s+([\d]+)"
-    }
-
-    def __init__(self, filename):
-        self.filename = filename
-        self.data = defaultdict(list)
-        self.read_pattern(PWOutput.patterns)
-        for k, v in self.data.items():
-            if k == "energies":
-                self.data[k] = [float(i[0][0]) for i in v]
-            elif k in ["lattice_type", "nkpts"]:
-                self.data[k] = int(v[0][0][0])
-            else:
-                self.data[k] = float(v[0][0][0])
+        Args:
+            string (str): string representation of an Xr object.
+            use_cores (bool): use core positions and discard shell
+                    positions if set to True (default).  Otherwise,
+                    use shell positions and discard core positions.
+            thresh (float): relative threshold for consistency check
+                    between cell parameters (lengths and angles) from
+                    header information and cell vectors, respectively.
+
+        Returns:
+            xr (Xr): Xr object corresponding to the input
+                    string representation.
+        """
+        lines = string.split("\n")
+        toks = lines[0].split()
+        lengths = [float(toks[i]) for i in range(1, len(toks))]
+        toks = lines[1].split()
+        angles = [float(i) for i in toks[0:3]]
+        toks = lines[2].split()
+        nsites = int(toks[0])
+        mat = np.zeros((3,3), dtype=float)
+        for i in range(3):
+            toks = lines[4+nsites+i].split()
+            toks2 = lines[4+nsites+i+3].split()
+            for j, item in enumerate(toks):
+                if item != toks2[j]:
+                    raise RuntimeError("expected both matrices"
+                            " to be the same in xr file")
+            mat[i] = np.array([float(w) for w in toks])
+        lat = Lattice(mat)
+        if fabs(lat.a-lengths[0])/fabs(lat.a) > thresh or \
+                fabs(lat.b-lengths[1])/fabs(lat.b) > thresh or \
+                fabs(lat.c-lengths[2])/fabs(lat.c) > thresh or \
+                fabs(lat.alpha-angles[0])/fabs(lat.alpha) > thresh or \
+                fabs(lat.beta-angles[1])/fabs(lat.beta) > thresh or \
+                fabs(lat.gamma-angles[2])/fabs(lat.gamma) > thresh:
+            raise RuntimeError("cell parameters in header ("+str(lengths)+\
+                    ", "+str(angles)+") are not consistent with Cartesian"+\
+                    " lattice vectors ("+str(lat.abc)+", "+\
+                    str(lat.angles)+")")
+        # Ignore line w/ index 3.
+        sp = []
+        coords = []
+        for j in range(nsites):
+            m = re.match(r"\d+\s+(\w+)\s+([0-9\-\.]+)\s+([0-9\-\.]+)\s+" +
+                         r"([0-9\-\.]+)", lines[4+j].strip())
+            if m:
+                tmp_sp = m.group(1)
+                if use_cores and tmp_sp[len(tmp_sp)-2:] == "_s":
+                    continue
+                if not use_cores and tmp_sp[len(tmp_sp)-2:] == "_c":
+                    continue
+                if tmp_sp[len(tmp_sp)-2] == "_":
+                    sp.append(tmp_sp[0:len(tmp_sp)-2])
+                else:
+                    sp.append(tmp_sp)
+                coords.append([float(m.group(i)) for i in range(2, 5)])
+        return Xr(Structure(lat, sp, coords, coords_are_cartesian=True))
 
-    def read_pattern(self, patterns, reverse=False,
-                     terminate_on_match=False, postprocess=str):
+    @staticmethod
+    def from_file(filename, use_cores=True, thresh=1.e-4):
         """
-        General pattern reading. Uses monty's regrep method. Takes the same
-        arguments.
+        Reads an xr-formatted file to create an Xr object.
 
         Args:
-            patterns (dict): A dict of patterns, e.g.,
-                {"energy": r"energy\\(sigma->0\\)\\s+=\\s+([\\d\\-.]+)"}.
-            reverse (bool): Read files in reverse. Defaults to false. Useful for
-                large files, esp OUTCARs, especially when used with
-                terminate_on_match.
-            terminate_on_match (bool): Whether to terminate when there is at
-                least one match in each key in pattern.
-            postprocess (callable): A post processing function to convert all
-                matches. Defaults to str, i.e., no change.
-
-        Renders accessible:
-            Any attribute in patterns. For example,
-            {"energy": r"energy\\(sigma->0\\)\\s+=\s+([\\d\\-.]+)"} will set the
-            value of self.data["energy"] = [[-1234], [-3453], ...], to the
-            results from regex and postprocess. Note that the returned
-            values are lists of lists, because you can grep multiple
-            items on one line.
-        """
-        matches = regrep(self.filename, patterns, reverse=reverse,
-                         terminate_on_match=terminate_on_match,
-                         postprocess=postprocess)
-        self.data.update(matches)
-
-    def get_celldm(self, i):
-        return self.data["celldm%d" % i]
-
-    @property
-    def final_energy(self):
-        return self.data["energies"][-1]
-
-    @property
-    def lattice_type(self):
-        return self.data["lattice_type"]
+            filename (str): name of file to read from.
+            use_cores (bool): use core positions and discard shell
+                    positions if set to True (default).  Otherwise,
+                    use shell positions and discard core positions.
+            thresh (float): relative threshold for consistency check
+                    between cell parameters (lengths and angles) from
+                    header information and cell vectors, respectively.
+
+        Returns:
+            xr (Xr): Xr object corresponding to the input
+                    file.
+        """
+        with zopen(filename, "rt") as f:
+            return Xr.from_string(
+                    f.read(), use_cores=use_cores,
+                    thresh=thresh)
+
```

### Comparing `pymatgen-4.7.6/pymatgen/io/qchem.py` & `pymatgen-4.7.7/pymatgen/io/qchem.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/vasp/GWVaspInputSet.yaml` & `pymatgen-4.7.7/pymatgen/io/vasp/GWVaspInputSet.yaml`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/vasp/GWvaspinputsets.py` & `pymatgen-4.7.7/pymatgen/io/vasp/GWvaspinputsets.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/vasp/inputs.py` & `pymatgen-4.7.7/pymatgen/io/vasp/inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1041,20 +1041,20 @@
             kppa (int): Grid density
             force_gamma (bool): Force a gamma centered mesh (default is to
                 use gamma only for hexagonal cells or odd meshes)
 
         Returns:
             Kpoints
         """
-        comment = "pymatgen generated KPOINTS with grid density = " + \
-            "{} / atom".format(kppa)
+        comment = "pymatgen 4.7.6+ generated KPOINTS with grid density = " + \
+            "%.0f / atom" % kppa
         latt = structure.lattice
         lengths = latt.abc
         ngrid = kppa / structure.num_sites
-        mult = (ngrid * structure.lattice.volume) ** (1 / 3)
+        mult = (ngrid * lengths[0] * lengths[1] * lengths[2]) ** (1 / 3)
 
         num_div = [int(math.floor(max(mult / l, 1))) for l in lengths]
 
         is_hexagonal = latt.is_hexagonal()
 
         has_odd = any([i % 2 == 1 for i in num_div])
         if has_odd or is_hexagonal or force_gamma:
@@ -1093,15 +1093,15 @@
 
         # VASP documentation recommends to use even grids for n <= 8 and odd
         # grids for n > 8.
         num_div = [i + i % 2 if i <= 8 else i - i % 2 + 1 for i in num_div]
 
         style = Kpoints.supported_modes.Gamma
 
-        comment = "pymatgen generated KPOINTS with grid density = " + \
+        comment = "pymatgen 4.7.6+ generated KPOINTS with grid density = " + \
                   "{} / atom".format(kppa)
         num_kpts = 0
         return Kpoints(comment, num_kpts, style, [num_div], [0, 0, 0])
 
     @staticmethod
     def automatic_density_by_vol(structure, kppvol, force_gamma=False):
         """
@@ -1284,14 +1284,17 @@
 
         Args:
             filename (str): Filename to write to.
         """
         with zopen(filename, "wt") as f:
             f.write(self.__str__())
 
+    def __repr__(self):
+        return self.__str__()
+
     def __str__(self):
         lines = [self.comment, str(self.num_kpts), self.style.name]
         style = self.style.name.lower()[0]
         if style == "l":
             lines.append(self.coord_type)
         for i in range(len(self.kpts)):
             lines.append(" ".join([str(x) for x in self.kpts[i]]))
```

### Comparing `pymatgen-4.7.6/pymatgen/io/vasp/MITRelaxSet.yaml` & `pymatgen-4.7.7/pymatgen/io/vasp/MITRelaxSet.yaml`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/vasp/MPHSERelaxSet.yaml` & `pymatgen-4.7.7/pymatgen/io/vasp/MPHSERelaxSet.yaml`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/vasp/MPRelaxSet.yaml` & `pymatgen-4.7.7/pymatgen/io/vasp/MPRelaxSet.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     Ce: 5
     Eu: 10
   NELM: 100
   NSW: 99
   PREC: Accurate
   SIGMA: 0.05
 KPOINTS:
-  reciprocal_density: 50
+  reciprocal_density: 64
 POTCAR:
   Ac: Ac
   Ag: Ag
   Al: Al
   Ar: Ar
   As: As
   Au: Au
```

### Comparing `pymatgen-4.7.6/pymatgen/io/vasp/outputs.py` & `pymatgen-4.7.7/pymatgen/io/vasp/outputs.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/vasp/sets.py` & `pymatgen-4.7.7/pymatgen/io/vasp/sets.py`

 * *Files 0% similar despite different names*

```diff
@@ -440,27 +440,29 @@
             structure, MPHSERelaxSet.CONFIG, **kwargs)
         self.kwargs = kwargs
 
 
 class MPStaticSet(MPRelaxSet):
 
     def __init__(self, structure, prev_incar=None, prev_kpoints=None,
-                 lepsilon=False, lcalcpol=False, reciprocal_density=100, **kwargs):
+                 lepsilon=False, lcalcpol=False, reciprocal_density=100,
+                 **kwargs):
         """
         Run a static calculation.
 
         Args:
             structure (Structure): Structure from previous run.
             prev_incar (Incar): Incar file from previous run.
             prev_kpoints (Kpoints): Kpoints from previous run.
             lepsilon (bool): Whether to add static dielectric calculation
             reciprocal_density (int): For static calculations,
-                we usually set the reciprocal density by voluyme. This is a
+                we usually set the reciprocal density by volume. This is a
                 convenience arg to change that, rather than using
-                user_kpoints_settings. Defaults to 100.
+                user_kpoints_settings. Defaults to 100, which is ~50% more than
+                that of standard relaxation calculations.
             \\*\\*kwargs: kwargs supported by MPRelaxSet.
         """
         super(MPStaticSet, self).__init__(structure, **kwargs)
         if isinstance(prev_incar, six.string_types):
             prev_incar = Incar.from_file(prev_incar)
         if isinstance(prev_kpoints, six.string_types):
             prev_kpoints = Kpoints.from_file(prev_kpoints)
```

### Comparing `pymatgen-4.7.6/pymatgen/io/xcrysden.py` & `pymatgen-4.7.7/pymatgen/io/xcrysden.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/xr.py` & `pymatgen-4.7.7/pymatgen/util/io_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,164 +1,192 @@
 # coding: utf-8
 # Copyright (c) Pymatgen Development Team.
 # Distributed under the terms of the MIT License.
 
-from __future__ import division, unicode_literals
+from __future__ import unicode_literals
+import re
+import six
+import errno
+import os
+import tempfile
+import codecs
+from monty.io import zopen
 
 """
-This module provides input and output mechanisms
-for the xr file format, which is a modified CSSR
-file format and, for example, used in GULP.
-In particular, the module makes it easy
-to remove shell positions from relaxations
-that employed core-shell models.
+This module provides utility classes for io operations.
 """
 
+__author__ = "Shyue Ping Ong, Rickard Armiento, Anubhav Jain, G Matteo, Ioannis Petousis"
+__copyright__ = "Copyright 2011, The Materials Project"
+__version__ = "1.0"
+__maintainer__ = "Shyue Ping Ong"
+__email__ = "shyuep@gmail.com"
+__status__ = "Production"
+__date__ = "Sep 23, 2011"
+
+
+def ask_yesno(question, default=True):
+    try:
+        answer = six.moves.input(question)
+        return answer.lower().strip() in ["y", "yes"]
+    except EOFError:
+        return default
 
-__author__ = "Nils Edvin Richard Zimmermann"
-__copyright__ = "Copyright 2016, The Materials Project"
-__version__ = "0.1"
-__maintainer__ = "Nils Edvin Richard Zimmermann"
-__email__ = "nils.e.r.zimmermann@gmail.com"
-__date__ = "June 23, 2016"
 
-import re
+def clean_lines(string_list, remove_empty_lines=True):
+    """
+    Strips whitespace, carriage returns and empty lines from a list of strings.
 
-from six.moves import map
-import numpy as np
+    Args:
+        string_list: List of strings
+        remove_empty_lines: Set to True to skip lines which are empty after
+            stripping.
 
-from monty.io import zopen
-from math import fabs
-from pymatgen.core.lattice import Lattice
-from pymatgen.core.structure import Structure
+    Returns:
+        List of clean strings with no whitespaces.
+    """
 
-class Xr(object):
+    for s in string_list:
+        clean_s = s
+        if '#' in s:
+            ind = s.index('#')
+            clean_s = s[:ind]
+        clean_s = clean_s.strip()
+        if (not remove_empty_lines) or clean_s != '':
+            yield clean_s
+
+
+def micro_pyawk(filename, search, results=None, debug=None, postdebug=None):
     """
-    Basic object for working with xr files.
+    Small awk-mimicking search routine.
 
-    Args:
-        structure (Structure/IStructure): Structure object to create the
-                Xr object.
+    'file' is file to search through.
+    'search' is the "search program", a list of lists/tuples with 3 elements;
+    i.e. [[regex,test,run],[regex,test,run],...]
+    'results' is a an object that your search program will have access to for
+    storing results.
+
+    Here regex is either as a Regex object, or a string that we compile into a
+    Regex. test and run are callable objects.
+
+    This function goes through each line in filename, and if regex matches that
+    line *and* test(results,line)==True (or test is None) we execute
+    run(results,match),where match is the match object from running
+    Regex.match.
+
+    The default results is an empty dictionary. Passing a results object let
+    you interact with it in run() and test(). Hence, in many occasions it is
+    thus clever to use results=self.
+
+    Author: Rickard Armiento, Ioannis Petousis
+
+    Returns:
+        results
     """
+    if results is None:
+        results = {}
+
+    # Compile strings into regexs
+    for entry in search:
+        entry[0] = re.compile(entry[0])
 
-    def __init__(self, structure):
-        if not structure.is_ordered:
-            raise ValueError("Xr file can only be constructed from ordered "
-                             "structure")
-        self.structure = structure
-
-    def __str__(self):
-        output = ["pymatgen   {:.4f} {:.4f} {:.4f}"
-                  .format(*self.structure.lattice.abc),
-                  "{:.3f} {:.3f} {:.3f}"
-                  .format(*self.structure.lattice.angles),
-                  "{} 0".format(len(self.structure)),
-                  "0 {}".format(self.structure.formula)]
-        # There are actually 10 more fields per site
-        # in a typical xr file from GULP, for example.
-        for i, site in enumerate(self.structure.sites):
-            output.append("{} {} {:.4f} {:.4f} {:.4f}"
-                          .format(i + 1, site.specie, site.x, site.y, site.z))
-        mat = self.structure.lattice.matrix
-        for i in range(2):
-            for j in range(3):
-                output.append("{:.4f} {:.4f} {:.4f}".format(
-                        mat[j][0], mat[j][1], mat[j][2]))
-        return "\n".join(output)
-
-    def write_file(self, filename):
-        """
-        Write out an xr file.
-
-        Args:
-            filename (str): name of the file to write to.
-        """
-        with zopen(filename, 'wt') as f:
-            f.write(str(self) + "\n")
-
-    @staticmethod
-    def from_string(string, use_cores=True, thresh=1.e-4):
-        """
-        Creates an Xr object from a string representation.
-
-        Args:
-            string (str): string representation of an Xr object.
-            use_cores (bool): use core positions and discard shell
-                    positions if set to True (default).  Otherwise,
-                    use shell positions and discard core positions.
-            thresh (float): relative threshold for consistency check
-                    between cell parameters (lengths and angles) from
-                    header information and cell vectors, respectively.
-
-        Returns:
-            xr (Xr): Xr object corresponding to the input
-                    string representation.
-        """
-        lines = string.split("\n")
-        toks = lines[0].split()
-        lengths = [float(toks[i]) for i in range(1, len(toks))]
-        toks = lines[1].split()
-        angles = [float(i) for i in toks[0:3]]
-        toks = lines[2].split()
-        nsites = int(toks[0])
-        mat = np.zeros((3,3), dtype=float)
-        for i in range(3):
-            toks = lines[4+nsites+i].split()
-            toks2 = lines[4+nsites+i+3].split()
-            for j, item in enumerate(toks):
-                if item != toks2[j]:
-                    raise RuntimeError("expected both matrices"
-                            " to be the same in xr file")
-            mat[i] = np.array([float(w) for w in toks])
-        lat = Lattice(mat)
-        if fabs(lat.a-lengths[0])/fabs(lat.a) > thresh or \
-                fabs(lat.b-lengths[1])/fabs(lat.b) > thresh or \
-                fabs(lat.c-lengths[2])/fabs(lat.c) > thresh or \
-                fabs(lat.alpha-angles[0])/fabs(lat.alpha) > thresh or \
-                fabs(lat.beta-angles[1])/fabs(lat.beta) > thresh or \
-                fabs(lat.gamma-angles[2])/fabs(lat.gamma) > thresh:
-            raise RuntimeError("cell parameters in header ("+str(lengths)+\
-                    ", "+str(angles)+") are not consistent with Cartesian"+\
-                    " lattice vectors ("+str(lat.abc)+", "+\
-                    str(lat.angles)+")")
-        # Ignore line w/ index 3.
-        sp = []
-        coords = []
-        for j in range(nsites):
-            m = re.match(r"\d+\s+(\w+)\s+([0-9\-\.]+)\s+([0-9\-\.]+)\s+" +
-                         r"([0-9\-\.]+)", lines[4+j].strip())
-            if m:
-                tmp_sp = m.group(1)
-                if use_cores and tmp_sp[len(tmp_sp)-2:] == "_s":
-                    continue
-                if not use_cores and tmp_sp[len(tmp_sp)-2:] == "_c":
-                    continue
-                if tmp_sp[len(tmp_sp)-2] == "_":
-                    sp.append(tmp_sp[0:len(tmp_sp)-2])
-                else:
-                    sp.append(tmp_sp)
-                coords.append([float(m.group(i)) for i in range(2, 5)])
-        return Xr(Structure(lat, sp, coords, coords_are_cartesian=True))
-
-    @staticmethod
-    def from_file(filename, use_cores=True, thresh=1.e-4):
-        """
-        Reads an xr-formatted file to create an Xr object.
-
-        Args:
-            filename (str): name of file to read from.
-            use_cores (bool): use core positions and discard shell
-                    positions if set to True (default).  Otherwise,
-                    use shell positions and discard core positions.
-            thresh (float): relative threshold for consistency check
-                    between cell parameters (lengths and angles) from
-                    header information and cell vectors, respectively.
-
-        Returns:
-            xr (Xr): Xr object corresponding to the input
-                    file.
-        """
-        with zopen(filename, "rt") as f:
-            return Xr.from_string(
-                    f.read(), use_cores=use_cores,
-                    thresh=thresh)
+    with zopen(filename, "rt") as f:
+        for line in f:
+            for entry in search:
+                match = re.search(entry[0], line)
+                if match and (entry[1] is None
+                              or entry[1](results, line)):
+                    if debug is not None:
+                        debug(results, match)
+                    entry[2](results, match)
+                    if postdebug is not None:
+                        postdebug(results, match)
 
+    return results
+
+
+umask = os.umask(0)
+os.umask(umask)
+
+
+def _maketemp(name, createmode=None):
+    """
+    Create a temporary file with the filename similar the given ``name``.
+    The permission bits are copied from the original file or ``createmode``.
+    Returns: the name of the temporary file.
+    """
+    d, fn = os.path.split(name)
+    fd, tempname = tempfile.mkstemp(prefix=".%s-" % fn, dir=d)
+    os.close(fd)
+
+    # Temporary files are created with mode 0600, which is usually not
+    # what we want. If the original file already exists, just copy its mode.
+    # Otherwise, manually obey umask.
+    try:
+        st_mode = os.lstat(name).st_mode & 0o777
+    except OSError as err:
+        if err.errno != errno.ENOENT:
+            raise
+        st_mode = createmode
+        if st_mode is None:
+            st_mode = ~umask
+        st_mode &= 0o666
+    os.chmod(tempname, st_mode)
+
+    return tempname
+
+
+class AtomicFile(object):
+    """
+    This is a straight port of Alexander Saltanov's atomicfile package.
+
+    Writeable file object that atomically writes a file.
+    All writes will go to a temporary file.
+    Call ``close()`` when you are done writing, and AtomicFile will rename
+    the temporary copy to the original name, making the changes visible.
+    If the object is destroyed without being closed, all your writes are
+    discarded.
+    If an ``encoding`` argument is specified, codecs.open will be called to open
+    the file in the wanted encoding.
+    """
+    def __init__(self, name, mode="w+b", createmode=None, encoding=None):
+        self.__name = name  # permanent name
+        self._tempname = _maketemp(name, createmode=createmode)
+        if encoding:
+            self._fp = codecs.open(self._tempname, mode, encoding)
+        else:
+            self._fp = open(self._tempname, mode)
+
+        # delegated methods
+        self.write = self._fp.write
+        self.fileno = self._fp.fileno
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_value, exc_tb):
+        if exc_type:
+            return
+        self.close()
+
+    def close(self):
+        if not self._fp.closed:
+            self._fp.close()
+            # This to avoid:
+            #   FileExistsError: [WinError 183] Cannot create a file when that file already exists:
+            # On Windows, if dst already exists, OSError will be raised even if it is a file;
+            # there may be no way to implement an atomic rename when dst names an existing file.
+            if os.name == 'nt' and os.path.exists(self.__name):
+                os.remove(self.__name)
+            os.rename(self._tempname, self.__name)
+
+    def discard(self):
+        if not self._fp.closed:
+            try:
+                os.unlink(self._tempname)
+            except OSError:
+                pass
+            self._fp.close()
+
+    def __del__(self):
+        if getattr(self, "_fp", None):  # constructor actually did something
+            self.discard()
```

### Comparing `pymatgen-4.7.6/pymatgen/io/xyz.py` & `pymatgen-4.7.7/pymatgen/io/xyz.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/io/zeopp.py` & `pymatgen-4.7.7/pymatgen/io/zeopp.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/matproj/snl.py` & `pymatgen-4.7.7/pymatgen/matproj/snl.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,17 @@
 
         # turn projects into list of Strings
         projects = projects if projects else []
         self.projects = [projects] \
             if isinstance(projects, string_types) else projects
 
         # check that references are valid BibTeX
+        if not isinstance(references, string_types):
+            raise ValueError("Invalid format for SNL reference! Should be "
+                             "empty string or BibTeX string.")
         if references and not is_valid_bibtex(references):
             raise ValueError("Invalid format for SNL reference! Should be "
                              "BibTeX string.")
         if len(references) > MAX_BIBTEX_CHARS:
             raise ValueError("The BibTeX string must be fewer than {} chars "
                              ", you have {}"
                              .format(MAX_BIBTEX_CHARS, len(references)))
```

### Comparing `pymatgen-4.7.6/pymatgen/optimization/linear_assignment.c` & `pymatgen-4.7.7/pymatgen/optimization/linear_assignment.c`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/optimization/linear_assignment.pyx` & `pymatgen-4.7.7/pymatgen/optimization/linear_assignment.pyx`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/optimization/linear_assignment_numpy.py` & `pymatgen-4.7.7/pymatgen/optimization/linear_assignment_numpy.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/phasediagram/analyzer.py` & `pymatgen-4.7.7/pymatgen/phasediagram/analyzer.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/phasediagram/entries.py` & `pymatgen-4.7.7/pymatgen/phasediagram/entries.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/phasediagram/maker.py` & `pymatgen-4.7.7/pymatgen/phasediagram/maker.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/phasediagram/plotter.py` & `pymatgen-4.7.7/pymatgen/phasediagram/plotter.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/phonon/bandstructure.py` & `pymatgen-4.7.7/pymatgen/phonon/bandstructure.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/phonon/dos.py` & `pymatgen-4.7.7/pymatgen/phonon/dos.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/phonon/plotter.py` & `pymatgen-4.7.7/pymatgen/phonon/plotter.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/serializers/json_coders.py` & `pymatgen-4.7.7/pymatgen/serializers/json_coders.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/serializers/pickle_coders.py` & `pymatgen-4.7.7/pymatgen/serializers/pickle_coders.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/structure_prediction/data/lambda.json` & `pymatgen-4.7.7/pymatgen/structure_prediction/data/lambda.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/structure_prediction/data/pair_correlation.json` & `pymatgen-4.7.7/pymatgen/structure_prediction/data/pair_correlation.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/structure_prediction/substitution_probability.py` & `pymatgen-4.7.7/pymatgen/structure_prediction/substitution_probability.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/structure_prediction/substitutor.py` & `pymatgen-4.7.7/pymatgen/structure_prediction/substitutor.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/symmetry/analyzer.py` & `pymatgen-4.7.7/pymatgen/symmetry/analyzer.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/symmetry/bandstructure.py` & `pymatgen-4.7.7/pymatgen/symmetry/bandstructure.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/symmetry/groups.py` & `pymatgen-4.7.7/pymatgen/symmetry/groups.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/symmetry/structure.py` & `pymatgen-4.7.7/pymatgen/symmetry/structure.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/symmetry/symm_data.yaml` & `pymatgen-4.7.7/pymatgen/symmetry/symm_data.yaml`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/symmetry/symm_ops.json` & `pymatgen-4.7.7/pymatgen/symmetry/symm_ops.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/symmetry/symm_ops.yaml` & `pymatgen-4.7.7/pymatgen/symmetry/symm_ops.yaml`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/transformations/advanced_transformations.py` & `pymatgen-4.7.7/pymatgen/transformations/advanced_transformations.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/transformations/defect_transformations.py` & `pymatgen-4.7.7/pymatgen/transformations/defect_transformations.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/transformations/site_transformations.py` & `pymatgen-4.7.7/pymatgen/transformations/site_transformations.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/transformations/standard_transformations.py` & `pymatgen-4.7.7/pymatgen/transformations/standard_transformations.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/transformations/transformation_abc.py` & `pymatgen-4.7.7/pymatgen/transformations/transformation_abc.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/util/convergence.py` & `pymatgen-4.7.7/pymatgen/util/convergence.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/util/coord_utils.py` & `pymatgen-4.7.7/pymatgen/util/coord_utils.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/util/coord_utils_cython.c` & `pymatgen-4.7.7/pymatgen/util/coord_utils_cython.c`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/util/coord_utils_cython.pyx` & `pymatgen-4.7.7/pymatgen/util/coord_utils_cython.pyx`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/util/num.py` & `pymatgen-4.7.7/pymatgen/util/num.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/util/plotting.py` & `pymatgen-4.7.7/pymatgen/util/plotting.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/util/string.py` & `pymatgen-4.7.7/pymatgen/util/string.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/util/structures/BaNiO3.json` & `pymatgen-4.7.7/pymatgen/util/structures/BaNiO3.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/util/structures/CsCl.json` & `pymatgen-4.7.7/pymatgen/util/structures/CsCl.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/util/structures/Graphite.json` & `pymatgen-4.7.7/pymatgen/util/structures/Graphite.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/util/structures/K2O2.json` & `pymatgen-4.7.7/pymatgen/util/structures/K2O2.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/util/structures/Li10GeP2S12.json` & `pymatgen-4.7.7/pymatgen/util/structures/Li10GeP2S12.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/util/structures/Li2O.json` & `pymatgen-4.7.7/pymatgen/util/structures/Li2O.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/util/structures/Li2O2.json` & `pymatgen-4.7.7/pymatgen/util/structures/Li2O2.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/util/structures/Li3V2(PO4)3.json` & `pymatgen-4.7.7/pymatgen/util/structures/Li3V2(PO4)3.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/util/structures/LiFePO4.json` & `pymatgen-4.7.7/pymatgen/util/structures/LiFePO4.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/util/structures/NaFePO4.json` & `pymatgen-4.7.7/pymatgen/util/structures/NaFePO4.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/util/structures/Si.json` & `pymatgen-4.7.7/pymatgen/util/structures/Si.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/util/structures/Sn.json` & `pymatgen-4.7.7/pymatgen/util/structures/Sn.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/util/structures/SrTiO3.json` & `pymatgen-4.7.7/pymatgen/util/structures/SrTiO3.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/util/structures/TiO2.json` & `pymatgen-4.7.7/pymatgen/util/structures/TiO2.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/util/structures/VO2.json` & `pymatgen-4.7.7/pymatgen/util/structures/VO2.json`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/util/testing.py` & `pymatgen-4.7.7/pymatgen/util/testing.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/vis/ElementColorSchemes.yaml` & `pymatgen-4.7.7/pymatgen/vis/ElementColorSchemes.yaml`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/vis/structure_chemview.py` & `pymatgen-4.7.7/pymatgen/vis/structure_chemview.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen/vis/structure_vtk.py` & `pymatgen-4.7.7/pymatgen/vis/structure_vtk.py`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/pymatgen.egg-info/PKG-INFO` & `pymatgen-4.7.7/pymatgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pymatgen
-Version: 4.7.6
+Version: 4.7.7
 Summary: Python Materials Genomics is a robust materials analysis code that defines core object representations for structures and molecules with support for many electronic structure codes. It is currently the core analysis code powering the Materials Project (https://www.materialsproject.org).
 Home-page: http://www.pymatgen.org
 Author: Shyue Ping Ong
 Author-email: ongsp@eng.ucsd.edu
 License: MIT
 Description: 
         .. image:: https://circleci.com/gh/materialsproject/pymatgen.svg?style=shield&circle-token=:circle-token
```

### Comparing `pymatgen-4.7.6/pymatgen.egg-info/SOURCES.txt` & `pymatgen-4.7.7/pymatgen.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -305,14 +305,15 @@
 pymatgen/structure_prediction/substitutor.py
 pymatgen/structure_prediction/data/lambda.json
 pymatgen/structure_prediction/data/pair_correlation.json
 pymatgen/symmetry/__init__.py
 pymatgen/symmetry/analyzer.py
 pymatgen/symmetry/bandstructure.py
 pymatgen/symmetry/groups.py
+pymatgen/symmetry/maggroups.py
 pymatgen/symmetry/structure.py
 pymatgen/symmetry/symm_data.yaml
 pymatgen/symmetry/symm_ops.json
 pymatgen/symmetry/symm_ops.yaml
 pymatgen/transformations/__init__.py
 pymatgen/transformations/advanced_transformations.py
 pymatgen/transformations/defect_transformations.py
```

### Comparing `pymatgen-4.7.6/README.rst` & `pymatgen-4.7.7/README.rst`

 * *Files identical despite different names*

### Comparing `pymatgen-4.7.6/setup.py` & `pymatgen-4.7.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     long_desc = f.read()
     ind = long_desc.find("\n")
     long_desc = long_desc[ind + 1:]
 
 setup(
     name="pymatgen",
     packages=find_packages(),
-    version="4.7.6",
+    version="4.7.7",
     cmdclass={'build_ext': build_ext},
     setup_requires=['numpy', 'setuptools>=18.0'],
     install_requires=["numpy>=1.9", "six", "requests", "pyyaml>=3.11",
                       "monty>=0.9.6", "scipy>=0.14", "pydispatcher>=2.0.5",
                       "tabulate", "spglib>=1.9.8.7",
                       "matplotlib>=1.5", "palettable>=2.1.1", "sympy"],
     extras_require={
```

