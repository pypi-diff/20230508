# Comparing `tmp/terka-1.7.2.tar.gz` & `tmp/terka-1.7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terka-1.7.2.tar", last modified: Wed May  3 19:51:38 2023, max compression
+gzip compressed data, was "terka-1.7.2.1.tar", last modified: Mon May  8 13:30:07 2023, max compression
```

## Comparing `terka-1.7.2.tar` & `terka-1.7.2.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-03 19:51:38.947424 terka-1.7.2/
--rw-r--r--   0 am        (1000) am        (1000)      292 2023-05-03 19:51:38.947424 terka-1.7.2/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)       38 2023-05-03 19:51:38.947424 terka-1.7.2/setup.cfg
--rw-r--r--   0 am        (1000) am        (1000)      903 2023-05-03 15:07:59.000000 terka-1.7.2/setup.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-03 19:51:38.943424 terka-1.7.2/terka/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2/terka/__init__.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-03 19:51:38.943424 terka-1.7.2/terka/adapters/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2/terka/adapters/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    16361 2023-04-26 19:48:32.000000 terka-1.7.2/terka/adapters/orm.py
--rw-r--r--   0 am        (1000) am        (1000)     6150 2023-04-26 19:47:22.000000 terka-1.7.2/terka/adapters/repository.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-03 19:51:38.947424 terka-1.7.2/terka/domain/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2/terka/domain/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-26 19:47:22.000000 terka-1.7.2/terka/domain/collaborators.py
--rw-r--r--   0 am        (1000) am        (1000)    44610 2023-05-03 19:48:27.000000 terka-1.7.2/terka/domain/commands.py
--rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-26 19:47:22.000000 terka-1.7.2/terka/domain/commentary.py
--rw-r--r--   0 am        (1000) am        (1000)      102 2023-04-26 19:47:22.000000 terka-1.7.2/terka/domain/element.py
--rw-r--r--   0 am        (1000) am        (1000)     1513 2023-05-01 11:31:58.000000 terka-1.7.2/terka/domain/epic.py
--rw-r--r--   0 am        (1000) am        (1000)     1440 2023-04-26 19:47:22.000000 terka-1.7.2/terka/domain/event_history.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-03 19:51:38.947424 terka-1.7.2/terka/domain/external_connectors/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2/terka/domain/external_connectors/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      265 2023-04-26 19:49:46.000000 terka-1.7.2/terka/domain/external_connectors/asana.py
--rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.7.2/terka/domain/helpers.py
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-04-26 19:47:22.000000 terka-1.7.2/terka/domain/project.py
--rw-r--r--   0 am        (1000) am        (1000)     2244 2023-05-03 16:06:42.000000 terka-1.7.2/terka/domain/sprint.py
--rw-r--r--   0 am        (1000) am        (1000)     1495 2023-05-01 11:32:09.000000 terka-1.7.2/terka/domain/story.py
--rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-26 19:47:22.000000 terka-1.7.2/terka/domain/tag.py
--rw-r--r--   0 am        (1000) am        (1000)     2082 2023-04-26 19:47:22.000000 terka-1.7.2/terka/domain/task.py
--rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-26 19:47:22.000000 terka-1.7.2/terka/domain/time_tracker.py
--rw-r--r--   0 am        (1000) am        (1000)      338 2023-04-26 19:47:22.000000 terka-1.7.2/terka/domain/user.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-03 19:51:38.947424 terka-1.7.2/terka/entrypoints/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2/terka/entrypoints/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)     6055 2023-04-30 19:45:41.000000 terka-1.7.2/terka/entrypoints/cli.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-03 19:51:38.947424 terka-1.7.2/terka/service_layer/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2/terka/service_layer/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    30533 2023-05-03 19:48:20.000000 terka-1.7.2/terka/service_layer/printer.py
--rw-r--r--   0 am        (1000) am        (1000)     2924 2023-04-26 19:47:22.000000 terka-1.7.2/terka/service_layer/services.py
--rw-r--r--   0 am        (1000) am        (1000)     3882 2023-04-26 19:47:22.000000 terka-1.7.2/terka/service_layer/ui.py
--rw-r--r--   0 am        (1000) am        (1000)      698 2023-04-26 19:47:22.000000 terka-1.7.2/terka/service_layer/vertical_layout.css
--rw-r--r--   0 am        (1000) am        (1000)     2382 2023-04-30 10:27:47.000000 terka-1.7.2/terka/service_layer/views.py
--rw-r--r--   0 am        (1000) am        (1000)     7907 2023-05-03 15:38:36.000000 terka-1.7.2/terka/utils.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-03 19:51:38.943424 terka-1.7.2/terka.egg-info/
--rw-r--r--   0 am        (1000) am        (1000)      292 2023-05-03 19:51:38.000000 terka-1.7.2/terka.egg-info/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      993 2023-05-03 19:51:38.000000 terka-1.7.2/terka.egg-info/SOURCES.txt
--rw-r--r--   0 am        (1000) am        (1000)        1 2023-05-03 19:51:38.000000 terka-1.7.2/terka.egg-info/dependency_links.txt
--rw-r--r--   0 am        (1000) am        (1000)       53 2023-05-03 19:51:38.000000 terka-1.7.2/terka.egg-info/entry_points.txt
--rw-r--r--   0 am        (1000) am        (1000)       52 2023-05-03 19:51:38.000000 terka-1.7.2/terka.egg-info/requires.txt
--rw-r--r--   0 am        (1000) am        (1000)        6 2023-05-03 19:51:38.000000 terka-1.7.2/terka.egg-info/top_level.txt
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:30:07.546904 terka-1.7.2.1/
+-rw-r--r--   0 am        (1000) am        (1000)      294 2023-05-08 13:30:07.546904 terka-1.7.2.1/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)       38 2023-05-08 13:30:07.546904 terka-1.7.2.1/setup.cfg
+-rw-r--r--   0 am        (1000) am        (1000)      905 2023-05-08 13:30:00.000000 terka-1.7.2.1/setup.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:30:07.538904 terka-1.7.2.1/terka/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/__init__.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:30:07.542904 terka-1.7.2.1/terka/adapters/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/adapters/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    16361 2023-04-26 19:48:32.000000 terka-1.7.2.1/terka/adapters/orm.py
+-rw-r--r--   0 am        (1000) am        (1000)     6150 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/adapters/repository.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:30:07.542904 terka-1.7.2.1/terka/domain/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/domain/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/domain/collaborators.py
+-rw-r--r--   0 am        (1000) am        (1000)    44539 2023-05-08 13:29:04.000000 terka-1.7.2.1/terka/domain/commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/domain/commentary.py
+-rw-r--r--   0 am        (1000) am        (1000)      102 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/domain/element.py
+-rw-r--r--   0 am        (1000) am        (1000)     1513 2023-05-01 11:31:58.000000 terka-1.7.2.1/terka/domain/epic.py
+-rw-r--r--   0 am        (1000) am        (1000)     1440 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/domain/event_history.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:30:07.542904 terka-1.7.2.1/terka/domain/external_connectors/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/domain/external_connectors/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      265 2023-04-26 19:49:46.000000 terka-1.7.2.1/terka/domain/external_connectors/asana.py
+-rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.7.2.1/terka/domain/helpers.py
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/domain/project.py
+-rw-r--r--   0 am        (1000) am        (1000)     2244 2023-05-03 16:06:42.000000 terka-1.7.2.1/terka/domain/sprint.py
+-rw-r--r--   0 am        (1000) am        (1000)     1495 2023-05-01 11:32:09.000000 terka-1.7.2.1/terka/domain/story.py
+-rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/domain/tag.py
+-rw-r--r--   0 am        (1000) am        (1000)     2082 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/domain/task.py
+-rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/domain/time_tracker.py
+-rw-r--r--   0 am        (1000) am        (1000)      338 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/domain/user.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:30:07.542904 terka-1.7.2.1/terka/entrypoints/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/entrypoints/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)     6055 2023-04-30 19:45:41.000000 terka-1.7.2.1/terka/entrypoints/cli.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:30:07.546904 terka-1.7.2.1/terka/service_layer/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/service_layer/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    30533 2023-05-03 19:48:20.000000 terka-1.7.2.1/terka/service_layer/printer.py
+-rw-r--r--   0 am        (1000) am        (1000)     2924 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/service_layer/services.py
+-rw-r--r--   0 am        (1000) am        (1000)     3882 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/service_layer/ui.py
+-rw-r--r--   0 am        (1000) am        (1000)      698 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/service_layer/vertical_layout.css
+-rw-r--r--   0 am        (1000) am        (1000)     2382 2023-04-30 10:27:47.000000 terka-1.7.2.1/terka/service_layer/views.py
+-rw-r--r--   0 am        (1000) am        (1000)     7907 2023-05-03 15:38:36.000000 terka-1.7.2.1/terka/utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:30:07.542904 terka-1.7.2.1/terka.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)      294 2023-05-08 13:30:07.000000 terka-1.7.2.1/terka.egg-info/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      993 2023-05-08 13:30:07.000000 terka-1.7.2.1/terka.egg-info/SOURCES.txt
+-rw-r--r--   0 am        (1000) am        (1000)        1 2023-05-08 13:30:07.000000 terka-1.7.2.1/terka.egg-info/dependency_links.txt
+-rw-r--r--   0 am        (1000) am        (1000)       53 2023-05-08 13:30:07.000000 terka-1.7.2.1/terka.egg-info/entry_points.txt
+-rw-r--r--   0 am        (1000) am        (1000)       52 2023-05-08 13:30:07.000000 terka-1.7.2.1/terka.egg-info/requires.txt
+-rw-r--r--   0 am        (1000) am        (1000)        6 2023-05-08 13:30:07.000000 terka-1.7.2.1/terka.egg-info/top_level.txt
```

### Comparing `terka-1.7.2/setup.py` & `terka-1.7.2.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 # README = (HERE.parent / "README.md").read_text()
 
 setup(
     name="terka",
-    version="1.7.2",
+    version="1.7.2.1",
     description="CLI utility for creating and managing tasks in a terminal",
     # long_description=README,
     long_description_content_type="text/markdown",
     author="Andrei Markin",
     author_email="andrey.markin.ppc@gmail.com",
     license="Apache 2.0",
     url="https://github.com/AndreyMarkinPPC/terka",
```

### Comparing `terka-1.7.2/terka/adapters/orm.py` & `terka-1.7.2.1/terka/adapters/orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2/terka/adapters/repository.py` & `terka-1.7.2.1/terka/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2/terka/domain/collaborators.py` & `terka-1.7.2.1/terka/domain/collaborators.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2/terka/domain/commands.py` & `terka-1.7.2.1/terka/domain/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -716,22 +716,21 @@
                     else:
                         for entity_task in added_task.tasks:
                             if entity_task.tasks.status.name not in (
                                     "DONE", "DELETED"):
                                 self._add_task_to_sprint(
                                     entity_task.tasks, sprint)
                 if story_points := kwargs.get("story_points"):
-                    if not sprint_task_id:
-                        sprint_task = self.execute("get", "sprint_tasks",
-                                                   {"task": task_id})
-                        if not sprint_task:
-                            exit(
-                                f"Task id {task_id} is not part of any sprint")
-                        else:
-                            sprint_task_id = sprint_task[0].id
+                    sprint_task = self.execute("get", "sprint_tasks",
+                                               {"task": task_id})
+                    if not sprint_task:
+                        exit(
+                            f"Task id {task_id} is not part of any sprint")
+                    else:
+                        sprint_task_id = sprint_task[0].id
                     self.repo.update(SprintTask, sprint_task_id,
                                      {"story_points": story_points})
             session.commit()
         elif command == "create":
             kwargs["created_by"] = services.lookup_user_id(
                 self.config.get("user"), self.repo)
             obj = entity(**kwargs)
```

### Comparing `terka-1.7.2/terka/domain/commentary.py` & `terka-1.7.2.1/terka/domain/commentary.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2/terka/domain/epic.py` & `terka-1.7.2.1/terka/domain/epic.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2/terka/domain/event_history.py` & `terka-1.7.2.1/terka/domain/event_history.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2/terka/domain/project.py` & `terka-1.7.2.1/terka/domain/project.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2/terka/domain/sprint.py` & `terka-1.7.2.1/terka/domain/sprint.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2/terka/domain/story.py` & `terka-1.7.2.1/terka/domain/story.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2/terka/domain/tag.py` & `terka-1.7.2.1/terka/domain/tag.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2/terka/domain/task.py` & `terka-1.7.2.1/terka/domain/task.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2/terka/domain/time_tracker.py` & `terka-1.7.2.1/terka/domain/time_tracker.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2/terka/entrypoints/cli.py` & `terka-1.7.2.1/terka/entrypoints/cli.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2/terka/service_layer/printer.py` & `terka-1.7.2.1/terka/service_layer/printer.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2/terka/service_layer/services.py` & `terka-1.7.2.1/terka/service_layer/services.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2/terka/service_layer/ui.py` & `terka-1.7.2.1/terka/service_layer/ui.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2/terka/service_layer/vertical_layout.css` & `terka-1.7.2.1/terka/service_layer/vertical_layout.css`

 * *Files identical despite different names*

### Comparing `terka-1.7.2/terka/service_layer/views.py` & `terka-1.7.2.1/terka/service_layer/views.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2/terka/utils.py` & `terka-1.7.2.1/terka/utils.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2/terka.egg-info/SOURCES.txt` & `terka-1.7.2.1/terka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

