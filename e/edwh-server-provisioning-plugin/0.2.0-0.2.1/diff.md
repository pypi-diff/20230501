# Comparing `tmp/edwh_server_provisioning_plugin-0.2.0.tar.gz` & `tmp/edwh_server_provisioning_plugin-0.2.1.tar.gz`

## Comparing `edwh_server_provisioning_plugin-0.2.0.tar` & `edwh_server_provisioning_plugin-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    23482 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.0/.dcignore
--rw-r--r--   0        0        0    15518 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.0/old_documentation_in_dutch.md
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.0/src/edwh_server_provisioning_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.0/src/edwh_server_provisioning_plugin/__init__.py
--rw-r--r--   0        0        0    45511 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.0/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.0/readme.md
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    23482 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.1/.dcignore
+-rw-r--r--   0        0        0    15737 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.1/old_documentation_in_dutch.md
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.1/src/edwh_server_provisioning_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.1/src/edwh_server_provisioning_plugin/__init__.py
+-rw-r--r--   0        0        0    45556 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.1/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.1/readme.md
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.1/PKG-INFO
```

### Comparing `edwh_server_provisioning_plugin-0.2.0/.dcignore` & `edwh_server_provisioning_plugin-0.2.1/.dcignore`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.2.0/CHANGELOG.md` & `edwh_server_provisioning_plugin-0.2.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.2.1 (2023-05-01)
+### Fix
+* **do:** Use connection user instead of os user (for remote fab) ([`9b8de23`](https://github.com/educationwarehouse/server_provisioning/commit/9b8de238069c2f3f21097a608666788e67655b9a))
+
 ## v0.2.0 (2023-05-01)
 ### Feature
 * **do:** Remote.do now supports --edwh flag which works similar to --invoke but for 'edwh' commands ([`6987fa8`](https://github.com/educationwarehouse/server_provisioning/commit/6987fa89741177de6e2046d1782fec860dc7d879))
 * **postgres:** Connect-postgres now accepts --omgeving to select a directory to read postgres port from dc ([`4b2fcda`](https://github.com/educationwarehouse/server_provisioning/commit/4b2fcda3eaee7a2e9d4610a744c115a7633fcf45))
 * Added auto edwh install when prepare_generic_server is called ([`f2e41df`](https://github.com/educationwarehouse/server_provisioning/commit/f2e41df419213924fd53e493fc8514d8dc78ea16))
 
 ### Fix
```

### Comparing `edwh_server_provisioning_plugin-0.2.0/old_documentation_in_dutch.md` & `edwh_server_provisioning_plugin-0.2.1/old_documentation_in_dutch.md`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.2.0/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py` & `edwh_server_provisioning_plugin-0.2.1/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,17 +137,17 @@
         if count_keys == len(command_line_key):
             for which_key in command_line_key:
                 for head_keys in all_key_information:
                     if which_key in head_keys:
                         for key, value in all_key_information[head_keys].items():
                             # gaat alleen de 'sleutel' toevoegen en niet de datetime enzovoort
                             if (
-                                bool(key.find('datetime'))
-                                and bool(key.find('wie@hostname'))
-                                and bool(key.find('message')) is True
+                                    bool(key.find('datetime'))
+                                    and bool(key.find('wie@hostname'))
+                                    and bool(key.find('message')) is True
                             ):
                                 c.run(f'echo {value} >> ~/.ssh/authorized_keys')
                                 c.run('touch ~/.ssh/keys')
                                 c.run('sort -u ~/.ssh/authorized_keys > ~/.ssh/keys')
                                 time.sleep(1)
                                 c.run('cp ~/.ssh/keys ~/.ssh/authorized_keys')
                                 c.run('rm ~/.ssh/keys')
@@ -204,17 +204,17 @@
         all_key_information = key_db.setdefault('sleutels')
     for which_key in command_line_key:
         for head_keys in all_key_information:
             if which_key in head_keys:
                 for key, value in all_key_information[head_keys].items():
                     # gaat alleen de 'sleutel' toevoegen en niet de datetime enzovoort
                     if (
-                        bool(key.find('datetime'))
-                        and bool(key.find('wie@hostname'))
-                        and bool(key.find('message')) is True
+                            bool(key.find('datetime'))
+                            and bool(key.find('wie@hostname'))
+                            and bool(key.find('message')) is True
                     ):
                         # pakt de juiste sleutel en 'verwijdert' die sleutel
                         c.run(f'grep -v "{value}" ~/.ssh/authorized_keys > ~/.ssh/keys')
                         c.run('mv ~/.ssh/keys ~/.ssh/authorized_keys')
                         print(f'Het is gelukt! De \033[1m{which_key}\033[0m key is verwijderd.')
 
 
@@ -558,17 +558,17 @@
 @task
 def set_noninteractive(c):
     c.run("export DEBIAN_FRONTEND=noninteractive")
 
 
 @task
 def prepare_git_client(
-    c,
-    username,
-    email,
+        c,
+        username,
+        email,
 ):
     c: Connection = c
     print(c.host)
     return
     # git config --global --add user.name spore
     c.run(f"git config --global --add user.name {username}")
     # git config --global --add user.email spore@edwh.nl
@@ -623,20 +623,20 @@
             c.put(io.StringIO(config), ".ssh/config")
 
         # respond_to_security=Responder(r'Are you sure you want to continue connecting \(yes/no/\[fingerprint\]\)\?.*','yes\n')
 
         # check als machine correcte git ssh verbinding kan maken
         # fingerprint
         if (
-            "Permission denied (publickey)"
-            in c.run(
-                "ssh-key -R github.com && ssh -tt -o StrictHostKeyChecking=accept-new git@github.com",
-                hide=True,
-                warn=True,
-            ).stderr
+                "Permission denied (publickey)"
+                in c.run(
+            "ssh-key -R github.com && ssh -tt -o StrictHostKeyChecking=accept-new git@github.com",
+            hide=True,
+            warn=True,
+        ).stderr
         ):
             raise Exception(
                 "github key klopt niet, CHECK ALS GITHUB_KNOWN_HOSTS KEY KLOPT IN DE server_provisioning_plugin.py"
             )
 
         # test if the repo exists:
         if "fatal:" in c.run(f"cd {target_directory or git_repo}; git status", warn=True, hide=True).stderr:
@@ -791,15 +791,15 @@
 def install_edwh(c):
     if execution_fails(c, c.run("pipx install edwh[omgeving,plugins]")):
         c.run("pipx upgrade edwh")
 
 
 @task()
 def prepare_generic_server(
-    c,
+        c,
 ):
     """Updates apt and dist-upgrades the machine. Installs python, docker, docker-compose, and xonsh.
 
     A default .xonshrc is added, as well as a microservices group and the current user is added to both
     the docker group as well as the microservices group.
     """
     set_noninteractive(c)
@@ -898,15 +898,15 @@
 
     cmd kan ook gebruikt worden voor troubleshooting/scripting.
     bijvoorbeeld:
 
       fab -H utils do --omgeving taiga --invoke "restart --quick" -e
 
     """
-    current_user = os.getlogin()
+    current_user = c.user
     bin_path = f"/home/{current_user}/.local/bin"
 
     if not omgeving:
         omgeving = ["."]
 
     if at_least([cmd, invoke, edwh], 2):
         print("Gebruik slechts --invoke of --cmd, niet beide")
@@ -1136,19 +1136,19 @@
           - "traefik.http.middlewares.{service}-compress.compress=true"
     
     """
     )
     print("------- [new] ---------------------------------------------------- ")
     print(compose_fragment)
     if yes or input(f"append to {docker_compose_path}/docker-compose.yaml? [NO,yes] #").lower().strip() in (
-        "y",
-        "yes",
-        "j",
-        "ja",
-        "1",
+            "y",
+            "yes",
+            "j",
+            "ja",
+            "1",
     ):
         print("Copying compose file to docker-compose.bak")
         c.run(
             f"cp {docker_compose_path}/docker-compose.yaml {docker_compose_path}/docker-compose.bak",
             hide=True,
         )
         # craft the directory if it doesn't exist already
```

### Comparing `edwh_server_provisioning_plugin-0.2.0/LICENSE.txt` & `edwh_server_provisioning_plugin-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.2.0/pyproject.toml` & `edwh_server_provisioning_plugin-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.2.0/readme.md` & `edwh_server_provisioning_plugin-0.2.1/readme.md`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.2.0/PKG-INFO` & `edwh_server_provisioning_plugin-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-server-provisioning-plugin
-Version: 0.2.0
+Version: 0.2.1
 Summary: Fabric-based remote server management plugin for `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/server_provisioning#readme
 Project-URL: Issues, https://github.com/educationwarehouse/server_provisioning/issues
 Project-URL: Source, https://github.com/educationwarehouse/server_provisioning
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

