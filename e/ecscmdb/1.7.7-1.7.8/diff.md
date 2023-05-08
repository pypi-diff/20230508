# Comparing `tmp/ecscmdb-1.7.7.tar.gz` & `tmp/ecscmdb-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecscmdb-1.7.7.tar", max compression
+gzip compressed data, was "ecscmdb-1.7.8.tar", max compression
```

## Comparing `ecscmdb-1.7.7.tar` & `ecscmdb-1.7.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    24376 2023-04-21 20:27:34.057888 ecscmdb-1.7.7/ChangeLog
--rw-r--r--   0        0        0     1075 2020-11-06 03:38:26.304234 ecscmdb-1.7.7/LICENSE.txt
--rw-r--r--   0        0        0    21667 2023-03-23 18:57:58.650594 ecscmdb-1.7.7/README.md
--rw-r--r--   0        0        0     1961 2023-04-21 20:27:34.057888 ecscmdb-1.7.7/pyproject.toml
--rw-r--r--   0        0        0      767 2023-01-19 22:49:05.887313 ecscmdb-1.7.7/src/ecscmdb/__init__.py
--rw-r--r--   0        0        0     8431 2023-04-13 20:42:38.830385 ecscmdb-1.7.7/src/ecscmdb/api.py
--rw-r--r--   0        0        0    22980 2023-04-13 20:42:38.830385 ecscmdb-1.7.7/src/ecscmdb/cmdb.py
--rw-r--r--   0        0        0    18320 2023-03-16 21:38:14.128543 ecscmdb-1.7.7/src/ecscmdb/cmdbdiff.py
--rw-r--r--   0        0        0     7543 2023-03-23 22:14:40.750876 ecscmdb-1.7.7/src/ecscmdb/finddifferences.py
--rw-r--r--   0        0        0     9055 2023-03-16 21:38:14.128543 ecscmdb-1.7.7/src/ecscmdb/initcheck.py
--rw-r--r--   0        0        0     4432 2023-03-04 03:40:16.010718 ecscmdb-1.7.7/src/ecscmdb/updatecells.py
--rw-r--r--   0        0        0    23588 1970-01-01 00:00:00.000000 ecscmdb-1.7.7/setup.py
--rw-r--r--   0        0        0    23612 1970-01-01 00:00:00.000000 ecscmdb-1.7.7/PKG-INFO
+-rw-r--r--   0        0        0    24511 2023-05-08 13:58:19.437667 ecscmdb-1.7.8/ChangeLog
+-rw-r--r--   0        0        0     1075 2020-11-06 03:38:26.304234 ecscmdb-1.7.8/LICENSE.txt
+-rw-r--r--   0        0        0    21667 2023-03-23 18:57:58.650594 ecscmdb-1.7.8/README.md
+-rw-r--r--   0        0        0     1960 2023-05-08 13:58:19.438667 ecscmdb-1.7.8/pyproject.toml
+-rw-r--r--   0        0        0      767 2023-01-19 22:49:05.887313 ecscmdb-1.7.8/src/ecscmdb/__init__.py
+-rw-r--r--   0        0        0     8431 2023-04-13 20:42:38.830385 ecscmdb-1.7.8/src/ecscmdb/api.py
+-rw-r--r--   0        0        0    22980 2023-05-08 13:53:07.442434 ecscmdb-1.7.8/src/ecscmdb/cmdb.py
+-rw-r--r--   0        0        0    18320 2023-03-16 21:38:14.128543 ecscmdb-1.7.8/src/ecscmdb/cmdbdiff.py
+-rw-r--r--   0        0        0     7543 2023-03-23 22:14:40.750876 ecscmdb-1.7.8/src/ecscmdb/finddifferences.py
+-rw-r--r--   0        0        0     9055 2023-03-16 21:38:14.128543 ecscmdb-1.7.8/src/ecscmdb/initcheck.py
+-rw-r--r--   0        0        0     4432 2023-03-04 03:40:16.010718 ecscmdb-1.7.8/src/ecscmdb/updatecells.py
+-rw-r--r--   0        0        0    23588 1970-01-01 00:00:00.000000 ecscmdb-1.7.8/setup.py
+-rw-r--r--   0        0        0    23612 1970-01-01 00:00:00.000000 ecscmdb-1.7.8/PKG-INFO
```

### Comparing `ecscmdb-1.7.7/ChangeLog` & `ecscmdb-1.7.8/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2023-05-08  Thomas R. Stevenson  <tom@tom.cc.wayne.edu>
+
+	* pyproject.toml: Update versions to ECScmdb@v1.7.8 and
+	ECSpylibs@v1.1.35.
+
 2023-04-21  Thomas R. Stevenson  <tom@tom.cc.wayne.edu>
 
 	* pyproject.toml: Update ECScmdb to v1.1.7.  Update ECSpylibs
 	version to v1.1.32.
 
 2023-04-13  Thomas R. Stevenson  <tom@tom.cc.wayne.edu>
```

### Comparing `ecscmdb-1.7.7/LICENSE.txt` & `ecscmdb-1.7.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ecscmdb-1.7.7/README.md` & `ecscmdb-1.7.8/README.md`

 * *Files identical despite different names*

### Comparing `ecscmdb-1.7.7/pyproject.toml` & `ecscmdb-1.7.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 #
 # Do NOT edit this system file by hand -- use git.
 # See "URL to git source" below.
 #
 # Author:        $Id: Thomas R. Stevenson <aa0026@wayne.edu> $
 #
-# Last Changed:  $Date: Fri Apr 21 16:27:06 2023 -0400 $
+# Last Changed:  $Date: Mon May 8 09:57:59 2023 -0400 $
 #
 # URL to git source: $URL: git@git.wayne.edu:ECS_Projects/ECScmdb.git $
 #
 [tool.poetry]
 name = "ecscmdb"
-version = "v1.7.7"
+version = "v1.7.8"
 packages = [{include = "ecscmdb", from = "src"}]
 description = "Dump the OpenManage database."
 license = "GPL-3.0-or-later"
 authors = ["Thomas R. Stevenson <aa0026@wayne.edu>"]
 maintainers = ["Thomas R. Stevenson <aa0026@wayne.edu>"]
 readme = "README.md"
 homepage = "https://git.wayne.edu/ECS_Projects/ECScmdb.git"
@@ -46,15 +46,15 @@
 
 [tool.poetry.scripts]
 cmdb = "ecscmdb.cmdb:main"
 cmdbdiff = "ecscmdb.cmdbdiff:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-ecspylibs = "^v1.1.32"
+ecspylibs = "^v1.1.35"
 Autologging = "^1.3.2"
 Jinja2 = "2.11.2"
 Markupsafe = "1.1.1"
 Xlsxwriter = "1.3.1"
 certifi = "^2022.12.7"
 charset-normalizer = "^3.1.0"
 docopt = "^0.6.2"
```

### Comparing `ecscmdb-1.7.7/src/ecscmdb/__init__.py` & `ecscmdb-1.7.8/src/ecscmdb/__init__.py`

 * *Files identical despite different names*

### Comparing `ecscmdb-1.7.7/src/ecscmdb/api.py` & `ecscmdb-1.7.8/src/ecscmdb/api.py`

 * *Files identical despite different names*

### Comparing `ecscmdb-1.7.7/src/ecscmdb/cmdb.py` & `ecscmdb-1.7.8/src/ecscmdb/cmdb.py`

 * *Files identical despite different names*

### Comparing `ecscmdb-1.7.7/src/ecscmdb/cmdbdiff.py` & `ecscmdb-1.7.8/src/ecscmdb/cmdbdiff.py`

 * *Files identical despite different names*

### Comparing `ecscmdb-1.7.7/src/ecscmdb/finddifferences.py` & `ecscmdb-1.7.8/src/ecscmdb/finddifferences.py`

 * *Files identical despite different names*

### Comparing `ecscmdb-1.7.7/src/ecscmdb/initcheck.py` & `ecscmdb-1.7.8/src/ecscmdb/initcheck.py`

 * *Files identical despite different names*

### Comparing `ecscmdb-1.7.7/src/ecscmdb/updatecells.py` & `ecscmdb-1.7.8/src/ecscmdb/updatecells.py`

 * *Files identical despite different names*

### Comparing `ecscmdb-1.7.7/setup.py` & `ecscmdb-1.7.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['Autologging>=1.3.2,<2.0.0',
  'Jinja2==2.11.2',
  'Markupsafe==1.1.1',
  'Xlsxwriter==1.3.1',
  'certifi>=2022.12.7,<2023.0.0',
  'charset-normalizer>=3.1.0,<4.0.0',
  'docopt>=0.6.2,<0.7.0',
- 'ecspylibs>=v1.1.32,<2.0.0',
+ 'ecspylibs>=v1.1.35,<2.0.0',
  'idna>=3.4,<4.0',
  'numpy==1.19.1',
  'pandas==1.0.5',
  'python-dateutil>=2.8.2,<3.0.0',
  'pytz==2020.1',
  'requests>=2.28.2,<3.0.0',
  'six>=1.16.0,<2.0.0',
@@ -31,15 +31,15 @@
 
 entry_points = \
 {'console_scripts': ['cmdb = ecscmdb.cmdb:main',
                      'cmdbdiff = ecscmdb.cmdbdiff:main']}
 
 setup_kwargs = {
     'name': 'ecscmdb',
-    'version': '1.7.7',
+    'version': '1.7.8',
     'description': 'Dump the OpenManage database.',
     'long_description': '# ECScmdb\n\n# CLI Version\n\n    cmdb:     ecscmdb(1.7.2), ecspylibs(1.1.27)\n    cmdbdiff: ecscmdb(1.7.2), ecspylibs(1.1.27)\n\n# Summary of commands\n\n    cmdb:     Download the devices in the OpenManage database into a\n              spreadsheet, one work sheet for each device.\n\n    cmdbdiff: Compare two cmdb spreadsheets for differences.\n\n# Assumptions\n\nThe ecscmdb user needs to know:\n\n* how to run commands in a Linux environment.\n* how to install python packages in a virtualenv.\n* how to run python commands in a virtualenv.\n* how to configure yaml files.\n* some basic understanding of jinja2 variable used in the yaml file.\n\n# Installation\n\n    It is best to create a dedicated python virtualenv to install\n    ecscmdb into so as not to interfere with any other python packages\n    installed on your system.\n\n    # virtualenv .venv\n    # . .venv/bin/activate\n    # pip install ecscmdb\n\n# Setup\n\n## cmdb\n\n    Before cmdb can be used to gather OpenManage data, two config\n    files and one password files must be created.  They are both\n    located in the directory etc/ecscmdb, which is relative to the\n    virtualenv directory ecscmdb was installed in.  The config files\n    can be in yaml, toml, or json formats.  Only yaml format will be\n    used in this documentation.  The two config files are cmdb.yml and\n    filter.yml.\n\n### cmdb.yml\n\n    cmdb.yml is a yaml file. The yaml file can have multiple "config" \n    sections defined within it.  There must be at lease one config section.\n    Each config secion has the following fields:\n    \n    name:       The name of the config section.\n\n    pw:         The location of the cmdb password file relative to \n                virtualenv base directory cmdb was installed in.\n\n    log_level:  The python log level cmdb will run at.  Must be one of \n                DEBUG, INFO, WARNING, ERROR, CRITICAL, or TRACE.\n\n    log_dir:    The location of the cmdb log directory relative to \n                virtualenv base directory cmdb was installed in. \n\n    OME_Login:  The User ID of the OpenManage server that will be used \n                to gather the data.\n\n    poolsize:   The number of python ProcessPoolExecutor pools that will\n                be used to gather the OpenManage data.\n\n    filter:     The location of the cmdb filter file.  The filter\n                file, explained in detail below, scans the incoming\n                OpenManage, and only stores the required columns and\n                rows of the data.  \n    \n    output:     The location of the cmdb output file that the cmdb \n                spreadsheet will be written to.  The name of the file can\n                include the jinja2 variable "{{ TOD }}" to include the \n                current date and time.\n\n    In addition to the config section(s), the yaml file also must include \n    the yaml variable "section:" which indicates which of the config sections\n    to process.\n\n### cmdb.yml example file\n```\nHere is an example cmdb.yml file with two config sections.  Because the\n"section:" variable is set to 2 in this example the second section, with \nname "Configuration file Testing", will be used.\n\n---\nsection: 2\nconfig:\n  - name: Configuration file Production.\n    pw: etc/ecscmdb/cmdb.pw\n    log_level: warning\n    log_dir: log\n    OME_Login: cmdb\n    poolsize: 12\n    filter: etc/ecscmdb/filter.yml\n    output: output/OpenManage-cmdb.{{ TOD }}.xlsx\n  - name: Configuration file Testing.\n    pw: etc/ecscmdb/cmdb.pw\n    log_level: TRACE\n    log_dir: log\n    OME_Login: cmdb\n    poolsize: 24\n    filter: etc/ecscmdb/filter.yml\n    output: output/OpenManage-test-cmdb.{{ TOD }}.xlsx\n...\n```\n\n### filter.yml\n\n    filter.yml is a yaml file. The yaml file can have multiple "config" \n    sections defined within it.  There must be at lease one config section.\n    Each config secion has the following fields:\n    \n    name:           The name of the config section.\n    \n    column_header:  The name of the column used to match the "row" labels.\n    \n    rename_columns: A dictionary of "Old Name": "New Name" used to rename\n                    Column lines.\n    \n    sort_columns:   A list of column names to sort the each worksheet with.\n    \n    filters:        A list of Row:Columns:Update to include from the \n                    OpenManage database into each created worksheet.  The\n                    Update option is optional.\n\t\n        Row:        The names of the row to look for matching columns in\n                    within the OpenManage database data.\n\t\n        Columns:    A list of matching Columns names for the given Row to\n                    include.\n\t\n        Update:     A dictional entry of "Column Name": "Function Name".\n                    If the Column Name is part of the data precented from\n                    the OpenManage database, then the cell for Row:Column\n                    will be modified using the Function Name provided.\n                    The Function is defined in the python library\n                    updatecells.py that is part of the ECScmdb packages.\n                    This should be the only python library that needs to\n                    be modified.\n\n    In addition to the config section(s), the yaml file also must\n    include the yaml variable "section:" which indicates which of the\n    config sections to process.\n\n### filter.yml example file\n```\nHere is an example filter.yml file with one config section.  Because the\n"section:" variable is set to 1 in this example the first section, with \nname "Partial", will be used.\n\n---\nsection: 1\nconfig:\n  - name: Partial\n    column_header: InventoryType\n    rename_columns:\n      Ports: "Mac Address"\n\n    sort_columns:\n      - InventoryType\n      - DeviceDescription\n      - DeviceName\n      - InstanceId\n      - NicId\n      - CapabilityType.CapabilityId\n      - CapabilityType.Description\n      - CapabilityType.IdOwner\n      - CapabilityType.Name\n      - DiskNumber\n      - DnsName\n      - EndDate\n      - EntitlementId\n      - Id\n      - IdOwner\n      - LicenseDescription\n      - LicenseType.LicenseId\n      - LicenseType.Name\n      - Name\n      - Number\n      - SasAddress\n      - SerialNumber\n      - ServiceTag\n      - SlotNumber\n      - SoldDate\n\n    filters:\n      -\n        row: serverProcessors\n        columns:\n          - InstanceId\n          - InventoryType\n          - ModelName\n          - NumberOfCores\n      -\n        row: serverFcCards\n        columns:\n          - DeviceDescription\n          - DeviceName\n          - InventoryType\n          - VirtualWwn\n          - VirtualWwpn\n          - Wwn\n          - Wwpn\n      -\n        row: serverOperatingSystems\n        columns:\n          - Hostname\n          - InventoryType\n          - OsName\n      -\n        row: serverArrayDisks\n        columns:\n          - BusType\n          - DiskNumber\n          - InventoryType\n          - MediaType\n          - ModelNumber\n          - SerialNumber\n          - Size\n      -\n        row: serverMemoryDevices\n        columns:\n          - DeviceDescription\n          - InstanceId\n          - InventoryType\n          - ManufacturerDate\n          - Name\n          - SerialNumber\n          - Size\n          - Speed\n          - TypeDetails\n      -\n        row: serverNetworkInterfaces\n        columns:\n          - InventoryType\n          - NicId\n          - Ports\n        update:\n          Ports: update_ports\n      -\n        row: chassisSlotsList\n        columns:\n          - DnsName\n          - InventoryType\n          - Model\n          - Name\n          - Number\n          - Occupied\n          - ServiceTag\n      -\n        row: chassisControllerList\n        columns:\n          - InventoryType\n          - Name\n      -\n        row: deviceManagement\n        columns:\n          - DnsName\n          - EndPointAgents\n          - InstrumentationName\n          - InventoryType\n          - IpAddress\n          - MacAddress\n          - ManagementId\n          - ManagementType.Description\n          - ManagementType.Name\n        update:\n          EndPointAgents: update_end_point_agents\n      -\n        row: nicInformation\n        columns:\n          - Description\n          - DeviceId\n          - InventoryType\n          - Ipv4_address\n          - Mac_address\n          - Subnet_mask\n...\n```\n\n### cmdb.pw\n    cmdb.pw is a python AES encripted password file.  It must contain the\n    following two entries: \n\n    1. A key that matches the OME_Login variable from the cmdb.yml\n       file. The value of the entry is the password for that user.\n\n    2. A key named "OMEHost" (case-sensitive string).  The value of\n       the entry is the URL for the OpenManage host.\n\n### Adding or updating an entry in the cmdb.pw file\n\n    Execute "cmdb --add=STRING", where STRING is the key to be created\n    or updated.  cmdb will then prompt for the value for the given\n    key.  The entries are encripted and stored in the cmdb.pw file.\n\n### Example \n\n    # cmdb --add=xyzzy\n    Enter password for user \'xyzzy\':\n    #\n\n### Deleting an entry from the cmdb.pw file\n\n    Execute "cmdb --delete=STRING", where STRING is the key to be\n    deleted.  The entries will be deleted without prompting.\n\n### Example\n\n    # cmdb --delete=xyzzy\n    #\n\n### List the keys or keys/values stored n the cmdb.pw file\n\n    Execute "cmdb --list" to list all of the keys in the cmdb.pw file,\n    or "cmdb --list --verbose" to list both the keys and the values\n    for each key.\n\n### Examples\n\n    # cmdb --list\n    # cmdb --list --verbose\n\n## cmdbdiff\n\n    Before cmdbdiff can be used to compare two OpenManage\n    spreadsheets, created using the cmdb command, the file\n    cmdbdiff.yml must be created.  This file is located in the\n    directory etc/ecscmdb, which is relative to the virtualenv\n    directory ecscmdb was installed in.\n\n### cmdbdiff.yml\n\n    cmdbdiff.yml is a yaml file. The yaml file can have multiple\n    "config" sections defined within it.  There must be at least one\n    config section in it.  In addition to the config section(s), the\n    yaml file also must include the yaml variable "section:" which\n    indicates which of the config sections to process.st be at lease\n    one config section.  Each config secion has the following fields:\n\n    name:                       The name of the configuration section \n                                (optional).\n    admin:                      The Admin managing cmdbdiff.\n        name:                   The Admin name.\n        email:                  The Admin email address.\n        phone:                  The Admin phone number.\n    log_level:                  The python log level cmdb will run at.  \n                                Must be one of DEBUG, INFO, WARNING, ERROR, \n                                CRITICAL, or TRACE.\n    log_dir:                    The location of the cmdb log directory \n                                relative to virtualenv base directory cmdb \n                                was installed in.\n    report:                     The location of the cmdbdiff report file \n                                that cmdbdiff writes to.  The name of the \n                                file can include the jinja2 variable \n                                "{{ TOD }}" to include the current date and \n                                time.\n    email:                      The email section indicates who should \n                                receive a copy of the cmdbdiff report.\n        subject:                The subject line of the report email.\n        from:                   The name and email address of the user \n                                sending the report.\n            name:               The sending name.\n            email:              The sending email address.\n        to:                     A list of zero or more "to" email addresses.\n            name:               The outgoing name.\n            email:              The outgoing email address.\n        cc:                     A list of zero or more "cc" email addresses. \n            name:               The outgoing name.\n            email:              The outgoing email address.\n        text:                   The text of the email that is sent.\n            with_changes:       The text of the email being if there are \n                                changes between the spreadsheets being \n                                checked.\n            without_changes:    The text of the email being if there are no \n                                changes between the spreadsheets being \n                                checked. \n\n    In addition to the config section(s), the yaml file also must include \n    the yaml variable "section:" which indicates which of the config sections\n    to process.\n\n### jinja2 variables used in the cmdbdiff.yml file\n\n```\nThere are several jinja2 variables that can be used in the cmdbdiff.yml \nconfiguration file.  Here is a list with a description of their values:\n\nTOD:            The current Date and Time.\nDATE:           The currect Date.\nTIME:           The current Time.\nHOST:           The Host name the report was generated on.\nVERSION:        The Version of the cmdbdiff program.\nSPREADSHEET1:   The name of the first spreadsheet being checked.\nWORKSHEETS1:    The number of Worksheets in the spreadsheet 1.\nSPREADSHEET2:   The name of the second spreadsheet being checked.\nWORKSHEETS2:    The number of Worksheets in the spreadsheet 2.\nREPORT:         The name of the report file (from config.report).\nADMINNAME:      The name of the cmdbdiff Admin (from config.admin.name).\nADMINEMAIL:     The email address of the cmdbdiff Admin (from \n                config.admin.email).\nADMINPHONE:     The phone number of the cmdbdiff Admin (from \n                config.admin.phone).\n```\n\n### cmdbdiff.yml example file\n\n```\nHere is an example cmdb.yml file with one config sections.  The "section:" \nvariable is set to 1 in this example the second section, with name \n"Configuration file Production", will be used.\n\n---\nsection: 1\nconfig:\n  - name: Configuration file Production.\n    admin:\n      name: Bill Jones\n      email: BJ@example.com\n      phone: 999.555.1234\n    log_level: warning\n    log_dir: log\n    report: report/OpenManage-cmdbdiff-{{ TOD }}.xlsx\n    email:\n      subject: CMDB Diff Report generated on {{ DATE }} at {{ TIME }} on server {{ HOST }}.\n      from:\n        name: CMDB Diff Report\n        email: CMDB-Diff-Report@{{ HOST }}\n      to:\n        -\n          name: John Smith\n          email: JS@example.com\n        -\n          name: Steve Thomas\n          email: ST@example.com\n      cc:\n        -\n          name: Tim George\n          email: TG@example.com\n      text:\n        with_changes:\n\n          "\\nCMDB Diff report, Version {{ VERSION }}, generated on {{ DATE\n          }} at {{ TIME }} on server {{ HOST }}.\\n\n\n          There are three attached spreadsheets in this report:\\n\n\n          1) {{ SPREADSHEET1 }}, is the previous CMDB spreadsheet with\n          {{ WORKSHEETS1 }} worksheets.\\n\n\n          2) {{ SPREADSHEET2 }}, is an currect CMDB spreadsheet with {{\n          WORKSHEETS2 }} worksheets.\\n\n\n          3) {{ REPORT }}, lists the changes between {{ SPREADSHEET1 }}\n          and {{ SPREADSHEET2 }}.\\n\n\n          The first worksheet in {{ REPORT }} lists a summary of all\n          changes. The remaining worksheets in {{ REPORT }}, if any, are\n          copies of the worksheets in {{ SPREADSHEET2 }} that are\n          different from {{ SPREADSHEET1 }}.\\n\n\n          Contact {{ ADMINNAME }} at email address {{ ADMINEMAIL }} or\n          phone number {{ ADMINPHONE }} if you have questions or\n          concerns regarding any of the spreadsheets generated in this\n          report.\\n\n\n          Thanks!\\n"\n\n        without_changes:\n\n          "\\nCMDB Diff report, Version {{ VERSION }}, generated on {{ DATE\n          }} at {{ TIME }} on server {{ HOST }}.\\n\n\n          The CMDB Diff report found no changes between {{\n          SPREADSHEET1 }} and {{ SPREADSHEET1 }} on {{ DATE }}.\\n\n\n          There are three attached spreadsheets in this report:\\n\n\n          1) {{ SPREADSHEET1 }}, is the previous CMDB spreadsheet with\n          {{ WORKSHEETS1 }} worksheets.\\n\n\n          2) {{ SPREADSHEET2 }}, is an currect CMDB spreadsheet with {{\n          WORKSHEETS2 }} worksheets.\\n\n\n          3) {{ REPORT }}, lists the changes between {{ SPREADSHEET1 }}\n          and {{ SPREADSHEET2 }}.\\n\n\n          Contact {{ ADMINNAME }} at email address {{ ADMINEMAIL }} or\n          phone number {{ ADMINPHONE }} if you have questions or\n          concerns regarding any of the spreadsheets generated in this\n          report.\\n\n\n          Thanks!\\n"\n\n```\n\n# CLI Help text\n\n## # cmdb --help\n\n    Program to download the data from the OpenManage DB and build a spreadsheet.\n\n    Some default option values listed below can be overridden within the\n    configuration file.\n\n    Usage:\n      cmdb [-v] [-L LEVEL] [--LOG=DIR] [-F] [-c CONFIG] [-s SECTION] [-o OUTPUT] [-p PWFILE] [-D] [-P SIZE]\n      cmdb [-vl] [-L LEVEL] [--LOG=DIR] [-c CONFIG] [-s SECTION] [-a ID]... [-d ID]... [-p PWFILE] [-D]\n      cmdb (-h | --help | -V | --version)\n\n      There are no required options.\n\n    Options:\n      -h, --help                     Show this help message and exit.\n      -V, --version                  Show version information and exit.\n      -F, --full                     Show all data, no filtering.\n      -c CONFIG, --config=CONFIG     The configuration file.\n                                     Default: "/home/tom/Run/ECScmdb/Testing/etc/ecscmdb/cmdb.yml"\n      -s SECTION, --section=SECTION  The configuration file version (default\n                                     defined within the configuration file).\n      -o OUTPUT, --output=OUTPUT     Output file or directory.\n                                     Default: "/home/tom/Run/ECScmdb/Testing/output/OpenManage-cmdb.2023-02-08-18-14-30.xlsx"\n      -p PWFILE, --pw=PWFILE         The password file.  This file is used when a\n                                     login to a website or webpage is required.\n                                     Default: "/home/tom/Run/ECScmdb/Testing/etc/ecscmdb/cmdb.pw"\n      -l, --list                     List all of the IDs in the password file and\n                                     exit.  If both the --list and --verbose\n                                     options are included, list both IDs and\n                                     Passwords and exit.\n      -a ID, --add=ID                Add (or update) an ID and Password and exit.\n                                     Program will prompt for the Password to be\n                                     saved to the password file.\n      -d ID, --delete=ID             Delete an ID (if it exists) from the\n                                     password file and exit.\n      -v, --verbose                  Print verbose messages.\n      -L LEVEL, --log=LEVEL          Print log messages at log value LEVEL.\n                                     Valid levels are: TRACE, DEBUG, INFO, WARNING,\n                                     ERROR, and CRITICAL.\n                                     Default: WARNING\n      --LOG=DIR                      Log directory.\n                                     Default: "/home/tom/Run/ECScmdb/Testing/log/cmdb.log"\n      -D, --dryrun                   Only print out what would be done.\n      -P SIZE, --poolsize=SIZE       Call OpenManage using pools of size SIZE.\n                                     Default: set by the OS.\n\n## # cmdbdiff --help\n\n    Program to analyze two spreadsheets for differences.\n\n    Some default option values listed below can be overridden within the initialization file.\n\n    Usage:\n      cmdbdiff [-v] [-L LEVEL] [--LOG=DIR] [-c CONFIG] [-s SECTION] [-r REPORT] [-D] SPREADSHEET1 SPREADSHEET2\n      cmdbdiff (-h | --help | -V | --version)\n\n      Variables SPREADSHEET1 and SPREADSHEET2 are required, all other parameters are optional.\n\n    Options:\n      -h, --help                          Show this help message and exit.\n      -V, --version                       Show version information and exit.\n      -c CONFIG, --config=CONFIG          The configuration file.\n                                          Default: "/home/tom/Run/ECScmdb/Testing/etc/ecscmdb/cmdbdiff.yml"\n      -s SECTION, --section=SECTION       The configuration file version (default\n                                          defined within the configuration file).\n      -r REPORT, --report=REPORT          Report directory or file.\n      -v, --verbose                       Print verbose messages.\n      -L LEVEL, --log=LEVEL               Print log messages at log value LEVEL.\n                                          Valid levels are: TRACE, DEBUG, INFO, WARNING,\n                                          ERROR, and CRITICAL.\n                                          Default: "WARNING"\n      --LOG=DIR                           Log Directory,\n                                          Default: "/home/tom/Run/ECScmdb/Testing/log/cmdbdiff.log"\n      -D, --dryrun                        Only print out what would be done.\n \n# Git information\n[GIT Home][CMDB],\n[README File][README],\n[LICENSE File][LICENSE],\n[ChangeLog File][CHANGELOG],\n[pyproject.toml File][PYPROJECT].\n\n# About me\n[My contact information][About Me].\n\n[CMDB]: https://git.wayne.edu/ECS_Projects/ECScmdb\n[README]: https://git.wayne.edu/ECS_Projects/ECScmdb/-/blob/master/README.md\n[LICENSE]: https://git.wayne.edu/ECS_Projects/ECScmdb/-/blob/master/LICENSE.txt\n[CHANGELOG]: https://git.wayne.edu/ECS_Projects/ECScmdb/-/blob/master/ChangeLog\n[PYPROJECT]: https://git.wayne.edu/ECS_Projects/ECScmdb/-/blob/master/pyproject.toml\n[About Me]: https://About.Me/Thomas.R.Stevenson\n',
     'author': 'Thomas R. Stevenson',
     'author_email': 'aa0026@wayne.edu',
     'maintainer': 'Thomas R. Stevenson',
     'maintainer_email': 'aa0026@wayne.edu',
     'url': 'https://git.wayne.edu/ECS_Projects/ECScmdb.git',
```

### Comparing `ecscmdb-1.7.7/PKG-INFO` & `ecscmdb-1.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecscmdb
-Version: 1.7.7
+Version: 1.7.8
 Summary: Dump the OpenManage database.
 Home-page: https://git.wayne.edu/ECS_Projects/ECScmdb.git
 License: GPL-3.0-or-later
 Keywords: cmdb,cmdbdiff
 Author: Thomas R. Stevenson
 Author-email: aa0026@wayne.edu
 Maintainer: Thomas R. Stevenson
@@ -25,15 +25,15 @@
 Requires-Dist: Autologging (>=1.3.2,<2.0.0)
 Requires-Dist: Jinja2 (==2.11.2)
 Requires-Dist: Markupsafe (==1.1.1)
 Requires-Dist: Xlsxwriter (==1.3.1)
 Requires-Dist: certifi (>=2022.12.7,<2023.0.0)
 Requires-Dist: charset-normalizer (>=3.1.0,<4.0.0)
 Requires-Dist: docopt (>=0.6.2,<0.7.0)
-Requires-Dist: ecspylibs (>=v1.1.32,<2.0.0)
+Requires-Dist: ecspylibs (>=v1.1.35,<2.0.0)
 Requires-Dist: idna (>=3.4,<4.0)
 Requires-Dist: numpy (==1.19.1)
 Requires-Dist: pandas (==1.0.5)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: pytz (==2020.1)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: six (>=1.16.0,<2.0.0)
```

