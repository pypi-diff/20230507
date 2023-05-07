# Comparing `tmp/pyglplot-0.1.0.tar.gz` & `tmp/pyglplot-0.1.1.tar.gz`

## Comparing `pyglplot-0.1.0.tar` & `pyglplot-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pyglplot-0.1.0/.gitattributes
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pyglplot-0.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 pyglplot-0.1.0/mkdocs.yml
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 pyglplot-0.1.0/examples/example-min.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyglplot-0.1.0/pyglplot/__init__.py
--rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 pyglplot-0.1.0/pyglplot/line.py
--rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 pyglplot-0.1.0/pyglplot/roll.py
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 pyglplot-0.1.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pyglplot-0.1.0/LICENSE
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 pyglplot-0.1.0/README.md
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 pyglplot-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 pyglplot-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pyglplot-0.1.1/.gitattributes
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pyglplot-0.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 pyglplot-0.1.1/mkdocs.yml
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 pyglplot-0.1.1/examples/example-min.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyglplot-0.1.1/pyglplot/__init__.py
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 pyglplot-0.1.1/pyglplot/line.py
+-rw-r--r--   0        0        0     6510 2020-02-02 00:00:00.000000 pyglplot-0.1.1/pyglplot/roll.py
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 pyglplot-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pyglplot-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 pyglplot-0.1.1/README.md
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 pyglplot-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 pyglplot-0.1.1/PKG-INFO
```

### Comparing `pyglplot-0.1.0/.readthedocs.yaml` & `pyglplot-0.1.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pyglplot-0.1.0/mkdocs.yml` & `pyglplot-0.1.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyglplot-0.1.0/examples/example-min.ipynb` & `pyglplot-0.1.1/examples/example-min.ipynb`

 * *Files identical despite different names*

### Comparing `pyglplot-0.1.0/pyglplot/line.py` & `pyglplot-0.1.1/pyglplot/line.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,14 +108,21 @@
 
         gl.glUseProgram(self.program)
 
         gl.glClearColor(0.1, 0.1, 0.1, 1.0)
 
         self.updateColor(255, 255, 0)
 
+        glfw.set_window_size_callback(self.window, self.on_resize)
+
+    
+    def on_resize(self, window, width, height):
+        gl.glViewport(0, 0, width, height)
+
+
 
     def updateColor(self, r, g, b):
         self.color_buffer[:] = r
         self.color_buffer[1::3] = g
         self.color_buffer[2::3] = b
 
         gl.glBindBuffer(gl.GL_ARRAY_BUFFER, self.cbo)
```

### Comparing `pyglplot-0.1.0/pyglplot/roll.py` & `pyglplot-0.1.1/pyglplot/roll.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 import glfw
 from OpenGL import GL as gl
 import numpy as np
 
 class Roll():
     
-    def __init__(self, rollBufferSize = 100):
+    def __init__(self, rollBufferSize = 100, numLines = 1):
 
         self.rollBufferSize = rollBufferSize
+        self.numLines = numLines
 
         vertex_shader_text = """
         # version 330
         layout(location = 1) in vec2 a_position;
-        uniform float uShift;
-        uniform vec4 uColor;
+        layout(location = 2) in vec3 a_color;
 
+        uniform float uShift;
 
+        out vec3 vColor;
             
         void main(void) {
             vec2 shiftedPosition = a_position - vec2(uShift, 0);
             gl_Position = vec4(shiftedPosition, 0, 1);
 
+            vColor = a_color / vec3(255.0, 255.0, 255.0);
+
         }
         """
 
         fragment_shader_text = """
         # version 330
         precision mediump float;  
+        in vec3 vColor;
+        out vec4 outColor;
+        
         void main()
         {
-            gl_FragColor = vec4(1.0, 1.0, 0.0, 1.0);
+            gl_FragColor = vec4(vColor, 0.8);
         }
         """
 
 
-        self.vertex_buffer = np.zeros( (self.rollBufferSize + 2) * 2, dtype=np.uint32)
+        self.vertex_buffer = np.zeros( (self.rollBufferSize + 2) * 2 * self.numLines, dtype=np.uint32)
+        self.color_buffer = np.ones( (self.rollBufferSize + 2) * 3 * self.numLines, dtype=np.uint8) * 255
 
         if not glfw.init():
             exit()
         # Create a windowed mode window and its OpenGL context
         glfw.window_hint(glfw.CONTEXT_VERSION_MAJOR, 1)
         glfw.window_hint(glfw.CONTEXT_VERSION_MINOR, 5)
 
@@ -76,18 +84,31 @@
             print(gl.glGetShaderInfoLog(fragment_shader))
         
         self.program = gl.glCreateProgram()
         gl.glAttachShader(self.program, vertex_shader)
         gl.glAttachShader(self.program, fragment_shader)
         gl.glLinkProgram(self.program)
 
+        
+        
+        self.cbo = gl.glGenBuffers(1)
+
+        gl.glBindBuffer(gl.GL_ARRAY_BUFFER, self.cbo)
+        gl.glBufferData(gl.GL_ARRAY_BUFFER, self.color_buffer.nbytes, self.color_buffer, gl.GL_STATIC_DRAW)
+
+        self.colorLocation = gl.glGetAttribLocation(self.program, "a_color")
+        gl.glVertexAttribPointer(self.colorLocation, 3, gl.GL_UNSIGNED_BYTE, gl.GL_FALSE, 0, None)
+        gl.glEnableVertexAttribArray(self.colorLocation)
+
+
+
         self.vbo = gl.glGenBuffers(1)
 
         gl.glBindBuffer(gl.GL_ARRAY_BUFFER, self.vbo)
-        gl.glBufferData(gl.GL_ARRAY_BUFFER, self.vertex_buffer.nbytes, self.vertex_buffer, gl.GL_STATIC_DRAW)
+        gl.glBufferData(gl.GL_ARRAY_BUFFER, self.vertex_buffer.nbytes, self.vertex_buffer, gl.GL_DYNAMIC_DRAW)
 
         self.positionLocation = gl.glGetAttribLocation(self.program, "a_position")
         gl.glVertexAttribPointer(self.positionLocation, 2, gl.GL_FLOAT, gl.GL_FALSE, 0, None)
         gl.glEnableVertexAttribArray(self.positionLocation)
 
         self.uShiftLocation = gl.glGetUniformLocation(self.program, "uShift")
 
@@ -95,54 +116,75 @@
 
         gl.glClearColor(0.1, 0.1, 0.1, 1.0)
 
         self.shift = 0
         self.dataX = 1
         self.dataIndex = 0
 
-        self.lastDataX = 0
-        self.lastDataY = 0
+        self.lastDataX = np.zeros(numLines)
+        self.lastDataY = np.zeros(numLines)
 
+        glfw.set_window_size_callback(self.window, self.resize)
+
+    
+    def resize(self, window, width, height):
+        gl.glViewport(0, 0, width, height)
 
 
     def addPoint(self, y):
         bfSize = self.rollBufferSize + 2
 
         self.shift += 2 / self.rollBufferSize
         self.dataX += 2 / self.rollBufferSize
 
         gl.glUniform1f(self.uShiftLocation, self.shift)
         gl.glBindBuffer(gl.GL_ARRAY_BUFFER, self.vbo)
 
-        gl.glBufferSubData(gl.GL_ARRAY_BUFFER, self.dataIndex *2 *4, np.array([self.dataX, y], dtype=np.float32))
+        for i in range(self.numLines):
+            gl.glBufferSubData(gl.GL_ARRAY_BUFFER, (self.dataIndex + bfSize*i) *2 *4, np.array([self.dataX, y[i]], dtype=np.float32))
 
         if self.dataIndex == self.rollBufferSize - 1:
-            self.lastDataX = self.dataX
-            self.lastDataY = y
-
-        if self.dataIndex == 0 and self.lastDataX != 0:
-            gl.glBufferSubData(gl.GL_ARRAY_BUFFER, self.rollBufferSize * 2 * 4, np.array([self.lastDataX, self.lastDataY, self.dataX, y], dtype=np.float32))
-
+            for i in range(self.numLines):
+                self.lastDataX[i] = self.dataX
+                self.lastDataY[i] = y[i]
+
+        if self.dataIndex == 0 and self.lastDataX[0] != 0:
+            for i in range(self.numLines):
+                gl.glBufferSubData(gl.GL_ARRAY_BUFFER, (self.rollBufferSize + bfSize*i) * 2 * 4, np.array([self.lastDataX[i], self.lastDataY[i], self.dataX, y[i]], dtype=np.float32))
 
         gl.glEnableVertexAttribArray(self.positionLocation)
 
+        
         self.dataIndex = (self.dataIndex + 1) % self.rollBufferSize
+
+    def setLineColor(self, color, line):
+        gl.glUseProgram(self.program)
+        gl.glBindBuffer(gl.GL_ARRAY_BUFFER, self.cbo)
+
+        for i in range(self.rollBufferSize + 2):
+            gl.glBufferSubData(gl.GL_ARRAY_BUFFER, (self.rollBufferSize + 2)*line*3 + i*3, np.array(color, dtype=np.uint8))
+
+        gl.glEnableVertexAttribArray(self.colorLocation)
+
     
 
 
     def run(self, updateFunc):
         while not glfw.window_should_close(self.window):
             # Render here, e.g. using pyOpenGL
             gl.glClear(gl.GL_COLOR_BUFFER_BIT)
 
             updateFunc()
 
-            gl.glDrawArrays(gl.GL_LINE_STRIP, 0, self.dataIndex)
-            gl.glDrawArrays(gl.GL_LINE_STRIP, self.dataIndex, self.rollBufferSize - self.dataIndex)
-            gl.glDrawArrays(gl.GL_LINE_STRIP, self.rollBufferSize, 2)
+            bfsize = self.rollBufferSize + 2
+
+            for i in range(self.numLines):
+                gl.glDrawArrays(gl.GL_LINE_STRIP, i*bfsize, self.dataIndex)
+                gl.glDrawArrays(gl.GL_LINE_STRIP, i*bfsize + self.dataIndex, self.rollBufferSize - self.dataIndex)
+                gl.glDrawArrays(gl.GL_LINE_STRIP, i*bfsize + self.rollBufferSize, 2)
 
             # Swap front and back buffers
             glfw.swap_buffers(self.window)
 
             # Poll for and process events
             glfw.poll_events()
```

### Comparing `pyglplot-0.1.0/.gitignore` & `pyglplot-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyglplot-0.1.0/LICENSE` & `pyglplot-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglplot-0.1.0/README.md` & `pyglplot-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyglplot-0.1.0/pyproject.toml` & `pyglplot-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyglplot"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Danial Chitnis", email="d.chitnis@ed.ac.uk" },
 ]
 description = "A Python package for plotting."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyglplot-0.1.0/PKG-INFO` & `pyglplot-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglplot
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for plotting.
 Project-URL: Homepage, https://github.com/danchitnis/pyglplot
 Project-URL: Bug Tracker, https://github.com/danchitnis/pyglplot/issues
 Author-email: Danial Chitnis <d.chitnis@ed.ac.uk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

