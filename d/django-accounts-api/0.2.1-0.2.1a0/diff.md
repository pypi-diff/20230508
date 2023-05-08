# Comparing `tmp/django_accounts_api-0.2.1.tar.gz` & `tmp/django_accounts_api-0.2.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_accounts_api-0.2.1.tar", max compression
+gzip compressed data, was "django_accounts_api-0.2.1a0.tar", max compression
```

## Comparing `django_accounts_api-0.2.1.tar` & `django_accounts_api-0.2.1a0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1204 2023-01-06 05:27:06.379634 django_accounts_api-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-01-05 07:41:34.771966 django_accounts_api-0.2.1/django_accounts_api/__init__.py
--rw-r--r--   0        0        0     2838 2023-04-25 07:23:55.980264 django_accounts_api-0.2.1/django_accounts_api/api_login_tests.py
--rw-r--r--   0        0        0     4437 2023-01-18 05:07:02.825752 django_accounts_api-0.2.1/django_accounts_api/api_password_change_tests.py
--rw-r--r--   0        0        0      159 2023-01-05 07:41:34.772082 django_accounts_api-0.2.1/django_accounts_api/apps.py
--rw-r--r--   0        0        0     5650 2023-04-25 07:23:55.980588 django_accounts_api-0.2.1/django_accounts_api/login_logout_tests.py
--rw-r--r--   0        0        0      621 2023-04-25 07:23:55.981861 django_accounts_api-0.2.1/django_accounts_api/manifest_tests.py
--rw-r--r--   0        0        0        0 2023-01-05 07:41:34.772396 django_accounts_api-0.2.1/django_accounts_api/migrations/__init__.py
--rw-r--r--   0        0        0     1844 2023-01-18 05:07:02.826459 django_accounts_api-0.2.1/django_accounts_api/password_change_tests.py
--rw-r--r--   0        0        0     2059 2023-03-22 04:20:55.389597 django_accounts_api-0.2.1/django_accounts_api/password_reset_confirm_tests.py
--rw-r--r--   0        0        0     1279 2023-04-25 07:23:55.982805 django_accounts_api-0.2.1/django_accounts_api/password_reset_tests.py
--rw-r--r--   0        0        0       18 2023-01-06 05:27:06.380468 django_accounts_api-0.2.1/django_accounts_api/templates/django_accounts_api/login.html
--rw-r--r--   0        0        0       18 2023-01-06 05:27:06.380624 django_accounts_api-0.2.1/django_accounts_api/templates/django_accounts_api/password_change.html
--rw-r--r--   0        0        0       47 2023-03-22 04:20:55.396743 django_accounts_api-0.2.1/django_accounts_api/templates/django_accounts_api/password_reset.html
--rw-r--r--   0        0        0       18 2023-03-22 04:12:48.577885 django_accounts_api-0.2.1/django_accounts_api/templates/django_accounts_api/password_reset_confirm.html
--rw-r--r--   0        0        0      575 2023-04-25 07:23:29.040141 django_accounts_api-0.2.1/django_accounts_api/templates/registration/password_reset_email.html
--rw-r--r--   0        0        0      828 2023-04-25 07:23:55.983039 django_accounts_api-0.2.1/django_accounts_api/urls.py
--rw-r--r--   0        0        0    10983 2023-04-25 07:23:55.983314 django_accounts_api-0.2.1/django_accounts_api/views.py
--rw-r--r--   0        0        0      793 2023-04-25 08:20:38.730233 django_accounts_api-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1813 1970-01-01 00:00:00.000000 django_accounts_api-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1204 2023-01-06 05:27:06.379634 django_accounts_api-0.2.1a0/README.md
+-rw-r--r--   0        0        0        0 2023-01-05 07:41:34.771966 django_accounts_api-0.2.1a0/django_accounts_api/__init__.py
+-rw-r--r--   0        0        0     2870 2023-05-04 17:45:05.326778 django_accounts_api-0.2.1a0/django_accounts_api/api_login_tests.py
+-rw-r--r--   0        0        0     4437 2023-01-18 05:07:02.825752 django_accounts_api-0.2.1a0/django_accounts_api/api_password_change_tests.py
+-rw-r--r--   0        0        0      159 2023-01-05 07:41:34.772082 django_accounts_api-0.2.1a0/django_accounts_api/apps.py
+-rw-r--r--   0        0        0     5657 2023-05-04 17:45:05.327197 django_accounts_api-0.2.1a0/django_accounts_api/login_logout_tests.py
+-rw-r--r--   0        0        0      622 2023-05-04 17:45:05.327716 django_accounts_api-0.2.1a0/django_accounts_api/manifest_tests.py
+-rw-r--r--   0        0        0        0 2023-01-05 07:41:34.772396 django_accounts_api-0.2.1a0/django_accounts_api/migrations/__init__.py
+-rw-r--r--   0        0        0     1844 2023-01-18 05:07:02.826459 django_accounts_api-0.2.1a0/django_accounts_api/password_change_tests.py
+-rw-r--r--   0        0        0     2059 2023-03-22 04:20:55.389597 django_accounts_api-0.2.1a0/django_accounts_api/password_reset_confirm_tests.py
+-rw-r--r--   0        0        0     1277 2023-05-04 17:45:05.328756 django_accounts_api-0.2.1a0/django_accounts_api/password_reset_tests.py
+-rw-r--r--   0        0        0       18 2023-01-06 05:27:06.380468 django_accounts_api-0.2.1a0/django_accounts_api/templates/django_accounts_api/login.html
+-rw-r--r--   0        0        0       18 2023-01-06 05:27:06.380624 django_accounts_api-0.2.1a0/django_accounts_api/templates/django_accounts_api/password_change.html
+-rw-r--r--   0        0        0       47 2023-03-22 04:20:55.396743 django_accounts_api-0.2.1a0/django_accounts_api/templates/django_accounts_api/password_reset.html
+-rw-r--r--   0        0        0       18 2023-03-22 04:12:48.577885 django_accounts_api-0.2.1a0/django_accounts_api/templates/django_accounts_api/password_reset_confirm.html
+-rw-r--r--   0        0        0      575 2023-04-25 07:23:29.040141 django_accounts_api-0.2.1a0/django_accounts_api/templates/registration/password_reset_email.html
+-rw-r--r--   0        0        0      906 2023-05-04 17:45:05.329485 django_accounts_api-0.2.1a0/django_accounts_api/urls.py
+-rw-r--r--   0        0        0    10860 2023-05-04 17:45:05.329864 django_accounts_api-0.2.1a0/django_accounts_api/views.py
+-rw-r--r--   0        0        0      714 2023-05-08 07:26:10.221458 django_accounts_api-0.2.1a0/pyproject.toml
+-rw-r--r--   0        0        0     1679 1970-01-01 00:00:00.000000 django_accounts_api-0.2.1a0/PKG-INFO
```

### Comparing `django_accounts_api-0.2.1/README.md` & `django_accounts_api-0.2.1a0/README.md`

 * *Files identical despite different names*

### Comparing `django_accounts_api-0.2.1/django_accounts_api/api_login_tests.py` & `django_accounts_api-0.2.1a0/django_accounts_api/api_login_tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from django.forms import Form
 from django.test import TestCase
 from django.urls import reverse
 from django.contrib.auth import get_user_model
 
 User = get_user_model()
 
 
@@ -11,23 +12,23 @@
     def setUp(self) -> None:
         """Get the url and create a user"""
         self.url = reverse("django_accounts_api:login")
         self.user = User.objects.create_user("test", password="test")
         return super().setUp()
 
     def test_json_login_get_unauthed(self):
-        """An unauthed get with accept json should return a 204"""
+        """An unauthed get with accept json should return a 401"""
         response = self.client.get(
             self.url,
             HTTP_ACCEPT='application/json'
         )
-        assert response.status_code == 204
+        assert response.status_code == 401
 
     def test_json_login_get_authed(self):
-        """An authed get with accept json should return a 200"""
+        """An unauthed get with accept json should return a 401"""
         self.client.force_login(self.user)
         response = self.client.get(
             self.url,
             HTTP_ACCEPT='application/json'
         )
         assert response.status_code == 200
```

### Comparing `django_accounts_api-0.2.1/django_accounts_api/api_password_change_tests.py` & `django_accounts_api-0.2.1a0/django_accounts_api/api_password_change_tests.py`

 * *Files identical despite different names*

### Comparing `django_accounts_api-0.2.1/django_accounts_api/login_logout_tests.py` & `django_accounts_api-0.2.1a0/django_accounts_api/login_logout_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     def test_get_logout(self):
         """Just getting this endpoint with no login should return 200"""
         response = self.client.get(self.url)
         assert response.status_code == 200
 
     def test_post_logout(self):
         """posting to this endpoint with login should return 200"""
-        self.client.force_login(self.user)
+        test = self.client.force_login(self.user)
         response = self.client.post(self.url)
         assert response.status_code == 200
 
 
 class LoginViewTestCase(TestCase):
     """Basic tests of the partial HTML login view"""
```

### Comparing `django_accounts_api-0.2.1/django_accounts_api/manifest_tests.py` & `django_accounts_api-0.2.1a0/django_accounts_api/manifest_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from django.test import TestCase
 from django.urls import reverse
 
 
+
 class ManifestTestCase(TestCase):
     """Basic tests of the manifest"""
 
     def setUp(self) -> None:
         """Get the url and create a user"""
         self.url = reverse("django_accounts_api:manifest")
         return super().setUp()
```

### Comparing `django_accounts_api-0.2.1/django_accounts_api/password_change_tests.py` & `django_accounts_api-0.2.1a0/django_accounts_api/password_change_tests.py`

 * *Files identical despite different names*

### Comparing `django_accounts_api-0.2.1/django_accounts_api/password_reset_confirm_tests.py` & `django_accounts_api-0.2.1a0/django_accounts_api/password_reset_confirm_tests.py`

 * *Files identical despite different names*

### Comparing `django_accounts_api-0.2.1/django_accounts_api/password_reset_tests.py` & `django_accounts_api-0.2.1a0/django_accounts_api/password_reset_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from django.test import TestCase
 from django.urls import reverse
 from django.contrib.auth import get_user_model
 
 User = get_user_model()
 test_user_email = "admin@admin.com"
 
-
 class PasswordResetTestCase(TestCase):
     """Basic tests of the partial HTML password reset view"""
 
     def setUp(self) -> None:
         """Get the url and create a user"""
         self.url = reverse("django_accounts_api:password_reset")
-        self.user = User.objects.create_user("test", password="test", email=test_user_email)
+        self.user = User.objects.create_user("test", password="test",email=test_user_email)
         return super().setUp()
 
     def test_passwordreset_get(self):
         """An unauthed get should get a 200 and a form"""
         response = self.client.get(self.url)
         assert response.status_code == 200
         assert "form" in response.context
```

### Comparing `django_accounts_api-0.2.1/django_accounts_api/templates/registration/password_reset_email.html` & `django_accounts_api-0.2.1a0/django_accounts_api/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `django_accounts_api-0.2.1/django_accounts_api/urls.py` & `django_accounts_api-0.2.1a0/django_accounts_api/urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from django.urls import path
+from django.contrib.auth import views as auth_views
 from .views import (
     Login,
     Logout,
     PasswordChange,
     PasswordReset,
     PasswordResetConfirmView,
+    PasswordResetConfirm,
     PasswordResetComplete,
     login_check,
     manifest
 )
 
 app_name = 'django_accounts_api'
 urlpatterns = [
```

### Comparing `django_accounts_api-0.2.1/django_accounts_api/views.py` & `django_accounts_api-0.2.1a0/django_accounts_api/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from http import HTTPStatus
 from typing import Any
 from django.views.generic import View
 from django.contrib.auth.models import User as DjangoUser
 from django.contrib.auth import get_user_model
 from django.contrib.auth.views import LoginView, LogoutView, PasswordChangeView, PasswordResetView, PasswordResetCompleteView, PasswordResetConfirmView
 from django.urls.exceptions import NoReverseMatch
 from django.http import HttpRequest, HttpResponse, JsonResponse
 from django.urls import reverse
 from django.utils.decorators import method_decorator
-from django.views.decorators.csrf import csrf_protect, ensure_csrf_cookie
+from django.utils.translation import gettext_lazy as _
+from django.views.decorators.csrf import csrf_protect
 from django.views.decorators.debug import sensitive_post_parameters
 
 
 class AcceptJsonMixin:
     """
     Adds method to detect if JSON was requested in the Accept header
     """
@@ -56,25 +56,24 @@
     user: DjangoUser = request.user
     if (user.is_authenticated):
         return JsonResponse(_user_details(user))
     else:
         return HttpResponse(status=401)
 
 
-@method_decorator(ensure_csrf_cookie, name='get')
 @method_decorator(sensitive_post_parameters(), name='dispatch')
 class Login(AcceptJsonMixin, LoginView):
     '''
     Override the Django login view to be API friendly for json or partial html
     '''
     template_name = "django_accounts_api/login.html"
 
     def form_valid(self, form):
         """Override redirect behavior to return JSON user details"""
-        _repressed_redirect = super().form_valid(form)  # noqa: F841
+        _repressed_redirect = super().form_valid(form)
         return JsonResponse(
             _user_details(self.request.user),
             status=201
         )
 
     def form_invalid(self, form):
         """Override redirect behavior if json is requested return json errors"""
@@ -85,27 +84,27 @@
 
     def get(self, request: HttpRequest, *args: str, **kwargs: Any) -> HttpResponse:
         """Override the get behavior if json requested return user details"""
         if self.json_response_requested():
             if (request.user.is_authenticated):
                 return JsonResponse(_user_details(request.user))
             else:
-                return JsonResponse({}, status=HTTPStatus.NO_CONTENT)
+                return HttpResponse(status=401)
         else:
             return super().get(request, *args, **kwargs)
 
 
 class Logout(LogoutView):
     ''' Override the Django logout view to NOT redirect on successful login
     GET - actually calls POST, but will error in Django 5
     POST - logs out, returns 200
     '''
 
     def post(self, request, *args, **kwargs):
-        _repressed_redirect_or_render = super().post(request, *args, **kwargs)  # noqa: F841
+        _repressed_redirect_or_render = super().post(request, *args, **kwargs)
         return HttpResponse(
             status=200
         )
 
 
 @method_decorator(sensitive_post_parameters(), name='dispatch')
 @method_decorator(csrf_protect, name='dispatch')
@@ -141,15 +140,15 @@
         if self.json_response_requested():
             return JsonResponse(dict(errors=form.errors), status=400)
         else:
             return super().form_invalid(form)
 
     def form_valid(self, form):
         try:
-            _repressed_redirect = super().form_valid(form)  # noqa: F841
+            _repressed_redirect = super().form_valid(form)
         except NoReverseMatch:
             pass
         return HttpResponse(status=200)
 
 
 @method_decorator(sensitive_post_parameters(), name='dispatch')
 @method_decorator(csrf_protect, name='dispatch')
@@ -216,15 +215,15 @@
             return JsonResponse(dict(errors=form.errors), status=400)
         else:
             return super().form_invalid(form)
 
     def form_valid(self, form):
         """Override form_valid method to return HttpResponse with status code"""
         try:
-            _repressed_redirect = super().form_valid(form)  # noqa: F841
+            _repressed_redirect = super().form_valid(form)
         except NoReverseMatch:
             pass
         return HttpResponse(status=200)
 
 
 @method_decorator(sensitive_post_parameters(), name='dispatch')
 @method_decorator(csrf_protect, name='dispatch')
@@ -262,19 +261,18 @@
         If the form is invalid, re-render the context data with the
         data-filled form and errors.
         """
         if self.json_response_requested():
             return JsonResponse({'errors': form.errors}, status=400)
         return super().form_invalid(form)
 
-
 class PasswordResetComplete(PasswordResetCompleteView):
     """
     Custom PasswordResetCompleteView to support API use
     """
     template_name = 'password_reset_complete.html'
 
     def render_to_response(self, context, **response_kwargs):
         if self.json_response_requested():
             return JsonResponse({'message': 'Password reset successful.'}, status=200)
         else:
-            return super().render_to_response(context, **response_kwargs)
+            return super().render_to_response(context, **response_kwargs)
```

### Comparing `django_accounts_api-0.2.1/pyproject.toml` & `django_accounts_api-0.2.1a0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 [tool.poetry]
 name = "django-accounts-api"
-version = "0.2.1"
+version = "0.2.1a0"
 description = ""
 authors = ["PeteCoward <peter@catalpa.io>"]
 readme = "README.md"
 packages = [{include = "django_accounts_api"}]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-django = [
-    {python = "<3.8", version = ">=3.2"},
-    {python = ">=3.8", version = ">=3.2 <4.2"}
-]
+python = ">=3.8,<4.0"
+django = "4.2"
 
 [tool.poetry.group.tox.dependencies]
 tox = "^4.0.16"
 
 [tool.poetry.group.test.dependencies]
 pytest-django = "^4.5.2"
 pytest-cov = "^4.0.0"
```

### Comparing `django_accounts_api-0.2.1/PKG-INFO` & `django_accounts_api-0.2.1a0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: django-accounts-api
-Version: 0.2.1
+Version: 0.2.1a0
 Summary: 
 Author: PeteCoward
 Author-email: peter@catalpa.io
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: django (>=3.2) ; python_version < "3.8"
-Requires-Dist: django (>=3.2,<4.2) ; python_version >= "3.8"
+Requires-Dist: django (==4.2)
 Description-Content-Type: text/markdown
 
 # Django Accounts API
 
 Scenario to support is a compiled javascript capable frontend needing to provide authentication features over api
 
 Caveat enptor, very early days, still being tested in it's first project
```

