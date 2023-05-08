# Comparing `tmp/yeref-0.1.56.tar.gz` & `tmp/yeref-0.1.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.56.tar", last modified: Mon May  8 07:22:39 2023, max compression
+gzip compressed data, was "yeref-0.1.57.tar", last modified: Mon May  8 10:57:19 2023, max compression
```

## Comparing `yeref-0.1.56.tar` & `yeref-0.1.57.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-08 07:22:39.953031 yeref-0.1.56/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-08 07:22:39.953467 yeref-0.1.56/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-08 07:22:39.954883 yeref-0.1.56/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1305 2023-05-08 07:22:36.000000 yeref-0.1.56/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-08 07:22:39.945826 yeref-0.1.56/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.56/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   508331 2023-05-07 13:42:35.000000 yeref-0.1.56/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   196885 2023-05-08 07:21:39.000000 yeref-0.1.56/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-08 07:22:39.952206 yeref-0.1.56/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-08 07:22:39.000000 yeref-0.1.56/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-08 07:22:39.000000 yeref-0.1.56/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-08 07:22:39.000000 yeref-0.1.56/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-08 07:22:39.000000 yeref-0.1.56/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-08 10:57:19.553101 yeref-0.1.57/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-08 10:57:19.553365 yeref-0.1.57/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-08 10:57:19.554601 yeref-0.1.57/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1351 2023-05-08 10:57:07.000000 yeref-0.1.57/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-08 10:57:19.547007 yeref-0.1.57/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.57/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   508331 2023-05-07 13:42:35.000000 yeref-0.1.57/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   198722 2023-05-08 10:48:49.000000 yeref-0.1.57/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-08 10:57:19.552324 yeref-0.1.57/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-08 10:57:19.000000 yeref-0.1.57/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-08 10:57:19.000000 yeref-0.1.57/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-08 10:57:19.000000 yeref-0.1.57/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-08 10:57:19.000000 yeref-0.1.57/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.56/setup.py` & `yeref-0.1.57/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.56',
+      version='0.1.57',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -39,14 +39,15 @@
 # python setup.py bdist_wheel
 # endregion
 
 # python -m build
 
 # twine upload dist/*
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.56-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.57-py3-none-any.whl
 
 # python3 -m pip install --upgrade yeref
 
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
 # pip show aiogram
+# ARCHFLAGS="-arch x86_64" pip install pycurl
```

### Comparing `yeref-0.1.56/yeref/l_.py` & `yeref-0.1.57/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.1.56/yeref/yeref.py` & `yeref-0.1.57/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,30 @@
 tg_ch_ads_un = 'kiejakn3_djdjn4m_ads'
 tg_ch_ads_id = -1001921910898
 price_one = 200
 price_all = 500
 passwd = 'lost9'
 
 TGPH_TOKEN_MAIN = 'a9335172886eae62ec0743bf8a4e195286ec30cff067da5fd1db2899d008'
+TGPH_TOKENS = {
+    'https://telegra.ph/pst-FereyDemoBot-05-08': 'f8c69d50846e8d55e08f8e3de514f41266e0150434219059f2c91fb4d75f',
+    'https://telegra.ph/pst-FereyBotBot-05-08': 'e7f943fcc98bac07ad6aaf6e570d0f51abadf02567938c997dbc1ad1923b',
+    'https://telegra.ph/pst-FereyPostBot-05-08': '14085be3058c0a25616d094f4bb65c73dc61f783468f01da41d99fb6ace1',
+    'https://telegra.ph/pst-FereyMediaBot-05-08': 'cf71a596b7ecdc96d30ddffdbf1e26863dd39755f47b4fc343fc3867f373',
+    'https://telegra.ph/pst-FereyChannelBot-05-08': 'f43f375b8aec531cee0d5048878943a3ccee97da4143d311d5b2c7ed3237',
+    'https://telegra.ph/pst-FereyGroupBot-05-08': 'c08f94618b94dd25ef75de70c1ed565853efef5479057c68a5720609bb7f',
+    'https://telegra.ph/pst-FereyFindBot-05-08': '2d005bb366dc5bef023d58b93d5f45fb9a02a7d2b0f9063a6fc277b5a62d',
+    'https://telegra.ph/pst-FereyTargetBot-05-08': 'bda8c0a4b7a35101d34252568acd46df7bd3d8d85f4e13dd35f3bddc2f80',
+    'https://telegra.ph/pst-FereyToolsBot-05-08': 'ea83403eb6ac7d2ad24d7e7a86163be20cd2d7f4734267808e154a8fd0a6',
+    'https://telegra.ph/pst-FereyVPNBot-05-08': '38086caf43905ef827715da999aae0be2427ebd7a05d9ff7420543b50613',
+    'https://telegra.ph/pst-FereyAIBot-05-08': 'bcda631d991c16b4fdfd15e7af6512bcf8fd679fee6bd4c717f6266671a0',
+    'https://telegra.ph/pst-FereyUserBot-05-08': '3698a3432c233bef48c238b35cfe94db844858b2ba98594007c7757dcf03',
+    'https://telegra.ph/pst-FereyWorkBot-05-08': 'd4930b2a9311ad63f7f0ae3d61ca7224ecf76a2434a50161e239a45199c5',
+    'https://telegra.ph/pst-FereyAdsBot-05-08': 'c1024508f1a5de4f9544dd10793b1401da95de5719bdcf0b4c9f6c26a672',
+}
 SECTION = 'CONFIG'
 LINES_ON_PAGE = 5
 short_name = 'me'
 const_url = 'https://t.me/'
 phone_number = '79999999999'
 vk_group = 'https://vk.com'
 vk_account = 'https://vk.com'
@@ -229,21 +245,38 @@
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
     finally:
         return result
 
 
-async def ban_handler_menu(bot, chat_id, prepare_ids):
+async def ban_handler_menu(bot, chat_id, args):
     try:
-        prepare_ids = [prepare_id for prepare_id in prepare_ids if prepare_id.isdigit()]
-        if not len(prepare_ids): return
         telegraph_ = Telegraph(access_token=TGPH_TOKEN_MAIN)
         pages = telegraph_.get_page_list()
 
+        if not args:
+            for item in pages['pages']:
+                try:
+                    if item['path'] == 'ban-04-11-7':
+                        page = telegraph_.get_page(path=item['path'], return_content=True, return_html=True)
+                        ban_ids = str(page['content'])
+                        ban_ids = ban_ids[:4096]
+                        ban_ids = ' '.join([f"<code>{it}</code>" for it in ban_ids.split()])
+
+                        await bot.send_message(chat_id, ban_ids)
+                        return
+                except Exception as e:
+                    logger.info(log_ % str(e))
+                    await asyncio.sleep(round(random.uniform(0, 1), 2))
+
+        prepare_ids = args.split()
+        prepare_ids = [prepare_id for prepare_id in prepare_ids if prepare_id.isdigit()]
+        if not len(prepare_ids): return
+
         for item in pages['pages']:
             try:
                 if item['path'] == 'ban-04-11-7':
                     page = telegraph_.get_page(path=item['path'], return_content=True, return_html=True)
                     ban_ids = str(page['content']).split()
                     length1 = len(ban_ids)
                     ban_ids = f"{page['content']} {' '.join(prepare_ids)}"
@@ -265,16 +298,21 @@
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
-async def unban_handler_menu(bot, chat_id, prepare_ids):
+async def unban_handler_menu(bot, chat_id, args):
     try:
+        if not args:
+            return
+        else:
+            prepare_ids = args.split()
+
         prepare_ids = [prepare_id for prepare_id in prepare_ids if prepare_id.isdigit()]
         if not len(prepare_ids): return
         telegraph_ = Telegraph(access_token=TGPH_TOKEN_MAIN)
         pages = telegraph_.get_page_list()
 
         for item in pages['pages']:
             try:
@@ -283,15 +321,17 @@
                     ban_ids = str(page['content']).split()
                     length1 = len(ban_ids)
 
                     ban_ids = [ban_id for ban_id in ban_ids if ban_id not in prepare_ids]
                     length2 = len(ban_ids)
                     ban_ids = list(set(ban_ids))
                     modul = abs(length1 - length2)
-                    telegraph_.edit_page(path=item['path'], title="ban", html_content=' '.join(ban_ids))
+                    html_content = ' '.join(ban_ids)
+                    html_content = '0' if html_content == '' else html_content
+                    telegraph_.edit_page(path=item['path'], title="ban", html_content=html_content)
 
                     if length1 != length2:
                         await bot.send_message(chat_id, f"👩🏽‍💻 {modul}th removed from /ban (len: {length2})")
                     else:
                         await bot.send_message(chat_id, f"👩🏽‍💻 {modul}th already deleted from /ban (len: {length2})")
                     break
             except Exception as e:
@@ -303,59 +343,50 @@
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
 async def check_tgph_posts(bot_username, BASE_D):
     try:
-        telegraph_ = Telegraph(access_token=TGPH_TOKEN_MAIN)
+        arr = [k for k, v in TGPH_TOKENS.items() if bot_username in k]
+        access_key = arr[0] if len(arr) else None
+        if not access_key: return
+
+        access_token = TGPH_TOKENS[access_key]
+        telegraph_ = Telegraph(access_token=access_token)
         pages = telegraph_.get_page_list()
 
         for item in pages['pages']:
             try:
-                if item['path'] == 'broadcasting-04-22':
+                if item['url'] == access_key:
                     page = telegraph_.get_page(path=item['path'], return_content=True, return_html=False)
-                    content_json = json.loads(str(page['content'][0]))
+                    try:
+                        content_json = json.loads(str(page['content'][0]))
+                    except:
+                        content_json = {}
 
                     for OFFER_USERTID, v in content_json.items():
-                        if v[bot_username]:
-                            FereyAdsBot, FereyDemoBot, FereyWorkBot, FereyVPNBot, FereyAIBot, FereyToolsBot, \
-                                FereyMediaBot, FereyFindBot, FereyTargetBot, FereyPostBot, FereyBotBot, FereyUserBot, \
-                                FereyChannelBot, FereyGroupBot, OFFER_TEXT, OFFER_MEDIATYPE, OFFER_FILEID, \
-                                OFFER_BUTTON, OFFER_ISBUTTON, OFFER_TGPHLINK, OFFER_ISTGPH, OFFER_ISSPOILER, \
-                                OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, OFFER_DT, OFFER_TZ = v
-
-                            sql = "INSERT OR IGNORE INTO OFFER (OFFER_USERTID, OFFER_TEXT, OFFER_MEDIATYPE, " \
-                                  "OFFER_FILEID, OFFER_BUTTON, OFFER_ISBUTTON, OFFER_TGPHLINK, OFFER_ISTGPH, " \
-                                  "OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, OFFER_DT, " \
-                                  "OFFER_TZ) VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)"
-                            await db_change(sql, (int(OFFER_USERTID), v[OFFER_TEXT], v[OFFER_MEDIATYPE],
-                                                  v[OFFER_FILEID], v[OFFER_BUTTON], v[OFFER_ISBUTTON],
-                                                  v[OFFER_TGPHLINK], v[OFFER_ISTGPH], v[OFFER_ISSPOILER],
-                                                  v[OFFER_ISPIN], v[OFFER_ISSILENCE], v[OFFER_ISGALLERY],
-                                                  v[OFFER_DT], v[OFFER_TZ],), BASE_D)
-
-                            v[bot_username] = not v[bot_username]
-                            tmp_lst = [FereyAdsBot, FereyDemoBot, FereyWorkBot, FereyVPNBot, FereyAIBot, FereyToolsBot,
-                                       FereyMediaBot, FereyFindBot, FereyTargetBot, FereyPostBot, FereyBotBot,
-                                       FereyUserBot, FereyChannelBot, FereyGroupBot]
-
-                            cnt = 0
-                            for it in tmp_lst:
-                                if v[it]:
-                                    cnt += 1
-
-                            if not cnt:
-                                del content_json[str(OFFER_USERTID)]
-                            else:
-                                content_json[str(OFFER_USERTID)] = v
-
-                            post_dumps = json.dumps(content_json, ensure_ascii=False)
-                            telegraph_.edit_page(path=item['path'], title="broadcasting", html_content=post_dumps)
-                    break
+                        OFFER_TEXT, OFFER_MEDIATYPE, OFFER_FILEID, OFFER_BUTTON, OFFER_ISBUTTON, OFFER_TGPHLINK, \
+                            OFFER_ISTGPH, OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, \
+                            OFFER_DT, OFFER_TZ = v
+
+                        sql = "INSERT OR IGNORE INTO OFFER (OFFER_USERTID, OFFER_TEXT, OFFER_MEDIATYPE, " \
+                              "OFFER_FILEID, OFFER_BUTTON, OFFER_ISBUTTON, OFFER_TGPHLINK, OFFER_ISTGPH, " \
+                              "OFFER_ISSPOILER, OFFER_ISPIN, OFFER_ISSILENCE, OFFER_ISGALLERY, OFFER_DT, " \
+                              "OFFER_TZ) VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)"
+                        await db_change(sql, (int(OFFER_USERTID), v[OFFER_TEXT], v[OFFER_MEDIATYPE],
+                                              v[OFFER_FILEID], v[OFFER_BUTTON], v[OFFER_ISBUTTON],
+                                              v[OFFER_TGPHLINK], v[OFFER_ISTGPH], v[OFFER_ISSPOILER],
+                                              v[OFFER_ISPIN], v[OFFER_ISSILENCE], v[OFFER_ISGALLERY],
+                                              v[OFFER_DT], v[OFFER_TZ],), BASE_D)
+
+                        del content_json[str(OFFER_USERTID)]
+                        post_dumps = json.dumps(content_json, ensure_ascii=False)
+                        telegraph_.edit_page(path=item['path'], title=access_key, html_content=post_dumps)
+                        return
             except Exception as e:
                 logger.info(log_ % str(e))
                 await asyncio.sleep(round(random.uniform(0, 1), 2))
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
@@ -861,14 +892,15 @@
                     media.append(types.InputMediaAudio(media=OFFER_FILEID[i], caption=caption))
                 elif OFFER_MEDIATYPE[i] == 'document':
                     media.append(types.InputMediaDocument(media=OFFER_FILEID[i], caption=caption,
                                                           disable_content_type_detection=True))
 
             result = await bot.send_media_group(chat_id, media)
         if OFFER_MEDIATYPE == 'text':
+            # await bot.send_message(chat_id=5491025132, text='OFFER_TEXT2')
             result = await bot.send_message(chat_id=chat_id,
                                             text=OFFER_TEXT,
                                             disable_web_page_preview=not OFFER_ISTGPH,
                                             disable_notification=OFFER_ISSILENCE,
                                             reply_markup=reply_markup.as_markup())
         elif OFFER_MEDIATYPE == 'animation':
             result = await bot.send_animation(chat_id=chat_id,
```

