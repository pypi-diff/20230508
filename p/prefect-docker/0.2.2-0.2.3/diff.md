# Comparing `tmp/prefect-docker-0.2.2.tar.gz` & `tmp/prefect-docker-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-docker/prefect-docker/dist/.tmp-2imrtbfp/prefect-docker-0.2.2.tar", last modified: Fri Apr 21 00:04:48 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-docker/prefect-docker/dist/.tmp-es7vqrnd/prefect-docker-0.2.3.tar", last modified: Mon May  8 17:53:45 2023, max compression
```

## Comparing `prefect-docker-0.2.2.tar` & `prefect-docker-0.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/prefect_docker/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/prefect_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/prefect_docker/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/prefect_docker/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/prefect_docker/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/prefect_docker/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/prefect_docker/images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/prefect_docker/projects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/prefect_docker/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/prefect_docker/projects/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    26399 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/prefect_docker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/prefect_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/prefect_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/prefect_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/prefect_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/prefect_docker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/prefect_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/prefect_docker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:04:48.000000 prefect-docker-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/tests/test_host.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (123)    41841 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-21 00:03:27.000000 prefect-docker-0.2.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/prefect_docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/prefect_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/prefect_docker/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/prefect_docker/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/prefect_docker/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/prefect_docker/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/prefect_docker/images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/prefect_docker/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/prefect_docker/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/prefect_docker/projects/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28174 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/prefect_docker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/prefect_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/prefect_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/prefect_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/prefect_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/prefect_docker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/prefect_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/prefect_docker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:53:45.000000 prefect-docker-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/tests/test_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44087 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-05-08 17:52:21.000000 prefect-docker-0.2.3/versioneer.py
```

### Comparing `prefect-docker-0.2.2/LICENSE` & `prefect-docker-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.2/PKG-INFO` & `prefect-docker-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-docker
-Version: 0.2.2
+Version: 0.2.3
 Summary: Prefect integrations for working with Docker
 Home-page: https://github.com/PrefectHQ/prefect-docker
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-docker-0.2.2/README.md` & `prefect-docker-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.2/prefect_docker/containers.py` & `prefect-docker-0.2.3/prefect_docker/containers.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.2/prefect_docker/credentials.py` & `prefect-docker-0.2.3/prefect_docker/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.2/prefect_docker/host.py` & `prefect-docker-0.2.3/prefect_docker/host.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.2/prefect_docker/images.py` & `prefect-docker-0.2.3/prefect_docker/images.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.2/prefect_docker/projects/steps.py` & `prefect-docker-0.2.3/prefect_docker/projects/steps.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.2/prefect_docker/worker.py` & `prefect-docker-0.2.3/prefect_docker/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from prefect.client.orchestration import ServerType, get_client
 from prefect.client.schemas import FlowRun
 from prefect.docker import (
     format_outlier_version_name,
     get_prefect_image_name,
     parse_image_tag,
 )
+from prefect.events import Event, RelatedResource, emit_event
 from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
 from prefect.server.schemas.core import Flow
 from prefect.server.schemas.responses import DeploymentResponse
 from prefect.settings import PREFECT_API_URL
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
 from prefect.workers.base import BaseJobConfiguration, BaseWorker, BaseWorkerResult
 from pydantic import Field, validator
@@ -389,26 +390,26 @@
     ) -> BaseWorkerResult:
         """
         Executes a flow run within a Docker container and waits for the flow run
         to complete.
         """
         # The `docker` library uses requests instead of an async http library so it must
         # be run in a thread to avoid blocking the event loop.
-        container = await run_sync_in_worker_thread(
+        container, created_event = await run_sync_in_worker_thread(
             self._create_and_start_container, configuration
         )
         container_pid = self._get_infrastructure_pid(container_id=container.id)
 
         # Mark as started and return the infrastructure id
         if task_status:
             task_status.started(container_pid)
 
         # Monitor the container
         container = await run_sync_in_worker_thread(
-            self._watch_container_safe, container, configuration
+            self._watch_container_safe, container, configuration, created_event
         )
 
         exit_code = container.attrs["State"].get("ExitCode")
         return DockerWorkerResult(
             status_code=exit_code if exit_code is not None else -1,
             identifier=container_pid,
         )
@@ -518,54 +519,69 @@
             mem_limit=configuration.mem_limit,
             memswap_limit=configuration.memswap_limit,
             privileged=configuration.privileged,
         )
 
     def _create_and_start_container(
         self, configuration: DockerWorkerJobConfiguration
-    ) -> "Container":
+    ) -> Tuple["Container", Event]:
         """Creates and starts a Docker container."""
         docker_client = self._get_client()
         container_settings = self._build_container_settings(
             docker_client, configuration
         )
 
         if self._should_pull_image(docker_client, configuration=configuration):
             self._logger.info(f"Pulling image {configuration.image!r}...")
             self._pull_image(docker_client, configuration)
 
         container = self._create_container(docker_client, **container_settings)
 
+        created_event = self._emit_container_status_change_event(
+            container, configuration
+        )
+
         # Add additional networks after the container is created; only one network can
         # be attached at creation time
         if len(configuration.networks) > 1:
             for network_name in configuration.networks[1:]:
                 network = docker_client.networks.get(network_name)
                 network.connect(container)
 
         # Start the container
         container.start()
 
         docker_client.close()
 
-        return container
+        return container, created_event
 
     def _watch_container_safe(
-        self, container: "Container", configuration: DockerWorkerJobConfiguration
+        self,
+        container: "Container",
+        configuration: DockerWorkerJobConfiguration,
+        created_event: Event,
     ) -> "Container":
         """Watches a container for completion, handling any errors that may occur."""
         # Monitor the container capturing the latest snapshot while capturing
         # not found errors
         docker_client = self._get_client()
 
         try:
+            seen_statuses = {container.status}
+            last_event = created_event
             for latest_container in self._watch_container(
                 docker_client, container.id, configuration
             ):
                 container = latest_container
+                if container.status not in seen_statuses:
+                    seen_statuses.add(container.status)
+                    last_event = self._emit_container_status_change_event(
+                        container, configuration, last_event=last_event
+                    )
+
         except docker.errors.NotFound:
             # The container was removed during watching
             self._logger.warning(
                 f"Docker container {container.name} was removed before we could wait "
                 "for its completion."
             )
         finally:
@@ -686,7 +702,36 @@
                 else:
                     raise
 
         self._logger.info(
             f"Docker container {container.name!r} has status {container.status!r}"
         )
         return container
+
+    def _container_as_resource(self, container: "Container") -> Dict[str, str]:
+        """Convert a container to a resource dictionary"""
+        return {
+            "prefect.resource.id": f"prefect.docker.container.{container.id}",
+            "prefect.resource.name": container.name,
+        }
+
+    def _emit_container_status_change_event(
+        self,
+        container: "Container",
+        configuration: DockerWorkerJobConfiguration,
+        last_event: Optional[Event] = None,
+    ) -> Event:
+        """Emit a Prefect event for a Docker container event."""
+        resource = self._container_as_resource(container)
+
+        related = self._event_related_resources(configuration=configuration)
+
+        worker_resource = self._event_resource()
+        worker_resource["prefect.resource.role"] = "worker"
+        worker_related_resource = RelatedResource(__root__=worker_resource)
+
+        return emit_event(
+            event=f"prefect.docker.container.{container.status.lower()}",
+            resource=resource,
+            related=related + [worker_related_resource],
+            follows=last_event,
+        )
```

### Comparing `prefect-docker-0.2.2/prefect_docker.egg-info/PKG-INFO` & `prefect-docker-0.2.3/prefect_docker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-docker
-Version: 0.2.2
+Version: 0.2.3
 Summary: Prefect integrations for working with Docker
 Home-page: https://github.com/PrefectHQ/prefect-docker
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-docker-0.2.2/prefect_docker.egg-info/SOURCES.txt` & `prefect-docker-0.2.3/prefect_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.2/setup.cfg` & `prefect-docker-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.2/setup.py` & `prefect-docker-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.2/tests/test_containers.py` & `prefect-docker-0.2.3/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.2/tests/test_host.py` & `prefect-docker-0.2.3/tests/test_host.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.2/tests/test_images.py` & `prefect-docker-0.2.3/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.2.2/tests/test_worker.py` & `prefect-docker-0.2.3/tests/test_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+import copy
 import re
 import uuid
-from unittest.mock import MagicMock
+from unittest.mock import MagicMock, call, patch
 
 import anyio.abc
 import docker
 import docker.errors
 import docker.models.containers
 import pytest
 from docker import DockerClient
 from docker.models.containers import Container
 from prefect.client.schemas import FlowRun
 from prefect.docker import get_prefect_image_name
+from prefect.events import RelatedResource
 from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
 from prefect.settings import (
     PREFECT_EXPERIMENTAL_ENABLE_WORKERS,
     PREFECT_EXPERIMENTAL_WARN_WORKERS,
     get_current_settings,
     temporary_settings,
 )
@@ -45,22 +47,23 @@
 
 @pytest.fixture
 def mock_docker_client(monkeypatch):
     mock = MagicMock(name="DockerClient", spec=docker.DockerClient)
     mock.version.return_value = {"Version": "20.10"}
 
     # Build a fake container object to return
+
     fake_container = docker.models.containers.Container()
     fake_container.client = MagicMock(name="Container.client")
     fake_container.collection = MagicMock(name="Container.collection")
     attrs = {
         "Id": FAKE_CONTAINER_ID,
         "Name": "fake-name",
         "State": {
-            "Status": "exited",
+            "Status": "running",
             "Running": False,
             "Paused": False,
             "Restarting": False,
             "OOMKilled": False,
             "Dead": True,
             "Pid": 0,
             "ExitCode": 0,
@@ -68,17 +71,27 @@
             "StartedAt": "2022-08-31T18:01:32.645851548Z",
             "FinishedAt": "2022-08-31T18:01:32.657076632Z",
         },
     }
     fake_container.collection.get().attrs = attrs
     fake_container.attrs = attrs
     fake_container.stop = MagicMock()
+
+    def fake_reload():
+        nonlocal fake_container
+        fake_container.attrs["State"]["Status"] = "exited"
+
+    fake_container.reload = MagicMock(side_effect=fake_reload)
+
+    created_container = copy.deepcopy(fake_container)
+    created_container.attrs["State"]["Status"] = "created"
+
     # Return the fake container on lookups and creation
     mock.containers.get.return_value = fake_container
-    mock.containers.create.return_value = fake_container
+    mock.containers.create.return_value = created_container
 
     # Set attributes for infrastructure PID lookup
     fake_api = MagicMock(name="APIClient")
     fake_api.base_url = FAKE_BASE_URL
     mock.api = fake_api
 
     monkeypatch.setattr("docker.from_env", MagicMock(return_value=mock))
@@ -158,15 +171,17 @@
         existing_names = []
 
     def fail_if_name_exists(*args, **kwargs):
         if kwargs.get("name") in existing_names:
             raise docker.errors.APIError(
                 "Conflict. The container name 'foobar' is already in use"
             )
-        return MagicMock()  # A container
+        container = MagicMock()
+        container.name = kwargs.get("name")
+        return container
 
     mock_docker_client.containers.create.side_effect = fail_if_name_exists
 
     default_docker_worker_job_configuration.name = "test-name"
     default_docker_worker_job_configuration.prepare_for_flow_run(flow_run)
     async with DockerWorker(work_pool_name="test") as worker:
         await worker.run(
@@ -1083,7 +1098,61 @@
     ):
         async with DockerWorker(work_pool_name="test") as worker:
             await worker.kill_infrastructure(
                 infrastructure_pid=f"{FAKE_BASE_URL}:{BAD_CONTAINER_ID}",
                 configuration=default_docker_worker_job_configuration,
                 grace_seconds=0,
             )
+
+
+async def test_emits_events(
+    mock_docker_client, flow_run, default_docker_worker_job_configuration
+):
+
+    event_count = 0
+
+    def event(*args, **kwargs):
+        nonlocal event_count
+        event_count += 1
+        return event_count
+
+    with patch("prefect_docker.worker.emit_event", side_effect=event) as mock_emit:
+        async with DockerWorker(work_pool_name="test") as worker:
+            await worker.run(
+                flow_run=flow_run, configuration=default_docker_worker_job_configuration
+            )
+
+    worker_resource = worker._event_resource()
+    worker_resource["prefect.resource.role"] = "worker"
+    worker_related_resource = RelatedResource(__root__=worker_resource)
+
+    mock_emit.assert_has_calls(
+        [
+            call(
+                event="prefect.docker.container.created",
+                resource={
+                    "prefect.resource.id": "prefect.docker.container.fake-id",
+                    "prefect.resource.name": "fake-name",
+                },
+                related=[worker_related_resource],
+                follows=None,
+            ),
+            call(
+                event="prefect.docker.container.running",
+                resource={
+                    "prefect.resource.id": "prefect.docker.container.fake-id",
+                    "prefect.resource.name": "fake-name",
+                },
+                related=[worker_related_resource],
+                follows=1,
+            ),
+            call(
+                event="prefect.docker.container.exited",
+                resource={
+                    "prefect.resource.id": "prefect.docker.container.fake-id",
+                    "prefect.resource.name": "fake-name",
+                },
+                related=[worker_related_resource],
+                follows=2,
+            ),
+        ]
+    )
```

### Comparing `prefect-docker-0.2.2/versioneer.py` & `prefect-docker-0.2.3/versioneer.py`

 * *Files identical despite different names*

