# Comparing `tmp/ms_imputedhours_core-0.3.7.tar.gz` & `tmp/ms_imputedhours_core-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_imputedhours_core-0.3.7.tar", max compression
+gzip compressed data, was "ms_imputedhours_core-0.3.8.tar", max compression
```

## Comparing `ms_imputedhours_core-0.3.7.tar` & `ms_imputedhours_core-0.3.8.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0    35149 2023-05-02 11:35:11.139471 ms_imputedhours_core-0.3.7/LICENSE
--rw-r--r--   0        0        0     2401 2023-05-02 11:35:11.139471 ms_imputedhours_core-0.3.7/README.md
--rw-r--r--   0        0        0       22 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/__init__.py
--rw-r--r--   0        0        0     3238 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/agreements/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/agreements/__tests__/__init__.py
--rw-r--r--   0        0        0     3228 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/agreements/__tests__/test_agreements.py
--rw-r--r--   0        0        0     2472 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/__tests__/__init__.py
--rw-r--r--   0        0        0     9750 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/__tests__/test_employee.py
--rw-r--r--   0        0        0     7081 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/__tests__/__init__.py
--rw-r--r--   0        0        0     9019 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/__tests__/test_data.py
--rw-r--r--   0        0        0    10493 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/bigquery.py
--rw-r--r--   0        0        0      171 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/constants.py
--rw-r--r--   0        0        0        0 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/__tests__/__init__.py
--rw-r--r--   0        0        0     4491 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py
--rw-r--r--   0        0        0     6206 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py
--rw-r--r--   0        0        0      776 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py
--rw-r--r--   0        0        0      654 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/alert.py
--rw-r--r--   0        0        0     3599 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/bigquery.py
--rw-r--r--   0        0        0      423 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/dates.py
--rw-r--r--   0        0        0        0 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/transformers/__init__.py
--rw-r--r--   0        0        0     3828 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/transformers/hours.py
--rw-r--r--   0        0        0      203 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/office/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/office/__tests__/__init__.py
--rw-r--r--   0        0        0      678 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/ms_imputedhours_core/office/__tests__/test_office.py
--rw-r--r--   0        0        0      950 2023-05-02 11:35:11.143471 ms_imputedhours_core-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     3069 1970-01-01 00:00:00.000000 ms_imputedhours_core-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/LICENSE
+-rw-r--r--   0        0        0     2401 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/README.md
+-rw-r--r--   0        0        0       22 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/__init__.py
+-rw-r--r--   0        0        0     3238 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/agreements/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/agreements/__tests__/__init__.py
+-rw-r--r--   0        0        0     3228 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/agreements/__tests__/test_agreements.py
+-rw-r--r--   0        0        0     2472 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/__tests__/__init__.py
+-rw-r--r--   0        0        0     9750 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/__tests__/test_employee.py
+-rw-r--r--   0        0        0     7158 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/__tests__/__init__.py
+-rw-r--r--   0        0        0     6373 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/__tests__/test_capacity.py
+-rw-r--r--   0        0        0     9019 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/__tests__/test_data.py
+-rw-r--r--   0        0        0    10493 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/bigquery.py
+-rw-r--r--   0        0        0      171 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/constants.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/__tests__/__init__.py
+-rw-r--r--   0        0        0     4491 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py
+-rw-r--r--   0        0        0     6206 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py
+-rw-r--r--   0        0        0      776 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py
+-rw-r--r--   0        0        0      654 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/alert.py
+-rw-r--r--   0        0        0     3599 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/bigquery.py
+-rw-r--r--   0        0        0      423 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/dates.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/transformers/__init__.py
+-rw-r--r--   0        0        0     3828 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/transformers/hours.py
+-rw-r--r--   0        0        0      203 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/office/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/office/__tests__/__init__.py
+-rw-r--r--   0        0        0      678 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/ms_imputedhours_core/office/__tests__/test_office.py
+-rw-r--r--   0        0        0      950 2023-05-08 09:49:19.398794 ms_imputedhours_core-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     3069 1970-01-01 00:00:00.000000 ms_imputedhours_core-0.3.8/PKG-INFO
```

### Comparing `ms_imputedhours_core-0.3.7/LICENSE` & `ms_imputedhours_core-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.7/README.md` & `ms_imputedhours_core-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.7/ms_imputedhours_core/agreements/__init__.py` & `ms_imputedhours_core-0.3.8/ms_imputedhours_core/agreements/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.7/ms_imputedhours_core/agreements/__tests__/test_agreements.py` & `ms_imputedhours_core-0.3.8/ms_imputedhours_core/agreements/__tests__/test_agreements.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/__init__.py` & `ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/__tests__/test_employee.py` & `ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/__tests__/test_employee.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/__init__.py` & `ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,18 @@
     get_imputed_hours,
     get_out_date_imputations,
     get_successfactor_all_data,
 )
 from ms_imputedhours_core.employee.data.helpers.alert import (
     should_exclude_employee,
 )
+from ms_imputedhours_core.employee.data.helpers.dates import (
+    get_first_day,
+    get_last_day,
+)
 from ms_imputedhours_core.employee.data.transformers.hours import (
     group_task_by_email,
     group_task_by_outdated,
     transform_all_capacities,
     transform_successfactor_all_data,
 )
 from ms_imputedhours_core.office import get_real_office_name
@@ -36,16 +40,18 @@
     'successfactor_data': EMPTY_SUCCESSFACTOR_DATA,
 }
 GOOGLE_API_MAX_REQUESTS_PER_SEG = 60
 
 
 def get_all_employees_monthly_data_by_office(date, office_name):
     data = {}
-    agreement_hours = Agreements(AGREEMENTS_SPREADSHEET_ID).get_hours_by_month(
-        date.month, date.year, office_name
+    first_date = get_first_day(date)
+    last_day = get_last_day(date)
+    agreement_hours = Agreements(AGREEMENTS_SPREADSHEET_ID).get_hours_by_range(
+        first_date, last_day, office_name
     )
     successfactor_all_data = transform_successfactor_all_data(
         get_successfactor_all_data(office_name, only_actives=False)
     )
     if successfactor_all_data:
         office_emails = successfactor_all_data.keys()
         current_month_data = group_task_by_email(
@@ -76,17 +82,18 @@
                 successfactor_data, all_employee_ftes.get(email), date
             )
 
             real_capacity = calculate_real_capacity(
                 agreement_hours,
                 successfactor_data.get('hiring_date'),
                 successfactor_data.get('enddate'),
-                date,
-                date,
+                first_date,
+                last_day,
                 fte,
+                True,
             )
 
             # Updating fte value
             successfactor_data['FTE'] = fte
 
             if email not in data.keys():
                 data[email] = {
@@ -168,17 +175,14 @@
             'real_capacity': employee_real_capacity,
             'current_capacity': employee_current_capacity,
             'current_percentage_hours_imputed': capacity_percentage,
             'supervisor': successfactor_data['supervisor'],
             'name': successfactor_data['name'],
         }
 
-        if email == 'daniel.guell@makingscience.com':
-            print(employees_data[email])
-            
     return employees_data
 
 
 def get_all_imputations_per_day(from_date, to_date):
     current_month_data = group_task_by_email(
         get_imputed_hours(from_date, to_date)
     )
@@ -212,9 +216,9 @@
             if supervisor_email not in employees_data.keys():
                 employees_data[supervisor_email] = {}
 
             employees_data[supervisor_email][email] = {
                 'data': current_data[email],
                 'name': successfactor_data['name'],
             }
-    # TODO:Fix this
+
     return employees_data
```

### Comparing `ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/__tests__/test_data.py` & `ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/__tests__/test_data.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/bigquery.py` & `ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py` & `ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py` & `ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py` & `ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/alert.py` & `ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/alert.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/helpers/bigquery.py` & `ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/helpers/bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.7/ms_imputedhours_core/employee/data/transformers/hours.py` & `ms_imputedhours_core-0.3.8/ms_imputedhours_core/employee/data/transformers/hours.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.7/ms_imputedhours_core/office/__tests__/test_office.py` & `ms_imputedhours_core-0.3.8/ms_imputedhours_core/office/__tests__/test_office.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.7/pyproject.toml` & `ms_imputedhours_core-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-imputedhours-core"
-version = "0.3.7"
+version = "0.3.8"
 description = "Python library to collect data about jira imputed hours and employee agreements"
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_imputedhours_core"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `ms_imputedhours_core-0.3.7/PKG-INFO` & `ms_imputedhours_core-0.3.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-imputedhours-core
-Version: 0.3.7
+Version: 0.3.8
 Summary: Python library to collect data about jira imputed hours and employee agreements
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

