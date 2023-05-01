# Comparing `tmp/optumi-core-3.15.4.tar.gz` & `tmp/optumi-core-3.15.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optumi-core-3.15.4.tar", last modified: Wed Apr 12 20:24:30 2023, max compression
+gzip compressed data, was "optumi-core-3.15.5.tar", last modified: Fri Apr 28 23:43:23 2023, max compression
```

## Comparing `optumi-core-3.15.4.tar` & `optumi-core-3.15.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-04-12 20:24:30.680214 optumi-core-3.15.4/
--rw-rw-r--   0 denis     (1001) denis     (1001)      280 2023-04-03 21:07:54.000000 optumi-core-3.15.4/LICENSE
--rw-rw-r--   0 denis     (1001) denis     (1001)       34 2023-04-03 21:07:54.000000 optumi-core-3.15.4/MANIFEST.in
--rw-rw-r--   0 denis     (1001) denis     (1001)     1562 2023-04-12 20:24:30.676214 optumi-core-3.15.4/PKG-INFO
--rw-rw-r--   0 denis     (1001) denis     (1001)      422 2023-04-03 21:07:54.000000 optumi-core-3.15.4/README.md
-drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-04-12 20:24:30.676214 optumi-core-3.15.4/optumi_core/
--rw-rw-r--   0 denis     (1001) denis     (1001)      408 2023-04-03 21:07:54.000000 optumi-core-3.15.4/optumi_core/__init__.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      322 2023-04-07 16:00:16.000000 optumi-core-3.15.4/optumi_core/_version.py
--rw-rw-r--   0 denis     (1001) denis     (1001)    39799 2023-04-03 21:07:54.000000 optumi-core-3.15.4/optumi_core/core.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1520 2023-04-03 21:07:54.000000 optumi-core-3.15.4/optumi_core/exceptions.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1043 2023-04-03 21:07:54.000000 optumi-core-3.15.4/optumi_core/logging.py
--rw-rw-r--   0 denis     (1001) denis     (1001)    14139 2023-04-04 21:44:37.000000 optumi-core-3.15.4/optumi_core/login.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     3407 2023-04-03 21:07:54.000000 optumi-core-3.15.4/optumi_core/sessions.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     2359 2023-04-03 21:07:54.000000 optumi-core-3.15.4/optumi_core/utils.py
-drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-04-12 20:24:30.676214 optumi-core-3.15.4/optumi_core.egg-info/
--rw-rw-r--   0 denis     (1001) denis     (1001)     1562 2023-04-12 20:24:30.000000 optumi-core-3.15.4/optumi_core.egg-info/PKG-INFO
--rw-rw-r--   0 denis     (1001) denis     (1001)      429 2023-04-12 20:24:30.000000 optumi-core-3.15.4/optumi_core.egg-info/SOURCES.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-04-12 20:24:30.000000 optumi-core-3.15.4/optumi_core.egg-info/dependency_links.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-04-12 20:24:30.000000 optumi-core-3.15.4/optumi_core.egg-info/not-zip-safe
--rw-rw-r--   0 denis     (1001) denis     (1001)       25 2023-04-12 20:24:30.000000 optumi-core-3.15.4/optumi_core.egg-info/requires.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)       12 2023-04-12 20:24:30.000000 optumi-core-3.15.4/optumi_core.egg-info/top_level.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)       38 2023-04-12 20:24:30.680214 optumi-core-3.15.4/setup.cfg
--rwxrwxr-x   0 denis     (1001) denis     (1001)     1932 2023-04-03 21:07:54.000000 optumi-core-3.15.4/setup.py
+drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-04-28 23:43:23.853155 optumi-core-3.15.5/
+-rw-rw-r--   0 denis     (1001) denis     (1001)      280 2023-04-27 13:56:16.000000 optumi-core-3.15.5/LICENSE
+-rw-rw-r--   0 denis     (1001) denis     (1001)       34 2023-04-27 13:56:16.000000 optumi-core-3.15.5/MANIFEST.in
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1562 2023-04-28 23:43:23.849156 optumi-core-3.15.5/PKG-INFO
+-rw-rw-r--   0 denis     (1001) denis     (1001)      422 2023-04-27 13:56:16.000000 optumi-core-3.15.5/README.md
+drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-04-28 23:43:23.849156 optumi-core-3.15.5/optumi_core/
+-rw-rw-r--   0 denis     (1001) denis     (1001)      408 2023-04-27 13:56:16.000000 optumi-core-3.15.5/optumi_core/__init__.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      322 2023-04-27 18:15:41.000000 optumi-core-3.15.5/optumi_core/_version.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)    39877 2023-04-27 18:15:41.000000 optumi-core-3.15.5/optumi_core/core.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1566 2023-04-27 18:15:41.000000 optumi-core-3.15.5/optumi_core/exceptions.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1043 2023-04-27 13:56:16.000000 optumi-core-3.15.5/optumi_core/logging.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)    13268 2023-04-27 18:15:41.000000 optumi-core-3.15.5/optumi_core/login.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3568 2023-04-28 13:25:45.000000 optumi-core-3.15.5/optumi_core/sessions.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     2359 2023-04-27 13:56:16.000000 optumi-core-3.15.5/optumi_core/utils.py
+drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-04-28 23:43:23.849156 optumi-core-3.15.5/optumi_core.egg-info/
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1562 2023-04-28 23:43:23.000000 optumi-core-3.15.5/optumi_core.egg-info/PKG-INFO
+-rw-rw-r--   0 denis     (1001) denis     (1001)      429 2023-04-28 23:43:23.000000 optumi-core-3.15.5/optumi_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-04-28 23:43:23.000000 optumi-core-3.15.5/optumi_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-04-28 23:43:23.000000 optumi-core-3.15.5/optumi_core.egg-info/not-zip-safe
+-rw-rw-r--   0 denis     (1001) denis     (1001)       25 2023-04-28 23:43:23.000000 optumi-core-3.15.5/optumi_core.egg-info/requires.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)       12 2023-04-28 23:43:23.000000 optumi-core-3.15.5/optumi_core.egg-info/top_level.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)       38 2023-04-28 23:43:23.853155 optumi-core-3.15.5/setup.cfg
+-rwxrwxr-x   0 denis     (1001) denis     (1001)     1932 2023-04-27 13:56:16.000000 optumi-core-3.15.5/setup.py
```

### Comparing `optumi-core-3.15.4/PKG-INFO` & `optumi-core-3.15.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optumi-core
-Version: 3.15.4
+Version: 3.15.5
 Summary: Optumi core library
 Home-page: https://optumi.com
 Author: Optumi Inc Authors
 Author-email: cs@optumi.com
 Keywords: Optumi
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `optumi-core-3.15.4/optumi_core/core.py` & `optumi-core-3.15.5/optumi_core/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,15 +318,15 @@
 
 # Leave module parameter for compatibility
 def stop_notebook(workload, module=None):
     URL = "/exp/jupyterlab/stop-notebook"
     try:
         try:
             lock.acquire()
-            launchStatus[uuid]["status"] = "Failed"
+            launchStatus[workload]["status"] = "Failed"
         except:
             pass
         finally:
             lock.release()
 
         return get_session().post(
             URL,
@@ -341,15 +341,15 @@
 
 # Leave module parameter for compatibility
 def teardown_notebook(workload, module=None):
     URL = "/exp/jupyterlab/teardown-notebook"
     try:
         try:
             lock.acquire()
-            launchStatus[uuid]["status"] = "Failed"
+            launchStatus[workload]["status"] = "Failed"
         except:
             pass
         finally:
             lock.release()
 
         return get_session().post(
             URL,
@@ -630,38 +630,39 @@
                     compressionProgress[key] = {"progress": -1, "total": 0}
                 uploadProgress[key] = {"progress": -1, "total": 0}
             except Exception as e:
                 pass
             finally:
                 lock.release()
     except OperationCanceled as e:
-        cleanup_progress(e, compress)
+        cleanup_progress(key, compress)
         if e.pathToRemove and os.path.exists(e.pathToRemove):
             os.remove(e.pathToRemove)
         return e
     except HTTPError as e:
-        cleanup_progress(e, compress)
+        cleanup_progress(key, compress)
         return e
 
 
-def cleanup_progress(e, compress):
+def cleanup_progress(key, compress):
     # Clean up ongoing progress in the case of a failure
-    try:
-        lock.acquire()
-        if compress:
-            # Cancel compression progress
-            if key in compressionProgress:
-                compressionProgress[key] = {"progress": -1, "total": 0}
-        # Cancel upload progress
-        if key in uploadProgress:
-            uploadProgress[key] = {"progress": -1, "total": 0}
-    except Exception:
-        pass
-    finally:
-        lock.release()
+    if key:
+        try:
+            lock.acquire()
+            if compress:
+                # Cancel compression progress
+                if key in compressionProgress:
+                    compressionProgress[key] = {"progress": -1, "total": 0}
+            # Cancel upload progress
+            if key in uploadProgress:
+                uploadProgress[key] = {"progress": -1, "total": 0}
+        except Exception:
+            pass
+        finally:
+            lock.release()
 
 
 def check_if_files_exist(paths):
     URL = "/exp/jupyterlab/check-if-files-exist"
     try:
         stats = [os.stat(f) if os.path.isfile(f) else None for f in paths]
         creationTimes = [datetime.datetime.utcfromtimestamp(stat.st_ctime).isoformat() + "Z" if stat != None else None for stat in stats]
```

### Comparing `optumi-core-3.15.4/optumi_core/exceptions.py` & `optumi-core-3.15.5/optumi_core/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 
 class ServiceException(OptumiException):
     def __init__(self, message: str = None):
         super().__init__(message if message else "Unable to contact Optumi services, please try again later")
 
 
 class NotLoggedInException(OptumiException):
-    def __init__(self, message: str = None):
+    def __init__(self, message: str = None, err: Exception = None):
         super().__init__(message if message else "Please use login() to access Optumi services")
+        self.err = err
 
 
 class OperationCanceled(OptumiException):
     def __init__(self, message: str, pathToRemove: str = None):
         super().__init__(message)
         self.pathToRemove = pathToRemove
```

### Comparing `optumi-core-3.15.4/optumi_core/logging.py` & `optumi-core-3.15.5/optumi_core/logging.py`

 * *Files identical despite different names*

### Comparing `optumi-core-3.15.4/optumi_core/login.py` & `optumi-core-3.15.5/optumi_core/login.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 ## To receive a copy of the licensing terms please write to contact@optumi.com or visit us at http://www.optumi.com.
 ##
 
 from ._version import __version__
 from .logging import optumi_format_and_log
 from .sessions import get_session, get_mode
 from .exceptions import NotLoggedInException, VersionIncompatibility
-from .utils import dev_version, get_portal_domain_and_port, get_portal_port
+from .utils import dev_version, get_portal_domain_and_port, get_portal, get_portal_port
+
 
 ## Standard library imports
 
 # Generic Operating System Services
 import time, os
 from pathlib import Path
 from datetime import datetime
@@ -24,17 +25,16 @@
 
 # Concurrent execution
 from threading import Lock
 
 # Internet Protocols and Support
 from http.cookiejar import DefaultCookiePolicy, CookieJar
 import requests
-from requests.exceptions import HTTPError
-from urllib.error import URLError
-from urllib.parse import urlparse, parse_qs
+from requests.exceptions import HTTPError, ConnectionError, Timeout
+from urllib.parse import urlparse
 
 # Internet Data Handling
 import json, base64
 
 # Networking and Interprocess Communication
 import socket, ssl
 
@@ -158,120 +158,107 @@
 
 
 def check_login(login_domain, login_port):
     session = get_session()
     try:
         response = get_redirect()
         if response.url.endswith("/login"):
-            session._domain_and_port = get_portal_domain_and_port()
+            session._domain_and_port = [get_portal_domain_and_port()]
             return False
         redirect = json.loads(response.text)
         if redirect == {}:
             # We have no assigned controller for a local station and therefore no redirect
             return True
         elif "dnsName" in redirect and "port" in redirect:
-            session._domain_and_port = redirect["dnsName"] + ":" + str(redirect["port"])
+            domain_and_port = redirect["dnsName"] + ":" + str(redirect["port"])
+            if session._domain_and_port[-1] != domain_and_port:
+                session._domain_and_port.append(domain_and_port)
             if redirect["dnsName"] == login_domain and redirect["port"] == login_port:
                 return True
             else:
                 return check_login(redirect["dnsName"], redirect["port"])
-        session._domain_and_port = get_portal_domain_and_port()
+        session._domain_and_port = [get_portal_domain_and_port()]
         return False
     except (HTTPError, NotLoggedInException) as e:
-        session._domain_and_port = get_portal_domain_and_port()
+        session._domain_and_port = [get_portal_domain_and_port()]
         return False
 
 
 def login_rest_server(
     login_domain,
     login_port,
     token=None,
     login_type="oauth",
     save_token=False,
 ):
     session = get_session()
     try:
         if check_login(login_domain, login_port):
-            return 1, get_session()._domain_and_port
+            return 1, get_session()._domain_and_port[-1]
 
         start_time = None
         last_domain_and_port = None
         while True:
             if start_time == None:
                 start_time = time.time()
             elif time.time() - start_time > 600:  # 10 minute timeout
-                session._domain_and_port = get_portal_domain_and_port()
+                session._domain_and_port = [get_portal_domain_and_port()]
                 return -1, "Timed out"
             # If we want to move back to using a devserver certificate we need to check for devserver.optumi.com explicitly
             # Since we are bypassing the hostname check for the SSL context, we manually check it here
             # cert = ssl.get_server_certificate((DOMAIN, 8443))
             # cert = x509.load_pem_x509_certificate(cert.encode(), default_backend())
             # name = cert.subject.get_attributes_for_oid(x509.oid.NameOID.COMMON_NAME)[0].value
             # if name != 'devserver.optumi.com':
             #     raise ssl.SSLCertVerificationError("SSL domain check failed (" + name + " is not devserver.optumi.com)")
 
-            session._domain_and_port = login_domain + ":" + str(login_port)
+            domain_and_port = login_domain + ":" + str(login_port)
+            if session._domain_and_port[-1] != domain_and_port:
+                session._domain_and_port.append(domain_and_port)
 
             URL = "/login"
             errorURL = URL + "?error"
 
             # We only want to print to the log when we try to contact somewhere new
-            if session._domain_and_port != last_domain_and_port:
+            if session._domain_and_port[-1] != last_domain_and_port:
                 if dev_version:
                     print(optumi_format_and_log(None, "Contacting " + URL))
                 else:
                     optumi_format_and_log(None, "Contacting " + URL)
 
             # since it can take a long time to log in to actually log in to the station, set a longer timeout for that request
             timeout = (
                 30
-                if session._domain_and_port == get_portal_domain_and_port() or session._domain_and_port == "portal.optumi.net:" + str(get_portal_port())
+                if session._domain_and_port[-1] == get_portal_domain_and_port() or session._domain_and_port[-1] == "portal.optumi.net:" + str(get_portal_port())
                 else 120
             )
 
             if login_type == "token" and token is None:
                 # Try to load the token from the disk
                 TOKEN_FILE = get_token_file()
 
                 if os.path.exists(TOKEN_FILE):
                     with open(TOKEN_FILE, "r") as f:
                         token = f.read()
                 else:
-                    session._domain_and_port = get_portal_domain_and_port()
+                    session._domain_and_port = [get_portal_domain_and_port()]
                     return -1, "No login token"
 
             try:
                 response = session.post(
                     URL,
                     data={"login_type": login_type, "username": "", "password": token},
                     timeout=timeout,
                 )
-            except URLError as err:
-                if isinstance(err.reason, socket.timeout):
-                    return -1, "Timed out"
-                if isinstance(err.reason, socket.gaierror):
-                    if session._domain_and_port == get_portal_domain_and_port() or session._domain_and_port == "portal.optumi.net:" + str(get_portal_port()):
-                        # If we failed trying to access portalAB.optumi.net or portal.optumi.net, redirect to the top level portal.optumi.net
-                        login_domain = "portal.optumi.net"
-                        login_port = PORTAL_PORT
-                        last_domain_and_port = session._domain_and_port
-                        continue
-                    else:
-                        # If we were trying to access a station, redirect to portalAB.optumi.net
-                        login_domain = PORTAL
-                        login_port = PORTAL_PORT
-                        last_domain_and_port = session._domain_and_port
-                        continue
-                if isinstance(err.reason, ConnectionRefusedError):
-                    time.sleep(2)
-                    login_domain = login_domain
-                    login_port = login_port
-                    last_domain_and_port = session._domain_and_port
-                    continue
-                raise err
+            except Timeout as err:
+                return -1, "Timed out"
+            except ConnectionError as err:
+                time.sleep(2)
+                last_domain_and_port = session._domain_and_port[-1]
+                continue
 
             parsed = urlparse(response.url)
 
             redirect = None
             try:
                 redirect = json.loads(response.text)
             except:
@@ -279,35 +266,35 @@
 
             if redirect != None:
                 if redirect["dnsName"] == "unknown":
                     set_login_progress("Allocating...")
                     time.sleep(2)
                     login_domain = login_domain
                     login_port = login_port
-                    last_domain_and_port = session._domain_and_port
+                    last_domain_and_port = session._domain_and_port[-1]
                     continue
                 elif redirect["dnsName"] == "no more stations" or redirect["dnsName"] == "no more trial stations":
-                    session._domain_and_port = get_portal_domain_and_port()
+                    session._domain_and_port = [get_portal_domain_and_port()]
                     return -1, redirect["dnsName"]
                 else:
                     set_login_progress("Restoring context...")
                     login_domain = redirect["dnsName"]
                     login_port = redirect["port"]
-                    last_domain_and_port = session._domain_and_port
+                    last_domain_and_port = session._domain_and_port[-1]
                     continue
 
             if parsed.path == "/login" and parsed.query == "error":
                 # Parse the error message to pass on to the user
                 raw_html = response.text
                 try:
                     message = raw_html.split('<div class="alert alert-danger" role="alert">')[1].split("</div>")[0]
                 except:
                     message = "Invalid username/password"
 
-                session._domain_and_port = get_portal_domain_and_port()
+                session._domain_and_port = [get_portal_domain_and_port()]
                 return -1, message
 
             ## This is currently necessary in order for the controller to recognize that the user has signed the agreement
             get_new_agreement()
 
             # make sure we have a compatible version
             try:
@@ -355,34 +342,33 @@
                     print("Saving connection token to", TOKEN_FILE)
                     with open(TOKEN_FILE, "w+") as f:
                         f.write(token)
 
                     os.chmod(TOKEN_FILE, 0o600)
 
             # On success return the status value 1 and the domain that we logged in to
-            return 1, session._domain_and_port
+            return 1, session._domain_and_port[-1]
     except Exception as err:
         print(optumi_format_and_log(None, str(err)))
         traceback.print_exc()
-        session._domain_and_port = get_portal_domain_and_port()
+        session._domain_and_port = [get_portal_domain_and_port()]
         return -3, ""
 
 
 def logout(remove_token=True):
-    URL = "/logout"
     try:
         if remove_token:
             TOKEN_FILE = get_token_file()
             try:
                 os.remove(TOKEN_FILE)
                 print("Removed connection token")
             except OSError:
                 pass
         # Silently remove cookies
         COOKIE_FILE = get_cookie_file()
         try:
             os.remove(COOKIE_FILE)
         except OSError:
             pass
-        return get_session().get(URL, timeout=120)
+        get_session().logout()
     except HTTPError as e:
         return e
```

### Comparing `optumi-core-3.15.4/optumi_core/sessions.py` & `optumi-core-3.15.5/optumi_core/sessions.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,63 +4,64 @@
 ## You may only use this code under license with Optumi Inc and any distribution or modification is strictly prohibited.
 ## To receive a copy of the licensing terms please write to contact@optumi.com or visit us at http://www.optumi.com.
 ##
 
 from ._version import __version__
 
 from requests import Session
-from requests.exceptions import ConnectionError
 from .exceptions import NotLoggedInException, OptumiException, NoAgreementException, VersionIncompatibility
-from .utils import dev_version, get_portal_domain_and_port, get_portal, get_portal_port
+from .utils import dev_version, get_portal_domain_and_port, get_portal, get_portal_port, is_dynamic
 
 import psutil, os
 
 sessions = {}
 
 
 class CustomSession(Session):
     def __init__(self):
         super().__init__()
-        self._domain_and_port = get_portal_domain_and_port()
-
-    def get_path(self):
-        return "https://" + self._domain_and_port
+        self._domain_and_port = [get_portal_domain_and_port()]
 
     def attempt_silent_login(self):
         from .login import login_rest_server
 
-        login_status, message = login_rest_server(get_portal(), get_portal_port(), login_type="token", save_token=True)
+        if is_dynamic():
+            login_status, message = login_rest_server(get_portal(), get_portal_port(), "", login_type="dynamic", save_token=True)
+        else:
+            login_status, message = login_rest_server(get_portal(), get_portal_port(), login_type="token", save_token=True)
         return login_status == 1
 
-    def _make_request(self, method, url, **kwargs):
-        try:
-            response = super().request(method, self.get_path() + url, **kwargs)
-            if (not url.endswith("/login")) and response.url.endswith("/login"):
-                raise NotLoggedInException()
-            if response.status_code >= 400:
-                text = response.text
-                if text == "User has not signed the Terms & Conditions of Service":
-                    raise NoAgreementException()
-                if "exchange-versions" in url:
-                    raise VersionIncompatibility(text)
-                raise OptumiException(text if (text != None and len(text) > 0) else None)
-            return response
-        except ConnectionError as err:
-            if self._domain_and_port == get_portal_domain_and_port():
-                raise
-        raise NotLoggedInException()
+    def _make_request(self, method, domain_and_port, url, **kwargs):
+        response = super().request(method, "https://" + domain_and_port + url, **kwargs)
+        if (not url.endswith("/login")) and response.url.endswith("/login"):
+            raise NotLoggedInException()
+        if response.status_code >= 400:
+            text = response.text
+            if text == "User has not signed the Terms & Conditions of Service":
+                raise NoAgreementException()
+            if "exchange-versions" in url:
+                raise VersionIncompatibility(text)
+            raise OptumiException(text if (text != None and len(text) > 0) else None)
+        return response
 
     def request(self, method, url, **kwargs):
         try:
-            return self._make_request(method, url, **(kwargs["get_kwargs"]() if "get_kwargs" in kwargs else kwargs))
+            return self._make_request(method, self._domain_and_port[-1], url, **(kwargs["get_kwargs"]() if "get_kwargs" in kwargs else kwargs))
         except NotLoggedInException:
             if not ("get-redirect" in url or "exchange-versions" in url or "login" in url or "logout" in url) and self.attempt_silent_login():
-                return self._make_request(method, url, **(kwargs["get_kwargs"]() if "get_kwargs" in kwargs else kwargs))
+                return self._make_request(method, self._domain_and_port[-1], url, **(kwargs["get_kwargs"]() if "get_kwargs" in kwargs else kwargs))
             raise
 
+    def logout(self):
+        for domain_and_port in self._domain_and_port:
+            try:
+                self._make_request("GET", domain_and_port, "/logout", timeout=30)
+            except NotLoggedInException:
+                pass
+
 
 def get_mode():
     import traceback
 
     for frame in reversed(traceback.extract_stack()):
         parts = frame.filename.split("/")
         if "optumi_api" in parts:
```

### Comparing `optumi-core-3.15.4/optumi_core/utils.py` & `optumi-core-3.15.5/optumi_core/utils.py`

 * *Files identical despite different names*

### Comparing `optumi-core-3.15.4/optumi_core.egg-info/PKG-INFO` & `optumi-core-3.15.5/optumi_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optumi-core
-Version: 3.15.4
+Version: 3.15.5
 Summary: Optumi core library
 Home-page: https://optumi.com
 Author: Optumi Inc Authors
 Author-email: cs@optumi.com
 Keywords: Optumi
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `optumi-core-3.15.4/setup.py` & `optumi-core-3.15.5/setup.py`

 * *Files identical despite different names*

