# Comparing `tmp/xmask-0.2.2.tar.gz` & `tmp/xmask-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmask-0.2.2.tar", last modified: Mon Apr  3 19:29:39 2023, max compression
+gzip compressed data, was "xmask-0.3.0.tar", last modified: Sun May  7 06:54:18 2023, max compression
```

## Comparing `xmask-0.2.2.tar` & `xmask-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-04-03 19:29:39.164495 xmask-0.2.2/
--rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:05:06.000000 xmask-0.2.2/LICENSE
--rw-r--r--   0 giadarol   (503) staff       (20)      237 2023-03-23 11:05:06.000000 xmask-0.2.2/MANIFEST.in
--rw-r--r--   0 giadarol   (503) staff       (20)      520 2023-04-03 19:29:39.164334 xmask-0.2.2/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)      115 2023-03-23 11:05:06.000000 xmask-0.2.2/pyproject.toml
--rw-r--r--   0 giadarol   (503) staff       (20)       38 2023-04-03 19:29:39.164544 xmask-0.2.2/setup.cfg
--rw-r--r--   0 giadarol   (503) staff       (20)     1433 2023-03-23 11:05:06.000000 xmask-0.2.2/setup.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-04-03 19:29:39.162097 xmask-0.2.2/xmask/
--rw-r--r--   0 giadarol   (503) staff       (20)      233 2023-03-23 11:05:06.000000 xmask-0.2.2/xmask/__init__.py
--rw-r--r--   0 giadarol   (503) staff       (20)       22 2023-04-03 19:29:27.000000 xmask-0.2.2/xmask/_version.py
--rw-r--r--   0 giadarol   (503) staff       (20)      225 2023-03-23 11:05:06.000000 xmask-0.2.2/xmask/env_and_links.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-04-03 19:29:39.164119 xmask-0.2.2/xmask/lhc/
--rw-r--r--   0 giadarol   (503) staff       (20)      390 2023-03-23 11:05:06.000000 xmask-0.2.2/xmask/lhc/__init__.py
--rw-r--r--   0 giadarol   (503) staff       (20)     5464 2023-03-29 07:14:03.000000 xmask-0.2.2/xmask/lhc/build_madx_and_xsuite_models.py
--rw-r--r--   0 giadarol   (503) staff       (20)     3553 2023-03-23 11:05:06.000000 xmask-0.2.2/xmask/lhc/errors.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2429 2023-03-23 11:05:06.000000 xmask-0.2.2/xmask/lhc/knob_manipulations.py
--rw-r--r--   0 giadarol   (503) staff       (20)    12248 2023-03-23 11:05:06.000000 xmask-0.2.2/xmask/madx_model.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2879 2023-03-23 11:05:06.000000 xmask-0.2.2/xmask/tuning.py
--rw-r--r--   0 giadarol   (503) staff       (20)      728 2023-03-23 11:05:06.000000 xmask-0.2.2/xmask/yaml.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-04-03 19:29:39.163304 xmask-0.2.2/xmask.egg-info/
--rw-r--r--   0 giadarol   (503) staff       (20)      520 2023-04-03 19:29:39.000000 xmask-0.2.2/xmask.egg-info/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)      412 2023-04-03 19:29:39.000000 xmask-0.2.2/xmask.egg-info/SOURCES.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        1 2023-04-03 19:29:39.000000 xmask-0.2.2/xmask.egg-info/dependency_links.txt
--rw-r--r--   0 giadarol   (503) staff       (20)       49 2023-04-03 19:29:39.000000 xmask-0.2.2/xmask.egg-info/requires.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        6 2023-04-03 19:29:39.000000 xmask-0.2.2/xmask.egg-info/top_level.txt
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-07 06:54:18.010465 xmask-0.3.0/
+-rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:05:06.000000 xmask-0.3.0/LICENSE
+-rw-r--r--   0 giadarol   (503) staff       (20)      237 2023-03-23 11:05:06.000000 xmask-0.3.0/MANIFEST.in
+-rw-r--r--   0 giadarol   (503) staff       (20)      520 2023-05-07 06:54:18.010324 xmask-0.3.0/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)      115 2023-03-23 11:05:06.000000 xmask-0.3.0/pyproject.toml
+-rw-r--r--   0 giadarol   (503) staff       (20)       38 2023-05-07 06:54:18.010511 xmask-0.3.0/setup.cfg
+-rw-r--r--   0 giadarol   (503) staff       (20)     1433 2023-03-23 11:05:06.000000 xmask-0.3.0/setup.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-07 06:54:18.008472 xmask-0.3.0/xmask/
+-rw-r--r--   0 giadarol   (503) staff       (20)      233 2023-03-23 11:05:06.000000 xmask-0.3.0/xmask/__init__.py
+-rw-r--r--   0 giadarol   (503) staff       (20)       22 2023-05-07 06:54:02.000000 xmask-0.3.0/xmask/_version.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      225 2023-03-23 11:05:06.000000 xmask-0.3.0/xmask/env_and_links.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-07 06:54:18.010131 xmask-0.3.0/xmask/lhc/
+-rw-r--r--   0 giadarol   (503) staff       (20)      432 2023-05-07 06:53:44.000000 xmask-0.3.0/xmask/lhc/__init__.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     5652 2023-05-07 06:53:44.000000 xmask-0.3.0/xmask/lhc/build_madx_and_xsuite_models.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     3553 2023-03-23 11:05:06.000000 xmask-0.3.0/xmask/lhc/errors.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2430 2023-05-07 06:53:44.000000 xmask-0.3.0/xmask/lhc/knob_manipulations.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     3231 2023-05-07 06:53:44.000000 xmask-0.3.0/xmask/lhc/leveling.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    12355 2023-05-07 06:53:44.000000 xmask-0.3.0/xmask/madx_model.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2883 2023-05-07 06:53:44.000000 xmask-0.3.0/xmask/tuning.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      728 2023-03-23 11:05:06.000000 xmask-0.3.0/xmask/yaml.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-07 06:54:18.009271 xmask-0.3.0/xmask.egg-info/
+-rw-r--r--   0 giadarol   (503) staff       (20)      520 2023-05-07 06:54:17.000000 xmask-0.3.0/xmask.egg-info/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)      434 2023-05-07 06:54:17.000000 xmask-0.3.0/xmask.egg-info/SOURCES.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        1 2023-05-07 06:54:17.000000 xmask-0.3.0/xmask.egg-info/dependency_links.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)       49 2023-05-07 06:54:17.000000 xmask-0.3.0/xmask.egg-info/requires.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        6 2023-05-07 06:54:17.000000 xmask-0.3.0/xmask.egg-info/top_level.txt
```

### Comparing `xmask-0.2.2/LICENSE` & `xmask-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xmask-0.2.2/PKG-INFO` & `xmask-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmask
-Version: 0.2.2
+Version: 0.3.0
 Summary: Configuration of tracking simulations for the LHC and other accelerators
 Home-page: https://github.com/xsuite/xsuite/issues
 Download-URL: https://pypi.python.org/pypi/xmask
 Author: G. Iadarola et al.
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
 Project-URL: Source Code, https://github.com/xsuite/xmask/
```

### Comparing `xmask-0.2.2/setup.py` & `xmask-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `xmask-0.2.2/xmask/lhc/build_madx_and_xsuite_models.py` & `xmask-0.3.0/xmask/lhc/build_madx_and_xsuite_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 
 def build_xsuite_collider(
     sequence_b1, sequence_b2, sequence_b4, beam_config,
     enable_imperfections,
     install_apertures=False,
     enable_knob_synthesis=False,
+    rename_coupling_knobs=False,
     pars_for_imperfections={},
     ver_lhc_run=None,
     ver_hllhc_optics=None,
     call_after_last_use=None,):
 
     """
     Build xsuite collider from madx sequences and optics.
@@ -45,14 +46,16 @@
         Dictionary with beam configuration (see examples)
     enable_imperfections: bool
         If True, lattice imperfections are installed and corrected
     install_apertures: bool
         If True, apertures are installed
     enable_knob_synthesis: bool
         If True, knobs (linear coupling) are synthesized
+    rename_coupling_knobs: bool
+        If True, coupling knobs are renamed to avoid clashes between b1 and b2
     pars_for_imperfections: dict
         Dictionary with parameters for imperfections configuration (see examples)
     ver_lhc_run: str
         Version of LHC optics (None if HL-LHC)
     ver_hllhc_optics: str
         Version of HL-LHC optics (None if LHC)
     call_after_last_use: callable
@@ -68,22 +71,21 @@
     if sequence_b4 is not None:
         assert sequence_b2 is not None, 'If b4 provided, b2 must be provided'
 
     for beam_n, sequence in zip((1, 2), [sequence_b1, sequence_b2]):
         if sequence is None: continue
         xm.attach_beam_to_sequence(sequence, beam_to_configure=beam_n,
                             beam_configuration=beam_config[sequence.name])
-        sequence._madx.globals.nrj = beam_config[sequence.name]['beam_energy_tot']
         # Warm up (seems I need to twiss for mad to load everything)
         sequence._madx.use(sequence.name)
         sequence._madx.twiss()
 
     # Store energy in nrj
     if sequence_b4 is not None:
-        sequence_b4._madx.globals.nrj = beam_config[sequence_b4.name]['beam_energy_tot']
+        sequence_b4._madx.globals.nrj = sequence_b2._madx.globals.nrj
 
     # Generate beam 4
     if sequence_b4 is not None:
         xm.configure_b4_from_b2(sequence_b4=sequence_b4, sequence_b2=sequence_b2)
 
     # Save lines for closed orbit reference
     lines_co_ref = xm.save_lines_for_closed_orbit_reference(
@@ -124,25 +126,32 @@
             install_apertures=install_apertures,
             replace_in_expr={'bv_aux': 'bvaux_'+sequence_name})
         mad_beam = mad_track.sequence[sequence_name].beam
         line.particle_ref = xp.Particles(p0c = mad_beam.pc*1e9,
             q0 = mad_beam.charge, mass0 = mad_beam.mass*1e9)
 
         # Prepare coupling and octupole knobs
-        rename_coupling_knobs_and_coefficients(line=line,
-                                            beamn=int(sequence_name[-1]))
-        define_octupole_current_knobs(line=line, beamn=int(sequence_name[-1]))
+        if rename_coupling_knobs:
+            rename_coupling_knobs_and_coefficients(line=line,
+                                    beamn=int(sequence_name[-1]))
+
         lines_to_track[sequence_name] = line
 
     lines = {}
     lines.update(lines_to_track)
     lines.update(lines_co_ref)
+
+    if 'lhcb1' in lines_to_track:
+        lines['lhcb1_co_ref'].particle_ref = lines['lhcb1'].particle_ref.copy()
+    if 'lhcb2' in lines_to_track:
+        lines['lhcb2_co_ref'].particle_ref = lines['lhcb2'].particle_ref.copy()
+
     collider = xt.Multiline(lines=lines)
 
     if 'lhcb1' in lines_to_track:
-        collider['lhcb1_co_ref'].particle_ref = collider['lhcb1'].particle_ref.copy()
+        define_octupole_current_knobs(line=collider.lhcb1, beamn=1)
     if 'lhcb2' in lines_to_track:
-        collider['lhcb2_co_ref'].particle_ref = collider['lhcb2'].particle_ref.copy()
+        define_octupole_current_knobs(line=collider.lhcb2, beamn=2)
 
     add_correction_term_to_dipole_correctors(collider)
 
     return collider
```

### Comparing `xmask-0.2.2/xmask/lhc/errors.py` & `xmask-0.3.0/xmask/lhc/errors.py`

 * *Files identical despite different names*

### Comparing `xmask-0.2.2/xmask/lhc/knob_manipulations.py` & `xmask-0.3.0/xmask/lhc/knob_manipulations.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
                     assert '"' not in kqs_knob_str
                     var_name = kqs_knob_str.split("'")[1]
                     assert var_name.startswith('kqs')
                     line.vars[var_name] += (line.vars[new_name]
                                 * line.vars[f'c_minus_{nn}_b{beamn}'])
 
 def define_octupole_current_knobs(line, beamn):
+
     line.vars[f'p0c_b{beamn}'] = line.particle_ref.p0c[0]
     line.vars[f'q0_b{beamn}'] = line.particle_ref.q0
     line.vars[f'brho0_b{beamn}'] = (line.vars[f'p0c_b{beamn}']
                                 / line.vars[f'q0_b{beamn}'] / clight)
 
     line.vars[f'i_oct_b{beamn}'] = 0
     for ss in '12 23 34 45 56 67 78 81'.split():
```

### Comparing `xmask-0.2.2/xmask/madx_model.py` & `xmask-0.3.0/xmask/madx_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,39 +34,43 @@
 
     if 'particle_charge' in beam_configuration.keys():
         particle_charge = beam_configuration['particle_charge']
         particle_type = 'ion'
     else:
         particle_charge = 1.
 
-    gamma_rel = (particle_charge*beam_configuration['beam_energy_tot'])/particle_mass
+    gamma_rel = (beam_configuration['beam_energy_tot'])/particle_mass
     # bv and bv_aux flags
     if beam_to_configure == 1:
         ss_beam_bv, ss_bv_aux = 1, 1
     elif beam_to_configure == 2:
         ss_beam_bv, ss_bv_aux = -1, 1
     elif beam_to_configure == 4:
         ss_beam_bv, ss_bv_aux = 1, -1
     else:
         raise ValueError("beam_to_configure must be 1, 2 or 4")
 
     mad.globals['bv_aux'] = ss_bv_aux
     mad.input(f'''
     beam, particle={particle_type},sequence={sequence.name},
-        energy={beam_configuration['beam_energy_tot']*particle_charge},
+        energy={beam_configuration['beam_energy_tot']},
         sigt={beam_configuration.get('beam_sigt', 0.0001)},
         bv={ss_beam_bv},
         npart={beam_configuration.get('beam_npart', 1)},
         sige={beam_configuration.get('beam_sige', 1e-6)},
         ex={beam_configuration.get('beam_norm_emit_x', 1) * 1e-6 / gamma_rel},
         ey={beam_configuration.get('beam_norm_emit_y', 1) * 1e-6 / gamma_rel},
         mass={particle_mass},
         charge={particle_charge};
     ''')
 
+    # Used for the rescaling of spectrometers
+    mad.use(sequence.name)
+    mad.globals.nrj = sequence.beam.energy / sequence.beam.charge
+
 def save_lines_for_closed_orbit_reference(sequence_clockwise, sequence_anticlockwise):
 
     lines_co_ref = {}
     if sequence_clockwise is not None:
         name_cw = sequence_clockwise.name
         lines_co_ref[name_cw + '_co_ref'] = xt.Line.from_madx_sequence(
             sequence_clockwise,
@@ -252,15 +256,15 @@
 def _dependent_variables_df(mad):
     '''
     Extract the pandas DF with the dependent variables of the MAD-X handle.
 
     Returns:
         The pandas DF of the dependent variables. The columns of the DF correspond to the
         - the numerical value of the dependent variable (value)
-        - the string corrensponding to the MAD-X expression (expression)
+        - the string corresponding to the MAD-X expression (expression)
         - the list of parameters used in the expression (parameters)
         - the list of the fundamental independent variables.
             These are independent variables that control numerical values of the variable (knobs).
 
     See madxp/examples/variablesExamples/000_run.py
     '''
     my_dict={}
```

### Comparing `xmask-0.2.2/xmask/tuning.py` & `xmask-0.3.0/xmask/tuning.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 from pathlib import Path
 
 import xtrack as xt
 
 def machine_tuning(line,
-        enable_closed_orbit_correction=True,
-        enable_linear_coupling_correction=True,
-        enable_tune_correction=True,
-        enable_chromaticity_correction=True,
+        enable_closed_orbit_correction=False,
+        enable_linear_coupling_correction=False,
+        enable_tune_correction=False,
+        enable_chromaticity_correction=False,
         knob_names=None,
         targets=None,
         line_co_ref=None, co_corr_config=None,
         verbose=False):
 
     # Correct closed orbit
     if enable_closed_orbit_correction:
```

### Comparing `xmask-0.2.2/xmask/yaml.py` & `xmask-0.3.0/xmask/yaml.py`

 * *Files identical despite different names*

### Comparing `xmask-0.2.2/xmask.egg-info/PKG-INFO` & `xmask-0.3.0/xmask.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmask
-Version: 0.2.2
+Version: 0.3.0
 Summary: Configuration of tracking simulations for the LHC and other accelerators
 Home-page: https://github.com/xsuite/xsuite/issues
 Download-URL: https://pypi.python.org/pypi/xmask
 Author: G. Iadarola et al.
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
 Project-URL: Source Code, https://github.com/xsuite/xmask/
```

