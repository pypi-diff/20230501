# Comparing `tmp/django-admin-modernize-1.0.2.tar.gz` & `tmp/django-admin-modernize-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-modernize-1.0.2.tar", last modified: Mon May  1 07:51:44 2023, max compression
+gzip compressed data, was "django-admin-modernize-1.0.3.tar", last modified: Mon May  1 07:58:52 2023, max compression
```

## Comparing `django-admin-modernize-1.0.2.tar` & `django-admin-modernize-1.0.3.tar`

### file list

```diff
@@ -1,833 +1,833 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.798108 django-admin-modernize-1.0.2/
--rw-rw-rw-   0        0        0     1113 2022-09-27 05:30:21.000000 django-admin-modernize-1.0.2/LICENSE.md
--rw-rw-rw-   0        0        0      152 2023-04-29 10:04:52.000000 django-admin-modernize-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6248 2023-05-01 07:51:44.796105 django-admin-modernize-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5168 2023-05-01 07:49:16.000000 django-admin-modernize-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:42.343218 django-admin-modernize-1.0.2/admin_modernize/
--rw-rw-rw-   0        0        0       78 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/__init__.py
--rw-rw-rw-   0        0        0       34 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/admin.py
--rw-rw-rw-   0        0        0      268 2023-04-29 10:06:11.000000 django-admin-modernize-1.0.2/admin_modernize/apps.py
--rw-rw-rw-   0        0        0     2907 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/forms.py
--rw-rw-rw-   0        0        0       60 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/models.py
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:42.345229 django-admin-modernize-1.0.2/admin_modernize/static/
--rw-rw-rw-   0        0        0        0 2022-09-27 05:30:21.000000 django-admin-modernize-1.0.2/admin_modernize/static/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:42.280594 django-admin-modernize-1.0.2/admin_modernize/static/assets/
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:42.362304 django-admin-modernize-1.0.2/admin_modernize/static/assets/css/
--rw-rw-rw-   0        0        0     9582 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/css/forms.css
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:42.213047 django-admin-modernize-1.0.2/admin_modernize/static/assets/css/icons/
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:42.365317 django-admin-modernize-1.0.2/admin_modernize/static/assets/css/icons/tabler-icons/
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:42.391879 django-admin-modernize-1.0.2/admin_modernize/static/assets/css/icons/tabler-icons/fonts/
--rw-rw-rw-   0        0        0  1521944 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/css/icons/tabler-icons/fonts/tabler-icons.eot
--rw-rw-rw-   0        0        0  6046707 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/css/icons/tabler-icons/fonts/tabler-icons.svg
--rw-rw-rw-   0        0        0  1521760 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/css/icons/tabler-icons/fonts/tabler-icons.ttf
--rw-rw-rw-   0        0        0   775616 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/css/icons/tabler-icons/fonts/tabler-icons.woff
--rw-rw-rw-   0        0        0   552144 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/css/icons/tabler-icons/fonts/tabler-icons.woff2
--rw-rw-rw-   0        0        0   146896 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/css/icons/tabler-icons/tabler-icons.css
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:42.395898 django-admin-modernize-1.0.2/admin_modernize/static/assets/css/plugins/
--rw-rw-rw-   0        0        0    58139 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/css/plugins/animate.min.css
--rw-rw-rw-   0        0        0   193535 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/css/plugins/bootstrap.min.css
--rw-rw-rw-   0        0        0   200840 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/css/style-preset.css
--rw-rw-rw-   0        0        0   339626 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/css/styles.css
--rw-rw-rw-   0        0        0   335915 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/css/styles.min.css
--rw-rw-rw-   0        0        0    12535 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/css/widgets.css
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:42.218028 django-admin-modernize-1.0.2/admin_modernize/static/assets/images/
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:42.396899 django-admin-modernize-1.0.2/admin_modernize/static/assets/images/backgrounds/
--rw-rw-rw-   0        0        0    15492 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/images/backgrounds/rocket.png
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:42.401404 django-admin-modernize-1.0.2/admin_modernize/static/assets/images/logos/
--rw-rw-rw-   0        0        0     6618 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/images/logos/dark-logo.svg
--rw-rw-rw-   0        0        0      583 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/images/logos/favicon.png
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:42.409417 django-admin-modernize-1.0.2/admin_modernize/static/assets/images/products/
--rw-rw-rw-   0        0        0   117358 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/images/products/s1.jpg
--rw-rw-rw-   0        0        0   231624 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/images/products/s11.jpg
--rw-rw-rw-   0        0        0    84198 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/images/products/s4.jpg
--rw-rw-rw-   0        0        0   124284 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/images/products/s5.jpg
--rw-rw-rw-   0        0        0    78225 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/images/products/s7.jpg
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:42.411414 django-admin-modernize-1.0.2/admin_modernize/static/assets/images/profile/
--rw-rw-rw-   0        0        0    30954 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/images/profile/user-1.jpg
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:42.415899 django-admin-modernize-1.0.2/admin_modernize/static/assets/js/
--rw-rw-rw-   0        0        0     1263 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/js/app.min.js
--rw-rw-rw-   0        0        0     3840 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/js/dashboard.js
--rw-rw-rw-   0        0        0     1846 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/js/sidebarmenu.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:42.279592 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:42.419900 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/
--rw-rw-rw-   0        0        0     1076 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/LICENSE
--rw-rw-rw-   0        0        0    14275 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:42.437474 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/
--rw-rw-rw-   0        0        0   549363 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.amd.js
--rw-rw-rw-   0        0        0   502932 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.common.js
--rw-rw-rw-   0        0        0    12763 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.css
--rw-rw-rw-   0        0        0   502923 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.esm.js
--rw-rw-rw-   0        0        0  1147184 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.js
--rw-rw-rw-   0        0        0   503168 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.min.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.416891 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/
--rw-rw-rw-   0        0        0     1004 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/ar.json
--rw-rw-rw-   0        0        0     1013 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/ca.json
--rw-rw-rw-   0        0        0     1011 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/cs.json
--rw-rw-rw-   0        0        0     1006 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/de.json
--rw-rw-rw-   0        0        0     1324 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/el.json
--rw-rw-rw-   0        0        0      983 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/en.json
--rw-rw-rw-   0        0        0     1001 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/es.json
--rw-rw-rw-   0        0        0     1055 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/et.json
--rw-rw-rw-   0        0        0     1170 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/fa.json
--rw-rw-rw-   0        0        0     1030 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/fi.json
--rw-rw-rw-   0        0        0     1071 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/fr.json
--rw-rw-rw-   0        0        0     1129 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/he.json
--rw-rw-rw-   0        0        0     1508 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/hi.json
--rw-rw-rw-   0        0        0     1035 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/hr.json
--rw-rw-rw-   0        0        0     1164 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/hu.json
--rw-rw-rw-   0        0        0     1323 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/hy.json
--rw-rw-rw-   0        0        0      917 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/id.json
--rw-rw-rw-   0        0        0      996 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/it.json
--rw-rw-rw-   0        0        0     1028 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/ja.json
--rw-rw-rw-   0        0        0     1618 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/ka.json
--rw-rw-rw-   0        0        0     1002 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/ko.json
--rw-rw-rw-   0        0        0     1064 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/lt.json
--rw-rw-rw-   0        0        0     1122 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/lv.json
--rw-rw-rw-   0        0        0      968 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/nb.json
--rw-rw-rw-   0        0        0      988 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/nl.json
--rw-rw-rw-   0        0        0     1012 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/pl.json
--rw-rw-rw-   0        0        0      989 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/pt-br.json
--rw-rw-rw-   0        0        0     1017 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/pt.json
--rw-rw-rw-   0        0        0      998 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/rs.json
--rw-rw-rw-   0        0        0     1268 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/ru.json
--rw-rw-rw-   0        0        0      986 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/se.json
--rw-rw-rw-   0        0        0     1006 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/sk.json
--rw-rw-rw-   0        0        0      982 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/sl.json
--rw-rw-rw-   0        0        0      999 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/sq.json
--rw-rw-rw-   0        0        0     1484 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/th.json
--rw-rw-rw-   0        0        0     1011 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/tr.json
--rw-rw-rw-   0        0        0     1277 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/ua.json
--rw-rw-rw-   0        0        0     1055 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/zh-cn.json
--rw-rw-rw-   0        0        0     1055 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/zh-tw.json
--rw-rw-rw-   0        0        0     3089 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/package.json
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.421497 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/
--rw-rw-rw-   0        0        0    22769 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/apexcharts.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.453433 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/assets/
--rw-rw-rw-   0        0        0    13601 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/assets/apexcharts.css
--rw-rw-rw-   0        0        0      355 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-camera.svg
--rw-rw-rw-   0        0        0      199 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-home.svg
--rw-rw-rw-   0        0        0      185 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-menu.svg
--rw-rw-rw-   0        0        0      416 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-minus-square.svg
--rw-rw-rw-   0        0        0      289 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-minus.svg
--rw-rw-rw-   0        0        0      656 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-pan-hand.svg
--rw-rw-rw-   0        0        0      269 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-pan.svg
--rw-rw-rw-   0        0        0      263 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-plus-square.svg
--rw-rw-rw-   0        0        0      308 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-plus.svg
--rw-rw-rw-   0        0        0      366 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-refresh.svg
--rw-rw-rw-   0        0        0      265 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-reset.svg
--rw-rw-rw-   0        0        0      439 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-select.svg
--rw-rw-rw-   0        0        0      231 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-select1.svg
--rw-rw-rw-   0        0        0      450 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-zoom-in.svg
--rw-rw-rw-   0        0        0      600 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-zoom-out.svg
--rw-rw-rw-   0        0        0      301 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-zoom.svg
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.472096 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/
--rw-rw-rw-   0        0        0    12112 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/Bar.js
--rw-rw-rw-   0        0        0    13155 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/BarStacked.js
--rw-rw-rw-   0        0        0    12007 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/BoxCandleStick.js
--rw-rw-rw-   0        0        0     6370 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/HeatMap.js
--rw-rw-rw-   0        0        0    19401 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/Line.js
--rw-rw-rw-   0        0        0    28958 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/Pie.js
--rw-rw-rw-   0        0        0    13446 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/Radar.js
--rw-rw-rw-   0        0        0    12331 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/Radial.js
--rw-rw-rw-   0        0        0    11291 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/RangeBar.js
--rw-rw-rw-   0        0        0     7196 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/Scatter.js
--rw-rw-rw-   0        0        0     7802 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/Treemap.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:42.228551 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/common/
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.475106 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/common/bar/
--rw-rw-rw-   0        0        0    11250 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/common/bar/DataLabels.js
--rw-rw-rw-   0        0        0    16884 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/common/bar/Helpers.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.477119 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/common/circle/
--rw-rw-rw-   0        0        0      832 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/common/circle/Helpers.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.478107 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/common/line/
--rw-rw-rw-   0        0        0     4369 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/common/line/Helpers.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.481618 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/common/treemap/
--rw-rw-rw-   0        0        0     5077 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/common/treemap/Helpers.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.486643 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/libs/
--rw-rw-rw-   0        0        0     9417 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/libs/Treemap-squared.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.560469 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/
--rw-rw-rw-   0        0        0     1004 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/ar.json
--rw-rw-rw-   0        0        0     1013 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/ca.json
--rw-rw-rw-   0        0        0     1011 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/cs.json
--rw-rw-rw-   0        0        0     1006 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/de.json
--rw-rw-rw-   0        0        0     1324 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/el.json
--rw-rw-rw-   0        0        0      983 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/en.json
--rw-rw-rw-   0        0        0     1001 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/es.json
--rw-rw-rw-   0        0        0     1055 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/et.json
--rw-rw-rw-   0        0        0     1170 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/fa.json
--rw-rw-rw-   0        0        0     1030 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/fi.json
--rw-rw-rw-   0        0        0     1071 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/fr.json
--rw-rw-rw-   0        0        0     1129 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/he.json
--rw-rw-rw-   0        0        0     1508 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/hi.json
--rw-rw-rw-   0        0        0     1035 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/hr.json
--rw-rw-rw-   0        0        0     1164 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/hu.json
--rw-rw-rw-   0        0        0     1323 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/hy.json
--rw-rw-rw-   0        0        0      917 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/id.json
--rw-rw-rw-   0        0        0      996 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/it.json
--rw-rw-rw-   0        0        0     1028 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/ja.json
--rw-rw-rw-   0        0        0     1618 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/ka.json
--rw-rw-rw-   0        0        0     1002 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/ko.json
--rw-rw-rw-   0        0        0     1064 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/lt.json
--rw-rw-rw-   0        0        0     1122 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/lv.json
--rw-rw-rw-   0        0        0      968 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/nb.json
--rw-rw-rw-   0        0        0      988 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/nl.json
--rw-rw-rw-   0        0        0     1012 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/pl.json
--rw-rw-rw-   0        0        0      989 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/pt-br.json
--rw-rw-rw-   0        0        0     1017 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/pt.json
--rw-rw-rw-   0        0        0      998 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/rs.json
--rw-rw-rw-   0        0        0     1268 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/ru.json
--rw-rw-rw-   0        0        0      986 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/se.json
--rw-rw-rw-   0        0        0     1006 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/sk.json
--rw-rw-rw-   0        0        0      982 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/sl.json
--rw-rw-rw-   0        0        0      999 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/sq.json
--rw-rw-rw-   0        0        0     1484 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/th.json
--rw-rw-rw-   0        0        0     1011 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/tr.json
--rw-rw-rw-   0        0        0     1277 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/ua.json
--rw-rw-rw-   0        0        0     1055 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/zh-cn.json
--rw-rw-rw-   0        0        0     1055 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/zh-tw.json
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.597248 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/
--rw-rw-rw-   0        0        0     5782 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Animations.js
--rw-rw-rw-   0        0        0      479 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Base.js
--rw-rw-rw-   0        0        0    17431 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Core.js
--rw-rw-rw-   0        0        0     9891 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/CoreUtils.js
--rw-rw-rw-   0        0        0     3692 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Crosshairs.js
--rw-rw-rw-   0        0        0    20941 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Data.js
--rw-rw-rw-   0        0        0     9971 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/DataLabels.js
--rw-rw-rw-   0        0        0     3048 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Events.js
--rw-rw-rw-   0        0        0    10938 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Exports.js
--rw-rw-rw-   0        0        0    10063 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Fill.js
--rw-rw-rw-   0        0        0     5604 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Filters.js
--rw-rw-rw-   0        0        0     4960 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Formatters.js
--rw-rw-rw-   0        0        0    21067 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Graphics.js
--rw-rw-rw-   0        0        0     7059 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Markers.js
--rw-rw-rw-   0        0        0    16559 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Range.js
--rw-rw-rw-   0        0        0     2083 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Responsive.js
--rw-rw-rw-   0        0        0    16955 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Scales.js
--rw-rw-rw-   0        0        0    12234 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Series.js
--rw-rw-rw-   0        0        0     7170 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Theme.js
--rw-rw-rw-   0        0        0    24177 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/TimeScale.js
--rw-rw-rw-   0        0        0     1262 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/TitleSubtitle.js
--rw-rw-rw-   0        0        0    14827 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Toolbar.js
--rw-rw-rw-   0        0        0    22002 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/ZoomPanSelection.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.605767 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/annotations/
--rw-rw-rw-   0        0        0     8325 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/annotations/Annotations.js
--rw-rw-rw-   0        0        0     6530 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/annotations/Helpers.js
--rw-rw-rw-   0        0        0     3146 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/annotations/PointsAnnotations.js
--rw-rw-rw-   0        0        0     3145 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/annotations/XAxisAnnotations.js
--rw-rw-rw-   0        0        0     2926 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/annotations/YAxisAnnotations.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.613399 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/axes/
--rw-rw-rw-   0        0        0      904 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/axes/Axes.js
--rw-rw-rw-   0        0        0     6093 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/axes/AxesUtils.js
--rw-rw-rw-   0        0        0    13749 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/axes/Grid.js
--rw-rw-rw-   0        0        0    19087 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/axes/XAxis.js
--rw-rw-rw-   0        0        0    16055 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/axes/YAxis.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.621367 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/dimensions/
--rw-rw-rw-   0        0        0     9510 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/dimensions/Dimensions.js
--rw-rw-rw-   0        0        0     3681 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/dimensions/Grid.js
--rw-rw-rw-   0        0        0     2388 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/dimensions/Helpers.js
--rw-rw-rw-   0        0        0    10704 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/dimensions/XAxis.js
--rw-rw-rw-   0        0        0     5444 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/dimensions/YAxis.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.628409 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/helpers/
--rw-rw-rw-   0        0        0     2310 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/helpers/Destroy.js
--rw-rw-rw-   0        0        0     3122 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/helpers/InitCtxVariables.js
--rw-rw-rw-   0        0        0     1245 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/helpers/Localization.js
--rw-rw-rw-   0        0        0     9031 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/helpers/UpdateHelpers.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.631914 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/legend/
--rw-rw-rw-   0        0        0     9280 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/legend/Helpers.js
--rw-rw-rw-   0        0        0    14694 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/legend/Legend.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.639968 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/settings/
--rw-rw-rw-   0        0        0     9734 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/settings/Config.js
--rw-rw-rw-   0        0        0    16712 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/settings/Defaults.js
--rw-rw-rw-   0        0        0     8637 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/settings/Globals.js
--rw-rw-rw-   0        0        0    27224 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/settings/Options.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.660638 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/
--rw-rw-rw-   0        0        0     5936 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/AxesTooltip.js
--rw-rw-rw-   0        0        0     9729 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Intersect.js
--rw-rw-rw-   0        0        0    14229 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Labels.js
--rw-rw-rw-   0        0        0     5119 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Marker.js
--rw-rw-rw-   0        0        0    12341 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Position.js
--rw-rw-rw-   0        0        0      723 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/README.md
--rw-rw-rw-   0        0        0    25334 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Tooltip.js
--rw-rw-rw-   0        0        0     9947 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Utils.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.662157 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/svgjs/
--rw-rw-rw-   0        0        0   103950 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/svgjs/svg.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.668183 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/utils/
--rw-rw-rw-   0        0        0     6856 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/utils/DateTime.js
--rw-rw-rw-   0        0        0     1538 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/utils/Resize.js
--rw-rw-rw-   0        0        0    10168 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/utils/Utils.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.670166 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/types/
--rw-rw-rw-   0        0        0    26539 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/types/apexcharts.d.ts
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.675690 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/
--rw-rw-rw-   0        0        0     1131 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/LICENSE
--rw-rw-rw-   0        0        0    13743 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:42.242182 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.740137 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/
--rw-rw-rw-   0        0        0    75616 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.css
--rw-rw-rw-   0        0        0   226018 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.css.map
--rw-rw-rw-   0        0        0    56464 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.min.css
--rw-rw-rw-   0        0        0   142342 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.min.css.map
--rw-rw-rw-   0        0        0    75690 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.rtl.css
--rw-rw-rw-   0        0        0   226022 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.rtl.css.map
--rw-rw-rw-   0        0        0    56539 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.rtl.min.css
--rw-rw-rw-   0        0        0   142419 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map
--rw-rw-rw-   0        0        0    11735 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.css
--rw-rw-rw-   0        0        0   126626 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.css.map
--rw-rw-rw-   0        0        0     9817 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.min.css
--rw-rw-rw-   0        0        0    51406 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.min.css.map
--rw-rw-rw-   0        0        0    11728 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.rtl.css
--rw-rw-rw-   0        0        0   126641 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.rtl.css.map
--rw-rw-rw-   0        0        0     9889 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.rtl.min.css
--rw-rw-rw-   0        0        0    63643 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map
--rw-rw-rw-   0        0        0    96254 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.css
--rw-rw-rw-   0        0        0   250681 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.css.map
--rw-rw-rw-   0        0        0    74887 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.min.css
--rw-rw-rw-   0        0        0   163881 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.min.css.map
--rw-rw-rw-   0        0        0    96121 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.rtl.css
--rw-rw-rw-   0        0        0   250622 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.rtl.css.map
--rw-rw-rw-   0        0        0    74815 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.rtl.min.css
--rw-rw-rw-   0        0        0   163716 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map
--rw-rw-rw-   0        0        0   267476 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.css
--rw-rw-rw-   0        0        0   658460 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.css.map
--rw-rw-rw-   0        0        0   220780 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.min.css
--rw-rw-rw-   0        0        0   568408 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.min.css.map
--rw-rw-rw-   0        0        0   267055 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.rtl.css
--rw-rw-rw-   0        0        0   658305 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.rtl.css.map
--rw-rw-rw-   0        0        0   220887 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.rtl.min.css
--rw-rw-rw-   0        0        0   567947 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.rtl.min.css.map
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.765689 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/
--rw-rw-rw-   0        0        0   208288 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.bundle.js
--rw-rw-rw-   0        0        0   448884 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.bundle.js.map
--rw-rw-rw-   0        0        0    80599 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   333974 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.bundle.min.js.map
--rw-rw-rw-   0        0        0   136243 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.esm.js
--rw-rw-rw-   0        0        0   305274 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.esm.js.map
--rw-rw-rw-   0        0        0    74135 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.esm.min.js
--rw-rw-rw-   0        0        0   222070 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.esm.min.js.map
--rw-rw-rw-   0        0        0   145819 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.js
--rw-rw-rw-   0        0        0   306458 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.js.map
--rw-rw-rw-   0        0        0    60554 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.min.js
--rw-rw-rw-   0        0        0   217885 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.min.js.map
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.769709 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.828554 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/
--rw-rw-rw-   0        0        0     3140 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/alert.js
--rw-rw-rw-   0        0        0     4294 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/alert.js.map
--rw-rw-rw-   0        0        0     3224 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/base-component.js
--rw-rw-rw-   0        0        0     4602 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/base-component.js.map
--rw-rw-rw-   0        0        0     2756 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/button.js
--rw-rw-rw-   0        0        0     3466 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/button.js.map
--rw-rw-rw-   0        0        0    14281 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/carousel.js
--rw-rw-rw-   0        0        0    27442 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/carousel.js.map
--rw-rw-rw-   0        0        0     9455 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/collapse.js
--rw-rw-rw-   0        0        0    18212 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/collapse.js.map
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.946572 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/
--rw-rw-rw-   0        0        0     2119 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/data.js
--rw-rw-rw-   0        0        0     3047 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/data.js.map
--rw-rw-rw-   0        0        0     9578 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/event-handler.js
--rw-rw-rw-   0        0        0    19800 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/event-handler.js.map
--rw-rw-rw-   0        0        0     2438 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/manipulator.js
--rw-rw-rw-   0        0        0     4319 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/manipulator.js.map
--rw-rw-rw-   0        0        0     2700 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/selector-engine.js
--rw-rw-rw-   0        0        0     4619 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/selector-engine.js.map
--rw-rw-rw-   0        0        0    16199 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/dropdown.js
--rw-rw-rw-   0        0        0    29448 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/dropdown.js.map
--rw-rw-rw-   0        0        0    12194 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/modal.js
--rw-rw-rw-   0        0        0    22634 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/modal.js.map
--rw-rw-rw-   0        0        0     9166 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/offcanvas.js
--rw-rw-rw-   0        0        0    16142 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/offcanvas.js.map
--rw-rw-rw-   0        0        0     2883 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/popover.js
--rw-rw-rw-   0        0        0     4053 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/popover.js.map
--rw-rw-rw-   0        0        0    10303 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/scrollspy.js
--rw-rw-rw-   0        0        0    18973 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/scrollspy.js.map
--rw-rw-rw-   0        0        0    10647 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/tab.js
--rw-rw-rw-   0        0        0    19947 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/tab.js.map
--rw-rw-rw-   0        0        0     6632 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/toast.js
--rw-rw-rw-   0        0        0    12018 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/toast.js.map
--rw-rw-rw-   0        0        0    19225 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/tooltip.js
--rw-rw-rw-   0        0        0    37599 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/tooltip.js.map
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:43.981195 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/
--rw-rw-rw-   0        0        0     4413 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/backdrop.js
--rw-rw-rw-   0        0        0     7172 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/backdrop.js.map
--rw-rw-rw-   0        0        0     2174 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/component-functions.js
--rw-rw-rw-   0        0        0     2310 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/component-functions.js.map
--rw-rw-rw-   0        0        0     2808 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/config.js
--rw-rw-rw-   0        0        0     4073 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/config.js.map
--rw-rw-rw-   0        0        0     3913 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/focustrap.js
--rw-rw-rw-   0        0        0     5891 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/focustrap.js.map
--rw-rw-rw-   0        0        0    10248 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/index.js
--rw-rw-rw-   0        0        0    18675 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/index.js.map
--rw-rw-rw-   0        0        0     4253 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/sanitizer.js
--rw-rw-rw-   0        0        0     7572 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/sanitizer.js.map
--rw-rw-rw-   0        0        0     5031 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/scrollbar.js
--rw-rw-rw-   0        0        0     8041 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/scrollbar.js.map
--rw-rw-rw-   0        0        0     4733 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/swipe.js
--rw-rw-rw-   0        0        0     8335 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/swipe.js.map
--rw-rw-rw-   0        0        0     4980 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/template-factory.js
--rw-rw-rw-   0        0        0     8655 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/template-factory.js.map
--rw-rw-rw-   0        0        0      881 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/index.esm.js
--rw-rw-rw-   0        0        0      848 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/index.umd.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.009798 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/
--rw-rw-rw-   0        0        0     1901 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/alert.js
--rw-rw-rw-   0        0        0     1930 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/base-component.js
--rw-rw-rw-   0        0        0     1626 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/button.js
--rw-rw-rw-   0        0        0    11820 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/carousel.js
--rw-rw-rw-   0        0        0     7669 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/collapse.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.017355 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/dom/
--rw-rw-rw-   0        0        0     1405 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/dom/data.js
--rw-rw-rw-   0        0        0     8450 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/dom/event-handler.js
--rw-rw-rw-   0        0        0     1668 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/dom/manipulator.js
--rw-rw-rw-   0        0        0     1968 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/dom/selector-engine.js
--rw-rw-rw-   0        0        0    13257 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/dropdown.js
--rw-rw-rw-   0        0        0     9629 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/modal.js
--rw-rw-rw-   0        0        0     6804 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/offcanvas.js
--rw-rw-rw-   0        0        0     1874 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/popover.js
--rw-rw-rw-   0        0        0     8448 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/scrollspy.js
--rw-rw-rw-   0        0        0     8756 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/tab.js
--rw-rw-rw-   0        0        0     5037 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/toast.js
--rw-rw-rw-   0        0        0    16188 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/tooltip.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.048339 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/util/
--rw-rw-rw-   0        0        0     3126 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/util/backdrop.js
--rw-rw-rw-   0        0        0     1072 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/util/component-functions.js
--rw-rw-rw-   0        0        0     1818 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/util/config.js
--rw-rw-rw-   0        0        0     2519 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/util/focustrap.js
--rw-rw-rw-   0        0        0     8436 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/util/index.js
--rw-rw-rw-   0        0        0     3253 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/util/sanitizer.js
--rw-rw-rw-   0        0        0     3755 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/util/scrollbar.js
--rw-rw-rw-   0        0        0     3410 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/util/swipe.js
--rw-rw-rw-   0        0        0     3630 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/util/template-factory.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.069483 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/
--rw-rw-rw-   0        0        0     3131 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/README.md
--rw-rw-rw-   0        0        0     1511 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/browsers.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.071453 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/helpers/
--rw-rw-rw-   0        0        0     1156 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/helpers/fixture.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.078762 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/integration/
--rw-rw-rw-   0        0        0      236 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/integration/bundle-modularity.js
--rw-rw-rw-   0        0        0      226 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/integration/bundle.js
--rw-rw-rw-   0        0        0     4274 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/integration/index.html
--rw-rw-rw-   0        0        0      358 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/integration/rollup.bundle-modularity.js
--rw-rw-rw-   0        0        0      539 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/integration/rollup.bundle.js
--rw-rw-rw-   0        0        0     4106 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/karma.conf.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.107309 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/
--rw-rw-rw-   0        0        0      247 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/.eslintrc.json
--rw-rw-rw-   0        0        0     7571 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/alert.spec.js
--rw-rw-rw-   0        0        0     4928 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/base-component.spec.js
--rw-rw-rw-   0        0        0     5424 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/button.spec.js
--rw-rw-rw-   0        0        0    52616 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/carousel.spec.js
--rw-rw-rw-   0        0        0    38351 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/collapse.spec.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.114326 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/dom/
--rw-rw-rw-   0        0        0     2621 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/dom/data.spec.js
--rw-rw-rw-   0        0        0    13110 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/dom/event-handler.spec.js
--rw-rw-rw-   0        0        0     4616 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/dom/manipulator.spec.js
--rw-rw-rw-   0        0        0     6892 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/dom/selector-engine.spec.js
--rw-rw-rw-   0        0        0    85853 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/dropdown.spec.js
--rw-rw-rw-   0        0        0     1988 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/jquery.spec.js
--rw-rw-rw-   0        0        0    40009 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/modal.spec.js
--rw-rw-rw-   0        0        0    29788 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/offcanvas.spec.js
--rw-rw-rw-   0        0        0    13775 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/popover.spec.js
--rw-rw-rw-   0        0        0    32996 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/scrollspy.spec.js
--rw-rw-rw-   0        0        0    42678 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/tab.spec.js
--rw-rw-rw-   0        0        0    19308 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/toast.spec.js
--rw-rw-rw-   0        0        0    49199 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/tooltip.spec.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.131462 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/
--rw-rw-rw-   0        0        0     9342 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/backdrop.spec.js
--rw-rw-rw-   0        0        0     3422 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/component-functions.spec.js
--rw-rw-rw-   0        0        0     5498 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/config.spec.js
--rw-rw-rw-   0        0        0     6901 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/focustrap.spec.js
--rw-rw-rw-   0        0        0    25378 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/index.spec.js
--rw-rw-rw-   0        0        0     3234 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/sanitizer.spec.js
--rw-rw-rw-   0        0        0    13963 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/scrollbar.spec.js
--rw-rw-rw-   0        0        0     8107 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/swipe.spec.js
--rw-rw-rw-   0        0        0     8929 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/template-factory.spec.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.153626 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/
--rw-rw-rw-   0        0        0      301 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/.eslintrc.json
--rw-rw-rw-   0        0        0     2189 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/alert.html
--rw-rw-rw-   0        0        0     2898 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/button.html
--rw-rw-rw-   0        0        0     2867 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/carousel.html
--rw-rw-rw-   0        0        0     5326 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/collapse.html
--rw-rw-rw-   0        0        0     9958 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/dropdown.html
--rw-rw-rw-   0        0        0    15667 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/modal.html
--rw-rw-rw-   0        0        0     1853 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/popover.html
--rw-rw-rw-   0        0        0    18801 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/scrollspy.html
--rw-rw-rw-   0        0        0    32225 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/tab.html
--rw-rw-rw-   0        0        0     2580 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/toast.html
--rw-rw-rw-   0        0        0     6309 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/tooltip.html
--rw-rw-rw-   0        0        0     9286 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/package.json
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.258992 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/
--rw-rw-rw-   0        0        0     5066 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_accordion.scss
--rw-rw-rw-   0        0        0     2055 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_alert.scss
--rw-rw-rw-   0        0        0     1118 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_badge.scss
--rw-rw-rw-   0        0        0     1751 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_breadcrumb.scss
--rw-rw-rw-   0        0        0     3195 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_button-group.scss
--rw-rw-rw-   0        0        0     6685 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_buttons.scss
--rw-rw-rw-   0        0        0     6941 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_card.scss
--rw-rw-rw-   0        0        0     5751 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_carousel.scss
--rw-rw-rw-   0        0        0     1948 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_close.scss
--rw-rw-rw-   0        0        0     1201 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_containers.scss
--rw-rw-rw-   0        0        0     8093 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_dropdown.scss
--rw-rw-rw-   0        0        0      256 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_forms.scss
--rw-rw-rw-   0        0        0    10554 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_functions.scss
--rw-rw-rw-   0        0        0      575 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_grid.scss
--rw-rw-rw-   0        0        0      294 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_helpers.scss
--rw-rw-rw-   0        0        0     1158 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_images.scss
--rw-rw-rw-   0        0        0     6775 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_list-group.scss
--rw-rw-rw-   0        0        0     4043 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_maps.scss
--rw-rw-rw-   0        0        0      875 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_mixins.scss
--rw-rw-rw-   0        0        0     7762 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_modal.scss
--rw-rw-rw-   0        0        0     4665 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_nav.scss
--rw-rw-rw-   0        0        0     9104 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_navbar.scss
--rw-rw-rw-   0        0        0     4725 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_offcanvas.scss
--rw-rw-rw-   0        0        0     3944 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_pagination.scss
--rw-rw-rw-   0        0        0      859 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_placeholders.scss
--rw-rw-rw-   0        0        0     6907 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_popover.scss
--rw-rw-rw-   0        0        0     2016 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_progress.scss
--rw-rw-rw-   0        0        0    12404 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_reboot.scss
--rw-rw-rw-   0        0        0     7371 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_root.scss
--rw-rw-rw-   0        0        0     2429 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_spinners.scss
--rw-rw-rw-   0        0        0     4413 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_tables.scss
--rw-rw-rw-   0        0        0     2490 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_toasts.scss
--rw-rw-rw-   0        0        0     3939 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_tooltip.scss
--rw-rw-rw-   0        0        0      425 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_transitions.scss
--rw-rw-rw-   0        0        0     1420 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_type.scss
--rw-rw-rw-   0        0        0    17886 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_utilities.scss
--rw-rw-rw-   0        0        0     3840 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_variables-dark.scss
--rw-rw-rw-   0        0        0    73610 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_variables.scss
--rw-rw-rw-   0        0        0    75614 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-grid.css
--rw-rw-rw-   0        0        0    34422 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-grid.css.map
--rw-rw-rw-   0        0        0     1253 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-grid.scss
--rw-rw-rw-   0        0        0    11668 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-reboot.css
--rw-rw-rw-   0        0        0     4760 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-reboot.css.map
--rw-rw-rw-   0        0        0      189 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-reboot.scss
--rw-rw-rw-   0        0        0    96160 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-utilities.css
--rw-rw-rw-   0        0        0    43440 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-utilities.css.map
--rw-rw-rw-   0        0        0      306 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-utilities.scss
--rw-rw-rw-   0        0        0   266178 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap.css
--rw-rw-rw-   0        0        0   103943 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap.css.map
--rw-rw-rw-   0        0        0      938 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap.scss
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.276786 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/css/
--rw-rw-rw-   0        0        0    75568 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-grid.css
--rw-rw-rw-   0        0        0    34458 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-grid.css.map
--rw-rw-rw-   0        0        0    11620 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-reboot.css
--rw-rw-rw-   0        0        0     4781 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-reboot.css.map
--rw-rw-rw-   0        0        0    96109 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-utilities.css
--rw-rw-rw-   0        0        0    43500 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-utilities.css.map
--rw-rw-rw-   0        0        0   266137 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap.css
--rw-rw-rw-   0        0        0   104156 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap.css.map
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.296838 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/forms/
--rw-rw-rw-   0        0        0     2480 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/forms/_floating-labels.scss
--rw-rw-rw-   0        0        0     4833 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/forms/_form-check.scss
--rw-rw-rw-   0        0        0     5868 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/forms/_form-control.scss
--rw-rw-rw-   0        0        0     2796 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/forms/_form-range.scss
--rw-rw-rw-   0        0        0     2603 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/forms/_form-select.scss
--rw-rw-rw-   0        0        0      219 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/forms/_form-text.scss
--rw-rw-rw-   0        0        0     3896 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/forms/_input-group.scss
--rw-rw-rw-   0        0        0     1142 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/forms/_labels.scss
--rw-rw-rw-   0        0        0      478 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/forms/_validation.scss
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.318900 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/helpers/
--rw-rw-rw-   0        0        0       37 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/helpers/_clearfix.scss
--rw-rw-rw-   0        0        0      454 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/helpers/_color-bg.scss
--rw-rw-rw-   0        0        0      426 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/helpers/_colored-links.scss
--rw-rw-rw-   0        0        0      621 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/helpers/_position.scss
--rw-rw-rw-   0        0        0      399 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/helpers/_ratio.scss
--rw-rw-rw-   0        0        0      245 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/helpers/_stacks.scss
--rw-rw-rw-   0        0        0      223 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/helpers/_stretched-link.scss
--rw-rw-rw-   0        0        0       73 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/helpers/_text-truncation.scss
--rw-rw-rw-   0        0        0      136 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/helpers/_visually-hidden.scss
--rw-rw-rw-   0        0        0      147 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/helpers/_vr.scss
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.370644 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/
--rw-rw-rw-   0        0        0      525 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_alert.scss
--rw-rw-rw-   0        0        0      328 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_backdrop.scss
--rw-rw-rw-   0        0        0      230 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_banner.scss
--rw-rw-rw-   0        0        0     2031 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_border-radius.scss
--rw-rw-rw-   0        0        0      398 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_box-shadow.scss
--rw-rw-rw-   0        0        0     4580 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_breakpoints.scss
--rw-rw-rw-   0        0        0     3220 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_buttons.scss
--rw-rw-rw-   0        0        0     1587 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_caret.scss
--rw-rw-rw-   0        0        0      147 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_clearfix.scss
--rw-rw-rw-   0        0        0      447 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_color-mode.scss
--rw-rw-rw-   0        0        0      167 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_color-scheme.scss
--rw-rw-rw-   0        0        0      410 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_container.scss
--rw-rw-rw-   0        0        0      613 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_deprecate.scss
--rw-rw-rw-   0        0        0     4164 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_forms.scss
--rw-rw-rw-   0        0        0     1956 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_gradients.scss
--rw-rw-rw-   0        0        0     4726 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_grid.scss
--rw-rw-rw-   0        0        0      395 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_image.scss
--rw-rw-rw-   0        0        0      582 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_list-group.scss
--rw-rw-rw-   0        0        0      168 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_lists.scss
--rw-rw-rw-   0        0        0      387 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_pagination.scss
--rw-rw-rw-   0        0        0      495 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_reset-text.scss
--rw-rw-rw-   0        0        0      202 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_resize.scss
--rw-rw-rw-   0        0        0     1101 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_table-variants.scss
--rw-rw-rw-   0        0        0      168 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_text-truncate.scss
--rw-rw-rw-   0        0        0      661 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_transition.scss
--rw-rw-rw-   0        0        0     3380 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_utilities.scss
--rw-rw-rw-   0        0        0     1012 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_visually-hidden.scss
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.373164 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/utilities/
--rw-rw-rw-   0        0        0     1737 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/utilities/_api.scss
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.374165 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/vendor/
--rw-rw-rw-   0        0        0    10029 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/vendor/_rfs.scss
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.385699 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/
--rw-rw-rw-   0        0        0    11945 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/AUTHORS.txt
--rw-rw-rw-   0        0        0     1095 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/LICENSE.txt
--rw-rw-rw-   0        0        0     1997 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/README.md
--rw-rw-rw-   0        0        0      190 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/bower.json
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.406776 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/dist/
--rw-rw-rw-   0        0        0     9165 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/dist/core.js
--rw-rw-rw-   0        0        0   279869 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/dist/jquery.js
--rw-rw-rw-   0        0        0    88151 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/dist/jquery.min.js
--rw-rw-rw-   0        0        0   136403 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/dist/jquery.min.map
--rw-rw-rw-   0        0        0   226527 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/dist/jquery.slim.js
--rw-rw-rw-   0        0        0    71043 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/dist/jquery.slim.min.js
--rw-rw-rw-   0        0        0   108763 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/dist/jquery.slim.min.map
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:42.261524 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/external/
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.409770 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/external/sizzle/
--rw-rw-rw-   0        0        0     1605 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/external/sizzle/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.415289 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/external/sizzle/dist/
--rw-rw-rw-   0        0        0    65675 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/external/sizzle/dist/sizzle.js
--rw-rw-rw-   0        0        0    19841 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/external/sizzle/dist/sizzle.min.js
--rw-rw-rw-   0        0        0    30740 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/external/sizzle/dist/sizzle.min.map
--rw-rw-rw-   0        0        0     2870 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/package.json
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.454915 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/
--rw-rw-rw-   0        0        0       96 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/.eslintrc.json
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.462435 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/ajax/
--rw-rw-rw-   0        0        0     2748 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/ajax/jsonp.js
--rw-rw-rw-   0        0        0     1904 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/ajax/load.js
--rw-rw-rw-   0        0        0      559 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/ajax/parseXML.js
--rw-rw-rw-   0        0        0     1637 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/ajax/script.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.467436 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/ajax/var/
--rw-rw-rw-   0        0        0       67 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/ajax/var/location.js
--rw-rw-rw-   0        0        0       62 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/ajax/var/nonce.js
--rw-rw-rw-   0        0        0       60 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/ajax/var/rquery.js
--rw-rw-rw-   0        0        0     4339 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/ajax/xhr.js
--rw-rw-rw-   0        0        0    22463 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/ajax.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.475601 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/attributes/
--rw-rw-rw-   0        0        0     3271 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/attributes/attr.js
--rw-rw-rw-   0        0        0     4447 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/attributes/classes.js
--rw-rw-rw-   0        0        0     3004 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/attributes/prop.js
--rw-rw-rw-   0        0        0      786 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/attributes/support.js
--rw-rw-rw-   0        0        0     4249 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/attributes/val.js
--rw-rw-rw-   0        0        0      217 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/attributes.js
--rw-rw-rw-   0        0        0     5552 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/callbacks.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.499668 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/
--rw-rw-rw-   0        0        0     1160 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/DOMEval.js
--rw-rw-rw-   0        0        0     1311 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/access.js
--rw-rw-rw-   0        0        0      545 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/camelCase.js
--rw-rw-rw-   0        0        0     3337 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/init.js
--rw-rw-rw-   0        0        0      566 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/isAttached.js
--rw-rw-rw-   0        0        0      178 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/nodeName.js
--rw-rw-rw-   0        0        0     1604 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/parseHTML.js
--rw-rw-rw-   0        0        0     2264 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/ready-no-deferred.js
--rw-rw-rw-   0        0        0     2097 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/ready.js
--rw-rw-rw-   0        0        0      168 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/readyException.js
--rw-rw-rw-   0        0        0      362 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/stripAndCollapse.js
--rw-rw-rw-   0        0        0      631 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/support.js
--rw-rw-rw-   0        0        0      379 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/toType.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.503198 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/var/
--rw-rw-rw-   0        0        0      244 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/var/rsingleTag.js
--rw-rw-rw-   0        0        0     9165 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.521247 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css/
--rw-rw-rw-   0        0        0      530 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css/addGetHookIf.js
--rw-rw-rw-   0        0        0     2002 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css/adjustCSS.js
--rw-rw-rw-   0        0        0     1656 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css/curCSS.js
--rw-rw-rw-   0        0        0      849 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css/finalPropName.js
--rw-rw-rw-   0        0        0      317 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css/hiddenVisibleSelectors.js
--rw-rw-rw-   0        0        0     2304 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css/showHide.js
--rw-rw-rw-   0        0        0     3070 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css/support.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.532301 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css/var/
--rw-rw-rw-   0        0        0       88 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css/var/cssExpand.js
--rw-rw-rw-   0        0        0      401 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css/var/getStyles.js
--rw-rw-rw-   0        0        0     1284 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css/var/isHiddenWithinTree.js
--rw-rw-rw-   0        0        0      123 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css/var/rboxStyle.js
--rw-rw-rw-   0        0        0      131 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css/var/rnumnonpx.js
--rw-rw-rw-   0        0        0      520 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css/var/swap.js
--rw-rw-rw-   0        0        0    13828 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.534306 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/data/
--rw-rw-rw-   0        0        0     3952 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/data/Data.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.540308 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/data/var/
--rw-rw-rw-   0        0        0      318 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/data/var/acceptData.js
--rw-rw-rw-   0        0        0       84 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/data/var/dataPriv.js
--rw-rw-rw-   0        0        0       84 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/data/var/dataUser.js
--rw-rw-rw-   0        0        0     4321 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/data.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.542829 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/deferred/
--rw-rw-rw-   0        0        0      640 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/deferred/exceptionHook.js
--rw-rw-rw-   0        0        0    10997 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/deferred.js
--rw-rw-rw-   0        0        0     2467 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/deprecated.js
--rw-rw-rw-   0        0        0     1751 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/dimensions.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.545827 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/effects/
--rw-rw-rw-   0        0        0     3292 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/effects/Tween.js
--rw-rw-rw-   0        0        0      244 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/effects/animatedSelector.js
--rw-rw-rw-   0        0        0    17455 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/effects.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.553347 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/event/
--rw-rw-rw-   0        0        0      346 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/event/ajax.js
--rw-rw-rw-   0        0        0      649 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/event/alias.js
--rw-rw-rw-   0        0        0     1512 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/event/focusin.js
--rw-rw-rw-   0        0        0      133 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/event/support.js
--rw-rw-rw-   0        0        0     5407 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/event/trigger.js
--rw-rw-rw-   0        0        0    24235 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/event.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.556353 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/exports/
--rw-rw-rw-   0        0        0     1024 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/exports/amd.js
--rw-rw-rw-   0        0        0      608 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/exports/global.js
--rw-rw-rw-   0        0        0      622 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/jquery.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.565870 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/manipulation/
--rw-rw-rw-   0        0        0      676 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/manipulation/_evalUrl.js
--rw-rw-rw-   0        0        0     2486 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/manipulation/buildFragment.js
--rw-rw-rw-   0        0        0      650 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/manipulation/getAll.js
--rw-rw-rw-   0        0        0      381 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/manipulation/setGlobalEval.js
--rw-rw-rw-   0        0        0     1034 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/manipulation/support.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.568871 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/manipulation/var/
--rw-rw-rw-   0        0        0       92 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/manipulation/var/rscriptType.js
--rw-rw-rw-   0        0        0      304 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/manipulation/var/rtagName.js
--rw-rw-rw-   0        0        0      798 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/manipulation/wrapMap.js
--rw-rw-rw-   0        0        0    12643 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/manipulation.js
--rw-rw-rw-   0        0        0     6868 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/offset.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.569872 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/queue/
--rw-rw-rw-   0        0        0      636 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/queue/delay.js
--rw-rw-rw-   0        0        0     3091 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/queue.js
--rw-rw-rw-   0        0        0     6394 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/selector-native.js
--rw-rw-rw-   0        0        0      411 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/selector-sizzle.js
--rw-rw-rw-   0        0        0       66 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/selector.js
--rw-rw-rw-   0        0        0     3241 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/serialize.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.572389 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/traversing/
--rw-rw-rw-   0        0        0     2352 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/traversing/findFilter.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.577397 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/traversing/var/
--rw-rw-rw-   0        0        0      371 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/traversing/var/dir.js
--rw-rw-rw-   0        0        0      128 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/traversing/var/rneedsContext.js
--rw-rw-rw-   0        0        0      218 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/traversing/var/siblings.js
--rw-rw-rw-   0        0        0     4500 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/traversing.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.616221 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/var/
--rw-rw-rw-   0        0        0      110 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/var/ObjectFunctionString.js
--rw-rw-rw-   0        0        0       54 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/var/arr.js
--rw-rw-rw-   0        0        0       82 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/var/class2type.js
--rw-rw-rw-   0        0        0       81 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/var/concat.js
--rw-rw-rw-   0        0        0       67 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/var/document.js
--rw-rw-rw-   0        0        0      105 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/var/documentElement.js
--rw-rw-rw-   0        0        0       92 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/var/fnToString.js
--rw-rw-rw-   0        0        0       73 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/var/getProto.js
--rw-rw-rw-   0        0        0      110 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/var/hasOwn.js
--rw-rw-rw-   0        0        0       82 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/var/indexOf.js
--rw-rw-rw-   0        0        0      428 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/var/isFunction.js
--rw-rw-rw-   0        0        0      126 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/var/isWindow.js
--rw-rw-rw-   0        0        0      100 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/var/pnum.js
--rw-rw-rw-   0        0        0       79 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/var/push.js
--rw-rw-rw-   0        0        0       79 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/var/rcheckableType.js
--rw-rw-rw-   0        0        0      136 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/var/rcssNum.js
--rw-rw-rw-   0        0        0      202 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/var/rnothtmlwhite.js
--rw-rw-rw-   0        0        0       80 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/var/slice.js
--rw-rw-rw-   0        0        0      117 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/var/support.js
--rw-rw-rw-   0        0        0      104 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/var/toString.js
--rw-rw-rw-   0        0        0     1477 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/wrap.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.625271 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/
--rw-rw-rw-   0        0        0     1080 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/LICENSE
--rw-rw-rw-   0        0        0    12252 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.646222 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/dist/
--rw-rw-rw-   0        0        0    32771 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/dist/simplebar-core.esm.js
--rw-rw-rw-   0        0        0    64425 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/dist/simplebar-core.esm.js.map
--rw-rw-rw-   0        0        0     3890 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/dist/simplebar.css
--rw-rw-rw-   0        0        0     1323 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/dist/simplebar.d.ts
--rw-rw-rw-   0        0        0    36530 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/dist/simplebar.esm.js
--rw-rw-rw-   0        0        0    71785 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/dist/simplebar.esm.js.map
--rw-rw-rw-   0        0        0   171895 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/dist/simplebar.js
--rw-rw-rw-   0        0        0     2937 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/dist/simplebar.min.css
--rw-rw-rw-   0        0        0    59030 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/dist/simplebar.min.js
--rw-rw-rw-   0        0        0     4604 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/dist/simplebar.umd.js
--rw-rw-rw-   0        0        0     1719 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/package.json
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.655743 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/src/
--rw-rw-rw-   0        0        0     1104 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/src/helpers.js
--rw-rw-rw-   0        0        0     3363 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/src/index.js
--rw-rw-rw-   0        0        0      953 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/src/scrollbar-width.js
--rw-rw-rw-   0        0        0     3890 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/src/simplebar.css
--rw-rw-rw-   0        0        0    29802 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/src/simplebar.js
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.658736 django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.661248 django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/component/
--rw-rw-rw-   0        0        0      344 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/component/_card.scss
--rw-rw-rw-   0        0        0      489 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/component/_reboot.scss
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.666256 django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/layouts/
--rw-rw-rw-   0        0        0     3362 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/layouts/_header.scss
--rw-rw-rw-   0        0        0     1833 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/layouts/_layouts.scss
--rw-rw-rw-   0        0        0     2210 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/layouts/_sidebar.scss
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.667261 django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/pages/
--rw-rw-rw-   0        0        0      842 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/pages/_dashboard1.scss
--rw-rw-rw-   0        0        0    23293 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/prepros.config
--rw-rw-rw-   0        0        0      844 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/styles.scss
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.671256 django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/utilities/
--rw-rw-rw-   0        0        0      487 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/utilities/_background.scss
--rw-rw-rw-   0        0        0      236 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/utilities/_icon-size.scss
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.673279 django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/variables/
--rw-rw-rw-   0        0        0      964 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/variables/_theme-variables.scss
--rw-rw-rw-   0        0        0     5275 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/variables/_variables.scss
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.675278 django-admin-modernize-1.0.2/admin_modernize/templates/
--rw-rw-rw-   0        0        0        0 2022-09-27 05:30:21.000000 django-admin-modernize-1.0.2/admin_modernize/templates/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.702417 django-admin-modernize-1.0.2/admin_modernize/templates/accounts/
--rw-rw-rw-   0        0        0     2799 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/accounts/login.html
--rw-rw-rw-   0        0        0     1889 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/accounts/password_change.html
--rw-rw-rw-   0        0        0     1116 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/accounts/password_change_done.html
--rw-rw-rw-   0        0        0     2125 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/accounts/password_reset.html
--rw-rw-rw-   0        0        0     1252 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/accounts/password_reset_complete.html
--rw-rw-rw-   0        0        0     2120 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/accounts/password_reset_confirm.html
--rw-rw-rw-   0        0        0     1398 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/accounts/password_reset_done.html
--rw-rw-rw-   0        0        0     1988 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/accounts/register.html
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.725614 django-admin-modernize-1.0.2/admin_modernize/templates/admin/
--rw-rw-rw-   0        0        0     1606 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/admin/actions.html
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:42.291583 django-admin-modernize-1.0.2/admin_modernize/templates/admin/auth/
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.727615 django-admin-modernize-1.0.2/admin_modernize/templates/admin/auth/user/
--rw-rw-rw-   0        0        0      334 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/admin/auth/user/add_form.html
--rw-rw-rw-   0        0        0     5386 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/admin/auth/user/change_password.html
--rw-rw-rw-   0        0        0     6178 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/admin/change_form.html
--rw-rw-rw-   0        0        0      556 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/admin/change_form_object_tools.html
--rw-rw-rw-   0        0        0     5638 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/admin/change_list.html
--rw-rw-rw-   0        0        0      470 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/admin/change_list_object_tools.html
--rw-rw-rw-   0        0        0     3004 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/admin/change_list_results.html
--rw-rw-rw-   0        0        0     7167 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/admin/delete_confirmation.html
--rw-rw-rw-   0        0        0     7168 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/admin/delete_selected_confirmation.html
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.730614 django-admin-modernize-1.0.2/admin_modernize/templates/admin/edit_inline/
--rw-rw-rw-   0        0        0     3893 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/admin/edit_inline/stacked.html
--rw-rw-rw-   0        0        0     7834 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/admin/edit_inline/tabular.html
--rw-rw-rw-   0        0        0      506 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/admin/filter.html
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.736708 django-admin-modernize-1.0.2/admin_modernize/templates/admin/includes/
--rw-rw-rw-   0        0        0     2572 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/admin/includes/fieldset.html
--rw-rw-rw-   0        0        0      348 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/admin/includes/object_delete_summary.html
--rw-rw-rw-   0        0        0    19871 2023-05-01 07:41:34.000000 django-admin-modernize-1.0.2/admin_modernize/templates/admin/index.html
--rw-rw-rw-   0        0        0     2590 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/admin/invalid_setup.html
--rw-rw-rw-   0        0        0     3378 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/admin/login.html
--rw-rw-rw-   0        0        0     3922 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/admin/object_history.html
--rw-rw-rw-   0        0        0     2184 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/admin/pagination.html
--rw-rw-rw-   0        0        0     2502 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/admin/search_form.html
--rw-rw-rw-   0        0        0     1481 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/admin/submit_line.html
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.744243 django-admin-modernize-1.0.2/admin_modernize/templates/includes/
--rw-rw-rw-   0        0        0      401 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/includes/head.html
--rw-rw-rw-   0        0        0     3745 2023-05-01 07:44:07.000000 django-admin-modernize-1.0.2/admin_modernize/templates/includes/navigation.html
--rw-rw-rw-   0        0        0      548 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/includes/scripts.html
--rw-rw-rw-   0        0        0     6445 2023-05-01 07:44:30.000000 django-admin-modernize-1.0.2/admin_modernize/templates/includes/sidebar.html
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.751244 django-admin-modernize-1.0.2/admin_modernize/templates/layouts/
--rw-rw-rw-   0        0        0     1130 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/layouts/auth_base.html
--rw-rw-rw-   0        0        0      842 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/layouts/base.html
--rw-rw-rw-   0        0        0     1037 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/layouts/base_logout.html
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.773999 django-admin-modernize-1.0.2/admin_modernize/templates/pages/
--rw-rw-rw-   0        0        0      481 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/pages/icon-tabler.html
--rw-rw-rw-   0        0        0    19821 2023-05-01 07:42:03.000000 django-admin-modernize-1.0.2/admin_modernize/templates/pages/index.html
--rw-rw-rw-   0        0        0      343 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/pages/sample-page.html
--rw-rw-rw-   0        0        0     2710 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/pages/sign-in.html
--rw-rw-rw-   0        0        0     2404 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/pages/sign-up.html
--rw-rw-rw-   0        0        0     1705 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/pages/ui-alerts.html
--rw-rw-rw-   0        0        0     2087 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/pages/ui-buttons.html
--rw-rw-rw-   0        0        0     2218 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/pages/ui-card.html
--rw-rw-rw-   0        0        0     2766 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/pages/ui-forms.html
--rw-rw-rw-   0        0        0     1563 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/pages/ui-typography.html
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.780005 django-admin-modernize-1.0.2/admin_modernize/templates/registration/
--rw-rw-rw-   0        0        0     1527 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/registration/logged_out.html
--rw-rw-rw-   0        0        0     2786 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/registration/password_change_done.html
--rw-rw-rw-   0        0        0     4185 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templates/registration/password_change_form.html
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.785531 django-admin-modernize-1.0.2/admin_modernize/templatetags/
--rw-rw-rw-   0        0        0        0 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templatetags/__init__.py
--rw-rw-rw-   0        0        0     2476 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/templatetags/admin_modernize.py
--rw-rw-rw-   0        0        0       63 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/tests.py
--rw-rw-rw-   0        0        0     1789 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/urls.py
--rw-rw-rw-   0        0        0    16503 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/utils.py
--rw-rw-rw-   0        0        0     2071 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.2/admin_modernize/views.py
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.793144 django-admin-modernize-1.0.2/django_admin_modernize.egg-info/
--rw-rw-rw-   0        0        0     6248 2023-05-01 07:51:41.000000 django-admin-modernize-1.0.2/django_admin_modernize.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    47647 2023-05-01 07:51:42.000000 django-admin-modernize-1.0.2/django_admin_modernize.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 07:51:41.000000 django-admin-modernize-1.0.2/django_admin_modernize.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-01 07:50:54.000000 django-admin-modernize-1.0.2/django_admin_modernize.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2023-05-01 07:51:41.000000 django-admin-modernize-1.0.2/django_admin_modernize.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 07:51:44.795254 django-admin-modernize-1.0.2/docs/
--rw-rw-rw-   0        0        0       13 2022-09-27 05:30:21.000000 django-admin-modernize-1.0.2/docs/blank.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 07:51:44.798108 django-admin-modernize-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1351 2023-05-01 07:51:22.000000 django-admin-modernize-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.698696 django-admin-modernize-1.0.3/
+-rw-rw-rw-   0        0        0     1113 2022-09-27 05:30:21.000000 django-admin-modernize-1.0.3/LICENSE.md
+-rw-rw-rw-   0        0        0      152 2023-04-29 10:04:52.000000 django-admin-modernize-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6248 2023-05-01 07:58:52.697694 django-admin-modernize-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5168 2023-05-01 07:49:16.000000 django-admin-modernize-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.295022 django-admin-modernize-1.0.3/admin_modernize/
+-rw-rw-rw-   0        0        0       78 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/__init__.py
+-rw-rw-rw-   0        0        0       34 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/admin.py
+-rw-rw-rw-   0        0        0      268 2023-04-29 10:06:11.000000 django-admin-modernize-1.0.3/admin_modernize/apps.py
+-rw-rw-rw-   0        0        0     2907 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/forms.py
+-rw-rw-rw-   0        0        0       60 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/models.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.297021 django-admin-modernize-1.0.3/admin_modernize/static/
+-rw-rw-rw-   0        0        0        0 2022-09-27 05:30:21.000000 django-admin-modernize-1.0.3/admin_modernize/static/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.256202 django-admin-modernize-1.0.3/admin_modernize/static/assets/
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.308553 django-admin-modernize-1.0.3/admin_modernize/static/assets/css/
+-rw-rw-rw-   0        0        0     9582 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/css/forms.css
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:50.971322 django-admin-modernize-1.0.3/admin_modernize/static/assets/css/icons/
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.311072 django-admin-modernize-1.0.3/admin_modernize/static/assets/css/icons/tabler-icons/
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.339156 django-admin-modernize-1.0.3/admin_modernize/static/assets/css/icons/tabler-icons/fonts/
+-rw-rw-rw-   0        0        0  1521944 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/css/icons/tabler-icons/fonts/tabler-icons.eot
+-rw-rw-rw-   0        0        0  6046707 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/css/icons/tabler-icons/fonts/tabler-icons.svg
+-rw-rw-rw-   0        0        0  1521760 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/css/icons/tabler-icons/fonts/tabler-icons.ttf
+-rw-rw-rw-   0        0        0   775616 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/css/icons/tabler-icons/fonts/tabler-icons.woff
+-rw-rw-rw-   0        0        0   552144 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/css/icons/tabler-icons/fonts/tabler-icons.woff2
+-rw-rw-rw-   0        0        0   146896 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/css/icons/tabler-icons/tabler-icons.css
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.343689 django-admin-modernize-1.0.3/admin_modernize/static/assets/css/plugins/
+-rw-rw-rw-   0        0        0    58139 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/css/plugins/animate.min.css
+-rw-rw-rw-   0        0        0   193535 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/css/plugins/bootstrap.min.css
+-rw-rw-rw-   0        0        0   200840 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/css/style-preset.css
+-rw-rw-rw-   0        0        0   339626 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/css/styles.css
+-rw-rw-rw-   0        0        0   335915 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/css/styles.min.css
+-rw-rw-rw-   0        0        0    12535 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/css/widgets.css
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:50.977322 django-admin-modernize-1.0.3/admin_modernize/static/assets/images/
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.345690 django-admin-modernize-1.0.3/admin_modernize/static/assets/images/backgrounds/
+-rw-rw-rw-   0        0        0    15492 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/images/backgrounds/rocket.png
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.348689 django-admin-modernize-1.0.3/admin_modernize/static/assets/images/logos/
+-rw-rw-rw-   0        0        0     6618 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/images/logos/dark-logo.svg
+-rw-rw-rw-   0        0        0      583 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/images/logos/favicon.png
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.358745 django-admin-modernize-1.0.3/admin_modernize/static/assets/images/products/
+-rw-rw-rw-   0        0        0   117358 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/images/products/s1.jpg
+-rw-rw-rw-   0        0        0   231624 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/images/products/s11.jpg
+-rw-rw-rw-   0        0        0    84198 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/images/products/s4.jpg
+-rw-rw-rw-   0        0        0   124284 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/images/products/s5.jpg
+-rw-rw-rw-   0        0        0    78225 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/images/products/s7.jpg
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.360265 django-admin-modernize-1.0.3/admin_modernize/static/assets/images/profile/
+-rw-rw-rw-   0        0        0    30954 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/images/profile/user-1.jpg
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.367279 django-admin-modernize-1.0.3/admin_modernize/static/assets/js/
+-rw-rw-rw-   0        0        0     1263 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/js/app.min.js
+-rw-rw-rw-   0        0        0     3840 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/js/dashboard.js
+-rw-rw-rw-   0        0        0     1846 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/js/sidebarmenu.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.254193 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.373458 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/
+-rw-rw-rw-   0        0        0     1076 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/LICENSE
+-rw-rw-rw-   0        0        0    14275 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.389001 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/
+-rw-rw-rw-   0        0        0   549363 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.amd.js
+-rw-rw-rw-   0        0        0   502932 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.common.js
+-rw-rw-rw-   0        0        0    12763 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.css
+-rw-rw-rw-   0        0        0   502923 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.esm.js
+-rw-rw-rw-   0        0        0  1147184 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.js
+-rw-rw-rw-   0        0        0   503168 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.min.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.476866 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/
+-rw-rw-rw-   0        0        0     1004 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/ar.json
+-rw-rw-rw-   0        0        0     1013 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/ca.json
+-rw-rw-rw-   0        0        0     1011 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/cs.json
+-rw-rw-rw-   0        0        0     1006 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/de.json
+-rw-rw-rw-   0        0        0     1324 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/el.json
+-rw-rw-rw-   0        0        0      983 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/en.json
+-rw-rw-rw-   0        0        0     1001 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/es.json
+-rw-rw-rw-   0        0        0     1055 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/et.json
+-rw-rw-rw-   0        0        0     1170 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/fa.json
+-rw-rw-rw-   0        0        0     1030 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/fi.json
+-rw-rw-rw-   0        0        0     1071 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/fr.json
+-rw-rw-rw-   0        0        0     1129 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/he.json
+-rw-rw-rw-   0        0        0     1508 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/hi.json
+-rw-rw-rw-   0        0        0     1035 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/hr.json
+-rw-rw-rw-   0        0        0     1164 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/hu.json
+-rw-rw-rw-   0        0        0     1323 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/hy.json
+-rw-rw-rw-   0        0        0      917 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/id.json
+-rw-rw-rw-   0        0        0      996 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/it.json
+-rw-rw-rw-   0        0        0     1028 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/ja.json
+-rw-rw-rw-   0        0        0     1618 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/ka.json
+-rw-rw-rw-   0        0        0     1002 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/ko.json
+-rw-rw-rw-   0        0        0     1064 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/lt.json
+-rw-rw-rw-   0        0        0     1122 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/lv.json
+-rw-rw-rw-   0        0        0      968 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/nb.json
+-rw-rw-rw-   0        0        0      988 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/nl.json
+-rw-rw-rw-   0        0        0     1012 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/pl.json
+-rw-rw-rw-   0        0        0      989 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/pt-br.json
+-rw-rw-rw-   0        0        0     1017 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/pt.json
+-rw-rw-rw-   0        0        0      998 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/rs.json
+-rw-rw-rw-   0        0        0     1268 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/ru.json
+-rw-rw-rw-   0        0        0      986 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/se.json
+-rw-rw-rw-   0        0        0     1006 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/sk.json
+-rw-rw-rw-   0        0        0      982 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/sl.json
+-rw-rw-rw-   0        0        0      999 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/sq.json
+-rw-rw-rw-   0        0        0     1484 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/th.json
+-rw-rw-rw-   0        0        0     1011 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/tr.json
+-rw-rw-rw-   0        0        0     1277 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/ua.json
+-rw-rw-rw-   0        0        0     1055 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/zh-cn.json
+-rw-rw-rw-   0        0        0     1055 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/zh-tw.json
+-rw-rw-rw-   0        0        0     3089 2023-04-29 09:52:33.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/package.json
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.479869 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/
+-rw-rw-rw-   0        0        0    22769 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/apexcharts.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.506950 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/assets/
+-rw-rw-rw-   0        0        0    13601 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/assets/apexcharts.css
+-rw-rw-rw-   0        0        0      355 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-camera.svg
+-rw-rw-rw-   0        0        0      199 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-home.svg
+-rw-rw-rw-   0        0        0      185 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-menu.svg
+-rw-rw-rw-   0        0        0      416 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-minus-square.svg
+-rw-rw-rw-   0        0        0      289 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-minus.svg
+-rw-rw-rw-   0        0        0      656 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-pan-hand.svg
+-rw-rw-rw-   0        0        0      269 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-pan.svg
+-rw-rw-rw-   0        0        0      263 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-plus-square.svg
+-rw-rw-rw-   0        0        0      308 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-plus.svg
+-rw-rw-rw-   0        0        0      366 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-refresh.svg
+-rw-rw-rw-   0        0        0      265 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-reset.svg
+-rw-rw-rw-   0        0        0      439 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-select.svg
+-rw-rw-rw-   0        0        0      231 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-select1.svg
+-rw-rw-rw-   0        0        0      450 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-zoom-in.svg
+-rw-rw-rw-   0        0        0      600 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-zoom-out.svg
+-rw-rw-rw-   0        0        0      301 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-zoom.svg
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.525999 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/
+-rw-rw-rw-   0        0        0    12112 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/Bar.js
+-rw-rw-rw-   0        0        0    13155 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/BarStacked.js
+-rw-rw-rw-   0        0        0    12007 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/BoxCandleStick.js
+-rw-rw-rw-   0        0        0     6370 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/HeatMap.js
+-rw-rw-rw-   0        0        0    19401 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/Line.js
+-rw-rw-rw-   0        0        0    28958 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/Pie.js
+-rw-rw-rw-   0        0        0    13446 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/Radar.js
+-rw-rw-rw-   0        0        0    12331 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/Radial.js
+-rw-rw-rw-   0        0        0    11291 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/RangeBar.js
+-rw-rw-rw-   0        0        0     7196 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/Scatter.js
+-rw-rw-rw-   0        0        0     7802 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/Treemap.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:50.987846 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/common/
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.530501 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/common/bar/
+-rw-rw-rw-   0        0        0    11250 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/common/bar/DataLabels.js
+-rw-rw-rw-   0        0        0    16884 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/common/bar/Helpers.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.531507 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/common/circle/
+-rw-rw-rw-   0        0        0      832 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/common/circle/Helpers.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.532507 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/common/line/
+-rw-rw-rw-   0        0        0     4369 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/common/line/Helpers.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.534511 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/common/treemap/
+-rw-rw-rw-   0        0        0     5077 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/common/treemap/Helpers.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.535511 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/libs/
+-rw-rw-rw-   0        0        0     9417 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/libs/Treemap-squared.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.595268 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/
+-rw-rw-rw-   0        0        0     1004 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/ar.json
+-rw-rw-rw-   0        0        0     1013 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/ca.json
+-rw-rw-rw-   0        0        0     1011 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/cs.json
+-rw-rw-rw-   0        0        0     1006 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/de.json
+-rw-rw-rw-   0        0        0     1324 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/el.json
+-rw-rw-rw-   0        0        0      983 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/en.json
+-rw-rw-rw-   0        0        0     1001 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/es.json
+-rw-rw-rw-   0        0        0     1055 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/et.json
+-rw-rw-rw-   0        0        0     1170 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/fa.json
+-rw-rw-rw-   0        0        0     1030 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/fi.json
+-rw-rw-rw-   0        0        0     1071 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/fr.json
+-rw-rw-rw-   0        0        0     1129 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/he.json
+-rw-rw-rw-   0        0        0     1508 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/hi.json
+-rw-rw-rw-   0        0        0     1035 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/hr.json
+-rw-rw-rw-   0        0        0     1164 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/hu.json
+-rw-rw-rw-   0        0        0     1323 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/hy.json
+-rw-rw-rw-   0        0        0      917 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/id.json
+-rw-rw-rw-   0        0        0      996 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/it.json
+-rw-rw-rw-   0        0        0     1028 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/ja.json
+-rw-rw-rw-   0        0        0     1618 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/ka.json
+-rw-rw-rw-   0        0        0     1002 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/ko.json
+-rw-rw-rw-   0        0        0     1064 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/lt.json
+-rw-rw-rw-   0        0        0     1122 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/lv.json
+-rw-rw-rw-   0        0        0      968 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/nb.json
+-rw-rw-rw-   0        0        0      988 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/nl.json
+-rw-rw-rw-   0        0        0     1012 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/pl.json
+-rw-rw-rw-   0        0        0      989 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/pt-br.json
+-rw-rw-rw-   0        0        0     1017 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/pt.json
+-rw-rw-rw-   0        0        0      998 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/rs.json
+-rw-rw-rw-   0        0        0     1268 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/ru.json
+-rw-rw-rw-   0        0        0      986 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/se.json
+-rw-rw-rw-   0        0        0     1006 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/sk.json
+-rw-rw-rw-   0        0        0      982 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/sl.json
+-rw-rw-rw-   0        0        0      999 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/sq.json
+-rw-rw-rw-   0        0        0     1484 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/th.json
+-rw-rw-rw-   0        0        0     1011 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/tr.json
+-rw-rw-rw-   0        0        0     1277 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/ua.json
+-rw-rw-rw-   0        0        0     1055 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/zh-cn.json
+-rw-rw-rw-   0        0        0     1055 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/zh-tw.json
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.633907 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/
+-rw-rw-rw-   0        0        0     5782 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Animations.js
+-rw-rw-rw-   0        0        0      479 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Base.js
+-rw-rw-rw-   0        0        0    17431 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Core.js
+-rw-rw-rw-   0        0        0     9891 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/CoreUtils.js
+-rw-rw-rw-   0        0        0     3692 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Crosshairs.js
+-rw-rw-rw-   0        0        0    20941 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Data.js
+-rw-rw-rw-   0        0        0     9971 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/DataLabels.js
+-rw-rw-rw-   0        0        0     3048 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Events.js
+-rw-rw-rw-   0        0        0    10938 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Exports.js
+-rw-rw-rw-   0        0        0    10063 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Fill.js
+-rw-rw-rw-   0        0        0     5604 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Filters.js
+-rw-rw-rw-   0        0        0     4960 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Formatters.js
+-rw-rw-rw-   0        0        0    21067 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Graphics.js
+-rw-rw-rw-   0        0        0     7059 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Markers.js
+-rw-rw-rw-   0        0        0    16559 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Range.js
+-rw-rw-rw-   0        0        0     2083 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Responsive.js
+-rw-rw-rw-   0        0        0    16955 2023-04-29 09:52:34.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Scales.js
+-rw-rw-rw-   0        0        0    12234 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Series.js
+-rw-rw-rw-   0        0        0     7170 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Theme.js
+-rw-rw-rw-   0        0        0    24177 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/TimeScale.js
+-rw-rw-rw-   0        0        0     1262 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/TitleSubtitle.js
+-rw-rw-rw-   0        0        0    14827 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Toolbar.js
+-rw-rw-rw-   0        0        0    22002 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/ZoomPanSelection.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.641431 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/annotations/
+-rw-rw-rw-   0        0        0     8325 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/annotations/Annotations.js
+-rw-rw-rw-   0        0        0     6530 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/annotations/Helpers.js
+-rw-rw-rw-   0        0        0     3146 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/annotations/PointsAnnotations.js
+-rw-rw-rw-   0        0        0     3145 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/annotations/XAxisAnnotations.js
+-rw-rw-rw-   0        0        0     2926 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/annotations/YAxisAnnotations.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.650959 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/axes/
+-rw-rw-rw-   0        0        0      904 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/axes/Axes.js
+-rw-rw-rw-   0        0        0     6093 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/axes/AxesUtils.js
+-rw-rw-rw-   0        0        0    13749 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/axes/Grid.js
+-rw-rw-rw-   0        0        0    19087 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/axes/XAxis.js
+-rw-rw-rw-   0        0        0    16055 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/axes/YAxis.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.660151 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/dimensions/
+-rw-rw-rw-   0        0        0     9510 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/dimensions/Dimensions.js
+-rw-rw-rw-   0        0        0     3681 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/dimensions/Grid.js
+-rw-rw-rw-   0        0        0     2388 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/dimensions/Helpers.js
+-rw-rw-rw-   0        0        0    10704 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/dimensions/XAxis.js
+-rw-rw-rw-   0        0        0     5444 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/dimensions/YAxis.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.667682 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/helpers/
+-rw-rw-rw-   0        0        0     2310 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/helpers/Destroy.js
+-rw-rw-rw-   0        0        0     3122 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/helpers/InitCtxVariables.js
+-rw-rw-rw-   0        0        0     1245 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/helpers/Localization.js
+-rw-rw-rw-   0        0        0     9031 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/helpers/UpdateHelpers.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.670235 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/legend/
+-rw-rw-rw-   0        0        0     9280 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/legend/Helpers.js
+-rw-rw-rw-   0        0        0    14694 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/legend/Legend.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.678252 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/settings/
+-rw-rw-rw-   0        0        0     9734 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/settings/Config.js
+-rw-rw-rw-   0        0        0    16712 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/settings/Defaults.js
+-rw-rw-rw-   0        0        0     8637 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/settings/Globals.js
+-rw-rw-rw-   0        0        0    27224 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/settings/Options.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.693933 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/
+-rw-rw-rw-   0        0        0     5936 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/AxesTooltip.js
+-rw-rw-rw-   0        0        0     9729 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Intersect.js
+-rw-rw-rw-   0        0        0    14229 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Labels.js
+-rw-rw-rw-   0        0        0     5119 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Marker.js
+-rw-rw-rw-   0        0        0    12341 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Position.js
+-rw-rw-rw-   0        0        0      723 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/README.md
+-rw-rw-rw-   0        0        0    25334 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Tooltip.js
+-rw-rw-rw-   0        0        0     9947 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Utils.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.695934 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/svgjs/
+-rw-rw-rw-   0        0        0   103950 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/svgjs/svg.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.701460 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/utils/
+-rw-rw-rw-   0        0        0     6856 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/utils/DateTime.js
+-rw-rw-rw-   0        0        0     1538 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/utils/Resize.js
+-rw-rw-rw-   0        0        0    10168 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/utils/Utils.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.702492 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/types/
+-rw-rw-rw-   0        0        0    26539 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/types/apexcharts.d.ts
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.707454 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/
+-rw-rw-rw-   0        0        0     1131 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/LICENSE
+-rw-rw-rw-   0        0        0    13743 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.202005 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.773593 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/
+-rw-rw-rw-   0        0        0    75616 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.css
+-rw-rw-rw-   0        0        0   226018 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.css.map
+-rw-rw-rw-   0        0        0    56464 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.min.css
+-rw-rw-rw-   0        0        0   142342 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.min.css.map
+-rw-rw-rw-   0        0        0    75690 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.rtl.css
+-rw-rw-rw-   0        0        0   226022 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.rtl.css.map
+-rw-rw-rw-   0        0        0    56539 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.rtl.min.css
+-rw-rw-rw-   0        0        0   142419 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map
+-rw-rw-rw-   0        0        0    11735 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.css
+-rw-rw-rw-   0        0        0   126626 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.css.map
+-rw-rw-rw-   0        0        0     9817 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.min.css
+-rw-rw-rw-   0        0        0    51406 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.min.css.map
+-rw-rw-rw-   0        0        0    11728 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.rtl.css
+-rw-rw-rw-   0        0        0   126641 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.rtl.css.map
+-rw-rw-rw-   0        0        0     9889 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.rtl.min.css
+-rw-rw-rw-   0        0        0    63643 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map
+-rw-rw-rw-   0        0        0    96254 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.css
+-rw-rw-rw-   0        0        0   250681 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.css.map
+-rw-rw-rw-   0        0        0    74887 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.min.css
+-rw-rw-rw-   0        0        0   163881 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.min.css.map
+-rw-rw-rw-   0        0        0    96121 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.rtl.css
+-rw-rw-rw-   0        0        0   250622 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.rtl.css.map
+-rw-rw-rw-   0        0        0    74815 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.rtl.min.css
+-rw-rw-rw-   0        0        0   163716 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map
+-rw-rw-rw-   0        0        0   267476 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.css
+-rw-rw-rw-   0        0        0   658460 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.css.map
+-rw-rw-rw-   0        0        0   220780 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0   568408 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.min.css.map
+-rw-rw-rw-   0        0        0   267055 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.rtl.css
+-rw-rw-rw-   0        0        0   658305 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.rtl.css.map
+-rw-rw-rw-   0        0        0   220887 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.rtl.min.css
+-rw-rw-rw-   0        0        0   567947 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.rtl.min.css.map
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.802220 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/
+-rw-rw-rw-   0        0        0   208288 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.bundle.js
+-rw-rw-rw-   0        0        0   448884 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.bundle.js.map
+-rw-rw-rw-   0        0        0    80599 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   333974 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.bundle.min.js.map
+-rw-rw-rw-   0        0        0   136243 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.esm.js
+-rw-rw-rw-   0        0        0   305274 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.esm.js.map
+-rw-rw-rw-   0        0        0    74135 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.esm.min.js
+-rw-rw-rw-   0        0        0   222070 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.esm.min.js.map
+-rw-rw-rw-   0        0        0   145819 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.js
+-rw-rw-rw-   0        0        0   306458 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.js.map
+-rw-rw-rw-   0        0        0    60554 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0   217885 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.min.js.map
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.804256 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.846243 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/
+-rw-rw-rw-   0        0        0     3140 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/alert.js
+-rw-rw-rw-   0        0        0     4294 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/alert.js.map
+-rw-rw-rw-   0        0        0     3224 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/base-component.js
+-rw-rw-rw-   0        0        0     4602 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/base-component.js.map
+-rw-rw-rw-   0        0        0     2756 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/button.js
+-rw-rw-rw-   0        0        0     3466 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/button.js.map
+-rw-rw-rw-   0        0        0    14281 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/carousel.js
+-rw-rw-rw-   0        0        0    27442 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/carousel.js.map
+-rw-rw-rw-   0        0        0     9455 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/collapse.js
+-rw-rw-rw-   0        0        0    18212 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/collapse.js.map
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.858341 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/
+-rw-rw-rw-   0        0        0     2119 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/data.js
+-rw-rw-rw-   0        0        0     3047 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/data.js.map
+-rw-rw-rw-   0        0        0     9578 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/event-handler.js
+-rw-rw-rw-   0        0        0    19800 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/event-handler.js.map
+-rw-rw-rw-   0        0        0     2438 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/manipulator.js
+-rw-rw-rw-   0        0        0     4319 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/manipulator.js.map
+-rw-rw-rw-   0        0        0     2700 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/selector-engine.js
+-rw-rw-rw-   0        0        0     4619 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/selector-engine.js.map
+-rw-rw-rw-   0        0        0    16199 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/dropdown.js
+-rw-rw-rw-   0        0        0    29448 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/dropdown.js.map
+-rw-rw-rw-   0        0        0    12194 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/modal.js
+-rw-rw-rw-   0        0        0    22634 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/modal.js.map
+-rw-rw-rw-   0        0        0     9166 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/offcanvas.js
+-rw-rw-rw-   0        0        0    16142 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/offcanvas.js.map
+-rw-rw-rw-   0        0        0     2883 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/popover.js
+-rw-rw-rw-   0        0        0     4053 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/popover.js.map
+-rw-rw-rw-   0        0        0    10303 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/scrollspy.js
+-rw-rw-rw-   0        0        0    18973 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/scrollspy.js.map
+-rw-rw-rw-   0        0        0    10647 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/tab.js
+-rw-rw-rw-   0        0        0    19947 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/tab.js.map
+-rw-rw-rw-   0        0        0     6632 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/toast.js
+-rw-rw-rw-   0        0        0    12018 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/toast.js.map
+-rw-rw-rw-   0        0        0    19225 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/tooltip.js
+-rw-rw-rw-   0        0        0    37599 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/tooltip.js.map
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.896009 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/
+-rw-rw-rw-   0        0        0     4413 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/backdrop.js
+-rw-rw-rw-   0        0        0     7172 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/backdrop.js.map
+-rw-rw-rw-   0        0        0     2174 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/component-functions.js
+-rw-rw-rw-   0        0        0     2310 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/component-functions.js.map
+-rw-rw-rw-   0        0        0     2808 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/config.js
+-rw-rw-rw-   0        0        0     4073 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/config.js.map
+-rw-rw-rw-   0        0        0     3913 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/focustrap.js
+-rw-rw-rw-   0        0        0     5891 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/focustrap.js.map
+-rw-rw-rw-   0        0        0    10248 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/index.js
+-rw-rw-rw-   0        0        0    18675 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/index.js.map
+-rw-rw-rw-   0        0        0     4253 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/sanitizer.js
+-rw-rw-rw-   0        0        0     7572 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/sanitizer.js.map
+-rw-rw-rw-   0        0        0     5031 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/scrollbar.js
+-rw-rw-rw-   0        0        0     8041 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/scrollbar.js.map
+-rw-rw-rw-   0        0        0     4733 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/swipe.js
+-rw-rw-rw-   0        0        0     8335 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/swipe.js.map
+-rw-rw-rw-   0        0        0     4980 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/template-factory.js
+-rw-rw-rw-   0        0        0     8655 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/template-factory.js.map
+-rw-rw-rw-   0        0        0      881 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/index.esm.js
+-rw-rw-rw-   0        0        0      848 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/index.umd.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.921936 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/
+-rw-rw-rw-   0        0        0     1901 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/alert.js
+-rw-rw-rw-   0        0        0     1930 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/base-component.js
+-rw-rw-rw-   0        0        0     1626 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/button.js
+-rw-rw-rw-   0        0        0    11820 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/carousel.js
+-rw-rw-rw-   0        0        0     7669 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/collapse.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.930457 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/dom/
+-rw-rw-rw-   0        0        0     1405 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/dom/data.js
+-rw-rw-rw-   0        0        0     8450 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/dom/event-handler.js
+-rw-rw-rw-   0        0        0     1668 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/dom/manipulator.js
+-rw-rw-rw-   0        0        0     1968 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/dom/selector-engine.js
+-rw-rw-rw-   0        0        0    13257 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/dropdown.js
+-rw-rw-rw-   0        0        0     9629 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/modal.js
+-rw-rw-rw-   0        0        0     6804 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/offcanvas.js
+-rw-rw-rw-   0        0        0     1874 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/popover.js
+-rw-rw-rw-   0        0        0     8448 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/scrollspy.js
+-rw-rw-rw-   0        0        0     8756 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/tab.js
+-rw-rw-rw-   0        0        0     5037 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/toast.js
+-rw-rw-rw-   0        0        0    16188 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/tooltip.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.946016 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/util/
+-rw-rw-rw-   0        0        0     3126 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/util/backdrop.js
+-rw-rw-rw-   0        0        0     1072 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/util/component-functions.js
+-rw-rw-rw-   0        0        0     1818 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/util/config.js
+-rw-rw-rw-   0        0        0     2519 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/util/focustrap.js
+-rw-rw-rw-   0        0        0     8436 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/util/index.js
+-rw-rw-rw-   0        0        0     3253 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/util/sanitizer.js
+-rw-rw-rw-   0        0        0     3755 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/util/scrollbar.js
+-rw-rw-rw-   0        0        0     3410 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/util/swipe.js
+-rw-rw-rw-   0        0        0     3630 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/util/template-factory.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.951526 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/
+-rw-rw-rw-   0        0        0     3131 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/README.md
+-rw-rw-rw-   0        0        0     1511 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/browsers.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.952521 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/helpers/
+-rw-rw-rw-   0        0        0     1156 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/helpers/fixture.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.960588 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/integration/
+-rw-rw-rw-   0        0        0      236 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/integration/bundle-modularity.js
+-rw-rw-rw-   0        0        0      226 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/integration/bundle.js
+-rw-rw-rw-   0        0        0     4274 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/integration/index.html
+-rw-rw-rw-   0        0        0      358 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/integration/rollup.bundle-modularity.js
+-rw-rw-rw-   0        0        0      539 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/integration/rollup.bundle.js
+-rw-rw-rw-   0        0        0     4106 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/karma.conf.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.999233 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/
+-rw-rw-rw-   0        0        0      247 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/.eslintrc.json
+-rw-rw-rw-   0        0        0     7571 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/alert.spec.js
+-rw-rw-rw-   0        0        0     4928 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/base-component.spec.js
+-rw-rw-rw-   0        0        0     5424 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/button.spec.js
+-rw-rw-rw-   0        0        0    52616 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/carousel.spec.js
+-rw-rw-rw-   0        0        0    38351 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/collapse.spec.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.008763 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/dom/
+-rw-rw-rw-   0        0        0     2621 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/dom/data.spec.js
+-rw-rw-rw-   0        0        0    13110 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/dom/event-handler.spec.js
+-rw-rw-rw-   0        0        0     4616 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/dom/manipulator.spec.js
+-rw-rw-rw-   0        0        0     6892 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/dom/selector-engine.spec.js
+-rw-rw-rw-   0        0        0    85853 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/dropdown.spec.js
+-rw-rw-rw-   0        0        0     1988 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/jquery.spec.js
+-rw-rw-rw-   0        0        0    40009 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/modal.spec.js
+-rw-rw-rw-   0        0        0    29788 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/offcanvas.spec.js
+-rw-rw-rw-   0        0        0    13775 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/popover.spec.js
+-rw-rw-rw-   0        0        0    32996 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/scrollspy.spec.js
+-rw-rw-rw-   0        0        0    42678 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/tab.spec.js
+-rw-rw-rw-   0        0        0    19308 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/toast.spec.js
+-rw-rw-rw-   0        0        0    49199 2023-04-29 09:52:36.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/tooltip.spec.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.023899 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/
+-rw-rw-rw-   0        0        0     9342 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/backdrop.spec.js
+-rw-rw-rw-   0        0        0     3422 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/component-functions.spec.js
+-rw-rw-rw-   0        0        0     5498 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/config.spec.js
+-rw-rw-rw-   0        0        0     6901 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/focustrap.spec.js
+-rw-rw-rw-   0        0        0    25378 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/index.spec.js
+-rw-rw-rw-   0        0        0     3234 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/sanitizer.spec.js
+-rw-rw-rw-   0        0        0    13963 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/scrollbar.spec.js
+-rw-rw-rw-   0        0        0     8107 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/swipe.spec.js
+-rw-rw-rw-   0        0        0     8929 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/template-factory.spec.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.044833 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/
+-rw-rw-rw-   0        0        0      301 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/.eslintrc.json
+-rw-rw-rw-   0        0        0     2189 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/alert.html
+-rw-rw-rw-   0        0        0     2898 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/button.html
+-rw-rw-rw-   0        0        0     2867 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/carousel.html
+-rw-rw-rw-   0        0        0     5326 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/collapse.html
+-rw-rw-rw-   0        0        0     9958 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/dropdown.html
+-rw-rw-rw-   0        0        0    15667 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/modal.html
+-rw-rw-rw-   0        0        0     1853 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/popover.html
+-rw-rw-rw-   0        0        0    18801 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/scrollspy.html
+-rw-rw-rw-   0        0        0    32225 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/tab.html
+-rw-rw-rw-   0        0        0     2580 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/toast.html
+-rw-rw-rw-   0        0        0     6309 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/tooltip.html
+-rw-rw-rw-   0        0        0     9286 2023-04-29 09:52:35.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/package.json
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.153222 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/
+-rw-rw-rw-   0        0        0     5066 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_accordion.scss
+-rw-rw-rw-   0        0        0     2055 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_alert.scss
+-rw-rw-rw-   0        0        0     1118 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_badge.scss
+-rw-rw-rw-   0        0        0     1751 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_breadcrumb.scss
+-rw-rw-rw-   0        0        0     3195 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_button-group.scss
+-rw-rw-rw-   0        0        0     6685 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_buttons.scss
+-rw-rw-rw-   0        0        0     6941 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_card.scss
+-rw-rw-rw-   0        0        0     5751 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_carousel.scss
+-rw-rw-rw-   0        0        0     1948 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_close.scss
+-rw-rw-rw-   0        0        0     1201 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_containers.scss
+-rw-rw-rw-   0        0        0     8093 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_dropdown.scss
+-rw-rw-rw-   0        0        0      256 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_forms.scss
+-rw-rw-rw-   0        0        0    10554 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_functions.scss
+-rw-rw-rw-   0        0        0      575 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_grid.scss
+-rw-rw-rw-   0        0        0      294 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_helpers.scss
+-rw-rw-rw-   0        0        0     1158 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_images.scss
+-rw-rw-rw-   0        0        0     6775 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_list-group.scss
+-rw-rw-rw-   0        0        0     4043 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_maps.scss
+-rw-rw-rw-   0        0        0      875 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_mixins.scss
+-rw-rw-rw-   0        0        0     7762 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_modal.scss
+-rw-rw-rw-   0        0        0     4665 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_nav.scss
+-rw-rw-rw-   0        0        0     9104 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_navbar.scss
+-rw-rw-rw-   0        0        0     4725 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_offcanvas.scss
+-rw-rw-rw-   0        0        0     3944 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_pagination.scss
+-rw-rw-rw-   0        0        0      859 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_placeholders.scss
+-rw-rw-rw-   0        0        0     6907 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_popover.scss
+-rw-rw-rw-   0        0        0     2016 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_progress.scss
+-rw-rw-rw-   0        0        0    12404 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_reboot.scss
+-rw-rw-rw-   0        0        0     7371 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_root.scss
+-rw-rw-rw-   0        0        0     2429 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_spinners.scss
+-rw-rw-rw-   0        0        0     4413 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_tables.scss
+-rw-rw-rw-   0        0        0     2490 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_toasts.scss
+-rw-rw-rw-   0        0        0     3939 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_tooltip.scss
+-rw-rw-rw-   0        0        0      425 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_transitions.scss
+-rw-rw-rw-   0        0        0     1420 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_type.scss
+-rw-rw-rw-   0        0        0    17886 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_utilities.scss
+-rw-rw-rw-   0        0        0     3840 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_variables-dark.scss
+-rw-rw-rw-   0        0        0    73610 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_variables.scss
+-rw-rw-rw-   0        0        0    75614 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-grid.css
+-rw-rw-rw-   0        0        0    34422 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-grid.css.map
+-rw-rw-rw-   0        0        0     1253 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-grid.scss
+-rw-rw-rw-   0        0        0    11668 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-reboot.css
+-rw-rw-rw-   0        0        0     4760 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-reboot.css.map
+-rw-rw-rw-   0        0        0      189 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-reboot.scss
+-rw-rw-rw-   0        0        0    96160 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-utilities.css
+-rw-rw-rw-   0        0        0    43440 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-utilities.css.map
+-rw-rw-rw-   0        0        0      306 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-utilities.scss
+-rw-rw-rw-   0        0        0   266178 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap.css
+-rw-rw-rw-   0        0        0   103943 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap.css.map
+-rw-rw-rw-   0        0        0      938 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap.scss
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.199929 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/css/
+-rw-rw-rw-   0        0        0    75568 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-grid.css
+-rw-rw-rw-   0        0        0    34458 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-grid.css.map
+-rw-rw-rw-   0        0        0    11620 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-reboot.css
+-rw-rw-rw-   0        0        0     4781 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-reboot.css.map
+-rw-rw-rw-   0        0        0    96109 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-utilities.css
+-rw-rw-rw-   0        0        0    43500 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-utilities.css.map
+-rw-rw-rw-   0        0        0   266137 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap.css
+-rw-rw-rw-   0        0        0   104156 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap.css.map
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.222307 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/forms/
+-rw-rw-rw-   0        0        0     2480 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/forms/_floating-labels.scss
+-rw-rw-rw-   0        0        0     4833 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/forms/_form-check.scss
+-rw-rw-rw-   0        0        0     5868 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/forms/_form-control.scss
+-rw-rw-rw-   0        0        0     2796 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/forms/_form-range.scss
+-rw-rw-rw-   0        0        0     2603 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/forms/_form-select.scss
+-rw-rw-rw-   0        0        0      219 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/forms/_form-text.scss
+-rw-rw-rw-   0        0        0     3896 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/forms/_input-group.scss
+-rw-rw-rw-   0        0        0     1142 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/forms/_labels.scss
+-rw-rw-rw-   0        0        0      478 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/forms/_validation.scss
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.240361 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/helpers/
+-rw-rw-rw-   0        0        0       37 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/helpers/_clearfix.scss
+-rw-rw-rw-   0        0        0      454 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/helpers/_color-bg.scss
+-rw-rw-rw-   0        0        0      426 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/helpers/_colored-links.scss
+-rw-rw-rw-   0        0        0      621 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/helpers/_position.scss
+-rw-rw-rw-   0        0        0      399 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/helpers/_ratio.scss
+-rw-rw-rw-   0        0        0      245 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/helpers/_stacks.scss
+-rw-rw-rw-   0        0        0      223 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/helpers/_stretched-link.scss
+-rw-rw-rw-   0        0        0       73 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/helpers/_text-truncation.scss
+-rw-rw-rw-   0        0        0      136 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/helpers/_visually-hidden.scss
+-rw-rw-rw-   0        0        0      147 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/helpers/_vr.scss
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.302108 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/
+-rw-rw-rw-   0        0        0      525 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_alert.scss
+-rw-rw-rw-   0        0        0      328 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_backdrop.scss
+-rw-rw-rw-   0        0        0      230 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_banner.scss
+-rw-rw-rw-   0        0        0     2031 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_border-radius.scss
+-rw-rw-rw-   0        0        0      398 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_box-shadow.scss
+-rw-rw-rw-   0        0        0     4580 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_breakpoints.scss
+-rw-rw-rw-   0        0        0     3220 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_buttons.scss
+-rw-rw-rw-   0        0        0     1587 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_caret.scss
+-rw-rw-rw-   0        0        0      147 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_clearfix.scss
+-rw-rw-rw-   0        0        0      447 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_color-mode.scss
+-rw-rw-rw-   0        0        0      167 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_color-scheme.scss
+-rw-rw-rw-   0        0        0      410 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_container.scss
+-rw-rw-rw-   0        0        0      613 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_deprecate.scss
+-rw-rw-rw-   0        0        0     4164 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_forms.scss
+-rw-rw-rw-   0        0        0     1956 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_gradients.scss
+-rw-rw-rw-   0        0        0     4726 2023-04-29 09:52:37.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_grid.scss
+-rw-rw-rw-   0        0        0      395 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_image.scss
+-rw-rw-rw-   0        0        0      582 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_list-group.scss
+-rw-rw-rw-   0        0        0      168 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_lists.scss
+-rw-rw-rw-   0        0        0      387 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_pagination.scss
+-rw-rw-rw-   0        0        0      495 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_reset-text.scss
+-rw-rw-rw-   0        0        0      202 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_resize.scss
+-rw-rw-rw-   0        0        0     1101 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_table-variants.scss
+-rw-rw-rw-   0        0        0      168 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_text-truncate.scss
+-rw-rw-rw-   0        0        0      661 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_transition.scss
+-rw-rw-rw-   0        0        0     3380 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_utilities.scss
+-rw-rw-rw-   0        0        0     1012 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_visually-hidden.scss
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.303108 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/utilities/
+-rw-rw-rw-   0        0        0     1737 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/utilities/_api.scss
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.304107 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/vendor/
+-rw-rw-rw-   0        0        0    10029 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/vendor/_rfs.scss
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.313652 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/
+-rw-rw-rw-   0        0        0    11945 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/AUTHORS.txt
+-rw-rw-rw-   0        0        0     1095 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/LICENSE.txt
+-rw-rw-rw-   0        0        0     1997 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/README.md
+-rw-rw-rw-   0        0        0      190 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/bower.json
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.325185 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/dist/
+-rw-rw-rw-   0        0        0     9165 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/dist/core.js
+-rw-rw-rw-   0        0        0   279869 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/dist/jquery.js
+-rw-rw-rw-   0        0        0    88151 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/dist/jquery.min.js
+-rw-rw-rw-   0        0        0   136403 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/dist/jquery.min.map
+-rw-rw-rw-   0        0        0   226527 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/dist/jquery.slim.js
+-rw-rw-rw-   0        0        0    71043 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/dist/jquery.slim.min.js
+-rw-rw-rw-   0        0        0   108763 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/dist/jquery.slim.min.map
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.235640 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/external/
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.327203 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/external/sizzle/
+-rw-rw-rw-   0        0        0     1605 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/external/sizzle/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.333727 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/external/sizzle/dist/
+-rw-rw-rw-   0        0        0    65675 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/external/sizzle/dist/sizzle.js
+-rw-rw-rw-   0        0        0    19841 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/external/sizzle/dist/sizzle.min.js
+-rw-rw-rw-   0        0        0    30740 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/external/sizzle/dist/sizzle.min.map
+-rw-rw-rw-   0        0        0     2870 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/package.json
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.371204 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/
+-rw-rw-rw-   0        0        0       96 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/.eslintrc.json
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.380722 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/ajax/
+-rw-rw-rw-   0        0        0     2748 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/ajax/jsonp.js
+-rw-rw-rw-   0        0        0     1904 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/ajax/load.js
+-rw-rw-rw-   0        0        0      559 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/ajax/parseXML.js
+-rw-rw-rw-   0        0        0     1637 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/ajax/script.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.385732 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/ajax/var/
+-rw-rw-rw-   0        0        0       67 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/ajax/var/location.js
+-rw-rw-rw-   0        0        0       62 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/ajax/var/nonce.js
+-rw-rw-rw-   0        0        0       60 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/ajax/var/rquery.js
+-rw-rw-rw-   0        0        0     4339 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/ajax/xhr.js
+-rw-rw-rw-   0        0        0    22463 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/ajax.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.392254 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/attributes/
+-rw-rw-rw-   0        0        0     3271 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/attributes/attr.js
+-rw-rw-rw-   0        0        0     4447 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/attributes/classes.js
+-rw-rw-rw-   0        0        0     3004 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/attributes/prop.js
+-rw-rw-rw-   0        0        0      786 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/attributes/support.js
+-rw-rw-rw-   0        0        0     4249 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/attributes/val.js
+-rw-rw-rw-   0        0        0      217 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/attributes.js
+-rw-rw-rw-   0        0        0     5552 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/callbacks.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.415250 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/
+-rw-rw-rw-   0        0        0     1160 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/DOMEval.js
+-rw-rw-rw-   0        0        0     1311 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/access.js
+-rw-rw-rw-   0        0        0      545 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/camelCase.js
+-rw-rw-rw-   0        0        0     3337 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/init.js
+-rw-rw-rw-   0        0        0      566 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/isAttached.js
+-rw-rw-rw-   0        0        0      178 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/nodeName.js
+-rw-rw-rw-   0        0        0     1604 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/parseHTML.js
+-rw-rw-rw-   0        0        0     2264 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/ready-no-deferred.js
+-rw-rw-rw-   0        0        0     2097 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/ready.js
+-rw-rw-rw-   0        0        0      168 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/readyException.js
+-rw-rw-rw-   0        0        0      362 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/stripAndCollapse.js
+-rw-rw-rw-   0        0        0      631 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/support.js
+-rw-rw-rw-   0        0        0      379 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/toType.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.417250 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/var/
+-rw-rw-rw-   0        0        0      244 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/var/rsingleTag.js
+-rw-rw-rw-   0        0        0     9165 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.428779 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css/
+-rw-rw-rw-   0        0        0      530 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css/addGetHookIf.js
+-rw-rw-rw-   0        0        0     2002 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css/adjustCSS.js
+-rw-rw-rw-   0        0        0     1656 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css/curCSS.js
+-rw-rw-rw-   0        0        0      849 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css/finalPropName.js
+-rw-rw-rw-   0        0        0      317 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css/hiddenVisibleSelectors.js
+-rw-rw-rw-   0        0        0     2304 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css/showHide.js
+-rw-rw-rw-   0        0        0     3070 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css/support.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.447858 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css/var/
+-rw-rw-rw-   0        0        0       88 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css/var/cssExpand.js
+-rw-rw-rw-   0        0        0      401 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css/var/getStyles.js
+-rw-rw-rw-   0        0        0     1284 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css/var/isHiddenWithinTree.js
+-rw-rw-rw-   0        0        0      123 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css/var/rboxStyle.js
+-rw-rw-rw-   0        0        0      131 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css/var/rnumnonpx.js
+-rw-rw-rw-   0        0        0      520 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css/var/swap.js
+-rw-rw-rw-   0        0        0    13828 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.450363 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/data/
+-rw-rw-rw-   0        0        0     3952 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/data/Data.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.458896 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/data/var/
+-rw-rw-rw-   0        0        0      318 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/data/var/acceptData.js
+-rw-rw-rw-   0        0        0       84 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/data/var/dataPriv.js
+-rw-rw-rw-   0        0        0       84 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/data/var/dataUser.js
+-rw-rw-rw-   0        0        0     4321 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/data.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.462429 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/deferred/
+-rw-rw-rw-   0        0        0      640 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/deferred/exceptionHook.js
+-rw-rw-rw-   0        0        0    10997 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/deferred.js
+-rw-rw-rw-   0        0        0     2467 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/deprecated.js
+-rw-rw-rw-   0        0        0     1751 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/dimensions.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.467447 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/effects/
+-rw-rw-rw-   0        0        0     3292 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/effects/Tween.js
+-rw-rw-rw-   0        0        0      244 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/effects/animatedSelector.js
+-rw-rw-rw-   0        0        0    17455 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/effects.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.476985 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/event/
+-rw-rw-rw-   0        0        0      346 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/event/ajax.js
+-rw-rw-rw-   0        0        0      649 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/event/alias.js
+-rw-rw-rw-   0        0        0     1512 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/event/focusin.js
+-rw-rw-rw-   0        0        0      133 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/event/support.js
+-rw-rw-rw-   0        0        0     5407 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/event/trigger.js
+-rw-rw-rw-   0        0        0    24235 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/event.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.481499 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/exports/
+-rw-rw-rw-   0        0        0     1024 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/exports/amd.js
+-rw-rw-rw-   0        0        0      608 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/exports/global.js
+-rw-rw-rw-   0        0        0      622 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/jquery.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.496031 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/manipulation/
+-rw-rw-rw-   0        0        0      676 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/manipulation/_evalUrl.js
+-rw-rw-rw-   0        0        0     2486 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/manipulation/buildFragment.js
+-rw-rw-rw-   0        0        0      650 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/manipulation/getAll.js
+-rw-rw-rw-   0        0        0      381 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/manipulation/setGlobalEval.js
+-rw-rw-rw-   0        0        0     1034 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/manipulation/support.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.500030 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/manipulation/var/
+-rw-rw-rw-   0        0        0       92 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/manipulation/var/rscriptType.js
+-rw-rw-rw-   0        0        0      304 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/manipulation/var/rtagName.js
+-rw-rw-rw-   0        0        0      798 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/manipulation/wrapMap.js
+-rw-rw-rw-   0        0        0    12643 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/manipulation.js
+-rw-rw-rw-   0        0        0     6868 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/offset.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.501366 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/queue/
+-rw-rw-rw-   0        0        0      636 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/queue/delay.js
+-rw-rw-rw-   0        0        0     3091 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/queue.js
+-rw-rw-rw-   0        0        0     6394 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/selector-native.js
+-rw-rw-rw-   0        0        0      411 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/selector-sizzle.js
+-rw-rw-rw-   0        0        0       66 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/selector.js
+-rw-rw-rw-   0        0        0     3241 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/serialize.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.503368 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/traversing/
+-rw-rw-rw-   0        0        0     2352 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/traversing/findFilter.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.507366 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/traversing/var/
+-rw-rw-rw-   0        0        0      371 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/traversing/var/dir.js
+-rw-rw-rw-   0        0        0      128 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/traversing/var/rneedsContext.js
+-rw-rw-rw-   0        0        0      218 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/traversing/var/siblings.js
+-rw-rw-rw-   0        0        0     4500 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/traversing.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.541171 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/var/
+-rw-rw-rw-   0        0        0      110 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/var/ObjectFunctionString.js
+-rw-rw-rw-   0        0        0       54 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/var/arr.js
+-rw-rw-rw-   0        0        0       82 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/var/class2type.js
+-rw-rw-rw-   0        0        0       81 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/var/concat.js
+-rw-rw-rw-   0        0        0       67 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/var/document.js
+-rw-rw-rw-   0        0        0      105 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/var/documentElement.js
+-rw-rw-rw-   0        0        0       92 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/var/fnToString.js
+-rw-rw-rw-   0        0        0       73 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/var/getProto.js
+-rw-rw-rw-   0        0        0      110 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/var/hasOwn.js
+-rw-rw-rw-   0        0        0       82 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/var/indexOf.js
+-rw-rw-rw-   0        0        0      428 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/var/isFunction.js
+-rw-rw-rw-   0        0        0      126 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/var/isWindow.js
+-rw-rw-rw-   0        0        0      100 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/var/pnum.js
+-rw-rw-rw-   0        0        0       79 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/var/push.js
+-rw-rw-rw-   0        0        0       79 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/var/rcheckableType.js
+-rw-rw-rw-   0        0        0      136 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/var/rcssNum.js
+-rw-rw-rw-   0        0        0      202 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/var/rnothtmlwhite.js
+-rw-rw-rw-   0        0        0       80 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/var/slice.js
+-rw-rw-rw-   0        0        0      117 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/var/support.js
+-rw-rw-rw-   0        0        0      104 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/var/toString.js
+-rw-rw-rw-   0        0        0     1477 2023-04-29 09:52:38.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/wrap.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.547169 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/
+-rw-rw-rw-   0        0        0     1080 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/LICENSE
+-rw-rw-rw-   0        0        0    12252 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/README.md
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.565542 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/dist/
+-rw-rw-rw-   0        0        0    32771 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/dist/simplebar-core.esm.js
+-rw-rw-rw-   0        0        0    64425 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/dist/simplebar-core.esm.js.map
+-rw-rw-rw-   0        0        0     3890 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/dist/simplebar.css
+-rw-rw-rw-   0        0        0     1323 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/dist/simplebar.d.ts
+-rw-rw-rw-   0        0        0    36530 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/dist/simplebar.esm.js
+-rw-rw-rw-   0        0        0    71785 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/dist/simplebar.esm.js.map
+-rw-rw-rw-   0        0        0   171895 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/dist/simplebar.js
+-rw-rw-rw-   0        0        0     2937 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/dist/simplebar.min.css
+-rw-rw-rw-   0        0        0    59030 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/dist/simplebar.min.js
+-rw-rw-rw-   0        0        0     4604 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/dist/simplebar.umd.js
+-rw-rw-rw-   0        0        0     1719 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/package.json
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.574028 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/src/
+-rw-rw-rw-   0        0        0     1104 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/src/helpers.js
+-rw-rw-rw-   0        0        0     3363 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/src/index.js
+-rw-rw-rw-   0        0        0      953 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/src/scrollbar-width.js
+-rw-rw-rw-   0        0        0     3890 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/src/simplebar.css
+-rw-rw-rw-   0        0        0    29802 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/src/simplebar.js
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.579031 django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.582355 django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/component/
+-rw-rw-rw-   0        0        0      344 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/component/_card.scss
+-rw-rw-rw-   0        0        0      489 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/component/_reboot.scss
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.587358 django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/layouts/
+-rw-rw-rw-   0        0        0     3362 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/layouts/_header.scss
+-rw-rw-rw-   0        0        0     1833 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/layouts/_layouts.scss
+-rw-rw-rw-   0        0        0     2210 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/layouts/_sidebar.scss
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.588349 django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/pages/
+-rw-rw-rw-   0        0        0      842 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/pages/_dashboard1.scss
+-rw-rw-rw-   0        0        0    23293 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/prepros.config
+-rw-rw-rw-   0        0        0      844 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/styles.scss
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.591875 django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/utilities/
+-rw-rw-rw-   0        0        0      487 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/utilities/_background.scss
+-rw-rw-rw-   0        0        0      236 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/utilities/_icon-size.scss
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.596872 django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/variables/
+-rw-rw-rw-   0        0        0      964 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/variables/_theme-variables.scss
+-rw-rw-rw-   0        0        0     5275 2023-04-29 09:52:39.000000 django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/variables/_variables.scss
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.599873 django-admin-modernize-1.0.3/admin_modernize/templates/
+-rw-rw-rw-   0        0        0        0 2022-09-27 05:30:21.000000 django-admin-modernize-1.0.3/admin_modernize/templates/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.612953 django-admin-modernize-1.0.3/admin_modernize/templates/accounts/
+-rw-rw-rw-   0        0        0     2799 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/accounts/login.html
+-rw-rw-rw-   0        0        0     1889 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/accounts/password_change.html
+-rw-rw-rw-   0        0        0     1116 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/accounts/password_change_done.html
+-rw-rw-rw-   0        0        0     2125 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/accounts/password_reset.html
+-rw-rw-rw-   0        0        0     1252 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/accounts/password_reset_complete.html
+-rw-rw-rw-   0        0        0     2120 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/accounts/password_reset_confirm.html
+-rw-rw-rw-   0        0        0     1398 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/accounts/password_reset_done.html
+-rw-rw-rw-   0        0        0     1988 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/accounts/register.html
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.639010 django-admin-modernize-1.0.3/admin_modernize/templates/admin/
+-rw-rw-rw-   0        0        0     1606 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/admin/actions.html
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:51.264723 django-admin-modernize-1.0.3/admin_modernize/templates/admin/auth/
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.641539 django-admin-modernize-1.0.3/admin_modernize/templates/admin/auth/user/
+-rw-rw-rw-   0        0        0      334 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/admin/auth/user/add_form.html
+-rw-rw-rw-   0        0        0     5386 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/admin/auth/user/change_password.html
+-rw-rw-rw-   0        0        0     6178 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/admin/change_form.html
+-rw-rw-rw-   0        0        0      556 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/admin/change_form_object_tools.html
+-rw-rw-rw-   0        0        0     5638 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/admin/change_list.html
+-rw-rw-rw-   0        0        0      470 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/admin/change_list_object_tools.html
+-rw-rw-rw-   0        0        0     3004 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/admin/change_list_results.html
+-rw-rw-rw-   0        0        0     7167 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/admin/delete_confirmation.html
+-rw-rw-rw-   0        0        0     7168 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/admin/delete_selected_confirmation.html
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.645565 django-admin-modernize-1.0.3/admin_modernize/templates/admin/edit_inline/
+-rw-rw-rw-   0        0        0     3893 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/admin/edit_inline/stacked.html
+-rw-rw-rw-   0        0        0     7834 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/admin/edit_inline/tabular.html
+-rw-rw-rw-   0        0        0      506 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/admin/filter.html
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.648553 django-admin-modernize-1.0.3/admin_modernize/templates/admin/includes/
+-rw-rw-rw-   0        0        0     2572 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/admin/includes/fieldset.html
+-rw-rw-rw-   0        0        0      348 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/admin/includes/object_delete_summary.html
+-rw-rw-rw-   0        0        0    19871 2023-05-01 07:41:34.000000 django-admin-modernize-1.0.3/admin_modernize/templates/admin/index.html
+-rw-rw-rw-   0        0        0     2590 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/admin/invalid_setup.html
+-rw-rw-rw-   0        0        0     3378 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/admin/login.html
+-rw-rw-rw-   0        0        0     3922 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/admin/object_history.html
+-rw-rw-rw-   0        0        0     2184 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/admin/pagination.html
+-rw-rw-rw-   0        0        0     2502 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/admin/search_form.html
+-rw-rw-rw-   0        0        0     1481 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/admin/submit_line.html
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.655094 django-admin-modernize-1.0.3/admin_modernize/templates/includes/
+-rw-rw-rw-   0        0        0      401 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/includes/head.html
+-rw-rw-rw-   0        0        0     3745 2023-05-01 07:44:07.000000 django-admin-modernize-1.0.3/admin_modernize/templates/includes/navigation.html
+-rw-rw-rw-   0        0        0      548 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/includes/scripts.html
+-rw-rw-rw-   0        0        0     6444 2023-05-01 07:57:23.000000 django-admin-modernize-1.0.3/admin_modernize/templates/includes/sidebar.html
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.660051 django-admin-modernize-1.0.3/admin_modernize/templates/layouts/
+-rw-rw-rw-   0        0        0     1130 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/layouts/auth_base.html
+-rw-rw-rw-   0        0        0      842 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/layouts/base.html
+-rw-rw-rw-   0        0        0     1037 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/layouts/base_logout.html
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.676621 django-admin-modernize-1.0.3/admin_modernize/templates/pages/
+-rw-rw-rw-   0        0        0      481 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/pages/icon-tabler.html
+-rw-rw-rw-   0        0        0    19821 2023-05-01 07:42:03.000000 django-admin-modernize-1.0.3/admin_modernize/templates/pages/index.html
+-rw-rw-rw-   0        0        0      343 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/pages/sample-page.html
+-rw-rw-rw-   0        0        0     2710 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/pages/sign-in.html
+-rw-rw-rw-   0        0        0     2404 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/pages/sign-up.html
+-rw-rw-rw-   0        0        0     1705 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/pages/ui-alerts.html
+-rw-rw-rw-   0        0        0     2087 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/pages/ui-buttons.html
+-rw-rw-rw-   0        0        0     2218 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/pages/ui-card.html
+-rw-rw-rw-   0        0        0     2766 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/pages/ui-forms.html
+-rw-rw-rw-   0        0        0     1563 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/pages/ui-typography.html
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.683174 django-admin-modernize-1.0.3/admin_modernize/templates/registration/
+-rw-rw-rw-   0        0        0     1527 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/registration/logged_out.html
+-rw-rw-rw-   0        0        0     2786 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/registration/password_change_done.html
+-rw-rw-rw-   0        0        0     4185 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templates/registration/password_change_form.html
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.685170 django-admin-modernize-1.0.3/admin_modernize/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     2476 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/templatetags/admin_modernize.py
+-rw-rw-rw-   0        0        0       63 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/tests.py
+-rw-rw-rw-   0        0        0     1789 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/urls.py
+-rw-rw-rw-   0        0        0    16503 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/utils.py
+-rw-rw-rw-   0        0        0     2071 2023-05-01 07:23:04.000000 django-admin-modernize-1.0.3/admin_modernize/views.py
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.693696 django-admin-modernize-1.0.3/django_admin_modernize.egg-info/
+-rw-rw-rw-   0        0        0     6248 2023-05-01 07:58:50.000000 django-admin-modernize-1.0.3/django_admin_modernize.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    47647 2023-05-01 07:58:50.000000 django-admin-modernize-1.0.3/django_admin_modernize.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 07:58:50.000000 django-admin-modernize-1.0.3/django_admin_modernize.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-01 07:50:54.000000 django-admin-modernize-1.0.3/django_admin_modernize.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2023-05-01 07:58:50.000000 django-admin-modernize-1.0.3/django_admin_modernize.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-01 07:58:52.695703 django-admin-modernize-1.0.3/docs/
+-rw-rw-rw-   0        0        0       13 2022-09-27 05:30:21.000000 django-admin-modernize-1.0.3/docs/blank.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 07:58:52.698696 django-admin-modernize-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1351 2023-05-01 07:57:47.000000 django-admin-modernize-1.0.3/setup.py
```

### Comparing `django-admin-modernize-1.0.2/LICENSE.md` & `django-admin-modernize-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/PKG-INFO` & `django-admin-modernize-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-modernize
-Version: 1.0.2
+Version: 1.0.3
 Summary: Modern template for Django admin interface
 Home-page: https://github.com/app-generator/django-modernize
 Author: AppSeed.us
 Author-email: support@appseed.us
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

### Comparing `django-admin-modernize-1.0.2/README.md` & `django-admin-modernize-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/forms.py` & `django-admin-modernize-1.0.3/admin_modernize/forms.py`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/css/forms.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/css/forms.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/css/icons/tabler-icons/fonts/tabler-icons.eot` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/css/icons/tabler-icons/fonts/tabler-icons.eot`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/css/icons/tabler-icons/fonts/tabler-icons.svg` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/css/icons/tabler-icons/fonts/tabler-icons.svg`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/css/icons/tabler-icons/fonts/tabler-icons.ttf` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/css/icons/tabler-icons/fonts/tabler-icons.ttf`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/css/icons/tabler-icons/fonts/tabler-icons.woff` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/css/icons/tabler-icons/fonts/tabler-icons.woff`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/css/icons/tabler-icons/fonts/tabler-icons.woff2` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/css/icons/tabler-icons/fonts/tabler-icons.woff2`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/css/icons/tabler-icons/tabler-icons.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/css/icons/tabler-icons/tabler-icons.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/css/plugins/animate.min.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/css/plugins/animate.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/css/plugins/bootstrap.min.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/css/plugins/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/css/style-preset.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/css/style-preset.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/css/styles.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/css/styles.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/css/styles.min.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/css/styles.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/css/widgets.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/css/widgets.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/images/backgrounds/rocket.png` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/images/backgrounds/rocket.png`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/images/logos/dark-logo.svg` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/images/logos/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/images/logos/favicon.png` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/images/logos/favicon.png`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/images/products/s1.jpg` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/images/products/s1.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/images/products/s11.jpg` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/images/products/s11.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/images/products/s4.jpg` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/images/products/s4.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/images/products/s5.jpg` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/images/products/s5.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/images/products/s7.jpg` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/images/products/s7.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/images/profile/user-1.jpg` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/images/profile/user-1.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/js/app.min.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/js/app.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/js/dashboard.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/js/dashboard.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/js/sidebarmenu.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/js/sidebarmenu.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/LICENSE` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/README.md` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/README.md`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.amd.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.amd.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.common.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.common.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.esm.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.esm.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.min.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/apexcharts.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/ar.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/ar.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/ca.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/ca.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/cs.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/cs.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/de.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/de.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/el.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/el.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/en.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/en.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/es.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/es.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/et.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/et.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/fa.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/fa.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/fi.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/fi.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/fr.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/fr.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/he.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/he.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/hi.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/hi.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/hr.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/hr.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/hu.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/hu.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/hy.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/hy.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/id.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/id.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/it.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/it.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/ja.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/ja.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/ka.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/ka.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/ko.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/ko.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/lt.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/lt.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/lv.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/lv.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/nb.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/nb.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/nl.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/nl.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/pl.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/pl.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/pt-br.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/pt-br.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/pt.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/pt.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/rs.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/rs.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/ru.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/ru.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/se.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/se.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/sk.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/sk.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/sl.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/sl.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/sq.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/sq.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/th.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/th.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/tr.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/tr.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/ua.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/ua.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/zh-cn.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/zh-cn.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/dist/locales/zh-tw.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/dist/locales/zh-tw.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/package.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/package.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/apexcharts.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/apexcharts.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/assets/apexcharts.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/assets/apexcharts.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-pan-hand.svg` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-pan-hand.svg`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-zoom-out.svg` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/assets/ico-zoom-out.svg`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/Bar.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/Bar.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/BarStacked.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/BarStacked.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/BoxCandleStick.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/BoxCandleStick.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/HeatMap.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/HeatMap.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/Line.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/Line.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/Pie.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/Pie.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/Radar.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/Radar.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/Radial.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/Radial.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/RangeBar.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/RangeBar.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/Scatter.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/Scatter.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/Treemap.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/Treemap.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/common/bar/DataLabels.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/common/bar/DataLabels.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/common/bar/Helpers.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/common/bar/Helpers.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/common/circle/Helpers.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/common/circle/Helpers.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/common/line/Helpers.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/common/line/Helpers.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/charts/common/treemap/Helpers.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/charts/common/treemap/Helpers.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/libs/Treemap-squared.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/libs/Treemap-squared.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/ar.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/ar.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/ca.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/ca.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/cs.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/cs.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/de.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/de.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/el.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/el.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/en.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/en.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/es.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/es.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/et.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/et.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/fa.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/fa.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/fi.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/fi.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/fr.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/fr.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/he.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/he.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/hi.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/hi.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/hr.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/hr.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/hu.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/hu.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/hy.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/hy.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/id.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/id.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/it.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/it.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/ja.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/ja.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/ka.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/ka.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/ko.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/ko.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/lt.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/lt.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/lv.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/lv.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/nb.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/nb.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/nl.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/nl.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/pl.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/pl.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/pt-br.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/pt-br.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/pt.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/pt.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/rs.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/rs.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/ru.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/ru.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/se.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/se.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/sk.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/sk.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/sl.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/sl.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/sq.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/sq.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/th.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/th.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/tr.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/tr.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/ua.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/ua.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/zh-cn.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/zh-cn.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/locales/zh-tw.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/locales/zh-tw.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Animations.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Animations.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Core.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Core.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/CoreUtils.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/CoreUtils.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Crosshairs.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Crosshairs.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Data.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Data.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/DataLabels.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/DataLabels.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Events.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Events.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Exports.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Exports.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Fill.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Fill.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Filters.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Filters.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Formatters.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Formatters.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Graphics.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Graphics.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Markers.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Markers.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Range.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Range.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Responsive.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Responsive.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Scales.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Scales.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Series.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Series.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Theme.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Theme.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/TimeScale.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/TimeScale.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/TitleSubtitle.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/TitleSubtitle.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/Toolbar.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/Toolbar.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/ZoomPanSelection.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/ZoomPanSelection.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/annotations/Annotations.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/annotations/Annotations.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/annotations/Helpers.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/annotations/Helpers.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/annotations/PointsAnnotations.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/annotations/PointsAnnotations.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/annotations/XAxisAnnotations.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/annotations/XAxisAnnotations.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/annotations/YAxisAnnotations.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/annotations/YAxisAnnotations.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/axes/Axes.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/axes/Axes.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/axes/AxesUtils.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/axes/AxesUtils.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/axes/Grid.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/axes/Grid.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/axes/XAxis.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/axes/XAxis.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/axes/YAxis.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/axes/YAxis.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/dimensions/Dimensions.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/dimensions/Dimensions.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/dimensions/Grid.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/dimensions/Grid.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/dimensions/Helpers.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/dimensions/Helpers.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/dimensions/XAxis.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/dimensions/XAxis.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/dimensions/YAxis.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/dimensions/YAxis.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/helpers/Destroy.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/helpers/Destroy.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/helpers/InitCtxVariables.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/helpers/InitCtxVariables.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/helpers/Localization.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/helpers/Localization.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/helpers/UpdateHelpers.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/helpers/UpdateHelpers.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/legend/Helpers.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/legend/Helpers.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/legend/Legend.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/legend/Legend.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/settings/Config.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/settings/Config.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/settings/Defaults.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/settings/Defaults.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/settings/Globals.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/settings/Globals.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/settings/Options.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/settings/Options.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/AxesTooltip.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/AxesTooltip.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Intersect.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Intersect.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Labels.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Labels.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Marker.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Marker.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Position.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Position.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/README.md` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/README.md`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Tooltip.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Tooltip.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Utils.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/modules/tooltip/Utils.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/svgjs/svg.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/svgjs/svg.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/utils/DateTime.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/utils/DateTime.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/utils/Resize.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/utils/Resize.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/src/utils/Utils.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/src/utils/Utils.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/apexcharts/types/apexcharts.d.ts` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/apexcharts/types/apexcharts.d.ts`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/LICENSE` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/README.md` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/README.md`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.min.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.min.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.rtl.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.rtl.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.rtl.min.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.min.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.min.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.rtl.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.rtl.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.rtl.min.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.min.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.min.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.rtl.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.rtl.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.rtl.min.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.min.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.min.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.rtl.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.rtl.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.rtl.min.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.rtl.min.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.bundle.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.bundle.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.bundle.min.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.bundle.min.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.esm.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.esm.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.esm.min.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.esm.min.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.min.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.min.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/dist/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/alert.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/alert.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/alert.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/alert.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/base-component.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/base-component.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/base-component.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/base-component.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/button.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/button.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/button.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/button.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/carousel.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/carousel.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/carousel.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/carousel.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/collapse.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/collapse.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/collapse.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/collapse.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/data.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/data.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/data.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/data.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/event-handler.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/event-handler.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/event-handler.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/event-handler.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/manipulator.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/manipulator.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/manipulator.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/manipulator.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/selector-engine.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/selector-engine.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/selector-engine.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/dom/selector-engine.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/dropdown.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/dropdown.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/dropdown.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/dropdown.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/modal.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/modal.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/modal.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/modal.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/offcanvas.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/offcanvas.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/offcanvas.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/offcanvas.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/popover.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/popover.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/popover.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/popover.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/scrollspy.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/scrollspy.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/scrollspy.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/scrollspy.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/tab.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/tab.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/tab.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/tab.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/toast.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/toast.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/toast.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/toast.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/tooltip.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/tooltip.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/tooltip.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/tooltip.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/backdrop.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/backdrop.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/backdrop.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/backdrop.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/component-functions.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/component-functions.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/component-functions.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/component-functions.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/config.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/config.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/config.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/config.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/focustrap.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/focustrap.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/focustrap.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/focustrap.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/index.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/index.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/index.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/index.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/sanitizer.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/sanitizer.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/sanitizer.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/sanitizer.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/scrollbar.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/scrollbar.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/scrollbar.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/scrollbar.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/swipe.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/swipe.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/swipe.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/swipe.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/template-factory.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/template-factory.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/dist/util/template-factory.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/dist/util/template-factory.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/index.esm.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/index.esm.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/index.umd.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/index.umd.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/alert.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/alert.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/base-component.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/base-component.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/button.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/button.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/carousel.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/carousel.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/collapse.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/collapse.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/dom/data.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/dom/data.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/dom/event-handler.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/dom/event-handler.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/dom/manipulator.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/dom/manipulator.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/dom/selector-engine.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/dom/selector-engine.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/dropdown.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/dropdown.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/modal.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/modal.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/offcanvas.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/offcanvas.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/popover.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/popover.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/scrollspy.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/scrollspy.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/tab.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/tab.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/toast.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/toast.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/tooltip.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/tooltip.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/util/backdrop.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/util/backdrop.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/util/component-functions.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/util/component-functions.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/util/config.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/util/config.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/util/focustrap.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/util/focustrap.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/util/index.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/util/index.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/util/sanitizer.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/util/sanitizer.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/util/scrollbar.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/util/scrollbar.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/util/swipe.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/util/swipe.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/src/util/template-factory.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/src/util/template-factory.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/README.md` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/README.md`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/browsers.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/browsers.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/helpers/fixture.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/helpers/fixture.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/integration/index.html` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/integration/index.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/integration/rollup.bundle.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/integration/rollup.bundle.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/karma.conf.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/karma.conf.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/alert.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/alert.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/base-component.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/base-component.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/button.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/button.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/carousel.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/carousel.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/collapse.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/collapse.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/dom/data.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/dom/data.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/dom/event-handler.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/dom/event-handler.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/dom/manipulator.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/dom/manipulator.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/dom/selector-engine.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/dom/selector-engine.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/dropdown.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/dropdown.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/jquery.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/jquery.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/modal.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/modal.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/offcanvas.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/offcanvas.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/popover.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/popover.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/scrollspy.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/scrollspy.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/tab.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/tab.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/toast.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/toast.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/tooltip.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/tooltip.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/backdrop.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/backdrop.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/component-functions.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/component-functions.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/config.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/config.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/focustrap.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/focustrap.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/index.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/index.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/sanitizer.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/sanitizer.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/scrollbar.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/scrollbar.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/swipe.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/swipe.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/template-factory.spec.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/unit/util/template-factory.spec.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/alert.html` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/alert.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/button.html` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/button.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/carousel.html` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/carousel.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/collapse.html` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/collapse.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/dropdown.html` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/dropdown.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/modal.html` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/modal.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/popover.html` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/popover.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/scrollspy.html` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/scrollspy.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/tab.html` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/tab.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/toast.html` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/toast.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/tooltip.html` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/js/tests/visual/tooltip.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/package.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/package.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_accordion.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_accordion.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_alert.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_alert.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_badge.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_badge.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_breadcrumb.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_button-group.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_button-group.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_buttons.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_buttons.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_card.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_card.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_carousel.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_carousel.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_close.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_close.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_containers.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_containers.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_dropdown.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_functions.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_functions.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_grid.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_grid.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_images.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_images.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_list-group.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_list-group.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_maps.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_maps.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_mixins.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_modal.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_modal.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_nav.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_navbar.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_navbar.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_offcanvas.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_offcanvas.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_pagination.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_pagination.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_placeholders.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_placeholders.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_popover.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_popover.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_progress.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_progress.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_reboot.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_reboot.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_root.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_root.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_spinners.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_spinners.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_tables.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_tables.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_toasts.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_toasts.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_tooltip.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_type.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_type.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_utilities.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_utilities.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_variables-dark.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_variables-dark.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/_variables.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-grid.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-grid.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-grid.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-reboot.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-reboot.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-utilities.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-utilities.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-grid.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-grid.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-reboot.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-reboot.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-utilities.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-utilities.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap.css.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/forms/_floating-labels.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/forms/_form-check.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/forms/_form-control.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/forms/_form-range.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/forms/_form-select.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/forms/_input-group.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/forms/_labels.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/helpers/_position.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/helpers/_position.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_alert.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_alert.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_border-radius.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_breakpoints.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_buttons.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_caret.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_deprecate.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_forms.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_gradients.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_grid.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_list-group.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_list-group.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_table-variants.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_transition.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_utilities.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_visually-hidden.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/utilities/_api.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/bootstrap/scss/vendor/_rfs.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/bootstrap/scss/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/AUTHORS.txt` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/LICENSE.txt` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/README.md` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/README.md`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/dist/core.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/dist/core.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/dist/jquery.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/dist/jquery.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/dist/jquery.min.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/dist/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/dist/jquery.min.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/dist/jquery.min.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/dist/jquery.slim.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/dist/jquery.slim.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/dist/jquery.slim.min.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/dist/jquery.slim.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/dist/jquery.slim.min.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/dist/jquery.slim.min.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/external/sizzle/LICENSE.txt` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/external/sizzle/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/external/sizzle/dist/sizzle.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/external/sizzle/dist/sizzle.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/external/sizzle/dist/sizzle.min.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/external/sizzle/dist/sizzle.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/external/sizzle/dist/sizzle.min.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/external/sizzle/dist/sizzle.min.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/package.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/package.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/ajax/jsonp.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/ajax/jsonp.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/ajax/load.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/ajax/load.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/ajax/parseXML.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/ajax/parseXML.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/ajax/script.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/ajax/script.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/ajax/xhr.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/ajax/xhr.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/ajax.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/ajax.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/attributes/attr.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/attributes/attr.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/attributes/classes.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/attributes/classes.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/attributes/prop.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/attributes/prop.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/attributes/support.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/attributes/support.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/attributes/val.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/attributes/val.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/callbacks.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/callbacks.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/DOMEval.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/DOMEval.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/access.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/access.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/camelCase.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/camelCase.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/init.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/init.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/isAttached.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/isAttached.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/parseHTML.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/parseHTML.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/ready-no-deferred.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/ready-no-deferred.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/ready.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/ready.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core/support.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core/support.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/core.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/core.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css/addGetHookIf.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css/addGetHookIf.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css/adjustCSS.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css/adjustCSS.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css/curCSS.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css/curCSS.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css/finalPropName.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css/finalPropName.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css/showHide.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css/showHide.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css/support.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css/support.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css/var/isHiddenWithinTree.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css/var/isHiddenWithinTree.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css/var/swap.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css/var/swap.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/css.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/css.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/data/Data.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/data/Data.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/data.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/data.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/deferred/exceptionHook.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/deferred/exceptionHook.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/deferred.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/deferred.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/deprecated.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/deprecated.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/dimensions.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/dimensions.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/effects/Tween.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/effects/Tween.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/effects.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/effects.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/event/alias.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/event/alias.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/event/focusin.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/event/focusin.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/event/trigger.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/event/trigger.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/event.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/event.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/exports/amd.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/exports/amd.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/exports/global.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/exports/global.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/jquery.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/jquery.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/manipulation/_evalUrl.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/manipulation/_evalUrl.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/manipulation/buildFragment.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/manipulation/buildFragment.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/manipulation/getAll.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/manipulation/getAll.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/manipulation/support.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/manipulation/support.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/manipulation/wrapMap.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/manipulation/wrapMap.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/manipulation.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/manipulation.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/offset.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/offset.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/queue/delay.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/queue/delay.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/queue.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/queue.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/selector-native.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/selector-native.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/serialize.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/serialize.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/traversing/findFilter.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/traversing/findFilter.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/traversing.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/traversing.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/jquery/src/wrap.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/jquery/src/wrap.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/LICENSE` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/README.md` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/README.md`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/dist/simplebar-core.esm.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/dist/simplebar-core.esm.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/dist/simplebar-core.esm.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/dist/simplebar-core.esm.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/dist/simplebar.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/dist/simplebar.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/dist/simplebar.d.ts` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/dist/simplebar.d.ts`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/dist/simplebar.esm.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/dist/simplebar.esm.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/dist/simplebar.esm.js.map` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/dist/simplebar.esm.js.map`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/dist/simplebar.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/dist/simplebar.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/dist/simplebar.min.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/dist/simplebar.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/dist/simplebar.min.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/dist/simplebar.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/dist/simplebar.umd.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/dist/simplebar.umd.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/package.json` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/package.json`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/src/helpers.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/src/helpers.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/src/index.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/src/index.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/src/scrollbar-width.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/src/scrollbar-width.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/src/simplebar.css` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/src/simplebar.css`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/libs/simplebar/src/simplebar.js` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/libs/simplebar/src/simplebar.js`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/layouts/_header.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/layouts/_header.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/layouts/_layouts.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/layouts/_layouts.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/layouts/_sidebar.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/layouts/_sidebar.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/pages/_dashboard1.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/pages/_dashboard1.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/prepros.config` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/prepros.config`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/styles.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/styles.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/variables/_theme-variables.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/variables/_theme-variables.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/static/assets/scss/variables/_variables.scss` & `django-admin-modernize-1.0.3/admin_modernize/static/assets/scss/variables/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/accounts/login.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/accounts/login.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/accounts/password_change.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/accounts/password_change.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/accounts/password_change_done.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/accounts/password_change_done.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/accounts/password_reset.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/accounts/password_reset.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/accounts/password_reset_complete.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/accounts/password_reset_complete.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/accounts/password_reset_confirm.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/accounts/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/accounts/password_reset_done.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/accounts/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/accounts/register.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/accounts/register.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/admin/actions.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/admin/auth/user/change_password.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/admin/auth/user/change_password.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/admin/change_form.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/admin/change_form_object_tools.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/admin/change_form_object_tools.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/admin/change_list.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/admin/change_list_results.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/admin/delete_confirmation.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/admin/delete_selected_confirmation.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/admin/edit_inline/stacked.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/admin/edit_inline/tabular.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/admin/edit_inline/tabular.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/admin/includes/fieldset.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/admin/index.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/admin/invalid_setup.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/admin/invalid_setup.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/admin/login.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/admin/object_history.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/admin/pagination.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/admin/search_form.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/admin/submit_line.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/includes/navigation.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/includes/navigation.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/includes/scripts.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/includes/scripts.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/includes/sidebar.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/includes/sidebar.html`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         </ul>
         {% endif %}
         <div class="unlimited-access hide-menu bg-light-primary position-relative mb-7 mt-5 rounded">
           <div class="d-flex">
             <div class="unlimited-access-title me-3">
               <h6 class="fw-semibold fs-4 mb-6 text-dark w-85">Need More?</h6>
               <a href="https://adminmart.com/product/modernize-bootstrap-5-admin-template/?ref=1" target="_blank"
-                class="btn btn-primary fs-2 fw-semibold lh-sm">Download Pro</a>
+                class="btn btn-primary fs-2 fw-semibold lh-sm">PRO Version</a>
             </div>
             <div class="unlimited-access-img">
               <img src="{% static 'assets/images/backgrounds/rocket.png' %}" alt="" class="img-fluid">
             </div>
           </div>
         </div>
       </nav>
```

#### html2text {}

```diff
@@ -23,10 +23,10 @@
     *  EXTRA
     *    Icons
     *    Sample_Page
     *  AUTH
     *    Logout
 {% endif %}
 * Need More? *
-Download_Pro
+PRO_Version
```

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/layouts/auth_base.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/layouts/auth_base.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/layouts/base.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/layouts/base.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/layouts/base_logout.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/layouts/base_logout.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/pages/index.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/pages/index.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/pages/sign-in.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/pages/sign-in.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/pages/sign-up.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/pages/sign-up.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/pages/ui-alerts.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/pages/ui-alerts.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/pages/ui-buttons.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/pages/ui-buttons.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/pages/ui-card.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/pages/ui-card.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/pages/ui-forms.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/pages/ui-forms.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/pages/ui-typography.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/pages/ui-typography.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/registration/logged_out.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/registration/logged_out.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/registration/password_change_done.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templates/registration/password_change_form.html` & `django-admin-modernize-1.0.3/admin_modernize/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/templatetags/admin_modernize.py` & `django-admin-modernize-1.0.3/admin_modernize/templatetags/admin_modernize.py`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/urls.py` & `django-admin-modernize-1.0.3/admin_modernize/urls.py`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/utils.py` & `django-admin-modernize-1.0.3/admin_modernize/utils.py`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/admin_modernize/views.py` & `django-admin-modernize-1.0.3/admin_modernize/views.py`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/django_admin_modernize.egg-info/PKG-INFO` & `django-admin-modernize-1.0.3/django_admin_modernize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-modernize
-Version: 1.0.2
+Version: 1.0.3
 Summary: Modern template for Django admin interface
 Home-page: https://github.com/app-generator/django-modernize
 Author: AppSeed.us
 Author-email: support@appseed.us
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

### Comparing `django-admin-modernize-1.0.2/django_admin_modernize.egg-info/SOURCES.txt` & `django-admin-modernize-1.0.3/django_admin_modernize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-admin-modernize-1.0.2/setup.py` & `django-admin-modernize-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
 name='django-admin-modernize',
-version='1.0.2',
+version='1.0.3',
 zip_safe=False,
 packages=find_packages(),
 include_package_data=True,
 description='Modern template for Django admin interface',
 long_description=README,
 long_description_content_type="text/markdown",
 url='https://github.com/app-generator/django-modernize',
```

