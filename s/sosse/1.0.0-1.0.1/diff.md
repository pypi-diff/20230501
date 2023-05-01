# Comparing `tmp/sosse-1.0.0.tar.gz` & `tmp/sosse-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosse-1.0.0.tar", last modified: Sun Apr 30 18:45:04 2023, max compression
+gzip compressed data, was "sosse-1.0.1.tar", last modified: Mon May  1 14:24:43 2023, max compression
```

## Comparing `sosse-1.0.0.tar` & `sosse-1.0.1.tar`

### file list

```diff
@@ -1,215 +1,222 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.494634 sosse-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-04-30 18:44:36.000000 sosse-1.0.0/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-04-30 18:44:36.000000 sosse-1.0.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     6363 2023-04-30 18:44:36.000000 sosse-1.0.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      491 2023-04-30 18:44:36.000000 sosse-1.0.0/.readthedocs.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1529 2023-04-30 18:44:36.000000 sosse-1.0.0/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)    34523 2023-04-30 18:44:36.000000 sosse-1.0.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-30 18:44:36.000000 sosse-1.0.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     6921 2023-04-30 18:44:36.000000 sosse-1.0.0/Makefile
--rw-r--r--   0 root         (0) root         (0)     3114 2023-04-30 18:45:04.494634 sosse-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2722 2023-04-30 18:44:36.000000 sosse-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.390636 sosse-1.0.0/debian/
--rw-rw-rw-   0 root         (0) root         (0)      141 2023-04-30 18:44:36.000000 sosse-1.0.0/debian/changelog
--rw-rw-rw-   0 root         (0) root         (0)        3 2023-04-30 18:44:36.000000 sosse-1.0.0/debian/compat
--rw-rw-rw-   0 root         (0) root         (0)      710 2023-04-30 18:44:36.000000 sosse-1.0.0/debian/control
--rwxrwxrwx   0 root         (0) root         (0)      182 2023-04-30 18:44:36.000000 sosse-1.0.0/debian/rules
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-04-30 18:44:36.000000 sosse-1.0.0/debian/sosse-crawler.service
--rw-rw-rw-   0 root         (0) root         (0)      803 2023-04-30 18:44:36.000000 sosse-1.0.0/debian/sosse-uwsgi.service
--rw-rw-rw-   0 root         (0) root         (0)     2176 2023-04-30 18:44:36.000000 sosse-1.0.0/debian/sosse.conf
--rw-rw-rw-   0 root         (0) root         (0)      196 2023-04-30 18:44:36.000000 sosse-1.0.0/debian/sosse.install
--rw-rw-rw-   0 root         (0) root         (0)     2733 2023-04-30 18:44:36.000000 sosse-1.0.0/debian/sosse.postinst
--rw-rw-rw-   0 root         (0) root         (0)      465 2023-04-30 18:44:36.000000 sosse-1.0.0/debian/uwsgi.ini
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-04-30 18:44:36.000000 sosse-1.0.0/debian/uwsgi.params
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.394636 sosse-1.0.0/doc/
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     1897 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/get_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.402636 sosse-1.0.0/doc/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.402636 sosse-1.0.0/doc/source/_extensions/
--rw-rw-rw-   0 root         (0) root         (0)     1124 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/_extensions/code_blocks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.406636 sosse-1.0.0/doc/source/_static/
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/_static/style.css
--rw-rw-rw-   0 root         (0) root         (0)      723 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/admin_ui.rst
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/administration.rst
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/authentication.rst
--rw-rw-rw-   0 root         (0) root         (0)      433 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/cli.rst
--rw-rw-rw-   0 root         (0) root         (0)     1860 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/config_file.rst
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/cookies.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.406636 sosse-1.0.0/doc/source/crawl/
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/crawl/add_to_queue.rst
--rw-rw-rw-   0 root         (0) root         (0)     1452 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/crawl/crawl_depth.rst
--rw-rw-rw-   0 root         (0) root         (0)     5773 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/crawl/policies.rst
--rw-rw-rw-   0 root         (0) root         (0)      316 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/crawl/status.rst
--rw-rw-rw-   0 root         (0) root         (0)     1210 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/documents.rst
--rw-rw-rw-   0 root         (0) root         (0)     1408 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/domain_settings.rst
--rw-rw-rw-   0 root         (0) root         (0)      315 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/excluded_urls.rst
--rw-rw-rw-   0 root         (0) root         (0)      510 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.410636 sosse-1.0.0/doc/source/install/
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/install/database.rst
--rw-rw-rw-   0 root         (0) root         (0)     1832 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/install/debian.rst
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/install/debian_upgrades.rst
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/install/docker.rst
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/install/docker_upgrades.rst
--rw-rw-rw-   0 root         (0) root         (0)     3287 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/install/pip.rst
--rw-rw-rw-   0 root         (0) root         (0)      450 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/install/pip_upgrades.rst
--rw-rw-rw-   0 root         (0) root         (0)      287 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/install.rst
--rw-rw-rw-   0 root         (0) root         (0)      988 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/permissions.rst
--rw-rw-rw-   0 root         (0) root         (0)      989 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/screenshots.rst
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/search_engines.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.414636 sosse-1.0.0/doc/source/user/
--rw-rw-rw-   0 root         (0) root         (0)      823 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/user/cached.rst
--rw-rw-rw-   0 root         (0) root         (0)      593 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/user/history.rst
--rw-rw-rw-   0 root         (0) root         (0)     1407 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/user/preferences.rst
--rw-rw-rw-   0 root         (0) root         (0)     4293 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/user/search.rst
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/user/shortcut_list.rst
--rw-rw-rw-   0 root         (0) root         (0)     1043 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/user/shortcuts.rst
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/user/statistics.rst
--rw-rw-rw-   0 root         (0) root         (0)      245 2023-04-30 18:44:36.000000 sosse-1.0.0/doc/source/user_doc.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.418635 sosse-1.0.0/docker/
--rw-rw-rw-   0 root         (0) root         (0)      761 2023-04-30 18:44:36.000000 sosse-1.0.0/docker/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      334 2023-04-30 18:44:36.000000 sosse-1.0.0/docker/Makefile.common
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.418635 sosse-1.0.0/docker/debian/
--rw-rw-rw-   0 root         (0) root         (0)     2128 2023-04-30 18:44:36.000000 sosse-1.0.0/docker/debian/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-04-30 18:44:36.000000 sosse-1.0.0/docker/debian/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.418635 sosse-1.0.0/docker/debian-pkg/
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-04-30 18:44:36.000000 sosse-1.0.0/docker/debian-pkg/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-30 18:44:36.000000 sosse-1.0.0/docker/debian-pkg/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.422635 sosse-1.0.0/docker/debian-test/
--rw-rw-rw-   0 root         (0) root         (0)     1166 2023-04-30 18:44:36.000000 sosse-1.0.0/docker/debian-test/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-04-30 18:44:36.000000 sosse-1.0.0/docker/debian-test/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.422635 sosse-1.0.0/docker/doc/
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-30 18:44:36.000000 sosse-1.0.0/docker/doc/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-30 18:44:36.000000 sosse-1.0.0/docker/doc/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.422635 sosse-1.0.0/docker/pip-base/
--rw-rw-rw-   0 root         (0) root         (0)      442 2023-04-30 18:44:36.000000 sosse-1.0.0/docker/pip-base/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-30 18:44:36.000000 sosse-1.0.0/docker/pip-base/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.426635 sosse-1.0.0/docker/pip-test/
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-04-30 18:44:36.000000 sosse-1.0.0/docker/pip-test/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-30 18:44:36.000000 sosse-1.0.0/docker/pip-test/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      892 2023-04-30 18:44:36.000000 sosse-1.0.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-04-30 18:44:36.000000 sosse-1.0.0/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.438635 sosse-1.0.0/se/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 18:44:36.000000 sosse-1.0.0/se/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20299 2023-04-30 18:44:36.000000 sosse-1.0.0/se/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      996 2023-04-30 18:44:36.000000 sosse-1.0.0/se/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     4121 2023-04-30 18:44:36.000000 sosse-1.0.0/se/atom.py
--rw-rw-rw-   0 root         (0) root         (0)    24133 2023-04-30 18:44:36.000000 sosse-1.0.0/se/browser.py
--rw-rw-rw-   0 root         (0) root         (0)     2804 2023-04-30 18:44:36.000000 sosse-1.0.0/se/cached.py
--rw-rw-rw-   0 root         (0) root         (0)     4314 2023-04-30 18:44:36.000000 sosse-1.0.0/se/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     1150 2023-04-30 18:44:36.000000 sosse-1.0.0/se/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.442635 sosse-1.0.0/se/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 18:44:36.000000 sosse-1.0.0/se/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.446635 sosse-1.0.0/se/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 18:44:36.000000 sosse-1.0.0/se/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4311 2023-04-30 18:44:36.000000 sosse-1.0.0/se/management/commands/crawl.py
--rw-rw-rw-   0 root         (0) root         (0)     1427 2023-04-30 18:44:36.000000 sosse-1.0.0/se/management/commands/default_admin.py
--rw-rw-rw-   0 root         (0) root         (0)      952 2023-04-30 18:44:36.000000 sosse-1.0.0/se/management/commands/default_conf.py
--rw-rw-rw-   0 root         (0) root         (0)     6143 2023-04-30 18:44:36.000000 sosse-1.0.0/se/management/commands/extract_doc.py
--rw-rw-rw-   0 root         (0) root         (0)     1275 2023-04-30 18:44:36.000000 sosse-1.0.0/se/management/commands/generate_secret.py
--rw-rw-rw-   0 root         (0) root         (0)     1746 2023-04-30 18:44:36.000000 sosse-1.0.0/se/management/commands/load_se.py
--rw-rw-rw-   0 root         (0) root         (0)     2150 2023-04-30 18:44:36.000000 sosse-1.0.0/se/management/commands/update_se.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.446635 sosse-1.0.0/se/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    13998 2023-04-30 18:39:24.000000 sosse-1.0.0/se/migrations/0001_initial.py
--rwxrwxrwx   0 root         (0) root         (0)     2976 2023-04-30 18:39:24.000000 sosse-1.0.0/se/migrations/0002_search_vector.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 18:39:24.000000 sosse-1.0.0/se/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    55276 2023-04-30 18:44:36.000000 sosse-1.0.0/se/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1941 2023-04-30 18:44:36.000000 sosse-1.0.0/se/screenshot.py
--rw-rw-rw-   0 root         (0) root         (0)     6607 2023-04-30 18:44:36.000000 sosse-1.0.0/se/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.370637 sosse-1.0.0/se/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.454635 sosse-1.0.0/se/static/se/
--rw-rw-rw-   0 root         (0) root         (0)    19511 2023-04-30 18:44:36.000000 sosse-1.0.0/se/static/se/admin-base.css
--rw-rw-rw-   0 root         (0) root         (0)     8810 2023-04-30 18:44:36.000000 sosse-1.0.0/se/static/se/admin-forms.css
--rw-rw-rw-   0 root         (0) root         (0)     2005 2023-04-30 18:44:36.000000 sosse-1.0.0/se/static/se/base.js
--rw-rw-rw-   0 root         (0) root         (0)     2435 2023-04-30 18:44:36.000000 sosse-1.0.0/se/static/se/icon-atom.svg
--rw-rw-rw-   0 root         (0) root         (0)     2196 2023-04-30 18:44:36.000000 sosse-1.0.0/se/static/se/icon-clear.svg
--rw-rw-rw-   0 root         (0) root         (0)     3722 2023-04-30 18:44:36.000000 sosse-1.0.0/se/static/se/icon-cog.svg
--rw-rw-rw-   0 root         (0) root         (0)     6887 2023-04-30 18:44:36.000000 sosse-1.0.0/se/static/se/icon-search.svg
--rw-rw-rw-   0 root         (0) root         (0)     2488 2023-04-30 18:44:36.000000 sosse-1.0.0/se/static/se/icon-stats.svg
--rw-rw-rw-   0 root         (0) root         (0)     3644 2023-04-30 18:44:36.000000 sosse-1.0.0/se/static/se/icon-trash.svg
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-04-30 18:44:36.000000 sosse-1.0.0/se/static/se/icon-user.svg
--rw-rw-rw-   0 root         (0) root         (0)     9798 2023-04-30 18:44:36.000000 sosse-1.0.0/se/static/se/index.js
--rw-rw-rw-   0 root         (0) root         (0)     4462 2023-04-30 18:44:36.000000 sosse-1.0.0/se/static/se/logo.png
--rw-rw-rw-   0 root         (0) root         (0)     9908 2023-04-30 18:44:36.000000 sosse-1.0.0/se/static/se/logo.svg
--rw-rw-rw-   0 root         (0) root         (0)     5967 2023-04-30 18:44:36.000000 sosse-1.0.0/se/static/se/pygal-tooltips.min.js
--rw-rw-rw-   0 root         (0) root         (0)      982 2023-04-30 18:44:36.000000 sosse-1.0.0/se/static/se/screenshot.js
--rw-rw-rw-   0 root         (0) root         (0)     2522 2023-04-30 18:44:36.000000 sosse-1.0.0/se/static/se/style.css
--rw-rw-rw-   0 root         (0) root         (0)     8567 2023-04-30 18:44:36.000000 sosse-1.0.0/se/stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.374637 sosse-1.0.0/se/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.458635 sosse-1.0.0/se/templates/admin/
--rw-rw-rw-   0 root         (0) root         (0)     3427 2023-04-30 18:44:36.000000 sosse-1.0.0/se/templates/admin/add_to_queue.html
--rw-rw-rw-   0 root         (0) root         (0)     2518 2023-04-30 18:44:36.000000 sosse-1.0.0/se/templates/admin/app_list.html
--rw-rw-rw-   0 root         (0) root         (0)     2270 2023-04-30 18:44:36.000000 sosse-1.0.0/se/templates/admin/base.html
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-04-30 18:44:36.000000 sosse-1.0.0/se/templates/admin/base_site.html
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-04-30 18:44:36.000000 sosse-1.0.0/se/templates/admin/change_form.html
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-04-30 18:44:36.000000 sosse-1.0.0/se/templates/admin/crawl_status.html
--rw-rw-rw-   0 root         (0) root         (0)     2706 2023-04-30 18:44:36.000000 sosse-1.0.0/se/templates/admin/crawl_status_content.html
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-30 18:44:36.000000 sosse-1.0.0/se/templates/admin/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.466634 sosse-1.0.0/se/templates/se/
--rw-rw-rw-   0 root         (0) root         (0)      661 2023-04-30 18:44:36.000000 sosse-1.0.0/se/templates/se/about.html
--rw-rw-rw-   0 root         (0) root         (0)     1473 2023-04-30 18:44:36.000000 sosse-1.0.0/se/templates/se/base.html
--rw-rw-rw-   0 root         (0) root         (0)     2285 2023-04-30 18:44:36.000000 sosse-1.0.0/se/templates/se/cached.html
--rw-rw-rw-   0 root         (0) root         (0)     1870 2023-04-30 18:44:36.000000 sosse-1.0.0/se/templates/se/history.html
--rw-rw-rw-   0 root         (0) root         (0)     8235 2023-04-30 18:44:36.000000 sosse-1.0.0/se/templates/se/index.html
--rw-rw-rw-   0 root         (0) root         (0)     1320 2023-04-30 18:44:36.000000 sosse-1.0.0/se/templates/se/main_menu.html
--rw-rw-rw-   0 root         (0) root         (0)      544 2023-04-30 18:44:36.000000 sosse-1.0.0/se/templates/se/opensearch.xml
--rw-rw-rw-   0 root         (0) root         (0)      761 2023-04-30 18:44:36.000000 sosse-1.0.0/se/templates/se/pagination.html
--rw-rw-rw-   0 root         (0) root         (0)     2242 2023-04-30 18:44:36.000000 sosse-1.0.0/se/templates/se/prefs.html
--rw-rw-rw-   0 root         (0) root         (0)     1706 2023-04-30 18:44:36.000000 sosse-1.0.0/se/templates/se/screenshot.html
--rw-rw-rw-   0 root         (0) root         (0)     1523 2023-04-30 18:44:36.000000 sosse-1.0.0/se/templates/se/search_redirect.html
--rw-rw-rw-   0 root         (0) root         (0)     1547 2023-04-30 18:44:36.000000 sosse-1.0.0/se/templates/se/stats.html
--rw-rw-rw-   0 root         (0) root         (0)      741 2023-04-30 18:44:36.000000 sosse-1.0.0/se/templates/se/unknown_url.html
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-04-30 18:44:36.000000 sosse-1.0.0/se/templates/se/words.html
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-04-30 18:44:36.000000 sosse-1.0.0/se/templates/se/www.html
--rw-rw-rw-   0 root         (0) root         (0)     5979 2023-04-30 18:44:36.000000 sosse-1.0.0/se/test_cookie.py
--rw-rw-rw-   0 root         (0) root         (0)    14144 2023-04-30 18:44:36.000000 sosse-1.0.0/se/test_crawl.py
--rw-rw-rw-   0 root         (0) root         (0)     9790 2023-04-30 18:44:36.000000 sosse-1.0.0/se/test_functionals.py
--rw-rw-rw-   0 root         (0) root         (0)     1459 2023-04-30 18:44:36.000000 sosse-1.0.0/se/test_misc.py
--rw-rw-rw-   0 root         (0) root         (0)     4659 2023-04-30 18:44:36.000000 sosse-1.0.0/se/test_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2133 2023-04-30 18:44:36.000000 sosse-1.0.0/se/test_redirect.py
--rw-rw-rw-   0 root         (0) root         (0)     1600 2023-04-30 18:44:36.000000 sosse-1.0.0/se/test_requests.py
--rw-rw-rw-   0 root         (0) root         (0)     9547 2023-04-30 18:44:36.000000 sosse-1.0.0/se/test_search.py
--rw-rw-rw-   0 root         (0) root         (0)     2612 2023-04-30 18:44:36.000000 sosse-1.0.0/se/test_url.py
--rw-rw-rw-   0 root         (0) root         (0)     6326 2023-04-30 18:44:36.000000 sosse-1.0.0/se/test_views.py
--rw-rw-rw-   0 root         (0) root         (0)     3101 2023-04-30 18:44:36.000000 sosse-1.0.0/se/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     8408 2023-04-30 18:44:36.000000 sosse-1.0.0/se/views.py
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-04-30 18:44:36.000000 sosse-1.0.0/se/words.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2023-04-30 18:44:36.000000 sosse-1.0.0/se/www.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-30 18:45:04.494634 sosse-1.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.478634 sosse-1.0.0/sosse/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-30 18:44:36.000000 sosse-1.0.0/sosse/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16555 2023-04-30 18:44:36.000000 sosse-1.0.0/sosse/conf.py
--rw-rw-rw-   0 root         (0) root         (0)    18193 2023-04-30 18:44:36.000000 sosse-1.0.0/sosse/search_engines.json
--rw-rw-rw-   0 root         (0) root         (0)     7433 2023-04-30 18:44:46.000000 sosse-1.0.0/sosse/settings.py
--rwxrwxrwx   0 root         (0) root         (0)     1328 2023-04-30 18:44:36.000000 sosse-1.0.0/sosse/sosse_admin.py
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-30 18:44:36.000000 sosse-1.0.0/sosse/test_runner.py
--rw-rw-rw-   0 root         (0) root         (0)     2548 2023-04-30 18:44:36.000000 sosse-1.0.0/sosse/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2023-04-30 18:44:36.000000 sosse-1.0.0/sosse/wsgi.py
--rwxrwxrwx   0 root         (0) root         (0)       70 2023-04-30 18:44:36.000000 sosse-1.0.0/sosse-admin
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.482634 sosse-1.0.0/sosse.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3114 2023-04-30 18:45:04.000000 sosse-1.0.0/sosse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4498 2023-04-30 18:45:04.000000 sosse-1.0.0/sosse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-30 18:45:04.000000 sosse-1.0.0/sosse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-04-30 18:45:04.000000 sosse-1.0.0/sosse.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      129 2023-04-30 18:45:04.000000 sosse-1.0.0/sosse.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-30 18:45:04.000000 sosse-1.0.0/sosse.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.486634 sosse-1.0.0/tests/
--rwxrwxrwx   0 root         (0) root         (0)      281 2023-04-30 18:44:36.000000 sosse-1.0.0/tests/build_doc.sh
--rw-rw-rw-   0 root         (0) root         (0)      809 2023-04-30 18:44:36.000000 sosse-1.0.0/tests/cookies.json
--rwxrwxrwx   0 root         (0) root         (0)     1047 2023-04-30 18:44:36.000000 sosse-1.0.0/tests/doc_test.sh
--rwxrwxrwx   0 root         (0) root         (0)      477 2023-04-30 18:44:36.000000 sosse-1.0.0/tests/docker_run.sh
--rw-rw-rw-   0 root         (0) root         (0)     1015 2023-04-30 18:44:36.000000 sosse-1.0.0/tests/document-ja.json
--rw-rw-rw-   0 root         (0) root         (0)      496 2023-04-30 18:44:36.000000 sosse-1.0.0/tests/opensearch.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.490634 sosse-1.0.0/tests/robotframework/
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-04-30 18:44:36.000000 sosse-1.0.0/tests/robotframework/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)      605 2023-04-30 18:44:36.000000 sosse-1.0.0/tests/robotframework/start.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-30 18:45:04.494634 sosse-1.0.0/tests/robotframework/tests/
--rw-rw-rw-   0 root         (0) root         (0)     5208 2023-04-30 18:44:36.000000 sosse-1.0.0/tests/robotframework/tests/01_crawl.robot
--rw-rw-rw-   0 root         (0) root         (0)     2862 2023-04-30 18:44:36.000000 sosse-1.0.0/tests/robotframework/tests/02_user.robot
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-04-30 18:44:36.000000 sosse-1.0.0/tests/robotframework/tests/__init__.robot
--rw-rw-rw-   0 root         (0) root         (0)     1535 2023-04-30 18:44:36.000000 sosse-1.0.0/tests/robotframework/tests/common.robot
--rw-rw-rw-   0 root         (0) root         (0)      467 2023-04-30 18:44:36.000000 sosse-1.0.0/tests/searchhistory.json
--rwxrwxrwx   0 root         (0) root         (0)      938 2023-04-30 18:44:36.000000 sosse-1.0.0/tests/test_app.sh
--rwxrwxrwx   0 root         (0) root         (0)      101 2023-04-30 18:44:36.000000 sosse-1.0.0/tests/wait_for_pg.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.499637 sosse-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-05-01 14:24:18.000000 sosse-1.0.1/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      276 2023-05-01 14:24:18.000000 sosse-1.0.1/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.383640 sosse-1.0.1/.gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-01 14:24:18.000000 sosse-1.0.1/.gitlab/changelog_config.yml
+-rw-rw-rw-   0 root         (0) root         (0)     6965 2023-05-01 14:24:18.000000 sosse-1.0.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      491 2023-05-01 14:24:18.000000 sosse-1.0.1/.readthedocs.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-05-01 14:24:18.000000 sosse-1.0.1/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2023-05-01 14:24:18.000000 sosse-1.0.1/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)    34523 2023-05-01 14:24:18.000000 sosse-1.0.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-01 14:24:18.000000 sosse-1.0.1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     7527 2023-05-01 14:24:18.000000 sosse-1.0.1/Makefile
+-rw-r--r--   0 root         (0) root         (0)     3182 2023-05-01 14:24:43.499637 sosse-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2790 2023-05-01 14:24:18.000000 sosse-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.391639 sosse-1.0.1/debian/
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-05-01 14:24:18.000000 sosse-1.0.1/debian/changelog
+-rw-rw-rw-   0 root         (0) root         (0)        3 2023-05-01 14:24:18.000000 sosse-1.0.1/debian/compat
+-rw-rw-rw-   0 root         (0) root         (0)      710 2023-05-01 14:24:18.000000 sosse-1.0.1/debian/control
+-rwxrwxrwx   0 root         (0) root         (0)      182 2023-05-01 14:24:18.000000 sosse-1.0.1/debian/rules
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-05-01 14:24:18.000000 sosse-1.0.1/debian/sosse-crawler.service
+-rw-rw-rw-   0 root         (0) root         (0)      803 2023-05-01 14:24:18.000000 sosse-1.0.1/debian/sosse-uwsgi.service
+-rw-rw-rw-   0 root         (0) root         (0)     2176 2023-05-01 14:24:18.000000 sosse-1.0.1/debian/sosse.conf
+-rw-rw-rw-   0 root         (0) root         (0)      196 2023-05-01 14:24:18.000000 sosse-1.0.1/debian/sosse.install
+-rw-rw-rw-   0 root         (0) root         (0)     2733 2023-05-01 14:24:18.000000 sosse-1.0.1/debian/sosse.postinst
+-rw-rw-rw-   0 root         (0) root         (0)      465 2023-05-01 14:24:18.000000 sosse-1.0.1/debian/uwsgi.ini
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-05-01 14:24:18.000000 sosse-1.0.1/debian/uwsgi.params
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.395639 sosse-1.0.1/doc/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/Makefile
+-rwxrwxrwx   0 root         (0) root         (0)      314 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/build_changelog.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1897 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/get_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.403639 sosse-1.0.1/doc/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.403639 sosse-1.0.1/doc/source/_extensions/
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/_extensions/code_blocks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.403639 sosse-1.0.1/doc/source/_static/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/_static/style.css
+-rw-rw-rw-   0 root         (0) root         (0)      723 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/admin_ui.rst
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/administration.rst
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/authentication.rst
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/cli.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1951 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/config_file.rst
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/cookies.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.407639 sosse-1.0.1/doc/source/crawl/
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/crawl/add_to_queue.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1452 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/crawl/crawl_depth.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5773 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/crawl/policies.rst
+-rw-rw-rw-   0 root         (0) root         (0)      316 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/crawl/status.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1210 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/documents.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1408 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/domain_settings.rst
+-rw-rw-rw-   0 root         (0) root         (0)      315 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/excluded_urls.rst
+-rw-rw-rw-   0 root         (0) root         (0)      531 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.411639 sosse-1.0.1/doc/source/install/
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/install/database.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1832 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/install/debian.rst
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/install/debian_upgrades.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/install/docker.rst
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/install/docker_upgrades.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3287 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/install/pip.rst
+-rw-rw-rw-   0 root         (0) root         (0)      450 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/install/pip_upgrades.rst
+-rw-rw-rw-   0 root         (0) root         (0)      287 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/install.rst
+-rw-rw-rw-   0 root         (0) root         (0)      988 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/permissions.rst
+-rw-rw-rw-   0 root         (0) root         (0)      989 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/screenshots.rst
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/search_engines.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.415639 sosse-1.0.1/doc/source/user/
+-rw-rw-rw-   0 root         (0) root         (0)      823 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/user/cached.rst
+-rw-rw-rw-   0 root         (0) root         (0)      593 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/user/history.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/user/preferences.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4293 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/user/search.rst
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/user/shortcut_list.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/user/shortcuts.rst
+-rw-rw-rw-   0 root         (0) root         (0)      201 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/user/statistics.rst
+-rw-rw-rw-   0 root         (0) root         (0)      245 2023-05-01 14:24:18.000000 sosse-1.0.1/doc/source/user_doc.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.419639 sosse-1.0.1/docker/
+-rw-rw-rw-   0 root         (0) root         (0)      882 2023-05-01 14:24:18.000000 sosse-1.0.1/docker/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-05-01 14:24:18.000000 sosse-1.0.1/docker/Makefile.common
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.419639 sosse-1.0.1/docker/debian/
+-rw-rw-rw-   0 root         (0) root         (0)     2128 2023-05-01 14:24:18.000000 sosse-1.0.1/docker/debian/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-05-01 14:24:18.000000 sosse-1.0.1/docker/debian/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.419639 sosse-1.0.1/docker/debian-pkg/
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-05-01 14:24:18.000000 sosse-1.0.1/docker/debian-pkg/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-01 14:24:18.000000 sosse-1.0.1/docker/debian-pkg/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.423639 sosse-1.0.1/docker/debian-test/
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2023-05-01 14:24:18.000000 sosse-1.0.1/docker/debian-test/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-05-01 14:24:18.000000 sosse-1.0.1/docker/debian-test/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.423639 sosse-1.0.1/docker/doc/
+-rw-rw-rw-   0 root         (0) root         (0)      449 2023-05-01 14:24:18.000000 sosse-1.0.1/docker/doc/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-05-01 14:24:18.000000 sosse-1.0.1/docker/doc/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.423639 sosse-1.0.1/docker/pip-base/
+-rw-rw-rw-   0 root         (0) root         (0)      442 2023-05-01 14:24:18.000000 sosse-1.0.1/docker/pip-base/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-01 14:24:18.000000 sosse-1.0.1/docker/pip-base/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.427639 sosse-1.0.1/docker/pip-release/
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2023-05-01 14:24:18.000000 sosse-1.0.1/docker/pip-release/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-05-01 14:24:18.000000 sosse-1.0.1/docker/pip-release/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.427639 sosse-1.0.1/docker/pip-test/
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-05-01 14:24:18.000000 sosse-1.0.1/docker/pip-test/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-01 14:24:18.000000 sosse-1.0.1/docker/pip-test/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      892 2023-05-01 14:24:18.000000 sosse-1.0.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-05-01 14:24:18.000000 sosse-1.0.1/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.443638 sosse-1.0.1/se/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-01 14:24:18.000000 sosse-1.0.1/se/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20299 2023-05-01 14:24:18.000000 sosse-1.0.1/se/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      996 2023-05-01 14:24:18.000000 sosse-1.0.1/se/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     4121 2023-05-01 14:24:18.000000 sosse-1.0.1/se/atom.py
+-rw-rw-rw-   0 root         (0) root         (0)    24133 2023-05-01 14:24:18.000000 sosse-1.0.1/se/browser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2804 2023-05-01 14:24:18.000000 sosse-1.0.1/se/cached.py
+-rw-rw-rw-   0 root         (0) root         (0)     4314 2023-05-01 14:24:18.000000 sosse-1.0.1/se/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-05-01 14:24:18.000000 sosse-1.0.1/se/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.447638 sosse-1.0.1/se/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-01 14:24:18.000000 sosse-1.0.1/se/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.451638 sosse-1.0.1/se/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-01 14:24:18.000000 sosse-1.0.1/se/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4311 2023-05-01 14:24:18.000000 sosse-1.0.1/se/management/commands/crawl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2023-05-01 14:24:18.000000 sosse-1.0.1/se/management/commands/default_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2023-05-01 14:24:18.000000 sosse-1.0.1/se/management/commands/default_conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     6143 2023-05-01 14:24:18.000000 sosse-1.0.1/se/management/commands/extract_doc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2023-05-01 14:24:18.000000 sosse-1.0.1/se/management/commands/generate_secret.py
+-rw-rw-rw-   0 root         (0) root         (0)     1746 2023-05-01 14:24:18.000000 sosse-1.0.1/se/management/commands/load_se.py
+-rw-rw-rw-   0 root         (0) root         (0)     2150 2023-05-01 14:24:18.000000 sosse-1.0.1/se/management/commands/update_se.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.451638 sosse-1.0.1/se/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    13998 2023-05-01 14:19:16.000000 sosse-1.0.1/se/migrations/0001_initial.py
+-rwxrwxrwx   0 root         (0) root         (0)     2976 2023-05-01 14:19:16.000000 sosse-1.0.1/se/migrations/0002_search_vector.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-01 14:19:17.000000 sosse-1.0.1/se/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    55276 2023-05-01 14:24:18.000000 sosse-1.0.1/se/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1941 2023-05-01 14:24:18.000000 sosse-1.0.1/se/screenshot.py
+-rw-rw-rw-   0 root         (0) root         (0)     6607 2023-05-01 14:24:18.000000 sosse-1.0.1/se/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.371640 sosse-1.0.1/se/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.463638 sosse-1.0.1/se/static/se/
+-rw-rw-rw-   0 root         (0) root         (0)    19511 2023-05-01 14:24:18.000000 sosse-1.0.1/se/static/se/admin-base.css
+-rw-rw-rw-   0 root         (0) root         (0)     8810 2023-05-01 14:24:18.000000 sosse-1.0.1/se/static/se/admin-forms.css
+-rw-rw-rw-   0 root         (0) root         (0)     2005 2023-05-01 14:24:18.000000 sosse-1.0.1/se/static/se/base.js
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2023-05-01 14:24:18.000000 sosse-1.0.1/se/static/se/icon-atom.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2196 2023-05-01 14:24:18.000000 sosse-1.0.1/se/static/se/icon-clear.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3722 2023-05-01 14:24:18.000000 sosse-1.0.1/se/static/se/icon-cog.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2023-05-01 14:24:18.000000 sosse-1.0.1/se/static/se/icon-search.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2488 2023-05-01 14:24:18.000000 sosse-1.0.1/se/static/se/icon-stats.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3644 2023-05-01 14:24:18.000000 sosse-1.0.1/se/static/se/icon-trash.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-05-01 14:24:18.000000 sosse-1.0.1/se/static/se/icon-user.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9798 2023-05-01 14:24:18.000000 sosse-1.0.1/se/static/se/index.js
+-rw-rw-rw-   0 root         (0) root         (0)     4462 2023-05-01 14:24:18.000000 sosse-1.0.1/se/static/se/logo.png
+-rw-rw-rw-   0 root         (0) root         (0)     9908 2023-05-01 14:24:18.000000 sosse-1.0.1/se/static/se/logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     5967 2023-05-01 14:24:18.000000 sosse-1.0.1/se/static/se/pygal-tooltips.min.js
+-rw-rw-rw-   0 root         (0) root         (0)      982 2023-05-01 14:24:18.000000 sosse-1.0.1/se/static/se/screenshot.js
+-rw-rw-rw-   0 root         (0) root         (0)     2522 2023-05-01 14:24:18.000000 sosse-1.0.1/se/static/se/style.css
+-rw-rw-rw-   0 root         (0) root         (0)     8567 2023-05-01 14:24:18.000000 sosse-1.0.1/se/stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.371640 sosse-1.0.1/se/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.467638 sosse-1.0.1/se/templates/admin/
+-rw-rw-rw-   0 root         (0) root         (0)     3427 2023-05-01 14:24:18.000000 sosse-1.0.1/se/templates/admin/add_to_queue.html
+-rw-rw-rw-   0 root         (0) root         (0)     2518 2023-05-01 14:24:18.000000 sosse-1.0.1/se/templates/admin/app_list.html
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2023-05-01 14:24:18.000000 sosse-1.0.1/se/templates/admin/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-05-01 14:24:18.000000 sosse-1.0.1/se/templates/admin/base_site.html
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-05-01 14:24:18.000000 sosse-1.0.1/se/templates/admin/change_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-01 14:24:18.000000 sosse-1.0.1/se/templates/admin/crawl_status.html
+-rw-rw-rw-   0 root         (0) root         (0)     2706 2023-05-01 14:24:18.000000 sosse-1.0.1/se/templates/admin/crawl_status_content.html
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-01 14:24:18.000000 sosse-1.0.1/se/templates/admin/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.479637 sosse-1.0.1/se/templates/se/
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-05-01 14:24:18.000000 sosse-1.0.1/se/templates/se/about.html
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-05-01 14:24:18.000000 sosse-1.0.1/se/templates/se/base.html
+-rw-rw-rw-   0 root         (0) root         (0)     2285 2023-05-01 14:24:18.000000 sosse-1.0.1/se/templates/se/cached.html
+-rw-rw-rw-   0 root         (0) root         (0)     1870 2023-05-01 14:24:18.000000 sosse-1.0.1/se/templates/se/history.html
+-rw-rw-rw-   0 root         (0) root         (0)     8235 2023-05-01 14:24:18.000000 sosse-1.0.1/se/templates/se/index.html
+-rw-rw-rw-   0 root         (0) root         (0)     1320 2023-05-01 14:24:18.000000 sosse-1.0.1/se/templates/se/main_menu.html
+-rw-rw-rw-   0 root         (0) root         (0)      544 2023-05-01 14:24:18.000000 sosse-1.0.1/se/templates/se/opensearch.xml
+-rw-rw-rw-   0 root         (0) root         (0)      761 2023-05-01 14:24:18.000000 sosse-1.0.1/se/templates/se/pagination.html
+-rw-rw-rw-   0 root         (0) root         (0)     2242 2023-05-01 14:24:18.000000 sosse-1.0.1/se/templates/se/prefs.html
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2023-05-01 14:24:18.000000 sosse-1.0.1/se/templates/se/screenshot.html
+-rw-rw-rw-   0 root         (0) root         (0)     1523 2023-05-01 14:24:18.000000 sosse-1.0.1/se/templates/se/search_redirect.html
+-rw-rw-rw-   0 root         (0) root         (0)     1547 2023-05-01 14:24:18.000000 sosse-1.0.1/se/templates/se/stats.html
+-rw-rw-rw-   0 root         (0) root         (0)      741 2023-05-01 14:24:18.000000 sosse-1.0.1/se/templates/se/unknown_url.html
+-rw-rw-rw-   0 root         (0) root         (0)      474 2023-05-01 14:24:18.000000 sosse-1.0.1/se/templates/se/words.html
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-01 14:24:18.000000 sosse-1.0.1/se/templates/se/www.html
+-rw-rw-rw-   0 root         (0) root         (0)     5979 2023-05-01 14:24:18.000000 sosse-1.0.1/se/test_cookie.py
+-rw-rw-rw-   0 root         (0) root         (0)    14144 2023-05-01 14:24:18.000000 sosse-1.0.1/se/test_crawl.py
+-rw-rw-rw-   0 root         (0) root         (0)     9790 2023-05-01 14:24:18.000000 sosse-1.0.1/se/test_functionals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1459 2023-05-01 14:24:18.000000 sosse-1.0.1/se/test_misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4659 2023-05-01 14:24:18.000000 sosse-1.0.1/se/test_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2133 2023-05-01 14:24:18.000000 sosse-1.0.1/se/test_redirect.py
+-rw-rw-rw-   0 root         (0) root         (0)     1600 2023-05-01 14:24:18.000000 sosse-1.0.1/se/test_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)     9547 2023-05-01 14:24:18.000000 sosse-1.0.1/se/test_search.py
+-rw-rw-rw-   0 root         (0) root         (0)     2612 2023-05-01 14:24:18.000000 sosse-1.0.1/se/test_url.py
+-rw-rw-rw-   0 root         (0) root         (0)     6326 2023-05-01 14:24:18.000000 sosse-1.0.1/se/test_views.py
+-rw-rw-rw-   0 root         (0) root         (0)     3101 2023-05-01 14:24:18.000000 sosse-1.0.1/se/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     8408 2023-05-01 14:24:18.000000 sosse-1.0.1/se/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-05-01 14:24:18.000000 sosse-1.0.1/se/words.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2023-05-01 14:24:18.000000 sosse-1.0.1/se/www.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 14:24:43.499637 sosse-1.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.483637 sosse-1.0.1/sosse/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-01 14:24:18.000000 sosse-1.0.1/sosse/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16555 2023-05-01 14:24:18.000000 sosse-1.0.1/sosse/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)    18193 2023-05-01 14:24:18.000000 sosse-1.0.1/sosse/search_engines.json
+-rw-rw-rw-   0 root         (0) root         (0)     7433 2023-05-01 14:24:25.000000 sosse-1.0.1/sosse/settings.py
+-rwxrwxrwx   0 root         (0) root         (0)     1328 2023-05-01 14:24:18.000000 sosse-1.0.1/sosse/sosse_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-05-01 14:24:18.000000 sosse-1.0.1/sosse/test_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2548 2023-05-01 14:24:18.000000 sosse-1.0.1/sosse/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2023-05-01 14:24:18.000000 sosse-1.0.1/sosse/wsgi.py
+-rwxrwxrwx   0 root         (0) root         (0)       70 2023-05-01 14:24:18.000000 sosse-1.0.1/sosse-admin
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.487637 sosse-1.0.1/sosse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3182 2023-05-01 14:24:43.000000 sosse-1.0.1/sosse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-05-01 14:24:43.000000 sosse-1.0.1/sosse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 14:24:43.000000 sosse-1.0.1/sosse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-01 14:24:43.000000 sosse-1.0.1/sosse.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      129 2023-05-01 14:24:43.000000 sosse-1.0.1/sosse.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-01 14:24:43.000000 sosse-1.0.1/sosse.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.495637 sosse-1.0.1/tests/
+-rwxrwxrwx   0 root         (0) root         (0)      281 2023-05-01 14:24:18.000000 sosse-1.0.1/tests/build_doc.sh
+-rw-rw-rw-   0 root         (0) root         (0)      809 2023-05-01 14:24:18.000000 sosse-1.0.1/tests/cookies.json
+-rwxrwxrwx   0 root         (0) root         (0)     1047 2023-05-01 14:24:18.000000 sosse-1.0.1/tests/doc_test.sh
+-rwxrwxrwx   0 root         (0) root         (0)      477 2023-05-01 14:24:18.000000 sosse-1.0.1/tests/docker_run.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1015 2023-05-01 14:24:18.000000 sosse-1.0.1/tests/document-ja.json
+-rw-rw-rw-   0 root         (0) root         (0)      496 2023-05-01 14:24:18.000000 sosse-1.0.1/tests/opensearch.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.495637 sosse-1.0.1/tests/robotframework/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-05-01 14:24:18.000000 sosse-1.0.1/tests/robotframework/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)      605 2023-05-01 14:24:18.000000 sosse-1.0.1/tests/robotframework/start.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 14:24:43.499637 sosse-1.0.1/tests/robotframework/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     5208 2023-05-01 14:24:18.000000 sosse-1.0.1/tests/robotframework/tests/01_crawl.robot
+-rw-rw-rw-   0 root         (0) root         (0)     2862 2023-05-01 14:24:18.000000 sosse-1.0.1/tests/robotframework/tests/02_user.robot
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-05-01 14:24:18.000000 sosse-1.0.1/tests/robotframework/tests/__init__.robot
+-rw-rw-rw-   0 root         (0) root         (0)     1535 2023-05-01 14:24:18.000000 sosse-1.0.1/tests/robotframework/tests/common.robot
+-rw-rw-rw-   0 root         (0) root         (0)      467 2023-05-01 14:24:18.000000 sosse-1.0.1/tests/searchhistory.json
+-rwxrwxrwx   0 root         (0) root         (0)      938 2023-05-01 14:24:18.000000 sosse-1.0.1/tests/test_app.sh
+-rwxrwxrwx   0 root         (0) root         (0)      101 2023-05-01 14:24:18.000000 sosse-1.0.1/tests/wait_for_pg.sh
```

### Comparing `sosse-1.0.0/.gitlab-ci.yml` & `sosse-1.0.1/.gitlab-ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -81,18 +81,20 @@
 doc_gen:
   image: biolds/sosse:debian-test
   stage: test
   artifacts:
     paths:
       - doc/source/*_generated.rst
       - doc/source/*/*_generated.rst
+      - doc/source/CHANGELOG.md
   script:
     - ./sosse-admin extract_doc conf > doc/source/config_file_generated.rst
     - ./sosse-admin extract_doc cli > doc/source/cli_generated.rst
     - ./sosse-admin extract_doc se > doc/source/user/shortcut_list_generated.rst
+    - ./doc/build_changelog.sh > doc/source/CHANGELOG.md
 
 doc_code_extract:
   image: biolds/sosse:doc
   stage: test
   needs:
     - doc_gen
   artifacts:
@@ -150,14 +152,27 @@
     - rm -rf htmlcov
     - sed -e "s/^SOSSE_VERSION_TAG = .*/SOSSE_VERSION_TAG = '${CI_COMMIT_TAG/v/}'/" -i sosse/settings.py
     - sed -e "s/^SOSSE_VERSION_COMMIT = .*/SOSSE_VERSION_COMMIT = '${CI_COMMIT_SHORT_SHA}'/" -i sosse/settings.py
     - mkdir /deb
     - make _deb
     - mv /deb .
 
+changelog:
+  image: biolds/sosse:debian-test
+  stage: build
+  needs: []
+  artifacts:
+    paths:
+      - CHANGELOG.md
+  script:
+    - 'last_ver="$(git tag -l | sort -V | tail -n 1 | sed -e "s/^v//")"'
+    - 'new_ver="${last_ver%.*}.$((${last_ver/*./} + 1))"'
+    - 'curl -X GET -H "PRIVATE-TOKEN: $GITLAB_REST_API_CHANGELOG" "https://gitlab.com/api/v4/projects/$CI_PROJECT_ID/repository/changelog?version=$new_ver" | jq -r .notes | tee /tmp/new'
+    - cat /tmp/new CHANGELOG.md > new.md && mv new.md CHANGELOG.md
+
 doc_test_debian:
   image: debian:bullseye
   stage: build_check
   needs:
     - doc_code_extract
   script:
     - apt update
```

### Comparing `sosse-1.0.0/Dockerfile` & `sosse-1.0.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/LICENSE` & `sosse-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/Makefile` & `sosse-1.0.1/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -25,25 +25,26 @@
 	/venv/bin/pip install twine
 	@echo ==============================================================================================
 	@echo 'Uploading to Pypi, please use "__token__" as username, and the token (pypi-xxxxxx) as password'
 	@echo ==============================================================================================
 	/venv/bin/twine upload --verbose dist/*
 
 pip_pkg_push:
-	docker run --rm -v $(current_dir):/sosse:ro -ti biolds/sosse:pip-base bash -c 'cd /sosse && make _pip_pkg_push'
+	docker run --rm -v $(current_dir):/sosse:ro -ti biolds/sosse:pip-test bash -c 'cd /sosse && make _pip_pkg_push'
 
 _deb:
 	dpkg-buildpackage -us -uc
 	mv ../sosse*_amd64.deb /deb/
 
 deb:
 	mkdir $(current_dir)/deb/ &>/dev/null ||:
 	docker run --rm -v $(current_dir):/sosse:ro -v $(current_dir)/deb:/deb biolds/sosse:debian-pkg bash -c 'cp -x -r /sosse /sosse-deb && make -C /sosse-deb _deb'
 
 _build_doc:
+	./doc/build_changelog.sh > doc/source/CHANGELOG.md
 	. /opt/sosse-doc/bin/activate ; make -C doc linkcheck html SPHINXOPTS="-W"
 	jq . < doc/code_blocks.json > /tmp/code_blocks.json
 	mv /tmp/code_blocks.json doc/code_blocks.json
 
 build_doc:
 	mkdir -p doc/build/
 	docker run --rm -v $(current_dir):/sosse:ro -v $(current_dir)/doc/build:/sosse/doc/build biolds/sosse:doc bash -c 'cd /sosse && make _build_doc'
@@ -51,21 +52,33 @@
 
 docker_run:
 	docker volume inspect sosse_postgres &>/dev/null || docker volume create sosse_postgres
 	docker volume inspect sosse_var &>/dev/null || docker volume create sosse_var
 	docker run -p 8005:80 --mount source=sosse_postgres,destination=/var/lib/postgresql \
 						--mount source=sosse_var,destination=/var/lib/sosse biolds/sosse:latest
 
+docker_release_push:
+	docker push biolds/sosse:latest
+
+docker_release_build:
+	docker pull debian:bullseye
+	$(MAKE) -C docker/pip-base build APT_PROXY=$(APT_PROXY) PIP_INDEX_URL=$(PIP_INDEX_URL) PIP_TRUSTED_HOST=$(PIP_TRUSTED_HOST)
+	$(MAKE) -C docker/pip-release build APT_PROXY=$(APT_PROXY) PIP_INDEX_URL=$(PIP_INDEX_URL) PIP_TRUSTED_HOST=$(PIP_TRUSTED_HOST)
+	docker tag biolds/sosse:pip-release biolds/sosse:latest
+
+docker_git_build:
+	docker pull debian:bullseye
+	$(MAKE) -C docker/pip-base build APT_PROXY=$(APT_PROXY) PIP_INDEX_URL=$(PIP_INDEX_URL) PIP_TRUSTED_HOST=$(PIP_TRUSTED_HOST)
+	docker build --build-arg APT_PROXY=$(APT_PROXY) --build-arg PIP_INDEX_URL=$(PIP_INDEX_URL) --build-arg PIP_TRUSTED_HOST=$(PIP_TRUSTED_HOST) -t biolds/sosse:git .
+
 docker_push:
 	$(MAKE) -C docker push
-	docker push biolds/sosse:latest
 
 docker_build:
 	$(MAKE) -C docker build
-	docker build --build-arg APT_PROXY=$(APT_PROXY) --build-arg PIP_INDEX_URL=$(PIP_INDEX_URL) --build-arg PIP_TRUSTED_HOST=$(PIP_TRUSTED_HOST) -t biolds/sosse:latest .
 
 _doc_test_debian:
 	cp doc/code_blocks.json /tmp/code_blocks.json
 	grep -q 'apt install -y python3-django/bullseye-backports sosse' /tmp/code_blocks.json
 	sed -e 's#apt install -y python3-django/bullseye-backports sosse#apt install -y python3-django/bullseye-backports sosse; /etc/init.d/nginx start \& /etc/init.d/postgresql start \& bash ./tests/wait_for_pg.sh#' -i /tmp/code_blocks.json
 	bash ./tests/doc_test.sh /tmp/code_blocks.json install/debian
```

### Comparing `sosse-1.0.0/PKG-INFO` & `sosse-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosse
-Version: 1.0.0
+Version: 1.0.1
 Summary: Selenium Open Source Search Engine
 Author-email: Laurent Defert <laurent_defert@yahoo.fr>
 License: GNU Affero General Public License v3
 Keywords: search engine,crawler
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
@@ -15,15 +15,15 @@
   <img src="https://raw.githubusercontent.com/biolds/sosse/main/se/static/se/logo.svg" width="64" align="right">
   <a href="https://gitlab.com/biolds1/sosse/" alt="Gitlab code coverage">
     <img src="https://img.shields.io/gitlab/pipeline-coverage/biolds1/sosse?branch=main&style=flat-square">
   </a>
   <a href="https://gitlab.com/biolds1/sosse/-/pipelines" alt="Gitlab pipeline status">
     <img src="https://img.shields.io/gitlab/pipeline-status/biolds1/sosse?branch=main&style=flat-square">
   </a>
-  <a href="https://sosse.readthedocs.io/en/latest/" alt="Documentation">
+  <a href="https://sosse.readthedocs.io/en/stable/" alt="Documentation">
     <img src="https://img.shields.io/readthedocs/sosse?style=flat-square">
   </a>
   <a href="https://gitlab.com/biolds1/sosse/-/blob/main/LICENSE" alt="License">
     <img src="https://img.shields.io/gitlab/license/biolds1/sosse?style=flat-square">
   </a>
 </p>
 
@@ -36,26 +36,26 @@
 - 🌍 Browser based crawling: the crawler can use [Google Chromium](https://www.chromium.org/Home) and [Selenium](https://www.selenium.dev/) to index pages that use Javascript. [Requests](https://docs.python-requests.org/en/latest/index.html) can also be used for faster crawling
 - 🏖 Low resources requirements: SOSSE is entirely written in Python and uses [PostgreSQL](https://www.postgresql.org/) for data storage
 - 🖼 Offline cache: SOSSE can take screenshots of crawled pages and make them browsable offline
 - 🔓 Authentication: the crawlers can submit authentication forms with provided credentials
 - 🔗 Search engines shortcuts: shortcuts search queries can be used to redirect to external search engines (sometime called "bang" searches)
 - 🔖 Search history: users can authenticate to log their search query history privately
 
-See the [documentation](https://sosse.readthedocs.io/en/latest/) and [screenshots](https://sosse.readthedocs.io/en/latest/).
+See the [documentation](https://sosse.readthedocs.io/en/stable/) and [screenshots](https://sosse.readthedocs.io/en/stable/screenshots.html).
 
 Try it out
 ==========
 
 You can try the latest version with Docker:
 
 ```
 docker run -p 8005:80 biolds/sosse:latest
 ```
 
-Default user is ``admin``, with password ``admin``.
+Connect to port 8005, and log in with user ``admin``, with password ``admin``.
 
-You can also find alternative installation methods in the [documentation](https://sosse.readthedocs.io/en/latest/install.html).
+To persist Docker data, or find alternative installation methods, please check the [documentation](https://sosse.readthedocs.io/en/stable/install.html).
 
 Keep in touch
 =============
 
 Join the [Discord server](https://discord.gg/Vt9cMf7BGK) to get help and share ideas!
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sosse Version: 1.0.0 Summary: Selenium Open Source
+Metadata-Version: 2.1 Name: sosse Version: 1.0.1 Summary: Selenium Open Source
 Search Engine Author-email: Laurent Defert
 yahoo.fr> License: GNU Affero General Public License v3 Keywords: search
 engine,crawler Classifier: Framework :: Django Classifier: Programming Language
 :: Python :: 3 Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE
 [https://raw.githubusercontent.com/biolds/sosse/main/se/static/se/logo.svg]
 [https://img.shields.io/gitlab/pipeline-coverage/biolds1/
@@ -24,14 +24,15 @@
 Python and uses [PostgreSQL](https://www.postgresql.org/) for data storage -
 ð¼ Offline cache: SOSSE can take screenshots of crawled pages and make them
 browsable offline - ð Authentication: the crawlers can submit authentication
 forms with provided credentials - ð Search engines shortcuts: shortcuts
 search queries can be used to redirect to external search engines (sometime
 called "bang" searches) - ð Search history: users can authenticate to log
 their search query history privately See the [documentation](https://
-sosse.readthedocs.io/en/latest/) and [screenshots](https://
-sosse.readthedocs.io/en/latest/). Try it out ========== You can try the latest
-version with Docker: ``` docker run -p 8005:80 biolds/sosse:latest ``` Default
-user is ``admin``, with password ``admin``. You can also find alternative
-installation methods in the [documentation](https://sosse.readthedocs.io/en/
-latest/install.html). Keep in touch ============= Join the [Discord server]
-(https://discord.gg/Vt9cMf7BGK) to get help and share ideas!
+sosse.readthedocs.io/en/stable/) and [screenshots](https://
+sosse.readthedocs.io/en/stable/screenshots.html). Try it out ========== You can
+try the latest version with Docker: ``` docker run -p 8005:80 biolds/sosse:
+latest ``` Connect to port 8005, and log in with user ``admin``, with password
+``admin``. To persist Docker data, or find alternative installation methods,
+please check the [documentation](https://sosse.readthedocs.io/en/stable/
+install.html). Keep in touch ============= Join the [Discord server](https://
+discord.gg/Vt9cMf7BGK) to get help and share ideas!
```

### Comparing `sosse-1.0.0/README.md` & `sosse-1.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   <img src="https://raw.githubusercontent.com/biolds/sosse/main/se/static/se/logo.svg" width="64" align="right">
   <a href="https://gitlab.com/biolds1/sosse/" alt="Gitlab code coverage">
     <img src="https://img.shields.io/gitlab/pipeline-coverage/biolds1/sosse?branch=main&style=flat-square">
   </a>
   <a href="https://gitlab.com/biolds1/sosse/-/pipelines" alt="Gitlab pipeline status">
     <img src="https://img.shields.io/gitlab/pipeline-status/biolds1/sosse?branch=main&style=flat-square">
   </a>
-  <a href="https://sosse.readthedocs.io/en/latest/" alt="Documentation">
+  <a href="https://sosse.readthedocs.io/en/stable/" alt="Documentation">
     <img src="https://img.shields.io/readthedocs/sosse?style=flat-square">
   </a>
   <a href="https://gitlab.com/biolds1/sosse/-/blob/main/LICENSE" alt="License">
     <img src="https://img.shields.io/gitlab/license/biolds1/sosse?style=flat-square">
   </a>
 </p>
 
@@ -23,26 +23,26 @@
 - 🌍 Browser based crawling: the crawler can use [Google Chromium](https://www.chromium.org/Home) and [Selenium](https://www.selenium.dev/) to index pages that use Javascript. [Requests](https://docs.python-requests.org/en/latest/index.html) can also be used for faster crawling
 - 🏖 Low resources requirements: SOSSE is entirely written in Python and uses [PostgreSQL](https://www.postgresql.org/) for data storage
 - 🖼 Offline cache: SOSSE can take screenshots of crawled pages and make them browsable offline
 - 🔓 Authentication: the crawlers can submit authentication forms with provided credentials
 - 🔗 Search engines shortcuts: shortcuts search queries can be used to redirect to external search engines (sometime called "bang" searches)
 - 🔖 Search history: users can authenticate to log their search query history privately
 
-See the [documentation](https://sosse.readthedocs.io/en/latest/) and [screenshots](https://sosse.readthedocs.io/en/latest/).
+See the [documentation](https://sosse.readthedocs.io/en/stable/) and [screenshots](https://sosse.readthedocs.io/en/stable/screenshots.html).
 
 Try it out
 ==========
 
 You can try the latest version with Docker:
 
 ```
 docker run -p 8005:80 biolds/sosse:latest
 ```
 
-Default user is ``admin``, with password ``admin``.
+Connect to port 8005, and log in with user ``admin``, with password ``admin``.
 
-You can also find alternative installation methods in the [documentation](https://sosse.readthedocs.io/en/latest/install.html).
+To persist Docker data, or find alternative installation methods, please check the [documentation](https://sosse.readthedocs.io/en/stable/install.html).
 
 Keep in touch
 =============
 
 Join the [Discord server](https://discord.gg/Vt9cMf7BGK) to get help and share ideas!
```

#### html2text {}

```diff
@@ -18,14 +18,15 @@
 Python and uses [PostgreSQL](https://www.postgresql.org/) for data storage -
 ð¼ Offline cache: SOSSE can take screenshots of crawled pages and make them
 browsable offline - ð Authentication: the crawlers can submit authentication
 forms with provided credentials - ð Search engines shortcuts: shortcuts
 search queries can be used to redirect to external search engines (sometime
 called "bang" searches) - ð Search history: users can authenticate to log
 their search query history privately See the [documentation](https://
-sosse.readthedocs.io/en/latest/) and [screenshots](https://
-sosse.readthedocs.io/en/latest/). Try it out ========== You can try the latest
-version with Docker: ``` docker run -p 8005:80 biolds/sosse:latest ``` Default
-user is ``admin``, with password ``admin``. You can also find alternative
-installation methods in the [documentation](https://sosse.readthedocs.io/en/
-latest/install.html). Keep in touch ============= Join the [Discord server]
-(https://discord.gg/Vt9cMf7BGK) to get help and share ideas!
+sosse.readthedocs.io/en/stable/) and [screenshots](https://
+sosse.readthedocs.io/en/stable/screenshots.html). Try it out ========== You can
+try the latest version with Docker: ``` docker run -p 8005:80 biolds/sosse:
+latest ``` Connect to port 8005, and log in with user ``admin``, with password
+``admin``. To persist Docker data, or find alternative installation methods,
+please check the [documentation](https://sosse.readthedocs.io/en/stable/
+install.html). Keep in touch ============= Join the [Discord server](https://
+discord.gg/Vt9cMf7BGK) to get help and share ideas!
```

### Comparing `sosse-1.0.0/debian/control` & `sosse-1.0.1/debian/control`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/debian/sosse-crawler.service` & `sosse-1.0.1/debian/sosse-crawler.service`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/debian/sosse-uwsgi.service` & `sosse-1.0.1/debian/sosse-uwsgi.service`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/debian/sosse.conf` & `sosse-1.0.1/debian/sosse.conf`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/debian/sosse.postinst` & `sosse-1.0.1/debian/sosse.postinst`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/debian/uwsgi.params` & `sosse-1.0.1/debian/uwsgi.params`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/doc/Makefile` & `sosse-1.0.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/doc/get_artifacts.py` & `sosse-1.0.1/doc/get_artifacts.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/doc/make.bat` & `sosse-1.0.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/doc/source/_extensions/code_blocks.py` & `sosse-1.0.1/doc/source/_extensions/code_blocks.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/doc/source/admin_ui.rst` & `sosse-1.0.1/doc/source/admin_ui.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/doc/source/authentication.rst` & `sosse-1.0.1/doc/source/authentication.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/doc/source/conf.py` & `sosse-1.0.1/doc/source/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,17 +28,22 @@
 author = 'Laurent Defert'
 release = '1.0'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 sys.path.append(os.path.abspath('_extensions'))
-extensions = ['code_blocks']
+extensions = ['code_blocks', 'myst_parser']
 test_code_output = 'code_blocks.json'
 
+source_suffix = {
+    '.rst': 'restructuredtext',
+    '.md': 'markdown',
+}
+
 templates_path = ['_templates']
 exclude_patterns = []
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = 'furo'
```

### Comparing `sosse-1.0.0/doc/source/crawl/add_to_queue.rst` & `sosse-1.0.1/doc/source/crawl/add_to_queue.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/doc/source/crawl/crawl_depth.rst` & `sosse-1.0.1/doc/source/crawl/crawl_depth.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/doc/source/crawl/policies.rst` & `sosse-1.0.1/doc/source/crawl/policies.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/doc/source/documents.rst` & `sosse-1.0.1/doc/source/documents.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/doc/source/domain_settings.rst` & `sosse-1.0.1/doc/source/domain_settings.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/doc/source/install/database.rst` & `sosse-1.0.1/doc/source/install/database.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/doc/source/install/debian.rst` & `sosse-1.0.1/doc/source/install/debian.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/doc/source/install/docker.rst` & `sosse-1.0.1/doc/source/install/docker.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/doc/source/install/pip.rst` & `sosse-1.0.1/doc/source/install/pip.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/doc/source/permissions.rst` & `sosse-1.0.1/doc/source/permissions.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/doc/source/screenshots.rst` & `sosse-1.0.1/doc/source/screenshots.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/doc/source/search_engines.rst` & `sosse-1.0.1/doc/source/search_engines.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/doc/source/user/cached.rst` & `sosse-1.0.1/doc/source/user/cached.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/doc/source/user/history.rst` & `sosse-1.0.1/doc/source/user/history.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/doc/source/user/preferences.rst` & `sosse-1.0.1/doc/source/user/preferences.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/doc/source/user/search.rst` & `sosse-1.0.1/doc/source/user/search.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/doc/source/user/shortcuts.rst` & `sosse-1.0.1/doc/source/user/shortcuts.rst`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/docker/Makefile` & `sosse-1.0.1/docker/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 build:
 	docker pull debian:bullseye
 	$(MAKE) -C debian build APT_PROXY=$(APT_PROXY) PIP_INDEX_URL=$(PIP_INDEX_URL) PIP_TRUSTED_HOST=$(PIP_TRUSTED_HOST)
 	$(MAKE) -C debian-pkg build APT_PROXY=$(APT_PROXY) PIP_INDEX_URL=$(PIP_INDEX_URL) PIP_TRUSTED_HOST=$(PIP_TRUSTED_HOST)
 	$(MAKE) -C debian-test build APT_PROXY=$(APT_PROXY) PIP_INDEX_URL=$(PIP_INDEX_URL) PIP_TRUSTED_HOST=$(PIP_TRUSTED_HOST)
 	$(MAKE) -C pip-base build APT_PROXY=$(APT_PROXY) PIP_INDEX_URL=$(PIP_INDEX_URL) PIP_TRUSTED_HOST=$(PIP_TRUSTED_HOST)
+	$(MAKE) -C pip-release build APT_PROXY=$(APT_PROXY) PIP_INDEX_URL=$(PIP_INDEX_URL) PIP_TRUSTED_HOST=$(PIP_TRUSTED_HOST)
 	$(MAKE) -C pip-test build APT_PROXY=$(APT_PROXY) PIP_INDEX_URL=$(PIP_INDEX_URL) PIP_TRUSTED_HOST=$(PIP_TRUSTED_HOST)
 	$(MAKE) -C doc build
 
 push:
 	@for a in $$(ls); do \
 		if [ -d $$a ]; then \
 			$(MAKE) -C $$a push; \
```

### Comparing `sosse-1.0.0/docker/debian/Dockerfile` & `sosse-1.0.1/docker/debian/Dockerfile`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/docker/debian-pkg/Dockerfile` & `sosse-1.0.1/docker/debian-pkg/Dockerfile`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/docker/debian-test/Dockerfile` & `sosse-1.0.1/docker/debian-test/Dockerfile`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 FROM biolds/sosse:debian
 ARG APT_PROXY=
 ARG PIP_INDEX_URL=
 ARG PIP_TRUSTED_HOST=
 RUN test -z "$APT_PROXY" || (echo "Acquire::http::Proxy \"$APT_PROXY\";" > /etc/apt/apt.conf.d/proxy.conf)
 RUN apt purge -y sosse
-RUN apt install -y python3-coverage python3-virtualenv flake8 git sudo jq make
+RUN apt install -y python3-coverage python3-virtualenv flake8 sudo jq make git/bullseye-backports
 RUN /etc/init.d/postgresql start && \
     su - postgres -c "psql --command 'ALTER USER sosse WITH SUPERUSER;'" && \
     /etc/init.d/postgresql stop
 RUN git clone --depth=1 https://gitlab.com/biolds1/httpbin.git /root/httpbin && \
     cd /root/httpbin/httpbin && \
     python3 manage.py migrate && \
     python3 manage.py shell -c "from django.contrib.auth.models import User ; u = User.objects.create(username='admin', is_superuser=True, is_staff=True) ; u.set_password('admin') ; u.save()"
```

### Comparing `sosse-1.0.0/docker/pip-test/Dockerfile` & `sosse-1.0.1/docker/pip-test/Dockerfile`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/pyproject.toml` & `sosse-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/admin.py` & `sosse-1.0.1/se/admin.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/apps.py` & `sosse-1.0.1/se/apps.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/atom.py` & `sosse-1.0.1/se/atom.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/browser.py` & `sosse-1.0.1/se/browser.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/cached.py` & `sosse-1.0.1/se/cached.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/forms.py` & `sosse-1.0.1/se/forms.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/login.py` & `sosse-1.0.1/se/login.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/management/commands/crawl.py` & `sosse-1.0.1/se/management/commands/crawl.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/management/commands/default_admin.py` & `sosse-1.0.1/se/management/commands/default_admin.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/management/commands/default_conf.py` & `sosse-1.0.1/se/management/commands/default_conf.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/management/commands/extract_doc.py` & `sosse-1.0.1/se/management/commands/extract_doc.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/management/commands/generate_secret.py` & `sosse-1.0.1/se/management/commands/generate_secret.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/management/commands/load_se.py` & `sosse-1.0.1/se/management/commands/load_se.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/management/commands/update_se.py` & `sosse-1.0.1/se/management/commands/update_se.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/migrations/0001_initial.py` & `sosse-1.0.1/se/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/migrations/0002_search_vector.py` & `sosse-1.0.1/se/migrations/0002_search_vector.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/models.py` & `sosse-1.0.1/se/models.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/screenshot.py` & `sosse-1.0.1/se/screenshot.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/search.py` & `sosse-1.0.1/se/search.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/static/se/admin-base.css` & `sosse-1.0.1/se/static/se/admin-base.css`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/static/se/admin-forms.css` & `sosse-1.0.1/se/static/se/admin-forms.css`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/static/se/base.js` & `sosse-1.0.1/se/static/se/base.js`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/static/se/icon-atom.svg` & `sosse-1.0.1/se/static/se/icon-atom.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/static/se/icon-clear.svg` & `sosse-1.0.1/se/static/se/icon-clear.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/static/se/icon-cog.svg` & `sosse-1.0.1/se/static/se/icon-cog.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/static/se/icon-search.svg` & `sosse-1.0.1/se/static/se/icon-search.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/static/se/icon-stats.svg` & `sosse-1.0.1/se/static/se/icon-stats.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/static/se/icon-trash.svg` & `sosse-1.0.1/se/static/se/icon-trash.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/static/se/icon-user.svg` & `sosse-1.0.1/se/static/se/icon-user.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/static/se/index.js` & `sosse-1.0.1/se/static/se/index.js`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/static/se/logo.png` & `sosse-1.0.1/se/static/se/logo.png`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/static/se/logo.svg` & `sosse-1.0.1/se/static/se/logo.svg`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/static/se/pygal-tooltips.min.js` & `sosse-1.0.1/se/static/se/pygal-tooltips.min.js`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/static/se/screenshot.js` & `sosse-1.0.1/se/static/se/screenshot.js`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/static/se/style.css` & `sosse-1.0.1/se/static/se/style.css`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/stats.py` & `sosse-1.0.1/se/stats.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/templates/admin/add_to_queue.html` & `sosse-1.0.1/se/templates/admin/add_to_queue.html`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/templates/admin/app_list.html` & `sosse-1.0.1/se/templates/admin/app_list.html`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/templates/admin/base.html` & `sosse-1.0.1/se/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/templates/admin/change_form.html` & `sosse-1.0.1/se/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/templates/admin/crawl_status.html` & `sosse-1.0.1/se/templates/admin/crawl_status.html`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/templates/admin/crawl_status_content.html` & `sosse-1.0.1/se/templates/admin/crawl_status_content.html`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/templates/se/about.html` & `sosse-1.0.1/se/templates/se/about.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% extends "se/base.html" %}
 
 {% block body %}
     <p>
-        SOSSE is a <a href="https://www.selenium.dev/">Selenium</a> based Open Source Search Engine.
+        SOSSE is a <a href="https://www.selenium.dev/">Selenium</a> based Open Source Search Engine {{ animal }}.
     </p>
     <p>
         It is distributed under the <a href="https://www.gnu.org/licenses/agpl-3.0.en.html">GNU Affero General Public License version 3</a>.
     </p>
     <p>
         You can download a copy of its source code on <a href="https://gitlab.com/biolds1/sosse">Gitlab</a>.
     </p>
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
 {% extends "se/base.html" %} {% block body %}
-SOSSE is a Selenium based Open Source Search Engine.
+SOSSE is a Selenium based Open Source Search Engine {{ animal }}.
 It is distributed under the GNU_Affero_General_Public_License_version_3.
 You can download a copy of its source code on Gitlab.
 SOSSE {{ settings.SOSSE_VERSION_TAG }} {% if settings.SOSSE_VERSION_TAG !=
 'dev' %} ({{ settings.SOSSE_VERSION_COMMIT }}) {% endif %} - Copyright 2022-
 2023 Laurent Defert. {% endblock %}
```

### Comparing `sosse-1.0.0/se/templates/se/base.html` & `sosse-1.0.1/se/templates/se/base.html`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/templates/se/cached.html` & `sosse-1.0.1/se/templates/se/cached.html`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/templates/se/history.html` & `sosse-1.0.1/se/templates/se/history.html`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/templates/se/index.html` & `sosse-1.0.1/se/templates/se/index.html`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/templates/se/main_menu.html` & `sosse-1.0.1/se/templates/se/main_menu.html`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/templates/se/opensearch.xml` & `sosse-1.0.1/se/templates/se/opensearch.xml`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/templates/se/pagination.html` & `sosse-1.0.1/se/templates/se/pagination.html`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/templates/se/prefs.html` & `sosse-1.0.1/se/templates/se/prefs.html`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/templates/se/screenshot.html` & `sosse-1.0.1/se/templates/se/screenshot.html`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/templates/se/search_redirect.html` & `sosse-1.0.1/se/templates/se/search_redirect.html`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/templates/se/stats.html` & `sosse-1.0.1/se/templates/se/stats.html`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/templates/se/unknown_url.html` & `sosse-1.0.1/se/templates/se/unknown_url.html`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/test_cookie.py` & `sosse-1.0.1/se/test_cookie.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/test_crawl.py` & `sosse-1.0.1/se/test_crawl.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/test_functionals.py` & `sosse-1.0.1/se/test_functionals.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/test_misc.py` & `sosse-1.0.1/se/test_misc.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/test_parser.py` & `sosse-1.0.1/se/test_parser.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/test_redirect.py` & `sosse-1.0.1/se/test_redirect.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/test_requests.py` & `sosse-1.0.1/se/test_requests.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/test_search.py` & `sosse-1.0.1/se/test_search.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/test_url.py` & `sosse-1.0.1/se/test_url.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/test_views.py` & `sosse-1.0.1/se/test_views.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/utils.py` & `sosse-1.0.1/se/utils.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/views.py` & `sosse-1.0.1/se/views.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/words.py` & `sosse-1.0.1/se/words.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/se/www.py` & `sosse-1.0.1/se/www.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/sosse/conf.py` & `sosse-1.0.1/sosse/conf.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/sosse/search_engines.json` & `sosse-1.0.1/sosse/search_engines.json`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/sosse/settings.py` & `sosse-1.0.1/sosse/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,9 +325,9 @@
         'name': 'chinese',
         'flag': '🇹🇼'
     }
 }
 
 globals().update(Conf.get())
 
-SOSSE_VERSION_TAG = '1.0.0'
-SOSSE_VERSION_COMMIT = '7875a44a'
+SOSSE_VERSION_TAG = '1.0.1'
+SOSSE_VERSION_COMMIT = '90f57b03'
```

### Comparing `sosse-1.0.0/sosse/sosse_admin.py` & `sosse-1.0.1/sosse/sosse_admin.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/sosse/urls.py` & `sosse-1.0.1/sosse/urls.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/sosse/wsgi.py` & `sosse-1.0.1/sosse/wsgi.py`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/sosse.egg-info/PKG-INFO` & `sosse-1.0.1/sosse.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosse
-Version: 1.0.0
+Version: 1.0.1
 Summary: Selenium Open Source Search Engine
 Author-email: Laurent Defert <laurent_defert@yahoo.fr>
 License: GNU Affero General Public License v3
 Keywords: search engine,crawler
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
@@ -15,15 +15,15 @@
   <img src="https://raw.githubusercontent.com/biolds/sosse/main/se/static/se/logo.svg" width="64" align="right">
   <a href="https://gitlab.com/biolds1/sosse/" alt="Gitlab code coverage">
     <img src="https://img.shields.io/gitlab/pipeline-coverage/biolds1/sosse?branch=main&style=flat-square">
   </a>
   <a href="https://gitlab.com/biolds1/sosse/-/pipelines" alt="Gitlab pipeline status">
     <img src="https://img.shields.io/gitlab/pipeline-status/biolds1/sosse?branch=main&style=flat-square">
   </a>
-  <a href="https://sosse.readthedocs.io/en/latest/" alt="Documentation">
+  <a href="https://sosse.readthedocs.io/en/stable/" alt="Documentation">
     <img src="https://img.shields.io/readthedocs/sosse?style=flat-square">
   </a>
   <a href="https://gitlab.com/biolds1/sosse/-/blob/main/LICENSE" alt="License">
     <img src="https://img.shields.io/gitlab/license/biolds1/sosse?style=flat-square">
   </a>
 </p>
 
@@ -36,26 +36,26 @@
 - 🌍 Browser based crawling: the crawler can use [Google Chromium](https://www.chromium.org/Home) and [Selenium](https://www.selenium.dev/) to index pages that use Javascript. [Requests](https://docs.python-requests.org/en/latest/index.html) can also be used for faster crawling
 - 🏖 Low resources requirements: SOSSE is entirely written in Python and uses [PostgreSQL](https://www.postgresql.org/) for data storage
 - 🖼 Offline cache: SOSSE can take screenshots of crawled pages and make them browsable offline
 - 🔓 Authentication: the crawlers can submit authentication forms with provided credentials
 - 🔗 Search engines shortcuts: shortcuts search queries can be used to redirect to external search engines (sometime called "bang" searches)
 - 🔖 Search history: users can authenticate to log their search query history privately
 
-See the [documentation](https://sosse.readthedocs.io/en/latest/) and [screenshots](https://sosse.readthedocs.io/en/latest/).
+See the [documentation](https://sosse.readthedocs.io/en/stable/) and [screenshots](https://sosse.readthedocs.io/en/stable/screenshots.html).
 
 Try it out
 ==========
 
 You can try the latest version with Docker:
 
 ```
 docker run -p 8005:80 biolds/sosse:latest
 ```
 
-Default user is ``admin``, with password ``admin``.
+Connect to port 8005, and log in with user ``admin``, with password ``admin``.
 
-You can also find alternative installation methods in the [documentation](https://sosse.readthedocs.io/en/latest/install.html).
+To persist Docker data, or find alternative installation methods, please check the [documentation](https://sosse.readthedocs.io/en/stable/install.html).
 
 Keep in touch
 =============
 
 Join the [Discord server](https://discord.gg/Vt9cMf7BGK) to get help and share ideas!
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sosse Version: 1.0.0 Summary: Selenium Open Source
+Metadata-Version: 2.1 Name: sosse Version: 1.0.1 Summary: Selenium Open Source
 Search Engine Author-email: Laurent Defert
 yahoo.fr> License: GNU Affero General Public License v3 Keywords: search
 engine,crawler Classifier: Framework :: Django Classifier: Programming Language
 :: Python :: 3 Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE
 [https://raw.githubusercontent.com/biolds/sosse/main/se/static/se/logo.svg]
 [https://img.shields.io/gitlab/pipeline-coverage/biolds1/
@@ -24,14 +24,15 @@
 Python and uses [PostgreSQL](https://www.postgresql.org/) for data storage -
 ð¼ Offline cache: SOSSE can take screenshots of crawled pages and make them
 browsable offline - ð Authentication: the crawlers can submit authentication
 forms with provided credentials - ð Search engines shortcuts: shortcuts
 search queries can be used to redirect to external search engines (sometime
 called "bang" searches) - ð Search history: users can authenticate to log
 their search query history privately See the [documentation](https://
-sosse.readthedocs.io/en/latest/) and [screenshots](https://
-sosse.readthedocs.io/en/latest/). Try it out ========== You can try the latest
-version with Docker: ``` docker run -p 8005:80 biolds/sosse:latest ``` Default
-user is ``admin``, with password ``admin``. You can also find alternative
-installation methods in the [documentation](https://sosse.readthedocs.io/en/
-latest/install.html). Keep in touch ============= Join the [Discord server]
-(https://discord.gg/Vt9cMf7BGK) to get help and share ideas!
+sosse.readthedocs.io/en/stable/) and [screenshots](https://
+sosse.readthedocs.io/en/stable/screenshots.html). Try it out ========== You can
+try the latest version with Docker: ``` docker run -p 8005:80 biolds/sosse:
+latest ``` Connect to port 8005, and log in with user ``admin``, with password
+``admin``. To persist Docker data, or find alternative installation methods,
+please check the [documentation](https://sosse.readthedocs.io/en/stable/
+install.html). Keep in touch ============= Join the [Discord server](https://
+discord.gg/Vt9cMf7BGK) to get help and share ideas!
```

### Comparing `sosse-1.0.0/sosse.egg-info/SOURCES.txt` & `sosse-1.0.1/sosse.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 .coveragerc
 .gitignore
 .gitlab-ci.yml
 .readthedocs.yaml
+CHANGELOG.md
 Dockerfile
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 pyproject.toml
 requirements.txt
 sosse-admin
+.gitlab/changelog_config.yml
 debian/changelog
 debian/compat
 debian/control
 debian/rules
 debian/sosse-crawler.service
 debian/sosse-uwsgi.service
 debian/sosse.conf
 debian/sosse.install
 debian/sosse.postinst
 debian/uwsgi.ini
 debian/uwsgi.params
 doc/Makefile
+doc/build_changelog.sh
 doc/get_artifacts.py
 doc/make.bat
 doc/requirements.txt
 doc/source/admin_ui.rst
 doc/source/administration.rst
 doc/source/authentication.rst
 doc/source/cli.rst
@@ -69,14 +72,16 @@
 docker/debian-pkg/Makefile
 docker/debian-test/Dockerfile
 docker/debian-test/Makefile
 docker/doc/Dockerfile
 docker/doc/Makefile
 docker/pip-base/Dockerfile
 docker/pip-base/Makefile
+docker/pip-release/Dockerfile
+docker/pip-release/Makefile
 docker/pip-test/Dockerfile
 docker/pip-test/Makefile
 se/__init__.py
 se/admin.py
 se/apps.py
 se/atom.py
 se/browser.py
```

### Comparing `sosse-1.0.0/tests/cookies.json` & `sosse-1.0.1/tests/cookies.json`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/tests/doc_test.sh` & `sosse-1.0.1/tests/doc_test.sh`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/tests/document-ja.json` & `sosse-1.0.1/tests/document-ja.json`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/tests/robotframework/start.sh` & `sosse-1.0.1/tests/robotframework/start.sh`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/tests/robotframework/tests/01_crawl.robot` & `sosse-1.0.1/tests/robotframework/tests/01_crawl.robot`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/tests/robotframework/tests/02_user.robot` & `sosse-1.0.1/tests/robotframework/tests/02_user.robot`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/tests/robotframework/tests/common.robot` & `sosse-1.0.1/tests/robotframework/tests/common.robot`

 * *Files identical despite different names*

### Comparing `sosse-1.0.0/tests/test_app.sh` & `sosse-1.0.1/tests/test_app.sh`

 * *Files identical despite different names*

