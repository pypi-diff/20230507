# Comparing `tmp/alns-5.0.4.tar.gz` & `tmp/alns-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alns-5.0.4.tar", max compression
+gzip compressed data, was "alns-5.1.0.tar", max compression
```

## Comparing `alns-5.0.4.tar` & `alns-5.1.0.tar`

### file list

```diff
@@ -1,60 +1,59 @@
--rw-r--r--   0        0        0     1095 2023-01-19 15:43:49.611467 alns-5.0.4/LICENSE.md
--rw-r--r--   0        0        0     4494 2023-01-19 15:43:49.611467 alns-5.0.4/README.md
--rw-r--r--   0        0        0    11290 2023-01-19 15:43:49.611467 alns-5.0.4/alns/ALNS.py
--rw-r--r--   0        0        0      495 2023-01-19 15:43:49.611467 alns-5.0.4/alns/Outcome.py
--rw-r--r--   0        0        0     5366 2023-01-19 15:43:49.611467 alns-5.0.4/alns/Result.py
--rw-r--r--   0        0        0      361 2023-01-19 15:43:49.611467 alns-5.0.4/alns/State.py
--rw-r--r--   0        0        0     3975 2023-01-19 15:43:49.611467 alns-5.0.4/alns/Statistics.py
--rw-r--r--   0        0        0       89 2023-01-19 15:43:49.611467 alns-5.0.4/alns/__init__.py
--rw-r--r--   0        0        0      940 2023-01-19 15:43:49.611467 alns-5.0.4/alns/accept/AcceptanceCriterion.py
--rw-r--r--   0        0        0     1943 2023-01-19 15:43:49.611467 alns-5.0.4/alns/accept/GreatDeluge.py
--rw-r--r--   0        0        0      363 2023-01-19 15:43:49.611467 alns-5.0.4/alns/accept/HillClimbing.py
--rw-r--r--   0        0        0     2567 2023-01-19 15:43:49.611467 alns-5.0.4/alns/accept/LateAcceptanceHillClimbing.py
--rw-r--r--   0        0        0     3545 2023-01-19 15:43:49.611467 alns-5.0.4/alns/accept/NonLinearGreatDeluge.py
--rw-r--r--   0        0        0      266 2023-01-19 15:43:49.611467 alns-5.0.4/alns/accept/RandomWalk.py
--rw-r--r--   0        0        0     6167 2023-01-19 15:43:49.611467 alns-5.0.4/alns/accept/RecordToRecordTravel.py
--rw-r--r--   0        0        0     6485 2023-01-19 15:43:49.611467 alns-5.0.4/alns/accept/SimulatedAnnealing.py
--rw-r--r--   0        0        0     2299 2023-01-19 15:43:49.611467 alns-5.0.4/alns/accept/WorseAccept.py
--rw-r--r--   0        0        0      429 2023-01-19 15:43:49.611467 alns-5.0.4/alns/accept/__init__.py
--rw-r--r--   0        0        0        0 2023-01-19 15:43:49.611467 alns-5.0.4/alns/accept/tests/__init__.py
--rw-r--r--   0        0        0     2311 2023-01-19 15:43:49.611467 alns-5.0.4/alns/accept/tests/test_great_deluge.py
--rw-r--r--   0        0        0      820 2023-01-19 15:43:49.611467 alns-5.0.4/alns/accept/tests/test_hill_climbing.py
--rw-r--r--   0        0        0     6012 2023-01-19 15:43:49.611467 alns-5.0.4/alns/accept/tests/test_late_acceptance_hill_climbing.py
--rw-r--r--   0        0        0     3452 2023-01-19 15:43:49.611467 alns-5.0.4/alns/accept/tests/test_non_linear_great_deluge.py
--rw-r--r--   0        0        0      790 2023-01-19 15:43:49.611467 alns-5.0.4/alns/accept/tests/test_random_walk.py
--rw-r--r--   0        0        0     5022 2023-01-19 15:43:49.611467 alns-5.0.4/alns/accept/tests/test_record_to_record_travel.py
--rw-r--r--   0        0        0     7119 2023-01-19 15:43:49.611467 alns-5.0.4/alns/accept/tests/test_simulated_annealing.py
--rw-r--r--   0        0        0     1947 2023-01-19 15:43:49.615468 alns-5.0.4/alns/accept/tests/test_threshold_accept.py
--rw-r--r--   0        0        0     1161 2023-01-19 15:43:49.615468 alns-5.0.4/alns/accept/tests/test_update.py
--rw-r--r--   0        0        0     4361 2023-01-19 15:43:49.615468 alns-5.0.4/alns/accept/tests/test_worse_accept.py
--rw-r--r--   0        0        0      907 2023-01-19 15:43:49.615468 alns-5.0.4/alns/accept/update.py
--rw-r--r--   0        0        0     5249 2023-01-19 15:43:49.615468 alns-5.0.4/alns/select/AlphaUCB.py
--rw-r--r--   0        0        0     3516 2023-01-19 15:43:49.615468 alns-5.0.4/alns/select/OperatorSelectionScheme.py
--rw-r--r--   0        0        0      635 2023-01-19 15:43:49.615468 alns-5.0.4/alns/select/RandomSelect.py
--rw-r--r--   0        0        0     5090 2023-01-19 15:43:49.615468 alns-5.0.4/alns/select/RouletteWheel.py
--rw-r--r--   0        0        0     3598 2023-01-19 15:43:49.615468 alns-5.0.4/alns/select/SegmentedRouletteWheel.py
--rw-r--r--   0        0        0      231 2023-01-19 15:43:49.615468 alns-5.0.4/alns/select/__init__.py
--rw-r--r--   0        0        0        0 2023-01-19 15:43:49.615468 alns-5.0.4/alns/select/tests/__init__.py
--rw-r--r--   0        0        0     2358 2023-01-19 15:43:49.615468 alns-5.0.4/alns/select/tests/test_alpha_ucb.py
--rw-r--r--   0        0        0     2180 2023-01-19 15:43:49.615468 alns-5.0.4/alns/select/tests/test_random_select.py
--rw-r--r--   0        0        0     3871 2023-01-19 15:43:49.615468 alns-5.0.4/alns/select/tests/test_roulette_wheel.py
--rw-r--r--   0        0        0     2754 2023-01-19 15:43:49.615468 alns-5.0.4/alns/select/tests/test_segmented_roulette_wheel.py
--rw-r--r--   0        0        0     1073 2023-01-19 15:43:49.615468 alns-5.0.4/alns/show_versions.py
--rw-r--r--   0        0        0      740 2023-01-19 15:43:49.615468 alns-5.0.4/alns/stop/MaxIterations.py
--rw-r--r--   0        0        0      846 2023-01-19 15:43:49.615468 alns-5.0.4/alns/stop/MaxRuntime.py
--rw-r--r--   0        0        0     1090 2023-01-19 15:43:49.615468 alns-5.0.4/alns/stop/NoImprovement.py
--rw-r--r--   0        0        0      724 2023-01-19 15:43:49.615468 alns-5.0.4/alns/stop/StoppingCriterion.py
--rw-r--r--   0        0        0      166 2023-01-19 15:43:49.615468 alns-5.0.4/alns/stop/__init__.py
--rw-r--r--   0        0        0        0 2023-01-19 15:43:49.615468 alns-5.0.4/alns/stop/tests/__init__.py
--rw-r--r--   0        0        0     1290 2023-01-19 15:43:49.615468 alns-5.0.4/alns/stop/tests/test_max_iterations.py
--rw-r--r--   0        0        0     1811 2023-01-19 15:43:49.615468 alns-5.0.4/alns/stop/tests/test_max_runtime.py
--rw-r--r--   0        0        0     2431 2023-01-19 15:43:49.615468 alns-5.0.4/alns/stop/tests/test_no_improvement.py
--rw-r--r--   0        0        0        0 2023-01-19 15:43:49.615468 alns-5.0.4/alns/tests/__init__.py
--rw-r--r--   0        0        0      385 2023-01-19 15:43:49.615468 alns-5.0.4/alns/tests/conftest.py
--rw-r--r--   0        0        0      387 2023-01-19 15:43:49.615468 alns-5.0.4/alns/tests/states.py
--rw-r--r--   0        0        0    10367 2023-01-19 15:43:49.615468 alns-5.0.4/alns/tests/test_alns.py
--rw-r--r--   0        0        0     6962 2023-01-19 15:43:49.615468 alns-5.0.4/alns/tests/test_result.py
--rw-r--r--   0        0        0     2796 2023-01-19 15:43:49.615468 alns-5.0.4/alns/tests/test_statistics.py
--rw-r--r--   0        0        0     2216 2023-01-19 15:43:49.631468 alns-5.0.4/pyproject.toml
--rw-r--r--   0        0        0     5424 1970-01-01 00:00:00.000000 alns-5.0.4/setup.py
--rw-r--r--   0        0        0     5841 1970-01-01 00:00:00.000000 alns-5.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-05-07 11:05:53.026157 alns-5.1.0/LICENSE.md
+-rw-r--r--   0        0        0     5392 2023-05-07 11:05:53.026157 alns-5.1.0/README.md
+-rw-r--r--   0        0        0    11418 2023-05-07 11:05:53.026157 alns-5.1.0/alns/ALNS.py
+-rw-r--r--   0        0        0      495 2023-05-07 11:05:53.026157 alns-5.1.0/alns/Outcome.py
+-rw-r--r--   0        0        0     5366 2023-05-07 11:05:53.026157 alns-5.1.0/alns/Result.py
+-rw-r--r--   0        0        0      299 2023-05-07 11:05:53.026157 alns-5.1.0/alns/State.py
+-rw-r--r--   0        0        0     3975 2023-05-07 11:05:53.026157 alns-5.1.0/alns/Statistics.py
+-rw-r--r--   0        0        0       89 2023-05-07 11:05:53.026157 alns-5.1.0/alns/__init__.py
+-rw-r--r--   0        0        0      885 2023-05-07 11:05:53.026157 alns-5.1.0/alns/accept/AcceptanceCriterion.py
+-rw-r--r--   0        0        0     1857 2023-05-07 11:05:53.026157 alns-5.1.0/alns/accept/GreatDeluge.py
+-rw-r--r--   0        0        0      276 2023-05-07 11:05:53.026157 alns-5.1.0/alns/accept/HillClimbing.py
+-rw-r--r--   0        0        0     2481 2023-05-07 11:05:53.026157 alns-5.1.0/alns/accept/LateAcceptanceHillClimbing.py
+-rw-r--r--   0        0        0     3545 2023-05-07 11:05:53.026157 alns-5.1.0/alns/accept/NonLinearGreatDeluge.py
+-rw-r--r--   0        0        0      179 2023-05-07 11:05:53.026157 alns-5.1.0/alns/accept/RandomWalk.py
+-rw-r--r--   0        0        0     6082 2023-05-07 11:05:53.026157 alns-5.1.0/alns/accept/RecordToRecordTravel.py
+-rw-r--r--   0        0        0     6400 2023-05-07 11:05:53.026157 alns-5.1.0/alns/accept/SimulatedAnnealing.py
+-rw-r--r--   0        0        0     2214 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/WorseAccept.py
+-rw-r--r--   0        0        0      429 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/tests/__init__.py
+-rw-r--r--   0        0        0     2311 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/tests/test_great_deluge.py
+-rw-r--r--   0        0        0      820 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/tests/test_hill_climbing.py
+-rw-r--r--   0        0        0     6012 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/tests/test_late_acceptance_hill_climbing.py
+-rw-r--r--   0        0        0     3452 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/tests/test_non_linear_great_deluge.py
+-rw-r--r--   0        0        0      790 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/tests/test_random_walk.py
+-rw-r--r--   0        0        0     5022 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/tests/test_record_to_record_travel.py
+-rw-r--r--   0        0        0     7119 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/tests/test_simulated_annealing.py
+-rw-r--r--   0        0        0     1947 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/tests/test_threshold_accept.py
+-rw-r--r--   0        0        0     1161 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/tests/test_update.py
+-rw-r--r--   0        0        0     4361 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/tests/test_worse_accept.py
+-rw-r--r--   0        0        0      907 2023-05-07 11:05:53.030156 alns-5.1.0/alns/accept/update.py
+-rw-r--r--   0        0        0     5249 2023-05-07 11:05:53.030156 alns-5.1.0/alns/select/AlphaUCB.py
+-rw-r--r--   0        0        0     3516 2023-05-07 11:05:53.030156 alns-5.1.0/alns/select/OperatorSelectionScheme.py
+-rw-r--r--   0        0        0      635 2023-05-07 11:05:53.030156 alns-5.1.0/alns/select/RandomSelect.py
+-rw-r--r--   0        0        0     5090 2023-05-07 11:05:53.030156 alns-5.1.0/alns/select/RouletteWheel.py
+-rw-r--r--   0        0        0     3598 2023-05-07 11:05:53.030156 alns-5.1.0/alns/select/SegmentedRouletteWheel.py
+-rw-r--r--   0        0        0      231 2023-05-07 11:05:53.030156 alns-5.1.0/alns/select/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 11:05:53.030156 alns-5.1.0/alns/select/tests/__init__.py
+-rw-r--r--   0        0        0     2358 2023-05-07 11:05:53.030156 alns-5.1.0/alns/select/tests/test_alpha_ucb.py
+-rw-r--r--   0        0        0     2180 2023-05-07 11:05:53.030156 alns-5.1.0/alns/select/tests/test_random_select.py
+-rw-r--r--   0        0        0     3871 2023-05-07 11:05:53.030156 alns-5.1.0/alns/select/tests/test_roulette_wheel.py
+-rw-r--r--   0        0        0     2754 2023-05-07 11:05:53.030156 alns-5.1.0/alns/select/tests/test_segmented_roulette_wheel.py
+-rw-r--r--   0        0        0      842 2023-05-07 11:05:53.030156 alns-5.1.0/alns/show_versions.py
+-rw-r--r--   0        0        0      663 2023-05-07 11:05:53.030156 alns-5.1.0/alns/stop/MaxIterations.py
+-rw-r--r--   0        0        0      769 2023-05-07 11:05:53.030156 alns-5.1.0/alns/stop/MaxRuntime.py
+-rw-r--r--   0        0        0     1013 2023-05-07 11:05:53.030156 alns-5.1.0/alns/stop/NoImprovement.py
+-rw-r--r--   0        0        0      669 2023-05-07 11:05:53.030156 alns-5.1.0/alns/stop/StoppingCriterion.py
+-rw-r--r--   0        0        0      166 2023-05-07 11:05:53.030156 alns-5.1.0/alns/stop/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 11:05:53.030156 alns-5.1.0/alns/stop/tests/__init__.py
+-rw-r--r--   0        0        0     1290 2023-05-07 11:05:53.030156 alns-5.1.0/alns/stop/tests/test_max_iterations.py
+-rw-r--r--   0        0        0     1811 2023-05-07 11:05:53.030156 alns-5.1.0/alns/stop/tests/test_max_runtime.py
+-rw-r--r--   0        0        0     2431 2023-05-07 11:05:53.030156 alns-5.1.0/alns/stop/tests/test_no_improvement.py
+-rw-r--r--   0        0        0        0 2023-05-07 11:05:53.030156 alns-5.1.0/alns/tests/__init__.py
+-rw-r--r--   0        0        0      385 2023-05-07 11:05:53.030156 alns-5.1.0/alns/tests/conftest.py
+-rw-r--r--   0        0        0      355 2023-05-07 11:05:53.030156 alns-5.1.0/alns/tests/states.py
+-rw-r--r--   0        0        0    10367 2023-05-07 11:05:53.030156 alns-5.1.0/alns/tests/test_alns.py
+-rw-r--r--   0        0        0     6962 2023-05-07 11:05:53.030156 alns-5.1.0/alns/tests/test_result.py
+-rw-r--r--   0        0        0     2796 2023-05-07 11:05:53.030156 alns-5.1.0/alns/tests/test_statistics.py
+-rw-r--r--   0        0        0     2664 2023-05-07 11:05:53.050156 alns-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6690 1970-01-01 00:00:00.000000 alns-5.1.0/PKG-INFO
```

### Comparing `alns-5.0.4/LICENSE.md` & `alns-5.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/ALNS.py` & `alns-5.1.0/alns/ALNS.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 import logging
 import time
-from typing import Callable, Dict, List, Optional, Tuple
+from typing import Dict, List, Optional, Protocol, Tuple
 
 import numpy.random as rnd
 
 from alns.Outcome import Outcome
 from alns.Result import Result
 from alns.State import State
 from alns.Statistics import Statistics
 from alns.accept import AcceptanceCriterion
 from alns.select import OperatorSelectionScheme
 from alns.stop import StoppingCriterion
 
-# TODO these should become Protocol to allow for kwargs. See also this issue:
-#  https://stackoverflow.com/q/61569324/4316405.
-_OperatorType = Callable[[State, rnd.RandomState], State]
-_CallbackType = Callable[[State, rnd.RandomState], None]
+
+class _OperatorType(Protocol):
+    __name__: str
+
+    def __call__(
+        self,
+        state: State,
+        rnd_state: rnd.RandomState,
+        **kwargs,
+    ) -> State:
+        pass  # pragma: no cover
+
+
+class _CallbackType(Protocol):
+    __name__: str
+
+    def __call__(self, state: State, rnd_state: rnd.RandomState, **kwargs):
+        pass  # pragma: no cover
+
 
 logger = logging.getLogger(__name__)
 
 
 class ALNS:
     """
     Implements the adaptive large neighbourhood search (ALNS) algorithm.
```

### Comparing `alns-5.0.4/alns/Result.py` & `alns-5.1.0/alns/Result.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/Statistics.py` & `alns-5.1.0/alns/Statistics.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/accept/AcceptanceCriterion.py` & `alns-5.1.0/alns/accept/AcceptanceCriterion.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-from abc import ABC, abstractmethod
+from typing import Protocol
 
 from numpy.random import RandomState
 
 from alns.State import State
 
 
-class AcceptanceCriterion(ABC):
+class AcceptanceCriterion(Protocol):
     """
-    Base class describing an acceptance criterion.
+    Protocol describing an acceptance criterion.
     """
 
-    @abstractmethod
     def __call__(
         self, rnd: RandomState, best: State, current: State, candidate: State
     ) -> bool:
         """
         Determines whether to accept the proposed, candidate solution based on
         this acceptance criterion and the other solution states.
 
@@ -30,8 +29,7 @@
             The proposed solution state.
 
         Returns
         -------
         bool
             Whether to accept the candidate state (True), or not (False).
         """
-        return NotImplemented
```

### Comparing `alns-5.0.4/alns/accept/GreatDeluge.py` & `alns-5.1.0/alns/accept/GreatDeluge.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from typing import Optional
 
-from alns.accept.AcceptanceCriterion import AcceptanceCriterion
 
-
-class GreatDeluge(AcceptanceCriterion):
+class GreatDeluge:
     """
     The Great Deluge (GD) criterion accepts solutions if the candidate solution
     has a value lower than a threshold (originally called the water level [1]).
     The initial threshold is computed as
 
     ``threshold = alpha * initial.objective()``
```

### Comparing `alns-5.0.4/alns/accept/LateAcceptanceHillClimbing.py` & `alns-5.1.0/alns/accept/LateAcceptanceHillClimbing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from collections import deque
 
-from alns.accept.AcceptanceCriterion import AcceptanceCriterion
 
-
-class LateAcceptanceHillClimbing(AcceptanceCriterion):
+class LateAcceptanceHillClimbing:
     """
     The Late Acceptance Hill Climbing (LAHC) criterion accepts a candidate
     solution when it is better than the current solution from a number of
     iterations ago.
 
     This implementation is based on the description of LAHC in [1].
```

### Comparing `alns-5.0.4/alns/accept/NonLinearGreatDeluge.py` & `alns-5.1.0/alns/accept/NonLinearGreatDeluge.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/accept/RecordToRecordTravel.py` & `alns-5.1.0/alns/accept/RecordToRecordTravel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import logging
 
-from alns.accept.AcceptanceCriterion import AcceptanceCriterion
 from alns.accept.update import update
 
 logger = logging.getLogger(__name__)
 
 
-class RecordToRecordTravel(AcceptanceCriterion):
+class RecordToRecordTravel:
     """
     The Record-to-Record Travel (RRT) criterion accepts a candidate solution
     if the absolute gap between the candidate and the best or current solution
     is smaller than a threshold. The threshold :math:`T` is updated in each
     iteration using a step size :math:`\\gamma`, as:
 
     .. math::
```

### Comparing `alns-5.0.4/alns/accept/SimulatedAnnealing.py` & `alns-5.1.0/alns/accept/SimulatedAnnealing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import logging
 
 import numpy as np
 
-from alns.accept.AcceptanceCriterion import AcceptanceCriterion
 from alns.accept.update import update
 
 logger = logging.getLogger(__name__)
 
 
-class SimulatedAnnealing(AcceptanceCriterion):
+class SimulatedAnnealing:
     R"""
     Simulated annealing, using an updating temperature.
 
     A candidate solution :math:`s^c` is compared against the current solution
     :math:`s`. The probability of accepting :math:`s^c` is given by
 
     .. math::
```

### Comparing `alns-5.0.4/alns/accept/WorseAccept.py` & `alns-5.1.0/alns/accept/WorseAccept.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from alns.accept.AcceptanceCriterion import AcceptanceCriterion
 from alns.accept.update import update
 
 
-class WorseAccept(AcceptanceCriterion):
+class WorseAccept:
     """
     The Worse Accept criterion accepts a candidate solution if it improves over
     the current one, or with a given probability :math:`P` regardless of the
     cost. :math:`P` is updated in each iteration as:
 
     .. math::
```

### Comparing `alns-5.0.4/alns/accept/tests/test_great_deluge.py` & `alns-5.1.0/alns/accept/tests/test_great_deluge.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/accept/tests/test_hill_climbing.py` & `alns-5.1.0/alns/accept/tests/test_hill_climbing.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/accept/tests/test_late_acceptance_hill_climbing.py` & `alns-5.1.0/alns/accept/tests/test_late_acceptance_hill_climbing.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/accept/tests/test_non_linear_great_deluge.py` & `alns-5.1.0/alns/accept/tests/test_non_linear_great_deluge.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/accept/tests/test_random_walk.py` & `alns-5.1.0/alns/accept/tests/test_random_walk.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/accept/tests/test_record_to_record_travel.py` & `alns-5.1.0/alns/accept/tests/test_record_to_record_travel.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/accept/tests/test_simulated_annealing.py` & `alns-5.1.0/alns/accept/tests/test_simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/accept/tests/test_threshold_accept.py` & `alns-5.1.0/alns/accept/tests/test_threshold_accept.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/accept/tests/test_update.py` & `alns-5.1.0/alns/accept/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/accept/tests/test_worse_accept.py` & `alns-5.1.0/alns/accept/tests/test_worse_accept.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/accept/update.py` & `alns-5.1.0/alns/accept/update.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/select/AlphaUCB.py` & `alns-5.1.0/alns/select/AlphaUCB.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/select/OperatorSelectionScheme.py` & `alns-5.1.0/alns/select/OperatorSelectionScheme.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/select/RandomSelect.py` & `alns-5.1.0/alns/select/RandomSelect.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/select/RouletteWheel.py` & `alns-5.1.0/alns/select/RouletteWheel.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/select/SegmentedRouletteWheel.py` & `alns-5.1.0/alns/select/SegmentedRouletteWheel.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/select/tests/test_alpha_ucb.py` & `alns-5.1.0/alns/select/tests/test_alpha_ucb.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/select/tests/test_random_select.py` & `alns-5.1.0/alns/select/tests/test_random_select.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/select/tests/test_roulette_wheel.py` & `alns-5.1.0/alns/select/tests/test_roulette_wheel.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/select/tests/test_segmented_roulette_wheel.py` & `alns-5.1.0/alns/select/tests/test_segmented_roulette_wheel.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/stop/MaxRuntime.py` & `alns-5.1.0/alns/stop/MaxRuntime.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import time
 from typing import Optional
 
 from numpy.random import RandomState
 
 from alns.State import State
-from alns.stop.StoppingCriterion import StoppingCriterion
 
 
-class MaxRuntime(StoppingCriterion):
+class MaxRuntime:
     """
     Criterion that stops after a specified maximum runtime.
     """
 
     def __init__(self, max_runtime: float):
         if max_runtime < 0:
             raise ValueError("max_runtime < 0 not understood.")
```

### Comparing `alns-5.0.4/alns/stop/NoImprovement.py` & `alns-5.1.0/alns/stop/NoImprovement.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import Optional
 
 from numpy.random import RandomState
 
 from alns.State import State
-from alns.stop.StoppingCriterion import StoppingCriterion
 
 
-class NoImprovement(StoppingCriterion):
+class NoImprovement:
     """
     Criterion that stops if the best solution has not been improved
     after a number of iterations.
 
     Parameters
     ----------
     max_iterations
```

### Comparing `alns-5.0.4/alns/stop/tests/test_max_iterations.py` & `alns-5.1.0/alns/stop/tests/test_max_iterations.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/stop/tests/test_max_runtime.py` & `alns-5.1.0/alns/stop/tests/test_max_runtime.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/stop/tests/test_no_improvement.py` & `alns-5.1.0/alns/stop/tests/test_no_improvement.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/tests/test_alns.py` & `alns-5.1.0/alns/tests/test_alns.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/tests/test_result.py` & `alns-5.1.0/alns/tests/test_result.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/alns/tests/test_statistics.py` & `alns-5.1.0/alns/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `alns-5.0.4/pyproject.toml` & `alns-5.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,65 @@
 [tool.poetry]
 name = "alns"
-version = "5.0.4"
+version = "5.1.0"
 description = "A flexible implementation of the adaptive large neighbourhood search (ALNS) algorithm."
 authors = ["Niels Wouda <nielswouda@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/N-Wouda/ALNS"
 include = [
     "LICENSE.md",
 ]
 packages = [
     {include = "alns"},
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Development Status :: 5 - Production/Stable",
     "Topic :: Software Development",
     "Topic :: Scientific/Engineering",
 ]
 
 [tool.poetry.urls]
 "Tracker" = "https://github.com/N-Wouda/ALNS/issues"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-numpy = ">=1.15.2"
-matplotlib = ">=2.2.0"
+python = "^3.8, <4.0"
+numpy = ">=1.18.0"
+matplotlib = ">=3.5.0"
 
-[tool.poetry.dev-dependencies]
+# This group is needed to develop the package itself.
+[tool.poetry.group.dev.dependencies]
+vrplib = "^1.0.1"
 pre-commit = "^2.20.0"
 pytest = ">=6.0.0"
 pytest-cov = ">=2.6.1"
 codecov = "*"
 
+# This optional docs group is needed to build the documentation. It is not 
+# required by the package itself.
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+tomli = ">=2.0.1"
+nbsphinx = ">=0.8.9"
+ipython = ">=8.6.0"
+numpydoc = ">=1.5.0"
+sphinx_rtd_theme = ">=0.5.1"
+sphinx-autoapi = ">=2.0.1"
+docutils = "==0.16"
+
 # This optional examples group is needed to run the example notebooks, but not
 # required for the package itself.
 [tool.poetry.group.examples]
 optional = true
 
 [tool.poetry.group.examples.dependencies]
 cvrplib = "^0.1.1"
```

### Comparing `alns-5.0.4/setup.py` & `alns-5.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,156 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['alns',
- 'alns.accept',
- 'alns.accept.tests',
- 'alns.select',
- 'alns.select.tests',
- 'alns.stop',
- 'alns.stop.tests',
- 'alns.tests']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['matplotlib>=2.2.0', 'numpy>=1.15.2']
-
-setup_kwargs = {
-    'name': 'alns',
-    'version': '5.0.4',
-    'description': 'A flexible implementation of the adaptive large neighbourhood search (ALNS) algorithm.',
-    'long_description': '[![PyPI version](https://badge.fury.io/py/alns.svg)](https://badge.fury.io/py/alns)\n[![ALNS](https://github.com/N-Wouda/ALNS/actions/workflows/alns.yaml/badge.svg)](https://github.com/N-Wouda/ALNS/actions/workflows/alns.yaml)\n[![Documentation Status](https://readthedocs.org/projects/alns/badge/?version=latest)](https://alns.readthedocs.io/en/latest/?badge=latest)\n[![codecov](https://codecov.io/gh/N-Wouda/ALNS/branch/master/graph/badge.svg)](https://codecov.io/gh/N-Wouda/ALNS)\n\n``alns`` is a general, well-documented and tested implementation of the adaptive\nlarge neighbourhood search (ALNS) metaheuristic in Python. ALNS is an algorithm\nthat can be used to solve difficult combinatorial optimisation problems. The\nalgorithm begins with an initial solution. Then the algorithm iterates until a\nstopping criterion is met. In each iteration, a destroy and repair operator are\nselected, which transform the current solution into a candidate solution. This\ncandidate solution is then evaluated by an acceptance criterion, and the\noperator selection scheme is updated based on the evaluation outcome.\n\n`alns` depends only on `numpy` and `matplotlib`. It may be installed in the\nusual way as\n\n```\npip install alns\n```\n\nThe documentation is available [here][1].\n\n### Getting started\n\nIf you are new to metaheuristics or ALNS, you might benefit from reading\nthe [introduction to ALNS][11] page.\n\nThe `alns` library provides the ALNS algorithm and various acceptance criteria,\noperator selection schemes, and stopping criteria. To solve your own problem,\nyou should provide the following:\n\n- A solution state for your problem that implements an `objective()` function.\n- An initial solution.\n- One or more destroy and repair operators tailored to your problem.\n\nA "quickstart" code template is available [here][10].\n\n### Examples\n\nWe provide several example notebooks showing how the ALNS library may be used.\nThese include:\n\n- The travelling salesman problem (TSP), [here][2]. We solve an instance of 131\n  cities using very simple destroy and repair heuristics.\n- The capacitated vehicle routing problem (CVRP), [here][8]. We solve an\n  instance with 241 customers using a combination of a greedy repair operator,\n  and a _slack-induced substring removal_ destroy operator.\n- The cutting-stock problem (CSP), [here][4]. We solve an instance with 180\n  beams over 165 distinct sizes in only a very limited number of iterations.\n- The resource-constrained project scheduling problem (RCPSP), [here][6]. We\n  solve an instance with 90 jobs and 4 resources using a number of different\n  operators and enhancement techniques from the literature.\n- The permutation flow shop problem (PFSP), [here][9]. We solve an instance with\n  50 jobs and 20 machines. Moreover, we demonstrate multiple advanced features\n  of ALNS, including auto-fitting the acceptance criterion and adding local\n  search to repair operators. We also demonstrate how one could tune ALNS\n  parameters.\n\nFinally, the features notebook gives an overview of various options available in\nthe `alns` package. In the notebook we use these different options to solve a\ntoy 0/1-knapsack problem. The notebook is a good starting point for when you\nwant to use different schemes, acceptance or stopping criteria yourself. It is\navailable [here][5].\n\n### Contributing\n\nWe are very grateful for any contributions you are willing to make. Please have\na look [here][3] to get started. If you aim to make a large change, it is\nhelpful to discuss the change first in a new GitHub issue. Feel free to open\none!\n\n### Getting help\n\nIf you are looking for help, please follow the instructions [here][7].\n\n[1]: https://alns.readthedocs.io/en/latest/\n\n[2]: https://alns.readthedocs.io/en/latest/examples/travelling_salesman_problem.html\n\n[3]: https://alns.readthedocs.io/en/latest/setup/contributing.html\n\n[4]: https://alns.readthedocs.io/en/latest/examples/cutting_stock_problem.html\n\n[5]: https://alns.readthedocs.io/en/latest/examples/alns_features.html\n\n[6]: https://alns.readthedocs.io/en/latest/examples/resource_constrained_project_scheduling_problem.html\n\n[7]: https://alns.readthedocs.io/en/latest/setup/getting_help.html\n\n[8]: https://alns.readthedocs.io/en/latest/examples/capacitated_vehicle_routing_problem.html\n\n[9]: https://alns.readthedocs.io/en/latest/examples/permutation_flow_shop_problem.html\n\n[10]: https://alns.readthedocs.io/en/latest/setup/template.html\n\n[11]: https://alns.readthedocs.io/en/latest/setup/introduction_to_alns.html\n',
-    'author': 'Niels Wouda',
-    'author_email': 'nielswouda@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/N-Wouda/ALNS',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+Metadata-Version: 2.1
+Name: alns
+Version: 5.1.0
+Summary: A flexible implementation of the adaptive large neighbourhood search (ALNS) algorithm.
+Home-page: https://github.com/N-Wouda/ALNS
+License: MIT
+Author: Niels Wouda
+Author-email: nielswouda@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development
+Requires-Dist: matplotlib (>=3.5.0)
+Requires-Dist: numpy (>=1.18.0)
+Project-URL: Repository, https://github.com/N-Wouda/ALNS
+Project-URL: Tracker, https://github.com/N-Wouda/ALNS/issues
+Description-Content-Type: text/markdown
+
+[![PyPI version](https://badge.fury.io/py/alns.svg)](https://badge.fury.io/py/alns)
+[![ALNS](https://github.com/N-Wouda/ALNS/actions/workflows/alns.yaml/badge.svg)](https://github.com/N-Wouda/ALNS/actions/workflows/alns.yaml)
+[![Documentation Status](https://readthedocs.org/projects/alns/badge/?version=latest)](https://alns.readthedocs.io/en/latest/?badge=latest)
+[![codecov](https://codecov.io/gh/N-Wouda/ALNS/branch/master/graph/badge.svg)](https://codecov.io/gh/N-Wouda/ALNS)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05028/status.svg)](https://doi.org/10.21105/joss.05028)
+
+``alns`` is a general, well-documented and tested implementation of the adaptive
+large neighbourhood search (ALNS) metaheuristic in Python. ALNS is an algorithm
+that can be used to solve difficult combinatorial optimisation problems. The
+algorithm begins with an initial solution. Then the algorithm iterates until a
+stopping criterion is met. In each iteration, a destroy and repair operator are
+selected, which transform the current solution into a candidate solution. This
+candidate solution is then evaluated by an acceptance criterion, and the
+operator selection scheme is updated based on the evaluation outcome.
+
+`alns` depends only on `numpy` and `matplotlib`. It may be installed in the
+usual way as
+
+```
+pip install alns
+```
+
+The documentation is available [here][1].
+
+### Getting started
+
+If you are new to metaheuristics or ALNS, you might benefit from reading
+the [introduction to ALNS][11] page.
+
+The `alns` library provides the ALNS algorithm and various acceptance criteria,
+operator selection schemes, and stopping criteria. To solve your own problem,
+you should provide the following:
+
+- A solution state for your problem that implements an `objective()` function.
+- An initial solution.
+- One or more destroy and repair operators tailored to your problem.
+
+A "quickstart" code template is available [here][10].
+
+### Examples
+
+We provide several example notebooks showing how the ALNS library may be used.
+These include:
+
+- The travelling salesman problem (TSP), [here][2]. We solve an instance of 131
+  cities using very simple destroy and repair heuristics.
+- The capacitated vehicle routing problem (CVRP), [here][8]. We solve an
+  instance with 241 customers using a combination of a greedy repair operator,
+  and a _slack-induced substring removal_ destroy operator.
+- The cutting-stock problem (CSP), [here][4]. We solve an instance with 180
+  beams over 165 distinct sizes in only a very limited number of iterations.
+- The resource-constrained project scheduling problem (RCPSP), [here][6]. We
+  solve an instance with 90 jobs and 4 resources using a number of different
+  operators and enhancement techniques from the literature.
+- The permutation flow shop problem (PFSP), [here][9]. We solve an instance with
+  50 jobs and 20 machines. Moreover, we demonstrate multiple advanced features
+  of ALNS, including auto-fitting the acceptance criterion and adding local
+  search to repair operators. We also demonstrate how one could tune ALNS
+  parameters.
+
+Finally, the features notebook gives an overview of various options available in
+the `alns` package. In the notebook we use these different options to solve a
+toy 0/1-knapsack problem. The notebook is a good starting point for when you
+want to use different schemes, acceptance or stopping criteria yourself. It is
+available [here][5].
+
+### Contributing
+
+We are very grateful for any contributions you are willing to make. Please have
+a look [here][3] to get started. If you aim to make a large change, it is
+helpful to discuss the change first in a new GitHub issue. Feel free to open
+one!
+
+### Getting help
+
+If you are looking for help, please follow the instructions [here][7].
+
+### How to cite `alns`
+
+If you use `alns` in your research, please consider citing the following paper:
+
+> Wouda, N.A., and L. Lan (2023). 
+> ALNS: a Python implementation of the adaptive large neighbourhood search metaheuristic. 
+> _Journal of Open Source Software_, 8(81): 5028. 
+> https://doi.org/10.21105/joss.05028
+
+Or, using the following BibTeX entry:
+
+```bibtex
+@article{Wouda_Lan_ALNS_2023, 
+  doi = {10.21105/joss.05028}, 
+  url = {https://doi.org/10.21105/joss.05028}, 
+  year = {2023}, 
+  publisher = {The Open Journal}, 
+  volume = {8}, 
+  number = {81}, 
+  pages = {5028}, 
+  author = {Niels A. Wouda and Leon Lan}, 
+  title = {{ALNS}: a {P}ython implementation of the adaptive large neighbourhood search metaheuristic}, 
+  journal = {Journal of Open Source Software} 
 }
+```
+
+[1]: https://alns.readthedocs.io/en/latest/
+
+[2]: https://alns.readthedocs.io/en/latest/examples/travelling_salesman_problem.html
+
+[3]: https://alns.readthedocs.io/en/latest/setup/contributing.html
+
+[4]: https://alns.readthedocs.io/en/latest/examples/cutting_stock_problem.html
+
+[5]: https://alns.readthedocs.io/en/latest/examples/alns_features.html
+
+[6]: https://alns.readthedocs.io/en/latest/examples/resource_constrained_project_scheduling_problem.html
+
+[7]: https://alns.readthedocs.io/en/latest/setup/getting_help.html
+
+[8]: https://alns.readthedocs.io/en/latest/examples/capacitated_vehicle_routing_problem.html
+
+[9]: https://alns.readthedocs.io/en/latest/examples/permutation_flow_shop_problem.html
+
+[10]: https://alns.readthedocs.io/en/latest/setup/template.html
 
+[11]: https://alns.readthedocs.io/en/latest/setup/introduction_to_alns.html
 
-setup(**setup_kwargs)
```

### Comparing `alns-5.0.4/PKG-INFO` & `alns-5.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,12 @@
-Metadata-Version: 2.1
-Name: alns
-Version: 5.0.4
-Summary: A flexible implementation of the adaptive large neighbourhood search (ALNS) algorithm.
-Home-page: https://github.com/N-Wouda/ALNS
-License: MIT
-Author: Niels Wouda
-Author-email: nielswouda@gmail.com
-Requires-Python: >=3.7,<4.0
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development
-Requires-Dist: matplotlib (>=2.2.0)
-Requires-Dist: numpy (>=1.15.2)
-Project-URL: Repository, https://github.com/N-Wouda/ALNS
-Project-URL: Tracker, https://github.com/N-Wouda/ALNS/issues
-Description-Content-Type: text/markdown
-
 [![PyPI version](https://badge.fury.io/py/alns.svg)](https://badge.fury.io/py/alns)
 [![ALNS](https://github.com/N-Wouda/ALNS/actions/workflows/alns.yaml/badge.svg)](https://github.com/N-Wouda/ALNS/actions/workflows/alns.yaml)
 [![Documentation Status](https://readthedocs.org/projects/alns/badge/?version=latest)](https://alns.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/N-Wouda/ALNS/branch/master/graph/badge.svg)](https://codecov.io/gh/N-Wouda/ALNS)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05028/status.svg)](https://doi.org/10.21105/joss.05028)
 
 ``alns`` is a general, well-documented and tested implementation of the adaptive
 large neighbourhood search (ALNS) metaheuristic in Python. ALNS is an algorithm
 that can be used to solve difficult combinatorial optimisation problems. The
 algorithm begins with an initial solution. Then the algorithm iterates until a
 stopping criterion is met. In each iteration, a destroy and repair operator are
 selected, which transform the current solution into a candidate solution. This
@@ -102,14 +71,40 @@
 helpful to discuss the change first in a new GitHub issue. Feel free to open
 one!
 
 ### Getting help
 
 If you are looking for help, please follow the instructions [here][7].
 
+### How to cite `alns`
+
+If you use `alns` in your research, please consider citing the following paper:
+
+> Wouda, N.A., and L. Lan (2023). 
+> ALNS: a Python implementation of the adaptive large neighbourhood search metaheuristic. 
+> _Journal of Open Source Software_, 8(81): 5028. 
+> https://doi.org/10.21105/joss.05028
+
+Or, using the following BibTeX entry:
+
+```bibtex
+@article{Wouda_Lan_ALNS_2023, 
+  doi = {10.21105/joss.05028}, 
+  url = {https://doi.org/10.21105/joss.05028}, 
+  year = {2023}, 
+  publisher = {The Open Journal}, 
+  volume = {8}, 
+  number = {81}, 
+  pages = {5028}, 
+  author = {Niels A. Wouda and Leon Lan}, 
+  title = {{ALNS}: a {P}ython implementation of the adaptive large neighbourhood search metaheuristic}, 
+  journal = {Journal of Open Source Software} 
+}
+```
+
 [1]: https://alns.readthedocs.io/en/latest/
 
 [2]: https://alns.readthedocs.io/en/latest/examples/travelling_salesman_problem.html
 
 [3]: https://alns.readthedocs.io/en/latest/setup/contributing.html
 
 [4]: https://alns.readthedocs.io/en/latest/examples/cutting_stock_problem.html
@@ -123,8 +118,7 @@
 [8]: https://alns.readthedocs.io/en/latest/examples/capacitated_vehicle_routing_problem.html
 
 [9]: https://alns.readthedocs.io/en/latest/examples/permutation_flow_shop_problem.html
 
 [10]: https://alns.readthedocs.io/en/latest/setup/template.html
 
 [11]: https://alns.readthedocs.io/en/latest/setup/introduction_to_alns.html
-
```

