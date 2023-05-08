# Comparing `tmp/webint_live-0.0.8.tar.gz` & `tmp/webint_live-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webint_live-0.0.8.tar", max compression
+gzip compressed data, was "webint_live-0.0.9.tar", max compression
```

## Comparing `webint_live-0.0.8.tar` & `webint_live-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      820 2023-02-24 02:06:31.891466 webint_live-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2076 2023-02-18 04:33:10.425065 webint_live-0.0.8/webint_live/__init__.py
--rw-r--r--   0        0        0       76 2023-01-27 00:43:31.827973 webint_live-0.0.8/webint_live/templates/__init__.py
--rw-r--r--   0        0        0      506 2023-02-19 00:01:50.628977 webint_live-0.0.8/webint_live/templates/live.html
--rw-r--r--   0        0        0    11324 2023-02-19 01:44:52.777751 webint_live-0.0.8/webint_live/templates/room.html
--rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 webint_live-0.0.8/setup.py
--rw-r--r--   0        0        0      415 1970-01-01 00:00:00.000000 webint_live-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      820 2023-03-06 05:09:59.120815 webint_live-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2175 2023-03-06 03:40:59.313199 webint_live-0.0.9/webint_live/__init__.py
+-rw-r--r--   0        0        0       76 2023-01-27 00:43:31.827973 webint_live-0.0.9/webint_live/templates/__init__.py
+-rw-r--r--   0        0        0    11370 2023-03-06 03:40:52.309114 webint_live-0.0.9/webint_live/templates/chat.html
+-rw-r--r--   0        0        0       42 2023-03-06 03:37:58.887081 webint_live-0.0.9/webint_live/templates/index.html
+-rw-r--r--   0        0        0      537 2023-03-06 03:59:22.079854 webint_live-0.0.9/webint_live/templates/stream.html
+-rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 webint_live-0.0.9/setup.py
+-rw-r--r--   0        0        0      415 1970-01-01 00:00:00.000000 webint_live-0.0.9/PKG-INFO
```

### Comparing `webint_live-0.0.8/pyproject.toml` & `webint_live-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webint-live"
-version = "0.0.8"
+version = "0.0.9"
 description = "go live from your website"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "BSD-2-Clause"
 packages = [{include = "webint_live"}]
 
 [tool.poetry.plugins."webapps"]
 live = "webint_live:app"
```

### Comparing `webint_live-0.0.8/webint_live/__init__.py` & `webint_live-0.0.9/webint_live/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 import web
 from twilio.base.exceptions import TwilioException, TwilioRestException
 from twilio.jwt.access_token import AccessToken
 from twilio.jwt.access_token.grants import ChatGrant, VideoGrant
 from twilio.rest import Client
 
-# from web import tx
-
 app = web.application(__name__, prefix="live")
 twilio_account_sid = app.cfg.get("TWILIO_ACCOUNT_SID")
 twilio_api_key_sid = app.cfg.get("TWILIO_API_KEY_SID")
 twilio_api_key_secret = app.cfg.get("TWILIO_API_KEY_SECRET")
 try:
     twilio_client = Client(
         twilio_api_key_sid, twilio_api_key_secret, twilio_account_sid
@@ -30,26 +28,35 @@
 
 @app.control("")
 class Live:
     """"""
 
     def get(self):
         """"""
-        return app.view.live()
+        return app.view.index()
+
+
+@app.control("stream")
+class Stream:
+    """"""
+
+    def get(self):
+        """"""
+        return app.view.stream()
 
 
 @app.control("chat")
 class Chat:
     """Chat with guests."""
 
     def get(self):
-        """Return the chat room."""
-        # if not tx.user.session:
+        """Return a chat room."""
+        # if not web.tx.user.session:
         #     raise web.SeeOther("/sign-in")
-        return app.view.room()
+        return app.view.chat()
 
     def post(self):
         """Sign user in to chat."""
         username = web.form("username").username
         conversation = get_chatroom("MyRoom")
         try:
             conversation.participants.create(identity=username)
```

### Comparing `webint_live-0.0.8/webint_live/templates/room.html` & `webint_live-0.0.9/webint_live/templates/chat.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 $def with ()
-$var title: Room
+$var title: Chat
 
 <form>
 <label for="username">Name: </label>
 <input type="text" name=username id="username">
-<button id="join_leave">Join call</button>
+<button id="join_leave">Join</button>
 <button id="share_screen" disabled>Share screen</button>
 <button id="toggle_chat" disabled>Toggle chat</button>
 </form>
 
 <p id="count">Disconnected.</p>
 <div id="root">
     <div id="container" class="container">
@@ -22,31 +22,31 @@
             </div>
         </div>
         <input id="chat-input" type="text">
     </div>
 </div>
 
 <style>
-html, body {
-    height: 100%;
-    display: flex;
-    flex-direction: column;
-}
-#root:not(.withChat) {
-    display: block;
-    width: 100%;
-    height: 100%;
-    margin-top: 20px;
-}
-#root.withChat {
-    display: grid;
-    grid-template-columns: 75% 25%;
-    height: 100%;
-    margin-top: 20px;
-}
+$# html, body {
+$#     height: 100%;
+$#     display: flex;
+$#     flex-direction: column;
+$# }
+$# #root:not(.withChat) {
+$#     display: block;
+$#     width: 100%;
+$#     height: 100%;
+$#     margin-top: 20px;
+$# }
+$# #root.withChat {
+$#     display: grid;
+$#     grid-template-columns: 75% 25%;
+$#     height: 100%;
+$#     margin-top: 20px;
+$# }
 
 /* video section */
 
 .container {
     width: calc(100% - 5px);
     height: 100%;
     padding-right: 5px;
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
-$def with () $var title: Room
-Name:  [username            ] Join call Share screen Toggle chat
+$def with () $var title: Chat
+Name:  [username            ] Join Share screen Toggle chat
 Disconnected.
 Me
 [                    ]
```

### Comparing `webint_live-0.0.8/setup.py` & `webint_live-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['twilio>=7.16.2,<8.0.0', 'webint>=0.0']
 
 entry_points = \
 {'webapps': ['live = webint_live:app']}
 
 setup_kwargs = {
     'name': 'webint-live',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'go live from your website',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

