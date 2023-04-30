# Comparing `tmp/pan-threat-vault-python-0.2.0.tar.gz` & `tmp/pan-threat-vault-python-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pan-threat-vault-python-0.2.0.tar", last modified: Tue Apr  4 20:55:07 2023, max compression
+gzip compressed data, was "pan-threat-vault-python-0.3.0.tar", last modified: Sun Apr 30 22:53:54 2023, max compression
```

## Comparing `pan-threat-vault-python-0.2.0.tar` & `pan-threat-vault-python-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,19 @@
-drwxr-xr-x   0 ksteves   (1000) ksteves   (1000)        0 2023-04-04 20:55:07.031204 pan-threat-vault-python-0.2.0/
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)      822 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/LICENSE.txt
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     1279 2023-04-04 20:55:07.031204 pan-threat-vault-python-0.2.0/PKG-INFO
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)      791 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/README.rst
-drwxr-xr-x   0 ksteves   (1000) ksteves   (1000)        0 2023-04-04 20:55:06.971205 pan-threat-vault-python-0.2.0/bin/
--rwxr-xr-x   0 ksteves   (1000) ksteves   (1000)    23704 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/bin/tvapi.py
-drwxr-xr-x   0 ksteves   (1000) ksteves   (1000)        0 2023-04-04 20:55:06.983193 pan-threat-vault-python-0.2.0/pan_threat_vault_python.egg-info/
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     1279 2023-04-04 20:55:06.000000 pan-threat-vault-python-0.2.0/pan_threat_vault_python.egg-info/PKG-INFO
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     1107 2023-04-04 20:55:06.000000 pan-threat-vault-python-0.2.0/pan_threat_vault_python.egg-info/SOURCES.txt
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)        1 2023-04-04 20:55:06.000000 pan-threat-vault-python-0.2.0/pan_threat_vault_python.egg-info/dependency_links.txt
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)       32 2023-04-04 20:55:06.000000 pan-threat-vault-python-0.2.0/pan_threat_vault_python.egg-info/requires.txt
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)        6 2023-04-04 20:55:06.000000 pan-threat-vault-python-0.2.0/pan_threat_vault_python.egg-info/top_level.txt
-drwxr-xr-x   0 ksteves   (1000) ksteves   (1000)        0 2023-04-04 20:55:06.991206 pan-threat-vault-python-0.2.0/pantv/
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     2685 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/pantv/__init__.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     5295 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/pantv/mixin.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)    11809 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/pantv/v1aioapi.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)    10893 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/pantv/v1api.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)       90 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/pyproject.toml
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)      655 2023-04-04 20:55:07.031204 pan-threat-vault-python-0.2.0/setup.cfg
-drwxr-xr-x   0 ksteves   (1000) ksteves   (1000)        0 2023-04-04 20:55:07.021206 pan-threat-vault-python-0.2.0/tests/
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     1287 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/tests/test_aio_atp_reports.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)      907 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/tests/test_aio_atp_reports_pcaps.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)      856 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/tests/test_aio_constructor.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)      801 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/tests/test_aio_release_notes.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     1600 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/tests/test_aio_release_notes_2.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     4796 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/tests/test_aio_threats.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     3631 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/tests/test_aio_threats2.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     2277 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/tests/test_aio_threats2_2.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     2422 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/tests/test_aio_threats_2.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     3969 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/tests/test_aio_threats_history.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     2395 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/tests/test_aio_threats_history_2.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     1210 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/tests/test_noaio_atp_reports.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)      850 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/tests/test_noaio_atp_reports_pcaps.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)      837 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/tests/test_noaio_constructor.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)      764 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/tests/test_noaio_release_notes.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     1511 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/tests/test_noaio_release_notes_2.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     4634 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/tests/test_noaio_threats.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     3522 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/tests/test_noaio_threats2.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     2142 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/tests/test_noaio_threats2_2.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     2293 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/tests/test_noaio_threats_2.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     2731 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/tests/test_noaio_threats_content_sync.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     3906 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/tests/test_noaio_threats_history.py
--rw-r--r--   0 ksteves   (1000) ksteves   (1000)     2268 2023-04-04 20:53:51.000000 pan-threat-vault-python-0.2.0/tests/test_noaio_threats_history_2.py
+drwxr-xr-x   0 ksteves   (1000) ksteves   (1000)        0 2023-04-30 22:53:54.461390 pan-threat-vault-python-0.3.0/
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)      822 2023-04-30 22:53:03.000000 pan-threat-vault-python-0.3.0/LICENSE.txt
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)     1279 2023-04-30 22:53:54.461390 pan-threat-vault-python-0.3.0/PKG-INFO
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)      791 2023-04-30 22:53:03.000000 pan-threat-vault-python-0.3.0/README.rst
+drwxr-xr-x   0 ksteves   (1000) ksteves   (1000)        0 2023-04-30 22:53:54.451390 pan-threat-vault-python-0.3.0/bin/
+-rwxr-xr-x   0 ksteves   (1000) ksteves   (1000)    26681 2023-04-30 22:53:03.000000 pan-threat-vault-python-0.3.0/bin/tvapi.py
+drwxr-xr-x   0 ksteves   (1000) ksteves   (1000)        0 2023-04-30 22:53:54.461390 pan-threat-vault-python-0.3.0/pan_threat_vault_python.egg-info/
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)     1279 2023-04-30 22:53:54.000000 pan-threat-vault-python-0.3.0/pan_threat_vault_python.egg-info/PKG-INFO
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)      360 2023-04-30 22:53:54.000000 pan-threat-vault-python-0.3.0/pan_threat_vault_python.egg-info/SOURCES.txt
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)        1 2023-04-30 22:53:54.000000 pan-threat-vault-python-0.3.0/pan_threat_vault_python.egg-info/dependency_links.txt
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)       32 2023-04-30 22:53:54.000000 pan-threat-vault-python-0.3.0/pan_threat_vault_python.egg-info/requires.txt
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)        6 2023-04-30 22:53:54.000000 pan-threat-vault-python-0.3.0/pan_threat_vault_python.egg-info/top_level.txt
+drwxr-xr-x   0 ksteves   (1000) ksteves   (1000)        0 2023-04-30 22:53:54.461390 pan-threat-vault-python-0.3.0/pantv/
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)     2685 2023-04-30 22:53:03.000000 pan-threat-vault-python-0.3.0/pantv/__init__.py
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)     5295 2023-04-30 22:53:03.000000 pan-threat-vault-python-0.3.0/pantv/mixin.py
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)    14365 2023-04-30 22:53:03.000000 pan-threat-vault-python-0.3.0/pantv/v1aioapi.py
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)    13170 2023-04-30 22:53:03.000000 pan-threat-vault-python-0.3.0/pantv/v1api.py
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)       90 2023-04-30 22:53:03.000000 pan-threat-vault-python-0.3.0/pyproject.toml
+-rw-r--r--   0 ksteves   (1000) ksteves   (1000)      655 2023-04-30 22:53:54.471390 pan-threat-vault-python-0.3.0/setup.cfg
```

### Comparing `pan-threat-vault-python-0.2.0/LICENSE.txt` & `pan-threat-vault-python-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pan-threat-vault-python-0.2.0/PKG-INFO` & `pan-threat-vault-python-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pan-threat-vault-python
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python interface to the Palo Alto Networks Threat Vault API
 Home-page: https://github.com/PaloAltoNetworks/pan-threat-vault-python
 Author: Palo Alto Networks, Inc.
 Author-email: devrel@paloaltonetworks.com
 License: ISC
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

### Comparing `pan-threat-vault-python-0.2.0/README.rst` & `pan-threat-vault-python-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `pan-threat-vault-python-0.2.0/bin/tvapi.py` & `pan-threat-vault-python-0.3.0/bin/tvapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -198,22 +198,61 @@
             limit=options['limit'],
             query_string=options['query_string_obj'])
         print_status('threats-history', resp)
         print_response(options, resp)
         resp.raise_for_status()
 
     elif options['release-notes']:
+        version = (options['content-version']
+                   if options['content-version'] is not None
+                   else options['note-version'])
         resp = api.release_notes(
             type=options['type'],
-            version=options['note-version'],
+            version=version,
             query_string=options['query_string_obj'])
         print_status('release-notes', resp)
         print_response(options, resp)
         resp.raise_for_status()
 
+    elif options['edl']:
+        name = options['name'][0] if options['name'] is not None else None
+        kwargs = {
+            'name': name,
+            'version': options['content-version'],
+            'offset': options['offset'],
+            'limit': options['limit'],
+            'query_string': options['query_string_obj'],
+        }
+
+        if options['all'] and options['opt_json']:
+            # only allowed with noaio
+            kwargs['retry'] = True
+            edl = GeneratorList(generator=api.edl_all, **kwargs)
+            for x in json.JSONEncoder().iterencode(edl):
+                if options['print_json']:
+                    # XXX warn if not print_json?
+                    print(x, end='')
+
+        elif options['all']:
+            obj = {'data': []}
+            for ok, x in api.edl_all(retry=True, **kwargs):
+                if ok:
+                    obj['data'].append(x)
+                else:
+                    print_status('edl_all', x)
+                    print_response(options, x)
+                    x.raise_for_status()
+            print_json_response(options, obj)
+
+        else:
+            resp = api.edl(**kwargs)
+            print_status('edl', resp)
+            print_response(options, resp)
+            resp.raise_for_status()
+
     elif options['atp-reports']:
         resp = api.atp_reports(
             id=options['id'],
             data=options['data'],
             query_string=options['query_string_obj'])
         print_status('atp-reports', resp)
         print_response(options, resp)
@@ -287,22 +326,52 @@
             limit=options['limit'],
             query_string=options['query_string_obj'])
         print_status('threats-history', resp)
         await aioprint_response(options, resp)
         resp.raise_for_status()
 
     elif options['release-notes']:
+        version = (options['content-version']
+                   if options['content-version'] is not None
+                   else options['note-version'])
         resp = await api.release_notes(
             type=options['type'],
-            version=options['note-version'],
+            version=version,
             query_string=options['query_string_obj'])
         print_status('release-notes', resp)
         await aioprint_response(options, resp)
         resp.raise_for_status()
 
+    elif options['edl']:
+        name = options['name'][0] if options['name'] is not None else None
+        kwargs = {
+            'name': name,
+            'version': options['content-version'],
+            'offset': options['offset'],
+            'limit': options['limit'],
+            'query_string': options['query_string_obj'],
+        }
+
+        if options['all']:
+            obj = {'data': []}
+            async for ok, x in api.edl_all(retry=True, **kwargs):
+                if ok:
+                    obj['data'].append(x)
+                else:
+                    print_status('edl_all', x)
+                    await aioprint_response(options, x)
+                    x.raise_for_status()
+            print_json_response(options, obj)
+
+        else:
+            resp = await api.edl(**kwargs)
+            print_status('edl', resp)
+            await aioprint_response(options, resp)
+            resp.raise_for_status()
+
     elif options['atp-reports']:
         resp = await api.atp_reports(
             id=options['id'],
             data=options['data'],
             query_string=options['query_string_obj'])
         print_status('atp-reports', resp)
         await aioprint_response(options, resp)
@@ -463,24 +532,26 @@
         'api-version': None,
         'url': None,
         'api-key': None,
         'threats': False,
         'threats2': False,
         'threats_history': False,
         'release-notes': False,
+        'edl': False,
         'atp-reports': False,
         'atp-pcaps': False,
         'all': False,
         'id': None,
         'cve': None,
         'name': None,
         'sha256': None,
         'md5': None,
         'type': None,
-        'note-version': None,
+        'content-version': None,
+        'note-version': None,  # XXX deprecated
         'data': None,
         'offset': None,
         'limit': None,
         'query_strings': [],
         'query_string_obj': None,
         'verify': None,
         'aio': True,
@@ -495,18 +566,19 @@
         'dtime': False,
     }
 
     short_options = 'F:J:jOpQ:'
     long_options = [
         'help', 'version', 'debug=', 'dtime',
         'api-version=', 'url=', 'api-key=',
-        'threats', 'threats2', 'threats-history', 'release-notes',
+        'threats', 'threats2', 'threats-history',
+        'release-notes', 'edl',
         'atp-reports', 'atp-pcaps',
         'all', 'id=', 'name=', 'cve=', 'sha256=', 'md5=',
-        'type=', 'note-version=', 'data=',
+        'type=', 'content-version=', 'note-version=', 'data=',
         'offset=', 'limit=',
         'rate-limits', 'dst=', 'verify=', 'aio', 'noaio',
         'timeout=',
     ]
 
     try:
         opts, args = getopt.getopt(sys.argv[1:],
@@ -537,14 +609,16 @@
             options['threats'] = True
         elif opt == '--threats2':
             options['threats2'] = True
         elif opt == '--threats-history':
             options['threats_history'] = True
         elif opt == '--release-notes':
             options['release-notes'] = True
+        elif opt == '--edl':
+            options['edl'] = True
         elif opt == '--atp-reports':
             options['atp-reports'] = True
         elif opt == '--atp-pcaps':
             options['atp-pcaps'] = True
         elif opt == '--all':
             options['all'] = True
         elif opt == '--id':
@@ -563,15 +637,17 @@
             options['sha256'].extend(process_arg(arg))
         elif opt == '--md5':
             if options['md5'] is None:
                 options['md5'] = []
             options['md5'].extend(process_arg(arg))
         elif opt == '--type':
             options['type'] = arg
-        elif opt == '--note-version':
+        elif opt == '--content-version':
+            options['content-version'] = arg
+        elif opt == '--note-version':  # XXX deprecated
             options['note-version'] = arg
         elif opt == '--data':
             options['data'] = process_arg(arg, string=True)
         elif opt == '--offset':
             options['offset'] = arg
         elif opt == '--limit':
             options['limit'] = arg
@@ -668,51 +744,53 @@
         print(pprint.pformat(x), file=sys.stderr)
 
     return options
 
 
 def usage():
     usage = '''%s [options]
-    --api-key key            API key
-    --threats                threats API request
-    --threats2               multiple threats bulk API request
-    --threats-history        threats release history API request
-    --release-notes          release-notes API request
-    --atp-reports            ATP reports API request
-    --atp-pcaps              ATP reports pcaps API request
-    --all                    get all threats
-    --id id                  signature/report ID (multiple --id's allowed)
-    --name name              signature name (multiple --name's allowed)
-    --cve id                 CVE ID
-    --sha256 hash            SHA-256 hash (multiple --sha256's allowed)
-    --md5 hash               MD5 hash (multiple --md5's allowed)
-    --type type              signature/release-note type
-    --note-version version   release-note version
-    --offset num             items offset
-    --limit num              number of items to return
-    -Q json                  URL query string (multiple -Q's allowed)
-    --data json              threats2, atp-reports POST data
-    --url url                API URL
-                             default %s
-    --verify opt             SSL server verify option: yes|no|path
-    --aio                    Use asyncio (default)
-    --noaio                  Don't use asyncio
-    --api-version version    API version (default %s)
-    -j                       print JSON
-    -p                       print Python
-    --rate-limits            print response header rate limits
-    --dst dst                save pcap to directory or path
-    -J expression            JMESPath expression for JSON response data
-    -O                       optimized get all with JSON only output
-    --timeout timeout        connect, read timeout
-    -F path                  JSON options (multiple -F's allowed)
-    --debug level            debug level (0-3)
-    --dtime                  add time string to debug output
-    --version                display version
-    --help                   display usage
+    --api-key key              API key
+    --threats                  threats API request
+    --threats2                 multiple threats bulk API request
+    --threats-history          threats release history API request
+    --release-notes            release-notes API request
+    --edl                      EDL (external dynamic list) API request
+    --atp-reports              ATP reports API request
+    --atp-pcaps                ATP reports pcaps API request
+    --all                      get all threats, EDL entries
+    --id id                    signature/report ID (multiple --id's allowed)
+    --name name                signature name (multiple --name's allowed)
+                               EDL name
+    --cve id                   CVE ID
+    --sha256 hash              SHA-256 hash (multiple --sha256's allowed)
+    --md5 hash                 MD5 hash (multiple --md5's allowed)
+    --type type                signature/release-note type
+    --content-version version  content version for release-notes, EDL
+    --offset num               items offset
+    --limit num                number of items to return
+    -Q json                    URL query string (multiple -Q's allowed)
+    --data json                threats2, atp-reports POST data
+    --url url                  API URL
+                               default %s
+    --verify opt               SSL server verify option: yes|no|path
+    --aio                      Use asyncio (default)
+    --noaio                    Don't use asyncio
+    --api-version version      API version (default %s)
+    -j                         print JSON
+    -p                         print Python
+    --rate-limits              print response header rate limits
+    --dst dst                  save pcap to directory or path
+    -J expression              JMESPath expression for JSON response data
+    -O                         optimized get all with JSON only output
+    --timeout timeout          connect, read timeout
+    -F path                    JSON options (multiple -F's allowed)
+    --debug level              debug level (0-3)
+    --dtime                    add time string to debug output
+    --version                  display version
+    --help                     display usage
 '''
     print(usage % (os.path.basename(sys.argv[0]),
                    DEFAULT_URL, DEFAULT_API_VERSION), end='')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pan-threat-vault-python-0.2.0/pan_threat_vault_python.egg-info/PKG-INFO` & `pan-threat-vault-python-0.3.0/pan_threat_vault_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pan-threat-vault-python
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python interface to the Palo Alto Networks Threat Vault API
 Home-page: https://github.com/PaloAltoNetworks/pan-threat-vault-python
 Author: Palo Alto Networks, Inc.
 Author-email: devrel@paloaltonetworks.com
 License: ISC
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: ISC License (ISCL)
```

### Comparing `pan-threat-vault-python-0.2.0/pantv/__init__.py` & `pan-threat-vault-python-0.3.0/pantv/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import asyncio
 from collections import namedtuple
 import logging
 import re
 import sys
 
-__version__ = '0.2.0'
+__version__ = '0.3.0'
 title = 'pan-threat-vault-python'
 
 _default_api_version = (1)
 DEFAULT_API_VERSION = 'v%d' % _default_api_version
 
 DEFAULT_URL = 'https://api.threatvault.paloaltonetworks.com'
```

### Comparing `pan-threat-vault-python-0.2.0/pantv/mixin.py` & `pan-threat-vault-python-0.3.0/pantv/mixin.py`

 * *Files identical despite different names*

### Comparing `pan-threat-vault-python-0.2.0/pantv/v1aioapi.py` & `pan-threat-vault-python-0.3.0/pantv/v1api.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,81 +10,73 @@
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 #
 
-import aiohttp
-import asyncio
 import logging
+import requests
 import ssl
 import sys
 import time
 
 from . import (mixin, ApiError, ArgsError,
                DEBUG1, DEBUG2, DEBUG3,
                title, __version__,
                DEFAULT_URL)
 
 
 BASE_PATH = '/service/v1'
 
 
-class ThreatVaultApi(mixin.AioMixin):
+class ThreatVaultApi(mixin.Mixin):
     def __init__(self, *,
                  api_version=None,
                  url=None,
                  api_key=None,
                  verify=None,
                  timeout=None):
-
         self._log = logging.getLogger(__name__).log
         self._log(DEBUG2, '%s: %s, ThreatVaultApi: %s',
                   title, __version__, api_version)
         self._log(DEBUG2, 'Python version: %s', sys.version)
         self._log(DEBUG2, 'ssl: %s', ssl.OPENSSL_VERSION)
-        self._log(DEBUG2, 'aiohttp: %s', aiohttp.__version__)
+        self._log(DEBUG2, 'requests: %s', requests.__version__)
 
         self.api_version = api_version
         if url is None:
             self.url = DEFAULT_URL
         else:
             self.url = url
-        try:
-            self.ssl = self._ssl_context(verify)
-        except ValueError as e:
-            raise ArgsError(e)
-        self._log(DEBUG2, 'ssl: %s %s', self.ssl.verify_mode,
-                  self.ssl.check_hostname)
         auth = self._auth(api_key)
-        timeout_ = self._timeout(timeout)
-        self._log(DEBUG2, 'timeout: %s', timeout_)
-        self.session = self._session(auth=auth, timeout=timeout_)
-
-    async def _request_retry(self, *,
-                             retry=False,
-                             retry_timeout=False,
-                             func=None,
-                             **kwargs):
+        self.session = self._session(auth=auth,
+                                     verify=verify,
+                                     timeout=timeout)
+
+    def _request_retry(self, *,
+                       retry=False,
+                       retry_timeout=False,
+                       func=None,
+                       **kwargs):
         if retry_timeout:
             timeout_delay = 5
             timeout_retries = 3
         while True:
             try:
-                resp = await func(**kwargs)
-            except asyncio.TimeoutError:
+                resp = func(**kwargs)
+            except requests.Timeout:
                 if not (retry_timeout and timeout_retries):
                     raise
                 self._log(DEBUG2, 'timeout, sleep %.2fs', timeout_delay)
-                await asyncio.sleep(timeout_delay)
+                time.sleep(timeout_delay)
                 timeout_delay *= 2
                 timeout_retries -= 1
             else:
-                if retry and resp.status == 429:
+                if retry and resp.status_code == 429:
                     now = time.time()
                     day_remaining = \
                         resp.headers.get('x-day-ratelimit-remaining')
                     if day_remaining is None or day_remaining == '0':
                         break
 
                     minute_reset = \
@@ -97,38 +89,38 @@
                         self._log(DEBUG1, '%s', e)
                         break
 
                     if minute_reset > now:
                         rate_limit_delay = minute_reset - now
                         self._log(DEBUG2, 'status code 429, sleep %.2fs',
                                   rate_limit_delay)
-                        await asyncio.sleep(rate_limit_delay)
+                        time.sleep(rate_limit_delay)
                 else:
                     break
 
         return resp
 
-    async def threats(self, *,
-                      type=None,
-                      id=None,
-                      name=None,
-                      cve=None,
-                      vendor=None,
-                      fromReleaseDate=None,
-                      toReleaseDate=None,
-                      fromReleaseVersion=None,
-                      toReleaseVersion=None,
-                      releaseDate=None,
-                      releaseVersion=None,
-                      sha256=None,
-                      md5=None,
-                      offset=None,
-                      limit=None,
-                      query_string=None,
-                      retry=False):
+    def threats(self, *,
+                type=None,
+                id=None,
+                name=None,
+                cve=None,
+                vendor=None,
+                fromReleaseDate=None,
+                toReleaseDate=None,
+                fromReleaseVersion=None,
+                toReleaseVersion=None,
+                releaseDate=None,
+                releaseVersion=None,
+                sha256=None,
+                md5=None,
+                offset=None,
+                limit=None,
+                query_string=None,
+                retry=False):
         args = locals()
         path = BASE_PATH + '/threats'
         url = self.url + path
 
         params = {}
         for x in args:
             if (x not in ('self', 'query_string', 'retry') and
@@ -136,26 +128,29 @@
                 params[x] = args[x]
 
         if query_string is not None:
             params.update(query_string)
 
         kwargs = {
             'url': url,
-            'ssl': self.ssl,
             'params': params,
         }
 
-        resp = await self._request_retry(retry=retry,
-                                         func=self.session.get,
-                                         **kwargs)
+        resp = self._request_retry(retry=retry,
+                                   func=self.session.get,
+                                   **kwargs)
 
         return resp
 
-    async def threats_all(self,
-                          **kwargs):
+    def _all(self, *,
+             func,
+             **kwargs):
+        assert func == self.threats or func == self.edl, \
+            'func not threats() or edl()'
+
         if 'offset' not in kwargs or kwargs['offset'] is None:
             kwargs['offset'] = 0
         else:
             try:
                 kwargs['offset'] = int(kwargs['offset'])
             except ValueError as e:
                 raise ArgsError('offset not int')
@@ -167,59 +162,89 @@
             try:
                 limit = int(kwargs['limit'])
             except ValueError as e:
                 raise ArgsError('limit not int')
 
         total = 0
         while True:
-            resp = await self.threats(**kwargs)
-            if resp.status == 200:
-                obj = await resp.json(content_type=None)
-                try:
-                    threats = [obj['data'][k] for k in obj['data']]
-                    count = obj['count']
-                except KeyError as e:
-                    raise ApiError('Malformed response, missing key %s' % e)
-                current = 0
-                for threat in threats:
-                    current += len(threat)
-                total += current
-                self._log(DEBUG1, 'count %d current %d total %d',
-                          count, current, total)
-                for threat in threats:
-                    for x in threat:
+            resp = func(**kwargs)
+            if resp.status_code == 200:
+                obj = resp.json()
+                if func == self.threats:
+                    try:
+                        threats = [obj['data'][k] for k in obj['data']]
+                        count = obj['count']
+                    except KeyError as e:
+                        raise ApiError('Malformed response, '
+                                       'missing key %s' % e)
+                    current = 0
+                    for threat in threats:
+                        current += len(threat)
+                    total += current
+                    self._log(DEBUG1, 'count %d current %d total %d',
+                              count, current, total)
+                    for threat in threats:
+                        for x in threat:
+                            yield True, x
+
+                elif func == self.edl:
+                    try:
+                        if isinstance(obj['data'], list):
+                            ips = obj['data']
+                        elif (isinstance(obj['data'], dict) and
+                              'ipaddr' in obj['data']):
+                            ips = obj['data']['ipaddr']
+                        else:
+                            raise ApiError('Malformed response, '
+                                           'data not list or dict')
+                        count = obj['count']
+                    except KeyError as e:
+                        raise ApiError('Malformed response, '
+                                       'missing key %s' % e)
+                    current = len(ips)
+                    total += current
+                    self._log(DEBUG1, 'count %d current %d total %d',
+                              count, current, total)
+                    for x in ips:
                         yield True, x
 
                 if total >= count:
                     break
 
                 kwargs['offset'] += limit
             else:
                 yield False, resp
 
-    async def threats2(self, *,
-                       type=None,
-                       id=None,
-                       name=None,
-                       sha256=None,
-                       md5=None,
-                       data=None,
-                       query_string=None,
-                       retry=False):
+    def threats_all(self,
+                    **kwargs):
+        return self._all(func=self.threats, **kwargs)
+
+    def edl_all(self,
+                **kwargs):
+        return self._all(func=self.edl, **kwargs)
+
+    def threats2(self, *,
+                 type=None,
+                 id=None,
+                 name=None,
+                 sha256=None,
+                 md5=None,
+                 data=None,
+                 query_string=None,
+                 retry=False):
         args = locals()
         path = BASE_PATH + '/threats'
         url = self.url + path
 
         params = {}
         if query_string is not None:
             params.update(query_string)
 
         kwargs = {
             'url': url,
-            'ssl': self.ssl,
             'params': params,
         }
         if data is not None:
             if isinstance(data, (bytes, str, bytearray)):
                 kwargs['data'] = data
                 kwargs['headers'] = {'content-type': 'application/json'}
             else:
@@ -229,28 +254,28 @@
                 if (x not in ('self', 'query_string', 'retry') and
                    args[x] is not None):
                     if 'json' in kwargs:
                         kwargs['json'].update({x: args[x]})
                     else:
                         kwargs['json'] = {x: args[x]}
 
-        resp = await self._request_retry(retry=retry,
-                                         func=self.session.post,
-                                         **kwargs)
+        resp = self._request_retry(retry=retry,
+                                   func=self.session.post,
+                                   **kwargs)
 
         return resp
 
-    async def threats_history(self, *,
-                              type=None,
-                              id=None,
-                              order=None,
-                              offset=None,
-                              limit=None,
-                              query_string=None,
-                              retry=False):
+    def threats_history(self, *,
+                        type=None,
+                        id=None,
+                        order=None,
+                        offset=None,
+                        limit=None,
+                        query_string=None,
+                        retry=False):
         args = locals()
         path = BASE_PATH + '/threats/history'
         url = self.url + path
 
         params = {}
         for x in args:
             if (x not in ('self', 'query_string', 'retry') and
@@ -258,29 +283,28 @@
                 params[x] = args[x]
 
         if query_string is not None:
             params.update(query_string)
 
         kwargs = {
             'url': url,
-            'ssl': self.ssl,
             'params': params,
         }
 
-        resp = await self._request_retry(retry=retry,
-                                         func=self.session.get,
-                                         **kwargs)
+        resp = self._request_retry(retry=retry,
+                                   func=self.session.get,
+                                   **kwargs)
 
         return resp
 
-    async def release_notes(self, *,
-                            type=None,
-                            version=None,
-                            query_string=None,
-                            retry=False):
+    def release_notes(self, *,
+                      type=None,
+                      version=None,
+                      query_string=None,
+                      retry=False):
         args = locals()
         path = BASE_PATH + '/release-notes'
         url = self.url + path
 
         params = {}
         for x in args:
             if (x not in ('self', 'query_string', 'retry') and
@@ -288,75 +312,105 @@
                 params[x] = args[x]
 
         if query_string is not None:
             params.update(query_string)
 
         kwargs = {
             'url': url,
-            'ssl': self.ssl,
             'params': params,
         }
 
-        resp = await self._request_retry(retry=retry,
-                                         func=self.session.get,
-                                         **kwargs)
+        resp = self._request_retry(retry=retry,
+                                   func=self.session.get,
+                                   **kwargs)
 
         return resp
 
-    async def atp_reports(self, *,
-                          id=None,
-                          query_string=None,
-                          data=None,
-                          retry=False):
+    def edl(self, *,
+            name=None,
+            ipaddr=None,
+            version=None,
+            listformat=None,
+            offset=None,
+            limit=None,
+            query_string=None,
+            retry=False):
+        args = locals()
+        path = BASE_PATH + '/edl'
+        url = self.url + path
+
+        params = {}
+        for x in args:
+            if (x not in ('self', 'query_string', 'retry') and
+               args[x] is not None):
+                params[x] = args[x]
+
+        if query_string is not None:
+            params.update(query_string)
+
+        kwargs = {
+            'url': url,
+            'params': params,
+        }
+
+        resp = self._request_retry(retry=retry,
+                                   func=self.session.get,
+                                   **kwargs)
+
+        return resp
+
+    def atp_reports(self, *,
+                    id=None,
+                    data=None,
+                    query_string=None,
+                    retry=False):
         path = BASE_PATH + '/atp/reports'
         url = self.url + path
 
         params = {}
         if query_string is not None:
             params.update(query_string)
 
         kwargs = {
             'url': url,
-            'ssl': self.ssl,
             'params': params,
         }
         if data is not None:
             if isinstance(data, (bytes, str, bytearray)):
                 kwargs['data'] = data
                 kwargs['headers'] = {'content-type': 'application/json'}
             else:
                 kwargs['json'] = data
         else:
             if id is not None:
                 kwargs['json'] = {'id': id}
 
-        resp = await self._request_retry(retry=retry,
-                                         func=self.session.post,
-                                         **kwargs)
+        resp = self._request_retry(retry=retry,
+                                   func=self.session.post,
+                                   **kwargs)
 
         return resp
 
-    async def atp_reports_pcaps(self, *,
-                                id=None,
-                                query_string=None,
-                                retry=False):
+    def atp_reports_pcaps(self, *,
+                          id=None,
+                          query_string=None,
+                          retry=False):
         path = BASE_PATH + '/atp/reports/pcaps'
         url = self.url + path
 
         params = {}
         if id is not None:
             params['id'] = id
 
         if query_string is not None:
             params.update(query_string)
 
         kwargs = {
             'url': url,
-            'ssl': self.ssl,
             'params': params,
         }
 
-        resp = await self._request_retry(retry=retry,
-                                         func=self.session.get,
-                                         **kwargs)
+        resp = self._request_retry(retry=retry,
+                                   func=self.session.get,
+                                   **kwargs)
 
         return resp
```

### Comparing `pan-threat-vault-python-0.2.0/pantv/v1api.py` & `pan-threat-vault-python-0.3.0/pantv/v1aioapi.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,73 +10,81 @@
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 #
 
+import aiohttp
+import asyncio
 import logging
-import requests
 import ssl
 import sys
 import time
 
 from . import (mixin, ApiError, ArgsError,
                DEBUG1, DEBUG2, DEBUG3,
                title, __version__,
                DEFAULT_URL)
 
 
 BASE_PATH = '/service/v1'
 
 
-class ThreatVaultApi(mixin.Mixin):
+class ThreatVaultApi(mixin.AioMixin):
     def __init__(self, *,
                  api_version=None,
                  url=None,
                  api_key=None,
                  verify=None,
                  timeout=None):
+
         self._log = logging.getLogger(__name__).log
         self._log(DEBUG2, '%s: %s, ThreatVaultApi: %s',
                   title, __version__, api_version)
         self._log(DEBUG2, 'Python version: %s', sys.version)
         self._log(DEBUG2, 'ssl: %s', ssl.OPENSSL_VERSION)
-        self._log(DEBUG2, 'requests: %s', requests.__version__)
+        self._log(DEBUG2, 'aiohttp: %s', aiohttp.__version__)
 
         self.api_version = api_version
         if url is None:
             self.url = DEFAULT_URL
         else:
             self.url = url
+        try:
+            self.ssl = self._ssl_context(verify)
+        except ValueError as e:
+            raise ArgsError(e)
+        self._log(DEBUG2, 'ssl: %s %s', self.ssl.verify_mode,
+                  self.ssl.check_hostname)
         auth = self._auth(api_key)
-        self.session = self._session(auth=auth,
-                                     verify=verify,
-                                     timeout=timeout)
-
-    def _request_retry(self, *,
-                       retry=False,
-                       retry_timeout=False,
-                       func=None,
-                       **kwargs):
+        timeout_ = self._timeout(timeout)
+        self._log(DEBUG2, 'timeout: %s', timeout_)
+        self.session = self._session(auth=auth, timeout=timeout_)
+
+    async def _request_retry(self, *,
+                             retry=False,
+                             retry_timeout=False,
+                             func=None,
+                             **kwargs):
         if retry_timeout:
             timeout_delay = 5
             timeout_retries = 3
         while True:
             try:
-                resp = func(**kwargs)
-            except requests.Timeout:
+                resp = await func(**kwargs)
+            except asyncio.TimeoutError:
                 if not (retry_timeout and timeout_retries):
                     raise
                 self._log(DEBUG2, 'timeout, sleep %.2fs', timeout_delay)
-                time.sleep(timeout_delay)
+                await asyncio.sleep(timeout_delay)
                 timeout_delay *= 2
                 timeout_retries -= 1
             else:
-                if retry and resp.status_code == 429:
+                if retry and resp.status == 429:
                     now = time.time()
                     day_remaining = \
                         resp.headers.get('x-day-ratelimit-remaining')
                     if day_remaining is None or day_remaining == '0':
                         break
 
                     minute_reset = \
@@ -89,38 +97,38 @@
                         self._log(DEBUG1, '%s', e)
                         break
 
                     if minute_reset > now:
                         rate_limit_delay = minute_reset - now
                         self._log(DEBUG2, 'status code 429, sleep %.2fs',
                                   rate_limit_delay)
-                        time.sleep(rate_limit_delay)
+                        await asyncio.sleep(rate_limit_delay)
                 else:
                     break
 
         return resp
 
-    def threats(self, *,
-                type=None,
-                id=None,
-                name=None,
-                cve=None,
-                vendor=None,
-                fromReleaseDate=None,
-                toReleaseDate=None,
-                fromReleaseVersion=None,
-                toReleaseVersion=None,
-                releaseDate=None,
-                releaseVersion=None,
-                sha256=None,
-                md5=None,
-                offset=None,
-                limit=None,
-                query_string=None,
-                retry=False):
+    async def threats(self, *,
+                      type=None,
+                      id=None,
+                      name=None,
+                      cve=None,
+                      vendor=None,
+                      fromReleaseDate=None,
+                      toReleaseDate=None,
+                      fromReleaseVersion=None,
+                      toReleaseVersion=None,
+                      releaseDate=None,
+                      releaseVersion=None,
+                      sha256=None,
+                      md5=None,
+                      offset=None,
+                      limit=None,
+                      query_string=None,
+                      retry=False):
         args = locals()
         path = BASE_PATH + '/threats'
         url = self.url + path
 
         params = {}
         for x in args:
             if (x not in ('self', 'query_string', 'retry') and
@@ -128,25 +136,30 @@
                 params[x] = args[x]
 
         if query_string is not None:
             params.update(query_string)
 
         kwargs = {
             'url': url,
+            'ssl': self.ssl,
             'params': params,
         }
 
-        resp = self._request_retry(retry=retry,
-                                   func=self.session.get,
-                                   **kwargs)
+        resp = await self._request_retry(retry=retry,
+                                         func=self.session.get,
+                                         **kwargs)
 
         return resp
 
-    def threats_all(self,
-                    **kwargs):
+    async def _all(self, *,
+                   func,
+                   **kwargs):
+        assert func == self.threats or func == self.edl, \
+            'func not threats() or edl()'
+
         if 'offset' not in kwargs or kwargs['offset'] is None:
             kwargs['offset'] = 0
         else:
             try:
                 kwargs['offset'] = int(kwargs['offset'])
             except ValueError as e:
                 raise ArgsError('offset not int')
@@ -158,58 +171,94 @@
             try:
                 limit = int(kwargs['limit'])
             except ValueError as e:
                 raise ArgsError('limit not int')
 
         total = 0
         while True:
-            resp = self.threats(**kwargs)
-            if resp.status_code == 200:
-                obj = resp.json()
-                try:
-                    threats = [obj['data'][k] for k in obj['data']]
-                    count = obj['count']
-                except KeyError as e:
-                    raise ApiError('Malformed response, missing key %s' % e)
-                current = 0
-                for threat in threats:
-                    current += len(threat)
-                total += current
-                self._log(DEBUG1, 'count %d current %d total %d',
-                          count, current, total)
-                for threat in threats:
-                    for x in threat:
+            resp = await func(**kwargs)
+            if resp.status == 200:
+                obj = await resp.json(content_type=None)
+                if func == self.threats:
+                    try:
+                        threats = [obj['data'][k] for k in obj['data']]
+                        count = obj['count']
+                    except KeyError as e:
+                        raise ApiError('Malformed response, '
+                                       'missing key %s' % e)
+                    current = 0
+                    for threat in threats:
+                        current += len(threat)
+                    total += current
+                    self._log(DEBUG1, 'count %d current %d total %d',
+                              count, current, total)
+                    for threat in threats:
+                        for x in threat:
+                            yield True, x
+
+                elif func == self.edl:
+                    try:
+                        if isinstance(obj['data'], list):
+                            ips = obj['data']
+                        elif (isinstance(obj['data'], dict) and
+                              'ipaddr' in obj['data']):
+                            ips = obj['data']['ipaddr']
+                        else:
+                            raise ApiError('Malformed response, '
+                                           'data not list or dict')
+                        count = obj['count']
+                    except KeyError as e:
+                        raise ApiError('Malformed response, '
+                                       'missing key %s' % e)
+                    current = len(ips)
+                    total += current
+                    self._log(DEBUG1, 'count %d current %d total %d',
+                              count, current, total)
+                    for x in ips:
                         yield True, x
 
                 if total >= count:
                     break
 
                 kwargs['offset'] += limit
             else:
                 yield False, resp
 
-    def threats2(self, *,
-                 type=None,
-                 id=None,
-                 name=None,
-                 sha256=None,
-                 md5=None,
-                 data=None,
-                 query_string=None,
-                 retry=False):
+    async def threats_all(self,
+                          **kwargs):
+        async for ok, x in self._all(func=self.threats,
+                                     **kwargs):
+            yield ok, x
+
+    async def edl_all(self,
+                      **kwargs):
+        async for ok, x in self._all(func=self.edl,
+                                     **kwargs):
+            yield ok, x
+
+    async def threats2(self, *,
+                       type=None,
+                       id=None,
+                       name=None,
+                       sha256=None,
+                       md5=None,
+                       data=None,
+                       query_string=None,
+                       retry=False):
         args = locals()
         path = BASE_PATH + '/threats'
         url = self.url + path
 
         params = {}
         if query_string is not None:
             params.update(query_string)
 
         kwargs = {
             'url': url,
+            'ssl': self.ssl,
             'params': params,
         }
         if data is not None:
             if isinstance(data, (bytes, str, bytearray)):
                 kwargs['data'] = data
                 kwargs['headers'] = {'content-type': 'application/json'}
             else:
@@ -219,28 +268,28 @@
                 if (x not in ('self', 'query_string', 'retry') and
                    args[x] is not None):
                     if 'json' in kwargs:
                         kwargs['json'].update({x: args[x]})
                     else:
                         kwargs['json'] = {x: args[x]}
 
-        resp = self._request_retry(retry=retry,
-                                   func=self.session.post,
-                                   **kwargs)
+        resp = await self._request_retry(retry=retry,
+                                         func=self.session.post,
+                                         **kwargs)
 
         return resp
 
-    def threats_history(self, *,
-                        type=None,
-                        id=None,
-                        order=None,
-                        offset=None,
-                        limit=None,
-                        query_string=None,
-                        retry=False):
+    async def threats_history(self, *,
+                              type=None,
+                              id=None,
+                              order=None,
+                              offset=None,
+                              limit=None,
+                              query_string=None,
+                              retry=False):
         args = locals()
         path = BASE_PATH + '/threats/history'
         url = self.url + path
 
         params = {}
         for x in args:
             if (x not in ('self', 'query_string', 'retry') and
@@ -248,28 +297,29 @@
                 params[x] = args[x]
 
         if query_string is not None:
             params.update(query_string)
 
         kwargs = {
             'url': url,
+            'ssl': self.ssl,
             'params': params,
         }
 
-        resp = self._request_retry(retry=retry,
-                                   func=self.session.get,
-                                   **kwargs)
+        resp = await self._request_retry(retry=retry,
+                                         func=self.session.get,
+                                         **kwargs)
 
         return resp
 
-    def release_notes(self, *,
-                      type=None,
-                      version=None,
-                      query_string=None,
-                      retry=False):
+    async def release_notes(self, *,
+                            type=None,
+                            version=None,
+                            query_string=None,
+                            retry=False):
         args = locals()
         path = BASE_PATH + '/release-notes'
         url = self.url + path
 
         params = {}
         for x in args:
             if (x not in ('self', 'query_string', 'retry') and
@@ -277,72 +327,109 @@
                 params[x] = args[x]
 
         if query_string is not None:
             params.update(query_string)
 
         kwargs = {
             'url': url,
+            'ssl': self.ssl,
             'params': params,
         }
 
-        resp = self._request_retry(retry=retry,
-                                   func=self.session.get,
-                                   **kwargs)
+        resp = await self._request_retry(retry=retry,
+                                         func=self.session.get,
+                                         **kwargs)
 
         return resp
 
-    def atp_reports(self, *,
-                    id=None,
-                    data=None,
-                    query_string=None,
-                    retry=False):
+    async def edl(self, *,
+                  name=None,
+                  ipaddr=None,
+                  version=None,
+                  listformat=None,
+                  offset=None,
+                  limit=None,
+                  query_string=None,
+                  retry=False):
+        args = locals()
+        path = BASE_PATH + '/edl'
+        url = self.url + path
+
+        params = {}
+        for x in args:
+            if (x not in ('self', 'query_string', 'retry') and
+               args[x] is not None):
+                params[x] = args[x]
+
+        if query_string is not None:
+            params.update(query_string)
+
+        kwargs = {
+            'url': url,
+            'ssl': self.ssl,
+            'params': params,
+        }
+
+        resp = await self._request_retry(retry=retry,
+                                         func=self.session.get,
+                                         **kwargs)
+
+        return resp
+
+    async def atp_reports(self, *,
+                          id=None,
+                          query_string=None,
+                          data=None,
+                          retry=False):
         path = BASE_PATH + '/atp/reports'
         url = self.url + path
 
         params = {}
         if query_string is not None:
             params.update(query_string)
 
         kwargs = {
             'url': url,
+            'ssl': self.ssl,
             'params': params,
         }
         if data is not None:
             if isinstance(data, (bytes, str, bytearray)):
                 kwargs['data'] = data
                 kwargs['headers'] = {'content-type': 'application/json'}
             else:
                 kwargs['json'] = data
         else:
             if id is not None:
                 kwargs['json'] = {'id': id}
 
-        resp = self._request_retry(retry=retry,
-                                   func=self.session.post,
-                                   **kwargs)
+        resp = await self._request_retry(retry=retry,
+                                         func=self.session.post,
+                                         **kwargs)
 
         return resp
 
-    def atp_reports_pcaps(self, *,
-                          id=None,
-                          query_string=None,
-                          retry=False):
+    async def atp_reports_pcaps(self, *,
+                                id=None,
+                                query_string=None,
+                                retry=False):
         path = BASE_PATH + '/atp/reports/pcaps'
         url = self.url + path
 
         params = {}
         if id is not None:
             params['id'] = id
 
         if query_string is not None:
             params.update(query_string)
 
         kwargs = {
             'url': url,
+            'ssl': self.ssl,
             'params': params,
         }
 
-        resp = self._request_retry(retry=retry,
-                                   func=self.session.get,
-                                   **kwargs)
+        resp = await self._request_retry(retry=retry,
+                                         func=self.session.get,
+                                         **kwargs)
 
         return resp
```

### Comparing `pan-threat-vault-python-0.2.0/setup.cfg` & `pan-threat-vault-python-0.3.0/setup.cfg`

 * *Files identical despite different names*

