# Comparing `tmp/veda_cli-0.0.3.tar.gz` & `tmp/veda_cli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veda_cli-0.0.3.tar", max compression
+gzip compressed data, was "veda_cli-0.0.4.tar", max compression
```

## Comparing `veda_cli-0.0.3.tar` & `veda_cli-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,12 @@
--rw-r--r--   0        0        0       72 2023-03-12 06:19:04.046534 veda_cli-0.0.3/README.md
--rw-r--r--   0        0        0     1309 2023-03-16 19:16:55.004510 veda_cli-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-12 04:30:35.194796 veda_cli-0.0.3/veda_cli/__init__.py
--rw-r--r--   0        0        0      915 2023-03-12 07:04:38.648016 veda_cli-0.0.3/veda_cli/applications/__init__.py
--rw-r--r--   0        0        0     1296 2023-03-13 06:26:16.030894 veda_cli-0.0.3/veda_cli/applications/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1063 2023-03-12 14:37:50.430269 veda_cli-0.0.3/veda_cli/applications/ecco/__init__.py
--rw-r--r--   0        0        0     1146 2023-03-13 06:26:16.035198 veda_cli-0.0.3/veda_cli/applications/ecco/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7744 2023-03-16 19:17:02.370085 veda_cli-0.0.3/veda_cli/applications/ecco/__pycache__/ecco_app.cpython-310.pyc
--rw-r--r--   0        0        0    10910 2023-03-16 19:16:33.662515 veda_cli-0.0.3/veda_cli/applications/ecco/ecco_app.py
--rw-r--r--   0        0        0        0 2023-03-12 05:07:59.351295 veda_cli-0.0.3/veda_cli/applications/wrf/__init__.py
--rw-r--r--   0        0        0      515 2023-03-12 07:06:20.230878 veda_cli-0.0.3/veda_cli/datasets/__init__.py
--rw-r--r--   0        0        0      822 2023-03-12 07:07:43.066401 veda_cli-0.0.3/veda_cli/datasets/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1972 2023-03-16 19:17:35.747378 veda_cli-0.0.3/veda_cli/executions/__init__.py
--rw-r--r--   0        0        0     2003 2023-03-13 07:47:45.558601 veda_cli-0.0.3/veda_cli/executions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1113 2023-03-13 07:17:41.103900 veda_cli-0.0.3/veda_cli/main.py
--rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 veda_cli-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-03-12 06:19:04.046534 veda_cli-0.0.4/README.md
+-rw-r--r--   0        0        0     1664 2023-05-01 10:06:45.994331 veda_cli-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-12 04:30:35.194796 veda_cli-0.0.4/veda_cli/__init__.py
+-rw-r--r--   0        0        0      915 2023-05-01 02:28:32.474565 veda_cli-0.0.4/veda_cli/applications/__init__.py
+-rw-r--r--   0        0        0     1148 2023-05-01 05:41:01.645101 veda_cli-0.0.4/veda_cli/applications/ecco/__init__.py
+-rw-r--r--   0        0        0    13066 2023-05-01 10:04:03.508678 veda_cli-0.0.4/veda_cli/applications/ecco/ecco_app.py
+-rw-r--r--   0        0        0        0 2023-03-12 05:07:59.351295 veda_cli-0.0.4/veda_cli/applications/wrf/__init__.py
+-rw-r--r--   0        0        0     1997 2023-05-01 10:03:35.491931 veda_cli-0.0.4/veda_cli/datasets/__init__.py
+-rw-r--r--   0        0        0     2070 2023-05-01 10:04:58.155027 veda_cli-0.0.4/veda_cli/executions/__init__.py
+-rw-r--r--   0        0        0     1002 2023-05-01 10:06:18.881461 veda_cli-0.0.4/veda_cli/executions/ouput.py
+-rw-r--r--   0        0        0     1204 2023-05-01 08:52:05.066412 veda_cli-0.0.4/veda_cli/main.py
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 veda_cli-0.0.4/PKG-INFO
```

### Comparing `veda_cli-0.0.3/pyproject.toml` & `veda_cli-0.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -14,26 +14,30 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 [tool.poetry]
 name = "veda-cli"
-version = "0.0.3"
+version = "0.0.4"
 description = "Command Line Client NASA VEDA Analytics"
 authors = ["Dimuthu Wannipurage <dwannipu@iu.edu>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 veda = "veda_cli.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = {extras = ["all"], version = "^0.7.0"}
 pick = {version= "2.2.0"}
 boto3 = {version= "^1.26.0"}
 paramiko = {version= "^3.0.0"}
 pysondb = {version= "^1.6.6"}
+grpcio= [{version="1.46.3", markers = "platform_machine != 'arm64'"},{version="1.47.0rc1", markers = "platform_machine == 'arm64'"}]
+grpcio-tools = [{version="1.46.3", markers = "platform_machine != 'arm64'"},{version="1.47.0rc1", markers = "platform_machine == 'arm64'"}]
+airavata_mft_sdk= {version="0.0.1-alpha27"}
+airavata-mft-cli = {version="0.1.10"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `veda_cli-0.0.3/veda_cli/applications/__init__.py` & `veda_cli-0.0.4/veda_cli/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `veda_cli-0.0.3/veda_cli/applications/ecco/__init__.py` & `veda_cli-0.0.4/veda_cli/applications/ecco/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,27 +6,29 @@
 def run_ecco():
     options = ["Amazon EC2", "Jetstream 2" ]
     server_option, index = pick(options, "Where Do you want to run ECCO Application?", indicator="=>")
 
     options = ['ECCO-NASA-V4 : NASA Hosted ECCO V4 Dataset', 'Custom']
     option, index = pick(options, "Which dataset do you want to use?", indicator="=>")
 
+    execution_name = typer.prompt("Execution Name")
+
     customize = typer.confirm("Do want to customize model parameters?", True)
 
     ecco_configs = {}
     if customize:
         ecco_configs['time_step'] = typer.prompt("Time Step (S)", 3600) 
         ecco_configs['total_time_steps'] = typer.prompt("Total Time (S)", 227903) 
         ecco_configs['gravity'] = typer.prompt("Gravity", 9.81)
         ecco_configs['rhonil']=typer.prompt("Rhonil", 1029)
 
     if server_option == 'Amazon EC2':
-        ecco_app.run_ecco_on_ec2(ecco_configs)
+        ecco_app.run_ecco_on_ec2(execution_name, ecco_configs)
     elif server_option == 'Jetstream 2':
-        ecco_app.run_ecco_on_jetstream2(ecco_configs)
+        ecco_app.run_ecco_on_jetstream2(execution_name, ecco_configs)
     else:
         print("Error: Unknow server selection")
```

### Comparing `veda_cli-0.0.3/veda_cli/applications/ecco/ecco_app.py` & `veda_cli-0.0.4/veda_cli/applications/ecco/ecco_app.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,19 +7,51 @@
 import paramiko
 import socket
 import time
 import typer
 from pysondb import db
 from datetime import datetime
 from rich import print
-
+from airavata_mft_cli import config as configcli
+from airavata_mft_sdk import mft_client
+from airavata_mft_sdk.scp import SCPCredential_pb2
+from airavata_mft_sdk.scp import SCPStorage_pb2
+from airavata_mft_sdk.common import StorageCommon_pb2
 
 def get_db():
     return db.getDb(os.path.join(os.path.expanduser('~'), ".veda", "db.json"))
 
+def register_execution_endpoint(storage_name, private_key, user_name, host_name, port):
+    client = mft_client.MFTClient(transfer_api_port = configcli.transfer_api_port,
+                                    transfer_api_secured = configcli.transfer_api_secured,
+                                    resource_service_host = configcli.resource_service_host,
+                                    resource_service_port = configcli.resource_service_port,
+                                    resource_service_secured = configcli.resource_service_secured,
+                                    secret_service_host = configcli.secret_service_host,
+                                    secret_service_port = configcli.secret_service_port)
+    
+    secret_create_req = SCPCredential_pb2.SCPSecretCreateRequest(privateKey=private_key, 
+                                                                 user=user_name)
+    created_secret = client.scp_secret_api.createSCPSecret(secret_create_req)
+
+    scp_storage_create_req = SCPStorage_pb2.SCPStorageCreateRequest(
+        host=host_name, port=port, name=storage_name)
+    
+    created_storage = client.scp_storage_api.createSCPStorage(scp_storage_create_req)
+
+    secret_for_storage_req = StorageCommon_pb2.SecretForStorage(storageId = created_storage.storageId,
+                                       secretId = created_secret.secretId,
+                                       storageType = StorageCommon_pb2.StorageType.SCP)
+
+    client.common_api.registerSecretForStorage(secret_for_storage_req)
+
+    return created_storage.storageId
+
+
+    
 def describe_vpcs(tag, tag_values, max_items, ec2_client):
     """
     Describes one or more VPCs.
     """
     try:
         # creating paginator object for describe_vpcs() method
         paginator = ec2_client.get_paginator('describe_vpcs')
@@ -116,24 +148,24 @@
     if not os.path.exists(veda_aws_credentials):
         os.makedirs(veda_aws_credentials)
 
     veda_ssh_credentials = os.path.join(os.path.expanduser('~'), ".veda", "credentials", "ssh")
     if not os.path.exists(veda_ssh_credentials):
         os.makedirs(veda_ssh_credentials)
     
-def run_ecco_on_ec2(ecco_configs):
+def run_ecco_on_ec2(execution_name, ecco_configs):
     print("Running the ECCO simulation on EC2")
 
     init_local()
 
     access_key = typer.prompt("AWS Access Key Id", hide_input=True)
     secret_key = typer.prompt("AWS Secret Access Key", hide_input=True)
 
     region = "us-west-2"
-    ecco_ami = 'ami-02cf064456f5c84f7'
+    ecco_ami = 'ami-01b3a8d8f90f3fd3c'
     instance_size = 'c5.24xlarge'
     vpc_name = 'veda_ecco_vpc'
     security_group_name = 'veda_ecco_sg'
     subnet_name = 'veda_ecco_subnet'
     route_table_name = 'veda_ecco_rt'
     internet_gateway_name = 'veda_ecco_ig'
     instance_name = 'VEDA ECCO Run'
@@ -278,30 +310,38 @@
     local_key_file = os.path.join(os.path.expanduser('~'), ".veda", "credentials", "ssh", key_name)
     print('[bold red]ssh -i ' + local_key_file + ' ubuntu@' + public_ip + '[/bold red]')
     ssh = create_ssh_connection('ubuntu', public_ip, local_key_file)
 
     ssh_stdin, ssh_stdout, ssh_stderr = ssh.exec_command("cd /home/ubuntu/MITgcm/ECCOV4/release4/run; nohup mpirun -np 96 ./mitgcmuv >> mpi.out 2>&1 &")
     stdout = ssh_stdout.readlines()
 
+    with open(local_key_file, 'r') as key_file:
+        private_key = key_file.read()
+
+    storage_id = register_execution_endpoint(execution_name + " storage",  private_key, "ubuntu", public_ip, 22)
+
     execution_id = ''.join(random.choices(string.ascii_lowercase + string.digits, k=5))
     db_conn = get_db()
     db_conn.add({
         "type": "Execution", 
         "runtime": "EC2", 
         "application": "ECCO", 
         "executionId": execution_id, 
         "createdTime": datetime.now().strftime("%m/%d/%Y, %H:%M:%S"),
         "instanceId": instance_id,
         "publicIp": public_ip,
         "loginUser": "ubuntu",
         "accessKey":access_key,
         "secretKey": secret_key,
         "region": region,
-        "keyPath": local_key_file})
+        "keyPath": local_key_file,
+        "storageId": storage_id,
+        "outputDir": "/home/ubuntu/MITgcm/ECCOV4/release4/run/diags"})
 
     print("[bold blue]Started the ECCO Model run. Execution Id: " + execution_id + "[/bold blue]")
 
-def run_ecco_on_jetstream2(ecco_configs):
+
+def run_ecco_on_jetstream2(execution_name, ecco_configs):
     print("Running the ECCO simulation on Jetstream 2")
     print("This is not yet supported...")
```

### Comparing `veda_cli-0.0.3/veda_cli/executions/__init__.py` & `veda_cli-0.0.4/veda_cli/executions/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import typer
 from rich.table import Table
 from rich.console import Console
 from pysondb import db
 import os
 from rich import print
 import boto3
+import veda_cli.executions.ouput as op
 
 
 app = typer.Typer()
 
+app.add_typer(op.app, name="output")
+
 def get_db():
     return db.getDb(os.path.join(os.path.expanduser('~'), ".veda", "db.json"))
 
 @app.command("list")
-def list():
+def list_executions():
     console = Console()
     table = Table()
 
     table.add_column('Execution Id', justify='left')
     table.add_column('Application', justify='left')
     table.add_column('Runtime', justify='left')
     table.add_column('Created Time', justify='left')
@@ -27,15 +30,15 @@
 
     for execution in executions:
         table.add_row(execution['executionId'], execution['application'], execution['runtime'], execution['createdTime'])
 
     console.print(table)
 
 @app.command("info")
-def info(executionid: str):
+def execution_info(executionid: str):
     db_conn = get_db()
     executions = db_conn.getBy({"type":"Execution", "executionId": executionid})
     print(executions)
 
 @app.command("kill")
 def kill_execution(executionid):
     db_conn = get_db()
```

### Comparing `veda_cli-0.0.3/veda_cli/main.py` & `veda_cli-0.0.4/veda_cli/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 # specific language governing permissions and limitations
 # under the License.
 #
 import typer
 import veda_cli.applications
 import veda_cli.datasets
 import veda_cli.executions
+import airavata_mft_cli.storage
 
 app = typer.Typer()
 app.add_typer(veda_cli.applications.app, name="application")
 app.add_typer(veda_cli.datasets.app, name="dataset")
 app.add_typer(veda_cli.executions.app, name="execution")
-
+app.add_typer(airavata_mft_cli.storage.app, name="storage")
 
 if __name__ == "__main__":
     app()
```

