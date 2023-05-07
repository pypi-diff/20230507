# Comparing `tmp/pyVLMP-1.0.1.tar.gz` & `tmp/pyVLMP-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyVLMP-1.0.1.tar", last modified: Fri May  5 16:07:36 2023, max compression
+gzip compressed data, was "pyVLMP-1.0.2.tar", last modified: Sun May  7 18:02:08 2023, max compression
```

## Comparing `pyVLMP-1.0.1.tar` & `pyVLMP-1.0.2.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 16:07:36.973706 pyVLMP-1.0.1/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    35149 2023-01-24 18:33:04.000000 pyVLMP-1.0.1/LICENSE
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-05-05 14:59:17.000000 pyVLMP-1.0.1/MANIFEST.in
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      759 2023-05-05 16:07:36.973706 pyVLMP-1.0.1/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       69 2023-01-24 18:33:04.000000 pyVLMP-1.0.1/README.md
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 16:07:36.969706 pyVLMP-1.0.1/VLMP/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    34280 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/VLMP.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1397 2023-05-03 15:53:33.000000 pyVLMP-1.0.1/VLMP/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     6969 2023-05-03 16:45:43.000000 pyVLMP-1.0.1/VLMP/__main__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 16:07:36.969706 pyVLMP-1.0.1/VLMP/components/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/__init__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 16:07:36.969706 pyVLMP-1.0.1/VLMP/components/globals/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1079 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/globals/NVT.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3340 2023-05-03 16:00:59.000000 pyVLMP-1.0.1/VLMP/components/globals/__init__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 16:07:36.969706 pyVLMP-1.0.1/VLMP/components/integrators/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1657 2023-05-02 14:06:34.000000 pyVLMP-1.0.1/VLMP/components/integrators/BBK.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1630 2023-05-02 14:06:57.000000 pyVLMP-1.0.1/VLMP/components/integrators/EulerMaruyama.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1668 2023-05-02 14:06:52.000000 pyVLMP-1.0.1/VLMP/components/integrators/EulerMaruyamaRigidBody.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1706 2023-05-02 14:07:04.000000 pyVLMP-1.0.1/VLMP/components/integrators/GJF.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     4134 2023-05-03 16:01:12.000000 pyVLMP-1.0.1/VLMP/components/integrators/__init__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 16:07:36.969706 pyVLMP-1.0.1/VLMP/components/modelExtensions/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     5853 2023-05-03 16:01:25.000000 pyVLMP-1.0.1/VLMP/components/modelExtensions/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1685 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/modelExtensions/constantForce.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2071 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/modelExtensions/constantForceBetweenCentersOfMass.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1891 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/modelExtensions/constantForceOverCenterOfMass.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2074 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/modelExtensions/constantTorqueBetweenCentersOfMass.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1866 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/modelExtensions/constantTorqueOverCenterOfMass.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2446 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/modelExtensions/constraintCenterOfMassPosition.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2198 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/modelExtensions/harmonicBondBetweenCentersOfMass.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 16:07:36.969706 pyVLMP-1.0.1/VLMP/components/modelOperations/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     6422 2023-05-03 16:01:39.000000 pyVLMP-1.0.1/VLMP/components/modelOperations/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1239 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/modelOperations/setCenterOfMassPosition.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 16:07:36.969706 pyVLMP-1.0.1/VLMP/components/models/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    27461 2023-04-28 14:56:31.000000 pyVLMP-1.0.1/VLMP/components/models/CORONAVIRUS.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    18939 2023-04-28 14:53:36.000000 pyVLMP-1.0.1/VLMP/components/models/HELIX.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2420 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/models/KB.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    35619 2023-04-28 14:55:03.000000 pyVLMP-1.0.1/VLMP/components/models/MADna.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2699 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/models/SBCG.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2450 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/models/SOP.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     4218 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/models/WLC.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     6169 2023-05-03 16:01:56.000000 pyVLMP-1.0.1/VLMP/components/models/__init__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 16:07:36.969706 pyVLMP-1.0.1/VLMP/components/models/data/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3895 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/models/data/CORONAVIRUS.json
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    38242 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/models/data/MADna.json
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 16:07:36.969706 pyVLMP-1.0.1/VLMP/components/simulationSteps/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     7439 2023-05-03 16:02:11.000000 pyVLMP-1.0.1/VLMP/components/simulationSteps/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1495 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/simulationSteps/centerOfMassMeasurement.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1802 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/simulationSteps/heightMeasurement.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1379 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/simulationSteps/info.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1821 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/simulationSteps/savePatchyParticlesState.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1740 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/simulationSteps/saveState.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 16:07:36.969706 pyVLMP-1.0.1/VLMP/components/system/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3054 2023-05-03 15:59:27.000000 pyVLMP-1.0.1/VLMP/components/system/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2218 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/system/backup.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1102 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/system/simulationName.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 16:07:36.973706 pyVLMP-1.0.1/VLMP/components/types/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     6496 2023-05-03 16:02:33.000000 pyVLMP-1.0.1/VLMP/components/types/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      992 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/types/basic.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      768 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/types/none.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 16:07:36.973706 pyVLMP-1.0.1/VLMP/components/units/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      891 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/units/KcalMol_A.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3921 2023-05-03 16:03:07.000000 pyVLMP-1.0.1/VLMP/components/units/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      887 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/components/units/none.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 16:07:36.973706 pyVLMP-1.0.1/VLMP/experiments/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)    15172 2023-05-02 13:54:57.000000 pyVLMP-1.0.1/VLMP/experiments/SurfaceUmbrellaSampling.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/experiments/__init__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 16:07:36.973706 pyVLMP-1.0.1/VLMP/utils/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/utils/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1784 2023-04-28 14:57:38.000000 pyVLMP-1.0.1/VLMP/utils/bounds.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3142 2023-04-28 14:44:21.000000 pyVLMP-1.0.1/VLMP/utils/utils.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-05 16:07:36.973706 pyVLMP-1.0.1/pyVLMP.egg-info/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      759 2023-05-05 16:07:36.000000 pyVLMP-1.0.1/pyVLMP.egg-info/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     2235 2023-05-05 16:07:36.000000 pyVLMP-1.0.1/pyVLMP.egg-info/SOURCES.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-05-05 16:07:36.000000 pyVLMP-1.0.1/pyVLMP.egg-info/dependency_links.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       41 2023-05-05 16:07:36.000000 pyVLMP-1.0.1/pyVLMP.egg-info/requires.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        5 2023-05-05 16:07:36.000000 pyVLMP-1.0.1/pyVLMP.egg-info/top_level.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      756 2023-05-05 16:06:58.000000 pyVLMP-1.0.1/pyproject.toml
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-05-05 16:07:36.973706 pyVLMP-1.0.1/setup.cfg
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      152 2023-05-03 15:40:43.000000 pyVLMP-1.0.1/setup.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-07 18:02:08.974557 pyVLMP-1.0.2/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    35149 2023-01-24 18:33:04.000000 pyVLMP-1.0.2/LICENSE
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-05-05 14:59:17.000000 pyVLMP-1.0.2/MANIFEST.in
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      759 2023-05-07 18:02:08.974557 pyVLMP-1.0.2/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       69 2023-01-24 18:33:04.000000 pyVLMP-1.0.2/README.md
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-07 18:02:08.970557 pyVLMP-1.0.2/VLMP/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    34280 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/VLMP.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1397 2023-05-03 15:53:33.000000 pyVLMP-1.0.2/VLMP/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     6969 2023-05-03 16:45:43.000000 pyVLMP-1.0.2/VLMP/__main__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-07 18:02:08.970557 pyVLMP-1.0.2/VLMP/components/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-07 18:02:08.970557 pyVLMP-1.0.2/VLMP/components/globals/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1079 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/globals/NVT.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3340 2023-05-03 16:00:59.000000 pyVLMP-1.0.2/VLMP/components/globals/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-07 18:02:08.970557 pyVLMP-1.0.2/VLMP/components/integrators/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1657 2023-05-02 14:06:34.000000 pyVLMP-1.0.2/VLMP/components/integrators/BBK.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1630 2023-05-02 14:06:57.000000 pyVLMP-1.0.2/VLMP/components/integrators/EulerMaruyama.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1668 2023-05-02 14:06:52.000000 pyVLMP-1.0.2/VLMP/components/integrators/EulerMaruyamaRigidBody.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1706 2023-05-02 14:07:04.000000 pyVLMP-1.0.2/VLMP/components/integrators/GJF.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     4134 2023-05-03 16:01:12.000000 pyVLMP-1.0.2/VLMP/components/integrators/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-07 18:02:08.970557 pyVLMP-1.0.2/VLMP/components/modelExtensions/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     5853 2023-05-03 16:01:25.000000 pyVLMP-1.0.2/VLMP/components/modelExtensions/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1685 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/modelExtensions/constantForce.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2071 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/modelExtensions/constantForceBetweenCentersOfMass.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1891 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/modelExtensions/constantForceOverCenterOfMass.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2074 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/modelExtensions/constantTorqueBetweenCentersOfMass.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1866 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/modelExtensions/constantTorqueOverCenterOfMass.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2446 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/modelExtensions/constraintCenterOfMassPosition.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2198 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/modelExtensions/harmonicBondBetweenCentersOfMass.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-07 18:02:08.970557 pyVLMP-1.0.2/VLMP/components/modelOperations/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     6422 2023-05-03 16:01:39.000000 pyVLMP-1.0.2/VLMP/components/modelOperations/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1239 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/modelOperations/setCenterOfMassPosition.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-07 18:02:08.974557 pyVLMP-1.0.2/VLMP/components/models/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    27461 2023-04-28 14:56:31.000000 pyVLMP-1.0.2/VLMP/components/models/CORONAVIRUS.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    18939 2023-04-28 14:53:36.000000 pyVLMP-1.0.2/VLMP/components/models/HELIX.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2420 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/models/KB.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    35619 2023-04-28 14:55:03.000000 pyVLMP-1.0.2/VLMP/components/models/MADna.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2699 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/models/SBCG.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2450 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/models/SOP.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     4218 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/models/WLC.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     6169 2023-05-03 16:01:56.000000 pyVLMP-1.0.2/VLMP/components/models/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-07 18:02:08.974557 pyVLMP-1.0.2/VLMP/components/models/data/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3895 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/models/data/CORONAVIRUS.json
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    38242 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/models/data/MADna.json
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-07 18:02:08.974557 pyVLMP-1.0.2/VLMP/components/simulationSteps/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     7439 2023-05-03 16:02:11.000000 pyVLMP-1.0.2/VLMP/components/simulationSteps/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1495 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/simulationSteps/centerOfMassMeasurement.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1802 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/simulationSteps/heightMeasurement.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1379 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/simulationSteps/info.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1697 2023-05-07 17:55:49.000000 pyVLMP-1.0.2/VLMP/components/simulationSteps/patchPolymersMeasurement.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1821 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/simulationSteps/savePatchyParticlesState.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1740 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/simulationSteps/saveState.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-07 18:02:08.974557 pyVLMP-1.0.2/VLMP/components/system/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3054 2023-05-03 15:59:27.000000 pyVLMP-1.0.2/VLMP/components/system/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2218 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/system/backup.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1102 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/system/simulationName.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-07 18:02:08.974557 pyVLMP-1.0.2/VLMP/components/types/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     6496 2023-05-03 16:02:33.000000 pyVLMP-1.0.2/VLMP/components/types/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      992 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/types/basic.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      768 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/types/none.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-07 18:02:08.974557 pyVLMP-1.0.2/VLMP/components/units/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      891 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/units/KcalMol_A.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3921 2023-05-03 16:03:07.000000 pyVLMP-1.0.2/VLMP/components/units/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      887 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/components/units/none.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-07 18:02:08.974557 pyVLMP-1.0.2/VLMP/experiments/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)    15172 2023-05-02 13:54:57.000000 pyVLMP-1.0.2/VLMP/experiments/SurfaceUmbrellaSampling.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/experiments/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-07 18:02:08.974557 pyVLMP-1.0.2/VLMP/utils/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/utils/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1784 2023-04-28 14:57:38.000000 pyVLMP-1.0.2/VLMP/utils/bounds.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3142 2023-04-28 14:44:21.000000 pyVLMP-1.0.2/VLMP/utils/utils.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2023-05-07 18:02:08.974557 pyVLMP-1.0.2/pyVLMP.egg-info/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      759 2023-05-07 18:02:08.000000 pyVLMP-1.0.2/pyVLMP.egg-info/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     2295 2023-05-07 18:02:08.000000 pyVLMP-1.0.2/pyVLMP.egg-info/SOURCES.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2023-05-07 18:02:08.000000 pyVLMP-1.0.2/pyVLMP.egg-info/dependency_links.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       41 2023-05-07 18:02:08.000000 pyVLMP-1.0.2/pyVLMP.egg-info/requires.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        5 2023-05-07 18:02:08.000000 pyVLMP-1.0.2/pyVLMP.egg-info/top_level.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      756 2023-05-07 17:53:19.000000 pyVLMP-1.0.2/pyproject.toml
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       38 2023-05-07 18:02:08.974557 pyVLMP-1.0.2/setup.cfg
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      152 2023-05-03 15:40:43.000000 pyVLMP-1.0.2/setup.py
```

### Comparing `pyVLMP-1.0.1/LICENSE` & `pyVLMP-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/PKG-INFO` & `pyVLMP-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyVLMP
-Version: 1.0.1
+Version: 1.0.2
 Summary: Virtual Laboratory for the simulation of Macromolecular Properties
 Home-page: https://github.com/PabloIbannez/pyGrained
 Author-email: Pablo Ibáñez-Freire <p.ibanez.fre@gmail.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyVLMP-1.0.1/VLMP/VLMP.py` & `pyVLMP-1.0.2/VLMP/VLMP.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/__init__.py` & `pyVLMP-1.0.2/VLMP/__init__.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/__main__.py` & `pyVLMP-1.0.2/VLMP/__main__.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/globals/NVT.py` & `pyVLMP-1.0.2/VLMP/components/globals/NVT.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/globals/__init__.py` & `pyVLMP-1.0.2/VLMP/components/globals/__init__.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/integrators/BBK.py` & `pyVLMP-1.0.2/VLMP/components/integrators/BBK.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/integrators/EulerMaruyama.py` & `pyVLMP-1.0.2/VLMP/components/integrators/EulerMaruyama.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/integrators/EulerMaruyamaRigidBody.py` & `pyVLMP-1.0.2/VLMP/components/integrators/EulerMaruyamaRigidBody.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/integrators/GJF.py` & `pyVLMP-1.0.2/VLMP/components/integrators/GJF.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/integrators/__init__.py` & `pyVLMP-1.0.2/VLMP/components/integrators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/modelExtensions/__init__.py` & `pyVLMP-1.0.2/VLMP/components/modelExtensions/__init__.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/modelExtensions/constantForce.py` & `pyVLMP-1.0.2/VLMP/components/modelExtensions/constantForce.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/modelExtensions/constantForceBetweenCentersOfMass.py` & `pyVLMP-1.0.2/VLMP/components/modelExtensions/constantForceBetweenCentersOfMass.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/modelExtensions/constantForceOverCenterOfMass.py` & `pyVLMP-1.0.2/VLMP/components/modelExtensions/constantForceOverCenterOfMass.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/modelExtensions/constantTorqueBetweenCentersOfMass.py` & `pyVLMP-1.0.2/VLMP/components/modelExtensions/constantTorqueBetweenCentersOfMass.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/modelExtensions/constantTorqueOverCenterOfMass.py` & `pyVLMP-1.0.2/VLMP/components/modelExtensions/constantTorqueOverCenterOfMass.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/modelExtensions/constraintCenterOfMassPosition.py` & `pyVLMP-1.0.2/VLMP/components/modelExtensions/constraintCenterOfMassPosition.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/modelExtensions/harmonicBondBetweenCentersOfMass.py` & `pyVLMP-1.0.2/VLMP/components/modelExtensions/harmonicBondBetweenCentersOfMass.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/modelOperations/__init__.py` & `pyVLMP-1.0.2/VLMP/components/modelOperations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/modelOperations/setCenterOfMassPosition.py` & `pyVLMP-1.0.2/VLMP/components/modelOperations/setCenterOfMassPosition.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/models/CORONAVIRUS.py` & `pyVLMP-1.0.2/VLMP/components/models/CORONAVIRUS.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/models/HELIX.py` & `pyVLMP-1.0.2/VLMP/components/models/HELIX.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/models/KB.py` & `pyVLMP-1.0.2/VLMP/components/models/KB.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/models/MADna.py` & `pyVLMP-1.0.2/VLMP/components/models/MADna.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/models/SBCG.py` & `pyVLMP-1.0.2/VLMP/components/models/SBCG.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/models/SOP.py` & `pyVLMP-1.0.2/VLMP/components/models/SOP.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/models/WLC.py` & `pyVLMP-1.0.2/VLMP/components/models/WLC.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/models/__init__.py` & `pyVLMP-1.0.2/VLMP/components/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/models/data/CORONAVIRUS.json` & `pyVLMP-1.0.2/VLMP/components/models/data/CORONAVIRUS.json`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/models/data/MADna.json` & `pyVLMP-1.0.2/VLMP/components/models/data/MADna.json`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/simulationSteps/__init__.py` & `pyVLMP-1.0.2/VLMP/components/simulationSteps/__init__.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/simulationSteps/centerOfMassMeasurement.py` & `pyVLMP-1.0.2/VLMP/components/simulationSteps/centerOfMassMeasurement.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/simulationSteps/heightMeasurement.py` & `pyVLMP-1.0.2/VLMP/components/simulationSteps/heightMeasurement.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/simulationSteps/info.py` & `pyVLMP-1.0.2/VLMP/components/simulationSteps/info.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/simulationSteps/savePatchyParticlesState.py` & `pyVLMP-1.0.2/VLMP/components/simulationSteps/savePatchyParticlesState.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/simulationSteps/saveState.py` & `pyVLMP-1.0.2/VLMP/components/simulationSteps/saveState.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/system/__init__.py` & `pyVLMP-1.0.2/VLMP/components/system/__init__.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/system/backup.py` & `pyVLMP-1.0.2/VLMP/components/system/backup.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/system/simulationName.py` & `pyVLMP-1.0.2/VLMP/components/system/simulationName.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/types/__init__.py` & `pyVLMP-1.0.2/VLMP/components/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/types/basic.py` & `pyVLMP-1.0.2/VLMP/components/types/basic.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/types/none.py` & `pyVLMP-1.0.2/VLMP/components/types/none.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/units/KcalMol_A.py` & `pyVLMP-1.0.2/VLMP/components/units/KcalMol_A.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/units/__init__.py` & `pyVLMP-1.0.2/VLMP/components/units/__init__.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/components/units/none.py` & `pyVLMP-1.0.2/VLMP/components/units/none.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/experiments/SurfaceUmbrellaSampling.py` & `pyVLMP-1.0.2/VLMP/experiments/SurfaceUmbrellaSampling.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/utils/bounds.py` & `pyVLMP-1.0.2/VLMP/utils/bounds.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/VLMP/utils/utils.py` & `pyVLMP-1.0.2/VLMP/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pyVLMP-1.0.1/pyVLMP.egg-info/PKG-INFO` & `pyVLMP-1.0.2/pyVLMP.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyVLMP
-Version: 1.0.1
+Version: 1.0.2
 Summary: Virtual Laboratory for the simulation of Macromolecular Properties
 Home-page: https://github.com/PabloIbannez/pyGrained
 Author-email: Pablo Ibáñez-Freire <p.ibanez.fre@gmail.com>
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyVLMP-1.0.1/pyVLMP.egg-info/SOURCES.txt` & `pyVLMP-1.0.2/pyVLMP.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 VLMP/components/models/__init__.py
 VLMP/components/models/data/CORONAVIRUS.json
 VLMP/components/models/data/MADna.json
 VLMP/components/simulationSteps/__init__.py
 VLMP/components/simulationSteps/centerOfMassMeasurement.py
 VLMP/components/simulationSteps/heightMeasurement.py
 VLMP/components/simulationSteps/info.py
+VLMP/components/simulationSteps/patchPolymersMeasurement.py
 VLMP/components/simulationSteps/savePatchyParticlesState.py
 VLMP/components/simulationSteps/saveState.py
 VLMP/components/system/__init__.py
 VLMP/components/system/backup.py
 VLMP/components/system/simulationName.py
 VLMP/components/types/__init__.py
 VLMP/components/types/basic.py
```

### Comparing `pyVLMP-1.0.1/pyproject.toml` & `pyVLMP-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="pyVLMP"
-version="1.0.1"
+version="1.0.2"
 authors = [
     {name = "Pablo Ibáñez-Freire", email = "p.ibanez.fre@gmail.com"},
 ]
 description = "Virtual Laboratory for the simulation of Macromolecular Properties"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT License"}
```

