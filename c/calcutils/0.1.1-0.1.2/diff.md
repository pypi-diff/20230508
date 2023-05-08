# Comparing `tmp/calcutils-0.1.1.tar.gz` & `tmp/calcutils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Python\calcutils\dist\.tmp-dphemvok\calcutils-0.1.1.tar", last modified: Mon May  8 10:11:01 2023, max compression
+gzip compressed data, was "D:\Python\calcutils\dist\.tmp-e4pdnkbe\calcutils-0.1.2.tar", last modified: Mon May  8 10:36:25 2023, max compression
```

## Comparing `calcutils-0.1.1.tar` & `calcutils-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 10:11:01.000000 calcutils-0.1.1/
--rw-rw-rw-   0        0        0       11 2023-05-08 09:36:20.000000 calcutils-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      584 2023-05-08 10:11:01.000000 calcutils-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        8 2023-05-08 07:30:00.000000 calcutils-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 10:11:01.000000 calcutils-0.1.1/calcutils/
--rw-rw-rw-   0        0        0     1098 2023-05-08 08:27:36.000000 calcutils-0.1.1/calcutils/calcu.p
--rw-rw-rw-   0        0        0     8279 2023-05-08 10:10:45.000000 calcutils-0.1.1/calcutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 10:11:01.000000 calcutils-0.1.1/calcutils.egg-info/
--rw-rw-rw-   0        0        0      584 2023-05-08 10:11:01.000000 calcutils-0.1.1/calcutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-05-08 10:11:01.000000 calcutils-0.1.1/calcutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 10:11:01.000000 calcutils-0.1.1/calcutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-08 10:11:01.000000 calcutils-0.1.1/calcutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      512 2023-05-08 10:10:45.000000 calcutils-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 10:11:01.000000 calcutils-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      487 2023-05-08 10:10:45.000000 calcutils-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:36:25.000000 calcutils-0.1.2/
+-rw-rw-rw-   0        0        0       11 2023-05-08 09:36:20.000000 calcutils-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      584 2023-05-08 10:36:25.000000 calcutils-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        8 2023-05-08 07:30:00.000000 calcutils-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 10:36:25.000000 calcutils-0.1.2/calcutils/
+-rw-rw-rw-   0        0        0     1098 2023-05-08 08:27:36.000000 calcutils-0.1.2/calcutils/calcu.p
+-rw-rw-rw-   0        0        0     7827 2023-05-08 10:35:32.000000 calcutils-0.1.2/calcutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:36:25.000000 calcutils-0.1.2/calcutils.egg-info/
+-rw-rw-rw-   0        0        0      584 2023-05-08 10:36:24.000000 calcutils-0.1.2/calcutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-05-08 10:36:25.000000 calcutils-0.1.2/calcutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 10:36:24.000000 calcutils-0.1.2/calcutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-08 10:36:24.000000 calcutils-0.1.2/calcutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      512 2023-05-08 10:35:59.000000 calcutils-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-08 10:36:25.000000 calcutils-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      487 2023-05-08 10:35:59.000000 calcutils-0.1.2/setup.py
```

### Comparing `calcutils-0.1.1/PKG-INFO` & `calcutils-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcutils
-Version: 0.1.1
+Version: 0.1.2
 Summary: A small calcu package
 Home-page: https://github.com/calcu_utils/calcu_utils
 Author: Lahani_Allen
 Author-email: Lahani_Allen <lahani_Allen@utc.com>
 Project-URL: Homepage, https://github.com/calcu_utils/calcu_utils
 Project-URL: Bug Tracker, https://github.com/calcu_utils/calcu_utils/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `calcutils-0.1.1/calcutils/calcu.p` & `calcutils-0.1.2/calcutils/calcu.p`

 * *Files identical despite different names*

### Comparing `calcutils-0.1.1/calcutils/utils.py` & `calcutils-0.1.2/calcutils/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -130,24 +130,24 @@
         if type(self.weight) == type(None):
             loss = self.loss(pred * mask_, target) / torch.sum(mask)
         else:
             loss = self.loss(pred * mask_, target) / torch.sum(self.weight[target] * mask_.squeeze())
         return loss
 
 
-def get_labelsi(res=[], ind=-1):
-    res = load_ca('i', ind)
-    count = [sum(i) for i in res]
-    labels = []
-    preds = []
-    for ind, c in enumerate(count):
-        labels.extend([ind for i in range(c)])
-        for ind_l, l in enumerate(res[ind]):
-            preds.extend([ind_l for j in range(l)])
-    return labels, preds
+def get_labelsi(target):
+    t = target.dataset_name[0].lower()
+    m = target.name[1].lower()
+    if m == 't':
+        ind = 0
+    elif m == 'i':
+        ind = -1
+    else:
+        ind = 1
+    return t, ind
 
 
 class MaskedMSELoss(nn.Module):
     def __init__(self):
         super(MaskedMSELoss, self).__init__()
         self.loss = nn.MSELoss(reduction='sum')
 
@@ -157,26 +157,14 @@
         target -> batch*seq_len
         mask -> batch*seq_len
         """
         loss = self.loss(pred * mask, target) / torch.sum(mask)
         return loss
 
 
-def get_labelse(res=[], ind=0):
-    res =  load_ca('e', 0)
-    count = [sum(i) for i in res]
-    labels = []
-    preds = []
-    for ind, c in enumerate(count):
-        labels.extend([ind for i in range(c)])
-        for ind_l, l in enumerate(res[ind]):
-            preds.extend([ind_l for j in range(l)])
-    return labels, preds
-
-
 class Heat_map():
     def __init__(self, dataset_name='IEMOCAP'):
         if dataset_name == 'IEMOCAP':
             self.classes = ['happiness', 'sadness', 'neutral', 'anger', 'excited', 'frustrated']
         elif dataset_name == 'MELD':
             self.classes = ['neutral', 'surprise', 'fear', 'sadness', 'joy', 'disgust', 'anger']
         elif dataset_name == 'DailyDialog':
@@ -213,16 +201,16 @@
         if show_data:
             for index_y in range(len_y):
                 for index_x in range(len_x):
                     plt.text(index_x, index_y, data[index_y][index_x], va='center', ha='center')
         plt.show()
 
 
-def get_labelsm(res=[], ind=0):
-    res = load_ca('m', ind)
+def get_labels(res, target=None):
+    res = load_ca(*get_labelsi(target))
     count = [sum(i) for i in res]
     labels = []
     preds = []
     for ind, c in enumerate(count):
         labels.extend([ind for i in range(c)])
         for ind_l, l in enumerate(res[ind]):
             preds.extend([ind_l for j in range(l)])
```

### Comparing `calcutils-0.1.1/calcutils.egg-info/PKG-INFO` & `calcutils-0.1.2/calcutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcutils
-Version: 0.1.1
+Version: 0.1.2
 Summary: A small calcu package
 Home-page: https://github.com/calcu_utils/calcu_utils
 Author: Lahani_Allen
 Author-email: Lahani_Allen <lahani_Allen@utc.com>
 Project-URL: Homepage, https://github.com/calcu_utils/calcu_utils
 Project-URL: Bug Tracker, https://github.com/calcu_utils/calcu_utils/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `calcutils-0.1.1/pyproject.toml` & `calcutils-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "calcutils"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Lahani_Allen", email="lahani_Allen@utc.com" },
 ]
 description = "A small calcu package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

