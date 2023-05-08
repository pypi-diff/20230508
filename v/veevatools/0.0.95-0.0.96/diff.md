# Comparing `tmp/veevatools-0.0.95.tar.gz` & `tmp/veevatools-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veevatools-0.0.95.tar", last modified: Thu Apr 13 20:49:57 2023, max compression
+gzip compressed data, was "veevatools-0.0.96.tar", last modified: Mon May  8 01:33:45 2023, max compression
```

## Comparing `veevatools-0.0.95.tar` & `veevatools-0.0.96.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 20:49:57.475044 veevatools-0.0.95/
--rw-rw-rw-   0        0        0      658 2022-05-07 04:14:46.000000 veevatools-0.0.95/LICENSE.txt
--rw-rw-rw-   0        0        0       38 2022-05-08 00:45:13.000000 veevatools-0.0.95/MANIFEST.in
--rw-rw-rw-   0        0        0     6648 2023-04-13 20:49:57.475044 veevatools-0.0.95/PKG-INFO
--rw-rw-rw-   0        0        0     6291 2022-06-29 21:08:45.000000 veevatools-0.0.95/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 20:49:57.459041 veevatools-0.0.95/salesforce/
--rw-rw-rw-   0        0        0       73 2022-05-19 04:32:15.000000 veevatools-0.0.95/salesforce/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:49:57.461041 veevatools-0.0.95/salesforce/custom_exceptions/
--rw-rw-rw-   0        0        0      142 2022-06-24 18:09:22.000000 veevatools-0.0.95/salesforce/custom_exceptions/__init__.py
--rw-rw-rw-   0        0        0     3416 2022-05-16 20:22:53.000000 veevatools-0.0.95/salesforce/custom_exceptions/salesforce_exceptions.py
--rw-rw-rw-   0        0        0      274 2022-05-19 04:43:58.000000 veevatools-0.0.95/salesforce/decorators.py
--rw-rw-rw-   0        0        0    94293 2023-04-13 20:49:22.000000 veevatools-0.0.95/salesforce/salesforce.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:49:57.464041 veevatools-0.0.95/salesforce/utilities/
--rw-rw-rw-   0        0        0      302 2022-09-01 00:09:33.000000 veevatools-0.0.95/salesforce/utilities/__init__.py
--rw-rw-rw-   0        0        0      704 2022-06-30 05:29:51.000000 veevatools-0.0.95/salesforce/utilities/async_utils.py
--rw-rw-rw-   0        0        0     3897 2022-06-28 03:58:32.000000 veevatools-0.0.95/salesforce/utilities/df_utils.py
--rw-rw-rw-   0        0        0     2112 2023-03-09 15:52:01.000000 veevatools-0.0.95/salesforce/utilities/sf_query_processors.py
--rw-rw-rw-   0        0        0      763 2023-04-13 20:49:57.476043 veevatools-0.0.95/setup.cfg
--rw-rw-rw-   0        0        0       39 2022-05-07 03:46:02.000000 veevatools-0.0.95/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:49:57.468042 veevatools-0.0.95/veevanetwork/
--rw-rw-rw-   0        0        0       40 2022-06-08 00:43:06.000000 veevatools-0.0.95/veevanetwork/__init__.py
--rw-rw-rw-   0        0        0        0 2022-06-16 04:00:20.000000 veevatools-0.0.95/veevanetwork/api.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:49:57.470042 veevatools-0.0.95/veevanetwork/custom_exceptions/
--rw-rw-rw-   0        0        0      148 2022-06-23 17:12:46.000000 veevatools-0.0.95/veevanetwork/custom_exceptions/__init__.py
--rw-rw-rw-   0        0        0     3870 2022-06-20 23:49:28.000000 veevatools-0.0.95/veevanetwork/custom_exceptions/veevanetwork_exceptions.py
--rw-rw-rw-   0        0        0   122066 2022-06-16 02:54:23.000000 veevatools-0.0.95/veevanetwork/network_api_v25.json
--rw-rw-rw-   0        0        0    81646 2022-12-02 05:41:49.000000 veevatools-0.0.95/veevanetwork/veevanetwork.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:49:57.473041 veevatools-0.0.95/veevatools.egg-info/
--rw-rw-rw-   0        0        0     6648 2023-04-13 20:49:57.000000 veevatools-0.0.95/veevatools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      792 2023-04-13 20:49:57.000000 veevatools-0.0.95/veevatools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 20:49:57.000000 veevatools-0.0.95/veevatools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      136 2023-04-13 20:49:57.000000 veevatools-0.0.95/veevatools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       35 2023-04-13 20:49:57.000000 veevatools-0.0.95/veevatools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 20:49:57.475044 veevatools-0.0.95/veevavault/
--rw-rw-rw-   0        0        0       36 2022-06-08 00:45:04.000000 veevatools-0.0.95/veevavault/__init__.py
--rw-rw-rw-   0        0        0     9177 2023-03-15 17:03:59.000000 veevatools-0.0.95/veevavault/veevavault.py
+drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-08 01:33:45.629585 veevatools-0.0.96/
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      651 2022-10-24 16:14:29.000000 veevatools-0.0.96/LICENSE.txt
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)       37 2022-10-24 16:14:29.000000 veevatools-0.0.96/MANIFEST.in
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     6385 2023-05-08 01:33:45.629846 veevatools-0.0.96/PKG-INFO
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     6079 2022-10-24 16:14:29.000000 veevatools-0.0.96/README.md
+drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-08 01:33:45.612831 veevatools-0.0.96/salesforce/
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)       72 2022-10-24 16:14:29.000000 veevatools-0.0.96/salesforce/__init__.py
+drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-08 01:33:45.614184 veevatools-0.0.96/salesforce/custom_exceptions/
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      139 2022-10-24 16:14:29.000000 veevatools-0.0.96/salesforce/custom_exceptions/__init__.py
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     3345 2022-10-24 16:14:29.000000 veevatools-0.0.96/salesforce/custom_exceptions/salesforce_exceptions.py
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      268 2022-10-24 16:14:29.000000 veevatools-0.0.96/salesforce/decorators.py
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)   104150 2023-05-08 01:26:39.000000 veevatools-0.0.96/salesforce/salesforce.py
+drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-08 01:33:45.616949 veevatools-0.0.96/salesforce/utilities/
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      295 2022-10-24 16:14:29.000000 veevatools-0.0.96/salesforce/utilities/__init__.py
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      685 2022-10-24 16:14:29.000000 veevatools-0.0.96/salesforce/utilities/async_utils.py
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     3827 2022-10-24 16:14:29.000000 veevatools-0.0.96/salesforce/utilities/df_utils.py
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     2055 2023-05-03 02:20:42.000000 veevatools-0.0.96/salesforce/utilities/sf_query_processors.py
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      757 2023-05-08 01:33:45.631214 veevatools-0.0.96/setup.cfg
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)       37 2022-10-24 16:14:29.000000 veevatools-0.0.96/setup.py
+drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-08 01:33:45.621230 veevatools-0.0.96/veevanetwork/
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)       40 2022-10-24 16:14:29.000000 veevatools-0.0.96/veevanetwork/__init__.py
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)        0 2022-10-24 16:14:29.000000 veevatools-0.0.96/veevanetwork/api.py
+drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-08 01:33:45.622832 veevatools-0.0.96/veevanetwork/custom_exceptions/
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      145 2022-10-24 16:14:29.000000 veevatools-0.0.96/veevanetwork/custom_exceptions/__init__.py
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     3793 2022-10-24 16:14:29.000000 veevatools-0.0.96/veevanetwork/custom_exceptions/veevanetwork_exceptions.py
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)   122066 2022-10-24 16:14:29.000000 veevatools-0.0.96/veevanetwork/network_api_v25.json
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)    80088 2023-01-30 16:08:51.000000 veevatools-0.0.96/veevanetwork/veevanetwork.py
+drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-08 01:33:45.627445 veevatools-0.0.96/veevatools.egg-info/
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     6385 2023-05-08 01:33:45.000000 veevatools-0.0.96/veevatools.egg-info/PKG-INFO
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      792 2023-05-08 01:33:45.000000 veevatools-0.0.96/veevatools.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)        1 2023-05-08 01:33:45.000000 veevatools-0.0.96/veevatools.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)      166 2023-05-08 01:33:45.000000 veevatools-0.0.96/veevatools.egg-info/requires.txt
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)       35 2023-05-08 01:33:45.000000 veevatools-0.0.96/veevatools.egg-info/top_level.txt
+drwxr-xr-x   0 michaelpay-mbpr16   (502) staff       (20)        0 2023-05-08 01:33:45.628894 veevatools-0.0.96/veevavault/
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)       36 2022-10-24 16:14:29.000000 veevatools-0.0.96/veevavault/__init__.py
+-rw-r--r--   0 michaelpay-mbpr16   (502) staff       (20)     8954 2023-03-06 16:42:47.000000 veevatools-0.0.96/veevavault/veevavault.py
```

### Comparing `veevatools-0.0.95/LICENSE.txt` & `veevatools-0.0.96/LICENSE.txt`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022 Veeva Systems, Inc. All Rights Reserved
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES 
-OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE 
-LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR 
+Copyright (c) 2022 Veeva Systems, Inc. All Rights Reserved
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES 
+OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE 
+LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR 
 IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `veevatools-0.0.95/PKG-INFO` & `veevatools-0.0.96/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,226 +1,212 @@
-Metadata-Version: 2.1
-Name: veevatools
-Version: 0.0.95
-Summary: Veeva tools library for accelerating Veeva Systems Internal Tools development
-Home-page: https://github.com/michaelpay
-Author: Michael Pay
-Author-email: monickenish@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-[![Downloads](https://pepy.tech/badge/veevatools)](https://pepy.tech/project/veevatools)
-
-# Introduction
-
-This python package is a set of Salesforce.com, Veeva Network, and Veeva Vault libraries, scripts, and functions used to help expedite the development of Veeva Tools.
-<br/>
-<br/>
-
-# Installation / Requirements
-
-Ensure you have **at least Python version 3.10** installed.
-To Check your installation version, type the following commands in the terminal (MacOs) / command prompt (Windows):
-```
-python --version
-```
-To install python, go to https://www.python.org/ then navigate to the download page of your Operating System.
-
-![Screenshot 2022-06-24 140724](https://user-images.githubusercontent.com/59848012/175649491-0eafdef7-acd2-4631-85cb-f9dee8630b04.png)
-
-You will need to have Packager Installer for Python (pip) installed. To install pip, run the following command in the terminal (MacOs) / command prompt (Windows):
-
-```
-curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
-python3 get-pip.py
-```
-To install the Veeva Tools library:
-
-```
-pip install veevatools
-```
-To upgrade to the latest version of Veeva Tools library:
-```
-pip install veevatools --upgrade
-```
-
-# Overview
-
-The Veeva Tools package currently contains 3 major components:
-## Salesforce library
-
-### Authentication:
-
-```python
-from salesforce import Sf
-from pandas import pd
-sf = Sf()
-sf.authenticate(
-    sfUsername='yourname@salesforce.com',
-    sfPassword='password123',
-    sfOrgId='00D2C0000008jIK',
-    isSandbox= false
-    )
-```
-> Sidenote on Pandas DataFrames: <br/>
-Pandas DataFrame (pd) is used to prepare the data for import (i.e. create, update methods) and additional export methods such as pd.to_excel() in order to save the output into an Excel file.<br/>
-Additionally, Complex data manipuation (joins, merges, groupbys, filters)and data analytics (describe, statistical analysis) can all be performed using Pandas. <br />
-To learn more about Pandas DataFrames, go to the [Pandas documentation](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html)
-<br \>
-> Or just Google tutorials on Pandas DataFrames. 
-[This YouTube playlist by Corey Schafer](https://www.youtube.com/watch?v=ZyhVh-qRZPA&list=PL-osiE80TeTsWmV9i9c58mdDCSskIFdDS&ab_channel=CoreySchafer)
-provides an excellent starting point into the world of Pandas!
-
-<br/>
-
-### Data methods:
-The salesforce class (Sf) contains methods that can help you interact with data and metadata components:
-<br/>
-#### **Query**
-
-```python
-account_recordtypes = sf.query("SELECT Id, Name, SobjectType from RecordType WHERE SobjectType = 'Account'")]
-
-account_recordtypes
-```
-
-`Return -> pd.DataFrame():`
-|    |                 Id |                      Name | SobjectType |
-|---:|-------------------:|--------------------------:|------------:|
-|  0 | 012f4000001ArT3AAK |          Professional_vod |     Account |
-|  1 | 012f4000001ArT4AAK |           Institution_vod |     Account |
-|  2 | 012f4000001ArT5AAK |                   MCO_vod |     Account |
-|  3 | 012f4000001ArT6AAK |          Organization_vod |     Account |
-|  4 | 012f4000001ArWzAAK |              Hospital_vod |     Account |
-
-> Sidenote: <br />
-You can use any Pandas (pd) methods on the return value of the query output. For example <br/>```account_recordtypes.to_excel("Account RecordTypes.xlsx")``` <br/>
-Will save the results of the DataFrame into an Excel file.
-
-<br/>
-
-### **Create**
-```python
-## Takes a DataFrame of CRM records and creates records in CRM
-
-account_records = pd.DataFrame([{'FirstName': 'Test', 'LastName': 'Account'}, {'FirstName': 'Test2', 'LastName': 'Account2'}])
-
-result = sf.create('Account', account_records)
-
-result
-```
-`Return -> pd.DataFrame():`
-|   | success | created |                 Id |
-|--:|--------:|--------:|-------------------:|
-| 0 |    True |    True | 0010r00000tF7L1AAK |
-| 1 |    True |    True | 0010r00000tF7L2AAK |
-
-<br/>
-
-### Update
-```python
-### Takes a dataframe that contains at least the Id column
-### and any other column to be updated, for example, FirstName
-update_account_name = pd.DataFrame(
-    [{'FirstName': 'Updated', 'Id': '0010r00000tF7L1AAK'},
-     {'FirstName': 'Name', 'Id': '0010r00000tF7L2AAK'}]
-    )
-
-result = sf.update('Account', update_account_name)
-
-result
-```
-`Return -> pd.DataFrame()`
-|   | success | created |                 Id |
-|--:|--------:|--------:|-------------------:|
-| 0 |    True |   False | 0010r00000tF7L1AAK |
-| 1 |    True |   False | 0010r00000tF7L2AAK |
-<br/>
-
-### Upsert
-```python
-### Takes a dataframe that contains an external ID column
-### and any other column to be updated, for example, Name
-### if the external ID matches an existing record,
-### the account is updated, otherwise, a new record is created
-
-upsert_account = pd.DataFrame(
-    [{'NET_External_Id__c': '242977178138969088', 'Name': 'Updated Hospital Name'},
-     {'NET_External_Id__c': '555579769212255555', 'Name': 'Create New Hospital'}]
-    )
-
-result = sf.upsert(object_api='Account', external_id_field_api='NET_External_Id__c', record_dataframe=upsert_account)
-
-result
-```
-`Return -> pd.DataFrame()`
-|   | success | created |                 id |
-|--:|--------:|--------:|-------------------:|
-| 0 |    True |   False | 001f400000PKOrwAAH |
-| 1 |    True |    True | 0010r00000tF7stAAC |
-
-<br/>
-
-### Delete
-```python
-### Takes a dataframe that contains the Id column
-### deletes records listed based on their SFID.
-
-delete_account = pd.DataFrame([{'Id': '0010r00000tF7stAAC'}, {'Id': '001f400000PKOrwAAH'}])
-
-result = sf.delete(object_api='Account', record_dataframe=delete_account)
-
-result
-```
-`Return -> pd.DataFrame()`
-
-|   | success | created |                 Id |
-|--:|--------:|--------:|-------------------:|
-| 0 |    True |   False | 0010r00000tF7stAAC |
-| 1 |    True |   False | 001f400000PKOrwAAH |
-
-<br/>
-
-### Read Metadata
-```python
-###
-
-```
-<br/>
-
-### Create Metadata
-```python
-###
-
-```
-<br/>
-
-### Update Metadata
-```python
-###
-
-```
-<br/>
-
-### Rename Metadata
-```python
-###
-
-```
-<br/>
-
-### Delete Metadata
-```python
-###
-
-```
-<br/>
-
-### List MetaData
-```python
-###
-
-```
-
-
+[![Downloads](https://pepy.tech/badge/veevatools)](https://pepy.tech/project/veevatools)
+
+# Introduction
+
+This python package is a set of Salesforce.com, Veeva Network, and Veeva Vault libraries, scripts, and functions used to help expedite the development of Veeva Tools.
+<br/>
+<br/>
+
+# Installation / Requirements
+
+Ensure you have **at least Python version 3.10** installed.
+To Check your installation version, type the following commands in the terminal (MacOs) / command prompt (Windows):
+```
+python --version
+```
+To install python, go to https://www.python.org/ then navigate to the download page of your Operating System.
+
+![Screenshot 2022-06-24 140724](https://user-images.githubusercontent.com/59848012/175649491-0eafdef7-acd2-4631-85cb-f9dee8630b04.png)
+
+You will need to have Packager Installer for Python (pip) installed. To install pip, run the following command in the terminal (MacOs) / command prompt (Windows):
+
+```
+curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
+python3 get-pip.py
+```
+To install the Veeva Tools library:
+
+```
+pip install veevatools
+```
+To upgrade to the latest version of Veeva Tools library:
+```
+pip install veevatools --upgrade
+```
+
+# Overview
+
+The Veeva Tools package currently contains 3 major components:
+## Salesforce library
+
+### Authentication:
+
+```python
+from salesforce import Sf
+from pandas import pd
+sf = Sf()
+sf.authenticate(
+    sfUsername='yourname@salesforce.com',
+    sfPassword='password123',
+    sfOrgId='00D2C0000008jIK',
+    isSandbox= false
+    )
+```
+> Sidenote on Pandas DataFrames: <br/>
+Pandas DataFrame (pd) is used to prepare the data for import (i.e. create, update methods) and additional export methods such as pd.to_excel() in order to save the output into an Excel file.<br/>
+Additionally, Complex data manipuation (joins, merges, groupbys, filters)and data analytics (describe, statistical analysis) can all be performed using Pandas. <br />
+To learn more about Pandas DataFrames, go to the [Pandas documentation](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html)
+<br \>
+> Or just Google tutorials on Pandas DataFrames. 
+[This YouTube playlist by Corey Schafer](https://www.youtube.com/watch?v=ZyhVh-qRZPA&list=PL-osiE80TeTsWmV9i9c58mdDCSskIFdDS&ab_channel=CoreySchafer)
+provides an excellent starting point into the world of Pandas!
+
+<br/>
+
+### Data methods:
+The salesforce class (Sf) contains methods that can help you interact with data and metadata components:
+<br/>
+#### **Query**
+
+```python
+account_recordtypes = sf.query("SELECT Id, Name, SobjectType from RecordType WHERE SobjectType = 'Account'")]
+
+account_recordtypes
+```
+
+`Return -> pd.DataFrame():`
+|    |                 Id |                      Name | SobjectType |
+|---:|-------------------:|--------------------------:|------------:|
+|  0 | 012f4000001ArT3AAK |          Professional_vod |     Account |
+|  1 | 012f4000001ArT4AAK |           Institution_vod |     Account |
+|  2 | 012f4000001ArT5AAK |                   MCO_vod |     Account |
+|  3 | 012f4000001ArT6AAK |          Organization_vod |     Account |
+|  4 | 012f4000001ArWzAAK |              Hospital_vod |     Account |
+
+> Sidenote: <br />
+You can use any Pandas (pd) methods on the return value of the query output. For example <br/>```account_recordtypes.to_excel("Account RecordTypes.xlsx")``` <br/>
+Will save the results of the DataFrame into an Excel file.
+
+<br/>
+
+### **Create**
+```python
+## Takes a DataFrame of CRM records and creates records in CRM
+
+account_records = pd.DataFrame([{'FirstName': 'Test', 'LastName': 'Account'}, {'FirstName': 'Test2', 'LastName': 'Account2'}])
+
+result = sf.create('Account', account_records)
+
+result
+```
+`Return -> pd.DataFrame():`
+|   | success | created |                 Id |
+|--:|--------:|--------:|-------------------:|
+| 0 |    True |    True | 0010r00000tF7L1AAK |
+| 1 |    True |    True | 0010r00000tF7L2AAK |
+
+<br/>
+
+### Update
+```python
+### Takes a dataframe that contains at least the Id column
+### and any other column to be updated, for example, FirstName
+update_account_name = pd.DataFrame(
+    [{'FirstName': 'Updated', 'Id': '0010r00000tF7L1AAK'},
+     {'FirstName': 'Name', 'Id': '0010r00000tF7L2AAK'}]
+    )
+
+result = sf.update('Account', update_account_name)
+
+result
+```
+`Return -> pd.DataFrame()`
+|   | success | created |                 Id |
+|--:|--------:|--------:|-------------------:|
+| 0 |    True |   False | 0010r00000tF7L1AAK |
+| 1 |    True |   False | 0010r00000tF7L2AAK |
+<br/>
+
+### Upsert
+```python
+### Takes a dataframe that contains an external ID column
+### and any other column to be updated, for example, Name
+### if the external ID matches an existing record,
+### the account is updated, otherwise, a new record is created
+
+upsert_account = pd.DataFrame(
+    [{'NET_External_Id__c': '242977178138969088', 'Name': 'Updated Hospital Name'},
+     {'NET_External_Id__c': '555579769212255555', 'Name': 'Create New Hospital'}]
+    )
+
+result = sf.upsert(object_api='Account', external_id_field_api='NET_External_Id__c', record_dataframe=upsert_account)
+
+result
+```
+`Return -> pd.DataFrame()`
+|   | success | created |                 id |
+|--:|--------:|--------:|-------------------:|
+| 0 |    True |   False | 001f400000PKOrwAAH |
+| 1 |    True |    True | 0010r00000tF7stAAC |
+
+<br/>
+
+### Delete
+```python
+### Takes a dataframe that contains the Id column
+### deletes records listed based on their SFID.
+
+delete_account = pd.DataFrame([{'Id': '0010r00000tF7stAAC'}, {'Id': '001f400000PKOrwAAH'}])
+
+result = sf.delete(object_api='Account', record_dataframe=delete_account)
+
+result
+```
+`Return -> pd.DataFrame()`
+
+|   | success | created |                 Id |
+|--:|--------:|--------:|-------------------:|
+| 0 |    True |   False | 0010r00000tF7stAAC |
+| 1 |    True |   False | 001f400000PKOrwAAH |
+
+<br/>
+
+### Read Metadata
+```python
+###
+
+```
+<br/>
+
+### Create Metadata
+```python
+###
+
+```
+<br/>
+
+### Update Metadata
+```python
+###
+
+```
+<br/>
+
+### Rename Metadata
+```python
+###
+
+```
+<br/>
+
+### Delete Metadata
+```python
+###
+
+```
+<br/>
+
+### List MetaData
+```python
+###
+
+```
```

### Comparing `veevatools-0.0.95/salesforce/custom_exceptions/salesforce_exceptions.py` & `veevatools-0.0.96/salesforce/custom_exceptions/salesforce_exceptions.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-class RequiredValuesNotProvidedDuringCreate(Exception):
-    """Exception raised when the required values are not provided to the
-    salesforce.create() function.
-
-    Required Values:
-        object_api: str -- The Object API name of the table to be inserted to in Salesforce.
-        record_dataframe: pd.DataFrame() -- a DataFrame of the records to be inserted, including required fields are available
-    """
-
-    def __init__(self, message="Required parameters missing on create. An object_api and the record_dataframe must be provided"):
-        self.message = message
-        super().__init__(self.message)
-
-class RequiredValuesNotProvidedDuringDelete(Exception):
-    """Exception raised when the required values are not provided to the
-    salesforce.delete() function.
-
-    Required Values:
-        object_api: str -- The Object API name of the table to be upserted to in Salesforce.
-        record_dataframe: pd.DataFrame() -- a DataFrame of the records to be deleted. 
-            The provided DataFrame must contain the "Id" column (Case sensitive)
-
-    """
-
-    def __init__(self, message="Required parameters missing on delete. \
-        An object_api and the record_dataframe must be provided or the Id column missing in the provided dataframe."):
-        self.message = message
-        super().__init__(self.message)
-
-class RequiredValuesNotProvidedDuringUpdate(Exception):
-    """Exception raised when the required values are not provided to the
-    salesforce.update() function.
-
-    Required Values:
-        object_api: str -- The Object API name of the table to be updated to in Salesforce.
-        record_dataframe: pd.DataFrame() -- a DataFrame of the records to be updated. 
-            The provided DataFrame must contain the "Id" column (Case sensitive)
-
-    """
-
-    def __init__(self, message="Required parameters missing on update. \
-        An object_api and the record_dataframe must be provided or the Id column missing in the provided dataframe \
-            or dataframe column names do not match a valid Salesforce field API name."):
-        self.message = message
-        super().__init__(self.message)
-
-class RequiredValuesNotProvidedDuringUpsert(Exception):
-    """Exception raised when the required values are not provided to the
-    salesforce.upsert() function.
-
-    Required Values:
-        object_api: str -- The Object API name of the table to be upserted to in Salesforce.
-        record_dataframe: pd.DataFrame() -- a DataFrame of the records to be upserted. 
-            The provided DataFrame must contain the API name of an external ID column.
-
-    """
-
-    def __init__(self, message="Required parameters missing on upserted. \
-        An object_api and the record_dataframe must be provided or and external ID column missing in the provided dataframe \
-            or dataframe column names do not match a valid Salesforce field API name."):
-        self.message = message
-        super().__init__(self.message)
-
-class RequiredFieldMissingDuringCreate(Exception):
-    """Exception raised when the required fields are not provided to the
-    salesforce.create() function.
-    """
-    def __init__(self, message="Required fields missing on create. Check your Salesforce datamodel to ensure all required fields are provided"):
-        self.message = message
-        super().__init__(self.message)
-
+class RequiredValuesNotProvidedDuringCreate(Exception):
+    """Exception raised when the required values are not provided to the
+    salesforce.create() function.
+
+    Required Values:
+        object_api: str -- The Object API name of the table to be inserted to in Salesforce.
+        record_dataframe: pd.DataFrame() -- a DataFrame of the records to be inserted, including required fields are available
+    """
+
+    def __init__(self, message="Required parameters missing on create. An object_api and the record_dataframe must be provided"):
+        self.message = message
+        super().__init__(self.message)
+
+class RequiredValuesNotProvidedDuringDelete(Exception):
+    """Exception raised when the required values are not provided to the
+    salesforce.delete() function.
+
+    Required Values:
+        object_api: str -- The Object API name of the table to be upserted to in Salesforce.
+        record_dataframe: pd.DataFrame() -- a DataFrame of the records to be deleted. 
+            The provided DataFrame must contain the "Id" column (Case sensitive)
+
+    """
+
+    def __init__(self, message="Required parameters missing on delete. \
+        An object_api and the record_dataframe must be provided or the Id column missing in the provided dataframe."):
+        self.message = message
+        super().__init__(self.message)
+
+class RequiredValuesNotProvidedDuringUpdate(Exception):
+    """Exception raised when the required values are not provided to the
+    salesforce.update() function.
+
+    Required Values:
+        object_api: str -- The Object API name of the table to be updated to in Salesforce.
+        record_dataframe: pd.DataFrame() -- a DataFrame of the records to be updated. 
+            The provided DataFrame must contain the "Id" column (Case sensitive)
+
+    """
+
+    def __init__(self, message="Required parameters missing on update. \
+        An object_api and the record_dataframe must be provided or the Id column missing in the provided dataframe \
+            or dataframe column names do not match a valid Salesforce field API name."):
+        self.message = message
+        super().__init__(self.message)
+
+class RequiredValuesNotProvidedDuringUpsert(Exception):
+    """Exception raised when the required values are not provided to the
+    salesforce.upsert() function.
+
+    Required Values:
+        object_api: str -- The Object API name of the table to be upserted to in Salesforce.
+        record_dataframe: pd.DataFrame() -- a DataFrame of the records to be upserted. 
+            The provided DataFrame must contain the API name of an external ID column.
+
+    """
+
+    def __init__(self, message="Required parameters missing on upserted. \
+        An object_api and the record_dataframe must be provided or and external ID column missing in the provided dataframe \
+            or dataframe column names do not match a valid Salesforce field API name."):
+        self.message = message
+        super().__init__(self.message)
+
+class RequiredFieldMissingDuringCreate(Exception):
+    """Exception raised when the required fields are not provided to the
+    salesforce.create() function.
+    """
+    def __init__(self, message="Required fields missing on create. Check your Salesforce datamodel to ensure all required fields are provided"):
+        self.message = message
+        super().__init__(self.message)
+
```

### Comparing `veevatools-0.0.95/salesforce/salesforce.py` & `veevatools-0.0.96/salesforce/salesforce.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,1543 +1,1796 @@
-from sys import platform
-import numpy as np
-import pandas as pd
-import os
-from simple_salesforce import Salesforce
-from simple_salesforce import SalesforceLogin
-from salesforce_bulk import SalesforceBulk
-from sfdclib import SfdcSession
-from sfdclib import SfdcMetadataApi
-from sfdclib import SfdcToolingApi
-import re
-import time
-import json
-from salesforce_bulk.util import IteratorBytesIO
-import pandas as pd
-import requests
-import base64
-from typing import List, Tuple, Optional, Union, Type
-from collections import OrderedDict
-import sys
-import zeep
-import ast
-sys.path.append("..")
-try:
-    from custom_exceptions.salesforce_exceptions import *
-    from utilities.df_utils import *
-    from utilities.async_utils import *
-    from utilities.sf_query_processors import *
-    from decorators import *
-except:
-    from salesforce.custom_exceptions.salesforce_exceptions import *
-    from salesforce.utilities.df_utils import *
-    from salesforce.utilities.async_utils import *
-    from salesforce.utilities.sf_query_processors import *
-    from salesforce.decorators import *
-import asyncio
-from functools import wraps, partial
-from pandas import json_normalize
-
-
-
-
-class Sf:
-    _REGEX_PARSE_SOQL_FIELDS = "(?<=select)(.*?)(?<!, )(?=from)"
-    _REGEX_PARSE_SOQL_OBJECT = "(?<!, from )(?<=from )\w*"
-    
-    def __init__(self) -> None:
-        self.filename: str = None
-        self.os_platform: str = platform
-        self.credentials: pd.DataFrame = pd.DataFrame()
-        self.sfUsername: str = None
-        self.sfPassword: str = None
-        self.sfOrgId: str = ""
-        self.isSandbox: bool = None
-        self.session_id: str = None
-        self.instance: str = None
-        self.domain: str = None
-        self.security_token: str = ''
-        self.sf: Salesforce = None
-        self.bulk: SalesforceBulk = None
-        self.sfMeta: SfdcMetadataApi = None
-        self.tooling: SfdcToolingApi = None
-        self.api_version: str = 'v52.0'
-        self.record_count: dict = {}
-        self.record_count_caseinsensitive: dict = {}
-        self.debug: bool = False
-        self.veeva_common:dict = None
-        self.org_info:dict = None
-        self.sfdc_limits: dict = None
-    
-    def authenticate(self, sfUsername: Optional[str]=None, 
-                                sfPassword: Optional[str]=None, 
-                                sfOrgId: Optional[str]=None, 
-                                isSandbox: Optional[bool]=None, 
-                                session_id: Optional[str]=None, 
-                                instance: Optional[str]=None, 
-                                security_token: Optional[str] = None,
-                                domain: Optional[str] = None,
-                                if_return: Optional[bool] = False,
-                                *args, **kwargs) -> Optional[dict]:
-        """
-        Authenticates Salesforce and retrieves the auth token.
-
-        Dependencies:
-            from simple_salesforce import Salesforce
-            from simple_salesforce import SalesforceLogin
-            from salesforce_bulk import SalesforceBulk
-            from sfdclib import SfdcSession
-            from sfdclib import SfdcMetadataApi
-            from sfdclib import SfdcToolingApi
-        """
-        
-        sfUsername = self.sfUsername if sfUsername is None else sfUsername
-        sfPassword = self.sfPassword if sfPassword is None else sfPassword
-        sfOrgId = self.sfOrgId if sfOrgId is None else sfOrgId
-        isSandbox = self.isSandbox if isSandbox is None else isSandbox
-        session_id = self.session_id if session_id is None else session_id
-        instance = self.instance if instance is None else instance
-        security_token = self.security_token if security_token is None else security_token
-        domain = self.domain if domain is None else domain
-        
-        # If session ID already exists and instance URL is already populated,
-        # reauthenticate using existing session ID
-        if session_id is not None and instance is not None:
-            sf = Salesforce(session_id = session_id, instance = instance)
-            self.sf = sf
-            self.instance = instance
-            self.session_id = session_id
-        
-        # If username, password, org ID, and isSandbox flags are all provided,
-        # authenticate using provided credentials
-        elif sfUsername is not None and sfPassword is not None and sfOrgId is not None and isSandbox is not None:
-            
-            # SFDC Sandbox authentication
-            if isSandbox:
-                self.domain = 'test'
-                sf = Salesforce(password=sfPassword, 
-                                username=sfUsername, 
-                                organizationId=sfOrgId, 
-                                security_token = self.security_token,domain='test')
-                session_id, instance = SalesforceLogin(
-                username=sfUsername,
-                password=sfPassword,
-                security_token=self.security_token,
-                domain= self.domain)
-                self.session_id = session_id
-                self.instance = instance
-                self.sf = sf
-                self.sfUsername = sfUsername
-                self.sfPassword = sfPassword
-                self.load_org_info()
-                self.sfOrgId = self.org_info['Id'][0]
-                self.isSandbox = isSandbox
-                
-            else:
-                sf = Salesforce(password=sfPassword, 
-                                username=sfUsername, 
-                                organizationId=sfOrgId, 
-                                security_token=self.security_token)
-                session_id, instance = SalesforceLogin(
-                username=sfUsername,
-                password=sfPassword,
-                security_token=self.security_token)
-                self.session_id = session_id
-                self.instance = instance
-                self.sf = sf
-                self.sfUsername = sfUsername
-                self.sfPassword = sfPassword
-                self.load_org_info()
-                self.sfOrgId = self.org_info['Id'][0]
-                self.isSandbox = isSandbox
-                
-        else:
-            raise Exception('Either sfUsername, sfPassword, sfOrgId and isSandbox must be populated, OR session_id and instance must be populated.')
-
-        # Alternative way to authenticate using SFDC Bulk API
-        # bulk = SalesforceBulk(username=sfUsername, password=sfPassword, security_token='')
-        bulk = SalesforceBulk(sessionId = self.session_id, host = self.instance)
-        self.bulk = bulk
-        # SFDC Metadata API
-        sf_meta_instance = ""
-        if self.instance.__contains__("my.salesforce.com"):
-            sf_meta_instance = self.instance.replace("my.salesforce.com","my")
-        else:
-            sf_meta_instance = ".".join(self.instance.split(".")[:2])
-            
-        sfMeta = SfdcSession(session_id=self.session_id, instance=sf_meta_instance)
-        self.sfMeta = sfMeta
-        # Alternative way to authenticate using SFDC Metadata API
-        # sfMeta = SfdcSession(username=sfUsername,password=sfPassword,token='',is_sandbox=isSandbox)
-        sfMeta._api_version = "54.0"
-        tooling = SfdcToolingApi(sfMeta)
-        self.tooling = tooling
-        
-        self.api_version = 'v' + self.sf_api_call('/services/data')[-1]['version']
-        
-        for x in self.sf_api_call('/services/data/'+self.api_version+'/limits/recordCount')['sObjects']:
-            self.record_count[x['name']] = x['count']
-            self.record_count_caseinsensitive[x['name'].lower()] = x['count']
-        
-        self.sfdc_limits = self.parse_sf_limits(self.sf_api_call('/services/data/'+self.api_version+'/limits'))
-        
-        
-        if if_return:
-            return {'sf':sf, 
-                    'bulk':bulk, 
-                    'sfMeta': sfMeta, 
-                    'tooling':tooling, 
-                    'session_id':session_id, 
-                    'instance':instance, 
-                    'sfMeta_is_connected':sfMeta.is_connected(), 
-                    'bulk_api_sessionId':bulk.sessionId}
-
-    ### ----------------------------------------------------------------------------------------------------
-    ### Synchronous Data Functions
-    ### ----------------------------------------------------------------------------------------------------
-
-    def query(self, query: str, excludedFields: Optional[List] = [], *args) -> pd.DataFrame:
-        """
-        Using SFDC SOQL Syntax, and allowing for Relationships and group bys. 
-        
-        Arguments:
-            query (str): A Standard SFDC SOQL Query allowing for relationships (Owner.Name)
-                Asterisks(*) represents all queryable fields and can be used in conjunction
-                with other relationship fields. 
-                i.e. (Select *, Owner.Profile.Name, Owner.Name From Account)
-        
-        Returns:
-            Pandas Dataframe Object.
-        
-        Raises:
-            KeyError: Typically raised when 0 records exist for the object
-                
-            badfield: A self-correcting error that is raised when a field is unqueriable, i.e. Address Fields
-            
-            Exception: When relationship query contains more than 4 layers, an Exception is raised.
-            i.e. Parent_Account_vod__r.Owner.Profile.LastModifiedBy.Name (<- a 5 layer deep relationship is not supported)
-        
-        Example of Usage:
-            sf.query("Select *, Owner.Profile.Name From Account ORDER BY CreatedDate DESC LIMIT 100")
-            
-            return:
-            A Pandas Dataframe of the last created 100 account records, with all queriable fields included in the query and a relationship field.
-            
-        """
-        objectName = re.search(self._REGEX_PARSE_SOQL_OBJECT, query.lower()).group(0)
-        successful = False
-        
-        extracted_object = pd.DataFrame()
-        # replaces "*" in query with all fields on object
-        sfSchema = getattr(self.sf, objectName).describe().get('fields')
-
-        schemaDict = {}
-        for x in sfSchema:
-            schemaDict[x['name']] = x
-
-        while not successful:
-            try:
-                results = []
-                for field in schemaDict:
-                    if (schemaDict[field]['type'] != 'location' and 
-                        schemaDict[field]['type'] != 'address' and 
-                        schemaDict[field]['name'] not in excludedFields):
-                        results.append(field)
-                final_query = query.replace("*", ", ".join(results))                
-                query_response = self.sf.query_all(final_query)
-                # if the object has 0 records in Salesforce, return empty dataframe
-                if query_response['totalSize'] == 0:
-                    fields_preparsed = re.search(self._REGEX_PARSE_SOQL_FIELDS, query,  re.IGNORECASE).group(0).split(",")
-                    return pd.DataFrame(columns=fields_preparsed)
-                else:
-                    result = pd.DataFrame(query_response)['records']
-                    for _ in result:
-                        del _['attributes']
-                    successful = True
-            except KeyError:
-                if self.debug:
-                    print(objectName + ' skipped. (Potentially due to no records found.)')
-                    
-                return pd.DataFrame(columns=results)
-            except Exception as badfield:
-                field_exclusion = badfield.state_message[badfield.state_message.find("No such column '")+\
-                    16:badfield.state_message.find("No such column '")+16+\
-                        badfield.state_message[badfield.state_message.find("No such column '")+16:].find("'")]
-                excludedFields.append(field_exclusion)
-                print("Excluded unqueriable field: " + field_exclusion)
-                if query.find("*") == -1:
-                    raise Exception(f"Unqueriable field {field_exclusion} found in query.")
-                else:
-                    continue
-            
-            result = result.apply(lambda x: pd.Series(x)).copy()
-
-            relationship_fields_preparsed = re.search(self._REGEX_PARSE_SOQL_FIELDS, query,  re.IGNORECASE).group(0).split(",")
-            # relationship_fields_prepared Example:
-            # ['*',
-            #  ' Parent_Account_vod__r.Owner.Profile.Name',
-            #  ' Child_Account_vod__r.Owner.Profile.Name',
-            #  'Parent_Account_vod__r.Owner.Profile.Id ']
-
-            relational_fields = [{x.strip(): x.strip().split(".")} for x in relationship_fields_preparsed if "." in x]
-            # relationship_fields Example:
-            # [{'Parent_Account_vod__r.Owner.Profile.Name': ['Parent_Account_vod__r',
-            #    'Owner',
-            #    'Profile',
-            #    'Name']},
-            #  {'Child_Account_vod__r.Owner.Profile.Name': ['Child_Account_vod__r',
-            #    'Owner',
-            #    'Profile',
-            #    'Name']},
-            #  {'Parent_Account_vod__r.Owner.Profile.Id': ['Parent_Account_vod__r',
-            #    'Owner',
-            #    'Profile',
-            #    'Id']}]
-
-            columns_to_remove = set()
-            for x in relational_fields:
-                if len(list(x.values())[0]) > 4:
-                    raise Exception("Too Many Relationship Levels. The Query you have entered contains more than 4 levels deep and is not supported.")
-                elif len(list(x.values())[0]) == 4:
-                    result[list(x.keys())[0]] = result[list(x.keys())[0].split(".")[0]].\
-                        apply(lambda z: z[list(x.values())[0][1]][list(x.values())[0][2]][list(x.values())[0][3]])
-                    columns_to_remove.add(list(x.values())[0][0])
-                elif len(list(x.values())[0]) == 3:
-                    result[list(x.keys())[0]] = result[list(x.keys())[0].split(".")[0]].\
-                        apply(lambda z: z[list(x.values())[0][1]][list(x.values())[0][2]])
-                    columns_to_remove.add(list(x.values())[0][0])
-                elif len(list(x.values())[0]) == 2:
-                    result[list(x.keys())[0]] = result[list(x.keys())[0].split(".")[0]].\
-                        apply(lambda z: z[list(x.values())[0][1]])
-                    columns_to_remove.add(list(x.values())[0][0])
-            result.drop(columns_to_remove, axis=1, inplace=True)
-            result.replace(np.nan, None, inplace=True)        
-
-                
-        return result
-
-    def create(self, object_api: str=None, record_dataframe: pd.DataFrame = pd.DataFrame()) -> pd.DataFrame:
-        """
-        Function creates records within the Salesforce instance using bulk api.
-
-        Arguments:
-        object_api: str: API name of the Salesforce Object for which the records are to be created.
-
-        record_dataframe: pd.DataFrame: A pandas dataframe object containing all the required fields for a record.
-
-        Returns:
-        result: pd.DataFrame: A pandas dataframe with the following columns:
-            success: boolean: indicates whether the create request was successful
-            created: boolean: this value should always be False in a create request
-            id: object[str]: this value typically is None in a create request
-            statusCode: object[str] - Optional: the error code of the create operation if failed
-            message: object[str] - Optional: the error message of the create operation if failed
-            fields: object[List[str]] - Optional: the fields for which the error code and message applies to.
-
-        Raises:
-            RequiredValuesNotProvidedDuringUpdate
-        """
-        if (object_api is None) or (len(record_dataframe) == 0):
-            raise RequiredValuesNotProvidedDuringCreate()
-        else:
-            result = getattr(self.sf.bulk, object_api).insert(record_dataframe.to_dict('records'), batch_size=10000, use_serial=False)
-            result = pd.DataFrame(result)
-            result = unpack_column(result, "errors")
-
-        return pd.DataFrame(result.rename(columns={'id': 'Id'}))
-
-    def delete(self, object_api: str=None, record_dataframe: pd.DataFrame = pd.DataFrame()) -> pd.DataFrame:
-        """
-        Function deletes records within the Salesforce instance using bulk api.
-
-        Arguments:
-        object_api: str: API name of the Salesforce Object for which the records are to be deleted from.
-
-        record_dataframe: pd.DataFrame: A pandas dataframe object containing at least 1 column with an Id column (case sensitive)
-
-        Returns:
-        result: pd.DataFrame: A pandas dataframe with the following columns:
-            success: boolean: indicates whether the delete request was successful
-            created: boolean: this value should always be False in a delete request
-            id: object[str]: this value typically is None in a delete request
-            statusCode: object[str] - Optional: the error code of the delete operation if failed
-            message: object[str] - Optional: the error message of the delete operation if failed
-            fields: object[List[str]] - Optional: the fields for which the error code and message applies to.
-
-        Raises:
-            RequiredValuesNotProvidedDuringDelete
-        """
-        if (object_api is None) or (len(record_dataframe) == 0) or record_dataframe.columns.__contains__('Id') == False:
-            raise RequiredValuesNotProvidedDuringDelete()
-        else:
-            result = getattr(self.sf.bulk, object_api).delete(record_dataframe['Id'].to_frame().to_dict('records'))
-            result = pd.DataFrame(result)
-            result = unpack_column(result, "errors")
-
-        return pd.DataFrame(result.rename(columns={'id': 'Id'}))
-    
-    def update(self, object_api: str=None, record_dataframe: pd.DataFrame = pd.DataFrame()) -> pd.DataFrame:
-        """
-        Function updates records within the Salesforce instance using bulk api.
-
-        Arguments:
-        object_api: str: API name of the Salesforce Object for which the records are to be updated.
-
-        record_dataframe: pd.DataFrame: A pandas dataframe object containing at least 1 column with an Id column (case sensitive)
-            and additional columns matching the Salesforce field api names.
-
-        Returns:
-        result: pd.DataFrame: A pandas dataframe with the following columns:
-            success: boolean: indicates whether the update request was successful
-            created: boolean: this value should always be False in a update request
-            id: object[str]: this value typically is None in a update request
-            statusCode: object[str] - Optional: the error code of the update operation if failed
-            message: object[str] - Optional: the error message of the update operation if failed
-            fields: object[List[str]] - Optional: the fields for which the error code and message applies to.
-
-        Raises:
-            RequiredValuesNotProvidedDuringUpdate
-        """
-
-        field_metadata = self.field_describe([object_api],attributes=['name','type','updateable','compoundFieldName'])
-
-        if ((object_api is None) or 
-        (len(record_dataframe) == 0)):
-            raise RequiredValuesNotProvidedDuringUpdate(message="Object API and Record Dataframe are required, ensure your record dataframe has at least 1 row and 1 column with an Id column")
-        elif record_dataframe.columns.__contains__('Id') == False:
-            raise RequiredValuesNotProvidedDuringUpdate(message="Record Dataframe must have an Id column")
-        elif ~record_dataframe.columns.isin(field_metadata[object_api]).all():
-            # checks whether any of the columns in the dataframe passed in are not valid field API names
-            raise RequiredValuesNotProvidedDuringUpdate(message="One of the columns in the record dataframe is not a valid field for the object")
-        elif record_dataframe.columns.isin(field_metadata[(field_metadata['Updateable'] == False) & (field_metadata[object_api] != "Id")][object_api]).any():
-            # checks whether any of the columns in the dataframe passed in are not updateable
-            non_updatable_fields = list(set(record_dataframe.columns) - set(field_metadata[(field_metadata['Updateable'] == True) | (field_metadata[object_api] == "Id")][object_api]))
-            raise RequiredValuesNotProvidedDuringUpdate(message=f"The following fields are not updatable: {', '.join(non_updatable_fields)}")
-        elif record_dataframe.columns.isin(field_metadata[(~field_metadata['Compoundfieldname'].isnull()) & (field_metadata['Compoundfieldname'] != 'Name')][object_api]).any():
-            # checks whether any of the columns in the dataframe passed in are compound fields
-            compound_fields = list(set(record_dataframe.columns) & set(field_metadata[(~field_metadata['Compoundfieldname'].isnull()) & (field_metadata['Compoundfieldname'] != 'Name')][object_api]))
-            raise RequiredValuesNotProvidedDuringUpdate(message=f"The following fields are compound fields, which are not updatable: {', '.join(compound_fields)}")
-        # checks whether an reference (lookup/master-detail) field is included in the source dataframe
-        #  or ~record_dataframe.columns.isin(field_metadata[field_metadata['Type'] == 'reference'][object_api]).any()
-            
-        else:
-            record_dataframe.replace(np.nan, None, inplace=True)
-            result = getattr(self.sf.bulk, object_api).update(record_dataframe.to_dict('records'), batch_size=10000, use_serial=False)
-            result = pd.DataFrame(result)
-            result = unpack_column(result, "errors")
-
-        return pd.DataFrame(result.rename(columns={'id': 'Id'}))
-
-    def upsert(self, object_api: str=None, external_id_field_api: str="", record_dataframe: pd.DataFrame = pd.DataFrame()) -> pd.DataFrame:
-        """
-        Function upserts records within the Salesforce instance using bulk api.
-
-        Arguments:
-        object_api: str: API name of the Salesforce Object for which the records are to be upserted into.
-
-        external_id_field_api: str: API name of the external ID field used for the upsert operation.
-
-        record_dataframe: pd.DataFrame: A pandas dataframe object containing the External column (case sensitive)
-            and additional columns matching the Salesforce field api names.
-
-        Returns:
-        result: pd.DataFrame: A pandas dataframe with the following columns:
-            success: boolean: indicates whether the upsert request was successful
-            created: boolean: this value should always be False in a upsert request
-            id: object[str]: this value typically is None in a upsert request
-            statusCode: object[str] - Optional: the error code of the upsert operation if failed
-            message: object[str] - Optional: the error message of the upsert operation if failed
-            fields: object[List[str]] - Optional: the fields for which the error code and message applies to.
-
-        Raises:
-            RequiredValuesNotProvidedDuringUpsert
-            SalesforceMalformedRequest
-        """
-
-        field_metadata = self.field_describe([object_api], ['name', 'type', 'length','externalId','updateable','compoundFieldName'])
-            
-            
-        if ((object_api is None) or 
-        (len(record_dataframe) == 0)):
-            raise RequiredValuesNotProvidedDuringUpdate(message="Object API and Record Dataframe are required, ensure your record dataframe has at least 1 row and 1 column with an Id column")
-        elif ~record_dataframe.columns.isin(field_metadata[object_api]).all():
-            # checks whether any of the columns in the dataframe passed in are not valid field API names
-            raise RequiredValuesNotProvidedDuringUpdate(message="One of the columns in the record dataframe is not a valid field for the object")
-        elif external_id_field_api == "":
-            raise RequiredValuesNotProvidedDuringUpsert(message="External ID field API is required")
-        elif record_dataframe.columns.isin(field_metadata[(field_metadata['Updateable'] == False) & (field_metadata[object_api] != "Id")][object_api]).any():
-            # checks whether any of the columns in the dataframe passed in are not updateable
-            non_updatable_fields = list(set(record_dataframe.columns) - set(field_metadata[(field_metadata['Updateable'] == True) | (field_metadata[object_api] == "Id")][object_api]))
-            raise RequiredValuesNotProvidedDuringUpdate(message=f"The following fields are not updatable: {', '.join(non_updatable_fields)}")
-        elif record_dataframe.columns.isin(field_metadata[(~field_metadata['Compoundfieldname'].isnull()) & (field_metadata['Compoundfieldname'] != 'Name')][object_api]).any():
-            # checks whether any of the columns in the dataframe passed in are compound fields
-            compound_fields = list(set(record_dataframe.columns) & set(field_metadata[(~field_metadata['Compoundfieldname'].isnull()) & (field_metadata['Compoundfieldname'] != 'Name')][object_api]))
-            raise RequiredValuesNotProvidedDuringUpdate(message=f"The following fields are compound fields, which are not updatable: {', '.join(compound_fields)}")
-        else:
-            record_dataframe.replace(np.nan, None, inplace=True)
-            result = getattr(self.sf.bulk, object_api).upsert(record_dataframe.to_dict('records'), external_id_field_api, batch_size=10000, use_serial=False)
-            result = pd.DataFrame(result)
-            result = unpack_column(result, "errors")
-
-        return pd.DataFrame(result)
-
-    def extract_bulk(self, og_query: str, 
-                        excludedFields: Optional[List] = []) -> pd.DataFrame:
-        """
-        Uses a standard SOQL query to extract Salesforce Data and outputs a pandas dataframe
-        
-        Dependencies:
-            import re
-            import time
-            import json
-            from salesforce_bulk.util import IteratorBytesIO
-            import pandas as pd
-        
-        """
-        objectName = re.search(self._REGEX_PARSE_SOQL_OBJECT, og_query.lower()).group(0)
-        successful = False
-        
-        extracted_object = pd.DataFrame()
-        # replaces "*" in query with all fields on object
-        sfSchema = getattr(self.sf, objectName).describe().get('fields')
-
-        schemaDict = {}
-        for x in sfSchema:
-            schemaDict[x['name']] = x
-
-        while not successful:
-            try:
-                results = []
-                for field in schemaDict:
-                    if (schemaDict[field]['type'] != 'location' and 
-                        schemaDict[field]['type'] != 'address' and 
-                        schemaDict[field]['name'] not in excludedFields):
-                        results.append(field)
-                query = og_query.replace("*", ", ".join(results))
-                
-#                 # if the object has 0 records in Salesforce, return empty dataframe
-#                 if objectName not in self.record_count_caseinsensitive.keys():
-#                     return pd.DataFrame(columns=results)
-                    
-                job = self.bulk.create_query_job(objectName, contentType='JSON')
-                batch = self.bulk.query(job, query)
-                while not self.bulk.is_batch_done(batch):
-                    time.sleep(1)
-                sfdf = pd.DataFrame()
-                for result in self.bulk.get_all_results_for_query_batch(batch):
-                    result = json.load(IteratorBytesIO(result))
-                    sfdf = pd.concat([sfdf, pd.DataFrame(result)])
-
-                # drops attributes column in dataframe
-                sfdf.drop(columns="attributes", inplace = True)
-
-                # formats all datetime to the proper formatting
-                for column in sfdf:
-                    if schemaDict[column]['type'] == 'datetime':
-                        sfdf[column] = pd.to_datetime(sfdf[column], unit='ms')
-                    # if the column has a 'scale' or salesforce's decimal places, then turn the column into an int
-                    elif schemaDict[column]['type'] == 'double' and schemaDict[column]['scale'] == 0:
-                        sfdf[column] = pd.to_numeric(sfdf[column], downcast='integer')
-
-            #                         pd.to_datetime(sfdf[column], unit = 's')
-            #                         sfdf[column].apply(lambda x : datetime.fromtimestamp(int(x), tz).isoformat())
-            #                 sfdf.convert_dtypes()
-                # converts the output of the bulk query to text so that the unix timestamp displays property, and fills and empty values with the '' string.
-                sfdf = sfdf.fillna('').astype(str)
-                successful = True
-            except KeyError:
-                if self.debug:
-                    print(objectName + ' skipped. (Potentially due to no records found.)')
-                    
-                return pd.DataFrame(columns=results)
-            except Exception as badfield:
-                field_exclusion = badfield.state_message[badfield.state_message.find("No such column '")+\
-                    16:badfield.state_message.find("No such column '")+16+\
-                        badfield.state_message[badfield.state_message.find("No such column '")+16:].find("'")]
-                excludedFields.append(field_exclusion)
-                print("Excluded unqueriable field: " + field_exclusion)
-                if og_query.find("*") == -1:
-                    raise Exception(f"Unqueriable field {field_exclusion} found in query.")
-                else:
-                    continue
-        if self.debug:
-            print("Extracted " + objectName + " successfully!")
-        return sfdf
-    
-    def entity_access_query(self, entity_type):
-        # Retrieves information about which Profile or PermissionSet
-        # grants permission to which Setup Entity (i.e. ApexPage, ApexClass, TabSets, etc)
-        
-        entity_access = transform_sf_result_set_rec(self.sf.query_all(f"""
-        SELECT Id, Parent.Id, Parent.ProfileId, Parent.Profile.Name, Parent.Name,SetupEntityId,SetupEntityType FROM
-        SetupEntityAccess WHERE SetupEntityType = '{entity_type}'""")['records'])
-        # entity_access.drop(columns=['PermissionSet.Profile'], inplace=True)
-        return {entity_type: entity_access}
-
-    ### ----------------------------------------------------------------------------------------------------
-    ### Asynchronous Data Functions
-    ### ----------------------------------------------------------------------------------------------------
-
-    async def async_query(self, query, excludedFields: Optional[List] = []) -> pd.DataFrame:
-        async_query = async_wrap(self.query)
-        return await async_query(query, excludedFields)
-    
-    async def async_queries(self, queries: List[str]):
-        async_queries = async_wrap(self.sf.query_all)
-        result_list = await asyncio.gather(*[async_queries(query) for query in queries])
-        result_pd_list = [transform_sf_result_set_rec(result['records']) for result in result_list]
-        return result_pd_list
-
-
-    async def async_upsert(self, object_api, record_dataframe, external_id_field_api, batchsize=2000, *args, **kwargs):
-        async_upsert = async_wrap(self.upsert)
-        batches = len(record_dataframe) / batchsize
-        result_list = await asyncio.gather(*[async_upsert(object_api= object_api, record_dataframe=batch, external_id_field_api=external_id_field_api) for batch in np.array_split(record_dataframe, batches)])
-        return pd.concat(result_list).reset_index(drop=True)
-
-    async def async_update(self, object_api, record_dataframe, batchsize=2000, *args, **kwargs):
-        async_update = async_wrap(self.update)
-        batches = len(record_dataframe) / batchsize
-        result_list = await asyncio.gather(*[async_update(object_api= object_api, record_dataframe=batch) for batch in np.array_split(record_dataframe, batches)])
-        return pd.concat(result_list).reset_index(drop=True)
-
-    async def async_create(self, object_api, record_dataframe, batchsize=2000, *args, **kwargs):
-        async_create = async_wrap(self.create)
-        batches = len(record_dataframe) / batchsize
-        result_list = await asyncio.gather(*[async_create(object_api= object_api, record_dataframe=batch) for batch in np.array_split(record_dataframe, batches)])
-        return pd.concat(result_list).reset_index(drop=True)
-
-    async def async_delete(self, object_api, record_dataframe, batchsize=2000, *args, **kwargs):
-        async_delete = async_wrap(self.delete)
-        batches = len(record_dataframe) / batchsize
-        result_list = await asyncio.gather(*[async_delete(object_api= object_api, record_dataframe=batch) for batch in np.array_split(record_dataframe, batches)])
-        return pd.concat(result_list).reset_index(drop=True)
-    
-    async def async_get_user_password_status(self, user_ids: list[str]) -> dict:
-        async_sf_api_call = async_wrap(self.sf_api_call)
-        response = await asyncio.gather(*[async_sf_api_call(f'/services/data/{self.api_version}/sobjects/User/{user_id}/password', method='GET') for user_id in user_ids])
-        # Return a dict
-        response = {user_id: result for user_id, result in zip(user_ids, response)}
-        return response
-    
-    
-    
-    ### ----------------------------------------------------------------------------------------------------
-    ### Asynchronous Metadata Functions
-    ### ----------------------------------------------------------------------------------------------------
-    async def async_get_non_updatable_fields(self, object_name: str):
-        """
-        Returns a list of fields that cannot be updated.
-        """
-        async_field_describe =  async_wrap(self.field_describe)
-        field_metadata = await async_field_describe([object_name], attributes=['name','updateable'])
-        non_updatable_fields = list(field_metadata[field_metadata['Updateable'] == False][object_name])[1:]
-        return non_updatable_fields
-
-    async def async_get_compound_field_names(self, object_name: str, include_name_compound_fields: bool=False):
-        """
-        Returns a list of compound fields. By default "Name" compound field names are excluded.
-        To return a list of compound fields including "Name" fields, set include_name_compound_fields to True.
-
-        Compound field names are fields that are composed of multiple fields. These fields are not updatable directly via the API
-        and may cause errors if updated directly.
-        """
-        async_field_describe =  async_wrap(self.field_describe)
-        field_metadata = await async_field_describe([object_name], attributes=['name','compoundFieldName'])
-
-        if include_name_compound_fields:
-            compound_field_names = list(field_metadata[(~field_metadata['Compoundfieldname'].isnull())][object_name])
-        elif include_name_compound_fields==False:
-            compound_field_names = list(field_metadata[(~field_metadata['Compoundfieldname'].isnull()) & (field_metadata['Compoundfieldname'] != 'Name')][object_name])
-        else:
-            raise ValueError('include_name_compound_fields must be a boolean.')
-        return compound_field_names
-    
-    async def get_picklist_values_by_object_record_type(self, object: str):
-        object_record_type_ids = self.query(f"Select Id, Name From RecordType Where SobjectType = '{object}'").apply(lambda row: {"Id": row['Id'], "Name": row['Name']}, axis=1)
-        if len(object_record_type_ids) == 0:
-            object_record_type_ids = pd.Series([{"Id": "012000000000000AAA", "Name": "Master"}]).to_list()
-        else:
-            object_record_type_ids = object_record_type_ids.to_list()
-            
-        object_describe = self.sf_api_call(f"/services/data/{self.api_version}/ui-api/object-info/{object}")['fields']
-        controlling_fields = []
-        for field, values in object_describe.items():
-            controlling_fields.append({"Field": field, "Controlling Field": "" if values['controllingFields'] == [] else "; ".join(values['controllingFields'])})
-        controlling_fields = pd.DataFrame(controlling_fields)
-
-        def record_type_picklist_retriever(self, object, record_type_id, record_type_name):
-            result = []
-            picklist_metadata = self.sf_api_call(f"/services/data/{self.api_version}/ui-api/object-info/{object}/picklist-values/{record_type_id}")['picklistFieldValues']
-            if len(picklist_metadata) == 0:
-                return pd.DataFrame(columns=['attributes',
-                                    'label',
-                                    'validFor',
-                                    'value',
-                                    'Field_API',
-                                    'defaultValueLabel',
-                                    'defaultValueValue',
-                                    'Controlling Field',
-                                    'RecordTypeName',
-                                    'Object'])
-                
-            for key, value in picklist_metadata.items():
-                result.append({"Field_API": key, "controllerValues": value['controllerValues'], "defaultValue":  value['defaultValue'], "values": value['values']})
-            final_result_pd = json_normalize(result, ['values'], ['defaultValue', 'controllerValues', 'Field_API'])
-            ## Converts the validFor numerical codes i.e. [0,2] to it's corresponding text values by looking it up on the controllerValues column i.e. {'Web': 0, 'Phone Inquiry': 1, 'Partner Reference': 2 ... }
-            ## [0,2] -> ['Web', 'Partner Reference']
-            final_result_pd['validFor'] = final_result_pd.apply(lambda row: "\n".join([{v: k for k, v in row['controllerValues'].items()}[value] for value in row['validFor']]), axis=1)
-            final_result_pd.drop(columns=['controllerValues'], inplace=True)
-            
-            try:
-                final_result_pd[['defaultValueLabel', 'defaultValueValue']] = json_normalize(final_result_pd['defaultValue'])[['label','value']]
-            except:
-                final_result_pd[['defaultValueLabel', 'defaultValueValue']] = [np.nan, np.nan]
-            
-            final_result_pd.drop(columns=['defaultValue'], inplace=True)
-            final_result_pd = pd.merge(final_result_pd, controlling_fields, left_on='Field_API', right_on='Field', how='left').drop(columns=['Field']).copy()
-            final_result_pd['RecordTypeName'] = record_type_name
-            final_result_pd['Object'] = object
-            return final_result_pd
-
-        async_picklist_rt_retrieve = async_wrap(record_type_picklist_retriever)
-        results = pd.concat(await asyncio.gather(*[async_picklist_rt_retrieve(self, object, record_type_id['Id'], record_type_id['Name']) for record_type_id in object_record_type_ids]))
-        results = results[['Object', 'RecordTypeName', 'Field_API', 'Controlling Field', 'defaultValueLabel', 'defaultValueValue', 'label', 'value', 'validFor']]
-        return results
-
-
-    async def object_permission_bulk_check(self, objects: list, permissions: list ):
-        async_object_permission_check = async_wrap(self.object_permission_check)
-        result_list = await asyncio.gather(*[async_object_permission_check(object, permission ) for object in objects for permission in permissions])
-        # for result in result_list:
-        #     data = deep_merge_dictionaries(data, result)
-        result_list = [item for sublist in result_list for item in sublist]
-        return result_list
-
-    async def field_permission_bulk_check(self, objects: list, ) -> dict[str, pd.DataFrame]:
-        async_field_permission_check = async_wrap(self.field_permission_check)
-        result_list = await asyncio.gather(*[async_field_permission_check( object ) for object in objects])
-        # for result in result_list:
-        #     data = deep_merge_dictionaries(data, result)
-        profile_list = [item['profilePermissions'] for item in result_list]
-        permissionSet_list = [item['permissionSetPermissions'] for item in result_list]
-        result_dict = {'profilePermissions': pd.concat(profile_list), 'permissionSetPermissions': pd.concat(permissionSet_list)}
-        
-        return result_dict
-    
-    async def async_set_user_passwords(self, user_id_password_list_dict: dict) -> dict:
-        async_set_user_password = async_wrap(self.set_user_password)
-        results = await asyncio.gather(*[async_set_user_password(user_id, password) for user_id, password in user_id_password_list_dict.items()])
-        results = {result['user_id']: result['message'] for result in results}
-        return results
-
-    async def entity_access_bulk_query(self, entity_types: list):
-        async_entity_access_query = async_wrap(self.entity_access_query)
-        results = await asyncio.gather(*[async_entity_access_query(entity_type) for entity_type in entity_types])
-        merged_dict = {}
-        for result in results:
-            for key, value in result.items():
-                merged_dict[key] = value
-        return merged_dict
-
-    async def apex_pages_profiles_and_permission_set_access_query(self, apex_pages_to_check: list[str]):
-        query_results = await self.entity_access_bulk_query(['ApexPage'])
-
-        entity_access_apex_pages_async =  query_results['ApexPage']
-
-        entity_permission_set_access_apex_pages_async = entity_access_apex_pages_async[entity_access_apex_pages_async['Profile.Name'].isna()]
-        entity_profile_access_apex_pages_async = entity_access_apex_pages_async[entity_access_apex_pages_async['Profile.Name'].notna()]
-
-        # filter = ['Scheduler_Administration_vod','Network_Admin_Page_vod','searchAccts_vod']
-        filter_join = "','".join(apex_pages_to_check)
-        where_clause = f" WHERE Name IN ('{filter_join}')"
-        apex_pages_query = transform_sf_result_set_rec(self.sf.query_all(f"""
-            SELECT Id, Name From ApexPage{where_clause}""")['records'])
-
-        permission_sets_with_apex_page_access = entity_permission_set_access_apex_pages_async[entity_permission_set_access_apex_pages_async['SetupEntityAccess.SetupEntityId'].isin(apex_pages_query['ApexPage.Id'].unique())]
-        profiles_with_apex_page_access = entity_profile_access_apex_pages_async[entity_profile_access_apex_pages_async['SetupEntityAccess.SetupEntityId'].isin(apex_pages_query['ApexPage.Id'].unique())]
-        permission_sets_with_apex_page_access = pd.merge(permission_sets_with_apex_page_access, apex_pages_query, left_on='SetupEntityAccess.SetupEntityId', right_on='ApexPage.Id', how='inner').drop(columns=['ApexPage.Id'], axis=1)
-        profiles_with_apex_page_access = pd.merge(profiles_with_apex_page_access, apex_pages_query, left_on='SetupEntityAccess.SetupEntityId', right_on='ApexPage.Id', how='inner').drop(columns=['ApexPage.Id'], axis=1)
-
-        profiles_with_apex_page_access = profiles_with_apex_page_access[['PermissionSet.ProfileId','Profile.Name','SetupEntityAccess.SetupEntityType','ApexPage.Name']]
-        profiles_with_apex_page_access.columns = ['Profile Id', 'Profile Name', 'Setup Entity Type', 'Visualforce (Apex) Name']
-        
-        permission_sets_with_apex_page_access = permission_sets_with_apex_page_access[['PermissionSet.Id','PermissionSet.Name','SetupEntityAccess.SetupEntityType','ApexPage.Name']]
-        permission_sets_with_apex_page_access.columns = ['PermissionSet Id', 'PermissionSet Name', 'Setup Entity Type', 'Visualforce (ApexPage) Name']
-        
-        return {'profiles_with_apex_page_access': profiles_with_apex_page_access, 'permission_sets_with_apex_page_access': permission_sets_with_apex_page_access}
-
-    # Retrieves the Page Layout by Profile by Record Type data for listed objects in the org
-    async def retrieve_profile_layout_record_type_matrix_by_objects(self, objects_to_retrieve_profile_layout_matrix = ['Account','Address_vod__c','Child_Account_vod__c'], discard_unqueriable_objects = False, return_pivot_table = False):
-        
-        objects_to_retrieve = [object[:-3] if object.endswith('__c') else object for object in objects_to_retrieve_profile_layout_matrix]
-        
-        # Objects in the Profile Layout table's TableEnumOrId column where the value is an object name instead of an object ID
-        
-        ENUM_OBJECTS = {'Account', 'AccountTeamMember', 'Asset', 'AuthorizationForm', 'AuthorizationFormConsent', 'BusinessBrand', 'Campaign', 'CampaignMember', 'Case',
-                            'CaseClose', 'CaseInteraction', 'CommunityMemberLayout', 'Contact', 'ContactPointAddress', 'ContactPointEmail', 'ContactPointPhone', 'ContentVersion', 'Contract', 'Customer', 'DelegatedAccount',
-                            'DuplicateRecordItem', 'DuplicateRecordSet', 'EmailMessage', 'Event', 'FeedItem', 'Global', 'Idea', 'Individual', 'Lead', 'Macro', 'ObjectTerritory2AssignmentRule',
-                            'Opportunity', 'OpportunityLineItem', 'Order', 'OrderItem', 'PersonAccount', 'Pricebook2', 'PricebookEntry', 'ProcessException', 'Product2',
-                            'ProfileSkill', 'ProfileSkillEndorsement', 'ProfileSkillUser', 'QuickText', 'Scorecard', 'ScorecardAssociation', 'ScorecardMetric', 'Seller', 'ServiceAppointmentGroup',
-                            'ServiceTerritoryRelationship', 'SignupRequest', 'SocialPersona', 'SocialPost', 'Solution', 'Task', 'Territory2', 'Territory2Model', 'Territory2Type', 'User',
-                            'UserAlt', 'UserProvAccount', 'UserProvisioningLog', 'UserProvisioningRequest', 'UserTerritory2Association', 'WorkProcedure', 'WorkProcedureStep', 'WorkTypeExtension'}
-        
-        # Objects that returns empty results if queried via the WHERE clause using Salesforce Tooling API.
-        # i.e. "Select LayoutId from ProfileLayout where TableEnumOrId = 'DelegatedAccount'" returns empty results.
-        UNQUERIABLE_ENUM_OBJECTS = {'DelegatedAccount','ProfileSkill','ProfileSkillEndorsement','ProfileSkillUser','ServiceTerritoryRelationship','WorkTypeExtension'}
-        
-        
-        
-        object_dataframe = pd.DataFrame(self.tooling_query_all("Select DeveloperName from CustomObject"))
-        object_dataframe['ObjectID'] = object_dataframe.apply(lambda row: row['attributes']['url'].split('/')[-1] if row['attributes']['url'] else "", axis=1)
-        
-        profile_layout_queries = []
-        
-        for object_name in objects_to_retrieve:
-            if object_name in UNQUERIABLE_ENUM_OBJECTS and discard_unqueriable_objects == False:
-                raise Exception("Unqueriable object: " + object_name + ". Please use retrieve_profile_layout_record_type_matrix_all() instead or set discard_unqueriable_objects parameter to True")
-            elif object_name in ENUM_OBJECTS:
-                profile_layout_queries.append("Select LayoutId, ProfileId, Profile.Name, RecordTypeId, RecordType.Name, Layout.Name, TableEnumOrId from ProfileLayout where TableEnumOrId = '" + object_name + "'")
-            else:
-                object_id = object_dataframe[object_dataframe['DeveloperName'] == object_name]['ObjectID'].values[0]
-                profile_layout_queries.append(f"Select LayoutId, ProfileId, Profile.Name, RecordTypeId, RecordType.Name, Layout.Name, TableEnumOrId from ProfileLayout where TableEnumOrId = '{object_id}'")
-        
-        
-        async_tooling_query_all = async_wrap(self.tooling_query_all)
-        
-        
-        await_results = await asyncio.gather(*[async_tooling_query_all(query) for query in profile_layout_queries])
-        
-        await_result_dataframe = [transform_sf_result_set_rec(result) for result in await_results if len(result) > 0]
-        
-        account_page_layouts_bulk = pd.concat(await_result_dataframe)
-
-        account_page_layouts_bulk['ProfileName'] = account_page_layouts_bulk.apply(lambda row: row['ProfileLayout.Profile']['Name'] if row['ProfileLayout.Profile'] else "", axis=1)
-        account_page_layouts_bulk['RecordTypeName'] = account_page_layouts_bulk.apply(lambda row: row['ProfileLayout.RecordType']['Name'] if row['ProfileLayout.RecordType'] else "", axis=1)
-        account_page_layouts_bulk['PageLayout'] = account_page_layouts_bulk.apply(lambda row: row['ProfileLayout.Layout']['Name'] if row['ProfileLayout.Layout'] else "", axis=1)
-        account_page_layouts_bulk.drop(['ProfileLayout.Profile','ProfileLayout.RecordType','ProfileLayout.Layout'], axis=1, inplace=True)
-
-        object_dataframe['ObjectID'] = object_dataframe.apply(lambda row: row['attributes']['url'].split('/')[-1] if row['attributes']['url'] else "", axis=1)
-
-        account_page_layouts_bulk = account_page_layouts_bulk.merge(object_dataframe, left_on='ProfileLayout.TableEnumOrId', right_on='ObjectID', how='left').copy()
-        account_page_layouts_bulk['DeveloperName'] = account_page_layouts_bulk.apply(lambda row: row['DeveloperName'] if pd.notnull(row['DeveloperName']) else row['ProfileLayout.TableEnumOrId'], axis=1)
-        account_page_layouts_bulk.drop(['attributes'], axis=1, inplace=True)
-        
-        # Fill in the RecordTypeName colum with the Master Record Type Name
-        account_page_layouts_bulk['RecordTypeName'] = account_page_layouts_bulk['RecordTypeName'].apply(lambda row: row if row else 'Master')
-        # Filter out Deprecated Profiles
-        account_page_layouts_bulk = account_page_layouts_bulk[(~account_page_layouts_bulk['ProfileName'].isnull()) & (account_page_layouts_bulk['ProfileName'] != '') & (account_page_layouts_bulk['PageLayout'] != 'Veeva Vpro Unit Testing Layout')].copy()
-        
-        if self.instance.__contains__("my.salesforce.com"):
-            sf_meta_instance = self.instance.replace(".my.salesforce.com","")
-        else:
-            sf_meta_instance = ".".join(self.instance.split(".")[:1])
-        
-        account_page_layouts_bulk['Edit Link'] = account_page_layouts_bulk.apply(lambda row: "https://" + sf_meta_instance + ".lightning.force.com/lightning/setup/ObjectManager/" + (row['DeveloperName'] if str(row['ObjectID']) == 'nan' else row['ObjectID']) + "/PageLayouts/" + row['ProfileLayout.LayoutId'] + "/view", axis=1)
-        
-        if return_pivot_table:
-            return account_page_layouts_bulk.pivot(index='ProfileName', columns=['DeveloperName','RecordTypeName'], values='PageLayout')
-        else:
-            return account_page_layouts_bulk
-
-    async def field_permission_user_check(self, objects: list[str], permissions: list[str], users=None) -> pd.DataFrame:
-        # Similar to the field_permission_check function, but this one will return a list of users that have the specified permission on the specified object
-        
-        # this is to avoid having a mutable default argument
-        users = [] if users is None else users
-        
-        object_query = "','".join(objects)
-        permission_query = ' OR '.join([f"({permission} = true)" for permission in permissions])
-
-        relevant_ps_and_profiles = transform_sf_result_set_rec(self.sf.query_all(f"""
-                                                SELECT ParentId,
-                                                        Field,
-                                                        PermissionsEdit,
-                                                        PermissionsRead
-                                                FROM FieldPermissions
-                                                WHERE SObjectType IN ('{object_query}') AND
-                                                ({permission_query})
-                                                """)['records'])
-
-        relevant_ps_and_profiles['Object API Name'] = relevant_ps_and_profiles['FieldPermissions.Field'].apply(lambda row: row.split('.')[0])
-        relevant_ps_and_profiles['Field API Name'] = relevant_ps_and_profiles['FieldPermissions.Field'].apply(lambda row: row.split('.')[1])
-        relevant_ps_and_profiles.drop(columns=['FieldPermissions.Field'], inplace=True)
-
-        user_query = (" AND Assignee.UserName IN ('" + "','".join(users) + "')") if len(users) > 0 else ""
-
-        relevant_ps_and_profiles_list = "','".join(relevant_ps_and_profiles['FieldPermissions.ParentId'].unique().tolist())
-
-        data = transform_sf_result_set_rec(self.sf.query_all(f"""SELECT Assignee.Id, Assignee.Name,Assignee.IsActive, 
-                                                                Assignee.UserName, PermissionSet.Id, 
-                                                                PermissionSet.isOwnedByProfile, PermissionSet.Profile.Name, PermissionSet.Label
-                                                                FROM PermissionSetAssignment
-                                                                WHERE PermissionSetId
-                                                                IN ('{relevant_ps_and_profiles_list}')
-                                                                {user_query} AND Assignee.IsActive = TRUE""")['records'])
-        
-        if len(data) == 0:
-            return pd.DataFrame(columns=['UserName', 'Profile', 'Field API Name', 'Object API Name','Permission', 'Permission Set'])
-        
-        # Retrieve Profile FLS data
-        profiles = data[data['PermissionSet.IsOwnedByProfile']]['Profile.Name'].unique().tolist()
-        profiles = ['Admin' if x == 'System Administrator' else x for x in profiles]
-
-
-        async_metadata_read = async_wrap(self.metadata_read)
-        profile_metadata_tasks = {}
-        profile_metadata_dict = {}
-
-        for profile in profiles:
-                profile_metadata_tasks[profile] = asyncio.create_task(async_metadata_read('Profile', profile))
-
-
-        task_result_list = await asyncio.gather(*profile_metadata_tasks.values())
-
-
-        for profile in profiles:
-                profile_metadata_dict["System Administrator" if profile == 'Admin' else profile] = pd.DataFrame(task_result_list[profiles.index(profile)]['fieldPermissions'][0])
-    
-        data = data.merge(relevant_ps_and_profiles, left_on='PermissionSet.Id', right_on='FieldPermissions.ParentId', how='left').copy()
-        if (len(data) > 0):
-                
-                profile_violations = data[data['PermissionSet.IsOwnedByProfile']== True][['User.Username', 'Profile.Name']].drop_duplicates().copy()
-                # profile_violations = data[data['PermissionSet.IsOwnedByProfile']== True][['User.Username', 'Profile.Name','Field API Name']]
-                profile_metadata_pd = pd.concat(profile_metadata_dict.values(), keys=profile_metadata_dict.keys(), names=['Profile', 'Index']).reset_index(level=1, drop=True).reset_index()
-                profile_metadata_pd.rename(columns={'Profile': 'Profile.Name'}, inplace=True)
-                profile_metadata_pd['Field API Name'] = profile_metadata_pd['field'].str.split('.').str[1]
-                profile_metadata_pd['Object API Name'] = profile_metadata_pd['field'].str.split('.').str[0]
-                profile_metadata_pd = profile_metadata_pd[profile_metadata_pd['Object API Name'].isin(objects)].copy()
-                profile_metadata_pd.drop(columns=['field'], inplace=True)
-
-                # if permission == 'PermissionsEdit':
-                #         profile_metadata_pd = profile_metadata_pd[profile_metadata_pd['editable'] == True].copy()
-                #         profile_metadata_pd.drop(columns=['editable', 'readable'], inplace=True)
-                # elif permission == 'PermissionsRead':
-                #         profile_metadata_pd = profile_metadata_pd[profile_metadata_pd['readable'] == True].copy()
-                #         profile_metadata_pd.drop(columns=['editable', 'readable'], inplace=True)
-                
-                profile_violations = profile_violations.merge(profile_metadata_pd, on='Profile.Name', how='left').copy()
-                profile_editable = profile_violations[profile_violations['editable'] == True].drop(columns=['editable','readable']).copy()
-                profile_editable['Permission'] = 'PermissionsEdit'
-                profile_readable = profile_violations[profile_violations['readable'] == True].drop(columns=['editable','readable']).copy()
-                profile_readable['Permission'] = 'PermissionsRead'
-
-                profile_fls_final = pd.concat([profile_editable, profile_readable])
-                profile_fls_final.columns = ['UserName','Profile','Field API Name','Object API Name','Permission']
-                
-                permission_set_violations = data[data['PermissionSet.IsOwnedByProfile']== False][['User.Username', 'PermissionSet.Label', 'Object API Name', 'FieldPermissions.PermissionsEdit','FieldPermissions.PermissionsRead','Field API Name']]
-                
-                ps_editable = permission_set_violations[permission_set_violations['FieldPermissions.PermissionsEdit'] == True].drop(columns=['FieldPermissions.PermissionsEdit','FieldPermissions.PermissionsRead']).copy()
-                ps_editable['Permission'] = 'PermissionsEdit'
-                ps_readable = permission_set_violations[permission_set_violations['FieldPermissions.PermissionsRead'] == True].drop(columns=['FieldPermissions.PermissionsEdit','FieldPermissions.PermissionsRead']).copy()
-                ps_readable['Permission'] = 'PermissionsRead'
-                
-                ps_fls_final = pd.concat([ps_editable, ps_readable])
-                ps_fls_final.columns = ['UserName','Permission Set','Object API Name','Field API Name', 'Permission']
-                
-                return pd.merge(profile_fls_final, ps_fls_final, on=['UserName','Object API Name', 'Field API Name','Permission'], how='outer')
-        else:
-                return pd.DataFrame(columns=['UserName', 'Profile', 'Field API Name', 'Object API Name','Permission', 'Permission Set'])
-          
-            
-    async def retrieve_user_profile_record_type_details(self, username: str, objects: list[str]):
-        
-        profile_metadata = pd.DataFrame(zeep.helpers.serialize_object(self.metadata_list("Profile")))
-        profile_metadata = profile_metadata[['id', 'fullName']].copy()
-        profile_metadata
-        user_profile_id = transform_sf_result_set_rec(self.sf.query_all(f"Select Id, ProfileId FROM User WHERE Username = '{username}'")['records'])
-        if len(profile_metadata[profile_metadata['id'] == user_profile_id['User.ProfileId'].values[0]]['fullName']) == 0:
-            raise Exception("User does not have a retrievable / valid profile")
-        else:
-            user_profile = profile_metadata[profile_metadata['id'] == user_profile_id['User.ProfileId'].values[0]]['fullName'].values[0]
-
-        async_profile_read = async_wrap(self.metadata_read)
-        
-        user_profile_metadata = async_profile_read('Profile', user_profile)
-        
-        results = {}
-        
-        async_object_describe = async_wrap(self.object_describe)
-        
-        tasks = {}
-        
-        for object in objects:
-            tasks[object] = async_object_describe(object)
-        tasks['get_profile_data'] = user_profile_metadata
-        
-        task_result_list = await asyncio.gather(*tasks.values())
-        
-        task_result_dict = {}
-        
-        for object in objects:
-            task_result_dict[object] = task_result_list[objects.index(object)]
-            
-        task_result_dict['get_profile_data'] = task_result_list[-1]
-        
-        user_rt_visibilities = pd.DataFrame(task_result_dict['get_profile_data']['recordTypeVisibilities'][0])
-        user_rt_visibilities['Object'] = user_rt_visibilities['recordType'].apply(lambda x: x.split('.')[0])
-        user_rt_visibilities['RecordType'] = user_rt_visibilities['recordType'].apply(lambda x: x.split('.')[1])
-        
-        for object in objects:
-            if object.lower() == 'account':
-                object_describe = task_result_dict[object]['recordTypeInfos'].T
-                object_record_types = object_describe[object_describe['active'] == True].reset_index()[['name','defaultRecordTypeMapping','developerName','master','recordTypeId']].copy()
-                user_object_rt_visibilities = user_rt_visibilities[(user_rt_visibilities['Object'] == object) | (user_rt_visibilities['Object'] == 'PersonAccount')][['default','personAccountDefault','Object','RecordType','visible']].copy()
-                
-            else:
-                object_describe = task_result_dict[object]['recordTypeInfos'].T
-                object_record_types = object_describe[object_describe['active'] == True].reset_index()[['name','defaultRecordTypeMapping','developerName','master','recordTypeId']].copy()
-                user_object_rt_visibilities = user_rt_visibilities[user_rt_visibilities['Object'] == object][['default','personAccountDefault','Object','RecordType','visible']].copy()
-
-            object_rt_visibility_with_master = pd.merge(user_object_rt_visibilities, object_record_types, left_on='RecordType', right_on='developerName', how='outer')
-            object_rt_visibility_with_master['visible'].fillna(False, inplace=True)
-            if not object_rt_visibility_with_master['visible'].any():
-                object_rt_visibility_with_master.loc[object_rt_visibility_with_master['developerName'] == 'Master', 'visible'] = True
-            if not object_rt_visibility_with_master['default'].any():
-                object_rt_visibility_with_master.loc[object_rt_visibility_with_master['developerName'] == 'Master', 'default'] = True
-                
-            visible_object_rt = object_rt_visibility_with_master[object_rt_visibility_with_master['visible'] == True].drop(['defaultRecordTypeMapping'], axis=1)
-            results[object] = visible_object_rt
-        
-        return results
-    
-    
-    async def permissionable_fields_bulk_check(self, object_list):
-        permissionable_fields = {}
-        nonpermissionable_fields = {}
-        async_permissionable_fields =  async_wrap(self.object_describe)
-        async_metadata_read = async_wrap(self.metadata_read)
-        
-        
-        task_dict = {}
-        task_result_dict = {}
-        
-        for object_name in object_list:
-            task_dict[object_name] = async_permissionable_fields(object_name)
-            task_dict[object_name + '_metadata'] = async_metadata_read('CustomObject', object_name)
-            
-        task_results = await asyncio.gather(*task_dict.values())
-        
-        for object_name, task_result in zip(task_dict.keys(), task_results):
-            task_result_dict[object_name] = task_result
-        
-        
-        for object in object_list:
-            permissionable_fields[object] = pd.DataFrame(task_result_dict[object + "_metadata"]['fields'][0])['fullName'].to_list()
-            
-            nonpermissionable_fields[object] = task_result_dict[object]['fields'].T[task_result_dict[object]['fields'].T['permissionable'] == False].index.tolist()
-        return permissionable_fields, nonpermissionable_fields, task_result_dict
-    
-    async def get_layout_metadata(self, layout_name):
-        # Layout Name is the Object API Name + Page Layout Name of the layout, for example:
-        # Account-Hospital Department
-        
-        async_metadata_read = async_wrap(self.metadata_read)
-        
-        layout_metadata = await async_metadata_read('Layout', layout_name)
-        
-        def parse_layoutSections(layout_metadata):
-            layoutSections = pd.DataFrame(layout_metadata)
-            layoutSections['layoutColumns'] = layoutSections['layoutColumns'].apply(lambda row: list(filter(lambda item: item is not None, row)))
-            layoutSections = layoutSections.explode('layoutColumns').reset_index(drop=True)
-            layoutSections['layoutColumns'] = layoutSections['layoutColumns'].apply(lambda row: "" if str(row) == 'nan' else row['layoutItems'])
-            layoutSections = layoutSections.explode('layoutColumns').reset_index(drop=True)
-            layoutSections = pd.concat([layoutSections, layoutSections['layoutColumns'].apply(pd.Series, dtype=str).add_prefix('layoutColumns.')], axis=1).drop(['layoutColumns', "layoutColumns.0"], axis=1)
-            layoutSections.fillna("", inplace=True)
-            layoutSections.drop_duplicates(inplace=True)
-            return layoutSections
-
-        def parse_platformActionList(platformActionList_metadata):
-            platformActionList = pd.DataFrame(platformActionList_metadata)
-            platformActionList = pd.concat([platformActionList, platformActionList['platformActionListItems'].apply(pd.Series, dtype=str).add_prefix('platformActionListItems.')], axis=1).drop(['platformActionListItems'], axis=1)
-            return platformActionList
-
-
-        def parse_quickActionList(quickActionList_metadata):
-            quickActionList = pd.DataFrame(quickActionList_metadata)
-            quickActionList = pd.concat([quickActionList, quickActionList['quickActionListItems'].apply(pd.Series, dtype=str).add_prefix('quickActionListItems.')], axis=1).drop(['quickActionListItems'], axis=1)
-            return quickActionList
-
-        parsed_layout_metadata = {}
-        parsed_layout_metadata['customButtonsList'] = layout_metadata['customButtons'][0]
-        parsed_layout_metadata['excludeButtonsList'] = layout_metadata['excludeButtons'][0]
-        # Adding required fields from the main page layout gives you the final list of mini layout items
-        parsed_layout_metadata['miniLayoutDict'] = dict(layout_metadata['miniLayout'][0]) if layout_metadata['miniLayout'][0] != None else {'fields': [],'relatedLists': []}
-        parsed_layout_metadata['layoutSectionsDataFrame'] = parse_layoutSections(layout_metadata['layoutSections'][0]) if layout_metadata['layoutSections'][0] != None else pd.DataFrame()
-        parsed_layout_metadata['platformActionListDataFrame'] = parse_platformActionList(layout_metadata['platformActionList'][0]) if layout_metadata['platformActionList'][0] != None else pd.DataFrame()
-        parsed_layout_metadata['quickActionListDataFrame'] = parse_quickActionList(layout_metadata['quickActionList'][0]) if layout_metadata['quickActionList'][0] != None else pd.DataFrame()
-        parsed_layout_metadata['relatedListDataFrame'] = pd.DataFrame(layout_metadata['relatedLists'][0]) if layout_metadata['relatedLists'][0] != None else pd.DataFrame()
-        return parsed_layout_metadata
-    
-    ### ----------------------------------------------------------------------------------------------------
-    ### Synchronous Metadata Functions
-    ### ----------------------------------------------------------------------------------------------------
-
-    def object_describe(self, sobject_api_name: str, export_excel: bool=False):
-        """
-
-        """
-        sfSchema = getattr(self.sf, sobject_api_name).describe()
-        boolMetadata = {}
-        nonetypeMetadata = {}
-        strMetadata = {}
-        orderedDictMetadata = pd.Series(dtype='object')
-        childRelationshipsPD = pd.DataFrame()
-        recordTypeInfosPD = pd.DataFrame()
-        fieldsPD = pd.DataFrame()
-        supportedScopesPD = pd.DataFrame()
-        namedLayoutInfosPD = pd.DataFrame()
-        actionOverridesPD = pd.DataFrame()
-
-        for metadata in sfSchema:
-            ## Processes all metadata that would return a boolean datatype
-            if type(sfSchema[metadata]) is bool:
-                boolMetadata[metadata] = sfSchema[metadata]
-
-            ## Processes all metadata that would return a NoneType datatype
-            elif type(sfSchema[metadata]) == type(None):
-                nonetypeMetadata[metadata] = sfSchema[metadata]
-
-            ## Processes all metadata that would return a string datatype
-            elif type(sfSchema[metadata]) is str:
-                strMetadata[metadata] = sfSchema[metadata]
-            ## Processes all metadata that would return an OrderedDict data type
-            elif type(sfSchema[metadata]) is OrderedDict and len(sfSchema[metadata]) != 0:
-                orderedDictMetadata = pd.concat([orderedDictMetadata,pd.Series(sfSchema['urls'])])
-            elif type(sfSchema[metadata]) is OrderedDict and len(sfSchema[metadata]) == 0:
-                nonetypeMetadata[metadata] = "None"
-
-            ## Processes all metadata that would return a list data type
-            elif type(sfSchema[metadata]) is list and len(sfSchema[metadata]) != 0:
-                if metadata == 'childRelationships':
-                    childRelationshipsPD = pd.DataFrame(sfSchema['childRelationships'], index = pd.DataFrame(sfSchema['childRelationships'])['field'])
-                    childRelationshipsPD = childRelationshipsPD.drop('field', axis=1).T
-                if metadata == 'recordTypeInfos':
-                    recordTypeInfosPD = pd.DataFrame(sfSchema['recordTypeInfos'], index = pd.DataFrame(sfSchema['recordTypeInfos'])['name'])
-                    recordTypeInfosPD = recordTypeInfosPD.drop('name', axis = 1).T  
-                if metadata == 'fields':
-                    fieldsPD = pd.DataFrame(sfSchema['fields'], index = pd.DataFrame(sfSchema['fields'])['name'])
-                    fieldsPD = fieldsPD.drop('name', axis = 1).T
-                if metadata == 'supportedScopes':
-                    supportedScopesPD = pd.DataFrame(sfSchema['supportedScopes'], index = pd.DataFrame(sfSchema['supportedScopes'])['name'])
-                    supportedScopesPD = supportedScopesPD.drop('name', axis = 1).T
-                if metadata == 'actionOverrides':
-                    actionOverridesPD = pd.DataFrame(sfSchema['actionOverrides'], index = pd.DataFrame(sfSchema['actionOverrides'])['name'])
-                    actionOverridesPD = actionOverridesPD.drop('name', axis = 1).T
-                if metadata == 'namedLayoutInfos':
-                    namedLayoutInfosPD = pd.DataFrame(sfSchema['namedLayoutInfos'], index = pd.DataFrame(sfSchema['namedLayoutInfos'])['name'])
-                    namedLayoutInfosPD = namedLayoutInfosPD.drop('name', axis = 1).T
-            ## Parses all empty list metadata
-            elif type(sfSchema[metadata]) is list and len(sfSchema[metadata]) == 0:
-                nonetypeMetadata[metadata] = "None"
-            else:
-                nonetypeMetadata[metadata] = "Unrecognized metadata type: " + metadata
-
-        output = {'metadata': pd.concat([pd.Series(nonetypeMetadata),
-                    pd.Series(boolMetadata),
-                    pd.Series(strMetadata),
-                    orderedDictMetadata]),
-                    'childRelationships': childRelationshipsPD if len(childRelationshipsPD)!=0 else None,
-                    'recordTypeInfos': recordTypeInfosPD if len(recordTypeInfosPD)!=0 else None,
-                    'fields': fieldsPD if len(fieldsPD)!=0 else None,
-                    'supportedScopes': supportedScopesPD if len(supportedScopesPD)!=0 else None, 
-                    'namedLayoutInfos': namedLayoutInfosPD if len(namedLayoutInfosPD)!=0 else None,
-                    'actionOverrides': actionOverridesPD if len(actionOverridesPD)!=0 else None}
-        if export_excel:
-            with pd.ExcelWriter(sobject_api_name + ' describe output.xlsx') as writer:  
-                for key in output.keys():
-                    try:
-                        pd.DataFrame(output[key]).to_excel(writer, sheet_name=key)
-                    except:
-                        continue
-
-        return output
-
-    def field_describe(self, objects: List = ['Account','Address_vod__c','Child_Account_vod__c'], 
-    attributes: List = ['name','type','length']) -> pd.DataFrame:
-        """
-        Returns a dataframe of the field metadata for the specified objects and attributes.
-
-        Parameters
-        ----------
-        objects : List, optional
-            A list of objects to get field metadata for. The default is ['Account','Address_vod__c','Child_Account_vod__c'].
-        attributes : List, optional
-            A list of attributes to get field metadata for. The default is ['name','type','length'].
-            For a full list of attributes, see 
-            https://developer.salesforce.com/docs/atlas.en-us.api.meta/api/sforce_api_calls_describesobjects_describesobjectresult.htm
-            A list of attributes can also be found by using the object_describe() method's field attribute.
-
-        Returns
-        -------
-        pd.DataFrame
-            A dataframe of the field metadata for the specified objects and attributes.
-        
-        """
-        outputList = []
-        columnNames = []
-        for sObjectAPIName in objects:
-            for attribute in attributes:
-                outputList.append([field[attribute] for field in getattr(self.sf, sObjectAPIName).describe()['fields']])
-                if attribute == "name":
-                    columnNames.append(sObjectAPIName)
-                else:
-                    columnNames.append(attribute.title())
-        field_describe = pd.DataFrame(outputList).transpose()
-        field_describe.columns = columnNames
-        return field_describe
-
-    def set_user_password(self, user_id, new_password):
-        result = {}
-        try:
-            result = self.sf_api_call(f'/services/data/{self.api_version}/sobjects/User/{user_id}/password', method='POST', data={'NewPassword': new_password})
-        except Exception as e:
-            message_list = str(e).split(" : ")[1].strip().removeprefix("b'[").removesuffix("]'")
-            result = ast.literal_eval(message_list)
-            result['user_id'] = user_id
-        
-        if len(result) == 0:
-            result = {'user_id': user_id,'message': 'success',  'errorCode': None}
-        return result
-        
-
-    def picklist_dataframe_stacked(self,objects: List =['Account','Address_vod__c','Child_Account_vod__c']) -> pd.DataFrame:
-        """
-        TODO:
-        
-        Description of what it does
-        
-        Description of arguments and data types
-        
-        Description of return values and data types
-        
-        Description of Errors raised
-        
-        Extra Notes and Examples of Usage
-        """
-        output_df = pd.DataFrame()
-        for object in objects:
-            objectDescribe = getattr(self.sf, object).describe()
-            processing_df = pd.DataFrame(pd.DataFrame([pd.Series(data = [picklist['value'] for picklist in field['picklistValues']], 
-                                                                   name = object + "." + field["name"]) for field in objectDescribe['fields'] if field['type'] == 'picklist']).stack())
-            processing_df.columns = ['Picklist API Value']
-            processing_df['CRM Object and Field API'] = processing_df.index.get_level_values(0)
-            processing_df[['CRM Object API','CRM Field API']] = processing_df['CRM Object and Field API'].str.split(".", expand = True)
-            processing_df.reset_index(drop=True, inplace=True)
-            output_df = pd.concat([output_df,processing_df])
-        return output_df
-
-    def picklist_dataframe(self,objects = ['Account','Address_vod__c','Child_Account_vod__c']) -> List:
-        """
-        TODO:
-        
-        Description of what it does
-        
-        Description of arguments and data types
-        
-        Description of return values and data types
-        
-        Description of Errors raised
-        
-        Extra Notes and Examples of Usage
-        """
-        referenceList = []
-        for object in objects:
-            objectDescribe = getattr(self.sf, object).describe()
-            objectPicklistValues = pd.DataFrame(index=range(0,max(len(field["picklistValues"]) for field in objectDescribe['fields'] if field['type'] == 'picklist')))
-            for x in [pd.Series(data = [picklist['value'] for picklist in field['picklistValues']], name = object + "." + field["name"]) for field in objectDescribe['fields'] if field['type'] == 'picklist']:
-                objectPicklistValues.insert(0, str(x.name), x)
-            referenceList.append(objectPicklistValues)
-        return referenceList
-
-    def record_type_retrieval(self, objectAPIName, fieldAPINames = ["Id","Name",'SobjectType', 'IsActive']):
-        """
-        TODO:
-        
-        Description of what it does
-        
-        Description of arguments and data types
-        
-        Description of return values and data types
-        
-        Description of Errors raised
-        
-        Extra Notes and Examples of Usage
-        """
-        sfRTDF = pd.DataFrame(self.sf.query_all("SELECT "+ ",".join(fieldAPINames) + " from RecordType WHERE SobjectType = '" + objectAPIName + "'")['records'])
-        
-        # If only master RT exists
-        if len(sfRTDF) == 0:
-            master_rt = {
-                "Name": "Master",
-                "DeveloperName": "Master",
-                "IsActive": True,
-            }
-
-            sfRTDF = pd.DataFrame(master_rt, index=[0])
-        else:
-            sfRTDF.drop(columns="attributes", inplace = True)
-        return sfRTDF
-
-    def object_permission_check(self, object, permission):
-        data = transform_sf_result_set_rec(self.sf.query_all(f"""SELECT Assignee.Id, Assignee.Name,Assignee.IsActive, Assignee.UserName, PermissionSet.Id, PermissionSet.isOwnedByProfile, PermissionSet.Profile.Name, PermissionSet.Label
-            FROM PermissionSetAssignment
-            WHERE PermissionSetId
-            IN (SELECT ParentId
-            FROM ObjectPermissions
-            WHERE SObjectType IN ('{object}') AND
-            ({permission} = true)) AND Assignee.IsActive = TRUE""")['records'])
-        
-        profile_violations = data[data['PermissionSet.IsOwnedByProfile']== True][['User.Username', 'Profile.Name']]
-        permission_set_violations = data[data['PermissionSet.IsOwnedByProfile']== False][['User.Username', 'PermissionSet.Label']]
-        result = []
-        for user in profile_violations['User.Username'].unique():
-            result.append({"UserName": user, 
-                            "Object API Name" : object,
-                            "Permission": permission,
-                            "Profile": "; ".join(list(profile_violations[profile_violations['User.Username'] == user]['Profile.Name'].unique())),
-                            "Permission Set": ""
-                        
-                        }
-                        
-                        )
-            
-        for user in permission_set_violations['User.Username'].unique():
-            result.append({"UserName": user, 
-                                                            "Object API Name" : object,
-                                                            "Permission": permission,
-                                                            "Profile": "",
-                                                            "Permission Set": "; ".join(list(permission_set_violations[permission_set_violations['User.Username'] == user]['PermissionSet.Label'].unique()))})
-        return result
-
-    def field_permission_check(self, object) -> dict[str, pd.DataFrame]:
-        fls_results = transform_sf_result_set_rec(self.sf.query_all(f"""
-                                            SELECT Field,
-                                            ParentId,
-                                            PermissionsEdit,
-                                            PermissionsRead,
-                                            SobjectType FROM FieldPermissions
-                                            WHERE SobjectType in ('{object}')
-                                            """)['records'])
-
-        permissionSetProfiles = transform_sf_result_set_rec(self.sf.query_all("""
-                                                    SELECT Id,Description,IsOwnedByProfile,Name,ProfileId, 
-                                                    Profile.Name, Profile.Description,Type FROM PermissionSet
-                                                    """)['records'])
-
-        profiles = permissionSetProfiles[permissionSetProfiles['PermissionSet.IsOwnedByProfile'] == True][['PermissionSet.ProfileId','PermissionSet.Id','Profile.Name','Profile.Description']].copy()
-        permissionSets = permissionSetProfiles[permissionSetProfiles['PermissionSet.IsOwnedByProfile'] == False][['PermissionSet.Id','PermissionSet.Name','PermissionSet.Description']].copy()
-
-        permissionSetPermissions = pd.merge(fls_results, permissionSets, left_on='FieldPermissions.ParentId', right_on='PermissionSet.Id', how='inner').drop(columns=['PermissionSet.Id'], axis=1)
-        permissionSetPermissions.columns = ['Field API Name', 'Permission Set Id', 'FLS Edit', 'FLS Read', 'Object API Name', 'Permission Set Name', 'Permission Set Description']
-        permissionSetPermissions = permissionSetPermissions[['Permission Set Id', 'Permission Set Name', 'Permission Set Description', 'Object API Name', 'Field API Name', 'FLS Edit', 'FLS Read']]
-        permissionSetPermissions['Field API Name'] = permissionSetPermissions['Field API Name'].apply(lambda x: x.split('.')[-1])
-
-
-        profilePermissions = pd.merge(fls_results, profiles, left_on='FieldPermissions.ParentId', right_on='PermissionSet.Id', how='inner').drop(columns=['PermissionSet.Id','FieldPermissions.ParentId'], axis=1)
-        profilePermissions.columns = ['Field API Name', 'FLS Edit', 'FLS Read', 'Object API Name','Profile Id',  'Profile Name', 'Profile Description']
-        profilePermissions = profilePermissions[['Profile Id', 'Profile Name', 'Profile Description', 'Object API Name', 'Field API Name', 'FLS Edit', 'FLS Read']]
-        profilePermissions['Field API Name'] = profilePermissions['Field API Name'].apply(lambda x: x.split('.')[-1])
-        
-        return {'permissionSetPermissions': permissionSetPermissions, 'profilePermissions': profilePermissions}
-
-
-    # Retrieves the Page Layout by Profile by Record Type data for all objects in the org
-    def retrieve_profile_layout_record_type_matrix_all(self, return_pivot_table = False):
-        account_page_layouts_bulk = transform_sf_result_set_rec(self.tooling_query_all("""select LayoutId, 
-                                                                                    ProfileId, Profile.Name, 
-                                                                                    RecordTypeId, RecordType.Name, 
-                                                                                    Layout.Name, TableEnumOrId from 
-                                                                                    ProfileLayout"""))
-
-        account_page_layouts_bulk['ProfileName'] = account_page_layouts_bulk.apply(lambda row: row['ProfileLayout.Profile']['Name'] if row['ProfileLayout.Profile'] else "", axis=1)
-        account_page_layouts_bulk['RecordTypeName'] = account_page_layouts_bulk.apply(lambda row: row['ProfileLayout.RecordType']['Name'] if row['ProfileLayout.RecordType'] else "", axis=1)
-        account_page_layouts_bulk['PageLayout'] = account_page_layouts_bulk.apply(lambda row: row['ProfileLayout.Layout']['Name'] if row['ProfileLayout.Layout'] else "", axis=1)
-        account_page_layouts_bulk.drop(['ProfileLayout.Profile','ProfileLayout.RecordType','ProfileLayout.Layout'], axis=1, inplace=True)
-
-
-        object_dataframe = pd.DataFrame(self.tooling_query_all("Select DeveloperName from CustomObject"))
-        object_dataframe['ObjectID'] = object_dataframe.apply(lambda row: row['attributes']['url'].split('/')[-1] if row['attributes']['url'] else "", axis=1)
-
-
-        account_page_layouts_bulk = account_page_layouts_bulk.merge(object_dataframe, left_on='ProfileLayout.TableEnumOrId', right_on='ObjectID', how='left').copy()
-        account_page_layouts_bulk['DeveloperName'] = account_page_layouts_bulk.apply(lambda row: row['DeveloperName'] if pd.notnull(row['DeveloperName']) else row['ProfileLayout.TableEnumOrId'], axis=1)
-        account_page_layouts_bulk.drop(['ObjectID','attributes'], axis=1, inplace=True)
-            
-        # Fill in the RecordTypeName colum with the Master Record Type Name
-        account_page_layouts_bulk['RecordTypeName'] = account_page_layouts_bulk['RecordTypeName'].apply(lambda row: row if row else 'Master')
-        # Filter out Deprecated Profiles
-        account_page_layouts_bulk = account_page_layouts_bulk[(~account_page_layouts_bulk['ProfileName'].isnull()) & (account_page_layouts_bulk['ProfileName'] != '') & (account_page_layouts_bulk['PageLayout'] != 'Veeva Vpro Unit Testing Layout')]
-        
-        if return_pivot_table:
-            return account_page_layouts_bulk.pivot(index='ProfileName', columns=['DeveloperName','RecordTypeName'], values='PageLayout')
-        else:
-            return account_page_layouts_bulk
-    
-
-    def load_veeva_common(self):
-        self.veeva_common = self.query("Select * From Veeva_Common_vod__c").to_dict()
-    
-    def load_org_info(self):
-        self.org_info = self.query("Select * From Organization").to_dict()
-        
-    def get_network_admin_sf_user_info(self):
-        
-        if self.veeva_common is None:
-            self.load_veeva_common()
-        
-        if self.org_info is None:
-            self.load_org_info()
-            
-        try:
-            response = requests.get(f"{self.veeva_common['Veeva_Server_vod__c'][0]}/{self.veeva_common['Veeva_Version_vod__c'][0]}?VER={self.veeva_common['Veeva_Version_vod__c'][0]}&SSID={self.session_id}&url=https://{self.instance}/services/Soap/u/24.0/{self.org_info['Id'][0]}&ses={self.session_id}&oType=networkAdmin&event=getSFCredentials")
-            return {'status': response.status_code, 'response': response.json()}
-        except:
-            return {'status': 500, 'response': {"error": "Unable to get network admin credentials"}}
-        
-    def get_network_admin_network_user_info(self):
-        
-        if self.veeva_common is None:
-            self.load_veeva_common()
-        
-        if self.org_info is None:
-            self.load_org_info()
-            
-        try:
-            response = requests.get(f"{self.veeva_common['Veeva_Server_vod__c'][0]}/{self.veeva_common['Veeva_Version_vod__c'][0]}?VER={self.veeva_common['Veeva_Version_vod__c'][0]}&SSID={self.session_id}&url=https://{self.instance}/services/Soap/u/24.0/{self.org_info['Id'][0]}&ses={self.session_id}&oType=networkAdmin&event=getNetworkCredentials")
-            return {'status': response.status_code, 'response': response.json()}
-        except:
-            return {'status': 500, 'response': {"error": "Unable to get network admin credentials"}}
-
-    @serialze_zeep
-    def metadata_read(self, metadata_type: str, fullName: str):
-        return getattr(self.sf.mdapi, metadata_type).read(fullName)
-
-    def metadata_delete(self, metadata_type: str, fullName: str):
-        return getattr(self.sf.mdapi, metadata_type).delete(fullName)
-
-    def metadata_update(self, metadata_type: str, parsed_metadata: dict):
-        mdapi_object = getattr(self.sf.mdapi, metadata_type)()
-        for key in parsed_metadata:
-            setattr(mdapi_object, key, parsed_metadata[key])
-        getattr(self.sf.mdapi, metadata_type).update(mdapi_object)
-        return mdapi_object
-
-    def metadata_create(self, metadata_type: str, parsed_metadata: dict):
-        mdapi_object = getattr(self.sf.mdapi, metadata_type)()
-        for key in parsed_metadata:
-            setattr(mdapi_object, key, parsed_metadata[key])
-        getattr(self.sf.mdapi, metadata_type).create(mdapi_object)
-        return mdapi_object
-
-    def metadata_list(self, metadata_type: str = '', metadata_type_list: list[str] = []) -> list:
-        if len(metadata_type_list) == 0 and metadata_type != '':
-            query = self.sf.mdapi.ListMetadataQuery(type=metadata_type)
-        elif len(metadata_type_list) > 3:
-            raise Exception("You can only query up to 3 metadata types at a time")
-        
-        elif len(metadata_type_list) > 0:
-            query = []
-            for metadata_type in metadata_type_list:
-                query.append(self.sf.mdapi.ListMetadataQuery(type=metadata_type))
-        else:
-            raise Exception("Please populate either metadata_type or metadata_type_list, but not both.")
-        
-        query_response = self.sf.mdapi.list_metadata(query)
-        return query_response
-    
-    def metadata_rename(self, metadata_type: str, previous_name: str, new_name: str): 
-        """
-        Renames the API name of SFDC metadata
-        """
-        getattr(self.sf.mdapi, metadata_type).rename(previous_name, new_name)
-    
-    ### ----------------------------------------------------------------------------------------------------
-    ### Custom Tooling API Methods
-    ### ----------------------------------------------------------------------------------------------------
-    
-    def tooling_query_all(self, query):
-        done = False
-        full_results = []
-        result = self.sf_api_call(f'/services/data/v52.0/tooling/query', method='get', parameters={'q': query})
-        while not done:
-            full_results.extend(result['records'])
-            done = result['done']
-            if not done:
-                result = self.sf_api_call(result['nextRecordsUrl'])
-        return full_results
-
-    ### ----------------------------------------------------------------------------------------------------
-    ### Utility Functions
-    ### ----------------------------------------------------------------------------------------------------
-    def query_performance_feedback(self, query: str):
-        # https://developer.salesforce.com/docs/atlas.en-us.240.0.api_rest.meta/api_rest/dome_query_explain.htm
-        
-        return self.sf_api_call(f'/services/data/{self.api_version}/query?explain={query}')
-    
-    def parse_sf_limits(self, sfdc_limits_result: dict, prefix=None) -> dict:
-        ## Recursively parse the limits result to find the limits that are not 0
-        result = {}
-        for key, item in sfdc_limits_result.items():
-            if set(['Max','Remaining']).issubset(set(item.keys())): 
-                if item['Max'] == 0:
-                    continue
-                else:
-                    result[key if prefix is None else prefix+' - '+key] = dict(zip(['Max','Remaining'],[item['Max'], item['Remaining']]))
-            
-            if len(set(item.keys()) - set(['Max','Remaining'])) > 0:
-                sub_item = item.copy()
-                if 'Max' in sub_item: 
-                    del sub_item['Max']
-                if 'Remaining' in sub_item: 
-                    del sub_item['Remaining']
-                result.update(self.parse_sf_limits(sub_item, prefix=key))
-        return result
-        
-    def sf_api_call(self, action, parameters = {}, method = 'get', data = {}):
-        """
-        Helper function to make calls to Salesforce REST API.
-        Parameters: action (the URL), URL params, method (get, post or patch), data for POST/PATCH.
-        """
-        headers = {
-            'Content-type': 'application/json',
-            'Accept-Encoding': 'gzip',
-            'Authorization': 'Bearer %s' % self.session_id
-        }
-        if method.lower() == 'get':
-            r = requests.request(method, 'https://'+self.instance+action, headers=headers, params=parameters, timeout=30)
-        elif method.lower() in ['post', 'patch']:
-            r = requests.request(method, 'https://'+self.instance+action, headers=headers, json=data, params=parameters, timeout=10)
-        else:
-            # other methods not implemented in this example
-            raise ValueError('Method should be get or post or patch.')
-#         print('Debug: API %s call: %s' % (method, r.url) )
-        if r.status_code < 300:
-            if method=='patch':
-                return None
-            else:
-                try:
-                    return r.json()
-                except:
-                    return {}
-        else:
-            raise Exception('API error when calling %s : %s' % (r.url, r.content))
-
-
-    def join(self, 
-                dataframe, 
-                rt_dataframe, 
-                left_on="", 
-                right_on="", 
-                new_columns=[], 
-                suffix = "_new"):
-        """
-        Joins and appends the Name and DeveloperName columns of record type to the dataframe.
-        The dataframe must contain a column named "RecordTypeId" with the 18 digit SFID of the record type.
-        """
-        df_columns = dataframe.columns.to_list()
-        if right_on not in new_columns:
-            new_columns.insert(0,right_on)
-        dataframe = pd.merge(dataframe, rt_dataframe[new_columns], how = 'inner', 
-                                left_on = left_on,right_on = right_on, suffixes=('', suffix))
-#         dataframe.drop([col for col in dataframe.columns if 'drop' in col], axis=1, inplace=True)
-        return dataframe
+from sys import platform
+import numpy as np
+import pandas as pd
+import os
+from simple_salesforce import Salesforce
+from simple_salesforce import SalesforceLogin
+from salesforce_bulk import SalesforceBulk
+from sfdclib import SfdcSession
+from sfdclib import SfdcMetadataApi
+from sfdclib import SfdcToolingApi
+import re
+import time
+import json
+from salesforce_bulk.util import IteratorBytesIO
+import pandas as pd
+import requests
+import base64
+from typing import List, Tuple, Optional, Union, Type
+from collections import OrderedDict
+import sys
+import zeep
+import ast
+sys.path.append("..")
+try:
+    from custom_exceptions.salesforce_exceptions import *
+    from utilities.df_utils import *
+    from utilities.async_utils import *
+    from utilities.sf_query_processors import *
+    from decorators import *
+except:
+    from salesforce.custom_exceptions.salesforce_exceptions import *
+    from salesforce.utilities.df_utils import *
+    from salesforce.utilities.async_utils import *
+    from salesforce.utilities.sf_query_processors import *
+    from salesforce.decorators import *
+import asyncio
+from functools import wraps, partial
+from pandas import json_normalize
+
+
+
+
+class Sf:
+    _REGEX_PARSE_SOQL_FIELDS = "(?<=select)(.*?)(?<!, )(?=from)"
+    _REGEX_PARSE_SOQL_OBJECT = "(?<!, from )(?<=from )\w*"
+    
+    def __init__(self) -> None:
+        self.filename: str = None
+        self.os_platform: str = platform
+        self.credentials: pd.DataFrame = pd.DataFrame()
+        self.sfUsername: str = None
+        self.sfPassword: str = None
+        self.sfOrgId: str = ""
+        self.isSandbox: bool = None
+        self.session_id: str = None
+        self.instance: str = None
+        self.domain: str = None
+        self.security_token: str = ''
+        self.sf: Salesforce = None
+        self.bulk: SalesforceBulk = None
+        self.sfMeta: SfdcMetadataApi = None
+        self.tooling: SfdcToolingApi = None
+        self.api_version: str = 'v52.0'
+        self.record_count: dict = {}
+        self.record_count_caseinsensitive: dict = {}
+        self.debug: bool = False
+        self.veeva_common:dict = None
+        self.org_info:dict = None
+        self.sfdc_limits: dict = None
+    
+    def authenticate(self, sfUsername: Optional[str]=None, 
+                                sfPassword: Optional[str]=None, 
+                                sfOrgId: Optional[str]=None, 
+                                isSandbox: Optional[bool]=None, 
+                                session_id: Optional[str]=None, 
+                                instance: Optional[str]=None, 
+                                security_token: Optional[str] = None,
+                                domain: Optional[str] = None,
+                                if_return: Optional[bool] = False,
+                                *args, **kwargs) -> Optional[dict]:
+        """
+        Authenticates Salesforce and retrieves the auth token.
+
+        Dependencies:
+            from simple_salesforce import Salesforce
+            from simple_salesforce import SalesforceLogin
+            from salesforce_bulk import SalesforceBulk
+            from sfdclib import SfdcSession
+            from sfdclib import SfdcMetadataApi
+            from sfdclib import SfdcToolingApi
+        """
+        
+        sfUsername = self.sfUsername if sfUsername is None else sfUsername
+        sfPassword = self.sfPassword if sfPassword is None else sfPassword
+        sfOrgId = self.sfOrgId if sfOrgId is None else sfOrgId
+        isSandbox = self.isSandbox if isSandbox is None else isSandbox
+        session_id = self.session_id if session_id is None else session_id
+        instance = self.instance if instance is None else instance
+        security_token = self.security_token if security_token is None else security_token
+        domain = self.domain if domain is None else domain
+        
+        # If session ID already exists and instance URL is already populated,
+        # reauthenticate using existing session ID
+        if session_id is not None and instance is not None:
+            sf = Salesforce(session_id = session_id, instance = instance)
+            self.sf = sf
+            self.instance = instance
+            self.session_id = session_id
+        
+        # If username, password, org ID, and isSandbox flags are all provided,
+        # authenticate using provided credentials
+        elif sfUsername is not None and sfPassword is not None and sfOrgId is not None and isSandbox is not None:
+            
+            # SFDC Sandbox authentication
+            if isSandbox:
+                self.domain = 'test'
+                sf = Salesforce(password=sfPassword, 
+                                username=sfUsername, 
+                                organizationId=sfOrgId, 
+                                security_token = self.security_token,domain='test')
+                session_id, instance = SalesforceLogin(
+                username=sfUsername,
+                password=sfPassword,
+                security_token=self.security_token,
+                domain= self.domain)
+                self.session_id = session_id
+                self.instance = instance
+                self.sf = sf
+                self.sfUsername = sfUsername
+                self.sfPassword = sfPassword
+                self.load_org_info()
+                self.sfOrgId = self.org_info['Id'][0]
+                self.isSandbox = isSandbox
+                
+            else:
+                sf = Salesforce(password=sfPassword, 
+                                username=sfUsername, 
+                                organizationId=sfOrgId, 
+                                security_token=self.security_token)
+                session_id, instance = SalesforceLogin(
+                username=sfUsername,
+                password=sfPassword,
+                security_token=self.security_token)
+                self.session_id = session_id
+                self.instance = instance
+                self.sf = sf
+                self.sfUsername = sfUsername
+                self.sfPassword = sfPassword
+                self.load_org_info()
+                self.sfOrgId = self.org_info['Id'][0]
+                self.isSandbox = isSandbox
+                
+        else:
+            raise Exception('Either sfUsername, sfPassword, sfOrgId and isSandbox must be populated, OR session_id and instance must be populated.')
+
+        # Alternative way to authenticate using SFDC Bulk API
+        # bulk = SalesforceBulk(username=sfUsername, password=sfPassword, security_token='')
+        bulk = SalesforceBulk(sessionId = self.session_id, host = self.instance)
+        self.bulk = bulk
+        # SFDC Metadata API
+        sf_meta_instance = ""
+        if self.instance.__contains__("my.salesforce.com"):
+            sf_meta_instance = self.instance.replace("my.salesforce.com","my")
+        else:
+            sf_meta_instance = ".".join(self.instance.split(".")[:2])
+            
+        sfMeta = SfdcSession(session_id=self.session_id, instance=sf_meta_instance)
+        self.sfMeta = sfMeta
+        # Alternative way to authenticate using SFDC Metadata API
+        # sfMeta = SfdcSession(username=sfUsername,password=sfPassword,token='',is_sandbox=isSandbox)
+        sfMeta._api_version = "54.0"
+        tooling = SfdcToolingApi(sfMeta)
+        self.tooling = tooling
+        
+        self.api_version = 'v' + self.sf_api_call('/services/data')[-1]['version']
+        
+        for x in self.sf_api_call('/services/data/'+self.api_version+'/limits/recordCount')['sObjects']:
+            self.record_count[x['name']] = x['count']
+            self.record_count_caseinsensitive[x['name'].lower()] = x['count']
+        
+        self.sfdc_limits = self.parse_sf_limits(self.sf_api_call('/services/data/'+self.api_version+'/limits'))
+        
+        
+        if if_return:
+            return {'sf':sf, 
+                    'bulk':bulk, 
+                    'sfMeta': sfMeta, 
+                    'tooling':tooling, 
+                    'session_id':session_id, 
+                    'instance':instance, 
+                    'sfMeta_is_connected':sfMeta.is_connected(), 
+                    'bulk_api_sessionId':bulk.sessionId}
+
+    ### ----------------------------------------------------------------------------------------------------
+    ### Synchronous Data Functions
+    ### ----------------------------------------------------------------------------------------------------
+
+    def query(self, query: str, excludedFields: Optional[List] = [], *args) -> pd.DataFrame:
+        """
+        Using SFDC SOQL Syntax, and allowing for Relationships and group bys. 
+        
+        Arguments:
+            query (str): A Standard SFDC SOQL Query allowing for relationships (Owner.Name)
+                Asterisks(*) represents all queryable fields and can be used in conjunction
+                with other relationship fields. 
+                i.e. (Select *, Owner.Profile.Name, Owner.Name From Account)
+        
+        Returns:
+            Pandas Dataframe Object.
+        
+        Raises:
+            KeyError: Typically raised when 0 records exist for the object
+                
+            badfield: A self-correcting error that is raised when a field is unqueriable, i.e. Address Fields
+            
+            Exception: When relationship query contains more than 4 layers, an Exception is raised.
+            i.e. Parent_Account_vod__r.Owner.Profile.LastModifiedBy.Name (<- a 5 layer deep relationship is not supported)
+        
+        Example of Usage:
+            sf.query("Select *, Owner.Profile.Name From Account ORDER BY CreatedDate DESC LIMIT 100")
+            
+            return:
+            A Pandas Dataframe of the last created 100 account records, with all queriable fields included in the query and a relationship field.
+            
+        """
+        objectName = re.search(self._REGEX_PARSE_SOQL_OBJECT, query.lower()).group(0)
+        successful = False
+        
+        extracted_object = pd.DataFrame()
+        # replaces "*" in query with all fields on object
+        sfSchema = getattr(self.sf, objectName).describe().get('fields')
+
+        schemaDict = {}
+        for x in sfSchema:
+            schemaDict[x['name']] = x
+
+        while not successful:
+            try:
+                results = []
+                for field in schemaDict:
+                    if (schemaDict[field]['type'] != 'location' and 
+                        schemaDict[field]['type'] != 'address' and 
+                        schemaDict[field]['name'] not in excludedFields):
+                        results.append(field)
+                final_query = query.replace("*", ", ".join(results))                
+                query_response = self.sf.query_all(final_query)
+                # if the object has 0 records in Salesforce, return empty dataframe
+                if query_response['totalSize'] == 0:
+                    fields_preparsed = re.search(self._REGEX_PARSE_SOQL_FIELDS, query,  re.IGNORECASE).group(0).split(",")
+                    return pd.DataFrame(columns=fields_preparsed)
+                else:
+                    result = pd.DataFrame(query_response)['records']
+                    for _ in result:
+                        del _['attributes']
+                    successful = True
+            except KeyError:
+                if self.debug:
+                    print(objectName + ' skipped. (Potentially due to no records found.)')
+                    
+                return pd.DataFrame(columns=results)
+            except Exception as badfield:
+                field_exclusion = badfield.state_message[badfield.state_message.find("No such column '")+\
+                    16:badfield.state_message.find("No such column '")+16+\
+                        badfield.state_message[badfield.state_message.find("No such column '")+16:].find("'")]
+                excludedFields.append(field_exclusion)
+                print("Excluded unqueriable field: " + field_exclusion)
+                if query.find("*") == -1:
+                    raise Exception(f"Unqueriable field {field_exclusion} found in query.")
+                else:
+                    continue
+            
+            result = result.apply(lambda x: pd.Series(x)).copy()
+
+            relationship_fields_preparsed = re.search(self._REGEX_PARSE_SOQL_FIELDS, query,  re.IGNORECASE).group(0).split(",")
+            # relationship_fields_prepared Example:
+            # ['*',
+            #  ' Parent_Account_vod__r.Owner.Profile.Name',
+            #  ' Child_Account_vod__r.Owner.Profile.Name',
+            #  'Parent_Account_vod__r.Owner.Profile.Id ']
+
+            relational_fields = [{x.strip(): x.strip().split(".")} for x in relationship_fields_preparsed if "." in x]
+            # relationship_fields Example:
+            # [{'Parent_Account_vod__r.Owner.Profile.Name': ['Parent_Account_vod__r',
+            #    'Owner',
+            #    'Profile',
+            #    'Name']},
+            #  {'Child_Account_vod__r.Owner.Profile.Name': ['Child_Account_vod__r',
+            #    'Owner',
+            #    'Profile',
+            #    'Name']},
+            #  {'Parent_Account_vod__r.Owner.Profile.Id': ['Parent_Account_vod__r',
+            #    'Owner',
+            #    'Profile',
+            #    'Id']}]
+
+            columns_to_remove = set()
+            for x in relational_fields:
+                if len(list(x.values())[0]) > 4:
+                    raise Exception("Too Many Relationship Levels. The Query you have entered contains more than 4 levels deep and is not supported.")
+                elif len(list(x.values())[0]) == 4:
+                    result[list(x.keys())[0]] = result[list(x.keys())[0].split(".")[0]].\
+                        apply(lambda z: z[list(x.values())[0][1]][list(x.values())[0][2]][list(x.values())[0][3]])
+                    columns_to_remove.add(list(x.values())[0][0])
+                elif len(list(x.values())[0]) == 3:
+                    result[list(x.keys())[0]] = result[list(x.keys())[0].split(".")[0]].\
+                        apply(lambda z: z[list(x.values())[0][1]][list(x.values())[0][2]])
+                    columns_to_remove.add(list(x.values())[0][0])
+                elif len(list(x.values())[0]) == 2:
+                    result[list(x.keys())[0]] = result[list(x.keys())[0].split(".")[0]].\
+                        apply(lambda z: z[list(x.values())[0][1]])
+                    columns_to_remove.add(list(x.values())[0][0])
+            result.drop(columns_to_remove, axis=1, inplace=True)
+            result.replace(np.nan, None, inplace=True)        
+
+                
+        return result
+
+    def create(self, object_api: str=None, record_dataframe: pd.DataFrame = pd.DataFrame()) -> pd.DataFrame:
+        """
+        Function creates records within the Salesforce instance using bulk api.
+
+        Arguments:
+        object_api: str: API name of the Salesforce Object for which the records are to be created.
+
+        record_dataframe: pd.DataFrame: A pandas dataframe object containing all the required fields for a record.
+
+        Returns:
+        result: pd.DataFrame: A pandas dataframe with the following columns:
+            success: boolean: indicates whether the create request was successful
+            created: boolean: this value should always be False in a create request
+            id: object[str]: this value typically is None in a create request
+            statusCode: object[str] - Optional: the error code of the create operation if failed
+            message: object[str] - Optional: the error message of the create operation if failed
+            fields: object[List[str]] - Optional: the fields for which the error code and message applies to.
+
+        Raises:
+            RequiredValuesNotProvidedDuringUpdate
+        """
+        if (object_api is None) or (len(record_dataframe) == 0):
+            raise RequiredValuesNotProvidedDuringCreate()
+        else:
+            result = getattr(self.sf.bulk, object_api).insert(record_dataframe.to_dict('records'), batch_size=10000, use_serial=False)
+            result = pd.DataFrame(result)
+            result = unpack_column(result, "errors")
+
+        return pd.DataFrame(result.rename(columns={'id': 'Id'}))
+
+    def delete(self, object_api: str=None, record_dataframe: pd.DataFrame = pd.DataFrame()) -> pd.DataFrame:
+        """
+        Function deletes records within the Salesforce instance using bulk api.
+
+        Arguments:
+        object_api: str: API name of the Salesforce Object for which the records are to be deleted from.
+
+        record_dataframe: pd.DataFrame: A pandas dataframe object containing at least 1 column with an Id column (case sensitive)
+
+        Returns:
+        result: pd.DataFrame: A pandas dataframe with the following columns:
+            success: boolean: indicates whether the delete request was successful
+            created: boolean: this value should always be False in a delete request
+            id: object[str]: this value typically is None in a delete request
+            statusCode: object[str] - Optional: the error code of the delete operation if failed
+            message: object[str] - Optional: the error message of the delete operation if failed
+            fields: object[List[str]] - Optional: the fields for which the error code and message applies to.
+
+        Raises:
+            RequiredValuesNotProvidedDuringDelete
+        """
+        if (object_api is None) or (len(record_dataframe) == 0) or record_dataframe.columns.__contains__('Id') == False:
+            raise RequiredValuesNotProvidedDuringDelete()
+        else:
+            result = getattr(self.sf.bulk, object_api).delete(record_dataframe['Id'].to_frame().to_dict('records'))
+            result = pd.DataFrame(result)
+            result = unpack_column(result, "errors")
+
+        return pd.DataFrame(result.rename(columns={'id': 'Id'}))
+    
+    def update(self, object_api: str=None, record_dataframe: pd.DataFrame = pd.DataFrame()) -> pd.DataFrame:
+        """
+        Function updates records within the Salesforce instance using bulk api.
+
+        Arguments:
+        object_api: str: API name of the Salesforce Object for which the records are to be updated.
+
+        record_dataframe: pd.DataFrame: A pandas dataframe object containing at least 1 column with an Id column (case sensitive)
+            and additional columns matching the Salesforce field api names.
+
+        Returns:
+        result: pd.DataFrame: A pandas dataframe with the following columns:
+            success: boolean: indicates whether the update request was successful
+            created: boolean: this value should always be False in a update request
+            id: object[str]: this value typically is None in a update request
+            statusCode: object[str] - Optional: the error code of the update operation if failed
+            message: object[str] - Optional: the error message of the update operation if failed
+            fields: object[List[str]] - Optional: the fields for which the error code and message applies to.
+
+        Raises:
+            RequiredValuesNotProvidedDuringUpdate
+        """
+
+        field_metadata = self.field_describe([object_api],attributes=['name','type','updateable','compoundFieldName'])
+
+        if ((object_api is None) or 
+        (len(record_dataframe) == 0)):
+            raise RequiredValuesNotProvidedDuringUpdate(message="Object API and Record Dataframe are required, ensure your record dataframe has at least 1 row and 1 column with an Id column")
+        elif record_dataframe.columns.__contains__('Id') == False:
+            raise RequiredValuesNotProvidedDuringUpdate(message="Record Dataframe must have an Id column")
+        elif ~record_dataframe.columns.isin(field_metadata[object_api]).all():
+            # checks whether any of the columns in the dataframe passed in are not valid field API names
+            raise RequiredValuesNotProvidedDuringUpdate(message="One of the columns in the record dataframe is not a valid field for the object")
+        elif record_dataframe.columns.isin(field_metadata[(field_metadata['Updateable'] == False) & (field_metadata[object_api] != "Id")][object_api]).any():
+            # checks whether any of the columns in the dataframe passed in are not updateable
+            non_updatable_fields = list(set(record_dataframe.columns) - set(field_metadata[(field_metadata['Updateable'] == True) | (field_metadata[object_api] == "Id")][object_api]))
+            raise RequiredValuesNotProvidedDuringUpdate(message=f"The following fields are not updatable: {', '.join(non_updatable_fields)}")
+        elif record_dataframe.columns.isin(field_metadata[(~field_metadata['Compoundfieldname'].isnull()) & (field_metadata['Compoundfieldname'] != 'Name')][object_api]).any():
+            # checks whether any of the columns in the dataframe passed in are compound fields
+            compound_fields = list(set(record_dataframe.columns) & set(field_metadata[(~field_metadata['Compoundfieldname'].isnull()) & (field_metadata['Compoundfieldname'] != 'Name')][object_api]))
+            raise RequiredValuesNotProvidedDuringUpdate(message=f"The following fields are compound fields, which are not updatable: {', '.join(compound_fields)}")
+        # checks whether an reference (lookup/master-detail) field is included in the source dataframe
+        #  or ~record_dataframe.columns.isin(field_metadata[field_metadata['Type'] == 'reference'][object_api]).any()
+            
+        else:
+            record_dataframe.replace(np.nan, None, inplace=True)
+            result = getattr(self.sf.bulk, object_api).update(record_dataframe.to_dict('records'), batch_size=10000, use_serial=False)
+            result = pd.DataFrame(result)
+            result = unpack_column(result, "errors")
+
+        return pd.DataFrame(result.rename(columns={'id': 'Id'}))
+
+    def upsert(self, object_api: str=None, external_id_field_api: str="", record_dataframe: pd.DataFrame = pd.DataFrame()) -> pd.DataFrame:
+        """
+        Function upserts records within the Salesforce instance using bulk api.
+
+        Arguments:
+        object_api: str: API name of the Salesforce Object for which the records are to be upserted into.
+
+        external_id_field_api: str: API name of the external ID field used for the upsert operation.
+
+        record_dataframe: pd.DataFrame: A pandas dataframe object containing the External column (case sensitive)
+            and additional columns matching the Salesforce field api names.
+
+        Returns:
+        result: pd.DataFrame: A pandas dataframe with the following columns:
+            success: boolean: indicates whether the upsert request was successful
+            created: boolean: this value should always be False in a upsert request
+            id: object[str]: this value typically is None in a upsert request
+            statusCode: object[str] - Optional: the error code of the upsert operation if failed
+            message: object[str] - Optional: the error message of the upsert operation if failed
+            fields: object[List[str]] - Optional: the fields for which the error code and message applies to.
+
+        Raises:
+            RequiredValuesNotProvidedDuringUpsert
+            SalesforceMalformedRequest
+        """
+
+        field_metadata = self.field_describe([object_api], ['name', 'type', 'length','externalId','updateable','compoundFieldName'])
+            
+            
+        if ((object_api is None) or 
+        (len(record_dataframe) == 0)):
+            raise RequiredValuesNotProvidedDuringUpdate(message="Object API and Record Dataframe are required, ensure your record dataframe has at least 1 row and 1 column with an Id column")
+        elif ~record_dataframe.columns.isin(field_metadata[object_api]).all():
+            # checks whether any of the columns in the dataframe passed in are not valid field API names
+            raise RequiredValuesNotProvidedDuringUpdate(message="One of the columns in the record dataframe is not a valid field for the object")
+        elif external_id_field_api == "":
+            raise RequiredValuesNotProvidedDuringUpsert(message="External ID field API is required")
+        elif record_dataframe.columns.isin(field_metadata[(field_metadata['Updateable'] == False) & (field_metadata[object_api] != "Id")][object_api]).any():
+            # checks whether any of the columns in the dataframe passed in are not updateable
+            non_updatable_fields = list(set(record_dataframe.columns) - set(field_metadata[(field_metadata['Updateable'] == True) | (field_metadata[object_api] == "Id")][object_api]))
+            raise RequiredValuesNotProvidedDuringUpdate(message=f"The following fields are not updatable: {', '.join(non_updatable_fields)}")
+        elif record_dataframe.columns.isin(field_metadata[(~field_metadata['Compoundfieldname'].isnull()) & (field_metadata['Compoundfieldname'] != 'Name')][object_api]).any():
+            # checks whether any of the columns in the dataframe passed in are compound fields
+            compound_fields = list(set(record_dataframe.columns) & set(field_metadata[(~field_metadata['Compoundfieldname'].isnull()) & (field_metadata['Compoundfieldname'] != 'Name')][object_api]))
+            raise RequiredValuesNotProvidedDuringUpdate(message=f"The following fields are compound fields, which are not updatable: {', '.join(compound_fields)}")
+        else:
+            record_dataframe.replace(np.nan, None, inplace=True)
+            result = getattr(self.sf.bulk, object_api).upsert(record_dataframe.to_dict('records'), external_id_field_api, batch_size=10000, use_serial=False)
+            result = pd.DataFrame(result)
+            result = unpack_column(result, "errors")
+
+        return pd.DataFrame(result)
+
+    def extract_bulk(self, og_query: str, 
+                        excludedFields: Optional[List] = []) -> pd.DataFrame:
+        """
+        Uses a standard SOQL query to extract Salesforce Data and outputs a pandas dataframe
+        
+        Dependencies:
+            import re
+            import time
+            import json
+            from salesforce_bulk.util import IteratorBytesIO
+            import pandas as pd
+        
+        """
+        objectName = re.search(self._REGEX_PARSE_SOQL_OBJECT, og_query.lower()).group(0)
+        successful = False
+        
+        extracted_object = pd.DataFrame()
+        # replaces "*" in query with all fields on object
+        sfSchema = getattr(self.sf, objectName).describe().get('fields')
+
+        schemaDict = {}
+        for x in sfSchema:
+            schemaDict[x['name']] = x
+
+        while not successful:
+            try:
+                results = []
+                for field in schemaDict:
+                    if (schemaDict[field]['type'] != 'location' and 
+                        schemaDict[field]['type'] != 'address' and 
+                        schemaDict[field]['name'] not in excludedFields):
+                        results.append(field)
+                query = og_query.replace("*", ", ".join(results))
+                
+#                 # if the object has 0 records in Salesforce, return empty dataframe
+#                 if objectName not in self.record_count_caseinsensitive.keys():
+#                     return pd.DataFrame(columns=results)
+                    
+                job = self.bulk.create_query_job(objectName, contentType='JSON')
+                batch = self.bulk.query(job, query)
+                while not self.bulk.is_batch_done(batch):
+                    time.sleep(1)
+                sfdf = pd.DataFrame()
+                for result in self.bulk.get_all_results_for_query_batch(batch):
+                    result = json.load(IteratorBytesIO(result))
+                    sfdf = pd.concat([sfdf, pd.DataFrame(result)])
+
+                # drops attributes column in dataframe
+                sfdf.drop(columns="attributes", inplace = True)
+
+                # formats all datetime to the proper formatting
+                for column in sfdf:
+                    if schemaDict[column]['type'] == 'datetime':
+                        sfdf[column] = pd.to_datetime(sfdf[column], unit='ms')
+                    # if the column has a 'scale' or salesforce's decimal places, then turn the column into an int
+                    elif schemaDict[column]['type'] == 'double' and schemaDict[column]['scale'] == 0:
+                        sfdf[column] = pd.to_numeric(sfdf[column], downcast='integer')
+
+            #                         pd.to_datetime(sfdf[column], unit = 's')
+            #                         sfdf[column].apply(lambda x : datetime.fromtimestamp(int(x), tz).isoformat())
+            #                 sfdf.convert_dtypes()
+                # converts the output of the bulk query to text so that the unix timestamp displays property, and fills and empty values with the '' string.
+                sfdf = sfdf.fillna('').astype(str)
+                successful = True
+            except KeyError:
+                if self.debug:
+                    print(objectName + ' skipped. (Potentially due to no records found.)')
+                    
+                return pd.DataFrame(columns=results)
+            except Exception as badfield:
+                field_exclusion = badfield.state_message[badfield.state_message.find("No such column '")+\
+                    16:badfield.state_message.find("No such column '")+16+\
+                        badfield.state_message[badfield.state_message.find("No such column '")+16:].find("'")]
+                excludedFields.append(field_exclusion)
+                print("Excluded unqueriable field: " + field_exclusion)
+                if og_query.find("*") == -1:
+                    raise Exception(f"Unqueriable field {field_exclusion} found in query.")
+                else:
+                    continue
+        if self.debug:
+            print("Extracted " + objectName + " successfully!")
+        return sfdf
+    
+    def entity_access_query(self, entity_type):
+        # Retrieves information about which Profile or PermissionSet
+        # grants permission to which Setup Entity (i.e. ApexPage, ApexClass, TabSets, etc)
+        
+        entity_access = transform_sf_result_set_rec(self.sf.query_all(f"""
+        SELECT Id, Parent.Id, Parent.ProfileId, Parent.Profile.Name, Parent.Name,SetupEntityId,SetupEntityType FROM
+        SetupEntityAccess WHERE SetupEntityType = '{entity_type}'""")['records'])
+        # entity_access.drop(columns=['PermissionSet.Profile'], inplace=True)
+        return {entity_type: entity_access}
+
+    ### ----------------------------------------------------------------------------------------------------
+    ### Asynchronous Data Functions
+    ### ----------------------------------------------------------------------------------------------------
+
+    async def async_query(self, query, excludedFields: Optional[List] = []) -> pd.DataFrame:
+        async_query = async_wrap(self.query)
+        return await async_query(query, excludedFields)
+    
+    async def async_queries(self, queries: List[str]):
+        async_queries = async_wrap(self.sf.query_all)
+        result_list = await asyncio.gather(*[async_queries(query) for query in queries])
+        result_pd_list = [transform_sf_result_set_rec(result['records']) for result in result_list]
+        return result_pd_list
+
+
+    async def async_upsert(self, object_api, record_dataframe, external_id_field_api, batchsize=2000, *args, **kwargs):
+        async_upsert = async_wrap(self.upsert)
+        batches = len(record_dataframe) / batchsize
+        result_list = await asyncio.gather(*[async_upsert(object_api= object_api, record_dataframe=batch, external_id_field_api=external_id_field_api) for batch in np.array_split(record_dataframe, batches)])
+        return pd.concat(result_list).reset_index(drop=True)
+
+    async def async_update(self, object_api, record_dataframe, batchsize=2000, *args, **kwargs):
+        async_update = async_wrap(self.update)
+        batches = len(record_dataframe) / batchsize
+        result_list = await asyncio.gather(*[async_update(object_api= object_api, record_dataframe=batch) for batch in np.array_split(record_dataframe, batches)])
+        return pd.concat(result_list).reset_index(drop=True)
+
+    async def async_create(self, object_api, record_dataframe, batchsize=2000, *args, **kwargs):
+        async_create = async_wrap(self.create)
+        batches = len(record_dataframe) / batchsize
+        result_list = await asyncio.gather(*[async_create(object_api= object_api, record_dataframe=batch) for batch in np.array_split(record_dataframe, batches)])
+        return pd.concat(result_list).reset_index(drop=True)
+
+    async def async_delete(self, object_api, record_dataframe, batchsize=2000, *args, **kwargs):
+        async_delete = async_wrap(self.delete)
+        batches = len(record_dataframe) / batchsize
+        result_list = await asyncio.gather(*[async_delete(object_api= object_api, record_dataframe=batch) for batch in np.array_split(record_dataframe, batches)])
+        return pd.concat(result_list).reset_index(drop=True)
+    
+    async def async_get_user_password_status(self, user_ids: list[str]) -> dict:
+        async_sf_api_call = async_wrap(self.sf_api_call)
+        response = await asyncio.gather(*[async_sf_api_call(f'/services/data/{self.api_version}/sobjects/User/{user_id}/password', method='GET') for user_id in user_ids])
+        # Return a dict
+        response = {user_id: result for user_id, result in zip(user_ids, response)}
+        return response
+    
+    
+    
+    ### ----------------------------------------------------------------------------------------------------
+    ### Asynchronous Metadata Functions
+    ### ----------------------------------------------------------------------------------------------------
+    async def async_get_non_updatable_fields(self, object_name: str):
+        """
+        Returns a list of fields that cannot be updated.
+        """
+        async_field_describe =  async_wrap(self.field_describe)
+        field_metadata = await async_field_describe([object_name], attributes=['name','updateable'])
+        non_updatable_fields = list(field_metadata[field_metadata['Updateable'] == False][object_name])[1:]
+        return non_updatable_fields
+
+    async def async_get_compound_field_names(self, object_name: str, include_name_compound_fields: bool=False):
+        """
+        Returns a list of compound fields. By default "Name" compound field names are excluded.
+        To return a list of compound fields including "Name" fields, set include_name_compound_fields to True.
+
+        Compound field names are fields that are composed of multiple fields. These fields are not updatable directly via the API
+        and may cause errors if updated directly.
+        """
+        async_field_describe =  async_wrap(self.field_describe)
+        field_metadata = await async_field_describe([object_name], attributes=['name','compoundFieldName'])
+
+        if include_name_compound_fields:
+            compound_field_names = list(field_metadata[(~field_metadata['Compoundfieldname'].isnull())][object_name])
+        elif include_name_compound_fields==False:
+            compound_field_names = list(field_metadata[(~field_metadata['Compoundfieldname'].isnull()) & (field_metadata['Compoundfieldname'] != 'Name')][object_name])
+        else:
+            raise ValueError('include_name_compound_fields must be a boolean.')
+        return compound_field_names
+    
+    async def get_picklist_values_by_object_record_type(self, object: str):
+        object_record_type_ids = self.query(f"Select Id, Name From RecordType Where SobjectType = '{object}'").apply(lambda row: {"Id": row['Id'], "Name": row['Name']}, axis=1)
+        if len(object_record_type_ids) == 0:
+            object_record_type_ids = pd.Series([{"Id": "012000000000000AAA", "Name": "Master"}]).to_list()
+        else:
+            object_record_type_ids = object_record_type_ids.to_list()
+            
+        object_describe = self.sf_api_call(f"/services/data/{self.api_version}/ui-api/object-info/{object}")['fields']
+        controlling_fields = []
+        for field, values in object_describe.items():
+            controlling_fields.append({"Field": field, "Controlling Field": "" if values['controllingFields'] == [] else "; ".join(values['controllingFields'])})
+        controlling_fields = pd.DataFrame(controlling_fields)
+
+        def record_type_picklist_retriever(self, object, record_type_id, record_type_name):
+            result = []
+            picklist_metadata = self.sf_api_call(f"/services/data/{self.api_version}/ui-api/object-info/{object}/picklist-values/{record_type_id}")['picklistFieldValues']
+            if len(picklist_metadata) == 0:
+                return pd.DataFrame(columns=['attributes',
+                                    'label',
+                                    'validFor',
+                                    'value',
+                                    'Field_API',
+                                    'defaultValueLabel',
+                                    'defaultValueValue',
+                                    'Controlling Field',
+                                    'RecordTypeName',
+                                    'Object'])
+                
+            for key, value in picklist_metadata.items():
+                result.append({"Field_API": key, "controllerValues": value['controllerValues'], "defaultValue":  value['defaultValue'], "values": value['values']})
+            final_result_pd = json_normalize(result, ['values'], ['defaultValue', 'controllerValues', 'Field_API'])
+            ## Converts the validFor numerical codes i.e. [0,2] to it's corresponding text values by looking it up on the controllerValues column i.e. {'Web': 0, 'Phone Inquiry': 1, 'Partner Reference': 2 ... }
+            ## [0,2] -> ['Web', 'Partner Reference']
+            final_result_pd['validFor'] = final_result_pd.apply(lambda row: "\n".join([{v: k for k, v in row['controllerValues'].items()}[value] for value in row['validFor']]), axis=1)
+            final_result_pd.drop(columns=['controllerValues'], inplace=True)
+            
+            try:
+                final_result_pd[['defaultValueLabel', 'defaultValueValue']] = json_normalize(final_result_pd['defaultValue'])[['label','value']]
+            except:
+                final_result_pd[['defaultValueLabel', 'defaultValueValue']] = [np.nan, np.nan]
+            
+            final_result_pd.drop(columns=['defaultValue'], inplace=True)
+            final_result_pd = pd.merge(final_result_pd, controlling_fields, left_on='Field_API', right_on='Field', how='left').drop(columns=['Field']).copy()
+            final_result_pd['RecordTypeName'] = record_type_name
+            final_result_pd['Object'] = object
+            return final_result_pd
+
+        async_picklist_rt_retrieve = async_wrap(record_type_picklist_retriever)
+        results = pd.concat(await asyncio.gather(*[async_picklist_rt_retrieve(self, object, record_type_id['Id'], record_type_id['Name']) for record_type_id in object_record_type_ids]))
+        results = results[['Object', 'RecordTypeName', 'Field_API', 'Controlling Field', 'defaultValueLabel', 'defaultValueValue', 'label', 'value', 'validFor']]
+        return results
+
+
+    async def object_permission_bulk_check(self, objects: list, permissions: list ):
+        async_object_permission_check = async_wrap(self.object_permission_check)
+        result_list = await asyncio.gather(*[async_object_permission_check(object, permission ) for object in objects for permission in permissions])
+        # for result in result_list:
+        #     data = deep_merge_dictionaries(data, result)
+        result_list = [item for sublist in result_list for item in sublist]
+        return result_list
+
+    async def field_permission_bulk_check(self, objects: list, ) -> dict[str, pd.DataFrame]:
+        async_field_permission_check = async_wrap(self.field_permission_check)
+        result_list = await asyncio.gather(*[async_field_permission_check( object ) for object in objects])
+        # for result in result_list:
+        #     data = deep_merge_dictionaries(data, result)
+        profile_list = [item['profilePermissions'] for item in result_list]
+        permissionSet_list = [item['permissionSetPermissions'] for item in result_list]
+        result_dict = {'profilePermissions': pd.concat(profile_list), 'permissionSetPermissions': pd.concat(permissionSet_list)}
+        
+        return result_dict
+    
+    async def async_set_user_passwords(self, user_id_password_list_dict: dict) -> dict:
+        async_set_user_password = async_wrap(self.set_user_password)
+        results = await asyncio.gather(*[async_set_user_password(user_id, password) for user_id, password in user_id_password_list_dict.items()])
+        results = {result['user_id']: result['message'] for result in results}
+        return results
+
+    async def entity_access_bulk_query(self, entity_types: list):
+        async_entity_access_query = async_wrap(self.entity_access_query)
+        results = await asyncio.gather(*[async_entity_access_query(entity_type) for entity_type in entity_types])
+        merged_dict = {}
+        for result in results:
+            for key, value in result.items():
+                merged_dict[key] = value
+        return merged_dict
+
+    async def apex_pages_profiles_and_permission_set_access_query(self, apex_pages_to_check: list[str]):
+        query_results = await self.entity_access_bulk_query(['ApexPage'])
+
+        entity_access_apex_pages_async =  query_results['ApexPage']
+
+        entity_permission_set_access_apex_pages_async = entity_access_apex_pages_async[entity_access_apex_pages_async['Profile.Name'].isna()]
+        entity_profile_access_apex_pages_async = entity_access_apex_pages_async[entity_access_apex_pages_async['Profile.Name'].notna()]
+
+        # filter = ['Scheduler_Administration_vod','Network_Admin_Page_vod','searchAccts_vod']
+        filter_join = "','".join(apex_pages_to_check)
+        where_clause = f" WHERE Name IN ('{filter_join}')"
+        apex_pages_query = transform_sf_result_set_rec(self.sf.query_all(f"""
+            SELECT Id, Name From ApexPage{where_clause}""")['records'])
+
+        permission_sets_with_apex_page_access = entity_permission_set_access_apex_pages_async[entity_permission_set_access_apex_pages_async['SetupEntityAccess.SetupEntityId'].isin(apex_pages_query['ApexPage.Id'].unique())]
+        profiles_with_apex_page_access = entity_profile_access_apex_pages_async[entity_profile_access_apex_pages_async['SetupEntityAccess.SetupEntityId'].isin(apex_pages_query['ApexPage.Id'].unique())]
+        permission_sets_with_apex_page_access = pd.merge(permission_sets_with_apex_page_access, apex_pages_query, left_on='SetupEntityAccess.SetupEntityId', right_on='ApexPage.Id', how='inner').drop(columns=['ApexPage.Id'], axis=1)
+        profiles_with_apex_page_access = pd.merge(profiles_with_apex_page_access, apex_pages_query, left_on='SetupEntityAccess.SetupEntityId', right_on='ApexPage.Id', how='inner').drop(columns=['ApexPage.Id'], axis=1)
+
+        profiles_with_apex_page_access = profiles_with_apex_page_access[['PermissionSet.ProfileId','Profile.Name','SetupEntityAccess.SetupEntityType','ApexPage.Name']]
+        profiles_with_apex_page_access.columns = ['Profile Id', 'Profile Name', 'Setup Entity Type', 'Visualforce (Apex) Name']
+        
+        permission_sets_with_apex_page_access = permission_sets_with_apex_page_access[['PermissionSet.Id','PermissionSet.Name','SetupEntityAccess.SetupEntityType','ApexPage.Name']]
+        permission_sets_with_apex_page_access.columns = ['PermissionSet Id', 'PermissionSet Name', 'Setup Entity Type', 'Visualforce (ApexPage) Name']
+        
+        return {'profiles_with_apex_page_access': profiles_with_apex_page_access, 'permission_sets_with_apex_page_access': permission_sets_with_apex_page_access}
+
+    # Retrieves the Page Layout by Profile by Record Type data for listed objects in the org
+    async def retrieve_profile_layout_record_type_matrix_by_objects(self, objects_to_retrieve_profile_layout_matrix = ['Account','Address_vod__c','Child_Account_vod__c'], discard_unqueriable_objects = False, return_pivot_table = False):
+        
+        objects_to_retrieve = [object[:-3] if object.endswith('__c') else object for object in objects_to_retrieve_profile_layout_matrix]
+        
+        # Objects in the Profile Layout table's TableEnumOrId column where the value is an object name instead of an object ID
+        
+        ENUM_OBJECTS = {'Account', 'AccountTeamMember', 'Asset', 'AuthorizationForm', 'AuthorizationFormConsent', 'BusinessBrand', 'Campaign', 'CampaignMember', 'Case',
+                            'CaseClose', 'CaseInteraction', 'CommunityMemberLayout', 'Contact', 'ContactPointAddress', 'ContactPointEmail', 'ContactPointPhone', 'ContentVersion', 'Contract', 'Customer', 'DelegatedAccount',
+                            'DuplicateRecordItem', 'DuplicateRecordSet', 'EmailMessage', 'Event', 'FeedItem', 'Global', 'Idea', 'Individual', 'Lead', 'Macro', 'ObjectTerritory2AssignmentRule',
+                            'Opportunity', 'OpportunityLineItem', 'Order', 'OrderItem', 'PersonAccount', 'Pricebook2', 'PricebookEntry', 'ProcessException', 'Product2',
+                            'ProfileSkill', 'ProfileSkillEndorsement', 'ProfileSkillUser', 'QuickText', 'Scorecard', 'ScorecardAssociation', 'ScorecardMetric', 'Seller', 'ServiceAppointmentGroup',
+                            'ServiceTerritoryRelationship', 'SignupRequest', 'SocialPersona', 'SocialPost', 'Solution', 'Task', 'Territory2', 'Territory2Model', 'Territory2Type', 'User',
+                            'UserAlt', 'UserProvAccount', 'UserProvisioningLog', 'UserProvisioningRequest', 'UserTerritory2Association', 'WorkProcedure', 'WorkProcedureStep', 'WorkTypeExtension'}
+        
+        # Objects that returns empty results if queried via the WHERE clause using Salesforce Tooling API.
+        # i.e. "Select LayoutId from ProfileLayout where TableEnumOrId = 'DelegatedAccount'" returns empty results.
+        UNQUERIABLE_ENUM_OBJECTS = {'DelegatedAccount','ProfileSkill','ProfileSkillEndorsement','ProfileSkillUser','ServiceTerritoryRelationship','WorkTypeExtension'}
+        
+        
+        
+        object_dataframe = pd.DataFrame(self.tooling_query_all("Select DeveloperName from CustomObject"))
+        object_dataframe['ObjectID'] = object_dataframe.apply(lambda row: row['attributes']['url'].split('/')[-1] if row['attributes']['url'] else "", axis=1)
+        
+        profile_layout_queries = []
+        
+        for object_name in objects_to_retrieve:
+            if object_name in UNQUERIABLE_ENUM_OBJECTS and discard_unqueriable_objects == False:
+                raise Exception("Unqueriable object: " + object_name + ". Please use retrieve_profile_layout_record_type_matrix_all() instead or set discard_unqueriable_objects parameter to True")
+            elif object_name in ENUM_OBJECTS:
+                profile_layout_queries.append("Select LayoutId, ProfileId, Profile.Name, RecordTypeId, RecordType.Name, Layout.Name, TableEnumOrId from ProfileLayout where TableEnumOrId = '" + object_name + "'")
+            else:
+                object_id = object_dataframe[object_dataframe['DeveloperName'] == object_name]['ObjectID'].values[0]
+                profile_layout_queries.append(f"Select LayoutId, ProfileId, Profile.Name, RecordTypeId, RecordType.Name, Layout.Name, TableEnumOrId from ProfileLayout where TableEnumOrId = '{object_id}'")
+        
+        
+        async_tooling_query_all = async_wrap(self.tooling_query_all)
+        
+        
+        await_results = await asyncio.gather(*[async_tooling_query_all(query) for query in profile_layout_queries])
+        
+        await_result_dataframe = [transform_sf_result_set_rec(result) for result in await_results if len(result) > 0]
+        
+        account_page_layouts_bulk = pd.concat(await_result_dataframe)
+
+        account_page_layouts_bulk['ProfileName'] = account_page_layouts_bulk.apply(lambda row: row['ProfileLayout.Profile']['Name'] if row['ProfileLayout.Profile'] else "", axis=1)
+        account_page_layouts_bulk['RecordTypeName'] = account_page_layouts_bulk.apply(lambda row: row['ProfileLayout.RecordType']['Name'] if row['ProfileLayout.RecordType'] else "", axis=1)
+        account_page_layouts_bulk['PageLayout'] = account_page_layouts_bulk.apply(lambda row: row['ProfileLayout.Layout']['Name'] if row['ProfileLayout.Layout'] else "", axis=1)
+        account_page_layouts_bulk.drop(['ProfileLayout.Profile','ProfileLayout.RecordType','ProfileLayout.Layout'], axis=1, inplace=True)
+
+        object_dataframe['ObjectID'] = object_dataframe.apply(lambda row: row['attributes']['url'].split('/')[-1] if row['attributes']['url'] else "", axis=1)
+
+        account_page_layouts_bulk = account_page_layouts_bulk.merge(object_dataframe, left_on='ProfileLayout.TableEnumOrId', right_on='ObjectID', how='left').copy()
+        account_page_layouts_bulk['DeveloperName'] = account_page_layouts_bulk.apply(lambda row: row['DeveloperName'] if pd.notnull(row['DeveloperName']) else row['ProfileLayout.TableEnumOrId'], axis=1)
+        account_page_layouts_bulk.drop(['attributes'], axis=1, inplace=True)
+        
+        # Fill in the RecordTypeName colum with the Master Record Type Name
+        account_page_layouts_bulk['RecordTypeName'] = account_page_layouts_bulk['RecordTypeName'].apply(lambda row: row if row else 'Master')
+        # Filter out Deprecated Profiles
+        account_page_layouts_bulk = account_page_layouts_bulk[(~account_page_layouts_bulk['ProfileName'].isnull()) & (account_page_layouts_bulk['ProfileName'] != '') & (account_page_layouts_bulk['PageLayout'] != 'Veeva Vpro Unit Testing Layout')].copy()
+        
+        if self.instance.__contains__("my.salesforce.com"):
+            sf_meta_instance = self.instance.replace(".my.salesforce.com","")
+        else:
+            sf_meta_instance = ".".join(self.instance.split(".")[:1])
+        
+        account_page_layouts_bulk['Edit Link'] = account_page_layouts_bulk.apply(lambda row: "https://" + sf_meta_instance + ".lightning.force.com/lightning/setup/ObjectManager/" + (row['DeveloperName'] if str(row['ObjectID']) == 'nan' else row['ObjectID']) + "/PageLayouts/" + row['ProfileLayout.LayoutId'] + "/view", axis=1)
+        
+        if return_pivot_table:
+            return account_page_layouts_bulk.pivot(index='ProfileName', columns=['DeveloperName','RecordTypeName'], values='PageLayout')
+        else:
+            return account_page_layouts_bulk
+
+    async def field_permission_user_check(self, objects: list[str], permissions: list[str], users=None) -> pd.DataFrame:
+        # Similar to the field_permission_check function, but this one will return a list of users that have the specified permission on the specified object
+        
+        # this is to avoid having a mutable default argument
+        users = [] if users is None else users
+        
+        object_query = "','".join(objects)
+        permission_query = ' OR '.join([f"({permission} = true)" for permission in permissions])
+
+        relevant_ps_and_profiles = transform_sf_result_set_rec(self.sf.query_all(f"""
+                                                SELECT ParentId,
+                                                        Field,
+                                                        PermissionsEdit,
+                                                        PermissionsRead
+                                                FROM FieldPermissions
+                                                WHERE SObjectType IN ('{object_query}') AND
+                                                ({permission_query})
+                                                """)['records'])
+
+        relevant_ps_and_profiles['Object API Name'] = relevant_ps_and_profiles['FieldPermissions.Field'].apply(lambda row: row.split('.')[0])
+        relevant_ps_and_profiles['Field API Name'] = relevant_ps_and_profiles['FieldPermissions.Field'].apply(lambda row: row.split('.')[1])
+        relevant_ps_and_profiles.drop(columns=['FieldPermissions.Field'], inplace=True)
+
+        user_query = (" AND Assignee.UserName IN ('" + "','".join(users) + "')") if len(users) > 0 else ""
+
+        relevant_ps_and_profiles_list = "','".join(relevant_ps_and_profiles['FieldPermissions.ParentId'].unique().tolist())
+
+        data = transform_sf_result_set_rec(self.sf.query_all(f"""SELECT Assignee.Id, Assignee.Name,Assignee.IsActive, 
+                                                                Assignee.UserName, PermissionSet.Id, 
+                                                                PermissionSet.isOwnedByProfile, PermissionSet.Profile.Name, PermissionSet.Label
+                                                                FROM PermissionSetAssignment
+                                                                WHERE PermissionSetId
+                                                                IN ('{relevant_ps_and_profiles_list}')
+                                                                {user_query} AND Assignee.IsActive = TRUE""")['records'])
+        
+        if len(data) == 0:
+            return pd.DataFrame(columns=['UserName', 'Profile', 'Field API Name', 'Object API Name','Permission', 'Permission Set'])
+        
+        # Retrieve Profile FLS data
+        profiles = data[data['PermissionSet.IsOwnedByProfile']]['Profile.Name'].unique().tolist()
+        profiles = ['Admin' if x == 'System Administrator' else x for x in profiles]
+
+
+        async_metadata_read = async_wrap(self.metadata_read)
+        profile_metadata_tasks = {}
+        profile_metadata_dict = {}
+
+        for profile in profiles:
+                profile_metadata_tasks[profile] = asyncio.create_task(async_metadata_read('Profile', profile))
+
+
+        task_result_list = await asyncio.gather(*profile_metadata_tasks.values())
+
+
+        for profile in profiles:
+                profile_metadata_dict["System Administrator" if profile == 'Admin' else profile] = pd.DataFrame(task_result_list[profiles.index(profile)]['fieldPermissions'][0])
+    
+        data = data.merge(relevant_ps_and_profiles, left_on='PermissionSet.Id', right_on='FieldPermissions.ParentId', how='left').copy()
+        if (len(data) > 0):
+                
+                profile_violations = data[data['PermissionSet.IsOwnedByProfile']== True][['User.Username', 'Profile.Name']].drop_duplicates().copy()
+                # profile_violations = data[data['PermissionSet.IsOwnedByProfile']== True][['User.Username', 'Profile.Name','Field API Name']]
+                profile_metadata_pd = pd.concat(profile_metadata_dict.values(), keys=profile_metadata_dict.keys(), names=['Profile', 'Index']).reset_index(level=1, drop=True).reset_index()
+                profile_metadata_pd.rename(columns={'Profile': 'Profile.Name'}, inplace=True)
+                profile_metadata_pd['Field API Name'] = profile_metadata_pd['field'].str.split('.').str[1]
+                profile_metadata_pd['Object API Name'] = profile_metadata_pd['field'].str.split('.').str[0]
+                profile_metadata_pd = profile_metadata_pd[profile_metadata_pd['Object API Name'].isin(objects)].copy()
+                profile_metadata_pd.drop(columns=['field'], inplace=True)
+
+                # if permission == 'PermissionsEdit':
+                #         profile_metadata_pd = profile_metadata_pd[profile_metadata_pd['editable'] == True].copy()
+                #         profile_metadata_pd.drop(columns=['editable', 'readable'], inplace=True)
+                # elif permission == 'PermissionsRead':
+                #         profile_metadata_pd = profile_metadata_pd[profile_metadata_pd['readable'] == True].copy()
+                #         profile_metadata_pd.drop(columns=['editable', 'readable'], inplace=True)
+                
+                profile_violations = profile_violations.merge(profile_metadata_pd, on='Profile.Name', how='left').copy()
+                profile_editable = profile_violations[profile_violations['editable'] == True].drop(columns=['editable','readable']).copy()
+                profile_editable['Permission'] = 'PermissionsEdit'
+                profile_readable = profile_violations[profile_violations['readable'] == True].drop(columns=['editable','readable']).copy()
+                profile_readable['Permission'] = 'PermissionsRead'
+
+                profile_fls_final = pd.concat([profile_editable, profile_readable])
+                profile_fls_final.columns = ['UserName','Profile','Field API Name','Object API Name','Permission']
+                
+                permission_set_violations = data[data['PermissionSet.IsOwnedByProfile']== False][['User.Username', 'PermissionSet.Label', 'Object API Name', 'FieldPermissions.PermissionsEdit','FieldPermissions.PermissionsRead','Field API Name']]
+                
+                ps_editable = permission_set_violations[permission_set_violations['FieldPermissions.PermissionsEdit'] == True].drop(columns=['FieldPermissions.PermissionsEdit','FieldPermissions.PermissionsRead']).copy()
+                ps_editable['Permission'] = 'PermissionsEdit'
+                ps_readable = permission_set_violations[permission_set_violations['FieldPermissions.PermissionsRead'] == True].drop(columns=['FieldPermissions.PermissionsEdit','FieldPermissions.PermissionsRead']).copy()
+                ps_readable['Permission'] = 'PermissionsRead'
+                
+                ps_fls_final = pd.concat([ps_editable, ps_readable])
+                ps_fls_final.columns = ['UserName','Permission Set','Object API Name','Field API Name', 'Permission']
+                
+                return pd.merge(profile_fls_final, ps_fls_final, on=['UserName','Object API Name', 'Field API Name','Permission'], how='outer')
+        else:
+                return pd.DataFrame(columns=['UserName', 'Profile', 'Field API Name', 'Object API Name','Permission', 'Permission Set'])
+          
+            
+    async def retrieve_user_profile_record_type_details(self, username: str, objects: list[str]):
+        
+        profile_metadata = pd.DataFrame(zeep.helpers.serialize_object(self.metadata_list("Profile")))
+        profile_metadata = profile_metadata[['id', 'fullName']].copy()
+        profile_metadata
+        user_profile_id = transform_sf_result_set_rec(self.sf.query_all(f"Select Id, ProfileId FROM User WHERE Username = '{username}'")['records'])
+        if len(profile_metadata[profile_metadata['id'] == user_profile_id['User.ProfileId'].values[0]]['fullName']) == 0:
+            raise Exception("User does not have a retrievable / valid profile")
+        else:
+            user_profile = profile_metadata[profile_metadata['id'] == user_profile_id['User.ProfileId'].values[0]]['fullName'].values[0]
+
+        async_profile_read = async_wrap(self.metadata_read)
+        
+        user_profile_metadata = async_profile_read('Profile', user_profile)
+        
+        results = {}
+        
+        async_object_describe = async_wrap(self.object_describe)
+        
+        tasks = {}
+        
+        for object in objects:
+            tasks[object] = async_object_describe(object)
+        tasks['get_profile_data'] = user_profile_metadata
+        
+        task_result_list = await asyncio.gather(*tasks.values())
+        
+        task_result_dict = {}
+        
+        for object in objects:
+            task_result_dict[object] = task_result_list[objects.index(object)]
+            
+        task_result_dict['get_profile_data'] = task_result_list[-1]
+        
+        user_rt_visibilities = pd.DataFrame(task_result_dict['get_profile_data']['recordTypeVisibilities'][0])
+        user_rt_visibilities['Object'] = user_rt_visibilities['recordType'].apply(lambda x: x.split('.')[0])
+        user_rt_visibilities['RecordType'] = user_rt_visibilities['recordType'].apply(lambda x: x.split('.')[1])
+        
+        for object in objects:
+            if object.lower() == 'account':
+                object_describe = task_result_dict[object]['recordTypeInfos'].T
+                object_record_types = object_describe[object_describe['active'] == True].reset_index()[['name','defaultRecordTypeMapping','developerName','master','recordTypeId']].copy()
+                user_object_rt_visibilities = user_rt_visibilities[(user_rt_visibilities['Object'] == object) | (user_rt_visibilities['Object'] == 'PersonAccount')][['default','personAccountDefault','Object','RecordType','visible']].copy()
+                
+            else:
+                object_describe = task_result_dict[object]['recordTypeInfos'].T
+                object_record_types = object_describe[object_describe['active'] == True].reset_index()[['name','defaultRecordTypeMapping','developerName','master','recordTypeId']].copy()
+                user_object_rt_visibilities = user_rt_visibilities[user_rt_visibilities['Object'] == object][['default','personAccountDefault','Object','RecordType','visible']].copy()
+
+            object_rt_visibility_with_master = pd.merge(user_object_rt_visibilities, object_record_types, left_on='RecordType', right_on='developerName', how='outer')
+            object_rt_visibility_with_master['visible'].fillna(False, inplace=True)
+            if not object_rt_visibility_with_master['visible'].any():
+                object_rt_visibility_with_master.loc[object_rt_visibility_with_master['developerName'] == 'Master', 'visible'] = True
+            if not object_rt_visibility_with_master['default'].any():
+                object_rt_visibility_with_master.loc[object_rt_visibility_with_master['developerName'] == 'Master', 'default'] = True
+                
+            visible_object_rt = object_rt_visibility_with_master[object_rt_visibility_with_master['visible'] == True].drop(['defaultRecordTypeMapping'], axis=1)
+            results[object] = visible_object_rt
+        
+        return results
+    
+    
+    async def permissionable_fields_bulk_check(self, object_list):
+        permissionable_fields = {}
+        nonpermissionable_fields = {}
+        async_permissionable_fields =  async_wrap(self.object_describe)
+        async_metadata_read = async_wrap(self.metadata_read)
+        
+        
+        task_dict = {}
+        task_result_dict = {}
+        
+        for object_name in object_list:
+            task_dict[object_name] = async_permissionable_fields(object_name)
+            task_dict[object_name + '_metadata'] = async_metadata_read('CustomObject', object_name)
+            
+        task_results = await asyncio.gather(*task_dict.values())
+        
+        for object_name, task_result in zip(task_dict.keys(), task_results):
+            task_result_dict[object_name] = task_result
+        
+        
+        for object in object_list:
+            permissionable_fields[object] = pd.DataFrame(task_result_dict[object + "_metadata"]['fields'][0])['fullName'].to_list()
+            
+            nonpermissionable_fields[object] = task_result_dict[object]['fields'].T[task_result_dict[object]['fields'].T['permissionable'] == False].index.tolist()
+        return permissionable_fields, nonpermissionable_fields, task_result_dict
+    
+    async def get_layout_metadata(self, layout_name):
+        # Layout Name is the Object API Name + Page Layout Name of the layout, for example:
+        # Account-Hospital Department
+        
+        async_metadata_read = async_wrap(self.metadata_read)
+        
+        layout_metadata = await async_metadata_read('Layout', layout_name)
+        
+        def parse_layoutSections(layout_metadata):
+            layoutSections = pd.DataFrame(layout_metadata)
+            layoutSections['layoutColumns'] = layoutSections['layoutColumns'].apply(lambda row: list(filter(lambda item: item is not None, row)))
+            layoutSections = layoutSections.explode('layoutColumns').reset_index(drop=True)
+            layoutSections['layoutColumns'] = layoutSections['layoutColumns'].apply(lambda row: "" if str(row) == 'nan' else row['layoutItems'])
+            layoutSections = layoutSections.explode('layoutColumns').reset_index(drop=True)
+            layoutSections = pd.concat([layoutSections, layoutSections['layoutColumns'].apply(pd.Series, dtype=str).add_prefix('layoutColumns.')], axis=1).drop(['layoutColumns', "layoutColumns.0"], axis=1)
+            layoutSections.fillna("", inplace=True)
+            layoutSections.drop_duplicates(inplace=True)
+            return layoutSections
+
+        def parse_platformActionList(platformActionList_metadata):
+            platformActionList = pd.DataFrame(platformActionList_metadata)
+            platformActionList = pd.concat([platformActionList, platformActionList['platformActionListItems'].apply(pd.Series, dtype=str).add_prefix('platformActionListItems.')], axis=1).drop(['platformActionListItems'], axis=1)
+            return platformActionList
+
+
+        def parse_quickActionList(quickActionList_metadata):
+            quickActionList = pd.DataFrame(quickActionList_metadata)
+            quickActionList = pd.concat([quickActionList, quickActionList['quickActionListItems'].apply(pd.Series, dtype=str).add_prefix('quickActionListItems.')], axis=1).drop(['quickActionListItems'], axis=1)
+            return quickActionList
+
+        parsed_layout_metadata = {}
+        parsed_layout_metadata['customButtonsList'] = layout_metadata['customButtons'][0]
+        parsed_layout_metadata['excludeButtonsList'] = layout_metadata['excludeButtons'][0]
+        # Adding required fields from the main page layout gives you the final list of mini layout items
+        parsed_layout_metadata['miniLayoutDict'] = dict(layout_metadata['miniLayout'][0]) if layout_metadata['miniLayout'][0] != None else {'fields': [],'relatedLists': []}
+        parsed_layout_metadata['layoutSectionsDataFrame'] = parse_layoutSections(layout_metadata['layoutSections'][0]) if layout_metadata['layoutSections'][0] != None else pd.DataFrame()
+        parsed_layout_metadata['platformActionListDataFrame'] = parse_platformActionList(layout_metadata['platformActionList'][0]) if layout_metadata['platformActionList'][0] != None else pd.DataFrame()
+        parsed_layout_metadata['quickActionListDataFrame'] = parse_quickActionList(layout_metadata['quickActionList'][0]) if layout_metadata['quickActionList'][0] != None else pd.DataFrame()
+        parsed_layout_metadata['relatedListDataFrame'] = pd.DataFrame(layout_metadata['relatedLists'][0]) if layout_metadata['relatedLists'][0] != None else pd.DataFrame()
+        return parsed_layout_metadata
+    
+    ### ----------------------------------------------------------------------------------------------------
+    ### Synchronous Metadata Functions
+    ### ----------------------------------------------------------------------------------------------------
+
+    def object_describe(self, sobject_api_name: str, export_excel: bool=False):
+        """
+
+        """
+        sfSchema = getattr(self.sf, sobject_api_name).describe()
+        boolMetadata = {}
+        nonetypeMetadata = {}
+        strMetadata = {}
+        orderedDictMetadata = pd.Series(dtype='object')
+        childRelationshipsPD = pd.DataFrame()
+        recordTypeInfosPD = pd.DataFrame()
+        fieldsPD = pd.DataFrame()
+        supportedScopesPD = pd.DataFrame()
+        namedLayoutInfosPD = pd.DataFrame()
+        actionOverridesPD = pd.DataFrame()
+
+        for metadata in sfSchema:
+            ## Processes all metadata that would return a boolean datatype
+            if type(sfSchema[metadata]) is bool:
+                boolMetadata[metadata] = sfSchema[metadata]
+
+            ## Processes all metadata that would return a NoneType datatype
+            elif type(sfSchema[metadata]) == type(None):
+                nonetypeMetadata[metadata] = sfSchema[metadata]
+
+            ## Processes all metadata that would return a string datatype
+            elif type(sfSchema[metadata]) is str:
+                strMetadata[metadata] = sfSchema[metadata]
+            ## Processes all metadata that would return an OrderedDict data type
+            elif type(sfSchema[metadata]) is OrderedDict and len(sfSchema[metadata]) != 0:
+                orderedDictMetadata = pd.concat([orderedDictMetadata,pd.Series(sfSchema['urls'])])
+            elif type(sfSchema[metadata]) is OrderedDict and len(sfSchema[metadata]) == 0:
+                nonetypeMetadata[metadata] = "None"
+
+            ## Processes all metadata that would return a list data type
+            elif type(sfSchema[metadata]) is list and len(sfSchema[metadata]) != 0:
+                if metadata == 'childRelationships':
+                    childRelationshipsPD = pd.DataFrame(sfSchema['childRelationships'], index = pd.DataFrame(sfSchema['childRelationships'])['field'])
+                    childRelationshipsPD = childRelationshipsPD.drop('field', axis=1).T
+                if metadata == 'recordTypeInfos':
+                    recordTypeInfosPD = pd.DataFrame(sfSchema['recordTypeInfos'], index = pd.DataFrame(sfSchema['recordTypeInfos'])['name'])
+                    recordTypeInfosPD = recordTypeInfosPD.drop('name', axis = 1).T  
+                if metadata == 'fields':
+                    fieldsPD = pd.DataFrame(sfSchema['fields'], index = pd.DataFrame(sfSchema['fields'])['name'])
+                    fieldsPD = fieldsPD.drop('name', axis = 1).T
+                if metadata == 'supportedScopes':
+                    supportedScopesPD = pd.DataFrame(sfSchema['supportedScopes'], index = pd.DataFrame(sfSchema['supportedScopes'])['name'])
+                    supportedScopesPD = supportedScopesPD.drop('name', axis = 1).T
+                if metadata == 'actionOverrides':
+                    actionOverridesPD = pd.DataFrame(sfSchema['actionOverrides'], index = pd.DataFrame(sfSchema['actionOverrides'])['name'])
+                    actionOverridesPD = actionOverridesPD.drop('name', axis = 1).T
+                if metadata == 'namedLayoutInfos':
+                    namedLayoutInfosPD = pd.DataFrame(sfSchema['namedLayoutInfos'], index = pd.DataFrame(sfSchema['namedLayoutInfos'])['name'])
+                    namedLayoutInfosPD = namedLayoutInfosPD.drop('name', axis = 1).T
+            ## Parses all empty list metadata
+            elif type(sfSchema[metadata]) is list and len(sfSchema[metadata]) == 0:
+                nonetypeMetadata[metadata] = "None"
+            else:
+                nonetypeMetadata[metadata] = "Unrecognized metadata type: " + metadata
+
+        output = {'metadata': pd.concat([pd.Series(nonetypeMetadata),
+                    pd.Series(boolMetadata),
+                    pd.Series(strMetadata),
+                    orderedDictMetadata]),
+                    'childRelationships': childRelationshipsPD if len(childRelationshipsPD)!=0 else None,
+                    'recordTypeInfos': recordTypeInfosPD if len(recordTypeInfosPD)!=0 else None,
+                    'fields': fieldsPD if len(fieldsPD)!=0 else None,
+                    'supportedScopes': supportedScopesPD if len(supportedScopesPD)!=0 else None, 
+                    'namedLayoutInfos': namedLayoutInfosPD if len(namedLayoutInfosPD)!=0 else None,
+                    'actionOverrides': actionOverridesPD if len(actionOverridesPD)!=0 else None}
+        if export_excel:
+            with pd.ExcelWriter(sobject_api_name + ' describe output.xlsx') as writer:  
+                for key in output.keys():
+                    try:
+                        pd.DataFrame(output[key]).to_excel(writer, sheet_name=key)
+                    except:
+                        continue
+
+        return output
+
+    def field_describe(self, objects: List = ['Account','Address_vod__c','Child_Account_vod__c'], 
+    attributes: List = ['name','type','length']) -> pd.DataFrame:
+        """
+        Returns a dataframe of the field metadata for the specified objects and attributes.
+
+        Parameters
+        ----------
+        objects : List, optional
+            A list of objects to get field metadata for. The default is ['Account','Address_vod__c','Child_Account_vod__c'].
+        attributes : List, optional
+            A list of attributes to get field metadata for. The default is ['name','type','length'].
+            For a full list of attributes, see 
+            https://developer.salesforce.com/docs/atlas.en-us.api.meta/api/sforce_api_calls_describesobjects_describesobjectresult.htm
+            A list of attributes can also be found by using the object_describe() method's field attribute.
+
+        Returns
+        -------
+        pd.DataFrame
+            A dataframe of the field metadata for the specified objects and attributes.
+        
+        """
+        outputList = []
+        columnNames = []
+        for sObjectAPIName in objects:
+            for attribute in attributes:
+                outputList.append([field[attribute] for field in getattr(self.sf, sObjectAPIName).describe()['fields']])
+                if attribute == "name":
+                    columnNames.append(sObjectAPIName)
+                else:
+                    columnNames.append(attribute.title())
+        field_describe = pd.DataFrame(outputList).transpose()
+        field_describe.columns = columnNames
+        return field_describe
+
+    def set_user_password(self, user_id, new_password):
+        result = {}
+        try:
+            result = self.sf_api_call(f'/services/data/{self.api_version}/sobjects/User/{user_id}/password', method='POST', data={'NewPassword': new_password})
+        except Exception as e:
+            message_list = str(e).split(" : ")[1].strip().removeprefix("b'[").removesuffix("]'")
+            result = ast.literal_eval(message_list)
+            result['user_id'] = user_id
+        
+        if len(result) == 0:
+            result = {'user_id': user_id,'message': 'success',  'errorCode': None}
+        return result
+        
+
+    def picklist_dataframe_stacked(self,objects: List =['Account','Address_vod__c','Child_Account_vod__c']) -> pd.DataFrame:
+        """
+        TODO:
+        
+        Description of what it does
+        
+        Description of arguments and data types
+        
+        Description of return values and data types
+        
+        Description of Errors raised
+        
+        Extra Notes and Examples of Usage
+        """
+        output_df = pd.DataFrame()
+        for object in objects:
+            objectDescribe = getattr(self.sf, object).describe()
+            processing_df = pd.DataFrame(pd.DataFrame([pd.Series(data = [picklist['value'] for picklist in field['picklistValues']], 
+                                                                   name = object + "." + field["name"]) for field in objectDescribe['fields'] if field['type'] == 'picklist']).stack())
+            processing_df.columns = ['Picklist API Value']
+            processing_df['CRM Object and Field API'] = processing_df.index.get_level_values(0)
+            processing_df[['CRM Object API','CRM Field API']] = processing_df['CRM Object and Field API'].str.split(".", expand = True)
+            processing_df.reset_index(drop=True, inplace=True)
+            output_df = pd.concat([output_df,processing_df])
+        return output_df
+
+    def picklist_dataframe(self,objects = ['Account','Address_vod__c','Child_Account_vod__c']) -> List:
+        """
+        TODO:
+        
+        Description of what it does
+        
+        Description of arguments and data types
+        
+        Description of return values and data types
+        
+        Description of Errors raised
+        
+        Extra Notes and Examples of Usage
+        """
+        referenceList = []
+        for object in objects:
+            objectDescribe = getattr(self.sf, object).describe()
+            objectPicklistValues = pd.DataFrame(index=range(0,max(len(field["picklistValues"]) for field in objectDescribe['fields'] if field['type'] == 'picklist')))
+            for x in [pd.Series(data = [picklist['value'] for picklist in field['picklistValues']], name = object + "." + field["name"]) for field in objectDescribe['fields'] if field['type'] == 'picklist']:
+                objectPicklistValues.insert(0, str(x.name), x)
+            referenceList.append(objectPicklistValues)
+        return referenceList
+
+    def record_type_retrieval(self, objectAPIName, fieldAPINames = ["Id","Name",'SobjectType', 'IsActive']):
+        """
+        TODO:
+        
+        Description of what it does
+        
+        Description of arguments and data types
+        
+        Description of return values and data types
+        
+        Description of Errors raised
+        
+        Extra Notes and Examples of Usage
+        """
+        sfRTDF = pd.DataFrame(self.sf.query_all("SELECT "+ ",".join(fieldAPINames) + " from RecordType WHERE SobjectType = '" + objectAPIName + "'")['records'])
+        
+        # If only master RT exists
+        if len(sfRTDF) == 0:
+            master_rt = {
+                "Name": "Master",
+                "DeveloperName": "Master",
+                "IsActive": True,
+            }
+
+            sfRTDF = pd.DataFrame(master_rt, index=[0])
+        else:
+            sfRTDF.drop(columns="attributes", inplace = True)
+        return sfRTDF
+
+    def object_permission_check(self, object, permission):
+        data = transform_sf_result_set_rec(self.sf.query_all(f"""SELECT Assignee.Id, Assignee.Name,Assignee.IsActive, Assignee.UserName, PermissionSet.Id, PermissionSet.isOwnedByProfile, PermissionSet.Profile.Name, PermissionSet.Label
+            FROM PermissionSetAssignment
+            WHERE PermissionSetId
+            IN (SELECT ParentId
+            FROM ObjectPermissions
+            WHERE SObjectType IN ('{object}') AND
+            ({permission} = true)) AND Assignee.IsActive = TRUE""")['records'])
+        
+        profile_violations = data[data['PermissionSet.IsOwnedByProfile']== True][['User.Username', 'Profile.Name']]
+        permission_set_violations = data[data['PermissionSet.IsOwnedByProfile']== False][['User.Username', 'PermissionSet.Label']]
+        result = []
+        for user in profile_violations['User.Username'].unique():
+            result.append({"UserName": user, 
+                            "Object API Name" : object,
+                            "Permission": permission,
+                            "Profile": "; ".join(list(profile_violations[profile_violations['User.Username'] == user]['Profile.Name'].unique())),
+                            "Permission Set": ""
+                        
+                        }
+                        
+                        )
+            
+        for user in permission_set_violations['User.Username'].unique():
+            result.append({"UserName": user, 
+                                                            "Object API Name" : object,
+                                                            "Permission": permission,
+                                                            "Profile": "",
+                                                            "Permission Set": "; ".join(list(permission_set_violations[permission_set_violations['User.Username'] == user]['PermissionSet.Label'].unique()))})
+        return result
+
+    def field_permission_check(self, object) -> dict[str, pd.DataFrame]:
+        fls_results = transform_sf_result_set_rec(self.sf.query_all(f"""
+                                            SELECT Field,
+                                            ParentId,
+                                            PermissionsEdit,
+                                            PermissionsRead,
+                                            SobjectType FROM FieldPermissions
+                                            WHERE SobjectType in ('{object}')
+                                            """)['records'])
+
+        permissionSetProfiles = transform_sf_result_set_rec(self.sf.query_all("""
+                                                    SELECT Id,Description,IsOwnedByProfile,Name,ProfileId, 
+                                                    Profile.Name, Profile.Description,Type FROM PermissionSet
+                                                    """)['records'])
+
+        profiles = permissionSetProfiles[permissionSetProfiles['PermissionSet.IsOwnedByProfile'] == True][['PermissionSet.ProfileId','PermissionSet.Id','Profile.Name','Profile.Description']].copy()
+        permissionSets = permissionSetProfiles[permissionSetProfiles['PermissionSet.IsOwnedByProfile'] == False][['PermissionSet.Id','PermissionSet.Name','PermissionSet.Description']].copy()
+
+        permissionSetPermissions = pd.merge(fls_results, permissionSets, left_on='FieldPermissions.ParentId', right_on='PermissionSet.Id', how='inner').drop(columns=['PermissionSet.Id'], axis=1)
+        permissionSetPermissions.columns = ['Field API Name', 'Permission Set Id', 'FLS Edit', 'FLS Read', 'Object API Name', 'Permission Set Name', 'Permission Set Description']
+        permissionSetPermissions = permissionSetPermissions[['Permission Set Id', 'Permission Set Name', 'Permission Set Description', 'Object API Name', 'Field API Name', 'FLS Edit', 'FLS Read']]
+        permissionSetPermissions['Field API Name'] = permissionSetPermissions['Field API Name'].apply(lambda x: x.split('.')[-1])
+
+
+        profilePermissions = pd.merge(fls_results, profiles, left_on='FieldPermissions.ParentId', right_on='PermissionSet.Id', how='inner').drop(columns=['PermissionSet.Id','FieldPermissions.ParentId'], axis=1)
+        profilePermissions.columns = ['Field API Name', 'FLS Edit', 'FLS Read', 'Object API Name','Profile Id',  'Profile Name', 'Profile Description']
+        profilePermissions = profilePermissions[['Profile Id', 'Profile Name', 'Profile Description', 'Object API Name', 'Field API Name', 'FLS Edit', 'FLS Read']]
+        profilePermissions['Field API Name'] = profilePermissions['Field API Name'].apply(lambda x: x.split('.')[-1])
+        
+        return {'permissionSetPermissions': permissionSetPermissions, 'profilePermissions': profilePermissions}
+
+
+    # Retrieves the Page Layout by Profile by Record Type data for all objects in the org
+    def retrieve_profile_layout_record_type_matrix_all(self, return_pivot_table = False):
+        account_page_layouts_bulk = transform_sf_result_set_rec(self.tooling_query_all("""select LayoutId, 
+                                                                                    ProfileId, Profile.Name, 
+                                                                                    RecordTypeId, RecordType.Name, 
+                                                                                    Layout.Name, TableEnumOrId from 
+                                                                                    ProfileLayout"""))
+
+        account_page_layouts_bulk['ProfileName'] = account_page_layouts_bulk.apply(lambda row: row['ProfileLayout.Profile']['Name'] if row['ProfileLayout.Profile'] else "", axis=1)
+        account_page_layouts_bulk['RecordTypeName'] = account_page_layouts_bulk.apply(lambda row: row['ProfileLayout.RecordType']['Name'] if row['ProfileLayout.RecordType'] else "", axis=1)
+        account_page_layouts_bulk['PageLayout'] = account_page_layouts_bulk.apply(lambda row: row['ProfileLayout.Layout']['Name'] if row['ProfileLayout.Layout'] else "", axis=1)
+        account_page_layouts_bulk.drop(['ProfileLayout.Profile','ProfileLayout.RecordType','ProfileLayout.Layout'], axis=1, inplace=True)
+
+
+        object_dataframe = pd.DataFrame(self.tooling_query_all("Select DeveloperName from CustomObject"))
+        object_dataframe['ObjectID'] = object_dataframe.apply(lambda row: row['attributes']['url'].split('/')[-1] if row['attributes']['url'] else "", axis=1)
+
+
+        account_page_layouts_bulk = account_page_layouts_bulk.merge(object_dataframe, left_on='ProfileLayout.TableEnumOrId', right_on='ObjectID', how='left').copy()
+        account_page_layouts_bulk['DeveloperName'] = account_page_layouts_bulk.apply(lambda row: row['DeveloperName'] if pd.notnull(row['DeveloperName']) else row['ProfileLayout.TableEnumOrId'], axis=1)
+        account_page_layouts_bulk.drop(['ObjectID','attributes'], axis=1, inplace=True)
+            
+        # Fill in the RecordTypeName colum with the Master Record Type Name
+        account_page_layouts_bulk['RecordTypeName'] = account_page_layouts_bulk['RecordTypeName'].apply(lambda row: row if row else 'Master')
+        # Filter out Deprecated Profiles
+        account_page_layouts_bulk = account_page_layouts_bulk[(~account_page_layouts_bulk['ProfileName'].isnull()) & (account_page_layouts_bulk['ProfileName'] != '') & (account_page_layouts_bulk['PageLayout'] != 'Veeva Vpro Unit Testing Layout')]
+        
+        if return_pivot_table:
+            return account_page_layouts_bulk.pivot(index='ProfileName', columns=['DeveloperName','RecordTypeName'], values='PageLayout')
+        else:
+            return account_page_layouts_bulk
+    
+    #######################################################################################
+    # Veeva CRM Server API Functions
+    #######################################################################################
+
+    def load_veeva_common(self):
+        self.veeva_common = self.query("Select * From Veeva_Common_vod__c").to_dict()
+    
+    def load_org_info(self):
+        self.org_info = self.query("Select * From Organization").to_dict()
+        
+    def get_network_admin_sf_user_info(self):
+        
+        if self.veeva_common is None:
+            self.load_veeva_common()
+        
+        if self.org_info is None:
+            self.load_org_info()
+            
+        try:
+            response = requests.get(f"{self.veeva_common['Veeva_Server_vod__c'][0]}/{self.veeva_common['Veeva_Version_vod__c'][0]}?VER={self.veeva_common['Veeva_Version_vod__c'][0]}&SSID={self.session_id}&url=https://{self.instance}/services/Soap/u/24.0/{self.org_info['Id'][0]}&ses={self.session_id}&oType=networkAdmin&event=getSFCredentials")
+            return {'status': response.status_code, 'response': response.json()}
+        except:
+            return {'status': 500, 'response': {"error": "Unable to "}}
+        
+    def get_network_admin_network_user_info(self):
+        
+        if self.veeva_common is None:
+            self.load_veeva_common()
+        
+        if self.org_info is None:
+            self.load_org_info()
+            
+        try:
+            response = requests.get(f"{self.veeva_common['Veeva_Server_vod__c'][0]}/{self.veeva_common['Veeva_Version_vod__c'][0]}?VER={self.veeva_common['Veeva_Version_vod__c'][0]}&SSID={self.session_id}&url=https://{self.instance}/services/Soap/u/24.0/{self.org_info['Id'][0]}&ses={self.session_id}&oType=networkAdmin&event=getNetworkCredentials")
+            return {'status': response.status_code, 'response': response.json()}
+        except:
+            return {'status': 500, 'response': {"error": "Unable to get network admin credentials"}}
+
+    def engage_admin_retrieve_groups(self):
+
+        headers = {
+            "Accept": "application/json, text/plain, */*",
+            "Sfendpoint": f"https://{self.instance.split('.')[0]}--c.sandbox.vf.force.com/services/Soap/u/54.0/{self.sfOrgId}",
+            "Sfsession": self.session_id,
+        }
+        
+        if self.veeva_common is None:
+            self.load_veeva_common()
+
+        veeva_server = self.veeva_common['Veeva_Server_vod__c'][0]
+        veeva_version = self.veeva_common['Veeva_Version_vod__c'][0]
+
+
+        try:
+            response = requests.get(f'{veeva_server}/{veeva_version}/api/v1/hcpproxy/groups', headers=headers)
+            return {'status': response.status_code, 'response': response.json()}
+        except:
+            return {'status': 500, 'response': {"error": "Unable to retrieve Engage groups"}}
+        
+    def engage_admin_retrieve_users(self):
+        headers = {
+            "Accept": "application/json, text/plain, */*",
+            "Sfendpoint": f"https://{self.instance.split('.')[0]}--c.sandbox.vf.force.com/services/Soap/u/54.0/{self.sfOrgId}",
+            "Sfsession": self.session_id,
+        }
+
+        if self.veeva_common is None:
+            self.load_veeva_common()
+
+        veeva_server = self.veeva_common['Veeva_Server_vod__c'][0]
+        veeva_version = self.veeva_common['Veeva_Version_vod__c'][0]
+
+
+        try:
+            response = requests.get(f'{veeva_server}/{veeva_version}/api/v1/hcpproxy/usersinfo', headers=headers)
+            return {'status': response.status_code, 'response': response.json()}
+        except:
+            return {'status': 500, 'response': {"error": "Unable to retrieve Engage users."}}
+
+    def engage_admin_get_license_info(self):
+        headers = {
+            "Accept": "application/json, text/plain, */*",
+            "Sfendpoint": f"https://{self.instance.split('.')[0]}--c.sandbox.vf.force.com/services/Soap/u/54.0/{self.sfOrgId}",
+            "Sfsession": self.session_id,
+        }
+
+        if self.veeva_common is None:
+            self.load_veeva_common()
+
+        veeva_server = self.veeva_common['Veeva_Server_vod__c'][0]
+        veeva_version = self.veeva_common['Veeva_Version_vod__c'][0]
+
+
+        try:
+            response = requests.get(f'{veeva_server}/{veeva_version}/api/v1/remoteMeetings/orgs/{self.sfOrgId}', headers=headers)
+            return {'status': response.status_code, 'response': response.json()}
+        except:
+            return {'status': 500, 'response': {"error": "Unable to retrieve Engage license info."}}
+        
+    def engage_meeting_process_admin_retrieve_history(self):
+        headers = {
+            "Accept": "application/json, text/plain, */*",
+            "Sfendpoint": f"https://{self.instance.split('.')[0]}--c.sandbox.vf.force.com/services/Soap/u/54.0/{self.sfOrgId}",
+            "Sfsession": self.session_id,
+        }
+
+        if self.veeva_common is None:
+            self.load_veeva_common()
+
+        mc_server = self.veeva_common['Multichannel_Server_vod__c'][0]
+        mc_context_root = self.veeva_common['Multichannel_Context_Root_vod__c'][0]
+
+
+        try:
+            response = requests.get(f'{mc_server}/{mc_context_root}/api/v1/epp-service/refresh/records', headers=headers)
+            return {'status': response.status_code, 'response': response.json()}
+        except:
+            return {'status': 500, 'response': {"error": "Unable to retrieve Engage process admin history."}}
+    
+    def engage_meeting_process_admin_retrieve_veeva_crm_connection_management(self):
+        headers = {
+            "Accept": "application/json, text/plain, */*",
+            "Sfendpoint": f"https://{self.instance.split('.')[0]}--c.sandbox.vf.force.com/services/Soap/u/54.0/{self.sfOrgId}",
+            "Sfsession": self.session_id,
+        }
+
+        if self.veeva_common is None:
+            self.load_veeva_common()
+
+        mc_server = self.veeva_common['Multichannel_Server_vod__c'][0]
+        mc_context_root = self.veeva_common['Multichannel_Context_Root_vod__c'][0]
+
+
+        try:
+            response = requests.get(f'{mc_server}/{mc_context_root}/api/v1/credentials/SalesForce_EPP?systemId={self.sfOrgId}', headers=headers)
+            return {'status': response.status_code, 'response': response.json()}
+        except:
+            return {'status': 500, 'response': {"error": "Unable to retrieve Engage process admin Veeva CRM connection management."}}
+        
+    def engage_meeting_process_admin_retrieve_veeva_vault_login_credential_management(self):
+        headers = {
+            "Accept": "application/json, text/plain, */*",
+            "Sfendpoint": f"https://{self.instance.split('.')[0]}--c.sandbox.vf.force.com/services/Soap/u/54.0/{self.sfOrgId}",
+            "Sfsession": self.session_id,
+        }
+
+        if self.veeva_common is None:
+            self.load_veeva_common()
+
+        mc_server = self.veeva_common['Multichannel_Server_vod__c'][0]
+        mc_context_root = self.veeva_common['Multichannel_Context_Root_vod__c'][0]
+
+
+        try:
+            response = requests.get(f'{mc_server}/{mc_context_root}/api/v1/credentials/Vault_EPP', headers=headers)
+            return {'status': response.status_code, 'response': response.json()}
+        except:
+            return {'status': 500, 'response': {"error": "Unable to retrieve Engage process admin Veeva Vault login credential management."}}
+
+    def engage_metadata_sync_admin_retrieve_vault_connection_management(self):
+        headers = {
+            "Accept": "application/json, text/plain, */*",
+            "Sfendpoint": f"https://{self.instance.split('.')[0]}--c.sandbox.vf.force.com/services/Soap/u/54.0/{self.sfOrgId}",
+            "Sfsession": self.session_id,
+        }
+
+        if self.veeva_common is None:
+            self.load_veeva_common()
+
+        mc_server = self.veeva_common['Multichannel_Server_vod__c'][0]
+        mc_context_root = self.veeva_common['Multichannel_Context_Root_vod__c'][0]
+
+
+        try:
+            response = requests.get(f'{mc_server}/{mc_context_root}/api/v1/credentials/Vault_Engage', headers=headers)
+            return {'status': response.status_code, 'response': response.json()}
+        except:
+            return {'status': 500, 'response': {"error": "Unable to retrieve Engage metadata sync admin Veeva Vault connection management."}}
+
+    def engage_metadata_sync_admin_retrieve_crm_connection_management(self):
+        headers = {
+            "Accept": "application/json, text/plain, */*",
+            "Sfendpoint": f"https://{self.instance.split('.')[0]}--c.sandbox.vf.force.com/services/Soap/u/54.0/{self.sfOrgId}",
+            "Sfsession": self.session_id,
+        }
+
+        if self.veeva_common is None:
+            self.load_veeva_common()
+
+        mc_server = self.veeva_common['Multichannel_Server_vod__c'][0]
+        mc_context_root = self.veeva_common['Multichannel_Context_Root_vod__c'][0]
+
+
+        try:
+            response = requests.get(f'{mc_server}/{mc_context_root}/api/v1/credentials/SalesForce_Engage?systemId=00D2g0000000ipMEAQ', headers=headers)
+            return {'status': response.status_code, 'response': response.json()}
+        except:
+            return {'status': 500, 'response': {"error": "Unable to retrieve Engage metadata sync admin CRM connection management."}}
+
+    def engage_metadata_sync_admin_retrieve_activity_debug_log(self):
+        headers = {
+            "Accept": "application/json, text/plain, */*",
+            "Sfendpoint": f"https://{self.instance.split('.')[0]}--c.sandbox.vf.force.com/services/Soap/u/54.0/{self.sfOrgId}",
+            "Sfsession": self.session_id,
+        }
+
+        if self.veeva_common is None:
+            self.load_veeva_common()
+
+        mc_server = self.veeva_common['Multichannel_Server_vod__c'][0]
+        mc_context_root = self.veeva_common['Multichannel_Context_Root_vod__c'][0]
+
+
+        try:
+            response = requests.get(f'{mc_server}/{mc_context_root}/api/v1/debug-log/collection?count=20&orgId=00D2g0000000ipMEAQ', headers=headers)
+            return {'status': response.status_code, 'response': response.json()}
+        except:
+            return {'status': 500, 'response': {"error": "Unable to retrieve Engage metadata sync admin activity debug log."}}
+
+    def engage_metadata_sync_admin_retrieve_metadata_sync(self):
+        headers = {
+            "Accept": "application/json, text/plain, */*",
+            "Sfendpoint": f"https://{self.instance.split('.')[0]}--c.sandbox.vf.force.com/services/Soap/u/54.0/{self.sfOrgId}",
+            "Sfsession": self.session_id,
+        }
+
+        if self.veeva_common is None:
+            self.load_veeva_common()
+
+        mc_server = self.veeva_common['Multichannel_Server_vod__c'][0]
+        mc_context_root = self.veeva_common['Multichannel_Context_Root_vod__c'][0]
+
+
+        try:
+            response = requests.get(f'{mc_server}/{mc_context_root}/api/v1/mcservice/status/refresh?count=10&recordType=Engage', headers=headers)
+            return {'status': response.status_code, 'response': response.json()}
+        except:
+            return {'status': 500, 'response': {"error": "Unable to retrieve Engage metadata sync admin metadata sync."}}
+        
+    def veeva_process_admin_alerts_status_report(self):
+        headers = {
+            "Accept": "application/json, text/plain, */*",
+            "Sfendpoint": f"https://{self.instance.split('.')[0]}--c.sandbox.vf.force.com/services/Soap/u/54.0/{self.sfOrgId}",
+            "Sfsession": self.session_id,
+        }
+
+        if self.veeva_common is None:
+            self.load_veeva_common()
+
+        mc_server = self.veeva_common['Multichannel_Server_vod__c'][0]
+        mc_context_root = self.veeva_common['Multichannel_Context_Root_vod__c'][0]
+
+
+        try:
+            response = requests.get(f'{mc_server}/{mc_context_root}/api/v1/email-alert/recipients', headers=headers)
+            return {'status': response.status_code, 'response': response.json()}
+        except:
+            return {'status': 500, 'response': {"error": "Unable to retrieve Veeva process admin alerts status report."}}
+
+    def process_scheduler_get_jobs(self):
+        headers = {
+            "Accept": "application/json, text/plain, */*",
+            "Sfendpoint": f"https://{self.instance.split('.')[0]}--c.sandbox.vf.force.com/services/Soap/u/54.0/{self.sfOrgId}",
+            "Sfsession": self.session_id,
+        }
+
+        if self.veeva_common is None:
+            self.load_veeva_common()
+
+        mc_server = self.veeva_common['Multichannel_Server_vod__c'][0]
+        mc_context_root = self.veeva_common['Multichannel_Context_Root_vod__c'][0]
+
+
+        try:
+            response = requests.get(f'{mc_server}/{mc_context_root}/api/v1/scheduler/jobs', headers=headers)
+            return {'status': response.status_code, 'response': response.json()}
+        except:
+            return {'status': 500, 'response': {"error": "Unable to retrieve process scheduler jobs."}}
+
+
+
+
+
+
+    ##############################################################################################################
+    # WSDL Derived Functions
+    ##############################################################################################################
+
+    @serialze_zeep
+    def metadata_read(self, metadata_type: str, fullName: str):
+        return getattr(self.sf.mdapi, metadata_type).read(fullName)
+
+    def metadata_delete(self, metadata_type: str, fullName: str):
+        return getattr(self.sf.mdapi, metadata_type).delete(fullName)
+
+    def metadata_update(self, metadata_type: str, parsed_metadata: dict):
+        mdapi_object = getattr(self.sf.mdapi, metadata_type)()
+        for key in parsed_metadata:
+            setattr(mdapi_object, key, parsed_metadata[key])
+        getattr(self.sf.mdapi, metadata_type).update(mdapi_object)
+        return mdapi_object
+
+    def metadata_create(self, metadata_type: str, parsed_metadata: dict):
+        mdapi_object = getattr(self.sf.mdapi, metadata_type)()
+        for key in parsed_metadata:
+            setattr(mdapi_object, key, parsed_metadata[key])
+        getattr(self.sf.mdapi, metadata_type).create(mdapi_object)
+        return mdapi_object
+
+    def metadata_list(self, metadata_type: str = '', metadata_type_list: list[str] = []) -> list:
+        if len(metadata_type_list) == 0 and metadata_type != '':
+            query = self.sf.mdapi.ListMetadataQuery(type=metadata_type)
+        elif len(metadata_type_list) > 3:
+            raise Exception("You can only query up to 3 metadata types at a time")
+        
+        elif len(metadata_type_list) > 0:
+            query = []
+            for metadata_type in metadata_type_list:
+                query.append(self.sf.mdapi.ListMetadataQuery(type=metadata_type))
+        else:
+            raise Exception("Please populate either metadata_type or metadata_type_list, but not both.")
+        
+        query_response = self.sf.mdapi.list_metadata(query)
+        return query_response
+    
+    def metadata_rename(self, metadata_type: str, previous_name: str, new_name: str): 
+        """
+        Renames the API name of SFDC metadata
+        """
+        getattr(self.sf.mdapi, metadata_type).rename(previous_name, new_name)
+    
+    ### ----------------------------------------------------------------------------------------------------
+    ### Custom Tooling API Methods
+    ### ----------------------------------------------------------------------------------------------------
+    
+    def tooling_query_all(self, query):
+        done = False
+        full_results = []
+        result = self.sf_api_call(f'/services/data/v52.0/tooling/query', method='get', parameters={'q': query})
+        while not done:
+            full_results.extend(result['records'])
+            done = result['done']
+            if not done:
+                result = self.sf_api_call(result['nextRecordsUrl'])
+        return full_results
+
+    ### ----------------------------------------------------------------------------------------------------
+    ### Utility Functions
+    ### ----------------------------------------------------------------------------------------------------
+    def query_performance_feedback(self, query: str):
+        # https://developer.salesforce.com/docs/atlas.en-us.240.0.api_rest.meta/api_rest/dome_query_explain.htm
+        
+        return self.sf_api_call(f'/services/data/{self.api_version}/query?explain={query}')
+    
+    def parse_sf_limits(self, sfdc_limits_result: dict, prefix=None) -> dict:
+        ## Recursively parse the limits result to find the limits that are not 0
+        result = {}
+        for key, item in sfdc_limits_result.items():
+            if set(['Max','Remaining']).issubset(set(item.keys())): 
+                if item['Max'] == 0:
+                    continue
+                else:
+                    result[key if prefix is None else prefix+' - '+key] = dict(zip(['Max','Remaining'],[item['Max'], item['Remaining']]))
+            
+            if len(set(item.keys()) - set(['Max','Remaining'])) > 0:
+                sub_item = item.copy()
+                if 'Max' in sub_item: 
+                    del sub_item['Max']
+                if 'Remaining' in sub_item: 
+                    del sub_item['Remaining']
+                result.update(self.parse_sf_limits(sub_item, prefix=key))
+        return result
+        
+    def sf_api_call(self, action, parameters = {}, method = 'get', data = {}):
+        """
+        Helper function to make calls to Salesforce REST API.
+        Parameters: action (the URL), URL params, method (get, post or patch), data for POST/PATCH.
+        """
+        headers = {
+            'Content-type': 'application/json',
+            'Accept-Encoding': 'gzip',
+            'Authorization': 'Bearer %s' % self.session_id
+        }
+        if method.lower() == 'get':
+            r = requests.request(method, 'https://'+self.instance+action, headers=headers, params=parameters, timeout=30)
+        elif method.lower() in ['post', 'patch']:
+            r = requests.request(method, 'https://'+self.instance+action, headers=headers, json=data, params=parameters, timeout=10)
+        else:
+            # other methods not implemented in this example
+            raise ValueError('Method should be get or post or patch.')
+#         print('Debug: API %s call: %s' % (method, r.url) )
+        if r.status_code < 300:
+            if method=='patch':
+                return None
+            else:
+                try:
+                    return r.json()
+                except:
+                    return {}
+        else:
+            raise Exception('API error when calling %s : %s' % (r.url, r.content))
+
+
+    def join(self, 
+                dataframe, 
+                rt_dataframe, 
+                left_on="", 
+                right_on="", 
+                new_columns=[], 
+                suffix = "_new"):
+        """
+        Joins and appends the Name and DeveloperName columns of record type to the dataframe.
+        The dataframe must contain a column named "RecordTypeId" with the 18 digit SFID of the record type.
+        """
+        df_columns = dataframe.columns.to_list()
+        if right_on not in new_columns:
+            new_columns.insert(0,right_on)
+        dataframe = pd.merge(dataframe, rt_dataframe[new_columns], how = 'inner', 
+                                left_on = left_on,right_on = right_on, suffixes=('', suffix))
+#         dataframe.drop([col for col in dataframe.columns if 'drop' in col], axis=1, inplace=True)
+        return dataframe
```

### Comparing `veevatools-0.0.95/salesforce/utilities/async_utils.py` & `veevatools-0.0.96/salesforce/utilities/async_utils.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import asyncio
-from functools import wraps, partial
-
-async def async_parallel(func, args):
-    # runs the function(s) in parallel
-    return await asyncio.gather(*[func(arg) for arg in args])
-
-async def async_serial(func, args):
-    # runs the function(s) in serial order, 
-    # awaiting for each iteration's completion before executing the next.
-    return [await func(arg) for arg in args]
-
-def async_wrap(func):
-    @wraps(func)
-    async def run(*args, loop=None, executor=None, **kwargs):
-        if loop is None:
-            loop = asyncio.get_event_loop()
-        pfunc = partial(func, *args, **kwargs)
-        return await loop.run_in_executor(executor, pfunc)
+import asyncio
+from functools import wraps, partial
+
+async def async_parallel(func, args):
+    # runs the function(s) in parallel
+    return await asyncio.gather(*[func(arg) for arg in args])
+
+async def async_serial(func, args):
+    # runs the function(s) in serial order, 
+    # awaiting for each iteration's completion before executing the next.
+    return [await func(arg) for arg in args]
+
+def async_wrap(func):
+    @wraps(func)
+    async def run(*args, loop=None, executor=None, **kwargs):
+        if loop is None:
+            loop = asyncio.get_event_loop()
+        pfunc = partial(func, *args, **kwargs)
+        return await loop.run_in_executor(executor, pfunc)
     return run
```

### Comparing `veevatools-0.0.95/salesforce/utilities/df_utils.py` & `veevatools-0.0.96/salesforce/utilities/df_utils.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-import pandas as pd
-from collections import OrderedDict
-from typing import Union, Iterable, final
-
-# ================================================
-# Account Object Functions
-# ================================================
-
-def object_account_drop_personaccount_cols(df: pd.DataFrame) -> pd.DataFrame:
-    # Drops Person Account columns from the DataFrame
-    person_account_list = ['FirstName', 'LastName', 'MiddleName', 'PersonDoNotCall','PersonIndividualId','PersonAssistantName', 'PersonAssistantPhone','PersonBirthdate', 'PersonBirthDate', 'PersonContactId', 'PersonDepartment', 'PersonEmail', 'PersonEmailBouncedDate', 'PersonEmailBouncedReason','PersonHasOptedOutOfFax', 'PersonHasOptedOutOfEmail', 'PersonHomePhone', 'PersonLeadSource', 'PersonMailingAddress', 'PersonMailingCity',
-                           'PersonMailingGeocodeAccuracy', 'PersonMailingLatitude', 'PersonMailingLongitude', 'PersonMailingStreet', 'PersonMobilePhone', 'PersonOtherCity', 'PersonOtherCountry', 'PersonOtherPostalCode', 'PersonOtherState', 'PersonOtherCountryCode', 'PersonOtherStateCode', 'PersonOtherLatitude', 'PersonOtherLongitude', 'PersonOtherPhone', 'PersonOtherStreet', 'PersonTitle', 'Suffix']
-    final_drop = []
-    for column in df.columns:
-        if column[-4:] == '__pc':
-            final_drop.append(column)
-        elif column in person_account_list:
-            final_drop.append(column)
-    
-    return df.drop(columns=final_drop, axis=1)
-
-def object_account_drop_businessaccount_cols(df: pd.DataFrame) -> pd.DataFrame:
-    # Drops Person Account columns from the DataFrame
-    business_account_list = ['DunsNumber','Jigsaw','NaicsCode','NaicsDesc','Name','Sic','Tradestyle','SicDesc','TickerSymbol']
-    final_drop = []
-    for column in df.columns:
-        if column in business_account_list:
-            final_drop.append(column)
-    return df.drop(columns=final_drop, axis=1)
-
-def unpack_column(result: pd.DataFrame, column: str='errors'):
-    return pd.concat([result, result[column].apply(lambda row: pd.Series(row[0]) if len(row) >0 else pd.Series(dtype='int64')).fillna("")], axis=1).drop(columns=[column])
-
-def metadata_parse(metadata_value: Union[pd.DataFrame, Iterable, OrderedDict, bool, list, int, None]) -> Union[Iterable, OrderedDict, dict, bool, list, int, None]:
-    """
-    Function recursively traverses down a set of nested DataFrame, Dict, List, Ordered Dict iterables until
-    it reaches a str, bool, empty list, or None value to return a dict comprising of the original hierarchical data.
-    """
-    if type(metadata_value) == str:
-        return metadata_value
-    elif type(metadata_value) == bool:
-        return metadata_value
-    elif metadata_value is None:
-        return None
-    elif type(metadata_value) == int:
-        return metadata_value
-    elif type(metadata_value) == list:
-        if len(metadata_value) == 0:
-            return []
-        else:
-            working_list = []
-            for item in metadata_value:
-                working_list.append(metadata_parse(item))
-            return working_list
-    elif type(metadata_value) == OrderedDict:
-        working_dict = {}
-        for key in metadata_value.keys():
-            working_dict[key] = metadata_parse(metadata_value[key])
-        return working_dict
-    elif type(metadata_value) == pd.DataFrame:
-        working_df_dict = {}
-        for column in metadata_value.columns:
-            if len(metadata_value[column]) == 0:
-                working_df_dict[column] = None
-            elif len(metadata_value[column]) > 1:
-                for item in metadata_value[column]:
-                    working_df_dict[column] = metadata_parse(item)
-            elif len(metadata_value[column]) == 1:
-                working_df_dict[column] = metadata_parse(metadata_value[column][0])
-        return working_df_dict
+import pandas as pd
+from collections import OrderedDict
+from typing import Union, Iterable, final
+
+# ================================================
+# Account Object Functions
+# ================================================
+
+def object_account_drop_personaccount_cols(df: pd.DataFrame) -> pd.DataFrame:
+    # Drops Person Account columns from the DataFrame
+    person_account_list = ['FirstName', 'LastName', 'MiddleName', 'PersonDoNotCall','PersonIndividualId','PersonAssistantName', 'PersonAssistantPhone','PersonBirthdate', 'PersonBirthDate', 'PersonContactId', 'PersonDepartment', 'PersonEmail', 'PersonEmailBouncedDate', 'PersonEmailBouncedReason','PersonHasOptedOutOfFax', 'PersonHasOptedOutOfEmail', 'PersonHomePhone', 'PersonLeadSource', 'PersonMailingAddress', 'PersonMailingCity',
+                           'PersonMailingGeocodeAccuracy', 'PersonMailingLatitude', 'PersonMailingLongitude', 'PersonMailingStreet', 'PersonMobilePhone', 'PersonOtherCity', 'PersonOtherCountry', 'PersonOtherPostalCode', 'PersonOtherState', 'PersonOtherCountryCode', 'PersonOtherStateCode', 'PersonOtherLatitude', 'PersonOtherLongitude', 'PersonOtherPhone', 'PersonOtherStreet', 'PersonTitle', 'Suffix']
+    final_drop = []
+    for column in df.columns:
+        if column[-4:] == '__pc':
+            final_drop.append(column)
+        elif column in person_account_list:
+            final_drop.append(column)
+    
+    return df.drop(columns=final_drop, axis=1)
+
+def object_account_drop_businessaccount_cols(df: pd.DataFrame) -> pd.DataFrame:
+    # Drops Person Account columns from the DataFrame
+    business_account_list = ['DunsNumber','Jigsaw','NaicsCode','NaicsDesc','Name','Sic','Tradestyle','SicDesc','TickerSymbol']
+    final_drop = []
+    for column in df.columns:
+        if column in business_account_list:
+            final_drop.append(column)
+    return df.drop(columns=final_drop, axis=1)
+
+def unpack_column(result: pd.DataFrame, column: str='errors'):
+    return pd.concat([result, result[column].apply(lambda row: pd.Series(row[0]) if len(row) >0 else pd.Series(dtype='int64')).fillna("")], axis=1).drop(columns=[column])
+
+def metadata_parse(metadata_value: Union[pd.DataFrame, Iterable, OrderedDict, bool, list, int, None]) -> Union[Iterable, OrderedDict, dict, bool, list, int, None]:
+    """
+    Function recursively traverses down a set of nested DataFrame, Dict, List, Ordered Dict iterables until
+    it reaches a str, bool, empty list, or None value to return a dict comprising of the original hierarchical data.
+    """
+    if type(metadata_value) == str:
+        return metadata_value
+    elif type(metadata_value) == bool:
+        return metadata_value
+    elif metadata_value is None:
+        return None
+    elif type(metadata_value) == int:
+        return metadata_value
+    elif type(metadata_value) == list:
+        if len(metadata_value) == 0:
+            return []
+        else:
+            working_list = []
+            for item in metadata_value:
+                working_list.append(metadata_parse(item))
+            return working_list
+    elif type(metadata_value) == OrderedDict:
+        working_dict = {}
+        for key in metadata_value.keys():
+            working_dict[key] = metadata_parse(metadata_value[key])
+        return working_dict
+    elif type(metadata_value) == pd.DataFrame:
+        working_df_dict = {}
+        for column in metadata_value.columns:
+            if len(metadata_value[column]) == 0:
+                working_df_dict[column] = None
+            elif len(metadata_value[column]) > 1:
+                for item in metadata_value[column]:
+                    working_df_dict[column] = metadata_parse(item)
+            elif len(metadata_value[column]) == 1:
+                working_df_dict[column] = metadata_parse(metadata_value[column][0])
+        return working_df_dict
```

### Comparing `veevatools-0.0.95/salesforce/utilities/sf_query_processors.py` & `veevatools-0.0.96/salesforce/utilities/sf_query_processors.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-from collections import OrderedDict
-import pandas as pd
-
-
-def recursive_walk(od_field: OrderedDict):
-    """
-    Recursively flattens each row the results of simple salesforce.
-    Only works for bottom up queries.
-    :param od_field: results returned by simple salesforce (multiple objects)
-    :return: returns a flattened list of dictionaries
-    """
-    d = {}
-    for k in od_field.keys():
-        if isinstance(od_field[k], OrderedDict) & (k != 'attributes'):
-            if 'attributes' in od_field[k].keys():
-                ret_df = recursive_walk(od_field[k])
-                d = {**d, **ret_df}
-            else:
-                obj = od_field['attributes']['type'].replace(" ", ".")
-                d[f'{obj}.{k}'] = ",\n".join([   f'{k}: {v}' for k, v in od_field[k].items() if v is not None])
-        else:
-            if k != 'attributes':
-                obj = od_field['attributes']['type'].replace(" ", ".")
-                d[f'{obj}.{k}'] = od_field[k]
-    return d
-
-def transform_sf_result_set_rec(query_results: OrderedDict):
-    """
-    Recursively flattens the results of simple salesforce. It needs flattening when  selecting
-    multiple objects.
-    :param query_results:
-    :return:
-    """
-    data = []
-    for res in query_results:
-        d = recursive_walk(res)
-        data.append(d)
-    data = pd.DataFrame(data)
-    return data
-
-def deep_merge_dictionaries(source, destination):
-    """
-    run me with nosetests --with-doctest file.py
-
-    >>> a = { 'first' : { 'all_rows' : { 'pass' : 'dog', 'number' : '1' } } }
-    >>> b = { 'first' : { 'all_rows' : { 'fail' : 'cat', 'number' : '5' } } }
-    >>> deep_merge_dictionaries(b, a) == { 'first' : { 'all_rows' : { 'pass' : 'dog', 'fail' : 'cat', 'number' : '5' } } }
-    True
-    """
-    for key, value in source.items():
-        if isinstance(value, dict):
-            # get node or create one
-            node = destination.setdefault(key, {})
-            deep_merge_dictionaries(value, node)
-        else:
-            destination[key] = value
-
+from collections import OrderedDict
+import pandas as pd
+
+
+def recursive_walk(od_field: OrderedDict):
+    """
+    Recursively flattens each row the results of simple salesforce.
+    Only works for bottom up queries.
+    :param od_field: results returned by simple salesforce (multiple objects)
+    :return: returns a flattened list of dictionaries
+    """
+    d = {}
+    for k in od_field.keys():
+        if isinstance(od_field[k], OrderedDict) & (k != 'attributes'):
+            if 'attributes' in od_field[k].keys():
+                ret_df = recursive_walk(od_field[k])
+                d = {**d, **ret_df}
+            else:
+                obj = od_field['attributes']['type'].replace(" ", ".")
+                d[f'{obj}.{k}'] = ",\n".join([   f'{k}: {v}' for k, v in od_field[k].items() if v is not None])
+        else:
+            if k != 'attributes':
+                obj = od_field['attributes']['type'].replace(" ", ".")
+                d[f'{obj}.{k}'] = od_field[k]
+    return d
+
+def transform_sf_result_set_rec(query_results: OrderedDict):
+    """
+    Recursively flattens the results of simple salesforce. It needs flattening when  selecting
+    multiple objects.
+    :param query_results:
+    :return:
+    """
+    data = []
+    for res in query_results:
+        d = recursive_walk(res)
+        data.append(d)
+    data = pd.DataFrame(data)
+    return data
+
+def deep_merge_dictionaries(source, destination):
+    """
+    run me with nosetests --with-doctest file.py
+
+    >>> a = { 'first' : { 'all_rows' : { 'pass' : 'dog', 'number' : '1' } } }
+    >>> b = { 'first' : { 'all_rows' : { 'fail' : 'cat', 'number' : '5' } } }
+    >>> deep_merge_dictionaries(b, a) == { 'first' : { 'all_rows' : { 'pass' : 'dog', 'fail' : 'cat', 'number' : '5' } } }
+    True
+    """
+    for key, value in source.items():
+        if isinstance(value, dict):
+            # get node or create one
+            node = destination.setdefault(key, {})
+            deep_merge_dictionaries(value, node)
+        else:
+            destination[key] = value
+
     return destination
```

### Comparing `veevatools-0.0.95/setup.cfg` & `veevatools-0.0.96/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2076 6565 7661 746f 6f6c 730d 0a76   = veevatools..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e39 350d  ersion = 0.0.95.
-00000030: 0a64 6573 6372 6970 7469 6f6e 203d 2056  .description = V
-00000040: 6565 7661 2074 6f6f 6c73 206c 6962 7261  eeva tools libra
-00000050: 7279 2066 6f72 2061 6363 656c 6572 6174  ry for accelerat
-00000060: 696e 6720 5665 6576 6120 5379 7374 656d  ing Veeva System
-00000070: 7320 496e 7465 726e 616c 2054 6f6f 6c73  s Internal Tools
-00000080: 2064 6576 656c 6f70 6d65 6e74 0d0a 6175   development..au
-00000090: 7468 6f72 203d 204d 6963 6861 656c 2050  thor = Michael P
-000000a0: 6179 0d0a 6175 7468 6f72 5f65 6d61 696c  ay..author_email
-000000b0: 203d 206d 6f6e 6963 6b65 6e69 7368 4067   = monickenish@g
-000000c0: 6d61 696c 2e63 6f6d 0d0a 7572 6c20 3d20  mail.com..url = 
-000000d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000000e0: 6f6d 2f6d 6963 6861 656c 7061 790d 0a6c  om/michaelpay..l
-000000f0: 6963 656e 7365 5f66 696c 6573 203d 204c  icense_files = L
-00000100: 4943 454e 5345 2e74 7874 0d0a 6c6f 6e67  ICENSE.txt..long
-00000110: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
-00000120: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
-00000130: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-00000140: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
-00000150: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a0d  text/markdown...
-00000160: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
-00000170: 6167 6573 203d 2066 696e 643a 0d0a 696e  ages = find:..in
-00000180: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
-00000190: 200d 0a09 7061 6e64 6173 3e3d 312e 332e   ...pandas>=1.3.
-000001a0: 300d 0a09 7369 6d70 6c65 2d73 616c 6573  0...simple-sales
-000001b0: 666f 7263 653e 3d31 2e31 312e 360d 0a09  force>=1.11.6...
-000001c0: 7361 6c65 7366 6f72 6365 2d62 756c 6b3e  salesforce-bulk>
-000001d0: 3d32 2e32 2e30 0d0a 0973 6664 636c 6962  =2.2.0...sfdclib
-000001e0: 3e3d 302e 322e 3236 0d0a 096f 7065 6e70  >=0.2.26...openp
-000001f0: 7978 6c3d 3d33 2e30 2e39 0d0a 097a 6565  yxl==3.0.9...zee
-00000200: 703d 3d34 2e31 2e30 0d0a 0961 696f 7369  p==4.1.0...aiosi
-00000210: 676e 616c 3d3d 312e 322e 300d 0a09 7a65  gnal==1.2.0...ze
-00000220: 6570 3d3d 342e 312e 300d 0a0d 0a5b 6f70  ep==4.1.0....[op
-00000230: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-00000240: 696e 645d 0d0a 6578 636c 7564 6520 3d20  ind]..exclude = 
-00000250: 7465 7374 730d 0a0d 0a5b 6f70 7469 6f6e  tests....[option
-00000260: 732e 6578 636c 7564 655f 7061 636b 6167  s.exclude_packag
-00000270: 655f 6461 7461 5d0d 0a76 6565 7661 746f  e_data]..veevato
-00000280: 6f6c 7320 3d20 0d0a 0963 7265 6465 6e74  ols = ...credent
-00000290: 6961 6c73 2e6a 736f 6e0d 0a0d 0a5b 6f70  ials.json....[op
-000002a0: 7469 6f6e 732e 7061 636b 6167 655f 6461  tions.package_da
-000002b0: 7461 5d0d 0a76 6565 7661 6e65 7477 6f72  ta]..veevanetwor
-000002c0: 6b20 3d20 0d0a 092a 2e6a 736f 6e0d 0a0d  k = ...*.json...
-000002d0: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-000002e0: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-000002f0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 7665 6576 6174 6f6f 6c73 0a76 6572  = veevatools.ver
+00000020: 7369 6f6e 203d 2030 2e30 2e39 360a 6465  sion = 0.0.96.de
+00000030: 7363 7269 7074 696f 6e20 3d20 5665 6576  scription = Veev
+00000040: 6120 746f 6f6c 7320 6c69 6272 6172 7920  a tools library 
+00000050: 666f 7220 6163 6365 6c65 7261 7469 6e67  for accelerating
+00000060: 2056 6565 7661 2053 7973 7465 6d73 2049   Veeva Systems I
+00000070: 6e74 6572 6e61 6c20 546f 6f6c 7320 6465  nternal Tools de
+00000080: 7665 6c6f 706d 656e 740a 6175 7468 6f72  velopment.author
+00000090: 203d 204d 6963 6861 656c 2050 6179 0a61   = Michael Pay.a
+000000a0: 7574 686f 725f 656d 6169 6c20 3d20 6d6f  uthor_email = mo
+000000b0: 6e69 636b 656e 6973 6840 676d 6169 6c2e  nickenish@gmail.
+000000c0: 636f 6d0a 7572 6c20 3d20 6874 7470 733a  com.url = https:
+000000d0: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 6963  //github.com/mic
+000000e0: 6861 656c 7061 790a 6c69 6365 6e73 655f  haelpay.license_
+000000f0: 6669 6c65 7320 3d20 4c49 4345 4e53 452e  files = LICENSE.
+00000100: 7478 740a 6c6f 6e67 5f64 6573 6372 6970  txt.long_descrip
+00000110: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
+00000120: 444d 452e 6d64 0a6c 6f6e 675f 6465 7363  DME.md.long_desc
+00000130: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
+00000140: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
+00000150: 646f 776e 0a0a 5b6f 7074 696f 6e73 5d0a  down..[options].
+00000160: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
+00000170: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
+00000180: 7320 3d20 0a09 7061 6e64 6173 3e3d 312e  s = ..pandas>=1.
+00000190: 332e 300a 0973 696d 706c 652d 7361 6c65  3.0..simple-sale
+000001a0: 7366 6f72 6365 3e3d 312e 3131 2e36 0a09  sforce>=1.11.6..
+000001b0: 7361 6c65 7366 6f72 6365 2d62 756c 6b3e  salesforce-bulk>
+000001c0: 3d32 2e32 2e30 0a09 7366 6463 6c69 623e  =2.2.0..sfdclib>
+000001d0: 3d30 2e32 2e32 360a 096f 7065 6e70 7978  =0.2.26..openpyx
+000001e0: 6c3d 3d33 2e30 2e39 0a09 7a65 6570 3d3d  l==3.0.9..zeep==
+000001f0: 342e 312e 300a 0961 696f 7369 676e 616c  4.1.0..aiosignal
+00000200: 3d3d 312e 322e 300a 097a 6565 703d 3d34  ==1.2.0..zeep==4
+00000210: 2e31 2e30 0a09 6169 6f68 7474 703d 3d33  .1.0..aiohttp==3
+00000220: 2e38 2e31 0a09 7079 6172 726f 773d 3d38  .8.1..pyarrow==8
+00000230: 2e30 2e30 0a0a 5b6f 7074 696f 6e73 2e70  .0.0..[options.p
+00000240: 6163 6b61 6765 732e 6669 6e64 5d0a 6578  ackages.find].ex
+00000250: 636c 7564 6520 3d20 7465 7374 730a 0a5b  clude = tests..[
+00000260: 6f70 7469 6f6e 732e 6578 636c 7564 655f  options.exclude_
+00000270: 7061 636b 6167 655f 6461 7461 5d0a 7665  package_data].ve
+00000280: 6576 6174 6f6f 6c73 203d 200a 0963 7265  evatools = ..cre
+00000290: 6465 6e74 6961 6c73 2e6a 736f 6e0a 0a5b  dentials.json..[
+000002a0: 6f70 7469 6f6e 732e 7061 636b 6167 655f  options.package_
+000002b0: 6461 7461 5d0a 7665 6576 616e 6574 776f  data].veevanetwo
+000002c0: 726b 203d 200a 092a 2e6a 736f 6e0a 0a5b  rk = ..*.json..[
+000002d0: 6567 675f 696e 666f 5d0a 7461 675f 6275  egg_info].tag_bu
+000002e0: 696c 6420 3d20 0a74 6167 5f64 6174 6520  ild = .tag_date 
+000002f0: 3d20 300a 0a                             = 0..
```

### Comparing `veevatools-0.0.95/veevanetwork/custom_exceptions/veevanetwork_exceptions.py` & `veevatools-0.0.96/veevanetwork/custom_exceptions/veevanetwork_exceptions.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-class NetworkAPIHeaderValueNotFound(Exception):
-    """Exception raised when the required values are not provided to the
-    Vn.api_call() method.
-
-    Expecting to find a api['request']['header'][key]['value'] attribute in the json/dict provided, 
-    where 'key' represents Authorization or Content Type header.
-    """
-
-    def __init__(self, message="The defined API does not contain a value parameter in its header.\
-Expecting to find a api['request']['header'][key]['value'] attribute in the json/dict provided, \
-where 'key' represents Authorization or Content Type header."):
-        self.message = message
-        super().__init__(self.message)
-
-class NetworkAPIRequestMethodNotFound(Exception):
-    """Exception raised when the required values are not provided to the
-    Vn.api_call() method.
-
-    Required Values:
-        Expecting to find a api['request']['method'] attribute in the json/dict provided.
-    """
-
-    def __init__(self, message="The defined API does not contain a method parameter in its request method.\
-Expecting to find a api['request']['method'] attribute in the json/dict provided."):
-        self.message = message
-        super().__init__(self.message)
-
-class NetworkAPIRequestURLNotFound(Exception):
-    """Exception raised when the required values are not provided to the
-    Vn.api_call() method.
-
-    Required Values:
-        Expecting to find a api['request']['url']['raw'] attribute in the json/dict provided.
-    """
-
-    def __init__(self, message="The defined API does not contain a method parameter in its request method.\
-Expecting to find a api['request']['url']['raw'] attribute in the json/dict provided."):
-        self.message = message
-        super().__init__(self.message)
-
-class NetworkAPIRequestBodyNotFound(Exception):
-    """Exception raised when the required values are not provided to the
-    Vn.api_call() method.
-
-    Required Values:
-        The parameter body: dict is required in this API call, please refer to the Network API documentation for the syntax of the body parameter or set the if_example parameter to True for an example.
-    """
-
-    def __init__(self, message="The parameter body: dict is is required in this API call, please refer to the Network API documentation for the syntax of the body parameter or set the if_example parameter to True for an example."):
-        self.message = message
-        super().__init__(self.message)
-
-class NetworkAPIRequestVariableNotFound(Exception):
-    """Exception raised when the required values are not provided to the
-    Vn.api_call() method.
-
-    Required Values:
-        The parameter variables: dict is required in this API call, please refer to the Network API documentation for the syntax of the body parameter or set the if_example parameter to True for an example.
-    """
-
-    def __init__(self, message="The parameter variables: dict is required in this API call, please refer to the Network API documentation for the syntax of the body parameter or set the if_example parameter to True for an example."):
-        self.message = message
-        super().__init__(self.message)
-
-class NetworkAPIRequestQueryNotFound(Exception):
-    """Exception raised when the required values are not provided to the
-    Vn.api_call() method.
-
-    Required Values:
-        The parameter queries: dict is required in this API call, please refer to the Network API documentation for the syntax of the body parameter or set the if_example parameter to True for an example.
-    """
-
-    def __init__(self, message="The parameter queries: dict is required in this API call, please refer to the Network API documentation for the syntax of the body parameter or set the if_example parameter to True for an example."):
-        self.message = message
-        super().__init__(self.message)
-
-
+class NetworkAPIHeaderValueNotFound(Exception):
+    """Exception raised when the required values are not provided to the
+    Vn.api_call() method.
+
+    Expecting to find a api['request']['header'][key]['value'] attribute in the json/dict provided, 
+    where 'key' represents Authorization or Content Type header.
+    """
+
+    def __init__(self, message="The defined API does not contain a value parameter in its header.\
+Expecting to find a api['request']['header'][key]['value'] attribute in the json/dict provided, \
+where 'key' represents Authorization or Content Type header."):
+        self.message = message
+        super().__init__(self.message)
+
+class NetworkAPIRequestMethodNotFound(Exception):
+    """Exception raised when the required values are not provided to the
+    Vn.api_call() method.
+
+    Required Values:
+        Expecting to find a api['request']['method'] attribute in the json/dict provided.
+    """
+
+    def __init__(self, message="The defined API does not contain a method parameter in its request method.\
+Expecting to find a api['request']['method'] attribute in the json/dict provided."):
+        self.message = message
+        super().__init__(self.message)
+
+class NetworkAPIRequestURLNotFound(Exception):
+    """Exception raised when the required values are not provided to the
+    Vn.api_call() method.
+
+    Required Values:
+        Expecting to find a api['request']['url']['raw'] attribute in the json/dict provided.
+    """
+
+    def __init__(self, message="The defined API does not contain a method parameter in its request method.\
+Expecting to find a api['request']['url']['raw'] attribute in the json/dict provided."):
+        self.message = message
+        super().__init__(self.message)
+
+class NetworkAPIRequestBodyNotFound(Exception):
+    """Exception raised when the required values are not provided to the
+    Vn.api_call() method.
+
+    Required Values:
+        The parameter body: dict is required in this API call, please refer to the Network API documentation for the syntax of the body parameter or set the if_example parameter to True for an example.
+    """
+
+    def __init__(self, message="The parameter body: dict is is required in this API call, please refer to the Network API documentation for the syntax of the body parameter or set the if_example parameter to True for an example."):
+        self.message = message
+        super().__init__(self.message)
+
+class NetworkAPIRequestVariableNotFound(Exception):
+    """Exception raised when the required values are not provided to the
+    Vn.api_call() method.
+
+    Required Values:
+        The parameter variables: dict is required in this API call, please refer to the Network API documentation for the syntax of the body parameter or set the if_example parameter to True for an example.
+    """
+
+    def __init__(self, message="The parameter variables: dict is required in this API call, please refer to the Network API documentation for the syntax of the body parameter or set the if_example parameter to True for an example."):
+        self.message = message
+        super().__init__(self.message)
+
+class NetworkAPIRequestQueryNotFound(Exception):
+    """Exception raised when the required values are not provided to the
+    Vn.api_call() method.
+
+    Required Values:
+        The parameter queries: dict is required in this API call, please refer to the Network API documentation for the syntax of the body parameter or set the if_example parameter to True for an example.
+    """
+
+    def __init__(self, message="The parameter queries: dict is required in this API call, please refer to the Network API documentation for the syntax of the body parameter or set the if_example parameter to True for an example."):
+        self.message = message
+        super().__init__(self.message)
+
+
```

### Comparing `veevatools-0.0.95/veevanetwork/network_api_v25.json` & `veevatools-0.0.96/veevanetwork/network_api_v25.json`

 * *Files identical despite different names*

### Comparing `veevatools-0.0.95/veevanetwork/veevanetwork.py` & `veevatools-0.0.96/veevanetwork/veevanetwork.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,1559 +1,1559 @@
-from sys import platform
-import requests
-import pandas as pd
-import os
-import json
-from typing import List, Tuple, Optional, Union, Type, OrderedDict, Iterable
-import numpy as np
-import sys
-import importlib.resources
-from urllib.parse import urlparse
-try:
-    from custom_exceptions.veevanetwork_exceptions import *
-except:
-    from veevanetwork.custom_exceptions.veevanetwork_exceptions import *
-
-class Vn:
-    def __init__(self):
-        self.os_platform: str = platform
-        self.networkURL: str = None # https://verteonetwork.veevanetwork.com
-        self.networkUserName: str = None
-        self.networkPassword: str = None
-        self.networkCountry: str = 'US'
-        self.networkConnection: requests.models.Response = None
-        self.networkLanguages: list = None # List of languages supported by this instance of Veeva Network
-        self.networkObjects: dict = None # Dictionary of Network Objects and their properties
-        self.networkObjectMetadata: dict = None # {'HCP': {'my_custom_field__c': {'fieldId': 'my_custom_field__c','type': {'dataType': 'STRING', 'discriminator': None}, 'labels': {'en': 'My Custom Field'}}}}
-        self.networkReferenceTypes: dict = None # {'AddressAdminArea': {'type': 'AddressAdminArea','customerOwned': False,'inactive': False,'description': 'AddressAdminArea'}, 'AddressCBSA': {'type': 'AddressCBSA' ... }}
-        self.networkReferenceValueMetadata: dict = None # Dictionary of Network Reference Value Metadata, including countries, reference codes, translated values, etc.
-        self.sessionId: str = None
-        self.networkId: str = None
-        self.APIheaders: dict = None
-        self.APIversionList: list = []
-        self.LatestAPIversion: str = None
-        self.network_references_all: pd.DataFrame = None
-        self.network_DNS: str = None # verteonetwork.veevanetwork.com
-        self.network_protocol: str = None # https
-
-        #----------------------------------------------------------------
-        # Load Network API Json
-        self.network_api_json: dict = None
-        try: # Try to load the network API json, to be used in a packaged distribution context
-            with importlib.resources.open_text("veevanetwork", "network_api_v25.json") as file:
-                self.network_api_json = json.load(file)
-        except: # If the above fails, try to load the network API json, to be used in a development context
-            with open('network_api_v25.json', encoding="utf-8") as file:
-                self.network_api_json = json.load(file)
-        self.network_api_parsed: dict = self.__parse_network_api_json(self.network_api_json)
-        self.api_categories: list = list(self.network_api_parsed['item'].keys())
-
-        self.api_change_request = self.network_api_parsed['item']['Change Request']
-        self.api_custom_key = self.network_api_parsed['item']['Custom Key']
-        self.api_entity = self.network_api_parsed['item']['Entity']
-        self.api_hco = self.network_api_parsed['item']['HCO']
-        self.api_hcp = self.network_api_parsed['item']['HCP']
-        self.api_metadata = self.network_api_parsed['item']['Metadata']
-        self.api_subscriptions = self.network_api_parsed['item']['Subscriptions']
-        self.api_subscriptions_compliance = self.network_api_parsed['item']['Subscriptions - Compliance']
-        self.api_subscriptions_source = self.network_api_parsed['item']['Subscriptions - Source']
-        self.api_subscriptions_target = self.network_api_parsed['item']['Subscriptions - Target']
-        self.api_events = self.network_api_parsed['item']['Events']
-        self.api_match = self.network_api_parsed['item']['Match']
-        self.api_suspect_match = self.network_api_parsed['item']['Suspect Match']
-        self.api_authentication = self.network_api_parsed['item']['Authentication']
-        self.api_retrieve_available_api_versions = self.network_api_parsed['item']['Retrieve Available API Versions']
-        self.api_search = self.network_api_parsed['item']['Search']
-        self.call = {
-            "Change Request": {
-                "change_request_create": self.change_request_create,
-                "change_request_cancel": self.change_request_cancel,
-                "change_request_retrieve": self.change_request_retrieve,
-                "change_request_batch_retrieve": self.change_request_batch_retrieve,
-                "change_request_update": self.change_request_update,
-                "change_request_batch_update": self.change_request_batch_update,
-                "change_request_process": self.change_request_process,
-                "change_request_batch_process": self.change_request_batch_process,
-                "change_request_search": self.change_request_search,
-                "change_request_match": self.change_request_match,
-                "change_request_batch_approve": self.change_request_batch_approve,
-                "change_request_batch_reject": self.change_request_batch_reject
-            },
-            "Custom Key": {
-                "custom_key_associate_to_entity": self.custom_key_associate_to_entity,
-                "custom_key_associate_to_child": self.custom_key_associate_to_child,
-                "custom_key_batch_associate_to_entities": self.custom_key_batch_associate_to_entities,
-                "custom_key_batch_associate_to_children": self.custom_key_batch_associate_to_children,
-                "custom_key_disassociate": self.custom_key_disassociate,
-                "custom_key_batch_disassociate": self.custom_key_batch_disassociate
-            },
-            "Entity": {
-                "entity_retrieve": self.entity_retrieve,
-                "entity_retrieve_child": self.entity_retrieve_child,
-                "entity_batch_retrieve": self.entity_batch_retrieve,
-                "entity_batch_retrieve_children": self.entity_batch_retrieve_children
-            },
-            "HCO": {
-                "hco_retrieve": self.hco_retrieve,
-                "hco_associate_custom_key": self.hco_associate_custom_key,
-                "hco_address_associate_custom_key": self.hco_address_associate_custom_key,
-                "hco_license_associate_custom_key": self.hco_license_associate_custom_key,
-                "hco_parenthco_associate_custom_key": self.hco_parenthco_associate_custom_key
-            },
-            "HCP": {
-                "hcp_retrive": self.hcp_retrive,
-                "hcp_associate_custom_key": self.hcp_associate_custom_key,
-                "hcp_address_associate_custom_key": self.hcp_address_associate_custom_key,
-                "hcp_license_associate_custom_key": self.hcp_license_associate_custom_key,
-                "hcp_parenthco_associate_custom_key": self.hcp_parenthco_associate_custom_key
-            },
-            "Metadata": {
-                "metadata_retrieve_available_api_versions": self.metadata_retrieve_available_api_versions,
-                "metadata_retrieve_hashtags": self.metadata_retrieve_hashtags,
-                "metadata_retrieve_object_types": self.metadata_retrieve_object_types,
-                "metadata_retrieve_field": self.metadata_retrieve_field,
-                "metadata_retrieve_field_details": self.metadata_retrieve_field_details,
-                "metadata_retrieve_field_groups": self.metadata_retrieve_field_groups,
-                "metadata_retrieve_reference_data_types": self.metadata_retrieve_reference_data_types,
-                "metadata_retrieve_reference_data_type_details": self.metadata_retrieve_reference_data_type_details,
-                "metadata_retrieve_reference_data_type_code_details": self.metadata_retrieve_reference_data_type_code_details
-            },
-            "Subscriptions": {
-                "subscriptions_create_job": self.subscriptions_create_job,
-                "subscriptions_retrieve_job": self.subscriptions_retrieve_job,
-                "subscriptions_cancel_job": self.subscriptions_cancel_job,
-                "subscriptions_retrieve_export_job_file": self.subscriptions_retrieve_export_job_file
-            },
-            "Subscriptions - Compliance": {
-                "subscriptions_compliance_create_job": self.subscriptions_compliance_create_job,
-                "subscriptions_compliance_retrieve_job": self.subscriptions_compliance_retrieve_job,
-                "subscriptions_compliance_cancel_job": self.subscriptions_compliance_cancel_job
-            },
-            "Subscriptions - Source": {
-                "subscriptions_source_create_job": self.subscriptions_source_create_job,
-                "subscriptions_source_retrieve_job": self.subscriptions_source_retrieve_job,
-                "subscriptions_source_cancel_job": self.subscriptions_source_cancel_job
-            },
-            "Subscriptions - Target": {
-                "subscriptions_target_create_job": self.subscriptions_target_create_job,
-                "subscriptions_target_retrieve_job": self.subscriptions_target_retrieve_job,
-                "subscriptions_target_cancel_job": self.subscriptions_target_cancel_job
-            },
-            "Events": {
-                "events_retrieve_merge": self.events_retrieve_merge,
-                "events_retrieve_unmerge": self.events_retrieve_unmerge
-            },
-            "Match": {
-                "match_retrieve": self.match_retrieve,
-                "suspect_match_batch_reject_task": self.suspect_match_batch_reject_task,
-
-            },
-            "Suspect Match": {
-                "suspect_match_batch_process": self.suspect_match_batch_process,
-                "suspect_match_batch_create": self.suspect_match_batch_create,
-                "suspect_match_batch_reject_task": self.suspect_match_batch_reject_task,
-                "suspect_match_batch_retrieve": self.suspect_match_batch_retrieve
-            },
-            "Retrieve Available API Versions": {
-                "retrieve_available_api_versions": self.retrieve_available_api_versions
-            },
-            "Search": {
-                "search": self.search
-            }
-            }
-    
-    # =============================================================================
-    # Authentication
-    # =============================================================================
-
-    # Refactored - MP 20220610
-    def authenticate(
-        self, 
-        networkURL: str=None, 
-        networkUserName: str=None, 
-        networkPassword: str=None, 
-        networkCountry: str=None, 
-        networkId: str=None,
-        sessionId: str=None,
-        if_return: bool=False, 
-        *args, **kwargs
-    ) -> Optional[dict]:
-        """
-        Authenticates Veeva Network and retrieves the auth token.
-
-        Example:
-        authenticate using unpacked kwargs from the retrieve_credentials function
-            authenticate_vn(**retrieve_credentials(platform, 'credentials.xlsx')[0])
-
-        Return Example:
-            {'sf': <simple_salesforce.api.Salesforce at 0x24a045c7b50>,
-             'bulk': <salesforce_bulk.salesforce_bulk.SalesforceBulk at 0x24a045c7e20>,
-             'sfMeta': <sfdclib.session.SfdcSession at 0x24a044b3400>,
-             'tooling': <sfdclib.tooling.SfdcToolingApi at 0x24a045d17f0>,
-             'session_id': '00D3F000000FZCq!AQYAQHYfSLYGI9cTyjDfxAAzYm.1uOKmNPXlKMW0sVz5ilIQ9ZwVTh6kOlaRuqfPuuzNnZNb3461sUGeUZ57ttE.GBawbt5h',
-             'instance': 'cslbehring-core--devr01.my.salesforce.com',
-             'sfMeta_is_connected': True,
-             'bulk_api_sessionId': '00D3F000000FZCq!AQYAQHYfSLYGI9cTyjDfxAAzYm.1uOKmNPXlKMW0sVz5ilIQ9ZwVTh6kOlaRuqfPuuzNnZNb3461sUGeUZ57ttE.GBawbt5h'}
-
-        Dependencies:
-            import requests
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Authenticate
-        
-        """
-        if (networkId and sessionId and networkURL):
-            self.networkId = self.networkId if networkId is None else networkId
-            self.sessionId = self.sessionId if sessionId is None else sessionId
-        
-        url_parse = urlparse(networkURL)
-        if len(url_parse.scheme) == 0:
-            self.network_protocol = 'https'
-            if len(url_parse.path) > 0:
-                self.network_DNS = url_parse.path
-                self.networkURL = self.network_protocol + '://' + url_parse.path
-
-        if len(url_parse.scheme) > 0:
-            self.network_protocol = url_parse.scheme
-            if len(url_parse.netloc) > 0:
-                self.network_DNS = url_parse.netloc
-                self.networkURL = url_parse.scheme + '://' + url_parse.netloc
-
-        if (self.networkURL is None) or (len(self.networkURL) == 0):
-            raise Exception('networkURL is required')
-
-
-        # self.networkURL = self.networkURL if networkURL is None else networkURL
-        self.networkUserName = self.networkUserName if networkUserName is None else networkUserName
-        self.networkPassword = self.networkPassword if networkPassword is None else networkPassword
-        self.networkCountry = self.networkCountry if networkCountry is None else networkCountry
-        
-        if (self.networkUserName and self.networkPassword and self.networkURL):
-            self.networkConnection = requests.post(self.networkURL + '/api/v17.0/auth?username=' + self.networkUserName + '&password=' + self.networkPassword)
-            if (self.networkConnection.json()['responseStatus'] == 'SUCCESS'):
-                self.sessionId = self.networkConnection.json()['sessionId']
-                self.userId = self.networkConnection.json()['userId']
-                self.networkId = self.networkConnection.json()['networkId']
-            else:
-                raise Exception(self.networkConnection.json())
-
-        
-        self.APIheaders = {'authorization': self.sessionId}
-        self.APIversionList = []
-        
-        # Error checking whether the required parameters are passed in
-        # The check happens here because this is where all the self assignments has completed
-        if (not (self.networkId and self.sessionId and self.networkURL)) and (not (self.networkUserName and self.networkPassword and self.networkCountry and self.networkURL)):
-            raise Exception("Please provide either networkId, sessionId, and networkURL or networkUserName, networkPassword, and networkURL")
-        
-        for API in requests.get(self.networkURL +'/api', headers=self.APIheaders).json()['values'].keys():
-            self.APIversionList.append(float(API.replace("v", "")))
-        self.APIversionList.sort()
-        self.LatestAPIversion = "v" + str(self.APIversionList[-1])
-        
-
-        if if_return:
-            return {'networkURL':self.networkURL, 
-                    'networkUserName':self.networkUserName, 
-                    'networkPassword':self.networkPassword, 
-                    'networkConnection':self.networkConnection, 
-                    'sessionId':self.sessionId, 
-                    'APIheaders':self.APIheaders, 
-                    'APIversionList':self.APIversionList, 
-                    'LatestAPIversion':self.LatestAPIversion}    
-
-    # Refactored - MP 20220610
-    def get_networkObjects(self) -> pd.DataFrame:
-        """
-        Returns a list of all objects in the Veeva Network.
-        """
-        self.authenticate()
-
-        self.networkObjects = self.list_of_dicts_to_dict(requests.get(self.networkURL + '/api/' + self.LatestAPIversion + '/metadata/objectTypes',
-                                      headers=self.APIheaders).json()['objectTypes'], 'name')
-        return self.networkObjects
-
-    # Refactored - MP 20220610
-    def get_networkObjectMetadata(self) -> pd.DataFrame:
-        self.authenticate()
-        if self.networkObjects is None:
-            self.get_networkObjects()
-
-        processing_dict = {}
-        __empty =[
-            processing_dict.update({networkObject: 
-                self.list_of_dicts_to_dict(requests.get(
-                        self.networkURL + 
-                        '/api/'+ self.LatestAPIversion +
-                        '/metadata/fields?objectTypes=' + 
-                        networkObject + '&details=full' + 
-                        '&countries='+ self.networkCountry, 
-                        headers=self.APIheaders).json()['attributes'],
-                        'fieldId')}) 
-                        for networkObject in self.networkObjects.keys()]
-        self.networkObjectMetadata = processing_dict
-        return self.networkObjectMetadata
-
-
-    # Refactored - MP 20220612
-    def process_networkReferenceCodeMetadata(
-        self,
-        referenceTypes: Optional[list] = None, # List of reference types to retrieve, leave empty (None) to retrieve all
-        customerOwned: Optional[bool] = None, # True (customer owned only), False (ootb), None (customer owned and ootb)
-        activeReferences: Optional[bool]= None, # True (active only), False (inactive only), None (active and inactive)
-        languages: Optional[list]= None, # List of languages to retrieve, leave empty (None) to retrieve all
-        countries: Optional[list]= None, # List of countries to retrieve, leave empty (None) to retrieve all
-    ):
-        """
-        Processes Network Reference Metadata and returns a DataFrame of the reference codes based on the parameters.
-
-        Parameters:
-        referenceTypes: List of reference types to retrieve, leave empty (None) to retrieve all
-        customerOwned (bool): Filter references by customerOwned status. Values: True (customerOwned only), False (ootb only), None (customerOwned and ootb)
-        activeReferences (bool): Filter references by status. Values: True (active only), False (inactive only), None (active and inactive)
-        languages (list): List of languages to return. Default: ['en']
-        countries (list): List of countries to return. Default: ['US']
-
-        Returns:
-        DataFrame: A DataFrame of the reference codes based on the parameters.
-        """
-
-        if self.networkReferenceValueMetadata is None:
-            self.get_networkReferenceValueMetadata()
-        
-        if languages is None:
-            if self.networkLanguages is None:
-                self.get_networkLanguages()
-            languages = self.networkLanguages
-            
-        networkReferenceDF = pd.DataFrame(self.networkReferenceValueMetadata)
-        networkReferenceCodeDataframe = networkReferenceDF.loc['reference_type_codes', :].dropna()
-        reference_code_dict_unfiltered: dict[str, pd.DataFrame] = {}
-        for index, values in zip(networkReferenceCodeDataframe.index, networkReferenceCodeDataframe.values):
-            reference_code_dict_unfiltered.update({index: pd.DataFrame(self.list_of_dicts_to_dict(values, 'code'))})
-        
-        final_df = pd.DataFrame()
-        for reference_type, reference_dataframe in zip(reference_code_dict_unfiltered.keys(), reference_code_dict_unfiltered.values()):
-            if referenceTypes is None or reference_type in referenceTypes:
-                activeReferences = None
-                customerOwned = None
-                activeReferences_filter = [True,False] if activeReferences is None else [not(activeReferences)]
-                customerOwned_filter = [True,False] if customerOwned is None else [customerOwned]
-                reference_dataframe = reference_dataframe.T.copy()
-                filtered_customerOwned_and_active = reference_dataframe[
-                                                (reference_dataframe['customerOwned'].isin(customerOwned_filter)) & 
-                                                (reference_dataframe['inactive'].isin(activeReferences_filter))
-                                                ]
-
-                filtered_languages = pd.DataFrame()
-
-                for language in languages:
-                    filtered_languages = pd.concat([filtered_languages,
-                                                pd.DataFrame(
-                                                    filtered_customerOwned_and_active["values"]
-                                                    .apply(lambda value: value[language] 
-                                                    if value.keys()
-                                                    .__contains__(language) 
-                                                    else np.nan)
-                                                    .dropna()
-                                                    .rename(language))], axis=1)
-                filtered_languages.insert(0, 'Network Code', filtered_languages.index)
-                filtered_languages.insert(1, 'Reference Type', reference_type)
-                filtered_languages.insert(2, 'Active Countries', pd.DataFrame(filtered_customerOwned_and_active["countries"]
-                                                    .apply(lambda value: ";".join(sorted(value)) if (countries is None or len(set(value).intersection(set(countries)))>0 ) else np.nan).rename('countries')
-                                                )['countries'])
-                filtered_languages.insert(3, 'Definition', pd.DataFrame(
-                                                    filtered_customerOwned_and_active["values"]
-                                                    .apply(lambda value: value['en'] 
-                                                    if value.keys()
-                                                    .__contains__('en') 
-                                                    else np.nan)
-                                                    .dropna()
-                                                    .rename('en'))['en'])
-                filtered_languages.insert(4, 'Active?', filtered_customerOwned_and_active["inactive"] == False)
-                filtered_languages.insert(5, 'Veeva Maintained?', filtered_customerOwned_and_active["customerOwned"] == False)             
-                filtered_languages.reset_index(drop=True, inplace=True)
-                filtered_languages.dropna(subset=['Active Countries'], inplace=True)
-                filtered_languages.replace(np.nan, "", inplace=True)
-                filtered_languages
-                final_df = pd.concat([final_df, filtered_languages], axis=0)
-
-        final_df.reset_index(drop=True, inplace=True)
-        
-        return final_df
-
-    # To be deprecated, used by object_metadata_dataframe()
-    def object_metadata(self):
-        self.networkObjects = requests.get(self.networkURL + '/api/' + self.LatestAPIversion + '/metadata/objectTypes',
-                                      headers=self.APIheaders).json()['objectTypes']
-        networkObjectList = []
-        for obj in self.networkObjects:
-            if obj['status'] == 'ACTIVE':
-                networkObjectList.append(obj['name'])
-            else:
-                pass
-        object_metadata = pd.DataFrame([requests.get(self.networkURL + '/api/'+ self.LatestAPIversion +'/metadata/fields?objectTypes=' + networkObject + '&details=full' + '&countries='+ self.networkCountry, headers=self.APIheaders).json()['attributes'] 
-                                              for networkObject in networkObjectList])
-        object_metadata = object_metadata.transpose()
-        object_metadata.columns = networkObjectList
-        return object_metadata
-
-    # To be deprecated, use get_networkObjectMetadata() instead
-    def object_metadata_dataframe(self, object_metadata = None, attribute = None, *args):
-        """
-        Function that takes an input of data table with metadata values containing field for each row and objects for each column, 
-        lists of input attributes available in the meta data (i.e. ['type','dataType']), 
-        and optional arguments containing comma separated lists of additional attributes available in the meta data 
-        
-        Example:
-            VeevaNetwork.object_metadata_dataframe(self.object_metadata(), ['fieldId'], ['type','dataType'], ['type','discriminator'], ['labels','en'],['maximumLength'])
-            
-        Return Example:
-        (Dataframe)
-            HCP.fieldId    HCP.type.dataType    HCP.type.discriminator    HCP.labels.en    HCP.maximumLength    HCO.fieldId      ...
-            hcp_type__v    REFERENCE            HCPType                   HCP Type         100.0                340B_eligible__v ...
-        
-        """
-        self.authenticate()
-        
-        object_metadata = self.object_metadata() if object_metadata is None else object_metadata
-        
-        object_metadata_dataframe = pd.DataFrame()
-        attribute1 = attribute[0]
-        attribute2 = attribute[1] if len(attribute) > 1 else ""
-        for networkObjectName, networkObjectMetaData in object_metadata.iteritems():
-            attributeList = []
-            for fieldMetaData in networkObjectMetaData:
-                try:
-                    if attribute2 == "":
-                        attributeList.append(fieldMetaData[attribute1])
-                    else:
-                        attributeList.append(fieldMetaData[attribute1][attribute2])
-                except TypeError:
-                    continue
-    #        object_metadata_dataframe[networkObjectName + '.' + attribute1 + (("." + attribute2) if attribute2 != "" else "")] = pd.Series(attributeList, name = networkObjectName)
-            object_metadata_dataframe = pd.concat([object_metadata_dataframe,pd.Series(attributeList, name = networkObjectName + '.' + attribute1 + (("." + attribute2) if attribute2 != "" else "")).to_frame()], ignore_index=False, axis=1)
-
-
-            # parse arguments
-            if args:
-                for arg in args:
-                    argAttribute1 = arg[0]
-                    argAttribute2 = arg[1] if len(arg)>1 else ""
-                    argAttributeList = []
-                    for fieldMetaData in networkObjectMetaData:
-                        try:
-                            if argAttribute2 == "":
-                                argAttributeList.append(fieldMetaData[argAttribute1])
-                            else:
-                                argAttributeList.append(fieldMetaData[argAttribute1][argAttribute2])
-                        except:
-                            argAttributeList.append("")
-                            continue
-    #                object_metadata_dataframe[networkObjectName + '.' + argAttribute1 + (("." + argAttribute2) if argAttribute2 != "" else "")] = pd.Series(argAttributeList, name = networkObjectName)
-                    object_metadata_dataframe = pd.concat([object_metadata_dataframe,pd.Series(argAttributeList, name = networkObjectName + '.' + argAttribute1 + (("." + argAttribute2) if argAttribute2 != "" else "")).to_frame()], ignore_index=False, axis=1)
-            else:
-                continue
-        return object_metadata_dataframe
-
-    # Refactored - MP 20220611
-    def get_networkReferenceValueMetadata(self):
-        """
-        Retruns a Dictionary of Network Reference Value Metadata, including countries, reference codes, translated values, etc.
-        """
-        self.authenticate()
-        self.networkReferenceValueMetadata = self.list_of_dicts_to_dict(requests.get(self.networkURL + '/api/' + self.LatestAPIversion + '/metadata/reference_values?includeCodes=True', headers = self.APIheaders).json()['reference_type_values'],'type')
-        return self.networkReferenceValueMetadata
-
-    # Deprecated
-    def reference_value_dataframe(self):
-        """
-        Retrieve all reference values in Network  
-        ** formula can be enhanced or take input parameters so it doesn't query every single reference alias
-
-        """
-        self.authenticate()
-
-        self.networkReferenceTypes = self.list_of_dicts_to_dict(requests.get(self.networkURL + '/api/' + self.LatestAPIversion + '/metadata/reference_values?includeCodes=True', headers = self.APIheaders).json()['reference_type_values'],'type')
-        reference_value_dataframe = pd.DataFrame()
-        for x in self.networkReferenceTypes.keys():
-            try:
-                referenceCall = requests.get(self.networkURL + '/api/'+ self.LatestAPIversion + '/metadata/reference_values/' + x + '?countries='+ self.networkCountry, headers = self.APIheaders).json()['reference_type_codes']
-                newColumn = pd.Series([x['values']['en'] for x in referenceCall],name = str(x) + " Value")
-                
-                newColumn2 = pd.Series([x['code'] for x in referenceCall], name = x)
-                reference_value_dataframe.insert(len(reference_value_dataframe.columns), column = x, value = newColumn2)
-                reference_value_dataframe.insert(len(reference_value_dataframe.columns), column = str(x) + " Value", value = newColumn)
-            except:
-                pass
-        return reference_value_dataframe
-
-    def extract_network_reference_table(self):
-        self.authenticate()
-        
-        references_all = pd.DataFrame(requests.get(self.networkURL + '/api/'+ self.LatestAPIversion + '/metadata/reference_values?includeCodes=true&countries='+ self.networkCountry, headers = self.APIheaders).json()['reference_type_values'])
-        network_reference_table = pd.DataFrame()
-        self.network_references_all = references_all
-        for row in references_all['reference_type_codes']:
-            if isinstance(row, list):
-                network_reference_table = pd.concat([network_reference_table, pd.json_normalize(row)], axis=1)
-            else:
-                continue
-        network_reference_table.fillna('',inplace=True)
-        return network_reference_table
-    
-    # =============================================================================
-    # WIP Functions
-    # =============================================================================
-
-
-    # =============================================================================
-    # Change Request
-    # =============================================================================
-
-    def change_request_create(self, *args, **kwargs):
-        """
-        This API enables you to create a Network change request to add or update an HCP or HCO and related entities (including addresses, licenses, or parentHCOs) for **gray** data only.
-
-        Change requests created using the API against orange data will be rejected.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Createachangerequest
-
-        """
-        
-        return self.api_call(self.api_change_request['item']['Create Change Request'], *args, **kwargs)
-        
-    def change_request_cancel(self, *args, **kwargs):
-        """
-        This API enables you to cancel a change request by providing the change request ID.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Cancelchangerequest
-
-        """
-        return self.api_call(self.api_change_request['item']['Cancel Change Request'], *args, **kwargs)
-
-    def change_request_retrieve(self, *args, **kwargs):
-        """
-        This API enables you to retrieve response information for the create, update, and merge change requests submitted by a client application.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#RetrieveChangeRequest
-
-        """
-        return self.api_call(self.api_change_request['item']['Retrieve Change Request'], *args, **kwargs)
-        
-    def change_request_batch_retrieve(self, *args, **kwargs):
-        """
-        This API enables you to obtain information about multiple change requests through the API.
-
-        Documenatation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Batchretrievechangerequest  
-
-        """
-        return self.api_call(self.api_change_request['item']['Change Request Batch Retrieve'], *args, **kwargs)
-        
-    def change_request_update(self, *args, **kwargs):
-        """
-        This API enables you to update an unprocessed change request through the API.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#UpdateChangeRequest
-
-        """
-        return self.api_call(self.api_change_request['item']['Change Request Update'], *args, **kwargs)
-
-    def change_request_batch_update(self, *args, **kwargs):
-        """
-        This API enables you to update multiple unprocessed change requests.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#BatchUpdateChangeRequests
-
-        """
-        return self.api_call(self.api_change_request['item']['Change Request Batch Update'], *args, **kwargs)
-
-    def change_request_process(self, *args, **kwargs):
-        """
-        This API enables you to process an unprocessed change request through the API.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#ProcessChangeRequest
-
-        """
-        return self.api_call(self.api_change_request['item']['Change Request Process'], *args, **kwargs)
-
-    def change_request_batch_process(self, *args, **kwargs):
-        """
-        This API enables you to process multiple unprocessed change requests.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#BatchProcessChangeRequests
-        """
-        return self.api_call(self.api_change_request['item']['Change Request Batch Process'], *args, **kwargs)
-
-    def change_request_search(self, *args, **kwargs):
-        """
-        This API enables you to retrieve all change requests that match a specified search criteria.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#ChangeRequestSearch
-
-        """
-        return self.api_call(self.api_change_request['item']['Change Request Search'], *args, **kwargs)
-
-    def change_request_match(self, *args, **kwargs):
-        """
-        This API enables you to match a request to an existing entity. You can use either the Veeva ID or custom key of an existing entity to match the request against.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#ChangeRequestMatch
-
-        """
-        return self.api_call(self.api_change_request['item']['Change Request Match'], *args, **kwargs)
-
-    def change_request_batch_approve(self, *args, **kwargs):
-        """
-        This API enables you to bulk approve up to 500 change requests.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#BatchApproveChangeRequests
-
-        """
-        return self.api_call(self.api_change_request['item']['Change Request Batch Approve'], *args, **kwargs)
-
-    def change_request_batch_reject(self, *args, **kwargs):
-        """
-        This API enables you to bulk reject up to 500 change requests.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#BatchRejectChangeRequests
-
-        """
-        return self.api_call(self.api_change_request['item']['Change Request Batch Reject'], *args, **kwargs)
-    
-    # =============================================================================
-    # Custom Key
-    # =============================================================================
-
-    def custom_key_associate_to_entity (self, *args, **kwargs):
-        """
-        This API enables you to submit external key identifiers when new HCPs or HCOs are downloaded from Network without going through the full change request process.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Associatecustomkeytoentity
-
-        """
-        return self.api_call(self.api_custom_key['item']['Associate Custom Key to Entity'], *args, **kwargs)
-
-    def custom_key_associate_to_child (self, *args, **kwargs):
-        """
-        This API enables you to submit external key identifiers when new children (address, license, or parent HCOs) are downloaded from Network without going through the full change request process.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Associatecustomkeytochildren
-
-        """
-        return self.api_call(self.api_custom_key['item']['Associate Custom Key to Children'], *args, **kwargs)
-
-    def custom_key_batch_associate_to_entities (self, *args, **kwargs):
-        """
-        This API enables you to submit external key identifiers whenever new HCPs or HCOs are downloaded from Network without going through the full change request process.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Batchassociatecustomkeystoentities
-
-        """
-        return self.api_call(self.api_custom_key['item']['Batch Associate Custom Keys to Entities'], *args, **kwargs)
-
-    def custom_key_batch_associate_to_children (self, *args, **kwargs):
-        """
-        This API enables you to submit external key identifiers when new children (address, license, or parent HCOs) are downloaded from Network without going through the full change request process.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Batchassociatecustomkeytochildren
-
-        """
-        return self.api_call(self.api_custom_key['item']['Batch Associate Custom Keys to Children'], *args, **kwargs)
-
-    def custom_key_disassociate (self, *args, **kwargs):
-        """
-        This API enables you to deactivate external key identifiers for any entity (an HCP, HCO, Address, License, or ParentHCO) in Network without going through the full change request process.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Disassociatecustomkey
-
-        """
-        return self.api_call(self.api_custom_key['item']['Disassociate Custom Key'], *args, **kwargs)
-
-    def custom_key_batch_disassociate (self, *args, **kwargs):
-        """
-        This API enables you to inactivate external key identifiers for any entity (HCP, HCO, Address, License, or ParentHCO) in Network without going through the full change request process.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Batchdisassociatecustomkey
-
-        """
-        return self.api_call(self.api_custom_key['item']['Batch Disassociate Custom Key'], *args, **kwargs)
-
-
-    # =============================================================================
-    # Entity
-    # =============================================================================
-
-    def entity_retrieve (self, *args, **kwargs):
-        """
-        This API enables you to obtain information on any entity without identifying the specific entity type. It is only used to retrieve information from Network using the GET method.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrieveentity
-
-        """
-        return self.api_call(self.api_entity['item']['Retrieve Entity'], *args, **kwargs)
-
-    def entity_retrieve_child (self, *args, **kwargs):
-        """
-        This API enables you to retrieve child entity information; for example address or license details, for the Network ID provided without identifying the specific entity type.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrievechildentity
-
-        """
-        return self.api_call(self.api_entity['item']['Retrieve Child Entity'], *args, **kwargs)
-
-    def entity_batch_retrieve (self, *args, **kwargs):
-        """
-        This API enables you to retrieve entity details directly from Network. It is only used to retrieve information using the GET method. To update or delete entity data, you must use the change request APIs.
-
-        The entities you can retrieve include HCPs and HCOs, and details are returned for all corresponding child entities: addresses, licenses, parent HCOs, and custom keys.
-        
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Batchretrieveentities
-
-        """
-        return self.api_call(self.api_entity['item']['Batch Retrieve Entities'], *args, **kwargs)
-
-    def entity_batch_retrieve_children (self, *args, **kwargs):
-        """
-        This API enables you to obtain information on child entities without identifying the specific entity type. Users are only allowed to retrieve (GET) information from Network.
-
-        All other operations (POST and DELETE) are restricted and can only be performed by submitting a change request using the change request APIs.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Batchretrievechildentities
-
-        """
-        return self.api_call(self.api_entity['item']['Batch Retrieve Child Entities'], *args, **kwargs)
-
-
-    # =============================================================================
-    # HCO
-    # =============================================================================
-
-    def hco_retrieve (self, *args, **kwargs):
-        """
-        This API enables you to retrieve information about an HCO. Information you can retrieve for an HCO includes the HCO, address, license, and parent HCO information (including their custom keys) for the HCO vid_key you provide.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#RetrieveHCO
-
-        """
-        return self.api_call(self.api_hco['item']['Retrieve HCO'], *args, **kwargs)
-
-    def hco_associate_custom_key (self, *args, **kwargs):
-        """
-        This API enables you to submit external key identifiers when new HCOs are downloaded from Network without going through the full change request process. This API associates the external identifier you submit to the HCO vid_key you provide.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#AssociatecustomkeytoHCO
-
-        """
-        return self.api_call(self.api_hco['item']['Associate Custom Key to HCO'], *args, **kwargs)
-
-    def hco_address_associate_custom_key (self, *args, **kwargs):
-        """
-        This API enables you to submit external key identifiers when new HCO child objects (addresses) 
-        are downloaded from Network without going through the full change request process. 
-        This API associates the external identifier you submit to the child object key you provide.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Associatecustomkeytoachildobject
-
-        """
-        return self.api_call(self.api_hco['item']['Associate Custom Key to HCO Address'], *args, **kwargs)
-
-    def hco_license_associate_custom_key (self, *args, **kwargs):
-        """
-        This API enables you to submit external key identifiers when new HCO child objects (licenses) 
-        are downloaded from Network without going through the full change request process. 
-        This API associates the external identifier you submit to the child object key you provide.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Associatecustomkeytoachildobject
-
-        """
-        return self.api_call(self.api_hco['item']['Associate Custom Key to HCO License'], *args, **kwargs)
-
-    def hco_parenthco_associate_custom_key (self, *args, **kwargs):
-        """
-        This API enables you to submit external key identifiers when new HCO child objects (parent HCOs) 
-        are downloaded from Network without going through the full change request process. 
-        This API associates the external identifier you submit to the child object key you provide.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Associatecustomkeytoachildobject
-
-        """
-        return self.api_call(self.api_hco['item']['Associate Custom Key to HCO ParentHCO'], *args, **kwargs)
-
-    # =============================================================================
-    # HCP
-    # =============================================================================
-    def hcp_retrive (self, *args, **kwargs):
-        """
-        This API enables you to retrieve information about an HCP including the HCP itself, address, license, and parent HCO information (including their custom keys) for the HCP vid_key you provide.
-
-        This API downloads the record for the specified entity from Veeva OpenData to your customer instance.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#RetrieveHCP
-
-        """
-        return self.api_call(self.api_hcp['item']['Retrieve HCP'], *args, **kwargs)
-
-    def hcp_associate_custom_key (self, *args, **kwargs):
-        """
-        This API enables you to submit external key identifiers when new HCPs are downloaded from Network without going through the full change request process. This API associates the external identifier you submit to the HCP vid_key you provide.
-
-        This API requires system administrator or API-only permissions.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#AssociatecustomkeytoHCP
-
-        """
-        return self.api_call(self.api_hcp['item']['Associate Custom Key to HCP'], *args, **kwargs)
-
-    def hcp_address_associate_custom_key (self, *args, **kwargs):
-        """
-        This API enables you to submit external key identifiers when new HCP child objects (addresses) are downloaded from Network without going through the full change request process. This API associates the external identifier you submit to the child object key you provide.
-
-        This API requires system administrator or API-only permissions.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Associatecustomkeytoachildobject1
-
-        """
-        return self.api_call(self.api_hcp['item']['Associate Custom Key to HCP Address'], *args, **kwargs)
-
-    def hcp_license_associate_custom_key (self, *args, **kwargs):
-        """
-        This API enables you to submit external key identifiers when new HCP child objects (licenses) are downloaded from Network without going through the full change request process. This API associates the external identifier you submit to the child object key you provide.
-
-        This API requires system administrator or API-only permissions.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Associatecustomkeytoachildobject1
-        
-        """
-        return self.api_call(self.api_hcp['item']['Associate Custom Key to HCP License'], *args, **kwargs)
-
-    def hcp_parenthco_associate_custom_key (self, *args, **kwargs):
-        """
-        This API enables you to submit external key identifiers when new HCP child objects (parent HCOs) are downloaded from Network without going through the full change request process. This API associates the external identifier you submit to the child object key you provide.
-
-        This API requires system administrator or API-only permissions.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Associatecustomkeytoachildobject1
-        
-        """
-        return self.api_call(self.api_hcp['item']['Associate Custom Key to HCP ParentHCO'], *args, **kwargs)
-
-    # =============================================================================
-    # Metadata
-    # =============================================================================
-    def metadata_retrieve_available_api_versions (self, *args, **kwargs):
-        """
-        This enables you to retrieve summary information about each API version available in Network.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#RetrieveavailableAPIversions
-        
-        """
-        return self.api_call(self.api_metadata['item']['Retrieve Available API Versions'], *args, **kwargs)
-        
-    def metadata_retrieve_hashtags (self, *args, **kwargs):
-        """
-        This API enables you to retrieve the list of hashtags available in a Network instance.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrievehashtags
-
-        """
-        return self.api_call(self.api_metadata['item']['Retrieve hashtags'], *args, **kwargs)
-
-    # TODO: rename/refactor method.
-    def get_networkLanguages(self) -> list:
-        """
-        This API enables you to retrieve the list of reference data languages available in a Network instance.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrievelanguages
-
-        """
-
-        self.authenticate()
-        self.networkLanguages = list(self.list_of_dicts_to_dict(
-            requests.get(
-                self.networkURL + 
-                '/api/' + 
-                self.LatestAPIversion + 
-                '/metadata/languages', 
-                headers=self.APIheaders).json()['languages'], 
-                'name'
-                ).keys())
-        return self.networkLanguages
-
-    def metadata_retrieve_object_types (self, *args, **kwargs):
-        """
-        This API enables you to retrieve the list of object types available in Network.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrieveobjecttypesmetadata
-
-        """
-        return self.api_call(self.api_metadata['item']['Retrieve Object Types Metadata'], *args, **kwargs)
-
-    def metadata_retrieve_field (self, *args, **kwargs):
-        """
-        This API enables you to retrieve detailed or summary information about the fields on each entity in Network.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrievefieldsmetadata
-
-        """
-        return self.api_call(self.api_metadata['item']['Retrieve Fields Metadata'], *args, **kwargs)
-
-    def metadata_retrieve_field_details (self, *args, **kwargs):
-        """
-        This API enables you to retrieve detailed information about the fields on each entity in Network.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrievefielddetailsmetadata
-
-        """
-        return self.api_call(self.api_metadata['item']['Retrieve Field Details Metadata'], *args, **kwargs)
-
-    def metadata_retrieve_field_groups (self, *args, **kwargs):
-        """
-        This API enables you to retrieve detailed information about the field groups available in Network. These field groups are used by the CRM bridge when retrieving and displaying information from Network in CRM.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrievefieldgroupsmetadata
-
-        """
-        return self.api_call(self.api_metadata['item']['Retrieve Field Groups Metadata'], *args, **kwargs)
-
-    def metadata_retrieve_reference_data_types (self, *args, **kwargs):
-        """
-        This API enables you to retrieve information about reference data types in Network.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrievereferencedatatypesmetadata
-
-        """
-        return self.api_call(self.api_metadata['item']['Retrieve Reference Data Types Metadata'], *args, **kwargs)
-
-    def metadata_retrieve_reference_data_type_details (self, *args, **kwargs):
-        """
-        This API enables you to retrieve detailed information about reference data types in Network.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrievereferencedatatypedetailsmetadata
-
-        """
-        return self.api_call(self.api_metadata['item']['Retrieve Reference Data Type Details Metadata'], *args, **kwargs)
-
-    def metadata_retrieve_reference_data_type_code_details (self, *args, **kwargs):
-        """
-        This API enables you to retrieve detailed information about reference data type codes in Network.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrievereferencedatatypecodedetailsmetadata
-
-        """
-        return self.api_call(self.api_metadata['item']['Retrieve Reference Data Type Code Details Metadata'], *args, **kwargs)
-
-    # =============================================================================
-    # Subscriptions
-    # =============================================================================
-    def subscriptions_create_job (self, *args, **kwargs):
-        """
-        This API enables you to create a subscription job.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Createasubscriptionjob
-
-        """
-        return self.api_call(self.api_subscriptions['item']['Create Subscription Job'], *args, **kwargs)
-
-    def subscriptions_retrieve_job (self, *args, **kwargs):
-        """
-        This API enables you to retrieve the status of a source or target subscription job.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrieveasubscriptionjobstatus
-
-        """
-        return self.api_call(self.api_subscriptions['item']['Retrieve Subscription Job'], *args, **kwargs)
-
-    def subscriptions_cancel_job (self, *args, **kwargs):
-        """
-        This API enables you to cancel a subscription job.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Cancelasubscriptionjob
-
-        """
-        return self.api_call(self.api_subscriptions['item']['Cancel Subscription Job'], *args, **kwargs)
-
-    def subscriptions_retrieve_export_job_file (self, *args, **kwargs):
-        """
-        This API enables you to retrieve the artifacts (file contents) of a target subscription job.
-        AKA: Retrieve target subscription artifact
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrievetargetsubscriptionartifact
-        
-        """
-        return self.api_call(self.api_subscriptions['item']['Retrieve Export Job File'], *args, **kwargs)
-
-    # =============================================================================
-    # Subscriptions - Compliance
-    # =============================================================================
-    def subscriptions_compliance_create_job (self, *args, **kwargs):
-        """
-        This API enables you to create a compliance subscription job.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Createacompliancesubscriptionjob
-
-        """
-        return self.api_call(self.api_subscriptions_compliance['item']['Create Compiance Subscription Job'], *args, **kwargs)
-
-    def subscriptions_compliance_retrieve_job (self, *args, **kwargs):
-        """
-        This API enables you to retrieve the status of a source or target subscription job.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrieveacompliancesubscriptionjobstatus
-        
-        """
-        return self.api_call(self.api_subscriptions_compliance['item']['Retrieve Compliance Subscription Job'], *args, **kwargs)
-
-    def subscriptions_compliance_cancel_job (self, *args, **kwargs):
-        """
-        This API enables you to cancel a compliance subscription job.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Cancelacompliancesubscriptionjob
-
-        """
-        return self.api_call(self.api_subscriptions_compliance['item']['Cancel Compliance Subscription Job'], *args, **kwargs)
-
-    # =============================================================================
-    # Subscriptions - Source
-    # =============================================================================
-    def subscriptions_source_create_job (self, *args, **kwargs):
-        """
-        This API enables you to create a source subscription job.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Createasourcesubscriptionjob
-
-        """
-        return self.api_call(self.api_subscriptions_source['item']['Create Source Subscription Job'], *args, **kwargs)
-
-    def subscriptions_source_retrieve_job (self, *args, **kwargs):
-        """
-        This API enables you to retrieve the status of a source subscription job.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrieveasourcesubscriptionjobstatus
-
-        """
-        return self.api_call(self.api_subscriptions_source['item']['Retrieve Source Subscription Job'], *args, **kwargs)
-
-    def subscriptions_source_cancel_job (self, *args, **kwargs):
-        """
-        This API enables you to cancel a source subscription job.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Cancelasourcesubscriptionjob
-        
-        """
-        return self.api_call(self.api_subscriptions_source['item']['Cancel Source Subscription Job'], *args, **kwargs)
-
-    # =============================================================================
-    # Subscriptions - Target
-    # =============================================================================
-    def subscriptions_target_create_job (self, *args, **kwargs):
-        """
-        This API enables you to create a target subscription job.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Createatargetsubscriptionjob
-
-        """
-        return self.api_call(self.api_subscriptions_target['item']['Create Target Subscription Job'], *args, **kwargs)
-
-    def subscriptions_target_retrieve_job (self, *args, **kwargs):
-        """
-        This API enables you to retrieve the status of a source or target subscription job.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrieveatargetsubscriptionjobstatus
-
-        """
-        return self.api_call(self.api_subscriptions_target['item']['Retrieve Target Subscription Job'], *args, **kwargs)
-
-    def subscriptions_target_cancel_job (self, *args, **kwargs):
-        """
-        This API enables you to cancel a target subscription job.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Cancelatargetsubscriptionjob
-        """
-        return self.api_call(self.api_subscriptions_target['item']['Cancel Target Subscription Job'], *args, **kwargs)
-
-    # =============================================================================
-    # Events
-    # =============================================================================
-    def events_retrieve_merge (self, *args, **kwargs):
-        """
-        This API enables you to retrieve the results of merge events that occurred in your Network instance.
-
-        Merges initiated by Veeva OpenData on a master instance are included if the surviving and losing records of the merge have been downloaded to your instance.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#RetrieveMerges
-
-        """
-        return self.api_call(self.api_events['item']['Retrieve Merge Events'], *args, **kwargs)
-
-    def events_retrieve_unmerge (self, *args, **kwargs):
-        """
-        This API enables you to retrieve the results of unmerge events that occurred in your Network instance.
-
-        Unmerges include events that occurred in your Network instance; only customer (gray) records are reported.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#RetrieveUnmerges
-
-        """
-        return self.api_call(self.api_events['item']['Retrieve Unmerge Events'], *args, **kwargs)
-
-    # =============================================================================
-    # Match
-    # =============================================================================
-    def match_retrieve (self, *args, **kwargs):
-        """
-        This API enables you to match data immediately for a single record using match rules from the specified Network instance.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#RetrieveMatches
-
-        """
-        return self.api_call(self.api_match['item']['Retrieve Matches'], *args, **kwargs)
-
-    # =============================================================================
-    # Suspect Match
-    # =============================================================================
-    def suspect_match_batch_process (self, *args, **kwargs):
-        """
-        This API enables enables you to process multiple unprocessed suspect matches.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#BatchProcessSuspectMatch
-
-        """
-        return self.api_call(self.api_suspect_match['item']['Batch Process Suspect Match'], *args, **kwargs)
-
-    def suspect_match_batch_create (self, *args, **kwargs):
-        """
-        This API enables enables you to create multiple suspect matches.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#BatchCreateSuspectMatch
-
-        """
-        return self.api_call(self.api_suspect_match['item']['Batch Create Suspect Match'], *args, **kwargs)
-
-    def suspect_match_batch_reject_task (self, *args, **kwargs):
-        """
-        This API enables enables you to reject multiple suspect match tasks.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#BatchRejectSuspectMatch
-
-        """
-        return self.api_call(self.api_suspect_match['item']['Batch Reject Suspect Match Task'], *args, **kwargs)
-
-    def suspect_match_batch_retrieve (self, *args, **kwargs):
-        """
-        This API enables enables you to retrieve information about multiple suspect matches.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#BatchRetrieveSuspectMatch
-
-        """
-        self.api_call(suspect_match['item']['Batch Retrieve Suspect Match'], *args, **kwargs)
-
-    # =============================================================================
-    # Retrieve Available API Versions
-    # =============================================================================
-    def retrieve_available_api_versions (self, *args, **kwargs):
-        """
-        This enables you to retrieve summary information about each API version available in Network.
-
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#RetrieveavailableAPIversions
-
-        """
-        return self.api_call(self.api_retrieve_available_api_versions, *args, **kwargs)
-    # =============================================================================
-    # Search
-    # =============================================================================
-    def search (self, *args, **kwargs):
-        """
-        Search calls enable you to construct simple, yet powerful searches to retrieve data from Network.
-
-        Calls through the Search API pass a query string in an expression that specifies the search text and specific parameters to get the intended set of entities from Network. Search results are ranked according to closeness to the search terms specified.
-        
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#search
-        
-        """
-        return self.api_call(self.api_search, *args, **kwargs)
-    # =============================================================================
-    # System Settings
-    # =============================================================================
-    def system_settings_retrieve (self):
-        """
-        This API enables you to retrieve the value for the geolocation system setting.
-
-        Currently only api.search.geolocation.countries is supported.
-        
-        Documentation:
-        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrievesystemsettings
-        
-        """
-        result = requests.get(
-            url=f"{self.networkURL}/api/v26.0/systemSettings/api.search.geolocation.countries", 
-            headers=self.APIheaders).json()
-        return result
-        
-
-    # =============================================================================
-    # Utilities
-    # =============================================================================
-
-    def api_call (
-        self,
-        api: dict, 
-        body: dict = None, 
-        variables: dict = None, 
-        queries: dict = None, 
-        if_print: bool=False,  # If True, prints each component of the api call, the api call will still execute unless if_debug or if_example paramters are set to True.
-        if_debug: bool=False, # If True, the api call does not execute, but instead returns the api call as a string for debugging
-        if_example: bool=False # If True, the api call does not execute and returns examples of any body, variables, or queries.
-    ):
-
-        examples = {}
-
-        result = {
-            'api_body' : body,
-            'api_variables' : variables,
-            'api_queries' : queries
-        }
-
-        request_params = {}
-
-        def print_if(text):
-            if if_print:
-                print(text)
-
-        if api.keys().__contains__('name'):
-            print_if('\n- Name: ')
-            print_if(api['name'])
-            result['api_name'] = api['name'] ### Updating Result Name
-
-        if api.keys().__contains__('protocolProfileBehavior'):
-            print_if('\n- protocolProfileBehavior: ')
-            if api['protocolProfileBehavior'].keys().__contains__('disableBodyPruning'):
-                print_if('- disableBodyPruning: ')
-                print_if(api['protocolProfileBehavior']['disableBodyPruning'])
-                result['api_protocolProfileBehavior_disableBodyPruning'] = api['protocolProfileBehavior']['disableBodyPruning'] ### Updating Result disableBodyPruning
-
-        if api.keys().__contains__('request'):
-
-            ### =============================================================================
-            ### Parsing Header
-            ### =============================================================================
-
-            if api['request'].keys().__contains__('header'):
-                if isinstance(api['request']['header'], dict):
-                    print_if("\n- Request header keys: ")
-                    print_if(api['request']['header'].keys())
-                    result['api_header'] = {}
-                    request_params['headers'] = {}
-                    for header_key, header_value in api['request']['header'].items():
-                        print_if("\n- Request header key:")
-                        print_if(header_key)
-                        if isinstance(header_value, dict):
-                            if header_value.keys().__contains__('value'):
-                                result['api_header'].update({header_key: self.sub_request_params(api['request']['header'][header_key]['value'])}) ### Updating Result API Header
-                                request_params['headers'].update({header_key: self.sub_request_params(api['request']['header'][header_key]['value'])}) ### Updating Request Header
-
-                            for key, value in header_value.items():
-                                print_if("\n- Request header value dict key and value:")
-                                print_if(key)
-                                print_if(value)
-                        else:
-                            print_if("Request Header Value: ")
-                            print_if(header_value)
-                            raise NetworkAPIHeaderValueNotFound
-
-            ### =============================================================================
-            ### Parsing Method
-            ### =============================================================================
-
-            if api['request'].keys().__contains__('method'):
-                print_if("\n- Request method: ")
-                print_if(api['request']['method'])
-
-                match api['request']['method']:
-                    case 'POST':
-                        result['api_method'] = requests.post # Updating Result Method
-                        print_if("\n- Request Method Post:")
-                        print_if("requests.post")
-                    case 'GET':
-                        result['api_method'] = requests.get # Updating Result Method
-                        print_if("\n- Request Method Get:")
-                        print_if("requests.get")
-                    case 'PUT':
-                        result['api_method'] = requests.put # Updating Result Method
-                        print_if("\n- Request Method Put:")
-                        print_if("requests.put")
-                    case 'DELETE':
-                        result['api_method'] = requests.delete # Updating Result Method
-                        print_if("\n- Request Method Delete:")
-                        print_if("requests.delete")
-                    case _:
-                        print_if("\n- Request Method Unknown:")
-                        print_if("unknown method")
-                        raise NetworkAPIRequestMethodNotFound
-
-            ### =============================================================================
-            ### Parsing Body
-            ### =============================================================================
-
-            if (api['request'].keys().__contains__('body') == True) and \
-                (api['request']['body'].keys().__contains__('raw') == True) and \
-                (api['request']['body']['raw'] != ''):
-                print_if("\n- Request body raw: ")
-                print_if(json.loads(api['request']['body']['raw']))
-                examples['body'] = json.loads(api['request']['body']['raw']) ### Updating Result API Body
-                # If the body parameter is not provided in an API call that requires a body. Raise Error.
-                if body is None and if_example==False:
-                    raise NetworkAPIRequestBodyNotFound
-                else:
-                    request_params['data']=json.dumps(body)
-            else:
-                print_if("\n- Request body raw: ")
-                print_if("No Body Found")
-            
-            ### =============================================================================
-            ### Parsing URL
-            ### =============================================================================
-
-            if api['request'].keys().__contains__('url'):
-                print_if("\n- Request url keys: ")
-                print_if(api['request']['url'].keys())
-
-                ### =============================================================================
-                ### Parsing Raw URL
-                ### =============================================================================
-
-                if api['request']['url'].keys().__contains__('raw'):
-                    print_if("\n- Request url raw: ")
-                    print_if(api['request']['url']['raw'])
-                    result['api_url'] = self.sub_request_params(api['request']['url']['protocol'] + "://" + api['request']['url']['host'][0] + "/" + "/".join(api['request']['url']['path'])) ### Updating Result API URL
-                    request_params['url'] = self.sub_request_params(api['request']['url']['protocol'] + "://" + api['request']['url']['host'][0] + "/" + "/".join(api['request']['url']['path'])) ### Updating Request URL
-                else:
-                    raise NetworkAPIRequestURLNotFound
-
-                
-                ### =============================================================================
-                ### Parsing URL Protocol
-                ### =============================================================================
-                
-                if api['request']['url'].keys().__contains__('protocol'):
-                    print_if("\n- Request url protocol: ")
-                    # always "https"
-                    print_if(api['request']['url']['protocol'])
-
-                ### =============================================================================
-                ### Parsing URL Host
-                ### =============================================================================
-                
-                if api['request']['url'].keys().__contains__('host'):
-                    print_if("\n- Request url host: ")
-                    # always ['{{DNS}}]
-                    print_if(api['request']['url']['host'][0])
-
-                ### =============================================================================
-                ### Parsing URL Path
-                ### =============================================================================
-
-                if api['request']['url'].keys().__contains__('path'):
-                    print_if("\n- Request url path: ")
-                    # A list of path components. i.e. ['api', '{{version}}', 'hcos', ':vid_key', 'addresses', ':address_key', 'custom_keys']
-                    print_if(api['request']['url']['path'])
-
-                ### =============================================================================
-                ### Parsing URL Variable
-                ### =============================================================================
-
-                if api['request']['url'].keys().__contains__('variable'):
-                    if variables is None and if_example==False:
-                        raise NetworkAPIRequestVariableNotFound
-                    elif if_example==False:
-                        for variable in variables.keys():
-                            result['api_url'] = result['api_url'].replace(":" + variable, variables[variable]['value'])
-                            request_params['url'] = request_params['url'].replace(":" + variable, variables[variable]['value'])
-
-                    if isinstance(api['request']['url']['variable'], dict):
-                        print_if("\n- Request url variable keys: ")
-                        print_if(api['request']['url']['variable'].keys())
-                        variables: dict = api['request']['url']['variable']
-                        examples['variables'] = variables ### Updating Result API URL Variable Examples
-                        
-                        for key, value in variables.items():
-                            if isinstance(value, dict):
-                                print_if("\n- Request url variable key and value dict: ")
-                                print_if(key)
-                                print_if(value)
-                            else:
-                                print_if("\n- Request url variable value: ") 
-                                print_if(str(value))
-
-                ### =============================================================================
-                ### Parsing URL Query
-                ### =============================================================================
-
-                if api['request']['url'].keys().__contains__('query'):
-                    if queries is None and if_example==False:
-                        raise NetworkAPIRequestQueryNotFound
-                    elif if_example==False:
-                        result['api_url'] = result['api_url'] + '?'
-                        request_params['url'] = request_params['url'] + '?'
-                        for key, value in queries.items():
-                            if result['api_url'][-1] == '?':
-                                result['api_url'] = result['api_url'] + key + '=' + value['value']
-                                request_params['url'] = request_params['url'] + key + '=' + value['value']
-                            else:
-                                result['api_url'] = result['api_url'] + '&' + key + '=' + value['value']
-                                request_params['url'] = request_params['url'] + '&' + key + '=' + value['value']
-
-                    print_if("\n- Request url query keys: ")
-                    print_if(api['request']['url']['query'].keys())
-                    queries: dict = api['request']['url']['query'] 
-                    examples['query'] = queries ### Updating Result API URL Query Examples
-                    for key, value in queries.items():
-                        print_if("\n- Request url query key and value: ")
-                        if isinstance(value, dict):
-                            print_if(key)
-                            print_if(value)
-                        else:
-                            print_if(str(value))
-
-            ### =============================================================================
-            ### Parsing Description
-            ### =============================================================================
-
-            if api['request'].keys().__contains__('description'):
-                print_if("\n- Request Description: ")
-                print_if(api['request']['description'])
-                examples['description'] = api['request']['description'] ### Updating Description
-
-        if api.keys().__contains__('response'):
-            print_if(api['response'])
-
-        if (not if_debug) & (not if_example) & (result.keys().__contains__('api_method')):
-            response = result['api_method'](**request_params)
-
-        if if_debug & if_example:
-            return result, examples, request_params
-        if if_debug:
-            return result, request_params
-        if if_example:
-            return examples
-        return response
-
-
-    @staticmethod
-    def list_of_dicts_to_dict(list_of_dict: list, key) -> dict:
-        """
-        Function takes a list of dicts and returns a single dict.
-
-        Parameters:
-        list_of_dict: list of dicts, i.e. [{'key1': 'value1', 'key2': 'value2'}, {'key1': 'value1', 'key2': 'value2'}]
-        key (str): key to use for the dict. i.e. 'key1'
-            in our example, [{'key1': 'value1', 'key2': 'value2'}, {'key1': 'value1', 'key2': 'value2'}]
-            The output dictionary would have value1, value2 as the keys:
-            {'value1': {'key1': 'value1', 'key2': 'value2'}, 'value2': {'key1': 'value1', 'key2': 'value2'}}
-
-        """
-        obj_dict = {}
-        __empty = [obj_dict.update({x[key]: x}) for x in list_of_dict]
-        return obj_dict
-
-    @staticmethod
-    def cartesian_join(pd1, pd2):
-        df1 = pd1.copy()
-        df2 = pd2.copy()
-        df1.reset_index()
-        df2.reset_index()
-        df1['cartesian_join_key'] = 1
-        df2['cartesian_join_key'] = 1
-        result = pd.merge(df1, df2, on ='cartesian_join_key').drop(labels="cartesian_join_key", axis=1)
-        return result
-        
-    def sub_request_params (self, request: str) -> str:
-        substitutions_dict = {
-            '{{AUTHORIZATION}}': self.APIheaders['authorization'],
-            '{{DNS}}': self.network_DNS,
-            '{{version}}': self.LatestAPIversion
-        }
-        for key, value in substitutions_dict.items():
-            request = request.replace(key, value)
-        return request
-    
-    def __parse_network_api_json(self, network_api: dict):
-        output = {}
-        for key, value in network_api.items():
-            if isinstance(value, dict):
-                output[key] = self.__parse_network_api_json(value)
-            elif isinstance(value, list):
-                first_key_set = set()
-                for item in value:
-                    if isinstance(item, dict):
-                        first_key_set.add(list(item.keys())[0])
-                if len(first_key_set) == 1:
-                    output[key] = self.__parse_network_api_json(self.list_of_dicts_to_dict(value, list(first_key_set)[0]))
-                else:
-                    output[key] = value
-            else:
-                output[key] = value
+from sys import platform
+import requests
+import pandas as pd
+import os
+import json
+from typing import List, Tuple, Optional, Union, Type, OrderedDict, Iterable
+import numpy as np
+import sys
+import importlib.resources
+from urllib.parse import urlparse
+try:
+    from custom_exceptions.veevanetwork_exceptions import *
+except:
+    from veevanetwork.custom_exceptions.veevanetwork_exceptions import *
+
+class Vn:
+    def __init__(self):
+        self.os_platform: str = platform
+        self.networkURL: str = None # https://verteonetwork.veevanetwork.com
+        self.networkUserName: str = None
+        self.networkPassword: str = None
+        self.networkCountry: str = 'US'
+        self.networkConnection: requests.models.Response = None
+        self.networkLanguages: list = None # List of languages supported by this instance of Veeva Network
+        self.networkObjects: dict = None # Dictionary of Network Objects and their properties
+        self.networkObjectMetadata: dict = None # {'HCP': {'my_custom_field__c': {'fieldId': 'my_custom_field__c','type': {'dataType': 'STRING', 'discriminator': None}, 'labels': {'en': 'My Custom Field'}}}}
+        self.networkReferenceTypes: dict = None # {'AddressAdminArea': {'type': 'AddressAdminArea','customerOwned': False,'inactive': False,'description': 'AddressAdminArea'}, 'AddressCBSA': {'type': 'AddressCBSA' ... }}
+        self.networkReferenceValueMetadata: dict = None # Dictionary of Network Reference Value Metadata, including countries, reference codes, translated values, etc.
+        self.sessionId: str = None
+        self.networkId: str = None
+        self.APIheaders: dict = None
+        self.APIversionList: list = []
+        self.LatestAPIversion: str = None
+        self.network_references_all: pd.DataFrame = None
+        self.network_DNS: str = None # verteonetwork.veevanetwork.com
+        self.network_protocol: str = None # https
+
+        #----------------------------------------------------------------
+        # Load Network API Json
+        self.network_api_json: dict = None
+        try: # Try to load the network API json, to be used in a packaged distribution context
+            with importlib.resources.open_text("veevanetwork", "network_api_v25.json") as file:
+                self.network_api_json = json.load(file)
+        except: # If the above fails, try to load the network API json, to be used in a development context
+            with open('network_api_v25.json', encoding="utf-8") as file:
+                self.network_api_json = json.load(file)
+        self.network_api_parsed: dict = self.__parse_network_api_json(self.network_api_json)
+        self.api_categories: list = list(self.network_api_parsed['item'].keys())
+
+        self.api_change_request = self.network_api_parsed['item']['Change Request']
+        self.api_custom_key = self.network_api_parsed['item']['Custom Key']
+        self.api_entity = self.network_api_parsed['item']['Entity']
+        self.api_hco = self.network_api_parsed['item']['HCO']
+        self.api_hcp = self.network_api_parsed['item']['HCP']
+        self.api_metadata = self.network_api_parsed['item']['Metadata']
+        self.api_subscriptions = self.network_api_parsed['item']['Subscriptions']
+        self.api_subscriptions_compliance = self.network_api_parsed['item']['Subscriptions - Compliance']
+        self.api_subscriptions_source = self.network_api_parsed['item']['Subscriptions - Source']
+        self.api_subscriptions_target = self.network_api_parsed['item']['Subscriptions - Target']
+        self.api_events = self.network_api_parsed['item']['Events']
+        self.api_match = self.network_api_parsed['item']['Match']
+        self.api_suspect_match = self.network_api_parsed['item']['Suspect Match']
+        self.api_authentication = self.network_api_parsed['item']['Authentication']
+        self.api_retrieve_available_api_versions = self.network_api_parsed['item']['Retrieve Available API Versions']
+        self.api_search = self.network_api_parsed['item']['Search']
+        self.call = {
+            "Change Request": {
+                "change_request_create": self.change_request_create,
+                "change_request_cancel": self.change_request_cancel,
+                "change_request_retrieve": self.change_request_retrieve,
+                "change_request_batch_retrieve": self.change_request_batch_retrieve,
+                "change_request_update": self.change_request_update,
+                "change_request_batch_update": self.change_request_batch_update,
+                "change_request_process": self.change_request_process,
+                "change_request_batch_process": self.change_request_batch_process,
+                "change_request_search": self.change_request_search,
+                "change_request_match": self.change_request_match,
+                "change_request_batch_approve": self.change_request_batch_approve,
+                "change_request_batch_reject": self.change_request_batch_reject
+            },
+            "Custom Key": {
+                "custom_key_associate_to_entity": self.custom_key_associate_to_entity,
+                "custom_key_associate_to_child": self.custom_key_associate_to_child,
+                "custom_key_batch_associate_to_entities": self.custom_key_batch_associate_to_entities,
+                "custom_key_batch_associate_to_children": self.custom_key_batch_associate_to_children,
+                "custom_key_disassociate": self.custom_key_disassociate,
+                "custom_key_batch_disassociate": self.custom_key_batch_disassociate
+            },
+            "Entity": {
+                "entity_retrieve": self.entity_retrieve,
+                "entity_retrieve_child": self.entity_retrieve_child,
+                "entity_batch_retrieve": self.entity_batch_retrieve,
+                "entity_batch_retrieve_children": self.entity_batch_retrieve_children
+            },
+            "HCO": {
+                "hco_retrieve": self.hco_retrieve,
+                "hco_associate_custom_key": self.hco_associate_custom_key,
+                "hco_address_associate_custom_key": self.hco_address_associate_custom_key,
+                "hco_license_associate_custom_key": self.hco_license_associate_custom_key,
+                "hco_parenthco_associate_custom_key": self.hco_parenthco_associate_custom_key
+            },
+            "HCP": {
+                "hcp_retrive": self.hcp_retrive,
+                "hcp_associate_custom_key": self.hcp_associate_custom_key,
+                "hcp_address_associate_custom_key": self.hcp_address_associate_custom_key,
+                "hcp_license_associate_custom_key": self.hcp_license_associate_custom_key,
+                "hcp_parenthco_associate_custom_key": self.hcp_parenthco_associate_custom_key
+            },
+            "Metadata": {
+                "metadata_retrieve_available_api_versions": self.metadata_retrieve_available_api_versions,
+                "metadata_retrieve_hashtags": self.metadata_retrieve_hashtags,
+                "metadata_retrieve_object_types": self.metadata_retrieve_object_types,
+                "metadata_retrieve_field": self.metadata_retrieve_field,
+                "metadata_retrieve_field_details": self.metadata_retrieve_field_details,
+                "metadata_retrieve_field_groups": self.metadata_retrieve_field_groups,
+                "metadata_retrieve_reference_data_types": self.metadata_retrieve_reference_data_types,
+                "metadata_retrieve_reference_data_type_details": self.metadata_retrieve_reference_data_type_details,
+                "metadata_retrieve_reference_data_type_code_details": self.metadata_retrieve_reference_data_type_code_details
+            },
+            "Subscriptions": {
+                "subscriptions_create_job": self.subscriptions_create_job,
+                "subscriptions_retrieve_job": self.subscriptions_retrieve_job,
+                "subscriptions_cancel_job": self.subscriptions_cancel_job,
+                "subscriptions_retrieve_export_job_file": self.subscriptions_retrieve_export_job_file
+            },
+            "Subscriptions - Compliance": {
+                "subscriptions_compliance_create_job": self.subscriptions_compliance_create_job,
+                "subscriptions_compliance_retrieve_job": self.subscriptions_compliance_retrieve_job,
+                "subscriptions_compliance_cancel_job": self.subscriptions_compliance_cancel_job
+            },
+            "Subscriptions - Source": {
+                "subscriptions_source_create_job": self.subscriptions_source_create_job,
+                "subscriptions_source_retrieve_job": self.subscriptions_source_retrieve_job,
+                "subscriptions_source_cancel_job": self.subscriptions_source_cancel_job
+            },
+            "Subscriptions - Target": {
+                "subscriptions_target_create_job": self.subscriptions_target_create_job,
+                "subscriptions_target_retrieve_job": self.subscriptions_target_retrieve_job,
+                "subscriptions_target_cancel_job": self.subscriptions_target_cancel_job
+            },
+            "Events": {
+                "events_retrieve_merge": self.events_retrieve_merge,
+                "events_retrieve_unmerge": self.events_retrieve_unmerge
+            },
+            "Match": {
+                "match_retrieve": self.match_retrieve,
+                "suspect_match_batch_reject_task": self.suspect_match_batch_reject_task,
+
+            },
+            "Suspect Match": {
+                "suspect_match_batch_process": self.suspect_match_batch_process,
+                "suspect_match_batch_create": self.suspect_match_batch_create,
+                "suspect_match_batch_reject_task": self.suspect_match_batch_reject_task,
+                "suspect_match_batch_retrieve": self.suspect_match_batch_retrieve
+            },
+            "Retrieve Available API Versions": {
+                "retrieve_available_api_versions": self.retrieve_available_api_versions
+            },
+            "Search": {
+                "search": self.search
+            }
+            }
+    
+    # =============================================================================
+    # Authentication
+    # =============================================================================
+
+    # Refactored - MP 20220610
+    def authenticate(
+        self, 
+        networkURL: str=None, 
+        networkUserName: str=None, 
+        networkPassword: str=None, 
+        networkCountry: str=None, 
+        networkId: str=None,
+        sessionId: str=None,
+        if_return: bool=False, 
+        *args, **kwargs
+    ) -> Optional[dict]:
+        """
+        Authenticates Veeva Network and retrieves the auth token.
+
+        Example:
+        authenticate using unpacked kwargs from the retrieve_credentials function
+            authenticate_vn(**retrieve_credentials(platform, 'credentials.xlsx')[0])
+
+        Return Example:
+            {'sf': <simple_salesforce.api.Salesforce at 0x24a045c7b50>,
+             'bulk': <salesforce_bulk.salesforce_bulk.SalesforceBulk at 0x24a045c7e20>,
+             'sfMeta': <sfdclib.session.SfdcSession at 0x24a044b3400>,
+             'tooling': <sfdclib.tooling.SfdcToolingApi at 0x24a045d17f0>,
+             'session_id': '00D3F000000FZCq!AQYAQHYfSLYGI9cTyjDfxAAzYm.1uOKmNPXlKMW0sVz5ilIQ9ZwVTh6kOlaRuqfPuuzNnZNb3461sUGeUZ57ttE.GBawbt5h',
+             'instance': 'cslbehring-core--devr01.my.salesforce.com',
+             'sfMeta_is_connected': True,
+             'bulk_api_sessionId': '00D3F000000FZCq!AQYAQHYfSLYGI9cTyjDfxAAzYm.1uOKmNPXlKMW0sVz5ilIQ9ZwVTh6kOlaRuqfPuuzNnZNb3461sUGeUZ57ttE.GBawbt5h'}
+
+        Dependencies:
+            import requests
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Authenticate
+        
+        """
+        if (networkId and sessionId and networkURL):
+            self.networkId = self.networkId if networkId is None else networkId
+            self.sessionId = self.sessionId if sessionId is None else sessionId
+        
+        url_parse = urlparse(networkURL)
+        if len(url_parse.scheme) == 0:
+            self.network_protocol = 'https'
+            if len(url_parse.path) > 0:
+                self.network_DNS = url_parse.path
+                self.networkURL = self.network_protocol + '://' + url_parse.path
+
+        if len(url_parse.scheme) > 0:
+            self.network_protocol = url_parse.scheme
+            if len(url_parse.netloc) > 0:
+                self.network_DNS = url_parse.netloc
+                self.networkURL = url_parse.scheme + '://' + url_parse.netloc
+
+        if (self.networkURL is None) or (len(self.networkURL) == 0):
+            raise Exception('networkURL is required')
+
+
+        # self.networkURL = self.networkURL if networkURL is None else networkURL
+        self.networkUserName = self.networkUserName if networkUserName is None else networkUserName
+        self.networkPassword = self.networkPassword if networkPassword is None else networkPassword
+        self.networkCountry = self.networkCountry if networkCountry is None else networkCountry
+        
+        if (self.networkUserName and self.networkPassword and self.networkURL):
+            self.networkConnection = requests.post(self.networkURL + '/api/v17.0/auth?username=' + self.networkUserName + '&password=' + self.networkPassword)
+            if (self.networkConnection.json()['responseStatus'] == 'SUCCESS'):
+                self.sessionId = self.networkConnection.json()['sessionId']
+                self.userId = self.networkConnection.json()['userId']
+                self.networkId = self.networkConnection.json()['networkId']
+            else:
+                raise Exception(self.networkConnection.json())
+
+        
+        self.APIheaders = {'authorization': self.sessionId}
+        self.APIversionList = []
+        
+        # Error checking whether the required parameters are passed in
+        # The check happens here because this is where all the self assignments has completed
+        if (not (self.networkId and self.sessionId and self.networkURL)) and (not (self.networkUserName and self.networkPassword and self.networkCountry and self.networkURL)):
+            raise Exception("Please provide either networkId, sessionId, and networkURL or networkUserName, networkPassword, and networkURL")
+        
+        for API in requests.get(self.networkURL +'/api', headers=self.APIheaders).json()['values'].keys():
+            self.APIversionList.append(float(API.replace("v", "")))
+        self.APIversionList.sort()
+        self.LatestAPIversion = "v" + str(self.APIversionList[-1])
+        
+
+        if if_return:
+            return {'networkURL':self.networkURL, 
+                    'networkUserName':self.networkUserName, 
+                    'networkPassword':self.networkPassword, 
+                    'networkConnection':self.networkConnection, 
+                    'sessionId':self.sessionId, 
+                    'APIheaders':self.APIheaders, 
+                    'APIversionList':self.APIversionList, 
+                    'LatestAPIversion':self.LatestAPIversion}    
+
+    # Refactored - MP 20220610
+    def get_networkObjects(self) -> pd.DataFrame:
+        """
+        Returns a list of all objects in the Veeva Network.
+        """
+        self.authenticate()
+
+        self.networkObjects = self.list_of_dicts_to_dict(requests.get(self.networkURL + '/api/' + self.LatestAPIversion + '/metadata/objectTypes',
+                                      headers=self.APIheaders).json()['objectTypes'], 'name')
+        return self.networkObjects
+
+    # Refactored - MP 20220610
+    def get_networkObjectMetadata(self) -> pd.DataFrame:
+        self.authenticate()
+        if self.networkObjects is None:
+            self.get_networkObjects()
+
+        processing_dict = {}
+        __empty =[
+            processing_dict.update({networkObject: 
+                self.list_of_dicts_to_dict(requests.get(
+                        self.networkURL + 
+                        '/api/'+ self.LatestAPIversion +
+                        '/metadata/fields?objectTypes=' + 
+                        networkObject + '&details=full' + 
+                        '&countries='+ self.networkCountry, 
+                        headers=self.APIheaders).json()['attributes'],
+                        'fieldId')}) 
+                        for networkObject in self.networkObjects.keys()]
+        self.networkObjectMetadata = processing_dict
+        return self.networkObjectMetadata
+
+
+    # Refactored - MP 20220612
+    def process_networkReferenceCodeMetadata(
+        self,
+        referenceTypes: Optional[list] = None, # List of reference types to retrieve, leave empty (None) to retrieve all
+        customerOwned: Optional[bool] = None, # True (customer owned only), False (ootb), None (customer owned and ootb)
+        activeReferences: Optional[bool]= None, # True (active only), False (inactive only), None (active and inactive)
+        languages: Optional[list]= None, # List of languages to retrieve, leave empty (None) to retrieve all
+        countries: Optional[list]= None, # List of countries to retrieve, leave empty (None) to retrieve all
+    ):
+        """
+        Processes Network Reference Metadata and returns a DataFrame of the reference codes based on the parameters.
+
+        Parameters:
+        referenceTypes: List of reference types to retrieve, leave empty (None) to retrieve all
+        customerOwned (bool): Filter references by customerOwned status. Values: True (customerOwned only), False (ootb only), None (customerOwned and ootb)
+        activeReferences (bool): Filter references by status. Values: True (active only), False (inactive only), None (active and inactive)
+        languages (list): List of languages to return. Default: ['en']
+        countries (list): List of countries to return. Default: ['US']
+
+        Returns:
+        DataFrame: A DataFrame of the reference codes based on the parameters.
+        """
+
+        if self.networkReferenceValueMetadata is None:
+            self.get_networkReferenceValueMetadata()
+        
+        if languages is None:
+            if self.networkLanguages is None:
+                self.get_networkLanguages()
+            languages = self.networkLanguages
+            
+        networkReferenceDF = pd.DataFrame(self.networkReferenceValueMetadata)
+        networkReferenceCodeDataframe = networkReferenceDF.loc['reference_type_codes', :].dropna()
+        reference_code_dict_unfiltered: dict[str, pd.DataFrame] = {}
+        for index, values in zip(networkReferenceCodeDataframe.index, networkReferenceCodeDataframe.values):
+            reference_code_dict_unfiltered.update({index: pd.DataFrame(self.list_of_dicts_to_dict(values, 'code'))})
+        
+        final_df = pd.DataFrame()
+        for reference_type, reference_dataframe in zip(reference_code_dict_unfiltered.keys(), reference_code_dict_unfiltered.values()):
+            if referenceTypes is None or reference_type in referenceTypes:
+                activeReferences = None
+                customerOwned = None
+                activeReferences_filter = [True,False] if activeReferences is None else [not(activeReferences)]
+                customerOwned_filter = [True,False] if customerOwned is None else [customerOwned]
+                reference_dataframe = reference_dataframe.T.copy()
+                filtered_customerOwned_and_active = reference_dataframe[
+                                                (reference_dataframe['customerOwned'].isin(customerOwned_filter)) & 
+                                                (reference_dataframe['inactive'].isin(activeReferences_filter))
+                                                ]
+
+                filtered_languages = pd.DataFrame()
+
+                for language in languages:
+                    filtered_languages = pd.concat([filtered_languages,
+                                                pd.DataFrame(
+                                                    filtered_customerOwned_and_active["values"]
+                                                    .apply(lambda value: value[language] 
+                                                    if value.keys()
+                                                    .__contains__(language) 
+                                                    else np.nan)
+                                                    .dropna()
+                                                    .rename(language))], axis=1)
+                filtered_languages.insert(0, 'Network Code', filtered_languages.index)
+                filtered_languages.insert(1, 'Reference Type', reference_type)
+                filtered_languages.insert(2, 'Active Countries', pd.DataFrame(filtered_customerOwned_and_active["countries"]
+                                                    .apply(lambda value: ";".join(sorted(value)) if (countries is None or len(set(value).intersection(set(countries)))>0 ) else np.nan).rename('countries')
+                                                )['countries'])
+                filtered_languages.insert(3, 'Definition', pd.DataFrame(
+                                                    filtered_customerOwned_and_active["values"]
+                                                    .apply(lambda value: value['en'] 
+                                                    if value.keys()
+                                                    .__contains__('en') 
+                                                    else np.nan)
+                                                    .dropna()
+                                                    .rename('en'))['en'])
+                filtered_languages.insert(4, 'Active?', filtered_customerOwned_and_active["inactive"] == False)
+                filtered_languages.insert(5, 'Veeva Maintained?', filtered_customerOwned_and_active["customerOwned"] == False)             
+                filtered_languages.reset_index(drop=True, inplace=True)
+                filtered_languages.dropna(subset=['Active Countries'], inplace=True)
+                filtered_languages.replace(np.nan, "", inplace=True)
+                filtered_languages
+                final_df = pd.concat([final_df, filtered_languages], axis=0)
+
+        final_df.reset_index(drop=True, inplace=True)
+        
+        return final_df
+
+    # To be deprecated, used by object_metadata_dataframe()
+    def object_metadata(self):
+        self.networkObjects = requests.get(self.networkURL + '/api/' + self.LatestAPIversion + '/metadata/objectTypes',
+                                      headers=self.APIheaders).json()['objectTypes']
+        networkObjectList = []
+        for obj in self.networkObjects:
+            if obj['status'] == 'ACTIVE':
+                networkObjectList.append(obj['name'])
+            else:
+                pass
+        object_metadata = pd.DataFrame([requests.get(self.networkURL + '/api/'+ self.LatestAPIversion +'/metadata/fields?objectTypes=' + networkObject + '&details=full' + '&countries='+ self.networkCountry, headers=self.APIheaders).json()['attributes'] 
+                                              for networkObject in networkObjectList])
+        object_metadata = object_metadata.transpose()
+        object_metadata.columns = networkObjectList
+        return object_metadata
+
+    # To be deprecated, use get_networkObjectMetadata() instead
+    def object_metadata_dataframe(self, object_metadata = None, attribute = None, *args):
+        """
+        Function that takes an input of data table with metadata values containing field for each row and objects for each column, 
+        lists of input attributes available in the meta data (i.e. ['type','dataType']), 
+        and optional arguments containing comma separated lists of additional attributes available in the meta data 
+        
+        Example:
+            VeevaNetwork.object_metadata_dataframe(self.object_metadata(), ['fieldId'], ['type','dataType'], ['type','discriminator'], ['labels','en'],['maximumLength'])
+            
+        Return Example:
+        (Dataframe)
+            HCP.fieldId    HCP.type.dataType    HCP.type.discriminator    HCP.labels.en    HCP.maximumLength    HCO.fieldId      ...
+            hcp_type__v    REFERENCE            HCPType                   HCP Type         100.0                340B_eligible__v ...
+        
+        """
+        self.authenticate()
+        
+        object_metadata = self.object_metadata() if object_metadata is None else object_metadata
+        
+        object_metadata_dataframe = pd.DataFrame()
+        attribute1 = attribute[0]
+        attribute2 = attribute[1] if len(attribute) > 1 else ""
+        for networkObjectName, networkObjectMetaData in object_metadata.iteritems():
+            attributeList = []
+            for fieldMetaData in networkObjectMetaData:
+                try:
+                    if attribute2 == "":
+                        attributeList.append(fieldMetaData[attribute1])
+                    else:
+                        attributeList.append(fieldMetaData[attribute1][attribute2])
+                except TypeError:
+                    continue
+    #        object_metadata_dataframe[networkObjectName + '.' + attribute1 + (("." + attribute2) if attribute2 != "" else "")] = pd.Series(attributeList, name = networkObjectName)
+            object_metadata_dataframe = pd.concat([object_metadata_dataframe,pd.Series(attributeList, name = networkObjectName + '.' + attribute1 + (("." + attribute2) if attribute2 != "" else "")).to_frame()], ignore_index=False, axis=1)
+
+
+            # parse arguments
+            if args:
+                for arg in args:
+                    argAttribute1 = arg[0]
+                    argAttribute2 = arg[1] if len(arg)>1 else ""
+                    argAttributeList = []
+                    for fieldMetaData in networkObjectMetaData:
+                        try:
+                            if argAttribute2 == "":
+                                argAttributeList.append(fieldMetaData[argAttribute1])
+                            else:
+                                argAttributeList.append(fieldMetaData[argAttribute1][argAttribute2])
+                        except:
+                            argAttributeList.append("")
+                            continue
+    #                object_metadata_dataframe[networkObjectName + '.' + argAttribute1 + (("." + argAttribute2) if argAttribute2 != "" else "")] = pd.Series(argAttributeList, name = networkObjectName)
+                    object_metadata_dataframe = pd.concat([object_metadata_dataframe,pd.Series(argAttributeList, name = networkObjectName + '.' + argAttribute1 + (("." + argAttribute2) if argAttribute2 != "" else "")).to_frame()], ignore_index=False, axis=1)
+            else:
+                continue
+        return object_metadata_dataframe
+
+    # Refactored - MP 20220611
+    def get_networkReferenceValueMetadata(self):
+        """
+        Retruns a Dictionary of Network Reference Value Metadata, including countries, reference codes, translated values, etc.
+        """
+        self.authenticate()
+        self.networkReferenceValueMetadata = self.list_of_dicts_to_dict(requests.get(self.networkURL + '/api/' + self.LatestAPIversion + '/metadata/reference_values?includeCodes=True', headers = self.APIheaders).json()['reference_type_values'],'type')
+        return self.networkReferenceValueMetadata
+
+    # Deprecated
+    def reference_value_dataframe(self):
+        """
+        Retrieve all reference values in Network  
+        ** formula can be enhanced or take input parameters so it doesn't query every single reference alias
+
+        """
+        self.authenticate()
+
+        self.networkReferenceTypes = self.list_of_dicts_to_dict(requests.get(self.networkURL + '/api/' + self.LatestAPIversion + '/metadata/reference_values?includeCodes=True', headers = self.APIheaders).json()['reference_type_values'],'type')
+        reference_value_dataframe = pd.DataFrame()
+        for x in self.networkReferenceTypes.keys():
+            try:
+                referenceCall = requests.get(self.networkURL + '/api/'+ self.LatestAPIversion + '/metadata/reference_values/' + x + '?countries='+ self.networkCountry, headers = self.APIheaders).json()['reference_type_codes']
+                newColumn = pd.Series([x['values']['en'] for x in referenceCall],name = str(x) + " Value")
+                
+                newColumn2 = pd.Series([x['code'] for x in referenceCall], name = x)
+                reference_value_dataframe.insert(len(reference_value_dataframe.columns), column = x, value = newColumn2)
+                reference_value_dataframe.insert(len(reference_value_dataframe.columns), column = str(x) + " Value", value = newColumn)
+            except:
+                pass
+        return reference_value_dataframe
+
+    def extract_network_reference_table(self):
+        self.authenticate()
+        
+        references_all = pd.DataFrame(requests.get(self.networkURL + '/api/'+ self.LatestAPIversion + '/metadata/reference_values?includeCodes=true&countries='+ self.networkCountry, headers = self.APIheaders).json()['reference_type_values'])
+        network_reference_table = pd.DataFrame()
+        self.network_references_all = references_all
+        for row in references_all['reference_type_codes']:
+            if isinstance(row, list):
+                network_reference_table = pd.concat([network_reference_table, pd.json_normalize(row)], axis=1)
+            else:
+                continue
+        network_reference_table.fillna('',inplace=True)
+        return network_reference_table
+    
+    # =============================================================================
+    # WIP Functions
+    # =============================================================================
+
+
+    # =============================================================================
+    # Change Request
+    # =============================================================================
+
+    def change_request_create(self, *args, **kwargs):
+        """
+        This API enables you to create a Network change request to add or update an HCP or HCO and related entities (including addresses, licenses, or parentHCOs) for **gray** data only.
+
+        Change requests created using the API against orange data will be rejected.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Createachangerequest
+
+        """
+        
+        return self.api_call(self.api_change_request['item']['Create Change Request'], *args, **kwargs)
+        
+    def change_request_cancel(self, *args, **kwargs):
+        """
+        This API enables you to cancel a change request by providing the change request ID.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Cancelchangerequest
+
+        """
+        return self.api_call(self.api_change_request['item']['Cancel Change Request'], *args, **kwargs)
+
+    def change_request_retrieve(self, *args, **kwargs):
+        """
+        This API enables you to retrieve response information for the create, update, and merge change requests submitted by a client application.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#RetrieveChangeRequest
+
+        """
+        return self.api_call(self.api_change_request['item']['Retrieve Change Request'], *args, **kwargs)
+        
+    def change_request_batch_retrieve(self, *args, **kwargs):
+        """
+        This API enables you to obtain information about multiple change requests through the API.
+
+        Documenatation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Batchretrievechangerequest  
+
+        """
+        return self.api_call(self.api_change_request['item']['Change Request Batch Retrieve'], *args, **kwargs)
+        
+    def change_request_update(self, *args, **kwargs):
+        """
+        This API enables you to update an unprocessed change request through the API.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#UpdateChangeRequest
+
+        """
+        return self.api_call(self.api_change_request['item']['Change Request Update'], *args, **kwargs)
+
+    def change_request_batch_update(self, *args, **kwargs):
+        """
+        This API enables you to update multiple unprocessed change requests.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#BatchUpdateChangeRequests
+
+        """
+        return self.api_call(self.api_change_request['item']['Change Request Batch Update'], *args, **kwargs)
+
+    def change_request_process(self, *args, **kwargs):
+        """
+        This API enables you to process an unprocessed change request through the API.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#ProcessChangeRequest
+
+        """
+        return self.api_call(self.api_change_request['item']['Change Request Process'], *args, **kwargs)
+
+    def change_request_batch_process(self, *args, **kwargs):
+        """
+        This API enables you to process multiple unprocessed change requests.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#BatchProcessChangeRequests
+        """
+        return self.api_call(self.api_change_request['item']['Change Request Batch Process'], *args, **kwargs)
+
+    def change_request_search(self, *args, **kwargs):
+        """
+        This API enables you to retrieve all change requests that match a specified search criteria.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#ChangeRequestSearch
+
+        """
+        return self.api_call(self.api_change_request['item']['Change Request Search'], *args, **kwargs)
+
+    def change_request_match(self, *args, **kwargs):
+        """
+        This API enables you to match a request to an existing entity. You can use either the Veeva ID or custom key of an existing entity to match the request against.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#ChangeRequestMatch
+
+        """
+        return self.api_call(self.api_change_request['item']['Change Request Match'], *args, **kwargs)
+
+    def change_request_batch_approve(self, *args, **kwargs):
+        """
+        This API enables you to bulk approve up to 500 change requests.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#BatchApproveChangeRequests
+
+        """
+        return self.api_call(self.api_change_request['item']['Change Request Batch Approve'], *args, **kwargs)
+
+    def change_request_batch_reject(self, *args, **kwargs):
+        """
+        This API enables you to bulk reject up to 500 change requests.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#BatchRejectChangeRequests
+
+        """
+        return self.api_call(self.api_change_request['item']['Change Request Batch Reject'], *args, **kwargs)
+    
+    # =============================================================================
+    # Custom Key
+    # =============================================================================
+
+    def custom_key_associate_to_entity (self, *args, **kwargs):
+        """
+        This API enables you to submit external key identifiers when new HCPs or HCOs are downloaded from Network without going through the full change request process.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Associatecustomkeytoentity
+
+        """
+        return self.api_call(self.api_custom_key['item']['Associate Custom Key to Entity'], *args, **kwargs)
+
+    def custom_key_associate_to_child (self, *args, **kwargs):
+        """
+        This API enables you to submit external key identifiers when new children (address, license, or parent HCOs) are downloaded from Network without going through the full change request process.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Associatecustomkeytochildren
+
+        """
+        return self.api_call(self.api_custom_key['item']['Associate Custom Key to Children'], *args, **kwargs)
+
+    def custom_key_batch_associate_to_entities (self, *args, **kwargs):
+        """
+        This API enables you to submit external key identifiers whenever new HCPs or HCOs are downloaded from Network without going through the full change request process.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Batchassociatecustomkeystoentities
+
+        """
+        return self.api_call(self.api_custom_key['item']['Batch Associate Custom Keys to Entities'], *args, **kwargs)
+
+    def custom_key_batch_associate_to_children (self, *args, **kwargs):
+        """
+        This API enables you to submit external key identifiers when new children (address, license, or parent HCOs) are downloaded from Network without going through the full change request process.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Batchassociatecustomkeytochildren
+
+        """
+        return self.api_call(self.api_custom_key['item']['Batch Associate Custom Keys to Children'], *args, **kwargs)
+
+    def custom_key_disassociate (self, *args, **kwargs):
+        """
+        This API enables you to deactivate external key identifiers for any entity (an HCP, HCO, Address, License, or ParentHCO) in Network without going through the full change request process.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Disassociatecustomkey
+
+        """
+        return self.api_call(self.api_custom_key['item']['Disassociate Custom Key'], *args, **kwargs)
+
+    def custom_key_batch_disassociate (self, *args, **kwargs):
+        """
+        This API enables you to inactivate external key identifiers for any entity (HCP, HCO, Address, License, or ParentHCO) in Network without going through the full change request process.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Batchdisassociatecustomkey
+
+        """
+        return self.api_call(self.api_custom_key['item']['Batch Disassociate Custom Key'], *args, **kwargs)
+
+
+    # =============================================================================
+    # Entity
+    # =============================================================================
+
+    def entity_retrieve (self, *args, **kwargs):
+        """
+        This API enables you to obtain information on any entity without identifying the specific entity type. It is only used to retrieve information from Network using the GET method.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrieveentity
+
+        """
+        return self.api_call(self.api_entity['item']['Retrieve Entity'], *args, **kwargs)
+
+    def entity_retrieve_child (self, *args, **kwargs):
+        """
+        This API enables you to retrieve child entity information; for example address or license details, for the Network ID provided without identifying the specific entity type.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrievechildentity
+
+        """
+        return self.api_call(self.api_entity['item']['Retrieve Child Entity'], *args, **kwargs)
+
+    def entity_batch_retrieve (self, *args, **kwargs):
+        """
+        This API enables you to retrieve entity details directly from Network. It is only used to retrieve information using the GET method. To update or delete entity data, you must use the change request APIs.
+
+        The entities you can retrieve include HCPs and HCOs, and details are returned for all corresponding child entities: addresses, licenses, parent HCOs, and custom keys.
+        
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Batchretrieveentities
+
+        """
+        return self.api_call(self.api_entity['item']['Batch Retrieve Entities'], *args, **kwargs)
+
+    def entity_batch_retrieve_children (self, *args, **kwargs):
+        """
+        This API enables you to obtain information on child entities without identifying the specific entity type. Users are only allowed to retrieve (GET) information from Network.
+
+        All other operations (POST and DELETE) are restricted and can only be performed by submitting a change request using the change request APIs.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Batchretrievechildentities
+
+        """
+        return self.api_call(self.api_entity['item']['Batch Retrieve Child Entities'], *args, **kwargs)
+
+
+    # =============================================================================
+    # HCO
+    # =============================================================================
+
+    def hco_retrieve (self, *args, **kwargs):
+        """
+        This API enables you to retrieve information about an HCO. Information you can retrieve for an HCO includes the HCO, address, license, and parent HCO information (including their custom keys) for the HCO vid_key you provide.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#RetrieveHCO
+
+        """
+        return self.api_call(self.api_hco['item']['Retrieve HCO'], *args, **kwargs)
+
+    def hco_associate_custom_key (self, *args, **kwargs):
+        """
+        This API enables you to submit external key identifiers when new HCOs are downloaded from Network without going through the full change request process. This API associates the external identifier you submit to the HCO vid_key you provide.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#AssociatecustomkeytoHCO
+
+        """
+        return self.api_call(self.api_hco['item']['Associate Custom Key to HCO'], *args, **kwargs)
+
+    def hco_address_associate_custom_key (self, *args, **kwargs):
+        """
+        This API enables you to submit external key identifiers when new HCO child objects (addresses) 
+        are downloaded from Network without going through the full change request process. 
+        This API associates the external identifier you submit to the child object key you provide.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Associatecustomkeytoachildobject
+
+        """
+        return self.api_call(self.api_hco['item']['Associate Custom Key to HCO Address'], *args, **kwargs)
+
+    def hco_license_associate_custom_key (self, *args, **kwargs):
+        """
+        This API enables you to submit external key identifiers when new HCO child objects (licenses) 
+        are downloaded from Network without going through the full change request process. 
+        This API associates the external identifier you submit to the child object key you provide.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Associatecustomkeytoachildobject
+
+        """
+        return self.api_call(self.api_hco['item']['Associate Custom Key to HCO License'], *args, **kwargs)
+
+    def hco_parenthco_associate_custom_key (self, *args, **kwargs):
+        """
+        This API enables you to submit external key identifiers when new HCO child objects (parent HCOs) 
+        are downloaded from Network without going through the full change request process. 
+        This API associates the external identifier you submit to the child object key you provide.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Associatecustomkeytoachildobject
+
+        """
+        return self.api_call(self.api_hco['item']['Associate Custom Key to HCO ParentHCO'], *args, **kwargs)
+
+    # =============================================================================
+    # HCP
+    # =============================================================================
+    def hcp_retrive (self, *args, **kwargs):
+        """
+        This API enables you to retrieve information about an HCP including the HCP itself, address, license, and parent HCO information (including their custom keys) for the HCP vid_key you provide.
+
+        This API downloads the record for the specified entity from Veeva OpenData to your customer instance.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#RetrieveHCP
+
+        """
+        return self.api_call(self.api_hcp['item']['Retrieve HCP'], *args, **kwargs)
+
+    def hcp_associate_custom_key (self, *args, **kwargs):
+        """
+        This API enables you to submit external key identifiers when new HCPs are downloaded from Network without going through the full change request process. This API associates the external identifier you submit to the HCP vid_key you provide.
+
+        This API requires system administrator or API-only permissions.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#AssociatecustomkeytoHCP
+
+        """
+        return self.api_call(self.api_hcp['item']['Associate Custom Key to HCP'], *args, **kwargs)
+
+    def hcp_address_associate_custom_key (self, *args, **kwargs):
+        """
+        This API enables you to submit external key identifiers when new HCP child objects (addresses) are downloaded from Network without going through the full change request process. This API associates the external identifier you submit to the child object key you provide.
+
+        This API requires system administrator or API-only permissions.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Associatecustomkeytoachildobject1
+
+        """
+        return self.api_call(self.api_hcp['item']['Associate Custom Key to HCP Address'], *args, **kwargs)
+
+    def hcp_license_associate_custom_key (self, *args, **kwargs):
+        """
+        This API enables you to submit external key identifiers when new HCP child objects (licenses) are downloaded from Network without going through the full change request process. This API associates the external identifier you submit to the child object key you provide.
+
+        This API requires system administrator or API-only permissions.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Associatecustomkeytoachildobject1
+        
+        """
+        return self.api_call(self.api_hcp['item']['Associate Custom Key to HCP License'], *args, **kwargs)
+
+    def hcp_parenthco_associate_custom_key (self, *args, **kwargs):
+        """
+        This API enables you to submit external key identifiers when new HCP child objects (parent HCOs) are downloaded from Network without going through the full change request process. This API associates the external identifier you submit to the child object key you provide.
+
+        This API requires system administrator or API-only permissions.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Associatecustomkeytoachildobject1
+        
+        """
+        return self.api_call(self.api_hcp['item']['Associate Custom Key to HCP ParentHCO'], *args, **kwargs)
+
+    # =============================================================================
+    # Metadata
+    # =============================================================================
+    def metadata_retrieve_available_api_versions (self, *args, **kwargs):
+        """
+        This enables you to retrieve summary information about each API version available in Network.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#RetrieveavailableAPIversions
+        
+        """
+        return self.api_call(self.api_metadata['item']['Retrieve Available API Versions'], *args, **kwargs)
+        
+    def metadata_retrieve_hashtags (self, *args, **kwargs):
+        """
+        This API enables you to retrieve the list of hashtags available in a Network instance.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrievehashtags
+
+        """
+        return self.api_call(self.api_metadata['item']['Retrieve hashtags'], *args, **kwargs)
+
+    # TODO: rename/refactor method.
+    def get_networkLanguages(self) -> list:
+        """
+        This API enables you to retrieve the list of reference data languages available in a Network instance.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrievelanguages
+
+        """
+
+        self.authenticate()
+        self.networkLanguages = list(self.list_of_dicts_to_dict(
+            requests.get(
+                self.networkURL + 
+                '/api/' + 
+                self.LatestAPIversion + 
+                '/metadata/languages', 
+                headers=self.APIheaders).json()['languages'], 
+                'name'
+                ).keys())
+        return self.networkLanguages
+
+    def metadata_retrieve_object_types (self, *args, **kwargs):
+        """
+        This API enables you to retrieve the list of object types available in Network.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrieveobjecttypesmetadata
+
+        """
+        return self.api_call(self.api_metadata['item']['Retrieve Object Types Metadata'], *args, **kwargs)
+
+    def metadata_retrieve_field (self, *args, **kwargs):
+        """
+        This API enables you to retrieve detailed or summary information about the fields on each entity in Network.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrievefieldsmetadata
+
+        """
+        return self.api_call(self.api_metadata['item']['Retrieve Fields Metadata'], *args, **kwargs)
+
+    def metadata_retrieve_field_details (self, *args, **kwargs):
+        """
+        This API enables you to retrieve detailed information about the fields on each entity in Network.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrievefielddetailsmetadata
+
+        """
+        return self.api_call(self.api_metadata['item']['Retrieve Field Details Metadata'], *args, **kwargs)
+
+    def metadata_retrieve_field_groups (self, *args, **kwargs):
+        """
+        This API enables you to retrieve detailed information about the field groups available in Network. These field groups are used by the CRM bridge when retrieving and displaying information from Network in CRM.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrievefieldgroupsmetadata
+
+        """
+        return self.api_call(self.api_metadata['item']['Retrieve Field Groups Metadata'], *args, **kwargs)
+
+    def metadata_retrieve_reference_data_types (self, *args, **kwargs):
+        """
+        This API enables you to retrieve information about reference data types in Network.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrievereferencedatatypesmetadata
+
+        """
+        return self.api_call(self.api_metadata['item']['Retrieve Reference Data Types Metadata'], *args, **kwargs)
+
+    def metadata_retrieve_reference_data_type_details (self, *args, **kwargs):
+        """
+        This API enables you to retrieve detailed information about reference data types in Network.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrievereferencedatatypedetailsmetadata
+
+        """
+        return self.api_call(self.api_metadata['item']['Retrieve Reference Data Type Details Metadata'], *args, **kwargs)
+
+    def metadata_retrieve_reference_data_type_code_details (self, *args, **kwargs):
+        """
+        This API enables you to retrieve detailed information about reference data type codes in Network.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrievereferencedatatypecodedetailsmetadata
+
+        """
+        return self.api_call(self.api_metadata['item']['Retrieve Reference Data Type Code Details Metadata'], *args, **kwargs)
+
+    # =============================================================================
+    # Subscriptions
+    # =============================================================================
+    def subscriptions_create_job (self, *args, **kwargs):
+        """
+        This API enables you to create a subscription job.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Createasubscriptionjob
+
+        """
+        return self.api_call(self.api_subscriptions['item']['Create Subscription Job'], *args, **kwargs)
+
+    def subscriptions_retrieve_job (self, *args, **kwargs):
+        """
+        This API enables you to retrieve the status of a source or target subscription job.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrieveasubscriptionjobstatus
+
+        """
+        return self.api_call(self.api_subscriptions['item']['Retrieve Subscription Job'], *args, **kwargs)
+
+    def subscriptions_cancel_job (self, *args, **kwargs):
+        """
+        This API enables you to cancel a subscription job.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Cancelasubscriptionjob
+
+        """
+        return self.api_call(self.api_subscriptions['item']['Cancel Subscription Job'], *args, **kwargs)
+
+    def subscriptions_retrieve_export_job_file (self, *args, **kwargs):
+        """
+        This API enables you to retrieve the artifacts (file contents) of a target subscription job.
+        AKA: Retrieve target subscription artifact
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrievetargetsubscriptionartifact
+        
+        """
+        return self.api_call(self.api_subscriptions['item']['Retrieve Export Job File'], *args, **kwargs)
+
+    # =============================================================================
+    # Subscriptions - Compliance
+    # =============================================================================
+    def subscriptions_compliance_create_job (self, *args, **kwargs):
+        """
+        This API enables you to create a compliance subscription job.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Createacompliancesubscriptionjob
+
+        """
+        return self.api_call(self.api_subscriptions_compliance['item']['Create Compiance Subscription Job'], *args, **kwargs)
+
+    def subscriptions_compliance_retrieve_job (self, *args, **kwargs):
+        """
+        This API enables you to retrieve the status of a source or target subscription job.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrieveacompliancesubscriptionjobstatus
+        
+        """
+        return self.api_call(self.api_subscriptions_compliance['item']['Retrieve Compliance Subscription Job'], *args, **kwargs)
+
+    def subscriptions_compliance_cancel_job (self, *args, **kwargs):
+        """
+        This API enables you to cancel a compliance subscription job.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Cancelacompliancesubscriptionjob
+
+        """
+        return self.api_call(self.api_subscriptions_compliance['item']['Cancel Compliance Subscription Job'], *args, **kwargs)
+
+    # =============================================================================
+    # Subscriptions - Source
+    # =============================================================================
+    def subscriptions_source_create_job (self, *args, **kwargs):
+        """
+        This API enables you to create a source subscription job.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Createasourcesubscriptionjob
+
+        """
+        return self.api_call(self.api_subscriptions_source['item']['Create Source Subscription Job'], *args, **kwargs)
+
+    def subscriptions_source_retrieve_job (self, *args, **kwargs):
+        """
+        This API enables you to retrieve the status of a source subscription job.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrieveasourcesubscriptionjobstatus
+
+        """
+        return self.api_call(self.api_subscriptions_source['item']['Retrieve Source Subscription Job'], *args, **kwargs)
+
+    def subscriptions_source_cancel_job (self, *args, **kwargs):
+        """
+        This API enables you to cancel a source subscription job.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Cancelasourcesubscriptionjob
+        
+        """
+        return self.api_call(self.api_subscriptions_source['item']['Cancel Source Subscription Job'], *args, **kwargs)
+
+    # =============================================================================
+    # Subscriptions - Target
+    # =============================================================================
+    def subscriptions_target_create_job (self, *args, **kwargs):
+        """
+        This API enables you to create a target subscription job.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Createatargetsubscriptionjob
+
+        """
+        return self.api_call(self.api_subscriptions_target['item']['Create Target Subscription Job'], *args, **kwargs)
+
+    def subscriptions_target_retrieve_job (self, *args, **kwargs):
+        """
+        This API enables you to retrieve the status of a source or target subscription job.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrieveatargetsubscriptionjobstatus
+
+        """
+        return self.api_call(self.api_subscriptions_target['item']['Retrieve Target Subscription Job'], *args, **kwargs)
+
+    def subscriptions_target_cancel_job (self, *args, **kwargs):
+        """
+        This API enables you to cancel a target subscription job.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Cancelatargetsubscriptionjob
+        """
+        return self.api_call(self.api_subscriptions_target['item']['Cancel Target Subscription Job'], *args, **kwargs)
+
+    # =============================================================================
+    # Events
+    # =============================================================================
+    def events_retrieve_merge (self, *args, **kwargs):
+        """
+        This API enables you to retrieve the results of merge events that occurred in your Network instance.
+
+        Merges initiated by Veeva OpenData on a master instance are included if the surviving and losing records of the merge have been downloaded to your instance.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#RetrieveMerges
+
+        """
+        return self.api_call(self.api_events['item']['Retrieve Merge Events'], *args, **kwargs)
+
+    def events_retrieve_unmerge (self, *args, **kwargs):
+        """
+        This API enables you to retrieve the results of unmerge events that occurred in your Network instance.
+
+        Unmerges include events that occurred in your Network instance; only customer (gray) records are reported.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#RetrieveUnmerges
+
+        """
+        return self.api_call(self.api_events['item']['Retrieve Unmerge Events'], *args, **kwargs)
+
+    # =============================================================================
+    # Match
+    # =============================================================================
+    def match_retrieve (self, *args, **kwargs):
+        """
+        This API enables you to match data immediately for a single record using match rules from the specified Network instance.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#RetrieveMatches
+
+        """
+        return self.api_call(self.api_match['item']['Retrieve Matches'], *args, **kwargs)
+
+    # =============================================================================
+    # Suspect Match
+    # =============================================================================
+    def suspect_match_batch_process (self, *args, **kwargs):
+        """
+        This API enables enables you to process multiple unprocessed suspect matches.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#BatchProcessSuspectMatch
+
+        """
+        return self.api_call(self.api_suspect_match['item']['Batch Process Suspect Match'], *args, **kwargs)
+
+    def suspect_match_batch_create (self, *args, **kwargs):
+        """
+        This API enables enables you to create multiple suspect matches.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#BatchCreateSuspectMatch
+
+        """
+        return self.api_call(self.api_suspect_match['item']['Batch Create Suspect Match'], *args, **kwargs)
+
+    def suspect_match_batch_reject_task (self, *args, **kwargs):
+        """
+        This API enables enables you to reject multiple suspect match tasks.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#BatchRejectSuspectMatch
+
+        """
+        return self.api_call(self.api_suspect_match['item']['Batch Reject Suspect Match Task'], *args, **kwargs)
+
+    def suspect_match_batch_retrieve (self, *args, **kwargs):
+        """
+        This API enables enables you to retrieve information about multiple suspect matches.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#BatchRetrieveSuspectMatch
+
+        """
+        self.api_call(suspect_match['item']['Batch Retrieve Suspect Match'], *args, **kwargs)
+
+    # =============================================================================
+    # Retrieve Available API Versions
+    # =============================================================================
+    def retrieve_available_api_versions (self, *args, **kwargs):
+        """
+        This enables you to retrieve summary information about each API version available in Network.
+
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#RetrieveavailableAPIversions
+
+        """
+        return self.api_call(self.api_retrieve_available_api_versions, *args, **kwargs)
+    # =============================================================================
+    # Search
+    # =============================================================================
+    def search (self, *args, **kwargs):
+        """
+        Search calls enable you to construct simple, yet powerful searches to retrieve data from Network.
+
+        Calls through the Search API pass a query string in an expression that specifies the search text and specific parameters to get the intended set of entities from Network. Search results are ranked according to closeness to the search terms specified.
+        
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#search
+        
+        """
+        return self.api_call(self.api_search, *args, **kwargs)
+    # =============================================================================
+    # System Settings
+    # =============================================================================
+    def system_settings_retrieve (self):
+        """
+        This API enables you to retrieve the value for the geolocation system setting.
+
+        Currently only api.search.geolocation.countries is supported.
+        
+        Documentation:
+        https://developer.veevanetwork.com/API_reference/API_reference.htm#Retrievesystemsettings
+        
+        """
+        result = requests.get(
+            url=f"{self.networkURL}/api/v26.0/systemSettings/api.search.geolocation.countries", 
+            headers=self.APIheaders).json()
+        return result
+        
+
+    # =============================================================================
+    # Utilities
+    # =============================================================================
+
+    def api_call (
+        self,
+        api: dict, 
+        body: dict = None, 
+        variables: dict = None, 
+        queries: dict = None, 
+        if_print: bool=False,  # If True, prints each component of the api call, the api call will still execute unless if_debug or if_example paramters are set to True.
+        if_debug: bool=False, # If True, the api call does not execute, but instead returns the api call as a string for debugging
+        if_example: bool=False # If True, the api call does not execute and returns examples of any body, variables, or queries.
+    ):
+
+        examples = {}
+
+        result = {
+            'api_body' : body,
+            'api_variables' : variables,
+            'api_queries' : queries
+        }
+
+        request_params = {}
+
+        def print_if(text):
+            if if_print:
+                print(text)
+
+        if api.keys().__contains__('name'):
+            print_if('\n- Name: ')
+            print_if(api['name'])
+            result['api_name'] = api['name'] ### Updating Result Name
+
+        if api.keys().__contains__('protocolProfileBehavior'):
+            print_if('\n- protocolProfileBehavior: ')
+            if api['protocolProfileBehavior'].keys().__contains__('disableBodyPruning'):
+                print_if('- disableBodyPruning: ')
+                print_if(api['protocolProfileBehavior']['disableBodyPruning'])
+                result['api_protocolProfileBehavior_disableBodyPruning'] = api['protocolProfileBehavior']['disableBodyPruning'] ### Updating Result disableBodyPruning
+
+        if api.keys().__contains__('request'):
+
+            ### =============================================================================
+            ### Parsing Header
+            ### =============================================================================
+
+            if api['request'].keys().__contains__('header'):
+                if isinstance(api['request']['header'], dict):
+                    print_if("\n- Request header keys: ")
+                    print_if(api['request']['header'].keys())
+                    result['api_header'] = {}
+                    request_params['headers'] = {}
+                    for header_key, header_value in api['request']['header'].items():
+                        print_if("\n- Request header key:")
+                        print_if(header_key)
+                        if isinstance(header_value, dict):
+                            if header_value.keys().__contains__('value'):
+                                result['api_header'].update({header_key: self.sub_request_params(api['request']['header'][header_key]['value'])}) ### Updating Result API Header
+                                request_params['headers'].update({header_key: self.sub_request_params(api['request']['header'][header_key]['value'])}) ### Updating Request Header
+
+                            for key, value in header_value.items():
+                                print_if("\n- Request header value dict key and value:")
+                                print_if(key)
+                                print_if(value)
+                        else:
+                            print_if("Request Header Value: ")
+                            print_if(header_value)
+                            raise NetworkAPIHeaderValueNotFound
+
+            ### =============================================================================
+            ### Parsing Method
+            ### =============================================================================
+
+            if api['request'].keys().__contains__('method'):
+                print_if("\n- Request method: ")
+                print_if(api['request']['method'])
+
+                match api['request']['method']:
+                    case 'POST':
+                        result['api_method'] = requests.post # Updating Result Method
+                        print_if("\n- Request Method Post:")
+                        print_if("requests.post")
+                    case 'GET':
+                        result['api_method'] = requests.get # Updating Result Method
+                        print_if("\n- Request Method Get:")
+                        print_if("requests.get")
+                    case 'PUT':
+                        result['api_method'] = requests.put # Updating Result Method
+                        print_if("\n- Request Method Put:")
+                        print_if("requests.put")
+                    case 'DELETE':
+                        result['api_method'] = requests.delete # Updating Result Method
+                        print_if("\n- Request Method Delete:")
+                        print_if("requests.delete")
+                    case _:
+                        print_if("\n- Request Method Unknown:")
+                        print_if("unknown method")
+                        raise NetworkAPIRequestMethodNotFound
+
+            ### =============================================================================
+            ### Parsing Body
+            ### =============================================================================
+
+            if (api['request'].keys().__contains__('body') == True) and \
+                (api['request']['body'].keys().__contains__('raw') == True) and \
+                (api['request']['body']['raw'] != ''):
+                print_if("\n- Request body raw: ")
+                print_if(json.loads(api['request']['body']['raw']))
+                examples['body'] = json.loads(api['request']['body']['raw']) ### Updating Result API Body
+                # If the body parameter is not provided in an API call that requires a body. Raise Error.
+                if body is None and if_example==False:
+                    raise NetworkAPIRequestBodyNotFound
+                else:
+                    request_params['data']=json.dumps(body)
+            else:
+                print_if("\n- Request body raw: ")
+                print_if("No Body Found")
+            
+            ### =============================================================================
+            ### Parsing URL
+            ### =============================================================================
+
+            if api['request'].keys().__contains__('url'):
+                print_if("\n- Request url keys: ")
+                print_if(api['request']['url'].keys())
+
+                ### =============================================================================
+                ### Parsing Raw URL
+                ### =============================================================================
+
+                if api['request']['url'].keys().__contains__('raw'):
+                    print_if("\n- Request url raw: ")
+                    print_if(api['request']['url']['raw'])
+                    result['api_url'] = self.sub_request_params(api['request']['url']['protocol'] + "://" + api['request']['url']['host'][0] + "/" + "/".join(api['request']['url']['path'])) ### Updating Result API URL
+                    request_params['url'] = self.sub_request_params(api['request']['url']['protocol'] + "://" + api['request']['url']['host'][0] + "/" + "/".join(api['request']['url']['path'])) ### Updating Request URL
+                else:
+                    raise NetworkAPIRequestURLNotFound
+
+                
+                ### =============================================================================
+                ### Parsing URL Protocol
+                ### =============================================================================
+                
+                if api['request']['url'].keys().__contains__('protocol'):
+                    print_if("\n- Request url protocol: ")
+                    # always "https"
+                    print_if(api['request']['url']['protocol'])
+
+                ### =============================================================================
+                ### Parsing URL Host
+                ### =============================================================================
+                
+                if api['request']['url'].keys().__contains__('host'):
+                    print_if("\n- Request url host: ")
+                    # always ['{{DNS}}]
+                    print_if(api['request']['url']['host'][0])
+
+                ### =============================================================================
+                ### Parsing URL Path
+                ### =============================================================================
+
+                if api['request']['url'].keys().__contains__('path'):
+                    print_if("\n- Request url path: ")
+                    # A list of path components. i.e. ['api', '{{version}}', 'hcos', ':vid_key', 'addresses', ':address_key', 'custom_keys']
+                    print_if(api['request']['url']['path'])
+
+                ### =============================================================================
+                ### Parsing URL Variable
+                ### =============================================================================
+
+                if api['request']['url'].keys().__contains__('variable'):
+                    if variables is None and if_example==False:
+                        raise NetworkAPIRequestVariableNotFound
+                    elif if_example==False:
+                        for variable in variables.keys():
+                            result['api_url'] = result['api_url'].replace(":" + variable, variables[variable]['value'])
+                            request_params['url'] = request_params['url'].replace(":" + variable, variables[variable]['value'])
+
+                    if isinstance(api['request']['url']['variable'], dict):
+                        print_if("\n- Request url variable keys: ")
+                        print_if(api['request']['url']['variable'].keys())
+                        variables: dict = api['request']['url']['variable']
+                        examples['variables'] = variables ### Updating Result API URL Variable Examples
+                        
+                        for key, value in variables.items():
+                            if isinstance(value, dict):
+                                print_if("\n- Request url variable key and value dict: ")
+                                print_if(key)
+                                print_if(value)
+                            else:
+                                print_if("\n- Request url variable value: ") 
+                                print_if(str(value))
+
+                ### =============================================================================
+                ### Parsing URL Query
+                ### =============================================================================
+
+                if api['request']['url'].keys().__contains__('query'):
+                    if queries is None and if_example==False:
+                        raise NetworkAPIRequestQueryNotFound
+                    elif if_example==False:
+                        result['api_url'] = result['api_url'] + '?'
+                        request_params['url'] = request_params['url'] + '?'
+                        for key, value in queries.items():
+                            if result['api_url'][-1] == '?':
+                                result['api_url'] = result['api_url'] + key + '=' + value['value']
+                                request_params['url'] = request_params['url'] + key + '=' + value['value']
+                            else:
+                                result['api_url'] = result['api_url'] + '&' + key + '=' + value['value']
+                                request_params['url'] = request_params['url'] + '&' + key + '=' + value['value']
+
+                    print_if("\n- Request url query keys: ")
+                    print_if(api['request']['url']['query'].keys())
+                    queries: dict = api['request']['url']['query'] 
+                    examples['query'] = queries ### Updating Result API URL Query Examples
+                    for key, value in queries.items():
+                        print_if("\n- Request url query key and value: ")
+                        if isinstance(value, dict):
+                            print_if(key)
+                            print_if(value)
+                        else:
+                            print_if(str(value))
+
+            ### =============================================================================
+            ### Parsing Description
+            ### =============================================================================
+
+            if api['request'].keys().__contains__('description'):
+                print_if("\n- Request Description: ")
+                print_if(api['request']['description'])
+                examples['description'] = api['request']['description'] ### Updating Description
+
+        if api.keys().__contains__('response'):
+            print_if(api['response'])
+
+        if (not if_debug) & (not if_example) & (result.keys().__contains__('api_method')):
+            response = result['api_method'](**request_params)
+
+        if if_debug & if_example:
+            return result, examples, request_params
+        if if_debug:
+            return result, request_params
+        if if_example:
+            return examples
+        return response
+
+
+    @staticmethod
+    def list_of_dicts_to_dict(list_of_dict: list, key) -> dict:
+        """
+        Function takes a list of dicts and returns a single dict.
+
+        Parameters:
+        list_of_dict: list of dicts, i.e. [{'key1': 'value1', 'key2': 'value2'}, {'key1': 'value1', 'key2': 'value2'}]
+        key (str): key to use for the dict. i.e. 'key1'
+            in our example, [{'key1': 'value1', 'key2': 'value2'}, {'key1': 'value1', 'key2': 'value2'}]
+            The output dictionary would have value1, value2 as the keys:
+            {'value1': {'key1': 'value1', 'key2': 'value2'}, 'value2': {'key1': 'value1', 'key2': 'value2'}}
+
+        """
+        obj_dict = {}
+        __empty = [obj_dict.update({x[key]: x}) for x in list_of_dict]
+        return obj_dict
+
+    @staticmethod
+    def cartesian_join(pd1, pd2):
+        df1 = pd1.copy()
+        df2 = pd2.copy()
+        df1.reset_index()
+        df2.reset_index()
+        df1['cartesian_join_key'] = 1
+        df2['cartesian_join_key'] = 1
+        result = pd.merge(df1, df2, on ='cartesian_join_key').drop(labels="cartesian_join_key", axis=1)
+        return result
+        
+    def sub_request_params (self, request: str) -> str:
+        substitutions_dict = {
+            '{{AUTHORIZATION}}': self.APIheaders['authorization'],
+            '{{DNS}}': self.network_DNS,
+            '{{version}}': self.LatestAPIversion
+        }
+        for key, value in substitutions_dict.items():
+            request = request.replace(key, value)
+        return request
+    
+    def __parse_network_api_json(self, network_api: dict):
+        output = {}
+        for key, value in network_api.items():
+            if isinstance(value, dict):
+                output[key] = self.__parse_network_api_json(value)
+            elif isinstance(value, list):
+                first_key_set = set()
+                for item in value:
+                    if isinstance(item, dict):
+                        first_key_set.add(list(item.keys())[0])
+                if len(first_key_set) == 1:
+                    output[key] = self.__parse_network_api_json(self.list_of_dicts_to_dict(value, list(first_key_set)[0]))
+                else:
+                    output[key] = value
+            else:
+                output[key] = value
         return output
```

### Comparing `veevatools-0.0.95/veevatools.egg-info/SOURCES.txt` & `veevatools-0.0.96/veevatools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `veevatools-0.0.95/veevavault/veevavault.py` & `veevatools-0.0.96/veevavault/veevavault.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,224 +1,224 @@
-from sys import platform
-import requests
-import pandas as pd
-import os
-import json
-from urllib.parse import urlparse
-from typing import List
-
-# Async
-import asyncio
-from functools import wraps, partial
-
-
-def async_wrap(func):
-    @wraps(func)
-    async def run(*args, loop=None, executor=None, **kwargs):
-        if loop is None:
-            loop = asyncio.get_event_loop()
-        pfunc = partial(func, *args, **kwargs)
-        return await loop.run_in_executor(executor, pfunc)
-    return run 
-
-
-class Vv:
-    def __init__(self):
-        self.vaultURL = None
-        self.vaultUserName = None
-        self.vaultPassword = None
-        self.vaultConnection = None
-        self.sessionId = None
-        self.vaultId: str = None
-        self.vaultDNS: str = None
-        self.APIheaders = None
-        self.APIversionList = []
-        self.LatestAPIversion = 'v21.3'
-#         self.vaultObjects = None
-#         self.all_references_metadata = None
-#         self.all_references_names = None
-#         self.vault_references_all = None
-
-
-
-    def authenticate(self, 
-                     vaultURL=None, 
-                     vaultUserName=None, 
-                     vaultPassword=None, 
-                     sessionId=None,
-                     vaultId=None,
-                     if_return=False, *args, **kwargs):
-        """
-        TODO: Docs
-        """
-
-        
-        self.vaultURL = self.vaultURL if vaultURL is None else vaultURL
-        self.vaultUserName = self.vaultUserName if vaultUserName is None else vaultUserName
-        self.vaultPassword = self.vaultPassword if vaultPassword is None else vaultPassword
-        self.sessionId = self.sessionId if sessionId is None else sessionId
-        self.vaultId = self.vaultId if vaultId is None else vaultId
-        
-        url_parse = urlparse(self.vaultURL)
-        if len(url_parse.scheme) == 0:
-            self.network_protocol = 'https'
-            if len(url_parse.path) > 0:
-                self.vaultDNS = url_parse.path
-                self.vaultURL = self.network_protocol + '://' + url_parse.path
-
-        if len(url_parse.scheme) > 0:
-            self.network_protocol = url_parse.scheme
-            if len(url_parse.netloc) > 0:
-                self.vaultDNS = url_parse.netloc
-                self.vaultURL = url_parse.scheme + '://' + url_parse.netloc
-
-        if (self.vaultURL is None) or (len(self.vaultURL) == 0):
-            raise Exception('vaultURL is required')
-        
-        if (self.vaultUserName and self.vaultPassword and self.vaultURL):
-            pload = {'username': self.vaultUserName,'password': self.vaultPassword}
-            self.vaultConnection = requests.post(f'{self.vaultURL}/api/{self.LatestAPIversion}/auth',data = pload)
-            if self.vaultConnection.json()['responseStatus'] == 'FAILURE':
-                exceptionMessage = ""
-                exceptionMessage += "Error: " + self.vaultConnection.json()['responseMessage'] + "\n"
-                exceptionMessage += self.vaultConnection.json()['errorType'] + "\n"
-                for error in self.vaultConnection.json()['errors']:
-                    exceptionMessage += error['type'] + ": " + error['message'] + "\n"
-                raise Exception(exceptionMessage)
-            
-            self.sessionId = self.vaultConnection.json()['sessionId']
-            self.vaultId = self.vaultConnection.json()['vaultId']
-            
-        self.APIheaders = {'Authorization': self.sessionId}
-        self.APIversionList = []
-        
-        # Error checking whether the required parameters are passed in
-        # The check happens here because this is where all the self assignments has completed
-        if (not (self.vaultId and self.sessionId and self.vaultURL)) and (not (self.vaultUserName and self.vaultPassword and  self.vaultURL)):
-            raise Exception("Please provide either vaultId, sessionId and vaultURL or vaultUserName, vaultPassword and vaultURL")
-        
-        for API in requests.get(self.vaultURL +'/api', headers=self.APIheaders).json()['values'].keys():
-            self.APIversionList.append(float(API.replace("v", "")))
-        self.APIversionList.sort()
-        self.LatestAPIversion = "v" + str(self.APIversionList[-1])
-        
-        if if_return:
-            return {'vaultURL':self.vaultURL, 
-                    'vaultUserName':self.vaultUserName, 
-                    'vaultPassword':self.vaultPassword, 
-                    'vaultConnection':self.vaultConnection, 
-                    'sessionId':self.sessionId, 
-                    'APIheaders':self.APIheaders, 
-                    'APIversionList':self.APIversionList, 
-                    'LatestAPIversion':self.LatestAPIversion}
-            
-            
-    def query(self, query):
-        url = f"{self.vaultURL}/api/{self.LatestAPIversion}/query"
-        
-        h = {
-        "X-VaultAPI-DescribeQuery":"true",
-        "Content-Type":"application/x-www-form-urlencoded",
-            "Accept": "application/json",
-            "Authorization": self.sessionId
-        }
-        params = {
-        "q":query
-        }
-
-        r = requests.get(url, headers=h, params=params).json()
-
-        if r['responseStatus'] == 'FAILURE':
-            raise Exception(r['errors'])
-        else:
-            r = pd.DataFrame(r['data'])
-        
-        return r
-    
-    def bulk_query(self, query):
-        url = f"{self.vaultURL}/api/{self.LatestAPIversion}/query"
-        
-        h = {
-        "X-VaultAPI-DescribeQuery":"true",
-        "Content-Type":"application/x-www-form-urlencoded",
-            "Accept": "application/json",
-            "Authorization": self.sessionId
-        }
-        params = {
-        "q":query
-        }
-
-        r = requests.get(url, headers=h, params=params).json()
-
-        if r['responseStatus'] == 'FAILURE':
-            raise Exception(r['errors'])
-        
-        output = pd.DataFrame(r['data'])
-        
-        try:
-            next_page_url = r['responseDetails']['next_page'][:-4]
-            more_pages = True
-            page_count = 1000
-            
-            while more_pages:
-                r = pd.DataFrame(requests.get(f"{self.vaultURL}"+ next_page_url+ str(page_count), headers=h).json()['data'])
-                if len(r) == 0:
-                    more_pages = False
-                else:
-                    output = pd.concat([output,r],ignore_index=True).copy()
-                    page_count += 1000
-        except:
-            pass
-        
-        return output
-    
-    def object_field_metadata(self, object_api_name):
-        url = f"{self.vaultURL}/api/{self.LatestAPIversion}/metadata/vobjects/{object_api_name}"
-        r = requests.get(url, headers = self.APIheaders).json()['object']['fields']
-        return pd.DataFrame(r)
-    
-    def describe_objects(self):
-        url = f"{self.vaultURL}/api/{self.LatestAPIversion}/metadata/vobjects"
-        r = requests.get(url, headers = self.APIheaders).json()['objects']
-        return pd.DataFrame(r).sort_values(by='name')
-    
-    def retrieve_picklist_values(self, picklist_name):
-        """
-        Note: This is not the picklist field's API name, but the picklist (to which the picklist field looks up to) API name.
-        For example, the picklist field "specialty_1__v", "specialty_2__v" and "specialty_3__v" all look up to the picklist "specialty__v".
-        """
-        url = f"{self.vaultURL}/api/{self.LatestAPIversion}/objects/picklists/{picklist_name}"
-        r = requests.get(url, headers = self.APIheaders).json()
-        if r['responseStatus'] == 'SUCCESS':
-            if 'picklistValues' in r.keys():
-                result = pd.DataFrame(r['picklistValues'])
-                result['picklist_api_name'] = picklist_name
-                return result
-            else:
-                print(f"Warning: Picklist {picklist_name} does not contain any values.")
-                result = pd.DataFrame(columns=['name','label','picklist_api_name'])
-                return result
-        else:
-            raise Exception(r['errors'][0]['type'] + ": " + r['errors'][0]['message'])
-    
-    async def async_bulk_retrieve_picklist_values(self, queries: List[str]) -> pd.DataFrame:
-        """_summary_: This function is the async version of the retrieve_picklist_values function. It is used to retrieve multiple picklist values in parallel.
-
-        Args:
-            queries (List[str]): List of picklist API names
-
-        Returns:
-            _type_: pd.DataFrame
-        """
-        async_queries = async_wrap(self.retrieve_picklist_values)
-        result_list = await asyncio.gather(*[async_queries(query) for query in queries])
-        result_length = 0
-        for result in result_list:
-            result_length += len(result)
-        
-        if result_length > 0:
-            result = pd.concat(result_list, ignore_index=True)
-        else:
-            result = pd.DataFrame(columns=['name','label','picklist_api_name'])
-            
-        return result
+from sys import platform
+import requests
+import pandas as pd
+import os
+import json
+from urllib.parse import urlparse
+from typing import List
+
+# Async
+import asyncio
+from functools import wraps, partial
+
+
+def async_wrap(func):
+    @wraps(func)
+    async def run(*args, loop=None, executor=None, **kwargs):
+        if loop is None:
+            loop = asyncio.get_event_loop()
+        pfunc = partial(func, *args, **kwargs)
+        return await loop.run_in_executor(executor, pfunc)
+    return run 
+
+
+class Vv:
+    def __init__(self):
+        self.vaultURL = None
+        self.vaultUserName = None
+        self.vaultPassword = None
+        self.vaultConnection = None
+        self.sessionId = None
+        self.vaultId: str = None
+        self.vaultDNS: str = None
+        self.APIheaders = None
+        self.APIversionList = []
+        self.LatestAPIversion = 'v21.3'
+#         self.vaultObjects = None
+#         self.all_references_metadata = None
+#         self.all_references_names = None
+#         self.vault_references_all = None
+
+
+
+    def authenticate(self, 
+                     vaultURL=None, 
+                     vaultUserName=None, 
+                     vaultPassword=None, 
+                     sessionId=None,
+                     vaultId=None,
+                     if_return=False, *args, **kwargs):
+        """
+        TODO: Docs
+        """
+
+        
+        self.vaultURL = self.vaultURL if vaultURL is None else vaultURL
+        self.vaultUserName = self.vaultUserName if vaultUserName is None else vaultUserName
+        self.vaultPassword = self.vaultPassword if vaultPassword is None else vaultPassword
+        self.sessionId = self.sessionId if sessionId is None else sessionId
+        self.vaultId = self.vaultId if vaultId is None else vaultId
+        
+        url_parse = urlparse(self.vaultURL)
+        if len(url_parse.scheme) == 0:
+            self.network_protocol = 'https'
+            if len(url_parse.path) > 0:
+                self.vaultDNS = url_parse.path
+                self.vaultURL = self.network_protocol + '://' + url_parse.path
+
+        if len(url_parse.scheme) > 0:
+            self.network_protocol = url_parse.scheme
+            if len(url_parse.netloc) > 0:
+                self.vaultDNS = url_parse.netloc
+                self.vaultURL = url_parse.scheme + '://' + url_parse.netloc
+
+        if (self.vaultURL is None) or (len(self.vaultURL) == 0):
+            raise Exception('vaultURL is required')
+        
+        if (self.vaultUserName and self.vaultPassword and self.vaultURL):
+            pload = {'username': self.vaultUserName,'password': self.vaultPassword}
+            self.vaultConnection = requests.post(f'{self.vaultURL}/api/{self.LatestAPIversion}/auth',data = pload)
+            if self.vaultConnection.json()['responseStatus'] == 'FAILURE':
+                exceptionMessage = ""
+                exceptionMessage += "Error: " + self.vaultConnection.json()['responseMessage'] + "\n"
+                exceptionMessage += self.vaultConnection.json()['errorType'] + "\n"
+                for error in self.vaultConnection.json()['errors']:
+                    exceptionMessage += error['type'] + ": " + error['message'] + "\n"
+                raise Exception(exceptionMessage)
+            
+            self.sessionId = self.vaultConnection.json()['sessionId']
+            self.vaultId = self.vaultConnection.json()['vaultId']
+            
+        self.APIheaders = {'Authorization': self.sessionId}
+        self.APIversionList = []
+        
+        # Error checking whether the required parameters are passed in
+        # The check happens here because this is where all the self assignments has completed
+        if (not (self.vaultId and self.sessionId and self.vaultURL)) and (not (self.vaultUserName and self.vaultPassword and  self.vaultURL)):
+            raise Exception("Please provide either vaultId, sessionId and vaultURL or vaultUserName, vaultPassword and vaultURL")
+        
+        for API in requests.get(self.vaultURL +'/api', headers=self.APIheaders).json()['values'].keys():
+            self.APIversionList.append(float(API.replace("v", "")))
+        self.APIversionList.sort()
+        self.LatestAPIversion = "v" + str(self.APIversionList[-1])
+        
+        if if_return:
+            return {'vaultURL':self.vaultURL, 
+                    'vaultUserName':self.vaultUserName, 
+                    'vaultPassword':self.vaultPassword, 
+                    'vaultConnection':self.vaultConnection, 
+                    'sessionId':self.sessionId, 
+                    'APIheaders':self.APIheaders, 
+                    'APIversionList':self.APIversionList, 
+                    'LatestAPIversion':self.LatestAPIversion}
+            
+            
+    def query(self, query):
+        url = f"{self.vaultURL}/api/{self.LatestAPIversion}/query"
+        
+        h = {
+        "X-VaultAPI-DescribeQuery":"true",
+        "Content-Type":"application/x-www-form-urlencoded",
+            "Accept": "application/json",
+            "Authorization": self.sessionId
+        }
+        params = {
+        "q":query
+        }
+
+        r = requests.get(url, headers=h, params=params).json()
+
+        if r['responseStatus'] == 'FAILURE':
+            raise Exception(r['errors'])
+        else:
+            r = pd.DataFrame(r['data'])
+        
+        return r
+    
+    def bulk_query(self, query):
+        url = f"{self.vaultURL}/api/{self.LatestAPIversion}/query"
+        
+        h = {
+        "X-VaultAPI-DescribeQuery":"true",
+        "Content-Type":"application/x-www-form-urlencoded",
+            "Accept": "application/json",
+            "Authorization": self.sessionId
+        }
+        params = {
+        "q":query
+        }
+
+        r = requests.get(url, headers=h, params=params).json()
+
+        if r['responseStatus'] == 'FAILURE':
+            raise Exception(r['errors'])
+        
+        output = pd.DataFrame(r['data'])
+        
+        try:
+            next_page_url = r['responseDetails']['next_page'][:-4]
+            more_pages = True
+            page_count = 1000
+            
+            while more_pages:
+                r = pd.DataFrame(requests.get(f"{self.vaultURL}"+ next_page_url+ str(page_count), headers=h).json()['data'])
+                if len(r) == 0:
+                    more_pages = False
+                else:
+                    output = pd.concat([output,r],ignore_index=True).copy()
+                    page_count += 1000
+        except:
+            pass
+        
+        return output
+    
+    def object_field_metadata(self, object_api_name):
+        url = f"{self.vaultURL}/api/{self.LatestAPIversion}/metadata/vobjects/{object_api_name}"
+        r = requests.get(url, headers = self.APIheaders).json()['object']['fields']
+        return pd.DataFrame(r)
+    
+    def describe_objects(self):
+        url = f"{self.vaultURL}/api/{self.LatestAPIversion}/metadata/vobjects"
+        r = requests.get(url, headers = self.APIheaders).json()['objects']
+        return pd.DataFrame(r).sort_values(by='name')
+    
+    def retrieve_picklist_values(self, picklist_name):
+        """
+        Note: This is not the picklist field's API name, but the picklist (to which the picklist field looks up to) API name.
+        For example, the picklist field "specialty_1__v", "specialty_2__v" and "specialty_3__v" all look up to the picklist "specialty__v".
+        """
+        url = f"{self.vaultURL}/api/{self.LatestAPIversion}/objects/picklists/{picklist_name}"
+        r = requests.get(url, headers = self.APIheaders).json()
+        if r['responseStatus'] == 'SUCCESS':
+            if 'picklistValues' in r.keys():
+                result = pd.DataFrame(r['picklistValues'])
+                result['picklist_api_name'] = picklist_name
+                return result
+            else:
+                print(f"Warning: Picklist {picklist_name} does not contain any values.")
+                result = pd.DataFrame(columns=['name','label','picklist_api_name'])
+                return result
+        else:
+            raise Exception(r['errors'][0]['type'] + ": " + r['errors'][0]['message'])
+    
+    async def async_bulk_retrieve_picklist_values(self, queries: List[str]) -> pd.DataFrame:
+        """_summary_: This function is the async version of the retrieve_picklist_values function. It is used to retrieve multiple picklist values in parallel.
+
+        Args:
+            queries (List[str]): List of picklist API names
+
+        Returns:
+            _type_: pd.DataFrame
+        """
+        async_queries = async_wrap(self.retrieve_picklist_values)
+        result_list = await asyncio.gather(*[async_queries(query) for query in queries])
+        result_length = 0
+        for result in result_list:
+            result_length += len(result)
+        
+        if result_length > 0:
+            result = pd.concat(result_list, ignore_index=True)
+        else:
+            result = pd.DataFrame(columns=['name','label','picklist_api_name'])
+            
+        return result
```

