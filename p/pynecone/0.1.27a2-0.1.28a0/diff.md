# Comparing `tmp/pynecone-0.1.27a2.tar.gz` & `tmp/pynecone-0.1.28a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynecone-0.1.27a2.tar", max compression
+gzip compressed data, was "pynecone-0.1.28a0.tar", max compression
```

## Comparing `pynecone-0.1.27a2.tar` & `pynecone-0.1.28a0.tar`

### file list

```diff
@@ -1,150 +1,150 @@
--rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.27a2/LICENSE
--rw-r--r--   0        0        0     7887 2023-04-27 02:06:35.740679 pynecone-0.1.27a2/README.md
--rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747147 pynecone-0.1.27a2/pynecone/.templates/apps/counter/__init__.py
--rw-r--r--   0        0        0     1340 2023-04-27 02:06:35.747526 pynecone-0.1.27a2/pynecone/.templates/apps/counter/counter.py
--rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747631 pynecone-0.1.27a2/pynecone/.templates/apps/default/__init__.py
--rw-r--r--   0        0        0     1036 2023-04-27 02:06:35.747905 pynecone-0.1.27a2/pynecone/.templates/apps/default/default.py
--rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.27a2/pynecone/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.27a2/pynecone/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   248832 2023-04-27 02:06:35.749179 pynecone-0.1.27a2/pynecone/.templates/web/bun.lockb
--rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.27a2/pynecone/.templates/web/next.config.js
--rw-r--r--   0        0        0     1017 2023-04-27 02:06:35.749525 pynecone-0.1.27a2/pynecone/.templates/web/package.json
--rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.27a2/pynecone/.templates/web/pages/404.js
--rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.27a2/pynecone/.templates/web/pages/_app.js
--rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.27a2/pynecone/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0     6690 2023-04-27 02:06:35.750015 pynecone-0.1.27a2/pynecone/.templates/web/utils/state.js
--rw-r--r--   0        0        0      808 2023-04-27 02:06:35.750342 pynecone-0.1.27a2/pynecone/__init__.py
--rw-r--r--   0        0        0    19779 2023-04-27 20:19:44.815410 pynecone-0.1.27a2/pynecone/app.py
--rw-r--r--   0        0        0     2510 2023-01-30 21:50:18.206745 pynecone-0.1.27a2/pynecone/base.py
--rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.27a2/pynecone/compiler/__init__.py
--rw-r--r--   0        0        0     5856 2023-04-27 02:06:35.751250 pynecone-0.1.27a2/pynecone/compiler/compiler.py
--rw-r--r--   0        0        0     5590 2023-04-27 02:06:35.751649 pynecone-0.1.27a2/pynecone/compiler/templates.py
--rw-r--r--   0        0        0     9084 2023-04-24 22:10:28.096707 pynecone-0.1.27a2/pynecone/compiler/utils.py
--rw-r--r--   0        0        0     6371 2023-04-02 23:51:14.631475 pynecone-0.1.27a2/pynecone/components/__init__.py
--rw-r--r--   0        0        0      226 2023-03-13 04:10:28.615930 pynecone-0.1.27a2/pynecone/components/base/__init__.py
--rw-r--r--   0        0        0      726 2023-04-27 20:19:44.815578 pynecone-0.1.27a2/pynecone/components/base/bare.py
--rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.27a2/pynecone/components/base/body.py
--rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.27a2/pynecone/components/base/document.py
--rw-r--r--   0        0        0      242 2022-11-18 20:43:33.735533 pynecone-0.1.27a2/pynecone/components/base/head.py
--rw-r--r--   0        0        0      929 2023-03-13 04:10:28.761099 pynecone-0.1.27a2/pynecone/components/base/link.py
--rw-r--r--   0        0        0     1399 2023-03-10 00:25:42.693576 pynecone-0.1.27a2/pynecone/components/base/meta.py
--rw-r--r--   0        0        0    21330 2023-04-27 20:25:18.590022 pynecone-0.1.27a2/pynecone/components/component.py
--rw-r--r--   0        0        0      422 2023-04-02 23:51:14.632016 pynecone-0.1.27a2/pynecone/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      333 2022-11-18 20:43:33.720898 pynecone-0.1.27a2/pynecone/components/datadisplay/badge.py
--rw-r--r--   0        0        0     2486 2023-03-16 23:52:12.744773 pynecone-0.1.27a2/pynecone/components/datadisplay/code.py
--rw-r--r--   0        0        0     4161 2023-04-27 02:06:35.752662 pynecone-0.1.27a2/pynecone/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      536 2022-11-18 20:43:33.720383 pynecone-0.1.27a2/pynecone/components/datadisplay/divider.py
--rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.27a2/pynecone/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1429 2023-03-13 04:10:28.547828 pynecone-0.1.27a2/pynecone/components/datadisplay/list.py
--rw-r--r--   0        0        0     2156 2023-03-09 23:41:57.135449 pynecone-0.1.27a2/pynecone/components/datadisplay/stat.py
--rw-r--r--   0        0        0     5156 2023-03-10 00:25:42.695438 pynecone-0.1.27a2/pynecone/components/datadisplay/table.py
--rw-r--r--   0        0        0      316 2023-01-24 02:43:48.871608 pynecone-0.1.27a2/pynecone/components/disclosure/__init__.py
--rw-r--r--   0        0        0     2940 2023-03-09 23:41:57.135814 pynecone-0.1.27a2/pynecone/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2776 2023-03-09 23:41:57.135961 pynecone-0.1.27a2/pynecone/components/disclosure/tabs.py
--rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.27a2/pynecone/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.27a2/pynecone/components/feedback/__init__.py
--rw-r--r--   0        0        0     1570 2023-03-10 00:25:42.695849 pynecone-0.1.27a2/pynecone/components/feedback/alert.py
--rw-r--r--   0        0        0     1904 2023-03-10 00:25:42.696112 pynecone-0.1.27a2/pynecone/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      878 2023-03-10 00:25:42.696451 pynecone-0.1.27a2/pynecone/components/feedback/progress.py
--rw-r--r--   0        0        0     1784 2022-11-18 20:43:33.722941 pynecone-0.1.27a2/pynecone/components/feedback/skeleton.py
--rw-r--r--   0        0        0      677 2022-11-18 20:43:33.724636 pynecone-0.1.27a2/pynecone/components/feedback/spinner.py
--rw-r--r--   0        0        0     1103 2023-03-10 00:25:42.696881 pynecone-0.1.27a2/pynecone/components/forms/__init__.py
--rw-r--r--   0        0        0     1717 2023-04-27 02:06:35.752925 pynecone-0.1.27a2/pynecone/components/forms/button.py
--rw-r--r--   0        0        0     2469 2023-04-27 02:06:35.753108 pynecone-0.1.27a2/pynecone/components/forms/checkbox.py
--rw-r--r--   0        0        0      593 2023-01-30 21:50:18.211339 pynecone-0.1.27a2/pynecone/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0     1964 2023-03-10 00:25:42.697696 pynecone-0.1.27a2/pynecone/components/forms/editable.py
--rw-r--r--   0        0        0     2323 2023-03-09 23:41:57.137070 pynecone-0.1.27a2/pynecone/components/forms/formcontrol.py
--rw-r--r--   0        0        0      801 2022-12-07 23:08:48.791901 pynecone-0.1.27a2/pynecone/components/forms/iconbutton.py
--rw-r--r--   0        0        0     2660 2023-04-22 16:00:37.547486 pynecone-0.1.27a2/pynecone/components/forms/input.py
--rw-r--r--   0        0        0     3916 2023-03-10 00:25:42.698330 pynecone-0.1.27a2/pynecone/components/forms/numberinput.py
--rw-r--r--   0        0        0      252 2023-03-10 00:25:42.698673 pynecone-0.1.27a2/pynecone/components/forms/password.py
--rw-r--r--   0        0        0     2685 2023-03-10 00:25:42.698849 pynecone-0.1.27a2/pynecone/components/forms/pininput.py
--rw-r--r--   0        0        0     3004 2023-03-16 23:52:12.745021 pynecone-0.1.27a2/pynecone/components/forms/radio.py
--rw-r--r--   0        0        0     2868 2023-03-10 00:25:42.699342 pynecone-0.1.27a2/pynecone/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3475 2023-03-16 23:52:12.745104 pynecone-0.1.27a2/pynecone/components/forms/select.py
--rw-r--r--   0        0        0     2782 2023-03-10 00:25:42.699714 pynecone-0.1.27a2/pynecone/components/forms/slider.py
--rw-r--r--   0        0        0     1466 2023-03-10 00:25:42.699988 pynecone-0.1.27a2/pynecone/components/forms/switch.py
--rw-r--r--   0        0        0     1550 2023-03-10 00:25:42.700204 pynecone-0.1.27a2/pynecone/components/forms/textarea.py
--rw-r--r--   0        0        0     2907 2023-04-27 02:06:35.753294 pynecone-0.1.27a2/pynecone/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.27a2/pynecone/components/graphing/__init__.py
--rw-r--r--   0        0        0     1356 2023-04-27 02:06:35.753790 pynecone-0.1.27a2/pynecone/components/graphing/plotly.py
--rw-r--r--   0        0        0    17359 2023-04-27 02:06:35.754541 pynecone-0.1.27a2/pynecone/components/graphing/victory.py
--rw-r--r--   0        0        0      815 2023-04-02 23:51:14.632791 pynecone-0.1.27a2/pynecone/components/layout/__init__.py
--rw-r--r--   0        0        0      323 2023-04-02 23:51:14.632894 pynecone-0.1.27a2/pynecone/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      768 2022-12-15 19:19:57.795670 pynecone-0.1.27a2/pynecone/components/layout/box.py
--rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.27a2/pynecone/components/layout/center.py
--rw-r--r--   0        0        0     3136 2023-03-16 23:52:12.745203 pynecone-0.1.27a2/pynecone/components/layout/cond.py
--rw-r--r--   0        0        0      362 2022-12-07 23:08:48.792884 pynecone-0.1.27a2/pynecone/components/layout/container.py
--rw-r--r--   0        0        0      655 2022-12-07 23:08:48.793078 pynecone-0.1.27a2/pynecone/components/layout/flex.py
--rw-r--r--   0        0        0     1781 2023-03-10 00:25:42.701858 pynecone-0.1.27a2/pynecone/components/layout/foreach.py
--rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.27a2/pynecone/components/layout/fragment.py
--rw-r--r--   0        0        0     2417 2023-01-28 19:09:51.493446 pynecone-0.1.27a2/pynecone/components/layout/grid.py
--rw-r--r--   0        0        0      979 2023-04-27 02:06:35.755389 pynecone-0.1.27a2/pynecone/components/layout/html.py
--rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.27a2/pynecone/components/layout/responsive.py
--rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.27a2/pynecone/components/layout/spacer.py
--rw-r--r--   0        0        0      994 2022-12-07 23:08:48.793762 pynecone-0.1.27a2/pynecone/components/layout/stack.py
--rw-r--r--   0        0        0     1470 2023-03-09 23:41:57.138212 pynecone-0.1.27a2/pynecone/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.27a2/pynecone/components/libs/__init__.py
--rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.27a2/pynecone/components/libs/chakra.py
--rw-r--r--   0        0        0      190 2022-11-18 20:43:33.736163 pynecone-0.1.27a2/pynecone/components/media/__init__.py
--rw-r--r--   0        0        0     1539 2022-11-28 06:46:25.092156 pynecone-0.1.27a2/pynecone/components/media/avatar.py
--rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.27a2/pynecone/components/media/icon.py
--rw-r--r--   0        0        0     1415 2022-12-07 23:08:48.794371 pynecone-0.1.27a2/pynecone/components/media/image.py
--rw-r--r--   0        0        0      282 2023-01-24 02:43:48.884756 pynecone-0.1.27a2/pynecone/components/navigation/__init__.py
--rw-r--r--   0        0        0     2022 2023-03-09 23:41:57.138732 pynecone-0.1.27a2/pynecone/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0     1005 2023-01-24 01:31:44.831545 pynecone-0.1.27a2/pynecone/components/navigation/link.py
--rw-r--r--   0        0        0      529 2022-12-07 23:08:48.794948 pynecone-0.1.27a2/pynecone/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      483 2022-12-07 23:08:48.795126 pynecone-0.1.27a2/pynecone/components/navigation/nextlink.py
--rw-r--r--   0        0        0      850 2023-01-24 02:43:48.892006 pynecone-0.1.27a2/pynecone/components/overlay/__init__.py
--rw-r--r--   0        0        0     5042 2023-03-10 00:25:42.703076 pynecone-0.1.27a2/pynecone/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     4696 2023-03-10 00:25:42.703402 pynecone-0.1.27a2/pynecone/components/overlay/drawer.py
--rw-r--r--   0        0        0     5545 2023-03-10 00:25:42.703834 pynecone-0.1.27a2/pynecone/components/overlay/menu.py
--rw-r--r--   0        0        0     4932 2023-03-10 00:25:42.704095 pynecone-0.1.27a2/pynecone/components/overlay/modal.py
--rw-r--r--   0        0        0     5703 2023-03-09 23:41:57.139627 pynecone-0.1.27a2/pynecone/components/overlay/popover.py
--rw-r--r--   0        0        0     1964 2023-01-28 19:09:51.496014 pynecone-0.1.27a2/pynecone/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.27a2/pynecone/components/tags/__init__.py
--rw-r--r--   0        0        0      840 2023-03-16 23:52:12.745828 pynecone-0.1.27a2/pynecone/components/tags/cond_tag.py
--rw-r--r--   0        0        0     3000 2023-03-16 23:52:12.746048 pynecone-0.1.27a2/pynecone/components/tags/iter_tag.py
--rw-r--r--   0        0        0     6443 2023-04-27 02:58:41.817899 pynecone-0.1.27a2/pynecone/components/tags/tag.py
--rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.27a2/pynecone/components/tags/tagless.py
--rw-r--r--   0        0        0      271 2022-12-07 23:08:48.795802 pynecone-0.1.27a2/pynecone/components/typography/__init__.py
--rw-r--r--   0        0        0      281 2022-12-07 23:08:48.796090 pynecone-0.1.27a2/pynecone/components/typography/heading.py
--rw-r--r--   0        0        0      357 2023-03-09 23:41:57.139928 pynecone-0.1.27a2/pynecone/components/typography/highlight.py
--rw-r--r--   0        0        0     2973 2023-04-27 02:06:35.755989 pynecone-0.1.27a2/pynecone/components/typography/markdown.py
--rw-r--r--   0        0        0      336 2022-12-08 04:28:39.380713 pynecone-0.1.27a2/pynecone/components/typography/span.py
--rw-r--r--   0        0        0      305 2022-12-07 23:08:48.796735 pynecone-0.1.27a2/pynecone/components/typography/text.py
--rw-r--r--   0        0        0     5296 2023-04-27 02:06:35.756502 pynecone-0.1.27a2/pynecone/config.py
--rw-r--r--   0        0        0     8765 2023-04-27 02:06:35.756870 pynecone-0.1.27a2/pynecone/constants.py
--rw-r--r--   0        0        0       73 2023-04-27 02:06:35.757531 pynecone-0.1.27a2/pynecone/el/__init__.py
--rw-r--r--   0        0        0      115 2023-04-27 02:06:35.757829 pynecone-0.1.27a2/pynecone/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-04-27 02:06:35.758045 pynecone-0.1.27a2/pynecone/el/constants/html.py
--rw-r--r--   0        0        0     1719 2023-04-27 02:06:35.758325 pynecone-0.1.27a2/pynecone/el/constants/pynecone.py
--rw-r--r--   0        0        0    15554 2023-04-27 02:06:35.758673 pynecone-0.1.27a2/pynecone/el/constants/react.py
--rw-r--r--   0        0        0     1289 2023-04-27 02:06:35.759113 pynecone-0.1.27a2/pynecone/el/element.py
--rw-r--r--   0        0        0   108515 2023-04-27 02:06:35.759585 pynecone-0.1.27a2/pynecone/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2666 2023-04-27 02:06:35.759864 pynecone-0.1.27a2/pynecone/el/precompile.py
--rw-r--r--   0        0        0     9731 2023-04-27 02:06:35.760254 pynecone-0.1.27a2/pynecone/event.py
--rw-r--r--   0        0        0      163 2022-12-27 07:24:05.349499 pynecone-0.1.27a2/pynecone/middleware/__init__.py
--rw-r--r--   0        0        0     3259 2023-04-27 02:06:35.760663 pynecone-0.1.27a2/pynecone/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1022 2023-04-27 02:06:35.761080 pynecone-0.1.27a2/pynecone/middleware/logging_middleware.py
--rw-r--r--   0        0        0     1193 2023-04-27 02:06:35.761405 pynecone-0.1.27a2/pynecone/middleware/middleware.py
--rw-r--r--   0        0        0     2085 2023-04-27 02:06:35.761858 pynecone-0.1.27a2/pynecone/model.py
--rw-r--r--   0        0        0     8093 2023-04-27 02:06:35.762135 pynecone-0.1.27a2/pynecone/pc.py
--rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.27a2/pynecone/py.typed
--rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.27a2/pynecone/route.py
--rw-r--r--   0        0        0    26831 2023-04-27 02:06:35.762920 pynecone-0.1.27a2/pynecone/state.py
--rw-r--r--   0        0        0     1059 2023-03-16 23:52:12.748857 pynecone-0.1.27a2/pynecone/style.py
--rw-r--r--   0        0        0     2411 2023-03-10 00:25:42.708535 pynecone-0.1.27a2/pynecone/telemetry.py
--rw-r--r--   0        0        0     4252 2023-04-27 02:06:35.763291 pynecone-0.1.27a2/pynecone/utils/build.py
--rw-r--r--   0        0        0     1627 2023-03-16 23:52:12.749156 pynecone-0.1.27a2/pynecone/utils/console.py
--rw-r--r--   0        0        0     3597 2023-04-27 02:06:35.763631 pynecone-0.1.27a2/pynecone/utils/exec.py
--rw-r--r--   0        0        0    10401 2023-04-27 02:10:11.487060 pynecone-0.1.27a2/pynecone/utils/format.py
--rw-r--r--   0        0        0      544 2023-03-16 23:52:12.757094 pynecone-0.1.27a2/pynecone/utils/imports.py
--rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.27a2/pynecone/utils/path_ops.py
--rw-r--r--   0        0        0     9121 2023-04-27 18:44:17.310876 pynecone-0.1.27a2/pynecone/utils/prerequisites.py
--rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.27a2/pynecone/utils/processes.py
--rw-r--r--   0        0        0     4299 2023-03-16 23:52:12.757408 pynecone-0.1.27a2/pynecone/utils/types.py
--rw-r--r--   0        0        0    25531 2023-04-27 02:07:41.860141 pynecone-0.1.27a2/pynecone/var.py
--rw-r--r--   0        0        0     2634 2023-03-13 04:10:28.761553 pynecone-0.1.27a2/pynecone/watch.py
--rw-r--r--   0        0        0     1758 2023-04-27 20:39:51.447563 pynecone-0.1.27a2/pyproject.toml
--rw-r--r--   0        0        0     9379 1970-01-01 00:00:00.000000 pynecone-0.1.27a2/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.28a0/LICENSE
+-rw-r--r--   0        0        0     7887 2023-04-27 23:08:51.375669 pynecone-0.1.28a0/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747147 pynecone-0.1.28a0/pynecone/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1340 2023-04-27 02:06:35.747526 pynecone-0.1.28a0/pynecone/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747631 pynecone-0.1.28a0/pynecone/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1036 2023-04-27 02:06:35.747905 pynecone-0.1.28a0/pynecone/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.28a0/pynecone/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.28a0/pynecone/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   248832 2023-04-28 22:48:11.602895 pynecone-0.1.28a0/pynecone/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.28a0/pynecone/.templates/web/next.config.js
+-rw-r--r--   0        0        0     1017 2023-04-28 22:48:11.603117 pynecone-0.1.28a0/pynecone/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.28a0/pynecone/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.28a0/pynecone/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.28a0/pynecone/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0     6809 2023-04-30 03:30:20.667278 pynecone-0.1.28a0/pynecone/.templates/web/utils/state.js
+-rw-r--r--   0        0        0      823 2023-04-30 03:30:20.667423 pynecone-0.1.28a0/pynecone/__init__.py
+-rw-r--r--   0        0        0    19779 2023-04-29 22:56:24.699882 pynecone-0.1.28a0/pynecone/app.py
+-rw-r--r--   0        0        0     2510 2023-01-30 21:50:18.206745 pynecone-0.1.28a0/pynecone/base.py
+-rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.28a0/pynecone/compiler/__init__.py
+-rw-r--r--   0        0        0     5856 2023-04-29 22:32:13.534526 pynecone-0.1.28a0/pynecone/compiler/compiler.py
+-rw-r--r--   0        0        0     5590 2023-04-27 23:08:51.378717 pynecone-0.1.28a0/pynecone/compiler/templates.py
+-rw-r--r--   0        0        0     9084 2023-04-24 22:10:28.096707 pynecone-0.1.28a0/pynecone/compiler/utils.py
+-rw-r--r--   0        0        0     6371 2023-05-01 17:34:03.602730 pynecone-0.1.28a0/pynecone/components/__init__.py
+-rw-r--r--   0        0        0      226 2023-03-13 04:10:28.615930 pynecone-0.1.28a0/pynecone/components/base/__init__.py
+-rw-r--r--   0        0        0      726 2023-04-27 21:37:27.235866 pynecone-0.1.28a0/pynecone/components/base/bare.py
+-rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.28a0/pynecone/components/base/body.py
+-rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.28a0/pynecone/components/base/document.py
+-rw-r--r--   0        0        0      242 2022-11-18 20:43:33.735533 pynecone-0.1.28a0/pynecone/components/base/head.py
+-rw-r--r--   0        0        0      929 2023-03-13 04:10:28.761099 pynecone-0.1.28a0/pynecone/components/base/link.py
+-rw-r--r--   0        0        0     1399 2023-03-10 00:25:42.693576 pynecone-0.1.28a0/pynecone/components/base/meta.py
+-rw-r--r--   0        0        0    21824 2023-04-30 03:30:20.667624 pynecone-0.1.28a0/pynecone/components/component.py
+-rw-r--r--   0        0        0      422 2023-04-02 23:51:14.632016 pynecone-0.1.28a0/pynecone/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      333 2022-11-18 20:43:33.720898 pynecone-0.1.28a0/pynecone/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     2486 2023-03-16 23:52:12.744773 pynecone-0.1.28a0/pynecone/components/datadisplay/code.py
+-rw-r--r--   0        0        0     4161 2023-04-27 23:08:51.379280 pynecone-0.1.28a0/pynecone/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      536 2022-11-18 20:43:33.720383 pynecone-0.1.28a0/pynecone/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.28a0/pynecone/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1429 2023-03-13 04:10:28.547828 pynecone-0.1.28a0/pynecone/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2156 2023-03-09 23:41:57.135449 pynecone-0.1.28a0/pynecone/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     5156 2023-03-10 00:25:42.695438 pynecone-0.1.28a0/pynecone/components/datadisplay/table.py
+-rw-r--r--   0        0        0      316 2023-01-24 02:43:48.871608 pynecone-0.1.28a0/pynecone/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     2940 2023-03-09 23:41:57.135814 pynecone-0.1.28a0/pynecone/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2776 2023-03-09 23:41:57.135961 pynecone-0.1.28a0/pynecone/components/disclosure/tabs.py
+-rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.28a0/pynecone/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.28a0/pynecone/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1570 2023-03-10 00:25:42.695849 pynecone-0.1.28a0/pynecone/components/feedback/alert.py
+-rw-r--r--   0        0        0     1904 2023-03-10 00:25:42.696112 pynecone-0.1.28a0/pynecone/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      878 2023-03-10 00:25:42.696451 pynecone-0.1.28a0/pynecone/components/feedback/progress.py
+-rw-r--r--   0        0        0     1784 2022-11-18 20:43:33.722941 pynecone-0.1.28a0/pynecone/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      677 2022-11-18 20:43:33.724636 pynecone-0.1.28a0/pynecone/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1103 2023-05-01 17:34:03.603087 pynecone-0.1.28a0/pynecone/components/forms/__init__.py
+-rw-r--r--   0        0        0     1717 2023-04-27 23:08:51.379424 pynecone-0.1.28a0/pynecone/components/forms/button.py
+-rw-r--r--   0        0        0     2469 2023-04-27 23:08:51.379545 pynecone-0.1.28a0/pynecone/components/forms/checkbox.py
+-rw-r--r--   0        0        0      593 2023-01-30 21:50:18.211339 pynecone-0.1.28a0/pynecone/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0     1964 2023-03-10 00:25:42.697696 pynecone-0.1.28a0/pynecone/components/forms/editable.py
+-rw-r--r--   0        0        0     2323 2023-05-01 17:34:03.603304 pynecone-0.1.28a0/pynecone/components/forms/formcontrol.py
+-rw-r--r--   0        0        0      801 2022-12-07 23:08:48.791901 pynecone-0.1.28a0/pynecone/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     3068 2023-04-30 03:30:20.667778 pynecone-0.1.28a0/pynecone/components/forms/input.py
+-rw-r--r--   0        0        0     3916 2023-03-10 00:25:42.698330 pynecone-0.1.28a0/pynecone/components/forms/numberinput.py
+-rw-r--r--   0        0        0      252 2023-03-10 00:25:42.698673 pynecone-0.1.28a0/pynecone/components/forms/password.py
+-rw-r--r--   0        0        0     2685 2023-03-10 00:25:42.698849 pynecone-0.1.28a0/pynecone/components/forms/pininput.py
+-rw-r--r--   0        0        0     3004 2023-03-16 23:52:12.745021 pynecone-0.1.28a0/pynecone/components/forms/radio.py
+-rw-r--r--   0        0        0     2868 2023-03-10 00:25:42.699342 pynecone-0.1.28a0/pynecone/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3475 2023-03-16 23:52:12.745104 pynecone-0.1.28a0/pynecone/components/forms/select.py
+-rw-r--r--   0        0        0     2782 2023-03-10 00:25:42.699714 pynecone-0.1.28a0/pynecone/components/forms/slider.py
+-rw-r--r--   0        0        0     1466 2023-03-10 00:25:42.699988 pynecone-0.1.28a0/pynecone/components/forms/switch.py
+-rw-r--r--   0        0        0     1550 2023-03-10 00:25:42.700204 pynecone-0.1.28a0/pynecone/components/forms/textarea.py
+-rw-r--r--   0        0        0     2907 2023-04-27 23:08:51.379851 pynecone-0.1.28a0/pynecone/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.28a0/pynecone/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1356 2023-04-27 02:06:35.753790 pynecone-0.1.28a0/pynecone/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17359 2023-04-27 02:06:35.754541 pynecone-0.1.28a0/pynecone/components/graphing/victory.py
+-rw-r--r--   0        0        0      815 2023-04-02 23:51:14.632791 pynecone-0.1.28a0/pynecone/components/layout/__init__.py
+-rw-r--r--   0        0        0      323 2023-04-02 23:51:14.632894 pynecone-0.1.28a0/pynecone/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      768 2022-12-15 19:19:57.795670 pynecone-0.1.28a0/pynecone/components/layout/box.py
+-rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.28a0/pynecone/components/layout/center.py
+-rw-r--r--   0        0        0     3136 2023-03-16 23:52:12.745203 pynecone-0.1.28a0/pynecone/components/layout/cond.py
+-rw-r--r--   0        0        0      362 2022-12-07 23:08:48.792884 pynecone-0.1.28a0/pynecone/components/layout/container.py
+-rw-r--r--   0        0        0      655 2022-12-07 23:08:48.793078 pynecone-0.1.28a0/pynecone/components/layout/flex.py
+-rw-r--r--   0        0        0     1781 2023-03-10 00:25:42.701858 pynecone-0.1.28a0/pynecone/components/layout/foreach.py
+-rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.28a0/pynecone/components/layout/fragment.py
+-rw-r--r--   0        0        0     2417 2023-01-28 19:09:51.493446 pynecone-0.1.28a0/pynecone/components/layout/grid.py
+-rw-r--r--   0        0        0      979 2023-04-27 02:06:35.755389 pynecone-0.1.28a0/pynecone/components/layout/html.py
+-rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.28a0/pynecone/components/layout/responsive.py
+-rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.28a0/pynecone/components/layout/spacer.py
+-rw-r--r--   0        0        0      994 2022-12-07 23:08:48.793762 pynecone-0.1.28a0/pynecone/components/layout/stack.py
+-rw-r--r--   0        0        0     1470 2023-03-09 23:41:57.138212 pynecone-0.1.28a0/pynecone/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.28a0/pynecone/components/libs/__init__.py
+-rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.28a0/pynecone/components/libs/chakra.py
+-rw-r--r--   0        0        0      190 2022-11-18 20:43:33.736163 pynecone-0.1.28a0/pynecone/components/media/__init__.py
+-rw-r--r--   0        0        0     1539 2022-11-28 06:46:25.092156 pynecone-0.1.28a0/pynecone/components/media/avatar.py
+-rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.28a0/pynecone/components/media/icon.py
+-rw-r--r--   0        0        0     1415 2022-12-07 23:08:48.794371 pynecone-0.1.28a0/pynecone/components/media/image.py
+-rw-r--r--   0        0        0      282 2023-01-24 02:43:48.884756 pynecone-0.1.28a0/pynecone/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2022 2023-03-09 23:41:57.138732 pynecone-0.1.28a0/pynecone/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1005 2023-04-28 22:48:11.604564 pynecone-0.1.28a0/pynecone/components/navigation/link.py
+-rw-r--r--   0        0        0      529 2022-12-07 23:08:48.794948 pynecone-0.1.28a0/pynecone/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      483 2022-12-07 23:08:48.795126 pynecone-0.1.28a0/pynecone/components/navigation/nextlink.py
+-rw-r--r--   0        0        0      850 2023-01-24 02:43:48.892006 pynecone-0.1.28a0/pynecone/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5042 2023-03-10 00:25:42.703076 pynecone-0.1.28a0/pynecone/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     4696 2023-03-10 00:25:42.703402 pynecone-0.1.28a0/pynecone/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5545 2023-03-10 00:25:42.703834 pynecone-0.1.28a0/pynecone/components/overlay/menu.py
+-rw-r--r--   0        0        0     4932 2023-03-10 00:25:42.704095 pynecone-0.1.28a0/pynecone/components/overlay/modal.py
+-rw-r--r--   0        0        0     5703 2023-03-09 23:41:57.139627 pynecone-0.1.28a0/pynecone/components/overlay/popover.py
+-rw-r--r--   0        0        0     1964 2023-01-28 19:09:51.496014 pynecone-0.1.28a0/pynecone/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.28a0/pynecone/components/tags/__init__.py
+-rw-r--r--   0        0        0      840 2023-03-16 23:52:12.745828 pynecone-0.1.28a0/pynecone/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     3000 2023-03-16 23:52:12.746048 pynecone-0.1.28a0/pynecone/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     6463 2023-04-30 03:30:20.667909 pynecone-0.1.28a0/pynecone/components/tags/tag.py
+-rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.28a0/pynecone/components/tags/tagless.py
+-rw-r--r--   0        0        0      271 2022-12-07 23:08:48.795802 pynecone-0.1.28a0/pynecone/components/typography/__init__.py
+-rw-r--r--   0        0        0      281 2022-12-07 23:08:48.796090 pynecone-0.1.28a0/pynecone/components/typography/heading.py
+-rw-r--r--   0        0        0      357 2023-03-09 23:41:57.139928 pynecone-0.1.28a0/pynecone/components/typography/highlight.py
+-rw-r--r--   0        0        0     2973 2023-04-27 02:06:35.755989 pynecone-0.1.28a0/pynecone/components/typography/markdown.py
+-rw-r--r--   0        0        0      336 2022-12-08 04:28:39.380713 pynecone-0.1.28a0/pynecone/components/typography/span.py
+-rw-r--r--   0        0        0      305 2022-12-07 23:08:48.796735 pynecone-0.1.28a0/pynecone/components/typography/text.py
+-rw-r--r--   0        0        0     5296 2023-04-27 02:06:35.756502 pynecone-0.1.28a0/pynecone/config.py
+-rw-r--r--   0        0        0     8765 2023-04-27 23:08:51.380182 pynecone-0.1.28a0/pynecone/constants.py
+-rw-r--r--   0        0        0       73 2023-04-27 02:06:35.757531 pynecone-0.1.28a0/pynecone/el/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-27 02:06:35.757829 pynecone-0.1.28a0/pynecone/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-04-27 02:06:35.758045 pynecone-0.1.28a0/pynecone/el/constants/html.py
+-rw-r--r--   0        0        0     1719 2023-04-27 02:06:35.758325 pynecone-0.1.28a0/pynecone/el/constants/pynecone.py
+-rw-r--r--   0        0        0    15554 2023-04-27 02:06:35.758673 pynecone-0.1.28a0/pynecone/el/constants/react.py
+-rw-r--r--   0        0        0     1289 2023-04-27 02:06:35.759113 pynecone-0.1.28a0/pynecone/el/element.py
+-rw-r--r--   0        0        0   108515 2023-04-27 02:06:35.759585 pynecone-0.1.28a0/pynecone/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2666 2023-04-27 02:06:35.759864 pynecone-0.1.28a0/pynecone/el/precompile.py
+-rw-r--r--   0        0        0    10189 2023-04-30 03:30:20.668065 pynecone-0.1.28a0/pynecone/event.py
+-rw-r--r--   0        0        0      163 2022-12-27 07:24:05.349499 pynecone-0.1.28a0/pynecone/middleware/__init__.py
+-rw-r--r--   0        0        0     3259 2023-04-27 23:08:51.380497 pynecone-0.1.28a0/pynecone/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1022 2023-04-27 02:06:35.761080 pynecone-0.1.28a0/pynecone/middleware/logging_middleware.py
+-rw-r--r--   0        0        0     1193 2023-04-27 02:06:35.761405 pynecone-0.1.28a0/pynecone/middleware/middleware.py
+-rw-r--r--   0        0        0     2085 2023-04-27 23:08:51.380631 pynecone-0.1.28a0/pynecone/model.py
+-rw-r--r--   0        0        0     8093 2023-04-27 02:06:35.762135 pynecone-0.1.28a0/pynecone/pc.py
+-rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.28a0/pynecone/py.typed
+-rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.28a0/pynecone/route.py
+-rw-r--r--   0        0        0    26952 2023-04-28 23:22:46.251992 pynecone-0.1.28a0/pynecone/state.py
+-rw-r--r--   0        0        0     1059 2023-03-16 23:52:12.748857 pynecone-0.1.28a0/pynecone/style.py
+-rw-r--r--   0        0        0     2411 2023-03-10 00:25:42.708535 pynecone-0.1.28a0/pynecone/telemetry.py
+-rw-r--r--   0        0        0     4252 2023-04-27 23:08:51.381036 pynecone-0.1.28a0/pynecone/utils/build.py
+-rw-r--r--   0        0        0     1627 2023-03-16 23:52:12.749156 pynecone-0.1.28a0/pynecone/utils/console.py
+-rw-r--r--   0        0        0     3597 2023-04-27 23:08:51.381176 pynecone-0.1.28a0/pynecone/utils/exec.py
+-rw-r--r--   0        0        0    10780 2023-04-30 03:30:20.668233 pynecone-0.1.28a0/pynecone/utils/format.py
+-rw-r--r--   0        0        0      544 2023-03-16 23:52:12.757094 pynecone-0.1.28a0/pynecone/utils/imports.py
+-rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.28a0/pynecone/utils/path_ops.py
+-rw-r--r--   0        0        0     9121 2023-04-27 23:08:51.381523 pynecone-0.1.28a0/pynecone/utils/prerequisites.py
+-rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.28a0/pynecone/utils/processes.py
+-rw-r--r--   0        0        0     4299 2023-03-16 23:52:12.757408 pynecone-0.1.28a0/pynecone/utils/types.py
+-rw-r--r--   0        0        0    26077 2023-04-30 03:30:20.668414 pynecone-0.1.28a0/pynecone/var.py
+-rw-r--r--   0        0        0     2634 2023-03-13 04:10:28.761553 pynecone-0.1.28a0/pynecone/watch.py
+-rw-r--r--   0        0        0     1758 2023-05-01 17:34:39.608453 pynecone-0.1.28a0/pyproject.toml
+-rw-r--r--   0        0        0     9379 1970-01-01 00:00:00.000000 pynecone-0.1.28a0/PKG-INFO
```

### Comparing `pynecone-0.1.27a2/LICENSE` & `pynecone-0.1.28a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/README.md` & `pynecone-0.1.28a0/README.md`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/.templates/apps/counter/counter.py` & `pynecone-0.1.28a0/pynecone/.templates/apps/counter/counter.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/.templates/apps/default/default.py` & `pynecone-0.1.28a0/pynecone/.templates/apps/default/default.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/.templates/assets/favicon.ico` & `pynecone-0.1.28a0/pynecone/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/.templates/web/bun.lockb` & `pynecone-0.1.28a0/pynecone/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/.templates/web/package.json` & `pynecone-0.1.28a0/pynecone/.templates/web/package.json`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/.templates/web/pages/_app.js` & `pynecone-0.1.28a0/pynecone/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/.templates/web/styles/code/prism.js` & `pynecone-0.1.28a0/pynecone/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/.templates/web/utils/state.js` & `pynecone-0.1.28a0/pynecone/.templates/web/utils/state.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -86,14 +86,19 @@
     }
 
     if (event.name == "_alert") {
         alert(event.payload.message);
         return false;
     }
 
+    if (event.name == "_set_value") {
+        event.payload.ref.current.value = event.payload.value;
+        return false;
+    }
+
     // Send the event to the server.
     event.token = getToken();
     event.router_data = (({
         pathname,
         query
     }) => ({
         pathname,
```

### Comparing `pynecone-0.1.27a2/pynecone/__init__.py` & `pynecone-0.1.28a0/pynecone/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from .config import Config, DBConfig
 from .constants import Env, Transports
 from .event import (
     EVENT_ARG,
     EventChain,
     console_log,
     redirect,
+    set_value,
     window_alert,
 )
 from .event import FileUpload as upload_files
 from .middleware import Middleware
 from .model import Model, session
 from .route import route
 from .state import ComputedVar as var
```

### Comparing `pynecone-0.1.27a2/pynecone/app.py` & `pynecone-0.1.28a0/pynecone/app.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/base.py` & `pynecone-0.1.28a0/pynecone/base.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/compiler/compiler.py` & `pynecone-0.1.28a0/pynecone/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/compiler/templates.py` & `pynecone-0.1.28a0/pynecone/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/compiler/utils.py` & `pynecone-0.1.28a0/pynecone/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/__init__.py` & `pynecone-0.1.28a0/pynecone/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/base/bare.py` & `pynecone-0.1.28a0/pynecone/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/base/document.py` & `pynecone-0.1.28a0/pynecone/components/base/document.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/base/link.py` & `pynecone-0.1.28a0/pynecone/components/base/link.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/base/meta.py` & `pynecone-0.1.28a0/pynecone/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/component.py` & `pynecone-0.1.28a0/pynecone/components/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
     ) -> Union[EventChain, Var]:
         """Create an event chain from a variety of input types.
 
         Args:
             event_trigger: The event trigger to bind the chain to.
             value: The value to create the event chain from.
             state_name: The state to be fully controlled.
-            full_control: Whether full contorolled or not.
+            full_control: Whether full controlled or not.
 
         Returns:
             The event chain.
 
         Raises:
             ValueError: If the value is not a valid event chain.
         """
@@ -239,15 +239,15 @@
             raise ValueError(f"Invalid event chain: {value}")
 
         # Add args to the event specs if necessary.
         if is_controlled_event:
             events = [
                 EventSpec(
                     handler=e.handler,
-                    local_args=(EVENT_ARG.name,),
+                    local_args=(EVENT_ARG,),
                     args=get_handler_args(e, arg),
                 )
                 for e in events
             ]
 
         # set state name when fully controlled input
         state_name = state_name if full_control else ""
@@ -457,18 +457,26 @@
             The import dict with the required imports.
         """
         return imports.merge_imports(
             self._get_imports(), *[child.get_imports() for child in self.children]
         )
 
     def _get_hooks(self) -> Optional[str]:
+        """Get the React hooks for this component.
+
+        Returns:
+            The hooks for just this component.
+        """
+        ref = self.get_ref()
+        if ref is not None:
+            return f"const {ref} = useRef(null);"
         return None
 
     def get_hooks(self) -> Set[str]:
-        """Get javascript code for react hooks.
+        """Get the React hooks for this component and its children.
 
         Returns:
             The code that should appear just before returning the rendered component.
         """
         # Store the code in a set to avoid duplicates.
         code = set()
 
@@ -479,14 +487,24 @@
 
         # Add the hook code for the children.
         for child in self.children:
             code.update(child.get_hooks())
 
         return code
 
+    def get_ref(self) -> Optional[str]:
+        """Get the name of the ref for the component.
+
+        Returns:
+            The ref name.
+        """
+        if self.id is None:
+            return None
+        return format.format_ref(self.id)
+
     def get_custom_components(
         self, seen: Optional[Set[str]] = None
     ) -> Set[CustomComponent]:
         """Get all the custom components used by the component.
 
         Args:
             seen: The tags of the components that have already been seen.
```

### Comparing `pynecone-0.1.27a2/pynecone/components/datadisplay/code.py` & `pynecone-0.1.28a0/pynecone/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/datadisplay/datatable.py` & `pynecone-0.1.28a0/pynecone/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/datadisplay/divider.py` & `pynecone-0.1.28a0/pynecone/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/datadisplay/list.py` & `pynecone-0.1.28a0/pynecone/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/datadisplay/stat.py` & `pynecone-0.1.28a0/pynecone/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/datadisplay/table.py` & `pynecone-0.1.28a0/pynecone/components/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/disclosure/accordion.py` & `pynecone-0.1.28a0/pynecone/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/disclosure/tabs.py` & `pynecone-0.1.28a0/pynecone/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/feedback/alert.py` & `pynecone-0.1.28a0/pynecone/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/feedback/circularprogress.py` & `pynecone-0.1.28a0/pynecone/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/feedback/progress.py` & `pynecone-0.1.28a0/pynecone/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/feedback/skeleton.py` & `pynecone-0.1.28a0/pynecone/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/feedback/spinner.py` & `pynecone-0.1.28a0/pynecone/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/forms/__init__.py` & `pynecone-0.1.28a0/pynecone/components/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/forms/button.py` & `pynecone-0.1.28a0/pynecone/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/forms/checkbox.py` & `pynecone-0.1.28a0/pynecone/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/forms/copytoclipboard.py` & `pynecone-0.1.28a0/pynecone/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/forms/editable.py` & `pynecone-0.1.28a0/pynecone/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/forms/formcontrol.py` & `pynecone-0.1.28a0/pynecone/components/forms/formcontrol.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/forms/iconbutton.py` & `pynecone-0.1.28a0/pynecone/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/forms/input.py` & `pynecone-0.1.28a0/pynecone/components/forms/input.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """An input component."""
 
 from typing import Dict
 
 from pynecone.components.component import EVENT_ARG
 from pynecone.components.libs.chakra import ChakraComponent
+from pynecone.utils import imports
 from pynecone.var import Var
 
 
 class Input(ChakraComponent):
     """The Input component is a component that is used to get user input in a text field."""
 
     tag = "Input"
@@ -44,14 +45,20 @@
 
     # "outline" | "filled" | "flushed" | "unstyled"
     variant: Var[str]
 
     # "lg" | "md" | "sm" | "xs"
     size: Var[str]
 
+    def _get_imports(self) -> imports.ImportDict:
+        return imports.merge_imports(
+            super()._get_imports(),
+            {"/utils/state": {"set_val"}},
+        )
+
     @classmethod
     def get_controlled_triggers(cls) -> Dict[str, Var]:
         """Get the event triggers that pass the component's value to the handler.
 
         Returns:
             A dict mapping the event trigger to the var that is passed to the handler.
         """
@@ -59,14 +66,21 @@
             "on_change": EVENT_ARG.target.value,
             "on_focus": EVENT_ARG.target.value,
             "on_blur": EVENT_ARG.target.value,
             "on_key_down": EVENT_ARG.key,
             "on_key_up": EVENT_ARG.key,
         }
 
+    def _render(self):
+        out = super()._render()
+        ref = self.get_ref()
+        if ref is not None:
+            out.add_props(ref=Var.create(ref, is_local=False))
+        return out
+
 
 class InputGroup(ChakraComponent):
     """The InputGroup component is a component that is used to group a set of inputs."""
 
     tag = "InputGroup"
```

### Comparing `pynecone-0.1.27a2/pynecone/components/forms/numberinput.py` & `pynecone-0.1.28a0/pynecone/components/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/forms/pininput.py` & `pynecone-0.1.28a0/pynecone/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/forms/radio.py` & `pynecone-0.1.28a0/pynecone/components/forms/radio.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/forms/rangeslider.py` & `pynecone-0.1.28a0/pynecone/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/forms/select.py` & `pynecone-0.1.28a0/pynecone/components/forms/select.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/forms/slider.py` & `pynecone-0.1.28a0/pynecone/components/forms/slider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/forms/switch.py` & `pynecone-0.1.28a0/pynecone/components/forms/switch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/forms/textarea.py` & `pynecone-0.1.28a0/pynecone/components/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/forms/upload.py` & `pynecone-0.1.28a0/pynecone/components/forms/upload.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/graphing/plotly.py` & `pynecone-0.1.28a0/pynecone/components/graphing/plotly.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/graphing/victory.py` & `pynecone-0.1.28a0/pynecone/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/layout/__init__.py` & `pynecone-0.1.28a0/pynecone/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/layout/box.py` & `pynecone-0.1.28a0/pynecone/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/layout/cond.py` & `pynecone-0.1.28a0/pynecone/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/layout/flex.py` & `pynecone-0.1.28a0/pynecone/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/layout/foreach.py` & `pynecone-0.1.28a0/pynecone/components/layout/foreach.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/layout/grid.py` & `pynecone-0.1.28a0/pynecone/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/layout/html.py` & `pynecone-0.1.28a0/pynecone/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/layout/responsive.py` & `pynecone-0.1.28a0/pynecone/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/layout/stack.py` & `pynecone-0.1.28a0/pynecone/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/layout/wrap.py` & `pynecone-0.1.28a0/pynecone/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/media/avatar.py` & `pynecone-0.1.28a0/pynecone/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/media/icon.py` & `pynecone-0.1.28a0/pynecone/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/media/image.py` & `pynecone-0.1.28a0/pynecone/components/media/image.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/navigation/breadcrumb.py` & `pynecone-0.1.28a0/pynecone/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/navigation/link.py` & `pynecone-0.1.28a0/pynecone/components/navigation/link.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/navigation/linkoverlay.py` & `pynecone-0.1.28a0/pynecone/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/overlay/__init__.py` & `pynecone-0.1.28a0/pynecone/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/overlay/alertdialog.py` & `pynecone-0.1.28a0/pynecone/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/overlay/drawer.py` & `pynecone-0.1.28a0/pynecone/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/overlay/menu.py` & `pynecone-0.1.28a0/pynecone/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/overlay/modal.py` & `pynecone-0.1.28a0/pynecone/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/overlay/popover.py` & `pynecone-0.1.28a0/pynecone/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/overlay/tooltip.py` & `pynecone-0.1.28a0/pynecone/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/tags/cond_tag.py` & `pynecone-0.1.28a0/pynecone/components/tags/cond_tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/tags/iter_tag.py` & `pynecone-0.1.28a0/pynecone/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/tags/tag.py` & `pynecone-0.1.28a0/pynecone/components/tags/tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                 return str(prop)
             if types._issubclass(prop.type_, str):
                 return format.json_dumps(prop.full_name)
             prop = prop.full_name
 
         # Handle event props.
         elif isinstance(prop, EventChain):
-            local_args = ",".join(prop.events[0].local_args)
+            local_args = ",".join(([str(a) for a in prop.events[0].local_args]))
 
             if len(prop.events) == 1 and prop.events[0].upload:
                 # Special case for upload events.
                 event = format.format_upload_event(prop.events[0])
             elif prop.full_control:
                 # Full control component events.
                 event = format.format_full_control_event(prop)
```

### Comparing `pynecone-0.1.27a2/pynecone/components/tags/tagless.py` & `pynecone-0.1.28a0/pynecone/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/components/typography/markdown.py` & `pynecone-0.1.28a0/pynecone/components/typography/markdown.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/config.py` & `pynecone-0.1.28a0/pynecone/config.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/constants.py` & `pynecone-0.1.28a0/pynecone/constants.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/el/constants/html.py` & `pynecone-0.1.28a0/pynecone/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/el/constants/pynecone.py` & `pynecone-0.1.28a0/pynecone/el/constants/pynecone.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/el/constants/react.py` & `pynecone-0.1.28a0/pynecone/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/el/element.py` & `pynecone-0.1.28a0/pynecone/el/element.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/el/elements/__init__.py` & `pynecone-0.1.28a0/pynecone/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/el/precompile.py` & `pynecone-0.1.28a0/pynecone/el/precompile.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/event.py` & `pynecone-0.1.28a0/pynecone/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     # The event name.
     name: str
 
     # The routing data where event occurred
     router_data: Dict[str, Any] = {}
 
     # The event payload.
-    payload: Dict[str, Any] = {}
+    payload: Dict[Any, Any] = {}
 
 
 class EventHandler(Base):
     """An event handler responds to an event to update the state."""
 
     # The function to call in response to the event.
     fn: Callable
@@ -50,29 +50,26 @@
             The event spec, containing both the function and args.
 
         Raises:
             TypeError: If the arguments are invalid.
         """
         # Get the function args.
         fn_args = inspect.getfullargspec(self.fn).args[1:]
+        fn_args = (Var.create_safe(arg) for arg in fn_args)
 
         # Construct the payload.
         values = []
         for arg in args:
-            # If it is a Var, add the full name.
-            if isinstance(arg, Var):
-                values.append(arg.full_name)
-                continue
-
+            # Special case for file uploads.
             if isinstance(arg, FileUpload):
                 return EventSpec(handler=self, upload=True)
 
             # Otherwise, convert to JSON.
             try:
-                values.append(format.json_dumps(arg))
+                values.append(Var.create(arg))
             except TypeError as e:
                 raise TypeError(
                     f"Arguments to event handlers must be Vars or JSON-serializable. Got {arg} of type {type(arg)}."
                 ) from e
         payload = tuple(zip(fn_args, values))
 
         # Return the event spec.
@@ -86,18 +83,18 @@
     during compile time to outline the structure of an event.
     """
 
     # The event handler.
     handler: EventHandler
 
     # The local arguments on the frontend.
-    local_args: Tuple[str, ...] = ()
+    local_args: Tuple[Var, ...] = ()
 
     # The arguments to pass to the function.
-    args: Tuple[Any, ...] = ()
+    args: Tuple[Tuple[Var, Var], ...] = ()
 
     # Whether to upload files.
     upload: bool = False
 
     class Config:
         """The Pydantic config."""
 
@@ -138,71 +135,86 @@
 class FileUpload(Base):
     """Class to represent a file upload."""
 
     pass
 
 
 # Special server-side events.
-def redirect(path: str) -> EventSpec:
-    """Redirect to a new path.
+def server_side(name: str, **kwargs) -> EventSpec:
+    """A server-side event.
 
     Args:
-        path: The path to redirect to.
+        name: The name of the event.
+        **kwargs: The arguments to pass to the event.
 
     Returns:
-        An event to redirect to the path.
+        An event spec for a server-side event.
     """
 
     def fn():
         return None
 
-    fn.__qualname__ = "_redirect"
+    fn.__qualname__ = name
     return EventSpec(
         handler=EventHandler(fn=fn),
-        args=(("path", path),),
+        args=tuple(
+            (Var.create_safe(k), Var.create_safe(v, is_string=type(v) is str))
+            for k, v in kwargs.items()
+        ),
     )
 
 
-def console_log(message: str) -> EventSpec:
+def redirect(path: Union[str, Var[str]]) -> EventSpec:
+    """Redirect to a new path.
+
+    Args:
+        path: The path to redirect to.
+
+    Returns:
+        An event to redirect to the path.
+    """
+    return server_side("_redirect", path=path)
+
+
+def console_log(message: Union[str, Var[str]]) -> EventSpec:
     """Do a console.log on the browser.
 
     Args:
         message: The message to log.
 
     Returns:
         An event to log the message.
     """
+    return server_side("_console", message=message)
 
-    def fn():
-        return None
 
-    fn.__qualname__ = "_console"
-    return EventSpec(
-        handler=EventHandler(fn=fn),
-        args=(("message", message),),
-    )
-
-
-def window_alert(message: str) -> EventSpec:
+def window_alert(message: Union[str, Var[str]]) -> EventSpec:
     """Create a window alert on the browser.
 
     Args:
         message: The message to alert.
 
     Returns:
         An event to alert the message.
     """
+    return server_side("_alert", message=message)
 
-    def fn():
-        return None
 
-    fn.__qualname__ = "_alert"
-    return EventSpec(
-        handler=EventHandler(fn=fn),
-        args=(("message", message),),
+def set_value(ref: str, value: Any) -> EventSpec:
+    """Set the value of a ref.
+
+    Args:
+        ref: The ref.
+        value: The value to set.
+
+    Returns:
+        An event to set the ref.
+    """
+    return server_side(
+        "_set_value", ref=Var.create_safe(format.format_ref(ref)), value=value
     )
 
 
 def get_event(state, event):
     """Get the event from the given state.
 
     Args:
@@ -302,15 +314,15 @@
         # Add the event spec to the chain.
         events.append(e)
 
     # Return the events.
     return events
 
 
-def get_handler_args(event_spec: EventSpec, arg: Var) -> Tuple[Tuple[str, str], ...]:
+def get_handler_args(event_spec: EventSpec, arg: Var) -> Tuple[Tuple[Var, Var], ...]:
     """Get the handler args for the given event spec.
 
     Args:
         event_spec: The event spec.
         arg: The controlled event argument.
 
     Returns:
@@ -320,31 +332,29 @@
         ValueError: If the event handler has an invalid signature.
     """
     args = inspect.getfullargspec(event_spec.handler.fn).args
     if len(args) < 2:
         raise ValueError(
             f"Event handler has an invalid signature, needed a method with a parameter, got {event_spec.handler}."
         )
-    return event_spec.args if len(args) > 2 else ((args[1], arg.name),)
+    return event_spec.args if len(args) > 2 else ((Var.create_safe(args[1]), arg),)
 
 
 def fix_events(
     events: Optional[List[Union[EventHandler, EventSpec]]], token: str
 ) -> List[Event]:
     """Fix a list of events returned by an event handler.
 
     Args:
         events: The events to fix.
         token: The user token.
 
     Returns:
         The fixed events.
     """
-    from pynecone.event import Event, EventHandler, EventSpec
-
     # If the event handler returns nothing, return an empty list.
     if events is None:
         return []
 
     # If the handler returns a single event, wrap it in a list.
     if not isinstance(events, List):
         events = [events]
@@ -355,15 +365,15 @@
         if not isinstance(e, (EventHandler, EventSpec)):
             e = EventHandler(fn=e)
         # Otherwise, create an event from the event spec.
         if isinstance(e, EventHandler):
             e = e()
         assert isinstance(e, EventSpec), f"Unexpected event type, {type(e)}."
         name = format.format_event_handler(e.handler)
-        payload = dict(e.args)
+        payload = {k.name: v.name for k, v in e.args}
 
         # Create an event and append it to the list.
         out.append(
             Event(
                 token=token,
                 name=name,
                 payload=payload,
```

### Comparing `pynecone-0.1.27a2/pynecone/middleware/hydrate_middleware.py` & `pynecone-0.1.28a0/pynecone/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/middleware/logging_middleware.py` & `pynecone-0.1.28a0/pynecone/middleware/logging_middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/middleware/middleware.py` & `pynecone-0.1.28a0/pynecone/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/model.py` & `pynecone-0.1.28a0/pynecone/model.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/pc.py` & `pynecone-0.1.28a0/pynecone/pc.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/route.py` & `pynecone-0.1.28a0/pynecone/route.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/state.py` & `pynecone-0.1.28a0/pynecone/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,17 @@
 
         # Setup the substates.
         for substate in self.get_substates():
             self.substates[substate.get_name()] = substate(parent_state=self)
 
         # Convert the event handlers to functions.
         for name, event_handler in self.event_handlers.items():
-            setattr(self, name, event_handler.fn)
+            fn = functools.partial(event_handler.fn, self)
+            fn.__qualname__ = event_handler.fn.__qualname__  # type: ignore
+            setattr(self, name, fn)
 
         # Initialize the mutable fields.
         self._init_mutable_fields()
 
         # Initialize computed vars dependencies.
         self.computed_var_dependencies = defaultdict(set)
         for cvar in self.computed_vars:
```

### Comparing `pynecone-0.1.27a2/pynecone/style.py` & `pynecone-0.1.28a0/pynecone/style.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/telemetry.py` & `pynecone-0.1.28a0/pynecone/telemetry.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/utils/build.py` & `pynecone-0.1.28a0/pynecone/utils/build.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/utils/console.py` & `pynecone-0.1.28a0/pynecone/utils/console.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/utils/exec.py` & `pynecone-0.1.28a0/pynecone/utils/exec.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/utils/format.py` & `pynecone-0.1.28a0/pynecone/utils/format.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,15 +282,20 @@
 
     Args:
         event_spec: The event to format.
 
     Returns:
         The compiled event.
     """
-    args = ",".join([":".join((name, val)) for name, val in event_spec.args])
+    args = ",".join(
+        [
+            ":".join((name.name, json.dumps(val.name) if val.is_string else val.name))
+            for name, val in event_spec.args
+        ]
+    )
     return f"E(\"{format_event_handler(event_spec.handler)}\", {wrap(args, '{')})"
 
 
 def format_upload_event(event_spec: EventSpec) -> str:
     """Format an upload event.
 
     Args:
@@ -394,14 +399,28 @@
     raise TypeError(
         "State vars must be primitive Python types, "
         "or subclasses of pc.Base. "
         f"Got var of type {type(value)}."
     )
 
 
+def format_ref(ref: str) -> str:
+    """Format a ref.
+
+    Args:
+        ref: The ref to format.
+
+    Returns:
+        The formatted ref.
+    """
+    # Replace all non-word characters with underscores.
+    clean_ref = re.sub(r"[^\w]+", "_", ref)
+    return f"ref_{clean_ref}"
+
+
 def json_dumps(obj: Any) -> str:
     """Takes an object and returns a jsonified string.
 
     Args:
         obj: The object to be serialized.
 
     Returns:
```

### Comparing `pynecone-0.1.27a2/pynecone/utils/imports.py` & `pynecone-0.1.28a0/pynecone/utils/imports.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/utils/path_ops.py` & `pynecone-0.1.28a0/pynecone/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/utils/prerequisites.py` & `pynecone-0.1.28a0/pynecone/utils/prerequisites.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/utils/processes.py` & `pynecone-0.1.28a0/pynecone/utils/processes.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/utils/types.py` & `pynecone-0.1.28a0/pynecone/utils/types.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pynecone/var.py` & `pynecone-0.1.28a0/pynecone/var.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,32 @@
             raise TypeError(
                 f"To create a Var must be Var or JSON-serializable. Got {value} of type {type(value)}."
             ) from e
 
         return BaseVar(name=name, type_=type_, is_local=is_local, is_string=is_string)
 
     @classmethod
+    def create_safe(
+        cls, value: Any, is_local: bool = True, is_string: bool = False
+    ) -> Var:
+        """Create a var from a value, guaranteeing that it is not None.
+
+        Args:
+            value: The value to create the var from.
+            is_local: Whether the var is local.
+            is_string: Whether the var is a string literal.
+
+        Returns:
+            The var.
+        """
+        var = cls.create(value, is_local=is_local, is_string=is_string)
+        assert var is not None
+        return var
+
+    @classmethod
     def __class_getitem__(cls, type_: str) -> _GenericAlias:
         """Get a typed var.
 
         Args:
             type_: The type of the var.
 
         Returns:
```

### Comparing `pynecone-0.1.27a2/pynecone/watch.py` & `pynecone-0.1.28a0/pynecone/watch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.27a2/pyproject.toml` & `pynecone-0.1.28a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynecone"
-version = "0.1.27a2"
+version = "0.1.28a0"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
```

### Comparing `pynecone-0.1.27a2/PKG-INFO` & `pynecone-0.1.28a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynecone
-Version: 0.1.27a2
+Version: 0.1.28a0
 Summary: Web apps in pure Python.
 Home-page: https://pynecone.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
```

