# Comparing `tmp/CDSupdate-1.1.0.tar.gz` & `tmp/CDSupdate-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CDSupdate-1.1.0.tar", last modified: Fri May  5 06:01:47 2023, max compression
+gzip compressed data, was "CDSupdate-1.2.1.tar", last modified: Mon May  8 10:03:39 2023, max compression
```

## Comparing `CDSupdate-1.1.0.tar` & `CDSupdate-1.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-05 06:01:47.895380 CDSupdate-1.1.0/
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-05 06:01:47.891449 CDSupdate-1.1.0/CDSupdate/
--rw-r--r--   0 yrobin     (501) staff       (20)     9376 2023-05-04 08:04:46.000000 CDSupdate-1.1.0/CDSupdate/__CDSUParams.py
--rw-r--r--   0 yrobin     (501) staff       (20)     5131 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/CDSupdate/__CVarsParams.py
--rw-r--r--   0 yrobin     (501) staff       (20)     2685 2022-08-31 14:53:13.000000 CDSupdate-1.1.0/CDSupdate/__curses_doc.py
--rw-r--r--   0 yrobin     (501) staff       (20)     3744 2023-05-05 06:01:11.000000 CDSupdate-1.1.0/CDSupdate/__doc.py
--rw-r--r--   0 yrobin     (501) staff       (20)      847 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/CDSupdate/__exceptions.py
--rw-r--r--   0 yrobin     (501) staff       (20)     4268 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/CDSupdate/__exec.py
--rw-r--r--   0 yrobin     (501) staff       (20)    15304 2023-05-05 06:01:11.000000 CDSupdate-1.1.0/CDSupdate/__extracvars.py
--rw-r--r--   0 yrobin     (501) staff       (20)      974 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/CDSupdate/__init__.py
--rw-r--r--   0 yrobin     (501) staff       (20)    14464 2023-05-03 12:54:20.000000 CDSupdate-1.1.0/CDSupdate/__io.py
--rw-r--r--   0 yrobin     (501) staff       (20)     1912 2023-05-05 06:01:11.000000 CDSupdate-1.1.0/CDSupdate/__release.py
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-05 06:01:47.894758 CDSupdate-1.1.0/CDSupdate/data/
--rw-r--r--   0 yrobin     (501) staff       (20)      574 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/CDSupdate/data/ERA5-dptas-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)     1865 2023-05-05 06:01:11.000000 CDSupdate-1.1.0/CDSupdate/data/ERA5-name.csv
--rw-r--r--   0 yrobin     (501) staff       (20)     1572 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/CDSupdate/data/ERA5-pr-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      717 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/CDSupdate/data/ERA5-ps-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      830 2022-08-31 14:53:14.000000 CDSupdate-1.1.0/CDSupdate/data/ERA5-psl-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      858 2023-05-05 06:01:11.000000 CDSupdate-1.1.0/CDSupdate/data/ERA5-rlds-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)     1280 2023-05-05 06:01:11.000000 CDSupdate-1.1.0/CDSupdate/data/ERA5-rsds-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      380 2022-08-31 14:53:14.000000 CDSupdate-1.1.0/CDSupdate/data/ERA5-tas-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      604 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/CDSupdate/data/ERA5-uas-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      606 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/CDSupdate/data/ERA5-vas-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      842 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/CDSupdate/data/ERA5-zg-description.txt
--rw-r--r--   0 yrobin     (501) staff       (20)      723 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/CDSupdate/data/__init__.py
--rw-r--r--   0 yrobin     (501) staff       (20)      134 2023-05-03 06:31:49.000000 CDSupdate-1.1.0/CDSupdate/data/areas.csv
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-05 06:01:47.892266 CDSupdate-1.1.0/CDSupdate.egg-info/
--rw-r--r--   0 yrobin     (501) staff       (20)     2326 2023-05-05 06:01:47.000000 CDSupdate-1.1.0/CDSupdate.egg-info/PKG-INFO
--rw-r--r--   0 yrobin     (501) staff       (20)      935 2023-05-05 06:01:47.000000 CDSupdate-1.1.0/CDSupdate.egg-info/SOURCES.txt
--rw-r--r--   0 yrobin     (501) staff       (20)        1 2023-05-05 06:01:47.000000 CDSupdate-1.1.0/CDSupdate.egg-info/dependency_links.txt
--rw-r--r--   0 yrobin     (501) staff       (20)       42 2023-05-05 06:01:47.000000 CDSupdate-1.1.0/CDSupdate.egg-info/requires.txt
--rw-r--r--   0 yrobin     (501) staff       (20)       10 2023-05-05 06:01:47.000000 CDSupdate-1.1.0/CDSupdate.egg-info/top_level.txt
--rw-r--r--   0 yrobin     (501) staff       (20)    35149 2022-03-16 15:22:09.000000 CDSupdate-1.1.0/LICENSE
--rw-r--r--   0 yrobin     (501) staff       (20)       58 2022-08-31 14:53:14.000000 CDSupdate-1.1.0/MANIFEST.in
--rw-r--r--   0 yrobin     (501) staff       (20)     2326 2023-05-05 06:01:47.895180 CDSupdate-1.1.0/PKG-INFO
--rw-r--r--   0 yrobin     (501) staff       (20)     1568 2023-05-04 08:04:46.000000 CDSupdate-1.1.0/README.md
-drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-05 06:01:47.894959 CDSupdate-1.1.0/scripts/
--rwxr-xr-x   0 yrobin     (501) staff       (20)      894 2023-05-02 14:45:32.000000 CDSupdate-1.1.0/scripts/cdsupdate
--rw-r--r--   0 yrobin     (501) staff       (20)       38 2023-05-05 06:01:47.895429 CDSupdate-1.1.0/setup.cfg
--rwxr-xr-x   0 yrobin     (501) staff       (20)     2417 2023-05-04 08:04:46.000000 CDSupdate-1.1.0/setup.py
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-08 10:03:39.371984 CDSupdate-1.2.1/
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-08 10:03:39.366754 CDSupdate-1.2.1/CDSupdate/
+-rw-r--r--   0 yrobin     (501) staff       (20)     9431 2023-05-08 10:02:58.000000 CDSupdate-1.2.1/CDSupdate/__CDSUParams.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     5131 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/CDSupdate/__CVarsParams.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     2685 2022-08-31 14:53:13.000000 CDSupdate-1.2.1/CDSupdate/__curses_doc.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     3744 2023-05-05 06:01:11.000000 CDSupdate-1.2.1/CDSupdate/__doc.py
+-rw-r--r--   0 yrobin     (501) staff       (20)      847 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/CDSupdate/__exceptions.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     4268 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/CDSupdate/__exec.py
+-rw-r--r--   0 yrobin     (501) staff       (20)    12881 2023-05-08 10:02:58.000000 CDSupdate-1.2.1/CDSupdate/__extracvars.py
+-rw-r--r--   0 yrobin     (501) staff       (20)      974 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/CDSupdate/__init__.py
+-rw-r--r--   0 yrobin     (501) staff       (20)    14464 2023-05-03 12:54:20.000000 CDSupdate-1.2.1/CDSupdate/__io.py
+-rw-r--r--   0 yrobin     (501) staff       (20)     1912 2023-05-08 10:02:58.000000 CDSupdate-1.2.1/CDSupdate/__release.py
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-08 10:03:39.371371 CDSupdate-1.2.1/CDSupdate/data/
+-rw-r--r--   0 yrobin     (501) staff       (20)      574 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/CDSupdate/data/ERA5-dptas-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)     2027 2023-05-08 10:02:58.000000 CDSupdate-1.2.1/CDSupdate/data/ERA5-name.csv
+-rw-r--r--   0 yrobin     (501) staff       (20)     1572 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/CDSupdate/data/ERA5-pr-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      717 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/CDSupdate/data/ERA5-ps-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      830 2022-08-31 14:53:14.000000 CDSupdate-1.2.1/CDSupdate/data/ERA5-psl-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      858 2023-05-05 06:01:11.000000 CDSupdate-1.2.1/CDSupdate/data/ERA5-rlds-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)     1280 2023-05-05 06:01:11.000000 CDSupdate-1.2.1/CDSupdate/data/ERA5-rsds-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      380 2022-08-31 14:53:14.000000 CDSupdate-1.2.1/CDSupdate/data/ERA5-tas-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      604 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/CDSupdate/data/ERA5-uas-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      606 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/CDSupdate/data/ERA5-vas-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      842 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/CDSupdate/data/ERA5-zg-description.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)      723 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/CDSupdate/data/__init__.py
+-rw-r--r--   0 yrobin     (501) staff       (20)      134 2023-05-03 06:31:49.000000 CDSupdate-1.2.1/CDSupdate/data/areas.csv
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-08 10:03:39.367621 CDSupdate-1.2.1/CDSupdate.egg-info/
+-rw-r--r--   0 yrobin     (501) staff       (20)     2326 2023-05-08 10:03:39.000000 CDSupdate-1.2.1/CDSupdate.egg-info/PKG-INFO
+-rw-r--r--   0 yrobin     (501) staff       (20)      935 2023-05-08 10:03:39.000000 CDSupdate-1.2.1/CDSupdate.egg-info/SOURCES.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)        1 2023-05-08 10:03:39.000000 CDSupdate-1.2.1/CDSupdate.egg-info/dependency_links.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)       42 2023-05-08 10:03:39.000000 CDSupdate-1.2.1/CDSupdate.egg-info/requires.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)       10 2023-05-08 10:03:39.000000 CDSupdate-1.2.1/CDSupdate.egg-info/top_level.txt
+-rw-r--r--   0 yrobin     (501) staff       (20)    35149 2022-03-16 15:22:09.000000 CDSupdate-1.2.1/LICENSE
+-rw-r--r--   0 yrobin     (501) staff       (20)       58 2022-08-31 14:53:14.000000 CDSupdate-1.2.1/MANIFEST.in
+-rw-r--r--   0 yrobin     (501) staff       (20)     2326 2023-05-08 10:03:39.371833 CDSupdate-1.2.1/PKG-INFO
+-rw-r--r--   0 yrobin     (501) staff       (20)     1568 2023-05-04 08:04:46.000000 CDSupdate-1.2.1/README.md
+drwxr-xr-x   0 yrobin     (501) staff       (20)        0 2023-05-08 10:03:39.371649 CDSupdate-1.2.1/scripts/
+-rwxr-xr-x   0 yrobin     (501) staff       (20)      894 2023-05-02 14:45:32.000000 CDSupdate-1.2.1/scripts/cdsupdate
+-rw-r--r--   0 yrobin     (501) staff       (20)       38 2023-05-08 10:03:39.372027 CDSupdate-1.2.1/setup.cfg
+-rwxr-xr-x   0 yrobin     (501) staff       (20)     2417 2023-05-04 08:04:46.000000 CDSupdate-1.2.1/setup.py
```

### Comparing `CDSupdate-1.1.0/CDSupdate/__CDSUParams.py` & `CDSupdate-1.2.1/CDSupdate/__CDSUParams.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,15 @@
 			## If help, stop
 			if self.help:
 				raise AbortForHelpException
 			
 			## Test of the output dir exist
 			if self.output_dir is None:
 				raise Exception("Output directory must be given!")
+			self.output_dir = os.path.split(self.output_dir)[0]
 			if not os.path.isdir(self.output_dir):
 				raise Exception( f"Output directory {self.output_dir} is not a path!" )
 			if self.output_dir.split(os.path.sep)[-1] == "ERA5":
 				self.output_dir = os.path.sep.join( self.output_dir.split(os.path.sep)[:-1] )
 			
 			## Test if the tmp directory exists
 			if self.tmp is not None:
```

### Comparing `CDSupdate-1.1.0/CDSupdate/__CVarsParams.py` & `CDSupdate-1.2.1/CDSupdate/__CVarsParams.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.1.0/CDSupdate/__curses_doc.py` & `CDSupdate-1.2.1/CDSupdate/__curses_doc.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.1.0/CDSupdate/__doc.py` & `CDSupdate-1.2.1/CDSupdate/__doc.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.1.0/CDSupdate/__exceptions.py` & `CDSupdate-1.2.1/CDSupdate/__exceptions.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.1.0/CDSupdate/__exec.py` & `CDSupdate-1.2.1/CDSupdate/__exec.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.1.0/CDSupdate/__extracvars.py` & `CDSupdate-1.2.1/CDSupdate/__extracvars.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,72 +43,14 @@
 logger.addHandler(logging.NullHandler())
 
 
 ###############
 ## Functions ##
 ###############
 
-def build_tasmin():##{{{
-	
-	area_name = cdsuParams.area_name
-	ipath  = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , "tas" )
-	ifiles = os.listdir(ipath)
-	ifiles.sort()
-	cvar = "tasmin"
-	
-	for ifile in ifiles:
-		
-		idata = xr.open_dataset( os.path.join( ipath , ifile ) )
-		year  = idata.time.dt.year[0].values
-		dtime = [dt.datetime(int(year),1,1) + dt.timedelta( days = int(i) - 1 ) for i in np.unique(idata.time.dt.dayofyear.values)]
-		
-		## Build daily variable
-		ddata = idata.groupby("time.dayofyear").min().rename( dayofyear = "time" ).assign_coords( time = dtime ).rename( { "tas" : cvar } )
-		
-		## Save daily variable
-		opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "day" , cvar )
-		t0    = str(ddata.time[ 0].values)[:10].replace("-","").replace(" ","").replace("T","")
-		t1    = str(ddata.time[-1].values)[:10].replace("-","").replace(" ","").replace("T","")
-		ofile = f"ERA5-AMIP_{cvar}_day_{area_name}_{t0}-{t1}.nc"
-		target = os.path.join( opath , ofile )
-		if not os.path.isdir(opath):
-			os.makedirs(opath)
-		logger.info( f" * Save 'TMP/ERA5-AMIP/day/{cvar}/{ofile}'" )
-		ddata.to_netcdf( os.path.join( opath , ofile ) )
-##}}}
-
-def build_tasmax():##{{{
-	
-	area_name = cdsuParams.area_name
-	ipath  = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , "tas" )
-	ifiles = os.listdir(ipath)
-	ifiles.sort()
-	cvar = "tasmax"
-	
-	for ifile in ifiles:
-		
-		idata = xr.open_dataset( os.path.join( ipath , ifile ) )
-		year  = idata.time.dt.year[0].values
-		dtime = [dt.datetime(int(year),1,1) + dt.timedelta( days = int(i) - 1 ) for i in np.unique(idata.time.dt.dayofyear.values)]
-		
-		## Build daily variable
-		ddata = idata.groupby("time.dayofyear").max().rename( dayofyear = "time" ).assign_coords( time = dtime ).rename( { "tas" : cvar } )
-		
-		## Save daily variable
-		opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "day" , cvar )
-		t0    = str(ddata.time[ 0].values)[:10].replace("-","").replace(" ","").replace("T","")
-		t1    = str(ddata.time[-1].values)[:10].replace("-","").replace(" ","").replace("T","")
-		ofile = f"ERA5-AMIP_{cvar}_day_{area_name}_{t0}-{t1}.nc"
-		target = os.path.join( opath , ofile )
-		if not os.path.isdir(opath):
-			os.makedirs(opath)
-		logger.info( f" * Save 'TMP/ERA5-AMIP/day/{cvar}/{ofile}'" )
-		ddata.to_netcdf( os.path.join( opath , ofile ) )
-##}}}
-
 def build_sfcWind():##{{{
 	
 	area_name = cdsuParams.area_name
 	
 	## files
 	ipathu  = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , "uas" )
 	ipathv  = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , "vas" )
@@ -152,48 +94,14 @@
 		if not os.path.isdir(opath):
 			os.makedirs(opath)
 		logger.info( f" * Save 'TMP/ERA5-AMIP/day/sfcWind/{ofile}'" )
 		odatad.to_netcdf( os.path.join( opath , ofile ) )
 	
 ##}}}
 
-def build_sfcWindmax():##{{{
-	
-	cvar = "sfcWindmax"
-	area_name = cdsuParams.area_name
-	
-	## files
-	cvar0   = "sfcWind"
-	ipath0  = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , cvar0 )
-	ifiles0 = os.listdir(ipath0)
-	ifiles0.sort()
-	
-	
-	for ifile0 in ifiles0:
-		
-		idata0 = xr.open_dataset( os.path.join( ipath0 , ifile0 ) )
-		
-		year  = idata0.time.dt.year[0].values
-		dtime = [dt.datetime(int(year),1,1) + dt.timedelta( days = int(i) - 1 ) for i in np.unique(idata0.time.dt.dayofyear.values)]
-		
-		## Build daily
-		odatad = idata0.groupby("time.dayofyear").max().rename( dayofyear = "time" ).assign_coords( time = dtime ).rename( { cvar0 : cvar } )
-		
-		## Save daily
-		opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "day" , cvar )
-		t0    = str(odatad.time[ 0].values)[:10].replace("-","").replace(" ","").replace("T","")
-		t1    = str(odatad.time[-1].values)[:10].replace("-","").replace(" ","").replace("T","")
-		ofile = f"ERA5-AMIP_{cvar}_day_{area_name}_{t0}-{t1}.nc"
-		target = os.path.join( opath , ofile )
-		if not os.path.isdir(opath):
-			os.makedirs(opath)
-		logger.info( f" * Save 'TMP/ERA5-AMIP/day/{cvar}/{ofile}'" )
-		odatad.to_netcdf( os.path.join( opath , ofile ) )
-##}}}
-
 def build_hurs():##{{{
 	
 	cvar = "hurs"
 	area_name = cdsuParams.area_name
 	
 	## files
 	ipathD  = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , "dptas" )
@@ -239,48 +147,14 @@
 		target = os.path.join( opath , ofile )
 		if not os.path.isdir(opath):
 			os.makedirs(opath)
 		logger.info( f" * Save 'TMP/ERA5-AMIP/day/{cvar}/{ofile}'" )
 		odatad.to_netcdf( os.path.join( opath , ofile ) )
 ##}}}
 
-def build_hursmax():##{{{
-	
-	cvar = "hursmax"
-	area_name = cdsuParams.area_name
-	
-	## files
-	cvar0   = "hurs"
-	ipath0  = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , cvar0 )
-	ifiles0 = os.listdir(ipath0)
-	ifiles0.sort()
-	
-	
-	for ifile0 in ifiles0:
-		
-		idata0 = xr.open_dataset( os.path.join( ipath0 , ifile0 ) )
-		
-		year  = idata0.time.dt.year[0].values
-		dtime = [dt.datetime(int(year),1,1) + dt.timedelta( days = int(i) - 1 ) for i in np.unique(idata0.time.dt.dayofyear.values)]
-		
-		## Build daily
-		odatad = idata0.groupby("time.dayofyear").max().rename( dayofyear = "time" ).assign_coords( time = dtime ).rename( { cvar0 : cvar } )
-		
-		## Save daily
-		opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "day" , cvar )
-		t0    = str(odatad.time[ 0].values)[:10].replace("-","").replace(" ","").replace("T","")
-		t1    = str(odatad.time[-1].values)[:10].replace("-","").replace(" ","").replace("T","")
-		ofile = f"ERA5-AMIP_{cvar}_day_{area_name}_{t0}-{t1}.nc"
-		target = os.path.join( opath , ofile )
-		if not os.path.isdir(opath):
-			os.makedirs(opath)
-		logger.info( f" * Save 'TMP/ERA5-AMIP/day/{cvar}/{ofile}'" )
-		odatad.to_netcdf( os.path.join( opath , ofile ) )
-##}}}
-
 def build_huss():##{{{
 	
 	cvar = "huss"
 	area_name = cdsuParams.area_name
 	
 	## files
 	ipathD  = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , "dptas" )
@@ -399,32 +273,94 @@
 		target = os.path.join( opath , ofile )
 		if not os.path.isdir(opath):
 			os.makedirs(opath)
 		logger.info( f" * Save 'TMP/ERA5-AMIP/day/{cvar}/{ofile}'" )
 		odatad.to_netcdf( os.path.join( opath , ofile ) )
 ##}}}
 
+def build_cvarmin( cvar ):##{{{
+	
+	cvarN = f"{cvar}min"
+	area_name = cdsuParams.area_name
+	
+	## files
+	ipath  = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , cvar )
+	ifiles = os.listdir(ipath)
+	ifiles.sort()
+	
+	
+	for ifile in ifiles:
+		
+		idata = xr.open_dataset( os.path.join( ipath , ifile ) )
+		
+		year  = idata.time.dt.year[0].values
+		dtime = [dt.datetime(int(year),1,1) + dt.timedelta( days = int(i) - 1 ) for i in np.unique(idata.time.dt.dayofyear.values)]
+		
+		## Build daily
+		odatad = idata.groupby("time.dayofyear").min().rename( dayofyear = "time" ).assign_coords( time = dtime ).rename( { cvar : cvarN } )
+		
+		## Save daily
+		opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "day" , cvarN )
+		t0    = str(odatad.time[ 0].values)[:10].replace("-","").replace(" ","").replace("T","")
+		t1    = str(odatad.time[-1].values)[:10].replace("-","").replace(" ","").replace("T","")
+		ofile = f"ERA5-AMIP_{cvarN}_day_{area_name}_{t0}-{t1}.nc"
+		target = os.path.join( opath , ofile )
+		if not os.path.isdir(opath):
+			os.makedirs(opath)
+		logger.info( f" * Save 'TMP/ERA5-AMIP/day/{cvarN}/{ofile}'" )
+		odatad.to_netcdf( os.path.join( opath , ofile ) )
+##}}}
+
+def build_cvarmax( cvar ):##{{{
+	
+	cvarX = f"{cvar}max"
+	area_name = cdsuParams.area_name
+	
+	## files
+	ipath  = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "hr" , cvar )
+	ifiles = os.listdir(ipath)
+	ifiles.sort()
+	
+	
+	for ifile in ifiles:
+		
+		idata = xr.open_dataset( os.path.join( ipath , ifile ) )
+		
+		year  = idata.time.dt.year[0].values
+		dtime = [dt.datetime(int(year),1,1) + dt.timedelta( days = int(i) - 1 ) for i in np.unique(idata.time.dt.dayofyear.values)]
+		
+		## Build daily
+		odatad = idata.groupby("time.dayofyear").max().rename( dayofyear = "time" ).assign_coords( time = dtime ).rename( { cvar : cvarX } )
+		
+		## Save daily
+		opath = os.path.join( cdsuParams.tmp , "ERA5-AMIP" , "day" , cvarX )
+		t0    = str(odatad.time[ 0].values)[:10].replace("-","").replace(" ","").replace("T","")
+		t1    = str(odatad.time[-1].values)[:10].replace("-","").replace(" ","").replace("T","")
+		ofile = f"ERA5-AMIP_{cvarX}_day_{area_name}_{t0}-{t1}.nc"
+		target = os.path.join( opath , ofile )
+		if not os.path.isdir(opath):
+			os.makedirs(opath)
+		logger.info( f" * Save 'TMP/ERA5-AMIP/day/{cvarX}/{ofile}'" )
+		odatad.to_netcdf( os.path.join( opath , ofile ) )
+##}}}
+
 def build_EXTRA_cvars():##{{{
 	
 	cvars_cmp = cdsuParams.cvars_cmp
 	for cvar in cvars_cmp:
 		logger.info( f"Build EXTRA cvar '{cvar}'" )
 		
-		if cvar == "tasmin":
-			build_tasmin()
-		if cvar == "tasmax":
-			build_tasmax()
+		if cvar[-3:] == "min":
+			build_cvarmin( cvar[:-3] )
+		if cvar[-3:] == "max":
+			build_cvarmax( cvar[:-3] )
 		if cvar == "sfcWind":
 			build_sfcWind()
-		if cvar == "sfcWindmax":
-			build_sfcWindmax()
 		if cvar == "hurs":
 			build_hurs()
-		if cvar == "hursmax":
-			build_hursmax()
 		if cvar == "huss":
 			build_huss()
 		if cvar == "heatIndex":
 			build_heatIndex()
 	
 ##}}}
```

### Comparing `CDSupdate-1.1.0/CDSupdate/__init__.py` & `CDSupdate-1.2.1/CDSupdate/__init__.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.1.0/CDSupdate/__io.py` & `CDSupdate-1.2.1/CDSupdate/__io.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.1.0/CDSupdate/__release.py` & `CDSupdate-1.2.1/CDSupdate/__release.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 ## GNU General Public License for more details.
 ## 
 ## You should have received a copy of the GNU General Public License
 ## along with CDSupdate.  If not, see <https://www.gnu.org/licenses/>.
 
 
 version_major = "1"
-version_minor = "1"
-version_patch = "0"
+version_minor = "2"
+version_patch = "1"
 version_extra = ""
 version       = f"{version_major}.{version_minor}.{version_patch}{version_extra}"
 
 name = "CDSupdate"
 
 description = "Auto-updater of data from the Climate Data Store"
```

### Comparing `CDSupdate-1.1.0/CDSupdate/data/ERA5-dptas-description.txt` & `CDSupdate-1.2.1/CDSupdate/data/ERA5-dptas-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.1.0/CDSupdate/data/ERA5-name.csv` & `CDSupdate-1.2.1/CDSupdate/data/ERA5-name.csv`

 * *Files 20% similar despite different names*

```diff
@@ -10,10 +10,11 @@
 single,10,,vas,10m_v_component_of_wind,v10,northward_wind,Northward Near-Surface Wind,m.s-1,
 single,10,uas;vas,sfcWind,,,wind_speed,Near-Surface Wind Speed,m.s-1,
 single,10,sfcWind,sfcWindmax,,,wind_speed,Daily Max Near-Surface Wind Speed,m.s-1,
 single,2,tas;dptas,hurs,,,relative_humidity,Near-Surface Relative Humidity,%,
 single,2,hurs,hursmax,,,relative_humidity,Daily Max Near-Surface Relative Humidity,%,
 single,2,dptas;ps,huss,,,specific_humidity,Near-Surface Specific Humidity,kg.kg-1,
 single,2,tas;hurs,heatIndex,,,heat_index_of_air_temperature,Heat Index of Air Temperature,K,see Blazejczyk et al 2012 doi:10.1007/s00484-011-0453-2
+single,2,heatIndex,heatIndexmax,,,heat_index_of_air_temperature,Daily Max Heat Index of Air Temperature,K,see Blazejczyk et al 2012 doi:10.1007/s00484-011-0453-2
 pressure,,,zg,geopotential,z,geopotential_height,Geopotential Height at __CHANGE__hPa,m,Multiply by 9.80665 to find the geopotential
 single,0,,rsds,mean_surface_downward_short_wave_radiation_flux,msdwswrf,surface_downwelling_shortwave_flux_in_air,Surface Downwelling Shortwave Radiation,
 single,0,,rlds,mean_surface_downward_long_wave_radiation_flux,msdwlwrf,surface_downwelling_longwave_flux_in_air,Surface Downwelling Longwave Radiation,
```

### Comparing `CDSupdate-1.1.0/CDSupdate/data/ERA5-pr-description.txt` & `CDSupdate-1.2.1/CDSupdate/data/ERA5-pr-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.1.0/CDSupdate/data/ERA5-ps-description.txt` & `CDSupdate-1.2.1/CDSupdate/data/ERA5-ps-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.1.0/CDSupdate/data/ERA5-psl-description.txt` & `CDSupdate-1.2.1/CDSupdate/data/ERA5-psl-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.1.0/CDSupdate/data/ERA5-rlds-description.txt` & `CDSupdate-1.2.1/CDSupdate/data/ERA5-rlds-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.1.0/CDSupdate/data/ERA5-rsds-description.txt` & `CDSupdate-1.2.1/CDSupdate/data/ERA5-rsds-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.1.0/CDSupdate/data/ERA5-uas-description.txt` & `CDSupdate-1.2.1/CDSupdate/data/ERA5-uas-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.1.0/CDSupdate/data/ERA5-vas-description.txt` & `CDSupdate-1.2.1/CDSupdate/data/ERA5-vas-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.1.0/CDSupdate/data/ERA5-zg-description.txt` & `CDSupdate-1.2.1/CDSupdate/data/ERA5-zg-description.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.1.0/CDSupdate/data/__init__.py` & `CDSupdate-1.2.1/CDSupdate/data/__init__.py`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.1.0/CDSupdate.egg-info/PKG-INFO` & `CDSupdate-1.2.1/CDSupdate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CDSupdate
-Version: 1.1.0
+Version: 1.2.1
 Summary: Auto-updater of data from the Climate Data Store
 Home-page: https://github.com/yrobink/CDSupdate
 Author: Yoann Robin
 Author-email: yoann.robin.k@gmail.com
 License: GNU-GPL3
 Keywords: Climate Data Store,Auto update
 Platform: linux
```

### Comparing `CDSupdate-1.1.0/CDSupdate.egg-info/SOURCES.txt` & `CDSupdate-1.2.1/CDSupdate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.1.0/LICENSE` & `CDSupdate-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.1.0/PKG-INFO` & `CDSupdate-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CDSupdate
-Version: 1.1.0
+Version: 1.2.1
 Summary: Auto-updater of data from the Climate Data Store
 Home-page: https://github.com/yrobink/CDSupdate
 Author: Yoann Robin
 Author-email: yoann.robin.k@gmail.com
 License: GNU-GPL3
 Keywords: Climate Data Store,Auto update
 Platform: linux
```

### Comparing `CDSupdate-1.1.0/README.md` & `CDSupdate-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.1.0/scripts/cdsupdate` & `CDSupdate-1.2.1/scripts/cdsupdate`

 * *Files identical despite different names*

### Comparing `CDSupdate-1.1.0/setup.py` & `CDSupdate-1.2.1/setup.py`

 * *Files identical despite different names*

