# Comparing `tmp/yeref-0.1.65.tar.gz` & `tmp/yeref-0.1.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.65.tar", last modified: Sun May 21 14:12:47 2023, max compression
+gzip compressed data, was "yeref-0.1.66.tar", last modified: Fri May 26 17:59:17 2023, max compression
```

## Comparing `yeref-0.1.65.tar` & `yeref-0.1.66.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-21 14:12:47.548693 yeref-0.1.65/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-21 14:12:47.548840 yeref-0.1.65/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-21 14:12:47.549407 yeref-0.1.65/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1351 2023-05-21 14:12:35.000000 yeref-0.1.65/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-21 14:12:47.542591 yeref-0.1.65/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.65/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   511251 2023-05-09 14:24:53.000000 yeref-0.1.65/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   204673 2023-05-21 14:10:12.000000 yeref-0.1.65/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-21 14:12:47.548301 yeref-0.1.65/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-21 14:12:47.000000 yeref-0.1.65/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-21 14:12:47.000000 yeref-0.1.65/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-21 14:12:47.000000 yeref-0.1.65/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-21 14:12:47.000000 yeref-0.1.65/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-26 17:59:17.559635 yeref-0.1.66/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-26 17:59:17.559863 yeref-0.1.66/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-26 17:59:17.562327 yeref-0.1.66/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1351 2023-05-26 17:59:04.000000 yeref-0.1.66/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-26 17:59:17.552749 yeref-0.1.66/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.66/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   489150 2023-05-26 17:58:09.000000 yeref-0.1.66/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   204673 2023-05-25 18:35:58.000000 yeref-0.1.66/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-26 17:59:17.559029 yeref-0.1.66/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-26 17:59:17.000000 yeref-0.1.66/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-26 17:59:17.000000 yeref-0.1.66/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-26 17:59:17.000000 yeref-0.1.66/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-26 17:59:17.000000 yeref-0.1.66/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.65/setup.py` & `yeref-0.1.66/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.65',
+      version='0.1.66',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.1.65/yeref/l_.py` & `yeref-0.1.66/yeref/l_.py`

 * *Files 7% similar despite different names*

```diff
@@ -171,15 +171,15 @@
     'ar': "💔 مثل",
 }
 # endregion
 
 
 # region post
 l_post_text = {
-    'ru': "✏️ 1. Напиши мне <b>текст</b> для нового поста (не забудь использовать <i>форматирование</i>)\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
+    'ru': "✏️ 1. Напиши <b>текст</b> для нового поста (не забудь использовать <i>форматирование</i>)\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
     'en': "✏️ 1. <b>Text</b> me for a new post (don&#x27;t forget to use <i>formatting</i> )\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
     'es': "✏️ 1. <b>Envíame un mensaje de texto</b> para una nueva publicación (no olvides usar <i>formato</i> )\n\n( <i>o presiona &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
     'fr': "✏️ 1. <b>Envoyez</b> -moi un SMS pour un nouveau message (n&#x27;oubliez pas d&#x27;utiliser <i>le formatage</i> )\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
     'zh': "✏️ 1.<b>发短信</b>给我（不要忘记使用<i>格式</i>）\n\n（<i>或按“➡️️/下一步”跳过此步骤</i>）",
     'ar': "✏️ 1. <b>أرسل</b> لي رسالة نصية لمنشور جديد (لا تنس استخدام <i>التنسيق</i> )\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لتخطي هذه الخطوة</i> )",
 }
 l_post_text_limit = {
@@ -187,15 +187,15 @@
     'en': "❗️ Number of <b>characters</b> of text ( <i>including formatting</i> ): <u>{0}</u> more than allowed 1024",
     'es': "❗️ Número de <b>caracteres</b> de texto ( <i>incluido el formato</i> ): <u>{0}</u> más de los permitidos 1024",
     'fr': "❗️ Nombre de <b>caractères</b> de texte ( <i>y compris le formatage</i> ) : <u>{0}</u> plus que autorisé 1024",
     'zh': "❗️ 文本<b>字符</b>数（<i>包括格式</i>）： <u>{0}</u>超过允许的 1024",
     'ar': "❗️ عدد <b>أحرف</b> النص ( <i>بما في ذلك التنسيق</i> ): <u>{0}</u> أكثر من العدد المسموح به وهو 1024",
 }
 l_post_text_empty = {
-    'ru': "❗️ пост пустой, попробуй сначала\n\n{0}",
+    'ru': "❗️ Пост пустой, попробуй сначала\n\n{0}",
     'en': "❗️ post is empty, try again\n\n{0}",
     'es': "❗️ la publicación está vacía, inténtalo de nuevo\n\n{0}",
     'fr': "❗️ la publication est vide, réessayez\n\n{0}",
     'zh': "❗️ 帖子为空，请重试\n\n{0}",
     'ar': "❗️ المنشور فارغ ، حاول مرة أخرى\n\n{0}",
 }
 l_post_edit = {
@@ -211,15 +211,15 @@
     'en': "✏️ 2. Attach <b>media</b> content: photo/gif/video/audio/document/sticker or write a voice/video note in a circle\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
     'es': "✏️ 2. Adjunte contenido <b>multimedia</b> : foto/gif/video/audio/documento/pegatina o escriba una nota de voz/video en un círculo\n\n( <i>o presione &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
     'fr': "✏️ 2. Joignez du contenu <b>multimédia</b> : photo/gif/vidéo/audio/document/autocollant ou écrivez une note vocale/vidéo dans un cercle\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
     'zh': "✏️ 2.附上<b>媒体</b>内容：照片/gif/视频/音频/文档/贴纸或在圈内写语音/视频备注\n\n（<i>或按“➡️️/下一步”跳过此步骤</i>）",
     'ar': "✏️ 2. أرفق محتوى <b>وسائط</b> : صورة / gif / فيديو / صوت / مستند / ملصق أو اكتب ملاحظة صوتية / فيديو في دائرة\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لتخطي هذه الخطوة</i> )",
 }
 l_post_media_wait = {
-    'ru': "👩🏽‍💻 Ожидай обработки {0}..\n#длительность {1}мин",
+    'ru': "👩🏽‍💻 <b>Обработка</b> {0}..\n#длительность {1}мин",
     'en': "👩🏽‍💻 Wait for processing {0}..\n#duration {1}min",
     'es': "👩🏽‍💻 Espere a que se procese {0}..\n#duration {1}min",
     'fr': "👩🏽‍💻 Attendez le traitement {0}..\n#duration {1}min",
     'zh': "👩🏽‍💻 等待处理 {0}..\n#duration {1}min",
     'ar': "👩🏽‍💻 انتظر المعالجة {0} ..\n# مدة {1} دقيقة",
 }
 l_post_media_toobig = {
@@ -565,39 +565,39 @@
     'en': "📍 Location <b>time zone</b> set\n\n🕐 Current time: <u>{0}</u> ({1}{2} GMT)",
     'es': "📍 Configuración <b>de la zona horaria</b> de la ubicación\n\n🕐 Hora actual: <u>{0}</u> ({1}{2} GMT)",
     'fr': "📍 <b>Fuseau horaire</b> de l&#x27;emplacement défini\n\n🕐 Heure actuelle : <u>{0}</u> ({1}{2} GMT)",
     'zh': "📍 位置<b>时区</b>设置\n\n🕐 当前时间： <u>{0}</u> （{1}{2} GMT）",
     'ar': "📍 تعيين <b>المنطقة الزمنية</b> للموقع\n\n🕐 الوقت الحالي: <u>{0}</u> ({1} {2} GMT)",
 }
 l_broadcast_plan = {
-    'ru': "🗝️ <b>Готово!</b> Рассылка запланирована",
+    'ru': "📧 <b>Готово!</b> Рассылка запланирована",
     'en': "🗝️ <b>Done!</b> Newsletter scheduled",
     'es': "🗝️ <b>Listo!</b> Boletín programado",
     'fr': "🗝️ <b>C&#x27;est fait !</b> Newsletter prévue",
     'zh': "🗝️<b>完成！</b>已安排时事通讯",
     'ar': "🗝️ <b>انتهى!</b> النشرة الإخبارية المجدولة",
 }
 l_broadcast_start = {
-    'ru': "🗝️ <b>Старт</b> рассылки..\n#длительность {0}min",
+    'ru': "📧 <b>Старт</b> рассылки..\n#длительность {0}min",
     'en': "🗝️ <b>Start</b> mailing..\n#duration {0}min",
     'es': "🗝️ <b>Empezar a</b> enviar correos..\n#duración {0}min",
     'fr': "🗝️ <b>Lancer</b> l'envoi..\n#durée {0}min",
     'zh': "🗝️<b>开始</b>邮寄..\n#duration {0}min",
     'ar': "🗝️ <b>ابدأ</b> المراسلة ..\n# مدة {0} دقيقة",
 }
 l_broadcast_process = {
-    'ru': "🗝️ <b>Рассылка</b>..{0}%",
+    'ru': "📧 <b>Рассылка</b>..{0}%",
     'en': "🗝️ <b>Newsletter</b> ..{0}%",
     'es': "🗝️ <b>Boletín</b> ..{0}%",
     'fr': "🗝️ <b>Newsletter</b> ..{0}%",
     'zh': "🗝️<b>时事通讯</b>..{0}%",
     'ar': "🗝️ <b>النشرة الإخبارية</b> .. {0}٪",
 }
 l_broadcast_finish = {
-    'ru': "🏁 <b>Рассылка</b> завершена\n\n🗝️ Число пользователей, получивших сообщение: <u>{0}</u>",
+    'ru': "🏁 <b>Рассылка</b> завершена\n\n📧 Число пользователей, получивших сообщение: <u>{0}</u>",
     'en': "🏁 <b>Newsletter</b> ended\n\n🗝️ Number of users who received the message: <u>{0}</u>",
     'es': "🏁 <b>Boletín</b> finalizado\n\n🗝️ Número de usuarios que recibieron el mensaje: <u>{0}</u>",
     'fr': "🏁 <b>Newsletter</b> terminée\n\n🗝️ Nombre d&#x27;utilisateurs ayant reçu le message : <u>{0}</u>",
     'zh': "🏁<b>通讯</b>结束\n\n🗝️ 收到消息的用户数： <u>{0}</u>",
     'ar': "🏁 انتهت <b>الرسالة الإخبارية</b>\n\n🗝️ عدد المستخدمين الذين تلقوا الرسالة: <u>{0}</u>",
 }
 
@@ -1872,15 +1872,15 @@
     'en': "👩🏽‍💻 <b>Select</b> media note to delete",
     'es': "👩🏽‍💻 <b>Seleccione</b> nota multimedia para eliminar",
     'fr': "👩🏽‍💻 <b>Sélectionnez</b> la note multimédia à supprimer",
     'zh': "👩🏽‍💻<b>选择</b>要删除的媒体备注",
     'ar': "<b>حدد</b> ملاحظة وسائط لحذفها",
 }
 l_media_random = {
-    'ru': "🎲 Случайный выбор",
+    'ru': "🎲 <b>Случайный</b> выбор",
     'en': "👩🏽‍💻 <b>Select</b> media note to delete",
     'es': "👩🏽‍💻 <b>Seleccione</b> nota multimedia para eliminar",
     'fr': "👩🏽‍💻 <b>Sélectionnez</b> la note multimédia à supprimer",
     'zh': "👩🏽‍💻<b>选择</b>要删除的媒体备注",
     'ar': "<b>حدد</b> ملاحظة وسائط لحذفها",
 }
 l_media_none = {
@@ -2076,15 +2076,15 @@
     'en': "📍 No users ( @username ) found in this location",
     'es': "📍 No se encontraron usuarios ( @username ) en esta ubicación",
     'fr': "📍 Aucun utilisateur ( @username ) trouvé à cet emplacement",
     'zh': "📍 在此位置找不到用户 ( @username )",
     'ar': "📍 لم يتم العثور على مستخدمين ( @username ) في هذا الموقع",
 }
 l_geo_finish = {
-    'ru': "🔥 Готово! Найдено пользователей: <u>{0}</u>",
+    'ru': "🔥 <b>Готово!</b> Найдено пользователей: <u>{0}</u>",
     'en': "🔥 Done! Found users: <u>{0}</u>",
     'es': "🔥 Listo! Usuarios encontrados: <u>{0}</u>",
     'fr': "🔥 C'est fait ! Utilisateurs trouvés : <u>{0}</u>",
     'zh': "🔥 完成！找到的用户： <u>{0}</u>",
     'ar': "🔥 انتهى! المستخدمون الموجودون: <u>{0}</u>",
 }
 
@@ -2093,15 +2093,15 @@
     'en': "👩🏽‍💻 <b>Send</b> a link to a channel/group/user/bot",
     'es': "👩🏽‍💻 <b>Enviar</b> un enlace a un canal/grupo/usuario/bot",
     'fr': "👩🏽‍💻 <b>Envoyer</b> un lien vers un canal/groupe/utilisateur/bot",
     'zh': "👩🏽‍💻<b>发送</b>指向频道/组/用户/机器人的链接",
     'ar': "👩🏽‍💻 <b>أرسل</b> رابطًا لقناة / مجموعة / مستخدم / روبوت",
 }
 l_find_err_cmd = {
-    'ru': "👩🏽‍💻 <b>Ошибка</b> добавления (вставь корректную ссылку или повтори позже)",
+    'ru': "👩🏽‍💻 <b>Ошибка</b> (вставь корректную ссылку или повтори позже)",
     'en': "👩🏽‍💻 <b>Error</b> adding (insert correct link or try again later)",
     'es': "👩🏽‍💻 <b>Error</b> al agregar (insertar enlace correcto o intentarlo más tarde)",
     'fr': "👩🏽‍💻 <b>Erreur</b> lors de l'ajout (insérez le lien correct ou réessayez plus tard)",
     'zh': "👩🏽‍💻 添加<b>错误</b>（插入正确的链接或稍后重试）",
     'ar': "👩🏽‍💻 <b>خطأ</b> في الإضافة (أدخل الرابط الصحيح أو حاول مرة أخرى لاحقًا)",
 }
 l_find_ok_cmd = {
@@ -2575,39 +2575,39 @@
     'es': "✅ Bot {0}: agregado a la base de datos y actualizado",
     'fr': "✅ Bot {0} - ajouté à la base de données et mis à jour",
     'zh': "✅ Bot {0} - 添加到数据库并更新",
     'ar': "✅ بوت {0} - تمت إضافته إلى قاعدة البيانات وتحديثها",
 }
 
 l_find_chn_done = {
-    'ru': "🔥 Готово! По {0} собрано <u>{1}</u> каналов, сегментированных по <i>ключевым</i> словам\n\n<b>Охват</b>: <u>{2}</u> польз\n\nМожно связаться с администраторами каналов, чтобы заказать рекламу",
+    'ru': "🔥 <b>Готово!</b> По {0} собрано <u>{1}</u> каналов, сегментированных по <i>ключевым</i> словам\n\n<b>Охват</b>: <u>{2}</u> польз\n\nМожно связаться с администраторами каналов, чтобы заказать рекламу",
     'en': "🔥 Done! {0} collected <u>{1}</u> channels segmented by <i>keywords</i>\n\n<b>Reach</b> : <u>{2}</u> users\n\nYou can contact channel administrators to order advertising",
     'es': "🔥 Listo! {0} recopilaron <u>{1}</u> canales segmentados por <i>palabras clave</i>\n\n<b>Alcance</b> : <u>{2}</u> usuarios\n\nPuede ponerse en contacto con los administradores del canal para solicitar publicidad",
     'fr': "🔥 C'est fait ! {0} a collecté <u>{1}</u> chaînes segmentées par <i>mots-clés</i>\n\n<b>Atteinte</b> : <u>{2}</u> utilisateurs\n\nVous pouvez contacter les administrateurs de chaîne pour commander de la publicité",
     'zh': "🔥 完成！ {0} 收集了<u>{1} 个</u>按<i>关键字</i>细分的频道\n\n<b>覆盖</b>： <u>{2} 个</u>用户\n\n您可以联系频道管理员订购广告",
     'ar': "🔥 انتهى! القنوات {0} المجمعة <u>{1}</u> المقسمة حسب <i>الكلمات الرئيسية</i>\n\n<b>الوصول إلى</b> : <u>{2}</u> المستخدمين\n\nيمكنك الاتصال بمسؤولي القناة لطلب الإعلانات",
 }
 l_find_grp_done = {
-    'ru': "🔥 Готово! По {0} собрано <u>{1}</u> чатов, сегментированных по <i>ключевым</i> словам\n\n<b>Охват</b>: <u>{2}</u> польз\n\nМожно сделать <b>рассылку</b> по группам",
+    'ru': "🔥 <b>Готово!</b> По {0} собрано <u>{1}</u> чатов, сегментированных по <i>ключевым</i> словам\n\n<b>Охват</b>: <u>{2}</u> польз\n\nМожно сделать <b>рассылку</b> по группам",
     'en': "🔥 Done! {0} collected <u>{1}</u> chats, segmented by <i>keywords</i>\n\n<b>Reach</b> : <u>{2}</u> users\n\nCan be <b>sent</b> to groups",
     'es': "🔥 Listo! {0} <u>{1}</u> chats recopilados, segmentados por <i>palabras clave</i>\n\n<b>Alcance</b> : <u>{2}</u> usuarios\n\nSe puede <b>enviar</b> a grupos",
     'fr': "🔥 C'est fait ! {0} a collecté <u>{1}</u> chats, segmentés par <i>mots-clés</i>\n\n<b>Atteinte</b> : <u>{2}</u> utilisateurs\n\nPeut être <b>envoyé</b> à des groupes",
     'zh': "🔥 完成！ {0} 收集了<u>{1} 个</u>聊天，按<i>关键字细分</i>\n\n<b>覆盖</b>： <u>{2} 个</u>用户\n\n可以<b>发送</b>到组",
     'ar': "🔥 انتهى! {0} دردشات <u>{1}</u> مجمعة ، مقسمة حسب <i>الكلمات الرئيسية</i>\n\n<b>مدى الوصول</b> : <u>{2}</u> مستخدمين\n\nيمكن <b>إرسالها</b> إلى مجموعات",
 }
 l_find_usr_done = {
-    'ru': "🔥 Готово! По {0} собрано <u>{1}</u> пользователей, сегментированных по <i>ключевым</i> словам\n\nМожно сразу сделать <b>рассылку</b> или подписку-<b>инвайт</b> в чат по <i>полученным</i> лидам",
+    'ru': "🔥 <b>Готово!</b> По {0} собрано <u>{1}</u> пользователей, сегментированных по <i>ключевым</i> словам\n\nМожно сразу сделать <b>рассылку</b> или подписку-<b>инвайт</b> в чат по <i>полученным</i> лидам",
     'en': "🔥 Done! {0} collected <u>{1}</u> users, segmented by <i>keywords</i>\n\nYou can immediately make <b>a mailing list</b> or subscribe <b>- invite</b> to the chat according to <i>the received</i> leads",
     'es': "🔥 Listo! {0} recopiló <u>{1}</u> usuarios, segmentados por <i>palabras clave</i>\n\nPuede crear <b>una lista de correo</b> o suscribirse de inmediato <b>: invite</b> al chat de acuerdo con <i>los clientes potenciales recibidos</i>",
     'fr': "🔥 C'est fait ! {0} utilisateurs collectés <u>{1}</u> , segmentés par <i>mots-clés</i>\n\nVous pouvez immédiatement créer <b>une liste de diffusion</b> ou vous abonner <b>- inviter</b> au chat en fonction <i>des prospects reçus</i>",
     'zh': "🔥 完成！ {0} 收集了<u>{1} 个</u>用户，按<i>关键字</i>细分\n\n您可以立即制作<b>邮件列表</b>或订阅<b>-</b>根据<i>收到的</i>线索邀请聊天",
     'ar': "🔥 انتهى! {0} تم تجميع <u>{1}</u> مستخدمين ، مقسمين حسب <i>الكلمات الرئيسية</i>\n\nيمكنك على الفور إنشاء <b>قائمة بريدية</b> أو الاشتراك <b>- قم بدعوة</b> إلى الدردشة وفقًا للعملاء <i>المحتملين المستلمين</i>",
 }
 l_find_bot_done = {
-    'ru': "🔥 Готово! По {0} собрано <u>{1}</u> ботов, сегментированных по <i>ключевым</i> словам",
+    'ru': "🔥 <b>Готово!</b> По {0} собрано <u>{1}</u> ботов, сегментированных по <i>ключевым</i> словам",
     'en': "🔥 Done! {0} collected <u>{1}</u> bots segmented by <i>keywords</i>",
     'es': "🔥 Listo! {0} recopilaron <u>{1}</u> bots segmentados por <i>palabras clave</i>",
     'fr': "🔥 C'est fait ! {0} collecté <u>{1}</u> bots segmentés par <i>mots-clés</i>",
     'zh': "🔥 完成！ {0} 收集了<u>{1} 个</u><i>按关键字</i>细分的机器人",
     'ar': "🔥 انتهى! {0} جمعت <u>{1}</u> برامج التتبع مقسمة حسب <i>الكلمات الرئيسية</i>",
 }
 l_hashtag_categories = {
@@ -3008,15 +3008,15 @@
     'fr': "👮🏽 Il est nécessaire d'ajouter un canal pour <i>vérifier l'abonnement</i> par la commande :\n\n/channel LINK",
     'zh': "👮🏽 <i>訂閱檢查</i>需要通過命令添加頻道：\n\n/channel LINK",
     'ar': "👮🏽 من الضروري إضافة قناة لـ <i> فحص الاشتراك </i> بواسطة الأمر: \n\n/channel LINK",
 }
 
 # region commands
 l_update_text = {
-    'ru': "👩🏽‍💻 Данные о канале успешно обновлены:\n\n<b>{0}</b> [<code>{1}</code>]\n{2}\n<i>{3}</i>\n\n⚙️ <b>Команды</b> /cmd",
+    'ru': "👩🏽‍💻 <b>Данные</b> о канале успешно обновлены:\n\n<b>{0}</b> [<code>{1}</code>]\n{2}\n<i>{3}</i>\n\n⚙️ <b>Команды</b> /cmd",
     'en': "➕ Add channel",
     'es': "➕ Agregar grupo",
     'fr': "➕ Ajouter un channele",
     'zh': "➕ 添加組",
     'ar': "➕ إضافة مجموعة",
 }
 l_chn_commands_handler = {
@@ -3251,23 +3251,23 @@
     'en': "🎥 Send this command as reply to message",
     'es': "🎥 Enviar este comando como respuesta al mensaje",
     'fr': "🎥 Envoyez cette commande en réponse au message",
     'zh': "🎥 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_ban_users_start = {
-    'ru': "👩🏽‍💻 Начинаем очистку\nТекущее количество пользователей в базе: {0}",
+    'ru': "👩🏽‍💻 <b>Очистка</b> запущена\nТекущее количество пользователей в базе: <u>{0}</u>",
     'en': "🎥 Send this command as reply to message",
     'es': "🎥 Enviar este comando como respuesta al mensaje",
     'fr': "🎥 Envoyez cette commande en réponse au message",
     'zh': "🎥 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_ban_users_stop = {
-    'ru': "👩🏽‍💻 Очистка завершена\nТекущее количество пользователей в базе: {0} (-{1})",
+    'ru': "👩🏽‍💻 <b>Очистка</b> завершена\nТекущее количество пользователей в базе: <u>{0}</u> (-{1})",
     'en': "🎥 Send this command as reply to message",
     'es': "🎥 Enviar este comando como respuesta al mensaje",
     'fr': "🎥 Envoyez cette commande en réponse au message",
     'zh': "🎥 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_chn_ccheck_handler = {
@@ -3439,23 +3439,23 @@
     'en': "🗣 Push the ✅/☑️ to <b>On/Off</b> auto-transcribe (speach to text) for <i><b>income</b>/<b>outgoing</b> messages</i>",
     'es': "🗣 Presiona ✅/☑️ para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <i>Usuario se unió al grupo</i>",
     'fr': "🗣 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>L'utilisateur a rejoint le bote</i>",
     'zh': "🗣 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👩🏽‍💻 例如，<i>用戶加入群組</i>",
     'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👩🏽‍💻 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
 }
 l_cban_text = {
-    'ru': "🕵🏽 Жми на ✅/☑️ чтобы <b>Вкл/Выкл</b> бан <u>пользователей</u> бота: <i>с недавно зарегистрированными new-id/аккаунтов без @username/аккаунтов из <a href='https://cas.chat'>Anti-Spam Системы</a>/аккаунтов с 文-глиф, ب-араб/ <a href='https://www.zalgo.org'>zalgo-символами</a></i>\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/ban - блок/разблок пользователя\n/parse - вывести всех пользователей",
+    'ru': "🕵🏽 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> бан <u>пользователей</u> бота: <i>с недавно зарегистрированными new-id/аккаунтов без @username/аккаунтов из <a href='https://cas.chat'>Anti-Spam Системы</a>/аккаунтов с 文-глиф, ب-араб/ <a href='https://www.zalgo.org'>zalgo-символами</a></i>\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/ban - блок/разблок пользователя\n/parse - вывести всех пользователей",
     'en': "🕵🏽 Push the ✅/☑️ to <b>On/Off</b> <u>auto</u>-ban <i>bots with recently registered new-id/without @username/bots from <a href='https://cas.chat'>Anti-Spam System</a>/bots with 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👩🏽‍💻 For example, option <b>new-id</b> blocks bots with <i>fresh</i> <u>id</u> and with the same photo upload <u>date</u> <i>many avatars</i>",
     'es': "🕵🏽 Presiona ✅/☑️ para <b>Encender/Apagar</b> <u>Auto</u>-banear <i>cuentas con nueva identificación registrada recientemente/cuentas eliminadas/cuentas de <a href='https://cas.chat'>Anti-Spam System</a>/cuentas con 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👩🏽‍💻 Por ejemplo, la opción <b>deleted-ban</b> elimina dichas cuentas: <i>👻 Cuenta eliminada [estafa, falsa]</i>",
     'fr': "🕵🏽 Appuyez sur ✅/☑️ pour <b>On/Off</b> <u>auto</u>-bannir <i>les comptes avec un nouvel identifiant/des comptes supprimés/des comptes récemment enregistrés depuis <a href='https://cas.chat'>Anti-Spam System</a>/comptes avec 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👩🏽‍💻 Par exemple, l'option <b>deleted-ban</b> supprime ces comptes : <i>👻 Compte supprimé [arnaque, faux]</i>",
     'zh': "🕵🏽 按下 ✅/☑️，以 <b>On/Off</b> <u>auto</u>-禁止 <i>具有最近從 註冊的 new-id/deleted-bots/bots <a href='https://cas.chat'>Anti-Spam System</a>/bots with text-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👩🏽‍💻 例如，選項 <b>deleted-ban</b> 刪除此類帳戶：<i>👻 Deleted bot [scam,fake]</i>",
     'ar': "🕵🏽 اضغط على ✅ / ☑️ ، إلى <b> تشغيل / إيقاف </b> <u> تلقائي </u> -حظر <i> الحسابات ذات المعرف الجديد / الحسابات / الحسابات المحذوفة حديثًا من <a href='https://cas.chat'> نظام مكافحة البريد العشوائي </a> / حسابات مع 文 -glif، ب- arab، <a href='https://www.zalgo.org'> zalgo-icons </a> </i> \n\n👩🏽‍💻 على سبيل المثال ، الخيار <b> حذف-حظر </b> يحذف مثل هذه الحسابات: <i> 👻 الحساب المحذوف [احتيال ، وهمي] </i>",
 }
 l_cban_done = {
-    'ru': "🕵🏽 Готово! /ban-список нежелательных пользователей @{0}-бота\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/ban - блок/разблок пользователя\n/parse - вывести всех пользователей\n\n👩🏽‍💻 Текущее число пользователей /ban-списка: <u>{1}</u>",
+    'ru': "🕵🏽 <b>Готово!</b> /ban-список нежелательных пользователей @{0}-бота\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/ban - блок/разблок пользователя\n/parse - вывести всех пользователей\n\n👩🏽‍💻 Текущее число пользователей /ban-списка: <u>{1}</u>",
     'en': "👥 Ready! Gathered members: <u>{0}</u>. You can immediately make an <b>sending</b> or <b>inviting</b> to channel by received members{1}",
     'es': "👥 Listo! Miembros reunidos: <u>{0}</u>. Inmediatamente puede hacer un <b>envío</b> o <b>invitación</b> al grupo por miembros recibidos{1}",
     'fr': "👥 Prêt ! Membres réunis : <u>{0}</u>. Vous pouvez immédiatement faire un <b>envoi</b> ou <b>inviter</b> pour channeler par membres reçus{1}",
     'zh': "👥 準備好了！ 聚集成員：<u>{0}</u>。 您可以立即<b>發送</b>或<b>邀請</b>按收到的成員分組{1}",
     'ar': "🔥 جاهز! الأعضاء الذين تم تجميعهم: <u>{0}</u>. يمكنك على الفور إجراء <b> إرسال </b> أو <b> دعوة </b> للانضمام إلى المجموعة بواسطة الأعضاء المستلمين {1}",
 }
 l_cban_correct = {
@@ -3615,15 +3615,15 @@
     'en': "👍🏽 Ready! Current primary delay for <u>new</u> users (before writing their <u>1</u>st message) is <u>{0}</u> min",
     'es': "👍🏽 Listo! El retraso principal actual para los <u>nuevos</u> usuarios (antes de escribir su <u>1</u>er mensaje) es <u>{0}</u> min",
     'fr': "👍🏽 Prêt! Le délai principal actuel pour les <u>nouveaux</u> utilisateurs (avant d'écrire leur <u>1</u>er message) est de <u>{0}</u> min",
     'zh': "👍🏽 準備好了！<u>新</u>用戶的當前主要延遲（在寫他們的<u>1</u>st消息之前）是<u>{0}</u>分鐘",
     'ar': "👥 جاهز! التأخير الأساسي الحالي لمستخدمي <u> الجدد </u> (قبل كتابة رسالتهم <u> 1 </u> st) هو <u>{0}</u> min",
 }
 l_creact_on = {
-    'ru': "👍🏽 Готово! Текущее количество <b>авто-реакций</b> на пост канала установлено в значение <u>{0}</u>",
+    'ru': "👍🏽 <b>Готово!</b> Текущее количество <b>авто-реакций</b> на пост канала установлено в значение <u>{0}</u>",
     'en': "👍🏽 Ready! Current primary delay for <u>new</u> users (before writing their <u>1</u>st message) is <u>{0}</u> min",
     'es': "👍🏽 Listo! El retraso principal actual para los <u>nuevos</u> usuarios (antes de escribir su <u>1</u>er mensaje) es <u>{0}</u> min",
     'fr': "👍🏽 Prêt! Le délai principal actuel pour les <u>nouveaux</u> utilisateurs (avant d'écrire leur <u>1</u>er message) est de <u>{0}</u> min",
     'zh': "👍🏽 準備好了！<u>新</u>用戶的當前主要延遲（在寫他們的<u>1</u>st消息之前）是<u>{0}</u>分鐘",
     'ar': "👥 جاهز! التأخير الأساسي الحالي لمستخدمي <u> الجدد </u> (قبل كتابة رسالتهم <u> 1 </u> st) هو <u>{0}</u> min",
 }
 l_creact_off = {
@@ -3659,15 +3659,15 @@
     'en': "👁️‍🗨️ Ready! Current primary delay for <u>new</u> users (before writing their <u>1</u>st message) is <u>{0}</u> min",
     'es': "👁️‍🗨️ Listo! El retraso principal actual para los <u>nuevos</u> usuarios (antes de escribir su <u>1</u>er mensaje) es <u>{0}</u> min",
     'fr': "👁️‍🗨️ Prêt! Le délai principal actuel pour les <u>nouveaux</u> utilisateurs (avant d'écrire leur <u>1</u>er message) est de <u>{0}</u> min",
     'zh': "👁️‍🗨️ 準備好了！<u>新</u>用戶的當前主要延遲（在寫他們的<u>1</u>st消息之前）是<u>{0}</u>分鐘",
     'ar': "👥 جاهز! التأخير الأساسي الحالي لمستخدمي <u> الجدد </u> (قبل كتابة رسالتهم <u> 1 </u> st) هو <u>{0}</u> min",
 }
 l_cview_on = {
-    'ru': "👁️‍🗨️ Готово! Текущее количество <b>авто-просмотров</b> на последний пост канала установлено в значение <u>{0}</u>",
+    'ru': "👁️‍🗨️ <b>Готово!</b> Текущее количество <b>авто-просмотров</b> на последний пост канала установлено в значение <u>{0}</u>",
     'en': "👁️‍🗨️ Ready! Current primary delay for <u>new</u> users (before writing their <u>1</u>st message) is <u>{0}</u> min",
     'es': "👁️‍🗨️ Listo! El retraso principal actual para los <u>nuevos</u> usuarios (antes de escribir su <u>1</u>er mensaje) es <u>{0}</u> min",
     'fr': "👁️‍🗨️ Prêt! Le délai principal actuel pour les <u>nouveaux</u> utilisateurs (avant d'écrire leur <u>1</u>er message) est de <u>{0}</u> min",
     'zh': "👁️‍🗨️ 準備好了！<u>新</u>用戶的當前主要延遲（在寫他們的<u>1</u>st消息之前）是<u>{0}</u>分鐘",
     'ar': "👥 جاهز! التأخير الأساسي الحالي لمستخدمي <u> الجدد </u> (قبل كتابة رسالتهم <u> 1 </u> st) هو <u>{0}</u> min",
 }
 l_cview_off = {
@@ -3711,15 +3711,15 @@
     'en': "🪄 There are no greetings you need to ⚙️Configure",
     'es': "🪄 No hay saludos que necesites ⚙️Configurar",
     'fr': "🪄 Vous n'avez pas besoin de salutations ⚙️Configurer",
     'zh': "🪄 無需問候⚙️配置",
     'ar': "🔔لا توجد تحيات تحتاج إلى تكوين",
 }
 l_cdecor_footer_done = {
-    'ru': "🪄 Готово! <b>Футер</b> из <u>{0}</u>-символов будет использоваться как окончание поста в канале\n\nОпцию можно включить, нажав <b>[✅☑Вкл футер]</b>",
+    'ru': "🪄 <b>Готово!</b> <b>Футер</b> из <u>{0}</u>-символов будет использоваться как окончание поста в канале\n\nОпцию можно включить, нажав <b>[✅☑Вкл футер]</b>",
     'en': "🪄 There are no greetings you need to ⚙️Configure",
     'es': "🪄 No hay saludos que necesites ⚙️Configurar",
     'fr': "🪄 Vous n'avez pas besoin de salutations ⚙️Configurer",
     'zh': "🪄 無需問候⚙️配置",
     'ar': "🔔لا توجد تحيات تحتاج إلى تكوين",
 }
 l_cdecor_page_on = {
@@ -3779,15 +3779,15 @@
     'en': "👥 Push the ✅/☑️, to <b>On/Off</b> auto-inviting users to your channel\n\n👉🏼 Inviting <u>{0}</u> users per day from channel {1}",
     'es': "👥 Presiona ✅/☑️ para <b>activar/desactivar</b> la invitación automática de usuarios a tu grupo\n\n👉🏼 Invitar a <u>{0}</u> usuarios por día del grupo {1}",
     'fr': "👥 Appuyez sur ✅/☑️, pour <b>Activer/Désactiver</b> l'invitation automatique d'utilisateurs dans votre channele\n\n👉🏼 Inviter <u>{0}</u> utilisateurs par jour à partir du channele {1}",
     'zh': "👥 按下 ✅/☑️, 以<b>開/關</b>自動邀請用戶加入您的群組\n\n👉🏼 每天從群組 {1} 中邀請 <u>{0}</u> 個用戶",
     'ar': "🚶 ادفع ✅ / ☑️ إلى <b> تشغيل / إيقاف </b> لدعوة المستخدمين تلقائيًا إلى مجموعتك \n\n👉🏼 دعوة <u>{0}</u> مستخدمين يوميًا من المجموعة {1}",
 }
 l_cmember_on = {
-    'ru': "👁️‍🗨️ Готово! Текущее количество <b>авто-просмотров</b> на последний пост канала установлено в значение <u>{0}</u>",
+    'ru': "👁️‍🗨️ <b>Готово!</b> Текущее количество <b>авто-просмотров</b> на последний пост канала установлено в значение <u>{0}</u>",
     'en': "👁️‍🗨️ Ready! Current primary delay for <u>new</u> users (before writing their <u>1</u>st message) is <u>{0}</u> min",
     'es': "👁️‍🗨️ Listo! El retraso principal actual para los <u>nuevos</u> usuarios (antes de escribir su <u>1</u>er mensaje) es <u>{0}</u> min",
     'fr': "👁️‍🗨️ Prêt! Le délai principal actuel pour les <u>nouveaux</u> utilisateurs (avant d'écrire leur <u>1</u>er message) est de <u>{0}</u> min",
     'zh': "👁️‍🗨️ 準備好了！<u>新</u>用戶的當前主要延遲（在寫他們的<u>1</u>st消息之前）是<u>{0}</u>分鐘",
     'ar': "👥 جاهز! التأخير الأساسي الحالي لمستخدمي <u> الجدد </u> (قبل كتابة رسالتهم <u> 1 </u> st) هو <u>{0}</u> min",
 }
 l_cmember_off = {
@@ -3795,15 +3795,15 @@
     'en': "👁️‍🗨️ Ready! Current primary delay for <u>new</u> users (before writing their <u>1</u>st message) is <u>{0}</u> min",
     'es': "👁️‍🗨️ Listo! El retraso principal actual para los <u>nuevos</u> usuarios (antes de escribir su <u>1</u>er mensaje) es <u>{0}</u> min",
     'fr': "👁️‍🗨️ Prêt! Le délai principal actuel pour les <u>nouveaux</u> utilisateurs (avant d'écrire leur <u>1</u>er message) est de <u>{0}</u> min",
     'zh': "👁️‍🗨️ 準備好了！<u>新</u>用戶的當前主要延遲（在寫他們的<u>1</u>st消息之前）是<u>{0}</u>分鐘",
     'ar': "👥 جاهز! التأخير الأساسي الحالي لمستخدمي <u> الجدد </u> (قبل كتابة رسالتهم <u> 1 </u> st) هو <u>{0}</u> min",
 }
 l_cmember_parse = {
-    'ru': "👥 Готово! Собрано реальных участников: <u>{0}</u>\n\n👩🏽‍💻 Старые подписчики будут постепенно пополнять базу, пока у @{1}-бота есть права [✅ Назначение администраторов]\n\n{2}",
+    'ru': "👥 <b>Готово!</b> Собрано реальных участников: <u>{0}</u>\n\n👩🏽‍💻 Старые подписчики будут постепенно пополнять базу, пока у @{1}-бота есть права [✅ Назначение администраторов]\n\n{2}",
     'en': "👥 Ready! Gathered members: <u>{0}</u>. You can immediately make an <b>sending</b> or <b>inviting</b> to channel by received members{1}",
     'es': "👥 Listo! Miembros reunidos: <u>{0}</u>. Inmediatamente puede hacer un <b>envío</b> o <b>invitación</b> al grupo por miembros recibidos{1}",
     'fr': "👥 Prêt ! Membres réunis : <u>{0}</u>. Vous pouvez immédiatement faire un <b>envoi</b> ou <b>inviter</b> pour channeler par membres reçus{1}",
     'zh': "👥 準備好了！ 聚集成員：<u>{0}</u>。 您可以立即<b>發送</b>或<b>邀請</b>按收到的成員分組{1}",
     'ar': "🔥 جاهز! الأعضاء الذين تم تجميعهم: <u>{0}</u>. يمكنك على الفور إجراء <b> إرسال </b> أو <b> دعوة </b> للانضمام إلى المجموعة بواسطة الأعضاء المستلمين {1}",
 }
 l_parse_rights = {
@@ -3840,15 +3840,15 @@
     'en': "🌱 {0}, welcome to <i>the landing bot</i> of the Ferey project:\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
     'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> del proyecto Ferey:\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ también puedes encargar el desarrollo de un chat bot en nuestro estudio Ferey",
     'fr': "🌱 {0}, bienvenue sur <i>le landing bot</i> du projet Ferey :\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
     'zh': "🌱 {0}，欢迎来到 Ferey 项目的<i>落地机器人</i>：\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️您也可以在我们的Ferey工作室订购聊天机器人的开发",
     'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> الخاص بمشروع Ferey:\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey",
 }
 l_add_group_text = {
-    'ru': "👇🏽 Жми на ‹➕ Добавить группу›, чтобы добавить в свою группу (с настройками по ум) бота: @{0}\n\n👮🏽‍♀️ Или добавь бота как <b>Administrator</b> через настройки своей группы: ‹👤Add Admin›\n\n👮🏽‍♀️ Если не добавляется группа, то измени <b>Должность</b> (см. скрин)",
+    'ru': "👇🏽 <b>Жми</b> на ‹➕ Добавить группу›, чтобы добавить в свою группу (с настройками по ум) бота: @{0}\n\n👮🏽‍♀️ Или добавь бота как <b>Administrator</b> через настройки своей группы: ‹👤Add Admin›\n\n👮🏽‍♀️ Если не добавляется группа, то измени <b>Должность</b> (см. скрин)",
     'en': "👇🏽 Push the ‹Group› to add into your group (with default settings): @{0}\n\n👮🏽‍♀️ Or add bot as <b>Admin</b> via Settings of your group: ‹👤Add Admin›\n\n👮🏽‍♀️ If you can't add group, try to change <b>Custom Title</b> (look screenshot)",
     'es': "👇🏽 Presione ‹➕ Agregar grupo› para agregar a su grupo (con la configuración predeterminada): @{0}\n\n👮🏽‍♀️ O agregue bot como <b>Administrador</b> a través de la Configuración de su grupo: ‹👤Agregar administrador›\n\n👮🏽‍♀️ Si no puede agregar un grupo, intente cambiar <b>Título personalizado</b> (ver captura de pantalla)",
     'fr': "👇🏽 Appuyez sur ‹➕ Ajouter un groupe› pour ajouter à votre groupe (avec les paramètres par défaut): @{0}\n\n👮🏽‍♀️ Ou ajoutez le bot en tant qu'<b>administrateur</b> via les paramètres de votre groupe : ‹👤Ajouter un administrateur›\n\n👮🏽‍♀️ Si vous ne pouvez pas ajouter de groupe, essayez de modifier le <b>Titre personnalisé</b> (regardez la capture d'écran)",
     'zh': "👇🏽 按下‹➕添加群組›以添加到您的群組（使用默認設置）: @{0}\n\n👮🏽‍♀️ 或通過您組的設置將機器人添加為 <b>Admin</b>：‹👤添加管理員›\n\n👮🏽‍♀️ 如果無法添加組，請嘗試更改 <b>自定義標題</b>（看截圖）",
     'ar': "👇🏽 اضغط على ‹➕ إضافة مجموعة› لإضافتها إلى مجموعتك (بالإعدادات الافتراضية): @{0}\n\n👮🏽‍♀️ أو أضف البوت كـ <b> مسؤول </b> عبر إعدادات مجموعتك: ‹👤 إضافة مسؤول›\n\n👮🏽‍♀️ إذا لم تتمكن من إضافة مجموعة ، فحاول تغيير <b> عنوان مخصص </b> (انظر في لقطة الشاشة)",
 }
 l_add_group_button = {
@@ -4331,15 +4331,15 @@
     'en': "⚠️ Use /transfer-command in reply user-message to transfer him ownership",
     'es': "⚠️ Use /transfer-command en el mensaje de usuario de respuesta para transferirle la propiedad",
     'fr': "⚠️ Utilisez /transfer-command dans le message utilisateur de réponse pour lui transférer la propriété",
     'zh': "⚠️ 使用 /transfer-command 回复 user-message 轉移他的所有權",
     'ar': "استخدم الأمر transfer-command/ في الرد على رسالة المستخدم لنقل ملكيته",
 }
 l_button_handler = {
-    'ru': "👮🏽 Готово! Текущее <b>имя кнопки</b> на <i>входном контроле</i> установлено: {0}",
+    'ru': "👮🏽 <b>Готово!</b> Текущее <b>имя кнопки</b> на <i>входном контроле</i> установлено: {0}",
     'en': "👮🏽 Ready! Current <b>button name</b> in <i>Enter control</i> is: {0}",
     'es': "👮🏽 Lista! El <b>nombre del botón</b> actual en <i>Control de entrada</i> es: {0}",
     'fr': "👮🏽 Prêt! Le <b>nom du bouton</b> actuel dans <i>Saisir le contrôle</i> est : {0}",
     'zh': "👮🏽 準備好! <i>輸入控件</i>中的當前<b>按鈕名稱</b>是：{0}",
     'ar': "👮🏽 جاهز! <b> اسم الزر </b> الحالي في <i> إدخال التحكم </i> هو: {0}",
 }
 l_button_correct = {
@@ -4355,15 +4355,15 @@
     'en': "⚙️ Add @{0} to channel for subscribe checking. Send me correct link to channel:",
     'es': "⚙️ Agregue @{0} al canal para verificar la suscripción. Envíame el enlace correcto al canal:",
     'fr': "⚙️ Ajoutez @{0} à la chaîne pour vérifier l'abonnement. Envoyez-moi le lien correct vers la chaîne :",
     'zh': "⚙️ 將@{0} 添加到頻道以進行訂閱檢查。 向我發送正確的頻道鏈接：",
     'ar': "⚙️ إضافة @{0} للقناة للتحقق من الاشتراك. أرسل لي الرابط الصحيح للقناة:",
 }
 l_channel_done = {
-    'ru': "👮🏽 Готово! Проверка подписки на {0} настроена\n\nОпцию можно включить в настройках, нажав [✅☑Вкл подписку]",
+    'ru': "👮🏽 <b>Готово!</b> Проверка подписки на {0} настроена\n\nОпцию можно включить в настройках, нажав [✅☑Вкл подписку]",
     'en': "👮🏽 Ready! Subscribe checking to {0}-channel is configured\n\nEnable this option in the Settings by pushing [✅☑Enable subscription]",
     'es': "👮🏽 Listo! La verificación de suscripción a {0}-canal está configurada\n\nActive esta opción en Configuración presionando [✅☑Habilitar suscripción]",
     'fr': "👮🏽 Prêt! La vérification de l'abonnement à la chaîne {0} est configurée\n\nActivez cette option dans les paramètres par push [✅☑Activer l'abonnement]",
     'zh': "👮🏽 準備好了！ 已配置對 {0} 頻道的訂閱檢查\n\n通過推送在“設置”中打開此選項 [✅☑啟用訂閱]",
     'ar': "👮🏽 جاهز! التحقق من الاشتراك في {0} - تم تكوين القناة \n\n قم بتشغيل هذا الخيار في الإعدادات عن طريق الدفع [✅☑ تمكين الاشتراك]",
 }
 l_channel_correct = {
@@ -4387,15 +4387,15 @@
     'en': "📇 Parsing (by @username) is failed",
     'es': "📇 El análisis (por @username) falló",
     'fr': "📇 L'analyse (par @username) a échoué",
     'zh': "📇 解析（@username）失敗",
     'ar': "📇 فشل التحليل (حسب اسم المستخدم)",
 }
 l_parse_done = {
-    'ru': "🔥 Готово! Собрано реальных участников: <u>{0}</u>. Можно сразу сделать <b>рассылку</b> или подписку-<b>инвайт</b> в чат по <i>полученным</i> лидам{1}",
+    'ru': "🔥 <b>Готово!</b> Собрано реальных участников: <u>{0}</u>. Можно сразу сделать <b>рассылку</b> или подписку-<b>инвайт</b> в чат по <i>полученным</i> лидам{1}",
     'en': "🔥 Ready! Gathered members: <u>{0}</u>. You can immediately make an <b>sending</b> or <b>inviting</b> to group by received members{1}",
     'es': "🔥 Listo! Miembros reunidos: <u>{0}</u>. Inmediatamente puede hacer un <b>envío</b> o <b>invitación</b> al grupo por miembros recibidos{1}",
     'fr': "🔥 Prêt ! Membres réunis : <u>{0}</u>. Vous pouvez immédiatement faire un <b>envoi</b> ou <b>inviter</b> pour grouper par membres reçus{1}",
     'zh': "🔥 準備好了！ 聚集成員：<u>{0}</u>。 您可以立即<b>發送</b>或<b>邀請</b>按收到的成員分組{1}",
     'ar': "🔥 جاهز! الأعضاء الذين تم تجميعهم: <u>{0}</u>. يمكنك على الفور إجراء <b> إرسال </b> أو <b> دعوة </b> للانضمام إلى المجموعة بواسطة الأعضاء المستلمين {1}",
 }
 l_parse_btnsend = {
@@ -4660,15 +4660,15 @@
     'en': "🎥 Send this command as reply to message",
     'es': "🎥 Enviar este comando como respuesta al mensaje",
     'fr': "🎥 Envoyez cette commande en réponse au message",
     'zh': "🎥 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_delay_on = {
-    'ru': "👥 Готово! Текущая первичная задержка для <u>новых</u> пользователей (перед написанием их <u>1</u>го сообщ) установлена в значение <u>{0}</u> min",
+    'ru': "👥 <b>Готово!</b> Текущая первичная задержка для <u>новых</u> пользователей (перед написанием их <u>1</u>го сообщ) установлена в значение <u>{0}</u> min",
     'en': "👥 Ready! Current primary delay for <u>new</u> users (before writing their <u>1</u>st message) is <u>{0}</u> min",
     'es': "👥 Listo! El retraso principal actual para los <u>nuevos</u> usuarios (antes de escribir su <u>1</u>er mensaje) es <u>{0}</u> min",
     'fr': "👥 Prêt! Le délai principal actuel pour les <u>nouveaux</u> utilisateurs (avant d'écrire leur <u>1</u>er message) est de <u>{0}</u> min",
     'zh': "👥 準備好了！<u>新</u>用戶的當前主要延遲（在寫他們的<u>1</u>st消息之前）是<u>{0}</u>分鐘",
     'ar': "👥 جاهز! التأخير الأساسي الحالي لمستخدمي <u> الجدد </u> (قبل كتابة رسالتهم <u> 1 </u> st) هو <u>{0}</u> min",
 }
 l_delay_off = {
@@ -4704,15 +4704,15 @@
     'ar': "👉🏼 لم تتم تهيئة <b> قواعد المجموعة </b> لـ <b>{0}</b>. يجب عليك <u> الرد على الرسالة </u> بالقواعد من خلال / rules- <b> أمر </b>",
 }
 # endregion
 
 
 # region ccheck
 l_ccheck_handler = {
-    'ru': "👮🏽 Жми на ✅/🔘, чтобы <b>переключить</b> тип <i>проверки</i> пользователя при <u>вступлении</u> в группу\n\n👉🏼 Для установки имени <b>нажимаемой кнопки</b>, выполни команду: <code>/button {0}</code>\n\n👉🏼 Для <b>проверки подписки</b> на канал <i>добавь</i> @{1}-бота в канал и выполни команду: <code>/channel {2}</code>\n\n👉🏼 Для <i>защиты от атаки</i> на группу включи режим <b>антирейд</b> (блокировка <u>всех</u> вступающих)",
+    'ru': "👮🏽 <b>Жми</b> на ✅/🔘, чтобы <b>переключить</b> тип <i>проверки</i> пользователя при <u>вступлении</u> в группу\n\n👉🏼 Для установки имени <b>нажимаемой кнопки</b>, выполни команду: <code>/button {0}</code>\n\n👉🏼 Для <b>проверки подписки</b> на канал <i>добавь</i> @{1}-бота в канал и выполни команду: <code>/channel {2}</code>\n\n👉🏼 Для <i>защиты от атаки</i> на группу включи режим <b>антирейд</b> (блокировка <u>всех</u> вступающих)",
     'en': "👮🏽 Push the ✅/🔘 to <b>switch</b> <i>Enter control</i> of user <u>joining</u> into group\n\n👉🏼 To set name of <b>pushing button</b> execute command: <code>/button {0}</code>\n\n👉🏼 To check <b>channel-subscription</b> <i>add</i> @{1} to channel and execute command: <code>/channel {2}</code>\n\n👉🏼 To <i>defend</i> from group-attack switch <b>anti-raid</b>-mode (ban <u>everyone</u> who joining)",
     'es': "👮🏽 Presiona ✅/🔘 para <b>cambiar</b> <i>Enter control</i> del usuario <u>uniéndose</u> al grupo\n\n👉🏼 Para establecer el nombre de <b> presionando el botón</b> ejecute el comando: <code>/button {0}</code>\n\n👉🏼 Para verificar <b>channel-subscription</b> <i>add</i> @{1} para canalizar y ejecutar el comando: <code>/channel {2}</code>\n\n👉🏼 Para <i>defender</i> del ataque grupal, active el modo <b>anti-raid</b> (prohibir a <u>todos</u> que se unan)",
     'fr': "👮🏽 Appuyez sur ✅/🔘 pour <b>commuter</b> <i>Entrez le contrôle</i> de l'utilisateur <u>rejoignant</u> le groupe\n\n👉🏼 Pour définir le nom de <b> en appuyant sur le bouton</b> exécutez la commande : <code>/button {0}</code>\n\n👉🏼 Pour vérifier <b>channel-subscription</b> <i>add</i> @{1} pour canaliser et exécuter la commande : <code>/channel {2}</code>\n\n👉🏼 Pour <i>se défendre</i> contre une attaque de groupe, activez le mode <b>anti-raid</b> (bannir <u>tous ceux</u> qui se joignent)",
     'zh': "👮🏽 按下 ✅/🔘 來<b>切換</b> <i>進入控制</i> 用戶<u>加入</u> 入組\n\n👉🏼 設置<b>的名字 按下按鈕</b> 執行命令：<code>/button {0}</code>\n\n👉🏼 檢查<b>頻道訂閱</b> <i>add</i> @{1} 引導並執行命令：<code>/channel {2}</code>\n\n👉🏼 以 <i>defend</i> 免受群攻開啟 <b>anti-raid</b>-mode （禁止加入的<u>每個人</u>）",
     'ar': "👮🏽 ادفع ✅ / 🔘 إلى <b> التبديل </b> <i> أدخل التحكم </i> للمستخدم <u> المنضم </u> إلى مجموعة \n\n👉🏼 لتعيين اسم <b> ضغط الزر </b> نفذ الأمر: <code> / button {0}</code>\n\n👉🏼 للتحقق من <b> اشتراك القناة </b> <i> إضافة </i> @{1} لتوجيه وتنفيذ الأمر: <code> / channel {2}</code>\n\n👉🏼 <i> للدفاع </i> من هجوم المجموعة ، شغّل وضع <b> anti-raid </b> (حظر <u> كل شخص </u> من ينضم)",
 }
 l_ccheck_add = {
@@ -4812,15 +4812,15 @@
     'en': "Your greeting",
     'es': "Tu saludo",
     'fr': "Votre message d'accueil",
     'zh': "你的問候",
     'ar': "تحياتك",
 }
 l_chello_text = {
-    'ru': "👋🏽 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> приветствие, а также его ⚙️Настроить\n\n👉🏼 Например, <code>{0}</code>{1}",
+    'ru': "👋🏽 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> приветствие, а также его ⚙️Настроить\n\n👉🏼 Например, <code>{0}</code>{1}",
     'en': "👋🏽 Push the ✅/☑️, to <b>On/Off</b> greeting, and to ⚙️Configure\n\n👉🏼 For example, <code>{0}</code>{1}",
     'es': "👋🏽 Presione ✅/☑️, para <b>Activar/Desactivar</b> el saludo y para ⚙️Configurar\n\n👉🏼 Por ejemplo, <code>{0}</code>{1}",
     'fr': "👋🏽 Appuyez sur ✅/☑️, sur <b>Activer/Désactiver</b> le message d'accueil et sur ⚙️Configurer\n\n👉🏼 Par exemple, <code>{0}</code>{1}",
     'zh': "👋🏽 按下 ✅/☑️、<b>On/Off</b> 問候語和 ⚙️Configure\n\n👉🏼 例如，<code>{0}</code>{1}",
     'ar': "👋🏽 اضغط على ✅ / ☑️ ، من أجل <b> تشغيل / إيقاف </b> الترحيب ، و تكوين \n\n👉🏼 على سبيل المثال ، <code>{0}</code>{1}",
 }
 l_btn_on = {
@@ -4880,15 +4880,15 @@
     'en': "🚶🏽 Push the ✅/☑️, to <b>On/Off</b> auto-inviting users to your group\n\n👉🏼 Inviting <u>{0}</u> users per day from group {1}",
     'es': "🚶🏽 Presiona ✅/☑️ para <b>activar/desactivar</b> la invitación automática de usuarios a tu grupo\n\n👉🏼 Invitar a <u>{0}</u> usuarios por día del grupo {1}",
     'fr': "🚶🏽 Appuyez sur ✅/☑️, pour <b>Activer/Désactiver</b> l'invitation automatique d'utilisateurs dans votre groupe\n\n👉🏼 Inviter <u>{0}</u> utilisateurs par jour à partir du groupe {1}",
     'zh': "🚶🏽 按下 ✅/☑️, 以<b>開/關</b>自動邀請用戶加入您的群組\n\n👉🏼 每天從群組 {1} 中邀請 <u>{0}</u> 個用戶",
     'ar': "🚶🏽 ادفع ✅ / ☑️ إلى <b> تشغيل / إيقاف </b> لدعوة المستخدمين تلقائيًا إلى مجموعتك \n\n👉🏼 دعوة <u>{0}</u> مستخدمين يوميًا من المجموعة {1}",
 }
 l_cinvite_text = {
-    'ru': "🚶🏽 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-инвайт пользователей в <b>{0}</b>-группу\n\n👩🏽‍💻 <b>Текущие</b> настройки авто-рассылки: {1}",
+    'ru': "🚶🏽 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-инвайт пользователей в <b>{0}</b>-группу\n\n👩🏽‍💻 <b>Текущие</b> настройки авто-рассылки: {1}",
     'en': "🚶🏽 Push the ✅/☑️, to <b>On/Off</b> auto-inviting users to your group\n\n👉🏼 Inviting <u>{0}</u> users per day from group {1}",
     'es': "🚶🏽 Presiona ✅/☑️ para <b>activar/desactivar</b> la invitación automática de usuarios a tu grupo\n\n👉🏼 Invitar a <u>{0}</u> usuarios por día del grupo {1}",
     'fr': "🚶🏽 Appuyez sur ✅/☑️, pour <b>Activer/Désactiver</b> l'invitation automatique d'utilisateurs dans votre groupe\n\n👉🏼 Inviter <u>{0}</u> utilisateurs par jour à partir du groupe {1}",
     'zh': "🚶🏽 按下 ✅/☑️, 以<b>開/關</b>自動邀請用戶加入您的群組\n\n👉🏼 每天從群組 {1} 中邀請 <u>{0}</u> 個用戶",
     'ar': "🚶🏽 ادفع ✅ / ☑️ إلى <b> تشغيل / إيقاف </b> لدعوة المستخدمين تلقائيًا إلى مجموعتك \n\n👉🏼 دعوة <u>{0}</u> مستخدمين يوميًا من المجموعة {1}",
 }
 
@@ -4913,15 +4913,15 @@
     'en': "Send <b>link</b> to userbot as source for new members\n\n👉🏼 For example, <code>https://t.me/likeconcentrat</code> - push the link to copy",
     'es': "Envía <b>enlace</b> al grupo como fuente para nuevos miembros\n\n👉🏼 Por ejemplo, <code>https://t.me/likeconcentrat</code> - presiona el enlace para copiar",
     'fr': "Envoyez <b>lien</b> au userbote comme source pour les nouveaux membres\n\n👉🏼 Par exemple, <code>https://t.me/likeconcentrat</code> - appuyez sur le lien pour le copier",
     'zh': "將 <b>link</b> 發送到群組作為新成員的來源\n\n👉🏼 例如，<code>https://t.me/likeconcentrat</code> - 推送鏈接以進行複制",
     'ar': "📨️ أرسل <b> ارتباط </b> للمجموعة كمصدر للأعضاء الجدد \n\n👉🏼 على سبيل المثال ، <code> https://t.me/likeconcentrat </code> - ادفع الرابط للنسخ",
 }
 l_cinvitechange_handler = {
-    'ru': "🚶🏽 Пришли мне <b>ссылку</b> на группу, откуда будем брать подписчиков\n\n👉🏼 Например, <code>https://t.me/likeconcentrat</code> - жми на ссылку, чтобы скопировать",
+    'ru': "🚶🏽 Пришли мне <b>ссылку</b> на группу, откуда будем брать подписчиков\n\n👉🏼 Например, <code>https://t.me/likeconcentrat</code> - <b>Жми</b> на ссылку, чтобы скопировать",
     'en': "🚶🏽 Send <b>link</b> to group as source for new members\n\n👉🏼 For example, <code>https://t.me/likeconcentrat</code> - push the link to copy",
     'es': "🚶🏽 Envía <b>enlace</b> al grupo como fuente para nuevos miembros\n\n👉🏼 Por ejemplo, <code>https://t.me/likeconcentrat</code> - presiona el enlace para copiar",
     'fr': "🚶🏽 Envoyez <b>lien</b> au groupe comme source pour les nouveaux membres\n\n👉🏼 Par exemple, <code>https://t.me/likeconcentrat</code> - appuyez sur le lien pour le copier",
     'zh': "🚶🏽 將 <b>link</b> 發送到群組作為新成員的來源\n\n👉🏼 例如，<code>https://t.me/likeconcentrat</code> - 推送鏈接以進行複制",
     'ar': "🚶🏽 أرسل <b> ارتباط </b> للمجموعة كمصدر للأعضاء الجدد \n\n👉🏼 على سبيل المثال ، <code> https://t.me/likeconcentrat </code> - ادفع الرابط للنسخ",
 }
 l_correct_link = {
@@ -4929,15 +4929,15 @@
     'en': "👩🏽‍💻 Send correct link or try again later",
     'es': "👩🏽‍💻 Envíe el enlace correcto o vuelva a intentarlo más tarde",
     'fr': "👩🏽‍💻 Envoyez le lien correct ou réessayez plus tard",
     'zh': "👩🏽‍💻 發送正確的鏈接或稍後再試",
     'ar': "👩🏽‍💻 أرسل الرابط الصحيح أو حاول مرة أخرى لاحقًا",
 }
 l_admin_require = {
-    'ru': "🔺 Требуются права администратора",
+    'ru': "👩🏽‍💻 Требуются права администратора",
     'en': "👩🏽‍💻 Send correct link or try again later",
     'es': "👩🏽‍💻 Envíe el enlace correcto o vuelva a intentarlo más tarde",
     'fr': "👩🏽‍💻 Envoyez le lien correct ou réessayez plus tard",
     'zh': "👩🏽‍💻 發送正確的鏈接或稍後再試",
     'ar': "👩🏽‍💻 أرسل الرابط الصحيح أو حاول مرة أخرى لاحقًا",
 }
 l_group_not_channel = {
@@ -4985,15 +4985,15 @@
     'en': "🚶🏽 Enter correct number",
     'es': "🚶🏽 Ingrese el número correcto",
     'fr': "🚶🏽 Entrez le bon numéro",
     'zh': "🚶輸入正確的數字",
     'ar': "🚶🏽 Enter correct number",
 }
 l_fsm_invite_finish = {
-    'ru': "🚶🏽 Готово! Настроен <b>авто</b>-инвайт <u>{0}</u> пользователей в сутки из группы {1}",
+    'ru': "🚶🏽 <b>Готово!</b> Настроен <b>авто</b>-инвайт <u>{0}</u> пользователей в сутки из группы {1}",
     'en': "🚶🏽 Ready! <b>Auto</b>-inviting <u>{0}</u> users per day from group {1}",
     'es': "🚶🏽 Listo! Invitación <b>automática</b> a <u>{0}</u> usuarios por día del grupo {1}",
     'fr': "🚶🏽 Prêt ! <b>Auto</b>-inviter <u>{0}</u> utilisateurs par jour du groupe {1}",
     'zh': "🚶🏽 準備好了！ <b>自動</b>-每天從組 {1} 中邀請 <u>{0}</u> 個用戶",
     'ar': "🚶🏽 جاهز! <b> دعوة تلقائية </b> <u>{0}</u> للمستخدمين يوميًا من المجموعة {1}",
 }
 l_cinvite_nosrc = {
@@ -5101,40 +5101,40 @@
     'ar': "🚶🏽 جاهز! <b> دعوة تلقائية </b> <u>{0}</u> للمستخدمين يوميًا من المجموعة {1}",
 }
 # endregion
 
 
 # region csystem_
 l_csystem_text = {
-    'ru': "👣 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> <i>системные</i> сообщения\n\n👉🏼 Например, <i>Пользователь вступил(а) в группу</i>",
+    'ru': "👣 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <i>системные</i> сообщения\n\n👉🏼 Например, <i>Пользователь вступил(а) в группу</i>",
     'en': "👣 Push the ✅/☑️, to <b>On/Off</b> <i>system</i> messages\n\n👉🏼 For example, <i>User joined the group</i>",
     'es': "👣 Presiona ✅/☑️, para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👉🏼 Por ejemplo, <i>Usuario se unió al grupo</i>",
     'fr': "👣 Appuyez sur ✅/☑️, pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👉🏼 Par exemple, <i>L'utilisateur a rejoint le groupe</i>",
     'zh': "👣 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👉🏼 例如，<i>用戶加入群組</i>",
     'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👉🏼 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
 }
 # endregion
 
 
 # region cchannel_
 l_cchannel_text = {
-    'ru': "🫥 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> <i>возможность</i> пользователю в группе писать <i>анонимно</i> (от имени <b>его</b> канала)",
+    'ru': "🫥 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <i>возможность</i> пользователю в группе писать <i>анонимно</i> (от имени <b>его</b> канала)",
     'en': "🫥 Push the ✅/☑️, to <b>On/Off</b> <i>opportunity</i> for users in group to write <i>anonymously</i> (from name of <b>his</b> channel)",
     'es': "🫥 Presiona ✅/☑️ para <b>Activar/Desactivar</b> <i>oportunidad</i> para que los usuarios del grupo escriban <i>anónimamente</i> (del nombre de <b>su</b> canal)",
     'fr': "🫥 Poussez le ✅/☑️, sur <b>On/Off</b> <i>opportunité</i> pour les utilisateurs du groupe d'écrire <i>anonymement</i> (du nom de <b>son</b> canal)",
     'zh': "🫥 將 ✅/☑️ 推到 <b>On/Off</b> <i>機會</i> 讓群組中的用戶<i>匿名</i> （來自<b>他的名字</b> 頻道）",
     'ar': "🫥 اضغط على ✅/☑️ ، من أجل <b> تشغيل / إيقاف </b> <i> فرصة </i> للمستخدمين في المجموعة لكتابة <i> مجهول </i> (من اسم <b> الخاص به </b> قناة)",
 }
 
 # endregion
 
 
 # region clink_
 l_clink_text = {
-    'ru': "🔗 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> <i>внешние <b>ссылки</b>/telegram-<b>ссылки</b>/forward</i>-<b>ссылки</b>\n\n👉🏼 Например, [✅☑Вкл forward-ссылки] означает разрешение на <b>forward-пересылку</b> сообщений из <u>других</u> Telegram-<i>каналов/групп/аккаунтов</i> в <u>нашу</u> группу",
+    'ru': "🔗 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <i>внешние <b>ссылки</b>/telegram-<b>ссылки</b>/forward</i>-<b>ссылки</b>\n\n👉🏼 Например, [✅☑Вкл forward-ссылки] означает разрешение на <b>forward-пересылку</b> сообщений из <u>других</u> Telegram-<i>каналов/групп/аккаунтов</i> в <u>нашу</u> группу",
     'en': "🔗 Push the ✅/☑️, to <b>On/Off</b> <i>externak <b>links</b>/telegram-<b>links</b>/forward</i>-<b>links</b>\n\n👉🏼 For example, [✅☑On forward-links] means permission on <b>forward</b> messages from <u>other</u> Telegram-<i>channels/groups/accounts</i> into <u>our</u> group",
     'es': "🔗 Presiona ✅/☑️ para <b>Activar/Desactivar</b> <i>externak <b>enlaces</b>/telegram-<b>enlaces</b>/reenviar</i>-<b>enlaces</b>\n\n👉🏼 Por ejemplo, [✅☑On forward-links] significa permiso en <b>reenviar</b> mensajes de <u>otros</u> Telegram-<i>canales /grupos/cuentas</i> en <u>nuestro</u> grupo",
     'fr': "🔗 Appuyez sur le ✅/☑️, sur <b>On/Off</b> <i>externak <b>links</b>/telegram-<b>links</b>/forward</i>-<b>liens</b>\n\n👉🏼 Par exemple, [✅☑On forward-links] signifie l'autorisation de <b>transférer</b> les messages provenant d'<u>autres</u> chaînes Telegram-<i> /groupes/comptes</i> dans <u>notre</u> groupe",
     'zh': "🔗 將 ✅/☑️ 推到 <b>On/Off</b> <i>externak <b>links</b>/telegram-<b>links</b>/forward</i>-<b>links</b>\n\n👉🏼 例如，[✅☑On forward-links] 表示允許 <b>forward</b> 來自 <u>other</u> Telegram-<i> 頻道的消息 /groups/accounts</i> 進入 <u>我們的</u> 組",
     'ar': "🔗 ادفع ✅ / ☑️ إلى تشغيل / إيقاف روابط خارجية telegram- روابط/ إعادة توجيه الروابط \n\n👉🏼 على سبيل المثال ، [على روابط إعادة التوجيه] تعني إذنًا بشأن <b> إعادة توجيه </b> الرسائل من أخرى Telegram قنوات/groups/accounts في مجموعتنا",
 }
 l_clink_http_on = {
@@ -5186,15 +5186,15 @@
     'ar': "☑️☐ تعطيل forward-الروابط",
 }
 # endregion
 
 
 # region csymbol_
 l_csymbol_text = {
-    'ru': "文 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> <u>авто</u>-бан <i>слов с 文-глиф, ب-араб/ <a href='https://www.zalgo.org'>zalgo-символами</a></i>\n\n👉🏼 Например, опция <b>zalgo-бан</b> удаляет сообщения такого вида <i>h̴̢̝̱̜͓̠̮̪̞͓͚̦͓͆͗̅̎̂͑̃̋͜e̷̡̧͙̹̥͓̣͍̰̮͙̻͍̐͒̒̍̈́̒̎̅̈́ḻ̸̨̢̘̥͛̈́̔̀̇̏̈́̂̎͠l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆̕͜͝ô̶͍̼͎͈̬̩̩̰̱͙̒͗͐̊̐̐͛̾́͗̈́̚͝͝ͅ</i>",
+    'ru': "文 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <u>авто</u>-бан <i>слов с 文-глиф, ب-араб/ <a href='https://www.zalgo.org'>zalgo-символами</a></i>\n\n👉🏼 Например, опция <b>zalgo-бан</b> удаляет сообщения такого вида <i>h̴̢̝̱̜͓̠̮̪̞͓͚̦͓͆͗̅̎̂͑̃̋͜e̷̡̧͙̹̥͓̣͍̰̮͙̻͍̐͒̒̍̈́̒̎̅̈́ḻ̸̨̢̘̥͛̈́̔̀̇̏̈́̂̎͠l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆̕͜͝ô̶͍̼͎͈̬̩̩̰̱͙̒͗͐̊̐̐͛̾́͗̈́̚͝͝ͅ</i>",
     'en': "文 Push the ✅/☑️, to <b>On/Off</b> <u>auto</u>-ban <i>words with 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👉🏼 For example, the option <b>zalgo-ban</b> delete messages <i>h̴̢̝̱̜͓̠̮̪̞͓͚̦͓͆͗̅̎̂͑̃̋͜e̷̡̧͙̹̥͓̣͍̰̮͙̻͍̐͒̒̍̈́̒̎̅̈́ḻ̸̨̢̘̥͛̈́̔̀̇̏̈́̂̎͠l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆̕͜͝ô̶͍̼͎͈̬̩̩̰̱͙̒͗͐̊̐̐͛̾́͗̈́̚͝͝ͅ</i>",
     'es': "文 Presione ✅/☑️, para <b>Encender/Apagar</b> <u>automático</u>-prohibir <i>palabras con 文-glif, ب-arab, <a href='https://www.zalgo.org'>Zalgo-Symbols</a></i>\n\n👉🏼 Por ejemplo, la opción <b>Zalgo-ban</b> Eliminar mensajes <i>h̴̢̝̱̜͓̠̮̪̞͓͚̦͓͆͗̅̎̂͑̃̋͜e̷̡̧͙̹̥͓̣͍̰̮͙̻͍̐͒̒̍̈́̒̎̅̈́ḻ̸̷̨̢̡̧̘̥͙̹̥͓̣͍̰̮͙̻͍͛̈́̔̀̐͒̒̍̈́̒̎̅̈́ḻ̸̨̢̘̥͛̈́̔̀l̶̶̡̡̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆̔̀̾̾͛͑́̏͆̕̕͜͜͝͝</i>",
     'fr': "文 Appuyez sur ✅/☑️, pour <b>On/Off</b> <u>auto</u>-bannir <i>les mots avec 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👉🏼 Par exemple, l'option <b>zalgo-ban</b> supprimer les messages <i>h̴̢̝̱̜͓̠̮̪̞͓͚̦͓͆͗̅̎̂͑̃̋͜e̷̡̧͙̹̥͓̣͍̰̮͙̻͍̐͒̒̍̈́̒̎̅̈́ḻ̸̷̨̢̡̧̘̥͙̹̥͓̣͍̰̮͙̻͍͛̈́̔̀̐͒̒̍̈́̒̎̅̈́ḻ̸̨̢̘̥͛̈́̔̀l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆̕͜͝ô̶͍̼͎͈̬̩̩̰̱͙̒͗͐̊̐̐͛̾́͗̈́̚͝͝ͅ</i>",
     'zh': "文推 ✅/☑️, 到 <b>On/Off</b> <u>auto</u>-ban <i>words with 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👉🏼 例如，選項<b>zalgo-ban</b>刪除消息",
     'ar': "文 اضغط على ✅ / ☑️ ، من أجل تشغيل / إيقاف تلقائي - حظر الكلمات التي تحتوي على -glif ، ب- arab ، <a href ='https://www.zalgo.org'>رموز zalgo</a>\n\n👉🏼 على سبيل المثال ، الخيار <b>zalgo-ban</b> يحذف الرسائل h̴̢̝̱̜͓̠̮̪̞͓͚̦͓͆͗̅̎̂͑̃̋͜e̷̡̧͙̹̥͓̣͍̰̮͙̻͍̐͒̒̍̈́̒̎̅̈́ḻ̸̨̢̘̥͛̈́̔̀̇̏̈́̂̎͠l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆̕͜͝ô̶͍̼͎͈̬̩̩̰̱͙̒͗͐̊̐̐͛̾́͗̈́̚͝͝ͅ",
 }
 l_csymbol_symbols_on = {
@@ -5230,15 +5230,15 @@
     'ar': "☑️☐ معاق zalgo-ban",
 }
 # endregion
 
 
 # region cmedia_
 l_cmedia_text = {
-    'ru': "🗣 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> разрешение на <i>media</i>-сообщения\n\n👉🏼 Например, [☑️☐Выкл видео-заметки] означает запрет на <b>видео-заметки в кружочке</b> в нашей группе\n\n👉🏼 Чтобы разрешить/запретить конкретный стикерпак, жми [⚙️Настроить]",
+    'ru': "🗣 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> разрешение на <i>media</i>-сообщения\n\n👉🏼 Например, [☑️☐Выкл видео-заметки] означает запрет на <b>видео-заметки в кружочке</b> в нашей группе\n\n👉🏼 Чтобы разрешить/запретить конкретный стикерпак, жми [⚙️Настроить]",
     'en': "🗣 Push the ✅/☑️, to <b>On/Off</b> permission on <i>media</i>-messages\n\n👉🏼 For example, [☑️☐Off video-note] means sending-prohibition on <b>video-note</b> in our group\n\n👉🏼 To allow/prohibit specific sticker-pack, push the [⚙️Configure]",
     'es': "🗣 Presiona ✅/☑️, para <b>Activar/Desactivar</b> permiso en <i>medios</i>-mensajes\n\n👉🏼 Por ejemplo, [☑️☐Off video-note] significa enviar- Prohibición de <b>notas de video</b> en nuestro grupo\n\n👉🏼 Para permitir/prohibir un paquete de calcomanías específico, presiona [⚙️Configurar]",
     'fr': "🗣 Appuyez sur ✅/☑️, sur l'autorisation <b>On/Off</b> sur les messages <i>media</i>\n\n👉🏼 Par exemple, [☑️☐Off video-note] signifie envoyer- interdiction de <b>video-note</b> dans notre groupe\n\n👉🏼 Pour autoriser/interdire un pack d'autocollants spécifique, appuyez sur [⚙️Configurer]",
     'zh': "🗣 將 ✅/☑️ 推送到 <i>media</i> 消息上的 <b>On/Off</b> 權限\n\n👉🏼 例如，[☑️☐Off video-note] 表示發送- 禁止我們組中的 <b>video-note</b>\n\n👉🏼 要允許/禁止特定的貼紙包，請按下 [⚙️Configure]",
     'ar': "🗣 ادفع ✅ / ☑️ ، إلى إذن <b> تشغيل / إيقاف </b> على <i> الوسائط </i> - الرسائل \n\n👉🏼 على سبيل المثال ، [☑️☐ Off video-note] تعني إرسال- حظر <b> ملاحظة الفيديو </b> في مجموعتنا \n\n👉🏼 للسماح / حظر حزمة ملصقات معينة ، اضغط على [⚙️ تكوين]",
 }
 l_cmedia_photo_on = {
@@ -5478,39 +5478,39 @@
     'en': "🚫 Remove",
     'es': "🚫 Eliminar",
     'fr': "🚫 Supprimer",
     'zh': "🚫 移除",
     'ar': "🚫 إزالة",
 }
 l_GROUPP_CSTICKER1_NUM1 = {
-    'ru': "🦊 Текущее количество <b>разрешенных</b> стикерпаков в <code>{0}</code>-файле: <u>{1}</u>\n\nЖми на ✅/🚫, чтобы <b>Добавить/Удалить</b> разрешенные стикерпаки",
+    'ru': "🦊 Текущее количество <b>разрешенных</b> стикерпаков в <code>{0}</code>-файле: <u>{1}</u>\n\n<b>Жми</b> на ✅/🚫, чтобы <b>Добавить/Удалить</b> разрешенные стикерпаки",
     'en': "🦊 Current number of <b>allowed</b> sticker-packs in the <code>{0}</code>-file: <u>{0}</u>\n\nPush the ✅/🚫, to <b>Add/Remove</b> allowed sticker-packs",
     'es': "🦊 Número actual de paquetes de pegatinas <b>permitidos</b> en el archivo <code>{0}</code>: <u>{0}</u>\n\nPresione ✅/🚫, para <b>Añadir/eliminar</b> paquetes de pegatinas permitidos",
     'fr': "🦊 Nombre actuel de packs d'autocollants <b>autorisés</b> dans le fichier <code>{0}</code> : <u>{0}</u>\n\nAppuyez sur ✅/🚫 pour <b>Ajouter/Supprimer</b> les packs d'autocollants autorisés",
     'zh': "🦊 <code>{0}</code>-文件中<b>允許</b>貼紙包的當前數量：<u>{0}</u>\n\n將 ✅/🚫 推到 <b>添加/刪除</b>允許的貼紙包",
     'ar': "🦊 العدد الحالي لحزم الملصقات <b> المسموح بها </b> في <code>{0}</code> -ملف: <u>{0}</u> \n\n اضغط على ✅/🚫 ، من أجل <b> إضافة / إزالة </b> حزم الملصقات المسموح بها",
 }
 l_GROUPP_CSTICKER1_NUM0 = {
-    'ru': "🦊 Текущее количество <b>разрешенных</b> стикерпаков: <u>{0}</u>\n\nЖми на ✅/🚫, чтобы <b>Добавить/Удалить</b> разрешенные стикерпаки",
+    'ru': "🦊 Текущее количество <b>разрешенных</b> стикерпаков: <u>{0}</u>\n\n<b>Жми</b> на ✅/🚫, чтобы <b>Добавить/Удалить</b> разрешенные стикерпаки",
     'en': "🦊 Current number of <b>allowed</b> sticker-packs: <u>{0}</u>\n\nPush the ✅/🚫, to <b>Add/Remove</b> allowed sticker-packs",
     'es': "🦊 Número actual de paquetes de adhesivos <b>permitidos</b>: <u>{0}</u>\n\nPresione ✅/🚫 para <b>Agregar/Quitar</b> paquetes de adhesivos permitidos",
     'fr': "🦊 Nombre actuel de packs d'autocollants <b>autorisés</b> : <u>{0}</u>\n\nAppuyez sur ✅/🚫 pour <b>ajouter/supprimer</b> les packs d'autocollants autorisés",
     'zh': "🦊 當前<b>允許</b>個貼紙包的數量：<u>{0}</u>\n\n按下 ✅/🚫，以<b>添加/刪除</b>個允許的貼紙包",
     'ar': "🦊 العدد الحالي لحزم الملصقات <b> المسموح بها </b>: <u>{0}</u> \n\n اضغط على ✅/🚫 ، من أجل <b> إضافة / إزالة </b> حزم الملصقات المسموح بها",
 }
 l_GROUPP_CSTICKER0_NUM1 = {
-    'ru': "🦊 Текущее количество <b>запрещенных</b> стикерпаков в <code>{0}</code>-файле: <u>{1}</u>\n\nЖми на ✅/🚫, чтобы <b>Добавить/Удалить</b> запрещенные стикерпаки",
+    'ru': "🦊 Текущее количество <b>запрещенных</b> стикерпаков в <code>{0}</code>-файле: <u>{1}</u>\n\n<b>Жми</b> на ✅/🚫, чтобы <b>Добавить/Удалить</b> запрещенные стикерпаки",
     'en': "🦊 Current number of <b>prohibited</b> sticker-packs in the <code>{0}</code>-file: <u>{0}</u>\n\nPush the ✅/🚫, to <b>Add/Remove</b> prohibited sticker-packs",
     'es': "🦊 Número actual de paquetes de adhesivos <b>prohibidos</b> en el archivo <code>{0}</code>: <u>{0}</u>\n\nPresione el ✅/🚫 para <b>Añadir/eliminar</b> paquetes de pegatinas prohibidos",
     'fr': "🦊 Nombre actuel de packs d'autocollants <b>interdits</b> dans le fichier <code>{0}</code> : <u>{0}</u>\n\nAppuyez sur ✅/🚫 pour <b>Ajouter/Supprimer</b> des packs d'autocollants interdits",
     'zh': "🦊 <code>{0}</code>-文件中<b>禁止</b>貼紙包的當前數量：<u>{0}</u>\n\n將 ✅/🚫 推到 <b>添加/刪除</b>禁止的貼紙包",
     'ar': "🦊 العدد الحالي لحزم الملصقات <b> المحظورة </b> في <code>{0}</code> -ملف: <u>{0}</u> \n\n اضغط على ✅/🚫 ، من أجل <b> إضافة / إزالة </b> حزم الملصقات المحظورة",
 }
 l_GROUPP_CSTICKER0_NUM0 = {
-    'ru': "🦊 Текущее количество <b>запрещенных</b> стикерпаков: <u>{0}</u>\n\nЖми на ✅/🚫, чтобы <b>Добавить/Удалить</b> запрещенные стикерпаки",
+    'ru': "🦊 Текущее количество <b>запрещенных</b> стикерпаков: <u>{0}</u>\n\n<b>Жми</b> на ✅/🚫, чтобы <b>Добавить/Удалить</b> запрещенные стикерпаки",
     'en': "🦊 Current number of <b>prohibited</b> sticker-packs: <u>{0}</u>\n\nPush the ✅/🚫, to <b>Add/Remove</b> prohibited sticker-packs",
     'es': "🦊 Número actual de paquetes de adhesivos <b>prohibidos</b>: <u>{0}</u>\n\nPresione ✅/🚫 para <b>Agregar/Quitar</b> paquetes de adhesivos prohibidos",
     'fr': "🦊 Nombre actuel de packs d'autocollants <b>interdits</b> : <u>{0}</u>\n\nAppuyez sur ✅/🚫 pour <b>Ajouter/Supprimer</b> des packs d'autocollants interdits",
     'zh': "🦊 當前<b>禁止</b>貼紙包的數量：<u>{0}</u>\n\n按下 ✅/🚫，<b>添加/刪除</b>禁止貼紙包",
     'ar': "🦊 العدد الحالي لحزم الملصقات <b> المحظورة </b>: <u>{0}</u> \n\n اضغط على ✅/🚫 ، من أجل <b> إضافة / إزالة </b> حزم الملصقات المحظورة",
 }
 l_cstickeroperation_add = {
@@ -5550,27 +5550,27 @@
     'en': "🚫 Send link or <b>sticker-pack</b>-name to <b>remove</b> it from prohibited list{0}",
     'es': "🚫 Enviar enlace o nombre de <b>paquete de pegatinas</b> para <b>eliminarlo</b> de la lista prohibida{0}",
     'fr': "🚫 Envoyez le lien ou le nom du <b>pack d'autocollants</b> pour le <b>supprimer</b> de la liste interdite{0}",
     'zh': "🚫 發送鏈接或 <b>sticker-pack</b>-name 以將其從禁止列表中<b>刪除</b>{0}",
     'ar': "🚫 أرسل رابطًا أو اسم <b> حزمة الملصقات </b> <b> لإزالته </b> من القائمة المحظورة {0}",
 }
 l_fsm_sticker_add = {
-    'ru': "🦊 Готово! <b>Исключения</b> для стикерпаков:\n\n+ Разрешенные: <u>{0}</u>\n- Запрещенные: <u>{1}</u>\n\n[✅ Разрешить] пропускает указанные стикерпаки <i>в качестве исключения</i>, когда выбрана опция [☑️☐Выкл sticker]\n[🚫 Запретить] запрещает указанные стикерпаки <i>в качестве исключения</i>, когда выбрана опция [✅☑Вкл sticker]",
+    'ru': "🦊 <b>Готово!</b> <b>Исключения</b> для стикерпаков:\n\n+ Разрешенные: <u>{0}</u>\n- Запрещенные: <u>{1}</u>\n\n[✅ Разрешить] пропускает указанные стикерпаки <i>в качестве исключения</i>, когда выбрана опция [☑️☐Выкл sticker]\n[🚫 Запретить] запрещает указанные стикерпаки <i>в качестве исключения</i>, когда выбрана опция [✅☑Вкл sticker]",
     'en': "🦊 Ready! <b>Exceptions</b> for sticker-packs:\n\n+ Allowed: <u>{0}</u>\n- Prohibited: <u>{1}</u>\n\n[✅ Allow] allow specified sticker-packs <i>as exception</i>, when [☑️☐Off sticker]\n[🚫 Prohibit] prohibits the specified sticker-packs <i>as exception</i>, when [✅☑On sticker]",
     'es': "🦊 Listo! <b>Excepciones</b> para paquetes de pegatinas:\n\n+ Permitido: <u>{0}</u>\n- Prohibido: <u>{1}</u>\n\n[✅ Permitir] permitir paquetes de adhesivos especificados <i>como excepción</i>, cuando [☑️☐De sticker]\n[🚫 Prohibir] prohíbe los paquetes de adhesivos especificados <i>como excepción</i>, cuando [✅☑En sticker]",
     'fr': "🦊 Prêt ! <b>Exceptions</b> pour les packs d'autocollants :\n\n+ Autorisé : <u>{0}</u>\n- Interdit : <u>{1}</u>\n\n[✅ Autoriser] autoriser les packs d'autocollants spécifiés <i>à titre exceptionnel</i>, lorsque [☑️☐En sticker]\n[🚫 Interdire] interdit les packs d'autocollants spécifiés <i>à titre exceptionnel</i>, lorsque [✅☑En sticker]",
     'zh': "🦊 準備好了！ 貼紙包的<b>例外情況</b>：\n\n+ 允許：<u>{0}</u>\n- 禁止：<u>{1}</u>\n\n[✅ Allow] 允許指定的貼紙包<i>作為例外</i>，當 [☑️☐Off 貼紙]\n[🚫 Prohibit] 禁止指定的貼紙包<i>作為例外</i>，當 [✅☑ 貼上]",
     'ar': "🦊 جاهز! <b> استثناءات </b> لحزم الملصقات: \n\n + المسموح بها: <u>{0}</u>\n- محظور: <u>{1}</u>\n\n [✅ السماح] السماح بحزم الملصقات المحددة <i> كاستثناء </i> ، عندما [☑️☐ ملصق إيقاف]\n[🚫 منع] يحظر حزم الملصقات المحددة <i> كاستثناء </i> ، عندما [✅☑ على الملصق]",
 }
 # endregion
 
 
 # region cstart_
 l_cstart_text = {
-    'ru': "🚀 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-ответ на триггер-сообщения, содержащие конкретные старт-слова\n\n👉🏼 Текущее количество старт-слов <u>{0}</u>",
+    'ru': "🚀 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-ответ на триггер-сообщения, содержащие конкретные старт-слова\n\n👉🏼 Текущее количество старт-слов <u>{0}</u>",
     'en': "🚀 Push the ✅/☑️, to <b>On/Off</b> auto-answer on trigger-messages, containing specific start-words\n\n👉🏼 Current number of start-words <u>{0}</u>",
     'es': "🚀 Presiona ✅/☑️, para <b>Activar/Desactivar</b> la respuesta automática en mensajes desencadenantes, que contienen palabras de inicio específicas\n\n👉🏼 Número actual de palabras de inicio <u>{0}</u>",
     'fr': "🚀 Appuyez sur ✅/☑️, pour <b>Activer/Désactiver</b> la réponse automatique aux messages déclencheurs, contenant des mots de départ spécifiques\n\n👉🏼 Nombre actuel de mots de départ <u>{0}</u>",
     'zh': "🚀 將 ✅/☑️ 推到 <b>On/Off</b> 觸發消息上的自動應答，包含特定的起始詞\n\n👉🏼 當前起始詞的數量<u>{0}</u>",
     'ar': "🚀 اضغط على ✅ / ☑️ ، لإجراء تشغيل / إيقاف الرد التلقائي على الرسائل المشغلة ، التي تحتوي على كلمات بداية محددة \n\n👉🏼 العدد الحالي لكلمات البداية {0} / ش",
 }
 l_cstart_call = {
@@ -5602,23 +5602,23 @@
     'en': "🚀 Use",
     'es': "🚀 Uso",
     'fr': "🚀 Utiliser",
     'zh': "🚀 使用",
     'ar': "🚀 استخدم",
 }
 l_cstartoperation_caption = {
-    'ru': "🚀 <b>Текущее</b> количество <i>старт-слов</i> для поста #{0} в <code>{1}</code>-файле: <u>{2}</u>\n\nЖми на ✅/🚫, чтобы <b>Добавить/Удалить</b> старт-слова",
+    'ru': "🚀 <b>Текущее</b> количество <i>старт-слов</i> для поста #{0} в <code>{1}</code>-файле: <u>{2}</u>\n\n<b>Жми</b> на ✅/🚫, чтобы <b>Добавить/Удалить</b> старт-слова",
     'en': "🚀 Current number of start-words for post #{0} in <code>{1}</code>-file: <u>{2}</u>\n\nPuch the ✅/🚫, to <b>Add/Remove</b> start-words",
     'es': "🚀 Número actual de palabras iniciales para la publicación #{0} en el archivo <code>{1}</code>: <u>{2}</u>\n\nPulse el ✅/🚫, para <b> Agregar o quitar</b> palabras de inicio",
     'fr': "🚀  Nombre actuel de mots de départ pour le message #{0} dans le fichier <code>{1}</code> : <u>{2}</u>\n\nAppuyez sur le ✅/🚫 pour <b> Ajouter/supprimer</b> des mots de départ",
     'zh': "🚀 當前的起始詞數 在 <code>{1}</code>-文件中發布 #{0}：<u>{2}</u>\n\n點擊 ✅/🚫，開始<b>添加/刪除</b> -字",
     'ar': "🚀 العدد الحالي لكلمات البداية للنشر # {0} في <code>{1}</code> -الملف:{2} \n\n قم بإرسال ✅/🚫 إلى إضافة / إزالة كلمات البداية",
 }
 l_cstartoperation_text = {
-    'ru': "🚀 <b>Текущее</b> количество <i>старт-слов</i> для поста #{0}: <u>{1}</u>\n\nЖми на ✅/🚫, чтобы <b>Добавить/Удалить</b> старт-слова",
+    'ru': "🚀 <b>Текущее</b> количество <i>старт-слов</i> для поста #{0}: <u>{1}</u>\n\n<b>Жми</b> на ✅/🚫, чтобы <b>Добавить/Удалить</b> старт-слова",
     'en': "🚀 Current number of start-words for post #{0}: <u>{2}</u>\n\nPuch the ✅/🚫, to <b>Add/Remove</b> start-words",
     'es': "🚀 Número actual de palabras de inicio para la publicación #{0}: <u>{2}</u>\n\nPresione ✅/🚫 para <b>Agregar/Quitar</b> palabras de inicio",
     'fr': "🚀  Nombre actuel de mots de départ pour le message #{0} : <u>{2}</u>\n\nAppuyez sur le ✅/🚫 pour <b>ajouter/supprimer</b> des mots de départ",
     'zh': "🚀 帖子 #{0} 的當前起始詞數：<u>{2}</u>\n\n點擊 ✅/🚫，以<b>添加/刪除</b>個起始詞",
     'ar': "🚀 العدد الحالي لكلمات البداية للنشر # {0}:{2}\n\n استخدم ✅/🚫 ، من أجل <b> إضافة / إزالة </b> كلمات البداية",
 }
 l_cstartoperation_handler = {
@@ -5642,23 +5642,23 @@
     'en': "🚫 Enter <u>start-words</u> <b>via</b> spaces or separators to <i>remove</i> them from Base{0}",
     'es': "🚫 Ingrese <u>palabras de inicio</u> <b>mediante</b> espacios o separadores para <i>eliminarlos</i> de la Base{0}",
     'fr': "🚫 輸入 <u>start-words</u> <b>via</b> 空格或分隔符以將它們從 Base 中<i>刪除</i>{0}",
     'zh': "🚫 輸入 <u>start-words</u> <b>via</b> 空格或分隔符以將它們從 Base 中<i>刪除</i>{0}",
     'ar': "🚫 أدخل كلمات البداية عبر مسافات أو فواصل <i> لإزالتها </i> من Base {0}",
 }
 l_fsm_start_add_caption = {
-    'ru': "🚀 Готово! <b>Текущее</b> количество старт-слов для поста #{0} в <code>{1}</code>-файле: <u>{2}</u>",
+    'ru': "🚀 <b>Готово!</b> <b>Текущее</b> количество старт-слов для поста #{0} в <code>{1}</code>-файле: <u>{2}</u>",
     'en': "🚀 Ready! <b>Current</b> number of start-words for post #{0} in <code>{1}</code>-file: <u>{2}</u>",
     'es': "🚀 Listo! Número <b>actual</b> de palabras de inicio para la publicación #{0} en el archivo <code>{1}</code>: <u>{2}</u>",
     'fr': "🚀 Prêt ! <b>Nombre actuel</b> de mots de départ pour le message  #{0} dans le fichier <code>{1}</code> : <u>{2}</u>",
     'zh': "🚀 準備好了！ <code>{1}</code>-文件中帖子 #{0} 的<b>當前</b> 起始字數：<u>{2}</u>",
     'ar': "🚀 جاهز! <b> العدد </b> الحالي لكلمات البداية للمشاركة # {0} في <code>{1}</code> -ملف:<u>{2}</u>",
 }
 l_fsm_start_add_text = {
-    'ru': "🚀 Готово! <b>Текущее</b> количество старт-слов для поста #{0}: <u>{1}</u>",
+    'ru': "🚀 <b>Готово!</b> <b>Текущее</b> количество старт-слов для поста #{0}: <u>{1}</u>",
     'en': "🚀 Ready! <b>Current</b> number of start-words for post #{0} <u>{1}</u>",
     'es': "🚀 Listo! <b>Número actual</b> de palabras de inicio para la publicación #{0} <u>{1}</u>",
     'fr': "🚀 Prêt ! <b>Nombre actuel</b> de mots de départ pour le message  #{0} <u>{1}</u>",
     'zh': "🚀 準備好了！ <b>當前</b>帖子#{0}的起始詞數 <u>{1}</u>",
     'ar': "🚀 جاهز! <b> العدد </b> الحالي لكلمات البداية للمشاركة # {0} <u> {1} </u>",
 }
 l_need_start_word = {
@@ -5671,15 +5671,15 @@
 }
 
 # endregion
 
 
 # region cstop_
 l_cstop_text = {
-    'ru': "🧾 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-удаление сообщений, содержащие запрещенные стоп-слова\n\n👉🏼 Текущее количество стоп-слов <u>{0}</u>",
+    'ru': "🧾 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-удаление сообщений, содержащие запрещенные стоп-слова\n\n👉🏼 Текущее количество стоп-слов <u>{0}</u>",
     'en': "🧾 Push the ✅/☑️, to <b>On/Off</b> auto-delete of messages, containing prohibited stop-words\n\n👉🏼 Current number of stop-words <u>{0}</u>",
     'es': "🧾 Pulsa ✅/☑️ para <b>activar/desactivar</b> la eliminación automática de mensajes que contengan palabras vacías prohibidas\n\n👉🏼 Número actual de palabras vacías <u>{0}</u>",
     'fr': "🧾 Appuyez sur ✅/☑️, pour <b>Activer/Désactiver</b> la suppression automatique des messages contenant des mots vides interdits\n\n👉🏼 Nombre actuel de mots vides <u>{0}</u>",
     'zh': "🧾 按下 ✅/☑️, 以<b>開/關</b>自動刪除包含禁止停用詞的消息\n\n👉🏼 當前停用詞數量<u>{0}</u>",
     'ar': "🧾 اضغط على ✅ / ☑️ ، من أجل <b> تشغيل / إيقاف </b> للحذف التلقائي للرسائل ، التي تحتوي على كلمات إيقاف محظورة \n\n👉🏼 العدد الحالي لكلمات التوقف <u>{0}</u>",
 }
 l_cstop_call = {
@@ -5687,23 +5687,23 @@
     'en': "🔔 You have to  ⚙️Configure at least one stop-word",
     'es': "🔔 Tienes que ⚙️Configurar al menos una palabra vacía",
     'fr': "🔔 Vous devez ⚙️Configurer au moins un mot vide",
     'zh': "🔔 你必須⚙️至少配置一個停用詞",
     'ar': "🔔 يجب عليك ⚙️ تكوين كلمة توقف واحدة على الأقل",
 }
 l_cstopchange_caption = {
-    'ru': "🧾 Текущее количество стоп-слов в <code>{0}</code>-файле: <u>{1}</u>\n\nЖми на ✅/🚫, чтобы <b>Добавить/Удалить</b> стоп-слова",
+    'ru': "🧾 Текущее количество стоп-слов в <code>{0}</code>-файле: <u>{1}</u>\n\n<b>Жми</b> на ✅/🚫, чтобы <b>Добавить/Удалить</b> стоп-слова",
     'en': "🧾 Current number of stop-words in <code>{0}</code>-file: <u>{1}</u>\n\nPush the ✅/🚫, to <b>Add/Remove</b> stop-words",
     'es': "🧾 Número actual de palabras vacías en el archivo <code>{0}</code>: <u>{1}</u>\n\nPresione ✅/🚫 para <b>Agregar/Quitar</b> palabras vacías",
     'fr': "🧾 Nombre actuel de mots vides dans le fichier <code>{0}</code> : <u>{1}</u>\n\nAppuyez sur ✅/🚫 pour <b>Ajouter/Supprimer</b> mots vides",
     'zh': "🧾 <code>{0}</code>-文件中當前停用詞的數量：<u>{1}</u>\n\n將 ✅/🚫 推到 <b>添加/刪除</b> 停用詞",
     'ar': "🧾 العدد الحالي لكلمات الإيقاف في <code>{0}</code> -الملف:{1}\n\n اضغط على ✅/🚫 ، من أجل إضافة / إزالة توقف الكلمات",
 }
 l_cstopchange_text = {
-    'ru': "🧾 Текущее количество стоп-слов <u>{0}</u>\n\nЖми на ✅/🚫, чтобы <b>Добавить/Удалить</b> стоп-слова",
+    'ru': "🧾 Текущее количество стоп-слов <u>{0}</u>\n\n<b>Жми</b> на ✅/🚫, чтобы <b>Добавить/Удалить</b> стоп-слова",
     'en': "🧾 Current number of stop-words: <u>{1}</u>\n\nPush the ✅/🚫, to <b>Add/Remove</b> stop-words",
     'es': "🧾 Número actual de palabras vacías: <u>{1}</u>\n\nPresione ✅/🚫 para <b>Agregar/Quitar</b> palabras vacías",
     'fr': "🧾 Nombre actuel de mots vides : <u>{1}</u>\n\nAppuyez sur ✅/🚫 pour <b>ajouter/supprimer</b> des mots vides",
     'zh': "🧾 當前停用詞數量：<u>{1}</u>\n\n按下 ✅/🚫, 以<b>添加/刪除</b>停用詞",
     'ar': "🧾 العدد الحالي لكلمات التوقف: <u>{1}</u>\n\n اضغط على ✅/🚫 ، من أجل <b> إضافة / إزالة <b/> كلمات الإيقاف",
 }
 l_cstopchange_add = {
@@ -5727,35 +5727,35 @@
     'en': "🚫 Enter <u>stop-words</u> <b>via</b> spaces or separators to <i>removed </i> them from Base{0}",
     'es': "🚫 Ingrese <u>palabras vacías</u> <b>a través de</b> espacios o separadores para <i>eliminarlos </i> de la base {0}",
     'fr': "🚫 Saisissez des <u>mots vides</u> <b>via</b> des espaces ou des séparateurs pour les <i>supprimer </i> de Base {0}",
     'zh': "🚫 輸入 <u>stop-words</u> <b>via</b> 空格或分隔符以將它們從 Base 中<i>刪除 </i>{0}",
     'ar': "🚫 أدخل <u> كلمات الإيقاف </u> <b> عبر </b> مسافات أو فواصل لـ <i> إزالتها </i> من Base {0}",
 }
 l_fsm_stop_add_caption = {
-    'ru': "🧾 Готово! <b>Текущее</b> количество стоп-слов в <code>{0}</code>-файле: <u>{1}</u>",
+    'ru': "🧾 <b>Готово!</b> <b>Текущее</b> количество стоп-слов в <code>{0}</code>-файле: <u>{1}</u>",
     'en': "🧾 Ready! <b>Current</b> number of stop-words in <code>{0}</code>-file: <u>{1}</u>",
     'es': "🧾 Listo! Número <b>actual</b> de palabras vacías en el archivo <code>{0}</code>: <u>{1}</u>",
     'fr': "🧾 Prêt ! <b>Nombre actuel</b> de mots vides dans le fichier <code>{0}</code> : <u>{1}</u>",
     'zh': "🧾 準備好了！ <b>當前</b> <code>{0}</code>-文件中的停用詞數：<u>{1}</u>",
     'ar': "🧾 جاهز! <b> العدد </b> الحالي لكلمات التوقف في <code>{0}</code> -الملف: <u>{1}</u>",
 }
 l_fsm_stop_add_text = {
-    'ru': "🧾 Готово! <b>Текущее</b> количество стоп-слов <u>{0}</u>",
+    'ru': "🧾 <b>Готово!</b> <b>Текущее</b> количество стоп-слов <u>{0}</u>",
     'en': "🧾 Ready! <b>Current</b> number of stop-words <u>{0}</u>",
     'es': "🧾 Listo! <b>Número actual</b> de palabras vacías <u>{0}</u>",
     'fr': "🧾 Prêt ! <b>Nombre actuel</b> de mots vides <u>{0}</u>",
     'zh': "🧾準備好了！ <b>當前</b>停用詞數<u>{0}</u>",
     'ar': "🧾 جاهز! <b> العدد </b> الحالي لكلمات التوقف <u>{0}</u>",
 }
 # endregion
 
 
 # region cflood_
 l_cflood_text = {
-    'ru': "💬 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> <i>проверку</i> на частоту подряд написанных сообщ за один промежуток времени\n\n👉🏼 Например, задай количество сообщ подряд, которое будет считаться флудом командой: <code>/flood 5</code>\n\n👉🏼 Или используй <b>медленный режим</b> в настройках группы для <u>1</u> сообщения",
+    'ru': "💬 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <i>проверку</i> на частоту подряд написанных сообщ за один промежуток времени\n\n👉🏼 Например, задай количество сообщ подряд, которое будет считаться флудом командой: <code>/flood 5</code>\n\n👉🏼 Или используй <b>медленный режим</b> в настройках группы для <u>1</u> сообщения",
     'en': "💬 Push the ✅/☑️, to <b>On/Off</b> messages frequency-<i>checking</i> in one period of time\n\n👉🏼 For example, specify the number of consecutive messages that will be considered as flood by the command: <code>/flood 5</code>\n\n👉🏼 Or use <b>Slow Mode</b> in the Settings of group for <u>1</u> message",
     'es': "💬 Presiona ✅/☑️, para <b>Activar/Desactivar</b> la frecuencia de mensajes-<i>comprobar</i> en un período de tiempo\n\n👉🏼 Por ejemplo, especifica la cantidad de mensajes consecutivos que será considerado como inundación por el comando: <code>/flood 5</code>\n\n👉🏼 O use <b>Modo lento</b> en la Configuración del grupo para <u>1</u> mensaje",
     'fr': "💬 Appuyez sur ✅/☑️, pour <b>Activer/Désactiver</b> la fréquence des messages-<i>vérification</i> dans une période de temps\n\n👉🏼 Par exemple, spécifiez le nombre de messages consécutifs qui sera considéré comme une inondation par la commande : <code>/flood 5</code>\n\n👉🏼 Ou utilisez le <b>mode lent</b> dans les paramètres du groupe pour <u>1</u> message",
     'zh': "💬 推 ✅/☑️, 到 <b>On/Off</b> 消息頻率-<i>檢查</i> 在一個時間段內\n\n👉🏼 例如，指定連續消息的數量 將被命令視為洪水： <code>/flood 5</code>\n\n👉🏼 或者在 <u>1</u> 的組的設置中使用 <b>Slow Mode</b> 信息",
     'ar': "💬 ادفع ✅ / ☑️ إلى تردد رسائل <b> تشغيل / إيقاف </b> - <i> التحقق </i> في فترة زمنية واحدة \n\n👉🏼 على سبيل المثال ، حدد عدد الرسائل المتتالية التي سيتم اعتباره فيضانًا بواسطة الأمر: <code> / Flood 5 </code> \n\n👉🏼 أو استخدم <b> الوضع البطيء </b> في إعدادات المجموعة لـ <u> 1 </u> رسالة",
 }
 l_cflood_count_on = {
@@ -5775,15 +5775,15 @@
     'ar': "☑️☐ تعطيل {0} رسائل",
 }
 # endregion
 
 
 # region cuser_
 l_cuser_text = {
-    'ru': "👥 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> первичную <i>задержку/свободный вход без входного контроля для premium-аккаунтов/разрешение на инвайт</i> пользователей/ботов в группу или разрешение на <i>редактирование</i> сообщений\n\n👉🏼 Например, <b>задержка</b> (<i>в мин</i>) для <u>новых</u> пользователей (перед написанием их <u>1</u>го сообщ) осуществляется командой: <code>/delay  {0}</code>",
+    'ru': "👥 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> первичную <i>задержку/свободный вход без входного контроля для premium-аккаунтов/разрешение на инвайт</i> пользователей/ботов в группу или разрешение на <i>редактирование</i> сообщений\n\n👉🏼 Например, <b>задержка</b> (<i>в мин</i>) для <u>новых</u> пользователей (перед написанием их <u>1</u>го сообщ) осуществляется командой: <code>/delay  {0}</code>",
     'en': "👥 Push the ✅/☑️, to <b>On/Off</b> primary <i>delay/free entrance without Enter Control for premium-accounts/permission for inviting</i> users/bots in group or permission to <i>edit</i> messages\n\n👉🏼 For example, <b>delay</b> (<i>in minutes</i>) for <u>new</u> users (before writing their <u>1</u>st message) executed by: <code>/delay  {0}</code>",
     'es': "👥 Presione ✅/☑️, para <b>Encender/Apagar</b> <i>retraso/entrada gratuita principal sin control de entrada para cuentas premium/permiso para invitar</i> usuarios/bots en grupo o permiso para <i>editar</i> mensajes\n\n👉🏼 Por ejemplo, <b>retraso</b> (<i>en minutos</i>) para <u>nuevos</u> usuarios (antes de escribir su <u>1</u>st mensaje) ejecutado por: <code>/delay {0}</code>",
     'fr': "👥 Appuyez sur ✅/☑️, pour <b>On/Off</b> le <i>retard principal/l'entrée gratuite sans Enter Control pour les comptes premium/l'autorisation d'inviter</i> les utilisateurs/bots en groupe ou l'autorisation de <i>modifier</i> les messages\n\n👉🏼 Par exemple, <b>délai</b> (<i>en minutes</i>) pour les <u>nouveaux</u> utilisateurs (avant d'écrire leur <u>1</u>er message) exécuté par : <code>/delay {0}</code>",
     'zh': "👥 按下 ✅/☑️，以 <b>開/關</b> 主要 <i>延遲/免費進入，無需進入高級帳戶控制/邀請</i>組中的用戶/機器人或權限<i>編輯</i>消息\n\n👉🏼例如，<u>新</u>用戶的<b>延遲</b>（<i>分鐘</i>）（在編寫他們的 <u>1</u>st message) 執行者：<code>/delay {0}</code>",
     'ar': "👥 اضغط على ✅ / ☑️ ، لـ <b> تشغيل / إيقاف </b> <i> تأخير / دخول مجاني بدون Enter Control للحسابات المميزة / إذن لدعوة </i> المستخدمين / الروبوتات في مجموعة أو إذن لـ <i> تحرير الرسائل </i> \n\n👉🏼 على سبيل المثال ، <b> تأخير </b> (<i> بالدقائق </i>) للمستخدمين <u> الجدد </u> (قبل كتابة <u> 1 </u> st) بواسطة: <code> / delay {0}</code>",
 }
 l_cuser_call = {
@@ -5876,15 +5876,15 @@
     'ar': "☑️☐ تعطيل تحرير الرسالة",
 }
 # endregion
 
 
 # region cadmin_
 l_cadmin_text = {
-    'ru': "👩🏽‍💻 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> <u>admin-доступ</u> (только к /cmd-командам для <i>других</i> администраторов) и <u>god-режим</u> (без ограничений для администраторов)\n\n👉🏼 <b>Текущие администраторы</b>:\n{0}",
+    'ru': "👩🏽‍💻 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <u>admin-доступ</u> (только к /cmd-командам для <i>других</i> администраторов) и <u>god-режим</u> (без ограничений для администраторов)\n\n👉🏼 <b>Текущие администраторы</b>:\n{0}",
     'en': "👩🏽‍💻 Push the ✅/☑️, to <b>On/Off</b> <u>admin-access</u> (to /cmd-commands for <i>other</i> admins) and <u>god-mode</u> (without limits for you and group-creator)\n\n👉🏼 <b>Current administrators</b>:\n{0}",
     'es': "👩🏽‍💻 Presiona ✅/☑️, para <b>Activar/Desactivar</b> <u>acceso de administrador</u> (para /cmd-comandos para <i>otros</i> administradores) y <u>modo dios</u> (sin límites para ti y el creador del grupo)\n\n👉🏼 <b>Administradores actuales</b>:\n{0}",
     'fr': "👩🏽‍💻 Appuyez sur ✅/☑️, pour <b>On/Off</b> <u>admin-access</u> (vers /cmd-commands pour les <i>autres</i> admins) et <u>god-mode</u> (sans limites pour vous et le créateur de groupe)\n\n👉🏼 <b>Administrateurs actuels</b> :\n{0}",
     'zh': "👩🏽‍💻 按下 ✅/☑️，到 <b>On/Off</b> <u>admin-access</u>（到 <i>other</i> 管理員的 /cmd-commands）和 <u>上帝模式</u>（對您和群組創建者沒有限制）\n\n👉🏼 <b>當前管理員</b>：\n{0}",
     'ar': "👩🏽‍💻 اضغط على ✅ / ☑️ ، من أجل <b> تشغيل / إيقاف </b> <u> وصول المشرف </u> (أوامر /cmd لـ <i> مشرفين آخرين </i>) و <u> god-mode </u> (بلا حدود لك ولمنشئ المجموعة) \n \n👉🏼 <b> المسؤولون الحاليون </b>: \n {0}",
 }
 l_cadmin_admin_on = {
@@ -5944,15 +5944,15 @@
     'en': "🚶🏽 Inviting of @name_bot is not allowed",
     'es': "🚶🏽 No se permite invitar a @name_bot",
     'fr': "🚶🏽 L'invitation de @name_bot n'est pas autorisée",
     'zh': "🚶🏽 不允許邀請 @name_bot",
     'ar': "🚶🏽 دعوة @name_bot غير مسموح بها",
 }
 l_content_types_button = {
-    'ru': "👮🏽 {0}, нажми на кнопку, чтобы вс︎тупить в группу",
+    'ru': "👮🏽 {0}, на<b>Жми</b> на кнопку, чтобы вс︎тупить в группу",
     'en': "👮🏽 {0}, push the button to join the group",
     'es': "👮🏽 {0}, presiona el botón para unirte al grupo",
     'fr': "👮🏽 {0}, appuyez sur le bouton pour rejoindre le groupe",
     'zh': "👮🏽 {0}，按按鈕加入群組",
     'ar': "👮🏽 {0} ، اضغط على الزر للانضمام إلى المجموعة",
 }
 l_content_types_captcha = {
@@ -6231,97 +6231,130 @@
     'en': "➕ Add bot",
     'es': "➕ Agregar grupo",
     'fr': "➕ Ajouter un bote",
     'zh': "➕ 添加組",
     'ar': "➕ إضافة مجموعة",
 }
 l_clone_bot_wait = {
-    'ru': "©️ Ожидай окончания клонирования бота\n\n#длительность 1мин",
+    'ru': "©️ <b>Клонирование</b> бота\n\n#длительность 1мин",
     'en': "➕ Add bot",
     'es': "➕ Agregar grupo",
     'fr': "➕ Ajouter un bote",
     'zh': "➕ 添加組",
     'ar': "➕ إضافة مجموعة",
 }
 l_addbot_handler = {
     'ru': "➕ Пришли корректный <b>ТОКЕН</b> Telegram-бота, полученный с помощью @botFather-бота\n\n👩🏽‍💻 Например, <code>117783159:BBAD2Kz2h8AQtHYiVtuyyyASdMN</code>",
     'en': "➕ <b>Create</b>/<code>user extra</code> <i>Telegram</i>-bot via <b>mobile</b> app, and then send its phone <u>number</u>℡\n\n👩🏽‍💻 For example, <code>79331114545</code>",
     'es': "➕ Volver..",
     'fr': "➕ Retour..",
     'zh': "➕ 回來..",
     'ar': "🔙 رجوع ..",
 }
+l_wait_for_translate_bot = {
+    'ru': "👩🏽‍💻 <b>Перевод</b> {0}-бота на <i>{1}</i>-язык\n\n#длительность 0мин",
+    'en': "👩🏽‍💻 <b>Template</b> for @{0} is ready!",
+    'es': "➕ Volver..",
+    'fr': "➕ Retour..",
+    'zh': "➕ 回來..",
+    'ar': "🔙 رجوع ..",
+}
+l_template_is_ready = {
+    'ru': "👩🏽‍💻 <b>Шаблон</b> для @{0} готов!",
+    'en': "👩🏽‍💻 <b>Template</b> for @{0} is ready!",
+    'es': "➕ Volver..",
+    'fr': "➕ Retour..",
+    'zh': "➕ 回來..",
+    'ar': "🔙 رجوع ..",
+}
+l_payment_successful = {
+    'ru': "👩🏽‍💻 <b>Пользователь</b> {0} 💰Внес оплату в размере {1} {2}",
+    'en': "👩🏽‍💻 <b>Template</b> for @{0} is ready!",
+    'es': "➕ Volver..",
+    'fr': "➕ Retour..",
+    'zh': "➕ 回來..",
+    'ar': "🔙 رجوع ..",
+}
+l_promocode_activated = {
+    'ru': "👩🏽‍💻 *Промокод*: `{txt}` активирован",
+    'en': "👩🏽‍💻 <b>Template</b> for @{0} is ready!",
+    'es': "➕ Volver..",
+    'fr': "➕ Retour..",
+    'zh': "➕ 回來..",
+    'ar': "🔙 رجوع ..",
+}
 
 # region commands
 l_bot_commands_handler = {
-    'ru': "⚙️ <b>Команды</b> /cmd для <b>@{0}</b>\n\n/update <i>копирование профиля</i>\n/info   <i>информация об боте</i>\n/stat   <i>аналитика бота</i>\n/status <i>статус бота</i>\n/log    <i>недавние действия</i>\n/on     <i>включить бот</i>\n<code>/off</code>    <i>выключить бот</i>\n<code>/repair</code> <i>очистка бота: чтение истории</i>\n<code>/reset</code>  <i>сброс бота: удаление диалогов</i>\n\n/parse      <i>[ссылка/id на чат] [аргумент]</i>\n/login      <i>вход в бот</i>\n/spambot    <i>карма бота</i>\n/autodel+days   <i>автоудаление 1-365 days</i>\n/delay+sec  <i>задержка авто-ответа</i>\n/join+file  <i>вступить в группы/каналы</i>\n/vote       <i>[id чата] [вариант ответа]</i>\n<code>/leaveall</code>   <i>покинуть все группы и каналы</i>\n<code>/deleteall</code>  <i>удалить все диалоги</i>\n\n# только от имени бота\n/screen <i>скриншот-уведомление</i>\n/type+сообщ     <i>печатание</i>\n/think          <i>обдумывание</i>\n<code>* отправка геопозиции возвращает @username-список</code>",
+    'ru': "⚙️ <b>Команды</b> /cmd для <b>@{0}</b>\n\n/info   <i>информация</i>\n/stat   <i>аналитика</i>\n/on     <i>включение</i>\n<code>/off</code>    <i>выключение</i>\n<code>/restart</code>  <i>перезагрузка</i>\n/status <i>статус</i>\n\n/parse [аргумент]  <i>участники</i>\n/admin      <i>администраторы</i>\n/promo      <i>промокод</i>\n/ban [id/@username]   <i>список</i>/unban     <i>разбан</i>",
     'en': "⚙️ <b>Account commands</b> /cmd for <b>{0}</b> in @{1} works also and in the target bot\n\n/update <i>profile copy</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/status <i>bot status</i>\n/log    <i>recent actions</i>\n/on     <i>enable bot</i>\n<code>/off</code>    <i>disable bot</i>\n<code>/repair</code> <i>accout clear: reading history</i>\n<code>/reset</code>  <i>bot reset: deleting dialogs</i>\n\n/parse      <i>[link/id on chat] [argument]</i>\n/login      <i>login to bot</i>\n/spambot    <i>bot karma</i>\n/autodel+days   <i>auto-deletion 1-365 days</i>\n/delay+sec  <i>auto-delay of auto-answer</i>\n/join+file  <i>join to groups/channels</i>\n/vote       <i>[id of chat] [option]</i>\n<code>/leaveall</code>   <i>leave all groups/channels</i>\n<code>/deleteall</code>  <i>delete all dialogs</i>\n\n# only from bot name\n/screen <i>screenshort-nortification</i>\n/type+msg     <i>typing</i>\n/think          <i>thinking</i>\n<code>* geo-location sending returns @username-list</code>",
     'es': "⚙️ Configuración de <b>Grupo</b> de <b>{0}</b>{1}\n\n<b>⛏ Comandos de administración @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-bots</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from bot for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in bot for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-bots</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for bot</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
     'fr': "⚙️ Paramètres de <b>bote</b> de <b>{0}</b>{1}\n\n<b>⛏ Commandes d'administration @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-bots</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from bot for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in bot for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-bots</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for bot</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
     'zh': "⚙️ <b>組</b>設置 <b>{0}</b>{1}\n\n<b>⛏ 管理員命令 @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-bots</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from bot for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in bot for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-bots</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for bot</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
     'ar': "⚙️ إعدادات <b> المجموعة </b> الخاصة بـ <b>{0}</b>{1}\n\n<b>⛏ أوامر المسؤول @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-bots</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from bot for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in bot for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-bots</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for bot</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
 }
 l_bot_status_handler = {
-    'ru': "👩🏽‍💻 Бот-статус: {0}",
+    'ru': "👩🏽‍💻 <b>Статус</b> @{0}-бота: {1}",
     'en': "👩🏽‍💻 Account-status: {0}",
     'es': "🎉 Enviar este comando como respuesta al mensaje",
     'fr': "🎉 Envoyez cette commande en réponse au message",
     'zh': "🎉 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_bot_on_handler = {
-    'ru': "👩🏽‍💻 Начинаем запуск бота..\n\n#длительность 1мин",
+    'ru': "👩🏽‍💻 <b>Запуск</b> @{0}-бота..\n\n#длительность 1мин",
     'en': "👩🏽‍💻 Begin to start bot..\n\n#duration 1min",
     'es': "🎉 Enviar este comando como respuesta al mensaje",
     'fr': "🎉 Envoyez cette commande en réponse au message",
     'zh': "🎉 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_bot_on_handler_already = {
-    'ru': "👩🏽‍💻 Бот уже запущен",
+    'ru': "👩🏽‍💻 <b>@{0}</b>-бот уже запущен",
     'en': "👩🏽‍💻 Account have already started",
     'es': "🎉 Enviar este comando como respuesta al mensaje",
     'fr': "🎉 Envoyez cette commande en réponse au message",
     'zh': "🎉 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_bot_off_handler = {
-    'ru': "👩🏽‍💻 Завершаем сессию бота {0}..\n\n#длительность 1мин",
+    'ru': "👩🏽‍💻 <b>Остановка</b> @{0}-бота..\n\n#длительность 1мин",
     'en': "👩🏽‍💻 Finishing bot-session {0}..\n\n#duration 1min",
     'es': "🎉 Enviar este comando como respuesta al mensaje",
     'fr': "🎉 Envoyez cette commande en réponse au message",
     'zh': "🎉 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_bot_off_handler_already = {
-    'ru': "👩🏽‍💻 Бот уже выключен",
+    'ru': "👩🏽‍💻 <b>@{0}</b>-бот уже выключен",
     'en': "👩🏽‍💻 Account have already finished",
     'es': "🎉 Enviar este comando como respuesta al mensaje",
     'fr': "🎉 Envoyez cette commande en réponse au message",
     'zh': "🎉 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_bot_off_handler_done = {
-    'ru': "👩🏽‍💻 Бот выключен",
+    'ru': "👩🏽‍💻 <b>@{0}</b>-бот выключен",
     'en': "👩🏽‍💻 Account is off",
     'es': "🎉 Enviar este comando como respuesta al mensaje",
     'fr': "🎉 Envoyez cette commande en réponse au message",
     'zh': "🎉 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_bot_restart_handler = {
-    'ru': "👩🏽‍💻 Перезапуск бота {0}..\n\n#длительность 1мин",
+    'ru': "👩🏽‍💻 <b>Перезапуск</b> @{0}-бота..\n\n#длительность 1мин",
     'en': "👩🏽‍💻 Restart of bot-session {0}..\n\n#duration 1min",
     'es': "🎉 Enviar este comando como respuesta al mensaje",
     'fr': "🎉 Envoyez cette commande en réponse au message",
     'zh': "🎉 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 # endregion
 
+
 # region bot
 l_bot_config = {
     ("cctor", "👩🏽‍💻", "☑"): {
         'ru': "Конструктор ᴺᴱᵂ",
         'en': "Builder ᴺᴱᵂ",
         'es': "Builder ᴺᴱᵂ",
         'fr': "Builder ᴺᴱᵂ",
@@ -6448,38 +6481,29 @@
     'ru': "🚫 Бот успешно откреплен [<b>{0}</b>]",
     'en': "🚫 Bot successfully disconnected from bot [<b>{0}</b>] and does not control it!",
     'es': "🚫 ¡El bot se desconectó con éxito del grupo [<b>{0}</b>] y no es miembro en absoluto!",
     'fr': "🚫 Le bot s'est déconnecté avec succès du bote [<b>{0}</b>] et il n'est pas du tout membre !",
     'zh': "🚫 Bot 已成功與群組 [<b>{0}</b>] 斷開連接，並且它根本不是成員！",
     'ar': "🚫 تم قطع اتصال البوت بنجاح بالمجموعة [<b>{0}</b>] وهو ليس عضوًا على الإطلاق!",
 }
-
-l_transfer_need_username = {
-    'ru': "👩🏽‍💻 Установи @username своего Telegram-профиля, чтобы получить права владения на @{0}-бота",
-    'en': "🚫 Bot successfully disconnected from bot [<b>{0}</b>] and does not control it!",
-    'es': "🚫 ¡El bot se desconectó con éxito del grupo [<b>{0}</b>] y no es miembro en absoluto!",
-    'fr': "🚫 Le bot s'est déconnecté avec succès du bote [<b>{0}</b>] et il n'est pas du tout membre !",
-    'zh': "🚫 Bot 已成功與群組 [<b>{0}</b>] 斷開連接，並且它根本不是成員！",
-    'ar': "🚫 تم قطع اتصال البوت بنجاح بالمجموعة [<b>{0}</b>] وهو ليس عضوًا على الإطلاق!",
-}
 l_transfer_success = {
-    'ru': "👩🏽‍💻 Права владения на @{0}-бота успешно переданы Вашему аккаунту!\n\n👩🏽‍💻 Теперь для передачи прав/настройки можно использовать @botfather-бота",
+    'ru': "👩🏽‍💻 <b>Права</b> владения на @{0}-бота успешно переданы @{1}-аккаунту!\n\n👩🏽‍💻 Теперь для передачи прав/настройки можно использовать @botfather-бота",
     'en': "🚫 Bot successfully disconnected from bot [<b>{0}</b>] and does not control it!",
     'es': "🚫 ¡El bot se desconectó con éxito del grupo [<b>{0}</b>] y no es miembro en absoluto!",
     'fr': "🚫 Le bot s'est déconnecté avec succès du bote [<b>{0}</b>] et il n'est pas du tout membre !",
     'zh': "🚫 Bot 已成功與群組 [<b>{0}</b>] 斷開連接，並且它根本不是成員！",
     'ar': "🚫 تم قطع اتصال البوت بنجاح بالمجموعة [<b>{0}</b>] وهو ليس عضوًا على الإطلاق!",
 }
 # endregion
 
 
 # region config
 # region ctranslate_
 l_ctranslate_text = {
-    'ru': "文 Жми на ✅/☑️ чтобы <b>Вкл/Выкл</b> авто-перевод для <i>исходящих</i> сообщений бота на язык пользователя, который запускает этого бота",
+    'ru': "文 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> авто-перевод для <i>исходящих</i> сообщений бота на язык пользователя при /start-запуске бота",
     'en': "文 Push the ✅/☑️ to <b>On/Off</b> auto-translate for <i><b>income</b>/<b>outgoing</b> messages</i>",
     'es': "文 Presiona ✅/☑️ para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <i>Usuario se unió al grupo</i>",
     'fr': "文 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>L'utilisateur a rejoint le bote</i>",
     'zh': "文 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👩🏽‍💻 例如，<i>用戶加入群組</i>",
     'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👩🏽‍💻 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
 }
 l_ctranslate_in_on = {
@@ -6515,15 +6539,15 @@
     'ar': "☑️☐ تعطيل حظر معرف جديد",
 }
 # endregion
 
 
 # region canswer_
 l_canswer_text = {
-    'ru': "👋🏽 Жми на ✅/☑️ чтобы <b>Вкл/Выкл</b> режим авто-ответа на текстовые сообщения с помощью нейросети",
+    'ru': "👋🏽 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> режим авто-ответа на текстовые сообщения с помощью нейросети",
     'en': "👋🏽 Push the ✅/☑️ to <b>On/Off</b> auto-answer on triggers\n\n👩🏽‍💻 Current number of triggers: <u>{0}</u>",
     'es': "👋🏽 Presiona ✅/☑️ para <b>Activar/Desactivar</b> la respuesta automática en mensajes desencadenantes, que contienen palabras de inicio específicas\n\n👩🏽‍💻 Número actual de palabras de inicio <u>{0}</u>",
     'fr': "👋🏽 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> la réponse automatique aux messages déclencheurs, contenant des mots de départ spécifiques\n\n👩🏽‍💻 Nombre actuel de mots de départ <u>{0}</u>",
     'zh': "👋🏽 將 ✅/☑️ 推到 <b>On/Off</b> 觸發消息上的自動應答，包含特定的起始詞\n\n👩🏽‍💻 當前起始詞的數量<u>{0}</u>",
     'ar': "🚀 اضغط على ✅ / ☑️ ، لإجراء تشغيل / إيقاف الرد التلقائي على الرسائل المشغلة ، التي تحتوي على كلمات بداية محددة \n\n👩🏽‍💻 العدد الحالي لكلمات البداية {0} / ش",
 }
 # endregion
@@ -6535,15 +6559,15 @@
     'en': "🗝️ You have to ⚙️Configure post and source for sending",
     'es': "🗝️ Tienes que ⚙️ Configurar al menos una palabra de inicio",
     'fr': "🗝️ Vous devez ⚙️ Configurer au moins un mot de départ",
     'zh': "🗝️ 你必須 ⚙️ 配置至少一個起始詞",
     'ar': "🔔 يجب عليك ⚙️ تكوين كلمة بداية واحدة على الأقل",
 }
 l_cpayment_text = {
-    'ru': "💳️ Жми на ✅/☑️ чтобы <b>Вкл/Выкл</b> платежи в @{0}-боте\n\n👩🏽‍💻 <b>Текущий</b> платежный токен:\n<code>{1}</code>",
+    'ru': "💳️ <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> платежи в @{0}-боте\n\n👩🏽‍💻 <b>Текущий</b> платежный токен:\n<code>{1}</code>",
     'en': "🗝️ Push the ✅/☑️ to <b>On/Off</b> auto-sending choosen post to many users\n\n👩🏽‍💻 <b>Current</b> settings of auto-sending: {0}",
     'es': "🗝️ Presiona ✅/☑️ para <b>activar/desactivar</b> la invitación automática de usuarios a tu grupo\n\n👩🏽‍💻 Invitar a <u>{0}</u> usuarios por día del grupo {1}",
     'fr': "🗝️ Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> l'invitation automatique d'utilisateurs dans votre bote\n\n👩🏽‍💻 Inviter <u>{0}</u> utilisateurs par jour à partir du bote {1}",
     'zh': "🗝️ 按下 ✅/☑️ 以<b>開/關</b>自動邀請用戶加入您的群組\n\n👩🏽‍💻 每天從群組 {1} 中邀請 <u>{0}</u> 個用戶",
     'ar': "🗝️ ادفع ✅ / ☑️ إلى <b> تشغيل / إيقاف </b> لدعوة المستخدمين تلقائيًا إلى مجموعتك \n\n👩🏽‍💻 دعوة <u>{0}</u> مستخدمين يوميًا من المجموعة {1}",
 }
 l_cpayment_token = {
@@ -6551,15 +6575,15 @@
     'en': "🗝️ Push the ✅/☑️ to <b>On/Off</b> auto-sending choosen post to many users\n\n👩🏽‍💻 <b>Current</b> settings of auto-sending: {0}",
     'es': "🗝️ Presiona ✅/☑️ para <b>activar/desactivar</b> la invitación automática de usuarios a tu grupo\n\n👩🏽‍💻 Invitar a <u>{0}</u> usuarios por día del grupo {1}",
     'fr': "🗝️ Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> l'invitation automatique d'utilisateurs dans votre bote\n\n👩🏽‍💻 Inviter <u>{0}</u> utilisateurs par jour à partir du bote {1}",
     'zh': "🗝️ 按下 ✅/☑️ 以<b>開/關</b>自動邀請用戶加入您的群組\n\n👩🏽‍💻 每天從群組 {1} 中邀請 <u>{0}</u> 個用戶",
     'ar': "🗝️ ادفع ✅ / ☑️ إلى <b> تشغيل / إيقاف </b> لدعوة المستخدمين تلقائيًا إلى مجموعتك \n\n👩🏽‍💻 دعوة <u>{0}</u> مستخدمين يوميًا من المجموعة {1}",
 }
 l_cpayment_done = {
-    'ru': "🗝️ <b>Готово</b>!\n\n👩🏽‍💻 <b>Текущий</b> платежный токен для @{0}-бота:\n\n<code>{1}</code>",
+    'ru': "💳️ <b>Готово!</b>\n\n👩🏽‍💻 <b>Текущий</b> платежный токен для @{0}-бота:\n\n<code>{1}</code>",
     'en': "🗝️ Push the ✅/☑️ to <b>On/Off</b> auto-sending choosen post to many users\n\n👩🏽‍💻 <b>Current</b> settings of auto-sending: {0}",
     'es': "🗝️ Presiona ✅/☑️ para <b>activar/desactivar</b> la invitación automática de usuarios a tu grupo\n\n👩🏽‍💻 Invitar a <u>{0}</u> usuarios por día del grupo {1}",
     'fr': "🗝️ Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> l'invitation automatique d'utilisateurs dans votre bote\n\n👩🏽‍💻 Inviter <u>{0}</u> utilisateurs par jour à partir du bote {1}",
     'zh': "🗝️ 按下 ✅/☑️ 以<b>開/關</b>自動邀請用戶加入您的群組\n\n👩🏽‍💻 每天從群組 {1} 中邀請 <u>{0}</u> 個用戶",
     'ar': "🗝️ ادفع ✅ / ☑️ إلى <b> تشغيل / إيقاف </b> لدعوة المستخدمين تلقائيًا إلى مجموعتك \n\n👩🏽‍💻 دعوة <u>{0}</u> مستخدمين يوميًا من المجموعة {1}",
 }
 # endregion
@@ -6571,15 +6595,15 @@
     'en': "🗝️ You have to ⚙️Configure post and source for sending",
     'es': "🗝️ Tienes que ⚙️ Configurar al menos una palabra de inicio",
     'fr': "🗝️ Vous devez ⚙️ Configurer au moins un mot de départ",
     'zh': "🗝️ 你必須 ⚙️ 配置至少一個起始詞",
     'ar': "🔔 يجب عليك ⚙️ تكوين كلمة بداية واحدة على الأقل",
 }
 l_cintegration_text = {
-    'ru': "🗝️ Жми на ✅/☑️ чтобы <b>Вкл/Выкл</b> интеграцию базы пользователей с <i><b>google</b>-crm/<b>airtable</b>-crm</i>\n\n👩🏽‍💻 Например, опция [<b>{0}</b>] означает возможность интеграции базы пользователей с <i>google-crm</i>",
+    'ru': "🗝️ <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> интеграцию базы пользователей с <i><b>google</b>-crm/<b>airtable</b>-crm</i>\n\n👩🏽‍💻 Например, опция [<b>{0}</b>] означает возможность интеграции базы пользователей с <i>google-crm</i>",
     'en': "🗝️ Push the ✅/☑️ to <b>On/Off</b> auto-sending choosen post to many users\n\n👩🏽‍💻 <b>Current</b> settings of auto-sending: {0}",
     'es': "🗝️ Presiona ✅/☑️ para <b>activar/desactivar</b> la invitación automática de usuarios a tu grupo\n\n👩🏽‍💻 Invitar a <u>{0}</u> usuarios por día del grupo {1}",
     'fr': "🗝️ Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> l'invitation automatique d'utilisateurs dans votre bote\n\n👩🏽‍💻 Inviter <u>{0}</u> utilisateurs par jour à partir du bote {1}",
     'zh': "🗝️ 按下 ✅/☑️ 以<b>開/關</b>自動邀請用戶加入您的群組\n\n👩🏽‍💻 每天從群組 {1} 中邀請 <u>{0}</u> 個用戶",
     'ar': "🗝️ ادفع ✅ / ☑️ إلى <b> تشغيل / إيقاف </b> لدعوة المستخدمين تلقائيًا إلى مجموعتك \n\n👩🏽‍💻 دعوة <u>{0}</u> مستخدمين يوميًا من المجموعة {1}",
 }
 
@@ -6629,27 +6653,27 @@
     'en': "🗝️ Push the ✅/☑️ to <b>On/Off</b> auto-sending choosen post to many users\n\n👩🏽‍💻 <b>Current</b> settings of auto-sending: {0}",
     'es': "🗝️ Presiona ✅/☑️ para <b>activar/desactivar</b> la invitación automática de usuarios a tu grupo\n\n👩🏽‍💻 Invitar a <u>{0}</u> usuarios por día del grupo {1}",
     'fr': "🗝️ Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> l'invitation automatique d'utilisateurs dans votre bote\n\n👩🏽‍💻 Inviter <u>{0}</u> utilisateurs par jour à partir du bote {1}",
     'zh': "🗝️ 按下 ✅/☑️ 以<b>開/關</b>自動邀請用戶加入您的群組\n\n👩🏽‍💻 每天從群組 {1} 中邀請 <u>{0}</u> 個用戶",
     'ar': "🗝️ ادفع ✅ / ☑️ إلى <b> تشغيل / إيقاف </b> لدعوة المستخدمين تلقائيًا إلى مجموعتك \n\n👩🏽‍💻 دعوة <u>{0}</u> مستخدمين يوميًا من المجموعة {1}",
 }
 l_cintegration_done = {
-    'ru': "🗝️ <b>Готово</b>!\n\n👩🏽‍💻 Текущая ссылка:\n{0}",
+    'ru': "🗝️ <b>Готово!</b>\n\n👩🏽‍💻 Текущая ссылка:\n{0}",
     'en': "🗝️ Push the ✅/☑️ to <b>On/Off</b> auto-sending choosen post to many users\n\n👩🏽‍💻 <b>Current</b> settings of auto-sending: {0}",
     'es': "🗝️ Presiona ✅/☑️ para <b>activar/desactivar</b> la invitación automática de usuarios a tu grupo\n\n👩🏽‍💻 Invitar a <u>{0}</u> usuarios por día del grupo {1}",
     'fr': "🗝️ Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> l'invitation automatique d'utilisateurs dans votre bote\n\n👩🏽‍💻 Inviter <u>{0}</u> utilisateurs par jour à partir du bote {1}",
     'zh': "🗝️ 按下 ✅/☑️ 以<b>開/關</b>自動邀請用戶加入您的群組\n\n👩🏽‍💻 每天從群組 {1} 中邀請 <u>{0}</u> 個用戶",
     'ar': "🗝️ ادفع ✅ / ☑️ إلى <b> تشغيل / إيقاف </b> لدعوة المستخدمين تلقائيًا إلى مجموعتك \n\n👩🏽‍💻 دعوة <u>{0}</u> مستخدمين يوميًا من المجموعة {1}",
 }
 # endregion
 
 
 # region cnotification_
 l_cnotification_text = {
-    'ru': "💬 Жми на ✅/☑️ чтобы <b>Вкл/Выкл</b> оповещения о <i><b>/start-stop</b> запуске/блокировке бота пользователем и попадании пользователя в <b>/ban</b>-список/<b>нажатии</b> на кнопки пользователем/<b>диалоге</b> с администраторами/<b>всех</b> действиях пользователя</i>\n\n👩🏽‍💻 Например, опция [<b>{0}</b>] означает <code>показ</code> сообщений от пользователя администраторам бота (/admin) с возможностью реплай-ответа на сообщения",
+    'ru': "💬 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> оповещения о <i><b>/start-stop</b> запуске/блокировке бота пользователем и попадании пользователя в <b>/ban</b>-список/<b>нажатии</b> на кнопки пользователем/<b>диалоге</b> с администраторами/<b>всех</b> действиях пользователя</i>\n\n👩🏽‍💻 Например, опция [<b>{0}</b>] означает <code>показ</code> сообщений от пользователя администраторам бота (/admin) с возможностью реплай-ответа на сообщения",
     'en': "💬 Push the ✅/☑️ to <b>On/Off</b> <i>service <b>statuses</b>/<b>forward</b> income for yourself (including original/<u>deleted</u> messages)/tag about income-<b>reading</b></i>\n\n👩🏽‍💻 For example, [{0}] means <code>show</code> service <b>statuses</b>: <i>typing..search sticker..</i>",
     'es': "💬 Presiona ✅/☑️ para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <i>Usuario se unió al grupo</i>",
     'fr': "💬 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>L'utilisateur a rejoint le bote</i>",
     'zh': "💬 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👩🏽‍💻 例如，<i>用戶加入群組</i>",
     'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👩🏽‍💻 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
 }
 l_cnotification_start_on = {
@@ -6727,15 +6751,15 @@
     'ar': '🌬 حول',
 }
 # endregion
 
 
 # region cuser_
 l_cuser_text2 = {
-    'ru': "👥 Жми на ✅/☑️ чтобы <b>Вкл/Выкл</b> <i>замену голосовых/телескопов на <b>audio/video</b> (*рекомендуется, если <code>premium</code>-пользователи установили такой запрет)/сервисные <b>статусы</b> бота (печатает..записывает видео..)/ведение списка <b>/utm-рефералов</b></i>\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/parse - вывести всех пользователей\n/utm - вывести utm-рефералов\n/link - создать реферальную /utm ссылку",
+    'ru': "👥 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> <i>замену голосовых/телескопов на <b>audio/video</b> (*рекомендуется, если <code>premium</code>-пользователи установили такой запрет)/сервисные <b>статусы</b> бота (печатает..записывает видео..)/ведение списка <b>/utm-рефералов</b></i>\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/parse - вывести всех пользователей\n/utm - вывести utm-рефералов\n/link - создать реферальную /utm ссылку",
     'en': "👥 Push the ✅/☑️ to <b>On/Off</b> auro-reaction on <i><b>emoji</b> inside message/<b>media</b>-content</i>/<b>reply</b> reaction",
     'es': "👥 Presiona ✅/☑️ para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <i>Usuario se unió al grupo</i>",
     'fr': "👥 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>L'utilisateur a rejoint le bote</i>",
     'zh': "👥 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👩🏽‍💻 例如，<i>用戶加入群組</i>",
     'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👩🏽‍💻 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>"
 }
 l_cuser_restricted_on = {
@@ -6783,31 +6807,31 @@
     'en': "☑️☐Off reaction to media",
     'es': "☑️☐De nueva-id-ban",
     'fr': "☑️☐De nouveau-id-ban",
     'zh': "☑️☐關閉新身份證",
     'ar': "☑️☐ تعطيل حظر معرف جديد",
 }
 l_bot_is_off = {
-    'ru': "👩🏽‍💻 <b>Бот:</b> выключен\n\n/on - включить бот",
+    'ru': "👩🏽‍💻 <b>@{0}-бот</b> выключен\n\n/on - включить бот",
     'en': "👩🏽‍💻 <b>Account:</b> is off\n\n/on - to on bot",
     'es': "💳 Agregar grupo",
     'fr': "💳 Ajouter un bote",
     'zh': "💳 添加組",
     'ar': "💳 إضافة مجموعة",
 }
 l_cuser_utm = {
-    'ru': "👥 Готово! <b>/utm-список</b> реферальных пользователей @{0}-бота\n\n👩🏽‍💻 <b>Вывести</b> рефералов конкретного пользователя можно командой:\n<code>/utm id</code> или <code>/utm @username</code>\n\n👩🏽‍💻 Текущее число utm-рефералов: <u>{1}</u>",
+    'ru': "👥 <b>Готово!</b> <b>/utm-список</b> реферальных пользователей @{0}-бота\n\n👩🏽‍💻 <b>Вывести</b> рефералов конкретного пользователя можно командой:\n<code>/utm id</code> или <code>/utm @username</code>\n\n👩🏽‍💻 Текущее число utm-рефералов: <u>{1}</u>",
     'en': "👥 Ready! Gathered members: <u>{0}</u>. You can immediately make an <b>sending</b> or <b>inviting</b> to channel by received members{1}",
     'es': "👥 Listo! Miembros reunidos: <u>{0}</u>. Inmediatamente puede hacer un <b>envío</b> o <b>invitación</b> al grupo por miembros recibidos{1}",
     'fr': "👥 Prêt ! Membres réunis : <u>{0}</u>. Vous pouvez immédiatement faire un <b>envoi</b> ou <b>inviter</b> pour channeler par membres reçus{1}",
     'zh': "👥 準備好了！ 聚集成員：<u>{0}</u>。 您可以立即<b>發送</b>或<b>邀請</b>按收到的成員分組{1}",
     'ar': "🔥 جاهز! الأعضاء الذين تم تجميعهم: <u>{0}</u>. يمكنك على الفور إجراء <b> إرسال </b> أو <b> دعوة </b> للانضمام إلى المجموعة بواسطة الأعضاء المستلمين {1}",
 }
 l_cuser_link_done = {
-    'ru': "👥 <b>Готово</b>! Реферальная /utm ссылка на @{0}-бота (размести ее на любой площадке, чтобы понимать, что пользователи перешли в бота с этой площадки):\n\n<code>{1}</code>",
+    'ru': "👥 <b>Готово!</b> Реферальная /utm ссылка на @{0}-бота (размести ее на любой площадке, чтобы понимать, что пользователи перешли в бота с этой площадки):\n\n<code>{1}</code>",
     'en': "👥 Ready! Gathered members: <u>{0}</u>. You can immediately make an <b>sending</b> or <b>inviting</b> to channel by received members{1}",
     'es': "👥 Listo! Miembros reunidos: <u>{0}</u>. Inmediatamente puede hacer un <b>envío</b> o <b>invitación</b> al grupo por miembros recibidos{1}",
     'fr': "👥 Prêt ! Membres réunis : <u>{0}</u>. Vous pouvez immédiatement faire un <b>envoi</b> ou <b>inviter</b> pour channeler par membres reçus{1}",
     'zh': "👥 準備好了！ 聚集成員：<u>{0}</u>。 您可以立即<b>發送</b>或<b>邀請</b>按收到的成員分組{1}",
     'ar': "🔥 جاهز! الأعضاء الذين تم تجميعهم: <u>{0}</u>. يمكنك على الفور إجراء <b> إرسال </b> أو <b> دعوة </b> للانضمام إلى المجموعة بواسطة الأعضاء المستلمين {1}",
 }
 l_cuser_link_start = {
@@ -6815,43 +6839,43 @@
     'en': "👥 Ready! Gathered members: <u>{0}</u>. You can immediately make an <b>sending</b> or <b>inviting</b> to channel by received members{1}",
     'es': "👥 Listo! Miembros reunidos: <u>{0}</u>. Inmediatamente puede hacer un <b>envío</b> o <b>invitación</b> al grupo por miembros recibidos{1}",
     'fr': "👥 Prêt ! Membres réunis : <u>{0}</u>. Vous pouvez immédiatement faire un <b>envoi</b> ou <b>inviter</b> pour channeler par membres reçus{1}",
     'zh': "👥 準備好了！ 聚集成員：<u>{0}</u>。 您可以立即<b>發送</b>或<b>邀請</b>按收到的成員分組{1}",
     'ar': "🔥 جاهز! الأعضاء الذين تم تجميعهم: <u>{0}</u>. يمكنك على الفور إجراء <b> إرسال </b> أو <b> دعوة </b> للانضمام إلى المجموعة بواسطة الأعضاء المستلمين {1}",
 }
 l_promo_done = {
-    'ru': "👩🏽‍💻 <b>Готово</b>!\n\n👩🏽‍💻 <i>Текущий /promo-код</i>:\n<code>{0}</code>\n👩🏽‍💻 <i>Удалить /promo-код</i>:\n<code>/promo 0</code>",
+    'ru': "👩🏽‍💻 <b>Готово!</b>\n\n👩🏽‍💻 <i>Текущий /promo-код</i>:\n<code>{0}</code>\n👩🏽‍💻 <i>Удалить /promo-код</i>:\n<code>/promo 0</code>",
     'en': "👩🏽‍💻 Ready! Gathered members: <u>{0}</u>. You can immediately make an <b>sending</b> or <b>inviting</b> to channel by received members{1}",
     'es': "👩🏽‍💻 Listo! Miembros reunidos: <u>{0}</u>. Inmediatamente puede hacer un <b>envío</b> o <b>invitación</b> al grupo por miembros recibidos{1}",
     'fr': "👩🏽‍💻 Prêt ! Membres réunis : <u>{0}</u>. Vous pouvez immédiatement faire un <b>envoi</b> ou <b>inviter</b> pour channeler par membres reçus{1}",
     'zh': "👩🏽‍💻 準備好了！ 聚集成員：<u>{0}</u>。 您可以立即<b>發送</b>或<b>邀請</b>按收到的成員分組{1}",
     'ar': "🔥 جاهز! الأعضاء الذين تم تجميعهم: <u>{0}</u>. يمكنك على الفور إجراء <b> إرسال </b> أو <b> دعوة </b> للانضمام إلى المجموعة بواسطة الأعضاء المستلمين {1}",
 }
 l_promo_start = {
-    'ru': "👩🏽‍💻 <b>Придумай</b> /promo-код для @{0}-бота:\n\n👩🏽‍💻 <i>Текущий /promo-код</i>:\n<code>{1}</code>\n👩🏽‍💻 <i>Удалить /promo-код</i>:\n<code>/promo 0</code>",
+    'ru': "👩🏽‍💻 <b>Введи</b> /promo-код для @{0}-бота:\n\n👩🏽‍💻 <i>Текущий /promo-код</i>:\n<code>{1}</code>\n👩🏽‍💻 <i>Удалить /promo-код</i>:\n<code>/promo 0</code>",
     'en': "👩🏽‍💻 Ready! Gathered members: <u>{0}</u>. You can immediately make an <b>sending</b> or <b>inviting</b> to channel by received members{1}",
     'es': "👩🏽‍💻 Listo! Miembros reunidos: <u>{0}</u>. Inmediatamente puede hacer un <b>envío</b> o <b>invitación</b> al grupo por miembros recibidos{1}",
     'fr': "👩🏽‍💻 Prêt ! Membres réunis : <u>{0}</u>. Vous pouvez immédiatement faire un <b>envoi</b> ou <b>inviter</b> pour channeler par membres reçus{1}",
     'zh': "👩🏽‍💻 準備好了！ 聚集成員：<u>{0}</u>。 您可以立即<b>發送</b>或<b>邀請</b>按收到的成員分組{1}",
     'ar': "🔥 جاهز! الأعضاء الذين تم تجميعهم: <u>{0}</u>. يمكنك على الفور إجراء <b> إرسال </b> أو <b> دعوة </b> للانضمام إلى المجموعة بواسطة الأعضاء المستلمين {1}",
 }
 # endregion
 
 
 # region cadmin_
 l_cadmin_text2 = {
-    'ru': "👮🏽 Жми на ✅/☑️ чтобы <b>Вкл/Выкл</b> <i>доступ добавленных администраторов к функционалу <b>[💬 Оповещения]</b></i>\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/admin - добавить/удалить администратора\n/parse - вывести всех пользователей",
+    'ru': "👮🏽 <b>Жми</b> на ✅/☑️ чтобы <b>Вкл/Выкл</b> <i>доступ добавленных администраторов к функционалу <b>[💬 Оповещения]</b></i>\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/admin - добавить/удалить администратора\n/parse - вывести всех пользователей",
     'en': "👮🏽 Push the ✅/☑️ to <b>On/Off</b> auto-transcribe (speach to text) for <i><b>income</b>/<b>outgoing</b> messages</i>",
     'es': "👮🏽 Presiona ✅/☑️ para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <i>Usuario se unió al grupo</i>",
     'fr': "👮🏽 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>L'utilisateur a rejoint le bote</i>",
     'zh': "👮🏽 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👩🏽‍💻 例如，<i>用戶加入群組</i>",
     'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👩🏽‍💻 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
 }
 l_cadmin_done = {
-    'ru': "👮🏽 Готово! /admin-список администраторов @{0}-бота\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/admin - добавить/удалить администратора\n/parse - вывести всех пользователей\n\n👩🏽‍💻 Текущее число администраторов: <u>{1}</u>",
+    'ru': "👮🏽 <b>Готово!</b>/admin-список администраторов @{0}-бота\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/admin - добавить/удалить администратора\n/parse - вывести всех пользователей\n\n👩🏽‍💻 Текущее число администраторов: <u>{1}</u>",
     'en': "🗣 Push the ✅/☑️ to <b>On/Off</b> auto-transcribe (speach to text) for <i><b>income</b>/<b>outgoing</b> messages</i>",
     'es': "🗣 Presiona ✅/☑️ para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <i>Usuario se unió al grupo</i>",
     'fr': "🗣 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>L'utilisateur a rejoint le bote</i>",
     'zh': "🗣 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👩🏽‍💻 例如，<i>用戶加入群組</i>",
     'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👩🏽‍💻 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
 }
 l_cadmin_add = {
@@ -6867,510 +6891,26 @@
     'en': "🗣 Push the ✅/☑️ to <b>On/Off</b> auto-transcribe (speach to text) for <i><b>income</b>/<b>outgoing</b> messages</i>",
     'es': "🗣 Presiona ✅/☑️ para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <i>Usuario se unió al grupo</i>",
     'fr': "🗣 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>L'utilisateur a rejoint le bote</i>",
     'zh': "🗣 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👩🏽‍💻 例如，<i>用戶加入群組</i>",
     'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👩🏽‍💻 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
 }
 l_parse_text = {
-    'ru': "👩🏽‍💻 Готово! Парсинг пользователей (<u>{0}</u>) @{1}-бота\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/parse - вывести всех пользователей\n<code>/parse premium</code> - вывести premium-пользователей\n<code>/parse admin</code> - вывести admin-пользователей\n<code>/parse utm</code> - вывести utm-рефералов\n",
+    'ru': "👩🏽‍💻 <b>Готово!</b> Парсинг пользователей (<u>{0}</u>) @{1}-бота\n\n👩🏽‍💻 <b>Команды</b>:\n/cmd - все команды\n/parse - вывести всех пользователей\n<code>/parse premium</code> - вывести premium-пользователей\n<code>/parse admin</code> - вывести admin-пользователей\n<code>/parse utm</code> - вывести utm-рефералов\n",
     'en': "🗣 Push the ✅/☑️ to <b>On/Off</b> auto-transcribe (speach to text) for <i><b>income</b>/<b>outgoing</b> messages</i>",
     'es': "🗣 Presiona ✅/☑️ para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <i>Usuario se unió al grupo</i>",
     'fr': "🗣 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>L'utilisateur a rejoint le bote</i>",
     'zh': "🗣 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👩🏽‍💻 例如，<i>用戶加入群組</i>",
     'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👩🏽‍💻 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
 }
 # endregion
 # endregion
 
 
 # region client
-l_bot_cmd_acc = {
-    'ru': "👩🏽‍💻 <b>бот:</b> {0}\n[<b>id</b>=<code>{1}</code>]\n<b>Био:</b> {2}",
-    'en': "👩🏽‍💻 <b>Account:</b> {0}\n[<b>id</b>=<code>{1}</code>]\n<b>Bio:</b> {2}",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_acc2 = {
-    'ru': "👩🏽‍💻 <b>бот:</b> {0}\n[<b>id</b>=<code>{1}</code>, +{2}]",
-    'en': "👩🏽‍💻 <b>Account:</b> {0}\n[<b>id</b>=<code>{1}</code>, +{2}]",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-
-l_bot_cmd_info_fun = {
-    'ru': "👩🏽‍💻 <b>бот:</b> {0}\n[<b>id</b>=<code>{1}</code>, +{2}]\n<b>Био:</b> {3}",
-    'en': "👩🏽‍💻 <b>Account:</b> {0}\n[<b>id</b>=<code>{1}</code>, +{2}]\n<b>Bio:</b> {3}",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_info_confident = {
-    'ru': "\n\n<b>Конфиденциальность:</b>\n{0}",
-    'en': "\n\n<b>Confidentiality:</b>\n{0}",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_info_status = {
-    'ru': "{0}-<i>эмоджи-статус</i>",
-    'en': "{0}-<i>status in emoji</i>",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_info_premium = {
-    'ru': "\n<b>Премиум:</b> {0}",
-    'en': "\n<b>Premium:</b> {0}",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_info_fake = {
-    'ru': "\n<b>Фейк:</b> да",
-    'en': "\n<b>Fake:</b> да",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_info_scam = {
-    'ru': "\n<b>Скам:</b> да",
-    'en': "\n<b>Scam:</b> да",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_info_restricted = {
-    'ru': "\n<b>Ограничен:</b> да",
-    'en': "\n<b>Restrected:</b> да",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-
-l_bot_cmd_nsfw = {
-    'ru': "<b>NSFW (небезопасный контент):</b> ",
-    'en': "<b>NSFW (not safe for work content):</b> ",
-    'es': "🗣 Presiona ✅/☑️ para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👩🏽‍💻 Por ejemplo, <i>Usuario se unió al grupo</i>",
-    'fr': "🗣 Appuyez sur ✅/☑️ pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👩🏽‍💻 Par exemple, <i>L'utilisateur a rejoint le bote</i>",
-    'zh': "🗣 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👩🏽‍💻 例如，<i>用戶加入群組</i>",
-    'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👩🏽‍💻 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
-}
-l_bot_cmd_auto_archive = {
-    'ru': "<b>Авто-архив spam-пользователей:</b> ",
-    'en': "<b>Auto-archive spam-users:</b> ",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_cloud_pswd = {
-    'ru': "<b>Облачный пароль</b>: <code>{0}</code>",
-    'en': "<b>Cloud password</b>: <code>{0}</code>",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_profile_photo = {
-    'ru': "\n<b>Фото профиля</b>: {0}",
-    'en': "\n<b>Profile photo</b>: {0}",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_common_chats = {
-    'ru': "\n<b>Общие чаты:</b> {0}",
-    'en': "\n<b>Common groups:</b> {0}",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_lang = {
-    'ru': "\n<b>Язык</b>: <code>{0}</code>",
-    'en': "\n<b>Language</b>: <code>{0}</code>",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_react = {
-    'ru': "\n<b>Стандарт-реакции:</b> <code>{0}</code>",
-    'en': "\n<b>Standart-reactions:</b> <code>{0}</code>",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_gif_mask = {
-    'ru': "\n<b>Сохраненные гиф/маски:</b> <code>{0}/{1}</code>",
-    'en': "\n<b>Saved giff/masks:</b> <code>{0}/{1}</code>",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_theme_wall = {
-    'ru': "\n<b>Темы/Обои:</b> <code>{0}/{1}</code> {2}",
-    'en': "\n<b>Themes/Walls:</b> <code>{0}/{1}</code> {2}",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_sick_emoj = {
-    'ru': "\n<b>Stickers/Emoji</b>: <code>{0}/{1}</code>{2}",
-    'en': "",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_bot = {
-    'ru': "\n\n<b>Бот:</b> @{0} ({1})",
-    'en': "\n\n<b>Bot:</b> @{0} ({1})",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_chn = {
-    'ru': "\n\n<b>Канал:</b> @{0} ({1})",
-    'en': "\n\n<b>Channel:</b> @{0} ({1})",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_bot_chn = {
-    'ru': "\n<i>[бот и публичный канал необходимы для работы со сложными постами]</i>",
-    'en': "\n<i>[bot & public channel are needed to work with complex posts]</i>",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_cmds = {
-    'ru': "\n\n⚙️ <b>Команды</b> /cmd",
-    'en': "\n\n⚙️ <b>Commands</b> /cmd",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_top_send = {
-    'ru': "\n@{0} написал(а): {1} сообщ",
-    'en': "\n@{0} write: {1} messages",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_top_users = {
-    'ru': "<b>\n\n👩🏽‍💻 Топ пользователей (на 1000 сообщ)</b>: {0}\n",
-    'en': "<b>\n\n👩🏽‍💻 Top users (for 1000 msgs)</b>: {0}\n",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_top_words = {
-    'ru': "\n{0}. <i>{1}</i>..: встретилось {2} раз",
-    'en': "\n{0}. <i>{1}</i>..: meeting {2} times",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_top_msgs = {
-    'ru': "<b>\n👩🏽‍💻 Топ сообщ (из 1000)</b>: {0}\n",
-    'en': "<b>\n👩🏽‍💻 Top messages (from 1000)</b>: {0}\n",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_fld_fave = {
-    'ru': "избранное",
-    'en': "favor",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_fld_users = {
-    'ru': "пользователи",
-    'en': "users",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_fld_chns = {
-    'ru': "каналы",
-    'en': "channels",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_fld_grps = {
-    'ru': "группы",
-    'en': "groups",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_fld_bots = {
-    'ru': "боты",
-    'en': "bots",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_life_time = {
-    'ru': "\n\n<b>Время жизни бота:</b> ~{0} дней",
-    'en': "\n\n<b>Lifetime of bot:</b> ~{0} days",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_first_dlg = {
-    'ru': "\n\n<b>Дата первого диалога:</b> ~{0} days",
-    'en': "\n\n<b>Datetime of first dialog:</b> ~{0}",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_first_karma = {
-    'ru': "\n<b>Карма:</b> <code>{0}</code> /spambot",
-    'en': "\n<b>Karma:</b> <code>{0}</code> /spambot",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_authorizations = {
-    'ru': "\n<b>Авторизации:</b> <code>{0}</code>\n{1}",
-    'en': "\n<b>Authorization:</b> <code>{0}</code>\n{1}",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_current_auth = {
-    'ru': "текущая",
-    'en': "current",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_flds = {
-    'ru': "\n<b>Папки</b>: <code>{0}</code>\n{1}",
-    'en': "\n<b>Folders</b>: <code>{0}</code>\n{1}",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_ring = {
-    'ru': "\n<b>Рингтоны:</b> <code>{0}</code>",
-    'en': "\n<b>Ringtones:</b> <code>{0}</code>",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_black = {
-    'ru': "\n<b>Черный список</b>: <code>{0}</code>",
-    'en': "\n<b>Black list</b>: <code>{0}</code>",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_notify = {
-    'ru': "\n<b>Особые уведомления:</b> {0}",
-    'en': "\n<b>Special notifications:</b> {0}",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_drafts = {
-    'ru': "\n<b>Черновики/помеченные:</b> <code>{0}/{1}</code>",
-    'en': "\n<b>Drafts/unread:</b> <code>{0}/{1}</code>",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_sched = {
-    'ru': "\n<b>Отложенные/посты/офферы</b>: {0}",
-    'en': "\n<b>Scheduled/posts/offers</b>: {0}",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_dlgs = {
-    'ru': "\n<b>Диалоги</b> <u>архив/закреп/все</u>: {0}",
-    'en': "\n<b>Dialogs</b> <u>archive/pin/all</u>: {0}",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_last_react = {
-    'ru': "\n<b>Последние реакции:</b> {0}",
-    'en': "\n<b>Last reactions:</b> {0}",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_unread_react = {
-    'ru': "\n<b>Непрочитанные @тэги/реакции:</b> <code>{0}/{1}</code>",
-    'en': "\n<b>Unread @tags/reactions:</b> <code>{0}/{1}</code>",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_unread_msgs = {
-    'ru': "\n<b>Непрочитанные сообщ (и архив):</b> <code>{0}</code>",
-    'en': "\n<b>Unread messages (& archive):</b> <code>{0}</code>",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_contacts = {
-    'ru': "\n<b>Контакты</b> <u>взаимные/недавние/все</u>: {0}",
-    'en': "\n<b>Contacts</b> <u>mutual/recent/all</u>: {0}",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_all = {
-    'ru': "\n<b>Пользователи/боты/группы/каналы</b>: {0}",
-    'en': "\n<b>Users/bots/groups/channels</b>: {0}",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_owner = {
-    'ru': "\n\n<b>Владелец</b> <u>групп/каналов</u>: <code>{0}</code>\n{1}",
-    'en': "\n\n<b>Owner</b> of <u>groups/channels</u>: <code>{0}</code>\n{1}",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_admin = {
-    'ru': "\n\n<b>Админ</b> <u>групп/каналов</u>: <code>{0}</code>\n{1}",
-    'en': "\n\n<b>Admin</b> of <u>groups/channels</u>: <code>{0}</code>\n{1}",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_bot_father = {
-    'ru': "\n\n<b>Боты {0}</b>: <code>{1}/20</code>\n{2}",
-    'en': "\n\n<b>Bots {0}</b>: <code>{1}/20</code>\n{2}",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_top_affects = {
-    'ru': "\n\n<b>Топ взаимодействий</b>:\n{0}",
-    'en': "\n\n<b>Top interactions</b>:\n{0}",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_last_msgs = {
-    'ru': "\n\n<b>Последние сообщения</b>:\n{0}",
-    'en': "\n\n<b>Last messages</b>:\n{0}",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_parse_fun = {
-    'ru': "🔥 Готово! Для <b>{0}</b> собрано реальных <b>{1}</b>-участников: <u>{2}</u>{3}\n\n👩🏽‍💻 Для рассылки и инвайта можно использовать @ferey_send_bot",
-    'en': "🔥 Ready! For <b>{0}</b> gathered of real <b>{1}</b>-members: <u>{2}</u>{3}\n\n👩🏽‍💻 For sending and invite use @ferey_send_bot",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_parse_handler_err = {
-    'ru': "👩🏽‍💻 Вставь корректную ссылку, повтори операцию или попробуй вступить вручную",
-    'en': "👩🏽‍💻 Enter correct link, repeat operation or try join manual",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-
-l_bot_cmd_update_err = {
-    'ru': "👩🏽‍💻 Ошибка обновления профиля",
-    'en': "👩🏽‍💻 Update profile error",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_update_info = {
-    'ru': "👩🏽‍💻 Ошибка получения профиля",
-    'en': "👩🏽‍💻 Getting profile error",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_update_stat = {
-    'ru': "👩🏽‍💻 Ошибка получения статистики",
-    'en': "👩🏽‍💻 Getting statistics error",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-l_bot_cmd_geo_fun = {
-    'ru': "🔥 Готово! По геопозиции <b>{0} {1}</b> собрано реальных участников: <u>{2}</u>\n\n👩🏽‍💻 Для рассылки и инвайта можно использовать @ferey_send_bot",
-    'en': "🔥 Ready! By geo-location <b>{0} {1}</b> gathered real of members: <u>{2}</u>\n\n👩🏽‍💻 For sending and invite use @ferey_send_bot",
-    'es': "",
-    'fr': "",
-    'zh': "",
-    'ar': "",
-}
-
 l_idea = {
     'ru': "💡 Идея!",
     'en': "💡 Idea!",
     'es': "🔙 Volver..",
     'fr': "🔙 Retour..",
     'zh': "🔙 回來..",
     'ar': "🔙 رجوع ..",
@@ -7399,153 +6939,14 @@
     'zh': "🔙 回來..",
     'ar': "🔙 رجوع ..",
 }
 # endregion
 
 
 # region extra bot
-l_markup_check_list = {
-    'ru': "📕 Чек-лист",
-    'en': "📕 Check-list",
-    'es': '🌬 Sobre',
-    'fr': '🌬 À propos de',
-    'zh': '🌬 關於',
-    'ar': '🌬 حول',
-}
-l_markup_check_contact = {
-    'ru': "☎️ Контакт",
-    'en': "☎️ Contact",
-    'es': '🌬 Sobre',
-    'fr': '🌬 À propos de',
-    'zh': '🌬 關於',
-    'ar': '🌬 حول',
-}
-l_markup_check_gift = {
-    'ru': "🎁 Подарок",
-    'en': "🎁 Present",
-    'es': '🌬 Sobre',
-    'fr': '🌬 À propos de',
-    'zh': '🌬 關於',
-    'ar': '🌬 حول',
-}
-l_markup_check_blog = {
-    'ru': "📰 Блог",
-    'en': "📰 Blog",
-    'es': '🌬 Sobre',
-    'fr': '🌬 À propos de',
-    'zh': '🌬 關於',
-    'ar': '🌬 حول',
-}
-
-l_bot_block = {
-    'ru': "👩🏽‍💻 <b>Пользователь</b> #<u>{0}</u>: {1} заблокировал @{2}-бота",
-    'en': "👩🏽‍💻 User <b>{0}</b> have blocked @{1}-bot",
-    'es': '🌬 Sobre',
-    'fr': '🌬 À propos de',
-    'zh': '🌬 關於',
-    'ar': '🌬 حول',
-}
-l_bot_unblock = {
-    'ru': "👩🏽‍💻 <b>Пользователь</b> #<u>{0}</u>: {1} разблокировал @{2}-бота",
-    'en': "👩🏽‍💻 User <b>{0}</b> unblock @{1}-bot",
-    'es': '🌬 Sobre',
-    'fr': '🌬 À propos de',
-    'zh': '🌬 關於',
-    'ar': '🌬 حول',
-}
-l_bot_answer = {
-    'ru': "👩🏽‍💻 <b>Пользователь<b>: {0} [<b>id</b>=<code>{1}</code>] ответил в @{2}-боте:",
-    'en': "👩🏽‍💻 User <b>{0}</b> (<code>{1}</code>) have answered into @{2}-bot:",
-    'es': '🌬 Sobre',
-    'fr': '🌬 À propos de',
-    'zh': '🌬 關於',
-    'ar': '🌬 حول',
-}
-l_bot_gift_choose = {
-    'ru': "👩🏽‍💻 <b>Пользователь</b>: {0} [<b>id</b>=<code>{1}</code>] выбрал [{2}] в @{3}-боте",
-    'en': "👩🏽‍💻 User {0} (<code>{1}</code>) choose [{2}] in @{3}-bot",
-    'es': '🌬 Sobre',
-    'fr': '🌬 À propos de',
-    'zh': '🌬 關於',
-    'ar': '🌬 حول',
-}
-l_bot_notify = {
-    'ru': "👩🏽‍💻 <b>Пользователь</b> (<u>{0}</u>): {1} [<b>id</b>=<code>{2}</code>] запустил @{3}-бота <b>{4}</b>",
-    'en': "👩🏽‍💻 User ({0}) {1} (<code>{2}</code>) start @{3}-bot <b>{4}</b>",
-    'es': "🔙 Volver..",
-    'fr': "🔙 Retour..",
-    'zh': "🔙 回來..",
-    'ar': "🔙 رجوع ..",
-}
-
-l_extra_bot_gift_handler = {
-    'ru': "🎁 <b>Разломи</b> одну из печенек, чтобы открыть свой бонус",
-    'en': "🎁 <b>Break</b> one of cookies to get your present",
-    'es': '🌬 Sobre',
-    'fr': '🌬 À propos de',
-    'zh': '🌬 關於',
-    'ar': '🌬 حول',
-}
-l_extra_bot_my_blog = {
-    'ru': "📑 <b> Мой блог</b>",
-    'en': "📑 My Blog",
-    'es': '🌬 Sobre',
-    'fr': '🌬 À propos de',
-    'zh': '🌬 關於',
-    'ar': '🌬 حول',
-}
-l_extra_bot_start = {
-    'ru': "👩🏽‍💻 <b>{0}</b>, добро пожаловать в <i>лендинг-бот</i> @{1}:\n\n▪️сбор ЦА и <b>рассылка</b> оффера\n▪️<b>публикация</b> постов через бота\n▪️ведение <b>telegraph</b>-блога\n▪️проведение <b>опросов</b> и квизов\n\n👩🏽‍💻 Больше возможностей в <a href='https://t.me/{2}'>demo</a>-боте",
-    'en': "👩🏽‍💻 <b>{0}</b>, welcome to <i>landing-bot</i> @{1}:\n\n▪️collect target users & <b>offer sending</b>\n▪️<b>post</b> publication via bot\n▪️<b>telegraph</b>-blog control\n▪️carry out <b>polls & quizes</b>\n\n👩🏽‍💻 More oportunities in <a href='https://t.me/{2}'>demo</a>-bot",
-    'es': '🌬 Sobre',
-    'fr': '🌬 À propos de',
-    'zh': '🌬 關於',
-    'ar': '🌬 حول',
-}
-l_extra_bot_option = {
-    'ru': "👇🏼 <b>Выбери</b> опцию ниже",
-    'en': "👇🏽 <b>Choose</b> direction",
-    'es': '🌬 Sobre',
-    'fr': '🌬 À propos de',
-    'zh': '🌬 關於',
-    'ar': '🌬 حول',
-}
-l_extra_bot_gift1 = {
-    'ru': "3️⃣ Активирован <b>промокод</b> на <b>3%-скидку</b>",
-    'en': "3️⃣ 3%-discount <b>promo-code</b> is activated",
-    'es': '🌬 Sobre',
-    'fr': '🌬 À propos de',
-    'zh': '🌬 關於',
-    'ar': '🌬 حول',
-}
-l_extra_bot_gift2 = {
-    'ru': "7️⃣ Активирован <b>промокод</b> на <b>7%-скидку</b>",
-    'en': "7️⃣ 7%-discount <b>promo-code</b> is activated",
-    'es': '🌬 Sobre',
-    'fr': '🌬 À propos de',
-    'zh': '🌬 關於',
-    'ar': '🌬 حول',
-}
-l_extra_bot_gift3 = {
-    'ru': "🎁 Запись на безоплатную <b>консультацию</b>",
-    'en': "🎁 Record to free <b>consultation</b>",
-    'es': '🌬 Sobre',
-    'fr': '🌬 À propos de',
-    'zh': '🌬 關於',
-    'ar': '🌬 حول',
-}
-l_extra_bot_gift_no = {
-    'ru': "😔 <b>Здесь</b> пусто",
-    'en': "😔 <b>Here</b> is empty",
-    'es': '🌬 Sobre',
-    'fr': '🌬 À propos de',
-    'zh': '🌬 關於',
-    'ar': '🌬 حول',
-}
-
 l_show_admin_panel_md = {
     'ru': "*👩🏽‍💻 Создание и редактирование блога*\n\n👩🏽‍💻 Вы зашли как *Администратор* и можете создавать и редактировать блоги, но не удалять их\n\n¹ Авторизация по ссылке в браузере:\n`{0}`\n\n² Перейди (в течение 10сек) по нужной ссылке для редактирования публикации (жми, чтобы скопировать):\n\n",
     'en': "<b>👩🏽‍💻 Blog-publication creating & editing</b>\n\n👩🏽‍💻 You entered as <b>Administrator</b> - you can create and edit blog-publication, but not to delete them\n\n - Push the button [👩🏽‍💻 Authorization] (it has short lifetime)\n2 - Then: click on the nessesary link (for copy) to open it on a browser for editing:\n\n",
     'es': "🔙 Volver..",
     'fr': "🔙 Retour..",
     'zh': "🔙 回來..",
     'ar': "🔙 رجوع ..",
@@ -7555,130 +6956,26 @@
     'en': "<b>👩🏽‍💻 Blog-publication creating & editing</b>\n\n👩🏽‍💻 You entered as <b>Administrator</b> - you can create and edit blog-publication, but not to delete them\n\n - Push the button [👩🏽‍💻 Authorization] (it has short lifetime)\n2 - Then: click on the nessesary link (for copy) to open it on a browser for editing:\n\n",
     'es': "🔙 Volver..",
     'fr': "🔙 Retour..",
     'zh': "🔙 回來..",
     'ar': "🔙 رجوع ..",
 }
 l_show_admin_panel_create = {
-    'ru': "🆕 Создать публикацию",
+    'ru': "🆕 Создать",
     'en': "🆕 Create publication",
     'es': "🔙 Volver..",
     'fr': "🔙 Retour..",
     'zh': "🔙 回來..",
     'ar': "🔙 رجوع ..",
 }
 l_show_admin_panel_auth = {
     'ru': "👩🏽‍💻 Авторизация",
     'en': "👩🏽‍💻 Authorization",
     'es': "🔙 Volver..",
     'fr': "🔙 Retour..",
     'zh': "🔙 回來..",
     'ar': "🔙 رجوع ..",
 }
-l_broadcast_send = {
-    'ru': "🏁 <b>Рассылка</b> завершена\n\n🗝️ число пользователей, получивших сообщение: <u>{0}</u>",
-    'en': "🏁 <b>Sending</b> is finished\n\n🗝️ User count of getting message: <u>{0}</u>",
-    'es': "🔙 Volver..",
-    'fr': "🔙 Retour..",
-    'zh': "🔙 回來..",
-    'ar': "🔙 رجوع ..",
-}
-l_get_default_link = {
-    'ru': "🤳🏽 Связаться",
-    'en': "🤳🏽 Connect",
-    'es': "🔙 Volver..",
-    'fr': "🔙 Retour..",
-    'zh': "🔙 回來..",
-    'ar': "🔙 رجوع ..",
-}
-l_get_default_share = {
-    'ru': "🔗 Поделиться",
-    'en': "🔗 Share",
-    'es': "🔙 Volver..",
-    'fr': "🔙 Retour..",
-    'zh': "🔙 回來..",
-    'ar': "🔙 رجوع ..",
-}
-l_get_default_channel = {
-    'ru': "🎥 Канал",
-    'en': "🎥 Channel",
-    'es': "🔙 Volver..",
-    'fr': "🔙 Retour..",
-    'zh': "🔙 回來..",
-    'ar': "🔙 رجوع ..",
-}
-l_get_default_blog = {
-    'ru': "📰 Блог",
-    'en': "📰 Blog",
-    'es': "🔙 Volver..",
-    'fr': "🔙 Retour..",
-    'zh': "🔙 回來..",
-    'ar': "🔙 رجوع ..",
-}
-l_contact_handler = {
-    'ru': "☎️ Получен <b>контакт</b>: {0}",
-    'en': "☎️ Getting <b>contact</b>: {0}",
-    'es': "🔙 Volver..",
-    'fr': "🔙 Retour..",
-    'zh': "🔙 回來..",
-    'ar': "🔙 رجوع ..",
-}
-l_handler_3127 = {
-    'ru': "👩🏽‍💻 Активирован <b>промокод</b> на 5%-скидку",
-    'en': "👩🏽‍💻 5%-discount <b>promo-code</b> is activated",
-    'es': "🔙 Volver..",
-    'fr': "🔙 Retour..",
-    'zh': "🔙 回來..",
-    'ar': "🔙 رجوع ..",
-}
-l_handler_3127_admin = {
-    'ru': "👩🏽‍💻 <b>Пользователь</b>: {0} [<b>id</b>=<code>{1}</code>] активировал <b>промокод</b> на 5% в @{2}-боте",
-    'en': "👩🏽‍💻 User: <b>{0}</b> (<b>id</b>=<code>{1}</code>) activate <b>promo-code</b> on 5% in @{2}-bot",
-    'es': "🔙 Volver..",
-    'fr': "🔙 Retour..",
-    'zh': "🔙 回來..",
-    'ar': "🔙 رجوع ..",
-}
-l_poll_explanation = {
-    'ru': "ℹ️ Следует держать руку на пульсе!",
-    'en': "ℹ️ You should have the pulse sense!",
-    'es': "🔙 Volver..",
-    'fr': "🔙 Retour..",
-    'zh': "🔙 回來..",
-    'ar': "🔙 رجوع ..",
-}
-l_poll_question = {
-    'ru': "💣 Лучшие инструменты продвижения в Telegram?\n\n*прими решение за 30 секунд",
-    'en': "💣 Best Telegram tools?\n\n*think no more than 30 seconds",
-    'es': "🔙 Volver..",
-    'fr': "🔙 Retour..",
-    'zh': "🔙 回來..",
-    'ar': "🔙 رجوع ..",
-}
-l_poll_option1 = {
-    'ru': "🇺🇸 Трансляция экспертности в блог/канал/группу",
-    'en': "🇺🇸 Expert translation into blog/channel/group",
-    'es': "🔙 Volver..",
-    'fr': "🔙 Retour..",
-    'zh': "🔙 回來..",
-    'ar': "🔙 رجوع ..",
-}
-l_poll_option2 = {
-    'ru': "🇺🎥 Использование ботов/веб-ботов/юзер-ботов",
-    'en': "🇺🎥 Using bots/web-bots/user-bots",
-    'es': "🔙 Volver..",
-    'fr': "🔙 Retour..",
-    'zh': "🔙 回來..",
-    'ar': "🔙 رجوع ..",
-}
-l_poll_option3 = {
-    'ru': "🇺📄 Все вышеперечисленное в одной экосистеме",
-    'en': "🇺📄 All of them in the one eco-system",
-    'es': "🔙 Volver..",
-    'fr': "🔙 Retour..",
-    'zh': "🔙 回來..",
-    'ar': "🔙 رجوع ..",
-}
 # endregion
 
 
 # endregion
```

### Comparing `yeref-0.1.65/yeref/yeref.py` & `yeref-0.1.66/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
 markupAdmin = types.ReplyKeyboardMarkup(keyboard=[
     [types.KeyboardButton(text='⬅️ Prev'), types.KeyboardButton(text='↩️ Menu'),
      types.KeyboardButton(text='➡️️ Next')]], resize_keyboard=True, selective=True, row_width=3)
 
 BOT_VARS_ = '{"DATE_TIME": 0, "BOT_PROMO": "#911", "BOT_CHANNEL": 0, "BOT_CHANNELTID": 0, "BOT_GROUP": 0, "BOT_GROUPTID": 0, "BOT_TZ": 0}'
 BOT_LSTS_ = '{"ADMIN_USERS": [], "PREMIUM_USERS": [], "CHANNEL_USERS": [], "GROUP_USERS": [], "PROMO_USERS": [], "UTM_USERS": []}'
-USER_VARS_ = '{"USER_TEXT": "", "USER_PHONE": "", "USER_GEO": "", "USER_PROMO": "", "USER_QUIZ": 0, "USER_DICE": 0, "USER_PAY": 0, "USER_UTM": "", "USER_ID": 0, "USER_TZ": 0, "USER_LZ": "", "USER_DT": "", "USER_ISADMIN": 0, "USER_ISPREMIUM": 0, "USER_BALL": 0, "USER_RAND": 0, "DATE_TIME": 0}'
+USER_VARS_ = '{"USER_TEXT": "", "USER_PHONE": "", "USER_GEO": "", "USER_PROMO": "", "USER_QUIZ": 0, "USER_DICE": 0, "USER_PAY": 0, "USER_UTM": "", "USER_ID": 0, "USER_TZ": 0, "USER_LC": "", "USER_DT": "", "USER_ISADMIN": 0, "USER_ISPREMIUM": 0, "USER_BALL": 0, "USER_RAND": 0, "DATE_TIME": 0}'
 USER_LSTS_ = '{"USER_UTMREF": []}'
 # endregion
 
 
 # region db
 def sqlite_lower(value_):
     return value_.lower() if value_ else None
```

