# Comparing `tmp/pyfmc-0.0.5.tar.gz` & `tmp/pyfmc-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfmc-0.0.5.tar", last modified: Sun May  7 08:19:05 2023, max compression
+gzip compressed data, was "pyfmc-0.0.6.tar", last modified: Sun May  7 12:51:13 2023, max compression
```

## Comparing `pyfmc-0.0.5.tar` & `pyfmc-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 08:19:05.810726 pyfmc-0.0.5/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1107 2023-05-07 08:19:05.810726 pyfmc-0.0.5/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      520 2023-05-06 14:11:21.000000 pyfmc-0.0.5/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 08:19:05.806726 pyfmc-0.0.5/pyfmc/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-06 14:11:21.000000 pyfmc-0.0.5/pyfmc/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 08:19:05.806726 pyfmc-0.0.5/pyfmc/common/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      395 2023-05-06 14:11:21.000000 pyfmc-0.0.5/pyfmc/common/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2023-05-06 14:11:21.000000 pyfmc-0.0.5/pyfmc/common/historical_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2023-05-06 14:11:21.000000 pyfmc-0.0.5/pyfmc/exceptions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 08:19:05.806726 pyfmc-0.0.5/pyfmc/simulations/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      266 2023-05-06 14:11:21.000000 pyfmc-0.0.5/pyfmc/simulations/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2700 2023-05-06 14:11:21.000000 pyfmc-0.0.5/pyfmc/simulations/gbm.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 08:19:05.810726 pyfmc-0.0.5/pyfmc.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1107 2023-05-07 08:19:05.000000 pyfmc-0.0.5/pyfmc.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      334 2023-05-07 08:19:05.000000 pyfmc-0.0.5/pyfmc.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-07 08:19:05.000000 pyfmc-0.0.5/pyfmc.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       54 2023-05-07 08:19:05.000000 pyfmc-0.0.5/pyfmc.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-05-07 08:19:05.000000 pyfmc-0.0.5/pyfmc.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-05-07 08:19:05.810726 pyfmc-0.0.5/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      714 2023-05-07 08:18:44.000000 pyfmc-0.0.5/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 12:51:13.352846 pyfmc-0.0.6/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1107 2023-05-07 12:51:13.352846 pyfmc-0.0.6/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      520 2023-05-06 14:11:21.000000 pyfmc-0.0.6/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 12:51:13.348846 pyfmc-0.0.6/pyfmc/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-06 14:11:21.000000 pyfmc-0.0.6/pyfmc/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 12:51:13.348846 pyfmc-0.0.6/pyfmc/common/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      395 2023-05-06 14:11:21.000000 pyfmc-0.0.6/pyfmc/common/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2023-05-06 14:11:21.000000 pyfmc-0.0.6/pyfmc/common/historical_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2023-05-06 14:11:21.000000 pyfmc-0.0.6/pyfmc/exceptions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 12:51:13.348846 pyfmc-0.0.6/pyfmc/simulations/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      266 2023-05-06 14:11:21.000000 pyfmc-0.0.6/pyfmc/simulations/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3332 2023-05-07 12:49:37.000000 pyfmc-0.0.6/pyfmc/simulations/gbm.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 12:51:13.352846 pyfmc-0.0.6/pyfmc.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1107 2023-05-07 12:51:13.000000 pyfmc-0.0.6/pyfmc.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      334 2023-05-07 12:51:13.000000 pyfmc-0.0.6/pyfmc.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-07 12:51:13.000000 pyfmc-0.0.6/pyfmc.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       54 2023-05-07 12:51:13.000000 pyfmc-0.0.6/pyfmc.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-05-07 12:51:13.000000 pyfmc-0.0.6/pyfmc.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-05-07 12:51:13.352846 pyfmc-0.0.6/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      695 2023-05-07 12:49:37.000000 pyfmc-0.0.6/setup.py
```

### Comparing `pyfmc-0.0.5/PKG-INFO` & `pyfmc-0.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfmc
-Version: 0.0.5
+Version: 0.0.6
 Summary: Finance Monte-Carlo Simulation using PyTorch
 Home-page: https://github.com/ethanlee928/pyfmc
 Author: Ethan Lee
 Author-email: ethan2000.el@gmail.com
 License: UNKNOWN
 Description: # Finance Monte-Carlo Simulation using PyTorch
```

### Comparing `pyfmc-0.0.5/README.md` & `pyfmc-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyfmc-0.0.5/pyfmc/common/historical_data.py` & `pyfmc-0.0.6/pyfmc/common/historical_data.py`

 * *Files identical despite different names*

### Comparing `pyfmc-0.0.5/pyfmc/simulations/gbm.py` & `pyfmc-0.0.6/pyfmc/simulations/gbm.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,68 +12,84 @@
 from ..common import HistoricalData, get_device
 
 logger = logging.getLogger("pyfmc.simulations.gbm")
 
 
 class GBMResult:
     def __init__(
-        self, init_dist: torch.Tensor, final_dist: torch.Tensor, trajectory: Optional[torch.Tensor] = None
+        self, init_dist: torch.Tensor, final_dist: torch.Tensor, trajectories: Optional[torch.Tensor] = None
     ) -> None:
         self.init_dist = init_dist.cpu()
         self.final_dist = final_dist.cpu()
-        self.trajectory = trajectory.cpu() if trajectory is not None else trajectory
+        self._trajectories = trajectories.cpu() if trajectories is not None else trajectories
 
     def price_distribution(self):
         return self.final_dist.numpy()
 
+    def trajectories(self):
+        if self._trajectories is None:
+            logger.warning("No trajectories")
+            return
+        return self._trajectories.numpy()
+
     def return_distribution(self):
         return torch.div(torch.sub(self.final_dist, self.init_dist), self.init_dist).numpy()
 
     def VaR(self, alpha: float):
         return np.percentile(self.return_distribution(), alpha)
 
 
 class GBM(Simulations):
     def __init__(
         self,
         df: pd.DataFrame,
         n_walkers: int,
         n_steps: int,
+        n_trajectories: int = 0,
         step_size: float = 1,
         open_index: str = "Open",
         close_index: str = "Close",
         device_acc: bool = False,
     ) -> None:
         super().__init__(n_walkers, n_steps, device_acc)
         self.df = df
         self.step_size = step_size
         self.open_index = open_index
         self.close_index = close_index
+        self.n_trajectories = n_trajectories
         if (open_index and close_index) not in df.columns:
             raise SimulationException("Wrong open_index or close_index")
 
     def simulate(self):
         hist_data = HistoricalData(self.df, self.open_index, self.close_index)
         device = get_device() if self.device_acc else torch.device("cpu")
         logger.info("Using device: %s", device)
 
         exp_return = torch.tensor(hist_data.return_mean, device=device)
         std_return = torch.tensor(hist_data.return_std, device=device)
         last_price = hist_data.get_latest_close_price()
 
         s0 = torch.tensor([last_price for _ in range(self.n_walkers)], device=device)
         init_dist = torch.clone(s0)
+        trajectories = init_dist[: self.n_trajectories] if self.n_trajectories > 0 else None
+
         s1 = torch.zeros(self.n_walkers, device=device)
         ds = torch.zeros(self.n_walkers, device=device)
         dt = torch.tensor(self.step_size)
 
         for _ in trange(self.n_steps):
             epsilon = torch.randn(self.n_walkers, device=device)
             shock = torch.multiply(std_return * sqrt(dt), epsilon)
             drift = torch.multiply(dt, exp_return)
             _sum = torch.add(shock, drift)
             ds = torch.multiply(_sum, s0)
             s1 = torch.add(s0, ds)
             s0 = torch.clone(s1)
+            if self.n_trajectories > 0:
+                trajectories = torch.concat((trajectories, s0[: self.n_trajectories]))
 
         s0 = s0[torch.isfinite(s0)]
-        return GBMResult(init_dist, s0)
+        return GBMResult(
+            init_dist,
+            s0,
+            trajectories.reshape([self.n_steps + 1, self.n_trajectories]) if self.n_trajectories > 0 else None,
+        )
```

### Comparing `pyfmc-0.0.5/pyfmc.egg-info/PKG-INFO` & `pyfmc-0.0.6/pyfmc.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfmc
-Version: 0.0.5
+Version: 0.0.6
 Summary: Finance Monte-Carlo Simulation using PyTorch
 Home-page: https://github.com/ethanlee928/pyfmc
 Author: Ethan Lee
 Author-email: ethan2000.el@gmail.com
 License: UNKNOWN
 Description: # Finance Monte-Carlo Simulation using PyTorch
```

### Comparing `pyfmc-0.0.5/setup.py` & `pyfmc-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import os
 from setuptools import setup, find_packages
 
 
 setup(
     name="pyfmc",
-    version=os.getenv("VER"),
+    version="0.0.6",
     author="Ethan Lee",
     author_email="ethan2000.el@gmail.com",
     description="Finance Monte-Carlo Simulation using PyTorch",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     packages=find_packages("."),
     package_dir={"": "."},
```

