# Comparing `tmp/waipy-0.0.8.9.tar.gz` & `tmp/waipy-0.0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/waipy-0.0.8.9.tar", last modified: Thu Oct 17 12:50:22 2013, max compression
+gzip compressed data, was "dist/waipy-0.0.9.0.tar", last modified: Wed Jan  8 16:59:20 2014, max compression
```

## Comparing `waipy-0.0.8.9.tar` & `waipy-0.0.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 calim      (502) staff       (20)        0 2013-10-17 12:50:22.000000 waipy-0.0.8.9/
-drwxr-xr-x   0 calim      (502) staff       (20)        0 2013-10-17 12:50:22.000000 waipy-0.0.8.9/lib/
-drwxr-xr-x   0 calim      (502) staff       (20)        0 2013-10-17 12:50:22.000000 waipy-0.0.8.9/lib/waipy/
--rw-r--r--   0 calim      (502) staff       (20)      970 2013-10-17 12:50:06.000000 waipy-0.0.8.9/lib/waipy/__init__.py
-drwxr-xr-x   0 calim      (502) staff       (20)        0 2013-10-17 12:50:22.000000 waipy-0.0.8.9/lib/waipy/cwa/
--rw-r--r--   0 calim      (502) staff       (20)       88 2013-06-27 18:26:35.000000 waipy-0.0.8.9/lib/waipy/cwa/__init__.py
--rw-r--r--   0 calim      (502) staff       (20)     3826 2013-07-04 18:01:07.000000 waipy-0.0.8.9/lib/waipy/cwa/cross_wavelet.py
-drwxr-xr-x   0 calim      (502) staff       (20)        0 2013-10-17 12:50:22.000000 waipy-0.0.8.9/lib/waipy/cwt/
--rw-r--r--   0 calim      (502) staff       (20)       88 2013-06-27 18:26:35.000000 waipy-0.0.8.9/lib/waipy/cwt/__init__.py
--rw-r--r--   0 calim      (502) staff       (20)     8954 2013-07-22 19:27:25.000000 waipy-0.0.8.9/lib/waipy/cwt/lib_wavelet.py
--rw-r--r--   0 calim      (502) staff       (20)     7876 2013-10-17 12:46:23.000000 waipy-0.0.8.9/lib/waipy/cwt/wavetest.py
--rw-r--r--   0 calim      (502) staff       (20)       88 2013-06-27 18:26:35.000000 waipy-0.0.8.9/lib/waipy/mainmodule.py
-drwxr-xr-x   0 calim      (502) staff       (20)        0 2013-10-17 12:50:22.000000 waipy-0.0.8.9/lib/waipy.egg-info/
--rw-r--r--   0 calim      (502) staff       (20)        1 2013-10-17 12:50:22.000000 waipy-0.0.8.9/lib/waipy.egg-info/dependency_links.txt
--rw-r--r--   0 calim      (502) staff       (20)      480 2013-10-17 12:50:22.000000 waipy-0.0.8.9/lib/waipy.egg-info/PKG-INFO
--rw-r--r--   0 calim      (502) staff       (20)      324 2013-10-17 12:50:22.000000 waipy-0.0.8.9/lib/waipy.egg-info/SOURCES.txt
--rw-r--r--   0 calim      (502) staff       (20)        6 2013-10-17 12:50:22.000000 waipy-0.0.8.9/lib/waipy.egg-info/top_level.txt
--rw-r--r--   0 calim      (502) staff       (20)      480 2013-10-17 12:50:22.000000 waipy-0.0.8.9/PKG-INFO
--rw-r--r--   0 calim      (502) staff       (20)       59 2013-10-17 12:50:22.000000 waipy-0.0.8.9/setup.cfg
--rw-r--r--   0 calim      (502) staff       (20)      834 2013-06-27 18:28:32.000000 waipy-0.0.8.9/setup.py
+drwxr-xr-x   0 calim      (502) staff       (20)        0 2014-01-08 16:59:20.000000 waipy-0.0.9.0/
+drwxr-xr-x   0 calim      (502) staff       (20)        0 2014-01-08 16:59:20.000000 waipy-0.0.9.0/lib/
+drwxr-xr-x   0 calim      (502) staff       (20)        0 2014-01-08 16:59:20.000000 waipy-0.0.9.0/lib/waipy/
+-rw-r--r--   0 calim      (502) staff       (20)      970 2014-01-08 16:59:05.000000 waipy-0.0.9.0/lib/waipy/__init__.py
+drwxr-xr-x   0 calim      (502) staff       (20)        0 2014-01-08 16:59:20.000000 waipy-0.0.9.0/lib/waipy/cwa/
+-rw-r--r--   0 calim      (502) staff       (20)       88 2013-06-27 18:26:35.000000 waipy-0.0.9.0/lib/waipy/cwa/__init__.py
+-rw-r--r--   0 calim      (502) staff       (20)     3826 2013-07-04 18:01:07.000000 waipy-0.0.9.0/lib/waipy/cwa/cross_wavelet.py
+drwxr-xr-x   0 calim      (502) staff       (20)        0 2014-01-08 16:59:20.000000 waipy-0.0.9.0/lib/waipy/cwt/
+-rw-r--r--   0 calim      (502) staff       (20)       88 2013-06-27 18:26:35.000000 waipy-0.0.9.0/lib/waipy/cwt/__init__.py
+-rw-r--r--   0 calim      (502) staff       (20)     8954 2013-07-22 19:27:25.000000 waipy-0.0.9.0/lib/waipy/cwt/lib_wavelet.py
+-rw-r--r--   0 calim      (502) staff       (20)     7869 2014-01-08 16:57:07.000000 waipy-0.0.9.0/lib/waipy/cwt/wavetest.py
+-rw-r--r--   0 calim      (502) staff       (20)       88 2013-06-27 18:26:35.000000 waipy-0.0.9.0/lib/waipy/mainmodule.py
+drwxr-xr-x   0 calim      (502) staff       (20)        0 2014-01-08 16:59:20.000000 waipy-0.0.9.0/lib/waipy.egg-info/
+-rw-r--r--   0 calim      (502) staff       (20)        1 2014-01-08 16:59:20.000000 waipy-0.0.9.0/lib/waipy.egg-info/dependency_links.txt
+-rw-r--r--   0 calim      (502) staff       (20)      480 2014-01-08 16:59:20.000000 waipy-0.0.9.0/lib/waipy.egg-info/PKG-INFO
+-rw-r--r--   0 calim      (502) staff       (20)      324 2014-01-08 16:59:20.000000 waipy-0.0.9.0/lib/waipy.egg-info/SOURCES.txt
+-rw-r--r--   0 calim      (502) staff       (20)        6 2014-01-08 16:59:20.000000 waipy-0.0.9.0/lib/waipy.egg-info/top_level.txt
+-rw-r--r--   0 calim      (502) staff       (20)      480 2014-01-08 16:59:20.000000 waipy-0.0.9.0/PKG-INFO
+-rw-r--r--   0 calim      (502) staff       (20)       59 2014-01-08 16:59:20.000000 waipy-0.0.9.0/setup.cfg
+-rw-r--r--   0 calim      (502) staff       (20)      834 2013-06-27 18:28:32.000000 waipy-0.0.9.0/setup.py
```

### Comparing `waipy-0.0.8.9/lib/waipy/__init__.py` & `waipy-0.0.9.0/lib/waipy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 
 
 
 # Define the objects imported by imports of the form: from pyclimatetools import *
 __all__ = ['nextpow2', 'wave_bases', 'wavelet', 'wave_signif','load_txt','load_nc','normalize','cwt','wavelet_plot','fft','cross_wavelet','plot_cross', 'plot_cohere']
 
 # Package version number.
-__version__ = '0.0.8.9'
+__version__ = '0.0.9.0'
```

### Comparing `waipy-0.0.8.9/lib/waipy/cwa/cross_wavelet.py` & `waipy-0.0.9.0/lib/waipy/cwa/cross_wavelet.py`

 * *Files identical despite different names*

### Comparing `waipy-0.0.8.9/lib/waipy/cwt/lib_wavelet.py` & `waipy-0.0.9.0/lib/waipy/cwt/lib_wavelet.py`

 * *Files identical despite different names*

### Comparing `waipy-0.0.8.9/lib/waipy/cwt/wavetest.py` & `waipy-0.0.9.0/lib/waipy/cwt/wavetest.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 	dtmax = result['power'].max()
 	lev = []
 	for i in range(int(log2(dtmax/dtmin))):
         	dtmin =dtmin*2
         	lev.append(dtmin)
 	return lev
 
-def wavelet_plot(var,time,data,data1,dtmin,result,impath):
+def wavelet_plot(var,time,data,dtmin,result,impath):
 	"""PLOT WAVELET TRANSFORM
 	   var 	 = title name from data
 	   time  = vector get in load function
 	   data  = from normalize function
 	   dtmin = minimum resolution :1 octave		 
 	   result= dict from cwt function 
 	"""
@@ -136,15 +136,15 @@
 	fig = plt.figure(figsize=(15,10), dpi=100)
 	ax = fig.add_subplot(411)
         # frequency limit
         lim = np.where(result['period'] == result['period'][-1]/2)[0][0]
         # ----------------------------------------------------------------------------------------------------------------#
 	"""Plot time series """
 	subplot(3,1,1)
-	plot(time,data1)
+	plot(time,data)
 	xlabel('Time')
 	ylabel('%s'%var)
 	title('TIME SERIES')
 	# ----------------------------------------------------------------------------------------------------------------#
 	subplot(7,4,14)
 	plot(range(-result['nw']/2,result['nw']/2),result['joint_wavelet'],'k')
 	plot(range(-result['nw']/2,result['nw']/2),result['imag_wavelet'],'--k')
```

### Comparing `waipy-0.0.8.9/setup.py` & `waipy-0.0.9.0/setup.py`

 * *Files identical despite different names*

