# Comparing `tmp/xyz_school-0.1.8-py3-none-any.whl.zip` & `tmp/xyz_school-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 25365 bytes, number of entries: 25
+Zip file size: 25390 bytes, number of entries: 25
 -rw-r--r--  2.0 unx       45 b- defN 20-Jan-22 16:01 xyz_school/__init__.py
 -rw-r--r--  2.0 unx     1782 b- defN 20-Jul-03 13:50 xyz_school/admin.py
--rw-r--r--  2.0 unx     8003 b- defN 21-Dec-18 03:05 xyz_school/apis.py
+-rw-r--r--  2.0 unx     8151 b- defN 21-Dec-30 17:55 xyz_school/apis.py
 -rw-r--r--  2.0 unx      330 b- defN 20-Jan-24 02:02 xyz_school/apps.py
 -rw-r--r--  2.0 unx     1799 b- defN 21-Dec-16 09:24 xyz_school/choices.py
 -rw-r--r--  2.0 unx    13981 b- defN 21-Dec-22 17:57 xyz_school/helper.py
 -rw-r--r--  2.0 unx     4567 b- defN 21-Dec-19 01:54 xyz_school/importers.py
 -rw-r--r--  2.0 unx    12135 b- defN 21-Dec-20 03:05 xyz_school/models.py
 -rw-r--r--  2.0 unx     3614 b- defN 21-Jun-20 03:44 xyz_school/receivers.py
 -rw-r--r--  2.0 unx     7245 b- defN 21-Dec-16 13:06 xyz_school/serializers.py
@@ -16,12 +16,12 @@
 -rw-r--r--  2.0 unx      497 b- defN 20-Jun-25 21:33 xyz_school/migrations/0002_teacher_description.py
 -rw-r--r--  2.0 unx      484 b- defN 20-Jul-03 07:05 xyz_school/migrations/0003_student_is_formal.py
 -rw-r--r--  2.0 unx      632 b- defN 20-Aug-03 10:20 xyz_school/migrations/0004_class_major.py
 -rw-r--r--  2.0 unx      570 b- defN 20-Aug-07 11:12 xyz_school/migrations/0005_major_courses.py
 -rw-r--r--  2.0 unx      494 b- defN 20-Dec-09 17:36 xyz_school/migrations/0006_class_tags.py
 -rw-r--r--  2.0 unx     3295 b- defN 21-Dec-16 09:27 xyz_school/migrations/0007_auto_20211212_1954.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-04 10:21 xyz_school/migrations/__init__.py
--rw-r--r--  2.0 unx      982 b- defN 21-Dec-26 16:23 xyz_school-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Dec-26 16:23 xyz_school-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 21-Dec-26 16:23 xyz_school-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2106 b- defN 21-Dec-26 16:23 xyz_school-0.1.8.dist-info/RECORD
-25 files, 82736 bytes uncompressed, 21945 bytes compressed:  73.5%
+-rw-r--r--  2.0 unx      982 b- defN 21-Dec-30 18:08 xyz_school-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Dec-30 18:08 xyz_school-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 21-Dec-30 18:08 xyz_school-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2106 b- defN 21-Dec-30 18:08 xyz_school-0.1.9.dist-info/RECORD
+25 files, 82884 bytes uncompressed, 21970 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -57,20 +57,20 @@
 
 Filename: xyz_school/migrations/0007_auto_20211212_1954.py
 Comment: 
 
 Filename: xyz_school/migrations/__init__.py
 Comment: 
 
-Filename: xyz_school-0.1.8.dist-info/METADATA
+Filename: xyz_school-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: xyz_school-0.1.8.dist-info/WHEEL
+Filename: xyz_school-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: xyz_school-0.1.8.dist-info/top_level.txt
+Filename: xyz_school-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xyz_school-0.1.8.dist-info/RECORD
+Filename: xyz_school-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xyz_school/apis.py

```diff
@@ -6,14 +6,15 @@
 
 from . import models, serializers, importers, helper, stats
 from rest_framework import viewsets, decorators, status
 from rest_framework.permissions import IsAuthenticated
 from rest_framework.response import Response
 from xyz_restful.decorators import register
 import django_filters
+
 __author__ = 'denishuang'
 
 
 @register()
 class TeacherViewSet(viewsets.ModelViewSet):
     queryset = models.Teacher.objects.all()
     serializer_class = serializers.TeacherSerializer
@@ -31,38 +32,42 @@
 
 
 @register()
 class GradeViewSet(viewsets.ModelViewSet):
     queryset = models.Grade.objects.all()
     serializer_class = serializers.GradeSerializer
 
-
     @decorators.action(['post'], detail=False)
     def gen_default(self, request):
         from . import helper
         if not self.get_queryset().exists():
             helper.gen_default_grades()
         return Response({'detail': 'ok'})
 
+
 @register()
 class SessionViewSet(viewsets.ModelViewSet):
     queryset = models.Session.objects.all()
     serializer_class = serializers.SessionSerializer
     search_fields = ('name', 'number')
-    filter_fields = {'id': ['in', 'exact']}
-
+    filter_fields = {
+        'id': ['in', 'exact'],
+        'end_date': ['gte', 'lte', 'gt', 'lt'],
+        'begin_date': ['gte', 'lte', 'gt', 'lt']
+    }
 
     @decorators.action(['post'], detail=False)
     def gen_default(self, request):
         from . import helper
         if not self.get_queryset().exists():
             helper.gen_default_session(-1)
             helper.gen_default_session(0)
         return Response({'detail': 'ok'})
 
+
 @register()
 class ClassViewSet(viewsets.ModelViewSet):
     queryset = models.Class.objects.all()
     serializer_class = serializers.ClassSerializer
     search_fields = ('name', 'code', 'tags')
     filter_fields = {
         'id': ['in', 'exact'],
@@ -103,14 +108,15 @@
         dl = []
         dl.append('班级,学生数,课程数,课程'.split(','))
         for c in qset:
             dl.append([c.name, c.students.count(), c.courses.count(),
                        ",".join(list(c.courses.values_list('name', flat=True)))])
         return Response({'data': dl})
 
+
 @register()
 class MajorViewSet(viewsets.ModelViewSet):
     queryset = models.Major.objects.all()
     serializer_class = serializers.MajorSerializer
     search_fields = ('name', 'code')
     filter_fields = {
         'code': ['exact'],
@@ -154,14 +160,15 @@
         'is_active': ['exact'],
         'is_bind': ['exact'],
         'is_formal': ['exact'],
         'stage': ['exact'],
         'class__id': ['exact', 'in'],
         'class__college': ['exact'],
         'class__major': ['exact'],
+        'class__tags': ['exact'],
         'user': ['exact'],
         'create_time': ['range']
     }
     ordering_fields = ('name', 'number', 'create_time', 'grade')
 
     def get_permissions(self):
         if self.action in ['binding', 'trial_application']:
```

## Comparing `xyz_school-0.1.8.dist-info/METADATA` & `xyz_school-0.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xyz-school
-Version: 0.1.8
+Version: 0.1.9
 Summary: school
 Home-page: https://github.com/szuprefix/py-xyz-school
 Author: szuprefix
 Author-email: szuprefix@126.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

## Comparing `xyz_school-0.1.8.dist-info/RECORD` & `xyz_school-0.1.9.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 xyz_school/__init__.py,sha256=a86c6y40NL5mGeFintcyVRrWnRZeCEJGyAjOogHbZB8,45
 xyz_school/admin.py,sha256=eM47X3uqtGhuGZd-V-HSXKX0y7v3Vp7y8E7nUAPzisY,1782
-xyz_school/apis.py,sha256=0SOYe2YPbE-P2wg7iVQGHaUK22oC2JWeyfPjguxZ_xA,8003
+xyz_school/apis.py,sha256=DQQLMZFS6JCrxQBlAFzobURZoMnRoqqArgu30flaWEg,8151
 xyz_school/apps.py,sha256=a6Wt_D8ullfP096hUgO18dzouYzOed6Z8gggGUzsmgo,330
 xyz_school/choices.py,sha256=jA6VXGWvGXatq8r_xTWYQ2RETqS74eyCDCYI8Tq5-9c,1799
 xyz_school/helper.py,sha256=pdXg6Rxcis_Mad5iG5K5eB4-rbAM0MppGeGBswyAnro,13981
 xyz_school/importers.py,sha256=DwN0Quhe7pPwKoKUboIXfSpQQTr-8wKiE5-MGtej6YM,4567
 xyz_school/models.py,sha256=sgdvRO4QsIMvXUjW7jZSCfgRHyRBtsawDrULZAaoNf8,12135
 xyz_school/receivers.py,sha256=RNXDZYKRHk6jWXXc623bco1qpOdvUnIFJ_-4mfEkvA4,3614
 xyz_school/serializers.py,sha256=laim7PlSyUtgb9AcfDxSPg2IZRMT01hWPEeSEz7rRsI,7245
@@ -15,11 +15,11 @@
 xyz_school/migrations/0002_teacher_description.py,sha256=9wSvbz3x8zE6QlZziLwOCKt7QaRqtGjCOgbuwxV0S4E,497
 xyz_school/migrations/0003_student_is_formal.py,sha256=S6QKQ-skiL2E9FphL7slS-heiJkqjdWngLW-HAEI2WU,484
 xyz_school/migrations/0004_class_major.py,sha256=prlR8yYBritrIqUlgdFcWu-DWmf5WAVb1PzwkbMnf38,632
 xyz_school/migrations/0005_major_courses.py,sha256=oiOlKj9KAvcnEHCYCb9Q7lexO19zj1-oKV7gf0nM1K0,570
 xyz_school/migrations/0006_class_tags.py,sha256=NGBxLDwESyxuDhpHj2NppuP2_s2-nfeQDZzF5_Pv9yw,494
 xyz_school/migrations/0007_auto_20211212_1954.py,sha256=aB2MQBDp1NP7VxMCPl0S719PQIwCH9A9uUxdpm-YzbU,3295
 xyz_school/migrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-xyz_school-0.1.8.dist-info/METADATA,sha256=1iXOe63oXs7AEOmduih7DZ87PF9mV_RgQ0ZTsYP7Dkw,982
-xyz_school-0.1.8.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-xyz_school-0.1.8.dist-info/top_level.txt,sha256=E5mxiGPJOzoOQEmdVnHxGpM5MXK6BNYWwJlFI1ncdqE,11
-xyz_school-0.1.8.dist-info/RECORD,,
+xyz_school-0.1.9.dist-info/METADATA,sha256=aPJE7o1J2I5HEzMej_ehg7w0bz2YJOiUgx4ml0P9do4,982
+xyz_school-0.1.9.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+xyz_school-0.1.9.dist-info/top_level.txt,sha256=E5mxiGPJOzoOQEmdVnHxGpM5MXK6BNYWwJlFI1ncdqE,11
+xyz_school-0.1.9.dist-info/RECORD,,
```

