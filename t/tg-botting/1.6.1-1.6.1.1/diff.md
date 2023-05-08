# Comparing `tmp/tg-botting-1.6.1.tar.gz` & `tmp/tg-botting-1.6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg-botting-1.6.1.tar", last modified: Mon May  8 11:04:56 2023, max compression
+gzip compressed data, was "tg-botting-1.6.1.1.tar", last modified: Mon May  8 14:10:05 2023, max compression
```

## Comparing `tg-botting-1.6.1.tar` & `tg-botting-1.6.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 11:04:56.187511 tg-botting-1.6.1/
--rw-rw-rw-   0        0        0      918 2023-05-08 11:04:56.186514 tg-botting-1.6.1/PKG-INFO
--rw-rw-rw-   0        0        0      930 2022-12-06 14:18:03.000000 tg-botting-1.6.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-08 11:04:56.187511 tg-botting-1.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1445 2023-05-08 10:30:06.000000 tg-botting-1.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 11:04:56.182562 tg-botting-1.6.1/tg_botting/
--rw-rw-rw-   0        0        0    27942 2023-04-11 17:05:02.000000 tg-botting-1.6.1/tg_botting/bot.py
--rw-rw-rw-   0        0        0      976 2023-01-11 17:39:26.000000 tg-botting-1.6.1/tg_botting/cog.py
--rw-rw-rw-   0        0        0      995 2022-12-13 21:08:58.000000 tg-botting-1.6.1/tg_botting/generals.py
--rw-rw-rw-   0        0        0    15712 2023-05-08 10:30:06.000000 tg-botting-1.6.1/tg_botting/objects.py
--rw-rw-rw-   0        0        0       38 2022-12-13 21:06:01.000000 tg-botting-1.6.1/tg_botting/user_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 11:04:56.186514 tg-botting-1.6.1/tg_botting.egg-info/
--rw-rw-rw-   0        0        0      918 2023-05-08 11:04:56.000000 tg-botting-1.6.1/tg_botting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-05-08 11:04:56.000000 tg-botting-1.6.1/tg_botting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 11:04:56.000000 tg-botting-1.6.1/tg_botting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-08 11:04:56.000000 tg-botting-1.6.1/tg_botting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-08 11:04:56.000000 tg-botting-1.6.1/tg_botting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 14:10:05.152740 tg-botting-1.6.1.1/
+-rw-rw-rw-   0        0        0      920 2023-05-08 14:10:05.151767 tg-botting-1.6.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      930 2022-12-06 14:18:03.000000 tg-botting-1.6.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-08 14:10:05.152740 tg-botting-1.6.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1447 2023-05-08 14:05:42.000000 tg-botting-1.6.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 14:10:05.146755 tg-botting-1.6.1.1/tg_botting/
+-rw-rw-rw-   0        0        0    27942 2023-04-11 17:05:02.000000 tg-botting-1.6.1.1/tg_botting/bot.py
+-rw-rw-rw-   0        0        0      976 2023-01-11 17:39:26.000000 tg-botting-1.6.1.1/tg_botting/cog.py
+-rw-rw-rw-   0        0        0      995 2022-12-13 21:08:58.000000 tg-botting-1.6.1.1/tg_botting/generals.py
+-rw-rw-rw-   0        0        0    15716 2023-05-08 14:05:42.000000 tg-botting-1.6.1.1/tg_botting/objects.py
+-rw-rw-rw-   0        0        0       38 2022-12-13 21:06:01.000000 tg-botting-1.6.1.1/tg_botting/user_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-08 14:10:05.150770 tg-botting-1.6.1.1/tg_botting.egg-info/
+-rw-rw-rw-   0        0        0      920 2023-05-08 14:10:05.000000 tg-botting-1.6.1.1/tg_botting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-05-08 14:10:05.000000 tg-botting-1.6.1.1/tg_botting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 14:10:05.000000 tg-botting-1.6.1.1/tg_botting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-08 14:10:05.000000 tg-botting-1.6.1.1/tg_botting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-08 14:10:05.000000 tg-botting-1.6.1.1/tg_botting.egg-info/top_level.txt
```

### Comparing `tg-botting-1.6.1/PKG-INFO` & `tg-botting-1.6.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 1.6.1
+Version: 1.6.1.1
 Summary: python library for easy creation of a telegram bot.
 Home-page: https://github.com/2sweetheart2/tg_botting/tree/master
 Author: Sweetie (Roma Fomkin)
 Author-email: <2004sweetheart2004@gmail.com>
 Keywords: python,bot,tg,tg bot,telegram,telegram bot,botting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `tg-botting-1.6.1/README.md` & `tg-botting-1.6.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tg-botting-1.6.1/setup.py` & `tg-botting-1.6.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.6.1'
+VERSION = '1.6.1.1'
 DESCRIPTION = 'python library for easy creation of a telegram bot.'
 LONG_DESCRIPTION = 'A package that allows you to create bots for telegram using its entire API.'
 
 setup(
     name="tg-botting",
     version=VERSION,
     url='https://github.com/2sweetheart2/tg_botting/tree/master',
```

### Comparing `tg-botting-1.6.1/tg_botting/bot.py` & `tg-botting-1.6.1.1/tg_botting/bot.py`

 * *Files identical despite different names*

### Comparing `tg-botting-1.6.1/tg_botting/cog.py` & `tg-botting-1.6.1.1/tg_botting/cog.py`

 * *Files identical despite different names*

### Comparing `tg-botting-1.6.1/tg_botting/generals.py` & `tg-botting-1.6.1.1/tg_botting/generals.py`

 * *Files identical despite different names*

### Comparing `tg-botting-1.6.1/tg_botting/objects.py` & `tg-botting-1.6.1.1/tg_botting/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,15 +273,15 @@
         if photo:
             data['caption'] = text
             data.pop('chat_id')
             return await self.send_photo(photo, **data)
         if text is not None:
             if len(text) > 4096:
                 datas = []
-                for i in range(0,len(text)//4094):
+                for i in range(0,(len(text)//4094)+1):
                     data['text'] = text[i*4096:(i+1)*4094]
                     rs = await self.bot.tg_request('sendMessage', True, **data)
                     datas.append(rs)
                 return datas
         data['text'] = text
         rs = await self.bot.tg_request('sendMessage', True, **data)
         return rs.get('ok')
```

### Comparing `tg-botting-1.6.1/tg_botting.egg-info/PKG-INFO` & `tg-botting-1.6.1.1/tg_botting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 1.6.1
+Version: 1.6.1.1
 Summary: python library for easy creation of a telegram bot.
 Home-page: https://github.com/2sweetheart2/tg_botting/tree/master
 Author: Sweetie (Roma Fomkin)
 Author-email: <2004sweetheart2004@gmail.com>
 Keywords: python,bot,tg,tg bot,telegram,telegram bot,botting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

