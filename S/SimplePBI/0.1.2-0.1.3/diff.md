# Comparing `tmp/SimplePBI-0.1.2-py3-none-any.whl.zip` & `tmp/SimplePBI-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 48796 bytes, number of entries: 20
+Zip file size: 49794 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat      643 b- defN 22-Sep-15 17:59 simplepbi/__init__.py
--rw-rw-rw-  2.0 fat    86402 b- defN 23-Feb-14 22:06 simplepbi/admin/__init__.py
+-rw-rw-rw-  2.0 fat    86420 b- defN 23-May-08 15:34 simplepbi/admin/__init__.py
 -rw-rw-rw-  2.0 fat     9878 b- defN 22-Sep-15 17:56 simplepbi/apps/__init__.py
 -rw-rw-rw-  2.0 fat    15534 b- defN 22-Sep-15 17:56 simplepbi/capacities/__init__.py
 -rw-rw-rw-  2.0 fat    17252 b- defN 22-Sep-15 17:56 simplepbi/dashboards/__init__.py
 -rw-rw-rw-  2.0 fat    15322 b- defN 22-Sep-15 17:56 simplepbi/dataflows/__init__.py
--rw-rw-rw-  2.0 fat    55768 b- defN 22-Sep-15 17:56 simplepbi/datasets/__init__.py
+-rw-rw-rw-  2.0 fat    58028 b- defN 23-Feb-22 18:07 simplepbi/datasets/__init__.py
 -rw-rw-rw-  2.0 fat    16099 b- defN 22-Sep-15 17:56 simplepbi/gateways/__init__.py
 -rw-rw-rw-  2.0 fat    14147 b- defN 22-Sep-15 17:57 simplepbi/groups/__init__.py
--rw-rw-rw-  2.0 fat    22377 b- defN 23-Jan-30 23:57 simplepbi/imports/__init__.py
+-rw-rw-rw-  2.0 fat    24405 b- defN 23-Apr-27 16:15 simplepbi/imports/__init__.py
 -rw-rw-rw-  2.0 fat    24126 b- defN 22-Sep-15 17:57 simplepbi/pipelines/__init__.py
--rw-rw-rw-  2.0 fat    44427 b- defN 22-Sep-15 17:57 simplepbi/reports/__init__.py
+-rw-rw-rw-  2.0 fat    44427 b- defN 23-Mar-10 18:36 simplepbi/reports/__init__.py
 -rw-rw-rw-  2.0 fat    12740 b- defN 22-Sep-15 17:57 simplepbi/scorecards/__init__.py
 -rw-rw-rw-  2.0 fat     4093 b- defN 22-Sep-15 17:57 simplepbi/token/__init__.py
--rw-rw-rw-  2.0 fat     3451 b- defN 22-Sep-15 17:57 simplepbi/utils/__init__.py
--rw-rw-rw-  2.0 fat     1072 b- defN 23-Feb-14 22:14 SimplePBI-0.1.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    10491 b- defN 23-Feb-14 22:14 SimplePBI-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Feb-14 22:14 SimplePBI-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Feb-14 22:14 SimplePBI-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1694 b- defN 23-Feb-14 22:14 SimplePBI-0.1.2.dist-info/RECORD
-20 files, 355623 bytes uncompressed, 46052 bytes compressed:  87.1%
+-rw-rw-rw-  2.0 fat     3457 b- defN 23-May-08 15:36 simplepbi/utils/__init__.py
+-rw-rw-rw-  2.0 fat     1072 b- defN 23-May-08 16:27 SimplePBI-0.1.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    11372 b- defN 23-May-08 16:27 SimplePBI-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-08 16:27 SimplePBI-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-May-08 16:27 SimplePBI-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1694 b- defN 23-May-08 16:27 SimplePBI-0.1.3.dist-info/RECORD
+20 files, 360811 bytes uncompressed, 47050 bytes compressed:  87.0%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: simplepbi/token/__init__.py
 Comment: 
 
 Filename: simplepbi/utils/__init__.py
 Comment: 
 
-Filename: SimplePBI-0.1.2.dist-info/LICENSE
+Filename: SimplePBI-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: SimplePBI-0.1.2.dist-info/METADATA
+Filename: SimplePBI-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: SimplePBI-0.1.2.dist-info/WHEEL
+Filename: SimplePBI-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: SimplePBI-0.1.2.dist-info/top_level.txt
+Filename: SimplePBI-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: SimplePBI-0.1.2.dist-info/RECORD
+Filename: SimplePBI-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simplepbi/admin/__init__.py

```diff
@@ -804,15 +804,15 @@
         contar = 0    
         try:
             while(ban):        
                 res = requests.get(url, headers=headers)
                 if return_pandas:
                     js = json.dumps(res.json()["ArtifactAccessEntities"])
                     df = pd.read_json(js)
-                    df_total = df_total.append(df, sort=True, ignore_index=True)
+                    df_total = pd.concat([df_total, df], sort=True, ignore_index=True)
                     print("Building dataframe iteration: ", str(contar))
                 else:
                     if res.json()["ArtifactAccessEntities"]:
                         list_total.extend(res.json()["ArtifactAccessEntities"])
                         #append_value(dict_total, "ArtifactAccessEntities", res.json()["ArtifactAccessEntities"])
                         print("Building dict iteration: ", str(contar))
                 print(res.status_code)
@@ -1425,15 +1425,15 @@
                 res = requests.get(url,
                     headers={'Content-Type': 'application/json', "Authorization": "Bearer {}".format(self.token)}
                     )
                 if return_pandas:
                     js = json.dumps(res.json()["activityEventEntities"])
                     df = pd.read_json(js)
                     #print(df.head())
-                    df_total = df_total.append(df, sort=True, ignore_index=True)
+                    df_total = pd.concat([df_total, df], sort=True, ignore_index=True)
                     print("Building dataframe iteration: ", str(contar))
                     #print(df_total.head())
                 else:
                     if res.json()["activityEventEntities"]:                
                         #append_value(dict_total, "activityEventEntities", res.json()["activityEventEntities"][0])
                         list_total.extend(res.json()["activityEventEntities"])
                         print("Building dict iteration: ", str(contar))
@@ -1491,15 +1491,15 @@
            'ModelsSnapshots', 'ObjectId', 'Operation', 'OrganizationId',
            'RecordType', 'RefreshType', 'ReportId', 'ReportName', 'ReportType',
            'RequestId', 'TableName', 'UserAgent', 'UserId', 'UserKey', 'UserType',
            'WorkSpaceName', 'Workload', 'WorkspaceId'])
         # Loop last 30 days appending the result in a single dataframe
         for i in last_30_days:
             df_temp = self.get_activity_events_preview(i, return_pandas=True)
-            df = df.append(df_temp)
+            df = pd.concat([df, df_temp])
             print("\nStarting date: ", i, "...\n")
         return df
             
     def get_modified_workspaces_preview(self, excludePersonalWorkspaces=True, modifiedSince=None):
         """Gets a list of workspace IDs in the organization. This is a preview API call.
         *** THIS REQUEST IS IN PREVIEW IN SIMPLEPBI ***
         ### Parameters
```

## simplepbi/datasets/__init__.py

```diff
@@ -1060,14 +1060,65 @@
             
             res = requests.patch(url, json.dumps(body), headers = headers)
             res.raise_for_status()
             return res
         except requests.exceptions.HTTPError as ex:
             print("HTTP Error: ", ex, "\nText: ", ex.response.text)
         except requests.exceptions.RequestException as e:
+            print("Request exception: ", e)
+            
+    def update_datasources_in_group_preview(self, workspace_id, dataset_id, updateDetails):
+        """Updates the data sources of the specified dataset from the specified workspace.
+        Only these data sources are supported: SQL Server, Azure SQL Server, Azure Analysis Services, Azure Synapse, OData, SharePoint, Teradata, and SAP HANA.
+        ### Parameters
+        ----
+        workspace_id: str uuid
+            The Power Bi workspace id. You can take it from PBI Service URL
+        dataset_id: str uuid
+            The Power Bi Dataset id. You can take it from PBI Service URL
+        ### Request Body (PLEASE READ THE DOCS)
+        ----
+        UpdateDetails[]: list
+            A list of data source connection update requests. PLEASE READ THE DOCS
+            E.g.[
+                {
+                  "datasourceSelector": {
+                    "datasourceType": "Sql",
+                    "connectionDetails": {
+                      "server": "My-Sql-Server",
+                      "database": "My-Sql-Database"
+                    }
+                  },
+                  "connectionDetails": {
+                    "server": "New-Sql-Server",
+                    "database": "New-Sql-Database"
+                  }
+                }
+            ]
+        ### Returns
+        ----
+        Response object from requests library. 200 OK
+        ### Limitations
+        ----
+        Datasets created using the public XMLA endpoint aren't supported.
+        """
+        try: 
+            url= "https://api.powerbi.com/v1.0/myorg/groups/{}/datasets/{}/Default.UpdateDatasources".format(workspace_id, dataset_id)
+            body = {
+                "updateDetails": updateDetails
+            }
+                
+            headers={'Content-Type': 'application/json', "Authorization": "Bearer {}".format(self.token)}
+            
+            res = requests.post(url, json.dumps(body), headers = headers)
+            res.raise_for_status()
+            return res
+        except requests.exceptions.HTTPError as ex:
+            print("HTTP Error: ", ex, "\nText: ", ex.response.text)
+        except requests.exceptions.RequestException as e:
             print("Request exception: ", e)            
             
     def enhanced_refresh_dataset_in_group(self, workspace_id, dataset_id, objects, typeProcessing="Full", commitMode="transactional", maxParallelism=1, retryCount=1, applyRefreshPolicy=True):
         """Triggers a refresh for the specified dataset from the specified workspace.
         For Shared capacities, a maximum of eight requests per day, which includes refreshes executed using a scheduled refresh.
         ### Parameters
         ----
```

## simplepbi/imports/__init__.py

```diff
@@ -392,8 +392,45 @@
                 res = requests.post(url, data = mp_encoder, headers=headers)
                 res.raise_for_status()
                 results.append(res)
             return results
         except requests.exceptions.HTTPError as ex:
             print("HTTP Error: ", ex, "\nText: ", ex.response.text)
         except requests.exceptions.RequestException as e:
+            print("Request exception: ", e)
+            
+    def simple_import_from_devops(self, organization, project, repository_id, path, devopsKey, workspace_id):
+        '''This function will import a PBIX file from DevOps to Power BI. Only available for Pbix with size lower than 1gb
+         ### Parameters
+        ----
+        organization: str
+            The organization name in DevOps. For example: https://dev.azure.com/ibarrau/ the organization name is ibarrau
+        project: str
+            The project name in DevOps. For example: https://dev.azure.com/ibarrau/ladataweb_proj/ the project name is ladataweb_proj
+        repository_id: str
+            The repository name in DevOps. Sometimes matches the name of the repo.
+        path: str
+            The path of the file in DevOps. For example: /Prod/PBITenantOverview.pbix
+        devopsKey: str
+            The DevOps Key. You can turn it on from DevOps > User Settings > Personal Access Tokens
+        workspace_id: str uuid
+            The Power Bi workspace id. You can take it from PBI Service URL    
+        ### Returns
+        ----
+        Dict:
+            Response 200 Ok
+        '''
+        file_name = path.split("/")[-1]
+        try:
+            pbix = requests.get(url="https://dev.azure.com/{}/{}/_apis/git/repositories/{}/items?path={}&download=true&api-version=6.0".format(organization, project, repository_id, path), auth=('user', pat))
+        except requests.exceptions.HTTPError as ex:
+            print("HTTP Error: ", ex, "\nText: ", ex.response.text)
+        except requests.exceptions.RequestException as e:
+            print("Request exception: ", e)
+        try:
+            res = self.simple_import_pbix_as_parameter(workspace_id, pbix.content, file_name)
+            res.raise_for_status()
+            return res
+        except requests.exceptions.HTTPError as ex:
+            print("HTTP Error: ", ex, "\nText: ", ex.response.text)
+        except requests.exceptions.RequestException as e:
             print("Request exception: ", e)
```

## simplepbi/utils/__init__.py

```diff
@@ -98,11 +98,11 @@
         Returns the status of the scan. Succeeded means you are ready to request scans.
     """
     df_total = pd.DataFrame()
     try:        
         for group in scan_result["workspaces"]:
             df = pd.read_json(json.dumps(group[artifact]))
             df["workspaceId"] = group["id"]
-            df_total = df_total.append(df, sort=True, ignore_index=True)
+            df_total = pd.concat([df_total, df], sort=True, ignore_index=True)
         return df_total
     except Exception as e:
         print("ERROR: ", e)
```

## Comparing `SimplePBI-0.1.2.dist-info/LICENSE` & `SimplePBI-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `SimplePBI-0.1.2.dist-info/METADATA` & `SimplePBI-0.1.3.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,656 +1,711 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 5369 6d70  : 2.1.Name: Simp
-00000020: 6c65 5042 490a 5665 7273 696f 6e3a 2030  lePBI.Version: 0
-00000030: 2e31 2e32 0a53 756d 6d61 7279 3a20 5369  .1.2.Summary: Si
-00000040: 6d70 6c69 6679 2075 7361 6765 206f 6620  mplify usage of 
-00000050: 506f 7765 7220 4269 2052 6573 7420 4150  Power Bi Rest AP
-00000060: 490a 486f 6d65 2d70 6167 653a 2055 4e4b  I.Home-page: UNK
-00000070: 4e4f 574e 0a41 7574 686f 723a 2049 676e  NOWN.Author: Ign
-00000080: 6163 696f 2042 6172 7261 7520 3c69 676e  acio Barrau <ign
-00000090: 615f 6261 7272 6175 4068 6f74 6d61 696c  a_barrau@hotmail
-000000a0: 2e63 6f6d 3e2c 204d 6172 7469 6e20 5a75  .com>, Martin Zu
-000000b0: 7269 7461 203c 6d61 7274 696e 7a75 7269  rita <martinzuri
-000000c0: 7461 3140 676d 6169 6c2e 636f 6d3e 0a4c  ta1@gmail.com>.L
-000000d0: 6963 656e 7365 3a20 4d49 540a 5072 6f6a  icense: MIT.Proj
-000000e0: 6563 742d 5552 4c3a 2044 6f63 756d 656e  ect-URL: Documen
-000000f0: 7461 7469 6f6e 2c20 6874 7470 733a 2f2f  tation, https://
-00000100: 646f 6373 2e6d 6963 726f 736f 6674 2e63  docs.microsoft.c
-00000110: 6f6d 2f65 6e2d 7573 2f72 6573 742f 6170  om/en-us/rest/ap
-00000120: 692f 706f 7765 722d 6269 2f0a 5072 6f6a  i/power-bi/.Proj
-00000130: 6563 742d 5552 4c3a 2053 6179 2054 6861  ect-URL: Say Tha
-00000140: 6e6b 7321 2c20 6874 7470 733a 2f2f 7777  nks!, https://ww
-00000150: 772e 6c61 6461 7461 7765 622e 636f 6d2e  w.ladataweb.com.
-00000160: 6172 2f63 6f6e 7461 6374 6f2e 6874 6d6c  ar/contacto.html
-00000170: 0a50 726f 6a65 6374 2d55 524c 3a20 536f  .Project-URL: So
-00000180: 7572 6365 2c20 6874 7470 733a 2f2f 6769  urce, https://gi
-00000190: 7468 7562 2e63 6f6d 2f6c 6164 6174 6177  thub.com/ladataw
-000001a0: 6562 2f53 696d 706c 6550 4249 0a50 726f  eb/SimplePBI.Pro
-000001b0: 6a65 6374 2d55 524c 3a20 5472 6163 6b65  ject-URL: Tracke
-000001c0: 722c 2068 7474 7073 3a2f 2f67 6974 6875  r, https://githu
-000001d0: 622e 636f 6d2f 6c61 6461 7461 7765 622f  b.com/ladataweb/
-000001e0: 5369 6d70 6c65 5042 492f 6973 7375 6573  SimplePBI/issues
-000001f0: 0a4b 6579 776f 7264 733a 2050 6f77 6572  .Keywords: Power
-00000200: 2042 492c 5042 492c 4c61 4461 7461 5765   BI,PBI,LaDataWe
-00000210: 622c 417a 7572 652c 4461 7461 2c50 7974  b,Azure,Data,Pyt
-00000220: 686f 6e0a 506c 6174 666f 726d 3a20 554e  hon.Platform: UN
-00000230: 4b4e 4f57 4e0a 436c 6173 7369 6669 6572  KNOWN.Classifier
-00000240: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
-00000250: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000260: 203a 3a20 330a 436c 6173 7369 6669 6572   :: 3.Classifier
-00000270: 3a20 4c69 6365 6e73 6520 3a3a 204f 5349  : License :: OSI
-00000280: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
-00000290: 204c 6963 656e 7365 0a43 6c61 7373 6966   License.Classif
-000002a0: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
-000002b0: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-000002c0: 7065 6e64 656e 740a 4465 7363 7269 7074  pendent.Descript
-000002d0: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
-000002e0: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
-000002f0: 5265 7175 6972 6573 2d44 6973 743a 2072  Requires-Dist: r
-00000300: 6571 7565 7374 730a 5265 7175 6972 6573  equests.Requires
-00000310: 2d44 6973 743a 2070 616e 6461 730a 5265  -Dist: pandas.Re
-00000320: 7175 6972 6573 2d44 6973 743a 2072 6571  quires-Dist: req
-00000330: 7565 7374 732d 746f 6f6c 6265 6c74 0a0a  uests-toolbelt..
-00000340: 2320 5369 6d70 6c65 5042 490a 0a54 6869  # SimplePBI..Thi
-00000350: 7320 6973 2061 2073 696d 706c 6520 6c69  s is a simple li
-00000360: 6272 6172 7920 7468 6174 206d 616b 6573  brary that makes
-00000370: 2069 7420 6561 7379 2074 6f20 7573 6520   it easy to use 
-00000380: 7468 6520 506f 7765 7220 4269 2052 4553  the Power Bi RES
-00000390: 5420 4150 492e 204f 6e65 2064 6179 2053  T API. One day S
-000003a0: 696d 706c 6550 4249 2077 696c 6c20 636f  implePBI will co
-000003b0: 6e74 6169 6e20 616c 6c20 7468 6520 6361  ntain all the ca
-000003c0: 7465 676f 7269 6573 2069 6e20 7468 6520  tegories in the 
-000003d0: 4150 4920 2841 646d 696e 2c20 6461 7461  API (Admin, data
-000003e0: 7365 7473 2c20 7265 706f 7274 732c 2065  sets, reports, e
-000003f0: 7463 292e 0a46 6565 6c20 6672 6565 2074  tc)..Feel free t
-00000400: 6f20 6368 6563 6b20 7468 6520 646f 6320  o check the doc 
-00000410: 746f 2067 6574 2061 2064 6565 7065 7220  to get a deeper 
-00000420: 756e 6465 7273 7461 6e64 696e 6720 6f66  understanding of
-00000430: 2061 2073 7065 6369 6669 6320 7265 7175   a specific requ
-00000440: 6573 743a 2068 7474 7073 3a2f 2f64 6f63  est: https://doc
-00000450: 732e 6d69 6372 6f73 6f66 742e 636f 6d2f  s.microsoft.com/
-00000460: 656e 2d75 732f 7265 7374 2f61 7069 2f70  en-us/rest/api/p
-00000470: 6f77 6572 2d62 692f 0a3c 6272 3e57 6520  ower-bi/.<br>We 
-00000480: 6172 6520 646f 696e 6720 6f75 7220 6265  are doing our be
-00000490: 7374 2074 6f20 6d61 6b65 2074 6869 7320  st to make this 
-000004a0: 6c69 6272 6172 7920 7573 6566 756c 2066  library useful f
-000004b0: 6f72 2074 6865 2063 6f6d 6d75 6e69 7479  or the community
-000004c0: 2e20 5468 6973 2070 726f 6a65 6374 2069  . This project i
-000004d0: 7320 6e6f 7420 6120 7265 6d75 6e65 7261  s not a remunera
-000004e0: 626c 6520 6a6f 6220 666f 7220 7573 2e20  ble job for us. 
-000004f0: 4974 2773 2061 2070 7562 6c69 6320 636f  It's a public co
-00000500: 6d6d 756e 6974 7920 7072 6f6a 6563 742e  mmunity project.
-00000510: 2050 6c65 6173 6520 6265 2070 6174 6965   Please be patie
-00000520: 6e74 2069 6620 796f 7520 7375 626d 6974  nt if you submit
-00000530: 2061 6e20 6973 7375 6520 616e 6420 6974   an issue and it
-00000540: 2773 206e 6f74 2066 6978 6564 2072 6967  's not fixed rig
-00000550: 6874 2061 7761 792e 2049 7427 7320 6120  ht away. It's a 
-00000560: 7761 7920 746f 2065 7870 7265 7373 206f  way to express o
-00000570: 7572 2070 6173 7369 6f6e 206f 6620 7368  ur passion of sh
-00000580: 6172 696e 6720 6b6e 6f77 6c65 6467 652e  aring knowledge.
-00000590: 0a3c 6272 3e45 6163 6820 6361 7465 676f  .<br>Each catego
-000005a0: 7279 2069 7320 616e 204f 626a 6563 742e  ry is an Object.
-000005b0: 2054 6869 7320 6d65 616e 7320 7765 206e   This means we n
-000005c0: 6565 6420 746f 2069 6e69 7469 616c 697a  eed to initializ
-000005d0: 6520 616e 206f 626a 6563 7420 746f 2073  e an object to s
-000005e0: 7461 7274 2075 7369 6e67 2069 7473 206d  tart using its m
-000005f0: 6574 686f 6473 2e20 496e 206f 7264 6572  ethods. In order
-00000600: 2074 6f20 6372 6561 7465 2074 6865 6d20   to create them 
-00000610: 7765 206e 6565 6420 7468 6520 4265 6172  we need the Bear
-00000620: 6572 2074 6f6b 656e 2074 6861 7420 6361  er token that ca
-00000630: 6e20 6265 206f 6274 6169 6e20 6672 6f6d  n be obtain from
-00000640: 2061 2054 6f6b 656e 204f 626a 6563 742e   a Token Object.
-00000650: 200a 4c65 7427 7320 7365 6520 686f 7720   .Let's see how 
-00000660: 7765 2063 616e 2063 7265 6174 6520 616e  we can create an
-00000670: 2041 646d 696e 204f 626a 6563 7420 746f   Admin Object to
-00000680: 2074 7279 2074 6865 2072 6571 7565 7374   try the request
-00000690: 7320 696e 2074 6861 7420 6361 7465 676f  s in that catego
-000006a0: 7279 2e0a 0a60 6060 7079 7468 6f6e 0a23  ry...```python.#
-000006b0: 2049 6d70 6f72 7420 6c69 6272 6172 790a   Import library.
-000006c0: 6672 6f6d 2073 696d 706c 6570 6269 2069  from simplepbi i
-000006d0: 6d70 6f72 7420 746f 6b65 6e0a 6672 6f6d  mport token.from
-000006e0: 2073 696d 706c 6570 6269 2069 6d70 6f72   simplepbi impor
-000006f0: 7420 6164 6d69 6e0a 6060 600a 0a57 6520  t admin.```..We 
-00000700: 616c 7761 7973 206e 6565 6420 746f 2069  always need to i
-00000710: 6d70 6f72 7420 746f 6b65 6e20 6f62 6a65  mport token obje
-00000720: 6374 2074 6f20 6372 6561 7465 2074 6865  ct to create the
-00000730: 206f 626a 6563 7420 746f 2072 756e 2072   object to run r
-00000740: 6571 7565 7374 732e 2054 6865 6e20 7765  equests. Then we
-00000750: 2063 616e 2070 6963 6b20 7468 6520 6f62   can pick the ob
-00000760: 6a65 6374 206f 6620 7468 6520 506f 7765  ject of the Powe
-00000770: 7220 4269 2052 6573 7420 4150 4920 6361  r Bi Rest API ca
-00000780: 7465 676f 7279 2077 6520 6e65 6564 2e20  tegory we need. 
-00000790: 466f 7220 696e 7374 616e 6365 2022 6164  For instance "ad
-000007a0: 6d69 6e22 2e0a 5468 6520 746f 6b65 6e20  min"..The token 
-000007b0: 6361 6e20 6265 2063 7265 6174 6564 2069  can be created i
-000007c0: 6e20 7477 6f20 7761 7973 2c20 7468 6520  n two ways, the 
-000007d0: 7265 6775 6c61 7220 6175 7468 656e 7469  regular authenti
-000007e0: 6361 7469 6f6e 2061 6e64 2074 6865 2073  cation and the s
-000007f0: 6572 7669 6365 2070 7269 6e63 6970 616c  ervice principal
-00000800: 206f 6e65 2e20 4974 2064 6570 656e 6473   one. It depends
-00000810: 2077 6869 6368 206f 6e65 2079 6f75 2070   which one you p
-00000820: 6963 6b20 746f 2063 6f6d 706c 6574 6520  ick to complete 
-00000830: 7468 6520 7265 7175 6573 742e 200a 5468  the request. .Th
-00000840: 6573 6520 6172 6520 7468 6520 6e65 6365  ese are the nece
-00000850: 7373 6172 7920 6172 6775 6d65 6e74 7320  ssary arguments 
-00000860: 746f 2067 6574 2061 2074 6f6b 656e 3a0a  to get a token:.
-00000870: 2d20 7465 6e61 6e74 5f69 6420 2879 6f75  - tenant_id (you
-00000880: 2063 616e 2067 6574 2069 7420 6672 6f6d   can get it from
-00000890: 2073 7562 7363 7269 7074 696f 6e20 7265   subscription re
-000008a0: 736f 7572 6365 2069 6e20 617a 7572 6520  source in azure 
-000008b0: 706f 7274 616c 206f 7220 6173 6b20 666f  portal or ask fo
-000008c0: 7220 6974 2074 6f20 7468 6520 4954 2064  r it to the IT d
-000008d0: 6570 6172 746d 656e 7429 0a2d 2061 7070  epartment).- app
-000008e0: 5f63 6c69 656e 745f 6964 2028 796f 7572  _client_id (your
-000008f0: 2061 7070 5f69 642f 636c 6965 6e74 5f69   app_id/client_i
-00000900: 6420 6672 6f6d 2074 6865 2041 7070 2072  d from the App r
-00000910: 6567 6973 7465 7265 6420 696e 2041 7a75  egistered in Azu
-00000920: 7265 2077 6974 6820 7065 726d 6973 7369  re with permissi
-00000930: 6f6e 7320 746f 2050 6f77 6572 2042 6920  ons to Power Bi 
-00000940: 5365 7276 6963 6529 0a2d 2075 7365 726e  Service).- usern
-00000950: 616d 6520 2870 726f 6665 7373 696f 6e61  ame (professiona
-00000960: 6c20 656d 6169 6c20 6163 636f 756e 7420  l email account 
-00000970: 696e 2041 7a75 7265 2041 4429 0a2d 2070  in Azure AD).- p
-00000980: 6173 7377 6f72 6420 2870 726f 6665 7373  assword (profess
-00000990: 696f 6e61 6c20 7061 7373 776f 7264 290a  ional password).
-000009a0: 2d20 6170 705f 7365 6372 6574 5f6b 6579  - app_secret_key
-000009b0: 2028 7365 6372 6574 206b 6579 2067 656e   (secret key gen
-000009c0: 6572 6174 6564 2066 6f72 2074 6865 2063  erated for the c
-000009d0: 6c69 656e 7420 6964 290a 2d20 7573 655f  lient id).- use_
-000009e0: 7365 7276 6963 655f 7072 696e 6369 7061  service_principa
-000009f0: 6c20 2854 7275 6520 746f 2061 7468 656e  l (True to athen
-00000a00: 7469 6361 7465 2077 6974 6820 5365 7276  ticate with Serv
-00000a10: 6963 6520 5072 696e 6369 7061 6c20 616e  ice Principal an
-00000a20: 6420 4661 6c73 6520 746f 2063 6f6e 7469  d False to conti
-00000a30: 6e75 6520 7769 7468 2075 7365 7220 6372  nue with user cr
-00000a40: 6564 656e 7469 616c 7329 0a0a 0a2a 4e4f  edentials)...*NO
-00000a50: 5445 3a20 6966 2079 6f75 2077 616e 7420  TE: if you want 
-00000a60: 746f 2075 7365 2073 6572 7669 6365 2070  to use service p
-00000a70: 7269 6e63 6970 616c 2c20 6265 2073 7572  rincipal, be sur
-00000a80: 6520 746f 2068 6176 6520 796f 7572 2074  e to have your t
-00000a90: 656e 616e 7420 7265 6164 7920 666f 7220  enant ready for 
-00000aa0: 7468 6174 2e0a 3c62 723e 5265 6769 7374  that..<br>Regist
-00000ab0: 6572 2061 7070 2065 7861 6d70 6c65 3a20  er app example: 
-00000ac0: 6874 7470 733a 2f2f 626c 6f67 2e6c 6164  https://blog.lad
-00000ad0: 6174 6177 6562 2e63 6f6d 2e61 722f 706f  ataweb.com.ar/po
-00000ae0: 7374 2f31 3838 3034 3532 3237 3733 352f  st/188045227735/
-00000af0: 6765 742d 6163 6365 7373 2d74 6f6b 656e  get-access-token
-00000b00: 0a3c 6272 3e53 6572 7669 6365 2050 7269  .<br>Service Pri
-00000b10: 6e63 6970 616c 2070 6572 6d69 7373 696f  ncipal permissio
-00000b20: 6e73 2066 6f72 2061 646d 696e 2061 7069  ns for admin api
-00000b30: 3a20 6874 7470 733a 2f2f 646f 6373 2e6d  : https://docs.m
-00000b40: 6963 726f 736f 6674 2e63 6f6d 2f65 6e2d  icrosoft.com/en-
-00000b50: 7573 2f70 6f77 6572 2d62 692f 6164 6d69  us/power-bi/admi
-00000b60: 6e2f 7265 6164 2d6f 6e6c 792d 6170 6973  n/read-only-apis
-00000b70: 2d73 6572 7669 6365 2d70 7269 6e63 6970  -service-princip
-00000b80: 616c 2d61 7574 6865 6e74 6963 6174 696f  al-authenticatio
-00000b90: 6e2a 0a0a 0a60 6060 7079 7468 6f6e 0a23  n*...```python.#
-00000ba0: 2043 7265 6174 696e 6720 6f62 6a65 6374   Creating object
-00000bb0: 730a 0a23 5265 6775 6c61 7220 4c6f 6769  s..#Regular Logi
-00000bc0: 6e0a 746f 6b20 3d20 746f 6b65 6e2e 546f  n.tok = token.To
-00000bd0: 6b65 6e28 7465 6e61 6e74 5f69 642c 2061  ken(tenant_id, a
-00000be0: 7070 5f63 6c69 656e 745f 6964 2c20 7573  pp_client_id, us
-00000bf0: 6572 6e61 6d65 2c20 7061 7373 776f 7264  ername, password
-00000c00: 2c20 4e6f 6e65 2c20 7573 655f 7365 7276  , None, use_serv
-00000c10: 6963 655f 7072 696e 6369 7061 6c3d 4661  ice_principal=Fa
-00000c20: 6c73 6529 0a0a 2353 6572 7669 6365 2050  lse)..#Service P
-00000c30: 7269 6e63 6970 616c 0a74 6f6b 203d 2074  rincipal.tok = t
-00000c40: 6f6b 656e 2e54 6f6b 656e 2874 656e 616e  oken.Token(tenan
-00000c50: 745f 6964 2c20 6170 705f 636c 6965 6e74  t_id, app_client
-00000c60: 5f69 642c 204e 6f6e 652c 204e 6f6e 652c  _id, None, None,
-00000c70: 2061 7070 5f73 6563 7265 745f 6b65 792c   app_secret_key,
-00000c80: 2075 7365 5f73 6572 7669 6365 5f70 7269   use_service_pri
-00000c90: 6e63 6970 616c 3d54 7275 6529 0a0a 6164  ncipal=True)..ad
-00000ca0: 203d 2061 646d 696e 2e41 646d 696e 2874   = admin.Admin(t
-00000cb0: 6f6b 2e74 6f6b 656e 290a 6060 600a 0a41  ok.token).```..A
-00000cc0: 7320 796f 7520 6361 6e20 7365 6520 7468  s you can see th
-00000cd0: 6520 546f 6b65 6e20 6f62 6a65 6374 2063  e Token object c
-00000ce0: 6f6e 7461 696e 7320 6120 746f 6b65 6e20  ontains a token 
-00000cf0: 6174 7472 6962 7574 6520 7769 7468 2074  attribute with t
-00000d00: 6865 2042 6561 7265 7220 7573 6564 2062  he Bearer used b
-00000d10: 7920 417a 7572 6520 746f 2072 756e 2072  y Azure to run r
-00000d20: 6573 7420 6d65 7468 6f64 732e 2054 6861  est methods. Tha
-00000d30: 7420 6174 7472 6962 7574 6520 7769 6c6c  t attribute will
-00000d40: 2062 6520 7573 6572 2074 6f20 6372 6561   be user to crea
-00000d50: 7465 2074 6865 2063 6174 6567 6f72 7920  te the category 
-00000d60: 6f62 6a65 6374 7320 6c69 6b65 2061 646d  objects like adm
-00000d70: 696e 2e0a 4f6e 6365 2077 6520 6372 6561  in..Once we crea
-00000d80: 7465 206f 7572 204f 626a 6563 7420 6c69  te our Object li
-00000d90: 6b65 2061 646d 696e 2c20 7765 2063 616e  ke admin, we can
-00000da0: 2073 7461 7274 2075 7369 6e67 2074 6865   start using the
-00000db0: 2072 6571 7565 7374 7320 6164 6469 6e67   requests adding
-00000dc0: 2074 6865 2063 6f72 7265 6374 2070 6172   the correct par
-00000dd0: 616d 6574 6572 7320 6966 2074 6865 7920  ameters if they 
-00000de0: 6172 6520 6e65 6564 6564 2e0a 0a60 6060  are needed...```
-00000df0: 7079 7468 6f6e 0a23 2047 6574 7469 6e67  python.# Getting
-00000e00: 206f 626a 6563 7473 0a0a 416c 6c5f 4461   objects..All_Da
-00000e10: 7461 7365 7473 203d 2061 642e 6765 745f  tasets = ad.get_
-00000e20: 6461 7461 7365 7473 2829 0a0a 4461 7461  datasets()..Data
-00000e30: 7365 7473 5f49 6e5f 4772 6f75 7073 203d  sets_In_Groups =
-00000e40: 2061 642e 6765 745f 6461 7461 7365 7473   ad.get_datasets
-00000e50: 5f69 6e5f 6772 6f75 7028 776f 726b 7370  _in_group(worksp
-00000e60: 6163 655f 6964 290a 6060 600a 0a54 6865  ace_id).```..The
-00000e70: 206c 6962 7261 7279 2067 6574 2072 6571   library get req
-00000e80: 7565 7374 7320 7769 6c6c 2072 6574 7572  uests will retur
-00000e90: 6e20 6120 7265 7370 6f6e 7365 206f 626a  n a response obj
-00000ea0: 6563 7420 2e6a 736f 6e28 2920 7468 6174  ect .json() that
-00000eb0: 2070 7974 686f 6e20 7265 6164 7320 6974   python reads it
-00000ec0: 2061 7320 6120 4469 6374 2e0a 0a23 2320   as a Dict...## 
-00000ed0: 5072 6576 6965 7720 6d65 7468 6f64 730a  Preview methods.
-00000ee0: 5468 6572 6520 6172 6520 736f 6d65 206d  There are some m
-00000ef0: 6574 686f 6473 2069 6e20 7468 6520 636c  ethods in the cl
-00000f00: 6173 7365 7320 7468 6174 2073 7469 6c6c  asses that still
-00000f10: 206e 6565 6420 6d6f 7265 2074 6573 7469   need more testi
-00000f20: 6e67 2e20 5468 6f73 6520 7769 6c6c 2068  ng. Those will h
-00000f30: 6176 6520 6120 2270 7265 7669 6577 2220  ave a "preview" 
-00000f40: 6174 2074 6865 2065 6e64 206f 6620 7468  at the end of th
-00000f50: 6520 6e61 6d65 2e20 506c 6561 7365 206c  e name. Please l
-00000f60: 6574 2075 7320 6b6e 6f77 2069 6620 736f  et us know if so
-00000f70: 6d65 7468 696e 6720 676f 6573 2077 726f  mething goes wro
-00000f80: 6e67 2077 6974 6820 7468 6f73 652e 0a0a  ng with those...
-00000f90: 2323 2043 6f6d 706c 6578 2072 6571 7565  ## Complex reque
-00000fa0: 7374 730a 4966 2079 6f75 2077 616e 7420  sts.If you want 
-00000fb0: 746f 2067 6574 2061 2064 6565 7065 7220  to get a deeper 
-00000fc0: 6c6f 6f6b 206f 6e20 636f 6d70 6c65 7820  look on complex 
-00000fd0: 5f5f 4164 6d69 6e5f 5f20 6d65 7468 6f64  __Admin__ method
-00000fe0: 732e 200a 3c61 2068 7265 663d 2268 7474  s. .<a href="htt
-00000ff0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001000: 6c61 6461 7461 7765 622f 5369 6d70 6c65  ladataweb/Simple
-00001010: 5042 492f 626c 6f62 2f6d 6169 6e2f 4164  PBI/blob/main/Ad
-00001020: 6d69 6e5f 636f 6d70 6c65 782e 6d64 2220  min_complex.md" 
-00001030: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
-00001040: 4368 6563 6b20 7468 6973 2064 6f63 3c2f  Check this doc</
-00001050: 613e 0a0a 2323 2045 7861 6d70 6c65 206f  a>..## Example o
-00001060: 6620 6f75 7220 616d 617a 696e 6720 756e  f our amazing un
-00001070: 6971 7565 2072 6571 7565 7374 730a 2d20  ique requests.- 
-00001080: 6765 745f 6f72 7068 616e 5f64 6174 6166  get_orphan_dataf
-00001090: 6c6f 7773 5f70 7265 7669 6577 0a2d 2073  lows_preview.- s
-000010a0: 696d 706c 655f 696d 706f 7274 5f70 6269  imple_import_pbi
-000010b0: 780a 2d20 7369 6d70 6c65 5f69 6d70 6f72  x.- simple_impor
-000010c0: 745f 7062 6978 5f61 735f 7061 7261 6d65  t_pbix_as_parame
-000010d0: 7465 720a 2d20 7369 6d70 6c65 5f69 6d70  ter.- simple_imp
-000010e0: 6f72 745f 7062 6978 5f66 6f6c 6465 725f  ort_pbix_folder_
-000010f0: 696e 5f67 726f 7570 5f70 7265 7669 6577  in_group_preview
-00001100: 0a2d 2073 696d 706c 655f 636f 7079 5f72  .- simple_copy_r
-00001110: 6570 6f72 7473 5f62 6574 7765 656e 5f67  eports_between_g
-00001120: 726f 7570 730a 2d20 656e 6861 6e63 6564  roups.- enhanced
-00001130: 5f72 6566 7265 7368 5f64 6174 6173 6574  _refresh_dataset
-00001140: 5f69 6e5f 6772 6f75 700a 2d20 6765 745f  _in_group.- get_
-00001150: 6163 7469 7669 7479 5f65 7665 6e74 735f  activity_events_
-00001160: 7072 6576 6965 7720 2861 6c72 6561 6479  preview (already
-00001170: 2069 7465 7261 7469 6e67 290a 2d20 6765   iterating).- ge
-00001180: 745f 7573 6572 5f61 7274 6966 6163 745f  t_user_artifact_
-00001190: 6163 6365 7373 5f70 7265 7669 6577 2028  access_preview (
-000011a0: 616c 7265 6164 7920 6974 6572 6174 696e  already iteratin
-000011b0: 6729 0a2d 2067 6574 5f77 6964 656c 7920  g).- get_widely 
-000011c0: 7368 6172 6564 5f61 7274 6966 6163 7473  shared_artifacts
-000011d0: 5f70 7562 6c69 7368 6564 5f74 6f5f 7765  _published_to_we
-000011e0: 6220 2861 6c72 6561 6479 2069 7465 7261  b (already itera
-000011f0: 7469 6e67 290a 0a23 2320 4375 7272 656e  ting)..## Curren
-00001200: 7420 4361 7465 676f 7269 6573 0a52 6967  t Categories.Rig
-00001210: 6874 206e 6f77 2074 6865 206c 6962 7261  ht now the libra
-00001220: 7279 2069 7320 636f 6e73 756d 696e 6720  ry is consuming 
-00001230: 656e 6470 6f69 6e74 7320 6672 6f6d 3a20  endpoints from: 
-00001240: 0a2d 203c 6120 6872 6566 3d22 6874 7470  .- <a href="http
-00001250: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6c  s://github.com/l
-00001260: 6164 6174 6177 6562 2f53 696d 706c 6550  adataweb/SimpleP
-00001270: 4249 2f62 6c6f 622f 6d61 696e 2f41 646d  BI/blob/main/Adm
-00001280: 696e 5f64 6574 6169 6c73 2e74 7874 2220  in_details.txt" 
-00001290: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
-000012a0: 4164 6d69 6e3c 2f61 3e0a 2d20 3c61 2068  Admin</a>.- <a h
-000012b0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-000012c0: 6875 622e 636f 6d2f 6c61 6461 7461 7765  hub.com/ladatawe
-000012d0: 622f 5369 6d70 6c65 5042 492f 626c 6f62  b/SimplePBI/blob
-000012e0: 2f6d 6169 6e2f 4772 6f75 7073 5f64 6574  /main/Groups_det
-000012f0: 6169 6c73 2e74 7874 2220 7461 7267 6574  ails.txt" target
-00001300: 3d22 5f62 6c61 6e6b 223e 4772 6f75 7073  ="_blank">Groups
-00001310: 3c2f 613e 0a2d 203c 6120 6872 6566 3d22  </a>.- <a href="
-00001320: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001330: 6f6d 2f6c 6164 6174 6177 6562 2f53 696d  om/ladataweb/Sim
-00001340: 706c 6550 4249 2f62 6c6f 622f 6d61 696e  plePBI/blob/main
-00001350: 2f44 6174 6173 6574 735f 6465 7461 696c  /Datasets_detail
-00001360: 732e 7478 7422 2074 6172 6765 743d 225f  s.txt" target="_
-00001370: 626c 616e 6b22 3e44 6174 6173 6574 733c  blank">Datasets<
-00001380: 2f61 3e0a 2d20 3c61 2068 7265 663d 2268  /a>.- <a href="h
-00001390: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000013a0: 6d2f 6c61 6461 7461 7765 622f 5369 6d70  m/ladataweb/Simp
-000013b0: 6c65 5042 492f 626c 6f62 2f6d 6169 6e2f  lePBI/blob/main/
-000013c0: 4461 7461 666c 6f77 735f 6465 7461 696c  Dataflows_detail
-000013d0: 732e 7478 7422 2074 6172 6765 743d 225f  s.txt" target="_
-000013e0: 626c 616e 6b22 3e44 6174 6166 6c6f 7773  blank">Dataflows
-000013f0: 3c2f 613e 0a2d 203c 6120 6872 6566 3d22  </a>.- <a href="
-00001400: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001410: 6f6d 2f6c 6164 6174 6177 6562 2f53 696d  om/ladataweb/Sim
-00001420: 706c 6550 4249 2f62 6c6f 622f 6d61 696e  plePBI/blob/main
-00001430: 2f52 6570 6f72 7473 5f64 6574 6169 6c73  /Reports_details
-00001440: 2e74 7874 2220 7461 7267 6574 3d22 5f62  .txt" target="_b
-00001450: 6c61 6e6b 223e 5265 706f 7274 733c 2f61  lank">Reports</a
-00001460: 3e0a 2d20 3c61 2068 7265 663d 2268 7474  >.- <a href="htt
-00001470: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001480: 6c61 6461 7461 7765 622f 5369 6d70 6c65  ladataweb/Simple
-00001490: 5042 492f 626c 6f62 2f6d 6169 6e2f 4461  PBI/blob/main/Da
-000014a0: 7368 626f 6172 6473 5f64 6574 6169 6c73  shboards_details
-000014b0: 2e74 7874 2220 7461 7267 6574 3d22 5f62  .txt" target="_b
-000014c0: 6c61 6e6b 223e 4461 7368 626f 6172 6473  lank">Dashboards
-000014d0: 3c2f 613e 0a2d 203c 6120 6872 6566 3d22  </a>.- <a href="
-000014e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000014f0: 6f6d 2f6c 6164 6174 6177 6562 2f53 696d  om/ladataweb/Sim
-00001500: 706c 6550 4249 2f62 6c6f 622f 6d61 696e  plePBI/blob/main
-00001510: 2f41 7070 735f 6465 7461 696c 732e 7478  /Apps_details.tx
-00001520: 7422 2074 6172 6765 743d 225f 626c 616e  t" target="_blan
-00001530: 6b22 3e41 7070 733c 2f61 3e0a 2d20 3c61  k">Apps</a>.- <a
-00001540: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
-00001550: 6974 6875 622e 636f 6d2f 6c61 6461 7461  ithub.com/ladata
-00001560: 7765 622f 5369 6d70 6c65 5042 492f 626c  web/SimplePBI/bl
-00001570: 6f62 2f6d 6169 6e2f 496d 706f 7274 735f  ob/main/Imports_
-00001580: 6465 7461 696c 732e 7478 7422 2074 6172  details.txt" tar
-00001590: 6765 743d 225f 626c 616e 6b22 3e49 6d70  get="_blank">Imp
-000015a0: 6f72 7473 3c2f 613e 0a2d 203c 6120 6872  orts</a>.- <a hr
-000015b0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-000015c0: 7562 2e63 6f6d 2f6c 6164 6174 6177 6562  ub.com/ladataweb
-000015d0: 2f53 696d 706c 6550 4249 2f62 6c6f 622f  /SimplePBI/blob/
-000015e0: 6d61 696e 2f47 6174 6577 6179 735f 6465  main/Gateways_de
-000015f0: 7461 696c 732e 7478 7422 2074 6172 6765  tails.txt" targe
-00001600: 743d 225f 626c 616e 6b22 3e47 6174 6577  t="_blank">Gatew
-00001610: 6179 733c 2f61 3e0a 2d20 3c61 2068 7265  ays</a>.- <a hre
-00001620: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00001630: 622e 636f 6d2f 6c61 6461 7461 7765 622f  b.com/ladataweb/
-00001640: 5369 6d70 6c65 5042 492f 626c 6f62 2f6d  SimplePBI/blob/m
-00001650: 6169 6e2f 4361 7061 6369 7469 6573 5f64  ain/Capacities_d
-00001660: 6574 6169 6c73 2e74 7874 2220 7461 7267  etails.txt" targ
-00001670: 6574 3d22 5f62 6c61 6e6b 223e 4361 7061  et="_blank">Capa
-00001680: 6369 7469 6573 3c2f 613e 0a2d 203c 6120  cities</a>.- <a 
-00001690: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-000016a0: 7468 7562 2e63 6f6d 2f6c 6164 6174 6177  thub.com/ladataw
-000016b0: 6562 2f53 696d 706c 6550 4249 2f62 6c6f  eb/SimplePBI/blo
-000016c0: 622f 6d61 696e 2f50 6970 656c 696e 6573  b/main/Pipelines
-000016d0: 5f64 6574 6169 6c73 2e74 7874 2220 7461  _details.txt" ta
-000016e0: 7267 6574 3d22 5f62 6c61 6e6b 223e 5069  rget="_blank">Pi
-000016f0: 7065 6c69 6e65 7320 2850 7265 7669 6577  pelines (Preview
-00001700: 293c 2f61 3e0a 2d20 3c61 2068 7265 663d  )</a>.- <a href=
-00001710: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00001720: 636f 6d2f 6c61 6461 7461 7765 622f 5369  com/ladataweb/Si
-00001730: 6d70 6c65 5042 492f 626c 6f62 2f6d 6169  mplePBI/blob/mai
-00001740: 6e2f 5363 6f72 6563 6172 6473 5f64 6574  n/Scorecards_det
-00001750: 6169 6c73 2e74 7874 2220 7461 7267 6574  ails.txt" target
-00001760: 3d22 5f62 6c61 6e6b 223e 5363 6f72 6563  ="_blank">Scorec
-00001770: 6172 6473 2028 5072 6576 6965 7729 3c2f  ards (Preview)</
-00001780: 613e 0a0a 2323 2041 6464 6974 696f 6e61  a>..## Additiona
-00001790: 6c20 636f 6e74 656e 740a 5468 6572 6520  l content.There 
-000017a0: 616e 2061 6469 7469 6f6e 616c 206c 6962  an aditional lib
-000017b0: 7261 7279 2055 7469 6c73 2066 6f72 2074  rary Utils for t
-000017c0: 7261 6e73 666f 726d 6174 696f 6e73 2e20  ransformations. 
-000017d0: 4974 2069 7320 7573 6564 2074 6f20 6865  It is used to he
-000017e0: 6c70 2073 6f6d 6520 7265 7175 6573 7473  lp some requests
-000017f0: 2072 6574 7572 6e69 6e67 2064 6966 6665   returning diffe
-00001800: 7265 6e74 2076 616c 7565 732e 0a54 6865  rent values..The
-00001810: 206d 6f73 7420 7573 6566 756c 206d 6574   most useful met
-00001820: 686f 6420 696e 2074 6865 2055 7469 6c73  hod in the Utils
-00001830: 2063 6c61 7373 206d 6967 6874 2062 6520   class might be 
-00001840: 746f 5f70 616e 6461 732e 2059 6f75 2063  to_pandas. You c
-00001850: 616e 2075 7365 2074 6865 206d 6574 686f  an use the metho
-00001860: 6420 746f 2063 6f6e 7665 7274 2073 696d  d to convert sim
-00001870: 706c 6520 6469 6374 7320 746f 2070 616e  ple dicts to pan
-00001880: 6461 732e 2049 7420 6e65 6564 7320 7468  das. It needs th
-00001890: 6520 6469 6374 2061 6e64 2074 6865 206b  e dict and the k
-000018a0: 6579 2066 6174 6865 7220 6f66 2061 206c  ey father of a l
-000018b0: 6973 7420 6f66 2064 6963 7473 2069 6e20  ist of dicts in 
-000018c0: 7468 6520 7265 7370 6f6e 7365 2e20 5468  the response. Th
-000018d0: 6520 7573 7561 6c20 6765 7420 7265 7370  e usual get resp
-000018e0: 6f6e 7365 7320 6172 6520 7573 696e 6720  onses are using 
-000018f0: 2276 616c 7565 2220 6173 2074 6865 206b  "value" as the k
-00001900: 6579 2e0a 5765 2061 7265 2061 6c73 6f20  ey..We are also 
-00001910: 6164 6469 6e67 206e 6577 206d 6574 686f  adding new metho
-00001920: 6473 2077 6974 6820 7468 6520 7265 7175  ds with the requ
-00001930: 6573 7473 2074 6f20 6865 6c70 2067 6574  ests to help get
-00001940: 206e 6577 2061 6374 696f 6e73 2e20 4578   new actions. Ex
-00001950: 616d 706c 6573 3a0a 2d20 4461 7461 666c  amples:.- Datafl
-00001960: 6f77 733a 2067 6574 206f 7270 6861 6e20  ows: get orphan 
-00001970: 6461 7461 666c 6f77 7320 2867 6574 2064  dataflows (get d
-00001980: 6174 6166 6c6f 7773 2077 6974 686f 7574  ataflows without
-00001990: 2064 6174 6173 6574 290a 2d20 496d 706f   dataset).- Impo
-000019a0: 7274 733a 2070 6f73 7420 696d 706f 7274  rts: post import
-000019b0: 2072 6570 6f72 7420 666f 6c64 6572 2028   report folder (
-000019c0: 706f 7374 2061 2061 6c6c 2070 6269 7820  post a all pbix 
-000019d0: 6669 6c65 7320 696e 2061 206c 6f63 616c  files in a local
-000019e0: 2066 6f6c 6465 7229 0a2d 2052 6570 6f72   folder).- Repor
-000019f0: 7473 3a20 7369 6d70 6c65 206d 6967 7261  ts: simple migra
-00001a00: 7465 2072 6570 6f72 7420 2863 6f70 7920  te report (copy 
-00001a10: 7265 706f 7274 2066 726f 6d20 776f 726b  report from work
-00001a20: 7370 6163 6520 746f 2061 2077 6f72 6b73  space to a works
-00001a30: 7061 6365 290a 0a23 2320 536d 616c 6c20  pace)..## Small 
-00001a40: 6361 7465 676f 7269 6573 0a53 6d61 6c6c  categories.Small
-00001a50: 2063 6174 6567 6f72 6965 7320 6c69 6b65   categories like
-00001a60: 2044 6174 6166 6c6f 7720 5374 6f72 6167   Dataflow Storag
-00001a70: 6520 4163 636f 756e 7473 2061 6e64 2041  e Accounts and A
-00001a80: 7661 696c 6162 6c65 2046 6561 7475 7265  vailable Feature
-00001a90: 7320 7765 7265 206d 6f76 6564 2074 6f20  s were moved to 
-00001aa0: 4772 6f75 7073 2061 6e64 2041 646d 696e  Groups and Admin
-00001ab0: 2e0a 0a23 204d 6973 7369 6e67 2065 6e64  ...# Missing end
-00001ac0: 706f 696e 7473 0a57 6520 6172 6520 7374  points.We are st
-00001ad0: 696c 6c20 6465 7665 6c6f 7069 6e67 2074  ill developing t
-00001ae0: 6865 206c 6962 7261 7279 2e20 5468 6520  he library. The 
-00001af0: 666f 6c6c 6f77 696e 6720 656e 6470 6f69  following endpoi
-00001b00: 6e74 7320 6672 6f6d 2061 646d 696e 2061  nts from admin a
-00001b10: 7265 2073 7469 6c6c 206d 6973 7369 6e67  re still missing
-00001b20: 0a23 2323 2041 646d 696e 200a 2d20 5365  .### Admin .- Se
-00001b30: 7420 616e 6420 5265 6d6f 7665 204c 6162  t and Remove Lab
-00001b40: 656c 7341 7341 646d 696e 0a23 2323 2047  elsAsAdmin.### G
-00001b50: 726f 7570 730a 2d20 5570 6461 7465 2067  roups.- Update g
-00001b60: 726f 7570 2055 7365 720a 2323 2320 4461  roup User.### Da
-00001b70: 7461 7365 7473 0a2d 2055 7064 6174 6520  tasets.- Update 
-00001b80: 6461 7461 736f 7572 6365 7320 2872 6567  datasources (reg
-00001b90: 756c 6172 2061 6e64 2069 6e20 6772 6f75  ular and in grou
-00001ba0: 7073 290a 2323 2320 5265 706f 7274 730a  ps).### Reports.
-00001bb0: 2d20 4578 706f 7274 2054 6f20 4669 6c65  - Export To File
-00001bc0: 2028 6675 6c6c 2072 6571 7565 7374 2c20   (full request, 
-00001bd0: 7468 6572 6520 6973 2061 2073 6d61 6c6c  there is a small
-00001be0: 6572 2073 696d 706c 6572 206f 6e65 290a  er simpler one).
-00001bf0: 2d20 4765 7420 4578 706f 7274 2054 6f20  - Get Export To 
-00001c00: 4669 6c65 2053 7461 7475 7320 2872 6567  File Status (reg
-00001c10: 756c 6172 2061 6e64 2069 6e20 6772 6f75  ular and in grou
-00001c20: 7073 290a 2d20 4765 7420 4669 6c65 204f  ps).- Get File O
-00001c30: 6620 4578 706f 7274 2054 6f20 4669 6c65  f Export To File
-00001c40: 2028 7265 6775 6c61 7220 616e 6420 696e   (regular and in
-00001c50: 2067 726f 7570 7329 0a2d 2055 7064 6174   groups).- Updat
-00001c60: 6520 4461 7461 736f 7572 6365 7320 2872  e Datasources (r
-00001c70: 6567 756c 6172 2061 6e64 2069 6e20 6772  egular and in gr
-00001c80: 6f75 7073 290a 2d20 5570 6461 7465 2052  oups).- Update R
-00001c90: 6570 6f72 7420 436f 6e74 656e 7420 2872  eport Content (r
-00001ca0: 6567 756c 6172 2061 6e64 2069 6e20 6772  egular and in gr
-00001cb0: 6f75 7073 290a 2323 2320 496d 706f 7274  oups).### Import
-00001cc0: 730a 2d20 4372 6561 7465 2054 656d 706f  s.- Create Tempo
-00001cd0: 7261 7279 2055 706c 6f61 6420 4c6f 6361  rary Upload Loca
-00001ce0: 7469 6f6e 0a2d 2043 7265 6174 6520 5465  tion.- Create Te
-00001cf0: 6d70 6f72 6172 7920 5570 6c6f 6164 204c  mporary Upload L
-00001d00: 6f63 6174 696f 6e20 496e 2047 726f 7570  ocation In Group
-00001d10: 0a2d 2050 6f73 7420 496d 706f 7274 2028  .- Post Import (
-00001d20: 666f 7220 786c 7378 2c20 6a73 6f6e 2061  for xlsx, json a
-00001d30: 6e64 2072 646c 290a 2d20 506f 7374 2049  nd rdl).- Post I
-00001d40: 6d70 6f72 7420 496e 2047 726f 7570 2028  mport In Group (
-00001d50: 666f 7220 786c 7378 2c20 6a73 6f6e 2061  for xlsx, json a
-00001d60: 6e64 2072 646c 290a 2323 2320 4761 7465  nd rdl).### Gate
-00001d70: 7761 7973 200a 2d20 4372 6561 7465 2044  ways .- Create D
-00001d80: 6174 6173 6f75 7263 6520 286c 6f6f 6b73  atasource (looks
-00001d90: 206c 696b 6520 7468 6572 6520 6973 2061   like there is a
-00001da0: 2062 7567 206f 6e20 7468 6520 4150 4929   bug on the API)
-00001db0: 0a2d 2055 7064 6174 6520 4461 7461 736f  .- Update Dataso
-00001dc0: 7572 6365 200a 2d20 4465 6c65 7465 2044  urce .- Delete D
-00001dd0: 6174 6173 6f75 7263 6520 0a23 2323 2053  atasource .### S
-00001de0: 636f 7265 6361 7264 7320 2870 7265 7669  corecards (previ
-00001df0: 6577 290a 2d20 5061 7463 6820 4279 2049  ew).- Patch By I
-00001e00: 6420 0a2d 204d 6f76 6520 476f 616c 730a  d .- Move Goals.
-00001e10: 2323 2320 5075 7368 2044 6174 6173 6574  ### Push Dataset
-00001e20: 730a 2d20 416c 6c20 7265 7175 6573 7473  s.- All requests
-00001e30: 0a23 2323 2045 6d62 6564 2054 6f6b 656e  .### Embed Token
-00001e40: 0a2d 2041 6c6c 2072 6571 7565 7374 7320  .- All requests 
-00001e50: 0a23 2323 2047 6f61 6c73 2028 7072 6576  .### Goals (prev
-00001e60: 6965 7729 0a2d 2041 6c6c 2072 6571 7565  iew).- All reque
-00001e70: 7374 730a 0a23 204e 6578 7420 5374 6570  sts..# Next Step
-00001e80: 7320 2870 6c61 6e6e 6564 2069 7465 6d73  s (planned items
-00001e90: 290a 2d20 4b65 6570 2063 6f6d 706c 6574  ).- Keep complet
-00001ea0: 696e 6720 6d69 7373 696e 6720 656e 6470  ing missing endp
-00001eb0: 6f69 6e74 7320 6361 7465 676f 7279 2e0a  oints category..
-00001ec0: 2d20 416e 616c 797a 696e 6720 686f 7720  - Analyzing how 
-00001ed0: 746f 2069 6e63 6c75 6465 2065 6d62 6564  to include embed
-00001ee0: 696e 6720 616e 6420 7075 7368 696e 6720  ing and pushing 
-00001ef0: 6461 7461 7365 7420 7265 7175 6573 7473  dataset requests
-00001f00: 2e0a 0a0a 0a0a 4368 616e 6765 204c 6f67  ......Change Log
-00001f10: 0a3d 3d3d 3d3d 3d3d 3d3d 3d0a 0a30 2e30  .==========..0.0
-00001f20: 2e31 2028 3034 2f30 392f 3230 3231 290a  .1 (04/09/2021).
-00001f30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001f40: 2d2d 2d0a 2d20 4669 7273 7420 436f 6d6d  ---.- First Comm
-00001f50: 6974 0a0a 302e 302e 3220 2832 392f 3130  it..0.0.2 (29/10
-00001f60: 2f32 3032 3129 0a2d 2d2d 2d2d 2d2d 2d2d  /2021).---------
-00001f70: 2d2d 2d2d 2d2d 2d2d 2d2d 0a2d 2043 6f6d  ----------.- Com
-00001f80: 706c 6574 696e 6720 616c 6d6f 7374 2061  pleting almost a
-00001f90: 6c6c 2074 6865 2072 6571 7565 7374 7320  ll the requests 
-00001fa0: 696e 2041 646d 696e 2053 6563 7469 6f6e  in Admin Section
-00001fb0: 0a0a 302e 302e 3320 2831 342f 3131 2f32  ..0.0.3 (14/11/2
-00001fc0: 3032 3129 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  021).-----------
-00001fd0: 2d2d 2d2d 2d2d 2d0a 2d20 4372 6561 7469  -------.- Creati
-00001fe0: 6e67 2061 6469 7469 6f6e 616c 2063 6f6e  ng aditional con
-00001ff0: 7465 6e74 2074 6f20 6164 6d69 6e20 616e  tent to admin an
-00002000: 6420 6164 6469 6e67 2066 6972 7374 2063  d adding first c
-00002010: 6f6d 6d69 7420 666f 7220 6772 6f75 7073  ommit for groups
-00002020: 2061 6e64 2064 6174 6173 6574 7320 6361   and datasets ca
-00002030: 7465 676f 7279 0a0a 302e 302e 3420 2831  tegory..0.0.4 (1
-00002040: 352f 3131 2f32 3032 3129 0a2d 2d2d 2d2d  5/11/2021).-----
-00002050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2d20  -------------.- 
-00002060: 5265 706f 2f73 6f75 7263 6520 676f 696e  Repo/source goin
-00002070: 6720 7075 626c 6963 2e20 4164 6469 6e67  g public. Adding
-00002080: 2064 6174 6173 6574 7320 616e 6420 6772   datasets and gr
-00002090: 6f75 7073 2050 6f77 6572 2042 6920 5265  oups Power Bi Re
-000020a0: 7374 2041 5049 2063 6174 6567 6f72 792e  st API category.
-000020b0: 0a0a 302e 302e 3520 2831 362f 3131 2f32  ..0.0.5 (16/11/2
-000020c0: 3032 3129 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  021).-----------
-000020d0: 2d2d 2d2d 2d2d 2d0a 2d20 4669 7869 6e67  -------.- Fixing
-000020e0: 2065 7272 6f72 2068 616e 646c 696e 672e   error handling.
-000020f0: 2041 6464 696e 6720 6461 7461 666c 6f77   Adding dataflow
-00002100: 7320 506f 7765 7220 4269 2052 6573 7420  s Power Bi Rest 
-00002110: 4150 4920 6361 7465 676f 7279 0a0a 302e  API category..0.
-00002120: 302e 3620 2832 392f 3131 2f32 3032 3129  0.6 (29/11/2021)
-00002130: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
-00002140: 2d2d 2d0a 2d20 4669 7869 6e67 2069 6e73  ---.- Fixing ins
-00002150: 7461 6c6c 206d 6f64 756c 6520 6973 7375  tall module issu
-00002160: 6573 0a0a 302e 302e 3720 2832 392f 3131  es..0.0.7 (29/11
-00002170: 2f32 3032 3129 0a2d 2d2d 2d2d 2d2d 2d2d  /2021).---------
-00002180: 2d2d 2d2d 2d2d 2d2d 2d0a 2d20 4669 7869  ---------.- Fixi
-00002190: 6e67 2064 6174 6173 6574 7320 666f 7220  ng datasets for 
-000021a0: 6461 7820 7175 6572 6965 730a 0a30 2e30  dax queries..0.0
-000021b0: 2e38 2028 3239 2f31 312f 3230 3231 290a  .8 (29/11/2021).
-000021c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000021d0: 2d2d 0a2d 2046 6978 696e 6720 7479 706f  --.- Fixing typo
-000021e0: 2066 6f72 2064 6178 2071 7565 7269 6573   for dax queries
-000021f0: 2061 766f 6964 696e 6720 6e75 6c6c 730a   avoiding nulls.
-00002200: 0a30 2e30 2e39 2028 3034 2f30 312f 3230  .0.0.9 (04/01/20
-00002210: 3232 290a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  22).------------
-00002220: 2d2d 2d2d 2d2d 0a2d 2041 6464 696e 6720  ------.- Adding 
-00002230: 6e65 7720 7072 6576 6965 7720 7265 7175  new preview requ
-00002240: 6573 7473 2066 6f72 2073 7562 7363 7269  ests for subscri
-00002250: 7074 696f 6e73 2069 6e20 4164 6d69 6e20  ptions in Admin 
-00002260: 6361 7465 676f 7279 2e20 5468 6f73 6520  category. Those 
-00002270: 7265 6c65 6173 6564 2074 6869 7320 6d6f  released this mo
-00002280: 6e74 6820 6279 2050 6f77 6572 2042 692e  nth by Power Bi.
-00002290: 0a0a 302e 302e 3130 2028 3138 2f30 312f  ..0.0.10 (18/01/
-000022a0: 3230 3232 290a 2d2d 2d2d 2d2d 2d2d 2d2d  2022).----------
-000022b0: 2d2d 2d2d 2d2d 2d2d 0a2d 2041 6464 696e  --------.- Addin
-000022c0: 6720 616c 6c20 6461 7368 626f 6172 6473  g all dashboards
-000022d0: 2072 6571 7565 7374 7320 616e 6420 3830   requests and 80
-000022e0: 2520 6f66 2072 6570 6f72 7473 2072 6571  % of reports req
-000022f0: 7565 7374 732e 0a0a 302e 302e 3131 2028  uests...0.0.11 (
-00002300: 3038 2f30 342f 3230 3232 290a 2d2d 2d2d  08/04/2022).----
-00002310: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a2d  --------------.-
-00002320: 2041 6464 696e 6720 7769 6465 6c79 2073   Adding widely s
-00002330: 6861 7265 6420 6172 7469 6661 6374 7320  hared artifacts 
-00002340: 7265 7175 6573 7473 2066 6f72 2061 646d  requests for adm
-00002350: 696e 2063 6174 6567 6f72 792e 200a 2d20  in category. .- 
-00002360: 4164 6469 6e67 2041 7070 2063 6174 6567  Adding App categ
-00002370: 6f72 7920 7265 7175 6573 7473 2e0a 2d20  ory requests..- 
-00002380: 4164 6469 6e67 2022 6765 7422 2072 6571  Adding "get" req
-00002390: 7565 7374 7320 6672 6f6d 2069 6d70 6f72  uests from impor
-000023a0: 7420 6361 7465 676f 7279 2e0a 0a30 2e30  t category...0.0
-000023b0: 2e31 3220 2832 302f 3035 2f32 3032 3229  .12 (20/05/2022)
-000023c0: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
-000023d0: 2d2d 2d0a 2d20 4669 7869 6e67 2072 6570  ---.- Fixing rep
-000023e0: 6f72 7473 2062 7567 7320 616e 6420 6164  orts bugs and ad
-000023f0: 6469 6e67 2065 7870 6f72 7420 746f 2066  ding export to f
-00002400: 696c 6520 6173 2070 7265 7669 6577 0a2d  ile as preview.-
-00002410: 2041 6464 696e 6720 706f 7374 2069 6d70   Adding post imp
-00002420: 6f72 7420 6669 6c65 2074 6f20 776f 726b  ort file to work
-00002430: 7370 6163 6520 286f 6e6c 7920 7062 6978  space (only pbix
-00002440: 2066 696c 6573 206f 6620 6c65 7373 2074   files of less t
-00002450: 6861 6e20 3167 6229 0a0a 302e 302e 3133  han 1gb)..0.0.13
-00002460: 2028 3237 2f30 352f 3230 3232 290a 2d2d   (27/05/2022).--
-00002470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002480: 0a2d 2055 7064 6174 696e 6720 496d 706f  .- Updating Impo
-00002490: 7274 2072 6571 7565 7374 2045 7865 6375  rt request Execu
-000024a0: 7465 5175 6572 6965 7320 7769 7468 2074  teQueries with t
-000024b0: 6865 206e 6577 2075 7064 6174 6520 6672  he new update fr
-000024c0: 6f6d 204d 6963 726f 736f 6674 206d 616b  om Microsoft mak
-000024d0: 696e 6720 6974 2047 412e 0a2d 2043 7265  ing it GA..- Cre
-000024e0: 6174 696e 6720 6120 6e65 7720 6d65 7468  ating a new meth
-000024f0: 6f64 2074 6f20 696d 706f 7274 2061 6c6c  od to import all
-00002500: 2070 6269 7820 6669 6c65 7320 696e 2061   pbix files in a
-00002510: 6e20 7370 6563 6966 6965 6420 6c6f 6361  n specified loca
-00002520: 6c20 666f 6c64 6572 2074 6f20 6120 776f  l folder to a wo
-00002530: 726b 7370 6163 650a 0a30 2e30 2e31 3420  rkspace..0.0.14 
-00002540: 2832 372f 3037 2f32 3032 3229 0a2d 2d2d  (27/07/2022).---
-00002550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-00002560: 2d20 4164 6469 6e67 2061 6c6d 6f73 7420  - Adding almost 
-00002570: 616c 6c20 6761 7465 7761 7920 6361 7465  all gateway cate
-00002580: 676f 7279 2072 6571 7565 7374 730a 2d20  gory requests.- 
-00002590: 4164 6469 6e67 206e 6577 2073 7065 6369  Adding new speci
-000025a0: 616c 2072 6571 7565 7374 2066 726f 6d20  al request from 
-000025b0: 6c61 6461 7461 7765 622e 204d 6967 7261  ladataweb. Migra
-000025c0: 7469 6e67 2072 6570 6f72 7473 2062 6574  ting reports bet
-000025d0: 7765 656e 2077 6f72 6b73 7061 6365 732e  ween workspaces.
-000025e0: 2049 6d70 6f72 7469 6e67 2070 6269 7820   Importing pbix 
-000025f0: 6669 6c65 7320 6672 6f6d 2052 6570 6f6e  files from Repon
-00002600: 7365 2e43 6f6e 7465 6e74 2072 6571 7565  se.Content reque
-00002610: 7374 7320 6c69 6272 6172 7920 746f 2061  sts library to a
-00002620: 2050 6f77 6572 2042 6920 5365 7276 6963   Power Bi Servic
-00002630: 6520 576f 726b 7370 6163 650a 0a30 2e30  e Workspace..0.0
-00002640: 2e31 3520 2830 382f 3038 2f32 3032 3229  .15 (08/08/2022)
-00002650: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
-00002660: 2d2d 2d0a 2d20 4164 6469 6e67 2063 6170  ---.- Adding cap
-00002670: 6163 6974 6965 7320 6361 7465 676f 7279  acities category
-00002680: 2072 6571 7565 7374 732e 0a2d 2046 6978   requests..- Fix
-00002690: 696e 6720 6465 7363 7269 7074 696f 6e73  ing descriptions
-000026a0: 0a0a 302e 312e 3020 2830 332f 3130 2f32  ..0.1.0 (03/10/2
-000026b0: 3032 3229 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  022).-----------
-000026c0: 2d2d 2d2d 2d2d 2d0a 2d20 4164 6469 6e67  -------.- Adding
-000026d0: 2070 6970 656c 696e 6573 2061 6e64 2073   pipelines and s
-000026e0: 636f 7265 6361 7264 7320 6361 7465 676f  corecards catego
-000026f0: 7279 2072 6571 7565 7374 732e 0a2d 2041  ry requests..- A
-00002700: 6c6c 2063 6f6d 706f 6e65 6e74 6573 2063  ll componentes c
-00002710: 6174 6567 6f72 7920 6172 6520 6e6f 7720  ategory are now 
-00002720: 6176 6169 6c61 626c 6520 7769 7468 2061  available with a
-00002730: 206c 6974 746c 6520 6d69 7373 696e 6720   little missing 
-00002740: 656e 6470 6f69 6e74 730a 2d20 436f 6d70  endpoints.- Comp
-00002750: 6c65 7469 6e67 2061 7420 6c65 6173 7420  leting at least 
-00002760: 3830 2520 6f66 2072 6571 7565 7374 2066  80% of request f
-00002770: 6f72 2061 6c6c 206d 6f73 7420 6672 6571  or all most freq
-00002780: 7565 6e74 2069 7465 6d73 2061 7420 506f  uent items at Po
-00002790: 7765 7220 4269 2e20 5468 6520 6f6e 6c79  wer Bi. The only
-000027a0: 2063 6174 6567 6f72 6965 7320 756e 6176   categories unav
-000027b0: 6169 6c61 626c 6573 2061 7265 2070 7573  ailables are pus
-000027c0: 6820 6461 7461 7365 7473 2061 6e64 2065  h datasets and e
-000027d0: 6d62 6564 6469 6e67 2e0a 2d20 4275 6720  mbedding..- Bug 
-000027e0: 6669 7869 6e67 2072 6571 7565 7374 7320  fixing requests 
-000027f0: 0a0a 302e 312e 3120 2833 302f 3031 2f32  ..0.1.1 (30/01/2
-00002800: 3032 3329 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  023).-----------
-00002810: 2d2d 2d2d 2d2d 2d0a 4d69 6e6f 7220 6275  -------.Minor bu
-00002820: 6720 6669 7869 6e67 2066 6f72 2069 6d70  g fixing for imp
-00002830: 6f72 7473 2074 6f20 7265 6164 2066 696c  orts to read fil
-00002840: 6573 7973 7465 6d0a 0a30 2e31 2e32 2028  esystem..0.1.2 (
-00002850: 3134 2f30 322f 3230 3233 290a 2d2d 2d2d  14/02/2023).----
-00002860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a49  --------------.I
-00002870: 6d70 726f 7669 6e67 2067 6574 2061 6374  mproving get act
-00002880: 6976 6974 7920 6576 656e 7473 2066 6f72  ivity events for
-00002890: 2073 696e 676c 6520 6461 7920 6166 7465   single day afte
-000028a0: 7220 506f 7765 7242 6920 7570 6461 7465  r PowerBi update
-000028b0: 732e 0a41 6464 696e 6720 6e65 7720 7265  s..Adding new re
-000028c0: 7175 6573 7420 746f 2067 6574 206c 6173  quest to get las
-000028d0: 7420 3330 2064 6179 7320 6f66 2061 6374  t 30 days of act
-000028e0: 6976 6974 7920 6c6f 6773 2061 7574 6f6d  ivity logs autom
-000028f0: 6174 6963 616c 6c79 2e0a 0a              atically...
+00000010: 3a20 322e 310d 0a4e 616d 653a 2053 696d  : 2.1..Name: Sim
+00000020: 706c 6550 4249 0d0a 5665 7273 696f 6e3a  plePBI..Version:
+00000030: 2030 2e31 2e33 0d0a 5375 6d6d 6172 793a   0.1.3..Summary:
+00000040: 2053 696d 706c 6966 7920 7573 6167 6520   Simplify usage 
+00000050: 6f66 2050 6f77 6572 2042 6920 5265 7374  of Power Bi Rest
+00000060: 2041 5049 0d0a 486f 6d65 2d70 6167 653a   API..Home-page:
+00000070: 200d 0a44 6f77 6e6c 6f61 642d 5552 4c3a   ..Download-URL:
+00000080: 200d 0a41 7574 686f 723a 2049 676e 6163   ..Author: Ignac
+00000090: 696f 2042 6172 7261 7520 3c69 676e 615f  io Barrau <igna_
+000000a0: 6261 7272 6175 4068 6f74 6d61 696c 2e63  barrau@hotmail.c
+000000b0: 6f6d 3e2c 204d 6172 7469 6e20 5a75 7269  om>, Martin Zuri
+000000c0: 7461 203c 6d61 7274 696e 7a75 7269 7461  ta <martinzurita
+000000d0: 3140 676d 6169 6c2e 636f 6d3e 0d0a 4c69  1@gmail.com>..Li
+000000e0: 6365 6e73 653a 204d 4954 0d0a 5072 6f6a  cense: MIT..Proj
+000000f0: 6563 742d 5552 4c3a 2044 6f63 756d 656e  ect-URL: Documen
+00000100: 7461 7469 6f6e 2c20 6874 7470 733a 2f2f  tation, https://
+00000110: 646f 6373 2e6d 6963 726f 736f 6674 2e63  docs.microsoft.c
+00000120: 6f6d 2f65 6e2d 7573 2f72 6573 742f 6170  om/en-us/rest/ap
+00000130: 692f 706f 7765 722d 6269 2f0d 0a50 726f  i/power-bi/..Pro
+00000140: 6a65 6374 2d55 524c 3a20 5361 7920 5468  ject-URL: Say Th
+00000150: 616e 6b73 212c 2068 7474 7073 3a2f 2f77  anks!, https://w
+00000160: 7777 2e6c 6164 6174 6177 6562 2e63 6f6d  ww.ladataweb.com
+00000170: 2e61 722f 636f 6e74 6163 746f 2e68 746d  .ar/contacto.htm
+00000180: 6c0d 0a50 726f 6a65 6374 2d55 524c 3a20  l..Project-URL: 
+00000190: 536f 7572 6365 2c20 6874 7470 733a 2f2f  Source, https://
+000001a0: 6769 7468 7562 2e63 6f6d 2f6c 6164 6174  github.com/ladat
+000001b0: 6177 6562 2f53 696d 706c 6550 4249 0d0a  aweb/SimplePBI..
+000001c0: 5072 6f6a 6563 742d 5552 4c3a 2054 7261  Project-URL: Tra
+000001d0: 636b 6572 2c20 6874 7470 733a 2f2f 6769  cker, https://gi
+000001e0: 7468 7562 2e63 6f6d 2f6c 6164 6174 6177  thub.com/ladataw
+000001f0: 6562 2f53 696d 706c 6550 4249 2f69 7373  eb/SimplePBI/iss
+00000200: 7565 730d 0a4b 6579 776f 7264 733a 2050  ues..Keywords: P
+00000210: 6f77 6572 2042 492c 5042 492c 4c61 4461  ower BI,PBI,LaDa
+00000220: 7461 5765 622c 417a 7572 652c 4461 7461  taWeb,Azure,Data
+00000230: 2c50 7974 686f 6e0d 0a43 6c61 7373 6966  ,Python..Classif
+00000240: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000250: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000260: 686f 6e20 3a3a 2033 0d0a 436c 6173 7369  hon :: 3..Classi
+00000270: 6669 6572 3a20 4c69 6365 6e73 6520 3a3a  fier: License ::
+00000280: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+00000290: 204d 4954 204c 6963 656e 7365 0d0a 436c   MIT License..Cl
+000002a0: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
+000002b0: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
+000002c0: 2049 6e64 6570 656e 6465 6e74 0d0a 4465   Independent..De
+000002d0: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
+000002e0: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
+000002f0: 6b64 6f77 6e0d 0a4c 6963 656e 7365 2d46  kdown..License-F
+00000300: 696c 653a 204c 4943 454e 5345 0d0a 5265  ile: LICENSE..Re
+00000310: 7175 6972 6573 2d44 6973 743a 2072 6571  quires-Dist: req
+00000320: 7565 7374 730d 0a52 6571 7569 7265 732d  uests..Requires-
+00000330: 4469 7374 3a20 7061 6e64 6173 0d0a 5265  Dist: pandas..Re
+00000340: 7175 6972 6573 2d44 6973 743a 2072 6571  quires-Dist: req
+00000350: 7565 7374 732d 746f 6f6c 6265 6c74 0d0a  uests-toolbelt..
+00000360: 0d0a 2320 5369 6d70 6c65 5042 490d 0a0d  ..# SimplePBI...
+00000370: 0a54 6869 7320 6973 2061 2073 696d 706c  .This is a simpl
+00000380: 6520 6c69 6272 6172 7920 7468 6174 206d  e library that m
+00000390: 616b 6573 2069 7420 6561 7379 2074 6f20  akes it easy to 
+000003a0: 7573 6520 7468 6520 506f 7765 7220 4269  use the Power Bi
+000003b0: 2052 4553 5420 4150 492e 204f 6e65 2064   REST API. One d
+000003c0: 6179 2053 696d 706c 6550 4249 2077 696c  ay SimplePBI wil
+000003d0: 6c20 636f 6e74 6169 6e20 616c 6c20 7468  l contain all th
+000003e0: 6520 6361 7465 676f 7269 6573 2069 6e20  e categories in 
+000003f0: 7468 6520 4150 4920 2841 646d 696e 2c20  the API (Admin, 
+00000400: 6461 7461 7365 7473 2c20 7265 706f 7274  datasets, report
+00000410: 732c 2065 7463 292e 0d0a 4665 656c 2066  s, etc)...Feel f
+00000420: 7265 6520 746f 2063 6865 636b 2074 6865  ree to check the
+00000430: 2064 6f63 2074 6f20 6765 7420 6120 6465   doc to get a de
+00000440: 6570 6572 2075 6e64 6572 7374 616e 6469  eper understandi
+00000450: 6e67 206f 6620 6120 7370 6563 6966 6963  ng of a specific
+00000460: 2072 6571 7565 7374 3a20 6874 7470 733a   request: https:
+00000470: 2f2f 646f 6373 2e6d 6963 726f 736f 6674  //docs.microsoft
+00000480: 2e63 6f6d 2f65 6e2d 7573 2f72 6573 742f  .com/en-us/rest/
+00000490: 6170 692f 706f 7765 722d 6269 2f0d 0a3c  api/power-bi/..<
+000004a0: 6272 3e57 6520 6172 6520 646f 696e 6720  br>We are doing 
+000004b0: 6f75 7220 6265 7374 2074 6f20 6d61 6b65  our best to make
+000004c0: 2074 6869 7320 6c69 6272 6172 7920 7573   this library us
+000004d0: 6566 756c 2066 6f72 2074 6865 2063 6f6d  eful for the com
+000004e0: 6d75 6e69 7479 2e20 5468 6973 2070 726f  munity. This pro
+000004f0: 6a65 6374 2069 7320 6e6f 7420 6120 7265  ject is not a re
+00000500: 6d75 6e65 7261 626c 6520 6a6f 6220 666f  munerable job fo
+00000510: 7220 7573 2e20 4974 2773 2061 2070 7562  r us. It's a pub
+00000520: 6c69 6320 636f 6d6d 756e 6974 7920 7072  lic community pr
+00000530: 6f6a 6563 742e 2050 6c65 6173 6520 6265  oject. Please be
+00000540: 2070 6174 6965 6e74 2069 6620 796f 7520   patient if you 
+00000550: 7375 626d 6974 2061 6e20 6973 7375 6520  submit an issue 
+00000560: 616e 6420 6974 2773 206e 6f74 2066 6978  and it's not fix
+00000570: 6564 2072 6967 6874 2061 7761 792e 2049  ed right away. I
+00000580: 7427 7320 6120 7761 7920 746f 2065 7870  t's a way to exp
+00000590: 7265 7373 206f 7572 2070 6173 7369 6f6e  ress our passion
+000005a0: 206f 6620 7368 6172 696e 6720 6b6e 6f77   of sharing know
+000005b0: 6c65 6467 652e 0d0a 3c62 723e 4561 6368  ledge...<br>Each
+000005c0: 2063 6174 6567 6f72 7920 6973 2061 6e20   category is an 
+000005d0: 4f62 6a65 6374 2e20 5468 6973 206d 6561  Object. This mea
+000005e0: 6e73 2077 6520 6e65 6564 2074 6f20 696e  ns we need to in
+000005f0: 6974 6961 6c69 7a65 2061 6e20 6f62 6a65  itialize an obje
+00000600: 6374 2074 6f20 7374 6172 7420 7573 696e  ct to start usin
+00000610: 6720 6974 7320 6d65 7468 6f64 732e 2049  g its methods. I
+00000620: 6e20 6f72 6465 7220 746f 2063 7265 6174  n order to creat
+00000630: 6520 7468 656d 2077 6520 6e65 6564 2074  e them we need t
+00000640: 6865 2042 6561 7265 7220 746f 6b65 6e20  he Bearer token 
+00000650: 7468 6174 2063 616e 2062 6520 6f62 7461  that can be obta
+00000660: 696e 2066 726f 6d20 6120 546f 6b65 6e20  in from a Token 
+00000670: 4f62 6a65 6374 2e20 0d0a 4c65 7427 7320  Object. ..Let's 
+00000680: 7365 6520 686f 7720 7765 2063 616e 2063  see how we can c
+00000690: 7265 6174 6520 616e 2041 646d 696e 204f  reate an Admin O
+000006a0: 626a 6563 7420 746f 2074 7279 2074 6865  bject to try the
+000006b0: 2072 6571 7565 7374 7320 696e 2074 6861   requests in tha
+000006c0: 7420 6361 7465 676f 7279 2e0d 0a0d 0a60  t category.....`
+000006d0: 6060 7079 7468 6f6e 0d0a 2320 496d 706f  ``python..# Impo
+000006e0: 7274 206c 6962 7261 7279 0d0a 6672 6f6d  rt library..from
+000006f0: 2073 696d 706c 6570 6269 2069 6d70 6f72   simplepbi impor
+00000700: 7420 746f 6b65 6e0d 0a66 726f 6d20 7369  t token..from si
+00000710: 6d70 6c65 7062 6920 696d 706f 7274 2061  mplepbi import a
+00000720: 646d 696e 0d0a 6060 600d 0a0d 0a57 6520  dmin..```....We 
+00000730: 616c 7761 7973 206e 6565 6420 746f 2069  always need to i
+00000740: 6d70 6f72 7420 746f 6b65 6e20 6f62 6a65  mport token obje
+00000750: 6374 2074 6f20 6372 6561 7465 2074 6865  ct to create the
+00000760: 206f 626a 6563 7420 746f 2072 756e 2072   object to run r
+00000770: 6571 7565 7374 732e 2054 6865 6e20 7765  equests. Then we
+00000780: 2063 616e 2070 6963 6b20 7468 6520 6f62   can pick the ob
+00000790: 6a65 6374 206f 6620 7468 6520 506f 7765  ject of the Powe
+000007a0: 7220 4269 2052 6573 7420 4150 4920 6361  r Bi Rest API ca
+000007b0: 7465 676f 7279 2077 6520 6e65 6564 2e20  tegory we need. 
+000007c0: 466f 7220 696e 7374 616e 6365 2022 6164  For instance "ad
+000007d0: 6d69 6e22 2e0d 0a54 6865 2074 6f6b 656e  min"...The token
+000007e0: 2063 616e 2062 6520 6372 6561 7465 6420   can be created 
+000007f0: 696e 2074 776f 2077 6179 732c 2074 6865  in two ways, the
+00000800: 2072 6567 756c 6172 2061 7574 6865 6e74   regular authent
+00000810: 6963 6174 696f 6e20 616e 6420 7468 6520  ication and the 
+00000820: 7365 7276 6963 6520 7072 696e 6369 7061  service principa
+00000830: 6c20 6f6e 652e 2049 7420 6465 7065 6e64  l one. It depend
+00000840: 7320 7768 6963 6820 6f6e 6520 796f 7520  s which one you 
+00000850: 7069 636b 2074 6f20 636f 6d70 6c65 7465  pick to complete
+00000860: 2074 6865 2072 6571 7565 7374 2e20 0d0a   the request. ..
+00000870: 5468 6573 6520 6172 6520 7468 6520 6e65  These are the ne
+00000880: 6365 7373 6172 7920 6172 6775 6d65 6e74  cessary argument
+00000890: 7320 746f 2067 6574 2061 2074 6f6b 656e  s to get a token
+000008a0: 3a0d 0a2d 2074 656e 616e 745f 6964 2028  :..- tenant_id (
+000008b0: 796f 7520 6361 6e20 6765 7420 6974 2066  you can get it f
+000008c0: 726f 6d20 7375 6273 6372 6970 7469 6f6e  rom subscription
+000008d0: 2072 6573 6f75 7263 6520 696e 2061 7a75   resource in azu
+000008e0: 7265 2070 6f72 7461 6c20 6f72 2061 736b  re portal or ask
+000008f0: 2066 6f72 2069 7420 746f 2074 6865 2049   for it to the I
+00000900: 5420 6465 7061 7274 6d65 6e74 290d 0a2d  T department)..-
+00000910: 2061 7070 5f63 6c69 656e 745f 6964 2028   app_client_id (
+00000920: 796f 7572 2061 7070 5f69 642f 636c 6965  your app_id/clie
+00000930: 6e74 5f69 6420 6672 6f6d 2074 6865 2041  nt_id from the A
+00000940: 7070 2072 6567 6973 7465 7265 6420 696e  pp registered in
+00000950: 2041 7a75 7265 2077 6974 6820 7065 726d   Azure with perm
+00000960: 6973 7369 6f6e 7320 746f 2050 6f77 6572  issions to Power
+00000970: 2042 6920 5365 7276 6963 6529 0d0a 2d20   Bi Service)..- 
+00000980: 7573 6572 6e61 6d65 2028 7072 6f66 6573  username (profes
+00000990: 7369 6f6e 616c 2065 6d61 696c 2061 6363  sional email acc
+000009a0: 6f75 6e74 2069 6e20 417a 7572 6520 4144  ount in Azure AD
+000009b0: 290d 0a2d 2070 6173 7377 6f72 6420 2870  )..- password (p
+000009c0: 726f 6665 7373 696f 6e61 6c20 7061 7373  rofessional pass
+000009d0: 776f 7264 290d 0a2d 2061 7070 5f73 6563  word)..- app_sec
+000009e0: 7265 745f 6b65 7920 2873 6563 7265 7420  ret_key (secret 
+000009f0: 6b65 7920 6765 6e65 7261 7465 6420 666f  key generated fo
+00000a00: 7220 7468 6520 636c 6965 6e74 2069 6429  r the client id)
+00000a10: 0d0a 2d20 7573 655f 7365 7276 6963 655f  ..- use_service_
+00000a20: 7072 696e 6369 7061 6c20 2854 7275 6520  principal (True 
+00000a30: 746f 2061 7468 656e 7469 6361 7465 2077  to athenticate w
+00000a40: 6974 6820 5365 7276 6963 6520 5072 696e  ith Service Prin
+00000a50: 6369 7061 6c20 616e 6420 4661 6c73 6520  cipal and False 
+00000a60: 746f 2063 6f6e 7469 6e75 6520 7769 7468  to continue with
+00000a70: 2075 7365 7220 6372 6564 656e 7469 616c   user credential
+00000a80: 7329 0d0a 0d0a 0d0a 2a4e 4f54 453a 2069  s)......*NOTE: i
+00000a90: 6620 796f 7520 7761 6e74 2074 6f20 7573  f you want to us
+00000aa0: 6520 7365 7276 6963 6520 7072 696e 6369  e service princi
+00000ab0: 7061 6c2c 2062 6520 7375 7265 2074 6f20  pal, be sure to 
+00000ac0: 6861 7665 2079 6f75 7220 7465 6e61 6e74  have your tenant
+00000ad0: 2072 6561 6479 2066 6f72 2074 6861 742e   ready for that.
+00000ae0: 0d0a 3c62 723e 5265 6769 7374 6572 2061  ..<br>Register a
+00000af0: 7070 2065 7861 6d70 6c65 3a20 6874 7470  pp example: http
+00000b00: 733a 2f2f 626c 6f67 2e6c 6164 6174 6177  s://blog.ladataw
+00000b10: 6562 2e63 6f6d 2e61 722f 706f 7374 2f31  eb.com.ar/post/1
+00000b20: 3838 3034 3532 3237 3733 352f 6765 742d  88045227735/get-
+00000b30: 6163 6365 7373 2d74 6f6b 656e 0d0a 3c62  access-token..<b
+00000b40: 723e 5365 7276 6963 6520 5072 696e 6369  r>Service Princi
+00000b50: 7061 6c20 7065 726d 6973 7369 6f6e 7320  pal permissions 
+00000b60: 666f 7220 6164 6d69 6e20 6170 693a 2068  for admin api: h
+00000b70: 7474 7073 3a2f 2f64 6f63 732e 6d69 6372  ttps://docs.micr
+00000b80: 6f73 6f66 742e 636f 6d2f 656e 2d75 732f  osoft.com/en-us/
+00000b90: 706f 7765 722d 6269 2f61 646d 696e 2f72  power-bi/admin/r
+00000ba0: 6561 642d 6f6e 6c79 2d61 7069 732d 7365  ead-only-apis-se
+00000bb0: 7276 6963 652d 7072 696e 6369 7061 6c2d  rvice-principal-
+00000bc0: 6175 7468 656e 7469 6361 7469 6f6e 2a0d  authentication*.
+00000bd0: 0a0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  .....```python..
+00000be0: 2320 4372 6561 7469 6e67 206f 626a 6563  # Creating objec
+00000bf0: 7473 0d0a 0d0a 2352 6567 756c 6172 204c  ts....#Regular L
+00000c00: 6f67 696e 0d0a 746f 6b20 3d20 746f 6b65  ogin..tok = toke
+00000c10: 6e2e 546f 6b65 6e28 7465 6e61 6e74 5f69  n.Token(tenant_i
+00000c20: 642c 2061 7070 5f63 6c69 656e 745f 6964  d, app_client_id
+00000c30: 2c20 7573 6572 6e61 6d65 2c20 7061 7373  , username, pass
+00000c40: 776f 7264 2c20 4e6f 6e65 2c20 7573 655f  word, None, use_
+00000c50: 7365 7276 6963 655f 7072 696e 6369 7061  service_principa
+00000c60: 6c3d 4661 6c73 6529 0d0a 0d0a 2353 6572  l=False)....#Ser
+00000c70: 7669 6365 2050 7269 6e63 6970 616c 0d0a  vice Principal..
+00000c80: 746f 6b20 3d20 746f 6b65 6e2e 546f 6b65  tok = token.Toke
+00000c90: 6e28 7465 6e61 6e74 5f69 642c 2061 7070  n(tenant_id, app
+00000ca0: 5f63 6c69 656e 745f 6964 2c20 4e6f 6e65  _client_id, None
+00000cb0: 2c20 4e6f 6e65 2c20 6170 705f 7365 6372  , None, app_secr
+00000cc0: 6574 5f6b 6579 2c20 7573 655f 7365 7276  et_key, use_serv
+00000cd0: 6963 655f 7072 696e 6369 7061 6c3d 5472  ice_principal=Tr
+00000ce0: 7565 290d 0a0d 0a61 6420 3d20 6164 6d69  ue)....ad = admi
+00000cf0: 6e2e 4164 6d69 6e28 746f 6b2e 746f 6b65  n.Admin(tok.toke
+00000d00: 6e29 0d0a 6060 600d 0a0d 0a41 7320 796f  n)..```....As yo
+00000d10: 7520 6361 6e20 7365 6520 7468 6520 546f  u can see the To
+00000d20: 6b65 6e20 6f62 6a65 6374 2063 6f6e 7461  ken object conta
+00000d30: 696e 7320 6120 746f 6b65 6e20 6174 7472  ins a token attr
+00000d40: 6962 7574 6520 7769 7468 2074 6865 2042  ibute with the B
+00000d50: 6561 7265 7220 7573 6564 2062 7920 417a  earer used by Az
+00000d60: 7572 6520 746f 2072 756e 2072 6573 7420  ure to run rest 
+00000d70: 6d65 7468 6f64 732e 2054 6861 7420 6174  methods. That at
+00000d80: 7472 6962 7574 6520 7769 6c6c 2062 6520  tribute will be 
+00000d90: 7573 6572 2074 6f20 6372 6561 7465 2074  user to create t
+00000da0: 6865 2063 6174 6567 6f72 7920 6f62 6a65  he category obje
+00000db0: 6374 7320 6c69 6b65 2061 646d 696e 2e0d  cts like admin..
+00000dc0: 0a4f 6e63 6520 7765 2063 7265 6174 6520  .Once we create 
+00000dd0: 6f75 7220 4f62 6a65 6374 206c 696b 6520  our Object like 
+00000de0: 6164 6d69 6e2c 2077 6520 6361 6e20 7374  admin, we can st
+00000df0: 6172 7420 7573 696e 6720 7468 6520 7265  art using the re
+00000e00: 7175 6573 7473 2061 6464 696e 6720 7468  quests adding th
+00000e10: 6520 636f 7272 6563 7420 7061 7261 6d65  e correct parame
+00000e20: 7465 7273 2069 6620 7468 6579 2061 7265  ters if they are
+00000e30: 206e 6565 6465 642e 0d0a 0d0a 6060 6070   needed.....```p
+00000e40: 7974 686f 6e0d 0a23 2047 6574 7469 6e67  ython..# Getting
+00000e50: 206f 626a 6563 7473 0d0a 0d0a 416c 6c5f   objects....All_
+00000e60: 4461 7461 7365 7473 203d 2061 642e 6765  Datasets = ad.ge
+00000e70: 745f 6461 7461 7365 7473 2829 0d0a 0d0a  t_datasets()....
+00000e80: 4461 7461 7365 7473 5f49 6e5f 4772 6f75  Datasets_In_Grou
+00000e90: 7073 203d 2061 642e 6765 745f 6461 7461  ps = ad.get_data
+00000ea0: 7365 7473 5f69 6e5f 6772 6f75 7028 776f  sets_in_group(wo
+00000eb0: 726b 7370 6163 655f 6964 290d 0a60 6060  rkspace_id)..```
+00000ec0: 0d0a 0d0a 5468 6520 6c69 6272 6172 7920  ....The library 
+00000ed0: 6765 7420 7265 7175 6573 7473 2077 696c  get requests wil
+00000ee0: 6c20 7265 7475 726e 2061 2072 6573 706f  l return a respo
+00000ef0: 6e73 6520 6f62 6a65 6374 202e 6a73 6f6e  nse object .json
+00000f00: 2829 2074 6861 7420 7079 7468 6f6e 2072  () that python r
+00000f10: 6561 6473 2069 7420 6173 2061 2044 6963  eads it as a Dic
+00000f20: 742e 0d0a 0d0a 2323 2050 7265 7669 6577  t.....## Preview
+00000f30: 206d 6574 686f 6473 0d0a 5468 6572 6520   methods..There 
+00000f40: 6172 6520 736f 6d65 206d 6574 686f 6473  are some methods
+00000f50: 2069 6e20 7468 6520 636c 6173 7365 7320   in the classes 
+00000f60: 7468 6174 2073 7469 6c6c 206e 6565 6420  that still need 
+00000f70: 6d6f 7265 2074 6573 7469 6e67 2e20 5468  more testing. Th
+00000f80: 6f73 6520 7769 6c6c 2068 6176 6520 6120  ose will have a 
+00000f90: 2270 7265 7669 6577 2220 6174 2074 6865  "preview" at the
+00000fa0: 2065 6e64 206f 6620 7468 6520 6e61 6d65   end of the name
+00000fb0: 2e20 506c 6561 7365 206c 6574 2075 7320  . Please let us 
+00000fc0: 6b6e 6f77 2069 6620 736f 6d65 7468 696e  know if somethin
+00000fd0: 6720 676f 6573 2077 726f 6e67 2077 6974  g goes wrong wit
+00000fe0: 6820 7468 6f73 652e 0d0a 0d0a 2323 2043  h those.....## C
+00000ff0: 7572 7265 6e74 2043 6174 6567 6f72 6965  urrent Categorie
+00001000: 730d 0a52 6967 6874 206e 6f77 2074 6865  s..Right now the
+00001010: 206c 6962 7261 7279 2069 7320 636f 6e73   library is cons
+00001020: 756d 696e 6720 656e 6470 6f69 6e74 7320  uming endpoints 
+00001030: 6672 6f6d 3a20 0d0a 2d20 3c61 2068 7265  from: ..- <a hre
+00001040: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00001050: 622e 636f 6d2f 6c61 6461 7461 7765 622f  b.com/ladataweb/
+00001060: 5369 6d70 6c65 5042 492f 626c 6f62 2f6d  SimplePBI/blob/m
+00001070: 6169 6e2f 4164 6d69 6e5f 6465 7461 696c  ain/Admin_detail
+00001080: 732e 7478 7422 2074 6172 6765 743d 225f  s.txt" target="_
+00001090: 626c 616e 6b22 3e41 646d 696e 3c2f 613e  blank">Admin</a>
+000010a0: 0d0a 2d20 3c61 2068 7265 663d 2268 7474  ..- <a href="htt
+000010b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000010c0: 6c61 6461 7461 7765 622f 5369 6d70 6c65  ladataweb/Simple
+000010d0: 5042 492f 626c 6f62 2f6d 6169 6e2f 4772  PBI/blob/main/Gr
+000010e0: 6f75 7073 5f64 6574 6169 6c73 2e74 7874  oups_details.txt
+000010f0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00001100: 223e 4772 6f75 7073 3c2f 613e 0d0a 2d20  ">Groups</a>..- 
+00001110: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00001120: 2f67 6974 6875 622e 636f 6d2f 6c61 6461  /github.com/lada
+00001130: 7461 7765 622f 5369 6d70 6c65 5042 492f  taweb/SimplePBI/
+00001140: 626c 6f62 2f6d 6169 6e2f 4461 7461 7365  blob/main/Datase
+00001150: 7473 5f64 6574 6169 6c73 2e74 7874 2220  ts_details.txt" 
+00001160: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00001170: 4461 7461 7365 7473 3c2f 613e 0d0a 2d20  Datasets</a>..- 
+00001180: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00001190: 2f67 6974 6875 622e 636f 6d2f 6c61 6461  /github.com/lada
+000011a0: 7461 7765 622f 5369 6d70 6c65 5042 492f  taweb/SimplePBI/
+000011b0: 626c 6f62 2f6d 6169 6e2f 4461 7461 666c  blob/main/Datafl
+000011c0: 6f77 735f 6465 7461 696c 732e 7478 7422  ows_details.txt"
+000011d0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+000011e0: 3e44 6174 6166 6c6f 7773 3c2f 613e 0d0a  >Dataflows</a>..
+000011f0: 2d20 3c61 2068 7265 663d 2268 7474 7073  - <a href="https
+00001200: 3a2f 2f67 6974 6875 622e 636f 6d2f 6c61  ://github.com/la
+00001210: 6461 7461 7765 622f 5369 6d70 6c65 5042  dataweb/SimplePB
+00001220: 492f 626c 6f62 2f6d 6169 6e2f 5265 706f  I/blob/main/Repo
+00001230: 7274 735f 6465 7461 696c 732e 7478 7422  rts_details.txt"
+00001240: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00001250: 3e52 6570 6f72 7473 3c2f 613e 0d0a 2d20  >Reports</a>..- 
+00001260: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00001270: 2f67 6974 6875 622e 636f 6d2f 6c61 6461  /github.com/lada
+00001280: 7461 7765 622f 5369 6d70 6c65 5042 492f  taweb/SimplePBI/
+00001290: 626c 6f62 2f6d 6169 6e2f 4461 7368 626f  blob/main/Dashbo
+000012a0: 6172 6473 5f64 6574 6169 6c73 2e74 7874  ards_details.txt
+000012b0: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+000012c0: 223e 4461 7368 626f 6172 6473 3c2f 613e  ">Dashboards</a>
+000012d0: 0d0a 2d20 3c61 2068 7265 663d 2268 7474  ..- <a href="htt
+000012e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000012f0: 6c61 6461 7461 7765 622f 5369 6d70 6c65  ladataweb/Simple
+00001300: 5042 492f 626c 6f62 2f6d 6169 6e2f 4170  PBI/blob/main/Ap
+00001310: 7073 5f64 6574 6169 6c73 2e74 7874 2220  ps_details.txt" 
+00001320: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00001330: 4170 7073 3c2f 613e 0d0a 2d20 3c61 2068  Apps</a>..- <a h
+00001340: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00001350: 6875 622e 636f 6d2f 6c61 6461 7461 7765  hub.com/ladatawe
+00001360: 622f 5369 6d70 6c65 5042 492f 626c 6f62  b/SimplePBI/blob
+00001370: 2f6d 6169 6e2f 496d 706f 7274 735f 6465  /main/Imports_de
+00001380: 7461 696c 732e 7478 7422 2074 6172 6765  tails.txt" targe
+00001390: 743d 225f 626c 616e 6b22 3e49 6d70 6f72  t="_blank">Impor
+000013a0: 7473 3c2f 613e 0d0a 2d20 3c61 2068 7265  ts</a>..- <a hre
+000013b0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+000013c0: 622e 636f 6d2f 6c61 6461 7461 7765 622f  b.com/ladataweb/
+000013d0: 5369 6d70 6c65 5042 492f 626c 6f62 2f6d  SimplePBI/blob/m
+000013e0: 6169 6e2f 4761 7465 7761 7973 5f64 6574  ain/Gateways_det
+000013f0: 6169 6c73 2e74 7874 2220 7461 7267 6574  ails.txt" target
+00001400: 3d22 5f62 6c61 6e6b 223e 4761 7465 7761  ="_blank">Gatewa
+00001410: 7973 3c2f 613e 0d0a 2d20 3c61 2068 7265  ys</a>..- <a hre
+00001420: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00001430: 622e 636f 6d2f 6c61 6461 7461 7765 622f  b.com/ladataweb/
+00001440: 5369 6d70 6c65 5042 492f 626c 6f62 2f6d  SimplePBI/blob/m
+00001450: 6169 6e2f 4361 7061 6369 7469 6573 5f64  ain/Capacities_d
+00001460: 6574 6169 6c73 2e74 7874 2220 7461 7267  etails.txt" targ
+00001470: 6574 3d22 5f62 6c61 6e6b 223e 4361 7061  et="_blank">Capa
+00001480: 6369 7469 6573 3c2f 613e 0d0a 2d20 3c61  cities</a>..- <a
+00001490: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+000014a0: 6974 6875 622e 636f 6d2f 6c61 6461 7461  ithub.com/ladata
+000014b0: 7765 622f 5369 6d70 6c65 5042 492f 626c  web/SimplePBI/bl
+000014c0: 6f62 2f6d 6169 6e2f 5069 7065 6c69 6e65  ob/main/Pipeline
+000014d0: 735f 6465 7461 696c 732e 7478 7422 2074  s_details.txt" t
+000014e0: 6172 6765 743d 225f 626c 616e 6b22 3e50  arget="_blank">P
+000014f0: 6970 656c 696e 6573 2028 5072 6576 6965  ipelines (Previe
+00001500: 7729 3c2f 613e 0d0a 2d20 3c61 2068 7265  w)</a>..- <a hre
+00001510: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00001520: 622e 636f 6d2f 6c61 6461 7461 7765 622f  b.com/ladataweb/
+00001530: 5369 6d70 6c65 5042 492f 626c 6f62 2f6d  SimplePBI/blob/m
+00001540: 6169 6e2f 5363 6f72 6563 6172 6473 5f64  ain/Scorecards_d
+00001550: 6574 6169 6c73 2e74 7874 2220 7461 7267  etails.txt" targ
+00001560: 6574 3d22 5f62 6c61 6e6b 223e 5363 6f72  et="_blank">Scor
+00001570: 6563 6172 6473 2028 5072 6576 6965 7729  ecards (Preview)
+00001580: 3c2f 613e 0d0a 0d0a 2323 2043 6f6d 706c  </a>....## Compl
+00001590: 6578 2072 6571 7565 7374 730d 0a49 6620  ex requests..If 
+000015a0: 796f 7520 7761 6e74 2074 6f20 6765 7420  you want to get 
+000015b0: 6120 6465 6570 6572 206c 6f6f 6b20 6f6e  a deeper look on
+000015c0: 2063 6f6d 706c 6578 205f 5f41 646d 696e   complex __Admin
+000015d0: 5f5f 206d 6574 686f 6473 2061 6e64 2075  __ methods and u
+000015e0: 6e69 7175 6520 6d65 7468 6f64 732e 200d  nique methods. .
+000015f0: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00001600: 2f2f 6769 7468 7562 2e63 6f6d 2f6c 6164  //github.com/lad
+00001610: 6174 6177 6562 2f53 696d 706c 6550 4249  ataweb/SimplePBI
+00001620: 2f62 6c6f 622f 6d61 696e 2f41 646d 696e  /blob/main/Admin
+00001630: 5f63 6f6d 706c 6578 2e6d 6422 2074 6172  _complex.md" tar
+00001640: 6765 743d 225f 626c 616e 6b22 3e43 6865  get="_blank">Che
+00001650: 636b 2074 6869 7320 646f 633c 2f61 3e0d  ck this doc</a>.
+00001660: 0a0d 0a23 2320 4164 6469 7469 6f6e 616c  ...## Additional
+00001670: 2063 6f6e 7465 6e74 0d0a 5468 6572 6520   content..There 
+00001680: 616e 2061 6469 7469 6f6e 616c 206c 6962  an aditional lib
+00001690: 7261 7279 2055 7469 6c73 2066 6f72 2074  rary Utils for t
+000016a0: 7261 6e73 666f 726d 6174 696f 6e73 2e20  ransformations. 
+000016b0: 4974 2069 7320 7573 6564 2074 6f20 6865  It is used to he
+000016c0: 6c70 2073 6f6d 6520 7265 7175 6573 7473  lp some requests
+000016d0: 2072 6574 7572 6e69 6e67 2064 6966 6665   returning diffe
+000016e0: 7265 6e74 2076 616c 7565 732e 0d0a 5468  rent values...Th
+000016f0: 6520 6d6f 7374 2075 7365 6675 6c20 6d65  e most useful me
+00001700: 7468 6f64 2069 6e20 7468 6520 5574 696c  thod in the Util
+00001710: 7320 636c 6173 7320 6d69 6768 7420 6265  s class might be
+00001720: 2074 6f5f 7061 6e64 6173 2e20 596f 7520   to_pandas. You 
+00001730: 6361 6e20 7573 6520 7468 6520 6d65 7468  can use the meth
+00001740: 6f64 2074 6f20 636f 6e76 6572 7420 7369  od to convert si
+00001750: 6d70 6c65 2064 6963 7473 2074 6f20 7061  mple dicts to pa
+00001760: 6e64 6173 2e20 4974 206e 6565 6473 2074  ndas. It needs t
+00001770: 6865 2064 6963 7420 616e 6420 7468 6520  he dict and the 
+00001780: 6b65 7920 6661 7468 6572 206f 6620 6120  key father of a 
+00001790: 6c69 7374 206f 6620 6469 6374 7320 696e  list of dicts in
+000017a0: 2074 6865 2072 6573 706f 6e73 652e 2054   the response. T
+000017b0: 6865 2075 7375 616c 2067 6574 2072 6573  he usual get res
+000017c0: 706f 6e73 6573 2061 7265 2075 7369 6e67  ponses are using
+000017d0: 2022 7661 6c75 6522 2061 7320 7468 6520   "value" as the 
+000017e0: 6b65 792e 0d0a 5765 2061 7265 2061 6c73  key...We are als
+000017f0: 6f20 6164 6469 6e67 206e 6577 206d 6574  o adding new met
+00001800: 686f 6473 2077 6974 6820 7468 6520 7265  hods with the re
+00001810: 7175 6573 7473 2074 6f20 6865 6c70 2067  quests to help g
+00001820: 6574 206e 6577 2061 6374 696f 6e73 2e20  et new actions. 
+00001830: 4578 616d 706c 6573 3a0d 0a0d 0a23 2323  Examples:....###
+00001840: 2045 7861 6d70 6c65 206f 6620 6f75 7220   Example of our 
+00001850: 616d 617a 696e 6720 756e 6971 7565 2072  amazing unique r
+00001860: 6571 7565 7374 730d 0a2d 2067 6574 5f6f  equests..- get_o
+00001870: 7270 6861 6e5f 6461 7461 666c 6f77 735f  rphan_dataflows_
+00001880: 7072 6576 6965 773a 2067 6574 2064 6174  preview: get dat
+00001890: 6166 6c6f 7773 2077 6974 686f 7574 2064  aflows without d
+000018a0: 6174 6173 6574 0d0a 2d20 7369 6d70 6c65  ataset..- simple
+000018b0: 5f69 6d70 6f72 745f 7062 6978 3a20 6d61  _import_pbix: ma
+000018c0: 6b65 7320 7075 626c 6973 6869 6e67 2061  kes publishing a
+000018d0: 2070 6269 7820 6669 6c65 2065 6173 6965   pbix file easie
+000018e0: 720d 0a2d 2073 696d 706c 655f 696d 706f  r..- simple_impo
+000018f0: 7274 5f70 6269 785f 6173 5f70 6172 616d  rt_pbix_as_param
+00001900: 6574 6572 3a20 696d 706f 7274 2061 2070  eter: import a p
+00001910: 6269 7820 6672 6f6d 2061 7069 2072 6573  bix from api res
+00001920: 706f 6e73 6520 636f 6e74 656e 740d 0a2d  ponse content..-
+00001930: 2073 696d 706c 655f 696d 706f 7274 5f70   simple_import_p
+00001940: 6269 785f 666f 6c64 6572 5f69 6e5f 6772  bix_folder_in_gr
+00001950: 6f75 705f 7072 6576 6965 773a 2070 6f73  oup_preview: pos
+00001960: 7420 6120 616c 6c20 7062 6978 2066 696c  t a all pbix fil
+00001970: 6573 2069 6e20 6120 6c6f 6361 6c20 666f  es in a local fo
+00001980: 6c64 6572 0d0a 2d20 7369 6d70 6c65 5f69  lder..- simple_i
+00001990: 6d70 6f72 745f 6672 6f6d 5f64 6576 6f70  mport_from_devop
+000019a0: 733a 2069 6d70 6f72 7420 6120 7062 6978  s: import a pbix
+000019b0: 2066 726f 6d20 617a 7572 6520 6465 766f   from azure devo
+000019c0: 7073 2072 6570 6f0d 0a2d 2073 696d 706c  ps repo..- simpl
+000019d0: 655f 636f 7079 5f72 6570 6f72 7473 5f62  e_copy_reports_b
+000019e0: 6574 7765 656e 5f67 726f 7570 733a 2063  etween_groups: c
+000019f0: 6f70 7920 7265 706f 7274 2066 726f 6d20  opy report from 
+00001a00: 776f 726b 7370 6163 6520 746f 2061 2077  workspace to a w
+00001a10: 6f72 6b73 7061 6365 0d0a 2d20 656e 6861  orkspace..- enha
+00001a20: 6e63 6564 5f72 6566 7265 7368 5f64 6174  nced_refresh_dat
+00001a30: 6173 6574 5f69 6e5f 6772 6f75 703a 2061  aset_in_group: a
+00001a40: 2073 7065 6369 616c 2072 6571 7565 7374   special request
+00001a50: 2066 6561 7475 7265 2074 6861 7420 6e6f   feature that no
+00001a60: 7420 6f6e 6c79 2065 6c69 6d69 6e61 7465  t only eliminate
+00001a70: 7320 7468 6520 6e65 6564 2066 6f72 2073  s the need for s
+00001a80: 796e 6368 726f 6e6f 7573 2063 6c69 656e  ynchronous clien
+00001a90: 7420 636f 6e6e 6563 7469 6f6e 7320 746f  t connections to
+00001aa0: 2070 6572 666f 726d 2061 2072 6566 7265   perform a refre
+00001ab0: 7368 2c20 6275 7420 616c 736f 2075 6e6c  sh, but also unl
+00001ac0: 6f63 6b73 2065 6e74 6572 7072 6973 652d  ocks enterprise-
+00001ad0: 6772 6164 6520 7265 6672 6573 6820 6361  grade refresh ca
+00001ae0: 7061 6269 6c69 7469 6573 2e0d 0a2d 2067  pabilities...- g
+00001af0: 6574 5f61 6374 6976 6974 795f 6576 656e  et_activity_even
+00001b00: 7473 5f70 7265 7669 6577 2028 616c 7265  ts_preview (alre
+00001b10: 6164 7920 6974 6572 6174 696e 6729 3a20  ady iterating): 
+00001b20: 6d61 6b65 7320 7468 6520 6765 7420 6163  makes the get ac
+00001b30: 7469 7669 7479 2065 7665 6e74 7320 7370  tivity events sp
+00001b40: 6563 6966 6965 6420 6279 2064 6174 6520  ecified by date 
+00001b50: 6561 7369 6572 0d0a 2d20 6765 745f 7573  easier..- get_us
+00001b60: 6572 5f61 7274 6966 6163 745f 6163 6365  er_artifact_acce
+00001b70: 7373 5f70 7265 7669 6577 2028 616c 7265  ss_preview (alre
+00001b80: 6164 7920 6974 6572 6174 696e 6729 3a20  ady iterating): 
+00001b90: 6d61 6b65 7320 7468 6520 6765 7420 7573  makes the get us
+00001ba0: 6572 2061 7274 6966 6163 7420 6163 6365  er artifact acce
+00001bb0: 7373 2065 6173 6965 720d 0a2d 2067 6574  ss easier..- get
+00001bc0: 5f77 6964 656c 7920 7368 6172 6564 5f61  _widely shared_a
+00001bd0: 7274 6966 6163 7473 5f70 7562 6c69 7368  rtifacts_publish
+00001be0: 6564 5f74 6f5f 7765 6220 2861 6c72 6561  ed_to_web (alrea
+00001bf0: 6479 2069 7465 7261 7469 6e67 293a 206d  dy iterating): m
+00001c00: 616b 6573 2067 6574 696e 6720 7468 6520  akes geting the 
+00001c10: 7075 626c 6973 6865 6420 746f 2077 6562  published to web
+00001c20: 2072 6570 6f73 2069 6e66 6f20 6561 7369   repos info easi
+00001c30: 6572 0d0a 0d0a 2323 2053 6d61 6c6c 2063  er....## Small c
+00001c40: 6174 6567 6f72 6965 730d 0a53 6d61 6c6c  ategories..Small
+00001c50: 2063 6174 6567 6f72 6965 7320 6c69 6b65   categories like
+00001c60: 2044 6174 6166 6c6f 7720 5374 6f72 6167   Dataflow Storag
+00001c70: 6520 4163 636f 756e 7473 2061 6e64 2041  e Accounts and A
+00001c80: 7661 696c 6162 6c65 2046 6561 7475 7265  vailable Feature
+00001c90: 7320 7765 7265 206d 6f76 6564 2074 6f20  s were moved to 
+00001ca0: 4772 6f75 7073 2061 6e64 2041 646d 696e  Groups and Admin
+00001cb0: 2e0d 0a0d 0a23 204d 6973 7369 6e67 2065  .....# Missing e
+00001cc0: 6e64 706f 696e 7473 0d0a 5765 2061 7265  ndpoints..We are
+00001cd0: 2073 7469 6c6c 2064 6576 656c 6f70 696e   still developin
+00001ce0: 6720 7468 6520 6c69 6272 6172 792e 2054  g the library. T
+00001cf0: 6865 2066 6f6c 6c6f 7769 6e67 2065 6e64  he following end
+00001d00: 706f 696e 7473 2066 726f 6d20 6164 6d69  points from admi
+00001d10: 6e20 6172 6520 7374 696c 6c20 6d69 7373  n are still miss
+00001d20: 696e 670d 0a23 2323 2041 646d 696e 200d  ing..### Admin .
+00001d30: 0a2d 2053 6574 2061 6e64 2052 656d 6f76  .- Set and Remov
+00001d40: 6520 4c61 6265 6c73 4173 4164 6d69 6e0d  e LabelsAsAdmin.
+00001d50: 0a23 2323 2047 726f 7570 730d 0a2d 2055  .### Groups..- U
+00001d60: 7064 6174 6520 6772 6f75 7020 5573 6572  pdate group User
+00001d70: 0d0a 2323 2320 5265 706f 7274 730d 0a2d  ..### Reports..-
+00001d80: 2045 7870 6f72 7420 546f 2046 696c 6520   Export To File 
+00001d90: 2866 756c 6c20 7265 7175 6573 742c 2074  (full request, t
+00001da0: 6865 7265 2069 7320 6120 736d 616c 6c65  here is a smalle
+00001db0: 7220 7369 6d70 6c65 7220 6f6e 6529 0d0a  r simpler one)..
+00001dc0: 2d20 4765 7420 4578 706f 7274 2054 6f20  - Get Export To 
+00001dd0: 4669 6c65 2053 7461 7475 7320 2872 6567  File Status (reg
+00001de0: 756c 6172 2061 6e64 2069 6e20 6772 6f75  ular and in grou
+00001df0: 7073 290d 0a2d 2047 6574 2046 696c 6520  ps)..- Get File 
+00001e00: 4f66 2045 7870 6f72 7420 546f 2046 696c  Of Export To Fil
+00001e10: 6520 2872 6567 756c 6172 2061 6e64 2069  e (regular and i
+00001e20: 6e20 6772 6f75 7073 290d 0a2d 2055 7064  n groups)..- Upd
+00001e30: 6174 6520 4461 7461 736f 7572 6365 7320  ate Datasources 
+00001e40: 2872 646c 2066 696c 6573 2072 6567 756c  (rdl files regul
+00001e50: 6172 2061 6e64 2069 6e20 6772 6f75 7073  ar and in groups
+00001e60: 290d 0a2d 2055 7064 6174 6520 5265 706f  )..- Update Repo
+00001e70: 7274 2043 6f6e 7465 6e74 2028 7265 6775  rt Content (regu
+00001e80: 6c61 7220 616e 6420 696e 2067 726f 7570  lar and in group
+00001e90: 7329 0d0a 2323 2320 496d 706f 7274 730d  s)..### Imports.
+00001ea0: 0a2d 2043 7265 6174 6520 5465 6d70 6f72  .- Create Tempor
+00001eb0: 6172 7920 5570 6c6f 6164 204c 6f63 6174  ary Upload Locat
+00001ec0: 696f 6e0d 0a2d 2043 7265 6174 6520 5465  ion..- Create Te
+00001ed0: 6d70 6f72 6172 7920 5570 6c6f 6164 204c  mporary Upload L
+00001ee0: 6f63 6174 696f 6e20 496e 2047 726f 7570  ocation In Group
+00001ef0: 0d0a 2d20 506f 7374 2049 6d70 6f72 7420  ..- Post Import 
+00001f00: 2866 6f72 2078 6c73 782c 206a 736f 6e20  (for xlsx, json 
+00001f10: 616e 6420 7264 6c29 0d0a 2d20 506f 7374  and rdl)..- Post
+00001f20: 2049 6d70 6f72 7420 496e 2047 726f 7570   Import In Group
+00001f30: 2028 666f 7220 786c 7378 2c20 6a73 6f6e   (for xlsx, json
+00001f40: 2061 6e64 2072 646c 290d 0a23 2323 2047   and rdl)..### G
+00001f50: 6174 6577 6179 7320 0d0a 2d20 4372 6561  ateways ..- Crea
+00001f60: 7465 2044 6174 6173 6f75 7263 6520 286c  te Datasource (l
+00001f70: 6f6f 6b73 206c 696b 6520 7468 6572 6520  ooks like there 
+00001f80: 6973 2061 2062 7567 206f 6e20 7468 6520  is a bug on the 
+00001f90: 4150 4929 0d0a 2d20 5570 6461 7465 2044  API)..- Update D
+00001fa0: 6174 6173 6f75 7263 6520 0d0a 2d20 4465  atasource ..- De
+00001fb0: 6c65 7465 2044 6174 6173 6f75 7263 6520  lete Datasource 
+00001fc0: 0d0a 2323 2320 5363 6f72 6563 6172 6473  ..### Scorecards
+00001fd0: 2028 7072 6576 6965 7729 0d0a 2d20 5061   (preview)..- Pa
+00001fe0: 7463 6820 4279 2049 6420 0d0a 2d20 4d6f  tch By Id ..- Mo
+00001ff0: 7665 2047 6f61 6c73 0d0a 2323 2320 5075  ve Goals..### Pu
+00002000: 7368 2044 6174 6173 6574 730d 0a2d 2041  sh Datasets..- A
+00002010: 6c6c 2072 6571 7565 7374 730d 0a23 2323  ll requests..###
+00002020: 2045 6d62 6564 2054 6f6b 656e 0d0a 2d20   Embed Token..- 
+00002030: 416c 6c20 7265 7175 6573 7473 200d 0a23  All requests ..#
+00002040: 2323 2047 6f61 6c73 2028 7072 6576 6965  ## Goals (previe
+00002050: 7729 0d0a 2d20 416c 6c20 7265 7175 6573  w)..- All reques
+00002060: 7473 0d0a 0d0a 2320 4e65 7874 2053 7465  ts....# Next Ste
+00002070: 7073 2028 706c 616e 6e65 6420 6974 656d  ps (planned item
+00002080: 7329 0d0a 2d20 4b65 6570 2063 6f6d 706c  s)..- Keep compl
+00002090: 6574 696e 6720 6d69 7373 696e 6720 656e  eting missing en
+000020a0: 6470 6f69 6e74 7320 6361 7465 676f 7279  dpoints category
+000020b0: 2e0d 0a2d 2043 7265 6174 696e 6720 6e65  ...- Creating ne
+000020c0: 7720 6177 6573 6f6d 6520 6964 6561 732e  w awesome ideas.
+000020d0: 0d0a 2d20 416e 616c 797a 696e 6720 686f  ..- Analyzing ho
+000020e0: 7720 746f 2069 6e63 6c75 6465 2065 6d62  w to include emb
+000020f0: 6564 696e 6720 616e 6420 7075 7368 696e  eding and pushin
+00002100: 6720 6461 7461 7365 7420 7265 7175 6573  g dataset reques
+00002110: 7473 2e0d 0a0d 0a0d 0a0d 0a0d 0a43 6861  ts...........Cha
+00002120: 6e67 6520 4c6f 670d 0a3d 3d3d 3d3d 3d3d  nge Log..=======
+00002130: 3d3d 3d0d 0a0d 0a30 2e30 2e31 2028 3034  ===....0.0.1 (04
+00002140: 2f30 392f 3230 3231 290d 0a2d 2d2d 2d2d  /09/2021)..-----
+00002150: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a  --------------..
+00002160: 2d20 4669 7273 7420 436f 6d6d 6974 0d0a  - First Commit..
+00002170: 0d0a 302e 302e 3220 2832 392f 3130 2f32  ..0.0.2 (29/10/2
+00002180: 3032 3129 0d0a 2d2d 2d2d 2d2d 2d2d 2d2d  021)..----------
+00002190: 2d2d 2d2d 2d2d 2d2d 2d0d 0a2d 2043 6f6d  ---------..- Com
+000021a0: 706c 6574 696e 6720 616c 6d6f 7374 2061  pleting almost a
+000021b0: 6c6c 2074 6865 2072 6571 7565 7374 7320  ll the requests 
+000021c0: 696e 2041 646d 696e 2053 6563 7469 6f6e  in Admin Section
+000021d0: 0d0a 0d0a 302e 302e 3320 2831 342f 3131  ....0.0.3 (14/11
+000021e0: 2f32 3032 3129 0d0a 2d2d 2d2d 2d2d 2d2d  /2021)..--------
+000021f0: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2d20 4372  ----------..- Cr
+00002200: 6561 7469 6e67 2061 6469 7469 6f6e 616c  eating aditional
+00002210: 2063 6f6e 7465 6e74 2074 6f20 6164 6d69   content to admi
+00002220: 6e20 616e 6420 6164 6469 6e67 2066 6972  n and adding fir
+00002230: 7374 2063 6f6d 6d69 7420 666f 7220 6772  st commit for gr
+00002240: 6f75 7073 2061 6e64 2064 6174 6173 6574  oups and dataset
+00002250: 7320 6361 7465 676f 7279 0d0a 0d0a 302e  s category....0.
+00002260: 302e 3420 2831 352f 3131 2f32 3032 3129  0.4 (15/11/2021)
+00002270: 0d0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ..--------------
+00002280: 2d2d 2d2d 0d0a 2d20 5265 706f 2f73 6f75  ----..- Repo/sou
+00002290: 7263 6520 676f 696e 6720 7075 626c 6963  rce going public
+000022a0: 2e20 4164 6469 6e67 2064 6174 6173 6574  . Adding dataset
+000022b0: 7320 616e 6420 6772 6f75 7073 2050 6f77  s and groups Pow
+000022c0: 6572 2042 6920 5265 7374 2041 5049 2063  er Bi Rest API c
+000022d0: 6174 6567 6f72 792e 0d0a 0d0a 302e 302e  ategory.....0.0.
+000022e0: 3520 2831 362f 3131 2f32 3032 3129 0d0a  5 (16/11/2021)..
+000022f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002300: 2d2d 0d0a 2d20 4669 7869 6e67 2065 7272  --..- Fixing err
+00002310: 6f72 2068 616e 646c 696e 672e 2041 6464  or handling. Add
+00002320: 696e 6720 6461 7461 666c 6f77 7320 506f  ing dataflows Po
+00002330: 7765 7220 4269 2052 6573 7420 4150 4920  wer Bi Rest API 
+00002340: 6361 7465 676f 7279 0d0a 0d0a 302e 302e  category....0.0.
+00002350: 3620 2832 392f 3131 2f32 3032 3129 0d0a  6 (29/11/2021)..
+00002360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002370: 2d2d 0d0a 2d20 4669 7869 6e67 2069 6e73  --..- Fixing ins
+00002380: 7461 6c6c 206d 6f64 756c 6520 6973 7375  tall module issu
+00002390: 6573 0d0a 0d0a 302e 302e 3720 2832 392f  es....0.0.7 (29/
+000023a0: 3131 2f32 3032 3129 0d0a 2d2d 2d2d 2d2d  11/2021)..------
+000023b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2d20  ------------..- 
+000023c0: 4669 7869 6e67 2064 6174 6173 6574 7320  Fixing datasets 
+000023d0: 666f 7220 6461 7820 7175 6572 6965 730d  for dax queries.
+000023e0: 0a0d 0a30 2e30 2e38 2028 3239 2f31 312f  ...0.0.8 (29/11/
+000023f0: 3230 3231 290d 0a2d 2d2d 2d2d 2d2d 2d2d  2021)..---------
+00002400: 2d2d 2d2d 2d2d 2d2d 2d0d 0a2d 2046 6978  ---------..- Fix
+00002410: 696e 6720 7479 706f 2066 6f72 2064 6178  ing typo for dax
+00002420: 2071 7565 7269 6573 2061 766f 6964 696e   queries avoidin
+00002430: 6720 6e75 6c6c 730d 0a0d 0a30 2e30 2e39  g nulls....0.0.9
+00002440: 2028 3034 2f30 312f 3230 3232 290d 0a2d   (04/01/2022)..-
+00002450: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002460: 2d0d 0a2d 2041 6464 696e 6720 6e65 7720  -..- Adding new 
+00002470: 7072 6576 6965 7720 7265 7175 6573 7473  preview requests
+00002480: 2066 6f72 2073 7562 7363 7269 7074 696f   for subscriptio
+00002490: 6e73 2069 6e20 4164 6d69 6e20 6361 7465  ns in Admin cate
+000024a0: 676f 7279 2e20 5468 6f73 6520 7265 6c65  gory. Those rele
+000024b0: 6173 6564 2074 6869 7320 6d6f 6e74 6820  ased this month 
+000024c0: 6279 2050 6f77 6572 2042 692e 0d0a 0d0a  by Power Bi.....
+000024d0: 302e 302e 3130 2028 3138 2f30 312f 3230  0.0.10 (18/01/20
+000024e0: 3232 290d 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  22)..-----------
+000024f0: 2d2d 2d2d 2d2d 2d0d 0a2d 2041 6464 696e  -------..- Addin
+00002500: 6720 616c 6c20 6461 7368 626f 6172 6473  g all dashboards
+00002510: 2072 6571 7565 7374 7320 616e 6420 3830   requests and 80
+00002520: 2520 6f66 2072 6570 6f72 7473 2072 6571  % of reports req
+00002530: 7565 7374 732e 0d0a 0d0a 302e 302e 3131  uests.....0.0.11
+00002540: 2028 3038 2f30 342f 3230 3232 290d 0a2d   (08/04/2022)..-
+00002550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002560: 2d0d 0a2d 2041 6464 696e 6720 7769 6465  -..- Adding wide
+00002570: 6c79 2073 6861 7265 6420 6172 7469 6661  ly shared artifa
+00002580: 6374 7320 7265 7175 6573 7473 2066 6f72  cts requests for
+00002590: 2061 646d 696e 2063 6174 6567 6f72 792e   admin category.
+000025a0: 200d 0a2d 2041 6464 696e 6720 4170 7020   ..- Adding App 
+000025b0: 6361 7465 676f 7279 2072 6571 7565 7374  category request
+000025c0: 732e 0d0a 2d20 4164 6469 6e67 2022 6765  s...- Adding "ge
+000025d0: 7422 2072 6571 7565 7374 7320 6672 6f6d  t" requests from
+000025e0: 2069 6d70 6f72 7420 6361 7465 676f 7279   import category
+000025f0: 2e0d 0a0d 0a30 2e30 2e31 3220 2832 302f  .....0.0.12 (20/
+00002600: 3035 2f32 3032 3229 0d0a 2d2d 2d2d 2d2d  05/2022)..------
+00002610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2d20  ------------..- 
+00002620: 4669 7869 6e67 2072 6570 6f72 7473 2062  Fixing reports b
+00002630: 7567 7320 616e 6420 6164 6469 6e67 2065  ugs and adding e
+00002640: 7870 6f72 7420 746f 2066 696c 6520 6173  xport to file as
+00002650: 2070 7265 7669 6577 0d0a 2d20 4164 6469   preview..- Addi
+00002660: 6e67 2070 6f73 7420 696d 706f 7274 2066  ng post import f
+00002670: 696c 6520 746f 2077 6f72 6b73 7061 6365  ile to workspace
+00002680: 2028 6f6e 6c79 2070 6269 7820 6669 6c65   (only pbix file
+00002690: 7320 6f66 206c 6573 7320 7468 616e 2031  s of less than 1
+000026a0: 6762 290d 0a0d 0a30 2e30 2e31 3320 2832  gb)....0.0.13 (2
+000026b0: 372f 3035 2f32 3032 3229 0d0a 2d2d 2d2d  7/05/2022)..----
+000026c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a  --------------..
+000026d0: 2d20 5570 6461 7469 6e67 2049 6d70 6f72  - Updating Impor
+000026e0: 7420 7265 7175 6573 7420 4578 6563 7574  t request Execut
+000026f0: 6551 7565 7269 6573 2077 6974 6820 7468  eQueries with th
+00002700: 6520 6e65 7720 7570 6461 7465 2066 726f  e new update fro
+00002710: 6d20 4d69 6372 6f73 6f66 7420 6d61 6b69  m Microsoft maki
+00002720: 6e67 2069 7420 4741 2e0d 0a2d 2043 7265  ng it GA...- Cre
+00002730: 6174 696e 6720 6120 6e65 7720 6d65 7468  ating a new meth
+00002740: 6f64 2074 6f20 696d 706f 7274 2061 6c6c  od to import all
+00002750: 2070 6269 7820 6669 6c65 7320 696e 2061   pbix files in a
+00002760: 6e20 7370 6563 6966 6965 6420 6c6f 6361  n specified loca
+00002770: 6c20 666f 6c64 6572 2074 6f20 6120 776f  l folder to a wo
+00002780: 726b 7370 6163 650d 0a0d 0a30 2e30 2e31  rkspace....0.0.1
+00002790: 3420 2832 372f 3037 2f32 3032 3229 0d0a  4 (27/07/2022)..
+000027a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000027b0: 2d2d 0d0a 2d20 4164 6469 6e67 2061 6c6d  --..- Adding alm
+000027c0: 6f73 7420 616c 6c20 6761 7465 7761 7920  ost all gateway 
+000027d0: 6361 7465 676f 7279 2072 6571 7565 7374  category request
+000027e0: 730d 0a2d 2041 6464 696e 6720 6e65 7720  s..- Adding new 
+000027f0: 7370 6563 6961 6c20 7265 7175 6573 7420  special request 
+00002800: 6672 6f6d 206c 6164 6174 6177 6562 2e20  from ladataweb. 
+00002810: 4d69 6772 6174 696e 6720 7265 706f 7274  Migrating report
+00002820: 7320 6265 7477 6565 6e20 776f 726b 7370  s between worksp
+00002830: 6163 6573 2e20 496d 706f 7274 696e 6720  aces. Importing 
+00002840: 7062 6978 2066 696c 6573 2066 726f 6d20  pbix files from 
+00002850: 5265 706f 6e73 652e 436f 6e74 656e 7420  Reponse.Content 
+00002860: 7265 7175 6573 7473 206c 6962 7261 7279  requests library
+00002870: 2074 6f20 6120 506f 7765 7220 4269 2053   to a Power Bi S
+00002880: 6572 7669 6365 2057 6f72 6b73 7061 6365  ervice Workspace
+00002890: 0d0a 0d0a 302e 302e 3135 2028 3038 2f30  ....0.0.15 (08/0
+000028a0: 382f 3230 3232 290d 0a2d 2d2d 2d2d 2d2d  8/2022)..-------
+000028b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a2d 2041  -----------..- A
+000028c0: 6464 696e 6720 6361 7061 6369 7469 6573  dding capacities
+000028d0: 2063 6174 6567 6f72 7920 7265 7175 6573   category reques
+000028e0: 7473 2e0d 0a2d 2046 6978 696e 6720 6465  ts...- Fixing de
+000028f0: 7363 7269 7074 696f 6e73 0d0a 0d0a 302e  scriptions....0.
+00002900: 312e 3020 2830 332f 3130 2f32 3032 3229  1.0 (03/10/2022)
+00002910: 0d0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ..--------------
+00002920: 2d2d 2d2d 0d0a 2d20 4164 6469 6e67 2070  ----..- Adding p
+00002930: 6970 656c 696e 6573 2061 6e64 2073 636f  ipelines and sco
+00002940: 7265 6361 7264 7320 6361 7465 676f 7279  recards category
+00002950: 2072 6571 7565 7374 732e 0d0a 2d20 416c   requests...- Al
+00002960: 6c20 636f 6d70 6f6e 656e 7465 7320 6361  l componentes ca
+00002970: 7465 676f 7279 2061 7265 206e 6f77 2061  tegory are now a
+00002980: 7661 696c 6162 6c65 2077 6974 6820 6120  vailable with a 
+00002990: 6c69 7474 6c65 206d 6973 7369 6e67 2065  little missing e
+000029a0: 6e64 706f 696e 7473 0d0a 2d20 436f 6d70  ndpoints..- Comp
+000029b0: 6c65 7469 6e67 2061 7420 6c65 6173 7420  leting at least 
+000029c0: 3830 2520 6f66 2072 6571 7565 7374 2066  80% of request f
+000029d0: 6f72 2061 6c6c 206d 6f73 7420 6672 6571  or all most freq
+000029e0: 7565 6e74 2069 7465 6d73 2061 7420 506f  uent items at Po
+000029f0: 7765 7220 4269 2e20 5468 6520 6f6e 6c79  wer Bi. The only
+00002a00: 2063 6174 6567 6f72 6965 7320 756e 6176   categories unav
+00002a10: 6169 6c61 626c 6573 2061 7265 2070 7573  ailables are pus
+00002a20: 6820 6461 7461 7365 7473 2061 6e64 2065  h datasets and e
+00002a30: 6d62 6564 6469 6e67 2e0d 0a2d 2042 7567  mbedding...- Bug
+00002a40: 2066 6978 696e 6720 7265 7175 6573 7473   fixing requests
+00002a50: 200d 0a0d 0a30 2e31 2e31 2028 3330 2f30   ....0.1.1 (30/0
+00002a60: 312f 3230 3233 290d 0a2d 2d2d 2d2d 2d2d  1/2023)..-------
+00002a70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a4d 696e  -----------..Min
+00002a80: 6f72 2062 7567 2066 6978 696e 6720 666f  or bug fixing fo
+00002a90: 7220 696d 706f 7274 7320 746f 2072 6561  r imports to rea
+00002aa0: 6420 6669 6c65 7379 7374 656d 0d0a 0d0a  d filesystem....
+00002ab0: 302e 312e 3220 2831 342f 3032 2f32 3032  0.1.2 (14/02/202
+00002ac0: 3329 0d0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  3)..------------
+00002ad0: 2d2d 2d2d 2d2d 0d0a 496d 7072 6f76 696e  ------..Improvin
+00002ae0: 6720 6765 7420 6163 7469 7669 7479 2065  g get activity e
+00002af0: 7665 6e74 7320 666f 7220 7369 6e67 6c65  vents for single
+00002b00: 2064 6179 2061 6674 6572 2050 6f77 6572   day after Power
+00002b10: 4269 2075 7064 6174 6573 2e0d 0a41 6464  Bi updates...Add
+00002b20: 696e 6720 6e65 7720 7265 7175 6573 7420  ing new request 
+00002b30: 746f 2067 6574 206c 6173 7420 3330 2064  to get last 30 d
+00002b40: 6179 7320 6f66 2061 6374 6976 6974 7920  ays of activity 
+00002b50: 6c6f 6773 2061 7574 6f6d 6174 6963 616c  logs automatical
+00002b60: 6c79 2e0d 0a0d 0a30 2e31 2e33 2028 3038  ly.....0.1.3 (08
+00002b70: 2f30 352f 3230 3233 290d 0a2d 2d2d 2d2d  /05/2023)..-----
+00002b80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a41  -------------..A
+00002b90: 6464 696e 6720 7570 6461 7465 2073 6f75  dding update sou
+00002ba0: 7263 6573 2066 6f72 2064 6174 6173 6574  rces for dataset
+00002bb0: 732e 2049 7427 7320 6120 636f 6d70 6c65  s. It's a comple
+00002bc0: 7820 626f 6479 2072 6571 7565 7374 2e0d  x body request..
+00002bd0: 0a41 6464 696e 6720 6e65 7720 756e 6971  .Adding new uniq
+00002be0: 7565 2072 6571 7565 7374 2066 6f72 2070  ue request for p
+00002bf0: 7562 6c69 7368 696e 6720 7062 6978 2066  ublishing pbix f
+00002c00: 696c 6520 6672 6f6d 2061 7a75 7265 2064  ile from azure d
+00002c10: 6576 6f70 7320 7265 706f 2e0d 0a43 6861  evops repo...Cha
+00002c20: 6e67 696e 6720 7061 6e64 6173 2063 6f64  nging pandas cod
+00002c30: 696e 6720 746f 2077 6f72 6b20 7769 7468  ing to work with
+00002c40: 2032 2e30 2e31 2076 6572 7369 6f6e 2e20   2.0.1 version. 
+00002c50: 4669 7869 6e67 2064 6570 7265 6361 7465  Fixing deprecate
+00002c60: 6420 6d65 7468 6f64 732e 0d0a            d methods...
```

## Comparing `SimplePBI-0.1.2.dist-info/RECORD` & `SimplePBI-0.1.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 simplepbi/__init__.py,sha256=6rG794o_Pw51N-rJOU--X3zs5TznwOk9vk7tNsw4E8Y,643
-simplepbi/admin/__init__.py,sha256=QcjfSzPst1eLHVNdoR6YLQQheYvO0LXeTIRE_f8gjSQ,86402
+simplepbi/admin/__init__.py,sha256=NGjCelRo8LUTDIkPNI5RlDWtcIfKApnmWGoAhbDE8S8,86420
 simplepbi/apps/__init__.py,sha256=vo6-DtuprZx9dfLqc6jeMvRVGYvNNj9QX4mpSfK15GY,9878
 simplepbi/capacities/__init__.py,sha256=1t9ancMJvpzht931qvto3Oah3Zjn-Ut2KFEq3-Ap10o,15534
 simplepbi/dashboards/__init__.py,sha256=TtH4u-wxKF7_C7byIFODavxb8flJiIyzxc-PdnpM7Ns,17252
 simplepbi/dataflows/__init__.py,sha256=QGP2rX4zeVQ44NUf0W8eP5Wm_zzwj8G52TxFNG3jnSA,15322
-simplepbi/datasets/__init__.py,sha256=P_Fa3DZ5sEKqiLJMVi1LiqQ2wooEHjwSibGNw6OPOwU,55768
+simplepbi/datasets/__init__.py,sha256=dqNLkYTUJIf-VKrVSUfBdA-mBNhCK6Ssylj-JHL0E3E,58028
 simplepbi/gateways/__init__.py,sha256=ol1eZBIAT0v764BCUSHMzhA4-e3FDh77I8D_wCWLSz8,16099
 simplepbi/groups/__init__.py,sha256=acPort3e99ajdTKXhLWvnGWevVIuaM3IBRrUjkIYTsY,14147
-simplepbi/imports/__init__.py,sha256=RxR6lWvxAnb7NAA0NSLpD7_seoLwOkA0nEgdN5ecmYQ,22377
+simplepbi/imports/__init__.py,sha256=GSgWOLBpBnvEyiQH6qjQxk-2E-4atBd8RgCWo0P03Gk,24405
 simplepbi/pipelines/__init__.py,sha256=KtmtGa1049qqtCCclaNB7_fBAv56PGIVMrWp4v-B9uQ,24126
 simplepbi/reports/__init__.py,sha256=x25_H-PVITI37luFK73BQdwIRD60nG9zRmnMhYPoJvU,44427
 simplepbi/scorecards/__init__.py,sha256=eb6Z4q6dasdPcGtsxTqbupkIhMo_sAHM98fgtqiCH4A,12740
 simplepbi/token/__init__.py,sha256=sT8EgSn3RQ-gbqmVPxVux37S_mUnLIm_0qQRkd6qqAw,4093
-simplepbi/utils/__init__.py,sha256=wiKw864ZTLucwhlmGqJbkiwg35pn2nK-7j8OfxC9TT8,3451
-SimplePBI-0.1.2.dist-info/LICENSE,sha256=ZtpzRFk5l7aVPep5WYvScxZ-tc4yiqgCR41jLTgns5I,1072
-SimplePBI-0.1.2.dist-info/METADATA,sha256=Zn31yXpH03FmawzrxpQUs-dzxJFnW-6oYEv4Bac-zLM,10491
-SimplePBI-0.1.2.dist-info/WHEEL,sha256=v8slff5hmCpvciQ3G55d2d1CnOBupjDFJHDE2dUb1Ao,97
-SimplePBI-0.1.2.dist-info/top_level.txt,sha256=IwRTqkuCr1bqy2LPIIj4_aHuRc9NNLgtB8VxuIl_OnM,10
-SimplePBI-0.1.2.dist-info/RECORD,,
+simplepbi/utils/__init__.py,sha256=k2Opnd02zwaXUocHmgUvaqFRjfvU14L5IfA0LaMHzjQ,3457
+SimplePBI-0.1.3.dist-info/LICENSE,sha256=ZtpzRFk5l7aVPep5WYvScxZ-tc4yiqgCR41jLTgns5I,1072
+SimplePBI-0.1.3.dist-info/METADATA,sha256=gtlfwH_mkIuM8t4SKcDL4lZMAX3P-OwDpz7RaByjzT8,11372
+SimplePBI-0.1.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+SimplePBI-0.1.3.dist-info/top_level.txt,sha256=IwRTqkuCr1bqy2LPIIj4_aHuRc9NNLgtB8VxuIl_OnM,10
+SimplePBI-0.1.3.dist-info/RECORD,,
```

