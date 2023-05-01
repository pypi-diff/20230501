# Comparing `tmp/yog-2.1.5.tar.gz` & `tmp/yog-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yog-2.1.5.tar", max compression
+gzip compressed data, was "yog-2.1.6.tar", max compression
```

## Comparing `yog-2.1.5.tar` & `yog-2.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    10174 2023-02-25 02:02:07.903436 yog-2.1.5/README.md
--rw-r--r--   0        0        0      541 2023-04-18 02:34:04.537034 yog-2.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2021-07-16 04:35:58.316463 yog-2.1.5/yog/__init__.py
--rw-r--r--   0        0        0      465 2023-02-22 20:50:59.508191 yog-2.1.5/yog/command.py
--rw-r--r--   0        0        0      636 2021-11-19 21:53:36.530661 yog-2.1.5/yog/git_utils.py
--rw-r--r--   0        0        0        0 2021-11-19 21:18:00.056940 yog-2.1.5/yog/host/__init__.py
--rw-r--r--   0        0        0    12156 2023-04-17 17:51:32.509096 yog-2.1.5/yog/host/docker_attrs.py
--rw-r--r--   0        0        0      499 2023-02-22 04:11:12.414451 yog-2.1.5/yog/host/main.py
--rw-r--r--   0        0        0     7468 2023-04-17 17:46:06.818706 yog-2.1.5/yog/host/manage.py
--rw-r--r--   0        0        0     8557 2023-04-17 17:47:42.812155 yog-2.1.5/yog/host/necronomicon.py
--rw-r--r--   0        0        0    11317 2023-02-22 22:13:28.278626 yog-2.1.5/yog/host/pki.py
--rw-r--r--   0        0        0      492 2023-02-22 04:11:12.414451 yog-2.1.5/yog/host/pki_model.py
--rw-r--r--   0        0        0    11039 2023-02-01 20:50:54.524689 yog-2.1.5/yog/host/test_docker_attrs.py
--rw-r--r--   0        0        0      936 2023-02-22 04:11:12.414451 yog-2.1.5/yog/logging_utils.py
--rw-r--r--   0        0        0      389 2023-02-22 04:11:12.414451 yog-2.1.5/yog/model_utils.py
--rw-r--r--   0        0        0        0 2021-11-19 21:17:46.640293 yog-2.1.5/yog/repo/__init__.py
--rw-r--r--   0        0        0     4580 2022-12-28 04:50:30.284835 yog-2.1.5/yog/repo/main.py
--rw-r--r--   0        0        0      120 2021-07-25 01:26:53.898074 yog-2.1.5/yog/res/__init__.py
--rw-r--r--   0        0        0       80 2023-02-22 04:11:12.414451 yog-2.1.5/yog/res/cas.yml
--rw-r--r--   0        0        0      707 2023-02-01 20:50:54.524689 yog-2.1.5/yog/res/docker_test.yml
--rw-r--r--   0        0        0      434 2023-02-01 20:50:54.524689 yog-2.1.5/yog/res/sample_necronomicon.yml
--rw-r--r--   0        0        0      426 2021-07-30 04:19:50.436971 yog-2.1.5/yog/res/sample_needs_tunnel_back.yml
--rw-r--r--   0        0        0      185 2023-02-22 04:11:12.414451 yog-2.1.5/yog/res/sample_pki_necronomicon.yml
--rw-r--r--   0        0        0       50 2021-07-25 01:26:25.424796 yog-2.1.5/yog/res/sample_site_necronomicon.yml
--rw-r--r--   0        0        0    10283 2023-02-22 04:11:12.414451 yog-2.1.5/yog/ssh_utils.py
--rw-r--r--   0        0        0    11384 2023-04-18 02:34:17.535767 yog-2.1.5/setup.py
--rw-r--r--   0        0        0    10753 2023-04-18 02:34:17.536693 yog-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-02-25 02:02:07.903436 yog-2.1.6/README.md
+-rw-r--r--   0        0        0      541 2023-05-01 02:05:05.613161 yog-2.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-07-16 04:35:58.316463 yog-2.1.6/yog/__init__.py
+-rw-r--r--   0        0        0      465 2023-02-22 20:50:59.508191 yog-2.1.6/yog/command.py
+-rw-r--r--   0        0        0      636 2021-11-19 21:53:36.530661 yog-2.1.6/yog/git_utils.py
+-rw-r--r--   0        0        0        0 2021-11-19 21:18:00.056940 yog-2.1.6/yog/host/__init__.py
+-rw-r--r--   0        0        0    12156 2023-04-17 17:51:32.509096 yog-2.1.6/yog/host/docker_attrs.py
+-rw-r--r--   0        0        0      499 2023-02-22 04:11:12.414451 yog-2.1.6/yog/host/main.py
+-rw-r--r--   0        0        0     7453 2023-05-01 02:04:55.579539 yog-2.1.6/yog/host/manage.py
+-rw-r--r--   0        0        0     8557 2023-04-17 17:47:42.812155 yog-2.1.6/yog/host/necronomicon.py
+-rw-r--r--   0        0        0    11317 2023-02-22 22:13:28.278626 yog-2.1.6/yog/host/pki.py
+-rw-r--r--   0        0        0      492 2023-02-22 04:11:12.414451 yog-2.1.6/yog/host/pki_model.py
+-rw-r--r--   0        0        0    11039 2023-02-01 20:50:54.524689 yog-2.1.6/yog/host/test_docker_attrs.py
+-rw-r--r--   0        0        0      936 2023-02-22 04:11:12.414451 yog-2.1.6/yog/logging_utils.py
+-rw-r--r--   0        0        0      389 2023-02-22 04:11:12.414451 yog-2.1.6/yog/model_utils.py
+-rw-r--r--   0        0        0        0 2021-11-19 21:17:46.640293 yog-2.1.6/yog/repo/__init__.py
+-rw-r--r--   0        0        0     4580 2022-12-28 04:50:30.284835 yog-2.1.6/yog/repo/main.py
+-rw-r--r--   0        0        0      120 2021-07-25 01:26:53.898074 yog-2.1.6/yog/res/__init__.py
+-rw-r--r--   0        0        0       80 2023-02-22 04:11:12.414451 yog-2.1.6/yog/res/cas.yml
+-rw-r--r--   0        0        0      707 2023-02-01 20:50:54.524689 yog-2.1.6/yog/res/docker_test.yml
+-rw-r--r--   0        0        0      434 2023-02-01 20:50:54.524689 yog-2.1.6/yog/res/sample_necronomicon.yml
+-rw-r--r--   0        0        0      426 2021-07-30 04:19:50.436971 yog-2.1.6/yog/res/sample_needs_tunnel_back.yml
+-rw-r--r--   0        0        0      185 2023-02-22 04:11:12.414451 yog-2.1.6/yog/res/sample_pki_necronomicon.yml
+-rw-r--r--   0        0        0       50 2021-07-25 01:26:25.424796 yog-2.1.6/yog/res/sample_site_necronomicon.yml
+-rw-r--r--   0        0        0    10283 2023-02-22 04:11:12.414451 yog-2.1.6/yog/ssh_utils.py
+-rw-r--r--   0        0        0    11384 2023-05-01 02:06:23.207026 yog-2.1.6/setup.py
+-rw-r--r--   0        0        0    10753 2023-05-01 02:06:23.207974 yog-2.1.6/PKG-INFO
```

### Comparing `yog-2.1.5/README.md` & `yog-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `yog-2.1.5/pyproject.toml` & `yog-2.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yog"
-version = "2.1.5"
+version = "2.1.6"
 description = "The Gate and Key"
 authors = ["Josh Hertlein <jmhertlein@gmail.com>"]
 license = "AGPLv3"
 readme = "README.md"
 
 [tool.poetry.scripts]
 yog = "yog.host.main:main"
```

### Comparing `yog-2.1.5/yog/git_utils.py` & `yog-2.1.6/yog/git_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.1.5/yog/host/docker_attrs.py` & `yog-2.1.6/yog/host/docker_attrs.py`

 * *Files identical despite different names*

### Comparing `yog-2.1.5/yog/host/manage.py` & `yog-2.1.6/yog/host/manage.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,19 +71,19 @@
 def apply_cron_section(host: str, n: Necronomicon, ssh: SSHClient):
     cronfile_lines = []
     line1_length = max([len(c.expr) for c in n.cron.crons])
     line2_length = max([len(c.user) for c in n.cron.crons])
     for cron in n.cron.crons:
         cronfile_lines.append(f"{cron.expr.ljust(line1_length, ' ')}\t{cron.user.ljust(line2_length, ' ')}\t{cron.command}")
     cronfile_body = "\n".join(cronfile_lines + [""])
-    ok, expected, found = compare_local_and_remote(bytes(cronfile_body, "utf-8"), "/etc/cron.d/yog.cron", ssh)
+    ok, expected, found = compare_local_and_remote(bytes(cronfile_body, "utf-8"), "/etc/cron.d/yog", ssh)
     if not ok:
         log.info(f"[{host}][cron]: stale")
-        log.info(f"Writing /etc/cron.d/yog.cron version {expected[:10]}")
-        check_call(ssh, "sudo bash -c 'cat - > /etc/cron.d/yog.cron'", send_stdin=cronfile_body)
+        log.info(f"Writing /etc/cron.d/yog version {expected[:10]}")
+        check_call(ssh, "sudo bash -c 'cat - > /etc/cron.d/yog'", send_stdin=cronfile_body)
     else:
         log.info(f"[{host}][cron]: OK")
 
 
 def apply_docker_section(host: str, n: Necronomicon):
     log.debug(f"Docker: {n.ident}")
     tunnels = []
```

### Comparing `yog-2.1.5/yog/host/necronomicon.py` & `yog-2.1.6/yog/host/necronomicon.py`

 * *Files identical despite different names*

### Comparing `yog-2.1.5/yog/host/pki.py` & `yog-2.1.6/yog/host/pki.py`

 * *Files identical despite different names*

### Comparing `yog-2.1.5/yog/host/test_docker_attrs.py` & `yog-2.1.6/yog/host/test_docker_attrs.py`

 * *Files identical despite different names*

### Comparing `yog-2.1.5/yog/logging_utils.py` & `yog-2.1.6/yog/logging_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.1.5/yog/repo/main.py` & `yog-2.1.6/yog/repo/main.py`

 * *Files identical despite different names*

### Comparing `yog-2.1.5/yog/res/docker_test.yml` & `yog-2.1.6/yog/res/docker_test.yml`

 * *Files identical despite different names*

### Comparing `yog-2.1.5/yog/ssh_utils.py` & `yog-2.1.6/yog/ssh_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.1.5/setup.py` & `yog-2.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 entry_points = \
 {'console_scripts': ['yog = yog.host.main:main',
                      'yog-pki = yog.command:ca_main',
                      'yog-repo = yog.repo.main:main']}
 
 setup_kwargs = {
     'name': 'yog',
-    'version': '2.1.5',
+    'version': '2.1.6',
     'description': 'The Gate and Key',
     'long_description': '# Overview\n\nAn opinionated docker-and-ssh-centric declarative system management tool.\n\n`pip3 install yog`\n\nFeatures:\n\n* Like puppet or ansible but a lot smaller and focused on docker, files, and cron\n* agentless - runs entirely on top of ssh\n* entirely defers auth(z/n) to ssh and the remote system\'s user permissions\n\nNon-features:\n\n* No intentional ipv6 support. I don\'t have anything against IPv6, but my ISP doesn\'t give me a v6 address and as such I\n  don\'t run ipv6 on my lan. So since I can\'t test it at all, I just kind of disregard it, especially where it lets me\n  make the ipv4 UX better.\n\nCommand summary:\n\n* `yog`: Applies configurations to hosts. e.g. `yog myhost.mytld` applies the config from `./domains/mytld/myhost.yml`.\n* `yog-repo`: Manages a docker repository. `yog-repo push` uses the contents of `./yog-repo.conf` to build an image and\n  push it to the configured registry with the configured name and tag.\n\nExample run:\n\n[usage.webm](https://user-images.githubusercontent.com/1287152/209723654-e78b5283-60b5-4894-b5a1-3d2d71bfcc45.webm)\n\n# Setup\n\n1. Configure docker to listen on localhost\'s port 4243 (which is the default). See below.\n2. Use `ssh-copy-id` to copy your ssh key to all the servers you wish to manage. You can look into ssh certificates if\n   you want a more general ssh PKI solution.\n3. Configure the target system to allow you to use sudo without a password. [2]\n4. That\'s it. You now serve the nameless mist. Do you hear whippoorwills?\n\n## Docker port listening setup (step 1)\n\n```bash\nssh myhost\nsudo systemctl edit docker\n```\n\nAnd add `-H tcp://127.0.0.1:4243` to the command. So for me, that file looks like:\n\n```text\n[Service]\nExecStart=\nExecStart=/usr/bin/dockerd -H fd:// -H tcp://127.0.0.1:4243\n```\n\nYog will apply files before docker containers, so you might also want to add a yog file entry like so:\n\n```yaml\nfiles:\n  - src: docker-override.conf\n    dest: /etc/systemd/system/docker.service.d/override.conf\n    root: yes\n    hupcmd: sudo systemctl restart docker\n```\n\n# Usage\n\nYog uses YML files that it calls "necronomicons" for configuration of hosts. It\'s organized hierarchically so\nthat a necronomicon for "mytld" will be applied to all hosts under that TLD.\n\nLet\'s learn by example:\n\nSuppose we have a folder, that can be named whatever we want, at `~/projects/my-config`. This is the root of a\ngit repo, and is also the root of our yog configuration. Make this your current working dir, or pass `--root-dir`.\n\n`$ cd ~/projects/my-config`\n\n```text\n.\n├── domains\n│      ├── com\n│      │      └── example\n│      │          └── myhost.yml\n│      └── com.yml\n└── files\n    ├── example.txt\n    ├── hello_world.html\n    └── helloworld-nginx.conf\n\n4 directories, 5 files\n```\n\nFiles that can be sent to hosts are stored under `files`.\n\nHost configurations - necronomicons - are stored under `domains`.\n\nIf we want to apply `myhost.yml`, we run:\n\n`yog myhost.example.com`\n\nExample output:\n\n```text\n$ yog myhost.example.com\n[2022-12-26 11:01:52,514] [INFO]: [myhost.example.com]\n[2022-12-26 11:01:59,121] [INFO]: [myhost.example.com][files]: OK [hello_world.html]\n[2022-12-26 11:01:59,274] [INFO]: [myhost.example.com][files]: OK [helloworld-nginx.conf]\n[2022-12-26 11:02:07,117] [INFO]: [myhost.example.com][docker]: OK registry@sha256:8be26f81ffea54106bae012c6f349df70f4d5e7e2ec01b143c46e2c03b9e551d\n```\n\n## Necronomicon format\n\nLet\'s look at a necronomicon.\n\n```yml\nfiles:\n  - src: hello_world.html\n    dest: /srv/hello_world/hello_world.html\n    root: yes\n  - src: helloworld-nginx.conf\n    dest: /etc/nginx/conf.d/helloworld.conf\n    root: yes\n    hupcmd: sudo systemctl restart nginx\n\n\ndocker:\n  - image: registry\n    name: my-registry\n    fingerprint: sha256:8be26f81ffea54106bae012c6f349df70f4d5e7e2ec01b143c46e2c03b9e551d\n    volumes:\n      images: /var/lib/registry\n    ports:\n      - container: 5000\n        host: [ 5000 ]\n    env:\n      REGISTRY_STORAGE_DELETE_ENABLED: true\n\npki:\n  certs:\n    - authority: my-ca\n      storage: /srv/pki/myhost/\n      validity_years: 2\n      refresh_at: 1\n      names:\n        - myhost.local\n        - myapp.local\n```\n\n### Files\n\nFiles are checked for equality via hash-comparison. I\'ve found this a useful way to manage:\n\n* cron files in /etc/cron.d/\n* Root certificates to put in the system trust store[1]\n* random config files\n\nAttributes:\n\n* `src`: the source. This is a _relative_ path rooted at the `files` directory in the hierarchy. You can use\n  intermediate dirs.\n* `dest`: the destination filepath on the managed host. This is an absolute path.\n* `root`: whether to `sudo` to root for the file put. This mainly picks who owns the file + can access files, but this\n  might have other useful properties for your use case. If set to `no`, the put operation is run as your ssh user.\n* `hupcmd`: a command to run after the file is placed. A common thing in ye olde days was to send SIGHUP to a process\n  which would handle it by reloading the config. Commonly nowadays you might be\n  using `hupcmd: sudo systemctl reload nginx`\n\n### Docker containers\n\nDocker containers are compared on all specified attributes and won\'t unnecessarily restart containers.\n\nAttributes:\n\n* `image`: the docker repository name. e.g. `itzg/minecraft-server` or `dockerrepo.local:5000/mything`\n* `name`: the container name.\n* `fingerprint`: sha digest of the desired version. Tags are bad news bears so we don\'t support them. This is called\n  fingerprint instead of digest because I didn\'t know they were called digests when I first coded this and then never\n  changed it once I did.\n* `volumes`: volumes to attach. see below.\n* `ports`: ports to open. see below.\n* `env`: environment variables to set.\n\n#### Volumes\n\nFor volumes, the key is the volume name and the value is the mount point.\n\nFor bind mounts, the key is the host path and the value is the container path.\n\n#### Ports\n\nIt\'s a list of:\n\n```text\ncontainer: port/protocol\nhost: [interface_ip:port, interface_ip:port]\n```\n\nFor the container, you can omit the protocol to get tcp by default.\n\nFor the host, you can omit the interface ip to get `0.0.0.0` which binds all interfaces.\n\nExamples:\n\n```yml\n- container: 53/tcp\n  host: [ 192.168.1.103:53, 127.0.0.1:53 ]\n- container: 53/udp\n  host: [ 192.168.1.103:53, 127.0.0.1:53 ]\n- container: 33200 # tcp is implicit default, this is the same behavior as docker\n  host: [ 33200 ] # binds 0.0.0.0\n- container: 3000\n  host: [ 8080 ]\n```\n\n### Public Key Infrastructure (PKI)\n\nYog supports low-fuss local/private PKI management.\n\nYou\'ll define certificate authories in `cas.yml` which is in your yog root (so, right next to `domains` and `files`).\n\nExample `cas.yml`:\n\n```yaml\n- ident: my-ca\n  storage: "myhost.local:/srv/yog/ca/my-ca/"\n  validity_years: 3\n```\n\nAs you can see, yog tries to keep you out of the crypto weeds.\n\n`ident` is both how you\'ll refer to this CA in necronomicons, and also the X.509 Common Name.\n`storage` is a string of format `<host>:<path>` where the trust material will be stored. More on that below.\n`validity_years` is how long the cert will be valid for upon generation.\n\nOnce you\'ve defined `cas.yml`, you can run `yog-pki`.\n\n```text\n$ yog-pki\nGenerating new CA...\n```\n\nNow you can use it in necronomicons.\n\n```yaml\npki:\n  certs:\n    - authority: my-ca # this has to refer to an "ident" in cas.yml\n      storage: /srv/pki/myhost/\n      validity_years: 2\n      refresh_at: 1 # yog runs will only renew a cert once the remaining validity time is < this number of years\n      names:\n        - myhost.local # first entry becomes X.509 Common Name\n        - myapp.local # subsequent names are X.509 Alternative Names\n```\n\n#### Trust Material Formats and Storage\n\nWhen yog or yog-pki write trust material to disk, it will restrict read access for private material but allow it for\npublic.\n\nYog writes multiple formats to facilitate as many use-cases as possible with the same PKI:\n\n| Filename             | Format              | Encoding | Public/Private | Notes                 |\n|:---------------------|:--------------------|:---------|:--------------:|-----------------------|\n| key.pem.openssl      | Traditional OpenSSL | PEM      |    private     | good for nginx        |\n| key.ssh              | SSH                 | SSH      |    private     |                       |\n| key.pem.pkcs1.public | PEM                 | PKCS1    |     public     | java\'s JCE likes this |\n| key.ssh.public       | SSH                 | SSH      |     public     |                       |\n| key.crt              | X.509 Certificate   | PEM      |     public     | good for nginx        |\n\n#### Crypto Remarks\n\nYog tries to keep you out of the weeds and also to be a good, expressive, concise tool for what it considers itself good at.\n\nYou don\'t need to, and shouldn\'t want to, read this section. It is here to help reassure anyone who knows\ntoo much about cryptography and wants to know some details.\n\nYog-pki uses Python\'s Rust-based cryptography module and doesn\'t do anything clever at all (which is dangerous in crypto).\n\nIt uses elliptic-curve keys, and uses the NIST P-384 R1 curve (known as `SECP384R1` in python\'s cryptography module).\nThis is a 384-bit key, roughly equivalent to the hardness of a 7000-bit RSA key. \n\nIt uses CN and Alternative Names to set the "names" that certificates represent. \n\nNothing else is configurable. Small tweaks come in the future but generally speaking,\nI don\'t intend for yog-pki to handle huge, complicated PKIs. If you need to do so, \nyou might want to look at https://smallstep.com/. (You can use Yog\'s docker and file capabilities to\ndeploy a smallstep installation!)\n\n# Footnotes\n\n[1] This is one of those things where I feel like you probably shouldn\'t manage root certs like this but I have yet to\nregret it? It\'s not a cryptographic secret, so.\n\n[2] Also something that people say you probably shouldn\'t do but I\'ve yet to regret. If your user is in the docker group\nit\'s basically root anyway from a threat modeling perspective.\n\n# `yog-repo`\n\nYog also includes a tool for pushing images to your local docker registry. I haven\'t documented it yet, apologies. \n',
     'author': 'Josh Hertlein',
     'author_email': 'jmhertlein@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `yog-2.1.5/PKG-INFO` & `yog-2.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yog
-Version: 2.1.5
+Version: 2.1.6
 Summary: The Gate and Key
 License: AGPLv3
 Author: Josh Hertlein
 Author-email: jmhertlein@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

