# Comparing `tmp/ocp_vscode-0.93.0.tar.gz` & `tmp/ocp_vscode-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp_vscode-0.93.0.tar", last modified: Sat Apr 29 10:16:34 2023, max compression
+gzip compressed data, was "ocp_vscode-1.0.0.tar", last modified: Sun May  7 16:14:31 2023, max compression
```

## Comparing `ocp_vscode-0.93.0.tar` & `ocp_vscode-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-29 10:16:34.079846 ocp_vscode-0.93.0/
--rw-r--r--   0 bernhard   (501) staff       (20)    10938 2022-10-05 06:47:11.000000 ocp_vscode-0.93.0/LICENSE
--rw-r--r--   0 bernhard   (501) staff       (20)      809 2023-04-29 10:16:34.079907 ocp_vscode-0.93.0/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)     7866 2023-04-29 07:30:35.000000 ocp_vscode-0.93.0/README.md
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-29 10:16:34.079139 ocp_vscode-0.93.0/ocp_vscode/
--rw-r--r--   0 bernhard   (501) staff       (20)      948 2023-04-27 17:11:08.000000 ocp_vscode-0.93.0/ocp_vscode/__init__.py
--rw-r--r--   0 bernhard   (501) staff       (20)     4750 2023-04-21 15:55:51.000000 ocp_vscode-0.93.0/ocp_vscode/animation.py
--rw-r--r--   0 bernhard   (501) staff       (20)    16915 2023-04-29 09:55:32.000000 ocp_vscode-0.93.0/ocp_vscode/colors.py
--rw-r--r--   0 bernhard   (501) staff       (20)     9463 2023-04-27 18:50:45.000000 ocp_vscode-0.93.0/ocp_vscode/config.py
--rw-r--r--   0 bernhard   (501) staff       (20)    18993 2023-04-29 06:29:08.000000 ocp_vscode-0.93.0/ocp_vscode/show.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-29 10:16:34.079759 ocp_vscode-0.93.0/ocp_vscode.egg-info/
--rw-r--r--   0 bernhard   (501) staff       (20)      809 2023-04-29 10:16:34.000000 ocp_vscode-0.93.0/ocp_vscode.egg-info/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)      346 2023-04-29 10:16:34.000000 ocp_vscode-0.93.0/ocp_vscode.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-04-29 10:16:34.000000 ocp_vscode-0.93.0/ocp_vscode.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-04-29 10:16:34.000000 ocp_vscode-0.93.0/ocp_vscode.egg-info/not-zip-safe
--rw-r--r--   0 bernhard   (501) staff       (20)       38 2023-04-29 10:16:34.000000 ocp_vscode-0.93.0/ocp_vscode.egg-info/requires.txt
--rw-r--r--   0 bernhard   (501) staff       (20)       11 2023-04-29 10:16:34.000000 ocp_vscode-0.93.0/ocp_vscode.egg-info/top_level.txt
--rw-r--r--   0 bernhard   (501) staff       (20)      901 2023-04-29 10:16:34.080172 ocp_vscode-0.93.0/setup.cfg
--rw-r--r--   0 bernhard   (501) staff       (20)     1137 2023-04-29 07:30:35.000000 ocp_vscode-0.93.0/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-05-07 16:14:31.684552 ocp_vscode-1.0.0/
+-rw-r--r--   0 bernhard   (501) staff       (20)    10938 2022-10-05 06:47:11.000000 ocp_vscode-1.0.0/LICENSE
+-rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-05-07 16:14:31.684606 ocp_vscode-1.0.0/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)     2228 2023-05-07 15:55:57.000000 ocp_vscode-1.0.0/README.md
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-05-07 16:14:31.683832 ocp_vscode-1.0.0/ocp_vscode/
+-rw-r--r--   0 bernhard   (501) staff       (20)      948 2023-04-27 17:11:08.000000 ocp_vscode-1.0.0/ocp_vscode/__init__.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     4750 2023-04-21 15:55:51.000000 ocp_vscode-1.0.0/ocp_vscode/animation.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    16915 2023-04-29 09:55:32.000000 ocp_vscode-1.0.0/ocp_vscode/colors.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    10045 2023-05-07 13:07:57.000000 ocp_vscode-1.0.0/ocp_vscode/config.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    21269 2023-05-07 13:29:25.000000 ocp_vscode-1.0.0/ocp_vscode/show.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-05-07 16:14:31.684462 ocp_vscode-1.0.0/ocp_vscode.egg-info/
+-rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-05-07 16:14:31.000000 ocp_vscode-1.0.0/ocp_vscode.egg-info/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)      346 2023-05-07 16:14:31.000000 ocp_vscode-1.0.0/ocp_vscode.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-05-07 16:14:31.000000 ocp_vscode-1.0.0/ocp_vscode.egg-info/dependency_links.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-05-07 16:14:31.000000 ocp_vscode-1.0.0/ocp_vscode.egg-info/not-zip-safe
+-rw-r--r--   0 bernhard   (501) staff       (20)       38 2023-05-07 16:14:31.000000 ocp_vscode-1.0.0/ocp_vscode.egg-info/requires.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)       11 2023-05-07 16:14:31.000000 ocp_vscode-1.0.0/ocp_vscode.egg-info/top_level.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)      900 2023-05-07 16:14:31.684875 ocp_vscode-1.0.0/setup.cfg
+-rw-r--r--   0 bernhard   (501) staff       (20)     1136 2023-05-07 11:26:55.000000 ocp_vscode-1.0.0/setup.py
```

### Comparing `ocp_vscode-0.93.0/LICENSE` & `ocp_vscode-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ocp_vscode-0.93.0/PKG-INFO` & `ocp_vscode-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_vscode
-Version: 0.93.0
+Version: 1.0.0
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_vscode-0.93.0/ocp_vscode/__init__.py` & `ocp_vscode-1.0.0/ocp_vscode/__init__.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-0.93.0/ocp_vscode/animation.py` & `ocp_vscode-1.0.0/ocp_vscode/animation.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-0.93.0/ocp_vscode/colors.py` & `ocp_vscode-1.0.0/ocp_vscode/colors.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-0.93.0/ocp_vscode/config.py` & `ocp_vscode-1.0.0/ocp_vscode/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 CONFIG_UI_KEYS = [
     "axes",
     "axes0",
     "black_edges",
     "grid",
     "ortho",
     "transparent",
+    "explode",
 ]
 
 CONFIG_WORKSPACE_KEYS = CONFIG_UI_KEYS + [
     # viewer
     "collapse",
     "dark",
     "glass",
@@ -43,39 +44,44 @@
     "rotate_speed",
     "zoom_speed",
     # render settings
     "ambient_intensity",
     "angular_tolerance",
     "default_color",
     "default_edgecolor",
+    "default_facecolor",
+    "default_thickedgecolor",
+    "default_vertexcolor",
     "default_opacity",
     "deviation",
     "direct_intensity",
 ]
 
 CONFIG_CONTROL_KEYS = [
     "edge_accuracy",
     "debug",
     "mate_scale",
     "render_edges",
     "render_mates",
+    "render_joints",
     "render_normals",
     "reset_camera",
     "timeit",
 ]
 
 CONFIG_KEYS = CONFIG_WORKSPACE_KEYS + CONFIG_CONTROL_KEYS + ["zoom"]
 
 CONFIG_SET_KEYS = [
     "axes",
     "axes0",
     "grid",
     "ortho",
     "transparent",
     "black_edges",
+    "explode",
     "zoom",
     "position",
     "quaternion",
     "target",
     "default_edgecolor",
     "default_opacity",
     "ambient_intensity",
@@ -90,14 +96,15 @@
     "collapse",
 ]
 
 DEFAULTS = {
     "render_edges": True,
     "render_normals": False,
     "render_mates": False,
+    "render_joints": False,
     "mate_scale": 1.0,
     "timeit": False,
     "reset_camera": True,
     "debug": False,
 }
 
 CMD_URL = "http://127.0.0.1"
@@ -135,14 +142,15 @@
 def set_viewer_config(
     axes=None,
     axes0=None,
     grid=None,
     ortho=None,
     transparent=None,
     black_edges=None,
+    explode=None,
     zoom=None,
     position=None,
     quaternion=None,
     target=None,
     default_edgecolor=None,
     default_opacity=None,
     ambient_intensity=None,
@@ -183,14 +191,15 @@
     transparent=None,
     default_opacity=None,
     black_edges=None,
     orbit_control=None,
     collapse=None,
     ticks=None,
     up=None,
+    explode=None,
     zoom=None,
     reset_camera=None,
     pan_speed=None,
     rotate_speed=None,
     zoom_speed=None,
     deviation=None,
     angular_tolerance=None,
@@ -198,14 +207,15 @@
     default_color=None,
     default_edgecolor=None,
     ambient_intensity=None,
     direct_intensity=None,
     render_edges=None,
     render_normals=None,
     render_mates=None,
+    render_joints=None,
     mate_scale=None,
     debug=None,
     timeit=None,
 ):
     """Set viewer defaults
     Keywords to configure the viewer:
     - UI
@@ -221,14 +231,15 @@
         transparent:       Show objects transparent (default=False)
         default_opacity:   Opacity value for transparent objects (default=0.5)
         black_edges:       Show edges in black color (default=False)
         orbit_control:     Mouse control use "orbit" control instead of "trackball" control (default=False)
         collapse:          1: collapse all leaf nodes, C: collapse all nodes, E: expand all nodes (default=1)
         ticks:             Hint for the number of ticks in both directions (default=10)
         up:                Use z-axis ('Z') or y-axis ('Y') as up direction for the camera (default="Z")
+        explode:           Turn on explode mode (default=False)
 
         zoom:              Zoom factor of view (default=1.0)
         position:          Camera position
         quaternion:        Camera orientation as quaternion
         target:            Camera look at target
         reset_camera:      Reset camera position, rotation and zoom to default (default=True)
 
@@ -245,14 +256,15 @@
         default_edgecolor: Default mesh color (default=(128, 128, 128))
         ambient_intensity  Intensity of ambient ligth (default=1.0)
         direct_intensity   Intensity of direct lights (default=0.12)
 
         render_edges:      Render edges  (default=True)
         render_normals:    Render normals (default=False)
         render_mates:      Render mates for MAssemblies (default=False)
+        render_joints:      Render mates for MAssemblies (default=False)
         mate_scale:        Scale of rendered mates for MAssemblies (default=1)
 
     - Debug
         debug:             Show debug statements to the VS Code browser console (default=False)
         timeit:            Show timing information from level 0-3 (default=False)
     """
 
@@ -280,37 +292,43 @@
     if port is None:
         port = CMD_PORT
     try:
         conf = requests.get(f"{CMD_URL}:{port}/status").json()["text"]
         return conf
 
     except Exception as ex:
-        print("Error: Cannot access viewer status:", ex)
+        raise RuntimeError(
+            "Cannot access viewer status. Is the viewer running?\n" + str(ex.args)
+        )
 
 
 def workspace_config(port=None):
     if port is None:
         port = CMD_PORT
     try:
         return requests.get(f"{CMD_URL}:{port}/config").json()
 
     except Exception as ex:
-        print("Error: Cannot access viewer config:", ex)
+        raise RuntimeError(
+            "Cannot access viewer config. Is the viewer running?\n" + str(ex.args)
+        )
 
 
 def combined_config(port=None, use_status=True):
     if port is None:
         port = CMD_PORT
 
     try:
         wspace_config = workspace_config(port)
         wspace_status = status(port)
 
     except Exception as ex:
-        print("Error: Cannot access viewer config:", ex)
+        raise RuntimeError(
+            "Cannot access viewer config. Is the viewer running?\n" + str(ex.args)
+        )
 
     if use_status and wspace_config["_splash"]:
         del wspace_config["_splash"]
         wspace_config["axes"] = False
         wspace_config["axes0"] = True
         wspace_config["grid"] = [True, False, False]
         wspace_config["ortho"] = False
@@ -345,12 +363,13 @@
     if config.get("transparent") is not None:
         set_viewer_config(transparent=config["transparent"])
 
     DEFAULTS = {
         "render_edges": True,
         "render_normals": False,
         "render_mates": False,
+        "render_joints": False,
         "mate_scale": 1.0,
         "timeit": False,
         "reset_camera": True,
         "debug": False,
     }
```

### Comparing `ocp_vscode-0.93.0/ocp_vscode/show.py` & `ocp_vscode-1.0.0/ocp_vscode/show.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     combined_bb,
     to_assembly,
     mp_get_results,
 )
 from ocp_tessellate.utils import numpy_to_buffer_json, Timer, Color
 from ocp_tessellate.mp_tessellator import init_pool, keymap, close_pool
 from ocp_tessellate.cad_objects import OCP_PartGroup
+import ocp_tessellate.convert as oc
 
 from .config import (
     preset,
     get_changed_config,
     workspace_config,
     combined_config,
     get_default,
@@ -38,14 +39,37 @@
 
 OBJECTS = {"objs": [], "names": [], "colors": [], "alphas": []}
 
 
 def _tessellate(
     *cad_objs, names=None, colors=None, alphas=None, progress=None, **kwargs
 ):
+    if workspace_config().get("_splash"):
+        conf = combined_config(use_status=False)
+    else:
+        conf = combined_config(use_status=True)
+
+    if kwargs.get("default_facecolor") is not None:
+        oc.FACE_COLOR = Color(kwargs["default_facecolor"]).percentage
+        del kwargs["default_facecolor"]
+    else:
+        oc.FACE_COLOR = Color(conf["default_facecolor"]).percentage
+
+    if kwargs.get("default_thickedgecolor") is not None:
+        oc.THICK_EDGE_COLOR = Color(kwargs["default_thickedgecolor"]).percentage
+        del kwargs["default_thickedgecolor"]
+    else:
+        oc.THICK_EDGE_COLOR = Color(conf["default_thickedgecolor"]).percentage
+
+    if kwargs.get("default_vertexcolor") is not None:
+        oc.VERTEX_COLOR = Color(kwargs["default_vertexcolor"]).percentage
+        del kwargs["default_vertexcolor"]
+    else:
+        oc.VERTEX_COLOR = Color(conf["default_vertexcolor"]).percentage
+
     timeit = preset("timeit", kwargs.get("timeit"))
 
     if timeit is None:
         timeit = False
 
     if progress is None:
         progress = Progress([c for c in "-+c"])
@@ -69,20 +93,14 @@
         )
 
         if len(part_group.objects) == 1 and isinstance(
             part_group.objects[0], PartGroup
         ):
             part_group = part_group.objects[0]
 
-    # Do not send defaults for postion, rotation and zoom unless they are set in kwargs
-    if workspace_config().get("_splash"):
-        conf = combined_config(use_status=False)
-    else:
-        conf = combined_config(use_status=True)
-
     params = {
         k: v
         for k, v in conf.items()
         if not k
         in (
             "position",
             "rotation",
@@ -170,14 +188,17 @@
     elif config.get("collapse") is not None:
         mapping = {"1": 1, "E": 0, "C": 2}
         config["collapse"] = mapping.get(config["collapse"], 1)
 
     if config.get("debug") is not None and config["debug"]:
         print("\nconfig:\n", config)
 
+    if kwargs.get("explode") is not None:
+        config["explode"] = kwargs["explode"]
+
     with Timer(timeit, "", "create data obj", 1):
         data = {
             "data": numpy_to_buffer_json(
                 dict(instances=instances, shapes=shapes, states=states)
             ),
             "type": "data",
             "config": config,
@@ -227,14 +248,15 @@
     grid=None,
     ortho=None,
     transparent=None,
     default_opacity=None,
     black_edges=None,
     orbit_control=None,
     collapse=None,
+    explode=None,
     ticks=None,
     up=None,
     zoom=None,
     position=None,
     quaternion=None,
     target=None,
     reset_camera=None,
@@ -242,88 +264,95 @@
     rotate_speed=None,
     zoom_speed=None,
     deviation=None,
     angular_tolerance=None,
     edge_accuracy=None,
     default_color=None,
     default_edgecolor=None,
+    default_facecolor=None,
+    default_thickedgecolor=None,
+    default_vertexcolor=None,
     ambient_intensity=None,
     direct_intensity=None,
     render_edges=None,
     render_normals=None,
     render_mates=None,
     render_joints=None,
     show_parent=None,
     parallel=None,
     mate_scale=None,
     debug=None,
     timeit=None,
 ):
     """Show CAD objects in Visual Studio Code
     Parameters
-        cad_objs:          All cad objects that should be shown as positional parameters
+        cad_objs:                All cad objects that should be shown as positional parameters
 
     Keywords for show:
-        names:             List of names for the cad_objs. Needs to have the same length as cad_objs
-        colors:            List of colors for the cad_objs. Needs to have the same length as cad_objs
-        alphas:            List of alpha values for the cad_objs. Needs to have the same length as cad_objs
-        port:              The port the viewer listens to. Typically use 'set_port(port)' instead
-        progress:          Show progress of tessellation with None is no progress indicator. (default="-+c")
-                           for object: "-": is reference, "+": gets tessellated, "c": from cache
+        names:                   List of names for the cad_objs. Needs to have the same length as cad_objs
+        colors:                  List of colors for the cad_objs. Needs to have the same length as cad_objs
+        alphas:                  List of alpha values for the cad_objs. Needs to have the same length as cad_objs
+        port:                    The port the viewer listens to. Typically use 'set_port(port)' instead
+        progress:                Show progress of tessellation with None is no progress indicator. (default="-+c")
+                                 for object: "-": is reference, "+": gets tessellated, "c": from cache
 
     Valid keywords to configure the viewer (**kwargs):
     - UI
-        glass:             Use glass mode where tree is an overlay over the cad object (default=False)
-        tools:             Show tools (default=True)
-        tree_width:        Width of the object tree (default=240)
+        glass:                   Use glass mode where tree is an overlay over the cad object (default=False)
+        tools:                   Show tools (default=True)
+        tree_width:              Width of the object tree (default=240)
 
     - Viewer
-        axes:              Show axes (default=False)
-        axes0:             Show axes at (0,0,0) (default=False)
-        grid:              Show grid (default=False)
-        ortho:             Use orthographic projections (default=True)
-        transparent:       Show objects transparent (default=False)
-        default_opacity:   Opacity value for transparent objects (default=0.5)
-        black_edges:       Show edges in black color (default=False)
-        orbit_control:     Mouse control use "orbit" control instead of "trackball" control (default=False)
-        collapse:          1: collapse all leaf nodes, C: collapse all nodes, E: expand all nodes (default=1)
-        ticks:             Hint for the number of ticks in both directions (default=10)
-        up:                Use z-axis ('Z') or y-axis ('Y') as up direction for the camera (default="Z")
-
-        zoom:              Zoom factor of view (default=1.0)
-        position:          Camera position
-        quaternion:        Camera orientation as quaternion
-        target:            Camera look at target
-        reset_camera:      Reset camera position, rotation and zoom to default (default=True)
-
-        pan_speed:         Speed of mouse panning (default=1)
-        rotate_speed:      Speed of mouse rotate (default=1)
-        zoom_speed:        Speed of mouse zoom (default=1)
+        axes:                    Show axes (default=False)
+        axes0:                   Show axes at (0,0,0) (default=False)
+        grid:                    Show grid (default=False)
+        ortho:                   Use orthographic projections (default=True)
+        transparent:             Show objects transparent (default=False)
+        default_opacity:         Opacity value for transparent objects (default=0.5)
+        black_edges:             Show edges in black color (default=False)
+        orbit_control:           Mouse control use "orbit" control instead of "trackball" control (default=False)
+        collapse:                1: collapse all leaf nodes, C: collapse all nodes, E: expand all nodes (default=1)
+        ticks:                   Hint for the number of ticks in both directions (default=10)
+        up:                      Use z-axis ('Z') or y-axis ('Y') as up direction for the camera (default="Z")
+        explode:                 Turn on explode mode (default=False)
+
+        zoom:                    Zoom factor of view (default=1.0)
+        position:                Camera position
+        quaternion:              Camera orientation as quaternion
+        target:                  Camera look at target
+        reset_camera:            Reset camera position, rotation and zoom to default (default=True)
+
+        pan_speed:               Speed of mouse panning (default=1)
+        rotate_speed:            Speed of mouse rotate (default=1)
+        zoom_speed:              Speed of mouse zoom (default=1)
 
     - Renderer
-        deviation:         Shapes: Deviation from linear deflection value (default=0.1)
-        angular_tolerance: Shapes: Angular deflection in radians for tessellation (default=0.2)
-        edge_accuracy:     Edges: Precision of edge discretization (default: mesh quality / 100)
-
-        default_color:     Default mesh color (default=(232, 176, 36))
-        default_edgecolor: Default color of the edges of a mesh (default=(128, 128, 128))
-        ambient_intensity  Intensity of ambient ligth (default=1.0)
-        direct_intensity   Intensity of direct lights (default=0.12)
-
-        render_edges:      Render edges  (default=True)
-        render_normals:    Render normals (default=False)
-        render_mates:      Render mates for MAssemblies (default=False)
-        render_joints:     Render build123d joints (default=False)
-        parallel:          Tessellate objects in parallel (default=False)
-        show_parent:       Render parent of faces, edges or vertices as wireframe
-        mate_scale:        Scale of rendered mates for MAssemblies (default=1)
+        deviation:               Shapes: Deviation from linear deflection value (default=0.1)
+        angular_tolerance:       Shapes: Angular deflection in radians for tessellation (default=0.2)
+        edge_accuracy:           Edges: Precision of edge discretization (default: mesh quality / 100)
+
+        default_color:           Default mesh color (default=(232, 176, 36))
+        default_edgecolor:       Default color of the edges of a mesh (default=#707070)
+        default_facecolor:       Default color of the edges of a mesh (default=#ee82ee)
+        default_thickedgecolor:  Default color of the edges of a mesh (default=#ba55d3)
+        default_vertexcolor:     Default color of the edges of a mesh (default=#ba55d3)
+        ambient_intensity        Intensity of ambient ligth (default=1.0)
+        direct_intensity         Intensity of direct lights (default=0.12)
+
+        render_edges:            Render edges  (default=True)
+        render_normals:          Render normals (default=False)
+        render_mates:            Render mates for MAssemblies (default=False)
+        render_joints:           Render build123d joints (default=False)
+        parallel:                Tessellate objects in parallel (default=False)
+        show_parent:             Render parent of faces, edges or vertices as wireframe
+        mate_scale:              Scale of rendered mates for MAssemblies (default=1)
 
     - Debug
-        debug:             Show debug statements to the VS Code browser console (default=False)
-        timeit:            Show timing information from level 0-3 (default=False)
+        debug:                   Show debug statements to the VS Code browser console (default=False)
+        timeit:                  Show timing information from level 0-3 (default=False)
     """
 
     timeit = preset("timeit", timeit)
 
     names = align_attrs(names, len(cad_objs), None, "names", explode=False)
 
     # Handle colormaps
@@ -367,14 +396,17 @@
             "colors",
             "alphas",
             "port",
             "progress",
         ]
     }
 
+    if explode is not None:
+        kwargs["explode"] = explode
+
     progress = Progress([] if progress is None else [c for c in progress])
 
     with Timer(timeit, "", "overall"):
         data = _convert(
             *cad_objs,
             names=names,
             colors=colors,
@@ -423,14 +455,17 @@
     pan_speed=None,
     rotate_speed=None,
     zoom_speed=None,
     deviation=None,
     angular_tolerance=None,
     edge_accuracy=None,
     default_color=None,
+    default_facecolor=None,
+    default_thickedgecolor=None,
+    default_vertexcolor=None,
     default_edgecolor=None,
     ambient_intensity=None,
     direct_intensity=None,
     render_edges=None,
     render_normals=None,
     render_mates=None,
     render_joints=None,
@@ -439,77 +474,80 @@
     mate_scale=None,
     debug=None,
     timeit=None,
 ):
     """Incrementally show CAD objects in Visual Studio Code
 
     Parameters:
-        obj:              The CAD object to be shown
+        obj:                     The CAD object to be shown
 
     Keywords for show_object:
-        name:              The name of the CAD object
-        options:           A dict of color and alpha value: {"alpha":0.5, "color": (64, 164, 223)}
-                           0 <= alpha <= 1.0 and color is a 3-tuple of values between 0 and 255
-        parent:            Add another object, usually the parent of e.g. edges or vertices with alpha=0.25
-        clear:             In interactice mode, clear the stack of objects to be shown
-                           (typically used for the first object)
-        port:              The port the viewer listens to. Typically use 'set_port(port)' instead
-        progress:          Show progress of tessellation with None is no progress indicator. (default="-+c")
-                           for object: "-": is reference, "+": gets tessellated, "c": from cache
+        name:                    The name of the CAD object
+        options:                 A dict of color and alpha value: {"alpha":0.5, "color": (64, 164, 223)}
+                                 0 <= alpha <= 1.0 and color is a 3-tuple of values between 0 and 255
+        parent:                  Add another object, usually the parent of e.g. edges or vertices with alpha=0.25
+        clear:                   In interactice mode, clear the stack of objects to be shown
+                                 (typically used for the first object)
+        port:                    The port the viewer listens to. Typically use 'set_port(port)' instead
+        progress:                Show progress of tessellation with None is no progress indicator. (default="-+c")
+                                 for object: "-": is reference, "+": gets tessellated, "c": from cache
 
     Valid keywords to configure the viewer (**kwargs):
     - UI
-        glass:             Use glass mode where tree is an overlay over the cad object (default=False)
-        tools:             Show tools (default=True)
-        tree_width:        Width of the object tree (default=240)
+        glass:                   Use glass mode where tree is an overlay over the cad object (default=False)
+        tools:                   Show tools (default=True)
+        tree_width:              Width of the object tree (default=240)
 
     - Viewer
-        axes:              Show axes (default=False)
-        axes0:             Show axes at (0,0,0) (default=False)
-        grid:              Show grid (default=False)
-        ortho:             Use orthographic projections (default=True)
-        transparent:       Show objects transparent (default=False)
-        default_opacity:   Opacity value for transparent objects (default=0.5)
-        black_edges:       Show edges in black color (default=False)
-        orbit_control:     Mouse control use "orbit" control instead of "trackball" control (default=False)
-        collapse:          1: collapse all leaf nodes, C: collapse all nodes, E: expand all nodes (default=1)
-        ticks:             Hint for the number of ticks in both directions (default=10)
-        up:                Use z-axis ('Z') or y-axis ('Y') as up direction for the camera (default="Z")
-
-        zoom:              Zoom factor of view (default=1.0)
-        position:          Camera position
-        quaternion:        Camera orientation as quaternion
-        target:            Camera look at target
-        reset_camera:      Reset camera position, rotation and zoom to default (default=True)
-
-        pan_speed:         Speed of mouse panning (default=1)
-        rotate_speed:      Speed of mouse rotate (default=1)
-        zoom_speed:        Speed of mouse zoom (default=1)
+        axes:                    Show axes (default=False)
+        axes0:                   Show axes at (0,0,0) (default=False)
+        grid:                    Show grid (default=False)
+        ortho:                   Use orthographic projections (default=True)
+        transparent:             Show objects transparent (default=False)
+        default_opacity:         Opacity value for transparent objects (default=0.5)
+        black_edges:             Show edges in black color (default=False)
+        orbit_control:           Mouse control use "orbit" control instead of "trackball" control (default=False)
+        collapse:                1: collapse all leaf nodes, C: collapse all nodes, E: expand all nodes (default=1)
+        ticks:                   Hint for the number of ticks in both directions (default=10)
+        up:                      Use z-axis ('Z') or y-axis ('Y') as up direction for the camera (default="Z")
+
+        zoom:                    Zoom factor of view (default=1.0)
+        position:                Camera position
+        quaternion:              Camera orientation as quaternion
+        target:                  Camera look at target
+        reset_camera:            Reset camera position, rotation and zoom to default (default=True)
+
+        pan_speed:               Speed of mouse panning (default=1)
+        rotate_speed:            Speed of mouse rotate (default=1)
+        zoom_speed:              Speed of mouse zoom (default=1)
 
     - Renderer
-        deviation:         Shapes: Deviation from linear deflection value (default=0.1)
-        angular_tolerance: Shapes: Angular deflection in radians for tessellation (default=0.2)
-        edge_accuracy:     Edges: Precision of edge discretization (default: mesh quality / 100)
-
-        default_color:     Default mesh color (default=(232, 176, 36))
-        default_edgecolor: Default color of the edges of a mesh (default=(128, 128, 128))
-        ambient_intensity  Intensity of ambient ligth (default=1.0)
-        direct_intensity   Intensity of direct lights (default=0.12)
-
-        render_edges:      Render edges  (default=True)
-        render_normals:    Render normals (default=False)
-        render_mates:      Render mates for MAssemblies (default=False)
-        render_joints:     Render build123d joints (default=False)
-        parallel:          Tessellate objects in parallel (default=False)
-        show_parent:       Render parent of faces, edges or vertices as wireframe
-        mate_scale:        Scale of rendered mates for MAssemblies (default=1)
+        deviation:               Shapes: Deviation from linear deflection value (default=0.1)
+        angular_tolerance:       Shapes: Angular deflection in radians for tessellation (default=0.2)
+        edge_accuracy:           Edges: Precision of edge discretization (default: mesh quality / 100)
+
+        default_color:           Default mesh color (default=(232, 176, 36))
+        default_edgecolor:       Default color of the edges of a mesh (default=(128, 128, 128))
+        default_facecolor:       Default color of the edges of a mesh (default=#ee82ee / Violet)
+        default_thickedgecolor:  Default color of the edges of a mesh (default=#ba55d3 / MediumOrchid)
+        default_vertexcolor:     Default color of the edges of a mesh (default=#ba55d3 / MediumOrchid)
+                                 ambient_intensity  Intensity of ambient ligth (default=1.0)
+        direct_intensity         Intensity of direct lights (default=0.12)
+
+        render_edges:            Render edges  (default=True)
+        render_normals:          Render normals (default=False)
+        render_mates:            Render mates for MAssemblies (default=False)
+        render_joints:           Render build123d joints (default=False)
+        parallel:                Tessellate objects in parallel (default=False)
+        show_parent:             Render parent of faces, edges or vertices as wireframe
+        mate_scale:              Scale of rendered mates for MAssemblies (default=1)
 
     - Debug
-        debug:             Show debug statements to the VS Code browser console (default=False)
-        imeit:             Show timing information from level 0-3 (default=False)
+        debug:                   Show debug statements to the VS Code browser console (default=False)
+        imeit:                   Show timing information from level 0-3 (default=False)
     """
 
     kwargs = {
         k: v
         for k, v in locals().items()
         if v is not None
         and k not in ["obj", "name", "options", "parent", "clear", "port", "progress"]
```

### Comparing `ocp_vscode-0.93.0/ocp_vscode.egg-info/PKG-INFO` & `ocp_vscode-1.0.0/ocp_vscode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp-vscode
-Version: 0.93.0
+Version: 1.0.0
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_vscode-0.93.0/setup.cfg` & `ocp_vscode-1.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.93.0
+current_version = 1.0.0
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>\D*)(?P<build>\d*)
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ocp_vscode-0.93.0/setup.py` & `ocp_vscode-1.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup_args = {
     "name": "ocp_vscode",
-    "version": "0.93.0",
+    "version": "1.0.0",
     "description": "OCP CAD Viewer for VSCode",
     "long_description": "An extension to show OCP cad CAD objects (CadQuery, build123d) in VS Code via pythreejs",
     "include_package_data": True,
     "python_requires": ">=3.9",
     "install_requires": ["ocp-tessellate>=1.0.2", "requests", "orjson"],
     "packages": find_packages(),
     "zip_safe": False,
```

