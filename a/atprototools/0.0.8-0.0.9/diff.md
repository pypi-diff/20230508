# Comparing `tmp/atprototools-0.0.8.tar.gz` & `tmp/atprototools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atprototools-0.0.8.tar", last modified: Mon Apr 10 18:59:40 2023, max compression
+gzip compressed data, was "atprototools-0.0.9.tar", last modified: Mon Apr 10 20:12:14 2023, max compression
```

## Comparing `atprototools-0.0.8.tar` & `atprototools-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-10 18:59:40.949046 atprototools-0.0.8/
--rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-10 18:59:40.949046 atprototools-0.0.8/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      753 2023-04-10 18:59:01.000000 atprototools-0.0.8/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-10 18:59:40.949046 atprototools-0.0.8/atprototools/
--rw-r--r--   0 user      (1000) user      (1000)     6195 2023-04-10 18:56:45.000000 atprototools-0.0.8/atprototools/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-10 18:59:40.949046 atprototools-0.0.8/atprototools.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-10 18:59:40.000000 atprototools-0.0.8/atprototools.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      222 2023-04-10 18:59:40.000000 atprototools-0.0.8/atprototools.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-10 18:59:40.000000 atprototools-0.0.8/atprototools.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       17 2023-04-10 18:59:40.000000 atprototools-0.0.8/atprototools.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       13 2023-04-10 18:59:40.000000 atprototools-0.0.8/atprototools.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-10 18:59:40.949046 atprototools-0.0.8/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      760 2023-04-10 18:59:04.000000 atprototools-0.0.8/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-10 20:12:14.118710 atprototools-0.0.9/
+-rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-10 20:12:14.118710 atprototools-0.0.9/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      896 2023-04-10 20:11:22.000000 atprototools-0.0.9/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-10 20:12:14.108710 atprototools-0.0.9/atprototools/
+-rw-r--r--   0 user      (1000) user      (1000)     7094 2023-04-10 20:09:56.000000 atprototools-0.0.9/atprototools/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-10 20:12:14.108710 atprototools-0.0.9/atprototools.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      622 2023-04-10 20:12:14.000000 atprototools-0.0.9/atprototools.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      259 2023-04-10 20:12:14.000000 atprototools-0.0.9/atprototools.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-10 20:12:14.000000 atprototools-0.0.9/atprototools.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       17 2023-04-10 20:12:14.000000 atprototools-0.0.9/atprototools.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       19 2023-04-10 20:12:14.000000 atprototools-0.0.9/atprototools.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-10 20:12:14.118710 atprototools-0.0.9/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      760 2023-04-10 20:10:24.000000 atprototools-0.0.9/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-10 20:12:14.118710 atprototools-0.0.9/tests/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-04-10 19:18:28.000000 atprototools-0.0.9/tests/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      430 2023-04-10 19:51:48.000000 atprototools-0.0.9/tests/test_main.py
```

### Comparing `atprototools-0.0.8/PKG-INFO` & `atprototools-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: atprototools
-Version: 0.0.8
+Version: 0.0.9
 Summary: tools for posting / deleting things from bsky, in python
 Home-page: https://github.com/ianklatzco/atprototools
 Author: Ian Klatzco
 Author-email: iklatzco@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `atprototools-0.0.8/atprototools/__init__.py` & `atprototools-0.0.9/atprototools/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,202 +1,199 @@
 import requests
 import datetime
 import os
+import unittest
 
-ATP_HOST = "https://bsky.social"
-ATP_AUTH_TOKEN = ""
-DID = "" # leave blank
+# ATP_HOST = "https://bsky.social"
+# ATP_AUTH_TOKEN = ""
+# DID = "" # leave blank
 # TODO prob makes sense to have username here too, and then always assume username + did are populated
 # two use cases: library calls login() (swap to a class later) and cli user uses a shell variable.
 # in either case login() should populate these globals within this file.
 # maybe PASSWORD shouldn't hang around, but you have bigger problems if you're relying on python encapsulation for security.
 
 # TODO annotate all requests.get/post with auth header
 
 
-def login(username, password):
-    data = {"identifier": username, "password": password}
-    resp = requests.post(
-        ATP_HOST + "/xrpc/com.atproto.server.createSession",
-        json=data
-    )
-
-    global ATP_AUTH_TOKEN
-    ATP_AUTH_TOKEN = resp.json().get('accessJwt')
-    if ATP_AUTH_TOKEN == None:
-        raise ValueError("No access token, is your password wrong?")
-
-    global DID
-    DID = resp.json().get("did")
-
-    # TODO
-    # global USERNAME
+class Session():
+    def __init__(self, username, password):
+        self.ATP_HOST = "https://bsky.social"
+        self.ATP_AUTH_TOKEN = ""
+        self.DID = ""
+        self.USERNAME = username
+
+        data = {"identifier": username, "password": password}
+        resp = requests.post(
+            self.ATP_HOST + "/xrpc/com.atproto.server.createSession",
+            json=data
+        )
+
+        self.ATP_AUTH_TOKEN = resp.json().get('accessJwt')
+        if self.ATP_AUTH_TOKEN == None:
+            raise ValueError("No access token, is your password wrong?")
+
+        self.DID = resp.json().get("did")
+
+        # TODO DIDs expire shortly and need to be refreshed for any long-lived sessions
+
+    def reskoot(self,url):
+        # sample url from desktop
+        # POST https://bsky.social/xrpc/com.atproto.repo.createRecord
+        # https://staging.bsky.app/profile/klatz.co/post/3jruqqeygrt2d
+        '''
+        {
+            "collection":"app.bsky.feed.repost",
+            "repo":"did:plc:n5ddwqolbjpv2czaronz6q3d",
+            "record":{
+                "subject":{
+                        "uri":"at://did:plc:scx5mrfxxrqlfzkjcpbt3xfr/app.bsky.feed.post/3jszsrnruws27",
+                        "cid":"bafyreiad336s3honwubedn4ww7m2iosefk5wqgkiity2ofc3ts4ii3ffkq"
+                        },
+                "createdAt":"2023-04-10T17:38:10.516Z",
+                "$type":"app.bsky.feed.repost"
+            }
+        }
+        '''
 
-    # global PASSWORD
+        person_youre_reskooting = self.resolveHandle(url.split('/')[-3]).json().get('did') # its a DID
+        url_identifier = url.split('/')[-1]
 
-    return resp
+        # import pdb; pdb.set_trace()
+        skoot_cid = self.get_skoot_by_url(url).json().get('thread').get('post').get('cid')
 
-def post_skoot(postcontent, timestamp=None):
-    if not timestamp:
+        # subject -> uri is the maia one (thing rt'ing, scx)
         timestamp = datetime.datetime.now(datetime.timezone.utc)
-    timestamp = timestamp.isoformat().replace('+00:00', 'Z')
+        timestamp = timestamp.isoformat().replace('+00:00', 'Z')
 
-    headers = {"Authorization": "Bearer " + ATP_AUTH_TOKEN}
+        headers = {"Authorization": "Bearer " + self.ATP_AUTH_TOKEN}
 
-    data = {
-        "collection": "app.bsky.feed.post",
-        "$type": "app.bsky.feed.post",
-        "repo": "{}".format(DID),
-        "record": {
-            "$type": "app.bsky.feed.post",
-            "createdAt": timestamp,
-            "text": postcontent,
+        data = {
+            "collection": "app.bsky.feed.repost",
+            "repo": "{}".format(self.DID),
+            "record": {
+                "subject": {
+                    "uri":"at://{}/app.bsky.feed.post/{}".format(person_youre_reskooting, url_identifier),
+                    "cid":"{}".format(skoot_cid) # cid of the skoot to reskoot
+                },
+                "createdAt": timestamp,
+                "$type": "app.bsky.feed.repost"
+            }
         }
-    }
 
-    resp = requests.post(
-        ATP_HOST + "/xrpc/com.atproto.repo.createRecord",
-        json=data,
-        headers=headers
-    )
-
-    return resp
-
-def get_skoot_by_url(url):
-    "https://bsky.social/xrpc/app.bsky.feed.getPostThread?uri=at%3A%2F%2Fdid%3Aplc%3Ascx5mrfxxrqlfzkjcpbt3xfr%2Fapp.bsky.feed.post%2F3jszsrnruws27A"
-    "at://did:plc:scx5mrfxxrqlfzkjcpbt3xfr/app.bsky.feed.post/3jszsrnruws27"
-    "https://staging.bsky.app/profile/naia.bsky.social/post/3jszsrnruws27"
-
-    headers = {"Authorization": "Bearer " + ATP_AUTH_TOKEN}
-
-    username_of_person_in_link = url.split('/')[-3]
-    did_of_person_in_link = resolveHandle(username_of_person_in_link).json().get('did')
-    url_identifier = url.split('/')[-1] # the random stuf at the end
-
-    uri = "at://{}/app.bsky.feed.post/{}".format(did_of_person_in_link, url_identifier)
-
-    resp = requests.get(
-        ATP_HOST + "/xrpc/app.bsky.feed.getPostThread?uri={}".format(uri),
-        headers=headers
-    )
-
-    return resp
+        resp = requests.post(
+            self.ATP_HOST + "/xrpc/com.atproto.repo.createRecord",
+            json=data,
+            headers=headers
+        )
 
+        return resp
 
+    def resolveHandle(self,username): # aka getDid
+        headers = {"Authorization": "Bearer " + self.ATP_AUTH_TOKEN}
+        resp = requests.get(
+            self.ATP_HOST + "/xrpc/com.atproto.identity.resolveHandle?handle={}".format(username),
+            headers=headers
+        )
+        return resp
 
-def reskoot(url):
-    # sample url from desktop
-    # POST https://bsky.social/xrpc/com.atproto.repo.createRecord
-    # https://staging.bsky.app/profile/klatz.co/post/3jruqqeygrt2d
-    '''
-    {
-        "collection":"app.bsky.feed.repost",
-        "repo":"did:plc:n5ddwqolbjpv2czaronz6q3d",
-        "record":{
-            "subject":{
-                    "uri":"at://did:plc:scx5mrfxxrqlfzkjcpbt3xfr/app.bsky.feed.post/3jszsrnruws27",
-                    "cid":"bafyreiad336s3honwubedn4ww7m2iosefk5wqgkiity2ofc3ts4ii3ffkq"
-                    },
-            "createdAt":"2023-04-10T17:38:10.516Z",
-            "$type":"app.bsky.feed.repost"
-        }
-    }
-    '''
 
-    person_youre_reskooting = resolveHandle(url.split('/')[-3]).json().get('did') # its a DID
-    url_identifier = url.split('/')[-1]
+    def get_skoot_by_url(self,url):
+        "https://bsky.social/xrpc/app.bsky.feed.getPostThread?uri=at%3A%2F%2Fdid%3Aplc%3Ascx5mrfxxrqlfzkjcpbt3xfr%2Fapp.bsky.feed.post%2F3jszsrnruws27A"
+        "at://did:plc:scx5mrfxxrqlfzkjcpbt3xfr/app.bsky.feed.post/3jszsrnruws27"
+        "https://staging.bsky.app/profile/naia.bsky.social/post/3jszsrnruws27"
+
+        headers = {"Authorization": "Bearer " + self.ATP_AUTH_TOKEN}
+
+        username_of_person_in_link = url.split('/')[-3]
+        did_of_person_in_link = self.resolveHandle(username_of_person_in_link).json().get('did')
+        url_identifier = url.split('/')[-1] # the random stuf at the end
 
-    # import pdb; pdb.set_trace()
-    skoot_cid = get_skoot_by_url(url).json().get('thread').get('post').get('cid')
+        uri = "at://{}/app.bsky.feed.post/{}".format(did_of_person_in_link, url_identifier)
 
-    # subject -> uri is the maia one (thing rt'ing, scx)
-    timestamp = datetime.datetime.now(datetime.timezone.utc)
-    timestamp = timestamp.isoformat().replace('+00:00', 'Z')
-
-    headers = {"Authorization": "Bearer " + ATP_AUTH_TOKEN}
-
-    data = {
-        "collection": "app.bsky.feed.repost",
-        "repo": "{}".format(DID),
-        "record": {
-            "subject": {
-                "uri":"at://{}/app.bsky.feed.post/{}".format(person_youre_reskooting, url_identifier),
-                "cid":"{}".format(skoot_cid) # cid of the skoot to reskoot
-            },
-            "createdAt": timestamp,
-            "$type": "app.bsky.feed.repost"
+        resp = requests.get(
+            self.ATP_HOST + "/xrpc/app.bsky.feed.getPostThread?uri={}".format(uri),
+            headers=headers
+        )
+
+        return resp
+
+    def post_skoot(self, postcontent, timestamp=None):
+        if not timestamp:
+            timestamp = datetime.datetime.now(datetime.timezone.utc)
+        timestamp = timestamp.isoformat().replace('+00:00', 'Z')
+
+        headers = {"Authorization": "Bearer " + self.ATP_AUTH_TOKEN}
+
+        data = {
+            "collection": "app.bsky.feed.post",
+            "$type": "app.bsky.feed.post",
+            "repo": "{}".format(self.DID),
+            "record": {
+                "$type": "app.bsky.feed.post",
+                "createdAt": timestamp,
+                "text": postcontent,
+            }
         }
-    }
 
-    resp = requests.post(
-        ATP_HOST + "/xrpc/com.atproto.repo.createRecord",
-        json=data,
-        headers=headers
-    )
-
-    # print(data)
-
-    return resp
-
-
-def delete_skoot(did,rkey):
-    data = {"collection":"app.bsky.feed.post","repo":"did:plc:{}".format(did),"rkey":"{}".format(rkey)}
-    headers = {"Authorization": "Bearer " + ATP_AUTH_TOKEN}
-    resp = requests.post(
-        ATP_HOST + "/xrpc/com.atproto.repo.deleteRecord",
-        json = data,
-        headers=headers
-    )
-    return resp
-
-def resolveHandle(username): # aka getDid
-    headers = {"Authorization": "Bearer " + ATP_AUTH_TOKEN}
-    resp = requests.get(
-        ATP_HOST + "/xrpc/com.atproto.identity.resolveHandle?handle={}".format(username),
-        headers=headers
-    )
-    return resp
-
-def get_car_file(did_of_car_to_fetch=None):
-    '''
-    Get a .car file contain all skoots.
-    TODO is there a putRepo?
-    TODO save to file
-    '''
-
-    if did_of_car_to_fetch == None:
-        did_of_car_to_fetch = DID
-
-    headers = {"Authorization": "Bearer " + ATP_AUTH_TOKEN}
-
-    resp = requests.get(
-        ATP_HOST + "/xrpc/com.atproto.sync.getRepo?did={}".format(did_of_car_to_fetch),
-        headers = headers
-    )
-
-    return resp
-
-def get_latest_skoot(accountname):
-    return get_latest_n_skoots(accountname, 1)
-
-def get_latest_n_skoots(username, n=5):
-    headers = {"Authorization": "Bearer " + ATP_AUTH_TOKEN}
-    resp = requests.get(
-        ATP_HOST + "/xrpc/app.bsky.feed.getAuthorFeed?actor={}&limit={}".format(username, n),
-        headers = headers
-    )
+        resp = requests.post(
+            self.ATP_HOST + "/xrpc/com.atproto.repo.createRecord",
+            json=data,
+            headers=headers
+        )
+
+        return resp
+
+    def delete_skoot(self, did,rkey):
+        data = {"collection":"app.bsky.feed.post","repo":"did:plc:{}".format(did),"rkey":"{}".format(rkey)}
+        headers = {"Authorization": "Bearer " + self.ATP_AUTH_TOKEN}
+        resp = requests.post(
+            self.ATP_HOST + "/xrpc/com.atproto.repo.deleteRecord",
+            json = data,
+            headers=headers
+        )
+        return resp
+
+    def get_car_file(self, did_of_car_to_fetch=None):
+        '''
+        Get a .car file contain all skoots.
+        TODO is there a putRepo?
+        TODO save to file
+        '''
+
+        if did_of_car_to_fetch == None:
+            did_of_car_to_fetch = self.DID
+
+        headers = {"Authorization": "Bearer " + self.ATP_AUTH_TOKEN}
+
+        resp = requests.get(
+            self.ATP_HOST + "/xrpc/com.atproto.sync.getRepo?did={}".format(did_of_car_to_fetch),
+            headers = headers
+        )
+
+        return resp
+
+    def get_latest_skoot(self, accountname):
+        return self.get_latest_n_skoots(accountname, 1)
+
+    def get_latest_n_skoots(self, username, n=5):
+        headers = {"Authorization": "Bearer " + self.ATP_AUTH_TOKEN}
+        resp = requests.get(
+            self.ATP_HOST + "/xrpc/app.bsky.feed.getAuthorFeed?actor={}&limit={}".format(username, n),
+            headers = headers
+        )
 
-    return resp
+        return resp
 
 if __name__ == "__main__":
     # This code will only be executed if the script is run directly
-    login(os.environ.get("BSKY_USERNAME"), os.environ.get("BSKY_PASSWORD"))
+    # login(os.environ.get("BSKY_USERNAME"), os.environ.get("BSKY_PASSWORD"))
+    sess = Session(os.environ.get("BSKY_USERNAME"), os.environ.get("BSKY_PASSWORD"))
     # f = get_latest_n_skoots('klatz.co',1).content
     # print(f)
-    resp = reskoot("https://staging.bsky.app/profile/naia.bsky.social/post/3jszsrnruws27")
+    # resp = reskoot("https://staging.bsky.app/profile/klatz.co/post/3jt22a3jx5l2a")
     # resp = get_car_file()
     import pdb; pdb.set_trace()
 
 
 
 # resp = login()
 # post("test post")
```

### Comparing `atprototools-0.0.8/atprototools.egg-info/PKG-INFO` & `atprototools-0.0.9/atprototools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: atprototools
-Version: 0.0.8
+Version: 0.0.9
 Summary: tools for posting / deleting things from bsky, in python
 Home-page: https://github.com/ianklatzco/atprototools
 Author: Ian Klatzco
 Author-email: iklatzco@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `atprototools-0.0.8/setup.py` & `atprototools-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='atprototools',
-    version='0.0.8',
+    version='0.0.9',
     description='tools for posting / deleting things from bsky, in python',
     author='Ian Klatzco',
     author_email='iklatzco@gmail.com',
     url='https://github.com/ianklatzco/atprototools',
     packages=find_packages(),
     install_requires=[
         'requests>=2.22.0'
```

