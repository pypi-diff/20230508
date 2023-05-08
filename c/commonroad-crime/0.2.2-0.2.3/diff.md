# Comparing `tmp/commonroad-crime-0.2.2.tar.gz` & `tmp/commonroad-crime-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/commonroad-crime-0.2.2.tar", last modified: Wed May  3 07:03:07 2023, max compression
+gzip compressed data, was "dist/commonroad-crime-0.2.3.tar", last modified: Mon May  8 07:15:30 2023, max compression
```

## Comparing `commonroad-crime-0.2.2.tar` & `commonroad-crime-0.2.3.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 07:03:07.000000 commonroad-crime-0.2.2/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1570 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/LICENSE
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      301 2023-05-03 07:03:07.000000 commonroad-crime-0.2.2/PKG-INFO
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4564 2023-04-09 12:14:11.000000 commonroad-crime-0.2.2/README.md
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 07:03:07.000000 commonroad-crime-0.2.2/commonroad_crime/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:41:04.000000 commonroad-crime-0.2.2/commonroad_crime/__init__.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 07:03:07.000000 commonroad-crime-0.2.2/commonroad_crime/data_structure/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:41:04.000000 commonroad-crime-0.2.2/commonroad_crime/data_structure/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     8736 2023-04-19 15:18:31.000000 commonroad-crime-0.2.2/commonroad_crime/data_structure/base.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 07:03:07.000000 commonroad-crime-0.2.2/commonroad_crime/data_structure/config_defaults/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:41:04.000000 commonroad-crime-0.2.2/commonroad_crime/data_structure/config_defaults/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    10783 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/data_structure/configuration.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4835 2023-04-02 10:41:04.000000 commonroad-crime-0.2.2/commonroad_crime/data_structure/configuration_builder.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3975 2023-04-04 14:41:32.000000 commonroad-crime-0.2.2/commonroad_crime/data_structure/crime_interface.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1898 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/data_structure/scene.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2681 2023-04-06 16:10:49.000000 commonroad-crime-0.2.2/commonroad_crime/data_structure/type.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 07:03:07.000000 commonroad-crime-0.2.2/commonroad_crime/measure/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1209 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/__init__.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 07:03:07.000000 commonroad-crime-0.2.2/commonroad_crime/measure/acceleration/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/acceleration/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5291 2023-04-20 08:47:33.000000 commonroad-crime-0.2.2/commonroad_crime/measure/acceleration/a_lat_req.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4420 2023-04-04 13:51:42.000000 commonroad-crime-0.2.2/commonroad_crime/measure/acceleration/a_long_req.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1944 2023-04-02 10:41:04.000000 commonroad-crime-0.2.2/commonroad_crime/measure/acceleration/a_req.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2633 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/acceleration/dst.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 07:03:07.000000 commonroad-crime-0.2.2/commonroad_crime/measure/distance/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/distance/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4425 2023-04-07 09:40:31.000000 commonroad-crime-0.2.2/commonroad_crime/measure/distance/dce.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3326 2023-04-19 08:48:11.000000 commonroad-crime-0.2.2/commonroad_crime/measure/distance/hw.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      980 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/distance/msd.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      980 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/distance/psd.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 07:03:07.000000 commonroad-crime-0.2.2/commonroad_crime/measure/index/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/index/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      974 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/index/aci.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2147 2023-04-04 14:10:05.000000 commonroad-crime-0.2.2/commonroad_crime/measure/index/btn.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      971 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/index/ci.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      974 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/index/cpi.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      974 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/index/pri.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      974 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/index/rss.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      974 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/index/soi.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2079 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/index/stn.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2827 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/index/tci.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 07:03:07.000000 commonroad-crime-0.2.2/commonroad_crime/measure/jerk/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/jerk/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1875 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/jerk/lat_j.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1957 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/jerk/long_j.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 07:03:07.000000 commonroad-crime-0.2.2/commonroad_crime/measure/potential/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/potential/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    13780 2023-04-04 14:43:20.000000 commonroad-crime-0.2.2/commonroad_crime/measure/potential/pf.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      979 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/potential/sp.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 07:03:07.000000 commonroad-crime-0.2.2/commonroad_crime/measure/probability/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/probability/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6753 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/probability/p_mc.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      992 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/probability/p_smh.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      992 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/probability/p_srs.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 07:03:07.000000 commonroad-crime-0.2.2/commonroad_crime/measure/reachable_set/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/reachable_set/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4617 2023-04-20 08:47:33.000000 commonroad-crime-0.2.2/commonroad_crime/measure/reachable_set/drivable_area.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 07:03:07.000000 commonroad-crime-0.2.2/commonroad_crime/measure/time/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/time/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      972 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/time/ags.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      969 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/time/et.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      972 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/time/pet.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      975 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/time/pttc.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      969 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/time/tc.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1578 2023-04-02 11:49:42.000000 commonroad-crime-0.2.2/commonroad_crime/measure/time/tet.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4298 2023-04-04 12:29:51.000000 commonroad-crime-0.2.2/commonroad_crime/measure/time/thw.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3495 2023-04-02 11:31:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/time/tit.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      629 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/time/ttb.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5797 2023-04-20 08:59:04.000000 commonroad-crime-0.2.2/commonroad_crime/measure/time/ttc.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6296 2023-05-03 06:44:51.000000 commonroad-crime-0.2.2/commonroad_crime/measure/time/ttc_star.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1988 2023-04-09 11:48:02.000000 commonroad-crime-0.2.2/commonroad_crime/measure/time/ttce.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      627 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/time/ttk.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6641 2023-04-20 14:19:33.000000 commonroad-crime-0.2.2/commonroad_crime/measure/time/ttm.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2250 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/time/ttr.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2370 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/time/tts.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6173 2023-04-02 10:41:04.000000 commonroad-crime-0.2.2/commonroad_crime/measure/time/ttz.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      969 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/time/tv.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5478 2023-05-03 06:44:51.000000 commonroad-crime-0.2.2/commonroad_crime/measure/time/wttc.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5879 2023-04-09 11:45:45.000000 commonroad-crime-0.2.2/commonroad_crime/measure/time/wttr.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 07:03:07.000000 commonroad-crime-0.2.2/commonroad_crime/measure/velocity/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)       28 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/velocity/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      977 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/measure/velocity/cs.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2782 2023-04-04 13:51:42.000000 commonroad-crime-0.2.2/commonroad_crime/measure/velocity/delta_v.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 07:03:07.000000 commonroad-crime-0.2.2/commonroad_crime/utility/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:41:04.000000 commonroad-crime-0.2.2/commonroad_crime/utility/__init__.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5829 2023-04-02 10:41:04.000000 commonroad-crime-0.2.2/commonroad_crime/utility/batch_evaluation.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5356 2023-04-20 09:32:40.000000 commonroad-crime-0.2.2/commonroad_crime/utility/general.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1855 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/commonroad_crime/utility/logger.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     8945 2023-04-02 10:41:04.000000 commonroad-crime-0.2.2/commonroad_crime/utility/optimization.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    25642 2023-04-20 09:31:14.000000 commonroad-crime-0.2.2/commonroad_crime/utility/simulation.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     9390 2023-04-19 08:46:38.000000 commonroad-crime-0.2.2/commonroad_crime/utility/solver.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     8546 2023-04-23 07:37:21.000000 commonroad-crime-0.2.2/commonroad_crime/utility/visualization.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 07:03:07.000000 commonroad-crime-0.2.2/commonroad_crime.egg-info/
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      301 2023-05-03 07:03:06.000000 commonroad-crime-0.2.2/commonroad_crime.egg-info/PKG-INFO
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     3605 2023-05-03 07:03:06.000000 commonroad-crime-0.2.2/commonroad_crime.egg-info/SOURCES.txt
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        1 2023-05-03 07:03:06.000000 commonroad-crime-0.2.2/commonroad_crime.egg-info/dependency_links.txt
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      253 2023-05-03 07:03:06.000000 commonroad-crime-0.2.2/commonroad_crime.egg-info/requires.txt
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       17 2023-05-03 07:03:06.000000 commonroad-crime-0.2.2/commonroad_crime.egg-info/top_level.txt
--rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       38 2023-05-03 07:03:07.000000 commonroad-crime-0.2.2/setup.cfg
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      887 2023-05-03 07:02:22.000000 commonroad-crime-0.2.2/setup.py
-drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-03 07:03:07.000000 commonroad-crime-0.2.2/tests/
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1674 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/tests/test_acceleration_domain.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      981 2022-11-01 14:27:06.000000 commonroad-crime-0.2.2/tests/test_base.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1143 2023-04-05 14:45:46.000000 commonroad-crime-0.2.2/tests/test_distance_domain.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1493 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/tests/test_index_domain.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1393 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/tests/test_jerk_domain.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      801 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/tests/test_potential_domain.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      855 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/tests/test_probability_domain.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      968 2023-04-09 11:42:41.000000 commonroad-crime-0.2.2/tests/test_reachable_set_domain.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6635 2023-05-03 06:44:51.000000 commonroad-crime-0.2.2/tests/test_time_domain.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6519 2023-04-20 08:59:04.000000 commonroad-crime-0.2.2/tests/test_utils_simulation.py
--rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      787 2023-04-02 10:40:15.000000 commonroad-crime-0.2.2/tests/test_velocity_domain.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1570 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/LICENSE
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      301 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/PKG-INFO
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4564 2023-04-09 12:14:11.000000 commonroad-crime-0.2.3/README.md
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/commonroad_crime/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:41:04.000000 commonroad-crime-0.2.3/commonroad_crime/__init__.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/commonroad_crime/data_structure/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:41:04.000000 commonroad-crime-0.2.3/commonroad_crime/data_structure/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     8736 2023-04-19 15:18:31.000000 commonroad-crime-0.2.3/commonroad_crime/data_structure/base.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/commonroad_crime/data_structure/config_defaults/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:41:04.000000 commonroad-crime-0.2.3/commonroad_crime/data_structure/config_defaults/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    10783 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/data_structure/configuration.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4788 2023-05-08 07:13:52.000000 commonroad-crime-0.2.3/commonroad_crime/data_structure/configuration_builder.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3975 2023-04-04 14:41:32.000000 commonroad-crime-0.2.3/commonroad_crime/data_structure/crime_interface.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1898 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/data_structure/scene.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2681 2023-04-06 16:10:49.000000 commonroad-crime-0.2.3/commonroad_crime/data_structure/type.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/commonroad_crime/measure/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1209 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/__init__.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/commonroad_crime/measure/acceleration/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/acceleration/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5291 2023-04-20 08:47:33.000000 commonroad-crime-0.2.3/commonroad_crime/measure/acceleration/a_lat_req.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4420 2023-04-04 13:51:42.000000 commonroad-crime-0.2.3/commonroad_crime/measure/acceleration/a_long_req.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1944 2023-04-02 10:41:04.000000 commonroad-crime-0.2.3/commonroad_crime/measure/acceleration/a_req.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2633 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/acceleration/dst.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/commonroad_crime/measure/distance/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/distance/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4425 2023-04-07 09:40:31.000000 commonroad-crime-0.2.3/commonroad_crime/measure/distance/dce.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3326 2023-04-19 08:48:11.000000 commonroad-crime-0.2.3/commonroad_crime/measure/distance/hw.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      980 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/distance/msd.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      980 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/distance/psd.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/commonroad_crime/measure/index/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/index/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      974 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/index/aci.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2147 2023-04-04 14:10:05.000000 commonroad-crime-0.2.3/commonroad_crime/measure/index/btn.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      971 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/index/ci.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      974 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/index/cpi.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      974 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/index/pri.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      974 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/index/rss.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      974 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/index/soi.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2079 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/index/stn.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2827 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/index/tci.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/commonroad_crime/measure/jerk/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/jerk/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1875 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/jerk/lat_j.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1957 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/jerk/long_j.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/commonroad_crime/measure/potential/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/potential/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    13780 2023-04-04 14:43:20.000000 commonroad-crime-0.2.3/commonroad_crime/measure/potential/pf.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      979 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/potential/sp.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/commonroad_crime/measure/probability/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/probability/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6753 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/probability/p_mc.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      992 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/probability/p_smh.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      992 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/probability/p_srs.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/commonroad_crime/measure/reachable_set/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/reachable_set/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4617 2023-04-20 08:47:33.000000 commonroad-crime-0.2.3/commonroad_crime/measure/reachable_set/drivable_area.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/commonroad_crime/measure/time/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/time/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      972 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/time/ags.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      969 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/time/et.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      972 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/time/pet.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      975 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/time/pttc.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      969 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/time/tc.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1578 2023-04-02 11:49:42.000000 commonroad-crime-0.2.3/commonroad_crime/measure/time/tet.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     4298 2023-04-04 12:29:51.000000 commonroad-crime-0.2.3/commonroad_crime/measure/time/thw.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     3495 2023-04-02 11:31:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/time/tit.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      629 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/time/ttb.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5797 2023-04-20 08:59:04.000000 commonroad-crime-0.2.3/commonroad_crime/measure/time/ttc.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6296 2023-05-03 06:44:51.000000 commonroad-crime-0.2.3/commonroad_crime/measure/time/ttc_star.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1988 2023-04-09 11:48:02.000000 commonroad-crime-0.2.3/commonroad_crime/measure/time/ttce.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      627 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/time/ttk.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6641 2023-04-20 14:19:33.000000 commonroad-crime-0.2.3/commonroad_crime/measure/time/ttm.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2250 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/time/ttr.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2370 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/time/tts.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6173 2023-04-02 10:41:04.000000 commonroad-crime-0.2.3/commonroad_crime/measure/time/ttz.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      969 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/time/tv.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5478 2023-05-03 06:44:51.000000 commonroad-crime-0.2.3/commonroad_crime/measure/time/wttc.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5879 2023-04-09 11:45:45.000000 commonroad-crime-0.2.3/commonroad_crime/measure/time/wttr.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/commonroad_crime/measure/velocity/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)       28 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/velocity/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      977 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/measure/velocity/cs.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     2782 2023-04-04 13:51:42.000000 commonroad-crime-0.2.3/commonroad_crime/measure/velocity/delta_v.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/commonroad_crime/utility/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)        0 2023-04-02 10:41:04.000000 commonroad-crime-0.2.3/commonroad_crime/utility/__init__.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5829 2023-04-02 10:41:04.000000 commonroad-crime-0.2.3/commonroad_crime/utility/batch_evaluation.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     5356 2023-04-20 09:32:40.000000 commonroad-crime-0.2.3/commonroad_crime/utility/general.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1855 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/commonroad_crime/utility/logger.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     8945 2023-04-02 10:41:04.000000 commonroad-crime-0.2.3/commonroad_crime/utility/optimization.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)    25672 2023-05-07 15:43:07.000000 commonroad-crime-0.2.3/commonroad_crime/utility/simulation.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     9390 2023-04-19 08:46:38.000000 commonroad-crime-0.2.3/commonroad_crime/utility/solver.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     8546 2023-04-23 07:37:21.000000 commonroad-crime-0.2.3/commonroad_crime/utility/visualization.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/commonroad_crime.egg-info/
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      301 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/commonroad_crime.egg-info/PKG-INFO
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)     3605 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/commonroad_crime.egg-info/SOURCES.txt
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)        1 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/commonroad_crime.egg-info/dependency_links.txt
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)      253 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/commonroad_crime.egg-info/requires.txt
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       17 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/commonroad_crime.egg-info/top_level.txt
+-rw-rw-r--   0 yuanfei   (1000) yuanfei   (1000)       38 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/setup.cfg
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      887 2023-05-08 07:13:39.000000 commonroad-crime-0.2.3/setup.py
+drwxrwxr-x   0 yuanfei   (1000) yuanfei   (1000)        0 2023-05-08 07:15:30.000000 commonroad-crime-0.2.3/tests/
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1674 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/tests/test_acceleration_domain.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      981 2022-11-01 14:27:06.000000 commonroad-crime-0.2.3/tests/test_base.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1143 2023-04-05 14:45:46.000000 commonroad-crime-0.2.3/tests/test_distance_domain.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1493 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/tests/test_index_domain.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     1393 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/tests/test_jerk_domain.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      801 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/tests/test_potential_domain.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      855 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/tests/test_probability_domain.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      968 2023-04-09 11:42:41.000000 commonroad-crime-0.2.3/tests/test_reachable_set_domain.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6635 2023-05-03 06:44:51.000000 commonroad-crime-0.2.3/tests/test_time_domain.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)     6519 2023-04-20 08:59:04.000000 commonroad-crime-0.2.3/tests/test_utils_simulation.py
+-rw-r--r--   0 yuanfei   (1000) yuanfei   (1000)      787 2023-04-02 10:40:15.000000 commonroad-crime-0.2.3/tests/test_velocity_domain.py
```

### Comparing `commonroad-crime-0.2.2/LICENSE` & `commonroad-crime-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/README.md` & `commonroad-crime-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/data_structure/base.py` & `commonroad-crime-0.2.3/commonroad_crime/data_structure/base.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/data_structure/configuration.py` & `commonroad-crime-0.2.3/commonroad_crime/data_structure/configuration.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/data_structure/configuration_builder.py` & `commonroad-crime-0.2.3/commonroad_crime/data_structure/configuration_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.0.1"
+__version__ = "0.2.3"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "Pre-alpha"
 
 import glob
 import os
 from typing import Union
-import pkg_resources
 from omegaconf import OmegaConf, ListConfig, DictConfig
 
 from commonroad_crime.data_structure.configuration import CriMeConfiguration
 
 class ConfigurationBuilder:
     path_root: str = None
     path_config: str = None
@@ -65,18 +64,19 @@
     def construct_default_configuration(cls) -> Union[ListConfig, DictConfig]:
         """Constructs default configuration by accumulating yaml files.
 
         Collects all configuration files ending with '.yaml'.
         """
         config_default = OmegaConf.create()
         if cls.path_config_default == "":
-            resource_dir = 'commonroad_crime.data_structure.config_defaults'
-            path_file_all = pkg_resources.resource_listdir(resource_dir, '')
-            path_file_all = [pkg_resources.resource_filename(resource_dir, filename) for filename in path_file_all if
-                             filename.endswith('.yaml')]
+
+            resource_dir = os.path.dirname(os.path.realpath(__file__)) + '/config_defaults/'
+            path_file_all = os.listdir(resource_dir)
+            path_file_all = [os.path.join(resource_dir, filename)
+                             for filename in path_file_all if filename.endswith('.yaml')]
         else:
             path_file_all = glob.glob(cls.path_config_default + "/*.yaml")
         for path_file in path_file_all:
             with open(path_file, "r") as file_config:
                 try:
                     config_partial = OmegaConf.load(file_config)
                     name_file = path_file.split("/")[-1].split(".")[0]
```

### Comparing `commonroad-crime-0.2.2/commonroad_crime/data_structure/crime_interface.py` & `commonroad-crime-0.2.3/commonroad_crime/data_structure/crime_interface.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/data_structure/scene.py` & `commonroad-crime-0.2.3/commonroad_crime/data_structure/scene.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/data_structure/type.py` & `commonroad-crime-0.2.3/commonroad_crime/data_structure/type.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/__init__.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/acceleration/a_lat_req.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/acceleration/a_lat_req.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/acceleration/a_long_req.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/acceleration/a_long_req.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/acceleration/a_req.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/acceleration/a_req.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/acceleration/dst.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/acceleration/dst.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/distance/dce.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/distance/dce.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/distance/hw.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/distance/hw.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/distance/msd.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/distance/msd.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/distance/psd.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/distance/psd.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/index/aci.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/index/aci.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/index/btn.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/index/btn.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/index/ci.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/index/ci.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/index/cpi.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/index/cpi.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/index/pri.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/index/pri.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/index/rss.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/index/rss.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/index/soi.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/index/soi.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/index/stn.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/index/stn.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/index/tci.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/index/tci.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/jerk/lat_j.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/jerk/lat_j.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/jerk/long_j.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/jerk/long_j.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/potential/pf.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/potential/pf.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/potential/sp.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/potential/sp.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/probability/p_mc.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/probability/p_mc.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/probability/p_smh.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/probability/p_smh.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/probability/p_srs.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/probability/p_srs.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/reachable_set/drivable_area.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/reachable_set/drivable_area.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/time/ags.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/time/ags.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/time/et.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/time/et.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/time/pet.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/time/pet.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/time/pttc.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/time/pttc.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/time/tc.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/time/tc.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/time/tet.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/time/tet.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/time/thw.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/time/thw.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/time/tit.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/time/tit.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/time/ttb.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/time/ttb.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/time/ttc.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/time/ttc.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/time/ttc_star.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/time/ttc_star.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/time/ttce.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/time/ttce.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/time/ttk.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/time/ttk.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/time/ttm.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/time/ttm.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/time/ttr.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/time/ttr.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/time/tts.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/time/tts.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/time/ttz.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/time/ttz.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/time/tv.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/time/tv.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/time/wttc.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/time/wttc.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/time/wttr.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/time/wttr.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/velocity/cs.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/velocity/cs.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/measure/velocity/delta_v.py` & `commonroad-crime-0.2.3/commonroad_crime/measure/velocity/delta_v.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/utility/batch_evaluation.py` & `commonroad-crime-0.2.3/commonroad_crime/utility/batch_evaluation.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/utility/general.py` & `commonroad-crime-0.2.3/commonroad_crime/utility/general.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/utility/logger.py` & `commonroad-crime-0.2.3/commonroad_crime/utility/logger.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/utility/optimization.py` & `commonroad-crime-0.2.3/commonroad_crime/utility/optimization.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/utility/simulation.py` & `commonroad-crime-0.2.3/commonroad_crime/utility/simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
     Simulate the trajectory in the longitudinal direction.
     """
 
     def __init__(self,
                  maneuver: Union[Maneuver],
                  simulated_vehicle: DynamicObstacle,
                  config: CriMeConfiguration):
-        if maneuver not in [Maneuver.BRAKE, Maneuver.KICKDOWN, Maneuver.CONSTANT, Maneuver.STOPMC]:
+        if maneuver not in [Maneuver.BRAKE, Maneuver.KICKDOWN, Maneuver.CONSTANT, Maneuver.STOPMC, Maneuver.NONE]:
             raise ValueError(
                 f"<Criticality/Simulation>: provided maneuver {maneuver} is not supported or goes to the wrong category")
         super(SimulationLong, self).__init__(maneuver, simulated_vehicle, config)
 
     def set_a_long_and_a_lat(self, ref_state: PMState):
         # set the lateral acceleration to 0
         self.a_lat = 0
@@ -310,15 +310,15 @@
                  maneuver: Maneuver,
                  simulated_vehicle: DynamicObstacle,
                  config: CriMeConfiguration):
         if maneuver not in [Maneuver.STEERLEFT, Maneuver.STEERRIGHT,
                             Maneuver.OVERTAKELEFT, Maneuver.OVERTAKERIGHT,
                             Maneuver.TURNLEFT, Maneuver.TURNRIGHT,
                             Maneuver.LANECHANGEMC, Maneuver.TURNMC,
-                            Maneuver.OVERTAKEMC]:
+                            Maneuver.OVERTAKEMC, Maneuver.NONE]:
             raise ValueError(
                 f"<Criticality/Simulation>: provided maneuver {maneuver} is not supported or goes to the wrong category")
         self._nr_stage = 0
         self._scenario = config.scenario
         self._lateral_distance_mode = config.time.steer_width
         self._direction = 'left'  # 'right'
         super(SimulationLat, self).__init__(maneuver, simulated_vehicle, config)
```

### Comparing `commonroad-crime-0.2.2/commonroad_crime/utility/solver.py` & `commonroad-crime-0.2.3/commonroad_crime/utility/solver.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime/utility/visualization.py` & `commonroad-crime-0.2.3/commonroad_crime/utility/visualization.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/commonroad_crime.egg-info/SOURCES.txt` & `commonroad-crime-0.2.3/commonroad_crime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/setup.py` & `commonroad-crime-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(name='commonroad-crime',
-      version='0.2.2',
+      version='0.2.3',
       description='criticality measures of automated vehicles',
       keywords="criticality, autonomous driving",
       author='Yuanfei Lin, Oliver Specht, Ivana Peneva',
       author_email='yuanfei.lin@tum.de',
       license='BSD 3-Clause',
       packages=find_packages(),
       install_requires=[
```

### Comparing `commonroad-crime-0.2.2/tests/test_acceleration_domain.py` & `commonroad-crime-0.2.3/tests/test_acceleration_domain.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/tests/test_base.py` & `commonroad-crime-0.2.3/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/tests/test_distance_domain.py` & `commonroad-crime-0.2.3/tests/test_distance_domain.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/tests/test_index_domain.py` & `commonroad-crime-0.2.3/tests/test_index_domain.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/tests/test_jerk_domain.py` & `commonroad-crime-0.2.3/tests/test_jerk_domain.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/tests/test_potential_domain.py` & `commonroad-crime-0.2.3/tests/test_potential_domain.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/tests/test_probability_domain.py` & `commonroad-crime-0.2.3/tests/test_probability_domain.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/tests/test_reachable_set_domain.py` & `commonroad-crime-0.2.3/tests/test_reachable_set_domain.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/tests/test_time_domain.py` & `commonroad-crime-0.2.3/tests/test_time_domain.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/tests/test_utils_simulation.py` & `commonroad-crime-0.2.3/tests/test_utils_simulation.py`

 * *Files identical despite different names*

### Comparing `commonroad-crime-0.2.2/tests/test_velocity_domain.py` & `commonroad-crime-0.2.3/tests/test_velocity_domain.py`

 * *Files identical despite different names*

