# Comparing `tmp/ursina-5.2.0.tar.gz` & `tmp/ursina-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ursina-5.2.0.tar", last modified: Mon Jan 30 22:38:33 2023, max compression
+gzip compressed data, was "ursina-5.3.0.tar", last modified: Sun May  7 14:08:20 2023, max compression
```

## Comparing `ursina-5.2.0.tar` & `ursina-5.3.0.tar`

### file list

```diff
@@ -1,215 +1,216 @@
-drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-01-30 22:38:33.721384 ursina-5.2.0/
--rw-rw-r--   0 poke      (1000) poke      (1000)     1091 2023-01-30 22:37:44.000000 ursina-5.2.0/LICENSE
--rw-rw-r--   0 poke      (1000) poke      (1000)      302 2023-01-30 22:37:44.000000 ursina-5.2.0/MANIFEST.in
--rw-rw-r--   0 poke      (1000) poke      (1000)     4606 2023-01-30 22:38:33.721384 ursina-5.2.0/PKG-INFO
--rw-rw-r--   0 poke      (1000) poke      (1000)     4370 2023-01-30 22:37:44.000000 ursina-5.2.0/README.md
--rw-rw-r--   0 poke      (1000) poke      (1000)       38 2023-01-30 22:38:33.721384 ursina-5.2.0/setup.cfg
--rw-rw-r--   0 poke      (1000) poke      (1000)      895 2023-01-30 22:37:44.000000 ursina-5.2.0/setup.py
-drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-01-30 22:38:33.717384 ursina-5.2.0/ursina/
--rw-rw-r--   0 poke      (1000) poke      (1000)     3162 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/__init__.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     2614 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/application.py
-drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-01-30 22:38:33.717384 ursina-5.2.0/ursina/audio/
--rw-rw-r--   0 poke      (1000) poke      (1000)   176444 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/audio/noise.wav
--rw-rw-r--   0 poke      (1000) poke      (1000)      288 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/audio/sine.wav
--rw-rw-r--   0 poke      (1000) poke      (1000)      484 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/audio/square.wav
--rw-rw-r--   0 poke      (1000) poke      (1000)      488 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/audio/triangle.wav
--rw-rw-r--   0 poke      (1000) poke      (1000)     6375 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/audio.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     4360 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/boxcast.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     9793 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/build.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     7848 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/camera.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     7858 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/collider.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     5120 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/color.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     8680 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/curve.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     2450 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/duplicate.py
-drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-01-30 22:38:33.717384 ursina-5.2.0/ursina/editor/
--rw-rw-r--   0 poke      (1000) poke      (1000)        0 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/editor/__init__.py
--rw-rw-r--   0 poke      (1000) poke      (1000)    91382 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/editor/level_editor.py
-drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-01-30 22:38:33.717384 ursina-5.2.0/ursina/editor/scenes/
--rw-rw-r--   0 poke      (1000) poke      (1000)        0 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/editor/scenes/__init__.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     5198 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/editor/scenes/test2[1,0].py
--rw-rw-r--   0 poke      (1000) poke      (1000)     6802 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/editor/scenes/untitled_scene[0,0].py
--rw-rw-r--   0 poke      (1000) poke      (1000)      278 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/editor/scenes/untitled_scene[1,1].py
--rw-rw-r--   0 poke      (1000) poke      (1000)      444 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/editor/scenes/untitled_scene[1,2].py
--rw-rw-r--   0 poke      (1000) poke      (1000)     3277 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/editor/scenes/untitled_scene[2,0].py
--rw-rw-r--   0 poke      (1000) poke      (1000)      784 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/editor/scenes/untitled_scene[2,3].py
--rw-rw-r--   0 poke      (1000) poke      (1000)    45754 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/entity.py
-drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-01-30 22:38:33.717384 ursina-5.2.0/ursina/fonts/
--rw-rw-r--   0 poke      (1000) poke      (1000)     6075 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/fonts/Bitstream Vera License.txt
--rw-rw-r--   0 poke      (1000) poke      (1000)    11560 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/fonts/LICENSE.txt
--rw-rw-r--   0 poke      (1000) poke      (1000)    96428 2023-01-30 22:37:44.000000 ursina-5.2.0/ursina/fonts/OpenSans-Regular.ttf
--rw-rw-r--   0 poke      (1000) poke      (1000)    49224 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/fonts/VeraMono.ttf
--rw-rw-r--   0 poke      (1000) poke      (1000)     2973 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/gamepad.py
--rw-rw-r--   0 poke      (1000) poke      (1000)      590 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/hit_info.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     4841 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/input_handler.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     3082 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/lights.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     9495 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/main.py
--rw-rw-r--   0 poke      (1000) poke      (1000)    10921 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/mesh.py
--rw-rw-r--   0 poke      (1000) poke      (1000)    20740 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/mesh_importer.py
-drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-01-30 22:38:33.717384 ursina-5.2.0/ursina/models/
--rw-rw-r--   0 poke      (1000) poke      (1000)        0 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models/__init__.py
-drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-01-30 22:38:33.717384 ursina-5.2.0/ursina/models/procedural/
--rw-rw-r--   0 poke      (1000) poke      (1000)        0 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models/procedural/__init__.py
--rw-rw-r--   0 poke      (1000) poke      (1000)      797 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models/procedural/capsule.py
--rw-rw-r--   0 poke      (1000) poke      (1000)      953 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models/procedural/circle.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     1413 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models/procedural/cone.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     1642 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models/procedural/cube.py
--rw-rw-r--   0 poke      (1000) poke      (1000)      736 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models/procedural/cylinder.py
--rw-rw-r--   0 poke      (1000) poke      (1000)      789 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models/procedural/grid.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     4761 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models/procedural/pipe.py
--rw-rw-r--   0 poke      (1000) poke      (1000)      914 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models/procedural/plane.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     3993 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models/procedural/quad.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     3947 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models/procedural/terrain.py
-drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-01-30 22:38:33.717384 ursina-5.2.0/ursina/models_compressed/
--rw-rw-r--   0 poke      (1000) poke      (1000)     4916 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models_compressed/arrow.ursinamesh
--rw-rw-r--   0 poke      (1000) poke      (1000)     5801 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models_compressed/circle.ursinamesh
--rw-rw-r--   0 poke      (1000) poke      (1000)     1837 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models_compressed/cube.ursinamesh
--rw-rw-r--   0 poke      (1000) poke      (1000)     1892 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models_compressed/cube_uv_top.ursinamesh
--rw-rw-r--   0 poke      (1000) poke      (1000)      153 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models_compressed/diamond.ursinamesh
--rw-rw-r--   0 poke      (1000) poke      (1000)     3381 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models_compressed/icosphere.ursinamesh
--rw-rw-r--   0 poke      (1000) poke      (1000)       56 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models_compressed/line.ursinamesh
--rw-rw-r--   0 poke      (1000) poke      (1000)      389 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models_compressed/plane.ursinamesh
--rw-rw-r--   0 poke      (1000) poke      (1000)      386 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models_compressed/quad.ursinamesh
--rw-rw-r--   0 poke      (1000) poke      (1000)     7100 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models_compressed/scale_gizmo.ursinamesh
--rw-rw-r--   0 poke      (1000) poke      (1000)   205071 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models_compressed/sky_dome.ursinamesh
--rw-rw-r--   0 poke      (1000) poke      (1000)   218850 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models_compressed/sphere.ursinamesh
--rw-rw-r--   0 poke      (1000) poke      (1000)      206 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models_compressed/wireframe_cube.ursinamesh
--rw-rw-r--   0 poke      (1000) poke      (1000)      124 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/models_compressed/wireframe_quad.ursinamesh
--rw-rw-r--   0 poke      (1000) poke      (1000)    12097 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/mouse.py
-drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-01-30 22:38:33.717384 ursina-5.2.0/ursina/prefabs/
--rw-rw-r--   0 poke      (1000) poke      (1000)        0 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/__init__.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     3312 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/animation.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     1782 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/animator.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     7238 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/button.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     3537 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/button_group.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     3403 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/button_list.py
--rw-rw-r--   0 poke      (1000) poke      (1000)    10028 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/conversation.py
--rw-rw-r--   0 poke      (1000) poke      (1000)      932 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/cursor.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     4707 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/draggable.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     2568 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/dropdown_menu.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     8073 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/editor_camera.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     7831 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/file_browser.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     2342 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/file_browser_save.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     6646 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/first_person_controller.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     2628 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/frame_animation_3d.py
--rw-rw-r--   0 poke      (1000) poke      (1000)    11167 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/grid_editor.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     3743 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/health_bar.py
--rw-rw-r--   0 poke      (1000) poke      (1000)    13231 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/hot_reloader.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     5025 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/input_field.py
--rw-rw-r--   0 poke      (1000) poke      (1000)      547 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/made_with_ursina.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     1182 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/memory_counter.py
--rw-rw-r--   0 poke      (1000) poke      (1000)      464 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/panel.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     7669 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/platformer_controller_2d.py
--rw-rw-r--   0 poke      (1000) poke      (1000)      913 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/primitives.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     2883 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/radial_menu.py
--rw-rw-r--   0 poke      (1000) poke      (1000)      561 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/sky.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     5423 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/slider.py
--rw-rw-r--   0 poke      (1000) poke      (1000)      784 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/sprite.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     2110 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/sprite_sheet_animation.py
--rw-rw-r--   0 poke      (1000) poke      (1000)    29975 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/text_field.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     9249 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/tilemap.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     1361 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/tooltip.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     2617 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/trail_renderer.py
--rw-rw-r--   0 poke      (1000) poke      (1000)    12449 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/ursfx.py
--rw-rw-r--   0 poke      (1000) poke      (1000)      604 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/ursina_splash.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     6729 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/video_recorder.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     4138 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/prefabs/window_panel.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     6201 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/raycast.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     1798 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/scene.py
-drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-01-30 22:38:33.717384 ursina-5.2.0/ursina/scripts/
--rw-rw-r--   0 poke      (1000) poke      (1000)        0 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/scripts/__init__.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     1445 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/scripts/_bat_to_exe.bat
--rw-rw-r--   0 poke      (1000) poke      (1000)      735 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/scripts/_blend_export.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     7184 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/scripts/_blender_scene_to_ursina.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     2268 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/scripts/chunk_mesh.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     2146 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/scripts/colorize.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     3288 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/scripts/combine.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     3820 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/scripts/generate_normals.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     2444 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/scripts/grid_layout.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     1417 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/scripts/merge_vertices.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     3107 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/scripts/noclip_mode.py
--rw-rw-r--   0 poke      (1000) poke      (1000)      620 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/scripts/position_limiter.py
--rw-rw-r--   0 poke      (1000) poke      (1000)      628 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/scripts/project_uvs.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     1594 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/scripts/scrollable.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     1320 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/scripts/smooth_follow.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     2917 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/scripts/terraincast.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     3341 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/sequence.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     2943 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shader.py
-drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-01-30 22:38:33.717384 ursina-5.2.0/ursina/shaders/
--rw-rw-r--   0 poke      (1000) poke      (1000)      950 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shaders/__init__.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     1969 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shaders/basic_lighting_shader.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     3107 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shaders/colored_lights_shader.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     3206 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shaders/fresnel_shader.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     1869 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shaders/geom_shader.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     2447 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shaders/instancing_shader.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     5352 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shaders/lit_with_shadows_shader.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     1773 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shaders/matcap_shader.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     1220 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shaders/noise_fog_shader.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     1372 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shaders/normals_shader.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     3260 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shaders/projector_shader.py
-drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-01-30 22:38:33.721384 ursina-5.2.0/ursina/shaders/screenspace_shaders/
--rw-rw-r--   0 poke      (1000) poke      (1000)     1428 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shaders/screenspace_shaders/camera_contrast.py
--rw-rw-r--   0 poke      (1000) poke      (1000)      973 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shaders/screenspace_shaders/camera_empty.py
--rw-rw-r--   0 poke      (1000) poke      (1000)      820 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shaders/screenspace_shaders/camera_grayscale.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     2257 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shaders/screenspace_shaders/camera_outline_shader.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     1222 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shaders/screenspace_shaders/camera_vertical_blur.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     4002 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shaders/screenspace_shaders/fxaa.py
--rw-rw-r--   0 poke      (1000) poke      (1000)      647 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shaders/screenspace_shaders/pixelation_shader.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     4138 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shaders/screenspace_shaders/ssao.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     3065 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shaders/texture_blend_shader.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     1835 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shaders/transition_shader.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     4355 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shaders/triplanar_shader.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     1690 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/shaders/unlit_shader.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     1745 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/string_utilities.py
--rw-rw-r--   0 poke      (1000) poke      (1000)    15356 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/text.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     7912 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/texture.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     3988 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/texture_importer.py
-drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-01-30 22:38:33.721384 ursina-5.2.0/ursina/textures/
--rw-rw-r--   0 poke      (1000) poke      (1000)     3018 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/arrow_down.png
--rw-rw-r--   0 poke      (1000) poke      (1000)     3025 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/arrow_right.png
--rw-rw-r--   0 poke      (1000) poke      (1000)     2896 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/brick.png
--rw-rw-r--   0 poke      (1000) poke      (1000)     3683 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/circle.png
--rw-rw-r--   0 poke      (1000) poke      (1000)     4194 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/circle_outlined.png
--rw-rw-r--   0 poke      (1000) poke      (1000)     3351 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/cog.png
--rw-rw-r--   0 poke      (1000) poke      (1000)    14902 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/cursor.png
--rw-rw-r--   0 poke      (1000) poke      (1000)     2895 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/file_icon.png
--rw-rw-r--   0 poke      (1000) poke      (1000)     2891 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/folder.png
--rw-rw-r--   0 poke      (1000) poke      (1000)    23748 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/grass.png
--rw-rw-r--   0 poke      (1000) poke      (1000)   848864 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/grass_tintable.png
--rw-rw-r--   0 poke      (1000) poke      (1000)    21070 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/heightmap_1.png
--rw-rw-r--   0 poke      (1000) poke      (1000)     2829 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/horizontal_gradient.png
-drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-01-30 22:38:33.721384 ursina-5.2.0/ursina/textures/items/
--rw-rw-r--   0 poke      (1000) poke      (1000)    44186 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/items/bag.png
--rw-rw-r--   0 poke      (1000) poke      (1000)    26101 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/items/bow_arrow.png
--rw-rw-r--   0 poke      (1000) poke      (1000)    45394 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/items/gem.png
--rw-rw-r--   0 poke      (1000) poke      (1000)   324040 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/items/items.psd
--rw-rw-r--   0 poke      (1000) poke      (1000)    16168 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/items/orb.png
--rw-rw-r--   0 poke      (1000) poke      (1000)    40572 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/items/sword.png
--rw-rw-r--   0 poke      (1000) poke      (1000)     7196 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/noise.png
--rw-rw-r--   0 poke      (1000) poke      (1000)   173070 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/perlin_noise.png
--rw-rw-r--   0 poke      (1000) poke      (1000)     6775 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/radial_gradient.png
--rw-rw-r--   0 poke      (1000) poke      (1000)     2875 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/rainbow.png
--rw-rw-r--   0 poke      (1000) poke      (1000)     6476 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/reflection_map_3.jpg
--rw-rw-r--   0 poke      (1000) poke      (1000)   222963 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/shore.jpg
--rw-rw-r--   0 poke      (1000) poke      (1000)   121903 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/sky_default.jpg
--rw-rw-r--   0 poke      (1000) poke      (1000)   125956 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/sky_sunset.jpg
--rw-rw-r--   0 poke      (1000) poke      (1000)     5326 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/test_tileset.png
--rw-rw-r--   0 poke      (1000) poke      (1000)      690 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/tilemap_test_level.png
--rw-rw-r--   0 poke      (1000) poke      (1000)    17689 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/ursina_logo.png
--rw-rw-r--   0 poke      (1000) poke      (1000)      760 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/ursina_wink_0000.png
--rw-rw-r--   0 poke      (1000) poke      (1000)      827 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/ursina_wink_0001.png
--rw-rw-r--   0 poke      (1000) poke      (1000)     2825 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/vertical_gradient.png
--rw-rw-r--   0 poke      (1000) poke      (1000)    32461 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/vignette.jpg
--rw-rw-r--   0 poke      (1000) poke      (1000)     2909 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/textures/white_cube.png
--rw-rw-r--   0 poke      (1000) poke      (1000)     1871 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/trigger.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     5045 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/ursinamath.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     4350 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/ursinastuff.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     1330 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/vec2.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     2681 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/vec3.py
--rw-rw-r--   0 poke      (1000) poke      (1000)     1877 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/vec4.py
--rw-rw-r--   0 poke      (1000) poke      (1000)    15999 2023-01-30 22:37:45.000000 ursina-5.2.0/ursina/window.py
-drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-01-30 22:38:33.717384 ursina-5.2.0/ursina.egg-info/
--rw-rw-r--   0 poke      (1000) poke      (1000)     4606 2023-01-30 22:38:33.000000 ursina-5.2.0/ursina.egg-info/PKG-INFO
--rw-rw-r--   0 poke      (1000) poke      (1000)     6082 2023-01-30 22:38:33.000000 ursina-5.2.0/ursina.egg-info/SOURCES.txt
--rw-rw-r--   0 poke      (1000) poke      (1000)        1 2023-01-30 22:38:33.000000 ursina-5.2.0/ursina.egg-info/dependency_links.txt
--rw-rw-r--   0 poke      (1000) poke      (1000)      116 2023-01-30 22:38:33.000000 ursina-5.2.0/ursina.egg-info/requires.txt
--rw-rw-r--   0 poke      (1000) poke      (1000)        7 2023-01-30 22:38:33.000000 ursina-5.2.0/ursina.egg-info/top_level.txt
+drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-05-07 14:08:20.388439 ursina-5.3.0/
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1091 2023-05-07 11:54:49.000000 ursina-5.3.0/LICENSE
+-rw-rw-r--   0 poke      (1000) poke      (1000)      302 2023-05-07 11:54:49.000000 ursina-5.3.0/MANIFEST.in
+-rw-rw-r--   0 poke      (1000) poke      (1000)     4607 2023-05-07 14:08:20.388439 ursina-5.3.0/PKG-INFO
+-rw-rw-r--   0 poke      (1000) poke      (1000)     4370 2023-05-07 11:54:49.000000 ursina-5.3.0/README.md
+-rw-rw-r--   0 poke      (1000) poke      (1000)       38 2023-05-07 14:08:20.388439 ursina-5.3.0/setup.cfg
+-rw-rw-r--   0 poke      (1000) poke      (1000)      874 2023-05-07 11:54:49.000000 ursina-5.3.0/setup.py
+drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-05-07 14:08:20.384439 ursina-5.3.0/ursina/
+-rw-rw-r--   0 poke      (1000) poke      (1000)     3162 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/__init__.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2686 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/application.py
+drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-05-07 14:08:20.384439 ursina-5.3.0/ursina/audio/
+-rw-rw-r--   0 poke      (1000) poke      (1000)   176444 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/audio/noise.wav
+-rw-rw-r--   0 poke      (1000) poke      (1000)      288 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/audio/sine.wav
+-rw-rw-r--   0 poke      (1000) poke      (1000)      484 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/audio/square.wav
+-rw-rw-r--   0 poke      (1000) poke      (1000)      488 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/audio/triangle.wav
+-rw-rw-r--   0 poke      (1000) poke      (1000)     6375 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/audio.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     4360 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/boxcast.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     9910 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/build.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     7848 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/camera.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     7858 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/collider.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     5120 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/color.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     8680 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/curve.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2450 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/duplicate.py
+drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-05-07 14:08:20.384439 ursina-5.3.0/ursina/editor/
+-rw-rw-r--   0 poke      (1000) poke      (1000)        0 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/editor/__init__.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)    95025 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/editor/level_editor.py
+drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-05-07 14:08:20.384439 ursina-5.3.0/ursina/editor/scenes/
+-rw-rw-r--   0 poke      (1000) poke      (1000)        0 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/editor/scenes/__init__.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     5198 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/editor/scenes/test2[1,0].py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     6802 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/editor/scenes/untitled_scene[0,0].py
+-rw-rw-r--   0 poke      (1000) poke      (1000)      278 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/editor/scenes/untitled_scene[1,1].py
+-rw-rw-r--   0 poke      (1000) poke      (1000)      444 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/editor/scenes/untitled_scene[1,2].py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     3277 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/editor/scenes/untitled_scene[2,0].py
+-rw-rw-r--   0 poke      (1000) poke      (1000)      784 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/editor/scenes/untitled_scene[2,3].py
+-rw-rw-r--   0 poke      (1000) poke      (1000)    46866 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/entity.py
+drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-05-07 14:08:20.384439 ursina-5.3.0/ursina/fonts/
+-rw-rw-r--   0 poke      (1000) poke      (1000)     6075 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/fonts/Bitstream Vera License.txt
+-rw-rw-r--   0 poke      (1000) poke      (1000)    11560 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/fonts/LICENSE.txt
+-rw-rw-r--   0 poke      (1000) poke      (1000)    96428 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/fonts/OpenSans-Regular.ttf
+-rw-rw-r--   0 poke      (1000) poke      (1000)    49224 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/fonts/VeraMono.ttf
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2973 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/gamepad.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)      590 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/hit_info.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     4842 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/input_handler.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     3082 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/lights.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)    11966 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/main.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)    10941 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/mesh.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)    21666 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/mesh_importer.py
+drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-05-07 14:08:20.384439 ursina-5.3.0/ursina/models/
+-rw-rw-r--   0 poke      (1000) poke      (1000)        0 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models/__init__.py
+drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-05-07 14:08:20.384439 ursina-5.3.0/ursina/models/procedural/
+-rw-rw-r--   0 poke      (1000) poke      (1000)        0 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models/procedural/__init__.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)      797 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models/procedural/capsule.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)      940 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models/procedural/circle.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1441 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models/procedural/cone.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1642 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models/procedural/cube.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)      736 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models/procedural/cylinder.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)      789 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models/procedural/grid.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     5106 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models/procedural/pipe.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)      914 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models/procedural/plane.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     3993 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models/procedural/quad.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     3947 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models/procedural/terrain.py
+drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-05-07 14:08:20.384439 ursina-5.3.0/ursina/models_compressed/
+-rw-rw-r--   0 poke      (1000) poke      (1000)     4916 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models_compressed/arrow.ursinamesh
+-rw-rw-r--   0 poke      (1000) poke      (1000)     5801 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models_compressed/circle.ursinamesh
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1837 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models_compressed/cube.ursinamesh
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1892 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models_compressed/cube_uv_top.ursinamesh
+-rw-rw-r--   0 poke      (1000) poke      (1000)      153 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models_compressed/diamond.ursinamesh
+-rw-rw-r--   0 poke      (1000) poke      (1000)     3381 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models_compressed/icosphere.ursinamesh
+-rw-rw-r--   0 poke      (1000) poke      (1000)       56 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models_compressed/line.ursinamesh
+-rw-rw-r--   0 poke      (1000) poke      (1000)      389 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models_compressed/plane.ursinamesh
+-rw-rw-r--   0 poke      (1000) poke      (1000)      386 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models_compressed/quad.ursinamesh
+-rw-rw-r--   0 poke      (1000) poke      (1000)     7100 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models_compressed/scale_gizmo.ursinamesh
+-rw-rw-r--   0 poke      (1000) poke      (1000)   205071 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models_compressed/sky_dome.ursinamesh
+-rw-rw-r--   0 poke      (1000) poke      (1000)   218850 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models_compressed/sphere.ursinamesh
+-rw-rw-r--   0 poke      (1000) poke      (1000)      206 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models_compressed/wireframe_cube.ursinamesh
+-rw-rw-r--   0 poke      (1000) poke      (1000)      124 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/models_compressed/wireframe_quad.ursinamesh
+-rw-rw-r--   0 poke      (1000) poke      (1000)    12172 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/mouse.py
+drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-05-07 14:08:20.388439 ursina-5.3.0/ursina/prefabs/
+-rw-rw-r--   0 poke      (1000) poke      (1000)        0 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/__init__.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     3312 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/animation.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1782 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/animator.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     7015 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/button.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     3537 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/button_group.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     3403 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/button_list.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2726 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/color_picker.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)    10028 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/conversation.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)      932 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/cursor.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     4707 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/draggable.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2568 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/dropdown_menu.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     8073 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/editor_camera.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     7831 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/file_browser.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2342 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/file_browser_save.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     6646 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/first_person_controller.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2628 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/frame_animation_3d.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)    11167 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/grid_editor.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     3297 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/health_bar.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)    13287 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/hot_reloader.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     5021 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/input_field.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)      547 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/made_with_ursina.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1182 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/memory_counter.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)      464 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/panel.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     7669 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/platformer_controller_2d.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)      913 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/primitives.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2883 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/radial_menu.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)      561 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/sky.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     5423 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/slider.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)      784 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/sprite.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2359 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/sprite_sheet_animation.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)    33795 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/text_field.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     9249 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/tilemap.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1318 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/tooltip.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2617 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/trail_renderer.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)    12457 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/ursfx.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)      604 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/ursina_splash.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     5703 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/video_recorder.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     4138 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/prefabs/window_panel.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     6230 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/raycast.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2334 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/scene.py
+drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-05-07 14:08:20.388439 ursina-5.3.0/ursina/scripts/
+-rw-rw-r--   0 poke      (1000) poke      (1000)        0 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/scripts/__init__.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1445 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/scripts/_bat_to_exe.bat
+-rw-rw-r--   0 poke      (1000) poke      (1000)      735 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/scripts/_blend_export.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     5094 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/scripts/_blender_scene_to_ursina.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2268 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/scripts/chunk_mesh.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2146 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/scripts/colorize.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     3290 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/scripts/combine.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     3820 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/scripts/generate_normals.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2444 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/scripts/grid_layout.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1417 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/scripts/merge_vertices.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     3107 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/scripts/noclip_mode.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)      620 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/scripts/position_limiter.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)      628 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/scripts/project_uvs.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1594 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/scripts/scrollable.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1320 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/scripts/smooth_follow.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2917 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/scripts/terraincast.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     3341 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/sequence.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2943 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shader.py
+drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-05-07 14:08:20.388439 ursina-5.3.0/ursina/shaders/
+-rw-rw-r--   0 poke      (1000) poke      (1000)      950 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shaders/__init__.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1969 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shaders/basic_lighting_shader.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     3107 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shaders/colored_lights_shader.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     3206 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shaders/fresnel_shader.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1869 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shaders/geom_shader.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2447 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shaders/instancing_shader.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     5352 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shaders/lit_with_shadows_shader.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1773 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shaders/matcap_shader.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1220 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shaders/noise_fog_shader.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1372 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shaders/normals_shader.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     3375 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shaders/projector_shader.py
+drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-05-07 14:08:20.388439 ursina-5.3.0/ursina/shaders/screenspace_shaders/
+-rw-rw-r--   0 poke      (1000) poke      (1000)      905 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shaders/screenspace_shaders/camera_contrast.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)      973 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shaders/screenspace_shaders/camera_empty.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)      820 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shaders/screenspace_shaders/camera_grayscale.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2257 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shaders/screenspace_shaders/camera_outline_shader.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1222 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shaders/screenspace_shaders/camera_vertical_blur.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     4002 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shaders/screenspace_shaders/fxaa.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)      647 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shaders/screenspace_shaders/pixelation_shader.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     4138 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shaders/screenspace_shaders/ssao.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     3065 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shaders/texture_blend_shader.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1835 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shaders/transition_shader.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     4355 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shaders/triplanar_shader.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1690 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/shaders/unlit_shader.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1745 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/string_utilities.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)    15356 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/text.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     7912 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/texture.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     4008 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/texture_importer.py
+drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-05-07 14:08:20.388439 ursina-5.3.0/ursina/textures/
+-rw-rw-r--   0 poke      (1000) poke      (1000)     3018 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/arrow_down.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)     3025 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/arrow_right.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2896 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/brick.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)     3683 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/circle.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)     4194 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/circle_outlined.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)     3351 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/cog.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)    14902 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/cursor.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2895 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/file_icon.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2891 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/folder.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)    23748 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/grass.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)   848864 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/grass_tintable.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)    21070 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/heightmap_1.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2829 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/horizontal_gradient.png
+drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-05-07 14:08:20.388439 ursina-5.3.0/ursina/textures/items/
+-rw-rw-r--   0 poke      (1000) poke      (1000)    44186 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/items/bag.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)    26101 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/items/bow_arrow.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)    45394 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/items/gem.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)   324040 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/items/items.psd
+-rw-rw-r--   0 poke      (1000) poke      (1000)    16168 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/items/orb.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)    40572 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/items/sword.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)     7196 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/noise.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)   173070 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/perlin_noise.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)     6775 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/radial_gradient.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2875 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/rainbow.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)     6476 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/reflection_map_3.jpg
+-rw-rw-r--   0 poke      (1000) poke      (1000)   222963 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/shore.jpg
+-rw-rw-r--   0 poke      (1000) poke      (1000)   121903 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/sky_default.jpg
+-rw-rw-r--   0 poke      (1000) poke      (1000)   125956 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/sky_sunset.jpg
+-rw-rw-r--   0 poke      (1000) poke      (1000)     5326 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/test_tileset.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)      690 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/tilemap_test_level.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)    17689 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/ursina_logo.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)      760 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/ursina_wink_0000.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)      827 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/ursina_wink_0001.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2825 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/vertical_gradient.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)    32461 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/vignette.jpg
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2909 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/textures/white_cube.png
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1871 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/trigger.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     5367 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/ursinamath.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     4213 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/ursinastuff.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1330 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/vec2.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     2681 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/vec3.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)     1877 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/vec4.py
+-rw-rw-r--   0 poke      (1000) poke      (1000)    15350 2023-05-07 11:54:49.000000 ursina-5.3.0/ursina/window.py
+drwxrwxr-x   0 poke      (1000) poke      (1000)        0 2023-05-07 14:08:20.384439 ursina-5.3.0/ursina.egg-info/
+-rw-rw-r--   0 poke      (1000) poke      (1000)     4607 2023-05-07 14:08:20.000000 ursina-5.3.0/ursina.egg-info/PKG-INFO
+-rw-rw-r--   0 poke      (1000) poke      (1000)     6113 2023-05-07 14:08:20.000000 ursina-5.3.0/ursina.egg-info/SOURCES.txt
+-rw-rw-r--   0 poke      (1000) poke      (1000)        1 2023-05-07 14:08:20.000000 ursina-5.3.0/ursina.egg-info/dependency_links.txt
+-rw-rw-r--   0 poke      (1000) poke      (1000)       91 2023-05-07 14:08:20.000000 ursina-5.3.0/ursina.egg-info/requires.txt
+-rw-rw-r--   0 poke      (1000) poke      (1000)        7 2023-05-07 14:08:20.000000 ursina-5.3.0/ursina.egg-info/top_level.txt
```

### Comparing `ursina-5.2.0/LICENSE` & `ursina-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/PKG-INFO` & `ursina-5.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ursina
-Version: 5.2.0
+Version: 5.3.0
 Summary: An easy to use game engine/framework for python.
 Home-page: https://github.com/pokepetter/ursina
 Author: Petter Amland
 Author-email: pokepetter@gmail.com
 License: MIT
 Keywords: game development
 Platform: UNKNOWN
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: extras
 License-File: LICENSE
 
 # ursina    ʕ •ᴥ•ʔゝ□
 An easy to use game engine/framework for python.
```

### Comparing `ursina-5.2.0/README.md` & `ursina-5.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/setup.py` & `ursina-5.3.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,32 +4,32 @@
     long_desc = f.read()
 
 setup(
     name='ursina',
     description='An easy to use game engine/framework for python.',
     long_description=long_desc,
     long_description_content_type="text/markdown",
-    version='5.2.0',
+    version='5.3.0',
     url='https://github.com/pokepetter/ursina',
     author='Petter Amland',
     author_email='pokepetter@gmail.com',
     license='MIT',
     keywords='game development',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'panda3d',
         'panda3d-gltf',
         'pillow',
         'pyperclip',
-        'Xlib; platform_system == "Linux"',
+        'screeninfo',
     ],
 
     extras_require={'extras': [
         'numpy',
         'imageio',
         'psd-tools3',
         'psutil',
         ],
     },
-    python_requires='>=3.6',
+    python_requires='>=3.10',
 )
```

### Comparing `ursina-5.2.0/ursina/__init__.py` & `ursina-5.3.0/ursina/__init__.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/application.py` & `ursina-5.3.0/ursina/application.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 import sys
 from pathlib import Path
 from panda3d.core import getModelPath
 from ursina import string_utilities
 
 paused = False
 time_scale = 1
+calculate_dt = True
 sequences = []
 trace_entity_definition = False # enable to set entity.line_definition
 print_entity_definition = False
 
 package_folder = Path(__file__).parent
 asset_folder = Path(sys.argv[0]).parent
 blender_paths = dict()
 
 development_mode = True
 dirs = [e.stem for e in asset_folder.parent.iterdir() if e.is_dir()]
 if 'src' in dirs and 'python' in dirs:
     development_mode = False
 
+window_type = 'onscreen'
+
+gltf_no_srgb = True
+
 print_info = development_mode
 print_warnings = True
 raise_exception_on_missing_model = False
 raise_exception_on_missing_texture = False
 
 internal_models_folder = package_folder / 'models/'
 internal_models_compressed_folder = package_folder / 'models_compressed/'
```

### Comparing `ursina-5.2.0/ursina/audio/noise.wav` & `ursina-5.3.0/ursina/audio/noise.wav`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/audio.py` & `ursina-5.3.0/ursina/audio.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/boxcast.py` & `ursina-5.3.0/ursina/boxcast.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/build.py` & `ursina-5.3.0/ursina/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from modulefinder import ModuleFinder
 import os
 import sys
 import shutil
-from shutil import copy, copyfile
-from distutils.dir_util import copy_tree
+from shutil import copy, copyfile, copytree
 from pathlib import Path
 import time
 from textwrap import dedent
+import platform
 
 project_folder = Path.cwd()
 project_name = project_folder.stem
-build_folder = Path(project_folder / 'build')
+build_folder = Path(project_folder / f'build_{platform.system()}')
 build_folder.mkdir(exist_ok=True)
 
 ignore = []
 
 compressed_textures = []
 compressed_textures_folder = Path(project_folder/'textures_compressed')
 if compressed_textures_folder.exists():
@@ -60,22 +60,23 @@
     if arg == '--help':
         print(dedent('''
             package ursina application for windows10.
             provided with project folder path, creates a build folder where
             it copies python and project's dependent packages. requires a main.py file.
             copies game scripts and assets into 'build/src' folder.
             creates a .bat file to start the game.
-            include extra modules like this: --include_modules module_one,module_two,module_tree
+
             --ignore            # add assets to ignore
             --name              # change project name
-            --include_modules   # include extra modules
+            --include_modules   # include extra modules like this: --include_modules module_one,module_two,module_tree
             --overwrite         # don't ask to overwrite existing build, just overwrite
             --skip_engine
             --skip_game
-            --compile_to_pyc    # default: True
+            --compile_to_pyc=True
+            --compile_to_pyc=False
 
             Make sure to include any extra modules with --include_modules PIL,numpy for example.
             Any errors while the application is running will be logged in log.txt instead of the console.
             '''
             )
         )
         sys.exit()
@@ -94,16 +95,18 @@
         include_modules = sys.argv[i+1].split(',')
 
     elif arg == '--skip_engine':
         build_engine = False
     elif arg == '--skip_game':
         build_game = False
 
-    elif arg == '--compile_to_pyc':
-        compile_to_pyc = bool(sys.argv[i+1])
+    elif arg == '--compile_to_pyc=True':
+        compile_to_pyc = True
+    elif arg == '--compile_to_pyc=False':
+        compile_to_pyc = False
 
 
 if (build_engine and python_dest.exists() or (build_game and src_dest.exists())):
     if not '--overwrite' in sys.argv:
         for e in (python_dest, src_dest):
             msg = f'Folder {e} already exists. \nProceed to delete and overwrite?'
             overwrite = input("%s (y/N) " % msg).lower() == 'y'
@@ -147,18 +150,20 @@
         'Lib/collections',
         'Lib/ctypes',
         'Lib/encodings',
         'Lib/importlib',
         'Lib/urllib',
         'Lib/logging',
         'Lib/xml',
+        'Lib/re',
         # 'Lib/site-packages/panda3d/',
         'Lib/site-packages/direct/',
         'Lib/site-packages/pyperclip/',
         'Lib/site-packages/PIL/',
+        'Lib/site-packages/screeninfo/',
         'DLLs/libffi-7.dll',
         'DLLs/_ctypes.pyd',
         ]
 
     for path in always_include + include_modules:
         source = python_folder / path
         dest = python_dest / path
@@ -229,25 +234,24 @@
 
 
 if build_game:
     if src_dest.exists():
         shutil.rmtree(str(src_dest))
     src_dest.mkdir()
 
-    ignore.extend(['.git', 'build', '.gitignore', 'build.bat'])
+    ignore.extend(['.git', 'build_Windows', 'build_Linux', '.gitignore', 'build.bat'])
     ignore_patterns = ['.psd', '.zip']
     ignore.append('__pycache__')
 
     if compile_to_pyc:
         import py_compile
         for f in project_folder.glob('**/*.py'):
-            if '\\build\\' in str(f):
+            parents = f.relative_to(project_folder).parents
+            if 'scenes' in parents:
                 continue
-
-            print('compiling:', f, src_dest / str(f)[len(str(project_folder))+1:])
             py_compile.compile(f, src_dest / (str(f)[len(str(project_folder))+1:]+'c'))
 
         ignore_patterns.append('.py')
 
 
     print('copying assets')
     for f in project_folder.iterdir():
```

### Comparing `ursina-5.2.0/ursina/camera.py` & `ursina-5.3.0/ursina/camera.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/collider.py` & `ursina-5.3.0/ursina/collider.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/color.py` & `ursina-5.3.0/ursina/color.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/curve.py` & `ursina-5.3.0/ursina/curve.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/duplicate.py` & `ursina-5.3.0/ursina/duplicate.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/editor/level_editor.py` & `ursina-5.3.0/ursina/editor/level_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from ursina import *
 from ursina.shaders import unlit_shader, lit_with_shadows_shader, matcap_shader, triplanar_shader, normals_shader
 from time import perf_counter
+import csv
 
 
+# from ursina.editor.prefabs.poke_shape import PokeShape
 
-class LevelEditorScene(Entity):
+
+class LevelEditorScene:
     def __init__(self, x, y, name, **kwargs):
         super().__init__()
         self.coordinates = [x,y]
         self.name = name
         self.path = None    # must be assigned to be able to load
         self.entities = []
         self.selection = []
@@ -17,79 +20,68 @@
 
     def save(self):
         if not self.path and not self.entities:
             print('cant save scene with not path and no entities')
             return
 
         level_editor.scene_folder.mkdir(parents=True, exist_ok=True)
-        # create __init__ file in scene folder so we can import it during self.load()
-        if not Path(level_editor.scene_folder / '__init__.py').is_file():
-            print('creating an __init__.py in the scene folder')
-            with open(level_editor.scene_folder / '__init__.py', 'w', encoding='utf-8') as f:
-                pass
-
-        print('saving:', self.name)
-        scene_file_content = dedent(f'''
-            class Scene(Entity):
-                def __init__(self, **kwargs):
-                    super().__init__(**kwargs)
-        ''')
+        list_of_dicts = []
 
-        for e in self.entities:
+        fields = ['class', ]
+        for e in level_editor.current_scene.entities:
             if hasattr(e, 'is_gizmo'):
                 continue
 
-            scene_file_content += '        '
-            if e.name != camel_to_snake(e.__class__.__name__):
-                scene_file_content += f'self.{camel_to_snake(e.__class__.__name__)} = '
-
-            scene_file_content += f'{e.__class__.__name__}(parent=self, '
-
-            if hasattr(e, '__repr__'):
-
-                # print('------------', repr(e), e.__class__.__name__)
-                recipe = repr(e).split(e.__class__.__name__)[1][1:-1] # remove start and end
-                scene_file_content += recipe
-                scene_file_content += ')\n' # TODO: add if it has a custom name
-
-        # print('scene_file_content:\n', scene_file_content)
-        self.path = level_editor.scene_folder/(self.name+'.py')
-        with open(self.path, 'w', encoding='utf-8') as f:
-            f.write(scene_file_content)
+            changes = e.get_changes()
+            changes['class'] = e.__class__.__name__
+            list_of_dicts.append(changes)
+            for key in changes.keys():
+                if key not in fields:
+                    fields.append(key)
+
+
+        name = level_editor.current_scene.name
+        self.path =  level_editor.scene_folder / f'{name}.csv'
+
+        with self.path.open('w', encoding='UTF8') as file:
+            writer = csv.DictWriter(file, fieldnames=fields, delimiter=';')
+            writer.writeheader()
+            writer.writerows(list_of_dicts)
+
         print('saved:', self.path)
 
 
     def load(self):
         if not self.path:
             print('cant load scene, no path')
             return
         if self.scene_parent:
             print('error, scene already loaded')
             return
 
         t = perf_counter()
+        with self.path.open('r') as f:
+            self.scene_parent = Entity()
+            reader = csv.DictReader(f, delimiter=';')
+            fields = reader.fieldnames[1:]
+
+            for line in reader:
+                args = ', '.join([f'{key}={value}' for key, value in line.items() if value and not key=='class'])
+                e = eval(f'{line["class"]}(parent=self.scene_parent, {args})')
 
-        with open(self.path) as f:
-            try:
-                entities_before_exec = [e for e in scene.entities]
-                exec(f.read())
-                self.scene_parent = eval(f'Scene()')
-                self.scene_parent.name = self.name
-                self.entities = [e for e in scene.entities if e.has_ancestor(self.scene_parent) and not hasattr(e, 'is_gizmo')]
+                self.entities.append(e)
                 for e in self.entities:
                     if not e.shader:
                         e.shader = lit_with_shadows_shader
                     e.selectable = True
                     e.original_parent = e.parent
                     if e.model.name == 'cube':
                         e.collider = 'box'
                         e.collision = False
 
-            except Exception as e:
-                print('error in scene:', self.name, e)
 
         if self.scene_parent:
             print(f'loaded scene: "{self.name}" in {perf_counter()-t}')
             return self.scene_parent
 
 
     def unload(self):
@@ -100,39 +92,39 @@
         #     return
 
         self.selection = []
         self.entities = []
         destroy(self.scene_parent)
 
 
+
 class LevelEditor(Entity):
     def __init__(self, **kwargs):
         super().__init__()
 
         self.scene_folder = application.asset_folder / 'scenes'
         self.scenes = [[LevelEditorScene(x, y, f'untitled_scene[{x},{y}]') for y in range(8)] for x in range(8)]
         self.current_scene = None
 
         self.grid = Entity(parent=self, model=Grid(16,16), rotation_x=90, scale=64, collider='box', color=color.white33, enabled=False)
         self.origin_mode = 'center'
         self.editor_camera = EditorCamera(parent=self, rotation_x=20, eternal=False, rotation_smoothing=0)
         self.ui = Entity(parent=camera.ui, name='level_editor.ui')
 
         self.point_renderer = Entity(parent=self, model=Mesh([], mode='point', thickness=.1, render_points_in_3d=True), texture='circle', always_on_top=True, unlit=True, render_queue=1)
-        self.cubes = [Entity(model='wireframe_cube', color=color.azure, parent=self, enabled=True) for i in range(128)] # max selection
+        self.cubes = [Entity(wireframe=True, color=color.azure, parent=self, enabled=True) for i in range(128)] # max selection
 
         self.origin_mode_menu = ButtonGroup(['last', 'center', 'individual'], min_selection=1, position=window.top, parent=self.ui)
         self.origin_mode_menu.scale *= .75
         self.origin_mode_menu.on_value_changed = self.render_selection
         self.local_global_menu = ButtonGroup(['local', 'global'], default='global', min_selection=1, position=window.top - Vec2(.2,0), parent=self.ui)
         self.local_global_menu.scale *= .75
         self.local_global_menu.on_value_changed = self.render_selection
         self.target_fov = 90
 
-
     @property
     def entities(self):
         if not self.current_scene:
             return []
         return self.current_scene.entities
 
     @property
@@ -222,16 +214,15 @@
 
         [e.disable() for e in self.cubes]
         # [setattr(e, 'parent', self) for e in self.cubes]
         for i, e in enumerate([e for e in self.selection if e.collider]):
             if i < len(self.cubes):
                 self.cubes[i].world_transform = e.world_transform
                 self.cubes[i].origin = e.origin
-
-                # self.cubes[i].parent = e
+                self.cubes[i].model = copy(e.model)
                 self.cubes[i].enabled = True
 
         # print('---------- rendered selection')
     def on_enable(self):
         if hasattr(self, 'ui'):
             self.ui.enabled = True
 
@@ -692,15 +683,15 @@
                 self.target.world_position = lerp(self.scaler.world_position, self.helper.world_position, .5)
 
 
 
 
 class GizmoToggler(Entity):
     def __init__(self, **kwargs):
-        super().__init__()
+        super().__init__(parent=level_editor)
         self.animator = Animator({
             'w' : gizmo.arrow_parent,
             'e' : scale_gizmo,
             'r' : rotation_gizmo,
             # 't' : box_gizmo,
 
             'q' : None,
@@ -709,15 +700,15 @@
     def input(self, key):
         if key in self.animator.animations:
             self.animator.state = key
 
 
 class QuickGrabber(Entity):
     def __init__(self, **kwargs):
-        super().__init__()
+        super().__init__(parent=level_editor)
         self.target_entity = None
         self.target_axis = None
         self.plane = Entity(model='quad', collider='box', scale=Vec3(100,100,1), visible_self=False, enabled=False)
         self.offset_helper = Entity()
         self.start_position = Vec3(0,0,0)
         self.axis_lock = [0,1,0]
         self.is_dragging = False
@@ -757,23 +748,32 @@
                 self._original_mouse_traverse_target = mouse.traverse_target
                 mouse.traverse_target = self.plane
                 mouse.update()
                 self.offset_helper.position = mouse.world_point
                 self.start_position = self.offset_helper.world_position
 
                 self.target_entity.original_parent = self.target_entity.parent
+                self.target_entity._original_world_position = self.target_entity.world_position
                 self.target_entity.world_parent = self.offset_helper
 
                 self.is_dragging = True
 
 
         elif key in ('x up', 'y up', 'z up', 'd up', 'w up') and self.target_entity:
             self.is_dragging = False
             mouse.traverse_target = self._original_mouse_traverse_target
             self.target_entity.world_parent = self.target_entity.original_parent
+
+            if self.target_entity.world_position != self.target_entity._original_world_position:
+                changes = []
+                for e in level_editor.selection:
+                    changes.append([level_editor.entities.index(e), 'world_position', e._original_world_position, e.world_position])
+
+                level_editor.current_scene.undo.record_undo(changes)
+
             self.target_entity = None
             self.plane.enabled = False
             level_editor.selection = []
             level_editor.render_selection()
 
 
     def update(self):
@@ -800,16 +800,14 @@
             },
             clear_selection=False,
             dragging=False,
             )
 
 
     def input(self, key):
-
-
         if held_keys['control'] or held_keys['shift'] or held_keys['alt']:
             return
 
         if (held_keys['x'] or held_keys['y'] or held_keys['z']) and key == 's':
             self.original_gizmo_state = gizmo_toggler.animator.state
             return
 
@@ -864,23 +862,29 @@
         for key in self.gizmos_to_toggle.keys():
             if held_keys[key] and not held_keys['control'] and not held_keys['shift'] and mouse.velocity != Vec3(0,0,0):
                 level_editor.render_selection(update_gizmo_position=False)
                 return
 
 
 class QuickRotator(Entity):
+    def __init__(self):
+        super().__init__(parent=level_editor)
+
     def input(self, key):
         if held_keys['control'] or held_keys['shift'] or held_keys['alt']:
             return
 
         if key == 'r' and len(level_editor.selection) <= 1:
             if not level_editor.selection:
                 level_editor.selection = [selector.get_hovered_entity(), ]
                 level_editor.render_selection()
 
+            if not level_editor.selection:
+                return
+
             self.target_entity = level_editor.selection[0]
             rotation_gizmo.subgizmos['y'].input('left mouse down')
             rotation_gizmo.subgizmos['y'].start_dragging()
 
         elif key == 'r up' and hasattr(self, 'target_entity') and self.target_entity:
             key = key[:-3]
             rotation_gizmo.subgizmos['y'].input('left mouse up')
@@ -890,14 +894,17 @@
             self.target_entity = None
 
 
 class RotateRelativeToView(Entity):
     _rotation_helper = Entity(name='RotateRelativeToView_rotation_helper')
     sensitivity = Vec2(200,200)
 
+    def __init__(self, **kwargs):
+        super().__init__(parent=level_editor, **kwargs)
+
     def input(self, key):
         if held_keys['control'] or held_keys['shift'] or held_keys['alt']:
             return
 
         if key == 'c':
             if len(level_editor.selection) > 1:
                 return
@@ -933,24 +940,28 @@
             __class__._rotation_helper.rotation_y -= mouse.velocity[0] * __class__.sensitivity.x / camera.aspect_ratio
             __class__._rotation_helper.rotation_x += mouse.velocity[1] * __class__.sensitivity.y
 
 
 
 
 class Selector(Entity):
+    def __init__(self):
+        super().__init__(parent=level_editor)
+
     def input(self, key):
         if key == 'left mouse down':
             if mouse.hovered_entity:
                 return
 
             clicked_entity = self.get_hovered_entity()
 
             if clicked_entity in level_editor.entities and not held_keys['alt']:
-                if held_keys['shift'] and not clicked_entity in level_editor.selection:
-                    level_editor.selection.append(clicked_entity) # append
+                if held_keys['shift']:
+                    if not clicked_entity in level_editor.selection:
+                        level_editor.selection.append(clicked_entity) # append
                 else:
                     print(clicked_entity)
                     level_editor.selection = [clicked_entity, ]   # overwrite
 
             if held_keys['alt'] and clicked_entity in level_editor.selection:
                 level_editor.selection.remove(clicked_entity) # remove
 
@@ -964,14 +975,16 @@
             level_editor.render_selection()
 
         elif key == 'h':
             level_editor.point_renderer.enabled = not level_editor.point_renderer.enabled
 
 
     def get_hovered_entity(self):
+        level_editor.entities = [e for e in level_editor.entities if e]
+        [print(str(e)) for e in level_editor.entities]
         entities_in_range = [(distance_2d(e.screen_position, mouse.position), e) for e in level_editor.entities if e.selectable and not e.collider]
         entities_in_range = [e for e in entities_in_range if e[0] < .03]
         entities_in_range.sort()
 
         clicked_entity = None
         if entities_in_range:
             return entities_in_range[0][1]
@@ -987,14 +1000,17 @@
             return mouse.hovered_entity
 
         [setattr(e, 'collision', False) for e in level_editor.entities if not hasattr(e, 'is_gizmo')]
 
 
 
 class SelectionBox(Entity):
+    def __init__(self, **kwargs):
+        super().__init__(parent=level_editor.ui, **kwargs)
+
     def input(self, key):
         if key == 'left mouse down':
             if mouse.hovered_entity and not mouse.hovered_entity in level_editor.selection:
                 # print('-------', 'clicked on gizmo, dont box select')
                 return
             self.position = mouse.position
             self.scale = .001
@@ -1065,18 +1081,25 @@
         super().__init__(model='procedural_rock_0', collider='box', color=hsv(20,.2,.45), **kwargs)
 
 
 class Spawner(Entity):
     def __init__(self):
         super().__init__(parent=level_editor)
         self.target = None
-        for i, prefab in enumerate([Cube, Pyramid, PokeShape]):
+        self.update_menu()
+
+    def update_menu(self):
+        for i, prefab in enumerate(prefabs):
             button = Button(parent=level_editor.ui, scale=.075/2, origin=(.5,-.5), position=window.bottom_right+Vec2(-.05 -(i*.0375),0), on_click=Func(self.spawn_entity, prefab))
-            button.text = str(prefab)
-            # self.button.i = Entity(parent=self.button, model='wireframe_cube', rotation=(-10,10,0), scale=.5, position=(-.5,.5,-1))
+            if hasattr(prefab, 'icon'):
+                button.icon = prefab.icon
+            else:
+                button.text = '\n'.join(chunk_list(prefab.__name__, 5))
+                button.text_entity.scale = .5
+
 
     def input(self, key):
         if key == 'i':
             mouse.traverse_target = level_editor.grid
             self.spawn_entity()
 
         elif key == 'i up' and self.target:
@@ -1113,34 +1136,41 @@
     def update(self):
         if mouse.world_point and self.target:
             if held_keys['n'] or mouse.left:
                 self.target.position = mouse.world_point
 
 
 class Deleter(Entity):
+    def __init__(self):
+        super().__init__(parent=level_editor)
+
     def input(self, key):
         if level_editor.selection and key == 'delete':
             self.delete_selected()
 
     def delete_selected(self):
         level_editor.current_scene.undo.record_undo((
             'restore entities',
             [level_editor.entities.index(e) for e in level_editor.selection],
             [repr(e) for e in level_editor.selection],
             ))
 
         [level_editor.entities.remove(e) for e in level_editor.selection]
+        [destroy(e) for e in level_editor.selection]
         [setattr(e, 'parent', level_editor) for e in level_editor.cubes]
-        [destroy(e, delay=1/60) for e in level_editor.selection]
+        level_editor.entities = [e for e in level_editor.entities if e]
         level_editor.selection = []
         level_editor.render_selection()
         hierarchy_list.render_selection()
 
 
 class PointOfViewSelector(Entity):
+    def __init__(self):
+        super().__init__(parent=level_editor)
+
     def __init__(self, **kwargs):
 
         super().__init__(parent=level_editor.ui, model='cube', collider='box', texture='white_cube', scale=.05, position=window.top_right-Vec2(.1,.05))
         self.front_text = Text(parent=self, text='front', z=-.5, scale=10, origin=(0,0), color=color.azure)
 
         for key, value in kwargs.items():
             setattr(self, key, value)
@@ -1154,18 +1184,19 @@
         elif mouse.normal == Vec3(0,-1,0): level_editor.editor_camera.animate_rotation((-90,0,0)) # top
 
 
     def update(self):
         self.rotation = -level_editor.editor_camera.rotation
 
     def input(self, key):
-        if key == '1':   level_editor.editor_camera.animate_rotation((0,0,0)) # front
-        elif key == '3': level_editor.editor_camera.animate_rotation((0,90,0)) # right
-        elif key == '7': level_editor.editor_camera.animate_rotation((90,0,0)) # top
-        elif key == '5': camera.orthographic = not camera.orthographic
+        if held_keys['shift']:
+            if key == '1':   level_editor.editor_camera.animate_rotation((0,0,0)) # front
+            elif key == '3': level_editor.editor_camera.animate_rotation((0,90,0)) # right
+            elif key == '7': level_editor.editor_camera.animate_rotation((90,0,0)) # top
+            elif key == '5': camera.orthographic = not camera.orthographic
 
 
 # class PaintBucket(Entity):
 #     def input(self, key):
 #         if held_keys['alt'] and key == 'c' and mouse.hovered_entity:
 #             self.color = mouse.hovered_entity.color
 
@@ -1189,15 +1220,15 @@
 
         self.load_scenes()
         # self.goto_scene(0, 0)
         self.draw()
 
 
     def load_scenes(self):
-        for scene_file in level_editor.scene_folder.glob('*.py'):
+        for scene_file in level_editor.scene_folder.glob('*.csv'):
             if '__' in scene_file.name:
                 continue
 
             print('found scene:', scene_file)
             name = scene_file.stem
             if '[' in name and ']' in name:
                 x, y = (int(e) for e in name.split('[')[1].split(']')[0].split(','))
@@ -1378,29 +1409,29 @@
 
         for y, names in enumerate((('x','y','z'), ('rotation_x','rotation_y','rotation_z'), ('scale_x','scale_y','scale_z'))):
             for x in range(3):
                 default = '0'
                 if y == 2:
                     default = '1'
 
-                field = InputField(max_width=5, model='quad', parent=self.name_field, scale_x=1/3, scale_y=1, origin=(-.5,.5), default_value=default, limit_content_to=ContentTypes.math, x=x/3, y=-y-1, color=color._8)
+                field = InputField(max_width=8, model='quad', parent=self.name_field, scale_x=1/3, scale_y=1, origin=(-.5,.5), default_value=default, limit_content_to=ContentTypes.math, x=x/3, y=-y-1, color=color._8)
                 def on_submit(names=names, x=x, field=field):
                     try:
-                        value = float(eval(field.text))
+                        value = float(eval(field.text[:8]))
                         if isinstance(value, float):
-                            field.text = str(value)
-                            # for e in level_editor.selection:
-                            #     setattr(e, names[x], value)
+                            field.text_field.text_entity.text = str(value)[:8]
+                            for e in level_editor.selection:
+                                setattr(e, names[x], float(field.text_field.text_entity.text))
                     except: # invalid/incomplete math
                         # print('invalid')
                         return
 
                 # field.submit_on = 'enter'
                 field.on_submit = on_submit
-                # field.on_value_changed = on_submit
+                field.on_value_changed = on_submit
 
                 self.transform_fields.append(field)
                 self.input_fields.append(field)
 
         for i in range(len(self.transform_fields)-1):
             self.transform_fields[i].next_field = self.transform_fields[i+1]
 
@@ -1453,15 +1484,15 @@
             self.fields['color'].color = level_editor.selection[0].color
 
             if len(level_editor.selection) == 1:
                 selected = level_editor.selection[0]
 
                 self.name_field.text_field.text_entity.text = selected.name
                 for i, attr_name in enumerate(('world_x', 'world_y', 'world_z', 'world_rotation_x', 'world_rotation_y', 'world_rotation_z', 'world_scale_x', 'world_scale_y', 'world_scale_z')):
-                    self.transform_fields[i].text = str(getattr(selected, attr_name))[:5]
+                    self.transform_fields[i].text = str(round(getattr(selected, attr_name),4))
 
                 [destroy(e) for e in self.shader_inputs_parent.children]
                 if selected.shader:
                     for i, (name, value) in enumerate(selected.shader.default_input.items()):
                         print('shader input', name, value)
                         b = Button(parent=self.shader_inputs_parent, model='quad', origin=(-.5,.5), text_origin=(-.5,0),
                             text_color=color.light_gray, text=f' {name}:', color=color.black90, highlight_color=color._32, y=-i,
@@ -1490,15 +1521,15 @@
             #     self.fields['texture'].text_entity.text = '--------'
             #     self.fields['color'].color = color._8
             #     self.fields['shader'].text_entity.text = '--------'
             #     [destroy(e) for e in self.shader_inputs_parent.children]
 
 class MenuHandler(Entity):
     def __init__(self):
-        super().__init__()
+        super().__init__(parent=level_editor)
         self._state = None
         self.states = {
             'None' : None,
             'model_menu' : model_menu,
             'texture_menu' : texture_menu,
             'shader_menu' : shader_menu,
             'color_menu' : color_menu,
@@ -1716,15 +1747,15 @@
             background=True,
             scale=.25
         )
         self.tooltip.original_scale = .75
 
 class Duplicator(Entity):
     def __init__(self, **kwargs):
-        super().__init__(clones=None)
+        super().__init__(parent=level_editor, clones=None)
         self.plane = Entity(model='plane', collider='box', scale=Vec3(100,.1,100), enabled=False, visible=False)
         self.dragger = Draggable(parent=scene, model=None, collider=None, enabled=False)
         self.dragging = False
         self.start_position = None
         self.clone_from_position = None
         self.axis_lock = None
         self.axis_lock_gizmos = [
@@ -1806,71 +1837,100 @@
 class PokeShape(Entity):
     default_values = Entity.default_values | dict(points=[Vec3(-.5,0,-.5), Vec3(.5,0,-.5), Vec3(.5,0,.5), Vec3(-.5,0,.5)], name='poke_shape') # combine dicts
 
     def __init__(self, points=[Vec3(-.5,0,-.5), Vec3(.5,0,-.5), Vec3(.5,0,.5), Vec3(-.5,0,.5)], **kwargs):
 
         self.original_parent = level_editor
         self.selectable = True
+        self.highlight_color = color.blue
         super().__init__(**__class__.default_values | kwargs)
         level_editor.entities.append(self)
         self.model = Mesh()
 
         self.point_gizmos = LoopingList([Entity(parent=self, original_parent=self, position=e, selectable=False, name='PokeShape_point', is_gizmo=True) for e in points])
-        self.edit_mode = False
+        self.add_new_point_renderer = Entity(model=Mesh(vertices=[], mode='point', thickness=.075), color=color.white, alpha=.5, texture='circle', unlit=True, is_gizmo=True, selectable=False, enabled=False, always_on_top=True)
 
         self.add_collider = False
 
         self.make_wall = True
         self.wall_parent = None
         if self.make_wall:
             self.wall_parent = Entity(parent=self, model=Mesh(), color=color.dark_gray, add_to_scene_entities=False)
 
         self.wall_height = 1
         self.wall_thickness = .1
+        self.subdivisions = 3
+        self.smoothing_distance = .1
 
+        self._edit_mode = False
         self.generate()
+        self.edit_mode = False
 
 
     def generate(self):
         import tripy
-        polygon = LoopingList(e.get_position(relative_to=self).xz for e in self.point_gizmos)
+        self.point_gizmos = LoopingList([e for e in self.point_gizmos if e])
+        polygon = LoopingList(Vec2(*e.get_position(relative_to=self).xz) for e in self.point_gizmos)
+
+        if self.subdivisions:
+            for j in range(self.subdivisions):
+                smooth_polygon = LoopingList()
+                for i, p in enumerate(polygon):
+                    smooth_polygon.append(lerp(p, polygon[i-1], self.smoothing_distance))
+                    smooth_polygon.append(lerp(p, polygon[i+1], self.smoothing_distance))
+                polygon = smooth_polygon
+
         triangles = tripy.earclip(polygon)
         self.model.vertices = []
         for tri in triangles:
             for v in tri:
                 self.model.vertices.append(Vec3(v[0], 0, v[1]))
 
         self.model.uvs = [Vec2(v[0],v[2])*1 for v in self.model.vertices]
         self.model.normals = [Vec3(0,1,0) for i in range(len(self.model.vertices))]
         self.model.generate()
         self.texture = 'grass'
-
+        self.texture_scale = Vec2(.125)
+        # [destroy(e) for e in self.wall_parent.children]
 
         if self.make_wall:
-            wall_verts = []
-            for i, vert in enumerate(polygon):
-                vert = Vec3(vert[0], 0, vert[1])
-                next_vert = Vec3(polygon[i+1][0], 0, polygon[i+1][1])
-
-                wall_verts.extend((
-                    vert,
-                    vert + Vec3(0,-1,0),
-                    next_vert,
-
-                    next_vert,
-                    vert + Vec3(0,-1,0),
-                    next_vert + Vec3(0,-1,0),
-                ))
+            pass
+            polygon_3d = [Vec3(e[0], 0, e[1]) for e in polygon]
+            polygon_3d.append(polygon_3d[0])
+            self.wall_parent.model = Pipe(base_shape=Quad(0), path=polygon_3d)
+            # wall_verts = []
+            # for i, vert in enumerate(polygon):
+            #     vert = Vec3(vert[0], 0, vert[1])
+            #     next_vert = Vec3(polygon[i+1][0], 0, polygon[i+1][1])
+            #
+            #     wall_verts.extend((
+            #         vert,
+            #         vert + Vec3(0,-1,0),
+            #         next_vert,
+            #
+            #         next_vert,
+            #         vert + Vec3(0,-1,0),
+            #         next_vert + Vec3(0,-1,0),
+            #     ))
+            # #     # wall = Entity(model='cube', origin_x=-.5, scale=.1, position=vert, scale_x=distance(vert, next_vert), color=color.blue, parent=self.wall_parent, add_to_scene_entities=False)
+            # #     # wall.look_at(next_vert, 'right')
+            # #
+            # self.wall_parent.model.vertices = wall_verts
+            # self.wall_parent.model.generate()
 
-            self.wall_parent.model.vertices = wall_verts
-            self.wall_parent.model.generate()
 
+        # if self.add_collider:
+        #     self.collider = self.model
 
-        if self.add_collider:
-            self.collider = self.model
+        if self.edit_mode:
+            self.add_new_point_renderer.model.vertices = []
+            for i, e in enumerate(self.point_gizmos):
+                self.add_new_point_renderer.model.vertices.append(lerp(self.point_gizmos[i].world_position, self.point_gizmos[i+1].world_position, .5))
+                # self.add_new_point_renderer.model.vertices.append(self.point_gizmos[i].world_position)
+            self.add_new_point_renderer.model.generate()
 
     def __deepcopy__(self, memo):
         return eval(repr(self))
 
 
     @property
     def points(self):
@@ -1878,81 +1938,95 @@
 
     @property
     def edit_mode(self):
         return self._edit_mode
 
     @edit_mode.setter
     def edit_mode(self, value):
+
         print('set edit mode', value)
         self._edit_mode = value
         if value:
             [setattr(e, 'selectable', False) for e in level_editor.entities if not e == self]
             for e in self.point_gizmos:
                 if not e in level_editor.entities:
                     level_editor.entities.append(e)
 
             [setattr(e, 'selectable', True) for e in self.point_gizmos]
             gizmo.subgizmos['y'].enabled = False
             gizmo.fake_gizmo.subgizmos['y'].enabled = False
-
+            self.add_new_point_renderer.enabled = True
+            self.collider = None
         else:
-            print(self.point_gizmos[0] in level_editor.entities)
             [level_editor.entities.remove(e) for e in self.point_gizmos]
             [setattr(e, 'selectable', True) for e in level_editor.entities]
             if True in [e in level_editor.selection for e in self.point_gizmos]: # if point is selected when exiting edit mode, select the poke shape
                 level_editor.selection = [self, ]
 
             gizmo.subgizmos['y'].enabled = True
             gizmo.fake_gizmo.subgizmos['y'].enabled = True
-
+            self.add_new_point_renderer.enabled = False
+            self.collider = 'mesh'
         level_editor.render_selection()
 
 
     def update(self):
         if self.edit_mode:
             if mouse.left or held_keys['d']:
                 level_editor.render_selection()
                 self.generate()
 
 
     def input(self, key):
         if key == 'tab':
+            if not level_editor.selection:
+                self.edit_mode = False
+
             if self in level_editor.selection or True in [e in level_editor.selection for e in self.point_gizmos]:
                 self.edit_mode = not self.edit_mode
 
-        # elif key == 'left mouse down' and self.edit_mode and selector.get_hovered_entity():
-        #     level_editor.selection.clear()
-        #     selection_box.enabled = False
-        #     quick_grabber.input('d')
-        #
-        # elif key == 'left mouse up' and self.edit_mode:
-        #     quick_grabber.input('d up')
-        #     selection_box.enabled = True
+        if self.edit_mode and (key == 'left mouse down' or key == 'd'):
+            if selector.get_hovered_entity():
+                return
+            points_in_range = [(distance_2d(world_position_to_screen_position(v), mouse.position), v) for v in self.add_new_point_renderer.model.vertices]
+            points_in_range = [e for e in points_in_range if e[0] < .075/2]
+            points_in_range.sort()
 
-        elif key == '+' and len(level_editor.selection) == 1 and level_editor.selection[0] in self.point_gizmos:
+            closest_point = None
+            if not points_in_range:
+                return
+
+            closest_point = points_in_range[0][1]
             print('add point')
-            i = self.point_gizmos.index(level_editor.selection[0])
+            # i = self.point_gizmos.index(level_editor.selection[0])
+            i = self.add_new_point_renderer.model.vertices.index(closest_point)
 
             new_point = Entity(parent=self, original_parent=self, position=lerp(self.point_gizmos[i].position, self.point_gizmos[i+1].position, .5), selectable=True, is_gizmo=True)
             level_editor.entities.append(new_point)
             self.point_gizmos.insert(i+1, new_point)
             level_editor.render_selection()
+            if key == 'd':
+                quick_grabber.input('d')
+            #     time.sleep(1/60)
+            #     level_editor.selection = [new_point, ]
+            #     invoke(quick_grabber.input, 'd', delay=1/60)
             # self.generate()
 
 
         elif key == 'space':
             self.generate()
 
         elif key == 'double click' and level_editor.selection == [self, ] and selector.get_hovered_entity() == self:
             self.edit_mode = not self.edit_mode
 
         elif self.edit_mode and key.endswith(' up'):
             invoke(self.generate, delay=3/60)
 
 
+
 class PipeEditor(Entity):
     def __init__(self, points=[Vec3(0,0,0), Vec3(0,1,0)], **kwargs):
         super().__init__(original_parent=level_editor, selectable=True, name='Pipe', **kwargs)
         level_editor.entities.append(self)
         self.point_gizmos = LoopingList([Entity(parent=self, original_parent=self, position=e, selectable=False, name='PipeEditor_point', is_gizmo=True) for e in points])
         self.model = Pipe()
         self.edit_mode = False
@@ -2035,30 +2109,31 @@
 
         elif self.edit_mode and key.endswith(' up'):
             invoke(self.generate, delay=3/60)
 
 
 class SunHandler(Entity):
     def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+        super().__init__(parent=level_editor, **kwargs)
         self.sun = DirectionalLight(parent=level_editor, shadow_map_resolution=(2048,2048))
         self.sun.look_at(Vec3(-2,-1,-1))
 
     def input(self, key):
         if key == 'l':
             print('toggle sun')
             # self.sun.enabled = not self.sun.enabled
-            for e in level_editor.entities:
-                # e.shader = unlit_shader
-                e.unlit = not e.unlit
+            self.sun.update_bounds()
+            # for e in level_editor.entities:
+            #     # e.shader = unlit_shader
+            #     e.unlit = not e.unlit
 
 from ursina.prefabs.radial_menu import RadialMenu
 class RightClickMenu(Entity):
     def __init__(self):
-        super().__init__()
+        super().__init__(parent=level_editor.ui)
         self.radial_menu = RadialMenu(
             parent=level_editor.ui,
             buttons = (
                 Button(highlight_color=color.azure, text='Model', on_click=Func(setattr, menu_handler, 'state', 'model_menu')),
                 Button(highlight_color=color.azure, text='Tex', on_click=Func(setattr, menu_handler, 'state', 'texture_menu')),
                 Button(highlight_color=color.azure, text='Col', on_click=Func(setattr, menu_handler, 'state', 'color_menu')),
                 Button(highlight_color=color.azure, text='Sh', on_click=Func(setattr, menu_handler, 'state', 'shader_menu')),
@@ -2077,15 +2152,15 @@
             if level_editor.selection and sum(abs(e) for e in mouse.position-self.start_click_pos) < .005 and selector.get_hovered_entity() in level_editor.selection:
                 self.radial_menu.enabled = True
 
 
 
 class Search(Entity):
     def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+        super().__init__(parent=level_editor.ui, **kwargs)
 
         self.input_field = InputField(parent=level_editor.ui, enabled=False)
 
 
     def input(self, key):
         if key == 'space' and level_editor.selection:
             self.input_field.enabled = True
@@ -2093,62 +2168,69 @@
 
         # elif len(key) == 1:
         #     print('---', self.input_field.text)
 
 
 if __name__ == '__main__':
     # app = Ursina(size=(1280,720))
-    app = Ursina(vsync=False, forced_aspect_ratio=16/9)
+    app = Ursina(vsync=False)
 
 # camera.fov = 90
 level_editor = LevelEditor()
 
 
 # AmbientLight(color=color._16)
-sun_handler = SunHandler(parent=level_editor)
+sun_handler = SunHandler()
 
 for x in range(8):
     for y in range(8):
         level_editor.scenes[x][y].undo = Undo()
 
 gizmo = Gizmo()
 level_editor.gizmo = gizmo
 t = perf_counter()
 rotation_gizmo = RotationGizmo()
 
 print('-----', perf_counter() - t)
 
 scale_gizmo = ScaleGizmo()
 box_gizmo = BoxGizmo()
-gizmo_toggler = GizmoToggler(parent=level_editor)
+gizmo_toggler = GizmoToggler()
 
-quick_grabber = QuickGrabber(parent=level_editor)   # requires gizmo, selector
+quick_grabber = QuickGrabber()   # requires gizmo, selector
 QuickScale()    # requires scale_gizmo, gizmo_toggler, selector
 QuickRotator()
 RotateRelativeToView(target_entity=None)
-selector = Selector(parent=level_editor)
-selection_box = SelectionBox(parent=level_editor.ui, model=Quad(0, mode='line'), origin=(-.5,-.5,0), scale=(0,0,1), color=color.white33, mode='new')
-spawner = Spawner()
-deleter = Deleter(parent=level_editor)
+selector = Selector()
+selection_box = SelectionBox(model=Quad(0, mode='line'), origin=(-.5,-.5,0), scale=(0,0,1), color=color.white33, mode='new')
+
+prefabs = [Cube, Pyramid, PokeShape]
+level_editor.spawner = Spawner()
+deleter = Deleter()
 level_menu = LevelMenu()
-goto_scene = level_menu.goto_scene
+level_editor.goto_scene = level_menu.goto_scene
 duplicator = Duplicator()
 
 model_menu = ModelMenu()
 texture_menu = TextureMenu()
 color_menu = ColorMenu()
 shader_menu = ShaderMenu()
 menu_handler = MenuHandler()
 right_click_menu = RightClickMenu()
 hierarchy_list = HierarchyList()
 inspector = Inspector()
 PointOfViewSelector()
 Help()
+
+
 # search = Search(parent=level_editor)
 
+# import ursina
+# ursina.editor.prefabs.poke_shape.level_editor = level_editor
+# ursina.editor.prefabs.poke_shape.quick_grabber = quick_grabber
 
 debug_text = Text(y=-.45)
 
 # def update():
 #     if level_editor.selection:
 #         print(get_major_axis_relative_to_view(level_editor.selection[-1]))
 
@@ -2196,23 +2278,25 @@
 #         super().__init__()
 #
 #
 #
 #     for key, value in kwargs.items():
 #         setattr(self, key, value)
 
-input_handler.bind('a', 'y')
+# input_handler.bind('a', 'y')
 
 if __name__ == '__main__':
-    goto_scene(0,0)
+    level_editor.goto_scene(0,0)
     level_editor.selection = [level_editor.entities[0], ]
     # middle = Entity(parent=camera.ui, model='quad', scale_x=.001, color=color.azure)
     # middle = Entity(parent=camera.ui, model='quad', scale_y=.001, color=color.azure)
     # color_menu.open()
     # from poke_shape import PokeShape
     # poke_shape = PokeShape(scale=4, points=[Vec3(-.5,0,-.5), Vec3(.5,0,-.5), Vec3(.5,0,-.25), Vec3(.75,0,-.25), Vec3(.75,0,.25), Vec3(.5,0,.25), Vec3(.5,0,.5), Vec3(-.5,0,.5)])
     # poke_shape = PokeShape(scale=4, points=[Vec3(-.5,0,-.5), Vec3(.5,0,-.5), Vec3(.5,0,-.25), Vec3(.75,0,-.25), Vec3(.75,0,.25), Vec3(.5,0,.25), Vec3(.5,0,.5), Vec3(.5,0,.55), Vec3(-.5,0,.5)])
     # level_editor.entities.append(poke_shape)
     # pipe = PipeEditor()
     # level_editor.entities.append(pipe)
+    # from ursina.shaders import ssao_shader
+    # camera.shader = ssao_shader
     Sky()
     app.run()
```

### Comparing `ursina-5.2.0/ursina/editor/scenes/test2[1,0].py` & `ursina-5.3.0/ursina/editor/scenes/test2[1,0].py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/editor/scenes/untitled_scene[0,0].py` & `ursina-5.3.0/ursina/editor/scenes/untitled_scene[0,0].py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/editor/scenes/untitled_scene[2,0].py` & `ursina-5.3.0/ursina/editor/scenes/untitled_scene[2,0].py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/editor/scenes/untitled_scene[2,3].py` & `ursina-5.3.0/ursina/editor/scenes/untitled_scene[2,3].py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/entity.py` & `ursina-5.3.0/ursina/entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,33 +48,35 @@
     default_shader = None
     default_values = {
         # 'parent':scene,
         'name':'entity', 'enabled':True, 'eternal':False, 'position':Vec3(0,0,0), 'rotation':Vec3(0,0,0), 'scale':Vec3(1,1,1), 'model':None, 'origin':Vec3(0,0,0),
         'shader':None, 'texture':None, 'color':color.white, 'collider':None}
 
     def __init__(self, add_to_scene_entities=True, **kwargs):
+        self._children = []
         super().__init__(self.__class__.__name__)
 
-        self.name = camel_to_snake(self.type)
+        self.name = camel_to_snake(self.__class__.__name__)
         self.enabled = True     # disabled entities will not be visible nor run code.
         self.visible = True
         self.ignore = False     # if True, will not try to run code.
         self.eternal = False    # eternal entities does not get destroyed on scene.clear()
         self.ignore_paused = False      # if True, will still run when application is paused. useful when making a pause menu for example.
         self.ignore_input = False
 
+        self._parent = None
         self.parent = scene     # default parent is scene, which means it's in 3d space. to use UI space, set the parent to camera.ui instead.
         self.add_to_scene_entities = add_to_scene_entities # set to False to be ignored by the engine, but still get rendered.
         if add_to_scene_entities:
             scene.entities.append(self)
 
         self.model = None       # set model with model='model_name' (without file type extension)
         self.color = color.white
         self.texture = None     # set model with texture='texture_name'. requires a model to be set beforehand.
-        self.render_queue = 0
+        self.render_queue = 0   # for custom sorting in case of conflict. To sort things in 2d, set .z instead of using this.
         self.double_sided = False
         if Entity.default_shader:
             self.shader = Entity.default_shader
 
         self.collision = False  # toggle collision without changing collider.
         self.collider = None    # set to 'box'/'sphere'/'capsule'/'mesh' for auto fitted collider.
         self.scripts = []   # add with add_script(class_instance). will assign an 'entity' variable to the script.
@@ -146,18 +148,18 @@
                 new_value.add_x(value[i])
                 new_value.add_y(value[i+1])
                 new_value.add_z(value[i+2])
 
         return new_value
 
 
-    def enable(self):
+    def enable(self): # same as .enabled = True
         self.enabled = True
 
-    def disable(self):
+    def disable(self): # same as .enabled = False
         self.enabled = False
 
 
     @property
     def enabled(self):
         if not hasattr(self, '_enabled'):
             return True
@@ -189,15 +191,15 @@
 
 
     def __setattr__(self, name, value):
         if name == 'eternal':
             for c in self.children:
                 c.eternal = value
 
-        elif name == 'model':
+        if name == 'model':
             if value is None:
                 if hasattr(self, 'model') and self.model:
                     self.model.removeNode()
                     # print('removed model')
                 object.__setattr__(self, name, value)
                 return None
 
@@ -263,14 +265,15 @@
         elif name == 'render_queue':
             if self.model:
                 self.model.setBin('fixed', value)
 
         elif name == 'double_sided':
             self.setTwoSided(value)
 
+
         elif hasattr(self, '_shader') and self.shader and name in self._shader.default_input:
             # print('set shader input:', name, value)
             object.__setattr__(self, name, value)
             self.set_shader_input(name, value)
 
 
         try:
@@ -278,42 +281,43 @@
         except:
             pass
             # print('failed to set attribute:', name)
 
 
     @property
     def parent(self):
-        try:
-            return self._parent
-        except:
-            return None
+        return self._parent
 
     @parent.setter
     def parent(self, value):
+        if hasattr(self, '_parent') and self._parent and hasattr(self._parent, '_children') and self in self._parent._children:
+            self._parent._children.remove(self)
+
+        if hasattr(value, '_children') and not self in value._children:
+            value._children.append(self)
+
+        self.reparent_to(value)
         self._parent = value
-        if value is None:
-            destroy(self)
-        else:
-            try:
-                self.reparentTo(value)
-            except:
-                raise ValueError(f'invalid parent: value')
+
 
     @property
     def world_parent(self):
-        return self.parent
+        return self._parent
 
     @world_parent.setter
     def world_parent(self, value):  # change the parent, but keep position, rotation and scale
-        self.reparent_to(value)
+        if hasattr(self, '_parent') and self._parent and hasattr(self._parent, '_children') and self in self._parent._children:
+            self._parent._children.remove(self)
 
+        if hasattr(value, '_children') and not self in value._children:
+            value._children.append(self)
+
+        self.wrtReparentTo(value)
+        self._parent = value
 
-    @property
-    def type(self): # get class name.
-        return self.__class__.__name__
 
     @property
     def types(self): # get all class names including those this inhertits from.
         from inspect import getmro
         return [c.__name__ for c in getmro(self.__class__)]
 
 
@@ -430,44 +434,44 @@
         return self.origin[2]
     @origin_z.setter
     def origin_z(self, value):
         self.origin = (self.origin_x, self.origin_y, value)
 
     @property
     def world_position(self):
-        return Vec3(self.get_position(render))
+        return Vec3(self.get_position(scene))
 
     @world_position.setter
     def world_position(self, value):
         if not isinstance(value, (Vec2, Vec3)):
             value = self._list_to_vec(value)
         if isinstance(value, Vec2):
             value = Vec3(*value, self.z)
 
-        self.setPos(render, Vec3(value[0], value[1], value[2]))
+        self.setPos(scene, Vec3(value[0], value[1], value[2]))
 
     @property
     def world_x(self):
-        return self.getX(render)
+        return self.getX(scene)
     @property
     def world_y(self):
-        return self.getY(render)
+        return self.getY(scene)
     @property
     def world_z(self):
-        return self.getZ(render)
+        return self.getZ(scene)
 
     @world_x.setter
     def world_x(self, value):
-        self.setX(render, value)
+        self.setX(scene, value)
     @world_y.setter
     def world_y(self, value):
-        self.setY(render, value)
+        self.setY(scene, value)
     @world_z.setter
     def world_z(self, value):
-        self.setZ(render, value)
+        self.setZ(scene, value)
 
     @property
     def position(self):
         return Vec3(*self.getPos())
 
     @position.setter
     def position(self, value):
@@ -582,42 +586,42 @@
         return self.get_quat()
     @quaternion.setter
     def quaternion(self, value):
         self.set_quat(value)
 
     @property
     def world_scale(self):
-        return Vec3(*self.getScale(base.render))
+        return Vec3(*self.getScale(scene))
     @world_scale.setter
     def world_scale(self, value):
         if isinstance(value, (int, float, complex)):
             value = Vec3(value, value, value)
 
-        self.setScale(base.render, value)
+        self.setScale(scene, value)
 
     @property
     def world_scale_x(self):
-        return self.getScale(base.render)[0]
+        return self.getScale(scene)[0]
     @world_scale_x.setter
     def world_scale_x(self, value):
-        self.setScale(base.render, Vec3(value, self.world_scale_y, self.world_scale_z))
+        self.setScale(scene, Vec3(value, self.world_scale_y, self.world_scale_z))
 
     @property
     def world_scale_y(self):
-        return self.getScale(base.render)[1]
+        return self.getScale(scene)[1]
     @world_scale_y.setter
     def world_scale_y(self, value):
-        self.setScale(base.render, Vec3(self.world_scale_x, value, self.world_scale_z))
+        self.setScale(scene, Vec3(self.world_scale_x, value, self.world_scale_z))
 
     @property
     def world_scale_z(self):
-        return self.getScale(base.render)[2]
+        return self.getScale(scene)[2]
     @world_scale_z.setter
     def world_scale_z(self, value):
-        self.setScale(base.render, Vec3(self.world_scale_x, self.world_scale_y, value))
+        self.setScale(scene, Vec3(self.world_scale_x, self.world_scale_y, value))
 
     @property
     def scale(self):
         scale = self.getScale()
         return Vec3(scale[0], scale[1], scale[2])
 
     @scale.setter
@@ -664,27 +668,27 @@
     @world_transform.setter
     def world_transform(self, value):
         self.world_position, self.world_rotation, self.world_scale = value
 
 
     @property
     def forward(self): # get forward direction.
-        return Vec3(*render.getRelativeVector(self, (0, 0, 1)))
+        return Vec3(*scene.getRelativeVector(self, (0, 0, 1)))
     @property
     def back(self): # get backwards direction.
         return -self.forward
     @property
     def right(self): # get right direction.
-        return Vec3(*render.getRelativeVector(self, (1, 0, 0)))
+        return Vec3(*scene.getRelativeVector(self, (1, 0, 0)))
     @property
     def left(self): # get left direction.
         return -self.right
     @property
     def up(self): # get up direction.
-        return Vec3(*render.getRelativeVector(self, (0, 1, 0)))
+        return Vec3(*scene.getRelativeVector(self, (0, 1, 0)))
     @property
     def down(self): # get down direction.
         return -self.up
 
     @property
     def screen_position(self): # get screen position(ui space) from world space.
         from ursina import camera
@@ -787,15 +791,15 @@
 
     @property
     def texture_scale(self):
         if not hasattr(self, '_texture_scale'):
             return Vec2(1,1)
         return self._texture_scale
     @texture_scale.setter
-    def texture_scale(self, value):
+    def texture_scale(self, value):  # how many times the texture should repeat, eg. texture_scale=(8,8).
         self._texture_scale = value
         if self.model and self.texture:
             self.model.setTexScale(TextureStage.getDefault(), value[0], value[1])
             self.set_shader_input('texture_scale', value)
 
     @property
     def texture_offset(self):
@@ -866,14 +870,23 @@
 
     @billboard.setter
     def billboard(self, value):
         self._billboard = value
         if value:
             self.setBillboardPointEye(value)
 
+    @property
+    def wireframe(self):
+        return self._wireframe
+
+    @wireframe.setter
+    def wireframe(self, value):
+        self._wireframe = value
+        self.setRenderModeWireframe(value)
+
 
     def generate_sphere_map(self, size=512, name=f'sphere_map_{len(scene.entities)}'):
         from ursina import camera
         _name = 'textures/' + name + '.jpg'
         org_pos = camera.position
         camera.position = self.position
         base.saveSphereMap(_name, size=size)
@@ -918,26 +931,19 @@
 
     @property
     def bounds(self):
         _bounds = self.model_bounds
         return Bounds(start=_bounds.start*self.scale, end=_bounds.end*self.scale, center=_bounds.center, size=_bounds.size*self.scale)
 
 
-    def reparent_to(self, entity):
-        if entity is not None:
-            self.wrtReparentTo(entity)
-
-        self._parent = entity
-
-
-    def get_position(self, relative_to=scene):
+    def get_position(self, relative_to=scene):  # get position relative to on other Entity. In most cases, use .position instead.
         return self.getPos(relative_to)
 
 
-    def set_position(self, value, relative_to=scene):
+    def set_position(self, value, relative_to=scene): # set position relative to on other Entity. In most cases, use .position instead.
         self.setPos(relative_to, Vec3(value[0], value[1], value[2]))
 
 
     def rotate(self, value, relative_to=None):  # rotate around local axis.
         if not relative_to:
             relative_to = self
 
@@ -969,22 +975,26 @@
         self._flipped_faces = value
         if value:
             self.setAttrib(CullFaceAttrib.make(CullFaceAttrib.MCullClockwise))
         else:
             self.setAttrib(CullFaceAttrib.make(CullFaceAttrib.MCullCounterClockwise))
 
 
-    def look_at(self, target, axis='forward'):
+    def look_at(self, target, axis='forward', up=None): # up defaults to self.up
         from panda3d.core import Quat
         if isinstance(target, Entity):
             target = Vec3(*target.world_position)
         elif not isinstance(target, Vec3):
             target = Vec3(*target)
 
-        self.lookAt(target, Vec3(0,0,1))
+        up_axis = self.up
+        if up:
+            up_axis = up
+        self.lookAt(target, up_axis)
+
         if axis == 'forward':
             return
 
         rotation_offset = {
             'back'    : Quat(0,0,1,0),
             'down'    : Quat(-.707,.707,0,0),
             'up'      : Quat(-.707,-.707,0,0),
@@ -1040,27 +1050,33 @@
                     p = p.parent
 
         return False
 
 
     @property
     def children(self):
-        return [e for e in scene.entities if e.parent == self]
+        return [e for e in self._children if e]     # make sure list doesn't contain destroyed entities
+
+    @children.setter
+    def children(self, value):
+        self._children = value
 
 
     @property
     def attributes(self): # attribute names. used by duplicate().
         return ('name', 'enabled', 'eternal', 'visible', 'parent',
             'origin', 'position', 'rotation', 'scale',
             'model', 'color', 'texture', 'texture_scale', 'texture_offset',
             'render_queue', 'always_on_top', 'collider', 'collision', 'scripts')
 
     def __str__(self):
-        return self.name
-
+        try:
+            return self.name
+        except:
+            return '*destroyed entity*'
 
     def get_changes(self, target_class=None): # returns a dict of all the changes
         if not target_class:
             target_class = self.__class__
 
         changes = dict()
         for key, value in target_class.default_values.items():
@@ -1257,29 +1273,29 @@
             self.hit = HitInfo(hit=False, distance=0)
             return self.hit
 
         collision = self.entries[0]
         nP = collision.get_into_node_path().parent
         point = collision.get_surface_point(nP)
         point = Vec3(*point)
-        world_point = collision.get_surface_point(render)
+        world_point = collision.get_surface_point(scene)
         world_point = Vec3(*world_point)
         hit_dist = distance(self.world_position, world_point)
 
         self.hit = HitInfo(hit=True)
         self.hit.entity = next(e for e in scene.entities if e == nP)
 
         self.hit.point = point
         self.hit.world_point = world_point
         self.hit.distance = hit_dist
 
         normal = collision.get_surface_normal(collision.get_into_node_path().parent).normalized()
         self.hit.normal = Vec3(*normal)
 
-        normal = collision.get_surface_normal(render).normalized()
+        normal = collision.get_surface_normal(scene).normalized()
         self.hit.world_normal = Vec3(*normal)
 
         self.hit.entities = []
         for collision in self.entries:
             self.hit.entities.append(next(e for e in scene.entities if e == collision.get_into_node_path().parent))
 
         return self.hit
@@ -1315,14 +1331,17 @@
 
     player = Player(x=-1)
 
 
     # test
     e = Entity(model='cube', collider='box', texture='shore', color=hsv(.3,1,.5))
     print(repr(e))
+    # a = Entity()
+    # b = Entity(parent=a)
+
 
     # e.animate_x(3, duration=2, delay=.5, loop=True)
     # e.animate_position(Vec3(1,1,1), duration=1, loop=True)
     # e.animate_rotation(Vec3(45,45,45))
     # e.animate_scale(2, duration=1, curve=curve.out_expo_boomerang, loop=True)
     # e.animate_color(color.green, loop=True)
     # e.shake()
```

### Comparing `ursina-5.2.0/ursina/fonts/Bitstream Vera License.txt` & `ursina-5.3.0/ursina/fonts/Bitstream Vera License.txt`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/fonts/LICENSE.txt` & `ursina-5.3.0/ursina/fonts/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/fonts/OpenSans-Regular.ttf` & `ursina-5.3.0/ursina/fonts/OpenSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/fonts/VeraMono.ttf` & `ursina-5.3.0/ursina/fonts/VeraMono.ttf`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/gamepad.py` & `ursina-5.3.0/ursina/gamepad.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/hit_info.py` & `ursina-5.3.0/ursina/hit_info.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/input_handler.py` & `ursina-5.3.0/ursina/input_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
 def input(key):
     if key.endswith('hold') or key == Keys.scroll_down or key == Keys.scroll_up:
         return
 
     key = key.replace('mouse down', 'mouse')
 
-    if key.endswith('up') and key != 'page up':
+    if key.endswith(' up') and key != 'page up':
         held_keys[key[:-3]] = 0
     else:
         held_keys[key] = 1
 
 
 
 if __name__ == '__main__':
```

### Comparing `ursina-5.2.0/ursina/lights.py` & `ursina-5.3.0/ursina/lights.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/main.py` & `ursina-5.3.0/ursina/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,51 +14,85 @@
 from ursina.string_utilities import print_info
 
 
 import __main__
 time.dt = 0
 keyboard_keys = '1234567890qwertyuiopasdfghjklzxcvbnm'
 
+def singleton(cls, **kwargs):
+    instances = {}
+    def getinstance(**kwargs):
+        if cls not in instances:
+            instances[cls] = cls(**kwargs)
+        return instances[cls]
+    return getinstance
 
+@singleton
 class Ursina(ShowBase):
-    def __init__(self, **kwargs): # optional arguments: title, fullscreen, size, forced_aspect_ratio, position, vsync, borderless, show_ursina_splash, render_mode, development_mode, editor_ui_enabled.
-        for name in ('size', 'vsync', 'forced_aspect_ratio'):
+    def __init__(self, **kwargs): # optional arguments: title, fullscreen, size, forced_aspect_ratio, position, vsync, borderless, show_ursina_splash, render_mode, development_mode, editor_ui_enabled, window_type='onscreen'/'offscreen'/'none'.
+        """The main class of Ursina. This class is a singleton, so you can only have one instance of it.
+
+        Keyword Args (optional):
+            title (str): The title of the window.\n
+            fullscreen (bool): Whether the window should be fullscreen or not.\n
+            size (tuple(int, int)): The size of the window.\n
+            forced_aspect_ratio (bool): Whether the window should have a forced aspect ratio or not.\n
+            position (tuple(int, int)): The position of the window.\n
+            vsync (bool): Whether the window should have vsync enabled or not.\n
+            borderless (bool): Whether the window should be borderless or not.\n
+            show_ursina_splash (bool): Whether the Ursina splash should be shown or not.\n
+            render_mode (str): The render mode of the window.\n
+            development_mode (bool): Whether the development mode should be enabled or not.\n
+            editor_ui_enabled (bool): Whether the editor UI should be enabled or not.\n
+            window_type (str): The type of the window. Can be 'onscreen', 'offscreen' or 'none'.\n
+        """
+        for name in ('title', 'size', 'vsync', 'forced_aspect_ratio'):
             if name in kwargs and hasattr(window, name):
                 setattr(window, name, kwargs[name])
 
         if 'development_mode' in kwargs:
             application.development_mode = kwargs['development_mode']
 
+        application.window_type = 'onscreen'
+        if 'window_type' in kwargs:
+            application.window_type = kwargs['window_type']
+        # application.window_type = window_type
+
         application.base = self
-        super().__init__()
+        super().__init__(windowType=application.window_type)
 
         try:
             import gltf
             gltf.patch_loader(self.loader)
         except:
             pass
 
+        if 'gltf_no_srgb' in kwargs:
+            application.gltf_no_srgb = kwargs['gltf_no_srgb']
+
         window.late_init()
-        for name in ('title', 'fullscreen', 'position', 'show_ursina_splash', 'borderless', 'render_mode'):
+        for name in ('fullscreen', 'position', 'show_ursina_splash', 'borderless', 'render_mode'):
             if name in kwargs and hasattr(window, name):
                 setattr(window, name, kwargs[name])
 
         # camera
-        camera._cam = self.camera
-        camera._cam.reparent_to(camera)
-        camera.render = self.render
-        camera.position = (0, 0, -20)
-        scene.camera = camera
-        camera.set_up()
+        if application.window_type != 'none':
+            camera._cam = self.camera
+            camera._cam.reparent_to(camera)
+            camera.render = self.render
+            camera.position = (0, 0, -20)
+            scene.camera = camera
+            camera.set_up()
 
         # input
-        self.buttonThrowers[0].node().setButtonDownEvent('buttonDown')
-        self.buttonThrowers[0].node().setButtonUpEvent('buttonUp')
-        self.buttonThrowers[0].node().setButtonRepeatEvent('buttonHold')
-        self.buttonThrowers[0].node().setKeystrokeEvent('keystroke')
+        if application.window_type == 'onscreen':
+            self.buttonThrowers[0].node().setButtonDownEvent('buttonDown')
+            self.buttonThrowers[0].node().setButtonUpEvent('buttonUp')
+            self.buttonThrowers[0].node().setButtonRepeatEvent('buttonHold')
+            self.buttonThrowers[0].node().setKeystrokeEvent('keystroke')
         self._input_name_changes = {
             'mouse1' : 'left mouse down', 'mouse1 up' : 'left mouse up', 'mouse2' : 'middle mouse down', 'mouse2 up' : 'middle mouse up', 'mouse3' : 'right mouse down', 'mouse3 up' : 'right mouse up',
             'wheel_up' : 'scroll up', 'wheel_down' : 'scroll down',
             'arrow_left' : 'left arrow', 'arrow_left up' : 'left arrow up', 'arrow_up' : 'up arrow', 'arrow_up up' : 'up arrow up', 'arrow_down' : 'down arrow', 'arrow_down up' : 'down arrow up', 'arrow_right' : 'right arrow', 'arrow_right up' : 'right arrow up',
             'lcontrol' : 'left control', 'rcontrol' : 'right control', 'lshift' : 'left shift', 'rshift' : 'right shift', 'lalt' : 'left alt', 'ralt' : 'right alt',
             'lcontrol up' : 'left control up', 'rcontrol up' : 'right control up', 'lshift up' : 'left shift up', 'rshift up' : 'right shift up', 'lalt up' : 'left alt up', 'ralt up' : 'right alt up',
             'control-mouse1' : 'left mouse down', 'control-mouse2' : 'middle mouse down', 'control-mouse3' : 'right mouse down',
@@ -86,29 +120,31 @@
         scene.set_up()
         self._update_task = taskMgr.add(self._update, "update")
 
         # try to load settings that need to be applied before entity creation
         application.load_settings()
 
         from ursina.prefabs.hot_reloader import HotReloader
-        # make sure it's running from a file and not an interactive session.
-        application.hot_reloader = HotReloader(__main__.__file__ if hasattr(__main__, '__file__') else 'None')
+        application.hot_reloader = HotReloader(__main__.__file__ if hasattr(__main__, '__file__') else 'None', enabled=application.development_mode)  # make sure it's running from a file and not an interactive session.
 
         try:
             from ursina import gamepad
         except e as Exception:
             print(e)
 
-        window.make_editor_gui()
+        if application.window_type != 'none':
+            window.make_editor_gui()
         if 'editor_ui_enabled' in kwargs:
             window.editor_ui.enabled = kwargs['editor_ui_enabled']
 
 
     def _update(self, task):
-        time.dt = globalClock.getDt() * application.time_scale          # time between frames
+        """Internal task that runs every frame. Updates time, mouse, sequences and entities."""
+        if application.calculate_dt:
+            time.dt = globalClock.getDt() * application.time_scale          # time between frames
         mouse.update()
 
         if hasattr(__main__, 'update') and __main__.update and not application.paused:
             __main__.update()
 
         for seq in application.sequences:
             seq.update()
@@ -151,14 +187,20 @@
             key = self._input_name_changes[key]
 
         key += ' hold'
         self.input(key)
 
 
     def input(self, key, is_raw=False):
+        """Built-in input handler. Propagates the input to all entities and the input function of the main script. MAin use case for this it to simulate input though code, like: app.input('a').
+
+        Args:
+            key (Any): The input key.
+            is_raw (bool, optional): Whether or not the input should be treated as "raw". Defaults to False.
+        """
         if not is_raw and key in keyboard_keys:
             return
 
         if not 'mouse' in key:
             for prefix in ('control-', 'shift-', 'alt-'):
                 if key.startswith(prefix):
                     key = key.replace('control-', '')
@@ -182,20 +224,22 @@
         for entity in scene.entities:
             if entity.enabled == False or entity.ignore or entity.ignore_input:
                 continue
             if application.paused and entity.ignore_paused == False:
                 continue
 
             if hasattr(entity, 'input') and callable(entity.input):
-                entity.input(key)
+                if entity.input(key):
+                    break
 
             if hasattr(entity, 'scripts'):
                 for script in entity.scripts:
                     if script.enabled and hasattr(script, 'input') and callable(script.input):
-                        script.input(key)
+                        if script.input(key):
+                            break
 
 
         mouse.input(key)
 
 
     def text_input(self, key):
         key_code = ord(key)
@@ -229,15 +273,14 @@
 
     def run(self, info=True):
         if window.show_ursina_splash:
             from ursina.prefabs import ursina_splash
 
         application.load_settings()
         if info:
-            print('screen resolution:', window.screen_resolution)
             print('os:', platform.system())
             print('development mode:', application.development_mode)
             print('application successfully started')
 
         super().run()
```

### Comparing `ursina-5.2.0/ursina/mesh.py` & `ursina-5.3.0/ursina/mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from panda3d.core import MeshDrawer, NodePath
 from panda3d.core import GeomVertexData, GeomVertexFormat, Geom, GeomVertexWriter, GeomNode
 from panda3d.core import GeomTriangles, GeomTristrips, GeomTrifans
 from panda3d.core import GeomLines, GeomLinestrips, GeomPoints
 from panda3d.core import TexGenAttrib, TextureStage
+from panda3d.core import LVector4f
 from ursina.vec3 import Vec3
 from ursina.scripts.generate_normals import generate_normals
 from ursina.scripts.project_uvs import project_uvs
 from ursina.scripts.colorize import colorize
 from ursina import color
 from ursina import application
 from textwrap import dedent
@@ -52,15 +53,14 @@
         'ngon' : GeomTrifans,
         'line' : GeomLinestrips,
         'point' : GeomPoints,
         }
 
     def __init__(self, vertices=None, triangles=None, colors=None, uvs=None, normals=None, static=True, mode='triangle', thickness=1, render_points_in_3d=True):
         super().__init__('mesh')
-        self.name = 'mesh'
         self.vertices = vertices
         self.triangles = triangles
         self.colors = colors
         self.uvs = uvs
         self.normals = normals
         self.static = static
         self.mode = mode
@@ -91,15 +91,15 @@
         vertexwriter = GeomVertexWriter(vdata, 'vertex')
         for v in self.vertices:
             vertexwriter.addData3f(*v)
 
         if self.colors:
             colorwriter = GeomVertexWriter(vdata, 'color')
             for c in self.colors:
-                colorwriter.addData4f(c)
+                colorwriter.addData4f(LVector4f(*c))
 
         if self.uvs:
             uvwriter = GeomVertexWriter(vdata, 'texcoord')
             for uv in self.uvs:
                 uvwriter.addData2f(uv[0], uv[1])
 
         if self.normals != None:
```

### Comparing `ursina-5.2.0/ursina/mesh_importer.py` & `ursina-5.3.0/ursina/mesh_importer.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 from pathlib import Path
 from ursina.mesh import Mesh
 from ursina import application
 from panda3d.core import CullFaceAttrib
 from time import perf_counter
 from ursina.string_utilities import print_info, print_warning
 from ursina import color
+import panda3d.core as p3d
+import gltf
 
 imported_meshes = dict()
 blender_scenes = dict()
 
-def load_model(name, path=application.asset_folder, file_types=('.bam', '.ursinamesh', '.obj', '.glb', '.gltf', '.blend'), use_deepcopy=False):
+def load_model(name, path=application.asset_folder, file_types=('.bam', '.ursinamesh', '.obj', '.glb', '.gltf', '.blend'), use_deepcopy=False, gltf_no_srgb=None):
     if not isinstance(name, str):
         raise TypeError(f"Argument save must be of type str, not {type(str)}")
 
     if '.' in name:
         full_name = name
         name = full_name.split('.')[0]
         file_types = ('.' + full_name.split('.',1)[1],)
@@ -37,45 +39,55 @@
         except:
             pass
 
     for filetype in file_types:
         # warning: glob is case-insensitive on windows, so m.path will be all lowercase
         for filename in path.glob(f'**/{name}{filetype}'):
             if filetype == '.bam':
-                print_info('loading bam')
+                # print_info('loading bam')
                 return loader.loadModel(filename)  # type: ignore
 
+            if filetype == '.gltf' or filetype == '.glb':
+                gltf_settings = gltf.GltfSettings()
+                if gltf_no_srgb is None:
+                    gltf_settings.no_srgb = application.gltf_no_srgb
+                else:
+                    gltf_settings.no_srgb = gltf_no_srgb
+                model_root = gltf.load_model(str(filename), gltf_settings=gltf_settings)
+                model_node_path = p3d.NodePath(model_root)
+                return model_node_path
+
             if filetype == '.ursinamesh':
                 try:
                     with open(filename) as f:
                         m = eval(f.read())
                         m.path = filename
                         m.name = name
                         imported_meshes[name] = m
                         return m
                 except:
                     print_warning('invalid ursinamesh file:', filename)
 
 
             if filetype == '.obj':
                 # print('found obj', filename)
-                # m = loader.loadModel(filename)
-                # m.setAttrib(CullFaceAttrib.make(CullFaceAttrib.MCullCounterClockwise))
                 m = obj_to_ursinamesh(path=path, name=name, return_mesh=True)
                 m.path = filename
                 m.name = name
                 imported_meshes[name] = m
+                if not use_deepcopy:
+                    m.save(f'{name}.bam')
+
                 return m
 
             elif filetype == '.blend':
                 print_info('found blend file:', filename)
                 if compress_models(path=path, name=name):
                     # obj_to_ursinamesh(name=name)
-                    return load_model(name, path)
-
+                    return load_model(name, path, use_deepcopy=use_deepcopy)
             else:
                 try:
                     return loader.loadModel(filename)  # type: ignore
                 except:
                     pass
 
     return None
@@ -112,20 +124,20 @@
         # Use "which" command to find blender
         which_process = subprocess.run(('which', 'blender'), stdout=subprocess.PIPE)
         if which_process.returncode == 0:
             blender_exec = which_process.stdout.decode().strip()
             application.blender_paths['default'] = blender_exec
 
 
-def load_blender_scene(name, path=application.asset_folder, load=True, reload=False, skip_hidden=True, models_only=False):
+def load_blender_scene(name, path=application.asset_folder, load=True, reload=False, skip_hidden=True, models_only=False, uvs=True, vertex_colors=True, normals=True, decimals=4):
     scenes_folder = Path(application.asset_folder / 'scenes')
     if not scenes_folder.exists():
         scenes_folder.mkdir()
 
-    out_file_path = scenes_folder / f'{name}.py'
+    out_file_path = scenes_folder / f'{name}.ursina_blender_scene'
     # print('loading:', out_file_path)
     if reload or not out_file_path.exists():
         print_info('reload:')
         t = perf_counter()
         blend_file = tuple(path.glob(f'**/{name}.blend'))
         if not blend_file:
             raise ValueError('no blender file found at:', path / name)
@@ -140,14 +152,18 @@
             blend_file,
             '--background',
             '--python',
             application.internal_scripts_folder / '_blender_scene_to_ursina.py',
             out_file_path,
             '--skip_hidden' if skip_hidden else '',
             '--models_only' if models_only else '',
+            '--uvs' if uvs else '',
+            '--normals' if normals else '',
+            '--vertex_colors' if vertex_colors else '',
+            f'--decimals={decimals}',
         ]
 
         subprocess.run(args)
 
 
     with open(out_file_path) as f:
         file_content = f.read()
@@ -182,14 +198,16 @@
             return application.blender_paths['default']
         except:
             print_info('using default blender version')
             return application.blender_paths['default']
 
 
 def compress_models(path=None, outpath=application.compressed_models_folder, name='*'):
+    if "/" in name or '\\' in name:
+        raise Exception(f'Path character "/" or "\\" found in blender name ({name}). To successfully import .blend files, use only the file name.')
 
     if not application.compressed_models_folder.exists():
         application.compressed_models_folder.mkdir()
 
     export_script_path = application.internal_scripts_folder / '_blend_export.py'
     exported = []
 
@@ -205,23 +223,15 @@
             subprocess.run((blender, blend_file, '--background', '--python', export_script_path, out_file_path))
 
         exported.append(blend_file)
 
     return exported
 
 
-def obj_to_ursinamesh(
-    path=application.compressed_models_folder,
-    outpath=application.compressed_models_folder,
-    name='*',
-    return_mesh=True,
-    save_to_file=False,
-    delete_obj=False
-    ):
-
+def obj_to_ursinamesh(path=application.compressed_models_folder, outpath=application.compressed_models_folder, name='*', return_mesh=True, save_to_file=False, delete_obj=False):
     if name.endswith('.obj'):
         name = name[:-4]
 
     for f in path.glob(f'**/{name}.obj'):
         # filepath = path / (os.path.splitext(f)[0] + '.obj')
         print('read obj at:', f)
```

### Comparing `ursina-5.2.0/ursina/models/procedural/capsule.py` & `ursina-5.3.0/ursina/models/procedural/capsule.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/models/procedural/circle.py` & `ursina-5.3.0/ursina/models/procedural/circle.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ursina import *
 
 
 class Circle(Mesh):
-    def __init__(self, resolution=16, radius=.5, rotate=True, mode='ngon', **kwargs):
+    def __init__(self, resolution=16, radius=.5, mode='ngon', **kwargs):
         origin = Entity()
         point = Entity(parent=origin)
         point.y = radius
 
         self.vertices = list()
         for i in range(resolution):
             origin.rotation_z -= 360 / resolution
```

### Comparing `ursina-5.2.0/ursina/models/procedural/cone.py` & `ursina-5.3.0/ursina/models/procedural/cone.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from ursina import Mesh, Vec3, rotate_point_2d
+from ursina import Mesh, Vec3, rotate_around_point_2d
 
 
 class Cone(Mesh):
     def __init__(self, resolution=4, radius=.5, height=1, add_bottom=True, mode='triangle', **kwargs):
 
         v = Vec3(radius, 0, 0)
         origin = Vec3(0,0,0)
         degrees_to_rotate = 360 / resolution
 
         verts = []
         for i in range(resolution):
             verts.append(Vec3(v[0], 0, v[1]))
-            v = rotate_point_2d(v, origin, -degrees_to_rotate)
+            v = rotate_around_point_2d(v, origin, -degrees_to_rotate)
             verts.append(Vec3(v[0], 0, v[1]))
 
             verts.append(Vec3(0,height,0))
         if add_bottom:
             for i in range(resolution):
                 verts.append(Vec3(v[0], 0, v[1]))
                 verts.append(Vec3(0,0,0))
-                v = rotate_point_2d(v, origin, -degrees_to_rotate)
+                v = rotate_around_point_2d(v, origin, -degrees_to_rotate)
                 verts.append(Vec3(v[0], 0, v[1]))
 
 
         super().__init__(vertices=verts, uvs=[e.xy for e in verts], mode=mode, **kwargs)
 
 
 if __name__ == '__main__':
     from ursina import Ursina, Entity, color, EditorCamera
     app = Ursina()
     e = Entity(model=Cone(3), texture='brick')
 
     # # rotate model
     # for i, v in enumerate(e.model.vertices):
-    #     x, y = rotate_point_2d((v.x, v.y), (0,0), 90)
+    #     x, y = rotate_around_point_2d((v.x, v.y), (0,0), 90)
     #
     #     e.model.vertices[i] = Vec3(x, y, v.z)
     #
     # e.model.generate()
 
     origin = Entity(model='quad', color=color.orange, scale=(.05, .05))
     ed = EditorCamera()
```

### Comparing `ursina-5.2.0/ursina/models/procedural/cube.py` & `ursina-5.3.0/ursina/models/procedural/cube.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/models/procedural/cylinder.py` & `ursina-5.3.0/ursina/models/procedural/cylinder.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/models/procedural/grid.py` & `ursina-5.3.0/ursina/models/procedural/grid.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/models/procedural/pipe.py` & `ursina-5.3.0/ursina/models/procedural/pipe.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,79 +12,83 @@
         self.origin = origin
         self.path = path
         self.thicknesses = thicknesses
         self.look_at = look_at
         self.cap_ends = cap_ends
         self.mode = mode
         self.color_gradient = color_gradient
-        self.b = None
-        self.e = None
-        super().__init__(**kwargs)
+        self.prev = None
+        self.curr = None
+        super().__init__(mode=mode, **kwargs)
 
 
 
     def generate(self):
         shape = self.base_shape.vertices
         # make the base shape and rotate it
-        if not self.b:
-            self.b = Entity(position=self.path[0], scale=self.thicknesses[0], origin=self.origin, enabled=False)
+        if not self.prev:
+            self.prev = Entity(position=self.path[0], scale=self.thicknesses[0], origin=self.origin, enabled=False)
             for p in shape:
-                Entity(parent=self.b, position=Vec3(p), scale=(.05, .05, .05), color=color.yellow, enabled=False)
+                Entity(parent=self.prev, position=Vec3(p), scale=(.05, .05, .05), color=color.yellow, enabled=False)
 
-            self.b.look_at(self.path[1])
-            self.e = duplicate(self.b)
+            self.prev.look_at(self.path[1])
+            self.curr = duplicate(self.prev)
 
         verts = []
         self.colors = []
 
         # cap start
         if self.cap_ends:
-            for i in range(len(self.b.children)):
+            for i in range(len(self.prev.children)):
                 verts.append(self.path[0])
-                verts.append(self.b.children[i].world_position)
-                if i >= len(self.b.children)-1:
-                    verts.append(self.b.children[0].world_position)
+                verts.append(self.prev.children[i].world_position)
+                if i >= len(self.prev.children)-1:
+                    verts.append(self.prev.children[0].world_position)
                 else:
-                    verts.append(self.b.children[i+1].world_position)
+                    verts.append(self.prev.children[i+1].world_position)
 
                 if self.color_gradient:
                     self.colors.extend([self.color_gradient[0], ]*3)
 
         for i in range(1, len(self.path)):
-            self.b.position = self.path[i-1]
+            self.prev.position = self.path[i-1]
+            self.curr.position = self.path[i]
             if self.look_at:
-                self.b.look_at(self.path[i])
-            self.e.position = self.path[i]
-            if i+1 < len(self.path) and self.look_at:
-                self.e.look_at(self.path[i+1])
+                self.prev.look_at(self.path[i])
+
+                if i+1 < len(self.path):
+                    self.curr.look_at(self.path[i+1])
+
+                if i == len(self.path)-1 and self.path[0] == self.path[-1]: # if the first and last point are the same, make the end math the rotation of the start.
+                    self.curr.look_at(self.path[1])
 
             # for debugging sections
             # clone = duplicate(e)
             # clone.color=color.brown
             # clone.scale *= 1.1
 
             try:
-                self.e.scale = self.thicknesses[i]
-                self.b.scale = self.thicknesses[i-1]
+                self.curr.scale = self.thicknesses[i]
+                self.prev.scale = self.thicknesses[i-1]
             except:
                 pass
 
             # add sides
-            for j in range(len(self.e.children)):
+            for j in range(len(self.curr.children)):
                 n = j+1
-                if j == len(self.e.children)-1:
+                if j == len(self.curr.children)-1:
                     n = 0
                 verts.extend([
-                    self.e.children[j].world_position,
-                    self.b.children[n].world_position,
-                    self.b.children[j].world_position,
-
-                    self.e.children[n].world_position,
-                    self.b.children[n].world_position,
-                    self.e.children[j].world_position
+                    self.curr.children[j].world_position,
+                    self.prev.children[n].world_position,
+                    self.prev.children[j].world_position,
+
+                    self.curr.children[n].world_position,
+                    self.prev.children[n].world_position,
+                    self.curr.children[j].world_position
                 ])
 
                 if self.color_gradient:
                     from_color = sample_gradient(self.color_gradient, (i-1)/(len(self.path)-1))
                     to_color = sample_gradient(self.color_gradient, (i-0)/(len(self.path)-1))
                     self.colors.extend([
                         to_color,
@@ -93,20 +97,20 @@
                         to_color,
                         from_color,
                         to_color,
                     ])
 
         # cap end
         if self.cap_ends:
-            for i in range(len(self.e.children)):
-                if i >= len(self.e.children)-1:
-                    verts.append(self.e.children[0].world_position)
+            for i in range(len(self.curr.children)):
+                if i >= len(self.curr.children)-1:
+                    verts.append(self.curr.children[0].world_position)
                 else:
-                    verts.append(self.e.children[i+1].world_position)
-                verts.append(self.e.children[i].world_position)
+                    verts.append(self.curr.children[i+1].world_position)
+                verts.append(self.curr.children[i].world_position)
                 verts.append(self.path[-1])
 
                 if self.color_gradient:
                     self.colors.extend([self.color_gradient[-1], ]*3)
 
         self.vertices = verts
         super().generate()
@@ -114,17 +118,20 @@
         # destroy(e)
 
 
 
 if __name__ == '__main__':
     app = Ursina()
     # e = Entity(model=Prism(mode='line'))
-    path = (Vec3(0,0,0), Vec3(0,1,0), Vec3(0,3,0), Vec3(0,4,0), Vec3(2,5,0))
-    thicknesses = ((1,1), (.5,.5), (.75,.75), (.5,.5), (1,1))
-    e = Entity(model=Pipe(path=path, thicknesses=thicknesses))
+    path = [e*5 for e in Circle().vertices]
+    # path = [e.xzy for e in path]
+
+    path.append(path[0])
+    # thicknesses = ((1,1), (.5,.5), (.75,.75), (.5,.5), (1,1))
+    e = Entity(model=Pipe(path=path, cap_ends=False))
     # print(e.model.colors)
     print(len(e.model.vertices), len(e.model.colors))
     # e.model.colorize()
     # e2 = duplicate(e)
     # e2.x=2
     # e2.color=color.red
```

### Comparing `ursina-5.2.0/ursina/models/procedural/plane.py` & `ursina-5.3.0/ursina/models/procedural/plane.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/models/procedural/quad.py` & `ursina-5.3.0/ursina/models/procedural/quad.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/models/procedural/terrain.py` & `ursina-5.3.0/ursina/models/procedural/terrain.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/models_compressed/arrow.ursinamesh` & `ursina-5.3.0/ursina/models_compressed/arrow.ursinamesh`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/models_compressed/circle.ursinamesh` & `ursina-5.3.0/ursina/models_compressed/circle.ursinamesh`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/models_compressed/cube.ursinamesh` & `ursina-5.3.0/ursina/models_compressed/cube.ursinamesh`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/models_compressed/cube_uv_top.ursinamesh` & `ursina-5.3.0/ursina/models_compressed/cube_uv_top.ursinamesh`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/models_compressed/icosphere.ursinamesh` & `ursina-5.3.0/ursina/models_compressed/icosphere.ursinamesh`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/models_compressed/scale_gizmo.ursinamesh` & `ursina-5.3.0/ursina/models_compressed/scale_gizmo.ursinamesh`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/models_compressed/sky_dome.ursinamesh` & `ursina-5.3.0/ursina/models_compressed/sky_dome.ursinamesh`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/models_compressed/sphere.ursinamesh` & `ursina-5.3.0/ursina/models_compressed/sphere.ursinamesh`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/mouse.py` & `ursina-5.3.0/ursina/mouse.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             window.set_mouse_mode(window.M_relative)
         else:
             window.set_mouse_mode(window.M_absolute)
 
         if not application.base:
             return
 
-        print('return', value)
+        # print('return', value)
         # self.position = Vec3(0,0,0)
         window.set_cursor_hidden(value)
         application.base.win.requestProperties(window)
         self._locked_mouse_last_frame = True
 
 
     @property
@@ -188,14 +188,17 @@
             self.middle = True
         if key == 'middle mouse up':
             self.middle = False
 
 
 
     def update(self):
+        if application.window_type != 'onscreen':
+            return
+
         if not self.enabled or not self._mouse_watcher.has_mouse() or self._locked_mouse_last_frame:
             self.velocity = Vec3(0,0,0)
             self._locked_mouse_last_frame = False
             return
 
         self.moving = self.x + self.y != self.prev_x + self.prev_y
```

### Comparing `ursina-5.2.0/ursina/prefabs/animation.py` & `ursina-5.3.0/ursina/prefabs/animation.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/animator.py` & `ursina-5.3.0/ursina/prefabs/animator.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/button.py` & `ursina-5.3.0/ursina/prefabs/button.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,20 +157,15 @@
         if not self.disabled and self.model:
             self.model.setColorScale(self.highlight_color)
 
             if self.highlight_scale != 1:
                 self.model.setScale(Vec3(self.highlight_scale, self.highlight_scale, 1))
 
         if hasattr(self, 'tooltip'):
-            self.tooltip.scale = (0,0,0)
             self.tooltip.enabled = True
-            if not hasattr(self.tooltip, 'original_scale'):
-                self.tooltip.original_scale = 1
-
-            self.tooltip.animate_scale(self.tooltip.original_scale)
 
 
     def on_mouse_exit(self):
         if not self.disabled and self.model:
             self.model.setColorScale(self.color)
 
             if not mouse.left and self.highlight_scale != 1:
```

### Comparing `ursina-5.2.0/ursina/prefabs/button_group.py` & `ursina-5.3.0/ursina/prefabs/button_group.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/button_list.py` & `ursina-5.3.0/ursina/prefabs/button_list.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/conversation.py` & `ursina-5.3.0/ursina/prefabs/conversation.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/cursor.py` & `ursina-5.3.0/ursina/prefabs/cursor.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/draggable.py` & `ursina-5.3.0/ursina/prefabs/draggable.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/dropdown_menu.py` & `ursina-5.3.0/ursina/prefabs/dropdown_menu.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/editor_camera.py` & `ursina-5.3.0/ursina/prefabs/editor_camera.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/file_browser.py` & `ursina-5.3.0/ursina/prefabs/file_browser.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/file_browser_save.py` & `ursina-5.3.0/ursina/prefabs/file_browser_save.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/first_person_controller.py` & `ursina-5.3.0/ursina/prefabs/first_person_controller.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/frame_animation_3d.py` & `ursina-5.3.0/ursina/prefabs/frame_animation_3d.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/grid_editor.py` & `ursina-5.3.0/ursina/prefabs/grid_editor.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/health_bar.py` & `ursina-5.3.0/ursina/prefabs/health_bar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from ursina import *
 
 
 class HealthBar(Button):
 
     def __init__(self, max_value=100, roundness=.25, animation_duration=.1, show_text=True, show_lines=False, **kwargs):
-        super().__init__(position=(-.45*window.aspect_ratio,.45), origin=(-.5,.5), scale=(Text.size*20,Text.size), color=color.black66, highlight_color=color.black66, text='hp / max hp', ignore=True)
+        super().__init__(position=(-.45*window.aspect_ratio,.45), origin=(-.5,.5), scale=(Text.size*20,Text.size), color=color.black66, highlight_color=color.black66, text='hp / max hp', radius=roundness, ignore=True)
 
-        self.bar = Entity(parent=self, model='quad', origin=self.origin, z=-.01, color=color.red.tint(-.2), ignore=True)
+        self.bar = Entity(parent=self, model=Quad(radius=roundness), origin=self.origin, z=-.01, color=color.red.tint(-.2), ignore=True)
         self.lines = Entity(parent=self.bar, y=-1, color=color.black33, ignore=True, enabled=show_lines, z=-.01)
         self.text_entity.scale *= .7
 
         self.max_value = max_value
         self.clamp = True
         self.roundness = roundness
         self.animation_duration = animation_duration
         self.show_lines = show_lines
         self.show_text = show_text
-        self.scale_x = self.scale_x # update rounded corners
 
         for key, value in kwargs.items():
             setattr(self, key, value)
 
-        self.scale_y = self.scale_y # update background's rounded corners
         self.value = self.max_value
         self.text_entity.enabled = show_text
 
 
     @property
     def value(self):
         return self._value
@@ -74,22 +72,17 @@
         return self.bar.color
     @bar_color.setter
     def bar_color(self, value):
         self.bar.color = value
 
 
     def __setattr__(self, name, value):
-        if 'scale' in name and hasattr(self, 'roundness'):  # update rounded corners of background when scaling
-            orginal_text_position = self.text_entity.position
-            self.model = Quad(radius=self.roundness, aspect=self.world_scale_x / self.world_scale_y)
-            self.origin = self.origin
-            self.text_entity.position = orginal_text_position
-
-        if 'scale' in name and hasattr(self, 'text_entity'):  # make sure the text doesn't scale awkwardly
-            self.text_entity.world_scale_x = self.text_entity.world_scale_y
+        if 'scale' and hasattr(self, 'model') and self.model:  # update rounded corners of background when scaling
+            self.model.aspect = self.world_scale_x / self.world_scale_y
+            self.model.generate()
 
         super().__setattr__(name, value)
 
 
 if __name__ == '__main__':
     app = Ursina()
```

### Comparing `ursina-5.2.0/ursina/prefabs/hot_reloader.py` & `ursina-5.3.0/ursina/prefabs/hot_reloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 
 
     def reload_textures(self):
         textured_entities = [e for e in scene.entities if e.texture]
         reloaded_textures = list()
 
         for e in textured_entities:
-            if e.texture.name in reloaded_textures:
+            if e.texture.name in reloaded_textures or not hasattr(e.texture, 'path') or not e.texture.path:
                 continue
 
             if e.texture.path.parent.name == application.compressed_textures_folder.name:
                 print('texture is made from .psd file', e.texture.path.stem + '.psd')
                 texture_importer.compress_textures(e.texture.path.stem)
             print('reloaded texture:', e.texture.path)
             e.texture._texture.reload()
```

### Comparing `ursina-5.2.0/ursina/prefabs/input_field.py` & `ursina-5.3.0/ursina/prefabs/input_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.hide_content = False   # if set to True, will display content as '*'. can also be set to character instead of True.
 
         self.next_field = None
         self.submit_on = None   # for example: self.submit_on = 'enter' will call self.on_submit when you press enter.
         self.on_submit = None   # function to be called when you press self.submit_on.
         self.on_value_changed = None
 
-        self.text_field = TextField(world_parent = self, x=-.45, y=.3, z=-.1, max_lines=max_lines, character_limit=character_limit, register_mouse_input = True)
+        self.text_field = TextField(world_parent=self, x=-.45, y=.3, z=-.1, max_lines=max_lines, character_limit=character_limit, register_mouse_input=True)
         destroy(self.text_field.bg)
         self.text_field.bg = self
 
         def render():
             if self.limit_content_to:
                 org_length = len(self.text_field.text)
                 self.text_field.text = ''.join([e for e in self.text_field.text if e in self.limit_content_to])
```

### Comparing `ursina-5.2.0/ursina/prefabs/made_with_ursina.py` & `ursina-5.3.0/ursina/prefabs/made_with_ursina.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/memory_counter.py` & `ursina-5.3.0/ursina/prefabs/memory_counter.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/platformer_controller_2d.py` & `ursina-5.3.0/ursina/prefabs/platformer_controller_2d.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/primitives.py` & `ursina-5.3.0/ursina/prefabs/primitives.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/radial_menu.py` & `ursina-5.3.0/ursina/prefabs/radial_menu.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/sky.py` & `ursina-5.3.0/ursina/prefabs/sky.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/slider.py` & `ursina-5.3.0/ursina/prefabs/slider.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/sprite.py` & `ursina-5.3.0/ursina/prefabs/sprite.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/sprite_sheet_animation.py` & `ursina-5.3.0/ursina/prefabs/sprite_sheet_animation.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,21 +30,25 @@
         [anim.pause() for anim in self.animations.values()]
 
         self.animations[animation_name].start()
 
 
 if __name__ == '__main__':
     '''
-    (0,0) is in bottom left
+    Sprite sheet coordinate system:
+    (0,3) (1,3) (2,3) (3,3)
+    (0,2) (1,2) (2,2) (3,2)
+    (0,1) (1,1) (2,1) (3,1)
+    (0,0) (1,0) (2,0) (3,0)
     '''
     from ursina import Ursina
     app = Ursina()
     player_graphics = SpriteSheetAnimation('sprite_sheet', tileset_size=(4,4), fps=6, animations={
-        'idle' : ((0,0), (0,0)),
-        'walk_up' : ((0,0), (3,0)),
+        'idle' : ((0,0), (0,0)),        # makes an animation from (0,0) to (0,0), a single frame
+        'walk_up' : ((0,0), (3,0)),     # makes an animation from (0,0) to (3,0), the bottom row
         'walk_right' : ((0,1), (3,1)),
         'walk_left' : ((0,2), (3,2)),
         'walk_down' : ((0,3), (3,3)),
         }
         )
     def input(key):
         if key == 'w':
```

### Comparing `ursina-5.2.0/ursina/prefabs/text_field.py` & `ursina-5.3.0/ursina/prefabs/text_field.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 from ursina import *
 import pyperclip
 # from tree_view import TreeView
 
 
 class TextField(Entity):
-    def __init__(self, max_lines=9999, line_height=1.1, **kwargs):
+    def __init__(self, max_lines=64, line_height=1.1, **kwargs):
         super().__init__(parent=camera.ui, x=-.5, y=.4, ignore_paused=True)
 
         self.font = 'VeraMono.ttf'
         self.line_height = line_height
         self.max_lines = max_lines
         self.character_limit = None
 
         self.scroll_parent = Entity(parent=self)
         self.text_entity = Text(parent=self.scroll_parent, start_tag='☾', end_tag='☽', font=self.font, text='', line_height=self.line_height, origin=(-.5, .5))
-        self.line_numbers = Text(parent=self.scroll_parent, font=self.font, text='0', origin=(.5,.5), x=-.04, color=color.gray, enabled=False)
+        self.line_numbers = Text(parent=self.scroll_parent, font=self.font, line_height=line_height, text='0', origin=(.5,.5), x=-.04, color=color.gray, enabled=False)
         self.character_width = Text.get_width('a', font=self.font)
         self.cursor_parent = Entity(parent=self.scroll_parent, scale=(self.character_width, -1*Text.size*self.line_height))
         self.cursor = Entity(name='text_field_cursor', parent=self.cursor_parent, model='cube', color=color.cyan, origin=(-.5, -.5), scale=(.1, 1, 0), enabled=False)
         self.cursor.blink(duration=1.2, loop=True)
         self.bg = Entity(name='text_field_bg', parent=self, model='quad', double_sided=True, color=color.dark_gray, origin=(-.5,.5), z=0.005, scale=(120, Text.size*self.max_lines), collider='box', visible=True)
 
         self.selection = [Vec2(0,0), Vec2(0,0)]
         self.selection_parent = Entity(name='text_field_selection_parent', parent=self.cursor_parent, scale=(1,1,0))
         self.register_mouse_input = False
         self.world_space_mouse = False
 
         self.triple_click_delay = 0.3
         self._last_double_click = 0
         self.scroll = 0
+        self.scroll_amount = 2
         self._prev_scroll = self.scroll
 
         self.active = True
         self.highlight_color = color.color(120,1,1,.1)
         self.text = ''
         self.delimiters = ' .,!?;:(){}[]<>\'\"@#$%^&*+=-\\|/`~'
         self.replacements = dict()
@@ -72,51 +73,91 @@
                 'move_to_end_of_word' :     ('ctrl+right arrow', 'ctrl+right arrow hold', 'ctrl+shift+right arrow', 'ctrl+shift+right arrow hold'),
                 'move_to_start_of_word' :   ('ctrl+left arrow', 'ctrl+left arrow hold', 'ctrl+shift+left arrow', 'ctrl+shift+left arrow hold'),
             },
 
             # 'select_word_left': ('ctrl+shift+left arrow', 'ctrl+shift+left arrow hold'),
             # 'select_word_right': ('ctrl+shift+right arrow', 'ctrl+shift+right arrow hold'),
         }
+        def middle_click_input(key):
+            if self.register_mouse_input:
+                if key == 'middle mouse down':
+                    self.middle_click_scroller.start_y = mouse.y
+                    self._original_scroll_amount = self.scroll_amount
+                elif key == 'middle mouse up':
+                    self.middle_click_scroller.start_y = None
+                    self.scroll_amount = self._original_scroll_amount
+
+        def middle_click_update():
+            if not mouse.middle:
+                return
+            self.middle_click_scroller.t += time.dt
+            if self.middle_click_scroller.t < self.middle_click_scroller.update_rate:
+                return
+
+            # self.middle_click_scroller.update_rate = 1-mouse.delta_drag[0]
+            # print('-aaaaaaaaaaa', 1-mouse.delta_drag[0])
+            dist = abs(mouse.y - self.middle_click_scroller.start_y)
+            self.scroll_amount = 1
+            if dist > .1:
+                self.scroll_amount = 4
+            elif dist > .2:
+                self.scroll_amount = 6
+            # elif dist > .4:
+            #     self.scroll_amount = 12
+
+            self.middle_click_scroller.t = 0
+
+            if self.register_mouse_input:
+                if mouse.y < self.middle_click_scroller.start_y:
+                    self.input('scroll down')
+                if mouse.y > self.middle_click_scroller.start_y:
+                    self.input('scroll up')
+
+        self.middle_click_scroller = Entity(parent=self, start_y=None, input=middle_click_input, update=middle_click_update, t=0, update_rate=.05)
 
 
         for key, value in kwargs.items():
             setattr(self, key, value)
 
         self._prev_text = ''
 
 
+
     @property
     def active(self):
         return self._active
 
     @active.setter
     def active(self, value):
         self._active = value
         self.cursor.enabled = value
 
         if not value:
             self.selection = [Vec2(0,0), Vec2(0,0)]
             self.draw_selection()
 
 
-    def add_text(self, s, move_cursor=True):
+    def add_text(self, s, move_cursor=True, rerender=True):
         if self.character_limit and len(self.text) >= self.character_limit:
             return
 
         x, y = int(self.cursor.x), int(self.cursor.y)
 
         lines = self.text.split('\n')
         l = lines[y]
         lines[y] =  l[:x] + s + l[x:]
         self._append_undo(self.text, y, x)
         self.text = '\n'.join(lines)
 
         if move_cursor:
             self.cursor.x += len(s)
 
+        if rerender:
+            self.render()
+
     def _append_undo(self, text, y, x, clear_redo = True):
         if clear_redo:
             self.on_redo.clear()
         self.on_undo.append((text, y, x))
 
 
     def move_line(self, line_index, delta, move_cursor=True):
@@ -136,15 +177,15 @@
 
         middle = lines[start_y:end_y+1]
         del lines[start_y:end_y+1]
         for l in middle[::delta]:
             lines.insert(start_y+delta, l)
         # end = lines[start_y+1:]
 
-        [print(e) for e in middle]
+        # [print(e) for e in middle]
         self.cursor.y += delta * move_cursor
         for e in self.selection:
             e.y += delta
         self.draw_selection()
 
         # if delta == 1:
         #     _ = start.pop()
@@ -153,18 +194,18 @@
         #     _ = end.pop(0)
         #     start.append(_)
         #
         # lines = start + middle + end
         #
         self._append_undo(self.text, y, x)
         self.text = '\n'.join(lines)
-        print('moved line')
+        # print('moved line')
 
 
-    def erase(self):
+    def erase(self, rerender=True):
         # if not self.selection or self.selection[0] == self.selection[1]:
         x, y = int(self.cursor.x), int(self.cursor.y)
         if x+y == 0:
             return
 
         lines = self.text.split('\n')
         l = lines[y]
@@ -211,14 +252,16 @@
             # for y in range(int(self.selection[0][1]), int(self.selection[1][1])):
             #     lines.pop(y)
 
 
 
 
         self.text = '\n'.join(lines)
+        if rerender:
+            self.render()
 
     def _ordered_selection(self):
         if not self.selection:
             return None
         if self.selection[1][1] < self.selection[0][1] or (self.selection[1][1] == self.selection[0][1] and self.selection[1][0] < self.selection[0][0]):
             return [self.selection[1], self.selection[0]]
         return self.selection
@@ -238,14 +281,15 @@
         del lines[(start_y + 1) : (end_y + 1)]
 
         self._append_undo(self.text, self.cursor.y, self.cursor.x)
         self.text = '\n'.join(lines)
         self.selection = [Vec2(0,0), Vec2(0,0)]
         # self._append_undo(self.text, y, x)
         self.draw_selection()
+        self.render()
 
 
     def get_selected(self):
         if not self.selection or self.selection[0] == self.selection[1]:
             return None
 
         sel = self._ordered_selection()
@@ -295,30 +339,45 @@
         return (x, y)
 
 
     def input(self, key):
         # print('-------------', key)
         text, cursor, on_undo, add_text, erase = self.text, self.cursor, self.on_undo, self.add_text, self.erase
 
-        if mouse.hovered_entity == self.bg:
-            if key in self.shortcuts['scroll_down']:
-                self.scroll = clamp(self.scroll+1, 0, self.max_lines)
-                self.render()
-
-            elif key in self.shortcuts['scroll_up']:
-                self.scroll = clamp(self.scroll-1, 0, self.max_lines)
-                self.render()
-
-
         if self.register_mouse_input and key == 'left mouse down':
             self.active = (mouse.hovered_entity == self.bg)
 
         if not self.active:
             return
 
+        if mouse.hovered_entity == self.bg:
+            if key in self.shortcuts['scroll_down']:
+                if self.max_lines < 9999:
+                    if self.scroll < 9999:
+                        self.scroll = clamp(self.scroll+self.scroll_amount, 0, 9999)
+                        self.y = .4-.025
+                        self.animate('y', .4, duration=.045, curve=curve.linear)
+                        self.render()
+                else:
+                    self.scroll = clamp(self.scroll+self.scroll_amount, 0, 9999)
+                    self.scroll_parent.y = (self.scroll * Text.size * self.line_height)
+                return
+
+            elif key in self.shortcuts['scroll_up']:
+                if self.max_lines < 9999:
+                    # if self.scroll > 0:
+                    self.scroll = clamp(self.scroll-self.scroll_amount, 0, 9999)
+                    # self.y = .4-.025
+                    # self.animate('y', .4, duration=.045, curve=curve.linear)
+                    self.render()
+                else:
+                    self.scroll = clamp(self.scroll-self.scroll_amount, 0, 9999)
+                    self.scroll_parent.y = (self.scroll * Text.size * self.line_height)
+                return
+
         if key == 'double click':
             t = time.time()
             if t - self._last_double_click < self.triple_click_delay:
                 key = 'triple click'
             self._last_double_click = t
 
         # key = f'{"ctrl" if held_keys["control"]} + {key}'
@@ -384,49 +443,52 @@
                 break
 
         if moved_cursor and held_keys['shift']:
             self.selection[1] = self.cursor.position
             self.draw_selection()
 
 
-        if key in self.shortcuts['newline'] and self.cursor.y < self.max_lines-1:
+        if key in self.shortcuts['newline'] and (self.cursor.y < self.max_lines-1 or self.max_lines == 9999):
             if self.selection:
                 self.delete_selected()
 
             if l.startswith('class ') and not l.endswith(':'):
-                add_text(':')
+                add_text(':', rerender=False)
             if l.startswith('def ') and not l.endswith(':'):
-                add_text(':')
+                add_text(':', rerender=False)
 
-            add_text('\n')
+            add_text('\n', rerender=False)
 
             if l.strip() == '':
                 indent = len(l)
             else:
                 indent = len(l) - len(l.lstrip())
                 if l.lstrip().startswith('class ') or l.lstrip().startswith('def '):
                     indent += 4
 
             self.cursor.y += 1
             self.cursor.x = 0
             add_text(' '*indent)
+            return
             # self.cursor.x = indent
 
         if key in self.shortcuts['indent']:
             if not self.selection or self.selection[0] == self.selection[1]:
                 add_text(' '*4, move_cursor=True)
+                return
 
             else:
                 for y in range(int(self.selection[0][1]), int(self.selection[1][1])+1):
                     # print('indent', y)
                     lines[y] = (' '*4) + lines[y]
                 self.cursor.x += 4
                 self._append_undo(self.text, y, x)
                 self.text = '\n'.join(lines)
-
+                self.render()
+                return
 
         if key in self.shortcuts['dedent']:
             if not self.selection or self.selection[0] == self.selection[1]:
                 if l.startswith(' '*4):
                     lines[y] = l[4:]
             else:
                 for y in range(int(self.selection[0][1]), int(self.selection[1][1])+1):
@@ -436,21 +498,24 @@
                         lines[y] = l[4:]
                         if y == int(cursor.y):
                             moveCursor = True
 
             self.cursor.x = max(self.cursor.x - 4, 0)
             self._append_undo(self.text, y, x)
             self.text = '\n'.join(lines)
-
+            self.render()
+            return
 
         if key in self.shortcuts['erase']:
             if not self.selection or self.selection[1] == self.selection[0]:
                 erase()
+                return
             else:
                 self.delete_selected()
+                return
 
         if key in self.shortcuts['erase_word']:
             # print('delete word')
             if x == 0:
                 erase()
                 return
 
@@ -476,65 +541,73 @@
                     beginning = beginning.rstrip().rsplit(' ', 1)[0]
 
                 removed = l[len(beginning):x]
 
                 l = beginning + l[x:]
                 self.cursor.x -= len(removed)
 
-
             lines[y] = l
             self._append_undo(self.text, y, x)
             self.text = '\n'.join(lines)
-
+            self.render()
+            return
 
         if key in self.shortcuts['move_line_down'] and self.cursor.y < self.max_lines:
             # print('move down')
             if y+1 == len(lines): # if at last line
                 self.text += '\n'
 
             self.move_line(y, 1)
+            self.render()
+            return
 
         if key in self.shortcuts['move_line_up'] and y > 0:
             self.move_line(y, -1)
-
+            self.render()
+            return
 
         if key in self.shortcuts['undo']:
             if not on_undo:
                 return
 
             self.on_redo.append((self.text, y, x))
             self.text = on_undo[-1][0]
             cursor.y = on_undo[-1][1]
             cursor.x = on_undo[-1][2]
             on_undo.pop()
+            self.render()
+            return
 
         if key in self.shortcuts['redo']:
             if not self.on_redo:
                 return
 
             on_undo.append((self.text, y, x))
             self.text = self.on_redo[-1][0]
             cursor.y = self.on_redo[-1][1]
             cursor.x = self.on_redo[-1][2]
             self.on_redo.pop()
-
+            self.render()
+            return
 
         if key in self.shortcuts['delete_line']:
             self._append_undo(self.text, y, 0)
             lines.pop(y)
 
             if y == 0:
                 self.cursor.x = 0
             else:
                 self.cursor.x = len(lines[y-1])
 
             if y >= len(lines) and y > 0:
                 self.cursor.y -= 1
 
             self.text = '\n'.join(lines)
+            self.render()
+            return
 
         if key in self.shortcuts['duplicate_line']:
             if len(lines) < self.max_lines:
                 self._append_undo(self.text, y, 0)
                 lines.insert(y, lines[y])
                 self.text = '\n'.join(lines)
                 cursor.y += 1
@@ -583,30 +656,29 @@
             if selectedText:
                 pyperclip.copy(selectedText)
                 self.delete_selected()
                 # print('-----cut:', selectedText)
 
         if key in self.shortcuts['select_all']:
             self.select_all()
+            return
 
-
-        elif self.register_mouse_input:
+        if self.register_mouse_input:
             if key == 'left mouse down' and mouse.hovered_entity == self.bg and mouse.point is not None:
                 cursor.position = self.get_mouse_position()
                 self.selection = [self.cursor.position, self.cursor.position]
                 self.draw_selection()
 
             if key == 'left mouse up':
                     cursor.position = self.get_mouse_position()
 
                     if self.selection:
                         self.selection[1] = self.cursor.position
 
 
-        self.render()
 
     def move_to_start_of_word(self):
         cursor = self.cursor
         x, y = int(cursor.x), int(cursor.y)
         lines = self.text.split('\n')
         l = lines[y]
         delimiters = self.delimiters
@@ -660,14 +732,17 @@
 
     def text_input(self, key):
         cursor, add_text = self.cursor, self.add_text
 
         if not self.active:
             return
 
+        if held_keys['shift'] and held_keys['alt']:
+            return
+
         if self.selection:  # delete selected text
             self.delete_selected()
 
         add_text(key)
 
         if key == '(':
             add_text(')')
@@ -680,16 +755,18 @@
             cursor.x -= 1
 
         self.render()
 
 
     def render(self):
         lines = self.text.split('\n')
-
-        text = '\n'*self.scroll + '\n'.join(lines[self.scroll : self.max_lines + self.scroll])
+        if self.max_lines < 9999:
+            text = '\n'*self.scroll + '\n'.join(lines[self.scroll : self.max_lines + self.scroll])
+        else:
+            text = self.text
 
         if not hasattr(self.text_entity, 'raw_text') or self._prev_text != text or self.scroll != self._prev_scroll:
             # print(self.scroll)
 
             if self.replacements:
                 _lines = text.split('\n')
                 for i in range(len(_lines)):
@@ -699,29 +776,29 @@
                         _lines[i] = multireplace(_lines[i], self.replacements)
                 self.text_entity.text = '\n'.join(_lines)
 
                 # self.text_entity.text = multireplace(text, self.replacements)
             else:
                 self.text_entity.text = text
 
-            self.line_numbers.text = ('     \n'*self.scroll) + '\n'.join([str(e + self.scroll).rjust(3, '0') for e in range(min(len(lines), self.max_lines))])
+            self.line_numbers.text = ('     \n'*self.scroll) + '\n'.join([str(e + self.scroll).rjust(3, ' ') for e in range(min(len(lines), self.max_lines))])
 
             self._prev_text = text
             self._prev_scroll = self.scroll
-            self.scroll_parent.y = (self.scroll * Text.size)
+            self.scroll_parent.y = (self.scroll * Text.size * self.line_height)
             self.cursor.visible = self.cursor.y >= self.scroll and self.cursor.y < self.scroll + self.max_lines
             self.draw_selection()
 
         if self.on_value_changed:
             self.on_value_changed()
 
 
 
     def update(self):
-        if self.register_mouse_input and mouse.left and mouse.moving:
+        if self.active and self.register_mouse_input and mouse.left and mouse.moving:
             self.cursor.position = self.get_mouse_position()
             if self.selection:
                 self.selection[1] = self.cursor.position
 
             self.draw_selection()
 
 
@@ -784,15 +861,15 @@
     Button.color = color._20
     window.color = color._25
 
     # Text.size = 1/window.fullscreen_size[1]*16
     # Text.default_font = 'consola.ttf'
     # Text.default_resolution = 16*2
     # TreeView()
-    te = TextField(max_lines=20, scale=1, register_mouse_input = True, text='1234')
+    te = TextField(max_lines=50, scale=1, register_mouse_input = True, text='1234')
     #te = TextField(max_lines=300, scale=1, register_mouse_input = True, scroll_size = (50,3))
     # te.line_numbers.enabled = True
     # for name in color.color_names:
     #     if name == 'black':
     #         continue
     #     te.replacements[f' {name}'] = f'☾{name}☽ {name}☾default☽'
     # te.replacements = {
@@ -808,12 +885,17 @@
     #
     import textwrap
     te.text = dedent('''
         Lorem ipsum dolor sit amet, consectetur adipiscing elit.
         Aliquam sapien tellus, venenatis sit amet ante et, malesuada porta risus.
         Etiam et mi luctus, viverra urna at, maximus eros. Sed dictum faucibus purus,
         nec rutrum ipsum condimentum in. Mauris iaculis arcu nec justo rutrum euismod.
-        Suspendisse dolor tortor, congue id erat sit amet, sollicitudin facilisis velit.'''
+        Suspendisse dolor tortor, congue id erat sit amet, sollicitudin facilisis velit.
+        Aliquam sapien tellus, venenatis sit amet ante et, malesuada porta risus.
+        Etiam et mi luctus, viverra urna at, maximus eros. Sed dictum faucibus purus,
+        nec rutrum ipsum condimentum in. Mauris iaculis arcu nec justo rutrum euismod.
+        Suspendisse dolor tortor, congue id erat sit amet, sollicitudin facilisis velit.
+        '''*30
         )[1:]
     te.render()
 
     app.run()
```

### Comparing `ursina-5.2.0/ursina/prefabs/tilemap.py` & `ursina-5.3.0/ursina/prefabs/tilemap.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/tooltip.py` & `ursina-5.3.0/ursina/prefabs/tooltip.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,26 +7,24 @@
         super().__init__(text=text, ignore=False, parent=camera.ui, wordwrap=wordwrap, origin=(-.5,-.5), margin=(2,2),
             background_color=color.inverse(color.text_color), enabled=False, background=True)
         self.background.color = background_color
 
         for key, value in kwargs.items():
             setattr(self, key, value)
 
-        self.original_scale = self.scale
-
 
     def update(self):
         self.position = mouse.position
         self.position = (
             mouse.x + (self.margin[0] * self.size/2) + .01,
             mouse.y + (self.margin[1] * self.size/2) + .01
             )
         self.x = min(self.x, (.5 * window.aspect_ratio) - self.width - self.size - .005)
         self.y = min(self.y, .5 - (self.height + self.size + .005))
-        self.z = -9
+        self.z = -99
 
 if __name__ == '__main__':
     app = Ursina()
 
     tooltip_test = Tooltip(
     '<scale:1.5><pink>' + 'Rainstorm' + '<scale:1> \n \n' +
 '''Summon a <blue>rain
```

### Comparing `ursina-5.2.0/ursina/prefabs/trail_renderer.py` & `ursina-5.3.0/ursina/prefabs/trail_renderer.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/ursfx.py` & `ursina-5.3.0/ursina/prefabs/ursfx.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     invoke(a.stop, delay=volume_curve[4][0] / speed)
     return a
 
 
 class SynthGUI(Entity):
     def __init__(self, **kwargs):
-        super().__init__(parent=camera.ui, **kwargs)
+        super().__init__(parent=camera.ui, z=-998, **kwargs)
 
         default_positions = [(0,0), (.1,.9), (.15,.75), (.6,.75), (1,0)]
         self.wave_panel = Entity(parent=self, scale=.35, x=-0)
         self.waveform = Entity(parent=self.wave_panel, scale_y=.75)
         self.waveform_bg = Entity(parent=self.waveform, model='quad', origin=(-.5,-.5), z=.01, color=color.black66)
         # self.bg_2 = Entity(parent=self.waveform, model='quad', origin=(-.5,-.5), z=.01, color=color._16)
         self.volume_slider = Slider(parent=self.wave_panel, x=-.05, vertical=True, scale=1.95, min=.05, max=1, default=.75, step=.01, on_value_changed=self.play)
```

### Comparing `ursina-5.2.0/ursina/prefabs/ursina_splash.py` & `ursina-5.3.0/ursina/prefabs/ursina_splash.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/prefabs/window_panel.py` & `ursina-5.3.0/ursina/prefabs/window_panel.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/raycast.py` & `ursina-5.3.0/ursina/raycast.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from ursina.hit_info import HitInfo
 from ursina import ursinamath, color
 from ursina.ursinastuff import destroy, invoke
 
 
 _line_model = Mesh(vertices=[Vec3(0,0,0), Vec3(0,0,1)], mode='line')
 
-_raycaster = Entity()
+_raycaster = Entity(add_to_scene_entities=False)
 _raycaster._picker = CollisionTraverser()  # Make a traverser
 _raycaster._pq = CollisionHandlerQueue()  # Make a handler
 _raycaster._pickerNode = CollisionNode('_raycaster')
 _raycaster._pickerNode.set_into_collide_mask(0)
 _raycaster._pickerNP = _raycaster.attach_new_node(_raycaster._pickerNode)
 _raycaster._picker.addCollider(_raycaster._pickerNP, _raycaster._pq)
 
@@ -116,15 +116,15 @@
     Player(model='cube', origin_y=-.5, color=color.orange)
     wall_left = Entity(model='cube', collider='box', scale_y=3, origin_y=-.5, color=color.azure, x=-4)
     wall_right = duplicate(wall_left, x=4)
     camera.y = 2
     app.run()
 
     # test
-    breakpoint()
+    # breakpoint()
     d = Entity(parent=scene, position=(0,0,2), model='cube', color=color.orange, collider='box', scale=2)
     e = Entity(model='cube', color=color.lime)
 
     camera.position = (0, 15, -15)
     camera.look_at(e)
     # camera.reparent_to(e)
     speed = .01
```

### Comparing `ursina-5.2.0/ursina/scene.py` & `ursina-5.3.0/ursina/scene.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,29 +3,42 @@
 
 
 class Scene(NodePath):
 
     def __init__(self):
         super().__init__('scene')
         self.entities = []
+        self._children = []
 
 
     def set_up(self):
         self.reparent_to(render)
         self.fog = Fog('fog')
         self.setFog(self.fog)
         self.fog_color = color.light_gray
         self.fog_density = 0
 
 
     def clear(self):
         from ursina.ursinastuff import destroy
         from ursina import application
 
-        [destroy(e) for e in self.entities if not e.eternal]
+        to_destroy = [e for e in self.entities if not e.eternal]
+        to_keep = [e for e in self.entities if e.eternal]
+
+        for d in to_destroy:
+            try:
+                destroy(d)
+            except Exception as e:
+                print('failed to destroy entity', e)
+
+
+        self.entities = to_keep
+
+
         application.sequences.clear()
 
 
     @property
     def fog_color(self):
         return self.fog.getColor()
 
@@ -42,14 +55,22 @@
     def fog_density(self, value):
         self._fog_density = value
         if isinstance(value, tuple):     # linear fog
             self.fog.setLinearRange(value[0], value[1])
         else:
             self.fog.setExpDensity(value)
 
+    @property
+    def children(self):
+        return [e for e in self._children if e]     # make sure list doesn't contain destroyed entities
+
+    @children.setter
+    def children(self, value):
+        self._children = value
+
 
 instance = Scene()
 
 
 
 if __name__ == '__main__':
     from ursina import *
```

### Comparing `ursina-5.2.0/ursina/scripts/_bat_to_exe.bat` & `ursina-5.3.0/ursina/scripts/_bat_to_exe.bat`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/scripts/_blend_export.py` & `ursina-5.3.0/ursina/scripts/_blend_export.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/scripts/_blender_scene_to_ursina.py` & `ursina-5.3.0/ursina/scripts/_blender_scene_to_ursina.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # print('starteddddddddddddddddddd')
 # for i, arg in enumerate(sys.argv):
 #     print('aaaaaaaaaaarg:', arg)
 
 blender_executable, blend_file = sys.argv[:2]
 script_file = sys.argv[4]
 out_file_path = sys.argv[5]
+decimals = int([e for e in sys.argv if e.startswith('--decimals=')][0][len('--decimals='):])
 
 scene_name = Path(bpy.data.filepath).stem
 print('file_name:', scene_name)
 
 code = ''
 
 if not '--models_only' in sys.argv:
@@ -56,52 +57,66 @@
     bm.free()
 
     verts = []
     normals = []
     vertex_colors = []
     uvs = []
 
+    indices = []
+
     for poly in mesh.polygons:
-        face_normal_x, face_normal_y, face_normal_z = 0, 0, 0
+        indices.extend(poly.vertices)
+
+    for idx in indices:
+        v = mesh.vertices[idx]
+        verts.append((round(v.co[0],decimals),round(v.co[2],decimals),round(v.co[1],decimals)))
+
+
+    if '--vertex_colors' in sys.argv:
+        v_cols = [
+            [round(e,decimals) for e in col.color_srgb]
+                for col in mesh.attributes.active_color.data]
+
+        for idx in indices:     # vertex colors
+            vertex_colors.append(v_cols[idx])
+
+        # vertex_colors = v_cols  # use this instead if using face color. face colors doesn't work with baking light to vertex colors though.
+
 
-        for idx in poly.vertices:
+    if '--normals' in sys.argv:
+        for idx in indices:
             v = mesh.vertices[idx]
-            verts.append((round(v.co[0],4),round(v.co[2],4),round(v.co[1],4)))
             normals.append((v.normal[0], v.normal[2], v.normal[1]))
-
     # average the vertex normals to get face normals
-    sharp_normals = []
-    for i in range(0, len(normals), 3):
-        averaged_normal = (
-            round(sum((normals[i][0], normals[i+1][0], normals[i+2][0])) / 3, 5),
-            round(sum((normals[i][1], normals[i+1][1], normals[i+2][1])) / 3, 5),
-            round(sum((normals[i][2], normals[i+1][2], normals[i+2][2])) / 3, 5),
-            )
-        for j in range(3):
-            sharp_normals.append(averaged_normal)
-
-    normals = sharp_normals
-
-    color_layer = mesh.vertex_colors.active
-    if color_layer and len(color_layer.data) > 0:
-        vertex_colors = [tuple(round(e, 4) for e in data.color) for data in color_layer.data]
-
-
-    uv_layer = mesh.uv_layers.active
-    if uv_layer and len(uv_layer.data) > 0:
-        uvs = [tuple(round(e, 4) for e in data.uv) for data in uv_layer.data]
+        sharp_normals = []
+        for i in range(0, len(normals), 3):
+            averaged_normal = (
+                round(sum((normals[i][0], normals[i+1][0], normals[i+2][0])) / 3, decimals),
+                round(sum((normals[i][1], normals[i+1][1], normals[i+2][1])) / 3, decimals),
+                round(sum((normals[i][2], normals[i+1][2], normals[i+2][2])) / 3, decimals),
+                )
+            for j in range(3):
+                sharp_normals.append(averaged_normal)
+
+        normals = sharp_normals
+
+
+    if '--uvs' in sys.argv:
+        uv_layer = mesh.uv_layers.active
+        if uv_layer and len(uv_layer.data) > 0:
+            uvs = [tuple(round(e, decimals) for e in data.uv) for data in uv_layer.data]
 
 
 
     code += f'''
 '{mesh.name.replace('.', '_')}' : Mesh(
-    vertices={verts},
-    normals={normals},
-    colors={vertex_colors},
-    uvs={uvs},
+    vertices={str(verts).replace(' ', '')},
+    normals={str(normals).replace(' ', '')},
+    colors={str(vertex_colors).replace(' ', '')},
+    uvs={str(uvs).replace(' ', '')},
 ),
 '''
 
 code += '}\n'
 
 if '--models_only' in sys.argv:
     print('sucessfully exported blender models')
@@ -139,89 +154,15 @@
             code += f'''
     color=({round(color[0],5)}, {round(color[1],5)}, {round(color[2],5)}, {round(color[3],5)}),'''
 
         code += f'''
     ignore=True,
     )'''
     code += '''\n\nscene_parent.meshes = meshes'''
-
     code += '''\nprint('created entities:', perf_counter() - t)\n'''
-    #        if ob.parent:
-    #            code += f'''parent=self.{ob.name.replace('.', '_')}'''
-
-
-
-        #This has to be done every time the object updates:
-        # ob = ob.evaluated_get(dg) #this gives us the evaluated version of the object. Aka with all modifiers and deformations applied.
-        # mesh = ob.to_mesh() #turn it into the mesh data block we want.
-        # verts = []
-        # tris = []
-        # uvs = []
-        # normals = []
-        # vertex_colors = []
-
-        # for poly in mesh.polygons:
-        #     tris.append(tuple(e for e in poly.vertices))
-        # # for poly in mesh.polygons:
-        # #     for idx in poly.vertices:
-        # #         verts.append(mesh.vertices[idx])
-        # #         normal = mesh.vertices[idx].normal
-        # #         n = (normal[0], normal[1], normal[2])
-        # #         normals.append(n)
-        #
-        #
-        # color_layer = mesh.vertex_colors.active
-        # if color_layer and len(color_layer.data) > 0:
-        #     if not vertex_colors:
-        #         vertex_colors = [(1,1,1,1) for e in mesh.vertices]
-        #
-        #     i = 0
-        #     for poly in mesh.polygons:
-        #         for idx in poly.vertices:
-        #             vertex_colors[idx] = tuple(round(e, 4) for e in color_layer.data[i].color)
-        #             i += 1
-        #
-        # uv_layer = mesh.uv_layers.active
-        # if uv_layer and len(uv_layer.data) > 0:
-        #     if not uvs:
-        #         uvs = [(0,0) for e in mesh.vertices]
-        #
-        #     i = 0
-        #     for poly in mesh.polygons:
-        #         for idx in poly.vertices:
-        #             uvs[idx] = tuple(round(e, 4) for e in uv_layer.data[i].uv)
-        #             i += 1
-
-
-    #     code += f'''
-    # model=Mesh('''
-    #     # code += f'''
-    #     # vertices=[{', '.join([f'Vec3({v.co[0]}, {v.co[2]}, {v.co[1]})' for v in verts])}],'''
-    #
-    #     code += f'''
-    #     vertices=[{', '.join([f'Vec3({round(v.co[0], 4)}, {round(v.co[2], 4)}, {round(v.co[1], 4)})' for v in mesh.vertices])}],
-    #     triangles={tris},'''
-    #
-    #     code += f'''
-    #     normals=({' ,'.join([f'Vec3({round(v.normal[0], 4)}, {round(v.normal[2], 4)}, {round(v.normal[1], 4)})' for v in mesh.vertices])}),'''
-    #     # code += f'''
-    #     # normals=({' ,'.join([f'Vec3({str(n[0])[5:]}, {n[2]}, {n[1]})' for v in normals])}),'''
-    #
-    #     if uvs:
-    #         code += f'''
-    #     uvs={uvs},'''
-    #
-    #     if vertex_colors:
-    #         code += f'''
-    #     colors={vertex_colors},'''
-    #
-    #     code += '\n    )'
-    #     code += '\n)'
-
-
 
     code += '''
 if __name__ == '__main__':
     EditorCamera()
     app.run()
 '''
```

### Comparing `ursina-5.2.0/ursina/scripts/chunk_mesh.py` & `ursina-5.3.0/ursina/scripts/chunk_mesh.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/scripts/colorize.py` & `ursina-5.3.0/ursina/scripts/colorize.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/scripts/combine.py` & `ursina-5.3.0/ursina/scripts/combine.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                 to_destroy.append(e)
 
     if auto_destroy:
         from ursina import destroy
         [destroy(e) for e in to_destroy]
 
     combine_parent.model = Mesh(vertices=verts, triangles=tris, normals=norms, uvs=uvs, colors=cols, mode='triangle')
-    print('combined')
+    # print('combined')
     # entity.model = Mesh(vertices=verts,  mode='triangle')
     # entity.flatten_strong()
     if analyze:
         render.analyze()
     return combine_parent.model
```

### Comparing `ursina-5.2.0/ursina/scripts/generate_normals.py` & `ursina-5.3.0/ursina/scripts/generate_normals.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/scripts/grid_layout.py` & `ursina-5.3.0/ursina/scripts/grid_layout.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/scripts/merge_vertices.py` & `ursina-5.3.0/ursina/scripts/merge_vertices.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/scripts/noclip_mode.py` & `ursina-5.3.0/ursina/scripts/noclip_mode.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/scripts/position_limiter.py` & `ursina-5.3.0/ursina/scripts/position_limiter.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/scripts/project_uvs.py` & `ursina-5.3.0/ursina/scripts/project_uvs.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/scripts/scrollable.py` & `ursina-5.3.0/ursina/scripts/scrollable.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/scripts/smooth_follow.py` & `ursina-5.3.0/ursina/scripts/smooth_follow.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/scripts/terraincast.py` & `ursina-5.3.0/ursina/scripts/terraincast.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/sequence.py` & `ursina-5.3.0/ursina/sequence.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/shader.py` & `ursina-5.3.0/ursina/shader.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/shaders/__init__.py` & `ursina-5.3.0/ursina/shaders/__init__.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/shaders/basic_lighting_shader.py` & `ursina-5.3.0/ursina/shaders/basic_lighting_shader.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/shaders/colored_lights_shader.py` & `ursina-5.3.0/ursina/shaders/colored_lights_shader.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/shaders/fresnel_shader.py` & `ursina-5.3.0/ursina/shaders/fresnel_shader.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/shaders/geom_shader.py` & `ursina-5.3.0/ursina/shaders/geom_shader.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/shaders/instancing_shader.py` & `ursina-5.3.0/ursina/shaders/instancing_shader.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/shaders/lit_with_shadows_shader.py` & `ursina-5.3.0/ursina/shaders/lit_with_shadows_shader.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/shaders/matcap_shader.py` & `ursina-5.3.0/ursina/shaders/matcap_shader.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/shaders/noise_fog_shader.py` & `ursina-5.3.0/ursina/shaders/noise_fog_shader.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/shaders/normals_shader.py` & `ursina-5.3.0/ursina/shaders/normals_shader.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/shaders/projector_shader.py` & `ursina-5.3.0/ursina/shaders/projector_shader.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,39 +4,44 @@
 uniform mat4 p3d_ModelMatrix;
 
 in vec4 p3d_Vertex;
 in vec2 p3d_MultiTexCoord0;
 uniform vec2 texture_scale;
 uniform vec2 texture_offset;
 out vec2 texcoord;
+in vec4 p3d_Color;
+out vec4 vertex_color;
 uniform vec2 projector_uv_scale;
 uniform vec2 projector_uv_offset;
 
 out vec2 world_uv;
 uniform float time;
 
 out float z;
 
 void main() {
     gl_Position = p3d_ModelViewProjectionMatrix * p3d_Vertex;
     texcoord = (p3d_MultiTexCoord0 * texture_scale) + texture_offset;
+    vertex_color = p3d_Color;
+
     world_uv = (p3d_ModelMatrix * p3d_Vertex).xz * projector_uv_scale;
     world_uv -= projector_uv_offset;
     world_uv += vec2(.5);
     z = gl_Position.z;
 }
 ''',
 
 fragment='''
 #version 140
 
 uniform sampler2D p3d_Texture0;
 uniform vec4 p3d_ColorScale;
 in vec2 texcoord;
 out vec4 fragColor;
+in vec4 vertex_color;
 
 uniform sampler2D projector_texture;
 uniform vec4 projector_color;
 in vec2 world_uv;
 
 uniform struct p3d_FogParameters {
   vec4 color;
@@ -53,15 +58,15 @@
 }
 
 void main() {
     vec4 color = texture(p3d_Texture0, texcoord) * p3d_ColorScale;
     color.rgb -= texture(projector_texture, world_uv).r * (vec3(1.) - projector_color.rgb) * projector_color.a;
     color.rgb = mix(color.rgb, p3d_Fog.color.rgb, clamp(inverse_lerp(p3d_Fog.start, p3d_Fog.end, z), 0.0, 1.0)); // linear fog
 
-    fragColor = color.rgba;
+    fragColor = color.rgba * vertex_color;
 }''',
 
 default_input = {
     'texture_scale': Vec2(1,1),
     'texture_offset': Vec2(0,0),
     'projector_texture' : Func(load_texture, 'vignette'),
     'projector_uv_scale' : Vec2(.05, .05),
```

### Comparing `ursina-5.2.0/ursina/shaders/screenspace_shaders/camera_empty.py` & `ursina-5.3.0/ursina/shaders/screenspace_shaders/camera_empty.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/shaders/screenspace_shaders/camera_grayscale.py` & `ursina-5.3.0/ursina/shaders/screenspace_shaders/camera_grayscale.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/shaders/screenspace_shaders/camera_outline_shader.py` & `ursina-5.3.0/ursina/shaders/screenspace_shaders/camera_outline_shader.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/shaders/screenspace_shaders/camera_vertical_blur.py` & `ursina-5.3.0/ursina/shaders/screenspace_shaders/camera_vertical_blur.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/shaders/screenspace_shaders/fxaa.py` & `ursina-5.3.0/ursina/shaders/screenspace_shaders/fxaa.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/shaders/screenspace_shaders/pixelation_shader.py` & `ursina-5.3.0/ursina/shaders/screenspace_shaders/pixelation_shader.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/shaders/screenspace_shaders/ssao.py` & `ursina-5.3.0/ursina/shaders/screenspace_shaders/ssao.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/shaders/texture_blend_shader.py` & `ursina-5.3.0/ursina/shaders/texture_blend_shader.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/shaders/transition_shader.py` & `ursina-5.3.0/ursina/shaders/transition_shader.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/shaders/triplanar_shader.py` & `ursina-5.3.0/ursina/shaders/triplanar_shader.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/shaders/unlit_shader.py` & `ursina-5.3.0/ursina/shaders/unlit_shader.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/string_utilities.py` & `ursina-5.3.0/ursina/string_utilities.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/text.py` & `ursina-5.3.0/ursina/text.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/texture.py` & `ursina-5.3.0/ursina/texture.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/texture_importer.py` & `ursina-5.3.0/ursina/texture_importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,16 @@
                 imported_textures[name] = t
                 return t
 
     if application.development_mode:
         try:
             from psd_tools import PSDImage
         except (ModuleNotFoundError, ImportError) as e:
-            print('info: psd-tools3 not installed')
+            pass
+            # print('info: psd-tools3 not installed')
 
         for folder in folders:
             for filename in folder.glob('**/' + name + '.psd'):
                 print('found uncompressed psd, compressing it...')
                 compress_textures(name)
                 return load_texture(name)
```

### Comparing `ursina-5.2.0/ursina/textures/arrow_down.png` & `ursina-5.3.0/ursina/textures/arrow_down.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/arrow_right.png` & `ursina-5.3.0/ursina/textures/arrow_right.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/brick.png` & `ursina-5.3.0/ursina/textures/brick.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/circle.png` & `ursina-5.3.0/ursina/textures/circle.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/circle_outlined.png` & `ursina-5.3.0/ursina/textures/circle_outlined.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/cog.png` & `ursina-5.3.0/ursina/textures/cog.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/cursor.png` & `ursina-5.3.0/ursina/textures/cursor.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/file_icon.png` & `ursina-5.3.0/ursina/textures/file_icon.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/folder.png` & `ursina-5.3.0/ursina/textures/folder.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/grass.png` & `ursina-5.3.0/ursina/textures/grass.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/grass_tintable.png` & `ursina-5.3.0/ursina/textures/grass_tintable.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/heightmap_1.png` & `ursina-5.3.0/ursina/textures/heightmap_1.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/horizontal_gradient.png` & `ursina-5.3.0/ursina/textures/horizontal_gradient.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/items/bag.png` & `ursina-5.3.0/ursina/textures/items/bag.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/items/bow_arrow.png` & `ursina-5.3.0/ursina/textures/items/bow_arrow.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/items/gem.png` & `ursina-5.3.0/ursina/textures/items/gem.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/items/items.psd` & `ursina-5.3.0/ursina/textures/items/items.psd`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/items/orb.png` & `ursina-5.3.0/ursina/textures/items/orb.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/items/sword.png` & `ursina-5.3.0/ursina/textures/items/sword.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/noise.png` & `ursina-5.3.0/ursina/textures/noise.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/perlin_noise.png` & `ursina-5.3.0/ursina/textures/perlin_noise.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/radial_gradient.png` & `ursina-5.3.0/ursina/textures/radial_gradient.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/rainbow.png` & `ursina-5.3.0/ursina/textures/rainbow.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/reflection_map_3.jpg` & `ursina-5.3.0/ursina/textures/reflection_map_3.jpg`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/shore.jpg` & `ursina-5.3.0/ursina/textures/shore.jpg`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/sky_default.jpg` & `ursina-5.3.0/ursina/textures/sky_default.jpg`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/sky_sunset.jpg` & `ursina-5.3.0/ursina/textures/sky_sunset.jpg`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/test_tileset.png` & `ursina-5.3.0/ursina/textures/test_tileset.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/tilemap_test_level.png` & `ursina-5.3.0/ursina/textures/tilemap_test_level.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/ursina_logo.png` & `ursina-5.3.0/ursina/textures/ursina_logo.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/ursina_wink_0000.png` & `ursina-5.3.0/ursina/textures/ursina_wink_0000.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/ursina_wink_0001.png` & `ursina-5.3.0/ursina/textures/ursina_wink_0001.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/vertical_gradient.png` & `ursina-5.3.0/ursina/textures/vertical_gradient.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/vignette.jpg` & `ursina-5.3.0/ursina/textures/vignette.jpg`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/textures/white_cube.png` & `ursina-5.3.0/ursina/textures/white_cube.png`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/trigger.py` & `ursina-5.3.0/ursina/trigger.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/ursinamath.py` & `ursina-5.3.0/ursina/ursinamath.py`

 * *Files 10% similar despite different names*

```diff
@@ -97,26 +97,33 @@
     if not step:
         return value
 
     step = 1/step
     return round(value * step) / step
 
 
-def rotate_point_2d(point, origin, deg):
+def rotate_around_point_2d(point, origin, deg):
     angle_rad = -deg/180 * pi # ursina rotation is positive=clockwise, so do *= -1
     cos_angle = cos(angle_rad)
     sin_angle = sin(angle_rad)
     dx = point[0] - origin[0]
     dy = point[1] - origin[1]
 
     return (
         origin[0] + (dx*cos_angle - dy*sin_angle),
         origin[1] + (dx*sin_angle + dy*cos_angle)
         )
 
+def world_position_to_screen_position(point): # get screen position(ui space) from world space.
+    from ursina import camera, Entity, destroy
+    _temp_entity = Entity(position=point, add_to_scene_entities=False)
+    result = _temp_entity.screen_position
+    destroy(_temp_entity)
+    return result
+
 
 def chunk_list(l, chunk_size):
     # yield successive chunks from list
     for i in range(0, len(l), chunk_size):
         yield l[i:i + chunk_size]
 
 
@@ -183,10 +190,10 @@
     print(lerp((0,0), (0,1), .5))
     print(lerp(Vec2(0,0), Vec2(0,1), .5))
     print(lerp([0,0], [0,1], .5))
 
     print(round(Vec3(.38, .1351, 353.26), 2))
 
     p = (1,0)
-    print(p, 'rotated ->', rotate_point_2d(p, (0,0), 90))
+    print(p, 'rotated ->', rotate_around_point_2d(p, (0,0), 90))
 
     app.run()
```

### Comparing `ursina-5.2.0/ursina/ursinastuff.py` & `ursina-5.3.0/ursina/ursinastuff.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,26 +58,21 @@
         return
 
     if entity.eternal and not force_destroy:
         return
 
     if hasattr(entity, 'stop'):
         entity.stop(False)
-        # return
 
     if hasattr(entity, 'on_destroy'):
         entity.on_destroy()
 
-    for c in entity.children:
-        _destroy(c)
-
     if entity in scene.entities:
         scene.entities.remove(entity)
 
-
     if hasattr(entity, 'scripts'):
         for s in entity.scripts:
             del s
 
     if hasattr(entity, 'animations'):
         for anim in entity.animations:
             anim.finish()
@@ -85,18 +80,15 @@
 
     if hasattr(entity, 'tooltip'):
         _destroy(entity.tooltip)
 
     if hasattr(entity, '_on_click') and isinstance(entity._on_click, Sequence):
         entity._on_click.kill()
 
-    try:
-        entity.removeNode()
-    except:
-        print('already destroyed')
+    entity.removeNode()
     #unload texture
     # if hasattr(entity, 'texture') and entity.texture != None:
     #     entity.texture.releaseAll()
 
     del entity
```

### Comparing `ursina-5.2.0/ursina/vec2.py` & `ursina-5.3.0/ursina/vec2.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/vec3.py` & `ursina-5.3.0/ursina/vec3.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/vec4.py` & `ursina-5.3.0/ursina/vec4.py`

 * *Files identical despite different names*

### Comparing `ursina-5.2.0/ursina/window.py` & `ursina-5.3.0/ursina/window.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import platform
 from panda3d.core import WindowProperties
 from panda3d.core import loadPrcFileData
 from ursina.vec2 import Vec2
 from ursina import color, application
 from ursina.scene import instance as scene    # for toggling collider visibility
 from ursina.string_utilities import print_info, print_warning
+from screeninfo import get_monitors
 
 
 class Window(WindowProperties):
 
     def __init__(self):
         super().__init__()
         loadPrcFileData('', 'window-title ursina')
@@ -31,63 +32,46 @@
 
         self.vsync = True   # can't be set during play
         self.show_ursina_splash = False
 
         self.title = application.asset_folder.name
         self.borderless = True
         # self.icon = 'textures/ursina.ico'
-        os_name = platform.system()
+        self.monitors = get_monitors()
+        self.monitor_index = 0
 
-        try:
-            if os_name == 'Windows':     # windows
-                import ctypes
-                user32 = ctypes.windll.user32
-                user32.SetProcessDPIAware()
-                self.screen_resolution = (user32.GetSystemMetrics(0), user32.GetSystemMetrics(1))
-
-            elif os_name == 'Linux':
-                import Xlib
-                import Xlib.display
-                resolution = Xlib.display.Display().screen().root.get_geometry()
-                self.screen_resolution = Vec2(resolution.width, resolution.height)
-
-            elif os_name == 'Darwin':     # mac
-                from AppKit import NSScreen
-                size = NSScreen.mainScreen().frame().size
-                self.screen_resolution = [size.width, size.height]
-        except:
-            from screeninfo import get_monitors
-            self.screen_resolution = [get_monitors()[0].width, get_monitors()[0].height]
-
-        self.fullscreen_size = Vec2(*self.screen_resolution)
+        monitor = self.monitors[self.monitor_index]
+        self.fullscreen_size = Vec2(monitor.width, monitor.height)
         self.windowed_size = self.fullscreen_size / 1.25
-        loadPrcFileData('', f'win-size {self.windowed_size[0]} {self.windowed_size[1]}')
         self.windowed_position = None   # gets set when entering fullscreen so position will be correct when going back to windowed mode
         self.forced_aspect_ratio = None # example: window.forced_aspect_ratio = 16/9
         self.size = self.windowed_size
         self.always_on_top = False
 
         self.top = Vec2(0, .5)
         self.bottom = Vec2(0, -.5)
         self.center = Vec2(0, 0)
 
 
     def late_init(self):
-        self.center_on_screen()
+        if application.window_type != 'none':
+            self.center_on_screen()
+
         if not application.development_mode:
             self.fullscreen = True
 
         self.color = color.dark_gray
         self.render_modes = ('default', 'wireframe', 'colliders', 'normals')
         self.render_mode = 'default'
         self.editor_ui = None
 
-        base.accept('aspectRatioChanged', self.update_aspect_ratio)
-        if self.always_on_top:
-            self.setZOrder(WindowProperties.Z_top)
+        if application.window_type != 'none':
+            base.accept('aspectRatioChanged', self.update_aspect_ratio)
+            if self.always_on_top:
+                self.setZOrder(WindowProperties.Z_top)
 
 
     @property
     def left(self):
         return Vec2(-self.aspect_ratio/2, 0)
     @property
     def right(self):
@@ -103,15 +87,19 @@
         return Vec2(-self.aspect_ratio/2, -.5)
     @property
     def bottom_right(self):
         return Vec2(self.aspect_ratio/2, -.5)
 
 
     def center_on_screen(self):
-        self.position = Vec2(int((self.screen_resolution[0]-self.size[0])/2), int((self.screen_resolution[1]-self.size[1])/2))
+        monitor = self.monitors[self.monitor_index]
+        x = monitor.x + (monitor.width-self.size[0])/2
+        y = monitor.y + (monitor.height-self.size[1])/2
+        self.position = Vec2(x,y)
+
 
     def make_editor_gui(self):     # called by main after setting up camera and application.development_mode
         from ursina import camera, Entity, Text, Button, ButtonList, Func, Tooltip, held_keys, mouse
         import time
 
         self.editor_ui = Entity(parent=camera.ui, eternal=True, enabled=bool(application.development_mode))
 
@@ -163,20 +151,19 @@
             'Reset Render Mode <gray>[Shift+F10]<default>' : Func(setattr, self, 'render_mode', 'default'),
             'Toggle Hotreloading <gray>[F9]<default>' : application.hot_reloader.toggle_hotreloading,
             'Reload Shaders <gray>[F7]<default>' : application.hot_reloader.reload_shaders,
             'Reload Models <gray>[F7]<default>' : application.hot_reloader.reload_models,
             'Reload Textures <gray>[F6]<default>' : application.hot_reloader.reload_textures,
             'Reload Code <gray>[F5]<default>' : application.hot_reloader.reload_code,
         },
-            width=.35, x=.62, enabled=False, eternal=True, name='cog_menu',
+            width=.4, scale=.75, x=(.5*self.aspect_ratio)-(.4*.75), enabled=False, eternal=True, name='cog_menu',
         )
         self.cog_menu.on_click = Func(setattr, self.cog_menu, 'enabled', False)
-        print(self.cog_menu.scale_y)
-        self.cog_menu.scale *= .75
-        self.cog_menu.text_entity.x += .025
+        # print(self.cog_menu.scale_y)
+        # self.cog_menu.scale *= .75
         self.cog_menu.highlight.color = color.azure
         self.cog_button = Button(parent=self.editor_ui, eternal=True, model='quad', texture='cog', scale=.015, origin=(1,-1), position=self.bottom_right, name='cog_button')
         self.cog_menu.y = self.cog_button.y + (self.cog_menu.bg.scale_y * self.cog_menu.scale_y) + Text.size
         info_text ='''This menu is not enabled in builds. To see how the app will look like in builds, do Ursina(development_mode=False), which will disable all editor ui and start the app in fullscreen. To disable only this menu, do window.cog_menu.enabled = False'''
         self.cog_menu.info = Button(parent=self.cog_menu, model='circle', text='<gray>?', scale=.025, origin=(.5,-.5), tooltip=Tooltip(info_text, scale=.75, origin=(-.5,-.5), eternal=True), eternal=True, name='cog_menu_info')
         self.cog_menu.info.text_entity.scale *= .75
         def _toggle_cog_menu():
@@ -313,14 +300,16 @@
     @icon.setter
     def icon(self, value):
         self._icon = value
         self.setIconFilename(value)
 
 
     def __setattr__(self, name, value):
+        if application.window_type == 'none':
+            return
         try:
             super().__setattr__(name, value)
         except:
             pass
 
         if name == 'fullscreen':
             try:
```

### Comparing `ursina-5.2.0/ursina.egg-info/PKG-INFO` & `ursina-5.3.0/ursina.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ursina
-Version: 5.2.0
+Version: 5.3.0
 Summary: An easy to use game engine/framework for python.
 Home-page: https://github.com/pokepetter/ursina
 Author: Petter Amland
 Author-email: pokepetter@gmail.com
 License: MIT
 Keywords: game development
 Platform: UNKNOWN
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: extras
 License-File: LICENSE
 
 # ursina    ʕ •ᴥ•ʔゝ□
 An easy to use game engine/framework for python.
```

### Comparing `ursina-5.2.0/ursina.egg-info/SOURCES.txt` & `ursina-5.3.0/ursina.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 ursina/models_compressed/wireframe_quad.ursinamesh
 ursina/prefabs/__init__.py
 ursina/prefabs/animation.py
 ursina/prefabs/animator.py
 ursina/prefabs/button.py
 ursina/prefabs/button_group.py
 ursina/prefabs/button_list.py
+ursina/prefabs/color_picker.py
 ursina/prefabs/conversation.py
 ursina/prefabs/cursor.py
 ursina/prefabs/draggable.py
 ursina/prefabs/dropdown_menu.py
 ursina/prefabs/editor_camera.py
 ursina/prefabs/file_browser.py
 ursina/prefabs/file_browser_save.py
```

