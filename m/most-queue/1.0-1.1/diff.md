# Comparing `tmp/most_queue-1.0.tar.gz` & `tmp/most-queue-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "most_queue-1.0.tar", last modified: Wed Jan 25 13:18:13 2023, max compression
+gzip compressed data, was "most-queue-1.1.tar", last modified: Mon May  8 07:41:53 2023, max compression
```

## Comparing `most_queue-1.0.tar` & `most-queue-1.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-01-25 13:18:13.094710 most_queue-1.0/
--rw-rw-rw-   0        0        0     1091 2022-09-15 10:35:18.000000 most_queue-1.0/LICENSE
--rw-rw-rw-   0        0        0     6117 2023-01-25 13:18:13.092839 most_queue-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4326 2022-12-01 21:12:39.000000 most_queue-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-01-25 13:18:12.380394 most_queue-1.0/most_queue/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.0/most_queue/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-25 13:18:12.462878 most_queue-1.0/most_queue/sim/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:45:51.000000 most_queue-1.0/most_queue/sim/__init__.py
--rw-rw-rw-   0        0        0    14664 2022-09-15 16:47:38.000000 most_queue-1.0/most_queue/sim/fj_delta_im.py
--rw-rw-rw-   0        0        0    11132 2022-09-23 20:35:51.000000 most_queue-1.0/most_queue/sim/fj_im.py
--rw-rw-rw-   0        0        0    10099 2022-09-15 12:02:16.000000 most_queue-1.0/most_queue/sim/flow_sum_im.py
--rw-rw-rw-   0        0        0    10619 2022-12-01 20:31:07.000000 most_queue-1.0/most_queue/sim/network_im_prty.py
--rw-rw-rw-   0        0        0    13161 2022-11-30 19:30:09.000000 most_queue-1.0/most_queue/sim/queue_finite_source_sim.py
--rw-rw-rw-   0        0        0    37331 2023-01-25 13:05:08.000000 most_queue-1.0/most_queue/sim/rand_destribution.py
--rw-rw-rw-   0        0        0     3913 2022-11-30 19:31:29.000000 most_queue-1.0/most_queue/sim/smo_batch_sim.py
--rw-rw-rw-   0        0        0    25978 2022-11-30 17:51:13.000000 most_queue-1.0/most_queue/sim/smo_im.py
--rw-rw-rw-   0        0        0    39946 2022-09-25 20:15:14.000000 most_queue-1.0/most_queue/sim/smo_im_prty.py
--rw-rw-rw-   0        0        0     7724 2022-11-29 20:49:52.000000 most_queue-1.0/most_queue/sim/smo_impatient_im.py
-drwxrwxrwx   0        0        0        0 2023-01-25 13:18:12.702030 most_queue-1.0/most_queue/tests/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.0/most_queue/tests/__init__.py
--rw-rw-rw-   0        0        0     3826 2022-09-16 06:55:00.000000 most_queue-1.0/most_queue/tests/ek_d_n.py
--rw-rw-rw-   0        0        0     4997 2022-09-16 07:21:38.000000 most_queue-1.0/most_queue/tests/fj_calc.py
--rw-rw-rw-   0        0        0     5539 2022-09-16 07:43:39.000000 most_queue-1.0/most_queue/tests/fj_im.py
--rw-rw-rw-   0        0        0     4278 2022-09-16 07:57:31.000000 most_queue-1.0/most_queue/tests/flow_sum.py
--rw-rw-rw-   0        0        0     5122 2022-09-16 08:17:30.000000 most_queue-1.0/most_queue/tests/gi_m_1_calc.py
--rw-rw-rw-   0        0        0     5258 2022-09-16 08:17:30.000000 most_queue-1.0/most_queue/tests/gi_m_n_calc.py
--rw-rw-rw-   0        0        0     2255 2022-09-16 08:20:45.000000 most_queue-1.0/most_queue/tests/m_d_n_calc.py
--rw-rw-rw-   0        0        0     6712 2022-09-16 08:52:49.000000 most_queue-1.0/most_queue/tests/m_ph_n_prty.py
--rw-rw-rw-   0        0        0     5267 2022-09-20 18:59:53.000000 most_queue-1.0/most_queue/tests/mg1_calc.py
--rw-rw-rw-   0        0        0      982 2022-09-15 18:04:48.000000 most_queue-1.0/most_queue/tests/mg1_warm_calc.py
--rw-rw-rw-   0        0        0     4743 2022-09-25 20:12:58.000000 most_queue-1.0/most_queue/tests/mgn_tt.py
--rw-rw-rw-   0        0        0     3337 2022-09-15 18:04:48.000000 most_queue-1.0/most_queue/tests/mmn3_pnz_cox_approx.py
--rw-rw-rw-   0        0        0     2830 2022-09-15 18:04:48.000000 most_queue-1.0/most_queue/tests/mmn_prty_pnz_approx.py
--rw-rw-rw-   0        0        0     8149 2022-09-23 20:18:42.000000 most_queue-1.0/most_queue/tests/network_im_prty.py
--rw-rw-rw-   0        0        0    17534 2022-09-15 18:04:48.000000 most_queue-1.0/most_queue/tests/passage_time.py
--rw-rw-rw-   0        0        0     2744 2022-09-23 19:56:01.000000 most_queue-1.0/most_queue/tests/smo_im.py
--rw-rw-rw-   0        0        0     6545 2022-09-23 20:18:42.000000 most_queue-1.0/most_queue/tests/smo_im_prty.py
--rw-rw-rw-   0        0        0      967 2022-09-16 08:52:49.000000 most_queue-1.0/most_queue/tests/weibull.py
-drwxrwxrwx   0        0        0        0 2023-01-25 13:18:13.021646 most_queue-1.0/most_queue/theory/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:45:51.000000 most_queue-1.0/most_queue/theory/__init__.py
--rw-rw-rw-   0        0        0     2092 2022-09-15 12:02:16.000000 most_queue-1.0/most_queue/theory/approx_cdf_make.py
--rw-rw-rw-   0        0        0     2360 2022-11-30 18:00:26.000000 most_queue-1.0/most_queue/theory/batch_mm1.py
--rw-rw-rw-   0        0        0     1304 2022-09-15 11:45:51.000000 most_queue-1.0/most_queue/theory/diff5dots.py
--rw-rw-rw-   0        0        0     6193 2022-09-15 16:51:31.000000 most_queue-1.0/most_queue/theory/ek_d_n_calc.py
--rw-rw-rw-   0        0        0     4760 2022-11-30 19:14:27.000000 most_queue-1.0/most_queue/theory/engset_model.py
--rw-rw-rw-   0        0        0    19414 2022-09-16 07:43:39.000000 most_queue-1.0/most_queue/theory/fj_calc.py
--rw-rw-rw-   0        0        0    10650 2022-09-15 16:54:06.000000 most_queue-1.0/most_queue/theory/flow_sum.py
--rw-rw-rw-   0        0        0     1626 2022-11-30 19:52:32.000000 most_queue-1.0/most_queue/theory/generate_pareto_noise.py
--rw-rw-rw-   0        0        0     5943 2022-09-15 16:55:04.000000 most_queue-1.0/most_queue/theory/gi_m_1_calc.py
--rw-rw-rw-   0        0        0     7888 2022-09-15 16:55:53.000000 most_queue-1.0/most_queue/theory/gi_m_n_calc.py
--rw-rw-rw-   0        0        0     2135 2022-11-29 13:43:22.000000 most_queue-1.0/most_queue/theory/impatience_calc.py
--rw-rw-rw-   0        0        0     4474 2022-09-15 16:56:34.000000 most_queue-1.0/most_queue/theory/m_d_n_calc.py
--rw-rw-rw-   0        0        0    29777 2022-09-15 16:57:11.000000 most_queue-1.0/most_queue/theory/m_ph_n_prty.py
--rw-rw-rw-   0        0        0     7316 2022-09-15 16:57:53.000000 most_queue-1.0/most_queue/theory/mg1_calc.py
--rw-rw-rw-   0        0        0     1625 2022-09-15 16:58:37.000000 most_queue-1.0/most_queue/theory/mg1_warm_calc.py
--rw-rw-rw-   0        0        0    22510 2022-09-20 18:47:52.000000 most_queue-1.0/most_queue/theory/mgn_tt.py
--rw-rw-rw-   0        0        0    18992 2022-09-15 17:02:09.000000 most_queue-1.0/most_queue/theory/mmn3_pnz_cox_approx.py
--rw-rw-rw-   0        0        0    26829 2022-09-15 17:03:10.000000 most_queue-1.0/most_queue/theory/mmn_prty_pnz_approx.py
--rw-rw-rw-   0        0        0     2010 2022-09-15 17:01:13.000000 most_queue-1.0/most_queue/theory/mmnr_calc.py
--rw-rw-rw-   0        0        0     5816 2022-09-23 20:42:20.000000 most_queue-1.0/most_queue/theory/network_calc.py
--rw-rw-rw-   0        0        0     1066 2022-12-04 16:14:36.000000 most_queue-1.0/most_queue/theory/network_viewer.py
--rw-rw-rw-   0        0        0    40783 2022-09-15 17:04:24.000000 most_queue-1.0/most_queue/theory/passage_time.py
--rw-rw-rw-   0        0        0    17732 2022-09-15 17:05:30.000000 most_queue-1.0/most_queue/theory/prty_calc.py
--rw-rw-rw-   0        0        0     2174 2022-09-15 17:05:30.000000 most_queue-1.0/most_queue/theory/q_poisson_arrival_calc.py
--rw-rw-rw-   0        0        0     5396 2022-09-15 11:45:51.000000 most_queue-1.0/most_queue/theory/student_stat.py
--rw-rw-rw-   0        0        0      632 2022-09-15 11:45:51.000000 most_queue-1.0/most_queue/theory/sv_sum_calc.py
--rw-rw-rw-   0        0        0     4079 2022-09-15 12:02:16.000000 most_queue-1.0/most_queue/theory/weibull.py
-drwxrwxrwx   0        0        0        0 2023-01-25 13:18:13.058477 most_queue-1.0/most_queue/visualisation/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.0/most_queue/visualisation/__init__.py
--rw-rw-rw-   0        0        0    35629 2022-09-30 18:59:24.000000 most_queue-1.0/most_queue/visualisation/smo_im_vis.py
-drwxrwxrwx   0        0        0        0 2023-01-25 13:18:13.091078 most_queue-1.0/most_queue/visualisation/utils/
--rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most_queue-1.0/most_queue/visualisation/utils/__init__.py
--rw-rw-rw-   0        0        0     3169 2022-06-17 16:46:09.000000 most_queue-1.0/most_queue/visualisation/utils/result_table.py
--rw-rw-rw-   0        0        0    14872 2022-08-16 20:24:21.000000 most_queue-1.0/most_queue/visualisation/utils/settings_window.py
--rw-rw-rw-   0        0        0     1432 2022-06-03 20:22:54.000000 most_queue-1.0/most_queue/visualisation/utils/splash_screen.py
-drwxrwxrwx   0        0        0        0 2023-01-25 13:18:12.389941 most_queue-1.0/most_queue.egg-info/
--rw-rw-rw-   0        0        0     6117 2023-01-25 13:18:12.000000 most_queue-1.0/most_queue.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2414 2023-01-25 13:18:12.000000 most_queue-1.0/most_queue.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-25 13:18:12.000000 most_queue-1.0/most_queue.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-25 20:28:16.000000 most_queue-1.0/most_queue.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      105 2023-01-25 13:18:12.000000 most_queue-1.0/most_queue.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-01-25 13:18:12.000000 most_queue-1.0/most_queue.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      508 2023-01-25 13:14:24.000000 most_queue-1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-25 13:18:13.094710 most_queue-1.0/setup.cfg
--rw-rw-rw-   0        0        0      975 2023-01-25 13:13:36.000000 most_queue-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:41:53.767445 most-queue-1.1/
+-rw-rw-rw-   0        0        0     1091 2022-09-15 10:35:18.000000 most-queue-1.1/LICENSE
+-rw-rw-rw-   0        0        0      504 2023-05-08 07:41:53.766930 most-queue-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4326 2022-12-01 21:12:39.000000 most-queue-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 07:41:53.732009 most-queue-1.1/most_queue/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most-queue-1.1/most_queue/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:41:53.740430 most-queue-1.1/most_queue/sim/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:45:51.000000 most-queue-1.1/most_queue/sim/__init__.py
+-rw-rw-rw-   0        0        0    14664 2022-09-15 16:47:38.000000 most-queue-1.1/most_queue/sim/fj_delta_im.py
+-rw-rw-rw-   0        0        0    11132 2022-09-23 20:35:51.000000 most-queue-1.1/most_queue/sim/fj_im.py
+-rw-rw-rw-   0        0        0    10099 2022-09-15 12:02:16.000000 most-queue-1.1/most_queue/sim/flow_sum_im.py
+-rw-rw-rw-   0        0        0    10619 2022-12-01 20:31:07.000000 most-queue-1.1/most_queue/sim/network_im_prty.py
+-rw-rw-rw-   0        0        0    13161 2022-11-30 19:30:09.000000 most-queue-1.1/most_queue/sim/queue_finite_source_sim.py
+-rw-rw-rw-   0        0        0    37331 2023-01-25 13:05:08.000000 most-queue-1.1/most_queue/sim/rand_destribution.py
+-rw-rw-rw-   0        0        0     3913 2022-11-30 19:31:29.000000 most-queue-1.1/most_queue/sim/smo_batch_sim.py
+-rw-rw-rw-   0        0        0    25978 2022-11-30 17:51:13.000000 most-queue-1.1/most_queue/sim/smo_im.py
+-rw-rw-rw-   0        0        0    39946 2022-09-25 20:15:14.000000 most-queue-1.1/most_queue/sim/smo_im_prty.py
+-rw-rw-rw-   0        0        0     7724 2022-11-29 20:49:52.000000 most-queue-1.1/most_queue/sim/smo_impatient_im.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:41:53.749931 most-queue-1.1/most_queue/tests/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most-queue-1.1/most_queue/tests/__init__.py
+-rw-rw-rw-   0        0        0     3826 2022-09-16 06:55:00.000000 most-queue-1.1/most_queue/tests/ek_d_n.py
+-rw-rw-rw-   0        0        0     4997 2022-09-16 07:21:38.000000 most-queue-1.1/most_queue/tests/fj_calc.py
+-rw-rw-rw-   0        0        0     5539 2022-09-16 07:43:39.000000 most-queue-1.1/most_queue/tests/fj_im.py
+-rw-rw-rw-   0        0        0     4262 2023-05-08 07:37:15.000000 most-queue-1.1/most_queue/tests/flow_sum.py
+-rw-rw-rw-   0        0        0     5122 2022-09-16 08:17:30.000000 most-queue-1.1/most_queue/tests/gi_m_1_calc.py
+-rw-rw-rw-   0        0        0     5258 2022-09-16 08:17:30.000000 most-queue-1.1/most_queue/tests/gi_m_n_calc.py
+-rw-rw-rw-   0        0        0     2255 2022-09-16 08:20:45.000000 most-queue-1.1/most_queue/tests/m_d_n_calc.py
+-rw-rw-rw-   0        0        0     6712 2022-09-16 08:52:49.000000 most-queue-1.1/most_queue/tests/m_ph_n_prty.py
+-rw-rw-rw-   0        0        0     5267 2022-09-20 18:59:53.000000 most-queue-1.1/most_queue/tests/mg1_calc.py
+-rw-rw-rw-   0        0        0      982 2022-09-15 18:04:48.000000 most-queue-1.1/most_queue/tests/mg1_warm_calc.py
+-rw-rw-rw-   0        0        0     4747 2023-05-08 07:36:11.000000 most-queue-1.1/most_queue/tests/mgn_tt.py
+-rw-rw-rw-   0        0        0     3337 2022-09-15 18:04:48.000000 most-queue-1.1/most_queue/tests/mmn3_pnz_cox_approx.py
+-rw-rw-rw-   0        0        0     2830 2022-09-15 18:04:48.000000 most-queue-1.1/most_queue/tests/mmn_prty_pnz_approx.py
+-rw-rw-rw-   0        0        0     8149 2022-09-23 20:18:42.000000 most-queue-1.1/most_queue/tests/network_im_prty.py
+-rw-rw-rw-   0        0        0    17534 2022-09-15 18:04:48.000000 most-queue-1.1/most_queue/tests/passage_time.py
+-rw-rw-rw-   0        0        0     2744 2022-09-23 19:56:01.000000 most-queue-1.1/most_queue/tests/smo_im.py
+-rw-rw-rw-   0        0        0     6545 2022-09-23 20:18:42.000000 most-queue-1.1/most_queue/tests/smo_im_prty.py
+-rw-rw-rw-   0        0        0      967 2022-09-16 08:52:49.000000 most-queue-1.1/most_queue/tests/weibull.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:41:53.764028 most-queue-1.1/most_queue/theory/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:45:51.000000 most-queue-1.1/most_queue/theory/__init__.py
+-rw-rw-rw-   0        0        0     2092 2022-09-15 12:02:16.000000 most-queue-1.1/most_queue/theory/approx_cdf_make.py
+-rw-rw-rw-   0        0        0     2360 2022-11-30 18:00:26.000000 most-queue-1.1/most_queue/theory/batch_mm1.py
+-rw-rw-rw-   0        0        0     1304 2022-09-15 11:45:51.000000 most-queue-1.1/most_queue/theory/diff5dots.py
+-rw-rw-rw-   0        0        0     6193 2022-09-15 16:51:31.000000 most-queue-1.1/most_queue/theory/ek_d_n_calc.py
+-rw-rw-rw-   0        0        0     4760 2022-11-30 19:14:27.000000 most-queue-1.1/most_queue/theory/engset_model.py
+-rw-rw-rw-   0        0        0    19414 2022-09-16 07:43:39.000000 most-queue-1.1/most_queue/theory/fj_calc.py
+-rw-rw-rw-   0        0        0    10650 2022-09-15 16:54:06.000000 most-queue-1.1/most_queue/theory/flow_sum.py
+-rw-rw-rw-   0        0        0     1626 2022-11-30 19:52:32.000000 most-queue-1.1/most_queue/theory/generate_pareto_noise.py
+-rw-rw-rw-   0        0        0     5943 2022-09-15 16:55:04.000000 most-queue-1.1/most_queue/theory/gi_m_1_calc.py
+-rw-rw-rw-   0        0        0     7888 2022-09-15 16:55:53.000000 most-queue-1.1/most_queue/theory/gi_m_n_calc.py
+-rw-rw-rw-   0        0        0     2135 2022-11-29 13:43:22.000000 most-queue-1.1/most_queue/theory/impatience_calc.py
+-rw-rw-rw-   0        0        0     4474 2022-09-15 16:56:34.000000 most-queue-1.1/most_queue/theory/m_d_n_calc.py
+-rw-rw-rw-   0        0        0    29777 2022-09-15 16:57:11.000000 most-queue-1.1/most_queue/theory/m_ph_n_prty.py
+-rw-rw-rw-   0        0        0     7316 2022-09-15 16:57:53.000000 most-queue-1.1/most_queue/theory/mg1_calc.py
+-rw-rw-rw-   0        0        0     1625 2022-09-15 16:58:37.000000 most-queue-1.1/most_queue/theory/mg1_warm_calc.py
+-rw-rw-rw-   0        0        0    22510 2022-09-20 18:47:52.000000 most-queue-1.1/most_queue/theory/mgn_tt.py
+-rw-rw-rw-   0        0        0    18992 2022-09-15 17:02:09.000000 most-queue-1.1/most_queue/theory/mmn3_pnz_cox_approx.py
+-rw-rw-rw-   0        0        0    26829 2022-09-15 17:03:10.000000 most-queue-1.1/most_queue/theory/mmn_prty_pnz_approx.py
+-rw-rw-rw-   0        0        0     2010 2022-09-15 17:01:13.000000 most-queue-1.1/most_queue/theory/mmnr_calc.py
+-rw-rw-rw-   0        0        0     5816 2022-09-23 20:42:20.000000 most-queue-1.1/most_queue/theory/network_calc.py
+-rw-rw-rw-   0        0        0     1066 2022-12-04 16:14:36.000000 most-queue-1.1/most_queue/theory/network_viewer.py
+-rw-rw-rw-   0        0        0    40783 2022-09-15 17:04:24.000000 most-queue-1.1/most_queue/theory/passage_time.py
+-rw-rw-rw-   0        0        0    17732 2022-09-15 17:05:30.000000 most-queue-1.1/most_queue/theory/prty_calc.py
+-rw-rw-rw-   0        0        0     2174 2022-09-15 17:05:30.000000 most-queue-1.1/most_queue/theory/q_poisson_arrival_calc.py
+-rw-rw-rw-   0        0        0     5396 2022-09-15 11:45:51.000000 most-queue-1.1/most_queue/theory/student_stat.py
+-rw-rw-rw-   0        0        0      632 2022-09-15 11:45:51.000000 most-queue-1.1/most_queue/theory/sv_sum_calc.py
+-rw-rw-rw-   0        0        0     4079 2022-09-15 12:02:16.000000 most-queue-1.1/most_queue/theory/weibull.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:41:53.764584 most-queue-1.1/most_queue/visualisation/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most-queue-1.1/most_queue/visualisation/__init__.py
+-rw-rw-rw-   0        0        0    35629 2022-09-30 18:59:24.000000 most-queue-1.1/most_queue/visualisation/smo_im_vis.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:41:53.766430 most-queue-1.1/most_queue/visualisation/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-15 11:32:20.000000 most-queue-1.1/most_queue/visualisation/utils/__init__.py
+-rw-rw-rw-   0        0        0     3169 2022-06-17 16:46:09.000000 most-queue-1.1/most_queue/visualisation/utils/result_table.py
+-rw-rw-rw-   0        0        0    14872 2022-08-16 20:24:21.000000 most-queue-1.1/most_queue/visualisation/utils/settings_window.py
+-rw-rw-rw-   0        0        0     1432 2022-06-03 20:22:54.000000 most-queue-1.1/most_queue/visualisation/utils/splash_screen.py
+drwxrwxrwx   0        0        0        0 2023-05-08 07:41:53.735552 most-queue-1.1/most_queue.egg-info/
+-rw-rw-rw-   0        0        0      504 2023-05-08 07:41:53.000000 most-queue-1.1/most_queue.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2414 2023-05-08 07:41:53.000000 most-queue-1.1/most_queue.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 07:41:53.000000 most-queue-1.1/most_queue.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-25 20:28:16.000000 most-queue-1.1/most_queue.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      105 2023-05-08 07:41:53.000000 most-queue-1.1/most_queue.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-08 07:41:53.000000 most-queue-1.1/most_queue.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      508 2023-05-08 07:41:19.000000 most-queue-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 07:41:53.767445 most-queue-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      975 2023-05-08 07:41:44.000000 most-queue-1.1/setup.py
```

### Comparing `most_queue-1.0/LICENSE` & `most-queue-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/PKG-INFO` & `most-queue-1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,7 @@
-Metadata-Version: 2.1
-Name: most_queue
-Version: 1.0
-Summary: Software package for calculation and simulation of queuing systems
-Home-page: https://github.com/xabarov/mps
-Author: Xabarov Roman
-Author-email: Xabarov Roman <xabarov1985@gmail.com>
-License: Copyright (c) 2018 The Python Packaging Authority
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: Homepage, https://github.com/xabarov/mps
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # most_queue
 Software package for calculation and simulation of queuing systems and networks
 
 ## Authors
 - [xabarov](https://github.com/xabarov)
 
 ## Installation
```

### Comparing `most_queue-1.0/most_queue/sim/fj_delta_im.py` & `most-queue-1.1/most_queue/sim/fj_delta_im.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/sim/fj_im.py` & `most-queue-1.1/most_queue/sim/fj_im.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/sim/flow_sum_im.py` & `most-queue-1.1/most_queue/sim/flow_sum_im.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/sim/network_im_prty.py` & `most-queue-1.1/most_queue/sim/network_im_prty.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/sim/queue_finite_source_sim.py` & `most-queue-1.1/most_queue/sim/queue_finite_source_sim.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/sim/rand_destribution.py` & `most-queue-1.1/most_queue/sim/rand_destribution.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/sim/smo_batch_sim.py` & `most-queue-1.1/most_queue/sim/smo_batch_sim.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/sim/smo_im.py` & `most-queue-1.1/most_queue/sim/smo_im.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/sim/smo_im_prty.py` & `most-queue-1.1/most_queue/sim/smo_im_prty.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/sim/smo_impatient_im.py` & `most-queue-1.1/most_queue/sim/smo_impatient_im.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/tests/ek_d_n.py` & `most-queue-1.1/most_queue/tests/ek_d_n.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/tests/fj_calc.py` & `most-queue-1.1/most_queue/tests/fj_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/tests/fj_im.py` & `most-queue-1.1/most_queue/tests/fj_im.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/tests/flow_sum.py` & `most-queue-1.1/most_queue/tests/flow_sum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from most_queue.theory.flow_sum import SummatorNumeric
-from most_queue.sim import flow_sum_im
-from most_queue.sim import rand_destribution as rd
+from .. sim import flow_sum_im
+from .. sim import rand_destribution as rd
 import matplotlib.pyplot as plt
 
 
 def test():
     """
     Тестирование суммирования потоков
     """
```

### Comparing `most_queue-1.0/most_queue/tests/gi_m_1_calc.py` & `most-queue-1.1/most_queue/tests/gi_m_1_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/tests/gi_m_n_calc.py` & `most-queue-1.1/most_queue/tests/gi_m_n_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/tests/m_d_n_calc.py` & `most-queue-1.1/most_queue/tests/m_d_n_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/tests/m_ph_n_prty.py` & `most-queue-1.1/most_queue/tests/m_ph_n_prty.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/tests/mg1_calc.py` & `most-queue-1.1/most_queue/tests/mg1_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/tests/mg1_warm_calc.py` & `most-queue-1.1/most_queue/tests/mg1_warm_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/tests/mgn_tt.py` & `most-queue-1.1/most_queue/tests/mgn_tt.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from most_queue.sim import rand_destribution as rd
 import time
 from most_queue.theory.mgn_tt import MGnCalc
 
 
 def test():
     """
-    Тестирование метода Такаха-Таками для расчета СМО М/H2/n
+    Тестирование метода Такахаси-Таками для расчета СМО М/H2/n
 
     При коэфф вариации времени обслуживания < 1 параметры аппроксимирующего Н2-распределения
     являются комплексными, что не мешает получению осмысленных результатов
 
     Для верификации используется ИМ
 
     """
```

### Comparing `most_queue-1.0/most_queue/tests/mmn3_pnz_cox_approx.py` & `most-queue-1.1/most_queue/tests/mmn3_pnz_cox_approx.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/tests/mmn_prty_pnz_approx.py` & `most-queue-1.1/most_queue/tests/mmn_prty_pnz_approx.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/tests/network_im_prty.py` & `most-queue-1.1/most_queue/tests/network_im_prty.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/tests/passage_time.py` & `most-queue-1.1/most_queue/tests/passage_time.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/tests/smo_im.py` & `most-queue-1.1/most_queue/tests/smo_im.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/tests/smo_im_prty.py` & `most-queue-1.1/most_queue/tests/smo_im_prty.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/tests/weibull.py` & `most-queue-1.1/most_queue/tests/weibull.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/approx_cdf_make.py` & `most-queue-1.1/most_queue/theory/approx_cdf_make.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/batch_mm1.py` & `most-queue-1.1/most_queue/theory/batch_mm1.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/diff5dots.py` & `most-queue-1.1/most_queue/theory/diff5dots.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/ek_d_n_calc.py` & `most-queue-1.1/most_queue/theory/ek_d_n_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/engset_model.py` & `most-queue-1.1/most_queue/theory/engset_model.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/fj_calc.py` & `most-queue-1.1/most_queue/theory/fj_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/flow_sum.py` & `most-queue-1.1/most_queue/theory/flow_sum.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/generate_pareto_noise.py` & `most-queue-1.1/most_queue/theory/generate_pareto_noise.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/gi_m_1_calc.py` & `most-queue-1.1/most_queue/theory/gi_m_1_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/gi_m_n_calc.py` & `most-queue-1.1/most_queue/theory/gi_m_n_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/impatience_calc.py` & `most-queue-1.1/most_queue/theory/impatience_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/m_d_n_calc.py` & `most-queue-1.1/most_queue/theory/m_d_n_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/m_ph_n_prty.py` & `most-queue-1.1/most_queue/theory/m_ph_n_prty.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/mg1_calc.py` & `most-queue-1.1/most_queue/theory/mg1_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/mg1_warm_calc.py` & `most-queue-1.1/most_queue/theory/mg1_warm_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/mgn_tt.py` & `most-queue-1.1/most_queue/theory/mgn_tt.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/mmn3_pnz_cox_approx.py` & `most-queue-1.1/most_queue/theory/mmn3_pnz_cox_approx.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/mmn_prty_pnz_approx.py` & `most-queue-1.1/most_queue/theory/mmn_prty_pnz_approx.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/mmnr_calc.py` & `most-queue-1.1/most_queue/theory/mmnr_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/network_calc.py` & `most-queue-1.1/most_queue/theory/network_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/network_viewer.py` & `most-queue-1.1/most_queue/theory/network_viewer.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/passage_time.py` & `most-queue-1.1/most_queue/theory/passage_time.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/prty_calc.py` & `most-queue-1.1/most_queue/theory/prty_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/q_poisson_arrival_calc.py` & `most-queue-1.1/most_queue/theory/q_poisson_arrival_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/student_stat.py` & `most-queue-1.1/most_queue/theory/student_stat.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/sv_sum_calc.py` & `most-queue-1.1/most_queue/theory/sv_sum_calc.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/theory/weibull.py` & `most-queue-1.1/most_queue/theory/weibull.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/visualisation/smo_im_vis.py` & `most-queue-1.1/most_queue/visualisation/smo_im_vis.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/visualisation/utils/result_table.py` & `most-queue-1.1/most_queue/visualisation/utils/result_table.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/visualisation/utils/settings_window.py` & `most-queue-1.1/most_queue/visualisation/utils/settings_window.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue/visualisation/utils/splash_screen.py` & `most-queue-1.1/most_queue/visualisation/utils/splash_screen.py`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/most_queue.egg-info/SOURCES.txt` & `most-queue-1.1/most_queue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `most_queue-1.0/setup.py` & `most-queue-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='most-queue',
-      version='1.00',
+      version='1.01',
       description="Software package for calculation and simulation of queuing systems",
       author='Xabarov Roman',
       author_email='xabarov1985@gmail.com',
       url='https://github.com/xabarov/mps',
       classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
```

