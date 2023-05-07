# Comparing `tmp/image-to-arduino-1.0.3.7.tar.gz` & `tmp/image-to-arduino-1.0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image-to-arduino-1.0.3.7.tar", last modified: Sun May  7 10:46:30 2023, max compression
+gzip compressed data, was "image-to-arduino-1.0.3.9.tar", last modified: Sun May  7 12:33:05 2023, max compression
```

## Comparing `image-to-arduino-1.0.3.7.tar` & `image-to-arduino-1.0.3.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 10:46:30.483131 image-to-arduino-1.0.3.7/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-04-21 14:35:32.000000 image-to-arduino-1.0.3.7/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 10:45:25.000000 image-to-arduino-1.0.3.7/MANIFEST.in
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-07 10:46:30.483131 image-to-arduino-1.0.3.7/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2842 2023-04-23 17:53:08.000000 image-to-arduino-1.0.3.7/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 10:46:30.483131 image-to-arduino-1.0.3.7/image_to_arduino.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-07 10:46:30.000000 image-to-arduino-1.0.3.7/image_to_arduino.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      337 2023-05-07 10:46:30.000000 image-to-arduino-1.0.3.7/image_to_arduino.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-07 10:46:30.000000 image-to-arduino-1.0.3.7/image_to_arduino.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       60 2023-05-07 10:46:30.000000 image-to-arduino-1.0.3.7/image_to_arduino.egg-info/entry_points.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-05-07 10:46:30.000000 image-to-arduino-1.0.3.7/image_to_arduino.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        4 2023-05-07 10:46:30.000000 image-to-arduino-1.0.3.7/image_to_arduino.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       77 2023-04-22 13:23:37.000000 image-to-arduino-1.0.3.7/requirements.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-07 10:46:30.483131 image-to-arduino-1.0.3.7/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1466 2023-05-07 10:43:26.000000 image-to-arduino-1.0.3.7/setup.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 10:46:30.483131 image-to-arduino-1.0.3.7/src/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 14:35:32.000000 image-to-arduino-1.0.3.7/src/__init__.py
--rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)     7724 2023-04-23 17:50:58.000000 image-to-arduino-1.0.3.7/src/image-to-arduino.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 12:33:05.576532 image-to-arduino-1.0.3.9/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-04-21 14:35:32.000000 image-to-arduino-1.0.3.9/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 10:45:25.000000 image-to-arduino-1.0.3.9/MANIFEST.in
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-07 12:33:05.576532 image-to-arduino-1.0.3.9/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2842 2023-04-23 17:53:08.000000 image-to-arduino-1.0.3.9/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 12:33:05.576532 image-to-arduino-1.0.3.9/image_to_arduino.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-07 12:33:05.000000 image-to-arduino-1.0.3.9/image_to_arduino.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      351 2023-05-07 12:33:05.000000 image-to-arduino-1.0.3.9/image_to_arduino.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-07 12:33:05.000000 image-to-arduino-1.0.3.9/image_to_arduino.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       59 2023-05-07 12:33:05.000000 image-to-arduino-1.0.3.9/image_to_arduino.egg-info/entry_points.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-05-07 12:33:05.000000 image-to-arduino-1.0.3.9/image_to_arduino.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        4 2023-05-07 12:33:05.000000 image-to-arduino-1.0.3.9/image_to_arduino.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       77 2023-04-22 13:23:37.000000 image-to-arduino-1.0.3.9/requirements.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-07 12:33:05.576532 image-to-arduino-1.0.3.9/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1154 2023-05-07 12:32:40.000000 image-to-arduino-1.0.3.9/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 12:33:05.576532 image-to-arduino-1.0.3.9/src/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 14:35:32.000000 image-to-arduino-1.0.3.9/src/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       71 2023-05-07 12:29:24.000000 image-to-arduino-1.0.3.9/src/__main__.py
+-rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)     8329 2023-05-07 12:28:36.000000 image-to-arduino-1.0.3.9/src/imagetoarduino.py
```

### Comparing `image-to-arduino-1.0.3.7/LICENSE` & `image-to-arduino-1.0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `image-to-arduino-1.0.3.7/README.md` & `image-to-arduino-1.0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `image-to-arduino-1.0.3.7/setup.py` & `image-to-arduino-1.0.3.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,43 +8,29 @@
 # Join the path to the requirements.txt file relative to the setup.py file
 req_file = os.path.join(here, 'requirements.txt')
 
 # Read the requirements.txt file and split into a list of lines
 with open(req_file, 'r') as f:
     REQUIREMENTS = [line.strip() for line in f.readlines()]
 LONG_DESCRIPTION = 'About Image converter GUI App to arduino oled display ssd1306 128x64'
-class MyCommand(Command):
-    description = 'Runs myscript.py'
-    user_options = []
 
-    def initialize_options(self):
-        pass
-
-    def finalize_options(self):
-        pass
-
-    def run(self):
-        os.system('python3 image-to-arduino.py')
 setup(
    name='image-to-arduino',
-   version='1.0.3.7',
+   version='1.0.3.9',
    description='Image converter to arduino',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/Image_Converter_App.git",
    long_description_content_type="text/markdown",
    long_description=LONG_DESCRIPTION,
    packages=['src'],
    package_data={'src': ['data/*.dat']},
    install_requires=REQUIREMENTS, 
-   entry_points={
+    entry_points={
         'console_scripts': [
-            'mycommand = mypackage.mycommand:MyCommand'
+            'imagetoarduino = src.imagetoarduino:main'
         ]
     },
-   cmdclass={
-        'mycommand': MyCommand
-    }
 
 )
```

### Comparing `image-to-arduino-1.0.3.7/src/image-to-arduino.py` & `image-to-arduino-1.0.3.9/src/imagetoarduino.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,193 +5,193 @@
 import cv2
 import numpy as np
 from PIL import Image, ImageTk, ImageOps
 import os
 
 # To check extenxion
 import imghdr
-
 file_path = ''
 image_tk = ''
 left_switch_state = False
 right_switch_state = False
+def main():
 
-def open_file():
-    global file_path
-    file_path = filedialog.askopenfilename()
-    if file_path:
-        # If file name len is greater than 15: return ... + extension
-        file_label.configure(text="File: " + (os.path.basename(file_path) if len(os.path.basename(file_path)) < 15 else "..." + imghdr.what(file_path)))
-    else:
-        file_label.configure(text="No file selected")
-
-def generate_text():
-    global image_tk, switch_var
-    if not file_path == '':    
-        try:
-            # To check extenxion
-            extension = imghdr.what(file_path)
-
-            if  extension == "jpeg" or extension == "png":
-                # Load image
-                image = cv2.imread(file_path, cv2.IMREAD_COLOR)
-                
-                # Resize the image to 128x64
-                image = cv2.resize(image, (128, 64))
+    def open_file():
+        global file_path
+        file_path = filedialog.askopenfilename()
+        if file_path:
+            # If file name len is greater than 15: return ... + extension
+            file_label.configure(text="File: " + (os.path.basename(file_path) if len(os.path.basename(file_path)) < 15 else "..." + imghdr.what(file_path)))
+        else:
+            file_label.configure(text="No file selected")
+
+    def generate_text():
+        global image_tk, switch_var
+        if not file_path == '':    
+            try:
+                # To check extenxion
+                extension = imghdr.what(file_path)
+
+                if  extension == "jpeg" or extension == "png":
+                    # Load image
+                    image = cv2.imread(file_path, cv2.IMREAD_COLOR)
+                    
+                    # Resize the image to 128x64
+                    image = cv2.resize(image, (128, 64))
+                    
+                    # Convert RGB image to grayscale
+                    grayscale_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
+                    
+                    # Convert the image to a PIL Image object
+                    image_pre = Image.fromarray(cv2.threshold(grayscale_image, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)[1])
+
+                    if left_switch_state == True:
+                        # Reverse the colors of the image
+                        image_pre = ImageOps.invert(image_pre)
+                    
+                    # Convert the PIL Image to a PhotoImage object
+                    image_pre = ImageTk.PhotoImage(image_pre)
+                    
+                    # Update the label's image
+                    image_preview_label.config(image=image_pre)
+                    image_preview_label.image = image_pre
                 
-                # Convert RGB image to grayscale
-                grayscale_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
-                
-                # Convert the image to a PIL Image object
-                image_pre = Image.fromarray(cv2.threshold(grayscale_image, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)[1])
-
-                if left_switch_state == True:
-                    # Reverse the colors of the image
-                    image_pre = ImageOps.invert(image_pre)
-                
-                # Convert the PIL Image to a PhotoImage object
-                image_pre = ImageTk.PhotoImage(image_pre)
-                
-                # Update the label's image
-                image_preview_label.config(image=image_pre)
-                image_preview_label.image = image_pre
-            
-                _, thresholded_image = cv2.threshold(grayscale_image, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)
+                    _, thresholded_image = cv2.threshold(grayscale_image, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)
 
-                if left_switch_state == True:
-                    # Convert the thresholded image to a binary array (0s and 1s)
-                    binary_array = np.where(thresholded_image > 0, 0, 1)
-                else:
-                    # Convert the thresholded image to a binary array (0s and 1s)
-                    binary_array = np.where(thresholded_image > 0, 1, 0)
-
-            # Convert the binary array to a 1D array
-            one_d_array = binary_array.flatten()
-
-            # Split the binary alpha values into 8-byte arrays
-            byte_arrays = np.packbits(one_d_array)
-
-            # Convert byte arrays to hexadecimal format
-            hex_byte_arrays = ['0x' + format(byte, '02x') for byte in byte_arrays]
-
-            cpp_array = ', '.join(hex_byte_arrays)
-            # Insert newline after every 10 hexadecimal numbers
-            cpp_array = [cpp_array[i:i+2] for i in range(0, len(cpp_array), 2)]  # Split into pairs of hexadecimal numbers
-            cpp_array = [''.join(cpp_array[i:i+30]) for i in range(0, len(cpp_array), 30)]  # Join pairs with space, and group every 10 pairs
-            cpp_array = '\n'.join(cpp_array)  # Join groups with newline character
-
-            if right_switch_state == False:
-                # Generate C++ array
-                cpp_array = 'const unsigned char PROGMEM ' + os.path.splitext(os.path.basename(file_path))[0] + ' [] = {\n' + cpp_array + '\n};' 
-            elif right_switch_state == True:
-                # Generate full code ready to use 
-                cpp_array = '''#include <Adafruit_SSD1306.h>
-#include <Adafruit_GFX.h>
-#define OLED_RESET 4
-Adafruit_SSD1306 display(OLED_RESET);
-const unsigned char PROGMEM ''' + os.path.splitext(os.path.basename(file_path))[0] + '''[] = {''' +  cpp_array + ''' };
-void setup() 
-{
-    display.begin(SSD1306_SWITCHCAPVCC, 0x3C);
-    display.display();
-    delay(2000);
-    display.clearDisplay();}
-void loop() 
-{
-    display.drawBitmap(0, 0, ''' + os.path.splitext(os.path.basename(file_path))[0] + ''', 128, 64, 1); 
-    display.display();
-    delay(5000);
-    display.clearDisplay();
-    delay(5000);}'''        
+                    if left_switch_state == True:
+                        # Convert the thresholded image to a binary array (0s and 1s)
+                        binary_array = np.where(thresholded_image > 0, 0, 1)
+                    else:
+                        # Convert the thresholded image to a binary array (0s and 1s)
+                        binary_array = np.where(thresholded_image > 0, 1, 0)
+
+                # Convert the binary array to a 1D array
+                one_d_array = binary_array.flatten()
+
+                # Split the binary alpha values into 8-byte arrays
+                byte_arrays = np.packbits(one_d_array)
+
+                # Convert byte arrays to hexadecimal format
+                hex_byte_arrays = ['0x' + format(byte, '02x') for byte in byte_arrays]
+
+                cpp_array = ', '.join(hex_byte_arrays)
+                # Insert newline after every 10 hexadecimal numbers
+                cpp_array = [cpp_array[i:i+2] for i in range(0, len(cpp_array), 2)]  # Split into pairs of hexadecimal numbers
+                cpp_array = [''.join(cpp_array[i:i+30]) for i in range(0, len(cpp_array), 30)]  # Join pairs with space, and group every 10 pairs
+                cpp_array = '\n'.join(cpp_array)  # Join groups with newline character
+
+                if right_switch_state == False:
+                    # Generate C++ array
+                    cpp_array = 'const unsigned char PROGMEM ' + os.path.splitext(os.path.basename(file_path))[0] + ' [] = {\n' + cpp_array + '\n};' 
+                elif right_switch_state == True:
+                    # Generate full code ready to use 
+                    cpp_array = '''#include <Adafruit_SSD1306.h>
+    #include <Adafruit_GFX.h>
+    #define OLED_RESET 4
+    Adafruit_SSD1306 display(OLED_RESET);
+    const unsigned char PROGMEM ''' + os.path.splitext(os.path.basename(file_path))[0] + '''[] = {''' +  cpp_array + ''' };
+    void setup() 
+    {
+        display.begin(SSD1306_SWITCHCAPVCC, 0x3C);
+        display.display();
+        delay(2000);
+        display.clearDisplay();}
+    void loop() 
+    {
+        display.drawBitmap(0, 0, ''' + os.path.splitext(os.path.basename(file_path))[0] + ''', 128, 64, 1); 
+        display.display();
+        delay(5000);
+        display.clearDisplay();
+        delay(5000);}'''        
 
+                output_text.delete(1.0, tk.END)
+                output_text.insert(tk.END, cpp_array)
+            
+            # In case of error or invalid extension 
+            except:
+                output_text.delete(1.0, tk.END)
+                output_text.insert(tk.END, "Error generating text")
+        else: 
             output_text.delete(1.0, tk.END)
-            output_text.insert(tk.END, cpp_array)
-        
-        # In case of error or invalid extension 
-        except:
-            output_text.delete(1.0, tk.END)
-            output_text.insert(tk.END, "Error generating text")
-    else: 
-        output_text.delete(1.0, tk.END)
-        output_text.insert(tk.END, "Select any file")
-
-def copy_all():
-    global file_path
-    if not file_path:
-        copied_all_label.configure(text="No text to copy")
-        return
+            output_text.insert(tk.END, "Select any file")
 
-    root.clipboard_clear()
-    root.clipboard_append(output_text.get(1.0, tk.END))
-    copied_all_label.configure(text="✓ Copied")
+    def copy_all():
+        global file_path
+        if not file_path:
+            copied_all_label.configure(text="No text to copy")
+            return
+
+        root.clipboard_clear()
+        root.clipboard_append(output_text.get(1.0, tk.END))
+        copied_all_label.configure(text="✓ Copied")
+
+    def toggle_left_switch():
+        global left_switch_state
+        left_switch_state = not left_switch_state
+
+    def toggle_right_switch():
+        global right_switch_state
+        right_switch_state = not right_switch_state
 
-def toggle_left_switch():
-    global left_switch_state
-    left_switch_state = not left_switch_state
-
-def toggle_right_switch():
-    global right_switch_state
-    right_switch_state = not right_switch_state
-
-def clear_all():
-    # Clear output text and image preview
-    output_text.delete(1.0, tk.END)
-    image_preview_label.config(image="")
+    def clear_all():
+        # Clear output text and image preview
+        output_text.delete(1.0, tk.END)
+        image_preview_label.config(image="")
 
-customtkinter.set_appearance_mode("dark")  
-customtkinter.set_default_color_theme("dark-blue")  
+    customtkinter.set_appearance_mode("dark")  
+    customtkinter.set_default_color_theme("dark-blue")  
 
-# Create customtkinter window
-root = customtkinter.CTk() 
-root.title("Image to arduino")
+    # Create customtkinter window
+    root = customtkinter.CTk() 
+    root.title("Image to arduino")
 
-# Set window size
-root.geometry("330x550") # Set width and height as desired
+    # Set window size
+    root.geometry("330x550") # Set width and height as desired
 
-# Label for displaying selected file path
-file_label =  customtkinter.CTkLabel(root, text="No file selected")
-file_label.grid(row=0, column=0, padx=10, columnspan=1, sticky="nsew", pady=5)
+    # Label for displaying selected file path
+    file_label =  customtkinter.CTkLabel(root, text="No file selected")
+    file_label.grid(row=0, column=0, padx=10, columnspan=1, sticky="nsew", pady=5)
 
-# "Open File" button
-open_file_button = customtkinter.CTkButton(root, text="Open Image File", command=open_file)
-open_file_button.grid(row=0, column=1, padx=10, pady=5, columnspan=1, sticky="nsew")
+    # "Open File" button
+    open_file_button = customtkinter.CTkButton(root, text="Open Image File", command=open_file)
+    open_file_button.grid(row=0, column=1, padx=10, pady=5, columnspan=1, sticky="nsew")
 
-# "Generate" button
-generate_button = customtkinter.CTkButton(root, text="Generate Code", command=generate_text)
-generate_button.grid(row=2, column=0, padx=10, pady=5, columnspan=1, sticky="nsew")
+    # "Generate" button
+    generate_button = customtkinter.CTkButton(root, text="Generate Code", command=generate_text)
+    generate_button.grid(row=2, column=0, padx=10, pady=5, columnspan=1, sticky="nsew")
 
-# "Copy All" button
-copy_all_button = customtkinter.CTkButton(root, text="Copy All", command=copy_all)
-copy_all_button.grid(row=2, column=1, padx=10, pady=5, columnspan=1, sticky="nsew")  
+    # "Copy All" button
+    copy_all_button = customtkinter.CTkButton(root, text="Copy All", command=copy_all)
+    copy_all_button.grid(row=2, column=1, padx=10, pady=5, columnspan=1, sticky="nsew")  
 
-# Output text 
-output_text = customtkinter.CTkTextbox(root, height = 280, width = 300 )   # 25 50
-output_text.grid(row=3, column=0, padx=10, pady=5, columnspan=3, sticky="nsew")
+    # Output text 
+    output_text = customtkinter.CTkTextbox(root, height = 280, width = 300 )   # 25 50
+    output_text.grid(row=3, column=0, padx=10, pady=5, columnspan=3, sticky="nsew")
 
-# Label for displaying "Copied All" text
-copied_all_label =  customtkinter.CTkLabel(root, text="")
-copied_all_label.grid(row=4, column=1, pady=5,columnspan=3, sticky="nsew")
+    # Label for displaying "Copied All" text
+    copied_all_label =  customtkinter.CTkLabel(root, text="")
+    copied_all_label.grid(row=4, column=1, pady=5,columnspan=3, sticky="nsew")
 
-# Preview text lael
-preview_text_label = customtkinter.CTkLabel(root, text="Preview")
-preview_text_label.grid(row=5, column=0, pady=5, padx=10)
+    # Preview text lael
+    preview_text_label = customtkinter.CTkLabel(root, text="Preview")
+    preview_text_label.grid(row=5, column=0, pady=5, padx=10)
 
-# Label to display the image
-image_preview_label = tk.Label(root, bg="#1b1a1b")
-image_preview_label.grid(row=6, column=0, columnspan=1, padx=10)
+    # Label to display the image
+    image_preview_label = tk.Label(root, bg="#1b1a1b")
+    image_preview_label.grid(row=6, column=0, columnspan=1, padx=10)
 
-# Switch label left
-switch = customtkinter.CTkSwitch(root, text="Reverse colors", command=toggle_left_switch)
-switch.grid(row=1, column=0, padx=10, sticky="nsew")
+    # Switch label left
+    switch = customtkinter.CTkSwitch(root, text="Reverse colors", command=toggle_left_switch)
+    switch.grid(row=1, column=0, padx=10, sticky="nsew")
 
-# Switch label right 
-switch_right = customtkinter.CTkSwitch(root, text="Full arduino code", command=toggle_right_switch)
-switch_right.grid(row=1, column=1, padx=10, sticky="nsew")
+    # Switch label right 
+    switch_right = customtkinter.CTkSwitch(root, text="Full arduino code", command=toggle_right_switch)
+    switch_right.grid(row=1, column=1, padx=10, sticky="nsew")
 
-# "Clear all" button 
-clear_all_button = customtkinter.CTkButton(root, text="Clear All", command=clear_all)
-clear_all_button.grid(row=4, column=0, pady=5, padx=10, columnspan=1, sticky="nsew")  
+    # "Clear all" button 
+    clear_all_button = customtkinter.CTkButton(root, text="Clear All", command=clear_all)
+    clear_all_button.grid(row=4, column=0, pady=5, padx=10, columnspan=1, sticky="nsew")  
 
-# Configure the window to not be resizable
-root.resizable(False, False)
+    # Configure the window to not be resizable
+    root.resizable(False, False)
 
-root.mainloop()
+    root.mainloop()
```

