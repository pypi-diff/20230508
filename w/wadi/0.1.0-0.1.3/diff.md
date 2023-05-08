# Comparing `tmp/wadi-0.1.0.tar.gz` & `tmp/wadi-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wadi-0.1.0.tar", last modified: Mon Apr 17 10:48:16 2023, max compression
+gzip compressed data, was "wadi-0.1.3.tar", last modified: Mon May  8 07:37:10 2023, max compression
```

## Comparing `wadi-0.1.0.tar` & `wadi-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:48:16.219895 wadi-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-17 10:48:05.000000 wadi-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-17 10:48:16.219895 wadi-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-17 10:48:05.000000 wadi-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 10:48:16.219895 wadi-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-17 10:48:05.000000 wadi-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:48:16.215895 wadi-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-17 10:48:05.000000 wadi-0.1.0/tests/test_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:48:16.215895 wadi-0.1.0/wadi/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-17 10:48:05.000000 wadi-0.1.0/wadi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-04-17 10:48:05.000000 wadi-0.1.0/wadi/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-04-17 10:48:05.000000 wadi-0.1.0/wadi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-04-17 10:48:05.000000 wadi-0.1.0/wadi/dataobject.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-04-17 10:48:05.000000 wadi-0.1.0/wadi/filereader.py
--rw-r--r--   0 runner    (1001) docker     (123)    17300 2023-04-17 10:48:05.000000 wadi-0.1.0/wadi/harmonizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-04-17 10:48:05.000000 wadi-0.1.0/wadi/infotable.py
--rw-r--r--   0 runner    (1001) docker     (123)    28719 2023-04-17 10:48:05.000000 wadi-0.1.0/wadi/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-04-17 10:48:05.000000 wadi-0.1.0/wadi/unitconverter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-04-17 10:48:05.000000 wadi-0.1.0/wadi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 10:48:16.219895 wadi-0.1.0/wadi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-17 10:48:16.000000 wadi-0.1.0/wadi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-17 10:48:16.000000 wadi-0.1.0/wadi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 10:48:16.000000 wadi-0.1.0/wadi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-17 10:48:16.000000 wadi-0.1.0/wadi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-17 10:48:16.000000 wadi-0.1.0/wadi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:37:10.103058 wadi-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-08 07:36:56.000000 wadi-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-08 07:37:10.103058 wadi-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-08 07:36:56.000000 wadi-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 07:37:10.103058 wadi-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-08 07:36:56.000000 wadi-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:37:10.099058 wadi-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-08 07:36:56.000000 wadi-0.1.3/tests/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:37:10.099058 wadi-0.1.3/wadi/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 07:36:56.000000 wadi-0.1.3/wadi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-05-08 07:36:56.000000 wadi-0.1.3/wadi/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-05-08 07:36:56.000000 wadi-0.1.3/wadi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7617 2023-05-08 07:36:56.000000 wadi-0.1.3/wadi/dataobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-08 07:36:56.000000 wadi-0.1.3/wadi/documentation_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-05-08 07:36:56.000000 wadi-0.1.3/wadi/filereader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17600 2023-05-08 07:36:56.000000 wadi-0.1.3/wadi/harmonizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-05-08 07:36:56.000000 wadi-0.1.3/wadi/infotable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29659 2023-05-08 07:36:56.000000 wadi-0.1.3/wadi/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-05-08 07:36:56.000000 wadi-0.1.3/wadi/unitconverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-05-08 07:36:56.000000 wadi-0.1.3/wadi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:37:10.103058 wadi-0.1.3/wadi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-08 07:37:10.000000 wadi-0.1.3/wadi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-08 07:37:10.000000 wadi-0.1.3/wadi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 07:37:10.000000 wadi-0.1.3/wadi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-08 07:37:10.000000 wadi-0.1.3/wadi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-08 07:37:10.000000 wadi-0.1.3/wadi.egg-info/top_level.txt
```

### Comparing `wadi-0.1.0/LICENSE` & `wadi-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wadi-0.1.0/setup.py` & `wadi-0.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
 
 setup(
     name='wadi',
-    version='0.1.0',
+    version='0.1.3',
     packages=find_packages(exclude=['tests*']),
     license='MIT',
     description='Generic importer for water quality data of the (Dutch) water laboratory',
     long_description=read('README.md'),
-    long_description_content_type="text/x-rst",
+    long_description_content_type="text/markdown",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Other Audience',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
```

### Comparing `wadi-0.1.0/wadi/api_utils.py` & `wadi-0.1.3/wadi/api_utils.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.0/wadi/base.py` & `wadi-0.1.3/wadi/base.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.0/wadi/dataobject.py` & `wadi-0.1.3/wadi/dataobject.py`

 * *Files 26% similar despite different names*

```diff
@@ -135,26 +135,54 @@
             self._infotable.list_keys(), self._infotable.list_dict1_item("unit")
         )
         self._infotable.update_items(info_table_items)
 
         # Harmonize
         self._converted_df = self.harmonizer._execute(self._infotable)
 
-    def get_converted_dataframe(self):
-        """
-        This method returns the converted DataFrame.
+    def get_converted_dataframe(self,
+            include_units=True,
+            force_conversion=False,
+        ):
+        """
+        This method converts the input data based on the specified
+        name and unit maps and harmonizer, and returns the result
+        as a DataFrame.
+
+        Parameters
+        ----------
+        include_units : bool, optional
+            When True the DataFrame's columns will be a MultiIndex
+            that contains both the feature aliases and their units.
+            When set to False a DataFrame is returned of which the 
+            columns simply correspond to the feature aliases and 
+            the units are discarded. The latter option is useful when
+            the DataFrame is intended for further processing in HGC.
+            Default: True.
+        force_conversion: bool, optional
+            When True, the function will always map and harmonize
+            the data before it returns the DataFrame. When False,
+            the results from any previously executed data mapping
+            and harmonizing are returned, when present. Default:
+            False. 
 
         Returns
         ----------
         result : DataFrame
             The converted DataFrame.
         """
-        self._execute()
-        return self._converted_df
+        if (self._converted_df is None) or (force_conversion == True):
+            self._execute()
 
+        if include_units == True:
+            return self._converted_df
+        else:
+            level0_cols = self._converted_df.columns.get_level_values(0)
+            return self._converted_df.set_axis(level0_cols, axis='columns')
+    
     def get_imported_dataframe(self):
         """
         This method returns the imported DataFrame (that is, the data 
         'as read').
 
         Returns
         ----------
@@ -163,18 +191,18 @@
         """
         if self._imported_df is None:
             self._execute(import_only=True)
         return self._imported_df
 
     def get_imported_names(self):
         """
-        This method returns the imported DataFrame (that is, the data 
-        'as read').
+        This method returns the names of the features
+        in the imported DataFrame.
 
         Returns
         ----------
-        result : DataFrame
-            The imported DataFrame.
+        result : list
+            A list with feature names in the imported DataFrame.
         """
         if self._infotable is None:
             self._execute(import_only=True)
         return self._infotable.list_dict1_item('name')
```

### Comparing `wadi-0.1.0/wadi/filereader.py` & `wadi-0.1.3/wadi/filereader.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
     def __call__(
         self,
         file_path,
         format="stacked",  # str, immutable
         c_dict=None,
         mask=None,
+        lod_column=None,
         pd_reader="read_excel",  # str, immutable
         **kwargs,
     ):
 
         """
         This method provides an interface for the user to set the
         attributes that determine the FileReader object behavior.
@@ -66,17 +67,26 @@
             format. Permissible formats are defined in VALID_FORMATS.
             The 'gef' format is not implemented (yet). Default: 'stacked'
         c_dict : dict, optional
             Only used when the format is 'stacked'. This dictionary maps
             column names in the file to the compulsory column names defined
             in REQUIRED_COLUMNS_S. Default: DEFAULT_C_DICT
         mask : str, optional
-            Name of the column that contains True/False labels, sometimes
-            used to indicate if a reported value is below or above the
-            detection limit. Only used when the format is 'stacked'.
+            Name of the column that contains True/False labels. These sometimes
+            occur in stacked data files to indicate if a reported value is 
+            below or above the detection limit. If a valid column name is 
+            specified, the values marked with `False` are filtered out from 
+            the converted DataFrame. Only used when the format is 'stacked'.
+            Default: None
+        lod_column : str, optional
+            Name of the column that contains information about whether the 
+            reported measurement value is below or above the limit of 
+            detection (LOD). If a valid column name is specified, the
+            symbol is prefixed to the measurement value.
+            Only used when the format is 'stacked'. Default: None
         pd_reader : str, optional
             Name of the Pandas function to read the file. Must be a valid
             function name. While all functions implemented in Pandas could
             be used in principle, the design of WaDI has not been tested
             for functions other than read_excel and read_csv. Default:
             'read_excel'.
         **kwargs: dict, optionalt
@@ -96,14 +106,15 @@
         self._format = format  # for use in read_data
 
         # Use c_dict to look up the names of the columns with the compulsory
         # names for stacked data.
         self._c_dict = c_dict or DEFAULT_C_DICT
 
         self._mask = mask
+        self._lod_column = lod_column
 
         self._kwargs = copy.deepcopy(vars()["kwargs"])  # deepcopy just to be sure
 
     def _execute(self):
         """
         This method imports the data from a file format readable by
         Pandas. Before calling the Pandas reader function, it checks
@@ -141,19 +152,22 @@
                 kwargs.pop("datatype")
                 self._warn("Argument 'datatype' is ignored when format is 'stacked'.")
 
         # Call _read_file to import the (blocks of) data into a single 
         # DataFrame.
         df, units, datatypes = self._read_file(self._file_path, self._pd_reader, blocks)
 
-        # Use the values in the column with name 'mask' to
-        # hide the values below the detection limit from view.
-        # Still to implement: Convert them to a lower than format.
-        if self._mask is not None:
-            df = df.loc[df[self._mask]]
+        if self._format == "stacked":
+            # Use the values in the column with name 'mask' to
+            # hide the values labelled as False from view.
+            if self._mask is not None:
+                df = df.loc[df[self._mask]]
+
+            if self._lod_column is not None:
+                df[self._c_dict["Values"]] = df[self._lod_column] + df[self._c_dict["Values"]].astype(str)
 
         # Create the InfoTable dictionary that stores views to the
         # imported data as well as additional information (units,
         # data type)
         infotable = InfoTable(
             df,
             self._format,
```

### Comparing `wadi-0.1.0/wadi/harmonizer.py` & `wadi-0.1.3/wadi/harmonizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 import re
-
 from wadi.base import WadiBaseClass
+from wadi.mapper import MapperDict
 from wadi.utils import check_if_nested_list
 from wadi.unitconverter import UnitConverter
 
 # Suppress performance warnings for that occur during harmonize because
 # DataFrame can contain lots of NaNs
 import warnings
 
@@ -177,26 +177,30 @@
         Returns
         -------
         df : DataFrame
             DataFrame with the transformed data.
         """
         self._msg("Harmonizing", header=True)
 
+        if (self._target_units == "hgc"):
+               hgc_units_dict = MapperDict._create_hgc_units_dict()
+
         # Initialize the DataFrame to be created. Uses the target_index
         # in the InfoTable that ensures that the sampleids for
         # stacked data are uniquely defined. For wide data the
         # target_index is None, and the DataFrame will have an
         # ordinary RangeIndex.
         df = pd.DataFrame(index=infotable.target_index)
 
         # Create empty dictionaries that will be filled with values
         # of alias_n and alias_u, respectively, to be able to assign
         # the right values to the DataFrame columns at the end.
         column_header_dict = {}
         units_header_dict = {}
+
         # Iterate over items in the InfoTable. Recall that InfoTable
         # is a nested dict and key_0 is used to indicate the level-0
         # keys and dict_1 (their corresponding values) are the
         # level-1 dictionaries. This terminology is used here as well
         # for consistency with the code in infotable.py.
         for key_0, dict_1 in infotable.items():
             # Do not process items that the user has indicated
@@ -250,15 +254,15 @@
                     self._warn(
                         f"Duplicate sampleids found for {key_0}. Keeping only first occurrence."
                     )
 
             # Rows with NaNs can be dropped for faster processing,
             # since all Series share a common index, they are easily
             # pieced together at the end into a new DataFrame.
-            values = pd.to_numeric(values.dropna(), errors="ignore")
+            values = values.dropna()
 
             # The column name in the new DataFrame will be the item's
             # alias...
             alias_n = dict_1["alias_n"]
             self._msg(f" - Alias: {alias_n}")
             # ... and the units will be the item's unit alias. Note 
             # that alias_u will be replaced by Pint's pretty format
@@ -280,24 +284,26 @@
                 # Returns a Pint Quantity objects qs (for the units) 
                 # and mw (for the molar mass).
                 u_str = dict_1["u_str"]
                 qs, mw_formula, msg = self._unit_converter._str2pint(alias_n, u_str)
                 self._log(msg)
                 
                 # Infer the unit alias from the short pretty
-                # format string representation of qs.  qs may be None
+                # format string representation of qs. qs may be None
                 # if the units were not properly identified by Pint.
                 if (qs is not None):
                     alias_u = f"{qs.units:~P}"
 
                 if self._convert_units:
                     # The user may wish to override the general
                     # target units, in which case the desired
                     # units were passed in the dict override_units.
-                    if key_0 in self._override_units:
+                    if (self._target_units == "hgc"):
+                        target_units = hgc_units_dict.get(alias_n)
+                    elif key_0 in self._override_units:
                         target_units = self._override_units[key_0]
                     else:
                         target_units = self._target_units
 
                     # Call the UnitConverter object's get_uc method,
                     # which returns the target units as qt and the 
                     # unit conversion factor as uc. Both are Pint
@@ -321,14 +327,15 @@
                         # Write a message to the log file about the failed unit
                         # conversion attempt.
                         self._log(
                             f" - Could not convert from {u_str} to {target_units} for {alias_n}."
                         )
 
                 # Convert the measurement values using _convert_values.
+                values = pd.to_numeric(values, errors="ignore")
                 values = values.apply(self._convert_values, conversion_factor=uc_factor)
 
             # Add the values Series as a column to the new DataFrame.
             df[key_0] = values
 
             # Replace the original name and units by their aliases.
             column_header_dict[key_0] = alias_n
```

### Comparing `wadi-0.1.0/wadi/infotable.py` & `wadi-0.1.3/wadi/infotable.py`

 * *Files identical despite different names*

### Comparing `wadi-0.1.0/wadi/mapper.py` & `wadi-0.1.3/wadi/mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     "Ö": "o",
     "ö": "o",
     "ï": "i",
     "Ï": "i",
     "μ": "u",
     "µ": "u",
     "%": "percentage",
+    "°C": "degC",
+    "°F": "degF",
 }
 DEFAULT_FILTERSTR = [
     "gefiltreerd",
     "na filtratie",
     "filtered",
     "filtration",
     " gef",
@@ -116,31 +118,53 @@
         ----------
         result : class instance
             An instance of the UserDict class containing the
             imported data.
         """
         # The json file resides in the parent directory of the
         # current module's py file. The __file__ attribute returns
-        # the pathname of the current py file and .parents[1]
+        # the pathname of the current py file and .parent
         # provides its parent directory.
-        filepath = Path(__file__).parents[1]
+        filepath = Path(__file__).parent
         # Import the file into a DataFrame.
         dfj = pd.read_json(Path(filepath, "default_feature_map.json"))
         # Use the DataFrame's explode function to transform any keys
         # that are a list (or list-like) into a row. The corresponding
         # value is duplicated for each list element that becomes a row.
         dfd = dfj[[keys, values]].explode(keys).dropna()
         # Convert the DataFrame to a dictionary
         rv_dict = dfd.set_index(keys)[values].to_dict()
         # Values are lists, gives problems when they become aliases so
         # keep only first list element if there are multiple.
         rv_dict = {k: str(v[0]) for k, v in rv_dict.items()}
         return cls(rv_dict)
 
     @classmethod
+    def _create_hgc_units_dict(cls):
+        """
+        This method initializes the class by reading the csv
+        files in the folder hgc_constants, which contain
+        the feature names and their target units.
+
+        Returns
+        ----------
+        result : class instance
+            An instance of the UserDict class containing the
+            imported data.
+        """
+
+        rv_dict = {}
+        filepath = Path(Path(__file__).parents[1], "hgc_constants")
+        for fname in ["atoms.csv", "ions.csv", "other_than_concentrations.csv"]:
+            df = pd.read_csv(Path(filepath, fname), comment='#')
+            rv_dict = {**rv_dict, **df.set_index("feature")["unit"].to_dict()}
+
+        return cls(rv_dict)
+
+    @classmethod
     def pubchem_cas_dict(
         cls,
         strings,
         src_lang=None,
         max_attempts=10,
     ):
         """
@@ -328,20 +352,25 @@
 
         Returns
         ----------
         result : str
             String that provides an overview of the keys and the values of
             the mapping dictionary.
         """
-        rv = "(Please note that long mapping dictionaries may be truncated when printed to the screen.)\n"
+        max_lines = 10
+        rv = f"This dictionary contains {len(self.data)} elements.\n"
+        if len(self.data) > max_lines:
+            rv += f"Only the first {max_lines} elements are shown.\n"
         rv += (
             f"This mapping dictionary contains the following names and their aliases:\n"
         )
-        for key, value in self.data.items():
+        for i, (key, value) in enumerate(self.data.items()):
             rv += f" - {key} --> {value}\n"
+            if i > max_lines:
+                break
 
         return rv
 
 
 class Mapper(WadiBaseClass):
     """
     WaDI class that implements the operations to map feature names
```

### Comparing `wadi-0.1.0/wadi/unitconverter.py` & `wadi-0.1.3/wadi/unitconverter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import molmass as mm
 from molmass.molmass import FormulaError
 from pint import UnitRegistry
-from pint.errors import DimensionalityError, UndefinedUnitError
+from pint.errors import DimensionalityError, UndefinedUnitError, OffsetUnitCalculusError
 
 from wadi.api_utils import get_pubchem_molecular_weight
 
 # DEFAULT_RE_DICT0 is the default dictionary to create a regular 
 # expression for matching chemical concentration units. It is 
 # designed to recognize variants such as mg/l, mg N/l or mg/l N. 
 # Each element is a list, the first element being the character set 
@@ -219,29 +219,36 @@
             The target units
         uc : Pint Quantity object
             The unit conversion factor.
         """
         try:
             # Convert the target_units string to a Pint Quantity object
             qt = self._ureg(target_units)
+
             # Determine the molecular mass in g/mol.
-            mw = self._get_mw(mw_formula)
-            if mw is None:
-                mw = get_pubchem_molecular_weight(mw_formula)
+            mw = None
+            # Only try to determine the molecular mass if the target units
+            # are molar units, which can be identified using the Pint
+            # Quantity's object dimensionality property. If this is the case
+            # a key called '[substance]' will be present.
+            if ('[substance]' in qt.dimensionality.keys()) and (mw_formula is not None):
+                mw = self._get_mw(mw_formula)
+                if mw is None:
+                    mw = get_pubchem_molecular_weight(mw_formula)
 
             # Use the source units 'to' method to determine the unit
             # conversion factor.
             if mw is None:
                 uc = qs.to(qt)
             else:
                 uc = qs.to(qt, "chemistry", mw=mw)
 
             # Divide uc by qs to get the right dimensions
             uc /= qs
-        except (AttributeError, DimensionalityError) as e:
+        except (AttributeError, DimensionalityError, OffsetUnitCalculusError) as e:
             qt = None
             uc = None
 
         return qt, uc
 
     def _str2pint(
         self,
@@ -304,9 +311,9 @@
             # Write a message to the log file
             msg = f" - Successfully parsed unit '{u_str}' with pint for {name}"
 
             return uq, mw_formula, msg
         except (AttributeError, TypeError, UndefinedUnitError, ValueError):
             # When an error occurs, write a message to the log file and
             # return empty return values.
-            msg = f" - Failed to parse unit '{u_str}' with pint for {name}"
+            msg = f" - Failed to parse unit '{u_str}' with Pint for {name}"
             return None, None, msg
```

### Comparing `wadi-0.1.0/wadi/utils.py` & `wadi-0.1.3/wadi/utils.py`

 * *Files identical despite different names*

