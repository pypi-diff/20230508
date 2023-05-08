# Comparing `tmp/terka-1.7.2.1.tar.gz` & `tmp/terka-1.7.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terka-1.7.2.1.tar", last modified: Mon May  8 13:30:07 2023, max compression
+gzip compressed data, was "terka-1.7.2.2.tar", last modified: Mon May  8 13:55:04 2023, max compression
```

## Comparing `terka-1.7.2.1.tar` & `terka-1.7.2.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:30:07.546904 terka-1.7.2.1/
--rw-r--r--   0 am        (1000) am        (1000)      294 2023-05-08 13:30:07.546904 terka-1.7.2.1/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)       38 2023-05-08 13:30:07.546904 terka-1.7.2.1/setup.cfg
--rw-r--r--   0 am        (1000) am        (1000)      905 2023-05-08 13:30:00.000000 terka-1.7.2.1/setup.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:30:07.538904 terka-1.7.2.1/terka/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/__init__.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:30:07.542904 terka-1.7.2.1/terka/adapters/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/adapters/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    16361 2023-04-26 19:48:32.000000 terka-1.7.2.1/terka/adapters/orm.py
--rw-r--r--   0 am        (1000) am        (1000)     6150 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/adapters/repository.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:30:07.542904 terka-1.7.2.1/terka/domain/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/domain/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/domain/collaborators.py
--rw-r--r--   0 am        (1000) am        (1000)    44539 2023-05-08 13:29:04.000000 terka-1.7.2.1/terka/domain/commands.py
--rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/domain/commentary.py
--rw-r--r--   0 am        (1000) am        (1000)      102 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/domain/element.py
--rw-r--r--   0 am        (1000) am        (1000)     1513 2023-05-01 11:31:58.000000 terka-1.7.2.1/terka/domain/epic.py
--rw-r--r--   0 am        (1000) am        (1000)     1440 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/domain/event_history.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:30:07.542904 terka-1.7.2.1/terka/domain/external_connectors/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/domain/external_connectors/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      265 2023-04-26 19:49:46.000000 terka-1.7.2.1/terka/domain/external_connectors/asana.py
--rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.7.2.1/terka/domain/helpers.py
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/domain/project.py
--rw-r--r--   0 am        (1000) am        (1000)     2244 2023-05-03 16:06:42.000000 terka-1.7.2.1/terka/domain/sprint.py
--rw-r--r--   0 am        (1000) am        (1000)     1495 2023-05-01 11:32:09.000000 terka-1.7.2.1/terka/domain/story.py
--rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/domain/tag.py
--rw-r--r--   0 am        (1000) am        (1000)     2082 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/domain/task.py
--rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/domain/time_tracker.py
--rw-r--r--   0 am        (1000) am        (1000)      338 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/domain/user.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:30:07.542904 terka-1.7.2.1/terka/entrypoints/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/entrypoints/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)     6055 2023-04-30 19:45:41.000000 terka-1.7.2.1/terka/entrypoints/cli.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:30:07.546904 terka-1.7.2.1/terka/service_layer/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/service_layer/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    30533 2023-05-03 19:48:20.000000 terka-1.7.2.1/terka/service_layer/printer.py
--rw-r--r--   0 am        (1000) am        (1000)     2924 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/service_layer/services.py
--rw-r--r--   0 am        (1000) am        (1000)     3882 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/service_layer/ui.py
--rw-r--r--   0 am        (1000) am        (1000)      698 2023-04-26 19:47:22.000000 terka-1.7.2.1/terka/service_layer/vertical_layout.css
--rw-r--r--   0 am        (1000) am        (1000)     2382 2023-04-30 10:27:47.000000 terka-1.7.2.1/terka/service_layer/views.py
--rw-r--r--   0 am        (1000) am        (1000)     7907 2023-05-03 15:38:36.000000 terka-1.7.2.1/terka/utils.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:30:07.542904 terka-1.7.2.1/terka.egg-info/
--rw-r--r--   0 am        (1000) am        (1000)      294 2023-05-08 13:30:07.000000 terka-1.7.2.1/terka.egg-info/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      993 2023-05-08 13:30:07.000000 terka-1.7.2.1/terka.egg-info/SOURCES.txt
--rw-r--r--   0 am        (1000) am        (1000)        1 2023-05-08 13:30:07.000000 terka-1.7.2.1/terka.egg-info/dependency_links.txt
--rw-r--r--   0 am        (1000) am        (1000)       53 2023-05-08 13:30:07.000000 terka-1.7.2.1/terka.egg-info/entry_points.txt
--rw-r--r--   0 am        (1000) am        (1000)       52 2023-05-08 13:30:07.000000 terka-1.7.2.1/terka.egg-info/requires.txt
--rw-r--r--   0 am        (1000) am        (1000)        6 2023-05-08 13:30:07.000000 terka-1.7.2.1/terka.egg-info/top_level.txt
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:55:04.900599 terka-1.7.2.2/
+-rw-r--r--   0 am        (1000) am        (1000)      294 2023-05-08 13:55:04.896598 terka-1.7.2.2/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)       38 2023-05-08 13:55:04.900599 terka-1.7.2.2/setup.cfg
+-rw-r--r--   0 am        (1000) am        (1000)      905 2023-05-08 13:54:13.000000 terka-1.7.2.2/setup.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:55:04.896598 terka-1.7.2.2/terka/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/__init__.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:55:04.896598 terka-1.7.2.2/terka/adapters/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/adapters/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    16361 2023-04-26 19:48:32.000000 terka-1.7.2.2/terka/adapters/orm.py
+-rw-r--r--   0 am        (1000) am        (1000)     6150 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/adapters/repository.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:55:04.896598 terka-1.7.2.2/terka/domain/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/domain/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/domain/collaborators.py
+-rw-r--r--   0 am        (1000) am        (1000)    44918 2023-05-08 13:53:31.000000 terka-1.7.2.2/terka/domain/commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/domain/commentary.py
+-rw-r--r--   0 am        (1000) am        (1000)      102 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/domain/element.py
+-rw-r--r--   0 am        (1000) am        (1000)     1513 2023-05-01 11:31:58.000000 terka-1.7.2.2/terka/domain/epic.py
+-rw-r--r--   0 am        (1000) am        (1000)     1440 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/domain/event_history.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:55:04.896598 terka-1.7.2.2/terka/domain/external_connectors/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/domain/external_connectors/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      265 2023-04-26 19:49:46.000000 terka-1.7.2.2/terka/domain/external_connectors/asana.py
+-rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.7.2.2/terka/domain/helpers.py
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/domain/project.py
+-rw-r--r--   0 am        (1000) am        (1000)     2244 2023-05-03 16:06:42.000000 terka-1.7.2.2/terka/domain/sprint.py
+-rw-r--r--   0 am        (1000) am        (1000)     1495 2023-05-01 11:32:09.000000 terka-1.7.2.2/terka/domain/story.py
+-rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/domain/tag.py
+-rw-r--r--   0 am        (1000) am        (1000)     2082 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/domain/task.py
+-rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/domain/time_tracker.py
+-rw-r--r--   0 am        (1000) am        (1000)      338 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/domain/user.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:55:04.896598 terka-1.7.2.2/terka/entrypoints/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/entrypoints/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)     6055 2023-04-30 19:45:41.000000 terka-1.7.2.2/terka/entrypoints/cli.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:55:04.896598 terka-1.7.2.2/terka/service_layer/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/service_layer/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    30533 2023-05-03 19:48:20.000000 terka-1.7.2.2/terka/service_layer/printer.py
+-rw-r--r--   0 am        (1000) am        (1000)     2924 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/service_layer/services.py
+-rw-r--r--   0 am        (1000) am        (1000)     3882 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/service_layer/ui.py
+-rw-r--r--   0 am        (1000) am        (1000)      698 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/service_layer/vertical_layout.css
+-rw-r--r--   0 am        (1000) am        (1000)     2382 2023-04-30 10:27:47.000000 terka-1.7.2.2/terka/service_layer/views.py
+-rw-r--r--   0 am        (1000) am        (1000)     7907 2023-05-03 15:38:36.000000 terka-1.7.2.2/terka/utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:55:04.896598 terka-1.7.2.2/terka.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)      294 2023-05-08 13:55:04.000000 terka-1.7.2.2/terka.egg-info/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      993 2023-05-08 13:55:04.000000 terka-1.7.2.2/terka.egg-info/SOURCES.txt
+-rw-r--r--   0 am        (1000) am        (1000)        1 2023-05-08 13:55:04.000000 terka-1.7.2.2/terka.egg-info/dependency_links.txt
+-rw-r--r--   0 am        (1000) am        (1000)       53 2023-05-08 13:55:04.000000 terka-1.7.2.2/terka.egg-info/entry_points.txt
+-rw-r--r--   0 am        (1000) am        (1000)       52 2023-05-08 13:55:04.000000 terka-1.7.2.2/terka.egg-info/requires.txt
+-rw-r--r--   0 am        (1000) am        (1000)        6 2023-05-08 13:55:04.000000 terka-1.7.2.2/terka.egg-info/top_level.txt
```

### Comparing `terka-1.7.2.1/setup.py` & `terka-1.7.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 # README = (HERE.parent / "README.md").read_text()
 
 setup(
     name="terka",
-    version="1.7.2.1",
+    version="1.7.2.2",
     description="CLI utility for creating and managing tasks in a terminal",
     # long_description=README,
     long_description_content_type="text/markdown",
     author="Andrei Markin",
     author_email="andrey.markin.ppc@gmail.com",
     license="Apache 2.0",
     url="https://github.com/AndreyMarkinPPC/terka",
```

### Comparing `terka-1.7.2.1/terka/adapters/orm.py` & `terka-1.7.2.2/terka/adapters/orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.1/terka/adapters/repository.py` & `terka-1.7.2.2/terka/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.1/terka/domain/collaborators.py` & `terka-1.7.2.2/terka/domain/collaborators.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.1/terka/domain/commands.py` & `terka-1.7.2.2/terka/domain/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -427,65 +427,68 @@
                 yaml.dump(self.config, f)
             logger.info("<unfocus> %s: %s", entity_type, "")
         elif command == "count":
             entities = self.repo.list(entity, kwargs)
             print(len(entities))
             logger.info("<count> tasks")
         elif command == "collaborate":
+            if entity_type not in ("tasks", "projects"):
+                raise ValueError("You can collaborate only on tasks and projects")
             if entity_type == "tasks":
-                task_id = kwargs["id"]
-                existing_task = self.repo.list(Task, {"id": task_id})
-                if not existing_task:
-                    raise ValueError(f"Task with id {task_id} is not found!")
-                user = self.repo.list(User, {"name": kwargs["name"]})
-                if not user:
-                    user = User(**kwargs)
-                    self.repo.add(user)
-                    session.commit()
-                    user_id = user.id
-                else:
-                    user_id = user[0].id
-                existing_task_collaborator = self.repo.list(
-                    TaskCollaborator, {
-                        "task": task_id,
-                        "collaborator": user_id
-                    })
-                if not existing_task_collaborator:
-                    task_ids = get_ids(task_id)
-                    for task_id in task_ids:
-                        obj = TaskCollaborator(id=task_id,
-                                               collaborator_id=user_id)
-                        self.repo.add(obj)
-                    session.commit()
+                task_ids = get_ids(kwargs["id"])
+                for task_id in task_ids:
+                    existing_task = self.repo.list(Task, {"id": task_id})
+                    if not existing_task:
+                        raise ValueError(f"Task with id {task_id} is not found!")
+                    user = self.repo.list(User, {"name": kwargs["name"]})
+                    if not user:
+                        user = User(**kwargs)
+                        self.repo.add(user)
+                        session.commit()
+                        user_id = user.id
+                    else:
+                        user_id = user[0].id
+                    existing_task_collaborator = self.repo.list(
+                        TaskCollaborator, {
+                            "task": task_id,
+                            "collaborator": user_id
+                        })
+                    if not existing_task_collaborator:
+                        task_ids = get_ids(task_id)
+                        for task_id in task_ids:
+                            obj = TaskCollaborator(id=task_id,
+                                                   collaborator_id=user_id)
+                            self.repo.add(obj)
             elif entity_type == "projects":
-                project_id = kwargs["id"]
-                existing_project = self.repo.list(Project, {"id": project_id})
-                if not existing_project:
-                    raise ValueError(
-                        f"Project with id {project_id} is not found!")
-                user = self.repo.list(User, {"name": kwargs["name"]})
-                if not user:
-                    user = User(**kwargs)
-                    self.repo.add(user)
-                    session.commit()
-                    user_id = user.id
-                else:
-                    user_id = user[0].id
-                existing_project_collaborator = self.repo.list(
-                    ProjectCollaborator, {
-                        "project": project_id,
-                        "collaborator": user_id
-                    })
-                if not existing_project_collaborator:
-                    project_ids = get_ids(project_id)
-                    for project_id in project_ids:
-                        obj = ProjectCollaborator(id=project_id,
-                                                  collaborator_id=user_id)
-                        self.repo.add(obj)
+                project_ids = get_ids(kwargs["id"])
+                for project_id in project_ids:
+                    existing_project = self.repo.list(Project, {"id": project_id})
+                    if not existing_project:
+                        raise ValueError(
+                            f"Project with id {project_id} is not found!")
+                    user = self.repo.list(User, {"name": kwargs["name"]})
+                    if not user:
+                        user = User(**kwargs)
+                        self.repo.add(user)
                         session.commit()
+                        user_id = user.id
+                    else:
+                        user_id = user[0].id
+                    existing_project_collaborator = self.repo.list(
+                        ProjectCollaborator, {
+                            "project": project_id,
+                            "collaborator": user_id
+                        })
+                    if not existing_project_collaborator:
+                        project_ids = get_ids(project_id)
+                        for project_id in project_ids:
+                            obj = ProjectCollaborator(id=project_id,
+                                                      collaborator_id=user_id)
+                            self.repo.add(obj)
+            session.commit()
         elif command == "tag":
             if entity_type == "tasks":
                 task_id = kwargs["id"]
                 existing_task = self.repo.list(Task, {"id": task_id})
                 if not existing_task:
                     raise ValueError(f"Task with id {task_id} is not found!")
                 tag_text = kwargs.get("text") or kwargs.get("tags")
```

### Comparing `terka-1.7.2.1/terka/domain/commentary.py` & `terka-1.7.2.2/terka/domain/commentary.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.1/terka/domain/epic.py` & `terka-1.7.2.2/terka/domain/epic.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.1/terka/domain/event_history.py` & `terka-1.7.2.2/terka/domain/event_history.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.1/terka/domain/project.py` & `terka-1.7.2.2/terka/domain/project.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.1/terka/domain/sprint.py` & `terka-1.7.2.2/terka/domain/sprint.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.1/terka/domain/story.py` & `terka-1.7.2.2/terka/domain/story.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.1/terka/domain/tag.py` & `terka-1.7.2.2/terka/domain/tag.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.1/terka/domain/task.py` & `terka-1.7.2.2/terka/domain/task.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.1/terka/domain/time_tracker.py` & `terka-1.7.2.2/terka/domain/time_tracker.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.1/terka/entrypoints/cli.py` & `terka-1.7.2.2/terka/entrypoints/cli.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.1/terka/service_layer/printer.py` & `terka-1.7.2.2/terka/service_layer/printer.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.1/terka/service_layer/services.py` & `terka-1.7.2.2/terka/service_layer/services.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.1/terka/service_layer/ui.py` & `terka-1.7.2.2/terka/service_layer/ui.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.1/terka/service_layer/vertical_layout.css` & `terka-1.7.2.2/terka/service_layer/vertical_layout.css`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.1/terka/service_layer/views.py` & `terka-1.7.2.2/terka/service_layer/views.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.1/terka/utils.py` & `terka-1.7.2.2/terka/utils.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.1/terka.egg-info/SOURCES.txt` & `terka-1.7.2.2/terka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

