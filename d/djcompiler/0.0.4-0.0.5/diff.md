# Comparing `tmp/djcompiler-0.0.4.tar.gz` & `tmp/djcompiler-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djcompiler-0.0.4.tar", last modified: Fri Jan 20 14:22:19 2023, max compression
+gzip compressed data, was "djcompiler-0.0.5.tar", last modified: Sun May  7 14:53:22 2023, max compression
```

## Comparing `djcompiler-0.0.4.tar` & `djcompiler-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 abdoo     (1000) abdoo     (1000)        0 2023-01-20 14:22:19.920738 djcompiler-0.0.4/
--rw-rw-r--   0 abdoo     (1000) abdoo     (1000)     1519 2023-01-18 16:32:33.000000 djcompiler-0.0.4/LICENSE
--rw-rw-r--   0 abdoo     (1000) abdoo     (1000)      249 2023-01-20 13:45:00.000000 djcompiler-0.0.4/MANIFEST.in
--rw-rw-r--   0 abdoo     (1000) abdoo     (1000)     1718 2023-01-20 14:22:19.920738 djcompiler-0.0.4/PKG-INFO
--rw-rw-r--   0 abdoo     (1000) abdoo     (1000)      602 2023-01-20 13:49:41.000000 djcompiler-0.0.4/README.rst
-drwxrwxr-x   0 abdoo     (1000) abdoo     (1000)        0 2023-01-20 14:22:19.920738 djcompiler-0.0.4/djcompiler/
--rw-rw-r--   0 abdoo     (1000) abdoo     (1000)       81 2023-01-20 13:11:45.000000 djcompiler-0.0.4/djcompiler/__init__.py
--rw-rw-r--   0 abdoo     (1000) abdoo     (1000)      228 2023-01-19 12:20:22.000000 djcompiler-0.0.4/djcompiler/__main__.py
-drwxrwxr-x   0 abdoo     (1000) abdoo     (1000)        0 2023-01-20 14:22:19.920738 djcompiler-0.0.4/djcompiler/compiler/
--rw-rw-r--   0 abdoo     (1000) abdoo     (1000)        0 2023-01-18 16:25:29.000000 djcompiler-0.0.4/djcompiler/compiler/__init__.py
--rw-rw-r--   0 abdoo     (1000) abdoo     (1000)     6902 2023-01-19 17:39:02.000000 djcompiler-0.0.4/djcompiler/compiler/djcompiler.py
-drwxrwxr-x   0 abdoo     (1000) abdoo     (1000)        0 2023-01-20 14:22:19.920738 djcompiler-0.0.4/djcompiler/management/
--rw-rw-r--   0 abdoo     (1000) abdoo     (1000)     1584 2023-01-20 13:14:23.000000 djcompiler-0.0.4/djcompiler/management/__init__.py
-drwxrwxr-x   0 abdoo     (1000) abdoo     (1000)        0 2023-01-20 14:22:19.920738 djcompiler-0.0.4/djcompiler/management/command/
--rw-rw-r--   0 abdoo     (1000) abdoo     (1000)      151 2023-01-20 12:45:42.000000 djcompiler-0.0.4/djcompiler/management/command/__init__.py
--rw-rw-r--   0 abdoo     (1000) abdoo     (1000)      886 2023-01-20 13:00:48.000000 djcompiler-0.0.4/djcompiler/management/command/buildfile.py
--rw-rw-r--   0 abdoo     (1000) abdoo     (1000)     1090 2023-01-20 13:00:48.000000 djcompiler-0.0.4/djcompiler/management/command/buildpy.py
--rw-rw-r--   0 abdoo     (1000) abdoo     (1000)     1717 2023-01-20 13:00:48.000000 djcompiler-0.0.4/djcompiler/management/command/compile.py
-drwxrwxr-x   0 abdoo     (1000) abdoo     (1000)        0 2023-01-20 14:22:19.920738 djcompiler-0.0.4/djcompiler.egg-info/
--rw-rw-r--   0 abdoo     (1000) abdoo     (1000)     1718 2023-01-20 14:22:19.000000 djcompiler-0.0.4/djcompiler.egg-info/PKG-INFO
--rw-rw-r--   0 abdoo     (1000) abdoo     (1000)      616 2023-01-20 14:22:19.000000 djcompiler-0.0.4/djcompiler.egg-info/SOURCES.txt
--rw-rw-r--   0 abdoo     (1000) abdoo     (1000)        1 2023-01-20 14:22:19.000000 djcompiler-0.0.4/djcompiler.egg-info/dependency_links.txt
--rw-rw-r--   0 abdoo     (1000) abdoo     (1000)       79 2023-01-20 14:22:19.000000 djcompiler-0.0.4/djcompiler.egg-info/entry_points.txt
--rw-rw-r--   0 abdoo     (1000) abdoo     (1000)        1 2023-01-20 13:53:17.000000 djcompiler-0.0.4/djcompiler.egg-info/not-zip-safe
--rw-rw-r--   0 abdoo     (1000) abdoo     (1000)       16 2023-01-20 14:22:19.000000 djcompiler-0.0.4/djcompiler.egg-info/requires.txt
--rw-rw-r--   0 abdoo     (1000) abdoo     (1000)       29 2023-01-20 14:22:19.000000 djcompiler-0.0.4/djcompiler.egg-info/top_level.txt
--rw-rw-r--   0 abdoo     (1000) abdoo     (1000)      128 2023-01-19 15:33:10.000000 djcompiler-0.0.4/pyproject.toml
--rw-rw-r--   0 abdoo     (1000) abdoo     (1000)     1477 2023-01-20 14:22:19.920738 djcompiler-0.0.4/setup.cfg
--rw-rw-r--   0 abdoo     (1000) abdoo     (1000)     1442 2023-01-18 16:58:33.000000 djcompiler-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:53:22.693694 djcompiler-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-07 14:53:10.000000 djcompiler-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-07 14:53:10.000000 djcompiler-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-07 14:53:22.693694 djcompiler-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-07 14:53:10.000000 djcompiler-0.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:53:22.693694 djcompiler-0.0.5/djcompiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-07 14:53:10.000000 djcompiler-0.0.5/djcompiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-07 14:53:10.000000 djcompiler-0.0.5/djcompiler/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:53:22.693694 djcompiler-0.0.5/djcompiler/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 14:53:10.000000 djcompiler-0.0.5/djcompiler/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-05-07 14:53:10.000000 djcompiler-0.0.5/djcompiler/compiler/djcompiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:53:22.693694 djcompiler-0.0.5/djcompiler/management/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-07 14:53:10.000000 djcompiler-0.0.5/djcompiler/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:53:22.693694 djcompiler-0.0.5/djcompiler/management/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-07 14:53:10.000000 djcompiler-0.0.5/djcompiler/management/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-07 14:53:10.000000 djcompiler-0.0.5/djcompiler/management/command/buildfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-07 14:53:10.000000 djcompiler-0.0.5/djcompiler/management/command/buildpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-07 14:53:10.000000 djcompiler-0.0.5/djcompiler/management/command/compile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:53:22.693694 djcompiler-0.0.5/djcompiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-07 14:53:22.000000 djcompiler-0.0.5/djcompiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-07 14:53:22.000000 djcompiler-0.0.5/djcompiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 14:53:22.000000 djcompiler-0.0.5/djcompiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-07 14:53:22.000000 djcompiler-0.0.5/djcompiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 14:53:22.000000 djcompiler-0.0.5/djcompiler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-07 14:53:22.000000 djcompiler-0.0.5/djcompiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-07 14:53:22.000000 djcompiler-0.0.5/djcompiler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-07 14:53:10.000000 djcompiler-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-07 14:53:22.697695 djcompiler-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-07 14:53:10.000000 djcompiler-0.0.5/setup.py
```

### Comparing `djcompiler-0.0.4/LICENSE` & `djcompiler-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `djcompiler-0.0.4/PKG-INFO` & `djcompiler-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djcompiler
-Version: 0.0.4
+Version: 0.0.5
 Summary: django compiler that compiles django project to a C language using Cython project which gives more performance and more security since the original code is hidden.
 Home-page: https://github.com/abdoohossamm/djcompiler
 Author: Abdalrahman Hossam Eldin Mohamed
 Author-email: abdoohossamm@outlook.com
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/abdoohossamm/djcompiler
 Project-URL: Tracker, https://github.com/abdoohossamm/djcompiler/issues
@@ -46,7 +46,9 @@
 Usage
 -----
 * run ``djcompiler help`` to see available commands.
 * run ``djcompiler compile`` to compile the django project.
 * run ``djcompiler buildfile`` to generate a config file.
 * run ``djcompiler buildpy`` to generate a python script that compiles the project when run.
 
+Future Features
+===============
```

### Comparing `djcompiler-0.0.4/djcompiler/compiler/djcompiler.py` & `djcompiler-0.0.5/djcompiler/compiler/djcompiler.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,37 +23,42 @@
     ignored_files: list = []
     initial_ignored_dirs: list = ["venv/", "cython/", ".git/", ".idea/", "build/", "__pycache__/"]
 
     def __init__(self,
                  ignored_dirs: List[str] = None,
                  build_directory: str = "build",
                  other_files_needed: List[str] = None,
+                 other_dirs_needed: List[str] = None,
                  ignored_files: List[str] = None,
                  project_name: str = "",
                  project_author: str = "author",
                  project_version: str = "1.0.0",
                  c_dir: str = "",
                  ):
         """
         A class that compiles django project to C language.
         :param ignored_dirs: list[str] -> a list of directories to ignore while building for example the env variables.
         :param build_directory: path to the build output directory.
         :param other_files_needed: files to copy to the build directory like the env file or manage.py script.
+        :param other_dirs_needed: dirs to copy to the build directory like the static dir and media dir.
         :param c_dir: a path to the C files output.
         """
         if ignored_dirs is None:
             ignored_dirs = []
         if ignored_files is None:
             ignored_files = []
         if other_files_needed is None:
             other_files_needed = []
+        if other_dirs_needed is None:
+            other_dirs_needed = []
         self.ignored_dirs = ignored_dirs
         self.ignored_files = ignored_files
         self.build_directory = build_directory
         self.other_files_needed = other_files_needed
+        self.other_dirs_needed = other_dirs_needed
         self.project_name = project_name
         self.project_author = project_author
         self.project_version = project_version
         if len(sys.argv) < 2:
             sys.argv = ['setup.py', 'build_ext', '--build-lib', build_directory]
         if '--build-lib' in sys.argv:
             self.build_directory = sys.argv[sys.argv.index('--build-lib') + 1]
@@ -111,39 +116,62 @@
                 continue
             try:
                 shutil.rmtree(migration_path)
             except FileNotFoundError as e:
                 print(f"building migration file {migration_path}")
             shutil.copytree(f"{dir_path}", migration_path)
 
-    def inital_python_modules(self):
+    def copy_needed_dirs(self, dirs: list = None):
+        if dirs is None:
+            dirs = self.other_dirs_needed
+        print("#################### Copy Needed Dirs ####################")
+        for dir_path in dirs:
+            build_dir_path: str = f"./{self.build_directory}/{dir_path}"
+            if self.check_ignored_dirs(path_name=dir_path):
+                continue
+            try:
+                shutil.copytree(f"{dir_path}", build_dir_path, dirs_exist_ok=True)
+                print(f"Copy dir {dir_path} to build")
+            except FileNotFoundError as e:
+                print(f"Couldn't copy directory {dir_path} to build directory")
+
+    def python_modules_rules(self, path_name):
+        ignore_build_dir = path_name.endswith(f"/{self.build_directory}")
+        ignore_temp_dirs = f"./{self.build_directory}/temp." in f"{path_name}/"
+        for dir in self.other_dirs_needed:
+            ignore_other_needed_dirs = f"./{self.build_directory}/{dir}" in f"{path_name}/"
+            if ignore_build_dir or ignore_temp_dirs or ignore_other_needed_dirs:
+                return True
+        return False
+
+    def initial_python_modules(self):
+        print("#################### Initial Python Modules ####################")
         for path, subdirs, files in os.walk(f"./{self.build_directory}"):
-            if path.endswith(f"/{self.build_directory}") or f"./{self.build_directory}/temp." in path:
+            if self.python_modules_rules(path):
                 continue
             f = open(f"{path}/__init__.py", "w")
             f.close()
 
     def copy_needed_files(self, files: list = None):
         print("#################### Copy needed files ####################")
         if files is None:
             files = self.other_files_needed
         for file in files:
             try:
-                shutil.copy(file, f"./{self.build_directory}")
+                shutil.copy(file, f"./{self.build_directory}/{file}")
             except FileNotFoundError:
                 print(f"file {file} not found")
             except FileExistsError:
                 print(f"file {file} already copied")
 
-    def compile_project(self, ext_modules: Set[Extension] = None,
+    def compile_modules(self, ext_modules: Set[Extension] = None,
                         cython_dir: str = "cython",
-                        compiler_directives: dict = None
-                        ) -> None:
+                        compiler_directives: dict = None) -> None:
         """
-        A function that compiles the django project
+        A method that compile the python modules
         :param ext_modules: set[Extension]: not required -> files that should be compiled
         :param cython_dir: str -> the C files output dir.
         :param compiler_directives: dict -> extra compiler option [like the lanugae]
         :return: None
         """
         if ext_modules is None:
             ext_modules = self.ext_modules()
@@ -154,12 +182,31 @@
             name=self.project_name,
             version=self.project_version,
             author=self.project_author,
             cmdclass={'build_ext': Cython.Distutils.build_ext},
             ext_modules=cythonize(ext_modules, build_dir=cython_dir,
                                   compiler_directives=compiler_directives,
                                   ),
-
         )
+
+    def compile_project(self) -> None:
+        """
+        A method that compiles the django project
+        the method runs:
+            compile_modules()
+
+            copy_migrations_to_build()
+
+            initial_python_modules()
+
+            copy_needed_files()
+
+            copy_needed_dirs()
+
+        methods
+        :return: None
+        """
+        self.compile_modules()
         self.copy_migrations_to_build()
-        self.inital_python_modules()
+        self.initial_python_modules()
         self.copy_needed_files()
+        self.copy_needed_dirs()
```

### Comparing `djcompiler-0.0.4/djcompiler/management/__init__.py` & `djcompiler-0.0.5/djcompiler/management/__init__.py`

 * *Files identical despite different names*

### Comparing `djcompiler-0.0.4/djcompiler/management/command/buildfile.py` & `djcompiler-0.0.5/djcompiler/management/command/buildfile.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     compiler_config: str = """# Project details
 project_name=DjCompiler
 project_author=author
 project_version=1.0.0
 # Compiler data
 build_directory=build
 other_files_needed=manage.py .env __init__.py
+other_dirs_needed=static media
 ignored_files=manage.py compiler.py
 ignored_dirs=venv/ cython/ .git/ .idea/ build/ __pycache__/"""
 
     def write_compiler_settings(self):
         with open(".djcompiler", "w") as f:
             f.writelines(self.compiler_config)
```

### Comparing `djcompiler-0.0.4/djcompiler/management/command/buildpy.py` & `djcompiler-0.0.5/djcompiler/management/command/buildpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 if __name__ == "__main__":
     compiler: DjangoCompiler = DjangoCompiler(
         project_name="DjCompiler",
         project_author="author",
         project_version="1.0.0",
         build_directory="build",
         other_files_needed=["manage.py", ".env", "__init__.py"],
+        other_dirs_needed=["static"]
         ignored_files=["manage.py", "setup.py", "compiler.py"]
     )
     ignored = compiler.initial_ignored_dirs + ["django_compiler/"]
     compiler.set_ignored(ignored)
     compiler.compile_project()
     """
```

### Comparing `djcompiler-0.0.4/djcompiler/management/command/compile.py` & `djcompiler-0.0.5/djcompiler/management/command/compile.py`

 * *Files identical despite different names*

### Comparing `djcompiler-0.0.4/djcompiler.egg-info/PKG-INFO` & `djcompiler-0.0.5/djcompiler.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djcompiler
-Version: 0.0.4
+Version: 0.0.5
 Summary: django compiler that compiles django project to a C language using Cython project which gives more performance and more security since the original code is hidden.
 Home-page: https://github.com/abdoohossamm/djcompiler
 Author: Abdalrahman Hossam Eldin Mohamed
 Author-email: abdoohossamm@outlook.com
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/abdoohossamm/djcompiler
 Project-URL: Tracker, https://github.com/abdoohossamm/djcompiler/issues
@@ -46,7 +46,9 @@
 Usage
 -----
 * run ``djcompiler help`` to see available commands.
 * run ``djcompiler compile`` to compile the django project.
 * run ``djcompiler buildfile`` to generate a config file.
 * run ``djcompiler buildpy`` to generate a python script that compiles the project when run.
 
+Future Features
+===============
```

### Comparing `djcompiler-0.0.4/djcompiler.egg-info/SOURCES.txt` & `djcompiler-0.0.5/djcompiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djcompiler-0.0.4/setup.cfg` & `djcompiler-0.0.5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djcompiler
-version = 0.0.4
+version = 0.0.5
 url = https://github.com/abdoohossamm/djcompiler
 author = Abdalrahman Hossam Eldin Mohamed
 author_email = abdoohossamm@outlook.com
 description = django compiler that compiles django project to a C language using Cython project which gives more performance and more security since the original code is hidden.
 long_description = file: README.rst
 license = BSD-3-Clause
 classifiers = 
@@ -25,15 +25,15 @@
 
 [options]
 python_requires = >=3.8
 packages = find:
 include_package_data = True
 zip_safe = false
 install_requires = 
-	Cython >= 0.29.33
+	Cython >= 0.29.34
 exclude = tests,testproject
 
 [options.entry_points]
 console_scripts = 
 	djcompiler = djcompiler.management:execute_from_command_line
 
 [flake8]
```

### Comparing `djcompiler-0.0.4/setup.py` & `djcompiler-0.0.5/setup.py`

 * *Files identical despite different names*

