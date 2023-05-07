# Comparing `tmp/ec2-manager-0.0.8.tar.gz` & `tmp/ec2-manager-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ec2-manager-0.0.8.tar", last modified: Thu Aug 25 01:20:54 2022, max compression
+gzip compressed data, was "ec2-manager-0.0.9.tar", last modified: Mon Aug 29 23:56:28 2022, max compression
```

## Comparing `ec2-manager-0.0.8.tar` & `ec2-manager-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 01:20:54.000203 ec2-manager-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     3024 2022-08-25 01:20:54.000203 ec2-manager-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2593 2022-08-25 01:20:37.000000 ec2-manager-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-08-25 01:20:37.000000 ec2-manager-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      889 2022-08-25 01:20:54.004203 ec2-manager-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 01:20:53.996203 ec2-manager-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 01:20:53.996203 ec2-manager-0.0.8/src/ec2_manager/
--rw-r--r--   0 runner    (1001) docker     (121)    17891 2022-08-25 01:20:37.000000 ec2-manager-0.0.8/src/ec2_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5374 2022-08-25 01:20:37.000000 ec2-manager-0.0.8/src/ec2_manager/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 01:20:54.000203 ec2-manager-0.0.8/src/ec2_manager/template/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-25 01:20:37.000000 ec2-manager-0.0.8/src/ec2_manager/template/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 01:20:53.996203 ec2-manager-0.0.8/src/ec2_manager/template/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 01:20:54.000203 ec2-manager-0.0.8/src/ec2_manager/template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-08-25 01:20:37.000000 ec2-manager-0.0.8/src/ec2_manager/template/.github/workflows/deploy.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-08-25 01:20:37.000000 ec2-manager-0.0.8/src/ec2_manager/template/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 01:20:54.000203 ec2-manager-0.0.8/src/ec2_manager/template/compose/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-25 01:20:37.000000 ec2-manager-0.0.8/src/ec2_manager/template/compose/docker-compose.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      963 2022-08-25 01:20:37.000000 ec2-manager-0.0.8/src/ec2_manager/template/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 01:20:54.000203 ec2-manager-0.0.8/src/ec2_manager/template/terraform/
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-08-25 01:20:37.000000 ec2-manager-0.0.8/src/ec2_manager/template/terraform/data.tf
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-08-25 01:20:37.000000 ec2-manager-0.0.8/src/ec2_manager/template/terraform/outputs.tf
--rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-08-25 01:20:37.000000 ec2-manager-0.0.8/src/ec2_manager/template/terraform/permissions.tf
--rw-r--r--   0 runner    (1001) docker     (121)      390 2022-08-25 01:20:37.000000 ec2-manager-0.0.8/src/ec2_manager/template/terraform/provider.tf
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-08-25 01:20:37.000000 ec2-manager-0.0.8/src/ec2_manager/template/terraform/resources.tf
--rw-r--r--   0 runner    (1001) docker     (121)     1922 2022-08-25 01:20:37.000000 ec2-manager-0.0.8/src/ec2_manager/template/terraform/user_data.sh.tpl
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-08-25 01:20:37.000000 ec2-manager-0.0.8/src/ec2_manager/template/terraform/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 01:20:54.000203 ec2-manager-0.0.8/src/ec2_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3024 2022-08-25 01:20:53.000000 ec2-manager-0.0.8/src/ec2_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      875 2022-08-25 01:20:53.000000 ec2-manager-0.0.8/src/ec2_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-25 01:20:53.000000 ec2-manager-0.0.8/src/ec2_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-08-25 01:20:53.000000 ec2-manager-0.0.8/src/ec2_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-08-25 01:20:53.000000 ec2-manager-0.0.8/src/ec2_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-25 01:20:53.000000 ec2-manager-0.0.8/src/ec2_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 23:56:28.472782 ec2-manager-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     3024 2022-08-29 23:56:28.472782 ec2-manager-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2593 2022-08-29 23:56:16.000000 ec2-manager-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      115 2022-08-29 23:56:16.000000 ec2-manager-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      889 2022-08-29 23:56:28.472782 ec2-manager-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 23:56:28.468782 ec2-manager-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 23:56:28.468782 ec2-manager-0.0.9/src/ec2_manager/
+-rw-r--r--   0 runner    (1001) docker     (121)    18036 2022-08-29 23:56:16.000000 ec2-manager-0.0.9/src/ec2_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5374 2022-08-29 23:56:16.000000 ec2-manager-0.0.9/src/ec2_manager/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 23:56:28.468782 ec2-manager-0.0.9/src/ec2_manager/template/
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-29 23:56:16.000000 ec2-manager-0.0.9/src/ec2_manager/template/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 23:56:28.468782 ec2-manager-0.0.9/src/ec2_manager/template/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 23:56:28.468782 ec2-manager-0.0.9/src/ec2_manager/template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-08-29 23:56:16.000000 ec2-manager-0.0.9/src/ec2_manager/template/.github/workflows/deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-08-29 23:56:16.000000 ec2-manager-0.0.9/src/ec2_manager/template/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 23:56:28.468782 ec2-manager-0.0.9/src/ec2_manager/template/compose/
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-29 23:56:16.000000 ec2-manager-0.0.9/src/ec2_manager/template/compose/docker-compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      963 2022-08-29 23:56:16.000000 ec2-manager-0.0.9/src/ec2_manager/template/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 23:56:28.472782 ec2-manager-0.0.9/src/ec2_manager/template/terraform/
+-rw-r--r--   0 runner    (1001) docker     (121)      775 2022-08-29 23:56:16.000000 ec2-manager-0.0.9/src/ec2_manager/template/terraform/data.tf
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-08-29 23:56:16.000000 ec2-manager-0.0.9/src/ec2_manager/template/terraform/outputs.tf
+-rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-08-29 23:56:16.000000 ec2-manager-0.0.9/src/ec2_manager/template/terraform/permissions.tf
+-rw-r--r--   0 runner    (1001) docker     (121)      390 2022-08-29 23:56:16.000000 ec2-manager-0.0.9/src/ec2_manager/template/terraform/provider.tf
+-rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-08-29 23:56:16.000000 ec2-manager-0.0.9/src/ec2_manager/template/terraform/resources.tf
+-rw-r--r--   0 runner    (1001) docker     (121)     1922 2022-08-29 23:56:16.000000 ec2-manager-0.0.9/src/ec2_manager/template/terraform/user_data.sh.tpl
+-rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-08-29 23:56:16.000000 ec2-manager-0.0.9/src/ec2_manager/template/terraform/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-29 23:56:28.468782 ec2-manager-0.0.9/src/ec2_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3024 2022-08-29 23:56:28.000000 ec2-manager-0.0.9/src/ec2_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      875 2022-08-29 23:56:28.000000 ec2-manager-0.0.9/src/ec2_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-29 23:56:28.000000 ec2-manager-0.0.9/src/ec2_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-08-29 23:56:28.000000 ec2-manager-0.0.9/src/ec2_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-08-29 23:56:28.000000 ec2-manager-0.0.9/src/ec2_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-29 23:56:28.000000 ec2-manager-0.0.9/src/ec2_manager.egg-info/top_level.txt
```

### Comparing `ec2-manager-0.0.8/PKG-INFO` & `ec2-manager-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ec2-manager
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/jamesbaber1/ec2-manager
 Author: jamesbaber1
 Author-email: 
 Project-URL: Bug Tracker, https://github.com/jamesbaber1/ec2-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ec2-manager-0.0.8/README.md` & `ec2-manager-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ec2-manager-0.0.8/setup.cfg` & `ec2-manager-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ec2-manager
-version = 0.0.8
+version = 0.0.9
 author = jamesbaber1
 author_email = 
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jamesbaber1/ec2-manager
 project_urls =
```

### Comparing `ec2-manager-0.0.8/src/ec2_manager/__init__.py` & `ec2-manager-0.0.9/src/ec2_manager/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 import base64
 import boto3
 import logging
 import subprocess
 import json
 import yaml
 import shutil
-from pprint import pprint
 from datetime import datetime
 from github import Github
 from botocore.exceptions import WaiterError
-
 logging.basicConfig(level=logging.INFO)
 
 
 class EC2Manager:
     def __init__(self, **kwargs):
         # needed envs
         self._repo = os.environ.get('REPO', kwargs.get('repo'))
@@ -34,14 +32,17 @@
         self._repo_url = (
             f'https://{self._github_user}:{self._github_token}@github.com/{self._github_user}/{self._repo}.git'
         )
         self._max_attempts = int(os.environ.get('MAX_TIMEOUT', 600))
 
         self._github_client = Github(self._github_token)
 
+        self._logger = logging.getLogger(self.__class__.__name__)
+        self._logger.setLevel(level=logging.INFO)
+
         # only when initialize with a config
         if self._config_file:
             # internal variables
             self._config = self._get_config()
             self._aws_default_region = self._config['aws_region']
             self._type = self._config['type']
             self._vpc_name = self._config['vpc_name']
@@ -119,15 +120,15 @@
         :param str name: The name of the bot.
         :param bool name: Whether to make one attempt to get the instance id.
         :param int attempts: The number of attempts made to get the instance id.
         :returns: Instance id.
         :rtype: str
         """
         if not try_once:
-            logging.info(f"{name} has been trying to get its instance id for {attempts} secs...")
+            self._logger.info(f"{name} has been trying to get its instance id for {attempts} secs...")
         instance_id = self.list_instances().get(name, {}).get('instance_id')
         if not instance_id and attempts < self._max_attempts and not try_once:
             time.sleep(5)
             instance_id = self._get_instance_id(name, try_once, attempts + 5)
         return instance_id
 
     def _get_terraform_outputs(self):
@@ -208,45 +209,45 @@
     def _status_check(self, name, status):
         """
         Check for the given status on the ec2 instance by id.
 
         :param str name: The name of the bot.
         :param str status: The name of the ec2 instance status check to wait for.
         """
-        logging.info(f"{name} instance {self._instance_id} is checking if its status is {status.split('_')[-1]}")
+        self._logger.info(f"{name} instance {self._instance_id} is checking if its status is {status.split('_')[-1]}")
         if self._instance_id:
             try:
                 waiter = self._ec2_client.get_waiter(status)
                 waiter.wait(InstanceIds=[self._instance_id])
-                logging.info(f"{name} instance {self._instance_id} is {status.split('_')[-1]}")
+                self._logger.info(f"{name} instance {self._instance_id} is {status.split('_')[-1]}")
             except WaiterError:
                 logging.error(f"{name} status check of instance {self._instance_id} failed")
         else:
-            logging.info(f"{name} instance does not exist")
+            self._logger.info(f"{name} instance does not exist")
 
     def _create_backend_bucket(self):
         """
         Creates terraform backend bucket if it doesn't exist.
         """
         buckets = [item['Name'] for item in self._s3_client.list_buckets().get('Buckets', [])]
         if self._aws_backend_bucket not in buckets:
-            logging.info(f'Creating Terraform backend...')
+            self._logger.info(f'Creating Terraform backend...')
             self._s3_client.create_bucket(
                 ACL='private',
                 Bucket=self._aws_backend_bucket
             )
             waiter = self._s3_client.get_waiter('bucket_exists')
             waiter.wait(Bucket=self._aws_backend_bucket)
 
     def _init_terraform(self):
         """
         Runs terraform init.
         """
         self._create_backend_bucket()
-        logging.info(f'Initializing Terraform backend...')
+        self._logger.info(f'Initializing Terraform backend...')
         process = subprocess.run(
             [
                 'terraform',
                 'init',
                 f'-backend-config="key={self._type}.tfstate"',
                 f'-backend-config="bucket={self._aws_backend_bucket}"'
             ],
@@ -258,15 +259,15 @@
 
     def _apply_terraform(self):
         """
         Runs terraform apply that creates the ec2 instances.
         """
         outputs = self._get_terraform_outputs()
         if outputs.get('instance_names', {}).get('value') != self._instance_names:
-            logging.info(f'Terraform instances...')
+            self._logger.info(f'Terraform instances...')
             instances = self.encode_string(json.dumps(self._get_instance_data()))
 
             process = subprocess.run(
                 [
                     'terraform',
                     'apply',
                     '-auto-approve',
@@ -394,18 +395,18 @@
 
     def update_repos(self):
         """
         Updates the code in the instance repos.
         """
         for name in self._instance_repo_updates:
             if self._repo not in self.run_command(name, ['ls'], print_output=False):
-                logging.info(f'{name} cloning {self._repo}')
+                self._logger.info(f'{name} cloning {self._repo}')
                 self.run_command(name, [f'git clone {self._repo_url}'])
 
-            logging.info(f'{name} checking out {self._commit}')
+            self._logger.info(f'{name} checking out {self._commit}')
             self.run_command(name, [
                 f'cd ./{self._repo}',
                 'git fetch',
                 f'git checkout {self._commit}',
                 'git pull',
             ])
 
@@ -414,27 +415,27 @@
         Runs stop if a docker container is already running.
         """
         for name, data in self._get_instance_data().items():
             # check if docker is already running
             result = list(filter(None, self.run_command(name, ['docker ps'], print_output=False).split('\n')))
             if len(result) > 1:
                 # then compose down
-                logging.info(f'{name} stopping...')
+                self._logger.info(f'{name} stopping...')
                 working_directory = self._get_working_directory(data['working_directory'])
                 self.run_command(name, [
                     f'cd {working_directory} ',
                     data['commands']['stop']
                 ])
 
     def start(self):
         """
         Runs start command on the instances.
         """
         for name, data in self._get_instance_data().items():
-            logging.info(f'{name} starting...')
+            self._logger.info(f'{name} starting...')
             working_directory = self._get_working_directory(data['working_directory'])
             self.run_command(name, [
                 f'cd {working_directory} ',
                 *[f'export {key}={value}' for key, value in data['envs'].items()],
                 data['commands']['start'],
                 *[f'unset {key}' for key in data['envs'].keys()]
             ])
```

### Comparing `ec2-manager-0.0.8/src/ec2_manager/cli.py` & `ec2-manager-0.0.9/src/ec2_manager/cli.py`

 * *Files identical despite different names*

### Comparing `ec2-manager-0.0.8/src/ec2_manager/template/.github/workflows/deploy.yaml` & `ec2-manager-0.0.9/src/ec2_manager/template/.github/workflows/deploy.yaml`

 * *Files identical despite different names*

### Comparing `ec2-manager-0.0.8/src/ec2_manager/template/config.yaml` & `ec2-manager-0.0.9/src/ec2_manager/template/config.yaml`

 * *Files identical despite different names*

### Comparing `ec2-manager-0.0.8/src/ec2_manager/template/terraform/data.tf` & `ec2-manager-0.0.9/src/ec2_manager/template/terraform/data.tf`

 * *Files identical despite different names*

### Comparing `ec2-manager-0.0.8/src/ec2_manager/template/terraform/permissions.tf` & `ec2-manager-0.0.9/src/ec2_manager/template/terraform/permissions.tf`

 * *Files identical despite different names*

### Comparing `ec2-manager-0.0.8/src/ec2_manager/template/terraform/resources.tf` & `ec2-manager-0.0.9/src/ec2_manager/template/terraform/resources.tf`

 * *Files identical despite different names*

### Comparing `ec2-manager-0.0.8/src/ec2_manager/template/terraform/user_data.sh.tpl` & `ec2-manager-0.0.9/src/ec2_manager/template/terraform/user_data.sh.tpl`

 * *Files identical despite different names*

### Comparing `ec2-manager-0.0.8/src/ec2_manager/template/terraform/variables.tf` & `ec2-manager-0.0.9/src/ec2_manager/template/terraform/variables.tf`

 * *Files identical despite different names*

### Comparing `ec2-manager-0.0.8/src/ec2_manager.egg-info/PKG-INFO` & `ec2-manager-0.0.9/src/ec2_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ec2-manager
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/jamesbaber1/ec2-manager
 Author: jamesbaber1
 Author-email: 
 Project-URL: Bug Tracker, https://github.com/jamesbaber1/ec2-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ec2-manager-0.0.8/src/ec2_manager.egg-info/SOURCES.txt` & `ec2-manager-0.0.9/src/ec2_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

