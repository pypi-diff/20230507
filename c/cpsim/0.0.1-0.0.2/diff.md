# Comparing `tmp/cpsim-0.0.1.tar.gz` & `tmp/cpsim-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpsim-0.0.1.tar", last modified: Sat May  6 22:23:32 2023, max compression
+gzip compressed data, was "cpsim-0.0.2.tar", last modified: Sun May  7 01:13:01 2023, max compression
```

## Comparing `cpsim-0.0.1.tar` & `cpsim-0.0.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 22:23:32.974540 cpsim-0.0.1/
--rw-rw-rw-   0        0        0     1087 2023-03-17 04:12:54.000000 cpsim-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2189 2023-05-06 22:23:32.972541 cpsim-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      129 2023-04-26 20:24:42.000000 cpsim-0.0.1/README.md
--rw-rw-rw-   0        0        0     1045 2023-05-06 21:49:38.000000 cpsim-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 22:23:32.975540 cpsim-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-06 22:23:32.899521 cpsim-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-06 22:23:32.910540 cpsim-0.0.1/src/cpsim/
--rw-rw-rw-   0        0        0      157 2023-05-06 21:25:36.000000 cpsim-0.0.1/src/cpsim/__init__.py
--rw-rw-rw-   0        0        0     2247 2022-10-21 16:01:42.000000 cpsim-0.0.1/src/cpsim/attack.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:23:32.925540 cpsim-0.0.1/src/cpsim/controllers/
--rw-rw-rw-   0        0        0     7156 2023-05-06 22:20:34.000000 cpsim-0.0.1/src/cpsim/controllers/LP_cvxpy.py
--rw-rw-rw-   0        0        0     1081 2023-05-06 21:25:36.000000 cpsim-0.0.1/src/cpsim/controllers/LQR.py
--rw-rw-rw-   0        0        0     1859 2023-05-06 21:25:36.000000 cpsim-0.0.1/src/cpsim/controllers/LQRSSE.py
--rw-rw-rw-   0        0        0     6429 2023-05-06 22:20:34.000000 cpsim-0.0.1/src/cpsim/controllers/MPC_OSQP.py
--rw-rw-rw-   0        0        0     7640 2023-05-06 22:20:34.000000 cpsim-0.0.1/src/cpsim/controllers/MPC_cvxpy.py
--rw-rw-rw-   0        0        0     5775 2023-05-06 21:25:36.000000 cpsim-0.0.1/src/cpsim/controllers/PID.py
--rw-rw-rw-   0        0        0     5815 2023-05-06 22:11:08.000000 cpsim-0.0.1/src/cpsim/controllers/PID_incremental.py
--rw-rw-rw-   0        0        0        0 2023-05-06 22:11:08.000000 cpsim-0.0.1/src/cpsim/controllers/__init__.py
--rw-rw-rw-   0        0        0      363 2022-10-21 16:01:42.000000 cpsim-0.0.1/src/cpsim/controllers/controller_base.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:23:32.933540 cpsim-0.0.1/src/cpsim/formal/
--rw-rw-rw-   0        0        0      124 2022-10-21 16:01:42.000000 cpsim-0.0.1/src/cpsim/formal/__init__.py
--rw-rw-rw-   0        0        0     4082 2023-05-06 22:20:34.000000 cpsim-0.0.1/src/cpsim/formal/gaussian_distribution.py
--rw-rw-rw-   0        0        0      691 2022-10-21 16:01:42.000000 cpsim-0.0.1/src/cpsim/formal/half_space.py
--rw-rw-rw-   0        0        0      263 2022-10-21 16:01:42.000000 cpsim-0.0.1/src/cpsim/formal/hyperplane.py
--rw-rw-rw-   0        0        0     7303 2023-05-06 22:20:34.000000 cpsim-0.0.1/src/cpsim/formal/reachability.py
--rw-rw-rw-   0        0        0     1442 2023-05-06 22:20:34.000000 cpsim-0.0.1/src/cpsim/formal/strip.py
--rw-rw-rw-   0        0        0     9321 2023-05-06 22:20:34.000000 cpsim-0.0.1/src/cpsim/formal/zonotope.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:23:32.936558 cpsim-0.0.1/src/cpsim/info/
--rw-rw-rw-   0        0        0      387 2023-01-15 15:39:18.000000 cpsim-0.0.1/src/cpsim/info/Timer.py
--rw-rw-rw-   0        0        0        0 2023-01-15 15:10:49.000000 cpsim-0.0.1/src/cpsim/info/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:23:32.937540 cpsim-0.0.1/src/cpsim/models/
--rw-rw-rw-   0        0        0        0 2023-05-06 22:11:08.000000 cpsim-0.0.1/src/cpsim/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:23:32.951540 cpsim-0.0.1/src/cpsim/models/linear/
--rw-rw-rw-   0        0        0     3307 2023-05-06 22:12:11.000000 cpsim-0.0.1/src/cpsim/models/linear/F16.py
--rw-rw-rw-   0        0        0        0 2022-10-21 16:01:42.000000 cpsim-0.0.1/src/cpsim/models/linear/__init__.py
--rw-rw-rw-   0        0        0     2931 2023-05-06 22:11:54.000000 cpsim-0.0.1/src/cpsim/models/linear/aircraft_pitch.py
--rw-rw-rw-   0        0        0     3870 2023-05-06 22:13:16.000000 cpsim-0.0.1/src/cpsim/models/linear/boeing747.py
--rw-rw-rw-   0        0        0     3803 2023-05-06 22:12:11.000000 cpsim-0.0.1/src/cpsim/models/linear/heat.py
--rw-rw-rw-   0        0        0     3024 2023-05-06 22:13:16.000000 cpsim-0.0.1/src/cpsim/models/linear/lane_keeping.py
--rw-rw-rw-   0        0        0     3203 2023-05-06 22:13:16.000000 cpsim-0.0.1/src/cpsim/models/linear/motor_speed.py
--rw-rw-rw-   0        0        0     3700 2023-05-06 22:13:16.000000 cpsim-0.0.1/src/cpsim/models/linear/platoon.py
--rw-rw-rw-   0        0        0     3900 2023-05-06 22:13:30.000000 cpsim-0.0.1/src/cpsim/models/linear/quadrotor.py
--rw-rw-rw-   0        0        0     5404 2023-05-06 22:13:39.000000 cpsim-0.0.1/src/cpsim/models/linear/quadruple_tank.py
--rw-rw-rw-   0        0        0     2406 2023-05-06 22:13:49.000000 cpsim-0.0.1/src/cpsim/models/linear/rlc_circuit.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:23:32.959620 cpsim-0.0.1/src/cpsim/models/nonlinear/
--rw-rw-rw-   0        0        0        0 2022-10-21 16:01:42.000000 cpsim-0.0.1/src/cpsim/models/nonlinear/__init__.py
--rw-rw-rw-   0        0        0      990 2023-05-06 21:25:36.000000 cpsim-0.0.1/src/cpsim/models/nonlinear/compute_analytical_model.py
--rw-rw-rw-   0        0        0     1481 2023-05-06 21:25:36.000000 cpsim-0.0.1/src/cpsim/models/nonlinear/compute_analytical_model_quad.py
--rw-rw-rw-   0        0        0     5471 2023-05-06 22:20:34.000000 cpsim-0.0.1/src/cpsim/models/nonlinear/continuous_stirred_tank_reactor.py
--rw-rw-rw-   0        0        0     4698 2023-05-06 22:20:34.000000 cpsim-0.0.1/src/cpsim/models/nonlinear/inverted_pendulum.py
--rw-rw-rw-   0        0        0     9187 2023-05-06 22:20:34.000000 cpsim-0.0.1/src/cpsim/models/nonlinear/quad.py
--rw-rw-rw-   0        0        0     8709 2023-05-06 22:20:34.000000 cpsim-0.0.1/src/cpsim/models/nonlinear/vessel.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:23:32.968541 cpsim-0.0.1/src/cpsim/observers/
--rw-rw-rw-   0        0        0        0 2023-04-26 20:26:31.000000 cpsim-0.0.1/src/cpsim/observers/__init__.py
--rw-rw-rw-   0        0        0     1736 2023-02-27 16:28:50.000000 cpsim-0.0.1/src/cpsim/observers/extended_kalman_filter.py
--rw-rw-rw-   0        0        0     3629 2023-05-06 21:25:36.000000 cpsim-0.0.1/src/cpsim/observers/full_state_bound.py
--rw-rw-rw-   0        0        0     1844 2023-05-06 21:25:36.000000 cpsim-0.0.1/src/cpsim/observers/full_state_bound_nonlinear.py
--rw-rw-rw-   0        0        0     4604 2023-05-06 22:20:34.000000 cpsim-0.0.1/src/cpsim/observers/interval_helpers.py
--rw-rw-rw-   0        0        0     1653 2022-10-21 16:01:42.000000 cpsim-0.0.1/src/cpsim/observers/kalman_filter.py
--rw-rw-rw-   0        0        0     9048 2023-05-06 22:20:34.000000 cpsim-0.0.1/src/cpsim/simulator.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:23:32.970539 cpsim-0.0.1/src/cpsim/utils/
--rw-rw-rw-   0        0        0        0 2022-10-23 22:09:23.000000 cpsim-0.0.1/src/cpsim/utils/__init__.py
--rw-rw-rw-   0        0        0     2605 2023-05-06 22:20:34.000000 cpsim-0.0.1/src/cpsim/utils/linearizer.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:23:32.915624 cpsim-0.0.1/src/cpsim.egg-info/
--rw-rw-rw-   0        0        0     2189 2023-05-06 22:23:32.000000 cpsim-0.0.1/src/cpsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1920 2023-05-06 22:23:32.000000 cpsim-0.0.1/src/cpsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 22:23:32.000000 cpsim-0.0.1/src/cpsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-05-06 22:23:32.000000 cpsim-0.0.1/src/cpsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-06 22:23:32.000000 cpsim-0.0.1/src/cpsim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 01:13:01.326233 cpsim-0.0.2/
+-rw-rw-rw-   0        0        0     1087 2023-03-17 04:12:54.000000 cpsim-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2210 2023-05-07 01:13:01.324236 cpsim-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      129 2023-04-26 20:24:42.000000 cpsim-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1083 2023-05-07 01:09:38.000000 cpsim-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 01:13:01.326233 cpsim-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-07 01:13:01.186745 cpsim-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-07 01:13:01.203801 cpsim-0.0.2/src/cpsim/
+-rw-rw-rw-   0        0        0      157 2023-05-06 21:25:36.000000 cpsim-0.0.2/src/cpsim/__init__.py
+-rw-rw-rw-   0        0        0     2247 2022-10-21 16:01:42.000000 cpsim-0.0.2/src/cpsim/attack.py
+drwxrwxrwx   0        0        0        0 2023-05-07 01:13:01.233805 cpsim-0.0.2/src/cpsim/controllers/
+-rw-rw-rw-   0        0        0     7156 2023-05-06 22:20:34.000000 cpsim-0.0.2/src/cpsim/controllers/LP_cvxpy.py
+-rw-rw-rw-   0        0        0     1081 2023-05-06 21:25:36.000000 cpsim-0.0.2/src/cpsim/controllers/LQR.py
+-rw-rw-rw-   0        0        0     1859 2023-05-06 21:25:36.000000 cpsim-0.0.2/src/cpsim/controllers/LQRSSE.py
+-rw-rw-rw-   0        0        0     6429 2023-05-06 22:20:34.000000 cpsim-0.0.2/src/cpsim/controllers/MPC_OSQP.py
+-rw-rw-rw-   0        0        0     7640 2023-05-06 22:20:34.000000 cpsim-0.0.2/src/cpsim/controllers/MPC_cvxpy.py
+-rw-rw-rw-   0        0        0     5775 2023-05-06 21:25:36.000000 cpsim-0.0.2/src/cpsim/controllers/PID.py
+-rw-rw-rw-   0        0        0     5815 2023-05-06 22:11:08.000000 cpsim-0.0.2/src/cpsim/controllers/PID_incremental.py
+-rw-rw-rw-   0        0        0        0 2023-05-06 22:11:08.000000 cpsim-0.0.2/src/cpsim/controllers/__init__.py
+-rw-rw-rw-   0        0        0      363 2022-10-21 16:01:42.000000 cpsim-0.0.2/src/cpsim/controllers/controller_base.py
+drwxrwxrwx   0        0        0        0 2023-05-07 01:13:01.246806 cpsim-0.0.2/src/cpsim/formal/
+-rw-rw-rw-   0        0        0      124 2022-10-21 16:01:42.000000 cpsim-0.0.2/src/cpsim/formal/__init__.py
+-rw-rw-rw-   0        0        0     4082 2023-05-06 22:20:34.000000 cpsim-0.0.2/src/cpsim/formal/gaussian_distribution.py
+-rw-rw-rw-   0        0        0      691 2022-10-21 16:01:42.000000 cpsim-0.0.2/src/cpsim/formal/half_space.py
+-rw-rw-rw-   0        0        0      263 2022-10-21 16:01:42.000000 cpsim-0.0.2/src/cpsim/formal/hyperplane.py
+-rw-rw-rw-   0        0        0     7303 2023-05-06 22:20:34.000000 cpsim-0.0.2/src/cpsim/formal/reachability.py
+-rw-rw-rw-   0        0        0     1442 2023-05-06 22:20:34.000000 cpsim-0.0.2/src/cpsim/formal/strip.py
+-rw-rw-rw-   0        0        0     9321 2023-05-06 22:20:34.000000 cpsim-0.0.2/src/cpsim/formal/zonotope.py
+drwxrwxrwx   0        0        0        0 2023-05-07 01:13:01.253943 cpsim-0.0.2/src/cpsim/info/
+-rw-rw-rw-   0        0        0      387 2023-01-15 15:39:18.000000 cpsim-0.0.2/src/cpsim/info/Timer.py
+-rw-rw-rw-   0        0        0        0 2023-01-15 15:10:49.000000 cpsim-0.0.2/src/cpsim/info/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 01:13:01.255956 cpsim-0.0.2/src/cpsim/models/
+-rw-rw-rw-   0        0        0        0 2023-05-06 22:11:08.000000 cpsim-0.0.2/src/cpsim/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 01:13:01.285250 cpsim-0.0.2/src/cpsim/models/linear/
+-rw-rw-rw-   0        0        0     3307 2023-05-06 22:12:11.000000 cpsim-0.0.2/src/cpsim/models/linear/F16.py
+-rw-rw-rw-   0        0        0        0 2022-10-21 16:01:42.000000 cpsim-0.0.2/src/cpsim/models/linear/__init__.py
+-rw-rw-rw-   0        0        0     2931 2023-05-06 22:11:54.000000 cpsim-0.0.2/src/cpsim/models/linear/aircraft_pitch.py
+-rw-rw-rw-   0        0        0     3870 2023-05-06 22:13:16.000000 cpsim-0.0.2/src/cpsim/models/linear/boeing747.py
+-rw-rw-rw-   0        0        0     3803 2023-05-06 22:12:11.000000 cpsim-0.0.2/src/cpsim/models/linear/heat.py
+-rw-rw-rw-   0        0        0     3024 2023-05-06 22:13:16.000000 cpsim-0.0.2/src/cpsim/models/linear/lane_keeping.py
+-rw-rw-rw-   0        0        0     3203 2023-05-06 22:13:16.000000 cpsim-0.0.2/src/cpsim/models/linear/motor_speed.py
+-rw-rw-rw-   0        0        0     3700 2023-05-06 22:13:16.000000 cpsim-0.0.2/src/cpsim/models/linear/platoon.py
+-rw-rw-rw-   0        0        0     3900 2023-05-06 22:13:30.000000 cpsim-0.0.2/src/cpsim/models/linear/quadrotor.py
+-rw-rw-rw-   0        0        0     5404 2023-05-06 22:13:39.000000 cpsim-0.0.2/src/cpsim/models/linear/quadruple_tank.py
+-rw-rw-rw-   0        0        0     2406 2023-05-06 22:13:49.000000 cpsim-0.0.2/src/cpsim/models/linear/rlc_circuit.py
+drwxrwxrwx   0        0        0        0 2023-05-07 01:13:01.305238 cpsim-0.0.2/src/cpsim/models/nonlinear/
+-rw-rw-rw-   0        0        0        0 2022-10-21 16:01:42.000000 cpsim-0.0.2/src/cpsim/models/nonlinear/__init__.py
+-rw-rw-rw-   0        0        0      990 2023-05-06 21:25:36.000000 cpsim-0.0.2/src/cpsim/models/nonlinear/compute_analytical_model.py
+-rw-rw-rw-   0        0        0     1481 2023-05-06 21:25:36.000000 cpsim-0.0.2/src/cpsim/models/nonlinear/compute_analytical_model_quad.py
+-rw-rw-rw-   0        0        0     5471 2023-05-06 22:20:34.000000 cpsim-0.0.2/src/cpsim/models/nonlinear/continuous_stirred_tank_reactor.py
+-rw-rw-rw-   0        0        0     4698 2023-05-06 22:20:34.000000 cpsim-0.0.2/src/cpsim/models/nonlinear/inverted_pendulum.py
+-rw-rw-rw-   0        0        0     9187 2023-05-06 22:20:34.000000 cpsim-0.0.2/src/cpsim/models/nonlinear/quad.py
+-rw-rw-rw-   0        0        0     8709 2023-05-06 22:20:34.000000 cpsim-0.0.2/src/cpsim/models/nonlinear/vessel.py
+drwxrwxrwx   0        0        0        0 2023-05-07 01:13:01.317233 cpsim-0.0.2/src/cpsim/observers/
+-rw-rw-rw-   0        0        0        0 2023-04-26 20:26:31.000000 cpsim-0.0.2/src/cpsim/observers/__init__.py
+-rw-rw-rw-   0        0        0     1736 2023-02-27 16:28:50.000000 cpsim-0.0.2/src/cpsim/observers/extended_kalman_filter.py
+-rw-rw-rw-   0        0        0     3629 2023-05-06 21:25:36.000000 cpsim-0.0.2/src/cpsim/observers/full_state_bound.py
+-rw-rw-rw-   0        0        0     1844 2023-05-06 21:25:36.000000 cpsim-0.0.2/src/cpsim/observers/full_state_bound_nonlinear.py
+-rw-rw-rw-   0        0        0     4604 2023-05-06 22:20:34.000000 cpsim-0.0.2/src/cpsim/observers/interval_helpers.py
+-rw-rw-rw-   0        0        0     1653 2022-10-21 16:01:42.000000 cpsim-0.0.2/src/cpsim/observers/kalman_filter.py
+-rw-rw-rw-   0        0        0     9027 2023-05-06 23:03:13.000000 cpsim-0.0.2/src/cpsim/simulator.py
+drwxrwxrwx   0        0        0        0 2023-05-07 01:13:01.322235 cpsim-0.0.2/src/cpsim/utils/
+-rw-rw-rw-   0        0        0        0 2022-10-23 22:09:23.000000 cpsim-0.0.2/src/cpsim/utils/__init__.py
+-rw-rw-rw-   0        0        0     2605 2023-05-06 22:20:34.000000 cpsim-0.0.2/src/cpsim/utils/linearizer.py
+drwxrwxrwx   0        0        0        0 2023-05-07 01:13:01.212813 cpsim-0.0.2/src/cpsim.egg-info/
+-rw-rw-rw-   0        0        0     2210 2023-05-07 01:13:01.000000 cpsim-0.0.2/src/cpsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1920 2023-05-07 01:13:01.000000 cpsim-0.0.2/src/cpsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 01:13:01.000000 cpsim-0.0.2/src/cpsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-05-07 01:13:01.000000 cpsim-0.0.2/src/cpsim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-07 01:13:01.000000 cpsim-0.0.2/src/cpsim.egg-info/top_level.txt
```

### Comparing `cpsim-0.0.1/LICENSE` & `cpsim-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/PKG-INFO` & `cpsim-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpsim
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simulation and Security Toolbox for Cyber-Physical Systems
 Author-email: Lin Zhang <lzhan120@syr.edu>
 Maintainer-email: Mengyu Liu <mliu71@syr.edu>
 License: MIT License
         
         Copyright (c) 2023 Lin Zhang
         
@@ -33,13 +33,14 @@
 Keywords: cyber-physical system,control,simulation,security,CPS
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: interval
+Provides-Extra: doc
 License-File: LICENSE
 
 # CPSim
 Simulation and Security Toolbox for Cyber-Physical Systems
 
 Homepage: [https://sim.cpsec.org](https://sim.cpsec.org)
```

### Comparing `cpsim-0.0.1/pyproject.toml` & `cpsim-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cpsim"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Lin Zhang", email="lzhan120@syr.edu" },
 ]
 maintainers = [
   { name="Mengyu Liu", email="mliu71@syr.edu" },
 ]
 description = "Simulation and Security Toolbox for Cyber-Physical Systems"
@@ -26,13 +26,14 @@
     "numpy",
     "cvxpy",
     "matplotlib",
 ]
 
 [project.optional-dependencies]
 interval = ["pyinterval"]
+doc = ["sphinx", "sphinx_rtd_theme"]
 
 [project.urls]
 homepage = "https://sim.cpsec.org/en/latest/"
 documentation = "https://sim.cpsec.org/en/latest/"
 repository = "https://github.com/lion-zhang/CPSim/"
 "Bug Tracker" = "https://github.com/lion-zhang/CPSim/issues"
```

### Comparing `cpsim-0.0.1/src/cpsim/attack.py` & `cpsim-0.0.2/src/cpsim/attack.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/controllers/LP_cvxpy.py` & `cpsim-0.0.2/src/cpsim/controllers/LP_cvxpy.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/controllers/LQR.py` & `cpsim-0.0.2/src/cpsim/controllers/LQR.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/controllers/LQRSSE.py` & `cpsim-0.0.2/src/cpsim/controllers/LQRSSE.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/controllers/MPC_OSQP.py` & `cpsim-0.0.2/src/cpsim/controllers/MPC_OSQP.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/controllers/MPC_cvxpy.py` & `cpsim-0.0.2/src/cpsim/controllers/MPC_cvxpy.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/controllers/PID.py` & `cpsim-0.0.2/src/cpsim/controllers/PID.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/controllers/PID_incremental.py` & `cpsim-0.0.2/src/cpsim/controllers/PID_incremental.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/formal/gaussian_distribution.py` & `cpsim-0.0.2/src/cpsim/formal/gaussian_distribution.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/formal/half_space.py` & `cpsim-0.0.2/src/cpsim/formal/half_space.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/formal/reachability.py` & `cpsim-0.0.2/src/cpsim/formal/reachability.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/formal/strip.py` & `cpsim-0.0.2/src/cpsim/formal/strip.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/formal/zonotope.py` & `cpsim-0.0.2/src/cpsim/formal/zonotope.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/models/linear/F16.py` & `cpsim-0.0.2/src/cpsim/models/linear/F16.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/models/linear/aircraft_pitch.py` & `cpsim-0.0.2/src/cpsim/models/linear/aircraft_pitch.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/models/linear/boeing747.py` & `cpsim-0.0.2/src/cpsim/models/linear/boeing747.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/models/linear/heat.py` & `cpsim-0.0.2/src/cpsim/models/linear/heat.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/models/linear/lane_keeping.py` & `cpsim-0.0.2/src/cpsim/models/linear/lane_keeping.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/models/linear/motor_speed.py` & `cpsim-0.0.2/src/cpsim/models/linear/motor_speed.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/models/linear/platoon.py` & `cpsim-0.0.2/src/cpsim/models/linear/platoon.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/models/linear/quadrotor.py` & `cpsim-0.0.2/src/cpsim/models/linear/quadrotor.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/models/linear/quadruple_tank.py` & `cpsim-0.0.2/src/cpsim/models/linear/quadruple_tank.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/models/linear/rlc_circuit.py` & `cpsim-0.0.2/src/cpsim/models/linear/rlc_circuit.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/models/nonlinear/compute_analytical_model.py` & `cpsim-0.0.2/src/cpsim/models/nonlinear/compute_analytical_model.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/models/nonlinear/compute_analytical_model_quad.py` & `cpsim-0.0.2/src/cpsim/models/nonlinear/compute_analytical_model_quad.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/models/nonlinear/continuous_stirred_tank_reactor.py` & `cpsim-0.0.2/src/cpsim/models/nonlinear/continuous_stirred_tank_reactor.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/models/nonlinear/inverted_pendulum.py` & `cpsim-0.0.2/src/cpsim/models/nonlinear/inverted_pendulum.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/models/nonlinear/quad.py` & `cpsim-0.0.2/src/cpsim/models/nonlinear/quad.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/models/nonlinear/vessel.py` & `cpsim-0.0.2/src/cpsim/models/nonlinear/vessel.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/observers/extended_kalman_filter.py` & `cpsim-0.0.2/src/cpsim/observers/extended_kalman_filter.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/observers/full_state_bound.py` & `cpsim-0.0.2/src/cpsim/observers/full_state_bound.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/observers/full_state_bound_nonlinear.py` & `cpsim-0.0.2/src/cpsim/observers/full_state_bound_nonlinear.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/observers/interval_helpers.py` & `cpsim-0.0.2/src/cpsim/observers/interval_helpers.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/observers/kalman_filter.py` & `cpsim-0.0.2/src/cpsim/observers/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim/simulator.py` & `cpsim-0.0.2/src/cpsim/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,23 +62,23 @@
         self.noise_setting = None
         self.m_noise = None
         self.p_noise = None
         self.m_noise_dist = None
         self.p_noise_dist = None
 
     def data_init(self):
-        self.inputs = np.empty((self.max_index + 2, self.m), dtype=np.float)
-        self.outputs = np.empty((self.max_index + 2, self.p), dtype=np.float)
-        self.states = np.empty((self.max_index + 2, self.n), dtype=np.float)
+        self.inputs = np.empty((self.max_index + 2, self.m), dtype=float)
+        self.outputs = np.empty((self.max_index + 2, self.p), dtype=float)
+        self.states = np.empty((self.max_index + 2, self.n), dtype=float)
         if self.feedback_type == 'output':
-            self.feedbacks = np.empty((self.max_index + 2, self.p), dtype=np.float)
-            self.refs = np.empty((self.max_index + 2, self.p), dtype=np.float)
+            self.feedbacks = np.empty((self.max_index + 2, self.p), dtype=float)
+            self.refs = np.empty((self.max_index + 2, self.p), dtype=float)
         elif self.feedback_type == 'state':
-            self.feedbacks = np.empty((self.max_index + 2, self.n), dtype=np.float)
-            self.refs = np.empty((self.max_index + 2, self.n), dtype=np.float)  # reference value
+            self.feedbacks = np.empty((self.max_index + 2, self.n), dtype=float)
+            self.refs = np.empty((self.max_index + 2, self.n), dtype=float)  # reference value
 
     def reset(self):
         # the noise will not reset!
         self.data_init()
         self.cur_index = 0
         self.set_init_state(self.init_state)
         self.controller.clear()
```

### Comparing `cpsim-0.0.1/src/cpsim/utils/linearizer.py` & `cpsim-0.0.2/src/cpsim/utils/linearizer.py`

 * *Files identical despite different names*

### Comparing `cpsim-0.0.1/src/cpsim.egg-info/PKG-INFO` & `cpsim-0.0.2/src/cpsim.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpsim
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simulation and Security Toolbox for Cyber-Physical Systems
 Author-email: Lin Zhang <lzhan120@syr.edu>
 Maintainer-email: Mengyu Liu <mliu71@syr.edu>
 License: MIT License
         
         Copyright (c) 2023 Lin Zhang
         
@@ -33,13 +33,14 @@
 Keywords: cyber-physical system,control,simulation,security,CPS
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: interval
+Provides-Extra: doc
 License-File: LICENSE
 
 # CPSim
 Simulation and Security Toolbox for Cyber-Physical Systems
 
 Homepage: [https://sim.cpsec.org](https://sim.cpsec.org)
```

### Comparing `cpsim-0.0.1/src/cpsim.egg-info/SOURCES.txt` & `cpsim-0.0.2/src/cpsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

