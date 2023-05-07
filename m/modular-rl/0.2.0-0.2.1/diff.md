# Comparing `tmp/modular_rl-0.2.0.tar.gz` & `tmp/modular_rl-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modular_rl-0.2.0.tar", last modified: Sun May  7 07:25:57 2023, max compression
+gzip compressed data, was "modular_rl-0.2.1.tar", last modified: Sun May  7 14:53:33 2023, max compression
```

## Comparing `modular_rl-0.2.0.tar` & `modular_rl-0.2.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 07:25:57.085531 modular_rl-0.2.0/
--rw-rw-rw-   0        0        0     1089 2023-05-04 06:13:20.000000 modular_rl-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      798 2023-05-07 07:25:57.085011 modular_rl-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3960 2023-05-07 07:25:04.000000 modular_rl-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 07:25:57.011166 modular_rl-0.2.0/modular_rl/
--rw-rw-rw-   0        0        0       36 2023-05-07 02:39:54.000000 modular_rl-0.2.0/modular_rl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-07 07:25:57.051609 modular_rl-0.2.0/modular_rl/agents/
--rw-rw-rw-   0        0        0       54 2023-05-07 02:39:10.000000 modular_rl-0.2.0/modular_rl/agents/__init__.py
--rw-rw-rw-   0        0        0     8892 2023-05-07 06:52:16.000000 modular_rl-0.2.0/modular_rl/agents/_agent.py
--rw-rw-rw-   0        0        0    11655 2023-05-07 07:04:46.000000 modular_rl-0.2.0/modular_rl/agents/mcts.py
--rw-rw-rw-   0        0        0    14827 2023-05-07 07:05:13.000000 modular_rl-0.2.0/modular_rl/agents/ppo.py
-drwxrwxrwx   0        0        0        0 2023-05-07 07:25:57.060609 modular_rl-0.2.0/modular_rl/networks/
--rw-rw-rw-   0        0        0       66 2023-05-07 02:38:25.000000 modular_rl-0.2.0/modular_rl/networks/__init__.py
--rw-rw-rw-   0        0        0     2121 2023-05-07 06:40:47.000000 modular_rl-0.2.0/modular_rl/networks/actor_critic.py
--rw-rw-rw-   0        0        0     2878 2023-05-04 23:35:18.000000 modular_rl-0.2.0/modular_rl/networks/policy.py
--rw-rw-rw-   0        0        0     2688 2023-05-04 23:33:52.000000 modular_rl-0.2.0/modular_rl/networks/value.py
-drwxrwxrwx   0        0        0        0 2023-05-07 07:25:57.068077 modular_rl-0.2.0/modular_rl/params/
--rw-rw-rw-   0        0        0       54 2023-05-07 02:39:30.000000 modular_rl-0.2.0/modular_rl/params/__init__.py
--rw-rw-rw-   0        0        0     2305 2023-05-07 06:43:45.000000 modular_rl-0.2.0/modular_rl/params/mcts.py
--rw-rw-rw-   0        0        0     2015 2023-05-07 06:44:07.000000 modular_rl-0.2.0/modular_rl/params/ppo.py
--rw-rw-rw-   0        0        0     1113 2023-05-07 06:45:58.000000 modular_rl-0.2.0/modular_rl/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-07 07:25:57.073078 modular_rl-0.2.0/modular_rl/tester/
--rw-rw-rw-   0        0        0       59 2023-05-07 06:49:12.000000 modular_rl-0.2.0/modular_rl/tester/__init__.py
--rw-rw-rw-   0        0        0      353 2023-05-07 06:48:36.000000 modular_rl-0.2.0/modular_rl/tester/mcts.py
--rw-rw-rw-   0        0        0     1552 2023-05-05 00:05:02.000000 modular_rl-0.2.0/modular_rl/tester/ppo.py
-drwxrwxrwx   0        0        0        0 2023-05-07 07:25:57.077082 modular_rl-0.2.0/modular_rl/util/
--rw-rw-rw-   0        0        0        0 2023-05-04 23:35:52.000000 modular_rl-0.2.0/modular_rl/util/__init__.py
--rw-rw-rw-   0        0        0     2371 2023-05-05 09:56:27.000000 modular_rl-0.2.0/modular_rl/util/node.py
-drwxrwxrwx   0        0        0        0 2023-05-07 07:25:57.042138 modular_rl-0.2.0/modular_rl.egg-info/
--rw-rw-rw-   0        0        0      798 2023-05-07 07:25:56.000000 modular_rl-0.2.0/modular_rl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      769 2023-05-07 07:25:56.000000 modular_rl-0.2.0/modular_rl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 07:25:56.000000 modular_rl-0.2.0/modular_rl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-05-07 07:25:56.000000 modular_rl-0.2.0/modular_rl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-07 07:25:56.000000 modular_rl-0.2.0/modular_rl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1414 2023-05-07 07:25:32.000000 modular_rl-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 07:25:57.085531 modular_rl-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      984 2023-05-05 13:24:21.000000 modular_rl-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 07:25:57.083450 modular_rl-0.2.0/tests/
--rw-rw-rw-   0        0        0       93 2023-05-07 06:51:17.000000 modular_rl-0.2.0/tests/test_mcts.py
--rw-rw-rw-   0        0        0       61 2023-05-05 10:03:21.000000 modular_rl-0.2.0/tests/test_ppo.py
--rw-rw-rw-   0        0        0       69 2023-05-05 10:03:28.000000 modular_rl-0.2.0/tests/test_ppo_modular.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:53:33.733066 modular_rl-0.2.1/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 06:13:20.000000 modular_rl-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     5462 2023-05-07 14:53:33.731892 modular_rl-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4096 2023-05-07 14:51:41.000000 modular_rl-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 14:53:33.680484 modular_rl-0.2.1/modular_rl/
+-rw-rw-rw-   0        0        0       37 2023-05-07 14:51:41.000000 modular_rl-0.2.1/modular_rl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:53:33.702316 modular_rl-0.2.1/modular_rl/agents/
+-rw-rw-rw-   0        0        0       56 2023-05-07 14:51:41.000000 modular_rl-0.2.1/modular_rl/agents/__init__.py
+-rw-rw-rw-   0        0        0     9120 2023-05-07 14:51:41.000000 modular_rl-0.2.1/modular_rl/agents/_agent.py
+-rw-rw-rw-   0        0        0    11964 2023-05-07 14:51:41.000000 modular_rl-0.2.1/modular_rl/agents/mcts.py
+-rw-rw-rw-   0        0        0    14793 2023-05-07 14:52:26.000000 modular_rl-0.2.1/modular_rl/agents/ppo.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:53:33.710075 modular_rl-0.2.1/modular_rl/networks/
+-rw-rw-rw-   0        0        0       68 2023-05-07 14:51:41.000000 modular_rl-0.2.1/modular_rl/networks/__init__.py
+-rw-rw-rw-   0        0        0     2174 2023-05-07 14:51:41.000000 modular_rl-0.2.1/modular_rl/networks/actor_critic.py
+-rw-rw-rw-   0        0        0     2878 2023-05-04 23:35:18.000000 modular_rl-0.2.1/modular_rl/networks/policy.py
+-rw-rw-rw-   0        0        0     2688 2023-05-04 23:33:52.000000 modular_rl-0.2.1/modular_rl/networks/value.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:53:33.716477 modular_rl-0.2.1/modular_rl/params/
+-rw-rw-rw-   0        0        0       56 2023-05-07 14:51:41.000000 modular_rl-0.2.1/modular_rl/params/__init__.py
+-rw-rw-rw-   0        0        0     2345 2023-05-07 14:51:41.000000 modular_rl-0.2.1/modular_rl/params/mcts.py
+-rw-rw-rw-   0        0        0     2053 2023-05-07 14:51:41.000000 modular_rl-0.2.1/modular_rl/params/ppo.py
+-rw-rw-rw-   0        0        0     1136 2023-05-07 14:51:41.000000 modular_rl-0.2.1/modular_rl/settings.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:53:33.721656 modular_rl-0.2.1/modular_rl/tester/
+-rw-rw-rw-   0        0        0       61 2023-05-07 14:51:41.000000 modular_rl-0.2.1/modular_rl/tester/__init__.py
+-rw-rw-rw-   0        0        0      366 2023-05-07 14:51:41.000000 modular_rl-0.2.1/modular_rl/tester/mcts.py
+-rw-rw-rw-   0        0        0     1552 2023-05-05 00:05:02.000000 modular_rl-0.2.1/modular_rl/tester/ppo.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:53:33.724864 modular_rl-0.2.1/modular_rl/util/
+-rw-rw-rw-   0        0        0        0 2023-05-04 23:35:52.000000 modular_rl-0.2.1/modular_rl/util/__init__.py
+-rw-rw-rw-   0        0        0     2371 2023-05-05 09:56:27.000000 modular_rl-0.2.1/modular_rl/util/node.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:53:33.693669 modular_rl-0.2.1/modular_rl.egg-info/
+-rw-rw-rw-   0        0        0     5462 2023-05-07 14:53:33.000000 modular_rl-0.2.1/modular_rl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      769 2023-05-07 14:53:33.000000 modular_rl-0.2.1/modular_rl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 14:53:33.000000 modular_rl-0.2.1/modular_rl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-07 14:53:33.000000 modular_rl-0.2.1/modular_rl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-07 14:53:33.000000 modular_rl-0.2.1/modular_rl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1414 2023-05-07 14:52:50.000000 modular_rl-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 14:53:33.734071 modular_rl-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      937 2023-05-07 14:52:59.000000 modular_rl-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:53:33.730646 modular_rl-0.2.1/tests/
+-rw-rw-rw-   0        0        0       97 2023-05-07 14:51:41.000000 modular_rl-0.2.1/tests/test_mcts.py
+-rw-rw-rw-   0        0        0       61 2023-05-05 10:03:21.000000 modular_rl-0.2.1/tests/test_ppo.py
+-rw-rw-rw-   0        0        0       69 2023-05-05 10:03:28.000000 modular_rl-0.2.1/tests/test_ppo_modular.py
```

### Comparing `modular_rl-0.2.0/LICENSE` & `modular_rl-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modular_rl-0.2.0/README.md` & `modular_rl-0.2.1/README.md`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-# ModularRL
-
-ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm.
-
-## Installation
-
-```powershell
-pip install modular_rl
-```
-
-## Features
-
--   Implementations of various reinforcement learning algorithms,
-    such as Proximal Policy Optimization (PPO) and Monte Carlo Tree Search (MCTS)
--   Customizable agent settings and network architectures
--   Modular structure for easy adaptation and extension across different algorithms
--   Model saving and loading functionality for easy reuse of trained models
-
-## Supported Algorithms
-
--   Proximal Policy Optimization (PPO)
--   Monte Carlo Tree Search (MCTS)
-
-Refer to the respective agent classes for each algorithm:
-
--   AgentPPO (Modular)
--   AgentMCTS
-
-## Example Usage
-
-You can use the tester.py script provided in the library to create and train an instance of an agent with default or modified settings:
-
-```python
-import modular_rl.tester as tester
-
-tester.init_ppo()
-# or
-tester.init_ppo_modular()
-
-tester.init_mcts()
-```
-
-As more algorithms are added, the tester functions will follow the naming convention init*[algorithm_name] or init*[algorithm_name]\_modular.
-
-Please note that not all algorithms support modular training due to the nature of their design.
-For such algorithms, you will need to use the non-modular training method provided by the respective agent class.
-You can refer to the list of supported algorithms to determine which training method is appropriate.
-
-Alternatively, you can create and train an instance of the AgentPPO(example) class directly in your code:
-
-```python
-from modular_rl.agents.agent_ppo import AgentPPO
-from modular_rl.settings import AgentSettings
-
-def init():
-    env = AgentPPO(env=None, setting=AgentSettings.default)
-    env.learn()
-
-init()
-```
-
-To create and train an instance of the AgentPPO(example) class with modified settings, use the following code:
-
-```python
-from modular_rl.agents.agent_ppo import AgentPPO
-from modular_rl.settings import AgentSettings
-
-def init_modular():
-    # Semi-automatic (defined record usage)
-    # Implement your environment and pass it to 'env' parameter.
-    env = AgentPPO(env=None, setting=AgentSettings.default_modular)
-    env.reset()
-    env.learn_reset()
-    action, reward, is_done = env.learn_next()
-    env.learn_check()
-    env.update()
-
-    # Proceed with the learning manually.
-    env.reset()
-    # Implement the 'reset' method in your environment.
-    '''
-    def reset(self):
-        ...
-        return initial_state
-    '''
-    env.learn_reset()
-    initial_state = env.learn_reset()
-    action, _ = env.select_action(initial_state)
-
-    '''
-    Note:
-    Please implement the resulting state of update_step in the step function of your environment.
-
-    For example:
-
-    def step(self, action):
-        ...
-        return next_state, reward, is_done, _
-    '''
-
-    env.update_step(initial_state, None, action, -1)
-
-    env.learn_check()
-    env.update()
-
-    env.learn_close()
-
-init_modular()
-```
-
-## Saving and Loading Models
-
-Agents can save and load their models using the save_model(file_name) and load_model(file_name) methods.
-The file_name parameter should be the name of the file to save or load the model to/from.
-
-Example:
-
-```python
-agent = AgentPPO(env, setting)
-agent.train()
-
-agent.save_model("my_saved_model.pth")
-
-loaded_agent = AgentPPO(env, setting)
-loaded_agent.load_model("my_saved_model.pth")
-```
-
-## Key Classes
-
--   AgentPPO, AgentMCTS: The main agent classes implementing various reinforcement learning algorithms.
--   PolicyNetwork, ValueNetwork, ActorCriticNetwork: Customizable neural networks for the agent's policy and value functions.
--   AgentSettings: A configuration class for setting up the agents.
-
-## License
-
-MIT License
+# ModularRL
+
+ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm.
+
+## Installation
+
+```powershell
+pip install modular_rl
+```
+
+## Features
+
+-   Implementations of various reinforcement learning algorithms,
+    such as Proximal Policy Optimization (PPO) and Monte Carlo Tree Search (MCTS)
+-   Customizable agent settings and network architectures
+-   Modular structure for easy adaptation and extension across different algorithms
+-   Model saving and loading functionality for easy reuse of trained models
+
+## Supported Algorithms
+
+-   Proximal Policy Optimization (PPO)
+-   Monte Carlo Tree Search (MCTS)
+
+Refer to the respective agent classes for each algorithm:
+
+-   AgentPPO (Modular)
+-   AgentMCTS
+
+## Example Usage
+
+You can use the tester.py script provided in the library to create and train an instance of an agent with default or modified settings:
+
+```python
+import modular_rl.tester as tester
+
+tester.init_ppo()
+# or
+tester.init_ppo_modular()
+
+tester.init_mcts()
+```
+
+As more algorithms are added, the tester functions will follow the naming convention init*[algorithm_name] or init*[algorithm_name]\_modular.
+
+Please note that not all algorithms support modular training due to the nature of their design.
+For such algorithms, you will need to use the non-modular training method provided by the respective agent class.
+You can refer to the list of supported algorithms to determine which training method is appropriate.
+
+Alternatively, you can create and train an instance of the AgentPPO(example) class directly in your code:
+
+```python
+from modular_rl.agents.agent_ppo import AgentPPO
+from modular_rl.settings import AgentSettings
+
+def init():
+    env = AgentPPO(env=None, setting=AgentSettings.default)
+    env.learn()
+
+init()
+```
+
+To create and train an instance of the AgentPPO(example) class with modified settings, use the following code:
+
+```python
+from modular_rl.agents.agent_ppo import AgentPPO
+from modular_rl.settings import AgentSettings
+
+def init_modular():
+    # Semi-automatic (defined record usage)
+    # Implement your environment and pass it to 'env' parameter.
+    env = AgentPPO(env=None, setting=AgentSettings.default_modular)
+    env.reset()
+    env.learn_reset()
+    action, reward, is_done = env.learn_next()
+    env.learn_check()
+    env.update()
+
+    # Proceed with the learning manually.
+    env.reset()
+    # Implement the 'reset' method in your environment.
+    '''
+    def reset(self):
+        ...
+        return initial_state
+    '''
+    env.learn_reset()
+    initial_state = env.learn_reset()
+    action, _ = env.select_action(initial_state)
+
+    '''
+    Note:
+    Please implement the resulting state of update_step in the step function of your environment.
+
+    For example:
+
+    def step(self, action):
+        ...
+        return next_state, reward, is_done, _
+    '''
+
+    env.update_step(initial_state, None, action, -1)
+
+    env.learn_check()
+    env.update()
+
+    env.learn_close()
+
+init_modular()
+```
+
+## Saving and Loading Models
+
+Agents can save and load their models using the save_model(file_name) and load_model(file_name) methods.
+The file_name parameter should be the name of the file to save or load the model to/from.
+
+Example:
+
+```python
+agent = AgentPPO(env, setting)
+agent.train()
+
+agent.save_model("my_saved_model.pth")
+
+loaded_agent = AgentPPO(env, setting)
+loaded_agent.load_model("my_saved_model.pth")
+```
+
+## Key Classes
+
+-   AgentPPO, AgentMCTS: The main agent classes implementing various reinforcement learning algorithms.
+-   PolicyNetwork, ValueNetwork, ActorCriticNetwork: Customizable neural networks for the agent's policy and value functions.
+-   AgentSettings: A configuration class for setting up the agents.
+
+## License
+
+MIT License
```

### Comparing `modular_rl-0.2.0/modular_rl/agents/_agent.py` & `modular_rl-0.2.1/modular_rl/agents/_agent.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,228 +1,228 @@
-# -*- coding: utf-8 -*-
-"""
-ModularRL project
-
-Copyright (c) 2023 horrible-gh
-
-Class AgentPPO is an implementation of the Proximal Policy Optimization (PPO) algorithm.
-It takes an environment and a setting configuration as inputs, initializes neural network instances and optimizers,
-and sets various learning parameters.
-It has methods to predict an action given a state, perform a learning step, update the neural network parameters,
-save and load a checkpoint, and reset learning parameters.
-The class also has instance variables to keep track of episode and total rewards, previous reward, and average reward.
-
-This software includes the following third-party libraries:
-Gym (MIT License): https://github.com/openai/gym - Copyright (c) OpenAI.
-NumPy (BSD License): https://numpy.org - Copyright (c) NumPy Developers.
-PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
-"""
-
-import gym
-from LogAssist.log import Logger
-import torch
-import torch.optim as optim
-from modular_rl.networks.policy import PolicyNetwork
-from modular_rl.networks.value import ValueNetwork
-from modular_rl.networks.actor_critic import ActorCriticNetwork
-
-
-class Agent:
-    def __init__(self, env, setting):
-        '''
-        :param env: The environment for the agent to interact with, if not provided, CartPole-v0 will be used.
-        :param setting: A dictionary containing the settings and hyperparameters for the agent's training process.
-        '''
-
-        # Environment preparation
-        self.env = env if env else gym.make('CartPole-v0')
-        self.setting = setting
-        self.state_dim = self.env.observation_space.shape[0]
-        self.action_dim = self.env.action_space.n
-
-        # Defination networks and optimizers
-        self.policy_net = None
-        self.value_net = None
-        self.policy_optimizer = None
-        self.value_optimizer = None
-
-        self.actor_critic_net = None
-        self.actor_critic_optimizer = None
-
-        # Training parameters(Common)
-        self.max_episodes = setting.get('max_episodes', 30)
-        self.max_timesteps = setting.get('max_timesteps', 1000)
-        self.update_timestep = setting.get('update_timestep', 200)
-        self.gamma = setting.get('gamma', 0.99)
-        self.early_stop_threshold = setting.get('early_stop_threshold', -1)
-        self.done_loop_end = setting.get('done_loop_end', False)
-
-        # Set learn episode parameters
-        self.episode_reward = 0
-        self.total_reward = 0
-        self.prev_reward = 0
-        self.episode = 0
-        self.avg_reward = 0
-
-        # Set learn parameters (If necessary)
-        self.state = None
-        self.action = None
-        self.reward = None
-        self.done = None
-
-        # Logger initialize
-        self.log_level = setting.get('log_level', 'debug')
-        self.log_init_pass = setting.get('log_init_pass', False)
-        if self.log_init_pass == False:
-            Logger.init(
-                dir_name=None,
-                file_name=None,
-                log_level=self.log_level,
-                out_console=True,
-                out_file=None,
-                prev_log_remove=None
-            )
-
-    def init_policy_value(self):
-        """
-        Initializes policy and value networks, and their respective optimizers.
-        """
-
-        # Create neural network instances and optimizer
-        self.policy_net = PolicyNetwork(
-            self.state_dim, self.action_dim, self.setting.get('networks', 'middle'))
-        self.value_net = ValueNetwork(
-            self.state_dim, self.setting.get('networks', 'middle'))
-        self.policy_optimizer = optim.Adam(
-            self.policy_net.parameters(), lr=self.setting.get('optimizer_speed', 3e-4))
-        self.value_optimizer = optim.Adam(
-            self.value_net.parameters(), lr=self.setting.get('optimizer_speed', 3e-4))
-
-    def init_actor_critic(self):
-        """
-        Initializes the actor-critic network and its optimizer.
-        """
-
-        # Neural Network
-        self.actor_critic_net = ActorCriticNetwork(
-            self.state_dim, self.action_dim)
-        self.actor_critic_optimizer = optim.Adam(
-            self.actor_critic_net.parameters(), lr=self.setting.get('optimizer_speed', 3e-4))
-
-    def _check_state(self, state):
-        '''
-        This function takes a state parameter and returns the first element of a tuple if state has a length of 2, otherwise it simply returns the state parameter.
-
-        :param state: The state data to be checked.
-        :return: The checked state data.
-        '''
-
-        state_num = len(state)
-        if state_num == 2:
-            state, _ = state  # Unpack the tuple
-        return state
-
-    def learn_reset(self):
-        """
-        Reset the agent's state and episode reward.
-        """
-
-        self.state = self.env.reset()
-        return self._check_state(self.state)
-
-    def learn_close(self):
-        """
-        Close the environment and reset the agent's total reward, episode count, and episode reward.
-        """
-
-        self.env.close()
-        self.total_reward = 0
-        self.episode = 0
-        self.episode_reward = 0
-
-    def learn_check(self):
-        """
-        Print the episode count, previous reward, episode reward, total reward, and average episode reward.
-        """
-
-        avg_reward = self.total_reward / (self.episode + 1)
-        Logger.debug(
-            f'Episode: {self.episode}, Previous Reward: {self.prev_reward},  Episode Reward: {self.episode_reward}, Total Reward: {self.total_reward}, Average Episode Reward: {avg_reward}')
-
-    def select_action(self, state):
-        '''
-        These functions are placeholders and must be implemented by the child class that extends this Agent class.
-
-        select_action() function is a placeholder that needs to be implemented in the child class that extends the Agent class. This function takes the current state of the environment and returns the selected action for the agent to take.
-
-        :param state: The current state of the environment.
-        :return: The selected action for the agent to take.
-        '''
-        pass
-
-    def update(self):
-        '''
-        This function is a placeholder and must be implemented by the child class that extends this Agent class.
-
-        update() function is a placeholder that needs to be implemented in the child class that extends the Agent class. This function is responsible for updating the agent's state, action, and policy based on the new state and reward received from the environment.
-
-        No parameters are passed into this function and it does not return anything.
-        '''
-        pass
-
-    def save_policy_value(self, file_name):
-        """
-        Save the policy and value networks and their optimizer states in a file.
-
-        :param file_name: The name of the file to save the networks and optimizer states.
-        :type file_name: str
-        """
-
-        torch.save({
-            'policy_net_state_dict': self.policy_net.state_dict(),
-            'value_net_state_dict': self.value_net.state_dict(),
-            'policy_optimizer_state_dict': self.policy_optimizer.state_dict(),
-            'value_optimizer_state_dict': self.value_optimizer.state_dict(),
-        }, file_name)
-
-    def load_policy_value(self, file_name):
-        """
-        Load the policy and value networks and their optimizer states from a file.
-
-        :param file_name: The name of the file to load the networks and optimizer states from.
-        :type file_name: str
-        """
-
-        checkpoint = torch.load(file_name)
-        self.policy_net.load_state_dict(checkpoint['policy_net_state_dict'])
-        self.value_net.load_state_dict(checkpoint['value_net_state_dict'])
-        self.policy_optimizer.load_state_dict(
-            checkpoint['policy_optimizer_state_dict'])
-        self.value_optimizer.load_state_dict(
-            checkpoint['value_optimizer_state_dict'])
-
-    def save_actor_critic(self, file_name):
-        """
-        Save the actor-critic network and its optimizer state in a file.
-
-        :param file_name: The name of the file to save the network and optimizer state.
-        :type file_name: str
-        """
-
-        torch.save({
-            'actor_critic_net_state_dict': self.actor_critic_net.state_dict(),
-            'optimizer_state_dict': self.actor_critic_optimizer.state_dict(),
-        }, file_name)
-
-    def load_actor_critic(self, file_name):
-        """
-        Load the actor-critic network and its optimizer state from a file.
-
-        :param file_name: The name of the file to load the network and optimizer state from.
-        :type file_name: str
-        """
-
-        checkpoint = torch.load(file_name)
-        self.actor_critic_net.load_state_dict(
-            checkpoint['actor_critic_net_state_dict'])
-        self.actor_critic_optimizer.load_state_dict(
-            checkpoint['optimizer_state_dict'])
+# -*- coding: utf-8 -*-
+"""
+ModularRL project
+
+Copyright (c) 2023 horrible-gh
+
+Class AgentPPO is an implementation of the Proximal Policy Optimization (PPO) algorithm.
+It takes an environment and a setting configuration as inputs, initializes neural network instances and optimizers,
+and sets various learning parameters.
+It has methods to predict an action given a state, perform a learning step, update the neural network parameters,
+save and load a checkpoint, and reset learning parameters.
+The class also has instance variables to keep track of episode and total rewards, previous reward, and average reward.
+
+This software includes the following third-party libraries:
+Gym (MIT License): https://github.com/openai/gym - Copyright (c) OpenAI.
+NumPy (BSD License): https://numpy.org - Copyright (c) NumPy Developers.
+PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
+"""
+
+import gym
+from LogAssist.log import Logger
+import torch
+import torch.optim as optim
+from modular_rl.networks.policy import PolicyNetwork
+from modular_rl.networks.value import ValueNetwork
+from modular_rl.networks.actor_critic import ActorCriticNetwork
+
+
+class Agent:
+    def __init__(self, env, setting):
+        '''
+        :param env: The environment for the agent to interact with, if not provided, CartPole-v0 will be used.
+        :param setting: A dictionary containing the settings and hyperparameters for the agent's training process.
+        '''
+
+        # Environment preparation
+        self.env = env if env else gym.make('CartPole-v0')
+        self.setting = setting
+        self.state_dim = self.env.observation_space.shape[0]
+        self.action_dim = self.env.action_space.n
+
+        # Defination networks and optimizers
+        self.policy_net = None
+        self.value_net = None
+        self.policy_optimizer = None
+        self.value_optimizer = None
+
+        self.actor_critic_net = None
+        self.actor_critic_optimizer = None
+
+        # Training parameters(Common)
+        self.max_episodes = setting.get('max_episodes', 30)
+        self.max_timesteps = setting.get('max_timesteps', 1000)
+        self.update_timestep = setting.get('update_timestep', 200)
+        self.gamma = setting.get('gamma', 0.99)
+        self.early_stop_threshold = setting.get('early_stop_threshold', -1)
+        self.done_loop_end = setting.get('done_loop_end', False)
+
+        # Set learn episode parameters
+        self.episode_reward = 0
+        self.total_reward = 0
+        self.prev_reward = 0
+        self.episode = 0
+        self.avg_reward = 0
+
+        # Set learn parameters (If necessary)
+        self.state = None
+        self.action = None
+        self.reward = None
+        self.done = None
+
+        # Logger initialize
+        self.log_level = setting.get('log_level', 'debug')
+        self.log_init_pass = setting.get('log_init_pass', False)
+        if self.log_init_pass == False:
+            Logger.init(
+                dir_name=None,
+                file_name=None,
+                log_level=self.log_level,
+                out_console=True,
+                out_file=None,
+                prev_log_remove=None
+            )
+
+    def init_policy_value(self):
+        """
+        Initializes policy and value networks, and their respective optimizers.
+        """
+
+        # Create neural network instances and optimizer
+        self.policy_net = PolicyNetwork(
+            self.state_dim, self.action_dim, self.setting.get('networks', 'middle'))
+        self.value_net = ValueNetwork(
+            self.state_dim, self.setting.get('networks', 'middle'))
+        self.policy_optimizer = optim.Adam(
+            self.policy_net.parameters(), lr=self.setting.get('optimizer_speed', 3e-4))
+        self.value_optimizer = optim.Adam(
+            self.value_net.parameters(), lr=self.setting.get('optimizer_speed', 3e-4))
+
+    def init_actor_critic(self):
+        """
+        Initializes the actor-critic network and its optimizer.
+        """
+
+        # Neural Network
+        self.actor_critic_net = ActorCriticNetwork(
+            self.state_dim, self.action_dim)
+        self.actor_critic_optimizer = optim.Adam(
+            self.actor_critic_net.parameters(), lr=self.setting.get('optimizer_speed', 3e-4))
+
+    def _check_state(self, state):
+        '''
+        This function takes a state parameter and returns the first element of a tuple if state has a length of 2, otherwise it simply returns the state parameter.
+
+        :param state: The state data to be checked.
+        :return: The checked state data.
+        '''
+
+        state_num = len(state)
+        if state_num == 2:
+            state, _ = state  # Unpack the tuple
+        return state
+
+    def learn_reset(self):
+        """
+        Reset the agent's state and episode reward.
+        """
+
+        self.state = self.env.reset()
+        return self._check_state(self.state)
+
+    def learn_close(self):
+        """
+        Close the environment and reset the agent's total reward, episode count, and episode reward.
+        """
+
+        self.env.close()
+        self.total_reward = 0
+        self.episode = 0
+        self.episode_reward = 0
+
+    def learn_check(self):
+        """
+        Print the episode count, previous reward, episode reward, total reward, and average episode reward.
+        """
+
+        avg_reward = self.total_reward / (self.episode + 1)
+        Logger.debug(
+            f'Episode: {self.episode}, Previous Reward: {self.prev_reward},  Episode Reward: {self.episode_reward}, Total Reward: {self.total_reward}, Average Episode Reward: {avg_reward}')
+
+    def select_action(self, state):
+        '''
+        These functions are placeholders and must be implemented by the child class that extends this Agent class.
+
+        select_action() function is a placeholder that needs to be implemented in the child class that extends the Agent class. This function takes the current state of the environment and returns the selected action for the agent to take.
+
+        :param state: The current state of the environment.
+        :return: The selected action for the agent to take.
+        '''
+        pass
+
+    def update(self):
+        '''
+        This function is a placeholder and must be implemented by the child class that extends this Agent class.
+
+        update() function is a placeholder that needs to be implemented in the child class that extends the Agent class. This function is responsible for updating the agent's state, action, and policy based on the new state and reward received from the environment.
+
+        No parameters are passed into this function and it does not return anything.
+        '''
+        pass
+
+    def save_policy_value(self, file_name):
+        """
+        Save the policy and value networks and their optimizer states in a file.
+
+        :param file_name: The name of the file to save the networks and optimizer states.
+        :type file_name: str
+        """
+
+        torch.save({
+            'policy_net_state_dict': self.policy_net.state_dict(),
+            'value_net_state_dict': self.value_net.state_dict(),
+            'policy_optimizer_state_dict': self.policy_optimizer.state_dict(),
+            'value_optimizer_state_dict': self.value_optimizer.state_dict(),
+        }, file_name)
+
+    def load_policy_value(self, file_name):
+        """
+        Load the policy and value networks and their optimizer states from a file.
+
+        :param file_name: The name of the file to load the networks and optimizer states from.
+        :type file_name: str
+        """
+
+        checkpoint = torch.load(file_name)
+        self.policy_net.load_state_dict(checkpoint['policy_net_state_dict'])
+        self.value_net.load_state_dict(checkpoint['value_net_state_dict'])
+        self.policy_optimizer.load_state_dict(
+            checkpoint['policy_optimizer_state_dict'])
+        self.value_optimizer.load_state_dict(
+            checkpoint['value_optimizer_state_dict'])
+
+    def save_actor_critic(self, file_name):
+        """
+        Save the actor-critic network and its optimizer state in a file.
+
+        :param file_name: The name of the file to save the network and optimizer state.
+        :type file_name: str
+        """
+
+        torch.save({
+            'actor_critic_net_state_dict': self.actor_critic_net.state_dict(),
+            'optimizer_state_dict': self.actor_critic_optimizer.state_dict(),
+        }, file_name)
+
+    def load_actor_critic(self, file_name):
+        """
+        Load the actor-critic network and its optimizer state from a file.
+
+        :param file_name: The name of the file to load the network and optimizer state from.
+        :type file_name: str
+        """
+
+        checkpoint = torch.load(file_name)
+        self.actor_critic_net.load_state_dict(
+            checkpoint['actor_critic_net_state_dict'])
+        self.actor_critic_optimizer.load_state_dict(
+            checkpoint['optimizer_state_dict'])
```

### Comparing `modular_rl-0.2.0/modular_rl/agents/mcts.py` & `modular_rl-0.2.1/modular_rl/agents/mcts.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,309 +1,309 @@
-
-# -*- coding: utf-8 -*-
-"""
-ModularRL project
-
-Copyright (c) 2023 horrible-gh
-
-Class AgentMCTS is an implementation of the Monte Carlo Tree Search (MCTS) algorithm.
-It takes an environment and a setting configuration as inputs, initializes neural network instances and optimizers,
-and sets various learning parameters.
-It has methods to predict an action given a state, perform a learning step, update the neural network parameters,
-save and load a checkpoint, and reset learning parameters.
-The class also has instance variables to keep track of episode and total rewards, previous reward, and average reward.
-
-This software includes the following third-party libraries:
-Gym (MIT License): https://github.com/openai/gym - Copyright (c) OpenAI.
-NumPy (BSD License): https://numpy.org - Copyright (c) NumPy Developers.
-PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
-"""
-
-import gym
-import torch
-import torch.optim as optim
-from torch.distributions import Categorical
-import torch.nn.functional as F
-from modular_rl.networks.actor_critic import ActorCriticNetwork
-from modular_rl.util.node import Node
-from modular_rl.agents._agent import Agent
-from LogAssist.log import Logger
-
-
-class AgentMCTS(Agent):
-    def __init__(self, env, setting):
-        """
-        Initialize the AgentMCTS class with the specified environment and settings.
-
-        :param env: The environment to use for training.
-        :type env: gym.Env or None
-        :param setting: The settings for the MCTS algorithm.
-        :type setting: AgentSettings
-        """
-
-        super().__init__(env, setting)
-        super().init_actor_critic()
-
-        # MCTS parameters
-        self.num_simulations = setting.get('num_simulations', 800)
-        self.cpuct = setting.get('cpuct', 1.0)
-        self.temperature = setting.get('temperature', 1.0)
-
-        self.device = setting.get('device', None)
-        if self.device == None:
-            self.device = torch.device(
-                "cuda" if torch.cuda.is_available() else "cpu")
-
-        # Save selected learning data separately
-        # self.state_tensor
-
-    def select_action(self, state):
-        """
-        Select an action using MCTS.
-
-        :param state: The current state.
-        :type state: numpy.ndarray
-        :return: The selected action.
-        :rtype: int
-        """
-
-        state_tensor = self.check_tensor(self._check_state(state))
-        action_probs, _ = self.actor_critic_net(state_tensor)
-        action_probs = action_probs.detach().numpy().flatten()
-        root = Node(state, action_probs)
-        Logger.verb(
-            'agents:mcts:select_action:self.num_simulations', self.num_simulations)
-        Logger.verb(
-            'agents:mcts:select_action:root', root)
-        Logger.verb(
-            'agents:mcts:select_action:action_probs', action_probs)
-        Logger.verb('agents:mcts:select_action:node', f'Root node: {root}')
-        for _ in range(self.num_simulations):
-            node = root
-            search_path = [node]
-            # Logger.verb(
-            #    'agents:mcts:select_action:search_path', search_path)
-            # Selection
-            while node.expanded():
-                action, node = node.select_child(self.cpuct)
-                search_path.append(node)
-            Logger.verb('agents:mcts:select_action:After selection',
-                        f' {search_path[-1]}')
-
-            # Expansion
-            if len(search_path) > 1:
-                parent, action = search_path[-2], search_path[-1].action
-            else:
-                # or some other suitable defaults
-                parent, action = search_path[0], None
-
-            # Logger.verb('mcts:select_action:action', action)
-            step_output = self.env.step(action) if action is not None else (
-                parent.state, 0, False, None)
-            step_output_num = len(step_output)
-
-            if step_output_num == 4:
-                state, reward, done, _ = step_output
-            elif step_output_num == 5:
-                state, reward, done, _, _ = step_output
-
-            if not done:
-                # Logger.verb(
-                #    'agents:mcts:select_action:state', state)
-                if not torch.is_tensor(state):
-                    state_tensor = torch.from_numpy(
-                        state).float().to(self.device)
-                else:
-                    state_tensor = state.to(self.device)
-
-                action_probs, value = self.actor_critic_net(state_tensor)
-                action_space = self.env.action_space.n
-                node.expand(action_space, action_probs)
-
-            # Backpropagation
-            self.backpropagate(search_path, reward, done)
-
-        chosen_action = root.select_action(self.temperature)
-        chosen_action_reward = root.children[chosen_action].total_value
-        chosen_action_state = root.children[chosen_action].state
-        # Assuming that a non-zero reward indicates a terminal state
-        done = (chosen_action_reward != 0)
-
-        # Save selected learning data separately
-        self.state = chosen_action_state
-        self.action = chosen_action
-        self.reward = chosen_action_reward
-        self.done = done
-
-        self.total_reward += reward
-        self.prev_reward = reward
-
-        return chosen_action_state, chosen_action, chosen_action_reward, done
-
-    def backpropagate(self, search_path, reward, done):
-        """
-        Backpropagate the value estimates back to the root node.
-
-        :param search_path: The nodes visited during the search.
-        :type search_path: list of Node
-        :param reward: The reward obtained after the search.
-        :type reward: float
-        :param done: Whether the episode has ended.
-        :type done: bool
-        """
-        for node in reversed(search_path):
-            node.update_stats(reward)
-            if not done:
-                _, reward = self.actor_critic_net(node.state)
-                reward = reward.item()
-
-    def learn(self):
-        """
-        Train the agent.
-        """
-        self.train()
-
-    def train(self):
-        """
-        Train the agent.
-        """
-        self.total_reward = 0
-        for episode in range(self.max_episodes):
-            self.episode = episode
-            state = self.learn_reset()
-            # state = self.env.reset()
-
-            for t in range(self.max_timesteps):
-                state = self._check_state(state)
-                self.state_tensor = self.check_tensor(state).squeeze(0)
-                self.next_state, self.action, self.reward, self.done = self.select_action(
-                    self.state_tensor)
-
-                self.learn_check()
-
-                if self.done:
-                    # self.update()
-                    break
-
-                self.update()
-
-                state = self.next_state
-
-            self.episode += 1
-            # print(f"Episode: {self.episode}, Reward: {self.total_reward}")
-
-    def compute_loss(self, state, action, reward, next_state, done):
-        '''
-        This function computes the actor and critic loss using the provided state, action, reward, next_state, and done variables.
-        The actor loss is computed based on the policy gradient algorithm,
-        and the critic loss is computed as the mean squared error between the estimated value of the current state and the target value of the next state.
-
-        compute_loss() function computes the actor and critic loss values for the provided state, action, reward, next_state, and done variables.
-
-        The state parameter is the current state of the environment.
-        The action parameter is the action taken in the current state.
-        The reward parameter is the reward received for taking the action in the current state.
-        The next_state parameter is the state resulting from taking the action in the current state.
-        The done parameter is a flag indicating whether the episode has ended.
-
-        :param state: The current state of the environment.
-        :param action: The action taken in the current state.
-        :param reward: The reward received for taking the action in the current state.
-        :param next_state: The state resulting from taking the action in the current state.
-        :param done: A flag indicating whether the episode has ended.
-        :return: The computed actor and critic loss values.
-        '''
-
-        # Predict action probabilities and values
-        action_probs, values = self.actor_critic_net(state)
-
-        # Compute the value loss
-        target_values = reward + self.gamma * \
-            self.actor_critic_net(next_state)[1] * (1 - done)
-        critic_loss = F.mse_loss(values, target_values.detach())
-
-        # Compute the policy loss
-        m = Categorical(action_probs)
-        logprobs = m.log_prob(self.check_tensor(action))
-        actor_loss = -logprobs * (target_values - values).detach()
-
-        return actor_loss, critic_loss
-
-    def update(self):
-        '''
-        This function updates the network parameters using the optimizer and computed loss values.
-
-        update() function updates the network parameters using the optimizer and computed loss values.
-        It uses the compute_loss() function to compute the loss and the optimizer object to perform the optimization step.
-
-        This function does not take any parameters and does not return anything.
-
-        :return: None
-        '''
-
-        # Update the network
-        self.actor_critic_optimizer.zero_grad()
-        actor_loss, critic_loss = self.compute_loss(
-            self.state_tensor, self.action, self.reward, self.next_state, self.done)
-        loss = actor_loss + critic_loss
-        loss.backward()
-        self.actor_critic_optimizer.step()
-
-    def check_tensor(self, obj):
-        '''
-        This function checks if the provided object is a PyTorch tensor, and if not, converts it to a tensor.
-
-        check_tensor() function checks if the provided obj parameter is a PyTorch tensor.
-        If it is not a tensor, it converts it to a tensor using torch.FloatTensor().
-        If it is already a tensor, it simply returns the tensor.
-
-        The obj parameter is the object to check/convert to a PyTorch tensor.
-
-        The function returns the input object as a PyTorch tensor.
-
-        :param obj: The object to check/convert to a PyTorch tensor.
-        :return: The input object as a PyTorch tensor.
-        '''
-
-        if not torch.is_tensor(obj):
-            obj_tensor = torch.FloatTensor(obj)
-        else:
-            obj_tensor = obj
-        return obj_tensor
-
-    def save_model(self, file_name):
-        """
-        This function saves the model to the specified file.
-
-        :param file_name: The name of the file to save the model to.
-        :return: None
-        """
-        self.save(file_name)
-
-    def save(self, file_name):
-        """
-        This function saves the actor critic network to the specified file.
-
-        :param file_name: The name of the file to save the actor critic network to.
-        :return: None
-        """
-
-        self.save_actor_critic(file_name)
-
-    def load_model(self, file_name):
-        """
-        This function loads the model from the specified file.
-
-        :param file_name: The name of the file to load the model from.
-        :return: None
-        """
-        self.load(file_name)
-
-    def load(self, file_name):
-        """
-        This function loads the actor critic network from the specified file.
-
-        :param file_name: The name of the file to load the actor critic network from.
-        :return: None
-        """
-
-        self.load_actor_critic(file_name)
+
+# -*- coding: utf-8 -*-
+"""
+ModularRL project
+
+Copyright (c) 2023 horrible-gh
+
+Class AgentMCTS is an implementation of the Monte Carlo Tree Search (MCTS) algorithm.
+It takes an environment and a setting configuration as inputs, initializes neural network instances and optimizers,
+and sets various learning parameters.
+It has methods to predict an action given a state, perform a learning step, update the neural network parameters,
+save and load a checkpoint, and reset learning parameters.
+The class also has instance variables to keep track of episode and total rewards, previous reward, and average reward.
+
+This software includes the following third-party libraries:
+Gym (MIT License): https://github.com/openai/gym - Copyright (c) OpenAI.
+NumPy (BSD License): https://numpy.org - Copyright (c) NumPy Developers.
+PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
+"""
+
+import gym
+import torch
+import torch.optim as optim
+from torch.distributions import Categorical
+import torch.nn.functional as F
+from modular_rl.networks.actor_critic import ActorCriticNetwork
+from modular_rl.util.node import Node
+from modular_rl.agents._agent import Agent
+from LogAssist.log import Logger
+
+
+class AgentMCTS(Agent):
+    def __init__(self, env, setting):
+        """
+        Initialize the AgentMCTS class with the specified environment and settings.
+
+        :param env: The environment to use for training.
+        :type env: gym.Env or None
+        :param setting: The settings for the MCTS algorithm.
+        :type setting: AgentSettings
+        """
+
+        super().__init__(env, setting)
+        super().init_actor_critic()
+
+        # MCTS parameters
+        self.num_simulations = setting.get('num_simulations', 800)
+        self.cpuct = setting.get('cpuct', 1.0)
+        self.temperature = setting.get('temperature', 1.0)
+
+        self.device = setting.get('device', None)
+        if self.device == None:
+            self.device = torch.device(
+                "cuda" if torch.cuda.is_available() else "cpu")
+
+        # Save selected learning data separately
+        # self.state_tensor
+
+    def select_action(self, state):
+        """
+        Select an action using MCTS.
+
+        :param state: The current state.
+        :type state: numpy.ndarray
+        :return: The selected action.
+        :rtype: int
+        """
+
+        state_tensor = self.check_tensor(self._check_state(state))
+        action_probs, _ = self.actor_critic_net(state_tensor)
+        action_probs = action_probs.detach().numpy().flatten()
+        root = Node(state, action_probs)
+        Logger.verb(
+            'agents:mcts:select_action:self.num_simulations', self.num_simulations)
+        Logger.verb(
+            'agents:mcts:select_action:root', root)
+        Logger.verb(
+            'agents:mcts:select_action:action_probs', action_probs)
+        Logger.verb('agents:mcts:select_action:node', f'Root node: {root}')
+        for _ in range(self.num_simulations):
+            node = root
+            search_path = [node]
+            # Logger.verb(
+            #    'agents:mcts:select_action:search_path', search_path)
+            # Selection
+            while node.expanded():
+                action, node = node.select_child(self.cpuct)
+                search_path.append(node)
+            Logger.verb('agents:mcts:select_action:After selection',
+                        f' {search_path[-1]}')
+
+            # Expansion
+            if len(search_path) > 1:
+                parent, action = search_path[-2], search_path[-1].action
+            else:
+                # or some other suitable defaults
+                parent, action = search_path[0], None
+
+            # Logger.verb('mcts:select_action:action', action)
+            step_output = self.env.step(action) if action is not None else (
+                parent.state, 0, False, None)
+            step_output_num = len(step_output)
+
+            if step_output_num == 4:
+                state, reward, done, _ = step_output
+            elif step_output_num == 5:
+                state, reward, done, _, _ = step_output
+
+            if not done:
+                # Logger.verb(
+                #    'agents:mcts:select_action:state', state)
+                if not torch.is_tensor(state):
+                    state_tensor = torch.from_numpy(
+                        state).float().to(self.device)
+                else:
+                    state_tensor = state.to(self.device)
+
+                action_probs, value = self.actor_critic_net(state_tensor)
+                action_space = self.env.action_space.n
+                node.expand(action_space, action_probs)
+
+            # Backpropagation
+            self.backpropagate(search_path, reward, done)
+
+        chosen_action = root.select_action(self.temperature)
+        chosen_action_reward = root.children[chosen_action].total_value
+        chosen_action_state = root.children[chosen_action].state
+        # Assuming that a non-zero reward indicates a terminal state
+        done = (chosen_action_reward != 0)
+
+        # Save selected learning data separately
+        self.state = chosen_action_state
+        self.action = chosen_action
+        self.reward = chosen_action_reward
+        self.done = done
+
+        self.total_reward += reward
+        self.prev_reward = reward
+
+        return chosen_action_state, chosen_action, chosen_action_reward, done
+
+    def backpropagate(self, search_path, reward, done):
+        """
+        Backpropagate the value estimates back to the root node.
+
+        :param search_path: The nodes visited during the search.
+        :type search_path: list of Node
+        :param reward: The reward obtained after the search.
+        :type reward: float
+        :param done: Whether the episode has ended.
+        :type done: bool
+        """
+        for node in reversed(search_path):
+            node.update_stats(reward)
+            if not done:
+                _, reward = self.actor_critic_net(node.state)
+                reward = reward.item()
+
+    def learn(self):
+        """
+        Train the agent.
+        """
+        self.train()
+
+    def train(self):
+        """
+        Train the agent.
+        """
+        self.total_reward = 0
+        for episode in range(self.max_episodes):
+            self.episode = episode
+            state = self.learn_reset()
+            # state = self.env.reset()
+
+            for t in range(self.max_timesteps):
+                state = self._check_state(state)
+                self.state_tensor = self.check_tensor(state).squeeze(0)
+                self.next_state, self.action, self.reward, self.done = self.select_action(
+                    self.state_tensor)
+
+                self.learn_check()
+
+                if self.done:
+                    # self.update()
+                    break
+
+                self.update()
+
+                state = self.next_state
+
+            self.episode += 1
+            # print(f"Episode: {self.episode}, Reward: {self.total_reward}")
+
+    def compute_loss(self, state, action, reward, next_state, done):
+        '''
+        This function computes the actor and critic loss using the provided state, action, reward, next_state, and done variables.
+        The actor loss is computed based on the policy gradient algorithm,
+        and the critic loss is computed as the mean squared error between the estimated value of the current state and the target value of the next state.
+
+        compute_loss() function computes the actor and critic loss values for the provided state, action, reward, next_state, and done variables.
+
+        The state parameter is the current state of the environment.
+        The action parameter is the action taken in the current state.
+        The reward parameter is the reward received for taking the action in the current state.
+        The next_state parameter is the state resulting from taking the action in the current state.
+        The done parameter is a flag indicating whether the episode has ended.
+
+        :param state: The current state of the environment.
+        :param action: The action taken in the current state.
+        :param reward: The reward received for taking the action in the current state.
+        :param next_state: The state resulting from taking the action in the current state.
+        :param done: A flag indicating whether the episode has ended.
+        :return: The computed actor and critic loss values.
+        '''
+
+        # Predict action probabilities and values
+        action_probs, values = self.actor_critic_net(state)
+
+        # Compute the value loss
+        target_values = reward + self.gamma * \
+            self.actor_critic_net(next_state)[1] * (1 - done)
+        critic_loss = F.mse_loss(values, target_values.detach())
+
+        # Compute the policy loss
+        m = Categorical(action_probs)
+        logprobs = m.log_prob(self.check_tensor(action))
+        actor_loss = -logprobs * (target_values - values).detach()
+
+        return actor_loss, critic_loss
+
+    def update(self):
+        '''
+        This function updates the network parameters using the optimizer and computed loss values.
+
+        update() function updates the network parameters using the optimizer and computed loss values.
+        It uses the compute_loss() function to compute the loss and the optimizer object to perform the optimization step.
+
+        This function does not take any parameters and does not return anything.
+
+        :return: None
+        '''
+
+        # Update the network
+        self.actor_critic_optimizer.zero_grad()
+        actor_loss, critic_loss = self.compute_loss(
+            self.state_tensor, self.action, self.reward, self.next_state, self.done)
+        loss = actor_loss + critic_loss
+        loss.backward()
+        self.actor_critic_optimizer.step()
+
+    def check_tensor(self, obj):
+        '''
+        This function checks if the provided object is a PyTorch tensor, and if not, converts it to a tensor.
+
+        check_tensor() function checks if the provided obj parameter is a PyTorch tensor.
+        If it is not a tensor, it converts it to a tensor using torch.FloatTensor().
+        If it is already a tensor, it simply returns the tensor.
+
+        The obj parameter is the object to check/convert to a PyTorch tensor.
+
+        The function returns the input object as a PyTorch tensor.
+
+        :param obj: The object to check/convert to a PyTorch tensor.
+        :return: The input object as a PyTorch tensor.
+        '''
+
+        if not torch.is_tensor(obj):
+            obj_tensor = torch.FloatTensor(obj)
+        else:
+            obj_tensor = obj
+        return obj_tensor
+
+    def save_model(self, file_name):
+        """
+        This function saves the model to the specified file.
+
+        :param file_name: The name of the file to save the model to.
+        :return: None
+        """
+        self.save(file_name)
+
+    def save(self, file_name):
+        """
+        This function saves the actor critic network to the specified file.
+
+        :param file_name: The name of the file to save the actor critic network to.
+        :return: None
+        """
+
+        self.save_actor_critic(file_name)
+
+    def load_model(self, file_name):
+        """
+        This function loads the model from the specified file.
+
+        :param file_name: The name of the file to load the model from.
+        :return: None
+        """
+        self.load(file_name)
+
+    def load(self, file_name):
+        """
+        This function loads the actor critic network from the specified file.
+
+        :param file_name: The name of the file to load the actor critic network from.
+        :return: None
+        """
+
+        self.load_actor_critic(file_name)
```

### Comparing `modular_rl-0.2.0/modular_rl/agents/ppo.py` & `modular_rl-0.2.1/modular_rl/agents/ppo.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,17 +200,17 @@
         if dist == None and self.dist:
             dist = self.dist
 
         step_output = self.env.step(action.item())
         step_output_num = len(step_output)
 
         if step_output_num == 4:
-            next_state, reward, is_done, _ = self.env.step(action.item())
+            next_state, reward, is_done, _ = step_output
         elif step_output_num == 5:
-            next_state, reward, is_done, _, _ = self.env.step(action.item())
+            next_state, reward, is_done, _, _ = step_output
 
         self.episode_reward += reward
         self.total_reward += reward
         self.prev_reward = reward
 
         state = self._check_state(state)
```

### Comparing `modular_rl-0.2.0/modular_rl/networks/actor_critic.py` & `modular_rl-0.2.1/modular_rl/networks/actor_critic.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-# -*- coding: utf-8 -*-
-"""
-ModularRL project
-
-Copyright (c) 2023 horrible
-
-This software includes the following third-party libraries:
-PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
-
-"""
-import torch.nn as nn
-
-
-class ActorCriticNetwork(nn.Module):
-    def __init__(self, state_dim, action_dim, hidden_size=256):
-        '''
-        This code defines a class ActorCriticNetwork that implements an actor-critic network using PyTorch.
-        The actor-critic algorithm is a popular reinforcement learning algorithm that is used to learn how to maximize rewards in an environment by having an agent interact with the environment.
-        This network takes as input the state and action dimensions, and the number of neurons in the hidden layers of both the actor and critic networks.
-        It then predicts state-value and action-value for the given input.
-
-        :param state_dim: (int) The dimensionality of the state space.
-        :param action_dim: (int) The dimensionality of the action space.
-        :param hidden_size: (int) The number of neurons in the hidden layers of both the actor and critic networks.
-        '''
-
-        super(ActorCriticNetwork, self).__init__()
-
-        # Actor network
-        self.actor = nn.Sequential(
-            nn.Linear(state_dim, hidden_size),
-            nn.ReLU(),
-            nn.Linear(hidden_size, action_dim),
-            nn.Softmax(dim=-1)
-        )
-
-        # Critic network
-        self.critic = nn.Sequential(
-            nn.Linear(state_dim, hidden_size),
-            nn.ReLU(),
-            nn.Linear(hidden_size, 1)
-        )
-
-    def forward(self, state):
-        '''
-        The forward method of this class takes a state tensor of shape (batch_size, state_dim) as input and returns the action probabilities and state value.
-        The :param comments provide additional information about the inputs to the functions.
-
-        :param state: (tensor) The input state tensor of shape (batch_size, state_dim).
-        '''
-        action_probs = self.actor(state)
-        value = self.critic(state)
-        return action_probs, value
+# -*- coding: utf-8 -*-
+"""
+ModularRL project
+
+Copyright (c) 2023 horrible
+
+This software includes the following third-party libraries:
+PyTorch  (BSD-Style License): https://pytorch.org/ - Copyright (c) Facebook.
+
+"""
+import torch.nn as nn
+
+
+class ActorCriticNetwork(nn.Module):
+    def __init__(self, state_dim, action_dim, hidden_size=256):
+        '''
+        This code defines a class ActorCriticNetwork that implements an actor-critic network using PyTorch.
+        The actor-critic algorithm is a popular reinforcement learning algorithm that is used to learn how to maximize rewards in an environment by having an agent interact with the environment.
+        This network takes as input the state and action dimensions, and the number of neurons in the hidden layers of both the actor and critic networks.
+        It then predicts state-value and action-value for the given input.
+
+        :param state_dim: (int) The dimensionality of the state space.
+        :param action_dim: (int) The dimensionality of the action space.
+        :param hidden_size: (int) The number of neurons in the hidden layers of both the actor and critic networks.
+        '''
+
+        super(ActorCriticNetwork, self).__init__()
+
+        # Actor network
+        self.actor = nn.Sequential(
+            nn.Linear(state_dim, hidden_size),
+            nn.ReLU(),
+            nn.Linear(hidden_size, action_dim),
+            nn.Softmax(dim=-1)
+        )
+
+        # Critic network
+        self.critic = nn.Sequential(
+            nn.Linear(state_dim, hidden_size),
+            nn.ReLU(),
+            nn.Linear(hidden_size, 1)
+        )
+
+    def forward(self, state):
+        '''
+        The forward method of this class takes a state tensor of shape (batch_size, state_dim) as input and returns the action probabilities and state value.
+        The :param comments provide additional information about the inputs to the functions.
+
+        :param state: (tensor) The input state tensor of shape (batch_size, state_dim).
+        '''
+        action_probs = self.actor(state)
+        value = self.critic(state)
+        return action_probs, value
```

### Comparing `modular_rl-0.2.0/modular_rl/networks/policy.py` & `modular_rl-0.2.1/modular_rl/networks/policy.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.2.0/modular_rl/networks/value.py` & `modular_rl-0.2.1/modular_rl/networks/value.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.2.0/modular_rl/params/mcts.py` & `modular_rl-0.2.1/modular_rl/params/mcts.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-class ParamMCTS:
-    default = {
-        'max_episodes': 10,  # Maximum number of episodes for training
-        'max_timesteps': 200,  # Maximum number of timesteps for each episode
-        'update_timestep': 2000,  # Update the policy every specified timestep
-        'networks': 'medium',  # Size of the hidden layer in neural networks
-        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
-        'num_simulations': 10,  # Number of MCTS simulations per move
-        'cpuct': 1.0,  # Exploration constant for MCTS
-        'temperature': 1.0,  # Temperature for action selection during MCTS
-        'gamma': 0.99,  # Discount factor
-        # If the average reward is greater than or equal to this value, training is stopped early
-        'early_stop_threshold': -1,
-        'done_loop_end': False,  # If True, end the episode when the done flag is set
-        'reward_print': True,  # If True, print the reward during training
-        'device': None,  # Device to run the model on, None for automatic selection
-        'log_level': 'debug',  # Log level for the logger
-        'log_init_pass': False,  # If True, skip logger initialization
-    }
-
-    default_modular = {
-        # Maximum number of episodes for training (-1 for no limit)
-        'max_episodes': -1,
-        # Maximum number of timesteps for each episode (-1 for no limit)
-        'max_timesteps': -1,
-        # Update the policy every specified timestep (-1 for no limit)
-        'update_timestep': -1,
-        'networks': 'medium',  # Size of the hidden layer in neural networks
-        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
-        'num_simulations': 800,  # Number of MCTS simulations per move
-        'cpuct': 1.0,  # Exploration constant for MCTS
-        'temperature': 1.0,  # Temperature for action selection during MCTS
-        'gamma': 0.99,  # Discount factor
-        # If the average reward is greater than or equal to this value, training is stopped early
-        'early_stop_threshold': -1,
-        'reward_print': True,  # If True, print the reward during training
-        'device': None,  # Device to run the model on, None for automatic selection
-        'log_level': 'debug',  # Log level for the logger
-        'log_init_pass': False,  # If True, skip logger initialization
-    }
+class ParamMCTS:
+    default = {
+        'max_episodes': 10,  # Maximum number of episodes for training
+        'max_timesteps': 200,  # Maximum number of timesteps for each episode
+        'update_timestep': 2000,  # Update the policy every specified timestep
+        'networks': 'medium',  # Size of the hidden layer in neural networks
+        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
+        'num_simulations': 10,  # Number of MCTS simulations per move
+        'cpuct': 1.0,  # Exploration constant for MCTS
+        'temperature': 1.0,  # Temperature for action selection during MCTS
+        'gamma': 0.99,  # Discount factor
+        # If the average reward is greater than or equal to this value, training is stopped early
+        'early_stop_threshold': -1,
+        'done_loop_end': False,  # If True, end the episode when the done flag is set
+        'reward_print': True,  # If True, print the reward during training
+        'device': None,  # Device to run the model on, None for automatic selection
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
+        'networks': 'medium',  # Size of the hidden layer in neural networks
+        'optimizer_speed': 3e-4,  # Learning rate for the optimizer
+        'num_simulations': 800,  # Number of MCTS simulations per move
+        'cpuct': 1.0,  # Exploration constant for MCTS
+        'temperature': 1.0,  # Temperature for action selection during MCTS
+        'gamma': 0.99,  # Discount factor
+        # If the average reward is greater than or equal to this value, training is stopped early
+        'early_stop_threshold': -1,
+        'reward_print': True,  # If True, print the reward during training
+        'device': None,  # Device to run the model on, None for automatic selection
+        'log_level': 'debug',  # Log level for the logger
+        'log_init_pass': False,  # If True, skip logger initialization
+    }
```

### Comparing `modular_rl-0.2.0/modular_rl/params/ppo.py` & `modular_rl-0.2.1/modular_rl/params/ppo.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-class ParamPPO:
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
-        'log_level': 'debug',  # Log level for the logger
-        'log_init_pass': False,  # If True, skip logger initialization
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
-        'log_level': 'debug',  # Log level for the logger
-        'log_init_pass': False,  # If True, skip logger initialization
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

### Comparing `modular_rl-0.2.0/modular_rl/settings.py` & `modular_rl-0.2.1/modular_rl/settings.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-'''
-The AgentSettings class is a configuration class used for setting up various reinforcement learning agents.
-
-It provides default values for various parameters used in the agents, such as the maximum number of episodes,
-maximum number of timesteps per episode, update timestep, network architecture, learning rate,
-discount factor, early stopping threshold, and whether to end training when the environment is done.
-
-The class currently supports PPO and MCTS algorithms, but it can be extended to include other algorithms in the future.
-The default dictionary provides default values for all parameters, while the modular version provides default values
-with more flexibility for specific use cases. These default values can be modified by passing in a dictionary of
-key-value pairs to the AgentSettings constructor.
-
-'''
-
-from modular_rl.params.ppo import ParamPPO
-from modular_rl.params.mcts import ParamMCTS
-
-
-class AgentSettings:
-    default_ppo = ParamPPO.default
-    default_ppo_modular = ParamPPO.default_modular
-    default_mcts = ParamMCTS.default
-    default_mcts_modular = ParamMCTS.default_modular
+'''
+The AgentSettings class is a configuration class used for setting up various reinforcement learning agents.
+
+It provides default values for various parameters used in the agents, such as the maximum number of episodes,
+maximum number of timesteps per episode, update timestep, network architecture, learning rate,
+discount factor, early stopping threshold, and whether to end training when the environment is done.
+
+The class currently supports PPO and MCTS algorithms, but it can be extended to include other algorithms in the future.
+The default dictionary provides default values for all parameters, while the modular version provides default values
+with more flexibility for specific use cases. These default values can be modified by passing in a dictionary of
+key-value pairs to the AgentSettings constructor.
+
+'''
+
+from modular_rl.params.ppo import ParamPPO
+from modular_rl.params.mcts import ParamMCTS
+
+
+class AgentSettings:
+    default_ppo = ParamPPO.default
+    default_ppo_modular = ParamPPO.default_modular
+    default_mcts = ParamMCTS.default
+    default_mcts_modular = ParamMCTS.default_modular
```

### Comparing `modular_rl-0.2.0/modular_rl/tester/ppo.py` & `modular_rl-0.2.1/modular_rl/tester/ppo.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.2.0/modular_rl/util/node.py` & `modular_rl-0.2.1/modular_rl/util/node.py`

 * *Files identical despite different names*

### Comparing `modular_rl-0.2.0/modular_rl.egg-info/SOURCES.txt` & `modular_rl-0.2.1/modular_rl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modular_rl-0.2.0/pyproject.toml` & `modular_rl-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "modular_rl"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="horrible", email="shinjpn1@gmail.com" },
 ]
 description = "ModularRL is a Python library for creating and training reinforcement learning agents using various algorithms. The library is designed to be easily customizable and modular, allowing users to quickly set up and train agents for various environments without being limited to a specific algorithm."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

