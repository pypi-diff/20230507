# Comparing `tmp/modular_rl-0.1.3a0.tar.gz` & `tmp/modular_rl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modular_rl-0.1.3a0.tar", last modified: Thu May  4 14:37:24 2023, max compression
+gzip compressed data, was "modular_rl-0.2.0.tar", last modified: Sun May  7 07:25:57 2023, max compression
```

## Comparing `modular_rl-0.1.3a0.tar` & `modular_rl-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 14:37:24.047910 modular_rl-0.1.3a0/
--rw-rw-rw-   0        0        0     1089 2023-05-04 06:13:20.000000 modular_rl-0.1.3a0/LICENSE
--rw-rw-rw-   0        0        0     3863 2023-05-04 14:37:24.046401 modular_rl-0.1.3a0/PKG-INFO
--rw-rw-rw-   0        0        0     2488 2023-05-04 14:35:54.000000 modular_rl-0.1.3a0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 14:37:24.025586 modular_rl-0.1.3a0/modular_rl/
--rw-rw-rw-   0        0        0        0 2023-05-04 06:12:40.000000 modular_rl-0.1.3a0/modular_rl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 14:37:24.040984 modular_rl-0.1.3a0/modular_rl/agents/
--rw-rw-rw-   0        0        0        0 2023-05-04 06:12:40.000000 modular_rl-0.1.3a0/modular_rl/agents/__init__.py
--rw-rw-rw-   0        0        0    17172 2023-05-04 14:16:43.000000 modular_rl-0.1.3a0/modular_rl/agents/agent_ppo.py
--rw-rw-rw-   0        0        0     4474 2023-05-04 06:12:40.000000 modular_rl-0.1.3a0/modular_rl/networks.py
--rw-rw-rw-   0        0        0     2632 2023-05-04 10:13:40.000000 modular_rl-0.1.3a0/modular_rl/settings.py
--rw-rw-rw-   0        0        0     2103 2023-05-04 14:32:55.000000 modular_rl-0.1.3a0/modular_rl/tester.py
-drwxrwxrwx   0        0        0        0 2023-05-04 14:37:24.038361 modular_rl-0.1.3a0/modular_rl.egg-info/
--rw-rw-rw-   0        0        0     3863 2023-05-04 14:37:23.000000 modular_rl-0.1.3a0/modular_rl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2023-05-04 14:37:23.000000 modular_rl-0.1.3a0/modular_rl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 14:37:23.000000 modular_rl-0.1.3a0/modular_rl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-04 14:37:23.000000 modular_rl-0.1.3a0/modular_rl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-04 14:37:23.000000 modular_rl-0.1.3a0/modular_rl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1422 2023-05-04 14:36:01.000000 modular_rl-0.1.3a0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 14:37:24.048918 modular_rl-0.1.3a0/setup.cfg
--rw-rw-rw-   0        0        0      957 2023-05-04 14:36:07.000000 modular_rl-0.1.3a0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 14:37:24.045404 modular_rl-0.1.3a0/tests/
--rw-rw-rw-   0        0        0       53 2023-05-04 09:26:16.000000 modular_rl-0.1.3a0/tests/test.py
--rw-rw-rw-   0        0        0       61 2023-05-04 09:26:43.000000 modular_rl-0.1.3a0/tests/test_modular.py
+drwxrwxrwx   0        0        0        0 2023-05-07 07:25:57.085531 modular_rl-0.2.0/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 06:13:20.000000 modular_rl-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      798 2023-05-07 07:25:57.085011 modular_rl-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3960 2023-05-07 07:25:04.000000 modular_rl-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 07:25:57.011166 modular_rl-0.2.0/modular_rl/
+-rw-rw-rw-   0        0        0       36 2023-05-07 02:39:54.000000 modular_rl-0.2.0/modular_rl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 07:25:57.051609 modular_rl-0.2.0/modular_rl/agents/
+-rw-rw-rw-   0        0        0       54 2023-05-07 02:39:10.000000 modular_rl-0.2.0/modular_rl/agents/__init__.py
+-rw-rw-rw-   0        0        0     8892 2023-05-07 06:52:16.000000 modular_rl-0.2.0/modular_rl/agents/_agent.py
+-rw-rw-rw-   0        0        0    11655 2023-05-07 07:04:46.000000 modular_rl-0.2.0/modular_rl/agents/mcts.py
+-rw-rw-rw-   0        0        0    14827 2023-05-07 07:05:13.000000 modular_rl-0.2.0/modular_rl/agents/ppo.py
+drwxrwxrwx   0        0        0        0 2023-05-07 07:25:57.060609 modular_rl-0.2.0/modular_rl/networks/
+-rw-rw-rw-   0        0        0       66 2023-05-07 02:38:25.000000 modular_rl-0.2.0/modular_rl/networks/__init__.py
+-rw-rw-rw-   0        0        0     2121 2023-05-07 06:40:47.000000 modular_rl-0.2.0/modular_rl/networks/actor_critic.py
+-rw-rw-rw-   0        0        0     2878 2023-05-04 23:35:18.000000 modular_rl-0.2.0/modular_rl/networks/policy.py
+-rw-rw-rw-   0        0        0     2688 2023-05-04 23:33:52.000000 modular_rl-0.2.0/modular_rl/networks/value.py
+drwxrwxrwx   0        0        0        0 2023-05-07 07:25:57.068077 modular_rl-0.2.0/modular_rl/params/
+-rw-rw-rw-   0        0        0       54 2023-05-07 02:39:30.000000 modular_rl-0.2.0/modular_rl/params/__init__.py
+-rw-rw-rw-   0        0        0     2305 2023-05-07 06:43:45.000000 modular_rl-0.2.0/modular_rl/params/mcts.py
+-rw-rw-rw-   0        0        0     2015 2023-05-07 06:44:07.000000 modular_rl-0.2.0/modular_rl/params/ppo.py
+-rw-rw-rw-   0        0        0     1113 2023-05-07 06:45:58.000000 modular_rl-0.2.0/modular_rl/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-07 07:25:57.073078 modular_rl-0.2.0/modular_rl/tester/
+-rw-rw-rw-   0        0        0       59 2023-05-07 06:49:12.000000 modular_rl-0.2.0/modular_rl/tester/__init__.py
+-rw-rw-rw-   0        0        0      353 2023-05-07 06:48:36.000000 modular_rl-0.2.0/modular_rl/tester/mcts.py
+-rw-rw-rw-   0        0        0     1552 2023-05-05 00:05:02.000000 modular_rl-0.2.0/modular_rl/tester/ppo.py
+drwxrwxrwx   0        0        0        0 2023-05-07 07:25:57.077082 modular_rl-0.2.0/modular_rl/util/
+-rw-rw-rw-   0        0        0        0 2023-05-04 23:35:52.000000 modular_rl-0.2.0/modular_rl/util/__init__.py
+-rw-rw-rw-   0        0        0     2371 2023-05-05 09:56:27.000000 modular_rl-0.2.0/modular_rl/util/node.py
+drwxrwxrwx   0        0        0        0 2023-05-07 07:25:57.042138 modular_rl-0.2.0/modular_rl.egg-info/
+-rw-rw-rw-   0        0        0      798 2023-05-07 07:25:56.000000 modular_rl-0.2.0/modular_rl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      769 2023-05-07 07:25:56.000000 modular_rl-0.2.0/modular_rl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 07:25:56.000000 modular_rl-0.2.0/modular_rl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-05-07 07:25:56.000000 modular_rl-0.2.0/modular_rl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-07 07:25:56.000000 modular_rl-0.2.0/modular_rl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1414 2023-05-07 07:25:32.000000 modular_rl-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 07:25:57.085531 modular_rl-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      984 2023-05-05 13:24:21.000000 modular_rl-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 07:25:57.083450 modular_rl-0.2.0/tests/
+-rw-rw-rw-   0        0        0       93 2023-05-07 06:51:17.000000 modular_rl-0.2.0/tests/test_mcts.py
+-rw-rw-rw-   0        0        0       61 2023-05-05 10:03:21.000000 modular_rl-0.2.0/tests/test_ppo.py
+-rw-rw-rw-   0        0        0       69 2023-05-05 10:03:28.000000 modular_rl-0.2.0/tests/test_ppo_modular.py
```

### Comparing `modular_rl-0.1.3a0/LICENSE` & `modular_rl-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modular_rl-0.1.3a0/modular_rl/settings.py` & `modular_rl-0.2.0/modular_rl/params/ppo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,38 @@
-'''
-The AgentSettings class is a configuration class used for setting up the PPO agent. 
-
-It provides default values for various parameters used in the agent, 
-such as the maximum number of episodes, maximum number of timesteps per episode, PPO update timestep, 
-number of PPO epochs, mini-batch size, network architecture, learning rate, 
-discount factor, lambda factor, clipping parameter, early stopping threshold, 
-and whether to end training when the environment is done.
-
-The default dictionary provides default values for all parameters, 
-while default_modular provides default values for all parameters except done_loop_end. 
-These default values can be modified by passing in a dictionary of key-value pairs to the AgentSettings constructor.
-
-'''
-
-
-class AgentSettings:
-    default = {
-        'max_episodes': 30,  # Maximum number of episodes for training
-        'max_timesteps': 200,  # Maximum number of timesteps for each episode
-        'update_timestep': 2000,  # Update the policy every specified timestep
-        'ppo_epochs': 4,  # Number of PPO epochs
-        'mini_batch_size': 64,  # Batch size for PPO updates
-        'networks': 'medium',  # Size of the hidden layer in neural networks
-        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
-        'gamma': 0.99,  # Discount factor
-        'lam': 0.95,  # Lambda parameter for GAE
-        'clip_param': 0.2,  # Clipping parameter for PPO
-        # If the average reward is greater than or equal to this value, training is stopped early
-        'early_stop_threshold': -1,
-        'done_loop_end': False,  # If True, end the episode when the done flag is set
-        'reward_print': True,
-    }
-
-    default_modular = {
-        # Maximum number of episodes for training (-1 for no limit)
-        'max_episodes': -1,
-        # Maximum number of timesteps for each episode (-1 for no limit)
-        'max_timesteps': -1,
-        # Update the policy every specified timestep (-1 for no limit)
-        'update_timestep': -1,
-        'ppo_epochs': 4,  # Number of PPO epochs
-        'mini_batch_size': 64,  # Batch size for PPO updates
-        'networks': 'medium',  # Size of the hidden layer in neural networks
-        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
-        'gamma': 0.99,  # Discount factor
-        'lam': 0.95,  # Lambda parameter for GAE
-        'clip_param': 0.2,  # Clipping parameter for PPO
-        # If the average reward is greater than or equal to this value, training is stopped early
-        'early_stop_threshold': -1,
-        'reward_print': True,
-    }
+class ParamPPO:
+    default = {
+        'max_episodes': 30,  # Maximum number of episodes for training
+        'max_timesteps': 200,  # Maximum number of timesteps for each episode
+        'update_timestep': 2000,  # Update the policy every specified timestep
+        'ppo_epochs': 4,  # Number of PPO epochs
+        'mini_batch_size': 64,  # Batch size for PPO updates
+        'networks': 'medium',  # Size of the hidden layer in neural networks
+        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
+        'gamma': 0.99,  # Discount factor
+        'lam': 0.95,  # Lambda parameter for GAE
+        'clip_param': 0.2,  # Clipping parameter for PPO
+        # If the average reward is greater than or equal to this value, training is stopped early
+        'early_stop_threshold': -1,
+        'done_loop_end': False,  # If True, end the episode when the done flag is set
+        'log_level': 'debug',  # Log level for the logger
+        'log_init_pass': False,  # If True, skip logger initialization
+    }
+
+    default_modular = {
+        # Maximum number of episodes for training (-1 for no limit)
+        'max_episodes': -1,
+        # Maximum number of timesteps for each episode (-1 for no limit)
+        'max_timesteps': -1,
+        # Update the policy every specified timestep (-1 for no limit)
+        'update_timestep': -1,
+        'ppo_epochs': 4,  # Number of PPO epochs
+        'mini_batch_size': 64,  # Batch size for PPO updates
+        'networks': 'medium',  # Size of the hidden layer in neural networks
+        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
+        'gamma': 0.99,  # Discount factor
+        'lam': 0.95,  # Lambda parameter for GAE
+        'clip_param': 0.2,  # Clipping parameter for PPO
+        # If the average reward is greater than or equal to this value, training is stopped early
+        'early_stop_threshold': -1,
+        'log_level': 'debug',  # Log level for the logger
+        'log_init_pass': False,  # If True, skip logger initialization
+    }
```

### Comparing `modular_rl-0.1.3a0/pyproject.toml` & `modular_rl-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "modular_rl"
-version = "0.1.3a"
-authors = [
-  { name="horrible", email="shinjpn1@gmail.com" },
-]
-description = "ModularRL is a Python library for creating and training reinforcement learning agents using the Proximal Policy Optimization (PPO) algorithm. The library is designed to be easily customizable and modular, allowing users to quickly set up and train PPO agents for various environments."
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.6',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.10',
-    'Programming Language :: Python :: 3.11',
-]
-keywords=['ModularRL', 'Modular-RL', 'Modular_RL', 'Modular RL',  'modularrl',  'modular_rl', 'modular-rl', 'modular rl', 'mrl', 'modular', 'learn', 'learning', 'pytorch learn', 'pytorch learning']
-dependencies=['gym', 'numpy', 'torch']
-
-
-[project.urls]
-"Homepage" = "https://github.com/horrible-gh/ModularRL"
-"Bug Tracker" = "https://github.com/horrible-gh/ModularRL/issues"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "modular_rl"
+version = "0.2.0"
+authors = [
+  { name="horrible", email="shinjpn1@gmail.com" },
+]
+description = "ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm."
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.6',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+]
+keywords=['ModularRL', 'Modular-RL', 'Modular_RL', 'Modular RL',  'modularrl',  'modular_rl', 'modular-rl', 'modular rl', 'mrl', 'modular', 'learn', 'learning', 'pytorch learn', 'pytorch learning']
+dependencies=['gym', 'numpy', 'torch', 'LogAssist']
+
+
+[project.urls]
+"Homepage" = "https://github.com/horrible-gh/ModularRL"
+"Bug Tracker" = "https://github.com/horrible-gh/ModularRL/issues"
```

### Comparing `modular_rl-0.1.3a0/setup.py` & `modular_rl-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='modular_rl',
-    version='0.1.3a',
+    version='0.2.0',
     description='ModularRL package',
     author='sjm',
     author_email='shinjpn1@gmail.com',
     url='https://shinjpn-gitea.duckdns.org/gitea/sjm/ModularRL.git',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
@@ -21,9 +21,10 @@
         'Programming Language :: Python :: 3.11',
     ],
     python_requires='>=3.6',
     install_requires=[
         'numpy>=1.18.0',
         'torch>=1.24.2',
         'gym>=0.23.0',
+        'LogAssist>=1.0.4'
     ],
 )
```

