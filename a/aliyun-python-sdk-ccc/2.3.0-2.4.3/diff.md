# Comparing `tmp/aliyun-python-sdk-ccc-2.3.0.tar.gz` & `tmp/aliyun-python-sdk-ccc-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-ccc-2.3.0.tar", last modified: Fri Jan 28 07:40:19 2022, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-ccc-2.4.3.tar", last modified: Tue Apr 26 03:28:10 2022, max compression
```

## Comparing `aliyun-python-sdk-ccc-2.3.0.tar` & `aliyun-python-sdk-ccc-2.4.3.tar`

### file list

```diff
@@ -1,135 +1,160 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/
--rw-r--r--   0 root         (0) root         (0)      575 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1537 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyun_python_sdk_ccc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1537 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyun_python_sdk_ccc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7242 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyun_python_sdk_ccc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyun_python_sdk_ccc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyun_python_sdk_ccc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyun_python_sdk_ccc.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/
--rw-r--r--   0 root         (0) root         (0)       21 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1968 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/
--rw-r--r--   0 root         (0) root         (0)     1602 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/AbortCampaignRequest.py
--rw-r--r--   0 root         (0) root         (0)     1804 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/AddNumbersToSkillGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1772 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/AddPersonalNumbersToUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     1814 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/AddPhoneNumberToSkillGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2128 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/AddPhoneNumbersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1788 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/AddSkillGroupsToUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     1848 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/AddUsersToSkillGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1874 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/AnswerCallRequest.py
--rw-r--r--   0 root         (0) root         (0)     2096 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/AssignUsersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2256 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/BargeInCallRequest.py
--rw-r--r--   0 root         (0) root         (0)     2420 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/BlindTransferRequest.py
--rw-r--r--   0 root         (0) root         (0)     1898 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/CancelAttendedTransferRequest.py
--rw-r--r--   0 root         (0) root         (0)     1900 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ChangeWorkModeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2258 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/CoachCallRequest.py
--rw-r--r--   0 root         (0) root         (0)     1902 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/CompleteAttendedTransferRequest.py
--rw-r--r--   0 root         (0) root         (0)     3984 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/CreateCampaignRequest.py
--rw-r--r--   0 root         (0) root         (0)     2114 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/CreateInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1928 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/CreateSkillGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2752 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/CreateUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     1762 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/DeleteSkillGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1608 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetCallDetailRecordRequest.py
--rw-r--r--   0 root         (0) root         (0)     1598 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetCampaignRequest.py
--rw-r--r--   0 root         (0) root         (0)     1604 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetCaseFileUploadUrlRequest.py
--rw-r--r--   0 root         (0) root         (0)     1970 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetHistoricalCallerReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     1778 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetHistoricalInstanceReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     1426 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1774 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetInstanceTrendingReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     1582 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetLoginDetailsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1602 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetMonoRecordingRequest.py
--rw-r--r--   0 root         (0) root         (0)     1618 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetMultiChannelRecordingRequest.py
--rw-r--r--   0 root         (0) root         (0)     1586 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetNumberLocationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1454 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetRealtimeInstanceStatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1588 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetTurnCredentialsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1438 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetTurnServerListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1732 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     2178 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/HoldCallRequest.py
--rw-r--r--   0 root         (0) root         (0)     2442 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/InitiateAttendedTransferRequest.py
--rw-r--r--   0 root         (0) root         (0)     2290 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/InterceptCallRequest.py
--rw-r--r--   0 root         (0) root         (0)     2084 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/LaunchAuthenticationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2068 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/LaunchSurveyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1914 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListAgentStateLogsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3335 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListAttemptsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1966 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListBriefSkillGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     4854 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListCallDetailRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1947 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListCampaignTrendingReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     3074 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListCampaignsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2104 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListCasesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1766 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListConfigItemsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1904 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListContactFlowsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1574 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListDevicesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2290 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListHistoricalAgentReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     2324 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListHistoricalSkillGroupReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     1602 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListInstancesOfUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     1590 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2084 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListIntervalAgentReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     1936 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListIntervalInstanceReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     2124 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListIntervalSkillGroupReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     1946 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListIvrTrackingDetailsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2142 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListOutboundNumbersOfUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     2284 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListPersonalNumbersOfUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     2474 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListPhoneNumbersOfSkillGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2248 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListPhoneNumbersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1444 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListPrivilegesOfUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     1950 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListRamUsersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2476 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListRealtimeAgentStatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2000 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListRealtimeSkillGroupStatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2270 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListRecentCallDetailRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1422 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListRolesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1630 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListSipCallRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1578 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListSipTracesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1956 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListSkillGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2276 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListSkillLevelsOfUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     1968 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListUnassignedNumbersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2322 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListUserLevelsOfSkillGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1944 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListUsersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2540 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/MakeCallRequest.py
--rw-r--r--   0 root         (0) root         (0)     1610 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ModifyInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1918 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ModifyPhoneNumberRequest.py
--rw-r--r--   0 root         (0) root         (0)     1976 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ModifySkillGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1794 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ModifySkillLevelsOfUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     1834 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ModifyUserLevelsOfSkillGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2028 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ModifyUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     2132 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/MonitorCallRequest.py
--rw-r--r--   0 root         (0) root         (0)     2036 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/MuteCallRequest.py
--rw-r--r--   0 root         (0) root         (0)     1602 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/PauseCampaignRequest.py
--rw-r--r--   0 root         (0) root         (0)     1976 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/PickOutboundNumbersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1740 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/PollUserStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1950 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ReadyForServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1900 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/RegisterDeviceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1950 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/RegisterDevicesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2042 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ReleaseCallRequest.py
--rw-r--r--   0 root         (0) root         (0)     1782 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/RemovePersonalNumbersFromUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     1824 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/RemovePhoneNumberFromSkillGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1824 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/RemovePhoneNumbersFromSkillGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1612 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/RemovePhoneNumbersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1810 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/RemoveSkillGroupsFromUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     1810 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/RemoveUsersFromSkillGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1598 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/RemoveUsersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1742 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ResetAgentStateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1746 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ResetUserPasswordRequest.py
--rw-r--r--   0 root         (0) root         (0)     1604 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ResumeCampaignRequest.py
--rw-r--r--   0 root         (0) root         (0)     2044 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/RetrieveCallRequest.py
--rw-r--r--   0 root         (0) root         (0)     2316 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/SaveRTCStatsV2Request.py
--rw-r--r--   0 root         (0) root         (0)     2714 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/SaveTerminalLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     2318 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/SaveWebRTCStatsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2054 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/SaveWebRtcInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     2190 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/SendDtmfSignalingRequest.py
--rw-r--r--   0 root         (0) root         (0)     1978 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/SignInGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1736 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/SignOutGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2424 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/StartBack2BackCallRequest.py
--rw-r--r--   0 root         (0) root         (0)     2860 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/StartPredictiveCallRequest.py
--rw-r--r--   0 root         (0) root         (0)     1604 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/SubmitCampaignRequest.py
--rw-r--r--   0 root         (0) root         (0)     1866 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/TakeBreakRequest.py
--rw-r--r--   0 root         (0) root         (0)     2040 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/UnmuteCallRequest.py
--rw-r--r--   0 root         (0) root         (0)     1948 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/UpdateConfigItemsRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2452 2022-01-28 07:40:19.000000 aliyun-python-sdk-ccc-2.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-26 03:28:10.000000 aliyun-python-sdk-ccc-2.4.3/
+-rw-r--r--   0 root         (0) root         (0)      575 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1537 2022-04-26 03:28:10.000000 aliyun-python-sdk-ccc-2.4.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-26 03:28:10.000000 aliyun-python-sdk-ccc-2.4.3/aliyun_python_sdk_ccc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1537 2022-04-26 03:28:10.000000 aliyun-python-sdk-ccc-2.4.3/aliyun_python_sdk_ccc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8833 2022-04-26 03:28:10.000000 aliyun-python-sdk-ccc-2.4.3/aliyun_python_sdk_ccc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-04-26 03:28:10.000000 aliyun-python-sdk-ccc-2.4.3/aliyun_python_sdk_ccc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2022-04-26 03:28:10.000000 aliyun-python-sdk-ccc-2.4.3/aliyun_python_sdk_ccc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-04-26 03:28:10.000000 aliyun-python-sdk-ccc-2.4.3/aliyun_python_sdk_ccc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-26 03:28:10.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1968 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-26 03:28:10.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-26 03:28:10.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/
+-rw-r--r--   0 root         (0) root         (0)     1644 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/AbortCampaignRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1865 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/AddNumbersToSkillGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/AddPersonalNumbersToUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1875 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/AddPhoneNumberToSkillGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/AddPhoneNumbersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/AddSkillGroupsToUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/AddUsersToSkillGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/AnswerCallRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/AssignUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/BargeInCallRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/BlindTransferRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/CancelAttendedTransferRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1980 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ChangeWorkModeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/CoachCallRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/CompleteAttendedTransferRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/CreateCallTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4267 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/CreateCampaignRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1700 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/CreateCustomCallTaggingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/CreateInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/CreateSkillGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3114 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/CreateUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/DeleteCallTagRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/DeleteCustomCallTaggingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/DeleteSkillGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1473 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ExportCustomCallTaggingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ExportDoNotCallNumbersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetCallDetailRecordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetCampaignRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetCaseFileUploadUrlRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetDoNotCallFileUploadParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetHistoricalCallerReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetHistoricalCampaignReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetHistoricalInstanceReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1449 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetInstanceTrendingReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1624 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetLoginDetailsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetMonoRecordingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetMultiChannelRecordingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetNumberLocationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1647 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetRealtimeCampaignStatsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1477 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetRealtimeInstanceStatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetSkillGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1630 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetTurnCredentialsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetTurnServerListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1793 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/HoldCallRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ImportAdminsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ImportCustomCallTaggingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ImportDoNotCallNumbersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2581 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/InitiateAttendedTransferRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2410 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/InterceptCallRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2434 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/LaunchAuthenticationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/LaunchSurveyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListAgentStateLogsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListAgentStatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2254 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListAgentSummaryReportsSinceMidnightRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3582 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListAttemptsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListBriefSkillGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5699 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListCallDetailRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListCallTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListCampaignTrendingReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3260 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListCampaignsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListCasesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListConfigItemsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListContactFlowsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListCustomCallTaggingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1616 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListDevicesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2211 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListDoNotCallNumbersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2403 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListHistoricalAgentReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2437 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListHistoricalSkillGroupReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListInstancesOfUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2175 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListIntervalAgentReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListIntervalInstanceReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2215 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListIntervalSkillGroupReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListIvrTrackingDetailsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListMonoRecordingsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListMultiChannelRecordingsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListOutboundNumbersOfUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2408 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListPersonalNumbersOfUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2619 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListPhoneNumbersOfSkillGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2372 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListPhoneNumbersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1467 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListPrivilegesOfUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListRamUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListRealtimeAgentStatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2083 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListRealtimeSkillGroupStatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2383 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListRecentCallDetailRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListRolesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListSipCallRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListSipTracesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListSkillGroupStatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2079 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListSkillGroupSummaryReportsSinceMidnightRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2040 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListSkillGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListSkillLevelsOfUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListUnassignedNumbersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2446 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListUserLevelsOfSkillGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2028 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2698 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/MakeCallRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ModifyCustomCallTaggingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ModifyInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1998 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ModifyPhoneNumberRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ModifySkillGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1855 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ModifySkillLevelsOfUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1895 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ModifyUserLevelsOfSkillGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ModifyUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/MonitorCallRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2135 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/MuteCallRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/PauseCampaignRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/PickOutboundNumbersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/PollUserStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ReadyForServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1980 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/RegisterDeviceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/RegisterDevicesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2141 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ReleaseCallRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/RemoveDoNotCallNumbersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/RemovePersonalNumbersFromUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1885 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/RemovePhoneNumberFromSkillGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1885 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/RemovePhoneNumbersFromSkillGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/RemovePhoneNumbersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/RemoveSkillGroupsFromUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/RemoveUsersFromSkillGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/RemoveUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1803 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ResetAgentStateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1807 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ResetUserPasswordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ResumeCampaignRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/RetrieveCallRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2434 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/SaveRTCStatsV2Request.py
+-rw-r--r--   0 root         (0) root         (0)     2891 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/SaveTerminalLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2436 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/SaveWebRTCStatsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/SaveWebRtcInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2308 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/SendDtmfSignalingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/SignInGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1797 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/SignOutGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/StartBack2BackCallRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3037 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/StartPredictiveCallRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/SubmitCampaignRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1946 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/TakeBreakRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2139 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/UnmuteCallRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/UnregisterDeviceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2028 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/UpdateConfigItemsRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2022-04-26 03:28:10.000000 aliyun-python-sdk-ccc-2.4.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2452 2022-04-26 03:28:09.000000 aliyun-python-sdk-ccc-2.4.3/setup.py
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/LICENSE` & `aliyun-python-sdk-ccc-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ccc-2.3.0/PKG-INFO` & `aliyun-python-sdk-ccc-2.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-ccc
-Version: 2.3.0
+Version: 2.4.3
 Summary: The ccc module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-ccc
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/README.rst` & `aliyun-python-sdk-ccc-2.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyun_python_sdk_ccc.egg-info/PKG-INFO` & `aliyun-python-sdk-ccc-2.4.3/aliyun_python_sdk_ccc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-ccc
-Version: 2.3.0
+Version: 2.4.3
 Summary: The ccc module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-ccc
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyun_python_sdk_ccc.egg-info/SOURCES.txt` & `aliyun-python-sdk-ccc-2.4.3/aliyun_python_sdk_ccc.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -22,75 +22,98 @@
 aliyunsdkccc/request/v20200701/AssignUsersRequest.py
 aliyunsdkccc/request/v20200701/BargeInCallRequest.py
 aliyunsdkccc/request/v20200701/BlindTransferRequest.py
 aliyunsdkccc/request/v20200701/CancelAttendedTransferRequest.py
 aliyunsdkccc/request/v20200701/ChangeWorkModeRequest.py
 aliyunsdkccc/request/v20200701/CoachCallRequest.py
 aliyunsdkccc/request/v20200701/CompleteAttendedTransferRequest.py
+aliyunsdkccc/request/v20200701/CreateCallTagsRequest.py
 aliyunsdkccc/request/v20200701/CreateCampaignRequest.py
+aliyunsdkccc/request/v20200701/CreateCustomCallTaggingRequest.py
 aliyunsdkccc/request/v20200701/CreateInstanceRequest.py
 aliyunsdkccc/request/v20200701/CreateSkillGroupRequest.py
 aliyunsdkccc/request/v20200701/CreateUserRequest.py
+aliyunsdkccc/request/v20200701/DeleteCallTagRequest.py
+aliyunsdkccc/request/v20200701/DeleteCustomCallTaggingRequest.py
 aliyunsdkccc/request/v20200701/DeleteSkillGroupRequest.py
+aliyunsdkccc/request/v20200701/ExportCustomCallTaggingRequest.py
+aliyunsdkccc/request/v20200701/ExportDoNotCallNumbersRequest.py
 aliyunsdkccc/request/v20200701/GetCallDetailRecordRequest.py
 aliyunsdkccc/request/v20200701/GetCampaignRequest.py
 aliyunsdkccc/request/v20200701/GetCaseFileUploadUrlRequest.py
+aliyunsdkccc/request/v20200701/GetDoNotCallFileUploadParametersRequest.py
 aliyunsdkccc/request/v20200701/GetHistoricalCallerReportRequest.py
+aliyunsdkccc/request/v20200701/GetHistoricalCampaignReportRequest.py
 aliyunsdkccc/request/v20200701/GetHistoricalInstanceReportRequest.py
 aliyunsdkccc/request/v20200701/GetInstanceRequest.py
 aliyunsdkccc/request/v20200701/GetInstanceTrendingReportRequest.py
 aliyunsdkccc/request/v20200701/GetLoginDetailsRequest.py
 aliyunsdkccc/request/v20200701/GetMonoRecordingRequest.py
 aliyunsdkccc/request/v20200701/GetMultiChannelRecordingRequest.py
 aliyunsdkccc/request/v20200701/GetNumberLocationRequest.py
+aliyunsdkccc/request/v20200701/GetRealtimeCampaignStatsRequest.py
 aliyunsdkccc/request/v20200701/GetRealtimeInstanceStatesRequest.py
+aliyunsdkccc/request/v20200701/GetSkillGroupRequest.py
 aliyunsdkccc/request/v20200701/GetTurnCredentialsRequest.py
 aliyunsdkccc/request/v20200701/GetTurnServerListRequest.py
 aliyunsdkccc/request/v20200701/GetUserRequest.py
 aliyunsdkccc/request/v20200701/HoldCallRequest.py
+aliyunsdkccc/request/v20200701/ImportAdminsRequest.py
+aliyunsdkccc/request/v20200701/ImportCustomCallTaggingRequest.py
+aliyunsdkccc/request/v20200701/ImportDoNotCallNumbersRequest.py
 aliyunsdkccc/request/v20200701/InitiateAttendedTransferRequest.py
 aliyunsdkccc/request/v20200701/InterceptCallRequest.py
 aliyunsdkccc/request/v20200701/LaunchAuthenticationRequest.py
 aliyunsdkccc/request/v20200701/LaunchSurveyRequest.py
 aliyunsdkccc/request/v20200701/ListAgentStateLogsRequest.py
+aliyunsdkccc/request/v20200701/ListAgentStatesRequest.py
+aliyunsdkccc/request/v20200701/ListAgentSummaryReportsSinceMidnightRequest.py
 aliyunsdkccc/request/v20200701/ListAttemptsRequest.py
 aliyunsdkccc/request/v20200701/ListBriefSkillGroupsRequest.py
 aliyunsdkccc/request/v20200701/ListCallDetailRecordsRequest.py
+aliyunsdkccc/request/v20200701/ListCallTagsRequest.py
 aliyunsdkccc/request/v20200701/ListCampaignTrendingReportRequest.py
 aliyunsdkccc/request/v20200701/ListCampaignsRequest.py
 aliyunsdkccc/request/v20200701/ListCasesRequest.py
 aliyunsdkccc/request/v20200701/ListConfigItemsRequest.py
 aliyunsdkccc/request/v20200701/ListContactFlowsRequest.py
+aliyunsdkccc/request/v20200701/ListCustomCallTaggingRequest.py
 aliyunsdkccc/request/v20200701/ListDevicesRequest.py
+aliyunsdkccc/request/v20200701/ListDoNotCallNumbersRequest.py
 aliyunsdkccc/request/v20200701/ListHistoricalAgentReportRequest.py
 aliyunsdkccc/request/v20200701/ListHistoricalSkillGroupReportRequest.py
 aliyunsdkccc/request/v20200701/ListInstancesOfUserRequest.py
 aliyunsdkccc/request/v20200701/ListInstancesRequest.py
 aliyunsdkccc/request/v20200701/ListIntervalAgentReportRequest.py
 aliyunsdkccc/request/v20200701/ListIntervalInstanceReportRequest.py
 aliyunsdkccc/request/v20200701/ListIntervalSkillGroupReportRequest.py
 aliyunsdkccc/request/v20200701/ListIvrTrackingDetailsRequest.py
+aliyunsdkccc/request/v20200701/ListMonoRecordingsRequest.py
+aliyunsdkccc/request/v20200701/ListMultiChannelRecordingsRequest.py
 aliyunsdkccc/request/v20200701/ListOutboundNumbersOfUserRequest.py
 aliyunsdkccc/request/v20200701/ListPersonalNumbersOfUserRequest.py
 aliyunsdkccc/request/v20200701/ListPhoneNumbersOfSkillGroupRequest.py
 aliyunsdkccc/request/v20200701/ListPhoneNumbersRequest.py
 aliyunsdkccc/request/v20200701/ListPrivilegesOfUserRequest.py
 aliyunsdkccc/request/v20200701/ListRamUsersRequest.py
 aliyunsdkccc/request/v20200701/ListRealtimeAgentStatesRequest.py
 aliyunsdkccc/request/v20200701/ListRealtimeSkillGroupStatesRequest.py
 aliyunsdkccc/request/v20200701/ListRecentCallDetailRecordsRequest.py
 aliyunsdkccc/request/v20200701/ListRolesRequest.py
 aliyunsdkccc/request/v20200701/ListSipCallRecordsRequest.py
 aliyunsdkccc/request/v20200701/ListSipTracesRequest.py
+aliyunsdkccc/request/v20200701/ListSkillGroupStatesRequest.py
+aliyunsdkccc/request/v20200701/ListSkillGroupSummaryReportsSinceMidnightRequest.py
 aliyunsdkccc/request/v20200701/ListSkillGroupsRequest.py
 aliyunsdkccc/request/v20200701/ListSkillLevelsOfUserRequest.py
 aliyunsdkccc/request/v20200701/ListUnassignedNumbersRequest.py
 aliyunsdkccc/request/v20200701/ListUserLevelsOfSkillGroupRequest.py
 aliyunsdkccc/request/v20200701/ListUsersRequest.py
 aliyunsdkccc/request/v20200701/MakeCallRequest.py
+aliyunsdkccc/request/v20200701/ModifyCustomCallTaggingRequest.py
 aliyunsdkccc/request/v20200701/ModifyInstanceRequest.py
 aliyunsdkccc/request/v20200701/ModifyPhoneNumberRequest.py
 aliyunsdkccc/request/v20200701/ModifySkillGroupRequest.py
 aliyunsdkccc/request/v20200701/ModifySkillLevelsOfUserRequest.py
 aliyunsdkccc/request/v20200701/ModifyUserLevelsOfSkillGroupRequest.py
 aliyunsdkccc/request/v20200701/ModifyUserRequest.py
 aliyunsdkccc/request/v20200701/MonitorCallRequest.py
@@ -98,14 +121,15 @@
 aliyunsdkccc/request/v20200701/PauseCampaignRequest.py
 aliyunsdkccc/request/v20200701/PickOutboundNumbersRequest.py
 aliyunsdkccc/request/v20200701/PollUserStatusRequest.py
 aliyunsdkccc/request/v20200701/ReadyForServiceRequest.py
 aliyunsdkccc/request/v20200701/RegisterDeviceRequest.py
 aliyunsdkccc/request/v20200701/RegisterDevicesRequest.py
 aliyunsdkccc/request/v20200701/ReleaseCallRequest.py
+aliyunsdkccc/request/v20200701/RemoveDoNotCallNumbersRequest.py
 aliyunsdkccc/request/v20200701/RemovePersonalNumbersFromUserRequest.py
 aliyunsdkccc/request/v20200701/RemovePhoneNumberFromSkillGroupsRequest.py
 aliyunsdkccc/request/v20200701/RemovePhoneNumbersFromSkillGroupRequest.py
 aliyunsdkccc/request/v20200701/RemovePhoneNumbersRequest.py
 aliyunsdkccc/request/v20200701/RemoveSkillGroupsFromUserRequest.py
 aliyunsdkccc/request/v20200701/RemoveUsersFromSkillGroupRequest.py
 aliyunsdkccc/request/v20200701/RemoveUsersRequest.py
@@ -121,9 +145,10 @@
 aliyunsdkccc/request/v20200701/SignInGroupRequest.py
 aliyunsdkccc/request/v20200701/SignOutGroupRequest.py
 aliyunsdkccc/request/v20200701/StartBack2BackCallRequest.py
 aliyunsdkccc/request/v20200701/StartPredictiveCallRequest.py
 aliyunsdkccc/request/v20200701/SubmitCampaignRequest.py
 aliyunsdkccc/request/v20200701/TakeBreakRequest.py
 aliyunsdkccc/request/v20200701/UnmuteCallRequest.py
+aliyunsdkccc/request/v20200701/UnregisterDeviceRequest.py
 aliyunsdkccc/request/v20200701/UpdateConfigItemsRequest.py
 aliyunsdkccc/request/v20200701/__init__.py
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/endpoint.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/AbortCampaignRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ModifyInstanceRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,29 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class AbortCampaignRequest(RpcRequest):
+class ModifyInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'AbortCampaign')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ModifyInstance')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Description(self): # String
+		return self.get_query_params().get('Description')
 
-	def get_InstanceId(self):
+	def set_Description(self, Description):  # String
+		self.add_query_param('Description', Description)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_CampaignId(self):
-		return self.get_query_params().get('CampaignId')
-
-	def set_CampaignId(self,CampaignId):
-		self.add_query_param('CampaignId',CampaignId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/AddNumbersToSkillGroupRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/DeleteSkillGroupRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,35 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class AddNumbersToSkillGroupRequest(RpcRequest):
+class DeleteSkillGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'AddNumbersToSkillGroup')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'DeleteSkillGroup')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_NumberList(self):
-		return self.get_query_params().get('NumberList')
-
-	def set_NumberList(self,NumberList):
-		self.add_query_param('NumberList',NumberList)
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_SkillGroupId(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_SkillGroupId(self): # String
 		return self.get_query_params().get('SkillGroupId')
 
-	def set_SkillGroupId(self,SkillGroupId):
-		self.add_query_param('SkillGroupId',SkillGroupId)
+	def set_SkillGroupId(self, SkillGroupId):  # String
+		self.add_query_param('SkillGroupId', SkillGroupId)
+	def get_Force(self): # Boolean
+		return self.get_query_params().get('Force')
+
+	def set_Force(self, Force):  # Boolean
+		self.add_query_param('Force', Force)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/AddPersonalNumbersToUserRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ResetUserPasswordRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,35 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class AddPersonalNumbersToUserRequest(RpcRequest):
+class ResetUserPasswordRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'AddPersonalNumbersToUser')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ResetUserPassword')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_UserId(self):
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_NumberList(self):
-		return self.get_query_params().get('NumberList')
-
-	def set_NumberList(self,NumberList):
-		self.add_query_param('NumberList',NumberList)
-
-	def get_InstanceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_Password(self): # String
+		return self.get_query_params().get('Password')
+
+	def set_Password(self, Password):  # String
+		self.add_query_param('Password', Password)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/AddPhoneNumberToSkillGroupsRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/PauseCampaignRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,35 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class AddPhoneNumberToSkillGroupsRequest(RpcRequest):
+class PauseCampaignRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'AddPhoneNumberToSkillGroups')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'PauseCampaign')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_Number(self):
-		return self.get_query_params().get('Number')
-
-	def set_Number(self,Number):
-		self.add_query_param('Number',Number)
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_SkillGroupIdList(self):
-		return self.get_query_params().get('SkillGroupIdList')
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_CampaignId(self): # String
+		return self.get_query_params().get('CampaignId')
 
-	def set_SkillGroupIdList(self,SkillGroupIdList):
-		self.add_query_param('SkillGroupIdList',SkillGroupIdList)
+	def set_CampaignId(self, CampaignId):  # String
+		self.add_query_param('CampaignId', CampaignId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/AddPhoneNumbersRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ModifyPhoneNumberRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,47 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class AddPhoneNumbersRequest(RpcRequest):
+class ModifyPhoneNumberRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'AddPhoneNumbers')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ModifyPhoneNumber')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ContactFlowId(self):
+	def get_ContactFlowId(self): # String
 		return self.get_query_params().get('ContactFlowId')
 
-	def set_ContactFlowId(self,ContactFlowId):
-		self.add_query_param('ContactFlowId',ContactFlowId)
-
-	def get_Usage(self):
+	def set_ContactFlowId(self, ContactFlowId):  # String
+		self.add_query_param('ContactFlowId', ContactFlowId)
+	def get_Usage(self): # String
 		return self.get_query_params().get('Usage')
 
-	def set_Usage(self,Usage):
-		self.add_query_param('Usage',Usage)
-
-	def get_NumberGroupId(self):
-		return self.get_query_params().get('NumberGroupId')
-
-	def set_NumberGroupId(self,NumberGroupId):
-		self.add_query_param('NumberGroupId',NumberGroupId)
-
-	def get_NumberList(self):
-		return self.get_query_params().get('NumberList')
-
-	def set_NumberList(self,NumberList):
-		self.add_query_param('NumberList',NumberList)
-
-	def get_InstanceId(self):
+	def set_Usage(self, Usage):  # String
+		self.add_query_param('Usage', Usage)
+	def get_Number(self): # String
+		return self.get_query_params().get('Number')
+
+	def set_Number(self, Number):  # String
+		self.add_query_param('Number', Number)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/AddSkillGroupsToUserRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ModifySkillLevelsOfUserRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,35 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class AddSkillGroupsToUserRequest(RpcRequest):
+class ModifySkillLevelsOfUserRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'AddSkillGroupsToUser')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ModifySkillLevelsOfUser')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_UserId(self):
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_InstanceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_SkillLevelList(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_SkillLevelList(self): # String
 		return self.get_query_params().get('SkillLevelList')
 
-	def set_SkillLevelList(self,SkillLevelList):
-		self.add_query_param('SkillLevelList',SkillLevelList)
+	def set_SkillLevelList(self, SkillLevelList):  # String
+		self.add_query_param('SkillLevelList', SkillLevelList)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/AddUsersToSkillGroupRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/AddUsersToSkillGroupRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,31 +20,29 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class AddUsersToSkillGroupRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'AddUsersToSkillGroup')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_UserSkillLevelList(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_UserSkillLevelList(self): # String
 		return self.get_query_params().get('UserSkillLevelList')
 
-	def set_UserSkillLevelList(self,UserSkillLevelList):
-		self.add_query_param('UserSkillLevelList',UserSkillLevelList)
-
-	def get_SkillGroupId(self):
+	def set_UserSkillLevelList(self, UserSkillLevelList):  # String
+		self.add_query_param('UserSkillLevelList', UserSkillLevelList)
+	def get_SkillGroupId(self): # String
 		return self.get_query_params().get('SkillGroupId')
 
-	def set_SkillGroupId(self,SkillGroupId):
-		self.add_query_param('SkillGroupId',SkillGroupId)
+	def set_SkillGroupId(self, SkillGroupId):  # String
+		self.add_query_param('SkillGroupId', SkillGroupId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/AnswerCallRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/TakeBreakRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,41 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class AnswerCallRequest(RpcRequest):
+class TakeBreakRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'AnswerCall')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'TakeBreak')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Code(self): # String
+		return self.get_query_params().get('Code')
 
-	def get_UserId(self):
+	def set_Code(self, Code):  # String
+		self.add_query_param('Code', Code)
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_DeviceId(self): # String
 		return self.get_query_params().get('DeviceId')
 
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_JobId(self):
-		return self.get_query_params().get('JobId')
-
-	def set_JobId(self,JobId):
-		self.add_query_param('JobId',JobId)
-
-	def get_InstanceId(self):
+	def set_DeviceId(self, DeviceId):  # String
+		self.add_query_param('DeviceId', DeviceId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/AssignUsersRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/RegisterDeviceRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,47 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class AssignUsersRequest(RpcRequest):
+class RegisterDeviceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'AssignUsers')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'RegisterDevice')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_UserId(self): # String
+		return self.get_query_params().get('UserId')
 
-	def get_RamIdList(self):
-		return self.get_query_params().get('RamIdList')
-
-	def set_RamIdList(self,RamIdList):
-		self.add_query_param('RamIdList',RamIdList)
-
-	def get_RoleId(self):
-		return self.get_query_params().get('RoleId')
-
-	def set_RoleId(self,RoleId):
-		self.add_query_param('RoleId',RoleId)
-
-	def get_WorkMode(self):
-		return self.get_query_params().get('WorkMode')
-
-	def set_WorkMode(self,WorkMode):
-		self.add_query_param('WorkMode',WorkMode)
-
-	def get_InstanceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_DeviceId(self): # String
+		return self.get_query_params().get('DeviceId')
+
+	def set_DeviceId(self, DeviceId):  # String
+		self.add_query_param('DeviceId', DeviceId)
+	def get_Password(self): # String
+		return self.get_query_params().get('Password')
+
+	def set_Password(self, Password):  # String
+		self.add_query_param('Password', Password)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_SkillLevelList(self):
-		return self.get_query_params().get('SkillLevelList')
-
-	def set_SkillLevelList(self,SkillLevelList):
-		self.add_query_param('SkillLevelList',SkillLevelList)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/BargeInCallRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/StartPredictiveCallRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,53 +16,63 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class BargeInCallRequest(RpcRequest):
+class StartPredictiveCallRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'BargeInCall')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'StartPredictiveCall')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ContactFlowId(self): # String
+		return self.get_query_params().get('ContactFlowId')
 
-	def get_UserId(self):
-		return self.get_query_params().get('UserId')
-
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
-		return self.get_query_params().get('DeviceId')
-
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_BargedUserId(self):
-		return self.get_query_params().get('BargedUserId')
-
-	def set_BargedUserId(self,BargedUserId):
-		self.add_query_param('BargedUserId',BargedUserId)
-
-	def get_JobId(self):
-		return self.get_query_params().get('JobId')
-
-	def set_JobId(self,JobId):
-		self.add_query_param('JobId',JobId)
-
-	def get_TimeoutSeconds(self):
+	def set_ContactFlowId(self, ContactFlowId):  # String
+		self.add_query_param('ContactFlowId', ContactFlowId)
+	def get_Callee(self): # String
+		return self.get_query_params().get('Callee')
+
+	def set_Callee(self, Callee):  # String
+		self.add_query_param('Callee', Callee)
+	def get_MaskedCallee(self): # String
+		return self.get_query_params().get('MaskedCallee')
+
+	def set_MaskedCallee(self, MaskedCallee):  # String
+		self.add_query_param('MaskedCallee', MaskedCallee)
+	def get_ContactFlowVariables(self): # String
+		return self.get_query_params().get('ContactFlowVariables')
+
+	def set_ContactFlowVariables(self, ContactFlowVariables):  # String
+		self.add_query_param('ContactFlowVariables', ContactFlowVariables)
+	def get_Tags(self): # String
+		return self.get_query_params().get('Tags')
+
+	def set_Tags(self, Tags):  # String
+		self.add_query_param('Tags', Tags)
+	def get_TimeoutSeconds(self): # Integer
 		return self.get_query_params().get('TimeoutSeconds')
 
-	def set_TimeoutSeconds(self,TimeoutSeconds):
-		self.add_query_param('TimeoutSeconds',TimeoutSeconds)
-
-	def get_InstanceId(self):
+	def set_TimeoutSeconds(self, TimeoutSeconds):  # Integer
+		self.add_query_param('TimeoutSeconds', TimeoutSeconds)
+	def get_Caller(self): # String
+		return self.get_query_params().get('Caller')
+
+	def set_Caller(self, Caller):  # String
+		self.add_query_param('Caller', Caller)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_SkillGroupId(self): # String
+		return self.get_query_params().get('SkillGroupId')
+
+	def set_SkillGroupId(self, SkillGroupId):  # String
+		self.add_query_param('SkillGroupId', SkillGroupId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/BlindTransferRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/BlindTransferRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,55 +20,49 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class BlindTransferRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'BlindTransfer')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_Transferee(self):
+	def get_Transferee(self): # String
 		return self.get_query_params().get('Transferee')
 
-	def set_Transferee(self,Transferee):
-		self.add_query_param('Transferee',Transferee)
-
-	def get_Transferor(self):
+	def set_Transferee(self, Transferee):  # String
+		self.add_query_param('Transferee', Transferee)
+	def get_Transferor(self): # String
 		return self.get_query_params().get('Transferor')
 
-	def set_Transferor(self,Transferor):
-		self.add_query_param('Transferor',Transferor)
-
-	def get_UserId(self):
+	def set_Transferor(self, Transferor):  # String
+		self.add_query_param('Transferor', Transferor)
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_DeviceId(self): # String
 		return self.get_query_params().get('DeviceId')
 
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_TimeoutSeconds(self):
+	def set_DeviceId(self, DeviceId):  # String
+		self.add_query_param('DeviceId', DeviceId)
+	def get_TimeoutSeconds(self): # Integer
 		return self.get_query_params().get('TimeoutSeconds')
 
-	def set_TimeoutSeconds(self,TimeoutSeconds):
-		self.add_query_param('TimeoutSeconds',TimeoutSeconds)
-
-	def get_JobId(self):
+	def set_TimeoutSeconds(self, TimeoutSeconds):  # Integer
+		self.add_query_param('TimeoutSeconds', TimeoutSeconds)
+	def get_JobId(self): # String
 		return self.get_query_params().get('JobId')
 
-	def set_JobId(self,JobId):
-		self.add_query_param('JobId',JobId)
-
-	def get_InstanceId(self):
+	def set_JobId(self, JobId):  # String
+		self.add_query_param('JobId', JobId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/CancelAttendedTransferRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetTurnCredentialsRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,41 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class CancelAttendedTransferRequest(RpcRequest):
+class GetTurnCredentialsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'CancelAttendedTransfer')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetTurnCredentials')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_UserId(self):
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
-		return self.get_query_params().get('DeviceId')
-
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_JobId(self):
-		return self.get_query_params().get('JobId')
-
-	def set_JobId(self,JobId):
-		self.add_query_param('JobId',JobId)
-
-	def get_InstanceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ChangeWorkModeRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ChangeWorkModeRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,37 +20,34 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class ChangeWorkModeRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ChangeWorkMode')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_WorkMode(self):
+	def get_WorkMode(self): # String
 		return self.get_query_params().get('WorkMode')
 
-	def set_WorkMode(self,WorkMode):
-		self.add_query_param('WorkMode',WorkMode)
-
-	def get_UserId(self):
+	def set_WorkMode(self, WorkMode):  # String
+		self.add_query_param('WorkMode', WorkMode)
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_DeviceId(self): # String
 		return self.get_query_params().get('DeviceId')
 
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_InstanceId(self):
+	def set_DeviceId(self, DeviceId):  # String
+		self.add_query_param('DeviceId', DeviceId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/CoachCallRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetCampaignRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,53 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class CoachCallRequest(RpcRequest):
+class GetCampaignRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'CoachCall')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetCampaign')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_CoachedUserId(self):
-		return self.get_query_params().get('CoachedUserId')
-
-	def set_CoachedUserId(self,CoachedUserId):
-		self.add_query_param('CoachedUserId',CoachedUserId)
-
-	def get_UserId(self):
-		return self.get_query_params().get('UserId')
-
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
-		return self.get_query_params().get('DeviceId')
-
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_JobId(self):
-		return self.get_query_params().get('JobId')
-
-	def set_JobId(self,JobId):
-		self.add_query_param('JobId',JobId)
-
-	def get_TimeoutSeconds(self):
-		return self.get_query_params().get('TimeoutSeconds')
-
-	def set_TimeoutSeconds(self,TimeoutSeconds):
-		self.add_query_param('TimeoutSeconds',TimeoutSeconds)
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_CampaignId(self): # String
+		return self.get_query_params().get('CampaignId')
+
+	def set_CampaignId(self, CampaignId):  # String
+		self.add_query_param('CampaignId', CampaignId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/CompleteAttendedTransferRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/SubmitCampaignRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,41 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class CompleteAttendedTransferRequest(RpcRequest):
+class SubmitCampaignRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'CompleteAttendedTransfer')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'SubmitCampaign')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_UserId(self):
-		return self.get_query_params().get('UserId')
-
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
-		return self.get_query_params().get('DeviceId')
-
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_JobId(self):
-		return self.get_query_params().get('JobId')
-
-	def set_JobId(self,JobId):
-		self.add_query_param('JobId',JobId)
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_CampaignId(self): # String
+		return self.get_query_params().get('CampaignId')
+
+	def set_CampaignId(self, CampaignId):  # String
+		self.add_query_param('CampaignId', CampaignId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/CreateCampaignRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/CreateCampaignRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,103 +20,89 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class CreateCampaignRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'CreateCampaign')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_QueueId(self):
+	def get_QueueId(self): # String
 		return self.get_query_params().get('QueueId')
 
-	def set_QueueId(self,QueueId):
-		self.add_query_param('QueueId',QueueId)
-
-	def get_ContactFlowId(self):
+	def set_QueueId(self, QueueId):  # String
+		self.add_query_param('QueueId', QueueId)
+	def get_ContactFlowId(self): # String
 		return self.get_query_params().get('ContactFlowId')
 
-	def set_ContactFlowId(self,ContactFlowId):
-		self.add_query_param('ContactFlowId',ContactFlowId)
-
-	def get_Simulation(self):
+	def set_ContactFlowId(self, ContactFlowId):  # String
+		self.add_query_param('ContactFlowId', ContactFlowId)
+	def get_Simulation(self): # Boolean
 		return self.get_query_params().get('Simulation')
 
-	def set_Simulation(self,Simulation):
-		self.add_query_param('Simulation',Simulation)
-
-	def get_EndTime(self):
+	def set_Simulation(self, Simulation):  # Boolean
+		self.add_query_param('Simulation', Simulation)
+	def get_EndTime(self): # String
 		return self.get_query_params().get('EndTime')
 
-	def set_EndTime(self,EndTime):
-		self.add_query_param('EndTime',EndTime)
-
-	def get_StartTime(self):
+	def set_EndTime(self, EndTime):  # String
+		self.add_query_param('EndTime', EndTime)
+	def get_StartTime(self): # String
 		return self.get_query_params().get('StartTime')
 
-	def set_StartTime(self,StartTime):
-		self.add_query_param('StartTime',StartTime)
-
-	def get_MaxAttemptCount(self):
+	def set_StartTime(self, StartTime):  # String
+		self.add_query_param('StartTime', StartTime)
+	def get_MaxAttemptCount(self): # Long
 		return self.get_query_params().get('MaxAttemptCount')
 
-	def set_MaxAttemptCount(self,MaxAttemptCount):
-		self.add_query_param('MaxAttemptCount',MaxAttemptCount)
-
-	def get_StrategyParameters(self):
+	def set_MaxAttemptCount(self, MaxAttemptCount):  # Long
+		self.add_query_param('MaxAttemptCount', MaxAttemptCount)
+	def get_StrategyParameters(self): # String
 		return self.get_query_params().get('StrategyParameters')
 
-	def set_StrategyParameters(self,StrategyParameters):
-		self.add_query_param('StrategyParameters',StrategyParameters)
-
-	def get_CaseFileKey(self):
+	def set_StrategyParameters(self, StrategyParameters):  # String
+		self.add_query_param('StrategyParameters', StrategyParameters)
+	def get_CaseFileKey(self): # String
 		return self.get_query_params().get('CaseFileKey')
 
-	def set_CaseFileKey(self,CaseFileKey):
-		self.add_query_param('CaseFileKey',CaseFileKey)
-
-	def get_MinAttemptInterval(self):
+	def set_CaseFileKey(self, CaseFileKey):  # String
+		self.add_query_param('CaseFileKey', CaseFileKey)
+	def get_MinAttemptInterval(self): # Long
 		return self.get_query_params().get('MinAttemptInterval')
 
-	def set_MinAttemptInterval(self,MinAttemptInterval):
-		self.add_query_param('MinAttemptInterval',MinAttemptInterval)
-
-	def get_InstanceId(self):
+	def set_MinAttemptInterval(self, MinAttemptInterval):  # Long
+		self.add_query_param('MinAttemptInterval', MinAttemptInterval)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_SimulationParameters(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_SimulationParameters(self): # String
 		return self.get_query_params().get('SimulationParameters')
 
-	def set_SimulationParameters(self,SimulationParameters):
-		self.add_query_param('SimulationParameters',SimulationParameters)
-
-	def get_Name(self):
+	def set_SimulationParameters(self, SimulationParameters):  # String
+		self.add_query_param('SimulationParameters', SimulationParameters)
+	def get_Name(self): # String
 		return self.get_query_params().get('Name')
 
-	def set_Name(self,Name):
-		self.add_query_param('Name',Name)
-
-	def get_StrategyType(self):
+	def set_Name(self, Name):  # String
+		self.add_query_param('Name', Name)
+	def get_StrategyType(self): # String
 		return self.get_query_params().get('StrategyType')
 
-	def set_StrategyType(self,StrategyType):
-		self.add_query_param('StrategyType',StrategyType)
-
-	def get_CaseList(self):
+	def set_StrategyType(self, StrategyType):  # String
+		self.add_query_param('StrategyType', StrategyType)
+	def get_CaseList(self): # String
 		return self.get_query_params().get('CaseList')
 
-	def set_CaseList(self,CaseList):
-		self.add_query_param('CaseList',CaseList)
-
-	def get_CallableTime(self):
+	def set_CaseList(self, CaseList):  # String
+		self.add_query_param('CaseList', CaseList)
+	def get_CallableTime(self): # String
 		return self.get_query_params().get('CallableTime')
 
-	def set_CallableTime(self,CallableTime):
-		self.add_query_param('CallableTime',CallableTime)
+	def set_CallableTime(self, CallableTime):  # String
+		self.add_query_param('CallableTime', CallableTime)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/CreateInstanceRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/CreateInstanceRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,43 +20,39 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class CreateInstanceRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'CreateInstance')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_AdminRamIdList(self):
+	def get_AdminRamIdList(self): # String
 		return self.get_query_params().get('AdminRamIdList')
 
-	def set_AdminRamIdList(self,AdminRamIdList):
-		self.add_query_param('AdminRamIdList',AdminRamIdList)
-
-	def get_DomainName(self):
+	def set_AdminRamIdList(self, AdminRamIdList):  # String
+		self.add_query_param('AdminRamIdList', AdminRamIdList)
+	def get_DomainName(self): # String
 		return self.get_query_params().get('DomainName')
 
-	def set_DomainName(self,DomainName):
-		self.add_query_param('DomainName',DomainName)
-
-	def get_Description(self):
+	def set_DomainName(self, DomainName):  # String
+		self.add_query_param('DomainName', DomainName)
+	def get_Description(self): # String
 		return self.get_query_params().get('Description')
 
-	def set_Description(self,Description):
-		self.add_query_param('Description',Description)
-
-	def get_NumberList(self):
+	def set_Description(self, Description):  # String
+		self.add_query_param('Description', Description)
+	def get_NumberList(self): # String
 		return self.get_query_params().get('NumberList')
 
-	def set_NumberList(self,NumberList):
-		self.add_query_param('NumberList',NumberList)
-
-	def get_Name(self):
+	def set_NumberList(self, NumberList):  # String
+		self.add_query_param('NumberList', NumberList)
+	def get_Name(self): # String
 		return self.get_query_params().get('Name')
 
-	def set_Name(self,Name):
-		self.add_query_param('Name',Name)
+	def set_Name(self, Name):  # String
+		self.add_query_param('Name', Name)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/CreateSkillGroupRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetSkillGroupRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,41 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class CreateSkillGroupRequest(RpcRequest):
+class GetSkillGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'CreateSkillGroup')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetSkillGroup')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_Description(self):
-		return self.get_query_params().get('Description')
-
-	def set_Description(self,Description):
-		self.add_query_param('Description',Description)
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_DisplayName(self):
-		return self.get_query_params().get('DisplayName')
-
-	def set_DisplayName(self,DisplayName):
-		self.add_query_param('DisplayName',DisplayName)
-
-	def get_Name(self):
-		return self.get_query_params().get('Name')
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_SkillGroupId(self): # String
+		return self.get_query_params().get('SkillGroupId')
 
-	def set_Name(self,Name):
-		self.add_query_param('Name',Name)
+	def set_SkillGroupId(self, SkillGroupId):  # String
+		self.add_query_param('SkillGroupId', SkillGroupId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/CreateUserRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/CreateUserRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,67 +20,64 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class CreateUserRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'CreateUser')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_LoginName(self):
+	def get_LoginName(self): # String
 		return self.get_query_params().get('LoginName')
 
-	def set_LoginName(self,LoginName):
-		self.add_query_param('LoginName',LoginName)
-
-	def get_RoleId(self):
+	def set_LoginName(self, LoginName):  # String
+		self.add_query_param('LoginName', LoginName)
+	def get_RoleId(self): # String
 		return self.get_query_params().get('RoleId')
 
-	def set_RoleId(self,RoleId):
-		self.add_query_param('RoleId',RoleId)
-
-	def get_Mobile(self):
+	def set_RoleId(self, RoleId):  # String
+		self.add_query_param('RoleId', RoleId)
+	def get_Mobile(self): # String
 		return self.get_query_params().get('Mobile')
 
-	def set_Mobile(self,Mobile):
-		self.add_query_param('Mobile',Mobile)
-
-	def get_WorkMode(self):
+	def set_Mobile(self, Mobile):  # String
+		self.add_query_param('Mobile', Mobile)
+	def get_WorkMode(self): # String
 		return self.get_query_params().get('WorkMode')
 
-	def set_WorkMode(self,WorkMode):
-		self.add_query_param('WorkMode',WorkMode)
-
-	def get_InstanceId(self):
+	def set_WorkMode(self, WorkMode):  # String
+		self.add_query_param('WorkMode', WorkMode)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_DisplayName(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_DisplayName(self): # String
 		return self.get_query_params().get('DisplayName')
 
-	def set_DisplayName(self,DisplayName):
-		self.add_query_param('DisplayName',DisplayName)
-
-	def get_ResetPassword(self):
+	def set_DisplayName(self, DisplayName):  # String
+		self.add_query_param('DisplayName', DisplayName)
+	def get_ResetPassword(self): # Boolean
 		return self.get_query_params().get('ResetPassword')
 
-	def set_ResetPassword(self,ResetPassword):
-		self.add_query_param('ResetPassword',ResetPassword)
-
-	def get_SkillLevelList(self):
+	def set_ResetPassword(self, ResetPassword):  # Boolean
+		self.add_query_param('ResetPassword', ResetPassword)
+	def get_DisplayId(self): # String
+		return self.get_query_params().get('DisplayId')
+
+	def set_DisplayId(self, DisplayId):  # String
+		self.add_query_param('DisplayId', DisplayId)
+	def get_SkillLevelList(self): # String
 		return self.get_query_params().get('SkillLevelList')
 
-	def set_SkillLevelList(self,SkillLevelList):
-		self.add_query_param('SkillLevelList',SkillLevelList)
-
-	def get_Email(self):
+	def set_SkillLevelList(self, SkillLevelList):  # String
+		self.add_query_param('SkillLevelList', SkillLevelList)
+	def get_Email(self): # String
 		return self.get_query_params().get('Email')
 
-	def set_Email(self,Email):
-		self.add_query_param('Email',Email)
+	def set_Email(self, Email):  # String
+		self.add_query_param('Email', Email)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/DeleteSkillGroupRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/RemovePhoneNumberFromSkillGroupsRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,35 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class DeleteSkillGroupRequest(RpcRequest):
+class RemovePhoneNumberFromSkillGroupsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'DeleteSkillGroup')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'RemovePhoneNumberFromSkillGroups')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Number(self): # String
+		return self.get_query_params().get('Number')
 
-	def get_InstanceId(self):
+	def set_Number(self, Number):  # String
+		self.add_query_param('Number', Number)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_SkillGroupId(self):
-		return self.get_query_params().get('SkillGroupId')
-
-	def set_SkillGroupId(self,SkillGroupId):
-		self.add_query_param('SkillGroupId',SkillGroupId)
-
-	def get_Force(self):
-		return self.get_query_params().get('Force')
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_SkillGroupIdList(self): # String
+		return self.get_query_params().get('SkillGroupIdList')
 
-	def set_Force(self,Force):
-		self.add_query_param('Force',Force)
+	def set_SkillGroupIdList(self, SkillGroupIdList):  # String
+		self.add_query_param('SkillGroupIdList', SkillGroupIdList)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetCallDetailRecordRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListMultiChannelRecordingsRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,29 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class GetCallDetailRecordRequest(RpcRequest):
+class ListMultiChannelRecordingsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetCallDetailRecord')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListMultiChannelRecordings')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ContactId(self):
+	def get_ContactId(self): # String
 		return self.get_query_params().get('ContactId')
 
-	def set_ContactId(self,ContactId):
-		self.add_query_param('ContactId',ContactId)
-
-	def get_InstanceId(self):
+	def set_ContactId(self, ContactId):  # String
+		self.add_query_param('ContactId', ContactId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetCampaignRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetInstanceRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,29 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class GetCampaignRequest(RpcRequest):
+class GetInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetCampaign')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetInstance')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_CampaignId(self):
-		return self.get_query_params().get('CampaignId')
-
-	def set_CampaignId(self,CampaignId):
-		self.add_query_param('CampaignId',CampaignId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetCaseFileUploadUrlRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/RemoveUsersRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,29 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class GetCaseFileUploadUrlRequest(RpcRequest):
+class RemoveUsersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetCaseFileUploadUrl')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'RemoveUsers')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_UserIdList(self): # String
+		return self.get_query_params().get('UserIdList')
 
-	def get_InstanceId(self):
+	def set_UserIdList(self, UserIdList):  # String
+		self.add_query_param('UserIdList', UserIdList)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_FileName(self):
-		return self.get_query_params().get('FileName')
-
-	def set_FileName(self,FileName):
-		self.add_query_param('FileName',FileName)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetHistoricalCallerReportRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetHistoricalCallerReportRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,37 +20,34 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class GetHistoricalCallerReportRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetHistoricalCallerReport')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_StopTime(self):
+	def get_StopTime(self): # Long
 		return self.get_query_params().get('StopTime')
 
-	def set_StopTime(self,StopTime):
-		self.add_query_param('StopTime',StopTime)
-
-	def get_StartTime(self):
+	def set_StopTime(self, StopTime):  # Long
+		self.add_query_param('StopTime', StopTime)
+	def get_StartTime(self): # Long
 		return self.get_query_params().get('StartTime')
 
-	def set_StartTime(self,StartTime):
-		self.add_query_param('StartTime',StartTime)
-
-	def get_CallingNumber(self):
+	def set_StartTime(self, StartTime):  # Long
+		self.add_query_param('StartTime', StartTime)
+	def get_CallingNumber(self): # String
 		return self.get_query_params().get('CallingNumber')
 
-	def set_CallingNumber(self,CallingNumber):
-		self.add_query_param('CallingNumber',CallingNumber)
-
-	def get_InstanceId(self):
+	def set_CallingNumber(self, CallingNumber):  # String
+		self.add_query_param('CallingNumber', CallingNumber)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetHistoricalInstanceReportRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListIntervalInstanceReportRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,35 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class GetHistoricalInstanceReportRequest(RpcRequest):
+class ListIntervalInstanceReportRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetHistoricalInstanceReport')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListIntervalInstanceReport')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_EndTime(self):
+	def get_EndTime(self): # Long
 		return self.get_query_params().get('EndTime')
 
-	def set_EndTime(self,EndTime):
-		self.add_query_param('EndTime',EndTime)
-
-	def get_StartTime(self):
+	def set_EndTime(self, EndTime):  # Long
+		self.add_query_param('EndTime', EndTime)
+	def get_StartTime(self): # Long
 		return self.get_query_params().get('StartTime')
 
-	def set_StartTime(self,StartTime):
-		self.add_query_param('StartTime',StartTime)
-
-	def get_InstanceId(self):
+	def set_StartTime(self, StartTime):  # Long
+		self.add_query_param('StartTime', StartTime)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_Interval(self): # String
+		return self.get_query_params().get('Interval')
+
+	def set_Interval(self, Interval):  # String
+		self.add_query_param('Interval', Interval)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetInstanceRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetRealtimeInstanceStatesRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class GetInstanceRequest(RpcRequest):
+class GetRealtimeInstanceStatesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetInstance')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetRealtimeInstanceStates')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetInstanceTrendingReportRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListIntervalAgentReportRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,35 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class GetInstanceTrendingReportRequest(RpcRequest):
+class ListIntervalAgentReportRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetInstanceTrendingReport')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListIntervalAgentReport')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_AgentId(self): # String
+		return self.get_query_params().get('AgentId')
 
-	def get_EndTime(self):
+	def set_AgentId(self, AgentId):  # String
+		self.add_query_param('AgentId', AgentId)
+	def get_EndTime(self): # Long
 		return self.get_query_params().get('EndTime')
 
-	def set_EndTime(self,EndTime):
-		self.add_query_param('EndTime',EndTime)
-
-	def get_StartTime(self):
+	def set_EndTime(self, EndTime):  # Long
+		self.add_query_param('EndTime', EndTime)
+	def get_StartTime(self): # Long
 		return self.get_query_params().get('StartTime')
 
-	def set_StartTime(self,StartTime):
-		self.add_query_param('StartTime',StartTime)
-
-	def get_InstanceId(self):
+	def set_StartTime(self, StartTime):  # Long
+		self.add_query_param('StartTime', StartTime)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_Interval(self): # String
+		return self.get_query_params().get('Interval')
+
+	def set_Interval(self, Interval):  # String
+		self.add_query_param('Interval', Interval)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetLoginDetailsRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetLoginDetailsRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,25 +20,24 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class GetLoginDetailsRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetLoginDetails')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_UserId(self):
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_InstanceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetMonoRecordingRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListSipCallRecordsRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,29 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class GetMonoRecordingRequest(RpcRequest):
+class ListSipCallRecordsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetMonoRecording')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListSipCallRecords')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ContactIdList(self): # String
+		return self.get_query_params().get('ContactIdList')
 
-	def get_ContactId(self):
-		return self.get_query_params().get('ContactId')
-
-	def set_ContactId(self,ContactId):
-		self.add_query_param('ContactId',ContactId)
-
-	def get_InstanceId(self):
+	def set_ContactIdList(self, ContactIdList):  # String
+		self.add_query_param('ContactIdList', ContactIdList)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetMultiChannelRecordingRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListPrivilegesOfUserRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,29 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class GetMultiChannelRecordingRequest(RpcRequest):
+class ListPrivilegesOfUserRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetMultiChannelRecording')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListPrivilegesOfUser')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ContactId(self):
-		return self.get_query_params().get('ContactId')
-
-	def set_ContactId(self,ContactId):
-		self.add_query_param('ContactId',ContactId)
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetNumberLocationRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetTurnServerListRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,29 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class GetNumberLocationRequest(RpcRequest):
+class GetTurnServerListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetNumberLocation')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetTurnServerList')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_Number(self):
-		return self.get_query_params().get('Number')
-
-	def set_Number(self,Number):
-		self.add_query_param('Number',Number)
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetRealtimeInstanceStatesRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ImportCustomCallTaggingRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,23 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class GetRealtimeInstanceStatesRequest(RpcRequest):
+class ImportCustomCallTaggingRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetRealtimeInstanceStates')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ImportCustomCallTagging')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_FilePath(self): # String
+		return self.get_query_params().get('FilePath')
+
+	def set_FilePath(self, FilePath):  # String
+		self.add_query_param('FilePath', FilePath)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetTurnCredentialsRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetNumberLocationRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,29 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class GetTurnCredentialsRequest(RpcRequest):
+class GetNumberLocationRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetTurnCredentials')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetNumberLocation')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Number(self): # String
+		return self.get_query_params().get('Number')
 
-	def get_UserId(self):
-		return self.get_query_params().get('UserId')
-
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_InstanceId(self):
+	def set_Number(self, Number):  # String
+		self.add_query_param('Number', Number)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetTurnServerListRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetCallDetailRecordRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,23 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class GetTurnServerListRequest(RpcRequest):
+class GetCallDetailRecordRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetTurnServerList')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetCallDetailRecord')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ContactId(self): # String
+		return self.get_query_params().get('ContactId')
 
-	def get_InstanceId(self):
+	def set_ContactId(self, ContactId):  # String
+		self.add_query_param('ContactId', ContactId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/GetUserRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/UnregisterDeviceRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,35 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class GetUserRequest(RpcRequest):
+class UnregisterDeviceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetUser')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'UnregisterDevice')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_Extension(self):
-		return self.get_query_params().get('Extension')
-
-	def set_Extension(self,Extension):
-		self.add_query_param('Extension',Extension)
-
-	def get_UserId(self):
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_InstanceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/HoldCallRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/HoldCallRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,49 +20,44 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class HoldCallRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'HoldCall')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_UserId(self):
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_DeviceId(self): # String
 		return self.get_query_params().get('DeviceId')
 
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_JobId(self):
+	def set_DeviceId(self, DeviceId):  # String
+		self.add_query_param('DeviceId', DeviceId)
+	def get_JobId(self): # String
 		return self.get_query_params().get('JobId')
 
-	def set_JobId(self,JobId):
-		self.add_query_param('JobId',JobId)
-
-	def get_InstanceId(self):
+	def set_JobId(self, JobId):  # String
+		self.add_query_param('JobId', JobId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_Music(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_Music(self): # String
 		return self.get_query_params().get('Music')
 
-	def set_Music(self,Music):
-		self.add_query_param('Music',Music)
-
-	def get_ChannelId(self):
+	def set_Music(self, Music):  # String
+		self.add_query_param('Music', Music)
+	def get_ChannelId(self): # String
 		return self.get_query_params().get('ChannelId')
 
-	def set_ChannelId(self,ChannelId):
-		self.add_query_param('ChannelId',ChannelId)
+	def set_ChannelId(self, ChannelId):  # String
+		self.add_query_param('ChannelId', ChannelId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/InitiateAttendedTransferRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/InitiateAttendedTransferRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,55 +20,49 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class InitiateAttendedTransferRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'InitiateAttendedTransfer')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_Transferee(self):
+	def get_Transferee(self): # String
 		return self.get_query_params().get('Transferee')
 
-	def set_Transferee(self,Transferee):
-		self.add_query_param('Transferee',Transferee)
-
-	def get_Transferor(self):
+	def set_Transferee(self, Transferee):  # String
+		self.add_query_param('Transferee', Transferee)
+	def get_Transferor(self): # String
 		return self.get_query_params().get('Transferor')
 
-	def set_Transferor(self,Transferor):
-		self.add_query_param('Transferor',Transferor)
-
-	def get_UserId(self):
+	def set_Transferor(self, Transferor):  # String
+		self.add_query_param('Transferor', Transferor)
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_DeviceId(self): # String
 		return self.get_query_params().get('DeviceId')
 
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_TimeoutSeconds(self):
+	def set_DeviceId(self, DeviceId):  # String
+		self.add_query_param('DeviceId', DeviceId)
+	def get_TimeoutSeconds(self): # Integer
 		return self.get_query_params().get('TimeoutSeconds')
 
-	def set_TimeoutSeconds(self,TimeoutSeconds):
-		self.add_query_param('TimeoutSeconds',TimeoutSeconds)
-
-	def get_JobId(self):
+	def set_TimeoutSeconds(self, TimeoutSeconds):  # Integer
+		self.add_query_param('TimeoutSeconds', TimeoutSeconds)
+	def get_JobId(self): # String
 		return self.get_query_params().get('JobId')
 
-	def set_JobId(self,JobId):
-		self.add_query_param('JobId',JobId)
-
-	def get_InstanceId(self):
+	def set_JobId(self, JobId):  # String
+		self.add_query_param('JobId', JobId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/InterceptCallRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/BargeInCallRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,53 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class InterceptCallRequest(RpcRequest):
+class BargeInCallRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'InterceptCall')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'BargeInCall')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_InterceptedUserId(self):
-		return self.get_query_params().get('InterceptedUserId')
-
-	def set_InterceptedUserId(self,InterceptedUserId):
-		self.add_query_param('InterceptedUserId',InterceptedUserId)
-
-	def get_UserId(self):
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_DeviceId(self): # String
 		return self.get_query_params().get('DeviceId')
 
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_JobId(self):
+	def set_DeviceId(self, DeviceId):  # String
+		self.add_query_param('DeviceId', DeviceId)
+	def get_BargedUserId(self): # String
+		return self.get_query_params().get('BargedUserId')
+
+	def set_BargedUserId(self, BargedUserId):  # String
+		self.add_query_param('BargedUserId', BargedUserId)
+	def get_JobId(self): # String
 		return self.get_query_params().get('JobId')
 
-	def set_JobId(self,JobId):
-		self.add_query_param('JobId',JobId)
-
-	def get_TimeoutSeconds(self):
+	def set_JobId(self, JobId):  # String
+		self.add_query_param('JobId', JobId)
+	def get_TimeoutSeconds(self): # Integer
 		return self.get_query_params().get('TimeoutSeconds')
 
-	def set_TimeoutSeconds(self,TimeoutSeconds):
-		self.add_query_param('TimeoutSeconds',TimeoutSeconds)
-
-	def get_InstanceId(self):
+	def set_TimeoutSeconds(self, TimeoutSeconds):  # Integer
+		self.add_query_param('TimeoutSeconds', TimeoutSeconds)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/LaunchAuthenticationRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ResumeCampaignRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,47 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class LaunchAuthenticationRequest(RpcRequest):
+class ResumeCampaignRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'LaunchAuthentication')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ResumeCampaign')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ContactFlowId(self):
-		return self.get_query_params().get('ContactFlowId')
-
-	def set_ContactFlowId(self,ContactFlowId):
-		self.add_query_param('ContactFlowId',ContactFlowId)
-
-	def get_UserId(self):
-		return self.get_query_params().get('UserId')
-
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
-		return self.get_query_params().get('DeviceId')
-
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_JobId(self):
-		return self.get_query_params().get('JobId')
-
-	def set_JobId(self,JobId):
-		self.add_query_param('JobId',JobId)
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_CampaignId(self): # String
+		return self.get_query_params().get('CampaignId')
+
+	def set_CampaignId(self, CampaignId):  # String
+		self.add_query_param('CampaignId', CampaignId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/LaunchSurveyRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/MonitorCallRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,47 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class LaunchSurveyRequest(RpcRequest):
+class MonitorCallRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'LaunchSurvey')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'MonitorCall')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ContactFlowId(self):
-		return self.get_query_params().get('ContactFlowId')
-
-	def set_ContactFlowId(self,ContactFlowId):
-		self.add_query_param('ContactFlowId',ContactFlowId)
-
-	def get_UserId(self):
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_DeviceId(self): # String
 		return self.get_query_params().get('DeviceId')
 
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_JobId(self):
-		return self.get_query_params().get('JobId')
-
-	def set_JobId(self,JobId):
-		self.add_query_param('JobId',JobId)
-
-	def get_InstanceId(self):
+	def set_DeviceId(self, DeviceId):  # String
+		self.add_query_param('DeviceId', DeviceId)
+	def get_TimeoutSeconds(self): # Integer
+		return self.get_query_params().get('TimeoutSeconds')
+
+	def set_TimeoutSeconds(self, TimeoutSeconds):  # Integer
+		self.add_query_param('TimeoutSeconds', TimeoutSeconds)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_MonitoredUserId(self): # String
+		return self.get_query_params().get('MonitoredUserId')
+
+	def set_MonitoredUserId(self, MonitoredUserId):  # String
+		self.add_query_param('MonitoredUserId', MonitoredUserId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListAgentStateLogsRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListRecentCallDetailRecordsRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,41 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListAgentStateLogsRequest(RpcRequest):
+class ListRecentCallDetailRecordsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListAgentStateLogs')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListRecentCallDetailRecords')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Criteria(self): # String
+		return self.get_query_params().get('Criteria')
 
-	def get_AgentId(self):
-		return self.get_query_params().get('AgentId')
-
-	def set_AgentId(self,AgentId):
-		self.add_query_param('AgentId',AgentId)
-
-	def get_EndTime(self):
+	def set_Criteria(self, Criteria):  # String
+		self.add_query_param('Criteria', Criteria)
+	def get_EndTime(self): # Long
 		return self.get_query_params().get('EndTime')
 
-	def set_EndTime(self,EndTime):
-		self.add_query_param('EndTime',EndTime)
-
-	def get_StartTime(self):
-		return self.get_query_params().get('StartTime')
-
-	def set_StartTime(self,StartTime):
-		self.add_query_param('StartTime',StartTime)
-
-	def get_InstanceId(self):
+	def set_EndTime(self, EndTime):  # Long
+		self.add_query_param('EndTime', EndTime)
+	def get_StartTime(self): # Long
+		return self.get_body_params().get('StartTime')
+
+	def set_StartTime(self, StartTime):  # Long
+		self.add_body_params('StartTime', StartTime)
+	def get_PageNumber(self): # Integer
+		return self.get_query_params().get('PageNumber')
+
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_PageSize(self): # Integer
+		return self.get_query_params().get('PageSize')
+
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListAttemptsRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListAttemptsRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,91 +20,79 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class ListAttemptsRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListAttempts')
-		self.set_method('GET')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ContactId(self):
+	def get_ContactId(self): # String
 		return self.get_query_params().get('ContactId')
 
-	def set_ContactId(self,ContactId):
-		self.add_query_param('ContactId',ContactId)
-
-	def get_CampaignId(self):
+	def set_ContactId(self, ContactId):  # String
+		self.add_query_param('ContactId', ContactId)
+	def get_CampaignId(self): # String
 		return self.get_query_params().get('CampaignId')
 
-	def set_CampaignId(self,CampaignId):
-		self.add_query_param('CampaignId',CampaignId)
-
-	def get_Callee(self):
+	def set_CampaignId(self, CampaignId):  # String
+		self.add_query_param('CampaignId', CampaignId)
+	def get_Callee(self): # String
 		return self.get_query_params().get('Callee')
 
-	def set_Callee(self,Callee):
-		self.add_query_param('Callee',Callee)
-
-	def get_StartTime(self):
+	def set_Callee(self, Callee):  # String
+		self.add_query_param('Callee', Callee)
+	def get_StartTime(self): # Long
 		return self.get_query_params().get('StartTime')
 
-	def set_StartTime(self,StartTime):
-		self.add_query_param('StartTime',StartTime)
-
-	def get_PageNumber(self):
+	def set_StartTime(self, StartTime):  # Long
+		self.add_query_param('StartTime', StartTime)
+	def get_PageNumber(self): # Integer
 		return self.get_query_params().get('PageNumber')
 
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
-
-	def get_PageSize(self):
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
 
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
-
-	def get_QueueId(self):
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
+	def get_QueueId(self): # String
 		return self.get_query_params().get('QueueId')
 
-	def set_QueueId(self,QueueId):
-		self.add_query_param('QueueId',QueueId)
-
-	def get_AgentId(self):
+	def set_QueueId(self, QueueId):  # String
+		self.add_query_param('QueueId', QueueId)
+	def get_AgentId(self): # String
 		return self.get_query_params().get('AgentId')
 
-	def set_AgentId(self,AgentId):
-		self.add_query_param('AgentId',AgentId)
-
-	def get_EndTime(self):
+	def set_AgentId(self, AgentId):  # String
+		self.add_query_param('AgentId', AgentId)
+	def get_EndTime(self): # Long
 		return self.get_query_params().get('EndTime')
 
-	def set_EndTime(self,EndTime):
-		self.add_query_param('EndTime',EndTime)
-
-	def get_Caller(self):
+	def set_EndTime(self, EndTime):  # Long
+		self.add_query_param('EndTime', EndTime)
+	def get_Caller(self): # String
 		return self.get_query_params().get('Caller')
 
-	def set_Caller(self,Caller):
-		self.add_query_param('Caller',Caller)
-
-	def get_InstanceId(self):
+	def set_Caller(self, Caller):  # String
+		self.add_query_param('Caller', Caller)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_CaseId(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_CaseId(self): # String
 		return self.get_query_params().get('CaseId')
 
-	def set_CaseId(self,CaseId):
-		self.add_query_param('CaseId',CaseId)
-
-	def get_AttemptId(self):
+	def set_CaseId(self, CaseId):  # String
+		self.add_query_param('CaseId', CaseId)
+	def get_AttemptId(self): # String
 		return self.get_query_params().get('AttemptId')
 
-	def set_AttemptId(self,AttemptId):
-		self.add_query_param('AttemptId',AttemptId)
+	def set_AttemptId(self, AttemptId):  # String
+		self.add_query_param('AttemptId', AttemptId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListBriefSkillGroupsRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListUsersRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,41 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListBriefSkillGroupsRequest(RpcRequest):
+class ListUsersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListBriefSkillGroups')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListUsers')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_PageNumber(self):
+	def get_PageNumber(self): # Integer
 		return self.get_query_params().get('PageNumber')
 
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
-
-	def get_SearchPattern(self):
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_SearchPattern(self): # String
 		return self.get_query_params().get('SearchPattern')
 
-	def set_SearchPattern(self,SearchPattern):
-		self.add_query_param('SearchPattern',SearchPattern)
-
-	def get_InstanceId(self):
+	def set_SearchPattern(self, SearchPattern):  # String
+		self.add_query_param('SearchPattern', SearchPattern)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_PageSize(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
 
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListCampaignTrendingReportRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetInstanceTrendingReportRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,41 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListCampaignTrendingReportRequest(RpcRequest):
+class GetInstanceTrendingReportRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListCampaignTrendingReport')
-		self.set_method('GET')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetInstanceTrendingReport')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_CampaignId(self):
-		return self.get_query_params().get('CampaignId')
-
-	def set_CampaignId(self,CampaignId):
-		self.add_query_param('CampaignId',CampaignId)
-
-	def get_EndTime(self):
+	def get_EndTime(self): # Long
 		return self.get_query_params().get('EndTime')
 
-	def set_EndTime(self,EndTime):
-		self.add_query_param('EndTime',EndTime)
-
-	def get_StartTime(self):
+	def set_EndTime(self, EndTime):  # Long
+		self.add_query_param('EndTime', EndTime)
+	def get_StartTime(self): # Long
 		return self.get_query_params().get('StartTime')
 
-	def set_StartTime(self,StartTime):
-		self.add_query_param('StartTime',StartTime)
-
-	def get_InstanceId(self):
+	def set_StartTime(self, StartTime):  # Long
+		self.add_query_param('StartTime', StartTime)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListCampaignsRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListCampaignsRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,73 +20,64 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class ListCampaignsRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListCampaigns')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ActualStartTimeTo(self):
+	def get_ActualStartTimeTo(self): # String
 		return self.get_query_params().get('ActualStartTimeTo')
 
-	def set_ActualStartTimeTo(self,ActualStartTimeTo):
-		self.add_query_param('ActualStartTimeTo',ActualStartTimeTo)
-
-	def get_QueueId(self):
+	def set_ActualStartTimeTo(self, ActualStartTimeTo):  # String
+		self.add_query_param('ActualStartTimeTo', ActualStartTimeTo)
+	def get_QueueId(self): # String
 		return self.get_query_params().get('QueueId')
 
-	def set_QueueId(self,QueueId):
-		self.add_query_param('QueueId',QueueId)
-
-	def get_ActualStartTimeFrom(self):
+	def set_QueueId(self, QueueId):  # String
+		self.add_query_param('QueueId', QueueId)
+	def get_ActualStartTimeFrom(self): # String
 		return self.get_query_params().get('ActualStartTimeFrom')
 
-	def set_ActualStartTimeFrom(self,ActualStartTimeFrom):
-		self.add_query_param('ActualStartTimeFrom',ActualStartTimeFrom)
-
-	def get_PageNumber(self):
+	def set_ActualStartTimeFrom(self, ActualStartTimeFrom):  # String
+		self.add_query_param('ActualStartTimeFrom', ActualStartTimeFrom)
+	def get_PageNumber(self): # Long
 		return self.get_query_params().get('PageNumber')
 
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
-
-	def get_PlanedStartTimeFrom(self):
+	def set_PageNumber(self, PageNumber):  # Long
+		self.add_query_param('PageNumber', PageNumber)
+	def get_PlanedStartTimeFrom(self): # String
 		return self.get_query_params().get('PlanedStartTimeFrom')
 
-	def set_PlanedStartTimeFrom(self,PlanedStartTimeFrom):
-		self.add_query_param('PlanedStartTimeFrom',PlanedStartTimeFrom)
-
-	def get_InstanceId(self):
+	def set_PlanedStartTimeFrom(self, PlanedStartTimeFrom):  # String
+		self.add_query_param('PlanedStartTimeFrom', PlanedStartTimeFrom)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_Name(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_Name(self): # String
 		return self.get_query_params().get('Name')
 
-	def set_Name(self,Name):
-		self.add_query_param('Name',Name)
-
-	def get_PageSize(self):
+	def set_Name(self, Name):  # String
+		self.add_query_param('Name', Name)
+	def get_PageSize(self): # Long
 		return self.get_query_params().get('PageSize')
 
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
-
-	def get_PlanedStartTimeTo(self):
+	def set_PageSize(self, PageSize):  # Long
+		self.add_query_param('PageSize', PageSize)
+	def get_PlanedStartTimeTo(self): # String
 		return self.get_query_params().get('PlanedStartTimeTo')
 
-	def set_PlanedStartTimeTo(self,PlanedStartTimeTo):
-		self.add_query_param('PlanedStartTimeTo',PlanedStartTimeTo)
-
-	def get_State(self):
+	def set_PlanedStartTimeTo(self, PlanedStartTimeTo):  # String
+		self.add_query_param('PlanedStartTimeTo', PlanedStartTimeTo)
+	def get_State(self): # String
 		return self.get_query_params().get('State')
 
-	def set_State(self,State):
-		self.add_query_param('State',State)
+	def set_State(self, State):  # String
+		self.add_query_param('State', State)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListCasesRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/RemoveSkillGroupsFromUserRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,47 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListCasesRequest(RpcRequest):
+class RemoveSkillGroupsFromUserRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListCases')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'RemoveSkillGroupsFromUser')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_UserId(self): # String
+		return self.get_query_params().get('UserId')
 
-	def get_InstanceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_CampaignId(self):
-		return self.get_query_params().get('CampaignId')
-
-	def set_CampaignId(self,CampaignId):
-		self.add_query_param('CampaignId',CampaignId)
-
-	def get_PhoneNumber(self):
-		return self.get_query_params().get('PhoneNumber')
-
-	def set_PhoneNumber(self,PhoneNumber):
-		self.add_query_param('PhoneNumber',PhoneNumber)
-
-	def get_PageSize(self):
-		return self.get_query_params().get('PageSize')
-
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
-
-	def get_PageNumber(self):
-		return self.get_query_params().get('PageNumber')
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_SkillGroupIdList(self): # String
+		return self.get_query_params().get('SkillGroupIdList')
 
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
+	def set_SkillGroupIdList(self, SkillGroupIdList):  # String
+		self.add_query_param('SkillGroupIdList', SkillGroupIdList)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListConfigItemsRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListConfigItemsRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,31 +20,29 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class ListConfigItemsRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListConfigItems')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_ObjectType(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_ObjectType(self): # String
 		return self.get_query_params().get('ObjectType')
 
-	def set_ObjectType(self,ObjectType):
-		self.add_query_param('ObjectType',ObjectType)
-
-	def get_ObjectId(self):
+	def set_ObjectType(self, ObjectType):  # String
+		self.add_query_param('ObjectType', ObjectType)
+	def get_ObjectId(self): # String
 		return self.get_query_params().get('ObjectId')
 
-	def set_ObjectId(self,ObjectId):
-		self.add_query_param('ObjectId',ObjectId)
+	def set_ObjectId(self, ObjectId):  # String
+		self.add_query_param('ObjectId', ObjectId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListContactFlowsRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListRealtimeSkillGroupStatesRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,41 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListContactFlowsRequest(RpcRequest):
+class ListRealtimeSkillGroupStatesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListContactFlows')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListRealtimeSkillGroupStates')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_Type(self):
-		return self.get_query_params().get('Type')
-
-	def set_Type(self,Type):
-		self.add_query_param('Type',Type)
-
-	def get_PageNumber(self):
+	def get_PageNumber(self): # Integer
 		return self.get_query_params().get('PageNumber')
 
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
-
-	def get_InstanceId(self):
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_SkillGroupIdList(self): # String
+		return self.get_body_params().get('SkillGroupIdList')
+
+	def set_SkillGroupIdList(self, SkillGroupIdList):  # String
+		self.add_body_params('SkillGroupIdList', SkillGroupIdList)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_PageSize(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
 
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListDevicesRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListDevicesRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,25 +20,24 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class ListDevicesRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListDevices')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_UserId(self):
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_InstanceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListHistoricalAgentReportRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListAgentStateLogsRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,53 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListHistoricalAgentReportRequest(RpcRequest):
+class ListAgentStateLogsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListHistoricalAgentReport')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListAgentStateLogs')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_AgentId(self): # String
+		return self.get_query_params().get('AgentId')
 
-	def get_StartTime(self):
+	def set_AgentId(self, AgentId):  # String
+		self.add_query_param('AgentId', AgentId)
+	def get_EndTime(self): # Long
+		return self.get_query_params().get('EndTime')
+
+	def set_EndTime(self, EndTime):  # Long
+		self.add_query_param('EndTime', EndTime)
+	def get_StartTime(self): # Long
 		return self.get_query_params().get('StartTime')
 
-	def set_StartTime(self,StartTime):
-		self.add_query_param('StartTime',StartTime)
-
-	def get_StopTime(self):
-		return self.get_query_params().get('StopTime')
-
-	def set_StopTime(self,StopTime):
-		self.add_query_param('StopTime',StopTime)
-
-	def get_PageNumber(self):
-		return self.get_query_params().get('PageNumber')
-
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
-
-	def get_InstanceId(self):
+	def set_StartTime(self, StartTime):  # Long
+		self.add_query_param('StartTime', StartTime)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_AgentIdList(self):
-		return self.get_body_params().get('AgentIdList')
-
-	def set_AgentIdList(self,AgentIdList):
-		self.add_body_params('AgentIdList', AgentIdList)
-
-	def get_PageSize(self):
-		return self.get_query_params().get('PageSize')
-
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListHistoricalSkillGroupReportRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/AssignUsersRequest.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,53 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListHistoricalSkillGroupReportRequest(RpcRequest):
+class AssignUsersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListHistoricalSkillGroupReport')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'AssignUsers')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_RamIdList(self): # String
+		return self.get_query_params().get('RamIdList')
 
-	def get_EndTime(self):
-		return self.get_query_params().get('EndTime')
-
-	def set_EndTime(self,EndTime):
-		self.add_query_param('EndTime',EndTime)
-
-	def get_StartTime(self):
-		return self.get_query_params().get('StartTime')
-
-	def set_StartTime(self,StartTime):
-		self.add_query_param('StartTime',StartTime)
-
-	def get_PageNumber(self):
-		return self.get_query_params().get('PageNumber')
-
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
-
-	def get_SkillGroupIdList(self):
-		return self.get_body_params().get('SkillGroupIdList')
-
-	def set_SkillGroupIdList(self,SkillGroupIdList):
-		self.add_body_params('SkillGroupIdList', SkillGroupIdList)
-
-	def get_InstanceId(self):
+	def set_RamIdList(self, RamIdList):  # String
+		self.add_query_param('RamIdList', RamIdList)
+	def get_RoleId(self): # String
+		return self.get_query_params().get('RoleId')
+
+	def set_RoleId(self, RoleId):  # String
+		self.add_query_param('RoleId', RoleId)
+	def get_WorkMode(self): # String
+		return self.get_query_params().get('WorkMode')
+
+	def set_WorkMode(self, WorkMode):  # String
+		self.add_query_param('WorkMode', WorkMode)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_PageSize(self):
-		return self.get_query_params().get('PageSize')
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_SkillLevelList(self): # String
+		return self.get_query_params().get('SkillLevelList')
 
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
+	def set_SkillLevelList(self, SkillLevelList):  # String
+		self.add_query_param('SkillLevelList', SkillLevelList)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListInstancesOfUserRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListInstancesRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,29 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListInstancesOfUserRequest(RpcRequest):
+class ListInstancesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListInstancesOfUser')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListInstances')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_PageNumber(self):
+	def get_PageNumber(self): # Integer
 		return self.get_query_params().get('PageNumber')
 
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
-
-	def get_PageSize(self):
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
 
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListInstancesRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListCallTagsRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,29 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListInstancesRequest(RpcRequest):
+class ListCallTagsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListInstances')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListCallTags')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_PageNumber(self):
+	def get_PageNumber(self): # Integer
 		return self.get_query_params().get('PageNumber')
 
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_InstanceId(self): # String
+		return self.get_query_params().get('InstanceId')
 
-	def get_PageSize(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
 
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListIntervalAgentReportRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetHistoricalInstanceReportRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,47 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListIntervalAgentReportRequest(RpcRequest):
+class GetHistoricalInstanceReportRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListIntervalAgentReport')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetHistoricalInstanceReport')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_AgentId(self):
-		return self.get_query_params().get('AgentId')
-
-	def set_AgentId(self,AgentId):
-		self.add_query_param('AgentId',AgentId)
-
-	def get_EndTime(self):
+	def get_EndTime(self): # Long
 		return self.get_query_params().get('EndTime')
 
-	def set_EndTime(self,EndTime):
-		self.add_query_param('EndTime',EndTime)
-
-	def get_StartTime(self):
+	def set_EndTime(self, EndTime):  # Long
+		self.add_query_param('EndTime', EndTime)
+	def get_StartTime(self): # Long
 		return self.get_query_params().get('StartTime')
 
-	def set_StartTime(self,StartTime):
-		self.add_query_param('StartTime',StartTime)
-
-	def get_InstanceId(self):
+	def set_StartTime(self, StartTime):  # Long
+		self.add_query_param('StartTime', StartTime)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_Interval(self):
-		return self.get_query_params().get('Interval')
-
-	def set_Interval(self,Interval):
-		self.add_query_param('Interval',Interval)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListIntervalInstanceReportRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListIntervalSkillGroupReportRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,41 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListIntervalInstanceReportRequest(RpcRequest):
+class ListIntervalSkillGroupReportRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListIntervalInstanceReport')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListIntervalSkillGroupReport')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_EndTime(self):
+	def get_EndTime(self): # Long
 		return self.get_query_params().get('EndTime')
 
-	def set_EndTime(self,EndTime):
-		self.add_query_param('EndTime',EndTime)
-
-	def get_StartTime(self):
+	def set_EndTime(self, EndTime):  # Long
+		self.add_query_param('EndTime', EndTime)
+	def get_StartTime(self): # Long
 		return self.get_query_params().get('StartTime')
 
-	def set_StartTime(self,StartTime):
-		self.add_query_param('StartTime',StartTime)
-
-	def get_InstanceId(self):
+	def set_StartTime(self, StartTime):  # Long
+		self.add_query_param('StartTime', StartTime)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_Interval(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_SkillGroupId(self): # String
+		return self.get_query_params().get('SkillGroupId')
+
+	def set_SkillGroupId(self, SkillGroupId):  # String
+		self.add_query_param('SkillGroupId', SkillGroupId)
+	def get_Interval(self): # String
 		return self.get_query_params().get('Interval')
 
-	def set_Interval(self,Interval):
-		self.add_query_param('Interval',Interval)
+	def set_Interval(self, Interval):  # String
+		self.add_query_param('Interval', Interval)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListIvrTrackingDetailsRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListCustomCallTaggingRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,41 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListIvrTrackingDetailsRequest(RpcRequest):
+class ListCustomCallTaggingRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListIvrTrackingDetails')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListCustomCallTagging')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ContactId(self):
-		return self.get_query_params().get('ContactId')
-
-	def set_ContactId(self,ContactId):
-		self.add_query_param('ContactId',ContactId)
-
-	def get_PageNumber(self):
+	def get_PageNumber(self): # Integer
 		return self.get_query_params().get('PageNumber')
 
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
-
-	def get_InstanceId(self):
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_SearchPattern(self): # String
+		return self.get_query_params().get('SearchPattern')
+
+	def set_SearchPattern(self, SearchPattern):  # String
+		self.add_query_param('SearchPattern', SearchPattern)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_PageSize(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
 
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
+	def get_CallTagNameList(self): # String
+		return self.get_query_params().get('CallTagNameList')
+
+	def set_CallTagNameList(self, CallTagNameList):  # String
+		self.add_query_param('CallTagNameList', CallTagNameList)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListOutboundNumbersOfUserRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/SignInGroupRequest.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,47 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListOutboundNumbersOfUserRequest(RpcRequest):
+class SignInGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListOutboundNumbersOfUser')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'SignInGroup')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_SignedSkillGroupIdList(self): # String
+		return self.get_query_params().get('SignedSkillGroupIdList')
 
-	def get_UserId(self):
+	def set_SignedSkillGroupIdList(self, SignedSkillGroupIdList):  # String
+		self.add_query_param('SignedSkillGroupIdList', SignedSkillGroupIdList)
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_PageNumber(self):
-		return self.get_query_params().get('PageNumber')
-
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
-
-	def get_InstanceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_DeviceId(self): # String
+		return self.get_query_params().get('DeviceId')
+
+	def set_DeviceId(self, DeviceId):  # String
+		self.add_query_param('DeviceId', DeviceId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_SkillGroupIdList(self):
-		return self.get_query_params().get('SkillGroupIdList')
-
-	def set_SkillGroupIdList(self,SkillGroupIdList):
-		self.add_query_param('SkillGroupIdList',SkillGroupIdList)
-
-	def get_PageSize(self):
-		return self.get_query_params().get('PageSize')
-
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListPersonalNumbersOfUserRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListPhoneNumbersRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,53 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListPersonalNumbersOfUserRequest(RpcRequest):
+class ListPhoneNumbersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListPersonalNumbersOfUser')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListPhoneNumbers')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Usage(self): # String
+		return self.get_query_params().get('Usage')
 
-	def get_UserId(self):
-		return self.get_query_params().get('UserId')
-
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_PageNumber(self):
+	def set_Usage(self, Usage):  # String
+		self.add_query_param('Usage', Usage)
+	def get_Active(self): # Boolean
+		return self.get_query_params().get('Active')
+
+	def set_Active(self, Active):  # Boolean
+		self.add_query_param('Active', Active)
+	def get_PageNumber(self): # Integer
 		return self.get_query_params().get('PageNumber')
 
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
-
-	def get_IsMember(self):
-		return self.get_query_params().get('IsMember')
-
-	def set_IsMember(self,IsMember):
-		self.add_query_param('IsMember',IsMember)
-
-	def get_SearchPattern(self):
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_SearchPattern(self): # String
 		return self.get_query_params().get('SearchPattern')
 
-	def set_SearchPattern(self,SearchPattern):
-		self.add_query_param('SearchPattern',SearchPattern)
-
-	def get_InstanceId(self):
+	def set_SearchPattern(self, SearchPattern):  # String
+		self.add_query_param('SearchPattern', SearchPattern)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_PageSize(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
 
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListPhoneNumbersOfSkillGroupRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/AddPhoneNumbersRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,59 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListPhoneNumbersOfSkillGroupRequest(RpcRequest):
+class AddPhoneNumbersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListPhoneNumbersOfSkillGroup')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'AddPhoneNumbers')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ContactFlowId(self): # String
+		return self.get_query_params().get('ContactFlowId')
 
-	def get_Active(self):
-		return self.get_query_params().get('Active')
-
-	def set_Active(self,Active):
-		self.add_query_param('Active',Active)
-
-	def get_PageNumber(self):
-		return self.get_query_params().get('PageNumber')
-
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
-
-	def get_IsMember(self):
-		return self.get_query_params().get('IsMember')
-
-	def set_IsMember(self,IsMember):
-		self.add_query_param('IsMember',IsMember)
-
-	def get_SearchPattern(self):
-		return self.get_query_params().get('SearchPattern')
-
-	def set_SearchPattern(self,SearchPattern):
-		self.add_query_param('SearchPattern',SearchPattern)
-
-	def get_InstanceId(self):
+	def set_ContactFlowId(self, ContactFlowId):  # String
+		self.add_query_param('ContactFlowId', ContactFlowId)
+	def get_Usage(self): # String
+		return self.get_query_params().get('Usage')
+
+	def set_Usage(self, Usage):  # String
+		self.add_query_param('Usage', Usage)
+	def get_NumberGroupId(self): # String
+		return self.get_query_params().get('NumberGroupId')
+
+	def set_NumberGroupId(self, NumberGroupId):  # String
+		self.add_query_param('NumberGroupId', NumberGroupId)
+	def get_NumberList(self): # String
+		return self.get_query_params().get('NumberList')
+
+	def set_NumberList(self, NumberList):  # String
+		self.add_query_param('NumberList', NumberList)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_SkillGroupId(self):
-		return self.get_query_params().get('SkillGroupId')
-
-	def set_SkillGroupId(self,SkillGroupId):
-		self.add_query_param('SkillGroupId',SkillGroupId)
-
-	def get_PageSize(self):
-		return self.get_query_params().get('PageSize')
-
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListPhoneNumbersRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListDoNotCallNumbersRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,53 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListPhoneNumbersRequest(RpcRequest):
+class ListDoNotCallNumbersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListPhoneNumbers')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListDoNotCallNumbers')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_Usage(self):
-		return self.get_query_params().get('Usage')
-
-	def set_Usage(self,Usage):
-		self.add_query_param('Usage',Usage)
-
-	def get_Active(self):
-		return self.get_query_params().get('Active')
-
-	def set_Active(self,Active):
-		self.add_query_param('Active',Active)
-
-	def get_PageNumber(self):
+	def get_PageNumber(self): # Integer
 		return self.get_query_params().get('PageNumber')
 
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
-
-	def get_SearchPattern(self):
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_SearchPattern(self): # String
 		return self.get_query_params().get('SearchPattern')
 
-	def set_SearchPattern(self,SearchPattern):
-		self.add_query_param('SearchPattern',SearchPattern)
-
-	def get_InstanceId(self):
+	def set_SearchPattern(self, SearchPattern):  # String
+		self.add_query_param('SearchPattern', SearchPattern)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_PageSize(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_Scope(self): # String
+		return self.get_query_params().get('Scope')
+
+	def set_Scope(self, Scope):  # String
+		self.add_query_param('Scope', Scope)
+	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
 
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListPrivilegesOfUserRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetMonoRecordingRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,23 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListPrivilegesOfUserRequest(RpcRequest):
+class GetMonoRecordingRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListPrivilegesOfUser')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetMonoRecording')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ContactId(self): # String
+		return self.get_query_params().get('ContactId')
 
-	def get_InstanceId(self):
+	def set_ContactId(self, ContactId):  # String
+		self.add_query_param('ContactId', ContactId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListRamUsersRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListRamUsersRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,37 +20,34 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class ListRamUsersRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListRamUsers')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_PageNumber(self):
+	def get_PageNumber(self): # Integer
 		return self.get_query_params().get('PageNumber')
 
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
-
-	def get_SearchPattern(self):
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_SearchPattern(self): # String
 		return self.get_query_params().get('SearchPattern')
 
-	def set_SearchPattern(self,SearchPattern):
-		self.add_query_param('SearchPattern',SearchPattern)
-
-	def get_InstanceId(self):
+	def set_SearchPattern(self, SearchPattern):  # String
+		self.add_query_param('SearchPattern', SearchPattern)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_PageSize(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
 
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListRealtimeAgentStatesRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListRealtimeAgentStatesRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,55 +20,49 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class ListRealtimeAgentStatesRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListRealtimeAgentStates')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_PageNumber(self):
+	def get_PageNumber(self): # Integer
 		return self.get_query_params().get('PageNumber')
 
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
-
-	def get_InstanceId(self):
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_AgentIdList(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_AgentIdList(self): # String
 		return self.get_body_params().get('AgentIdList')
 
-	def set_AgentIdList(self,AgentIdList):
+	def set_AgentIdList(self, AgentIdList):  # String
 		self.add_body_params('AgentIdList', AgentIdList)
-
-	def get_SkillGroupId(self):
+	def get_SkillGroupId(self): # String
 		return self.get_query_params().get('SkillGroupId')
 
-	def set_SkillGroupId(self,SkillGroupId):
-		self.add_query_param('SkillGroupId',SkillGroupId)
-
-	def get_AgentName(self):
+	def set_SkillGroupId(self, SkillGroupId):  # String
+		self.add_query_param('SkillGroupId', SkillGroupId)
+	def get_AgentName(self): # String
 		return self.get_query_params().get('AgentName')
 
-	def set_AgentName(self,AgentName):
-		self.add_query_param('AgentName',AgentName)
-
-	def get_PageSize(self):
+	def set_AgentName(self, AgentName):  # String
+		self.add_query_param('AgentName', AgentName)
+	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
 
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
-
-	def get_StateList(self):
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
+	def get_StateList(self): # String
 		return self.get_body_params().get('StateList')
 
-	def set_StateList(self,StateList):
-		self.add_body_params('StateList', StateList)
+	def set_StateList(self, StateList):  # String
+		self.add_body_params('StateList', StateList)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListRealtimeSkillGroupStatesRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ModifyUserLevelsOfSkillGroupRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,41 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListRealtimeSkillGroupStatesRequest(RpcRequest):
+class ModifyUserLevelsOfSkillGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListRealtimeSkillGroupStates')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ModifyUserLevelsOfSkillGroup')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_UserLevelList(self): # String
+		return self.get_query_params().get('UserLevelList')
 
-	def get_PageNumber(self):
-		return self.get_query_params().get('PageNumber')
-
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
-
-	def get_SkillGroupIdList(self):
-		return self.get_body_params().get('SkillGroupIdList')
-
-	def set_SkillGroupIdList(self,SkillGroupIdList):
-		self.add_body_params('SkillGroupIdList', SkillGroupIdList)
-
-	def get_InstanceId(self):
+	def set_UserLevelList(self, UserLevelList):  # String
+		self.add_query_param('UserLevelList', UserLevelList)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_PageSize(self):
-		return self.get_query_params().get('PageSize')
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_SkillGroupId(self): # String
+		return self.get_query_params().get('SkillGroupId')
 
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
+	def set_SkillGroupId(self, SkillGroupId):  # String
+		self.add_query_param('SkillGroupId', SkillGroupId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListRecentCallDetailRecordsRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListHistoricalSkillGroupReportRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,53 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListRecentCallDetailRecordsRequest(RpcRequest):
+class ListHistoricalSkillGroupReportRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListRecentCallDetailRecords')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListHistoricalSkillGroupReport')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_Criteria(self):
-		return self.get_query_params().get('Criteria')
-
-	def set_Criteria(self,Criteria):
-		self.add_query_param('Criteria',Criteria)
-
-	def get_EndTime(self):
+	def get_EndTime(self): # Long
 		return self.get_query_params().get('EndTime')
 
-	def set_EndTime(self,EndTime):
-		self.add_query_param('EndTime',EndTime)
-
-	def get_StartTime(self):
-		return self.get_body_params().get('StartTime')
-
-	def set_StartTime(self,StartTime):
-		self.add_body_params('StartTime', StartTime)
-
-	def get_PageNumber(self):
+	def set_EndTime(self, EndTime):  # Long
+		self.add_query_param('EndTime', EndTime)
+	def get_StartTime(self): # Long
+		return self.get_query_params().get('StartTime')
+
+	def set_StartTime(self, StartTime):  # Long
+		self.add_query_param('StartTime', StartTime)
+	def get_PageNumber(self): # Integer
 		return self.get_query_params().get('PageNumber')
 
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
-
-	def get_InstanceId(self):
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_SkillGroupIdList(self): # String
+		return self.get_body_params().get('SkillGroupIdList')
+
+	def set_SkillGroupIdList(self, SkillGroupIdList):  # String
+		self.add_body_params('SkillGroupIdList', SkillGroupIdList)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_PageSize(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
 
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListRolesRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ExportCustomCallTaggingRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListRolesRequest(RpcRequest):
+class ExportCustomCallTaggingRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListRoles')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ExportCustomCallTagging')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListSipCallRecordsRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetUserRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,29 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListSipCallRecordsRequest(RpcRequest):
+class GetUserRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListSipCallRecords')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetUser')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Extension(self): # String
+		return self.get_query_params().get('Extension')
 
-	def get_ContactIdList(self):
-		return self.get_query_params().get('ContactIdList')
-
-	def set_ContactIdList(self,ContactIdList):
-		self.add_query_param('ContactIdList',ContactIdList)
+	def set_Extension(self, Extension):  # String
+		self.add_query_param('Extension', Extension)
+	def get_UserId(self): # String
+		return self.get_query_params().get('UserId')
 
-	def get_InstanceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListSipTracesRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListSipTracesRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,25 +20,24 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class ListSipTracesRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListSipTraces')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_CallId(self):
+	def get_CallId(self): # String
 		return self.get_query_params().get('CallId')
 
-	def set_CallId(self,CallId):
-		self.add_query_param('CallId',CallId)
-
-	def get_InstanceId(self):
+	def set_CallId(self, CallId):  # String
+		self.add_query_param('CallId', CallId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListSkillGroupsRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListUnassignedNumbersRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,41 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListSkillGroupsRequest(RpcRequest):
+class ListUnassignedNumbersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListSkillGroups')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListUnassignedNumbers')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_PageNumber(self):
+	def get_PageNumber(self): # Integer
 		return self.get_query_params().get('PageNumber')
 
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
-
-	def get_SearchPattern(self):
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_SearchPattern(self): # String
 		return self.get_query_params().get('SearchPattern')
 
-	def set_SearchPattern(self,SearchPattern):
-		self.add_query_param('SearchPattern',SearchPattern)
-
-	def get_InstanceId(self):
+	def set_SearchPattern(self, SearchPattern):  # String
+		self.add_query_param('SearchPattern', SearchPattern)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_PageSize(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
 
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListSkillLevelsOfUserRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListSkillLevelsOfUserRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,49 +20,44 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class ListSkillLevelsOfUserRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListSkillLevelsOfUser')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_UserId(self):
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_IsMember(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_IsMember(self): # Boolean
 		return self.get_query_params().get('IsMember')
 
-	def set_IsMember(self,IsMember):
-		self.add_query_param('IsMember',IsMember)
-
-	def get_PageNumber(self):
+	def set_IsMember(self, IsMember):  # Boolean
+		self.add_query_param('IsMember', IsMember)
+	def get_PageNumber(self): # Integer
 		return self.get_query_params().get('PageNumber')
 
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
-
-	def get_SearchPattern(self):
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_SearchPattern(self): # String
 		return self.get_query_params().get('SearchPattern')
 
-	def set_SearchPattern(self,SearchPattern):
-		self.add_query_param('SearchPattern',SearchPattern)
-
-	def get_InstanceId(self):
+	def set_SearchPattern(self, SearchPattern):  # String
+		self.add_query_param('SearchPattern', SearchPattern)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_PageSize(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
 
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListUnassignedNumbersRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetDoNotCallFileUploadParametersRequest.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,41 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListUnassignedNumbersRequest(RpcRequest):
+class GetDoNotCallFileUploadParametersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListUnassignedNumbers')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetDoNotCallFileUploadParameters')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_PageNumber(self):
-		return self.get_query_params().get('PageNumber')
-
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
-
-	def get_SearchPattern(self):
-		return self.get_query_params().get('SearchPattern')
-
-	def set_SearchPattern(self,SearchPattern):
-		self.add_query_param('SearchPattern',SearchPattern)
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_PageSize(self):
-		return self.get_query_params().get('PageSize')
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_FileName(self): # String
+		return self.get_query_params().get('FileName')
 
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
+	def set_FileName(self, FileName):  # String
+		self.add_query_param('FileName', FileName)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListUserLevelsOfSkillGroupRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListUserLevelsOfSkillGroupRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,49 +20,44 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class ListUserLevelsOfSkillGroupRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListUserLevelsOfSkillGroup')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_IsMember(self):
+	def get_IsMember(self): # Boolean
 		return self.get_query_params().get('IsMember')
 
-	def set_IsMember(self,IsMember):
-		self.add_query_param('IsMember',IsMember)
-
-	def get_PageNumber(self):
+	def set_IsMember(self, IsMember):  # Boolean
+		self.add_query_param('IsMember', IsMember)
+	def get_PageNumber(self): # Integer
 		return self.get_query_params().get('PageNumber')
 
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
-
-	def get_SearchPattern(self):
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_SearchPattern(self): # String
 		return self.get_query_params().get('SearchPattern')
 
-	def set_SearchPattern(self,SearchPattern):
-		self.add_query_param('SearchPattern',SearchPattern)
-
-	def get_InstanceId(self):
+	def set_SearchPattern(self, SearchPattern):  # String
+		self.add_query_param('SearchPattern', SearchPattern)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_SkillGroupId(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_SkillGroupId(self): # String
 		return self.get_query_params().get('SkillGroupId')
 
-	def set_SkillGroupId(self,SkillGroupId):
-		self.add_query_param('SkillGroupId',SkillGroupId)
-
-	def get_PageSize(self):
+	def set_SkillGroupId(self, SkillGroupId):  # String
+		self.add_query_param('SkillGroupId', SkillGroupId)
+	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
 
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ListUsersRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListIvrTrackingDetailsRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,41 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ListUsersRequest(RpcRequest):
+class ListIvrTrackingDetailsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListUsers')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListIvrTrackingDetails')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ContactId(self): # String
+		return self.get_query_params().get('ContactId')
 
-	def get_PageNumber(self):
+	def set_ContactId(self, ContactId):  # String
+		self.add_query_param('ContactId', ContactId)
+	def get_PageNumber(self): # Integer
 		return self.get_query_params().get('PageNumber')
 
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
-
-	def get_SearchPattern(self):
-		return self.get_query_params().get('SearchPattern')
-
-	def set_SearchPattern(self,SearchPattern):
-		self.add_query_param('SearchPattern',SearchPattern)
-
-	def get_InstanceId(self):
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_PageSize(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
 
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/MakeCallRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/MakeCallRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,61 +20,54 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class MakeCallRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'MakeCall')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_Callee(self):
+	def get_Callee(self): # String
 		return self.get_query_params().get('Callee')
 
-	def set_Callee(self,Callee):
-		self.add_query_param('Callee',Callee)
-
-	def get_MaskedCallee(self):
+	def set_Callee(self, Callee):  # String
+		self.add_query_param('Callee', Callee)
+	def get_MaskedCallee(self): # String
 		return self.get_query_params().get('MaskedCallee')
 
-	def set_MaskedCallee(self,MaskedCallee):
-		self.add_query_param('MaskedCallee',MaskedCallee)
-
-	def get_UserId(self):
+	def set_MaskedCallee(self, MaskedCallee):  # String
+		self.add_query_param('MaskedCallee', MaskedCallee)
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_DeviceId(self): # String
 		return self.get_query_params().get('DeviceId')
 
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_Tags(self):
+	def set_DeviceId(self, DeviceId):  # String
+		self.add_query_param('DeviceId', DeviceId)
+	def get_Tags(self): # String
 		return self.get_query_params().get('Tags')
 
-	def set_Tags(self,Tags):
-		self.add_query_param('Tags',Tags)
-
-	def get_TimeoutSeconds(self):
+	def set_Tags(self, Tags):  # String
+		self.add_query_param('Tags', Tags)
+	def get_TimeoutSeconds(self): # Integer
 		return self.get_query_params().get('TimeoutSeconds')
 
-	def set_TimeoutSeconds(self,TimeoutSeconds):
-		self.add_query_param('TimeoutSeconds',TimeoutSeconds)
-
-	def get_Caller(self):
+	def set_TimeoutSeconds(self, TimeoutSeconds):  # Integer
+		self.add_query_param('TimeoutSeconds', TimeoutSeconds)
+	def get_Caller(self): # String
 		return self.get_query_params().get('Caller')
 
-	def set_Caller(self,Caller):
-		self.add_query_param('Caller',Caller)
-
-	def get_InstanceId(self):
+	def set_Caller(self, Caller):  # String
+		self.add_query_param('Caller', Caller)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ModifyInstanceRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ModifySkillGroupRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,29 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ModifyInstanceRequest(RpcRequest):
+class ModifySkillGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ModifyInstance')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ModifySkillGroup')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_Description(self):
+	def get_Description(self): # String
 		return self.get_query_params().get('Description')
 
-	def set_Description(self,Description):
-		self.add_query_param('Description',Description)
-
-	def get_InstanceId(self):
+	def set_Description(self, Description):  # String
+		self.add_query_param('Description', Description)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_SkillGroupId(self): # String
+		return self.get_query_params().get('SkillGroupId')
+
+	def set_SkillGroupId(self, SkillGroupId):  # String
+		self.add_query_param('SkillGroupId', SkillGroupId)
+	def get_DisplayName(self): # String
+		return self.get_query_params().get('DisplayName')
+
+	def set_DisplayName(self, DisplayName):  # String
+		self.add_query_param('DisplayName', DisplayName)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ModifyPhoneNumberRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/AddSkillGroupsToUserRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,41 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ModifyPhoneNumberRequest(RpcRequest):
+class AddSkillGroupsToUserRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ModifyPhoneNumber')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'AddSkillGroupsToUser')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_UserId(self): # String
+		return self.get_query_params().get('UserId')
 
-	def get_ContactFlowId(self):
-		return self.get_query_params().get('ContactFlowId')
-
-	def set_ContactFlowId(self,ContactFlowId):
-		self.add_query_param('ContactFlowId',ContactFlowId)
-
-	def get_Usage(self):
-		return self.get_query_params().get('Usage')
-
-	def set_Usage(self,Usage):
-		self.add_query_param('Usage',Usage)
-
-	def get_Number(self):
-		return self.get_query_params().get('Number')
-
-	def set_Number(self,Number):
-		self.add_query_param('Number',Number)
-
-	def get_InstanceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_SkillLevelList(self): # String
+		return self.get_query_params().get('SkillLevelList')
+
+	def set_SkillLevelList(self, SkillLevelList):  # String
+		self.add_query_param('SkillLevelList', SkillLevelList)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ModifySkillGroupRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListRolesRequest.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,41 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ModifySkillGroupRequest(RpcRequest):
+class ListRolesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ModifySkillGroup')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListRoles')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_Description(self):
-		return self.get_query_params().get('Description')
-
-	def set_Description(self,Description):
-		self.add_query_param('Description',Description)
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_SkillGroupId(self):
-		return self.get_query_params().get('SkillGroupId')
-
-	def set_SkillGroupId(self,SkillGroupId):
-		self.add_query_param('SkillGroupId',SkillGroupId)
-
-	def get_DisplayName(self):
-		return self.get_query_params().get('DisplayName')
-
-	def set_DisplayName(self,DisplayName):
-		self.add_query_param('DisplayName',DisplayName)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ModifySkillLevelsOfUserRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/RemoveUsersFromSkillGroupRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,35 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ModifySkillLevelsOfUserRequest(RpcRequest):
+class RemoveUsersFromSkillGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ModifySkillLevelsOfUser')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'RemoveUsersFromSkillGroup')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_UserIdList(self): # String
+		return self.get_query_params().get('UserIdList')
 
-	def get_UserId(self):
-		return self.get_query_params().get('UserId')
-
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_InstanceId(self):
+	def set_UserIdList(self, UserIdList):  # String
+		self.add_query_param('UserIdList', UserIdList)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_SkillLevelList(self):
-		return self.get_query_params().get('SkillLevelList')
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_SkillGroupId(self): # String
+		return self.get_query_params().get('SkillGroupId')
 
-	def set_SkillLevelList(self,SkillLevelList):
-		self.add_query_param('SkillLevelList',SkillLevelList)
+	def set_SkillGroupId(self, SkillGroupId):  # String
+		self.add_query_param('SkillGroupId', SkillGroupId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ModifyUserLevelsOfSkillGroupRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/SaveWebRtcInfoRequest.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,35 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ModifyUserLevelsOfSkillGroupRequest(RpcRequest):
+class SaveWebRtcInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ModifyUserLevelsOfSkillGroup')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'SaveWebRtcInfo')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_CallId(self): # String
+		return self.get_query_params().get('CallId')
 
-	def get_UserLevelList(self):
-		return self.get_query_params().get('UserLevelList')
-
-	def set_UserLevelList(self,UserLevelList):
-		self.add_query_param('UserLevelList',UserLevelList)
-
-	def get_InstanceId(self):
+	def set_CallId(self, CallId):  # String
+		self.add_query_param('CallId', CallId)
+	def get_Content(self): # String
+		return self.get_query_params().get('Content')
+
+	def set_Content(self, Content):  # String
+		self.add_query_param('Content', Content)
+	def get_ContentType(self): # String
+		return self.get_query_params().get('ContentType')
+
+	def set_ContentType(self, ContentType):  # String
+		self.add_query_param('ContentType', ContentType)
+	def get_JobId(self): # String
+		return self.get_query_params().get('JobId')
+
+	def set_JobId(self, JobId):  # String
+		self.add_query_param('JobId', JobId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_SkillGroupId(self):
-		return self.get_query_params().get('SkillGroupId')
-
-	def set_SkillGroupId(self,SkillGroupId):
-		self.add_query_param('SkillGroupId',SkillGroupId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ModifyUserRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ModifyUserRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,43 +20,44 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class ModifyUserRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ModifyUser')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_RoleId(self):
+	def get_RoleId(self): # String
 		return self.get_query_params().get('RoleId')
 
-	def set_RoleId(self,RoleId):
-		self.add_query_param('RoleId',RoleId)
-
-	def get_Mobile(self):
+	def set_RoleId(self, RoleId):  # String
+		self.add_query_param('RoleId', RoleId)
+	def get_Mobile(self): # String
 		return self.get_query_params().get('Mobile')
 
-	def set_Mobile(self,Mobile):
-		self.add_query_param('Mobile',Mobile)
-
-	def get_WorkMode(self):
+	def set_Mobile(self, Mobile):  # String
+		self.add_query_param('Mobile', Mobile)
+	def get_WorkMode(self): # String
 		return self.get_query_params().get('WorkMode')
 
-	def set_WorkMode(self,WorkMode):
-		self.add_query_param('WorkMode',WorkMode)
-
-	def get_UserId(self):
+	def set_WorkMode(self, WorkMode):  # String
+		self.add_query_param('WorkMode', WorkMode)
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_InstanceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_DisplayId(self): # String
+		return self.get_query_params().get('DisplayId')
+
+	def set_DisplayId(self, DisplayId):  # String
+		self.add_query_param('DisplayId', DisplayId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/MonitorCallRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/RetrieveCallRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,47 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class MonitorCallRequest(RpcRequest):
+class RetrieveCallRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'MonitorCall')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'RetrieveCall')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_UserId(self):
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_DeviceId(self): # String
 		return self.get_query_params().get('DeviceId')
 
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_TimeoutSeconds(self):
-		return self.get_query_params().get('TimeoutSeconds')
-
-	def set_TimeoutSeconds(self,TimeoutSeconds):
-		self.add_query_param('TimeoutSeconds',TimeoutSeconds)
-
-	def get_InstanceId(self):
+	def set_DeviceId(self, DeviceId):  # String
+		self.add_query_param('DeviceId', DeviceId)
+	def get_JobId(self): # String
+		return self.get_query_params().get('JobId')
+
+	def set_JobId(self, JobId):  # String
+		self.add_query_param('JobId', JobId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_MonitoredUserId(self):
-		return self.get_query_params().get('MonitoredUserId')
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_ChannelId(self): # String
+		return self.get_query_params().get('ChannelId')
 
-	def set_MonitoredUserId(self,MonitoredUserId):
-		self.add_query_param('MonitoredUserId',MonitoredUserId)
+	def set_ChannelId(self, ChannelId):  # String
+		self.add_query_param('ChannelId', ChannelId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/MuteCallRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/UnmuteCallRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,47 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class MuteCallRequest(RpcRequest):
+class UnmuteCallRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'MuteCall')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'UnmuteCall')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_UserId(self):
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_DeviceId(self): # String
 		return self.get_query_params().get('DeviceId')
 
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_JobId(self):
+	def set_DeviceId(self, DeviceId):  # String
+		self.add_query_param('DeviceId', DeviceId)
+	def get_JobId(self): # String
 		return self.get_query_params().get('JobId')
 
-	def set_JobId(self,JobId):
-		self.add_query_param('JobId',JobId)
-
-	def get_InstanceId(self):
+	def set_JobId(self, JobId):  # String
+		self.add_query_param('JobId', JobId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_ChannelId(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_ChannelId(self): # String
 		return self.get_query_params().get('ChannelId')
 
-	def set_ChannelId(self,ChannelId):
-		self.add_query_param('ChannelId',ChannelId)
+	def set_ChannelId(self, ChannelId):  # String
+		self.add_query_param('ChannelId', ChannelId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/PauseCampaignRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/AbortCampaignRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,29 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class PauseCampaignRequest(RpcRequest):
+class AbortCampaignRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'PauseCampaign')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'AbortCampaign')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_CampaignId(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_CampaignId(self): # String
 		return self.get_query_params().get('CampaignId')
 
-	def set_CampaignId(self,CampaignId):
-		self.add_query_param('CampaignId',CampaignId)
+	def set_CampaignId(self, CampaignId):  # String
+		self.add_query_param('CampaignId', CampaignId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/PickOutboundNumbersRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/PickOutboundNumbersRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,37 +20,34 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class PickOutboundNumbersRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'PickOutboundNumbers')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_Count(self):
+	def get_Count(self): # Integer
 		return self.get_query_params().get('Count')
 
-	def set_Count(self,Count):
-		self.add_query_param('Count',Count)
-
-	def get_InstanceId(self):
+	def set_Count(self, Count):  # Integer
+		self.add_query_param('Count', Count)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_SkillGroupIdList(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_SkillGroupIdList(self): # String
 		return self.get_query_params().get('SkillGroupIdList')
 
-	def set_SkillGroupIdList(self,SkillGroupIdList):
-		self.add_query_param('SkillGroupIdList',SkillGroupIdList)
-
-	def get_CalledNumber(self):
+	def set_SkillGroupIdList(self, SkillGroupIdList):  # String
+		self.add_query_param('SkillGroupIdList', SkillGroupIdList)
+	def get_CalledNumber(self): # String
 		return self.get_query_params().get('CalledNumber')
 
-	def set_CalledNumber(self,CalledNumber):
-		self.add_query_param('CalledNumber',CalledNumber)
+	def set_CalledNumber(self, CalledNumber):  # String
+		self.add_query_param('CalledNumber', CalledNumber)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/PollUserStatusRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListMonoRecordingsRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,35 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class PollUserStatusRequest(RpcRequest):
+class ListMonoRecordingsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'PollUserStatus')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListMonoRecordings')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ContactId(self): # String
+		return self.get_query_params().get('ContactId')
 
-	def get_UserId(self):
-		return self.get_query_params().get('UserId')
-
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
-		return self.get_query_params().get('DeviceId')
-
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_InstanceId(self):
+	def set_ContactId(self, ContactId):  # String
+		self.add_query_param('ContactId', ContactId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ReadyForServiceRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/PollUserStatusRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,41 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ReadyForServiceRequest(RpcRequest):
+class PollUserStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ReadyForService')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'PollUserStatus')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_OutboundScenario(self):
-		return self.get_query_params().get('OutboundScenario')
-
-	def set_OutboundScenario(self,OutboundScenario):
-		self.add_query_param('OutboundScenario',OutboundScenario)
-
-	def get_UserId(self):
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_DeviceId(self): # String
 		return self.get_query_params().get('DeviceId')
 
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_InstanceId(self):
+	def set_DeviceId(self, DeviceId):  # String
+		self.add_query_param('DeviceId', DeviceId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/RegisterDeviceRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/UpdateConfigItemsRequest.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,41 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class RegisterDeviceRequest(RpcRequest):
+class UpdateConfigItemsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'RegisterDevice')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'UpdateConfigItems')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ConfigItems(self): # String
+		return self.get_query_params().get('ConfigItems')
 
-	def get_UserId(self):
-		return self.get_query_params().get('UserId')
-
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
-		return self.get_query_params().get('DeviceId')
-
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_Password(self):
-		return self.get_query_params().get('Password')
-
-	def set_Password(self,Password):
-		self.add_query_param('Password',Password)
-
-	def get_InstanceId(self):
+	def set_ConfigItems(self, ConfigItems):  # String
+		self.add_query_param('ConfigItems', ConfigItems)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_ObjectType(self): # String
+		return self.get_query_params().get('ObjectType')
+
+	def set_ObjectType(self, ObjectType):  # String
+		self.add_query_param('ObjectType', ObjectType)
+	def get_ObjectId(self): # String
+		return self.get_query_params().get('ObjectId')
+
+	def set_ObjectId(self, ObjectId):  # String
+		self.add_query_param('ObjectId', ObjectId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/RegisterDevicesRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/RemovePhoneNumbersFromSkillGroupRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,41 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class RegisterDevicesRequest(RpcRequest):
+class RemovePhoneNumbersFromSkillGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'RegisterDevices')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'RemovePhoneNumbersFromSkillGroup')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_NumberList(self): # String
+		return self.get_query_params().get('NumberList')
 
-	def get_UserIdListJson(self):
-		return self.get_query_params().get('UserIdListJson')
-
-	def set_UserIdListJson(self,UserIdListJson):
-		self.add_query_param('UserIdListJson',UserIdListJson)
-
-	def get_DeviceId(self):
-		return self.get_query_params().get('DeviceId')
-
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_Password(self):
-		return self.get_query_params().get('Password')
-
-	def set_Password(self,Password):
-		self.add_query_param('Password',Password)
-
-	def get_InstanceId(self):
+	def set_NumberList(self, NumberList):  # String
+		self.add_query_param('NumberList', NumberList)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_SkillGroupId(self): # String
+		return self.get_query_params().get('SkillGroupId')
+
+	def set_SkillGroupId(self, SkillGroupId):  # String
+		self.add_query_param('SkillGroupId', SkillGroupId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ReleaseCallRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/CompleteAttendedTransferRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,47 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ReleaseCallRequest(RpcRequest):
+class CompleteAttendedTransferRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ReleaseCall')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'CompleteAttendedTransfer')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_UserId(self):
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_DeviceId(self): # String
 		return self.get_query_params().get('DeviceId')
 
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_JobId(self):
+	def set_DeviceId(self, DeviceId):  # String
+		self.add_query_param('DeviceId', DeviceId)
+	def get_JobId(self): # String
 		return self.get_query_params().get('JobId')
 
-	def set_JobId(self,JobId):
-		self.add_query_param('JobId',JobId)
-
-	def get_InstanceId(self):
+	def set_JobId(self, JobId):  # String
+		self.add_query_param('JobId', JobId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_ChannelId(self):
-		return self.get_query_params().get('ChannelId')
-
-	def set_ChannelId(self,ChannelId):
-		self.add_query_param('ChannelId',ChannelId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/RemovePersonalNumbersFromUserRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ReleaseCallRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,35 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class RemovePersonalNumbersFromUserRequest(RpcRequest):
+class ReleaseCallRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'RemovePersonalNumbersFromUser')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ReleaseCall')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_UserId(self):
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_NumberList(self):
-		return self.get_query_params().get('NumberList')
-
-	def set_NumberList(self,NumberList):
-		self.add_query_param('NumberList',NumberList)
-
-	def get_InstanceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_DeviceId(self): # String
+		return self.get_query_params().get('DeviceId')
+
+	def set_DeviceId(self, DeviceId):  # String
+		self.add_query_param('DeviceId', DeviceId)
+	def get_JobId(self): # String
+		return self.get_query_params().get('JobId')
+
+	def set_JobId(self, JobId):  # String
+		self.add_query_param('JobId', JobId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_ChannelId(self): # String
+		return self.get_query_params().get('ChannelId')
+
+	def set_ChannelId(self, ChannelId):  # String
+		self.add_query_param('ChannelId', ChannelId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/RemovePhoneNumberFromSkillGroupsRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListSkillGroupSummaryReportsSinceMidnightRequest.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,35 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class RemovePhoneNumberFromSkillGroupsRequest(RpcRequest):
+class ListSkillGroupSummaryReportsSinceMidnightRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'RemovePhoneNumberFromSkillGroups')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListSkillGroupSummaryReportsSinceMidnight')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_PageNumber(self): # Integer
+		return self.get_query_params().get('PageNumber')
 
-	def get_Number(self):
-		return self.get_query_params().get('Number')
-
-	def set_Number(self,Number):
-		self.add_query_param('Number',Number)
-
-	def get_InstanceId(self):
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_SkillGroupIdList(self):
-		return self.get_query_params().get('SkillGroupIdList')
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_SkillGroups(self): # String
+		return self.get_query_params().get('SkillGroups')
+
+	def set_SkillGroups(self, SkillGroups):  # String
+		self.add_query_param('SkillGroups', SkillGroups)
+	def get_PageSize(self): # Integer
+		return self.get_query_params().get('PageSize')
 
-	def set_SkillGroupIdList(self,SkillGroupIdList):
-		self.add_query_param('SkillGroupIdList',SkillGroupIdList)
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/RemovePhoneNumbersFromSkillGroupRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/AddNumbersToSkillGroupRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,35 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class RemovePhoneNumbersFromSkillGroupRequest(RpcRequest):
+class AddNumbersToSkillGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'RemovePhoneNumbersFromSkillGroup')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'AddNumbersToSkillGroup')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_NumberList(self):
+	def get_NumberList(self): # String
 		return self.get_query_params().get('NumberList')
 
-	def set_NumberList(self,NumberList):
-		self.add_query_param('NumberList',NumberList)
-
-	def get_InstanceId(self):
+	def set_NumberList(self, NumberList):  # String
+		self.add_query_param('NumberList', NumberList)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_SkillGroupId(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_SkillGroupId(self): # String
 		return self.get_query_params().get('SkillGroupId')
 
-	def set_SkillGroupId(self,SkillGroupId):
-		self.add_query_param('SkillGroupId',SkillGroupId)
+	def set_SkillGroupId(self, SkillGroupId):  # String
+		self.add_query_param('SkillGroupId', SkillGroupId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/RemovePhoneNumbersRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/RemovePhoneNumbersRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,25 +20,29 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class RemovePhoneNumbersRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'RemovePhoneNumbers')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_NumberList(self):
+	def get_NumberList(self): # String
 		return self.get_query_params().get('NumberList')
 
-	def set_NumberList(self,NumberList):
-		self.add_query_param('NumberList',NumberList)
-
-	def get_InstanceId(self):
+	def set_NumberList(self, NumberList):  # String
+		self.add_query_param('NumberList', NumberList)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_Force(self): # Boolean
+		return self.get_query_params().get('Force')
+
+	def set_Force(self, Force):  # Boolean
+		self.add_query_param('Force', Force)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/RemoveSkillGroupsFromUserRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListSkillGroupStatesRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,35 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class RemoveSkillGroupsFromUserRequest(RpcRequest):
+class ListSkillGroupStatesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'RemoveSkillGroupsFromUser')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListSkillGroupStates')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_PageNumber(self): # Integer
+		return self.get_query_params().get('PageNumber')
 
-	def get_UserId(self):
-		return self.get_query_params().get('UserId')
-
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_InstanceId(self):
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_SkillGroupIdList(self):
-		return self.get_query_params().get('SkillGroupIdList')
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_SkillGroupIds(self): # String
+		return self.get_query_params().get('SkillGroupIds')
+
+	def set_SkillGroupIds(self, SkillGroupIds):  # String
+		self.add_query_param('SkillGroupIds', SkillGroupIds)
+	def get_PageSize(self): # Integer
+		return self.get_query_params().get('PageSize')
 
-	def set_SkillGroupIdList(self,SkillGroupIdList):
-		self.add_query_param('SkillGroupIdList',SkillGroupIdList)
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/RemoveUsersFromSkillGroupRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/CreateSkillGroupRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,35 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class RemoveUsersFromSkillGroupRequest(RpcRequest):
+class CreateSkillGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'RemoveUsersFromSkillGroup')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'CreateSkillGroup')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Description(self): # String
+		return self.get_query_params().get('Description')
 
-	def get_UserIdList(self):
-		return self.get_query_params().get('UserIdList')
-
-	def set_UserIdList(self,UserIdList):
-		self.add_query_param('UserIdList',UserIdList)
-
-	def get_InstanceId(self):
+	def set_Description(self, Description):  # String
+		self.add_query_param('Description', Description)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_SkillGroupId(self):
-		return self.get_query_params().get('SkillGroupId')
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_DisplayName(self): # String
+		return self.get_query_params().get('DisplayName')
+
+	def set_DisplayName(self, DisplayName):  # String
+		self.add_query_param('DisplayName', DisplayName)
+	def get_Name(self): # String
+		return self.get_query_params().get('Name')
 
-	def set_SkillGroupId(self,SkillGroupId):
-		self.add_query_param('SkillGroupId',SkillGroupId)
+	def set_Name(self, Name):  # String
+		self.add_query_param('Name', Name)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/RemoveUsersRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/DeleteCallTagRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,29 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class RemoveUsersRequest(RpcRequest):
+class DeleteCallTagRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'RemoveUsers')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'DeleteCallTag')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_TagName(self): # String
+		return self.get_query_params().get('TagName')
 
-	def get_UserIdList(self):
-		return self.get_query_params().get('UserIdList')
-
-	def set_UserIdList(self,UserIdList):
-		self.add_query_param('UserIdList',UserIdList)
-
-	def get_InstanceId(self):
+	def set_TagName(self, TagName):  # String
+		self.add_query_param('TagName', TagName)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ResetAgentStateRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/CreateCallTagsRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,35 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ResetAgentStateRequest(RpcRequest):
+class CreateCallTagsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ResetAgentState')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'CreateCallTags')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_UserId(self):
-		return self.get_query_params().get('UserId')
-
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
-		return self.get_query_params().get('DeviceId')
-
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_InstanceId(self):
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_CallTagNameList(self): # String
+		return self.get_query_params().get('CallTagNameList')
+
+	def set_CallTagNameList(self, CallTagNameList):  # String
+		self.add_query_param('CallTagNameList', CallTagNameList)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ResetUserPasswordRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListOutboundNumbersOfUserRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,35 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ResetUserPasswordRequest(RpcRequest):
+class ListOutboundNumbersOfUserRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ResetUserPassword')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListOutboundNumbersOfUser')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_UserId(self):
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_Password(self):
-		return self.get_query_params().get('Password')
-
-	def set_Password(self,Password):
-		self.add_query_param('Password',Password)
-
-	def get_InstanceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_PageNumber(self): # Integer
+		return self.get_query_params().get('PageNumber')
+
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_SkillGroupIdList(self): # String
+		return self.get_query_params().get('SkillGroupIdList')
+
+	def set_SkillGroupIdList(self, SkillGroupIdList):  # String
+		self.add_query_param('SkillGroupIdList', SkillGroupIdList)
+	def get_PageSize(self): # Integer
+		return self.get_query_params().get('PageSize')
+
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/ResumeCampaignRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/LaunchAuthenticationRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,29 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class ResumeCampaignRequest(RpcRequest):
+class LaunchAuthenticationRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ResumeCampaign')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'LaunchAuthentication')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ContactFlowId(self): # String
+		return self.get_query_params().get('ContactFlowId')
 
-	def get_InstanceId(self):
-		return self.get_query_params().get('InstanceId')
+	def set_ContactFlowId(self, ContactFlowId):  # String
+		self.add_query_param('ContactFlowId', ContactFlowId)
+	def get_ContactFlowVariables(self): # String
+		return self.get_query_params().get('ContactFlowVariables')
+
+	def set_ContactFlowVariables(self, ContactFlowVariables):  # String
+		self.add_query_param('ContactFlowVariables', ContactFlowVariables)
+	def get_UserId(self): # String
+		return self.get_query_params().get('UserId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_DeviceId(self): # String
+		return self.get_query_params().get('DeviceId')
 
-	def get_CampaignId(self):
-		return self.get_query_params().get('CampaignId')
+	def set_DeviceId(self, DeviceId):  # String
+		self.add_query_param('DeviceId', DeviceId)
+	def get_JobId(self): # String
+		return self.get_query_params().get('JobId')
+
+	def set_JobId(self, JobId):  # String
+		self.add_query_param('JobId', JobId)
+	def get_InstanceId(self): # String
+		return self.get_query_params().get('InstanceId')
 
-	def set_CampaignId(self,CampaignId):
-		self.add_query_param('CampaignId',CampaignId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/RetrieveCallRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/SaveTerminalLogRequest.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,47 +16,63 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class RetrieveCallRequest(RpcRequest):
+class SaveTerminalLogRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'RetrieveCall')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'SaveTerminalLog')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_CallId(self): # String
+		return self.get_query_params().get('CallId')
 
-	def get_UserId(self):
-		return self.get_query_params().get('UserId')
-
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
-		return self.get_query_params().get('DeviceId')
-
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_JobId(self):
+	def set_CallId(self, CallId):  # String
+		self.add_query_param('CallId', CallId)
+	def get_Content(self): # String
+		return self.get_query_params().get('Content')
+
+	def set_Content(self, Content):  # String
+		self.add_query_param('Content', Content)
+	def get_UniqueRequestId(self): # String
+		return self.get_query_params().get('UniqueRequestId')
+
+	def set_UniqueRequestId(self, UniqueRequestId):  # String
+		self.add_query_param('UniqueRequestId', UniqueRequestId)
+	def get_JobId(self): # String
 		return self.get_query_params().get('JobId')
 
-	def set_JobId(self,JobId):
-		self.add_query_param('JobId',JobId)
-
-	def get_InstanceId(self):
+	def set_JobId(self, JobId):  # String
+		self.add_query_param('JobId', JobId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_ChannelId(self):
-		return self.get_query_params().get('ChannelId')
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_AppName(self): # String
+		return self.get_query_params().get('AppName')
+
+	def set_AppName(self, AppName):  # String
+		self.add_query_param('AppName', AppName)
+	def get_DataType(self): # Integer
+		return self.get_query_params().get('DataType')
+
+	def set_DataType(self, DataType):  # Integer
+		self.add_query_param('DataType', DataType)
+	def get_Status(self): # String
+		return self.get_query_params().get('Status')
+
+	def set_Status(self, Status):  # String
+		self.add_query_param('Status', Status)
+	def get_MethodName(self): # String
+		return self.get_query_params().get('MethodName')
 
-	def set_ChannelId(self,ChannelId):
-		self.add_query_param('ChannelId',ChannelId)
+	def set_MethodName(self, MethodName):  # String
+		self.add_query_param('MethodName', MethodName)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/SaveRTCStatsV2Request.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/SendDtmfSignalingRequest.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,53 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class SaveRTCStatsV2Request(RpcRequest):
+class SendDtmfSignalingRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'SaveRTCStatsV2')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'SendDtmfSignaling')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Dtmf(self): # String
+		return self.get_query_params().get('Dtmf')
 
-	def get_CallId(self):
-		return self.get_query_params().get('CallId')
-
-	def set_CallId(self,CallId):
-		self.add_query_param('CallId',CallId)
-
-	def get_SenderReport(self):
-		return self.get_query_params().get('SenderReport')
-
-	def set_SenderReport(self,SenderReport):
-		self.add_query_param('SenderReport',SenderReport)
-
-	def get_InstanceId(self):
+	def set_Dtmf(self, Dtmf):  # String
+		self.add_query_param('Dtmf', Dtmf)
+	def get_UserId(self): # String
+		return self.get_query_params().get('UserId')
+
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_DeviceId(self): # String
+		return self.get_query_params().get('DeviceId')
+
+	def set_DeviceId(self, DeviceId):  # String
+		self.add_query_param('DeviceId', DeviceId)
+	def get_JobId(self): # String
+		return self.get_query_params().get('JobId')
+
+	def set_JobId(self, JobId):  # String
+		self.add_query_param('JobId', JobId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_ReceiverReport(self):
-		return self.get_query_params().get('ReceiverReport')
-
-	def set_ReceiverReport(self,ReceiverReport):
-		self.add_query_param('ReceiverReport',ReceiverReport)
-
-	def get_GoogAddress(self):
-		return self.get_query_params().get('GoogAddress')
-
-	def set_GoogAddress(self,GoogAddress):
-		self.add_query_param('GoogAddress',GoogAddress)
-
-	def get_GeneralInfo(self):
-		return self.get_query_params().get('GeneralInfo')
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_ChannelId(self): # String
+		return self.get_query_params().get('ChannelId')
 
-	def set_GeneralInfo(self,GeneralInfo):
-		self.add_query_param('GeneralInfo',GeneralInfo)
+	def set_ChannelId(self, ChannelId):  # String
+		self.add_query_param('ChannelId', ChannelId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/SaveTerminalLogRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListPersonalNumbersOfUserRequest.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,71 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class SaveTerminalLogRequest(RpcRequest):
+class ListPersonalNumbersOfUserRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'SaveTerminalLog')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListPersonalNumbersOfUser')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_UserId(self): # String
+		return self.get_query_params().get('UserId')
 
-	def get_CallId(self):
-		return self.get_query_params().get('CallId')
-
-	def set_CallId(self,CallId):
-		self.add_query_param('CallId',CallId)
-
-	def get_Content(self):
-		return self.get_query_params().get('Content')
-
-	def set_Content(self,Content):
-		self.add_query_param('Content',Content)
-
-	def get_UniqueRequestId(self):
-		return self.get_query_params().get('UniqueRequestId')
-
-	def set_UniqueRequestId(self,UniqueRequestId):
-		self.add_query_param('UniqueRequestId',UniqueRequestId)
-
-	def get_JobId(self):
-		return self.get_query_params().get('JobId')
-
-	def set_JobId(self,JobId):
-		self.add_query_param('JobId',JobId)
-
-	def get_InstanceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_PageNumber(self): # Integer
+		return self.get_query_params().get('PageNumber')
+
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_IsMember(self): # Boolean
+		return self.get_query_params().get('IsMember')
+
+	def set_IsMember(self, IsMember):  # Boolean
+		self.add_query_param('IsMember', IsMember)
+	def get_SearchPattern(self): # String
+		return self.get_query_params().get('SearchPattern')
+
+	def set_SearchPattern(self, SearchPattern):  # String
+		self.add_query_param('SearchPattern', SearchPattern)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_AppName(self):
-		return self.get_query_params().get('AppName')
-
-	def set_AppName(self,AppName):
-		self.add_query_param('AppName',AppName)
-
-	def get_DataType(self):
-		return self.get_query_params().get('DataType')
-
-	def set_DataType(self,DataType):
-		self.add_query_param('DataType',DataType)
-
-	def get_Status(self):
-		return self.get_query_params().get('Status')
-
-	def set_Status(self,Status):
-		self.add_query_param('Status',Status)
-
-	def get_MethodName(self):
-		return self.get_query_params().get('MethodName')
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_PageSize(self): # Integer
+		return self.get_query_params().get('PageSize')
 
-	def set_MethodName(self,MethodName):
-		self.add_query_param('MethodName',MethodName)
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/SaveWebRTCStatsRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/StartBack2BackCallRequest.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,53 +16,53 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class SaveWebRTCStatsRequest(RpcRequest):
+class StartBack2BackCallRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'SaveWebRTCStats')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'StartBack2BackCall')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Callee(self): # String
+		return self.get_query_params().get('Callee')
 
-	def get_CallId(self):
-		return self.get_query_params().get('CallId')
-
-	def set_CallId(self,CallId):
-		self.add_query_param('CallId',CallId)
-
-	def get_SenderReport(self):
-		return self.get_query_params().get('SenderReport')
-
-	def set_SenderReport(self,SenderReport):
-		self.add_query_param('SenderReport',SenderReport)
-
-	def get_InstanceId(self):
+	def set_Callee(self, Callee):  # String
+		self.add_query_param('Callee', Callee)
+	def get_Broker(self): # String
+		return self.get_query_params().get('Broker')
+
+	def set_Broker(self, Broker):  # String
+		self.add_query_param('Broker', Broker)
+	def get_AdditionalBroker(self): # String
+		return self.get_query_params().get('AdditionalBroker')
+
+	def set_AdditionalBroker(self, AdditionalBroker):  # String
+		self.add_query_param('AdditionalBroker', AdditionalBroker)
+	def get_Tags(self): # String
+		return self.get_query_params().get('Tags')
+
+	def set_Tags(self, Tags):  # String
+		self.add_query_param('Tags', Tags)
+	def get_TimeoutSeconds(self): # Integer
+		return self.get_query_params().get('TimeoutSeconds')
+
+	def set_TimeoutSeconds(self, TimeoutSeconds):  # Integer
+		self.add_query_param('TimeoutSeconds', TimeoutSeconds)
+	def get_Caller(self): # String
+		return self.get_query_params().get('Caller')
+
+	def set_Caller(self, Caller):  # String
+		self.add_query_param('Caller', Caller)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_ReceiverReport(self):
-		return self.get_query_params().get('ReceiverReport')
-
-	def set_ReceiverReport(self,ReceiverReport):
-		self.add_query_param('ReceiverReport',ReceiverReport)
-
-	def get_GoogAddress(self):
-		return self.get_query_params().get('GoogAddress')
-
-	def set_GoogAddress(self,GoogAddress):
-		self.add_query_param('GoogAddress',GoogAddress)
-
-	def get_GeneralInfo(self):
-		return self.get_query_params().get('GeneralInfo')
-
-	def set_GeneralInfo(self,GeneralInfo):
-		self.add_query_param('GeneralInfo',GeneralInfo)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/SaveWebRtcInfoRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListContactFlowsRequest.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,47 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class SaveWebRtcInfoRequest(RpcRequest):
+class ListContactFlowsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'SaveWebRtcInfo')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListContactFlows')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Type(self): # String
+		return self.get_query_params().get('Type')
 
-	def get_CallId(self):
-		return self.get_query_params().get('CallId')
-
-	def set_CallId(self,CallId):
-		self.add_query_param('CallId',CallId)
-
-	def get_Content(self):
-		return self.get_query_params().get('Content')
-
-	def set_Content(self,Content):
-		self.add_query_param('Content',Content)
-
-	def get_ContentType(self):
-		return self.get_query_params().get('ContentType')
-
-	def set_ContentType(self,ContentType):
-		self.add_query_param('ContentType',ContentType)
-
-	def get_JobId(self):
-		return self.get_query_params().get('JobId')
-
-	def set_JobId(self,JobId):
-		self.add_query_param('JobId',JobId)
-
-	def get_InstanceId(self):
+	def set_Type(self, Type):  # String
+		self.add_query_param('Type', Type)
+	def get_PageNumber(self): # Integer
+		return self.get_query_params().get('PageNumber')
+
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_PageSize(self): # Integer
+		return self.get_query_params().get('PageSize')
+
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/SignOutGroupRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/SignOutGroupRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,31 +20,29 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
 class SignOutGroupRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'SignOutGroup')
-		self.set_method('POST')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_UserId(self):
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_DeviceId(self): # String
 		return self.get_query_params().get('DeviceId')
 
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_InstanceId(self):
+	def set_DeviceId(self, DeviceId):  # String
+		self.add_query_param('DeviceId', DeviceId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/StartBack2BackCallRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/ListPhoneNumbersOfSkillGroupRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,59 +16,53 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class StartBack2BackCallRequest(RpcRequest):
+class ListPhoneNumbersOfSkillGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'StartBack2BackCall')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'ListPhoneNumbersOfSkillGroup')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Active(self): # Boolean
+		return self.get_query_params().get('Active')
 
-	def get_Callee(self):
-		return self.get_query_params().get('Callee')
-
-	def set_Callee(self,Callee):
-		self.add_query_param('Callee',Callee)
-
-	def get_Broker(self):
-		return self.get_query_params().get('Broker')
-
-	def set_Broker(self,Broker):
-		self.add_query_param('Broker',Broker)
-
-	def get_AdditionalBroker(self):
-		return self.get_query_params().get('AdditionalBroker')
-
-	def set_AdditionalBroker(self,AdditionalBroker):
-		self.add_query_param('AdditionalBroker',AdditionalBroker)
-
-	def get_Tags(self):
-		return self.get_query_params().get('Tags')
-
-	def set_Tags(self,Tags):
-		self.add_query_param('Tags',Tags)
-
-	def get_TimeoutSeconds(self):
-		return self.get_query_params().get('TimeoutSeconds')
-
-	def set_TimeoutSeconds(self,TimeoutSeconds):
-		self.add_query_param('TimeoutSeconds',TimeoutSeconds)
-
-	def get_Caller(self):
-		return self.get_query_params().get('Caller')
-
-	def set_Caller(self,Caller):
-		self.add_query_param('Caller',Caller)
-
-	def get_InstanceId(self):
+	def set_Active(self, Active):  # Boolean
+		self.add_query_param('Active', Active)
+	def get_PageNumber(self): # Integer
+		return self.get_query_params().get('PageNumber')
+
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_IsMember(self): # Boolean
+		return self.get_query_params().get('IsMember')
+
+	def set_IsMember(self, IsMember):  # Boolean
+		self.add_query_param('IsMember', IsMember)
+	def get_SearchPattern(self): # String
+		return self.get_query_params().get('SearchPattern')
+
+	def set_SearchPattern(self, SearchPattern):  # String
+		self.add_query_param('SearchPattern', SearchPattern)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_SkillGroupId(self): # String
+		return self.get_query_params().get('SkillGroupId')
+
+	def set_SkillGroupId(self, SkillGroupId):  # String
+		self.add_query_param('SkillGroupId', SkillGroupId)
+	def get_PageSize(self): # Integer
+		return self.get_query_params().get('PageSize')
+
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/SubmitCampaignRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetHistoricalCampaignReportRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,29 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class SubmitCampaignRequest(RpcRequest):
+class GetHistoricalCampaignReportRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'SubmitCampaign')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetHistoricalCampaignReport')
+		self.set_method('GET')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_CampaignId(self): # String
+		return self.get_query_params().get('CampaignId')
 
-	def get_InstanceId(self):
+	def set_CampaignId(self, CampaignId):  # String
+		self.add_query_param('CampaignId', CampaignId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_CampaignId(self):
-		return self.get_query_params().get('CampaignId')
-
-	def set_CampaignId(self,CampaignId):
-		self.add_query_param('CampaignId',CampaignId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/TakeBreakRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/GetMultiChannelRecordingRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,41 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class TakeBreakRequest(RpcRequest):
+class GetMultiChannelRecordingRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'TakeBreak')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'GetMultiChannelRecording')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ContactId(self): # String
+		return self.get_query_params().get('ContactId')
 
-	def get_Code(self):
-		return self.get_query_params().get('Code')
-
-	def set_Code(self,Code):
-		self.add_query_param('Code',Code)
-
-	def get_UserId(self):
-		return self.get_query_params().get('UserId')
-
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
-		return self.get_query_params().get('DeviceId')
-
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_InstanceId(self):
+	def set_ContactId(self, ContactId):  # String
+		self.add_query_param('ContactId', ContactId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/UnmuteCallRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/MuteCallRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,47 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class UnmuteCallRequest(RpcRequest):
+class MuteCallRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'UnmuteCall')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'MuteCall')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_UserId(self):
+	def get_UserId(self): # String
 		return self.get_query_params().get('UserId')
 
-	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
-
-	def get_DeviceId(self):
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_DeviceId(self): # String
 		return self.get_query_params().get('DeviceId')
 
-	def set_DeviceId(self,DeviceId):
-		self.add_query_param('DeviceId',DeviceId)
-
-	def get_JobId(self):
+	def set_DeviceId(self, DeviceId):  # String
+		self.add_query_param('DeviceId', DeviceId)
+	def get_JobId(self): # String
 		return self.get_query_params().get('JobId')
 
-	def set_JobId(self,JobId):
-		self.add_query_param('JobId',JobId)
-
-	def get_InstanceId(self):
+	def set_JobId(self, JobId):  # String
+		self.add_query_param('JobId', JobId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_ChannelId(self):
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_ChannelId(self): # String
 		return self.get_query_params().get('ChannelId')
 
-	def set_ChannelId(self,ChannelId):
-		self.add_query_param('ChannelId',ChannelId)
+	def set_ChannelId(self, ChannelId):  # String
+		self.add_query_param('ChannelId', ChannelId)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/aliyunsdkccc/request/v20200701/UpdateConfigItemsRequest.py` & `aliyun-python-sdk-ccc-2.4.3/aliyunsdkccc/request/v20200701/LaunchSurveyRequest.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,41 +16,58 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkccc.endpoint import endpoint_data
 
-class UpdateConfigItemsRequest(RpcRequest):
+class LaunchSurveyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'UpdateConfigItems')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'CCC', '2020-07-01', 'LaunchSurvey')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ContactFlowId(self): # String
+		return self.get_query_params().get('ContactFlowId')
 
-	def get_ConfigItems(self):
-		return self.get_query_params().get('ConfigItems')
-
-	def set_ConfigItems(self,ConfigItems):
-		self.add_query_param('ConfigItems',ConfigItems)
-
-	def get_InstanceId(self):
+	def set_ContactFlowId(self, ContactFlowId):  # String
+		self.add_query_param('ContactFlowId', ContactFlowId)
+	def get_ContactFlowVariables(self): # String
+		return self.get_query_params().get('ContactFlowVariables')
+
+	def set_ContactFlowVariables(self, ContactFlowVariables):  # String
+		self.add_query_param('ContactFlowVariables', ContactFlowVariables)
+	def get_UserId(self): # String
+		return self.get_query_params().get('UserId')
+
+	def set_UserId(self, UserId):  # String
+		self.add_query_param('UserId', UserId)
+	def get_DeviceId(self): # String
+		return self.get_query_params().get('DeviceId')
+
+	def set_DeviceId(self, DeviceId):  # String
+		self.add_query_param('DeviceId', DeviceId)
+	def get_JobId(self): # String
+		return self.get_query_params().get('JobId')
+
+	def set_JobId(self, JobId):  # String
+		self.add_query_param('JobId', JobId)
+	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
-	def set_InstanceId(self,InstanceId):
-		self.add_query_param('InstanceId',InstanceId)
-
-	def get_ObjectType(self):
-		return self.get_query_params().get('ObjectType')
-
-	def set_ObjectType(self,ObjectType):
-		self.add_query_param('ObjectType',ObjectType)
-
-	def get_ObjectId(self):
-		return self.get_query_params().get('ObjectId')
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
+	def get_SmsMetadataId(self): # String
+		return self.get_query_params().get('SmsMetadataId')
+
+	def set_SmsMetadataId(self, SmsMetadataId):  # String
+		self.add_query_param('SmsMetadataId', SmsMetadataId)
+	def get_SurveyChannel(self): # String
+		return self.get_query_params().get('SurveyChannel')
 
-	def set_ObjectId(self,ObjectId):
-		self.add_query_param('ObjectId',ObjectId)
+	def set_SurveyChannel(self, SurveyChannel):  # String
+		self.add_query_param('SurveyChannel', SurveyChannel)
```

### Comparing `aliyun-python-sdk-ccc-2.3.0/setup.py` & `aliyun-python-sdk-ccc-2.4.3/setup.py`

 * *Files identical despite different names*

