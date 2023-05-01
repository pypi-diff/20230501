# Comparing `tmp/edwh_server_provisioning_plugin-0.2.1.tar.gz` & `tmp/edwh_server_provisioning_plugin-0.3.0.tar.gz`

## Comparing `edwh_server_provisioning_plugin-0.2.1.tar` & `edwh_server_provisioning_plugin-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    23482 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.1/.dcignore
--rw-r--r--   0        0        0    15737 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.1/old_documentation_in_dutch.md
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.1/src/edwh_server_provisioning_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.1/src/edwh_server_provisioning_plugin/__init__.py
--rw-r--r--   0        0        0    45556 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.1/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.1/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.1/readme.md
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    23482 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.0/.dcignore
+-rw-r--r--   0        0        0    16037 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.0/old_documentation_in_dutch.md
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.0/src/edwh_server_provisioning_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.0/src/edwh_server_provisioning_plugin/__init__.py
+-rw-r--r--   0        0        0    46442 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.0/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.0/readme.md
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.3.0/PKG-INFO
```

### Comparing `edwh_server_provisioning_plugin-0.2.1/.dcignore` & `edwh_server_provisioning_plugin-0.3.0/.dcignore`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.2.1/CHANGELOG.md` & `edwh_server_provisioning_plugin-0.3.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.3.0 (2023-05-01)
+### Feature
+* **server_provisioning_plugin.py:** Add `install_generic_service` function to clone a generic-service repository without running `edwh setup` ([`c01f928`](https://github.com/educationwarehouse/server_provisioning/commit/c01f928634deb656dd58260f79ded41882e84749))
+
 ## v0.2.1 (2023-05-01)
 ### Fix
 * **do:** Use connection user instead of os user (for remote fab) ([`9b8de23`](https://github.com/educationwarehouse/server_provisioning/commit/9b8de238069c2f3f21097a608666788e67655b9a))
 
 ## v0.2.0 (2023-05-01)
 ### Feature
 * **do:** Remote.do now supports --edwh flag which works similar to --invoke but for 'edwh' commands ([`6987fa8`](https://github.com/educationwarehouse/server_provisioning/commit/6987fa89741177de6e2046d1782fec860dc7d879))
```

### Comparing `edwh_server_provisioning_plugin-0.2.1/old_documentation_in_dutch.md` & `edwh_server_provisioning_plugin-0.3.0/old_documentation_in_dutch.md`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.2.1/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py` & `edwh_server_provisioning_plugin-0.3.0/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -931,30 +931,54 @@
         "clone_source_url": '"educationwarehouse/repo" of andere toevoeging achter https://github.com/',
         "is_production": "in productie alleen lees rechten op de repo, anders lees en schrijf rechten.",
         "omgeving": "De target directory voor deze omgeving als subfolder in de home van de connectie.",
     }
 )
 def install_omgeving(c, clone_source_url, omgeving, is_production=False, branch=None):
     """
-    Clone een git repository naar de directory `omgeving` in de homefolder, en voer `invoke setup` daar uit.
+    Clone een git repository naar de directory `omgeving` in de homefolder, en voer `edwh setup` daar uit.
     """
     clone_git_repo_with_new_key_file_for_edwh_repos(
         c,
         clone_source_url,
         "r" if is_production else "rw",
         target_directory=omgeving,
         branch=branch,
     )
-    do(c, omgeving=[omgeving], invoke="setup")
+    do(c, omgeving=[omgeving], edwh="setup")
+
+
+@task(
+    help={
+        "clone_source_url": '"educationwarehouse/generic-service" of andere toevoeging achter https://github.com/',
+        "is_production": "in productie alleen lees rechten op de repo, anders lees en schrijf rechten.",
+        "omgeving": "De target directory voor deze omgeving als subfolder in de home van de connectie.",
+    }
+)
+def install_generic_service(
+        c, omgeving, clone_source_url="educationwarehouse/generic-service", is_production=False, branch=None
+):
+    """
+    Lijkt op install_omgeving maar dan voor een generic-service (die nog niet af is), dus zonder `edwh setup`
+    """
+    clone_git_repo_with_new_key_file_for_edwh_repos(
+        c,
+        clone_source_url,
+        "r" if is_production else "rw",
+        target_directory=omgeving,
+        branch=branch,
+    )
+
+    # NO ew setup, since this service is (probably) not functional yet.
 
 
 @task
 def prepare_ontwikkelstraat_server(c, is_production=False):
     prepare_generic_server(c)
-    install_ontwikkelstraat(c)
+    # install_ontwikkelstraat(c)
     if is_production:
         subscription_key = input(
             "WithSecure linux server Subscription Key (https://elements.f-secure.com/apps/psb/c556915/subscription) [blank=ignore]: "
         )
         if subscription_key.strip():
             install_antivirus(c, subscription_key=subscription_key)
             print("/!\ Denk eraan, hier moet nog een profiel aan gekoppeld worden in de withsecure website! ")
```

### Comparing `edwh_server_provisioning_plugin-0.2.1/LICENSE.txt` & `edwh_server_provisioning_plugin-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.2.1/pyproject.toml` & `edwh_server_provisioning_plugin-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.2.1/readme.md` & `edwh_server_provisioning_plugin-0.3.0/readme.md`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.2.1/PKG-INFO` & `edwh_server_provisioning_plugin-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-server-provisioning-plugin
-Version: 0.2.1
+Version: 0.3.0
 Summary: Fabric-based remote server management plugin for `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/server_provisioning#readme
 Project-URL: Issues, https://github.com/educationwarehouse/server_provisioning/issues
 Project-URL: Source, https://github.com/educationwarehouse/server_provisioning
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

