# Comparing `tmp/mwrpy-0.1.2.tar.gz` & `tmp/mwrpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwrpy-0.1.2.tar", last modified: Tue May  2 14:19:57 2023, max compression
+gzip compressed data, was "mwrpy-0.1.3.tar", last modified: Mon May  8 13:02:03 2023, max compression
```

## Comparing `mwrpy-0.1.2.tar` & `mwrpy-0.1.3.tar`

### file list

```diff
@@ -1,73 +1,71 @@
-drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 14:19:57.665817 mwrpy-0.1.2/
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     1078 2023-03-27 10:23:04.000000 mwrpy-0.1.2/LICENSE
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)       64 2023-05-02 13:57:04.000000 mwrpy-0.1.2/MANIFEST.in
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     7016 2023-05-02 14:19:57.665817 mwrpy-0.1.2/PKG-INFO
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     6665 2023-05-02 13:40:32.000000 mwrpy-0.1.2/README.md
-drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 14:19:57.661817 mwrpy-0.1.2/mwrpy/
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)      156 2023-04-06 10:43:22.000000 mwrpy-0.1.2/mwrpy/__init__.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     4562 2023-04-11 13:40:37.000000 mwrpy-0.1.2/mwrpy/atmos.py
--rwxrwxr-x   0 tukiains  (1000) tukiains  (1000)     1939 2023-04-06 10:42:59.000000 mwrpy-0.1.2/mwrpy/cli.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)      471 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/constants.py
-drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 14:19:57.661817 mwrpy-0.1.2/mwrpy/level1/
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)       38 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/level1/__init__.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    10903 2023-05-02 12:53:20.000000 mwrpy-0.1.2/mwrpy/level1/lev1_meta_nc.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     1091 2023-03-28 08:55:18.000000 mwrpy-0.1.2/mwrpy/level1/met_quality_control.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    10143 2023-04-06 10:42:59.000000 mwrpy-0.1.2/mwrpy/level1/quality_control.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    48094 2023-05-02 13:05:25.000000 mwrpy-0.1.2/mwrpy/level1/rpg_bin.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    24760 2023-04-26 11:33:16.000000 mwrpy-0.1.2/mwrpy/level1/write_lev1_nc.py
-drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 14:19:57.661817 mwrpy-0.1.2/mwrpy/level2/
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)       38 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/level2/__init__.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    26379 2023-04-06 10:42:59.000000 mwrpy-0.1.2/mwrpy/level2/get_ret_coeff.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     8776 2023-05-02 12:53:25.000000 mwrpy-0.1.2/mwrpy/level2/lev2_meta_nc.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     4229 2023-04-06 10:42:59.000000 mwrpy-0.1.2/mwrpy/level2/lwp_offset.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    23559 2023-04-11 13:46:20.000000 mwrpy-0.1.2/mwrpy/level2/write_lev2_nc.py
-drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 14:19:57.665817 mwrpy-0.1.2/mwrpy/plots/
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)       44 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/plots/__init__.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    51855 2023-04-03 06:30:29.000000 mwrpy-0.1.2/mwrpy/plots/generate_plots.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     6938 2023-04-03 06:30:29.000000 mwrpy-0.1.2/mwrpy/plots/plot_meta.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     8292 2023-04-03 06:30:29.000000 mwrpy-0.1.2/mwrpy/plots/plot_utils.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     7674 2023-04-06 10:42:59.000000 mwrpy-0.1.2/mwrpy/process_mwrpy.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     9306 2023-04-06 10:42:59.000000 mwrpy-0.1.2/mwrpy/rpg_mwr.py
-drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 14:19:57.665817 mwrpy-0.1.2/mwrpy/site_config/
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     6234 2023-04-03 06:30:29.000000 mwrpy-0.1.2/mwrpy/site_config/hatpro.yaml
-drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 14:19:57.665817 mwrpy-0.1.2/mwrpy/site_config/hyytiala/
-drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 14:19:57.665817 mwrpy-0.1.2/mwrpy/site_config/hyytiala/coefficients/
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    33953 2023-04-03 06:30:29.000000 mwrpy-0.1.2/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    73995 2023-04-03 06:30:29.000000 mwrpy-0.1.2/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    73995 2023-04-03 06:30:29.000000 mwrpy-0.1.2/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    80385 2023-04-03 06:30:29.000000 mwrpy-0.1.2/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    39550 2023-04-03 06:30:29.000000 mwrpy-0.1.2/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     2965 2023-04-03 06:30:29.000000 mwrpy-0.1.2/mwrpy/site_config/hyytiala/config.yaml
--rw-r--r--   0 tukiains  (1000) tukiains  (1000)       12 2023-04-03 12:47:52.000000 mwrpy-0.1.2/mwrpy/site_config/hyytiala/lwp_offset_1970.csv
-drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 14:19:57.665817 mwrpy-0.1.2/mwrpy/site_config/juelich/
-drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 14:19:57.665817 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     6284 2023-03-30 13:48:57.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3100 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3100 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     3176 2023-03-27 10:20:23.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     8692 2023-03-30 13:48:57.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     6256 2023-03-30 13:48:57.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc
--rw-r--r--   0 tukiains  (1000) tukiains  (1000)       12 2023-03-31 08:32:30.000000 mwrpy-0.1.2/mwrpy/site_config/juelich/lwp_offset_1970.csv
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)    15449 2023-04-06 10:42:59.000000 mwrpy-0.1.2/mwrpy/utils.py
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)       71 2023-05-02 13:57:53.000000 mwrpy-0.1.2/mwrpy/version.py
-drwxrwxr-x   0 tukiains  (1000) tukiains  (1000)        0 2023-05-02 14:19:57.661817 mwrpy-0.1.2/mwrpy.egg-info/
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     7016 2023-05-02 14:19:57.000000 mwrpy-0.1.2/mwrpy.egg-info/PKG-INFO
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)     2460 2023-05-02 14:19:57.000000 mwrpy-0.1.2/mwrpy.egg-info/SOURCES.txt
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)        1 2023-05-02 14:19:57.000000 mwrpy-0.1.2/mwrpy.egg-info/dependency_links.txt
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)      112 2023-05-02 14:19:57.000000 mwrpy-0.1.2/mwrpy.egg-info/requires.txt
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)        6 2023-05-02 14:19:57.000000 mwrpy-0.1.2/mwrpy.egg-info/top_level.txt
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)       38 2023-05-02 14:19:57.669818 mwrpy-0.1.2/setup.cfg
--rw-rw-r--   0 tukiains  (1000) tukiains  (1000)      970 2023-04-06 10:43:22.000000 mwrpy-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:02:03.533244 mwrpy-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-08 13:01:52.000000 mwrpy-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-08 13:01:52.000000 mwrpy-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-08 13:02:03.533244 mwrpy-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-08 13:01:52.000000 mwrpy-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:02:03.529244 mwrpy-0.1.3/mwrpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/atmos.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1939 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:02:03.529244 mwrpy-0.1.3/mwrpy/level1/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/level1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/level1/lev1_meta_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/level1/met_quality_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/level1/quality_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48094 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/level1/rpg_bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24775 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/level1/write_lev1_nc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:02:03.529244 mwrpy-0.1.3/mwrpy/level2/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/level2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26379 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/level2/get_ret_coeff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/level2/lev2_meta_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/level2/lwp_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23559 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/level2/write_lev2_nc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:02:03.529244 mwrpy-0.1.3/mwrpy/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51855 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/plots/generate_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/plots/plot_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/plots/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/process_mwrpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/rpg_mwr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:02:03.529244 mwrpy-0.1.3/mwrpy/site_config/
+-rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/hatpro.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:02:03.529244 mwrpy-0.1.3/mwrpy/site_config/hyytiala/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:02:03.533244 mwrpy-0.1.3/mwrpy/site_config/hyytiala/coefficients/
+-rw-r--r--   0 runner    (1001) docker     (123)    33953 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    80385 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    39550 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/hyytiala/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:02:03.529244 mwrpy-0.1.3/mwrpy/site_config/juelich/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:02:03.533244 mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    15449 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 13:01:52.000000 mwrpy-0.1.3/mwrpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:02:03.529244 mwrpy-0.1.3/mwrpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-08 13:02:03.000000 mwrpy-0.1.3/mwrpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-08 13:02:03.000000 mwrpy-0.1.3/mwrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:02:03.000000 mwrpy-0.1.3/mwrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-08 13:02:03.000000 mwrpy-0.1.3/mwrpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 13:02:03.000000 mwrpy-0.1.3/mwrpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 13:02:03.537244 mwrpy-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-08 13:01:52.000000 mwrpy-0.1.3/setup.py
```

### Comparing `mwrpy-0.1.2/LICENSE` & `mwrpy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/PKG-INFO` & `mwrpy-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: mwrpy
-Version: 0.1.2
-Summary: Python package for Microwave Radiometer processing in ACTRIS
-Home-page: https://github.com/igmk/actris_mwr_pro
-Author: University of Cologne
-Author-email: actris-ccres-mwr@uni-koeln.de
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # MWRpy
 
 [![Tests](https://github.com/actris-cloudnet/mwrpy/actions/workflows/test.yml/badge.svg)](https://github.com/actris-cloudnet/mwrpy/actions/workflows/test.yml)
 
 ### Usage
 
 ```python
```

### Comparing `mwrpy-0.1.2/mwrpy/atmos.py` & `mwrpy-0.1.3/mwrpy/atmos.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/cli.py` & `mwrpy-0.1.3/mwrpy/cli.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/level1/lev1_meta_nc.py` & `mwrpy-0.1.3/mwrpy/level1/lev1_meta_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/level1/met_quality_control.py` & `mwrpy-0.1.3/mwrpy/level1/met_quality_control.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/level1/quality_control.py` & `mwrpy-0.1.3/mwrpy/level1/quality_control.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/level1/rpg_bin.py` & `mwrpy-0.1.3/mwrpy/level1/rpg_bin.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/level1/write_lev1_nc.py` & `mwrpy-0.1.3/mwrpy/level1/write_lev1_nc.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 
 def lev1_to_nc(
     site: str,
     data_type: str,
     path_to_files: str,
     output_file: str | None = None,
-):
+) -> rpg_mwr.Rpg:
     """This function reads one day of RPG MWR binary files,
     adds attributes and writes it into netCDF file.
 
     Args:
         site: Name of site.
         data_type: Data type of the netCDF file.
         path_to_files: Folder containing one day of RPG MWR binary files.
```

### Comparing `mwrpy-0.1.2/mwrpy/level2/get_ret_coeff.py` & `mwrpy-0.1.3/mwrpy/level2/get_ret_coeff.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/level2/lev2_meta_nc.py` & `mwrpy-0.1.3/mwrpy/level2/lev2_meta_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/level2/lwp_offset.py` & `mwrpy-0.1.3/mwrpy/level2/lwp_offset.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/level2/write_lev2_nc.py` & `mwrpy-0.1.3/mwrpy/level2/write_lev2_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/plots/generate_plots.py` & `mwrpy-0.1.3/mwrpy/plots/generate_plots.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/plots/plot_meta.py` & `mwrpy-0.1.3/mwrpy/plots/plot_meta.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/plots/plot_utils.py` & `mwrpy-0.1.3/mwrpy/plots/plot_utils.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/process_mwrpy.py` & `mwrpy-0.1.3/mwrpy/process_mwrpy.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/rpg_mwr.py` & `mwrpy-0.1.3/mwrpy/rpg_mwr.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/hatpro.yaml` & `mwrpy-0.1.3/mwrpy/site_config/hatpro.yaml`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.1.3/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.1.3/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.1.3/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.1.3/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.1.3/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/hyytiala/config.yaml` & `mwrpy-0.1.3/mwrpy/site_config/hyytiala/config.yaml`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc` & `mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc` & `mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc` & `mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc` & `mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc` & `mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc` & `mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc` & `mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc` & `mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc` & `mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc` & `mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc` & `mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc` & `mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc` & `mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc` & `mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc` & `mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc` & `mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc` & `mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc` & `mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc` & `mwrpy-0.1.3/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy/utils.py` & `mwrpy-0.1.3/mwrpy/utils.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.2/mwrpy.egg-info/SOURCES.txt` & `mwrpy-0.1.3/mwrpy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -28,21 +28,19 @@
 mwrpy/level2/write_lev2_nc.py
 mwrpy/plots/__init__.py
 mwrpy/plots/generate_plots.py
 mwrpy/plots/plot_meta.py
 mwrpy/plots/plot_utils.py
 mwrpy/site_config/hatpro.yaml
 mwrpy/site_config/hyytiala/config.yaml
-mwrpy/site_config/hyytiala/lwp_offset_1970.csv
 mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
 mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
 mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
 mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret
 mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
-mwrpy/site_config/juelich/lwp_offset_1970.csv
 mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc
 mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc
 mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc
 mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc
 mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc
 mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc
 mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc
```

### Comparing `mwrpy-0.1.2/setup.py` & `mwrpy-0.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     name="mwrpy",
     version=version["__version__"],
     description="Python package for Microwave Radiometer processing in ACTRIS",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="University of Cologne",
     author_email="actris-ccres-mwr@uni-koeln.de",
-    url="https://github.com/igmk/actris_mwr_pro",
+    url="https://github.com/actris-cloudnet/mwrpy",
     packages=find_packages(),
     include_package_data=True,
     python_requires=">=3.10",
     install_requires=[
         "scipy",
         "netCDF4",
         "matplotlib",
```

