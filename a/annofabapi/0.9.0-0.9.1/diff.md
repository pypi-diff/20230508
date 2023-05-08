# Comparing `tmp/annofabapi-0.9.0.tar.gz` & `tmp/annofabapi-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/annofabapi-0.9.0.tar", last modified: Fri Jul 19 07:36:20 2019, max compression
+gzip compressed data, was "dist/annofabapi-0.9.1.tar", last modified: Fri Jul 26 03:18:02 2019, max compression
```

## Comparing `annofabapi-0.9.0.tar` & `annofabapi-0.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-07-19 07:36:20.000000 annofabapi-0.9.0/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     6626 2019-07-19 07:36:20.000000 annofabapi-0.9.0/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1356 2019-07-02 07:49:55.000000 annofabapi-0.9.0/setup.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-07-19 07:36:20.000000 annofabapi-0.9.0/annofabapi.egg-info/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      553 2019-07-19 07:36:20.000000 annofabapi-0.9.0/annofabapi.egg-info/SOURCES.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2019-07-19 07:36:20.000000 annofabapi-0.9.0/annofabapi.egg-info/dependency_links.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     6626 2019-07-19 07:36:20.000000 annofabapi-0.9.0/annofabapi.egg-info/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       17 2019-07-19 07:36:20.000000 annofabapi-0.9.0/annofabapi.egg-info/top_level.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       33 2019-07-19 07:36:20.000000 annofabapi-0.9.0/annofabapi.egg-info/requires.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      320 2019-07-19 07:36:20.000000 annofabapi-0.9.0/setup.cfg
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-07-19 07:36:20.000000 annofabapi-0.9.0/annofabapi/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    58348 2019-07-19 07:29:04.000000 annofabapi-0.9.0/annofabapi/models.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      162 2019-07-06 12:39:09.000000 annofabapi-0.9.0/annofabapi/exceptions.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2738 2019-07-16 02:43:47.000000 annofabapi-0.9.0/annofabapi/resource.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      237 2019-07-04 10:59:56.000000 annofabapi-0.9.0/annofabapi/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2071 2019-07-16 01:59:37.000000 annofabapi-0.9.0/annofabapi/utils.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4133 2019-07-16 02:43:48.000000 annofabapi-0.9.0/annofabapi/api2.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)   109680 2019-07-19 07:29:04.000000 annofabapi-0.9.0/annofabapi/generated_api.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7895 2019-07-16 02:43:49.000000 annofabapi-0.9.0/annofabapi/api.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       22 2019-07-19 07:31:42.000000 annofabapi-0.9.0/annofabapi/__version__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     8354 2019-07-19 07:29:04.000000 annofabapi-0.9.0/annofabapi/generated_api2.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    29294 2019-07-16 02:43:49.000000 annofabapi-0.9.0/annofabapi/wrapper.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-07-19 07:36:20.000000 annofabapi-0.9.0/tests/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-05-13 01:07:51.000000 annofabapi-0.9.0/tests/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      759 2019-07-02 07:30:09.000000 annofabapi-0.9.0/tests/test_resource.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    16965 2019-07-14 13:04:32.000000 annofabapi-0.9.0/tests/test_api.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1363 2019-07-01 13:00:50.000000 annofabapi-0.9.0/tests/test_api2.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1574 2019-07-16 02:43:50.000000 annofabapi-0.9.0/tests/utils_for_test.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4668 2019-07-04 13:07:17.000000 annofabapi-0.9.0/README.md
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-07-26 03:18:02.000000 annofabapi-0.9.1/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     6626 2019-07-26 03:18:02.000000 annofabapi-0.9.1/PKG-INFO
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4668 2019-07-04 13:07:17.000000 annofabapi-0.9.1/README.md
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-07-26 03:18:02.000000 annofabapi-0.9.1/annofabapi/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      237 2019-07-04 10:59:56.000000 annofabapi-0.9.1/annofabapi/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       22 2019-07-26 03:17:08.000000 annofabapi-0.9.1/annofabapi/__version__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7895 2019-07-22 03:01:22.000000 annofabapi-0.9.1/annofabapi/api.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4133 2019-07-16 02:43:48.000000 annofabapi-0.9.1/annofabapi/api2.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      162 2019-07-06 12:39:09.000000 annofabapi-0.9.1/annofabapi/exceptions.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)   109722 2019-07-26 03:15:25.000000 annofabapi-0.9.1/annofabapi/generated_api.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     8354 2019-07-26 03:15:25.000000 annofabapi-0.9.1/annofabapi/generated_api2.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    60152 2019-07-26 03:15:26.000000 annofabapi-0.9.1/annofabapi/models.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2738 2019-07-16 02:43:47.000000 annofabapi-0.9.1/annofabapi/resource.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2071 2019-07-16 01:59:37.000000 annofabapi-0.9.1/annofabapi/utils.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    29476 2019-07-25 07:13:28.000000 annofabapi-0.9.1/annofabapi/wrapper.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-07-26 03:18:02.000000 annofabapi-0.9.1/annofabapi.egg-info/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     6626 2019-07-26 03:18:02.000000 annofabapi-0.9.1/annofabapi.egg-info/PKG-INFO
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      553 2019-07-26 03:18:02.000000 annofabapi-0.9.1/annofabapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2019-07-26 03:18:02.000000 annofabapi-0.9.1/annofabapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       33 2019-07-26 03:18:02.000000 annofabapi-0.9.1/annofabapi.egg-info/requires.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       17 2019-07-26 03:18:02.000000 annofabapi-0.9.1/annofabapi.egg-info/top_level.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1592 2019-07-26 03:18:02.000000 annofabapi-0.9.1/setup.cfg
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1356 2019-07-02 07:49:55.000000 annofabapi-0.9.1/setup.py
+drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-07-26 03:18:02.000000 annofabapi-0.9.1/tests/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        0 2019-05-13 01:07:51.000000 annofabapi-0.9.1/tests/__init__.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    16965 2019-07-14 13:04:32.000000 annofabapi-0.9.1/tests/test_api.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1363 2019-07-01 13:00:50.000000 annofabapi-0.9.1/tests/test_api2.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      759 2019-07-02 07:30:09.000000 annofabapi-0.9.1/tests/test_resource.py
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1574 2019-07-16 02:43:50.000000 annofabapi-0.9.1/tests/utils_for_test.py
```

### Comparing `annofabapi-0.9.0/PKG-INFO` & `annofabapi-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annofabapi
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python Clinet Library of AnnoFab API (https://annofab.com/docs/api/)
 Home-page: https://github.com/kurusugawa-computer/annofab-api-python-client
 Author: yuji38kwmt
 Author-email: yuji38kwmt@gmail.com
 Maintainer: yuji38kwmt
 License: MIT
 Description: # annofab-api-python-client
```

### Comparing `annofabapi-0.9.0/setup.py` & `annofabapi-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `annofabapi-0.9.0/annofabapi.egg-info/SOURCES.txt` & `annofabapi-0.9.1/annofabapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `annofabapi-0.9.0/annofabapi.egg-info/PKG-INFO` & `annofabapi-0.9.1/annofabapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annofabapi
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python Clinet Library of AnnoFab API (https://annofab.com/docs/api/)
 Home-page: https://github.com/kurusugawa-computer/annofab-api-python-client
 Author: yuji38kwmt
 Author-email: yuji38kwmt@gmail.com
 Maintainer: yuji38kwmt
 License: MIT
 Description: # annofab-api-python-client
```

### Comparing `annofabapi-0.9.0/annofabapi/models.py` & `annofabapi-0.9.1/annofabapi/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,155 @@
 
 Note:
     このファイルはopenapi-generatorで自動生成される。詳細は generate/README.mdを参照
 """
 
 import warnings  # pylint: disable=unused-import
 from enum import Enum
-from typing import Any, Dict, List, Optional, Tuple, Union  # pylint: disable=unused-import
+from typing import Any, Dict, List, NewType, Optional, Tuple, Union  # pylint: disable=unused-import
 
-AcceptOrganizationInvitationRequest = Dict[str, Any]
+### 手動の部分
+
+AccountId = NewType('AccountId', str)
+"""
+
+Example:
+    ``12345678-abcd-1234-abcd-1234abcd5678``
+    
+"""
+
+UserId = NewType('UserId', str)
+"""
+
+Example:
+    ``john_doe``
+
+"""
+
+OrganizationId = NewType('OrganizationId', str)
+"""
+
+Example:
+    ``12345678-abcd-1234-abcd-1234abcd5678``
+
+"""
+
+ProjectId = NewType('ProjectId', str)
+"""
+
+Example:
+    ``12345678-abcd-1234-abcd-1234abcd5678``
+
+"""
+
+LabelId = NewType('LabelId', str)
+"""
+
+Example:
+    ``12345678-abcd-1234-abcd-1234abcd5678``
+
+"""
+
+AdditionalDataDefinitionId = NewType('AdditionalDataDefinitionId', str)
+"""
+
+Example:
+    ``12345678-abcd-1234-abcd-1234abcd5678``
+
+"""
+
+ChoiceId = NewType('ChoiceId', str)
+"""
+
+Example:
+    ``12345678-abcd-1234-abcd-1234abcd5678``
+
+"""
+
+PhraseId = NewType('PhraseId', str)
+"""
+
+Example:
+    ``my_phrase_id``
+
+"""
+
+TaskId = NewType('TaskId', str)
+"""
+
+Example:
+    ``12345678-abcd-1234-abcd-1234abcd5678``
+
+"""
+
+InputDataId = NewType('InputDataId', str)
+"""
+
+Example:
+    ``12345678-abcd-1234-abcd-1234abcd5678``
+
+"""
+
+SupplementaryDataId = NewType('SupplementaryDataId', str)
+"""
+
+Example:
+    ``12345678-abcd-1234-abcd-1234abcd5678``
+
+"""
+
+TaskHistoryId = NewType('TaskHistoryId', str)
+"""
+
+Example:
+    ``12345678-abcd-1234-abcd-1234abcd5678``
+
+"""
+
+AnnotationId = NewType('AnnotationId', str)
+"""
+
+Example:
+    ``12345678-abcd-1234-abcd-1234abcd5678``
+
+"""
+
+InspectionId = NewType('InspectionId', str)
+"""
+
+Example:
+    ``12345678-abcd-1234-abcd-1234abcd5678``
+
+"""
+
+JobId = NewType('JobId', str)
+"""
+
+Example:
+    ``12345678-abcd-1234-abcd-1234abcd5678``
+
+"""
+
+WebhookId = NewType('WebhookId', str)
+"""
+
+Example:
+    ``12345678-abcd-1234-abcd-1234abcd5678``
+
+"""
+
+Duration = NewType('Duration', str)
+"""
+
+Example:
+    ``PT34H17M36.789S``
+
+"""
+
+### 以下は自動生成の部分AcceptOrganizationInvitationRequest = Dict[str, Any]
 """
 
 
 Kyes of Dict
 
 * token: str
```

### Comparing `annofabapi-0.9.0/annofabapi/resource.py` & `annofabapi-0.9.1/annofabapi/resource.py`

 * *Files identical despite different names*

### Comparing `annofabapi-0.9.0/annofabapi/utils.py` & `annofabapi-0.9.1/annofabapi/utils.py`

 * *Files identical despite different names*

### Comparing `annofabapi-0.9.0/annofabapi/api2.py` & `annofabapi-0.9.1/annofabapi/api2.py`

 * *Files identical despite different names*

### Comparing `annofabapi-0.9.0/annofabapi/generated_api.py` & `annofabapi-0.9.1/annofabapi/generated_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,15 @@
 
     def get_archive_full_with_pro_id(
             self,
             project_id: str,
     ) -> Tuple[Any, requests.Response]:
         """fullアノテーションZIP取得
 
-        DEPRECATED
+        .. deprecated:: X
 
         authorizations: ProjectDataUser
 
 
         **このAPIは廃止予定です。fullアノテーションZIPにある情報で、simpleアノテーションZIPにも欲しいものがあれば、ご連絡ください。**  プロジェクト内のアノテーション（full版）がまとめられたZIPを取得します。  full版のアノテーションJSONデータは、画像やアノテーションやアノテーション作成者など管理用の詳細情報が付随しています。機械学習での一般的な利用には、[詳細情報を省いた扱いやすい構造の simple版](#operation/getAnnotationArchive) を推奨します。  取得できるZIPファイルの構造は以下のとおりです。  * ファイル名: af-annotation-{プロジェクトID}-{更新日時: yyyyMMdd-hhmmss}.zip * 内容: /   * {タスクID}/     * {入力データID}.json       * アノテーションJSONデータ (詳細は 200レスポンス を参照)     * {入力データID}/ (塗りつぶしアノテーション時のみ)       * combined/         * {ラベルID} (ラベルごとに結合した塗りつぶしのPNG画像)       * {アノテーションデータID} (塗りつぶしのPNG画像) 
 
         Args:
@@ -428,15 +428,15 @@
             project_id: str,
             task_id: str,
             input_data_id: str,
             annotation_id: str,
     ) -> Tuple[Any, requests.Response]:
         """【エディタ用】外部ファイル形式のアノテーション取得
 
-        DEPRECATED
+        .. deprecated:: X
 
         authorizations: AllProjectMember
 
 
         このAPIが返すアノテーションは、エディタ用です。 機械学習などで利用する成果物としてのアノテーションを取得するには、以下をご利用いただけます。  * [getAnnotation](#operation/getAnnotation): 特定のタスク - 入力データのアノテーション取得 * [getAnnotationArchive](#operation/getAnnotationArchive): プロジェクト全体のアノテーション（ZIP） 
 
         Args:
@@ -717,15 +717,15 @@
     def get_signed_url_of_input_data(
             self,
             project_id: str,
             input_data_id: str,
     ) -> Tuple[Any, requests.Response]:
         """実体参照用認証済みURL取得
 
-        DEPRECATED
+        .. deprecated:: X
 
         authorizations: AllProjectMember
 
 
         入力データの実体（画像や動画などのファイルそのもの）にアクセスするための、認証済み一時URLを取得します。  取得したURLは、1時間で失効し、アクセスできなくなります。 
 
         Args:
@@ -2194,15 +2194,15 @@
             self,
             project_id: str,
             task_id: str,
             task_history_id: str,
     ) -> Tuple[Any, requests.Response]:
         """タスク履歴取得
 
-        DEPRECATED
+        .. deprecated:: X
 
         authorizations: AllProjectMember
 
 
 
         Args:
             project_id (str):  プロジェクトID (required)
@@ -2223,15 +2223,15 @@
     def get_history_events_with_pro_id_tas_id(
             self,
             project_id: str,
             task_id: str,
     ) -> Tuple[Any, requests.Response]:
         """タスク履歴イベント取得
 
-        DEPRECATED
+        .. deprecated:: X
 
         authorizations: AllProjectMember
 
 
         作業時間を計算したタスク履歴ではなく、その元となったタスク履歴イベントを一括で取得します。 
 
         Args:
@@ -2373,15 +2373,15 @@
 
     def get_tasks_inputs_with_pro_id(
             self,
             project_id: str,
     ) -> Tuple[Any, requests.Response]:
         """【非推奨】タスク-入力データ一括取得
 
-        DEPRECATED
+        .. deprecated:: X
 
         authorizations: AllProjectMember
 
 
 
         Args:
             project_id (str):  プロジェクトID (required)
```

### Comparing `annofabapi-0.9.0/annofabapi/api.py` & `annofabapi-0.9.1/annofabapi/api.py`

 * *Files identical despite different names*

### Comparing `annofabapi-0.9.0/annofabapi/generated_api2.py` & `annofabapi-0.9.1/annofabapi/generated_api2.py`

 * *Files identical despite different names*

### Comparing `annofabapi-0.9.0/annofabapi/wrapper.py` & `annofabapi-0.9.1/annofabapi/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,16 @@
         copied_query_params = copy.deepcopy(arg_query_params) if arg_query_params is not None else {}
 
         all_objects: List[Dict[str, Any]] = []
 
         copied_query_params.update({"page": 1, "limit": limit})
         kwargs_for_func_get_list['query_params'] = copied_query_params
         content, _ = func_get_list(**kwargs_for_func_get_list)
+        if content.get('over_limit'):
+            logger.warning(f"検索結果が10,000件を超えてますが、Web APIの都合上10,000件までしか取得できません。")
 
         all_objects.extend(content["list"])
 
         while content["page_no"] < content["total_page_no"]:
             next_page_no = content["page_no"] + 1
             copied_query_params.update({"page": next_page_no})
             kwargs_for_func_get_list['query_params'] = copied_query_params
```

### Comparing `annofabapi-0.9.0/tests/test_resource.py` & `annofabapi-0.9.1/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `annofabapi-0.9.0/tests/test_api.py` & `annofabapi-0.9.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `annofabapi-0.9.0/tests/test_api2.py` & `annofabapi-0.9.1/tests/test_api2.py`

 * *Files identical despite different names*

### Comparing `annofabapi-0.9.0/tests/utils_for_test.py` & `annofabapi-0.9.1/tests/utils_for_test.py`

 * *Files identical despite different names*

### Comparing `annofabapi-0.9.0/README.md` & `annofabapi-0.9.1/README.md`

 * *Files identical despite different names*

