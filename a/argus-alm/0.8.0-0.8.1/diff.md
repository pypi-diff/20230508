# Comparing `tmp/argus-alm-0.8.0.tar.gz` & `tmp/argus-alm-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argus-alm-0.8.0.tar", max compression
+gzip compressed data, was "argus-alm-0.8.1.tar", max compression
```

## Comparing `argus-alm-0.8.0.tar` & `argus-alm-0.8.1.tar`

### file list

```diff
@@ -1,34 +1,60 @@
--rw-r--r--   0        0        0    11357 2021-09-26 18:50:58.000000 argus-alm-0.8.0/LICENSE
--rw-r--r--   0        0        0     3980 2022-05-27 12:21:06.789497 argus-alm-0.8.0/README.md
--rw-r--r--   0        0        0        0 2021-09-15 07:58:01.000000 argus-alm-0.8.0/argus/__init__.py
--rw-r--r--   0        0        0        0 2021-09-26 18:50:58.000000 argus-alm-0.8.0/argus/backend/.gitkeep
--rw-r--r--   0        0        0        0 2022-05-27 12:21:06.789497 argus-alm-0.8.0/argus/backend/__init__.py
--rw-r--r--   0        0        0     6808 2022-05-27 12:21:06.789497 argus-alm-0.8.0/argus/backend/build_system_monitor.py
--rw-r--r--   0        0        0        0 2022-05-27 12:21:06.789497 argus-alm-0.8.0/argus/backend/controller/__init__.py
--rw-r--r--   0        0        0      856 2022-05-27 12:21:06.789497 argus-alm-0.8.0/argus/backend/controller/admin.py
--rw-r--r--   0        0        0     9753 2022-05-27 12:21:06.789497 argus-alm-0.8.0/argus/backend/controller/admin_api.py
--rw-r--r--   0        0        0    28344 2022-06-20 08:35:36.973586 argus-alm-0.8.0/argus/backend/controller/api.py
--rw-r--r--   0        0        0     3010 2022-05-27 12:21:06.789497 argus-alm-0.8.0/argus/backend/controller/auth.py
--rw-r--r--   0        0        0     8137 2022-06-05 11:27:37.110413 argus-alm-0.8.0/argus/backend/controller/main.py
--rw-r--r--   0        0        0     3332 2022-05-27 12:21:06.789497 argus-alm-0.8.0/argus/backend/controller/notification_api.py
--rw-r--r--   0        0        0      324 2022-05-27 12:21:06.789497 argus-alm-0.8.0/argus/backend/controller/notifications.py
--rw-r--r--   0        0        0     4511 2022-06-12 15:33:09.057315 argus-alm-0.8.0/argus/backend/db.py
--rw-r--r--   0        0        0     1179 2022-05-27 12:21:06.789497 argus-alm-0.8.0/argus/backend/event_processors.py
--rw-r--r--   0        0        0     2280 2022-05-27 12:21:06.789497 argus-alm-0.8.0/argus/backend/logsetup.py
--rw-r--r--   0        0        0      675 2022-05-27 12:21:06.789497 argus-alm-0.8.0/argus/backend/service/admin.py
--rw-r--r--   0        0        0    49667 2022-06-20 08:35:36.974586 argus-alm-0.8.0/argus/backend/service/argus_service.py
--rw-r--r--   0        0        0     3800 2022-05-27 12:21:06.790497 argus-alm-0.8.0/argus/backend/service/notification_manager.py
--rw-r--r--   0        0        0     6332 2022-05-27 12:21:06.790497 argus-alm-0.8.0/argus/backend/service/release_manager.py
--rw-r--r--   0        0        0     8530 2022-06-20 08:35:36.975586 argus-alm-0.8.0/argus/backend/service/stats.py
--rw-r--r--   0        0        0        0 2021-09-26 18:50:58.000000 argus-alm-0.8.0/argus/db/.gitkeep
--rw-r--r--   0        0        0      391 2022-05-27 12:21:06.790497 argus-alm-0.8.0/argus/db/argus_json.py
--rw-r--r--   0        0        0     3702 2022-02-10 08:32:30.049072 argus-alm-0.8.0/argus/db/cloud_types.py
--rw-r--r--   0        0        0     3125 2022-05-31 10:04:33.709865 argus-alm-0.8.0/argus/db/config.py
--rw-r--r--   0        0        0     3612 2022-06-02 12:42:55.427721 argus-alm-0.8.0/argus/db/db_types.py
--rw-r--r--   0        0        0    16654 2022-05-27 12:21:06.790497 argus-alm-0.8.0/argus/db/interface.py
--rw-r--r--   0        0        0    11678 2022-06-02 12:42:55.428721 argus-alm-0.8.0/argus/db/models.py
--rw-r--r--   0        0        0    26069 2022-06-20 08:35:36.975586 argus-alm-0.8.0/argus/db/testrun.py
--rw-r--r--   0        0        0      337 2021-10-03 12:19:16.000000 argus-alm-0.8.0/argus/db/utils.py
--rw-r--r--   0        0        0     1011 2022-06-20 08:36:53.320134 argus-alm-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4918 1970-01-01 00:00:00.000000 argus-alm-0.8.0/setup.py
--rw-r--r--   0        0        0     4601 1970-01-01 00:00:00.000000 argus-alm-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-09-26 18:50:58.000000 argus-alm-0.8.1/LICENSE
+-rw-r--r--   0        0        0     6236 2022-09-01 05:49:21.483607 argus-alm-0.8.1/README.md
+-rw-r--r--   0        0        0        0 2021-09-15 07:58:01.000000 argus-alm-0.8.1/argus/__init__.py
+-rw-r--r--   0        0        0        0 2021-09-26 18:50:58.000000 argus-alm-0.8.1/argus/backend/.gitkeep
+-rw-r--r--   0        0        0        0 2022-05-27 12:21:06.789497 argus-alm-0.8.1/argus/backend/__init__.py
+-rw-r--r--   0        0        0      607 2022-11-27 07:38:08.654478 argus-alm-0.8.1/argus/backend/cli.py
+-rw-r--r--   0        0        0        0 2022-05-27 12:21:06.789497 argus-alm-0.8.1/argus/backend/controller/__init__.py
+-rw-r--r--   0        0        0      575 2022-07-28 08:36:38.800118 argus-alm-0.8.1/argus/backend/controller/admin.py
+-rw-r--r--   0        0        0     5545 2022-07-28 08:36:38.800118 argus-alm-0.8.1/argus/backend/controller/admin_api.py
+-rw-r--r--   0        0        0    18152 2022-11-27 07:38:08.654478 argus-alm-0.8.1/argus/backend/controller/api.py
+-rw-r--r--   0        0        0     2029 2022-09-01 05:49:21.483607 argus-alm-0.8.1/argus/backend/controller/auth.py
+-rw-r--r--   0        0        0     2582 2022-11-27 07:38:08.654478 argus-alm-0.8.1/argus/backend/controller/client_api.py
+-rw-r--r--   0        0        0     8212 2022-07-28 08:36:38.800118 argus-alm-0.8.1/argus/backend/controller/main.py
+-rw-r--r--   0        0        0     1964 2022-07-28 08:36:38.800118 argus-alm-0.8.1/argus/backend/controller/notification_api.py
+-rw-r--r--   0        0        0      290 2022-07-28 08:36:38.800118 argus-alm-0.8.1/argus/backend/controller/notifications.py
+-rw-r--r--   0        0        0     3794 2022-11-27 07:38:08.654478 argus-alm-0.8.1/argus/backend/db.py
+-rw-r--r--   0        0        0      480 2022-07-28 08:36:38.800118 argus-alm-0.8.1/argus/backend/error_handlers.py
+-rw-r--r--   0        0        0     1188 2022-07-28 08:36:38.800118 argus-alm-0.8.1/argus/backend/events/event_processors.py
+-rw-r--r--   0        0        0        0 2022-07-28 08:36:38.800118 argus-alm-0.8.1/argus/backend/models/__init__.py
+-rw-r--r--   0        0        0    11658 2022-11-27 07:38:08.654478 argus-alm-0.8.1/argus/backend/models/web.py
+-rw-r--r--   0        0        0        0 2022-07-28 08:36:38.800118 argus-alm-0.8.1/argus/backend/plugins/__init__.py
+-rw-r--r--   0        0        0     2209 2022-11-27 07:38:08.655478 argus-alm-0.8.1/argus/backend/plugins/core.py
+-rw-r--r--   0        0        0      953 2022-11-27 07:38:08.655478 argus-alm-0.8.1/argus/backend/plugins/loader.py
+-rw-r--r--   0        0        0     3382 2022-11-16 08:22:10.409524 argus-alm-0.8.1/argus/backend/plugins/sct/controller.py
+-rw-r--r--   0        0        0      369 2022-11-27 07:38:08.655478 argus-alm-0.8.1/argus/backend/plugins/sct/plugin.py
+-rw-r--r--   0        0        0    10120 2022-09-01 05:48:41.448176 argus-alm-0.8.1/argus/backend/plugins/sct/resource_setup.py
+-rw-r--r--   0        0        0     8723 2022-11-16 08:24:35.462120 argus-alm-0.8.1/argus/backend/plugins/sct/service.py
+-rw-r--r--   0        0        0     8679 2022-11-27 07:38:08.655478 argus-alm-0.8.1/argus/backend/plugins/sct/testrun.py
+-rw-r--r--   0        0        0     2420 2022-09-01 05:48:41.450177 argus-alm-0.8.1/argus/backend/plugins/sct/udt.py
+-rw-r--r--   0        0        0      637 2022-07-28 08:36:38.801118 argus-alm-0.8.1/argus/backend/service/admin.py
+-rw-r--r--   0        0        0    39389 2022-11-27 07:38:08.655478 argus-alm-0.8.1/argus/backend/service/argus_service.py
+-rw-r--r--   0        0        0     6586 2022-07-28 08:36:38.801118 argus-alm-0.8.1/argus/backend/service/build_system_monitor.py
+-rw-r--r--   0        0        0     2109 2022-08-09 10:19:50.898405 argus-alm-0.8.1/argus/backend/service/client_service.py
+-rw-r--r--   0        0        0     6953 2022-11-27 07:38:08.656478 argus-alm-0.8.1/argus/backend/service/notification_manager.py
+-rw-r--r--   0        0        0     6146 2022-07-28 08:36:38.802118 argus-alm-0.8.1/argus/backend/service/release_manager.py
+-rw-r--r--   0        0        0    11632 2022-11-27 07:38:08.656478 argus-alm-0.8.1/argus/backend/service/stats.py
+-rw-r--r--   0        0        0     8858 2022-07-28 08:36:38.802118 argus-alm-0.8.1/argus/backend/service/user.py
+-rw-r--r--   0        0        0      523 2022-07-28 08:36:38.802118 argus-alm-0.8.1/argus/backend/template_filters.py
+-rw-r--r--   0        0        0     1033 2022-11-27 07:38:08.656478 argus-alm-0.8.1/argus/backend/util/common.py
+-rw-r--r--   0        0        0      860 2022-07-28 08:36:38.802118 argus-alm-0.8.1/argus/backend/util/config.py
+-rw-r--r--   0        0        0      596 2022-07-28 08:36:38.802118 argus-alm-0.8.1/argus/backend/util/encoders.py
+-rw-r--r--   0        0        0      675 2022-07-28 08:36:38.802118 argus-alm-0.8.1/argus/backend/util/enums.py
+-rw-r--r--   0        0        0     2323 2022-11-27 07:38:08.656478 argus-alm-0.8.1/argus/backend/util/logsetup.py
+-rw-r--r--   0        0        0      698 2022-07-28 08:36:38.802118 argus-alm-0.8.1/argus/backend/util/module_loaders.py
+-rw-r--r--   0        0        0     3217 2022-09-07 08:26:07.827285 argus-alm-0.8.1/argus/backend/util/send_email.py
+-rw-r--r--   0        0        0       42 2022-09-01 05:48:41.452177 argus-alm-0.8.1/argus/client/__init__.py
+-rw-r--r--   0        0        0     5832 2022-11-27 07:38:08.656478 argus-alm-0.8.1/argus/client/base.py
+-rw-r--r--   0        0        0     8217 2022-09-01 05:48:41.453177 argus-alm-0.8.1/argus/client/sct/client.py
+-rw-r--r--   0        0        0      371 2022-09-01 05:48:41.453177 argus-alm-0.8.1/argus/client/sct/types.py
+-rw-r--r--   0        0        0        0 2021-09-26 18:50:58.000000 argus-alm-0.8.1/argus/db/.gitkeep
+-rw-r--r--   0        0        0      391 2022-07-11 19:38:43.143896 argus-alm-0.8.1/argus/db/argus_json.py
+-rw-r--r--   0        0        0     3702 2022-07-05 06:42:49.837801 argus-alm-0.8.1/argus/db/cloud_types.py
+-rw-r--r--   0        0        0     3511 2022-11-27 07:38:53.330132 argus-alm-0.8.1/argus/db/config.py
+-rw-r--r--   0        0        0     3612 2022-06-02 12:42:55.427721 argus-alm-0.8.1/argus/db/db_types.py
+-rw-r--r--   0        0        0    17146 2022-11-27 07:38:53.330132 argus-alm-0.8.1/argus/db/interface.py
+-rw-r--r--   0        0        0    26014 2022-07-28 08:36:38.802118 argus-alm-0.8.1/argus/db/testrun.py
+-rw-r--r--   0        0        0      337 2021-10-03 12:19:16.000000 argus-alm-0.8.1/argus/db/utils.py
+-rw-r--r--   0        0        0     1011 2022-11-27 07:39:09.248421 argus-alm-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     7378 1970-01-01 00:00:00.000000 argus-alm-0.8.1/setup.py
+-rw-r--r--   0        0        0     6857 1970-01-01 00:00:00.000000 argus-alm-0.8.1/PKG-INFO
```

### Comparing `argus-alm-0.8.0/LICENSE` & `argus-alm-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `argus-alm-0.8.0/argus/backend/build_system_monitor.py` & `argus-alm-0.8.1/argus/backend/service/build_system_monitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,52 +2,52 @@
 from abc import ABC, abstractmethod
 import jenkins
 import click
 from flask import current_app
 from flask.cli import with_appcontext
 
 from argus.backend.db import ScyllaCluster
-from argus.db.models import ArgusRelease, ArgusReleaseGroup, ArgusReleaseGroupTest
+from argus.backend.models.web import ArgusRelease, ArgusGroup, ArgusTest
 from argus.backend.service.release_manager import ReleaseManagerService
 
 LOGGER = logging.getLogger(__name__)
 
 
 class ArgusTestsMonitor(ABC):
     def __init__(self) -> None:
         self._cluster = ScyllaCluster.get()
         self._existing_releases = list(ArgusRelease.all())
-        self._existing_groups = list(ArgusReleaseGroup.all())
-        self._existing_tests = list(ArgusReleaseGroupTest.all())
+        self._existing_groups = list(ArgusGroup.all())
+        self._existing_tests = list(ArgusTest.all())
         self._filtered_groups: list[str] = current_app.config["BUILD_SYSTEM_FILTERED_PREFIXES"]
 
     def create_release(self, release_name):
         # pylint: disable=no-self-use
         release = ArgusRelease()
         release.name = release_name
         release.save()
 
         return release
 
     def create_group(self, release: ArgusRelease, group_name: str, build_id: str, group_pretty_name: str | None = None):
         # pylint: disable=no-self-use
-        group = ArgusReleaseGroup()
+        group = ArgusGroup()
         group.release_id = release.id
         group.name = group_name
         group.build_system_id = build_id
         if group_pretty_name:
             group.pretty_name = group_pretty_name
         group.save()
 
         return group
 
-    def create_test(self, release: ArgusRelease, group: ArgusReleaseGroup,
-                    test_name: str, build_id: str, build_url: str) -> ArgusReleaseGroupTest:
+    def create_test(self, release: ArgusRelease, group: ArgusGroup,
+                    test_name: str, build_id: str, build_url: str) -> ArgusTest:
         # pylint: disable=no-self-use
-        test = ArgusReleaseGroupTest()
+        test = ArgusTest()
         test.name = test_name
         test.group_id = group.id
         test.release_id = release.id
         test.build_system_id = build_id
         test.build_system_url = build_url
         test.validate_build_system_id()
         test.save()
@@ -134,15 +134,7 @@
 
     def collect_groups_for_release(self, jobs):
         # pylint: disable=no-self-use
         groups = [folder for folder in jobs if "Folder" in folder["_class"]]
         groups = [group for group in groups if self.check_filter(group["name"])]
 
         return groups
-
-
-@click.command('scan-jenkins')
-@with_appcontext
-def scan_jenkins_command():
-    monitor = JenkinsMonitor()
-    monitor.collect()
-    click.echo("Done.")
```

### Comparing `argus-alm-0.8.0/argus/backend/controller/admin.py` & `argus-alm-0.8.1/argus/backend/controller/admin.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,16 @@
 import logging
-from uuid import UUID
 from flask import (
     Blueprint,
-    g,
-    request,
-    session,
-    flash,
-    redirect,
     render_template,
-    url_for,
-    make_response
 )
-from flask.json import jsonify
-from argus.backend.service.argus_service import ArgusService
-from argus.backend.service.admin import AdminService
 from argus.backend.controller.admin_api import bp as admin_api_bp
-from argus.backend.controller.auth import login_required, check_roles
-from argus.db.models import UserRoles
+from argus.backend.service.user import login_required, check_roles
+from argus.backend.models.web import UserRoles
 
-# pylint: disable=broad-except
 bp = Blueprint('admin', __name__, url_prefix='/admin')
 bp.register_blueprint(admin_api_bp)
 LOGGER = logging.getLogger(__name__)
 
 
 @bp.route("/")
 @bp.route("/<string:path>")
```

### Comparing `argus-alm-0.8.0/argus/backend/controller/main.py` & `argus-alm-0.8.1/argus/backend/controller/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 from uuid import UUID
 from flask import (
     Blueprint, flash, g, redirect, render_template, request, session, url_for, make_response
 )
 from argus.backend.controller.notifications import bp as notifications_bp
 from argus.backend.service.argus_service import ArgusService
-from argus.db.models import WebFileStorage
-from argus.backend.controller.auth import login_required
+from argus.backend.models.web import WebFileStorage
+from argus.backend.service.user import UserService, login_required
 
 LOGGER = logging.getLogger(__name__)
 
 bp = Blueprint('main', __name__)
 bp.register_blueprint(notifications_bp)
 
 
@@ -109,26 +109,27 @@
     return render_template("error.html.j2", type=request.args.get("type", 400))
 
 
 @bp.route("/profile/")
 @login_required
 def profile():
     first_run = session.pop("first_run_info", None)
+    token_generated = session.pop("token_generated", None)
 
-    return render_template("profile.html.j2", first_run=first_run)
+    return render_template("profile.html.j2", first_run=first_run, token_generated=token_generated)
 
 
 @bp.route("/profile/oauth/github", methods=["GET"])
 def profile_oauth_github_callback():
     req_state = request.args.get('state', '')
     if req_state != session["csrf_token"]:
         return redirect(url_for("main.error", type=403))
 
     req_code = request.args.get("code", "WTF")
-    service = ArgusService()
+    service = UserService()
     try:
         first_run_info = service.github_callback(req_code)
     except Exception as exc:  # pylint: disable=broad-except
         flash(message=exc.args[0], category="error")
         return redirect(url_for("main.error", type=403))
     if first_run_info:
         session["first_run_info"] = first_run_info
@@ -166,43 +167,43 @@
         flash(
             message=f"Expected image/*, got {req_file.content_type}", category="error")
         return redirect(url_for("main.profile"))
     if not picture_data:
         flash(message="No picture provided", category="error")
         return redirect(url_for("main.profile"))
 
-    service = ArgusService()
+    service = UserService()
     filename, filepath = service.save_profile_picture_to_disk(
         picture_name, picture_data, g.user.username)
     service.update_profile_picture(filename, filepath)
 
     return redirect(url_for("main.profile"))
 
 
 @bp.route("/profile/update/name", methods=["POST"])
 @login_required
 def update_full_name():
     new_name = request.values.get("new_name")
     if not new_name:
         flash(message="Incorrect new name", category="error")
     else:
-        service = ArgusService()
+        service = UserService()
         service.update_name(g.user, new_name)
         flash("Successfully changed name!", category="success")
     return redirect(url_for("main.profile"))
 
 
 @bp.route("/profile/update/email", methods=["POST"])
 @login_required
 def update_email():
     new_email = request.values.get("new_email")
     if not new_email:
         flash("Incorrect new email", category="error")
     else:
-        service = ArgusService()
+        service = UserService()
         service.update_email(g.user, new_email)
         flash("Successfully changed email!", category="success")
     return redirect(url_for("main.profile"))
 
 
 @bp.route("/profile/update/password", methods=["POST"])
 @login_required
@@ -217,15 +218,15 @@
         flash("New password wasn't provided", category="error")
         return redirect(url_for("main.profile"))
 
     if not new_password == new_password_confirm:
         flash("New password doesn't match confirmation!", category="error")
         return redirect(url_for("main.profile"))
 
-    service = ArgusService()
+    service = UserService()
     try:
         service.update_password(
             g.user, old_password=old_password, new_password=new_password)
     except Exception:  # pylint: disable=broad-except
         flash("Old password is incorrect", category="error")
         return redirect(url_for("main.profile"))
 
@@ -233,15 +234,15 @@
     return redirect(url_for("main.profile"))
 
 
 @bp.route("/profile/jobs", methods=["GET"])
 @login_required
 def profile_jobs():
     service = ArgusService()
-    jobs = [dict(job.items()) for job in service.get_jobs_for_user(g.user)]
+    jobs = service.get_jobs_for_user(g.user)
     return render_template("profile_jobs.html.j2", runs=jobs)
 
 
 @bp.route("/profile/schedules", methods=["GET"])
 @login_required
 def profile_schedules():
     service = ArgusService()
```

### Comparing `argus-alm-0.8.0/argus/backend/db.py` & `argus-alm-0.8.1/argus/backend/db.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,61 @@
 import logging
 from typing import Optional
-import click
 from flask import g, Flask
-from flask.cli import with_appcontext
 # pylint: disable=no-name-in-module
 from cassandra.policies import WhiteListRoundRobinPolicy
 from cassandra.cluster import Session
 from cassandra import ConsistencyLevel
 from cassandra.cluster import ExecutionProfile, EXEC_PROFILE_DEFAULT, Cluster
 from cassandra.cluster import PreparedStatement
 from cassandra.cqlengine.management import sync_table, sync_type
 from cassandra.cqlengine import connection
 from cassandra.query import dict_factory
 from cassandra.auth import PlainTextAuthProvider
+from argus.backend.util.config import Config
 
-from argus.db.config import FileConfig
-from argus.db.models import USED_MODELS, USED_TYPES
-from argus.db.interface import ArgusDatabase
-from argus.db.testrun import TestRun
+from argus.backend.models.web import USED_MODELS, USED_TYPES
 
-DB_CONFIG = FileConfig()
-CLUSTER: Cluster | None = None
 LOGGER = logging.getLogger(__name__)
 
 
 class ScyllaCluster:
     # pylint: disable=too-many-instance-attributes
     APP_INSTANCE: Optional['ScyllaCluster'] = None
 
     def __init__(self, config=None):
         if not config:
-            config = FileConfig()
+            config = Config.load_yaml_config()
         self.config = config
-        self.auth_provider = PlainTextAuthProvider(username=config.username, password=config.password)
-        self.lb_policy = WhiteListRoundRobinPolicy(hosts=config.contact_points)
+        self.auth_provider = PlainTextAuthProvider(
+            username=config["SCYLLA_USERNAME"], password=config["SCYLLA_PASSWORD"])
+        self.lb_policy = WhiteListRoundRobinPolicy(hosts=config["SCYLLA_CONTACT_POINTS"])
         self.execution_profile = ExecutionProfile(
             load_balancing_policy=self.lb_policy, consistency_level=ConsistencyLevel.QUORUM)
-        connection.setup(hosts=config.contact_points, default_keyspace=config.keyspace_name,
+        connection.setup(hosts=config["SCYLLA_CONTACT_POINTS"], default_keyspace=config["SCYLLA_KEYSPACE_NAME"],
                          auth_provider=self.auth_provider,
                          protocol_version=4,
                          execution_profiles={EXEC_PROFILE_DEFAULT: self.execution_profile})
         self.cluster: Cluster = connection.get_cluster(connection='default')
-        self.session = self.cluster.connect(keyspace=self.config.keyspace_name)
+        self.session: Session = self.cluster.connect(keyspace=config["SCYLLA_KEYSPACE_NAME"])
         self.prepared_statements = {}
-        self.argus_interface = ArgusDatabase(config=FileConfig())
         self.read_exec_profile = ExecutionProfile(
             consistency_level=ConsistencyLevel.ONE,
             row_factory=dict_factory,
             load_balancing_policy=self.lb_policy
         )
         self.read_named_tuple_exec_profile = ExecutionProfile(
             consistency_level=ConsistencyLevel.ONE,
             load_balancing_policy=self.lb_policy
         )
         self.cluster.add_execution_profile("read_fast", self.read_exec_profile)
         self.cluster.add_execution_profile("read_fast_named_tuple", self.read_named_tuple_exec_profile)
-        TestRun.set_argus(self.argus_interface)
 
     @classmethod
-    def get(cls, config: FileConfig = None) -> 'ScyllaCluster':
+    def get(cls, config: Config = None) -> 'ScyllaCluster':
         if cls.APP_INSTANCE:
             return cls.APP_INSTANCE
 
         cls.APP_INSTANCE = cls(config)
         return cls.APP_INSTANCE
 
     @classmethod
@@ -76,43 +69,25 @@
             LOGGER.info("Unprepared statement %s, preparing...", query)
             statement = self.session.prepare(query=query)
             self.prepared_statements[query] = statement
         return statement
 
     def sync_models(self):
         for udt in USED_TYPES:
-            sync_type(ks_name=self.config.keyspace_name, type_model=udt)
+            sync_type(ks_name=self.config["SCYLLA_KEYSPACE_NAME"], type_model=udt)
         for model in USED_MODELS:
             sync_table(model)
 
-    def create_session(self) -> Session:
-        return self.session
-
-    def shutdown_session(self, session: Session):
-        pass
-
     @classmethod
     def get_session(cls):
         cluster = cls.get()
         if 'scylla_session' not in g:
-            g.scylla_session = cluster.create_session()  # pylint: disable=assigning-non-slot
+            g.scylla_session = cluster.session  # pylint: disable=assigning-non-slot
         return g.scylla_session
 
     @classmethod
     def close_session(cls, error=None):  # pylint: disable=unused-argument
-        cluster = cls.get()
-        session: Session = g.pop("scylla_session", None)
-        if session:
-            cluster.shutdown_session(session)
-
-    @click.command('sync-models')
-    @with_appcontext
-    @staticmethod
-    def sync_models_command():
-        cluster = ScyllaCluster.get()
-        cluster.sync_models()
-        click.echo("Models synchronized.")
+        g.pop("scylla_session", None)
 
     @classmethod
     def attach_to_app(cls, app: Flask):
         app.teardown_appcontext(cls.close_session)
-        app.cli.add_command(cls.sync_models_command)
```

### Comparing `argus-alm-0.8.0/argus/backend/event_processors.py` & `argus-alm-0.8.1/argus/backend/events/event_processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from argus.db.models import ArgusEventTypes
+from argus.backend.models.web import ArgusEventTypes
 
 
 def event_process_posted_comment(event: dict) -> dict:
     return event["message"].format(**event)
 
 
 def event_process_status_changed(event: dict) -> dict:
```

### Comparing `argus-alm-0.8.0/argus/backend/logsetup.py` & `argus-alm-0.8.1/argus/backend/util/logsetup.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,46 +32,46 @@
         else:
             record.url = ''
             record.remote_addr = ''
             record.endpoint = ''
         return super().format(record)
 
 
-def setup_argus_logging():
+def setup_application_logging(log_level=logging.INFO):
     dictConfig({
         'version': 1,
         'formatters': {
             'request': {
-                'class': 'argus.backend.logsetup.ArgusRequestLogFormatter',
+                'class': f"{__name__}.{ArgusRequestLogFormatter.__name__}",
                 'format': LOG_FORMAT_REQUEST,
             }
         },
         'handlers': {
             'main': {
                 'class': 'logging.StreamHandler',
                 'stream': 'ext://sys.stderr',
                 'formatter': 'request'
             }
         },
         'loggers': {
             'cassandra': {
-                'level': 'INFO',
+                'level': log_level,
                 'handlers': ['main']
             },
             'argus': {
-                'level': 'INFO',
+                'level': log_level,
                 'handlers': ['main']
             },
             'argus_backend': {
-                'level': 'INFO',
+                'level': log_level,
                 'handlers': ['main']
             },
             'werkzeug': {
-                'level': 'INFO',
+                'level': log_level,
                 'handlers': ['main']
             },
             'uwsgi': {
-                'level': 'INFO',
+                'level': log_level,
                 'handlers': ['main']
             }
         }
     })
```

### Comparing `argus-alm-0.8.0/argus/backend/service/admin.py` & `argus-alm-0.8.1/argus/backend/service/admin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 
 from flask import g, current_app, session
 
 from argus.backend.db import ScyllaCluster
-from argus.db.models import (
+from argus.backend.models.web import (
     ArgusGithubIssue,
     ArgusRelease,
-    ArgusReleaseGroup,
-    ArgusReleaseGroupTest,
-    ArgusReleaseSchedule,
-    ArgusReleaseScheduleAssignee,
-    ArgusReleaseScheduleGroup,
-    ArgusReleaseScheduleTest,
+    ArgusGroup,
+    ArgusTest,
+    ArgusSchedule,
+    ArgusScheduleAssignee,
+    ArgusScheduleGroup,
+    ArgusScheduleTest,
     ArgusTestRunComment,
     ArgusEvent,
     ArgusEventTypes,
     ReleasePlannerComment,
     User,
     UserOauthToken,
     WebFileStorage,
```

### Comparing `argus-alm-0.8.0/argus/backend/service/argus_service.py` & `argus-alm-0.8.1/argus/backend/service/argus_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,141 +1,68 @@
-import base64
 import subprocess
 import time
 import json
 import re
-import os
-import hashlib
 import logging
 import datetime
 from types import NoneType
-from typing import Callable
 from collections import namedtuple
 from uuid import UUID, uuid4
 
-import humanize
 import requests
-from cassandra.util import uuid_from_time
+from cassandra.util import uuid_from_time  # pylint: disable=no-name-in-module
 from cassandra.cqlengine import ValidationError
-from flask import g, current_app, session
-from werkzeug.security import check_password_hash, generate_password_hash
+from flask import g, current_app
 from argus.backend.db import ScyllaCluster
+from argus.backend.plugins.sct.testrun import SCTTestRun
 from argus.backend.service.notification_manager import NotificationManagerService
-from argus.db.db_types import TestInvestigationStatus
-from argus.db.testrun import TestRun, TestStatus
-from argus.db.models import (
+from argus.backend.util.enums import TestStatus, TestInvestigationStatus
+from argus.backend.models.web import (
     ArgusGithubIssue,
     ArgusRelease,
-    ArgusReleaseGroup,
-    ArgusReleaseGroupTest,
-    ArgusReleaseSchedule,
-    ArgusReleaseScheduleAssignee,
-    ArgusReleaseScheduleGroup,
-    ArgusReleaseScheduleTest,
+    ArgusGroup,
+    ArgusTest,
+    ArgusSchedule,
+    ArgusScheduleAssignee,
+    ArgusScheduleGroup,
+    ArgusScheduleTest,
     ArgusTestRunComment,
     ArgusNotificationSourceTypes,
     ArgusNotificationTypes,
     ArgusEvent,
     ArgusEventTypes,
     ReleasePlannerComment,
     User,
-    UserOauthToken,
-    WebFileStorage,
 )
-from argus.backend.event_processors import EVENT_PROCESSORS
+from argus.backend.events.event_processors import EVENT_PROCESSORS
+from argus.backend.util.common import strip_html_tags
 
 LOGGER = logging.getLogger(__name__)
 
 
-def first(iterable, value, key: Callable = None, predicate: Callable = None):
-    for elem in iterable:
-        if predicate and predicate(elem, value):
-            return elem
-        elif key and key(elem) == value:
-            return elem
-        elif elem == value:
-            return elem
-    return None
-
-
-def check_scheduled_test(test, group, testname):
-    return testname == f"{group}/{test}" or testname == test
-
-
-def strip_html_tags(text: str):
-    return text.replace("<", "&lt;").replace(">", "&gt;")
-
-
-def convert_str_list_to_uuid(l: list[str]) -> list[UUID]:
-    return [UUID(s) for s in l]
-
-
-class GithubOrganizationMissingError(Exception):
-    pass
-
-
 class ArgusService:
     # pylint: disable=no-self-use,too-many-arguments,too-many-instance-attributes,too-many-locals, too-many-public-methods
     def __init__(self, database_session=None):
         self.session = database_session if database_session else ScyllaCluster.get_session()
         self.database = ScyllaCluster.get()
         self.notification_manager = NotificationManagerService()
         self.github_headers = {
             "Accept": "application/vnd.github.v3+json",
             "Authorization": f"token {current_app.config['GITHUB_ACCESS_TOKEN']}"
         }
-        self.runs_by_id_stmt = self.database.prepare(
-            f"SELECT * FROM {TestRun.table_name()} WHERE id = ?"
-        )
-        self.run_by_release_name_stmt = self.database.prepare(
-            "SELECT id, test_id, group_id, release_id, build_job_url, build_id, "
-            "status, start_time, end_time, heartbeat "
-            f"FROM {TestRun.table_name()} WHERE release_id = ?"
-        )
-        self.runs_by_build_system_id = self.database.prepare(
-            "SELECT id, test_id, group_id, release_id, build_job_url, build_id, "
-            "status, start_time, end_time, heartbeat "
-            f"FROM {TestRun.table_name()} WHERE build_id = ? LIMIT ?"
-        )
-        self.jobs_by_assignee = self.database.prepare(
-            "SELECT id, status, start_time, assignee, release_id, "
-            "investigation_status, "
-            "group_id, test_id, build_job_url, build_id FROM "
-            f"{TestRun.table_name()} WHERE assignee = ?"
-        )
-        self.run_by_release_stats_statement = self.database.prepare(
-            "SELECT id, test_id, group_id, release_id, status, start_time, build_job_url, build_id, assignee, "
-            f"end_time, investigation_status, heartbeat FROM {TestRun.table_name()} WHERE release_id = ?"
-        )
-        self.stats_by_build_id_statement = self.database.prepare(
-            "SELECT id, test_id, group_id, release_id, status, start_time, build_job_url, build_id, assignee, "
-            f"end_time, investigation_status, heartbeat FROM {TestRun.table_name()} WHERE build_id IN ?"
-        )
         self.build_id_and_url_statement = self.database.prepare(
-            f"SELECT build_id, build_job_url, test_id FROM {TestRun.table_name()} WHERE id = ?"
+            f"SELECT build_id, build_job_url, test_id FROM {SCTTestRun.table_name()} WHERE id = ?"
         )
         self.event_insert_statement = self.database.prepare(
             'INSERT INTO argus.argus_event '
             '("id", "release_id", "group_id", "test_id", "run_id", "user_id", "kind", "body", "created_at") '
             'VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?)'
         )
-        self.assignee_runs_by_schedule = self.database.prepare(
-            f"SELECT build_id, start_time, assignee, test_id FROM {TestRun.table_name()} "
-            "WHERE build_id = ? AND start_time >= ? AND start_time <= ?"
-        )
-        self.assignee_runs_by_schedule_multi = self.database.prepare(
-            f"SELECT build_id, start_time, assignee, test_id FROM {TestRun.table_name()} "
-            "WHERE build_id IN ? AND start_time >= ? AND start_time <= ?"
-        )
-        self.assignee_update_stmt = self.database.prepare(
-            f"UPDATE {TestRun.table_name()} SET assignee = ?"
-            "WHERE build_id = ? AND start_time = ?"
-        )
         self.scylla_versions_by_release = self.database.prepare(
-            f"SELECT scylla_version FROM {TestRun.table_name()} WHERE release_id = ?"
+            f"SELECT scylla_version FROM {SCTTestRun.table_name()} WHERE release_id = ?"
         )
 
     def get_version(self) -> str:
         try:
             proc = subprocess.run(["git", "rev-parse", "HEAD"], check=True, capture_output=True)
         except subprocess.CalledProcessError:
             proc = None
@@ -172,15 +99,15 @@
             )
 
         return response
 
     def create_groups(self, groups: dict, parent_release_id) -> dict:
         response = {}
         for group_name, group_definition in groups.items():
-            new_group = ArgusReleaseGroup()
+            new_group = ArgusGroup()
             new_group.release_id = parent_release_id
             new_group.name = group_name
             new_group.pretty_name = group_definition.get("pretty_name")
             new_group.save()
             response[group_name] = {}
             response[group_name]["status"] = "created"
             response[group_name]["tests"] = self.create_tests(
@@ -190,40 +117,38 @@
             )
         return response
 
     def create_tests(self, tests: dict, parent_group_id: UUID, parent_release_id: UUID) -> dict:
         response = {}
 
         for test_name in tests:
-            new_test = ArgusReleaseGroupTest()
+            new_test = ArgusTest()
             new_test.release_id = parent_release_id
             new_test.group_id = parent_group_id
             new_test.name = test_name
             new_test.save()
             response[test_name] = "created"
 
         return response
 
     def load_test_run(self, test_run_id: UUID):
-        run = TestRun.from_id(test_id=test_run_id)
-        return run.serialize() if run else None
+        try:
+            return SCTTestRun.get(id=test_run_id)
+        except SCTTestRun.DoesNotExist:
+            return None
 
     def get_comment(self, comment_id: UUID) -> ArgusTestRunComment | None:
         try:
             return ArgusTestRunComment.get(id=comment_id)
         except ArgusTestRunComment.DoesNotExist:
             return None
 
     def get_comments(self, test_id: UUID) -> list[ArgusTestRunComment]:
         return sorted(ArgusTestRunComment.filter(test_run_id=test_id).all(), key=lambda c: c.posted_at)
 
-    def get_user_info(self) -> dict:
-        users = User.all()
-        return {str(user.id): user.to_json() for user in users}
-
     def post_comment(self, payload: dict) -> list[ArgusTestRunComment]:
         test_run_id: str = payload.get("test_run_id")
         if not test_run_id:
             raise Exception("TestId wasn't specified in the payload")
 
         message: str = payload.get("message")
         if not message:
@@ -265,15 +190,16 @@
             }
             self.notification_manager.send_notification(
                 receiver=mention.id,
                 sender=comment.user_id,
                 notification_type=ArgusNotificationTypes.Mention,
                 source_type=ArgusNotificationSourceTypes.Comment,
                 source_id=comment.id,
-                content_params=params
+                content_params=params,
+                source_message=comment.message,
             )
 
         self.send_event(kind=ArgusEventTypes.TestRunCommentPosted, body={
             "message": "A comment was posted by {username}",
             "username": g.user.username
         }, user_id=g.user.id, run_id=UUID(test_run_id), release_id=release.id)
 
@@ -342,88 +268,79 @@
 
     def get_releases(self):
         releases = list(ArgusRelease.all())
         releases = sorted(releases, key=lambda r: r.name)
         releases = sorted(releases, key=lambda r: r.dormant)
         return releases
 
-    def get_groups(self, release_id: UUID) -> list[ArgusReleaseGroup]:
-        groups = list(ArgusReleaseGroup.filter(release_id=release_id).all())
+    def get_groups(self, release_id: UUID) -> list[ArgusGroup]:
+        groups = list(ArgusGroup.filter(release_id=release_id).all())
         return sorted(groups, key=lambda g: g.pretty_name if g.pretty_name else g.name)
 
     def get_groups_for_release(self, release: ArgusRelease):
-        groups = ArgusReleaseGroup.filter(release_id=release.id).all()
+        groups = ArgusGroup.filter(release_id=release.id).all()
         return sorted(groups, key=lambda g: g.pretty_name if g.pretty_name else g.name)
 
-    def get_tests(self, group_id: UUID) -> list[ArgusReleaseGroupTest]:
-        return list(ArgusReleaseGroupTest.filter(group_id=group_id).all())
+    def get_tests(self, group_id: UUID) -> list[ArgusTest]:
+        return list(ArgusTest.filter(group_id=group_id).all())
 
     def get_test_info(self, test_id: UUID) -> dict:
-        test = ArgusReleaseGroupTest.get(id=test_id)
-        group = ArgusReleaseGroup.get(id=test.group_id)
+        test = ArgusTest.get(id=test_id)
+        group = ArgusGroup.get(id=test.group_id)
         release = ArgusRelease.get(id=test.release_id)
         return {
             "test": dict(test.items()),
             "group": dict(group.items()),
             "release": dict(release.items()),
         }
 
     def get_data_for_release_dashboard(self, release_name: str):
         release = ArgusRelease.get(name=release_name)
-        release_groups = ArgusReleaseGroup.filter(release_id=release.id).all()
-        release_tests = ArgusReleaseGroupTest.filter(release_id=release.id).all()
+        release_groups = ArgusGroup.filter(release_id=release.id).all()
+        release_tests = ArgusTest.filter(release_id=release.id).all()
 
         return release, release_groups, release_tests
 
     def get_distinct_release_versions(self, release_id: UUID | str) -> list[str]:
         release_id = UUID(release_id) if isinstance(release_id, str) else release_id
         rows = self.session.execute(self.scylla_versions_by_release, parameters=(release_id,))
         unique_versions = {r["scylla_version"] for r in rows if r["scylla_version"]}
 
         return sorted(list(unique_versions), reverse=True)
 
     def poll_test_runs(self, test_id: UUID, additional_runs: list[UUID], limit: int = 10):
-        test: ArgusReleaseGroupTest = ArgusReleaseGroupTest.get(id=test_id)
+        test: ArgusTest = ArgusTest.get(id=test_id)
 
-        rows = self.session.execute(
-            self.runs_by_build_system_id,
-            parameters=(test.build_system_id, limit),
-            execution_profile="read_fast"
-        ).all()
+        rows: list[SCTTestRun] = list(SCTTestRun.filter(build_id=test.build_system_id).all().limit(limit))
 
-        rows_ids = [row["id"] for row in rows]
+        rows_ids = [row.id for row in rows]
 
         for run_id in additional_runs:
             if run_id not in rows_ids:
-                row = self.session.execute(
-                    self.runs_by_id_stmt,
-                    parameters=(UUID(run_id),),
-                    execution_profile="read_fast"
-                ).one()
+                row: SCTTestRun = SCTTestRun.get(id=run_id)
                 rows.append(row)
 
         for row in rows:
             try:
-                row["build_number"] = int(
-                    row["build_job_url"].rstrip("/").split("/")[-1])
+                setattr(row, "build_number", int(row["build_job_url"].rstrip("/").split("/")[-1]))
             except ValueError:
-                row["build_number"] = -1
+                setattr(row, "build_number", -1)
 
         return rows
 
     def poll_test_runs_single(self, runs: list[UUID]):
-        rows = []
+        rows: list[SCTTestRun] = []
         for run_id in runs:
-            row = self.session.execute(self.runs_by_id_stmt, parameters=(
-                run_id,), execution_profile="read_fast_named_tuple").one()
-            rows.append(row)
-
-        response = {str(row.id): TestRun.from_db_row(row).serialize()
-                    for row in rows if row}
+            try:
+                row: SCTTestRun = SCTTestRun.get(id=run_id)
+                rows.append(row)
+            except SCTTestRun.DoesNotExist:
+                pass
 
+        response = {str(row.id): row for row in rows}
         return response
 
     def send_event(self, kind: str, body: dict, user_id=None, run_id=None, release_id=None, group_id=None, test_id=None):
         params = (
             uuid4(),
             release_id,
             group_id,
@@ -441,18 +358,18 @@
         test_run_id = payload.get("test_run_id")
         if not test_run_id:
             raise Exception("Test run id wasn't specified in the request")
         if not new_status:
             raise Exception("New Status wasn't specified in the request")
 
         new_status = TestStatus(new_status)
-        test_run = TestRun.from_id(test_id=UUID(test_run_id))
-        test = ArgusReleaseGroupTest.get(build_system_id=test_run.build_id)
-        old_status = test_run.run_info.results.status
-        test_run.run_info.results.status = new_status
+        test_run: SCTTestRun = SCTTestRun.get(id=UUID(test_run_id))
+        test = ArgusTest.get(build_system_id=test_run.build_id)
+        old_status = TestStatus(test_run.status)
+        test_run.status = new_status.value
         test_run.save()
 
         self.send_event(
             kind=ArgusEventTypes.TestRunStatusChanged,
             body={
                 "message": "Status was changed from {old_status} to {new_status} by {username}",
                 "old_status": old_status.value,
@@ -475,18 +392,18 @@
         test_run_id = payload.get("test_run_id")
         if not test_run_id:
             raise Exception("Test run id wasn't specified in the request")
         if not new_status:
             raise Exception("New investigation status wasn't specified in the request")
 
         new_status = TestInvestigationStatus(new_status)
-        test_run = TestRun.from_id(UUID(test_run_id))
-        test = ArgusReleaseGroupTest.get(build_system_id=test_run.build_id)
+        test_run: SCTTestRun = SCTTestRun.get(id=UUID(test_run_id))
+        test = ArgusTest.get(build_system_id=test_run.build_id)
         old_status = test_run.investigation_status
-        test_run.investigation_status = new_status
+        test_run.investigation_status = new_status.value
         test_run.save()
 
         self.send_event(
             kind=ArgusEventTypes.TestRunStatusChanged,
             body={
                 "message": "Investigation status was changed from {old_status} to {new_status} by {username}",
                 "old_status": old_status,
@@ -515,16 +432,16 @@
 
         try:
             new_assignee = User.get(id=new_assignee)
         except ValidationError:
             if new_assignee != "none-none-none":
                 raise
             new_assignee = DummyUser(id=None, username="None")
-        test_run = TestRun.from_id(test_id=UUID(test_run_id))
-        test = ArgusReleaseGroupTest.get(build_system_id=test_run.build_id)
+        test_run: SCTTestRun = SCTTestRun.get(id=UUID(test_run_id))
+        test = ArgusTest.get(build_system_id=test_run.build_id)
         old_assignee = test_run.assignee
         old_assignee = User.get(id=old_assignee) if old_assignee else None
         test_run.assignee = new_assignee.id
         test_run.save()
 
         self.send_event(
             kind=ArgusEventTypes.AssigneeChanged,
@@ -584,18 +501,18 @@
         match = re.match(
             r"http(s)?://(www\.)?github\.com/(?P<owner>[\w\d]+)/"
             r"(?P<repo>[\w\d\-_]+)/(?P<type>issues|pull)/(?P<issue_number>\d+)(/)?",
             issue_url)
         if not match:
             raise Exception("URL doesn't match Github schema")
 
-        run = self.session.execute(self.runs_by_id_stmt, parameters=(UUID(run_id),)).one()
+        run = SCTTestRun.get(id=UUID(run_id))
         release = ArgusRelease.get(id=run["release_id"])
-        test = ArgusReleaseGroupTest.get(build_system_id=run["build_id"])
-        group = ArgusReleaseGroup.get(id=test.group_id)
+        test = ArgusTest.get(build_system_id=run["build_id"])
+        group = ArgusGroup.get(id=test.group_id)
 
         new_issue = ArgusGithubIssue()
         new_issue.user_id = g.user.id
         new_issue.run_id = run_id
         new_issue.group_id = group.id
         new_issue.release_id = release.id
         new_issue.test_id = test.id
@@ -686,119 +603,85 @@
         )
         issue.delete()
 
         return {
             "deleted": issue_id
         }
 
-    def fetch_release_issues(self, payload: dict) -> dict:
-        # TODO: Unused
-        """
-        Example payload
-        {
-            "release_id": "abcadedf-efadd-24124",
-            "tests": [ArgusReleaseGroupTest <, ...>]
-        }
-        Response
-        [[ArgusReleaseGroupTest, GithubIssue[]], ...]
-        """
-
-        release_id = payload.get("release_id")
-        if not release_id:
-            raise Exception("ReleaseId wasn't specified in the request")
-
-        release_issues = self.get_github_issues({
-            "filter_key": "release_id",
-            "id": release_id
-        })
-
-        tests = payload.get("tests", [])
-
-        response = []
-        for test in tests:
-            issues_for_test = [issue for issue in release_issues if issue["test_id"] == UUID(test["id"])]
-            if len(issues_for_test) > 0:
-                response.append([test, issues_for_test])
-
-        return response
-
-    def assign_runs_for_scheduled_test(self, schedule: ArgusReleaseSchedule, test_id: UUID, new_assignee: UUID):
-        test = ArgusReleaseGroupTest.get(id=test_id)
-        affected_rows = self.session.execute(
-            self.assignee_runs_by_schedule,
-            parameters=(test.build_system_id, schedule.period_start, schedule.period_end)
+    def assign_runs_for_scheduled_test(self, schedule: ArgusSchedule, test_id: UUID, new_assignee: UUID):
+        test: ArgusTest = ArgusTest.get(id=test_id)
+        affected_rows: list[SCTTestRun] = list(SCTTestRun.filter(
+            build_id=test.build_system_id,
+            start_time__gte=schedule.period_start,
+            start_time__lte=schedule.period_end
+        ).all()
         )
-
         for row in affected_rows:
-            if row["assignee"] == new_assignee:
-                continue
-            self.session.execute(
-                self.assignee_update_stmt,
-                parameters=(new_assignee, row["build_id"], row["start_time"])
-            )
+            if row.assignee != new_assignee:
+                row.assignee = new_assignee
+                row.save()
 
-    def assign_runs_for_scheduled_group(self, schedule: ArgusReleaseSchedule, group_id: UUID, new_assignee: UUID):
-        tests = ArgusReleaseGroupTest.filter(group_id=group_id).all()
+    def assign_runs_for_scheduled_group(self, schedule: ArgusSchedule, group_id: UUID, new_assignee: UUID):
+        tests = ArgusTest.filter(group_id=group_id).all()
         build_ids = [test.build_system_id for test in tests]
-        affected_rows = self.session.execute(
-            self.assignee_runs_by_schedule_multi,
-            parameters=(build_ids, schedule.period_start, schedule.period_end)
+        affected_rows: list[SCTTestRun] = list(SCTTestRun.filter(
+            build_id__in=build_ids,
+            start_time__gte=schedule.period_start,
+            start_time__lte=schedule.period_end
+        ).all()
         )
         for row in affected_rows:
-            if row["assignee"] == new_assignee:
-                continue
-            self.session.execute(
-                self.assignee_update_stmt,
-                parameters=(new_assignee, row["build_id"], row["start_time"])
-            )
+            if row.assignee != new_assignee:
+                row.assignee = new_assignee
+                row.save()
 
     def submit_new_schedule(self, release: str | UUID, start_time: str, end_time: str, tests: list[str | UUID],
                             groups: list[str | UUID], assignees: list[str | UUID], tag: str) -> dict:
         release = UUID(release) if isinstance(release, str) else release
         if len(assignees) == 0:
             raise Exception("Assignees not specified in the new schedule")
 
         if len(tests) == 0 and len(groups) == 0:
             raise Exception("Schedule does not contain scheduled objects")
 
-        schedule = ArgusReleaseSchedule()
+        schedule = ArgusSchedule()
         schedule.release_id = release
         schedule.period_start = datetime.datetime.fromisoformat(start_time)
         schedule.period_end = datetime.datetime.fromisoformat(end_time)
         schedule.id = uuid_from_time(schedule.period_start)
         schedule.tag = tag
         schedule.save()
 
         response = dict(schedule.items())
         response["assignees"] = []
         response["tests"] = []
         response["groups"] = []
 
         for test_id in tests:
-            test_entity = ArgusReleaseScheduleTest()
+            test_entity = ArgusScheduleTest()
             test_entity.id = uuid_from_time(schedule.period_start)
             test_entity.schedule_id = schedule.id
             test_entity.test_id = UUID(test_id) if isinstance(test_id, str) else test_id
             test_entity.release_id = release
             test_entity.save()
             self.assign_runs_for_scheduled_test(schedule, test_entity.test_id, UUID(assignees[0]))
             response["tests"].append(test_id)
 
         for group_id in groups:
-            group_entity = ArgusReleaseScheduleGroup()
+            group_entity = ArgusScheduleGroup()
             group_entity.id = uuid_from_time(schedule.period_start)
             group_entity.schedule_id = schedule.id
             group_entity.group_id = UUID(group_id) if isinstance(group_id, str) else group_id
             group_entity.release_id = release
             group_entity.save()
             self.assign_runs_for_scheduled_group(schedule, group_entity.group_id, UUID(assignees[0]))
             response["groups"].append(group_id)
 
         for assignee_id in assignees:
-            assignee_entity = ArgusReleaseScheduleAssignee()
+            assignee_entity = ArgusScheduleAssignee()
             assignee_entity.id = uuid_from_time(schedule.period_start)
             assignee_entity.schedule_id = schedule.id
             assignee_entity.assignee = UUID(assignee_id) if isinstance(assignee_id, str) else assignee_id
             assignee_entity.release_id = release
             assignee_entity.save()
             response["assignees"].append(assignee_id)
 
@@ -811,28 +694,28 @@
         }
         """
         release_id = UUID(release_id) if isinstance(release_id, str) else release_id
         release: ArgusRelease = ArgusRelease.get(id=release_id)
         if release.perpetual:
             today = datetime.datetime.utcnow()
             six_months_ago = today - datetime.timedelta(days=180)
-            u = uuid_from_time(six_months_ago)
-            schedules = ArgusReleaseSchedule.filter(release_id=release_id, id__gte=u).all()
+            uuid_six_months = uuid_from_time(six_months_ago)
+            schedules = ArgusSchedule.filter(release_id=release_id, id__gte=uuid_six_months).all()
         else:
-            schedules = ArgusReleaseSchedule.filter(release_id=release_id).all()
+            schedules = ArgusSchedule.filter(release_id=release_id).all()
         response = {
             "schedules": []
         }
         for schedule in schedules:
             serialized_schedule = dict(schedule.items())
-            tests = ArgusReleaseScheduleTest.filter(schedule_id=schedule.id).all()
+            tests = ArgusScheduleTest.filter(schedule_id=schedule.id).all()
             serialized_schedule["tests"] = [test.test_id for test in tests]
-            groups = ArgusReleaseScheduleGroup.filter(schedule_id=schedule.id).all()
+            groups = ArgusScheduleGroup.filter(schedule_id=schedule.id).all()
             serialized_schedule["groups"] = [group.group_id for group in groups]
-            assignees = ArgusReleaseScheduleAssignee.filter(schedule_id=schedule.id).all()
+            assignees = ArgusScheduleAssignee.filter(schedule_id=schedule.id).all()
             serialized_schedule["assignees"] = [assignee.assignee for assignee in assignees]
             response["schedules"].append(serialized_schedule)
 
         return response
 
     def update_schedule_assignees(self, payload: dict) -> dict:
         """
@@ -850,26 +733,26 @@
             raise Exception("No schedule Id provided")
 
         assignees = payload.get("newAssignees")
         if not assignees:
             raise Exception("No assignees provided")
 
         release = ArgusRelease.get(id=release_id)
-        schedule = ArgusReleaseSchedule.get(release_id=release.id, id=schedule_id)
-        schedule_tests = ArgusReleaseScheduleTest.filter(schedule_id=schedule.id).all()
-        schedule_groups = ArgusReleaseScheduleGroup.filter(schedule_id=schedule.id).all()
+        schedule = ArgusSchedule.get(release_id=release.id, id=schedule_id)
+        schedule_tests = ArgusScheduleTest.filter(schedule_id=schedule.id).all()
+        schedule_groups = ArgusScheduleGroup.filter(schedule_id=schedule.id).all()
         for test in schedule_tests:
             self.assign_runs_for_scheduled_test(schedule, test.test_id, UUID(assignees[0]))
 
         for group in schedule_groups:
             self.assign_runs_for_scheduled_group(schedule, group.group_id, UUID(assignees[0]))
 
-        old_assignees = list(ArgusReleaseScheduleAssignee.filter(schedule_id=schedule.id).all())
+        old_assignees = list(ArgusScheduleAssignee.filter(schedule_id=schedule.id).all())
         for new_assignee in assignees:
-            assignee = ArgusReleaseScheduleAssignee()
+            assignee = ArgusScheduleAssignee()
             assignee.release_id = release.id
             assignee.schedule_id = schedule.id
             assignee.assignee = UUID(new_assignee)
             assignee.save()
 
         for old_assignee in old_assignees:
             old_assignee.delete()
@@ -928,18 +811,18 @@
             raise Exception("Release name not specified in the request")
 
         schedule_id = payload.get("scheduleId")
         if not schedule_id:
             raise Exception("Schedule id not specified in the request")
 
         release = ArgusRelease.get(id=release_id)
-        schedule = ArgusReleaseSchedule.get(release_id=release.id, id=schedule_id)
-        tests = ArgusReleaseScheduleTest.filter(schedule_id=schedule.id).all()
-        groups = ArgusReleaseScheduleGroup.filter(schedule_id=schedule.id).all()
-        assignees = ArgusReleaseScheduleAssignee.filter(schedule_id=schedule.id).all()
+        schedule = ArgusSchedule.get(release_id=release.id, id=schedule_id)
+        tests = ArgusScheduleTest.filter(schedule_id=schedule.id).all()
+        groups = ArgusScheduleGroup.filter(schedule_id=schedule.id).all()
+        assignees = ArgusScheduleAssignee.filter(schedule_id=schedule.id).all()
 
         for entities in [tests, groups, assignees]:
             for entity in entities:
                 entity.delete()
 
         schedule.delete()
         return {
@@ -948,17 +831,17 @@
             "result": "deleted"
         }
 
     def get_planner_data(self, release_id: UUID | str) -> dict:
 
         release = ArgusRelease.get(id=release_id)
         release_comments = list(ReleasePlannerComment.filter(release=release.id).all())
-        groups = ArgusReleaseGroup.filter(release_id=release.id).all()
+        groups = ArgusGroup.filter(release_id=release.id).all()
         groups_by_group_id = {str(group.id): dict(group.items()) for group in groups if group.enabled}
-        tests = ArgusReleaseGroupTest.filter(release_id=release.id).all()
+        tests = ArgusTest.filter(release_id=release.id).all()
         tests = [dict(t.items()) for t in tests if t.enabled]
         tests_by_group = {}
         for test in tests:
             group = groups_by_group_id.get(str(test["group_id"]))
             if not group:
                 continue
             test["group_name"] = group["name"]
@@ -981,237 +864,114 @@
 
         return response
 
     def get_groups_assignees(self, release_id: UUID | str):
         release_id = UUID(release_id) if isinstance(release_id, str) else release_id
         release = ArgusRelease.get(id=release_id)
 
-        groups = ArgusReleaseGroup.filter(release_id=release_id).all()
+        groups = ArgusGroup.filter(release_id=release_id).all()
         group_ids = [group.id for group in groups if group.enabled]
 
-        scheduled_groups = ArgusReleaseScheduleGroup.filter(release_id=release.id, group_id__in=group_ids).all()
+        scheduled_groups = ArgusScheduleGroup.filter(release_id=release.id, group_id__in=group_ids).all()
         schedule_ids = {schedule.schedule_id for schedule in scheduled_groups}
 
-        schedules = ArgusReleaseSchedule.filter(release_id=release.id, id__in=tuple(schedule_ids)).all()
+        schedules = ArgusSchedule.filter(release_id=release.id, id__in=tuple(schedule_ids)).all()
 
+        valid_schedules = schedules
         if release.perpetual:
             today = datetime.datetime.utcnow()
             valid_schedules = [s for s in schedules if s.period_start <= today <= s.period_end]
 
         response = {}
         for schedule in valid_schedules:
-            assignees = ArgusReleaseScheduleAssignee.filter(schedule_id=schedule.id).all()
+            assignees = ArgusScheduleAssignee.filter(schedule_id=schedule.id).all()
             assignees_uuids = [assignee.assignee for assignee in assignees]
             schedule_groups = filter(lambda g: g.schedule_id == schedule.id, scheduled_groups)
             groups = {str(group.group_id): assignees_uuids for group in schedule_groups}
             response = {**groups, **response}
 
         return response
 
     def get_tests_assignees(self, group_id: UUID | str):
         group_id = UUID(group_id) if isinstance(group_id, str) else group_id
-        group = ArgusReleaseGroup.get(id=group_id)
+        group = ArgusGroup.get(id=group_id)
 
         release = ArgusRelease.get(id=group.release_id)
-        tests = ArgusReleaseGroupTest.filter(group_id=group_id).all()
+        tests = ArgusTest.filter(group_id=group_id).all()
 
         test_ids = [test.id for test in tests if test.enabled]
 
-        scheduled_tests = ArgusReleaseScheduleTest.filter(release_id=release.id, test_id__in=tuple(test_ids)).all()
+        scheduled_tests = ArgusScheduleTest.filter(release_id=release.id, test_id__in=tuple(test_ids)).all()
         schedule_ids = {test.schedule_id for test in scheduled_tests}
-        schedules = list(ArgusReleaseSchedule.filter(release_id=release.id, id__in=tuple(schedule_ids)).all())
+        schedules: list[ArgusSchedule] = list(ArgusSchedule.filter(
+            release_id=release.id, id__in=tuple(schedule_ids)).all())
 
         if release.perpetual:
             today = datetime.datetime.utcnow()
             schedules = list(filter(lambda s: s.period_start <= today <= s.period_end, schedules))
 
         response = {}
         for schedule in schedules:
-            assignees = ArgusReleaseScheduleAssignee.filter(schedule_id=schedule.id).all()
+            assignees = ArgusScheduleAssignee.filter(schedule_id=schedule.id).all()
             assignees_uuids = [assignee.assignee for assignee in assignees]
             schedule_tests = filter(lambda t: t.schedule_id == schedule.id, scheduled_tests)
             tests = {str(test.test_id): assignees_uuids for test in schedule_tests}
             response = {**tests, **response}
 
         return response
 
-    def update_email(self, user: User, new_email: str):
-        user.email = new_email
-        user.save()
-
-    def update_password(self, user: User, old_password: str, new_password: str):
-        if check_password_hash(user.password, old_password):
-            raise Exception("Incorrect old password")
-
-        user.password = generate_password_hash(new_password)
-        user.save()
-
-    def update_name(self, user: User, new_name: str):
-        user.full_name = new_name
-        user.save()
-
-    def update_profile_picture(self, filename, filepath):
-        web_file = WebFileStorage()
-        web_file.filename = filename
-        web_file.filepath = filepath
-        web_file.save()
-
-        try:
-            if old_picture_id := g.user.picture_id:
-                old_file = WebFileStorage.get(id=old_picture_id)
-                os.unlink(old_file.filepath)
-                old_file.delete()
-        except Exception as exc:  # pylint: disable=broad-except
-            print(exc)
-
-        g.user.picture_id = web_file.id
-        g.user.save()
-
-    def save_profile_picture_to_disk(self, original_filename, filedata, suffix):
-        filename_fragment = hashlib.sha256(os.urandom(64)).hexdigest()[:10]
-        filename = f"profile_{suffix}_{filename_fragment}"
-        filepath = f"storage/profile_pictures/{filename}"
-        with open(filepath, "wb") as file:
-            file.write(filedata)
-
-        return original_filename, filepath
-
-    def github_callback(self, req_code):
-        oauth_response = requests.post("https://github.com/login/oauth/access_token",
-                                       headers={
-                                           "Accept": "application/json",
-                                       },
-                                       params={
-                                           "code": req_code,
-                                           "client_id": current_app.config.get("GITHUB_CLIENT_ID"),
-                                           "client_secret": current_app.config.get("GITHUB_CLIENT_SECRET"),
-                                       })
-
-        oauth_data = oauth_response.json()
-
-        user_info = requests.get("https://api.github.com/user",
-                                 headers={
-                                     "Accept": "application/json",
-                                     "Authorization": f"token {oauth_data.get('access_token')}"
-                                 }).json()
-        email_info = requests.get("https://api.github.com/user/emails",
-                                  headers={
-                                      "Accept": "application/json",
-                                      "Authorization": f"token {oauth_data.get('access_token')}"
-                                  }).json()
-
-        organizations = requests.get("https://api.github.com/user/orgs", headers={
-            "Accept": "application/json",
-            "Authorization": f"token {oauth_data.get('access_token')}"
-        }).json()
-        temp_password = None
-        required_organizations = current_app.config.get("GITHUB_REQUIRED_ORGANIZATIONS")
-        if required_organizations:
-            logins = set([org["login"] for org in organizations])  # pylint: disable=consider-using-set-comprehension
-            required_organizations = set(required_organizations)
-            if len(logins.intersection(required_organizations)) == 0:
-                raise GithubOrganizationMissingError(
-                    "Not a member of a required organization or missing organization scope")
-
-        try:
-            user = User.get(username=user_info.get("login"))
-        except User.DoesNotExist:
-            user = User()
-            user.username = user_info.get("login")
-            user.email = email_info[-1].get("email")
-            user.full_name = user_info.get("name", user_info.get("login"))
-            user.registration_date = datetime.datetime.utcnow()
-            user.roles = ["ROLE_USER"]
-            temp_password = base64.encodebytes(
-                os.urandom(48)).decode("ascii").strip()
-            user.password = generate_password_hash(temp_password)
-
-            avatar_url: str = user_info.get("avatar_url")
-            avatar = requests.get(avatar_url).content
-            avatar_name = avatar_url.split("/")[-1]
-            filename, filepath = self.save_profile_picture_to_disk(avatar_name, avatar, user.username)
-
-            web_file = WebFileStorage()
-            web_file.filename = filename
-            web_file.filepath = filepath
-            web_file.save()
-            user.picture_id = web_file.id
-            user.save()
-
-        try:
-            tokens = list(UserOauthToken.filter(user_id=user.id).all())
-            github_token = [
-                token for token in tokens if token["kind"] == "github"][0]
-            github_token.token = oauth_data.get('access_token')
-            github_token.save()
-        except (UserOauthToken.DoesNotExist, IndexError):
-            github_token = UserOauthToken()
-            github_token.kind = "github"
-            github_token.user_id = user.id
-            github_token.token = oauth_data.get('access_token')
-            github_token.save()
-
-        session.clear()
-        session["user_id"] = str(user.id)
-        if temp_password:
-            return {
-                "password": temp_password,
-                "first_login": True
-            }
-        return None
-
     def get_jobs_for_user(self, user: User):
-        runs = self.session.execute(self.jobs_by_assignee, parameters=(user.id,))
+        runs: list[SCTTestRun] = list(SCTTestRun.filter(assignee=user.id).all())
         schedules = self.get_schedules_for_user(user)
         valid_runs = []
         today = datetime.datetime.now()
         month_ago = today - datetime.timedelta(days=30)
         for run in runs:
-            run_date = run["start_time"]
-            if user.id == run["assignee"] and run_date >= month_ago:
+            run_date = run.start_time
+            if user.id == run.assignee and run_date >= month_ago:
                 valid_runs.append(run)
                 continue
             for schedule in schedules:
-                if not run["release_id"] == schedule["release_id"]:
+                if not run.release_id == schedule["release_id"]:
                     continue
                 if not schedule["period_start"] < run_date < schedule["period_end"]:
                     continue
-                if run["assignee"] in schedule["assignees"]:
+                if run.assignee in schedule["assignees"]:
                     valid_runs.append(run)
                     break
-                if run["group_id"] in schedule["groups"]:
+                if run.group_id in schedule["groups"]:
                     valid_runs.append(run)
                     break
-                filtered_tests = [test for test in schedule["tests"] if test == run["test_id"]]
+                filtered_tests = [test for test in schedule["tests"] if test == run.test_id]
                 if len(filtered_tests) > 0:
                     valid_runs.append(run)
                     break
         return valid_runs
 
     def get_schedules_for_user(self, user: User):
-        all_assigned_schedules = ArgusReleaseScheduleAssignee.filter(assignee=user.id).all()
+        all_assigned_schedules = ArgusScheduleAssignee.filter(assignee=user.id).all()
         schedule_keys = [(schedule_assignee.release_id, schedule_assignee.schedule_id)
                          for schedule_assignee in all_assigned_schedules]
         schedules = []
         today = datetime.datetime.utcnow()
         for release_id, schedule_id in schedule_keys:
             try:
-                schedule = dict(ArgusReleaseSchedule.get(release_id=release_id, id=schedule_id).items())
-            except ArgusReleaseSchedule.DoesNotExist:
+                schedule = dict(ArgusSchedule.get(release_id=release_id, id=schedule_id).items())
+            except ArgusSchedule.DoesNotExist:
                 continue
             if schedule["period_start"] <= today <= schedule["period_end"]:
-                tests = ArgusReleaseScheduleTest.filter(schedule_id=schedule_id).all()
+                tests = ArgusScheduleTest.filter(schedule_id=schedule_id).all()
                 schedule["tests"] = [test.test_id for test in tests]
-                groups = ArgusReleaseScheduleGroup.filter(schedule_id=schedule_id).all()
+                groups = ArgusScheduleGroup.filter(schedule_id=schedule_id).all()
                 schedule["groups"] = [group.group_id for group in groups]
-                assignees = ArgusReleaseScheduleAssignee.filter(schedule_id=schedule_id).all()
+                assignees = ArgusScheduleAssignee.filter(schedule_id=schedule_id).all()
                 schedule["assignees"] = [assignee.assignee for assignee in assignees]
                 schedules.append(schedule)
 
         return schedules
 
     def get_planner_comment_by_test(self, test_id):
         try:
-            test = ArgusReleaseGroupTest.get(id=test_id)
+            test = ArgusTest.get(id=test_id)
             return ReleasePlannerComment.get(test=test.id, release=test.release_id, group=test.group_id).comment
         except ReleasePlannerComment.DoesNotExist:
             return ""
```

### Comparing `argus-alm-0.8.0/argus/backend/service/release_manager.py` & `argus-alm-0.8.1/argus/backend/service/release_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import logging
 from uuid import UUID
 from argus.backend.db import ScyllaCluster
-from argus.db.models import ArgusRelease, ArgusReleaseGroup, ArgusReleaseGroupTest
-from argus.db.testrun import TestRun
+from argus.backend.plugins.sct.testrun import SCTTestRun
+from argus.backend.models.web import ArgusRelease, ArgusGroup, ArgusTest
 
 LOGGER = logging.getLogger(__name__)
 
 
 class ReleaseManagerException(Exception):
     pass
 
 
 class ReleaseManagerService:
     def __init__(self) -> None:
         self.session = ScyllaCluster.get_session()
         self.database = ScyllaCluster.get()
         self.runs_by_build_id_stmt = self.database.prepare(
             "SELECT id, test_id, group_id, release_id, build_id, start_time "
-            f"FROM {TestRun.table_name()} WHERE build_id = ?"
+            f"FROM {SCTTestRun.table_name()} WHERE build_id = ?"
         )
         self.update_run_stmt = self.database.prepare(
-            f"UPDATE {TestRun.table_name()} SET test_id = ?, group_id = ?, release_id = ? "
+            f"UPDATE {SCTTestRun.table_name()} SET test_id = ?, group_id = ?, release_id = ? "
             "WHERE build_id = ? AND start_time = ?"
         )
 
     def get_releases(self) -> list[ArgusRelease]:
         return list(ArgusRelease.all())
 
-    def get_groups(self, release_id: UUID) -> list[ArgusReleaseGroup]:
-        return list(ArgusReleaseGroup.filter(release_id=release_id).all())
+    def get_groups(self, release_id: UUID) -> list[ArgusGroup]:
+        return list(ArgusGroup.filter(release_id=release_id).all())
 
-    def get_tests(self, group_id: UUID) -> list[ArgusReleaseGroupTest]:
-        return list(ArgusReleaseGroupTest.filter(group_id=group_id).all())
+    def get_tests(self, group_id: UUID) -> list[ArgusTest]:
+        return list(ArgusTest.filter(group_id=group_id).all())
 
     def create_release(self, release_name: str, pretty_name: str, perpetual: bool) -> ArgusRelease:
         try:
             release = ArgusRelease.get(name=release_name)
         except ArgusRelease.DoesNotExist:
             release = ArgusRelease()
             release.name = release_name
@@ -46,82 +46,82 @@
         else:
             raise ReleaseManagerException(
                 f"Release {release_name} already exists!", release_name)
 
         return release
 
     def create_group(self, group_name: str, pretty_name: str, build_system_id: str,
-                     release_id: str) -> ArgusReleaseGroup:
+                     release_id: str) -> ArgusGroup:
         release = ArgusRelease.get(id=UUID(release_id))
 
-        new_group = ArgusReleaseGroup()
+        new_group = ArgusGroup()
         new_group.name = group_name
         new_group.pretty_name = pretty_name
         new_group.release_id = release.id
         new_group.build_system_id = build_system_id
         new_group.save()
 
         return new_group
 
-    def create_test(self, test_name, pretty_name, build_id, build_url, group_id, release_id) -> ArgusReleaseGroupTest:
+    def create_test(self, test_name, pretty_name, build_id, build_url, group_id, release_id) -> ArgusTest:
         release = ArgusRelease.get(id=UUID(release_id))
-        group = ArgusReleaseGroup.get(id=UUID(group_id))
+        group = ArgusGroup.get(id=UUID(group_id))
 
-        new_test = ArgusReleaseGroupTest()
+        new_test = ArgusTest()
         new_test.name = test_name
         new_test.pretty_name = pretty_name
         new_test.build_system_id = build_id
         new_test.release_id = release.id
         new_test.group_id = group.id
         new_test.build_system_url = build_url
         new_test.validate_build_system_id()
         new_test.save()
         self.move_test_runs(new_test)
         return new_test
 
     def delete_group(self, group_id: str, delete_tests: bool = True, new_group_id: str = "") -> bool:
-        group_to_delete = ArgusReleaseGroup.get(id=UUID(group_id))
+        group_to_delete = ArgusGroup.get(id=UUID(group_id))
 
-        tests_to_change = ArgusReleaseGroupTest.filter(
+        tests_to_change = ArgusTest.filter(
             group_id=group_to_delete.id)
         if delete_tests:
             for test in tests_to_change.all():
                 test.delete()
         else:
-            new_group = ArgusReleaseGroup.get(id=UUID(new_group_id))
+            new_group = ArgusGroup.get(id=UUID(new_group_id))
             for test in tests_to_change.all():
                 test.group_id = new_group.id
                 test.save()
 
         group_to_delete.delete()
 
         return True
 
     def delete_test(self, test_id: str) -> bool:
-        test_to_delete = ArgusReleaseGroupTest.get(id=test_id)
+        test_to_delete = ArgusTest.get(id=test_id)
         test_to_delete.delete()
 
         return True
 
     def update_group(self, group_id: str, name: str, pretty_name: str, enabled: bool, build_system_id: str) -> bool:
-        group = ArgusReleaseGroup.get(id=UUID(group_id))
+        group = ArgusGroup.get(id=UUID(group_id))
 
         group.name = name
         group.build_system_id = build_system_id
         group.pretty_name = pretty_name
         group.enabled = enabled
 
         group.save()
 
         return True
 
     def update_test(self, test_id: str, name: str, pretty_name: str,
                     enabled: bool, build_system_id: str, build_system_url: str, group_id) -> bool:
-        test: ArgusReleaseGroupTest = ArgusReleaseGroupTest.get(id=UUID(test_id))
-        group = ArgusReleaseGroup.get(id=UUID(group_id))
+        test: ArgusTest = ArgusTest.get(id=UUID(test_id))
+        group = ArgusGroup.get(id=UUID(group_id))
 
         test.name = name
         test.pretty_name = pretty_name
         test.enabled = enabled
         test.build_system_id = build_system_id
         test.build_system_url = build_system_url
         if test.group_id != group.id:
@@ -151,26 +151,26 @@
         release = ArgusRelease.get(id=UUID(release_id))
         release.perpetual = perpetual
         release.save()
 
         return True
 
     def batch_move_tests(self, new_group_id: str, tests: list[str]) -> bool:
-        group = ArgusReleaseGroup.get(id=UUID(new_group_id))
+        group = ArgusGroup.get(id=UUID(new_group_id))
 
-        tests: list[ArgusReleaseGroupTest] = [ArgusReleaseGroupTest.get(id=UUID(test_id)) for test_id in tests]
+        tests: list[ArgusTest] = [ArgusTest.get(id=UUID(test_id)) for test_id in tests]
 
         for test in tests:
             test.group_id = group.id
             test.save()
             self.move_test_runs(test)
 
         return True
 
-    def move_test_runs(self, test: ArgusReleaseGroupTest) -> None:
+    def move_test_runs(self, test: ArgusTest) -> None:
         run_rows = self.session.execute(self.runs_by_build_id_stmt, parameters=(
             test.build_system_id,), execution_profile="read_fast")
         for run in run_rows:
             run["test_id"] = test.id
             run["group_id"] = test.group_id
             run["release_id"] = test.release_id
             self.session.execute(self.update_run_stmt, parameters=run)
```

### Comparing `argus-alm-0.8.0/argus/backend/service/stats.py` & `argus-alm-0.8.1/argus/backend/service/stats.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,75 +1,142 @@
 import logging
 
 from datetime import datetime
-from argus.db.db_types import TestStatus, TestInvestigationStatus
-from argus.db.testrun import TestRun
-from argus.db.models import ArgusGithubIssue, ArgusRelease, ArgusReleaseGroup, ArgusReleaseGroupTest, ArgusReleaseScheduleTest, ArgusTestRunComment
+from typing import TypedDict
+from uuid import UUID
+from argus.backend.plugins.sct.testrun import SCTTestRun
+from argus.backend.util.enums import TestStatus, TestInvestigationStatus
+from argus.backend.models.web import ArgusGithubIssue, ArgusRelease, ArgusGroup, ArgusTest,\
+    ArgusScheduleTest, ArgusTestRunComment
 from argus.backend.db import ScyllaCluster
 
 LOGGER = logging.getLogger(__name__)
 
 
+class TestRunStatRow(TypedDict):
+    build_id: str
+    status: TestStatus
+    investigation_status: TestInvestigationStatus
+    assignee: UUID
+    scylla_version: str  # TODO: rework SCT specific field
+    start_time: datetime
+    end_time: datetime
+    heartbeat: int
+    id: UUID
+    test_id: UUID
+    group_id: UUID
+    release_id: UUID
+    build_job_url: str
+
+
+class ComparableTestStatus:
+    PRIORITY_MAP = {
+        TestStatus.FAILED: 10,
+        TestStatus.ABORTED: 9,
+        TestStatus.RUNNING: 8,
+        TestStatus.CREATED: 7,
+        TestStatus.PASSED: 6,
+    }
+
+    def __init__(self, status: TestStatus):
+        self._status = status
+
+    def _get_prio(self):
+        return self.PRIORITY_MAP.get(self._status, 0)
+
+    def __eq__(self, __o: object) -> bool:
+        if not isinstance(__o, ComparableTestStatus):
+            return False
+        return self._get_prio() == __o._get_prio()
+
+    def __ne__(self, __o: object) -> bool:
+        if not isinstance(__o, ComparableTestStatus):
+            return False
+        return not self.__eq__(__o)
+
+    def __lt__(self, __o: object) -> bool:
+        if not isinstance(__o, ComparableTestStatus):
+            return False
+        return self._get_prio() < __o._get_prio()
+
+    def __gt__(self, __o: object) -> bool:
+        if not isinstance(__o, ComparableTestStatus):
+            return False
+        return self._get_prio() > __o._get_prio()
+
+    def __ge__(self, __o: object) -> bool:
+        if not isinstance(__o, ComparableTestStatus):
+            return False
+        return self._get_prio() >= __o._get_prio()
+
+    def __le__(self, __o: object) -> bool:
+        if not isinstance(__o, ComparableTestStatus):
+            return False
+        return self._get_prio() <= __o._get_prio()
+
+
 class ReleaseStats:
     def __init__(self, release: ArgusRelease) -> None:
         self.release = release
         self.groups: list[GroupStats] = []
         self.status_map = {status: 0 for status in TestStatus}
         self.total_tests = 0
         self.last_status = TestStatus.NOT_PLANNED
         self.last_investigation_status = TestInvestigationStatus.NOT_INVESTIGATED
         self.has_bug_report = False
         self.issues: list[ArgusGithubIssue] = []
         self.comments: list[ArgusTestRunComment] = []
-        self.test_schedules: list[ArgusReleaseScheduleTest] = []
+        self.test_schedules: list[ArgusScheduleTest] = []
         self.forced_collection = False
+        self.rows = []
+        self.all_tests = []
 
     def to_dict(self) -> dict:
         return {
             "release": dict(self.release.items()),
             "groups": {str(group.group.id): group.to_dict() for group in self.groups},
             "total": self.total_tests,
             **self.status_map,
             "disabled": not self.release.enabled,
             "perpetual": self.release.perpetual,
             "lastStatus": self.last_investigation_status,
             "lastInvestigationStatus": self.last_investigation_status,
             "hasBugReport": self.has_bug_report
         }
 
-    def collect(self, rows: list[dict], limited=False, force=False) -> None:
+    def collect(self, rows: list[TestRunStatRow], limited=False, force=False) -> None:
         self.forced_collection = force
         if not self.release.enabled and not force:
             return
 
         if not self.release.perpetual and not limited:
-            self.test_schedules = list(ArgusReleaseScheduleTest.filter(
+            self.test_schedules = list(ArgusScheduleTest.filter(
                 release_id=self.release.id
             ).all())
 
         self.rows = rows
         if not limited or force:
             self.issues = ArgusGithubIssue.filter(release_id=self.release.id).all()
             self.comments = ArgusTestRunComment.filter(release_id=self.release.id).all()
-        self.all_tests = ArgusReleaseGroupTest.filter(release_id=self.release.id).all()
-        groups: list[ArgusReleaseGroup] = ArgusReleaseGroup.filter(release_id=self.release.id).all()
+        self.all_tests = ArgusTest.filter(release_id=self.release.id).all()
+        groups: list[ArgusGroup] = ArgusGroup.filter(release_id=self.release.id).all()
         for group in groups:
             if group.enabled:
                 stats = GroupStats(group=group, parent_release=self)
                 stats.collect(limited=limited)
                 self.groups.append(stats)
 
     def increment_status(self, status=TestStatus.NOT_PLANNED):
         self.total_tests += 1
         self.status_map[TestStatus(status)] += 1
         self.last_status = TestStatus(status)
 
 
 class GroupStats:
-    def __init__(self, group: ArgusReleaseGroup, parent_release: ReleaseStats) -> None:
+    def __init__(self, group: ArgusGroup, parent_release: ReleaseStats) -> None:
         self.group = group
         self.parent_release = parent_release
         self.status_map = {status: 0 for status in TestStatus}
         self.total_tests = 0
         self.last_status = TestStatus.NOT_PLANNED
         self.last_investigation_status = TestInvestigationStatus.NOT_INVESTIGATED
         self.disabled = False
@@ -106,17 +173,17 @@
         self.last_status = TestStatus(status)
         self.parent_release.increment_status(status)
 
 
 class TestStats:
     def __init__(
         self,
-        test: ArgusReleaseGroupTest,
+        test: ArgusTest,
         parent_group: GroupStats,
-        schedules: list[ArgusReleaseScheduleTest] | None = None
+        schedules: list[ArgusScheduleTest] | None = None
     ) -> None:
         self.test = test
         self.parent_group = parent_group
         self.start_time = datetime.fromtimestamp(0)
         self.status = TestStatus.NOT_PLANNED
         self.investigation_status = TestInvestigationStatus.NOT_INVESTIGATED
         self.last_runs: list[dict] = []
@@ -132,57 +199,85 @@
             "investigation_status": self.investigation_status,
             "last_runs": self.last_runs,
             "start_time": self.start_time,
             "hasBugReport": self.has_bug_report,
             "hasComments": self.has_comments
         }
 
+    def _generate_status_map(self, last_runs: list[TestRunStatRow]) -> dict[int, str]:
+        status_map = {}
+        for run in last_runs:
+            run_number = self._get_build_number(run["build_job_url"])
+            match status := status_map.get(run_number):
+                case str():
+                    if ComparableTestStatus(TestStatus(status)) < ComparableTestStatus(TestStatus(run["status"])):
+                        status_map[run_number] = run["status"]
+                case _:
+                    status_map[run_number] = run["status"]
+        return status_map
+
+    @staticmethod
+    def _get_build_number(build_job_url: str) -> int | None:
+        build_number = build_job_url.rstrip("/").split("/")[-1]
+        if build_number:
+            try:
+                return int(build_number)
+            except ValueError:
+                LOGGER.error("Error parsing build number from %s: got %s as build_number", build_job_url, build_number)
+        return None
+
     def collect(self, limited=False):
 
-        last_runs = filter(lambda r: r["build_id"] == self.test.build_system_id, self.parent_group.parent_release.rows)
+        last_runs = [r for r in self.parent_group.parent_release.rows if r["build_id"] == self.test.build_system_id]
+        last_runs: list[TestRunStatRow] = sorted(
+            last_runs, reverse=True, key=lambda r: self._get_build_number(r["build_job_url"]))
         try:
-            last_run = next(last_runs)
-        except StopIteration:
+            last_run = last_runs[0]
+        except IndexError:
             self.status = TestStatus.NOT_RUN if self.is_scheduled else TestStatus.NOT_PLANNED
             self.parent_group.increment_status(status=self.status)
             return
+        status_map = self._generate_status_map(last_runs)
 
-        self.status = TestStatus(last_run["status"])
+        self.status = status_map.get(self._get_build_number(last_run["build_job_url"]))
         self.investigation_status = TestInvestigationStatus(last_run["investigation_status"])
         self.start_time = last_run["start_time"]
 
-        self.parent_group.increment_status(status=last_run["status"])
+        self.parent_group.increment_status(status=self.status)
         if limited and not self.parent_group.parent_release.forced_collection:
             return
 
         self.last_runs = [
             {
                 "status": run["status"],
-                "build_number": run["build_job_url"].rstrip("/").split("/")[-1],
+                "build_number": self._get_build_number(run["build_job_url"]),
                 "build_job_name": run["build_id"],
                 "start_time": run["start_time"],
                 "assignee": run["assignee"],
                 "issues": [dict(i.items()) for i in self.parent_group.parent_release.issues if i.run_id == run["id"]],
                 "comments": [dict(i.items()) for i in self.parent_group.parent_release.comments if i.test_run_id == run["id"]],
             }
-            for run in [last_run, *last_runs]
-        ][:4]
+            for run in last_runs
+        ][:5]
         self.has_bug_report = len(self.last_runs[0]["issues"]) > 0
         self.parent_group.parent_release.has_bug_report = self.has_bug_report or self.parent_group.parent_release.has_bug_report
         self.has_comments = len(self.last_runs[0]["comments"]) > 0
 
 
 class ReleaseStatsCollector:
     def __init__(self, release_name: str, release_version: str | None = None) -> None:
         self.database = ScyllaCluster.get()
         self.session = self.database.get_session()
         self.run_by_release_stats_statement = self.database.prepare(
             "SELECT id, test_id, group_id, release_id, status, start_time, build_job_url, build_id, assignee, "
-            f"end_time, investigation_status, heartbeat, scylla_version FROM {TestRun.table_name()} WHERE release_id = ?"
+            f"end_time, investigation_status, heartbeat, scylla_version FROM {SCTTestRun.table_name()} WHERE release_id = ?"
         )
+        self.release = None
+        self.release_stats = None
+        self.release_rows = []
         self.release_name = release_name
         self.release_version = release_version
 
     def collect(self, limited=False, force=False) -> dict:
         self.release: ArgusRelease = ArgusRelease.get(name=self.release_name)
         self.release_rows = self.session.execute(
             self.run_by_release_stats_statement, parameters=(self.release.id,)).all()
```

### Comparing `argus-alm-0.8.0/argus/db/cloud_types.py` & `argus-alm-0.8.1/argus/db/cloud_types.py`

 * *Files identical despite different names*

### Comparing `argus-alm-0.8.0/argus/db/config.py` & `argus-alm-0.8.1/argus/db/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,14 +32,18 @@
     def contact_points(self) -> list[str]:
         raise NotImplementedError()
 
     @property
     def keyspace_name(self) -> str:
         raise NotImplementedError()
 
+    @property
+    def address_mapping(self) -> dict:
+        return NotImplementedError()
+
 
 class FileConfig(BaseConfig):
     @property
     def username(self):
         return self.as_dict.get("username")
 
     @property
@@ -50,14 +54,18 @@
     def contact_points(self) -> list[str]:
         return self.as_dict.get("contact_points")
 
     @property
     def keyspace_name(self) -> str:
         return self.as_dict.get("keyspace_name")
 
+    @property
+    def address_mapping(self) -> dict:
+        return self.as_dict.get("address_mapping")
+
     DEFAULT_CONFIG_PATHS = (
         "./config/argus.local.yaml",
         "argus.local.yaml",
         "argus.yaml",
         getenv("HOME") + "/.argus.yaml"
     )
 
@@ -104,19 +112,24 @@
     def contact_points(self) -> list[str]:
         return self.as_dict.get("contact_points")
 
     @property
     def keyspace_name(self) -> str:
         return self.as_dict.get("keyspace_name")
 
-    def __init__(self, username: str, password: str, contact_points: list[str], keyspace_name: str):
+    @property
+    def address_mapping(self) -> dict:
+        return self.as_dict.get("address_mapping")
+
+    def __init__(self, username: str, password: str, contact_points: list[str], keyspace_name: str, address_mapping: dict | None = None):
         super().__init__()
         self._config = {
             "username": username,
             "password": password,
             "contact_points": contact_points,
             "keyspace_name": keyspace_name,
+            "address_mapping": address_mapping,
         }
 
     @property
     def as_dict(self) -> dict[Hashable, Any]:
         return self._config
```

### Comparing `argus-alm-0.8.0/argus/db/db_types.py` & `argus-alm-0.8.1/argus/db/db_types.py`

 * *Files identical despite different names*

### Comparing `argus-alm-0.8.0/argus/db/interface.py` & `argus-alm-0.8.1/argus/db/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# TODO: Deprecated, will be removed once REST API client is ready
 from datetime import datetime
 import re
 import logging
 import json
 from uuid import UUID
 from hashlib import sha1
 from dataclasses import fields as dataclass_fields
@@ -9,26 +10,26 @@
 from types import GenericAlias
 
 import cassandra.cluster
 import cassandra.cqltypes
 from cassandra import ConsistencyLevel
 from cassandra.auth import PlainTextAuthProvider
 from cassandra.query import named_tuple_factory
-from cassandra.policies import WhiteListRoundRobinPolicy
+from cassandra.policies import WhiteListRoundRobinPolicy, AddressTranslator
 from cassandra.cluster import ExecutionProfile, EXEC_PROFILE_DEFAULT
 from cassandra.cqlengine import connection
 from cassandra.cqlengine import models
 from cassandra.cqlengine import management
 from argus.db.argus_json import ArgusJSONEncoder
 
 from argus.db.config import BaseConfig, FileConfig
 from argus.db.db_types import ColumnInfo, CollectionHint, ArgusUDTBase
 from argus.db.cloud_types import ResourceState
-from argus.db.models import ArgusReleaseSchedule, ArgusReleaseScheduleAssignee, \
-    ArgusReleaseScheduleGroup, ArgusReleaseScheduleTest, ArgusRelease, ArgusReleaseGroup, ArgusReleaseGroupTest
+from argus.backend.models.web import ArgusSchedule, ArgusScheduleAssignee, \
+    ArgusScheduleGroup, ArgusScheduleTest, ArgusRelease, ArgusGroup, ArgusTest
 
 LOGGER = logging.getLogger(__name__)
 
 
 class ArgusInterfaceSingletonError(Exception):
     pass
 
@@ -41,25 +42,33 @@
     pass
 
 
 class ArgusInterfaceNameError(Exception):
     pass
 
 
+class PrivateToPublicAddressTranslator(AddressTranslator):
+    def __init__(self, address_mapping):
+        self.address_mapping = address_mapping
+
+    def translate(self, addr):
+        return self.address_mapping.get(addr, addr)
+
+
 class ArgusDatabase:
     # pylint: disable=too-many-instance-attributes
     CQL_ENGINE_CONNECTION_NAME = 'argus_cql_engine_conn'
     ARGUS_EXECUTION_PROFILE = "argus_named_tuple"
     REQUIRED_CQL_ENGINE_MODELS = [
-        ArgusReleaseSchedule,
-        ArgusReleaseScheduleGroup,
-        ArgusReleaseScheduleTest,
-        ArgusReleaseScheduleAssignee,
-        ArgusReleaseGroupTest,
-        ArgusReleaseGroup,
+        ArgusSchedule,
+        ArgusScheduleGroup,
+        ArgusScheduleTest,
+        ArgusScheduleAssignee,
+        ArgusTest,
+        ArgusGroup,
         ArgusRelease,
     ]
     PYTHON_SCYLLA_TYPE_MAPPING = {
         int: cassandra.cqltypes.IntegerType.typename,
         float: cassandra.cqltypes.FloatType.typename,
         str: cassandra.cqltypes.VarcharType.typename,
         UUID: cassandra.cqltypes.UUIDType.typename,
@@ -80,23 +89,28 @@
             consistency_level=ConsistencyLevel.QUORUM,
         )
         self.exec_profile_named_tuple = ExecutionProfile(
             load_balancing_policy=WhiteListRoundRobinPolicy(hosts=self.config.contact_points),
             consistency_level=ConsistencyLevel.QUORUM,
             row_factory=named_tuple_factory
         )
+        address_translator = None
+        if self.config.address_mapping:
+            address_translator = PrivateToPublicAddressTranslator(self.config.address_mapping)
+
         self.cluster = cassandra.cluster.Cluster(contact_points=self.config.contact_points,
                                                  protocol_version=4,
                                                  auth_provider=PlainTextAuthProvider(
                                                      username=self.config.username,
                                                      password=self.config.password),
                                                  execution_profiles={
                                                      EXEC_PROFILE_DEFAULT: self.execution_profile,
                                                      self.ARGUS_EXECUTION_PROFILE: self.exec_profile_named_tuple
-                                                 }
+                                                 },
+                                                 address_translator=address_translator,
                                                  )
         self.session = self.cluster.connect()
         self._keyspace_initialized = False
         self.prepared_statements = {}
         self.initialized_tables = {}
         self._table_keys = {}
         self._mapped_udts = {}
```

### Comparing `argus-alm-0.8.0/argus/db/models.py` & `argus-alm-0.8.1/argus/backend/models/web.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from uuid import UUID, uuid1, uuid4
 from datetime import datetime
 from enum import Enum, IntEnum, auto
 from cassandra.cqlengine.models import Model
-from cassandra.cqlengine.usertype import UserType
 from cassandra.cqlengine import columns
-from cassandra.util import uuid_from_time, unix_time_from_uuid1
-from cassandra.cqlengine.columns import UserDefinedType
+from cassandra.util import uuid_from_time, unix_time_from_uuid1  # pylint: disable=no-name-in-module
 
 
 def uuid_now():
     return uuid_from_time(datetime.utcnow())
 
 # pylint: disable=invalid-name
 
@@ -29,52 +27,59 @@
     username = columns.Text(index=True)
     full_name = columns.Text()
     password = columns.Text()
     email = columns.Text(index=True)
     registration_date = columns.DateTime()
     roles = columns.List(value_type=columns.Text)
     picture_id = columns.UUID(default=None)
+    api_token = columns.Text(index=True)
 
     def __hash__(self) -> int:
         return hash(self.id)
 
     def is_manager(self) -> bool:
+        # pylint: disable=unsupported-membership-test
         return UserRoles.Manager in self.roles
 
     def is_admin(self) -> bool:
+        # pylint: disable=unsupported-membership-test
         return UserRoles.Admin in self.roles
 
     def set_as_admin(self) -> None:
+        # pylint: disable=unsupported-membership-test
         if UserRoles.Admin not in self.roles:
             self.roles.append(UserRoles.Admin.value)
 
     def set_as_manager(self) -> None:
+        # pylint: disable=unsupported-membership-test
         if UserRoles.Manager not in self.roles:
             self.roles.append(UserRoles.Manager.value)
 
     def get_id(self):
         return str(self.id)
 
     @classmethod
     def exists(cls, user_id: UUID):
         try:
             user = cls.get(id=user_id)
             if user:
                 return user
         except cls.DoesNotExist:
-            return None
+            pass
+        return None
 
     @classmethod
     def exists_by_name(cls, name: str):
         try:
             user = cls.get(username=name)
             if user:
                 return user
         except cls.DoesNotExist:
-            return None
+            pass
+        return None
 
     def __str__(self):
         return f"User('{self.id}','{self.username}')"
 
     def to_json(self):
         return {
             "id": str(self.id),
@@ -107,65 +112,61 @@
     def __eq__(self, other):
         if isinstance(other, ArgusRelease):
             return self.name == other.name
         else:
             return super().__eq__(other)
 
 
-class ArgusReleaseGroup(Model):
+class ArgusGroup(Model):
     __table_name__ = "argus_group_v2"
     id = columns.UUID(primary_key=True, default=uuid4)
     release_id = columns.UUID(required=True, index=True)
     name = columns.Text(required=True, index=True)
     pretty_name = columns.Text()
     description = columns.Text()
     assignee = columns.List(value_type=columns.UUID)
     build_system_id = columns.Text()
     enabled = columns.Boolean(default=lambda: True)
 
     def __hash__(self) -> int:
         return hash((self.id, self.release_id))
 
     def __eq__(self, other):
-        if isinstance(other, ArgusReleaseGroup):
+        if isinstance(other, ArgusGroup):
             return self.name == other.name and self.release_id == other.release_id
         else:
             return super().__eq__(other)
 
 
-class ArgusReleaseGroupTest(Model):
+class ArgusTest(Model):
     __table_name__ = "argus_test_v2"
     id = columns.UUID(primary_key=True, default=uuid4)
     group_id = columns.UUID(required=True, index=True)
     release_id = columns.UUID(required=True, index=True)
     name = columns.Text(required=True, index=True)
     pretty_name = columns.Text()
     description = columns.Text()
     assignee = columns.List(value_type=columns.UUID)
     build_system_id = columns.Text(index=True)
     enabled = columns.Boolean(default=lambda: True)
     build_system_url = columns.Text()
 
     def __eq__(self, other):
-        if isinstance(other, ArgusReleaseGroupTest):
+        if isinstance(other, ArgusTest):
             return self.name == other.name and self.group_id == other.group_id and self.release_id == other.release_id
         else:
             return super().__eq__(other)
 
     def validate_build_system_id(self):
         try:
-            t = ArgusReleaseGroupTest.get(build_system_id=self.build_system_id)
+            t = ArgusTest.get(build_system_id=self.build_system_id)
             if t.id != self.id:
                 raise ArgusTestException("Build Id is already used by another test", t.id, self.id)
-        except ArgusReleaseGroupTest.DoesNotExist:
+        except ArgusTest.DoesNotExist:
             pass
-        except ArgusReleaseGroupTest.MultipleObjectsReturned:
-            raise
-
-        return
 
 
 class ArgusTestRunComment(Model):
     id = columns.UUID(primary_key=True, default=uuid4, partition_key=True)
     test_run_id = columns.UUID(required=True, index=True)
     user_id = columns.UUID(required=True, index=True)
     release_id = columns.UUID(required=True, index=True)
@@ -275,45 +276,45 @@
 
     def __eq__(self, other):
         if isinstance(other, ArgusGithubIssue):
             return self.owner == other.owner and self.repo == other.repo and self.issue_number == other.issue_number
         return super().__eq__(other)
 
     def __ne__(self, other):
-        return not(self == other)
+        return not self == other
 
 
-class ArgusReleaseSchedule(Model):
+class ArgusSchedule(Model):
     __table_name__ = "argus_schedule_v4"
     release_id = columns.UUID(primary_key=True, required=True)
     id = columns.TimeUUID(primary_key=True, default=uuid1, clustering_order="DESC")
     period_start = columns.DateTime(required=True, default=datetime.utcnow)
     period_end = columns.DateTime(required=True, primary_key=True, clustering_order="DESC")
     tag = columns.Text(default="")
 
 
-class ArgusReleaseScheduleAssignee(Model):
+class ArgusScheduleAssignee(Model):
     __table_name__ = "argus_schedule_user_v3"
     assignee = columns.UUID(primary_key=True)
     id = columns.TimeUUID(primary_key=True, default=uuid1,
                           clustering_order="DESC")
     schedule_id = columns.TimeUUID(required=True, index=True)
     release_id = columns.UUID(required=True)
 
 
-class ArgusReleaseScheduleTest(Model):
+class ArgusScheduleTest(Model):
     __table_name__ = "argus_schedule_test_v5"
     test_id = columns.UUID(primary_key=True, required=True)
     id = columns.TimeUUID(primary_key=True, default=uuid1,
                           clustering_order="DESC")
     schedule_id = columns.TimeUUID(required=True, index=True)
     release_id = columns.UUID(partition_key=True)
 
 
-class ArgusReleaseScheduleGroup(Model):
+class ArgusScheduleGroup(Model):
     __table_name__ = "argus_schedule_group_v3"
     group_id = columns.UUID(partition_key=True, required=True)
     id = columns.TimeUUID(primary_key=True, default=uuid1,
                           clustering_order="DESC")
     schedule_id = columns.TimeUUID(required=True, index=True)
     release_id = columns.UUID(partition_key=True)
 
@@ -330,13 +331,13 @@
     id = columns.UUID(primary_key=True, default=uuid4)
     filepath = columns.Text(min_length=1)
     filename = columns.Text(min_length=1)
 
 
 USED_MODELS = [
     User, UserOauthToken,
-    ArgusRelease, ArgusReleaseGroup, ArgusReleaseGroupTest,
+    ArgusRelease, ArgusGroup, ArgusTest,
     ArgusTestRunComment, ArgusEvent,
     WebFileStorage, ArgusGithubIssue, ReleasePlannerComment, ArgusNotification,
-    ArgusReleaseSchedule, ArgusReleaseScheduleAssignee, ArgusReleaseScheduleGroup, ArgusReleaseScheduleTest
+    ArgusSchedule, ArgusScheduleAssignee, ArgusScheduleGroup, ArgusScheduleTest
 ]
 USED_TYPES = []
```

### Comparing `argus-alm-0.8.0/argus/db/testrun.py` & `argus-alm-0.8.1/argus/db/testrun.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# TODO: Deprecated, will be removed once REST API client is ready
 import logging
 import datetime
 import time
 import traceback
 import sys
 import threading
 from dataclasses import asdict, is_dataclass, fields, Field, dataclass
@@ -10,16 +11,16 @@
 
 from argus.db.config import BaseConfig
 from argus.db.utils import is_list_homogeneous
 from argus.db.cloud_types import CloudResource, CloudInstanceDetails, BaseCloudSetupDetails
 from argus.db.interface import ArgusDatabase
 from argus.db.db_types import ColumnInfo, CollectionHint, NemesisRunInfo, TestStatus, TestInvestigationStatus, \
     EventsBySeverity, PackageVersion
-from argus.db.models import ArgusRelease, ArgusReleaseGroup, ArgusReleaseGroupTest, ArgusReleaseSchedule, ArgusReleaseScheduleAssignee, ArgusReleaseScheduleGroup, \
-    ArgusReleaseScheduleTest
+from argus.backend.models.web import ArgusRelease, ArgusGroup, ArgusTest, ArgusSchedule, ArgusScheduleAssignee, ArgusScheduleGroup, \
+    ArgusScheduleTest
 
 LOGGER = logging.getLogger(__name__)
 
 
 class TestInfoSerializationError(Exception):
     pass
 
@@ -605,54 +606,54 @@
         if self.argus.fetch(table_name=self._TABLE_NAME, run_id=self.id):
             return True
         return False
 
     def _assign_categories(self):
         key = self._build_id
         try:
-            test: ArgusReleaseGroupTest = ArgusReleaseGroupTest.using(
+            test: ArgusTest = ArgusTest.using(
                 connection=self.argus.CQL_ENGINE_CONNECTION_NAME
             ).get(build_system_id=key)
             self.release_id = test.release_id
             self.group_id = test.group_id
             self.test_id = test.id
-        except ArgusReleaseGroupTest.DoesNotExist:
+        except ArgusTest.DoesNotExist:
             LOGGER.warning(
                 "Test entity missing for key \"%s\", run won't be visible until this is corrected", key)
 
     def _get_current_assignee_from_schedule(self) -> UUID:
         """
             Iterate over all schedules (groups and tests) and return first available assignee
         """
-        associated_test = ArgusReleaseGroupTest.using(
+        associated_test = ArgusTest.using(
             connection=self.argus.CQL_ENGINE_CONNECTION_NAME
         ).get(build_system_id=self.build_id)
-        associated_group = ArgusReleaseGroup.using(
+        associated_group = ArgusGroup.using(
             connection=self.argus.CQL_ENGINE_CONNECTION_NAME
         ).get(id=associated_test.group_id)
         associated_release = ArgusRelease.using(
             connection=self.argus.CQL_ENGINE_CONNECTION_NAME
         ).get(id=associated_test.release_id)
 
-        scheduled_groups = ArgusReleaseScheduleGroup.filter(
+        scheduled_groups = ArgusScheduleGroup.filter(
             release_id=associated_release.id, group_id=associated_group.id
         ).all().using(
             connection=self.argus.CQL_ENGINE_CONNECTION_NAME
         )
 
-        scheduled_tests = ArgusReleaseScheduleTest.filter(
+        scheduled_tests = ArgusScheduleTest.filter(
             release_id=associated_release.id, test_id=associated_test.id
         ).all().using(
             connection=self.argus.CQL_ENGINE_CONNECTION_NAME
         )
 
         unique_schedule_ids = {scheduled_obj.schedule_id for scheduled_obj in [
             *scheduled_tests, *scheduled_groups]}
 
-        schedules = ArgusReleaseSchedule.filter(
+        schedules = ArgusSchedule.filter(
             release_id=associated_release.id, id__in=tuple(
                 unique_schedule_ids)
         ).all().using(
             connection=self.argus.CQL_ENGINE_CONNECTION_NAME
         )
 
         today = datetime.datetime.utcnow()
@@ -660,15 +661,15 @@
         valid_schedules = []
         for schedule in schedules:
             if schedule.period_start <= today <= schedule.period_end:
                 valid_schedules.append(schedule)
 
         assignees_uuids = []
         for schedule in valid_schedules:
-            assignees = ArgusReleaseScheduleAssignee.filter(
+            assignees = ArgusScheduleAssignee.filter(
                 schedule_id=schedule.id
             ).all().using(
                 connection=self.argus.CQL_ENGINE_CONNECTION_NAME
             )
             assignees_uuids.append(
                 *[assignee.assignee for assignee in assignees])
```

### Comparing `argus-alm-0.8.0/pyproject.toml` & `argus-alm-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "argus-alm"
-version = "0.8.0"
+version = "0.8.1"
 description = "Argus"
 authors = ["Alexey Kartashov <alexey.kartashov@scylladb.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/scylladb/argus"
 readme = "README.md"
 packages = [{include = "argus"}]
```

