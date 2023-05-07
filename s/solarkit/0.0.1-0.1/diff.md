# Comparing `tmp/solarkit-0.0.1.tar.gz` & `tmp/solarkit-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solarkit-0.0.1.tar", last modified: Sat May  6 20:22:36 2023, max compression
+gzip compressed data, was "solarkit-0.1.tar", last modified: Sun May  7 17:19:23 2023, max compression
```

## Comparing `solarkit-0.0.1.tar` & `solarkit-0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 20:22:36.183603 solarkit-0.0.1/
--rw-rw-rw-   0        0        0     1092 2023-05-01 11:48:54.000000 solarkit-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1407 2023-05-06 20:22:36.183101 solarkit-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      807 2023-05-06 20:21:46.000000 solarkit-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-06 20:22:36.184101 solarkit-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1057 2023-05-06 20:22:34.000000 solarkit-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 20:22:36.176600 solarkit-0.0.1/solarkit/
--rw-rw-rw-   0        0        0      117 2023-05-01 16:29:31.000000 solarkit-0.0.1/solarkit/__init__.py
--rw-rw-rw-   0        0        0     3597 2023-05-02 16:04:11.000000 solarkit-0.0.1/solarkit/planet.py
--rw-rw-rw-   0        0        0     2867 2023-05-06 19:41:16.000000 solarkit-0.0.1/solarkit/solar_system.py
--rw-rw-rw-   0        0        0     2268 2023-05-06 20:16:20.000000 solarkit-0.0.1/solarkit/utils.py
--rw-rw-rw-   0        0        0    12381 2023-05-06 19:41:07.000000 solarkit-0.0.1/solarkit/viewer.py
-drwxrwxrwx   0        0        0        0 2023-05-06 20:22:36.182103 solarkit-0.0.1/solarkit.egg-info/
--rw-rw-rw-   0        0        0     1407 2023-05-06 20:22:36.000000 solarkit-0.0.1/solarkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-05-06 20:22:36.000000 solarkit-0.0.1/solarkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 20:22:36.000000 solarkit-0.0.1/solarkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-06 20:22:36.000000 solarkit-0.0.1/solarkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-06 20:22:36.000000 solarkit-0.0.1/solarkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 17:19:23.821237 solarkit-0.1/
+-rw-rw-rw-   0        0        0     1092 2023-05-01 11:48:54.000000 solarkit-0.1/LICENSE
+-rw-rw-rw-   0        0        0     1654 2023-05-07 17:19:23.820238 solarkit-0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1055 2023-05-07 17:17:01.000000 solarkit-0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-07 17:19:23.821237 solarkit-0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1051 2023-05-07 17:09:44.000000 solarkit-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 17:19:23.813240 solarkit-0.1/solarkit/
+-rw-rw-rw-   0        0        0      117 2023-05-01 16:29:31.000000 solarkit-0.1/solarkit/__init__.py
+-rw-rw-rw-   0        0        0     3597 2023-05-02 16:04:11.000000 solarkit-0.1/solarkit/planet.py
+-rw-rw-rw-   0        0        0     2867 2023-05-06 19:41:16.000000 solarkit-0.1/solarkit/solar_system.py
+-rw-rw-rw-   0        0        0     2072 2023-05-07 16:25:21.000000 solarkit-0.1/solarkit/utils.py
+-rw-rw-rw-   0        0        0    11888 2023-05-07 17:04:12.000000 solarkit-0.1/solarkit/viewer.py
+drwxrwxrwx   0        0        0        0 2023-05-07 17:19:23.819238 solarkit-0.1/solarkit.egg-info/
+-rw-rw-rw-   0        0        0     1654 2023-05-07 17:19:23.000000 solarkit-0.1/solarkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-05-07 17:19:23.000000 solarkit-0.1/solarkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 17:19:23.000000 solarkit-0.1/solarkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-07 17:19:23.000000 solarkit-0.1/solarkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-07 17:19:23.000000 solarkit-0.1/solarkit.egg-info/top_level.txt
```

### Comparing `solarkit-0.0.1/LICENSE` & `solarkit-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `solarkit-0.0.1/PKG-INFO` & `solarkit-0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: solarkit
-Version: 0.0.1
+Version: 0.1
 Summary: Visualise a solar system and do cool stuff with it
 Author: Carlos Lorenzo
 Author-email: <clorenzozuniga@gmail.com>
 Keywords: solar system,space,astrophysics,bpho
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -17,19 +17,25 @@
 
 # solarkit - BPhO Computational challenge
 ## A tool to easily visualise and perform calculation on a solar system. The solutions for all challenges are embed but also provides the tools to tinker around and build new, original simulations
 
 It was built as the first part of a two part subimission for the challenge. My idea is to create a website using django to allow anyone to use the simulation. Having this package will ensure clean, backend code that will do the work in just a couple of lines.
 
 ### Challenges
+* Kepler's Third Law
 * Visualise a solar system
 * Visualise the solar system, animated
 * Spinograph
 * Heliocentric model
 
 ### Personal aditions
 * Tools to create, save & load a custom solar system
 * Save the model output to an image
 * Spinograph, animated
 
 ### How to use
-1. pip install solarkit
+1. pip install solarkit
+2. create .py file
+3. start experimenting! (follow example image for guidance)
+
+### Use example
+![solarkit_example](https://user-images.githubusercontent.com/91377173/236692357-7e14751b-2e94-4a01-894f-2202fef1e30d.jpg)
```

### Comparing `solarkit-0.0.1/setup.py` & `solarkit-0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.1"
+VERSION = "0.1"
 DESCRIPTION = "Visualise a solar system and do cool stuff with it"
 
 # Setting up
 setup(
     name="solarkit",
     version=VERSION,
     author="Carlos Lorenzo",
@@ -19,15 +19,15 @@
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=["numpy", "pandas", "matplotlib"],
     keywords=["solar system", "space", "astrophysics", "bpho"],
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Education",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

### Comparing `solarkit-0.0.1/solarkit/planet.py` & `solarkit-0.1/solarkit/planet.py`

 * *Files identical despite different names*

### Comparing `solarkit-0.0.1/solarkit/solar_system.py` & `solarkit-0.1/solarkit/solar_system.py`

 * *Files identical despite different names*

### Comparing `solarkit-0.0.1/solarkit/utils.py` & `solarkit-0.1/solarkit/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import pickle
-import os
 
 import pandas as pd
-import matplotlib.pyplot as plt
 
 from planet import Planet
 from solar_system import Solar_System
 
 
 def create_planet(planet_data: pd.Series(object)) -> Planet:
     
@@ -47,19 +45,15 @@
         # If a is smaller than 0, simulation would break trying to draw it. It is a sun, it will be manually added during the simulation
         
         system.add(create_planet(planet_data=planet_data))
         
     return system
 
 
-def save_figure(name: str) -> None:
-    if not os.path.exists("figures"):
-        os.mkdir("figures")
-        
-    plt.savefig(f"figures/{name}", dpi=250)
+
 
 
 def save_system(model: Solar_System) -> None:
     """
     Serialises Solar_System object with pickle
 
     Args:
```

### Comparing `solarkit-0.0.1/solarkit/viewer.py` & `solarkit-0.1/solarkit/viewer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from dataclasses import dataclass, field
 from typing import Optional, List, Dict
-
+import os
 
 import matplotlib.pyplot as plt
 import numpy as np
 
-
-import utils
-
 from solar_system import Solar_System
 from planet import Planet
 
 
 @dataclass
 class Viewer:
     """
@@ -48,38 +45,91 @@
         
         self.system.planets = dict(sorted(self.system.planets.items(), key=lambda planet: planet[1].P))
         
         self.chosen_planets = list(map(self.system.planets.get, self.planets_to_use))
         
         self.orbit_data = [planet.compute_orbit(compute_3D=self.compute_3D) for planet in self.chosen_planets]
 
-        
+    
         
         self.tmax = 4 * self.chosen_planets[-1].P
         self.dt = self.tmax/2500
         
+    def __str__(self) -> str:
+        return f"Planets: {self.system.__str__()}\n3D: {self.compute_3D}\nAnimation FPS: {self.target_fps}"
+    
+    
+    
+    def initialise_plotter(self) -> None:
+        """
+        Initalises the area where everythin will be drawn on. Call every time you want to draw a new model
+        """
+        
         if self.compute_3D:
             self.fig: plt.figure = plt.figure()
             self.ax: plt.Axes = self.fig.add_subplot(projection='3d')
             self.ax.view_init(None, 225)
           
         else:
             self.fig, self.ax = plt.subplots()
             
             #set aspect ratio to 1
             RATIO = 1.0
             x_left, x_right = self.ax.get_xlim()
             y_low, y_high = self.ax.get_ylim()
             self.ax.set_aspect(abs((x_right - x_left)/(y_low - y_high)) * RATIO)
-            
+    
+    
+    def add_grid(self):
+        """
+        Adds a grid
+        """
+        plt.grid()
+    
+    def add_legend(self):
+        """
+        Adds a legend
+        """
+        plt.legend()
+    
+    def lable_axes(self, x_lable: str = " x (AU)", y_lable: str = "y (AU)", z_lable: str = "z (AU)"):
+        """
+        Adds lables to axes. Call to override default axes' lables
+
+        Args:
+            x_lable (str, optional): x lable. Defaults to " x (AU)".
+            y_lable (str, optional): y lable. Defaults to "y (AU)".
+            z_lable (str, optional): z lable. Defaults to "z (AU)".
+        """
         
-    def __str__(self) -> str:
-        return f"Planets: {self.system.__str__()}\n3D: {self.compute_3D}\nAnimation FPS: {self.target_fps}"
+        self.ax.set_xlabel(x_lable)
+        self.ax.set_ylabel(y_lable)
+        if self.compute_3D:
+            self.ax.set_zlabel(z_lable)
+    
+    def show_plot(self):
+        """
+        Show drawn figure (calls plt.show())
+        """
+        plt.show()
+    
+    def save_figure(self, filename: str) -> None:
+        """_summary_
+
+        Args:
+            filename (str): _description_
+        """
+        
+
+        if not os.path.exists("figures"):
+            os.mkdir("figures")
+        
+        plt.savefig(f"figures/{filename}", dpi=250)
         
-           
+          
     def plot_orbit(self, orbit_data: Dict[str, List[float]]) -> None:
         """
         Plots the orbit of a planet
 
         Args:
             orbit_data Dict: {name: planet name, 
                     c: colour,
@@ -95,14 +145,15 @@
         """
         
         if "z" in orbit_data.keys(): # if self.compute_3D
             
             self.ax.plot(orbit_data["x"], orbit_data["y"], orbit_data["z"], label=f"{orbit_data['name']}'s orbit", c=orbit_data["c"])
         else:
             self.ax.plot(orbit_data["x"], orbit_data["y"], label=f"{orbit_data['name']}'s orbit", c=orbit_data["c"])
+    
             
     def plot_planet(self, planet_data: Dict[str, float]) -> None:
         """
         Plots a planet on self.ax
         
         Args:
             planet_data Dict: {name: planet name, 
@@ -114,14 +165,15 @@
         """
         if "z" in planet_data.keys(): # if self.compute_3D
             
             self.ax.scatter(planet_data["x"], planet_data["y"], planet_data["z"], label=planet_data["name"], s=25, c=planet_data["c"])
         else:
             # Draw 2D
             self.ax.scatter(planet_data["x"], planet_data["y"], label=planet_data["name"], s=25, c=planet_data["c"])
+   
              
     def plot_centre(self, name: str, colour: str) -> None:
         """
         Draw the centre of the model, can be a sun or a planet when using heliocentric model
 
         Args:
             name (str): Legend label
@@ -130,41 +182,49 @@
 
         if self.compute_3D:
             self.ax.scatter(0, 0, 0, s=100, label=name, c=colour)
             
         else:
             self.ax.scatter(0, 0, s=100, label=name, c=colour)
       
-    def show_orbits(self, show_plot: bool = True, save_figure: bool = False) -> None:
+
+    
+    def third_law(self):
+        """
+        Proves Kepler's third law
         """
-        Show the orbits of the selected planets
         
-        Args:
-            show_plot (bool, optional): Show the final figure (plt.show()). Defaults to True.
-            save_figure (bool, optional): Save the final figure to an image (The image will be saved in /figures). Defaults to False.
+        
+        x = [planet.a**3 for planet in  self.system.planets.values()]
+        y = [planet.P**2 for planet in  self.system.planets.values()]
+        
+
+        plt.scatter(x, y, c="#4F81BD", marker="D", label="Kepler's third law")
+        plt.plot(x, y, c="r", label="Linear (Kepler's third law)")
+
+
+        plt.title("Kepler's third law")
+        self.lable_axes(x_lable="a (AU)", y_lable="P (Yr)")
+        
+        
+        
+    def system_orbits(self) -> None:
+        """
+        Plot the orbits of the selected planets
         """
         self.plot_centre(name="Sun", colour="y")
         
         for planet_orbit_data in self.orbit_data:
             self.plot_orbit(orbit_data=planet_orbit_data)  
         
         plt.title("Planet orbits")
-        self.ax.set_xlabel('x (AU)')
-        self.ax.set_ylabel('y (AU)')
-        if self.compute_3D:
-            self.ax.set_zlabel('z (AU)')
-            
-        plt.legend()
-        plt.grid()
+        self.lable_axes()
         
-        if save_figure: 
-            utils.save_figure(name=f"{self.system.system_name}'s orbit")
+            
         
-        if show_plot:
-            plt.show()
             
     def animate_orbits(self) -> None:
         """
         Animate the orbits of the selected planets
         """
         
         while self.t < self.tmax:
@@ -176,34 +236,26 @@
             planet_data = [planet.compute_position(compute_3D=self.compute_3D, t=self.t) for planet in self.chosen_planets]
             for planet_planet_data in planet_data:
                 self.plot_planet(planet_data=planet_planet_data)
 
             self.t += self.dt
             
             plt.title("Planet orbits")
-            self.ax.set_xlabel('x (AU)')
-            self.ax.set_ylabel('y (AU)')
-            
-            if self.compute_3D:
-                self.ax.set_zlabel('z (AU)')
+            self.lable_axes()
             
             plt.legend()
             plt.grid()
             
             plt.pause(1/self.target_fps)
             plt.cla()
     
-    def spinograph(self, show_plot: bool = True, save_figure: bool = False) -> None:
+    
+    def spinograph(self) -> None:
         """
         Draw a spinograph with the chosen planets        
-
-        Args:
-            show_plot (bool, optional): Show the final figure (plt.show()). Defaults to True.           
-            save_figure (bool, optional): Save the final figure to an image (The image will be saved in /figures). Defaults to False.
-            
         """
         
         self.tmax *= 10
         self.dt = self.tmax / 1234
         
         
         while self.t < self.tmax:
@@ -222,36 +274,22 @@
             self.t += self.dt
         
         for planet_orbit_data in self.orbit_data:
             self.plot_orbit(orbit_data=planet_orbit_data)
         
         
         plt.title(f"{self.system.system_name}'s spinograph")
-        self.ax.set_xlabel('x (AU)')
-        self.ax.set_ylabel('y (AU)')
-        
-        if self.compute_3D:
-                self.ax.set_zlabel('z (AU)')
+        self.lable_axes()
         
-        if save_figure:
-            utils.save_figure(name=f"{self.system.system_name}'s spinograph")
         
-        if show_plot:   
-            plt.show()
-        
-    def animate_spinograph(self, save_figure: bool = False) -> None:
+    def animate_spinograph(self) -> None:
         """
-        Animate the drawing of a spinograph with the chosen planets        
-
-        Args:  
-            save_figure (bool, optional): Save the final figure to an image (The image will be saved in /figures). Defaults to False.
-            
+        Animate the drawing of a spinograph with the chosen planets            
         """
         
-        
         self.tmax *= 10
         self.dt = self.tmax / 1234
         
         
         while self.t < self.tmax:
             planet_data = [planet.compute_position(compute_3D=self.compute_3D, t=self.t) for planet in self.chosen_planets]
             
@@ -269,31 +307,23 @@
             for planet_orbit_data in self.orbit_data:
                 self.plot_orbit(orbit_data=planet_orbit_data)
         
             
             plt.pause(1/self.target_fps)
         
         plt.title(f"{self.system.system_name}'s spinograph")
-        self.ax.set_xlabel('x (AU)')
-        self.ax.set_ylabel('y (AU)')
+        self.lable_axes()
         
-        if self.compute_3D:
-            self.ax.set_zlabel('z (AU)')
-        
-        if save_figure:
-            utils.save_figure(name=f"{self.system.system_name}'s spinograph")
-            
-    def heliocentric_model(self, origin_planet_name: str, show_plot: bool = True, save_figure: bool = False) -> None:
+              
+    def heliocentric_model(self, origin_planet_name: str) -> None:
         """
         Compute the heliocentric using origin_planet_name as centre
 
         Args:
-            origin_planet_name (str): Name of centre planet (from planets in self.system.planets).\n
-            show_plot (bool, optional): Show the final figure (plt.show()). Defaults to True.\n
-            save_figure (bool, optional): Save the final figure to an image (The image will be saved in /figures). Defaults to False.
+            origin_planet_name (str): Name of centre planet (from planets in self.system.planets).
         """
         
         num_points = 3000
         
         self.tmax *= 20
         self.dt = self.tmax / num_points
         
@@ -335,22 +365,11 @@
                 self.ax.plot(planet_x, planet_y, label=planet.name, c=planet.colour)
             
 
         self.plot_centre(name=origin_planet_name, colour=origin_planet_data["c"])
 
         
         plt.title(f"{origin_planet_name}'s heliocentric model")
-        self.ax.set_xlabel('x (AU)')
-        self.ax.set_ylabel('y (AU)')
-        
-        if self.compute_3D:
-            self.ax.set_zlabel('z (AU)')
-        
-        plt.legend()
-        
-        if save_figure: 
-            utils.save_figure(name=f"{origin_planet_name}'s heliocentric model")
+        self.lable_axes()
         
-        if show_plot:
-            plt.show()
                     
-       
+
```

### Comparing `solarkit-0.0.1/solarkit.egg-info/PKG-INFO` & `solarkit-0.1/solarkit.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: solarkit
-Version: 0.0.1
+Version: 0.1
 Summary: Visualise a solar system and do cool stuff with it
 Author: Carlos Lorenzo
 Author-email: <clorenzozuniga@gmail.com>
 Keywords: solar system,space,astrophysics,bpho
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -17,19 +17,25 @@
 
 # solarkit - BPhO Computational challenge
 ## A tool to easily visualise and perform calculation on a solar system. The solutions for all challenges are embed but also provides the tools to tinker around and build new, original simulations
 
 It was built as the first part of a two part subimission for the challenge. My idea is to create a website using django to allow anyone to use the simulation. Having this package will ensure clean, backend code that will do the work in just a couple of lines.
 
 ### Challenges
+* Kepler's Third Law
 * Visualise a solar system
 * Visualise the solar system, animated
 * Spinograph
 * Heliocentric model
 
 ### Personal aditions
 * Tools to create, save & load a custom solar system
 * Save the model output to an image
 * Spinograph, animated
 
 ### How to use
-1. pip install solarkit
+1. pip install solarkit
+2. create .py file
+3. start experimenting! (follow example image for guidance)
+
+### Use example
+![solarkit_example](https://user-images.githubusercontent.com/91377173/236692357-7e14751b-2e94-4a01-894f-2202fef1e30d.jpg)
```

