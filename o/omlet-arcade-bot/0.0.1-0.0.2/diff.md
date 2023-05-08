# Comparing `tmp/omlet_arcade_bot-0.0.1.tar.gz` & `tmp/omlet_arcade_bot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omlet_arcade_bot-0.0.1.tar", last modified: Sun May  7 15:34:30 2023, max compression
+gzip compressed data, was "omlet_arcade_bot-0.0.2.tar", last modified: Mon May  8 07:35:11 2023, max compression
```

## Comparing `omlet_arcade_bot-0.0.1.tar` & `omlet_arcade_bot-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-07 15:34:30.956950 omlet_arcade_bot-0.0.1/
--rw-rw----   0 root         (0) everybody  (9997)     1152 2023-05-07 15:34:30.952950 omlet_arcade_bot-0.0.1/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      887 2023-05-07 15:31:54.000000 omlet_arcade_bot-0.0.1/README.md
--rw-rw----   0 root         (0) everybody  (9997)     1760 2023-05-07 15:27:58.000000 omlet_arcade_bot-0.0.1/omlet_arcade_app.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-07 15:34:30.944950 omlet_arcade_bot-0.0.1/omlet_arcade_bot.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     1152 2023-05-07 15:34:30.000000 omlet_arcade_bot-0.0.1/omlet_arcade_bot.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      198 2023-05-07 15:34:30.000000 omlet_arcade_bot-0.0.1/omlet_arcade_bot.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-07 15:34:30.000000 omlet_arcade_bot-0.0.1/omlet_arcade_bot.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       17 2023-05-07 15:34:30.000000 omlet_arcade_bot-0.0.1/omlet_arcade_bot.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-07 15:34:30.960950 omlet_arcade_bot-0.0.1/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      343 2023-05-07 15:29:06.000000 omlet_arcade_bot-0.0.1/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-08 07:35:11.247758 omlet_arcade_bot-0.0.2/
+-rw-rw----   0 root         (0) everybody  (9997)     1159 2023-05-08 07:35:11.239758 omlet_arcade_bot-0.0.2/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      887 2023-05-08 07:34:04.000000 omlet_arcade_bot-0.0.2/README.md
+-rw-rw----   0 root         (0) everybody  (9997)     2320 2023-05-08 07:33:42.000000 omlet_arcade_bot-0.0.2/omlet_arcade_app.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-08 07:35:11.231758 omlet_arcade_bot-0.0.2/omlet_arcade_bot.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     1159 2023-05-08 07:35:10.000000 omlet_arcade_bot-0.0.2/omlet_arcade_bot.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      198 2023-05-08 07:35:10.000000 omlet_arcade_bot-0.0.2/omlet_arcade_bot.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-08 07:35:10.000000 omlet_arcade_bot-0.0.2/omlet_arcade_bot.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       17 2023-05-08 07:35:10.000000 omlet_arcade_bot-0.0.2/omlet_arcade_bot.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-08 07:35:11.247758 omlet_arcade_bot-0.0.2/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      350 2023-05-08 07:34:31.000000 omlet_arcade_bot-0.0.2/setup.py
```

### Comparing `omlet_arcade_bot-0.0.1/PKG-INFO` & `omlet_arcade_bot-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: omlet_arcade_bot
-Version: 0.0.1
-Summary: Модуль использующий, апи Omlet Arcade с 2-мя классами Auth,и Bot.
+Version: 0.0.2
+Summary: Модуль использующий, апи Omlet Arcade с 3-мя классами Auth, Bot и Power.
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
-omlet-arcade_app - это модуль Python для взаимодействия с платформой Omlet Arcade. Модуль позволяет автоматизировать задачи, связанные со стримингом, и взаимодействовать с пользователями.
+omlet-arcade_bot - это модуль Python для взаимодействия с платформой Omlet Arcade. Модуль позволяет автоматизировать задачи, связанные со стримингом, и взаимодействовать с пользователями.
 
 Основные возможности модуля:
 
 - Аутентификация с помощью API-ключа
 - Взаимодействие с платформой Omlet Arcade, включая получение информации о стриме, обработку комментариев и действий пользователей
 - Поддержка команд, модерации и взаимодействия с авторами
```

### Comparing `omlet_arcade_bot-0.0.1/README.md` & `omlet_arcade_bot-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-omlet-arcade_app - это модуль Python для взаимодействия с платформой Omlet Arcade. Модуль позволяет автоматизировать задачи, связанные со стримингом, и взаимодействовать с пользователями.
+omlet-arcade_bot - это модуль Python для взаимодействия с платформой Omlet Arcade. Модуль позволяет автоматизировать задачи, связанные со стримингом, и взаимодействовать с пользователями.
 
 Основные возможности модуля:
 
 - Аутентификация с помощью API-ключа
 - Взаимодействие с платформой Omlet Arcade, включая получение информации о стриме, обработку комментариев и действий пользователей
 - Поддержка команд, модерации и взаимодействия с авторами
```

### Comparing `omlet_arcade_bot-0.0.1/omlet_arcade_app.py` & `omlet_arcade_bot-0.0.2/omlet_arcade_app.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,20 +6,40 @@
         self.api_key = api_key
 
     def api(self):
         headers = {"Authorization": f"Bearer {self.api_key}"}
         response = requests.get("https://api.omlet.gg/v1/user", headers=headers)
         return response.json()
 
+class Power:
+    def __init__(self, bot):
+        self.bot = bot
+
+    def ban(self, user):
+        if self.bot.role != "moderator":
+            print("Error: check bot role, he does not have permission to ban users.")
+            return
+        # бан пользователя
+        pass
+
+    def delete_message(self, message_id):
+        if self.bot.role != "moderator" and self.bot.nickname != self.bot.author:
+            print("Error: check bot role, he does not have permission to delete messages.")
+            return
+        # удаление сообщения
+        pass
+
 class Bot:
     def __init__(self, stream_link, interaction, role, nickname):
         self.stream_link = stream_link
         self.interaction = interaction
         self.role = role
         self.nickname = nickname
+        self.author = None
+        self.power = Power(self)
 
     def interaction(self):
         if self.interaction == "command":
             # реакция на команды
             pass
         elif self.interaction == "moderator":
             # реакция на действия модератора
@@ -36,12 +56,11 @@
         response = requests.get(self.stream_link)
         soup = BeautifulSoup(response.content, "html.parser")
         # парсинг информации о стриме
         pass
 
     def message_context(self, word):
         if self.role == "moderator" and word == "ban":
-            # реакция на слово "ban" для модератора
-            pass
-        elif self.nickname == self.author and word == "subscribe":
-            # реакция на слово "subscribe" для автора
-            pass
+            self.power.ban("user_to_ban")
+        elif self.nickname == self.author and word == "delete":
+            self.power.delete_message("message_id_to_delete")
+
```

### Comparing `omlet_arcade_bot-0.0.1/omlet_arcade_bot.egg-info/PKG-INFO` & `omlet_arcade_bot-0.0.2/omlet_arcade_bot.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: omlet-arcade-bot
-Version: 0.0.1
-Summary: Модуль использующий, апи Omlet Arcade с 2-мя классами Auth,и Bot.
+Version: 0.0.2
+Summary: Модуль использующий, апи Omlet Arcade с 3-мя классами Auth, Bot и Power.
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
-omlet-arcade_app - это модуль Python для взаимодействия с платформой Omlet Arcade. Модуль позволяет автоматизировать задачи, связанные со стримингом, и взаимодействовать с пользователями.
+omlet-arcade_bot - это модуль Python для взаимодействия с платформой Omlet Arcade. Модуль позволяет автоматизировать задачи, связанные со стримингом, и взаимодействовать с пользователями.
 
 Основные возможности модуля:
 
 - Аутентификация с помощью API-ключа
 - Взаимодействие с платформой Omlet Arcade, включая получение информации о стриме, обработку комментариев и действий пользователей
 - Поддержка команд, модерации и взаимодействия с авторами
```

