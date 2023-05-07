# Comparing `tmp/openlane-2.0.0a8.tar.gz` & `tmp/openlane-2.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlane-2.0.0a8.tar", last modified: Tue Mar 21 14:08:17 2023, max compression
+gzip compressed data, was "openlane-2.0.0a9.tar", last modified: Tue Mar 28 20:05:45 2023, max compression
```

## Comparing `openlane-2.0.0a8.tar` & `openlane-2.0.0a9.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:08:17.881924 openlane-2.0.0a8/
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-03-21 14:08:17.881924 openlane-2.0.0a8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:08:17.865924 openlane-2.0.0a8/openlane/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:08:17.869924 openlane-2.0.0a8/openlane/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/config/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/config/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    17026 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/config/pdk.py
--rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/config/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/config/tcleval.py
--rw-r--r--   0 runner    (1001) docker     (123)    12973 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/config/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/env_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:08:17.869924 openlane-2.0.0a8/openlane/flows/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/flows/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/flows/classic.py
--rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/flows/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/flows/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/flows/optimizing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/flows/sequential.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/open_pdks_rev
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:08:17.869924 openlane-2.0.0a8/openlane/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/base.sdc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:08:17.869924 openlane-2.0.0a8/openlane/scripts/klayout/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/klayout/Readme.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     2681 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/klayout/open_design.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4581 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/klayout/render.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6482 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/klayout/stream_out.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2758 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/klayout/xor.drc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:08:17.869924 openlane-2.0.0a8/openlane/scripts/magic/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/magic/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:08:17.869924 openlane-2.0.0a8/openlane/scripts/magic/def/
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/magic/def/antenna_check.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/magic/def/mag.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2699 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/magic/def/mag_gds.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/magic/def/read.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2320 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/magic/drc.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/magic/extract_spice.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:08:17.869924 openlane-2.0.0a8/openlane/scripts/magic/gds/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2198 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/magic/gds/drc_batch.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/magic/gds/erase_box.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1353 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/magic/gds/extras_mag.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/magic/gds/mag_with_pointers.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/magic/gds/read.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:08:17.869924 openlane-2.0.0a8/openlane/scripts/magic/lef/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1594 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/magic/lef/extras_maglef.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      863 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/magic/lef/maglef.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:08:17.869924 openlane-2.0.0a8/openlane/scripts/magic/mag/
--rwxr-xr-x   0 runner    (1001) docker     (123)      579 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/magic/mag/lef.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:08:17.869924 openlane-2.0.0a8/openlane/scripts/odbpy/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/odbpy/apply_def_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/odbpy/contextualize.py
--rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/odbpy/defutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/odbpy/diodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/odbpy/io_place.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/odbpy/label_macro_pins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/odbpy/lefutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/odbpy/manual_macro_place.py
--rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/odbpy/padringer.py
--rw-r--r--   0 runner    (1001) docker     (123)    39971 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/odbpy/power_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/odbpy/random_place.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/odbpy/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/odbpy/remove_buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/odbpy/snap_to_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/odbpy/wire_lengths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:08:17.873924 openlane-2.0.0a8/openlane/scripts/openroad/
--rwxr-xr-x   0 runner    (1001) docker     (123)      741 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/basic_mp.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      785 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/check_antennae.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:08:17.873924 openlane-2.0.0a8/openlane/scripts/openroad/common/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/common/dpl.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/common/dpl_cell_pad.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/common/grt.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/common/io.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/common/pdn_cfg.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/common/resizer.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/common/set_global_connections.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/common/set_layer_adjustments.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/common/set_power_nets.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/common/set_rc.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/common/set_routing_layers.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3151 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/cts.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/dpl.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1159 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/drt.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      708 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/fill.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     3592 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/floorplan.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     2136 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/gpl.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/grt.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/gui.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/insert_buffer.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     1635 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/ioplacer.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/irdrop.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/pdn.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/rcx.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/repair_design.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/rsz_timing_postcts.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/rsz_timing_postgrt.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/sta.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)     8648 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/sta_multi_corner.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      889 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/tapcell.tcl
--rwxr-xr-x   0 runner    (1001) docker     (123)      645 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/openroad/write_views.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:08:17.873924 openlane-2.0.0a8/openlane/scripts/tclsh/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/tclsh/hello.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:08:17.873924 openlane-2.0.0a8/openlane/scripts/yosys/
--rw-r--r--   0 runner    (1001) docker     (123)    14278 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/scripts/yosys/synthesize.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:08:17.873924 openlane-2.0.0a8/openlane/smoke_test_design/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/smoke_test_design/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:08:17.873924 openlane-2.0.0a8/openlane/smoke_test_design/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/smoke_test_design/src/spm.v
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:08:17.873924 openlane-2.0.0a8/openlane/state/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/state/design_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/state/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:08:17.881924 openlane-2.0.0a8/openlane/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/steps/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/steps/common_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/steps/klayout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/steps/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/steps/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/steps/netgen.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/steps/odb.py
--rw-r--r--   0 runner    (1001) docker     (123)    35176 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/steps/openroad.py
--rw-r--r--   0 runner    (1001) docker     (123)    18838 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/steps/step.py
--rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/steps/tclstep.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/steps/yosys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:08:17.881924 openlane-2.0.0a8/openlane/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/utils/drc.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/utils/memoize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-03-21 14:02:18.000000 openlane-2.0.0a8/openlane/utils/toolbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:08:17.865924 openlane-2.0.0a8/openlane.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-03-21 14:08:17.000000 openlane-2.0.0a8/openlane.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-03-21 14:08:17.000000 openlane-2.0.0a8/openlane.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 14:08:17.000000 openlane-2.0.0a8/openlane.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-21 14:08:17.000000 openlane-2.0.0a8/openlane.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-21 14:08:17.000000 openlane-2.0.0a8/openlane.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-21 14:08:17.000000 openlane-2.0.0a8/openlane.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 14:08:17.881924 openlane-2.0.0a8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1391 2023-03-21 14:02:18.000000 openlane-2.0.0a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.087321 openlane-2.0.0a9/
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-03-28 20:05:45.087321 openlane-2.0.0a9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.075321 openlane-2.0.0a9/openlane/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.079321 openlane-2.0.0a9/openlane/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/config/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/config/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16694 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/config/pdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/config/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/config/tcleval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/config/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/env_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.079321 openlane-2.0.0a9/openlane/flows/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/flows/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/flows/classic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/flows/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/flows/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/flows/optimizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/flows/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/open_pdks_rev
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.079321 openlane-2.0.0a9/openlane/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/base.sdc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.079321 openlane-2.0.0a9/openlane/scripts/klayout/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/klayout/Readme.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2681 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/klayout/open_design.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4581 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/klayout/render.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6482 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/klayout/stream_out.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2758 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/klayout/xor.drc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.079321 openlane-2.0.0a9/openlane/scripts/magic/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.079321 openlane-2.0.0a9/openlane/scripts/magic/def/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/def/antenna_check.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/def/mag.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2699 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/def/mag_gds.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/def/read.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2320 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/drc.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/extract_spice.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.079321 openlane-2.0.0a9/openlane/scripts/magic/gds/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2198 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/gds/drc_batch.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/gds/erase_box.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1353 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/gds/extras_mag.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/gds/mag_with_pointers.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/gds/read.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.079321 openlane-2.0.0a9/openlane/scripts/magic/lef/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1594 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/lef/extras_maglef.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      863 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/lef/maglef.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.079321 openlane-2.0.0a9/openlane/scripts/magic/mag/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      579 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/magic/mag/lef.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.083321 openlane-2.0.0a9/openlane/scripts/odbpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/apply_def_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/contextualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/defutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/diodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/io_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/label_macro_pins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/lefutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/manual_macro_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/padringer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39971 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/power_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/random_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/remove_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/snap_to_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/odbpy/wire_lengths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.083321 openlane-2.0.0a9/openlane/scripts/openroad/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      741 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/basic_mp.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      785 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/check_antennae.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.083321 openlane-2.0.0a9/openlane/scripts/openroad/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/common/dpl.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/common/dpl_cell_pad.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/common/grt.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/common/io.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/common/pdn_cfg.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/common/resizer.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/common/set_global_connections.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/common/set_layer_adjustments.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/common/set_power_nets.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/common/set_rc.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/common/set_routing_layers.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3151 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/cts.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/dpl.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1159 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/drt.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      708 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/fill.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3592 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/floorplan.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2136 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/gpl.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/grt.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/gui.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/insert_buffer.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1635 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/ioplacer.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/irdrop.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/pdn.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/rcx.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/repair_design.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/rsz_timing_postcts.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/rsz_timing_postgrt.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/sta.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8648 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/sta_multi_corner.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      889 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/tapcell.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (123)      645 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/openroad/write_views.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.083321 openlane-2.0.0a9/openlane/scripts/tclsh/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/tclsh/hello.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.083321 openlane-2.0.0a9/openlane/scripts/yosys/
+-rw-r--r--   0 runner    (1001) docker     (123)    14278 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/scripts/yosys/synthesize.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.083321 openlane-2.0.0a9/openlane/smoke_test_design/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/smoke_test_design/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.083321 openlane-2.0.0a9/openlane/smoke_test_design/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/smoke_test_design/src/spm.v
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.083321 openlane-2.0.0a9/openlane/state/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/state/design_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/state/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.087321 openlane-2.0.0a9/openlane/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/common_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/klayout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/netgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/odb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35320 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/openroad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18839 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/tclstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/steps/yosys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.087321 openlane-2.0.0a9/openlane/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/utils/drc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/utils/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-03-28 19:59:10.000000 openlane-2.0.0a9/openlane/utils/toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 20:05:45.079321 openlane-2.0.0a9/openlane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-03-28 20:05:44.000000 openlane-2.0.0a9/openlane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-03-28 20:05:44.000000 openlane-2.0.0a9/openlane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 20:05:44.000000 openlane-2.0.0a9/openlane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-28 20:05:44.000000 openlane-2.0.0a9/openlane.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-28 20:05:44.000000 openlane-2.0.0a9/openlane.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-28 20:05:44.000000 openlane-2.0.0a9/openlane.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 20:05:45.087321 openlane-2.0.0a9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1391 2023-03-28 19:59:10.000000 openlane-2.0.0a9/setup.py
```

### Comparing `openlane-2.0.0a8/PKG-INFO` & `openlane-2.0.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlane
-Version: 2.0.0a8
+Version: 2.0.0a9
 Summary: An infrastructure for implementing chip design flows
 Home-page: UNKNOWN
 Author: Efabless Corporation and Contributors
 Author-email: donn@efabless.com
 License: UNKNOWN
 Description: > Efabless OpenLane 2 is in early access and all APIs are, presently, highly unstable and subject to change without notice.
         >
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openlane Version: 2.0.0a8 Summary: An
+Metadata-Version: 2.1 Name: openlane Version: 2.0.0a9 Summary: An
 infrastructure for implementing chip design flows Home-page: UNKNOWN Author:
 Efabless Corporation and Contributors Author-email: donn@efabless.com License:
 UNKNOWN Description: > Efabless OpenLane 2 is in early access and all APIs are,
 presently, highly unstable and subject to change without notice. > > If you
 don't know why you're here, you're probably looking for the stable version of
 OpenLane at https://github.com/The-OpenROAD-Project/OpenLane.
                             ****** OpenLane ******
```

### Comparing `openlane-2.0.0a8/openlane/__init__.py` & `openlane-2.0.0a9/openlane/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/__main__.py` & `openlane-2.0.0a9/openlane/__main__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/__version__.py` & `openlane-2.0.0a9/openlane/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "2.0.0a8"
+__version__ = "2.0.0a9"
 
 if __name__ == "__main__":
     print(__version__, end="")
```

### Comparing `openlane-2.0.0a8/openlane/common.py` & `openlane-2.0.0a9/openlane/common.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/config/__init__.py` & `openlane-2.0.0a9/openlane/config/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/config/builder.py` & `openlane-2.0.0a9/openlane/config/builder.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/config/config.py` & `openlane-2.0.0a9/openlane/config/config.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/config/flow.py` & `openlane-2.0.0a9/openlane/config/flow.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/config/pdk.py` & `openlane-2.0.0a9/openlane/config/pdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -458,41 +458,35 @@
         "PLACE_SITE_HEIGHT",
         Decimal,
         "The site height for the previously designated place site.",
         units="µm",
     ),
     Variable(
         "GPL_CELL_PADDING",
-        Optional[Decimal],
-        "Cell padding value (in sites) for global placement. Using this is not recommended as you can simply use the density control for global placement.",
+        Decimal,
+        "Cell padding value (in sites) for global placement. The number will be integer divided by 2 and placed on both sides.",
         units="sites",
     ),
     Variable(
         "DPL_CELL_PADDING",
         Decimal,
-        "Defines the number of sites to pad the cells lef views with during detailed placement. The number will be integer divided by 2 and placed on both sides.",
+        "Cell padding value (in sites) for detailed placement. The number will be integer divided by 2 and placed on both sides. Should be <= global placement.",
         units="sites",
     ),
     Variable(
         "CELL_PAD_EXCLUDE",
         List[str],
         "Defines a list of cells to be excluded from cell padding.",
     ),
     # Antenna
     Variable(
         "DIODE_CELL",
         Optional[str],
         "Defines a diode cell used to fix antenna violations, in the format {name}/{port}.",
     ),
-    Variable(
-        "HEURISTIC_ANTENNA_THRESHOLD",
-        Optional[Decimal],
-        "A manhattan distance above which a diode is recommended to be inserted by a heuristic inserter. If not specified, the heuristic inserter will typically use a default value.",
-        units="µm",
-    ),
     # Routing
     Variable(
         "GRT_LAYER_ADJUSTMENTS",
         List[Decimal],
         "Layer-specific reductions in the routing capacity of the edges between the cells in the global routing graph, delimited by commas. Values range from 0 through 1.",
     ),
     # CVC
```

### Comparing `openlane-2.0.0a8/openlane/config/resolve.py` & `openlane-2.0.0a9/openlane/config/resolve.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/config/tcleval.py` & `openlane-2.0.0a9/openlane/config/tcleval.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/config/variable.py` & `openlane-2.0.0a9/openlane/config/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,14 +339,15 @@
 
                 config["GRT_REPAIR_ANTENNAS"] = False
                 config["RUN_HEURISTIC_DIODE_INSERTION"] = False
                 if dis in [3, 6]:
                     config["GRT_REPAIR_ANTENNAS"] = True
                 if dis in [5, 6]:
                     config["RUN_HEURISTIC_DIODE_INSERTION"] = True
+                    config["DIODE_ON_PORTS"] = "in"
 
             del mutable["DIODE_INSERTION_STRATEGY"]
 
         for variable in variables:
             try:
                 value_processed = variable._compile(
                     mutable_config=mutable,
```

### Comparing `openlane-2.0.0a8/openlane/container.py` & `openlane-2.0.0a9/openlane/container.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/env_info.py` & `openlane-2.0.0a9/openlane/env_info.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/flows/__init__.py` & `openlane-2.0.0a9/openlane/flows/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/flows/builtins.py` & `openlane-2.0.0a9/openlane/flows/builtins.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/flows/classic.py` & `openlane-2.0.0a9/openlane/flows/classic.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,17 @@
         Odb.ManualMacroPlacement,
         Odb.ApplyDEFTemplate,
         OpenROAD.TapDecapInsertion,
         OpenROAD.IOPlacement,
         Odb.CustomIOPlacement,
         OpenROAD.GeneratePDN,
         OpenROAD.GlobalPlacement,
-        OpenROAD.RepairDesign,
+        Odb.DiodesOnPorts,
         Odb.HeuristicDiodeInsertion,
+        OpenROAD.RepairDesign,
         OpenROAD.DetailedPlacement,
         OpenROAD.CTS,
         OpenROAD.ResizerTimingPostCTS,
         OpenROAD.GlobalRouting,
         OpenROAD.ResizerTimingPostGRT,
         OpenROAD.DetailedRouting,
         Checker.TrDRC,
```

### Comparing `openlane-2.0.0a8/openlane/flows/flow.py` & `openlane-2.0.0a9/openlane/flows/flow.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/flows/misc.py` & `openlane-2.0.0a9/openlane/flows/misc.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/flows/optimizing.py` & `openlane-2.0.0a9/openlane/flows/optimizing.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/flows/sequential.py` & `openlane-2.0.0a9/openlane/flows/sequential.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/logging.py` & `openlane-2.0.0a9/openlane/logging.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/base.sdc` & `openlane-2.0.0a9/openlane/scripts/base.sdc`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/klayout/open_design.py` & `openlane-2.0.0a9/openlane/scripts/klayout/open_design.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/klayout/render.py` & `openlane-2.0.0a9/openlane/scripts/klayout/render.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/klayout/stream_out.py` & `openlane-2.0.0a9/openlane/scripts/klayout/stream_out.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/klayout/xor.drc` & `openlane-2.0.0a9/openlane/scripts/klayout/xor.drc`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/magic/def/antenna_check.tcl` & `openlane-2.0.0a9/openlane/scripts/magic/def/antenna_check.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/magic/def/mag.tcl` & `openlane-2.0.0a9/openlane/scripts/magic/def/mag.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/magic/def/mag_gds.tcl` & `openlane-2.0.0a9/openlane/scripts/magic/def/mag_gds.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/magic/def/read.tcl` & `openlane-2.0.0a9/openlane/scripts/magic/def/read.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/magic/drc.tcl` & `openlane-2.0.0a9/openlane/scripts/magic/drc.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/magic/extract_spice.tcl` & `openlane-2.0.0a9/openlane/scripts/magic/extract_spice.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/magic/gds/drc_batch.tcl` & `openlane-2.0.0a9/openlane/scripts/magic/gds/drc_batch.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/magic/gds/erase_box.tcl` & `openlane-2.0.0a9/openlane/scripts/magic/gds/erase_box.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/magic/gds/extras_mag.tcl` & `openlane-2.0.0a9/openlane/scripts/magic/gds/extras_mag.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/magic/gds/mag_with_pointers.tcl` & `openlane-2.0.0a9/openlane/scripts/magic/gds/mag_with_pointers.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/magic/gds/read.tcl` & `openlane-2.0.0a9/openlane/scripts/magic/gds/read.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/magic/lef/extras_maglef.tcl` & `openlane-2.0.0a9/openlane/scripts/magic/lef/extras_maglef.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/magic/lef/maglef.tcl` & `openlane-2.0.0a9/openlane/scripts/magic/lef/maglef.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/magic/mag/lef.tcl` & `openlane-2.0.0a9/openlane/scripts/magic/mag/lef.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/odbpy/apply_def_template.py` & `openlane-2.0.0a9/openlane/scripts/odbpy/apply_def_template.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/odbpy/contextualize.py` & `openlane-2.0.0a9/openlane/scripts/odbpy/contextualize.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/odbpy/defutil.py` & `openlane-2.0.0a9/openlane/scripts/odbpy/defutil.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/odbpy/diodes.py` & `openlane-2.0.0a9/openlane/scripts/odbpy/diodes.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,83 +12,52 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import odb
 
-import re
 import sys
+import click
 import random
 from decimal import Decimal
 
-from reader import click_odb, click
+from reader import click_odb
 
 
 @click.group()
 def cli():
     pass
 
 
 class DiodeInserter:
     def __init__(
         self,
         block,
         diode_cell,
         diode_pin,
-        fake_diode_cell=None,
         side_strategy="source",
-        threshold=0,
+        threshold_microns=0,
         port_protect=[],
         verbose=False,
     ):
         self.block = block
         self.verbose = verbose
 
         self.diode_cell = diode_cell
         self.diode_pin = diode_pin
-        self.fake_diode_cell = fake_diode_cell
         self.side_strategy = side_strategy
-        self.threshold = threshold
+        self.threshold_microns = threshold_microns
         self.port_protect = port_protect
 
-        self.true_diode_master = block.getDataBase().findMaster(diode_cell)
-        self.fake_diode_master = (
-            block.getDataBase().findMaster(fake_diode_cell)
-            if (fake_diode_cell is not None)
-            else None
-        )
-        if not self.check():
-            raise RuntimeError("True and Fake diodes are inconsistent")
-
-        self.diode_master = self.fake_diode_master or self.true_diode_master
-        self.diode_site = self.true_diode_master.getSite().getConstName()
+        self.diode_master = block.getDataBase().findMaster(diode_cell)
+        self.diode_site = self.diode_master.getSite().getConstName()
 
         self.inserted = {}
 
-    def check(self):
-        if self.fake_diode_master is None:
-            return True
-
-        tm = self.true_diode_master
-        fm = self.fake_diode_master
-
-        if fm.getSite() is None:
-            self.error("[!] Fake diode cell missing SITE attribute")
-        else:
-            if fm.getSite().getConstName() != tm.getSite().getConstName():
-                return False
-
-        if fm.getWidth() != tm.getWidth():
-            return False
-        if fm.getHeight() != tm.getHeight():
-            return False
-
-        return True
-
     def debug(self, msg):
         if self.verbose:
             print(msg, file=sys.stderr)
 
     def error(self, msg):
         print(msg, file=sys.stderr)
 
@@ -126,15 +95,15 @@
             cell_type = it.getInst().getMaster().getConstName()
             cell_pin = it.getMTerm().getConstName()
             if (cell_type == self.diode_cell) and (cell_pin == self.diode_pin):
                 return True
         else:
             return False
 
-    def net_span(self, net):
+    def net_manhattan_distance(self, net):
         xs = []
         ys = []
 
         for bt in net.getBTerms():
             good, x, y = bt.getFirstPinLocation()
             if good:
                 xs.append(x)
@@ -226,15 +195,15 @@
             d = abs(px - dx) + abs(py - dy)
 
             if (best is None) or (best[0] > d):
                 best = (d, dx, dy, do)
 
         return best[1:]
 
-    def insert_diode(self, it, src_pos, force_true=False):
+    def insert_diode(self, it, src_pos):
         # Get information about the instance
         inst = it.getInst()
         inst_name = inst.getConstName()
         inst_site = (
             inst.getMaster().getSite().getConstName()
             if (inst.getMaster().getSite() is not None)
             else None
@@ -247,15 +216,15 @@
         if inst_site == self.diode_site:
             dx, dy, do = self.place_diode_stdcell(it, px, py, src_pos)
         else:
             dx, dy, do = self.place_diode_macro(it, px, py, src_pos)
 
         # Insert instance and wire it up
         diode_inst_name = "ANTENNA_" + inst_name + "_" + it.getMTerm().getConstName()
-        diode_master = self.true_diode_master if force_true else self.diode_master
+        diode_master = self.diode_master
 
         diode_inst = odb.dbInst_create(self.block, diode_master, diode_inst_name)
 
         diode_inst.setOrient(do)
         diode_inst.setLocation(dx, dy)
         diode_inst.setPlacementStatus("PLACED")
 
@@ -278,49 +247,48 @@
                 )
                 continue
 
             # Find signal source (first one found ...)
             src_pos = self.net_source(net)
 
             # Is this an IO we need to protect
-            io_protect = self.net_from_pin(net, io_types=self.port_protect)
-            if io_protect:
-                self.debug(
-                    f"[d] Forcing protection diode on net  {net.getConstName():s}"
-                )
+            io_protect = None
+            if self.net_from_pin(net, io_types=["INPUT", "OUTPUT"]):
+                io_protect = self.net_from_pin(net, io_types=self.port_protect)
+                if io_protect:
+                    self.debug(
+                        f"[d] Forcing protection diode on I/O net {net.getConstName():s}"
+                    )
+                else:
+                    self.debug(f"[d] Skipping I/O net {net.getConstName():s}")
+                    continue
 
             # Determine the span of the signal and skip small internal nets
-            span = self.net_span(net)
-            if (span < self.threshold) and not io_protect:
-                self.debug(f"[d] Skipping small net {net.getConstName():s} ({span:d})")
+            span = self.net_manhattan_distance(net) / self.block.getDbUnitsPerMicron()
+            if (span < self.threshold_microns) and not io_protect:
+                self.debug(f"[d] Skipping small net {net.getConstName():s} ({span:f})")
                 continue
 
             # Scan all internal terminals
             for it in net.getITerms():
                 if it.isInputSignal():
-                    self.insert_diode(it, src_pos, force_true=io_protect)
+                    self.insert_diode(it, src_pos)
 
 
 @click.command()
 @click.option(
     "-v", "--verbose", default=False, is_flag=True, help="Verbose debug output"
 )
 @click.option(
     "-c",
     "--diode-cell",
     default="sky130_fd_sc_hd__diode_2",
     help="Name of the cell to use as diode",
 )
 @click.option(
-    "-f",
-    "--fake-diode-cell",
-    default=None,
-    help="Name of the cell to use as fake diode",
-)
-@click.option(
     "-p", "--diode-pin", default="DIODE", help="Name of the pin to use on diode cells"
 )
 @click.option(
     "--side-strategy",
     type=click.Choice(["source", "pin", "balanced", "random"]),
     default="source",
     help="Strategy to select if placing diode left/right of the cell",
@@ -340,80 +308,41 @@
     help="Minimum manhattan distance of a net to be considered an antenna risk requiring a diode",
 )
 @click_odb
 def place(
     reader,
     verbose,
     diode_cell,
-    fake_diode_cell,
     diode_pin,
     side_strategy,
     port_protect,
     threshold_microns,
 ):
-    threshold = int(
-        threshold_microns * Decimal(reader.db.getTech().getDbUnitsPerMicron())
-    )
-    print(f"Inserting for nets >= {threshold} dbus ({threshold_microns} microns)...")
 
     print(f"Design name: {reader.name}")
 
     pp_val = {
         "none": [],
         "in": ["INPUT"],
         "out": ["OUTPUT"],
         "both": ["INPUT", "OUTPUT"],
     }
 
     di = DiodeInserter(
         reader.block,
         diode_cell=diode_cell,
         diode_pin=diode_pin,
-        fake_diode_cell=fake_diode_cell,
         side_strategy=side_strategy,
-        threshold=threshold,
+        threshold_microns=threshold_microns,
         port_protect=pp_val[port_protect],
         verbose=verbose,
     )
     di.execute()
 
     print("Inserted", len(di.inserted), "diodes.")
 
 
 cli.add_command(place)
 
 
-@click.command("replace_fake")
-@click.option("-f", "--fake-diode", required=True, help="Name of the fake diode cell")
-@click.option("-t", "--true-diode", required=True, help="Name of the true diode")
-@click.option(
-    "-v",
-    "--violations-file",
-    required=True,
-    help="Text file with white space separated cells that cause antenna violations",
-)
-@click_odb
-def replace_fake(fake_diode, true_diode, violations_file, reader):
-    violations = open(violations_file).read().strip().split()
-
-    diode = [sc for sc in reader.block.getMasters() if sc.getName() == true_diode]
-
-    antenna_rx = re.compile(r"ANTENNA_(\s+)_.*")
-
-    instances = reader.block.getInsts()
-
-    for instance in instances:
-        name: str = instance.getName()
-        m = antenna_rx.match(name)
-        if m is None:
-            continue
-        if m[1] not in violations:
-            continue
-        master_name = instance.getMaster().getName()
-        if master_name == fake_diode:
-            instance.swapMasters(diode)
-
-
-cli.add_command(replace_fake)
-
 if __name__ == "__main__":
     cli()
```

### Comparing `openlane-2.0.0a8/openlane/scripts/odbpy/io_place.py` & `openlane-2.0.0a9/openlane/scripts/odbpy/io_place.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/odbpy/label_macro_pins.py` & `openlane-2.0.0a9/openlane/scripts/odbpy/label_macro_pins.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/odbpy/lefutil.py` & `openlane-2.0.0a9/openlane/scripts/odbpy/lefutil.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/odbpy/manual_macro_place.py` & `openlane-2.0.0a9/openlane/scripts/odbpy/manual_macro_place.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/odbpy/padringer.py` & `openlane-2.0.0a9/openlane/scripts/odbpy/padringer.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/odbpy/power_utils.py` & `openlane-2.0.0a9/openlane/scripts/odbpy/power_utils.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/odbpy/random_place.py` & `openlane-2.0.0a9/openlane/scripts/odbpy/random_place.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/odbpy/reader.py` & `openlane-2.0.0a9/openlane/scripts/odbpy/reader.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/odbpy/remove_buffers.py` & `openlane-2.0.0a9/openlane/scripts/odbpy/remove_buffers.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/odbpy/snap_to_grid.py` & `openlane-2.0.0a9/openlane/scripts/odbpy/snap_to_grid.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/odbpy/wire_lengths.py` & `openlane-2.0.0a9/openlane/scripts/odbpy/wire_lengths.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/basic_mp.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/basic_mp.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/check_antennae.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/check_antennae.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/common/dpl.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/common/dpl.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/common/dpl_cell_pad.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/common/dpl_cell_pad.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/common/grt.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/common/grt.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/common/io.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/common/io.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/common/pdn_cfg.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/common/pdn_cfg.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/common/resizer.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/common/resizer.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/common/set_global_connections.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/common/set_global_connections.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/common/set_layer_adjustments.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/common/set_layer_adjustments.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/common/set_power_nets.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/common/set_power_nets.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/common/set_rc.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/common/set_rc.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/common/set_routing_layers.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/common/set_routing_layers.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/cts.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/cts.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/dpl.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/dpl.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/drt.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/drt.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/fill.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/fill.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/floorplan.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/floorplan.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/gpl.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/gpl.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/grt.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/grt.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/gui.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/gui.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/insert_buffer.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/insert_buffer.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/ioplacer.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/ioplacer.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/irdrop.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/irdrop.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/pdn.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/pdn.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/rcx.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/rcx.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/repair_design.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/repair_design.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/rsz_timing_postcts.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/rsz_timing_postcts.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/rsz_timing_postgrt.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/rsz_timing_postgrt.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/sta.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/sta.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/sta_multi_corner.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/sta_multi_corner.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/tapcell.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/tapcell.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/openroad/write_views.tcl` & `openlane-2.0.0a9/openlane/scripts/openroad/write_views.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/scripts/yosys/synthesize.tcl` & `openlane-2.0.0a9/openlane/scripts/yosys/synthesize.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/smoke_test_design/src/spm.v` & `openlane-2.0.0a9/openlane/smoke_test_design/src/spm.v`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/state/__init__.py` & `openlane-2.0.0a9/openlane/state/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/state/design_format.py` & `openlane-2.0.0a9/openlane/state/design_format.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/state/state.py` & `openlane-2.0.0a9/openlane/state/state.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/steps/__init__.py` & `openlane-2.0.0a9/openlane/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/steps/checker.py` & `openlane-2.0.0a9/openlane/steps/checker.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/steps/common_variables.py` & `openlane-2.0.0a9/openlane/steps/common_variables.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/steps/klayout.py` & `openlane-2.0.0a9/openlane/steps/klayout.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/steps/magic.py` & `openlane-2.0.0a9/openlane/steps/magic.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/steps/misc.py` & `openlane-2.0.0a9/openlane/steps/misc.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/steps/netgen.py` & `openlane-2.0.0a9/openlane/steps/netgen.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/steps/odb.py` & `openlane-2.0.0a9/openlane/steps/odb.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import re
 import sys
 import json
+from decimal import Decimal
 from abc import abstractmethod
 from typing import List, Optional
 
 
 from .step import Step
 from ..state import State
 from ..state import DesignFormat
 from .common_variables import io_layer_variables
 
 from ..config import Path, Variable, StringEnum
 from ..common import get_openlane_root, get_script_dir
+from ..logging import warn
 
 inf_rx = re.compile(r"\b(-?)inf\b")
 
 
 class OdbpyStep(Step):
     inputs = [DesignFormat.ODB]
     outputs = [DesignFormat.ODB, DesignFormat.DEF]
@@ -240,32 +242,80 @@
                 if self.config["QUIT_ON_UNMATCHED_IO"]
                 else "--ignore-unmatched"
             ),
         ]
 
 
 @Step.factory.register()
+class DiodesOnPorts(OdbpyStep):
+    id = "Odb.DiodesOnPorts"
+    name = "Diodes on Ports"
+    long_name = "Diode on Port Insertion Script"
+
+    config_vars = [
+        Variable(
+            "DIODE_ON_PORTS",
+            StringEnum("DIODE_ON_PORTS", ["none", "in", "out", "both"]),
+            "Always insert diodes on ports with the specified polarities.",
+            default="none",
+        ),
+    ]
+
+    def get_script_path(self):
+        return os.path.join(get_script_dir(), "odbpy", "diodes.py")
+
+    def get_subcommand(self) -> List[str]:
+        return ["place"]
+
+    def get_command(self) -> List[str]:
+        cell, pin = self.config["DIODE_CELL"].split("/")
+
+        return super().get_command() + [
+            "--threshold",
+            "Infinity",
+            "--diode-cell",
+            cell,
+            "--diode-pin",
+            pin,
+            "--port-protect",
+            self.config["DIODE_ON_PORTS"].value,
+        ]
+
+    def run(self, **kwargs) -> State:
+        if self.config["DIODE_ON_PORTS"].value == "none":
+            warn("'DIODE_ON_PORTS' is set to 'none': skipping…")
+            return Step.run(self, **kwargs)
+
+        if self.config["GPL_CELL_PADDING"] == 0:
+            warn(
+                "'GPL_CELL_PADDING' is set to 0. This step may cause overlap failures."
+            )
+
+        return super().run(**kwargs)
+
+
+@Step.factory.register()
 class HeuristicDiodeInsertion(OdbpyStep):
     id = "Odb.HeuristicDiodeInsertion"
     name = "Heuristic Diode Insertion"
     long_name = "Heuristic Diode Insertion Script"
 
     flow_control_variable = "RUN_HEURISTIC_DIODE_INSERTION"
     config_vars = [
         Variable(
             "RUN_HEURISTIC_DIODE_INSERTION",
             bool,
             "Enables/disables this step.",
             default=False,  # For compatibility with OL1. Yep.
         ),
         Variable(
-            "DIODE_ON_PORTS",
-            StringEnum("DIODE_ON_PORTS", ["none", "in", "out", "both"]),
-            "Always insert diodes on ports with the specified polarities.",
-            default="in",
+            "HEURISTIC_ANTENNA_THRESHOLD",
+            Optional[Decimal],
+            "A manhattan distance above which a diode is recommended to be inserted by a heuristic inserter. If not specified, the heuristic inserter will typically use a default value.",
+            units="µm",
         ),
     ]
 
     def get_script_path(self):
         return os.path.join(get_script_dir(), "odbpy", "diodes.py")
 
     def get_subcommand(self) -> List[str]:
@@ -281,12 +331,18 @@
         return (
             super().get_command()
             + [
                 "--diode-cell",
                 cell,
                 "--diode-pin",
                 pin,
-                "--port-protect",
-                self.config["DIODE_ON_PORTS"].value,
             ]
             + threshold_opts
         )
+
+    def run(self, **kwargs) -> State:
+        if self.config["GPL_CELL_PADDING"] == 0:
+            warn(
+                "'GPL_CELL_PADDING' is set to 0. This step may cause overlap failures."
+            )
+
+        return super().run(**kwargs)
```

### Comparing `openlane-2.0.0a8/openlane/steps/openroad.py` & `openlane-2.0.0a9/openlane/steps/openroad.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,15 +364,15 @@
     config_vars = (
         OpenROADStep.config_vars
         + routing_layer_variables
         + [
             Variable(
                 "PL_TARGET_DENSITY_PCT",
                 Optional[Decimal],
-                "The desired placement density of cells. If not specified, the value will be equal to `FP_CORE_UTIL` + 5%.",
+                "The desired placement density of cells. If not specified, the value will be equal to (`FP_CORE_UTIL` + 5 * `GPL_CELL_PADDING` + 10).",
                 units="%",
                 deprecated_names=[
                     ("PL_TARGET_DENSITY", lambda d: Decimal(d) * Decimal(100.0))
                 ],
             ),
             Variable(
                 "PL_TIME_DRIVEN",
@@ -402,15 +402,18 @@
     )
 
     def get_script_path(self):
         return os.path.join(get_script_dir(), "openroad", "gpl.tcl")
 
     def run(self, **kwargs) -> State:
         kwargs, env = self.extract_env(kwargs)
-        env["PL_TARGET_DENSITY_PCT"] = f"{self.config['FP_CORE_UTIL'] + 5}"
+        env[
+            "PL_TARGET_DENSITY_PCT"
+        ] = f"{self.config['FP_CORE_UTIL'] + (5 * self.config['GPL_CELL_PADDING']) + 10}"
+        # Overriden by super if the value is not None
         return super().run(env=env, **kwargs)
 
 
 @Step.factory.register()
 class BasicMacroPlacement(OpenROADStep):
     id = "OpenROAD.BasicMacroPlacement"
     name = "Basic Macro Placement"
```

### Comparing `openlane-2.0.0a8/openlane/steps/step.py` & `openlane-2.0.0a9/openlane/steps/step.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,40 +339,41 @@
                 pass
         else:
             self.toolbox = toolbox
 
         if isinstance(self.state_in, Future):
             self.state_in = self.state_in.result()
 
+        rule(f"{self.long_name}")
+
         if self.flow is not None and self.flow_control_variable is not None:
             flow_control_value = self.config[self.flow_control_variable]
             if isinstance(flow_control_value, bool):
                 if not flow_control_value:
                     if self.flow_control_msg is not None:
                         info(self.flow_control_msg)
                     else:
                         info(
-                            f"`{self.flow_control_variable}` is set to False: skipping…"
+                            f"'{self.flow_control_variable}' is set to False: skipping…"
                         )
                         return self.state_in.copy()
             elif flow_control_value is None:
                 if self.flow_control_msg is not None:
                     info(self.flow_control_msg)
                 else:
                     info(
-                        f"Required variable `{self.flow_control_variable}` is set to null: skipping…"
+                        f"Required variable '{self.flow_control_variable}' is set to null: skipping…"
                     )
                 return self.state_in.copy()
 
         mkdirp(self.step_dir)
         with open(os.path.join(self.step_dir, "state_in.json"), "w") as f:
             f.write(self.state_in.dumps())
 
         self.start_time = time.time()
-        rule(f"{self.long_name}")
         self.state_out = self.run(**kwargs)
         try:
             self.state_out.validate()
         except InvalidState as e:
             raise StepException(f"Step {self.name} generated invalid state: {e}")
         self.end_time = time.time()
```

### Comparing `openlane-2.0.0a8/openlane/steps/tclstep.py` & `openlane-2.0.0a9/openlane/steps/tclstep.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/steps/yosys.py` & `openlane-2.0.0a9/openlane/steps/yosys.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/utils/__init__.py` & `openlane-2.0.0a9/openlane/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/utils/drc.py` & `openlane-2.0.0a9/openlane/utils/drc.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/utils/memoize.py` & `openlane-2.0.0a9/openlane/utils/memoize.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane/utils/toolbox.py` & `openlane-2.0.0a9/openlane/utils/toolbox.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/openlane.egg-info/PKG-INFO` & `openlane-2.0.0a9/openlane.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlane
-Version: 2.0.0a8
+Version: 2.0.0a9
 Summary: An infrastructure for implementing chip design flows
 Home-page: UNKNOWN
 Author: Efabless Corporation and Contributors
 Author-email: donn@efabless.com
 License: UNKNOWN
 Description: > Efabless OpenLane 2 is in early access and all APIs are, presently, highly unstable and subject to change without notice.
         >
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openlane Version: 2.0.0a8 Summary: An
+Metadata-Version: 2.1 Name: openlane Version: 2.0.0a9 Summary: An
 infrastructure for implementing chip design flows Home-page: UNKNOWN Author:
 Efabless Corporation and Contributors Author-email: donn@efabless.com License:
 UNKNOWN Description: > Efabless OpenLane 2 is in early access and all APIs are,
 presently, highly unstable and subject to change without notice. > > If you
 don't know why you're here, you're probably looking for the stable version of
 OpenLane at https://github.com/The-OpenROAD-Project/OpenLane.
                             ****** OpenLane ******
```

### Comparing `openlane-2.0.0a8/openlane.egg-info/SOURCES.txt` & `openlane-2.0.0a9/openlane.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openlane-2.0.0a8/setup.py` & `openlane-2.0.0a9/setup.py`

 * *Files identical despite different names*

