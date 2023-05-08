# Comparing `tmp/mypy-boto3-glue-1.26.74.tar.gz` & `tmp/mypy-boto3-glue-1.26.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-glue-1.26.74.tar", last modified: Fri Feb 17 20:26:41 2023, max compression
+gzip compressed data, was "mypy-boto3-glue-1.26.8.tar", last modified: Fri Nov 11 21:07:54 2022, max compression
```

## Comparing `mypy-boto3-glue-1.26.74.tar` & `mypy-boto3-glue-1.26.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 20:26:41.051546 mypy-boto3-glue-1.26.74/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-17 20:26:21.000000 mypy-boto3-glue-1.26.74/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41749 2023-02-17 20:26:41.051546 mypy-boto3-glue-1.26.74/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40274 2023-02-17 20:26:21.000000 mypy-boto3-glue-1.26.74/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 20:26:41.051546 mypy-boto3-glue-1.26.74/mypy_boto3_glue/
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-02-17 20:26:21.000000 mypy-boto3-glue-1.26.74/mypy_boto3_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-02-17 20:26:21.000000 mypy-boto3-glue-1.26.74/mypy_boto3_glue/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-02-17 20:26:22.000000 mypy-boto3-glue-1.26.74/mypy_boto3_glue/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   136828 2023-02-17 20:26:23.000000 mypy-boto3-glue-1.26.74/mypy_boto3_glue/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   136600 2023-02-17 20:26:22.000000 mypy-boto3-glue-1.26.74/mypy_boto3_glue/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20307 2023-02-17 20:26:24.000000 mypy-boto3-glue-1.26.74/mypy_boto3_glue/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    20305 2023-02-17 20:26:23.000000 mypy-boto3-glue-1.26.74/mypy_boto3_glue/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21235 2023-02-17 20:26:23.000000 mypy-boto3-glue-1.26.74/mypy_boto3_glue/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21214 2023-02-17 20:26:23.000000 mypy-boto3-glue-1.26.74/mypy_boto3_glue/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 20:26:22.000000 mypy-boto3-glue-1.26.74/mypy_boto3_glue/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   248914 2023-02-17 20:26:29.000000 mypy-boto3-glue-1.26.74/mypy_boto3_glue/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   248543 2023-02-17 20:26:26.000000 mypy-boto3-glue-1.26.74/mypy_boto3_glue/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-17 20:26:21.000000 mypy-boto3-glue-1.26.74/mypy_boto3_glue/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 20:26:41.051546 mypy-boto3-glue-1.26.74/mypy_boto3_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41749 2023-02-17 20:26:40.000000 mypy-boto3-glue-1.26.74/mypy_boto3_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-02-17 20:26:40.000000 mypy-boto3-glue-1.26.74/mypy_boto3_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 20:26:40.000000 mypy-boto3-glue-1.26.74/mypy_boto3_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 20:26:40.000000 mypy-boto3-glue-1.26.74/mypy_boto3_glue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-17 20:26:40.000000 mypy-boto3-glue-1.26.74/mypy_boto3_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-17 20:26:40.000000 mypy-boto3-glue-1.26.74/mypy_boto3_glue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 20:26:41.051546 mypy-boto3-glue-1.26.74/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-02-17 20:26:21.000000 mypy-boto3-glue-1.26.74/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.082122 mypy-boto3-glue-1.26.8/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-11 21:07:11.000000 mypy-boto3-glue-1.26.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    38830 2022-11-11 21:07:54.074122 mypy-boto3-glue-1.26.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    37407 2022-11-11 21:07:11.000000 mypy-boto3-glue-1.26.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.070122 mypy-boto3-glue-1.26.8/mypy_boto3_glue/
+-rw-r--r--   0 runner    (1001) docker     (121)     4090 2022-11-11 21:07:11.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4089 2022-11-11 21:07:11.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      893 2022-11-11 21:07:11.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   126110 2022-11-11 21:07:12.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)   125898 2022-11-11 21:07:11.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    19003 2022-11-11 21:07:13.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/literals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19001 2022-11-11 21:07:12.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    21235 2022-11-11 21:07:12.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21214 2022-11-11 21:07:12.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:11.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)   222337 2022-11-11 21:07:17.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (121)   222006 2022-11-11 21:07:15.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-11 21:07:11.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 21:07:54.074122 mypy-boto3-glue-1.26.8/mypy_boto3_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    38830 2022-11-11 21:07:53.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2022-11-11 21:07:53.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 21:07:53.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 21:07:53.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-11 21:07:53.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-11 21:07:53.000000 mypy-boto3-glue-1.26.8/mypy_boto3_glue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 21:07:54.082122 mypy-boto3-glue-1.26.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1930 2022-11-11 21:07:10.000000 mypy-boto3-glue-1.26.8/setup.py
```

### Comparing `mypy-boto3-glue-1.26.74/LICENSE` & `mypy-boto3-glue-1.26.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.26.74/PKG-INFO` & `mypy-boto3-glue-1.26.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-glue
-Version: 1.26.74
-Summary: Type annotations for boto3.Glue 1.26.74 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.8
+Summary: Type annotations for boto3.Glue 1.26.8 service generated with mypy-boto3-builder 7.11.10
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,15 +18,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -38,24 +37,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-glue?color=blue)](https://pypistats.org/packages/mypy-boto3-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glue 1.26.74](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[boto3.Glue 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-glue docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/).
 
 See how it helps to find and fix potential bugs:
 
@@ -363,20 +362,16 @@
     ConnectionPropertyKeyType,
     ConnectionTypeType,
     CrawlStateType,
     CrawlerHistoryStateType,
     CrawlerLineageSettingsType,
     CrawlerStateType,
     CsvHeaderOptionType,
-    DQStopJobOnFailureTimingType,
-    DQTransformOutputType,
     DataFormatType,
-    DataQualityRuleResultStatusType,
     DeleteBehaviorType,
-    DeltaTargetCompressionTypeType,
     EnableHybridValuesType,
     ExecutionClassType,
     ExistConditionType,
     FieldNameType,
     FilterLogicalOperatorType,
     FilterOperationType,
     FilterOperatorType,
@@ -394,31 +389,27 @@
     GetResourcePoliciesPaginatorName,
     GetSecurityConfigurationsPaginatorName,
     GetTableVersionsPaginatorName,
     GetTablesPaginatorName,
     GetTriggersPaginatorName,
     GetUserDefinedFunctionsPaginatorName,
     GlueRecordTypeType,
-    HudiTargetCompressionTypeType,
-    JDBCConnectionTypeType,
     JDBCDataTypeType,
-    JdbcMetadataEntryType,
     JobBookmarksEncryptionModeType,
     JobRunStateType,
     JoinTypeType,
     LanguageType,
     LastCrawlStatusType,
     ListRegistriesPaginatorName,
     ListSchemaVersionsPaginatorName,
     ListSchemasPaginatorName,
     LogicalOperatorType,
     LogicalType,
     MLUserDataEncryptionModeStringType,
     NodeTypeType,
-    ParamTypeType,
     ParquetCompressionTypeType,
     PartitionIndexStatusType,
     PermissionType,
     PermissionTypeType,
     PiiTypeType,
     PrincipalTypeType,
     QuoteCharType,
@@ -485,29 +476,26 @@
     ErrorDetailTypeDef,
     BatchDeleteTableRequestRequestTypeDef,
     BatchDeleteTableVersionRequestRequestTypeDef,
     BatchGetBlueprintsRequestRequestTypeDef,
     BatchGetCrawlersRequestRequestTypeDef,
     BatchGetCustomEntityTypesRequestRequestTypeDef,
     CustomEntityTypeTypeDef,
-    BatchGetDataQualityResultRequestRequestTypeDef,
     BatchGetDevEndpointsRequestRequestTypeDef,
     DevEndpointTypeDef,
     BatchGetJobsRequestRequestTypeDef,
     BatchGetTriggersRequestRequestTypeDef,
     BatchGetWorkflowsRequestRequestTypeDef,
     BatchStopJobRunRequestRequestTypeDef,
     BatchStopJobRunSuccessfulSubmissionTypeDef,
     BinaryColumnStatisticsDataTypeDef,
     BlueprintDetailsTypeDef,
     BlueprintRunTypeDef,
     LastActiveDefinitionTypeDef,
     BooleanColumnStatisticsDataTypeDef,
-    CancelDataQualityRuleRecommendationRunRequestRequestTypeDef,
-    CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef,
     CancelMLTaskRunRequestRequestTypeDef,
     CancelStatementRequestRequestTypeDef,
     CatalogEntryTypeDef,
     CatalogImportStatusTypeDef,
     KafkaStreamingSourceOptionsTypeDef,
     StreamingDataPreviewOptionsTypeDef,
     KinesisStreamingSourceOptionsTypeDef,
@@ -516,15 +504,14 @@
     CatalogTargetTypeDef,
     CheckSchemaVersionValidityInputRequestTypeDef,
     CsvClassifierTypeDef,
     GrokClassifierTypeDef,
     JsonClassifierTypeDef,
     XMLClassifierTypeDef,
     CloudWatchEncryptionTypeDef,
-    DirectJDBCSourceTypeDef,
     DropDuplicatesTypeDef,
     DropFieldsTypeDef,
     DynamoDBCatalogSourceTypeDef,
     FillMissingValuesTypeDef,
     MergeTypeDef,
     MicrosoftSQLServerCatalogSourceTypeDef,
     MicrosoftSQLServerCatalogTargetTypeDef,
@@ -574,43 +561,37 @@
     CrawlsFilterTypeDef,
     CreateBlueprintRequestRequestTypeDef,
     CreateCsvClassifierRequestTypeDef,
     CreateGrokClassifierRequestTypeDef,
     CreateJsonClassifierRequestTypeDef,
     CreateXMLClassifierRequestTypeDef,
     CreateCustomEntityTypeRequestRequestTypeDef,
-    DataQualityTargetTableTypeDef,
     CreateDevEndpointRequestRequestTypeDef,
     ExecutionPropertyTypeDef,
     JobCommandTypeDef,
     SourceControlDetailsTypeDef,
     GlueTableTypeDef,
     PartitionIndexTypeDef,
     CreateRegistryInputRequestTypeDef,
     RegistryIdTypeDef,
     SessionCommandTypeDef,
     EventBatchingConditionTypeDef,
     CreateWorkflowRequestRequestTypeDef,
-    DQResultsPublishingOptionsTypeDef,
-    DQStopJobOnFailureOptionsTypeDef,
     EncryptionAtRestTypeDef,
     DataLakePrincipalTypeDef,
-    DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
-    DataQualityRuleResultTypeDef,
     DatabaseIdentifierTypeDef,
     DatatypeTypeDef,
     DecimalNumberTypeDef,
     DeleteBlueprintRequestRequestTypeDef,
     DeleteClassifierRequestRequestTypeDef,
     DeleteColumnStatisticsForPartitionRequestRequestTypeDef,
     DeleteColumnStatisticsForTableRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteCrawlerRequestRequestTypeDef,
     DeleteCustomEntityTypeRequestRequestTypeDef,
-    DeleteDataQualityRulesetRequestRequestTypeDef,
     DeleteDatabaseRequestRequestTypeDef,
     DeleteDevEndpointRequestRequestTypeDef,
     DeleteJobRequestRequestTypeDef,
     DeleteMLTransformRequestRequestTypeDef,
     DeletePartitionIndexRequestRequestTypeDef,
     DeletePartitionRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
@@ -621,15 +602,14 @@
     DeleteTableVersionRequestRequestTypeDef,
     DeleteTriggerRequestRequestTypeDef,
     DeleteUserDefinedFunctionRequestRequestTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     DevEndpointCustomLibrariesTypeDef,
     DirectSchemaChangePolicyTypeDef,
     NullCheckBoxListTypeDef,
-    TransformConfigParameterTypeDef,
     EdgeTypeDef,
     JobBookmarksEncryptionTypeDef,
     S3EncryptionTypeDef,
     ErrorDetailsTypeDef,
     ExportLabelsTaskRunPropertiesTypeDef,
     FilterValueTypeDef,
     FindMatchesParametersTypeDef,
@@ -646,18 +626,14 @@
     GetConnectionRequestRequestTypeDef,
     GetConnectionsFilterTypeDef,
     GetCrawlerMetricsRequestRequestTypeDef,
     GetCrawlerRequestRequestTypeDef,
     GetCrawlersRequestRequestTypeDef,
     GetCustomEntityTypeRequestRequestTypeDef,
     GetDataCatalogEncryptionSettingsRequestRequestTypeDef,
-    GetDataQualityResultRequestRequestTypeDef,
-    GetDataQualityRuleRecommendationRunRequestRequestTypeDef,
-    GetDataQualityRulesetEvaluationRunRequestRequestTypeDef,
-    GetDataQualityRulesetRequestRequestTypeDef,
     GetDatabaseRequestRequestTypeDef,
     GetDatabasesRequestRequestTypeDef,
     GetDataflowGraphRequestRequestTypeDef,
     GetDevEndpointRequestRequestTypeDef,
     GetDevEndpointsRequestRequestTypeDef,
     GetJobBookmarkRequestRequestTypeDef,
     JobBookmarkEntryTypeDef,
@@ -757,15 +733,14 @@
     UntagResourceRequestRequestTypeDef,
     UpdateBlueprintRequestRequestTypeDef,
     UpdateCsvClassifierRequestTypeDef,
     UpdateGrokClassifierRequestTypeDef,
     UpdateJsonClassifierRequestTypeDef,
     UpdateXMLClassifierRequestTypeDef,
     UpdateCrawlerScheduleRequestRequestTypeDef,
-    UpdateDataQualityRulesetRequestRequestTypeDef,
     UpdateJobFromSourceControlRequestRequestTypeDef,
     UpdateSourceControlFromJobRequestRequestTypeDef,
     UpdateWorkflowRequestRequestTypeDef,
     WorkflowRunStatisticsTypeDef,
     ActionTypeDef,
     StartJobRunRequestRequestTypeDef,
     AggregateTypeDef,
@@ -774,15 +749,14 @@
     BackfillErrorTypeDef,
     BatchDeletePartitionRequestRequestTypeDef,
     BatchGetPartitionRequestRequestTypeDef,
     CancelMLTaskRunResponseTypeDef,
     CheckSchemaVersionValidityResponseTypeDef,
     CreateBlueprintResponseTypeDef,
     CreateCustomEntityTypeResponseTypeDef,
-    CreateDataQualityRulesetResponseTypeDef,
     CreateDevEndpointResponseTypeDef,
     CreateJobResponseTypeDef,
     CreateMLTransformResponseTypeDef,
     CreateRegistryResponseTypeDef,
     CreateSchemaResponseTypeDef,
     CreateScriptResponseTypeDef,
     CreateSecurityConfigurationResponseTypeDef,
@@ -817,27 +791,24 @@
     PutResourcePolicyResponseTypeDef,
     PutSchemaVersionMetadataResponseTypeDef,
     RegisterSchemaVersionResponseTypeDef,
     RemoveSchemaVersionMetadataResponseTypeDef,
     ResumeWorkflowRunResponseTypeDef,
     RunStatementResponseTypeDef,
     StartBlueprintRunResponseTypeDef,
-    StartDataQualityRuleRecommendationRunResponseTypeDef,
-    StartDataQualityRulesetEvaluationRunResponseTypeDef,
     StartExportLabelsTaskRunResponseTypeDef,
     StartImportLabelsTaskRunResponseTypeDef,
     StartJobRunResponseTypeDef,
     StartMLEvaluationTaskRunResponseTypeDef,
     StartMLLabelingSetGenerationTaskRunResponseTypeDef,
     StartTriggerResponseTypeDef,
     StartWorkflowRunResponseTypeDef,
     StopSessionResponseTypeDef,
     StopTriggerResponseTypeDef,
     UpdateBlueprintResponseTypeDef,
-    UpdateDataQualityRulesetResponseTypeDef,
     UpdateJobFromSourceControlResponseTypeDef,
     UpdateJobResponseTypeDef,
     UpdateMLTransformResponseTypeDef,
     UpdateRegistryResponseTypeDef,
     UpdateSchemaResponseTypeDef,
     UpdateSourceControlFromJobResponseTypeDef,
     UpdateWorkflowResponseTypeDef,
@@ -859,60 +830,49 @@
     GetCatalogImportStatusResponseTypeDef,
     CatalogKafkaSourceTypeDef,
     DirectKafkaSourceTypeDef,
     CatalogKinesisSourceTypeDef,
     DirectKinesisSourceTypeDef,
     GovernedCatalogTargetTypeDef,
     S3CatalogTargetTypeDef,
-    S3DeltaCatalogTargetTypeDef,
-    S3HudiCatalogTargetTypeDef,
     ClassifierTypeDef,
     CodeGenNodeTypeDef,
     LocationTypeDef,
     PredicateTypeDef,
     FindMatchesMetricsTypeDef,
     ConnectionInputTypeDef,
     ConnectionTypeDef,
     CrawlerNodeDetailsTypeDef,
     ListCrawlsResponseTypeDef,
     GetCrawlerMetricsResponseTypeDef,
     CrawlerTargetsTypeDef,
     ListCrawlsRequestRequestTypeDef,
     CreateClassifierRequestRequestTypeDef,
-    CreateDataQualityRulesetRequestRequestTypeDef,
-    DataQualityRulesetFilterCriteriaTypeDef,
-    DataQualityRulesetListDetailsTypeDef,
-    GetDataQualityRulesetResponseTypeDef,
-    DataSourceTypeDef,
     CreatePartitionIndexRequestRequestTypeDef,
     CreateSchemaInputRequestTypeDef,
     DeleteRegistryInputRequestTypeDef,
     GetRegistryInputRequestTypeDef,
     ListSchemasInputRequestTypeDef,
     UpdateRegistryInputRequestTypeDef,
     CreateSessionRequestRequestTypeDef,
     SessionTypeDef,
-    EvaluateDataQualityTypeDef,
     DataCatalogEncryptionSettingsTypeDef,
     PrincipalPermissionsTypeDef,
     NullValueFieldTypeDef,
     DecimalColumnStatisticsDataTypeDef,
     DeleteSchemaInputRequestTypeDef,
     DeleteSchemaVersionsInputRequestTypeDef,
     GetSchemaByDefinitionInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
     ListSchemaVersionsInputRequestTypeDef,
     RegisterSchemaVersionInputRequestTypeDef,
     SchemaReferenceTypeDef,
     UpdateDevEndpointRequestRequestTypeDef,
-    S3DeltaDirectTargetTypeDef,
     S3DirectTargetTypeDef,
     S3GlueParquetTargetTypeDef,
-    S3HudiDirectTargetTypeDef,
-    DynamicTransformTypeDef,
     EncryptionConfigurationTypeDef,
     SchemaVersionErrorItemTypeDef,
     FilterExpressionTypeDef,
     TransformParametersTypeDef,
     GetClassifiersRequestGetClassifiersPaginateTypeDef,
     GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef,
     GetCrawlersRequestGetCrawlersPaginateTypeDef,
@@ -986,28 +946,14 @@
     CreateConnectionRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     GetConnectionResponseTypeDef,
     GetConnectionsResponseTypeDef,
     CrawlerTypeDef,
     CreateCrawlerRequestRequestTypeDef,
     UpdateCrawlerRequestRequestTypeDef,
-    ListDataQualityRulesetsRequestRequestTypeDef,
-    ListDataQualityRulesetsResponseTypeDef,
-    DataQualityResultDescriptionTypeDef,
-    DataQualityResultFilterCriteriaTypeDef,
-    DataQualityResultTypeDef,
-    DataQualityRuleRecommendationRunDescriptionTypeDef,
-    DataQualityRuleRecommendationRunFilterTypeDef,
-    DataQualityRulesetEvaluationRunDescriptionTypeDef,
-    DataQualityRulesetEvaluationRunFilterTypeDef,
-    GetDataQualityResultResponseTypeDef,
-    GetDataQualityRuleRecommendationRunResponseTypeDef,
-    GetDataQualityRulesetEvaluationRunResponseTypeDef,
-    StartDataQualityRuleRecommendationRunRequestRequestTypeDef,
-    StartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
     CreateSessionResponseTypeDef,
     GetSessionResponseTypeDef,
     ListSessionsResponseTypeDef,
     GetDataCatalogEncryptionSettingsResponseTypeDef,
     PutDataCatalogEncryptionSettingsRequestRequestTypeDef,
     DatabaseInputTypeDef,
     DatabaseTypeDef,
@@ -1018,24 +964,18 @@
     SecurityConfigurationTypeDef,
     DeleteSchemaVersionsResponseTypeDef,
     FilterTypeDef,
     UpdateMLTransformRequestRequestTypeDef,
     GetMLTransformsRequestRequestTypeDef,
     ListMLTransformsRequestRequestTypeDef,
     AthenaConnectorSourceTypeDef,
-    CatalogDeltaSourceTypeDef,
-    CatalogHudiSourceTypeDef,
     CustomCodeTypeDef,
     JDBCConnectorSourceTypeDef,
     JDBCConnectorTargetTypeDef,
-    S3CatalogDeltaSourceTypeDef,
-    S3CatalogHudiSourceTypeDef,
     S3CsvSourceTypeDef,
-    S3DeltaSourceTypeDef,
-    S3HudiSourceTypeDef,
     S3JsonSourceTypeDef,
     S3ParquetSourceTypeDef,
     SparkConnectorSourceTypeDef,
     SparkConnectorTargetTypeDef,
     SparkSQLTypeDef,
     GetJobRunResponseTypeDef,
     GetJobRunsResponseTypeDef,
@@ -1057,21 +997,14 @@
     UpdateTriggerResponseTypeDef,
     UpdateTriggerRequestRequestTypeDef,
     GetMLTransformResponseTypeDef,
     MLTransformTypeDef,
     BatchGetCrawlersResponseTypeDef,
     GetCrawlerResponseTypeDef,
     GetCrawlersResponseTypeDef,
-    ListDataQualityResultsResponseTypeDef,
-    ListDataQualityResultsRequestRequestTypeDef,
-    BatchGetDataQualityResultResponseTypeDef,
-    ListDataQualityRuleRecommendationRunsResponseTypeDef,
-    ListDataQualityRuleRecommendationRunsRequestRequestTypeDef,
-    ListDataQualityRulesetEvaluationRunsResponseTypeDef,
-    ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef,
     CreateDatabaseRequestRequestTypeDef,
     UpdateDatabaseRequestRequestTypeDef,
     GetDatabaseResponseTypeDef,
     GetDatabasesResponseTypeDef,
     ColumnStatisticsTypeDef,
     PartitionInputTypeDef,
     PartitionTypeDef,
```

### Comparing `mypy-boto3-glue-1.26.74/README.md` & `mypy-boto3-glue-1.26.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-glue?color=blue)](https://pypistats.org/packages/mypy-boto3-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glue 1.26.74](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[boto3.Glue 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-glue docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/).
 
 See how it helps to find and fix potential bugs:
 
@@ -331,20 +331,16 @@
     ConnectionPropertyKeyType,
     ConnectionTypeType,
     CrawlStateType,
     CrawlerHistoryStateType,
     CrawlerLineageSettingsType,
     CrawlerStateType,
     CsvHeaderOptionType,
-    DQStopJobOnFailureTimingType,
-    DQTransformOutputType,
     DataFormatType,
-    DataQualityRuleResultStatusType,
     DeleteBehaviorType,
-    DeltaTargetCompressionTypeType,
     EnableHybridValuesType,
     ExecutionClassType,
     ExistConditionType,
     FieldNameType,
     FilterLogicalOperatorType,
     FilterOperationType,
     FilterOperatorType,
@@ -362,31 +358,27 @@
     GetResourcePoliciesPaginatorName,
     GetSecurityConfigurationsPaginatorName,
     GetTableVersionsPaginatorName,
     GetTablesPaginatorName,
     GetTriggersPaginatorName,
     GetUserDefinedFunctionsPaginatorName,
     GlueRecordTypeType,
-    HudiTargetCompressionTypeType,
-    JDBCConnectionTypeType,
     JDBCDataTypeType,
-    JdbcMetadataEntryType,
     JobBookmarksEncryptionModeType,
     JobRunStateType,
     JoinTypeType,
     LanguageType,
     LastCrawlStatusType,
     ListRegistriesPaginatorName,
     ListSchemaVersionsPaginatorName,
     ListSchemasPaginatorName,
     LogicalOperatorType,
     LogicalType,
     MLUserDataEncryptionModeStringType,
     NodeTypeType,
-    ParamTypeType,
     ParquetCompressionTypeType,
     PartitionIndexStatusType,
     PermissionType,
     PermissionTypeType,
     PiiTypeType,
     PrincipalTypeType,
     QuoteCharType,
@@ -453,29 +445,26 @@
     ErrorDetailTypeDef,
     BatchDeleteTableRequestRequestTypeDef,
     BatchDeleteTableVersionRequestRequestTypeDef,
     BatchGetBlueprintsRequestRequestTypeDef,
     BatchGetCrawlersRequestRequestTypeDef,
     BatchGetCustomEntityTypesRequestRequestTypeDef,
     CustomEntityTypeTypeDef,
-    BatchGetDataQualityResultRequestRequestTypeDef,
     BatchGetDevEndpointsRequestRequestTypeDef,
     DevEndpointTypeDef,
     BatchGetJobsRequestRequestTypeDef,
     BatchGetTriggersRequestRequestTypeDef,
     BatchGetWorkflowsRequestRequestTypeDef,
     BatchStopJobRunRequestRequestTypeDef,
     BatchStopJobRunSuccessfulSubmissionTypeDef,
     BinaryColumnStatisticsDataTypeDef,
     BlueprintDetailsTypeDef,
     BlueprintRunTypeDef,
     LastActiveDefinitionTypeDef,
     BooleanColumnStatisticsDataTypeDef,
-    CancelDataQualityRuleRecommendationRunRequestRequestTypeDef,
-    CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef,
     CancelMLTaskRunRequestRequestTypeDef,
     CancelStatementRequestRequestTypeDef,
     CatalogEntryTypeDef,
     CatalogImportStatusTypeDef,
     KafkaStreamingSourceOptionsTypeDef,
     StreamingDataPreviewOptionsTypeDef,
     KinesisStreamingSourceOptionsTypeDef,
@@ -484,15 +473,14 @@
     CatalogTargetTypeDef,
     CheckSchemaVersionValidityInputRequestTypeDef,
     CsvClassifierTypeDef,
     GrokClassifierTypeDef,
     JsonClassifierTypeDef,
     XMLClassifierTypeDef,
     CloudWatchEncryptionTypeDef,
-    DirectJDBCSourceTypeDef,
     DropDuplicatesTypeDef,
     DropFieldsTypeDef,
     DynamoDBCatalogSourceTypeDef,
     FillMissingValuesTypeDef,
     MergeTypeDef,
     MicrosoftSQLServerCatalogSourceTypeDef,
     MicrosoftSQLServerCatalogTargetTypeDef,
@@ -542,43 +530,37 @@
     CrawlsFilterTypeDef,
     CreateBlueprintRequestRequestTypeDef,
     CreateCsvClassifierRequestTypeDef,
     CreateGrokClassifierRequestTypeDef,
     CreateJsonClassifierRequestTypeDef,
     CreateXMLClassifierRequestTypeDef,
     CreateCustomEntityTypeRequestRequestTypeDef,
-    DataQualityTargetTableTypeDef,
     CreateDevEndpointRequestRequestTypeDef,
     ExecutionPropertyTypeDef,
     JobCommandTypeDef,
     SourceControlDetailsTypeDef,
     GlueTableTypeDef,
     PartitionIndexTypeDef,
     CreateRegistryInputRequestTypeDef,
     RegistryIdTypeDef,
     SessionCommandTypeDef,
     EventBatchingConditionTypeDef,
     CreateWorkflowRequestRequestTypeDef,
-    DQResultsPublishingOptionsTypeDef,
-    DQStopJobOnFailureOptionsTypeDef,
     EncryptionAtRestTypeDef,
     DataLakePrincipalTypeDef,
-    DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
-    DataQualityRuleResultTypeDef,
     DatabaseIdentifierTypeDef,
     DatatypeTypeDef,
     DecimalNumberTypeDef,
     DeleteBlueprintRequestRequestTypeDef,
     DeleteClassifierRequestRequestTypeDef,
     DeleteColumnStatisticsForPartitionRequestRequestTypeDef,
     DeleteColumnStatisticsForTableRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteCrawlerRequestRequestTypeDef,
     DeleteCustomEntityTypeRequestRequestTypeDef,
-    DeleteDataQualityRulesetRequestRequestTypeDef,
     DeleteDatabaseRequestRequestTypeDef,
     DeleteDevEndpointRequestRequestTypeDef,
     DeleteJobRequestRequestTypeDef,
     DeleteMLTransformRequestRequestTypeDef,
     DeletePartitionIndexRequestRequestTypeDef,
     DeletePartitionRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
@@ -589,15 +571,14 @@
     DeleteTableVersionRequestRequestTypeDef,
     DeleteTriggerRequestRequestTypeDef,
     DeleteUserDefinedFunctionRequestRequestTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     DevEndpointCustomLibrariesTypeDef,
     DirectSchemaChangePolicyTypeDef,
     NullCheckBoxListTypeDef,
-    TransformConfigParameterTypeDef,
     EdgeTypeDef,
     JobBookmarksEncryptionTypeDef,
     S3EncryptionTypeDef,
     ErrorDetailsTypeDef,
     ExportLabelsTaskRunPropertiesTypeDef,
     FilterValueTypeDef,
     FindMatchesParametersTypeDef,
@@ -614,18 +595,14 @@
     GetConnectionRequestRequestTypeDef,
     GetConnectionsFilterTypeDef,
     GetCrawlerMetricsRequestRequestTypeDef,
     GetCrawlerRequestRequestTypeDef,
     GetCrawlersRequestRequestTypeDef,
     GetCustomEntityTypeRequestRequestTypeDef,
     GetDataCatalogEncryptionSettingsRequestRequestTypeDef,
-    GetDataQualityResultRequestRequestTypeDef,
-    GetDataQualityRuleRecommendationRunRequestRequestTypeDef,
-    GetDataQualityRulesetEvaluationRunRequestRequestTypeDef,
-    GetDataQualityRulesetRequestRequestTypeDef,
     GetDatabaseRequestRequestTypeDef,
     GetDatabasesRequestRequestTypeDef,
     GetDataflowGraphRequestRequestTypeDef,
     GetDevEndpointRequestRequestTypeDef,
     GetDevEndpointsRequestRequestTypeDef,
     GetJobBookmarkRequestRequestTypeDef,
     JobBookmarkEntryTypeDef,
@@ -725,15 +702,14 @@
     UntagResourceRequestRequestTypeDef,
     UpdateBlueprintRequestRequestTypeDef,
     UpdateCsvClassifierRequestTypeDef,
     UpdateGrokClassifierRequestTypeDef,
     UpdateJsonClassifierRequestTypeDef,
     UpdateXMLClassifierRequestTypeDef,
     UpdateCrawlerScheduleRequestRequestTypeDef,
-    UpdateDataQualityRulesetRequestRequestTypeDef,
     UpdateJobFromSourceControlRequestRequestTypeDef,
     UpdateSourceControlFromJobRequestRequestTypeDef,
     UpdateWorkflowRequestRequestTypeDef,
     WorkflowRunStatisticsTypeDef,
     ActionTypeDef,
     StartJobRunRequestRequestTypeDef,
     AggregateTypeDef,
@@ -742,15 +718,14 @@
     BackfillErrorTypeDef,
     BatchDeletePartitionRequestRequestTypeDef,
     BatchGetPartitionRequestRequestTypeDef,
     CancelMLTaskRunResponseTypeDef,
     CheckSchemaVersionValidityResponseTypeDef,
     CreateBlueprintResponseTypeDef,
     CreateCustomEntityTypeResponseTypeDef,
-    CreateDataQualityRulesetResponseTypeDef,
     CreateDevEndpointResponseTypeDef,
     CreateJobResponseTypeDef,
     CreateMLTransformResponseTypeDef,
     CreateRegistryResponseTypeDef,
     CreateSchemaResponseTypeDef,
     CreateScriptResponseTypeDef,
     CreateSecurityConfigurationResponseTypeDef,
@@ -785,27 +760,24 @@
     PutResourcePolicyResponseTypeDef,
     PutSchemaVersionMetadataResponseTypeDef,
     RegisterSchemaVersionResponseTypeDef,
     RemoveSchemaVersionMetadataResponseTypeDef,
     ResumeWorkflowRunResponseTypeDef,
     RunStatementResponseTypeDef,
     StartBlueprintRunResponseTypeDef,
-    StartDataQualityRuleRecommendationRunResponseTypeDef,
-    StartDataQualityRulesetEvaluationRunResponseTypeDef,
     StartExportLabelsTaskRunResponseTypeDef,
     StartImportLabelsTaskRunResponseTypeDef,
     StartJobRunResponseTypeDef,
     StartMLEvaluationTaskRunResponseTypeDef,
     StartMLLabelingSetGenerationTaskRunResponseTypeDef,
     StartTriggerResponseTypeDef,
     StartWorkflowRunResponseTypeDef,
     StopSessionResponseTypeDef,
     StopTriggerResponseTypeDef,
     UpdateBlueprintResponseTypeDef,
-    UpdateDataQualityRulesetResponseTypeDef,
     UpdateJobFromSourceControlResponseTypeDef,
     UpdateJobResponseTypeDef,
     UpdateMLTransformResponseTypeDef,
     UpdateRegistryResponseTypeDef,
     UpdateSchemaResponseTypeDef,
     UpdateSourceControlFromJobResponseTypeDef,
     UpdateWorkflowResponseTypeDef,
@@ -827,60 +799,49 @@
     GetCatalogImportStatusResponseTypeDef,
     CatalogKafkaSourceTypeDef,
     DirectKafkaSourceTypeDef,
     CatalogKinesisSourceTypeDef,
     DirectKinesisSourceTypeDef,
     GovernedCatalogTargetTypeDef,
     S3CatalogTargetTypeDef,
-    S3DeltaCatalogTargetTypeDef,
-    S3HudiCatalogTargetTypeDef,
     ClassifierTypeDef,
     CodeGenNodeTypeDef,
     LocationTypeDef,
     PredicateTypeDef,
     FindMatchesMetricsTypeDef,
     ConnectionInputTypeDef,
     ConnectionTypeDef,
     CrawlerNodeDetailsTypeDef,
     ListCrawlsResponseTypeDef,
     GetCrawlerMetricsResponseTypeDef,
     CrawlerTargetsTypeDef,
     ListCrawlsRequestRequestTypeDef,
     CreateClassifierRequestRequestTypeDef,
-    CreateDataQualityRulesetRequestRequestTypeDef,
-    DataQualityRulesetFilterCriteriaTypeDef,
-    DataQualityRulesetListDetailsTypeDef,
-    GetDataQualityRulesetResponseTypeDef,
-    DataSourceTypeDef,
     CreatePartitionIndexRequestRequestTypeDef,
     CreateSchemaInputRequestTypeDef,
     DeleteRegistryInputRequestTypeDef,
     GetRegistryInputRequestTypeDef,
     ListSchemasInputRequestTypeDef,
     UpdateRegistryInputRequestTypeDef,
     CreateSessionRequestRequestTypeDef,
     SessionTypeDef,
-    EvaluateDataQualityTypeDef,
     DataCatalogEncryptionSettingsTypeDef,
     PrincipalPermissionsTypeDef,
     NullValueFieldTypeDef,
     DecimalColumnStatisticsDataTypeDef,
     DeleteSchemaInputRequestTypeDef,
     DeleteSchemaVersionsInputRequestTypeDef,
     GetSchemaByDefinitionInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
     ListSchemaVersionsInputRequestTypeDef,
     RegisterSchemaVersionInputRequestTypeDef,
     SchemaReferenceTypeDef,
     UpdateDevEndpointRequestRequestTypeDef,
-    S3DeltaDirectTargetTypeDef,
     S3DirectTargetTypeDef,
     S3GlueParquetTargetTypeDef,
-    S3HudiDirectTargetTypeDef,
-    DynamicTransformTypeDef,
     EncryptionConfigurationTypeDef,
     SchemaVersionErrorItemTypeDef,
     FilterExpressionTypeDef,
     TransformParametersTypeDef,
     GetClassifiersRequestGetClassifiersPaginateTypeDef,
     GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef,
     GetCrawlersRequestGetCrawlersPaginateTypeDef,
@@ -954,28 +915,14 @@
     CreateConnectionRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     GetConnectionResponseTypeDef,
     GetConnectionsResponseTypeDef,
     CrawlerTypeDef,
     CreateCrawlerRequestRequestTypeDef,
     UpdateCrawlerRequestRequestTypeDef,
-    ListDataQualityRulesetsRequestRequestTypeDef,
-    ListDataQualityRulesetsResponseTypeDef,
-    DataQualityResultDescriptionTypeDef,
-    DataQualityResultFilterCriteriaTypeDef,
-    DataQualityResultTypeDef,
-    DataQualityRuleRecommendationRunDescriptionTypeDef,
-    DataQualityRuleRecommendationRunFilterTypeDef,
-    DataQualityRulesetEvaluationRunDescriptionTypeDef,
-    DataQualityRulesetEvaluationRunFilterTypeDef,
-    GetDataQualityResultResponseTypeDef,
-    GetDataQualityRuleRecommendationRunResponseTypeDef,
-    GetDataQualityRulesetEvaluationRunResponseTypeDef,
-    StartDataQualityRuleRecommendationRunRequestRequestTypeDef,
-    StartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
     CreateSessionResponseTypeDef,
     GetSessionResponseTypeDef,
     ListSessionsResponseTypeDef,
     GetDataCatalogEncryptionSettingsResponseTypeDef,
     PutDataCatalogEncryptionSettingsRequestRequestTypeDef,
     DatabaseInputTypeDef,
     DatabaseTypeDef,
@@ -986,24 +933,18 @@
     SecurityConfigurationTypeDef,
     DeleteSchemaVersionsResponseTypeDef,
     FilterTypeDef,
     UpdateMLTransformRequestRequestTypeDef,
     GetMLTransformsRequestRequestTypeDef,
     ListMLTransformsRequestRequestTypeDef,
     AthenaConnectorSourceTypeDef,
-    CatalogDeltaSourceTypeDef,
-    CatalogHudiSourceTypeDef,
     CustomCodeTypeDef,
     JDBCConnectorSourceTypeDef,
     JDBCConnectorTargetTypeDef,
-    S3CatalogDeltaSourceTypeDef,
-    S3CatalogHudiSourceTypeDef,
     S3CsvSourceTypeDef,
-    S3DeltaSourceTypeDef,
-    S3HudiSourceTypeDef,
     S3JsonSourceTypeDef,
     S3ParquetSourceTypeDef,
     SparkConnectorSourceTypeDef,
     SparkConnectorTargetTypeDef,
     SparkSQLTypeDef,
     GetJobRunResponseTypeDef,
     GetJobRunsResponseTypeDef,
@@ -1025,21 +966,14 @@
     UpdateTriggerResponseTypeDef,
     UpdateTriggerRequestRequestTypeDef,
     GetMLTransformResponseTypeDef,
     MLTransformTypeDef,
     BatchGetCrawlersResponseTypeDef,
     GetCrawlerResponseTypeDef,
     GetCrawlersResponseTypeDef,
-    ListDataQualityResultsResponseTypeDef,
-    ListDataQualityResultsRequestRequestTypeDef,
-    BatchGetDataQualityResultResponseTypeDef,
-    ListDataQualityRuleRecommendationRunsResponseTypeDef,
-    ListDataQualityRuleRecommendationRunsRequestRequestTypeDef,
-    ListDataQualityRulesetEvaluationRunsResponseTypeDef,
-    ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef,
     CreateDatabaseRequestRequestTypeDef,
     UpdateDatabaseRequestRequestTypeDef,
     GetDatabaseResponseTypeDef,
     GetDatabasesResponseTypeDef,
     ColumnStatisticsTypeDef,
     PartitionInputTypeDef,
     PartitionTypeDef,
```

### Comparing `mypy-boto3-glue-1.26.74/mypy_boto3_glue/__init__.py` & `mypy-boto3-glue-1.26.8/mypy_boto3_glue/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.26.74/mypy_boto3_glue/__init__.pyi` & `mypy-boto3-glue-1.26.8/mypy_boto3_glue/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.26.74/mypy_boto3_glue/__main__.py` & `mypy-boto3-glue-1.26.8/mypy_boto3_glue/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Glue 1.26.74\nVersion:         1.26.74\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.Glue 1.26.8\nVersion:         1.26.8\nBuilder version:"
+        " 7.11.10\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.74")
+    print("1.26.8")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-glue-1.26.74/mypy_boto3_glue/client.py` & `mypy-boto3-glue-1.26.8/mypy_boto3_glue/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,14 @@
     BatchDeleteConnectionResponseTypeDef,
     BatchDeletePartitionResponseTypeDef,
     BatchDeleteTableResponseTypeDef,
     BatchDeleteTableVersionResponseTypeDef,
     BatchGetBlueprintsResponseTypeDef,
     BatchGetCrawlersResponseTypeDef,
     BatchGetCustomEntityTypesResponseTypeDef,
-    BatchGetDataQualityResultResponseTypeDef,
     BatchGetDevEndpointsResponseTypeDef,
     BatchGetJobsResponseTypeDef,
     BatchGetPartitionResponseTypeDef,
     BatchGetTriggersResponseTypeDef,
     BatchGetWorkflowsResponseTypeDef,
     BatchStopJobRunResponseTypeDef,
     BatchUpdatePartitionRequestEntryTypeDef,
@@ -84,15 +83,14 @@
     ConnectionInputTypeDef,
     ConnectionsListTypeDef,
     CrawlerTargetsTypeDef,
     CrawlsFilterTypeDef,
     CreateBlueprintResponseTypeDef,
     CreateCsvClassifierRequestTypeDef,
     CreateCustomEntityTypeResponseTypeDef,
-    CreateDataQualityRulesetResponseTypeDef,
     CreateDevEndpointResponseTypeDef,
     CreateGrokClassifierRequestTypeDef,
     CreateJobResponseTypeDef,
     CreateJsonClassifierRequestTypeDef,
     CreateMLTransformResponseTypeDef,
     CreateRegistryResponseTypeDef,
     CreateSchemaResponseTypeDef,
@@ -100,21 +98,14 @@
     CreateSecurityConfigurationResponseTypeDef,
     CreateSessionResponseTypeDef,
     CreateTriggerResponseTypeDef,
     CreateWorkflowResponseTypeDef,
     CreateXMLClassifierRequestTypeDef,
     DatabaseInputTypeDef,
     DataCatalogEncryptionSettingsTypeDef,
-    DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
-    DataQualityResultFilterCriteriaTypeDef,
-    DataQualityRuleRecommendationRunFilterTypeDef,
-    DataQualityRulesetEvaluationRunFilterTypeDef,
-    DataQualityRulesetFilterCriteriaTypeDef,
-    DataQualityTargetTableTypeDef,
-    DataSourceTypeDef,
     DeleteBlueprintResponseTypeDef,
     DeleteCustomEntityTypeResponseTypeDef,
     DeleteJobResponseTypeDef,
     DeleteMLTransformResponseTypeDef,
     DeleteRegistryResponseTypeDef,
     DeleteSchemaResponseTypeDef,
     DeleteSchemaVersionsResponseTypeDef,
@@ -140,18 +131,14 @@
     GetCrawlerResponseTypeDef,
     GetCrawlersResponseTypeDef,
     GetCustomEntityTypeResponseTypeDef,
     GetDatabaseResponseTypeDef,
     GetDatabasesResponseTypeDef,
     GetDataCatalogEncryptionSettingsResponseTypeDef,
     GetDataflowGraphResponseTypeDef,
-    GetDataQualityResultResponseTypeDef,
-    GetDataQualityRuleRecommendationRunResponseTypeDef,
-    GetDataQualityRulesetEvaluationRunResponseTypeDef,
-    GetDataQualityRulesetResponseTypeDef,
     GetDevEndpointResponseTypeDef,
     GetDevEndpointsResponseTypeDef,
     GetJobBookmarkResponseTypeDef,
     GetJobResponseTypeDef,
     GetJobRunResponseTypeDef,
     GetJobRunsResponseTypeDef,
     GetJobsResponseTypeDef,
@@ -196,18 +183,14 @@
     JobUpdateTypeDef,
     LakeFormationConfigurationTypeDef,
     LineageConfigurationTypeDef,
     ListBlueprintsResponseTypeDef,
     ListCrawlersResponseTypeDef,
     ListCrawlsResponseTypeDef,
     ListCustomEntityTypesResponseTypeDef,
-    ListDataQualityResultsResponseTypeDef,
-    ListDataQualityRuleRecommendationRunsResponseTypeDef,
-    ListDataQualityRulesetEvaluationRunsResponseTypeDef,
-    ListDataQualityRulesetsResponseTypeDef,
     ListDevEndpointsResponseTypeDef,
     ListJobsResponseTypeDef,
     ListMLTransformsResponseTypeDef,
     ListRegistriesResponseTypeDef,
     ListSchemasResponseTypeDef,
     ListSchemaVersionsResponseTypeDef,
     ListSessionsResponseTypeDef,
@@ -238,16 +221,14 @@
     SchemaVersionNumberTypeDef,
     SearchTablesResponseTypeDef,
     SegmentTypeDef,
     SessionCommandTypeDef,
     SortCriterionTypeDef,
     SourceControlDetailsTypeDef,
     StartBlueprintRunResponseTypeDef,
-    StartDataQualityRuleRecommendationRunResponseTypeDef,
-    StartDataQualityRulesetEvaluationRunResponseTypeDef,
     StartExportLabelsTaskRunResponseTypeDef,
     StartImportLabelsTaskRunResponseTypeDef,
     StartJobRunResponseTypeDef,
     StartMLEvaluationTaskRunResponseTypeDef,
     StartMLLabelingSetGenerationTaskRunResponseTypeDef,
     StartTriggerResponseTypeDef,
     StartWorkflowRunResponseTypeDef,
@@ -261,15 +242,14 @@
     TransformParametersTypeDef,
     TransformSortCriteriaTypeDef,
     TriggerUpdateTypeDef,
     UpdateBlueprintResponseTypeDef,
     UpdateColumnStatisticsForPartitionResponseTypeDef,
     UpdateColumnStatisticsForTableResponseTypeDef,
     UpdateCsvClassifierRequestTypeDef,
-    UpdateDataQualityRulesetResponseTypeDef,
     UpdateGrokClassifierRequestTypeDef,
     UpdateJobFromSourceControlResponseTypeDef,
     UpdateJobResponseTypeDef,
     UpdateJsonClassifierRequestTypeDef,
     UpdateMLTransformResponseTypeDef,
     UpdateRegistryResponseTypeDef,
     UpdateSchemaResponseTypeDef,
@@ -440,24 +420,14 @@
         """
         Retrieves the details for the custom patterns specified by a list of names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_get_custom_entity_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#batch_get_custom_entity_types)
         """
 
-    def batch_get_data_quality_result(
-        self, *, ResultIds: Sequence[str]
-    ) -> BatchGetDataQualityResultResponseTypeDef:
-        """
-        Retrieves a list of data quality results for the specified result IDs.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_get_data_quality_result)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#batch_get_data_quality_result)
-        """
-
     def batch_get_dev_endpoints(
         self, *, DevEndpointNames: Sequence[str]
     ) -> BatchGetDevEndpointsResponseTypeDef:
         """
         Returns a list of resource metadata for a given list of development endpoint
         names.
 
@@ -535,30 +505,14 @@
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#can_paginate)
         """
 
-    def cancel_data_quality_rule_recommendation_run(self, *, RunId: str) -> Dict[str, Any]:
-        """
-        Cancels the specified recommendation run that was being used to generate rules.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.cancel_data_quality_rule_recommendation_run)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#cancel_data_quality_rule_recommendation_run)
-        """
-
-    def cancel_data_quality_ruleset_evaluation_run(self, *, RunId: str) -> Dict[str, Any]:
-        """
-        Cancels a run where a ruleset is being evaluated against a data source.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.cancel_data_quality_ruleset_evaluation_run)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#cancel_data_quality_ruleset_evaluation_run)
-        """
-
     def cancel_ml_task_run(
         self, *, TransformId: str, TaskRunId: str
     ) -> CancelMLTaskRunResponseTypeDef:
         """
         Cancels (stops) a task run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.cancel_ml_task_run)
@@ -671,32 +625,14 @@
         Creates a custom pattern that is used to detect sensitive data across the
         columns and rows of your structured data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_custom_entity_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#create_custom_entity_type)
         """
 
-    def create_data_quality_ruleset(
-        self,
-        *,
-        Name: str,
-        Ruleset: str,
-        Description: str = ...,
-        Tags: Mapping[str, str] = ...,
-        TargetTable: DataQualityTargetTableTypeDef = ...,
-        ClientToken: str = ...
-    ) -> CreateDataQualityRulesetResponseTypeDef:
-        """
-        Creates a data quality ruleset with DQDL rules applied to a specified Glue
-        table.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_data_quality_ruleset)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#create_data_quality_ruleset)
-        """
-
     def create_database(
         self,
         *,
         DatabaseInput: DatabaseInputTypeDef,
         CatalogId: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> Dict[str, Any]:
@@ -1028,22 +964,14 @@
         """
         Deletes a custom pattern by specifying its name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.delete_custom_entity_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#delete_custom_entity_type)
         """
 
-    def delete_data_quality_ruleset(self, *, Name: str) -> Dict[str, Any]:
-        """
-        Deletes a data quality ruleset.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.delete_data_quality_ruleset)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#delete_data_quality_ruleset)
-        """
-
     def delete_database(self, *, Name: str, CatalogId: str = ...) -> Dict[str, Any]:
         """
         Removes a specified database from a Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.delete_database)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#delete_database)
         """
@@ -1361,50 +1289,14 @@
         """
         Retrieves the security configuration for a specified catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_data_catalog_encryption_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_data_catalog_encryption_settings)
         """
 
-    def get_data_quality_result(self, *, ResultId: str) -> GetDataQualityResultResponseTypeDef:
-        """
-        Retrieves the result of a data quality rule evaluation.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_data_quality_result)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_data_quality_result)
-        """
-
-    def get_data_quality_rule_recommendation_run(
-        self, *, RunId: str
-    ) -> GetDataQualityRuleRecommendationRunResponseTypeDef:
-        """
-        Gets the specified recommendation run that was used to generate rules.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_data_quality_rule_recommendation_run)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_data_quality_rule_recommendation_run)
-        """
-
-    def get_data_quality_ruleset(self, *, Name: str) -> GetDataQualityRulesetResponseTypeDef:
-        """
-        Returns an existing ruleset by identifier or name.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_data_quality_ruleset)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_data_quality_ruleset)
-        """
-
-    def get_data_quality_ruleset_evaluation_run(
-        self, *, RunId: str
-    ) -> GetDataQualityRulesetEvaluationRunResponseTypeDef:
-        """
-        Retrieves a specific run where a ruleset is evaluated against a data source.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_data_quality_ruleset_evaluation_run)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_data_quality_ruleset_evaluation_run)
-        """
-
     def get_database(self, *, Name: str, CatalogId: str = ...) -> GetDatabaseResponseTypeDef:
         """
         Retrieves the definition of a specified database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_database)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_database)
         """
@@ -1825,16 +1717,16 @@
         DatabaseName: str,
         TableName: str,
         PartitionValues: Sequence[str],
         SupportedPermissionTypes: Sequence[PermissionTypeType],
         AuditContext: AuditContextTypeDef = ...
     ) -> GetUnfilteredPartitionMetadataResponseTypeDef:
         """
-        Retrieves partition metadata from the Data Catalog that contains unfiltered
-        metadata.
+        See also: [AWS API
+        Documentation](https://docs.aws.amazon.com/goto/WebAPI/glue-2017-03-31/GetUnfilteredPartitionMetadata).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_unfiltered_partition_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_unfiltered_partition_metadata)
         """
 
     def get_unfiltered_partitions_metadata(
         self,
@@ -1846,16 +1738,16 @@
         Expression: str = ...,
         AuditContext: AuditContextTypeDef = ...,
         NextToken: str = ...,
         Segment: SegmentTypeDef = ...,
         MaxResults: int = ...
     ) -> GetUnfilteredPartitionsMetadataResponseTypeDef:
         """
-        Retrieves partition metadata from the Data Catalog that contains unfiltered
-        metadata.
+        See also: [AWS API
+        Documentation](https://docs.aws.amazon.com/goto/WebAPI/glue-2017-03-31/GetUnfilteredPartitionsMetadata).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_unfiltered_partitions_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_unfiltered_partitions_metadata)
         """
 
     def get_unfiltered_table_metadata(
         self,
@@ -1863,16 +1755,16 @@
         CatalogId: str,
         DatabaseName: str,
         Name: str,
         SupportedPermissionTypes: Sequence[PermissionTypeType],
         AuditContext: AuditContextTypeDef = ...
     ) -> GetUnfilteredTableMetadataResponseTypeDef:
         """
-        Retrieves table metadata from the Data Catalog that contains unfiltered
-        metadata.
+        See also: [AWS API
+        Documentation](https://docs.aws.amazon.com/goto/WebAPI/glue-2017-03-31/GetUnfilteredTableMetadata).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_unfiltered_table_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_unfiltered_table_metadata)
         """
 
     def get_user_defined_function(
         self, *, DatabaseName: str, FunctionName: str, CatalogId: str = ...
@@ -1988,72 +1880,14 @@
         """
         Lists all the custom patterns that have been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_custom_entity_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#list_custom_entity_types)
         """
 
-    def list_data_quality_results(
-        self,
-        *,
-        Filter: DataQualityResultFilterCriteriaTypeDef = ...,
-        NextToken: str = ...,
-        MaxResults: int = ...
-    ) -> ListDataQualityResultsResponseTypeDef:
-        """
-        Returns all data quality execution results for your account.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_results)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#list_data_quality_results)
-        """
-
-    def list_data_quality_rule_recommendation_runs(
-        self,
-        *,
-        Filter: DataQualityRuleRecommendationRunFilterTypeDef = ...,
-        NextToken: str = ...,
-        MaxResults: int = ...
-    ) -> ListDataQualityRuleRecommendationRunsResponseTypeDef:
-        """
-        Lists the recommendation runs meeting the filter criteria.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_rule_recommendation_runs)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#list_data_quality_rule_recommendation_runs)
-        """
-
-    def list_data_quality_ruleset_evaluation_runs(
-        self,
-        *,
-        Filter: DataQualityRulesetEvaluationRunFilterTypeDef = ...,
-        NextToken: str = ...,
-        MaxResults: int = ...
-    ) -> ListDataQualityRulesetEvaluationRunsResponseTypeDef:
-        """
-        Lists all the runs meeting the filter criteria, where a ruleset is evaluated
-        against a data source.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_ruleset_evaluation_runs)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#list_data_quality_ruleset_evaluation_runs)
-        """
-
-    def list_data_quality_rulesets(
-        self,
-        *,
-        NextToken: str = ...,
-        MaxResults: int = ...,
-        Filter: DataQualityRulesetFilterCriteriaTypeDef = ...,
-        Tags: Mapping[str, str] = ...
-    ) -> ListDataQualityRulesetsResponseTypeDef:
-        """
-        Returns a paginated list of rulesets for the specified list of Glue tables.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_rulesets)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#list_data_quality_rulesets)
-        """
-
     def list_dev_endpoints(
         self, *, NextToken: str = ..., MaxResults: int = ..., Tags: Mapping[str, str] = ...
     ) -> ListDevEndpointsResponseTypeDef:
         """
         Retrieves the names of all `DevEndpoint` resources in this Amazon Web Services
         account, or the resources with the specified tag.
 
@@ -2343,51 +2177,14 @@
         Changes the schedule state of the specified crawler to `SCHEDULED` , unless the
         crawler is already running or the schedule state is already `SCHEDULED` .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_crawler_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#start_crawler_schedule)
         """
 
-    def start_data_quality_rule_recommendation_run(
-        self,
-        *,
-        DataSource: DataSourceTypeDef,
-        Role: str,
-        NumberOfWorkers: int = ...,
-        Timeout: int = ...,
-        CreatedRulesetName: str = ...,
-        ClientToken: str = ...
-    ) -> StartDataQualityRuleRecommendationRunResponseTypeDef:
-        """
-        Starts a recommendation run that is used to generate rules when you don't know
-        what rules to write.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_data_quality_rule_recommendation_run)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#start_data_quality_rule_recommendation_run)
-        """
-
-    def start_data_quality_ruleset_evaluation_run(
-        self,
-        *,
-        DataSource: DataSourceTypeDef,
-        Role: str,
-        RulesetNames: Sequence[str],
-        NumberOfWorkers: int = ...,
-        Timeout: int = ...,
-        ClientToken: str = ...,
-        AdditionalRunOptions: DataQualityEvaluationRunAdditionalRunOptionsTypeDef = ...
-    ) -> StartDataQualityRulesetEvaluationRunResponseTypeDef:
-        """
-        Once you have a ruleset definition (either recommended or your own), you call
-        this operation to evaluate the ruleset against a data source (Glue table).
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_data_quality_ruleset_evaluation_run)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#start_data_quality_ruleset_evaluation_run)
-        """
-
     def start_export_labels_task_run(
         self, *, TransformId: str, OutputS3Path: str
     ) -> StartExportLabelsTaskRunResponseTypeDef:
         """
         Begins an asynchronous task to export all labeled data for a particular
         transform.
 
@@ -2620,24 +2417,14 @@
         """
         Updates the schedule of a crawler using a `cron` expression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_crawler_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#update_crawler_schedule)
         """
 
-    def update_data_quality_ruleset(
-        self, *, Name: str, UpdatedName: str = ..., Description: str = ..., Ruleset: str = ...
-    ) -> UpdateDataQualityRulesetResponseTypeDef:
-        """
-        Updates the specified data quality ruleset.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_data_quality_ruleset)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#update_data_quality_ruleset)
-        """
-
     def update_database(
         self, *, Name: str, DatabaseInput: DatabaseInputTypeDef, CatalogId: str = ...
     ) -> Dict[str, Any]:
         """
         Updates an existing database definition in a Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_database)
```

### Comparing `mypy-boto3-glue-1.26.74/mypy_boto3_glue/client.pyi` & `mypy-boto3-glue-1.26.8/mypy_boto3_glue/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,14 @@
     BatchDeleteConnectionResponseTypeDef,
     BatchDeletePartitionResponseTypeDef,
     BatchDeleteTableResponseTypeDef,
     BatchDeleteTableVersionResponseTypeDef,
     BatchGetBlueprintsResponseTypeDef,
     BatchGetCrawlersResponseTypeDef,
     BatchGetCustomEntityTypesResponseTypeDef,
-    BatchGetDataQualityResultResponseTypeDef,
     BatchGetDevEndpointsResponseTypeDef,
     BatchGetJobsResponseTypeDef,
     BatchGetPartitionResponseTypeDef,
     BatchGetTriggersResponseTypeDef,
     BatchGetWorkflowsResponseTypeDef,
     BatchStopJobRunResponseTypeDef,
     BatchUpdatePartitionRequestEntryTypeDef,
@@ -84,15 +83,14 @@
     ConnectionInputTypeDef,
     ConnectionsListTypeDef,
     CrawlerTargetsTypeDef,
     CrawlsFilterTypeDef,
     CreateBlueprintResponseTypeDef,
     CreateCsvClassifierRequestTypeDef,
     CreateCustomEntityTypeResponseTypeDef,
-    CreateDataQualityRulesetResponseTypeDef,
     CreateDevEndpointResponseTypeDef,
     CreateGrokClassifierRequestTypeDef,
     CreateJobResponseTypeDef,
     CreateJsonClassifierRequestTypeDef,
     CreateMLTransformResponseTypeDef,
     CreateRegistryResponseTypeDef,
     CreateSchemaResponseTypeDef,
@@ -100,21 +98,14 @@
     CreateSecurityConfigurationResponseTypeDef,
     CreateSessionResponseTypeDef,
     CreateTriggerResponseTypeDef,
     CreateWorkflowResponseTypeDef,
     CreateXMLClassifierRequestTypeDef,
     DatabaseInputTypeDef,
     DataCatalogEncryptionSettingsTypeDef,
-    DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
-    DataQualityResultFilterCriteriaTypeDef,
-    DataQualityRuleRecommendationRunFilterTypeDef,
-    DataQualityRulesetEvaluationRunFilterTypeDef,
-    DataQualityRulesetFilterCriteriaTypeDef,
-    DataQualityTargetTableTypeDef,
-    DataSourceTypeDef,
     DeleteBlueprintResponseTypeDef,
     DeleteCustomEntityTypeResponseTypeDef,
     DeleteJobResponseTypeDef,
     DeleteMLTransformResponseTypeDef,
     DeleteRegistryResponseTypeDef,
     DeleteSchemaResponseTypeDef,
     DeleteSchemaVersionsResponseTypeDef,
@@ -140,18 +131,14 @@
     GetCrawlerResponseTypeDef,
     GetCrawlersResponseTypeDef,
     GetCustomEntityTypeResponseTypeDef,
     GetDatabaseResponseTypeDef,
     GetDatabasesResponseTypeDef,
     GetDataCatalogEncryptionSettingsResponseTypeDef,
     GetDataflowGraphResponseTypeDef,
-    GetDataQualityResultResponseTypeDef,
-    GetDataQualityRuleRecommendationRunResponseTypeDef,
-    GetDataQualityRulesetEvaluationRunResponseTypeDef,
-    GetDataQualityRulesetResponseTypeDef,
     GetDevEndpointResponseTypeDef,
     GetDevEndpointsResponseTypeDef,
     GetJobBookmarkResponseTypeDef,
     GetJobResponseTypeDef,
     GetJobRunResponseTypeDef,
     GetJobRunsResponseTypeDef,
     GetJobsResponseTypeDef,
@@ -196,18 +183,14 @@
     JobUpdateTypeDef,
     LakeFormationConfigurationTypeDef,
     LineageConfigurationTypeDef,
     ListBlueprintsResponseTypeDef,
     ListCrawlersResponseTypeDef,
     ListCrawlsResponseTypeDef,
     ListCustomEntityTypesResponseTypeDef,
-    ListDataQualityResultsResponseTypeDef,
-    ListDataQualityRuleRecommendationRunsResponseTypeDef,
-    ListDataQualityRulesetEvaluationRunsResponseTypeDef,
-    ListDataQualityRulesetsResponseTypeDef,
     ListDevEndpointsResponseTypeDef,
     ListJobsResponseTypeDef,
     ListMLTransformsResponseTypeDef,
     ListRegistriesResponseTypeDef,
     ListSchemasResponseTypeDef,
     ListSchemaVersionsResponseTypeDef,
     ListSessionsResponseTypeDef,
@@ -238,16 +221,14 @@
     SchemaVersionNumberTypeDef,
     SearchTablesResponseTypeDef,
     SegmentTypeDef,
     SessionCommandTypeDef,
     SortCriterionTypeDef,
     SourceControlDetailsTypeDef,
     StartBlueprintRunResponseTypeDef,
-    StartDataQualityRuleRecommendationRunResponseTypeDef,
-    StartDataQualityRulesetEvaluationRunResponseTypeDef,
     StartExportLabelsTaskRunResponseTypeDef,
     StartImportLabelsTaskRunResponseTypeDef,
     StartJobRunResponseTypeDef,
     StartMLEvaluationTaskRunResponseTypeDef,
     StartMLLabelingSetGenerationTaskRunResponseTypeDef,
     StartTriggerResponseTypeDef,
     StartWorkflowRunResponseTypeDef,
@@ -261,15 +242,14 @@
     TransformParametersTypeDef,
     TransformSortCriteriaTypeDef,
     TriggerUpdateTypeDef,
     UpdateBlueprintResponseTypeDef,
     UpdateColumnStatisticsForPartitionResponseTypeDef,
     UpdateColumnStatisticsForTableResponseTypeDef,
     UpdateCsvClassifierRequestTypeDef,
-    UpdateDataQualityRulesetResponseTypeDef,
     UpdateGrokClassifierRequestTypeDef,
     UpdateJobFromSourceControlResponseTypeDef,
     UpdateJobResponseTypeDef,
     UpdateJsonClassifierRequestTypeDef,
     UpdateMLTransformResponseTypeDef,
     UpdateRegistryResponseTypeDef,
     UpdateSchemaResponseTypeDef,
@@ -427,23 +407,14 @@
     ) -> BatchGetCustomEntityTypesResponseTypeDef:
         """
         Retrieves the details for the custom patterns specified by a list of names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_get_custom_entity_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#batch_get_custom_entity_types)
         """
-    def batch_get_data_quality_result(
-        self, *, ResultIds: Sequence[str]
-    ) -> BatchGetDataQualityResultResponseTypeDef:
-        """
-        Retrieves a list of data quality results for the specified result IDs.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.batch_get_data_quality_result)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#batch_get_data_quality_result)
-        """
     def batch_get_dev_endpoints(
         self, *, DevEndpointNames: Sequence[str]
     ) -> BatchGetDevEndpointsResponseTypeDef:
         """
         Returns a list of resource metadata for a given list of development endpoint
         names.
 
@@ -513,28 +484,14 @@
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#can_paginate)
         """
-    def cancel_data_quality_rule_recommendation_run(self, *, RunId: str) -> Dict[str, Any]:
-        """
-        Cancels the specified recommendation run that was being used to generate rules.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.cancel_data_quality_rule_recommendation_run)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#cancel_data_quality_rule_recommendation_run)
-        """
-    def cancel_data_quality_ruleset_evaluation_run(self, *, RunId: str) -> Dict[str, Any]:
-        """
-        Cancels a run where a ruleset is being evaluated against a data source.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.cancel_data_quality_ruleset_evaluation_run)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#cancel_data_quality_ruleset_evaluation_run)
-        """
     def cancel_ml_task_run(
         self, *, TransformId: str, TaskRunId: str
     ) -> CancelMLTaskRunResponseTypeDef:
         """
         Cancels (stops) a task run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.cancel_ml_task_run)
@@ -638,31 +595,14 @@
         """
         Creates a custom pattern that is used to detect sensitive data across the
         columns and rows of your structured data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_custom_entity_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#create_custom_entity_type)
         """
-    def create_data_quality_ruleset(
-        self,
-        *,
-        Name: str,
-        Ruleset: str,
-        Description: str = ...,
-        Tags: Mapping[str, str] = ...,
-        TargetTable: DataQualityTargetTableTypeDef = ...,
-        ClientToken: str = ...
-    ) -> CreateDataQualityRulesetResponseTypeDef:
-        """
-        Creates a data quality ruleset with DQDL rules applied to a specified Glue
-        table.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.create_data_quality_ruleset)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#create_data_quality_ruleset)
-        """
     def create_database(
         self,
         *,
         DatabaseInput: DatabaseInputTypeDef,
         CatalogId: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> Dict[str, Any]:
@@ -972,21 +912,14 @@
     def delete_custom_entity_type(self, *, Name: str) -> DeleteCustomEntityTypeResponseTypeDef:
         """
         Deletes a custom pattern by specifying its name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.delete_custom_entity_type)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#delete_custom_entity_type)
         """
-    def delete_data_quality_ruleset(self, *, Name: str) -> Dict[str, Any]:
-        """
-        Deletes a data quality ruleset.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.delete_data_quality_ruleset)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#delete_data_quality_ruleset)
-        """
     def delete_database(self, *, Name: str, CatalogId: str = ...) -> Dict[str, Any]:
         """
         Removes a specified database from a Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.delete_database)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#delete_database)
         """
@@ -1271,46 +1204,14 @@
     ) -> GetDataCatalogEncryptionSettingsResponseTypeDef:
         """
         Retrieves the security configuration for a specified catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_data_catalog_encryption_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_data_catalog_encryption_settings)
         """
-    def get_data_quality_result(self, *, ResultId: str) -> GetDataQualityResultResponseTypeDef:
-        """
-        Retrieves the result of a data quality rule evaluation.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_data_quality_result)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_data_quality_result)
-        """
-    def get_data_quality_rule_recommendation_run(
-        self, *, RunId: str
-    ) -> GetDataQualityRuleRecommendationRunResponseTypeDef:
-        """
-        Gets the specified recommendation run that was used to generate rules.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_data_quality_rule_recommendation_run)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_data_quality_rule_recommendation_run)
-        """
-    def get_data_quality_ruleset(self, *, Name: str) -> GetDataQualityRulesetResponseTypeDef:
-        """
-        Returns an existing ruleset by identifier or name.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_data_quality_ruleset)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_data_quality_ruleset)
-        """
-    def get_data_quality_ruleset_evaluation_run(
-        self, *, RunId: str
-    ) -> GetDataQualityRulesetEvaluationRunResponseTypeDef:
-        """
-        Retrieves a specific run where a ruleset is evaluated against a data source.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_data_quality_ruleset_evaluation_run)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_data_quality_ruleset_evaluation_run)
-        """
     def get_database(self, *, Name: str, CatalogId: str = ...) -> GetDatabaseResponseTypeDef:
         """
         Retrieves the definition of a specified database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_database)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_database)
         """
@@ -1694,16 +1595,16 @@
         DatabaseName: str,
         TableName: str,
         PartitionValues: Sequence[str],
         SupportedPermissionTypes: Sequence[PermissionTypeType],
         AuditContext: AuditContextTypeDef = ...
     ) -> GetUnfilteredPartitionMetadataResponseTypeDef:
         """
-        Retrieves partition metadata from the Data Catalog that contains unfiltered
-        metadata.
+        See also: [AWS API
+        Documentation](https://docs.aws.amazon.com/goto/WebAPI/glue-2017-03-31/GetUnfilteredPartitionMetadata).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_unfiltered_partition_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_unfiltered_partition_metadata)
         """
     def get_unfiltered_partitions_metadata(
         self,
         *,
@@ -1714,32 +1615,32 @@
         Expression: str = ...,
         AuditContext: AuditContextTypeDef = ...,
         NextToken: str = ...,
         Segment: SegmentTypeDef = ...,
         MaxResults: int = ...
     ) -> GetUnfilteredPartitionsMetadataResponseTypeDef:
         """
-        Retrieves partition metadata from the Data Catalog that contains unfiltered
-        metadata.
+        See also: [AWS API
+        Documentation](https://docs.aws.amazon.com/goto/WebAPI/glue-2017-03-31/GetUnfilteredPartitionsMetadata).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_unfiltered_partitions_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_unfiltered_partitions_metadata)
         """
     def get_unfiltered_table_metadata(
         self,
         *,
         CatalogId: str,
         DatabaseName: str,
         Name: str,
         SupportedPermissionTypes: Sequence[PermissionTypeType],
         AuditContext: AuditContextTypeDef = ...
     ) -> GetUnfilteredTableMetadataResponseTypeDef:
         """
-        Retrieves table metadata from the Data Catalog that contains unfiltered
-        metadata.
+        See also: [AWS API
+        Documentation](https://docs.aws.amazon.com/goto/WebAPI/glue-2017-03-31/GetUnfilteredTableMetadata).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.get_unfiltered_table_metadata)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#get_unfiltered_table_metadata)
         """
     def get_user_defined_function(
         self, *, DatabaseName: str, FunctionName: str, CatalogId: str = ...
     ) -> GetUserDefinedFunctionResponseTypeDef:
@@ -1843,68 +1744,14 @@
     ) -> ListCustomEntityTypesResponseTypeDef:
         """
         Lists all the custom patterns that have been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_custom_entity_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#list_custom_entity_types)
         """
-    def list_data_quality_results(
-        self,
-        *,
-        Filter: DataQualityResultFilterCriteriaTypeDef = ...,
-        NextToken: str = ...,
-        MaxResults: int = ...
-    ) -> ListDataQualityResultsResponseTypeDef:
-        """
-        Returns all data quality execution results for your account.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_results)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#list_data_quality_results)
-        """
-    def list_data_quality_rule_recommendation_runs(
-        self,
-        *,
-        Filter: DataQualityRuleRecommendationRunFilterTypeDef = ...,
-        NextToken: str = ...,
-        MaxResults: int = ...
-    ) -> ListDataQualityRuleRecommendationRunsResponseTypeDef:
-        """
-        Lists the recommendation runs meeting the filter criteria.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_rule_recommendation_runs)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#list_data_quality_rule_recommendation_runs)
-        """
-    def list_data_quality_ruleset_evaluation_runs(
-        self,
-        *,
-        Filter: DataQualityRulesetEvaluationRunFilterTypeDef = ...,
-        NextToken: str = ...,
-        MaxResults: int = ...
-    ) -> ListDataQualityRulesetEvaluationRunsResponseTypeDef:
-        """
-        Lists all the runs meeting the filter criteria, where a ruleset is evaluated
-        against a data source.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_ruleset_evaluation_runs)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#list_data_quality_ruleset_evaluation_runs)
-        """
-    def list_data_quality_rulesets(
-        self,
-        *,
-        NextToken: str = ...,
-        MaxResults: int = ...,
-        Filter: DataQualityRulesetFilterCriteriaTypeDef = ...,
-        Tags: Mapping[str, str] = ...
-    ) -> ListDataQualityRulesetsResponseTypeDef:
-        """
-        Returns a paginated list of rulesets for the specified list of Glue tables.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.list_data_quality_rulesets)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#list_data_quality_rulesets)
-        """
     def list_dev_endpoints(
         self, *, NextToken: str = ..., MaxResults: int = ..., Tags: Mapping[str, str] = ...
     ) -> ListDevEndpointsResponseTypeDef:
         """
         Retrieves the names of all `DevEndpoint` resources in this Amazon Web Services
         account, or the resources with the specified tag.
 
@@ -2170,49 +2017,14 @@
         """
         Changes the schedule state of the specified crawler to `SCHEDULED` , unless the
         crawler is already running or the schedule state is already `SCHEDULED` .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_crawler_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#start_crawler_schedule)
         """
-    def start_data_quality_rule_recommendation_run(
-        self,
-        *,
-        DataSource: DataSourceTypeDef,
-        Role: str,
-        NumberOfWorkers: int = ...,
-        Timeout: int = ...,
-        CreatedRulesetName: str = ...,
-        ClientToken: str = ...
-    ) -> StartDataQualityRuleRecommendationRunResponseTypeDef:
-        """
-        Starts a recommendation run that is used to generate rules when you don't know
-        what rules to write.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_data_quality_rule_recommendation_run)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#start_data_quality_rule_recommendation_run)
-        """
-    def start_data_quality_ruleset_evaluation_run(
-        self,
-        *,
-        DataSource: DataSourceTypeDef,
-        Role: str,
-        RulesetNames: Sequence[str],
-        NumberOfWorkers: int = ...,
-        Timeout: int = ...,
-        ClientToken: str = ...,
-        AdditionalRunOptions: DataQualityEvaluationRunAdditionalRunOptionsTypeDef = ...
-    ) -> StartDataQualityRulesetEvaluationRunResponseTypeDef:
-        """
-        Once you have a ruleset definition (either recommended or your own), you call
-        this operation to evaluate the ruleset against a data source (Glue table).
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.start_data_quality_ruleset_evaluation_run)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#start_data_quality_ruleset_evaluation_run)
-        """
     def start_export_labels_task_run(
         self, *, TransformId: str, OutputS3Path: str
     ) -> StartExportLabelsTaskRunResponseTypeDef:
         """
         Begins an asynchronous task to export all labeled data for a particular
         transform.
 
@@ -2424,23 +2236,14 @@
     def update_crawler_schedule(self, *, CrawlerName: str, Schedule: str = ...) -> Dict[str, Any]:
         """
         Updates the schedule of a crawler using a `cron` expression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_crawler_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#update_crawler_schedule)
         """
-    def update_data_quality_ruleset(
-        self, *, Name: str, UpdatedName: str = ..., Description: str = ..., Ruleset: str = ...
-    ) -> UpdateDataQualityRulesetResponseTypeDef:
-        """
-        Updates the specified data quality ruleset.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_data_quality_ruleset)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/client/#update_data_quality_ruleset)
-        """
     def update_database(
         self, *, Name: str, DatabaseInput: DatabaseInputTypeDef, CatalogId: str = ...
     ) -> Dict[str, Any]:
         """
         Updates an existing database definition in a Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue.Client.update_database)
```

### Comparing `mypy-boto3-glue-1.26.74/mypy_boto3_glue/literals.py` & `mypy-boto3-glue-1.26.8/mypy_boto3_glue/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,20 +33,16 @@
     "ConnectionPropertyKeyType",
     "ConnectionTypeType",
     "CrawlStateType",
     "CrawlerHistoryStateType",
     "CrawlerLineageSettingsType",
     "CrawlerStateType",
     "CsvHeaderOptionType",
-    "DQStopJobOnFailureTimingType",
-    "DQTransformOutputType",
     "DataFormatType",
-    "DataQualityRuleResultStatusType",
     "DeleteBehaviorType",
-    "DeltaTargetCompressionTypeType",
     "EnableHybridValuesType",
     "ExecutionClassType",
     "ExistConditionType",
     "FieldNameType",
     "FilterLogicalOperatorType",
     "FilterOperationType",
     "FilterOperatorType",
@@ -64,31 +60,27 @@
     "GetResourcePoliciesPaginatorName",
     "GetSecurityConfigurationsPaginatorName",
     "GetTableVersionsPaginatorName",
     "GetTablesPaginatorName",
     "GetTriggersPaginatorName",
     "GetUserDefinedFunctionsPaginatorName",
     "GlueRecordTypeType",
-    "HudiTargetCompressionTypeType",
-    "JDBCConnectionTypeType",
     "JDBCDataTypeType",
-    "JdbcMetadataEntryType",
     "JobBookmarksEncryptionModeType",
     "JobRunStateType",
     "JoinTypeType",
     "LanguageType",
     "LastCrawlStatusType",
     "ListRegistriesPaginatorName",
     "ListSchemaVersionsPaginatorName",
     "ListSchemasPaginatorName",
     "LogicalOperatorType",
     "LogicalType",
     "MLUserDataEncryptionModeStringType",
     "NodeTypeType",
-    "ParamTypeType",
     "ParquetCompressionTypeType",
     "PartitionIndexStatusType",
     "PermissionType",
     "PermissionTypeType",
     "PiiTypeType",
     "PrincipalTypeType",
     "QuoteCharType",
@@ -203,20 +195,16 @@
 ]
 ConnectionTypeType = Literal["CUSTOM", "JDBC", "KAFKA", "MARKETPLACE", "MONGODB", "NETWORK", "SFTP"]
 CrawlStateType = Literal["CANCELLED", "CANCELLING", "ERROR", "FAILED", "RUNNING", "SUCCEEDED"]
 CrawlerHistoryStateType = Literal["COMPLETED", "FAILED", "RUNNING", "STOPPED"]
 CrawlerLineageSettingsType = Literal["DISABLE", "ENABLE"]
 CrawlerStateType = Literal["READY", "RUNNING", "STOPPING"]
 CsvHeaderOptionType = Literal["ABSENT", "PRESENT", "UNKNOWN"]
-DQStopJobOnFailureTimingType = Literal["AfterDataLoad", "Immediate"]
-DQTransformOutputType = Literal["EvaluationResults", "PrimaryInput"]
 DataFormatType = Literal["AVRO", "JSON", "PROTOBUF"]
-DataQualityRuleResultStatusType = Literal["ERROR", "FAIL", "PASS"]
 DeleteBehaviorType = Literal["DELETE_FROM_DATABASE", "DEPRECATE_IN_DATABASE", "LOG"]
-DeltaTargetCompressionTypeType = Literal["snappy", "uncompressed"]
 EnableHybridValuesType = Literal["FALSE", "TRUE"]
 ExecutionClassType = Literal["FLEX", "STANDARD"]
 ExistConditionType = Literal["MUST_EXIST", "NONE", "NOT_EXIST"]
 FieldNameType = Literal["CRAWL_ID", "DPU_HOUR", "END_TIME", "START_TIME", "STATE"]
 FilterLogicalOperatorType = Literal["AND", "OR"]
 FilterOperationType = Literal["EQ", "GT", "GTE", "ISNULL", "LT", "LTE", "REGEX"]
 FilterOperatorType = Literal["EQ", "GE", "GT", "LE", "LT", "NE"]
@@ -236,16 +224,14 @@
 GetTableVersionsPaginatorName = Literal["get_table_versions"]
 GetTablesPaginatorName = Literal["get_tables"]
 GetTriggersPaginatorName = Literal["get_triggers"]
 GetUserDefinedFunctionsPaginatorName = Literal["get_user_defined_functions"]
 GlueRecordTypeType = Literal[
     "BIGDECIMAL", "BYTE", "DATE", "DOUBLE", "FLOAT", "INT", "LONG", "SHORT", "STRING", "TIMESTAMP"
 ]
-HudiTargetCompressionTypeType = Literal["gzip", "lzo", "snappy", "uncompressed"]
-JDBCConnectionTypeType = Literal["mysql", "oracle", "postgresql", "redshift", "sqlserver"]
 JDBCDataTypeType = Literal[
     "ARRAY",
     "BIGINT",
     "BINARY",
     "BIT",
     "BLOB",
     "BOOLEAN",
@@ -279,15 +265,14 @@
     "TIMESTAMP",
     "TIMESTAMP_WITH_TIMEZONE",
     "TIME_WITH_TIMEZONE",
     "TINYINT",
     "VARBINARY",
     "VARCHAR",
 ]
-JdbcMetadataEntryType = Literal["COMMENTS", "RAWTYPES"]
 JobBookmarksEncryptionModeType = Literal["CSE-KMS", "DISABLED"]
 JobRunStateType = Literal[
     "ERROR",
     "FAILED",
     "RUNNING",
     "STARTING",
     "STOPPED",
@@ -302,15 +287,14 @@
 ListRegistriesPaginatorName = Literal["list_registries"]
 ListSchemaVersionsPaginatorName = Literal["list_schema_versions"]
 ListSchemasPaginatorName = Literal["list_schemas"]
 LogicalOperatorType = Literal["EQUALS"]
 LogicalType = Literal["AND", "ANY"]
 MLUserDataEncryptionModeStringType = Literal["DISABLED", "SSE-KMS"]
 NodeTypeType = Literal["CRAWLER", "JOB", "TRIGGER"]
-ParamTypeType = Literal["bool", "complex", "float", "int", "list", "null", "str"]
 ParquetCompressionTypeType = Literal["gzip", "lzo", "none", "snappy", "uncompressed"]
 PartitionIndexStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED"]
 PermissionType = Literal[
     "ALL",
     "ALTER",
     "CREATE_DATABASE",
     "CREATE_TABLE",
@@ -337,15 +321,15 @@
 SessionStatusType = Literal["FAILED", "PROVISIONING", "READY", "STOPPED", "STOPPING", "TIMEOUT"]
 SortDirectionTypeType = Literal["ASCENDING", "DESCENDING"]
 SortType = Literal["ASC", "DESC"]
 SourceControlAuthStrategyType = Literal["AWS_SECRETS_MANAGER", "PERSONAL_ACCESS_TOKEN"]
 SourceControlProviderType = Literal["AWS_CODE_COMMIT", "GITHUB"]
 StartingPositionType = Literal["earliest", "latest", "trim_horizon"]
 StatementStateType = Literal["AVAILABLE", "CANCELLED", "CANCELLING", "ERROR", "RUNNING", "WAITING"]
-TargetFormatType = Literal["avro", "csv", "delta", "hudi", "json", "orc", "parquet"]
+TargetFormatType = Literal["avro", "csv", "json", "orc", "parquet"]
 TaskRunSortColumnTypeType = Literal["STARTED", "STATUS", "TASK_RUN_TYPE"]
 TaskStatusTypeType = Literal[
     "FAILED", "RUNNING", "STARTING", "STOPPED", "STOPPING", "SUCCEEDED", "TIMEOUT"
 ]
 TaskTypeType = Literal[
     "EVALUATION", "EXPORT_LABELS", "FIND_MATCHES", "IMPORT_LABELS", "LABELING_SET_GENERATION"
 ]
@@ -391,15 +375,14 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
-    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -409,31 +392,27 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
-    "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
-    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -462,15 +441,14 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
-    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -518,15 +496,14 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -537,33 +514,30 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -595,32 +569,28 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
-    "oam",
-    "omics",
     "opensearch",
-    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
-    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -648,44 +618,39 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
-    "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
-    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
-    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
@@ -758,15 +723,14 @@
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
-    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-glue-1.26.74/mypy_boto3_glue/literals.pyi` & `mypy-boto3-glue-1.26.8/mypy_boto3_glue/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -32,20 +32,16 @@
     "ConnectionPropertyKeyType",
     "ConnectionTypeType",
     "CrawlStateType",
     "CrawlerHistoryStateType",
     "CrawlerLineageSettingsType",
     "CrawlerStateType",
     "CsvHeaderOptionType",
-    "DQStopJobOnFailureTimingType",
-    "DQTransformOutputType",
     "DataFormatType",
-    "DataQualityRuleResultStatusType",
     "DeleteBehaviorType",
-    "DeltaTargetCompressionTypeType",
     "EnableHybridValuesType",
     "ExecutionClassType",
     "ExistConditionType",
     "FieldNameType",
     "FilterLogicalOperatorType",
     "FilterOperationType",
     "FilterOperatorType",
@@ -63,31 +59,27 @@
     "GetResourcePoliciesPaginatorName",
     "GetSecurityConfigurationsPaginatorName",
     "GetTableVersionsPaginatorName",
     "GetTablesPaginatorName",
     "GetTriggersPaginatorName",
     "GetUserDefinedFunctionsPaginatorName",
     "GlueRecordTypeType",
-    "HudiTargetCompressionTypeType",
-    "JDBCConnectionTypeType",
     "JDBCDataTypeType",
-    "JdbcMetadataEntryType",
     "JobBookmarksEncryptionModeType",
     "JobRunStateType",
     "JoinTypeType",
     "LanguageType",
     "LastCrawlStatusType",
     "ListRegistriesPaginatorName",
     "ListSchemaVersionsPaginatorName",
     "ListSchemasPaginatorName",
     "LogicalOperatorType",
     "LogicalType",
     "MLUserDataEncryptionModeStringType",
     "NodeTypeType",
-    "ParamTypeType",
     "ParquetCompressionTypeType",
     "PartitionIndexStatusType",
     "PermissionType",
     "PermissionTypeType",
     "PiiTypeType",
     "PrincipalTypeType",
     "QuoteCharType",
@@ -201,20 +193,16 @@
 ]
 ConnectionTypeType = Literal["CUSTOM", "JDBC", "KAFKA", "MARKETPLACE", "MONGODB", "NETWORK", "SFTP"]
 CrawlStateType = Literal["CANCELLED", "CANCELLING", "ERROR", "FAILED", "RUNNING", "SUCCEEDED"]
 CrawlerHistoryStateType = Literal["COMPLETED", "FAILED", "RUNNING", "STOPPED"]
 CrawlerLineageSettingsType = Literal["DISABLE", "ENABLE"]
 CrawlerStateType = Literal["READY", "RUNNING", "STOPPING"]
 CsvHeaderOptionType = Literal["ABSENT", "PRESENT", "UNKNOWN"]
-DQStopJobOnFailureTimingType = Literal["AfterDataLoad", "Immediate"]
-DQTransformOutputType = Literal["EvaluationResults", "PrimaryInput"]
 DataFormatType = Literal["AVRO", "JSON", "PROTOBUF"]
-DataQualityRuleResultStatusType = Literal["ERROR", "FAIL", "PASS"]
 DeleteBehaviorType = Literal["DELETE_FROM_DATABASE", "DEPRECATE_IN_DATABASE", "LOG"]
-DeltaTargetCompressionTypeType = Literal["snappy", "uncompressed"]
 EnableHybridValuesType = Literal["FALSE", "TRUE"]
 ExecutionClassType = Literal["FLEX", "STANDARD"]
 ExistConditionType = Literal["MUST_EXIST", "NONE", "NOT_EXIST"]
 FieldNameType = Literal["CRAWL_ID", "DPU_HOUR", "END_TIME", "START_TIME", "STATE"]
 FilterLogicalOperatorType = Literal["AND", "OR"]
 FilterOperationType = Literal["EQ", "GT", "GTE", "ISNULL", "LT", "LTE", "REGEX"]
 FilterOperatorType = Literal["EQ", "GE", "GT", "LE", "LT", "NE"]
@@ -234,16 +222,14 @@
 GetTableVersionsPaginatorName = Literal["get_table_versions"]
 GetTablesPaginatorName = Literal["get_tables"]
 GetTriggersPaginatorName = Literal["get_triggers"]
 GetUserDefinedFunctionsPaginatorName = Literal["get_user_defined_functions"]
 GlueRecordTypeType = Literal[
     "BIGDECIMAL", "BYTE", "DATE", "DOUBLE", "FLOAT", "INT", "LONG", "SHORT", "STRING", "TIMESTAMP"
 ]
-HudiTargetCompressionTypeType = Literal["gzip", "lzo", "snappy", "uncompressed"]
-JDBCConnectionTypeType = Literal["mysql", "oracle", "postgresql", "redshift", "sqlserver"]
 JDBCDataTypeType = Literal[
     "ARRAY",
     "BIGINT",
     "BINARY",
     "BIT",
     "BLOB",
     "BOOLEAN",
@@ -277,15 +263,14 @@
     "TIMESTAMP",
     "TIMESTAMP_WITH_TIMEZONE",
     "TIME_WITH_TIMEZONE",
     "TINYINT",
     "VARBINARY",
     "VARCHAR",
 ]
-JdbcMetadataEntryType = Literal["COMMENTS", "RAWTYPES"]
 JobBookmarksEncryptionModeType = Literal["CSE-KMS", "DISABLED"]
 JobRunStateType = Literal[
     "ERROR",
     "FAILED",
     "RUNNING",
     "STARTING",
     "STOPPED",
@@ -300,15 +285,14 @@
 ListRegistriesPaginatorName = Literal["list_registries"]
 ListSchemaVersionsPaginatorName = Literal["list_schema_versions"]
 ListSchemasPaginatorName = Literal["list_schemas"]
 LogicalOperatorType = Literal["EQUALS"]
 LogicalType = Literal["AND", "ANY"]
 MLUserDataEncryptionModeStringType = Literal["DISABLED", "SSE-KMS"]
 NodeTypeType = Literal["CRAWLER", "JOB", "TRIGGER"]
-ParamTypeType = Literal["bool", "complex", "float", "int", "list", "null", "str"]
 ParquetCompressionTypeType = Literal["gzip", "lzo", "none", "snappy", "uncompressed"]
 PartitionIndexStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED"]
 PermissionType = Literal[
     "ALL",
     "ALTER",
     "CREATE_DATABASE",
     "CREATE_TABLE",
@@ -335,15 +319,15 @@
 SessionStatusType = Literal["FAILED", "PROVISIONING", "READY", "STOPPED", "STOPPING", "TIMEOUT"]
 SortDirectionTypeType = Literal["ASCENDING", "DESCENDING"]
 SortType = Literal["ASC", "DESC"]
 SourceControlAuthStrategyType = Literal["AWS_SECRETS_MANAGER", "PERSONAL_ACCESS_TOKEN"]
 SourceControlProviderType = Literal["AWS_CODE_COMMIT", "GITHUB"]
 StartingPositionType = Literal["earliest", "latest", "trim_horizon"]
 StatementStateType = Literal["AVAILABLE", "CANCELLED", "CANCELLING", "ERROR", "RUNNING", "WAITING"]
-TargetFormatType = Literal["avro", "csv", "delta", "hudi", "json", "orc", "parquet"]
+TargetFormatType = Literal["avro", "csv", "json", "orc", "parquet"]
 TaskRunSortColumnTypeType = Literal["STARTED", "STATUS", "TASK_RUN_TYPE"]
 TaskStatusTypeType = Literal[
     "FAILED", "RUNNING", "STARTING", "STOPPED", "STOPPING", "SUCCEEDED", "TIMEOUT"
 ]
 TaskTypeType = Literal[
     "EVALUATION", "EXPORT_LABELS", "FIND_MATCHES", "IMPORT_LABELS", "LABELING_SET_GENERATION"
 ]
@@ -389,15 +373,14 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
-    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -407,31 +390,27 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
-    "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
-    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -460,15 +439,14 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
-    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -516,15 +494,14 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -535,33 +512,30 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -593,32 +567,28 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
-    "oam",
-    "omics",
     "opensearch",
-    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
-    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -646,44 +616,39 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
-    "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
-    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
-    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
@@ -756,15 +721,14 @@
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-south-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
-    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-glue-1.26.74/mypy_boto3_glue/paginator.py` & `mypy-boto3-glue-1.26.8/mypy_boto3_glue/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.26.74/mypy_boto3_glue/paginator.pyi` & `mypy-boto3-glue-1.26.8/mypy_boto3_glue/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.26.74/mypy_boto3_glue/type_defs.py` & `mypy-boto3-glue-1.26.8/mypy_boto3_glue/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -30,41 +30,33 @@
     ConnectionTypeType,
     CrawlerHistoryStateType,
     CrawlerLineageSettingsType,
     CrawlerStateType,
     CrawlStateType,
     CsvHeaderOptionType,
     DataFormatType,
-    DataQualityRuleResultStatusType,
     DeleteBehaviorType,
-    DeltaTargetCompressionTypeType,
-    DQStopJobOnFailureTimingType,
-    DQTransformOutputType,
     EnableHybridValuesType,
     ExecutionClassType,
     ExistConditionType,
     FieldNameType,
     FilterLogicalOperatorType,
     FilterOperationType,
     FilterOperatorType,
     FilterValueTypeType,
     GlueRecordTypeType,
-    HudiTargetCompressionTypeType,
-    JDBCConnectionTypeType,
     JDBCDataTypeType,
-    JdbcMetadataEntryType,
     JobBookmarksEncryptionModeType,
     JobRunStateType,
     JoinTypeType,
     LanguageType,
     LastCrawlStatusType,
     LogicalType,
     MLUserDataEncryptionModeStringType,
     NodeTypeType,
-    ParamTypeType,
     ParquetCompressionTypeType,
     PartitionIndexStatusType,
     PermissionType,
     PermissionTypeType,
     PiiTypeType,
     PrincipalTypeType,
     QuoteCharType,
@@ -104,15 +96,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "NotificationPropertyTypeDef",
     "AggregateOperationTypeDef",
     "ApplyMappingTypeDef",
     "AuditContextTypeDef",
     "PartitionValueListTypeDef",
     "BasicCatalogTargetTypeDef",
@@ -121,29 +112,26 @@
     "ErrorDetailTypeDef",
     "BatchDeleteTableRequestRequestTypeDef",
     "BatchDeleteTableVersionRequestRequestTypeDef",
     "BatchGetBlueprintsRequestRequestTypeDef",
     "BatchGetCrawlersRequestRequestTypeDef",
     "BatchGetCustomEntityTypesRequestRequestTypeDef",
     "CustomEntityTypeTypeDef",
-    "BatchGetDataQualityResultRequestRequestTypeDef",
     "BatchGetDevEndpointsRequestRequestTypeDef",
     "DevEndpointTypeDef",
     "BatchGetJobsRequestRequestTypeDef",
     "BatchGetTriggersRequestRequestTypeDef",
     "BatchGetWorkflowsRequestRequestTypeDef",
     "BatchStopJobRunRequestRequestTypeDef",
     "BatchStopJobRunSuccessfulSubmissionTypeDef",
     "BinaryColumnStatisticsDataTypeDef",
     "BlueprintDetailsTypeDef",
     "BlueprintRunTypeDef",
     "LastActiveDefinitionTypeDef",
     "BooleanColumnStatisticsDataTypeDef",
-    "CancelDataQualityRuleRecommendationRunRequestRequestTypeDef",
-    "CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef",
     "CancelMLTaskRunRequestRequestTypeDef",
     "CancelStatementRequestRequestTypeDef",
     "CatalogEntryTypeDef",
     "CatalogImportStatusTypeDef",
     "KafkaStreamingSourceOptionsTypeDef",
     "StreamingDataPreviewOptionsTypeDef",
     "KinesisStreamingSourceOptionsTypeDef",
@@ -152,15 +140,14 @@
     "CatalogTargetTypeDef",
     "CheckSchemaVersionValidityInputRequestTypeDef",
     "CsvClassifierTypeDef",
     "GrokClassifierTypeDef",
     "JsonClassifierTypeDef",
     "XMLClassifierTypeDef",
     "CloudWatchEncryptionTypeDef",
-    "DirectJDBCSourceTypeDef",
     "DropDuplicatesTypeDef",
     "DropFieldsTypeDef",
     "DynamoDBCatalogSourceTypeDef",
     "FillMissingValuesTypeDef",
     "MergeTypeDef",
     "MicrosoftSQLServerCatalogSourceTypeDef",
     "MicrosoftSQLServerCatalogTargetTypeDef",
@@ -210,43 +197,37 @@
     "CrawlsFilterTypeDef",
     "CreateBlueprintRequestRequestTypeDef",
     "CreateCsvClassifierRequestTypeDef",
     "CreateGrokClassifierRequestTypeDef",
     "CreateJsonClassifierRequestTypeDef",
     "CreateXMLClassifierRequestTypeDef",
     "CreateCustomEntityTypeRequestRequestTypeDef",
-    "DataQualityTargetTableTypeDef",
     "CreateDevEndpointRequestRequestTypeDef",
     "ExecutionPropertyTypeDef",
     "JobCommandTypeDef",
     "SourceControlDetailsTypeDef",
     "GlueTableTypeDef",
     "PartitionIndexTypeDef",
     "CreateRegistryInputRequestTypeDef",
     "RegistryIdTypeDef",
     "SessionCommandTypeDef",
     "EventBatchingConditionTypeDef",
     "CreateWorkflowRequestRequestTypeDef",
-    "DQResultsPublishingOptionsTypeDef",
-    "DQStopJobOnFailureOptionsTypeDef",
     "EncryptionAtRestTypeDef",
     "DataLakePrincipalTypeDef",
-    "DataQualityEvaluationRunAdditionalRunOptionsTypeDef",
-    "DataQualityRuleResultTypeDef",
     "DatabaseIdentifierTypeDef",
     "DatatypeTypeDef",
     "DecimalNumberTypeDef",
     "DeleteBlueprintRequestRequestTypeDef",
     "DeleteClassifierRequestRequestTypeDef",
     "DeleteColumnStatisticsForPartitionRequestRequestTypeDef",
     "DeleteColumnStatisticsForTableRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
     "DeleteCrawlerRequestRequestTypeDef",
     "DeleteCustomEntityTypeRequestRequestTypeDef",
-    "DeleteDataQualityRulesetRequestRequestTypeDef",
     "DeleteDatabaseRequestRequestTypeDef",
     "DeleteDevEndpointRequestRequestTypeDef",
     "DeleteJobRequestRequestTypeDef",
     "DeleteMLTransformRequestRequestTypeDef",
     "DeletePartitionIndexRequestRequestTypeDef",
     "DeletePartitionRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
@@ -257,15 +238,14 @@
     "DeleteTableVersionRequestRequestTypeDef",
     "DeleteTriggerRequestRequestTypeDef",
     "DeleteUserDefinedFunctionRequestRequestTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
     "DevEndpointCustomLibrariesTypeDef",
     "DirectSchemaChangePolicyTypeDef",
     "NullCheckBoxListTypeDef",
-    "TransformConfigParameterTypeDef",
     "EdgeTypeDef",
     "JobBookmarksEncryptionTypeDef",
     "S3EncryptionTypeDef",
     "ErrorDetailsTypeDef",
     "ExportLabelsTaskRunPropertiesTypeDef",
     "FilterValueTypeDef",
     "FindMatchesParametersTypeDef",
@@ -282,18 +262,14 @@
     "GetConnectionRequestRequestTypeDef",
     "GetConnectionsFilterTypeDef",
     "GetCrawlerMetricsRequestRequestTypeDef",
     "GetCrawlerRequestRequestTypeDef",
     "GetCrawlersRequestRequestTypeDef",
     "GetCustomEntityTypeRequestRequestTypeDef",
     "GetDataCatalogEncryptionSettingsRequestRequestTypeDef",
-    "GetDataQualityResultRequestRequestTypeDef",
-    "GetDataQualityRuleRecommendationRunRequestRequestTypeDef",
-    "GetDataQualityRulesetEvaluationRunRequestRequestTypeDef",
-    "GetDataQualityRulesetRequestRequestTypeDef",
     "GetDatabaseRequestRequestTypeDef",
     "GetDatabasesRequestRequestTypeDef",
     "GetDataflowGraphRequestRequestTypeDef",
     "GetDevEndpointRequestRequestTypeDef",
     "GetDevEndpointsRequestRequestTypeDef",
     "GetJobBookmarkRequestRequestTypeDef",
     "JobBookmarkEntryTypeDef",
@@ -393,15 +369,14 @@
     "UntagResourceRequestRequestTypeDef",
     "UpdateBlueprintRequestRequestTypeDef",
     "UpdateCsvClassifierRequestTypeDef",
     "UpdateGrokClassifierRequestTypeDef",
     "UpdateJsonClassifierRequestTypeDef",
     "UpdateXMLClassifierRequestTypeDef",
     "UpdateCrawlerScheduleRequestRequestTypeDef",
-    "UpdateDataQualityRulesetRequestRequestTypeDef",
     "UpdateJobFromSourceControlRequestRequestTypeDef",
     "UpdateSourceControlFromJobRequestRequestTypeDef",
     "UpdateWorkflowRequestRequestTypeDef",
     "WorkflowRunStatisticsTypeDef",
     "ActionTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "AggregateTypeDef",
@@ -410,15 +385,14 @@
     "BackfillErrorTypeDef",
     "BatchDeletePartitionRequestRequestTypeDef",
     "BatchGetPartitionRequestRequestTypeDef",
     "CancelMLTaskRunResponseTypeDef",
     "CheckSchemaVersionValidityResponseTypeDef",
     "CreateBlueprintResponseTypeDef",
     "CreateCustomEntityTypeResponseTypeDef",
-    "CreateDataQualityRulesetResponseTypeDef",
     "CreateDevEndpointResponseTypeDef",
     "CreateJobResponseTypeDef",
     "CreateMLTransformResponseTypeDef",
     "CreateRegistryResponseTypeDef",
     "CreateSchemaResponseTypeDef",
     "CreateScriptResponseTypeDef",
     "CreateSecurityConfigurationResponseTypeDef",
@@ -453,27 +427,24 @@
     "PutResourcePolicyResponseTypeDef",
     "PutSchemaVersionMetadataResponseTypeDef",
     "RegisterSchemaVersionResponseTypeDef",
     "RemoveSchemaVersionMetadataResponseTypeDef",
     "ResumeWorkflowRunResponseTypeDef",
     "RunStatementResponseTypeDef",
     "StartBlueprintRunResponseTypeDef",
-    "StartDataQualityRuleRecommendationRunResponseTypeDef",
-    "StartDataQualityRulesetEvaluationRunResponseTypeDef",
     "StartExportLabelsTaskRunResponseTypeDef",
     "StartImportLabelsTaskRunResponseTypeDef",
     "StartJobRunResponseTypeDef",
     "StartMLEvaluationTaskRunResponseTypeDef",
     "StartMLLabelingSetGenerationTaskRunResponseTypeDef",
     "StartTriggerResponseTypeDef",
     "StartWorkflowRunResponseTypeDef",
     "StopSessionResponseTypeDef",
     "StopTriggerResponseTypeDef",
     "UpdateBlueprintResponseTypeDef",
-    "UpdateDataQualityRulesetResponseTypeDef",
     "UpdateJobFromSourceControlResponseTypeDef",
     "UpdateJobResponseTypeDef",
     "UpdateMLTransformResponseTypeDef",
     "UpdateRegistryResponseTypeDef",
     "UpdateSchemaResponseTypeDef",
     "UpdateSourceControlFromJobResponseTypeDef",
     "UpdateWorkflowResponseTypeDef",
@@ -495,60 +466,49 @@
     "GetCatalogImportStatusResponseTypeDef",
     "CatalogKafkaSourceTypeDef",
     "DirectKafkaSourceTypeDef",
     "CatalogKinesisSourceTypeDef",
     "DirectKinesisSourceTypeDef",
     "GovernedCatalogTargetTypeDef",
     "S3CatalogTargetTypeDef",
-    "S3DeltaCatalogTargetTypeDef",
-    "S3HudiCatalogTargetTypeDef",
     "ClassifierTypeDef",
     "CodeGenNodeTypeDef",
     "LocationTypeDef",
     "PredicateTypeDef",
     "FindMatchesMetricsTypeDef",
     "ConnectionInputTypeDef",
     "ConnectionTypeDef",
     "CrawlerNodeDetailsTypeDef",
     "ListCrawlsResponseTypeDef",
     "GetCrawlerMetricsResponseTypeDef",
     "CrawlerTargetsTypeDef",
     "ListCrawlsRequestRequestTypeDef",
     "CreateClassifierRequestRequestTypeDef",
-    "CreateDataQualityRulesetRequestRequestTypeDef",
-    "DataQualityRulesetFilterCriteriaTypeDef",
-    "DataQualityRulesetListDetailsTypeDef",
-    "GetDataQualityRulesetResponseTypeDef",
-    "DataSourceTypeDef",
     "CreatePartitionIndexRequestRequestTypeDef",
     "CreateSchemaInputRequestTypeDef",
     "DeleteRegistryInputRequestTypeDef",
     "GetRegistryInputRequestTypeDef",
     "ListSchemasInputRequestTypeDef",
     "UpdateRegistryInputRequestTypeDef",
     "CreateSessionRequestRequestTypeDef",
     "SessionTypeDef",
-    "EvaluateDataQualityTypeDef",
     "DataCatalogEncryptionSettingsTypeDef",
     "PrincipalPermissionsTypeDef",
     "NullValueFieldTypeDef",
     "DecimalColumnStatisticsDataTypeDef",
     "DeleteSchemaInputRequestTypeDef",
     "DeleteSchemaVersionsInputRequestTypeDef",
     "GetSchemaByDefinitionInputRequestTypeDef",
     "GetSchemaInputRequestTypeDef",
     "ListSchemaVersionsInputRequestTypeDef",
     "RegisterSchemaVersionInputRequestTypeDef",
     "SchemaReferenceTypeDef",
     "UpdateDevEndpointRequestRequestTypeDef",
-    "S3DeltaDirectTargetTypeDef",
     "S3DirectTargetTypeDef",
     "S3GlueParquetTargetTypeDef",
-    "S3HudiDirectTargetTypeDef",
-    "DynamicTransformTypeDef",
     "EncryptionConfigurationTypeDef",
     "SchemaVersionErrorItemTypeDef",
     "FilterExpressionTypeDef",
     "TransformParametersTypeDef",
     "GetClassifiersRequestGetClassifiersPaginateTypeDef",
     "GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef",
     "GetCrawlersRequestGetCrawlersPaginateTypeDef",
@@ -622,28 +582,14 @@
     "CreateConnectionRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "GetConnectionResponseTypeDef",
     "GetConnectionsResponseTypeDef",
     "CrawlerTypeDef",
     "CreateCrawlerRequestRequestTypeDef",
     "UpdateCrawlerRequestRequestTypeDef",
-    "ListDataQualityRulesetsRequestRequestTypeDef",
-    "ListDataQualityRulesetsResponseTypeDef",
-    "DataQualityResultDescriptionTypeDef",
-    "DataQualityResultFilterCriteriaTypeDef",
-    "DataQualityResultTypeDef",
-    "DataQualityRuleRecommendationRunDescriptionTypeDef",
-    "DataQualityRuleRecommendationRunFilterTypeDef",
-    "DataQualityRulesetEvaluationRunDescriptionTypeDef",
-    "DataQualityRulesetEvaluationRunFilterTypeDef",
-    "GetDataQualityResultResponseTypeDef",
-    "GetDataQualityRuleRecommendationRunResponseTypeDef",
-    "GetDataQualityRulesetEvaluationRunResponseTypeDef",
-    "StartDataQualityRuleRecommendationRunRequestRequestTypeDef",
-    "StartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
     "CreateSessionResponseTypeDef",
     "GetSessionResponseTypeDef",
     "ListSessionsResponseTypeDef",
     "GetDataCatalogEncryptionSettingsResponseTypeDef",
     "PutDataCatalogEncryptionSettingsRequestRequestTypeDef",
     "DatabaseInputTypeDef",
     "DatabaseTypeDef",
@@ -654,24 +600,18 @@
     "SecurityConfigurationTypeDef",
     "DeleteSchemaVersionsResponseTypeDef",
     "FilterTypeDef",
     "UpdateMLTransformRequestRequestTypeDef",
     "GetMLTransformsRequestRequestTypeDef",
     "ListMLTransformsRequestRequestTypeDef",
     "AthenaConnectorSourceTypeDef",
-    "CatalogDeltaSourceTypeDef",
-    "CatalogHudiSourceTypeDef",
     "CustomCodeTypeDef",
     "JDBCConnectorSourceTypeDef",
     "JDBCConnectorTargetTypeDef",
-    "S3CatalogDeltaSourceTypeDef",
-    "S3CatalogHudiSourceTypeDef",
     "S3CsvSourceTypeDef",
-    "S3DeltaSourceTypeDef",
-    "S3HudiSourceTypeDef",
     "S3JsonSourceTypeDef",
     "S3ParquetSourceTypeDef",
     "SparkConnectorSourceTypeDef",
     "SparkConnectorTargetTypeDef",
     "SparkSQLTypeDef",
     "GetJobRunResponseTypeDef",
     "GetJobRunsResponseTypeDef",
@@ -693,21 +633,14 @@
     "UpdateTriggerResponseTypeDef",
     "UpdateTriggerRequestRequestTypeDef",
     "GetMLTransformResponseTypeDef",
     "MLTransformTypeDef",
     "BatchGetCrawlersResponseTypeDef",
     "GetCrawlerResponseTypeDef",
     "GetCrawlersResponseTypeDef",
-    "ListDataQualityResultsResponseTypeDef",
-    "ListDataQualityResultsRequestRequestTypeDef",
-    "BatchGetDataQualityResultResponseTypeDef",
-    "ListDataQualityRuleRecommendationRunsResponseTypeDef",
-    "ListDataQualityRuleRecommendationRunsRequestRequestTypeDef",
-    "ListDataQualityRulesetEvaluationRunsResponseTypeDef",
-    "ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef",
     "CreateDatabaseRequestRequestTypeDef",
     "UpdateDatabaseRequestRequestTypeDef",
     "GetDatabaseResponseTypeDef",
     "GetDatabasesResponseTypeDef",
     "ColumnStatisticsTypeDef",
     "PartitionInputTypeDef",
     "PartitionTypeDef",
@@ -837,22 +770,20 @@
     "_OptionalBatchDeleteConnectionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class BatchDeleteConnectionRequestRequestTypeDef(
     _RequiredBatchDeleteConnectionRequestRequestTypeDef,
     _OptionalBatchDeleteConnectionRequestRequestTypeDef,
 ):
     pass
 
-
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
@@ -870,21 +801,19 @@
     {
         "CatalogId": str,
         "TransactionId": str,
     },
     total=False,
 )
 
-
 class BatchDeleteTableRequestRequestTypeDef(
     _RequiredBatchDeleteTableRequestRequestTypeDef, _OptionalBatchDeleteTableRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredBatchDeleteTableVersionRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDeleteTableVersionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "VersionIds": Sequence[str],
     },
@@ -893,22 +822,20 @@
     "_OptionalBatchDeleteTableVersionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class BatchDeleteTableVersionRequestRequestTypeDef(
     _RequiredBatchDeleteTableVersionRequestRequestTypeDef,
     _OptionalBatchDeleteTableVersionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredBatchGetBlueprintsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetBlueprintsRequestRequestTypeDef",
     {
         "Names": Sequence[str],
     },
 )
 _OptionalBatchGetBlueprintsRequestRequestTypeDef = TypedDict(
@@ -916,22 +843,20 @@
     {
         "IncludeBlueprint": bool,
         "IncludeParameterSpec": bool,
     },
     total=False,
 )
 
-
 class BatchGetBlueprintsRequestRequestTypeDef(
     _RequiredBatchGetBlueprintsRequestRequestTypeDef,
     _OptionalBatchGetBlueprintsRequestRequestTypeDef,
 ):
     pass
 
-
 BatchGetCrawlersRequestRequestTypeDef = TypedDict(
     "BatchGetCrawlersRequestRequestTypeDef",
     {
         "CrawlerNames": Sequence[str],
     },
 )
 
@@ -953,26 +878,17 @@
     "_OptionalCustomEntityTypeTypeDef",
     {
         "ContextWords": List[str],
     },
     total=False,
 )
 
-
 class CustomEntityTypeTypeDef(_RequiredCustomEntityTypeTypeDef, _OptionalCustomEntityTypeTypeDef):
     pass
 
-
-BatchGetDataQualityResultRequestRequestTypeDef = TypedDict(
-    "BatchGetDataQualityResultRequestRequestTypeDef",
-    {
-        "ResultIds": Sequence[str],
-    },
-)
-
 BatchGetDevEndpointsRequestRequestTypeDef = TypedDict(
     "BatchGetDevEndpointsRequestRequestTypeDef",
     {
         "DevEndpointNames": Sequence[str],
     },
 )
 
@@ -1032,21 +948,19 @@
     "_OptionalBatchGetWorkflowsRequestRequestTypeDef",
     {
         "IncludeGraph": bool,
     },
     total=False,
 )
 
-
 class BatchGetWorkflowsRequestRequestTypeDef(
     _RequiredBatchGetWorkflowsRequestRequestTypeDef, _OptionalBatchGetWorkflowsRequestRequestTypeDef
 ):
     pass
 
-
 BatchStopJobRunRequestRequestTypeDef = TypedDict(
     "BatchStopJobRunRequestRequestTypeDef",
     {
         "JobName": str,
         "JobRunIds": Sequence[str],
     },
 )
@@ -1112,28 +1026,14 @@
     {
         "NumberOfTrues": int,
         "NumberOfFalses": int,
         "NumberOfNulls": int,
     },
 )
 
-CancelDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
-    "CancelDataQualityRuleRecommendationRunRequestRequestTypeDef",
-    {
-        "RunId": str,
-    },
-)
-
-CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
-    "CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef",
-    {
-        "RunId": str,
-    },
-)
-
 CancelMLTaskRunRequestRequestTypeDef = TypedDict(
     "CancelMLTaskRunRequestRequestTypeDef",
     {
         "TransformId": str,
         "TaskRunId": str,
     },
 )
@@ -1149,21 +1049,19 @@
     "_OptionalCancelStatementRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
-
 class CancelStatementRequestRequestTypeDef(
     _RequiredCancelStatementRequestRequestTypeDef, _OptionalCancelStatementRequestRequestTypeDef
 ):
     pass
 
-
 CatalogEntryTypeDef = TypedDict(
     "CatalogEntryTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -1192,17 +1090,14 @@
         "StartingOffsets": str,
         "EndingOffsets": str,
         "PollTimeoutMs": int,
         "NumRetries": int,
         "RetryIntervalMs": int,
         "MaxOffsetsPerTrigger": int,
         "MinPartitions": int,
-        "IncludeHeaders": bool,
-        "AddRecordTimestamp": str,
-        "EmitConsumerLagMetrics": str,
     },
     total=False,
 )
 
 StreamingDataPreviewOptionsTypeDef = TypedDict(
     "StreamingDataPreviewOptionsTypeDef",
     {
@@ -1229,16 +1124,14 @@
         "NumRetries": int,
         "RetryIntervalMs": int,
         "MaxRetryIntervalMs": int,
         "AvoidEmptyBatches": bool,
         "StreamArn": str,
         "RoleArn": str,
         "RoleSessionName": str,
-        "AddRecordTimestamp": str,
-        "EmitConsumerLagMetrics": str,
     },
     total=False,
 )
 
 CatalogSchemaChangePolicyTypeDef = TypedDict(
     "CatalogSchemaChangePolicyTypeDef",
     {
@@ -1270,19 +1163,17 @@
         "ConnectionName": str,
         "EventQueueArn": str,
         "DlqEventQueueArn": str,
     },
     total=False,
 )
 
-
 class CatalogTargetTypeDef(_RequiredCatalogTargetTypeDef, _OptionalCatalogTargetTypeDef):
     pass
 
-
 CheckSchemaVersionValidityInputRequestTypeDef = TypedDict(
     "CheckSchemaVersionValidityInputRequestTypeDef",
     {
         "DataFormat": DataFormatType,
         "SchemaDefinition": str,
     },
 )
@@ -1307,19 +1198,17 @@
         "AllowSingleColumn": bool,
         "CustomDatatypeConfigured": bool,
         "CustomDatatypes": List[str],
     },
     total=False,
 )
 
-
 class CsvClassifierTypeDef(_RequiredCsvClassifierTypeDef, _OptionalCsvClassifierTypeDef):
     pass
 
-
 _RequiredGrokClassifierTypeDef = TypedDict(
     "_RequiredGrokClassifierTypeDef",
     {
         "Name": str,
         "Classification": str,
         "GrokPattern": str,
     },
@@ -1331,19 +1220,17 @@
         "LastUpdated": datetime,
         "Version": int,
         "CustomPatterns": str,
     },
     total=False,
 )
 
-
 class GrokClassifierTypeDef(_RequiredGrokClassifierTypeDef, _OptionalGrokClassifierTypeDef):
     pass
 
-
 _RequiredJsonClassifierTypeDef = TypedDict(
     "_RequiredJsonClassifierTypeDef",
     {
         "Name": str,
         "JsonPath": str,
     },
 )
@@ -1353,19 +1240,17 @@
         "CreationTime": datetime,
         "LastUpdated": datetime,
         "Version": int,
     },
     total=False,
 )
 
-
 class JsonClassifierTypeDef(_RequiredJsonClassifierTypeDef, _OptionalJsonClassifierTypeDef):
     pass
 
-
 _RequiredXMLClassifierTypeDef = TypedDict(
     "_RequiredXMLClassifierTypeDef",
     {
         "Name": str,
         "Classification": str,
     },
 )
@@ -1376,51 +1261,26 @@
         "LastUpdated": datetime,
         "Version": int,
         "RowTag": str,
     },
     total=False,
 )
 
-
 class XMLClassifierTypeDef(_RequiredXMLClassifierTypeDef, _OptionalXMLClassifierTypeDef):
     pass
 
-
 CloudWatchEncryptionTypeDef = TypedDict(
     "CloudWatchEncryptionTypeDef",
     {
         "CloudWatchEncryptionMode": CloudWatchEncryptionModeType,
         "KmsKeyArn": str,
     },
     total=False,
 )
 
-_RequiredDirectJDBCSourceTypeDef = TypedDict(
-    "_RequiredDirectJDBCSourceTypeDef",
-    {
-        "Name": str,
-        "Database": str,
-        "Table": str,
-        "ConnectionName": str,
-        "ConnectionType": JDBCConnectionTypeType,
-    },
-)
-_OptionalDirectJDBCSourceTypeDef = TypedDict(
-    "_OptionalDirectJDBCSourceTypeDef",
-    {
-        "RedshiftTmpDir": str,
-    },
-    total=False,
-)
-
-
-class DirectJDBCSourceTypeDef(_RequiredDirectJDBCSourceTypeDef, _OptionalDirectJDBCSourceTypeDef):
-    pass
-
-
 _RequiredDropDuplicatesTypeDef = TypedDict(
     "_RequiredDropDuplicatesTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
     },
 )
@@ -1428,19 +1288,17 @@
     "_OptionalDropDuplicatesTypeDef",
     {
         "Columns": List[List[str]],
     },
     total=False,
 )
 
-
 class DropDuplicatesTypeDef(_RequiredDropDuplicatesTypeDef, _OptionalDropDuplicatesTypeDef):
     pass
 
-
 DropFieldsTypeDef = TypedDict(
     "DropFieldsTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Paths": List[List[str]],
     },
@@ -1467,21 +1325,19 @@
     "_OptionalFillMissingValuesTypeDef",
     {
         "FilledPath": str,
     },
     total=False,
 )
 
-
 class FillMissingValuesTypeDef(
     _RequiredFillMissingValuesTypeDef, _OptionalFillMissingValuesTypeDef
 ):
     pass
 
-
 MergeTypeDef = TypedDict(
     "MergeTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Source": str,
         "PrimaryKeys": List[List[str]],
@@ -1561,19 +1417,17 @@
         "SampleFraction": float,
         "ThresholdFraction": float,
         "MaskValue": str,
     },
     total=False,
 )
 
-
 class PIIDetectionTypeDef(_RequiredPIIDetectionTypeDef, _OptionalPIIDetectionTypeDef):
     pass
 
-
 PostgreSQLCatalogSourceTypeDef = TypedDict(
     "PostgreSQLCatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -1602,19 +1456,17 @@
     {
         "RedshiftTmpDir": str,
         "TmpDirIAMRole": str,
     },
     total=False,
 )
 
-
 class RedshiftSourceTypeDef(_RequiredRedshiftSourceTypeDef, _OptionalRedshiftSourceTypeDef):
     pass
 
-
 RelationalCatalogSourceTypeDef = TypedDict(
     "RelationalCatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -1661,19 +1513,17 @@
     {
         "Topk": int,
         "Prob": float,
     },
     total=False,
 )
 
-
 class SpigotTypeDef(_RequiredSpigotTypeDef, _OptionalSpigotTypeDef):
     pass
 
-
 SplitFieldsTypeDef = TypedDict(
     "SplitFieldsTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Paths": List[List[str]],
     },
@@ -1699,19 +1549,17 @@
     "_OptionalCodeGenEdgeTypeDef",
     {
         "TargetParameter": str,
     },
     total=False,
 )
 
-
 class CodeGenEdgeTypeDef(_RequiredCodeGenEdgeTypeDef, _OptionalCodeGenEdgeTypeDef):
     pass
 
-
 _RequiredCodeGenNodeArgTypeDef = TypedDict(
     "_RequiredCodeGenNodeArgTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -1719,19 +1567,17 @@
     "_OptionalCodeGenNodeArgTypeDef",
     {
         "Param": bool,
     },
     total=False,
 )
 
-
 class CodeGenNodeArgTypeDef(_RequiredCodeGenNodeArgTypeDef, _OptionalCodeGenNodeArgTypeDef):
     pass
 
-
 ColumnImportanceTypeDef = TypedDict(
     "ColumnImportanceTypeDef",
     {
         "ColumnName": str,
         "Importance": float,
     },
     total=False,
@@ -1758,21 +1604,19 @@
     {
         "MinimumValue": datetime,
         "MaximumValue": datetime,
     },
     total=False,
 )
 
-
 class DateColumnStatisticsDataTypeDef(
     _RequiredDateColumnStatisticsDataTypeDef, _OptionalDateColumnStatisticsDataTypeDef
 ):
     pass
 
-
 _RequiredDoubleColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredDoubleColumnStatisticsDataTypeDef",
     {
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
     },
 )
@@ -1781,21 +1625,19 @@
     {
         "MinimumValue": float,
         "MaximumValue": float,
     },
     total=False,
 )
 
-
 class DoubleColumnStatisticsDataTypeDef(
     _RequiredDoubleColumnStatisticsDataTypeDef, _OptionalDoubleColumnStatisticsDataTypeDef
 ):
     pass
 
-
 _RequiredLongColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredLongColumnStatisticsDataTypeDef",
     {
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
     },
 )
@@ -1804,21 +1646,19 @@
     {
         "MinimumValue": int,
         "MaximumValue": int,
     },
     total=False,
 )
 
-
 class LongColumnStatisticsDataTypeDef(
     _RequiredLongColumnStatisticsDataTypeDef, _OptionalLongColumnStatisticsDataTypeDef
 ):
     pass
 
-
 StringColumnStatisticsDataTypeDef = TypedDict(
     "StringColumnStatisticsDataTypeDef",
     {
         "MaximumLength": int,
         "AverageLength": float,
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
@@ -1837,19 +1677,17 @@
         "Type": str,
         "Comment": str,
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
-
 class ColumnTypeDef(_RequiredColumnTypeDef, _OptionalColumnTypeDef):
     pass
 
-
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "LogicalOperator": Literal["EQUALS"],
         "JobName": str,
         "State": JobRunStateType,
         "CrawlerName": str,
@@ -1889,21 +1727,19 @@
     "_OptionalConnectionPasswordEncryptionTypeDef",
     {
         "AwsKmsKeyId": str,
     },
     total=False,
 )
 
-
 class ConnectionPasswordEncryptionTypeDef(
     _RequiredConnectionPasswordEncryptionTypeDef, _OptionalConnectionPasswordEncryptionTypeDef
 ):
     pass
 
-
 ConnectionsListTypeDef = TypedDict(
     "ConnectionsListTypeDef",
     {
         "Connections": List[str],
     },
     total=False,
 )
@@ -1955,15 +1791,14 @@
 
 DeltaTargetTypeDef = TypedDict(
     "DeltaTargetTypeDef",
     {
         "DeltaTables": List[str],
         "ConnectionName": str,
         "WriteManifest": bool,
-        "CreateNativeDeltaTable": bool,
     },
     total=False,
 )
 
 DynamoDBTargetTypeDef = TypedDict(
     "DynamoDBTargetTypeDef",
     {
@@ -1976,15 +1811,14 @@
 
 JdbcTargetTypeDef = TypedDict(
     "JdbcTargetTypeDef",
     {
         "ConnectionName": str,
         "Path": str,
         "Exclusions": List[str],
-        "EnableAdditionalMetadata": List[JdbcMetadataEntryType],
     },
     total=False,
 )
 
 MongoDBTargetTypeDef = TypedDict(
     "MongoDBTargetTypeDef",
     {
@@ -2086,21 +1920,19 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateBlueprintRequestRequestTypeDef(
     _RequiredCreateBlueprintRequestRequestTypeDef, _OptionalCreateBlueprintRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateCsvClassifierRequestTypeDef = TypedDict(
     "_RequiredCreateCsvClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateCsvClassifierRequestTypeDef = TypedDict(
@@ -2114,21 +1946,19 @@
         "AllowSingleColumn": bool,
         "CustomDatatypeConfigured": bool,
         "CustomDatatypes": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateCsvClassifierRequestTypeDef(
     _RequiredCreateCsvClassifierRequestTypeDef, _OptionalCreateCsvClassifierRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateGrokClassifierRequestTypeDef = TypedDict(
     "_RequiredCreateGrokClassifierRequestTypeDef",
     {
         "Classification": str,
         "Name": str,
         "GrokPattern": str,
     },
@@ -2137,21 +1967,19 @@
     "_OptionalCreateGrokClassifierRequestTypeDef",
     {
         "CustomPatterns": str,
     },
     total=False,
 )
 
-
 class CreateGrokClassifierRequestTypeDef(
     _RequiredCreateGrokClassifierRequestTypeDef, _OptionalCreateGrokClassifierRequestTypeDef
 ):
     pass
 
-
 CreateJsonClassifierRequestTypeDef = TypedDict(
     "CreateJsonClassifierRequestTypeDef",
     {
         "Name": str,
         "JsonPath": str,
     },
 )
@@ -2167,21 +1995,19 @@
     "_OptionalCreateXMLClassifierRequestTypeDef",
     {
         "RowTag": str,
     },
     total=False,
 )
 
-
 class CreateXMLClassifierRequestTypeDef(
     _RequiredCreateXMLClassifierRequestTypeDef, _OptionalCreateXMLClassifierRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateCustomEntityTypeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCustomEntityTypeRequestRequestTypeDef",
     {
         "Name": str,
         "RegexString": str,
     },
 )
@@ -2189,30 +2015,20 @@
     "_OptionalCreateCustomEntityTypeRequestRequestTypeDef",
     {
         "ContextWords": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateCustomEntityTypeRequestRequestTypeDef(
     _RequiredCreateCustomEntityTypeRequestRequestTypeDef,
     _OptionalCreateCustomEntityTypeRequestRequestTypeDef,
 ):
     pass
 
-
-DataQualityTargetTableTypeDef = TypedDict(
-    "DataQualityTargetTableTypeDef",
-    {
-        "TableName": str,
-        "DatabaseName": str,
-    },
-)
-
 _RequiredCreateDevEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDevEndpointRequestRequestTypeDef",
     {
         "EndpointName": str,
         "RoleArn": str,
     },
 )
@@ -2232,21 +2048,19 @@
         "SecurityConfiguration": str,
         "Tags": Mapping[str, str],
         "Arguments": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateDevEndpointRequestRequestTypeDef(
     _RequiredCreateDevEndpointRequestRequestTypeDef, _OptionalCreateDevEndpointRequestRequestTypeDef
 ):
     pass
 
-
 ExecutionPropertyTypeDef = TypedDict(
     "ExecutionPropertyTypeDef",
     {
         "MaxConcurrentRuns": int,
     },
     total=False,
 )
@@ -2284,24 +2098,21 @@
     },
 )
 _OptionalGlueTableTypeDef = TypedDict(
     "_OptionalGlueTableTypeDef",
     {
         "CatalogId": str,
         "ConnectionName": str,
-        "AdditionalOptions": Dict[str, str],
     },
     total=False,
 )
 
-
 class GlueTableTypeDef(_RequiredGlueTableTypeDef, _OptionalGlueTableTypeDef):
     pass
 
-
 PartitionIndexTypeDef = TypedDict(
     "PartitionIndexTypeDef",
     {
         "Keys": Sequence[str],
         "IndexName": str,
     },
 )
@@ -2317,21 +2128,19 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateRegistryInputRequestTypeDef(
     _RequiredCreateRegistryInputRequestTypeDef, _OptionalCreateRegistryInputRequestTypeDef
 ):
     pass
 
-
 RegistryIdTypeDef = TypedDict(
     "RegistryIdTypeDef",
     {
         "RegistryName": str,
         "RegistryArn": str,
     },
     total=False,
@@ -2356,21 +2165,19 @@
     "_OptionalEventBatchingConditionTypeDef",
     {
         "BatchWindow": int,
     },
     total=False,
 )
 
-
 class EventBatchingConditionTypeDef(
     _RequiredEventBatchingConditionTypeDef, _OptionalEventBatchingConditionTypeDef
 ):
     pass
 
-
 _RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
@@ -2380,87 +2187,44 @@
         "DefaultRunProperties": Mapping[str, str],
         "Tags": Mapping[str, str],
         "MaxConcurrentRuns": int,
     },
     total=False,
 )
 
-
 class CreateWorkflowRequestRequestTypeDef(
     _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
 ):
     pass
 
-
-DQResultsPublishingOptionsTypeDef = TypedDict(
-    "DQResultsPublishingOptionsTypeDef",
-    {
-        "EvaluationContext": str,
-        "ResultsS3Prefix": str,
-        "CloudWatchMetricsEnabled": bool,
-        "ResultsPublishingEnabled": bool,
-    },
-    total=False,
-)
-
-DQStopJobOnFailureOptionsTypeDef = TypedDict(
-    "DQStopJobOnFailureOptionsTypeDef",
-    {
-        "StopJobOnFailureTiming": DQStopJobOnFailureTimingType,
-    },
-    total=False,
-)
-
 _RequiredEncryptionAtRestTypeDef = TypedDict(
     "_RequiredEncryptionAtRestTypeDef",
     {
         "CatalogEncryptionMode": CatalogEncryptionModeType,
     },
 )
 _OptionalEncryptionAtRestTypeDef = TypedDict(
     "_OptionalEncryptionAtRestTypeDef",
     {
         "SseAwsKmsKeyId": str,
     },
     total=False,
 )
 
-
 class EncryptionAtRestTypeDef(_RequiredEncryptionAtRestTypeDef, _OptionalEncryptionAtRestTypeDef):
     pass
 
-
 DataLakePrincipalTypeDef = TypedDict(
     "DataLakePrincipalTypeDef",
     {
         "DataLakePrincipalIdentifier": str,
     },
     total=False,
 )
 
-DataQualityEvaluationRunAdditionalRunOptionsTypeDef = TypedDict(
-    "DataQualityEvaluationRunAdditionalRunOptionsTypeDef",
-    {
-        "CloudWatchMetricsEnabled": bool,
-        "ResultsS3Prefix": str,
-    },
-    total=False,
-)
-
-DataQualityRuleResultTypeDef = TypedDict(
-    "DataQualityRuleResultTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "EvaluationMessage": str,
-        "Result": DataQualityRuleResultStatusType,
-    },
-    total=False,
-)
-
 DatabaseIdentifierTypeDef = TypedDict(
     "DatabaseIdentifierTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
     },
     total=False,
@@ -2509,22 +2273,20 @@
     "_OptionalDeleteColumnStatisticsForPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeleteColumnStatisticsForPartitionRequestRequestTypeDef(
     _RequiredDeleteColumnStatisticsForPartitionRequestRequestTypeDef,
     _OptionalDeleteColumnStatisticsForPartitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteColumnStatisticsForTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "ColumnName": str,
     },
@@ -2533,85 +2295,72 @@
     "_OptionalDeleteColumnStatisticsForTableRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeleteColumnStatisticsForTableRequestRequestTypeDef(
     _RequiredDeleteColumnStatisticsForTableRequestRequestTypeDef,
     _OptionalDeleteColumnStatisticsForTableRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteConnectionRequestRequestTypeDef",
     {
         "ConnectionName": str,
     },
 )
 _OptionalDeleteConnectionRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteConnectionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeleteConnectionRequestRequestTypeDef(
     _RequiredDeleteConnectionRequestRequestTypeDef, _OptionalDeleteConnectionRequestRequestTypeDef
 ):
     pass
 
-
 DeleteCrawlerRequestRequestTypeDef = TypedDict(
     "DeleteCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
 DeleteCustomEntityTypeRequestRequestTypeDef = TypedDict(
     "DeleteCustomEntityTypeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DeleteDataQualityRulesetRequestRequestTypeDef = TypedDict(
-    "DeleteDataQualityRulesetRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 _RequiredDeleteDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDatabaseRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDeleteDatabaseRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteDatabaseRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeleteDatabaseRequestRequestTypeDef(
     _RequiredDeleteDatabaseRequestRequestTypeDef, _OptionalDeleteDatabaseRequestRequestTypeDef
 ):
     pass
 
-
 DeleteDevEndpointRequestRequestTypeDef = TypedDict(
     "DeleteDevEndpointRequestRequestTypeDef",
     {
         "EndpointName": str,
     },
 )
 
@@ -2641,22 +2390,20 @@
     "_OptionalDeletePartitionIndexRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeletePartitionIndexRequestRequestTypeDef(
     _RequiredDeletePartitionIndexRequestRequestTypeDef,
     _OptionalDeletePartitionIndexRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeletePartitionRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionValues": Sequence[str],
     },
@@ -2665,21 +2412,19 @@
     "_OptionalDeletePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeletePartitionRequestRequestTypeDef(
     _RequiredDeletePartitionRequestRequestTypeDef, _OptionalDeletePartitionRequestRequestTypeDef
 ):
     pass
 
-
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "PolicyHashCondition": str,
         "ResourceArn": str,
     },
     total=False,
@@ -2712,21 +2457,19 @@
     "_OptionalDeleteSessionRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
-
 class DeleteSessionRequestRequestTypeDef(
     _RequiredDeleteSessionRequestRequestTypeDef, _OptionalDeleteSessionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteTableRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -2735,21 +2478,19 @@
     {
         "CatalogId": str,
         "TransactionId": str,
     },
     total=False,
 )
 
-
 class DeleteTableRequestRequestTypeDef(
     _RequiredDeleteTableRequestRequestTypeDef, _OptionalDeleteTableRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteTableVersionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTableVersionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "VersionId": str,
     },
@@ -2758,22 +2499,20 @@
     "_OptionalDeleteTableVersionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeleteTableVersionRequestRequestTypeDef(
     _RequiredDeleteTableVersionRequestRequestTypeDef,
     _OptionalDeleteTableVersionRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteTriggerRequestRequestTypeDef = TypedDict(
     "DeleteTriggerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -2788,22 +2527,20 @@
     "_OptionalDeleteUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DeleteUserDefinedFunctionRequestRequestTypeDef(
     _RequiredDeleteUserDefinedFunctionRequestRequestTypeDef,
     _OptionalDeleteUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -2833,40 +2570,14 @@
         "IsEmpty": bool,
         "IsNullString": bool,
         "IsNegOne": bool,
     },
     total=False,
 )
 
-_RequiredTransformConfigParameterTypeDef = TypedDict(
-    "_RequiredTransformConfigParameterTypeDef",
-    {
-        "Name": str,
-        "Type": ParamTypeType,
-    },
-)
-_OptionalTransformConfigParameterTypeDef = TypedDict(
-    "_OptionalTransformConfigParameterTypeDef",
-    {
-        "ValidationRule": str,
-        "ValidationMessage": str,
-        "Value": List[str],
-        "ListType": ParamTypeType,
-        "IsOptional": bool,
-    },
-    total=False,
-)
-
-
-class TransformConfigParameterTypeDef(
-    _RequiredTransformConfigParameterTypeDef, _OptionalTransformConfigParameterTypeDef
-):
-    pass
-
-
 EdgeTypeDef = TypedDict(
     "EdgeTypeDef",
     {
         "SourceId": str,
         "DestinationId": str,
     },
     total=False,
@@ -2947,21 +2658,19 @@
     {
         "IncludeBlueprint": bool,
         "IncludeParameterSpec": bool,
     },
     total=False,
 )
 
-
 class GetBlueprintRequestRequestTypeDef(
     _RequiredGetBlueprintRequestRequestTypeDef, _OptionalGetBlueprintRequestRequestTypeDef
 ):
     pass
 
-
 GetBlueprintRunRequestRequestTypeDef = TypedDict(
     "GetBlueprintRunRequestRequestTypeDef",
     {
         "BlueprintName": str,
         "RunId": str,
     },
 )
@@ -2977,21 +2686,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetBlueprintRunsRequestRequestTypeDef(
     _RequiredGetBlueprintRunsRequestRequestTypeDef, _OptionalGetBlueprintRunsRequestRequestTypeDef
 ):
     pass
 
-
 GetCatalogImportStatusRequestRequestTypeDef = TypedDict(
     "GetCatalogImportStatusRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
@@ -3035,22 +2742,20 @@
     "_OptionalGetColumnStatisticsForPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class GetColumnStatisticsForPartitionRequestRequestTypeDef(
     _RequiredGetColumnStatisticsForPartitionRequestRequestTypeDef,
     _OptionalGetColumnStatisticsForPartitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
     "_RequiredGetColumnStatisticsForTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "ColumnNames": Sequence[str],
     },
@@ -3059,22 +2764,20 @@
     "_OptionalGetColumnStatisticsForTableRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class GetColumnStatisticsForTableRequestRequestTypeDef(
     _RequiredGetColumnStatisticsForTableRequestRequestTypeDef,
     _OptionalGetColumnStatisticsForTableRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetConnectionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetConnectionRequestRequestTypeDef = TypedDict(
@@ -3082,21 +2785,19 @@
     {
         "CatalogId": str,
         "HidePassword": bool,
     },
     total=False,
 )
 
-
 class GetConnectionRequestRequestTypeDef(
     _RequiredGetConnectionRequestRequestTypeDef, _OptionalGetConnectionRequestRequestTypeDef
 ):
     pass
 
-
 GetConnectionsFilterTypeDef = TypedDict(
     "GetConnectionsFilterTypeDef",
     {
         "MatchCriteria": Sequence[str],
         "ConnectionType": ConnectionTypeType,
     },
     total=False,
@@ -3139,63 +2840,33 @@
     "GetDataCatalogEncryptionSettingsRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-GetDataQualityResultRequestRequestTypeDef = TypedDict(
-    "GetDataQualityResultRequestRequestTypeDef",
-    {
-        "ResultId": str,
-    },
-)
-
-GetDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
-    "GetDataQualityRuleRecommendationRunRequestRequestTypeDef",
-    {
-        "RunId": str,
-    },
-)
-
-GetDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
-    "GetDataQualityRulesetEvaluationRunRequestRequestTypeDef",
-    {
-        "RunId": str,
-    },
-)
-
-GetDataQualityRulesetRequestRequestTypeDef = TypedDict(
-    "GetDataQualityRulesetRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 _RequiredGetDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredGetDatabaseRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetDatabaseRequestRequestTypeDef = TypedDict(
     "_OptionalGetDatabaseRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class GetDatabaseRequestRequestTypeDef(
     _RequiredGetDatabaseRequestRequestTypeDef, _OptionalGetDatabaseRequestRequestTypeDef
 ):
     pass
 
-
 GetDatabasesRequestRequestTypeDef = TypedDict(
     "GetDatabasesRequestRequestTypeDef",
     {
         "CatalogId": str,
         "NextToken": str,
         "MaxResults": int,
         "ResourceShareType": ResourceShareTypeType,
@@ -3237,21 +2908,19 @@
     "_OptionalGetJobBookmarkRequestRequestTypeDef",
     {
         "RunId": str,
     },
     total=False,
 )
 
-
 class GetJobBookmarkRequestRequestTypeDef(
     _RequiredGetJobBookmarkRequestRequestTypeDef, _OptionalGetJobBookmarkRequestRequestTypeDef
 ):
     pass
 
-
 JobBookmarkEntryTypeDef = TypedDict(
     "JobBookmarkEntryTypeDef",
     {
         "JobName": str,
         "Version": int,
         "Run": int,
         "Attempt": int,
@@ -3280,21 +2949,19 @@
     "_OptionalGetJobRunRequestRequestTypeDef",
     {
         "PredecessorsIncluded": bool,
     },
     total=False,
 )
 
-
 class GetJobRunRequestRequestTypeDef(
     _RequiredGetJobRunRequestRequestTypeDef, _OptionalGetJobRunRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredGetJobRunsRequestRequestTypeDef",
     {
         "JobName": str,
     },
 )
 _OptionalGetJobRunsRequestRequestTypeDef = TypedDict(
@@ -3302,21 +2969,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetJobRunsRequestRequestTypeDef(
     _RequiredGetJobRunsRequestRequestTypeDef, _OptionalGetJobRunsRequestRequestTypeDef
 ):
     pass
 
-
 GetJobsRequestRequestTypeDef = TypedDict(
     "GetJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -3398,22 +3063,20 @@
     {
         "CatalogId": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetPartitionIndexesRequestRequestTypeDef(
     _RequiredGetPartitionIndexesRequestRequestTypeDef,
     _OptionalGetPartitionIndexesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetPartitionRequestRequestTypeDef = TypedDict(
     "_RequiredGetPartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionValues": Sequence[str],
     },
@@ -3422,21 +3085,19 @@
     "_OptionalGetPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class GetPartitionRequestRequestTypeDef(
     _RequiredGetPartitionRequestRequestTypeDef, _OptionalGetPartitionRequestRequestTypeDef
 ):
     pass
 
-
 SegmentTypeDef = TypedDict(
     "SegmentTypeDef",
     {
         "SegmentNumber": int,
         "TotalSegments": int,
     },
 )
@@ -3504,21 +3165,19 @@
     "_OptionalGetSessionRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
-
 class GetSessionRequestRequestTypeDef(
     _RequiredGetSessionRequestRequestTypeDef, _OptionalGetSessionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetStatementRequestRequestTypeDef = TypedDict(
     "_RequiredGetStatementRequestRequestTypeDef",
     {
         "SessionId": str,
         "Id": int,
     },
 )
@@ -3526,21 +3185,19 @@
     "_OptionalGetStatementRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
-
 class GetStatementRequestRequestTypeDef(
     _RequiredGetStatementRequestRequestTypeDef, _OptionalGetStatementRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetTableRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -3550,21 +3207,19 @@
         "CatalogId": str,
         "TransactionId": str,
         "QueryAsOfTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class GetTableRequestRequestTypeDef(
     _RequiredGetTableRequestRequestTypeDef, _OptionalGetTableRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetTableVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableVersionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -3573,21 +3228,19 @@
     {
         "CatalogId": str,
         "VersionId": str,
     },
     total=False,
 )
 
-
 class GetTableVersionRequestRequestTypeDef(
     _RequiredGetTableVersionRequestRequestTypeDef, _OptionalGetTableVersionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetTableVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableVersionsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -3597,21 +3250,19 @@
         "CatalogId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetTableVersionsRequestRequestTypeDef(
     _RequiredGetTableVersionsRequestRequestTypeDef, _OptionalGetTableVersionsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetTablesRequestRequestTypeDef = TypedDict(
     "_RequiredGetTablesRequestRequestTypeDef",
     {
         "DatabaseName": str,
     },
 )
 _OptionalGetTablesRequestRequestTypeDef = TypedDict(
@@ -3623,21 +3274,19 @@
         "MaxResults": int,
         "TransactionId": str,
         "QueryAsOfTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class GetTablesRequestRequestTypeDef(
     _RequiredGetTablesRequestRequestTypeDef, _OptionalGetTablesRequestRequestTypeDef
 ):
     pass
 
-
 GetTagsRequestRequestTypeDef = TypedDict(
     "GetTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -3669,22 +3318,20 @@
     "_OptionalGetUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class GetUserDefinedFunctionRequestRequestTypeDef(
     _RequiredGetUserDefinedFunctionRequestRequestTypeDef,
     _OptionalGetUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetUserDefinedFunctionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetUserDefinedFunctionsRequestRequestTypeDef",
     {
         "Pattern": str,
     },
 )
 _OptionalGetUserDefinedFunctionsRequestRequestTypeDef = TypedDict(
@@ -3694,43 +3341,39 @@
         "DatabaseName": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetUserDefinedFunctionsRequestRequestTypeDef(
     _RequiredGetUserDefinedFunctionsRequestRequestTypeDef,
     _OptionalGetUserDefinedFunctionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredGetWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetWorkflowRequestRequestTypeDef = TypedDict(
     "_OptionalGetWorkflowRequestRequestTypeDef",
     {
         "IncludeGraph": bool,
     },
     total=False,
 )
 
-
 class GetWorkflowRequestRequestTypeDef(
     _RequiredGetWorkflowRequestRequestTypeDef, _OptionalGetWorkflowRequestRequestTypeDef
 ):
     pass
 
-
 GetWorkflowRunPropertiesRequestRequestTypeDef = TypedDict(
     "GetWorkflowRunPropertiesRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
     },
 )
@@ -3746,21 +3389,19 @@
     "_OptionalGetWorkflowRunRequestRequestTypeDef",
     {
         "IncludeGraph": bool,
     },
     total=False,
 )
 
-
 class GetWorkflowRunRequestRequestTypeDef(
     _RequiredGetWorkflowRunRequestRequestTypeDef, _OptionalGetWorkflowRunRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetWorkflowRunsRequestRequestTypeDef = TypedDict(
     "_RequiredGetWorkflowRunsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetWorkflowRunsRequestRequestTypeDef = TypedDict(
@@ -3769,42 +3410,38 @@
         "IncludeGraph": bool,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetWorkflowRunsRequestRequestTypeDef(
     _RequiredGetWorkflowRunsRequestRequestTypeDef, _OptionalGetWorkflowRunsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGlueStudioSchemaColumnTypeDef = TypedDict(
     "_RequiredGlueStudioSchemaColumnTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGlueStudioSchemaColumnTypeDef = TypedDict(
     "_OptionalGlueStudioSchemaColumnTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-
 class GlueStudioSchemaColumnTypeDef(
     _RequiredGlueStudioSchemaColumnTypeDef, _OptionalGlueStudioSchemaColumnTypeDef
 ):
     pass
 
-
 S3SourceAdditionalOptionsTypeDef = TypedDict(
     "S3SourceAdditionalOptionsTypeDef",
     {
         "BoundedSize": int,
         "BoundedFiles": int,
     },
     total=False,
@@ -3994,21 +3631,19 @@
     {
         "RequestOrigin": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListStatementsRequestRequestTypeDef(
     _RequiredListStatementsRequestRequestTypeDef, _OptionalListStatementsRequestRequestTypeDef
 ):
     pass
 
-
 ListTriggersRequestRequestTypeDef = TypedDict(
     "ListTriggersRequestRequestTypeDef",
     {
         "NextToken": str,
         "DependentJobName": str,
         "MaxResults": int,
         "Tags": Mapping[str, str],
@@ -4035,21 +3670,19 @@
     "_OptionalMLUserDataEncryptionTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
-
 class MLUserDataEncryptionTypeDef(
     _RequiredMLUserDataEncryptionTypeDef, _OptionalMLUserDataEncryptionTypeDef
 ):
     pass
 
-
 MappingTypeDef = TypedDict(
     "MappingTypeDef",
     {
         "ToKey": str,
         "FromPath": List[str],
         "FromType": str,
         "ToType": str,
@@ -4108,21 +3741,19 @@
         "PolicyHashCondition": str,
         "PolicyExistsCondition": ExistConditionType,
         "EnableHybrid": EnableHybridValuesType,
     },
     total=False,
 )
 
-
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-
 PutWorkflowRunPropertiesRequestRequestTypeDef = TypedDict(
     "PutWorkflowRunPropertiesRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
         "RunProperties": Mapping[str, str],
     },
@@ -4148,21 +3779,19 @@
     "_OptionalResetJobBookmarkRequestRequestTypeDef",
     {
         "RunId": str,
     },
     total=False,
 )
 
-
 class ResetJobBookmarkRequestRequestTypeDef(
     _RequiredResetJobBookmarkRequestRequestTypeDef, _OptionalResetJobBookmarkRequestRequestTypeDef
 ):
     pass
 
-
 ResourceUriTypeDef = TypedDict(
     "ResourceUriTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "Uri": str,
     },
     total=False,
@@ -4188,21 +3817,19 @@
     "_OptionalRunStatementRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
-
 class RunStatementRequestRequestTypeDef(
     _RequiredRunStatementRequestRequestTypeDef, _OptionalRunStatementRequestRequestTypeDef
 ):
     pass
 
-
 S3DirectSourceAdditionalOptionsTypeDef = TypedDict(
     "S3DirectSourceAdditionalOptionsTypeDef",
     {
         "BoundedSize": int,
         "BoundedFiles": int,
         "EnableSamplePath": bool,
         "SamplePath": str,
@@ -4258,21 +3885,19 @@
     "_OptionalStartBlueprintRunRequestRequestTypeDef",
     {
         "Parameters": str,
     },
     total=False,
 )
 
-
 class StartBlueprintRunRequestRequestTypeDef(
     _RequiredStartBlueprintRunRequestRequestTypeDef, _OptionalStartBlueprintRunRequestRequestTypeDef
 ):
     pass
 
-
 StartCrawlerRequestRequestTypeDef = TypedDict(
     "StartCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -4302,22 +3927,20 @@
     "_OptionalStartImportLabelsTaskRunRequestRequestTypeDef",
     {
         "ReplaceAllLabels": bool,
     },
     total=False,
 )
 
-
 class StartImportLabelsTaskRunRequestRequestTypeDef(
     _RequiredStartImportLabelsTaskRunRequestRequestTypeDef,
     _OptionalStartImportLabelsTaskRunRequestRequestTypeDef,
 ):
     pass
 
-
 StartMLEvaluationTaskRunRequestRequestTypeDef = TypedDict(
     "StartMLEvaluationTaskRunRequestRequestTypeDef",
     {
         "TransformId": str,
     },
 )
 
@@ -4346,21 +3969,19 @@
     "_OptionalStartWorkflowRunRequestRequestTypeDef",
     {
         "RunProperties": Mapping[str, str],
     },
     total=False,
 )
 
-
 class StartWorkflowRunRequestRequestTypeDef(
     _RequiredStartWorkflowRunRequestRequestTypeDef, _OptionalStartWorkflowRunRequestRequestTypeDef
 ):
     pass
 
-
 StartingEventBatchConditionTypeDef = TypedDict(
     "StartingEventBatchConditionTypeDef",
     {
         "BatchSize": int,
         "BatchWindow": int,
     },
     total=False,
@@ -4398,21 +4019,19 @@
     "_OptionalStopSessionRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
-
 class StopSessionRequestRequestTypeDef(
     _RequiredStopSessionRequestRequestTypeDef, _OptionalStopSessionRequestRequestTypeDef
 ):
     pass
 
-
 StopTriggerRequestRequestTypeDef = TypedDict(
     "StopTriggerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -4461,21 +4080,19 @@
     "_OptionalUpdateBlueprintRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateBlueprintRequestRequestTypeDef(
     _RequiredUpdateBlueprintRequestRequestTypeDef, _OptionalUpdateBlueprintRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateCsvClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateCsvClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateCsvClassifierRequestTypeDef = TypedDict(
@@ -4489,21 +4106,19 @@
         "AllowSingleColumn": bool,
         "CustomDatatypeConfigured": bool,
         "CustomDatatypes": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateCsvClassifierRequestTypeDef(
     _RequiredUpdateCsvClassifierRequestTypeDef, _OptionalUpdateCsvClassifierRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateGrokClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateGrokClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateGrokClassifierRequestTypeDef = TypedDict(
@@ -4512,42 +4127,38 @@
         "Classification": str,
         "GrokPattern": str,
         "CustomPatterns": str,
     },
     total=False,
 )
 
-
 class UpdateGrokClassifierRequestTypeDef(
     _RequiredUpdateGrokClassifierRequestTypeDef, _OptionalUpdateGrokClassifierRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateJsonClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateJsonClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateJsonClassifierRequestTypeDef = TypedDict(
     "_OptionalUpdateJsonClassifierRequestTypeDef",
     {
         "JsonPath": str,
     },
     total=False,
 )
 
-
 class UpdateJsonClassifierRequestTypeDef(
     _RequiredUpdateJsonClassifierRequestTypeDef, _OptionalUpdateJsonClassifierRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateXMLClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateXMLClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateXMLClassifierRequestTypeDef = TypedDict(
@@ -4555,67 +4166,39 @@
     {
         "Classification": str,
         "RowTag": str,
     },
     total=False,
 )
 
-
 class UpdateXMLClassifierRequestTypeDef(
     _RequiredUpdateXMLClassifierRequestTypeDef, _OptionalUpdateXMLClassifierRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateCrawlerScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCrawlerScheduleRequestRequestTypeDef",
     {
         "CrawlerName": str,
     },
 )
 _OptionalUpdateCrawlerScheduleRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateCrawlerScheduleRequestRequestTypeDef",
     {
         "Schedule": str,
     },
     total=False,
 )
 
-
 class UpdateCrawlerScheduleRequestRequestTypeDef(
     _RequiredUpdateCrawlerScheduleRequestRequestTypeDef,
     _OptionalUpdateCrawlerScheduleRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredUpdateDataQualityRulesetRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDataQualityRulesetRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateDataQualityRulesetRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDataQualityRulesetRequestRequestTypeDef",
-    {
-        "UpdatedName": str,
-        "Description": str,
-        "Ruleset": str,
-    },
-    total=False,
-)
-
-
-class UpdateDataQualityRulesetRequestRequestTypeDef(
-    _RequiredUpdateDataQualityRulesetRequestRequestTypeDef,
-    _OptionalUpdateDataQualityRulesetRequestRequestTypeDef,
-):
-    pass
-
-
 UpdateJobFromSourceControlRequestRequestTypeDef = TypedDict(
     "UpdateJobFromSourceControlRequestRequestTypeDef",
     {
         "JobName": str,
         "Provider": SourceControlProviderType,
         "RepositoryName": str,
         "RepositoryOwner": str,
@@ -4656,21 +4239,19 @@
         "Description": str,
         "DefaultRunProperties": Mapping[str, str],
         "MaxConcurrentRuns": int,
     },
     total=False,
 )
 
-
 class UpdateWorkflowRequestRequestTypeDef(
     _RequiredUpdateWorkflowRequestRequestTypeDef, _OptionalUpdateWorkflowRequestRequestTypeDef
 ):
     pass
 
-
 WorkflowRunStatisticsTypeDef = TypedDict(
     "WorkflowRunStatisticsTypeDef",
     {
         "TotalActions": int,
         "TimeoutActions": int,
         "FailedActions": int,
         "StoppedActions": int,
@@ -4714,21 +4295,19 @@
         "WorkerType": WorkerTypeType,
         "NumberOfWorkers": int,
         "ExecutionClass": ExecutionClassType,
     },
     total=False,
 )
 
-
 class StartJobRunRequestRequestTypeDef(
     _RequiredStartJobRunRequestRequestTypeDef, _OptionalStartJobRunRequestRequestTypeDef
 ):
     pass
 
-
 AggregateTypeDef = TypedDict(
     "AggregateTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Groups": List[List[str]],
         "Aggs": List[AggregateOperationTypeDef],
@@ -4749,22 +4328,20 @@
     "_OptionalGetUnfilteredPartitionMetadataRequestRequestTypeDef",
     {
         "AuditContext": AuditContextTypeDef,
     },
     total=False,
 )
 
-
 class GetUnfilteredPartitionMetadataRequestRequestTypeDef(
     _RequiredGetUnfilteredPartitionMetadataRequestRequestTypeDef,
     _OptionalGetUnfilteredPartitionMetadataRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetUnfilteredTableMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetUnfilteredTableMetadataRequestRequestTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "Name": str,
         "SupportedPermissionTypes": Sequence[PermissionTypeType],
@@ -4774,22 +4351,20 @@
     "_OptionalGetUnfilteredTableMetadataRequestRequestTypeDef",
     {
         "AuditContext": AuditContextTypeDef,
     },
     total=False,
 )
 
-
 class GetUnfilteredTableMetadataRequestRequestTypeDef(
     _RequiredGetUnfilteredTableMetadataRequestRequestTypeDef,
     _OptionalGetUnfilteredTableMetadataRequestRequestTypeDef,
 ):
     pass
 
-
 BackfillErrorTypeDef = TypedDict(
     "BackfillErrorTypeDef",
     {
         "Code": BackfillErrorCodeType,
         "Partitions": List[PartitionValueListTypeDef],
     },
     total=False,
@@ -4807,22 +4382,20 @@
     "_OptionalBatchDeletePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class BatchDeletePartitionRequestRequestTypeDef(
     _RequiredBatchDeletePartitionRequestRequestTypeDef,
     _OptionalBatchDeletePartitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredBatchGetPartitionRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetPartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionsToGet": Sequence[PartitionValueListTypeDef],
     },
@@ -4831,21 +4404,19 @@
     "_OptionalBatchGetPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class BatchGetPartitionRequestRequestTypeDef(
     _RequiredBatchGetPartitionRequestRequestTypeDef, _OptionalBatchGetPartitionRequestRequestTypeDef
 ):
     pass
 
-
 CancelMLTaskRunResponseTypeDef = TypedDict(
     "CancelMLTaskRunResponseTypeDef",
     {
         "TransformId": str,
         "TaskRunId": str,
         "Status": TaskStatusTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -4873,22 +4444,14 @@
     "CreateCustomEntityTypeResponseTypeDef",
     {
         "Name": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateDataQualityRulesetResponseTypeDef = TypedDict(
-    "CreateDataQualityRulesetResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateDevEndpointResponseTypeDef = TypedDict(
     "CreateDevEndpointResponseTypeDef",
     {
         "EndpointName": str,
         "Status": str,
         "SecurityGroupIds": List[str],
         "SubnetId": str,
@@ -5314,30 +4877,14 @@
     "StartBlueprintRunResponseTypeDef",
     {
         "RunId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartDataQualityRuleRecommendationRunResponseTypeDef = TypedDict(
-    "StartDataQualityRuleRecommendationRunResponseTypeDef",
-    {
-        "RunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartDataQualityRulesetEvaluationRunResponseTypeDef = TypedDict(
-    "StartDataQualityRulesetEvaluationRunResponseTypeDef",
-    {
-        "RunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 StartExportLabelsTaskRunResponseTypeDef = TypedDict(
     "StartExportLabelsTaskRunResponseTypeDef",
     {
         "TaskRunId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5410,24 +4957,14 @@
     "UpdateBlueprintResponseTypeDef",
     {
         "Name": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateDataQualityRulesetResponseTypeDef = TypedDict(
-    "UpdateDataQualityRulesetResponseTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "Ruleset": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateJobFromSourceControlResponseTypeDef = TypedDict(
     "UpdateJobFromSourceControlResponseTypeDef",
     {
         "JobName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5649,21 +5186,19 @@
         "DetectSchema": bool,
         "StreamingOptions": KafkaStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
-
 class CatalogKafkaSourceTypeDef(
     _RequiredCatalogKafkaSourceTypeDef, _OptionalCatalogKafkaSourceTypeDef
 ):
     pass
 
-
 _RequiredDirectKafkaSourceTypeDef = TypedDict(
     "_RequiredDirectKafkaSourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDirectKafkaSourceTypeDef = TypedDict(
@@ -5673,21 +5208,19 @@
         "WindowSize": int,
         "DetectSchema": bool,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
-
 class DirectKafkaSourceTypeDef(
     _RequiredDirectKafkaSourceTypeDef, _OptionalDirectKafkaSourceTypeDef
 ):
     pass
 
-
 _RequiredCatalogKinesisSourceTypeDef = TypedDict(
     "_RequiredCatalogKinesisSourceTypeDef",
     {
         "Name": str,
         "Table": str,
         "Database": str,
     },
@@ -5699,21 +5232,19 @@
         "DetectSchema": bool,
         "StreamingOptions": KinesisStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
-
 class CatalogKinesisSourceTypeDef(
     _RequiredCatalogKinesisSourceTypeDef, _OptionalCatalogKinesisSourceTypeDef
 ):
     pass
 
-
 _RequiredDirectKinesisSourceTypeDef = TypedDict(
     "_RequiredDirectKinesisSourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDirectKinesisSourceTypeDef = TypedDict(
@@ -5723,21 +5254,19 @@
         "DetectSchema": bool,
         "StreamingOptions": KinesisStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
-
 class DirectKinesisSourceTypeDef(
     _RequiredDirectKinesisSourceTypeDef, _OptionalDirectKinesisSourceTypeDef
 ):
     pass
 
-
 _RequiredGovernedCatalogTargetTypeDef = TypedDict(
     "_RequiredGovernedCatalogTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Table": str,
         "Database": str,
@@ -5748,21 +5277,19 @@
     {
         "PartitionKeys": List[List[str]],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
-
 class GovernedCatalogTargetTypeDef(
     _RequiredGovernedCatalogTargetTypeDef, _OptionalGovernedCatalogTargetTypeDef
 ):
     pass
 
-
 _RequiredS3CatalogTargetTypeDef = TypedDict(
     "_RequiredS3CatalogTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Table": str,
         "Database": str,
@@ -5773,71 +5300,17 @@
     {
         "PartitionKeys": List[List[str]],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
-
 class S3CatalogTargetTypeDef(_RequiredS3CatalogTargetTypeDef, _OptionalS3CatalogTargetTypeDef):
     pass
 
-
-_RequiredS3DeltaCatalogTargetTypeDef = TypedDict(
-    "_RequiredS3DeltaCatalogTargetTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Table": str,
-        "Database": str,
-    },
-)
-_OptionalS3DeltaCatalogTargetTypeDef = TypedDict(
-    "_OptionalS3DeltaCatalogTargetTypeDef",
-    {
-        "PartitionKeys": List[List[str]],
-        "AdditionalOptions": Dict[str, str],
-        "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-
-class S3DeltaCatalogTargetTypeDef(
-    _RequiredS3DeltaCatalogTargetTypeDef, _OptionalS3DeltaCatalogTargetTypeDef
-):
-    pass
-
-
-_RequiredS3HudiCatalogTargetTypeDef = TypedDict(
-    "_RequiredS3HudiCatalogTargetTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Table": str,
-        "Database": str,
-        "AdditionalOptions": Dict[str, str],
-    },
-)
-_OptionalS3HudiCatalogTargetTypeDef = TypedDict(
-    "_OptionalS3HudiCatalogTargetTypeDef",
-    {
-        "PartitionKeys": List[List[str]],
-        "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-
-class S3HudiCatalogTargetTypeDef(
-    _RequiredS3HudiCatalogTargetTypeDef, _OptionalS3HudiCatalogTargetTypeDef
-):
-    pass
-
-
 ClassifierTypeDef = TypedDict(
     "ClassifierTypeDef",
     {
         "GrokClassifier": GrokClassifierTypeDef,
         "XMLClassifier": XMLClassifierTypeDef,
         "JsonClassifier": JsonClassifierTypeDef,
         "CsvClassifier": CsvClassifierTypeDef,
@@ -5857,19 +5330,17 @@
     "_OptionalCodeGenNodeTypeDef",
     {
         "LineNumber": int,
     },
     total=False,
 )
 
-
 class CodeGenNodeTypeDef(_RequiredCodeGenNodeTypeDef, _OptionalCodeGenNodeTypeDef):
     pass
 
-
 LocationTypeDef = TypedDict(
     "LocationTypeDef",
     {
         "Jdbc": Sequence[CodeGenNodeArgTypeDef],
         "S3": Sequence[CodeGenNodeArgTypeDef],
         "DynamoDB": Sequence[CodeGenNodeArgTypeDef],
     },
@@ -5912,19 +5383,17 @@
         "Description": str,
         "MatchCriteria": Sequence[str],
         "PhysicalConnectionRequirements": PhysicalConnectionRequirementsTypeDef,
     },
     total=False,
 )
 
-
 class ConnectionInputTypeDef(_RequiredConnectionInputTypeDef, _OptionalConnectionInputTypeDef):
     pass
 
-
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "Name": str,
         "Description": str,
         "ConnectionType": ConnectionTypeType,
         "MatchCriteria": List[str],
@@ -5988,107 +5457,30 @@
         "MaxResults": int,
         "Filters": Sequence[CrawlsFilterTypeDef],
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListCrawlsRequestRequestTypeDef(
     _RequiredListCrawlsRequestRequestTypeDef, _OptionalListCrawlsRequestRequestTypeDef
 ):
     pass
 
-
 CreateClassifierRequestRequestTypeDef = TypedDict(
     "CreateClassifierRequestRequestTypeDef",
     {
         "GrokClassifier": CreateGrokClassifierRequestTypeDef,
         "XMLClassifier": CreateXMLClassifierRequestTypeDef,
         "JsonClassifier": CreateJsonClassifierRequestTypeDef,
         "CsvClassifier": CreateCsvClassifierRequestTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateDataQualityRulesetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDataQualityRulesetRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Ruleset": str,
-    },
-)
-_OptionalCreateDataQualityRulesetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDataQualityRulesetRequestRequestTypeDef",
-    {
-        "Description": str,
-        "Tags": Mapping[str, str],
-        "TargetTable": DataQualityTargetTableTypeDef,
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-
-class CreateDataQualityRulesetRequestRequestTypeDef(
-    _RequiredCreateDataQualityRulesetRequestRequestTypeDef,
-    _OptionalCreateDataQualityRulesetRequestRequestTypeDef,
-):
-    pass
-
-
-DataQualityRulesetFilterCriteriaTypeDef = TypedDict(
-    "DataQualityRulesetFilterCriteriaTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "CreatedBefore": Union[datetime, str],
-        "CreatedAfter": Union[datetime, str],
-        "LastModifiedBefore": Union[datetime, str],
-        "LastModifiedAfter": Union[datetime, str],
-        "TargetTable": DataQualityTargetTableTypeDef,
-    },
-    total=False,
-)
-
-DataQualityRulesetListDetailsTypeDef = TypedDict(
-    "DataQualityRulesetListDetailsTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "CreatedOn": datetime,
-        "LastModifiedOn": datetime,
-        "TargetTable": DataQualityTargetTableTypeDef,
-        "RecommendationRunId": str,
-        "RuleCount": int,
-    },
-    total=False,
-)
-
-GetDataQualityRulesetResponseTypeDef = TypedDict(
-    "GetDataQualityRulesetResponseTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "Ruleset": str,
-        "TargetTable": DataQualityTargetTableTypeDef,
-        "CreatedOn": datetime,
-        "LastModifiedOn": datetime,
-        "RecommendationRunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DataSourceTypeDef = TypedDict(
-    "DataSourceTypeDef",
-    {
-        "GlueTable": GlueTableTypeDef,
-    },
-)
-
 _RequiredCreatePartitionIndexRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePartitionIndexRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionIndex": PartitionIndexTypeDef,
     },
@@ -6097,22 +5489,20 @@
     "_OptionalCreatePartitionIndexRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class CreatePartitionIndexRequestRequestTypeDef(
     _RequiredCreatePartitionIndexRequestRequestTypeDef,
     _OptionalCreatePartitionIndexRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateSchemaInputRequestTypeDef = TypedDict(
     "_RequiredCreateSchemaInputRequestTypeDef",
     {
         "SchemaName": str,
         "DataFormat": DataFormatType,
     },
 )
@@ -6124,21 +5514,19 @@
         "Description": str,
         "Tags": Mapping[str, str],
         "SchemaDefinition": str,
     },
     total=False,
 )
 
-
 class CreateSchemaInputRequestTypeDef(
     _RequiredCreateSchemaInputRequestTypeDef, _OptionalCreateSchemaInputRequestTypeDef
 ):
     pass
 
-
 DeleteRegistryInputRequestTypeDef = TypedDict(
     "DeleteRegistryInputRequestTypeDef",
     {
         "RegistryId": RegistryIdTypeDef,
     },
 )
 
@@ -6190,21 +5578,19 @@
         "GlueVersion": str,
         "Tags": Mapping[str, str],
         "RequestOrigin": str,
     },
     total=False,
 )
 
-
 class CreateSessionRequestRequestTypeDef(
     _RequiredCreateSessionRequestRequestTypeDef, _OptionalCreateSessionRequestRequestTypeDef
 ):
     pass
 
-
 SessionTypeDef = TypedDict(
     "SessionTypeDef",
     {
         "Id": str,
         "CreatedOn": datetime,
         "Status": SessionStatusType,
         "ErrorMessage": str,
@@ -6217,39 +5603,14 @@
         "MaxCapacity": float,
         "SecurityConfiguration": str,
         "GlueVersion": str,
     },
     total=False,
 )
 
-_RequiredEvaluateDataQualityTypeDef = TypedDict(
-    "_RequiredEvaluateDataQualityTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Ruleset": str,
-    },
-)
-_OptionalEvaluateDataQualityTypeDef = TypedDict(
-    "_OptionalEvaluateDataQualityTypeDef",
-    {
-        "Output": DQTransformOutputType,
-        "PublishingOptions": DQResultsPublishingOptionsTypeDef,
-        "StopJobOnFailureOptions": DQStopJobOnFailureOptionsTypeDef,
-    },
-    total=False,
-)
-
-
-class EvaluateDataQualityTypeDef(
-    _RequiredEvaluateDataQualityTypeDef, _OptionalEvaluateDataQualityTypeDef
-):
-    pass
-
-
 DataCatalogEncryptionSettingsTypeDef = TypedDict(
     "DataCatalogEncryptionSettingsTypeDef",
     {
         "EncryptionAtRest": EncryptionAtRestTypeDef,
         "ConnectionPasswordEncryption": ConnectionPasswordEncryptionTypeDef,
     },
     total=False,
@@ -6284,21 +5645,19 @@
     {
         "MinimumValue": DecimalNumberTypeDef,
         "MaximumValue": DecimalNumberTypeDef,
     },
     total=False,
 )
 
-
 class DecimalColumnStatisticsDataTypeDef(
     _RequiredDecimalColumnStatisticsDataTypeDef, _OptionalDecimalColumnStatisticsDataTypeDef
 ):
     pass
 
-
 DeleteSchemaInputRequestTypeDef = TypedDict(
     "DeleteSchemaInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
     },
 )
 
@@ -6336,21 +5695,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListSchemaVersionsInputRequestTypeDef(
     _RequiredListSchemaVersionsInputRequestTypeDef, _OptionalListSchemaVersionsInputRequestTypeDef
 ):
     pass
 
-
 RegisterSchemaVersionInputRequestTypeDef = TypedDict(
     "RegisterSchemaVersionInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
         "SchemaDefinition": str,
     },
 )
@@ -6381,48 +5738,19 @@
         "UpdateEtlLibraries": bool,
         "DeleteArguments": Sequence[str],
         "AddArguments": Mapping[str, str],
     },
     total=False,
 )
 
-
 class UpdateDevEndpointRequestRequestTypeDef(
     _RequiredUpdateDevEndpointRequestRequestTypeDef, _OptionalUpdateDevEndpointRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredS3DeltaDirectTargetTypeDef = TypedDict(
-    "_RequiredS3DeltaDirectTargetTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Path": str,
-        "Compression": DeltaTargetCompressionTypeType,
-        "Format": TargetFormatType,
-    },
-)
-_OptionalS3DeltaDirectTargetTypeDef = TypedDict(
-    "_OptionalS3DeltaDirectTargetTypeDef",
-    {
-        "PartitionKeys": List[List[str]],
-        "AdditionalOptions": Dict[str, str],
-        "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-
-class S3DeltaDirectTargetTypeDef(
-    _RequiredS3DeltaDirectTargetTypeDef, _OptionalS3DeltaDirectTargetTypeDef
-):
-    pass
-
-
 _RequiredS3DirectTargetTypeDef = TypedDict(
     "_RequiredS3DirectTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Path": str,
         "Format": TargetFormatType,
@@ -6434,19 +5762,17 @@
         "PartitionKeys": List[List[str]],
         "Compression": str,
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
-
 class S3DirectTargetTypeDef(_RequiredS3DirectTargetTypeDef, _OptionalS3DirectTargetTypeDef):
     pass
 
-
 _RequiredS3GlueParquetTargetTypeDef = TypedDict(
     "_RequiredS3GlueParquetTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Path": str,
     },
@@ -6457,72 +5783,19 @@
         "PartitionKeys": List[List[str]],
         "Compression": ParquetCompressionTypeType,
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
-
 class S3GlueParquetTargetTypeDef(
     _RequiredS3GlueParquetTargetTypeDef, _OptionalS3GlueParquetTargetTypeDef
 ):
     pass
 
-
-_RequiredS3HudiDirectTargetTypeDef = TypedDict(
-    "_RequiredS3HudiDirectTargetTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Path": str,
-        "Compression": HudiTargetCompressionTypeType,
-        "Format": TargetFormatType,
-        "AdditionalOptions": Dict[str, str],
-    },
-)
-_OptionalS3HudiDirectTargetTypeDef = TypedDict(
-    "_OptionalS3HudiDirectTargetTypeDef",
-    {
-        "PartitionKeys": List[List[str]],
-        "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-
-class S3HudiDirectTargetTypeDef(
-    _RequiredS3HudiDirectTargetTypeDef, _OptionalS3HudiDirectTargetTypeDef
-):
-    pass
-
-
-_RequiredDynamicTransformTypeDef = TypedDict(
-    "_RequiredDynamicTransformTypeDef",
-    {
-        "Name": str,
-        "TransformName": str,
-        "Inputs": List[str],
-        "FunctionName": str,
-        "Path": str,
-    },
-)
-_OptionalDynamicTransformTypeDef = TypedDict(
-    "_OptionalDynamicTransformTypeDef",
-    {
-        "Parameters": List[TransformConfigParameterTypeDef],
-        "Version": str,
-    },
-    total=False,
-)
-
-
-class DynamicTransformTypeDef(_RequiredDynamicTransformTypeDef, _OptionalDynamicTransformTypeDef):
-    pass
-
-
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "S3Encryption": Sequence[S3EncryptionTypeDef],
         "CloudWatchEncryption": CloudWatchEncryptionTypeDef,
         "JobBookmarksEncryption": JobBookmarksEncryptionTypeDef,
     },
@@ -6549,40 +5822,36 @@
     "_OptionalFilterExpressionTypeDef",
     {
         "Negated": bool,
     },
     total=False,
 )
 
-
 class FilterExpressionTypeDef(_RequiredFilterExpressionTypeDef, _OptionalFilterExpressionTypeDef):
     pass
 
-
 _RequiredTransformParametersTypeDef = TypedDict(
     "_RequiredTransformParametersTypeDef",
     {
         "TransformType": Literal["FIND_MATCHES"],
     },
 )
 _OptionalTransformParametersTypeDef = TypedDict(
     "_OptionalTransformParametersTypeDef",
     {
         "FindMatchesParameters": FindMatchesParametersTypeDef,
     },
     total=False,
 )
 
-
 class TransformParametersTypeDef(
     _RequiredTransformParametersTypeDef, _OptionalTransformParametersTypeDef
 ):
     pass
 
-
 GetClassifiersRequestGetClassifiersPaginateTypeDef = TypedDict(
     "GetClassifiersRequestGetClassifiersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6632,22 +5901,20 @@
     "_OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetJobRunsRequestGetJobRunsPaginateTypeDef(
     _RequiredGetJobRunsRequestGetJobRunsPaginateTypeDef,
     _OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef,
 ):
     pass
 
-
 GetJobsRequestGetJobsPaginateTypeDef = TypedDict(
     "GetJobsRequestGetJobsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6664,22 +5931,20 @@
     {
         "CatalogId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef(
     _RequiredGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
     _OptionalGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
 ):
     pass
 
-
 GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
     "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6704,22 +5969,20 @@
     {
         "CatalogId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetTableVersionsRequestGetTableVersionsPaginateTypeDef(
     _RequiredGetTableVersionsRequestGetTableVersionsPaginateTypeDef,
     _OptionalGetTableVersionsRequestGetTableVersionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetTablesRequestGetTablesPaginateTypeDef = TypedDict(
     "_RequiredGetTablesRequestGetTablesPaginateTypeDef",
     {
         "DatabaseName": str,
     },
 )
 _OptionalGetTablesRequestGetTablesPaginateTypeDef = TypedDict(
@@ -6730,22 +5993,20 @@
         "TransactionId": str,
         "QueryAsOfTime": Union[datetime, str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetTablesRequestGetTablesPaginateTypeDef(
     _RequiredGetTablesRequestGetTablesPaginateTypeDef,
     _OptionalGetTablesRequestGetTablesPaginateTypeDef,
 ):
     pass
 
-
 GetTriggersRequestGetTriggersPaginateTypeDef = TypedDict(
     "GetTriggersRequestGetTriggersPaginateTypeDef",
     {
         "DependentJobName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -6763,22 +6024,20 @@
         "CatalogId": str,
         "DatabaseName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef(
     _RequiredGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
     _OptionalGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
 ):
     pass
 
-
 ListRegistriesInputListRegistriesPaginateTypeDef = TypedDict(
     "ListRegistriesInputListRegistriesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6793,22 +6052,20 @@
     "_OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef(
     _RequiredListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
     _OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
 ):
     pass
 
-
 ListSchemasInputListSchemasPaginateTypeDef = TypedDict(
     "ListSchemasInputListSchemasPaginateTypeDef",
     {
         "RegistryId": RegistryIdTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -6866,21 +6123,19 @@
         "MaxResults": int,
         "Filter": TaskRunFilterCriteriaTypeDef,
         "Sort": TaskRunSortCriteriaTypeDef,
     },
     total=False,
 )
 
-
 class GetMLTaskRunsRequestRequestTypeDef(
     _RequiredGetMLTaskRunsRequestRequestTypeDef, _OptionalGetMLTaskRunsRequestRequestTypeDef
 ):
     pass
 
-
 TransformFilterCriteriaTypeDef = TypedDict(
     "TransformFilterCriteriaTypeDef",
     {
         "Name": str,
         "TransformType": Literal["FIND_MATCHES"],
         "Status": TransformStatusTypeType,
         "GlueVersion": str,
@@ -6918,22 +6173,20 @@
         "TransactionId": str,
         "QueryAsOfTime": Union[datetime, str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetPartitionsRequestGetPartitionsPaginateTypeDef(
     _RequiredGetPartitionsRequestGetPartitionsPaginateTypeDef,
     _OptionalGetPartitionsRequestGetPartitionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetPartitionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetPartitionsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -6948,21 +6201,19 @@
         "ExcludeColumnSchema": bool,
         "TransactionId": str,
         "QueryAsOfTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class GetPartitionsRequestRequestTypeDef(
     _RequiredGetPartitionsRequestRequestTypeDef, _OptionalGetPartitionsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetUnfilteredPartitionsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetUnfilteredPartitionsMetadataRequestRequestTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "SupportedPermissionTypes": Sequence[PermissionTypeType],
@@ -6976,22 +6227,20 @@
         "NextToken": str,
         "Segment": SegmentTypeDef,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetUnfilteredPartitionsMetadataRequestRequestTypeDef(
     _RequiredGetUnfilteredPartitionsMetadataRequestRequestTypeDef,
     _OptionalGetUnfilteredPartitionsMetadataRequestRequestTypeDef,
 ):
     pass
 
-
 GetResourcePoliciesResponseTypeDef = TypedDict(
     "GetResourcePoliciesResponseTypeDef",
     {
         "GetResourcePoliciesResponseList": List[GluePolicyTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -7029,21 +6278,19 @@
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "Compatibility": CompatibilityType,
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateSchemaInputRequestTypeDef(
     _RequiredUpdateSchemaInputRequestTypeDef, _OptionalUpdateSchemaInputRequestTypeDef
 ):
     pass
 
-
 GlueSchemaTypeDef = TypedDict(
     "GlueSchemaTypeDef",
     {
         "Columns": List[GlueStudioSchemaColumnTypeDef],
     },
     total=False,
 )
@@ -7061,21 +6308,19 @@
     {
         "PartitionPredicate": str,
         "AdditionalOptions": S3SourceAdditionalOptionsTypeDef,
     },
     total=False,
 )
 
-
 class GovernedCatalogSourceTypeDef(
     _RequiredGovernedCatalogSourceTypeDef, _OptionalGovernedCatalogSourceTypeDef
 ):
     pass
 
-
 _RequiredS3CatalogSourceTypeDef = TypedDict(
     "_RequiredS3CatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -7085,19 +6330,17 @@
     {
         "PartitionPredicate": str,
         "AdditionalOptions": S3SourceAdditionalOptionsTypeDef,
     },
     total=False,
 )
 
-
 class S3CatalogSourceTypeDef(_RequiredS3CatalogSourceTypeDef, _OptionalS3CatalogSourceTypeDef):
     pass
 
-
 JobRunTypeDef = TypedDict(
     "JobRunTypeDef",
     {
         "Id": str,
         "Attempt": int,
         "PreviousRunId": str,
         "TriggerName": str,
@@ -7205,22 +6448,20 @@
         "SchemaId": SchemaIdTypeDef,
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "SchemaVersionId": str,
     },
     total=False,
 )
 
-
 class PutSchemaVersionMetadataInputRequestTypeDef(
     _RequiredPutSchemaVersionMetadataInputRequestTypeDef,
     _OptionalPutSchemaVersionMetadataInputRequestTypeDef,
 ):
     pass
 
-
 QuerySchemaVersionMetadataInputRequestTypeDef = TypedDict(
     "QuerySchemaVersionMetadataInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "SchemaVersionId": str,
         "MetadataList": Sequence[MetadataKeyValuePairTypeDef],
@@ -7242,22 +6483,20 @@
         "SchemaId": SchemaIdTypeDef,
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "SchemaVersionId": str,
     },
     total=False,
 )
 
-
 class RemoveSchemaVersionMetadataInputRequestTypeDef(
     _RequiredRemoveSchemaVersionMetadataInputRequestTypeDef,
     _OptionalRemoveSchemaVersionMetadataInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredRedshiftTargetTypeDef = TypedDict(
     "_RequiredRedshiftTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Database": str,
         "Table": str,
@@ -7269,19 +6508,17 @@
         "RedshiftTmpDir": str,
         "TmpDirIAMRole": str,
         "UpsertRedshiftOptions": UpsertRedshiftTargetOptionsTypeDef,
     },
     total=False,
 )
 
-
 class RedshiftTargetTypeDef(_RequiredRedshiftTargetTypeDef, _OptionalRedshiftTargetTypeDef):
     pass
 
-
 UserDefinedFunctionInputTypeDef = TypedDict(
     "UserDefinedFunctionInputTypeDef",
     {
         "FunctionName": str,
         "ClassName": str,
         "OwnerName": str,
         "OwnerType": PrincipalTypeType,
@@ -7355,21 +6592,19 @@
     "_OptionalPartitionIndexDescriptorTypeDef",
     {
         "BackfillErrors": List[BackfillErrorTypeDef],
     },
     total=False,
 )
 
-
 class PartitionIndexDescriptorTypeDef(
     _RequiredPartitionIndexDescriptorTypeDef, _OptionalPartitionIndexDescriptorTypeDef
 ):
     pass
 
-
 BatchStopJobRunResponseTypeDef = TypedDict(
     "BatchStopJobRunResponseTypeDef",
     {
         "SuccessfulSubmissions": List[BatchStopJobRunSuccessfulSubmissionTypeDef],
         "Errors": List[BatchStopJobRunErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -7479,21 +6714,19 @@
     {
         "Sinks": Sequence[CatalogEntryTypeDef],
         "Location": LocationTypeDef,
     },
     total=False,
 )
 
-
 class GetMappingRequestRequestTypeDef(
     _RequiredGetMappingRequestRequestTypeDef, _OptionalGetMappingRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetPlanRequestRequestTypeDef = TypedDict(
     "_RequiredGetPlanRequestRequestTypeDef",
     {
         "Mapping": Sequence[MappingEntryTypeDef],
         "Source": CatalogEntryTypeDef,
     },
 )
@@ -7504,21 +6737,19 @@
         "Location": LocationTypeDef,
         "Language": LanguageType,
         "AdditionalPlanOptionsMap": Mapping[str, str],
     },
     total=False,
 )
 
-
 class GetPlanRequestRequestTypeDef(
     _RequiredGetPlanRequestRequestTypeDef, _OptionalGetPlanRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateTriggerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTriggerRequestRequestTypeDef",
     {
         "Name": str,
         "Type": TriggerTypeType,
         "Actions": Sequence[ActionTypeDef],
     },
@@ -7533,21 +6764,19 @@
         "StartOnCreation": bool,
         "Tags": Mapping[str, str],
         "EventBatchingCondition": EventBatchingConditionTypeDef,
     },
     total=False,
 )
 
-
 class CreateTriggerRequestRequestTypeDef(
     _RequiredCreateTriggerRequestRequestTypeDef, _OptionalCreateTriggerRequestRequestTypeDef
 ):
     pass
 
-
 TriggerTypeDef = TypedDict(
     "TriggerTypeDef",
     {
         "Name": str,
         "WorkflowName": str,
         "Id": str,
         "Type": TriggerTypeType,
@@ -7584,21 +6813,19 @@
     "_OptionalEvaluationMetricsTypeDef",
     {
         "FindMatchesMetrics": FindMatchesMetricsTypeDef,
     },
     total=False,
 )
 
-
 class EvaluationMetricsTypeDef(
     _RequiredEvaluationMetricsTypeDef, _OptionalEvaluationMetricsTypeDef
 ):
     pass
 
-
 _RequiredCreateConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectionRequestRequestTypeDef",
     {
         "ConnectionInput": ConnectionInputTypeDef,
     },
 )
 _OptionalCreateConnectionRequestRequestTypeDef = TypedDict(
@@ -7606,21 +6833,19 @@
     {
         "CatalogId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateConnectionRequestRequestTypeDef(
     _RequiredCreateConnectionRequestRequestTypeDef, _OptionalCreateConnectionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConnectionRequestRequestTypeDef",
     {
         "Name": str,
         "ConnectionInput": ConnectionInputTypeDef,
     },
 )
@@ -7628,21 +6853,19 @@
     "_OptionalUpdateConnectionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class UpdateConnectionRequestRequestTypeDef(
     _RequiredUpdateConnectionRequestRequestTypeDef, _OptionalUpdateConnectionRequestRequestTypeDef
 ):
     pass
 
-
 GetConnectionResponseTypeDef = TypedDict(
     "GetConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -7706,21 +6929,19 @@
         "Configuration": str,
         "CrawlerSecurityConfiguration": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateCrawlerRequestRequestTypeDef(
     _RequiredCreateCrawlerRequestRequestTypeDef, _OptionalCreateCrawlerRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateCrawlerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateCrawlerRequestRequestTypeDef = TypedDict(
@@ -7739,263 +6960,19 @@
         "LakeFormationConfiguration": LakeFormationConfigurationTypeDef,
         "Configuration": str,
         "CrawlerSecurityConfiguration": str,
     },
     total=False,
 )
 
-
 class UpdateCrawlerRequestRequestTypeDef(
     _RequiredUpdateCrawlerRequestRequestTypeDef, _OptionalUpdateCrawlerRequestRequestTypeDef
 ):
     pass
 
-
-ListDataQualityRulesetsRequestRequestTypeDef = TypedDict(
-    "ListDataQualityRulesetsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "Filter": DataQualityRulesetFilterCriteriaTypeDef,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-ListDataQualityRulesetsResponseTypeDef = TypedDict(
-    "ListDataQualityRulesetsResponseTypeDef",
-    {
-        "Rulesets": List[DataQualityRulesetListDetailsTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DataQualityResultDescriptionTypeDef = TypedDict(
-    "DataQualityResultDescriptionTypeDef",
-    {
-        "ResultId": str,
-        "DataSource": DataSourceTypeDef,
-        "JobName": str,
-        "JobRunId": str,
-        "StartedOn": datetime,
-    },
-    total=False,
-)
-
-DataQualityResultFilterCriteriaTypeDef = TypedDict(
-    "DataQualityResultFilterCriteriaTypeDef",
-    {
-        "DataSource": DataSourceTypeDef,
-        "JobName": str,
-        "JobRunId": str,
-        "StartedAfter": Union[datetime, str],
-        "StartedBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
-DataQualityResultTypeDef = TypedDict(
-    "DataQualityResultTypeDef",
-    {
-        "ResultId": str,
-        "Score": float,
-        "DataSource": DataSourceTypeDef,
-        "RulesetName": str,
-        "EvaluationContext": str,
-        "StartedOn": datetime,
-        "CompletedOn": datetime,
-        "JobName": str,
-        "JobRunId": str,
-        "RulesetEvaluationRunId": str,
-        "RuleResults": List[DataQualityRuleResultTypeDef],
-    },
-    total=False,
-)
-
-DataQualityRuleRecommendationRunDescriptionTypeDef = TypedDict(
-    "DataQualityRuleRecommendationRunDescriptionTypeDef",
-    {
-        "RunId": str,
-        "Status": TaskStatusTypeType,
-        "StartedOn": datetime,
-        "DataSource": DataSourceTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDataQualityRuleRecommendationRunFilterTypeDef = TypedDict(
-    "_RequiredDataQualityRuleRecommendationRunFilterTypeDef",
-    {
-        "DataSource": DataSourceTypeDef,
-    },
-)
-_OptionalDataQualityRuleRecommendationRunFilterTypeDef = TypedDict(
-    "_OptionalDataQualityRuleRecommendationRunFilterTypeDef",
-    {
-        "StartedBefore": Union[datetime, str],
-        "StartedAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class DataQualityRuleRecommendationRunFilterTypeDef(
-    _RequiredDataQualityRuleRecommendationRunFilterTypeDef,
-    _OptionalDataQualityRuleRecommendationRunFilterTypeDef,
-):
-    pass
-
-
-DataQualityRulesetEvaluationRunDescriptionTypeDef = TypedDict(
-    "DataQualityRulesetEvaluationRunDescriptionTypeDef",
-    {
-        "RunId": str,
-        "Status": TaskStatusTypeType,
-        "StartedOn": datetime,
-        "DataSource": DataSourceTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDataQualityRulesetEvaluationRunFilterTypeDef = TypedDict(
-    "_RequiredDataQualityRulesetEvaluationRunFilterTypeDef",
-    {
-        "DataSource": DataSourceTypeDef,
-    },
-)
-_OptionalDataQualityRulesetEvaluationRunFilterTypeDef = TypedDict(
-    "_OptionalDataQualityRulesetEvaluationRunFilterTypeDef",
-    {
-        "StartedBefore": Union[datetime, str],
-        "StartedAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class DataQualityRulesetEvaluationRunFilterTypeDef(
-    _RequiredDataQualityRulesetEvaluationRunFilterTypeDef,
-    _OptionalDataQualityRulesetEvaluationRunFilterTypeDef,
-):
-    pass
-
-
-GetDataQualityResultResponseTypeDef = TypedDict(
-    "GetDataQualityResultResponseTypeDef",
-    {
-        "ResultId": str,
-        "Score": float,
-        "DataSource": DataSourceTypeDef,
-        "RulesetName": str,
-        "EvaluationContext": str,
-        "StartedOn": datetime,
-        "CompletedOn": datetime,
-        "JobName": str,
-        "JobRunId": str,
-        "RulesetEvaluationRunId": str,
-        "RuleResults": List[DataQualityRuleResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDataQualityRuleRecommendationRunResponseTypeDef = TypedDict(
-    "GetDataQualityRuleRecommendationRunResponseTypeDef",
-    {
-        "RunId": str,
-        "DataSource": DataSourceTypeDef,
-        "Role": str,
-        "NumberOfWorkers": int,
-        "Timeout": int,
-        "Status": TaskStatusTypeType,
-        "ErrorString": str,
-        "StartedOn": datetime,
-        "LastModifiedOn": datetime,
-        "CompletedOn": datetime,
-        "ExecutionTime": int,
-        "RecommendedRuleset": str,
-        "CreatedRulesetName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDataQualityRulesetEvaluationRunResponseTypeDef = TypedDict(
-    "GetDataQualityRulesetEvaluationRunResponseTypeDef",
-    {
-        "RunId": str,
-        "DataSource": DataSourceTypeDef,
-        "Role": str,
-        "NumberOfWorkers": int,
-        "Timeout": int,
-        "AdditionalRunOptions": DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
-        "Status": TaskStatusTypeType,
-        "ErrorString": str,
-        "StartedOn": datetime,
-        "LastModifiedOn": datetime,
-        "CompletedOn": datetime,
-        "ExecutionTime": int,
-        "RulesetNames": List[str],
-        "ResultIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
-    "_RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef",
-    {
-        "DataSource": DataSourceTypeDef,
-        "Role": str,
-    },
-)
-_OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
-    "_OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef",
-    {
-        "NumberOfWorkers": int,
-        "Timeout": int,
-        "CreatedRulesetName": str,
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-
-class StartDataQualityRuleRecommendationRunRequestRequestTypeDef(
-    _RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
-    _OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
-    "_RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
-    {
-        "DataSource": DataSourceTypeDef,
-        "Role": str,
-        "RulesetNames": Sequence[str],
-    },
-)
-_OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
-    "_OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
-    {
-        "NumberOfWorkers": int,
-        "Timeout": int,
-        "ClientToken": str,
-        "AdditionalRunOptions": DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
-    },
-    total=False,
-)
-
-
-class StartDataQualityRulesetEvaluationRunRequestRequestTypeDef(
-    _RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
-    _OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
-):
-    pass
-
-
 CreateSessionResponseTypeDef = TypedDict(
     "CreateSessionResponseTypeDef",
     {
         "Session": SessionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -8036,22 +7013,20 @@
     "_OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class PutDataCatalogEncryptionSettingsRequestRequestTypeDef(
     _RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef,
     _OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDatabaseInputTypeDef = TypedDict(
     "_RequiredDatabaseInputTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDatabaseInputTypeDef = TypedDict(
@@ -8062,19 +7037,17 @@
         "Parameters": Mapping[str, str],
         "CreateTableDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
         "TargetDatabase": DatabaseIdentifierTypeDef,
     },
     total=False,
 )
 
-
 class DatabaseInputTypeDef(_RequiredDatabaseInputTypeDef, _OptionalDatabaseInputTypeDef):
     pass
 
-
 _RequiredDatabaseTypeDef = TypedDict(
     "_RequiredDatabaseTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDatabaseTypeDef = TypedDict(
@@ -8087,19 +7060,17 @@
         "CreateTableDefaultPermissions": List[PrincipalPermissionsTypeDef],
         "TargetDatabase": DatabaseIdentifierTypeDef,
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class DatabaseTypeDef(_RequiredDatabaseTypeDef, _OptionalDatabaseTypeDef):
     pass
 
-
 _RequiredDropNullFieldsTypeDef = TypedDict(
     "_RequiredDropNullFieldsTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
     },
 )
@@ -8108,19 +7079,17 @@
     {
         "NullCheckBoxList": NullCheckBoxListTypeDef,
         "NullTextList": List[NullValueFieldTypeDef],
     },
     total=False,
 )
 
-
 class DropNullFieldsTypeDef(_RequiredDropNullFieldsTypeDef, _OptionalDropNullFieldsTypeDef):
     pass
 
-
 _RequiredColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredColumnStatisticsDataTypeDef",
     {
         "Type": ColumnStatisticsTypeType,
     },
 )
 _OptionalColumnStatisticsDataTypeDef = TypedDict(
@@ -8133,21 +7102,19 @@
         "LongColumnStatisticsData": LongColumnStatisticsDataTypeDef,
         "StringColumnStatisticsData": StringColumnStatisticsDataTypeDef,
         "BinaryColumnStatisticsData": BinaryColumnStatisticsDataTypeDef,
     },
     total=False,
 )
 
-
 class ColumnStatisticsDataTypeDef(
     _RequiredColumnStatisticsDataTypeDef, _OptionalColumnStatisticsDataTypeDef
 ):
     pass
 
-
 StorageDescriptorTypeDef = TypedDict(
     "StorageDescriptorTypeDef",
     {
         "Columns": Sequence[ColumnTypeDef],
         "Location": str,
         "AdditionalLocations": Sequence[str],
         "InputFormat": str,
@@ -8220,21 +7187,19 @@
         "NumberOfWorkers": int,
         "Timeout": int,
         "MaxRetries": int,
     },
     total=False,
 )
 
-
 class UpdateMLTransformRequestRequestTypeDef(
     _RequiredUpdateMLTransformRequestRequestTypeDef, _OptionalUpdateMLTransformRequestRequestTypeDef
 ):
     pass
 
-
 GetMLTransformsRequestRequestTypeDef = TypedDict(
     "GetMLTransformsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filter": TransformFilterCriteriaTypeDef,
         "Sort": TransformSortCriteriaTypeDef,
@@ -8269,69 +7234,19 @@
     {
         "ConnectionTable": str,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class AthenaConnectorSourceTypeDef(
     _RequiredAthenaConnectorSourceTypeDef, _OptionalAthenaConnectorSourceTypeDef
 ):
     pass
 
-
-_RequiredCatalogDeltaSourceTypeDef = TypedDict(
-    "_RequiredCatalogDeltaSourceTypeDef",
-    {
-        "Name": str,
-        "Database": str,
-        "Table": str,
-    },
-)
-_OptionalCatalogDeltaSourceTypeDef = TypedDict(
-    "_OptionalCatalogDeltaSourceTypeDef",
-    {
-        "AdditionalDeltaOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaTypeDef],
-    },
-    total=False,
-)
-
-
-class CatalogDeltaSourceTypeDef(
-    _RequiredCatalogDeltaSourceTypeDef, _OptionalCatalogDeltaSourceTypeDef
-):
-    pass
-
-
-_RequiredCatalogHudiSourceTypeDef = TypedDict(
-    "_RequiredCatalogHudiSourceTypeDef",
-    {
-        "Name": str,
-        "Database": str,
-        "Table": str,
-    },
-)
-_OptionalCatalogHudiSourceTypeDef = TypedDict(
-    "_OptionalCatalogHudiSourceTypeDef",
-    {
-        "AdditionalHudiOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaTypeDef],
-    },
-    total=False,
-)
-
-
-class CatalogHudiSourceTypeDef(
-    _RequiredCatalogHudiSourceTypeDef, _OptionalCatalogHudiSourceTypeDef
-):
-    pass
-
-
 _RequiredCustomCodeTypeDef = TypedDict(
     "_RequiredCustomCodeTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Code": str,
         "ClassName": str,
@@ -8341,19 +7256,17 @@
     "_OptionalCustomCodeTypeDef",
     {
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class CustomCodeTypeDef(_RequiredCustomCodeTypeDef, _OptionalCustomCodeTypeDef):
     pass
 
-
 _RequiredJDBCConnectorSourceTypeDef = TypedDict(
     "_RequiredJDBCConnectorSourceTypeDef",
     {
         "Name": str,
         "ConnectionName": str,
         "ConnectorName": str,
         "ConnectionType": str,
@@ -8366,21 +7279,19 @@
         "ConnectionTable": str,
         "Query": str,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class JDBCConnectorSourceTypeDef(
     _RequiredJDBCConnectorSourceTypeDef, _OptionalJDBCConnectorSourceTypeDef
 ):
     pass
 
-
 _RequiredJDBCConnectorTargetTypeDef = TypedDict(
     "_RequiredJDBCConnectorTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "ConnectionName": str,
         "ConnectionTable": str,
@@ -8393,69 +7304,19 @@
     {
         "AdditionalOptions": Dict[str, str],
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class JDBCConnectorTargetTypeDef(
     _RequiredJDBCConnectorTargetTypeDef, _OptionalJDBCConnectorTargetTypeDef
 ):
     pass
 
-
-_RequiredS3CatalogDeltaSourceTypeDef = TypedDict(
-    "_RequiredS3CatalogDeltaSourceTypeDef",
-    {
-        "Name": str,
-        "Database": str,
-        "Table": str,
-    },
-)
-_OptionalS3CatalogDeltaSourceTypeDef = TypedDict(
-    "_OptionalS3CatalogDeltaSourceTypeDef",
-    {
-        "AdditionalDeltaOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaTypeDef],
-    },
-    total=False,
-)
-
-
-class S3CatalogDeltaSourceTypeDef(
-    _RequiredS3CatalogDeltaSourceTypeDef, _OptionalS3CatalogDeltaSourceTypeDef
-):
-    pass
-
-
-_RequiredS3CatalogHudiSourceTypeDef = TypedDict(
-    "_RequiredS3CatalogHudiSourceTypeDef",
-    {
-        "Name": str,
-        "Database": str,
-        "Table": str,
-    },
-)
-_OptionalS3CatalogHudiSourceTypeDef = TypedDict(
-    "_OptionalS3CatalogHudiSourceTypeDef",
-    {
-        "AdditionalHudiOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaTypeDef],
-    },
-    total=False,
-)
-
-
-class S3CatalogHudiSourceTypeDef(
-    _RequiredS3CatalogHudiSourceTypeDef, _OptionalS3CatalogHudiSourceTypeDef
-):
-    pass
-
-
 _RequiredS3CsvSourceTypeDef = TypedDict(
     "_RequiredS3CsvSourceTypeDef",
     {
         "Name": str,
         "Paths": List[str],
         "Separator": SeparatorType,
         "QuoteChar": QuoteCharType,
@@ -8479,63 +7340,17 @@
         "SkipFirst": bool,
         "OptimizePerformance": bool,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class S3CsvSourceTypeDef(_RequiredS3CsvSourceTypeDef, _OptionalS3CsvSourceTypeDef):
     pass
 
-
-_RequiredS3DeltaSourceTypeDef = TypedDict(
-    "_RequiredS3DeltaSourceTypeDef",
-    {
-        "Name": str,
-        "Paths": List[str],
-    },
-)
-_OptionalS3DeltaSourceTypeDef = TypedDict(
-    "_OptionalS3DeltaSourceTypeDef",
-    {
-        "AdditionalDeltaOptions": Dict[str, str],
-        "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "OutputSchemas": List[GlueSchemaTypeDef],
-    },
-    total=False,
-)
-
-
-class S3DeltaSourceTypeDef(_RequiredS3DeltaSourceTypeDef, _OptionalS3DeltaSourceTypeDef):
-    pass
-
-
-_RequiredS3HudiSourceTypeDef = TypedDict(
-    "_RequiredS3HudiSourceTypeDef",
-    {
-        "Name": str,
-        "Paths": List[str],
-    },
-)
-_OptionalS3HudiSourceTypeDef = TypedDict(
-    "_OptionalS3HudiSourceTypeDef",
-    {
-        "AdditionalHudiOptions": Dict[str, str],
-        "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "OutputSchemas": List[GlueSchemaTypeDef],
-    },
-    total=False,
-)
-
-
-class S3HudiSourceTypeDef(_RequiredS3HudiSourceTypeDef, _OptionalS3HudiSourceTypeDef):
-    pass
-
-
 _RequiredS3JsonSourceTypeDef = TypedDict(
     "_RequiredS3JsonSourceTypeDef",
     {
         "Name": str,
         "Paths": List[str],
     },
 )
@@ -8553,19 +7368,17 @@
         "JsonPath": str,
         "Multiline": bool,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class S3JsonSourceTypeDef(_RequiredS3JsonSourceTypeDef, _OptionalS3JsonSourceTypeDef):
     pass
 
-
 _RequiredS3ParquetSourceTypeDef = TypedDict(
     "_RequiredS3ParquetSourceTypeDef",
     {
         "Name": str,
         "Paths": List[str],
     },
 )
@@ -8581,19 +7394,17 @@
         "MaxFilesInBand": int,
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class S3ParquetSourceTypeDef(_RequiredS3ParquetSourceTypeDef, _OptionalS3ParquetSourceTypeDef):
     pass
 
-
 _RequiredSparkConnectorSourceTypeDef = TypedDict(
     "_RequiredSparkConnectorSourceTypeDef",
     {
         "Name": str,
         "ConnectionName": str,
         "ConnectorName": str,
         "ConnectionType": str,
@@ -8604,21 +7415,19 @@
     {
         "AdditionalOptions": Dict[str, str],
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class SparkConnectorSourceTypeDef(
     _RequiredSparkConnectorSourceTypeDef, _OptionalSparkConnectorSourceTypeDef
 ):
     pass
 
-
 _RequiredSparkConnectorTargetTypeDef = TypedDict(
     "_RequiredSparkConnectorTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "ConnectionName": str,
         "ConnectorName": str,
@@ -8630,21 +7439,19 @@
     {
         "AdditionalOptions": Dict[str, str],
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class SparkConnectorTargetTypeDef(
     _RequiredSparkConnectorTargetTypeDef, _OptionalSparkConnectorTargetTypeDef
 ):
     pass
 
-
 _RequiredSparkSQLTypeDef = TypedDict(
     "_RequiredSparkSQLTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "SqlQuery": str,
         "SqlAliases": List[SqlAliasTypeDef],
@@ -8654,19 +7461,17 @@
     "_OptionalSparkSQLTypeDef",
     {
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-
 class SparkSQLTypeDef(_RequiredSparkSQLTypeDef, _OptionalSparkSQLTypeDef):
     pass
 
-
 GetJobRunResponseTypeDef = TypedDict(
     "GetJobRunResponseTypeDef",
     {
         "JobRun": JobRunTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -8743,21 +7548,19 @@
         "MaxRetries": int,
         "Tags": Mapping[str, str],
         "TransformEncryption": TransformEncryptionTypeDef,
     },
     total=False,
 )
 
-
 class CreateMLTransformRequestRequestTypeDef(
     _RequiredCreateMLTransformRequestRequestTypeDef, _OptionalCreateMLTransformRequestRequestTypeDef
 ):
     pass
 
-
 QuerySchemaVersionMetadataResponseTypeDef = TypedDict(
     "QuerySchemaVersionMetadataResponseTypeDef",
     {
         "MetadataInfoMap": Dict[str, MetadataInfoTypeDef],
         "SchemaVersionId": str,
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -8775,22 +7578,20 @@
     "_OptionalCreateUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class CreateUserDefinedFunctionRequestRequestTypeDef(
     _RequiredCreateUserDefinedFunctionRequestRequestTypeDef,
     _OptionalCreateUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateUserDefinedFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserDefinedFunctionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "FunctionName": str,
         "FunctionInput": UserDefinedFunctionInputTypeDef,
     },
@@ -8799,22 +7600,20 @@
     "_OptionalUpdateUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class UpdateUserDefinedFunctionRequestRequestTypeDef(
     _RequiredUpdateUserDefinedFunctionRequestRequestTypeDef,
     _OptionalUpdateUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
-
 GetUserDefinedFunctionResponseTypeDef = TypedDict(
     "GetUserDefinedFunctionResponseTypeDef",
     {
         "UserDefinedFunction": UserDefinedFunctionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -8975,80 +7774,14 @@
     {
         "Crawlers": List[CrawlerTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListDataQualityResultsResponseTypeDef = TypedDict(
-    "ListDataQualityResultsResponseTypeDef",
-    {
-        "Results": List[DataQualityResultDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDataQualityResultsRequestRequestTypeDef = TypedDict(
-    "ListDataQualityResultsRequestRequestTypeDef",
-    {
-        "Filter": DataQualityResultFilterCriteriaTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-BatchGetDataQualityResultResponseTypeDef = TypedDict(
-    "BatchGetDataQualityResultResponseTypeDef",
-    {
-        "Results": List[DataQualityResultTypeDef],
-        "ResultsNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDataQualityRuleRecommendationRunsResponseTypeDef = TypedDict(
-    "ListDataQualityRuleRecommendationRunsResponseTypeDef",
-    {
-        "Runs": List[DataQualityRuleRecommendationRunDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDataQualityRuleRecommendationRunsRequestRequestTypeDef = TypedDict(
-    "ListDataQualityRuleRecommendationRunsRequestRequestTypeDef",
-    {
-        "Filter": DataQualityRuleRecommendationRunFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListDataQualityRulesetEvaluationRunsResponseTypeDef = TypedDict(
-    "ListDataQualityRulesetEvaluationRunsResponseTypeDef",
-    {
-        "Runs": List[DataQualityRulesetEvaluationRunDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef = TypedDict(
-    "ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef",
-    {
-        "Filter": DataQualityRulesetEvaluationRunFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
 _RequiredCreateDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatabaseRequestRequestTypeDef",
     {
         "DatabaseInput": DatabaseInputTypeDef,
     },
 )
 _OptionalCreateDatabaseRequestRequestTypeDef = TypedDict(
@@ -9056,21 +7789,19 @@
     {
         "CatalogId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateDatabaseRequestRequestTypeDef(
     _RequiredCreateDatabaseRequestRequestTypeDef, _OptionalCreateDatabaseRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatabaseRequestRequestTypeDef",
     {
         "Name": str,
         "DatabaseInput": DatabaseInputTypeDef,
     },
 )
@@ -9078,21 +7809,19 @@
     "_OptionalUpdateDatabaseRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class UpdateDatabaseRequestRequestTypeDef(
     _RequiredUpdateDatabaseRequestRequestTypeDef, _OptionalUpdateDatabaseRequestRequestTypeDef
 ):
     pass
 
-
 GetDatabaseResponseTypeDef = TypedDict(
     "GetDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -9165,19 +7894,17 @@
         "TableType": str,
         "Parameters": Mapping[str, str],
         "TargetTable": TableIdentifierTypeDef,
     },
     total=False,
 )
 
-
 class TableInputTypeDef(_RequiredTableInputTypeDef, _OptionalTableInputTypeDef):
     pass
 
-
 _RequiredTableTypeDef = TypedDict(
     "_RequiredTableTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalTableTypeDef = TypedDict(
@@ -9202,19 +7929,17 @@
         "TargetTable": TableIdentifierTypeDef,
         "CatalogId": str,
         "VersionId": str,
     },
     total=False,
 )
 
-
 class TableTypeDef(_RequiredTableTypeDef, _OptionalTableTypeDef):
     pass
 
-
 GetSecurityConfigurationResponseTypeDef = TypedDict(
     "GetSecurityConfigurationResponseTypeDef",
     {
         "SecurityConfiguration": SecurityConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -9277,27 +8002,14 @@
         "MySQLCatalogSource": MySQLCatalogSourceTypeDef,
         "OracleSQLCatalogSource": OracleSQLCatalogSourceTypeDef,
         "PostgreSQLCatalogSource": PostgreSQLCatalogSourceTypeDef,
         "MicrosoftSQLServerCatalogTarget": MicrosoftSQLServerCatalogTargetTypeDef,
         "MySQLCatalogTarget": MySQLCatalogTargetTypeDef,
         "OracleSQLCatalogTarget": OracleSQLCatalogTargetTypeDef,
         "PostgreSQLCatalogTarget": PostgreSQLCatalogTargetTypeDef,
-        "DynamicTransform": DynamicTransformTypeDef,
-        "EvaluateDataQuality": EvaluateDataQualityTypeDef,
-        "S3CatalogHudiSource": S3CatalogHudiSourceTypeDef,
-        "CatalogHudiSource": CatalogHudiSourceTypeDef,
-        "S3HudiSource": S3HudiSourceTypeDef,
-        "S3HudiCatalogTarget": S3HudiCatalogTargetTypeDef,
-        "S3HudiDirectTarget": S3HudiDirectTargetTypeDef,
-        "DirectJDBCSource": DirectJDBCSourceTypeDef,
-        "S3CatalogDeltaSource": S3CatalogDeltaSourceTypeDef,
-        "CatalogDeltaSource": CatalogDeltaSourceTypeDef,
-        "S3DeltaSource": S3DeltaSourceTypeDef,
-        "S3DeltaCatalogTarget": S3DeltaCatalogTargetTypeDef,
-        "S3DeltaDirectTarget": S3DeltaDirectTargetTypeDef,
     },
     total=False,
 )
 
 GetMLTaskRunsResponseTypeDef = TypedDict(
     "GetMLTaskRunsResponseTypeDef",
     {
@@ -9386,22 +8098,20 @@
     "_OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class UpdateColumnStatisticsForPartitionRequestRequestTypeDef(
     _RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef,
     _OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "ColumnStatisticsList": Sequence[ColumnStatisticsTypeDef],
     },
@@ -9410,22 +8120,20 @@
     "_OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class UpdateColumnStatisticsForTableRequestRequestTypeDef(
     _RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef,
     _OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredBatchCreatePartitionRequestRequestTypeDef = TypedDict(
     "_RequiredBatchCreatePartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionInputList": Sequence[PartitionInputTypeDef],
     },
@@ -9434,22 +8142,20 @@
     "_OptionalBatchCreatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class BatchCreatePartitionRequestRequestTypeDef(
     _RequiredBatchCreatePartitionRequestRequestTypeDef,
     _OptionalBatchCreatePartitionRequestRequestTypeDef,
 ):
     pass
 
-
 BatchUpdatePartitionRequestEntryTypeDef = TypedDict(
     "BatchUpdatePartitionRequestEntryTypeDef",
     {
         "PartitionValueList": Sequence[str],
         "PartitionInput": PartitionInputTypeDef,
     },
 )
@@ -9466,21 +8172,19 @@
     "_OptionalCreatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class CreatePartitionRequestRequestTypeDef(
     _RequiredCreatePartitionRequestRequestTypeDef, _OptionalCreatePartitionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdatePartitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionValueList": Sequence[str],
         "PartitionInput": PartitionInputTypeDef,
@@ -9490,21 +8194,19 @@
     "_OptionalUpdatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class UpdatePartitionRequestRequestTypeDef(
     _RequiredUpdatePartitionRequestRequestTypeDef, _OptionalUpdatePartitionRequestRequestTypeDef
 ):
     pass
 
-
 BatchGetPartitionResponseTypeDef = TypedDict(
     "BatchGetPartitionResponseTypeDef",
     {
         "Partitions": List[PartitionTypeDef],
         "UnprocessedKeys": List[PartitionValueListTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -9560,21 +8262,19 @@
         "CatalogId": str,
         "PartitionIndexes": Sequence[PartitionIndexTypeDef],
         "TransactionId": str,
     },
     total=False,
 )
 
-
 class CreateTableRequestRequestTypeDef(
     _RequiredCreateTableRequestRequestTypeDef, _OptionalCreateTableRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableInput": TableInputTypeDef,
     },
 )
@@ -9585,21 +8285,19 @@
         "SkipArchive": bool,
         "TransactionId": str,
         "VersionId": str,
     },
     total=False,
 )
 
-
 class UpdateTableRequestRequestTypeDef(
     _RequiredUpdateTableRequestRequestTypeDef, _OptionalUpdateTableRequestRequestTypeDef
 ):
     pass
 
-
 GetTableResponseTypeDef = TypedDict(
     "GetTableResponseTypeDef",
     {
         "Table": TableTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -9672,21 +8370,19 @@
         "CodeGenConfigurationNodes": Mapping[str, CodeGenConfigurationNodeTypeDef],
         "ExecutionClass": ExecutionClassType,
         "SourceControlDetails": SourceControlDetailsTypeDef,
     },
     total=False,
 )
 
-
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
 
-
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "Name": str,
         "Description": str,
         "LogUri": str,
         "Role": str,
@@ -9777,22 +8473,20 @@
     "_OptionalBatchUpdatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-
 class BatchUpdatePartitionRequestRequestTypeDef(
     _RequiredBatchUpdatePartitionRequestRequestTypeDef,
     _OptionalBatchUpdatePartitionRequestRequestTypeDef,
 ):
     pass
 
-
 GetUnfilteredPartitionsMetadataResponseTypeDef = TypedDict(
     "GetUnfilteredPartitionsMetadataResponseTypeDef",
     {
         "UnfilteredPartitions": List[UnfilteredPartitionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-glue-1.26.74/mypy_boto3_glue/type_defs.pyi` & `mypy-boto3-glue-1.26.8/mypy_boto3_glue/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,41 +30,33 @@
     ConnectionTypeType,
     CrawlerHistoryStateType,
     CrawlerLineageSettingsType,
     CrawlerStateType,
     CrawlStateType,
     CsvHeaderOptionType,
     DataFormatType,
-    DataQualityRuleResultStatusType,
     DeleteBehaviorType,
-    DeltaTargetCompressionTypeType,
-    DQStopJobOnFailureTimingType,
-    DQTransformOutputType,
     EnableHybridValuesType,
     ExecutionClassType,
     ExistConditionType,
     FieldNameType,
     FilterLogicalOperatorType,
     FilterOperationType,
     FilterOperatorType,
     FilterValueTypeType,
     GlueRecordTypeType,
-    HudiTargetCompressionTypeType,
-    JDBCConnectionTypeType,
     JDBCDataTypeType,
-    JdbcMetadataEntryType,
     JobBookmarksEncryptionModeType,
     JobRunStateType,
     JoinTypeType,
     LanguageType,
     LastCrawlStatusType,
     LogicalType,
     MLUserDataEncryptionModeStringType,
     NodeTypeType,
-    ParamTypeType,
     ParquetCompressionTypeType,
     PartitionIndexStatusType,
     PermissionType,
     PermissionTypeType,
     PiiTypeType,
     PrincipalTypeType,
     QuoteCharType,
@@ -104,14 +96,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "NotificationPropertyTypeDef",
     "AggregateOperationTypeDef",
     "ApplyMappingTypeDef",
     "AuditContextTypeDef",
     "PartitionValueListTypeDef",
     "BasicCatalogTargetTypeDef",
@@ -120,29 +113,26 @@
     "ErrorDetailTypeDef",
     "BatchDeleteTableRequestRequestTypeDef",
     "BatchDeleteTableVersionRequestRequestTypeDef",
     "BatchGetBlueprintsRequestRequestTypeDef",
     "BatchGetCrawlersRequestRequestTypeDef",
     "BatchGetCustomEntityTypesRequestRequestTypeDef",
     "CustomEntityTypeTypeDef",
-    "BatchGetDataQualityResultRequestRequestTypeDef",
     "BatchGetDevEndpointsRequestRequestTypeDef",
     "DevEndpointTypeDef",
     "BatchGetJobsRequestRequestTypeDef",
     "BatchGetTriggersRequestRequestTypeDef",
     "BatchGetWorkflowsRequestRequestTypeDef",
     "BatchStopJobRunRequestRequestTypeDef",
     "BatchStopJobRunSuccessfulSubmissionTypeDef",
     "BinaryColumnStatisticsDataTypeDef",
     "BlueprintDetailsTypeDef",
     "BlueprintRunTypeDef",
     "LastActiveDefinitionTypeDef",
     "BooleanColumnStatisticsDataTypeDef",
-    "CancelDataQualityRuleRecommendationRunRequestRequestTypeDef",
-    "CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef",
     "CancelMLTaskRunRequestRequestTypeDef",
     "CancelStatementRequestRequestTypeDef",
     "CatalogEntryTypeDef",
     "CatalogImportStatusTypeDef",
     "KafkaStreamingSourceOptionsTypeDef",
     "StreamingDataPreviewOptionsTypeDef",
     "KinesisStreamingSourceOptionsTypeDef",
@@ -151,15 +141,14 @@
     "CatalogTargetTypeDef",
     "CheckSchemaVersionValidityInputRequestTypeDef",
     "CsvClassifierTypeDef",
     "GrokClassifierTypeDef",
     "JsonClassifierTypeDef",
     "XMLClassifierTypeDef",
     "CloudWatchEncryptionTypeDef",
-    "DirectJDBCSourceTypeDef",
     "DropDuplicatesTypeDef",
     "DropFieldsTypeDef",
     "DynamoDBCatalogSourceTypeDef",
     "FillMissingValuesTypeDef",
     "MergeTypeDef",
     "MicrosoftSQLServerCatalogSourceTypeDef",
     "MicrosoftSQLServerCatalogTargetTypeDef",
@@ -209,43 +198,37 @@
     "CrawlsFilterTypeDef",
     "CreateBlueprintRequestRequestTypeDef",
     "CreateCsvClassifierRequestTypeDef",
     "CreateGrokClassifierRequestTypeDef",
     "CreateJsonClassifierRequestTypeDef",
     "CreateXMLClassifierRequestTypeDef",
     "CreateCustomEntityTypeRequestRequestTypeDef",
-    "DataQualityTargetTableTypeDef",
     "CreateDevEndpointRequestRequestTypeDef",
     "ExecutionPropertyTypeDef",
     "JobCommandTypeDef",
     "SourceControlDetailsTypeDef",
     "GlueTableTypeDef",
     "PartitionIndexTypeDef",
     "CreateRegistryInputRequestTypeDef",
     "RegistryIdTypeDef",
     "SessionCommandTypeDef",
     "EventBatchingConditionTypeDef",
     "CreateWorkflowRequestRequestTypeDef",
-    "DQResultsPublishingOptionsTypeDef",
-    "DQStopJobOnFailureOptionsTypeDef",
     "EncryptionAtRestTypeDef",
     "DataLakePrincipalTypeDef",
-    "DataQualityEvaluationRunAdditionalRunOptionsTypeDef",
-    "DataQualityRuleResultTypeDef",
     "DatabaseIdentifierTypeDef",
     "DatatypeTypeDef",
     "DecimalNumberTypeDef",
     "DeleteBlueprintRequestRequestTypeDef",
     "DeleteClassifierRequestRequestTypeDef",
     "DeleteColumnStatisticsForPartitionRequestRequestTypeDef",
     "DeleteColumnStatisticsForTableRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
     "DeleteCrawlerRequestRequestTypeDef",
     "DeleteCustomEntityTypeRequestRequestTypeDef",
-    "DeleteDataQualityRulesetRequestRequestTypeDef",
     "DeleteDatabaseRequestRequestTypeDef",
     "DeleteDevEndpointRequestRequestTypeDef",
     "DeleteJobRequestRequestTypeDef",
     "DeleteMLTransformRequestRequestTypeDef",
     "DeletePartitionIndexRequestRequestTypeDef",
     "DeletePartitionRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
@@ -256,15 +239,14 @@
     "DeleteTableVersionRequestRequestTypeDef",
     "DeleteTriggerRequestRequestTypeDef",
     "DeleteUserDefinedFunctionRequestRequestTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
     "DevEndpointCustomLibrariesTypeDef",
     "DirectSchemaChangePolicyTypeDef",
     "NullCheckBoxListTypeDef",
-    "TransformConfigParameterTypeDef",
     "EdgeTypeDef",
     "JobBookmarksEncryptionTypeDef",
     "S3EncryptionTypeDef",
     "ErrorDetailsTypeDef",
     "ExportLabelsTaskRunPropertiesTypeDef",
     "FilterValueTypeDef",
     "FindMatchesParametersTypeDef",
@@ -281,18 +263,14 @@
     "GetConnectionRequestRequestTypeDef",
     "GetConnectionsFilterTypeDef",
     "GetCrawlerMetricsRequestRequestTypeDef",
     "GetCrawlerRequestRequestTypeDef",
     "GetCrawlersRequestRequestTypeDef",
     "GetCustomEntityTypeRequestRequestTypeDef",
     "GetDataCatalogEncryptionSettingsRequestRequestTypeDef",
-    "GetDataQualityResultRequestRequestTypeDef",
-    "GetDataQualityRuleRecommendationRunRequestRequestTypeDef",
-    "GetDataQualityRulesetEvaluationRunRequestRequestTypeDef",
-    "GetDataQualityRulesetRequestRequestTypeDef",
     "GetDatabaseRequestRequestTypeDef",
     "GetDatabasesRequestRequestTypeDef",
     "GetDataflowGraphRequestRequestTypeDef",
     "GetDevEndpointRequestRequestTypeDef",
     "GetDevEndpointsRequestRequestTypeDef",
     "GetJobBookmarkRequestRequestTypeDef",
     "JobBookmarkEntryTypeDef",
@@ -392,15 +370,14 @@
     "UntagResourceRequestRequestTypeDef",
     "UpdateBlueprintRequestRequestTypeDef",
     "UpdateCsvClassifierRequestTypeDef",
     "UpdateGrokClassifierRequestTypeDef",
     "UpdateJsonClassifierRequestTypeDef",
     "UpdateXMLClassifierRequestTypeDef",
     "UpdateCrawlerScheduleRequestRequestTypeDef",
-    "UpdateDataQualityRulesetRequestRequestTypeDef",
     "UpdateJobFromSourceControlRequestRequestTypeDef",
     "UpdateSourceControlFromJobRequestRequestTypeDef",
     "UpdateWorkflowRequestRequestTypeDef",
     "WorkflowRunStatisticsTypeDef",
     "ActionTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "AggregateTypeDef",
@@ -409,15 +386,14 @@
     "BackfillErrorTypeDef",
     "BatchDeletePartitionRequestRequestTypeDef",
     "BatchGetPartitionRequestRequestTypeDef",
     "CancelMLTaskRunResponseTypeDef",
     "CheckSchemaVersionValidityResponseTypeDef",
     "CreateBlueprintResponseTypeDef",
     "CreateCustomEntityTypeResponseTypeDef",
-    "CreateDataQualityRulesetResponseTypeDef",
     "CreateDevEndpointResponseTypeDef",
     "CreateJobResponseTypeDef",
     "CreateMLTransformResponseTypeDef",
     "CreateRegistryResponseTypeDef",
     "CreateSchemaResponseTypeDef",
     "CreateScriptResponseTypeDef",
     "CreateSecurityConfigurationResponseTypeDef",
@@ -452,27 +428,24 @@
     "PutResourcePolicyResponseTypeDef",
     "PutSchemaVersionMetadataResponseTypeDef",
     "RegisterSchemaVersionResponseTypeDef",
     "RemoveSchemaVersionMetadataResponseTypeDef",
     "ResumeWorkflowRunResponseTypeDef",
     "RunStatementResponseTypeDef",
     "StartBlueprintRunResponseTypeDef",
-    "StartDataQualityRuleRecommendationRunResponseTypeDef",
-    "StartDataQualityRulesetEvaluationRunResponseTypeDef",
     "StartExportLabelsTaskRunResponseTypeDef",
     "StartImportLabelsTaskRunResponseTypeDef",
     "StartJobRunResponseTypeDef",
     "StartMLEvaluationTaskRunResponseTypeDef",
     "StartMLLabelingSetGenerationTaskRunResponseTypeDef",
     "StartTriggerResponseTypeDef",
     "StartWorkflowRunResponseTypeDef",
     "StopSessionResponseTypeDef",
     "StopTriggerResponseTypeDef",
     "UpdateBlueprintResponseTypeDef",
-    "UpdateDataQualityRulesetResponseTypeDef",
     "UpdateJobFromSourceControlResponseTypeDef",
     "UpdateJobResponseTypeDef",
     "UpdateMLTransformResponseTypeDef",
     "UpdateRegistryResponseTypeDef",
     "UpdateSchemaResponseTypeDef",
     "UpdateSourceControlFromJobResponseTypeDef",
     "UpdateWorkflowResponseTypeDef",
@@ -494,60 +467,49 @@
     "GetCatalogImportStatusResponseTypeDef",
     "CatalogKafkaSourceTypeDef",
     "DirectKafkaSourceTypeDef",
     "CatalogKinesisSourceTypeDef",
     "DirectKinesisSourceTypeDef",
     "GovernedCatalogTargetTypeDef",
     "S3CatalogTargetTypeDef",
-    "S3DeltaCatalogTargetTypeDef",
-    "S3HudiCatalogTargetTypeDef",
     "ClassifierTypeDef",
     "CodeGenNodeTypeDef",
     "LocationTypeDef",
     "PredicateTypeDef",
     "FindMatchesMetricsTypeDef",
     "ConnectionInputTypeDef",
     "ConnectionTypeDef",
     "CrawlerNodeDetailsTypeDef",
     "ListCrawlsResponseTypeDef",
     "GetCrawlerMetricsResponseTypeDef",
     "CrawlerTargetsTypeDef",
     "ListCrawlsRequestRequestTypeDef",
     "CreateClassifierRequestRequestTypeDef",
-    "CreateDataQualityRulesetRequestRequestTypeDef",
-    "DataQualityRulesetFilterCriteriaTypeDef",
-    "DataQualityRulesetListDetailsTypeDef",
-    "GetDataQualityRulesetResponseTypeDef",
-    "DataSourceTypeDef",
     "CreatePartitionIndexRequestRequestTypeDef",
     "CreateSchemaInputRequestTypeDef",
     "DeleteRegistryInputRequestTypeDef",
     "GetRegistryInputRequestTypeDef",
     "ListSchemasInputRequestTypeDef",
     "UpdateRegistryInputRequestTypeDef",
     "CreateSessionRequestRequestTypeDef",
     "SessionTypeDef",
-    "EvaluateDataQualityTypeDef",
     "DataCatalogEncryptionSettingsTypeDef",
     "PrincipalPermissionsTypeDef",
     "NullValueFieldTypeDef",
     "DecimalColumnStatisticsDataTypeDef",
     "DeleteSchemaInputRequestTypeDef",
     "DeleteSchemaVersionsInputRequestTypeDef",
     "GetSchemaByDefinitionInputRequestTypeDef",
     "GetSchemaInputRequestTypeDef",
     "ListSchemaVersionsInputRequestTypeDef",
     "RegisterSchemaVersionInputRequestTypeDef",
     "SchemaReferenceTypeDef",
     "UpdateDevEndpointRequestRequestTypeDef",
-    "S3DeltaDirectTargetTypeDef",
     "S3DirectTargetTypeDef",
     "S3GlueParquetTargetTypeDef",
-    "S3HudiDirectTargetTypeDef",
-    "DynamicTransformTypeDef",
     "EncryptionConfigurationTypeDef",
     "SchemaVersionErrorItemTypeDef",
     "FilterExpressionTypeDef",
     "TransformParametersTypeDef",
     "GetClassifiersRequestGetClassifiersPaginateTypeDef",
     "GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef",
     "GetCrawlersRequestGetCrawlersPaginateTypeDef",
@@ -621,28 +583,14 @@
     "CreateConnectionRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "GetConnectionResponseTypeDef",
     "GetConnectionsResponseTypeDef",
     "CrawlerTypeDef",
     "CreateCrawlerRequestRequestTypeDef",
     "UpdateCrawlerRequestRequestTypeDef",
-    "ListDataQualityRulesetsRequestRequestTypeDef",
-    "ListDataQualityRulesetsResponseTypeDef",
-    "DataQualityResultDescriptionTypeDef",
-    "DataQualityResultFilterCriteriaTypeDef",
-    "DataQualityResultTypeDef",
-    "DataQualityRuleRecommendationRunDescriptionTypeDef",
-    "DataQualityRuleRecommendationRunFilterTypeDef",
-    "DataQualityRulesetEvaluationRunDescriptionTypeDef",
-    "DataQualityRulesetEvaluationRunFilterTypeDef",
-    "GetDataQualityResultResponseTypeDef",
-    "GetDataQualityRuleRecommendationRunResponseTypeDef",
-    "GetDataQualityRulesetEvaluationRunResponseTypeDef",
-    "StartDataQualityRuleRecommendationRunRequestRequestTypeDef",
-    "StartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
     "CreateSessionResponseTypeDef",
     "GetSessionResponseTypeDef",
     "ListSessionsResponseTypeDef",
     "GetDataCatalogEncryptionSettingsResponseTypeDef",
     "PutDataCatalogEncryptionSettingsRequestRequestTypeDef",
     "DatabaseInputTypeDef",
     "DatabaseTypeDef",
@@ -653,24 +601,18 @@
     "SecurityConfigurationTypeDef",
     "DeleteSchemaVersionsResponseTypeDef",
     "FilterTypeDef",
     "UpdateMLTransformRequestRequestTypeDef",
     "GetMLTransformsRequestRequestTypeDef",
     "ListMLTransformsRequestRequestTypeDef",
     "AthenaConnectorSourceTypeDef",
-    "CatalogDeltaSourceTypeDef",
-    "CatalogHudiSourceTypeDef",
     "CustomCodeTypeDef",
     "JDBCConnectorSourceTypeDef",
     "JDBCConnectorTargetTypeDef",
-    "S3CatalogDeltaSourceTypeDef",
-    "S3CatalogHudiSourceTypeDef",
     "S3CsvSourceTypeDef",
-    "S3DeltaSourceTypeDef",
-    "S3HudiSourceTypeDef",
     "S3JsonSourceTypeDef",
     "S3ParquetSourceTypeDef",
     "SparkConnectorSourceTypeDef",
     "SparkConnectorTargetTypeDef",
     "SparkSQLTypeDef",
     "GetJobRunResponseTypeDef",
     "GetJobRunsResponseTypeDef",
@@ -692,21 +634,14 @@
     "UpdateTriggerResponseTypeDef",
     "UpdateTriggerRequestRequestTypeDef",
     "GetMLTransformResponseTypeDef",
     "MLTransformTypeDef",
     "BatchGetCrawlersResponseTypeDef",
     "GetCrawlerResponseTypeDef",
     "GetCrawlersResponseTypeDef",
-    "ListDataQualityResultsResponseTypeDef",
-    "ListDataQualityResultsRequestRequestTypeDef",
-    "BatchGetDataQualityResultResponseTypeDef",
-    "ListDataQualityRuleRecommendationRunsResponseTypeDef",
-    "ListDataQualityRuleRecommendationRunsRequestRequestTypeDef",
-    "ListDataQualityRulesetEvaluationRunsResponseTypeDef",
-    "ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef",
     "CreateDatabaseRequestRequestTypeDef",
     "UpdateDatabaseRequestRequestTypeDef",
     "GetDatabaseResponseTypeDef",
     "GetDatabasesResponseTypeDef",
     "ColumnStatisticsTypeDef",
     "PartitionInputTypeDef",
     "PartitionTypeDef",
@@ -836,20 +771,22 @@
     "_OptionalBatchDeleteConnectionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class BatchDeleteConnectionRequestRequestTypeDef(
     _RequiredBatchDeleteConnectionRequestRequestTypeDef,
     _OptionalBatchDeleteConnectionRequestRequestTypeDef,
 ):
     pass
 
+
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
@@ -867,19 +804,21 @@
     {
         "CatalogId": str,
         "TransactionId": str,
     },
     total=False,
 )
 
+
 class BatchDeleteTableRequestRequestTypeDef(
     _RequiredBatchDeleteTableRequestRequestTypeDef, _OptionalBatchDeleteTableRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredBatchDeleteTableVersionRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDeleteTableVersionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "VersionIds": Sequence[str],
     },
@@ -888,20 +827,22 @@
     "_OptionalBatchDeleteTableVersionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class BatchDeleteTableVersionRequestRequestTypeDef(
     _RequiredBatchDeleteTableVersionRequestRequestTypeDef,
     _OptionalBatchDeleteTableVersionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredBatchGetBlueprintsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetBlueprintsRequestRequestTypeDef",
     {
         "Names": Sequence[str],
     },
 )
 _OptionalBatchGetBlueprintsRequestRequestTypeDef = TypedDict(
@@ -909,20 +850,22 @@
     {
         "IncludeBlueprint": bool,
         "IncludeParameterSpec": bool,
     },
     total=False,
 )
 
+
 class BatchGetBlueprintsRequestRequestTypeDef(
     _RequiredBatchGetBlueprintsRequestRequestTypeDef,
     _OptionalBatchGetBlueprintsRequestRequestTypeDef,
 ):
     pass
 
+
 BatchGetCrawlersRequestRequestTypeDef = TypedDict(
     "BatchGetCrawlersRequestRequestTypeDef",
     {
         "CrawlerNames": Sequence[str],
     },
 )
 
@@ -944,23 +887,18 @@
     "_OptionalCustomEntityTypeTypeDef",
     {
         "ContextWords": List[str],
     },
     total=False,
 )
 
+
 class CustomEntityTypeTypeDef(_RequiredCustomEntityTypeTypeDef, _OptionalCustomEntityTypeTypeDef):
     pass
 
-BatchGetDataQualityResultRequestRequestTypeDef = TypedDict(
-    "BatchGetDataQualityResultRequestRequestTypeDef",
-    {
-        "ResultIds": Sequence[str],
-    },
-)
 
 BatchGetDevEndpointsRequestRequestTypeDef = TypedDict(
     "BatchGetDevEndpointsRequestRequestTypeDef",
     {
         "DevEndpointNames": Sequence[str],
     },
 )
@@ -1021,19 +959,21 @@
     "_OptionalBatchGetWorkflowsRequestRequestTypeDef",
     {
         "IncludeGraph": bool,
     },
     total=False,
 )
 
+
 class BatchGetWorkflowsRequestRequestTypeDef(
     _RequiredBatchGetWorkflowsRequestRequestTypeDef, _OptionalBatchGetWorkflowsRequestRequestTypeDef
 ):
     pass
 
+
 BatchStopJobRunRequestRequestTypeDef = TypedDict(
     "BatchStopJobRunRequestRequestTypeDef",
     {
         "JobName": str,
         "JobRunIds": Sequence[str],
     },
 )
@@ -1099,28 +1039,14 @@
     {
         "NumberOfTrues": int,
         "NumberOfFalses": int,
         "NumberOfNulls": int,
     },
 )
 
-CancelDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
-    "CancelDataQualityRuleRecommendationRunRequestRequestTypeDef",
-    {
-        "RunId": str,
-    },
-)
-
-CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
-    "CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef",
-    {
-        "RunId": str,
-    },
-)
-
 CancelMLTaskRunRequestRequestTypeDef = TypedDict(
     "CancelMLTaskRunRequestRequestTypeDef",
     {
         "TransformId": str,
         "TaskRunId": str,
     },
 )
@@ -1136,19 +1062,21 @@
     "_OptionalCancelStatementRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
+
 class CancelStatementRequestRequestTypeDef(
     _RequiredCancelStatementRequestRequestTypeDef, _OptionalCancelStatementRequestRequestTypeDef
 ):
     pass
 
+
 CatalogEntryTypeDef = TypedDict(
     "CatalogEntryTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -1177,17 +1105,14 @@
         "StartingOffsets": str,
         "EndingOffsets": str,
         "PollTimeoutMs": int,
         "NumRetries": int,
         "RetryIntervalMs": int,
         "MaxOffsetsPerTrigger": int,
         "MinPartitions": int,
-        "IncludeHeaders": bool,
-        "AddRecordTimestamp": str,
-        "EmitConsumerLagMetrics": str,
     },
     total=False,
 )
 
 StreamingDataPreviewOptionsTypeDef = TypedDict(
     "StreamingDataPreviewOptionsTypeDef",
     {
@@ -1214,16 +1139,14 @@
         "NumRetries": int,
         "RetryIntervalMs": int,
         "MaxRetryIntervalMs": int,
         "AvoidEmptyBatches": bool,
         "StreamArn": str,
         "RoleArn": str,
         "RoleSessionName": str,
-        "AddRecordTimestamp": str,
-        "EmitConsumerLagMetrics": str,
     },
     total=False,
 )
 
 CatalogSchemaChangePolicyTypeDef = TypedDict(
     "CatalogSchemaChangePolicyTypeDef",
     {
@@ -1255,17 +1178,19 @@
         "ConnectionName": str,
         "EventQueueArn": str,
         "DlqEventQueueArn": str,
     },
     total=False,
 )
 
+
 class CatalogTargetTypeDef(_RequiredCatalogTargetTypeDef, _OptionalCatalogTargetTypeDef):
     pass
 
+
 CheckSchemaVersionValidityInputRequestTypeDef = TypedDict(
     "CheckSchemaVersionValidityInputRequestTypeDef",
     {
         "DataFormat": DataFormatType,
         "SchemaDefinition": str,
     },
 )
@@ -1290,17 +1215,19 @@
         "AllowSingleColumn": bool,
         "CustomDatatypeConfigured": bool,
         "CustomDatatypes": List[str],
     },
     total=False,
 )
 
+
 class CsvClassifierTypeDef(_RequiredCsvClassifierTypeDef, _OptionalCsvClassifierTypeDef):
     pass
 
+
 _RequiredGrokClassifierTypeDef = TypedDict(
     "_RequiredGrokClassifierTypeDef",
     {
         "Name": str,
         "Classification": str,
         "GrokPattern": str,
     },
@@ -1312,17 +1239,19 @@
         "LastUpdated": datetime,
         "Version": int,
         "CustomPatterns": str,
     },
     total=False,
 )
 
+
 class GrokClassifierTypeDef(_RequiredGrokClassifierTypeDef, _OptionalGrokClassifierTypeDef):
     pass
 
+
 _RequiredJsonClassifierTypeDef = TypedDict(
     "_RequiredJsonClassifierTypeDef",
     {
         "Name": str,
         "JsonPath": str,
     },
 )
@@ -1332,17 +1261,19 @@
         "CreationTime": datetime,
         "LastUpdated": datetime,
         "Version": int,
     },
     total=False,
 )
 
+
 class JsonClassifierTypeDef(_RequiredJsonClassifierTypeDef, _OptionalJsonClassifierTypeDef):
     pass
 
+
 _RequiredXMLClassifierTypeDef = TypedDict(
     "_RequiredXMLClassifierTypeDef",
     {
         "Name": str,
         "Classification": str,
     },
 )
@@ -1353,47 +1284,28 @@
         "LastUpdated": datetime,
         "Version": int,
         "RowTag": str,
     },
     total=False,
 )
 
+
 class XMLClassifierTypeDef(_RequiredXMLClassifierTypeDef, _OptionalXMLClassifierTypeDef):
     pass
 
+
 CloudWatchEncryptionTypeDef = TypedDict(
     "CloudWatchEncryptionTypeDef",
     {
         "CloudWatchEncryptionMode": CloudWatchEncryptionModeType,
         "KmsKeyArn": str,
     },
     total=False,
 )
 
-_RequiredDirectJDBCSourceTypeDef = TypedDict(
-    "_RequiredDirectJDBCSourceTypeDef",
-    {
-        "Name": str,
-        "Database": str,
-        "Table": str,
-        "ConnectionName": str,
-        "ConnectionType": JDBCConnectionTypeType,
-    },
-)
-_OptionalDirectJDBCSourceTypeDef = TypedDict(
-    "_OptionalDirectJDBCSourceTypeDef",
-    {
-        "RedshiftTmpDir": str,
-    },
-    total=False,
-)
-
-class DirectJDBCSourceTypeDef(_RequiredDirectJDBCSourceTypeDef, _OptionalDirectJDBCSourceTypeDef):
-    pass
-
 _RequiredDropDuplicatesTypeDef = TypedDict(
     "_RequiredDropDuplicatesTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
     },
 )
@@ -1401,17 +1313,19 @@
     "_OptionalDropDuplicatesTypeDef",
     {
         "Columns": List[List[str]],
     },
     total=False,
 )
 
+
 class DropDuplicatesTypeDef(_RequiredDropDuplicatesTypeDef, _OptionalDropDuplicatesTypeDef):
     pass
 
+
 DropFieldsTypeDef = TypedDict(
     "DropFieldsTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Paths": List[List[str]],
     },
@@ -1438,19 +1352,21 @@
     "_OptionalFillMissingValuesTypeDef",
     {
         "FilledPath": str,
     },
     total=False,
 )
 
+
 class FillMissingValuesTypeDef(
     _RequiredFillMissingValuesTypeDef, _OptionalFillMissingValuesTypeDef
 ):
     pass
 
+
 MergeTypeDef = TypedDict(
     "MergeTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Source": str,
         "PrimaryKeys": List[List[str]],
@@ -1530,17 +1446,19 @@
         "SampleFraction": float,
         "ThresholdFraction": float,
         "MaskValue": str,
     },
     total=False,
 )
 
+
 class PIIDetectionTypeDef(_RequiredPIIDetectionTypeDef, _OptionalPIIDetectionTypeDef):
     pass
 
+
 PostgreSQLCatalogSourceTypeDef = TypedDict(
     "PostgreSQLCatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -1569,17 +1487,19 @@
     {
         "RedshiftTmpDir": str,
         "TmpDirIAMRole": str,
     },
     total=False,
 )
 
+
 class RedshiftSourceTypeDef(_RequiredRedshiftSourceTypeDef, _OptionalRedshiftSourceTypeDef):
     pass
 
+
 RelationalCatalogSourceTypeDef = TypedDict(
     "RelationalCatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -1626,17 +1546,19 @@
     {
         "Topk": int,
         "Prob": float,
     },
     total=False,
 )
 
+
 class SpigotTypeDef(_RequiredSpigotTypeDef, _OptionalSpigotTypeDef):
     pass
 
+
 SplitFieldsTypeDef = TypedDict(
     "SplitFieldsTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Paths": List[List[str]],
     },
@@ -1662,17 +1584,19 @@
     "_OptionalCodeGenEdgeTypeDef",
     {
         "TargetParameter": str,
     },
     total=False,
 )
 
+
 class CodeGenEdgeTypeDef(_RequiredCodeGenEdgeTypeDef, _OptionalCodeGenEdgeTypeDef):
     pass
 
+
 _RequiredCodeGenNodeArgTypeDef = TypedDict(
     "_RequiredCodeGenNodeArgTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -1680,17 +1604,19 @@
     "_OptionalCodeGenNodeArgTypeDef",
     {
         "Param": bool,
     },
     total=False,
 )
 
+
 class CodeGenNodeArgTypeDef(_RequiredCodeGenNodeArgTypeDef, _OptionalCodeGenNodeArgTypeDef):
     pass
 
+
 ColumnImportanceTypeDef = TypedDict(
     "ColumnImportanceTypeDef",
     {
         "ColumnName": str,
         "Importance": float,
     },
     total=False,
@@ -1717,19 +1643,21 @@
     {
         "MinimumValue": datetime,
         "MaximumValue": datetime,
     },
     total=False,
 )
 
+
 class DateColumnStatisticsDataTypeDef(
     _RequiredDateColumnStatisticsDataTypeDef, _OptionalDateColumnStatisticsDataTypeDef
 ):
     pass
 
+
 _RequiredDoubleColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredDoubleColumnStatisticsDataTypeDef",
     {
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
     },
 )
@@ -1738,19 +1666,21 @@
     {
         "MinimumValue": float,
         "MaximumValue": float,
     },
     total=False,
 )
 
+
 class DoubleColumnStatisticsDataTypeDef(
     _RequiredDoubleColumnStatisticsDataTypeDef, _OptionalDoubleColumnStatisticsDataTypeDef
 ):
     pass
 
+
 _RequiredLongColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredLongColumnStatisticsDataTypeDef",
     {
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
     },
 )
@@ -1759,19 +1689,21 @@
     {
         "MinimumValue": int,
         "MaximumValue": int,
     },
     total=False,
 )
 
+
 class LongColumnStatisticsDataTypeDef(
     _RequiredLongColumnStatisticsDataTypeDef, _OptionalLongColumnStatisticsDataTypeDef
 ):
     pass
 
+
 StringColumnStatisticsDataTypeDef = TypedDict(
     "StringColumnStatisticsDataTypeDef",
     {
         "MaximumLength": int,
         "AverageLength": float,
         "NumberOfNulls": int,
         "NumberOfDistinctValues": int,
@@ -1790,17 +1722,19 @@
         "Type": str,
         "Comment": str,
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
+
 class ColumnTypeDef(_RequiredColumnTypeDef, _OptionalColumnTypeDef):
     pass
 
+
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "LogicalOperator": Literal["EQUALS"],
         "JobName": str,
         "State": JobRunStateType,
         "CrawlerName": str,
@@ -1840,19 +1774,21 @@
     "_OptionalConnectionPasswordEncryptionTypeDef",
     {
         "AwsKmsKeyId": str,
     },
     total=False,
 )
 
+
 class ConnectionPasswordEncryptionTypeDef(
     _RequiredConnectionPasswordEncryptionTypeDef, _OptionalConnectionPasswordEncryptionTypeDef
 ):
     pass
 
+
 ConnectionsListTypeDef = TypedDict(
     "ConnectionsListTypeDef",
     {
         "Connections": List[str],
     },
     total=False,
 )
@@ -1904,15 +1840,14 @@
 
 DeltaTargetTypeDef = TypedDict(
     "DeltaTargetTypeDef",
     {
         "DeltaTables": List[str],
         "ConnectionName": str,
         "WriteManifest": bool,
-        "CreateNativeDeltaTable": bool,
     },
     total=False,
 )
 
 DynamoDBTargetTypeDef = TypedDict(
     "DynamoDBTargetTypeDef",
     {
@@ -1925,15 +1860,14 @@
 
 JdbcTargetTypeDef = TypedDict(
     "JdbcTargetTypeDef",
     {
         "ConnectionName": str,
         "Path": str,
         "Exclusions": List[str],
-        "EnableAdditionalMetadata": List[JdbcMetadataEntryType],
     },
     total=False,
 )
 
 MongoDBTargetTypeDef = TypedDict(
     "MongoDBTargetTypeDef",
     {
@@ -2035,19 +1969,21 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateBlueprintRequestRequestTypeDef(
     _RequiredCreateBlueprintRequestRequestTypeDef, _OptionalCreateBlueprintRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateCsvClassifierRequestTypeDef = TypedDict(
     "_RequiredCreateCsvClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateCsvClassifierRequestTypeDef = TypedDict(
@@ -2061,19 +1997,21 @@
         "AllowSingleColumn": bool,
         "CustomDatatypeConfigured": bool,
         "CustomDatatypes": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateCsvClassifierRequestTypeDef(
     _RequiredCreateCsvClassifierRequestTypeDef, _OptionalCreateCsvClassifierRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateGrokClassifierRequestTypeDef = TypedDict(
     "_RequiredCreateGrokClassifierRequestTypeDef",
     {
         "Classification": str,
         "Name": str,
         "GrokPattern": str,
     },
@@ -2082,19 +2020,21 @@
     "_OptionalCreateGrokClassifierRequestTypeDef",
     {
         "CustomPatterns": str,
     },
     total=False,
 )
 
+
 class CreateGrokClassifierRequestTypeDef(
     _RequiredCreateGrokClassifierRequestTypeDef, _OptionalCreateGrokClassifierRequestTypeDef
 ):
     pass
 
+
 CreateJsonClassifierRequestTypeDef = TypedDict(
     "CreateJsonClassifierRequestTypeDef",
     {
         "Name": str,
         "JsonPath": str,
     },
 )
@@ -2110,19 +2050,21 @@
     "_OptionalCreateXMLClassifierRequestTypeDef",
     {
         "RowTag": str,
     },
     total=False,
 )
 
+
 class CreateXMLClassifierRequestTypeDef(
     _RequiredCreateXMLClassifierRequestTypeDef, _OptionalCreateXMLClassifierRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateCustomEntityTypeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCustomEntityTypeRequestRequestTypeDef",
     {
         "Name": str,
         "RegexString": str,
     },
 )
@@ -2130,27 +2072,21 @@
     "_OptionalCreateCustomEntityTypeRequestRequestTypeDef",
     {
         "ContextWords": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateCustomEntityTypeRequestRequestTypeDef(
     _RequiredCreateCustomEntityTypeRequestRequestTypeDef,
     _OptionalCreateCustomEntityTypeRequestRequestTypeDef,
 ):
     pass
 
-DataQualityTargetTableTypeDef = TypedDict(
-    "DataQualityTargetTableTypeDef",
-    {
-        "TableName": str,
-        "DatabaseName": str,
-    },
-)
 
 _RequiredCreateDevEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDevEndpointRequestRequestTypeDef",
     {
         "EndpointName": str,
         "RoleArn": str,
     },
@@ -2171,19 +2107,21 @@
         "SecurityConfiguration": str,
         "Tags": Mapping[str, str],
         "Arguments": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateDevEndpointRequestRequestTypeDef(
     _RequiredCreateDevEndpointRequestRequestTypeDef, _OptionalCreateDevEndpointRequestRequestTypeDef
 ):
     pass
 
+
 ExecutionPropertyTypeDef = TypedDict(
     "ExecutionPropertyTypeDef",
     {
         "MaxConcurrentRuns": int,
     },
     total=False,
 )
@@ -2221,22 +2159,23 @@
     },
 )
 _OptionalGlueTableTypeDef = TypedDict(
     "_OptionalGlueTableTypeDef",
     {
         "CatalogId": str,
         "ConnectionName": str,
-        "AdditionalOptions": Dict[str, str],
     },
     total=False,
 )
 
+
 class GlueTableTypeDef(_RequiredGlueTableTypeDef, _OptionalGlueTableTypeDef):
     pass
 
+
 PartitionIndexTypeDef = TypedDict(
     "PartitionIndexTypeDef",
     {
         "Keys": Sequence[str],
         "IndexName": str,
     },
 )
@@ -2252,19 +2191,21 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateRegistryInputRequestTypeDef(
     _RequiredCreateRegistryInputRequestTypeDef, _OptionalCreateRegistryInputRequestTypeDef
 ):
     pass
 
+
 RegistryIdTypeDef = TypedDict(
     "RegistryIdTypeDef",
     {
         "RegistryName": str,
         "RegistryArn": str,
     },
     total=False,
@@ -2289,19 +2230,21 @@
     "_OptionalEventBatchingConditionTypeDef",
     {
         "BatchWindow": int,
     },
     total=False,
 )
 
+
 class EventBatchingConditionTypeDef(
     _RequiredEventBatchingConditionTypeDef, _OptionalEventBatchingConditionTypeDef
 ):
     pass
 
+
 _RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
@@ -2311,37 +2254,20 @@
         "DefaultRunProperties": Mapping[str, str],
         "Tags": Mapping[str, str],
         "MaxConcurrentRuns": int,
     },
     total=False,
 )
 
+
 class CreateWorkflowRequestRequestTypeDef(
     _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
 ):
     pass
 
-DQResultsPublishingOptionsTypeDef = TypedDict(
-    "DQResultsPublishingOptionsTypeDef",
-    {
-        "EvaluationContext": str,
-        "ResultsS3Prefix": str,
-        "CloudWatchMetricsEnabled": bool,
-        "ResultsPublishingEnabled": bool,
-    },
-    total=False,
-)
-
-DQStopJobOnFailureOptionsTypeDef = TypedDict(
-    "DQStopJobOnFailureOptionsTypeDef",
-    {
-        "StopJobOnFailureTiming": DQStopJobOnFailureTimingType,
-    },
-    total=False,
-)
 
 _RequiredEncryptionAtRestTypeDef = TypedDict(
     "_RequiredEncryptionAtRestTypeDef",
     {
         "CatalogEncryptionMode": CatalogEncryptionModeType,
     },
 )
@@ -2349,45 +2275,27 @@
     "_OptionalEncryptionAtRestTypeDef",
     {
         "SseAwsKmsKeyId": str,
     },
     total=False,
 )
 
+
 class EncryptionAtRestTypeDef(_RequiredEncryptionAtRestTypeDef, _OptionalEncryptionAtRestTypeDef):
     pass
 
+
 DataLakePrincipalTypeDef = TypedDict(
     "DataLakePrincipalTypeDef",
     {
         "DataLakePrincipalIdentifier": str,
     },
     total=False,
 )
 
-DataQualityEvaluationRunAdditionalRunOptionsTypeDef = TypedDict(
-    "DataQualityEvaluationRunAdditionalRunOptionsTypeDef",
-    {
-        "CloudWatchMetricsEnabled": bool,
-        "ResultsS3Prefix": str,
-    },
-    total=False,
-)
-
-DataQualityRuleResultTypeDef = TypedDict(
-    "DataQualityRuleResultTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "EvaluationMessage": str,
-        "Result": DataQualityRuleResultStatusType,
-    },
-    total=False,
-)
-
 DatabaseIdentifierTypeDef = TypedDict(
     "DatabaseIdentifierTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
     },
     total=False,
@@ -2436,20 +2344,22 @@
     "_OptionalDeleteColumnStatisticsForPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeleteColumnStatisticsForPartitionRequestRequestTypeDef(
     _RequiredDeleteColumnStatisticsForPartitionRequestRequestTypeDef,
     _OptionalDeleteColumnStatisticsForPartitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteColumnStatisticsForTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "ColumnName": str,
     },
@@ -2458,79 +2368,78 @@
     "_OptionalDeleteColumnStatisticsForTableRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeleteColumnStatisticsForTableRequestRequestTypeDef(
     _RequiredDeleteColumnStatisticsForTableRequestRequestTypeDef,
     _OptionalDeleteColumnStatisticsForTableRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteConnectionRequestRequestTypeDef",
     {
         "ConnectionName": str,
     },
 )
 _OptionalDeleteConnectionRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteConnectionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeleteConnectionRequestRequestTypeDef(
     _RequiredDeleteConnectionRequestRequestTypeDef, _OptionalDeleteConnectionRequestRequestTypeDef
 ):
     pass
 
+
 DeleteCrawlerRequestRequestTypeDef = TypedDict(
     "DeleteCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
 DeleteCustomEntityTypeRequestRequestTypeDef = TypedDict(
     "DeleteCustomEntityTypeRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DeleteDataQualityRulesetRequestRequestTypeDef = TypedDict(
-    "DeleteDataQualityRulesetRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 _RequiredDeleteDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDatabaseRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDeleteDatabaseRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteDatabaseRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeleteDatabaseRequestRequestTypeDef(
     _RequiredDeleteDatabaseRequestRequestTypeDef, _OptionalDeleteDatabaseRequestRequestTypeDef
 ):
     pass
 
+
 DeleteDevEndpointRequestRequestTypeDef = TypedDict(
     "DeleteDevEndpointRequestRequestTypeDef",
     {
         "EndpointName": str,
     },
 )
 
@@ -2560,20 +2469,22 @@
     "_OptionalDeletePartitionIndexRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeletePartitionIndexRequestRequestTypeDef(
     _RequiredDeletePartitionIndexRequestRequestTypeDef,
     _OptionalDeletePartitionIndexRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeletePartitionRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionValues": Sequence[str],
     },
@@ -2582,19 +2493,21 @@
     "_OptionalDeletePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeletePartitionRequestRequestTypeDef(
     _RequiredDeletePartitionRequestRequestTypeDef, _OptionalDeletePartitionRequestRequestTypeDef
 ):
     pass
 
+
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "PolicyHashCondition": str,
         "ResourceArn": str,
     },
     total=False,
@@ -2627,19 +2540,21 @@
     "_OptionalDeleteSessionRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
+
 class DeleteSessionRequestRequestTypeDef(
     _RequiredDeleteSessionRequestRequestTypeDef, _OptionalDeleteSessionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteTableRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -2648,19 +2563,21 @@
     {
         "CatalogId": str,
         "TransactionId": str,
     },
     total=False,
 )
 
+
 class DeleteTableRequestRequestTypeDef(
     _RequiredDeleteTableRequestRequestTypeDef, _OptionalDeleteTableRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteTableVersionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTableVersionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "VersionId": str,
     },
@@ -2669,20 +2586,22 @@
     "_OptionalDeleteTableVersionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeleteTableVersionRequestRequestTypeDef(
     _RequiredDeleteTableVersionRequestRequestTypeDef,
     _OptionalDeleteTableVersionRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteTriggerRequestRequestTypeDef = TypedDict(
     "DeleteTriggerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -2697,20 +2616,22 @@
     "_OptionalDeleteUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DeleteUserDefinedFunctionRequestRequestTypeDef(
     _RequiredDeleteUserDefinedFunctionRequestRequestTypeDef,
     _OptionalDeleteUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -2740,38 +2661,14 @@
         "IsEmpty": bool,
         "IsNullString": bool,
         "IsNegOne": bool,
     },
     total=False,
 )
 
-_RequiredTransformConfigParameterTypeDef = TypedDict(
-    "_RequiredTransformConfigParameterTypeDef",
-    {
-        "Name": str,
-        "Type": ParamTypeType,
-    },
-)
-_OptionalTransformConfigParameterTypeDef = TypedDict(
-    "_OptionalTransformConfigParameterTypeDef",
-    {
-        "ValidationRule": str,
-        "ValidationMessage": str,
-        "Value": List[str],
-        "ListType": ParamTypeType,
-        "IsOptional": bool,
-    },
-    total=False,
-)
-
-class TransformConfigParameterTypeDef(
-    _RequiredTransformConfigParameterTypeDef, _OptionalTransformConfigParameterTypeDef
-):
-    pass
-
 EdgeTypeDef = TypedDict(
     "EdgeTypeDef",
     {
         "SourceId": str,
         "DestinationId": str,
     },
     total=False,
@@ -2852,19 +2749,21 @@
     {
         "IncludeBlueprint": bool,
         "IncludeParameterSpec": bool,
     },
     total=False,
 )
 
+
 class GetBlueprintRequestRequestTypeDef(
     _RequiredGetBlueprintRequestRequestTypeDef, _OptionalGetBlueprintRequestRequestTypeDef
 ):
     pass
 
+
 GetBlueprintRunRequestRequestTypeDef = TypedDict(
     "GetBlueprintRunRequestRequestTypeDef",
     {
         "BlueprintName": str,
         "RunId": str,
     },
 )
@@ -2880,19 +2779,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetBlueprintRunsRequestRequestTypeDef(
     _RequiredGetBlueprintRunsRequestRequestTypeDef, _OptionalGetBlueprintRunsRequestRequestTypeDef
 ):
     pass
 
+
 GetCatalogImportStatusRequestRequestTypeDef = TypedDict(
     "GetCatalogImportStatusRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
@@ -2936,20 +2837,22 @@
     "_OptionalGetColumnStatisticsForPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class GetColumnStatisticsForPartitionRequestRequestTypeDef(
     _RequiredGetColumnStatisticsForPartitionRequestRequestTypeDef,
     _OptionalGetColumnStatisticsForPartitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
     "_RequiredGetColumnStatisticsForTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "ColumnNames": Sequence[str],
     },
@@ -2958,20 +2861,22 @@
     "_OptionalGetColumnStatisticsForTableRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class GetColumnStatisticsForTableRequestRequestTypeDef(
     _RequiredGetColumnStatisticsForTableRequestRequestTypeDef,
     _OptionalGetColumnStatisticsForTableRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetConnectionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetConnectionRequestRequestTypeDef = TypedDict(
@@ -2979,19 +2884,21 @@
     {
         "CatalogId": str,
         "HidePassword": bool,
     },
     total=False,
 )
 
+
 class GetConnectionRequestRequestTypeDef(
     _RequiredGetConnectionRequestRequestTypeDef, _OptionalGetConnectionRequestRequestTypeDef
 ):
     pass
 
+
 GetConnectionsFilterTypeDef = TypedDict(
     "GetConnectionsFilterTypeDef",
     {
         "MatchCriteria": Sequence[str],
         "ConnectionType": ConnectionTypeType,
     },
     total=False,
@@ -3034,61 +2941,35 @@
     "GetDataCatalogEncryptionSettingsRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
-GetDataQualityResultRequestRequestTypeDef = TypedDict(
-    "GetDataQualityResultRequestRequestTypeDef",
-    {
-        "ResultId": str,
-    },
-)
-
-GetDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
-    "GetDataQualityRuleRecommendationRunRequestRequestTypeDef",
-    {
-        "RunId": str,
-    },
-)
-
-GetDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
-    "GetDataQualityRulesetEvaluationRunRequestRequestTypeDef",
-    {
-        "RunId": str,
-    },
-)
-
-GetDataQualityRulesetRequestRequestTypeDef = TypedDict(
-    "GetDataQualityRulesetRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 _RequiredGetDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredGetDatabaseRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetDatabaseRequestRequestTypeDef = TypedDict(
     "_OptionalGetDatabaseRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class GetDatabaseRequestRequestTypeDef(
     _RequiredGetDatabaseRequestRequestTypeDef, _OptionalGetDatabaseRequestRequestTypeDef
 ):
     pass
 
+
 GetDatabasesRequestRequestTypeDef = TypedDict(
     "GetDatabasesRequestRequestTypeDef",
     {
         "CatalogId": str,
         "NextToken": str,
         "MaxResults": int,
         "ResourceShareType": ResourceShareTypeType,
@@ -3130,19 +3011,21 @@
     "_OptionalGetJobBookmarkRequestRequestTypeDef",
     {
         "RunId": str,
     },
     total=False,
 )
 
+
 class GetJobBookmarkRequestRequestTypeDef(
     _RequiredGetJobBookmarkRequestRequestTypeDef, _OptionalGetJobBookmarkRequestRequestTypeDef
 ):
     pass
 
+
 JobBookmarkEntryTypeDef = TypedDict(
     "JobBookmarkEntryTypeDef",
     {
         "JobName": str,
         "Version": int,
         "Run": int,
         "Attempt": int,
@@ -3171,19 +3054,21 @@
     "_OptionalGetJobRunRequestRequestTypeDef",
     {
         "PredecessorsIncluded": bool,
     },
     total=False,
 )
 
+
 class GetJobRunRequestRequestTypeDef(
     _RequiredGetJobRunRequestRequestTypeDef, _OptionalGetJobRunRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetJobRunsRequestRequestTypeDef = TypedDict(
     "_RequiredGetJobRunsRequestRequestTypeDef",
     {
         "JobName": str,
     },
 )
 _OptionalGetJobRunsRequestRequestTypeDef = TypedDict(
@@ -3191,19 +3076,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetJobRunsRequestRequestTypeDef(
     _RequiredGetJobRunsRequestRequestTypeDef, _OptionalGetJobRunsRequestRequestTypeDef
 ):
     pass
 
+
 GetJobsRequestRequestTypeDef = TypedDict(
     "GetJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -3285,20 +3172,22 @@
     {
         "CatalogId": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetPartitionIndexesRequestRequestTypeDef(
     _RequiredGetPartitionIndexesRequestRequestTypeDef,
     _OptionalGetPartitionIndexesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetPartitionRequestRequestTypeDef = TypedDict(
     "_RequiredGetPartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionValues": Sequence[str],
     },
@@ -3307,19 +3196,21 @@
     "_OptionalGetPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class GetPartitionRequestRequestTypeDef(
     _RequiredGetPartitionRequestRequestTypeDef, _OptionalGetPartitionRequestRequestTypeDef
 ):
     pass
 
+
 SegmentTypeDef = TypedDict(
     "SegmentTypeDef",
     {
         "SegmentNumber": int,
         "TotalSegments": int,
     },
 )
@@ -3387,19 +3278,21 @@
     "_OptionalGetSessionRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
+
 class GetSessionRequestRequestTypeDef(
     _RequiredGetSessionRequestRequestTypeDef, _OptionalGetSessionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetStatementRequestRequestTypeDef = TypedDict(
     "_RequiredGetStatementRequestRequestTypeDef",
     {
         "SessionId": str,
         "Id": int,
     },
 )
@@ -3407,19 +3300,21 @@
     "_OptionalGetStatementRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
+
 class GetStatementRequestRequestTypeDef(
     _RequiredGetStatementRequestRequestTypeDef, _OptionalGetStatementRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetTableRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -3429,19 +3324,21 @@
         "CatalogId": str,
         "TransactionId": str,
         "QueryAsOfTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class GetTableRequestRequestTypeDef(
     _RequiredGetTableRequestRequestTypeDef, _OptionalGetTableRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetTableVersionRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableVersionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -3450,19 +3347,21 @@
     {
         "CatalogId": str,
         "VersionId": str,
     },
     total=False,
 )
 
+
 class GetTableVersionRequestRequestTypeDef(
     _RequiredGetTableVersionRequestRequestTypeDef, _OptionalGetTableVersionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetTableVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableVersionsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -3472,19 +3371,21 @@
         "CatalogId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetTableVersionsRequestRequestTypeDef(
     _RequiredGetTableVersionsRequestRequestTypeDef, _OptionalGetTableVersionsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetTablesRequestRequestTypeDef = TypedDict(
     "_RequiredGetTablesRequestRequestTypeDef",
     {
         "DatabaseName": str,
     },
 )
 _OptionalGetTablesRequestRequestTypeDef = TypedDict(
@@ -3496,19 +3397,21 @@
         "MaxResults": int,
         "TransactionId": str,
         "QueryAsOfTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class GetTablesRequestRequestTypeDef(
     _RequiredGetTablesRequestRequestTypeDef, _OptionalGetTablesRequestRequestTypeDef
 ):
     pass
 
+
 GetTagsRequestRequestTypeDef = TypedDict(
     "GetTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -3540,20 +3443,22 @@
     "_OptionalGetUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class GetUserDefinedFunctionRequestRequestTypeDef(
     _RequiredGetUserDefinedFunctionRequestRequestTypeDef,
     _OptionalGetUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetUserDefinedFunctionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetUserDefinedFunctionsRequestRequestTypeDef",
     {
         "Pattern": str,
     },
 )
 _OptionalGetUserDefinedFunctionsRequestRequestTypeDef = TypedDict(
@@ -3563,39 +3468,43 @@
         "DatabaseName": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetUserDefinedFunctionsRequestRequestTypeDef(
     _RequiredGetUserDefinedFunctionsRequestRequestTypeDef,
     _OptionalGetUserDefinedFunctionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredGetWorkflowRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetWorkflowRequestRequestTypeDef = TypedDict(
     "_OptionalGetWorkflowRequestRequestTypeDef",
     {
         "IncludeGraph": bool,
     },
     total=False,
 )
 
+
 class GetWorkflowRequestRequestTypeDef(
     _RequiredGetWorkflowRequestRequestTypeDef, _OptionalGetWorkflowRequestRequestTypeDef
 ):
     pass
 
+
 GetWorkflowRunPropertiesRequestRequestTypeDef = TypedDict(
     "GetWorkflowRunPropertiesRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
     },
 )
@@ -3611,19 +3520,21 @@
     "_OptionalGetWorkflowRunRequestRequestTypeDef",
     {
         "IncludeGraph": bool,
     },
     total=False,
 )
 
+
 class GetWorkflowRunRequestRequestTypeDef(
     _RequiredGetWorkflowRunRequestRequestTypeDef, _OptionalGetWorkflowRunRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetWorkflowRunsRequestRequestTypeDef = TypedDict(
     "_RequiredGetWorkflowRunsRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetWorkflowRunsRequestRequestTypeDef = TypedDict(
@@ -3632,38 +3543,42 @@
         "IncludeGraph": bool,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetWorkflowRunsRequestRequestTypeDef(
     _RequiredGetWorkflowRunsRequestRequestTypeDef, _OptionalGetWorkflowRunsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGlueStudioSchemaColumnTypeDef = TypedDict(
     "_RequiredGlueStudioSchemaColumnTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGlueStudioSchemaColumnTypeDef = TypedDict(
     "_OptionalGlueStudioSchemaColumnTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
+
 class GlueStudioSchemaColumnTypeDef(
     _RequiredGlueStudioSchemaColumnTypeDef, _OptionalGlueStudioSchemaColumnTypeDef
 ):
     pass
 
+
 S3SourceAdditionalOptionsTypeDef = TypedDict(
     "S3SourceAdditionalOptionsTypeDef",
     {
         "BoundedSize": int,
         "BoundedFiles": int,
     },
     total=False,
@@ -3853,19 +3768,21 @@
     {
         "RequestOrigin": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListStatementsRequestRequestTypeDef(
     _RequiredListStatementsRequestRequestTypeDef, _OptionalListStatementsRequestRequestTypeDef
 ):
     pass
 
+
 ListTriggersRequestRequestTypeDef = TypedDict(
     "ListTriggersRequestRequestTypeDef",
     {
         "NextToken": str,
         "DependentJobName": str,
         "MaxResults": int,
         "Tags": Mapping[str, str],
@@ -3892,19 +3809,21 @@
     "_OptionalMLUserDataEncryptionTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
+
 class MLUserDataEncryptionTypeDef(
     _RequiredMLUserDataEncryptionTypeDef, _OptionalMLUserDataEncryptionTypeDef
 ):
     pass
 
+
 MappingTypeDef = TypedDict(
     "MappingTypeDef",
     {
         "ToKey": str,
         "FromPath": List[str],
         "FromType": str,
         "ToType": str,
@@ -3963,19 +3882,21 @@
         "PolicyHashCondition": str,
         "PolicyExistsCondition": ExistConditionType,
         "EnableHybrid": EnableHybridValuesType,
     },
     total=False,
 )
 
+
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
+
 PutWorkflowRunPropertiesRequestRequestTypeDef = TypedDict(
     "PutWorkflowRunPropertiesRequestRequestTypeDef",
     {
         "Name": str,
         "RunId": str,
         "RunProperties": Mapping[str, str],
     },
@@ -4001,19 +3922,21 @@
     "_OptionalResetJobBookmarkRequestRequestTypeDef",
     {
         "RunId": str,
     },
     total=False,
 )
 
+
 class ResetJobBookmarkRequestRequestTypeDef(
     _RequiredResetJobBookmarkRequestRequestTypeDef, _OptionalResetJobBookmarkRequestRequestTypeDef
 ):
     pass
 
+
 ResourceUriTypeDef = TypedDict(
     "ResourceUriTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "Uri": str,
     },
     total=False,
@@ -4039,19 +3962,21 @@
     "_OptionalRunStatementRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
+
 class RunStatementRequestRequestTypeDef(
     _RequiredRunStatementRequestRequestTypeDef, _OptionalRunStatementRequestRequestTypeDef
 ):
     pass
 
+
 S3DirectSourceAdditionalOptionsTypeDef = TypedDict(
     "S3DirectSourceAdditionalOptionsTypeDef",
     {
         "BoundedSize": int,
         "BoundedFiles": int,
         "EnableSamplePath": bool,
         "SamplePath": str,
@@ -4107,19 +4032,21 @@
     "_OptionalStartBlueprintRunRequestRequestTypeDef",
     {
         "Parameters": str,
     },
     total=False,
 )
 
+
 class StartBlueprintRunRequestRequestTypeDef(
     _RequiredStartBlueprintRunRequestRequestTypeDef, _OptionalStartBlueprintRunRequestRequestTypeDef
 ):
     pass
 
+
 StartCrawlerRequestRequestTypeDef = TypedDict(
     "StartCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -4149,20 +4076,22 @@
     "_OptionalStartImportLabelsTaskRunRequestRequestTypeDef",
     {
         "ReplaceAllLabels": bool,
     },
     total=False,
 )
 
+
 class StartImportLabelsTaskRunRequestRequestTypeDef(
     _RequiredStartImportLabelsTaskRunRequestRequestTypeDef,
     _OptionalStartImportLabelsTaskRunRequestRequestTypeDef,
 ):
     pass
 
+
 StartMLEvaluationTaskRunRequestRequestTypeDef = TypedDict(
     "StartMLEvaluationTaskRunRequestRequestTypeDef",
     {
         "TransformId": str,
     },
 )
 
@@ -4191,19 +4120,21 @@
     "_OptionalStartWorkflowRunRequestRequestTypeDef",
     {
         "RunProperties": Mapping[str, str],
     },
     total=False,
 )
 
+
 class StartWorkflowRunRequestRequestTypeDef(
     _RequiredStartWorkflowRunRequestRequestTypeDef, _OptionalStartWorkflowRunRequestRequestTypeDef
 ):
     pass
 
+
 StartingEventBatchConditionTypeDef = TypedDict(
     "StartingEventBatchConditionTypeDef",
     {
         "BatchSize": int,
         "BatchWindow": int,
     },
     total=False,
@@ -4241,19 +4172,21 @@
     "_OptionalStopSessionRequestRequestTypeDef",
     {
         "RequestOrigin": str,
     },
     total=False,
 )
 
+
 class StopSessionRequestRequestTypeDef(
     _RequiredStopSessionRequestRequestTypeDef, _OptionalStopSessionRequestRequestTypeDef
 ):
     pass
 
+
 StopTriggerRequestRequestTypeDef = TypedDict(
     "StopTriggerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -4302,19 +4235,21 @@
     "_OptionalUpdateBlueprintRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateBlueprintRequestRequestTypeDef(
     _RequiredUpdateBlueprintRequestRequestTypeDef, _OptionalUpdateBlueprintRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateCsvClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateCsvClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateCsvClassifierRequestTypeDef = TypedDict(
@@ -4328,19 +4263,21 @@
         "AllowSingleColumn": bool,
         "CustomDatatypeConfigured": bool,
         "CustomDatatypes": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateCsvClassifierRequestTypeDef(
     _RequiredUpdateCsvClassifierRequestTypeDef, _OptionalUpdateCsvClassifierRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateGrokClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateGrokClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateGrokClassifierRequestTypeDef = TypedDict(
@@ -4349,38 +4286,42 @@
         "Classification": str,
         "GrokPattern": str,
         "CustomPatterns": str,
     },
     total=False,
 )
 
+
 class UpdateGrokClassifierRequestTypeDef(
     _RequiredUpdateGrokClassifierRequestTypeDef, _OptionalUpdateGrokClassifierRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateJsonClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateJsonClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateJsonClassifierRequestTypeDef = TypedDict(
     "_OptionalUpdateJsonClassifierRequestTypeDef",
     {
         "JsonPath": str,
     },
     total=False,
 )
 
+
 class UpdateJsonClassifierRequestTypeDef(
     _RequiredUpdateJsonClassifierRequestTypeDef, _OptionalUpdateJsonClassifierRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateXMLClassifierRequestTypeDef = TypedDict(
     "_RequiredUpdateXMLClassifierRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateXMLClassifierRequestTypeDef = TypedDict(
@@ -4388,60 +4329,42 @@
     {
         "Classification": str,
         "RowTag": str,
     },
     total=False,
 )
 
+
 class UpdateXMLClassifierRequestTypeDef(
     _RequiredUpdateXMLClassifierRequestTypeDef, _OptionalUpdateXMLClassifierRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateCrawlerScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCrawlerScheduleRequestRequestTypeDef",
     {
         "CrawlerName": str,
     },
 )
 _OptionalUpdateCrawlerScheduleRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateCrawlerScheduleRequestRequestTypeDef",
     {
         "Schedule": str,
     },
     total=False,
 )
 
+
 class UpdateCrawlerScheduleRequestRequestTypeDef(
     _RequiredUpdateCrawlerScheduleRequestRequestTypeDef,
     _OptionalUpdateCrawlerScheduleRequestRequestTypeDef,
 ):
     pass
 
-_RequiredUpdateDataQualityRulesetRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDataQualityRulesetRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateDataQualityRulesetRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDataQualityRulesetRequestRequestTypeDef",
-    {
-        "UpdatedName": str,
-        "Description": str,
-        "Ruleset": str,
-    },
-    total=False,
-)
-
-class UpdateDataQualityRulesetRequestRequestTypeDef(
-    _RequiredUpdateDataQualityRulesetRequestRequestTypeDef,
-    _OptionalUpdateDataQualityRulesetRequestRequestTypeDef,
-):
-    pass
 
 UpdateJobFromSourceControlRequestRequestTypeDef = TypedDict(
     "UpdateJobFromSourceControlRequestRequestTypeDef",
     {
         "JobName": str,
         "Provider": SourceControlProviderType,
         "RepositoryName": str,
@@ -4483,19 +4406,21 @@
         "Description": str,
         "DefaultRunProperties": Mapping[str, str],
         "MaxConcurrentRuns": int,
     },
     total=False,
 )
 
+
 class UpdateWorkflowRequestRequestTypeDef(
     _RequiredUpdateWorkflowRequestRequestTypeDef, _OptionalUpdateWorkflowRequestRequestTypeDef
 ):
     pass
 
+
 WorkflowRunStatisticsTypeDef = TypedDict(
     "WorkflowRunStatisticsTypeDef",
     {
         "TotalActions": int,
         "TimeoutActions": int,
         "FailedActions": int,
         "StoppedActions": int,
@@ -4539,19 +4464,21 @@
         "WorkerType": WorkerTypeType,
         "NumberOfWorkers": int,
         "ExecutionClass": ExecutionClassType,
     },
     total=False,
 )
 
+
 class StartJobRunRequestRequestTypeDef(
     _RequiredStartJobRunRequestRequestTypeDef, _OptionalStartJobRunRequestRequestTypeDef
 ):
     pass
 
+
 AggregateTypeDef = TypedDict(
     "AggregateTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Groups": List[List[str]],
         "Aggs": List[AggregateOperationTypeDef],
@@ -4572,20 +4499,22 @@
     "_OptionalGetUnfilteredPartitionMetadataRequestRequestTypeDef",
     {
         "AuditContext": AuditContextTypeDef,
     },
     total=False,
 )
 
+
 class GetUnfilteredPartitionMetadataRequestRequestTypeDef(
     _RequiredGetUnfilteredPartitionMetadataRequestRequestTypeDef,
     _OptionalGetUnfilteredPartitionMetadataRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetUnfilteredTableMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetUnfilteredTableMetadataRequestRequestTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "Name": str,
         "SupportedPermissionTypes": Sequence[PermissionTypeType],
@@ -4595,20 +4524,22 @@
     "_OptionalGetUnfilteredTableMetadataRequestRequestTypeDef",
     {
         "AuditContext": AuditContextTypeDef,
     },
     total=False,
 )
 
+
 class GetUnfilteredTableMetadataRequestRequestTypeDef(
     _RequiredGetUnfilteredTableMetadataRequestRequestTypeDef,
     _OptionalGetUnfilteredTableMetadataRequestRequestTypeDef,
 ):
     pass
 
+
 BackfillErrorTypeDef = TypedDict(
     "BackfillErrorTypeDef",
     {
         "Code": BackfillErrorCodeType,
         "Partitions": List[PartitionValueListTypeDef],
     },
     total=False,
@@ -4626,20 +4557,22 @@
     "_OptionalBatchDeletePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class BatchDeletePartitionRequestRequestTypeDef(
     _RequiredBatchDeletePartitionRequestRequestTypeDef,
     _OptionalBatchDeletePartitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredBatchGetPartitionRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetPartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionsToGet": Sequence[PartitionValueListTypeDef],
     },
@@ -4648,19 +4581,21 @@
     "_OptionalBatchGetPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class BatchGetPartitionRequestRequestTypeDef(
     _RequiredBatchGetPartitionRequestRequestTypeDef, _OptionalBatchGetPartitionRequestRequestTypeDef
 ):
     pass
 
+
 CancelMLTaskRunResponseTypeDef = TypedDict(
     "CancelMLTaskRunResponseTypeDef",
     {
         "TransformId": str,
         "TaskRunId": str,
         "Status": TaskStatusTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -4688,22 +4623,14 @@
     "CreateCustomEntityTypeResponseTypeDef",
     {
         "Name": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateDataQualityRulesetResponseTypeDef = TypedDict(
-    "CreateDataQualityRulesetResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateDevEndpointResponseTypeDef = TypedDict(
     "CreateDevEndpointResponseTypeDef",
     {
         "EndpointName": str,
         "Status": str,
         "SecurityGroupIds": List[str],
         "SubnetId": str,
@@ -5129,30 +5056,14 @@
     "StartBlueprintRunResponseTypeDef",
     {
         "RunId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartDataQualityRuleRecommendationRunResponseTypeDef = TypedDict(
-    "StartDataQualityRuleRecommendationRunResponseTypeDef",
-    {
-        "RunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartDataQualityRulesetEvaluationRunResponseTypeDef = TypedDict(
-    "StartDataQualityRulesetEvaluationRunResponseTypeDef",
-    {
-        "RunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 StartExportLabelsTaskRunResponseTypeDef = TypedDict(
     "StartExportLabelsTaskRunResponseTypeDef",
     {
         "TaskRunId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5225,24 +5136,14 @@
     "UpdateBlueprintResponseTypeDef",
     {
         "Name": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateDataQualityRulesetResponseTypeDef = TypedDict(
-    "UpdateDataQualityRulesetResponseTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "Ruleset": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateJobFromSourceControlResponseTypeDef = TypedDict(
     "UpdateJobFromSourceControlResponseTypeDef",
     {
         "JobName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5464,19 +5365,21 @@
         "DetectSchema": bool,
         "StreamingOptions": KafkaStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
+
 class CatalogKafkaSourceTypeDef(
     _RequiredCatalogKafkaSourceTypeDef, _OptionalCatalogKafkaSourceTypeDef
 ):
     pass
 
+
 _RequiredDirectKafkaSourceTypeDef = TypedDict(
     "_RequiredDirectKafkaSourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDirectKafkaSourceTypeDef = TypedDict(
@@ -5486,19 +5389,21 @@
         "WindowSize": int,
         "DetectSchema": bool,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
+
 class DirectKafkaSourceTypeDef(
     _RequiredDirectKafkaSourceTypeDef, _OptionalDirectKafkaSourceTypeDef
 ):
     pass
 
+
 _RequiredCatalogKinesisSourceTypeDef = TypedDict(
     "_RequiredCatalogKinesisSourceTypeDef",
     {
         "Name": str,
         "Table": str,
         "Database": str,
     },
@@ -5510,19 +5415,21 @@
         "DetectSchema": bool,
         "StreamingOptions": KinesisStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
+
 class CatalogKinesisSourceTypeDef(
     _RequiredCatalogKinesisSourceTypeDef, _OptionalCatalogKinesisSourceTypeDef
 ):
     pass
 
+
 _RequiredDirectKinesisSourceTypeDef = TypedDict(
     "_RequiredDirectKinesisSourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDirectKinesisSourceTypeDef = TypedDict(
@@ -5532,19 +5439,21 @@
         "DetectSchema": bool,
         "StreamingOptions": KinesisStreamingSourceOptionsTypeDef,
         "DataPreviewOptions": StreamingDataPreviewOptionsTypeDef,
     },
     total=False,
 )
 
+
 class DirectKinesisSourceTypeDef(
     _RequiredDirectKinesisSourceTypeDef, _OptionalDirectKinesisSourceTypeDef
 ):
     pass
 
+
 _RequiredGovernedCatalogTargetTypeDef = TypedDict(
     "_RequiredGovernedCatalogTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Table": str,
         "Database": str,
@@ -5555,19 +5464,21 @@
     {
         "PartitionKeys": List[List[str]],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
+
 class GovernedCatalogTargetTypeDef(
     _RequiredGovernedCatalogTargetTypeDef, _OptionalGovernedCatalogTargetTypeDef
 ):
     pass
 
+
 _RequiredS3CatalogTargetTypeDef = TypedDict(
     "_RequiredS3CatalogTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Table": str,
         "Database": str,
@@ -5578,64 +5489,18 @@
     {
         "PartitionKeys": List[List[str]],
         "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
-class S3CatalogTargetTypeDef(_RequiredS3CatalogTargetTypeDef, _OptionalS3CatalogTargetTypeDef):
-    pass
 
-_RequiredS3DeltaCatalogTargetTypeDef = TypedDict(
-    "_RequiredS3DeltaCatalogTargetTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Table": str,
-        "Database": str,
-    },
-)
-_OptionalS3DeltaCatalogTargetTypeDef = TypedDict(
-    "_OptionalS3DeltaCatalogTargetTypeDef",
-    {
-        "PartitionKeys": List[List[str]],
-        "AdditionalOptions": Dict[str, str],
-        "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-class S3DeltaCatalogTargetTypeDef(
-    _RequiredS3DeltaCatalogTargetTypeDef, _OptionalS3DeltaCatalogTargetTypeDef
-):
+class S3CatalogTargetTypeDef(_RequiredS3CatalogTargetTypeDef, _OptionalS3CatalogTargetTypeDef):
     pass
 
-_RequiredS3HudiCatalogTargetTypeDef = TypedDict(
-    "_RequiredS3HudiCatalogTargetTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Table": str,
-        "Database": str,
-        "AdditionalOptions": Dict[str, str],
-    },
-)
-_OptionalS3HudiCatalogTargetTypeDef = TypedDict(
-    "_OptionalS3HudiCatalogTargetTypeDef",
-    {
-        "PartitionKeys": List[List[str]],
-        "SchemaChangePolicy": CatalogSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-class S3HudiCatalogTargetTypeDef(
-    _RequiredS3HudiCatalogTargetTypeDef, _OptionalS3HudiCatalogTargetTypeDef
-):
-    pass
 
 ClassifierTypeDef = TypedDict(
     "ClassifierTypeDef",
     {
         "GrokClassifier": GrokClassifierTypeDef,
         "XMLClassifier": XMLClassifierTypeDef,
         "JsonClassifier": JsonClassifierTypeDef,
@@ -5656,17 +5521,19 @@
     "_OptionalCodeGenNodeTypeDef",
     {
         "LineNumber": int,
     },
     total=False,
 )
 
+
 class CodeGenNodeTypeDef(_RequiredCodeGenNodeTypeDef, _OptionalCodeGenNodeTypeDef):
     pass
 
+
 LocationTypeDef = TypedDict(
     "LocationTypeDef",
     {
         "Jdbc": Sequence[CodeGenNodeArgTypeDef],
         "S3": Sequence[CodeGenNodeArgTypeDef],
         "DynamoDB": Sequence[CodeGenNodeArgTypeDef],
     },
@@ -5709,17 +5576,19 @@
         "Description": str,
         "MatchCriteria": Sequence[str],
         "PhysicalConnectionRequirements": PhysicalConnectionRequirementsTypeDef,
     },
     total=False,
 )
 
+
 class ConnectionInputTypeDef(_RequiredConnectionInputTypeDef, _OptionalConnectionInputTypeDef):
     pass
 
+
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "Name": str,
         "Description": str,
         "ConnectionType": ConnectionTypeType,
         "MatchCriteria": List[str],
@@ -5783,103 +5652,32 @@
         "MaxResults": int,
         "Filters": Sequence[CrawlsFilterTypeDef],
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListCrawlsRequestRequestTypeDef(
     _RequiredListCrawlsRequestRequestTypeDef, _OptionalListCrawlsRequestRequestTypeDef
 ):
     pass
 
+
 CreateClassifierRequestRequestTypeDef = TypedDict(
     "CreateClassifierRequestRequestTypeDef",
     {
         "GrokClassifier": CreateGrokClassifierRequestTypeDef,
         "XMLClassifier": CreateXMLClassifierRequestTypeDef,
         "JsonClassifier": CreateJsonClassifierRequestTypeDef,
         "CsvClassifier": CreateCsvClassifierRequestTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateDataQualityRulesetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDataQualityRulesetRequestRequestTypeDef",
-    {
-        "Name": str,
-        "Ruleset": str,
-    },
-)
-_OptionalCreateDataQualityRulesetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDataQualityRulesetRequestRequestTypeDef",
-    {
-        "Description": str,
-        "Tags": Mapping[str, str],
-        "TargetTable": DataQualityTargetTableTypeDef,
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-class CreateDataQualityRulesetRequestRequestTypeDef(
-    _RequiredCreateDataQualityRulesetRequestRequestTypeDef,
-    _OptionalCreateDataQualityRulesetRequestRequestTypeDef,
-):
-    pass
-
-DataQualityRulesetFilterCriteriaTypeDef = TypedDict(
-    "DataQualityRulesetFilterCriteriaTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "CreatedBefore": Union[datetime, str],
-        "CreatedAfter": Union[datetime, str],
-        "LastModifiedBefore": Union[datetime, str],
-        "LastModifiedAfter": Union[datetime, str],
-        "TargetTable": DataQualityTargetTableTypeDef,
-    },
-    total=False,
-)
-
-DataQualityRulesetListDetailsTypeDef = TypedDict(
-    "DataQualityRulesetListDetailsTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "CreatedOn": datetime,
-        "LastModifiedOn": datetime,
-        "TargetTable": DataQualityTargetTableTypeDef,
-        "RecommendationRunId": str,
-        "RuleCount": int,
-    },
-    total=False,
-)
-
-GetDataQualityRulesetResponseTypeDef = TypedDict(
-    "GetDataQualityRulesetResponseTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "Ruleset": str,
-        "TargetTable": DataQualityTargetTableTypeDef,
-        "CreatedOn": datetime,
-        "LastModifiedOn": datetime,
-        "RecommendationRunId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DataSourceTypeDef = TypedDict(
-    "DataSourceTypeDef",
-    {
-        "GlueTable": GlueTableTypeDef,
-    },
-)
-
 _RequiredCreatePartitionIndexRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePartitionIndexRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionIndex": PartitionIndexTypeDef,
     },
@@ -5888,20 +5686,22 @@
     "_OptionalCreatePartitionIndexRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class CreatePartitionIndexRequestRequestTypeDef(
     _RequiredCreatePartitionIndexRequestRequestTypeDef,
     _OptionalCreatePartitionIndexRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateSchemaInputRequestTypeDef = TypedDict(
     "_RequiredCreateSchemaInputRequestTypeDef",
     {
         "SchemaName": str,
         "DataFormat": DataFormatType,
     },
 )
@@ -5913,19 +5713,21 @@
         "Description": str,
         "Tags": Mapping[str, str],
         "SchemaDefinition": str,
     },
     total=False,
 )
 
+
 class CreateSchemaInputRequestTypeDef(
     _RequiredCreateSchemaInputRequestTypeDef, _OptionalCreateSchemaInputRequestTypeDef
 ):
     pass
 
+
 DeleteRegistryInputRequestTypeDef = TypedDict(
     "DeleteRegistryInputRequestTypeDef",
     {
         "RegistryId": RegistryIdTypeDef,
     },
 )
 
@@ -5977,19 +5779,21 @@
         "GlueVersion": str,
         "Tags": Mapping[str, str],
         "RequestOrigin": str,
     },
     total=False,
 )
 
+
 class CreateSessionRequestRequestTypeDef(
     _RequiredCreateSessionRequestRequestTypeDef, _OptionalCreateSessionRequestRequestTypeDef
 ):
     pass
 
+
 SessionTypeDef = TypedDict(
     "SessionTypeDef",
     {
         "Id": str,
         "CreatedOn": datetime,
         "Status": SessionStatusType,
         "ErrorMessage": str,
@@ -6002,37 +5806,14 @@
         "MaxCapacity": float,
         "SecurityConfiguration": str,
         "GlueVersion": str,
     },
     total=False,
 )
 
-_RequiredEvaluateDataQualityTypeDef = TypedDict(
-    "_RequiredEvaluateDataQualityTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Ruleset": str,
-    },
-)
-_OptionalEvaluateDataQualityTypeDef = TypedDict(
-    "_OptionalEvaluateDataQualityTypeDef",
-    {
-        "Output": DQTransformOutputType,
-        "PublishingOptions": DQResultsPublishingOptionsTypeDef,
-        "StopJobOnFailureOptions": DQStopJobOnFailureOptionsTypeDef,
-    },
-    total=False,
-)
-
-class EvaluateDataQualityTypeDef(
-    _RequiredEvaluateDataQualityTypeDef, _OptionalEvaluateDataQualityTypeDef
-):
-    pass
-
 DataCatalogEncryptionSettingsTypeDef = TypedDict(
     "DataCatalogEncryptionSettingsTypeDef",
     {
         "EncryptionAtRest": EncryptionAtRestTypeDef,
         "ConnectionPasswordEncryption": ConnectionPasswordEncryptionTypeDef,
     },
     total=False,
@@ -6067,19 +5848,21 @@
     {
         "MinimumValue": DecimalNumberTypeDef,
         "MaximumValue": DecimalNumberTypeDef,
     },
     total=False,
 )
 
+
 class DecimalColumnStatisticsDataTypeDef(
     _RequiredDecimalColumnStatisticsDataTypeDef, _OptionalDecimalColumnStatisticsDataTypeDef
 ):
     pass
 
+
 DeleteSchemaInputRequestTypeDef = TypedDict(
     "DeleteSchemaInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
     },
 )
 
@@ -6117,19 +5900,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListSchemaVersionsInputRequestTypeDef(
     _RequiredListSchemaVersionsInputRequestTypeDef, _OptionalListSchemaVersionsInputRequestTypeDef
 ):
     pass
 
+
 RegisterSchemaVersionInputRequestTypeDef = TypedDict(
     "RegisterSchemaVersionInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
         "SchemaDefinition": str,
     },
 )
@@ -6160,43 +5945,20 @@
         "UpdateEtlLibraries": bool,
         "DeleteArguments": Sequence[str],
         "AddArguments": Mapping[str, str],
     },
     total=False,
 )
 
+
 class UpdateDevEndpointRequestRequestTypeDef(
     _RequiredUpdateDevEndpointRequestRequestTypeDef, _OptionalUpdateDevEndpointRequestRequestTypeDef
 ):
     pass
 
-_RequiredS3DeltaDirectTargetTypeDef = TypedDict(
-    "_RequiredS3DeltaDirectTargetTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Path": str,
-        "Compression": DeltaTargetCompressionTypeType,
-        "Format": TargetFormatType,
-    },
-)
-_OptionalS3DeltaDirectTargetTypeDef = TypedDict(
-    "_OptionalS3DeltaDirectTargetTypeDef",
-    {
-        "PartitionKeys": List[List[str]],
-        "AdditionalOptions": Dict[str, str],
-        "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-class S3DeltaDirectTargetTypeDef(
-    _RequiredS3DeltaDirectTargetTypeDef, _OptionalS3DeltaDirectTargetTypeDef
-):
-    pass
 
 _RequiredS3DirectTargetTypeDef = TypedDict(
     "_RequiredS3DirectTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Path": str,
@@ -6209,17 +5971,19 @@
         "PartitionKeys": List[List[str]],
         "Compression": str,
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
+
 class S3DirectTargetTypeDef(_RequiredS3DirectTargetTypeDef, _OptionalS3DirectTargetTypeDef):
     pass
 
+
 _RequiredS3GlueParquetTargetTypeDef = TypedDict(
     "_RequiredS3GlueParquetTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Path": str,
     },
@@ -6230,65 +5994,20 @@
         "PartitionKeys": List[List[str]],
         "Compression": ParquetCompressionTypeType,
         "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
     },
     total=False,
 )
 
+
 class S3GlueParquetTargetTypeDef(
     _RequiredS3GlueParquetTargetTypeDef, _OptionalS3GlueParquetTargetTypeDef
 ):
     pass
 
-_RequiredS3HudiDirectTargetTypeDef = TypedDict(
-    "_RequiredS3HudiDirectTargetTypeDef",
-    {
-        "Name": str,
-        "Inputs": List[str],
-        "Path": str,
-        "Compression": HudiTargetCompressionTypeType,
-        "Format": TargetFormatType,
-        "AdditionalOptions": Dict[str, str],
-    },
-)
-_OptionalS3HudiDirectTargetTypeDef = TypedDict(
-    "_OptionalS3HudiDirectTargetTypeDef",
-    {
-        "PartitionKeys": List[List[str]],
-        "SchemaChangePolicy": DirectSchemaChangePolicyTypeDef,
-    },
-    total=False,
-)
-
-class S3HudiDirectTargetTypeDef(
-    _RequiredS3HudiDirectTargetTypeDef, _OptionalS3HudiDirectTargetTypeDef
-):
-    pass
-
-_RequiredDynamicTransformTypeDef = TypedDict(
-    "_RequiredDynamicTransformTypeDef",
-    {
-        "Name": str,
-        "TransformName": str,
-        "Inputs": List[str],
-        "FunctionName": str,
-        "Path": str,
-    },
-)
-_OptionalDynamicTransformTypeDef = TypedDict(
-    "_OptionalDynamicTransformTypeDef",
-    {
-        "Parameters": List[TransformConfigParameterTypeDef],
-        "Version": str,
-    },
-    total=False,
-)
-
-class DynamicTransformTypeDef(_RequiredDynamicTransformTypeDef, _OptionalDynamicTransformTypeDef):
-    pass
 
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "S3Encryption": Sequence[S3EncryptionTypeDef],
         "CloudWatchEncryption": CloudWatchEncryptionTypeDef,
         "JobBookmarksEncryption": JobBookmarksEncryptionTypeDef,
@@ -6316,36 +6035,40 @@
     "_OptionalFilterExpressionTypeDef",
     {
         "Negated": bool,
     },
     total=False,
 )
 
+
 class FilterExpressionTypeDef(_RequiredFilterExpressionTypeDef, _OptionalFilterExpressionTypeDef):
     pass
 
+
 _RequiredTransformParametersTypeDef = TypedDict(
     "_RequiredTransformParametersTypeDef",
     {
         "TransformType": Literal["FIND_MATCHES"],
     },
 )
 _OptionalTransformParametersTypeDef = TypedDict(
     "_OptionalTransformParametersTypeDef",
     {
         "FindMatchesParameters": FindMatchesParametersTypeDef,
     },
     total=False,
 )
 
+
 class TransformParametersTypeDef(
     _RequiredTransformParametersTypeDef, _OptionalTransformParametersTypeDef
 ):
     pass
 
+
 GetClassifiersRequestGetClassifiersPaginateTypeDef = TypedDict(
     "GetClassifiersRequestGetClassifiersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6395,20 +6118,22 @@
     "_OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetJobRunsRequestGetJobRunsPaginateTypeDef(
     _RequiredGetJobRunsRequestGetJobRunsPaginateTypeDef,
     _OptionalGetJobRunsRequestGetJobRunsPaginateTypeDef,
 ):
     pass
 
+
 GetJobsRequestGetJobsPaginateTypeDef = TypedDict(
     "GetJobsRequestGetJobsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6425,20 +6150,22 @@
     {
         "CatalogId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef(
     _RequiredGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
     _OptionalGetPartitionIndexesRequestGetPartitionIndexesPaginateTypeDef,
 ):
     pass
 
+
 GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef = TypedDict(
     "GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6463,20 +6190,22 @@
     {
         "CatalogId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetTableVersionsRequestGetTableVersionsPaginateTypeDef(
     _RequiredGetTableVersionsRequestGetTableVersionsPaginateTypeDef,
     _OptionalGetTableVersionsRequestGetTableVersionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetTablesRequestGetTablesPaginateTypeDef = TypedDict(
     "_RequiredGetTablesRequestGetTablesPaginateTypeDef",
     {
         "DatabaseName": str,
     },
 )
 _OptionalGetTablesRequestGetTablesPaginateTypeDef = TypedDict(
@@ -6487,20 +6216,22 @@
         "TransactionId": str,
         "QueryAsOfTime": Union[datetime, str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetTablesRequestGetTablesPaginateTypeDef(
     _RequiredGetTablesRequestGetTablesPaginateTypeDef,
     _OptionalGetTablesRequestGetTablesPaginateTypeDef,
 ):
     pass
 
+
 GetTriggersRequestGetTriggersPaginateTypeDef = TypedDict(
     "GetTriggersRequestGetTriggersPaginateTypeDef",
     {
         "DependentJobName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -6518,20 +6249,22 @@
         "CatalogId": str,
         "DatabaseName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef(
     _RequiredGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
     _OptionalGetUserDefinedFunctionsRequestGetUserDefinedFunctionsPaginateTypeDef,
 ):
     pass
 
+
 ListRegistriesInputListRegistriesPaginateTypeDef = TypedDict(
     "ListRegistriesInputListRegistriesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -6546,20 +6279,22 @@
     "_OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListSchemaVersionsInputListSchemaVersionsPaginateTypeDef(
     _RequiredListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
     _OptionalListSchemaVersionsInputListSchemaVersionsPaginateTypeDef,
 ):
     pass
 
+
 ListSchemasInputListSchemasPaginateTypeDef = TypedDict(
     "ListSchemasInputListSchemasPaginateTypeDef",
     {
         "RegistryId": RegistryIdTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -6617,19 +6352,21 @@
         "MaxResults": int,
         "Filter": TaskRunFilterCriteriaTypeDef,
         "Sort": TaskRunSortCriteriaTypeDef,
     },
     total=False,
 )
 
+
 class GetMLTaskRunsRequestRequestTypeDef(
     _RequiredGetMLTaskRunsRequestRequestTypeDef, _OptionalGetMLTaskRunsRequestRequestTypeDef
 ):
     pass
 
+
 TransformFilterCriteriaTypeDef = TypedDict(
     "TransformFilterCriteriaTypeDef",
     {
         "Name": str,
         "TransformType": Literal["FIND_MATCHES"],
         "Status": TransformStatusTypeType,
         "GlueVersion": str,
@@ -6667,20 +6404,22 @@
         "TransactionId": str,
         "QueryAsOfTime": Union[datetime, str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetPartitionsRequestGetPartitionsPaginateTypeDef(
     _RequiredGetPartitionsRequestGetPartitionsPaginateTypeDef,
     _OptionalGetPartitionsRequestGetPartitionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetPartitionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetPartitionsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -6695,19 +6434,21 @@
         "ExcludeColumnSchema": bool,
         "TransactionId": str,
         "QueryAsOfTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class GetPartitionsRequestRequestTypeDef(
     _RequiredGetPartitionsRequestRequestTypeDef, _OptionalGetPartitionsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetUnfilteredPartitionsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetUnfilteredPartitionsMetadataRequestRequestTypeDef",
     {
         "CatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "SupportedPermissionTypes": Sequence[PermissionTypeType],
@@ -6721,20 +6462,22 @@
         "NextToken": str,
         "Segment": SegmentTypeDef,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetUnfilteredPartitionsMetadataRequestRequestTypeDef(
     _RequiredGetUnfilteredPartitionsMetadataRequestRequestTypeDef,
     _OptionalGetUnfilteredPartitionsMetadataRequestRequestTypeDef,
 ):
     pass
 
+
 GetResourcePoliciesResponseTypeDef = TypedDict(
     "GetResourcePoliciesResponseTypeDef",
     {
         "GetResourcePoliciesResponseList": List[GluePolicyTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6772,19 +6515,21 @@
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "Compatibility": CompatibilityType,
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateSchemaInputRequestTypeDef(
     _RequiredUpdateSchemaInputRequestTypeDef, _OptionalUpdateSchemaInputRequestTypeDef
 ):
     pass
 
+
 GlueSchemaTypeDef = TypedDict(
     "GlueSchemaTypeDef",
     {
         "Columns": List[GlueStudioSchemaColumnTypeDef],
     },
     total=False,
 )
@@ -6802,19 +6547,21 @@
     {
         "PartitionPredicate": str,
         "AdditionalOptions": S3SourceAdditionalOptionsTypeDef,
     },
     total=False,
 )
 
+
 class GovernedCatalogSourceTypeDef(
     _RequiredGovernedCatalogSourceTypeDef, _OptionalGovernedCatalogSourceTypeDef
 ):
     pass
 
+
 _RequiredS3CatalogSourceTypeDef = TypedDict(
     "_RequiredS3CatalogSourceTypeDef",
     {
         "Name": str,
         "Database": str,
         "Table": str,
     },
@@ -6824,17 +6571,19 @@
     {
         "PartitionPredicate": str,
         "AdditionalOptions": S3SourceAdditionalOptionsTypeDef,
     },
     total=False,
 )
 
+
 class S3CatalogSourceTypeDef(_RequiredS3CatalogSourceTypeDef, _OptionalS3CatalogSourceTypeDef):
     pass
 
+
 JobRunTypeDef = TypedDict(
     "JobRunTypeDef",
     {
         "Id": str,
         "Attempt": int,
         "PreviousRunId": str,
         "TriggerName": str,
@@ -6942,20 +6691,22 @@
         "SchemaId": SchemaIdTypeDef,
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "SchemaVersionId": str,
     },
     total=False,
 )
 
+
 class PutSchemaVersionMetadataInputRequestTypeDef(
     _RequiredPutSchemaVersionMetadataInputRequestTypeDef,
     _OptionalPutSchemaVersionMetadataInputRequestTypeDef,
 ):
     pass
 
+
 QuerySchemaVersionMetadataInputRequestTypeDef = TypedDict(
     "QuerySchemaVersionMetadataInputRequestTypeDef",
     {
         "SchemaId": SchemaIdTypeDef,
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "SchemaVersionId": str,
         "MetadataList": Sequence[MetadataKeyValuePairTypeDef],
@@ -6977,20 +6728,22 @@
         "SchemaId": SchemaIdTypeDef,
         "SchemaVersionNumber": SchemaVersionNumberTypeDef,
         "SchemaVersionId": str,
     },
     total=False,
 )
 
+
 class RemoveSchemaVersionMetadataInputRequestTypeDef(
     _RequiredRemoveSchemaVersionMetadataInputRequestTypeDef,
     _OptionalRemoveSchemaVersionMetadataInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredRedshiftTargetTypeDef = TypedDict(
     "_RequiredRedshiftTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Database": str,
         "Table": str,
@@ -7002,17 +6755,19 @@
         "RedshiftTmpDir": str,
         "TmpDirIAMRole": str,
         "UpsertRedshiftOptions": UpsertRedshiftTargetOptionsTypeDef,
     },
     total=False,
 )
 
+
 class RedshiftTargetTypeDef(_RequiredRedshiftTargetTypeDef, _OptionalRedshiftTargetTypeDef):
     pass
 
+
 UserDefinedFunctionInputTypeDef = TypedDict(
     "UserDefinedFunctionInputTypeDef",
     {
         "FunctionName": str,
         "ClassName": str,
         "OwnerName": str,
         "OwnerType": PrincipalTypeType,
@@ -7086,19 +6841,21 @@
     "_OptionalPartitionIndexDescriptorTypeDef",
     {
         "BackfillErrors": List[BackfillErrorTypeDef],
     },
     total=False,
 )
 
+
 class PartitionIndexDescriptorTypeDef(
     _RequiredPartitionIndexDescriptorTypeDef, _OptionalPartitionIndexDescriptorTypeDef
 ):
     pass
 
+
 BatchStopJobRunResponseTypeDef = TypedDict(
     "BatchStopJobRunResponseTypeDef",
     {
         "SuccessfulSubmissions": List[BatchStopJobRunSuccessfulSubmissionTypeDef],
         "Errors": List[BatchStopJobRunErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -7208,19 +6965,21 @@
     {
         "Sinks": Sequence[CatalogEntryTypeDef],
         "Location": LocationTypeDef,
     },
     total=False,
 )
 
+
 class GetMappingRequestRequestTypeDef(
     _RequiredGetMappingRequestRequestTypeDef, _OptionalGetMappingRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetPlanRequestRequestTypeDef = TypedDict(
     "_RequiredGetPlanRequestRequestTypeDef",
     {
         "Mapping": Sequence[MappingEntryTypeDef],
         "Source": CatalogEntryTypeDef,
     },
 )
@@ -7231,19 +6990,21 @@
         "Location": LocationTypeDef,
         "Language": LanguageType,
         "AdditionalPlanOptionsMap": Mapping[str, str],
     },
     total=False,
 )
 
+
 class GetPlanRequestRequestTypeDef(
     _RequiredGetPlanRequestRequestTypeDef, _OptionalGetPlanRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateTriggerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTriggerRequestRequestTypeDef",
     {
         "Name": str,
         "Type": TriggerTypeType,
         "Actions": Sequence[ActionTypeDef],
     },
@@ -7258,19 +7019,21 @@
         "StartOnCreation": bool,
         "Tags": Mapping[str, str],
         "EventBatchingCondition": EventBatchingConditionTypeDef,
     },
     total=False,
 )
 
+
 class CreateTriggerRequestRequestTypeDef(
     _RequiredCreateTriggerRequestRequestTypeDef, _OptionalCreateTriggerRequestRequestTypeDef
 ):
     pass
 
+
 TriggerTypeDef = TypedDict(
     "TriggerTypeDef",
     {
         "Name": str,
         "WorkflowName": str,
         "Id": str,
         "Type": TriggerTypeType,
@@ -7307,19 +7070,21 @@
     "_OptionalEvaluationMetricsTypeDef",
     {
         "FindMatchesMetrics": FindMatchesMetricsTypeDef,
     },
     total=False,
 )
 
+
 class EvaluationMetricsTypeDef(
     _RequiredEvaluationMetricsTypeDef, _OptionalEvaluationMetricsTypeDef
 ):
     pass
 
+
 _RequiredCreateConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectionRequestRequestTypeDef",
     {
         "ConnectionInput": ConnectionInputTypeDef,
     },
 )
 _OptionalCreateConnectionRequestRequestTypeDef = TypedDict(
@@ -7327,19 +7092,21 @@
     {
         "CatalogId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateConnectionRequestRequestTypeDef(
     _RequiredCreateConnectionRequestRequestTypeDef, _OptionalCreateConnectionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateConnectionRequestRequestTypeDef",
     {
         "Name": str,
         "ConnectionInput": ConnectionInputTypeDef,
     },
 )
@@ -7347,19 +7114,21 @@
     "_OptionalUpdateConnectionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class UpdateConnectionRequestRequestTypeDef(
     _RequiredUpdateConnectionRequestRequestTypeDef, _OptionalUpdateConnectionRequestRequestTypeDef
 ):
     pass
 
+
 GetConnectionResponseTypeDef = TypedDict(
     "GetConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -7423,19 +7192,21 @@
         "Configuration": str,
         "CrawlerSecurityConfiguration": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateCrawlerRequestRequestTypeDef(
     _RequiredCreateCrawlerRequestRequestTypeDef, _OptionalCreateCrawlerRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateCrawlerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCrawlerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateCrawlerRequestRequestTypeDef = TypedDict(
@@ -7454,252 +7225,20 @@
         "LakeFormationConfiguration": LakeFormationConfigurationTypeDef,
         "Configuration": str,
         "CrawlerSecurityConfiguration": str,
     },
     total=False,
 )
 
+
 class UpdateCrawlerRequestRequestTypeDef(
     _RequiredUpdateCrawlerRequestRequestTypeDef, _OptionalUpdateCrawlerRequestRequestTypeDef
 ):
     pass
 
-ListDataQualityRulesetsRequestRequestTypeDef = TypedDict(
-    "ListDataQualityRulesetsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "MaxResults": int,
-        "Filter": DataQualityRulesetFilterCriteriaTypeDef,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-ListDataQualityRulesetsResponseTypeDef = TypedDict(
-    "ListDataQualityRulesetsResponseTypeDef",
-    {
-        "Rulesets": List[DataQualityRulesetListDetailsTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DataQualityResultDescriptionTypeDef = TypedDict(
-    "DataQualityResultDescriptionTypeDef",
-    {
-        "ResultId": str,
-        "DataSource": DataSourceTypeDef,
-        "JobName": str,
-        "JobRunId": str,
-        "StartedOn": datetime,
-    },
-    total=False,
-)
-
-DataQualityResultFilterCriteriaTypeDef = TypedDict(
-    "DataQualityResultFilterCriteriaTypeDef",
-    {
-        "DataSource": DataSourceTypeDef,
-        "JobName": str,
-        "JobRunId": str,
-        "StartedAfter": Union[datetime, str],
-        "StartedBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
-DataQualityResultTypeDef = TypedDict(
-    "DataQualityResultTypeDef",
-    {
-        "ResultId": str,
-        "Score": float,
-        "DataSource": DataSourceTypeDef,
-        "RulesetName": str,
-        "EvaluationContext": str,
-        "StartedOn": datetime,
-        "CompletedOn": datetime,
-        "JobName": str,
-        "JobRunId": str,
-        "RulesetEvaluationRunId": str,
-        "RuleResults": List[DataQualityRuleResultTypeDef],
-    },
-    total=False,
-)
-
-DataQualityRuleRecommendationRunDescriptionTypeDef = TypedDict(
-    "DataQualityRuleRecommendationRunDescriptionTypeDef",
-    {
-        "RunId": str,
-        "Status": TaskStatusTypeType,
-        "StartedOn": datetime,
-        "DataSource": DataSourceTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDataQualityRuleRecommendationRunFilterTypeDef = TypedDict(
-    "_RequiredDataQualityRuleRecommendationRunFilterTypeDef",
-    {
-        "DataSource": DataSourceTypeDef,
-    },
-)
-_OptionalDataQualityRuleRecommendationRunFilterTypeDef = TypedDict(
-    "_OptionalDataQualityRuleRecommendationRunFilterTypeDef",
-    {
-        "StartedBefore": Union[datetime, str],
-        "StartedAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-class DataQualityRuleRecommendationRunFilterTypeDef(
-    _RequiredDataQualityRuleRecommendationRunFilterTypeDef,
-    _OptionalDataQualityRuleRecommendationRunFilterTypeDef,
-):
-    pass
-
-DataQualityRulesetEvaluationRunDescriptionTypeDef = TypedDict(
-    "DataQualityRulesetEvaluationRunDescriptionTypeDef",
-    {
-        "RunId": str,
-        "Status": TaskStatusTypeType,
-        "StartedOn": datetime,
-        "DataSource": DataSourceTypeDef,
-    },
-    total=False,
-)
-
-_RequiredDataQualityRulesetEvaluationRunFilterTypeDef = TypedDict(
-    "_RequiredDataQualityRulesetEvaluationRunFilterTypeDef",
-    {
-        "DataSource": DataSourceTypeDef,
-    },
-)
-_OptionalDataQualityRulesetEvaluationRunFilterTypeDef = TypedDict(
-    "_OptionalDataQualityRulesetEvaluationRunFilterTypeDef",
-    {
-        "StartedBefore": Union[datetime, str],
-        "StartedAfter": Union[datetime, str],
-    },
-    total=False,
-)
-
-class DataQualityRulesetEvaluationRunFilterTypeDef(
-    _RequiredDataQualityRulesetEvaluationRunFilterTypeDef,
-    _OptionalDataQualityRulesetEvaluationRunFilterTypeDef,
-):
-    pass
-
-GetDataQualityResultResponseTypeDef = TypedDict(
-    "GetDataQualityResultResponseTypeDef",
-    {
-        "ResultId": str,
-        "Score": float,
-        "DataSource": DataSourceTypeDef,
-        "RulesetName": str,
-        "EvaluationContext": str,
-        "StartedOn": datetime,
-        "CompletedOn": datetime,
-        "JobName": str,
-        "JobRunId": str,
-        "RulesetEvaluationRunId": str,
-        "RuleResults": List[DataQualityRuleResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDataQualityRuleRecommendationRunResponseTypeDef = TypedDict(
-    "GetDataQualityRuleRecommendationRunResponseTypeDef",
-    {
-        "RunId": str,
-        "DataSource": DataSourceTypeDef,
-        "Role": str,
-        "NumberOfWorkers": int,
-        "Timeout": int,
-        "Status": TaskStatusTypeType,
-        "ErrorString": str,
-        "StartedOn": datetime,
-        "LastModifiedOn": datetime,
-        "CompletedOn": datetime,
-        "ExecutionTime": int,
-        "RecommendedRuleset": str,
-        "CreatedRulesetName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDataQualityRulesetEvaluationRunResponseTypeDef = TypedDict(
-    "GetDataQualityRulesetEvaluationRunResponseTypeDef",
-    {
-        "RunId": str,
-        "DataSource": DataSourceTypeDef,
-        "Role": str,
-        "NumberOfWorkers": int,
-        "Timeout": int,
-        "AdditionalRunOptions": DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
-        "Status": TaskStatusTypeType,
-        "ErrorString": str,
-        "StartedOn": datetime,
-        "LastModifiedOn": datetime,
-        "CompletedOn": datetime,
-        "ExecutionTime": int,
-        "RulesetNames": List[str],
-        "ResultIds": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
-    "_RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef",
-    {
-        "DataSource": DataSourceTypeDef,
-        "Role": str,
-    },
-)
-_OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef = TypedDict(
-    "_OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef",
-    {
-        "NumberOfWorkers": int,
-        "Timeout": int,
-        "CreatedRulesetName": str,
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-class StartDataQualityRuleRecommendationRunRequestRequestTypeDef(
-    _RequiredStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
-    _OptionalStartDataQualityRuleRecommendationRunRequestRequestTypeDef,
-):
-    pass
-
-_RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
-    "_RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
-    {
-        "DataSource": DataSourceTypeDef,
-        "Role": str,
-        "RulesetNames": Sequence[str],
-    },
-)
-_OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef = TypedDict(
-    "_OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef",
-    {
-        "NumberOfWorkers": int,
-        "Timeout": int,
-        "ClientToken": str,
-        "AdditionalRunOptions": DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
-    },
-    total=False,
-)
-
-class StartDataQualityRulesetEvaluationRunRequestRequestTypeDef(
-    _RequiredStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
-    _OptionalStartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
-):
-    pass
 
 CreateSessionResponseTypeDef = TypedDict(
     "CreateSessionResponseTypeDef",
     {
         "Session": SessionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -7741,20 +7280,22 @@
     "_OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class PutDataCatalogEncryptionSettingsRequestRequestTypeDef(
     _RequiredPutDataCatalogEncryptionSettingsRequestRequestTypeDef,
     _OptionalPutDataCatalogEncryptionSettingsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDatabaseInputTypeDef = TypedDict(
     "_RequiredDatabaseInputTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDatabaseInputTypeDef = TypedDict(
@@ -7765,17 +7306,19 @@
         "Parameters": Mapping[str, str],
         "CreateTableDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
         "TargetDatabase": DatabaseIdentifierTypeDef,
     },
     total=False,
 )
 
+
 class DatabaseInputTypeDef(_RequiredDatabaseInputTypeDef, _OptionalDatabaseInputTypeDef):
     pass
 
+
 _RequiredDatabaseTypeDef = TypedDict(
     "_RequiredDatabaseTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDatabaseTypeDef = TypedDict(
@@ -7788,17 +7331,19 @@
         "CreateTableDefaultPermissions": List[PrincipalPermissionsTypeDef],
         "TargetDatabase": DatabaseIdentifierTypeDef,
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class DatabaseTypeDef(_RequiredDatabaseTypeDef, _OptionalDatabaseTypeDef):
     pass
 
+
 _RequiredDropNullFieldsTypeDef = TypedDict(
     "_RequiredDropNullFieldsTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
     },
 )
@@ -7807,17 +7352,19 @@
     {
         "NullCheckBoxList": NullCheckBoxListTypeDef,
         "NullTextList": List[NullValueFieldTypeDef],
     },
     total=False,
 )
 
+
 class DropNullFieldsTypeDef(_RequiredDropNullFieldsTypeDef, _OptionalDropNullFieldsTypeDef):
     pass
 
+
 _RequiredColumnStatisticsDataTypeDef = TypedDict(
     "_RequiredColumnStatisticsDataTypeDef",
     {
         "Type": ColumnStatisticsTypeType,
     },
 )
 _OptionalColumnStatisticsDataTypeDef = TypedDict(
@@ -7830,19 +7377,21 @@
         "LongColumnStatisticsData": LongColumnStatisticsDataTypeDef,
         "StringColumnStatisticsData": StringColumnStatisticsDataTypeDef,
         "BinaryColumnStatisticsData": BinaryColumnStatisticsDataTypeDef,
     },
     total=False,
 )
 
+
 class ColumnStatisticsDataTypeDef(
     _RequiredColumnStatisticsDataTypeDef, _OptionalColumnStatisticsDataTypeDef
 ):
     pass
 
+
 StorageDescriptorTypeDef = TypedDict(
     "StorageDescriptorTypeDef",
     {
         "Columns": Sequence[ColumnTypeDef],
         "Location": str,
         "AdditionalLocations": Sequence[str],
         "InputFormat": str,
@@ -7915,19 +7464,21 @@
         "NumberOfWorkers": int,
         "Timeout": int,
         "MaxRetries": int,
     },
     total=False,
 )
 
+
 class UpdateMLTransformRequestRequestTypeDef(
     _RequiredUpdateMLTransformRequestRequestTypeDef, _OptionalUpdateMLTransformRequestRequestTypeDef
 ):
     pass
 
+
 GetMLTransformsRequestRequestTypeDef = TypedDict(
     "GetMLTransformsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filter": TransformFilterCriteriaTypeDef,
         "Sort": TransformSortCriteriaTypeDef,
@@ -7962,62 +7513,20 @@
     {
         "ConnectionTable": str,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class AthenaConnectorSourceTypeDef(
     _RequiredAthenaConnectorSourceTypeDef, _OptionalAthenaConnectorSourceTypeDef
 ):
     pass
 
-_RequiredCatalogDeltaSourceTypeDef = TypedDict(
-    "_RequiredCatalogDeltaSourceTypeDef",
-    {
-        "Name": str,
-        "Database": str,
-        "Table": str,
-    },
-)
-_OptionalCatalogDeltaSourceTypeDef = TypedDict(
-    "_OptionalCatalogDeltaSourceTypeDef",
-    {
-        "AdditionalDeltaOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaTypeDef],
-    },
-    total=False,
-)
-
-class CatalogDeltaSourceTypeDef(
-    _RequiredCatalogDeltaSourceTypeDef, _OptionalCatalogDeltaSourceTypeDef
-):
-    pass
-
-_RequiredCatalogHudiSourceTypeDef = TypedDict(
-    "_RequiredCatalogHudiSourceTypeDef",
-    {
-        "Name": str,
-        "Database": str,
-        "Table": str,
-    },
-)
-_OptionalCatalogHudiSourceTypeDef = TypedDict(
-    "_OptionalCatalogHudiSourceTypeDef",
-    {
-        "AdditionalHudiOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaTypeDef],
-    },
-    total=False,
-)
-
-class CatalogHudiSourceTypeDef(
-    _RequiredCatalogHudiSourceTypeDef, _OptionalCatalogHudiSourceTypeDef
-):
-    pass
 
 _RequiredCustomCodeTypeDef = TypedDict(
     "_RequiredCustomCodeTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "Code": str,
@@ -8028,17 +7537,19 @@
     "_OptionalCustomCodeTypeDef",
     {
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class CustomCodeTypeDef(_RequiredCustomCodeTypeDef, _OptionalCustomCodeTypeDef):
     pass
 
+
 _RequiredJDBCConnectorSourceTypeDef = TypedDict(
     "_RequiredJDBCConnectorSourceTypeDef",
     {
         "Name": str,
         "ConnectionName": str,
         "ConnectorName": str,
         "ConnectionType": str,
@@ -8051,19 +7562,21 @@
         "ConnectionTable": str,
         "Query": str,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class JDBCConnectorSourceTypeDef(
     _RequiredJDBCConnectorSourceTypeDef, _OptionalJDBCConnectorSourceTypeDef
 ):
     pass
 
+
 _RequiredJDBCConnectorTargetTypeDef = TypedDict(
     "_RequiredJDBCConnectorTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "ConnectionName": str,
         "ConnectionTable": str,
@@ -8076,62 +7589,20 @@
     {
         "AdditionalOptions": Dict[str, str],
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class JDBCConnectorTargetTypeDef(
     _RequiredJDBCConnectorTargetTypeDef, _OptionalJDBCConnectorTargetTypeDef
 ):
     pass
 
-_RequiredS3CatalogDeltaSourceTypeDef = TypedDict(
-    "_RequiredS3CatalogDeltaSourceTypeDef",
-    {
-        "Name": str,
-        "Database": str,
-        "Table": str,
-    },
-)
-_OptionalS3CatalogDeltaSourceTypeDef = TypedDict(
-    "_OptionalS3CatalogDeltaSourceTypeDef",
-    {
-        "AdditionalDeltaOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaTypeDef],
-    },
-    total=False,
-)
-
-class S3CatalogDeltaSourceTypeDef(
-    _RequiredS3CatalogDeltaSourceTypeDef, _OptionalS3CatalogDeltaSourceTypeDef
-):
-    pass
-
-_RequiredS3CatalogHudiSourceTypeDef = TypedDict(
-    "_RequiredS3CatalogHudiSourceTypeDef",
-    {
-        "Name": str,
-        "Database": str,
-        "Table": str,
-    },
-)
-_OptionalS3CatalogHudiSourceTypeDef = TypedDict(
-    "_OptionalS3CatalogHudiSourceTypeDef",
-    {
-        "AdditionalHudiOptions": Dict[str, str],
-        "OutputSchemas": List[GlueSchemaTypeDef],
-    },
-    total=False,
-)
-
-class S3CatalogHudiSourceTypeDef(
-    _RequiredS3CatalogHudiSourceTypeDef, _OptionalS3CatalogHudiSourceTypeDef
-):
-    pass
 
 _RequiredS3CsvSourceTypeDef = TypedDict(
     "_RequiredS3CsvSourceTypeDef",
     {
         "Name": str,
         "Paths": List[str],
         "Separator": SeparatorType,
@@ -8156,56 +7627,18 @@
         "SkipFirst": bool,
         "OptimizePerformance": bool,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
-class S3CsvSourceTypeDef(_RequiredS3CsvSourceTypeDef, _OptionalS3CsvSourceTypeDef):
-    pass
 
-_RequiredS3DeltaSourceTypeDef = TypedDict(
-    "_RequiredS3DeltaSourceTypeDef",
-    {
-        "Name": str,
-        "Paths": List[str],
-    },
-)
-_OptionalS3DeltaSourceTypeDef = TypedDict(
-    "_OptionalS3DeltaSourceTypeDef",
-    {
-        "AdditionalDeltaOptions": Dict[str, str],
-        "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "OutputSchemas": List[GlueSchemaTypeDef],
-    },
-    total=False,
-)
-
-class S3DeltaSourceTypeDef(_RequiredS3DeltaSourceTypeDef, _OptionalS3DeltaSourceTypeDef):
+class S3CsvSourceTypeDef(_RequiredS3CsvSourceTypeDef, _OptionalS3CsvSourceTypeDef):
     pass
 
-_RequiredS3HudiSourceTypeDef = TypedDict(
-    "_RequiredS3HudiSourceTypeDef",
-    {
-        "Name": str,
-        "Paths": List[str],
-    },
-)
-_OptionalS3HudiSourceTypeDef = TypedDict(
-    "_OptionalS3HudiSourceTypeDef",
-    {
-        "AdditionalHudiOptions": Dict[str, str],
-        "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
-        "OutputSchemas": List[GlueSchemaTypeDef],
-    },
-    total=False,
-)
-
-class S3HudiSourceTypeDef(_RequiredS3HudiSourceTypeDef, _OptionalS3HudiSourceTypeDef):
-    pass
 
 _RequiredS3JsonSourceTypeDef = TypedDict(
     "_RequiredS3JsonSourceTypeDef",
     {
         "Name": str,
         "Paths": List[str],
     },
@@ -8224,17 +7657,19 @@
         "JsonPath": str,
         "Multiline": bool,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class S3JsonSourceTypeDef(_RequiredS3JsonSourceTypeDef, _OptionalS3JsonSourceTypeDef):
     pass
 
+
 _RequiredS3ParquetSourceTypeDef = TypedDict(
     "_RequiredS3ParquetSourceTypeDef",
     {
         "Name": str,
         "Paths": List[str],
     },
 )
@@ -8250,17 +7685,19 @@
         "MaxFilesInBand": int,
         "AdditionalOptions": S3DirectSourceAdditionalOptionsTypeDef,
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class S3ParquetSourceTypeDef(_RequiredS3ParquetSourceTypeDef, _OptionalS3ParquetSourceTypeDef):
     pass
 
+
 _RequiredSparkConnectorSourceTypeDef = TypedDict(
     "_RequiredSparkConnectorSourceTypeDef",
     {
         "Name": str,
         "ConnectionName": str,
         "ConnectorName": str,
         "ConnectionType": str,
@@ -8271,19 +7708,21 @@
     {
         "AdditionalOptions": Dict[str, str],
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class SparkConnectorSourceTypeDef(
     _RequiredSparkConnectorSourceTypeDef, _OptionalSparkConnectorSourceTypeDef
 ):
     pass
 
+
 _RequiredSparkConnectorTargetTypeDef = TypedDict(
     "_RequiredSparkConnectorTargetTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "ConnectionName": str,
         "ConnectorName": str,
@@ -8295,19 +7734,21 @@
     {
         "AdditionalOptions": Dict[str, str],
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class SparkConnectorTargetTypeDef(
     _RequiredSparkConnectorTargetTypeDef, _OptionalSparkConnectorTargetTypeDef
 ):
     pass
 
+
 _RequiredSparkSQLTypeDef = TypedDict(
     "_RequiredSparkSQLTypeDef",
     {
         "Name": str,
         "Inputs": List[str],
         "SqlQuery": str,
         "SqlAliases": List[SqlAliasTypeDef],
@@ -8317,17 +7758,19 @@
     "_OptionalSparkSQLTypeDef",
     {
         "OutputSchemas": List[GlueSchemaTypeDef],
     },
     total=False,
 )
 
+
 class SparkSQLTypeDef(_RequiredSparkSQLTypeDef, _OptionalSparkSQLTypeDef):
     pass
 
+
 GetJobRunResponseTypeDef = TypedDict(
     "GetJobRunResponseTypeDef",
     {
         "JobRun": JobRunTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -8404,19 +7847,21 @@
         "MaxRetries": int,
         "Tags": Mapping[str, str],
         "TransformEncryption": TransformEncryptionTypeDef,
     },
     total=False,
 )
 
+
 class CreateMLTransformRequestRequestTypeDef(
     _RequiredCreateMLTransformRequestRequestTypeDef, _OptionalCreateMLTransformRequestRequestTypeDef
 ):
     pass
 
+
 QuerySchemaVersionMetadataResponseTypeDef = TypedDict(
     "QuerySchemaVersionMetadataResponseTypeDef",
     {
         "MetadataInfoMap": Dict[str, MetadataInfoTypeDef],
         "SchemaVersionId": str,
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -8434,20 +7879,22 @@
     "_OptionalCreateUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class CreateUserDefinedFunctionRequestRequestTypeDef(
     _RequiredCreateUserDefinedFunctionRequestRequestTypeDef,
     _OptionalCreateUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateUserDefinedFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserDefinedFunctionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "FunctionName": str,
         "FunctionInput": UserDefinedFunctionInputTypeDef,
     },
@@ -8456,20 +7903,22 @@
     "_OptionalUpdateUserDefinedFunctionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class UpdateUserDefinedFunctionRequestRequestTypeDef(
     _RequiredUpdateUserDefinedFunctionRequestRequestTypeDef,
     _OptionalUpdateUserDefinedFunctionRequestRequestTypeDef,
 ):
     pass
 
+
 GetUserDefinedFunctionResponseTypeDef = TypedDict(
     "GetUserDefinedFunctionResponseTypeDef",
     {
         "UserDefinedFunction": UserDefinedFunctionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -8630,80 +8079,14 @@
     {
         "Crawlers": List[CrawlerTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListDataQualityResultsResponseTypeDef = TypedDict(
-    "ListDataQualityResultsResponseTypeDef",
-    {
-        "Results": List[DataQualityResultDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDataQualityResultsRequestRequestTypeDef = TypedDict(
-    "ListDataQualityResultsRequestRequestTypeDef",
-    {
-        "Filter": DataQualityResultFilterCriteriaTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-BatchGetDataQualityResultResponseTypeDef = TypedDict(
-    "BatchGetDataQualityResultResponseTypeDef",
-    {
-        "Results": List[DataQualityResultTypeDef],
-        "ResultsNotFound": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDataQualityRuleRecommendationRunsResponseTypeDef = TypedDict(
-    "ListDataQualityRuleRecommendationRunsResponseTypeDef",
-    {
-        "Runs": List[DataQualityRuleRecommendationRunDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDataQualityRuleRecommendationRunsRequestRequestTypeDef = TypedDict(
-    "ListDataQualityRuleRecommendationRunsRequestRequestTypeDef",
-    {
-        "Filter": DataQualityRuleRecommendationRunFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-ListDataQualityRulesetEvaluationRunsResponseTypeDef = TypedDict(
-    "ListDataQualityRulesetEvaluationRunsResponseTypeDef",
-    {
-        "Runs": List[DataQualityRulesetEvaluationRunDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef = TypedDict(
-    "ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef",
-    {
-        "Filter": DataQualityRulesetEvaluationRunFilterTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
 _RequiredCreateDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatabaseRequestRequestTypeDef",
     {
         "DatabaseInput": DatabaseInputTypeDef,
     },
 )
 _OptionalCreateDatabaseRequestRequestTypeDef = TypedDict(
@@ -8711,19 +8094,21 @@
     {
         "CatalogId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateDatabaseRequestRequestTypeDef(
     _RequiredCreateDatabaseRequestRequestTypeDef, _OptionalCreateDatabaseRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatabaseRequestRequestTypeDef",
     {
         "Name": str,
         "DatabaseInput": DatabaseInputTypeDef,
     },
 )
@@ -8731,19 +8116,21 @@
     "_OptionalUpdateDatabaseRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class UpdateDatabaseRequestRequestTypeDef(
     _RequiredUpdateDatabaseRequestRequestTypeDef, _OptionalUpdateDatabaseRequestRequestTypeDef
 ):
     pass
 
+
 GetDatabaseResponseTypeDef = TypedDict(
     "GetDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -8816,17 +8203,19 @@
         "TableType": str,
         "Parameters": Mapping[str, str],
         "TargetTable": TableIdentifierTypeDef,
     },
     total=False,
 )
 
+
 class TableInputTypeDef(_RequiredTableInputTypeDef, _OptionalTableInputTypeDef):
     pass
 
+
 _RequiredTableTypeDef = TypedDict(
     "_RequiredTableTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalTableTypeDef = TypedDict(
@@ -8851,17 +8240,19 @@
         "TargetTable": TableIdentifierTypeDef,
         "CatalogId": str,
         "VersionId": str,
     },
     total=False,
 )
 
+
 class TableTypeDef(_RequiredTableTypeDef, _OptionalTableTypeDef):
     pass
 
+
 GetSecurityConfigurationResponseTypeDef = TypedDict(
     "GetSecurityConfigurationResponseTypeDef",
     {
         "SecurityConfiguration": SecurityConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -8924,27 +8315,14 @@
         "MySQLCatalogSource": MySQLCatalogSourceTypeDef,
         "OracleSQLCatalogSource": OracleSQLCatalogSourceTypeDef,
         "PostgreSQLCatalogSource": PostgreSQLCatalogSourceTypeDef,
         "MicrosoftSQLServerCatalogTarget": MicrosoftSQLServerCatalogTargetTypeDef,
         "MySQLCatalogTarget": MySQLCatalogTargetTypeDef,
         "OracleSQLCatalogTarget": OracleSQLCatalogTargetTypeDef,
         "PostgreSQLCatalogTarget": PostgreSQLCatalogTargetTypeDef,
-        "DynamicTransform": DynamicTransformTypeDef,
-        "EvaluateDataQuality": EvaluateDataQualityTypeDef,
-        "S3CatalogHudiSource": S3CatalogHudiSourceTypeDef,
-        "CatalogHudiSource": CatalogHudiSourceTypeDef,
-        "S3HudiSource": S3HudiSourceTypeDef,
-        "S3HudiCatalogTarget": S3HudiCatalogTargetTypeDef,
-        "S3HudiDirectTarget": S3HudiDirectTargetTypeDef,
-        "DirectJDBCSource": DirectJDBCSourceTypeDef,
-        "S3CatalogDeltaSource": S3CatalogDeltaSourceTypeDef,
-        "CatalogDeltaSource": CatalogDeltaSourceTypeDef,
-        "S3DeltaSource": S3DeltaSourceTypeDef,
-        "S3DeltaCatalogTarget": S3DeltaCatalogTargetTypeDef,
-        "S3DeltaDirectTarget": S3DeltaDirectTargetTypeDef,
     },
     total=False,
 )
 
 GetMLTaskRunsResponseTypeDef = TypedDict(
     "GetMLTaskRunsResponseTypeDef",
     {
@@ -9033,20 +8411,22 @@
     "_OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class UpdateColumnStatisticsForPartitionRequestRequestTypeDef(
     _RequiredUpdateColumnStatisticsForPartitionRequestRequestTypeDef,
     _OptionalUpdateColumnStatisticsForPartitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "ColumnStatisticsList": Sequence[ColumnStatisticsTypeDef],
     },
@@ -9055,20 +8435,22 @@
     "_OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class UpdateColumnStatisticsForTableRequestRequestTypeDef(
     _RequiredUpdateColumnStatisticsForTableRequestRequestTypeDef,
     _OptionalUpdateColumnStatisticsForTableRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredBatchCreatePartitionRequestRequestTypeDef = TypedDict(
     "_RequiredBatchCreatePartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionInputList": Sequence[PartitionInputTypeDef],
     },
@@ -9077,20 +8459,22 @@
     "_OptionalBatchCreatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class BatchCreatePartitionRequestRequestTypeDef(
     _RequiredBatchCreatePartitionRequestRequestTypeDef,
     _OptionalBatchCreatePartitionRequestRequestTypeDef,
 ):
     pass
 
+
 BatchUpdatePartitionRequestEntryTypeDef = TypedDict(
     "BatchUpdatePartitionRequestEntryTypeDef",
     {
         "PartitionValueList": Sequence[str],
         "PartitionInput": PartitionInputTypeDef,
     },
 )
@@ -9107,19 +8491,21 @@
     "_OptionalCreatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class CreatePartitionRequestRequestTypeDef(
     _RequiredCreatePartitionRequestRequestTypeDef, _OptionalCreatePartitionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdatePartitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePartitionRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "PartitionValueList": Sequence[str],
         "PartitionInput": PartitionInputTypeDef,
@@ -9129,19 +8515,21 @@
     "_OptionalUpdatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class UpdatePartitionRequestRequestTypeDef(
     _RequiredUpdatePartitionRequestRequestTypeDef, _OptionalUpdatePartitionRequestRequestTypeDef
 ):
     pass
 
+
 BatchGetPartitionResponseTypeDef = TypedDict(
     "BatchGetPartitionResponseTypeDef",
     {
         "Partitions": List[PartitionTypeDef],
         "UnprocessedKeys": List[PartitionValueListTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -9197,19 +8585,21 @@
         "CatalogId": str,
         "PartitionIndexes": Sequence[PartitionIndexTypeDef],
         "TransactionId": str,
     },
     total=False,
 )
 
+
 class CreateTableRequestRequestTypeDef(
     _RequiredCreateTableRequestRequestTypeDef, _OptionalCreateTableRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableInput": TableInputTypeDef,
     },
 )
@@ -9220,19 +8610,21 @@
         "SkipArchive": bool,
         "TransactionId": str,
         "VersionId": str,
     },
     total=False,
 )
 
+
 class UpdateTableRequestRequestTypeDef(
     _RequiredUpdateTableRequestRequestTypeDef, _OptionalUpdateTableRequestRequestTypeDef
 ):
     pass
 
+
 GetTableResponseTypeDef = TypedDict(
     "GetTableResponseTypeDef",
     {
         "Table": TableTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -9305,19 +8697,21 @@
         "CodeGenConfigurationNodes": Mapping[str, CodeGenConfigurationNodeTypeDef],
         "ExecutionClass": ExecutionClassType,
         "SourceControlDetails": SourceControlDetailsTypeDef,
     },
     total=False,
 )
 
+
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
 
+
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "Name": str,
         "Description": str,
         "LogUri": str,
         "Role": str,
@@ -9408,20 +8802,22 @@
     "_OptionalBatchUpdatePartitionRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
     total=False,
 )
 
+
 class BatchUpdatePartitionRequestRequestTypeDef(
     _RequiredBatchUpdatePartitionRequestRequestTypeDef,
     _OptionalBatchUpdatePartitionRequestRequestTypeDef,
 ):
     pass
 
+
 GetUnfilteredPartitionsMetadataResponseTypeDef = TypedDict(
     "GetUnfilteredPartitionsMetadataResponseTypeDef",
     {
         "UnfilteredPartitions": List[UnfilteredPartitionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-glue-1.26.74/mypy_boto3_glue.egg-info/PKG-INFO` & `mypy-boto3-glue-1.26.8/mypy_boto3_glue.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-glue
-Version: 1.26.74
-Summary: Type annotations for boto3.Glue 1.26.74 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.8
+Summary: Type annotations for boto3.Glue 1.26.8 service generated with mypy-boto3-builder 7.11.10
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,15 +18,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -38,24 +37,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-glue.svg?color=blue)](https://pypi.org/project/mypy-boto3-glue)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-glue?color=blue)](https://pypistats.org/packages/mypy-boto3-glue)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Glue 1.26.74](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
+[boto3.Glue 1.26.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-glue docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/).
 
 See how it helps to find and fix potential bugs:
 
@@ -363,20 +362,16 @@
     ConnectionPropertyKeyType,
     ConnectionTypeType,
     CrawlStateType,
     CrawlerHistoryStateType,
     CrawlerLineageSettingsType,
     CrawlerStateType,
     CsvHeaderOptionType,
-    DQStopJobOnFailureTimingType,
-    DQTransformOutputType,
     DataFormatType,
-    DataQualityRuleResultStatusType,
     DeleteBehaviorType,
-    DeltaTargetCompressionTypeType,
     EnableHybridValuesType,
     ExecutionClassType,
     ExistConditionType,
     FieldNameType,
     FilterLogicalOperatorType,
     FilterOperationType,
     FilterOperatorType,
@@ -394,31 +389,27 @@
     GetResourcePoliciesPaginatorName,
     GetSecurityConfigurationsPaginatorName,
     GetTableVersionsPaginatorName,
     GetTablesPaginatorName,
     GetTriggersPaginatorName,
     GetUserDefinedFunctionsPaginatorName,
     GlueRecordTypeType,
-    HudiTargetCompressionTypeType,
-    JDBCConnectionTypeType,
     JDBCDataTypeType,
-    JdbcMetadataEntryType,
     JobBookmarksEncryptionModeType,
     JobRunStateType,
     JoinTypeType,
     LanguageType,
     LastCrawlStatusType,
     ListRegistriesPaginatorName,
     ListSchemaVersionsPaginatorName,
     ListSchemasPaginatorName,
     LogicalOperatorType,
     LogicalType,
     MLUserDataEncryptionModeStringType,
     NodeTypeType,
-    ParamTypeType,
     ParquetCompressionTypeType,
     PartitionIndexStatusType,
     PermissionType,
     PermissionTypeType,
     PiiTypeType,
     PrincipalTypeType,
     QuoteCharType,
@@ -485,29 +476,26 @@
     ErrorDetailTypeDef,
     BatchDeleteTableRequestRequestTypeDef,
     BatchDeleteTableVersionRequestRequestTypeDef,
     BatchGetBlueprintsRequestRequestTypeDef,
     BatchGetCrawlersRequestRequestTypeDef,
     BatchGetCustomEntityTypesRequestRequestTypeDef,
     CustomEntityTypeTypeDef,
-    BatchGetDataQualityResultRequestRequestTypeDef,
     BatchGetDevEndpointsRequestRequestTypeDef,
     DevEndpointTypeDef,
     BatchGetJobsRequestRequestTypeDef,
     BatchGetTriggersRequestRequestTypeDef,
     BatchGetWorkflowsRequestRequestTypeDef,
     BatchStopJobRunRequestRequestTypeDef,
     BatchStopJobRunSuccessfulSubmissionTypeDef,
     BinaryColumnStatisticsDataTypeDef,
     BlueprintDetailsTypeDef,
     BlueprintRunTypeDef,
     LastActiveDefinitionTypeDef,
     BooleanColumnStatisticsDataTypeDef,
-    CancelDataQualityRuleRecommendationRunRequestRequestTypeDef,
-    CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef,
     CancelMLTaskRunRequestRequestTypeDef,
     CancelStatementRequestRequestTypeDef,
     CatalogEntryTypeDef,
     CatalogImportStatusTypeDef,
     KafkaStreamingSourceOptionsTypeDef,
     StreamingDataPreviewOptionsTypeDef,
     KinesisStreamingSourceOptionsTypeDef,
@@ -516,15 +504,14 @@
     CatalogTargetTypeDef,
     CheckSchemaVersionValidityInputRequestTypeDef,
     CsvClassifierTypeDef,
     GrokClassifierTypeDef,
     JsonClassifierTypeDef,
     XMLClassifierTypeDef,
     CloudWatchEncryptionTypeDef,
-    DirectJDBCSourceTypeDef,
     DropDuplicatesTypeDef,
     DropFieldsTypeDef,
     DynamoDBCatalogSourceTypeDef,
     FillMissingValuesTypeDef,
     MergeTypeDef,
     MicrosoftSQLServerCatalogSourceTypeDef,
     MicrosoftSQLServerCatalogTargetTypeDef,
@@ -574,43 +561,37 @@
     CrawlsFilterTypeDef,
     CreateBlueprintRequestRequestTypeDef,
     CreateCsvClassifierRequestTypeDef,
     CreateGrokClassifierRequestTypeDef,
     CreateJsonClassifierRequestTypeDef,
     CreateXMLClassifierRequestTypeDef,
     CreateCustomEntityTypeRequestRequestTypeDef,
-    DataQualityTargetTableTypeDef,
     CreateDevEndpointRequestRequestTypeDef,
     ExecutionPropertyTypeDef,
     JobCommandTypeDef,
     SourceControlDetailsTypeDef,
     GlueTableTypeDef,
     PartitionIndexTypeDef,
     CreateRegistryInputRequestTypeDef,
     RegistryIdTypeDef,
     SessionCommandTypeDef,
     EventBatchingConditionTypeDef,
     CreateWorkflowRequestRequestTypeDef,
-    DQResultsPublishingOptionsTypeDef,
-    DQStopJobOnFailureOptionsTypeDef,
     EncryptionAtRestTypeDef,
     DataLakePrincipalTypeDef,
-    DataQualityEvaluationRunAdditionalRunOptionsTypeDef,
-    DataQualityRuleResultTypeDef,
     DatabaseIdentifierTypeDef,
     DatatypeTypeDef,
     DecimalNumberTypeDef,
     DeleteBlueprintRequestRequestTypeDef,
     DeleteClassifierRequestRequestTypeDef,
     DeleteColumnStatisticsForPartitionRequestRequestTypeDef,
     DeleteColumnStatisticsForTableRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteCrawlerRequestRequestTypeDef,
     DeleteCustomEntityTypeRequestRequestTypeDef,
-    DeleteDataQualityRulesetRequestRequestTypeDef,
     DeleteDatabaseRequestRequestTypeDef,
     DeleteDevEndpointRequestRequestTypeDef,
     DeleteJobRequestRequestTypeDef,
     DeleteMLTransformRequestRequestTypeDef,
     DeletePartitionIndexRequestRequestTypeDef,
     DeletePartitionRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
@@ -621,15 +602,14 @@
     DeleteTableVersionRequestRequestTypeDef,
     DeleteTriggerRequestRequestTypeDef,
     DeleteUserDefinedFunctionRequestRequestTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     DevEndpointCustomLibrariesTypeDef,
     DirectSchemaChangePolicyTypeDef,
     NullCheckBoxListTypeDef,
-    TransformConfigParameterTypeDef,
     EdgeTypeDef,
     JobBookmarksEncryptionTypeDef,
     S3EncryptionTypeDef,
     ErrorDetailsTypeDef,
     ExportLabelsTaskRunPropertiesTypeDef,
     FilterValueTypeDef,
     FindMatchesParametersTypeDef,
@@ -646,18 +626,14 @@
     GetConnectionRequestRequestTypeDef,
     GetConnectionsFilterTypeDef,
     GetCrawlerMetricsRequestRequestTypeDef,
     GetCrawlerRequestRequestTypeDef,
     GetCrawlersRequestRequestTypeDef,
     GetCustomEntityTypeRequestRequestTypeDef,
     GetDataCatalogEncryptionSettingsRequestRequestTypeDef,
-    GetDataQualityResultRequestRequestTypeDef,
-    GetDataQualityRuleRecommendationRunRequestRequestTypeDef,
-    GetDataQualityRulesetEvaluationRunRequestRequestTypeDef,
-    GetDataQualityRulesetRequestRequestTypeDef,
     GetDatabaseRequestRequestTypeDef,
     GetDatabasesRequestRequestTypeDef,
     GetDataflowGraphRequestRequestTypeDef,
     GetDevEndpointRequestRequestTypeDef,
     GetDevEndpointsRequestRequestTypeDef,
     GetJobBookmarkRequestRequestTypeDef,
     JobBookmarkEntryTypeDef,
@@ -757,15 +733,14 @@
     UntagResourceRequestRequestTypeDef,
     UpdateBlueprintRequestRequestTypeDef,
     UpdateCsvClassifierRequestTypeDef,
     UpdateGrokClassifierRequestTypeDef,
     UpdateJsonClassifierRequestTypeDef,
     UpdateXMLClassifierRequestTypeDef,
     UpdateCrawlerScheduleRequestRequestTypeDef,
-    UpdateDataQualityRulesetRequestRequestTypeDef,
     UpdateJobFromSourceControlRequestRequestTypeDef,
     UpdateSourceControlFromJobRequestRequestTypeDef,
     UpdateWorkflowRequestRequestTypeDef,
     WorkflowRunStatisticsTypeDef,
     ActionTypeDef,
     StartJobRunRequestRequestTypeDef,
     AggregateTypeDef,
@@ -774,15 +749,14 @@
     BackfillErrorTypeDef,
     BatchDeletePartitionRequestRequestTypeDef,
     BatchGetPartitionRequestRequestTypeDef,
     CancelMLTaskRunResponseTypeDef,
     CheckSchemaVersionValidityResponseTypeDef,
     CreateBlueprintResponseTypeDef,
     CreateCustomEntityTypeResponseTypeDef,
-    CreateDataQualityRulesetResponseTypeDef,
     CreateDevEndpointResponseTypeDef,
     CreateJobResponseTypeDef,
     CreateMLTransformResponseTypeDef,
     CreateRegistryResponseTypeDef,
     CreateSchemaResponseTypeDef,
     CreateScriptResponseTypeDef,
     CreateSecurityConfigurationResponseTypeDef,
@@ -817,27 +791,24 @@
     PutResourcePolicyResponseTypeDef,
     PutSchemaVersionMetadataResponseTypeDef,
     RegisterSchemaVersionResponseTypeDef,
     RemoveSchemaVersionMetadataResponseTypeDef,
     ResumeWorkflowRunResponseTypeDef,
     RunStatementResponseTypeDef,
     StartBlueprintRunResponseTypeDef,
-    StartDataQualityRuleRecommendationRunResponseTypeDef,
-    StartDataQualityRulesetEvaluationRunResponseTypeDef,
     StartExportLabelsTaskRunResponseTypeDef,
     StartImportLabelsTaskRunResponseTypeDef,
     StartJobRunResponseTypeDef,
     StartMLEvaluationTaskRunResponseTypeDef,
     StartMLLabelingSetGenerationTaskRunResponseTypeDef,
     StartTriggerResponseTypeDef,
     StartWorkflowRunResponseTypeDef,
     StopSessionResponseTypeDef,
     StopTriggerResponseTypeDef,
     UpdateBlueprintResponseTypeDef,
-    UpdateDataQualityRulesetResponseTypeDef,
     UpdateJobFromSourceControlResponseTypeDef,
     UpdateJobResponseTypeDef,
     UpdateMLTransformResponseTypeDef,
     UpdateRegistryResponseTypeDef,
     UpdateSchemaResponseTypeDef,
     UpdateSourceControlFromJobResponseTypeDef,
     UpdateWorkflowResponseTypeDef,
@@ -859,60 +830,49 @@
     GetCatalogImportStatusResponseTypeDef,
     CatalogKafkaSourceTypeDef,
     DirectKafkaSourceTypeDef,
     CatalogKinesisSourceTypeDef,
     DirectKinesisSourceTypeDef,
     GovernedCatalogTargetTypeDef,
     S3CatalogTargetTypeDef,
-    S3DeltaCatalogTargetTypeDef,
-    S3HudiCatalogTargetTypeDef,
     ClassifierTypeDef,
     CodeGenNodeTypeDef,
     LocationTypeDef,
     PredicateTypeDef,
     FindMatchesMetricsTypeDef,
     ConnectionInputTypeDef,
     ConnectionTypeDef,
     CrawlerNodeDetailsTypeDef,
     ListCrawlsResponseTypeDef,
     GetCrawlerMetricsResponseTypeDef,
     CrawlerTargetsTypeDef,
     ListCrawlsRequestRequestTypeDef,
     CreateClassifierRequestRequestTypeDef,
-    CreateDataQualityRulesetRequestRequestTypeDef,
-    DataQualityRulesetFilterCriteriaTypeDef,
-    DataQualityRulesetListDetailsTypeDef,
-    GetDataQualityRulesetResponseTypeDef,
-    DataSourceTypeDef,
     CreatePartitionIndexRequestRequestTypeDef,
     CreateSchemaInputRequestTypeDef,
     DeleteRegistryInputRequestTypeDef,
     GetRegistryInputRequestTypeDef,
     ListSchemasInputRequestTypeDef,
     UpdateRegistryInputRequestTypeDef,
     CreateSessionRequestRequestTypeDef,
     SessionTypeDef,
-    EvaluateDataQualityTypeDef,
     DataCatalogEncryptionSettingsTypeDef,
     PrincipalPermissionsTypeDef,
     NullValueFieldTypeDef,
     DecimalColumnStatisticsDataTypeDef,
     DeleteSchemaInputRequestTypeDef,
     DeleteSchemaVersionsInputRequestTypeDef,
     GetSchemaByDefinitionInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
     ListSchemaVersionsInputRequestTypeDef,
     RegisterSchemaVersionInputRequestTypeDef,
     SchemaReferenceTypeDef,
     UpdateDevEndpointRequestRequestTypeDef,
-    S3DeltaDirectTargetTypeDef,
     S3DirectTargetTypeDef,
     S3GlueParquetTargetTypeDef,
-    S3HudiDirectTargetTypeDef,
-    DynamicTransformTypeDef,
     EncryptionConfigurationTypeDef,
     SchemaVersionErrorItemTypeDef,
     FilterExpressionTypeDef,
     TransformParametersTypeDef,
     GetClassifiersRequestGetClassifiersPaginateTypeDef,
     GetCrawlerMetricsRequestGetCrawlerMetricsPaginateTypeDef,
     GetCrawlersRequestGetCrawlersPaginateTypeDef,
@@ -986,28 +946,14 @@
     CreateConnectionRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     GetConnectionResponseTypeDef,
     GetConnectionsResponseTypeDef,
     CrawlerTypeDef,
     CreateCrawlerRequestRequestTypeDef,
     UpdateCrawlerRequestRequestTypeDef,
-    ListDataQualityRulesetsRequestRequestTypeDef,
-    ListDataQualityRulesetsResponseTypeDef,
-    DataQualityResultDescriptionTypeDef,
-    DataQualityResultFilterCriteriaTypeDef,
-    DataQualityResultTypeDef,
-    DataQualityRuleRecommendationRunDescriptionTypeDef,
-    DataQualityRuleRecommendationRunFilterTypeDef,
-    DataQualityRulesetEvaluationRunDescriptionTypeDef,
-    DataQualityRulesetEvaluationRunFilterTypeDef,
-    GetDataQualityResultResponseTypeDef,
-    GetDataQualityRuleRecommendationRunResponseTypeDef,
-    GetDataQualityRulesetEvaluationRunResponseTypeDef,
-    StartDataQualityRuleRecommendationRunRequestRequestTypeDef,
-    StartDataQualityRulesetEvaluationRunRequestRequestTypeDef,
     CreateSessionResponseTypeDef,
     GetSessionResponseTypeDef,
     ListSessionsResponseTypeDef,
     GetDataCatalogEncryptionSettingsResponseTypeDef,
     PutDataCatalogEncryptionSettingsRequestRequestTypeDef,
     DatabaseInputTypeDef,
     DatabaseTypeDef,
@@ -1018,24 +964,18 @@
     SecurityConfigurationTypeDef,
     DeleteSchemaVersionsResponseTypeDef,
     FilterTypeDef,
     UpdateMLTransformRequestRequestTypeDef,
     GetMLTransformsRequestRequestTypeDef,
     ListMLTransformsRequestRequestTypeDef,
     AthenaConnectorSourceTypeDef,
-    CatalogDeltaSourceTypeDef,
-    CatalogHudiSourceTypeDef,
     CustomCodeTypeDef,
     JDBCConnectorSourceTypeDef,
     JDBCConnectorTargetTypeDef,
-    S3CatalogDeltaSourceTypeDef,
-    S3CatalogHudiSourceTypeDef,
     S3CsvSourceTypeDef,
-    S3DeltaSourceTypeDef,
-    S3HudiSourceTypeDef,
     S3JsonSourceTypeDef,
     S3ParquetSourceTypeDef,
     SparkConnectorSourceTypeDef,
     SparkConnectorTargetTypeDef,
     SparkSQLTypeDef,
     GetJobRunResponseTypeDef,
     GetJobRunsResponseTypeDef,
@@ -1057,21 +997,14 @@
     UpdateTriggerResponseTypeDef,
     UpdateTriggerRequestRequestTypeDef,
     GetMLTransformResponseTypeDef,
     MLTransformTypeDef,
     BatchGetCrawlersResponseTypeDef,
     GetCrawlerResponseTypeDef,
     GetCrawlersResponseTypeDef,
-    ListDataQualityResultsResponseTypeDef,
-    ListDataQualityResultsRequestRequestTypeDef,
-    BatchGetDataQualityResultResponseTypeDef,
-    ListDataQualityRuleRecommendationRunsResponseTypeDef,
-    ListDataQualityRuleRecommendationRunsRequestRequestTypeDef,
-    ListDataQualityRulesetEvaluationRunsResponseTypeDef,
-    ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef,
     CreateDatabaseRequestRequestTypeDef,
     UpdateDatabaseRequestRequestTypeDef,
     GetDatabaseResponseTypeDef,
     GetDatabasesResponseTypeDef,
     ColumnStatisticsTypeDef,
     PartitionInputTypeDef,
     PartitionTypeDef,
```

### Comparing `mypy-boto3-glue-1.26.74/mypy_boto3_glue.egg-info/SOURCES.txt` & `mypy-boto3-glue-1.26.8/mypy_boto3_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-glue-1.26.74/setup.py` & `mypy-boto3-glue-1.26.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,45 +6,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-glue",
-    version="1.26.74",
+    version="1.26.8",
     packages=["mypy_boto3_glue"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Glue 1.26.74 service generated with mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.Glue 1.26.8 service generated with mypy-boto3-builder 7.11.10"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 glue type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"mypy_boto3_glue": ["py.typed", "*.pyi"]},
+    package_data={"": ["LICENSE"], "mypy_boto3_glue": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_glue/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

