# Comparing `tmp/oasees_sdk-0.2.1.tar.gz` & `tmp/oasees_sdk-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oasees_sdk-0.2.1.tar", max compression
+gzip compressed data, was "oasees_sdk-0.2.2.tar", max compression
```

## Comparing `oasees_sdk-0.2.1.tar` & `oasees_sdk-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0       10 2024-04-22 11:03:39.624851 oasees_sdk-0.2.1/README.md
--rw-r--r--   0        0        0      582 2024-04-25 11:42:26.463653 oasees_sdk-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    13812 2024-04-25 11:35:43.655512 oasees_sdk-0.2.1/src/oasees_sdk/cli/__pycache__/cli.cpython-310.pyc
--rw-r--r--   0        0        0    18067 2024-04-25 11:38:45.889519 oasees_sdk-0.2.1/src/oasees_sdk/cli/cli.py
--rw-r--r--   0        0        0       18 2024-04-19 14:55:41.703893 oasees_sdk-0.2.1/src/oasees_sdk/oasees_sdk/__init__.py
--rw-r--r--   0        0        0      170 2024-04-19 15:01:29.590771 oasees_sdk-0.2.1/src/oasees_sdk/oasees_sdk/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5636 2024-04-19 15:27:00.935485 oasees_sdk-0.2.1/src/oasees_sdk/oasees_sdk/__pycache__/sdk.cpython-310.pyc
--rw-r--r--   0        0        0     6368 2024-04-19 15:26:29.095703 oasees_sdk-0.2.1/src/oasees_sdk/oasees_sdk/sdk.py
--rw-r--r--   0        0        0     1015 1970-01-01 00:00:00.000000 oasees_sdk-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       10 2024-04-22 11:03:39.624851 oasees_sdk-0.2.2/README.md
+-rw-r--r--   0        0        0      619 2024-05-13 14:35:05.186648 oasees_sdk-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    20316 2024-05-13 14:33:09.171369 oasees_sdk-0.2.2/src/oasees_sdk/cli/cli.py
+-rw-r--r--   0        0        0       18 2024-05-10 14:31:20.743803 oasees_sdk-0.2.2/src/oasees_sdk/oasees_sdk/__init__.py
+-rw-r--r--   0        0        0      887 2024-05-10 14:31:20.755803 oasees_sdk-0.2.2/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py
+-rw-r--r--   0        0        0     1934 2024-05-10 14:31:20.699804 oasees_sdk-0.2.2/src/oasees_sdk/oasees_sdk/deploy_pipeline.py
+-rw-r--r--   0        0        0     9898 2024-05-13 14:33:13.795340 oasees_sdk-0.2.2/src/oasees_sdk/oasees_sdk/sdk.py
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 oasees_sdk-0.2.2/PKG-INFO
```

### Comparing `oasees_sdk-0.2.1/pyproject.toml` & `oasees_sdk-0.2.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "oasees_sdk"
-version = "0.2.1"
+version = "0.2.2"
 description = "Oasees SDK"
 authors = [
     "Example Author <author@example.com>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -19,11 +19,13 @@
 
 [tool.poetry.dependencies]
 Click="*"
 web3="*"
 ipfshttpclient="0.8.0a2"
 requests="*"
 python-dotenv="*"
+kubernetes="*"
+requests_toolbelt="*"
 
 
 [tool.poetry.plugins."console_scripts"]
 oasees-sdk = "oasees_sdk.cli.cli:cli"
```

### Comparing `oasees_sdk-0.2.1/src/oasees_sdk/cli/cli.py` & `oasees_sdk-0.2.2/src/oasees_sdk/cli/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import json
 import ipfshttpclient
 import requests
 import web3
 import socket
 import os
 from dotenv import load_dotenv
+import yaml
 
 
 @click.group(invoke_without_command=True)
 @click.pass_context
 def cli(ctx):
     if not ctx.invoked_subcommand:
         bash_script = r'''
@@ -85,22 +86,36 @@
 
         nft_contract = w3.eth.contract(address=nft_address, abi=nft_abi)
         marketplace_contract = w3.eth.contract(address=marketplace_address, abi=marketplace_abi)
 
         deployer_account = w3.to_checksum_address(config['ACCOUNT'])
         deployer_key = config['KEY']
 
+        mkdir_1 = subprocess.run(['sudo','mkdir','/etc/rancher'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+        mkdir_2 = subprocess.run(['sudo','mkdir','/etc/rancher/k3s'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+        echo = subprocess.run(['sudo','sh', '-c','echo "mirrors:\n  docker.io:\n  registry.k8s.io:" > /etc/rancher/k3s/registries.yaml'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
         curl = subprocess.Popen(['curl','-sfL', 'https://get.k3s.io'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
-        result = subprocess.check_output(['sh','-s','-','--write-kubeconfig-mode','644', '--write-kubeconfig', '/home/'+getpass.getuser()+'/.kube/config'], stdin=curl.stdout)
+        result = subprocess.check_output(['sh','-s','-','--write-kubeconfig-mode','644', '--write-kubeconfig', '/home/'+getpass.getuser()+'/.kube/config','--embedded-registry'], stdin=curl.stdout)
         click.echo(result)
         curl.wait()
         # Print the output of the 'ls' command
 
+        with open('/home/'+getpass.getuser()+'/.kube/config', 'r') as f:
+            cluster_config = yaml.safe_load(f)
+
+        result = subprocess.run(['kubectl','get','nodes','-o','custom-columns=IP:.status.addresses[].address','--no-headers'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+        ip = result.stdout.strip().split('\n')
+
+
+        cluster_config['clusters'][0]['cluster']['server'] = "https://{}:6443".format(ip[0])
+
         client = ipfshttpclient.connect("/ip4/{}/tcp/5001".format(config['IPFS_IP']))
-        cluster_config_hash = client.add_json({"test": "test string"})
+        cluster_config_hash = client.add_json(cluster_config)
+        click.echo(cluster_config_hash)
+
 
         transaction = nft_contract.functions.mint(cluster_config_hash).build_transaction({
 		'chainId': 31337,
 		'gas': 2000000,
 		'gasPrice': w3.eth.gas_price,
 		'nonce': w3.eth.get_transaction_count(deployer_account) + 0
 	    })
@@ -182,14 +197,17 @@
 
 @cli.command()
 @click.option('--ip', required=True, help="The cluster's master ip address.")
 @click.option('--token', required=True, help="The cluster's master token.")
 def join_cluster(ip,token):
     '''Joins the current machine to the specified cluster.'''
     try:
+        mkdir_1 = subprocess.run(['sudo','mkdir','/etc/rancher'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+        mkdir_2 = subprocess.run(['sudo','mkdir','/etc/rancher/k3s'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+        echo = subprocess.run(['sudo','sh', '-c','echo "mirrors:\n  docker.io:\n  registry.k8s.io:" > /etc/rancher/k3s/registries.yaml'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
         curl = subprocess.Popen(['curl','-sfL', 'https://get.k3s.io'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
         result = subprocess.check_output(['sh','-'], env={'K3S_URL' : 'https://'+ip+':6443', 'K3S_TOKEN': token}, stdin=curl.stdout)
         click.echo(result)
         curl.wait()
     except FileNotFoundError:
         click.echo("Error: K3S cluster could not be joined.\n")
             
@@ -408,9 +426,18 @@
         if(changed):
             with open('/home/'+getpass.getuser()+'/config.json', 'w') as f:
                 json.dump(config,f)
 
     except FileNotFoundError:
         click.echo("Error: config file not found.")
     
+@cli.command()
+def new_cluster():
+    mkdir_1 = subprocess.run(['sudo','mkdir','/etc/rancher'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+    mkdir_2 = subprocess.run(['sudo','mkdir','/etc/rancher/k3s'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+    echo = subprocess.run(['sudo','sh', '-c','echo "mirrors:\n  docker.io:\n  registry.k8s.io:" > /etc/rancher/k3s/registries.yaml'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+    curl = subprocess.Popen(['curl','-sfL', 'https://get.k3s.io'], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+    result = subprocess.check_output(['sh','-s','-','--write-kubeconfig-mode','644', '--write-kubeconfig', '/home/'+getpass.getuser()+'/.kube/config','--embedded-registry'], stdin=curl.stdout)
+    click.echo(result)
+    curl.wait()
 
 config_exists()
```

### Comparing `oasees_sdk-0.2.1/PKG-INFO` & `oasees_sdk-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oasees_sdk
-Version: 0.2.1
+Version: 0.2.2
 Summary: Oasees SDK
 Author: Example Author
 Author-email: author@example.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -16,13 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Click
 Requires-Dist: ipfshttpclient (==0.8.0a2)
+Requires-Dist: kubernetes
 Requires-Dist: python-dotenv
 Requires-Dist: requests
+Requires-Dist: requests_toolbelt
 Requires-Dist: web3
 Description-Content-Type: text/markdown
 
 OASEES SDK
```

