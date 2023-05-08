# Comparing `tmp/django_fragments-0.0.1.tar.gz` & `tmp/django_fragments-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_fragments-0.0.1.tar", max compression
+gzip compressed data, was "django_fragments-0.0.2.tar", max compression
```

## Comparing `django_fragments-0.0.1.tar` & `django_fragments-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1361 2023-05-08 11:12:44.134573 django_fragments-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-05-07 21:19:46.006724 django_fragments-0.0.1/django_fragments/__init__.py
--rw-r--r--   0        0        0      163 2023-05-08 11:11:49.135944 django_fragments-0.0.1/django_fragments/apps.py
--rw-r--r--   0        0        0      292 2023-05-07 15:19:00.977243 django_fragments-0.0.1/django_fragments/templates/svg/heroicons_x_mark_mini.html
--rw-r--r--   0        0        0        0 2023-05-07 23:31:34.843055 django_fragments-0.0.1/django_fragments/templatetags/__init__.py
--rw-r--r--   0        0        0     9728 2023-05-08 11:06:35.869723 django_fragments-0.0.1/django_fragments/templatetags/fragments.py
--rw-r--r--   0        0        0     2559 2023-05-08 09:31:53.991102 django_fragments-0.0.1/django_fragments/templatetags/og.py
--rw-r--r--   0        0        0       70 2023-05-08 02:09:45.909742 django_fragments-0.0.1/django_fragments/templatetags/utils/__init__.py
--rw-r--r--   0        0        0     2157 2023-05-08 02:17:55.382358 django_fragments-0.0.1/django_fragments/templatetags/utils/filter_attrs.py
--rw-r--r--   0        0        0     4146 2023-05-08 08:19:35.581999 django_fragments-0.0.1/django_fragments/templatetags/utils/wrap_svg.py
--rw-r--r--   0        0        0     2463 2023-05-08 02:19:36.975224 django_fragments-0.0.1/django_fragments/tests.py
--rw-r--r--   0        0        0     1366 2023-05-08 08:19:18.571245 django_fragments-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2176 1970-01-01 00:00:00.000000 django_fragments-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1361 2023-05-08 11:12:44.134573 django_fragments-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-07 21:19:46.006724 django_fragments-0.0.2/django_fragments/__init__.py
+-rw-r--r--   0        0        0      163 2023-05-08 11:11:49.135944 django_fragments-0.0.2/django_fragments/apps.py
+-rw-r--r--   0        0        0      292 2023-05-07 15:19:00.977243 django_fragments-0.0.2/django_fragments/templates/svg/heroicons_x_mark_mini.html
+-rw-r--r--   0        0        0        0 2023-05-07 23:31:34.843055 django_fragments-0.0.2/django_fragments/templatetags/__init__.py
+-rw-r--r--   0        0        0     9728 2023-05-08 12:19:35.043053 django_fragments-0.0.2/django_fragments/templatetags/fragments.py
+-rw-r--r--   0        0        0     2559 2023-05-08 09:31:53.991102 django_fragments-0.0.2/django_fragments/templatetags/og.py
+-rw-r--r--   0        0        0       70 2023-05-08 02:09:45.909742 django_fragments-0.0.2/django_fragments/templatetags/utils/__init__.py
+-rw-r--r--   0        0        0     2157 2023-05-08 02:17:55.382358 django_fragments-0.0.2/django_fragments/templatetags/utils/filter_attrs.py
+-rw-r--r--   0        0        0     4146 2023-05-08 08:19:35.581999 django_fragments-0.0.2/django_fragments/templatetags/utils/wrap_svg.py
+-rw-r--r--   0        0        0     2463 2023-05-08 02:19:36.975224 django_fragments-0.0.2/django_fragments/tests.py
+-rw-r--r--   0        0        0     1366 2023-05-08 12:31:15.447840 django_fragments-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2176 1970-01-01 00:00:00.000000 django_fragments-0.0.2/PKG-INFO
```

### Comparing `django_fragments-0.0.1/README.md` & `django_fragments-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django_fragments-0.0.1/django_fragments/templatetags/fragments.py` & `django_fragments-0.0.2/django_fragments/templatetags/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         SafeString: A partial template tag representing a button.
     """  # noqa: E501
     return mark_safe(
         Template("""
         {% load i18n fragments %}
         {% whitespaceless %}
         <div {% if parent_class %}class="{{parent_class}}"{% endif %}>
-            <button {% if css %}class="btn {{css}}"{% endif %}
+            <button class="btn {% if css %}{{css}}{% endif %}"
                 {% for k, v in aria_attrs.items %}{{k}}="{{v}}"{% endfor %}
                 {% for k, v in data_attrs.items %}{{k}}="{{v}}"{% endfor %}
                 {% for k, v in btn_attrs.items %}{{k}}="{{v}}"{% endfor %}
                 {% for k, v in hx_attrs.items %}{{k}}="{{v}}"{% endfor %}>
                 {% trans text %}
             </button>
         </div>
@@ -171,15 +171,15 @@
         Template("""
         {% load i18n fragments %}
         {% whitespaceless %}
         <a type="button"
             {% for k, v in a_attrs.items %}{{k}}="{{v}}"{% endfor %}
             {% for k, v in aria_attrs.items %}{{k}}="{{v}}"{% endfor %}
             {% for k, v in data_attrs.items %}{{k}}="{{v}}"{% endfor %}
-            {% if css %}class="btn {{css}}"{% endif %}
+            class="btn {% if css %}{{css}}{% endif %}"
         >{% trans text %}</a>
         {% endwhitespaceless %}
         """)
         .render(
             context=Context(
                 {
                     "text": text,
```

### Comparing `django_fragments-0.0.1/django_fragments/templatetags/og.py` & `django_fragments-0.0.2/django_fragments/templatetags/og.py`

 * *Files identical despite different names*

### Comparing `django_fragments-0.0.1/django_fragments/templatetags/utils/filter_attrs.py` & `django_fragments-0.0.2/django_fragments/templatetags/utils/filter_attrs.py`

 * *Files identical despite different names*

### Comparing `django_fragments-0.0.1/django_fragments/templatetags/utils/wrap_svg.py` & `django_fragments-0.0.2/django_fragments/templatetags/utils/wrap_svg.py`

 * *Files identical despite different names*

### Comparing `django_fragments-0.0.1/django_fragments/tests.py` & `django_fragments-0.0.2/django_fragments/tests.py`

 * *Files identical despite different names*

### Comparing `django_fragments-0.0.1/pyproject.toml` & `django_fragments-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "django-fragments"
 description = "Custom template tags for common html idioms in Django, e.g. button, svg, etc."
-version = "0.0.1"
+version = "0.0.2"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/django-fragments"
 documentation = "https://mv3.dev/django-fragments"
 classifiers = [
   "Programming Language :: Python :: 3.11",
```

### Comparing `django_fragments-0.0.1/PKG-INFO` & `django_fragments-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-fragments
-Version: 0.0.1
+Version: 0.0.2
 Summary: Custom template tags for common html idioms in Django, e.g. button, svg, etc.
 Home-page: https://mv3.dev
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
```

