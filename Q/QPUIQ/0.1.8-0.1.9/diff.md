# Comparing `tmp/QPUIQ-0.1.8.tar.gz` & `tmp/QPUIQ-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QPUIQ-0.1.8.tar", last modified: Sun Apr 30 05:52:49 2023, max compression
+gzip compressed data, was "QPUIQ-0.1.9.tar", last modified: Mon May  1 15:14:04 2023, max compression
```

## Comparing `QPUIQ-0.1.8.tar` & `QPUIQ-0.1.9.tar`

### file list

```diff
@@ -1,71 +1,74 @@
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-30 05:52:49.775992 QPUIQ-0.1.8/
--rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-03-12 08:03:22.000000 QPUIQ-0.1.8/LICENSE.txt
--rw-r--r--   0 Bug        (504) staff       (20)     2889 2023-04-30 05:52:49.775860 QPUIQ-0.1.8/PKG-INFO
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-30 05:52:49.769022 QPUIQ-0.1.8/PUI/
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-30 05:52:49.770354 QPUIQ-0.1.8/PUI/PySide6/
--rw-r--r--   0 Bug        (504) staff       (20)      891 2023-04-30 05:45:53.000000 QPUIQ-0.1.8/PUI/PySide6/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      498 2023-04-29 18:30:29.000000 QPUIQ-0.1.8/PUI/PySide6/application.py
--rw-r--r--   0 Bug        (504) staff       (20)     1187 2023-04-30 05:12:20.000000 QPUIQ-0.1.8/PUI/PySide6/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      616 2023-04-29 06:22:40.000000 QPUIQ-0.1.8/PUI/PySide6/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     2838 2023-04-30 05:45:40.000000 QPUIQ-0.1.8/PUI/PySide6/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      352 2023-04-23 17:43:52.000000 QPUIQ-0.1.8/PUI/PySide6/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      543 2023-04-26 17:57:33.000000 QPUIQ-0.1.8/PUI/PySide6/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      464 2023-04-23 17:43:58.000000 QPUIQ-0.1.8/PUI/PySide6/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      791 2023-04-23 17:44:06.000000 QPUIQ-0.1.8/PUI/PySide6/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1299 2023-04-29 16:58:24.000000 QPUIQ-0.1.8/PUI/PySide6/window.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-30 05:52:49.771678 QPUIQ-0.1.8/PUI/Qt5/
--rw-r--r--   0 Bug        (504) staff       (20)      417 2023-04-29 17:06:45.000000 QPUIQ-0.1.8/PUI/Qt5/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      496 2023-04-29 18:30:13.000000 QPUIQ-0.1.8/PUI/Qt5/application.py
--rw-r--r--   0 Bug        (504) staff       (20)     1138 2023-04-30 05:12:20.000000 QPUIQ-0.1.8/PUI/Qt5/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      616 2023-04-23 17:44:21.000000 QPUIQ-0.1.8/PUI/Qt5/button.py
--rw-r--r--   0 Bug        (504) staff       (20)     1527 2023-04-26 17:40:36.000000 QPUIQ-0.1.8/PUI/Qt5/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      352 2023-04-23 17:44:32.000000 QPUIQ-0.1.8/PUI/Qt5/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      541 2023-03-13 15:01:12.000000 QPUIQ-0.1.8/PUI/Qt5/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      464 2023-04-23 17:44:38.000000 QPUIQ-0.1.8/PUI/Qt5/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      791 2023-04-23 17:44:41.000000 QPUIQ-0.1.8/PUI/Qt5/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1297 2023-04-29 17:05:56.000000 QPUIQ-0.1.8/PUI/Qt5/window.py
--rw-r--r--   0 Bug        (504) staff       (20)      486 2023-04-30 05:52:33.000000 QPUIQ-0.1.8/PUI/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      458 2023-04-29 06:46:04.000000 QPUIQ-0.1.8/PUI/decorator.py
--rw-r--r--   0 Bug        (504) staff       (20)     2627 2023-04-29 19:40:07.000000 QPUIQ-0.1.8/PUI/dom.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-30 05:52:49.772838 QPUIQ-0.1.8/PUI/flet/
--rw-r--r--   0 Bug        (504) staff       (20)      452 2023-04-29 19:08:30.000000 QPUIQ-0.1.8/PUI/flet/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      551 2023-04-29 19:19:55.000000 QPUIQ-0.1.8/PUI/flet/application.py
--rw-r--r--   0 Bug        (504) staff       (20)       68 2023-03-13 14:50:39.000000 QPUIQ-0.1.8/PUI/flet/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      647 2023-03-15 07:54:51.000000 QPUIQ-0.1.8/PUI/flet/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      407 2023-03-13 16:17:28.000000 QPUIQ-0.1.8/PUI/flet/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      943 2023-04-14 18:19:33.000000 QPUIQ-0.1.8/PUI/flet/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      425 2023-03-14 19:58:06.000000 QPUIQ-0.1.8/PUI/flet/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      748 2023-03-13 16:17:18.000000 QPUIQ-0.1.8/PUI/flet/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)      482 2023-04-29 19:19:13.000000 QPUIQ-0.1.8/PUI/flet/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     3075 2023-04-29 20:53:50.000000 QPUIQ-0.1.8/PUI/node.py
--rw-r--r--   0 Bug        (504) staff       (20)     8973 2023-04-29 20:54:27.000000 QPUIQ-0.1.8/PUI/state.py
--rw-r--r--   0 Bug        (504) staff       (20)      983 2023-03-16 07:50:08.000000 QPUIQ-0.1.8/PUI/timeline.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-30 05:52:49.774165 QPUIQ-0.1.8/PUI/tkinter/
--rw-r--r--   0 Bug        (504) staff       (20)      414 2023-04-29 18:25:14.000000 QPUIQ-0.1.8/PUI/tkinter/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)      568 2023-04-29 18:55:09.000000 QPUIQ-0.1.8/PUI/tkinter/application.py
--rw-r--r--   0 Bug        (504) staff       (20)      541 2023-04-29 19:57:02.000000 QPUIQ-0.1.8/PUI/tkinter/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      528 2023-04-23 17:43:10.000000 QPUIQ-0.1.8/PUI/tkinter/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      954 2023-04-29 19:31:18.000000 QPUIQ-0.1.8/PUI/tkinter/canvas.py
--rw-r--r--   0 Bug        (504) staff       (20)      403 2023-04-23 17:43:21.000000 QPUIQ-0.1.8/PUI/tkinter/label.py
--rw-r--r--   0 Bug        (504) staff       (20)     1636 2023-04-29 19:55:02.000000 QPUIQ-0.1.8/PUI/tkinter/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      468 2023-04-23 17:43:25.000000 QPUIQ-0.1.8/PUI/tkinter/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      866 2023-04-23 17:43:29.000000 QPUIQ-0.1.8/PUI/tkinter/textfield.py
--rw-r--r--   0 Bug        (504) staff       (20)     1530 2023-04-29 19:56:35.000000 QPUIQ-0.1.8/PUI/tkinter/window.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-30 05:52:49.775198 QPUIQ-0.1.8/PUI/urwid/
--rw-r--r--   0 Bug        (504) staff       (20)      429 2023-04-29 17:20:40.000000 QPUIQ-0.1.8/PUI/urwid/__init__.py
--rw-r--r--   0 Bug        (504) staff       (20)     1246 2023-04-29 19:07:03.000000 QPUIQ-0.1.8/PUI/urwid/application.py
--rw-r--r--   0 Bug        (504) staff       (20)       63 2023-03-14 09:21:15.000000 QPUIQ-0.1.8/PUI/urwid/base.py
--rw-r--r--   0 Bug        (504) staff       (20)      678 2023-03-15 07:59:17.000000 QPUIQ-0.1.8/PUI/urwid/button.py
--rw-r--r--   0 Bug        (504) staff       (20)      356 2023-03-16 07:54:05.000000 QPUIQ-0.1.8/PUI/urwid/label.py
--rw-r--r--   0 Bug        (504) staff       (20)      734 2023-03-16 07:54:02.000000 QPUIQ-0.1.8/PUI/urwid/layout.py
--rw-r--r--   0 Bug        (504) staff       (20)      462 2023-03-15 00:27:06.000000 QPUIQ-0.1.8/PUI/urwid/progressbar.py
--rw-r--r--   0 Bug        (504) staff       (20)      315 2023-04-29 19:07:06.000000 QPUIQ-0.1.8/PUI/urwid/window.py
--rw-r--r--   0 Bug        (504) staff       (20)     2604 2023-04-30 05:49:42.000000 QPUIQ-0.1.8/PUI/view.py
-drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-04-30 05:52:49.775682 QPUIQ-0.1.8/QPUIQ.egg-info/
--rw-r--r--   0 Bug        (504) staff       (20)     2889 2023-04-30 05:52:49.000000 QPUIQ-0.1.8/QPUIQ.egg-info/PKG-INFO
--rw-r--r--   0 Bug        (504) staff       (20)     1251 2023-04-30 05:52:49.000000 QPUIQ-0.1.8/QPUIQ.egg-info/SOURCES.txt
--rw-r--r--   0 Bug        (504) staff       (20)        1 2023-04-30 05:52:49.000000 QPUIQ-0.1.8/QPUIQ.egg-info/dependency_links.txt
--rw-r--r--   0 Bug        (504) staff       (20)        4 2023-04-30 05:52:49.000000 QPUIQ-0.1.8/QPUIQ.egg-info/top_level.txt
--rw-r--r--   0 Bug        (504) staff       (20)     2629 2023-04-29 21:00:52.000000 QPUIQ-0.1.8/README.md
--rw-r--r--   0 Bug        (504) staff       (20)       38 2023-04-30 05:52:49.776027 QPUIQ-0.1.8/setup.cfg
--rw-r--r--   0 Bug        (504) staff       (20)      539 2023-04-29 10:19:13.000000 QPUIQ-0.1.8/setup.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-01 15:14:04.670331 QPUIQ-0.1.9/
+-rw-r--r--   0 Bug        (504) staff       (20)     1072 2023-03-12 08:03:22.000000 QPUIQ-0.1.9/LICENSE.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     2889 2023-05-01 15:14:04.670198 QPUIQ-0.1.9/PKG-INFO
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-01 15:14:04.655351 QPUIQ-0.1.9/PUI/
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-01 15:14:04.658463 QPUIQ-0.1.9/PUI/PySide6/
+-rw-r--r--   0 Bug        (504) staff       (20)     1109 2023-05-01 14:22:51.000000 QPUIQ-0.1.9/PUI/PySide6/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      498 2023-04-29 18:30:29.000000 QPUIQ-0.1.9/PUI/PySide6/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2334 2023-05-01 15:09:58.000000 QPUIQ-0.1.9/PUI/PySide6/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      616 2023-04-29 06:22:40.000000 QPUIQ-0.1.9/PUI/PySide6/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     3128 2023-05-01 15:09:30.000000 QPUIQ-0.1.9/PUI/PySide6/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      352 2023-04-23 17:43:52.000000 QPUIQ-0.1.9/PUI/PySide6/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      807 2023-05-01 14:28:35.000000 QPUIQ-0.1.9/PUI/PySide6/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      464 2023-04-23 17:43:58.000000 QPUIQ-0.1.9/PUI/PySide6/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      991 2023-04-30 15:12:34.000000 QPUIQ-0.1.9/PUI/PySide6/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)      791 2023-04-23 17:44:06.000000 QPUIQ-0.1.9/PUI/PySide6/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1326 2023-05-01 13:25:01.000000 QPUIQ-0.1.9/PUI/PySide6/window.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-01 15:14:04.660914 QPUIQ-0.1.9/PUI/Qt5/
+-rw-r--r--   0 Bug        (504) staff       (20)      417 2023-04-29 17:06:45.000000 QPUIQ-0.1.9/PUI/Qt5/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      496 2023-04-29 18:30:13.000000 QPUIQ-0.1.9/PUI/Qt5/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1138 2023-04-30 05:12:20.000000 QPUIQ-0.1.9/PUI/Qt5/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      616 2023-04-23 17:44:21.000000 QPUIQ-0.1.9/PUI/Qt5/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1527 2023-04-26 17:40:36.000000 QPUIQ-0.1.9/PUI/Qt5/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      352 2023-04-23 17:44:32.000000 QPUIQ-0.1.9/PUI/Qt5/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      541 2023-03-13 15:01:12.000000 QPUIQ-0.1.9/PUI/Qt5/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      464 2023-04-23 17:44:38.000000 QPUIQ-0.1.9/PUI/Qt5/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      791 2023-04-23 17:44:41.000000 QPUIQ-0.1.9/PUI/Qt5/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1297 2023-04-29 17:05:56.000000 QPUIQ-0.1.9/PUI/Qt5/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)      488 2023-05-01 15:12:51.000000 QPUIQ-0.1.9/PUI/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      525 2023-05-01 12:18:54.000000 QPUIQ-0.1.9/PUI/decorator.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2627 2023-04-30 15:12:00.000000 QPUIQ-0.1.9/PUI/dom.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-01 15:14:04.663889 QPUIQ-0.1.9/PUI/flet/
+-rw-r--r--   0 Bug        (504) staff       (20)      452 2023-04-29 19:08:30.000000 QPUIQ-0.1.9/PUI/flet/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      551 2023-04-29 19:19:55.000000 QPUIQ-0.1.9/PUI/flet/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)       68 2023-03-13 14:50:39.000000 QPUIQ-0.1.9/PUI/flet/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      647 2023-03-15 07:54:51.000000 QPUIQ-0.1.9/PUI/flet/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      407 2023-03-13 16:17:28.000000 QPUIQ-0.1.9/PUI/flet/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      943 2023-04-14 18:19:33.000000 QPUIQ-0.1.9/PUI/flet/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      425 2023-03-14 19:58:06.000000 QPUIQ-0.1.9/PUI/flet/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      748 2023-03-13 16:17:18.000000 QPUIQ-0.1.9/PUI/flet/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)      482 2023-04-29 19:19:13.000000 QPUIQ-0.1.9/PUI/flet/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     3309 2023-05-01 14:03:40.000000 QPUIQ-0.1.9/PUI/node.py
+-rw-r--r--   0 Bug        (504) staff       (20)     8998 2023-05-01 12:23:44.000000 QPUIQ-0.1.9/PUI/state.py
+-rw-r--r--   0 Bug        (504) staff       (20)      983 2023-03-16 07:50:08.000000 QPUIQ-0.1.9/PUI/timeline.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-01 15:14:04.666993 QPUIQ-0.1.9/PUI/tkinter/
+-rw-r--r--   0 Bug        (504) staff       (20)      488 2023-04-30 08:13:51.000000 QPUIQ-0.1.9/PUI/tkinter/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)      568 2023-04-29 18:55:09.000000 QPUIQ-0.1.9/PUI/tkinter/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)      541 2023-04-29 19:57:02.000000 QPUIQ-0.1.9/PUI/tkinter/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      528 2023-04-23 17:43:10.000000 QPUIQ-0.1.9/PUI/tkinter/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1729 2023-04-30 08:20:56.000000 QPUIQ-0.1.9/PUI/tkinter/canvas.py
+-rw-r--r--   0 Bug        (504) staff       (20)      403 2023-04-23 17:43:21.000000 QPUIQ-0.1.9/PUI/tkinter/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1642 2023-04-30 08:53:03.000000 QPUIQ-0.1.9/PUI/tkinter/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      468 2023-04-23 17:43:25.000000 QPUIQ-0.1.9/PUI/tkinter/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      694 2023-04-30 09:14:54.000000 QPUIQ-0.1.9/PUI/tkinter/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)      866 2023-04-23 17:43:29.000000 QPUIQ-0.1.9/PUI/tkinter/textfield.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1530 2023-04-29 19:56:35.000000 QPUIQ-0.1.9/PUI/tkinter/window.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-01 15:14:04.669426 QPUIQ-0.1.9/PUI/urwid/
+-rw-r--r--   0 Bug        (504) staff       (20)      469 2023-04-30 08:00:16.000000 QPUIQ-0.1.9/PUI/urwid/__init__.py
+-rw-r--r--   0 Bug        (504) staff       (20)     1246 2023-04-29 19:07:03.000000 QPUIQ-0.1.9/PUI/urwid/application.py
+-rw-r--r--   0 Bug        (504) staff       (20)       63 2023-03-14 09:21:15.000000 QPUIQ-0.1.9/PUI/urwid/base.py
+-rw-r--r--   0 Bug        (504) staff       (20)      678 2023-03-15 07:59:17.000000 QPUIQ-0.1.9/PUI/urwid/button.py
+-rw-r--r--   0 Bug        (504) staff       (20)      356 2023-03-16 07:54:05.000000 QPUIQ-0.1.9/PUI/urwid/label.py
+-rw-r--r--   0 Bug        (504) staff       (20)      734 2023-03-16 07:54:02.000000 QPUIQ-0.1.9/PUI/urwid/layout.py
+-rw-r--r--   0 Bug        (504) staff       (20)      462 2023-03-15 00:27:06.000000 QPUIQ-0.1.9/PUI/urwid/progressbar.py
+-rw-r--r--   0 Bug        (504) staff       (20)      674 2023-04-30 08:07:16.000000 QPUIQ-0.1.9/PUI/urwid/scroll.py
+-rw-r--r--   0 Bug        (504) staff       (20)      315 2023-04-29 19:07:06.000000 QPUIQ-0.1.9/PUI/urwid/window.py
+-rw-r--r--   0 Bug        (504) staff       (20)     2604 2023-04-30 15:11:41.000000 QPUIQ-0.1.9/PUI/view.py
+drwxr-xr-x   0 Bug        (504) staff       (20)        0 2023-05-01 15:14:04.670018 QPUIQ-0.1.9/QPUIQ.egg-info/
+-rw-r--r--   0 Bug        (504) staff       (20)     2889 2023-05-01 15:14:04.000000 QPUIQ-0.1.9/QPUIQ.egg-info/PKG-INFO
+-rw-r--r--   0 Bug        (504) staff       (20)     1315 2023-05-01 15:14:04.000000 QPUIQ-0.1.9/QPUIQ.egg-info/SOURCES.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        1 2023-05-01 15:14:04.000000 QPUIQ-0.1.9/QPUIQ.egg-info/dependency_links.txt
+-rw-r--r--   0 Bug        (504) staff       (20)        4 2023-05-01 15:14:04.000000 QPUIQ-0.1.9/QPUIQ.egg-info/top_level.txt
+-rw-r--r--   0 Bug        (504) staff       (20)     2629 2023-04-29 21:00:52.000000 QPUIQ-0.1.9/README.md
+-rw-r--r--   0 Bug        (504) staff       (20)       38 2023-05-01 15:14:04.670371 QPUIQ-0.1.9/setup.cfg
+-rw-r--r--   0 Bug        (504) staff       (20)      539 2023-04-29 10:19:13.000000 QPUIQ-0.1.9/setup.py
```

### Comparing `QPUIQ-0.1.8/LICENSE.txt` & `QPUIQ-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.8/PKG-INFO` & `QPUIQ-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QPUIQ
-Version: 0.1.8
+Version: 0.1.9
 Summary: "PUI" Python Declarative UI Framework
 Home-page: https://github.com/buganini/PUI
 Author: Buganini Chiu
 Author-email: buganini@b612.tw
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `QPUIQ-0.1.8/PUI/PySide6/base.py` & `QPUIQ-0.1.9/PUI/Qt5/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 from .. import *
-
-from PySide6 import QtCore, QtWidgets
+from PyQt5 import QtCore, QtWidgets
 
 class QtViewSignal(QtCore.QObject):
-    redraw = QtCore.Signal()
+    redraw = QtCore.pyqtSignal()
 
 class QPUIView(PUIView):
     def __init__(self):
         super().__init__()
         self.signal = QtViewSignal()
         self.signal.redraw.connect(self.update)
 
     def redraw(self):
         self.signal.redraw.emit()
 
 class QtBaseWidget(PUINode):
-    terminal = True
     def destroy(self):
         self.ui.deleteLater()
 
 class QtBaseLayout(PUINode):
     def addChild(self, idx, child):
         if isinstance(child, QtBaseLayout):
             self.ui.addLayout(child.ui)
         elif isinstance(child, QtBaseWidget):
             params = {}
             if not child.layout_weight is None:
                 params["stretch"] = child.layout_weight
             self.ui.addWidget(child.ui, **params)
-        elif child.children:
+        else:
             self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
         if isinstance(child, QtBaseLayout):
             self.ui.removeItem(child.ui)
         elif isinstance(child, QtBaseWidget):
             child.ui.setParent(None)
-        elif child.children:
+        else:
             self.removeChild(idx, child.children[0])
```

### Comparing `QPUIQ-0.1.8/PUI/PySide6/button.py` & `QPUIQ-0.1.9/PUI/PySide6/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.8/PUI/PySide6/canvas.py` & `QPUIQ-0.1.9/PUI/PySide6/canvas.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,45 +1,52 @@
 from .. import *
 from .base import *
 
-from PySide6 import QtWidgets
+from PySide6 import QtWidgets, QtGui
 from PySide6.QtGui import QPainter, QColor
 from PySide6.QtCore import QPoint
 
 class PUIQtCanvas(QtWidgets.QWidget):
     def __init__(self, puinode, width=None, height=None):
         self.puinode = puinode
         self.width = width
         self.height = height
         super().__init__()
 
-    def sizeHint(self):
+    def minimumSizeHint(self):
         return QtCore.QSize(self.width, self.height)
 
     def paintEvent(self, event):
         qpainter = QPainter()
         qpainter.begin(self)
 
+        if not self.puinode.bgColor is None:
+            bgBrush = QtGui.QBrush()
+            bgBrush.setColor(QtGui.QColor(self.puinode.bgColor))
+            bgBrush.setStyle(QtCore.Qt.SolidPattern)
+            rect = QtCore.QRect(0, 0, qpainter.device().width, qpainter.device().height)
+            qpainter.fillRect(rect, bgBrush)
+
         for c in self.puinode.children:
             c.draw(qpainter)
 
         qpainter.end()
 
 class QtCanvas(QtBaseWidget):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self, bgColor=None):
+        super().__init__()
         self.ui = None
+        self.bgColor = bgColor
 
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
             self.ui.puinode = self
         else:
             self.ui = PUIQtCanvas(self, self.layout_width or 0, self.layout_height or 0)
-        self.ui.resize(self.layout_width or 0, self.layout_height or 0)
         self.ui.update()
 
 class QtCanvasText(PUINode):
     def __init__(self, x, y, text):
         super().__init__()
         self.x = x
         self.y = y
```

### Comparing `QPUIQ-0.1.8/PUI/PySide6/layout.py` & `QPUIQ-0.1.9/PUI/Qt5/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from .base import *
 
 class QtHBox(QtBaseLayout):
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
-            from PySide6 import QtWidgets
+            from PyQt5 import QtWidgets
             self.ui = QtWidgets.QHBoxLayout()
             self.ui.setObjectName(self.key)
 
 class QtVBox(QtBaseLayout):
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
```

### Comparing `QPUIQ-0.1.8/PUI/PySide6/textfield.py` & `QPUIQ-0.1.9/PUI/PySide6/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.8/PUI/PySide6/window.py` & `QPUIQ-0.1.9/PUI/Qt5/window.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         self.title = title
         self.size = size
 
     def update(self, prev=None):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
-            from PySide6 import QtWidgets
+            from PyQt5 import QtWidgets
             self.ui = QtWidgets.QWidget()
             self.ui.setObjectName("Window")
             self.box = QtWidgets.QBoxLayout(QtWidgets.QBoxLayout.Direction.LeftToRight)
             self.ui.setLayout(self.box)
 
         if not self.title is None:
             self.ui.setWindowTitle(self.title)
```

### Comparing `QPUIQ-0.1.8/PUI/Qt5/base.py` & `QPUIQ-0.1.9/PUI/tkinter/layout.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,49 @@
 from .. import *
-from PyQt5 import QtCore, QtWidgets
+from .base import *
 
-class QtViewSignal(QtCore.QObject):
-    redraw = QtCore.pyqtSignal()
+class TkHBox(TkBaseWidget):
+    def update(self, prev):
+        if prev and hasattr(prev, "ui"):
+            self.ui = prev.ui
+        else:
+            self.ui = tk.Frame(self.tkparent.inner)
+            self.ui.rowconfigure(0, weight=1)
 
-class QPUIView(PUIView):
-    def __init__(self):
-        super().__init__()
-        self.signal = QtViewSignal()
-        self.signal.redraw.connect(self.update)
+    def addChild(self, idx, child):
+        if isinstance(child, TkBaseWidget):
+            child.ui.grid(row=0, column=idx, sticky='nsew')
+            if not child.layout_weight is None:
+                self.ui.columnconfigure(idx, weight=child.layout_weight)
+        elif child.children:
+            self.addChild(idx, child.children[0])
 
-    def redraw(self):
-        self.signal.redraw.emit()
+    def removeChild(self, idx, child):
+        if isinstance(child, TkBaseWidget):
+            child.ui.grid_forget()
+        elif child.children:
+            self.removeChild(idx, child.children[0])
 
-class QtBaseWidget(PUINode):
-    def destroy(self):
-        self.ui.deleteLater()
+class TkVBox(TkBaseWidget):
+    def update(self, prev):
+        if prev and hasattr(prev, "ui"):
+            self.ui = prev.ui
+        else:
+            self.ui = tk.Frame(self.tkparent.inner)
+            self.ui.config(bg="white")
+            self.ui.columnconfigure(0, weight=1)
 
-class QtBaseLayout(PUINode):
     def addChild(self, idx, child):
-        if isinstance(child, QtBaseLayout):
-            self.ui.addLayout(child.ui)
-        elif isinstance(child, QtBaseWidget):
-            params = {}
+        if isinstance(child, TkBaseWidget):
+            child.ui.grid(row=idx, column=0, sticky='nsew')
             if not child.layout_weight is None:
-                params["stretch"] = child.layout_weight
-            self.ui.addWidget(child.ui, **params)
-        else:
+                self.ui.rowconfigure(idx, weight=child.layout_weight)
+        elif child.children:
             self.addChild(idx, child.children[0])
 
     def removeChild(self, idx, child):
-        if isinstance(child, QtBaseLayout):
-            self.ui.removeItem(child.ui)
-        elif isinstance(child, QtBaseWidget):
-            child.ui.setParent(None)
-        else:
+        if isinstance(child, TkBaseWidget):
+            child.ui.grid_forget()
+        elif child.children:
             self.removeChild(idx, child.children[0])
+
+
```

### Comparing `QPUIQ-0.1.8/PUI/Qt5/button.py` & `QPUIQ-0.1.9/PUI/Qt5/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.8/PUI/Qt5/canvas.py` & `QPUIQ-0.1.9/PUI/Qt5/canvas.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.8/PUI/Qt5/layout.py` & `QPUIQ-0.1.9/PUI/PySide6/layout.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,18 +2,25 @@
 from .base import *
 
 class QtHBox(QtBaseLayout):
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
-            from PyQt5 import QtWidgets
+            from PySide6 import QtWidgets
             self.ui = QtWidgets.QHBoxLayout()
             self.ui.setObjectName(self.key)
 
 class QtVBox(QtBaseLayout):
     def update(self, prev):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
             self.ui = QtWidgets.QVBoxLayout()
             self.ui.setObjectName(self.key)
+
+class QtSpacerItem(QtBaseWidget):
+    def update(self, prev):
+        if prev and hasattr(prev, "ui"):
+            self.ui = prev.ui
+        else:
+            self.ui = QtWidgets.QSpacerItem(0, 0, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
```

### Comparing `QPUIQ-0.1.8/PUI/Qt5/textfield.py` & `QPUIQ-0.1.9/PUI/Qt5/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.8/PUI/Qt5/window.py` & `QPUIQ-0.1.9/PUI/PySide6/window.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from .. import *
 from .base import *
 
-class QtWindow(PUINode):
+class QtWindow(QtBaseWidget):
+    terminal = False
+
     def __init__(self, title=None, size=None):
         super().__init__()
         self.title = title
         self.size = size
 
     def update(self, prev=None):
         if prev and hasattr(prev, "ui"):
             self.ui = prev.ui
         else:
-            from PyQt5 import QtWidgets
+            from PySide6 import QtWidgets
             self.ui = QtWidgets.QWidget()
             self.ui.setObjectName("Window")
             self.box = QtWidgets.QBoxLayout(QtWidgets.QBoxLayout.Direction.LeftToRight)
             self.ui.setLayout(self.box)
 
         if not self.title is None:
             self.ui.setWindowTitle(self.title)
```

### Comparing `QPUIQ-0.1.8/PUI/dom.py` & `QPUIQ-0.1.9/PUI/dom.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.8/PUI/flet/application.py` & `QPUIQ-0.1.9/PUI/flet/application.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.8/PUI/flet/button.py` & `QPUIQ-0.1.9/PUI/flet/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.8/PUI/flet/layout.py` & `QPUIQ-0.1.9/PUI/flet/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.8/PUI/flet/textfield.py` & `QPUIQ-0.1.9/PUI/flet/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.8/PUI/node.py` & `QPUIQ-0.1.9/PUI/node.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
         if not hasattr(self, "name"):
             self.name = None
 
         self.layout_weight = None
         self.layout_width = None
         self.layout_height = None
+        self.layout_params = {}
 
         self.ui = None
         self.args = args
         try:
             self.root = find_puiview()
             self.parent = self.root.frames[-1]
         except PuiViewNotFoundError:
@@ -42,26 +43,33 @@
         if self.parent is self:
             self.path = tuple()
         else:
             self.path = self.parent.path + tuple([len(self.parent.children)])
             self.parent.children.append(self)
         # print(type(self).__name__, self.path, "parent=", self.parent.path)
 
-
     def __enter__(self):
         # print("enter", type(self).__name__, id(self))
         self.root.frames.append(self)
         return self
 
     def __exit__(self, ex_type, value, traceback):
         # print("exit", type(self).__name__, id(self))
         self.root.frames.pop()
         if ex_type is None: # don't consume exception
             return self
 
+    @property
+    def inner(self):
+        return self.ui
+
+    @property
+    def outer(self):
+        return self.ui
+
     def comment(self):
         return None
 
     def update(self, prev):
         return None
 
     def destroy(self):
@@ -100,15 +108,19 @@
             if i > 0:
                 segs.append(",\n")
             segs.append(c.__repr__())
         segs.append("\n")
         segs.append("".join(["  "*len(self.path), "}"]))
         return "".join(segs)
 
-    def layout(self, width=None, height=None, weight=None):
+    def layout(self, width=None, height=None, weight=None, **kwargs):
         if not width is None:
             self.layout_width = width
         if not height is None:
             self.layout_height = height
         if not weight is None:
             self.layout_weight = weight
+
+        for k,v in kwargs.items():
+            self.layout_params[k] = v
+
         return self
```

### Comparing `QPUIQ-0.1.8/PUI/state.py` & `QPUIQ-0.1.9/PUI/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
             view = find_puiview()
             self.__listeners.add(view)
         except PuiViewNotFoundError:
             pass
         return self.__values[key]
 
     def __setitem__(self, key, value):
-        if key >= len (self.values) or self.__values[key] != value:
+        if key >= len (self.__values) or self.__values[key] != value:
             self.__values[key] = value
             for l in self.__listeners:
                 l.redraw()
 
     def __len__(self):
         try:
             view = find_puiview()
@@ -306,21 +306,21 @@
         try:
             view = find_puiview()
             self.__listeners.add(view)
         except PuiViewNotFoundError:
             pass
         return self.__values.keys()
 
-    def pop(self, key):
+    def pop(self, key, default=None):
         try:
             view = find_puiview()
             self.__listeners.add(view)
         except PuiViewNotFoundError:
             pass
-        r = self.__values.pop(key)
+        r = self.__values.pop(key, default)
         for l in self.__listeners:
             l.redraw()
         return r
 
     def setdefault(self, key, default=None):
         try:
             view = find_puiview()
```

### Comparing `QPUIQ-0.1.8/PUI/timeline.py` & `QPUIQ-0.1.9/PUI/timeline.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.8/PUI/tkinter/application.py` & `QPUIQ-0.1.9/PUI/tkinter/application.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.8/PUI/tkinter/base.py` & `QPUIQ-0.1.9/PUI/tkinter/base.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.8/PUI/tkinter/button.py` & `QPUIQ-0.1.9/PUI/tkinter/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.8/PUI/tkinter/textfield.py` & `QPUIQ-0.1.9/PUI/tkinter/textfield.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.8/PUI/tkinter/window.py` & `QPUIQ-0.1.9/PUI/tkinter/window.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.8/PUI/urwid/application.py` & `QPUIQ-0.1.9/PUI/urwid/application.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.8/PUI/urwid/button.py` & `QPUIQ-0.1.9/PUI/urwid/button.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.8/PUI/urwid/layout.py` & `QPUIQ-0.1.9/PUI/urwid/layout.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.8/PUI/view.py` & `QPUIQ-0.1.9/PUI/view.py`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.8/QPUIQ.egg-info/PKG-INFO` & `QPUIQ-0.1.9/QPUIQ.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QPUIQ
-Version: 0.1.8
+Version: 0.1.9
 Summary: "PUI" Python Declarative UI Framework
 Home-page: https://github.com/buganini/PUI
 Author: Buganini Chiu
 Author-email: buganini@b612.tw
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `QPUIQ-0.1.8/QPUIQ.egg-info/SOURCES.txt` & `QPUIQ-0.1.9/QPUIQ.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 PUI/PySide6/application.py
 PUI/PySide6/base.py
 PUI/PySide6/button.py
 PUI/PySide6/canvas.py
 PUI/PySide6/label.py
 PUI/PySide6/layout.py
 PUI/PySide6/progressbar.py
+PUI/PySide6/scroll.py
 PUI/PySide6/textfield.py
 PUI/PySide6/window.py
 PUI/Qt5/__init__.py
 PUI/Qt5/application.py
 PUI/Qt5/base.py
 PUI/Qt5/button.py
 PUI/Qt5/canvas.py
@@ -41,21 +42,23 @@
 PUI/tkinter/application.py
 PUI/tkinter/base.py
 PUI/tkinter/button.py
 PUI/tkinter/canvas.py
 PUI/tkinter/label.py
 PUI/tkinter/layout.py
 PUI/tkinter/progressbar.py
+PUI/tkinter/scroll.py
 PUI/tkinter/textfield.py
 PUI/tkinter/window.py
 PUI/urwid/__init__.py
 PUI/urwid/application.py
 PUI/urwid/base.py
 PUI/urwid/button.py
 PUI/urwid/label.py
 PUI/urwid/layout.py
 PUI/urwid/progressbar.py
+PUI/urwid/scroll.py
 PUI/urwid/window.py
 QPUIQ.egg-info/PKG-INFO
 QPUIQ.egg-info/SOURCES.txt
 QPUIQ.egg-info/dependency_links.txt
 QPUIQ.egg-info/top_level.txt
```

### Comparing `QPUIQ-0.1.8/README.md` & `QPUIQ-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `QPUIQ-0.1.8/setup.py` & `QPUIQ-0.1.9/setup.py`

 * *Files identical despite different names*

