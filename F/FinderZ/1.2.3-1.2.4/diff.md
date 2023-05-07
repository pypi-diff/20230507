# Comparing `tmp/finderz-1.2.3.tar.gz` & `tmp/finderz-1.2.4.tar.gz`

## Comparing `finderz-1.2.3.tar` & `finderz-1.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-1.2.3/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-1.2.3/src/.DS_Store
--rw-r--r--   0        0        0     9581 2020-02-02 00:00:00.000000 finderz-1.2.3/src/FinderZ/FinderZLib.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 finderz-1.2.3/src/FinderZ/__init__.py
--rwxr-xr-x   0        0        0       31 2020-02-02 00:00:00.000000 finderz-1.2.3/tests/bash.sh
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 finderz-1.2.3/tests/importTests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finderz-1.2.3/tests/insertion.txt
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 finderz-1.2.3/tests/insertiontest.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 finderz-1.2.3/tests/parentFunctions.py
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 finderz-1.2.3/tests/updates/update.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 finderz-1.2.3/LICENSE
--rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 finderz-1.2.3/README.md
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 finderz-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     5225 2020-02-02 00:00:00.000000 finderz-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-1.2.4/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 finderz-1.2.4/src/.DS_Store
+-rw-r--r--   0        0        0     9713 2020-02-02 00:00:00.000000 finderz-1.2.4/src/FinderZ/FinderZLib.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 finderz-1.2.4/src/FinderZ/__init__.py
+-rwxr-xr-x   0        0        0       31 2020-02-02 00:00:00.000000 finderz-1.2.4/tests/bash.sh
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 finderz-1.2.4/tests/importTests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finderz-1.2.4/tests/insertion.txt
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 finderz-1.2.4/tests/insertiontest.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 finderz-1.2.4/tests/parentFunctions.py
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 finderz-1.2.4/tests/updates/update.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 finderz-1.2.4/LICENSE
+-rw-r--r--   0        0        0     4453 2020-02-02 00:00:00.000000 finderz-1.2.4/README.md
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 finderz-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 finderz-1.2.4/PKG-INFO
```

### Comparing `finderz-1.2.3/.DS_Store` & `finderz-1.2.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `finderz-1.2.3/src/.DS_Store` & `finderz-1.2.4/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `finderz-1.2.3/src/FinderZ/FinderZLib.py` & `finderz-1.2.4/src/FinderZ/FinderZLib.py`

 * *Files 4% similar despite different names*

```diff
@@ -231,91 +231,98 @@
 
 
 
 
 	#Version 1.2.3:
 	def insertTextInFile(insertionText, lineNumber, filePath, appendNewLines = False):
 			
-			if lineNumber < 1:
-				raise Exception("ERR: Line number can not be less than 1.")
-			#Open the file and start scanning:
-			fileObject = open(filePath, 'r')
-			
-			
-			#Read the lines, if it fails, then raise exception:
-			try:
-				fileLines = fileObject.readlines()
-				readable = True
-			except UnicodeDecodeError:
-				
-				raise Exception("ERR: The file seems to be un-decodable.")
+		if lineNumber < 1:
+			raise Exception("ERR: Line number can not be less than 1.")
+		#Open the file and start scanning:
+		fileObject = open(filePath, 'r')
+		
+		
+		#Read the lines, if it fails, then raise exception:
+		try:
+			fileLines = fileObject.readlines()
+			readable = True
+		except UnicodeDecodeError:
 			
-			#Check if the file has any content in the first place, and if it doesn't, append a value to avoid errors:
-			if fileLines == []:
-				fileLines.append("")
+			raise Exception("ERR: The file seems to be un-decodable.")
+		
+		#Check if the file has any content in the first place, and if it doesn't, append a value to avoid errors:
+		if fileLines == []:
+			fileLines.append("")
 
 
 
-			#Get the line amount:
-			lineamount = len(fileLines)
+		#Get the line amount:
+		lineamount = len(fileLines)
 
-			#Define the main line iterator, which starts at 1:
-			line = 1
+		#Define the main line iterator, which starts at 1:
+		line = 1
 
-			#For each line...
-			for i in range(lineamount):
+		#For each line...
+		for i in range(lineamount):
+			
+			#Check if the line is in the lineCount to see if the destination has been reached:
+			if int(line) == int(lineNumber):
+				#Set Check = True
+				Check = True
 				
-				#Check if the line is in the lineCount to see if the destination has been reached:
-				if int(line) == int(lineNumber):
-					#Set Check = True
-					Check = True
-					
-					
-					#Get the info in that line.
-					foundLine = fileLines[line-1]
-					
-					#Add on to the line contents.
-					
-					insertion = foundLine + insertionText
-					#Set the line equal to the insertion:
-					fileLines[line-1] = insertion.replace("\n", '', 1) + "\n"
-					
-					break
+				
+				#Get the info in that line.
+				foundLine = fileLines[line-1]
+				
+				#Add on to the line contents.
+				
+				insertion = foundLine + insertionText
+				#Set the line equal to the insertion:
+				fileLines[line-1] = insertion.replace("\n", '', 1) + "\n"
+				
+				break
 
-				elif int(line) == int(len(fileLines)) and appendNewLines == True:
-					
-					#Replace any initial "\n" in the initial contents (to avoid ghost indents)
-					fileLines[line-1] = fileLines[line-1].replace('\n', '', 1)
+			elif int(line) == int(len(fileLines)) and appendNewLines == True:
+				
+				#Replace any initial "\n" in the initial contents (to avoid ghost indents)
+				fileLines[line-1] = fileLines[line-1].replace('\n', '', 1)
 
-					#While the specified lineNumber is not reached yet, append a new line for each remaining line.
-					while int(line) != (lineNumber):
-						
-						fileLines.append('')
-						fileLines[line-1] = fileLines[line-1] + "\n"
-						
-						line += 1
+				#While the specified lineNumber is not reached yet, append a new line for each remaining line.
+				while int(line) != (lineNumber):
 					
-					insertion = fileLines[lineNumber-1] + insertionText
-					#Set the line equal to the insertion:
-					fileLines[lineNumber-1] = insertion.replace("\n", '', 1)
+					fileLines.append('')
+					fileLines[line-1] = fileLines[line-1] + "\n"
 					
-					Check = True
-				else:
-					#Set the check = False
-					Check = False
-				line += 1
-		#If the check is True, then write the lines to the file. Else, raise exception as no line was found.
-			if Check == True:
-				f = open(filePath, 'w')
+					line += 1
+				
+				insertion = fileLines[lineNumber-1] + insertionText
+				#Set the line equal to the insertion:
+				fileLines[lineNumber-1] = insertion.replace("\n", '', 1)
 				
-				f.writelines(fileLines)
-			#If the Check == False, then raise this exception:
+				Check = True
 			else:
-				raise Exception("ERR: No specified line number found in file.")
-
-		
+				#Set the check = False
+				Check = False
+			line += 1
+	#If the check is True, then write the lines to the file. Else, raise exception as no line was found.
+		if Check == True:
+			f = open(filePath, 'w')
+			
+			f.writelines(fileLines)
+		#If the Check == False, then raise this exception:
+		else:
+			raise Exception("ERR: No specified line number found in file.")
+	#VERSION: 1.2.4
+    #Create a single file:
+	def createFile(fileName, path):
+		os.chdir(path)
+		f = open(fileName, 'w')
+		f.close()
+	#Remove a single file:
+	def removeFile(filePath):
+		os.remove(filePath)
 #Class to call bash scripts (Gives even more flexibilty):
 class callBash:
 	def runFile(path):
 		os.system("chmod +x " + path)
 		subprocess.run([path], shell = True)
```

### Comparing `finderz-1.2.3/tests/parentFunctions.py` & `finderz-1.2.4/tests/parentFunctions.py`

 * *Files identical despite different names*

### Comparing `finderz-1.2.3/tests/updates/update.py` & `finderz-1.2.4/tests/updates/update.py`

 * *Files identical despite different names*

### Comparing `finderz-1.2.3/LICENSE` & `finderz-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `finderz-1.2.3/README.md` & `finderz-1.2.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,35 +6,43 @@
 <p align="center">
 	<img src="https://img.shields.io/badge/License-GPL--3.0-brightgreen"
 		height="23">
 	<img src="https://img.shields.io/badge/Creator-PatzEdi-brightgreen"
 		height="23">
 	<img src="https://img.shields.io/badge/Version-Latest-brightgreen"
 		height="23">
+	
+	
 </p>
 <p align = "center">
 	<img src="https://static.pepy.tech/badge/finderz"
 		height="23">
 </p>
-This script uses the os and subprocess libraries in order to function properly. 
+FinderZ uses the os, subprocess, and shutil libraries in order to function properly. 
 
 ## **Written in python, this library provides you with different file operation commands as well as info gathering commands on directories as well as files.** 
 ____________________________________________________________________________
-## **CHANGELOG: 1.2.3**
-- Release version 1.2.3
-- Added new function: insertTextInFile
-- With this new function, you can insert text in any line of a file. 
+## **CHANGELOG: 1.2.4**
+- Release version 1.2.4
+- Added new functions: createFile and removeFile
+- With these new functions, you can easily create and remove singular files.
+- Fixed some README issues.
 
-In order to add text at a specific line in a file, do so like this:
+If you want to create a single file, you can do so like this:
 
 ```
-fileOperands.insertTextInFile("insertionText", lineNumber, "/path/to/file/", appendNewLines = False) #Where append new lines creates new lines if you want to put text in a line that is bigger than the current line amount of the file.
+from FinderZ import fileOperands
+
+fileOperands.createFile("FileName", "fileCreationPath")
 ```
+Note that the "FileName" in this case may also include a file extension.
+
+- Documentation will be added soon that explains each function and functionality of each function in a detailed manner.
 
-- New documentation will be added soon that explains each function and functionality of each function in a detailed manner.
+Thank you all for 10K Downloads!
 
 ## **Usage**
 Installation:
 ```
 pip3 install FinderZ
 ```
 Importing:
@@ -77,8 +85,8 @@
 ## **Services used (Credits):**
 - [OS module](https://docs.python.org/3/library/os.html)
 - [Shutil module](https://docs.python.org/3/library/shutil.html)
 - [Subprocess module](https://docs.python.org/3/library/subprocess.html)
 
 ____________________________________________________________________________
 ## **Make sure to leave a star!**
-- If you like this project, leaving a star is what motivates me in doing more. Thank you, and I hope this is useful to all.
+- If you like this project, leaving a star is what motivates me in doing more. Thank you, and I hope this is useful to all.
```

### Comparing `finderz-1.2.3/pyproject.toml` & `finderz-1.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "FinderZ"
-version = "1.2.3"
+version = "1.2.4"
 authors = [
 	{ name="PatzEdi", email="patzedigithub@gmail.com" },
 ]
 description = "A library that extends file management functionality in Python with many useful features in order to save your time and make life easier!"
 readme = "README.md"
 license = "GPL-3.0-or-later"
 keywords = ["files", "filemanagement", "library", "development"]
```

### Comparing `finderz-1.2.3/PKG-INFO` & `finderz-1.2.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinderZ
-Version: 1.2.3
+Version: 1.2.4
 Summary: A library that extends file management functionality in Python with many useful features in order to save your time and make life easier!
 Project-URL: Homepage, https://github.com/PatzEdi
 Project-URL: Repository, https://github.com/PatzEdi/FinderZ
 Project-URL: Bug Tracker, https://github.com/PatzEdi/FinderZ/issues
 Author-email: PatzEdi <patzedigithub@gmail.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
@@ -23,35 +23,43 @@
 <p align="center">
 	<img src="https://img.shields.io/badge/License-GPL--3.0-brightgreen"
 		height="23">
 	<img src="https://img.shields.io/badge/Creator-PatzEdi-brightgreen"
 		height="23">
 	<img src="https://img.shields.io/badge/Version-Latest-brightgreen"
 		height="23">
+	
+	
 </p>
 <p align = "center">
 	<img src="https://static.pepy.tech/badge/finderz"
 		height="23">
 </p>
-This script uses the os and subprocess libraries in order to function properly. 
+FinderZ uses the os, subprocess, and shutil libraries in order to function properly. 
 
 ## **Written in python, this library provides you with different file operation commands as well as info gathering commands on directories as well as files.** 
 ____________________________________________________________________________
-## **CHANGELOG: 1.2.3**
-- Release version 1.2.3
-- Added new function: insertTextInFile
-- With this new function, you can insert text in any line of a file. 
+## **CHANGELOG: 1.2.4**
+- Release version 1.2.4
+- Added new functions: createFile and removeFile
+- With these new functions, you can easily create and remove singular files.
+- Fixed some README issues.
 
-In order to add text at a specific line in a file, do so like this:
+If you want to create a single file, you can do so like this:
 
 ```
-fileOperands.insertTextInFile("insertionText", lineNumber, "/path/to/file/", appendNewLines = False) #Where append new lines creates new lines if you want to put text in a line that is bigger than the current line amount of the file.
+from FinderZ import fileOperands
+
+fileOperands.createFile("FileName", "fileCreationPath")
 ```
+Note that the "FileName" in this case may also include a file extension.
+
+- Documentation will be added soon that explains each function and functionality of each function in a detailed manner.
 
-- New documentation will be added soon that explains each function and functionality of each function in a detailed manner.
+Thank you all for 10K Downloads!
 
 ## **Usage**
 Installation:
 ```
 pip3 install FinderZ
 ```
 Importing:
@@ -94,8 +102,8 @@
 ## **Services used (Credits):**
 - [OS module](https://docs.python.org/3/library/os.html)
 - [Shutil module](https://docs.python.org/3/library/shutil.html)
 - [Subprocess module](https://docs.python.org/3/library/subprocess.html)
 
 ____________________________________________________________________________
 ## **Make sure to leave a star!**
-- If you like this project, leaving a star is what motivates me in doing more. Thank you, and I hope this is useful to all.
+- If you like this project, leaving a star is what motivates me in doing more. Thank you, and I hope this is useful to all.
```

