# Comparing `tmp/django_tsp-3.14.7.tar.gz` & `tmp/django_tsp-3.14.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tsp-3.14.7.tar", last modified: Sun May  7 19:01:16 2023, max compression
+gzip compressed data, was "django_tsp-3.14.8.tar", last modified: Mon May  8 14:48:40 2023, max compression
```

## Comparing `django_tsp-3.14.7.tar` & `django_tsp-3.14.8.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-07 19:01:16.781947 django_tsp-3.14.7/
--rw-r--r--   0 abb       (1000) abb       (1000)    11813 2023-04-28 13:49:49.000000 django_tsp-3.14.7/CHANGELOG.rst
--rw-r--r--   0 abb       (1000) abb       (1000)     1078 2023-04-19 16:29:15.000000 django_tsp-3.14.7/LICENSE
--rw-r--r--   0 abb       (1000) abb       (1000)      206 2023-05-07 19:00:59.000000 django_tsp-3.14.7/MANIFEST.in
--rw-r--r--   0 abb       (1000) abb       (1000)     1462 2023-05-07 19:01:16.781947 django_tsp-3.14.7/PKG-INFO
--rw-r--r--   0 abb       (1000) abb       (1000)       44 2023-04-19 16:29:15.000000 django_tsp-3.14.7/README.md
--rw-r--r--   0 abb       (1000) abb       (1000)      499 2023-04-28 10:29:09.000000 django_tsp-3.14.7/pyproject.toml
--rw-r--r--   0 abb       (1000) abb       (1000)     1705 2023-05-07 19:01:16.785280 django_tsp-3.14.7/setup.cfg
-drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-07 19:01:16.548607 django_tsp-3.14.7/src/
-drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-07 19:01:16.551941 django_tsp-3.14.7/src/django_tsp/
--rw-r--r--   0 abb       (1000) abb       (1000)        0 2023-04-09 10:17:38.000000 django_tsp-3.14.7/src/django_tsp/__init__.py
--rw-r--r--   0 abb       (1000) abb       (1000)     1766 2023-05-07 17:51:34.000000 django_tsp-3.14.7/src/django_tsp/apis.py
--rw-r--r--   0 abb       (1000) abb       (1000)      429 2023-04-28 14:31:07.000000 django_tsp-3.14.7/src/django_tsp/apps.py
--rw-r--r--   0 abb       (1000) abb       (1000)     1141 2023-05-07 17:51:34.000000 django_tsp-3.14.7/src/django_tsp/checks.py
--rw-r--r--   0 abb       (1000) abb       (1000)      448 2023-05-07 18:18:07.000000 django_tsp-3.14.7/src/django_tsp/conf.py
--rw-r--r--   0 abb       (1000) abb       (1000)      590 2023-05-07 17:51:34.000000 django_tsp-3.14.7/src/django_tsp/consumer.py
-drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-07 19:01:16.548607 django_tsp-3.14.7/src/django_tsp/management/
-drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-07 19:01:16.555274 django_tsp-3.14.7/src/django_tsp/management/commands/
-drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-07 19:01:16.738613 django_tsp-3.14.7/src/django_tsp/management/commands/__pycache__/
--rw-r--r--   0 abb       (1000) abb       (1000)      904 2023-05-07 09:12:22.000000 django_tsp-3.14.7/src/django_tsp/management/commands/__pycache__/bridge.cpython-310.pyc
--rw-r--r--   0 abb       (1000) abb       (1000)     1265 2023-05-07 17:13:27.000000 django_tsp-3.14.7/src/django_tsp/management/commands/__pycache__/reciver.cpython-310.pyc
--rw-r--r--   0 abb       (1000) abb       (1000)      426 2023-05-07 17:51:34.000000 django_tsp-3.14.7/src/django_tsp/management/commands/bridge.py
--rw-r--r--   0 abb       (1000) abb       (1000)      707 2023-05-07 17:51:34.000000 django_tsp-3.14.7/src/django_tsp/management/commands/reciver.py
--rw-r--r--   0 abb       (1000) abb       (1000)      132 2023-05-07 17:51:34.000000 django_tsp-3.14.7/src/django_tsp/routing.py
--rw-r--r--   0 abb       (1000) abb       (1000)      212 2023-05-07 17:51:34.000000 django_tsp-3.14.7/src/django_tsp/serializers.py
--rw-r--r--   0 abb       (1000) abb       (1000)      648 2023-05-07 17:51:34.000000 django_tsp-3.14.7/src/django_tsp/services.py
-drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-07 19:01:16.781947 django_tsp-3.14.7/src/django_tsp/templates/
--rw-r--r--   0 abb       (1000) abb       (1000)     6005 2023-05-07 17:51:34.000000 django_tsp-3.14.7/src/django_tsp/templates/index.html
--rw-r--r--   0 abb       (1000) abb       (1000)      102 2023-05-07 17:51:34.000000 django_tsp-3.14.7/src/django_tsp/views.py
-drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-07 19:01:16.555274 django_tsp-3.14.7/src/django_tsp.egg-info/
--rw-r--r--   0 abb       (1000) abb       (1000)     1462 2023-05-07 19:01:16.000000 django_tsp-3.14.7/src/django_tsp.egg-info/PKG-INFO
--rw-r--r--   0 abb       (1000) abb       (1000)      817 2023-05-07 19:01:16.000000 django_tsp-3.14.7/src/django_tsp.egg-info/SOURCES.txt
--rw-r--r--   0 abb       (1000) abb       (1000)        1 2023-05-07 19:01:16.000000 django_tsp-3.14.7/src/django_tsp.egg-info/dependency_links.txt
--rw-r--r--   0 abb       (1000) abb       (1000)        1 2023-04-28 13:56:46.000000 django_tsp-3.14.7/src/django_tsp.egg-info/not-zip-safe
--rw-r--r--   0 abb       (1000) abb       (1000)       31 2023-05-07 19:01:16.000000 django_tsp-3.14.7/src/django_tsp.egg-info/requires.txt
--rw-r--r--   0 abb       (1000) abb       (1000)       11 2023-05-07 19:01:16.000000 django_tsp-3.14.7/src/django_tsp.egg-info/top_level.txt
+drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-08 14:48:40.158819 django_tsp-3.14.8/
+-rw-r--r--   0 abb       (1000) abb       (1000)     1078 2023-04-19 16:29:15.000000 django_tsp-3.14.8/LICENSE
+-rw-r--r--   0 abb       (1000) abb       (1000)      206 2023-05-08 14:44:07.000000 django_tsp-3.14.8/MANIFEST.in
+-rw-r--r--   0 abb       (1000) abb       (1000)     3441 2023-05-08 14:48:40.158819 django_tsp-3.14.8/PKG-INFO
+-rw-r--r--   0 abb       (1000) abb       (1000)     2020 2023-05-08 14:44:07.000000 django_tsp-3.14.8/README.md
+-rw-r--r--   0 abb       (1000) abb       (1000)      499 2023-04-28 10:29:09.000000 django_tsp-3.14.8/pyproject.toml
+-rw-r--r--   0 abb       (1000) abb       (1000)     1708 2023-05-08 14:48:40.158819 django_tsp-3.14.8/setup.cfg
+drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-08 14:48:40.152152 django_tsp-3.14.8/src/
+drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-08 14:48:40.155485 django_tsp-3.14.8/src/django_tsp/
+-rw-r--r--   0 abb       (1000) abb       (1000)        0 2023-04-09 10:17:38.000000 django_tsp-3.14.8/src/django_tsp/__init__.py
+-rw-r--r--   0 abb       (1000) abb       (1000)     2042 2023-05-08 14:44:07.000000 django_tsp-3.14.8/src/django_tsp/apis.py
+-rw-r--r--   0 abb       (1000) abb       (1000)      533 2023-05-08 14:44:07.000000 django_tsp-3.14.8/src/django_tsp/apps.py
+-rw-r--r--   0 abb       (1000) abb       (1000)     1141 2023-05-07 17:51:34.000000 django_tsp-3.14.8/src/django_tsp/checks.py
+-rw-r--r--   0 abb       (1000) abb       (1000)      448 2023-05-08 14:44:07.000000 django_tsp-3.14.8/src/django_tsp/conf.py
+-rw-r--r--   0 abb       (1000) abb       (1000)      590 2023-05-07 17:51:34.000000 django_tsp-3.14.8/src/django_tsp/consumer.py
+drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-08 14:48:40.152152 django_tsp-3.14.8/src/django_tsp/management/
+drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-08 14:48:40.155485 django_tsp-3.14.8/src/django_tsp/management/commands/
+drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-08 14:48:40.158819 django_tsp-3.14.8/src/django_tsp/management/commands/__pycache__/
+-rw-r--r--   0 abb       (1000) abb       (1000)      904 2023-05-07 09:12:22.000000 django_tsp-3.14.8/src/django_tsp/management/commands/__pycache__/bridge.cpython-310.pyc
+-rw-r--r--   0 abb       (1000) abb       (1000)     1265 2023-05-07 17:13:27.000000 django_tsp-3.14.8/src/django_tsp/management/commands/__pycache__/reciver.cpython-310.pyc
+-rw-r--r--   0 abb       (1000) abb       (1000)      499 2023-05-08 14:44:07.000000 django_tsp-3.14.8/src/django_tsp/management/commands/bridge.py
+-rw-r--r--   0 abb       (1000) abb       (1000)      851 2023-05-08 14:44:07.000000 django_tsp-3.14.8/src/django_tsp/management/commands/reciver.py
+-rw-r--r--   0 abb       (1000) abb       (1000)      132 2023-05-07 17:51:34.000000 django_tsp-3.14.8/src/django_tsp/routing.py
+-rw-r--r--   0 abb       (1000) abb       (1000)      212 2023-05-07 17:51:34.000000 django_tsp-3.14.8/src/django_tsp/serializers.py
+-rw-r--r--   0 abb       (1000) abb       (1000)      987 2023-05-08 14:44:07.000000 django_tsp-3.14.8/src/django_tsp/services.py
+drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-08 14:48:40.158819 django_tsp-3.14.8/src/django_tsp/templates/
+-rw-r--r--   0 abb       (1000) abb       (1000)     6005 2023-05-07 17:51:34.000000 django_tsp-3.14.8/src/django_tsp/templates/index.html
+-rw-r--r--   0 abb       (1000) abb       (1000)      102 2023-05-08 14:22:50.000000 django_tsp-3.14.8/src/django_tsp/views.py
+drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-05-08 14:48:40.155485 django_tsp-3.14.8/src/django_tsp.egg-info/
+-rw-r--r--   0 abb       (1000) abb       (1000)     3441 2023-05-08 14:48:39.000000 django_tsp-3.14.8/src/django_tsp.egg-info/PKG-INFO
+-rw-r--r--   0 abb       (1000) abb       (1000)      803 2023-05-08 14:48:40.000000 django_tsp-3.14.8/src/django_tsp.egg-info/SOURCES.txt
+-rw-r--r--   0 abb       (1000) abb       (1000)        1 2023-05-08 14:48:39.000000 django_tsp-3.14.8/src/django_tsp.egg-info/dependency_links.txt
+-rw-r--r--   0 abb       (1000) abb       (1000)        1 2023-04-28 13:56:46.000000 django_tsp-3.14.8/src/django_tsp.egg-info/not-zip-safe
+-rw-r--r--   0 abb       (1000) abb       (1000)       31 2023-05-08 14:48:40.000000 django_tsp-3.14.8/src/django_tsp.egg-info/requires.txt
+-rw-r--r--   0 abb       (1000) abb       (1000)       11 2023-05-08 14:48:40.000000 django_tsp-3.14.8/src/django_tsp.egg-info/top_level.txt
```

### Comparing `django_tsp-3.14.7/LICENSE` & `django_tsp-3.14.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django_tsp-3.14.7/setup.cfg` & `django_tsp-3.14.8/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = django_tsp
-version = 3.14.7
+version = 3.14.8
 description = django-tsp is a django travel salesman problem.
 long_description = file: README.md
-long_description_content_type = text/x-rst
+long_description_content_type = text/markdown
 url = https://github.com/TravelSalesmanProblem/django_tsp
 author = AmirBahador Bahadori
 author_email = amirbahador.pv@gmail.com
 maintainer = AmirBahador Bahadori
 maintainer_email = amirbahador.pv@gmail.com
 license = MIT
 license_file = LICENSE
```

### Comparing `django_tsp-3.14.7/src/django_tsp/apis.py` & `django_tsp-3.14.8/src/django_tsp/apis.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 from rest_framework import status, serializers
 from drf_spectacular.utils import extend_schema
 from .services import create_tsp_problem, publish_tsp_sloution
 from .serializers import LocationSerializer 
 
 
 class SolverApi(APIView):
+    """
+        Accept the tsp problem instance and 
+        broadcast question to websocket 
+    """
     class InputSolverSerializer(serializers.Serializer):
         locations = LocationSerializer(many=True)
         num_vehicles = serializers.FloatField(default=1)
         depot = serializers.FloatField(default=0)
 
     @extend_schema(request=InputSolverSerializer)
     def post(self, request):
@@ -24,14 +28,18 @@
             return Response(
                     f"Database Error {ex}",
                     status=status.HTTP_400_BAD_REQUEST
                     )
         return Response(status=status.HTTP_204_NO_CONTENT)
 
 class WebhookApi(APIView):
+    """
+        Recive the sloution response and notify websocket clients
+        TODO: make this endpoint private or using other portocol for handeling the sloution
+    """
     class InputSerializer(serializers.Serializer):
         locations = serializers.ListSerializer(child=serializers.CharField())
         id = serializers.CharField()
 
     @extend_schema(request=InputSerializer)
     def post(self, request):
         serializer = self.InputSerializer(data=request.data)
```

### Comparing `django_tsp-3.14.7/src/django_tsp/checks.py` & `django_tsp-3.14.8/src/django_tsp/checks.py`

 * *Files identical despite different names*

### Comparing `django_tsp-3.14.7/src/django_tsp/consumer.py` & `django_tsp-3.14.8/src/django_tsp/consumer.py`

 * *Files identical despite different names*

### Comparing `django_tsp-3.14.7/src/django_tsp/management/commands/__pycache__/bridge.cpython-310.pyc` & `django_tsp-3.14.8/src/django_tsp/management/commands/__pycache__/bridge.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tsp-3.14.7/src/django_tsp/management/commands/__pycache__/reciver.cpython-310.pyc` & `django_tsp-3.14.8/src/django_tsp/management/commands/__pycache__/reciver.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django_tsp-3.14.7/src/django_tsp/management/commands/reciver.py` & `django_tsp-3.14.8/src/django_tsp/management/commands/reciver.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from django.core.management.base import BaseCommand
-from tsp_wrapper import broker, setup, OUTBOUND_QUEUE
+from tsp_wrapper import broker, OUTBOUND_QUEUE
+from django_tsp.services import prepare_broker
 import requests
 from django_tsp.conf import conf
 
 
-def socket_tsp(res):
-    requests.post(conf.TSP_HOOK_URL, json = res)
-
 class Command(BaseCommand):
-    help = 'Show all available styles'
+    help = 'Consume the tsp sloution and bordcast it to the /ws/tsp socket'
 
     def handle(self, *args, **kwargs):
-        setup()
+        prepare_broker()
         self.stdout.write(self.style.SUCCESS('Starting the Reciver.'))
         worker = broker.Worker(connection=broker.get_broker(), handler=self.socket_tsp, type=OUTBOUND_QUEUE)
         worker.run()
 
     def socket_tsp(self, res):
+        """
+        our costume task for notifing the sloution to the web socket client
+        """
         response = requests.post(conf.TSP_HOOK_URL, json = res)
-        self.stdout.write(self.style.NOTICE(f'{response}'))
+        self.stdout.write(self.style.NOTICE(f'socket_tsp task response --> {response}'))
```

### Comparing `django_tsp-3.14.7/src/django_tsp/services.py` & `django_tsp-3.14.8/src/django_tsp/services.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from channels.layers import get_channel_layer
-from tsp_wrapper import broker, INBOUND_QUEUE
+from tsp_wrapper import broker, INBOUND_QUEUE, setup
 from asgiref.sync import async_to_sync
 import secrets 
+from kombu import Connection
+from django_tsp.conf import conf
 
 
 channel_layer = get_channel_layer()
 
 def notify_event(event:dict) -> None:
     """
     call sockets
@@ -15,10 +17,20 @@
 
 def publish_tsp_sloution(data):
     data["type"] = "answer"
     notify_event(data)
 
 def create_tsp_problem(data):
     data["type"] = "question"
-    data["id"] = secrets.token_hex(5)
+    data["id"] = secrets.token_hex(5)  # TODO: store the task ids 
     notify_event(data)
     broker.send_data(connection=broker.get_broker(), message=data, routing_key=INBOUND_QUEUE)
+
+
+def prepare_broker():
+    """
+        changing the broker url with settings.py variables
+        and connecting to the broker
+        and setting up the middlewares
+    """
+    broker.set_broker(Connection(conf.TSP_BROKER_URL))
+    setup()
```

### Comparing `django_tsp-3.14.7/src/django_tsp/templates/index.html` & `django_tsp-3.14.8/src/django_tsp/templates/index.html`

 * *Files identical despite different names*

### Comparing `django_tsp-3.14.7/src/django_tsp.egg-info/SOURCES.txt` & `django_tsp-3.14.8/src/django_tsp.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-CHANGELOG.rst
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 src/django_tsp/__init__.py
 src/django_tsp/apis.py
```

