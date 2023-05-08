# Comparing `tmp/lime-stable-0.9.8.tar.gz` & `tmp/lime-stable-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lime-stable-0.9.8.tar", last modified: Mon Nov  7 10:56:22 2022, max compression
+gzip compressed data, was "lime-stable-0.9.9.tar", last modified: Mon Nov 28 17:57:20 2022, max compression
```

## Comparing `lime-stable-0.9.8.tar` & `lime-stable-0.9.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2022-11-07 10:56:22.215336 lime-stable-0.9.8/
--rw-rw-rw-   0        0        0    36315 2022-03-04 21:17:46.000000 lime-stable-0.9.8/LICENSE.rst
--rw-rw-rw-   0        0        0      147 2022-07-17 04:44:42.000000 lime-stable-0.9.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1482 2022-11-07 10:56:22.215336 lime-stable-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0      994 2022-07-11 03:06:21.000000 lime-stable-0.9.8/README.rst
--rw-rw-rw-   0        0        0      455 2022-11-07 10:56:22.216338 lime-stable-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0     1412 2022-10-05 00:46:05.000000 lime-stable-0.9.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-07 10:56:22.197338 lime-stable-0.9.8/src/
-drwxrwxrwx   0        0        0        0 2022-11-07 10:56:22.209336 lime-stable-0.9.8/src/lime/
--rw-rw-rw-   0        0        0     1149 2022-11-04 13:46:58.000000 lime-stable-0.9.8/src/lime/__init__.py
--rw-rw-rw-   0        0        0      747 2022-07-17 02:39:00.000000 lime-stable-0.9.8/src/lime/config.py
--rw-rw-rw-   0        0        0    36298 2022-11-02 14:22:44.000000 lime-stable-0.9.8/src/lime/io.py
--rw-rw-rw-   0        0        0     3089 2022-10-05 00:46:06.000000 lime-stable-0.9.8/src/lime/logo.py
--rw-rw-rw-   0        0        0    44892 2022-11-07 09:40:59.000000 lime-stable-0.9.8/src/lime/model.py
--rw-rw-rw-   0        0        0    93273 2022-11-07 09:53:58.000000 lime-stable-0.9.8/src/lime/plots.py
--rw-rw-rw-   0        0        0    21548 2022-10-31 15:57:05.000000 lime-stable-0.9.8/src/lime/plots_interactive.py
--rw-rw-rw-   0        0        0    14462 2022-10-05 00:46:05.000000 lime-stable-0.9.8/src/lime/tables.py
--rw-rw-rw-   0        0        0    39896 2022-10-31 14:29:14.000000 lime-stable-0.9.8/src/lime/tools.py
--rw-rw-rw-   0        0        0    10788 2022-11-07 10:35:16.000000 lime-stable-0.9.8/src/lime/transitions.py
--rw-rw-rw-   0        0        0    48530 2022-11-04 13:48:06.000000 lime-stable-0.9.8/src/lime/treatment.py
--rw-rw-rw-   0        0        0    13288 2022-11-07 09:41:22.000000 lime-stable-0.9.8/src/lime/workflow.py
-drwxrwxrwx   0        0        0        0 2022-11-07 10:56:22.214339 lime-stable-0.9.8/src/lime_stable.egg-info/
--rw-rw-rw-   0        0        0     1482 2022-11-07 10:56:22.000000 lime-stable-0.9.8/src/lime_stable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2022-11-07 10:56:22.000000 lime-stable-0.9.8/src/lime_stable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-07 10:56:22.000000 lime-stable-0.9.8/src/lime_stable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2022-11-07 10:56:22.000000 lime-stable-0.9.8/src/lime_stable.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-11-07 10:56:22.000000 lime-stable-0.9.8/src/lime_stable.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-11-28 17:57:20.798108 lime-stable-0.9.9/
+-rw-rw-rw-   0        0        0    36315 2022-03-04 21:17:46.000000 lime-stable-0.9.9/LICENSE.rst
+-rw-rw-rw-   0        0        0      147 2022-07-17 04:44:42.000000 lime-stable-0.9.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1482 2022-11-28 17:57:20.798108 lime-stable-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2022-07-11 03:06:21.000000 lime-stable-0.9.9/README.rst
+-rw-rw-rw-   0        0        0      455 2022-11-28 17:57:20.799108 lime-stable-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     1412 2022-10-05 00:46:05.000000 lime-stable-0.9.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-11-28 17:57:20.774591 lime-stable-0.9.9/src/
+drwxrwxrwx   0        0        0        0 2022-11-28 17:57:20.792107 lime-stable-0.9.9/src/lime/
+-rw-rw-rw-   0        0        0     1238 2022-11-17 11:14:58.000000 lime-stable-0.9.9/src/lime/__init__.py
+-rw-rw-rw-   0        0        0      747 2022-07-17 02:39:00.000000 lime-stable-0.9.9/src/lime/config.py
+-rw-rw-rw-   0        0        0    37807 2022-11-25 12:20:53.000000 lime-stable-0.9.9/src/lime/io.py
+-rw-rw-rw-   0        0        0     3089 2022-10-05 00:46:06.000000 lime-stable-0.9.9/src/lime/logo.py
+-rw-rw-rw-   0        0        0    45336 2022-11-28 17:44:50.000000 lime-stable-0.9.9/src/lime/model.py
+-rw-rw-rw-   0        0        0   108081 2022-11-28 17:47:05.000000 lime-stable-0.9.9/src/lime/plots.py
+-rw-rw-rw-   0        0        0    36458 2022-11-28 15:52:59.000000 lime-stable-0.9.9/src/lime/plots_interactive.py
+-rw-rw-rw-   0        0        0    14462 2022-10-05 00:46:05.000000 lime-stable-0.9.9/src/lime/tables.py
+-rw-rw-rw-   0        0        0    40786 2022-11-28 16:17:14.000000 lime-stable-0.9.9/src/lime/tools.py
+-rw-rw-rw-   0        0        0    12743 2022-11-22 11:47:24.000000 lime-stable-0.9.9/src/lime/transitions.py
+-rw-rw-rw-   0        0        0    62016 2022-11-25 18:15:10.000000 lime-stable-0.9.9/src/lime/treatment.py
+-rw-rw-rw-   0        0        0    18414 2022-11-25 18:29:35.000000 lime-stable-0.9.9/src/lime/workflow.py
+drwxrwxrwx   0        0        0        0 2022-11-28 17:57:20.797109 lime-stable-0.9.9/src/lime_stable.egg-info/
+-rw-rw-rw-   0        0        0     1482 2022-11-28 17:57:20.000000 lime-stable-0.9.9/src/lime_stable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2022-11-28 17:57:20.000000 lime-stable-0.9.9/src/lime_stable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-28 17:57:20.000000 lime-stable-0.9.9/src/lime_stable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2022-11-28 17:57:20.000000 lime-stable-0.9.9/src/lime_stable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2022-11-28 17:57:20.000000 lime-stable-0.9.9/src/lime_stable.egg-info/top_level.txt
```

### Comparing `lime-stable-0.9.8/LICENSE.rst` & `lime-stable-0.9.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `lime-stable-0.9.8/PKG-INFO` & `lime-stable-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lime-stable
-Version: 0.9.8
+Version: 0.9.9
 Summary: Line measuring algorithm for ionized nebulae
 Home-page: https://github.com/Vital-Fernandez/lime
 Author: Vital Fernandez
 Author-email: vital.fernandez@userena.cl
 License: GNU
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lime-stable-0.9.8/README.rst` & `lime-stable-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `lime-stable-0.9.8/setup.py` & `lime-stable-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `lime-stable-0.9.8/src/lime/__init__.py` & `lime-stable-0.9.9/src/lime/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,12 +27,16 @@
 
 __version__ = _setup_cfg['metadata']['version']
 _lines_database_path = (os.path.join(_dir_path, '/resources/parent_mask.txt'))
 
 # Logging configuration
 _logger.debug(f'Launching LiMe {__version__} in Python {__python_version__}')
 
-from .treatment import Spectrum, Sample, CubeInspector
+
+class Error(Exception):
+    """LiMe exception function"""
+
+from .treatment import Spectrum, Sample, CubeInspector, Cube
 from .io import *
-from .tools import label_decomposition, LineFinder, spectral_mask_generator
+from .tools import label_decomposition, LineFinder, spectral_mask_generator, get_coord_entries
 from .plots import spatial_mask_generator
```

### Comparing `lime-stable-0.9.8/src/lime/config.py` & `lime-stable-0.9.9/src/lime/config.py`

 * *Files identical despite different names*

### Comparing `lime-stable-0.9.8/src/lime/io.py` & `lime-stable-0.9.9/src/lime/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
     'save_cfg',
     'load_cfg',
     'load_lines_log',
     'save_line_log',
     'log_parameters_calculation',
     'log_to_HDU',
     'save_param_maps',
-    'COORD_ENTRIES',
     '_LOG_DTYPES_REC',
     '_LOG_EXPORT',
     '_LOG_COLUMNS']
 
 import os
 import configparser
 import copy
@@ -22,14 +21,15 @@
 from sys import exit, stdout
 from pathlib import Path
 from distutils.util import strtobool
 from collections import Sequence
 
 from astropy.io import fits
 from astropy.table import Table
+from parso.python.tree import Class
 
 from .tables import table_fluxes
 
 try:
     import openpyxl
     openpyxl_check = True
 except ImportError:
@@ -61,27 +61,26 @@
 # Dictionary with the parameter dtypes
 _LOG_TYPES_DICT = dict(zip(_PARAMS_CONF_TABLE.index.values,
                            _PARAMS_CONF_TABLE.dtype.values))
 
 # Numpy recarray dtype for the pandas dataframe creation
 _LOG_DTYPES_REC = np.dtype(list(_LOG_TYPES_DICT.items()))
 
-# Variables with the astronomical coordinate information for the creation of new .fits files
-COORD_ENTRIES = ['CRPIX1', 'CRPIX2', 'CRVAL1', 'CRVAL2', 'CD1_1', 'CD1_2', 'CD2_1', 'CD2_2', 'CUNIT1', 'CUNIT2',
-                 'CTYPE1', 'CTYPE2']
-
 GLOBAL_LOCAL_GROUPS = ['line_fitting', 'chemical_model'] # TODO not implemented
 
 FLUX_TEX_TABLE_HEADERS = [r'$Transition$', '$EW(\AA)$', '$F(\lambda)$', '$I(\lambda)$']
 FLUX_TXT_TABLE_HEADERS = [r'$Transition$', 'EW', 'EW_error', 'F(lambda)', 'F(lambda)_error', 'I(lambda)', 'I(lambda)_error']
 
 KIN_TEX_TABLE_HEADERS = [r'$Transition$', r'$Comp$', r'$v_{r}\left(\nicefrac{km}{s}\right)$', r'$\sigma_{int}\left(\nicefrac{km}{s}\right)$', r'Flux $(\nicefrac{erg}{cm^{-2} s^{-1} \AA^{-1})}$']
 KIN_TXT_TABLE_HEADERS = [r'$Transition$', r'$Comp$', 'v_r', 'v_r_error', 'sigma_int', 'sigma_int_error', 'flux', 'flux_error']
 
 
+class LiMe_Error(Exception):
+    """LiMe exception function"""
+
 def load_lines_log(log_address, ext='LINESLOG'):
 
     """
     This function reads a lines log table as a pandas dataframe. The accepted input file types are a whitespace separated
     text file, a ``.fits`` file, a ``.asdf`` file and an excel file (``.xlsx``). In the case of ``.fits``, ``.asdf`` or
     ``.xlsx`` files the user should specify the target extension/sheet name (the default one is ``LINESLOG``).
 
@@ -167,104 +166,109 @@
     """
 
     # Confirm file path exits
     log_path = Path(log_address)
     assert log_path.parent.exists(), f'- ERROR: Output lines log folder not found ({log_path.parent})'
     file_name, file_type = log_path.name, log_path.suffix
 
-    # Slice the log if the user provides a list of columns
-    if parameters != 'all':
-        parameters_list = np.array(parameters, ndmin=1)
-        lines_log = log[parameters_list]
-        param_dtypes = [_LOG_DTYPES_REC[param] for param in parameters_list]
-
-    else:
-        lines_log = log
-        param_dtypes = list(_LOG_TYPES_DICT.values())
+    if len(log.index) > 0:
 
-    # Default txt log with the complete information
-    if file_type == '.txt':
-        with open(log_path, 'wb') as output_file:
-            string_DF = lines_log.to_string()
-            output_file.write(string_DF.encode('UTF-8'))
-
-    # Pdf fluxes table
-    elif file_type == '.pdf':
-
-        # Recover the fit components for merged lines from the log
-        if 'profile_label' in log.columns:
-            idcs_m = (log.index.str.contains('_m')) & (log.profile_label != 'no')
-            fit_conf = dict(zip(log.loc[idcs_m].index.values, log.loc[idcs_m].profile_label.values))
-        else:
-            fit_conf = {}
-        table_fluxes(lines_log, log_path.parent/log_path.stem, header_format_latex=_LOG_COLUMNS_LATEX,
-                     lines_notation=log.latex_label.values)
-
-    # Lines log in a fits file
-    elif file_type == '.fits':
-        if isinstance(lines_log, pd.DataFrame):
-            lineLogHDU = log_to_HDU(lines_log, ext_name=ext, header_dict=fits_header)
-
-            if log_path.is_file():
-                try:
-                    fits.update(log_path, data=lineLogHDU.data, header=lineLogHDU.header, extname=lineLogHDU.name, verify=True)
-                except KeyError:
-                    fits.append(log_path, data=lineLogHDU.data, header=lineLogHDU.header, extname=lineLogHDU.name)
+        # Slice the log if the user provides a list of columns
+        if parameters != 'all':
+            parameters_list = np.array(parameters, ndmin=1)
+            lines_log = log[parameters_list]
+            param_dtypes = [_LOG_DTYPES_REC[param] for param in parameters_list]
+
+        else:
+            lines_log = log
+            param_dtypes = list(_LOG_TYPES_DICT.values())
+
+        # Default txt log with the complete information
+        if file_type == '.txt':
+            with open(log_path, 'wb') as output_file:
+                string_DF = lines_log.to_string()
+                output_file.write(string_DF.encode('UTF-8'))
+
+        # Pdf fluxes table
+        elif file_type == '.pdf':
+
+            # Recover the fit components for merged lines from the log
+            if 'profile_label' in log.columns:
+                idcs_m = (log.index.str.contains('_m')) & (log.profile_label != 'no')
+                fit_conf = dict(zip(log.loc[idcs_m].index.values, log.loc[idcs_m].profile_label.values))
             else:
-                hdul = fits.HDUList([fits.PrimaryHDU(), lineLogHDU])
-                hdul.writeto(log_path, overwrite=True, output_verify='fix')
+                fit_conf = {}
+            table_fluxes(lines_log, log_path.parent/log_path.stem, header_format_latex=_LOG_COLUMNS_LATEX,
+                         lines_notation=log.latex_label.values)
+
+        # Lines log in a fits file
+        elif file_type == '.fits':
+            if isinstance(lines_log, pd.DataFrame):
+                lineLogHDU = log_to_HDU(lines_log, ext_name=ext, header_dict=fits_header)
+
+                if log_path.is_file():
+                    try:
+                        fits.update(log_path, data=lineLogHDU.data, header=lineLogHDU.header, extname=lineLogHDU.name, verify=True)
+                    except KeyError:
+                        fits.append(log_path, data=lineLogHDU.data, header=lineLogHDU.header, extname=lineLogHDU.name)
+                else:
+                    hdul = fits.HDUList([fits.PrimaryHDU(), lineLogHDU])
+                    hdul.writeto(log_path, overwrite=True, output_verify='fix')
 
-    # Default log in excel format
-    elif file_type == '.xlsx' or file_type == '.xls':
+        # Default log in excel format
+        elif file_type == '.xlsx' or file_type == '.xls':
 
-        # Check openpyxl is installed else leave
-        if openpyxl:
-            pass
-        else:
-            print(f'\n- WARNING: openpyxl is not installed. Lines log {log_address} could not be saved')
-            return
+            # Check openpyxl is installed else leave
+            if openpyxl:
+                pass
+            else:
+                print(f'\n- WARNING: openpyxl is not installed. Lines log {log_address} could not be saved')
+                return
 
-        if not log_path.is_file():
-            with pd.ExcelWriter(log_path) as writer:
-                lines_log.to_excel(writer, sheet_name=ext)
-        else:
-            # THIS WORKS IN WINDOWS BUT NOT IN LINUX
-            # with pd.ExcelWriter(log_path, mode="a", engine="openpyxl", if_sheet_exists="replace") as writer:
-            #     log.to_excel(writer, sheet_name=ext)
-
-            if file_type == '.xlsx':
-                book = openpyxl.load_workbook(log_path)
-                with pd.ExcelWriter(log_path, mode="a", engine="openpyxl", if_sheet_exists="replace") as writer:
-                    writer.book = book
-                    writer.sheets = dict((ws.title, ws) for ws in book.worksheets)
+            if not log_path.is_file():
+                with pd.ExcelWriter(log_path) as writer:
                     lines_log.to_excel(writer, sheet_name=ext)
             else:
-                # TODO this does not write to a xlsx file
-                with pd.ExcelWriter(log_path, mode="a", engine="openpyxl", if_sheet_exists="replace") as writer:
-                    lines_log.to_excel(writer, sheet_name=ext)
+                # THIS WORKS IN WINDOWS BUT NOT IN LINUX
+                # with pd.ExcelWriter(log_path, mode="a", engine="openpyxl", if_sheet_exists="replace") as writer:
+                #     log.to_excel(writer, sheet_name=ext)
+
+                if file_type == '.xlsx':
+                    book = openpyxl.load_workbook(log_path)
+                    with pd.ExcelWriter(log_path, mode="a", engine="openpyxl", if_sheet_exists="replace") as writer:
+                        writer.book = book
+                        writer.sheets = dict((ws.title, ws) for ws in book.worksheets)
+                        lines_log.to_excel(writer, sheet_name=ext)
+                else:
+                    # TODO this does not write to a xlsx file
+                    with pd.ExcelWriter(log_path, mode="a", engine="openpyxl", if_sheet_exists="replace") as writer:
+                        lines_log.to_excel(writer, sheet_name=ext)
 
-    # Advance Scientific Storage Format
-    elif file_type == '.asdf':
+        # Advance Scientific Storage Format
+        elif file_type == '.asdf':
+
+            tree = {ext: lines_log.to_records(index=True, column_dtypes=_LOG_TYPES_DICT, index_dtypes='<U50')}
 
-        tree = {ext: lines_log.to_records(index=True, column_dtypes=_LOG_TYPES_DICT, index_dtypes='<U50')}
+            # Create new file
+            if not log_path.is_file():
+                af = asdf.AsdfFile(tree)
+                af.write_to(log_path)
 
-        # Create new file
-        if not log_path.is_file():
-            af = asdf.AsdfFile(tree)
-            af.write_to(log_path)
+            # Update file
+            else:
+                with asdf.open(log_path, mode='rw') as af:
+                    af.tree.update(tree)
+                    af.update()
 
-        # Update file
         else:
-            with asdf.open(log_path, mode='rw') as af:
-                af.tree.update(tree)
-                af.update()
+            print(f"--WARNING: output extension {file_type} was not recognised in file {log_path}")
+            exit()
 
     else:
-        print(f"--WARNING: output extension {file_type} was not recognised in file {log_path}")
-        exit()
+        _logger.info('The output log has no measurements. An output file will not be saved')
 
     return
 
 
 _parent_bands_file = Path(__file__).parent/'resources/parent_mask.txt'
 _PARENT_BANDS = load_lines_log(_parent_bands_file)
 
@@ -614,14 +618,17 @@
     return linesHDU
 
 
 def load_fits(file_address, instrument, frame_idx=None):
 
     if instrument == 'ISIS':
 
+        if frame_idx is None:
+            frame_idx = 0
+
         # Open fits file
         with fits.open(file_address) as hdul:
             data, header = hdul[frame_idx].data, hdul[frame_idx].header
 
         assert 'ISIS' in header['INSTRUME'], 'Input spectrum instrument '
 
         # William Herschel Telescope ISIS instrument
@@ -957,7 +964,41 @@
         # Write to new file
         output_file = Path(output_folder)/f'{output_files_prefix}{param}.fits'
         paramHDUs.writeto(output_file, overwrite=True, output_verify='fix')
 
     return
 
 
+def load_spatial_masks(mask_file, mask_list=[]):
+
+    # Masks array container
+    spatial_mask_dict = {}
+
+    # Limit the analysis to some masks
+    mask_list_check = False if len(mask_list) == 0 else True
+
+    # Check that mask is there:
+    if mask_file is not None:
+
+        mask_file = Path(mask_file)
+
+        if mask_file.is_file():
+
+            with fits.open(mask_file) as maskHDULs:
+
+                # Save the fits data to restore later
+                counter = 0
+                for HDU in maskHDULs:
+                    ext_name = HDU.name
+                    if HDU.name != 'PRIMARY':
+                        if (ext_name in mask_list) or not mask_list_check:
+                            spatial_mask_dict[ext_name] = (HDU.data.astype('bool'), HDU.header)
+                            counter += 1
+
+                # Warn if the mask file does not contain any of the expected masks
+                if counter == 0:
+                    _logger.warning(f'No masks extensions were found in file {mask_file}')
+
+        else:
+            _logger.warning(f'No mask file was found at {mask_file.as_posix()}.')
+
+    return spatial_mask_dict
```

### Comparing `lime-stable-0.9.8/src/lime/logo.py` & `lime-stable-0.9.9/src/lime/logo.py`

 * *Files identical despite different names*

### Comparing `lime-stable-0.9.8/src/lime/model.py` & `lime-stable-0.9.9/src/lime/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 
 import matplotlib.pyplot as plt
 import numpy as np
 from lmfit.models import Model
+from lmfit import fit_report
 from scipy import stats, optimize
 from scipy.interpolate import interp1d
 from .tools import label_decomposition, compute_FWHM0
 from .transitions import label_components
 
 _logger = logging.getLogger('LiMe')
 
@@ -335,16 +336,18 @@
 
         # _fig, _ax = plt.subplots()
         # _ax.plot(emisWave, emisFlux)
         # plt.show()
 
         # Velocity calculations
         velocArray = c_KMpS * (emisWave[idx_0:idx_f] - self.peak_wave) / self.peak_wave
-        self.FWZI = velocArray[-1] - velocArray[0]
-        self.velocity_percentiles_calculations(velocArray, emisFlux[idx_0:idx_f], lineLinearCont[idx_0:idx_f])
+
+        if velocArray.size > 2:
+            self.FWZI = velocArray[-1] - velocArray[0]
+            self.velocity_percentiles_calculations(velocArray, emisFlux[idx_0:idx_f], lineLinearCont[idx_0:idx_f])
 
         # Pixel velocity # TODO we are not using this one
         self.pixel_vel = c_KMpS * self.pixelWidth/self.peak_wave
 
         # Equivalent width computation
         lineContinuumMatrix = lineLinearCont + normalNoise
         eqwMatrix = areasArray / lineContinuumMatrix.mean(axis=1)
@@ -698,14 +701,21 @@
         line.peak_wave = emis_wave[peakIdx]
         line.peak_flux = emis_flux[peakIdx]
         line.pixelWidth = np.diff(emis_wave).mean()
 
         line.cont = line.peak_wave * line.m_cont + line.n_cont
         line.std_cont = np.std(cont_flux - continuaFit)
 
+        # Warning if continuum above or below line peak/through
+        if line._emission_check and (lineLinearCont[peakIdx] > emis_flux[peakIdx]):
+            _logger.warning(f'Line {line.line} introduced as an emission but the line peak is below the continuum level')
+
+        if not line._emission_check and (lineLinearCont[peakIdx] > emis_flux[peakIdx]):
+            _logger.warning(f'Line {line.line} introduced as an absorption but the line peak is below the continuum level')
+
         # Establish the pixel sigma error
         err_array = line.std_cont if emis_err is None else emis_err
 
         # Monte Carlo to measure line flux and uncertainty
         normalNoise = np.random.normal(0.0, err_array, (n_steps, emis_flux.size))
         lineFluxMatrix = emis_flux + normalNoise
         areasArray = (lineFluxMatrix.sum(axis=1) - lineLinearCont.sum()) * line.pixelWidth
@@ -716,23 +726,15 @@
         line.snr_line = signal_to_noise(line.intg_flux, line.std_cont, emis_wave.size)
         line.snr_cont = line.cont/line.std_cont
 
         # Line width to the pixel below the continuum (or mask size if not happening)
         idx_0 = compute_FWHM0(peakIdx, emis_flux, -1, lineLinearCont, line._emission_check)
         idx_f = compute_FWHM0(peakIdx, emis_flux, 1, lineLinearCont, line._emission_check)
 
-        line.w_i = emis_wave[idx_0]
-        line.w_f = emis_wave[idx_f]
-
-        # Warning if continuum above or below line peak/through
-        if line._emission_check and (lineLinearCont[peakIdx] > emis_flux[peakIdx]):
-            _logger.warning(f'Line {line.line} introduced as an emission but the line peak is below the continuum level')
-
-        if not line._emission_check and (lineLinearCont[peakIdx] > emis_flux[peakIdx]):
-            _logger.warning(f'Line {line.line} introduced as an absorption but the line peak is below the continuum level')
+        line.w_i, line.w_f = emis_wave[idx_0], emis_wave[idx_f]
 
         # Velocity calculations
         velocArray = c_KMpS * (emis_wave[idx_0:idx_f] - line.peak_wave) / line.peak_wave
         self.velocity_profile_calc(line, velocArray, emis_flux[idx_0:idx_f], lineLinearCont[idx_0:idx_f])
 
         # Pixel velocity # TODO we are not using this one
         line.pixel_vel = c_KMpS * line.pixelWidth/line.peak_wave
@@ -758,21 +760,18 @@
         n_comps = len(self.line.list_comps)
 
         # # TODO maybe we need this operation just once and create self.ion, self.trans_array, self.latex_label
         # ion_arr, theoWave_arr, latexLabel_arr = label_decomposition(compList, user_conf, units_wave=units_wave)
 
         # Compute the line redshift and reference wavelength
         if line.blended_check:
-            ref_wave = line.wave * (1 + z_obj)
+            ref_wave = line.wavelength * (1 + z_obj)
         else:
             ref_wave = np.array([line.peak_wave], ndmin=1)
 
-        # Line redshift # TODO calculate z_line using the label reference
-        line.z_line = line.peak_wave/(ref_wave[0] * (1 + z_obj)) - 1
-
         # Continuum model
         fit_model = Model(linear_model)
         fit_model.prefix = f'line0_'
 
         if line._cont_from_adjacent:
             SLOPE_PAR = self._SLOPE_PAR
             INTER_PAR = self._INTER_PAR
@@ -879,14 +878,20 @@
             #     line.sigma_thermal[i] = np.sqrt(k_Boltzmann * temp / self._atomic_mass_dict[ion_arr[i][:-1]]) / 1000
             # except:
             #     line.sigma_thermal[i] = np.nan
 
             # Check parameters error progragation from the lmfit parameter
             review_err_propagation(line, i, comp)
 
+        # Calculate the line redshift
+        if line.blended_check:
+            line.z_line = line.center/line.wavelength - 1
+        else:
+            line.z_line = line.peak_wave/line.wavelength - 1
+
         # Recalculate the equivalent width with the gaussian fluxes if blended
         if line.blended_check:
             line.eqw = eqw_g
             line.eqw_err = eqwErr_g
 
         return
 
@@ -981,50 +986,56 @@
         # Assign the parameter configuration to the model
         model_obj.set_param_hint(param_ref, **param_conf)
 
         return
 
     def velocity_profile_calc(self, line, vel_array, line_flux, cont_flux, min_array_dim=15):
 
-        # Full width zero intensity
-        line.FWZI = vel_array[-1] - vel_array[0]
+        # In case the vel_array has length zero:
+        if vel_array.size > 2:
 
-        # Only compute the velocity percentiles for line bands with more than 15 pixels
-        valid_pixels = vel_array.size if not np.ma.is_masked(vel_array) else np.sum(~vel_array.mask)
+            # Full width zero intensity
+            line.FWZI = vel_array[-1] - vel_array[0]
 
-        if valid_pixels > min_array_dim:
+            # Only compute the velocity percentiles for line bands with more than 15 pixels
+            valid_pixels = vel_array.size if not np.ma.is_masked(vel_array) else np.sum(~vel_array.mask)
 
-            peakIdx = np.argmax(line_flux)
-            percentFluxArray = np.cumsum(line_flux-cont_flux) * line.pixelWidth / line.intg_flux * 100
+            if valid_pixels > min_array_dim:
 
-            if line._emission_check:
-                blue_range = line_flux[:peakIdx] > line.peak_flux/2
-                red_range = line_flux[peakIdx:] < line.peak_flux/2
-            else:
-                blue_range = line_flux[:peakIdx] < line.peak_flux/2
-                red_range = line_flux[peakIdx:] > line.peak_flux/2
+                peakIdx = np.argmax(line_flux)
+                percentFluxArray = np.cumsum(line_flux-cont_flux) * line.pixelWidth / line.intg_flux * 100
 
-            # In case the peak is at the edge
-            if (blue_range.size > 2) and (red_range.size > 2):
+                if line._emission_check:
+                    blue_range = line_flux[:peakIdx] > line.peak_flux/2
+                    red_range = line_flux[peakIdx:] < line.peak_flux/2
+                else:
+                    blue_range = line_flux[:peakIdx] < line.peak_flux/2
+                    red_range = line_flux[peakIdx:] > line.peak_flux/2
 
-                # Integrated FWHM
-                vel_FWHM_blue = vel_array[:peakIdx][np.argmax(blue_range)]
-                vel_FWHM_red = vel_array[peakIdx:][np.argmax(red_range)]
+                # In case the peak is at the edge
+                if (blue_range.size > 2) and (red_range.size > 2):
 
-                line.FWHM_intg = vel_FWHM_red - vel_FWHM_blue
+                    # Integrated FWHM
+                    vel_FWHM_blue = vel_array[:peakIdx][np.argmax(blue_range)]
+                    vel_FWHM_red = vel_array[peakIdx:][np.argmax(red_range)]
 
-                # Interpolation for integrated kinematics
-                percentInterp = interp1d(percentFluxArray, vel_array, kind='slinear', fill_value='extrapolate')
-                velocPercent = percentInterp(TARGET_PERCENTILES)
+                    line.FWHM_intg = vel_FWHM_red - vel_FWHM_blue
+
+                    # Interpolation for integrated kinematics
+                    percentInterp = interp1d(percentFluxArray, vel_array, kind='slinear', fill_value='extrapolate')
+                    velocPercent = percentInterp(TARGET_PERCENTILES)
+
+                    line.v_med, line.v_50 = np.median(vel_array), velocPercent[3] # TODO np.median ignores the mask
+                    line.v_5, line.v_10 = velocPercent[1], velocPercent[2]
+                    line.v_90, line.v_95 = velocPercent[4], velocPercent[5]
 
-                line.v_med, line.v_50 = np.median(vel_array), velocPercent[3] # TODO np.median ignores the mask
-                line.v_5, line.v_10 = velocPercent[1], velocPercent[2]
-                line.v_90, line.v_95 = velocPercent[4], velocPercent[5]
-
-                W_80 = line.v_90 - line.v_10
-                W_90 = line.v_95 - line.v_5
-
-                # This are not saved... should they
-                A_factor = ((line.v_90 - line.v_med) - (line.v_med-line.v_10)) / W_80
-                K_factor = W_90 / (1.397 * line.FWHM_intg)
+                    W_80 = line.v_90 - line.v_10
+                    W_90 = line.v_95 - line.v_5
 
-        return
+                    # This are not saved... should they
+                    A_factor = ((line.v_90 - line.v_med) - (line.v_med-line.v_10)) / W_80
+                    K_factor = W_90 / (1.397 * line.FWHM_intg)
+
+        else:
+            _logger.warning(f'{line.label} failure to measure the non-parametric FWHM')
+
+        return
```

### Comparing `lime-stable-0.9.8/src/lime/plots.py` & `lime-stable-0.9.9/src/lime/plots.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import logging
 import numpy as np
 
 from matplotlib import pyplot as plt, gridspec, patches, rc_context, cm, colors
-from matplotlib.widgets import SpanSelector, RadioButtons
 from astropy.wcs import WCS
 from astropy.io import fits
 
 import pandas as pd
 from pathlib import Path
 
 from .model import c_KMpS, gaussian_profiles_computation, linear_continuum_computation
-from .tools import label_decomposition, blended_label_from_log, ASTRO_UNITS_KEYS, UNITS_LATEX_DICT, latex_science_float
+from .tools import label_decomposition, blended_label_from_log, ASTRO_UNITS_KEYS, UNITS_LATEX_DICT, latex_science_float, PARAMETER_LATEX_DICT
 from .tools import define_masks, format_line_mask_option
-from .io import load_lines_log, save_line_log, _PARENT_BANDS
-from .transitions import  check_line_in_log
+from .io import load_lines_log, save_line_log, _PARENT_BANDS, load_spatial_masks
+from .transitions import check_line_in_log, Line
 
 _logger = logging.getLogger('LiMe')
 
+
 try:
     import mplcursors
     mplcursors_check = True
 except ImportError:
     mplcursors_check = False
 
 if mplcursors_check:
@@ -401,14 +401,26 @@
     else:
         idcs_mask = np.zeros(wave_obs.size).astype(bool)
         wave_plot, flux_plot = wave_obs, flux_obs
 
     return wave_plot, flux_plot, z_corr, idcs_mask
 
 
+def _mplcursor_parser(line_g_list, list_comps, log, norm_flux, units_wave, units_flux):
+
+    if mplcursors_check:
+        for i, line_g in enumerate(line_g_list):
+            line_label = list_comps[i]
+            latex_label = log.loc[line_label, 'latex_label']
+            label_complex = mplcursors_legend(line_label, log, latex_label, norm_flux, units_wave, units_flux)
+            mplcursors.cursor(line_g).connect("add", lambda sel, label=label_complex: sel.annotation.set_text(label))
+
+    return
+
+
 def maximize_center_fig(maximize_check=False, center_check=False):
 
     # mng = plt.get_current_fig_manager()
     # mng.resize(*mng.window.maxsize())
 
     if maximize_check:
 
@@ -462,38 +474,311 @@
 
 
 def check_line_for_bandplot(label, user_band, spec, log_ref=_PARENT_BANDS):
 
     # If no line provided, use the one from the last fitting
     if label is None:
         if spec.fit.line.label is not None:
-            label =spec.fit.line.label[:-2] if spec.fit.line.label.endswith('_b') else spec.fit.line.label # TODO replace .line with .label
+            label = spec.fit.line.label[:-2] if spec.fit.line.label.endswith('_b') else spec.fit.line.label # TODO replace .line with .label
             if label in spec.log.index:
                 band = spec.log.loc[label, 'w1':'w6'].values
             else:
                 _logger.warning(f'The line {label} is not found at the spectrum log')
 
     # The user provides a line and a band
     elif (label is not None) and (user_band is not None):
         band = user_band
 
     # The user only provides a label
     else:
         # The line has not been measured before (just plot the region)
+        if isinstance(label, str):
+            if label.endswith('_b'):
+                label = label[:-2]
+
         if label not in spec.log.index:
             label = check_line_in_log(label, log_ref)
             band = log_ref.loc[label, 'w1':'w6'].values
 
         # The line has been plotted before
         else:
             band = spec.log.loc[label, 'w1':'w6'].values
 
     return label, band
 
 
+def check_image_size(bg_image, fg_image, mask_dict):
+
+    # Confirm that the background and foreground images have the same size
+    if fg_image is not None:
+        if bg_image.shape != fg_image.shape:
+            _logger.warning(f'The cube background ({bg_image.shape}) image and foreground image ({fg_image.shape}) have'
+                            f' different size')
+
+    # Confirm that the background and mask images have the same size
+    for mask_name, mask_hdul in mask_dict.items():
+        mask_data, mask_hdr = mask_hdul
+        if bg_image.shape != mask_data.shape:
+            _logger.warning(f'The cube background ({bg_image.shape}) image and mask {mask_name} ({mask_data.shape}) have'
+                            f' different size')
+
+    return
+
+
+def determine_cube_images(cube, line, band, bands_frame, percentiles, color_scale, contours_check=False):
+
+    # Generate line object
+    if line is not None:
+
+        # Determine the line of reference
+        line = Line(line, band, ref_log=bands_frame)
+
+        # Compute the band map slice
+        idcsEmis, idcsCont = define_masks(cube.wave, line.mask * (1 + cube.redshift), line.pixel_mask)
+        image = cube.flux[idcsEmis, :, :].sum(axis=0)
+
+        # If no scale provided compute a default one
+        if color_scale is None:
+
+            levels = np.nanpercentile(image, np.array(percentiles, ndmin=1))
+
+            # For the background image (A minimum level)
+            if not contours_check:
+                color_scale = colors.SymLogNorm(linthresh=levels[0], vmin=levels[0], base=10)
+
+            # For the foreground
+            else:
+                color_scale = colors.LogNorm()
+
+    else:
+        line, image, levels, color_scale = None, None, None, None
+
+    return line, image, levels, color_scale
+
+
+def image_map_labels(title, wcs, line_bg, line_fg, masks_dict):
+
+    # Define the title
+    if title is None:
+        title = r'{} band'.format(line_bg.latex[0])
+        if line_fg is not None:
+            # title = f'{} with {} contours'.format(title, line_fg.latex[0])
+            title = f'{title} with {line_fg.latex[0]} contours'
+        if len(masks_dict) > 0:
+            title += f'\n and spatial masks'
+
+    # Generate the figure
+    if wcs is not None:
+        x_label, y_label = 'RA', 'DEC'
+    else:
+        x_label, y_label = 'x', 'y'
+
+    return title, x_label, y_label
+
+
+def image_plot(ax, image_bg, image_fg, fg_levels, fg_mesh, bg_scale, fg_scale, bg_color, fg_color, cursor_cords=None):
+
+    # Background image plot
+    im = ax.imshow(image_bg, cmap=bg_color, norm=bg_scale)
+
+    # Foreground contours
+    if image_fg is not None:
+        contours = ax.contour(fg_mesh[0], fg_mesh[1], image_fg, cmap=fg_color, levels=fg_levels, norm=fg_scale)
+    else:
+        contours = None
+
+    # Marker
+    if cursor_cords is not None:
+        marker, = ax.plot(cursor_cords[1], cursor_cords[0], '+', color='red')
+    else:
+        marker = None
+
+    return im, contours, marker
+
+
+def spatial_mask_plot(ax, masks_dict, mask_color, mask_alpha, units_flux, mask_list=[]):
+
+    # Container for the legends
+    legend_list = [None] * len(masks_dict)
+
+    cmap_contours = cm.get_cmap(mask_color, len(masks_dict))
+
+    for idx_mask, items in enumerate(masks_dict.items()):
+
+        mask_name, hdu_mask = items
+        mask_data, mask_header = hdu_mask
+
+        if (len(mask_list) == 0) or (mask_name in mask_list):
+
+            mask_param = mask_header['PARAM']
+            param_idx = mask_header['PARAMIDX']
+            param_val = mask_header['PARAMVAL']
+            n_spaxels = mask_header['NUMSPAXE']
+
+            # Inverse the mask array for the plot
+            inv_mask_array = np.ma.masked_array(mask_data, ~mask_data)
+
+            # Create the legend label
+            legend_i = f'{mask_name}, ' + PARAMETER_LATEX_DICT.get(mask_param, f'${mask_param}$')
+
+            # Add units if using the flux
+            if mask_param == units_flux:
+                units_text = r'{:latex}'.format(ASTRO_UNITS_KEYS[units_flux])
+                legend_i += r'$\left({}\right)$'.format(units_text[1:-1])
+
+            # Add percentile number
+            legend_i += r', $P_{{{}th}}$ = '.format(param_idx)
+
+            # Add percentile value and number voxels
+            legend_i += f'${latex_science_float(param_val, dec=3)}$ ({n_spaxels} voxels)'
+
+            cm_i = colors.ListedColormap([cmap_contours(idx_mask)])
+
+            legend_list[idx_mask] = patches.Patch(color=cmap_contours(idx_mask), label=legend_i)
+
+            ax.imshow(inv_mask_array, cmap=cm_i, vmin=0, vmax=1, alpha=mask_alpha)
+
+    return legend_list
+
+
+def spec_plot(ax, wave, flux, redshift, norm_flux, label='', rest_frame=False, log=None, include_fits=True,
+              units_wave='A', units_flux='Flam', log_scale=False, color_dict=colorDict):
+
+
+    # Reference frame for the plot
+    wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch_2(wave, flux, redshift, rest_frame)
+
+    # Plot the spectrum
+    ax.step(wave_plot / z_corr, flux_plot * z_corr, label=label, where='mid', color=color_dict['fg'])
+
+    # List of lines in the log
+    line_list = []
+    if log is not None:
+        if log.index.size > 0 and include_fits:
+            line_list = log.index.values
+
+            # Fitted continua and profiles
+            wave_array, gaussian_array = gaussian_profiles_computation(line_list, log, (1 + redshift))
+            wave_array, cont_array = linear_continuum_computation(line_list, log, (1 + redshift))
+
+
+            # Single component lines
+            line_g_list = _gaussian_line_profiler(ax, line_list, wave_array, gaussian_array, cont_array,
+                                                  z_corr, log, norm_flux)
+
+            # Add the interactive pop-ups
+            _mplcursor_parser(line_g_list, line_list, log, norm_flux, units_wave, units_flux)
+
+    # Plot the masked pixels
+    _masks_plot(ax, line_list, wave_plot, flux_plot, z_corr, log, idcs_mask)
+
+    return
+
+
+def _profile_plot(axis, x, y, label, idx_line=0, n_comps=1, observations_list='yes', color_dict=colorDict):
+
+    # Color and thickness
+    if observations_list == 'no':
+
+        # If only one component or combined
+        if n_comps == 1:
+            width_i, style, color = 1.5, '-', color_dict['profile']
+
+        # Component
+        else:
+            cmap = cm.get_cmap(color_dict['comps_map'])
+            width_i, style, color = 2, ':', cmap(idx_line/n_comps)
+
+    # Case where the line has an error
+    else:
+        width_i, style, color = 3, '-', 'red'
+
+    # Plot the profile
+    line_g = axis.plot(x, y, label=label, linewidth=width_i, linestyle=style, color=color)
+
+    return line_g
+
+
+def _gaussian_line_profiler(axis, line_list, wave_array, gaussian_array, cont_array, z_corr, log, norm_flux,
+                            color_dict=colorDict):
+
+    # Data for the plot
+    idcs_lines = log.index.isin(line_list)
+    observations = log.loc[idcs_lines].observations.values
+
+    # Plot them
+    line_g_list = [None] * len(line_list)
+    for i, line in enumerate(line_list):
+
+        # Check if blended or single/merged
+        idcs_comp = None
+        if (not line.endswith('_m')) and (log.loc[line, 'profile_label'] != 'no') and (len(line_list) > 1):
+            profile_comps = log.loc[line, 'profile_label'].split('-')
+            idx_line = profile_comps.index(line)
+            n_comps = len(profile_comps)
+            if profile_comps.index(line) == 0:
+                idcs_comp = (log['profile_label'] == log.loc[line, 'profile_label']).values
+        else:
+            idx_line = 0
+            n_comps = 1
+
+        # label for th elegend
+        latex_label = log.loc[line, 'latex_label']
+
+        # Get the corresponding axis
+        wave_i = wave_array[:, i]
+        cont_i = cont_array[:, i]
+        gauss_i = gaussian_array[:, i]
+
+        # Continuum (only one per line)
+        if idx_line == 0:
+            axis.plot(wave_i/z_corr, cont_i*z_corr/norm_flux, color=colorDict['cont'], label=None,
+                      linestyle='--', linewidth=0.5)
+
+        # Plot combined gaussian profile if blended
+        if idcs_comp is not None:
+            gauss_comb = gaussian_array[:, idcs_comp].sum(axis=1) + cont_i
+            _profile_plot(axis, wave_i/z_corr, gauss_comb*z_corr/norm_flux, None,
+                               idx_line=idx_line, n_comps=1, observations_list=observations[i], color_dict=color_dict)
+
+        # Gaussian component plot
+        line_g_list[i] = _profile_plot(axis, wave_i/z_corr, (gauss_i+cont_i)*z_corr/norm_flux, latex_label,
+                                       idx_line=idx_line, n_comps=n_comps, observations_list=observations[i],
+                                       color_dict=color_dict)
+
+    return line_g_list
+
+
+def _masks_plot(axis, line_list, x, y, z_corr, log, spectrum_mask, color_dict={}):
+
+    # Spectrum mask
+    if np.any(spectrum_mask):
+        x_mask = x[spectrum_mask]/z_corr
+        y_mask = y[spectrum_mask]*z_corr
+        if not np.all(np.isnan(y_mask)):
+            axis.scatter(x_mask, y_mask, marker='x', label='Masked pixels', color=color_dict['mask_marker'])
+
+    # Line masks
+    if log is not None:
+        if 'pixel_mask' in log.columns:
+            if line_list is not None:
+                for i, line in enumerate(line_list):
+                    if line in log.index:
+                        pixel_mask = log.loc[line, 'pixel_mask']
+                        if pixel_mask != 'no':
+                            line_mask_limits = format_line_mask_option(pixel_mask, x)
+                            idcsMask = (x[:, None] >= line_mask_limits[:, 0]) & (x[:, None] <= line_mask_limits[:, 1])
+                            idcsMask = idcsMask.sum(axis=1).astype(bool)
+                            if np.sum(idcsMask) >= 1:
+                                axis.scatter(x[idcsMask]/z_corr, y[idcsMask]*z_corr, marker="x",
+                                             color=color_dict['mask_marker'])
+
+    return
+
+
 class LiMePlots:
 
     def __init__(self, ):
 
         self._color_dict = colorDict
         self._legends_dict = {}
 
@@ -1213,18 +1498,16 @@
 
             # Band limits
             label = r'$16^{{th}}/{} - 84^{{th}}\cdot{}$ flux percentiles band'.format(threshold_factor, threshold_factor)
             ax.axhspan(low_lim, high_lim, alpha=0.2, label=label, color=self._color_dict['line_band'])
             ax.axhline(np.median(flux_plot[idcs_cont]), label='Median flux', linestyle=':', color='black')
 
             # Masked and rectected pixels
-            ax.scatter(wave_plot[~idcs_cont], flux_plot[~idcs_cont], label='Rejected pixels',
-                       color=self._color_dict['peak'], facecolor='none')
-            ax.scatter(wave_plot[idcs_mask], flux_plot[idcs_mask], marker='x', label='Masked pixels',
-                       color=self._color_dict['mask_marker'])
+            ax.scatter(wave_plot[~idcs_cont], flux_plot[~idcs_cont], label='Rejected pixels', color=self._color_dict['peak'], facecolor='none')
+            ax.scatter(wave_plot[idcs_mask], flux_plot[idcs_mask], marker='x', label='Masked pixels', color=self._color_dict['mask_marker'])
 
             # Output continuum
             ax.plot(wave_plot, continuum_fit, label='Continuum')
 
             ax.update(AXES_CONF)
             ax.legend()
             plt.tight_layout()
@@ -1260,16 +1543,14 @@
 
             if continuum is not None:
                 ax.plot(wave_plot, continuum, label='Continuum')
 
             ax.scatter(wave_plot[idcs_mask], flux_plot[idcs_mask], label='Masked pixels', marker='x',
                        color=self._color_dict['mask_marker'])
 
-
-
             ax.legend()
             ax.update(AXES_CONF)
             plt.tight_layout()
             plt.show()
 
         return
 
@@ -1373,209 +1654,38 @@
 
         peak_wave = log.loc[list_comps[0]].peak_wave/z_corr,
         peak_flux = log.loc[list_comps[0]].peak_flux*z_corr/norm_flux
         axis.scatter(peak_wave, peak_flux, facecolors=self._color_dict['peak'])
 
         return
 
-    def _profile_plot(self, axis, x, y, label, idx_line=0, n_comps=1, observations_list='yes'):
-
-        # Color and thickness
-        if observations_list == 'no':
-
-            # If only one component or combined
-            if n_comps == 1:
-                width_i, style, color = 2, '-', self._color_dict['profile']
-
-            # Component
-            else:
-                cmap = cm.get_cmap(self._color_dict['comps_map'])
-                width_i, style, color = 2, ':', cmap(idx_line/n_comps)
-
-        # Case where the line has an error
-        else:
-            width_i, style, color = 3, '-', 'red'
-
-        # Plot the profile
-        line_g = axis.plot(x, y, label=label, linewidth=width_i, linestyle=style, color=color)
-
-        return line_g
-
     def _cont_plot(self, axis, x, y, z_corr, norm_flux):
 
         # Plot the continuum,  Usine wavelength array and continuum form the first component
         # cont_wave = wave_array[:, 0]
         # cont_linear = cont_array[:, 0]
         axis.plot(x/z_corr, y*z_corr/norm_flux, color=self._color_dict['cont'], linestyle='--', linewidth=0.5)
 
         return
 
-    def _masks_plot(self, axis, line_list,  x, y, z_corr, log, spectrum_mask):
-
-        # Spectrum mask
-        if np.any(spectrum_mask):
-            axis.scatter(x[spectrum_mask]/z_corr, y[spectrum_mask]*z_corr, marker='x', label='Masked pixels',
-                         color=self._color_dict['mask_marker'])
-
-        # Line masks
-        if 'pixel_mask' in log.columns:
-            if line_list is not None:
-                for i, line in enumerate(line_list):
-                    if line in log.index:
-                        pixel_mask = log.loc[line, 'pixel_mask']
-                        if pixel_mask != 'no':
-                            line_mask_limits = format_line_mask_option(pixel_mask, x)
-                            idcsMask = (x[:, None] >= line_mask_limits[:, 0]) & (x[:, None] <= line_mask_limits[:, 1])
-                            idcsMask = idcsMask.sum(axis=1).astype(bool)
-                            if np.sum(idcsMask) >= 1:
-                                axis.scatter(x[idcsMask]/z_corr, y[idcsMask]*z_corr, marker="x",
-                                             color=self._color_dict['mask_marker'])
-
-        return
-
-    # def _auto_flux_scale(self, axis, y, y_scale):
-    #
-    #     if y_scale == 'auto':
-    #
-    #         # Limits for the axes
-    #         y_max, y_min = np.nanmax(y), np.nanmin(y)
-    #         cont, std = np.nanmedian(y), np.nanstd(y)
-    #         high_limit = y_max + 2 * std
-    #         low_limit = y_min if (y_min - std < 0) and (y_min > 0) else y_min - 2 * std
-    #         # axis.set_ylim(ymin=low_limit, ymax=high_limit)
-    #
-    #         # Scale for the y axis
-    #         if y_scale == 'auto':
-    #
-    #             if np.all(y > 1e-10) and (high_limit > 10 * y.mean()):
-    #                 axis.set_yscale('log')
-    #             else:
-    #                 axis.set_yscale('linear')
-    #         else:
-    #             axis.set_yscale(y_scale)
-    #
-    #     else:
-    #         axis.set_yscale(y_scale)
-    #
-    #     return
-
 
-class LimeFigures(Plotter):
+class SpectrumFigures(Plotter):
 
     def __init__(self, spectrum):
 
         # Instantiate the dependencies
         Plotter.__init__(self)
 
         # Lime spectrum object with the scientific data
         self._spec = spectrum
 
         # Container for the matplotlib figures
         self._fig, self._ax = None, None
 
-    def line(self, line=None, band=None, include_fits=True, rest_frame=False, y_scale='auto', trans_line=False, in_fig=None, in_axis=None,
-             plt_cfg={}, ax_cfg={}, output_address=None):
-
-        # Establish the line and band to user for the analysis
-        line, band = check_line_for_bandplot(line, band, self._spec, _PARENT_BANDS)
-
-        # Guess whether we need both lines
-        include_fits = include_fits and (line in self._spec.log.index)
-
-        # Adjust the default theme
-        plt_cfg.setdefault('axes.labelsize', 14)
-        PLT_CONF, AXES_CONF = self._figure_format(plt_cfg, ax_cfg, self._spec.norm_flux, self._spec.units_wave,
-                                                  self._spec.units_flux)
-
-        # Create and fill the figure
-        with rc_context(PLT_CONF):
-
-            # Generate the figure object and figures
-            if include_fits:
-                gs = gridspec.GridSpec(2, 1, height_ratios=[3, 1])
-                spec_ax = plt.subplot(gs[0])
-                resid_ax = plt.subplot(gs[1], sharex=spec_ax)
-                fig, ax = None, (spec_ax, resid_ax)
-            else:
-                fig, ax = plt.subplots()
-                ax = [ax]
-
-            self._fig, self._ax = fig, ax
-            self._ax[0].set(**AXES_CONF)
-
-            # self._fig, self._ax = self._plot_container(in_fig, in_axis, AXES_CONF, gfit_type=include_fits)
-            # self._ax[0].set(**AXES_CONF)
-
-            # Reference _frame for the plot
-            wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch_2(self._spec.wave, self._spec.flux,
-                                                                          self._spec.redshift, rest_frame)
-            err_plot = self._spec.err_flux
-
-            # Establish the limits for the line spectrum plot
-            mask = band * (1 + self._spec.redshift)
-            idcsM = np.searchsorted(wave_plot, mask)
-
-            # Plot the spectrum
-            label = '' if include_fits else line
-            self._ax[0].step(wave_plot[idcsM[0]:idcsM[5]] / z_corr, flux_plot[idcsM[0]:idcsM[5]] * z_corr,
-                             where='mid', color=self._color_dict['fg'], label=label)
-
-            # Add the fitting results
-            if include_fits:
-
-                # Check components
-                blended_check, profile_label = blended_label_from_log(line, self._spec.log)
-                list_comps = profile_label.split('-') if blended_check else [line]
-
-                wave_array, gaussian_array = gaussian_profiles_computation(list_comps, self._spec.log, (1 + self._spec.redshift))
-                wave_array, cont_array = linear_continuum_computation(list_comps, self._spec.log, (1 + self._spec.redshift))
-
-                # Continuum bands
-                self._bands_plot(self._ax[0], wave_plot, flux_plot, z_corr, idcsM, line)
-
-                # Gaussian profiles
-                idcs_lines = self._spec.log.index.isin(list_comps)
-                line_g_list = self._gaussian_line_profiler(self._ax[0], list_comps, wave_array, gaussian_array, cont_array,
-                                                           z_corr, self._spec.log.loc[idcs_lines], self._spec.norm_flux)
-
-                # Add the interactive text
-                self._mplcursor_parser(line_g_list, list_comps, self._spec.log, self._spec.norm_flux, self._spec.units_wave,
-                                       self._spec.units_flux)
-
-                # Residual flux component
-                err_region = None if err_plot is None else err_plot[idcsM[0]:idcsM[5]]
-                self._residual_line_plotter(self._ax[1], wave_plot[idcsM[0]:idcsM[5]], flux_plot[idcsM[0]:idcsM[5]],
-                                            err_region, list_comps, z_corr, self._spec.log, self._spec.norm_flux,
-                                            self._spec.redshift, idcs_mask)
-
-                # Synchronizing the x-axis
-                self._ax[1].set_xlim(self._ax[0].get_xlim())
-                self._ax[1].set_xlabel(AXES_CONF['xlabel'])
-                self._ax[0].set_xlabel(None)
-
-            # Plot the masked pixels
-            self._masks_plot(self._ax[0], [line], wave_plot[idcsM[0]:idcsM[5]], flux_plot[idcsM[0]:idcsM[5]], z_corr,
-                             self._spec.log, idcs_mask[idcsM[0]:idcsM[5]])
-
-            # Line location
-            if trans_line:
-                wave = 3426
-                self._ax[0].axvline(wave, linestyle='--', alpha=0.5,
-                                    color=self._color_dict['fg'])
-
-            # Display the legend
-            self._ax[0].legend()
-
-            # Set the scale
-            _auto_flux_scale(self._ax[0], y=flux_plot[idcsM[0]:idcsM[5]] * z_corr, y_scale=y_scale)
-
-            # By default, plot on screen unless an output address is provided
-            save_close_fig_swicth(output_address, 'tight', fig_obj=None)
-
-            return
+        return
 
     def spectrum(self, extra_comp=None, line_bands=None, label=None, noise_region=None, log_scale=False,
                  output_address=None, rest_frame=False, include_fits=False, in_fig=None, in_axis=None, plt_cfg={}, ax_cfg={},
                  maximize=False):
 
         """
 
@@ -1676,24 +1786,25 @@
 
                 if line_list.size > 0:
 
                     wave_array, gaussian_array = gaussian_profiles_computation(line_list, self._spec.log, (1 + self._spec.redshift))
                     wave_array, cont_array = linear_continuum_computation(line_list, self._spec.log, (1 + self._spec.redshift))
 
                     # Single component lines
-                    line_g_list = self._gaussian_line_profiler(self._ax, line_list,
+                    line_g_list = _gaussian_line_profiler(self._ax, line_list,
                                                                wave_array, gaussian_array, cont_array,
-                                                               z_corr, self._spec.log, self._spec.norm_flux)
+                                                               z_corr, self._spec.log, self._spec.norm_flux,
+                                                               color_dict=self._color_dict)
 
                     # Add the interactive pop-ups
-                    self._mplcursor_parser(line_g_list, line_list, self._spec.log, self._spec.norm_flux,
+                    _mplcursor_parser(line_g_list, line_list, self._spec.log, self._spec.norm_flux,
                                            self._spec.units_wave, self._spec.units_flux)
 
             # Plot the masked pixels
-            self._masks_plot(self._ax, line_list, wave_plot, flux_plot, z_corr, self._spec.log, idcs_mask)
+            _masks_plot(self._ax, line_list, wave_plot, flux_plot, z_corr, self._spec.log, idcs_mask)
 
             # Switch y_axis to logarithmic scale if requested
             if log_scale:
                 self._ax.set_yscale('log')
 
             # Add or remove legend according to the plot type:
             if legend_check:
@@ -1767,32 +1878,33 @@
                         self._ax[i].step(wave_plot[idxL:idxH] / z_corr, flux_plot[idxL:idxH] * z_corr, where='mid',
                                         color=self._color_dict['fg'])
 
                         # Continuum bands
                         self._bands_plot(self._ax[i], wave_plot, flux_plot, z_corr, idcsM, line_i)
 
                         # Plot the masked pixels
-                        self._masks_plot(self._ax[i], [line_i], wave_plot[idxL:idxH], flux_plot[idxL:idxH], z_corr, log,
+                        _masks_plot(self._ax[i], [line_i], wave_plot[idxL:idxH], flux_plot[idxL:idxH], z_corr, log,
                                          idcs_mask[idxL:idxH])
 
                         # Plot the fitting results
                         if include_fits:
 
                             wave_array, gaussian_array = gaussian_profiles_computation([line_i], self._spec.log,
                                                                                        (1 + self._spec.redshift))
                             wave_array, cont_array = linear_continuum_computation([line_i], self._spec.log,
                                                                                   (1 + self._spec.redshift))
 
                             # Single component lines
-                            line_g_list = self._gaussian_line_profiler(self._ax[i], [line_i],
+                            line_g_list = _gaussian_line_profiler(self._ax[i], [line_i],
                                                                        wave_array, gaussian_array, cont_array,
-                                                                       z_corr, self._spec.log, self._spec.norm_flux)
+                                                                       z_corr, self._spec.log, self._spec.norm_flux,
+                                                                       color_dict=self._color_dict)
 
                             # Add the interactive pop-ups
-                            self._mplcursor_parser(line_g_list, [line_i], self._spec.log, self._spec.norm_flux,
+                            _mplcursor_parser(line_g_list, [line_i], self._spec.log, self._spec.norm_flux,
                                                    self._spec.units_wave, self._spec.units_flux)
 
                         # Formatting the figure
                         self._ax[i].yaxis.set_major_locator(plt.NullLocator())
                         self._ax[i].xaxis.set_major_locator(plt.NullLocator())
 
                         self._ax[i].update({'title': log.loc[line_i, 'latex_label']})
@@ -1809,60 +1921,229 @@
                 save_close_fig_swicth(output_address, 'tight', self._fig, maximize=maximize)
 
         else:
             _logger.info('The bands log does not contain lines')
 
         return
 
-    def _gaussian_line_profiler(self, axis, line_list, wave_array, gaussian_array, cont_array, z_corr, log, norm_flux):
+    def line(self, line=None, band=None, include_fits=True, rest_frame=False, y_scale='auto', trans_line=False,
+             in_fig=None, in_axis=None, plt_cfg={}, ax_cfg={}, output_address=None):
+
+        # Establish the line and band to user for the analysis
+        line, band = check_line_for_bandplot(line, band, self._spec, _PARENT_BANDS)
+
+        # Guess whether we need both lines
+        include_fits = include_fits and (line in self._spec.log.index)
 
-        # Data for the plot
-        idcs_lines = log.index.isin(line_list)
-        observations = log.loc[idcs_lines].observations.values
-
-        # Plot them
-        line_g_list = [None] * len(line_list)
-        for i, line in enumerate(line_list):
-
-            # Check if blended or single/merged
-            idcs_comp = None
-            if (not line.endswith('_m')) and (log.loc[line, 'profile_label'] != 'no') and (len(line_list) > 1):
-                profile_comps = log.loc[line, 'profile_label'].split('-')
-                idx_line = profile_comps.index(line)
-                n_comps = len(profile_comps)
-                if profile_comps.index(line) == 0:
-                    idcs_comp = (log['profile_label'] == log.loc[line, 'profile_label']).values
+        # Adjust the default theme
+        plt_cfg.setdefault('axes.labelsize', 14)
+        PLT_CONF, AXES_CONF = self._figure_format(plt_cfg, ax_cfg, self._spec.norm_flux, self._spec.units_wave,
+                                                  self._spec.units_flux)
+
+        # Create and fill the figure
+        with rc_context(PLT_CONF):
+
+            # Generate the figure object and figures
+            if include_fits:
+                gs = gridspec.GridSpec(2, 1, height_ratios=[3, 1])
+                spec_ax = plt.subplot(gs[0])
+                resid_ax = plt.subplot(gs[1], sharex=spec_ax)
+                fig, ax = None, (spec_ax, resid_ax)
             else:
-                idx_line = 0
-                n_comps = 1
+                fig, ax = plt.subplots()
+                ax = [ax]
+
+            self._fig, self._ax = fig, ax
+            self._ax[0].set(**AXES_CONF)
+
+            # self._fig, self._ax = self._plot_container(in_fig, in_axis, AXES_CONF, gfit_type=include_fits)
+            # self._ax[0].set(**AXES_CONF)
+
+            # Reference _frame for the plot
+            wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch_2(self._spec.wave, self._spec.flux,
+                                                                          self._spec.redshift, rest_frame)
+            err_plot = self._spec.err_flux
+
+            # Establish the limits for the line spectrum plot
+            mask = band * (1 + self._spec.redshift)
+            idcsM = np.searchsorted(wave_plot, mask)
+
+            # Plot the spectrum
+            label = '' if include_fits else line
+            self._ax[0].step(wave_plot[idcsM[0]:idcsM[5]] / z_corr, flux_plot[idcsM[0]:idcsM[5]] * z_corr,
+                             where='mid', color=self._color_dict['fg'], label=label)
+
+            # Add the fitting results
+            if include_fits:
+
+                # Check components
+                blended_check, profile_label = blended_label_from_log(line, self._spec.log)
+                list_comps = profile_label.split('-') if blended_check else [line]
+
+                wave_array, gaussian_array = gaussian_profiles_computation(list_comps, self._spec.log, (1 + self._spec.redshift))
+                wave_array, cont_array = linear_continuum_computation(list_comps, self._spec.log, (1 + self._spec.redshift))
 
-            # label for th elegend
-            latex_label = log.loc[line, 'latex_label']
+                # Continuum bands
+                self._bands_plot(self._ax[0], wave_plot, flux_plot, z_corr, idcsM, line)
 
-            # Get the corresponding axis
-            wave_i = wave_array[:, i]
-            cont_i = cont_array[:, i]
-            gauss_i = gaussian_array[:, i]
-
-            # Continuum (only one per line)
-            if idx_line == 0:
-                axis.plot(wave_i/z_corr, cont_i*z_corr/norm_flux, color=self._color_dict['cont'], label=None,
-                          linestyle='--', linewidth=0.5)
-
-            # Plot combined gaussian profile if blended
-            if idcs_comp is not None:
-                gauss_comb = gaussian_array[:, idcs_comp].sum(axis=1) + cont_i
-                self._profile_plot(axis, wave_i/z_corr, gauss_comb*z_corr/norm_flux, None,
-                                   idx_line=idx_line, n_comps=1, observations_list=observations[i])
-
-            # Gaussian component plot
-            line_g_list[i] = self._profile_plot(axis, wave_i/z_corr, (gauss_i+cont_i)*z_corr/norm_flux, latex_label,
-                                                idx_line=idx_line, n_comps=n_comps, observations_list=observations[i])
+                # Gaussian profiles
+                idcs_lines = self._spec.log.index.isin(list_comps)
+                line_g_list = _gaussian_line_profiler(self._ax[0], list_comps, wave_array, gaussian_array, cont_array,
+                                                           z_corr, self._spec.log.loc[idcs_lines], self._spec.norm_flux,
+                                                           color_dict=self._color_dict)
 
-        return line_g_list
+                # Add the interactive text
+                _mplcursor_parser(line_g_list, list_comps, self._spec.log, self._spec.norm_flux, self._spec.units_wave,
+                                       self._spec.units_flux)
+
+                # Residual flux component
+                err_region = None if err_plot is None else err_plot[idcsM[0]:idcsM[5]]
+                self._residual_line_plotter(self._ax[1], wave_plot[idcsM[0]:idcsM[5]], flux_plot[idcsM[0]:idcsM[5]],
+                                            err_region, list_comps, z_corr, self._spec.log, self._spec.norm_flux,
+                                            self._spec.redshift, idcs_mask[idcsM[0]:idcsM[5]])
+
+                # Synchronizing the x-axis
+                self._ax[1].set_xlim(self._ax[0].get_xlim())
+                self._ax[1].set_xlabel(AXES_CONF['xlabel'])
+                self._ax[0].set_xlabel(None)
+
+            # Plot the masked pixels
+            _masks_plot(self._ax[0], [line], wave_plot[idcsM[0]:idcsM[5]], flux_plot[idcsM[0]:idcsM[5]], z_corr,
+                             self._spec.log, idcs_mask[idcsM[0]:idcsM[5]])
+
+            # Line location
+            if trans_line:
+                self._ax[0].axvline(line.wavelength, linestyle='--', alpha=0.5,
+                                    color=self._color_dict['fg'])
+
+            # Display the legend
+            self._ax[0].legend()
+
+            # Set the scale
+            _auto_flux_scale(self._ax[0], y=flux_plot[idcsM[0]:idcsM[5]] * z_corr, y_scale=y_scale)
+
+            # By default, plot on screen unless an output address is provided
+            save_close_fig_swicth(output_address, 'tight', fig_obj=None)
+
+            return
+
+    def velocity_profile(self,  line=None, band=None, y_scale='auto', plt_cfg={}, ax_cfg={}, in_fig=None,
+                         output_address=None):
+
+        # Establish the line and band to user for the analysis
+        line, band = check_line_for_bandplot(line, band, self._spec, _PARENT_BANDS)
+
+        # Adjust the default theme
+        ax_cfg.setdefault('xlabel',  'Velocity (Km/s)')
+        PLT_CONF, AXES_CONF = self._figure_format(plt_cfg, ax_cfg, self._spec.norm_flux, self._spec.units_wave,
+                                                  self._spec.units_flux)
+
+        # Recover the line data
+        line = Line.from_log(line, self._spec.log, self._spec.norm_flux)
+
+        # Line spectrum
+        wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch_2(self._spec.wave, self._spec.flux,
+                                                                      self._spec.redshift, False)
+
+        # Establish the limits for the line spectrum plot
+        mask = band * (1 + self._spec.redshift)
+        idcsM = np.searchsorted(wave_plot, mask)
+
+        # Velocity spectrum for the line region
+        flux_plot = flux_plot[idcsM[0]:idcsM[5]]
+        cont_plot = line.m_cont * wave_plot[idcsM[0]:idcsM[5]] + line.n_cont
+        vel_plot = c_KMpS * (wave_plot[idcsM[0]:idcsM[5]] - line.peak_wave) / line.peak_wave
+
+        # Line edges
+        w_limits = np.array([line.w_i, line.w_f])
+        v_i, v_f = c_KMpS * (w_limits - line.peak_wave) / line.peak_wave
+        idx_i, idx_f = np.searchsorted(wave_plot[idcsM[0]:idcsM[5]], w_limits)
+
+        # Create and fill the figure
+        with rc_context(PLT_CONF):
+
+            # Figure and its axis
+            if in_fig is None:
+                self._fig, self._ax = plt.subplots()
+            else:
+                self._fig = in_fig
+                self._ax = self.fig.add_subplot()
+
+            self._ax.set(**AXES_CONF)
+            trans = self._ax.get_xaxis_transform()
+
+            # Plot the spectrum
+            self._ax.step(vel_plot, flux_plot, label=line.latex_label, where='mid', color=self._color_dict['fg'])
+
+            # Velocity percentiles
+            target_percen = ['v_5', 'v_10', 'v_50', 'v_90', 'v_95']
+            for i_percentil, percentil in enumerate(target_percen):
+
+                vel_per = line.__getattribute__(percentil)
+                label_text = None if i_percentil > 0 else r'$v_{Pth}$'
+                self._ax.axvline(x=vel_per, label=label_text, color=self._color_dict['fg'], linestyle='dotted', alpha=0.5)
+
+                label_plot = r'$v_{{{}}}$'.format(percentil[2:])
+                self._ax.text(vel_per, 0.80, label_plot, ha='center', va='center', rotation='vertical',
+                              backgroundcolor=self._color_dict['bg'], transform=trans, alpha=0.5)
+
+            # Velocity edges
+            label_v_i, label_v_f = r'$v_{{0}}$', r'$v_{{100}}$'
+            self._ax.axvline(x=v_i, alpha=0.5, color=self._color_dict['fg'], linestyle='dotted')
+            self._ax.text(v_i, 0.50, label_v_i, ha='center', va='center', rotation='vertical',
+                          backgroundcolor=self._color_dict['bg'], transform=trans, alpha=0.5)
+
+            self._ax.axvline(x=v_f, alpha=0.5, color=self._color_dict['fg'], linestyle='dotted')
+            self._ax.text(v_f, 0.50, label_v_f, ha='center', va='center', rotation='vertical',
+                          backgroundcolor=self._color_dict['bg'], transform=trans, alpha=0.5)
+
+            # Plot the line profile
+            self._ax.plot(vel_plot, cont_plot, linestyle='--', color=self._color_dict['fg'])
+
+            # Plot velocity bands
+            w80 = line.v_90-line.v_10
+            label_arrow = r'$w_{{80}}={:0.1f}\,Km/s$'.format(w80)
+            p1 = patches.FancyArrowPatch((line.v_10, 0.4),
+                                         (line.v_90, 0.4),
+                                         label=label_arrow,
+                                         arrowstyle='<->',
+                                         color='tab:blue',
+                                         transform=trans,
+                                         mutation_scale=20)
+            self._ax.add_patch(p1)
+
+            # Plot FWHM bands
+            label_arrow = r'$FWZI={:0.1f}\,Km/s$'.format(line.FWZI)
+            p2 = patches.FancyArrowPatch((vel_plot[idx_i], cont_plot[idx_i]),
+                                         (vel_plot[idx_f], cont_plot[idx_f]),
+                                         label=label_arrow,
+                                         arrowstyle='<->',
+                                         color='tab:red',
+                                         transform=self._ax.transData,
+                                         mutation_scale=20)
+            self._ax.add_patch(p2)
+
+            # Median velocity
+            label_vmed = r'$v_{{med}}={:0.1f}\,Km/s$'.format(line.v_med)
+            self._ax.axvline(x=line.v_med, color=self._color_dict['fg'], label=label_vmed, linestyle='dashed', alpha=0.5)
+
+            # Peak velocity
+            label_vmed = r'$v_{{peak}}$'
+            self._ax.axvline(x=0.0, color=self._color_dict['fg'], label=label_vmed, alpha=0.5)
+
+            # Set the scale
+            _auto_flux_scale(self._ax, y=flux_plot, y_scale=y_scale)
+
+            # Legend
+            self._ax.legend()
+
+            # By default, plot on screen unless an output address is provided
+            save_close_fig_swicth(output_address, 'tight', fig_obj=None)
+
+        return
 
     def _residual_line_plotter(self, axis, x, y, err, list_comps, z_corr, log, norm_flux, redshift, spec_mask):
 
         # Continuum level
         cont_level = self._spec.log.loc[list_comps[0], 'cont']
         cont_std = self._spec.log.loc[list_comps[0], 'std_cont']
 
@@ -1897,26 +2178,105 @@
             _logger.warning(f'Nan or inf entries in axis limit for {self.line}')
 
         # Residual plot labeling
         axis.legend(loc='upper left')
         axis.set_ylabel(label_residual, fontsize=22)
 
         # Spectrum mask
-        self._masks_plot(self._ax[0], [list_comps[0]], x, y, z_corr, log, spec_mask)
+        _masks_plot(self._ax[0], [list_comps[0]], x, y, z_corr, log, spec_mask)
 
         return
 
-    def _mplcursor_parser(self, line_g_list, list_comps, log, norm_flux, units_wave, units_flux):
 
-        if mplcursors_check:
-            for i, line_g in enumerate(line_g_list):
-                line_label = list_comps[i]
-                latex_label = log.loc[line_label, 'latex_label']
-                label_complex = mplcursors_legend(line_label, log, latex_label, norm_flux, units_wave, units_flux)
-                mplcursors.cursor(line_g).connect("add", lambda sel, label=label_complex: sel.annotation.set_text(label))
+class CubeFigures(Plotter):
+
+    def __init__(self, cube):
+
+        # Instantiate the dependencies
+        Plotter.__init__(self)
+
+        # Lime spectrum object with the scientific data
+        self._cube = cube
+
+        # Container for the matplotlib figures
+        self._fig, self._ax = None, None
+
+        self.param_conv = {'SN_line': r'$\frac{S}{N}_{line}$',
+                           'SN_cont': r'$\frac{S}{N}_{cont}$',
+                           self._cube.units_flux: None}
+
+        return
+
+    def cube(self, line, band=None, percentil_bg=60, line_fg=None, band_fg=None, percentils_fg=[90, 95, 99], bands_frame=None,
+             bg_scale=None, fg_scale=None, bg_color='gray', fg_color='viridis', mask_color='viridis_r', mask_alpha=0.2,
+             wcs=None, plt_cfg={}, ax_cfg={}, in_fig=None, in_ax=None, title=None, masks_file=None, output_address=None,
+             maximise=False):
+
+
+        # Prepare the background image data
+        line_bg, bg_image, bg_levels, bg_scale = determine_cube_images(self._cube, line, band, bands_frame,
+                                                                       percentil_bg, bg_scale, contours_check=False)
+
+        # Prepare the foreground image data
+        line_fg, fg_image, fg_levels, fg_scale = determine_cube_images(self._cube, line_fg, band_fg, bands_frame,
+                                                                       percentils_fg, fg_scale, contours_check=True)
+
+        # Mesh for the countours
+        if line_fg is not None:
+            y, x = np.arange(0, fg_image.shape[0]), np.arange(0, fg_image.shape[1])
+            fg_mesh = np.meshgrid(x, y)
+        else:
+            fg_mesh = None
+
+        # Load the masks
+        masks_dict = load_spatial_masks(masks_file)
+
+        # Check that the images have the same size
+        check_image_size(bg_image, fg_image, masks_dict)
+
+        # State the plot labelling
+        title, x_label, y_label = image_map_labels(title, wcs, line_bg, line_fg, masks_dict)
+
+        # User configuration overrites user
+        ax_cfg.setdefault('xlabel', x_label)
+        ax_cfg.setdefault('ylabel', y_label)
+        ax_cfg.setdefault('title', title)
+        plt_cfg.setdefault('figure.figsize', (5 if masks_file is None else 10, 5))
+        plt_cfg.setdefault('axes.titlesize', 12)
+        plt_cfg.setdefault('legend.fontsize', 10)
+
+        PLT_CONF = {**STANDARD_PLOT, **plt_cfg}
+        AXES_CONF = {**STANDARD_AXES, **ax_cfg}
+
+        # Create and fill the figure
+        with rc_context(PLT_CONF):
+
+            # Generate the figure object
+            if (in_fig is None) and (in_ax is None):
+                if wcs is None:
+                    in_fig, in_ax = plt.subplots()
+                else:
+                    in_fig = plt.figure()
+                    in_ax = in_fig.add_subplot(projection=wcs, slices=('x', 'y', 1)) # TODO this extra dimension...
+
+            # Assing the axis
+            self._fig, self._ax = in_fig, in_ax
+            self._ax.update(AXES_CONF)
+
+            # Plot the image
+            image_plot(self._ax, bg_image, fg_image, fg_levels, fg_mesh, bg_scale, fg_scale, bg_color, fg_color)
+
+            # Plot the spatial masks
+            if len(masks_dict) > 0:
+                legend_hdl = spatial_mask_plot(self._ax, masks_dict, mask_color, mask_alpha, self._cube.units_flux)
+                self._ax.legend(handles=legend_hdl, bbox_to_anchor=(1.05, 1), loc=2, borderaxespad=0.)
+
+            # By default, plot on screen unless an output address is provided
+            self._fig.canvas.draw()
+            save_close_fig_swicth(output_address, 'tight', self._fig, maximise)
 
         return
 
 
 class SampleFigures(Plotter):
 
     def __init__(self, sample):
@@ -1970,22 +2330,22 @@
 
                         wave_array, gaussian_array = gaussian_profiles_computation(line_list, spec.log, (1 + spec.redshift))
                         wave_array, cont_array = linear_continuum_computation(line_list, spec.log, (1 + spec.redshift))
 
                         # Single component lines
                         line_g_list = self._gaussian_line_profiler(self._ax, line_list,
                                                                    wave_array, gaussian_array, cont_array,
-                                                                   z_corr, spec.log, spec.norm_flux)
+                                                                   z_corr, spec.log, spec.norm_flux,)
 
                         # Add the interactive pop-ups
                         self._mplcursor_parser(line_g_list, line_list, spec.log, spec.norm_flux, spec.units_wave,
                                                spec.units_flux)
 
                 # Plot the masked pixels
-                self._masks_plot(self._ax, line_list, wave_plot, flux_plot, z_corr, spec.log, idcs_mask)
+                _masks_plot(self._ax, line_list, wave_plot, flux_plot, z_corr, spec.log, idcs_mask)
 
             # Switch y_axis to logarithmic scale if requested
             if log_scale:
                 self._ax.set_yscale('log')
 
             # Add or remove legend according to the plot type:
             # TODO we should be able to separate labels from sample objects from line fits
```

### Comparing `lime-stable-0.9.8/src/lime/tables.py` & `lime-stable-0.9.9/src/lime/tables.py`

 * *Files identical despite different names*

### Comparing `lime-stable-0.9.8/src/lime/tools.py` & `lime-stable-0.9.9/src/lime/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,32 +30,41 @@
                     'mm': au.mm,
                     'Flam': au.erg/au.s/au.cm**2/au.AA,
                     'Fnu': au.erg/au.s/au.cm**2/au.Hz,
                     'Jy': au.Jy,
                     'mJy': au.mJy,
                     'nJy': au.nJy}
 
-UNITS_LATEX_DICT = {'A': '\AA',
-                    'um': '\mu\!m',
+UNITS_LATEX_DICT = {'A': r'\AA',
+                    'um': r'\mu\!m',
                     'nm': 'nm',
                     'Hz': 'Hz',
                     'cm': 'cm',
                     'mm': 'mm',
                     'Flam': r'erg\,cm^{-2}s^{-1}\AA^{-1}',
                     'Fnu': r'erg\,cm^{-2}s^{-1}\Hz^{-1}',
                     'Jy': 'Jy',
                     'mJy': 'mJy',
                     'nJy': 'nJy'}
 
 DISPERSION_UNITS = ('A', 'um', 'nm', 'Hz', 'cm', 'mm')
 
 FLUX_DENSITY_UNITS = ('Flam', 'Fnu', 'Jy', 'mJy', 'nJy')
 
+PARAMETER_LATEX_DICT = {'Flam': r'$F_{\lambda}$',
+                        'Fnu': r'$F_{\nu}$',
+                        'SN_line': r'$\frac{S}{N}_{line}$',
+                        'SN_cont': r'$\frac{S}{N}_{cont}$'}
+
 WAVE_UNITS_DEFAULT, FLUX_UNITS_DEFAULT = au.AA, au.erg / au.s / au.cm ** 2 / au.AA
 
+# Variables with the astronomical coordinate information for the creation of new .fits files
+COORD_ENTRIES = ['CRPIX1', 'CRPIX2', 'CRVAL1', 'CRVAL2', 'CD1_1', 'CD1_2', 'CD2_1', 'CD2_2', 'CUNIT1', 'CUNIT2',
+                 'CTYPE1', 'CTYPE2']
+
 MACHINE_PATH = Path(__file__).parent/'resources'/'LogitistRegression_v2_cost1_logNorm.joblib'
 
 _REFERENCE_LINES = np.array(['H1_1216A', 'C4_1549A', 'He2_1640A', 'O3]_1666A', 'C3]_1980A', 'Mg2_2800A', '[O3]_3727A',
                              '[Ne3]_3869A', 'H1_3889A', 'H1_3970A', 'H1_4341A',
                              'H1_4861A', '[O3]_5007A', 'H1_6563A', 'S3_9069A', 'S3_9531A', 'H1_10050A', 'He1_10830A', 'H1_10940A',  'H1_12820A',
                               'Fe2_16440A', 'H1_18756A', 'H1_19450A', 'Si6_19620A', 'He1_20590A', 'H2_21210A', 'H1_21661A', 'H2_24070A',
                               'Si6_24830A', 'H1_26259A',  'H1_32970A', 'PAH1_33000A', 'H1_37406A', 'H1_40522A', 'H1_46539A'])
@@ -544,15 +553,28 @@
 
         idcsContLeft = ((wave_arr[idcsW[:, 0]] <= wave_arr[:, None]) & (wave_arr[:, None] <= wave_arr[idcsW[:, 1]]) & idcsValid).squeeze()
         idcsContRight = ((wave_arr[idcsW[:, 4]] <= wave_arr[:, None]) & (wave_arr[:, None] <= wave_arr[idcsW[:, 5]]) & idcsValid).squeeze()
 
         return idcsLineRegion, idcsContLeft, idcsContRight
 
 
+def get_coord_entries(hdr, coord_entries=None):
+
+    if coord_entries is None:
+        coord_entries = COORD_ENTRIES
+
+    output_dict = {}
+    for key in coord_entries:
+        if key in hdr:
+            output_dict[key] = hdr[key]
+
+    if len(output_dict) < 2:
+        _logger.info(f'{len(output_dict)} coordinate entries were found in the input header: {output_dict.keys()}')
 
+    return output_dict
 
 
 class LineFinder:
 
     def __init__(self, machine_model_path=MACHINE_PATH):
 
         # self.ml_model = joblib.load(machine_model_path) # THIS CAN be warning at opening the file
@@ -592,15 +614,15 @@
                                 f' number')
                 continuum_fit = np.full(input_wave.size, np.nan)
 
             # Compute the continuum and assign replace the value outside the bands the new continuum
             if plot_results:
                 title = f'Continuum fitting, iteration ({i+1}/{len(degree_list)})'
                 continuum_full = poly3Out.eval(x=self.wave.data)
-                self._plot_continuum_fit(continuum_full, mask_cont, low_lim, high_lim, threshold_list[i], title)
+                self.plot._plot_continuum_fit(continuum_full, mask_cont, low_lim, high_lim, threshold_list[i], title)
 
         # Include the standard deviation of the spectrum for the unmasked pixels
         if return_std:
             std_spec = np.std((self.flux-continuum_fit)[mask_cont])
             output_params = (continuum_fit, std_spec)
         else:
             output_params = continuum_fit
```

### Comparing `lime-stable-0.9.8/src/lime/transitions.py` & `lime-stable-0.9.9/src/lime/transitions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 
 from numpy import array, abs, nan, all, diff, char, searchsorted, zeros, unique, empty
 from .tools import DISPERSION_UNITS, UNITS_LATEX_DICT
-from .io import _PARENT_BANDS
+from .io import _PARENT_BANDS, _LOG_EXPORT, _LOG_COLUMNS
+# from .io import _LOG_EXPORT, _LOG_COLUMNS, load_lines_log, progress_bar
 
 _logger = logging.getLogger('LiMe')
 
 
 VAL_LIST = [1000, 900, 500, 400, 100, 90, 50, 40, 10, 9, 5, 4, 1]
 SYB_LIST = ["M", "CM", "D", "CD", "C", "XC", "L", "XL", "X", "IX", "V", "IV", "I"]
 
@@ -146,20 +147,20 @@
     
     return ion, wave, units_wave, kinem
 
 
 class Line:
 
     def __init__(self, label, band=None, fit_conf=None, emission_check=True, cont_from_bands=True, ref_log=None,
-                 z_line=0):
+                 z_line=0, interpret=True):
 
-        self.line, self.mask = None, array([nan] * 6)
+        self.label, self.mask = label, array([nan] * 6)
         self.blended_check, self.merged_check = False, False
         self.profile_label, self.list_comps = 'no', None
-        self.ion, self.wave, self.units_wave, self.kinem, self.latex = None, None, None, None, None
+        self.ion, self.wavelength, self.units_wave, self.kinem, self.latex = None, None, None, None, None
 
         self.intg_flux, self.intg_err = None, None
         self.peak_wave, self.peak_flux = None, None
         self.eqw, self.eqw_err = None, None
         self.gauss_flux, self.gauss_err = None, None
         self.cont, self.std_cont =None, None
         self.m_cont, self.n_cont = None, None
@@ -185,18 +186,74 @@
         self._fit_conf = None
         self._emission_check = emission_check
         self._cont_from_adjacent = cont_from_bands
         self._decimal_wave = False
         self._narrow_check = False
 
         # Interpret the line from the user reference
-        self._line_derivation(label, band, fit_conf, ref_log=ref_log)
+        if interpret:
+            self._line_derivation(label, band, fit_conf, ref_log=ref_log)
 
         return
 
+    @classmethod
+    def from_log(cls, label, log=None, norm_flux=1):
+
+        # Recover the label just in case
+        label = check_line_in_log(label, log)
+
+        # Create the line object
+        inline = cls(label, interpret=False)
+
+        if log is not None:
+
+            if label in log.index:
+
+                # Recover "simple" attributes
+                for param in _LOG_EXPORT:
+
+                    param_value = log.loc[label, param]
+
+                    # Normalize
+                    if _LOG_COLUMNS[param][0]:
+                        param_value = param_value / norm_flux
+
+                    inline.__setattr__(param, param_value)
+
+                # Recover "complex" attributes
+                for param in ['ion', 'wavelength', 'latex_label']:
+                    inline.__setattr__(param, log.loc[label, param])
+
+                # Band
+                inline.mask = log.loc[label, 'w1':'w6'].values
+
+                # Checks:
+                if inline.profile_label != 'no':
+                    inline.blended_check, inline.merged_check = False, False
+
+                    if inline.label.endswith('_m'):
+                        inline.merged_check = True
+                    else:
+                        inline.blended_check = True
+
+                # List comps
+                if inline.blended_check:
+                    inline.list_comps = array(inline.profile_label.split('-'))
+
+                else:
+                    inline.list_comps = array([inline.label])
+
+            else:
+                _logger.warning(f'Input line {inline.label} not found in log')
+
+        else:
+            _logger.warning(f'No lines log introduced for the line {inline.label}')
+
+        return inline
+
     def _line_derivation(self, label, band, fit_conf=None, ref_log=None):
 
         # Discriminate between string and float transitions
         ref_log = ref_log if ref_log is not None else _PARENT_BANDS
         self.label = check_line_in_log(label, ref_log)
 
         # Copy the input configuration dictionary
@@ -210,22 +267,22 @@
         if (suffix == '_b') or (suffix == '_m'):
             if self.profile_label != 'no':
                 if suffix == '_b':
                     self.blended_check = True
                 else:
                     self.merged_check = True
             else:
-                _logger.warning(f'The line {self.line} has the "{suffix}" suffix but no components have been specified '
+                _logger.warning(f'The line {self.label} has the "{suffix}" suffix but no components have been specified '
                                 f'for the fitting')
 
         # Blended lines have various elements in the list, single and merged only one
         self.list_comps = self.profile_label.split('-') if self.blended_check else [self.label]
 
         # Get transition data from label
-        self.ion, self.wave, self.units_wave, self.kinem = label_components(self.list_comps)
+        self.ion, self.wavelength, self.units_wave, self.kinem = label_components(self.list_comps)
 
         # Provide a band from the log if available the band
         if band is None:
             query_label = self.label if self.profile_label == 'no' else self.label[:-2]
             if query_label in ref_log.index:
                 try:
                     self.mask = ref_log.loc[query_label, 'w1':'w6'].values
@@ -234,16 +291,16 @@
         else:
             self.mask = band
 
         # Warn if the band wavelengths are not sorted and the theoretical value is not within the line region
         if self.mask is not None:
             if not all(diff(self.mask) >= 0):
                 _logger.warning(f'The line {label} band wavelengths are not sorted: {band}')
-            if not all(self.mask[2] < self.wave) and all(self.wave < self.mask[3]):
-                _logger.warning(f'The line {label} transition at {self.wave} is outside the line band wavelengths: '
+            if not all(self.mask[2] < self.wavelength) and not all(self.wavelength < self.mask[3]):
+                _logger.warning(f'The line {label} transition at {self.wavelength} is outside the line band wavelengths: '
                                 f'w3 = {self.mask[2]};  w4 = {self.mask[3]}')
 
         # Check if there are masked pixels in the line
         self.pixel_mask = self._fit_conf.get(f'{self.label}_mask', 'no')
 
         # Check if the wavelength has decimal transition
         self._decimal_wave = True if '.' in self.label else False
@@ -264,10 +321,10 @@
         elif self.blended_check:
             list_comps = self.list_comps
             for i, comp in enumerate(list_comps):
                 self.latex[i] = latex_from_label(comp)
 
         # Single
         else:
-            self.latex[0] = latex_from_label(None, self.ion[0], self.wave[0], self.units_wave[0], self.kinem[0])
+            self.latex[0] = latex_from_label(None, self.ion[0], self.wavelength[0], self.units_wave[0], self.kinem[0])
 
         return
```

### Comparing `lime-stable-0.9.8/src/lime/treatment.py` & `lime-stable-0.9.9/src/lime/treatment.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 from astropy.io import fits
 from astropy.wcs import WCS
 
 from .model import EmissionFitting
 from .tools import label_decomposition, LineFinder, UNITS_LATEX_DICT, latex_science_float, DISPERSION_UNITS,\
                    FLUX_DENSITY_UNITS, unit_convertor, define_masks
 
-from .plots import LiMePlots, STANDARD_PLOT, STANDARD_AXES, colorDict, save_close_fig_swicth, frame_mask_switch, LimeFigures, SampleFigures
-from .plots_interactive import SpectrumCheck
-from .io import _LOG_DTYPES_REC, _LOG_EXPORT, _LOG_COLUMNS, load_lines_log, save_line_log
+from .plots import LiMePlots, STANDARD_PLOT, STANDARD_AXES, colorDict, save_close_fig_swicth, frame_mask_switch, SpectrumFigures, SampleFigures, CubeFigures
+from .plots_interactive import SpectrumCheck, CubeCheck
+from .io import _LOG_DTYPES_REC, _LOG_EXPORT, _LOG_COLUMNS, load_lines_log, save_line_log, LiMe_Error
 from .model import gaussian_profiles_computation, linear_continuum_computation
 from .transitions import Line
-from .workflow import LineTreatment
+from .workflow import SpecTreatment, CubeTreatment
+from . import Error
 
 from matplotlib import pyplot as plt, colors, cm, gridspec, rc_context
 from matplotlib.widgets import SpanSelector
 from matplotlib.widgets import RadioButtons
 
 _logger = logging.getLogger('LiMe')
 
@@ -32,14 +33,45 @@
     mplcursors_check = False
 
 if mplcursors_check:
     from mplcursors._mplcursors import _default_annotation_kwargs as popupProps
     popupProps['bbox']['alpha'] = 0.9
 
 
+
+def check_inputs(wave, flux, err_flux, lime_object):
+
+    for i, items in enumerate(locals().items()):
+
+        if i < 3:
+
+            key, value = items
+            if value is not None:
+
+                # Confirm numpy array inputs
+                if isinstance(value, np.ndarray):
+
+                    # Confirm dimensions
+                    dimensions = len(value.shape)
+                    spec_check = dimensions == 1 and (isinstance(lime_object, Spectrum) or key == 'wave')
+                    cube_type = dimensions == 3 and isinstance(lime_object, Cube)
+                    if not spec_check and not cube_type:
+                        raise LiMe_Error(f'The dimensions of the input {key} are {dimensions}.\n'
+                                         f'LiMe only recognizes 1D arrays for the wavelength array, \n'
+                                         f'1D flux arrays for the Spectrum objects \n'
+                                         f'and 3D flux arrays Cube objects.')
+                else:
+                    raise LiMe_Error(f'The input {key} array must be numpy array. The input variable type is a {type(value)}')
+            else:
+                if key in ['wave', 'flux']:
+                    _logger.info(f'No value has been provided for {key}.')
+
+    return
+
+
 def check_units_norm_redshift(units_wave, units_flux, norm_flux, redshift):
 
     # Checks spectra units
     for arg in ['units_wave', 'units_flux']:
         arg_value = locals()[arg]
         if arg_value not in UNITS_LATEX_DICT:
             _logger.warning(f'Input {arg} = {arg_value} is not recognized.\nPlease try to convert it to the accepted'
@@ -47,32 +79,72 @@
 
     # Check if spectrum redshift and flux normalization flux are provided
     for arg in ['norm_flux', 'redshift']:
         arg_value = locals()[arg]
         if arg_value is None:
             _logger.debug(f'No value provided for the {arg}')
 
+
+    return
+
+
+def check_spectrum_axes(lime_object):
+
+    # Check for masked arrays
+    check_mask = np.zeros(3).astype(bool)
+    for i, arg in enumerate(['wave', 'wave_rest', 'flux']):
+        if np.ma.is_masked(lime_object.__getattribute__(arg)):
+            check_mask[i] = True
+
+    if np.any(check_mask):
+        lime_object._masked_inputs = True
+        if ~np.all(check_mask):
+            _logger.warning(f'Make sure *all* your input wavelength, flux and uncertainty are masked arrays')
+
+    # Check that the flux and wavelength normalization
+    if not isinstance(lime_object, Cube):
+        if np.nanmedian(lime_object.flux) < 0.0001:
+            _logger.info(f'The input flux has a median value of {np.nanmedian(lime_object.flux):.2e} '
+                            f'{UNITS_LATEX_DICT[lime_object.units_flux]}. This can cause issues in the fitting. '
+                            f'Try changing the flux normalization')
+
     return
 
 
 def cropping_spectrum(crop_waves, input_wave, input_flux, input_err, pixel_mask):
 
     if crop_waves is not None:
+
         idcs_crop = np.searchsorted(input_wave, crop_waves)
         input_wave = input_wave[idcs_crop[0]:idcs_crop[1]]
-        input_flux = input_flux[idcs_crop[0]:idcs_crop[1]]
-        if input_err is not None:
-            input_err = input_err[idcs_crop[0]:idcs_crop[1]]
+
+        # Spectrum
+        if input_flux.shape == 1:
+            input_flux = input_flux[idcs_crop[0]:idcs_crop[1]]
+            if input_err is not None:
+                input_err = input_err[idcs_crop[0]:idcs_crop[1]]
+
+        # Cube
+        elif input_flux.shape == 3:
+            input_flux = input_flux[idcs_crop[0]:idcs_crop[1], :, :]
+            if input_err is not None:
+                input_err = input_err[idcs_crop[0]:idcs_crop[1], :, :]
+
+        # Not recognized
+        else:
+            raise LiMe_Error(f'The dimensions of the input flux are {input_flux.shape}. LiMe only recognized flux 1D '
+                             f'arrays for Spectrum objects and 3D arrays for Cube objects')
+
         if pixel_mask is not None:
             pixel_mask = pixel_mask[idcs_crop[0]:idcs_crop[1]]
 
     return input_wave, input_flux, input_err, pixel_mask
 
 
-def spec_definition(input_wave, input_flux, input_err, pixel_mask, redshift, norm_flux):
+def spec_normalization_masking(input_wave, input_flux, input_err, pixel_mask, redshift, norm_flux):
 
     # Apply the redshift correction
     if input_wave is not None:
         wave_rest = input_wave / (1 + redshift)
         if (input_wave is not None) and (input_flux is not None):
             wave = input_wave
             flux = input_flux  # * (1 + self.redshift)
@@ -87,18 +159,25 @@
         if input_err is not None:
             err_flux = err_flux / norm_flux
 
     # Masked the arrays if requested
     if pixel_mask is not None:
         wave = np.ma.masked_array(wave, pixel_mask)
         wave_rest = np.ma.masked_array(wave_rest, pixel_mask)
-        flux = np.ma.masked_array(flux, pixel_mask)
+
+        # Spectrum or Cube spectral masking
+        if len(input_flux.shape) == 1:
+            mask_array = pixel_mask
+        else:
+            mask_array = np.ones(flux.shape).astype(bool)
+            mask_array[pixel_mask, :, :] = pixel_mask
+        flux = np.ma.masked_array(flux, mask_array)
 
         if err_flux is not None:
-            err_flux = np.ma.masked_array(err_flux, pixel_mask)
+            err_flux = np.ma.masked_array(err_flux, mask_array)
 
     return wave, wave_rest, flux, err_flux
 
 
 class Spectrum(LineFinder):
 
     """
@@ -145,82 +224,120 @@
 
     :param label: Name for the spectrum object
     :type label: str, optional
 
     """
 
     def __init__(self, input_wave=None, input_flux=None, input_err=None, redshift=0, norm_flux=1.0, crop_waves=None,
-                 inst_FWHM = np.nan, units_wave='A', units_flux='Flam', pixel_mask=None, label=None):
+                 inst_FWHM = np.nan, units_wave='A', units_flux='Flam', pixel_mask=None, label=None, review_inputs=True):
 
-        # # Load parent classes
+        # Load parent classes
         LineFinder.__init__(self)
-        # EmissionFitting.__init__(self)
-        # LiMePlots.__init__(self)
-        # IntMaskInspector.__init__(self)
+
+        # Review the inputs
+        # check_inputs(input_wave, input_flux, input_err, self)
 
         # Class attributes
-        self.label = label
+        self.label = None
         self.wave = None
         self.wave_rest = None
         self.flux = None
         self.err_flux = None
-        self.norm_flux = norm_flux
-        self.redshift = redshift
+        self.norm_flux = None
+        self.redshift = None
         self.log = None
-        self.inst_FWHM = inst_FWHM
-        self.units_wave = units_wave
-        self.units_flux = units_flux
+        self.inst_FWHM = None
+        self.units_wave = None
+        self.units_flux = None
         self._masked_inputs = False
 
         # Treatments objects
-        self.fit = LineTreatment(self)
+        self.fit = SpecTreatment(self)
 
         # Plotting objects
-        self.plot = LimeFigures(self)
+        self.plot = SpectrumFigures(self)
         self.check = SpectrumCheck(self)
 
+        # # Checks spectra units
+        # check_units_norm_redshift(self.units_wave, self.units_flux, self.norm_flux, self.redshift)
+        #
+        # # Start cropping the input spectrum if necessary
+        # input_wave, input_flux, input_err, pixel_mask = cropping_spectrum(crop_waves, input_wave, input_flux, input_err,
+        #                                                                   pixel_mask)
+        #
+        # # Spectra normalization and masking
+        # self.wave, self.wave_rest, self.flux, self.err_flux = spec_normalization_masking(input_wave, input_flux,
+        #                                                                                  input_err, pixel_mask,
+        #                                                                                  self.redshift, self.norm_flux)
+        #
+        # # Check nan entries and mask quality
+        # check_spectrum_axes(self)
+        #
+        # # Generate empty dataframe to store measurement use cwd as default storing folder # TODO we are not using this
+        # self.log = pd.DataFrame(np.empty(0, dtype=_LOG_DTYPES_REC))
+
+        # Review and assign the attibutes data
+        if review_inputs:
+            self._set_attributes(input_wave, input_flux, input_err, redshift, norm_flux, crop_waves, inst_FWHM,
+                                 units_wave, units_flux, pixel_mask, label)
+
+        return
+
+    @classmethod
+    def from_cube(cls, cube, idx_j, idx_i, label=None):
+
+        # Load parent classes
+        spec = cls(review_inputs=False)
+
+        # Class attributes
+        spec.label = label
+        spec.wave = cube.wave
+        spec.wave_rest = cube.wave_rest
+        spec.flux = cube.flux[:, idx_j, idx_i]
+        spec.err_flux = None if cube.err_flux is None else cube.err_flux[:, idx_j, idx_i]
+        spec.norm_flux = cube.norm_flux
+        spec.redshift = cube.redshift
+        spec.log = pd.DataFrame(np.empty(0, dtype=_LOG_DTYPES_REC))
+        spec.inst_FWHM = cube.inst_FWHM
+        spec.units_wave = cube.units_wave
+        spec.units_flux = cube.units_flux
+        spec._masked_inputs = False
+
+        return spec
+
+    def _set_attributes(self, input_wave, input_flux, input_err, redshift, norm_flux, crop_waves, inst_FWHM, units_wave,
+                        units_flux, pixel_mask, label):
+
+        # Class attributes
+        self.label = label
+        self.norm_flux = norm_flux
+        self.redshift = redshift
+        self.inst_FWHM = inst_FWHM
+        self.units_wave = units_wave
+        self.units_flux = units_flux
+
+        # Review the inputs
+        check_inputs(input_wave, input_flux, input_err, self)
+
         # Checks spectra units
         check_units_norm_redshift(self.units_wave, self.units_flux, self.norm_flux, self.redshift)
 
         # Start cropping the input spectrum if necessary
         input_wave, input_flux, input_err, pixel_mask = cropping_spectrum(crop_waves, input_wave, input_flux, input_err,
                                                                           pixel_mask)
 
-        # Spectra normalization, redshift and mask calculation
-        self.wave, self.wave_rest, self.flux, self.err_flux = spec_definition(input_wave, input_flux, input_err,
-                                                                              pixel_mask, self.redshift, self.norm_flux)
-
-        # Check for dimensions and nan entries
-        for arg in ['wave', 'flux', 'err_flux']:
-            arg_array = self.__getattribute__(arg)
-            if arg_array is not None:
-                dimensions = len(arg_array.shape)
-                nan_entries = np.isnan(arg_array)
-                if np.any(nan_entries):
-                    _logger.warning(f'Input spectrum {arg} array has {np.sum(nan_entries)} nan entries. Try to mask '
-                                    f'these pixels to avoid issues with the measurements')
-                if dimensions != 1:
-                    _logger.warning(f'The input spectrum {arg} array has a number of dimensions {dimensions} > 1. This '
-                                    f'will cause issues in the measurements')
-            else:
-                if arg in ['wave', 'flux']:
-                    _logger.warning(f'No {arg} array introduced. This may bring issues in the measurement.')
+        # Spectra normalization and masking
+        self.wave, self.wave_rest, self.flux, self.err_flux = spec_normalization_masking(input_wave, input_flux,
+                                                                                         input_err, pixel_mask,
+                                                                                         self.redshift, self.norm_flux)
 
-        # Check for masked arrays
-        check_mask = np.zeros(3).astype(bool)
-        for i, arg in enumerate(['wave', 'wave_rest', 'flux']):
-            if np.ma.is_masked(self.__getattribute__(arg)):
-                check_mask[i] = True
-
-        if np.any(check_mask):
-            self._masked_inputs = True
-            if ~np.all(check_mask):
-                _logger.warning(f'Make sure *all* your input wavelength, flux and uncertainty are masked arrays')
+        # Check nan entries and mask quality
+        check_spectrum_axes(self)
 
-        # Generate empty dataframe to store measurement use cwd as default storing folder
+        # Generate empty dataframe to store measurement use cwd as default storing folder # TODO we are not using this
         self.log = pd.DataFrame(np.empty(0, dtype=_LOG_DTYPES_REC))
 
         return
 
     def convert_units(self, units_wave=None, units_flux=None, norm_flux=None):
 
         # Dispersion axes conversion
@@ -290,460 +407,642 @@
                 self.flux = self.flux * self.norm_flux / norm_flux
                 self.err_flux = None if self.err_flux is None else self.err_flux * self.norm_flux / norm_flux
             self.norm_flux = norm_flux
 
         return
 
 
-class Cube(EmissionFitting, LineFinder, LiMePlots):
+class Cube:
 
     def __init__(self, input_wave=None, input_flux=None, input_err=None, redshift=0, norm_flux=1.0, crop_waves=None,
-                 inst_FWHM = np.nan, units_wave='A', units_flux='Flam', spatial_mask=None, label=None):
+                 inst_FWHM = np.nan, units_wave='A', units_flux='Flam', spatial_mask=None, pixel_mask=None, obj_name=None):
+
+        # Review the inputs
+        check_inputs(input_wave, input_flux, input_err, self)
 
         # Class attributes
-        self.label = label
+        self.obj_name = obj_name
         self.wave = None
         self.wave_rest = None
         self.flux = None
         self.err_flux = None
         self.norm_flux = norm_flux
         self.redshift = redshift
         self.log = None
         self.inst_FWHM = inst_FWHM
         self.units_wave = units_wave
         self.units_flux = units_flux
         self._masked_inputs = False
 
-        return
+        # Treatments objects
+        self.fit = CubeTreatment(self)
 
+        # Plotting objects
+        self.plot = CubeFigures(self)
+        self.check = CubeCheck(self)
 
-class Sample(dict):
+        # Checks spectra units
+        check_units_norm_redshift(self.units_wave, self.units_flux, self.norm_flux, self.redshift)
 
-    def __init__(self, spec_dict={}):
+        # Start cropping the input spectrum if necessary
+        input_wave, input_flux, input_err, pixel_mask = cropping_spectrum(crop_waves, input_wave, input_flux, input_err,
+                                                                          pixel_mask)
 
-        # Inherit the default dictionary properties
-        super().__init__(spec_dict)
+        # Spectra normalization, redshift and mask calculation
+        self.wave, self.wave_rest, self.flux, self.err_flux = spec_normalization_masking(input_wave, input_flux,
+                                                                                         input_err, pixel_mask,
+                                                                                         self.redshift, self.norm_flux)
 
-        # Attributes
-        self.obj_list = np.array([])
-        self.plot = SampleFigures(self)
-        self.norm_flux = None
-        self.units_wave = None
-        self.units_flux = None
+        # Check nan entries and mask quality
+        check_spectrum_axes(self)
 
         return
 
-    def add_object(self, label, obs_type='spectrum', **kwargs):
-
-        # Establish the type of observations
-        if obs_type == 'spectrum':
-
-            lime_obj = Spectrum(label=label, **kwargs)
-
-        # Add object to the container
-        self[label] = lime_obj
-
-        # Renew the list of objects
-        self.obj_list = np.array(list(self.keys()))
-
-        # Check if the units and normalizations match
-        if len(self.keys()) == 1:
-            print('ALOMOJOR')
-            self.norm_flux = lime_obj.norm_flux
-            self.units_wave, self.units_flux = lime_obj.units_wave, lime_obj.units_flux
-
-        else:
-            for prop in ['norm_flux', 'units_wave', 'units_flux']:
-                if self.__getattribute__(prop) != lime_obj.__getattribute__(prop):
-                    _logger.warning(f'The {prop} of object {label} do not match those in the sample:'
-                                    f' "{lime_obj.__getattribute__(prop)}" in object versus "{self.__getattribute__(prop)}" in sample')
-
-
-class MaskInspector(Spectrum):
+    def spatial_masker(self, line, band=None, param=None, percentiles=[85, 90, 95], mask_ref=None, min_percentil=None,
+                       output_address=None, header_dict={}, bands_frame=None):
 
-    """
-    This class plots the masks from the ``_log_address`` as a grid for the input spectrum. Clicking and
-    dragging the mouse within a line cell will update the line band region, both in the plot and the ``_log_address``
-    file provided.
-
-    Assuming that the band wavelengths `w1` and `w2` specify the adjacent blue (left continuum), the `w3` and `w4`
-    wavelengths specify the line band and the `w5` and `w6` wavelengths specify the adjacent red (right continuum)
-    the interactive selection has the following rules:
-
-    * The plot wavelength range is always 5 pixels beyond the mask bands. Therefore dragging the mouse beyond the
-      mask limits (below `w1` or above `w6`) will change the displayed range. This can be used to move beyond the
-      original mask limits.
-
-    * Selections between the `w2` and `w5` wavelength bands are always assigned to the line region mask as the new
-      `w3` and `w4` values.
-
-    * Due to the previous point, to increase the `w2` value or to decrease `w5` value the user must select a region
-      between `w1` and `w3` or `w4` and `w6` respectively.
+        """
+        This function computes a spatial mask for an input flux image given an array of limits for a certain intensity parameter.
+        Currently, the only one implemented is the percentile intensity. If an output address is provided, the mask is saved as a fits file
+        where each intensity level mask is stored in its corresponding page. The parameter calculation method, its intensity and mask
+        index are saved in the corresponding HDU header as PARAM, PARAMIDX and PARAMVAL.
 
-    The user can limit the number of lines displayed on the screen using the ``lines_interval`` parameter. This
-    parameter can be an array of strings with the labels of the target lines or a two value integer array with the
-    interval of lines to plot.
+        :param image_flux: Matrix with the image flux to be spatially masked.
+        :type image_flux: np.array()
 
-    Lines in the mask file outside the spectral wavelength range will be excluded from the plot: w2 and w5 smaller
-    and greater than the blue and red wavelegnth values respectively.
+        :param mask_param: Flux intensity model from which the masks are calculated. The options available are 'flux',
+               'SN_line' and 'SN_cont'.
+        :type mask_param: str, optional
 
-    :param log_address: Address for the lines log mask file.
-    :type log_address: str
+        :param contour_levels: Vector in decreasing order with the parameter values for the mask_param chosen.
+        :type contour_levels: np.array()
 
-    :param input_wave: Wavelength array of the input spectrum.
-    :type input_wave: numpy.array
+        :param mask_ref: String label for the mask. If none provided the masks will be named in cardinal order.
+        :type mask_ref: str, optional
 
-    :param input_flux: Flux array for the input spectrum.
-    :type input_flux: numpy.array
+        :param output_address: Output address for the mask fits file.
+        :type output_address: str, optional
 
-    :param input_err: Sigma array of the `input_flux`
-    :type input_err: numpy.array, optional
+        :param min_level: Minimum level for the masks calculation. If none is provided the minimum value from the contour_levels
+                          vector will be used.
+        :type min_level: float, optional
 
-    :param redshift: Spectrum redshift
-    :type redshift: float, optional
+        :param show_plot: If true a plot will be displayed with the mask calculation. Additionally, if an output_address is
+                          provided the plot will be saved in the parent folder as image taking into consideration the
+                          mask_ref value.
+        :type show_plot: bool, optional
 
-    :param norm_flux: Spectrum flux normalization
-    :type norm_flux: float, optional
+        :param fits_header: Dictionary with key-values to be included in the output .fits file header.
+        :type fits_header: dict, optional
 
-    :param crop_waves: Wavelength limits in a two value array
-    :type crop_waves: np.array, optional
+        :return:
+        """
 
-    :param n_cols: Number of columns of the grid plot
-    :type n_cols: integer
+        # Check the function inputs
+        if not np.all(np.diff(percentiles) > 0):
+            raise Error(f'The mask percentiles ({percentiles}) must be in increasing order')
+        inver_percentiles = np.flip(percentiles)
 
-    :param n_rows: Number of columns of the grid plot
-    :type n_rows: integer
+        if not param in [None, 'SN_line', 'SN_cont']:
+            raise Error(f'The mask calculation parameter ({param}) is not recognised. Please use "flux", "SN_line", "SN_cont"')
 
-    :param lines_interval: List of lines or mask file line interval to display on the grid plot. In the later case
-                           this interval must be a two value array.
-    :type lines_interval: list
-
-    :param y_scale: Y axis scale. The default value (auto) will switch between between linear and logarithmic scale
-                    strong and weak lines respectively. Use ``linear`` and ``log`` for a fixed scale for all lines.
-    :type y_scale: str, optional
 
-    """
+        # TODO overwrite spatial mask file not update
+        # Line for the background image
+        line_bg = Line(line, band, ref_log=bands_frame)
 
-    def __init__(self, log_address, input_wave=None, input_flux=None, input_err=None, redshift=0,
-                 norm_flux=1.0, crop_waves=None, n_cols=10, n_rows=None, lines_interval=None, y_scale='auto'):
+        # Get the band indexes
+        idcsEmis, idcsCont = define_masks(self.wave, line_bg.mask * (1 + self.redshift), line_bg.pixel_mask)
+        signal_slice = self.flux[idcsEmis, :, :]
 
-        # Output file address
-        self.linesLogAddress = Path(log_address)
-        self.y_scale = y_scale
+        # If not mask parameter provided we use the flux percentiles
+        if param is None:
+            default_title = 'Flux percentiles masks'
+            param = self.units_flux
+            param_image = signal_slice.sum(axis=0)
 
-        # Assign attributes to the parent class
-        super().__init__(input_wave, input_flux, input_err, redshift, norm_flux, crop_waves)
+        # S/N cont
+        elif param == 'SN_cont':
+            default_title = 'Continuum S/N percentile masks'
 
-        # Lines log address is provided and we read the DF from it
-        if Path(self.linesLogAddress).is_file():
-            self.log = load_lines_log(self.linesLogAddress)
+            param_image = np.nanmean(signal_slice, axis=0) / np.nanstd(signal_slice, axis=0)
 
-        # Lines log not provide code ends
+        # S/N line
         else:
-            _logger.warning(f'No lines log file found at {log_address}. Leaving the script')
-            exit()
+            default_title = 'Emission line S/N percentile masks'
 
-        # Only plotting the lines in the lines interval
-        self.line_inter = lines_interval
-        if lines_interval is None:
-            n_lines = len(self.log.index)
-            self.target_lines = self.log.index.values
+            n_pixels = np.sum(idcsCont)
+            cont_slice = self.flux[idcsCont, :, :]
+            Amp_image = np.nanmax(signal_slice, axis=0) - np.nanmean(cont_slice, axis=0)
+            std_image = np.nanstd(cont_slice, axis=0)
+            param_image = (np.sqrt(2 * n_pixels * np.pi) / 6) * (Amp_image / std_image)
+
+        # Percentiles vector for the target parameter
+        param_array = np.nanpercentile(param_image, inver_percentiles)
+
+        # If minimum level not provided by user use lowest contour_level
+        min_level = param_array[-1] if min_percentil is None else min_percentil
+
+        # Containers for the mask parameters
+        mask_dict = {}
+        param_level = {}
+        boundary_dict = {}
+
+        # Loop throught the counter levels and compute the
+        for i, n_levels in enumerate(param_array):
+
+            # # Operation every element
+            if i == 0:
+                maParamImage = np.ma.masked_where((param_image >= param_array[i]) &
+                                                  (param_image >= min_level),
+                                                  param_image)
 
-        else:
-            # Array of strings
-            if isinstance(lines_interval[0], str):
-                n_lines = len(lines_interval)
-                self.target_lines = np.array(lines_interval, ndmin=1)
-            # Array of integers
             else:
-                n_lines = lines_interval[1] - lines_interval[0]
-                self.target_lines = self.log[lines_interval[0]:lines_interval[1]].index.values
-
-        # Establish the grid shape
-        if n_lines > n_cols:
-            if n_rows is None:
-                n_rows = int(np.ceil(n_lines / n_cols))
-        else:
-            n_cols = n_lines
-            n_rows = 1
-
-        # Adjust the plot theme
-        PLOT_CONF = STANDARD_PLOT.copy()
-        AXES_CONF = STANDARD_AXES.copy()
-        PLOT_CONF['figure.figsize'] = (n_rows * 2, 8)
-        AXES_CONF.pop('xlabel')
-
-        with rc_context(PLOT_CONF):
-
-            self.fig, ax = plt.subplots(nrows=n_rows, ncols=n_cols)
-            self.ax = ax.flatten() if n_lines > 1 else [ax]
-            self.in_ax = None
-            self.dict_spanSelec = {}
-            self.axConf = {}
-
-            # Plot function
-            self.plot_line_mask_selection(logscale=self.y_scale, grid_size=n_rows * n_cols, n_lines=n_lines)
-            plt.gca().axes.yaxis.set_ticklabels([])
-
-            try:
-                manager = plt.get_current_fig_manager()
-                manager.window.showMaximized()
-            except:
-                print()
-
-            # Show the image
-            save_close_fig_swicth(None, 'tight', self.fig)
-
-
-        return
-
-    def plot_line_mask_selection(self, logscale='auto', grid_size=None, n_lines=None):
-
-        # Generate plot
-        for i in range(grid_size):
-            if i < n_lines:
-                line = self.target_lines[i]
-                if line in self.log.index:
-                    self.mask = self.log.loc[line, 'w1':'w6'].values
-                    self.plot_line_region_i(self.ax[i], line, logscale=logscale)
-                    self.dict_spanSelec[f'spanner_{i}'] = SpanSelector(self.ax[i],
-                                                                       self.on_select,
-                                                                       'horizontal',
-                                                                       useblit=True,
-                                                                       rectprops=dict(alpha=0.5, facecolor='tab:blue'))
-                else:
-                    print(f'- WARNING: line {line} not found in the input mask')
-
-            # Clear not filled axes
+                maParamImage = np.ma.masked_where((param_image >= param_array[i]) &
+                                                  (param_image < param_array[i - 1]) &
+                                                  (param_image >= min_level),
+                                                  param_image)
+
+            if np.sum(maParamImage.mask) > 0:
+                mask_dict[f'mask_{i}'] = maParamImage.mask
+                boundary_dict[f'mask_{i}'] = inver_percentiles[i]
+                param_level[f'mask_{i}'] = param_array[i]
+
+        # Use as HDU as container for the mask
+        hdul = fits.HDUList([fits.PrimaryHDU()])
+
+        for idx_region, region_items in enumerate(mask_dict.items()):
+            region_label, region_mask = region_items
+
+            # Metadata for the fits page
+            header_lime = {'PARAM': param,
+                           'PARAMIDX': boundary_dict[region_label],
+                           'PARAMVAL': param_level[region_label],
+                           'NUMSPAXE': np.sum(region_mask)}
+            fits_hdr = fits.Header(header_lime)
+
+            if header_dict is not None:
+                fits_hdr.update(header_dict)
+
+            # Extension for the mask
+            mask_ext = region_label if mask_ref is None else f'{mask_ref}_{region_label}'
+
+            # Mask HDU
+            mask_hdu = fits.ImageHDU(name=mask_ext, data=region_mask.astype(int), ver=1, header=fits_hdr)
+
+            hdul.append(mask_hdu)
+
+        # Output folder computed from the output address
+        output_address = Path(output_address) if output_address is not None else None
+
+        # Return an array with the masks
+        if output_address is not None:
+            if output_address.parent.is_dir():
+                hdul.writeto(output_address, overwrite=True, output_verify='fix')
+                output_func = None
             else:
-                self.fig.delaxes(self.ax[i])
-
-        bpe = self.fig.canvas.mpl_connect('button_press_event', self.on_click)
-        aee = self.fig.canvas.mpl_connect('axes_enter_event', self.on_enter_axes)
-
-        return
-
-    def plot_line_region_i(self, ax, lineLabel, limitPeak=5, logscale='auto'):
-
-        # Plot line region:
-        ion, lineWave, latexLabel = label_decomposition(lineLabel, scalar_output=True, units_wave=self.units_wave)
+                raise LiMe_Error(f'Mask could not be saved. Folder not found: {output_address.parent.as_posix()}')
 
-        # Decide type of plot
-        non_nan = (~pd.isnull(self.mask)).sum()
-
-        # Incomplete selections
-        if non_nan < 6:  # selections
-
-            # Peak region
-            idcsLinePeak = (lineWave - limitPeak <= self.wave_rest) & (self.wave_rest <= lineWave + limitPeak)
-            wavePeak, fluxPeak = self.wave_rest[idcsLinePeak], self.flux[idcsLinePeak]
-
-            # Plot region
-            idcsLineArea = (lineWave - limitPeak * 2 <= self.wave_rest) & (
-                        lineWave - limitPeak * 2 <= self.mask[3])
-            waveLine, fluxLine = self.wave_rest[idcsLineArea], self.flux[idcsLineArea]
-
-            # Plot the line region
-            ax.step(waveLine, fluxLine, where='mid')
-
-            # Fill the user selections
-            if non_nan == 2:
-                idx1, idx2 = np.searchsorted(self.wave_rest, self.mask[0:2])
-                ax.fill_between(self.wave_rest[idx1:idx2], 0.0, self.flux[idx1:idx2], facecolor=self._color_dict['cont_band'],
-                                step='mid', alpha=0.5)
-
-            if non_nan == 4:
-                idx1, idx2, idx3, idx4 = np.searchsorted(self.wave_rest, self.mask[0:4])
-                ax.fill_between(self.wave_rest[idx1:idx2], 0.0, self.flux[idx1:idx2], facecolor=self._color_dict['cont_band'],
-                                step='mid', alpha=0.5)
-                ax.fill_between(self.wave_rest[idx3:idx4], 0.0, self.flux[idx3:idx4], facecolor=self._color_dict['cont_band'],
-                                step='mid', alpha=0.5)
-
-        # Complete selections
+        # Return the hdul
         else:
+            output_func = hdul
 
-            # Get line regions
-            idcsContLeft = (self.mask[0] <= self.wave_rest) & (self.wave_rest <= self.mask[1])
-            idcsContRight = (self.mask[4] <= self.wave_rest) & (self.wave_rest <= self.mask[5])
-
-            idcsLinePeak = (lineWave - limitPeak <= self.wave_rest) & (self.wave_rest <= lineWave + limitPeak)
-            idcsLineArea = (self.mask[2] <= self.wave_rest) & (self.wave_rest <= self.mask[3])
-
-            waveCentral, fluxCentral = self.wave_rest[idcsLineArea], self.flux[idcsLineArea]
-            wavePeak, fluxPeak = self.wave_rest[idcsLinePeak], self.flux[idcsLinePeak]
-
-            idcsLinePlot = (self.mask[0] - 5 <= self.wave_rest) & (self.wave_rest <= self.mask[5] + 5)
-            waveLine, fluxLine = self.wave_rest[idcsLinePlot], self.flux[idcsLinePlot]
-
-            # Plot the line
-            ax.step(waveLine, fluxLine, color=self._color_dict['fg'], where='mid')
-
-            # Fill the user selections
-            ax.fill_between(waveCentral, 0, fluxCentral, step="mid", alpha=0.4, facecolor=self._color_dict['line_band'])
-            ax.fill_between(self.wave_rest[idcsContLeft], 0, self.flux[idcsContLeft], facecolor=self._color_dict['cont_band'],
-                            step="mid", alpha=0.2)
-            ax.fill_between(self.wave_rest[idcsContRight], 0, self.flux[idcsContRight], facecolor=self._color_dict['cont_band'],
-                            step="mid", alpha=0.2)
-
-        # Plot format
-        ax.yaxis.set_major_locator(plt.NullLocator())
-        ax.xaxis.set_major_locator(plt.NullLocator())
-
-        ax.update({'title': lineLabel})
-        ax.yaxis.set_ticklabels([])
-        ax.axes.yaxis.set_visible(False)
-        try:
-            idxPeakFlux = np.argmax(fluxPeak)
-            ax.set_ylim(ymin=np.min(fluxLine) / 5, ymax=fluxPeak[idxPeakFlux] * 1.25)
-
-            if logscale == 'auto':
-                if fluxPeak[idxPeakFlux] > 5 * np.median(fluxLine):
-                    ax.set_yscale('log')
-            else:
-                if logscale == 'log':
-                    ax.set_yscale('log')
-        except:
-            print(f'fail at {self.line}')
-
-
-        return
-
-    def on_select(self, w_low, w_high):
-
-        # Check we are not just clicking on the plot
-        if w_low != w_high:
-
-            # Count number of empty entries to determine next step
-            non_nans = (~pd.isnull(self.mask)).sum()
+        return output_func
 
-            # Case selecting 1/3 region
-            if non_nans == 0:
-                self.mask[0] = w_low
-                self.mask[1] = w_high
-
-            # Case selecting 2/3 region
-            elif non_nans == 2:
-                self.mask[2] = w_low
-                self.mask[3] = w_high
-                self.mask = np.sort(self.mask)
-
-            # Case selecting 3/3 region
-            elif non_nans == 4:
-                self.mask[4] = w_low
-                self.mask[5] = w_high
-                self.mask = np.sort(self.mask)
-
-            elif non_nans == 6:
-                self.mask = np.sort(self.mask)
-
-                # Caso que se corrija la region de la linea
-                if w_low > self.mask[1] and w_high < self.mask[4]:
-                    self.mask[2] = w_low
-                    self.mask[3] = w_high
-
-                # Caso que se corrija el continuum izquierdo
-                elif w_low < self.mask[2] and w_high < self.mask[2]:
-                    self.mask[0] = w_low
-                    self.mask[1] = w_high
-
-                # Caso que se corrija el continuum derecho
-                elif w_low > self.mask[3] and w_high > self.mask[3]:
-                    self.mask[4] = w_low
-                    self.mask[5] = w_high
-
-                # Case we want to select the complete region
-                elif w_low < self.mask[0] and w_high > self.mask[5]:
-
-                    # # Remove line from dataframe and save it
-                    # self.remove_lines_df(self.current_df, self.Current_Label)
-                    #
-                    # # Save lines log df
-                    # self.save_lineslog_dataframe(self.current_df, self.lineslog_df_address)
+    def get_spaxel(self, idx_j, idx_i, label=None):
 
-                    # Clear the selections
-                    # self.mask = np.array([np.nan] * 6)
-
-                    print(f'\n-- The line {self.line} mask has been removed')
-
-                else:
-                    print('- WARNING: Unsucessful line selection:')
-                    print(f'-- {self.line}: w_low: {w_low}, w_high: {w_high}')
+        spaxel = Spectrum.from_cube(self, idx_j, idx_i, label)
 
-            # Check number of measurements after selection
-            non_nans = (~pd.isnull(self.mask)).sum()
+        return spaxel
 
-            # Proceed to re-measurement if possible:
-            if non_nans == 6:
 
-                # TODO add option to perform the measurement a new
-                # self.clear_fit()
-                # self.fit_from_wavelengths(self.line, self.mask, user_cfg={})
+class Sample(dict):
 
-                # Parse the line regions to the dataframe
-                self.results_to_database(self.line, self.log, fit_conf={}, export_params=[])
+    def __init__(self, spec_dict={}):
 
-                # Save the corrected mask to a file
-                self.store_measurement()
+        # Inherit the default dictionary properties
+        super().__init__(spec_dict)
 
-            # Redraw the line measurement
-            self.in_ax.clear()
-            self.plot_line_region_i(self.in_ax, self.line, logscale=self.y_scale)
-            self.in_fig.canvas.draw()
+        # Attributes
+        self.obj_list = np.array([])
+        self.plot = SampleFigures(self)
+        self.norm_flux = None
+        self.units_wave = None
+        self.units_flux = None
 
         return
 
-    def on_enter_axes(self, event):
-
-        # Assign new axis
-        self.in_fig = event.canvas.figure
-        self.in_ax = event.inaxes
-
-        # TODO we need a better way to index than the latex label
-        # Recognise line line
-        idx_line = self.log.index == self.in_ax.get_title()
-        self.line = self.log.loc[idx_line].index.values[0]
-        self.mask = self.log.loc[idx_line, 'w1':'w6'].values[0]
-
-        # Restore measurements from log
-        # self.database_to_attr()
-
-        # event.inaxes.patch.set_edgecolor('red')
-        # event.canvas.draw()
-
-    def on_click(self, event):
+    def add_object(self, label, obs_type='spectrum', **kwargs):
 
-        if event.dblclick:
-            print(self.line)
-            print(f'{event.button}, {event.x}, {event.y}, {event.xdata}, {event.ydata}')
+        # Establish the type of observations
+        if obs_type == 'spectrum':
 
-    def store_measurement(self):
+            lime_obj = Spectrum(label=label, **kwargs)
 
-        # Read file in the stored address
-        if self.linesLogAddress.is_file():
-            file_DF = load_lines_log(self.linesLogAddress)
+        # Add object to the container
+        self[label] = lime_obj
 
-            # Add new line to the DF and sort it if it was new
-            if self.line in file_DF.index:
-                file_DF.loc[self.line, 'w1':'w6'] = self.mask
-            else:
-                file_DF.loc[self.line, 'w1':'w6'] = self.mask
+        # Renew the list of objects
+        self.obj_list = np.array(list(self.keys()))
 
-                # Sort the lines by theoretical wavelength
-                lineLabels = file_DF.index.values
-                ion_array, wavelength_array, latexLabel_array = label_decomposition(lineLabels, units_wave=self.units_wave)
-                file_DF = file_DF.iloc[wavelength_array.argsort()]
+        # Check if the units and normalizations match
+        if len(self.keys()) == 1:
+            print('ALOMOJOR')
+            self.norm_flux = lime_obj.norm_flux
+            self.units_wave, self.units_flux = lime_obj.units_wave, lime_obj.units_flux
 
-        # If the file does not exist (or it is the first time)
         else:
-            file_DF = self.log
+            for prop in ['norm_flux', 'units_wave', 'units_flux']:
+                if self.__getattribute__(prop) != lime_obj.__getattribute__(prop):
+                    _logger.warning(f'The {prop} of object {label} do not match those in the sample:'
+                                    f' "{lime_obj.__getattribute__(prop)}" in object versus "{self.__getattribute__(prop)}" in sample')
 
-        # Save to a file
-        save_line_log(file_DF, self.linesLogAddress)
 
-        return
+# class MaskInspector(Spectrum):
+#
+#     """
+#     This class plots the masks from the ``_log_address`` as a grid for the input spectrum. Clicking and
+#     dragging the mouse within a line cell will update the line band region, both in the plot and the ``_log_address``
+#     file provided.
+#
+#     Assuming that the band wavelengths `w1` and `w2` specify the adjacent blue (left continuum), the `w3` and `w4`
+#     wavelengths specify the line band and the `w5` and `w6` wavelengths specify the adjacent red (right continuum)
+#     the interactive selection has the following rules:
+#
+#     * The plot wavelength range is always 5 pixels beyond the mask bands. Therefore dragging the mouse beyond the
+#       mask limits (below `w1` or above `w6`) will change the displayed range. This can be used to move beyond the
+#       original mask limits.
+#
+#     * Selections between the `w2` and `w5` wavelength bands are always assigned to the line region mask as the new
+#       `w3` and `w4` values.
+#
+#     * Due to the previous point, to increase the `w2` value or to decrease `w5` value the user must select a region
+#       between `w1` and `w3` or `w4` and `w6` respectively.
+#
+#     The user can limit the number of lines displayed on the screen using the ``lines_interval`` parameter. This
+#     parameter can be an array of strings with the labels of the target lines or a two value integer array with the
+#     interval of lines to plot.
+#
+#     Lines in the mask file outside the spectral wavelength range will be excluded from the plot: w2 and w5 smaller
+#     and greater than the blue and red wavelegnth values respectively.
+#
+#     :param log_address: Address for the lines log mask file.
+#     :type log_address: str
+#
+#     :param input_wave: Wavelength array of the input spectrum.
+#     :type input_wave: numpy.array
+#
+#     :param input_flux: Flux array for the input spectrum.
+#     :type input_flux: numpy.array
+#
+#     :param input_err: Sigma array of the `input_flux`
+#     :type input_err: numpy.array, optional
+#
+#     :param redshift: Spectrum redshift
+#     :type redshift: float, optional
+#
+#     :param norm_flux: Spectrum flux normalization
+#     :type norm_flux: float, optional
+#
+#     :param crop_waves: Wavelength limits in a two value array
+#     :type crop_waves: np.array, optional
+#
+#     :param n_cols: Number of columns of the grid plot
+#     :type n_cols: integer
+#
+#     :param n_rows: Number of columns of the grid plot
+#     :type n_rows: integer
+#
+#     :param lines_interval: List of lines or mask file line interval to display on the grid plot. In the later case
+#                            this interval must be a two value array.
+#     :type lines_interval: list
+#
+#     :param y_scale: Y axis scale. The default value (auto) will switch between between linear and logarithmic scale
+#                     strong and weak lines respectively. Use ``linear`` and ``log`` for a fixed scale for all lines.
+#     :type y_scale: str, optional
+#
+#     """
+#
+#     def __init__(self, log_address, input_wave=None, input_flux=None, input_err=None, redshift=0,
+#                  norm_flux=1.0, crop_waves=None, n_cols=10, n_rows=None, lines_interval=None, y_scale='auto'):
+#
+#         # Output file address
+#         self.linesLogAddress = Path(log_address)
+#         self.y_scale = y_scale
+#
+#         # Assign attributes to the parent class
+#         super().__init__(input_wave, input_flux, input_err, redshift, norm_flux, crop_waves)
+#
+#         # Lines log address is provided and we read the DF from it
+#         if Path(self.linesLogAddress).is_file():
+#             self.log = load_lines_log(self.linesLogAddress)
+#
+#         # Lines log not provide code ends
+#         else:
+#             _logger.warning(f'No lines log file found at {log_address}. Leaving the script')
+#             exit()
+#
+#         # Only plotting the lines in the lines interval
+#         self.line_inter = lines_interval
+#         if lines_interval is None:
+#             n_lines = len(self.log.index)
+#             self.target_lines = self.log.index.values
+#
+#         else:
+#             # Array of strings
+#             if isinstance(lines_interval[0], str):
+#                 n_lines = len(lines_interval)
+#                 self.target_lines = np.array(lines_interval, ndmin=1)
+#             # Array of integers
+#             else:
+#                 n_lines = lines_interval[1] - lines_interval[0]
+#                 self.target_lines = self.log[lines_interval[0]:lines_interval[1]].index.values
+#
+#         # Establish the grid shape
+#         if n_lines > n_cols:
+#             if n_rows is None:
+#                 n_rows = int(np.ceil(n_lines / n_cols))
+#         else:
+#             n_cols = n_lines
+#             n_rows = 1
+#
+#         # Adjust the plot theme
+#         PLOT_CONF = STANDARD_PLOT.copy()
+#         AXES_CONF = STANDARD_AXES.copy()
+#         PLOT_CONF['figure.figsize'] = (n_rows * 2, 8)
+#         AXES_CONF.pop('xlabel')
+#
+#         with rc_context(PLOT_CONF):
+#
+#             self.fig, ax = plt.subplots(nrows=n_rows, ncols=n_cols)
+#             self.ax = ax.flatten() if n_lines > 1 else [ax]
+#             self.in_ax = None
+#             self.dict_spanSelec = {}
+#             self.axConf = {}
+#
+#             # Plot function
+#             self.plot_line_mask_selection(logscale=self.y_scale, grid_size=n_rows * n_cols, n_lines=n_lines)
+#             plt.gca().axes.yaxis.set_ticklabels([])
+#
+#             try:
+#                 manager = plt.get_current_fig_manager()
+#                 manager.window.showMaximized()
+#             except:
+#                 print()
+#
+#             # Show the image
+#             save_close_fig_swicth(None, 'tight', self.fig)
+#
+#
+#         return
+#
+#     def plot_line_mask_selection(self, logscale='auto', grid_size=None, n_lines=None):
+#
+#         # Generate plot
+#         for i in range(grid_size):
+#             if i < n_lines:
+#                 line = self.target_lines[i]
+#                 if line in self.log.index:
+#                     self.mask = self.log.loc[line, 'w1':'w6'].values
+#                     self.plot_line_region_i(self.ax[i], line, logscale=logscale)
+#                     self.dict_spanSelec[f'spanner_{i}'] = SpanSelector(self.ax[i],
+#                                                                        self.on_select,
+#                                                                        'horizontal',
+#                                                                        useblit=True,
+#                                                                        rectprops=dict(alpha=0.5, facecolor='tab:blue'))
+#                 else:
+#                     print(f'- WARNING: line {line} not found in the input mask')
+#
+#             # Clear not filled axes
+#             else:
+#                 self.fig.delaxes(self.ax[i])
+#
+#         bpe = self.fig.canvas.mpl_connect('button_press_event', self.on_click)
+#         aee = self.fig.canvas.mpl_connect('axes_enter_event', self.on_enter_axes)
+#
+#         return
+#
+#     def plot_line_region_i(self, ax, lineLabel, limitPeak=5, logscale='auto'):
+#
+#         # Plot line region:
+#         ion, lineWave, latexLabel = label_decomposition(lineLabel, scalar_output=True, units_wave=self.units_wave)
+#
+#         # Decide type of plot
+#         non_nan = (~pd.isnull(self.mask)).sum()
+#
+#         # Incomplete selections
+#         if non_nan < 6:  # selections
+#
+#             # Peak region
+#             idcsLinePeak = (lineWave - limitPeak <= self.wave_rest) & (self.wave_rest <= lineWave + limitPeak)
+#             wavePeak, fluxPeak = self.wave_rest[idcsLinePeak], self.flux[idcsLinePeak]
+#
+#             # Plot region
+#             idcsLineArea = (lineWave - limitPeak * 2 <= self.wave_rest) & (
+#                         lineWave - limitPeak * 2 <= self.mask[3])
+#             waveLine, fluxLine = self.wave_rest[idcsLineArea], self.flux[idcsLineArea]
+#
+#             # Plot the line region
+#             ax.step(waveLine, fluxLine, where='mid')
+#
+#             # Fill the user selections
+#             if non_nan == 2:
+#                 idx1, idx2 = np.searchsorted(self.wave_rest, self.mask[0:2])
+#                 ax.fill_between(self.wave_rest[idx1:idx2], 0.0, self.flux[idx1:idx2], facecolor=self._color_dict['cont_band'],
+#                                 step='mid', alpha=0.5)
+#
+#             if non_nan == 4:
+#                 idx1, idx2, idx3, idx4 = np.searchsorted(self.wave_rest, self.mask[0:4])
+#                 ax.fill_between(self.wave_rest[idx1:idx2], 0.0, self.flux[idx1:idx2], facecolor=self._color_dict['cont_band'],
+#                                 step='mid', alpha=0.5)
+#                 ax.fill_between(self.wave_rest[idx3:idx4], 0.0, self.flux[idx3:idx4], facecolor=self._color_dict['cont_band'],
+#                                 step='mid', alpha=0.5)
+#
+#         # Complete selections
+#         else:
+#
+#             # Get line regions
+#             idcsContLeft = (self.mask[0] <= self.wave_rest) & (self.wave_rest <= self.mask[1])
+#             idcsContRight = (self.mask[4] <= self.wave_rest) & (self.wave_rest <= self.mask[5])
+#
+#             idcsLinePeak = (lineWave - limitPeak <= self.wave_rest) & (self.wave_rest <= lineWave + limitPeak)
+#             idcsLineArea = (self.mask[2] <= self.wave_rest) & (self.wave_rest <= self.mask[3])
+#
+#             waveCentral, fluxCentral = self.wave_rest[idcsLineArea], self.flux[idcsLineArea]
+#             wavePeak, fluxPeak = self.wave_rest[idcsLinePeak], self.flux[idcsLinePeak]
+#
+#             idcsLinePlot = (self.mask[0] - 5 <= self.wave_rest) & (self.wave_rest <= self.mask[5] + 5)
+#             waveLine, fluxLine = self.wave_rest[idcsLinePlot], self.flux[idcsLinePlot]
+#
+#             # Plot the line
+#             ax.step(waveLine, fluxLine, color=self._color_dict['fg'], where='mid')
+#
+#             # Fill the user selections
+#             ax.fill_between(waveCentral, 0, fluxCentral, step="mid", alpha=0.4, facecolor=self._color_dict['line_band'])
+#             ax.fill_between(self.wave_rest[idcsContLeft], 0, self.flux[idcsContLeft], facecolor=self._color_dict['cont_band'],
+#                             step="mid", alpha=0.2)
+#             ax.fill_between(self.wave_rest[idcsContRight], 0, self.flux[idcsContRight], facecolor=self._color_dict['cont_band'],
+#                             step="mid", alpha=0.2)
+#
+#         # Plot format
+#         ax.yaxis.set_major_locator(plt.NullLocator())
+#         ax.xaxis.set_major_locator(plt.NullLocator())
+#
+#         ax.update({'title': lineLabel})
+#         ax.yaxis.set_ticklabels([])
+#         ax.axes.yaxis.set_visible(False)
+#         try:
+#             idxPeakFlux = np.argmax(fluxPeak)
+#             ax.set_ylim(ymin=np.min(fluxLine) / 5, ymax=fluxPeak[idxPeakFlux] * 1.25)
+#
+#             if logscale == 'auto':
+#                 if fluxPeak[idxPeakFlux] > 5 * np.median(fluxLine):
+#                     ax.set_yscale('log')
+#             else:
+#                 if logscale == 'log':
+#                     ax.set_yscale('log')
+#         except:
+#             print(f'fail at {self.line}')
+#
+#
+#         return
+#
+#     def on_select(self, w_low, w_high):
+#
+#         # Check we are not just clicking on the plot
+#         if w_low != w_high:
+#
+#             # Count number of empty entries to determine next step
+#             non_nans = (~pd.isnull(self.mask)).sum()
+#
+#             # Case selecting 1/3 region
+#             if non_nans == 0:
+#                 self.mask[0] = w_low
+#                 self.mask[1] = w_high
+#
+#             # Case selecting 2/3 region
+#             elif non_nans == 2:
+#                 self.mask[2] = w_low
+#                 self.mask[3] = w_high
+#                 self.mask = np.sort(self.mask)
+#
+#             # Case selecting 3/3 region
+#             elif non_nans == 4:
+#                 self.mask[4] = w_low
+#                 self.mask[5] = w_high
+#                 self.mask = np.sort(self.mask)
+#
+#             elif non_nans == 6:
+#                 self.mask = np.sort(self.mask)
+#
+#                 # Caso que se corrija la region de la linea
+#                 if w_low > self.mask[1] and w_high < self.mask[4]:
+#                     self.mask[2] = w_low
+#                     self.mask[3] = w_high
+#
+#                 # Caso que se corrija el continuum izquierdo
+#                 elif w_low < self.mask[2] and w_high < self.mask[2]:
+#                     self.mask[0] = w_low
+#                     self.mask[1] = w_high
+#
+#                 # Caso que se corrija el continuum derecho
+#                 elif w_low > self.mask[3] and w_high > self.mask[3]:
+#                     self.mask[4] = w_low
+#                     self.mask[5] = w_high
+#
+#                 # Case we want to select the complete region
+#                 elif w_low < self.mask[0] and w_high > self.mask[5]:
+#
+#                     # # Remove line from dataframe and save it
+#                     # self.remove_lines_df(self.current_df, self.Current_Label)
+#                     #
+#                     # # Save lines log df
+#                     # self.save_lineslog_dataframe(self.current_df, self.lineslog_df_address)
+#
+#                     # Clear the selections
+#                     # self.mask = np.array([np.nan] * 6)
+#
+#                     print(f'\n-- The line {self.line} mask has been removed')
+#
+#                 else:
+#                     print('- WARNING: Unsucessful line selection:')
+#                     print(f'-- {self.line}: w_low: {w_low}, w_high: {w_high}')
+#
+#             # Check number of measurements after selection
+#             non_nans = (~pd.isnull(self.mask)).sum()
+#
+#             # Proceed to re-measurement if possible:
+#             if non_nans == 6:
+#
+#                 # TODO add option to perform the measurement a new
+#                 # self.clear_fit()
+#                 # self.fit_from_wavelengths(self.line, self.mask, user_cfg={})
+#
+#                 # Parse the line regions to the dataframe
+#                 self.results_to_database(self.line, self.log, fit_conf={}, export_params=[])
+#
+#                 # Save the corrected mask to a file
+#                 self.store_measurement()
+#
+#             # Redraw the line measurement
+#             self.in_ax.clear()
+#             self.plot_line_region_i(self.in_ax, self.line, logscale=self.y_scale)
+#             self.in_fig.canvas.draw()
+#
+#         return
+#
+#     def on_enter_axes(self, event):
+#
+#         # Assign new axis
+#         self.in_fig = event.canvas.figure
+#         self.in_ax = event.inaxes
+#
+#         # TODO we need a better way to index than the latex label
+#         # Recognise line line
+#         idx_line = self.log.index == self.in_ax.get_title()
+#         self.line = self.log.loc[idx_line].index.values[0]
+#         self.mask = self.log.loc[idx_line, 'w1':'w6'].values[0]
+#
+#         # Restore measurements from log
+#         # self.database_to_attr()
+#
+#         # event.inaxes.patch.set_edgecolor('red')
+#         # event.canvas.draw()
+#
+#     def on_click(self, event):
+#
+#         if event.dblclick:
+#             print(self.line)
+#             print(f'{event.button}, {event.x}, {event.y}, {event.xdata}, {event.ydata}')
+#
+#     def store_measurement(self):
+#
+#         # Read file in the stored address
+#         if self.linesLogAddress.is_file():
+#             file_DF = load_lines_log(self.linesLogAddress)
+#
+#             # Add new line to the DF and sort it if it was new
+#             if self.line in file_DF.index:
+#                 file_DF.loc[self.line, 'w1':'w6'] = self.mask
+#             else:
+#                 file_DF.loc[self.line, 'w1':'w6'] = self.mask
+#
+#                 # Sort the lines by theoretical wavelength
+#                 lineLabels = file_DF.index.values
+#                 ion_array, wavelength_array, latexLabel_array = label_decomposition(lineLabels, units_wave=self.units_wave)
+#                 file_DF = file_DF.iloc[wavelength_array.argsort()]
+#
+#         # If the file does not exist (or it is the first time)
+#         else:
+#             file_DF = self.log
+#
+#         # Save to a file
+#         save_line_log(file_DF, self.linesLogAddress)
+#
+#         return
 
 
 class CubeInspector(Spectrum):
 
     def __init__(self, wave, cube_flux, image_bg, image_fg=None, contour_levels=None, color_norm=None,
                  redshift=0, lines_log_address=None, fits_header=None, plt_cfg={}, ax_cfg={},
                  ext_suffix='_LINESLOG', mask_file=None, units_wave='A', units_flux='Flam'):
@@ -808,15 +1107,16 @@
         :type units_flux: str, optional
 
         """
 
         #TODO add _frame argument
 
         # Assign attributes to the parent class
-        super().__init__(input_wave=np.zeros(1), input_flux=np.zeros(1), redshift=redshift, norm_flux=1, units_wave=units_wave, units_flux=units_flux)
+        super().__init__(input_wave=np.zeros(1), input_flux=np.zeros(1), redshift=redshift, norm_flux=1,
+                         units_wave=units_wave, units_flux=units_flux)
 
         # Data attributes
         self.grid_mesh = None
         self.cube_flux = cube_flux
         self.wave = wave
         self.header = fits_header
         self.image_bg = image_bg
@@ -838,15 +1138,15 @@
         self.fig_conf = None
         self.axes_conf = {}
         self.axlim_dict = {}
         self.color_norm = color_norm
         self.mask_color_i = None
         self.key_coords = None
         self.marker = None
-
+        self._color_dict = colorDict
         # Scenario we use the background image also for the contours
         if (image_fg is None) and (contour_levels is not None):
             self.image_fg = image_bg
 
         # Update the axes labels to the units
         AXES_CONF = STANDARD_AXES.copy()
         norm_label = r' $\,/\,{}$'.format(latex_science_float(self.norm_flux)) if self.norm_flux != 1.0 else ''
```

### Comparing `lime-stable-0.9.8/src/lime/workflow.py` & `lime-stable-0.9.9/src/lime/workflow.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,87 @@
 import logging
 import numpy as np
 import pandas as pd
 from pathlib import Path
-from sys import exit
+from astropy.io import fits
 
+from . import Error
 from .model import LineFitting
-from .tools import define_masks, label_decomposition
+from .tools import define_masks, label_decomposition, COORD_ENTRIES
 from .transitions import Line
-from .io import _LOG_EXPORT, _LOG_COLUMNS, load_lines_log, progress_bar
+from .io import _LOG_EXPORT, _LOG_COLUMNS, load_lines_log, progress_bar, load_spatial_masks, log_to_HDU
 
 _logger = logging.getLogger('LiMe')
 
 
-def check_file(input, variable_type):
+def check_file_dataframe(input, variable_type):
 
     if isinstance(input, variable_type):
         output = input
 
     elif Path(input).is_file():
         output = load_lines_log(input)
 
     else:
-        _logger.critical(f'Not file found at {input}.\nPlease introduce a {variable_type} as input or check the'
+        _logger.warning(f'Not file found at {input}.\nPlease introduce a {variable_type} as input or check the'
                          f'file address.')
-        exit()
+        output = None
 
     return output
 
 
-def review_bands(line, emis_wave, cont_wave, limit_narrow=6):
+def check_file_array_mask(var, mask_list=[]):
+
+    # Check if file
+    if isinstance(var, (str, Path)):
+
+        input = Path(var)
+        if input.is_file():
+            mask_dict = load_spatial_masks(var, mask_list)
+        else:
+            raise Error(f'No spatial mask file at {var.as_posix()}')
+
+    # Array
+    elif isinstance(var, (np.ndarray, list)):
+
+        # Re-adjust the variable
+        var = np.ndarray(var, ndmin=3)
+        masks_array = np.squeeze(np.array_split(var, var.shape[0], axis=0))
+
+        # Confirm boolean array
+        if masks_array.dtype != bool:
+            _logger.warning(f'The input mask array should have a boolean variables (True/False)')
+
+        # Incase user gives a str
+        mask_list = [mask_list] if isinstance(mask_list, str) else mask_list
+
+        # Check if there is a mask list
+        if len(mask_list) == 0:
+            mask_list = [f'SPMASK{i}' for i in range(masks_array.shape[0])]
+
+        # Case the number of masks names and arrays is different
+        elif masks_array.shape[0] != len(mask_list):
+            _logger.warning(f'The number of input spatial mask arrays is different than the number of mask names')
+
+        # Everything is fine
+        else:
+            mask_list = mask_list
+
+        # Create mask dict with empty headers
+        mask_dict = dict(zip(mask_list, (masks_array, {})))
+
+    else:
+
+        raise Error(f'Input mask format {type(input)} is not recognized for a mask file. Please declare a fits file, a'
+                    f' numpy array or a list/array of numpy arrays')
+
+    return mask_dict
+
+
+def review_bands(line, emis_wave, cont_wave, limit_narrow=7):
 
     # Review the transition bands before
     emis_band_lengh = emis_wave.size if not np.ma.is_masked(emis_wave) else np.sum(~emis_wave.mask)
     cont_band_length = cont_wave.size if not np.ma.is_masked(cont_wave) else np.sum(~cont_wave.mask)
 
     if emis_band_lengh / emis_wave.size < 0.5:
         _logger.warning(f'The line band for {line.label} has very few valid pixels')
@@ -42,17 +91,22 @@
 
     # Store error very small mask
     if emis_band_lengh <= 1:
         if line.observations == 'no':
             line.observations = 'Small_line_band'
         else:
             line.observations += '-Small_line_band'
-        _logger.warning(f'- Line {line.label} mask band is too small ({emis_wave.size} value array): {emis_wave}')
 
-    # Check if the line is very narrow for fit initial conditions
+        if np.ma.is_masked(emis_wave):
+            length = np.sum(~emis_wave.mask)
+        else:
+            length = emis_band_lengh
+        _logger.warning(f'The  {line.label} band is too small ({length} length array): {emis_wave}')
+
+    # Check if the line is very narrow for fit initial conditions # TODO change logic to number of pixels above cont level
     line._narrow_check = True if emis_band_lengh <= limit_narrow else False
 
     return
 
 
 def import_line_kinematics(line, z_cor, log, units_wave):
 
@@ -105,27 +159,19 @@
                         line._fit_conf[f'{param_label_child}_err'] = param_value[1]
 
     return
 
 
 def results_to_log(line, log, norm_flux, units_wave, export_params=_LOG_EXPORT):
 
-    # # Recover line data
-    # if line.blended_check:
-    #     line_components = line.profile_label.split('-')
-    # else:
-    #     line_components = np.array([line.label], ndmin=1)
-    #
-    # ion, waveRef, latexLabel = label_decomposition(line_components, comp_dict=line._fit_conf, units_wave=units_wave)
-
     # Loop through the line components
     for i, comp in enumerate(line.list_comps):
 
         # Convert current measurement to a pandas series container
-        log.loc[comp, ['ion', 'wavelength', 'latex_label']] = line.ion[i], line.wave[i], line.latex[i]
+        log.loc[comp, ['ion', 'wavelength', 'latex_label']] = line.ion[i], line.wavelength[i], line.latex[i]
         log.loc[comp, 'w1':'w6'] = line.mask
 
         # Treat every line
         for param in export_params:
 
             # Get component parameter
             if _LOG_COLUMNS[param][2]:
@@ -138,15 +184,15 @@
                 param_value = param_value * norm_flux
 
             log.loc[comp, param] = param_value
 
     return
 
 
-class LineTreatment(LineFitting):
+class SpecTreatment(LineFitting):
 
     def __init__(self, spectrum):
 
         # Instantiate the dependencies
         LineFitting.__init__(self)
 
         # Lime spectrum object with the scientific data
@@ -241,80 +287,174 @@
 
         return
 
     def frame(self, bands_df, fit_conf=None,  label=None, fit_method='leastsq', emission_check=True, cont_from_bands=True,
               temp=10000.0, progress_output=None, plot_fits=False):
 
         # Check if the lines table is a dataframe or a file
-        bands_df = check_file(bands_df, pd.DataFrame)
+        bands_df = check_file_dataframe(bands_df, pd.DataFrame)
+
+        if bands_df is not None:
+
+            # Crop the analysis to the target lines
+            if label is not None:
+                idcs = bands_df.index.isin(label)
+                line_list = bands_df.loc[idcs].index.values
+            else:
+                line_list = bands_df.index.values
+
+            # Loop text decision
+            bar_output = True if progress_output == 'bar' else False
+
+            # Loop through the lines
+            n_lines = len(line_list)
+            for i in np.arange(n_lines):
+
+                line = line_list[i]
+
+                # Progress message
+                if progress_output is not None:
+                    if bar_output:
+                        progress_bar(i+1, n_lines, post_text=f'of lines')
+                    else:
+                        print(f'{i+1}/{n_lines}) {line}')
+
+                # Fit the lines
+                self.band(line, bands_df.loc[line, 'w1':'w6'].values, fit_conf, fit_method, emission_check,
+                          cont_from_bands, temp)
+
+                if plot_fits:
+                    self._spec.plot.line()
 
-        # Crop the analysis to the target lines
-        if label is not None:
-            idcs = bands_df.index.isin(label)
-            line_list = bands_df.loc[idcs].index.values
         else:
-            line_list = bands_df.index.values
+            _logger.info(f'Not input dataframe. Lines were not measured')
+
+
+        return
+
+
+class CubeTreatment(LineFitting):
+
+    def __init__(self, cube):
+
+        # Instantiate the dependencies
+        LineFitting.__init__(self)
+
+        # Lime spectrum object with the scientific data
+        self._cube = cube
+        self._spec = None
+
+    def spatial_mask(self, spatial_mask, mask_name_list=[], bands_frame=None, fit_conf={}, output_log=None, fit_method='leastsq',
+                     line_detection=False, emission_check=True, cont_from_bands=True, temp=10000, n_save=100,
+                     progress_output=None, log_ext_suffix='_LINESLOG', **kwargs):
+
+        # Check if the mask variable is a file or an array
+        mask_dict = check_file_array_mask(spatial_mask, mask_name_list)
+
+        # Check if the lines table is a dataframe or a file
+        if bands_frame is not None:
+            bands_frame = check_file_dataframe(bands_frame, pd.DataFrame)
+        else:
+            raise(Error(f'No input bands frame or file in the spatial mask line fitting'))
+
+        # Check if output log
+        if output_log is None:
+            raise(Error(f'No output log file address to save the line measurements log'))
+        else:
+            output_log = Path(output_log)
+            if not output_log.parent.is_dir():
+                raise(Error(f'The folder of the output log file does not exist at {output_log}'))
+
+        # Unpack mask dictionary
+        mask_list = np.array(list(mask_dict.keys()))
+        mask_data_list = list(mask_dict.values())
+
+        # Determine the spaxels to treat at each mask
+        total_spaxels, spaxels_dict = 0, {}
+        for idx_mask, mask_data in enumerate(mask_data_list):
+            spa_mask, hdr_mask = mask_data
+            idcs_spaxels = np.argwhere(spa_mask)
+
+            total_spaxels += len(idcs_spaxels)
+            spaxels_dict[idx_mask] = idcs_spaxels
 
         # Loop text decision
         bar_output = True if progress_output == 'bar' else False
 
-        # Loop through the lines
-        n_lines = len(line_list)
-        for i in np.arange(n_lines):
+        # Spaxel counter to save the data everytime n_save is reached
+        spax_counter = 0
+
+        # HDU_container
+        hdul_log = fits.HDUList([fits.PrimaryHDU()])
 
-            line = line_list[i]
+        # Loop through the masks
+        n_masks = len(mask_list)
+        for i in np.arange(n_masks):
+
+            mask_name = mask_list[i]
+            mask_hdr = mask_data_list[i][1]
+            idcs_spaxels = spaxels_dict[i]
 
             # Progress message
             if progress_output is not None:
                 if bar_output:
-                    progress_bar(i+1, n_lines, post_text=f'of lines')
+                    progress_bar(i + 1, n_masks, post_text=f'of masks')
+                else:
+                    print(f'{i + 1}/{n_masks}) {mask_name}')
+
+            # Get mask line fitting_conf
+            mask_conf = fit_conf.get(f'{mask_name}_line_fitting', fit_conf)
+
+            # WCS header data
+            hdr_coords = {}
+            for key in COORD_ENTRIES:
+                if key in mask_hdr:
+                    hdr_coords[key] = mask_hdr[key]
+            hdr_coords = fits.Header(hdr_coords)
+
+            # Loop through the spaxels
+            n_spaxels = idcs_spaxels.shape[0]
+            for j in np.arange(n_spaxels):
+
+                idx_j, idx_i = idcs_spaxels[j]
+                spaxel_label = f'{idx_j}-{idx_i}'
+
+                # Get the spaxel fitting configuration
+                spaxel_conf = fit_conf.get(f'{spaxel_label}_line_fitting', mask_conf)
+
+                # Progress message
+                if progress_output is not None:
+                    if bar_output:
+                        progress_bar(j + 1, n_spaxels, post_text=f'of masks')
+                    else:
+                        print(f'{j + 1}/{n_spaxels}) {idx_j}-{idx_i}')
+
+                # Get spaxel data
+                spaxel = self._cube.get_spaxel(idx_j, idx_i, spaxel_label)
+
+                # Detect the lines
+                if line_detection:
+                    bands_frame = spaxel.line_detection(bands_log=bands_frame)
                 else:
-                    print(f'{i+1}/{n_lines}) {line}')
+                    bands_frame = bands_frame
 
-            # Fit the lines
-            self.band(line, bands_df.loc[line, 'w1':'w6'].values, fit_conf, fit_method, emission_check, cont_from_bands,
-                      temp)
-
-            if plot_fits:
-                self._spec.plot.line()
-
-        # self.band(line, bands_df.loc[line, 'w1':'w6'].values, fit_conf, fit_method, emission_check,
-        #                   cont_from_bands, temp)
-
-
-        #
-        # # Loop through the lines
-        # if progress_output is None:
-        #
-        #     # No message:
-        #     for line in line_list:
-        #         self.band(line, bands_df.loc[line, 'w1':'w6'].values, fit_conf, fit_method, emission_check,
-        #                   cont_from_bands, temp)
-        #
-        # # Progress bar
-        # elif progress_output == 'bar':
-        #     n_lines = line_list.size
-        #
-        #     for i, line in enumerate(line_list):
-        #         progress_bar(i, n_lines, post_text=f'of lines')
-        #         self.band(line, bands_df.loc[line, 'w1':'w6'].values, fit_conf, fit_method, emission_check,
-        #                   cont_from_bands, temp)
-        #
-        # # Line labels and numbers
-        # elif progress_output == 'labels':
-        #
-        #     n_lines = line_list.size
-        #     for i, line in enumerate(line_list):
-        #         print(f'{i}/{n_lines}) {line}')
-        #         self.band(line, bands_df.loc[line, 'w1':'w6'].values, fit_conf, fit_method, emission_check,
-        #                   cont_from_bands, temp)
-        #
-        # # Line name and number:
-        # else:
-        #
-        #     for line in line_list:
-        #         self.band(line, bands_df.loc[line, 'w1':'w6'].values, fit_conf, fit_method, emission_check,
-        #                   cont_from_bands, temp)
+                # Fit the lines
+                spaxel.fit.frame(bands_frame, spaxel_conf, None, fit_method, emission_check, cont_from_bands,
+                                 temp, progress_output=None, plot_fits=None)
+
+                # Save to a fits file
+                linesHDU = log_to_HDU(spaxel.log, ext_name=f'{spaxel_label}{log_ext_suffix}', header_dict=hdr_coords)
+                hdul_log.append(linesHDU)
+
+                # Save the data every 100 spaxels
+                if spax_counter < n_save:
+                    spax_counter += 1
+                else:
+                    spax_counter = 0
+                    hdul_log.writeto(output_log, overwrite=True, output_verify='fix')
 
+            # Save the log at each new mask
+            hdul_log.writeto(output_log, overwrite=True, output_verify='fix')
 
         return
 
+
```

### Comparing `lime-stable-0.9.8/src/lime_stable.egg-info/PKG-INFO` & `lime-stable-0.9.9/src/lime_stable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lime-stable
-Version: 0.9.8
+Version: 0.9.9
 Summary: Line measuring algorithm for ionized nebulae
 Home-page: https://github.com/Vital-Fernandez/lime
 Author: Vital Fernandez
 Author-email: vital.fernandez@userena.cl
 License: GNU
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

