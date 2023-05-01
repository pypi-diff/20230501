# Comparing `tmp/edwh_multipass_plugin-1.0.0.tar.gz` & `tmp/edwh_multipass_plugin-1.0.1.tar.gz`

## Comparing `edwh_multipass_plugin-1.0.0.tar` & `edwh_multipass_plugin-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.0/src/edwh_multipass_plugin/__about__.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.0/src/edwh_multipass_plugin/__init__.py
--rw-r--r--   0        0        0     6932 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.0/src/edwh_multipass_plugin/tasks.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.0/.gitignore
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.0/README.md
--rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.1/src/edwh_multipass_plugin/__about__.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.1/src/edwh_multipass_plugin/__init__.py
+-rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.1/src/edwh_multipass_plugin/tasks.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.1/README.md
+-rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 edwh_multipass_plugin-1.0.1/PKG-INFO
```

### Comparing `edwh_multipass_plugin-1.0.0/src/edwh_multipass_plugin/tasks.py` & `edwh_multipass_plugin-1.0.1/src/edwh_multipass_plugin/tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import json, pathlib
+import json
+import pathlib
 import re
 import sys
 
 import invoke
-from invoke import task, Collection, Task
+from invoke import task
 
 
 @task(name="install")
 def install_multipass(c):
     if not c.run("multipass --version", warn=True, hide=True).ok:
         print(" [ ] Multipass not found. installing...")
         c.sudo("snap install multipass")
@@ -31,16 +32,16 @@
         # wat het script is dat dit uitvoert. Dus met `which invoke` vinden
         # we het volledige pad naar invoke, en van daaruit hebben we vermoedelijk
         # de juiste pip te pakken. Of het nou een virtualenv van de gebruiker is, van pipx
         # of geinstalleerd met --user of zelfs `pip install invoke` als root...
         print("Missing pip, installing...")
         invoke_path = c.run("which invoke", hide=True).stdout.strip()
         pip_path = invoke_path.replace("/invoke", "/pip")
-        print("running:", pip_path + " install pyyaml")
-        c.run(pip_path + " install pyyaml")
+        print(f"running: {pip_path} install pyyaml")
+        c.run(f"{pip_path} install pyyaml")
         import yaml
     if not machine_name:
         print("Machine name required. Use -m or --machine-name", file=sys.stderr)
     output = c.run("multipass list --format yaml", hide=True).stdout.strip()
     machines = yaml.load(output, yaml.SafeLoader)
     if machine_name not in machines:
         print(
@@ -90,17 +91,18 @@
                             r"  +", " ", f'{first_address}      {line.split(" ",1)[1]}'
                         )
                     )
                     print(new_hosts[-1])
                 else:
                     new_hosts.append(line)
             c: invoke.Context
-            # simpelweg overschrijven via een echo of cat >> /etc/hosts mag niet. dus dan maar via een python script.
-            overwrite_hosts_command = """python3 -c "import sys \nwith open('/etc/hosts','w') as h: h.write(sys.stdin.read().strip())" <<EOFEOFEOF\n"""
-            overwrite_hosts_command += "\n".join(new_hosts)
+            overwrite_hosts_command = (
+                """python3 -c "import sys \nwith open('/etc/hosts','w') as h: h.write(sys.stdin.read().strip())" <<EOFEOFEOF\n"""
+                + "\n".join(new_hosts)
+            )
             overwrite_hosts_command += "\nEOFEOFEOF"
             c.sudo("ls >> /dev/null")  # force a sudo to ask for password
             c.sudo(overwrite_hosts_command)
         else:
             print("Appending to hosts file")
             c.sudo("ls >> /dev/null")  # force a sudo to ask for password
             line_to_append = re.sub(
@@ -117,29 +119,29 @@
 def prepare_multipass(c, machine_name):
     print(" ... Searching for vms")
     machines = json.loads(c.run("multipass list --format json", hide=True).stdout)[
         "list"
     ]
     # convert to lookup by name
     machines = {m["name"]: m for m in machines}
-    if not machine_name in machines:
+    if machine_name not in machines:
         raise KeyError(
             f'Machine name "{machine_name}" not found in multipass. Available names: {", ".join(list(machines.keys()))}'
         )
     machine = machines[machine_name]
     ip = machine["ipv4"][0]
     print(f" [x] {machine_name} found @ {ip} ")
     multipass_keyfile = pathlib.Path("~/.ssh/multipass.key").expanduser()
     if not multipass_keyfile.exists():
         # create keyfile
         generate_key(c, "pyinvoke access to multipass machines", str(multipass_keyfile))
         print(" [x] created missing key file")
     else:
         print(" [x] key file exists")
-    pub_file = pathlib.Path(str(multipass_keyfile) + ".pub")
+    pub_file = pathlib.Path(f"{str(multipass_keyfile)}.pub")
     pub_key = pub_file.read_text().strip()
     if (
         pub_key
         in c.run(
             f'echo "cat .ssh/authorized_keys ; exit " | multipass shell {machine_name}',
             warn=False,
             hide=True,
@@ -149,12 +151,13 @@
     else:
         print(" [ ] installing public key to access machine")
         c.run(
             f'echo "echo {pub_key} >> .ssh/authorized_keys; exit" | multipass shell {machine_name}',
             hide=True,
         )
         print(f" [x] installed multipass keyfile on {machine_name}")
-    print("Execute fabric with:")
-    fab_commands = "|".join(c.run("fab --complete",hide=True).stdout.strip().split("\n"))
-    print(f"  fab -eH ubuntu@{ip} [{fab_commands}]")
-    print(f'  fab -eH ubuntu@{ip} -- echo "or some other arbitrary bash command"')
+    edwh_cmd = pathlib.Path(sys.argv[0]).name
+    print(f"Execute {edwh_cmd} with:")
+    fab_commands = "|".join(c.run(f"{edwh_cmd} --complete",hide=True).stdout.strip().split("\n"))
+    print(f"  {edwh_cmd} -eH ubuntu@{ip} [{fab_commands}]")
+    print(f'  {edwh_cmd} -eH ubuntu@{ip} -- echo "or some other arbitrary bash command"')
```

### Comparing `edwh_multipass_plugin-1.0.0/LICENSE.txt` & `edwh_multipass_plugin-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_multipass_plugin-1.0.0/README.md` & `edwh_multipass_plugin-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 pip install edwh-multipass-plugin
 ```
 
 But probably you want to install the whole `edwh` package:
 
 ```console
 pipx install edwh[plugins,omgeving]
+# or
+pipx install edwh[multipass]
 ```
 
 if you want to use the `edwh` command line tool with just the `multipass` plugin:
 
 ```console
 pipx install edwh
 pipx inject edwh edwh-multipass-plugin
```

### Comparing `edwh_multipass_plugin-1.0.0/pyproject.toml` & `edwh_multipass_plugin-1.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "edwh-multipass-plugin"
 dynamic = ["version"]
 description = 'An `edwh`plugin to work with multipass instances for local development.'
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MIT"
-keywords = []
+keywords = ['edwh','multipass','plugin','invoke']
 authors = [
   { name = "Remco", email = "remco@educationwarehouse.nl" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.10",
@@ -51,22 +51,23 @@
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
 
 [[tool.hatch.envs.all.matrix]]
-python = ["3.10", "3.11"]
+python = ["3.11"]
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
   "black>=23.1.0",
   "mypy>=1.0.0",
   "ruff>=0.0.243",
+  'pip',
 ]
 [tool.hatch.envs.lint.scripts]
 typing = "mypy --install-types --non-interactive {args:src/edwh_multipass_plugin tests}"
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
 ]
@@ -154,7 +155,16 @@
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
+
+[tool.semantic_release]
+version_variable = "src/edwh_multipass_plugin/__about__.py:__version__"
+branch = "main"
+change_log = "CHANGELOG.md"
+upload_to_repository = false
+upload_to_release = false
+build_command = "hatch build -c"
+
```

### Comparing `edwh_multipass_plugin-1.0.0/PKG-INFO` & `edwh_multipass_plugin-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: edwh-multipass-plugin
-Version: 1.0.0
+Version: 1.0.1
 Summary: An `edwh`plugin to work with multipass instances for local development.
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-multipass-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-multipass-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-multipass-plugin
 Author-email: Remco <remco@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
+Keywords: edwh,invoke,multipass,plugin
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
@@ -41,14 +42,16 @@
 pip install edwh-multipass-plugin
 ```
 
 But probably you want to install the whole `edwh` package:
 
 ```console
 pipx install edwh[plugins,omgeving]
+# or
+pipx install edwh[multipass]
 ```
 
 if you want to use the `edwh` command line tool with just the `multipass` plugin:
 
 ```console
 pipx install edwh
 pipx inject edwh edwh-multipass-plugin
```

