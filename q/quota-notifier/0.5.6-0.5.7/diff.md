# Comparing `tmp/quota_notifier-0.5.6.tar.gz` & `tmp/quota_notifier-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quota_notifier-0.5.6.tar", max compression
+gzip compressed data, was "quota_notifier-0.5.7.tar", max compression
```

## Comparing `quota_notifier-0.5.6.tar` & `quota_notifier-0.5.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    34906 2023-05-01 16:10:25.970055 quota_notifier-0.5.6/LICENSE.md
--rw-r--r--   0        0        0      653 2023-05-01 16:10:25.970055 quota_notifier-0.5.6/README.md
--rw-r--r--   0        0        0     1288 2023-05-01 16:10:43.702262 quota_notifier-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     1506 2023-05-01 16:10:25.974055 quota_notifier-0.5.6/quota_notifier/__init__.py
--rw-r--r--   0        0        0      202 2023-05-01 16:10:25.974055 quota_notifier-0.5.6/quota_notifier/__main__.py
--rw-r--r--   0        0        0     6662 2023-05-01 16:10:25.974055 quota_notifier-0.5.6/quota_notifier/cli.py
--rw-r--r--   0        0        0      298 2023-05-01 16:10:25.974055 quota_notifier-0.5.6/quota_notifier/data/template.html
--rw-r--r--   0        0        0    10990 2023-05-01 16:10:25.974055 quota_notifier-0.5.6/quota_notifier/disk_utils.py
--rw-r--r--   0        0        0    10400 2023-05-01 16:10:25.974055 quota_notifier-0.5.6/quota_notifier/notify.py
--rw-r--r--   0        0        0     3220 2023-05-01 16:10:25.974055 quota_notifier-0.5.6/quota_notifier/orm.py
--rw-r--r--   0        0        0     8626 2023-05-01 16:10:25.974055 quota_notifier-0.5.6/quota_notifier/settings.py
--rw-r--r--   0        0        0     2874 2023-05-01 16:10:25.974055 quota_notifier-0.5.6/quota_notifier/shell.py
--rw-r--r--   0        0        0     1777 1970-01-01 00:00:00.000000 quota_notifier-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0    34906 2023-05-08 14:17:22.913718 quota_notifier-0.5.7/LICENSE.md
+-rw-r--r--   0        0        0      653 2023-05-08 14:17:22.913718 quota_notifier-0.5.7/README.md
+-rw-r--r--   0        0        0     1415 2023-05-08 14:17:45.889735 quota_notifier-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     1506 2023-05-08 14:17:22.917719 quota_notifier-0.5.7/quota_notifier/__init__.py
+-rw-r--r--   0        0        0      202 2023-05-08 14:17:22.917719 quota_notifier-0.5.7/quota_notifier/__main__.py
+-rw-r--r--   0        0        0     6662 2023-05-08 14:17:22.917719 quota_notifier-0.5.7/quota_notifier/cli.py
+-rw-r--r--   0        0        0      298 2023-05-08 14:17:22.917719 quota_notifier-0.5.7/quota_notifier/data/template.html
+-rw-r--r--   0        0        0    10990 2023-05-08 14:17:22.917719 quota_notifier-0.5.7/quota_notifier/disk_utils.py
+-rw-r--r--   0        0        0    11137 2023-05-08 14:17:22.917719 quota_notifier-0.5.7/quota_notifier/notify.py
+-rw-r--r--   0        0        0     3220 2023-05-08 14:17:22.917719 quota_notifier-0.5.7/quota_notifier/orm.py
+-rw-r--r--   0        0        0     9157 2023-05-08 14:17:22.917719 quota_notifier-0.5.7/quota_notifier/settings.py
+-rw-r--r--   0        0        0     2874 2023-05-08 14:17:22.917719 quota_notifier-0.5.7/quota_notifier/shell.py
+-rw-r--r--   0        0        0     1821 1970-01-01 00:00:00.000000 quota_notifier-0.5.7/PKG-INFO
```

### Comparing `quota_notifier-0.5.6/LICENSE.md` & `quota_notifier-0.5.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.6/README.md` & `quota_notifier-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.6/pyproject.toml` & `quota_notifier-0.5.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "quota-notifier"
-version = "0.5.6"  # Version is set dynamically by the CI tool on publication
+version = "0.5.7"  # Version is set dynamically by the CI tool on publication
 authors = ["Pitt Center for Research Computing", ]
 readme = "README.md"
 description = "Automatic email notification tool for disk quota usage."
 homepage = "https://github.com/pitt-crc/quota_notifier"
 repository = "https://github.com/pitt-crc/quota_notifier"
 documentation = "https://crc-pages.pitt.edu/quota_notifier/"
 keywords = ["disk", "usage", "quota", "notify", "email", ]
@@ -26,14 +26,21 @@
 [tool.poetry.scripts]
 notifier = "quota_notifier.cli:Application.execute"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 pydantic = "1.10.7"
 sqlalchemy = "2.0.12"
+prometheus_client = "0.16.0"
+
+[tool.poetry.group.tests]
+optional = true
+
+[tool.poetry.group.tests.dependencies]
+coverage = "*"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "6.2.1"
 sphinx-argparse = "0.4.0"
```

### Comparing `quota_notifier-0.5.6/quota_notifier/__init__.py` & `quota_notifier-0.5.7/quota_notifier/__init__.py`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.6/quota_notifier/cli.py` & `quota_notifier-0.5.7/quota_notifier/cli.py`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.6/quota_notifier/disk_utils.py` & `quota_notifier-0.5.7/quota_notifier/disk_utils.py`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.6/quota_notifier/notify.py` & `quota_notifier-0.5.7/quota_notifier/notify.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 import logging
 from bisect import bisect_right
 from email.message import EmailMessage
 from pathlib import Path
 from smtplib import SMTP
 from typing import Collection, Optional, Set, Union, Tuple, List
-from typing import Iterable
 
+from prometheus_client import Summary, CollectorRegistry, push_to_gateway
 from sqlalchemy import delete, insert, select
 from sqlalchemy.orm import Session
 
 from .disk_utils import AbstractQuota, BeeGFSQuota, QuotaFactory
 from .orm import DBConnection, Notification
 from .settings import ApplicationSettings
 from .shell import User
@@ -89,15 +89,15 @@
         return email
 
 
 class UserNotifier:
     """Issue and manage user quota notifications"""
 
     @classmethod
-    def get_users(cls) -> Iterable[User]:
+    def get_users(cls) -> List[User]:
         """Return a collection of users to check quotas for
 
         Returns:
             An iterable collection of ``User`` objects
         """
 
         logging.info('Fetching user list...')
@@ -280,15 +280,32 @@
                 cachable_systems_found = True
                 BeeGFSQuota.cache_quotas(name=file_system.name, path=file_system.path, users=users)
 
         if not cachable_systems_found:
             logging.debug('No cachable system queries found')
 
         logging.info('Scanning user quotas...')
+        failures = 0
         for user in users:
             try:
                 self.notify_user(user)
 
             except Exception as caught:
-                # Only include exception information in the logfile, not the console
+                failures += 1
                 logging.getLogger('file_logger').error(f'Error notifying {user}', exc_info=caught)
                 logging.getLogger('console_logger').error(f'Error notifying {user} - {caught}')
+
+        # Check if prometheus reporting is enabled
+        prom_host = ApplicationSettings.get('prometheus_host')
+        if not prom_host:
+            return
+
+        registry = CollectorRegistry()
+        failed_summary = Summary('failed_users', 'Number of users with failed notifications', registry=registry)
+        failed_summary.observe(failures)
+
+        processed_summary = Summary('processed_users', 'Number of users scanned for notification', registry=registry)
+        processed_summary.observe(len(users))
+
+        prom_port = ApplicationSettings.get('prometheus_port')
+        prom_job = ApplicationSettings.get('prometheus_job')
+        push_to_gateway(f'{prom_host}:{prom_port}', job=prom_job, registry=registry)
```

### Comparing `quota_notifier-0.5.6/quota_notifier/orm.py` & `quota_notifier-0.5.7/quota_notifier/orm.py`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.6/quota_notifier/settings.py` & `quota_notifier-0.5.7/quota_notifier/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 Class definitions inheriting from ``BaseSettings`` directly define
 the settings file schema.  The ``ApplicationSettings`` class is used to manage
 application settings in memory.
 
 Module Contents
 ---------------
 """
+
 import logging
 from pathlib import Path
 from tempfile import NamedTemporaryFile
-from typing import Any, List, Union, Tuple, Set, Optional, Literal
+from typing import Any, List, Literal, Optional, Set, Tuple, Union
 
 from pydantic import BaseSettings, Field, validator
 
 DEFAULT_DB_PATH = Path.cwd().resolve() / 'notifier_data.db'
 
 
 class FileSystemSchema(BaseSettings):
@@ -134,14 +135,33 @@
         description='Application logging level.')
 
     log_path: Optional[Path] = Field(
         title='Log Path',
         default_factory=lambda: Path(NamedTemporaryFile().name),
         description='Optionally log application events to a file.')
 
+    # Prometheus settings
+    prometheus_host: str = Field(
+        title='Prometheus Server Host Name',
+        default='',
+        description='Optional report metrics to a Prometheus server.'
+    )
+
+    prometheus_port: int = Field(
+        title='Prometheus Server Port Number',
+        default=9091,
+        description='Port for the Prometheus server'
+    )
+
+    prometheus_job: str = Field(
+        title='Prometheus Job Name',
+        default='notifier',
+        description='Job label attached to pushed metrics '
+    )
+
     # Settings for the smtp host/port
     smtp_host: str = Field(
         title='SMTP Server Host Name',
         default='',
         description='Name of the SMTP host server'
     )
```

### Comparing `quota_notifier-0.5.6/quota_notifier/shell.py` & `quota_notifier-0.5.7/quota_notifier/shell.py`

 * *Files identical despite different names*

### Comparing `quota_notifier-0.5.6/PKG-INFO` & `quota_notifier-0.5.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quota-notifier
-Version: 0.5.6
+Version: 0.5.7
 Summary: Automatic email notification tool for disk quota usage.
 Home-page: https://github.com/pitt-crc/quota_notifier
 Keywords: disk,usage,quota,notify,email
 Author: Pitt Center for Research Computing
 Requires-Python: >=3.8
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: System :: Monitoring
 Classifier: Typing :: Typed
+Requires-Dist: prometheus_client (==0.16.0)
 Requires-Dist: pydantic (==1.10.7)
 Requires-Dist: sqlalchemy (==2.0.12)
 Project-URL: Documentation, https://crc-pages.pitt.edu/quota_notifier/
 Project-URL: Repository, https://github.com/pitt-crc/quota_notifier
 Description-Content-Type: text/markdown
 
 # Storage Quota Notifier
```

