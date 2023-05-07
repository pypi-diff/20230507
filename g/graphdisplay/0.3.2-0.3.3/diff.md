# Comparing `tmp/graphdisplay-0.3.2.tar.gz` & `tmp/graphdisplay-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphdisplay-0.3.2.tar", last modified: Sat May  6 17:32:44 2023, max compression
+gzip compressed data, was "graphdisplay-0.3.3.tar", last modified: Sun May  7 19:46:29 2023, max compression
```

## Comparing `graphdisplay-0.3.2.tar` & `graphdisplay-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 17:32:44.443505 graphdisplay-0.3.2/
--rw-rw-rw-   0        0        0     5408 2023-05-06 17:32:44.442554 graphdisplay-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     4753 2023-05-06 17:15:34.000000 graphdisplay-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 17:32:44.428066 graphdisplay-0.3.2/graphdisplay/
--rw-rw-rw-   0        0        0       60 2023-05-03 20:40:03.000000 graphdisplay-0.3.2/graphdisplay/__init__.py
--rw-rw-rw-   0        0        0      114 2023-05-06 17:02:49.000000 graphdisplay-0.3.2/graphdisplay/general_config.py
--rw-rw-rw-   0        0        0     3483 2023-05-06 17:26:05.000000 graphdisplay-0.3.2/graphdisplay/graph.py
--rw-rw-rw-   0        0        0    15740 2023-05-06 17:31:26.000000 graphdisplay-0.3.2/graphdisplay/graphdisplay.py
--rw-rw-rw-   0        0        0     4904 2023-05-06 17:29:34.000000 graphdisplay-0.3.2/graphdisplay/json_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-06 17:32:44.441003 graphdisplay-0.3.2/graphdisplay/store/
--rw-rw-rw-   0        0        0        0 2023-05-06 17:02:49.000000 graphdisplay-0.3.2/graphdisplay/store/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 17:32:44.440006 graphdisplay-0.3.2/graphdisplay.egg-info/
--rw-rw-rw-   0        0        0     5408 2023-05-06 17:32:44.000000 graphdisplay-0.3.2/graphdisplay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-05-06 17:32:44.000000 graphdisplay-0.3.2/graphdisplay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 17:32:44.000000 graphdisplay-0.3.2/graphdisplay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-06 17:32:44.000000 graphdisplay-0.3.2/graphdisplay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 17:32:44.443505 graphdisplay-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1322 2023-05-06 17:32:42.000000 graphdisplay-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 19:46:29.419618 graphdisplay-0.3.3/
+-rw-rw-rw-   0        0        0     5408 2023-05-07 19:46:29.418620 graphdisplay-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4753 2023-05-06 17:15:34.000000 graphdisplay-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 19:46:29.406652 graphdisplay-0.3.3/graphdisplay/
+-rw-rw-rw-   0        0        0       60 2023-05-03 20:40:03.000000 graphdisplay-0.3.3/graphdisplay/__init__.py
+-rw-rw-rw-   0        0        0     2440 2023-05-07 19:37:48.000000 graphdisplay-0.3.3/graphdisplay/general_config.py
+-rw-rw-rw-   0        0        0    17455 2023-05-07 10:31:30.000000 graphdisplay-0.3.3/graphdisplay/graph.py
+-rw-rw-rw-   0        0        0    17579 2023-05-07 19:42:11.000000 graphdisplay-0.3.3/graphdisplay/graphdisplay.py
+-rw-rw-rw-   0        0        0     7108 2023-05-07 19:37:48.000000 graphdisplay-0.3.3/graphdisplay/json_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-07 19:46:29.417623 graphdisplay-0.3.3/graphdisplay/store/
+-rw-rw-rw-   0        0        0        0 2023-05-06 17:02:49.000000 graphdisplay-0.3.3/graphdisplay/store/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 19:46:29.416626 graphdisplay-0.3.3/graphdisplay.egg-info/
+-rw-rw-rw-   0        0        0     5408 2023-05-07 19:46:29.000000 graphdisplay-0.3.3/graphdisplay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-05-07 19:46:29.000000 graphdisplay-0.3.3/graphdisplay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 19:46:29.000000 graphdisplay-0.3.3/graphdisplay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-07 19:46:29.000000 graphdisplay-0.3.3/graphdisplay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 19:46:29.419618 graphdisplay-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1322 2023-05-07 19:46:27.000000 graphdisplay-0.3.3/setup.py
```

### Comparing `graphdisplay-0.3.2/PKG-INFO` & `graphdisplay-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphdisplay
-Version: 0.3.2
+Version: 0.3.3
 Summary: Librería para representar visualmente grafos de tipo diccionario
 Home-page: https://github.com/seniorbeto
 Author: Alberto Penas Díaz
 Author-email: albertopenasdiaz@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `graphdisplay-0.3.2/README.md` & `graphdisplay-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.3.2/graphdisplay/graphdisplay.py` & `graphdisplay-0.3.3/graphdisplay/graphdisplay.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 from .json_manager import JsonManager
 from .general_config import *
 
 class GraphGUI:
 
     instance = 0
 
-    def __new__(cls, graph, node_radius: int = 40, scr_width: int = 600, scr_height: int = 600):
+    def __new__(cls, graph, node_radius: int = 40, scr_width: int = 600, scr_height: int = 600, theme: str = 'BROWN'):
         GraphGUI.instance += 1
-        return GraphGUI.__GraphGUI(graph, GraphGUI.instance, node_radius, scr_width, scr_height)
+        if GraphGUI.instance > 5:
+            raise Exception("For safety reasons, only five instances of GraphGUI can be created")
+        return GraphGUI.__GraphGUI(graph, GraphGUI.instance, node_radius, scr_width, scr_height, theme)
 
     def __getattr__(self, name):
         return getattr(self.instance, name)
 
     def __setattr__(self, name, value):
         return setattr(self.instance, name, value)
 
     class __GraphGUI:
-        def __init__(self, graph, instance, node_radius: int = 40, scr_width: int = 600, scr_height: int = 600):
+        def __init__(self, graph, instance, node_radius: int = 40, scr_width: int = 600, scr_height: int = 600, theme: str = 'BROWN'):
             """
             Creates a GraphGUI object, which will display the graph in a external window. Nodes can be moved with the mouse.
             The creation of the window will stop the execution of the program until the window is closed. Thus, it is recommended
             to create the GraphGUI object at the end of the program.
             :param graph: The graph to be displayed
             :param node_radius: The radius of the nodes (default 40)
             :param scr_width: The width of the window (default 600)
@@ -42,74 +44,94 @@
             self.__ACTUAL_INSTANCE = instance
             self.__graph = graph
             self.__node_radius = node_radius
             self.__scr_width = scr_width
             self.__scr_height = scr_height
             self.__XMARGIN = 7
             self.__YMARGIN = 7
+            self._theme = theme.upper()
             self.nodes = []
             self.edges = []
+            try:
+                self._BACKGROUND_CANVAS_COLOR = THEMES[theme.upper()]['BACKGROUND_CANVAS_COLOR']
+                self._BUTTON_COLOR = THEMES[theme.upper()]['BUTTON_COLOR']
+                self._FRAME_COLOR = THEMES[theme.upper()]['FRAME_COLOR']
+                self._VERTEX_COLOR = THEMES[theme.upper()]['VERTEX_COLOR']
+                self._AUTHOR_NAME_COLOR = THEMES[theme.upper()]['AUTHOR_NAME_COLOR']
+            except KeyError:
+                raise ValueError("The theme must be one of the following: " + str(list(THEMES.keys())))
 
             # create the main window and start the GUI
             self.root = tk.Tk()
             self.root.title('GraphGUI')
             self.root.resizable(False, False)
-            self.root.configure(bg=FRAME_COLOR, border=0, width=self.__scr_width, height=self.__scr_height)
+            self.root.configure(bg=self._FRAME_COLOR, border=0, width=self.__scr_width, height=self.__scr_height)
 
             self.json_manager = JsonManager(self.root, self)
 
             # Closing protocol
             self.root.protocol("WM_DELETE_WINDOW", self.__on_closing)
 
-            self.canvas = tk.Canvas(self.root, bg=BACKGROUND_CANVAS_COLOR)
+            self.canvas = tk.Canvas(self.root, bg=self._BACKGROUND_CANVAS_COLOR, bd=0)
             self.canvas.place(x=self.__XMARGIN,
                               y=self.__YMARGIN,
                               width=self.__scr_width - self.__XMARGIN * 2,
                               height=self.__scr_height - self.__YMARGIN * 2 - 30)
 
             # Reset button
-            self.reset_button = tk.Button(self.root, text="Reset", bg=BUTTON_COLOR, command=self.display_reset)
+            self.reset_button = tk.Button(self.root, text="Reset", bg=self._BUTTON_COLOR, command=self.display_reset,
+                                          bd=0)
             self.reset_button.place(x=self.__XMARGIN, y=self.__scr_height-self.__YMARGIN//2-30, width=60, height=30)
 
             # Load button
-            self.load_button = tk.Button(self.root, text="Load", bg=BUTTON_COLOR, command=self.__call_manager_load)
+            self.load_button = tk.Button(self.root, text="Load", bg=self._BUTTON_COLOR, command=self.__call_manager_load,
+                                         bd=0)
             self.load_button.place(x=self.__XMARGIN + 60 + 7, y=self.__scr_height - self.__YMARGIN // 2 - 30, width=60,
                                     height=30)
 
             # Save button
-            self.save_button = tk.Button(self.root, text="Save", bg=BUTTON_COLOR, command=self.__call_manager_save)
+            self.save_button = tk.Button(self.root, text="Save", bg=self._BUTTON_COLOR, command=self.__call_manager_save,
+                                         bd=0)
             self.save_button.place(x=self.__XMARGIN + 60 + 60 + 7 + 7, y=self.__scr_height - self.__YMARGIN // 2 - 30, width=60,
                                     height=30)
 
+            # Delete button
+            self.save_button = tk.Button(self.root, text="Delete", bg=self._BUTTON_COLOR,
+                                         command=self.__call_manager_delete, bd=0)
+            self.save_button.place(x=self.__XMARGIN + 60 + 60 + 60 + 7 + 7 + 7,
+                                   y=self.__scr_height - self.__YMARGIN // 2 - 30,
+                                   width=60,
+                                   height=30)
+
             # Main display
-            data = self.json_manager.get_data('save'+str(self.__ACTUAL_INSTANCE))
+            data = self.json_manager.get_data('__last_store_'+str(self.__ACTUAL_INSTANCE))
             self.__display(data)
 
             self.canvas.tag_bind("movil", "<ButtonPress-1>", self.on_press)
             self.canvas.tag_bind("movil", "<Button1-Motion>", self.move)
             self.selected_node = None
 
             self.root.mainloop()
 
+        def __call_manager_delete(self):
+            self.json_manager.generate_delete_window()
+
         def __call_manager_load(self):
             new_position = self.json_manager.generate_load_window()
             if new_position:
                 self.display_reset(new_position)
 
         def __call_manager_save(self):
             curr_pos = {}
             for node in self.nodes:
                 curr_pos[node.id] = (node.pos_x, node.pos_y)
             self.json_manager.generate_save_window(curr_pos)
 
         def display_reset(self, new_data: dict = None):
-            for node in self.nodes:
-                node.terminate()
-            for edge in self.edges:
-                edge.terminate()
+            self.canvas.delete("all")
             self.__display(new_data)
 
         def __display(self, data: dict = None):
             # Preparation for the nodes display
             scr_center = (self.__scr_width // 2, self.__scr_height // 2)
             display_radius = min(self.__scr_width, self.__scr_height) // 2 - self.__node_radius - 10
             arch_angle = 360 / len(self.__graph._vertices)
@@ -123,45 +145,45 @@
                 if i == 0:
                     if data and str(vertex) in data and \
                             data[str(vertex)][0] < self.__scr_width and \
                             data[str(vertex)][1] < self.__scr_height - 30 and \
                             data[str(vertex)][0] + self.__node_radius*2 > 0 and \
                             data[str(vertex)][1] + self.__node_radius*2 > 0:
                         self.nodes.append(
-                            Node(self.canvas, self.__node_radius, data[str(vertex)][0], data[str(vertex)][1], text=vertex))
+                            Node(self.canvas, self.__node_radius, data[str(vertex)][0], data[str(vertex)][1], text=vertex, bg=self._VERTEX_COLOR))
                     else:
                         self.nodes.append(
-                            Node(self.canvas, self.__node_radius, first_node_pos[0], first_node_pos[1], text=vertex))
+                            Node(self.canvas, self.__node_radius, first_node_pos[0], first_node_pos[1], text=vertex, bg=self._VERTEX_COLOR))
                 else:
                     if data and str(vertex) in data and \
                             data[str(vertex)][0] < self.__scr_width and \
                             data[str(vertex)][1] < self.__scr_height - 30 and \
                             data[str(vertex)][0] + self.__node_radius*2 > 0 and \
                             data[str(vertex)][1] + self.__node_radius*2 > 0:
                         self.nodes.append(
-                            Node(self.canvas, self.__node_radius, data[str(vertex)][0], data[str(vertex)][1], text=vertex))
+                            Node(self.canvas, self.__node_radius, data[str(vertex)][0], data[str(vertex)][1], text=vertex, bg=self._VERTEX_COLOR))
                     else:
                         self.nodes.append(Node(self.canvas,
                                                self.__node_radius,
                                                int(scr_center[0] - self.__node_radius - display_radius * math.sin(
                                                    math.radians(angle))),
                                                int(scr_center[1] - self.__node_radius - display_radius * math.cos(
                                                    math.radians(angle))),
-                                               text=vertex))
+                                               text=vertex, bg=self._VERTEX_COLOR))
                 i += 1
                 angle += arch_angle
 
             # Create the edges
             i = 0
             self.edges = []
             for vertex in self.__graph._vertices:
                 for adj in self.__graph._vertices[vertex]:
                     for node in self.nodes:
                         if node.id == adj._vertex:
-                            self.edges.append(Edge(self.canvas, self.nodes[i], node, adj._weight if adj._weight else 1))
+                            self.edges.append(Edge(self.canvas, self.nodes[i], node, adj._weight if adj._weight else 1, window_color=self._BACKGROUND_CANVAS_COLOR))
                             node.asociated_edges_IN.append(self.edges[-1])
                             self.nodes[i].asociated_edges_OUT.append(self.edges[-1])
                 i += 1
 
             # Display the edges
             if self.__graph._directed:
                 for edge in self.edges:
@@ -177,22 +199,22 @@
                     if not found:
                         edge.show()
             else:
                 for edge in self.edges:
                     edge.show()
 
             # Display author
-            self.canvas.create_text(self.__scr_width // 2, self.__YMARGIN + 3, text="by @seniorbeto", fill=FRAME_COLOR,
-                                    font=("Courier", 10))
+            self.__autor = self.canvas.create_text(self.__scr_width // 2, self.__YMARGIN + 3, text="by @seniorbeto",
+                                                   fill=self._AUTHOR_NAME_COLOR, font=("Courier", 10))
 
         def __on_closing(self):
             data = {}
             for node in self.nodes:
                 data[node.id] = (node.pos_x, node.pos_y)
-            self.json_manager.save_data('save'+str(self.__ACTUAL_INSTANCE), data)
+            self.json_manager.save_data('__last_store_'+str(self.__ACTUAL_INSTANCE), data)
             self.root.destroy()
 
         def on_press(self, event):
             node = self.canvas.find_withtag(tk.CURRENT)
             self.selected_node = (node, event.x, event.y)
 
         def move(self, event):
@@ -203,43 +225,45 @@
                     self.canvas.move(i.circle, x - x0, y - y0)
                     self.canvas.move(i.text, x - x0, y - y0)
                     i.pos_x += x - x0
                     i.pos_y += y - y0
                     for edge in i.asociated_edges_IN:
                         edge_start = edge.start_node
                         weight = edge.weight
+                        color = edge.window_color
                         overlaped = edge.overlaped
                         i.asociated_edges_IN.remove(edge)
                         self.canvas.delete(edge.line)
                         self.canvas.delete(edge.window)
                         del edge
-                        edge = Edge(self.canvas, edge_start, i, weight, overlaped=overlaped)
+                        edge = Edge(self.canvas, edge_start, i, weight, overlaped=overlaped, window_color=color)
                         edge.show()
                         i.asociated_edges_IN.append(edge)
                     for adj in self.__graph._vertices[i.id]:
                         for nd in self.nodes:
                             if nd.id == adj._vertex:
                                 for edge in nd.asociated_edges_IN:
                                     if edge.start_node == i:
                                         edge_end = edge.end_node
+                                        color = edge.window_color
                                         weight = edge.weight
                                         overlaped = edge.overlaped
                                         nd.asociated_edges_IN.remove(edge)
                                         self.canvas.delete(edge.line)
                                         self.canvas.delete(edge.window)
                                         del edge
-                                        edge = Edge(self.canvas, i, edge_end, weight, overlaped=overlaped)
+                                        edge = Edge(self.canvas, i, edge_end, weight, overlaped=overlaped, window_color=color)
                                         edge.show()
                                         nd.asociated_edges_IN.append(edge)
 
 
             self.selected_node = (node, x, y)
 
 class Node:
-    def __init__(self, canvas: tk.Canvas, radius:int, posx: int, posy: int, text: str, bg: str = VERTEX_COLOR):
+    def __init__(self, canvas: tk.Canvas, radius:int, posx: int, posy: int, text: str, bg: str = "white"):
         self.asociated_edges_IN = []
         self.asociated_edges_OUT = []
         self.canvas = canvas
         self.id = text
         self.radius = radius
         self.pos_x = posx
         self.pos_y = posy
@@ -252,36 +276,37 @@
             edge.terminate()
         for edge in self.asociated_edges_OUT:
             edge.terminate()
         self.canvas.delete(self.circle)
         self.canvas.delete(self.text)
 
 class Edge:
-    def __init__(self, canvas: tk.Canvas, start: Node, end: Node, weight: int = 1, overlaped: bool = False):
+    def __init__(self, canvas: tk.Canvas, start: Node, end: Node, weight: int = 1, overlaped: bool = False, window_color: str = "white"):
         self.canvas = canvas
         self.overlaped = overlaped
         self.start_node = start
         self.end_node = end
         self.weight = weight
+        self.window_color = window_color
         self.start = self.__calculate_start(start, end)
         self.end = self.__calculate_end(start, end)
 
     def terminate(self):
         self.canvas.delete(self.line)
         self.canvas.delete(self.window)
 
     def show(self):
         self.line = self.canvas.create_line(self.start[0], self.start[1], self.end[0], self.end[1], arrow=tk.LAST, width=1.5)
         if not self.overlaped:
             self.window = self.canvas.create_window((self.start[0] + self.end[0]) // 2, (self.start[1] + self.end[1]) // 2,
-                                               window=tk.Label(self.canvas,bg=BACKGROUND_CANVAS_COLOR ,text=str(self.weight)))
+                                               window=tk.Label(self.canvas,bg=self.window_color ,text=str(self.weight)))
         else:
             self.window = self.canvas.create_window((self.start[0] * 0.2 + self.end[0] * 0.8),
                                                (self.start[1] * 0.2 + self.end[1] * 0.8),
-                                               window=tk.Label(self.canvas, bg=BACKGROUND_CANVAS_COLOR, text=str(self.weight)))
+                                               window=tk.Label(self.canvas, bg=self.window_color, text=str(self.weight)))
 
     def __calculate_start(self, start: Node, end: Node) -> tuple:
         """
         It calculates the initial position of the arrow that connects the nodes "start" and "end"
         :param start: Node
         :param end: Node
         :return: tuple with the initial position of the arrow
```

### Comparing `graphdisplay-0.3.2/graphdisplay/json_manager.py` & `graphdisplay-0.3.3/graphdisplay/json_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import os
 import json
 import tkinter as tk
 from tkinter import messagebox
-from tkinter import ttk
 from datetime import datetime
-from .general_config import *
 
 class JsonManager:
     def __init__(self, parent, graphgui):
         self.__JSON_SAVE_DIR = os.path.join(os.path.dirname(__file__), 'store/')
 
         self.graphgui = graphgui
         self.__parent = parent
@@ -21,14 +19,19 @@
         except FileNotFoundError:
             self.__permanent = {}
 
     def update_permanent(self):
         with open(self.__JSON_SAVE_DIR + '../permanent.json', "w", encoding="utf-8", newline="") as file:
             json.dump(self.__permanent, file, indent=4)
 
+    def delete_permanent(self, name: str):
+        del self.__permanent[name]
+        os.remove(self.__JSON_SAVE_DIR + name + '.json')
+        self.update_permanent()
+
     def add_permanent(self, name: str):
         self.__permanent[name] = str(datetime.now())
         self.update_permanent()
 
     def get_data(self, file_name: str) -> dict:
         try:
             with open(self.__JSON_SAVE_DIR + file_name + '.json', "r", encoding="utf-8", newline="") as file:
@@ -45,39 +48,79 @@
 
     def generate_save_window(self, current_position: dict):
         SaveWindow(self.__parent, self, current_position)
 
     def generate_load_window(self):
         LoadWindow(self.__parent, self)
 
+    def generate_delete_window(self):
+        DeleteWindow(self.__parent, self)
+
+class DeleteWindow(tk.Toplevel):
+    def __init__(self, root, json_manager: JsonManager):
+        super().__init__(root)
+        self.title("Delete save")
+        self.geometry("200x100")
+        self.resizable(False, False)
+        self.__manager = json_manager
+        self.configure(background=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
+
+        self.__label = tk.Label(self, text="Select save:", bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
+        self.__label.pack(side=tk.TOP)
+
+        options = list(self.__manager._JsonManager__permanent.keys())
+        if len(options) > 0:
+            self.__selecion = tk.StringVar(self)
+            self.__selecion.set(options[0])
+            self.__option_menu = tk.OptionMenu(self, self.__selecion, *options)
+            self.__option_menu.config(bg=self.__manager.graphgui._BUTTON_COLOR)
+            self.__option_menu.pack(side=tk.TOP)
+
+            self.__button = tk.Button(self, text="Delete", command=self.__on_delete, bg=self.__manager.graphgui._BUTTON_COLOR)
+            self.__button.place(x=0+7, y=100-7-30, width=60, height=30)
+
+            self.__button2 = tk.Button(self, text="Cancel", command=self.__on_cancel, bg=self.__manager.graphgui._BUTTON_COLOR)
+            self.__button2.place(x=200-7-60, y=100-7-30, width=60, height=30)
+
+    def __on_delete(self):
+        selection = self.__selecion.get()
+        if selection not in self.__manager._JsonManager__permanent:
+            messagebox.showerror("Error", "The selected save does not exist")
+            self.destroy()
+        self.__manager.delete_permanent(selection)
+        messagebox.showinfo("Confirm", f"Removed : {selection}")
+        self.destroy()
+
+    def __on_cancel(self):
+        self.destroy()
 
 class LoadWindow(tk.Toplevel):
     def __init__(self, root, json_manager: JsonManager):
         super().__init__(root)
         self.title("Load")
         self.geometry("200x100")
         self.resizable(False, False)
-        self.configure(background=BACKGROUND_CANVAS_COLOR)
         self.__manager = json_manager
+        self.configure(background=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
 
-        self.__label = tk.Label(self, text="Select save:", bg=BACKGROUND_CANVAS_COLOR)
+        self.__label = tk.Label(self, text="Select save:", bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
         self.__label.pack(side=tk.TOP)
 
         options = list(self.__manager._JsonManager__permanent.keys())
         if len(options) > 0:
             self.__selecion = tk.StringVar(self)
             self.__selecion.set(options[0])
             self.__option_menu = tk.OptionMenu(self, self.__selecion, *options)
-            self.__option_menu.config(bg=BUTTON_COLOR)
+            self.__option_menu.config(bg=self.__manager.graphgui._BUTTON_COLOR)
             self.__option_menu.pack(side=tk.TOP)
 
-            self.__button = tk.Button(self, text="Load", command=self.__on_load, bg=BUTTON_COLOR)
+            self.__button = tk.Button(self, text="Load", command=self.__on_load, bg=self.__manager.graphgui._BUTTON_COLOR)
             self.__button.place(x=0+7, y=100-7-30, width=60, height=30)
 
-            self.__button2 = tk.Button(self, text="Cancel", command=self.__on_cancel, bg=BUTTON_COLOR)
+            self.__button2 = tk.Button(self, text="Cancel", command=self.__on_cancel, bg=self.__manager.graphgui._BUTTON_COLOR)
             self.__button2.place(x=200-7-60, y=100-7-30, width=60, height=30)
 
     def __on_load(self):
         selection = self.__selecion.get()
         if selection not in self.__manager._JsonManager__permanent:
             messagebox.showerror("Error", "The selected save does not exist")
             self.destroy()
@@ -89,29 +132,29 @@
 
 class SaveWindow(tk.Toplevel):
     def __init__(self, root, json_manager: JsonManager, graph_position: dict):
         super().__init__(root)
         self.title("Save")
         self.geometry("200x100")
         self.resizable(False, False)
-        self.configure(bg=BACKGROUND_CANVAS_COLOR)
         self.__current_position = graph_position
         self.__manager = json_manager
+        self.configure(bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
         self.__root = root
 
-        self.__label = tk.Label(self, text="Save as:", bg=BACKGROUND_CANVAS_COLOR)
+        self.__label = tk.Label(self, text="Save as:", bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
         self.__label.pack(side=tk.TOP)
 
         self.__entry = tk.Entry(self)
         self.__entry.pack(side=tk.TOP)
 
-        self.__button = tk.Button(self, text="Save", command=self.__on_save, bg=BUTTON_COLOR)
+        self.__button = tk.Button(self, text="Save", command=self.__on_save, bg=self.__manager.graphgui._BUTTON_COLOR)
         self.__button.place(x=0+7, y=100-7-30, width=60, height=30)
 
-        self.__button2 = tk.Button(self, text="Cancel", command=self.__on_cancel, bg=BUTTON_COLOR)
+        self.__button2 = tk.Button(self, text="Cancel", command=self.__on_cancel, bg=self.__manager.graphgui._BUTTON_COLOR)
         self.__button2.place(x=200-7-60, y=100-7-30, width=60, height=30)
 
     def __on_save(self):
         word = self.__entry.get()
         word = word.strip()
         word = word.replace(" ", "_")
         if word:
```

### Comparing `graphdisplay-0.3.2/graphdisplay.egg-info/PKG-INFO` & `graphdisplay-0.3.3/graphdisplay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphdisplay
-Version: 0.3.2
+Version: 0.3.3
 Summary: Librería para representar visualmente grafos de tipo diccionario
 Home-page: https://github.com/seniorbeto
 Author: Alberto Penas Díaz
 Author-email: albertopenasdiaz@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `graphdisplay-0.3.2/setup.py` & `graphdisplay-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.3.2'
+VERSION = '0.3.3'
 PACKAGE_NAME = 'graphdisplay'
 AUTHOR = 'Alberto Penas Díaz'
 AUTHOR_EMAIL = 'albertopenasdiaz@gmail.com'
 URL = 'https://github.com/seniorbeto'
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = 'Librería para representar visualmente grafos de tipo diccionario'
```

