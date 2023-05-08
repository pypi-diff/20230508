# Comparing `tmp/django-easy-faq-1.5.tar.gz` & `tmp/django-easy-faq-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-easy-faq-1.5.tar", last modified: Tue Feb 14 03:20:44 2023, max compression
+gzip compressed data, was "django-easy-faq-1.6.tar", last modified: Mon May  8 00:49:20 2023, max compression
```

## Comparing `django-easy-faq-1.5.tar` & `django-easy-faq-1.6.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-02-14 03:20:44.059645 django-easy-faq-1.5/
--rw-rw-rw-   0        0        0     1089 2023-02-14 02:47:58.000000 django-easy-faq-1.5/LICENSE.txt
--rw-rw-rw-   0        0        0      108 2023-02-14 02:47:58.000000 django-easy-faq-1.5/MANIFEST.in
--rw-rw-rw-   0        0        0    15061 2023-02-14 03:20:44.059645 django-easy-faq-1.5/PKG-INFO
--rw-rw-rw-   0        0        0    14084 2023-02-14 03:17:24.000000 django-easy-faq-1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-02-14 03:20:44.028133 django-easy-faq-1.5/django_easy_faq.egg-info/
--rw-rw-rw-   0        0        0    15061 2023-02-14 03:20:43.000000 django-easy-faq-1.5/django_easy_faq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1024 2023-02-14 03:20:43.000000 django-easy-faq-1.5/django_easy_faq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-14 03:20:43.000000 django-easy-faq-1.5/django_easy_faq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-02-14 03:20:43.000000 django-easy-faq-1.5/django_easy_faq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-02-14 03:20:43.000000 django-easy-faq-1.5/django_easy_faq.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-14 03:20:44.043142 django-easy-faq-1.5/faq/
--rw-rw-rw-   0        0        0       41 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/__init__.py
--rw-rw-rw-   0        0        0     2118 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/admin.py
--rw-rw-rw-   0        0        0      170 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/apps.py
--rw-rw-rw-   0        0        0      969 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/forms.py
-drwxrwxrwx   0        0        0        0 2023-02-14 03:20:44.053440 django-easy-faq-1.5/faq/migrations/
--rw-rw-rw-   0        0        0     4220 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1543 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/migrations/0002_alter_answer_id_alter_answerhelpful_id_and_more.py
--rw-rw-rw-   0        0        0      455 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/migrations/0003_auto_20220619_0939.py
--rw-rw-rw-   0        0        0      576 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/migrations/0004_alter_answer_slug_alter_category_slug.py
--rw-rw-rw-   0        0        0        0 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/migrations/__init__.py
--rw-rw-rw-   0        0        0     4385 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/models.py
--rw-rw-rw-   0        0        0      346 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/path_converters.py
--rw-rw-rw-   0        0        0     2476 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/snippets.py
-drwxrwxrwx   0        0        0        0 2023-02-14 03:20:44.007774 django-easy-faq-1.5/faq/templates/
-drwxrwxrwx   0        0        0        0 2023-02-14 03:20:44.059645 django-easy-faq-1.5/faq/templates/faq/
--rw-rw-rw-   0        0        0      342 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/templates/faq/answer_form.html
--rw-rw-rw-   0        0        0      242 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/templates/faq/base.html
--rw-rw-rw-   0        0        0      421 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/templates/faq/categories_list.html
--rw-rw-rw-   0        0        0      633 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/templates/faq/category_detail.html
--rw-rw-rw-   0        0        0      281 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/templates/faq/comment_form.html
--rw-rw-rw-   0        0        0      758 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/templates/faq/comments.html
--rw-rw-rw-   0        0        0     1264 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/templates/faq/question_base.html
--rw-rw-rw-   0        0        0     2877 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/templates/faq/question_detail.html
--rw-rw-rw-   0        0        0      264 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/templates/faq/question_form.html
--rw-rw-rw-   0        0        0      434 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/templates/faq/questions_list.html
--rw-rw-rw-   0        0        0      262 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/templates/faq/vote_form.html
--rw-rw-rw-   0        0        0     7564 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/tests.py
--rw-rw-rw-   0        0        0     2206 2023-02-14 03:11:28.000000 django-easy-faq-1.5/faq/urls.py
--rw-rw-rw-   0        0        0    12821 2023-02-14 02:47:58.000000 django-easy-faq-1.5/faq/views.py
--rw-rw-rw-   0        0        0     1089 2023-02-14 02:47:58.000000 django-easy-faq-1.5/license
--rw-rw-rw-   0        0        0      951 2023-02-14 03:20:44.059645 django-easy-faq-1.5/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-02-14 02:47:58.000000 django-easy-faq-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 00:49:20.957297 django-easy-faq-1.6/
+-rw-rw-rw-   0        0        0     1089 2023-02-14 02:47:58.000000 django-easy-faq-1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      108 2023-02-14 02:47:58.000000 django-easy-faq-1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    15281 2023-05-08 00:49:20.958304 django-easy-faq-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    14304 2023-05-08 00:43:53.000000 django-easy-faq-1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 00:49:20.805131 django-easy-faq-1.6/django_easy_faq.egg-info/
+-rw-rw-rw-   0        0        0    15281 2023-05-08 00:49:20.000000 django-easy-faq-1.6/django_easy_faq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1088 2023-05-08 00:49:20.000000 django-easy-faq-1.6/django_easy_faq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 00:49:20.000000 django-easy-faq-1.6/django_easy_faq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-08 00:49:20.000000 django-easy-faq-1.6/django_easy_faq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-08 00:49:20.000000 django-easy-faq-1.6/django_easy_faq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 00:49:20.853702 django-easy-faq-1.6/faq/
+-rw-rw-rw-   0        0        0       41 2023-02-14 02:47:58.000000 django-easy-faq-1.6/faq/__init__.py
+-rw-rw-rw-   0        0        0     2429 2023-05-05 20:03:31.000000 django-easy-faq-1.6/faq/admin.py
+-rw-rw-rw-   0        0        0      170 2023-02-14 02:47:58.000000 django-easy-faq-1.6/faq/apps.py
+-rw-rw-rw-   0        0        0      270 2023-05-05 19:44:23.000000 django-easy-faq-1.6/faq/forms.py
+drwxrwxrwx   0        0        0        0 2023-05-08 00:49:20.889190 django-easy-faq-1.6/faq/migrations/
+-rw-rw-rw-   0        0        0     4220 2023-02-14 02:47:58.000000 django-easy-faq-1.6/faq/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1543 2023-02-14 02:47:58.000000 django-easy-faq-1.6/faq/migrations/0002_alter_answer_id_alter_answerhelpful_id_and_more.py
+-rw-rw-rw-   0        0        0      455 2023-02-14 02:47:58.000000 django-easy-faq-1.6/faq/migrations/0003_auto_20220619_0939.py
+-rw-rw-rw-   0        0        0      576 2023-02-14 02:47:58.000000 django-easy-faq-1.6/faq/migrations/0004_alter_answer_slug_alter_category_slug.py
+-rw-rw-rw-   0        0        0      409 2023-05-05 20:01:24.000000 django-easy-faq-1.6/faq/migrations/0005_rename_description_category__description.py
+-rw-rw-rw-   0        0        0        0 2023-02-14 02:47:58.000000 django-easy-faq-1.6/faq/migrations/__init__.py
+-rw-rw-rw-   0        0        0     4646 2023-05-05 20:05:19.000000 django-easy-faq-1.6/faq/models.py
+-rw-rw-rw-   0        0        0      346 2023-02-14 02:47:58.000000 django-easy-faq-1.6/faq/path_converters.py
+-rw-rw-rw-   0        0        0     2476 2023-02-14 02:47:58.000000 django-easy-faq-1.6/faq/snippets.py
+drwxrwxrwx   0        0        0        0 2023-05-08 00:49:20.765500 django-easy-faq-1.6/faq/templates/
+drwxrwxrwx   0        0        0        0 2023-05-08 00:49:20.955384 django-easy-faq-1.6/faq/templates/faq/
+-rw-rw-rw-   0        0        0      342 2023-02-14 02:47:58.000000 django-easy-faq-1.6/faq/templates/faq/answer_form.html
+-rw-rw-rw-   0        0        0      242 2023-02-14 02:47:58.000000 django-easy-faq-1.6/faq/templates/faq/base.html
+-rw-rw-rw-   0        0        0      421 2023-02-14 02:47:58.000000 django-easy-faq-1.6/faq/templates/faq/categories_list.html
+-rw-rw-rw-   0        0        0      633 2023-02-14 02:47:58.000000 django-easy-faq-1.6/faq/templates/faq/category_detail.html
+-rw-rw-rw-   0        0        0      281 2023-02-14 02:47:58.000000 django-easy-faq-1.6/faq/templates/faq/comment_form.html
+-rw-rw-rw-   0        0        0      758 2023-02-14 02:47:58.000000 django-easy-faq-1.6/faq/templates/faq/comments.html
+-rw-rw-rw-   0        0        0     1264 2023-02-14 02:47:58.000000 django-easy-faq-1.6/faq/templates/faq/question_base.html
+-rw-rw-rw-   0        0        0     2877 2023-02-14 02:47:58.000000 django-easy-faq-1.6/faq/templates/faq/question_detail.html
+-rw-rw-rw-   0        0        0      264 2023-02-14 02:47:58.000000 django-easy-faq-1.6/faq/templates/faq/question_form.html
+-rw-rw-rw-   0        0        0      434 2023-02-14 02:47:58.000000 django-easy-faq-1.6/faq/templates/faq/questions_list.html
+-rw-rw-rw-   0        0        0      262 2023-02-14 02:47:58.000000 django-easy-faq-1.6/faq/templates/faq/vote_form.html
+-rw-rw-rw-   0        0        0     7564 2023-02-14 02:47:58.000000 django-easy-faq-1.6/faq/tests.py
+-rw-rw-rw-   0        0        0     2964 2023-02-14 03:22:49.000000 django-easy-faq-1.6/faq/urls.py
+-rw-rw-rw-   0        0        0    13091 2023-05-05 22:13:32.000000 django-easy-faq-1.6/faq/views.py
+-rw-rw-rw-   0        0        0     1089 2023-02-14 02:47:58.000000 django-easy-faq-1.6/license
+-rw-rw-rw-   0        0        0      951 2023-05-08 00:49:20.960297 django-easy-faq-1.6/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-02-14 02:47:58.000000 django-easy-faq-1.6/setup.py
```

### Comparing `django-easy-faq-1.5/LICENSE.txt` & `django-easy-faq-1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-easy-faq-1.5/PKG-INFO` & `django-easy-faq-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-easy-faq
-Version: 1.5
+Version: 1.6
 Summary: A Django app to add great faq functionality to website.
 Home-page: https://github.com/dragoncommits/django-easy-faq
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: license
 
 # django-easy-faq
 
-django-easy-faq is a Django app to allow for a simple yet feature rich faq app. with categories, commenting voting of questions and answers all as an optional part of the app.
+django-easy-faq is a Django app to allow for a simple yet feature rich faq app. with categories, commenting voting of questions and answers all as an optional part of the app. To see screenshots of what this django-easy-faq could look like with bootstrap 5 styling [click here](demo/demo.md).
 
 
 ## Quick start
 
 1. pip install:
 
     `pip install django-easy-faq`
@@ -359,7 +359,9 @@
 
 1.3 fixed bug where a slug must be filled out in admin even though slug gets auto generated to save for questions, answers, and categories. made questions, answers, categories slugs readonly in admin
 
 1.4 added unicode option to add unicode slugs
 
 1.5 added login_required setting to allow faq app to be available to only logged in users
 
+1.6 fixed bug where no_category_description did not do remove the category description in the admin
+
```

### Comparing `django-easy-faq-1.5/README.md` & `django-easy-faq-1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # django-easy-faq
 
-django-easy-faq is a Django app to allow for a simple yet feature rich faq app. with categories, commenting voting of questions and answers all as an optional part of the app.
+django-easy-faq is a Django app to allow for a simple yet feature rich faq app. with categories, commenting voting of questions and answers all as an optional part of the app. To see screenshots of what this django-easy-faq could look like with bootstrap 5 styling [click here](demo/demo.md).
 
 
 ## Quick start
 
 1. pip install:
 
     `pip install django-easy-faq`
@@ -332,8 +332,10 @@
 
 1.2 fixed bug in pypi distro not including faq app
 
 1.3 fixed bug where a slug must be filled out in admin even though slug gets auto generated to save for questions, answers, and categories. made questions, answers, categories slugs readonly in admin
 
 1.4 added unicode option to add unicode slugs
 
-1.5 added login_required setting to allow faq app to be available to only logged in users
+1.5 added login_required setting to allow faq app to be available to only logged in users
+
+1.6 fixed bug where no_category_description did not do remove the category description in the admin
```

#### html2text {}

```diff
@@ -1,21 +1,23 @@
 # django-easy-faq django-easy-faq is a Django app to allow for a simple yet
 feature rich faq app. with categories, commenting voting of questions and
-answers all as an optional part of the app. ## Quick start 1. pip install: `pip
-install django-easy-faq` 2. Add "faq" to your INSTALLED_APPS setting like this:
-```python INSTALLED_APPS = [ ... 'faq',] ``` 3. Include the easy-faq URLconf in
-your project urls.py like this:: ```python #â¦ path('faq/', include
-('faq.urls')), #â¦ ``` 4. Add `FAQ_SETTINGS = []` to your `settings.py` 5. Run
-``python manage.py makemigrations`` to create the faq models migrations. 6. Run
-``python manage.py migrate`` to create the faq models. 7. Start the development
-server and visit http://127.0.0.1:8000/admin/ to create a category (you'll need
-the Admin app enabled).(categories part of the app can be disabled) 8. Visit
-http://127.0.0.1:8000/faq/ to see the categories. ## Settings you can change
-most things in settings below is a list of all settings add any or all to
-change to desired behavior:: FAQ_SETTINGS = ['your_settings_here',] 1.
+answers all as an optional part of the app. To see screenshots of what this
+django-easy-faq could look like with bootstrap 5 styling [click here](demo/
+demo.md). ## Quick start 1. pip install: `pip install django-easy-faq` 2. Add
+"faq" to your INSTALLED_APPS setting like this: ```python INSTALLED_APPS =
+[ ... 'faq',] ``` 3. Include the easy-faq URLconf in your project urls.py like
+this:: ```python #â¦ path('faq/', include('faq.urls')), #â¦ ``` 4. Add
+`FAQ_SETTINGS = []` to your `settings.py` 5. Run ``python manage.py
+makemigrations`` to create the faq models migrations. 6. Run ``python manage.py
+migrate`` to create the faq models. 7. Start the development server and visit
+http://127.0.0.1:8000/admin/ to create a category (you'll need the Admin app
+enabled).(categories part of the app can be disabled) 8. Visit http://
+127.0.0.1:8000/faq/ to see the categories. ## Settings you can change most
+things in settings below is a list of all settings add any or all to change to
+desired behavior:: FAQ_SETTINGS = ['your_settings_here',] 1.
 no_category_description - add if using categories but don't want descriptions
 for them 2. no_category - add if don't want to use categories 3.
 logged_in_users_can_add_question - add if you want any logged in user to be
 able to ask a question 4. logged_in_users_can_answer_question - add if you want
 any logged in user to be able to answer a question 5. allow_multiple_answers -
 add if you want a question to be able to be answered multiple times 6.
 no_comments - add if don't want to use comments 7. anonymous_user_can_comment -
@@ -150,7 +152,9 @@
 logged out users can vote - which then raises exceptions 0.5 fixed migrations
 1.0 added pypi distribution 1.1 added more templates to override easily 1.2
 fixed bug in pypi distro not including faq app 1.3 fixed bug where a slug must
 be filled out in admin even though slug gets auto generated to save for
 questions, answers, and categories. made questions, answers, categories slugs
 readonly in admin 1.4 added unicode option to add unicode slugs 1.5 added
 login_required setting to allow faq app to be available to only logged in users
+1.6 fixed bug where no_category_description did not do remove the category
+description in the admin
```

### Comparing `django-easy-faq-1.5/django_easy_faq.egg-info/PKG-INFO` & `django-easy-faq-1.6/django_easy_faq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-easy-faq
-Version: 1.5
+Version: 1.6
 Summary: A Django app to add great faq functionality to website.
 Home-page: https://github.com/dragoncommits/django-easy-faq
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: license
 
 # django-easy-faq
 
-django-easy-faq is a Django app to allow for a simple yet feature rich faq app. with categories, commenting voting of questions and answers all as an optional part of the app.
+django-easy-faq is a Django app to allow for a simple yet feature rich faq app. with categories, commenting voting of questions and answers all as an optional part of the app. To see screenshots of what this django-easy-faq could look like with bootstrap 5 styling [click here](demo/demo.md).
 
 
 ## Quick start
 
 1. pip install:
 
     `pip install django-easy-faq`
@@ -359,7 +359,9 @@
 
 1.3 fixed bug where a slug must be filled out in admin even though slug gets auto generated to save for questions, answers, and categories. made questions, answers, categories slugs readonly in admin
 
 1.4 added unicode option to add unicode slugs
 
 1.5 added login_required setting to allow faq app to be available to only logged in users
 
+1.6 fixed bug where no_category_description did not do remove the category description in the admin
+
```

### Comparing `django-easy-faq-1.5/django_easy_faq.egg-info/SOURCES.txt` & `django-easy-faq-1.6/django_easy_faq.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 faq/tests.py
 faq/urls.py
 faq/views.py
 faq/migrations/0001_initial.py
 faq/migrations/0002_alter_answer_id_alter_answerhelpful_id_and_more.py
 faq/migrations/0003_auto_20220619_0939.py
 faq/migrations/0004_alter_answer_slug_alter_category_slug.py
+faq/migrations/0005_rename_description_category__description.py
 faq/migrations/__init__.py
 faq/templates/faq/answer_form.html
 faq/templates/faq/base.html
 faq/templates/faq/categories_list.html
 faq/templates/faq/category_detail.html
 faq/templates/faq/comment_form.html
 faq/templates/faq/comments.html
```

### Comparing `django-easy-faq-1.5/faq/admin.py` & `django-easy-faq-1.6/faq/admin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from django.contrib import admin
 from .models import *
 from django.conf import settings
-from . import forms
-
 
 # Register your models here.
 
 class AnswerHelpfulAdmin(admin.ModelAdmin):
     list_display = ("vote", "answer", "user")
     list_filter = ('vote',)
     search_fields = ['answer', "user"]
@@ -22,18 +20,27 @@
     list_display = ("answer", "question", "helpful", "not_helpful")
     list_filter = ('helpful', "not_helpful")
     search_fields = ['answer', "question"]
     readonly_fields = ('helpful', "not_helpful", 'slug')
 
 
 class CategoryAdmin(admin.ModelAdmin):
-    list_display = ("name", "slug", "description")
-    search_fields = ['name', "description"]
+    search_fields = ['name', "_description"]
     readonly_fields = ("slug",)
 
+    def get_list_display(self, request):
+        if "no_category_description" not in settings.FAQ_SETTINGS:
+            return ["name", "slug", "description"]
+        return ['name', 'slug']
+
+    def get_exclude(self, request, obj=None):
+        if "no_category_description" in settings.FAQ_SETTINGS:
+            return ['_description']
+        else:
+            return None
 
 class CommentAdmin(admin.ModelAdmin):
     list_display = ("comment", "question", "user", "post_time")
     list_filter = ('question', "post_time")
     search_fields = ['comment', "question"]
```

### Comparing `django-easy-faq-1.5/faq/migrations/0001_initial.py` & `django-easy-faq-1.6/faq/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-easy-faq-1.5/faq/migrations/0002_alter_answer_id_alter_answerhelpful_id_and_more.py` & `django-easy-faq-1.6/faq/migrations/0002_alter_answer_id_alter_answerhelpful_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django-easy-faq-1.5/faq/migrations/0004_alter_answer_slug_alter_category_slug.py` & `django-easy-faq-1.6/faq/migrations/0004_alter_answer_slug_alter_category_slug.py`

 * *Files identical despite different names*

### Comparing `django-easy-faq-1.5/faq/models.py` & `django-easy-faq-1.6/faq/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,23 +66,31 @@
         self.helpful = self.get_helpful()
         self.not_helpful = self.get_not_helpful()
         super().save(*args, **kwargs)
 
 
 class Category(models.Model):
     name = models.CharField(max_length=50, unique=True)
-    description = models.TextField()
+    _description = models.TextField()
     slug = models.SlugField(max_length=50, unique=True, blank=True)
 
     def __str__(self):
         return self.name
 
     class Meta:
         verbose_name_plural = "categories"
 
+    @property
+    def description(self):
+        """only show the description is categories have descriptions"""
+        if "no_category_description" in settings.FAQ_SETTINGS:
+            return None
+        else:
+            return self._description
+
     def save(self, *args, **kwargs):
         self.slug = slugify(self.name, allow_unicode='allow_unicode' in settings.FAQ_SETTINGS)[:50]
         return super().save(*args, **kwargs)
 
 
 class FAQComment(models.Model):
     user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.CASCADE, null=True)
```

### Comparing `django-easy-faq-1.5/faq/snippets.py` & `django-easy-faq-1.6/faq/snippets.py`

 * *Files identical despite different names*

### Comparing `django-easy-faq-1.5/faq/templates/faq/category_detail.html` & `django-easy-faq-1.6/faq/templates/faq/category_detail.html`

 * *Files identical despite different names*

### Comparing `django-easy-faq-1.5/faq/templates/faq/comments.html` & `django-easy-faq-1.6/faq/templates/faq/comments.html`

 * *Files identical despite different names*

### Comparing `django-easy-faq-1.5/faq/templates/faq/question_base.html` & `django-easy-faq-1.6/faq/templates/faq/question_base.html`

 * *Files identical despite different names*

### Comparing `django-easy-faq-1.5/faq/templates/faq/question_detail.html` & `django-easy-faq-1.6/faq/templates/faq/question_detail.html`

 * *Files identical despite different names*

### Comparing `django-easy-faq-1.5/faq/tests.py` & `django-easy-faq-1.6/faq/tests.py`

 * *Files identical despite different names*

### Comparing `django-easy-faq-1.5/faq/views.py` & `django-easy-faq-1.6/faq/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,21 @@
             self.question_url = form.get_absolute_url()
             return super().form_valid(form)
         else:
             form = form.save()
             self.question_url = form.get_absolute_url()
             return super().form_valid(form)
 
+    def get_context_data(self, **kwargs):
+        context = super().get_context_data(**kwargs)
+
+        if "no_category" not in settings.FAQ_SETTINGS:
+            context['category'] = models.Category.objects.get(slug=self.kwargs["slug"])
+        return context
+
 
 class QuestionDetail(generic.DetailView):
     model = models.Question
     template_name = "faq/question_detail.html"
     context_object_name = "question"
 
     def get_object(self, queryset=None):
```

### Comparing `django-easy-faq-1.5/license` & `django-easy-faq-1.6/license`

 * *Files identical despite different names*

### Comparing `django-easy-faq-1.5/setup.cfg` & `django-easy-faq-1.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 6561 7379 2d66   = django-easy-f
 00000020: 6171 0d0a 7665 7273 696f 6e20 3d20 312e  aq..version = 1.
-00000030: 350d 0a64 6573 6372 6970 7469 6f6e 203d  5..description =
+00000030: 360d 0a64 6573 6372 6970 7469 6f6e 203d  6..description =
 00000040: 2041 2044 6a61 6e67 6f20 6170 7020 746f   A Django app to
 00000050: 2061 6464 2067 7265 6174 2066 6171 2066   add great faq f
 00000060: 756e 6374 696f 6e61 6c69 7479 2074 6f20  unctionality to 
 00000070: 7765 6273 6974 652e 0d0a 6c6f 6e67 5f64  website...long_d
 00000080: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
 00000090: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
 000000a0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
```

