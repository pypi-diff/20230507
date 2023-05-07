# Comparing `tmp/openrlbenchmark-0.2.0b2.tar.gz` & `tmp/openrlbenchmark-0.2.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openrlbenchmark-0.2.0b2.tar", max compression
+gzip compressed data, was "openrlbenchmark-0.2.0b3.tar", max compression
```

## Comparing `openrlbenchmark-0.2.0b2.tar` & `openrlbenchmark-0.2.0b3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1087 2022-05-10 21:09:01.507394 openrlbenchmark-0.2.0b2/LICENSE
--rw-r--r--   0        0        0    17986 2023-05-05 19:43:33.380795 openrlbenchmark-0.2.0b2/README.md
--rw-r--r--   0        0        0       75 2022-12-25 01:21:13.410700 openrlbenchmark-0.2.0b2/openrlbenchmark/__init__.py
--rw-r--r--   0        0        0     1746 2023-05-05 13:12:27.589472 openrlbenchmark-0.2.0b2/openrlbenchmark/cache.py
--rw-r--r--   0        0        0     1746 2023-05-05 13:01:23.002773 openrlbenchmark-0.2.0b2/openrlbenchmark/cache_legacy.py
--rw-r--r--   0        0        0     6147 2023-05-01 14:06:32.647152 openrlbenchmark-0.2.0b2/openrlbenchmark/capped_hns.py
--rw-r--r--   0        0        0     6050 2023-04-04 00:37:30.606222 openrlbenchmark-0.2.0b2/openrlbenchmark/hns.py
--rw-r--r--   0        0        0     2178 2023-05-05 13:13:16.550687 openrlbenchmark-0.2.0b2/openrlbenchmark/offline_db.py
--rw-r--r--   0        0        0    19847 2023-05-05 20:43:14.490099 openrlbenchmark-0.2.0b2/openrlbenchmark/rlops.py
--rw-r--r--   0        0        0    29838 2023-05-05 20:43:14.498224 openrlbenchmark-0.2.0b2/openrlbenchmark/rlops_hns.py
--rw-r--r--   0        0        0      696 2023-05-05 20:43:39.223827 openrlbenchmark-0.2.0b2/pyproject.toml
--rw-r--r--   0        0        0    19471 1970-01-01 00:00:00.000000 openrlbenchmark-0.2.0b2/setup.py
--rw-r--r--   0        0        0    18949 1970-01-01 00:00:00.000000 openrlbenchmark-0.2.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1087 2022-05-10 21:09:01.507394 openrlbenchmark-0.2.0b3/LICENSE
+-rw-r--r--   0        0        0    17986 2023-05-05 19:43:33.380795 openrlbenchmark-0.2.0b3/README.md
+-rw-r--r--   0        0        0       75 2022-12-25 01:21:13.410700 openrlbenchmark-0.2.0b3/openrlbenchmark/__init__.py
+-rw-r--r--   0        0        0     1746 2023-05-05 13:12:27.589472 openrlbenchmark-0.2.0b3/openrlbenchmark/cache.py
+-rw-r--r--   0        0        0     1746 2023-05-05 13:01:23.002773 openrlbenchmark-0.2.0b3/openrlbenchmark/cache_legacy.py
+-rw-r--r--   0        0        0     6147 2023-05-01 14:06:32.647152 openrlbenchmark-0.2.0b3/openrlbenchmark/capped_hns.py
+-rw-r--r--   0        0        0     6050 2023-04-04 00:37:30.606222 openrlbenchmark-0.2.0b3/openrlbenchmark/hns.py
+-rw-r--r--   0        0        0     2178 2023-05-05 13:13:16.550687 openrlbenchmark-0.2.0b3/openrlbenchmark/offline_db.py
+-rw-r--r--   0        0        0    19969 2023-05-07 18:03:12.931345 openrlbenchmark-0.2.0b3/openrlbenchmark/rlops.py
+-rw-r--r--   0        0        0    29960 2023-05-07 18:03:12.931232 openrlbenchmark-0.2.0b3/openrlbenchmark/rlops_hns.py
+-rw-r--r--   0        0        0      696 2023-05-07 18:04:08.835973 openrlbenchmark-0.2.0b3/pyproject.toml
+-rw-r--r--   0        0        0    19471 1970-01-01 00:00:00.000000 openrlbenchmark-0.2.0b3/setup.py
+-rw-r--r--   0        0        0    18949 1970-01-01 00:00:00.000000 openrlbenchmark-0.2.0b3/PKG-INFO
```

### Comparing `openrlbenchmark-0.2.0b2/LICENSE` & `openrlbenchmark-0.2.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.0b2/README.md` & `openrlbenchmark-0.2.0b3/README.md`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.0b2/openrlbenchmark/cache.py` & `openrlbenchmark-0.2.0b3/openrlbenchmark/cache.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.0b2/openrlbenchmark/cache_legacy.py` & `openrlbenchmark-0.2.0b3/openrlbenchmark/cache_legacy.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.0b2/openrlbenchmark/capped_hns.py` & `openrlbenchmark-0.2.0b3/openrlbenchmark/capped_hns.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.0b2/openrlbenchmark/hns.py` & `openrlbenchmark-0.2.0b3/openrlbenchmark/hns.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.0b2/openrlbenchmark/offline_db.py` & `openrlbenchmark-0.2.0b3/openrlbenchmark/offline_db.py`

 * *Files identical despite different names*

### Comparing `openrlbenchmark-0.2.0b2/openrlbenchmark/rlops.py` & `openrlbenchmark-0.2.0b3/openrlbenchmark/rlops.py`

 * *Files 2% similar despite different names*

```diff
@@ -426,18 +426,20 @@
                 "custom_env_id_key": custom_env_id_key,
                 "custom_exp_name_key": custom_exp_name_key,
                 "metric": metric,
             },
             expand_all=True,
         )
         if f"{wandb_entity}/{wandb_project_name}" not in offline_dbs:
-            offline_db_path = os.path.join(
-                openrlbenchmark.__path__[0], "dataset", f"{wandb_entity}/{wandb_project_name}", "offline.sqlite"
+            offline_db_folder = os.path.join(
+                openrlbenchmark.__path__[0], "dataset", f"{wandb_entity}/{wandb_project_name}"
             )
+            offline_db_path = os.path.join(offline_db_folder, "offline.sqlite")
             print(offline_db_path)
+            os.makedirs(offline_db_folder, exist_ok=True)
             offline_db = pw.SqliteDatabase(offline_db_path)
             database_proxy.initialize(offline_db)
             offline_db.connect()
             offline_db.create_tables([OfflineRun, Tag, OfflineRunTag])
             offline_dbs[f"{wandb_entity}/{wandb_project_name}"] = offline_db
 
         for filter_str, color in zip(filters[1:], colors[filters_idx]):
```

### Comparing `openrlbenchmark-0.2.0b2/openrlbenchmark/rlops_hns.py` & `openrlbenchmark-0.2.0b3/openrlbenchmark/rlops_hns.py`

 * *Files 1% similar despite different names*

```diff
@@ -576,18 +576,20 @@
                 "custom_env_id_key": custom_env_id_key,
                 "custom_exp_name_key": custom_exp_name_key,
                 "metric": metric,
             },
             expand_all=True,
         )
         if f"{wandb_entity}/{wandb_project_name}" not in offline_dbs:
-            offline_db_path = os.path.join(
-                openrlbenchmark.__path__[0], "dataset", f"{wandb_entity}/{wandb_project_name}", "offline.sqlite"
+            offline_db_folder = os.path.join(
+                openrlbenchmark.__path__[0], "dataset", f"{wandb_entity}/{wandb_project_name}"
             )
+            offline_db_path = os.path.join(offline_db_folder, "offline.sqlite")
             print(offline_db_path)
+            os.makedirs(offline_db_folder, exist_ok=True)
             offline_db = pw.SqliteDatabase(offline_db_path)
             database_proxy.initialize(offline_db)
             offline_db.connect()
             offline_db.create_tables([OfflineRun, Tag, OfflineRunTag])
             offline_dbs[f"{wandb_entity}/{wandb_project_name}"] = offline_db
 
         for filter_str, color in zip(filters[1:], colors[filters_idx]):
```

### Comparing `openrlbenchmark-0.2.0b2/pyproject.toml` & `openrlbenchmark-0.2.0b3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openrlbenchmark"
-version = "0.2.0b2"
+version = "0.2.0b3"
 description = ""
 authors = ["Costa Huang <costa.huang@outlook.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.11"
 wandb = "^0.13.7"
```

### Comparing `openrlbenchmark-0.2.0b2/setup.py` & `openrlbenchmark-0.2.0b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'tqdm>=4.65.0,<5.0.0',
  'tueplots>=0.0.4,<0.0.5',
  'tyro>=0.5.0,<0.6.0',
  'wandb>=0.13.7,<0.14.0']
 
 setup_kwargs = {
     'name': 'openrlbenchmark',
-    'version': '0.2.0b2',
+    'version': '0.2.0b3',
     'description': '',
     'long_description': '# Open RL Benchmark: Comprehensive Tracked Experiments for Reinforcement Learning\n\n\n[<img src="https://img.shields.io/badge/license-MIT-blue">](https://github.com/vwxyzjn/cleanrl)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/openrlbenchmark/openrlbenchmark/blob/master/README.ipynb)\n[<img src="https://dcbadge.vercel.app/api/server/GsmqhDcea5?style=flat">](https://discord.gg/GsmqhDcea5)\n\n\n\nOpen RL Benchmark is a comprehensive collection of tracked experiments for RL. It aims to make it easier for RL practitioners to pull and compare all kinds of metrics from reputable RL libraries like Stable-baselines3, Tianshou, CleanRL, and others.\n\n* 💾 [GitHub Repo](https://github.com/openrlbenchmark/openrlbenchmark): source code and more docs.\n* 📜 [Design docs](https://docs.google.com/document/d/1cDI_AMr2QVmkC53dCHFMYwGJtLC8V4p6KdL2wnYPaiI/edit?usp=sharing): our motivation and vision.\n* 🔗 [Open RL Benchmark reports](https://wandb.ai/openrlbenchmark/openrlbenchmark/reportlist):  W&B reports with tracked Atari, MuJoCo experiments from SB3, CleanRL, and others.\n\n\n\n## Installation\nYou can install it via pip or the dev setup.\n\n### Pip install\n\n```shell\npip install openrlbenchmark --upgrade\n```\n\n### Dev Setup\n\nPrerequisites:\n* Python >=3.7.1,<3.10 (not yet 3.10)\n* [Poetry 1.2.1+](https://python-poetry.org)\n\n```shell\ngit clone https://github.com/openrlbenchmark/openrlbenchmark.git\ncd openrlbenchmark\npoetry install\n```\n\n\n## Get started\n\nOpen RL Benchmark provides an RLops CLI to pull and compare metrics from Weights and Biases. The following example shows how to compare the performance of SB3\'s ppo, a2c, ddpg, ppo_lstm, sac, td3, ppo, trpo, CleanRL\'s sac on `HalfCheetahBulletEnv-v0`.\n\n```shell\npython -m openrlbenchmark.rlops \\\n    --filters \'?we=openrlbenchmark&wpn=sb3&ceik=env&cen=algo&metric=rollout/ep_rew_mean\' \\\n        \'a2c\' \\\n        \'ddpg\' \\\n        \'ppo_lstm?cl=PPO w/ LSTM\' \\\n        \'sac\' \\\n        \'td3\' \\\n        \'ppo\' \\\n        \'trpo\' \\\n    --filters \'?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return\' \\\n        \'sac_continuous_action?tag=rlops-pilot&cl=SAC\' \\\n    --env-ids HalfCheetahBulletEnv-v0 \\\n    --pc.ncols 1 \\\n    --pc.ncols-legend 2 \\\n    --pc.xlabel \'Training Steps\' \\\n    --pc.ylabel \'Episodic Return\' \\\n    --output-filename compare \\\n    --report\n```\n\nHere, we created multiple filters. The first string in the first filter is `\'?we=openrlbenchmark&wpn=sb3&ceik=env&cen=algo&metric=rollout/ep_rew_mean\'`, which is a query string that specifies the following:\n\n* `we`: the W&B entity name\n* `wpn`: the W&B project name\n* `ceik`: the custom key for the environment id\n* `cen`: the custom key for the experiment name\n* `metric`: the metric we are interested in\n\nSo we are fetching metrics from [https://wandb.ai/openrlbenchmark/sb3](https://wandb.ai/openrlbenchmark/sb3). The environment id is stored in the `env` key, and the experiment name is stored in the `algo` key. The metric we are interested in is `rollout/ep_rew_mean`.\n\nSimilarly, we are fetching metrics from [https://wandb.ai/openrlbenchmark/cleanrl](https://wandb.ai/openrlbenchmark/cleanrl). The environment id is stored in the `env_id` key, and the experiment name is stored in the `exp_name` key. The metric we are interested in is `charts/episodic_return`. You can also customize the legend with the `cl` query string, such as `ppo_lstm?cl=PPO w/ LSTM`.\n\nThe labels of the figure can be customized with the `--pc.xlabel` and `--pc.ylabel` flags. The `--pc.ncols` flag specifies the number of columns in the figure. The `--pc.ncols-legend` flag specifies the number of columns in the legend. The `--output-filename` flag specifies the filename of the output figure\n\nThe command above generates the following plot:\n\n|    cleanrl vs. Stable Baselines 3   |    cleanrl vs. Stable Baselines 3 (Time)   |\n|:----------------------------------:|:----------------------------------------:|\n|  ![](static/cleanrl_vs_sb3.png)   |   ![](static/cleanrl_vs_sb3-time.png)   |\n\n\n\nThe `--report` tag also generates a [wandb report](https://wandb.ai/costa-huang/cleanrl/reports/Regression-Report-sac_continuous_action--VmlldzozMTY4NDQ3)\n\n\nThe command also generates a `compare.png`, a `compare.md`, and a `compare.csv` in the current directory.\n\n**Learning curves:** the `compare.png` shows the learning curves which subsamples 10000 data points and and interpolate. The curves are smoothed by a rolling average with a window size 100 and their shaded region represents the standard deviation.\n\n**Result table:** the `compare.md` and `compare.csv` shows the average episodic return of the last 100 episodes. For each random seed $i$ (we have 3 random seeds for each set of experiments), we calculate the average episodic return of the last 100 training episodes as $a_i$. We then average the $a_i$\'s over all random seeds to get the final average episodic return and report its standard deviation. This type of evaluation is known as an implicit evaluation method ([Machado et al., 2017](https://arxiv.org/pdf/1709.06009.pdf)) which aligns better with the general goal of RL which is continual learning. This method also detects issues with catastrophic forgetting compared to the evaluation method that evaluates the best model.\n\n\n> **Warning**\n> You may get slightly different curves every time you run the commands. This is because we sample 500 data points from the track experiments to save bandwidth. If you are using `openrlbenchmark` repeatedly or you wanto to generate consistent `compare.md` and learning curves, we recommend you to use `--scan-history` to get all of the data points, but initially it may take a while to run.\n\n\n## Currently supported libraries\n\n* [CleanRL](https://wandb.ai/openrlbenchmark/cleanrl)\n    * `ceik`: `env_id`\n    * `cen`: `exp_name` (e.g., `sac_continuous_action`, `ppo_continuous_action`, `ppo_atari`)\n    * `metric`: `charts/episodic_return`\n* [Stable-baselines3](https://wandb.ai/openrlbenchmark/sb3)\n    * `ceik`: `env`\n    * `cen`: `algo` (e.g., `sac`, `ppo`, `a2c`)\n    * `metric`: `rollout/ep_rew_mean` or `eval/mean_reward`\n* [ikostrikov/jaxrl](https://wandb.ai/openrlbenchmark/jaxrl)\n    * `ceik`: `env_name`\n    * `cen`: `algo` (e.g., `sac`)\n    * `metric`: `training/return` or `evaluation/average_returns`\n* [baselines](https://wandb.ai/openrlbenchmark/baselines)\n    * `ceik`: `env`\n    * `cen`: `alg` (e.g., `ppo2`)\n    * `metric`: `charts/episodic_return` or `eprewmean`\n* [sbx](https://wandb.ai/openrlbenchmark/sbx)\n    * `ceik`: `env`\n    * `cen`: `alg` (e.g., `sac`, `tqc`)\n    * `metric`: `rollout/ep_rew_mean` or `eval/mean_reward`\n* [Tianshou](https://wandb.ai/tianshou/atari.benchmark)\n    * `ceik`: `task`\n    * `cen`: `algo_name` (e.g., `ppo`, `iqn`)\n    * `metric`: `test/reward`\n* [MORL-Baselines](https://wandb.ai/openrlbenchmark/morl-baselines)\n    * `ceik`: `env_id`\n    * `cen`: `algo` (e.g., `PGMORL`, `PCN`)\n    * `metric`: `eval/hypervolume`, `eval/igd`, `eval/sparsity`, `eval/eum`, `eval/mul`\n\nThe following libraries have some recorded experiments:\n\n* [openai/phasic-policy-gradient](https://wandb.ai/openrlbenchmark/phasic-policy-gradient) (has some metrics)\n    * `ceik`: `env_name`\n    * `cen`: `arch` (`shared`)\n    * `metric`: `charts/episodic_return`\n* [sfujim/TD3](https://wandb.ai/openrlbenchmark/sfujim-TD3) (has some metrics)\n    * `ceik`: `env`\n    * `cen`: `policy` (e.g., `TD3`)\n    * `metric`: `charts/episodic_return`\n\n\n## More examples\n\n### Compare CleanRL\'s PPO with `openai/baselines`\'s PPO2 on Atari games:\n\nSometimes the same environments could have different names in different libraries. For example, `openai/baselines` uses `BreakoutNoFrameskip-v4` while [EnvPool](https://envpool.readthedocs.io/en/latest/env/atari.html) uses `Breakout-v5`. To compare the two libraries, we need to specify the `env_id` for `CleanRL` and `env` for `openai/baselines`. In this case, can specify the corresponding `env_ids` for each filter.\n\nFor Atari games, we have additional batteries included `openrlbenchmark.rlops_hns` to show human normalized-scores and further statistical analysis through [`rliable`](https://github.com/google-research/rliable).\n\n\n```shell\npython -m openrlbenchmark.rlops_hns \\\n    --filters \'?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return\' \'baselines-ppo2-cnn\' \\\n    --filters \'?we=openrlbenchmark&wpn=envpool-atari&ceik=env_id&cen=exp_name&metric=charts/avg_episodic_return\' \'ppo_atari_envpool_xla_jax_truncation\' \\\n    --env-ids AlienNoFrameskip-v4 AmidarNoFrameskip-v4 AssaultNoFrameskip-v4 AsterixNoFrameskip-v4 AsteroidsNoFrameskip-v4 AtlantisNoFrameskip-v4 BankHeistNoFrameskip-v4 BattleZoneNoFrameskip-v4 BeamRiderNoFrameskip-v4 BerzerkNoFrameskip-v4 BowlingNoFrameskip-v4 BoxingNoFrameskip-v4 BreakoutNoFrameskip-v4 CentipedeNoFrameskip-v4 ChopperCommandNoFrameskip-v4 CrazyClimberNoFrameskip-v4 DefenderNoFrameskip-v4 DemonAttackNoFrameskip-v4 DoubleDunkNoFrameskip-v4 EnduroNoFrameskip-v4 FishingDerbyNoFrameskip-v4 FreewayNoFrameskip-v4 FrostbiteNoFrameskip-v4 GopherNoFrameskip-v4 GravitarNoFrameskip-v4 HeroNoFrameskip-v4 IceHockeyNoFrameskip-v4 PrivateEyeNoFrameskip-v4 QbertNoFrameskip-v4 RiverraidNoFrameskip-v4 RoadRunnerNoFrameskip-v4 RobotankNoFrameskip-v4 SeaquestNoFrameskip-v4 SkiingNoFrameskip-v4 SolarisNoFrameskip-v4 SpaceInvadersNoFrameskip-v4 StarGunnerNoFrameskip-v4 SurroundNoFrameskip-v4 TennisNoFrameskip-v4 TimePilotNoFrameskip-v4 TutankhamNoFrameskip-v4 UpNDownNoFrameskip-v4 VentureNoFrameskip-v4 VideoPinballNoFrameskip-v4 WizardOfWorNoFrameskip-v4 YarsRevengeNoFrameskip-v4 ZaxxonNoFrameskip-v4 JamesbondNoFrameskip-v4 KangarooNoFrameskip-v4 KrullNoFrameskip-v4 KungFuMasterNoFrameskip-v4 MontezumaRevengeNoFrameskip-v4 MsPacmanNoFrameskip-v4 NameThisGameNoFrameskip-v4 PhoenixNoFrameskip-v4 PitfallNoFrameskip-v4 PongNoFrameskip-v4 \\\n    --env-ids Alien-v5 Amidar-v5 Assault-v5 Asterix-v5 Asteroids-v5 Atlantis-v5 BankHeist-v5 BattleZone-v5 BeamRider-v5 Berzerk-v5 Bowling-v5 Boxing-v5 Breakout-v5 Centipede-v5 ChopperCommand-v5 CrazyClimber-v5 Defender-v5 DemonAttack-v5 DoubleDunk-v5 Enduro-v5 FishingDerby-v5 Freeway-v5 Frostbite-v5 Gopher-v5 Gravitar-v5 Hero-v5 IceHockey-v5 PrivateEye-v5 Qbert-v5 Riverraid-v5 RoadRunner-v5 Robotank-v5 Seaquest-v5 Skiing-v5 Solaris-v5 SpaceInvaders-v5 StarGunner-v5 Surround-v5 Tennis-v5 TimePilot-v5 Tutankham-v5 UpNDown-v5 Venture-v5 VideoPinball-v5 WizardOfWor-v5 YarsRevenge-v5 Zaxxon-v5 Jamesbond-v5 Kangaroo-v5 Krull-v5 KungFuMaster-v5 MontezumaRevenge-v5 MsPacman-v5 NameThisGame-v5 Phoenix-v5 Pitfall-v5 Pong-v5 \\\n    --no-check-empty-runs \\\n    --pc.ncols 5 \\\n    --pc.ncols-legend 2 \\\n    --output-filename static/cleanrl_vs_baselines \\\n    --scan-history --rliable\n```\n\nIn the individual learning curves below, the right y-axis is the human normalized score. The left y-axis is the raw episodic return.\n![](static/cleanrl_vs_baselines.png) The script also generates `cleanrl_vs_baselines_hns_median.png`, the learning curves for median human-normalized scores. \n\nFurthermore, the `--rliable` integration generates `cleanrl_vs_baselines_iqm_profile.png`, the  Interquartile Mean (IQM) and performance profile ([Agarwal et al., 2022](https://arxiv.org/pdf/2108.13264.pdf)), and `cleanrl_vs_baselines_hns_aggregate.png`, the aggregate human-normalized scores with Stratified Bootstrap Confidence Intervals (see @araffin\'s excellent blog post [explainer](https://araffin.github.io/post/rliable/)). \n\n\n![](static/cleanrl_vs_baselines_hns_median.png)\n\n![](static/cleanrl_vs_baselines_iqm_profile.png)\n\n![](static/cleanrl_vs_baselines_hns_aggregate.png)\n\n\n### Offline mode\n\nSometimes even with caching `--scan-history` the script can still take a long time if there are too many environments or experiments. This is because we are still calling many `wandb.Api().runs(..., filters)` under the hood. \n\nNo worries though. When running with `--scan-history`, we also automatically build a local `sqlite` database to store the metadata of runs, enabling us to run the script without internet connection.\n\n```shell\npython -m openrlbenchmark.rlops \\\n    --filters \'?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return\' \'baselines-ppo2-mlp\' \\\n    --filters \'?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return\' \'ppo_continuous_action?tag=v1.0.0-27-gde3f410\' \\\n    --filters \'?we=openrlbenchmark&wpn=jaxrl&ceik=env_name&cen=algo&metric=training/return\' \'sac\' \\\n    --env-ids HalfCheetah-v2 Walker2d-v2 Hopper-v2 InvertedPendulum-v2 Humanoid-v2 Pusher-v2 \\\n    --no-check-empty-runs \\\n    --pc.ncols 3 \\\n    --pc.ncols-legend 3 \\\n    --output-filename static/baselines_vs_cleanrl_vs_jaxrl \\\n    --scan-history \\\n    --offline\n```\n\n### Compare CleanRL\'s PPO with `openai/baselines`\'s PPO2 and `jaxrl`\'s SAC on Mujoco:\n\n```shell\npython -m openrlbenchmark.rlops \\\n    --filters \'?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return\' \'baselines-ppo2-mlp\' \\\n    --filters \'?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return\' \'ppo_continuous_action?tag=v1.0.0-27-gde3f410\' \\\n    --filters \'?we=openrlbenchmark&wpn=jaxrl&ceik=env_name&cen=algo&metric=training/return\' \'sac\' \\\n    --env-ids HalfCheetah-v2 Walker2d-v2 Hopper-v2 InvertedPendulum-v2 Humanoid-v2 Pusher-v2 \\\n    --no-check-empty-runs \\\n    --pc.ncols 3 \\\n    --pc.ncols-legend 3 \\\n    --output-filename static/baselines_vs_cleanrl_vs_jaxrl \\\n    --scan-history\n```\n![](static/baselines_vs_cleanrl_vs_jaxrl.png)\n\n\n\n### Compare Tianshou\'s algorithms with `openai/baselines`\'s PPO2 on Atari:\n\n```shell\npython -m openrlbenchmark.rlops \\\n    --filters \'?we=tianshou&wpn=atari.benchmark&ceik=task&cen=algo_name&metric=test/reward\' \'iqn\' \'ppo\' \'rainbow\' \'fqf\' \'c51\' \'dqn\' \'qrdqn\' \\\n    --filters \'?we=openrlbenchmark&wpn=baselines&ceik=env&cen=exp_name&metric=charts/episodic_return\' \'baselines-ppo2-cnn\' \\\n    --env-ids BreakoutNoFrameskip-v4 SpaceInvadersNoFrameskip-v4 SeaquestNoFrameskip-v4 MsPacmanNoFrameskip-v4 EnduroNoFrameskip-v4 PongNoFrameskip-v4 QbertNoFrameskip-v4 \\\n    --no-check-empty-runs \\\n    --pc.ncols 4 \\\n    --pc.ncols-legend 4 \\\n    --output-filename static/baselines_vs_tianshou --scan-history\n```\n![](static/baselines_vs_tianshou.png)\n\n\n### Compare CleanRL\'s PPG and PPO with `openai/phasic-policy-gradient`\'s PPG on procgen:\n\n```shell\npython -m openrlbenchmark.rlops \\\n    --filters \'?we=openrlbenchmark&wpn=phasic-policy-gradient&ceik=env_name&cen=arch&metric=charts/episodic_return\' \'shared\' \\\n    --filters \'?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return\' \'ppo_procgen?tag=v1.0.0b1-4-g4ea73d9\' \'ppg_procgen?tag=v1.0.0b1-4-g4ea73d9\' \\\n    --env-ids starpilot bossfight bigfish \\\n    --no-check-empty-runs \\\n    --pc.ncols 3 \\\n    --pc.ncols-legend 3 \\\n    --output-filename static/ppg_vs_cleanrl \\\n    --scan-history\n```\n\n![](static/ppg_vs_cleanrl.png)\n\n\n### Compare CleanRL\'s TD3 with `sfujim/TD3`\'s TD3 on Mujoco:\n\n```shell\npython -m openrlbenchmark.rlops \\\n    --filters \'?we=openrlbenchmark&wpn=sfujim-TD3&ceik=env&cen=policy&metric=charts/episodic_return\' \'TD3\' \\\n    --filters \'?we=openrlbenchmark&wpn=cleanrl&ceik=env_id&cen=exp_name&metric=charts/episodic_return\' \'td3_continuous_action_jax?tag=pr-285\' \'ddpg_continuous_action_jax?tag=pr-298\' \\\n    --env-ids HalfCheetah-v2 Walker2d-v2 Hopper-v2 \\\n    --no-check-empty-runs \\\n    --pc.ncols 3 \\\n    --pc.ncols-legend 3 \\\n    --output-filename static/td3_vs_cleanrl \\\n    --scan-history\n```\n![](static/td3_vs_cleanrl.png)\n\n\n\n### Compare MORL Baselines algorithms on deterministic environments\n\n```shell\npython -m openrlbenchmark.rlops \\\n  --filters \'?we=openrlbenchmark&wpn=MORL-Baselines&ceik=env_id&cen=algo&metric=eval/hypervolume\' \\\n  \'Pareto Q-Learning?cl=Pareto Q-Learning\' \\\n  \'MultiPolicy MO Q-Learning?cl=MultiPolicy MO Q-Learning\' \\\n  \'MultiPolicy MO Q-Learning (OLS)?cl=MultiPolicy MO Q-Learning (OLS)\' \\\n  --env-ids deep-sea-treasure-v0 deep-sea-treasure-concave-v0 \\\n  --pc.ncols 2 \\\n  --pc.ncols-legend 1 \\\n  --pc.xlabel \'Training steps\' \\\n  --pc.ylabel \'Hypervolume\' \\\n  --output-filename morl_deterministic_envs \\\n  --scan-history\n```\n\n![](static/morl_deterministic_envs.png)\n![](static/morl_deterministic_envs-time.png)\n\n### Calculate human normalized scores\n\n```shell\npython -m openrlbenchmark.hns --files static/cleanrl_vs_baselines.csv static/machado_10M.csv static/machado_50M.csv \n```\n\n```\nbaselines-ppo2-cnn ({})\n┣━━ median hns: 0.7959851540635047\n┣━━ mean hns: 4.54588939893709\nppo_atari_envpool_xla_jax_truncation ({})\n┣━━ median hns: 0.9783505154639175\n┣━━ mean hns: 6.841083973256849\nppo_atari_envpool_xla_jax_truncation_machado_10M ({})\n┣━━ median hns: 0.7347972972972973\n┣━━ mean hns: 2.919095857954249\nppo_atari_envpool_xla_jax_truncation ({\'metric\': [\'charts/avg_episodic_return\']})\n┣━━ median hns: 0.9783505154639175\n┣━━ mean hns: 6.841083973256849\nppo_atari_envpool_xla_jax_truncation_machado ({\'metric\': [\'charts/avg_episodic_return\']})\n┣━━ median hns: 1.5679929625118418\n┣━━ mean hns: 8.352308370550299\n```\n\n## What\'s going on right now?\n\nThis is a project we are slowly working on. There is no specific timeline or roadmap, but if you want to get involved. Feel free to reach out to me or open an issue. We are looking for volunteers to help us with the following:\n\n* Add experiments from other libraries\n* Run more experiments from currently supported libraries\n* Documentation and designing standards\n* Download the tensorboard metrics from the tracked experiments and load them locally to save time\n\n',
     'author': 'Costa Huang',
     'author_email': 'costa.huang@outlook.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `openrlbenchmark-0.2.0b2/PKG-INFO` & `openrlbenchmark-0.2.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openrlbenchmark
-Version: 0.2.0b2
+Version: 0.2.0b3
 Summary: 
 Author: Costa Huang
 Author-email: costa.huang@outlook.com
 Requires-Python: >=3.7.1,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

