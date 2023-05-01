# Comparing `tmp/edwh_server_provisioning_plugin-0.1.3b1.tar.gz` & `tmp/edwh_server_provisioning_plugin-0.2.0.tar.gz`

## Comparing `edwh_server_provisioning_plugin-0.1.3b1.tar` & `edwh_server_provisioning_plugin-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    23482 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3b1/.dcignore
--rw-r--r--   0        0        0    14236 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3b1/CHANGELOG.md
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3b1/old_documentation_in_dutch.md
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3b1/src/edwh_server_provisioning_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3b1/src/edwh_server_provisioning_plugin/__init__.py
--rw-r--r--   0        0        0    45350 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3b1/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3b1/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3b1/LICENSE.txt
--rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3b1/pyproject.toml
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3b1/readme.md
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.1.3b1/PKG-INFO
+-rw-r--r--   0        0        0    23482 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.0/.dcignore
+-rw-r--r--   0        0        0    15518 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.0/old_documentation_in_dutch.md
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.0/src/edwh_server_provisioning_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.0/src/edwh_server_provisioning_plugin/__init__.py
+-rw-r--r--   0        0        0    45511 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.0/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.0/readme.md
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 edwh_server_provisioning_plugin-0.2.0/PKG-INFO
```

### Comparing `edwh_server_provisioning_plugin-0.1.3b1/.dcignore` & `edwh_server_provisioning_plugin-0.2.0/.dcignore`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.1.3b1/CHANGELOG.md` & `edwh_server_provisioning_plugin-0.2.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.2.0 (2023-05-01)
+### Feature
+* **do:** Remote.do now supports --edwh flag which works similar to --invoke but for 'edwh' commands ([`6987fa8`](https://github.com/educationwarehouse/server_provisioning/commit/6987fa89741177de6e2046d1782fec860dc7d879))
+* **postgres:** Connect-postgres now accepts --omgeving to select a directory to read postgres port from dc ([`4b2fcda`](https://github.com/educationwarehouse/server_provisioning/commit/4b2fcda3eaee7a2e9d4610a744c115a7633fcf45))
+* Added auto edwh install when prepare_generic_server is called ([`f2e41df`](https://github.com/educationwarehouse/server_provisioning/commit/f2e41df419213924fd53e493fc8514d8dc78ea16))
+
+### Fix
+* **dev:** Additional dependencies for dev now exclude semantic-release, which conflicts with invoke 2.0 ([`6e98b1a`](https://github.com/educationwarehouse/server_provisioning/commit/6e98b1a905ab92ec2518a4018e95db6ac4edc096))
+
+## v0.1.3 (2023-04-25)
+### Fix
+* Now removes github keys before reassigning using `ssh -o StricHostKeyChecking=accept-new` to flush the old one and insert a new one. Also adds a better warning when installing a repo inside a git-repo (which you can't). ([`5402e03`](https://github.com/educationwarehouse/server_provisioning/commit/5402e0322301380dbd9e9abcdfe99457c7b4d288))
+
 ## v0.1.3-beta.1 (2023-04-25)
 ### Fix
 * `ssh -tt` instead of `ssh -t` to avoid `pseudo-terminal  will not be allocated because stdin is not a terminal` ([`fa18bd9`](https://github.com/educationwarehouse/server_provisioning/commit/fa18bd980763790df7ef3a34c4193d1b171189a2))
 
 ## v0.1.2 (2023-04-17)
 ### Documentation
 * **versions:** Remove unsupported python versions + fix md badges ([`d696150`](https://github.com/educationwarehouse/server_provisioning/commit/d696150b974bb8e37faf08ebcbc9d524d3d29586))
```

### Comparing `edwh_server_provisioning_plugin-0.1.3b1/old_documentation_in_dutch.md` & `edwh_server_provisioning_plugin-0.2.0/old_documentation_in_dutch.md`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.1.3b1/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py` & `edwh_server_provisioning_plugin-0.2.0/src/edwh_server_provisioning_plugin/server_provisioning_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import io
 import os
 import pprint
 import re
 import sys
 import textwrap
 import time
+import typing
 import urllib.parse
 from abc import ABC
 from datetime import datetime
 from pathlib import Path
 from textwrap import dedent
 
 import yaml
@@ -34,18 +35,14 @@
 $PATH.extend(':~/.local/bin/')
 #$FLIT_USERNAME='...'
 #$FLIT_PASSWORD='...'
 $PROMPT_FIELDS['prompt_end'] = $PROMPT_FIELDS['prompt_end'].replace('$', '{WHITE}@')
 $PROMPT = '{env_name}{BOLD_GREEN}{user}@{hostname}{BOLD_BLUE} {short_cwd}{branch_color}{curr_branch: {}}{NO_COLOR} {BOLD_BLUE}{prompt_end}{NO_COLOR} '
 """
 
-GITHUB_KNOWN_HOSTS = """
-|1|GNDleqLr6aOVYd889BVVy2ErPA4=|XdPSQ2p/b47kjCr8gt/vKTi+KT0= ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIOMqqnkVzrm0SdG6UOoqKLsabgH5C9okWi0dh2l9GKJl
-"""
-
 JOPLIN_DOCKER_COMPOSE = """
 version: '3.3'
 services:
     proxy:
         image: "traefik:v2.5"
         container_name: "traefik"
         restart: unless-stopped
@@ -139,30 +136,34 @@
                 count_keys += 1
         if count_keys == len(command_line_key):
             for which_key in command_line_key:
                 for head_keys in all_key_information:
                     if which_key in head_keys:
                         for key, value in all_key_information[head_keys].items():
                             # gaat alleen de 'sleutel' toevoegen en niet de datetime enzovoort
-                            if bool(key.find('datetime')) and bool(key.find('wie@hostname')) and bool(
-                                    key.find('message')) is True:
+                            if (
+                                bool(key.find('datetime'))
+                                and bool(key.find('wie@hostname'))
+                                and bool(key.find('message')) is True
+                            ):
                                 c.run(f'echo {value} >> ~/.ssh/authorized_keys')
                                 c.run('touch ~/.ssh/keys')
                                 c.run('sort -u ~/.ssh/authorized_keys > ~/.ssh/keys')
                                 time.sleep(1)
                                 c.run('cp ~/.ssh/keys ~/.ssh/authorized_keys')
                                 c.run('rm ~/.ssh/keys')
                                 print(f'Het is gelukt! De \033[1m{which_key}\033[0m key is toegevoegd.')
         else:
             # verwijder alle keys die WEL in de yaml file staan
             not_in_yaml_keys = command_line_key
             for head_keys in all_key_information:
                 not_in_yaml_keys = [which_key for which_key in not_in_yaml_keys if which_key not in head_keys]
             print(
-                f'Verkeerde \033[1m{" ".join(not_in_yaml_keys)}\033[0m key, controleer eerst of je de juiste key hebt ingevuld. Of als die wel in de YAML file staat.')
+                f'Verkeerde \033[1m{" ".join(not_in_yaml_keys)}\033[0m key, controleer eerst of je de juiste key hebt ingevuld. Of als die wel in de YAML file staat.'
+            )
             for which_key in not_in_yaml_keys:
                 split_key = which_key.replace('-', ' ')
                 generate_doel = ''
                 if len(split_key.split()) == 3:
                     generate_doel = split_key.split()[2]
                 # maak de key aan die nog NIET in de yaml file stond
                 if input(f"Wil je de {which_key} key aanmaken? [Yn]") in ("y", "Y", ""):
@@ -172,16 +173,21 @@
                         exit(1)
                     # print('\n\nJe moet minimaal 2/3 invullen: Owner, Hostname en/of Doel!!\n\n')
                     # owner = str(input("Wie is de owner van de Private key?"'\n')) or ''
                     # hostname = str(input('Wie is de specifieke host? bvb: productie - testomgeving - naam van de stagiar''\n')) or ''
                     # doel = str(input('Waarom maak je deze key aan?''\n')) or ''
                     # generate(c, message, owner=owner.replace(" ", ""), hostname=hostname.replace(" ", ""), doel=doel.replace(" ", ""))
                     # voer dus de functie generate_keys uit om de key dus daadwerkelijk aan te maken
-                    generate_key(c, generate_message, owner=split_key.split()[0], hostname=split_key.split()[1],
-                                 doel=generate_doel)
+                    generate_key(
+                        c,
+                        generate_message,
+                        owner=split_key.split()[0],
+                        hostname=split_key.split()[1],
+                        doel=generate_doel,
+                    )
                     # bekijk of nu wel alle keys in de yaml file staan, zo ja, ga dan alsnog toevoegen
                     if head_keys in command_line_key:
                         count_keys += 1
                     if count_keys == len(command_line_key):
                         append_key_to_remote(c, command_line_key)
 
 
@@ -197,16 +203,19 @@
         key_db: dict = yaml.load(yaml_file, Loader=SafeLoader)
         all_key_information = key_db.setdefault('sleutels')
     for which_key in command_line_key:
         for head_keys in all_key_information:
             if which_key in head_keys:
                 for key, value in all_key_information[head_keys].items():
                     # gaat alleen de 'sleutel' toevoegen en niet de datetime enzovoort
-                    if bool(key.find('datetime')) and bool(key.find('wie@hostname')) and bool(
-                            key.find('message')) is True:
+                    if (
+                        bool(key.find('datetime'))
+                        and bool(key.find('wie@hostname'))
+                        and bool(key.find('message')) is True
+                    ):
                         # pakt de juiste sleutel en 'verwijdert' die sleutel
                         c.run(f'grep -v "{value}" ~/.ssh/authorized_keys > ~/.ssh/keys')
                         c.run('mv ~/.ssh/keys ~/.ssh/authorized_keys')
                         print(f'Het is gelukt! De \033[1m{which_key}\033[0m key is verwijderd.')
 
 
 @task
@@ -251,23 +260,22 @@
     whoami_local = whoami_local_handle.read().replace('\n', '')
     whoami_local_handle.close()
     cat_local_public_key_handle = os.popen(f'cat ~/.managed_ssh_keys-{key_name}.pub')
     cat_local_public_key = cat_local_public_key_handle.read().replace('\n', '')
     cat_local_public_key_handle.close()
     # zo komt het dus er uit te zien in de yaml file
     sleutel_dict = {
-        'sleutels':
-            {key_name:
-                {
-                    'sleutel': cat_local_public_key,
-                    'datetime': datetime.today().strftime("Datum: %Y-%m-%d Tijdstip: %H:%M:%S"),
-                    'wie@hostname': whoami_local,
-                    'message': message
-                }
+        'sleutels': {
+            key_name: {
+                'sleutel': cat_local_public_key,
+                'datetime': datetime.today().strftime("Datum: %Y-%m-%d Tijdstip: %H:%M:%S"),
+                'wie@hostname': whoami_local,
+                'message': message,
             }
+        }
     }
     # voor de eerste keer (wanneer het script dus nog niet bestond) wordt de hoofdkey sleutels nog aangemaakt en anders wordt het erin toegevoegd.
     with open('key_holder.yaml', 'w') as stream:
         try:
             if key_db is not None:
                 new_key_dict = sleutel_dict.pop('sleutels')
                 all_key_information.update(new_key_dict)
@@ -372,23 +380,23 @@
         print('Er staan nog geen sleutels op deze remote machine die in de yaml file staan...')
         print('\033[1mlocal\033[0m')
         for head_keys in all_key_information:
             print(head_keys)
 
 
 class RemoteWentWrong(Exception):
-
     pass
 
 
 def failsafe(callable):
     "Executes the callable, and if not result.ok raises a RemoteWentWrong exception."
     result: Result = callable()
     if not result.ok:
         raise RemoteWentWrong(result.stderr)
+    return result
 
 
 class TestOnce(ABC):
     tested = False
 
     @classmethod
     def test(cls, c):
@@ -414,17 +422,15 @@
             )
             exit(1)
 
 
 class OsVersionCheck(TestOnce):
     @classmethod
     def evaluate(cls, c):
-        if "22.04" not in (
-                version := c.run("lsb_release -a", hide=True, warn=True).stdout
-        ):
+        if "22.04" not in (version := c.run("lsb_release -a", hide=True, warn=True).stdout):
             print(
                 f"ERROR: Ubuntu version {version} other than 22.04 is detected, aborting. ",
                 file=sys.stderr,
             )
             exit(1)
 
 
@@ -470,17 +476,15 @@
         ],
     )
 
 
 @task
 def add_apt_repository(c, gpg_url, repo_url):
     c.run(f"curl -fsSL {gpg_url} | sudo apt-key add -")
-    c.sudo(
-        f'add-apt-repository "deb [arch=amd64] {repo_url} $(lsb_release -cs) stable"'
-    )
+    c.sudo(f'add-apt-repository "deb [arch=amd64] {repo_url} $(lsb_release -cs) stable"')
     apt_upgrade(c)
 
 
 @task
 def add_user_to_group(c, group):
     current_groups = c.run("groups").stdout
     if group not in current_groups:
@@ -503,17 +507,15 @@
     if execution_fails(c, "docker-compose --version"):
         failsafe(lambda: c.sudo("pip3 install docker-compose"))
 
     if "microservices" not in c.run("groups").stdout:
         # maak een nieuwe microservices group met dit specifieke ID
         c.sudo("addgroup --gid 1050 microservices")
         # maak hier ook een nieuwe suer voor aan, met hetzelfde ID die niet mag inloggen
-        c.sudo(
-            "adduser --uid 1050 --gid 1050 --disabled-password --disabled-login --system microservices"
-        )
+        c.sudo("adduser --uid 1050 --gid 1050 --disabled-password --disabled-login --system microservices")
         # voeg deze gebruiker toe aan die nieuwe groep
         c.sudo("usermod --groups microservices --append `whoami`")
 
     add_user_to_group(c, "docker")
 
 
 @task
@@ -556,57 +558,51 @@
 @task
 def set_noninteractive(c):
     c.run("export DEBIAN_FRONTEND=noninteractive")
 
 
 @task
 def prepare_git_client(
-        c,
-        username,
-        email,
+    c,
+    username,
+    email,
 ):
     c: Connection = c
     print(c.host)
     return
     # git config --global --add user.name spore
     c.run(f"git config --global --add user.name {username}")
     # git config --global --add user.email spore@edwh.nl
     c.run(f"git config --global --add user.email {email}")
     # git config --global core.editor "vim"
     c.run(f'git config --global core.editor "vim"')
 
 
 @task
-def clone_git_repo_with_new_key_file_for_edwh_repos(
-        c, repo, rw, target_directory="", branch=None
-):
+def clone_git_repo_with_new_key_file_for_edwh_repos(c, repo, rw, target_directory="", branch=None):
     c: Connection = c
     git_user, git_repo = repo.split("/")
     if git_user == "educationwarehouse":
         # alleen sleutels gebruiken voor edwh eigen repo's, voor de rest is anon access genoeg
         assert rw in ("r", "rw"), "rw should be either r or rw"
         # ssh-keygen -t ed25519 -C "bla die pir" -f .ssh/bla_die_pir.key -N ""
         # -t == type : ecc type
         # -C == comment, geef naam op
         # -f == Destination file, neemt aan dat cwd == ~
         # -N == new passphrase. blanco dus.
         username = c.run("whoami").stdout.strip()
         host = c.host
         if host == "localhost":
-            raise ValueError(
-                "Do not connect with localhost, use the hostname to avoid collisions in the keyfilename. "
-            )
+            raise ValueError("Do not connect with localhost, use the hostname to avoid collisions in the keyfilename. ")
         filename = f"git-{git_user}-{git_repo}-{rw}".lower()
         if execution_fails(c, f"cat .ssh/{filename}.pub"):
-            comment = f"{username}@{host} for {rw.lower()} on git:{git_user}/{git_repo} added {datetime.now().isoformat()}"
-            failsafe(
-                lambda: c.run(
-                    f'ssh-keygen -t ed25519 -C "{comment}" -f .ssh/{filename} -N ""'
-                )
+            comment = (
+                f"{username}@{host} for {rw.lower()} on git:{git_user}/{git_repo} added {datetime.now().isoformat()}"
             )
+            failsafe(lambda: c.run(f'ssh-keygen -t ed25519 -C "{comment}" -f .ssh/{filename} -N ""'))
             key = c.run(f"cat .ssh/{filename}.pub").stdout
             url = f"https://github.com/{git_user}/{git_repo}/settings/keys/new"
             print(f"Post this key on the following page: {url}")
             print(key)
             input("\n\nPress enter when done.")
 
             # $ cat ~/.ssh/config
@@ -622,42 +618,35 @@
             """
             )
             # Host github.com-ontwikkelstraat
             #         Hostname github.com
             #         IdentityFile=/home/ubuntu/.ssh/git-ontwikkelstraat.id_rsa
             c.put(io.StringIO(config), ".ssh/config")
 
-        # fix the .ssh/known_hosts
-        known_hosts = c.run(f"cat .ssh/known_hosts", warn=True).stdout
-        if GITHUB_KNOWN_HOSTS.strip() not in known_hosts:
-            known_hosts += GITHUB_KNOWN_HOSTS
-            print("Adding github.com signatures to .ssh/known_hosts")
-            c.put(io.StringIO(known_hosts), ".ssh/known_hosts")
         # respond_to_security=Responder(r'Are you sure you want to continue connecting \(yes/no/\[fingerprint\]\)\?.*','yes\n')
-        # failsafe(lambda:c.run(f'ssh -tN git@github.com', watchers=[respond_to_security]))
 
         # check als machine correcte git ssh verbinding kan maken
         # fingerprint
-        if failsafe("Permission denied" in c.run("ssh -tt git@github.com", hide=True)).stderr:
-            raise Exception("github key klopt niet, CHECK ALS GITHUB_KNOWN_HOSTS KEY KLOPT IN DE server_provisioning_plugin.py")
-
-        # test if the repo exists:
         if (
-                "fatal:"
-                in c.run(
-            f"cd {target_directory or git_repo}; git status", warn=True, hide=True
-        ).stderr
+            "Permission denied (publickey)"
+            in c.run(
+                "ssh-key -R github.com && ssh -tt -o StrictHostKeyChecking=accept-new git@github.com",
+                hide=True,
+                warn=True,
+            ).stderr
         ):
-            failsafe(
-                lambda: c.run(
-                    f"git clone git@github.com-{git_repo}:{git_user}/{git_repo} {target_directory}"
-                )
+            raise Exception(
+                "github key klopt niet, CHECK ALS GITHUB_KNOWN_HOSTS KEY KLOPT IN DE server_provisioning_plugin.py"
             )
+
+        # test if the repo exists:
+        if "fatal:" in c.run(f"cd {target_directory or git_repo}; git status", warn=True, hide=True).stderr:
+            failsafe(lambda: c.run(f"git clone git@github.com-{git_repo}:{git_user}/{git_repo} {target_directory}"))
         else:
-            print(f"Repo {git_repo} already installed")
+            print(f"Repo {git_repo} already installed in {target_directory}, or a git repository exists higher-up")
         if branch:
             c.run(f"cd {target_directory}; git checkout {branch}")
     else:
         # anonymous git
         failsafe(lambda: c.run(f"git clone https://github.com/{git_user}/{git_repo}"))
 
 
@@ -665,56 +654,40 @@
     pass
 
 
 @task()
 def assert_root_disabled_on_ssh(c):
     print(f"Validating SSHd config file disallows root on {c.host}.")
     sshd_config_parts = (
-        c.sudo("grep -i PermitRootLogin /etc/ssh/sshd_config", warn=True, hide=True)
-        .stdout.strip()
-        .split("\n")
+        c.sudo("grep -i PermitRootLogin /etc/ssh/sshd_config", warn=True, hide=True).stdout.strip().split("\n")
     )
     if sshd_config_parts:
-        enabled_linecount = sum(
-            1 for line in sshd_config_parts if not line.startswith("#")
-        )
+        enabled_linecount = sum(1 for line in sshd_config_parts if not line.startswith("#"))
         if enabled_linecount:
             print(
                 """Invalid content in: \n\t""",
                 "\t\n".join(sshd_config_parts),
                 file=sys.stderr,
             )
             raise SecurityException(
                 "PermitRootLogin found enabled in /etc/ssh/sshd_config on target host. Disable manually. "
             )
-    authorized_keys = (
-        c.sudo("cat /root/.ssh/authorized_keys", warn=True, hide=True)
-        .stdout.strip()
-        .split("\n")
-    )
+    authorized_keys = c.sudo("cat /root/.ssh/authorized_keys", warn=True, hide=True).stdout.strip().split("\n")
     if len(authorized_keys) > 1:
-        raise SecurityException(
-            "There should only be one key in /root/.ssh/authorized_keys"
-        )
+        raise SecurityException("There should only be one key in /root/.ssh/authorized_keys")
     if "command=" not in authorized_keys[0].lower():
-        raise SecurityException(
-            "Missing a blocking command section in /root/.ssh/authorized_keys"
-        )
+        raise SecurityException("Missing a blocking command section in /root/.ssh/authorized_keys")
     print("Good, root seems unable to login.")
 
 
 @task()
 def assert_passwords_disabled_on_ssh(c):
     print(f"Validating SSHd config file disallows passwords on {c.host}.")
     sshd_config_parts = (
-        c.sudo(
-            "grep -i PasswordAuthentication /etc/ssh/sshd_config", hide=True, warn=True
-        )
-        .stdout.strip()
-        .split("\n")
+        c.sudo("grep -i PasswordAuthentication /etc/ssh/sshd_config", hide=True, warn=True).stdout.strip().split("\n")
     )
     if sshd_config_parts:
         for line in sshd_config_parts:
             line = line.strip()
             if line.startswith("#"):
                 # ignore comments
                 continue
@@ -727,18 +700,15 @@
                     )
     print("Good, password authentication seems disabled")
 
 
 @task()
 def set_root_password(c, password=None, overwrite=False):
     "Sets remote root password to given password, or asks the user for one."
-    shadow = [
-        line.strip().split(":")
-        for line in c.sudo("cat /etc/shadow", hide=True).stdout.strip().split("\n")
-    ]
+    shadow = [line.strip().split(":") for line in c.sudo("cat /etc/shadow", hide=True).stdout.strip().split("\n")]
     for username, password_hash, *_ in shadow:
         if username == "root":
             if len(password_hash) > 1:
                 # Some password exists for root
                 if not overwrite:
                     print("Not overwriting existing root password.")
                     return
@@ -777,19 +747,15 @@
     assert_passwords_disabled_on_ssh(c)
     print("Current open ports:")
     get_open_ports(c)
     print("Setup up firewall on ", c.host)
     c.sudo(f"ufw disable")
     c.sudo(f"ufw reset")
     ports = [mapping.split(":")[1] for mapping in portmapping.split(";")]
-    service_ports = dict(
-        mapping.split(":")
-        for mapping in portmapping.split(";")
-        if not mapping.startswith(":")
-    )
+    service_ports = dict(mapping.split(":") for mapping in portmapping.split(";") if not mapping.startswith(":"))
     ports = [int(_) for _ in ports.strip().split(",") if int(_)]
     if 22 not in ports:
         # niet jezelf uitsluiten
         ports.append(22)
     for port in ports:
         print("Allowing", port)
         c.sudo(f"ufw allow {port}", hide=True)
@@ -818,26 +784,33 @@
 @task()
 def get_open_ports(c):
     print("Checking", c.host)
     c.sudo("ufw status verbose")
 
 
 @task()
+def install_edwh(c):
+    if execution_fails(c, c.run("pipx install edwh[omgeving,plugins]")):
+        c.run("pipx upgrade edwh")
+
+
+@task()
 def prepare_generic_server(
-        c,
+    c,
 ):
     """Updates apt and dist-upgrades the machine. Installs python, docker, docker-compose, and xonsh.
 
     A default .xonshrc is added, as well as a microservices group and the current user is added to both
     the docker group as well as the microservices group.
     """
     set_noninteractive(c)
     prepare_apt(c)
     install_python(c)
     install_docker(c)
+    install_edwh(c)
     install_xonsh(c)
     assert_passwords_disabled_on_ssh(c)
     assert_root_disabled_on_ssh(c)
 
 
 @task
 def install_joplin(c):
@@ -891,42 +864,65 @@
 #     # tot hier ...
 #     # .env file instellen/kopieren
 #     # docker builden via `docker-compose build`
 #     # uitvoeren via `invoke up -d?`
 #
 
 
+def at_least(iterable: typing.Iterable, n: int):
+    """
+    Like 'all()' or 'any()' but for at least 'n'
+
+    https://stackoverflow.com/questions/42514445/clever-any-like-function-to-check-if-at-least-n-elements-are-true
+    """
+    if n < 1:
+        return True
+    counter = 0
+    for x in iterable:
+        if x:
+            counter += 1
+            if counter == n:
+                return True
+    return False
+
+
 @task(
     iterable=["omgeving"],
     help=dict(
         omgeving="Directory waarin opdrachten worden uitgevoerd, kan meerdere keren voorkomen.",
         cmd="Willekeurig welk shell commando.",
         invoke='argumenten aan invoke, denk eraan dat er 1 argument wordt opgegeven vanuit de cli, dus gebruik "" om meerdere mee te geven.',
     ),
 )
-def do(c, omgeving=["."], cmd=None, invoke=None):
+def do(c, omgeving=None, cmd=None, invoke=None, edwh=None):
     """Voert remote commandos of invoke statements uit, binnen de opgegeven omgeving(en).
 
     cmd kan ook gebruikt worden voor troubleshooting/scripting.
     bijvoorbeeld:
 
       fab -H utils do --omgeving taiga --invoke "restart --quick" -e
 
     """
+    current_user = os.getlogin()
+    bin_path = f"/home/{current_user}/.local/bin"
+
     if not omgeving:
         omgeving = ["."]
-    if cmd:
-        commando = cmd
-    elif invoke:
-        commando = f"/home/ubuntu/.local/bin/invoke {invoke}"
-    elif cmd and invoke:
+
+    if at_least([cmd, invoke, edwh], 2):
         print("Gebruik slechts --invoke of --cmd, niet beide")
         exit(1)
+    elif cmd:
+        commando = cmd
+    elif invoke:
+        commando = f"{bin_path}/invoke {invoke}"
+    elif edwh:
+        commando = f"{bin_path}/edwh {edwh}"
     else:
-        print("Gebruik ofwel cmd of invoke")
+        print("Gebruik ofwel cmd, edwh of invoke")
         exit(1)
     for directory in omgeving:
         print("Uitvoeren voor ", directory)
         # omgeving is een lijst van omgevingen
         c.run(f"cd {directory}; {commando}")
 
 
@@ -957,37 +953,34 @@
     install_ontwikkelstraat(c)
     if is_production:
         subscription_key = input(
             "WithSecure linux server Subscription Key (https://elements.f-secure.com/apps/psb/c556915/subscription) [blank=ignore]: "
         )
         if subscription_key.strip():
             install_antivirus(c, subscription_key=subscription_key)
-            print(
-                "/!\ Denk eraan, hier moet nog een profiel aan gekoppeld worden in de withsecure website! "
-            )
+            print("/!\ Denk eraan, hier moet nog een profiel aan gekoppeld worden in de withsecure website! ")
 
 
 @task
 def install_antivirus(c, subscription_key):
     c: Connection
     subscription_key: str
     c.run(
         "curl https://download.sp.f-secure.com/linuxsecurity64/f-secure-linuxsecurity.deb -o f-secure-linuxsecurity.deb"
     )
     c.sudo("dpkg -i f-secure-linuxsecurity.deb")
     # https://help.f-secure.com/product.html#business/linux-protection/latest/en/task_7C893CC525EF4BA5B7B4477FDE23E40F-latest-en
-    c.sudo(
-        f"/opt/f-secure/linuxsecurity/bin/activate --psb --subscription-key {subscription_key}"
-    )
+    c.sudo(f"/opt/f-secure/linuxsecurity/bin/activate --psb --subscription-key {subscription_key}")
 
 
 # @task
 # def new_proxy(c, docker_compose_path):
 #     dc_path =
 
+
 def read_dotenv_remote(c: Connection, path: Path):
     lines = c.run(f"cat {path}", hide=True).stdout.split("\n")
 
     # remove comments
     lines = [line.split("#", 1)[0] for line in lines]
     # remove redundant whitespace
     lines = [line.strip() for line in lines]
@@ -996,14 +989,15 @@
     # convert to tuples
     items = [line.split("=", 1) for line in lines]
     # clean the tuples
     items = [(key.strip(), value.strip()) for key, value in items]
     # convert to dict for quick lookup of keys
     return dict(items)
 
+
 @task
 def connect_postgres(c, omgeving=None, port=None, local_port=None):
     """
     Forward a remote port (--port or 5432) to the host machine (--local-port or 5432).
     If --omgeving is passed, the PG_PORT is used from the .env file (or 5432)
     """
 
@@ -1022,25 +1016,25 @@
     if local_port:
         local_port = int(local_port)
     else:
         local_port = 5432
 
     c: Connection
     import time
+
     with c.forward_local(local_port, port, '127.0.0.1', '127.0.0.1'):
         print(f'Connected remote :{port} to local :{local_port}, sleeping until Ctrl-C')
         while True:
             try:
                 time.sleep(3)
             except KeyboardInterrupt:
                 print('closing connection.')
                 break
 
 
-
 @task
 def require_npx(c):
     # npm installs npx
     c.sudo('npm --version > /dev/null || sudo apt install npm -y')
 
 
 def background_run(c, command):
@@ -1141,17 +1135,21 @@
           # gzip compress 
           - "traefik.http.middlewares.{service}-compress.compress=true"
     
     """
     )
     print("------- [new] ---------------------------------------------------- ")
     print(compose_fragment)
-    if yes or input(
-            f"append to {docker_compose_path}/docker-compose.yaml? [NO,yes] #"
-    ).lower().strip() in ("y", "yes", "j", "ja", "1"):
+    if yes or input(f"append to {docker_compose_path}/docker-compose.yaml? [NO,yes] #").lower().strip() in (
+        "y",
+        "yes",
+        "j",
+        "ja",
+        "1",
+    ):
         print("Copying compose file to docker-compose.bak")
         c.run(
             f"cp {docker_compose_path}/docker-compose.yaml {docker_compose_path}/docker-compose.bak",
             hide=True,
         )
         # craft the directory if it doesn't exist already
         c.run(f"mkdir {docker_compose_path}/{path}_content", warn=True, hide=True)
```

### Comparing `edwh_server_provisioning_plugin-0.1.3b1/LICENSE.txt` & `edwh_server_provisioning_plugin-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.1.3b1/pyproject.toml` & `edwh_server_provisioning_plugin-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ['fabric', 'pyyaml', 'tabulate']
 
 [project.optional-dependencies]
 dev = [
     "hatch",
-    "python-semantic-release",
+    # "python-semantic-release",
     "black",
 ]
 
 [project.urls]
 Documentation = "https://github.com/educationwarehouse/server_provisioning#readme"
 Issues = "https://github.com/educationwarehouse/server_provisioning/issues"
 Source = "https://github.com/educationwarehouse/server_provisioning"
```

### Comparing `edwh_server_provisioning_plugin-0.1.3b1/readme.md` & `edwh_server_provisioning_plugin-0.2.0/readme.md`

 * *Files identical despite different names*

### Comparing `edwh_server_provisioning_plugin-0.1.3b1/PKG-INFO` & `edwh_server_provisioning_plugin-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-server-provisioning-plugin
-Version: 0.1.3b1
+Version: 0.2.0
 Summary: Fabric-based remote server management plugin for `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/server_provisioning#readme
 Project-URL: Issues, https://github.com/educationwarehouse/server_provisioning/issues
 Project-URL: Source, https://github.com/educationwarehouse/server_provisioning
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -17,15 +17,14 @@
 Requires-Python: >=3.10
 Requires-Dist: fabric
 Requires-Dist: pyyaml
 Requires-Dist: tabulate
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
-Requires-Dist: python-semantic-release; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # edwh-server-provisioning-plugin
 
 [![PyPI - Version](https://img.shields.io/pypi/v/edwh-server-provisioning-plugin.svg)](https://pypi.org/project/edwh-server-provisioning-plugin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edwh-server-provisioning-plugin.svg)](https://pypi.org/project/edwh-server-provisioning-plugin)
```

