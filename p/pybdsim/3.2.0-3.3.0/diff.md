# Comparing `tmp/pybdsim-3.2.0.tar.gz` & `tmp/pybdsim-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybdsim-3.2.0.tar", last modified: Wed Apr 26 20:33:29 2023, max compression
+gzip compressed data, was "pybdsim-3.3.0.tar", last modified: Mon May  8 16:11:41 2023, max compression
```

## Comparing `pybdsim-3.2.0.tar` & `pybdsim-3.3.0.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.946318 pybdsim-3.2.0/
--rw-r--r--   0 lnevay     (501) staff       (20)      116 2023-03-19 12:01:08.000000 pybdsim-3.2.0/.gitignore
--rw-r--r--   0 lnevay     (501) staff       (20)    35149 2020-05-18 14:14:31.000000 pybdsim-3.2.0/COPYING.txt
--rw-r--r--   0 lnevay     (501) staff       (20)      615 2023-03-19 11:23:51.000000 pybdsim-3.2.0/LICENSE.txt
--rw-r--r--   0 lnevay     (501) staff       (20)      565 2023-03-17 15:48:00.000000 pybdsim-3.2.0/Makefile
--rw-r--r--   0 lnevay     (501) staff       (20)     2090 2023-04-26 20:33:29.946434 pybdsim-3.2.0/PKG-INFO
--rw-r--r--   0 lnevay     (501) staff       (20)      924 2023-03-19 11:28:25.000000 pybdsim-3.2.0/README.md
--rw-r--r--   0 lnevay     (501) staff       (20)      960 2020-06-08 21:19:17.000000 pybdsim-3.2.0/bitbucket-pipelines.yml
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.911662 pybdsim-3.2.0/docs/
--rw-r--r--   0 lnevay     (501) staff       (20)      611 2020-05-18 14:14:31.000000 pybdsim-3.2.0/docs/Makefile
--rw-r--r--   0 lnevay     (501) staff       (20)      809 2020-05-18 14:14:31.000000 pybdsim-3.2.0/docs/make.bat
--rw-r--r--   0 lnevay     (501) staff       (20)  1197598 2023-04-26 20:32:00.000000 pybdsim-3.2.0/docs/pybdsim.pdf
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.914553 pybdsim-3.2.0/docs/source/
--rw-r--r--   0 lnevay     (501) staff       (20)      291 2023-03-17 15:48:00.000000 pybdsim-3.2.0/docs/source/authorship.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     5049 2023-03-17 15:47:53.000000 pybdsim-3.2.0/docs/source/builder.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     2784 2023-03-17 15:47:53.000000 pybdsim-3.2.0/docs/source/classes.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     5251 2022-02-14 12:30:59.000000 pybdsim-3.2.0/docs/source/compare.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     5444 2023-03-19 13:19:27.000000 pybdsim-3.2.0/docs/source/conf.py
--rw-r--r--   0 lnevay     (501) staff       (20)    20082 2021-06-15 15:09:13.000000 pybdsim-3.2.0/docs/source/convert.rst
--rw-r--r--   0 lnevay     (501) staff       (20)    11964 2023-03-19 11:16:47.000000 pybdsim-3.2.0/docs/source/data.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     3032 2023-03-19 12:42:38.000000 pybdsim-3.2.0/docs/source/data_uproot.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     1448 2023-04-02 20:14:28.000000 pybdsim-3.2.0/docs/source/developer.rst
--rw-r--r--   0 lnevay     (501) staff       (20)    12892 2023-03-29 08:13:29.000000 pybdsim-3.2.0/docs/source/fieldmaps.rst
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.915709 pybdsim-3.2.0/docs/source/figures/
--rw-r--r--   0 lnevay     (501) staff       (20)   459915 2020-05-18 14:14:31.000000 pybdsim-3.2.0/docs/source/figures/rebdsimFileHistograms.png
--rw-r--r--   0 lnevay     (501) staff       (20)   536529 2020-05-18 14:14:31.000000 pybdsim-3.2.0/docs/source/figures/rebdsimFileHistogramsWrapped.png
--rw-r--r--   0 lnevay     (501) staff       (20)   287477 2020-05-18 14:14:31.000000 pybdsim-3.2.0/docs/source/figures/rebdsimFileMembers.png
--rw-r--r--   0 lnevay     (501) staff       (20)   196253 2020-05-18 14:14:31.000000 pybdsim-3.2.0/docs/source/figures/simpleHistogramPlot.png
--rw-r--r--   0 lnevay     (501) staff       (20)      468 2023-04-26 11:59:44.000000 pybdsim-3.2.0/docs/source/index.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     2107 2023-03-19 13:20:03.000000 pybdsim-3.2.0/docs/source/installation.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      679 2023-03-19 13:16:04.000000 pybdsim-3.2.0/docs/source/licence.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     2827 2023-03-17 15:47:53.000000 pybdsim-3.2.0/docs/source/moduledocs.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     3420 2023-04-26 14:47:31.000000 pybdsim-3.2.0/docs/source/plotting.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      558 2020-05-18 14:14:31.000000 pybdsim-3.2.0/docs/source/support.rst
--rw-r--r--   0 lnevay     (501) staff       (20)    11854 2023-04-26 14:49:01.000000 pybdsim-3.2.0/docs/source/version_history.rst
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.915939 pybdsim-3.2.0/examples/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.917608 pybdsim-3.2.0/examples/1_builder/
--rw-r--r--   0 lnevay     (501) staff       (20)      396 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/1_builder/1_builder.rst
--rw-r--r--   0 lnevay     (501) staff       (20)   348736 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/1_builder/1_testmachine.png
--rwxr-xr-x   0 lnevay     (501) staff       (20)      379 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/1_builder/1_testmachine.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.922961 pybdsim-3.2.0/examples/2_convert/
--rw-r--r--   0 lnevay     (501) staff       (20)    84758 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/2_convert/1_madxtfs2gmad.png
--rwxr-xr-x   0 lnevay     (501) staff       (20)      165 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/2_convert/1_madxtfs2gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1068 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/2_convert/2_convert.rst
--rw-r--r--   0 lnevay     (501) staff       (20)   107428 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/2_convert/2_transport2gmad.png
--rwxr-xr-x   0 lnevay     (501) staff       (20)      184 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/2_convert/2_transport2gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)   134154 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/2_convert/transport_example.dat
--rw-r--r--   0 lnevay     (501) staff       (20)    19220 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/2_convert/transport_example.pdf
--rw-r--r--   0 lnevay     (501) staff       (20)    24970 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/2_convert/twiss35tevb1_short.pdf
--rw-r--r--   0 lnevay     (501) staff       (20)    21778 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/2_convert/twiss35tevb1_short.tar.gz
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.923160 pybdsim-3.2.0/examples/3_optics/
--rw-r--r--   0 lnevay     (501) staff       (20)     4703 2023-03-19 12:30:43.000000 pybdsim-3.2.0/examples/3_optics/optics_validation.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.923407 pybdsim-3.2.0/examples/4_uproot/
--rw-r--r--   0 lnevay     (501) staff       (20)      943 2023-03-19 11:16:47.000000 pybdsim-3.2.0/examples/4_uproot/4_uproot.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      446 2023-03-19 11:16:47.000000 pybdsim-3.2.0/examples/examples.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     1731 2023-04-22 17:03:22.000000 pybdsim-3.2.0/pyproject.toml
--rw-r--r--   0 lnevay     (501) staff       (20)      257 2023-04-26 20:33:29.946752 pybdsim-3.2.0/setup.cfg
--rw-r--r--   0 lnevay     (501) staff       (20)       38 2023-03-19 11:23:22.000000 pybdsim-3.2.0/setup.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.908655 pybdsim-3.2.0/src/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.927912 pybdsim-3.2.0/src/pybdsim/
--rw-r--r--   0 lnevay     (501) staff       (20)    12864 2023-03-17 15:50:15.000000 pybdsim-3.2.0/src/pybdsim/Beam.py
--rw-r--r--   0 lnevay     (501) staff       (20)    71670 2023-03-29 08:02:12.000000 pybdsim-3.2.0/src/pybdsim/Builder.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.930554 pybdsim-3.2.0/src/pybdsim/Compare/
--rw-r--r--   0 lnevay     (501) staff       (20)     8655 2023-04-26 11:56:15.000000 pybdsim-3.2.0/src/pybdsim/Compare/_BdsimBdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)    10617 2023-03-29 08:03:23.000000 pybdsim-3.2.0/src/pybdsim/Compare/_ElegantBdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)    14701 2023-03-17 15:47:53.000000 pybdsim-3.2.0/src/pybdsim/Compare/_Mad8BdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)    28319 2023-03-17 15:47:53.000000 pybdsim-3.2.0/src/pybdsim/Compare/_Mad8BdsimComparisonOld.py
--rw-r--r--   0 lnevay     (501) staff       (20)    23115 2023-04-26 11:54:49.000000 pybdsim-3.2.0/src/pybdsim/Compare/_MadxBdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)      294 2020-05-18 14:14:31.000000 pybdsim-3.2.0/src/pybdsim/Compare/_MadxMadxComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)    48470 2023-04-26 11:55:02.000000 pybdsim-3.2.0/src/pybdsim/Compare/_MultipleCodeComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3641 2020-05-18 14:14:31.000000 pybdsim-3.2.0/src/pybdsim/Compare/_SadComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)     6448 2023-04-26 11:55:20.000000 pybdsim-3.2.0/src/pybdsim/Compare/_TransportBdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)      822 2023-03-17 15:47:53.000000 pybdsim-3.2.0/src/pybdsim/Compare/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)     2584 2023-04-22 20:29:56.000000 pybdsim-3.2.0/src/pybdsim/Constants.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.934297 pybdsim-3.2.0/src/pybdsim/Convert/
--rw-r--r--   0 lnevay     (501) staff       (20)     2801 2023-03-28 19:08:52.000000 pybdsim-3.2.0/src/pybdsim/Convert/_BdsimElement2TransferMatrix.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12960 2023-03-28 19:07:59.000000 pybdsim-3.2.0/src/pybdsim/Convert/_BdsimPrimaries2Inrays.py
--rw-r--r--   0 lnevay     (501) staff       (20)    24068 2023-03-28 19:16:33.000000 pybdsim-3.2.0/src/pybdsim/Convert/_CPyMad2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3984 2023-03-17 15:47:53.000000 pybdsim-3.2.0/src/pybdsim/Convert/_ElegantParamToStrength.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12045 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Convert/_Mad8Saveline2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)    30913 2023-03-17 15:47:53.000000 pybdsim-3.2.0/src/pybdsim/Convert/_Mad8Twiss2Gmad.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)    34813 2023-03-17 15:47:53.000000 pybdsim-3.2.0/src/pybdsim/Convert/_Mad8Twiss2GmadOld.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)    37650 2023-03-17 15:47:53.000000 pybdsim-3.2.0/src/pybdsim/Convert/_MadxTfs2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)     6282 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Convert/_MadxTfs2GmadStrength.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)     1561 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Convert/_Rebdsim2Numpy.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12293 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Convert/_SadFlat2Gmad.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)     4460 2020-05-18 14:14:31.000000 pybdsim-3.2.0/src/pybdsim/Convert/_Transport2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1115 2023-03-28 19:11:54.000000 pybdsim-3.2.0/src/pybdsim/Convert/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1044 2020-05-18 14:14:31.000000 pybdsim-3.2.0/src/pybdsim/Convert/collimator_analysis.py
--rw-r--r--   0 lnevay     (501) staff       (20)    78167 2023-04-22 20:33:46.000000 pybdsim-3.2.0/src/pybdsim/Data.py
--rw-r--r--   0 lnevay     (501) staff       (20)    69562 2023-04-10 18:48:13.000000 pybdsim-3.2.0/src/pybdsim/DataUproot.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.934869 pybdsim-3.2.0/src/pybdsim/Field/
--rwxr-xr-x   0 lnevay     (501) staff       (20)    19403 2023-03-17 15:47:53.000000 pybdsim-3.2.0/src/pybdsim/Field/FieldPlotter.py
--rw-r--r--   0 lnevay     (501) staff       (20)     2427 2023-03-17 15:47:53.000000 pybdsim-3.2.0/src/pybdsim/Field/FieldPlotterVtk.py
--rw-r--r--   0 lnevay     (501) staff       (20)    16881 2023-04-17 18:48:37.000000 pybdsim-3.2.0/src/pybdsim/Field/_Field.py
--rw-r--r--   0 lnevay     (501) staff       (20)      981 2023-04-22 17:06:38.000000 pybdsim-3.2.0/src/pybdsim/Field/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)     2704 2023-03-17 15:47:53.000000 pybdsim-3.2.0/src/pybdsim/Geant4.py
--rw-r--r--   0 lnevay     (501) staff       (20)    18652 2023-04-17 19:55:26.000000 pybdsim-3.2.0/src/pybdsim/Gmad.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)     2654 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Joinhistograms.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3648 2023-04-10 22:16:41.000000 pybdsim-3.2.0/src/pybdsim/ModelProcessing.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.908956 pybdsim-3.2.0/src/pybdsim/Obsolete/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.936887 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/
--rw-r--r--   0 lnevay     (501) staff       (20)     3587 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Analysis.py
--rw-r--r--   0 lnevay     (501) staff       (20)     4482 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/AnalysisRoot.py
--rw-r--r--   0 lnevay     (501) staff       (20)      934 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/AnalysisRootOptics.py
--rw-r--r--   0 lnevay     (501) staff       (20)     5562 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Event.py
--rw-r--r--   0 lnevay     (501) staff       (20)      348 2020-05-18 14:14:31.000000 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Model.py
--rw-r--r--   0 lnevay     (501) staff       (20)      353 2020-05-18 14:14:31.000000 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Options.py
--rw-r--r--   0 lnevay     (501) staff       (20)      115 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Plots.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3276 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Processed.py
--rw-r--r--   0 lnevay     (501) staff       (20)    11554 2020-05-18 14:14:31.000000 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Root.py
--rw-r--r--   0 lnevay     (501) staff       (20)      479 2020-05-18 14:14:31.000000 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Run.py
--rw-r--r--   0 lnevay     (501) staff       (20)      513 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)    15291 2023-03-29 19:06:12.000000 pybdsim-3.2.0/src/pybdsim/Optics.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12066 2023-03-19 13:13:38.000000 pybdsim-3.2.0/src/pybdsim/Options.py
--rw-r--r--   0 lnevay     (501) staff       (20)    76164 2023-04-26 14:35:42.000000 pybdsim-3.2.0/src/pybdsim/Plot.py
--rw-r--r--   0 lnevay     (501) staff       (20)     9630 2023-03-19 13:00:55.000000 pybdsim-3.2.0/src/pybdsim/Run.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.937880 pybdsim-3.2.0/src/pybdsim/Testing/
--rw-r--r--   0 lnevay     (501) staff       (20)       25 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Testing/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)    48656 2023-04-26 11:55:44.000000 pybdsim-3.2.0/src/pybdsim/Testing/bdsimMadx.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12119 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Testing/trackingTester.py
--rw-r--r--   0 lnevay     (501) staff       (20)     2484 2023-03-19 13:02:51.000000 pybdsim-3.2.0/src/pybdsim/Visualisation.py
--rw-r--r--   0 lnevay     (501) staff       (20)    25579 2023-03-19 13:03:02.000000 pybdsim-3.2.0/src/pybdsim/Writer.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3125 2020-05-18 17:03:47.000000 pybdsim-3.2.0/src/pybdsim/XSecBias.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3358 2023-04-26 09:53:42.000000 pybdsim-3.2.0/src/pybdsim/_General.py
--rw-r--r--   0 lnevay     (501) staff       (20)     4658 2023-04-22 20:04:46.000000 pybdsim-3.2.0/src/pybdsim/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)      160 2023-04-26 20:33:29.000000 pybdsim-3.2.0/src/pybdsim/_version.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.928662 pybdsim-3.2.0/src/pybdsim.egg-info/
--rw-r--r--   0 lnevay     (501) staff       (20)     2090 2023-04-26 20:33:29.000000 pybdsim-3.2.0/src/pybdsim.egg-info/PKG-INFO
--rw-r--r--   0 lnevay     (501) staff       (20)     5148 2023-04-26 20:33:29.000000 pybdsim-3.2.0/src/pybdsim.egg-info/SOURCES.txt
--rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-04-26 20:33:29.000000 pybdsim-3.2.0/src/pybdsim.egg-info/dependency_links.txt
--rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-03-19 11:36:13.000000 pybdsim-3.2.0/src/pybdsim.egg-info/not-zip-safe
--rw-r--r--   0 lnevay     (501) staff       (20)      245 2023-04-26 20:33:29.000000 pybdsim-3.2.0/src/pybdsim.egg-info/requires.txt
--rw-r--r--   0 lnevay     (501) staff       (20)        8 2023-04-26 20:33:29.000000 pybdsim-3.2.0/src/pybdsim.egg-info/top_level.txt
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.938126 pybdsim-3.2.0/tests/
--rw-r--r--   0 lnevay     (501) staff       (20)       13 2020-06-08 21:19:17.000000 pybdsim-3.2.0/tests/__init__.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.939693 pybdsim-3.2.0/tests/test_input/
--rw-r--r--   0 lnevay     (501) staff       (20)   122327 2020-05-18 14:14:31.000000 pybdsim-3.2.0/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz
--rw-r--r--   0 lnevay     (501) staff       (20)   137539 2020-05-18 14:14:31.000000 pybdsim-3.2.0/tests/test_input/model-model-aper.tfs.gz
--rw-r--r--   0 lnevay     (501) staff       (20)      459 2020-05-18 14:14:31.000000 pybdsim-3.2.0/tests/test_input/model-model-collsettings.dat
--rw-r--r--   0 lnevay     (501) staff       (20)   231976 2020-05-18 14:14:31.000000 pybdsim-3.2.0/tests/test_input/model-model.tfs.gz
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.940140 pybdsim-3.2.0/tests/test_output/
--rw-r--r--   0 lnevay     (501) staff       (20)        0 2020-05-18 14:14:31.000000 pybdsim-3.2.0/tests/test_output/.gitkeep
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.942494 pybdsim-3.2.0/tests/test_output/atf2-nominal-twiss-v5.2/
--rw-r--r--   0 lnevay     (501) staff       (20)      281 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output/atf2-nominal-twiss-v5.2/model.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      424 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output/atf2-nominal-twiss-v5.2/model_beam.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)    27567 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output/atf2-nominal-twiss-v5.2/model_components.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output/atf2-nominal-twiss-v5.2/model_options.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)     9339 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output/atf2-nominal-twiss-v5.2/model_sequence.gmad
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.943291 pybdsim-3.2.0/tests/test_output/model-model/
--rw-r--r--   0 lnevay     (501) staff       (20)      269 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output/model-model/model.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      478 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output/model-model/model_beam.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)     5311 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output/model-model/model_components.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output/model-model/model_options.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)    10521 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output/model-model/model_sequence.gmad
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.909513 pybdsim-3.2.0/tests/test_output2/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.944144 pybdsim-3.2.0/tests/test_output2/atf2-nominal-twiss-v5.2/
--rw-r--r--   0 lnevay     (501) staff       (20)      277 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output2/atf2-nominal-twiss-v5.2/model.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      424 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_beam.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)    27349 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_components.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_options.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)     9339 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_sequence.gmad
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.944947 pybdsim-3.2.0/tests/test_output2/model-model/
--rw-r--r--   0 lnevay     (501) staff       (20)      269 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output2/model-model/model.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      478 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output2/model-model/model_beam.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)     5281 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output2/model-model/model_components.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output2/model-model/model_options.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)    10521 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output2/model-model/model_sequence.gmad
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.946029 pybdsim-3.2.0/tests/tests/
--rw-r--r--   0 lnevay     (501) staff       (20)       31 2023-03-17 15:49:55.000000 pybdsim-3.2.0/tests/tests/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1359 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/tests/pybdsim_test_utils.py
--rw-r--r--   0 lnevay     (501) staff       (20)     8239 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/tests/test_MadxTfs2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)      631 2022-02-14 12:30:59.000000 pybdsim-3.2.0/tests/tests/testratio.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1424 2020-05-18 15:11:01.000000 pybdsim-3.2.0/tests/tests/write_test_outputs.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.946186 pybdsim-3.2.0/tests/unit/
--rw-r--r--   0 lnevay     (501) staff       (20)     9948 2020-05-18 14:14:31.000000 pybdsim-3.2.0/tests/unit/test_Builder.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.301689 pybdsim-3.3.0/
+-rw-r--r--   0 lnevay     (501) staff       (20)      116 2023-03-19 12:01:08.000000 pybdsim-3.3.0/.gitignore
+-rw-r--r--   0 lnevay     (501) staff       (20)    35149 2020-05-18 14:14:31.000000 pybdsim-3.3.0/COPYING.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)      615 2023-03-19 11:23:51.000000 pybdsim-3.3.0/LICENSE.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)      565 2023-03-17 15:48:00.000000 pybdsim-3.3.0/Makefile
+-rw-r--r--   0 lnevay     (501) staff       (20)     2144 2023-05-08 16:11:41.301792 pybdsim-3.3.0/PKG-INFO
+-rw-r--r--   0 lnevay     (501) staff       (20)      936 2023-05-08 16:07:40.000000 pybdsim-3.3.0/README.md
+-rw-r--r--   0 lnevay     (501) staff       (20)      960 2020-06-08 21:19:17.000000 pybdsim-3.3.0/bitbucket-pipelines.yml
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.258791 pybdsim-3.3.0/docs/
+-rw-r--r--   0 lnevay     (501) staff       (20)      611 2020-05-18 14:14:31.000000 pybdsim-3.3.0/docs/Makefile
+-rw-r--r--   0 lnevay     (501) staff       (20)      809 2020-05-18 14:14:31.000000 pybdsim-3.3.0/docs/make.bat
+-rw-r--r--   0 lnevay     (501) staff       (20)  1199563 2023-05-08 16:10:24.000000 pybdsim-3.3.0/docs/pybdsim.pdf
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.269123 pybdsim-3.3.0/docs/source/
+-rw-r--r--   0 lnevay     (501) staff       (20)      307 2023-05-08 16:07:51.000000 pybdsim-3.3.0/docs/source/authorship.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     5049 2023-03-17 15:47:53.000000 pybdsim-3.3.0/docs/source/builder.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     2784 2023-03-17 15:47:53.000000 pybdsim-3.3.0/docs/source/classes.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     5251 2022-02-14 12:30:59.000000 pybdsim-3.3.0/docs/source/compare.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     5444 2023-03-19 13:19:27.000000 pybdsim-3.3.0/docs/source/conf.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    20082 2021-06-15 15:09:13.000000 pybdsim-3.3.0/docs/source/convert.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)    11964 2023-03-19 11:16:47.000000 pybdsim-3.3.0/docs/source/data.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     3032 2023-03-19 12:42:38.000000 pybdsim-3.3.0/docs/source/data_uproot.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     1448 2023-04-02 20:14:28.000000 pybdsim-3.3.0/docs/source/developer.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)    12892 2023-03-29 08:13:29.000000 pybdsim-3.3.0/docs/source/fieldmaps.rst
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.272076 pybdsim-3.3.0/docs/source/figures/
+-rw-r--r--   0 lnevay     (501) staff       (20)   459915 2020-05-18 14:14:31.000000 pybdsim-3.3.0/docs/source/figures/rebdsimFileHistograms.png
+-rw-r--r--   0 lnevay     (501) staff       (20)   536529 2020-05-18 14:14:31.000000 pybdsim-3.3.0/docs/source/figures/rebdsimFileHistogramsWrapped.png
+-rw-r--r--   0 lnevay     (501) staff       (20)   287477 2020-05-18 14:14:31.000000 pybdsim-3.3.0/docs/source/figures/rebdsimFileMembers.png
+-rw-r--r--   0 lnevay     (501) staff       (20)   196253 2020-05-18 14:14:31.000000 pybdsim-3.3.0/docs/source/figures/simpleHistogramPlot.png
+-rw-r--r--   0 lnevay     (501) staff       (20)      468 2023-04-26 11:59:44.000000 pybdsim-3.3.0/docs/source/index.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     2198 2023-05-08 16:05:46.000000 pybdsim-3.3.0/docs/source/installation.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      679 2023-03-19 13:16:04.000000 pybdsim-3.3.0/docs/source/licence.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     2827 2023-03-17 15:47:53.000000 pybdsim-3.3.0/docs/source/moduledocs.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     3420 2023-04-26 14:47:31.000000 pybdsim-3.3.0/docs/source/plotting.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      558 2020-05-18 14:14:31.000000 pybdsim-3.3.0/docs/source/support.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)    12250 2023-05-08 16:08:56.000000 pybdsim-3.3.0/docs/source/version_history.rst
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.272693 pybdsim-3.3.0/examples/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.273855 pybdsim-3.3.0/examples/1_builder/
+-rw-r--r--   0 lnevay     (501) staff       (20)      396 2020-05-18 14:14:31.000000 pybdsim-3.3.0/examples/1_builder/1_builder.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)   348736 2020-05-18 14:14:31.000000 pybdsim-3.3.0/examples/1_builder/1_testmachine.png
+-rwxr-xr-x   0 lnevay     (501) staff       (20)      379 2020-05-18 14:14:31.000000 pybdsim-3.3.0/examples/1_builder/1_testmachine.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.276149 pybdsim-3.3.0/examples/2_convert/
+-rw-r--r--   0 lnevay     (501) staff       (20)    84758 2020-05-18 14:14:31.000000 pybdsim-3.3.0/examples/2_convert/1_madxtfs2gmad.png
+-rwxr-xr-x   0 lnevay     (501) staff       (20)      165 2020-05-18 14:14:31.000000 pybdsim-3.3.0/examples/2_convert/1_madxtfs2gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1068 2020-05-18 14:14:31.000000 pybdsim-3.3.0/examples/2_convert/2_convert.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)   107428 2020-05-18 14:14:31.000000 pybdsim-3.3.0/examples/2_convert/2_transport2gmad.png
+-rwxr-xr-x   0 lnevay     (501) staff       (20)      184 2020-05-18 14:14:31.000000 pybdsim-3.3.0/examples/2_convert/2_transport2gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)   134154 2020-05-18 14:14:31.000000 pybdsim-3.3.0/examples/2_convert/transport_example.dat
+-rw-r--r--   0 lnevay     (501) staff       (20)    19220 2020-05-18 14:14:31.000000 pybdsim-3.3.0/examples/2_convert/transport_example.pdf
+-rw-r--r--   0 lnevay     (501) staff       (20)    24970 2020-05-18 14:14:31.000000 pybdsim-3.3.0/examples/2_convert/twiss35tevb1_short.pdf
+-rw-r--r--   0 lnevay     (501) staff       (20)    21778 2020-05-18 14:14:31.000000 pybdsim-3.3.0/examples/2_convert/twiss35tevb1_short.tar.gz
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.276329 pybdsim-3.3.0/examples/3_optics/
+-rw-r--r--   0 lnevay     (501) staff       (20)     4703 2023-03-19 12:30:43.000000 pybdsim-3.3.0/examples/3_optics/optics_validation.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.276548 pybdsim-3.3.0/examples/4_uproot/
+-rw-r--r--   0 lnevay     (501) staff       (20)      943 2023-03-19 11:16:47.000000 pybdsim-3.3.0/examples/4_uproot/4_uproot.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      446 2023-03-19 11:16:47.000000 pybdsim-3.3.0/examples/examples.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     1846 2023-05-08 16:01:13.000000 pybdsim-3.3.0/pyproject.toml
+-rw-r--r--   0 lnevay     (501) staff       (20)      258 2023-05-08 16:11:41.302061 pybdsim-3.3.0/setup.cfg
+-rw-r--r--   0 lnevay     (501) staff       (20)       38 2023-03-19 11:23:22.000000 pybdsim-3.3.0/setup.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.255239 pybdsim-3.3.0/src/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.282544 pybdsim-3.3.0/src/pybdsim/
+-rw-r--r--   0 lnevay     (501) staff       (20)    12864 2023-03-17 15:50:15.000000 pybdsim-3.3.0/src/pybdsim/Beam.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    71670 2023-03-29 08:02:12.000000 pybdsim-3.3.0/src/pybdsim/Builder.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.285475 pybdsim-3.3.0/src/pybdsim/Compare/
+-rw-r--r--   0 lnevay     (501) staff       (20)     8655 2023-04-26 11:56:15.000000 pybdsim-3.3.0/src/pybdsim/Compare/_BdsimBdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    10617 2023-03-29 08:03:23.000000 pybdsim-3.3.0/src/pybdsim/Compare/_ElegantBdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    14701 2023-03-17 15:47:53.000000 pybdsim-3.3.0/src/pybdsim/Compare/_Mad8BdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    28319 2023-03-17 15:47:53.000000 pybdsim-3.3.0/src/pybdsim/Compare/_Mad8BdsimComparisonOld.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    23115 2023-04-26 11:54:49.000000 pybdsim-3.3.0/src/pybdsim/Compare/_MadxBdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      294 2020-05-18 14:14:31.000000 pybdsim-3.3.0/src/pybdsim/Compare/_MadxMadxComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    48470 2023-04-26 11:55:02.000000 pybdsim-3.3.0/src/pybdsim/Compare/_MultipleCodeComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3641 2020-05-18 14:14:31.000000 pybdsim-3.3.0/src/pybdsim/Compare/_SadComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     6438 2023-05-08 16:03:57.000000 pybdsim-3.3.0/src/pybdsim/Compare/_TransportBdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      827 2023-05-08 16:04:54.000000 pybdsim-3.3.0/src/pybdsim/Compare/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     2584 2023-04-22 20:29:56.000000 pybdsim-3.3.0/src/pybdsim/Constants.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.288709 pybdsim-3.3.0/src/pybdsim/Convert/
+-rw-r--r--   0 lnevay     (501) staff       (20)     2801 2023-03-28 19:08:52.000000 pybdsim-3.3.0/src/pybdsim/Convert/_BdsimElement2TransferMatrix.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12960 2023-03-28 19:07:59.000000 pybdsim-3.3.0/src/pybdsim/Convert/_BdsimPrimaries2Inrays.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    24068 2023-03-28 19:16:33.000000 pybdsim-3.3.0/src/pybdsim/Convert/_CPyMad2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3984 2023-03-17 15:47:53.000000 pybdsim-3.3.0/src/pybdsim/Convert/_ElegantParamToStrength.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12045 2020-05-18 15:11:01.000000 pybdsim-3.3.0/src/pybdsim/Convert/_Mad8Saveline2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    30913 2023-03-17 15:47:53.000000 pybdsim-3.3.0/src/pybdsim/Convert/_Mad8Twiss2Gmad.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)    34813 2023-03-17 15:47:53.000000 pybdsim-3.3.0/src/pybdsim/Convert/_Mad8Twiss2GmadOld.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)    37650 2023-03-17 15:47:53.000000 pybdsim-3.3.0/src/pybdsim/Convert/_MadxTfs2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     6282 2020-05-18 15:11:01.000000 pybdsim-3.3.0/src/pybdsim/Convert/_MadxTfs2GmadStrength.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)     1561 2020-05-18 15:11:01.000000 pybdsim-3.3.0/src/pybdsim/Convert/_Rebdsim2Numpy.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12293 2020-05-18 15:11:01.000000 pybdsim-3.3.0/src/pybdsim/Convert/_SadFlat2Gmad.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)     4483 2023-05-08 16:02:45.000000 pybdsim-3.3.0/src/pybdsim/Convert/_Transport2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1115 2023-05-08 15:59:37.000000 pybdsim-3.3.0/src/pybdsim/Convert/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1044 2020-05-18 14:14:31.000000 pybdsim-3.3.0/src/pybdsim/Convert/collimator_analysis.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    79780 2023-05-03 14:03:26.000000 pybdsim-3.3.0/src/pybdsim/Data.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    69562 2023-04-10 18:48:13.000000 pybdsim-3.3.0/src/pybdsim/DataUproot.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.289602 pybdsim-3.3.0/src/pybdsim/Field/
+-rwxr-xr-x   0 lnevay     (501) staff       (20)    19403 2023-03-17 15:47:53.000000 pybdsim-3.3.0/src/pybdsim/Field/FieldPlotter.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     2427 2023-03-17 15:47:53.000000 pybdsim-3.3.0/src/pybdsim/Field/FieldPlotterVtk.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    16881 2023-04-17 18:48:37.000000 pybdsim-3.3.0/src/pybdsim/Field/_Field.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      981 2023-04-22 17:06:38.000000 pybdsim-3.3.0/src/pybdsim/Field/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     2704 2023-03-17 15:47:53.000000 pybdsim-3.3.0/src/pybdsim/Geant4.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    18652 2023-04-17 19:55:26.000000 pybdsim-3.3.0/src/pybdsim/Gmad.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)     2654 2020-05-18 15:11:01.000000 pybdsim-3.3.0/src/pybdsim/Joinhistograms.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3648 2023-04-10 22:16:41.000000 pybdsim-3.3.0/src/pybdsim/ModelProcessing.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.255515 pybdsim-3.3.0/src/pybdsim/Obsolete/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.291582 pybdsim-3.3.0/src/pybdsim/Obsolete/Rebdsim/
+-rw-r--r--   0 lnevay     (501) staff       (20)     3587 2020-05-18 15:11:01.000000 pybdsim-3.3.0/src/pybdsim/Obsolete/Rebdsim/Analysis.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     4482 2020-05-18 15:11:01.000000 pybdsim-3.3.0/src/pybdsim/Obsolete/Rebdsim/AnalysisRoot.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      934 2020-05-18 15:11:01.000000 pybdsim-3.3.0/src/pybdsim/Obsolete/Rebdsim/AnalysisRootOptics.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     5562 2020-05-18 15:11:01.000000 pybdsim-3.3.0/src/pybdsim/Obsolete/Rebdsim/Event.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      348 2020-05-18 14:14:31.000000 pybdsim-3.3.0/src/pybdsim/Obsolete/Rebdsim/Model.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      353 2020-05-18 14:14:31.000000 pybdsim-3.3.0/src/pybdsim/Obsolete/Rebdsim/Options.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      115 2020-05-18 15:11:01.000000 pybdsim-3.3.0/src/pybdsim/Obsolete/Rebdsim/Plots.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3276 2020-05-18 15:11:01.000000 pybdsim-3.3.0/src/pybdsim/Obsolete/Rebdsim/Processed.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    11554 2020-05-18 14:14:31.000000 pybdsim-3.3.0/src/pybdsim/Obsolete/Rebdsim/Root.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      479 2020-05-18 14:14:31.000000 pybdsim-3.3.0/src/pybdsim/Obsolete/Rebdsim/Run.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      513 2020-05-18 15:11:01.000000 pybdsim-3.3.0/src/pybdsim/Obsolete/Rebdsim/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    15291 2023-03-29 19:06:12.000000 pybdsim-3.3.0/src/pybdsim/Optics.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12066 2023-03-19 13:13:38.000000 pybdsim-3.3.0/src/pybdsim/Options.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    76884 2023-04-26 21:11:06.000000 pybdsim-3.3.0/src/pybdsim/Plot.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     9630 2023-03-19 13:00:55.000000 pybdsim-3.3.0/src/pybdsim/Run.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.292307 pybdsim-3.3.0/src/pybdsim/Testing/
+-rw-r--r--   0 lnevay     (501) staff       (20)       25 2020-05-18 15:11:01.000000 pybdsim-3.3.0/src/pybdsim/Testing/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    48656 2023-04-26 11:55:44.000000 pybdsim-3.3.0/src/pybdsim/Testing/bdsimMadx.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12119 2020-05-18 15:11:01.000000 pybdsim-3.3.0/src/pybdsim/Testing/trackingTester.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     2484 2023-03-19 13:02:51.000000 pybdsim-3.3.0/src/pybdsim/Visualisation.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    25579 2023-03-19 13:03:02.000000 pybdsim-3.3.0/src/pybdsim/Writer.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3125 2020-05-18 17:03:47.000000 pybdsim-3.3.0/src/pybdsim/XSecBias.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3358 2023-04-26 09:53:42.000000 pybdsim-3.3.0/src/pybdsim/_General.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     4658 2023-04-22 20:04:46.000000 pybdsim-3.3.0/src/pybdsim/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      160 2023-05-08 16:11:41.000000 pybdsim-3.3.0/src/pybdsim/_version.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.283270 pybdsim-3.3.0/src/pybdsim.egg-info/
+-rw-r--r--   0 lnevay     (501) staff       (20)     2144 2023-05-08 16:11:41.000000 pybdsim-3.3.0/src/pybdsim.egg-info/PKG-INFO
+-rw-r--r--   0 lnevay     (501) staff       (20)     5148 2023-05-08 16:11:41.000000 pybdsim-3.3.0/src/pybdsim.egg-info/SOURCES.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-05-08 16:11:41.000000 pybdsim-3.3.0/src/pybdsim.egg-info/dependency_links.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-03-19 11:36:13.000000 pybdsim-3.3.0/src/pybdsim.egg-info/not-zip-safe
+-rw-r--r--   0 lnevay     (501) staff       (20)      335 2023-05-08 16:11:41.000000 pybdsim-3.3.0/src/pybdsim.egg-info/requires.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)        8 2023-05-08 16:11:41.000000 pybdsim-3.3.0/src/pybdsim.egg-info/top_level.txt
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.292526 pybdsim-3.3.0/tests/
+-rw-r--r--   0 lnevay     (501) staff       (20)       13 2020-06-08 21:19:17.000000 pybdsim-3.3.0/tests/__init__.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.293833 pybdsim-3.3.0/tests/test_input/
+-rw-r--r--   0 lnevay     (501) staff       (20)   122327 2020-05-18 14:14:31.000000 pybdsim-3.3.0/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz
+-rw-r--r--   0 lnevay     (501) staff       (20)   137539 2020-05-18 14:14:31.000000 pybdsim-3.3.0/tests/test_input/model-model-aper.tfs.gz
+-rw-r--r--   0 lnevay     (501) staff       (20)      459 2020-05-18 14:14:31.000000 pybdsim-3.3.0/tests/test_input/model-model-collsettings.dat
+-rw-r--r--   0 lnevay     (501) staff       (20)   231976 2020-05-18 14:14:31.000000 pybdsim-3.3.0/tests/test_input/model-model.tfs.gz
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.294175 pybdsim-3.3.0/tests/test_output/
+-rw-r--r--   0 lnevay     (501) staff       (20)        0 2020-05-18 14:14:31.000000 pybdsim-3.3.0/tests/test_output/.gitkeep
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.295010 pybdsim-3.3.0/tests/test_output/atf2-nominal-twiss-v5.2/
+-rw-r--r--   0 lnevay     (501) staff       (20)      281 2020-05-18 17:03:47.000000 pybdsim-3.3.0/tests/test_output/atf2-nominal-twiss-v5.2/model.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      424 2020-05-18 17:03:47.000000 pybdsim-3.3.0/tests/test_output/atf2-nominal-twiss-v5.2/model_beam.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)    27567 2020-05-18 17:03:47.000000 pybdsim-3.3.0/tests/test_output/atf2-nominal-twiss-v5.2/model_components.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.3.0/tests/test_output/atf2-nominal-twiss-v5.2/model_options.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)     9339 2020-05-18 17:03:47.000000 pybdsim-3.3.0/tests/test_output/atf2-nominal-twiss-v5.2/model_sequence.gmad
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.295880 pybdsim-3.3.0/tests/test_output/model-model/
+-rw-r--r--   0 lnevay     (501) staff       (20)      269 2020-05-18 17:03:47.000000 pybdsim-3.3.0/tests/test_output/model-model/model.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      478 2020-05-18 17:03:47.000000 pybdsim-3.3.0/tests/test_output/model-model/model_beam.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)     5311 2020-05-18 17:03:47.000000 pybdsim-3.3.0/tests/test_output/model-model/model_components.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.3.0/tests/test_output/model-model/model_options.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)    10521 2020-05-18 17:03:47.000000 pybdsim-3.3.0/tests/test_output/model-model/model_sequence.gmad
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.256040 pybdsim-3.3.0/tests/test_output2/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.296707 pybdsim-3.3.0/tests/test_output2/atf2-nominal-twiss-v5.2/
+-rw-r--r--   0 lnevay     (501) staff       (20)      277 2020-05-18 17:03:47.000000 pybdsim-3.3.0/tests/test_output2/atf2-nominal-twiss-v5.2/model.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      424 2020-05-18 17:03:47.000000 pybdsim-3.3.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_beam.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)    27349 2020-05-18 17:03:47.000000 pybdsim-3.3.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_components.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.3.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_options.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)     9339 2020-05-18 17:03:47.000000 pybdsim-3.3.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_sequence.gmad
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.300596 pybdsim-3.3.0/tests/test_output2/model-model/
+-rw-r--r--   0 lnevay     (501) staff       (20)      269 2020-05-18 17:03:47.000000 pybdsim-3.3.0/tests/test_output2/model-model/model.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      478 2020-05-18 17:03:47.000000 pybdsim-3.3.0/tests/test_output2/model-model/model_beam.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)     5281 2020-05-18 17:03:47.000000 pybdsim-3.3.0/tests/test_output2/model-model/model_components.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.3.0/tests/test_output2/model-model/model_options.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)    10521 2020-05-18 17:03:47.000000 pybdsim-3.3.0/tests/test_output2/model-model/model_sequence.gmad
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.301432 pybdsim-3.3.0/tests/tests/
+-rw-r--r--   0 lnevay     (501) staff       (20)       31 2023-03-17 15:49:55.000000 pybdsim-3.3.0/tests/tests/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1359 2020-05-18 17:03:47.000000 pybdsim-3.3.0/tests/tests/pybdsim_test_utils.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     8239 2020-05-18 17:03:47.000000 pybdsim-3.3.0/tests/tests/test_MadxTfs2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      631 2022-02-14 12:30:59.000000 pybdsim-3.3.0/tests/tests/testratio.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1424 2020-05-18 15:11:01.000000 pybdsim-3.3.0/tests/tests/write_test_outputs.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-05-08 16:11:41.301569 pybdsim-3.3.0/tests/unit/
+-rw-r--r--   0 lnevay     (501) staff       (20)     9948 2020-05-18 14:14:31.000000 pybdsim-3.3.0/tests/unit/test_Builder.py
```

### Comparing `pybdsim-3.2.0/COPYING.txt` & `pybdsim-3.3.0/COPYING.txt`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/LICENSE.txt` & `pybdsim-3.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/Makefile` & `pybdsim-3.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/PKG-INFO` & `pybdsim-3.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybdsim
-Version: 3.2.0
+Version: 3.3.0
 Summary: Python utilities for the Monte Carlo Particle accelerator code BDSIM.
 Author-email: "JAI@RHUL" <laurie.nevay@cern.ch>
 Maintainer-email: Laurie Nevay <laurie.nevay@cern.ch>
 Project-URL: homepage, http://www.pp.rhul.ac.uk/bdsim/pybdsim
 Project-URL: documentation, http://www.pp.rhul.ac.uk/bdsim/pybdsim
 Project-URL: repository, https://bitbucket.org/jairhul/pybdsim
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,28 +21,31 @@
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: uproot
 Provides-Extra: boost_histogram
 Provides-Extra: cpymad
 Provides-Extra: pysad
+Provides-Extra: pymad8
+Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE.txt
 License-File: COPYING.txt
 
 # pybdsim #
 
 A python package containing both utilities for preparing and analysing BDSIM input and output as well as controlling BDSIM.
 
 ## Authors ##
 
 L. Nevay
 A. Abramov
 S. Alden
 S. Boogert
+M. Deniaud
 C. Hernalsteens
 W. Parker
 E. Ramoisiaux
 W. Shields
 J. Snuverink
 R. Tesse
 S. Walker
```

### Comparing `pybdsim-3.2.0/README.md` & `pybdsim-3.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 ## Authors ##
 
 L. Nevay
 A. Abramov
 S. Alden
 S. Boogert
+M. Deniaud
 C. Hernalsteens
 W. Parker
 E. Ramoisiaux
 W. Shields
 J. Snuverink
 R. Tesse
 S. Walker
```

### Comparing `pybdsim-3.2.0/bitbucket-pipelines.yml` & `pybdsim-3.3.0/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/docs/Makefile` & `pybdsim-3.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/docs/make.bat` & `pybdsim-3.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/docs/pybdsim.pdf` & `pybdsim-3.3.0/docs/pybdsim.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 7% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,13 +1,13 @@
 pybdsim Documentation
-Release 3.2.0
+Release 3.3.0
 
 Royal Holloway
 
-Apr 26, 2023
+May 08, 2023
 
 CONTENTS
 
 1
 
 Licence & Disclaimer
 
@@ -158,50 +158,52 @@
 12 Support
 12.1 Feature Request . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 47
 47
 
 13 Version History
-13.1 V3.2.0 - 2023 / 04 / 26 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.2 V3.1.1 - 2023 / 04 / 23 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.3 V3.1.0 - 2023 / 04 / 02 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.4 V3.0.1 - 2023 / 03 / 22 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.5 V3.0.0 - 2023 / 03 / 19 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.6 v2.4.0 - 2021 / 06 / 16 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.7 v2.3.0 - 2020 / 12 / 15 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.8 v2.2.0 - 2020 / 06 / 08 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.9 v2.1 - 2019 / 04 / 20 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.10 v2.0 - 2019 / 02 / 27 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.11 v1.9 - 2018 / 08 / 24 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.12 v1.8 - 2018 / 06 / 23 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.13 v1.7 - 2018 / 06 / 30 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.14 v1.6 - 2018 / 05 / 23 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.15 v1.5 - 2018 / 05 / 17 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.16 v1.4 - 2018 / 10 / 04 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.17 v1.3 - 2017 / 12 / 05 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.1 V3.3.0 - 2023 / 05 / 08 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.2 V3.2.0 - 2023 / 04 / 26 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.3 V3.1.1 - 2023 / 04 / 23 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.4 V3.1.0 - 2023 / 04 / 02 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.5 V3.0.1 - 2023 / 03 / 22 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.6 V3.0.0 - 2023 / 03 / 19 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.7 v2.4.0 - 2021 / 06 / 16 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.8 v2.3.0 - 2020 / 12 / 15 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.9 v2.2.0 - 2020 / 06 / 08 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.10 v2.1 - 2019 / 04 / 20 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.11 v2.0 - 2019 / 02 / 27 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.12 v1.9 - 2018 / 08 / 24 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.13 v1.8 - 2018 / 06 / 23 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.14 v1.7 - 2018 / 06 / 30 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.15 v1.6 - 2018 / 05 / 23 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.16 v1.5 - 2018 / 05 / 17 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.17 v1.4 - 2018 / 10 / 04 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.18 v1.3 - 2017 / 12 / 05 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 49
 49
 49
 49
 50
 50
+50
 51
-51
+52
 52
 52
 52
 53
 53
 54
 54
 54
 55
-55
+56
 
 14 Module Contents
 14.1 pybdsim.Beam module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 14.2 pybdsim.Builder module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 14.3 pybdsim.Compare . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 14.4 pybdsim.Constants module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 14.5 pybdsim.Convert . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
@@ -219,31 +221,29 @@
 57
 57
 58
 67
 68
 68
 73
-79
+80
 85
 87
-87
+88
 90
 95
 96
-96
+97
 99
 
-15 Developer Documentation
-
-101
-
 ii
 
-15.1 Release Checklist . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 101
+15 Developer Documentation
+101
+15.1 Release Checklist . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 101
 16 Indices and tables
 
 103
 
 Python Module Index
 
 105
@@ -252,23 +252,23 @@
 
 107
 
 iii
 
 iv
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 pybdsim is a Python package to aid in the preparation, running and validation of BDSIM models.
 
 CONTENTS
 
 1
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 2
 
 CONTENTS
 
 CHAPTER
 
@@ -282,15 +282,15 @@
 pybdsim is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General
 Public License for more details.
 You should have received a copy of the GNU General Public License along with pybdsim. If not, see <http:
 //www.gnu.org/licenses/>.
 
 3
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 4
 
 Chapter 1. Licence & Disclaimer
 
 CHAPTER
 
@@ -299,26 +299,27 @@
 AUTHORSHIP
 
 The following people have contributed to pybdsim:
 • Laurie Nevay
 • Andrey Abramov
 • Siobhan Alden
 • Stewart Boogert
+• Marin Deniaud
 • Cedric Hernalsteens
 • Fabian Metzger
 • Will Parker
 • Eliott Ramoisiaux
 • William Shields
 • Jochem Snuverink
 • Robin Tesse
 • Stuart Walker
 
 5
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 6
 
 Chapter 2. Authorship
 
 CHAPTER
 
@@ -330,38 +331,39 @@
 access):
 pip install pybdsim
 There are the following features that result in more dependencies being installed:
 • uproot - includes uproot data loading
 • boost_histogram - includes boost-histogram package for 4d histograms
 • cpymad - allows usage of cpymad for converting models
 • pysad - allows usage of pysad for converting models
+• pymad8 - allows usage of pymad8 for converting models
+• all - all of the above at once
 These can be installed as:
 pip install pybdsim[uproot]
 or:
-pip install pybdsim[uproot,boost_histogram,cpymad,pysad]
+pip install pybdsim[uproot,boost_histogram,cpymad,pysad,pymad8]
 
 3.1 Requirements
 ROOT and its python interface are required to load BDSIM output and also histogram files from rebdsim (the
 analysis tool). This cannot be found through pip but must be separately installed.
 Note: When installing ROOT, make sure that ROOT is installed with the same python interpreter you intend to
 use the package through. Most systems have more than one Python.
 Generally, the requirements for pybdsim are
 • matplotlib >= 3.0
 • numpy >= 1.14
 • scipy
 • fortranformat
 • pymadx
-• pymad8
 • pytransport
-These are all available through pip and will be automatically installed.
 
 7
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
+These are all available through pip and will be automatically installed.
 Optional:
 • ROOT Python interface
 
 3.2 Local Installation
 Although on pip, for development purposes you may wish to use pybdsim from a copy of the source code. It is
 possible to clone the git repository and use pip to point at the local set of files, or generally install that set of files
 as a once off.
@@ -410,15 +412,15 @@
 File:
 ~/physics/reps/pybdsim/Builder.py
 Type:
 instancemethod
 
 9
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 4.2 Adding Options
 No options are required to run the most basic BDSIM model. However, it is often advantageous to specify at least
 a few options such as the physics list and default aperture. To add options programmatically, there is an options
 class. This is instantiated and then ‘setter’ methods are used to set values of parameters. This options instance can
 then be associated with a machine instance. For example:
 >>> o = pybdsim.Options.Options()
@@ -450,15 +452,15 @@
 >>> a = pybdsim.Builder.Machine()
 >>> a.Write('outputfilename')
 
 10
 
 Chapter 4. Building Models
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 4.5 Units
 The user may supply units as strings that will be written to the gmad syntax as a Python tuple. For example:
 >>> a = pybdsim.Builder.Machine()
 >>> a.AddDrift('d1', (3.2, 'm'))
 This will result in the following gmad syntax:
 >>> print a[0]
@@ -484,15 +486,15 @@
 Anywhere you see a function with the last argument as **kwargs, this feature can be used.
 The arguments included in the function signatures are the minimum arguments required for functionality.
 
 4.5. Units
 
 11
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 12
 
 Chapter 4. Building Models
 
 CHAPTER
 
@@ -526,15 +528,15 @@
 where SEQUENCENAME is the name of the sequence in madx. By not specifying the output columns, a very large
 file is produced containing all possible columns. This is required to successfully convert the lattice. If the tfs file
 contains insufficient information, pybdsim will not be able to convert the model.
 Note: The python utilities require “.tfs” suffix as the file type to work properly.
 
 13
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 5.1.2 Converting the Tfs File
 Once prepared, the Tfs file can be converted. The converter is used as follows:
 >>> pybdsim.Convert.MadxTfs2Gmad('inputfile.tfs', 'latticev1')
 The conversion returns three objects, which are the pybdsim.Builder.Machine instance as converted, a second
 Machine that isn’t split by aperture and a list of any ommitted items by name.
 >>> a,b,c = pybdsim.Convert.MadxTfs2Gmad('inputfile.tfs', 'latticev1')
@@ -545,15 +547,15 @@
 will create a directory test if it doesn’t exist already.
 There are a few options that provide useful functionality for conversion:
 
 14
 
 Chapter 5. Converting Models
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 tfs
 outputfilename
 startname
 
 stopname
 
@@ -645,15 +647,15 @@
 Do not append an integer to the base file name if it already exists. Instead
 overwrite the files.
 15
 Treat every row in the TFS file/instance as a unique element. This makes
 it easier to edit individual components as they are guaranteed to appear
 only once in the entire resulting GMAD lattice.
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 The user may convert only part of the input model by specifying startname and stopname.
 Generally speaking, extra information can be folded into the conversion via a user supplied dictionary with extra
 parameters for a particular element by name. For a given element, for example ‘drift123’, extra parameters can
 be speficied in a dictionary. This leads to a dictionary of dictionaries being supplied. This is a relatively simple
 structure the user may prepare from their own input format and converters in Python. For example:
 >>> drift123dict = {'aper1':0.03, 'aper2':0.05, 'apertureType':'rectangular'}
@@ -691,15 +693,15 @@
 2. echo variables in the mad8 job log (SIGPT, SIGT)
 3. converting the tape files to gmad using pybdsim
 
 16
 
 Chapter 5. Converting Models
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 5.3.1 Running mad8
 The following variables need to be defined in the Mad8 job from a BETA0
 EMITX
 EMITY
 BLENG
 ESPRD
@@ -763,15 +765,15 @@
 pybdsim.Convert.Mad8MakeApertureTemplate(<inputtwissfilename>,<aperturedbfilename>)
 Copy the <collimatordbfilename> to collimator.dat and <aperturedbfilename> to apertures.dat Once prepared, the Tape files can be converted. The converter is used as follows:
 
 5.3. Mad8Twiss2Gmad (using saved TWISS output)
 
 17
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 pybdsim.Convert.Mad8Twiss2Gmad(<inputtwissfilename>,<outputgamdfilename>)
 
 5.4 pytransport
 https://bitbucket.org/jairhul/pytransport is a separate utility to convert transport models into BDSIM ones.
 
 5.5 BDSIM Primaries To Others
@@ -804,15 +806,15 @@
 The primary BDSIM coordinates are converted to a BDSIM userFile format. The converter is used as follows:
 >>> pybdsim.Convert.BdsimPrimaries2BdsimUserFile('output.root', 'inrays.dat')
 
 18
 
 Chapter 5. Converting Models
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 5.5.4 BdsimSampler2BdsimUserFile
 The BDSIM coordinates from a provided sampler name are converted to a BDSIM userFile format. The converter
 is used as follows:
 >>> pybdsim.Convert.BdsimSampler2BdsimUserFile('output.root', 'inrays.dat','DR1')
 The time coordinate recorded in the input file will be finite if the sampler being converted is not at the start of the
 machine. This function is intended to convert particles into a primary distribution, therefore the time coordinate
@@ -828,15 +830,15 @@
 The primary BDSIM coordinates are converted to mad8 format. The converter is used as follows:
 >>> pybdsim.Convert.BdsimPrimaries2Mad8('output.root', 'inrays.dat')
 
 5.5. BDSIM Primaries To Others
 
 19
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 20
 
 Chapter 5. Converting Models
 
 CHAPTER
 
@@ -869,15 +871,15 @@
 present, these should be set to zero strength but must remain in the lattice. The pybdsim.Convert.MadxTfs2Gmad
 converter for example provides a boolean flag to convert the lattice with only linear optical components. The user
 may of course proceed with non-linear magnetic fields included but it is only useful to compare the sigma in each
 dimension to a similarly similuated distribution and not the Twiss parameters.
 
 21
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 6.1.2 Analysing Optical Data
 The rebdsim tool can be used with an input analysisConfig.txt that specifies CalculateOpticalFunctions to 1 or true
 in the header (see BDSIM manual). Or the specially prepared optics tool rebdsimOptics can be used to achieve the
 same outcome - we recommend this. In the terminal:
 rebdsimOptics bdsimRawOutputFile.root optics.root
 This may take a few minutes to process. This analyses the file from the BDSIM run called ‘bdsimRawOutputFile.root’ and produces another ROOT file called optics.root with a different structure. This output file contains
@@ -906,15 +908,15 @@
 Two BDSIM optics files can also be compared with the following command:
 >>> pybdsim.Compare.BDSIMVsBDSIM('optics1.root', 'optics2.root')
 
 22
 
 Chapter 6. Model Comparison
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 6.5 Comparing to PTC
 BDSIM output can be compared to the PTC output from the PTC_TRACK routine available in MADX. The PTC
 output is written to a file typically named trackone, however it is necessary to convert this into a BDSIM-like ROOT
 output file. This can be easily accomplished with the ptc2bdsim tool, however the particle species and nominal
 momentum is required to correctly convert to the BDSIM coordinate convention. An example terminal command:
 ptc2bdsim trackone ptc.root proton 0.9999
@@ -927,15 +929,15 @@
 With the help of pytransport a TRANSPORT “FOR002” output file that has sigma matrices can be read and compared with BDSIM output:
 >>> pybdsim.Compare.TransportVsBDSIM('FOR002.DAT', 'bdsim_optics.root')
 
 6.5. Comparing to PTC
 
 23
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 24
 
 Chapter 6. Model Comparison
 
 CHAPTER
 
@@ -977,15 +979,15 @@
 'Event/MergedHistograms/PlossHisto': <pybdsim.Data.TH1 at 0x15503aeb0>,
 'Event/MergedHistograms/ElossHisto': <pybdsim.Data.TH1 at 0x15503aee0>,
 'Event/MergedHistograms/PhitsPEHisto': <pybdsim.Data.TH1 at 0x15503af10>,
 (continues on next page)
 
 25
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 (continued from previous page)
 
 'Event/MergedHistograms/PlossPEHisto': <pybdsim.Data.TH1 at 0x15503af40>,
 'Event/MergedHistograms/ElossPEHisto': <pybdsim.Data.TH1 at 0x15503af70>,
 'Event/MergedHistograms/PFirstAIHisto': <pybdsim.Data.TH1 at 0x15503afa0>,
 'Event/MergedHistograms/ElossTunnelHisto': <pybdsim.Data.TH1 at 0x15503afd0>,
@@ -1019,21 +1021,21 @@
 ˓→'])
 Note, the use of d.histogramspy for the wrapped set of histograms and not the raw ROOT histograms.
 
 26
 
 Chapter 7. Data Loading
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 7.4. Histogram Plotting
 
 27
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 7.5 ROOT Histogram Operations
 Loaded histograms from a rebdsim file are both wrapped in our pybdsim.Data.THX classes for nice numpy arrays
 for easy plotting, but also we retain the original ROOT objects.
 We can use the original ROOT objects to do many very useful things with the histogram, then wrap it again for
 plotting.
 1) Get the ROOT histogram from the loaded file in pybdsim
@@ -1051,21 +1053,21 @@
 • https://root.cern.ch/doc/master/classTH1.html
 • https://root.cern.ch/doc/master/classTH2D.html
 • https://root.cern.ch/doc/master/classTH3D.html
 28
 
 Chapter 7. Data Loading
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 7.5. ROOT Histogram Operations
 
 29
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 TH1 is, perhaps nonintuitively, the base class for 2D and 3D histograms, so many functions are documented there.
 The 2D and 3D ones have some specialised methods.
 Note: The integral and its error are nicely provided as members in pybdsim.Data.THXD. Also, you can use the
 pybdsim.Plot.Histogram. . . functions with a scaling parameter for the data.
 Some useful functions assuming a histogram h of type TH1D or TH2D or TH3D in Python:
 TH1
@@ -1105,15 +1107,15 @@
 ROOT Jargon
 • “Profile” histogram is an average in 1 dimension, not a ‘profile’ as per the real meaning of the word.
 • “Projection” means integral.
 30
 
 Chapter 7. Data Loading
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 7.6 Python Histogram Operations
 Some of the above operations are provided in functions of pybdsim.Data.TH2 and pybdsim.Data.TH3 - the ‘Python’
 versions in pybdsim.
 See pybdsim.Data module and look for each of the classes there, where their functions are listed.
 Some specifically for 3D histograms (i.e. often scoring meshes) are described below.
 
@@ -1153,15 +1155,15 @@
 # now the same as pybdsim.Data.Load("run1.root")
 (continues on next page)
 
 7.6. Python Histogram Operations
 
 31
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 (continued from previous page)
 
 model = pybdsim.Data.GetModelForPlotting(d)
 
 7.9 Sampler Data
 Warning: This is a simplified way of loading sampler data that “flattens” the structure losing all concept of
@@ -1218,15 +1220,15 @@
 >>> import pybdsim
 >>> d = pybdsim.DataUproot.BDSimOutput("output.root")
 >>> samplers = d.event.samplers
 samplers is a dictionary where keys are the name of the samplers and values are an instance of pybdsim.DataUproot.BDSimOutput.Event.Sampler. Data can be easily converted in a pandas.DataFrame using:
 
 33
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 >>> samplers['sampler_name'].df
 The primary beam can be extracted using the same procedure:
 >>> primary_beam = d.event.primary
 
 8.1.3 Optics Files
 After loading the file using pybdsim.DataUproot.ReBDSimOpticsOutput, the optics of the line can be accessed
@@ -1282,21 +1284,21 @@
 Note, the use of d.histogramspy for the wrapped set of histograms and not the raw ROOT histograms.
 
 9.2.2 2D Histogram
 See pybdsim.Plot.Histogram2D
 
 35
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 36
 
 Chapter 9. Plotting
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 9.2.3 Spectra
 >>> d = pybdsim.Data.Load("ana1.root")
 >>> d.spectra
 defaultdict(pybdsim.Data.Spectra,
 {'t10_0': <pybdsim.Data.Spectra at 0x28eaf3cd0>,
 'tax_0': <pybdsim.Data.Spectra at 0x290ed6f90>,
@@ -1333,15 +1335,15 @@
 >>> pybdsim.Plot.AddMachineLatticeFromSurveyToFigure(f, d)
 or
 
 9.3. Energy Deposition
 
 37
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 >>> pybdsim.Plot.AddMachineLatticeFromSurveyToFigure(f, "ana1.root")
 
 9.4.2 BDSIM Survey
 bdsim --file=mymodel.gmad --output=none --batch --ngenerate=1 --survey=survey1
 This produces the file survey1.dat for example, for some input model mymodel.gmad.
 >>> import pybdsim
@@ -1382,15 +1384,15 @@
 the instance of that class (i.e. that particular field map data) to a BDSIM-format field map file.
 Therefore, these classes represent a a very good route for creation and conversion of field maps. The recommended
 strategy is to get the information into one of those classes then it can be written out to file, loaded, plotted with
 ease.
 
 39
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 10.3 Creation
 A field map can be created from scratch in Python from knowledge of a field, such as an equation. A numpy array
 of the right shape should be created, then an instance of pybdsim.Field.Field[N]D created (where N is one of
 (1,2,3,4).
 Creating the array is entirely up to the user as this depends on how they get the information. However, a small
 example script is shown below here (in Python language):
@@ -1432,15 +1434,15 @@
 Generally, the numpy.shape(array) would look like:
 • 1D: (N_x, 4)
 
 40
 
 Chapter 10. Field Maps
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 • 2D: (N_x, N_y, 5)
 • 3D: (N_x, N_y, N_z, 6)
 • 4D: (N_x, N_y, N_z, N_t, 7)
 Warning: A key check is looking at the field map, the higher dimension coordinates (e.g. Y, not X) should
 change first. So for a given X value we should see the Y values cycle through a range, then the X should
 increment then the Y values cycle again. If this is not the case, then the loop order of dimensions is backwards.
@@ -1483,15 +1485,15 @@
 py) that shows 4 ways to write a field map with the same information. Ultimately, they convey the exact same field
 map to BDSIM although the file contents differ (2 sets of possible contents).
 
 10.3. Creation
 
 41
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 import numpy as _np
 import pybdsim
 B = 2.0
 # LOOP METHOD 1
 data = []
 # loop over and build up 3d lists of lists of lists
@@ -1531,15 +1533,15 @@
 # this will write out a file identical to the second one
 g.Write('2dexample_loopOrder_for_zx_tzyx.dat', writeLoopOrderReversed=True)
 
 42
 
 Chapter 10. Field Maps
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 10.4 Visualisation and Plotting
 To visualise a field map, it is possible to do so in BDSIM / Geant4. See the BDSIM manual for this information.
 This draws a selection of arrows in the 3D model and gives a rough indication that the field map is as intended.
 An alternative way is to load the data in pybdsim in Python and plot it, either fully or in slices (for 3D or 4D maps).
 Any library desired can be used in Python and the classes described above in Loading provide an excellent way to
 get a numpy array, that is ubiquitous in Python programming and libraries.
@@ -1574,15 +1576,15 @@
 :type scale: float
 >>>
 
 10.4. Visualisation and Plotting
 
 43
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 10.5 Conversion
 your data -> numpy array -> pybdsim.Field.FieldND(data) class
 To convert a field map, you should first write a loader from your own format to the field map into a numpy array
 with a structure described in Creation. Then, this array can be wrapped in an instance of one of the pybdsim Field
 classes. This class can then be used to write out the field map in BDSIM’s format. This would look something
 like:
@@ -1655,15 +1657,15 @@
 'aperDef1: aperture, aper1=3, aper2=2.5*cm;\n'
 Acceptable types are int, float, str, list, tuple(number, str). In the case of a tuple (e.g. ()), it should contain 2 items
 and the second is the units string.
 An example with a list:
 
 45
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 >>> sp = pybdsim.Builder.SamplerPlacement('z350mL',
 z=(350,'m'),
 shape="rectangular",
 aper1=(5,'m'),
 aper2=(5,'m'),
 partID=[13,-13])
@@ -1702,66 +1704,72 @@
 
 12.1 Feature Request
 Feature requests or proposals can be submitted to the issue tracker - select the issue type as proposal or enhancement..
 Please have a look at the existing list of proposals before submitting a new one.
 
 47
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 48
 
 Chapter 12. Support
 
 CHAPTER
 
 THIRTEEN
 
 VERSION HISTORY
 
-13.1 V3.2.0 - 2023 / 04 / 26
+13.1 V3.3.0 - 2023 / 05 / 08
+• Fix installation where there was a missing dependency of pandas with pymad8. pymad8 is now no longer a
+formal dependency but all the conversion and comparison code still exists.
+• Fix setup.cfg having pymadx in the name although it makes no difference.
+• Add new pybdsim.Data.GetHistoryPDGTuple() function to aid trajectory analysis.
+
+13.2 V3.2.0 - 2023 / 04 / 26
 • Remove the function pybdsim.Plot.AddMachineLatticeToFigure(). This was just a forward to
 pymadx.Plot.AddMachineLatticeToFigure() and this should be used explicitly for machine diagram
 plotting for TFS files. Otherwise, pybdsim.Plot.AddMachineLatticeFromSurveyToFigure should be
 used.
 • Better documentation about plotting.
 • Increase the visibility of light grey elements in the machine diagram from alpha 0.1 to 0.4.
 
-13.2 V3.1.1 - 2023 / 04 / 23
+13.3 V3.1.1 - 2023 / 04 / 23
 • Fixed spectra loading and plotting for when the ‘p’ and ‘s’ prefixes are used in the rebdsim Spectra command
 to denote primary and secondary particles.
 • Fixed error with default log scale in Plot.Histogram2D when no vmin was specified.
 • Fix pybdsim._version_tuple which should be pybdsim.__version_tuple__.
 • Fix import without awkward array which is only required for the [uproot] feature of pybdsim.
 • pybdsim.Plot.Spectra() now makes more than one plot if more than 8 particles are specified.
 • Recognised PDG ID 0 as “total” from BDSIM.
 
-13.3 V3.1.0 - 2023 / 04 / 02
+49
+
+pybdsim Documentation, Release 3.3.0
+
+13.4 V3.1.0 - 2023 / 04 / 02
 • Add the writing and reading of comment lines in field maps.
 • Reduce print out when loading a field map.
 • Clean imports in cpymad interface as well as in Convert functions.
 
-49
-
-pybdsim Documentation, Release 3.2.0
-
-13.4 V3.0.1 - 2023 / 03 / 22
+13.5 V3.0.1 - 2023 / 03 / 22
 • Fix import for pybdsim when ROOT is present but librebdsim etc. are not available through environmental
 variables, or findable. Would cause induce a classic ROOT segfault when importing pybdsim.
 • Fix wrong exception being raised.
 • Always write a comment string at the start of a BDSIM field map file to specify the units of the file.
 
-13.5 V3.0.0 - 2023 / 03 / 19
+13.6 V3.0.0 - 2023 / 03 / 19
 • Restructure package into a declarative Python package where all source files are now in src/pybdsim/.
 • The package now has a feature called uproot for the optional dependencies of uproot, pandas, and pint
 packages.
 • Field classes no longer have flip=True as the default - it is now False. Please check any field maps created
 by scripts using these classes.
 
-13.5.1 New Features
+13.6.1 New Features
 • Add a module to load BDSIM output file, included rebdsim files with uproot.
 • Create a nice Python copy of the header information from any (re)bdsim file when loading with pybdsim
 using only Python types.
 • New integration for 2D histograms along each axis to 1D histograms.
 • New slices for 3D histograms as well as integrating along a dimension (‘projection’). See 3D Scoring Histograms.
 • New ratio plot for 2x 1D histograms. See pybdsim.Plot.Histogram1DRatio.
 • New loading and handling of 4D histograms (from BDSIM with Boost). They can now be loaded and handled
@@ -1772,220 +1780,222 @@
 objects as you’re making them.
 • New field plotting for 2D field maps showing each component.
 • New field reflection utility function pybdsim.Field.MirrorDipoleQuadrant1 for 2D fields.
 • New field plotting function pybdsim.Field.Plot2DXYConnectionOrder to see the order an array is written in.
 This can be used to validate any field manipulations.
 • New field plotting function pybdsim.Field.Plot1DFxFyFz to see field components in 1D.
 • Field loading automatically works for dimensions such as X, Z for 2D instead of X, Y now.
-• Ability to load a rebdsim output file and only load the ROOT histograms without loading the BDSIM and
-rebdsim shared libraries, so it can be used on a separate computer with just ROOT.
-• Added classes to Builder for all GMAD objects. New ones include aperture, atom, blm, cavitymodel, crystal,
-field, material, newcolour, query, region, samplerplacement, scorer, tunnel, xsecbias.
 
 50
 
 Chapter 13. Version History
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
-13.5.2 Bug Fixes
+• Ability to load a rebdsim output file and only load the ROOT histograms without loading the BDSIM and
+rebdsim shared libraries, so it can be used on a separate computer with just ROOT.
+• Added classes to Builder for all GMAD objects. New ones include aperture, atom, blm, cavitymodel, crystal,
+field, material, newcolour, query, region, samplerplacement, scorer, tunnel, xsecbias.
+
+13.6.2 Bug Fixes
 • pybdsim would throw an exception that librebdsim and libbdsimRootEvent could not be loaded and stop if the
 libraries had been already loaded separately outside pybdsim. This has been fixed by fixing the interpretation
 of the error codes from ROOT.
 • Fix warning about “nonposy” in matplotlib version for log scales.
 • Fix check in Run of if it’s a ROOT file or not. Simplify it to use file extension.
 • Tolerate no pytransport installation.
 • Fix loading of aperture data from a BDSIM output file.
 • Fix loading of model data.
 • Fix aperture plots from a BDSIM output file.
 
-13.5.3 General
+13.6.3 General
 • The Beam class now takes distrType and not distrtype so as to match BDSIM syntax and be less confusing.
 • Updated out of date documentation.
 • Better automatic ranges for Histogram1DMultiple plots by default.
 • Better field loading in pybdsim.Field.Load. Returns the same Field object from pybdsim as you would write.
 
-13.6 v2.4.0 - 2021 / 06 / 16
-13.6.1 New Features
+13.7 v2.4.0 - 2021 / 06 / 16
+13.7.1 New Features
 • Transform3D function in a Machine.
 • Crystal, ScorerMesh and Placement also can be added to a Machine.
 • Ability to insert and replace an element in a machine.
 
-13.6.2 Bug Fixes
+13.7.2 Bug Fixes
 • Python 3.8+ warnings fixed.
 • Add ROOT_INCLUDE_PATH to ROOT as newer versions don’t do this automatically.
 • Fixed vmin for 2D histogram plot.
 
-13.7 v2.3.0 - 2020 / 12 / 15
-13.7.1 New Features
-• Convenience functions for pickling and un-pickling data in the Data module with optional compression.
-• Generic loss map plot.
-
-13.6. v2.4.0 - 2021 / 06 / 16
+13.7. v2.4.0 - 2021 / 06 / 16
 
 51
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
-13.8 v2.2.0 - 2020 / 06 / 08
+13.8 v2.3.0 - 2020 / 12 / 15
 13.8.1 New Features
+• Convenience functions for pickling and un-pickling data in the Data module with optional compression.
+• Generic loss map plot.
+
+13.9 v2.2.0 - 2020 / 06 / 08
+13.9.1 New Features
 • Support for Python3.
 
-13.9 v2.1 - 2019 / 04 / 20
-13.9.1 New Featuers
+13.10 v2.1 - 2019 / 04 / 20
+13.10.1 New Featuers
 • Optional flag of whether to write out the converted model with pybdsim.Convert.MadxTfs2Gmad.
 • Machine builder now supports new bdsim jcol element.
 • Machine diagram drawing can now start from any arbitrary S location.
 • For loaded histograms (using pybdsim.Data.TH1, TH2, TH3 classes, there are now functions ErrorsToSTD()
 and ErrorsToErrorOnMean() to easily convert between the different types of error - the default is error on
 the mean.
 • New plotting function pybdsim.Plot.Histogram2DErrors to visualise 2D histogram errors.
 
-13.9.2 General
+13.10.2 General
 • Return arguments of pybdsim.Convert.MadxTfs2Gmad is now just 2 items - machine and omitted items.
 Previously 3.
 
-13.9.3 Bug Fixes
+13.10.3 Bug Fixes
 • Fix loading of Model tree from ROOT output given some recent collimation variables may have a different
 structure or type from the existing ones.
 • In pybdsim.Plot.Histogram2D, the y log scale argument was “ylocscale” and is fixed to “yLogScale”.
 
-13.10 v2.0 - 2019 / 02 / 27
-13.10.1 New Features
+13.11 v2.0 - 2019 / 02 / 27
+13.11.1 New Features
 • Machine diagram plotting automatically from BDSIM output. Compatible with newer BDSIM output format.
 • Support for thin R matrix, parallel transporter and thick R matrix in builder.
 • Generate transfer matrix from tracking data from BDSIM for a single element.
 • Control over legend location in standard energy deposition and loss plots.
-• Utility function to write sampler data from BDSIM output to a user input file.
-• Support for energy variation in the beam line in MAD8 conversion.
-
 52
 
 Chapter 13. Version History
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
-13.10.2 General
+• Utility function to write sampler data from BDSIM output to a user input file.
+• Support for energy variation in the beam line in MAD8 conversion.
+
+13.11.2 General
 • Remove dependency of root_numpy. pybdsim now uses only standard ROOT interfaces.
 • Update physics lists.
 
-13.10.3 Bug Fixes
+13.11.3 Bug Fixes
 • Fix bug where calling pybdsim.Plot.PrimaryPhaseSpace with an output file name would result in an error as
 this argument was wrongly supplied to the number of bins argument.
 • Fix for hidden scientific notation when using machine diagram.
 • Fix TH1 TH2 TH3 histogram x,y,z highedge variables in histogram loading. These were the lowedge duplicated, which was wrong.
 • Add missing variables from sampler data given changes in BDSIM.
 
-13.11 v1.9 - 2018 / 08 / 24
-13.11.1 General
+13.12 v1.9 - 2018 / 08 / 24
+13.12.1 General
 • Significant new tests.
 • Trajectory loading from BDSIM ROOT output.
 • Plot trajectories.
 • New padding function for 1D histogram to ensure lines in plots.
 • New value replacement function for histograms to ensure continuous line in log plots.
 • Control over aspect ration in default 2D histogram plots.
 • New classes for each element in the Builder.
 • Refactor of MadxTfs2Gmad to use new classes in Builder.
 
-13.11.2 Bug Fixes
+13.12.2 Bug Fixes
 • Fix orientation of 2D histograms in plotting.
 • Fix header information labels when writing field maps with reversed order.
 
-13.12 v1.8 - 2018 / 06 / 23
-13.12.1 General
+13.13 v1.8 - 2018 / 06 / 23
+13.13.1 General
 • Setup requires pytest-runner.
 • Introduction of testing.
 • Removed line wrapping written to GMAD files in Builder.
 • “PlotBdsimOptics” is now “BDSIMOptics” in the Plot module.
-• New comparison plots for arbitrary inputs from different tracking codes.
-• Prepare PTC coordinates from any BDSIM sampler.
 
-13.11. v1.9 - 2018 / 08 / 24
+13.12. v1.9 - 2018 / 08 / 24
 
 53
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
-13.12.2 Bug Fixes
+• New comparison plots for arbitrary inputs from different tracking codes.
+• Prepare PTC coordinates from any BDSIM sampler.
+
+13.13.2 Bug Fixes
 • Fixes for “Optics” vs “optics” naming change in ROOT files.
 
-13.13 v1.7 - 2018 / 06 / 30
-13.13.1 General
+13.14 v1.7 - 2018 / 06 / 30
+13.14.1 General
 • Can specify which dimension in Field class construction (i.e. ‘x’:’z’ instead of default ‘x’:’y’).
 
-13.13.2 Bug Fixes
+13.14.2 Bug Fixes
 • ‘nx’ and ‘ny’ were written the wrong way around from a 2D field map in pybdsim.
 
-13.14 v1.6 - 2018 / 05 / 23
-13.14.1 Bug Fixes
+13.15 v1.6 - 2018 / 05 / 23
+13.15.1 Bug Fixes
 • Fix machine diagram plotting from BDSIM survey.
 • Fix machine diagram searching with right-click in plots.
 
-13.15 v1.5 - 2018 / 05 / 17
-13.15.1 New Features
+13.16 v1.5 - 2018 / 05 / 17
+13.16.1 New Features
 • Function now public to create beam from Madx TFS file.
 • Improved searching for BDSAsciiData class.
 • Ability to easily write out beam class.
 • Plot phase space from any sampler in a BDSIM output file.
 • __version__ information in package.
 • Get a column from data irrespective of case.
 • Coded energy deposition plot. Use for example for labelling cyrogenic, warm and collimator losses.
 • Improved Transport BDSIM comparison.
 • Function to convert a line from a TFS file into a beam definition file.
 
-13.15.2 Bug Fixes
+54
+
+Chapter 13. Version History
+
+pybdsim Documentation, Release 3.3.0
+
+13.16.2 Bug Fixes
 • Fix library loading given changes to capitalisation in BDSIM.
 • Beam class now supports all BDSIM beam definitions.
 • Support all aperture shapes in Builder.
 • Fixes for loading optics given changes to capitalisation and BDSAsciiData class usage.
 • Fixes for collimator conversion from MADX.
 
-54
-
-Chapter 13. Version History
-
-pybdsim Documentation, Release 3.2.0
-
-13.16 v1.4 - 2018 / 10 / 04
-13.16.1 New Features
+13.17 v1.4 - 2018 / 10 / 04
+13.17.1 New Features
 • Full support for loading BDSIM output formats through ROOT.
 • Extraction of data from ROOT histograms to numpy arrays.
 • Simple histogram plotting from ROOT files.
 • Loading of sampler data and simple extraction of phase space data.
 • Line wrapping for elements with very long definitions.
 • Comparison plots standardised.
 • New BDSIM BDSIM comparison.
 • New BDSIM Mad8 comparison.
 • Support for changes to BDSIM data format variable renaming in V1.0
 
-13.16.2 Bug Fixes
+13.17.2 Bug Fixes
 • Correct conversion of all dispersion component for Beam.
 • Don’t write all multipole components if not needed.
 • Fixed histogram plotting.
 • Fixed conversion of coordinates in BDSIM2PtcInrays for subrelativistic particles.
 • Fixed behaviour of fringe field fint and fintx behaviour from MADX.
 • Fixed pole face angles given MADX writes out wrong angles.
 • Fixed conversion of multipoles and other components for ‘linear’ flag in MadxTfs2Gmad.
 • Fixed axis labels in field map plotting utilities.
 • MADX BDSIM testing suite now works with subrelativistic particles.
 • Many small fixes to conversion.
 
-13.17 v1.3 - 2017 / 12 / 05
-13.17.1 New Features
+13.17. v1.4 - 2018 / 10 / 04
+
+55
+
+pybdsim Documentation, Release 3.3.0
+
+13.18 v1.3 - 2017 / 12 / 05
+13.18.1 New Features
 • GPL3 licence introduced.
 • Compatibility with PIP install system.
 • Manual.
 • Testing suite.
 
-13.16. v1.4 - 2018 / 10 / 04
-
-55
-
-pybdsim Documentation, Release 3.2.0
-
 56
 
 Chapter 13. Version History
 
 CHAPTER
 
 FOURTEEN
@@ -2046,15 +2056,15 @@
 ReturnBeamString()
 SetDistributionType(distrType='reference')
 SetE0(e0=1, unitsstring='GeV')
 SetEnergy(energy=1.0, unitsstring='GeV')
 
 57
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 SetParticleType(particleType='e-')
 SetS0(s0=0, unitsstring='m')
 SetT0(t0=0.0, unitsstring='s')
 SetX0(x0=0.0, unitsstring='m')
 SetXP0(xp0=0.0)
 SetY0(y0=0.0, unitsstring='m')
@@ -2087,15 +2097,15 @@
 Bases: GmadObject
 A cavitymodel definition. Any kwargs will be written as parameter=value. parameter=(value,unit) -> parameter=value*unit
 
 58
 
 Chapter 14. Module Contents
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 pybdsim.Builder.CreateDipoleDriftRing(filename, ncells=60, circumference=100.0, driftfraction=0.1,
 samplers='first')
 Create a ring composed of dipoles and drifts filename ncells - number of cells, each containing 1 dipole and
 a drift circumference - in metres driftfraction - the fraction of drift in each cell (0.0 < driftfraction < 1.0)
 samplers - ‘first’, ‘last’ or ‘all’
 pybdsim.Builder.CreateDipoleFodoRing(filename, ncells=60, circumference=200.0,
@@ -2139,15 +2149,15 @@
 >>> print(b)
 (continues on next page)
 
 14.2. pybdsim.Builder module
 
 59
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 (continued from previous page)
 
 qx1f: quadrupole, k1=0.2, l=0.4*m, aper1=0.223*m;
 >>> str(c)
 qx1f: quadrupole, k1=0.2, l=0.4*m, aper1=0.223*m\n;
 A beam line element must ALWAYs have a name, and type. The keyword arguments are specific to the type
@@ -2188,15 +2198,15 @@
 Bases: GmadObject
 A field definition. Any kwargs will be written as parameter=value. parameteter=(value,unit) -> parameter=value*unit
 
 60
 
 Chapter 14. Module Contents
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 class pybdsim.Builder.Gap(name, l, **kwargs)
 Bases: Element
 pybdsim.Builder.GenerateSamplersFromBDSIMSurvey(surveyfile, outputfilename,
 excludesamplers=True)
 Create a gmad file with samplers for all the elements in a beamline as described by the survey outline from
 bdsim
@@ -2237,15 +2247,15 @@
 >>> f.write(l.DefineConsituentElements())
 >>> f.close()
 
 14.2. pybdsim.Builder module
 
 61
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 class pybdsim.Builder.Machine(verbose=False, sr=False, energy0=0.0, charge=-1.0)
 Bases: object
 A class represents an accelerator lattice as a sequence of components. Member functions allow various lattice
 components to be append to the sequence of the machine. This class allows the user to programatically create
 a lattice and write the BDSIM gmad representation of it.
 Example:
@@ -2286,15 +2296,15 @@
 - alternates between magnets
 kwargs are other parameters for bdsim - ie material=’Fe’
 
 62
 
 Chapter 14. Module Contents
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 AddFodoCellMultiple(basename='fodo', magnetlength=1.0, driftlength=4.0, kabs=0.2, ncells=2,
 **kwargs)
 AddFodoCellSplitDrift(basename, magnetlength, driftlength, kabs, nsplits, **kwargs)
 basename - the basename for the fodo cell beam line elements magnetlength - length of magnets in
 metres driftlength - length of drift segment in metres kabs - the absolute value of the quadrupole strength
 - alternates between magnets nsplits - number of segments drift length is split into
@@ -2333,15 +2343,15 @@
 AddQuadrupole(name='qd', length=0.1, k1=0.0, **kwargs)
 AddRBend(name='rb', length=0.1, angle=None, b=None, **kwargs)
 
 14.2. pybdsim.Builder module
 
 63
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 AddRCol(name='rc', length=0.1, xsize=0.1, ysize=0.1, **kwargs)
 AddRFCavity(name='arreff', length=0.1, gradient=10, **kwargs)
 AddRmat(name='rmat', length=0.1, r11=1.0, r12=0, r13=0, r14=0, r21=0, r22=1.0, r23=0, r24=0,
 r31=0, r32=0, r33=1.0, r34=0, r41=0, r42=0, r43=0, r44=1.0, **kwargs)
 AddSBend(name='sb', length=0.1, angle=None, b=None, **kwargs)
 AddSampler(names)
@@ -2378,15 +2388,15 @@
 SynchrotronRadiationRescale()
 Rescale all component strengths for SR
 
 64
 
 Chapter 14. Module Contents
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 UpdateCategoryParameter(category, parameter, value)
 Update parameter for all elements of a given category.
 UpdateElement(name, parameter, value)
 Update a parameter for a specified element name. Modifying element length will produce a warning.
 If a value for that parameter already exists, the value will be overwritten.
 UpdateElements(names, parameter, value, namelocation='all')
@@ -2424,15 +2434,15 @@
 class pybdsim.Builder.Quadrupole(name, l, k1, **kwargs)
 Bases: Element
 
 14.2. pybdsim.Builder module
 
 65
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 class pybdsim.Builder.Query(name, **kwargs)
 Bases: GmadObject
 A query definition. Any kwargs will be written as parameter=value. parameter=(value,unit) -> parameter=value*unit
 class pybdsim.Builder.RBend(name, l, angle=None, B=None, **kwargs)
 Bases: _Dipole
 class pybdsim.Builder.RCol(name, l, xsize, ysize, **kwargs)
@@ -2468,15 +2478,15 @@
 class pybdsim.Builder.Solenoid(name, l, ks, **kwargs)
 Bases: Element
 
 66
 
 Chapter 14. Module Contents
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 pybdsim.Builder.SuggestFodoK(magnetlength, driftlength)
 returns k1 (float) value for matching into next quad in a FODO cell. f = 1/(k1 * magnetlength) = driftlength
 -> solve for k1
 Note the convention in pybdsim.Builder is that the quadrupoles in the fodo cell are split in two. So this is in
 fact half the integrated k you need. This matches with the other functions in Builder.
 class pybdsim.Builder.TKicker(name, hkick, vkick, **kwargs)
@@ -2509,15 +2519,15 @@
 5), saveAll=True, outputFileName=None)
 Compares MadX and BDSIM optics variables. User must provide a tfsoptIn file or Tfsinstance and a BDSAscii file or instance.
 
 14.3. pybdsim.Compare
 
 67
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 Parameters
 tfs
 bdsim
 survey
 functions
 figsize
@@ -2561,15 +2571,15 @@
 particle tree.
 Parameters
 
 68
 
 Chapter 14. Module Contents
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 • inputfile (str) – root format output from BDSIM run
 • outfile (str) – filename for the inrays file
 • start (int) – starting primary particle index
 • ninrays (int) – total number of inrays to generate, default is all available
 pybdsim.Convert.BdsimPrimaries2Ptc(inputfile, outfile=None, start=0, ninrays=-1)
 Takes .root file generated from a BDSIM run an an input and creates a PTC inrays file from the primary
@@ -2593,15 +2603,15 @@
 Returns two pybdsim.Builder.Machine instances. The first desired full conversion. The second is the raw
 conversion that’s not split by aperture. Thirdly, a list of the names of the omitted items is returned.
 
 14.5. pybdsim.Convert
 
 69
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 tfs
 outputfilename
 startname
 
 stopname
 
@@ -2674,15 +2684,15 @@
 containContents
 a dictio14.and
 Module
 nary itself with key, value pairs of parameters and
 values to be added to that particular element.
 A python dictionary of dictionaries. The key is a
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 pybdsim.Convert.MadxTfs2GmadStrength(input, outputfilename, existingmachine=None, verbose=False,
 flipmagnets=False, linear=False, allNamesUnique=False,
 ignoreZeroLengthItems=True)
 Use a MADX Tfs file containing full twiss information to generate a strength (only) BDSIM GMAD file to
 be used with an existing lattice.
 existingmachine
@@ -2710,15 +2720,15 @@
 Returns two pybdsim.Builder.Machine instances. The first desired full conversion. The second is the raw
 conversion that’s not split by aperture. Thirdly, a list of the names of the omitted items is returned.
 
 14.5. pybdsim.Convert
 
 71
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 tfs
 outputfilename
 startname
 
 stopname
 
@@ -2791,15 +2801,15 @@
 containContents
 a dictio14.and
 Module
 nary itself with key, value pairs of parameters and
 values to be added to that particular element.
 A python dictionary of dictionaries. The key is a
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 pybdsim.Convert._MadxTfs2Gmad.MadxTfs2GmadBeam(tfs, startname=None, verbose=False,
 extraParamsDict={})
 Takes a pymadx.Data.Tfs instance and extracts information from first line to create a BDSIM beam definition
 in a pybdsim.Beam object. Note that if kwarg startname is used, the optics are retrieved at the start of the
 element, i.e. you do not need to get the optics of the previous element, this function does that automatically.
 Works for e+, e- and proton. Default emittance is 1e-9mrad if 1 in tfs file.
@@ -2839,15 +2849,15 @@
 You can therefore used to match any parameter.
 Return type is BDSAsciiData
 
 14.6. pybdsim.Data module
 
 73
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 NameFromNearestS(S)
 ToDF()
 Get this BDSAsciiData instance as a pandas.DataFrame instance.
 class pybdsim.Data.BDSBH4D(hist, extractData=True)
 Bases: object
 Wrapper for a BDSBH instance. Converts to numpy data.
@@ -2872,30 +2882,47 @@
 Bases: object
 Extract data from the Info branch of the Event tree.
 classmethod FromROOTFile(path)
 class pybdsim.Data.EventSummaryData(data)
 Bases: EventInfoData
 Extract data from the Summary branch of the Event tree.
 pybdsim.Data.GetApertureExtent(apertureType, aper1=0, aper2=0, aper3=0, aper4=0)
+pybdsim.Data.GetHistoryPDGTuple(trajectories, startingTrajectoryStorageIndex, reduceDuplicates=False)
+Return a tuple of PDG IDs for the history of a particle given by trajectories in an event.
+Parameters
+• trajectories (event.Trajectory) – event.Trajectory instance from loaded ROOT
+data
+• startingTrajectoryStorageIndex (int) – storage index of which trajectory to start
+from
+• reduceDuplicates (bool) – whether to remove sequential duplicates from the history
+
+74
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.3.0
+
+>>> d = pybdsim.Data.Load("somdbdsimoutputfile.root")
+>>> et = d.GetEventTree()
+>>> for event in et:
+tid = event.sampler1.trackID[0]
+history = pybdsim.Data.GetHistoryPDGTuple(event.Trajectory, tid)
+print(history)
+An example might be (13,211,211,2212) or with reducedDuplicates (31,211,2212)
+Note, this will raise an IndexError if you haven’t stored the right trajectories. and must be used knowing that
+the connected trajectories for a given starting trackID are stored.
 pybdsim.Data.GetModelForPlotting(rootFile, beamlineIndex=0)
 Returns BDSAsciiData object with just the columns from the model for plotting.
 pybdsim.Data.GetNEventsInBDSIMFile(filename)
 Utility function to extract the number of events in a file quickly without fully loading it. Uses only ROOT to
 inspect the tree. Will raise an IOError exception if no Event tree is found. No check if it’s a BDSIM format
 file or not.
 class pybdsim.Data.Header(**kwargs)
 Bases: object
 A simple Python version of a header in a (RE)BDSIM file for easy access to the data.
-
-74
-
-Chapter 14. Module Contents
-
-pybdsim Documentation, Release 3.2.0
-
 class pybdsim.Data.Histogram1DSet(name=None)
 Bases: object
 Basic histogram for a categorical axis with a dict / map as the storage.
 This is completely agnostic of the type of the value used as the axis.
 It is ultimately a python dict[key] = (value, sumWeightsSq) where ‘key’ is the ‘x’ used to file the histogram.
 The bin errors can be accessed by calling Result() to return a dictionary of key : (value, error)
 h = Histogram1DSet(“PDG_ID”) h.Fill(2212) h.Fill(-13)
@@ -2910,14 +2937,21 @@
 value is the bin value. error is calculated as sqrt(sum(weights^2)/n) for the sum of the weights squared
 in an individual bin.
 ResultMean()
 return a dictionary of key : (mean, error)
 mean is the bin value / n error is calculated as sqrt(1/n * sum(weights^2)/n) for the sum of the weights
 squared in an individual bin.
 SortByBin()
+
+14.6. pybdsim.Data module
+
+75
+
+pybdsim Documentation, Release 3.3.0
+
 pybdsim.Data.Load(filepath)
 Load the data with the appropriate loader.
 ASCII file - returns BDSAsciiData instance. BDSIM file - uses ROOT, returns BDSIM DataLoader instance.
 REBDSIM file - uses ROOT, returns RebdsimFile instance.
 pybdsim.Data.LoadPickledObject(filename)
 Unpickle an object. If the name contains .pbz2 the bz2 library will be used as well to load the compressed
 pickled object.
@@ -2929,21 +2963,14 @@
 returns dict{columnname:1d numpy array}
 class pybdsim.Data.ModelData(data)
 Bases: object
 A python versio of the data held in a Model tree in BDSIM output.
 d = pybdsim.Data.Load(“output.root”) md = pybdsim.Data.ModelData(d)
 Extracts this from a bdsim output file.
 classmethod FromROOTFile(path)
-
-14.6. pybdsim.Data module
-
-75
-
-pybdsim Documentation, Release 3.2.0
-
 GetApertureData(removeZeroLength=False, removeZeroApertures=True, lengthTolerance=1e-06)
 return a list of aperture instances along with coordinates: l,s,x,y,apertures l - length of element s curvilinear S coordinate at the end of the element x - horizontal extent y - vertical extent apertures =
 [ApertureInfo]
 PrepareAxisAngleRotations()
 class pybdsim.Data.OptionsData(data)
 Bases: object
 classmethod FromROOTFile(path)
@@ -2959,14 +2986,21 @@
 Extracts only: ‘x’,’xp’,’y’,’yp’,’z’,’zp’,’energy’,’T’
 Can either supply the sampler name or index as the optional second argument. The index is 0 counting
 including the primaries (ie +1 on the index in data.GetSamplerNames()). Examples:
 >>> f = pybdsim.Data.Load("file.root")
 >>> primaries = pybdsim.Data.PhaseSpaceData(f)
 >>> samplerfd45 = pybdsim.Data.PhaseSpaceData(f, "samplerfd45")
 >>> thirdAfterPrimaries = pybdsim.Data.PhaseSpaceData(f, 3)
+
+76
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.3.0
+
 pybdsim.Data.PickleObject(ob, filename, compress=True)
 Write an object to a pickled file using Python pickle.
 If compress is True, the bz2 package will be imported and used to compress the file.
 class pybdsim.Data.ROOTHist(hist)
 Bases: object
 Base class for histogram wrappers.
 ErrorsToErrorOnMean()
@@ -2977,21 +3011,14 @@
 standard deviation. Will automatically only apply itself once even if repeatedly called.
 class pybdsim.Data.RebdsimFile(filename, convert=True, histogramsOnly=False)
 Bases: object
 Class to represent data in rebdsim output file.
 Parameters
 • filename (str) – File to load
 • convert (bool) – Whether to ROOT histograms to pybdsim ones as well
-
-76
-
-Chapter 14. Module Contents
-
-pybdsim Documentation, Release 3.2.0
-
 • histogramsOnly (bool) – If true, then don’t load rebdsim libraries and only load histograms.
 Contains histograms as root objects. Conversion function converts to pybdsim.Rebdsim.THX classes holding
 numpy data.
 If optics data is present, this is loaded into self.Optics which is BDSAsciiData instance.
 If convert=True (default), root histograms are automatically converted to classes provided here with numpy
 data.
 If histogramsOnly is true, only the basic ROOT libraries are needed (i.e. import ROOT) and no Model data
@@ -3008,14 +3035,21 @@
 List all trees inside the root file.
 pybdsim.Data.ReplaceZeroWithMinimum(hist, value=1e-20)
 Replace zero values with given value. Useful for log plots.
 For log plots we want a small but +ve number instead of 0 so the line is continuous on the plot. This is also
 required for padding to work for the edge of the lines.
 Works for TH1, TH2, TH3.
 returns a new instance of the pybdsim.Data.TH1, TH2 or TH3.
+
+14.6. pybdsim.Data module
+
+77
+
+pybdsim Documentation, Release 3.3.0
+
 pybdsim.Data.SDDSBuildParameterDicts(sddsColumnDict)
 Use first the LoadSDDSColumnsToDict on a parameters file. Then call this function to sort it into ElementName : {ParameterName:ParameterValue}. An extra key will be added that is KEYWORD for the
 ElementType in the inner dictionary.
 class pybdsim.Data.SamplerData(data, samplerIndexOrName=0)
 Bases: _SamplerData
 Pull sampler data from a loaded DataLoader instance of raw data for all events.
 Loads all data in a given sampler.
@@ -3024,21 +3058,14 @@
 >>> f = pybdsim.Data.Load("file.root")
 >>> primaries = pybdsim.Data.SamplerData(f)
 >>> samplerfd45 = pybdsim.Data.SamplerData(f, "samplerfd45")
 >>> thirdAfterPrimaries = pybdsim.Data.SamplerData(f, 3)
 class pybdsim.Data.Spectra(nameIn=None)
 Bases: object
 append(pdgid, hist, path, nameIn=None, flag=None)
-
-14.6. pybdsim.Data module
-
-77
-
-pybdsim Documentation, Release 3.2.0
-
 class pybdsim.Data.TH1(hist, extractData=True)
 Bases: ROOTHist
 Wrapper for a ROOT TH1 instance. Converts to numpy data.
 >>> h = file.Get("histogramName")
 >>> hpy = TH1(h)
 Rebin(nBins)
 class pybdsim.Data.TH2(hist, extractData=True)
@@ -3054,14 +3081,21 @@
 SwapAxes()
 Swap X and Y for all members. Returns a new copy of the histogram.
 class pybdsim.Data.TH3(hist, extractData=True)
 Bases: TH2
 Wrapper for a ROOT TH3 instance. Converts to numpy data.
 >>> h = file.Get("histogramName")
 >>> hpy = TH3(h)
+
+78
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.3.0
+
 IntegateAlong1Dimension(dimension)
 Integrate along a dimension returning a new 2D histogram.
 Parameters
 dimension (str) – ‘x’, ‘y’ or ‘z’ dimension to integrate along
 returns pybdsim.Data.TH2 instance.
 If the projection is done in z, a 2D histogram of x,y is returned that is the sum of the bins along z. The
 errors are also calculated.
@@ -3071,21 +3105,14 @@
 Parameters
 resultDimension (str) – ‘x’, ‘y’ or ‘z’ dimension to produce 1D histogram along.
 returns pybdsim.Data.TH1 instance.
 Slice2DXY(index)
 Extract a single 2D histogram from an index along the Z dimension.
 Parameters
 index (int) – index in z array of bins to extract, e.g. 0 -> nbinsz-1
-
-78
-
-Chapter 14. Module Contents
-
-pybdsim Documentation, Release 3.2.0
-
 Slice2DXZ(index)
 Extract a single 2D histogram from an index along the Y dimension.
 Parameters
 index (int) – index in y array of bins to extract, e.g. 0 -> nbinsy-1
 Slice2DZY(index)
 Extract a single 2D histogram from an index along the X dimension.
 Parameters
@@ -3102,35 +3129,33 @@
 next()
 pybdsim.Data.WriteROOTHistogramsToDirectory(tfile, directoryName, histograms)
 Parameters
 • tfile (ROOT.TFile.) – TFile object to write to.
 • directoryName (str (e.g. "Event/PerEntryHistograms" )) – Full path of directory you wish to write the histograms to.
 • histograms ([ROOT.TH1,..]) – List of ROOT histograms to write.
 Write a list of histograms (ROOT.TH*) to a directory (str) in a ROOT.TFile instance.
+14.6. pybdsim.Data module
+
+79
+
+pybdsim Documentation, Release 3.3.0
 
 14.7 pybdsim.Field module
 Utilities to convert and prepare field maps.
 Most of the plots assume magnetic fields for the labels, but they work equally well for electric fields.
 class pybdsim.Field._Field.Field(array=array([], dtype=float64), columns=[], flip=False,
 doublePrecision=False)
 Bases: object
 Base class used for common writing procedures for BDSIM field format.
 This does not support arbitrary loop ordering - only the originally intended xyzt.
 AddComment(commentString)
 Add a string that will be put on a comment line at the beginning of the file.
 Write(fileName, writeLoopOrderReversed=False, overrideLoopOrder=None)
 Parameters
 • writeLoopOrderReversed (bool) – Write this field map with the other loop order.
-
-14.7. pybdsim.Field module
-
-79
-
-pybdsim Documentation, Release 3.2.0
-
 • overrideLoopOrder (str) – string to write irrespective of internal data as the loop
 order.
 gzip - if the file ends with “.gz” the file will be compressed automatically.
 For overrideLoopOrder it should be only ‘xyzt’ or ‘tzyx’. This option is provided in case a field is
 prepared in the other order somehow and you want to control the writing of this header variable independently.
 WriteFLUKA2DFormat1(fileName)
 Write one of the FLUKA formats (x,y,Bx,by) in cm,T with no header.
@@ -3149,14 +3174,21 @@
 Bases: Field
 Utility class to write a 2D field map array to BDSIM field format.
 The array supplied should be 3 dimensional. Dimensions are: (x,y,value) where value has 5 elements
 [x,y,fx,fy,fz]. So a 100x50 (x,y) grid would have np.shape of (100,50,5).
 Example:
 >>> a = Field2D(data) # data is a prepared array
 >>> a.Write('outputFileName.dat')
+
+80
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.3.0
+
 The ‘flip’ boolean allows an array with (y,x,value) dimension order to be written as (x,y,value). Values must
 still be (x,y,fx,fy,fz).
 The ‘doublePrecision’ boolean controls whether the field and spatial values are written to 16 s.f. (True) or 8
 s.f. (False - default).
 class pybdsim.Field._Field.Field3D(data, flip=False, doublePrecision=False, firstColumn='X',
 secondColumn='Y', thirdColumn='Z')
 Bases: Field
@@ -3164,21 +3196,14 @@
 The array supplied should be 4 dimensional. Dimensions are: (x,y,z,value) where value has 6 elements
 [x,y,z,fx,fy,fz]. So a 100x50x30 (x,y,z) grid would have np.shape of (100,50,30,6).
 Example:
 >>> a = Field3D(data) # data is a prepared array
 >>> a.Write('outputFileName.dat')
 The ‘flip’ boolean allows an array with (z,y,x,value) dimension order to be written as (x,y,z,value). Values
 must still be (x,y,fx,fy,fz).
-
-80
-
-Chapter 14. Module Contents
-
-pybdsim Documentation, Release 3.2.0
-
 The ‘doublePrecision’ boolean controls whether the field and spatial values are written to 16 s.f. (True) or 8
 s.f. (False - default).
 class pybdsim.Field._Field.Field4D(data, flip=False, doublePrecision=False)
 Bases: Field
 Utility class to write a 4D field map array to BDSIM field format.
 The array supplied should be 5 dimensional. Dimensions are: (t,y,z,x,value) where value has 7 elements
 [x,y,z,t,fx,fy,fz]. So a 100x50x30x10 (x,y,z,t) grid would have np.shape of (10,30,50,100,7).
@@ -3201,35 +3226,35 @@
 3
 
 1
 4
 
 Parameters
 field2D (pybdsim.Field._Field.Field2D instance) – field object
+
+14.7. pybdsim.Field module
+
+81
+
+pybdsim Documentation, Release 3.3.0
+
 returns an instance of the same type.
 For a 2D field (i.e. function of x,y but can include Bx,By,Bz), for the quadrant number 1, mirror it and
 generate a bigger field for all four quadrants.
 1. original data
 2. data mirrored in x, (x,Bx) *= -1
 3. data mirrored in x,y, (x,y,By) *= -1
 4. data mirrored in y, (y,Bx) *= -1
 This is based on a dipole field.
 pybdsim.Field._Field.SortUnorderedFieldMap2D(field)
 Rearrange the data in a 2D field map to be in a linearly progressing loop of (x,y). In future this could be
 generalised to more dimensions and also any two dimensions, not just x,y.
 Parameters
 field (pybdsim.Field.Field2D) – Incoming jumbled field map
 Returns a new Field2D object
-
-14.7. pybdsim.Field module
-
-81
-
-pybdsim Documentation, Release 3.2.0
-
 class pybdsim.Field.FieldPlotter.FourDData(filename, xind=0, yind=1, zind=2, tind=3)
 Class purely to simplify plotting of fields. Not for general use.
 class pybdsim.Field.FieldPlotter.OneDData(filename)
 Class purely to simplify plotting of fields. Not for general use.
 pybdsim.Field.FieldPlotter.Plot1DFxFyFz(filename)
 Plot a bdsim 1D field map file.
 Parameters
@@ -3252,34 +3277,34 @@
 pybdsim.Field.FieldPlotter.Plot2DXY(filename, scale=None, title=None, flipX=False,
 firstDimension='X', secondDimension='Y', aspect='equal',
 figsize=(6, 5))
 Plot a bdsim field map file using the X,Y plane.
 Parameters
 • filename (str, pybdsim.Field._Field.Field2D instance) – name of field
 map file or object
+82
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.3.0
+
 • scale (float) – numerical scaling for quiver plot arrow lengths.
 • title (str) – title for plot
 • flipX (bool) – whether to plot x backwards to match the right hand coordinate system
 of Geant4.
 • firstDimension (str) – Label of first dimension, e.g. “X”
 • secondDimension (str) – Label of second dimension, e.g. “Z”
 • aspect (str) – Matplotlib axes aspect (e.g. ‘auto’ or ‘equal’)
 pybdsim.Field.FieldPlotter.Plot2DXYBx(filename, scale=None, title=None, flipX=False,
 aspect='equal')
 Plot a bdsim field map file use the X,Y plane, but plotting By component.
 Parameters
 • filename (str, pybdsim.Field._Field.Field2D instance) – name of field
 map file or object
 • scale (float) – numerical scaling for quiver plot arrow lengths.
-82
-
-Chapter 14. Module Contents
-
-pybdsim Documentation, Release 3.2.0
-
 • title (str) – title for plot
 • aspect (str) – Matplotlib axes aspect (e.g. ‘auto’ or ‘equal’)
 pybdsim.Field.FieldPlotter.Plot2DXYBy(filename, scale=None, title=None, flipX=False,
 aspect='equal')
 Plot a bdsim field map file use the X,Y plane, but plotting By component.
 Parameters
 • filename (str, pybdsim.Field._Field.Field2D instance) – name of field
@@ -3300,14 +3325,21 @@
 title=None, flipX=False, aspect='equal')
 Plot a bdsim field map file use the X,Y plane, but plotting By component.
 Parameters
 • filename (str, pybdsim.Field._Field.Field2D instance) – name of field
 map file or object
 • componentIndex (int) – index of field component (0,1,2) for Fx, Fy, Fz
 • scale (float) – numerical scaling for quiver plot arrow lengths.
+
+14.7. pybdsim.Field module
+
+83
+
+pybdsim Documentation, Release 3.3.0
+
 • title (str) – title for plot
 • aspect (str) – Matplotlib axes aspect (e.g. ‘auto’ or ‘equal’)
 pybdsim.Field.FieldPlotter.Plot2DXYConnectionOrder(filename)
 Plot a point in orange and a line in blue (default matplotlib colours) for each locationin the field map. If the
 field map is constructed correctly, this should show a set of lines with diagonals between them. The other
 plots with the arrows are independent of order unlike when BDSIM loads the fields. So you might see an
 OK field map, but it could be wrong if hand written.
@@ -3315,21 +3347,14 @@
 **imshowKwargs)
 Plot Fx,Fy,Fz components of a field separately as a function of X,Y.
 Parameters
 • filename (str, pybdsim.Field._Field.Field1D instance) – name of field
 map file or object
 • title (None, str) – optional title for plot
 • aspect (str) – aspect ratio for matplotlib imshow
-
-14.7. pybdsim.Field module
-
-83
-
-pybdsim Documentation, Release 3.2.0
-
 • extent (list,tuple) – list or tuple of (xmin,xmax,ymin,ymax) for each plot (optional)
 pybdsim.Field.FieldPlotter.Plot2DXYMagnitude(filename, title=None, flipX=False,
 firstDimension='X', secondDimension='Y',
 aspect='equal', zlabel='|$B_{x,y}$| (T)', figsize=(6,
 5))
 Plot a the magnitude of a 2D bdsim field map file using any two planes.
 Parameters
@@ -3349,14 +3374,21 @@
 • filename (str, pybdsim.Field._Field.Field2D or Field3D instance) –
 name of field map file or object
 • density (float) – arrow density (default=1) for matplotlib streamplot
 • zIndexIf3D (int) – index in Z if using 3D field map (default=0)
 • useColour (bool :param aspect: Matplotlib axes aspect (e.g. 'auto'
 or 'equal')) – use magnitude of field as colour.
 Note, matplotlibs streamplot may raise an exception if the field is entriely 0 valued.
+
+84
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.3.0
+
 pybdsim.Field.FieldPlotter.Plot2DXZStream(filename, density=1, yIndexIf3D=0, useColour=True,
 aspect='equal')
 Plot a bdsim field map file using the X,Z plane as a stream plot and plotting Fx, Fz.
 Parameters
 • filename (str, pybdsim.Field._Field.Field2D or Field3D instance) –
 name of field map file or object
 • density (float) – arrow density (default=1) for matplotlib streamplot
@@ -3364,21 +3396,14 @@
 • useColour (bool) – use magnitude of field as colour.
 • aspect (str) – Matplotlib axes aspect (e.g. ‘auto’ or ‘equal’)
 Note, matplotlibs streamplot may raise an exception if the field is entriely 0 valued.
 pybdsim.Field.FieldPlotter.Plot3DXY(filename, scale=None)
 Plots (B_x,B_y) as a function of x and y.
 pybdsim.Field.FieldPlotter.Plot3DXZ(filename, scale=None)
 Plots (B_x,B_z) as a function of x and z.
-
-84
-
-Chapter 14. Module Contents
-
-pybdsim Documentation, Release 3.2.0
-
 class pybdsim.Field.FieldPlotter.ThreeDData(filename)
 Class purely to simplify plotting of fields. Not for general use.
 class pybdsim.Field.FieldPlotter.TwoDData(filename)
 Class purely to simplify plotting of fields. Not for general use.
 
 14.8 pybdsim.Gmad module
 Survey() - survey a gmad lattice, plot element coords
@@ -3396,14 +3421,21 @@
 Class to load a gmad components file to a buffer and modify the contents
 Example : python> g = pybdsim.Gmad.GmadFileComponents(“./atf2_components.gmad”) python>
 g.change(“KEX1A”,”l”,”10”) python> g.write(“./atf2_components.gmad”)
 change(element, parameter, value)
 Edit element dictionary
 elementNames()
 Make a list of element names, stored in self.elementNameList
+
+14.8. pybdsim.Gmad module
+
+85
+
+pybdsim Documentation, Release 3.3.0
+
 findElement(elementName)
 Returns the start and end (inclusive location of the element lines as a tuble (start,end)
 getParameter(element, parameter)
 Edit element dictionary
 getType(element)
 parseElement(elementString)
 Create element dictionary from element
@@ -3412,21 +3444,14 @@
 Bases: object
 Class to load a gmad options file to a buffer and modify the contents
 class pybdsim.Gmad.Lattice(filename=None)
 Bases: object
 BDSIM Gmad parser lattice.
 Use this class to load a bdsim input file using the BDSIM parser (GMAD) and then interrogate it. You can
 use this to regenerate a lattice with less information for example
-
-14.8. pybdsim.Gmad module
-
-85
-
-pybdsim Documentation, Release 3.2.0
-
 >>> a = Lattice("filename.gmad")
 or
 >>> a = Lattice()
 >>> a.Load("filename.gmad")
 >>> a # this will tell you some basic details
 >>> print(a) # this will print out the full lattice
 GetAllNames()
@@ -3440,35 +3465,35 @@
 GetColumn(column)
 GetElement(i)
 GetIndexOfElementNamed(elementname)
 GetKs(index)
 GetLength(index)
 GetName(index)
 GetType(index)
+
+86
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.3.0
+
 IndexFromNearestS(S)
 return the index of the beamline element clostest to S
 Load(filename)
 Load the BDSIM input file and parse it using the BDSIM parser (GMAD).
 ParseLattice()
 Put lattice data into python data structure
 Print(includeheaderlines=True)
 PrintZeroLength(includeheaderlines=True)
 Print elements with zero length with s location
 next()
 class pybdsim.Gmad.Survey(filename=None)
 Bases: object
 Survey - load a gmad lattice and have a look
 Example:
-
-86
-
-Chapter 14. Module Contents
-
-pybdsim Documentation, Release 3.2.0
-
 >>> a = Survey()
 >>> a.Load('mylattice.gmad')
 >>> a.Plot()
 CompareMadX(fileName)
 FinalDiff()
 FindClosestElement(coord)
 Load(filename)
@@ -3487,32 +3512,31 @@
 Inspect pybdsim.Data.ModelData assuming collimator info was stored to give an axis aligned bounding box
 set of ranges in global coordinates.
 pybdsim.ModelProcessing.GetMaterialIDOfCollimator(modelData, collimatorName)
 Inspect pybdsim.Data.ModelData assuming collimator info was stored to give an axis aligned bounding box
 set of ranges in global coordinates.
 pybdsim.ModelProcessing.WrapLatticeAboutItem(maingmadfile, itemname, outputfilename)
 
+14.9. pybdsim.ModelProcessing module
+
+87
+
+pybdsim Documentation, Release 3.3.0
+
 14.10 pybdsim.Options module
 See Options class inside this module.
 pybdsim.Options.ElectronColliderOptions()
 class pybdsim.Options.Options(*args, **kwargs)
 Bases: dict
 Inherits a dict. Converting to a string or using ReturnOptionsString() will give a suitable GMAD string to
 write out to a file.
 o = pybdsim.Options.Options() o[“trajectoryConnect”] = 1 o[“aper1”] = (5, ‘m’) str(o) ‘option, trajectoryConnect=1,
 aper1=5*m;’
 There is no checking on the option if using []. A tuple of (value, unitsString) can be used too resulting in
 value*unitsString.
-
-14.9. pybdsim.ModelProcessing module
-
-87
-
-pybdsim Documentation, Release 3.2.0
-
 ReturnOptionsString()
 SetBLMLength(length=50.0, unitsstring='cm')
 SetBLMRadius(radius=5.0, unitsstring='cm')
 SetBeamPipeRadius(beampiperadius=5.0, unitsstring='cm')
 SetBeamPipeThickness(bpt, unitsstring='mm')
 SetBeamlineS(beamlineS=0, unitsstring='m')
 SetBuildTunnel(tunnel=False)
@@ -3528,31 +3552,31 @@
 SetDontSplitSBends(dontsplitsbends=False)
 SetELossHistBinWidth(width)
 SetEMLeadParticleBiasing(on=True)
 SetEPAnnihilation2HadronEnhancementFactor(ef=1.0)
 SetEPAnnihilation2MuonEnhancementFactor(ef=1.0)
 SetGamma2MuonEnahncementFactor(ef=1.0)
 SetGeneralOption(option, value)
+
+88
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.3.0
+
 SetIncludeFringeFields(on=True)
 SetIncludeIronMagField(iron=True)
 SetIntegratorSet(integratorSet='"bdsim"')
 SetLPBFraction(fraction=0.5)
 SetLengthSafety(ls=10.0, unitsstring='um')
 SetMagnetGeometryType(magnetGeometryType='"none"')
 SetMaximumEpsilonStep(mes=1.0, unitsstring='m')
 SetMaximumStepLength(msl=20.0, unitsstring='m')
 SetMaximumTrackingTime(mtt=-1.0, unitsstring='s')
 SetMinimumEpsilonStep(mes=10.0, unitsstring='nm')
-
-88
-
-Chapter 14. Module Contents
-
-pybdsim Documentation, Release 3.2.0
-
 SetNGenerate(nparticles=10)
 SetNLinesIgnore(nlines=0)
 SetNPerFile(nperfile=100)
 SetOuterDiameter(outerdiameter=2.0, unitsstring='m')
 SetPhysicsList(physicslist='')
 SetPipeMaterial(bpm)
 SetPrintModuloFraction(pmf=0.01)
@@ -3568,31 +3592,31 @@
 SetSenssitiveBLMs(on=True)
 SetSoilMaterial(sm)
 SetSoilThickness(st=4.0, unitsstring='m')
 SetStopSecondaries(stop=True)
 SetStoreTrajectory(on=True)
 SetStoreTrajectoryParticle(particle='muon')
 SetSynchRadiationOn(on=True)
+
+14.10. pybdsim.Options module
+
+89
+
+pybdsim Documentation, Release 3.3.0
+
 SetThresholdCutCharged(tcc=100.0, unitsstring='MeV')
 SetThresholdCutPhotons(tcp=1.0, unitsstring='MeV')
 SetTrackSRPhotons(track=True)
 SetTrajectoryCutGTZ(gtz=0.0, unitsstring='m')
 SetTrajectoryCutLTR(ltr=10.0, unitsstring='m')
 SetTunnelFloorOffset(offset=1.0, unitsstring='m')
 SetTunnelMaterial(tm)
 SetTunnelOffsetX(offset=0.0, unitsstring='m')
 SetTunnelOffsetY(offset=0.0, unitsstring='m')
 SetTunnelRadius(tunnelradius=2.0, unitsstring='m')
-
-14.10. pybdsim.Options module
-
-89
-
-pybdsim Documentation, Release 3.2.0
-
 SetTunnelThickness(tt=1.0, unitsstring='m')
 SetVacuumMaterial(vm)
 SetVacuumPressure(vp)
 Vacuum pressure in bar
 SetWritePrimaries(on=True)
 pybdsim.Options.ProtonColliderOptions()
 
@@ -3615,34 +3639,34 @@
 pybdsim.Plot.AddMachineLatticeFromSurveyToFigureMultiple(figure, machines, tightLayout=True)
 Similar to AddMachineLatticeFromSurveyToFigure() but accepts multiple machines.
 pybdsim.Plot.Aperture(rootFileName, filterThin=False, surveyFileName=None)
 pybdsim.Plot.BDSIMAperture(data, machineDiagram=True, plot='xy', plotApertureType=True,
 removeZeroLength=False, removeZeroApertures=True)
 Plot the aperture from a BDSIM DataLoader instance. By default it’s colour coded and excludes any 0
 aperture elements. Zero length elements are included.
+
+90
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.3.0
+
 pybdsim.Plot.BDSIMApertureFromFile(filename, machineDiagram=True, plot='xy',
 plotApertureType=True, removeZeroLength=False,
 removeZeroApertures=True)
 Plot the aperture from a BDSIM output file. By default it’s colour coded and excludes any 0s.
 pybdsim.Plot.BDSIMOptics(rebdsimOpticsOutput, outputfilename=None, saveall=True, survey=None,
 **kwargs)
 Display all the optical function plots for a rebdsim optics root file. By default, this saves all optical functions
 into a single (outputfilename) pdf, to save the optical functions separately, supply an outputfilename with
 saveall=false.
 pybdsim.Plot.DrawMachineLattice(axesinstance, bdsasciidataobject, sOffset=0.0)
 The low-level version of drawing a machine diagram. Draws into an axes instance given using loaded model
 data in the form of a pybdsim.Data.BDSAsciiData instance.
 Parameters
-
-90
-
-Chapter 14. Module Contents
-
-pybdsim Documentation, Release 3.2.0
-
 • axesinstance (matplotlib.axes.Axes) – the plotting axis to draw the machine diagram into.
 • sOffset (float) – add this value to the S of all machine elements in the diagram.
 Param
 bdsasciidataobject The model data.
 The main interface is AddMachineLatticeFromSurveyToFigure, but this function may be useful for more
 granular plotting, e.g. with custom subfigures / axes.
 pybdsim.Plot.EnergyDeposition(filename, outputfilename=None, tfssurvey=None, bdsimsurvey=None)
@@ -3665,34 +3689,34 @@
 file with the plot. Default is None.
 tfssurvey (str, optional): Path to MADX survey used to plot machine diagram on top of figure. Default
 is None.
 tfssurvey (str, optional): Path to BDSIM survey used to classify losses into collimator/warm/cold and/or
 plot machine diagram on top of figure. Default is None.
 warmaperinfo (int|list|str, optional): Information about warm aperture in the machine. Default is None.
 **kwargs: Arbitrary keyword arguments.
+
+14.11. pybdsim.Plot module
+
+91
+
+pybdsim Documentation, Release 3.3.0
+
 Kwargs:
 skipMachineLattice (bool): If enabled, use the BDSIM survey to classify losses, but do not plot the
 lattice on top.
 Returns:
 matplotlib.pyplot.Figure object
 pybdsim.Plot.Histogram1D(histogram, xlabel=None, ylabel=None, title=None, scalingFactor=1.0,
 xScalingFactor=1.0, figsize=(6.4, 4.8), log=False, **errorbarKwargs)
 Plot a pybdsim.Data.TH1 instance.
 Parameters
 • xlabel – x axis label
 • ylabel – y axis label
 • title – plot title
 • scalingFactor – multiplier for values
-
-14.11. pybdsim.Plot module
-
-91
-
-pybdsim Documentation, Release 3.2.0
-
 • xScalingFactor – multiplier for x axis coordinates
 • log – whether to automatically plot on a vertical log scale
 return figure instance
 pybdsim.Plot.Histogram1DMultiple(histograms, labels, log=False, xlog=False, xlabel=None,
 ylabel=None, title=None, scalingFactors=None,
 xScalingFactors=None, figsize=(10, 5), legendKwargs={},
 **errorbarKwargs)
@@ -3717,14 +3741,20 @@
 Parameters
 • histogram1 – a pybdsim.Data.TH1 instance
 • histogram2 – a pybdsim.Data.TH1 instance
 • label1 – legend label for histogram1 (str or “” or None)
 • label2 – legend label for histogram2
 • ratio – integer ratio of main plot height to ratio plot height (recommend 1 - 5)
 • ratioYAxisLimit (tuple(float, float)) – ylim upper for ratio subplot y axis
+92
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.3.0
+
 If the labels are “” then the histogram.title string will be used. If None, then no label will be added.
 pybdsim.Plot.Histogram2D(histogram, logNorm=False, xLogScale=False, yLogScale=False, xlabel='',
 ylabel='', zlabel='', title='', aspect='auto', scalingFactor=1.0,
 xScalingFactor=1.0, yScalingFactor=1.0, figsize=(6, 5), vmin=None,
 autovmin=False, vmax=None, colourbar=True, **imshowKwargs)
 Plot a pybdsim.Data.TH2 instance. logNorm - logarithmic colour scale xlogscale - x axis logarithmic scale
 ylogscale - y axis logarithmic scale zlabel - label for color bar scale aspect - “auto”, “equal”, “none” - see
@@ -3733,20 +3763,14 @@
 data vmin - explicitly control the vmin for the colour normalisation vmax - explicitly control the vmax for
 the colour normalisation
 return figure instance
 pybdsim.Plot.Histogram2DErrors(histogram, logNorm=False, xLogScale=False, yLogScale=False,
 xlabel='', ylabel='', zlabel='', title='', aspect='auto', scalingFactor=1.0,
 xScalingFactor=1.0, yScalingFactor=1.0, figsize=(6, 5), vmin=None,
 autovmin=False, vmax=None, **imshowKwargs)
-92
-
-Chapter 14. Module Contents
-
-pybdsim Documentation, Release 3.2.0
-
 Similar to Histogram2D() but plot the errors from the histogram instead of the contents. See pybdsim.Plot.Histogram2D for documentation of arguments.
 pybdsim.Plot.Histogram3D(th3)
 Plot a pybdsim.Data.TH3 instance - TBC
 pybdsim.Plot.LossAndEnergyDeposition(filename, outputfilename=None, tfssurvey=None,
 bdsimsurvey=None, hitslegendloc='upper left',
 elosslegendloc='upper right', perelement=False,
 elossylim=None, phitsylim=None)
@@ -3769,34 +3793,34 @@
 end positions of each element in the sequence.
 pybdsim.Plot.ModelBDSIMYZ(model, ax=None)
 The ModelBDSIMXZ and ModelBDSIMYZ functions add the possibility to plot a survey done in BDSIM.
 The results can be found in the BDSIM output file in the Model tree. The functions can plot the start and
 end positions of each element in the sequence.
 pybdsim.Plot.ModelElegantXZ(model, ax=None, transpose=False)
 Plot a model madx from elegant. In development.
+
+14.11. pybdsim.Plot module
+
+93
+
+pybdsim Documentation, Release 3.3.0
+
 pybdsim.Plot.ModelElegantYZ(model, ax=None, transpose=False)
 Plot a model madx from elegant. In development.
 pybdsim.Plot.PhaseSpace(data, nbins=None, outputfilename=None, extension='.pdf')
 Make two figures for coordinates and correlations.
 Number of bins chosen depending on number of samples.
 ‘outputfilename’ should be without an extension - any extension will be stripped off.
 Plots are saves automatically as pdf, the file extension can be changed with the ‘extension’ kwarg, e.g.
 extension=’.png’.
 pybdsim.Plot.PhaseSpaceFromFile(filename, samplerIndexOrName=0, nbins=None,
 outputfilename=None, extension='.pdf')
 Load a BDSIM output file and plot the phase space of a sampler (default the primaries). Only accepts raw
 BDSIM output.
 Number of bins chosen depending on number of samples.
-
-14.11. pybdsim.Plot module
-
-93
-
-pybdsim Documentation, Release 3.2.0
-
 ‘outputfilename’ should be without an extension - any extension will be stripped off. Plots are saves automatically as pdf, the file extension can be changed with the ‘extension’ kwarg, e.g. extension=’.png’.
 pybdsim.Plot.PhaseSpaceSeparateAxes(filename, samplerIndexOrName=0, outputfilename=None,
 extension='.pdf', nbins=None, energy='total', offsetTime=True,
 includeSecondaries=False, coordsTitle=None,
 correlationTitle=None, scalefactors={}, labels={},
 log1daxes=False, log2daxes=False, includeColorbar=True)
 Plot the coordinates and correlations of both the transverse and longitudinal phase space in separate plots
@@ -3816,33 +3840,33 @@
 includeColorbar adds a colorbar to the correlation plots. The colorbar is normalised for all plot subfigures.
 Default = True.
 pybdsim.Plot.PlotAlpha(bds, outputfilename=None, survey=None, **kwargs)
 pybdsim.Plot.PlotBeta(bds, outputfilename=None, survey=None, **kwargs)
 pybdsim.Plot.PlotDisp(bds, outputfilename=None, survey=None, **kwargs)
 pybdsim.Plot.PlotDispP(bds, outputfilename=None, survey=None, **kwargs)
 pybdsim.Plot.PlotMean(bds, outputfilename=None, survey=None, **kwargs)
+
+94
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.3.0
+
 pybdsim.Plot.PlotNPart(bds, outputfilename=None, survey=None, **kwargs)
 pybdsim.Plot.PlotSigma(bds, outputfilename=None, survey=None, **kwargs)
 pybdsim.Plot.PlotSigmaP(bds, outputfilename=None, survey=None, **kwargs)
 pybdsim.Plot.PrimaryPhaseSpace(filename, outputfilename=None, extension='.pdf')
 Load a BDSIM output file and plot primary phase space. Only accepts raw BDSIM output.
 ‘outputfilename’ should be without an extension - any extension will be stripped off. Plots are saves automatically as pdf, the file extension can be changed with the ‘extension’ kwarg, e.g. extension=’.png’.
 pybdsim.Plot.PrimarySurvival(filename, outputfilename=None, tfssurvey=None, bdsimsurvey=None)
 pybdsim.Plot.PrimaryTrajectoryAndProcess(rootData, eventNumber)
 pybdsim.Plot.ProvideWrappedS(sArray, index)
-
-94
-
-Chapter 14. Module Contents
-
-pybdsim Documentation, Release 3.2.0
-
 pybdsim.Plot.Spectra(spectra, log=False, xlog=False, xlabel=None, ylabel=None, title=None,
 scalingFactors=None, xScalingFactors=None, figsize=(10, 5), legendKwargs={},
-**errorbarKwargs)
+vmin=None, vmax=None, **errorbarKwargs)
 Plot a Spectra object loaded from data that represents a set of histograms.
 returns a list of figure objects.
 pybdsim.Plot.SubplotsWithDrawnMachineLattice(survey, nrows=2, machine_plot_gap=0.01,
 gridspec_kw=None, subplots_kw=None, **fig_kw)
 Create a figure with a single column of axes, sharing the x-axis by default, with the machine drawn from the
 provided survey on the top row axes. nrows gives the number of axes, the first is always the machine lattice.
 by default 2 are drawn, the first for the machine, and the second for any data to be plotted to afterwards.
@@ -3864,32 +3888,32 @@
 options=None, bdsimExecutable=None)
 Runs bdsim with gmadpath as inputfile and outfile as outfile. Runs in batch mode by default, with 10,000
 particles. Any extra options should be provided as a string or iterable of strings of the form “–vis_debug” or
 “–vis_mac=vis.mac”, etc.
 class pybdsim.Run.ExecOptions(*args, **kwargs)
 Bases: dict
 GetExecArgs()
+
+14.12. pybdsim.Run module
+
+95
+
+pybdsim Documentation, Release 3.3.0
+
 GetExecFlags()
 pybdsim.Run.GetOpticsFromGMAD(gmad, keep_optics=False)
 Get the optical functions as a BDSAsciiData instance from this GMAD file. If keep_optics is false then all
 intermediate files are discarded, otherwise the final optics ROOT file is written to ./
 class pybdsim.Run.GmadModifier(rootgmadfilename)
 Bases: object
 CheckExtensions()
 DetermineIncludes(filename)
 ReplaceTokens(tokenDict)
 pybdsim.Run.Rebdsim(rootpath, inpath, outpath, silent=False, rebdsimExecutable=None)
 Run rebdsim with rootpath as analysisConfig file, inpath as bdsim file, and outpath as output analysis file.
-
-14.12. pybdsim.Run module
-
-95
-
-pybdsim Documentation, Release 3.2.0
-
 pybdsim.Run.RebdsimCombine(rootpath, outpath, silent=False, rebdsimHistoExecutable=None)
 Run rebdsimCombine
 pybdsim.Run.RebdsimHistoMerge(rootpath, outpath, silent=False, rebdsimHistoExecutable=None)
 Run rebdsimHistoMerge
 pybdsim.Run.RebdsimOptics(rootpath, outpath, silent=False)
 Run rebdsimOptics
 pybdsim.Run.RebdsimOrbit(rootpath, outpath, index='1', silent=False, rebdsimHistoExecutable=None)
@@ -3911,30 +3935,29 @@
 draw()
 Quick survey drawing for diagnostic reasons.
 findComponentCoords(componentName)
 Returns the XYZ coordinates of a component relative to the centre
 getWorldCentre(type='linear')
 Returns the center in world coordinates of the centre of the visualisation space
 
+96
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.3.0
+
 14.14 pybdsim.Writer module
 Writer
 Write files for a pybdsim.Builder.Machine instance. Each section of the written output (e.g. components, sequence,
 beam etc.) can be written in the main gmad file, written in its own separate file, or called from an external, preexisting file.
 Classes: File - A class that represents each section of the written output - contains booleans and strings. Writer A class that writes the data to disk.
 class pybdsim.Writer.FileSection(willContain='')
 Bases: object
 A class that represents a section of a gmad file. The sections that this class can represent are:
 • Components
-
-96
-
-Chapter 14. Module Contents
-
-pybdsim Documentation, Release 3.2.0
-
 • Sequence
 • Samplers
 • Beam
 • Options
 • Bias
 • Material
 The class contains booleans and strings relating to the location of that sections data. The section can set to
@@ -3955,37 +3978,34 @@
 WriteInMain()
 WriteSeparately()
 class pybdsim.Writer.Writer
 Bases: object
 A class for writing a pybdsim.Builder.Machine instance to file.
 This class allows the user to write individual sections of a BDSIM input file (e.g. components, sequence,
 beam etc.) or write the machine as a whole.
+
+14.14. pybdsim.Writer module
+
+97
+
+pybdsim Documentation, Release 3.3.0
+
 There are 6 attributes in this class which are FileSection instances representing each section of the data. The
 location where these sections will be written/read is stored in these instances. See the FileSection class for
 further details.
 The optional boolean ‘singlefile’ in the WriteMachine function for writing the sections to a single file overrides any sections locations set in their respective FileSection instances.
 This class also has individual functions (e.g. WriteBeam) to write each file section and the main file
 (WriteMain) separately. These section functions must be called BEFORE the WriteMain function is called
 otherwise the main file will have no reference to these sections.
 Examples:
 Writing the Builder.Machine instance myMachine to separate files:
 >>> a = Writer()
 >>> a.WriteMachine(myMachine,'lattice.gmad')
 Lattice written to:
 lattice_components.gmad
-(continues on next page)
-
-14.14. pybdsim.Writer module
-
-97
-
-pybdsim Documentation, Release 3.2.0
-
-(continued from previous page)
-
 lattice_sequence.gmad
 lattice_beam.gmad
 lattice.gmad
 All included in main file:
 lattice.gmad
 Writing the Builder.Machine instance myMachine into a single file:
 >>> a = Writer()
@@ -4020,14 +4040,20 @@
 machine biases (if defined)
 machine materials (if defined)
 suitable main file with all sub files in correct order
 
 These are prefixed with the specified filename / path
 The optional bool singlefile = True will write all the above sections into a single file:
 filename.gmad
+98
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.3.0
+
 kwargs: overwrite : Do not append an integer to the basefilename if already exists, instead overwrite
 existing files.
 WriteMain(machine(machine), filename(string))
 Write the main gmad file: filename.gmad
 The
 functions
 for
@@ -4039,21 +4065,14 @@
 machine
 (components,sequence,beam,options,samplers,bias,material) must be written BEFORE this function is
 called.
 WriteMaterial(machine, filename='')
 Write the machines material to disk: filename.gmad
 WriteObjects(machine, filename='')
 Write the machines objects (e.g. crystals) to disk: filename.gmad
-
-98
-
-Chapter 14. Module Contents
-
-pybdsim Documentation, Release 3.2.0
-
 WriteOptions(machine, filename='')
 Write a machines options to disk: filename.gmad
 Machine can be either a pybdsim.Builder.Machine instance or a pybdsim.Options.Options instance.
 WriteSamplers(machine, filename='')
 Write the machines samplers to disk: filename.gmad
 WriteSequence(machine, filename='')
 Write the machines sequence to disk: filename.gmad
@@ -4074,15 +4093,15 @@
 SetXSecFactors(xsecs)
 Set cross section factors. xsecs should be a space-delimited string of floats, e.g. “1.0 1e13 1234.9”
 
 14.15. pybdsim.XSecBias module
 
 99
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 100
 
 Chapter 14. Module Contents
 
 CHAPTER
 
@@ -4109,15 +4128,15 @@
 Then you can test by importing it and using it. Afterwards, remove it.
 1) twine upload --repository pypi dist/*
 Warning: Once a tag is pushed to pypi, it can never be deleted or replaced. Similarly for testpypi. Consider
 using v1.2.3-rc or v1.2.3-rc1, which will be recognised as a release candidate by pypi.
 
 101
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 102
 
 Chapter 15. Developer Documentation
 
 CHAPTER
 
@@ -4127,15 +4146,15 @@
 
 • genindex
 • modindex
 • search
 
 103
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 104
 
 Chapter 16. Indices and tables
 
 PYTHON MODULE INDEX
 
@@ -4144,29 +4163,29 @@
 pybdsim.Beam, 57
 pybdsim.Builder, 58
 pybdsim.Compare, 67
 pybdsim.Constants, 68
 pybdsim.Convert, 68
 pybdsim.Convert._MadxTfs2Gmad, 71
 pybdsim.Data, 73
-pybdsim.Field, 79
-pybdsim.Field._Field, 79
-pybdsim.Field.FieldPlotter, 81
+pybdsim.Field, 80
+pybdsim.Field._Field, 80
+pybdsim.Field.FieldPlotter, 82
 pybdsim.Gmad, 85
 pybdsim.ModelProcessing, 87
-pybdsim.Options, 87
+pybdsim.Options, 88
 pybdsim.Plot, 90
 pybdsim.Run, 95
 pybdsim.Visualisation, 96
-pybdsim.Writer, 96
+pybdsim.Writer, 97
 pybdsim.XSecBias, 99
 
 105
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 106
 
 Python Module Index
 
 INDEX
 
@@ -4179,15 +4198,15 @@
 AddOctupole()
 (pybdsim.Builder.Machine method),
 AddBias() (pybdsim.Builder.Machine method), 62
 63
 AddBLM() (pybdsim.Builder.Machine method), 62
 AddComment() (pybdsim.Field._Field.Field method), AddOptions() (pybdsim.Builder.Machine method), 63
 AddPlacement() (pybdsim.Builder.Machine method),
-79
+80
 63
 AddCrystal() (pybdsim.Builder.Machine method), 62
 AddQuadrupole()
 (pybdsim.Builder.Machine
 AddCrystalCol()
 (pybdsim.Builder.Machine
 method),
@@ -4264,33 +4283,33 @@
 Aperture() (in module pybdsim.Plot), 90
 module pybdsim.Plot), 90
 AddMachineLatticeFromSurveyToFigureMultiple()ApertureInfo (class in pybdsim.Data), 73
 ApertureModel (class in pybdsim.Builder), 58
 (in module pybdsim.Plot), 90
 Append() (pybdsim.Builder.Machine method), 64
 AddMarker() (pybdsim.Builder.Machine method), 63
-AddMaterial() (pybdsim.Builder.Machine method), append() (pybdsim.Data.Spectra method), 77
+AddMaterial() (pybdsim.Builder.Machine method), append() (pybdsim.Data.Spectra method), 78
 Atom (class in pybdsim.Builder), 58
 63
 AddMultipole() (pybdsim.Builder.Machine method),
 63
 AddMuSpoiler() (pybdsim.Builder.Machine method),
 
 B
 BDSAsciiData (class in pybdsim.Data), 73
 
 107
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 BDSBH4D (class in pybdsim.Data), 74
 Bdsim() (in module pybdsim.Run), 95
 BDSIMAperture() (in module pybdsim.Plot), 90
 BDSIMApertureFromFile() (in module pybdsim.Plot), 90
-BDSIMOptics() (in module pybdsim.Plot), 90
+BDSIMOptics() (in module pybdsim.Plot), 91
 BdsimPrimaries2Mad8()
 (in
 module
 pybdsim.Convert), 68
 BdsimPrimaries2Madx()
 (in
 module
@@ -4303,61 +4322,61 @@
 Beam (class in pybdsim.Beam), 57
 BeamData (class in pybdsim.Data), 74
 BLM (class in pybdsim.Builder), 58
 
 E
 
 ECol (class in pybdsim.Builder), 59
-ElectronColliderOptions() (in module pybdsim.Options), 87
+ElectronColliderOptions() (in module pybdsim.Options), 88
 Element (class in pybdsim.Builder), 59
 ElementBase (class in pybdsim.Builder), 60
 ElementModifier (class in pybdsim.Builder), 60
 elementNames()
 (pybdsim.Gmad.GmadFileComponents method),
 85
 EnergyDeposition() (in module pybdsim.Plot), 91
 EnergyDepositionCoded() (in module pybdsim.Plot), 91
 ErrorsToErrorOnMean() (pybdsim.Data.BDSBH4D
 method), 74
 ErrorsToErrorOnMean() (pybdsim.Data.ROOTHist
-method), 76
+method), 77
 C
 ErrorsToSTD() (pybdsim.Data.BDSBH4D method),
 CallExternalFile()
 (pybdsim.Writer.FileSection
 74
 method), 97
 ErrorsToSTD() (pybdsim.Data.ROOTHist method),
 CavityInfo (class in pybdsim.Data), 74
-76
+77
 CavityModel (class in pybdsim.Builder), 58
 EventInfoData (class in pybdsim.Data), 74
 change()
 (pybdsim.Gmad.GmadFileComponents EventSummaryData (class in pybdsim.Data), 74
 method), 85
 ExecOptions (class in pybdsim.Run), 95
 CheckBiasedProcesses()
 (pybd- ExternalGeometry (class in pybdsim.Builder), 60
 sim.XSecBias.XSecBias method), 99
 CheckExtensions()
 (pybdsim.Run.GmadModifier F
-method), 95
+method), 96
 Field (class in pybdsim.Builder), 60
 CollimatorInfo (class in pybdsim.Data), 74
-Field (class in pybdsim.Field._Field), 79
+Field (class in pybdsim.Field._Field), 80
 CompareMadX() (pybdsim.Gmad.Survey method), 87
 Field1D (class in pybdsim.Field._Field), 80
 ConcatenateMachine()
 (pybd- Field2D (class in pybdsim.Field._Field), 80
 sim.Data.BDSAsciiData method), 73
-Field3D (class in pybdsim.Field._Field), 80
+Field3D (class in pybdsim.Field._Field), 81
 ConvertToPybdsimHistograms()
 (pybd- Field4D (class in pybdsim.Field._Field), 81
 sim.Data.RebdsimFile method), 77
-FileSection (class in pybdsim.Writer), 96
+FileSection (class in pybdsim.Writer), 97
 CreateDipoleDriftRing() (in module pybd- Fill() (pybdsim.Data.Histogram1DSet method), 75
 sim.Builder), 58
 Filter() (pybdsim.Data.BDSAsciiData method), 73
 CreateDipoleFodoRing() (in module pybd- FinalDiff() (pybdsim.Gmad.Survey method), 87
 sim.Builder), 59
 FindClosestElement()
 (pybdsim.Gmad.Survey
@@ -4371,180 +4390,201 @@
 (pybdCreateFodoLine() (in module pybdsim.Builder), 59
 sim.Gmad.GmadFileComponents method),
 Crystal (class in pybdsim.Builder), 59
 85
 CrystalCol (class in pybdsim.Builder), 59
 Flush() (pybdsim.Data.Histogram1DSet method), 75
 
-FourDData (class in pybdsim.Field.FieldPlotter), 81
+FourDData (class in pybdsim.Field.FieldPlotter), 82
 from_element() (pybdsim.Builder.Element class
 Decapole (class in pybdsim.Builder), 59
 method), 60
 DefineConstituentElements()
 (pybd- FromROOTFile() (pybdsim.Data.BeamData class
 sim.Builder.Line method), 61
 method), 74
 Degrader (class in pybdsim.Builder), 59
 FromROOTFile() (pybdsim.Data.EventInfoData class
 DetermineIncludes() (pybdsim.Run.GmadModifier
 method), 74
-method), 95
+method), 96
 FromROOTFile() (pybdsim.Data.ModelData class
 draw() (pybdsim.Visualisation.Helper method), 96
-method), 75
-DrawMachineLattice() (in module pybdsim.Plot), 90 FromROOTFile() (pybdsim.Data.OptionsData class
+method), 76
+DrawMachineLattice() (in module pybdsim.Plot), 91 FromROOTFile() (pybdsim.Data.OptionsData class
 Drift (class in pybdsim.Builder), 59
 method), 76
 Dump (class in pybdsim.Builder), 59
 
 D
 
 108
 
 Index
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
 G
+
+GetPDGInd() (in module pybdsim.Constants), 68
+GetPDGName() (in module pybdsim.Constants), 68
 Gap (class in pybdsim.Builder), 60
-GenerateFullListOfSamplers() (in module pybdsim.ModelProcessing), 87
+(pybdsim.Gmad.GmadFileComponents
+GenerateFullListOfSamplers() (in module pybd- getType()
+method),
+86
+sim.ModelProcessing), 87
+GetType()
+(pybdsim.Gmad.Lattice
+method), 86
 GenerateSamplersFromBDSIMSurvey() (in module
+getWorldCentre()
+(pybdsim.Visualisation.Helper
 pybdsim.Builder), 61
+method), 96
 GetAllNames() (pybdsim.Gmad.Lattice method), 86
+GmadFile
+(class in pybdsim.Gmad), 85
 GetAngle() (pybdsim.Gmad.Lattice method), 86
+GmadFileBeam
+(class in pybdsim.Gmad), 85
 GetAper1() (pybdsim.Gmad.Lattice method), 86
+GmadFileComponents
+(class in pybdsim.Gmad), 85
 GetAper2() (pybdsim.Gmad.Lattice method), 86
+GmadFileOptions
+(class
+in pybdsim.Gmad), 86
 GetAper3() (pybdsim.Gmad.Lattice method), 86
+GmadModifier
+(class
+in
+pybdsim.Run),
+96
 GetAper4() (pybdsim.Gmad.Lattice method), 86
+GmadObject
+(class
+in
+pybdsim.Builder),
+61
 GetApertureData()
 (pybdsim.Data.ModelData
-method), 75
-GetApertureExtent() (in module pybdsim.Data), 74
+method), 76
+GetApertureExtent() (in module pybdsim.Data), 74 H
 GetApertureExtents()
-(pybdsim.Gmad.Lattice
+(pybdsim.Gmad.Lattice Header (class in pybdsim.Data), 75
+Helper (class in pybdsim.Visualisation), 96
 method), 86
 GetApertureType()
-(pybdsim.Gmad.Lattice
+(pybdsim.Gmad.Lattice Histogram1D() (in module pybdsim.Plot), 92
+Histogram1DMultiple() (in module pybdsim.Plot),
 method), 86
+92
 GetAxisAlignedBoundingBoxOfCollimator() (in
+Histogram1DRatio()
+(in module pybdsim.Plot), 92
 module pybdsim.ModelProcessing), 87
+Histogram1DSet
+(class
+in pybdsim.Data), 75
 GetColumn() (pybdsim.Data.BDSAsciiData method),
+Histogram2D()
+(in
+module
+pybdsim.Plot), 93
 73
+Histogram2DErrors()
+(in
+module
+pybdsim.Plot), 93
 GetColumn() (pybdsim.Gmad.Lattice method), 86
+Histogram3D()
+(in
+module
+pybdsim.Plot),
+93
 GetElement() (pybdsim.Gmad.Lattice method), 86
+HKicker
+(class
+in
+pybdsim.Builder),
+61
 GetExecArgs() (pybdsim.Run.ExecOptions method),
 95
-GetExecFlags() (pybdsim.Run.ExecOptions method),
+GetExecFlags() (pybdsim.Run.ExecOptions method), I
 95
+IndexFromNearestS() (pybdsim.Data.BDSAsciiData
+GetHistoryPDGTuple() (in module pybdsim.Data),
+method), 73
+74
+IndexFromNearestS()
+(pybdsim.Gmad.Lattice
 GetIndexOfElementNamed()
-(pybdsim.Gmad.Lattice method), 86
+(pybdmethod), 86
+sim.Gmad.Lattice method), 86
+InsertAndReplace()
+(pybdsim.Builder.Machine
 GetInfo() (pybdsim.Run.Study method), 96
-GetIntegratedAngle() (pybdsim.Builder.Machine
 method), 64
-GetIntegratedLength() (pybdsim.Builder.Machine
+GetIntegratedAngle() (pybdsim.Builder.Machine IntegateAlong1Dimension() (pybdsim.Data.TH3
 method), 64
+method), 78
+GetIntegratedLength() (pybdsim.Builder.Machine IntegateAlong2Dimensions() (pybdsim.Data.TH3
+method), 64
+method), 79
 GetItemTuple()
-(pybdsim.Data.BDSAsciiData
+(pybdsim.Data.BDSAsciiData IntegrateAlongX() (pybdsim.Data.TH2 method), 78
 method), 73
+IntegrateAlongY() (pybdsim.Data.TH2 method), 78
 GetKs() (pybdsim.Gmad.Lattice method), 86
 GetLength() (pybdsim.Gmad.Lattice method), 86
-GetMaterialIDOfCollimator() (in module pybdsim.ModelProcessing), 87
-GetModel() (pybdsim.Data.RebdsimFile method), 77
+J
+GetMaterialIDOfCollimator() (in module pybd- JCol (class in pybdsim.Builder), 61
+sim.ModelProcessing), 87
+GetModel() (pybdsim.Data.RebdsimFile method), 77 K
 GetModelForPlotting() (in module pybdsim.Data),
-74
+keysextra() (pybdsim.Builder.ElementBase method),
+75
+60
 GetModelTree()
 (pybdsim.Data.RebdsimFile
+keysextra() (pybdsim.Builder.GmadObject method),
 method), 77
+61
 GetName() (pybdsim.Gmad.Lattice method), 86
+Kicker (class in pybdsim.Builder), 61
 GetNamesOfType()
 (pybdsim.Builder.Machine
 method), 64
-GetNEventsInBDSIMFile() (in module pybdsim.Data), 74
-GetOpticsFromGMAD() (in module pybdsim.Run), 95
+L
+GetNEventsInBDSIMFile() (in module pybdLaser (class in pybdsim.Builder), 61
+sim.Data), 75
+GetOpticsFromGMAD() (in module pybdsim.Run), 96 Lattice (class in pybdsim.Gmad), 86
 getParameter()
-(pybdsim.Gmad.GmadFileComponents method),
-85
-GetPDGInd() (in module pybdsim.Constants), 68
-GetPDGName() (in module pybdsim.Constants), 68
+(pybd- Line (class in pybdsim.Builder), 61
+sim.Gmad.GmadFileComponents method), ListOfDirectories() (pybdsim.Data.RebdsimFile
+method), 77
+86
 Index
 
-getType()
-(pybdsim.Gmad.GmadFileComponents
-method), 85
-GetType() (pybdsim.Gmad.Lattice method), 86
-getWorldCentre()
-(pybdsim.Visualisation.Helper
-method), 96
-GmadFile (class in pybdsim.Gmad), 85
-GmadFileBeam (class in pybdsim.Gmad), 85
-GmadFileComponents (class in pybdsim.Gmad), 85
-GmadFileOptions (class in pybdsim.Gmad), 85
-GmadModifier (class in pybdsim.Run), 95
-GmadObject (class in pybdsim.Builder), 61
-
-H
-Header (class in pybdsim.Data), 74
-Helper (class in pybdsim.Visualisation), 96
-Histogram1D() (in module pybdsim.Plot), 91
-Histogram1DMultiple() (in module pybdsim.Plot),
-92
-Histogram1DRatio() (in module pybdsim.Plot), 92
-Histogram1DSet (class in pybdsim.Data), 74
-Histogram2D() (in module pybdsim.Plot), 92
-Histogram2DErrors() (in module pybdsim.Plot), 92
-Histogram3D() (in module pybdsim.Plot), 93
-HKicker (class in pybdsim.Builder), 61
-
-I
-IndexFromNearestS() (pybdsim.Data.BDSAsciiData
-method), 73
-IndexFromNearestS()
-(pybdsim.Gmad.Lattice
-method), 86
-InsertAndReplace()
-(pybdsim.Builder.Machine
-method), 64
-IntegateAlong1Dimension() (pybdsim.Data.TH3
-method), 78
-IntegateAlong2Dimensions() (pybdsim.Data.TH3
-method), 78
-IntegrateAlongX() (pybdsim.Data.TH2 method), 78
-IntegrateAlongY() (pybdsim.Data.TH2 method), 78
-
-J
-JCol (class in pybdsim.Builder), 61
+109
 
-K
-keysextra() (pybdsim.Builder.ElementBase method),
-60
-keysextra() (pybdsim.Builder.GmadObject method),
-61
-Kicker (class in pybdsim.Builder), 61
+pybdsim Documentation, Release 3.3.0
 
-L
-Laser (class in pybdsim.Builder), 61
-Lattice (class in pybdsim.Gmad), 85
-Line (class in pybdsim.Builder), 61
-ListOfDirectories() (pybdsim.Data.RebdsimFile
-method), 77
 ListOfLeavesInTree() (pybdsim.Data.RebdsimFile
 method), 77
-109
-
-pybdsim Documentation, Release 3.2.0
-
 ListOfTrees() (pybdsim.Data.RebdsimFile method),
 77
 Load() (in module pybdsim.Data), 75
 Load() (in module pybdsim.Field._Field), 81
-Load() (pybdsim.Gmad.Lattice method), 86
+Load() (pybdsim.Gmad.Lattice method), 87
 Load() (pybdsim.Gmad.Survey method), 87
-LoadPickledObject() (in module pybdsim.Data), 75
-LoadROOTLibraries() (in module pybdsim.Data), 75
-LoadSDDSColumnsToDict() (in module pybdsim.Data), 75
+LoadPickledObject() (in module pybdsim.Data), 76
+LoadROOTLibraries() (in module pybdsim.Data), 76
+LoadSDDSColumnsToDict() (in module pybdsim.Data), 76
 LossAndEnergyDeposition() (in module pybdsim.Plot), 93
 LossMap() (in module pybdsim.Plot), 93
 
 M
 Machine (class in pybdsim.Builder), 61
 MadxTfs2Gmad() (in module pybdsim.Convert), 69
 MadxTfs2Gmad()
@@ -4564,139 +4604,139 @@
 MatchValue()
 (pybdsim.Data.BDSAsciiData
 method), 73
 Material (class in pybdsim.Builder), 65
 MirrorDipoleQuadrant1() (in module pybdsim.Field._Field), 81
 ModelBDSIMXZ() (in module pybdsim.Plot), 93
 ModelBDSIMYZ() (in module pybdsim.Plot), 93
-ModelData (class in pybdsim.Data), 75
+ModelData (class in pybdsim.Data), 76
 ModelElegantXZ() (in module pybdsim.Plot), 93
 ModelElegantYZ() (in module pybdsim.Plot), 93
 module
 pybdsim, 57
 pybdsim.Beam, 57
 pybdsim.Builder, 58
 pybdsim.Compare, 67
 pybdsim.Constants, 68
 pybdsim.Convert, 68
 pybdsim.Convert._MadxTfs2Gmad, 71
 pybdsim.Data, 73
-pybdsim.Field, 79
-pybdsim.Field._Field, 79
-pybdsim.Field.FieldPlotter, 81
+pybdsim.Field, 80
+pybdsim.Field._Field, 80
+pybdsim.Field.FieldPlotter, 82
 pybdsim.Gmad, 85
 pybdsim.ModelProcessing, 87
-pybdsim.Options, 87
+pybdsim.Options, 88
 pybdsim.Plot, 90
 pybdsim.Run, 95
 pybdsim.Visualisation, 96
-pybdsim.Writer, 96
-pybdsim.XSecBias, 99
 110
 
+pybdsim.Writer, 97
+pybdsim.XSecBias, 99
 Multipole (class in pybdsim.Builder), 65
 MuSpoiler (class in pybdsim.Builder), 65
 
 N
 NameFromNearestS() (pybdsim.Data.BDSAsciiData
 method), 73
 NewColour (class in pybdsim.Builder), 65
 next() (pybdsim.Builder.Machine method), 65
 next() (pybdsim.Data.TrajectoryData method), 79
-next() (pybdsim.Gmad.Lattice method), 86
+next() (pybdsim.Gmad.Lattice method), 87
 
 O
 Octupole (class in pybdsim.Builder), 65
 OneDData (class in pybdsim.Field.FieldPlotter), 82
-Options (class in pybdsim.Options), 87
+Options (class in pybdsim.Options), 88
 OptionsData (class in pybdsim.Data), 76
 
 P
 PadHistogram1D() (in module pybdsim.Data), 76
 parseElement()
 (pybdsim.Gmad.GmadFileComponents method),
-85
-ParseLattice() (pybdsim.Gmad.Lattice method), 86
+86
+ParseLattice() (pybdsim.Gmad.Lattice method), 87
 ParseSpectraName() (in module pybdsim.Data), 76
-PhaseSpace() (in module pybdsim.Plot), 93
+PhaseSpace() (in module pybdsim.Plot), 94
 PhaseSpaceData (class in pybdsim.Data), 76
-PhaseSpaceFromFile() (in module pybdsim.Plot), 93
+PhaseSpaceFromFile() (in module pybdsim.Plot), 94
 PhaseSpaceSeparateAxes() (in module pybdsim.Plot), 94
 PickleObject() (in module pybdsim.Data), 76
 Placement (class in pybdsim.Builder), 65
 Plot() (pybdsim.Gmad.Survey method), 87
 Plot1DFxFyFz()
 (in
 module
 pybdsim.Field.FieldPlotter), 82
 Plot2D() (in module pybdsim.Field.FieldPlotter), 82
 Plot2DXY() (in module pybdsim.Field.FieldPlotter),
 82
 Plot2DXYBx()
 (in
 module
-pybdsim.Field.FieldPlotter), 82
+pybdsim.Field.FieldPlotter), 83
 Plot2DXYBy()
 (in
 module
 pybdsim.Field.FieldPlotter), 83
 Plot2DXYBz()
 (in
 module
 pybdsim.Field.FieldPlotter), 83
 Plot2DXYComponent()
 (in
 module
 pybdsim.Field.FieldPlotter), 83
-Plot2DXYConnectionOrder() (in module pybdsim.Field.FieldPlotter), 83
+Plot2DXYConnectionOrder() (in module pybdsim.Field.FieldPlotter), 84
 Plot2DXYFxFyFz()
 (in
 module
-pybdsim.Field.FieldPlotter), 83
+pybdsim.Field.FieldPlotter), 84
 Plot2DXYMagnitude()
 (in
 module
 pybdsim.Field.FieldPlotter), 84
 Plot2DXYStream()
 (in
 module
 pybdsim.Field.FieldPlotter), 84
 Plot2DXZStream()
 (in
 module
 pybdsim.Field.FieldPlotter), 84
-Plot3DXY() (in module pybdsim.Field.FieldPlotter),
-84
 
 Index
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
+Plot3DXY() (in module pybdsim.Field.FieldPlotter),
+85
 Plot3DXZ() (in module pybdsim.Field.FieldPlotter),
-84
+85
 PlotAlpha() (in module pybdsim.Plot), 94
 PlotBeta() (in module pybdsim.Plot), 94
 PlotDisp() (in module pybdsim.Plot), 94
 PlotDispP() (in module pybdsim.Plot), 94
 PlotMean() (in module pybdsim.Plot), 94
 PlotNPart() (in module pybdsim.Plot), 94
-PlotSigma() (in module pybdsim.Plot), 94
-PlotSigmaP() (in module pybdsim.Plot), 94
+PlotSigma() (in module pybdsim.Plot), 95
+PlotSigmaP() (in module pybdsim.Plot), 95
 PrepareApertureModel() (in module pybdsim.Builder), 65
 PrepareAxisAngleRotations()
 (pybdsim.Data.ModelData method), 76
-PrimaryPhaseSpace() (in module pybdsim.Plot), 94
-PrimarySurvival() (in module pybdsim.Plot), 94
-PrimaryTrajectoryAndProcess() (in module pybdsim.Plot), 94
-Print() (pybdsim.Gmad.Lattice method), 86
+PrimaryPhaseSpace() (in module pybdsim.Plot), 95
+PrimarySurvival() (in module pybdsim.Plot), 95
+PrimaryTrajectoryAndProcess() (in module pybdsim.Plot), 95
+Print() (pybdsim.Gmad.Lattice method), 87
 PrintZeroLength()
 (pybdsim.Gmad.Lattice
-method), 86
+method), 87
 ProtonColliderOptions() (in module pybdsim.Options), 90
-ProvideWrappedS() (in module pybdsim.Plot), 94
+ProvideWrappedS() (in module pybdsim.Plot), 95
 pybdsim
 module, 57
 pybdsim.Beam
 module, 57
 pybdsim.Builder
 module, 58
 pybdsim.Compare
@@ -4706,118 +4746,120 @@
 pybdsim.Convert
 module, 68
 pybdsim.Convert._MadxTfs2Gmad
 module, 71
 pybdsim.Data
 module, 73
 pybdsim.Field
-module, 79
+module, 80
 pybdsim.Field._Field
-module, 79
+module, 80
 pybdsim.Field.FieldPlotter
-module, 81
+module, 82
 pybdsim.Gmad
 module, 85
 pybdsim.ModelProcessing
 module, 87
 pybdsim.Options
-module, 87
+module, 88
 pybdsim.Plot
 module, 90
 pybdsim.Run
 module, 95
-pybdsim.Visualisation
-module, 96
 
 Index
 
-pybdsim.Writer
+pybdsim.Visualisation
 module, 96
+pybdsim.Writer
+module, 97
 pybdsim.XSecBias
 module, 99
 
 Q
 Quadrupole (class in pybdsim.Builder), 65
 Query (class in pybdsim.Builder), 65
 
 R
 RBend (class in pybdsim.Builder), 66
 RCol (class in pybdsim.Builder), 66
-Rebdsim() (in module pybdsim.Run), 95
-RebdsimCombine() (in module pybdsim.Run), 95
-RebdsimFile (class in pybdsim.Data), 76
+Rebdsim() (in module pybdsim.Run), 96
+RebdsimCombine() (in module pybdsim.Run), 96
+RebdsimFile (class in pybdsim.Data), 77
 RebdsimHistoMerge() (in module pybdsim.Run), 96
 RebdsimOptics() (in module pybdsim.Run), 96
 RebdsimOrbit() (in module pybdsim.Run), 96
 Rebin() (pybdsim.Data.TH1 method), 78
 Rebin() (pybdsim.Data.TH2 method), 78
 RegenerateLenInt()
 (pybdsim.Builder.Machine
 method), 64
 Region (class in pybdsim.Builder), 66
 ReplaceElementCategory()
 (pybdsim.Builder.Machine method), 64
 ReplaceTokens()
 (pybdsim.Run.GmadModifier
-method), 95
+method), 96
 ReplaceWithElement() (pybdsim.Builder.Machine
 method), 64
 ReplaceZeroWithMinimum() (in module pybdsim.Data), 77
 Result() (pybdsim.Data.Histogram1DSet method), 75
 ResultMean()
 (pybdsim.Data.Histogram1DSet
 method), 75
 ReturnBeamString() (pybdsim.Beam.Beam method),
 57
 ReturnOptionsString() (pybdsim.Options.Options
-method), 87
+method), 88
 RFCavity (class in pybdsim.Builder), 66
 Rmat (class in pybdsim.Builder), 66
-ROOTHist (class in pybdsim.Data), 76
+ROOTHist (class in pybdsim.Data), 77
 Run() (pybdsim.Run.Study method), 96
 RunExecOptions() (pybdsim.Run.Study method), 96
 
 S
 Sampler (class in pybdsim.Builder), 66
-SamplerData (class in pybdsim.Data), 77
+SamplerData (class in pybdsim.Data), 78
 SamplerPlacement (class in pybdsim.Builder), 66
 SBend (class in pybdsim.Builder), 66
 Scorer (class in pybdsim.Builder), 66
 ScorerMesh (class in pybdsim.Builder), 66
 SDDSBuildParameterDicts() (in module pybdsim.Data), 77
 SetBeamlineS() (pybdsim.Options.Options method),
 88
-SetBeamPipeRadius()
-(pybdsim.Options.Options
-method), 88
 
 111
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
-SetBeamPipeThickness()
-(pybdsim.Options.Options method), 88
+SetBeamPipeRadius()
+(pybdsim.Options.Options
+sim.Options.Options method), 89
+method), 88
+SetMaximumEpsilonStep()
+(pybdSetBeamPipeThickness()
+(pybdsim.Options.Options method), 89
 sim.Options.Options method), 88
 SetMaximumStepLength()
 (pybdSetBLMLength() (pybdsim.Options.Options method),
-sim.Options.Options method), 88
+sim.Options.Options method), 89
 88
 SetMaximumTrackingTime()
 (pybdSetBLMRadius() (pybdsim.Options.Options method),
-sim.Options.Options method), 88
+sim.Options.Options method), 89
 88
 SetMinimumEpsilonStep()
 (pybdSetBuildTunnel()
 (pybdsim.Options.Options
-sim.Options.Options method), 88
+sim.Options.Options method), 89
 method), 88
 SetName() (pybdsim.XSecBias.XSecBias method), 99
 SetBuildTunnelFloor() (pybdsim.Options.Options SetNGenerate() (pybdsim.Options.Options method),
 method), 88
-88
+89
 SetCherenkovOn()
 (pybdsim.Options.Options SetNLinesIgnore()
 (pybdsim.Options.Options
 method), 88
 method), 89
 SetChordStepMinimum() (pybdsim.Options.Options SetNPerFile() (pybdsim.Options.Options method),
 method), 88
@@ -4892,74 +4934,72 @@
 (pybd- SetSoilMaterial()
 (pybdsim.Options.Options
 sim.Options.Options method), 88
 method), 89
 SetIncludeIronMagField()
 (pybd- SetSoilThickness()
 (pybdsim.Options.Options
-sim.Options.Options method), 88
+sim.Options.Options method), 89
 method), 89
 SetIntegratorSet()
 (pybdsim.Options.Options SetSRLowX() (pybdsim.Options.Options method), 89
-method), 88
+method), 89
 SetSRMultiplicity()
 (pybdsim.Options.Options
 SetLengthSafety()
 (pybdsim.Options.Options
 method), 89
-method), 88
+method), 89
 SetStopSecondaries() (pybdsim.Options.Options
 SetLPBFraction()
 (pybdsim.Options.Options
 method), 89
-method), 88
+method), 89
 SetStoreTrajectory() (pybdsim.Options.Options
 SetMagnetGeometryType()
 (pybdmethod), 89
-sim.Options.Options method), 88
-SetStoreTrajectoryParticle()
-(pybdSetMaximumEpsilonStep()
-(pybdsim.Options.Options method), 89
 
 112
 
 Index
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
+SetStoreTrajectoryParticle()
+(pybdsim.Options.Options method), 89
 SetSynchRadiationOn() (pybdsim.Options.Options
 method), 89
 SetT0() (pybdsim.Beam.Beam method), 58
 SetThresholdCutCharged()
 (pybdsim.Options.Options method), 89
 SetThresholdCutPhotons()
-(pybdsim.Options.Options method), 89
+(pybdsim.Options.Options method), 90
 SetTrackSRPhotons()
 (pybdsim.Options.Options
-method), 89
+method), 90
 SetTrajectoryCutGTZ() (pybdsim.Options.Options
-method), 89
+method), 90
 SetTrajectoryCutLTR() (pybdsim.Options.Options
-method), 89
+method), 90
 SetTunnelFloorOffset()
-(pybdsim.Options.Options method), 89
+(pybdsim.Options.Options method), 90
 SetTunnelMaterial()
 (pybdsim.Options.Options
-method), 89
+method), 90
 SetTunnelOffsetX()
 (pybdsim.Options.Options
-method), 89
+method), 90
 SetTunnelOffsetY()
 (pybdsim.Options.Options
-method), 89
+method), 90
 SetTunnelRadius()
 (pybdsim.Options.Options
-method), 89
+method), 90
 SetTunnelThickness() (pybdsim.Options.Options
-method), 89
+method), 90
 SetVacuumMaterial()
 (pybdsim.Options.Options
 method), 90
 SetVacuumPressure()
 (pybdsim.Options.Options
 method), 90
 SetWritePrimaries()
@@ -4972,49 +5012,49 @@
 method), 99
 SetY0() (pybdsim.Beam.Beam method), 58
 SetYP0() (pybdsim.Beam.Beam method), 58
 SetZ0() (pybdsim.Beam.Beam method), 58
 SetZP0() (pybdsim.Beam.Beam method), 58
 Sextupole (class in pybdsim.Builder), 66
 Shield (class in pybdsim.Builder), 66
-Slice2DXY() (pybdsim.Data.TH3 method), 78
-Slice2DXZ() (pybdsim.Data.TH3 method), 78
+Slice2DXY() (pybdsim.Data.TH3 method), 79
+Slice2DXZ() (pybdsim.Data.TH3 method), 79
 Slice2DZY() (pybdsim.Data.TH3 method), 79
 Solenoid (class in pybdsim.Builder), 66
 SortByBin()
 (pybdsim.Data.Histogram1DSet
 method), 75
-SortUnorderedFieldMap2D() (in module pybdsim.Field._Field), 81
-Spectra (class in pybdsim.Data), 77
-Spectra() (in module pybdsim.Plot), 94
+SortUnorderedFieldMap2D() (in module pybdsim.Field._Field), 82
+Spectra (class in pybdsim.Data), 78
+Spectra() (in module pybdsim.Plot), 95
 split() (pybdsim.Builder.Element method), 60
 split() (pybdsim.Builder.HKicker method), 61
 split() (pybdsim.Builder.Kicker method), 61
 split() (pybdsim.Builder.Multipole method), 65
 split() (pybdsim.Builder.TKicker method), 67
-split() (pybdsim.Builder.VKicker method), 67
-Step() (pybdsim.Gmad.Survey method), 87
 
 Index
 
+split() (pybdsim.Builder.VKicker method), 67
+Step() (pybdsim.Gmad.Survey method), 87
 Study (class in pybdsim.Run), 96
 SubplotsWithDrawnMachineLattice() (in module
 pybdsim.Plot), 95
 SuggestFodoK() (in module pybdsim.Builder), 66
-Survey (class in pybdsim.Gmad), 86
+Survey (class in pybdsim.Gmad), 87
 SwapAxes() (pybdsim.Data.TH2 method), 78
 SynchrotronRadiationRescale()
 (pybdsim.Builder.Machine method), 64
 
 T
-TH1 (class in pybdsim.Data), 77
+TH1 (class in pybdsim.Data), 78
 TH2 (class in pybdsim.Data), 78
 TH3 (class in pybdsim.Data), 78
 ThinMultipole (class in pybdsim.Builder), 67
-ThreeDData (class in pybdsim.Field.FieldPlotter), 84
+ThreeDData (class in pybdsim.Field.FieldPlotter), 85
 TKicker (class in pybdsim.Builder), 67
 ToDF() (pybdsim.Data.BDSAsciiData method), 74
 Trajectory3D() (in module pybdsim.Plot), 95
 TrajectoryData (class in pybdsim.Data), 79
 Transform3D (class in pybdsim.Builder), 67
 TransportVsBDSIM() (in module pybdsim.Compare),
 68
@@ -5038,36 +5078,37 @@
 V
 VKicker (class in pybdsim.Builder), 67
 
 W
 WireScanner (class in pybdsim.Builder), 67
 WrapLatticeAboutItem() (in module pybdsim.ModelProcessing), 87
 Write() (pybdsim.Builder.Machine method), 65
-Write() (pybdsim.Field._Field.Field method), 79
+Write() (pybdsim.Field._Field.Field method), 80
 write()
 (pybdsim.Gmad.GmadFileComponents
-method), 85
+method), 86
 WriteBeam() (pybdsim.Writer.Writer method), 98
 WriteBias() (pybdsim.Writer.Writer method), 98
 WriteComponents() (pybdsim.Writer.Writer method),
 98
 WriteFLUKA2DFormat1()
 (pybdsim.Field._Field.Field method), 80
-WriteInMain() (pybdsim.Writer.FileSection method),
-97
-WriteMachine() (pybdsim.Writer.Writer method), 98
+
 113
 
-pybdsim Documentation, Release 3.2.0
+pybdsim Documentation, Release 3.3.0
 
-WriteMain() (pybdsim.Writer.Writer method), 98
+WriteInMain() (pybdsim.Writer.FileSection method),
+97
+WriteMachine() (pybdsim.Writer.Writer method), 98
+WriteMain() (pybdsim.Writer.Writer method), 99
 WriteMaterial() (pybdsim.Writer.Writer method),
-98
-WriteObjects() (pybdsim.Writer.Writer method), 98
-WriteOptions() (pybdsim.Writer.Writer method), 98
+99
+WriteObjects() (pybdsim.Writer.Writer method), 99
+WriteOptions() (pybdsim.Writer.Writer method), 99
 Writer (class in pybdsim.Writer), 97
 WriteROOTHistogramsToDirectory() (in module
 pybdsim.Data), 79
 WriteSamplers() (pybdsim.Writer.Writer method),
 99
 WriteSeparately()
 (pybdsim.Writer.FileSection
```

### Comparing `pybdsim-3.2.0/docs/source/builder.rst` & `pybdsim-3.3.0/docs/source/builder.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/docs/source/classes.rst` & `pybdsim-3.3.0/docs/source/classes.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/docs/source/compare.rst` & `pybdsim-3.3.0/docs/source/compare.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/docs/source/conf.py` & `pybdsim-3.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/docs/source/convert.rst` & `pybdsim-3.3.0/docs/source/convert.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/docs/source/data.rst` & `pybdsim-3.3.0/docs/source/data.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/docs/source/data_uproot.rst` & `pybdsim-3.3.0/docs/source/data_uproot.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/docs/source/developer.rst` & `pybdsim-3.3.0/docs/source/developer.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/docs/source/fieldmaps.rst` & `pybdsim-3.3.0/docs/source/fieldmaps.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/docs/source/figures/rebdsimFileHistograms.png` & `pybdsim-3.3.0/docs/source/figures/rebdsimFileHistograms.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/docs/source/figures/rebdsimFileHistogramsWrapped.png` & `pybdsim-3.3.0/docs/source/figures/rebdsimFileHistogramsWrapped.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/docs/source/figures/rebdsimFileMembers.png` & `pybdsim-3.3.0/docs/source/figures/rebdsimFileMembers.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/docs/source/figures/simpleHistogramPlot.png` & `pybdsim-3.3.0/docs/source/figures/simpleHistogramPlot.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/docs/source/installation.rst` & `pybdsim-3.3.0/docs/source/installation.rst`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 
 There are the following features that result in more dependencies being installed:
 
 * `uproot` - includes uproot data loading
 * `boost_histogram` - includes boost-histogram package for 4d histograms
 * `cpymad` - allows usage of cpymad for converting models
 * `pysad` - allows usage of pysad for converting models
+* `pymad8` - allows usage of pymad8 for converting models
+* `all` - all of the above at once
 
 These can be installed as: ::
 
   pip install pybdsim[uproot]
 
 or: ::
 
-  pip install pybdsim[uproot,boost_histogram,cpymad,pysad]
+  pip install pybdsim[uproot,boost_histogram,cpymad,pysad,pymad8]
 
 
 Requirements
 ------------
 
 ROOT and its python interface are required to load BDSIM output and also histogram files
 from rebdsim (the analysis tool). This cannot be found through pip but must be separately
@@ -37,15 +39,14 @@
 Generally, the requirements for pybdsim are
 
 * matplotlib >= 3.0
 * numpy >= 1.14
 * scipy
 * fortranformat
 * pymadx
-* pymad8
 * pytransport
 
 These are all available through pip and will be automatically installed.
 
 Optional:
  * ROOT Python interface
```

### Comparing `pybdsim-3.2.0/docs/source/licence.rst` & `pybdsim-3.3.0/docs/source/licence.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/docs/source/moduledocs.rst` & `pybdsim-3.3.0/docs/source/moduledocs.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/docs/source/plotting.rst` & `pybdsim-3.3.0/docs/source/plotting.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/docs/source/support.rst` & `pybdsim-3.3.0/docs/source/support.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/docs/source/version_history.rst` & `pybdsim-3.3.0/docs/source/version_history.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 ===============
 Version History
 ===============
 
+V3.3.0 - 2023 / 05 / 08
+=======================
+
+* Fix installation where there was a missing dependency of pandas with pymad8. pymad8 is
+  now no longer a formal dependency but all the conversion and comparison code still exists.
+* Fix setup.cfg having pymadx in the name although it makes no difference.
+* Add new :code:`pybdsim.Data.GetHistoryPDGTuple()` function to aid trajectory analysis.
+
 V3.2.0 - 2023 / 04 / 26
 =======================
 
 * Remove the function :code:`pybdsim.Plot.AddMachineLatticeToFigure()`. This was just a forward to
   :code:`pymadx.Plot.AddMachineLatticeToFigure()` and this should be used explicitly for
   machine diagram plotting for TFS files. Otherwise, :code:`pybdsim.Plot.AddMachineLatticeFromSurveyToFigure`
   should be used.
```

### Comparing `pybdsim-3.2.0/examples/1_builder/1_testmachine.png` & `pybdsim-3.3.0/examples/1_builder/1_testmachine.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/examples/2_convert/1_madxtfs2gmad.png` & `pybdsim-3.3.0/examples/2_convert/1_madxtfs2gmad.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/examples/2_convert/2_convert.rst` & `pybdsim-3.3.0/examples/2_convert/2_convert.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/examples/2_convert/2_transport2gmad.png` & `pybdsim-3.3.0/examples/2_convert/2_transport2gmad.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/examples/2_convert/transport_example.dat` & `pybdsim-3.3.0/examples/2_convert/transport_example.dat`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/examples/2_convert/transport_example.pdf` & `pybdsim-3.3.0/examples/2_convert/transport_example.pdf`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/examples/2_convert/twiss35tevb1_short.pdf` & `pybdsim-3.3.0/examples/2_convert/twiss35tevb1_short.pdf`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/examples/2_convert/twiss35tevb1_short.tar.gz` & `pybdsim-3.3.0/examples/2_convert/twiss35tevb1_short.tar.gz`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/examples/3_optics/optics_validation.py` & `pybdsim-3.3.0/examples/3_optics/optics_validation.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/examples/4_uproot/4_uproot.rst` & `pybdsim-3.3.0/examples/4_uproot/4_uproot.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/pyproject.toml` & `pybdsim-3.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -28,23 +28,24 @@
 dependencies = [
   "matplotlib>=3.0",
   "numpy>=1.14",
   "importlib-metadata",
   "scipy",
   "fortranformat",
   "pymadx",
-  "pymad8",
   "pytransport"
 ]
 
 [project.optional-dependencies]
 uproot = ["awkward", "uproot", "pandas", "pint"]
 boost_histogram = ["boost-histogram"]
 cpymad = ["cpymad", "mergedeep"]
 pysad = ["pysad"]
+pymad8 = ["pymad8"]
+all = ["awkward", "uproot", "pandas", "pint", "boost-histogram", "cpymad", "mergedeep", "pysad", "pymad8"]
 dev = ["pytest", "sphinx", "sphinx-rtd-theme"]
 
 [project.urls]
 homepage = "http://www.pp.rhul.ac.uk/bdsim/pybdsim"
 documentation = "http://www.pp.rhul.ac.uk/bdsim/pybdsim"
 repository = "https://bitbucket.org/jairhul/pybdsim"
```

### Comparing `pybdsim-3.2.0/src/pybdsim/Beam.py` & `pybdsim-3.3.0/src/pybdsim/Beam.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Builder.py` & `pybdsim-3.3.0/src/pybdsim/Builder.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Compare/_BdsimBdsimComparison.py` & `pybdsim-3.3.0/src/pybdsim/Compare/_BdsimBdsimComparison.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Compare/_ElegantBdsimComparison.py` & `pybdsim-3.3.0/src/pybdsim/Compare/_ElegantBdsimComparison.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Compare/_Mad8BdsimComparison.py` & `pybdsim-3.3.0/src/pybdsim/Compare/_Mad8BdsimComparison.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Compare/_Mad8BdsimComparisonOld.py` & `pybdsim-3.3.0/src/pybdsim/Compare/_Mad8BdsimComparisonOld.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Compare/_MadxBdsimComparison.py` & `pybdsim-3.3.0/src/pybdsim/Compare/_MadxBdsimComparison.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Compare/_MultipleCodeComparison.py` & `pybdsim-3.3.0/src/pybdsim/Compare/_MultipleCodeComparison.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Compare/_SadComparison.py` & `pybdsim-3.3.0/src/pybdsim/Compare/_SadComparison.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Compare/_TransportBdsimComparison.py` & `pybdsim-3.3.0/src/pybdsim/Compare/_TransportBdsimComparison.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 """
 
 import os.path as _path
 import matplotlib.pyplot as _plt
 import datetime as _datetime
 from matplotlib.backends.backend_pdf import PdfPages as _PdfPages
 
-import pybdsim.Data
-import pybdsim.Plot
-import pybdsim._General as _Gen
+import pybdsim.Data as _Data
+import pybdsim.Plot as _Plot
 
+import pymadx as _pymadx
 import pytransport as _pyt
 
 # Predefined lists of tuples for making the standard plots,
 # format = (optical_var_name, optical_var_error_name, legend_name)
 
 _BETA = [("Beta_x", "Sigma_Beta_x", r'$\beta_{x}$'),
          ("Beta_y", "Sigma_Beta_y", r'$\beta_{y}$')]
@@ -45,24 +45,24 @@
    or a BDSAsciiData instance, and in either case, generate a
    name if None is provided, and return that as well."""
    if isinstance(bdsim_in, str):
        if not _path.isfile(bdsim_in):
            raise IOError("file \"{}\" not found!".format(bdsim_in))
        name = (_path.splitext(_path.basename(bdsim_in))[0]
                if name is None else name)
-       data = pybdsim.Data.Load(bdsim_in)
+       data = _Data.Load(bdsim_in)
        if hasattr(data, 'optics'):
            data = data.optics
        elif hasattr(data, 'Optics'):
            data = data.Optics
        else:
            raise AttributeError("No optics found for BDSIM file: {}".format(bdsim_in))
        return data, name
    try:
-       if isinstance(bdsim_in, pybdsim.Data.RebdsimFile):
+       if isinstance(bdsim_in, _Data.RebdsimFile):
            if hasattr(bdsim_in,'optics'):
                bdsim_in = bdsim_in.optics
            elif hasattr(bdsim_in,'Optics'):
                bdsim_in = bdsim_in.Optics
            else:
                raise AttributeError("No optics found in rebdsim file.")
        name = bdsim_in.filename if name is None else name
@@ -103,15 +103,15 @@
         axes = _plt.gcf().gca()
         axes.set_ylabel(y_label)
         axes.set_xlabel(x_label)
         axes.legend(loc='best')
 
         if survey is not None:
            try:
-               pybdsim.Plot.AddMachineLatticeFromSurveyToFigure(_plt.gcf(), survey)
+               _Plot.AddMachineLatticeFromSurveyToFigure(_plt.gcf(), survey)
            except IOError:
                _pymadx.Plot.AddMachineLatticeToFigure(_plt.gcf(), survey)
         _plt.show(block=False)
         return plot
     return f_out
 
 PlotBeta   = _make_plotter(_BETA,    "S / m", r"$\beta_{x,y}$ / m",      "Beta")
```

### Comparing `pybdsim-3.2.0/src/pybdsim/Compare/__init__.py` & `pybdsim-3.3.0/src/pybdsim/Compare/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 #explicit imports to keep namespace clean
 
 from ._MadxBdsimComparison import MadxVsBDSIM
 from ._MadxBdsimComparison import MadxVsBDSIMOrbit
 from ._MadxBdsimComparison import MadxVsBDSIMOrbitResiduals
 from ._MadxBdsimComparison import MadxVsBDSIMFromGMAD
-
-try:
-    from ._TransportBdsimComparison import TransportVsBDSIM
-except ImportError:
-    pass
-
-from ._Mad8BdsimComparison import Mad8VsBDSIM
-
 from ._BdsimBdsimComparison import BDSIMVsBDSIM
 from ._BdsimBdsimComparison import PTCVsBDSIM
-
+from ._TransportBdsimComparison import TransportVsBDSIM
 from ._MadxMadxComparison import MadxVsMadx
-
 from ._MultipleCodeComparison import Optics
 from ._MultipleCodeComparison import OpticsResiduals
+from ._ElegantBdsimComparison import ElegantVsBDSIM
 
+# optional pymad8
+try:
+    from ._Mad8BdsimComparison import Mad8VsBDSIM
+except ImportError:
+    pass
 
-import pymad8 as _pymad8
-
+# optional pysad
 try:
     import pysad as _pysad
     from ._SadComparison import SadComparison
 except ImportError:
     pass
 
-from ._ElegantBdsimComparison import ElegantVsBDSIM
+
```

### Comparing `pybdsim-3.2.0/src/pybdsim/Constants.py` & `pybdsim-3.3.0/src/pybdsim/Constants.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Convert/_BdsimElement2TransferMatrix.py` & `pybdsim-3.3.0/src/pybdsim/Convert/_BdsimElement2TransferMatrix.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Convert/_BdsimPrimaries2Inrays.py` & `pybdsim-3.3.0/src/pybdsim/Convert/_BdsimPrimaries2Inrays.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Convert/_CPyMad2Gmad.py` & `pybdsim-3.3.0/src/pybdsim/Convert/_CPyMad2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Convert/_ElegantParamToStrength.py` & `pybdsim-3.3.0/src/pybdsim/Convert/_ElegantParamToStrength.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Convert/_Mad8Saveline2Gmad.py` & `pybdsim-3.3.0/src/pybdsim/Convert/_Mad8Saveline2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Convert/_Mad8Twiss2Gmad.py` & `pybdsim-3.3.0/src/pybdsim/Convert/_Mad8Twiss2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Convert/_Mad8Twiss2GmadOld.py` & `pybdsim-3.3.0/src/pybdsim/Convert/_Mad8Twiss2GmadOld.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Convert/_MadxTfs2Gmad.py` & `pybdsim-3.3.0/src/pybdsim/Convert/_MadxTfs2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Convert/_MadxTfs2GmadStrength.py` & `pybdsim-3.3.0/src/pybdsim/Convert/_MadxTfs2GmadStrength.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Convert/_Rebdsim2Numpy.py` & `pybdsim-3.3.0/src/pybdsim/Convert/_Rebdsim2Numpy.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Convert/_SadFlat2Gmad.py` & `pybdsim-3.3.0/src/pybdsim/Convert/_SadFlat2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Convert/_Transport2Gmad.py` & `pybdsim-3.3.0/src/pybdsim/Convert/_Transport2Gmad.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Wrapper for pytransport conversion.
 
 from pybdsim import Builder as _pyBuilder
 from pybdsim import Options as _Options
 
 from pytransport.Convert import _Convert
-from pytransport.Data import ConversionData
+from pytransport.Data import ConversionData as _ConversionData
 
 
 def Transport2Gmad(inputfile,
                    particle='proton',
                    distrType='gauss',
                    outputDir='gmad',
                    debug=False,
@@ -53,14 +53,14 @@
 
     >>> Transport2Gmad(inputfile)
 
     Writes converted machine to disk. Reader automatically detects if the supplied input file is a Transport input
     file or Transport output file.
 
     """
-    converter = _Convert(ConversionData(inputfile=inputfile, options=_Options.Options(), machine=_pyBuilder.Machine(),
-                                        particle=particle, debug=debug, distrType=distrType, gmad=True,
-                                        gmadDir=outputDir, madx=False, madxDir='', dontSplit=dontSplit,
-                                        keepName=keepName, combineDrifts=combineDrifts))
+    converter = _Convert(_ConversionData(inputfile=inputfile, options=_Options.Options(), machine=_pyBuilder.Machine(),
+                                         particle=particle, debug=debug, distrType=distrType, gmad=True,
+                                         gmadDir=outputDir, madx=False, madxDir='', dontSplit=dontSplit,
+                                         keepName=keepName, combineDrifts=combineDrifts))
     # automatically convert
     converter.Convert()
```

### Comparing `pybdsim-3.2.0/src/pybdsim/Convert/__init__.py` & `pybdsim-3.3.0/src/pybdsim/Convert/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 """
 Module for various conversions.
 
 """
-
+# pymadx
 from ._MadxTfs2Gmad import MadxTfs2Gmad
 from ._MadxTfs2Gmad import ZeroMissingRequiredColumns as _ZeroMissingRequiredColumns
 from ._MadxTfs2GmadStrength import MadxTfs2GmadStrength
 from ._MadxTfs2Gmad import MadxTfs2GmadBeam
-from ._Mad8Twiss2Gmad import Mad8Twiss2Gmad
+
+from ._BdsimPrimaries2Inrays import BdsimPrimaries2Ptc
+from ._BdsimPrimaries2Inrays import BdsimPrimaries2Madx
+from ._BdsimPrimaries2Inrays import BdsimPrimaries2Mad8
+from ._BdsimPrimaries2Inrays import BdsimSampler2Ptc
+from ._BdsimPrimaries2Inrays import BdsimPrimaries2BdsimUserFile
+from ._BdsimPrimaries2Inrays import BdsimSampler2BdsimUserFile
+
+from ._BdsimElement2TransferMatrix import BdsimElement2TransferMatrix
+
+from ._ElegantParamToStrength import ElegantParam2GmadStrength
+
 from ._Transport2Gmad import Transport2Gmad
 
-# all optional imports are quiet without warning, so we don't see print out all the time for each one
+# optional pymad8
+try:
+    from ._Mad8Twiss2Gmad import Mad8Twiss2Gmad
+except ImportError:
+    pass
 
+# optional pysad
 try:
     import pysad
     from ._SadFlat2Gmad import SadFlat2GMad
 except ImportError:
     pass
 
+# optional cpymad
 try:
     from ._CPyMad2Gmad import CPyMad2Gmad
 except ImportError:
     pass
 
-from ._BdsimPrimaries2Inrays import BdsimPrimaries2Ptc
-from ._BdsimPrimaries2Inrays import BdsimPrimaries2Madx
-from ._BdsimPrimaries2Inrays import BdsimPrimaries2Mad8
-from ._BdsimPrimaries2Inrays import BdsimSampler2Ptc
-from ._BdsimPrimaries2Inrays import BdsimPrimaries2BdsimUserFile
-from ._BdsimPrimaries2Inrays import BdsimSampler2BdsimUserFile
-
-from ._BdsimElement2TransferMatrix import BdsimElement2TransferMatrix
 
-from ._ElegantParamToStrength import ElegantParam2GmadStrength
```

### Comparing `pybdsim-3.2.0/src/pybdsim/Convert/collimator_analysis.py` & `pybdsim-3.3.0/src/pybdsim/Convert/collimator_analysis.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Data.py` & `pybdsim-3.3.0/src/pybdsim/Data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1410,14 +1410,55 @@
 
     def SortByBin(self):
         newBins = sorted(self.bins.items(), key=lambda item: item[1], reverse=True)
         self.bins = _defaultdict(float, **newBins)
         newSumWeightsSq = {key:self.sumWeightsSq[key] for key in newBins.keys()}
         self.sumWeightsSq = _defaultdict(float, **newSumWeightsSq)
 
+
+def GetHistoryPDGTuple(trajectories, startingTrajectoryStorageIndex, reduceDuplicates=False):
+    """
+    Return a tuple of PDG IDs for the history of a particle given by trajectories in an event.
+
+    :param trajectories: event.Trajectory instance from loaded ROOT data
+    :type trajectories: event.Trajectory
+    :param startingTrajectoryStorageIndex: storage index of which trajectory to start from
+    :type startingTrajectoryStorageIndex: int
+    :param reduceDuplicates: whether to remove sequential duplicates from the history
+    :type reduceDuplicates: bool
+
+    >>> d = pybdsim.Data.Load("somdbdsimoutputfile.root")
+    >>> et = d.GetEventTree()
+    >>> for event in et:
+            tid = event.sampler1.trackID[0]
+            history = pybdsim.Data.GetHistoryPDGTuple(event.Trajectory, tid)
+            print(history)
+
+    An example might be (13,211,211,2212) or with reducedDuplicates (31,211,2212)
+
+    Note, this will raise an IndexError if you haven't stored the right trajectories.
+    and must be used knowing that the connected trajectories for a given starting trackID
+    are stored.
+    """
+    ts = trajectories
+    storageIndex = startingTrajectoryStorageIndex
+    parentID = 1  # just not 0
+    history = []
+
+    while parentID != 0:
+        pdgID = ts.partID[storageIndex]
+        history.append(pdgID)
+        storageIndex = ts.parentIndex[storageIndex]
+        parentID = ts.parentID[storageIndex]
+    history.append(ts.partID[storageIndex])
+    history = tuple(history)
+    if reduceDuplicates:
+        history = tuple(x for x, y in _itertools.groupby(history))
+    return history
+
 class _SamplerData:
     """
     Base class for loading a chosen set of sampler data from a file.
     data - is the DataLoader instance.
     params - is a list of parameter names as strings.
     samplerIndexOrName - is the index of the sampler (0=primaries) or name.
```

### Comparing `pybdsim-3.2.0/src/pybdsim/DataUproot.py` & `pybdsim-3.3.0/src/pybdsim/DataUproot.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Field/FieldPlotter.py` & `pybdsim-3.3.0/src/pybdsim/Field/FieldPlotter.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Field/FieldPlotterVtk.py` & `pybdsim-3.3.0/src/pybdsim/Field/FieldPlotterVtk.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Field/_Field.py` & `pybdsim-3.3.0/src/pybdsim/Field/_Field.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Field/__init__.py` & `pybdsim-3.3.0/src/pybdsim/Field/__init__.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Geant4.py` & `pybdsim-3.3.0/src/pybdsim/Geant4.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Gmad.py` & `pybdsim-3.3.0/src/pybdsim/Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Joinhistograms.py` & `pybdsim-3.3.0/src/pybdsim/Joinhistograms.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/ModelProcessing.py` & `pybdsim-3.3.0/src/pybdsim/ModelProcessing.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Analysis.py` & `pybdsim-3.3.0/src/pybdsim/Obsolete/Rebdsim/Analysis.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/AnalysisRoot.py` & `pybdsim-3.3.0/src/pybdsim/Obsolete/Rebdsim/AnalysisRoot.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/AnalysisRootOptics.py` & `pybdsim-3.3.0/src/pybdsim/Obsolete/Rebdsim/AnalysisRootOptics.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Event.py` & `pybdsim-3.3.0/src/pybdsim/Obsolete/Rebdsim/Event.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Processed.py` & `pybdsim-3.3.0/src/pybdsim/Obsolete/Rebdsim/Processed.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Root.py` & `pybdsim-3.3.0/src/pybdsim/Obsolete/Rebdsim/Root.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/__init__.py` & `pybdsim-3.3.0/src/pybdsim/Obsolete/Rebdsim/__init__.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Optics.py` & `pybdsim-3.3.0/src/pybdsim/Optics.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Options.py` & `pybdsim-3.3.0/src/pybdsim/Options.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Plot.py` & `pybdsim-3.3.0/src/pybdsim/Plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -540,19 +540,17 @@
             _plt.yscale('log', nonposy='clip')
     else:
         _plt.ylim(ymin*0.8, ymax*1.05)
 
     _plt.tight_layout()
     return f
 
-def Spectra(spectra,
-            log=False, xlog=False,
-            xlabel=None, ylabel=None, title=None,
+def Spectra(spectra, log=False, xlog=False, xlabel=None, ylabel=None, title=None,
             scalingFactors=None, xScalingFactors=None,
-            figsize=(10,5), legendKwargs={}, **errorbarKwargs):
+            figsize=(10,5), legendKwargs={}, vmin=None, vmax=None, **errorbarKwargs):
     """
     Plot a Spectra object loaded from data that represents a set of histograms.
 
     returns a list of figure objects.
     """
     histograms = [spectra.histogramspy[(pdgid,flag)] for (pdgid,flag) in spectra.pdgidsSorted]
     
@@ -583,23 +581,42 @@
         labelsA = labels[:9]
         labelsB = labels[9:]
         if (0,'n') in spectra.pdgidsSorted:
             # if pdgid of 0, which is the 'total' histogram is present,
             # then it's integral must be the greatest and it should be first
             # in the A list, so also put it first in the B list
             histogramsB.insert(0, histogramsA[0])
+            labelsB.insert(0, labelsA[0])
             
         f1 = Histogram1DMultiple(histogramsA, labelsA, log, xlog, xlabel, ylabel, title,
                                  scalingFactors, xScalingFactors, figsize, legendKwargs, **errorbarKwargs)
         f2 = Histogram1DMultiple(histogramsB, labelsB, log, xlog, xlabel, ylabel, title,
                                  scalingFactors, xScalingFactors, figsize, legendKwargs, **errorbarKwargs)
+        for f in [f1,f2]:
+            ax = f.get_axes()[0]
+            if vmin:
+                yl = ax.get_ylim()
+                yl = (vmin,yl[1])
+                ax.set_ylim(*yl)
+            if vmax:
+                yl = ax.get_ylim()
+                yl = (yl[0],vmax)
+                ax.set_ylim(*yl)
         return [f1,f2]
     else:
         f1 = Histogram1DMultiple(histograms, labels, log, xlog, xlabel, ylabel, title,
                                  scalingFactors, xScalingFactors, figsize, legendKwargs, **errorbarKwargs)
+        if vmin:
+            yl = _plt.ylim()
+            yl = (vmin,yl[1])
+            _plt.ylim(*yl)
+        if vmax:
+            yl = _plt.ylim()
+            yl = (yl[0],vmax)
+            _plt.ylim(*yl)
         return [f1]
 
 
 def Histogram1DMultiple(histograms, labels, log=False, xlog=False, xlabel=None, ylabel=None, title=None, scalingFactors=None, xScalingFactors=None, figsize=(10,5), legendKwargs={}, **errorbarKwargs):
     """
     Plot multiple 1D histograms on the same plot. Histograms and labels should 
     be lists of the same length with pybdsim.Data.TH1 objects and strings.
@@ -713,18 +730,23 @@
     x, y = _np.meshgrid(h.xcentres,h.ycentres)
     sf  = scalingFactor #shortcut
     xsf = xScalingFactor
     ysf = yScalingFactor
     ext = [_np.min(xsf*h.xlowedge),_np.max(xsf*h.xhighedge),_np.min(ysf*h.ylowedge),_np.max(ysf*h.yhighedge)]
     histEmpty = len(h.contents[h.contents!=0]) == 0
     if vmin is None:
-        if autovmin and vmin is None and not histEmpty:
+        if autovmin and not histEmpty:
             vmin = _np.min(h.contents[h.contents!=0])
         else:
-            vmin = None
+            vmin = 1.0/h.entries # statistical floor and matplotlib requires a finite vmin
+    if vmax is None:
+        if histEmpty:
+            vmax = 1.0
+        else:
+            vmax = _np.max(h.contents)
     if logNorm:
         d = _copy.deepcopy(sf*h.contents.T)
         norm = _LogNorm(vmin=vmin,vmax=vmax) if vmax is not None else _LogNorm(vmin=vmin)
         ax = f.add_subplot(111)
         im = ax.pcolormesh(h.xedges*xsf, h.yedges*ysf, d, norm=norm, rasterized=True, **imshowKwargs)
         #_plt.imshow(d, extent=ext, origin='lower', aspect=aspect, norm=norm, interpolation='none', **imshowKwargs)
         if colourbar:
```

### Comparing `pybdsim-3.2.0/src/pybdsim/Run.py` & `pybdsim-3.3.0/src/pybdsim/Run.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Testing/bdsimMadx.py` & `pybdsim-3.3.0/src/pybdsim/Testing/bdsimMadx.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Testing/trackingTester.py` & `pybdsim-3.3.0/src/pybdsim/Testing/trackingTester.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Visualisation.py` & `pybdsim-3.3.0/src/pybdsim/Visualisation.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/Writer.py` & `pybdsim-3.3.0/src/pybdsim/Writer.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/XSecBias.py` & `pybdsim-3.3.0/src/pybdsim/XSecBias.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/_General.py` & `pybdsim-3.3.0/src/pybdsim/_General.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim/__init__.py` & `pybdsim-3.3.0/src/pybdsim/__init__.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/src/pybdsim.egg-info/PKG-INFO` & `pybdsim-3.3.0/src/pybdsim.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybdsim
-Version: 3.2.0
+Version: 3.3.0
 Summary: Python utilities for the Monte Carlo Particle accelerator code BDSIM.
 Author-email: "JAI@RHUL" <laurie.nevay@cern.ch>
 Maintainer-email: Laurie Nevay <laurie.nevay@cern.ch>
 Project-URL: homepage, http://www.pp.rhul.ac.uk/bdsim/pybdsim
 Project-URL: documentation, http://www.pp.rhul.ac.uk/bdsim/pybdsim
 Project-URL: repository, https://bitbucket.org/jairhul/pybdsim
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,28 +21,31 @@
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: uproot
 Provides-Extra: boost_histogram
 Provides-Extra: cpymad
 Provides-Extra: pysad
+Provides-Extra: pymad8
+Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE.txt
 License-File: COPYING.txt
 
 # pybdsim #
 
 A python package containing both utilities for preparing and analysing BDSIM input and output as well as controlling BDSIM.
 
 ## Authors ##
 
 L. Nevay
 A. Abramov
 S. Alden
 S. Boogert
+M. Deniaud
 C. Hernalsteens
 W. Parker
 E. Ramoisiaux
 W. Shields
 J. Snuverink
 R. Tesse
 S. Walker
```

### Comparing `pybdsim-3.2.0/src/pybdsim.egg-info/SOURCES.txt` & `pybdsim-3.3.0/src/pybdsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz` & `pybdsim-3.3.0/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/tests/test_input/model-model-aper.tfs.gz` & `pybdsim-3.3.0/tests/test_input/model-model-aper.tfs.gz`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/tests/test_input/model-model.tfs.gz` & `pybdsim-3.3.0/tests/test_input/model-model.tfs.gz`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/tests/test_output/atf2-nominal-twiss-v5.2/model_components.gmad` & `pybdsim-3.3.0/tests/test_output/atf2-nominal-twiss-v5.2/model_components.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/tests/test_output/atf2-nominal-twiss-v5.2/model_sequence.gmad` & `pybdsim-3.3.0/tests/test_output/atf2-nominal-twiss-v5.2/model_sequence.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/tests/test_output/model-model/model_components.gmad` & `pybdsim-3.3.0/tests/test_output/model-model/model_components.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/tests/test_output/model-model/model_sequence.gmad` & `pybdsim-3.3.0/tests/test_output/model-model/model_sequence.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_components.gmad` & `pybdsim-3.3.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_components.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_sequence.gmad` & `pybdsim-3.3.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_sequence.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/tests/test_output2/model-model/model_components.gmad` & `pybdsim-3.3.0/tests/test_output2/model-model/model_components.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/tests/test_output2/model-model/model_sequence.gmad` & `pybdsim-3.3.0/tests/test_output2/model-model/model_sequence.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/tests/tests/pybdsim_test_utils.py` & `pybdsim-3.3.0/tests/tests/pybdsim_test_utils.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/tests/tests/test_MadxTfs2Gmad.py` & `pybdsim-3.3.0/tests/tests/test_MadxTfs2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/tests/tests/testratio.py` & `pybdsim-3.3.0/tests/tests/testratio.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/tests/tests/write_test_outputs.py` & `pybdsim-3.3.0/tests/tests/write_test_outputs.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.2.0/tests/unit/test_Builder.py` & `pybdsim-3.3.0/tests/unit/test_Builder.py`

 * *Files identical despite different names*

