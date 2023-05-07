# Comparing `tmp/PDFVisor-0.1.4.tar.gz` & `tmp/PDFVisor-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PDFVisor-0.1.4.tar", last modified: Sat May  6 16:22:37 2023, max compression
+gzip compressed data, was "PDFVisor-0.1.5.tar", last modified: Sun May  7 14:41:57 2023, max compression
```

## Comparing `PDFVisor-0.1.4.tar` & `PDFVisor-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 16:22:37.855533 PDFVisor-0.1.4/
--rw-rw-rw-   0        0        0      888 2023-03-30 11:59:20.000000 PDFVisor-0.1.4/LICENSE.rst
--rw-rw-rw-   0        0        0       60 2023-05-06 16:14:37.000000 PDFVisor-0.1.4/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-06 16:22:37.767145 PDFVisor-0.1.4/PDFVisor.egg-info/
--rw-rw-rw-   0        0        0     1478 2023-05-06 16:22:37.000000 PDFVisor-0.1.4/PDFVisor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-05-06 16:22:37.000000 PDFVisor-0.1.4/PDFVisor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 16:22:37.000000 PDFVisor-0.1.4/PDFVisor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-06 16:22:37.000000 PDFVisor-0.1.4/PDFVisor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-06 16:22:37.000000 PDFVisor-0.1.4/PDFVisor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1478 2023-05-06 16:22:37.847530 PDFVisor-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1171 2023-03-29 11:56:40.000000 PDFVisor-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-06 16:22:37.855533 PDFVisor-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1779 2023-05-06 16:21:38.000000 PDFVisor-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 16:22:37.791147 PDFVisor-0.1.4/src/
--rw-rw-rw-   0        0        0     9817 2023-05-06 14:10:16.000000 PDFVisor-0.1.4/src/PDFViewr.py
--rw-rw-rw-   0        0        0        0 2023-04-07 17:56:52.000000 PDFVisor-0.1.4/src/__init__.py
--rw-rw-rw-   0        0        0     4113 2023-04-14 20:56:10.000000 PDFVisor-0.1.4/src/funcsVisorPDF.py
-drwxrwxrwx   0        0        0        0 2023-05-06 16:22:37.839519 PDFVisor-0.1.4/src/img/
--rw-rw-rw-   0        0        0     5315 2023-04-21 15:35:44.000000 PDFVisor-0.1.4/src/img/avanceDeshabilitado.png
--rw-rw-rw-   0        0        0     4991 2023-04-21 14:52:58.000000 PDFVisor-0.1.4/src/img/avanceHighlight.png
--rw-rw-rw-   0        0        0     4385 2023-04-21 15:23:16.000000 PDFVisor-0.1.4/src/img/avanceHighlightPressed.png
--rw-rw-rw-   0        0        0     5250 2023-04-20 10:47:56.000000 PDFVisor-0.1.4/src/img/avanceNormal.png
--rw-rw-rw-   0        0        0     5231 2023-04-21 15:37:12.000000 PDFVisor-0.1.4/src/img/retroDeshabilitado.png
--rw-rw-rw-   0        0        0     4836 2023-04-21 15:27:38.000000 PDFVisor-0.1.4/src/img/retroHighlight.png
--rw-rw-rw-   0        0        0     4305 2023-04-21 15:24:26.000000 PDFVisor-0.1.4/src/img/retroHighlightPressed.png
--rw-rw-rw-   0        0        0     5947 2023-04-20 17:09:38.000000 PDFVisor-0.1.4/src/img/retroNormal.png
--rw-rw-rw-   0        0        0  1206884 2022-05-07 05:19:20.000000 PDFVisor-0.1.4/src/times.ttf
+drwxrwxrwx   0        0        0        0 2023-05-07 14:41:57.526229 PDFVisor-0.1.5/
+-rw-rw-rw-   0        0        0      888 2023-03-30 11:59:20.000000 PDFVisor-0.1.5/LICENSE.rst
+-rw-rw-rw-   0        0        0       60 2023-05-06 16:14:37.000000 PDFVisor-0.1.5/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-07 14:41:57.432003 PDFVisor-0.1.5/PDFVisor.egg-info/
+-rw-rw-rw-   0        0        0     1478 2023-05-07 14:41:57.000000 PDFVisor-0.1.5/PDFVisor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-05-07 14:41:57.000000 PDFVisor-0.1.5/PDFVisor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 14:41:57.000000 PDFVisor-0.1.5/PDFVisor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-07 14:41:57.000000 PDFVisor-0.1.5/PDFVisor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-07 14:41:57.000000 PDFVisor-0.1.5/PDFVisor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1478 2023-05-07 14:41:57.526229 PDFVisor-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1171 2023-03-29 11:56:40.000000 PDFVisor-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-07 14:41:57.526229 PDFVisor-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1779 2023-05-07 14:39:47.000000 PDFVisor-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:41:57.447631 PDFVisor-0.1.5/src/
+-rw-rw-rw-   0        0        0     9499 2023-05-07 14:36:37.000000 PDFVisor-0.1.5/src/PDFViewr.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 17:56:52.000000 PDFVisor-0.1.5/src/__init__.py
+-rw-rw-rw-   0        0        0     4371 2023-05-07 14:09:48.000000 PDFVisor-0.1.5/src/funcsVisorPDF.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:41:57.510581 PDFVisor-0.1.5/src/img/
+-rw-rw-rw-   0        0        0     5315 2023-04-21 15:35:44.000000 PDFVisor-0.1.5/src/img/avanceDeshabilitado.png
+-rw-rw-rw-   0        0        0     4991 2023-04-21 14:52:58.000000 PDFVisor-0.1.5/src/img/avanceHighlight.png
+-rw-rw-rw-   0        0        0     4385 2023-04-21 15:23:16.000000 PDFVisor-0.1.5/src/img/avanceHighlightPressed.png
+-rw-rw-rw-   0        0        0     5250 2023-04-20 10:47:56.000000 PDFVisor-0.1.5/src/img/avanceNormal.png
+-rw-rw-rw-   0        0        0     5231 2023-04-21 15:37:12.000000 PDFVisor-0.1.5/src/img/retroDeshabilitado.png
+-rw-rw-rw-   0        0        0     4836 2023-04-21 15:27:38.000000 PDFVisor-0.1.5/src/img/retroHighlight.png
+-rw-rw-rw-   0        0        0     4305 2023-04-21 15:24:26.000000 PDFVisor-0.1.5/src/img/retroHighlightPressed.png
+-rw-rw-rw-   0        0        0     5947 2023-04-20 17:09:38.000000 PDFVisor-0.1.5/src/img/retroNormal.png
+-rw-rw-rw-   0        0        0  1206884 2022-05-07 05:19:20.000000 PDFVisor-0.1.5/src/times.ttf
```

### Comparing `PDFVisor-0.1.4/LICENSE.rst` & `PDFVisor-0.1.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `PDFVisor-0.1.4/PDFVisor.egg-info/PKG-INFO` & `PDFVisor-0.1.5/PDFVisor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PDFVisor
-Version: 0.1.4
+Version: 0.1.5
 Summary: Recurso para moverse por documentos PDF
 Author: Antonio San Román
 Author-email: asanro46@gmail.com
 License: MIT
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
```

### Comparing `PDFVisor-0.1.4/PKG-INFO` & `PDFVisor-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PDFVisor
-Version: 0.1.4
+Version: 0.1.5
 Summary: Recurso para moverse por documentos PDF
 Author: Antonio San Román
 Author-email: asanro46@gmail.com
 License: MIT
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
```

### Comparing `PDFVisor-0.1.4/README.md` & `PDFVisor-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `PDFVisor-0.1.4/setup.py` & `PDFVisor-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
       "numpy",
       "PyMuPDF",
       "opencv-contrib-python",
       ] 
 
 setup(
     name= "PDFVisor",
-    version= '0.1.4',
+    version= '0.1.5',
     description= 'Recurso para moverse por documentos PDF',
     long_description=  (HERE / "README.md").read_text(encoding='utf-8'),
     long_description_content_type= "text/markdown",
     author= 'Antonio San Román',
     author_email= 'asanro46@gmail.com',
     install_requires=INSTALL_REQUIRES,
     license= 'MIT',
```

### Comparing `PDFVisor-0.1.4/src/PDFViewr.py` & `PDFVisor-0.1.5/src/PDFViewr.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,33 +2,26 @@
    import tkinter as tk
    from tkinter.messagebox import showerror, showinfo
    import tkinter as tk
    from tkinter import ttk
    from tkinter import*
    import cv2
    import numpy as np
-   from PIL import Image, ImageTk, ImageFont 
+   from PIL import Image, ImageTk 
    import PDFVisor.funcsVisorPDF as vPDF
 except Exception as e:
       print(f"This error occured while importing neccesary modules or library {e}")   
 
 nombre = ""
 lenguaje = ""
 bandaFrame = None
 marcovisor = None
 opcion = ""
 image_on_canvas = None
 
-def centraTexto(text, centroFrame):
-    centroFrame = int(centroFrame/2)
-    text = text[0:int(text.__len__()/2)]
-    fuente = ImageFont.truetype("times.ttf", 12)
-    size = int(fuente.getlength(text))
-    return (centroFrame - size) - 47
-
 
 class Visor(tk.Frame):
      def __init__(self, master=None):
          #tk.Toplevel.__init__(self, master)
          tk.Frame.__init__(self, master)
          global btnEstado
          global bandaFrame
@@ -56,39 +49,39 @@
 
          self.master.configure(height=675, width= 770, bg= "#1a5e92")
          #self.config(height=529, width= 330, bg= "#1a5e92")
          self.grid_rowconfigure(0, weight= 60)
          self.grid_rowconfigure(1, weight= 120)
          self.place()
          
-         bandaFrame = tk.Frame(self.master, bg="#2596be", anchor= "NW", height=80, width= 770)
+         bandaFrame = tk.Frame(self.master, bg="#2596be", height=80, width= 770)
          bandaFrame.grid(row= 0, column= 0, padx=2, sticky="nw")
          bandaFrame.grid_columnconfigure(0, weight=50)
          bandaFrame.grid_columnconfigure(1, weight=150)
          bandaFrame.grid_columnconfigure(2, weight=50)
          bandaFrame.place_configure(x=0, y=0)
 
          marcovisor = tk.LabelFrame(self.master, width= 770, height= 605, borderwidth= 2, bg= "#2596be", relief= "raised")
          marcovisor.grid(row=1, column=0, padx= 2, pady= 2, sticky="se")
          marcovisor.place_configure(x=0, y=80, bordermode="outside")
         
          btnEstado = vPDF.defEstado(self.master.getvar(name="PDFDOC"))
          archEstados = btnEstado["imagStates"]
          estados = btnEstado["Estado"]
-         self.imgAvance = ImageTk.PhotoImage(file= r"./img/avanceNormal.png")
+         self.imgAvance = ImageTk.PhotoImage(file= archEstados[0])
          btnAvance = ttk.Label(bandaFrame, image= self.imgAvance, state= estados[0], width= 106, border=0, background=None)
          btnAvance.config(style= "Emergency.TLabel")
          btnAvance.grid(row=0, column=0, ipadx=0, ipady=0)
          btnAvance.place()
 
          metaDataDoc = vPDF.metaDataPDF(self.master.getvar(name="PDFDOC"))
          rotulo = Canvas(bandaFrame, width=330, height=60, highlightthickness=0, bg="#2596be", bd=0, borderwidth= 0)
          rotulo.grid(row=0, column=1, ipady=0, ipadx=5)
          metadatosPDF = "{}\n{}".format(metaDataDoc.get("Titulo"), metaDataDoc.get("Fecha_creacion"))
-         x = centraTexto(metaDataDoc.get("Titulo"), bandaFrame.cget('width'))
+         x = vPDF.centraTexto(metaDataDoc.get("Titulo"), bandaFrame.cget('width'))
          lblInformacion = rotulo.create_text(x, 28, justify="center", text= metadatosPDF, fill="white", font= ("Times New Roman", 12, "bold"))
 
          btnEstado = vPDF.defEstado(self.master.getvar(name="PDFDOC"))
          archEstados = btnEstado["imagStates"]  #estados[1]
          estados = btnEstado["Estado"]
          self.imgRetro = ImageTk.PhotoImage(file= archEstados[1]) 
          btnRetro = ttk.Label(bandaFrame, image= self.imgRetro, state= "normal", width= 106)  
@@ -185,19 +178,19 @@
 
          if btnEstado[opcion] == 'normal':
              imgFlecha = ImageTk.PhotoImage(file= fileflecha)
              bandaFrame.children[parOpcion].__setattr__('image', imgFlecha)
          else:
              return 
 
-         pdfPag = "PARREL-ISEC(Feb 23)_Page-{}.jpg".format(opcion)
-         imgk = ImageTk.PhotoImage(file= r"D:/Temp/" + pdfPag)
-         image_on_canvas.__setattr__('image', imgk)
-         marcovisor.children['!canvas'].__setitem__('itemconfig', image_on_canvas)
-         #visorPDF.itemconfig(image_on_canvas, image= imgk)
+         nomFile = self.master.getvar(name="PDFDOC")
+         nomFile = nomFile[0:-4] + "_Page-{}.jpg".format(opcion)
+         imgk = Image.open(nomFile)
+         imgk = imgk.resize((752,577), Image.Resampling.LANCZOS)
+         marcovisor.children['!label'].__setattr__('image', imgk)
          
          
      def gestorEventos(self):    
          archEstados = btnEstado["imagStates"]
          
          bandaFrame.children['!label'].bind("<Enter>", lambda event: auto.on_enter('!label', 0, r"./img/avanceHighlight.png"))                    
          bandaFrame.children['!label2'].bind("<Enter>", lambda event: auto.on_enter('!label2', 1, r"./img/retroHighlight.png") )
```

### Comparing `PDFVisor-0.1.4/src/funcsVisorPDF.py` & `PDFVisor-0.1.5/src/funcsVisorPDF.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
 from PyPDF2 import PdfReader
-from PIL import Image, ImageColor, ImageTk
+from PIL import Image, ImageColor, ImageTk, ImageFont
 import fitz
 import cv2
 import numpy as np
 import os
 import pathlib
 
 global image_on_canvas
@@ -118,7 +118,14 @@
      outimage = cv2.add(foreground, background)
      return outimage
 
 def cargaPagPDF(archivo, indice):
    nomFilePag = archivo[:-4]
    nomFilePag = nomFilePag[8:] + "_Page-{}.jpg".format(indice)
    return ImageTk.PhotoImage(file= r"D:/Temp/" + nomFilePag)
+
+def centraTexto(text, centroFrame):
+    centroFrame = int(centroFrame/2)
+    text = text[0:int(text.__len__()/2)]
+    fuente = ImageFont.truetype("times.ttf", 12)
+    size = int(fuente.getlength(text))
+    return (centroFrame - size) - 47
```

### Comparing `PDFVisor-0.1.4/src/img/avanceDeshabilitado.png` & `PDFVisor-0.1.5/src/img/avanceDeshabilitado.png`

 * *Files identical despite different names*

### Comparing `PDFVisor-0.1.4/src/img/avanceHighlight.png` & `PDFVisor-0.1.5/src/img/avanceHighlight.png`

 * *Files identical despite different names*

### Comparing `PDFVisor-0.1.4/src/img/avanceHighlightPressed.png` & `PDFVisor-0.1.5/src/img/avanceHighlightPressed.png`

 * *Files identical despite different names*

### Comparing `PDFVisor-0.1.4/src/img/avanceNormal.png` & `PDFVisor-0.1.5/src/img/avanceNormal.png`

 * *Files identical despite different names*

### Comparing `PDFVisor-0.1.4/src/img/retroDeshabilitado.png` & `PDFVisor-0.1.5/src/img/retroDeshabilitado.png`

 * *Files identical despite different names*

### Comparing `PDFVisor-0.1.4/src/img/retroHighlight.png` & `PDFVisor-0.1.5/src/img/retroHighlight.png`

 * *Files identical despite different names*

### Comparing `PDFVisor-0.1.4/src/img/retroHighlightPressed.png` & `PDFVisor-0.1.5/src/img/retroHighlightPressed.png`

 * *Files identical despite different names*

### Comparing `PDFVisor-0.1.4/src/img/retroNormal.png` & `PDFVisor-0.1.5/src/img/retroNormal.png`

 * *Files identical despite different names*

### Comparing `PDFVisor-0.1.4/src/times.ttf` & `PDFVisor-0.1.5/src/times.ttf`

 * *Files identical despite different names*

