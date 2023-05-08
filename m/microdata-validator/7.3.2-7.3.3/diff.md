# Comparing `tmp/microdata-validator-7.3.2.tar.gz` & `tmp/microdata_validator-7.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microdata-validator-7.3.2.tar", max compression
+gzip compressed data, was "microdata_validator-7.3.3.tar", max compression
```

## Comparing `microdata-validator-7.3.2.tar` & `microdata_validator-7.3.3.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0     1102 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/LICENSE
--rw-r--r--   0        0        0     1707 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/README.md
--rw-r--r--   0        0        0     6760 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/microdata_validator/__init__.py
--rw-r--r--   0        0        0     4424 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/microdata_validator/adapter/local_storage.py
--rw-r--r--   0        0        0     5603 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/microdata_validator/components/temporal_attributes.py
--rw-r--r--   0        0        0      776 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/microdata_validator/components/unit_id_types.py
--rw-r--r--   0        0        0     1581 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/microdata_validator/components/unit_type_variables/BK_HELSESTASJONSKONSULTASJON.json
--rw-r--r--   0        0        0     2091 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/microdata_validator/components/unit_type_variables/FAMILIE.json
--rw-r--r--   0        0        0     1525 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/microdata_validator/components/unit_type_variables/FORETAK.json
--rw-r--r--   0        0        0     2124 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/microdata_validator/components/unit_type_variables/HUSHOLDNING.json
--rw-r--r--   0        0        0     1429 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/microdata_validator/components/unit_type_variables/JOBB.json
--rw-r--r--   0        0        0     1378 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/microdata_validator/components/unit_type_variables/KJORETOY.json
--rw-r--r--   0        0        0   232471 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/microdata_validator/components/unit_type_variables/KOMMUNE.json
--rw-r--r--   0        0        0     1242 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/microdata_validator/components/unit_type_variables/KURS.json
--rw-r--r--   0        0        0     1202 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/microdata_validator/components/unit_type_variables/PERSON.json
--rw-r--r--   0        0        0     1535 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/microdata_validator/components/unit_type_variables/VIRKSOMHET.json
--rw-r--r--   0        0        0     1166 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/microdata_validator/components/unit_type_variables/__init__.py
--rw-r--r--   0        0        0      414 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/microdata_validator/exceptions/__init__.py
--rw-r--r--   0        0        0      872 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/microdata_validator/model/__init__.py
--rw-r--r--   0        0        0     5781 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/microdata_validator/model/metadata.py
--rw-r--r--   0        0        0     7854 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/microdata_validator/steps/dataset_reader.py
--rw-r--r--   0        0        0     7837 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/microdata_validator/steps/dataset_validator.py
--rw-r--r--   0        0        0     1663 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/microdata_validator/steps/metadata_inliner.py
--rw-r--r--   0        0        0     1682 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/microdata_validator/steps/metadata_reader.py
--rw-r--r--   0        0        0      652 2023-05-04 11:30:33.007422 microdata-validator-7.3.2/pyproject.toml
--rw-r--r--   0        0        0     2698 2023-05-04 11:31:05.562569 microdata-validator-7.3.2/setup.py
--rw-r--r--   0        0        0     2417 2023-05-04 11:31:05.563434 microdata-validator-7.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-05-08 12:02:34.301743 microdata_validator-7.3.3/LICENSE
+-rw-r--r--   0        0        0     1707 2023-05-08 12:02:34.301743 microdata_validator-7.3.3/README.md
+-rw-r--r--   0        0        0     6877 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/__init__.py
+-rw-r--r--   0        0        0     4424 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/adapter/local_storage.py
+-rw-r--r--   0        0        0     5603 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/temporal_attributes.py
+-rw-r--r--   0        0        0      776 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_id_types.py
+-rw-r--r--   0        0        0     1581 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/BK_HELSESTASJONSKONSULTASJON.json
+-rw-r--r--   0        0        0     2091 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/FAMILIE.json
+-rw-r--r--   0        0        0     1525 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/FORETAK.json
+-rw-r--r--   0        0        0     2124 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/HUSHOLDNING.json
+-rw-r--r--   0        0        0     1429 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/JOBB.json
+-rw-r--r--   0        0        0     1378 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/KJORETOY.json
+-rw-r--r--   0        0        0   232471 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/KOMMUNE.json
+-rw-r--r--   0        0        0     1242 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/KURS.json
+-rw-r--r--   0        0        0     1202 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/PERSON.json
+-rw-r--r--   0        0        0     1535 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/VIRKSOMHET.json
+-rw-r--r--   0        0        0     1166 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/__init__.py
+-rw-r--r--   0        0        0      414 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/exceptions/__init__.py
+-rw-r--r--   0        0        0      872 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/model/__init__.py
+-rw-r--r--   0        0        0     5781 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/model/metadata.py
+-rw-r--r--   0        0        0     7854 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/steps/dataset_reader.py
+-rw-r--r--   0        0        0     7837 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/steps/dataset_validator.py
+-rw-r--r--   0        0        0     1663 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/steps/metadata_inliner.py
+-rw-r--r--   0        0        0     1682 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/microdata_validator/steps/metadata_reader.py
+-rw-r--r--   0        0        0      682 2023-05-08 12:02:34.305743 microdata_validator-7.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2468 1970-01-01 00:00:00.000000 microdata_validator-7.3.3/PKG-INFO
```

### Comparing `microdata-validator-7.3.2/LICENSE` & `microdata_validator-7.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.2/README.md` & `microdata_validator-7.3.3/README.md`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.2/microdata_validator/__init__.py` & `microdata_validator-7.3.3/microdata_validator/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     # Make paths for input and ref directory
     input_directory_path = Path(input_directory)
     if metadata_ref_directory is not None:
         metadata_ref_directory = Path(metadata_ref_directory)
 
     # Run readers and validator
     data_errors = []
+    unexpected_exception_occured = False
     try:
         metadata_file_path = (
             input_directory_path / dataset_name / f'{dataset_name}.json'
         )
         metadata_dict = metadata_inliner.run_inliner(
             metadata_file_path,
             metadata_ref_directory
@@ -67,18 +68,19 @@
         data_errors = dataset_validator.run_validator(
             working_directory_path, dataset_name
         )
     except InvalidDatasetException as e:
         data_errors = e.errors
     except Exception as e:
         # Raise unexpected exceptions to user
+        unexpected_exception_occured = True
         raise e
     finally:
         # Delete temporary files
-        if not keep_temporary_files:
+        if not keep_temporary_files or unexpected_exception_occured:
             local_storage.clean_up_temporary_files(
                 dataset_name,
                 working_directory_path,
                 delete_working_directory=working_directory_was_generated
             )
     return data_errors
```

### Comparing `microdata-validator-7.3.2/microdata_validator/adapter/local_storage.py` & `microdata_validator-7.3.3/microdata_validator/adapter/local_storage.py`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.2/microdata_validator/components/temporal_attributes.py` & `microdata_validator-7.3.3/microdata_validator/components/temporal_attributes.py`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.2/microdata_validator/components/unit_id_types.py` & `microdata_validator-7.3.3/microdata_validator/components/unit_id_types.py`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.2/microdata_validator/components/unit_type_variables/BK_HELSESTASJONSKONSULTASJON.json` & `microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/BK_HELSESTASJONSKONSULTASJON.json`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.2/microdata_validator/components/unit_type_variables/FAMILIE.json` & `microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/FAMILIE.json`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.2/microdata_validator/components/unit_type_variables/FORETAK.json` & `microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/FORETAK.json`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.2/microdata_validator/components/unit_type_variables/HUSHOLDNING.json` & `microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/HUSHOLDNING.json`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.2/microdata_validator/components/unit_type_variables/JOBB.json` & `microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/JOBB.json`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.2/microdata_validator/components/unit_type_variables/KJORETOY.json` & `microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/KJORETOY.json`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.2/microdata_validator/components/unit_type_variables/KOMMUNE.json` & `microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/KOMMUNE.json`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.2/microdata_validator/components/unit_type_variables/KURS.json` & `microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/KURS.json`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.2/microdata_validator/components/unit_type_variables/PERSON.json` & `microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/PERSON.json`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.2/microdata_validator/components/unit_type_variables/VIRKSOMHET.json` & `microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/VIRKSOMHET.json`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.2/microdata_validator/components/unit_type_variables/__init__.py` & `microdata_validator-7.3.3/microdata_validator/components/unit_type_variables/__init__.py`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.2/microdata_validator/model/__init__.py` & `microdata_validator-7.3.3/microdata_validator/model/__init__.py`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.2/microdata_validator/model/metadata.py` & `microdata_validator-7.3.3/microdata_validator/model/metadata.py`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.2/microdata_validator/steps/dataset_reader.py` & `microdata_validator-7.3.3/microdata_validator/steps/dataset_reader.py`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.2/microdata_validator/steps/dataset_validator.py` & `microdata_validator-7.3.3/microdata_validator/steps/dataset_validator.py`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.2/microdata_validator/steps/metadata_inliner.py` & `microdata_validator-7.3.3/microdata_validator/steps/metadata_inliner.py`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.2/microdata_validator/steps/metadata_reader.py` & `microdata_validator-7.3.3/microdata_validator/steps/metadata_reader.py`

 * *Files identical despite different names*

### Comparing `microdata-validator-7.3.2/pyproject.toml` & `microdata_validator-7.3.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "microdata-validator"
-version = "7.3.2"
+version = "7.3.3"
 description = "Python package for validating datasets in the microdata platform"
 authors = ["microdata-developers"]
 license = "Apache-2.0"
 repository = 'https://github.com/statisticsnorway/microdata-validator'
 readme = 'README.md'
 
 [tool.poetry.dependencies]
 python = ">=3.7.2,<4.0"
 pydantic = "^1.10.4"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+pytest-mock = "^3.10.0"
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
 pytest-dotenv = "^0.5.2"
 black = {version = "^22.3.0", allow-prereleases = true}
 pylint = "^2.15.3"
 pycodestyle = "^2.9.1"
```

### Comparing `microdata-validator-7.3.2/PKG-INFO` & `microdata_validator-7.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: microdata-validator
-Version: 7.3.2
+Version: 7.3.3
 Summary: Python package for validating datasets in the microdata platform
 Home-page: https://github.com/statisticsnorway/microdata-validator
 License: Apache-2.0
 Author: microdata-developers
 Requires-Python: >=3.7.2,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
 Project-URL: Repository, https://github.com/statisticsnorway/microdata-validator
 Description-Content-Type: text/markdown
 
 # microdata-validator
 
 Python package for validating datasets in the microdata platform.
```

