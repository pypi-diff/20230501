# Comparing `tmp/yeref-0.1.49.tar.gz` & `tmp/yeref-0.1.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.49.tar", last modified: Sat Apr 29 17:08:29 2023, max compression
+gzip compressed data, was "yeref-0.1.50.tar", last modified: Mon May  1 08:43:57 2023, max compression
```

## Comparing `yeref-0.1.49.tar` & `yeref-0.1.50.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-29 17:08:29.005755 yeref-0.1.49/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-29 17:08:29.005979 yeref-0.1.49/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-29 17:08:29.007532 yeref-0.1.49/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1154 2023-04-29 17:08:10.000000 yeref-0.1.49/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-29 17:08:28.998571 yeref-0.1.49/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.49/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   252620 2023-04-29 16:47:57.000000 yeref-0.1.49/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   192928 2023-04-28 18:02:08.000000 yeref-0.1.49/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-29 17:08:29.005228 yeref-0.1.49/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-29 17:08:28.000000 yeref-0.1.49/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-04-29 17:08:28.000000 yeref-0.1.49/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-29 17:08:28.000000 yeref-0.1.49/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-29 17:08:28.000000 yeref-0.1.49/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-01 08:43:57.700813 yeref-0.1.50/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-01 08:43:57.701054 yeref-0.1.50/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-01 08:43:57.701989 yeref-0.1.50/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1154 2023-05-01 08:43:36.000000 yeref-0.1.50/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-01 08:43:57.693487 yeref-0.1.50/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.50/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   416973 2023-05-01 08:16:24.000000 yeref-0.1.50/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   194265 2023-05-01 08:41:44.000000 yeref-0.1.50/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-01 08:43:57.700129 yeref-0.1.50/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-01 08:43:57.000000 yeref-0.1.50/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-01 08:43:57.000000 yeref-0.1.50/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-01 08:43:57.000000 yeref-0.1.50/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-01 08:43:57.000000 yeref-0.1.50/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.49/setup.py` & `yeref-0.1.50/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.49',
+      version='0.1.50',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -39,10 +39,10 @@
 # python setup.py bdist_wheel
 # endregion
 
 # python -m build
 
 # twine upload dist/*
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.48-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.50-py3-none-any.whl
 
 # python3 -m pip install --upgrade yeref
```

### Comparing `yeref-0.1.49/yeref/l_.py` & `yeref-0.1.50/yeref/l_.py`

 * *Files 24% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     'en': "👩🏽‍💻 No, 0%",
     'es': "👩🏽‍💻 No, 0%",
     'fr': "👩🏽‍💻 Non, 0%",
     'zh': "👩🏽‍💻 没有，0%",
     'ar': "👩🏽‍💻 لا ، 0٪",
 }
 l_creturn_text = {
-    'ru': "✖️ <b>Сбросить</b> настройки по умолчанию (до рекомендуемых) для канала [<b>{0}</b>]?",
+    'ru': "✖️ <b>Сбросить</b> настройки по умолчанию (до рекомендуемых) для [<b>{0}</b>]?",
     'en': "✖️ Reset default settings (recommended) for channel [<b>{0}</b>]?",
     'es': "✖️ ¿Restablecer la configuración predeterminada (recomendado) para el canal [<b>{0}</b>]?",
     'fr': "✖️ Réinitialiser les paramètres par défaut (recommandé) pour la chaîne [<b>{0}</b>] ?",
     'zh': "✖️ 重置频道 [<b>{0}</b>] 的默认设置（推荐）？",
     'ar': "✖️ إعادة تعيين الإعدادات الافتراضية (مستحسن) للقناة [<b>{0}</b>]؟",
 }
 l_all_ans = {
@@ -2379,30 +2379,14 @@
     'ru': "<b>Охват</b>: <u>{0}</u> польз.",
     'en': "<b>Reach</b> : <u>{0}</u> users",
     'es': "<b>Alcance</b> : <u>{0}</u> usuarios",
     'fr': "<b>Atteignez</b> : <u>{0}</u> utilisateurs",
     'zh': "<b>覆盖</b>： <u>{0}</u>个用户",
     'ar': "<b>الوصول</b> : <u>{0}</u> مستخدمين",
 }
-l_parse_btnsend = {
-    'ru': "📨️ Рассылка",
-    'en': "📨️ Newsletter",
-    'es': "📨️ Boletín",
-    'fr': "📨️ Newsletter",
-    'zh': "📨️ 时事通讯",
-    'ar': "📨️ النشرة الإخبارية",
-}
-l_parse_btninvite = {
-    'ru': "🚶🏽 Инвайт",
-    'en': "🚶🏽 Invite",
-    'es': "🚶🏽 invitar",
-    'fr': "🚶🏽 Inviter",
-    'zh': "🚶🏽邀请",
-    'ar': "🚶🏽 دعوة",
-}
 l_find_watch = {
     'ru': "🔎 Просмотр",
     'en': "🔎 View",
     'es': "🔎 Ver",
     'fr': "🔎 Voir",
     'zh': "🔎 查看",
     'ar': "🔎 عرض",
@@ -2737,23 +2721,23 @@
     'en': "➕ Add channel",
     'es': "➕ Agregar grupo",
     'fr': "➕ Ajouter un channele",
     'zh': "➕ 添加組",
     'ar': "➕ إضافة مجموعة",
 }
 l_bot_removed = {
-    'ru': "🚫 @{0}-бот удален из канала <b>{1}</b> (<code>{2}</code>)",
-    'en': "🚫 @{0}-бот удален из канала {1} (<code>{2}</code>)",
+    'ru': "🚫 @{0}-бот удален из <b>{1}</b> (<code>{2}</code>)",
+    'en': "🚫 @{0}-бот удален из {1} (<code>{2}</code>)",
     'es': "➕ Agregar grupo",
     'fr': "➕ Ajouter un channele",
     'zh': "➕ 添加組",
     'ar': "➕ إضافة مجموعة",
 }
 
-l_msgConfig = {
+l_chn_config = {
     ("cban", "🕵🏽", "☑"): {
         'ru': "Авто-бан",
         'en': "Auto-ban",
         'es': "Prohibición automática",
         'fr': "Interdiction automatique",
         'zh': "自動禁止",
         'ar': "حظر تلقائي",
@@ -2836,15 +2820,15 @@
     'en': "⚙️ <b>Choose</b> option for <i>settings</i> /cmd <b>{0}</b> {1}",
     'es': "⚙️ <b>Elegir</b> opción para <i>configuración</i> /cmd <b>{0}</b> {1}",
     'fr': "⚙️ <b>Choisir</b> l'option pour les <i>paramètres</i> /cmd <b>{0}</b> {1}",
     'zh': "⚙️ <i>設置</i> /cmd <b>{0}</b>{1}的<b>選擇</b>選項",
     'ar': "⚙️ <b> اختر </b> خيار <i> الإعدادات </i> /cmd <b>{0}</b>{1}",
 }
 l_chat_join_request_handler = {
-    'ru': "👮🏽 {0}, ты отправил(а) заявку на вступление в канал <b>{1}</b>\n\n👉🏼 Выбери <i>правильный вариант</i> в соответствии с <code>заданием</code> на картинке, чтобы твоя <i>заявка</i> на вступление была <b>одобрена</b>",
+    'ru': "👮🏽 {0}, ты отправил(а) заявку на вступление в <b>{1}</b>\n\n👉🏼 Выбери <i>правильный вариант</i> в соответствии с <code>заданием</code> на картинке, чтобы твоя <i>заявка</i> на вступление была <b>одобрена</b>",
     'en': "👮🏽 {0}, you send join-request to channel <b>{1}</b>\n\n👉🏼 Choose <i>correct option</i> according to the <code>task</code> on picture to Approve your join-<i>request</i>",
     'es': "👮🏽 {0}, envías una solicitud de unión al grupo <b>{1}</b>\n\n👉🏼 Elige la <i>opción correcta</i> según la <code>tarea</code> en la imagen para aprobar su <i>solicitud de unión</i>",
     'fr': "👮🏽 {0}, vous envoyez une demande de participation au channele <b>{1}</b>\n\n👉🏼 Choisissez <i>l'option correcte</i> en fonction de la <code>tâche</code> sur l'image pour approuver votre inscription-<i>demande</i>",
     'zh': "👮🏽 {0}，你發送加入請求到組 <b>{1}</b>\n\n👉🏼 根據<code>task</code>選擇<i>正確的選項</i> 在圖片上批准您的加入-<i>請求</i>",
     'ar': "👮🏽 {0} ، ترسل طلب انضمام إلى المجموعة <b>{1}</b> \n\n👉🏼 اختر <i> الخيار الصحيح </i> وفقًا لـ <code> المهمة </code> على الصورة للموافقة على انضمامك- <i> طلب </i>",
 }
 l_content_types_sub_button = {
@@ -2852,15 +2836,15 @@
     'en': "👮🏽 I subscribed",
     'es': "👮🏽 Me suscribí",
     'fr': "👮🏽 Je me suis abonné",
     'zh': "👮🏽 我訂閱了",
     'ar': "👮🏽 لقد اشتركت",
 }
 l_content_types_subscribe = {
-    'ru': "👮🏽 {0}, подпишись на {1}, чтобы вступить в канал",
+    'ru': "👮🏽 {0}, подпишись на {1}, чтобы твоя заявка на вступление была одобрена",
     'en': "👮🏽 {0}, subscribe on the {1} to join the channel",
     'es': "👮🏽 {0}, suscríbete en {1} para unirte al grupo",
     'fr': "👮🏽 {0}, abonnez-vous sur le {1} pour rejoindre le channele",
     'zh': "👮🏽 {0}，在 {1} 上訂閱以加入群組",
     'ar': "👮🏽 {0} ، اشترك في {1} للانضمام إلى المجموعة",
 }
 l_wait_1_min = {
@@ -2869,55 +2853,55 @@
     'es': "✖️ ¡La configuración de grupo de [<b>{0}</b>] se restableció correctamente!",
     'fr': "✖️ Les paramètres de channele de [<b>{0}</b>] ont été réinitialisés !",
     'zh': "✖️ [<b>{0}</b>] 的群組設置已成功重置！",
     'ar': "✖️ تمت إعادة تعيين إعدادات المجموعة لـ [<b>{0}</b>] بنجاح!",
 }
 
 l_creturn_answer = {
-    'ru': "✖️ Настройки канала [<b>{0}</b>] успешно сброшены!",
+    'ru': "✖️ Настройки для [<b>{0}</b>] успешно сброшены!",
     'en': "✖️ channel settings of [<b>{0}</b>] successfully reset!",
     'es': "✖️ ¡La configuración de grupo de [<b>{0}</b>] se restableció correctamente!",
     'fr': "✖️ Les paramètres de channele de [<b>{0}</b>] ont été réinitialisés !",
     'zh': "✖️ [<b>{0}</b>] 的群組設置已成功重置！",
     'ar': "✖️ تمت إعادة تعيين إعدادات المجموعة لـ [<b>{0}</b>] بنجاح!",
 }
 l_cdelete_text = {
-    'ru': "🚫 Убрать привязку бота к канале [<b>{0}</b>]?",
+    'ru': "🚫 Убрать привязку бота к [<b>{0}</b>]?",
     'en': "🚫 Put away bot-connection with channel [<b>{0}</b>]?",
     'es': "🚫 ¿Eliminar la conexión de bot con el grupo [<b>{0}</b>]?",
     'fr': "🚫 Mettre de côté la connexion au bot avec le channele [<b>{0}</b>] ?",
     'zh': "🚫 放棄與組 [<b>{0}</b>] 的機器人連接？",
     'ar': "🚫 التخلص من اتصال الروبوت بالمجموعة [<b>{0}</b>]؟",
 }
 l_cdelete_answer = {
-    'ru': "🚫 <b>Бот</b> успешно отвязан от канала [<b>{0}</b>] и не числится его в участниках!",
+    'ru': "🚫 <b>Бот</b> успешно отвязан от [<b>{0}</b>] и не числится его в участниках!",
     'en': "🚫 Bot successfully disconnected from channel [<b>{0}</b>] and it is not a member at all!",
     'es': "🚫 ¡El bot se desconectó con éxito del grupo [<b>{0}</b>] y no es miembro en absoluto!",
     'fr': "🚫 Le bot s'est déconnecté avec succès du channele [<b>{0}</b>] et il n'est pas du tout membre !",
     'zh': "🚫 Bot 已成功與群組 [<b>{0}</b>] 斷開連接，並且它根本不是成員！",
     'ar': "🚫 تم قطع اتصال البوت بنجاح بالمجموعة [<b>{0}</b>] وهو ليس عضوًا على الإطلاق!",
 }
 
-l_chn_CCHECKBTNNAME = {
+l_ccheck_btn_name = {
     'ru': "✔ Я человек",
     'en': "✔ I am human",
     'es': "✔ Soy humana",
     'fr': "✔ Je suis humain",
     'zh': "✔ 我是人",
     'ar': "✔ أنا إنسان",
 }
-l_chn_CHELLOTEXT = {
+l_ccheck_hello_txt = {
     'ru': "🌱 {name}, добро пожаловать в нашу <b>канал</b> {title}!",
     'en': "🌱 {name}, welcome to our <b>channel</b> {title}!",
     'es': "🌱 {name}, Bienvenida a nuestro <b>grupo</b> {title}!",
     'fr': "🌱 {name}, bienvenue dans notre <b>channele</b> {title}!",
     'zh': "🌱 {name}, 歡迎加入我們的<b>群</b> {title}!",
     'ar': "🌱 {name} ، مرحبًا بك في <b> مجموعتنا </ b> {title}!"
 }
-l_chn_CCHECKCHANNEL = {
+l_ccheck_add_channel = {
     'ru': "👮🏽 Для <i>проверки подписки</i> необходимо добавить канал командой:\n\n/channel ССЫЛКА НА КАНАЛ",
     'en': "👮🏽 It is necessary add channel for <i>subscribe checking</i> by command:\n\n/channel LINK",
     'es': "👮🏽 Es necesario agregar un canal para <i>comprobar suscripciones</i> mediante el comando:\n\n/channel LINK",
     'fr': "👮🏽 Il est nécessaire d'ajouter un canal pour <i>vérifier l'abonnement</i> par la commande :\n\n/channel LINK",
     'zh': "👮🏽 <i>訂閱檢查</i>需要通過命令添加頻道：\n\n/channel LINK",
     'ar': "👮🏽 من الضروري إضافة قناة لـ <i> فحص الاشتراك </i> بواسطة الأمر: \n\n/channel LINK",
 }
@@ -2928,15 +2912,15 @@
     'ru': "👩🏽‍💻 Данные о канале успешно обновлены:\n\n<b>{0}</b> [<code>{1}</code>]\n{2}\n<i>{3}</i>\n\n⚙️ <b>Команды</b> /cmd",
     'en': "➕ Add channel",
     'es': "➕ Agregar grupo",
     'fr': "➕ Ajouter un channele",
     'zh': "➕ 添加組",
     'ar': "➕ إضافة مجموعة",
 }
-l_commands_handler = {
+l_chn_commands_handler = {
     'ru': "⚙️ <b>Настройка</b> канала <b>{0}</b> {1}\n\n<b>⛏ Admin-команды @{2}</b>\n/update <i>обновление параметров</i>\n/transfer   <i>передача admin-прав</i>\n/info   <i>информация</i>\n/stat   <i>статистика</i>\n/parse  <i>выгрузка базы подписчиков</i>\n/videochat 1 1 <i>анонс видео-трансляции</i>\n/clean  <i>долгая очистка канала от deleted/scam/fake-аккаунтов, а также по 🕵🏽 Авто-бан правилам</i>\n/channel NAME   <i>добавить другой канал для проверки подписки</i>",
     'en': "⚙️ <b>channel</b> settings of <b>{0}</b> {1}\n\n<b>⛏ Admin-commands @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/log   <i>see logs</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-accounts</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from channel for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in channel for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-accounts</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for channel</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
     'es': "⚙️ Configuración de <b>Grupo</b> de <b>{0}</b> {1}\n\n<b>⛏ Comandos de administración @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/log   <i>see logs</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-accounts</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from channel for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in channel for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-accounts</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for channel</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
     'fr': "⚙️ Paramètres de <b>channele</b> de <b>{0}</b> {1}\n\n<b>⛏ Commandes d'administration @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/log   <i>see logs</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-accounts</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from channel for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in channel for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-accounts</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for channel</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
     'zh': "⚙️ <b>組</b>設置 <b>{0}</b> {1}\n\n<b>⛏ 管理員命令 @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/log   <i>see logs</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-accounts</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from channel for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in channel for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-accounts</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for channel</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
     'ar': "⚙️ إعدادات <b> المجموعة </b> الخاصة بـ <b>{0}</b> {1}\n\n<b>⛏ أوامر المسؤول @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/parse  <i>[all|old|premium|active|online]</i>\n/log   <i>see logs</i>\n<code>/parse old</code> - <i>parsing old id-accounts</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from channel for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in channel for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-accounts</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for channel</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
 }
@@ -2984,22 +2968,14 @@
     'ru': "<b>Проверка подписки при вступлении в канал</b>: ",
     'en': "<b>Check subscription to join</b>: ",
     'es': "<b>Verifique la suscripción para unirse</b>:",
     'fr': "<b>Vérifier l'abonnement pour rejoindre</b> :",
     'zh': "<b>檢查訂閱以加入</b>：",
     'ar': "<b> تحقق من الاشتراك للانضمام </b>:",
 }
-l_info_oppforpart = {
-    'ru': "Возможности подписчиков",
-    'en': "Participants opportunities",
-    'es': "Oportunidades de los participantes",
-    'fr': "Opportunités pour les participants",
-    'zh': "參與者機會",
-    'ar': "فرص المشاركين",
-}
 l_info_cmd = {
     'ru': "⚙️ <b>Команды</b> /cmd",
     'en': "Participants opportunities",
     'es': "Oportunidades de los participantes",
     'fr': "Opportunités pour les participants",
     'zh': "參與者機會",
     'ar': "فرص المشاركين",
@@ -3009,70 +2985,22 @@
     'ru': "Изменение профиля канала",
     'en': "Change channel Info",
     'es': "Cambiar información del grupo",
     'fr': "Modifier les informations du channele",
     'zh': "更改組信息",
     'ar': "تغيير معلومات المجموعة",
 }
-l_pin_message = {
-    'ru': "Закрепление сообщений",
-    'en': "Pin Messages",
-    'es': "Mensajes de pines",
-    'fr': "Épingler les messages",
-    'zh': "固定消息",
-    'ar': "تثبيت الرسائل",
-}
-l_add_members = {
-    'ru': "Добавление участников",
-    'en': "Add Members",
-    'es': "Añadir miembros",
-    'fr': "Ajouter des membres",
-    'zh': "添加成員",
-    'ar': "إضافة أعضاء",
-}
-l_embed_links = {
-    'ru': "Предпросмотр ссылок",
-    'en': "Embed links",
-    'es': "Insertar enlaces",
-    'fr': "Intégrer des liens",
-    'zh': "嵌入鏈接",
-    'ar': "روابط التضمين",
-}
 l_send_messages = {
     'ru': "Отправка сообщений",
     'en': "Send Messages",
     'es': "Enviar mensajes",
     'fr': "Envoyer des messages",
     'zh': "發送信息",
     'ar': "إرسل رسائل",
 }
-l_send_media = {
-    'ru': "Отправка фото и видео",
-    'en': "Send Media",
-    'es': "Enviar medios",
-    'fr': "Envoyer le média",
-    'zh': "發送媒體",
-    'ar': "إرسال الوسائط",
-}
-l_send_polls = {
-    'ru': "Отправка опросов",
-    'en': "Send Polls",
-    'es': "Enviar encuestas",
-    'fr': "Envoyer des sondages",
-    'zh': "發送投票",
-    'ar': "إرسال استطلاعات الرأي",
-}
-l_send_stickers = {
-    'ru': "Отправка sticker/giff/via_bot",
-    'en': "Send sticker/giff/via_bot",
-    'es': "apagada",
-    'fr': "à l'arrêt",
-    'zh': "離開",
-    'ar': "إيقاف",
-}
 l_info_reactions = {
     'ru': "Допуск emoji-реакций",
     'en': "Allowed emoji-reactions",
     'es': "Emoji-reacciones permitidas",
     'fr': "Emoji-réactions autorisées",
     'zh': "允許的表情符號反應",
     'ar': "ردود فعل الرموز التعبيرية المسموح بها",
@@ -3081,55 +3009,48 @@
     'ru': "Администраторы",
     'en': "Administrators",
     'es': "Administradoras",
     'fr': "Administratrices",
     'zh': "管理員",
     'ar': "المسؤولين",
 }
-l_info_anonymous_for = {
-    'ru': "Анонимность для",
-    'en': "Anonymous for",
-    'es': "Anónimo para",
-    'fr': "Anonyme pour",
-    'zh': "匿名",
-    'ar': "مجهول لـ",
-}
+
 l_info_invite_admins = {
     'ru': "Приглашение других админов для",
     'en': "Promote admins for",
     'es': "Promocionar administradores para",
     'fr': "Promouvoir les administrateurs pour",
     'zh': "提升管理員為",
     'ar': "قم بترقية المسؤولين لـ",
 }
-l_info_start1 = {
+l_chn_info_start1 = {
     'ru': "ℹ️ <b>Общая информация о канале</b>\n\n<b>Название</b>: {0} [id=<code>{1}</code>, <i>{2} {3}</i>, <u>{4}</u> участ.]{5}{6}{7}",
     'en': "ℹ️ <b>Common info about channel statistics</b>\n\n",
     'es': "ℹ️ <b>Información común sobre las estadísticas del grupo</b>\n\n",
     'fr': "ℹ️ <b>Informations communes sur les statistiques de channele</b>\n\n",
     'zh': "ℹ️ <b>關於組統計的常見信息</b>\n\n",
     'ar': "ℹ️ <b> معلومات عامة حول إحصائيات المجموعة </b> \n\n",
 }
-l_stat_start1 = {
+l_chn_stat_start1 = {
     'ru': "ℹ️ <b>Общая статистика канала</b>\n\n<b>Название</b>: {0} [id=<code>{1}</code>, <i>{2} {3}</i>, <u>{4}</u> участ.]{5}{6}{7}",
     'en': "ℹ️ <b>Common info about channel statistics</b>\n\n",
     'es': "ℹ️ <b>Información común sobre las estadísticas del grupo</b>\n\n",
     'fr': "ℹ️ <b>Informations communes sur les statistiques de channele</b>\n\n",
     'zh': "ℹ️ <b>關於組統計的常見信息</b>\n\n",
     'ar': "ℹ️ <b> معلومات عامة حول إحصائيات المجموعة </b> \n\n",
 }
-l_stat_start2 = {
+l_chn_stat_start2 = {
     'ru': "\n<b>Ссылка</b>: {0}\n<b>Описание</b>: {1}\n<b>Привязанная группа</b>: <code>{2}</code>\n",
     'en': "ℹ️ <b>Common info about channel statistics</b>\n\n",
     'es': "ℹ️ <b>Información común sobre las estadísticas del grupo</b>\n\n",
     'fr': "ℹ️ <b>Informations communes sur les statistiques de channele</b>\n\n",
     'zh': "ℹ️ <b>關於組統計的常見信息</b>\n\n",
     'ar': "ℹ️ <b> معلومات عامة حول إحصائيات المجموعة </b> \n\n",
 }
-l_stat_start3 = {
+l_chn_stat_start3 = {
     'ru': "\n<b>ID последнего поста</b>: {0}\n<b>Посты</b>: {1}\n<b>Реакции</b>: {2}\n<b>Просмотры</b>: {3}\n<b>Комментарии</b>: {4}\n<b>$кэштеги</b>: {5}\n<b>#хэштеги</b>: {6}\n",
     'en': "ℹ️ <b>Common info about channel statistics</b>\n\n",
     'es': "ℹ️ <b>Información común sobre las estadísticas del grupo</b>\n\n",
     'fr': "ℹ️ <b>Informations communes sur les statistiques de channele</b>\n\n",
     'zh': "ℹ️ <b>關於組統計的常見信息</b>\n\n",
     'ar': "ℹ️ <b> معلومات عامة حول إحصائيات المجموعة </b> \n\n",
 }
@@ -3138,48 +3059,32 @@
     'en': "ℹ️ <b>Common info about channel statistics</b>\n\n",
     'es': "ℹ️ <b>Información común sobre las estadísticas del grupo</b>\n\n",
     'fr': "ℹ️ <b>Informations communes sur les statistiques de channele</b>\n\n",
     'zh': "ℹ️ <b>關於組統計的常見信息</b>\n\n",
     'ar': "ℹ️ <b> معلومات عامة حول إحصائيات المجموعة </b> \n\n",
 }
 
-l_stat_top5users = {
-    'ru': "Топ 5 пользователей (на 1000 сообщ)",
-    'en': "Top 5 users (for 1000 msgs)",
-    'es': "Las 5 mejores usuarios (para 1000 msgs)",
-    'fr': "Top 5 des utilisateurs (pour 1000 msgs)",
-    'zh': "前 5 名用戶（1000 條消息）",
-    'ar': "أعلى 5 مستخدمين (لكل 1000 رسالة)",
-}
-l_stat_top5msgs = {
-    'ru': "Топ 5 сообщ (из 1000)",
-    'en': "Top 5 msgs (from 1000)",
-    'es': "Las 5 mejores mensajes (desde 1000)",
-    'fr': "Top 5 des messages (sur 1000)",
-    'zh': "前 5 條消息（來自 1000 條）",
-    'ar': "أهم 5 رسائل (من 1000)",
-}
 l_transfer_start = {
     'ru': "⚠️ Пользователь {0} должен /start-запустить @{1}",
     'en': "⚠️ User {0} have to /start @{1}",
     'es': "⚠️ El usuario {0} debe /iniciar @{1}",
     'fr': "⚠️ L'utilisateur {0} doit /start @{1}",
     'zh': "⚠️ 用戶 {0} 必須 /start @{1}",
     'ar': "⚠️ المستخدم {0} يجب أن يبدأ @{1}",
 }
 l_transfer_admin = {
-    'ru': "⚠️ Пользователь {0} должен быть <b>администратором</b> канала <b>{1}</b>",
+    'ru': "⚠️ Пользователь {0} должен быть <b>администратором</b> в <b>{1}</b>",
     'en': "⚠️ User {0} have to be <b>admin</b> of channel <b>{1}</b>",
     'es': "⚠️ El usuario {0} debe ser <b>administrador</b> del grupo <b>{1}</b>",
     'fr': "⚠️ L'utilisateur {0} doit être <b>admin</b> du channele <b>{1}</b>",
     'zh': "⚠️ 用戶 {0} 必須是組 <b>{1}</b> 的 <b>admin</b>",
     'ar': "⚠️ يجب أن يكون المستخدم {0}<b> مسؤولًا </b> للمجموعة <b>{1}</b>",
 }
 l_transfer_transfer = {
-    'ru': "⚠️ Передать <b>admin</b>-права на канал <b>{0}</b> пользователю {1} в @{2}-боте?",
+    'ru': "⚠️ Передать <b>admin</b>-права на <b>{0}</b> пользователю {1} в @{2}-боте?",
     'en': "⚠️ Are you sure to transfer ownership of channel <b>{0}</b> to user {1} in @{2}?",
     'es': "⚠️ ¿Estás seguro de transferir la propiedad del grupo <b>{0}</b> al usuario {1} en @{2}?",
     'fr': "⚠️ Êtes-vous sûr de transférer la propriété du channele <b>{0}</b> à l'utilisateur {1} dans @{2} ?",
     'zh': "⚠️ 您確定將組 <b>{0}</b> 的所有權轉讓給 @{2} 中的用戶 {1}？",
     'ar': "⚠️ هل أنت متأكد من نقل ملكية المجموعة <b>{0}</b> إلى المستخدم {1} في @{2}؟",
 }
 l_transfer_text = {
@@ -3187,23 +3092,23 @@
     'en': "⚠️ Use /transfer-command in reply user-message to transfer him ownership",
     'es': "⚠️ Use /transfer-command en el mensaje de usuario de respuesta para transferirle la propiedad",
     'fr': "⚠️ Utilisez /transfer-command dans le message utilisateur de réponse pour lui transférer la propriété",
     'zh': "⚠️ 使用 /transfer-command 回复 user-message 轉移他的所有權",
     'ar': "استخدم الأمر transfer-command/ في الرد على رسالة المستخدم لنقل ملكيته",
 }
 l_transfer_done_to = {
-    'ru': "⚠️ <b>Admin</b>-права на канал [<b>{0}</b>] успешно переданы {1}",
+    'ru': "⚠️ <b>Admin</b>-права на [<b>{0}</b>] успешно переданы {1}",
     'en': "⚠️ <b>Admin</b>-privileges for channel [<b>{0}</b>] are successfully transferred to {1}",
     'es': "⚠️ <b>Administrador</b>: los privilegios del grupo [<b>{0}</b>] se transfirieron correctamente a {1}",
     'fr': "⚠️ Les privilèges <b>Admin</b> pour le channele [<b>{0}</b>] ont été transférés avec succès vers {1}",
     'zh': "⚠️ <b>Admin</b>-組 [<b>{0}</b>] 的權限已成功轉移到 {1}",
     'ar': "⚠️ تم نقل امتيازات <b> المسؤول </b> للمجموعة [<b>{0}</b>] بنجاح إلى {1}",
 }
 l_transfer_done_from = {
-    'ru': "⚠️ <b>Admin</b>-права на канал [<b>{0}</b>] успешно получены от {1}",
+    'ru': "⚠️ <b>Admin</b>-права на [<b>{0}</b>] успешно получены от {1}",
     'en': "⚠️ <b>Admin</b>-privileges for channel [<b>{0}</b>] are successfully received from {1}",
     'es': "⚠️ <b>Administrador</b>: los privilegios para el grupo [<b>{0}</b>] se recibieron correctamente de {1}",
     'fr': "⚠️ Les privilèges <b>Admin</b> pour le channele [<b>{0}</b>] ont bien été reçus de {1}",
     'zh': "⚠️ <b>Admin</b>-組 [<b>{0}</b>] 的權限已從 {1} 成功接收",
     'ar': "⚠️ تم استلام امتيازات <b> المسؤول </b> للمجموعة [<b>{0}</b>] بنجاح من {1}",
 }
 l_chn_check = {
@@ -3251,30 +3156,30 @@
     'en': "🎥 Send this command as reply to message",
     'es': "🎥 Enviar este comando como respuesta al mensaje",
     'fr': "🎥 Envoyez cette commande en réponse au message",
     'zh': "🎥 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_ban_users_start = {
-    'ru': "👩🏽‍💻 Начинаем очистку канала\nТекущее количество пользователей в базе: {0}",
+    'ru': "👩🏽‍💻 Начинаем очистку\nТекущее количество пользователей в базе: {0}",
     'en': "🎥 Send this command as reply to message",
     'es': "🎥 Enviar este comando como respuesta al mensaje",
     'fr': "🎥 Envoyez cette commande en réponse au message",
     'zh': "🎥 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
 l_ban_users_stop = {
     'ru': "👩🏽‍💻 Очистка завершена\nТекущее количество пользователей в базе: {0} (-{1})",
     'en': "🎥 Send this command as reply to message",
     'es': "🎥 Enviar este comando como respuesta al mensaje",
     'fr': "🎥 Envoyez cette commande en réponse au message",
     'zh': "🎥 將此命令作為對消息的回復發送",
     'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
 }
-l_ccheck_handler = {
+l_chn_ccheck_handler = {
     'ru': "👮🏽 <b>Жми</b> на ✅/🔘, чтобы <b>переключить</b> тип <i>проверки</i> пользователя при <u>вступлении</u> по сгенерированной ссылке: {0} (только для <code>ЧАСТНЫХ</code> каналов)\n\n👉🏼 Для <b>проверки подписки</b> на другой канал <i>добавь</i> @{1}-бота в канал и выполни команду: <code>/channel {2}</code>\n\n👉🏼 Для <i>защиты от атаки</i> на канал включи режим <b>антирейд</b> (блокировка <u>всех</u> вступающих)",
     'en': "👮🏽 Push the ✅/🔘 to <b>switch</b> <i>Enter control</i> of user <u>joining</u> into channel\n\n👉🏼 To set name of <b>pushing button</b> execute command: <code>/button {0}</code>\n\n👉🏼 To check <b>channel-subscription</b> <i>add</i> @{1} to channel and execute command: <code>/channel {2}</code>\n\n👉🏼 To <i>defend</i> from channel-attack switch <b>anti-raid</b>-mode (ban <u>everyone</u> who joining)",
     'es': "👮🏽 Presiona ✅/🔘 para <b>cambiar</b> <i>Enter control</i> del usuario <u>uniéndose</u> al grupo\n\n👉🏼 Para establecer el nombre de <b> presionando el botón</b> ejecute el comando: <code>/button {0}</code>\n\n👉🏼 Para verificar <b>channel-subscription</b> <i>add</i> @{1} para canalizar y ejecutar el comando: <code>/channel {2}</code>\n\n👉🏼 Para <i>defender</i> del ataque grupal, active el modo <b>anti-raid</b> (prohibir a <u>todos</u> que se unan)",
     'fr': "👮🏽 Appuyez sur ✅/🔘 pour <b>commuter</b> <i>Entrez le contrôle</i> de l'utilisateur <u>rejoignant</u> le channele\n\n👉🏼 Pour définir le nom de <b> en appuyant sur le bouton</b> exécutez la commande : <code>/button {0}</code>\n\n👉🏼 Pour vérifier <b>channel-subscription</b> <i>add</i> @{1} pour canaliser et exécuter la commande : <code>/channel {2}</code>\n\n👉🏼 Pour <i>se défendre</i> contre une attaque de channele, activez le mode <b>anti-raid</b> (bannir <u>tous ceux</u> qui se joignent)",
     'zh': "👮🏽 按下 ✅/🔘 來<b>切換</b> <i>進入控制</i> 用戶<u>加入</u> 入組\n\n👉🏼 設置<b>的名字 按下按鈕</b> 執行命令：<code>/button {0}</code>\n\n👉🏼 檢查<b>頻道訂閱</b> <i>add</i> @{1} 引導並執行命令：<code>/channel {2}</code>\n\n👉🏼 以 <i>defend</i> 免受群攻開啟 <b>anti-raid</b>-mode （禁止加入的<u>每個人</u>）",
     'ar': "👮🏽 ادفع ✅ / 🔘 إلى <b> التبديل </b> <i> أدخل التحكم </i> للمستخدم <u> المنضم </u> إلى مجموعة \n\n👉🏼 لتعيين اسم <b> ضغط الزر </b> نفذ الأمر: <code> / button {0}</code>\n\n👉🏼 للتحقق من <b> اشتراك القناة </b> <i> إضافة </i> @{1} لتوجيه وتنفيذ الأمر: <code> / channel {2}</code>\n\n👉🏼 <i> للدفاع </i> من هجوم المجموعة ، شغّل وضع <b> anti-raid </b> (حظر <u> كل شخص </u> من ينضم)",
 }
@@ -3410,134 +3315,14 @@
     'ru': "🔘️☐Выкл антирейд",
     'en': "🔘️☐Off anti-raid",
     'es': "🔘️☐De anti-raid",
     'fr': "🔘️☐De anti-raid",
     'zh': "🔘️☐禁用反襲擊",
     'ar': "🔘️☐ تعطيل مكافحة الغارة",
 }
-
-l_ccheckconfig_handler = {
-    'ru': "Текущий добавленный канал",
-    'en': "Current added channel",
-    'es': "Canal agregado actual",
-    'fr': "Chaîne actuellement ajoutée",
-    'zh': "當前添加的頻道",
-    'ar': "القناة المضافة الحالية",
-}
-l_ccheckchannel_link = {
-    'ru': "👮🏽 Ссылка на {0} не доступна",
-    'en': "👮🏽 Link for {0} is invalid",
-    'es': "👮🏽 El enlace para {0} no es válido",
-    'fr': "👮🏽 Le lien pour {0} n'est pas valide",
-    'zh': "👮🏽 {0} 的鏈接無效",
-    'ar': "👮🏽 ارتباط {0} غير صالح",
-}
-l_ccheckchannel_chn = {
-    'ru': "👮🏽 Ты не вступил в {0}\n\nПопробуй ещё раз позже",
-    'en': "👮🏽 You are not join to {0}\n\nTry again later",
-    'es': "👮🏽 No te has unido a {0}\n\nInténtalo de nuevo más tarde",
-    'fr': "👮🏽 您沒有加入 {0}\n\n 請稍後再試",
-    'zh': "👮🏽 您沒有加入 {0}\n\n 請稍後再試",
-    'ar': "👮🏽 أنت لست مشتركًا في {0} \n\n حاول مرة أخرى لاحقًا",
-}
-l_ccheck_ban = {
-    'ru': "👮🏽‍ Пользователь <b>{0}</b> не прошел входной контроль",
-    'en': "👮🏽 User {0} did not pass Enter Control and have been deleted from this channel",
-    'es': "👮🏽 El usuario {0} no pasa el control de entrada y ha sido eliminado de este grupo",
-    'fr': "👮🏽 L'utilisateur {0} ne passe pas Enter Control et a été supprimé de ce channele",
-    'zh': "👮🏽 用戶 {0} 未通過 Enter Control 並已從該組中刪除",
-    'ar': "👮🏽 المستخدم {0} لا يجتاز إدخال التحكم وقد تم حذفه من هذه المجموعة",
-}
-
-l_ccheckchannel_error = {
-    'ru': "👮🏽 Ошибка проверки",
-    'en': "👮🏽 Error of checking",
-    'es': "👮🏽 Error de verificación",
-    'fr': "👮🏽 Erreur de vérification",
-    'zh': "👮🏽檢查錯誤",
-    'ar': "👮🏽 خطأ في الفحص",
-}
-l_ccheck_wrong = {
-    'ru': "👮🏽 К сожалению, ответ неверный\n\nПопробуйте ещё раз позже",
-    'en': "👮🏽 Unfortunately the answer is not correct\n\nTry again later",
-    'es': "👮🏽 Lamentablemente la respuesta no es correcta\n\nVuelve a intentarlo más tarde",
-    'fr': "👮🏽 Malheureusement, la réponse n'est pas correcte\n\nRéessayez plus tard",
-    'zh': "👮🏽 很遺憾答案不正確\n\n稍後再試",
-    'ar': "👮🏽 للأسف الإجابة غير صحيحة \n\n حاول مرة أخرى لاحقًا",
-}
-l_ccheck_time = {
-    'ru': "👮🏽 Входной контроль пройден за {0} sec",
-    'en': "👮🏽 Enter Control passed for {0} sec",
-    'es': "👮🏽 Control de entrada superado durante {1} seg.",
-    'fr': "👮🏽 Entrez le contrôle passé pendant {1} sec",
-    'zh': "👮🏽 輸入控制已通過 {1} 秒",
-    'ar': "👮🏽 أدخل التحكم الذي تم تمريره لمدة {1} ثانية",
-}
-
-# endregion
-
-
-# region chello_
-l_chello_your_hello = {
-    'ru': "Ваше приветствие",
-    'en': "Your greeting",
-    'es': "Tu saludo",
-    'fr': "Votre message d'accueil",
-    'zh': "你的問候",
-    'ar': "تحياتك",
-}
-l_chello_text = {
-    'ru': "👋🏽 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> приветствие, а также его ⚙️Настроить\n\n👉🏼 Например, <code>{0}</code>{1}",
-    'en': "👋🏽 Push the ✅/☑️, to <b>On/Off</b> greeting, and to ⚙️Configure\n\n👉🏼 For example, <code>{0}</code>{1}",
-    'es': "👋🏽 Presione ✅/☑️, para <b>Activar/Desactivar</b> el saludo y para ⚙️Configurar\n\n👉🏼 Por ejemplo, <code>{0}</code>{1}",
-    'fr': "👋🏽 Appuyez sur ✅/☑️, sur <b>Activer/Désactiver</b> le message d'accueil et sur ⚙️Configurer\n\n👉🏼 Par exemple, <code>{0}</code>{1}",
-    'zh': "👋🏽 按下 ✅/☑️、<b>On/Off</b> 問候語和 ⚙️Configure\n\n👉🏼 例如，<code>{0}</code>{1}",
-    'ar': "👋🏽 اضغط على ✅ / ☑️ ، من أجل <b> تشغيل / إيقاف </b> الترحيب ، و تكوين \n\n👉🏼 على سبيل المثال ، <code>{0}</code>{1}",
-}
-l_btn_on = {
-    'ru': "✅☑Вкл",
-    'en': "✅☑On",
-    'es': "✅☑En",
-    'fr': "✅☑En",
-    'zh': "✅☑使能夠",
-    'ar': "✅☑ تمكين",
-}
-l_btn_off = {
-    'ru': "☑️☐Выкл",
-    'en': "☑️☐Off",
-    'es': "☑️☐De",
-    'fr': "☑️☐De",
-    'zh': "☑️☐禁用",
-    'ar': "☑️☐ تعطيل",
-}
-l_btn_settings = {
-    'ru': "⚙️Настроить",
-    'en': "⚙️Configure",
-    'es': "⚙️Configurar",
-    'fr': "⚙️Configurer",
-    'zh': "⚙️配置",
-    'ar': "⚙️ تكوين",
-}
-l_chellochange_handler = {
-    'ru': "👋🏽 Отправь мне <b>текст</b>/<b>медиа</b> контент с текстом: фото/гиф/видео/аудио/документ или запиши голосовое/видео-заметку в кружке\n\n👉🏼 Например, <code>{0}</code>",
-    'en': "👋🏽 Send me <b>text</b>/<b>media</b> content with text: photo/giff/video/audio/document or voice/video-note\n\n👉🏼 For example, <code>{0}</code>",
-    'es': "👋🏽 Envíame contenido de <b>texto</b>/<b>medios</b> con texto: photo/giff/video/audio/document or voice/video-note\n\n👉🏼 Par exemple, <code>{0}</code>",
-    'fr': "👋🏽 Envoyez-moi du contenu <b>texte</b>/<b>média</b> avec du texte: photo/giff/video/audio/document or voice/video-note\n\n👉🏼 Par exemple, <code>{0}</code>",
-    'zh': "👋🏽 向我發送帶有文本的 <b>text</b>/<b>media</b> 內容: photo/giff/video/audio/document or voice/video-note\n\n👉🏼 例如, <code>{0}</code>",
-    'ar': "👋🏽 أرسل لي محتوى <b> نصًا </b> / <b> وسائط </b> مع نص: photo/giff/video/audio/document or voice/video-note\n\n👉🏼 فمثلا, <code>{0}</code>",
-}
-l_fsm_hello_finish = {
-    'ru': "👋🏽 Приветствие записано!\n\nОпцию можно включить в настройках [👋🏽Авто-приветствие], нажав [✅☑Вкл]",
-    'en': "👋🏽 Greeting is recorded!\n\nYou can enable this option in the Settings [👋🏽Auto-greeting], by pushing [✅☑On]",
-    'es': "👋🏽 ¡Se graba el saludo!\n\nPuede habilitar esta opción en la Configuración [👋🏽Auto-saludo], presionando [✅☑On]",
-    'fr': "👋🏽 Le message d'accueil est enregistré !\n\nVous pouvez activer cette option dans les paramètres [👋🏽Auto-salutation], en appuyant sur [✅☑On]",
-    'zh': "👋🏽問候語已錄製！\n\n您可以在設置[👋🏽自動問候語]中啟用此選項，方法是按[✅☑On]",
-    'ar': "👋🏽 تم تسجيل الترحيب!\n\n يمكنك تمكين هذا الخيار في الإعدادات [الترحيب التلقائي] ، بالضغط على [تشغيل]",
-}
-
 # endregion
 
 
 # region cban_
 l_cban_handler = {
     'ru': "🕵🏽 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <u>авто</u>-бан <i>аккаунтов с недавно зарегистрированными new-id/без @username/аккаунтов из <a href='https://cas.chat'>Anti-Spam Системы</a>/аккаунтов с 文-глиф, ب-араб, <a href='https://www.zalgo.org'>zalgo-символами</a></i>\n\n👉🏼 Например, опция <b>new-id</b> блокирует аккаунты со <i>свежим</i> <u>id</u>",
     'en': "🕵🏽 Push the ✅/☑️, to <b>On/Off</b> <u>auto</u>-ban <i>accounts with recently registered new-id/deleted-accounts/accounts from <a href='https://cas.chat'>Anti-Spam System</a>/accounts with 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👉🏼 For example, the option <b>deleted-ban</b> delete such accounts: <i>👻 Deleted account [scam,fake]</i>",
@@ -3881,7 +3666,2350 @@
     'fr': "Dans les paramètres [Administrateurs] pour @{0}, activez :\n[✅ Supprimer les messages]\n[✅ Bannir les utilisateurs]\n[✅ Inviter des utilisateurs]\n🕚Attendez 1 minute",
     'zh': "在@{0}的設置[管理員]中打開：\n[✅刪除消息]\n[✅禁止用戶]\n[✅邀請用戶]\n🕚等待1分鐘",
     'ar': " في الإعدادات [Administrators] لـ @{0} شغّل:\n [✅ حذف الرسائل] \n على [✅ حظر المستخدمين] \n [✅ دعوة المستخدمين] \n وانتظر لمدة دقيقة واحدة",
 }
 # endregion
 # endregion
 
+
+# region FereyGroupBot
+l_group_btn1 = {
+    'ru': '⛰️ Группы',
+    'en': "⛰️ VPN",
+    'es': "⛰️VPN",
+    'fr': "⛰️VPN",
+    'zh': "⛰️ VPN",
+    'ar': "⛰️ VPN",
+}
+l_group_btn2 = {
+    'ru': "🌬 Подписка",
+    'en': "🌬 Subscription",
+    'es': "🌬 Suscripción",
+    'fr': "🌬 Abonnement",
+    'zh': "🌬订阅",
+    'ar': "🌬 الاشتراك",
+}
+l_group_welcome = {
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>администрирования</code> <b>Telegram</b>-групп:\n\n▪️<b>защита</b> группы от вступления шпионов\n▪️вывод <b>статистики</b> и вовлеченности (%)\n▪️ограничение прав до <b>подписки</b> на канал\n▪️<b>организация</b> бана и антифлуда\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
+    'en': "🌱 {0}, welcome to <i>the landing bot</i> of the Ferey project:\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
+    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> del proyecto Ferey:\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ también puedes encargar el desarrollo de un chat bot en nuestro estudio Ferey",
+    'fr': "🌱 {0}, bienvenue sur <i>le landing bot</i> du projet Ferey :\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
+    'zh': "🌱 {0}，欢迎来到 Ferey 项目的<i>落地机器人</i>：\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️您也可以在我们的Ferey工作室订购聊天机器人的开发",
+    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> الخاص بمشروع Ferey:\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey",
+}
+l_add_group_text = {
+    'ru': "👇🏽 Жми на ‹➕ Добавить группу›, чтобы добавить в свою группу (с настройками по ум) бота: @{0}\n\n👮🏽‍♀️ Или добавь бота как <b>Administrator</b> через настройки своей группы: ‹👤Add Admin›\n\n👮🏽‍♀️ Если не добавляется группа, то измени <b>Должность</b> (см. скрин)",
+    'en': "👇🏽 Push the ‹Group› to add into your group (with default settings): @{0}\n\n👮🏽‍♀️ Or add bot as <b>Admin</b> via Settings of your group: ‹👤Add Admin›\n\n👮🏽‍♀️ If you can't add group, try to change <b>Custom Title</b> (look screenshot)",
+    'es': "👇🏽 Presione ‹➕ Agregar grupo› para agregar a su grupo (con la configuración predeterminada): @{0}\n\n👮🏽‍♀️ O agregue bot como <b>Administrador</b> a través de la Configuración de su grupo: ‹👤Agregar administrador›\n\n👮🏽‍♀️ Si no puede agregar un grupo, intente cambiar <b>Título personalizado</b> (ver captura de pantalla)",
+    'fr': "👇🏽 Appuyez sur ‹➕ Ajouter un groupe› pour ajouter à votre groupe (avec les paramètres par défaut): @{0}\n\n👮🏽‍♀️ Ou ajoutez le bot en tant qu'<b>administrateur</b> via les paramètres de votre groupe : ‹👤Ajouter un administrateur›\n\n👮🏽‍♀️ Si vous ne pouvez pas ajouter de groupe, essayez de modifier le <b>Titre personnalisé</b> (regardez la capture d'écran)",
+    'zh': "👇🏽 按下‹➕添加群組›以添加到您的群組（使用默認設置）: @{0}\n\n👮🏽‍♀️ 或通過您組的設置將機器人添加為 <b>Admin</b>：‹👤添加管理員›\n\n👮🏽‍♀️ 如果無法添加組，請嘗試更改 <b>自定義標題</b>（看截圖）",
+    'ar': "👇🏽 اضغط على ‹➕ إضافة مجموعة› لإضافتها إلى مجموعتك (بالإعدادات الافتراضية): @{0}\n\n👮🏽‍♀️ أو أضف البوت كـ <b> مسؤول </b> عبر إعدادات مجموعتك: ‹👤 إضافة مسؤول›\n\n👮🏽‍♀️ إذا لم تتمكن من إضافة مجموعة ، فحاول تغيير <b> عنوان مخصص </b> (انظر في لقطة الشاشة)",
+}
+l_add_group_button = {
+    'ru': "➕ Добавить группу",
+    'en': "➕ Add group",
+    'es': "➕ Agregar grupo",
+    'fr': "➕ Ajouter un groupe",
+    'zh': "➕ 添加組",
+    'ar': "➕ إضافة مجموعة",
+}
+
+
+# region group
+l_group_config = {
+    ("ccheck",  "👮🏽‍", "☑"): {
+        'ru': "Входной контроль",
+        'en': "Enter control",
+        'es': "Entrar en control",
+        'fr': "Prenez le contrôle",
+        'zh': "進入控制",
+        'ar': "أدخل السيطرة",
+    },
+    ("chello", "👋🏽", "☐"): {
+        'ru': "Авто-приветствие",
+        'en': "Auto-greeting",
+        'es': "Saludo automático",
+        'fr': "Message d'accueil automatique",
+        'zh': "自動問候",
+        'ar': "الترحيب التلقائي",
+    },
+    ("cban", "🕵🏽", "☑"): {
+        'ru': "Авто-бан",
+        'en': "Auto-ban",
+        'es': "Prohibición automática",
+        'fr': "Interdiction automatique",
+        'zh': "自動禁止",
+        'ar': "حظر تلقائي",
+    },
+    ("cpost", "🔔", "☐"): {
+        'ru': "Авто-постинг",
+        'en': "Auto-posting",
+        'es': "Publicación automática",
+        'fr': "Publication automatique",
+        'zh': "自動發布",
+        'ar': "النشر التلقائي",
+    },
+    ("cinvite", "🚶", "☐"): {
+        'ru': "Авто-инвайтинг",
+        'en': "Auto-inviting",
+        'es': "Invitación automática",
+        'fr': "Invitation automatiquel",
+        'zh': "自動邀請",
+        'ar': "دعوة تلقائية",
+    },
+    ("csystem", "👣", "☐"): {
+        'ru': "Сообщ системные",
+        'en': "System messages",
+        'es': "Mensajes del sistema",
+        'fr': "Messages système",
+        'zh': "系統消息",
+        'ar': "رسائل النظام",
+    },
+    ("cchannel", "🫥", "☐"): {
+        'ru': "Cообщ от‍ имени канала",
+        'en': "Msgs from channel name",
+        'es': "Msjs del nombre del canal",
+        'fr': "Msgs du nom de la chaîne",
+        'zh': "來自頻道名稱的消息",
+        'ar': "رسائل من اسم القناة",
+    },
+    ("clink", "🔗", "☑"): {
+        'ru': "Cообщ с ссылками",
+        'en': "Messages with links",
+        'es': "Mensajes con enlaces",
+        'fr': "Messages avec liens",
+        'zh': "帶有鏈接的消息",
+        'ar': "الرسائل ذات الروابط",
+    },
+    ("csymbol", "文", "☐"): {
+        'ru': "Cообщ с 文/ب/ȳ̵͘̚",
+        'en': "Messages with 文/ب/ȳ̵͘̚",
+        'es': "Mensajes con 文/ب/y",
+        'fr': "Messagerie avec 文/ب/y",
+        'zh': "與消息 文/ب/y",
+        'ar': "文/ب/y الرسائل ذات",
+    },
+    ("cmedia", "🗣", "☐"): {
+        'ru': "Сообщ с медиа",
+        'en': "Messages with media",
+        'es': "Mensajes con medios",
+        'fr': "Msgs avec les médias",
+        'zh': "與媒體的消息",
+        'ar': "الرسائل بوسائل الإعلام",
+    },
+    ("cstart", "🚀", "☐"): {
+        'ru': "Старт-слова",
+        'en': "Start-words",
+        'es': "Palabras de inicio",
+        'fr': "Mots de départ",
+        'zh': "起始詞",
+        'ar': "بداية الكلمات",
+    },
+    ("cstop", "🧾", "☐"): {
+        'ru': "Стоп-слова",
+        'en': "Stop-words",
+        'es': "Para las palabras",
+        'fr': "Mots vides",
+        'zh': "停用詞",
+        'ar': "كلمات التوقف",
+    },
+    ("cflood", "💬", "☐"): {
+        'ru': "Стоп-флуд",
+        'en': "Stop-flood",
+        'es': "Stop-inundación",
+        'fr': "Arrêt-inondation",
+        'zh': "止水",
+        'ar': "وقف الفيضان",
+    },
+    ("cuser", "👥", "☑"): {
+        'ru': "Пользователи",
+        'en': "Users",
+        'es': "Usuarias",
+        'fr': "Utilisatrices",
+        'zh': "用戶",
+        'ar': "المستخدمون",
+    },
+    ("cadmin", "👮🏽", "☑"): {
+        'ru': "Администраторы",
+        'en': "Admins",
+        'es': "Administradoras",
+        'fr': "Administratrices",
+        'zh': "管理員",
+        'ar': "المشرفون",
+    },
+}
+l_to_group_delete = {
+    'ru': "🚫Убрать группу",
+    'en': "🚫Put away group",
+    'es': "🚫Guardar grupo",
+    'fr': "🚫Groupe de rangement",
+    'zh': "🚫收起組",
+    'ar': "🚫 أبعد المجموعة",
+}
+l_show_groups = {
+    'ru': "👩🏽‍💻 <b>Добавленные группы</b>\n\n[команды /cmd]",
+    'en': "👩🏽‍💻 <b>Добавленные группы</b>\n\n[команды /cmd]",
+    'es': "👩🏽‍💻 <b>Добавленные группы</b>\n\n[команды /cmd]",
+    'fr': "👩🏽‍💻 <b>Добавленные группы</b>\n\n[команды /cmd]",
+    'zh': "👩🏽‍💻 <b>Добавленные группы</b>\n\n[команды /cmd]",
+    'ar': "👩🏽‍💻 <b>Добавленные группы</b>\n\n[команды /cmd]",
+}
+
+l_GROUPP_CCHECKBTNNAME = {
+    'ru': "✔ Я человек",
+    'en': "✔ I am human",
+    'es': "✔ Soy humana",
+    'fr': "✔ Je suis humain",
+    'zh': "✔ 我是人",
+    'ar': "✔ أنا إنسان",
+}
+l_GROUPP_CHELLOTEXT = {
+    'ru': "🌱 {name}, добро пожаловать в нашу <b>группу</b> {title}!",
+    'en': "🌱 {name}, welcome to our <b>group</b> {title}!",
+    'es': "🌱 {name}, Bienvenida a nuestro <b>grupo</b> {title}!",
+    'fr': "🌱 {name}, bienvenue dans notre <b>groupe</b> {title}!",
+    'zh': "🌱 {name}, 歡迎加入我們的<b>群</b> {title}!",
+    'ar': "🌱 {name} ، مرحبًا بك في <b> مجموعتنا </ b> {title}!"
+}
+l_GROUPP_CCHECKCHANNEL = {
+    'ru': "👮🏽 Для <i>проверки подписки</i> необходимо добавить канал командой:\n\n/channel ССЫЛКА НА КАНАЛ",
+    'en': "👮🏽 It is necessary add channel for <i>subscribe checking</i> by command:\n\n/channel LINK",
+    'es': "👮🏽 Es necesario agregar un canal para <i>comprobar suscripciones</i> mediante el comando:\n\n/channel LINK",
+    'fr': "👮🏽 Il est nécessaire d'ajouter un canal pour <i>vérifier l'abonnement</i> par la commande :\n\n/channel LINK",
+    'zh': "👮🏽 <i>訂閱檢查</i>需要通過命令添加頻道：\n\n/channel LINK",
+    'ar': "👮🏽 من الضروري إضافة قناة لـ <i> فحص الاشتراك </i> بواسطة الأمر: \n\n/channel LINK",
+}
+# endregion
+
+
+# region commands
+l_group_commands_handler = {
+    'ru': "⚙️ <b>Настройка</b> группы <b>{0}</b> {1}\n\n<b>⛏ Admin-команды @{2}</b>\n/update <i>обновление параметров</i>\n/transfer   <i>передача admin-прав</i>\n/info   <i>информация</i>\n/stat   <i>статистика</i>\n/log   <i>посмотреть логи</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>парсинг старых id-аккаунтов</i>\n\n<b>⛏ Команды администраторов</b>\n/ban 5m|1h|10d <i>удаление из группы на время</i>\n/unban\n/mute 5m|1h|10d <i>ограничение в группе на время</i>\n/unmute\n/warn+сообщ <i>предупреждение</i>\n/status\n/karma  [+|-]\n/tag+сообщ   <i>@tager random-аккаунтов</i>\n/stop  <i>добавить стоп-слово</i>\n/channel NAME   <i>добавить канал для проверки подписки</i>\n/button NAME    <i>добавить имя кнопки входного контроля</i>\n/delay MIN      <i>установить количество min для задержки 1го сообщ</i>\n/flood NUM      <i>установить количество сообщ для flood</i>\n\n<b>⛏ Команды пользователей</b>\n/help   <i>вывод команд</i>\n/rules  <i>правила группы</i>\n/report <i>сообщить о нарушении</i>\n/happy  <i>получить радость</i>\n/thanks <i>поблагодарить</i>",
+    'en': "⚙️ <b>Group</b> settings of <b>{0}</b> {1}\n\n<b>⛏ Admin-commands @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/log   <i>see logs</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-accounts</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from group for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in group for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-accounts</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for group</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
+    'es': "⚙️ Configuración de <b>Grupo</b> de <b>{0}</b> {1}\n\n<b>⛏ Comandos de administración @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/log   <i>see logs</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-accounts</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from group for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in group for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-accounts</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for group</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
+    'fr': "⚙️ Paramètres de <b>groupe</b> de <b>{0}</b> {1}\n\n<b>⛏ Commandes d'administration @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/log   <i>see logs</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-accounts</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from group for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in group for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-accounts</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for group</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
+    'zh': "⚙️ <b>組</b>設置 <b>{0}</b> {1}\n\n<b>⛏ 管理員命令 @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/log   <i>see logs</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-accounts</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from group for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in group for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-accounts</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for group</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
+    'ar': "⚙️ إعدادات <b> المجموعة </b> الخاصة بـ <b>{0}</b> {1}\n\n<b>⛏ أوامر المسؤول @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/parse  <i>[all|old|premium|active|online]</i>\n/log   <i>see logs</i>\n<code>/parse old</code> - <i>parsing old id-accounts</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from group for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in group for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-accounts</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for group</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
+}
+l_update_handler00 = {
+    'ru': "🛡 Для дальнейшего <b>администрирования</b> данной группы запустите @{0}-бота и добавьте его в группу как <b>Administrator</b>",
+    'en': "🛡 For further <b>administration</b> of this group, please start @{0} and add this bot to group as <b>Administrator</b>",
+    'es': "🛡 Para una mayor <b>administración</b> de este grupo, inicie @{0} y agregue este bot al grupo como <b>Administrador</b>",
+    'fr': "🛡 Pour plus d'<b>administration</b> de ce groupe, veuillez démarrer @{0} et ajouter ce bot au groupe en tant qu'<b>administrateur</b>",
+    'zh': "🛡 如需進一步<b>管理</b>此群組，請啟動@{0}並將此機器人添加到群組中作為<b>管理員</b>",
+    'ar': "🛡 لمزيد من <b> الإدارة </b> لهذه المجموعة ، يرجى البدء @{0} وإضافة هذا الروبوت إلى المجموعة <b> كمسؤول </b>",
+}
+l_update_handler01 = {
+    'ru': "🛡 Группа добавлена в @{0}-бота и готова к администрированию",
+    'en': "🛡 Group added to @{0} and ready for administration",
+    'es': "🛡 Grupo agregado a @{0} y listo para administración",
+    'fr': "🛡 Groupe ajouté à @{0} et prêt pour l'administration",
+    'zh': "🛡 組已添加到 @{0} 並準備好進行管理",
+    'ar': "🛡 تمت إضافة المجموعة إلى @{0} وهي جاهزة للإدارة",
+}
+l_update_handler10 = {
+    'ru': "🛡 Группа обновлена и администрируется в @{0}-боте",
+    'en': "🛡 Group updated and administered by @{0}",
+    'es': "🛡 Grupo actualizado y administrado por @{0}",
+    'fr': "🛡 Groupe mis à jour et administré par @{0}",
+    'zh': "🛡 群組由 @{0} 更新和管理",
+    'ar': "🛡 تم تحديث المجموعة وإدارتها بواسطة @{0}",
+}
+l_update_handler100 = {
+    'ru': "🛡 Группа обновлена, но не подключена @{0}-боту! Для дальнейшего <b>администрирования</b> данной группы зайдите в @{0}-бота и нажмите /start",
+    'en': "🛡 Group updated, but not connected to @{0}! For further <b>administration</b> of this group, please /start @{0}",
+    'es': "🛡 ¡Grupo actualizado, pero no conectado a @{0}! Para continuar con la <b>administración</b> de este grupo, /start @{0}",
+    'fr': "🛡 Groupe mis à jour, mais pas connecté à @{0} ! Pour plus d'<b>administration</b> de ce groupe, veuillez /start @{0}",
+    'zh': "🛡 群組已更新，但未連接到 @{0}！ 如需進一步<b>管理</b>此組，請 /start @{0}",
+    'ar': "🛡 تم تحديث المجموعة ولكنها غير مرتبطة بـ @{0}! لمزيد من <b> الإدارة </b> لهذه المجموعة ، يرجى / start @{0}",
+}
+l_group_info_start1 = {
+    'ru': "ℹ️ <b>Общая информация о группе</b>\n\n<b>Название</b>: {0} [id=<code>{1}</code>, <i>{2} {3}</i>, <u>{4}</u> участ.]{5}{6}{7}",
+    'en': "ℹ️ <b>Common info about channel statistics</b>\n\n",
+    'es': "ℹ️ <b>Información común sobre las estadísticas del grupo</b>\n\n",
+    'fr': "ℹ️ <b>Informations communes sur les statistiques de channele</b>\n\n",
+    'zh': "ℹ️ <b>關於組統計的常見信息</b>\n\n",
+    'ar': "ℹ️ <b> معلومات عامة حول إحصائيات المجموعة </b> \n\n",
+}
+l_group_stat_start = {
+    'ru': "ℹ️ <b>Общая информация о статистике группы</b>\n\n",
+    'en': "ℹ️ <b>Common info about group statistics</b>\n\n",
+    'es': "ℹ️ <b>Información común sobre las estadísticas del grupo</b>\n\n",
+    'fr': "ℹ️ <b>Informations communes sur les statistiques de groupe</b>\n\n",
+    'zh': "ℹ️ <b>關於組統計的常見信息</b>\n\n",
+    'ar': "ℹ️ <b> معلومات عامة حول إحصائيات المجموعة </b> \n\n",
+}
+l_group_stat_start1 = {
+    'ru': "ℹ️ <b>Общая статистика группы</b>\n\n<b>Название</b>: {0} [id=<code>{1}</code>, <i>{2} {3}</i>, <u>{4}</u> участ.]{5}{6}{7}",
+    'en': "ℹ️ <b>Common info about channel statistics</b>\n\n",
+    'es': "ℹ️ <b>Información común sobre las estadísticas del grupo</b>\n\n",
+    'fr': "ℹ️ <b>Informations communes sur les statistiques de channele</b>\n\n",
+    'zh': "ℹ️ <b>關於組統計的常見信息</b>\n\n",
+    'ar': "ℹ️ <b> معلومات عامة حول إحصائيات المجموعة </b> \n\n",
+}
+l_group_stat_start2 = {
+    'ru': "\n<b>Ссылка</b>: {0}\n<b>Описание</b>: {1}\n<b>Привязанный канал</b>: <code>{2}</code>\n",
+    'en': "ℹ️ <b>Common info about channel statistics</b>\n\n",
+    'es': "ℹ️ <b>Información común sobre las estadísticas del grupo</b>\n\n",
+    'fr': "ℹ️ <b>Informations communes sur les statistiques de channele</b>\n\n",
+    'zh': "ℹ️ <b>關於組統計的常見信息</b>\n\n",
+    'ar': "ℹ️ <b> معلومات عامة حول إحصائيات المجموعة </b> \n\n",
+}
+l_group_stat_start3 = {
+    'ru': "<b>Сообщения</b>: {0}\n<b>Дата 1го сообщ</b>: ~{1}\n<b>ID последнего сообщ</b>: {2}\n",
+    'en': "ℹ️ <b>Common info about channel statistics</b>\n\n",
+    'es': "ℹ️ <b>Información común sobre las estadísticas del grupo</b>\n\n",
+    'fr': "ℹ️ <b>Informations communes sur les statistiques de channele</b>\n\n",
+    'zh': "ℹ️ <b>關於組統計的常見信息</b>\n\n",
+    'ar': "ℹ️ <b> معلومات عامة حول إحصائيات المجموعة </b> \n\n",
+}
+l_participants = {
+    'ru': "участ.",
+    'en': "users",
+    'es': "usuarias",
+    'fr': "utilisatrices",
+    'zh': "用戶",
+    'ar': "المستخدمين",
+}
+l_info_opportunity = {
+    'ru': "<b>Возможность просмотра увидевших сообщ</b>: <code>Да (до 50участ.)</code>\n",
+    'en': "<b>Opportunity to see Message-Seen</b>: <code>Yes (up to 50users)</code>\n",
+    'es': "<b>Oportunidad de ver mensajes vistos</b>: <code>Sí (hasta 50 usuarios)</code>\n",
+    'fr': "<b>Possibilité de voir Message-Seen</b> : <code>Oui (jusqu'à 50 utilisateurs)</code>\n",
+    'zh': "<b>查看消息的機會</b>：<code>是（最多 50 個用戶）</code>\n",
+    'ar': "<b> فرصة لرؤية الرسالة المرئية </b>: <code> نعم (حتى 50 مستخدمًا) </code> \n",
+}
+l_info_history = {
+    'ru': "<b>История для новых участников</b>: ",
+    'en': "<b>History for new participants</b>: ",
+    'es': "<b>Historial de nuevos participantes</b>:",
+    'fr': "<b>Historique pour les nouveaux participants</b> :",
+    'zh': "<b>新參與者的歷史</b>：",
+    'ar': "<b> سجل للمشاركين الجدد </b>:",
+}
+l_info_history_show = {
+    'ru': "<code>видна</code>\n",
+    'en': "<code>visible</code>\n",
+    'es': "<code>visible</code>\n",
+    'fr': "<code>visible</code>\n",
+    'zh': "<code>可見的</code>\n",
+    'ar': "<code>مرئي</code>\n",
+}
+l_info_history_hide = {
+    'ru': "<code>скрыта</code>\n",
+    'en': "<code>hidden</code>\n",
+    'es': "<code>oculta</code>\n",
+    'fr': "<code>cachée</code>\n",
+    'zh': "<code>隱</code>\n",
+    'ar': "<code>مختفي</code>\n",
+}
+l_info_autodel = {
+    'ru': "<b>Автоудаление сообщений</b>: ",
+    'en': "<b>Auto-delete time for msg</b>: ",
+    'es': "<b>Tiempo de eliminación automática para msg</b>:",
+    'fr': "<b>Heure de suppression automatique des msg</b> :",
+    'zh': "<b>自動刪除消息的時間</b>：",
+    'ar': "<b> وقت الحذف التلقائي للرسائل </b>:",
+}
+l_info_slowmode = {
+    'ru': "<b>Как часто можно писать</b>: ",
+    'en': "<b>Slow Mode</b>: ",
+    'es': "<b>Modo lento</b>:",
+    'fr': "<b>Mode lent</b> :",
+    'zh': "<b>慢速模式</b>：",
+    'ar': "<b> الوضع البطيء </b>:",
+}
+l_info_slowmode_limitless = {
+    'ru': "<code>без ограничений</code>\n",
+    'en': "<code>without limits</code>\n",
+    'es': "<code>sin límites</code>\n",
+    'fr': "<code>sans limites</code>\n",
+    'zh': "<code>沒有限制</code>\n",
+    'ar': "<code>من غير قيود</code>\n",
+}
+l_info_oppforpart = {
+    'ru': "Возможности участников",
+    'en': "Participants opportunities",
+    'es': "Oportunidades de los participantes",
+    'fr': "Opportunités pour les participants",
+    'zh': "參與者機會",
+    'ar': "فرص المشاركين",
+}
+l_change_group_info = {
+    'ru': "Изменение профиля группы",
+    'en': "Change Group Info",
+    'es': "Cambiar información del grupo",
+    'fr': "Modifier les informations du groupe",
+    'zh': "更改組信息",
+    'ar': "تغيير معلومات المجموعة",
+}
+l_pin_message = {
+    'ru': "Закрепление сообщений",
+    'en': "Pin Messages",
+    'es': "Mensajes de pines",
+    'fr': "Épingler les messages",
+    'zh': "固定消息",
+    'ar': "تثبيت الرسائل",
+}
+l_add_members = {
+    'ru': "Добавление участников",
+    'en': "Add Members",
+    'es': "Añadir miembros",
+    'fr': "Ajouter des membres",
+    'zh': "添加成員",
+    'ar': "إضافة أعضاء",
+}
+l_embed_links = {
+    'ru': "Предпросмотр ссылок",
+    'en': "Embed links",
+    'es': "Insertar enlaces",
+    'fr': "Intégrer des liens",
+    'zh': "嵌入鏈接",
+    'ar': "روابط التضمين",
+}
+l_send_media = {
+    'ru': "Отправка фото и видео",
+    'en': "Send Media",
+    'es': "Enviar medios",
+    'fr': "Envoyer le média",
+    'zh': "發送媒體",
+    'ar': "إرسال الوسائط",
+}
+l_send_polls = {
+    'ru': "Отправка опросов",
+    'en': "Send Polls",
+    'es': "Enviar encuestas",
+    'fr': "Envoyer des sondages",
+    'zh': "發送投票",
+    'ar': "إرسال استطلاعات الرأي",
+}
+l_send_stickers = {
+    'ru': "Отправка sticker/giff/via_bot",
+    'en': "Send sticker/giff/via_bot",
+    'es': "apagada",
+    'fr': "à l'arrêt",
+    'zh': "離開",
+    'ar': "إيقاف",
+}
+l_info_anonymous_for = {
+    'ru': "Анонимность для",
+    'en': "Anonymous for",
+    'es': "Anónimo para",
+    'fr': "Anonyme pour",
+    'zh': "匿名",
+    'ar': "مجهول لـ",
+}
+
+l_stat_msg_cnt = {
+    'ru': "Количество сообщ",
+    'en': "Message number",
+    'es': "Recuento de mensajes",
+    'fr': "Nombre de messages",
+    'zh': "消息數",
+    'ar': "عدد الرسائل",
+}
+l_stat_history_for_new = {
+    'ru': "История для новых участников",
+    'en': "History for new members",
+    'es': "Historia para nuevas miembros",
+    'fr': "Historique pour les nouveaux membres",
+    'zh': "Historia para nuevas miembros",
+    'ar': "التاريخ للأعضاء الجدد",
+}
+l_stat_history_turn_on = {
+    'ru': "(для просмотра статистики <u>включите</u> [Историю группы])",
+    'en': "(to show statistics <u>enable</u> [Group history])",
+    'es': "(para mostrar estadísticas <u>activar</u> [Historial del grupo])",
+    'fr': "(pour afficher les statistiques, <u>activez</u> [Historique du groupe])",
+    'zh': "（顯示統計信息<u>開啟</u> [群組歷史]）",
+    'ar': "(لإظهار الإحصائيات <u> قم بتشغيل </u> [سجل المجموعة])",
+}
+l_stat_first_msg_date = {
+    'ru': "Дата 1-го сообщ",
+    'en': "1st msg date",
+    'es': "fecha del 1er mensaje",
+    'fr': "Date du 1er message",
+    'zh': "第一個消息日期",
+    'ar': "تاريخ الرسالة الأولى",
+}
+l_stat_involved = {
+    'ru': "Вовлеченность в чате",
+    'en': "Сhat engagement",
+    'es': "Compromiso de chat",
+    'fr': "Сat engagement",
+    'zh': "Сhat 訂婚",
+    'ar': "المشاركة الدردشة",
+}
+l_stat_sent = {
+    'ru': "{0}\n@{1} написал(а): {2}  сообщ",
+    'en': "{0}\n@{1} write: {2} message",
+    'es': "{0}\n@{1} escribir: {2} mensaje",
+    'fr': "{0}\n@{1} écrire : {2} message",
+    'zh': "{0}\n@{1} 寫：{2} 條消息",
+    'ar': "{0} \n @{1} اكتب: {2} رسالة",
+}
+l_stat_meet = {
+    'ru': "{0}\n{1}. <i>{2}</i>..: встретилось {3} раз",
+    'en': "{0}\n{1}. <i>{2}</i>..: met {3} times",
+    'es': "{0}\n{1}. <i>{2}</i>..: se reunió {3} veces",
+    'fr': "{0}\n{1}. <i>{2}</i>.. : rencontré {3} fois",
+    'zh': "{0}\n{1}。 <i>{2}</i>..：遇到 {3} 次",
+    'ar': "{0} \n {1}. <i>{2}</i> ..: التقى {3} مرة",
+}
+l_stat_top5users = {
+    'ru': "Топ 5 пользователей (на 1000 сообщ)",
+    'en': "Top 5 users (for 1000 msgs)",
+    'es': "Las 5 mejores usuarios (para 1000 msgs)",
+    'fr': "Top 5 des utilisateurs (pour 1000 msgs)",
+    'zh': "前 5 名用戶（1000 條消息）",
+    'ar': "أعلى 5 مستخدمين (لكل 1000 رسالة)",
+}
+l_stat_top5msgs = {
+    'ru': "Топ 5 сообщ (из 1000)",
+    'en': "Top 5 msgs (from 1000)",
+    'es': "Las 5 mejores mensajes (desde 1000)",
+    'fr': "Top 5 des messages (sur 1000)",
+    'zh': "前 5 條消息（來自 1000 條）",
+    'ar': "أهم 5 رسائل (من 1000)",
+}
+l_status_for = {
+    'ru': "⚠️ Статус <b>{0}</b> для {1}:\n\n",
+    'en': "⚠️ Статус <b>{0}</b> для {1}:\n\n",
+    'es': "Las 5 mejores mensajes (desde 1000)",
+    'fr': "Top 5 des messages (sur 1000)",
+    'zh': "前 5 條消息（來自 1000 條）",
+    'ar': "أهم 5 رسائل (من 1000)",
+}
+
+l_transfer_reply = {
+    'ru': "⚠️ Используйте команду /transfer в <b>ответном</b> сообщении пользователя, которому вы хотите передать права",
+    'en': "⚠️ Use /transfer-command in reply user-message to transfer him ownership",
+    'es': "⚠️ Use /transfer-command en el mensaje de usuario de respuesta para transferirle la propiedad",
+    'fr': "⚠️ Utilisez /transfer-command dans le message utilisateur de réponse pour lui transférer la propriété",
+    'zh': "⚠️ 使用 /transfer-command 回复 user-message 轉移他的所有權",
+    'ar': "استخدم الأمر transfer-command/ في الرد على رسالة المستخدم لنقل ملكيته",
+}
+l_button_handler = {
+    'ru': "👮🏽 Готово! Текущее <b>имя кнопки</b> на <i>входном контроле</i> установлено: {0}",
+    'en': "👮🏽 Ready! Current <b>button name</b> in <i>Enter control</i> is: {0}",
+    'es': "👮🏽 Lista! El <b>nombre del botón</b> actual en <i>Control de entrada</i> es: {0}",
+    'fr': "👮🏽 Prêt! Le <b>nom du bouton</b> actuel dans <i>Saisir le contrôle</i> est : {0}",
+    'zh': "👮🏽 準備好! <i>輸入控件</i>中的當前<b>按鈕名稱</b>是：{0}",
+    'ar': "👮🏽 جاهز! <b> اسم الزر </b> الحالي في <i> إدخال التحكم </i> هو: {0}",
+}
+l_button_correct = {
+    'ru': "👮🏽 Введи корректное название <i>для имени кнопки</i> Входного контроля\n\n👉🏼 Например, <code>/button {0}</code>",
+    'en': "👮🏽 Enter correct <i>button name</i> for Enter control\n\n👉🏼 For example, <code>/button {0}</code>",
+    'es': "👮🏽 Ingrese el <i>nombre del botón</i> correcto para el control Intro\n\n👉🏼 Por ejemplo, <código>/botón {0}</código>",
+    'fr': "👮🏽 Saisissez le <i>nom du bouton</i> correct pour Entrer le contrôle\n\n👉🏼 Par exemple, <code>/bouton {0}</code>",
+    'zh': "👮🏽 為 Enter 控件輸入正確的 <i>按鈕名稱</i>\n\n👉🏼 例如，<code>/button {0}</code>",
+    'ar': "👮🏽 أدخل <i> اسم الزر </i> الصحيح لإدخال عنصر التحكم \n\n👉🏼 على سبيل المثال ، <code> / button {0}</code>",
+}
+l_channel_check = {
+    'ru': "⚙️ Добавь @{0}-бота в канал для проверки подписки на него. Пришли мне корректную ссылку на канал:",
+    'en': "⚙️ Add @{0} to channel for subscribe checking. Send me correct link to channel:",
+    'es': "⚙️ Agregue @{0} al canal para verificar la suscripción. Envíame el enlace correcto al canal:",
+    'fr': "⚙️ Ajoutez @{0} à la chaîne pour vérifier l'abonnement. Envoyez-moi le lien correct vers la chaîne :",
+    'zh': "⚙️ 將@{0} 添加到頻道以進行訂閱檢查。 向我發送正確的頻道鏈接：",
+    'ar': "⚙️ إضافة @{0} للقناة للتحقق من الاشتراك. أرسل لي الرابط الصحيح للقناة:",
+}
+l_channel_done = {
+    'ru': "👮🏽 Готово! Проверка подписки на {0}-канал настроена\n\nОпцию можно включить в настройках, нажав [✅☑Вкл подписку]",
+    'en': "👮🏽 Ready! Subscribe checking to {0}-channel is configured\n\nEnable this option in the Settings by pushing [✅☑Enable subscription]",
+    'es': "👮🏽 Listo! La verificación de suscripción a {0}-canal está configurada\n\nActive esta opción en Configuración presionando [✅☑Habilitar suscripción]",
+    'fr': "👮🏽 Prêt! La vérification de l'abonnement à la chaîne {0} est configurée\n\nActivez cette option dans les paramètres par push [✅☑Activer l'abonnement]",
+    'zh': "👮🏽 準備好了！ 已配置對 {0} 頻道的訂閱檢查\n\n通過推送在“設置”中打開此選項 [✅☑啟用訂閱]",
+    'ar': "👮🏽 جاهز! التحقق من الاشتراك في {0} - تم تكوين القناة \n\n قم بتشغيل هذا الخيار في الإعدادات عن طريق الدفع [✅☑ تمكين الاشتراك]",
+}
+l_channel_correct = {
+    'ru': "👮🏽 Добавь @{0}-бота в канал и отправь корректную <i>ссылку</i> этого канала\n\n👉🏼 Например, <code>/channel @{1}</code>",
+    'en': "👮🏽 Add @{0} to channel and send correct <i>link</i> of this channel\n\n👉🏼 For example, <code>/channel @{1}</code>",
+    'es': "👮🏽 Agrega @{0} al canal y envía el <i>enlace</i> correcto de este canal\n\n👉🏼 Por ejemplo, <code>/channel @{1}</code>",
+    'fr': "👮🏽 Ajoutez @{0} au canal et envoyez le <i>lien</i> correct de ce canal\n\n👉🏼 Par exemple, <code>/channel @{1}</code>",
+    'zh': "👮🏽 將@{0} 添加到頻道並發送此頻道的正確<i>鏈接</i>\n\n👉🏼 例如，<code>/channel @{1}</code>",
+    'ar': "👮🏽 إضافة @{0} إلى القناة وإرسال <i> الرابط </i> الصحيح لهذه القناة \n \n👉🏼 على سبيل المثال ، <code> / channel @{1}</code>",
+}
+l_delay_correct = {
+    'ru': "👥 Введи корректное <i>число</i> минут для первичного ограничения новых пользователей\n\n👉🏼 Например, <code>/delay 1</code>\n\nИли используй <b>медленный режим</b> в настройках группы для <u>1</u> сообщения",
+    'en': "👥 Enter correct <i>number</i> in minutes for primary mute-restriction for new users\n\n👉🏼 For example, <code>/delay 1</code>\n\nOr use <b>Slow Mode</b> in group Settings for <u>1</u>st message",
+    'es': "👥 Ingrese el <i>número</i> correcto en minutos para la restricción de silencio principal para nuevos usuarios\n\n👉🏼 Por ejemplo, <code>/delay 1</code>\n\nO use <b>Slow Mode </b> en Configuración de grupo para <u>1</u>er mensaje",
+    'fr': "👥 Entrez le <i>nombre</i> correct en minutes pour la restriction principale de mise en sourdine pour les nouveaux utilisateurs\n\n👉🏼 Par exemple, <code>/delay 1</code>\n\nOu utilisez le <b>mode lent </b> dans le groupe Paramètres pour le <u>1</u>er message",
+    'zh': "👥 在分鐘內輸入正確的 <i>number</i> 用於新用戶的主要靜音限制\n\n👉🏼 例如，<code>/delay 1</code>\n\n或使用 <b>Slow Mode <u>1</u>st 消息的組設置中的</b>",
+    'ar': "👥 أدخل <i> الرقم الصحيح </i> في دقائق لتقييد كتم الصوت الأساسي للمستخدمين الجدد \n \n👉🏼 على سبيل المثال ، <code> / تأخير 1 </code> \n \n أو استخدم <b> الوضع البطيء </b> في إعدادات المجموعة لرسالة <u> 1 </u> st",
+}
+l_parse_error = {
+    'ru': "📇 Осуществить парсинг пользователей  не удалось",
+    'en': "📇 Parsing (by @username) is failed",
+    'es': "📇 El análisis (por @username) falló",
+    'fr': "📇 L'analyse (par @username) a échoué",
+    'zh': "📇 解析（@username）失敗",
+    'ar': "📇 فشل التحليل (حسب اسم المستخدم)",
+}
+l_parse_done = {
+    'ru': "🔥 Готово! Собрано реальных участников: <u>{0}</u>. Можно сразу сделать <b>рассылку</b> или подписку-<b>инвайт</b> в чат по <i>полученным</i> лидам{1}",
+    'en': "🔥 Ready! Gathered members: <u>{0}</u>. You can immediately make an <b>sending</b> or <b>inviting</b> to group by received members{1}",
+    'es': "🔥 Listo! Miembros reunidos: <u>{0}</u>. Inmediatamente puede hacer un <b>envío</b> o <b>invitación</b> al grupo por miembros recibidos{1}",
+    'fr': "🔥 Prêt ! Membres réunis : <u>{0}</u>. Vous pouvez immédiatement faire un <b>envoi</b> ou <b>inviter</b> pour grouper par membres reçus{1}",
+    'zh': "🔥 準備好了！ 聚集成員：<u>{0}</u>。 您可以立即<b>發送</b>或<b>邀請</b>按收到的成員分組{1}",
+    'ar': "🔥 جاهز! الأعضاء الذين تم تجميعهم: <u>{0}</u>. يمكنك على الفور إجراء <b> إرسال </b> أو <b> دعوة </b> للانضمام إلى المجموعة بواسطة الأعضاء المستلمين {1}",
+}
+l_parse_btnsend = {
+    'ru': "📨️ Рассылка",
+    'en': "📨️ Sending",
+    'es': "📨️ Enviando",
+    'fr': "📨️ Envoi",
+    'zh': "📨️ 發送",
+    'ar': "📨️ الإرسال",
+}
+l_parse_btninvite = {
+    'ru': "🚶🏽 Инвайт",
+    'en': "🚶🏽 Inviting",
+    'es': "🚶🏽 invitando",
+    'fr': "🚶🏽 Invitant",
+    'zh': "🚶🏽 邀請",
+    'ar': "🚶🏽 دعوة",
+}
+l_parse_start = {
+    'ru': "📇 Начинаем парсинг..",
+    'en': "📇 Parsing is started..",
+    'es': "📇 Se inicia el análisis..",
+    'fr': "📇 L'analyse est lancée..",
+    'zh': "📇 解析開始..",
+    'ar': "📇 بدأ الإعراب ..",
+}
+l_ban_handler = {
+    'ru': "🪦 Пользователь {0} в бане на {1}",
+    'en': "🪦 User {0} is banned for {1}",
+    'es': "🪦 El usuario {0} está baneado por{1}",
+    'fr': "🪦 L'utilisateur {0} est banni pour{1}",
+    'zh': "🪦 用戶 {0} 因 в {1} 而被禁止",
+    'ar': "🪦 المستخدم {0} محظور منذ {1}",
+}
+l_ban_error = {
+    'ru': "🪦 Формат бана: /ban (1m|1h|10d)",
+    'en': "🪦 Ban format: /ban (1m|1h|10d)",
+    'es': "🪦 Formato de prohibición: /ban (1m|1h|10d)",
+    'fr': "🪦 Format d'interdiction : /ban (1m|1h|10j)",
+    'zh': "🪦 禁令格式：/ban (1m|1h|10d)",
+    'ar': "🪦 تنسيق الحظر: / ban (1m | 1h | 10d)",
+}
+l_ban_unban = {
+    'ru': "🪦 Пользователь возвращен из бана",
+    'en': "🪦 User is returned from ban",
+    'es': "🪦 Usuario que regresa de la prohibición",
+    'fr': "🪦 Retour de l'utilisateur de l'interdiction",
+    'zh': "🪦 用戶從禁令中返回",
+    'ar': "🪦 عودة المستخدم من الحظر",
+}
+l_mute_handler = {
+    'ru': "💤 Пользователь {0} обеззвучен на {1}",
+    'en': "💤 User {0} is muted for {1}",
+    'es': "💤 La usuario {0} está silenciada por {1}",
+    'fr': "💤 L'utilisateur {0} est mis en sourdine pendant {1}",
+    'zh': "💤 用戶 {0} 為 {1} 靜音",
+    'ar': "💤 المستخدم {0} مكتوم لـ {1}",
+}
+l_mute_error = {
+    'ru': "💤 Формат обеззвучивания: /mute (1m|1h|10d)",
+    'en': "💤 Mute format: /mute (1m|1h|10d)",
+    'es': "💤 Formato de silencio: /mute (1m|1h|10d)",
+    'fr': "💤 Format muet : /muet (1m|1h|10j)",
+    'zh': "💤 靜音格式：/mute (1m|1h|10d)",
+    'ar': "💤 تنسيق كتم الصوت: / كتم الصوت (1 م | 1 س | 10 د)",
+}
+l_mute_unmute = {
+    'ru': "💤 Пользователь {0} больше не обеззвучен",
+    'en': "💤 User is no longer in mute",
+    'es': "💤 La usuario ya no está en silencio.",
+    'fr': "💤 L'utilisateur n'est plus en mode muet",
+    'zh': "💤 用戶不再靜音",
+    'ar': "💤 لم يعد المستخدم في وضع الصامت",
+}
+l_warn_handler = {
+    'ru': "⚠️ От имени группы <b>{0}</b> выносится предупреждение {1}{2}",
+    'en': "⚠️ In the name of the group <b>{0}</b> a warning is issued to {1}{2}",
+    'es': "⚠️ En el nombre del grupo <b>{0}</b> se emite una advertencia a {1}{2}",
+    'fr': "⚠️ Au nom du groupe <b>{0}</b> un avertissement est émis à {1}{2}",
+    'zh': "⚠️ 以組 <b>{0}</b> 的名義向 {1}{2} 發出警告",
+    'ar': "⚠️ باسم المجموعة <b>{0}</b> تم إصدار تحذير لـ {1} {2}",
+}
+l_status_pin = {
+    'ru': "Закреп сообщ",
+    'en': "Pin message",
+    'es': "Pin mensaje",
+    'fr': "Épingler le message",
+    'zh': "固定消息",
+    'ar': "رسالة دبوس",
+}
+l_status_profile = {
+    'ru': "Изменение профиля группы",
+    'en': "Change Group Info",
+    'es': "Cambiar información del grupo",
+    'fr': "Modifier les informations du groupe",
+    'zh': "更改組信息",
+    'ar': "تغيير معلومات المجموعة",
+}
+l_sendmsg = {
+    'ru': "Отправка сообщ",
+    'en': "Sending messages",
+    'es': "Enviando mensajes",
+    'fr': "Envoi de messages",
+    'zh': "發送消息",
+    'ar': "إرسال الرسائل",
+}
+l_status_limit = {
+    'ru': "Ограничения до",
+    'en': "Limit for",
+    'es': "Límite para",
+    'fr': "Limite pour",
+    'zh': "限制為",
+    'ar': "حد لـ",
+}
+l_status_without = {
+    'ru': "(отсутствует) для",
+    'en': "(none) for",
+    'es': "(ninguno) para",
+    'fr': "(aucun) pour",
+    'zh': "（無）為",
+    'ar': "(لا شيء) لـ",
+}
+
+l_karma_current = {
+    'ru': "Текущая карма пользователя",
+    'en': "Current Karma of user",
+    'es': "Karma actual de la usuaria",
+    'fr': "Karma actuel de l'utilisateur",
+    'zh': "用戶當前的業力",
+    'ar': "الكارما الحالية للمستخدم",
+}
+l_karma_in_group = {
+    'ru': "в группе",
+    'en': "in group",
+    'es': "en grupo",
+    'fr': "en groupe",
+    'zh': "在小組中",
+    'ar': "في مجموعة",
+}
+l_karma_all = {
+    'ru': "🪺 Карма пользователей группы <b>{0}</b>",
+    'en': "🪺 Karma of group users <b>{0}</b>",
+    'es': "🪺 Karma de las usuarias del grupo <b>{0}</b>",
+    'fr': "🪺 Karma des utilisateurs du groupe <b>{0}</b>",
+    'zh': "🪺 群組用戶的業力 <b>{0}</b>",
+    'ar': "🪺 كارما مجموعة المستخدمين <b>{0}</b>",
+}
+l_karma_off = {
+    'ru': "🪹 Карма пользователей группы <b>{0}</b> не установлена",
+    'en': "🪹 Karma of group users <b>{0}</b> is none",
+    'es': "🪹 El karma de las usuarias del grupo <b>{0}</b> no es ninguna",
+    'fr': "🪹 Le karma des utilisateurs du groupe <b>{0}</b> est nul",
+    'zh': "🪹 群組用戶 <b>{0}</b> 的業力是無",
+    'ar': "🪹 كارما مجموعة المستخدمين <b>{0}</b> لا توجد",
+}
+l_tag_handler = {
+    'ru': "@ Необходимо ввести сообщение",
+    'en': "@ You have to write message",
+    'es': "@ Tienes que escribir mensaje",
+    'fr': "@ Vous devez écrire un message",
+    'zh': "@你必須寫消息",
+    'ar': "@ عليك كتابة رسالة",
+}
+l_help_handler = {
+    'ru': "👉🏼 <b>Команды</b> пользователя:\n\n/rules - правила группы\n/report - сообщить о нарушении\n/happy - получить радость\n/thanks - поблагодарить",
+    'en': "👉🏼 <b>Users commands</b>:\n\n/rules - of group\n/report - about violation of the rules\n/happy - get happiness\n/thanks - say thank you",
+    'es': "👉🏼 <b>Comandos de las usuarias</b>:\n\n/rules - of group\n/report - about violation of the rules\n/happy - get happiness\n/thanks - say thank you",
+    'fr': "👉🏼 <b>Commandes utilisateurs</b>:\n\n/rules - of group\n/report - about violation of the rules\n/happy - get happiness\n/thanks - say thank you",
+    'zh': "👉🏼 <b>用戶命令</b>:\n\n/rules - of group\n/report - about violation of the rules\n/happy - get happiness\n/thanks - say thank you",
+    'ar': "👉🏼 <b>أوامر المستخدمين</b>:\n\n/rules - of group\n/report - about violation of the rules\n/happy - get happiness\n/thanks - say thank you",
+}
+l_report_handler = {
+    'ru': "❗️ Информация передана администратору. Пользователь {0} взят на карандаш",
+    'en': "❗️ User {0} in group <b>{1}</b> ask to pay attention to message {2}{3}",
+    'es': "❗️ El usuario {0} del grupo <b>{1}</b> pide prestar atención al mensaje {2}{3}",
+    'fr': "❗️ L'utilisateur {0} du groupe <b>{1}</b> demande de prêter attention au message {2}{3}",
+    'zh': "❗️ <b>{1}</b> 組中的用戶 {0} 要求關註消息 {2}{3}",
+    'ar': "❗️ يطلب المستخدم {0} في مجموعة <b>{1}</b> الانتباه إلى الرسالة {2} {3}",
+}
+l_report_admin = {
+    'ru': "❗️ Пользователь {0} в группе <b>{1}</b> просит обратить внимание на сообщение {2}{3}",
+    'en': "❗️ User {0} in group <b>{1}</b> ask to pay attention to message {2}{3}",
+    'es': "❗️ El usuario {0} del grupo <b>{1}</b> pide prestar atención al mensaje {2}{3}",
+    'fr': "❗️ L'utilisateur {0} du groupe <b>{1}</b> demande de prêter attention au message {2}{3}",
+    'zh': "❗️ <b>{1}</b> 組中的用戶 {0} 要求關註消息 {2}{3}",
+    'ar': "❗️ يطلب المستخدم {0} في مجموعة <b>{1}</b> الانتباه إلى الرسالة {2} {3}",
+}
+l_report_reply = {
+    'ru': "❗ Отправь эту команду в ответ на сообщение",
+    'en': "❗ Send this command as reply to message",
+    'es': "❗ Enviar este comando como respuesta al mensaje",
+    'fr': "❗ Envoyez cette commande en réponse au message",
+    'zh': "❗ 將此命令作為對消息的回復發送",
+    'ar': "❗ أرسل هذا الأمر كرد على الرسالة",
+}
+l_thanks_handler = {
+    'ru': "🎉 От имени группы <b>{0}</b> обьявляется благодарность {1}{2}",
+    'en': "🎉 In the name of the group <b>{0}</b> gratitude is announced to {1}{2}",
+    'es': "🎉 En nombre del grupo <b>{0}</b> se anuncia el agradecimiento a {1}{2}",
+    'fr': "🎉 Au nom du groupe <b>{0}</b> la gratitude est annoncée à {1}{2}",
+    'zh': "🎉 以 <b>{0}</b> 小組的名義向 {1}{2} 宣布感謝",
+    'ar': "🎉 باسم المجموعة <b>{0}</b> تم الإعلان عن الامتنان لـ {1} {2}",
+}
+l_thanks_reply = {
+    'ru': "🎉 Отправь эту команду в ответ на сообщение",
+    'en': "🎉 Send this command as reply to message",
+    'es': "🎉 Enviar este comando como respuesta al mensaje",
+    'fr': "🎉 Envoyez cette commande en réponse au message",
+    'zh': "🎉 將此命令作為對消息的回復發送",
+    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
+}
+l_birthday_handler = {
+    'ru': "🎉 От имени группы <b>{0}</b> поздравляем с днем рождения {1}{2}",
+    'en': "🎉 In the name of the group <b>{0}</b> gratitude is announced to {1}{2}",
+    'es': "🎉 En nombre del grupo <b>{0}</b> se anuncia el agradecimiento a {1}{2}",
+    'fr': "🎉 Au nom du groupe <b>{0}</b> la gratitude est annoncée à {1}{2}",
+    'zh': "🎉 以 <b>{0}</b> 小組的名義向 {1}{2} 宣布感謝",
+    'ar': "🎉 باسم المجموعة <b>{0}</b> تم الإعلان عن الامتنان لـ {1} {2}",
+}
+l_birthday_reply = {
+    'ru': "🎉 Отправь эту команду в ответ на сообщение",
+    'en': "🎉 Send this command as reply to message",
+    'es': "🎉 Enviar este comando como respuesta al mensaje",
+    'fr': "🎉 Envoyez cette commande en réponse au message",
+    'zh': "🎉 將此命令作為對消息的回復發送",
+    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
+}
+l_videochat_text = {
+    'ru': "🎥 Автоматическое анонсирование <b>видео-трансляции</b> <code>[/videochat d h]</code> каждый <u>d</u>-день (1-31) на <u>h</u>-часов (1-168). Текущее значение: /videochat {0}\n\n👩🏽‍💻 Например,\n<code>/videochat 1 1</code> (ежедневный видео-анонс длительностью 1 час)\n<code>/videochat 0</code> (отключение опции)",
+    'en': "🎥 Send this command as reply to message",
+    'es': "🎥 Enviar este comando como respuesta al mensaje",
+    'fr': "🎥 Envoyez cette commande en réponse au message",
+    'zh': "🎥 將此命令作為對消息的回復發送",
+    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
+}
+l_flood_text = {
+    'ru': "💬 Введи корректное <i>число</i> сообщений от <u>3</u> до <u>10</u>\n\n👉🏼 Текущее значение <code>/flood {0}</code>\n\n👩🏽‍💻 Например, /flood 3 (идентификация 3х сообщений подряд как flood)\n/flood 0 (отключение опции)",
+    'en': "🎥 Send this command as reply to message",
+    'es': "🎥 Enviar este comando como respuesta al mensaje",
+    'fr': "🎥 Envoyez cette commande en réponse au message",
+    'zh': "🎥 將此命令作為對消息的回復發送",
+    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
+}
+l_flood_on = {
+    'ru': "💬 Установлен flood-режим: {0} сообщения подряд",
+    'en': "🎥 Send this command as reply to message",
+    'es': "🎥 Enviar este comando como respuesta al mensaje",
+    'fr': "🎥 Envoyez cette commande en réponse au message",
+    'zh': "🎥 將此命令作為對消息的回復發送",
+    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
+}
+l_flood_off = {
+    'ru': "💬 Режим flood отключен",
+    'en': "🎥 Send this command as reply to message",
+    'es': "🎥 Enviar este comando como respuesta al mensaje",
+    'fr': "🎥 Envoyez cette commande en réponse au message",
+    'zh': "🎥 將此命令作為對消息的回復發送",
+    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
+}
+l_delay_text = {
+    'ru': "👥 Введи корректное <i>число</i> минут для первичного ограничения новых пользователей\n\n👉🏼 Текущее значение <code>/delay {0}</code>\n\n👩🏽‍💻 Например, /delay 3 (ограничение на 3 min)\n/delay 0 (отключение опции)",
+    'en': "🎥 Send this command as reply to message",
+    'es': "🎥 Enviar este comando como respuesta al mensaje",
+    'fr': "🎥 Envoyez cette commande en réponse au message",
+    'zh': "🎥 將此命令作為對消息的回復發送",
+    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
+}
+l_delay_on = {
+    'ru': "👥 Готово! Текущая первичная задержка для <u>новых</u> пользователей (перед написанием их <u>1</u>го сообщ) установлена в значение <u>{0}</u> min",
+    'en': "👥 Ready! Current primary delay for <u>new</u> users (before writing their <u>1</u>st message) is <u>{0}</u> min",
+    'es': "👥 Listo! El retraso principal actual para los <u>nuevos</u> usuarios (antes de escribir su <u>1</u>er mensaje) es <u>{0}</u> min",
+    'fr': "👥 Prêt! Le délai principal actuel pour les <u>nouveaux</u> utilisateurs (avant d'écrire leur <u>1</u>er message) est de <u>{0}</u> min",
+    'zh': "👥 準備好了！<u>新</u>用戶的當前主要延遲（在寫他們的<u>1</u>st消息之前）是<u>{0}</u>分鐘",
+    'ar': "👥 جاهز! التأخير الأساسي الحالي لمستخدمي <u> الجدد </u> (قبل كتابة رسالتهم <u> 1 </u> st) هو <u>{0}</u> min",
+}
+l_delay_off = {
+    'ru': "👥 Режим delay отключен",
+    'en': "👥 Ready! Current primary delay for <u>new</u> users (before writing their <u>1</u>st message) is <u>{0}</u> min",
+    'es': "👥 Listo! El retraso principal actual para los <u>nuevos</u> usuarios (antes de escribir su <u>1</u>er mensaje) es <u>{0}</u> min",
+    'fr': "👥 Prêt! Le délai principal actuel pour les <u>nouveaux</u> utilisateurs (avant d'écrire leur <u>1</u>er message) est de <u>{0}</u> min",
+    'zh': "👥 準備好了！<u>新</u>用戶的當前主要延遲（在寫他們的<u>1</u>st消息之前）是<u>{0}</u>分鐘",
+    'ar': "👥 جاهز! التأخير الأساسي الحالي لمستخدمي <u> الجدد </u> (قبل كتابة رسالتهم <u> 1 </u> st) هو <u>{0}</u> min",
+}
+l_rules_handler = {
+    'ru': "👉🏼 <b>Правила</b> группы <b>{0}</b>:\n\n{1}",
+    'en': "👉🏼 <b>Group rules</b> for <b>{0}</b>:\n\n{1}",
+    'es': "👉🏼 <b>Reglas de grupo</b> para <b>{0}</b>:\n\n{1}",
+    'fr': "👉🏼 <b>Règles de groupe</b> pour <b>{0}</b> :\n\n{1}",
+    'zh': "👉🏼 <b>{0}</b> 的 <b>組規則</b>：\n\n{1}",
+    'ar': "👉🏼 <b> قواعد المجموعة </b> لـ <b>{0}</b>:\n\n{1}",
+}
+l_rules_on = {
+    'ru': "👉🏼 Установлены <u>новые</u> <b>правила</b> для группы <b>{0}</b>:\n\n{1}",
+    'en': "👉🏼 New <u>rules</u> for group<b>{0}</b>:\n\n{1}",
+    'es': "👉🏼 Nuevas <u>reglas</u> para el grupo<b>{0}</b>:\n\n{1}",
+    'fr': "👉🏼 Nouvelles <u>règles</u> pour le groupe<b>{0}</b> :\n\n{1}",
+    'zh': "👉🏼 組<b>{0}</b>的新<u>規則</u>：\n\n{1}",
+    'ar': "👉🏼 قواعد <u> جديدة </u> للمجموعة <b>{0}</b>:\n\n{1}",
+}
+l_rules_off = {
+    'ru': "👉🏼 <b>Правила</b> в группе <b>{0}</b> не установлены. Необходимо <u>ответить на пост</u> с правилами <b>командой</b> /rules",
+    'en': "👉🏼 <b>Group rules</b> for <b>{0}</b> is not configured. You have to <u>reply to message</u> with rules by /rules-<b>command</b>",
+    'es': "👉🏼 <b>Reglas de grupo</b> para <b>{0}</b> no están configuradas. Tienes que <u>responder al mensaje</u> con reglas por /rules-<b>comando</b>",
+    'fr': "👉🏼 Les <b>règles de groupe</b> pour <b>{0}</b> ne sont pas configurées. Vous devez <u>répondre au message</u> avec des règles par /rules-<b>commande</b>",
+    'zh': "👉🏼 <b>{0}</b> 的 <b>組規則</b> 未配置。 您必須通過 /rules-<b>command</b> 使用規則<u>回复消息</u>",
+    'ar': "👉🏼 لم تتم تهيئة <b> قواعد المجموعة </b> لـ <b>{0}</b>. يجب عليك <u> الرد على الرسالة </u> بالقواعد من خلال / rules- <b> أمر </b>",
+}
+# endregion
+
+
+# region ccheck
+l_ccheck_handler = {
+    'ru': "👮🏽 Жми на ✅/🔘, чтобы <b>переключить</b> тип <i>проверки</i> пользователя при <u>вступлении</u> в группу\n\n👉🏼 Для установки имени <b>нажимаемой кнопки</b>, выполни команду: <code>/button {0}</code>\n\n👉🏼 Для <b>проверки подписки</b> на канал <i>добавь</i> @{1}-бота в канал и выполни команду: <code>/channel {2}</code>\n\n👉🏼 Для <i>защиты от атаки</i> на группу включи режим <b>антирейд</b> (блокировка <u>всех</u> вступающих)",
+    'en': "👮🏽 Push the ✅/🔘 to <b>switch</b> <i>Enter control</i> of user <u>joining</u> into group\n\n👉🏼 To set name of <b>pushing button</b> execute command: <code>/button {0}</code>\n\n👉🏼 To check <b>channel-subscription</b> <i>add</i> @{1} to channel and execute command: <code>/channel {2}</code>\n\n👉🏼 To <i>defend</i> from group-attack switch <b>anti-raid</b>-mode (ban <u>everyone</u> who joining)",
+    'es': "👮🏽 Presiona ✅/🔘 para <b>cambiar</b> <i>Enter control</i> del usuario <u>uniéndose</u> al grupo\n\n👉🏼 Para establecer el nombre de <b> presionando el botón</b> ejecute el comando: <code>/button {0}</code>\n\n👉🏼 Para verificar <b>channel-subscription</b> <i>add</i> @{1} para canalizar y ejecutar el comando: <code>/channel {2}</code>\n\n👉🏼 Para <i>defender</i> del ataque grupal, active el modo <b>anti-raid</b> (prohibir a <u>todos</u> que se unan)",
+    'fr': "👮🏽 Appuyez sur ✅/🔘 pour <b>commuter</b> <i>Entrez le contrôle</i> de l'utilisateur <u>rejoignant</u> le groupe\n\n👉🏼 Pour définir le nom de <b> en appuyant sur le bouton</b> exécutez la commande : <code>/button {0}</code>\n\n👉🏼 Pour vérifier <b>channel-subscription</b> <i>add</i> @{1} pour canaliser et exécuter la commande : <code>/channel {2}</code>\n\n👉🏼 Pour <i>se défendre</i> contre une attaque de groupe, activez le mode <b>anti-raid</b> (bannir <u>tous ceux</u> qui se joignent)",
+    'zh': "👮🏽 按下 ✅/🔘 來<b>切換</b> <i>進入控制</i> 用戶<u>加入</u> 入組\n\n👉🏼 設置<b>的名字 按下按鈕</b> 執行命令：<code>/button {0}</code>\n\n👉🏼 檢查<b>頻道訂閱</b> <i>add</i> @{1} 引導並執行命令：<code>/channel {2}</code>\n\n👉🏼 以 <i>defend</i> 免受群攻開啟 <b>anti-raid</b>-mode （禁止加入的<u>每個人</u>）",
+    'ar': "👮🏽 ادفع ✅ / 🔘 إلى <b> التبديل </b> <i> أدخل التحكم </i> للمستخدم <u> المنضم </u> إلى مجموعة \n\n👉🏼 لتعيين اسم <b> ضغط الزر </b> نفذ الأمر: <code> / button {0}</code>\n\n👉🏼 للتحقق من <b> اشتراك القناة </b> <i> إضافة </i> @{1} لتوجيه وتنفيذ الأمر: <code> / channel {2}</code>\n\n👉🏼 <i> للدفاع </i> من هجوم المجموعة ، شغّل وضع <b> anti-raid </b> (حظر <u> كل شخص </u> من ينضم)",
+}
+l_ccheck_add = {
+    'ru': "\n\nВ настройках [Администраторы] вкл для {0}-бота:\n[✅ Удаление сообщ]\n[✅ Блокировка польз]\n[✅ Добавление участ]\n\n🕚Подожди 1min",
+    'en': "\n\nIn the Settings [Administrators] for @{0} enable:\n[✅ Delete Msgs]\n[✅ Ban Users]\n[✅ Invite Users]\n🕚Wait for 1min",
+    'es': "\n\nEn la Configuración [Administradores] para @{0} active:\n[✅ Eliminar mensajes]\n[✅ Prohibir usuarios]\n[✅ Invitar usuarios]\n🕚Espere 1 minuto",
+    'fr': "\n\nDans les paramètres [Administrateurs] pour @{0}, activez :\n[✅ Supprimer les messages]\n[✅ Bannir les utilisateurs]\n[✅ Inviter des utilisateurs]\n🕚Attendez 1 minute",
+    'zh': "\n\n在@{0}的設置[管理員]中打開：\n[✅刪除消息]\n[✅禁止用戶]\n[✅邀請用戶]\n🕚等待1分鐘",
+    'ar': "\n\n في الإعدادات [Administrators] لـ @{0} شغّل:\n [✅ حذف الرسائل] \n على [✅ حظر المستخدمين] \n [✅ دعوة المستخدمين] \n وانتظر لمدة دقيقة واحدة",
+}
+l_ccheck_call_request_on = {
+    'ru': "👮🏽 В настройках [Тип группы] вкл:\n[✅ Заявки на вступление]{0}",
+    'en': "👮🏽 In the Settings [Group Type] enable:\n[✅ Approve New Members]{0}",
+    'es': "👮🏽 En la Configuración [Tipo de grupo] habilite:\n[✅ Aprobar nuevos miembros]{0}",
+    'fr': "👮🏽 Dans les paramètres [Type de groupe], activez :\n[✅ Approuver les nouveaux membres]{0}",
+    'zh': "👮🏽 在設置 [群組類型] 中啟用：\n[✅ 批准新成員]{0}",
+    'ar': "👮🏽 في إعدادات [نوع المجموعة] تمكين: \n [✅ الموافقة على أعضاء جدد] {0}",
+}
+l_ccheck_call_request_off = {
+    'ru': "👮🏽 В настройках [Тип группы] выкл:\n[☑️ Заявки на вступление]{0}",
+    'en': "👮🏽 In the Settings [Group Type] disable:\n[☑️ Approve New Members]{0}",
+    'es': "👮🏽 En la Configuración [Tipo de grupo], deshabilite:\n[☑️ Aprobar nuevos miembros]{0}",
+    'fr': "👮🏽 在設置 [群組類型] 中禁用：\n[☑️ 批准新成員]{0}",
+    'zh': "👮🏽 在設置 [群組類型] 中禁用：\n[☑️ 批准新成員]{0}",
+    'ar': "👮🏽 في إعدادات [نوع المجموعة] تعطيل: \n [☑️ الموافقة على أعضاء جدد] {0}",
+}
+l_ccheck_other_person = {
+    'ru': "👮🏽 Эта кнопка не для тебя",
+    'en': "👮🏽 This button is not for you",
+    'es': "👮🏽 Este botón no es para ti",
+    'fr': "👮🏽 Ce bouton n'est pas pour vous",
+    'zh': "👮🏽 這個按鈕不適合你",
+    'ar': "👮🏽 هذا الزر ليس لك",
+}
+l_ccheckchannel_link = {
+    'ru': "👮🏽 Ссылка на {0} не доступна",
+    'en': "👮🏽 Link for {0} is invalid",
+    'es': "👮🏽 El enlace para {0} no es válido",
+    'fr': "👮🏽 Le lien pour {0} n'est pas valide",
+    'zh': "👮🏽 {0} 的鏈接無效",
+    'ar': "👮🏽 ارتباط {0} غير صالح",
+}
+l_ccheckchannel_chn = {
+    'ru': "👮🏽 Ты не вступил в {0}\n\nПопробуй ещё раз позже",
+    'en': "👮🏽 You are not join to {0}\n\nTry again later",
+    'es': "👮🏽 No te has unido a {0}\n\nInténtalo de nuevo más tarde",
+    'fr': "👮🏽 您沒有加入 {0}\n\n 請稍後再試",
+    'zh': "👮🏽 您沒有加入 {0}\n\n 請稍後再試",
+    'ar': "👮🏽 أنت لست مشتركًا في {0} \n\n حاول مرة أخرى لاحقًا",
+}
+l_ccheck_ban = {
+    'ru': "👮🏽‍ Пользователь {0} не прошел входной контроль и был удален из группы",
+    'en': "👮🏽 User {0} did not pass Enter Control and have been deleted from this group",
+    'es': "👮🏽 El usuario {0} no pasa el control de entrada y ha sido eliminado de este grupo",
+    'fr': "👮🏽 L'utilisateur {0} ne passe pas Enter Control et a été supprimé de ce groupe",
+    'zh': "👮🏽 用戶 {0} 未通過 Enter Control 並已從該組中刪除",
+    'ar': "👮🏽 المستخدم {0} لا يجتاز إدخال التحكم وقد تم حذفه من هذه المجموعة",
+}
+l_ccheckchannel_error = {
+    'ru': "👮🏽 Ошибка проверки",
+    'en': "👮🏽 Error of checking",
+    'es': "👮🏽 Error de verificación",
+    'fr': "👮🏽 Erreur de vérification",
+    'zh': "👮🏽檢查錯誤",
+    'ar': "👮🏽 خطأ في الفحص",
+}
+l_ccheck_wrong = {
+    'ru': "👮🏽 К сожалению, ответ неверный\n\nПопробуйте ещё раз позже",
+    'en': "👮🏽 Unfortunately the answer is not correct\n\nTry again later",
+    'es': "👮🏽 Lamentablemente la respuesta no es correcta\n\nVuelve a intentarlo más tarde",
+    'fr': "👮🏽 Malheureusement, la réponse n'est pas correcte\n\nRéessayez plus tard",
+    'zh': "👮🏽 很遺憾答案不正確\n\n稍後再試",
+    'ar': "👮🏽 للأسف الإجابة غير صحيحة \n\n حاول مرة أخرى لاحقًا",
+}
+l_ccheck_time = {
+    'ru': "👮🏽 Входной контроль пройден за {0} sec",
+    'en': "👮🏽 Enter Control passed for {0} sec",
+    'es': "👮🏽 Control de entrada superado durante {1} seg.",
+    'fr': "👮🏽 Entrez le contrôle passé pendant {1} sec",
+    'zh': "👮🏽 輸入控制已通過 {1} 秒",
+    'ar': "👮🏽 أدخل التحكم الذي تم تمريره لمدة {1} ثانية",
+}
+# endregion
+
+
+# region chello_
+l_chello_call = {
+    'ru': "🔔 Нет ни одного приветствия, необходимо ⚙️Настроить",
+    'en': "🔔 There are no greetings you need to ⚙️Configure",
+    'es': "🔔 No hay saludos que necesites ⚙️Configurar",
+    'fr': "🔔 Vous n'avez pas besoin de salutations ⚙️Configurer",
+    'zh': "🔔無需問候⚙️配置",
+    'ar': "🔔لا توجد تحيات تحتاج إلى تكوين",
+}
+l_chello_your_hello = {
+    'ru': "Ваше приветствие",
+    'en': "Your greeting",
+    'es': "Tu saludo",
+    'fr': "Votre message d'accueil",
+    'zh': "你的問候",
+    'ar': "تحياتك",
+}
+l_chello_text = {
+    'ru': "👋🏽 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> приветствие, а также его ⚙️Настроить\n\n👉🏼 Например, <code>{0}</code>{1}",
+    'en': "👋🏽 Push the ✅/☑️, to <b>On/Off</b> greeting, and to ⚙️Configure\n\n👉🏼 For example, <code>{0}</code>{1}",
+    'es': "👋🏽 Presione ✅/☑️, para <b>Activar/Desactivar</b> el saludo y para ⚙️Configurar\n\n👉🏼 Por ejemplo, <code>{0}</code>{1}",
+    'fr': "👋🏽 Appuyez sur ✅/☑️, sur <b>Activer/Désactiver</b> le message d'accueil et sur ⚙️Configurer\n\n👉🏼 Par exemple, <code>{0}</code>{1}",
+    'zh': "👋🏽 按下 ✅/☑️、<b>On/Off</b> 問候語和 ⚙️Configure\n\n👉🏼 例如，<code>{0}</code>{1}",
+    'ar': "👋🏽 اضغط على ✅ / ☑️ ، من أجل <b> تشغيل / إيقاف </b> الترحيب ، و تكوين \n\n👉🏼 على سبيل المثال ، <code>{0}</code>{1}",
+}
+l_btn_on = {
+    'ru': "✅☑Вкл",
+    'en': "✅☑On",
+    'es': "✅☑En",
+    'fr': "✅☑En",
+    'zh': "✅☑使能夠",
+    'ar': "✅☑ تمكين",
+}
+l_btn_off = {
+    'ru': "☑️☐Выкл",
+    'en': "☑️☐Off",
+    'es': "☑️☐De",
+    'fr': "☑️☐De",
+    'zh': "☑️☐禁用",
+    'ar': "☑️☐ تعطيل",
+}
+l_btn_settings = {
+    'ru': "⚙️Настроить",
+    'en': "⚙️Configure",
+    'es': "⚙️Configurar",
+    'fr': "⚙️Configurer",
+    'zh': "⚙️配置",
+    'ar': "⚙️ تكوين",
+}
+l_chellochange_handler = {
+    'ru': "👋🏽 Отправь мне <b>текст</b>/<b>медиа</b> контент с текстом: фото/гиф/видео/аудио/документ или запиши голосовое/видео-заметку в кружке\n\n👉🏼 Например, <code>{0}</code>",
+    'en': "👋🏽 Send me <b>text</b>/<b>media</b> content with text: photo/giff/video/audio/document or voice/video-note\n\n👉🏼 For example, <code>{0}</code>",
+    'es': "👋🏽 Envíame contenido de <b>texto</b>/<b>medios</b> con texto: photo/giff/video/audio/document or voice/video-note\n\n👉🏼 Par exemple, <code>{0}</code>",
+    'fr': "👋🏽 Envoyez-moi du contenu <b>texte</b>/<b>média</b> avec du texte: photo/giff/video/audio/document or voice/video-note\n\n👉🏼 Par exemple, <code>{0}</code>",
+    'zh': "👋🏽 向我發送帶有文本的 <b>text</b>/<b>media</b> 內容: photo/giff/video/audio/document or voice/video-note\n\n👉🏼 例如, <code>{0}</code>",
+    'ar': "👋🏽 أرسل لي محتوى <b> نصًا </b> / <b> وسائط </b> مع نص: photo/giff/video/audio/document or voice/video-note\n\n👉🏼 فمثلا, <code>{0}</code>",
+}
+l_fsm_hello_finish = {
+    'ru': "👋🏽 Приветствие записано!\n\nОпцию можно включить в настройках [👋🏽Авто-приветствие], нажав [✅☑Вкл]",
+    'en': "👋🏽 Greeting is recorded!\n\nYou can enable this option in the Settings [👋🏽Auto-greeting], by pushing [✅☑On]",
+    'es': "👋🏽 ¡Se graba el saludo!\n\nPuede habilitar esta opción en la Configuración [👋🏽Auto-saludo], presionando [✅☑On]",
+    'fr': "👋🏽 Le message d'accueil est enregistré !\n\nVous pouvez activer cette option dans les paramètres [👋🏽Auto-salutation], en appuyant sur [✅☑On]",
+    'zh': "👋🏽問候語已錄製！\n\n您可以在設置[👋🏽自動問候語]中啟用此選項，方法是按[✅☑On]",
+    'ar': "👋🏽 تم تسجيل الترحيب!\n\n يمكنك تمكين هذا الخيار في الإعدادات [الترحيب التلقائي] ، بالضغط على [تشغيل]",
+}
+# endregion
+
+
+# region cinvite_
+l_cinvite_call = {
+    'ru': "👮🏽 В настройках [Разрешения] вкл опцию:\n\n[✅ Добавление участ]\n\n🕚Подожди 1min",
+    'en': "👮🏽 In the Settings [Permissions] enable:\n\n[✅ Add memebers]\n🕚Wait for 1min",
+    'es': "👮🏽 En la Configuración [Permisos] habilite:\n\n[✅ Agregar miembros]\n🕚Espere 1 minuto",
+    'fr': "👮🏽 Dans les paramètres [Autorisations], activez :\n\n[✅ Ajouter des membres]\n🕚Attendez 1 min",
+    'zh': "👮🏽在設置[權限]中啟用：\n\n[✅添加成員]\n🕚等待1分鐘",
+    'ar': "👮🏽 في الإعدادات [الأذونات] ، قم بتمكين: \n\n [✅ إضافة أعضاء]\n🕚 انتظر لمدة دقيقة واحدة",
+}
+l_cinvite_text_add = {
+    'ru': "\n\n👉🏼 Приглашается <u>{0}</u> пользователей в сутки из группы {1}",
+    'en': "🚶🏽 Push the ✅/☑️, to <b>On/Off</b> auto-inviting users to your group\n\n👉🏼 Inviting <u>{0}</u> users per day from group {1}",
+    'es': "🚶🏽 Presiona ✅/☑️ para <b>activar/desactivar</b> la invitación automática de usuarios a tu grupo\n\n👉🏼 Invitar a <u>{0}</u> usuarios por día del grupo {1}",
+    'fr': "🚶🏽 Appuyez sur ✅/☑️, pour <b>Activer/Désactiver</b> l'invitation automatique d'utilisateurs dans votre groupe\n\n👉🏼 Inviter <u>{0}</u> utilisateurs par jour à partir du groupe {1}",
+    'zh': "🚶🏽 按下 ✅/☑️, 以<b>開/關</b>自動邀請用戶加入您的群組\n\n👉🏼 每天從群組 {1} 中邀請 <u>{0}</u> 個用戶",
+    'ar': "🚶🏽 ادفع ✅ / ☑️ إلى <b> تشغيل / إيقاف </b> لدعوة المستخدمين تلقائيًا إلى مجموعتك \n\n👉🏼 دعوة <u>{0}</u> مستخدمين يوميًا من المجموعة {1}",
+}
+l_cinvite_text = {
+    'ru': "🚶🏽 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-инвайт пользователей в <b>{0}</b>-группу\n\n👩🏽‍💻 <b>Текущие</b> настройки авто-рассылки: {1}",
+    'en': "🚶🏽 Push the ✅/☑️, to <b>On/Off</b> auto-inviting users to your group\n\n👉🏼 Inviting <u>{0}</u> users per day from group {1}",
+    'es': "🚶🏽 Presiona ✅/☑️ para <b>activar/desactivar</b> la invitación automática de usuarios a tu grupo\n\n👉🏼 Invitar a <u>{0}</u> usuarios por día del grupo {1}",
+    'fr': "🚶🏽 Appuyez sur ✅/☑️, pour <b>Activer/Désactiver</b> l'invitation automatique d'utilisateurs dans votre groupe\n\n👉🏼 Inviter <u>{0}</u> utilisateurs par jour à partir du groupe {1}",
+    'zh': "🚶🏽 按下 ✅/☑️, 以<b>開/關</b>自動邀請用戶加入您的群組\n\n👉🏼 每天從群組 {1} 中邀請 <u>{0}</u> 個用戶",
+    'ar': "🚶🏽 ادفع ✅ / ☑️ إلى <b> تشغيل / إيقاف </b> لدعوة المستخدمين تلقائيًا إلى مجموعتك \n\n👉🏼 دعوة <u>{0}</u> مستخدمين يوميًا من المجموعة {1}",
+}
+
+l_cinvite_current = {
+    'ru': "🚶🏽 <b>Текущие</b> настройки авто-инвайта в группу:\n\n<u>{0}</u> пользователей/сутки\n<u>{1}</u> источник",
+    'en': "🚶🏽 Send <b>link</b> to userbot as source for new members\n\n👉🏼 For example, <code>https://t.me/likeconcentrat</code> - push the link to copy",
+    'es': "🚶🏽 Envía <b>enlace</b> al grupo como fuente para nuevos miembros\n\n👉🏼 Por ejemplo, <code>https://t.me/likeconcentrat</code> - presiona el enlace para copiar",
+    'fr': "🚶🏽 Envoyez <b>lien</b> au userbote comme source pour les nouveaux membres\n\n👉🏼 Par exemple, <code>https://t.me/likeconcentrat</code> - appuyez sur le lien pour le copier",
+    'zh': "🚶🏽 將 <b>link</b> 發送到群組作為新成員的來源\n\n👉🏼 例如，<code>https://t.me/likeconcentrat</code> - 推送鏈接以進行複制",
+    'ar': "📨️ أرسل <b> ارتباط </b> للمجموعة كمصدر للأعضاء الجدد \n\n👉🏼 على سبيل المثال ، <code> https://t.me/likeconcentrat </code> - ادفع الرابط للنسخ",
+}
+l_cinvite_cnt = {
+    'ru': "{0} польз/сутки",
+    'en': "Send <b>link</b> to userbot as source for new members\n\n👉🏼 For example, <code>https://t.me/likeconcentrat</code> - push the link to copy",
+    'es': "Envía <b>enlace</b> al grupo como fuente para nuevos miembros\n\n👉🏼 Por ejemplo, <code>https://t.me/likeconcentrat</code> - presiona el enlace para copiar",
+    'fr': "Envoyez <b>lien</b> au userbote comme source pour les nouveaux membres\n\n👉🏼 Par exemple, <code>https://t.me/likeconcentrat</code> - appuyez sur le lien pour le copier",
+    'zh': "將 <b>link</b> 發送到群組作為新成員的來源\n\n👉🏼 例如，<code>https://t.me/likeconcentrat</code> - 推送鏈接以進行複制",
+    'ar': "📨️ أرسل <b> ارتباط </b> للمجموعة كمصدر للأعضاء الجدد \n\n👉🏼 على سبيل المثال ، <code> https://t.me/likeconcentrat </code> - ادفع الرابط للنسخ",
+}
+l_cinvite_src = {
+    'ru': "{0} источник",
+    'en': "Send <b>link</b> to userbot as source for new members\n\n👉🏼 For example, <code>https://t.me/likeconcentrat</code> - push the link to copy",
+    'es': "Envía <b>enlace</b> al grupo como fuente para nuevos miembros\n\n👉🏼 Por ejemplo, <code>https://t.me/likeconcentrat</code> - presiona el enlace para copiar",
+    'fr': "Envoyez <b>lien</b> au userbote comme source pour les nouveaux membres\n\n👉🏼 Par exemple, <code>https://t.me/likeconcentrat</code> - appuyez sur le lien pour le copier",
+    'zh': "將 <b>link</b> 發送到群組作為新成員的來源\n\n👉🏼 例如，<code>https://t.me/likeconcentrat</code> - 推送鏈接以進行複制",
+    'ar': "📨️ أرسل <b> ارتباط </b> للمجموعة كمصدر للأعضاء الجدد \n\n👉🏼 على سبيل المثال ، <code> https://t.me/likeconcentrat </code> - ادفع الرابط للنسخ",
+}
+l_cinvitechange_handler = {
+    'ru': "🚶🏽 Пришли мне <b>ссылку</b> на группу, откуда будем брать подписчиков\n\n👉🏼 Например, <code>https://t.me/likeconcentrat</code> - жми на ссылку, чтобы скопировать",
+    'en': "🚶🏽 Send <b>link</b> to group as source for new members\n\n👉🏼 For example, <code>https://t.me/likeconcentrat</code> - push the link to copy",
+    'es': "🚶🏽 Envía <b>enlace</b> al grupo como fuente para nuevos miembros\n\n👉🏼 Por ejemplo, <code>https://t.me/likeconcentrat</code> - presiona el enlace para copiar",
+    'fr': "🚶🏽 Envoyez <b>lien</b> au groupe comme source pour les nouveaux membres\n\n👉🏼 Par exemple, <code>https://t.me/likeconcentrat</code> - appuyez sur le lien pour le copier",
+    'zh': "🚶🏽 將 <b>link</b> 發送到群組作為新成員的來源\n\n👉🏼 例如，<code>https://t.me/likeconcentrat</code> - 推送鏈接以進行複制",
+    'ar': "🚶🏽 أرسل <b> ارتباط </b> للمجموعة كمصدر للأعضاء الجدد \n\n👉🏼 على سبيل المثال ، <code> https://t.me/likeconcentrat </code> - ادفع الرابط للنسخ",
+}
+l_correct_link = {
+    'ru': "👩🏽‍💻 Вставь корректную ссылку или повтори операцию",
+    'en': "👩🏽‍💻 Send correct link or try again later",
+    'es': "👩🏽‍💻 Envíe el enlace correcto o vuelva a intentarlo más tarde",
+    'fr': "👩🏽‍💻 Envoyez le lien correct ou réessayez plus tard",
+    'zh': "👩🏽‍💻 發送正確的鏈接或稍後再試",
+    'ar': "👩🏽‍💻 أرسل الرابط الصحيح أو حاول مرة أخرى لاحقًا",
+}
+l_admin_require = {
+    'ru': "🔺 Требуются права админа",
+    'en': "👩🏽‍💻 Send correct link or try again later",
+    'es': "👩🏽‍💻 Envíe el enlace correcto o vuelva a intentarlo más tarde",
+    'fr': "👩🏽‍💻 Envoyez le lien correct ou réessayez plus tard",
+    'zh': "👩🏽‍💻 發送正確的鏈接或稍後再試",
+    'ar': "👩🏽‍💻 أرسل الرابط الصحيح أو حاول مرة أخرى لاحقًا",
+}
+l_group_not_channel = {
+    'ru': "🚶🏽 Вставь ссылку на группу, а не канал",
+    'en': "🚶🏽 Send group-link, not channel-link",
+    'es': "🚶🏽 Enviar enlace de grupo, no enlace de canal",
+    'fr': "🚶🏽 Envoyer un lien de groupe, pas un lien de chaîne",
+    'zh': "🚶🏽 發送群組鏈接，而不是頻道鏈接",
+    'ar': "🚶🏽 أرسل رابط المجموعة ، وليس رابط القناة",
+}
+l_no_participants = {
+    'ru': "🚶🏽 Нет доступных подписчиков",
+    'en': "🚶🏽 No available subscribers",
+    'es': "🚶🏽 No hay suscriptores disponibles",
+    'fr': "🚶🏽 Aucun abonné disponible",
+    'zh': "🚶🏽 沒有可用的訂閱者",
+    'ar': "🚶🏽 لا يوجد مشتركون متاحون",
+}
+l_current_participants = {
+    'ru': "🚶🏽 Для {0}<b>текущее количество</b> реальных подписчиков: <u>{1}</u>\n\n▪️ Введи <i>число</i> подписчиков, которое необходимо подписывать <b>ежедневно</b> от 1 до 3 (без подписки +{2}):",
+    'en': "🚶🏽 For {0}<b>current number</b> of real members: <u>{1}</u>\n\n▪️ Enter <i>number</i> of members to subscribe <b>everyday</b> from 1 to 3 (without subscription +{2}):",
+    'es': "🚶🏽 Para {0}<b>número actual</b> de miembros reales: <u>{1}</u>\n\n▪️ Ingrese <i>número</i> de miembros para suscribirse <b>todos los días </b> del 1 al 3 (sin suscripción +{2}):",
+    'fr': "🚶🏽 Pour {0}<b>nombre actuel</b> de membres réels : <u>{1}</u>\n\n▪️ Saisissez le <i>nombre</i> de membres à souscrire <b>tous les jours </b> de 1 à 3 (sans abonnement +{2}) :",
+    'zh': "🚶🏽 {0}<b>當前人數</b> 的真實會員：<u>{1}</u>\n\n▪️ 輸入 <i>會員人數</i> 以訂閱<b>每天 </b> 從 1 到 3（無訂閱 +{2}）：",
+    'ar': "🚶🏽 بالنسبة إلى {0}<b> العدد الحالي </b> للأعضاء الحقيقيين: <u>{1}</u> \n\n▪️ أدخل <i> عدد </i> من الأعضاء للاشتراك <b> كل يوم </b> من 1 إلى 3 (بدون اشتراك + {2}):",
+}
+l_everyday_participants = {
+    'ru': "🚶🏽 Введи количество пользователей для ежедневной подписки от 1 до 3 включительно",
+    'en': "🚶🏽 Enter number of users for everyday inviting from 1 to 3",
+    'es': "🚶🏽 Ingrese el número de usuarios para invitar todos los días de 1 a 3",
+    'fr': "🚶🏽 Entrez le nombre d'utilisateurs pour l'invitation quotidienne de 1 à 3",
+    'zh': "🚶🏽 輸入每天邀請的用戶數，從 1 到 3",
+    'ar': "🚶🏽 أدخل عدد المستخدمين للدعوة اليومية من 1 إلى 3",
+}
+l_invite_need_subscribe = {
+    'ru': "🚶🏽 Для инвайта > 1 пользователя в день необходимо приобрести подписку. Оформи подписку или введи 1:",
+    'en': "🚶🏽 For inviting > 1 members per day you have to subscribe or type 1:",
+    'es': "🚶🏽 Para invitar > 1 miembros por día tienes que suscribirte o escribir 1:",
+    'fr': "🚶🏽 Pour inviter > 1 membres par jour il faut s'inscrire ou taper 1 :",
+    'zh': "🚶🏽 每天邀請 > 1 個成員，您必須訂閱或輸入 1：",
+    'ar': "🚶🏽 لدعوة> عضو واحد يوميًا ، يجب عليك الاشتراك أو اكتب 1:",
+}
+l_invite_correct_num = {
+    'ru': "🚶🏽 Введи корректное число",
+    'en': "🚶🏽 Enter correct number",
+    'es': "🚶🏽 Ingrese el número correcto",
+    'fr': "🚶🏽 Entrez le bon numéro",
+    'zh': "🚶輸入正確的數字",
+    'ar': "🚶🏽 Enter correct number",
+}
+l_fsm_invite_finish = {
+    'ru': "🚶🏽 Готово! Настроен <b>авто</b>-инвайт <u>{0}</u> пользователей в сутки из группы {1}",
+    'en': "🚶🏽 Ready! <b>Auto</b>-inviting <u>{0}</u> users per day from group {1}",
+    'es': "🚶🏽 Listo! Invitación <b>automática</b> a <u>{0}</u> usuarios por día del grupo {1}",
+    'fr': "🚶🏽 Prêt ! <b>Auto</b>-inviter <u>{0}</u> utilisateurs par jour du groupe {1}",
+    'zh': "🚶🏽 準備好了！ <b>自動</b>-每天從組 {1} 中邀請 <u>{0}</u> 個用戶",
+    'ar': "🚶🏽 جاهز! <b> دعوة تلقائية </b> <u>{0}</u> للمستخدمين يوميًا من المجموعة {1}",
+}
+l_cinvite_nosrc = {
+    'ru': "🚶🏽 Не задан источник для инвайта пользователей в группу",
+    'en': "🚶🏽 Ready! <b>Auto</b>-inviting <u>{0}</u> users per day from group {1}",
+    'es': "🚶🏽 Listo! Invitación <b>automática</b> a <u>{0}</u> usuarios por día del grupo {1}",
+    'fr': "🚶🏽 Prêt ! <b>Auto</b>-inviter <u>{0}</u> utilisateurs par jour du groupe {1}",
+    'zh': "🚶🏽 準備好了！ <b>自動</b>-每天從組 {1} 中邀請 <u>{0}</u> 個用戶",
+    'ar': "🚶🏽 جاهز! <b> دعوة تلقائية </b> <u>{0}</u> للمستخدمين يوميًا من المجموعة {1}",
+}
+l_cinvite_group = {
+    'ru': "🚶🏽 Группа",
+    'en': "🚶🏽 Ready! <b>Auto</b>-inviting <u>{0}</u> users per day from group {1}",
+    'es': "🚶🏽 Listo! Invitación <b>automática</b> a <u>{0}</u> usuarios por día del grupo {1}",
+    'fr': "🚶🏽 Prêt ! <b>Auto</b>-inviter <u>{0}</u> utilisateurs par jour du groupe {1}",
+    'zh': "🚶🏽 準備好了！ <b>自動</b>-每天從組 {1} 中邀請 <u>{0}</u> 個用戶",
+    'ar': "🚶🏽 جاهز! <b> دعوة تلقائية </b> <u>{0}</u> للمستخدمين يوميًا من المجموعة {1}",
+}
+l_cinvite_file = {
+    'ru': "🚶🏽 Файл",
+    'en': "🚶🏽 Ready! <b>Auto</b>-inviting <u>{0}</u> users per day from group {1}",
+    'es': "🚶🏽 Listo! Invitación <b>automática</b> a <u>{0}</u> usuarios por día del grupo {1}",
+    'fr': "🚶🏽 Prêt ! <b>Auto</b>-inviter <u>{0}</u> utilisateurs par jour du groupe {1}",
+    'zh': "🚶🏽 準備好了！ <b>自動</b>-每天從組 {1} 中邀請 <u>{0}</u> 個用戶",
+    'ar': "🚶🏽 جاهز! <b> دعوة تلقائية </b> <u>{0}</u> للمستخدمين يوميًا من المجموعة {1}",
+}
+l_cinvite_geo = {
+    'ru': "🚶🏽 Гео",
+    'en': "🚶🏽 Ready! <b>Auto</b>-inviting <u>{0}</u> users per day from group {1}",
+    'es': "🚶🏽 Listo! Invitación <b>automática</b> a <u>{0}</u> usuarios por día del grupo {1}",
+    'fr': "🚶🏽 Prêt ! <b>Auto</b>-inviter <u>{0}</u> utilisateurs par jour du groupe {1}",
+    'zh': "🚶🏽 準備好了！ <b>自動</b>-每天從組 {1} 中邀請 <u>{0}</u> 個用戶",
+    'ar': "🚶🏽 جاهز! <b> دعوة تلقائية </b> <u>{0}</u> للمستخدمين يوميًا من المجموعة {1}",
+}
+l_cinvite_choose_src = {
+    'ru': "🚶🏽 Выбери <b>источник</b>, откуда будем брать @username для авто-инвайта",
+    'en': "🚶🏽 Ready! <b>Auto</b>-inviting <u>{0}</u> users per day from group {1}",
+    'es': "🚶🏽 Listo! Invitación <b>automática</b> a <u>{0}</u> usuarios por día del grupo {1}",
+    'fr': "🚶🏽 Prêt ! <b>Auto</b>-inviter <u>{0}</u> utilisateurs par jour du groupe {1}",
+    'zh': "🚶🏽 準備好了！ <b>自動</b>-每天從組 {1} 中邀請 <u>{0}</u> 個用戶",
+    'ar': "🚶🏽 جاهز! <b> دعوة تلقائية </b> <u>{0}</u> للمستخدمين يوميًا من المجموعة {1}",
+}
+l_cinvite_choose_cnt = {
+    'ru': "🚶🏽 Введи <b>количество</b> пользователей для авто-инвайта, которые будут приглашаться ежедневно (без подписки: 1 польз)",
+    'en': "🚶🏽 Ready! <b>Auto</b>-inviting <u>{0}</u> users per day from group {1}",
+    'es': "🚶🏽 Listo! Invitación <b>automática</b> a <u>{0}</u> usuarios por día del grupo {1}",
+    'fr': "🚶🏽 Prêt ! <b>Auto</b>-inviter <u>{0}</u> utilisateurs par jour du groupe {1}",
+    'zh': "🚶🏽 準備好了！ <b>自動</b>-每天從組 {1} 中邀請 <u>{0}</u> 個用戶",
+    'ar': "🚶🏽 جاهز! <b> دعوة تلقائية </b> <u>{0}</u> للمستخدمين يوميًا من المجموعة {1}",
+}
+l_cinvite_choose_group = {
+    'ru': "🚶🏽 Отправь <b>ссылку</b> на группу, чтобы сделать авто-инвайт по ее @username\n\n👩🏽‍💻 Например, @ferey_group_english",
+    'en': "🚶🏽 Ready! <b>Auto</b>-inviting <u>{0}</u> users per day from group {1}",
+    'es': "🚶🏽 Listo! Invitación <b>automática</b> a <u>{0}</u> usuarios por día del grupo {1}",
+    'fr': "🚶🏽 Prêt ! <b>Auto</b>-inviter <u>{0}</u> utilisateurs par jour du groupe {1}",
+    'zh': "🚶🏽 準備好了！ <b>自動</b>-每天從組 {1} 中邀請 <u>{0}</u> 個用戶",
+    'ar': "🚶🏽 جاهز! <b> دعوة تلقائية </b> <u>{0}</u> للمستخدمين يوميًا من المجموعة {1}",
+}
+l_cinvite_choose_file = {
+    'ru': "🚶🏽 Отправь текстовый <b>файл</b> со списком @username, чтобы сделать по ним авто-инвайт",
+    'en': "🚶🏽 Ready! <b>Auto</b>-inviting <u>{0}</u> users per day from group {1}",
+    'es': "🚶🏽 Listo! Invitación <b>automática</b> a <u>{0}</u> usuarios por día del grupo {1}",
+    'fr': "🚶🏽 Prêt ! <b>Auto</b>-inviter <u>{0}</u> utilisateurs par jour du groupe {1}",
+    'zh': "🚶🏽 準備好了！ <b>自動</b>-每天從組 {1} 中邀請 <u>{0}</u> 個用戶",
+    'ar': "🚶🏽 جاهز! <b> دعوة تلقائية </b> <u>{0}</u> للمستخدمين يوميًا من المجموعة {1}",
+}
+l_cinvite_choose_geo = {
+    'ru': "🚶🏽 Отправь <b>геопозицию</b>, чтобы получить гео-@username для авто-инвайта",
+    'en': "🚶🏽 Ready! <b>Auto</b>-inviting <u>{0}</u> users per day from group {1}",
+    'es': "🚶🏽 Listo! Invitación <b>automática</b> a <u>{0}</u> usuarios por día del grupo {1}",
+    'fr': "🚶🏽 Prêt ! <b>Auto</b>-inviter <u>{0}</u> utilisateurs par jour du groupe {1}",
+    'zh': "🚶🏽 準備好了！ <b>自動</b>-每天從組 {1} 中邀請 <u>{0}</u> 個用戶",
+    'ar': "🚶🏽 جاهز! <b> دعوة تلقائية </b> <u>{0}</u> للمستخدمين يوميًا من المجموعة {1}",
+}
+l_cinvite_csv_table = {
+    'ru': "🚶🏽 В csv-файле @username или ссылка должны быть в 3м столбце",
+    'en': "🚶🏽 Ready! <b>Auto</b>-inviting <u>{0}</u> users per day from group {1}",
+    'es': "🚶🏽 Listo! Invitación <b>automática</b> a <u>{0}</u> usuarios por día del grupo {1}",
+    'fr': "🚶🏽 Prêt ! <b>Auto</b>-inviter <u>{0}</u> utilisateurs par jour du groupe {1}",
+    'zh': "🚶🏽 準備好了！ <b>自動</b>-每天從組 {1} 中邀請 <u>{0}</u> 個用戶",
+    'ar': "🚶🏽 جاهز! <b> دعوة تلقائية </b> <u>{0}</u> للمستخدمين يوميًا من المجموعة {1}",
+}
+l_cinvite_csv_file = {
+    'ru': "🚶🏽 Пришли корректный текстовый <b>файл</b> со списком @username",
+    'en': "🚶🏽 Ready! <b>Auto</b>-inviting <u>{0}</u> users per day from group {1}",
+    'es': "🚶🏽 Listo! Invitación <b>automática</b> a <u>{0}</u> usuarios por día del grupo {1}",
+    'fr': "🚶🏽 Prêt ! <b>Auto</b>-inviter <u>{0}</u> utilisateurs par jour du groupe {1}",
+    'zh': "🚶🏽 準備好了！ <b>自動</b>-每天從組 {1} 中邀請 <u>{0}</u> 個用戶",
+    'ar': "🚶🏽 جاهز! <b> دعوة تلقائية </b> <u>{0}</u> للمستخدمين يوميًا من المجموعة {1}",
+}
+l_cinvite_src_empty = {
+    'ru': "🚶🏽 В источнике {0} закончились пользователи для подписки на группу {1}",
+    'en': "🚶🏽 Ready! <b>Auto</b>-inviting <u>{0}</u> users per day from group {1}",
+    'es': "🚶🏽 Listo! Invitación <b>automática</b> a <u>{0}</u> usuarios por día del grupo {1}",
+    'fr': "🚶🏽 Prêt ! <b>Auto</b>-inviter <u>{0}</u> utilisateurs par jour du groupe {1}",
+    'zh': "🚶🏽 準備好了！ <b>自動</b>-每天從組 {1} 中邀請 <u>{0}</u> 個用戶",
+    'ar': "🚶🏽 جاهز! <b> دعوة تلقائية </b> <u>{0}</u> للمستخدمين يوميًا من المجموعة {1}",
+}
+l_cinvite_choose = {
+    'ru': "Выбрать",
+    'en': "Ready! <b>Auto</b>-inviting <u>{0}</u> users per day from group {1}",
+    'es': "Listo! Invitación <b>automática</b> a <u>{0}</u> usuarios por día del grupo {1}",
+    'fr': "Prêt ! <b>Auto</b>-inviter <u>{0}</u> utilisateurs par jour du groupe {1}",
+    'zh': "準備好了！ <b>自動</b>-每天從組 {1} 中邀請 <u>{0}</u> 個用戶",
+    'ar': "🚶🏽 جاهز! <b> دعوة تلقائية </b> <u>{0}</u> للمستخدمين يوميًا من المجموعة {1}",
+}
+# endregion
+
+
+# region csystem_
+l_csystem_text = {
+    'ru': "👣 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> <i>системные</i> сообщения\n\n👉🏼 Например, <i>Пользователь вступил(а) в группу</i>",
+    'en': "👣 Push the ✅/☑️, to <b>On/Off</b> <i>system</i> messages\n\n👉🏼 For example, <i>User joined the group</i>",
+    'es': "👣 Presiona ✅/☑️, para <b>Encender/Apagar</b> <i>sistema</i> mensajes\n\n👉🏼 Por ejemplo, <i>Usuario se unió al grupo</i>",
+    'fr': "👣 Appuyez sur ✅/☑️, pour <b>Activer/Désactiver</b> les messages <i>système</i>\n\n👉🏼 Par exemple, <i>L'utilisateur a rejoint le groupe</i>",
+    'zh': "👣 將 ✅/☑️ 推送到 <b>On/Off</b> <i>system</i> 消息\n\n👉🏼 例如，<i>用戶加入群組</i>",
+    'ar': "👣 اضغط على ✅ / ☑️ ، إلى رسائل <b> تشغيل / إيقاف </b> <i> النظام </i>\n\n👉🏼 على سبيل المثال ، <i> انضم المستخدم إلى المجموعة </i>",
+}
+# endregion
+
+
+# region cchannel_
+l_cchannel_text = {
+    'ru': "🫥 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> <i>возможность</i> пользователю в группе писать <i>анонимно</i> (от имени <b>его</b> канала)",
+    'en': "🫥 Push the ✅/☑️, to <b>On/Off</b> <i>opportunity</i> for users in group to write <i>anonymously</i> (from name of <b>his</b> channel)",
+    'es': "🫥 Presiona ✅/☑️ para <b>Activar/Desactivar</b> <i>oportunidad</i> para que los usuarios del grupo escriban <i>anónimamente</i> (del nombre de <b>su</b> canal)",
+    'fr': "🫥 Poussez le ✅/☑️, sur <b>On/Off</b> <i>opportunité</i> pour les utilisateurs du groupe d'écrire <i>anonymement</i> (du nom de <b>son</b> canal)",
+    'zh': "🫥 將 ✅/☑️ 推到 <b>On/Off</b> <i>機會</i> 讓群組中的用戶<i>匿名</i> （來自<b>他的名字</b> 頻道）",
+    'ar': "🫥 اضغط على ✅/☑️ ، من أجل <b> تشغيل / إيقاف </b> <i> فرصة </i> للمستخدمين في المجموعة لكتابة <i> مجهول </i> (من اسم <b> الخاص به </b> قناة)",
+}
+
+# endregion
+
+
+# region clink_
+l_clink_text = {
+    'ru': "🔗 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> <i>внешние <b>ссылки</b>/telegram-<b>ссылки</b>/forward</i>-<b>ссылки</b>\n\n👉🏼 Например, [✅☑Вкл forward-ссылки] означает разрешение на <b>forward-пересылку</b> сообщений из <u>других</u> Telegram-<i>каналов/групп/аккаунтов</i> в <u>нашу</u> группу",
+    'en': "🔗 Push the ✅/☑️, to <b>On/Off</b> <i>externak <b>links</b>/telegram-<b>links</b>/forward</i>-<b>links</b>\n\n👉🏼 For example, [✅☑On forward-links] means permission on <b>forward</b> messages from <u>other</u> Telegram-<i>channels/groups/accounts</i> into <u>our</u> group",
+    'es': "🔗 Presiona ✅/☑️ para <b>Activar/Desactivar</b> <i>externak <b>enlaces</b>/telegram-<b>enlaces</b>/reenviar</i>-<b>enlaces</b>\n\n👉🏼 Por ejemplo, [✅☑On forward-links] significa permiso en <b>reenviar</b> mensajes de <u>otros</u> Telegram-<i>canales /grupos/cuentas</i> en <u>nuestro</u> grupo",
+    'fr': "🔗 Appuyez sur le ✅/☑️, sur <b>On/Off</b> <i>externak <b>links</b>/telegram-<b>links</b>/forward</i>-<b>liens</b>\n\n👉🏼 Par exemple, [✅☑On forward-links] signifie l'autorisation de <b>transférer</b> les messages provenant d'<u>autres</u> chaînes Telegram-<i> /groupes/comptes</i> dans <u>notre</u> groupe",
+    'zh': "🔗 將 ✅/☑️ 推到 <b>On/Off</b> <i>externak <b>links</b>/telegram-<b>links</b>/forward</i>-<b>links</b>\n\n👉🏼 例如，[✅☑On forward-links] 表示允許 <b>forward</b> 來自 <u>other</u> Telegram-<i> 頻道的消息 /groups/accounts</i> 進入 <u>我們的</u> 組",
+    'ar': "🔗 ادفع ✅ / ☑️ إلى تشغيل / إيقاف روابط خارجية telegram- روابط/ إعادة توجيه الروابط \n\n👉🏼 على سبيل المثال ، [على روابط إعادة التوجيه] تعني إذنًا بشأن <b> إعادة توجيه </b> الرسائل من أخرى Telegram قنوات/groups/accounts في مجموعتنا",
+}
+l_clink_http_on = {
+    'ru': "✅☑Вкл внешние-ссылки",
+    'en': "✅☑On external links",
+    'es': "✅☑En enlaces externos",
+    'fr': "✅☑En Liens externes",
+    'zh': "✅☑使能夠 外部鏈接",
+    'ar': "✅☑ يُمكَِن روابط خارجية",
+}
+l_clink_http_off = {
+    'ru': "☑️☐Выкл внешние-ссылки",
+    'en': "☑️☐Off external links",
+    'es': "☑️☐De enlaces externos",
+    'fr': "☑️☐De Liens externes",
+    'zh': "☑️☐禁用 外部鏈接",
+    'ar': "☑️☐ تعطيل روابط خارجية",
+}
+l_clink_telegram_on = {
+    'ru': "✅☑Вкл @telegram-ссылки",
+    'en': "✅☑On @telegram links",
+    'es': "✅☑En enlaces @telegram",
+    'fr': "✅☑En Liens @telegram",
+    'zh': "✅☑使能夠 @telegram-鏈接",
+    'ar': "✅☑ يُمكَِن @telegram-الروابط",
+}
+l_clink_telegram_off = {
+    'ru': "☑️☐Выкл @telegram-ссылки",
+    'en': "☑️☐Off @telegram-links",
+    'es': "☑️☐De @telegram-enlaces",
+    'fr': "☑️☐De @telegram-Liens",
+    'zh': "☑️☐禁用 @telegram-鏈接",
+    'ar': "☑️☐ تعطيل @telegram-الروابط",
+}
+l_clink_forward_on = {
+    'ru': "✅☑Вкл forward-ссылки",
+    'en': "✅☑On forward-links",
+    'es': "✅☑En forward-enlaces",
+    'fr': "✅☑En forward-Liens",
+    'zh': "✅☑使能夠 forward-鏈接",
+    'ar': "✅☑ يُمكَِن forward-الروابط",
+}
+l_clink_forward_off = {
+    'ru': "☑️☐Выкл forward-ссылки",
+    'en': "☑️☐Off forward-links",
+    'es': "☑️☐De forward-enlaces",
+    'fr': "☑️☐De forward-Liens",
+    'zh': "☑️☐禁用 forward-鏈接",
+    'ar': "☑️☐ تعطيل forward-الروابط",
+}
+# endregion
+
+
+# region csymbol_
+l_csymbol_text = {
+    'ru': "文 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> <u>авто</u>-бан <i>слов с 文-глиф, ب-араб, <a href='https://www.zalgo.org'>zalgo-символами</a></i>\n\n👉🏼 Например, опция <b>zalgo-бан</b> удаляет сообщения такого вида <i>h̴̢̝̱̜͓̠̮̪̞͓͚̦͓͆͗̅̎̂͑̃̋͜e̷̡̧͙̹̥͓̣͍̰̮͙̻͍̐͒̒̍̈́̒̎̅̈́ḻ̸̨̢̘̥͛̈́̔̀̇̏̈́̂̎͠l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆̕͜͝ô̶͍̼͎͈̬̩̩̰̱͙̒͗͐̊̐̐͛̾́͗̈́̚͝͝ͅ</i>",
+    'en': "文 Push the ✅/☑️, to <b>On/Off</b> <u>auto</u>-ban <i>words with 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👉🏼 For example, the option <b>zalgo-ban</b> delete messages <i>h̴̢̝̱̜͓̠̮̪̞͓͚̦͓͆͗̅̎̂͑̃̋͜e̷̡̧͙̹̥͓̣͍̰̮͙̻͍̐͒̒̍̈́̒̎̅̈́ḻ̸̨̢̘̥͛̈́̔̀̇̏̈́̂̎͠l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆̕͜͝ô̶͍̼͎͈̬̩̩̰̱͙̒͗͐̊̐̐͛̾́͗̈́̚͝͝ͅ</i>",
+    'es': "文 Presione ✅/☑️, para <b>Encender/Apagar</b> <u>automático</u>-prohibir <i>palabras con 文-glif, ب-arab, <a href='https://www.zalgo.org'>Zalgo-Symbols</a></i>\n\n👉🏼 Por ejemplo, la opción <b>Zalgo-ban</b> Eliminar mensajes <i>h̴̢̝̱̜͓̠̮̪̞͓͚̦͓͆͗̅̎̂͑̃̋͜e̷̡̧͙̹̥͓̣͍̰̮͙̻͍̐͒̒̍̈́̒̎̅̈́ḻ̸̷̨̢̡̧̘̥͙̹̥͓̣͍̰̮͙̻͍͛̈́̔̀̐͒̒̍̈́̒̎̅̈́ḻ̸̨̢̘̥͛̈́̔̀l̶̶̡̡̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆̔̀̾̾͛͑́̏͆̕̕͜͜͝͝</i>",
+    'fr': "文 Appuyez sur ✅/☑️, pour <b>On/Off</b> <u>auto</u>-bannir <i>les mots avec 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👉🏼 Par exemple, l'option <b>zalgo-ban</b> supprimer les messages <i>h̴̢̝̱̜͓̠̮̪̞͓͚̦͓͆͗̅̎̂͑̃̋͜e̷̡̧͙̹̥͓̣͍̰̮͙̻͍̐͒̒̍̈́̒̎̅̈́ḻ̸̷̨̢̡̧̘̥͙̹̥͓̣͍̰̮͙̻͍͛̈́̔̀̐͒̒̍̈́̒̎̅̈́ḻ̸̨̢̘̥͛̈́̔̀l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆̕͜͝ô̶͍̼͎͈̬̩̩̰̱͙̒͗͐̊̐̐͛̾́͗̈́̚͝͝ͅ</i>",
+    'zh': "文推 ✅/☑️, 到 <b>On/Off</b> <u>auto</u>-ban <i>words with 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👉🏼 例如，選項<b>zalgo-ban</b>刪除消息",
+    'ar': "文 اضغط على ✅ / ☑️ ، من أجل تشغيل / إيقاف تلقائي - حظر الكلمات التي تحتوي على -glif ، ب- arab ، <a href ='https://www.zalgo.org'>رموز zalgo</a>\n\n👉🏼 على سبيل المثال ، الخيار <b>zalgo-ban</b> يحذف الرسائل h̴̢̝̱̜͓̠̮̪̞͓͚̦͓͆͗̅̎̂͑̃̋͜e̷̡̧͙̹̥͓̣͍̰̮͙̻͍̐͒̒̍̈́̒̎̅̈́ḻ̸̨̢̘̥͛̈́̔̀̇̏̈́̂̎͠l̶̡̡͖͚̥͇͙͈̜̲͚̼̻͇͙̹̔̀̾̾͛͑́̏͆̕͜͝ô̶͍̼͎͈̬̩̩̰̱͙̒͗͐̊̐̐͛̾́͗̈́̚͝͝ͅ",
+}
+l_csymbol_symbols_on = {
+    'ru': "✅☑Вкл 文ب-бан",
+    'en': "✅☑On 文ب-ban",
+    'es': "✅☑En 文ب-ban",
+    'fr': "✅☑En 文ب-ban",
+    'zh': "✅☑使能夠 文ب-ban",
+    'ar': "✅☑ يُمكَِن 文ب-ban",
+}
+l_csymbol_symbols_off = {
+    'ru': "☑️☐Выкл 文ب-бан",
+    'en': "☑️☐Off 文ب-ban",
+    'es': "☑️☐De 文ب-ban",
+    'fr': "☑️☐De 文ب-ban",
+    'zh': "☑️☐禁用 文ب-ban",
+    'ar': "☑️☐ معاق 文ب-ban",
+}
+l_csymbol_zalgo_on = {
+    'ru': "✅☑Вкл zalgo-бан",
+    'en': "✅☑On zalgo-ban",
+    'es': "✅☑En zalgo-ban",
+    'fr': "✅☑En zalgo-ban",
+    'zh': "✅☑使能夠 zalgo-ban",
+    'ar': "✅☑ يُمكَِن zalgo-ban",
+}
+l_csymbol_zalgo_off = {
+    'ru': "☑️☐Выкл zalgo-бан",
+    'en': "☑️☐Off zalgo-ban",
+    'es': "☑️☐De zalgo-ban",
+    'fr': "☑️☐De zalgo-ban",
+    'zh': "☑️☐禁用 zalgo-ban",
+    'ar': "☑️☐ معاق zalgo-ban",
+}
+# endregion
+
+
+# region cmedia_
+l_cmedia_text = {
+    'ru': "🗣 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> разрешение на <i>media</i>-сообщения\n\n👉🏼 Например, [☑️☐Выкл видео-заметки] означает запрет на <b>видео-заметки в кружочке</b> в нашей группе\n\n👉🏼 Чтобы разрешить/запретить конкретный стикерпак, жми [⚙️Настроить]",
+    'en': "🗣 Push the ✅/☑️, to <b>On/Off</b> permission on <i>media</i>-messages\n\n👉🏼 For example, [☑️☐Off video-note] means sending-prohibition on <b>video-note</b> in our group\n\n👉🏼 To allow/prohibit specific sticker-pack, push the [⚙️Configure]",
+    'es': "🗣 Presiona ✅/☑️, para <b>Activar/Desactivar</b> permiso en <i>medios</i>-mensajes\n\n👉🏼 Por ejemplo, [☑️☐Off video-note] significa enviar- Prohibición de <b>notas de video</b> en nuestro grupo\n\n👉🏼 Para permitir/prohibir un paquete de calcomanías específico, presiona [⚙️Configurar]",
+    'fr': "🗣 Appuyez sur ✅/☑️, sur l'autorisation <b>On/Off</b> sur les messages <i>media</i>\n\n👉🏼 Par exemple, [☑️☐Off video-note] signifie envoyer- interdiction de <b>video-note</b> dans notre groupe\n\n👉🏼 Pour autoriser/interdire un pack d'autocollants spécifique, appuyez sur [⚙️Configurer]",
+    'zh': "🗣 將 ✅/☑️ 推送到 <i>media</i> 消息上的 <b>On/Off</b> 權限\n\n👉🏼 例如，[☑️☐Off video-note] 表示發送- 禁止我們組中的 <b>video-note</b>\n\n👉🏼 要允許/禁止特定的貼紙包，請按下 [⚙️Configure]",
+    'ar': "🗣 ادفع ✅ / ☑️ ، إلى إذن <b> تشغيل / إيقاف </b> على <i> الوسائط </i> - الرسائل \n\n👉🏼 على سبيل المثال ، [☑️☐ Off video-note] تعني إرسال- حظر <b> ملاحظة الفيديو </b> في مجموعتنا \n\n👉🏼 للسماح / حظر حزمة ملصقات معينة ، اضغط على [⚙️ تكوين]",
+}
+l_cmedia_photo_on = {
+    'ru': "✅☑Вкл photo",
+    'en': "✅☑On photo",
+    'es': "✅☑En photo",
+    'fr': "✅☑En photo",
+    'zh': "✅☑使能夠 photo",
+    'ar': "✅☑ يُمكَِن photo",
+}
+l_cmedia_photo_off = {
+    'ru': "☑️☐Выкл photo",
+    'en': "☑️☐Off photo",
+    'es': "☑️☐De photo",
+    'fr': "☑️☐De photo",
+    'zh': "☑️☐禁用 photo",
+    'ar': "☑️☐تعطيل photo",
+}
+l_cmedia_video_on = {
+    'ru': "✅☑Вкл video",
+    'en': "✅☑On video",
+    'es': "✅☑En video",
+    'fr': "✅☑En video",
+    'zh': "✅☑使能夠 video",
+    'ar': "✅☑ يُمكَِن video",
+}
+l_cmedia_video_off = {
+    'ru': "☑️☐Выкл video",
+    'en': "☑️☐Off video",
+    'es': "☑️☐De video",
+    'fr': "☑️☐De video",
+    'zh': "☑️☐禁用 video",
+    'ar': "☑️☐تعطيل video",
+}
+l_cmedia_giff_on = {
+    'ru': "✅☑Вкл giff",
+    'en': "✅☑On giff",
+    'es': "✅☑En giff",
+    'fr': "✅☑En giff",
+    'zh': "✅☑使能夠 giff",
+    'ar': "✅☑ يُمكَِن giff",
+}
+l_cmedia_giff_off = {
+    'ru': "☑️☐Выкл giff",
+    'en': "☑️☐Off giff",
+    'es': "☑️☐De giff",
+    'fr': "☑️☐De giff",
+    'zh': "☑️☐禁用 giff",
+    'ar': "☑️☐تعطيل giff",
+}
+l_cmedia_audio_on = {
+    'ru': "✅☑Вкл audio",
+    'en': "✅☑On audio",
+    'es': "✅☑En audio",
+    'fr': "✅☑En audio",
+    'zh': "✅☑使能夠 audio",
+    'ar': "✅☑ يُمكَِن audio",
+}
+l_cmedia_audio_off = {
+    'ru': "☑️☐Выкл audio",
+    'en': "☑️☐Off audio",
+    'es': "☑️☐De audio",
+    'fr': "☑️☐De audio",
+    'zh': "☑️☐禁用 audio",
+    'ar': "☑️☐تعطيل audio",
+}
+l_cmedia_emoji_on = {
+    'ru': "✅☑Вкл emoji",
+    'en': "✅☑On emoji",
+    'es': "✅☑En emoji",
+    'fr': "✅☑En emoji",
+    'zh': "✅☑使能夠 emoji",
+    'ar': "✅☑ يُمكَِن emoji",
+}
+l_cmedia_emoji_off = {
+    'ru': "☑️☐Выкл emoji",
+    'en': "☑️☐Off emoji",
+    'es': "☑️☐De emoji",
+    'fr': "☑️☐De emoji",
+    'zh': "☑️☐禁用 emoji",
+    'ar': "☑️☐تعطيل emoji",
+}
+l_cmedia_docum_on = {
+    'ru': "✅☑Вкл docum",
+    'en': "✅☑On docum",
+    'es': "✅☑En docum",
+    'fr': "✅☑En docum",
+    'zh': "✅☑使能夠 docum",
+    'ar': "✅☑ يُمكَِن docum",
+}
+l_cmedia_docum_off = {
+    'ru': "☑️☐Выкл docum",
+    'en': "☑️☐Off docum",
+    'es': "☑️☐De docum",
+    'fr': "☑️☐De docum",
+    'zh': "☑️☐禁用 docum",
+    'ar': "☑️☐تعطيل docum",
+}
+l_cmedia_viabot_on = {
+    'ru': "✅☑Вкл via_bot",
+    'en': "✅☑On via_bot",
+    'es': "✅☑En via_bot",
+    'fr': "✅☑En via_bot",
+    'zh': "✅☑使能夠 via_bot",
+    'ar': "✅☑ يُمكَِن via_bot",
+}
+l_cmedia_viabot_off = {
+    'ru': "☑️☐Выкл via_bot",
+    'en': "☑️☐Off via_bot",
+    'es': "☑️☐De via_bot",
+    'fr': "☑️☐De via_bot",
+    'zh': "☑️☐禁用 via_bot",
+    'ar': "☑️☐تعطيل via_bot",
+}
+l_cmedia_poll_on = {
+    'ru': "✅☑Вкл опросы",
+    'en': "✅☑On poll",
+    'es': "✅☑En poll",
+    'fr': "✅☑En poll",
+    'zh': "✅☑使能夠 poll",
+    'ar': "✅☑ يُمكَِن poll",
+}
+l_cmedia_poll_off = {
+    'ru': "☑️☐Выкл опросы",
+    'en': "☑️☐Off poll",
+    'es': "☑️☐De poll",
+    'fr': "☑️☐De poll",
+    'zh': "☑️☐禁用 poll",
+    'ar': "☑️☐تعطيل poll",
+}
+l_cmedia_sticker_on = {
+    'ru': "✅☑Вкл sticker",
+    'en': "✅☑On sticker",
+    'es': "✅☑En sticker",
+    'fr': "✅☑En sticker",
+    'zh': "✅☑使能夠 sticker",
+    'ar': "✅☑ يُمكَِن sticker",
+}
+l_cmedia_sticker_off = {
+    'ru': "☑️☐Выкл sticker",
+    'en': "☑️☐Off sticker",
+    'es': "☑️☐De sticker",
+    'fr': "☑️☐De sticker",
+    'zh': "☑️☐禁用 sticker",
+    'ar': "☑️☐تعطيل sticker",
+}
+l_cmedia_voice_on = {
+    'ru': "✅☑Вкл голосовые",
+    'en': "✅☑On voice",
+    'es': "✅☑En voice",
+    'fr': "✅☑En voice",
+    'zh': "✅☑使能夠 voice",
+    'ar': "✅☑ يُمكَِن voice",
+}
+l_cmedia_voice_off = {
+    'ru': "☑️☐Выкл голосовые",
+    'en': "☑️☐Off voice",
+    'es': "☑️☐De voice",
+    'fr': "☑️☐De voice",
+    'zh': "☑️☐禁用 voice",
+    'ar': "☑️☐تعطيل voice",
+}
+l_cmedia_videonote_on = {
+    'ru': "✅☑Вкл видео-заметки",
+    'en': "✅☑On video-note",
+    'es': "✅☑En video-note",
+    'fr': "✅☑En video-note",
+    'zh': "✅☑使能夠 video-note",
+    'ar': "✅☑ يُمكَِن video-note",
+}
+l_cmedia_videonote_off = {
+    'ru': "☑️☐Выкл видео-заметки",
+    'en': "☑️☐Off video-note",
+    'es': "☑️☐De video-note",
+    'fr': "☑️☐De video-note",
+    'zh': "☑️☐禁用 video-note",
+    'ar': "☑️☐تعطيل video-note",
+}
+l_cmedia_call_photo = {
+    'ru': "👮🏽 В настройках [Разрешения] включи опцию:\n\n[✅ Отправка фото и видео]\n\n🕚Подожди 1min",
+    'en': "👮🏽 In the Settings [Permissions] enable:\n\n[✅ Send Media]\n🕚Wait for 1min",
+    'es': "👮🏽 En la Configuración [Permisos] habilite:\n\n[✅ Enviar medios]\n🕚 Espere 1 minuto",
+    'fr': "👮🏽 Dans les paramètres [Autorisations], activez :\n\n[✅ Envoyer un média]\nt🕚Attendez 1 min",
+    'zh': "👮🏽在設置[權限]中啟用：\n\n[✅發送媒體]\n🕚等待1分鐘",
+    'ar': "👮🏽 في الإعدادات [الأذونات] ، قم بتمكين: \n\n [✅ إرسال الوسائط]\n🕚 انتظر لمدة دقيقة واحدة",
+}
+l_cmedia_call_sticker_giff = {
+    'ru': "👮🏽 В настройках [Разрешения] включи опцию:\n\n[✅ Отправка стикеров и GIF]\n\n🕚Подожди 1min",
+    'en': "👮🏽 In the Settings [Permissions] enable:\n\n[✅ Send Stickers]\n🕚Wait for 1min",
+    'es': "👮🏽 En la Configuración [Permisos] habilite:\n\n[✅ Enviar Pegatinas]\n🕚Espere 1 minuto",
+    'fr': "👮🏽 Dans les paramètres [Autorisations], activez :\n\n[✅ Envoyer des Autocollants]\n🕚Attendez 1 min",
+    'zh': "👮🏽 在設置[權限]中啟用：\n\n[✅發送貼紙]\n🕚等待1分鐘",
+    'ar': "👮🏽 في الإعدادات [الأذونات] ، قم بتمكين: \n\n [✅ إرسال ملصقات] \n🕚 انتظر لمدة دقيقة واحدة",
+}
+l_cmedia_call_poll = {
+    'ru': "👮🏽 В настройках [Разрешения] включи опцию:\n\n[✅ Отправка опросов]\n\n🕚Подожди 1min",
+    'en': "👮🏽 In the Settings [Permissions] enable:\n\n[✅ Send Poll]\n🕚Wait for 1min",
+    'es': "👮🏽 En la Configuración [Permisos] habilite:\n\n[✅ Enviar encuesta]\n🕚Espere 1 minuto",
+    'fr': "👮🏽 Dans les paramètres [Autorisations], activez :\n\n[✅ Envoyer un sondage]\n🕚Attendez 1 min",
+    'zh': "👮🏽 在設置[權限]中啟用：\n\n[✅發送投票]\n🕚等待1分鐘",
+    'ar': "👮🏽 في الإعدادات [الأذونات] ، قم بتمكين: \n\n [✅ إرسال استطلاع] \n🕚 انتظر لمدة دقيقة واحدة",
+}
+l_cstickerconfig_text = {
+    'ru': "🦊 <b>Исключения</b> для стикерпаков в <code>{0}</code>-файле:\n\n+ Разрешенные: <u>{1}</u>\n- Запрещенные: <u>{2}</u>\n\n[✅ Разрешить] пропускает указанные стикерпаки <i>в качестве исключения</i>, когда выбрана опция [☑️☐Выкл sticker]\n\n[🚫 Запретить] запрещает указанные стикерпаки <i>в качестве исключения</i>, когда выбрана опция [✅☑Вкл sticker]",
+    'en': "🦊 <b>Exceptions</b> for sticker-packs in <code>{0}</code>-file:\n\n+ Allowed: <u>{1}</u>\n- Prohibited: <u>{2}</u>\n\n[✅ Allow] allow specified sticker-packs <i>as exception</i>, when [☑️☐Off sticker]\n[🚫 Prohibit] prohibits the specified sticker-packs <i>as exception</i>, when [✅☑On sticker]",
+    'es': "🦊 <b>Excepciones</b> para paquetes de pegatinas en el archivo <code>{0}</code>:\n\n+ Permitido: <u>{1}</u>\n- Prohibido: <u>{2}</u>\n\n[✅ Permitir] permitir paquetes de adhesivos especificados <i>como excepción</i>, cuando [☑️☐Desactivar adhesivo]\n[🚫 Prohibir] prohíbe los paquetes de adhesivos especificados <i>como excepción</i>, cuando [✅☑En la etiqueta]",
+    'fr': "🦊 <b>Exceptions</b> pour les packs d'autocollants dans le fichier <code>{0}</code> :\n\n+ Autorisé : <u>{1}</u>\n- Interdit : <u>{2}</u>\n\n[✅ Autoriser] autoriser les packs d'autocollants spécifiés <i>à titre exceptionnel</i>, lorsque [☑️☐Autocollant désactivé]\n[🚫 Interdire] interdit les packs d'autocollants spécifiés <i>par exception</i>, lorsque [✅☑Sur l'autocollant]",
+    'zh': "🦊 <code>{0}</code>-文件中貼紙包的<b>例外</b>：\n\n+ 允許：<u>{1}</u>\n- 禁止：<u>{2}</u>\n\n[✅ Allow] 允許指定的貼紙包<i>作為例外</i>，當 [☑️☐Off 貼紙]\n[🚫 Prohibit] 禁止指定的貼紙包 <i>例外</i>，當 [✅☑On 貼紙]",
+    'ar': "🦊 <b> استثناءات </b> لحزم الملصقات في <code>{0}</code> -ملف: \n\n + المسموح به: <u>{1}</u> \n- محظور: <u>{2}</u> \n\n [✅ السماح] السماح بحزم الملصقات المحددة <i> كاستثناء </i> ، عندما يحظر [☑️☐ إيقاف الملصق] \n [🚫 منع] حزم الملصقات المحددة <i> كاستثناء </i> ، عند [✅☑ على الملصق]",
+}
+l_cstickerpack_1 = {
+    'ru': "✅ Разрешить",
+    'en': "✅ Allow",
+    'es': "✅ Permitir",
+    'fr': "✅ Autoriser",
+    'zh': "✅ 允許",
+    'ar': "✅ سماح",
+}
+l_cstickerpack_0 = {
+    'ru': "🚫 Запретить",
+    'en': "🚫 Prohibit",
+    'es': "🚫 Prohibir",
+    'fr': "🚫 Interdire",
+    'zh': "🚫 禁止",
+    'ar': "🚫 تحظر",
+}
+l_coperation_1 = {
+    'ru': "✅ Добавить",
+    'en': "✅ Add",
+    'es': "✅ Añadir",
+    'fr': "✅ Ajouter",
+    'zh': "✅ 添加",
+    'ar': "✅ أضف",
+}
+l_coperation_0 = {
+    'ru': "🚫 Удалить",
+    'en': "🚫 Remove",
+    'es': "🚫 Eliminar",
+    'fr': "🚫 Supprimer",
+    'zh': "🚫 移除",
+    'ar': "🚫 إزالة",
+}
+l_GROUPP_CSTICKER1_NUM1 = {
+    'ru': "🦊 Текущее количество <b>разрешенных</b> стикерпаков в <code>{0}</code>-файле: <u>{1}</u>\n\nЖми на ✅/🚫, чтобы <b>Добавить/Удалить</b> разрешенные стикерпаки",
+    'en': "🦊 Current number of <b>allowed</b> sticker-packs in the <code>{0}</code>-file: <u>{0}</u>\n\nPush the ✅/🚫, to <b>Add/Remove</b> allowed sticker-packs",
+    'es': "🦊 Número actual de paquetes de pegatinas <b>permitidos</b> en el archivo <code>{0}</code>: <u>{0}</u>\n\nPresione ✅/🚫, para <b>Añadir/eliminar</b> paquetes de pegatinas permitidos",
+    'fr': "🦊 Nombre actuel de packs d'autocollants <b>autorisés</b> dans le fichier <code>{0}</code> : <u>{0}</u>\n\nAppuyez sur ✅/🚫 pour <b>Ajouter/Supprimer</b> les packs d'autocollants autorisés",
+    'zh': "🦊 <code>{0}</code>-文件中<b>允許</b>貼紙包的當前數量：<u>{0}</u>\n\n將 ✅/🚫 推到 <b>添加/刪除</b>允許的貼紙包",
+    'ar': "🦊 العدد الحالي لحزم الملصقات <b> المسموح بها </b> في <code>{0}</code> -ملف: <u>{0}</u> \n\n اضغط على ✅/🚫 ، من أجل <b> إضافة / إزالة </b> حزم الملصقات المسموح بها",
+}
+l_GROUPP_CSTICKER1_NUM0 = {
+    'ru': "🦊 Текущее количество <b>разрешенных</b> стикерпаков: <u>{0}</u>\n\nЖми на ✅/🚫, чтобы <b>Добавить/Удалить</b> разрешенные стикерпаки",
+    'en': "🦊 Current number of <b>allowed</b> sticker-packs: <u>{0}</u>\n\nPush the ✅/🚫, to <b>Add/Remove</b> allowed sticker-packs",
+    'es': "🦊 Número actual de paquetes de adhesivos <b>permitidos</b>: <u>{0}</u>\n\nPresione ✅/🚫 para <b>Agregar/Quitar</b> paquetes de adhesivos permitidos",
+    'fr': "🦊 Nombre actuel de packs d'autocollants <b>autorisés</b> : <u>{0}</u>\n\nAppuyez sur ✅/🚫 pour <b>ajouter/supprimer</b> les packs d'autocollants autorisés",
+    'zh': "🦊 當前<b>允許</b>個貼紙包的數量：<u>{0}</u>\n\n按下 ✅/🚫，以<b>添加/刪除</b>個允許的貼紙包",
+    'ar': "🦊 العدد الحالي لحزم الملصقات <b> المسموح بها </b>: <u>{0}</u> \n\n اضغط على ✅/🚫 ، من أجل <b> إضافة / إزالة </b> حزم الملصقات المسموح بها",
+}
+l_GROUPP_CSTICKER0_NUM1 = {
+    'ru': "🦊 Текущее количество <b>запрещенных</b> стикерпаков в <code>{0}</code>-файле: <u>{1}</u>\n\nЖми на ✅/🚫, чтобы <b>Добавить/Удалить</b> запрещенные стикерпаки",
+    'en': "🦊 Current number of <b>prohibited</b> sticker-packs in the <code>{0}</code>-file: <u>{0}</u>\n\nPush the ✅/🚫, to <b>Add/Remove</b> prohibited sticker-packs",
+    'es': "🦊 Número actual de paquetes de adhesivos <b>prohibidos</b> en el archivo <code>{0}</code>: <u>{0}</u>\n\nPresione el ✅/🚫 para <b>Añadir/eliminar</b> paquetes de pegatinas prohibidos",
+    'fr': "🦊 Nombre actuel de packs d'autocollants <b>interdits</b> dans le fichier <code>{0}</code> : <u>{0}</u>\n\nAppuyez sur ✅/🚫 pour <b>Ajouter/Supprimer</b> des packs d'autocollants interdits",
+    'zh': "🦊 <code>{0}</code>-文件中<b>禁止</b>貼紙包的當前數量：<u>{0}</u>\n\n將 ✅/🚫 推到 <b>添加/刪除</b>禁止的貼紙包",
+    'ar': "🦊 العدد الحالي لحزم الملصقات <b> المحظورة </b> في <code>{0}</code> -ملف: <u>{0}</u> \n\n اضغط على ✅/🚫 ، من أجل <b> إضافة / إزالة </b> حزم الملصقات المحظورة",
+}
+l_GROUPP_CSTICKER0_NUM0 = {
+    'ru': "🦊 Текущее количество <b>запрещенных</b> стикерпаков: <u>{0}</u>\n\nЖми на ✅/🚫, чтобы <b>Добавить/Удалить</b> запрещенные стикерпаки",
+    'en': "🦊 Current number of <b>prohibited</b> sticker-packs: <u>{0}</u>\n\nPush the ✅/🚫, to <b>Add/Remove</b> prohibited sticker-packs",
+    'es': "🦊 Número actual de paquetes de adhesivos <b>prohibidos</b>: <u>{0}</u>\n\nPresione ✅/🚫 para <b>Agregar/Quitar</b> paquetes de adhesivos prohibidos",
+    'fr': "🦊 Nombre actuel de packs d'autocollants <b>interdits</b> : <u>{0}</u>\n\nAppuyez sur ✅/🚫 pour <b>Ajouter/Supprimer</b> des packs d'autocollants interdits",
+    'zh': "🦊 當前<b>禁止</b>貼紙包的數量：<u>{0}</u>\n\n按下 ✅/🚫，<b>添加/刪除</b>禁止貼紙包",
+    'ar': "🦊 العدد الحالي لحزم الملصقات <b> المحظورة </b>: <u>{0}</u> \n\n اضغط على ✅/🚫 ، من أجل <b> إضافة / إزالة </b> حزم الملصقات المحظورة",
+}
+l_cstickeroperation_add = {
+    'ru': "\n\n👉🏼 Например, https://t.me/addstickers/HotCherry или <code>HotCherry</code>",
+    'en': "\n\n👉🏼 For example, https://t.me/addstickers/HotCherry or <code>HotCherry</code>",
+    'es': "\n\n👉🏼 Por ejemplo, https://t.me/addstickers/HotCherry o <code>HotCherry</code>",
+    'fr': "\n\n👉🏼 Par exemple, https://t.me/addstickers/HotCherry ou <code>HotCherry</code>",
+    'zh': "\n\n👉🏼 例如, https://t.me/addstickers/HotCherry 或者 <code>HotCherry</code>",
+    'ar': "\n\n👉🏼 فمثلا, https://t.me/addstickers/HotCherry أو <code>HotCherry</code>",
+}
+l_cstickeroperation_isadd = {
+    'ru': "✅ Пришли ссылку или имя <b>стикерпака</b>, чтобы <b>добавить</b> его в список разрешенных{0}",
+    'en': "✅ Send link or <b>sticker-pack</b>-name to <b>add</b> it to allowed list{0}",
+    'es': "✅ Enviar enlace o nombre de <b>paquete de pegatinas</b> para <b>añadir</b> a la lista de permitidos{0}",
+    'fr': "✅ Envoyez le lien ou le nom du <b>pack d'autocollants</b> pour <b>l'ajouter</b> à la liste autorisée{0}",
+    'zh': "✅ 發送鏈接或 <b>sticker-pack</b>-name 以將其<b>添加</b>到允許列表{0}",
+    'ar': "✅ أرسل رابطًا أو اسم <b> حزمة الملصقات </b> <b> لإضافته </b> إلى القائمة المسموح بها {0}",
+}
+l_cstickeroperation_isnotadd = {
+    'ru': "🚫 Пришли ссылку или имя <b>стикерпака</b>, чтобы <b>удалить</b> из списка разрешенных{0}",
+    'en': "🚫 Send link or <b>sticker-pack</b>-name to <b>remove</b> it from allowed list{0}",
+    'es': "🚫 Enviar enlace o nombre de <b>paquete de pegatinas</b> para <b>eliminarlo</b> de la lista permitida{0}",
+    'fr': "🚫 Envoyez le lien ou le nom du <b>pack d'autocollants</b> pour le <b>supprimer</b> de la liste autorisée{0}",
+    'zh': "🚫 發送鏈接或 <b>sticker-pack</b>-name 以將其從允許列表中<b>刪除</b>{0}",
+    'ar': "🚫 أرسل رابطًا أو اسم <b> حزمة الملصقات </b> <b> لإزالته </b> من القائمة المسموح بها {0}",
+}
+l_cstickeroperation_isadd2 = {
+    'ru': "✅ Пришли ссылку или имя <b>стикерпака</b>, чтобы <b>добавить</b> его в список запрещенных{0}",
+    'en': "✅ Send link or <b>sticker-pack</b>-name to <b>add</b> it to prohibited list{0}",
+    'es': "✅ Enviar enlace o nombre de <b>paquete de pegatinas</b> para <b>añadir</b> a la lista prohibida{0}",
+    'fr': "✅ Envoyez le lien ou le nom du <b>pack d'autocollants</b> pour <b>l'ajouter</b> à la liste interdite{0}",
+    'zh': "✅ 發送鏈接或 <b>sticker-pack</b>-name 以將其<b>添加</b>到禁止列表{0}",
+    'ar': "✅ أرسل رابطًا أو اسم <b> حزمة الملصقات </b> <b> لإضافته </b> إلى القائمة المحظورة {0}",
+}
+l_cstickeroperation_isnotadd2 = {
+    'ru': "🚫 Пришли ссылку или имя <b>стикерпака</b>,  чтобы <b>удалить</b> его из списка запрещенных{0}",
+    'en': "🚫 Send link or <b>sticker-pack</b>-name to <b>remove</b> it from prohibited list{0}",
+    'es': "🚫 Enviar enlace o nombre de <b>paquete de pegatinas</b> para <b>eliminarlo</b> de la lista prohibida{0}",
+    'fr': "🚫 Envoyez le lien ou le nom du <b>pack d'autocollants</b> pour le <b>supprimer</b> de la liste interdite{0}",
+    'zh': "🚫 發送鏈接或 <b>sticker-pack</b>-name 以將其從禁止列表中<b>刪除</b>{0}",
+    'ar': "🚫 أرسل رابطًا أو اسم <b> حزمة الملصقات </b> <b> لإزالته </b> من القائمة المحظورة {0}",
+}
+l_fsm_sticker_add = {
+    'ru': "🦊 Готово! <b>Исключения</b> для стикерпаков:\n\n+ Разрешенные: <u>{0}</u>\n- Запрещенные: <u>{1}</u>\n\n[✅ Разрешить] пропускает указанные стикерпаки <i>в качестве исключения</i>, когда выбрана опция [☑️☐Выкл sticker]\n[🚫 Запретить] запрещает указанные стикерпаки <i>в качестве исключения</i>, когда выбрана опция [✅☑Вкл sticker]",
+    'en': "🦊 Ready! <b>Exceptions</b> for sticker-packs:\n\n+ Allowed: <u>{0}</u>\n- Prohibited: <u>{1}</u>\n\n[✅ Allow] allow specified sticker-packs <i>as exception</i>, when [☑️☐Off sticker]\n[🚫 Prohibit] prohibits the specified sticker-packs <i>as exception</i>, when [✅☑On sticker]",
+    'es': "🦊 Listo! <b>Excepciones</b> para paquetes de pegatinas:\n\n+ Permitido: <u>{0}</u>\n- Prohibido: <u>{1}</u>\n\n[✅ Permitir] permitir paquetes de adhesivos especificados <i>como excepción</i>, cuando [☑️☐De sticker]\n[🚫 Prohibir] prohíbe los paquetes de adhesivos especificados <i>como excepción</i>, cuando [✅☑En sticker]",
+    'fr': "🦊 Prêt ! <b>Exceptions</b> pour les packs d'autocollants :\n\n+ Autorisé : <u>{0}</u>\n- Interdit : <u>{1}</u>\n\n[✅ Autoriser] autoriser les packs d'autocollants spécifiés <i>à titre exceptionnel</i>, lorsque [☑️☐En sticker]\n[🚫 Interdire] interdit les packs d'autocollants spécifiés <i>à titre exceptionnel</i>, lorsque [✅☑En sticker]",
+    'zh': "🦊 準備好了！ 貼紙包的<b>例外情況</b>：\n\n+ 允許：<u>{0}</u>\n- 禁止：<u>{1}</u>\n\n[✅ Allow] 允許指定的貼紙包<i>作為例外</i>，當 [☑️☐Off 貼紙]\n[🚫 Prohibit] 禁止指定的貼紙包<i>作為例外</i>，當 [✅☑ 貼上]",
+    'ar': "🦊 جاهز! <b> استثناءات </b> لحزم الملصقات: \n\n + المسموح بها: <u>{0}</u>\n- محظور: <u>{1}</u>\n\n [✅ السماح] السماح بحزم الملصقات المحددة <i> كاستثناء </i> ، عندما [☑️☐ ملصق إيقاف]\n[🚫 منع] يحظر حزم الملصقات المحددة <i> كاستثناء </i> ، عندما [✅☑ على الملصق]",
+}
+# endregion
+
+
+# region cstart_
+l_cstart_text = {
+    'ru': "🚀 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-ответ на триггер-сообщения, содержащие конкретные старт-слова\n\n👉🏼 Текущее количество старт-слов <u>{0}</u>",
+    'en': "🚀 Push the ✅/☑️, to <b>On/Off</b> auto-answer on trigger-messages, containing specific start-words\n\n👉🏼 Current number of start-words <u>{0}</u>",
+    'es': "🚀 Presiona ✅/☑️, para <b>Activar/Desactivar</b> la respuesta automática en mensajes desencadenantes, que contienen palabras de inicio específicas\n\n👉🏼 Número actual de palabras de inicio <u>{0}</u>",
+    'fr': "🚀 Appuyez sur ✅/☑️, pour <b>Activer/Désactiver</b> la réponse automatique aux messages déclencheurs, contenant des mots de départ spécifiques\n\n👉🏼 Nombre actuel de mots de départ <u>{0}</u>",
+    'zh': "🚀 將 ✅/☑️ 推到 <b>On/Off</b> 觸發消息上的自動應答，包含特定的起始詞\n\n👉🏼 當前起始詞的數量<u>{0}</u>",
+    'ar': "🚀 اضغط على ✅ / ☑️ ، لإجراء تشغيل / إيقاف الرد التلقائي على الرسائل المشغلة ، التي تحتوي على كلمات بداية محددة \n\n👉🏼 العدد الحالي لكلمات البداية {0} / ش",
+}
+l_cstart_call = {
+    'ru': "🔔 Нужно ⚙️Настроить хотя бы одно старт-слово",
+    'en': "🔔 You have to ⚙️Configure at least one start-word",
+    'es': "🔔 Tienes que ⚙️ Configurar al menos una palabra de inicio",
+    'fr': "🔔 Vous devez ⚙️ Configurer au moins un mot de départ",
+    'zh': "🔔 你必須 ⚙️ 配置至少一個起始詞",
+    'ar': "🔔 يجب عليك ⚙️ تكوين كلمة بداية واحدة على الأقل",
+}
+l_cstartconfig_call = {
+    'ru': "🚀 Нужно ⚙️Настроить хотя бы один пост через опцию 🔔Авто-постинг",
+    'en': "🚀 You have to ⚙️Configure at least one post via 🔔Auto-posting",
+    'es': "🚀 Tienes que ⚙️Configurar al menos una publicación a través de 🔔Publicación automática",
+    'fr': "🚀 Vous devez ⚙️Configurer au moins une publication via 🔔Auto-publication",
+    'zh': "🚀您必須通過🔔自動發布⚙️配置至少一篇帖子",
+    'ar': "🚀 عليك تكوين منشور واحد على الأقل عبر النشر التلقائي",
+}
+l_cstartconfig_text = {
+    'ru': "🚀 Выбери <b>пост</b>, который будет присылаться в ответ на <b>старт</b>-слова и жми [🚀 <b>Использовать</b>] под выбранным постом\n\n👉🏼 Общее количество старт-слов: <u>{0}</u>",
+    'en': "🚀 At first, choose the auto-reply (from posts), which will be sent in response to the start-words",
+    'es': "🚀 Al principio, elija la respuesta automática (de las publicaciones), que se enviará en respuesta a las palabras de inicio",
+    'fr': "🚀 Dans un premier temps, choisissez la réponse automatique (à partir des messages), qui sera envoyée en réponse aux mots de départ",
+    'zh': "🚀 首先，選擇自動回复（來自帖子），它將響應起始詞發送",
+    'ar': "🚀 في البداية ، اختر الرد التلقائي (من المشاركات) ، والذي سيتم إرساله ردًا على كلمات البداية",
+}
+l_cstartconfig_use = {
+    'ru': "🚀 Использовать",
+    'en': "🚀 Use",
+    'es': "🚀 Uso",
+    'fr': "🚀 Utiliser",
+    'zh': "🚀 使用",
+    'ar': "🚀 استخدم",
+}
+l_cstartoperation_caption = {
+    'ru': "🚀 <b>Текущее</b> количество <i>старт-слов</i> для поста #{0} в <code>{1}</code>-файле: <u>{2}</u>\n\nЖми на ✅/🚫, чтобы <b>Добавить/Удалить</b> старт-слова",
+    'en': "🚀 Current number of start-words for post #{0} in <code>{1}</code>-file: <u>{2}</u>\n\nPuch the ✅/🚫, to <b>Add/Remove</b> start-words",
+    'es': "🚀 Número actual de palabras iniciales para la publicación #{0} en el archivo <code>{1}</code>: <u>{2}</u>\n\nPulse el ✅/🚫, para <b> Agregar o quitar</b> palabras de inicio",
+    'fr': "🚀  Nombre actuel de mots de départ pour le message #{0} dans le fichier <code>{1}</code> : <u>{2}</u>\n\nAppuyez sur le ✅/🚫 pour <b> Ajouter/supprimer</b> des mots de départ",
+    'zh': "🚀 當前的起始詞數 在 <code>{1}</code>-文件中發布 #{0}：<u>{2}</u>\n\n點擊 ✅/🚫，開始<b>添加/刪除</b> -字",
+    'ar': "🚀 العدد الحالي لكلمات البداية للنشر # {0} في <code>{1}</code> -الملف:{2} \n\n قم بإرسال ✅/🚫 إلى إضافة / إزالة كلمات البداية",
+}
+l_cstartoperation_text = {
+    'ru': "🚀 <b>Текущее</b> количество <i>старт-слов</i> для поста #{0}: <u>{1}</u>\n\nЖми на ✅/🚫, чтобы <b>Добавить/Удалить</b> старт-слова",
+    'en': "🚀 Current number of start-words for post #{0}: <u>{2}</u>\n\nPuch the ✅/🚫, to <b>Add/Remove</b> start-words",
+    'es': "🚀 Número actual de palabras de inicio para la publicación #{0}: <u>{2}</u>\n\nPresione ✅/🚫 para <b>Agregar/Quitar</b> palabras de inicio",
+    'fr': "🚀  Nombre actuel de mots de départ pour le message #{0} : <u>{2}</u>\n\nAppuyez sur le ✅/🚫 pour <b>ajouter/supprimer</b> des mots de départ",
+    'zh': "🚀 帖子 #{0} 的當前起始詞數：<u>{2}</u>\n\n點擊 ✅/🚫，以<b>添加/刪除</b>個起始詞",
+    'ar': "🚀 العدد الحالي لكلمات البداية للنشر # {0}:{2}\n\n استخدم ✅/🚫 ، من أجل <b> إضافة / إزالة </b> كلمات البداية",
+}
+l_cstartoperation_handler = {
+    'ru': "\n\n▪️регистр не важен\n▪️поставь звездочку после слова, чтобы учитывать вхождение\n▪️например, если ввести <b>психо*</b>, то авто-постинг сработает на <u>все</u> сообщения, которые <b>содержат</b> данное сочетание: <i>анти<u>психо</u>лог, <u>Психо</u>терапевт..</i>",
+    'en': "\n\n▪️word case is not important\n▪️set * after word to account for occurrence\n▪️for example, if write <b>psy*</b>, then <u>all</u> messages, which are <b>contained</b> this combination of letters will be removed: <i>anti-<u>psy</u>chologist, <u>Psy</u>chotherapist..</i>",
+    'es': "\n\n▪️las mayúsculas y minúsculas no son importantes\n▪️establezca * después de la palabra para tener en cuenta la ocurrencia\n▪️por ejemplo, si escribe <b>psi*</b>, entonces <u>todos</u> los mensajes, que están <b>contenidos</b> se eliminará esta combinación de letras: <i>anti-<u>psicólogo</u>, <u>Psi</u>coterapeuta..</i>",
+    'fr': "\n\n▪️la casse des mots n'est pas importante\n▪️définissez * après le mot pour tenir compte de l'occurrence\n▪️par exemple, si écrivez <b>psy*</b>, alors <u>tous</u> les messages, qui sont <b>contenues</b> cette combinaison de lettres sera supprimée : <i>anti-<u>psychologue</u>, <u>Psy</u>chothérapeute..</i>",
+    'zh': "\n\n▪️單詞大小寫不重要\n▪️在單詞之後設置*以說明出現\n▪️例如，如果寫<b>psy*</b>，則<u>所有</u>消息， <b>包含</b>這些字母組合將被刪除：<i>anti-<u>psy</u>chologist, <u>Psy</u>chotherapy..</i>",
+    'ar': "\n\n▪️ حالة الكلمة ليست مهمة \n▪️ اضبط * بعد كلمة لحساب الحدوث \n▪️ على سبيل المثال ، إذا كتبت <b>psy*</b> ، ثم <u> كل </u> الرسائل ، التي <b> احتوت </b> ستتم إزالة هذه المجموعة من الأحرف:",
+}
+l_cstartoperation_answer = {
+    'ru': "🚀 Введи <u>старт-слова</u> <b>через</b> пробелы или разделители, чтобы <i>добавить</i> их в базу{0}",
+    'en': "🚀 Enter <u>start-words</u> <b>via</b> spaces or separators to <i>add</i> them to Base{0}",
+    'es': "🚀 Ingrese <u>palabras de inicio</u> <b>mediante</b> espacios o separadores para <i>agregarlos</i> a la Base{0}",
+    'fr': "🚀 Saisissez des <u>start-words</u> <b>via</b> des espaces ou des séparateurs pour les <i>ajouter</i> à Base{0}",
+    'zh': "🚀 輸入 <u>start-words</u> <b>via</b> 空格或分隔符以將它們<i>添加</i>到 Base{0}",
+    'ar': "✅ أدخل كلمات البداية عبر مسافات أو فواصل من أجل <i> إضافتها </i> إلى القاعدة {0}",
+}
+l_cstartoperation_noanswer = {
+    'ru': "🚫 Введи <u>старт-слова</u> <b>через</b> пробелы или разделители, чтобы их <i>удалить</i> из базы{0}",
+    'en': "🚫 Enter <u>start-words</u> <b>via</b> spaces or separators to <i>remove</i> them from Base{0}",
+    'es': "🚫 Ingrese <u>palabras de inicio</u> <b>mediante</b> espacios o separadores para <i>eliminarlos</i> de la Base{0}",
+    'fr': "🚫 輸入 <u>start-words</u> <b>via</b> 空格或分隔符以將它們從 Base 中<i>刪除</i>{0}",
+    'zh': "🚫 輸入 <u>start-words</u> <b>via</b> 空格或分隔符以將它們從 Base 中<i>刪除</i>{0}",
+    'ar': "🚫 أدخل كلمات البداية عبر مسافات أو فواصل <i> لإزالتها </i> من Base {0}",
+}
+l_fsm_start_add_caption = {
+    'ru': "🚀 Готово! <b>Текущее</b> количество старт-слов для поста #{0} в <code>{1}</code>-файле: <u>{2}</u>",
+    'en': "🚀 Ready! <b>Current</b> number of start-words for post #{0} in <code>{1}</code>-file: <u>{2}</u>",
+    'es': "🚀 Listo! Número <b>actual</b> de palabras de inicio para la publicación #{0} en el archivo <code>{1}</code>: <u>{2}</u>",
+    'fr': "🚀 Prêt ! <b>Nombre actuel</b> de mots de départ pour le message  #{0} dans le fichier <code>{1}</code> : <u>{2}</u>",
+    'zh': "🚀 準備好了！ <code>{1}</code>-文件中帖子 #{0} 的<b>當前</b> 起始字數：<u>{2}</u>",
+    'ar': "🚀 جاهز! <b> العدد </b> الحالي لكلمات البداية للمشاركة # {0} في <code>{1}</code> -ملف:<u>{2}</u>",
+}
+l_fsm_start_add_text = {
+    'ru': "🚀 Готово! <b>Текущее</b> количество старт-слов для поста #{0}: <u>{1}</u>",
+    'en': "🚀 Ready! <b>Current</b> number of start-words for post #{0} <u>{1}</u>",
+    'es': "🚀 Listo! <b>Número actual</b> de palabras de inicio para la publicación #{0} <u>{1}</u>",
+    'fr': "🚀 Prêt ! <b>Nombre actuel</b> de mots de départ pour le message  #{0} <u>{1}</u>",
+    'zh': "🚀 準備好了！ <b>當前</b>帖子#{0}的起始詞數 <u>{1}</u>",
+    'ar': "🚀 جاهز! <b> العدد </b> الحالي لكلمات البداية للمشاركة # {0} <u> {1} </u>",
+}
+l_need_start_word = {
+    'ru': f"🚀 Сначала добавь хотя бы одно старт-слово",
+    'en': "🚀 Ready! <b>Current</b> number of start-words for post #{0} <u>{1}</u>",
+    'es': "🚀 Listo! <b>Número actual</b> de palabras de inicio para la publicación #{0} <u>{1}</u>",
+    'fr': "🚀 Prêt ! <b>Nombre actuel</b> de mots de départ pour le message  #{0} <u>{1}</u>",
+    'zh': "🚀 準備好了！ <b>當前</b>帖子#{0}的起始詞數 <u>{1}</u>",
+    'ar': "🚀 جاهز! <b> العدد </b> الحالي لكلمات البداية للمشاركة # {0} <u> {1} </u>",
+}
+
+# endregion
+
+
+# region cstop_
+l_cstop_text = {
+    'ru': "🧾 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-удаление сообщений, содержащие запрещенные стоп-слова\n\n👉🏼 Текущее количество стоп-слов <u>{0}</u>",
+    'en': "🧾 Push the ✅/☑️, to <b>On/Off</b> auto-delete of messages, containing prohibited stop-words\n\n👉🏼 Current number of stop-words <u>{0}</u>",
+    'es': "🧾 Pulsa ✅/☑️ para <b>activar/desactivar</b> la eliminación automática de mensajes que contengan palabras vacías prohibidas\n\n👉🏼 Número actual de palabras vacías <u>{0}</u>",
+    'fr': "🧾 Appuyez sur ✅/☑️, pour <b>Activer/Désactiver</b> la suppression automatique des messages contenant des mots vides interdits\n\n👉🏼 Nombre actuel de mots vides <u>{0}</u>",
+    'zh': "🧾 按下 ✅/☑️, 以<b>開/關</b>自動刪除包含禁止停用詞的消息\n\n👉🏼 當前停用詞數量<u>{0}</u>",
+    'ar': "🧾 اضغط على ✅ / ☑️ ، من أجل <b> تشغيل / إيقاف </b> للحذف التلقائي للرسائل ، التي تحتوي على كلمات إيقاف محظورة \n\n👉🏼 العدد الحالي لكلمات التوقف <u>{0}</u>",
+}
+l_cstop_call = {
+    'ru': "🔔 Нужно ⚙️Настроить хотя бы одно стоп-слово",
+    'en': "🔔 You have to  ⚙️Configure at least one stop-word",
+    'es': "🔔 Tienes que ⚙️Configurar al menos una palabra vacía",
+    'fr': "🔔 Vous devez ⚙️Configurer au moins un mot vide",
+    'zh': "🔔 你必須⚙️至少配置一個停用詞",
+    'ar': "🔔 يجب عليك ⚙️ تكوين كلمة توقف واحدة على الأقل",
+}
+l_cstopchange_caption = {
+    'ru': "🧾 Текущее количество стоп-слов в <code>{0}</code>-файле: <u>{1}</u>\n\nЖми на ✅/🚫, чтобы <b>Добавить/Удалить</b> стоп-слова",
+    'en': "🧾 Current number of stop-words in <code>{0}</code>-file: <u>{1}</u>\n\nPush the ✅/🚫, to <b>Add/Remove</b> stop-words",
+    'es': "🧾 Número actual de palabras vacías en el archivo <code>{0}</code>: <u>{1}</u>\n\nPresione ✅/🚫 para <b>Agregar/Quitar</b> palabras vacías",
+    'fr': "🧾 Nombre actuel de mots vides dans le fichier <code>{0}</code> : <u>{1}</u>\n\nAppuyez sur ✅/🚫 pour <b>Ajouter/Supprimer</b> mots vides",
+    'zh': "🧾 <code>{0}</code>-文件中當前停用詞的數量：<u>{1}</u>\n\n將 ✅/🚫 推到 <b>添加/刪除</b> 停用詞",
+    'ar': "🧾 العدد الحالي لكلمات الإيقاف في <code>{0}</code> -الملف:{1}\n\n اضغط على ✅/🚫 ، من أجل إضافة / إزالة توقف الكلمات",
+}
+l_cstopchange_text = {
+    'ru': "🧾 Текущее количество стоп-слов <u>{0}</u>\n\nЖми на ✅/🚫, чтобы <b>Добавить/Удалить</b> стоп-слова",
+    'en': "🧾 Current number of stop-words: <u>{1}</u>\n\nPush the ✅/🚫, to <b>Add/Remove</b> stop-words",
+    'es': "🧾 Número actual de palabras vacías: <u>{1}</u>\n\nPresione ✅/🚫 para <b>Agregar/Quitar</b> palabras vacías",
+    'fr': "🧾 Nombre actuel de mots vides : <u>{1}</u>\n\nAppuyez sur ✅/🚫 pour <b>ajouter/supprimer</b> des mots vides",
+    'zh': "🧾 當前停用詞數量：<u>{1}</u>\n\n按下 ✅/🚫, 以<b>添加/刪除</b>停用詞",
+    'ar': "🧾 العدد الحالي لكلمات التوقف: <u>{1}</u>\n\n اضغط على ✅/🚫 ، من أجل <b> إضافة / إزالة <b/> كلمات الإيقاف",
+}
+l_cstopchange_add = {
+    'ru': "\n\n▪️регистр не важен\n▪️поставь звездочку после слова, чтобы учитывать вхождение\n▪️например, если ввести <b>психо*</b>, то будут удаляться <u>все</u> сообщения, которые <b>содержат</b> данное сочетание: <i>анти<u>психо</u>лог, <u>Психо</u>терапевт..</i>",
+    'en': "\n\n▪️word case is not important\n▪️set * after word to account for occurrence\n▪️for example, if write <b>psy*</b>, then <u>all</u> messages, which are <b>contained</b> this combination of letters will be removed: <i>anti-<u>psy</u>chologist, <u>Psy</u>chotherapist..</i>",
+    'es': "\n\n▪️las mayúsculas y minúsculas no son importantes\n▪️establezca * después de la palabra para tener en cuenta la ocurrencia\n▪️por ejemplo, si escribe <b>psi*</b>, entonces <u>todos</u> los mensajes, que están <b>contenidos</b> se eliminará esta combinación de letras: <i>anti-<u>psicólogo</u>, <u>Psi</u>coterapeuta..</i>",
+    'fr': "\n\n▪️la casse des mots n'est pas importante\n▪️définissez * après le mot pour tenir compte de l'occurrence\n▪️par exemple, si écrivez <b>psy*</b>, alors <u>tous</u> les messages, qui sont <b>contenues</b> cette combinaison de lettres sera supprimée : <i>anti-<u>psychologue</u>, <u>Psy</u>chothérapeute..</i>",
+    'zh': "\n\n▪️單詞大小寫不重要\n▪️在單詞之後設置*以說明出現\n▪️例如，如果寫<b>psy*</b>，則<u>所有</u>消息， <b>包含</b>這些字母組合將被刪除：<i>anti-<u>psy</u>chologist, <u>Psy</u>chotherapy..</i>",
+    'ar': "\n\n▪️ حالة الكلمة ليست مهمة \n▪️ اضبط * بعد كلمة لحساب الحدوث \n▪️ على سبيل المثال ، إذا كتبت <b>psy*</b> ، ثم <u> كل </u> الرسائل ، التي <b> احتوت </b> ستتم إزالة هذه المجموعة من الأحرف:",
+}
+l_cstopchange_answer = {
+    'ru': "✅ Введи <u>стоп-слова</u> <b>через</b> пробелы или разделители, чтобы <i>добавить</i> их в базу{0}",
+    'en': "✅ Enter <u>stop-words</u> <b>via</b> spaces or separators to <i>add</i> them to Base{0}",
+    'es': "✅ Ingrese <u>palabras vacías</u> <b>a través de</b> espacios o separadores para <i>agregarlos</i> a la Base{0}",
+    'fr': "✅ Saisissez des <u>mots vides</u> <b>via</b> des espaces ou des séparateurs pour les <i>ajouter</i> à Base{0}",
+    'zh': "✅ 輸入 <u>停用詞</u> <b>通過</b> 空格或分隔符將它們<i>添加</i>到 Base{0}",
+    'ar': "✅ أدخل <u> كلمات الإيقاف </u> <b> عبر </b> مسافات أو فواصل من أجل <i> إضافتها </i> إلى القاعدة {0}",
+}
+l_cstopchange_noanswer = {
+    'ru': "🚫 Введи <u>стоп-слова</u> <b>через</b> пробелы или разделители, чтобы их <i>удалить</i> из базы{0}",
+    'en': "🚫 Enter <u>stop-words</u> <b>via</b> spaces or separators to <i>removed </i> them from Base{0}",
+    'es': "🚫 Ingrese <u>palabras vacías</u> <b>a través de</b> espacios o separadores para <i>eliminarlos </i> de la base {0}",
+    'fr': "🚫 Saisissez des <u>mots vides</u> <b>via</b> des espaces ou des séparateurs pour les <i>supprimer </i> de Base {0}",
+    'zh': "🚫 輸入 <u>stop-words</u> <b>via</b> 空格或分隔符以將它們從 Base 中<i>刪除 </i>{0}",
+    'ar': "🚫 أدخل <u> كلمات الإيقاف </u> <b> عبر </b> مسافات أو فواصل لـ <i> إزالتها </i> من Base {0}",
+}
+l_fsm_stop_add_caption = {
+    'ru': "🧾 Готово! <b>Текущее</b> количество стоп-слов в <code>{0}</code>-файле: <u>{1}</u>",
+    'en': "🧾 Ready! <b>Current</b> number of stop-words in <code>{0}</code>-file: <u>{1}</u>",
+    'es': "🧾 Listo! Número <b>actual</b> de palabras vacías en el archivo <code>{0}</code>: <u>{1}</u>",
+    'fr': "🧾 Prêt ! <b>Nombre actuel</b> de mots vides dans le fichier <code>{0}</code> : <u>{1}</u>",
+    'zh': "🧾 準備好了！ <b>當前</b> <code>{0}</code>-文件中的停用詞數：<u>{1}</u>",
+    'ar': "🧾 جاهز! <b> العدد </b> الحالي لكلمات التوقف في <code>{0}</code> -الملف: <u>{1}</u>",
+}
+l_fsm_stop_add_text = {
+    'ru': "🧾 Готово! <b>Текущее</b> количество стоп-слов <u>{0}</u>",
+    'en': "🧾 Ready! <b>Current</b> number of stop-words <u>{0}</u>",
+    'es': "🧾 Listo! <b>Número actual</b> de palabras vacías <u>{0}</u>",
+    'fr': "🧾 Prêt ! <b>Nombre actuel</b> de mots vides <u>{0}</u>",
+    'zh': "🧾準備好了！ <b>當前</b>停用詞數<u>{0}</u>",
+    'ar': "🧾 جاهز! <b> العدد </b> الحالي لكلمات التوقف <u>{0}</u>",
+}
+# endregion
+
+
+# region cflood_
+l_cflood_text = {
+    'ru': "💬 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> <i>проверку</i> на частоту подряд написанных сообщ за один промежуток времени\n\n👉🏼 Например, задай количество сообщ подряд, которое будет считаться флудом командой: <code>/flood 5</code>\n\n👉🏼 Или используй <b>медленный режим</b> в настройках группы для <u>1</u> сообщения",
+    'en': "💬 Push the ✅/☑️, to <b>On/Off</b> messages frequency-<i>checking</i> in one period of time\n\n👉🏼 For example, specify the number of consecutive messages that will be considered as flood by the command: <code>/flood 5</code>\n\n👉🏼 Or use <b>Slow Mode</b> in the Settings of group for <u>1</u> message",
+    'es': "💬 Presiona ✅/☑️, para <b>Activar/Desactivar</b> la frecuencia de mensajes-<i>comprobar</i> en un período de tiempo\n\n👉🏼 Por ejemplo, especifica la cantidad de mensajes consecutivos que será considerado como inundación por el comando: <code>/flood 5</code>\n\n👉🏼 O use <b>Modo lento</b> en la Configuración del grupo para <u>1</u> mensaje",
+    'fr': "💬 Appuyez sur ✅/☑️, pour <b>Activer/Désactiver</b> la fréquence des messages-<i>vérification</i> dans une période de temps\n\n👉🏼 Par exemple, spécifiez le nombre de messages consécutifs qui sera considéré comme une inondation par la commande : <code>/flood 5</code>\n\n👉🏼 Ou utilisez le <b>mode lent</b> dans les paramètres du groupe pour <u>1</u> message",
+    'zh': "💬 推 ✅/☑️, 到 <b>On/Off</b> 消息頻率-<i>檢查</i> 在一個時間段內\n\n👉🏼 例如，指定連續消息的數量 將被命令視為洪水： <code>/flood 5</code>\n\n👉🏼 或者在 <u>1</u> 的組的設置中使用 <b>Slow Mode</b> 信息",
+    'ar': "💬 ادفع ✅ / ☑️ إلى تردد رسائل <b> تشغيل / إيقاف </b> - <i> التحقق </i> في فترة زمنية واحدة \n\n👉🏼 على سبيل المثال ، حدد عدد الرسائل المتتالية التي سيتم اعتباره فيضانًا بواسطة الأمر: <code> / Flood 5 </code> \n\n👉🏼 أو استخدم <b> الوضع البطيء </b> في إعدادات المجموعة لـ <u> 1 </u> رسالة",
+}
+l_cflood_count_on = {
+    'ru': "✅☑Вкл {0} сообщ",
+    'en': "✅☑On {0} msgs",
+    'es': "✅☑En {0} mensajes",
+    'fr': "✅☑En {0} messages",
+    'zh': "✅☑使能夠 {0} 消息",
+    'ar': "✅☑يُمكَِن {0} رسائل",
+}
+l_cflood_count_off = {
+    'ru': "☑️☐Выкл {0} сообщ",
+    'en': "☑️☐Off {0} msgs",
+    'es': "☑️☐De {0} mensajes",
+    'fr': "☑️☐De {0} messages",
+    'zh': "☑️☐禁用 {0} 消息",
+    'ar': "☑️☐ تعطيل {0} رسائل",
+}
+# endregion
+
+
+# region cuser_
+l_cuser_text = {
+    'ru': "👥 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> первичную <i>задержку/свободный вход без входного контроля для premium-аккаунтов/разрешение на инвайт</i> пользователей/ботов в группу или разрешение на <i>редактирование</i> сообщений\n\n👉🏼 Например, <b>задержка</b> (<i>в мин</i>) для <u>новых</u> пользователей (перед написанием их <u>1</u>го сообщ) осуществляется командой: <code>/delay  {0}</code>",
+    'en': "👥 Push the ✅/☑️, to <b>On/Off</b> primary <i>delay/free entrance without Enter Control for premium-accounts/permission for inviting</i> users/bots in group or permission to <i>edit</i> messages\n\n👉🏼 For example, <b>delay</b> (<i>in minutes</i>) for <u>new</u> users (before writing their <u>1</u>st message) executed by: <code>/delay  {0}</code>",
+    'es': "👥 Presione ✅/☑️, para <b>Encender/Apagar</b> <i>retraso/entrada gratuita principal sin control de entrada para cuentas premium/permiso para invitar</i> usuarios/bots en grupo o permiso para <i>editar</i> mensajes\n\n👉🏼 Por ejemplo, <b>retraso</b> (<i>en minutos</i>) para <u>nuevos</u> usuarios (antes de escribir su <u>1</u>st mensaje) ejecutado por: <code>/delay {0}</code>",
+    'fr': "👥 Appuyez sur ✅/☑️, pour <b>On/Off</b> le <i>retard principal/l'entrée gratuite sans Enter Control pour les comptes premium/l'autorisation d'inviter</i> les utilisateurs/bots en groupe ou l'autorisation de <i>modifier</i> les messages\n\n👉🏼 Par exemple, <b>délai</b> (<i>en minutes</i>) pour les <u>nouveaux</u> utilisateurs (avant d'écrire leur <u>1</u>er message) exécuté par : <code>/delay {0}</code>",
+    'zh': "👥 按下 ✅/☑️，以 <b>開/關</b> 主要 <i>延遲/免費進入，無需進入高級帳戶控制/邀請</i>組中的用戶/機器人或權限<i>編輯</i>消息\n\n👉🏼例如，<u>新</u>用戶的<b>延遲</b>（<i>分鐘</i>）（在編寫他們的 <u>1</u>st message) 執行者：<code>/delay {0}</code>",
+    'ar': "👥 اضغط على ✅ / ☑️ ، لـ <b> تشغيل / إيقاف </b> <i> تأخير / دخول مجاني بدون Enter Control للحسابات المميزة / إذن لدعوة </i> المستخدمين / الروبوتات في مجموعة أو إذن لـ <i> تحرير الرسائل </i> \n\n👉🏼 على سبيل المثال ، <b> تأخير </b> (<i> بالدقائق </i>) للمستخدمين <u> الجدد </u> (قبل كتابة <u> 1 </u> st) بواسطة: <code> / delay {0}</code>",
+}
+l_cuser_call = {
+    'ru': "👮🏽 В настройках [Разрешения] включи опцию:\n\n[✅ Добавление участ]\n\n🕚Подожди 1min",
+    'en': "👮🏽 In the Settings [Permissions] enable:\n\n[✅ Add members]\n🕚Wait for 1min",
+    'es': "👮🏽 En la Configuración [Permisos] habilite:\n\n[✅ Agregar miembros]\n🕚Espere 1 minuto",
+    'fr': "👮🏽 Dans les paramètres [Autorisations], activez :\n\n[✅ Ajouter des membres]\n🕚Attendez 1 min",
+    'zh': "👮🏽在設置[權限]中啟用：\n\n[✅添加成員]\n🕚等待1分鐘",
+    'ar': "👮🏽 في الإعدادات [الأذونات] ، قم بتمكين: \n\n [✅ إضافة أعضاء] \n🕚 انتظر لمدة دقيقة واحدة",
+}
+l_cuser_delay_on = {
+    'ru': "✅☑Вкл задержку {0}min",
+    'en': "✅☑On delay {0}min",
+    'es': "✅☑En demora {0}min",
+    'fr': "✅☑En retard {0}min",
+    'zh': "✅☑使能夠 延遲 {0}min",
+    'ar': "✅☑يُمكَِن تأخير {0}min",
+}
+l_cuser_delay_off = {
+    'ru': "☑️☐Выкл задержку {0}min",
+    'en': "☑️☐Off delay {0}min",
+    'es': "☑️☐De demora {0}min",
+    'fr': "☑️☐De retard {0}min",
+    'zh': "☑️☐禁用 延遲 {0}min",
+    'ar': "☑️☐ تعطيل تأخير {0}min",
+}
+l_cuser_invite_user_on = {
+    'ru': "✅☑Вкл инвайт польз.",
+    'en': "✅☑On invite users",
+    'es': "✅☑En invitar a los usuarios",
+    'fr': "✅☑En inviter des utilisateurs",
+    'zh': "✅☑使能夠 邀請用戶",
+    'ar': "✅☑يُمكَِندعوة المستخدمين",
+}
+l_cuser_invite_user_off = {
+    'ru': "☑️☐Выкл инвайт польз.",
+    'en': "☑️☐Off invite users",
+    'es': "☑️☐De invitar a los usuarios",
+    'fr': "☑️☐De inviter des utilisateurs",
+    'zh': "☑️☐禁用 邀請用戶",
+    'ar': "☑️☐ تعطيل دعوة المستخدمين",
+}
+
+l_cuser_invite_bot_on = {
+    'ru': "✅☑Вкл инвайт ботов",
+    'en': "✅☑On invite bots",
+    'es': "✅☑En invitar robots",
+    'fr': "✅☑En inviter des robots",
+    'zh': "✅☑使能夠 邀請機器人",
+    'ar': "✅☑يُمكَِندعوة دعوة الروبوتات",
+}
+l_cuser_invite_bot_off = {
+    'ru': "☑️☐Выкл инвайт ботов",
+    'en': "☑️☐Off invite bots",
+    'es': "☑️☐De invitar robots",
+    'fr': "☑️☐De inviter des robots",
+    'zh': "☑️☐禁用 邀請機器人",
+    'ar': "☑️☐ تعطيل دعوة الروبوتات",
+}
+l_cuser_premium_on = {
+    'ru': "✅☑Вкл premium-вход",
+    'en': "✅☑On premium-entrance",
+    'es': "✅☑En entrada premium",
+    'fr': "✅☑En entrée premium",
+    'zh': "✅☑使能夠 高級入口",
+    'ar': "✅☑ يُمكَِندعوة دخول ممتاز",
+}
+l_cuser_premium_off = {
+    'ru': "☑️☐Выкл premium-вход",
+    'en': "☑️☐Off premium-entrance",
+    'es': "☑️☐De entrada premium",
+    'fr': "☑️☐De entrée premium",
+    'zh': "☑️☐禁用 高級入口",
+    'ar': "☑️☐ تعطيل دخول ممتاز",
+}
+l_cuser_edit_on = {
+    'ru': "✅☑Вкл редактирование сообщ",
+    'en': "✅☑On edit msg",
+    'es': "✅☑En editar mensaje",
+    'fr': "✅☑En editar mensaje",
+    'zh': "✅☑使能夠 編輯消息",
+    'ar': "✅☑ يُمكَِندعوة تحرير الرسالة",
+}
+l_cuser_edit_off = {
+    'ru': "☑️☐Выкл редактирование сообщ",
+    'en': "☑️☐Off edit msg",
+    'es': "☑️☐De editar mensaje",
+    'fr': "☑️☐De entrée premium",
+    'zh': "☑️☐禁用 編輯消息",
+    'ar': "☑️☐ تعطيل تحرير الرسالة",
+}
+# endregion
+
+
+# region cadmin_
+l_cadmin_text = {
+    'ru': "👩🏽‍💻 Жми на ✅/☑️, чтобы <b>Вкл/Выкл</b> <u>admin-доступ</u> (только к /cmd-командам для <i>других</i> администраторов) и <u>god-режим</u> (без ограничений для администраторов)\n\n👉🏼 <b>Текущие администраторы</b>:\n{0}",
+    'en': "👩🏽‍💻 Push the ✅/☑️, to <b>On/Off</b> <u>admin-access</u> (to /cmd-commands for <i>other</i> admins) and <u>god-mode</u> (without limits for you and group-creator)\n\n👉🏼 <b>Current administrators</b>:\n{0}",
+    'es': "👩🏽‍💻 Presiona ✅/☑️, para <b>Activar/Desactivar</b> <u>acceso de administrador</u> (para /cmd-comandos para <i>otros</i> administradores) y <u>modo dios</u> (sin límites para ti y el creador del grupo)\n\n👉🏼 <b>Administradores actuales</b>:\n{0}",
+    'fr': "👩🏽‍💻 Appuyez sur ✅/☑️, pour <b>On/Off</b> <u>admin-access</u> (vers /cmd-commands pour les <i>autres</i> admins) et <u>god-mode</u> (sans limites pour vous et le créateur de groupe)\n\n👉🏼 <b>Administrateurs actuels</b> :\n{0}",
+    'zh': "👩🏽‍💻 按下 ✅/☑️，到 <b>On/Off</b> <u>admin-access</u>（到 <i>other</i> 管理員的 /cmd-commands）和 <u>上帝模式</u>（對您和群組創建者沒有限制）\n\n👉🏼 <b>當前管理員</b>：\n{0}",
+    'ar': "👩🏽‍💻 اضغط على ✅ / ☑️ ، من أجل <b> تشغيل / إيقاف </b> <u> وصول المشرف </u> (أوامر /cmd لـ <i> مشرفين آخرين </i>) و <u> god-mode </u> (بلا حدود لك ولمنشئ المجموعة) \n \n👉🏼 <b> المسؤولون الحاليون </b>: \n {0}",
+}
+l_cadmin_admin_on = {
+    'ru': "✅☑Вкл admin-доступ",
+    'en': "✅☑On admin-access",
+    'es': "✅☑En acceso de administrador",
+    'fr': "✅☑En accès administrateur",
+    'zh': "✅☑啟用管理員訪問",
+    'ar': "✅☑ تمكين وصول المسؤول",
+}
+l_cadmin_admin_off = {
+    'ru': "☑️☐Выкл admin-доступ",
+    'en': "☑️☐Off admin-access",
+    'es': "☑️☐De acceso de administrador",
+    'fr': "☑️☐De accès administrateur",
+    'zh': "☑️☐禁用管理員訪問",
+    'ar': "☑️☐ تعطيل وصول المسؤول",
+}
+l_cadmin_god_on = {
+    'ru': "✅☑Вкл god-режим",
+    'en': "✅☑On god-mode",
+    'es': "✅☑En modo de Dios",
+    'fr': "✅☑En mode divin",
+    'zh': "✅☑開啟上帝模式",
+    'ar': "✅☑ تمكين وضع الله",
+}
+l_cadmin_god_off = {
+    'ru': "☑️☐Выкл god-режим",
+    'en': "☑️☐Off god-mode",
+    'es': "☑️☐De modo de Dios",
+    'fr': "☑️☐De mode divin",
+    'zh': "☑️☐禁用上帝模式",
+    'ar': "☑️☐ تعطيل وضع الله",
+}
+# endregion
+
+
+# region handlers
+l_content_types_invite_user_bot = {
+    'ru': "🚶🏽 Инвайт @username/@name_bot не разрешены",
+    'en': "🚶🏽 Inviting of @username/@name_bot is not allowed",
+    'es': "🚶🏽 No se permite invitar a @username/@name_bot",
+    'fr': "🚶🏽 L'invitation de @username/@name_bot n'est pas autorisée",
+    'zh': "🚶🏽 不允許邀請 @username/@name_bot",
+    'ar': "🚶🏽 دعوة @ username / @ name_bot غير مسموح بها",
+}
+l_content_types_invite_user = {
+    'ru': "🚶🏽 Инвайт @username не разрешен",
+    'en': "🚶🏽 Inviting of @username is not allowed",
+    'es': "🚶🏽 No se permite invitar a @username",
+    'fr': "🚶🏽 L'invitation de @username n'est pas autorisée",
+    'zh': "🚶🏽 不允許邀請 @username",
+    'ar': "🚶🏽 دعوة @username غير مسموح بها",
+}
+l_content_types_invite_bot = {
+    'ru': "🚶🏽 Инвайт @name_bot не разрешен",
+    'en': "🚶🏽 Inviting of @name_bot is not allowed",
+    'es': "🚶🏽 No se permite invitar a @name_bot",
+    'fr': "🚶🏽 L'invitation de @name_bot n'est pas autorisée",
+    'zh': "🚶🏽 不允許邀請 @name_bot",
+    'ar': "🚶🏽 دعوة @name_bot غير مسموح بها",
+}
+l_content_types_button = {
+    'ru': "👮🏽 {0}, нажми на кнопку, чтобы вс︎тупить в группу",
+    'en': "👮🏽 {0}, push the button to join the group",
+    'es': "👮🏽 {0}, presiona el botón para unirte al grupo",
+    'fr': "👮🏽 {0}, appuyez sur le bouton pour rejoindre le groupe",
+    'zh': "👮🏽 {0}，按按鈕加入群組",
+    'ar': "👮🏽 {0} ، اضغط على الزر للانضمام إلى المجموعة",
+}
+l_content_types_captcha = {
+    'ru': "👮🏽 {0}, выбери <i>правильный вариант</i> ответа, чтобы вс︎тупить в группу:\n\n<code>{1}</code>",
+    'en': "👮🏽 {0}, choose <i>correct option</i> to join the group:\n\n<code>{1}</code>",
+    'es': "👮🏽 {0}, elige la <i>opción correcta</i> para unirte al grupo:\n\n<code>{1}</code>",
+    'fr': "👮🏽 {0}, choisissez la <i>bonne option</i> pour rejoindre le groupe :\n\n<code>{1}</code>",
+    'zh': "👮🏽 {0}，選擇<i>正確選項</i>加入群組：\n\n<code>{1}</code>",
+    'ar': "👮🏽 {0} اختر <i> الخيار الصحيح </i> للانضمام إلى المجموعة: \n\n <code>{1}</code>",
+}
+l_hand_msg_FLOOD_USERNAME = {
+    'ru': "💬 Пользователь @{0} изменил <b>name/@username</b>! Возможно, шпион!",
+    'en': "💬 User @{0} change the <b>name/@username</b>! Possibly a spy!",
+    'es': "💬 ¡Usuario @{0} cambia el <b>nombre/@nombre de usuario</b>! ¡Posiblemente un espía!",
+    'fr': "💬 L'utilisateur @{0} change le <b>nom/@nom d'utilisateur</b> ! Peut-être un espion !",
+    'zh': "💬 用戶@{0} 更改<b>名稱/@用戶名</b>！ 可能是間諜！",
+    'ar': "💬 المستخدم @{0} غيّر <b> الاسم / @ اسم المستخدم </b>! ربما جاسوس!",
+}
+l_hand_msg_flood = {
+    'ru': "💬 <i>Flood</i>-сообщения",
+    'en': "💬 <i>Flood</i>-messages",
+    'es': "💬 <i>Flood</i>-mensajes",
+    'fr': "💬 <i>Flood</i>-messages",
+    'zh': "💬 <i>Flood</i>-消息",
+    'ar': "💬 <i>Flood</i>-رسائل",
+}
+l_hand_msg_via_bot = {
+    'ru': "🗣 Сообщения <i>от имени бота</i> не разрешены",
+    'en': "🗣 Messages <i>via bot</i> are not allowed",
+    'es': "🗣 Les messages <i>via bot</i> ne sont pas autorisés",
+    'fr': "🗣 Les messages <i>via bot</i> ne sont pas autorisés",
+    'zh': "🗣 消息<i>通過機器人</i>是不允許的",
+    'ar': "🗣 الرسائل <i> عبر البوت </i> غير مسموح بها",
+}
+l_hand_msg_channel = {
+    'ru': "🫥 Сообщения <i>от имени канала</i> не разрешены",
+    'en': "🫥 Messages <i>as channel name</i> are not allowed",
+    'es': "🫥 No se permiten mensajes <i>como nombre del canal</i>",
+    'fr': "🫥 Les messages <i>comme nom de chaîne</i> ne sont pas autorisés",
+    'zh': "🫥 消息<i>作為頻道名稱</i>是不允許的",
+    'ar': "🫥 الرسائل <i> كاسم قناة </i> غير مسموح بها",
+}
+l_hand_msg_emoji = {
+    'ru': "🗣 Сообщения <i>c emoji</i> не разрешены",
+    'en': "🗣 Messages <i>with emoji</i> are not allowed",
+    'es': "🗣 No se permiten mensajes <i>con emoji</i>",
+    'fr': "🗣 Les messages <i>avec emoji</i> ne sont pas autorisés",
+    'zh': "🗣 不允許<i>帶有表情符號</i>的消息",
+    'ar': "🗣 غير مسموح بالرسائل <i> ذات الرموز التعبيرية </i>",
+}
+l_hand_msg_http = {
+    'ru': "🔗 Сообщения <i>c внешними ссылками</i> не разрешены",
+    'en': "🔗 Messages <i>with external links</i> are not allowed",
+    'es': "🔗 No se permiten mensajes <i>con enlaces externos</i>",
+    'fr': "🔗 Les messages <i>avec des liens externes</i> ne sont pas autorisés",
+    'zh': "🔗 不允許<i>帶有外部鏈接</i>的消息",
+    'ar': "🔗 الرسائل <i> ذات الروابط الخارجية </i> غير مسموح بها",
+}
+l_hand_msg_telegram = {
+    'ru': "🔗 Сообщения <i>c telegram-ссылками</i> не разрешены",
+    'en': "🔗 Messages <i>with telegram-links</i> are not allowed",
+    'es': "🔗 Mensajes <i>con enlaces de Telegram</i> no están permitidos",
+    'fr': "🔗 Les messages <i>avec des liens de télégramme</i> ne sont pas autorisés",
+    'zh': "🔗 不允許<i>帶有電報鏈接</i>的消息",
+    'ar': "🔗 الرسائل <i> التي تحتوي على روابط برقية </i> غير مسموح بها",
+}
+l_hand_msg_forward = {
+    'ru': "🔗 Сообщения <i>c forward-ссылками</i> не разрешены",
+    'en': "🔗 Messages <i>with forward-links</i> are not allowed",
+    'es': "🔗 No se permiten mensajes <i>con enlaces hacia adelante</i>",
+    'fr': "🔗 Les messages <i>avec des liens vers l'avant</i> ne sont pas autorisés",
+    'zh': "🔗 不允許<i>帶有轉發鏈接</i>的消息",
+    'ar': "🔗 الرسائل <i> ذات الروابط الأمامية </i> غير مسموح بها",
+}
+l_hand_msg_zalgo = {
+    'ru': "文 Сообщения <i>c <a href='https://www.zalgo.org'>zalgo-символами</a></i> не разрешены",
+    'en': "文 Messages <i>with <a href='https://www.zalgo.org'>zalgo-symbols</a></i> are not allowed",
+    'es': "文 Mensajes <i>con <a href='https://www.zalgo.org'>símbolos-zalgo</a></i> no están permitidos",
+    'fr': "文 Les messages <i>avec <a href='https://www.zalgo.org'>symboles zalgo</a></i> ne sont pas autorisés",
+    'zh': "<i>帶有<a href='https://www.zalgo.org'>zalgo-symbols</a></i>的消息是不允許的",
+    'ar': "文 الرسائل <i> التي تحتوي على <a href='https://www.zalgo.org'> رموز zalgo </a> </i> غير مسموح بها",
+}
+l_hand_msg_symbols = {
+    'ru': "文 Сообщения <i>c 文ب-алфавитами</i> не разрешены",
+    'en': "文 Messages <i>with 文ب-alphabet</i> are not allowed",
+    'es': "文 Mensajes <i>con 文ب-alfabeto</i> no están permitidos",
+    'fr': "文 Les messages <i>avec l'alphabet 文ب</i> ne sont pas autorisés",
+    'zh': "不允許<i>帶有文ب-alphabet</i>的文消息",
+    'ar': "文 الرسائل <i> التي تحتوي على 文 ب- الأبجدية </i> غير مسموح بها",
+}
+l_hand_msg_stop = {
+    'ru': "🧾 Сообщение содержит <i>стоп-слова</i>",
+    'en': "🧾 Message contains <i>stop-words</i>",
+    'es': "🧾 El mensaje contiene <i>palabras vacías</i>",
+    'fr': "🧾 Le message contient des <i>mots vides</i>",
+    'zh': "🧾 消息包含 <i>停用詞</i>",
+    'ar': "🧾 تحتوي الرسالة على <i> كلمات التوقف </i>",
+}
+l_hand_msg_edit = {
+    'ru': "👥 <i>Редактирование</i> сообщений не разрешено",
+    'en': "👥 Message <i>editing</i> is not allowed",
+    'es': "👥 La <i>edición</i> de mensajes no está permitida",
+    'fr': "👥 La <i>modification</i> des messages n'est pas autorisée",
+    'zh': "👥 消息<i>編輯</i>是不允許的",
+    'ar': "👥 رسالة <i> تحرير </i> غير مسموح بها",
+}
+l_scheduler_autoinvite_is_over = {
+    'ru': "🚶🏽 Закончились пользователи для инвайта в группе {0}",
+    'en': "🚶🏽 Users for the invite in the {0} group have ended",
+    'es': "🚶🏽 Los usuarios de la invitación en el grupo {0} han terminado",
+    'fr': "🚶🏽 Les utilisateurs de l'invitation dans le groupe {0} sont terminés",
+    'zh': "🚶🏽 {0} 組中邀請的用戶已結束",
+    'ar': "🚶🏽 انتهى مستخدمو الدعوة في مجموعة {0}",
+}
+l_scheduler_autoinvite_success = {
+    'ru': "🚶🏽 Успешный инвайт пользователя {0} в группу {1}",
+    'en': "🚶🏽 Successful invite of a user {0} to a {1} group",
+    'es': "🚶🏽 Invitación exitosa de un usuario {0} a un grupo {1}",
+    'fr': "🚶🏽 Invitation réussie d'un utilisateur {0} à un groupe {1}",
+    'zh': "🚶🏽 成功邀請用戶 {0} 加入 {1} 組",
+    'ar': "دعوة ناجحة من مستخدم {0} إلى مجموعة {1}",
+}
+l_hand_msg_photo = {
+    'ru': "🗣 Сообщения <i>с фото</i> не разрешены",
+    'en': "🗣 Messages <i>with photo</i> are not allowed",
+    'es': "🗣 No se permiten mensajes <i>con foto</i>",
+    'fr': "🗣 Les messages <i>avec photo</i> ne sont pas autorisés",
+    'zh': "🗣 不允許<i>帶有照片</i>的消息",
+    'ar': "🗣 الرسائل <i> مع الصورة </i> غير مسموح بها",
+}
+l_hand_msg_video = {
+    'ru': "🗣 Сообщения <i>с видео</i> не разрешены",
+    'en': "🗣 Messages <i>with video</i> are not allowed",
+    'es': "🗣 No se permiten mensajes <i>con video</i>",
+    'fr': "🗣 Les messages <i>avec vidéo</i> ne sont pas autorisés",
+    'zh': "🗣 不允許<i>帶有視頻</i>的消息",
+    'ar': "🗣 الرسائل <i> مع الفيديو </i> غير مسموح بها",
+}
+l_hand_msg_giff = {
+    'ru': "🗣 Сообщения <i>с гиф</i> не разрешены",
+    'en': "🗣 Messages <i>with giff</i> are not allowed",
+    'es': "🗣 No se permiten mensajes <i>con animación</i>",
+    'fr': "🗣 Les messages <i>avec animation</i> ne sont pas autorisés",
+    'zh': "🗣 不允許<i>帶有動畫</i>的消息",
+    'ar': "🗣 الرسائل <i> ذات الرسوم المتحركة </i> غير مسموح بها",
+}
+l_hand_msg_audio = {
+    'ru': "🗣 Сообщения <i>с аудио</i> не разрешены",
+    'en': "🗣 Messages <i>with audio</i> are not allowed",
+    'es': "🗣 No se permiten mensajes <i>con audio</i>",
+    'fr': "🗣 Les messages <i>avec l'audio</i> ne sont pas autorisés",
+    'zh': "🗣 不允許<i>帶有音頻</i>的消息",
+    'ar': "🗣 الرسائل <i> مع الصوت </i> غير مسموح بها",
+}
+l_hand_msg_sticker = {
+    'ru': "🗣 Сообщения <i>со стикерами</i> не разрешены",
+    'en': "🗣 Messages <i>with sticker</i> are not allowed",
+    'es': "🗣 No se permiten mensajes <i>con pegatina</i>",
+    'fr': "🗣 Les messages <i>avec autocollant</i> ne sont pas autorisés",
+    'zh': "🗣 不允許<i>帶有貼紙</i>的消息",
+    'ar': "🗣 الرسائل <i> ذات الملصق </i> غير مسموح بها",
+}
+l_hand_msg_sticker_ex = {
+    'ru': "🗣 Сообщения <i>со стикерами</i> разрешены, но есть исключения",
+    'en': "🗣 Messages <i>with sticker</i> are not allowed, but there are exceptions",
+    'es': "🗣 No se permiten mensajes <i>con sticker</i>, pero hay excepciones",
+    'fr': "🗣 Les messages <i>avec autocollant</i> ne sont pas autorisés, mais il y a des exceptions",
+    'zh': "🗣 不允許<i>帶有貼紙</i>的消息，但也有例外",
+    'ar': "🗣 الرسائل <i> ذات الملصق </i> غير مسموح بها ، ولكن هناك استثناءات",
+}
+l_hand_msg_docum = {
+    'ru': "🗣 Сообщения <i>с документами</i> не разрешены",
+    'en': "🗣 Messages <i>with document</i> are not allowed",
+    'es': "🗣 No se permiten mensajes <i>con documento</i>",
+    'fr': "🗣 Les messages <i>avec document</i> ne sont pas autorisés",
+    'zh': "🗣 不允許<i>帶有文檔</i>的消息",
+    'ar': "🗣 الرسائل <i> مع المستند </i> غير مسموح بها",
+}
+l_hand_msg_poll = {
+    'ru': "🗣 Сообщения <i>с опросами</i> не разрешены",
+    'en': "🗣 Messages <i>with poll</i> are not allowed",
+    'es': "🗣 No se permiten mensajes <i>con prueba</i>",
+    'fr': "🗣 Les messages <i>avec questionnaire</i> ne sont pas autorisés",
+    'zh': "🗣 不允許<i>帶有測驗</i>的消息",
+    'ar': "🗣 الرسائل <i> مع الاستطلاع </i> غير مسموح بها",
+}
+l_hand_msg_voice = {
+    'ru': "🗣 <i>Голосовые-сообщения не разрешены</i>",
+    'en': "🗣 <i>Voice-messages are not allowed</i>",
+    'es': "🗣 <i>No se permiten mensajes de voz</i>",
+    'fr': "🗣 <i>Les messages vocaux ne sont pas autorisés</i>",
+    'zh': "🗣 <i>不允許語音留言</i>",
+    'ar': "🗣 <i> الرسائل الصوتية غير مسموح بها </i>",
+}
+l_hand_msg_video_note = {
+    'ru': "🗣 Сообщения <i>с видео-заметками</i> не разрешены",
+    'en': "🗣 Messages <i>with video-note</i> are not allowed",
+    'es': "🗣 No se permiten mensajes <i>con video-nota</i>",
+    'fr': "🗣 Les messages <i>avec note vidéo</i> ne sont pas autorisés",
+    'zh': "🗣 不允許<i>帶有視頻註釋</i>的消息",
+    'ar': "🗣 الرسائل <i> مع ملاحظة الفيديو </i> غير مسموح بها",
+}
+# endregion
+
+# endregion
+
```

### Comparing `yeref-0.1.49/yeref/yeref.py` & `yeref-0.1.50/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -1943,14 +1943,47 @@
     finally:
         return result
 
 # endregion
 
 
 # region functions
+async def auto_destroy_msg(bot, telegram_bot, chat_id, text, message_id, type_='text', sec=5):
+    result = None
+    try:
+        step = 1
+        by = f"<a href='https://t.me/{ferey_telegram_demo_bot}'>by</a>"
+        text = f"{text}\n\n{by} @{telegram_bot} <b>{sec}</b>sec"
+        ix_sec = text.rfind('</b>sec')
+        while text[ix_sec] != '>': ix_sec -= 1
+
+        while sec > 0:
+            try:
+                text = text.replace(f"<b>{sec}</b>sec", f"<b>{sec - 1}</b>sec")
+                sec -= step
+                if type_ == 'text':
+                    await bot.edit_message_text(text, chat_id, message_id, disable_web_page_preview=True)
+                else:
+                    await bot.edit_message_caption(chat_id=chat_id, message_id=message_id, caption=text)
+                await asyncio.sleep(1)
+            except Exception as e:
+                logger.info(log_ % str(e))
+                await asyncio.sleep(round(random.uniform(1, 2), 2))
+                break
+        await bot.delete_message(chat_id, message_id)
+    except TelegramRetryAfter as e:
+        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
+        await asyncio.sleep(e.retry_after + 1)
+    except Exception as e:
+        logger.info(e)
+        await asyncio.sleep(round(random.uniform(1, 2), 2))
+    finally:
+        return result
+
+
 async def log_old(txt, LOG_DEFAULT, colour=92):
     try:
         logging.info(f'\033[{colour}m%s\033[0m' % (str(txt)))
         with open(LOG_DEFAULT, 'a') as f:
             f.write(str(txt) + '\n')
     except Exception as e:
         logger.info(f'\033[{95}m%s\033[0m' % str(e))
```

