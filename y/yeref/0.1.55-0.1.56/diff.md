# Comparing `tmp/yeref-0.1.55.tar.gz` & `tmp/yeref-0.1.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.55.tar", last modified: Fri May  5 13:12:35 2023, max compression
+gzip compressed data, was "yeref-0.1.56.tar", last modified: Mon May  8 07:22:39 2023, max compression
```

## Comparing `yeref-0.1.55.tar` & `yeref-0.1.56.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-05 13:12:35.792867 yeref-0.1.55/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-05 13:12:35.793152 yeref-0.1.55/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-05 13:12:35.794153 yeref-0.1.55/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1305 2023-05-05 13:12:14.000000 yeref-0.1.55/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-05 13:12:35.785848 yeref-0.1.55/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.55/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   508189 2023-05-05 13:09:46.000000 yeref-0.1.55/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   196882 2023-05-02 12:09:42.000000 yeref-0.1.55/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-05 13:12:35.792120 yeref-0.1.55/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-05 13:12:35.000000 yeref-0.1.55/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-05 13:12:35.000000 yeref-0.1.55/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-05 13:12:35.000000 yeref-0.1.55/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-05 13:12:35.000000 yeref-0.1.55/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-08 07:22:39.953031 yeref-0.1.56/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-08 07:22:39.953467 yeref-0.1.56/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-08 07:22:39.954883 yeref-0.1.56/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1305 2023-05-08 07:22:36.000000 yeref-0.1.56/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-08 07:22:39.945826 yeref-0.1.56/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.56/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   508331 2023-05-07 13:42:35.000000 yeref-0.1.56/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   196885 2023-05-08 07:21:39.000000 yeref-0.1.56/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-08 07:22:39.952206 yeref-0.1.56/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-08 07:22:39.000000 yeref-0.1.56/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-08 07:22:39.000000 yeref-0.1.56/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-08 07:22:39.000000 yeref-0.1.56/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-08 07:22:39.000000 yeref-0.1.56/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.55/setup.py` & `yeref-0.1.56/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.55',
+      version='0.1.56',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -39,14 +39,14 @@
 # python setup.py bdist_wheel
 # endregion
 
 # python -m build
 
 # twine upload dist/*
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.55-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.56-py3-none-any.whl
 
 # python3 -m pip install --upgrade yeref
 
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
 # pip show aiogram
```

### Comparing `yeref-0.1.55/yeref/l_.py` & `yeref-0.1.56/yeref/l_.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
     'en': "✏️ 2. Attach <b>media</b> content: photo/gif/video/audio/document/sticker or write a voice/video note in a circle\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
     'es': "✏️ 2. Adjunte contenido <b>multimedia</b> : foto/gif/video/audio/documento/pegatina o escriba una nota de voz/video en un círculo\n\n( <i>o presione &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
     'fr': "✏️ 2. Joignez du contenu <b>multimédia</b> : photo/gif/vidéo/audio/document/autocollant ou écrivez une note vocale/vidéo dans un cercle\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
     'zh': "✏️ 2.附上<b>媒体</b>内容：照片/gif/视频/音频/文档/贴纸或在圈内写语音/视频备注\n\n（<i>或按“➡️️/下一步”跳过此步骤</i>）",
     'ar': "✏️ 2. أرفق محتوى <b>وسائط</b> : صورة / gif / فيديو / صوت / مستند / ملصق أو اكتب ملاحظة صوتية / فيديو في دائرة\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لتخطي هذه الخطوة</i> )",
 }
 l_post_media_wait = {
-    'ru': "👩🏽‍💻 Ожидайте обработки {0}..\n#длительность {1}мин",
+    'ru': "👩🏽‍💻 Ожидай обработки {0}..\n#длительность {1}мин",
     'en': "👩🏽‍💻 Wait for processing {0}..\n#duration {1}min",
     'es': "👩🏽‍💻 Espere a que se procese {0}..\n#duration {1}min",
     'fr': "👩🏽‍💻 Attendez le traitement {0}..\n#duration {1}min",
     'zh': "👩🏽‍💻 等待处理 {0}..\n#duration {1}min",
     'ar': "👩🏽‍💻 انتظر المعالجة {0} ..\n# مدة {1} دقيقة",
 }
 l_post_media_toobig = {
@@ -469,15 +469,15 @@
     'en': "👩🏽‍💻 [spoiler] mode available for photo/gif/video",
     'es': "👩🏽‍💻 Modo [spoiler] disponible para foto/gif/video",
     'fr': "👩🏽‍💻 Mode [spoiler] disponible pour photo/gif/vidéo",
     'zh': "👩🏽‍💻 [剧透] 模式可用于照片/gif/视频",
     'ar': "👩🏽‍💻 وضع [المفسد] متاح للصور / gif / الفيديو",
 }
 l_post_has_restricted = {
-    'ru': "👩🏽‍💻 В настройках <b>[Конфиденциальность]</b> добавь @{0} в <i>исключения</i> для <b>[Голосовые сообщения]</b>, чтобы отобразить <code>видео-заметку</code>/<code>голосовое</code>",
+    'ru': "👩🏽‍💻 У вас premium-аккаунт! В настройках <b>[Конфиденциальность]</b> добавь @{0} в <i>исключения</i> для <b>[Голосовые сообщения]</b>, чтобы отобразить <code>видео-заметку</code>/<code>голосовое</code>",
     'en': "👩🏽‍💻 In the <b>[Privacy]</b> settings, add @{0} to <i>the exclusions</i> for <b>[Voice Messages]</b> to display <code>видео-заметку</code> / <code>голосовое</code>",
     'es': "👩🏽‍💻 En la configuración <b>de [Privacidad]</b> , agregue @{0} a <i>las exclusiones</i> de <b>[Mensajes de voz]</b> para mostrar <code>видео-заметку</code> / <code>голосовое</code>",
     'fr': "👩🏽‍💻 Dans les paramètres <b>[Confidentialité]</b> , ajoutez @{0} aux <i>exclusions</i> pour <b>[Messages vocaux]</b> pour afficher <code>видео-заметку</code> / <code>голосовое</code>",
     'zh': "👩🏽‍💻在<b>【隐私】</b>设置中，添加@{0}到<b>【语音消息】</b>的<i>排除项</i>中，以显示<code>видео-заметку</code> / <code>голосовое</code>",
     'ar': "👩🏽‍💻 في إعدادات <b>[الخصوصية]</b> ، أضف @ {0} إلى <i>استثناءات</i> <b>[الرسائل الصوتية]</b> لعرض <code>видео-заметку</code> / <code>голосовое</code>",
 }
 l_post_tz = {
@@ -1141,15 +1141,15 @@
     'en': "👩🏽‍💻 <b>Insert</b> a link to the Telegram channel to analyze financial performance",
     'es': "👩🏽‍💻 <b>Inserta</b> un enlace al canal de Telegram para analizar el desempeño financiero",
     'fr': "👩🏽‍💻 <b>Insérez</b> un lien vers la chaîne Telegram pour analyser les performances financières",
     'zh': "👩🏽‍💻<b>插入</b>到 Telegram 频道的链接以分析财务绩效",
     'ar': "👩🏽‍💻 <b>أدخل</b> رابطًا إلى قناة Telegram لتحليل الأداء المالي",
 }
 l_generate_wait = {
-    'ru': "👩🏽‍💻 <b>Выбери режим</b> и <b>дождись</b> окончания генерации..",
+    'ru': "👩🏽‍💻 <b>Выбери режим</b> или <b>дождись</b> окончания генерации..",
     'en': "👩🏽‍💻 <b>Wait for</b> the generation to finish..",
     'es': "👩🏽‍💻 <b>Espera a</b> que termine la generación..",
     'fr': "👩🏽‍💻 <b>Attendez que</b> la génération se termine..",
     'zh': "👩🏽‍💻<b>等待</b>生成结束..",
     'ar': "👩🏽‍💻 <b>انتظر حتى</b> ينتهي الجيل ..",
 }
 l_generate_subcribe = {
@@ -1165,15 +1165,15 @@
     'en': "👩🏽‍💻 Generation <b>Error</b>",
     'es': "👩🏽‍💻 <b>Error</b> de generación",
     'fr': "👩🏽‍💻 <b>Erreur</b> de génération",
     'zh': "👩🏽‍💻 生成<b>错误</b>",
     'ar': "👩🏽‍💻 <b>خطأ</b> في التوليد",
 }
 l_generate_errchn = {
-    'ru': "👩🏽‍💻 <b>Ошибка</b> доступа к каналу (попробуйте позже или сделайте канал публичным)",
+    'ru': "👩🏽‍💻 <b>Ошибка</b> доступа к каналу (попробуй позже или сделай канал публичным)",
     'en': "👩🏽‍💻 Channel access <b>error</b> (try again later or make the channel public)",
     'es': "👩🏽‍💻 <b>Error</b> de acceso al canal (inténtalo de nuevo más tarde o haz público el canal)",
     'fr': "👩🏽‍💻 <b>Erreur</b> d'accès à la chaîne (réessayez plus tard ou rendez la chaîne publique)",
     'zh': "👩🏽‍💻频道访问<b>错误</b>（稍后重试或公开频道）",
     'ar': "👩🏽‍💻 <b>خطأ</b> في الوصول إلى القناة (حاول مرة أخرى لاحقًا أو اجعل القناة عامة)",
 }
 # endregion
@@ -1584,15 +1584,15 @@
     'en': "👩🏽‍💻 <b>Attach</b> video to convert to GIF",
     'es': "👩🏽‍💻 <b>Adjuntar</b> video para convertir a GIF",
     'fr': "👩🏽‍💻 <b>Joindre</b> une vidéo à convertir en GIF",
     'zh': "👩🏽‍💻<b>附加</b>视频以转换为 GIF",
     'ar': "👩🏽‍💻 <b>إرفاق</b> الفيديو لتحويله إلى GIF",
 }
 l_video_transcribe_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> круглую видео-заметку (телескоп) для преобразования в текст (преобразованный формат не поддерживается)",
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> круглую видео для преобразования в текст",
     'en': "👩🏽‍💻 <b>Attach</b> a round video note (telescope) to convert to text (converted format is not supported)",
     'es': "👩🏽‍💻 <b>Adjunte</b> una nota de video redonda (telescopio) para convertir a texto (no se admite el formato convertido)",
     'fr': "👩🏽‍💻 <b>Joignez</b> une note vidéo ronde (télescope) à convertir en texte (le format converti n'est pas pris en charge)",
     'zh': "👩🏽‍💻<b>附上</b>圆形视频笔记（望远镜）转文字（不支持转换格式）",
     'ar': "<b>إرفاق</b> مذكرة فيديو مستديرة (تلسكوب) لتحويلها إلى نص (التنسيق المحول غير مدعوم)",
 }
 
@@ -1641,15 +1641,15 @@
     'en': "👩🏽‍💻 <b>Attach</b> audio to convert to voice",
     'es': "👩🏽‍💻 <b>Adjuntar</b> audio para convertir a voz",
     'fr': "👩🏽‍💻 <b>Attachez</b> l'audio pour convertir en voix",
     'zh': "👩🏽‍💻<b>附加</b>音频以转换为语音",
     'ar': "👩🏽‍💻 <b>إرفاق</b> الصوت لتحويله إلى صوت",
 }
 l_audio_transcribe_attach = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> голосовое для преобразования в текст (преобразованный формат не поддерживается)",
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> голосовое для преобразования в текст",
     'en': "👩🏽‍💻 <b>Attach</b> voice to convert to text (converted format not supported)",
     'es': "👩🏽‍💻 <b>Adjuntar</b> voz para convertir a texto (formato convertido no compatible)",
     'fr': "👩🏽‍💻 <b>Attachez</b> la voix pour convertir en texte (format converti non pris en charge)",
     'zh': "👩🏽‍💻<b>附加</b>语音转换为文本（不支持转换格式）",
     'ar': "<b>إرفاق</b> صوت لتحويله إلى نص (التنسيق المحول غير مدعوم)",
 }
 l_audio_recognize = {
@@ -1715,15 +1715,15 @@
     'es': "🗯️ Texto 4096 caracteres",
     'fr': "🗯️ Texte 4096 caractères",
     'zh': "🗯️ 文本 4096 个字符",
     'ar': "🗯️ نص 4096 حرفًا",
 }
 
 l_convert_error = {
-    'ru': "👩🏽‍💻 <b>Ошибка</b> преобразования контента (попробуйте позже ии загрузи другой файл)",
+    'ru': "👩🏽‍💻 <b>Ошибка</b> преобразования контента (попробуй позже и загрузи другой файл)",
     'en': "👩🏽‍💻 Content Conversion <b>Error</b> (Please try later and upload another file)",
     'es': "👩🏽‍💻 <b>Error</b> de conversión de contenido (intente más tarde y cargue otro archivo)",
     'fr': "👩🏽‍💻 <b>Erreur</b> de conversion de contenu (veuillez réessayer plus tard et télécharger un autre fichier)",
     'zh': "👩🏽‍💻内容转换<b>错误</b>（请稍后再试并上传另一个文件）",
     'ar': "👩🏽‍💻 <b>خطأ</b> في تحويل المحتوى (يرجى المحاولة لاحقًا وتحميل ملف آخر)",
 }
 l_telegraph_text = {
@@ -1731,15 +1731,15 @@
     'en': "👩🏽‍💻 <b>Attach</b> .jpg/.png/.gif/.mp4 content to create a link",
     'es': "👩🏽‍💻 <b>Adjunte</b> contenido .jpg/.png/.gif/.mp4 para crear un enlace",
     'fr': "👩🏽‍💻 <b>Joignez</b> du contenu .jpg/.png/.gif/.mp4 pour créer un lien",
     'zh': "👩🏽‍💻<b>附加</b>.jpg/.png/.gif/.mp4 内容以创建链接",
     'ar': "👩🏽‍💻 <b>أرفق</b> محتوى .jpg / .png / .gif / .mp4 لإنشاء ارتباط",
 }
 l_telegraph_error = {
-    'ru': "👩🏽‍💻 <b>Ошибка</b> получения ссылки (попробуйте позже ии загрузи другой файл)",
+    'ru': "👩🏽‍💻 <b>Ошибка</b> получения ссылки (попробуй позже ии загрузи другой файл)",
     'en': "👩🏽‍💻 <b>Failed</b> to get link (try later and upload another file)",
     'es': "👩🏽‍💻 <b>No se pudo</b> obtener el enlace (intente más tarde y cargue otro archivo)",
     'fr': "👩🏽‍💻 <b>Échec</b> de l'obtention du lien (essayez plus tard et téléchargez un autre fichier)",
     'zh': "👩🏽‍💻 获取链接<b>失败</b>（请稍后尝试并上传另一个文件）",
     'ar': "👩🏽‍💻 <b>فشل</b> الحصول على الرابط (حاول لاحقًا وقم بتحميل ملف آخر)",
 }
 l_json_text = {
@@ -1848,15 +1848,15 @@
     'en': "🏁 Complete",
     'es': "🏁 Completa",
     'fr': "🏁 Complet",
     'zh': "🏁 完成",
     'ar': "🏁 مكتمل",
 }
 l_media_error = {
-    'ru': "👩🏽‍💻 <b>Ошибка</b> (попробуйте позже или загрузи другое media)",
+    'ru': "👩🏽‍💻 <b>Ошибка</b> (попробуй позже или загрузи другое media)",
     'en': "👩🏽‍💻 <b>Error</b> (try later or upload another media)",
     'es': "👩🏽‍💻 <b>Error</b> (intenta más tarde o sube otro medio)",
     'fr': "👩🏽‍💻 <b>Erreur</b> (essayez plus tard ou téléchargez un autre média)",
     'zh': "👩🏽‍💻<b>错误</b>（稍后再试或上传其他媒体）",
     'ar': "👩🏽‍💻 <b>خطأ</b> (حاول لاحقًا أو قم بتحميل وسائط أخرى)",
 }
 l_media_finish = {
@@ -3366,14 +3366,22 @@
     'ru': "🕵🏽 Пользователь {0} добавлен в /ban-список (причина: <i>{1}</i>)",
     'en': "🗣 Push the ✅/☑️ to <b>On/Off</b> auto-transcribe (speach to text) for <i><b>income</b>/<b>outgoing</b> messages</i>",
     'es': "🗣 Presiona ✅/☑️ para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <i>Usuario se unió al grupo</i>",
     'fr': "🗣 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>L'utilisateur a rejoint le bote</i>",
     'zh': "🗣 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👩🏽‍💻 例如，<i>用戶加入群組</i>",
     'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👩🏽‍💻 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
 }
+l_cban_text = {
+    'ru': "🕵🏽 Жми на ✅/☑️ чтобы <b>Вкл/Выкл</b> бан <u>пользователей</u> бота: <i>с недавно зарегистрированными new-id/аккаунтов без @username/аккаунтов из <a href='https://cas.chat'>Anti-Spam Системы</a>/аккаунтов с 文-глиф, ب-араб/ <a href='https://www.zalgo.org'>zalgo-символами</a></i>\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/ban - блок/разблок пользователя\n/parse - вывести всех пользователей",
+    'en': "🕵🏽 Push the ✅/☑️ to <b>On/Off</b> <u>auto</u>-ban <i>bots with recently registered new-id/without @username/bots from <a href='https://cas.chat'>Anti-Spam System</a>/bots with 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👩🏽‍💻 For example, option <b>new-id</b> blocks bots with <i>fresh</i> <u>id</u> and with the same photo upload <u>date</u> <i>many avatars</i>",
+    'es': "🕵🏽 Presiona ✅/☑️ para <b>Encender/Apagar</b> <u>Auto</u>-banear <i>cuentas con nueva identificación registrada recientemente/cuentas eliminadas/cuentas de <a href='https://cas.chat'>Anti-Spam System</a>/cuentas con 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👩🏽‍💻 Por ejemplo, la opción <b>deleted-ban</b> elimina dichas cuentas: <i>👻 Cuenta eliminada [estafa, falsa]</i>",
+    'fr': "🕵🏽 Appuyez sur ✅/☑️ pour <b>On/Off</b> <u>auto</u>-bannir <i>les comptes avec un nouvel identifiant/des comptes supprimés/des comptes récemment enregistrés depuis <a href='https://cas.chat'>Anti-Spam System</a>/comptes avec 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👩🏽‍💻 Par exemple, l'option <b>deleted-ban</b> supprime ces comptes : <i>👻 Compte supprimé [arnaque, faux]</i>",
+    'zh': "🕵🏽 按下 ✅/☑️，以 <b>On/Off</b> <u>auto</u>-禁止 <i>具有最近從 註冊的 new-id/deleted-bots/bots <a href='https://cas.chat'>Anti-Spam System</a>/bots with text-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👩🏽‍💻 例如，選項 <b>deleted-ban</b> 刪除此類帳戶：<i>👻 Deleted bot [scam,fake]</i>",
+    'ar': "🕵🏽 اضغط على ✅ / ☑️ ، إلى <b> تشغيل / إيقاف </b> <u> تلقائي </u> -حظر <i> الحسابات ذات المعرف الجديد / الحسابات / الحسابات المحذوفة حديثًا من <a href='https://cas.chat'> نظام مكافحة البريد العشوائي </a> / حسابات مع 文 -glif، ب- arab، <a href='https://www.zalgo.org'> zalgo-icons </a> </i> \n\n👩🏽‍💻 على سبيل المثال ، الخيار <b> حذف-حظر </b> يحذف مثل هذه الحسابات: <i> 👻 الحساب المحذوف [احتيال ، وهمي] </i>",
+}
 l_cban_done = {
     'ru': "🕵🏽 Готово! /ban-список нежелательных пользователей @{0}-бота\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/ban - блок/разблок пользователя\n/parse - вывести всех пользователей\n\n👩🏽‍💻 Текущее число пользователей /ban-списка: <u>{1}</u>",
     'en': "👥 Ready! Gathered members: <u>{0}</u>. You can immediately make an <b>sending</b> or <b>inviting</b> to channel by received members{1}",
     'es': "👥 Listo! Miembros reunidos: <u>{0}</u>. Inmediatamente puede hacer un <b>envío</b> o <b>invitación</b> al grupo por miembros recibidos{1}",
     'fr': "👥 Prêt ! Membres réunis : <u>{0}</u>. Vous pouvez immédiatement faire un <b>envoi</b> ou <b>inviter</b> pour channeler par membres reçus{1}",
     'zh': "👥 準備好了！ 聚集成員：<u>{0}</u>。 您可以立即<b>發送</b>或<b>邀請</b>按收到的成員分組{1}",
     'ar': "🔥 جاهز! الأعضاء الذين تم تجميعهم: <u>{0}</u>. يمكنك على الفور إجراء <b> إرسال </b> أو <b> دعوة </b> للانضمام إلى المجموعة بواسطة الأعضاء المستلمين {1}",
@@ -3384,15 +3392,15 @@
     'es': "👥 Listo! Miembros reunidos: <u>{0}</u>. Inmediatamente puede hacer un <b>envío</b> o <b>invitación</b> al grupo por miembros recibidos{1}",
     'fr': "👥 Prêt ! Membres réunis : <u>{0}</u>. Vous pouvez immédiatement faire un <b>envoi</b> ou <b>inviter</b> pour channeler par membres reçus{1}",
     'zh': "👥 準備好了！ 聚集成員：<u>{0}</u>。 您可以立即<b>發送</b>或<b>邀請</b>按收到的成員分組{1}",
     'ar': "🔥 جاهز! الأعضاء الذين تم تجميعهم: <u>{0}</u>. يمكنك على الفور إجراء <b> إرسال </b> أو <b> دعوة </b> للانضمام إلى المجموعة بواسطة الأعضاء المستلمين {1}",
 }
 
 l_cban_handler = {
-    'ru': "🕵🏽 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <u>авто</u>-бан <i>аккаунтов с недавно зарегистрированными new-id/без @username/аккаунтов из <a href='https://cas.chat'>Anti-Spam Системы</a>/аккаунтов с 文-глиф, ب-араб, <a href='https://www.zalgo.org'>zalgo-символами</a></i>\n\n👉🏼 Например, опция <b>new-id</b> блокирует аккаунты со <i>свежим</i> <u>id</u>",
+    'ru': "🕵🏽 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <u>авто</u>-бан <i>аккаунтов с недавно зарегистрированными new-id/без @username/аккаунтов из <a href='https://cas.chat'>Anti-Spam Системы</a>/аккаунтов с 文-глиф, ب-араб/ <a href='https://www.zalgo.org'>zalgo-символами</a></i>\n\n👉🏼 Например, опция <b>new-id</b> блокирует аккаунты со <i>свежим</i> <u>id</u>",
     'en': "🕵🏽 Push the ✅/☑️, to <b>On/Off</b> <u>auto</u>-ban <i>accounts with recently registered new-id/deleted-accounts/accounts from <a href='https://cas.chat'>Anti-Spam System</a>/accounts with 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👉🏼 For example, the option <b>deleted-ban</b> delete such accounts: <i>👻 Deleted account [scam,fake]</i>",
     'es': "🕵🏽 Presiona ✅/☑️, para <b>Encender/Apagar</b> <u>Auto</u>-banear <i>cuentas con nueva identificación registrada recientemente/cuentas eliminadas/cuentas de <a href='https://cas.chat'>Anti-Spam System</a>/cuentas con 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👉🏼 Por ejemplo, la opción <b>deleted-ban</b> elimina dichas cuentas: <i>👻 Cuenta eliminada [estafa, falsa]</i>",
     'fr': "🕵🏽 Appuyez sur ✅/☑️, pour <b>On/Off</b> <u>auto</u>-bannir <i>les comptes avec un nouvel identifiant/des comptes supprimés/des comptes récemment enregistrés depuis <a href='https://cas.chat'>Anti-Spam System</a>/comptes avec 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👉🏼 Par exemple, l'option <b>deleted-ban</b> supprime ces comptes : <i>👻 Compte supprimé [arnaque, faux]</i>",
     'zh': "🕵🏽 按下 ✅/☑️，以 <b>On/Off</b> <u>auto</u>-禁止 <i>具有最近從 註冊的 new-id/deleted-accounts/accounts <a href='https://cas.chat'>Anti-Spam System</a>/accounts with text-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👉🏼 例如，選項 <b>deleted-ban</b> 刪除此類帳戶：<i>👻 Deleted account [scam,fake]</i>",
     'ar': "🕵🏽 اضغط على ✅ / ☑️ ، إلى <b> تشغيل / إيقاف </b> <u> تلقائي </u> -حظر <i> الحسابات ذات المعرف الجديد / الحسابات / الحسابات المحذوفة حديثًا من <a href='https://cas.chat'> نظام مكافحة البريد العشوائي </a> / حسابات مع 文 -glif، ب- arab، <a href='https://www.zalgo.org'> zalgo-icons </a> </i> \n\n👉🏼 على سبيل المثال ، الخيار <b> حذف-حظر </b> يحذف مثل هذه الحسابات: <i> 👻 الحساب المحذوف [احتيال ، وهمي] </i>",
 }
 l_cban_new_on = {
@@ -4243,15 +4251,15 @@
     'es': "Las 5 mejores mensajes (desde 1000)",
     'fr': "Top 5 des messages (sur 1000)",
     'zh': "前 5 條消息（來自 1000 條）",
     'ar': "أهم 5 رسائل (من 1000)",
 }
 
 l_transfer_reply = {
-    'ru': "⚠️ Используйте команду /transfer в <b>ответном</b> сообщении пользователя, которому вы хотите передать права",
+    'ru': "⚠️ Используй команду /transfer в <b>ответном</b> сообщении пользователя, которому вы хотите передать права",
     'en': "⚠️ Use /transfer-command in reply user-message to transfer him ownership",
     'es': "⚠️ Use /transfer-command en el mensaje de usuario de respuesta para transferirle la propiedad",
     'fr': "⚠️ Utilisez /transfer-command dans le message utilisateur de réponse pour lui transférer la propriété",
     'zh': "⚠️ 使用 /transfer-command 回复 user-message 轉移他的所有權",
     'ar': "استخدم الأمر transfer-command/ في الرد على رسالة المستخدم لنقل ملكيته",
 }
 l_button_handler = {
@@ -4696,15 +4704,15 @@
     'en': "👮🏽 Error of checking",
     'es': "👮🏽 Error de verificación",
     'fr': "👮🏽 Erreur de vérification",
     'zh': "👮🏽檢查錯誤",
     'ar': "👮🏽 خطأ في الفحص",
 }
 l_ccheck_wrong = {
-    'ru': "👮🏽 К сожалению, ответ неверный\n\nПопробуйте ещё раз позже",
+    'ru': "👮🏽 К сожалению, ответ неверный\n\nПопробуй ещё раз позже",
     'en': "👮🏽 Unfortunately the answer is not correct\n\nTry again later",
     'es': "👮🏽 Lamentablemente la respuesta no es correcta\n\nVuelve a intentarlo más tarde",
     'fr': "👮🏽 Malheureusement, la réponse n'est pas correcte\n\nRéessayez plus tard",
     'zh': "👮🏽 很遺憾答案不正確\n\n稍後再試",
     'ar': "👮🏽 للأسف الإجابة غير صحيحة \n\n حاول مرة أخرى لاحقًا",
 }
 l_ccheck_time = {
@@ -5106,15 +5114,15 @@
     'ar': "☑️☐ تعطيل forward-الروابط",
 }
 # endregion
 
 
 # region csymbol_
 l_csymbol_text = {
-    'ru': "文 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> <u>авто</u>-бан <i>слов с 文-глиф, ب-араб, <a href='https://www.zalgo.org'>zalgo-символами</a></i>\n\n👉🏼 Например, опция <b>zalgo-бан</b> удаляет сообщения такого вида <i>h̴̢̝̱̜͓̠̮̪̞͓͚̦͓͆͗̅̎̂͑̃̋͜e̷̡̧͙̹̥͓̣͍̰̮͙̻͍̐͒̒̍̈́̒̎̅̈́ḻ̸̨̢̘̥͛̈́̔̀̇̏̈́̂̎͠l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆̕͜͝ô̶͍̼͎͈̬̩̩̰̱͙̒͗͐̊̐̐͛̾́͗̈́̚͝͝ͅ</i>",
+    'ru': "文 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> <u>авто</u>-бан <i>слов с 文-глиф, ب-араб/ <a href='https://www.zalgo.org'>zalgo-символами</a></i>\n\n👉🏼 Например, опция <b>zalgo-бан</b> удаляет сообщения такого вида <i>h̴̢̝̱̜͓̠̮̪̞͓͚̦͓͆͗̅̎̂͑̃̋͜e̷̡̧͙̹̥͓̣͍̰̮͙̻͍̐͒̒̍̈́̒̎̅̈́ḻ̸̨̢̘̥͛̈́̔̀̇̏̈́̂̎͠l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆̕͜͝ô̶͍̼͎͈̬̩̩̰̱͙̒͗͐̊̐̐͛̾́͗̈́̚͝͝ͅ</i>",
     'en': "文 Push the ✅/☑️, to <b>On/Off</b> <u>auto</u>-ban <i>words with 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👉🏼 For example, the option <b>zalgo-ban</b> delete messages <i>h̴̢̝̱̜͓̠̮̪̞͓͚̦͓͆͗̅̎̂͑̃̋͜e̷̡̧͙̹̥͓̣͍̰̮͙̻͍̐͒̒̍̈́̒̎̅̈́ḻ̸̨̢̘̥͛̈́̔̀̇̏̈́̂̎͠l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆̕͜͝ô̶͍̼͎͈̬̩̩̰̱͙̒͗͐̊̐̐͛̾́͗̈́̚͝͝ͅ</i>",
     'es': "文 Presione ✅/☑️, para <b>Encender/Apagar</b> <u>automático</u>-prohibir <i>palabras con 文-glif, ب-arab, <a href='https://www.zalgo.org'>Zalgo-Symbols</a></i>\n\n👉🏼 Por ejemplo, la opción <b>Zalgo-ban</b> Eliminar mensajes <i>h̴̢̝̱̜͓̠̮̪̞͓͚̦͓͆͗̅̎̂͑̃̋͜e̷̡̧͙̹̥͓̣͍̰̮͙̻͍̐͒̒̍̈́̒̎̅̈́ḻ̸̷̨̢̡̧̘̥͙̹̥͓̣͍̰̮͙̻͍͛̈́̔̀̐͒̒̍̈́̒̎̅̈́ḻ̸̨̢̘̥͛̈́̔̀l̶̶̡̡̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆̔̀̾̾͛͑́̏͆̕̕͜͜͝͝</i>",
     'fr': "文 Appuyez sur ✅/☑️, pour <b>On/Off</b> <u>auto</u>-bannir <i>les mots avec 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👉🏼 Par exemple, l'option <b>zalgo-ban</b> supprimer les messages <i>h̴̢̝̱̜͓̠̮̪̞͓͚̦͓͆͗̅̎̂͑̃̋͜e̷̡̧͙̹̥͓̣͍̰̮͙̻͍̐͒̒̍̈́̒̎̅̈́ḻ̸̷̨̢̡̧̘̥͙̹̥͓̣͍̰̮͙̻͍͛̈́̔̀̐͒̒̍̈́̒̎̅̈́ḻ̸̨̢̘̥͛̈́̔̀l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆̕͜͝ô̶͍̼͎͈̬̩̩̰̱͙̒͗͐̊̐̐͛̾́͗̈́̚͝͝ͅ</i>",
     'zh': "文推 ✅/☑️, 到 <b>On/Off</b> <u>auto</u>-ban <i>words with 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👉🏼 例如，選項<b>zalgo-ban</b>刪除消息",
     'ar': "文 اضغط على ✅ / ☑️ ، من أجل تشغيل / إيقاف تلقائي - حظر الكلمات التي تحتوي على -glif ، ب- arab ، <a href ='https://www.zalgo.org'>رموز zalgo</a>\n\n👉🏼 على سبيل المثال ، الخيار <b>zalgo-ban</b> يحذف الرسائل h̴̢̝̱̜͓̠̮̪̞͓͚̦͓͆͗̅̎̂͑̃̋͜e̷̡̧͙̹̥͓̣͍̰̮͙̻͍̐͒̒̍̈́̒̎̅̈́ḻ̸̨̢̘̥͛̈́̔̀̇̏̈́̂̎͠l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆̕͜͝ô̶͍̼͎͈̬̩̩̰̱͙̒͗͐̊̐̐͛̾́͗̈́̚͝͝ͅ",
 }
 l_csymbol_symbols_on = {
@@ -6151,15 +6159,15 @@
     'en': "➕ Add bot",
     'es': "➕ Agregar grupo",
     'fr': "➕ Ajouter un bote",
     'zh': "➕ 添加組",
     'ar': "➕ إضافة مجموعة",
 }
 l_clone_bot_wait = {
-    'ru': "©️ Ожидайте окончания клонирования бота\n\n#длительность 1мин",
+    'ru': "©️ Ожидай окончания клонирования бота\n\n#длительность 1мин",
     'en': "➕ Add bot",
     'es': "➕ Agregar grupo",
     'fr': "➕ Ajouter un bote",
     'zh': "➕ 添加組",
     'ar': "➕ إضافة مجموعة",
 }
 l_addbot_handler = {
@@ -6167,14 +6175,81 @@
     'en': "➕ <b>Create</b>/<code>user extra</code> <i>Telegram</i>-bot via <b>mobile</b> app, and then send its phone <u>number</u>℡\n\n👩🏽‍💻 For example, <code>79331114545</code>",
     'es': "➕ Volver..",
     'fr': "➕ Retour..",
     'zh': "➕ 回來..",
     'ar': "🔙 رجوع ..",
 }
 
+# region commands
+l_bot_commands_handler = {
+    'ru': "⚙️ <b>Команды</b> /cmd для <b>@{0}</b>\n\n/update <i>копирование профиля</i>\n/info   <i>информация об боте</i>\n/stat   <i>аналитика бота</i>\n/status <i>статус бота</i>\n/log    <i>недавние действия</i>\n/on     <i>включить бот</i>\n<code>/off</code>    <i>выключить бот</i>\n<code>/repair</code> <i>очистка бота: чтение истории</i>\n<code>/reset</code>  <i>сброс бота: удаление диалогов</i>\n\n/parse      <i>[ссылка/id на чат] [аргумент]</i>\n/login      <i>вход в бот</i>\n/spambot    <i>карма бота</i>\n/autodel+days   <i>автоудаление 1-365 days</i>\n/delay+sec  <i>задержка авто-ответа</i>\n/join+file  <i>вступить в группы/каналы</i>\n/vote       <i>[id чата] [вариант ответа]</i>\n<code>/leaveall</code>   <i>покинуть все группы и каналы</i>\n<code>/deleteall</code>  <i>удалить все диалоги</i>\n\n# только от имени бота\n/screen <i>скриншот-уведомление</i>\n/type+сообщ     <i>печатание</i>\n/think          <i>обдумывание</i>\n<code>* отправка геопозиции возвращает @username-список</code>",
+    'en': "⚙️ <b>Account commands</b> /cmd for <b>{0}</b> in @{1} works also and in the target bot\n\n/update <i>profile copy</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/status <i>bot status</i>\n/log    <i>recent actions</i>\n/on     <i>enable bot</i>\n<code>/off</code>    <i>disable bot</i>\n<code>/repair</code> <i>accout clear: reading history</i>\n<code>/reset</code>  <i>bot reset: deleting dialogs</i>\n\n/parse      <i>[link/id on chat] [argument]</i>\n/login      <i>login to bot</i>\n/spambot    <i>bot karma</i>\n/autodel+days   <i>auto-deletion 1-365 days</i>\n/delay+sec  <i>auto-delay of auto-answer</i>\n/join+file  <i>join to groups/channels</i>\n/vote       <i>[id of chat] [option]</i>\n<code>/leaveall</code>   <i>leave all groups/channels</i>\n<code>/deleteall</code>  <i>delete all dialogs</i>\n\n# only from bot name\n/screen <i>screenshort-nortification</i>\n/type+msg     <i>typing</i>\n/think          <i>thinking</i>\n<code>* geo-location sending returns @username-list</code>",
+    'es': "⚙️ Configuración de <b>Grupo</b> de <b>{0}</b>{1}\n\n<b>⛏ Comandos de administración @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-bots</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from bot for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in bot for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-bots</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for bot</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
+    'fr': "⚙️ Paramètres de <b>bote</b> de <b>{0}</b>{1}\n\n<b>⛏ Commandes d'administration @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-bots</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from bot for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in bot for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-bots</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for bot</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
+    'zh': "⚙️ <b>組</b>設置 <b>{0}</b>{1}\n\n<b>⛏ 管理員命令 @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-bots</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from bot for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in bot for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-bots</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for bot</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
+    'ar': "⚙️ إعدادات <b> المجموعة </b> الخاصة بـ <b>{0}</b>{1}\n\n<b>⛏ أوامر المسؤول @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-bots</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from bot for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in bot for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-bots</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for bot</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
+}
+l_bot_status_handler = {
+    'ru': "👩🏽‍💻 Бот-статус: {0}",
+    'en': "👩🏽‍💻 Account-status: {0}",
+    'es': "🎉 Enviar este comando como respuesta al mensaje",
+    'fr': "🎉 Envoyez cette commande en réponse au message",
+    'zh': "🎉 將此命令作為對消息的回復發送",
+    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
+}
+l_bot_on_handler = {
+    'ru': "👩🏽‍💻 Начинаем запуск бота..\n\n#длительность 1мин",
+    'en': "👩🏽‍💻 Begin to start bot..\n\n#duration 1min",
+    'es': "🎉 Enviar este comando como respuesta al mensaje",
+    'fr': "🎉 Envoyez cette commande en réponse au message",
+    'zh': "🎉 將此命令作為對消息的回復發送",
+    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
+}
+l_bot_on_handler_already = {
+    'ru': "👩🏽‍💻 Бот уже запущен",
+    'en': "👩🏽‍💻 Account have already started",
+    'es': "🎉 Enviar este comando como respuesta al mensaje",
+    'fr': "🎉 Envoyez cette commande en réponse au message",
+    'zh': "🎉 將此命令作為對消息的回復發送",
+    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
+}
+l_bot_off_handler = {
+    'ru': "👩🏽‍💻 Завершаем сессию бота {0}..\n\n#длительность 1мин",
+    'en': "👩🏽‍💻 Finishing bot-session {0}..\n\n#duration 1min",
+    'es': "🎉 Enviar este comando como respuesta al mensaje",
+    'fr': "🎉 Envoyez cette commande en réponse au message",
+    'zh': "🎉 將此命令作為對消息的回復發送",
+    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
+}
+l_bot_off_handler_already = {
+    'ru': "👩🏽‍💻 Бот уже выключен",
+    'en': "👩🏽‍💻 Account have already finished",
+    'es': "🎉 Enviar este comando como respuesta al mensaje",
+    'fr': "🎉 Envoyez cette commande en réponse au message",
+    'zh': "🎉 將此命令作為對消息的回復發送",
+    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
+}
+l_bot_off_handler_done = {
+    'ru': "👩🏽‍💻 Бот выключен",
+    'en': "👩🏽‍💻 Account is off",
+    'es': "🎉 Enviar este comando como respuesta al mensaje",
+    'fr': "🎉 Envoyez cette commande en réponse au message",
+    'zh': "🎉 將此命令作為對消息的回復發送",
+    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
+}
+l_bot_restart_handler = {
+    'ru': "👩🏽‍💻 Перезапуск бота {0}..\n\n#длительность 1мин",
+    'en': "👩🏽‍💻 Restart of bot-session {0}..\n\n#duration 1min",
+    'es': "🎉 Enviar este comando como respuesta al mensaje",
+    'fr': "🎉 Envoyez cette commande en réponse au message",
+    'zh': "🎉 將此命令作為對消息的回復發送",
+    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
+}
+# endregion
+
 # region bot
 l_bot_config = {
     ("cctor", "👩🏽‍💻", "☑"): {
         'ru': "Конструктор ᴺᴱᵂ",
         'en': "Builder ᴺᴱᵂ",
         'es': "Builder ᴺᴱᵂ",
         'fr': "Builder ᴺᴱᵂ",
@@ -6367,159 +6442,22 @@
     'zh': "☑️☐關閉新身份證",
     'ar': "☑️☐ تعطيل حظر معرف جديد",
 }
 # endregion
 
 
 # region canswer_
-l_canswer_alert = {
-    'ru': "👋🏽 Нужно ⚙️Настроить хотя бы один триггер",
-    'en': "👋🏽 You have to ⚙️Configure at least one trigger",
-    'es': "👋🏽 Tienes que ⚙️ Configurar al menos una palabra de inicio",
-    'fr': "👋🏽 Vous devez ⚙️ Configurer au moins un mot de départ",
-    'zh': "👋🏽 你必須 ⚙️ 配置至少一個起始詞",
-    'ar': "🔔 يجب عليك ⚙️ تكوين كلمة بداية واحدة على الأقل",
-}
 l_canswer_text = {
-    'ru': "👋🏽 Жми на ✅/☑️ чтобы <b>Вкл/Выкл</b> режим авто-ответа на триггеры\n\n👩🏽‍💻 Общее число триггеров: <u>{0}</u>",
+    'ru': "👋🏽 Жми на ✅/☑️ чтобы <b>Вкл/Выкл</b> режим авто-ответа на текстовые сообщения с помощью нейросети",
     'en': "👋🏽 Push the ✅/☑️ to <b>On/Off</b> auto-answer on triggers\n\n👩🏽‍💻 Current number of triggers: <u>{0}</u>",
     'es': "👋🏽 Presiona ✅/☑️ para <b>Activar/Desactivar</b> la respuesta automática en mensajes desencadenantes, que contienen palabras de inicio específicas\n\n👩🏽‍💻 Número actual de palabras de inicio <u>{0}</u>",
     'fr': "👋🏽 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> la réponse automatique aux messages déclencheurs, contenant des mots de départ spécifiques\n\n👩🏽‍💻 Nombre actuel de mots de départ <u>{0}</u>",
     'zh': "👋🏽 將 ✅/☑️ 推到 <b>On/Off</b> 觸發消息上的自動應答，包含特定的起始詞\n\n👩🏽‍💻 當前起始詞的數量<u>{0}</u>",
     'ar': "🚀 اضغط على ✅ / ☑️ ، لإجراء تشغيل / إيقاف الرد التلقائي على الرسائل المشغلة ، التي تحتوي على كلمات بداية محددة \n\n👩🏽‍💻 العدد الحالي لكلمات البداية {0} / ش",
 }
-l_canswerconfigtext = {
-    'ru': "👋🏽 Выбери пост, который будет использован для авто-ответа и жми <b>[{0}]</b> под выбранным постом\n\n👩🏽‍💻 <b>Общее</b> число триггеров: <u>{1}</u>",
-    'en': "👋🏽 Choose post for auto-answer and push the [{0}] under the choosen post\n\n👩🏽‍💻 Total number of triggers: <u>{1}</u>",
-    'es': "👋🏽 Al principio, elija la respuesta automática (de las publicaciones), que se enviará en respuesta a las palabras de inicio",
-    'fr': "👋🏽 Dans un premier temps, choisissez la réponse automatique (à partir des messages), qui sera envoyée en réponse aux mots de départ",
-    'zh': "👋🏽 首先，選擇自動回复（來自帖子），它將響應起始詞發送",
-    'ar': "🚀 في البداية ، اختر الرد التلقائي (من المشاركات) ، والذي سيتم إرساله ردًا على كلمات البداية",
-}
-l_canswerconfig_use = {
-    'ru': "👋🏽 Использовать",
-    'en': "👋🏽 Use",
-    'es': "👋🏽 Uso",
-    'fr': "👋🏽 Utiliser",
-    'zh': "👋🏽 使用",
-    'ar': "🚀 استخدم",
-}
-l_cansweroperationcaption = {
-    'ru': "👋🏽 <b>Текущее</b> число <i>триггеров</i> для поста #{0} в <code>{1}</code>-файле: <u>{2}</u>\n\n👩🏽‍💻 Жми на ✅/🚫, чтобы <b>Добавить/Удалить</b> триггер",
-    'en': "👋🏽 Current number of triggers for post #{0} in <code>{1}</code>-file: <u>{2}</u>\n\nPush the ✅/🚫, to <b>Add/Remove</b> triggers",
-    'es': "👋🏽 Número actual de palabras iniciales para la publicación #{0} en el archivo <code>{1}</code>: <u>{2}</u>\n\nPulse el ✅/🚫, para <b> Agregar o quitar</b> palabras de inicio",
-    'fr': "👋🏽  Nombre actuel de mots de départ pour le message #{0} dans le fichier <code>{1}</code> : <u>{2}</u>\n\nAppuyez sur le ✅/🚫 pour <b> Ajouter/supprimer</b> des mots de départ",
-    'zh': "👋🏽 當前的起始詞數 在 <code>{1}</code>-文件中發布 #{0}：<u>{2}</u>\n\n點擊 ✅/🚫，開始<b>添加/刪除</b> -字",
-    'ar': "🚀 العدد الحالي لكلمات البداية للنشر # {0} في <code>{1}</code> -الملف:{2} \n\n قم بإرسال ✅/🚫 إلى إضافة / إزالة كلمات البداية",
-}
-l_cansweroperationtext = {
-    'ru': "👋🏽 <b>Текущее</b> число <i>триггеров</i> для поста #{0}: <u>{1}</u>\n\n👩🏽‍💻 Жми на ✅/🚫, чтобы <b>Добавить/Удалить</b> триггер",
-    'en': "👋🏽 Current number of triggers for post #{0}: <u>{2}</u>\n\nPush the ✅/🚫 to <b>Add/Remove</b> trigger",
-    'es': "👋🏽 Número actual de palabras de inicio para la publicación #{0}: <u>{2}</u>\n\nPresione ✅/🚫 para <b>Agregar/Quitar</b> palabras de inicio",
-    'fr': "👋🏽  Nombre actuel de mots de départ pour le message #{0} : <u>{2}</u>\n\nAppuyez sur le ✅/🚫 pour <b>ajouter/supprimer</b> des mots de départ",
-    'zh': "👋🏽 帖子 #{0} 的當前起始詞數：<u>{2}</u>\n\n點擊 ✅/🚫，以<b>添加/刪除</b>個起始詞",
-    'ar': "🚀 العدد الحالي لكلمات البداية للنشر # {0}:{2}\n\n استخدم ✅/🚫 ، من أجل <b> إضافة / إزالة </b> كلمات البداية",
-}
-l_cansweroperation_add = {
-    'ru': "\n\n▪️регистр не важен\n▪️поставь *-звездочку после слова, чтобы учитывать вхождение\n▪️например, если ввести <b>психо*</b>, то авто-ответ сработает на <u>все</u> сообщения, которые <b>содержат</b> данное сочетание: <i>анти<u>психо</u>лог, <u>Психо</u>терапевт</i>",
-    'en': "\n\n▪️word case is not important\n▪️set * after word to bot for occurrence\n▪️for example, if write <b>psy*</b>, then <u>all</u> messages, which are <b>contained</b> this combination of letters will be removed: <i>anti-<u>psy</u>chologist, <u>Psy</u>chotherapist..</i>",
-    'es': "\n\n▪️las mayúsculas y minúsculas no son importantes\n▪️establezca * después de la palabra para tener en cuenta la ocurrencia\n▪️por ejemplo, si escribe <b>psi*</b>, entonces <u>todos</u> los mensajes, que están <b>contenidos</b> se eliminará esta combinación de letras: <i>anti-<u>psicólogo</u>, <u>Psi</u>coterapeuta..</i>",
-    'fr': "\n\n▪️la casse des mots n'est pas importante\n▪️définissez * après le mot pour tenir compte de l'occurrence\n▪️par exemple, si écrivez <b>psy*</b>, alors <u>tous</u> les messages, qui sont <b>contenues</b> cette combinaison de lettres sera supprimée : <i>anti-<u>psychologue</u>, <u>Psy</u>chothérapeute..</i>",
-    'zh': "\n\n▪️單詞大小寫不重要\n▪️在單詞之後設置*以說明出現\n▪️例如，如果寫<b>psy*</b>，則<u>所有</u>消息， <b>包含</b>這些字母組合將被刪除：<i>anti-<u>psy</u>chologist, <u>Psy</u>chotherapy..</i>",
-    'ar': "\n\n▪️ حالة الكلمة ليست مهمة \n▪️ اضبط * بعد كلمة لحساب الحدوث \n▪️ على سبيل المثال ، إذا كتبت <b>psy*</b> ، ثم <u> كل </u> الرسائل ، التي <b> احتوت </b> ستتم إزالة هذه المجموعة من الأحرف:",
-}
-l_cansweroperation_words = {
-    'ru': "👋🏽 Введи <u>триггер-слова</u> <b>через</b> пробелы или разделители, в ответ на которые будет приходить пост #<u>{0}</u>{1}",
-    'en': "👋🏽 Enter <u>trigger-words</u> <b>via</b> spaces or separators for auto-answer to post #<u>{0}</u>{1}",
-    'es': "👋🏽 Ingrese <u>palabras de inicio</u> <b>mediante</b> espacios o separadores para <i>agregarlos</i> a la Base{0}",
-    'fr': "👋🏽 Saisissez des <u>start-words</u> <b>via</b> des espaces ou des séparateurs pour les <i>ajouter</i> à Base{0}",
-    'zh': "👋🏽 輸入 <u>start-words</u> <b>via</b> 空格或分隔符以將它們<i>添加</i>到 Base{0}",
-    'ar': "✅ أدخل كلمات البداية عبر مسافات أو فواصل من أجل <i> إضافتها </i> إلى القاعدة {0}",
-}
-l_cansweroperationnoanswer = {
-    'ru': "🚫 Выбери <b>триггер</b> для отключения <i>авто-ответа</i>:",
-    'en': "🚫 Choose <b>trigger</b> for disable <i>auto-answer</i>:",
-    'es': "🚫 Ingrese <u>palabras de inicio</u> <b>mediante</b> espacios o separadores para <i>eliminarlos</i> de la Base{0}",
-    'fr': "🚫 輸入 <u>start-words</u> <b>via</b> 空格或分隔符以將它們從 Base 中<i>刪除</i>{0}",
-    'zh': "🚫 輸入 <u>start-words</u> <b>via</b> 空格或分隔符以將它們從 Base 中<i>刪除</i>{0}",
-    'ar': "🚫 أدخل كلمات البداية عبر مسافات أو فواصل <i> لإزالتها </i> من Base {0}",
-}
-l_fsmAnswer_add_caption = {
-    'ru': "👋🏽 Готово! <b>Текущее</b> число триггеров для поста #{0} в <code>{1}</code>-файле: <u>{2}</u>\n\n👩🏽‍💻 Жми на ✅/🚫, чтобы <b>Добавить/Удалить</b> триггер",
-    'en': "👋🏽 Ready! <b>Current</b> count of triggers for post #{0} in <code>{1}</code>-file: <u>{2}</u>\n\n👩🏽‍💻 Push the ✅/🚫 to <b>Add/Remove</b> trigger",
-    'es': "👋🏽 Listo! Número <b>actual</b> de palabras de inicio para la publicación #{0} en el archivo <code>{1}</code>: <u>{2}</u>",
-    'fr': "👋🏽 Prêt ! <b>Nombre actuel</b> de mots de départ pour le message  #{0} dans le fichier <code>{1}</code> : <u>{2}</u>",
-    'zh': "👋🏽 準備好了！ <code>{1}</code>-文件中帖子 #{0} 的<b>當前</b> 起始字數：<u>{2}</u>",
-    'ar': "🚀 جاهز! <b> العدد </b> الحالي لكلمات البداية للمشاركة # {0} في <code>{1}</code> -ملف:<u>{2}</u>",
-}
-
-l_canswer_handler_btn = {
-    'ru': "🔣 Нажатие на кнопку",
-    'en': "🔣 Pushing on the button",
-    'es': "🎉 Enviar este comando como respuesta al mensaje",
-    'fr': "🎉 Envoyez cette commande en réponse au message",
-    'zh': "🎉 將此命令作為對消息的回復發送",
-    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
-}
-l_canswer_handler_txt = {
-    'ru': "🔡 Текст содержится",
-    'en': "🔡 Text is contained",
-    'es': "🎉 Enviar este comando como respuesta al mensaje",
-    'fr': "🎉 Envoyez cette commande en réponse au message",
-    'zh': "🎉 將此命令作為對消息的回復發送",
-    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
-}
-l_canswer_no_triggers = {
-    'ru': "👋🏽 Для поста #{0} триггеры отсутствуют",
-    'en': "👋🏽 There are no triggers for post #{0}",
-    'es': "🎉 Enviar este comando como respuesta al mensaje",
-    'fr': "🎉 Envoyez cette commande en réponse au message",
-    'zh': "🎉 將此命令作為對消息的回復發送",
-    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
-}
-l_canswer_push_triggers = {
-    'ru': "👋🏽 Жми на ❌, чтобы удалить триггер для поста #<u>{0}</u>",
-    'en': "👋🏽 Push the ❌ to remove trigger for post #<u>{0}</u>",
-    'es': "🎉 Enviar este comando como respuesta al mensaje",
-    'fr': "🎉 Envoyez cette commande en réponse au message",
-    'zh': "🎉 將此命令作為對消息的回復發送",
-    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
-}
-l_canswer_choose_btn = {
-    'ru': "👩🏽‍💻 Выбери одну из <b>кнопок</b>, нажав на которую, пользователю придет пост #<u>{0}</u>",
-    'en': "👩🏽‍💻 Choose one of the <b>button</b>, pushing on which, user will receive post #<u>{0}</u>",
-    'es': "🎉 Enviar este comando como respuesta al mensaje",
-    'fr': "🎉 Envoyez cette commande en réponse au message",
-    'zh': "🎉 將此命令作為對消息的回復發送",
-    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
-}
-l_canswer_add_trigger = {
-    'ru': "👋🏽 Готово! Триггер ({0}): <b>{1}</b> добавлен для поста #{2}\n\n👩🏽‍💻 <b>Текущее</b> число триггеров для поста #{2}: <u>{3}</u>",
-    'en': "👋🏽 Ready! Trigger ({0}): <b>{1}</b> has added for post #{2}\n\n👩🏽‍💻 <b>Current</b> count of triggers for post #{2}: <u>{3}</u>",
-    'es': "🎉 Enviar este comando como respuesta al mensaje",
-    'fr': "🎉 Envoyez cette commande en réponse au message",
-    'zh': "🎉 將此命令作為對消息的回復發送",
-    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
-}
-l_canswer_trigger_choose = {
-    'ru': "👋🏽 Выбери <b>триггер</b>, в ответ на который будет присылаться пост #<u>{0}</u>",
-    'en': "👋🏽 Choose <b>trigger</b> for post #<u>{0}</u>",
-    'es': "💳 Agregar grupo",
-    'fr': "💳 Ajouter un bote",
-    'zh': "💳 添加組",
-    'ar': "💳 إضافة مجموعة",
-}
-l_canswer_trigger_without_url_buttons = {
-    'ru': "👩🏽‍💻 Создай хотя бы один пост с кнопками без url-ссылок",
-    'en': "👩🏽‍💻 Create at least one post with buttons without url-links",
-    'es': "💳 Agregar grupo",
-    'fr': "💳 Ajouter un bote",
-    'zh': "💳 添加組",
-    'ar': "💳 إضافة مجموعة",
-}
 # endregion
 
 
 # region cpayment_
 l_cpayment_alert = {
     'ru': "💳️ Нужно ⚙️Настроить хотя бы один платежный токен",
     'en': "🗝️ You have to ⚙️Configure post and source for sending",
@@ -6553,23 +6491,23 @@
     'ar': "🗝️ ادفع ✅ / ☑️ إلى <b> تشغيل / إيقاف </b> لدعوة المستخدمين تلقائيًا إلى مجموعتك \n\n👩🏽‍💻 دعوة <u>{0}</u> مستخدمين يوميًا من المجموعة {1}",
 }
 # endregion
 
 
 # region cintegration_
 l_cintegration_alert = {
-    'ru': "🗝️ Нужно ⚙️Настроить ТОКЕН доступа к CRM",
+    'ru': "🗝️ Нужно ⚙️Настроить ССЫЛКУ доступа",
     'en': "🗝️ You have to ⚙️Configure post and source for sending",
     'es': "🗝️ Tienes que ⚙️ Configurar al menos una palabra de inicio",
     'fr': "🗝️ Vous devez ⚙️ Configurer au moins un mot de départ",
     'zh': "🗝️ 你必須 ⚙️ 配置至少一個起始詞",
     'ar': "🔔 يجب عليك ⚙️ تكوين كلمة بداية واحدة على الأقل",
 }
 l_cintegration_text = {
-    'ru': "🗝️ Жми на ✅/☑️ чтобы <b>Вкл/Выкл</b> интеграцию базы пользователей с <i><b>google</b>-crm/<b>airtable</b>-crm</i>\n\n👩🏽‍💻 Например, опция [<b>{0}</b>] означает возможность интеграции базы пользователей с <i>google-crm</i>, а также синхронизацию <i>google-календаря</i> с @{1}-ботом",
+    'ru': "🗝️ Жми на ✅/☑️ чтобы <b>Вкл/Выкл</b> интеграцию базы пользователей с <i><b>google</b>-crm/<b>airtable</b>-crm</i>\n\n👩🏽‍💻 Например, опция [<b>{0}</b>] означает возможность интеграции базы пользователей с <i>google-crm</i>",
     'en': "🗝️ Push the ✅/☑️ to <b>On/Off</b> auto-sending choosen post to many users\n\n👩🏽‍💻 <b>Current</b> settings of auto-sending: {0}",
     'es': "🗝️ Presiona ✅/☑️ para <b>activar/desactivar</b> la invitación automática de usuarios a tu grupo\n\n👩🏽‍💻 Invitar a <u>{0}</u> usuarios por día del grupo {1}",
     'fr': "🗝️ Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> l'invitation automatique d'utilisateurs dans votre bote\n\n👩🏽‍💻 Inviter <u>{0}</u> utilisateurs par jour à partir du bote {1}",
     'zh': "🗝️ 按下 ✅/☑️ 以<b>開/關</b>自動邀請用戶加入您的群組\n\n👩🏽‍💻 每天從群組 {1} 中邀請 <u>{0}</u> 個用戶",
     'ar': "🗝️ ادفع ✅ / ☑️ إلى <b> تشغيل / إيقاف </b> لدعوة المستخدمين تلقائيًا إلى مجموعتك \n\n👩🏽‍💻 دعوة <u>{0}</u> مستخدمين يوميًا من المجموعة {1}",
 }
 
@@ -6631,15 +6569,15 @@
     'ar': "🗝️ ادفع ✅ / ☑️ إلى <b> تشغيل / إيقاف </b> لدعوة المستخدمين تلقائيًا إلى مجموعتك \n\n👩🏽‍💻 دعوة <u>{0}</u> مستخدمين يوميًا من المجموعة {1}",
 }
 # endregion
 
 
 # region cnotification_
 l_cnotification_text = {
-    'ru': "💬 Жми на ✅/☑️ чтобы <b>Вкл/Выкл</b> оповещения о <i><b>/start-stop</b> запуске/блокировке бота пользователем и попадании пользователя в <b>/ban</b>-список/<b>нажатии</b> на кнопки пользователем/<b>диалоге</b> с администраторами/<b>всех</b> действиях пользователя</i>\n\n👩🏽‍💻 Например, опция [<b>{0}</b>] означает <code>показ</code> сообщений от пользователя администраторам бота (/admin) с возможностью реплай-ответа на сообщения (*рекомендуется)",
+    'ru': "💬 Жми на ✅/☑️ чтобы <b>Вкл/Выкл</b> оповещения о <i><b>/start-stop</b> запуске/блокировке бота пользователем и попадании пользователя в <b>/ban</b>-список/<b>нажатии</b> на кнопки пользователем/<b>диалоге</b> с администраторами/<b>всех</b> действиях пользователя</i>\n\n👩🏽‍💻 Например, опция [<b>{0}</b>] означает <code>показ</code> сообщений от пользователя администраторам бота (/admin) с возможностью реплай-ответа на сообщения",
     'en': "💬 Push the ✅/☑️ to <b>On/Off</b> <i>service <b>statuses</b>/<b>forward</b> income for yourself (including original/<u>deleted</u> messages)/tag about income-<b>reading</b></i>\n\n👩🏽‍💻 For example, [{0}] means <code>show</code> service <b>statuses</b>: <i>typing..search sticker..</i>",
     'es': "💬 Presiona ✅/☑️ para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <i>Usuario se unió al grupo</i>",
     'fr': "💬 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>L'utilisateur a rejoint le bote</i>",
     'zh': "💬 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👩🏽‍💻 例如，<i>用戶加入群組</i>",
     'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👩🏽‍💻 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
 }
 l_cnotification_start_on = {
@@ -6772,14 +6710,22 @@
     'ru': "☑️☐Выкл utm-рефералы",
     'en': "☑️☐Off reaction to media",
     'es': "☑️☐De nueva-id-ban",
     'fr': "☑️☐De nouveau-id-ban",
     'zh': "☑️☐關閉新身份證",
     'ar': "☑️☐ تعطيل حظر معرف جديد",
 }
+l_bot_is_off = {
+    'ru': "👩🏽‍💻 <b>Бот:</b> выключен\n\n/on - включить бот",
+    'en': "👩🏽‍💻 <b>Account:</b> is off\n\n/on - to on bot",
+    'es': "💳 Agregar grupo",
+    'fr': "💳 Ajouter un bote",
+    'zh': "💳 添加組",
+    'ar': "💳 إضافة مجموعة",
+}
 l_cuser_utm = {
     'ru': "👥 Готово! <b>/utm-список</b> реферальных пользователей @{0}-бота\n\n👩🏽‍💻 <b>Вывести</b> рефералов конкретного пользователя можно командой:\n<code>/utm id</code> или <code>/utm @username</code>\n\n👩🏽‍💻 Текущее число utm-рефералов: <u>{1}</u>",
     'en': "👥 Ready! Gathered members: <u>{0}</u>. You can immediately make an <b>sending</b> or <b>inviting</b> to channel by received members{1}",
     'es': "👥 Listo! Miembros reunidos: <u>{0}</u>. Inmediatamente puede hacer un <b>envío</b> o <b>invitación</b> al grupo por miembros recibidos{1}",
     'fr': "👥 Prêt ! Membres réunis : <u>{0}</u>. Vous pouvez immédiatement faire un <b>envoi</b> ou <b>inviter</b> pour channeler par membres reçus{1}",
     'zh': "👥 準備好了！ 聚集成員：<u>{0}</u>。 您可以立即<b>發送</b>或<b>邀請</b>按收到的成員分組{1}",
     'ar': "🔥 جاهز! الأعضاء الذين تم تجميعهم: <u>{0}</u>. يمكنك على الفور إجراء <b> إرسال </b> أو <b> دعوة </b> للانضمام إلى المجموعة بواسطة الأعضاء المستلمين {1}",
```

### Comparing `yeref-0.1.55/yeref/yeref.py` & `yeref-0.1.56/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,16 +208,16 @@
         for item in pages['pages']:
             try:
                 if item['path'] == 'ban-04-11-7':
                     page = telegraph_.get_page(path=item['path'], return_content=True, return_html=True)
                     ban_ids = str(page['content']).split()
 
                     if str(chat_id) in ban_ids:
-                        return True
-                    break
+                        result = True
+                    return
             except Exception as e:
                 logger.info(log_ % str(e))
                 await asyncio.sleep(round(random.uniform(0, 1), 2))
 
         # telegraph_ = Telegraph(access_token=TGPH_TOKEN_MAIN)
         # html_ = {'one': '1', 'two': '2'}
         # html_ = json.dumps(html_, ensure_ascii=False)
```

