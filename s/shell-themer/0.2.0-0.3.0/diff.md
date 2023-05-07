# Comparing `tmp/shell-themer-0.2.0.tar.gz` & `tmp/shell-themer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell-themer-0.2.0.tar", last modified: Wed Apr 19 17:49:48 2023, max compression
+gzip compressed data, was "shell-themer-0.3.0.tar", last modified: Sun May  7 19:48:43 2023, max compression
```

## Comparing `shell-themer-0.2.0.tar` & `shell-themer-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-19 17:49:48.167468 shell-themer-0.2.0/
--rw-r--r--   0 jared      (501) staff       (20)      430 2023-03-24 22:19:37.000000 shell-themer-0.2.0/.gitignore
--rw-r--r--   0 jared      (501) staff       (20)      724 2023-04-19 17:43:58.000000 shell-themer-0.2.0/CHANGELOG.md
--rw-r--r--   0 jared      (501) staff       (20)     5359 2023-04-19 17:43:58.000000 shell-themer-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 jared      (501) staff       (20)     1062 2023-03-15 00:19:15.000000 shell-themer-0.2.0/LICENSE
--rw-r--r--   0 jared      (501) staff       (20)     3596 2023-04-19 17:49:48.167323 shell-themer-0.2.0/PKG-INFO
--rw-r--r--   0 jared      (501) staff       (20)     1352 2023-04-07 23:49:41.000000 shell-themer-0.2.0/README.md
--rw-r--r--   0 jared      (501) staff       (20)     2085 2023-04-15 04:34:30.000000 shell-themer-0.2.0/TODO.md
--rw-r--r--   0 jared      (501) staff       (20)     2635 2023-04-15 03:22:17.000000 shell-themer-0.2.0/pyproject.toml
--rw-r--r--   0 jared      (501) staff       (20)       38 2023-04-19 17:49:48.167505 shell-themer-0.2.0/setup.cfg
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-19 17:49:48.163814 shell-themer-0.2.0/src/
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-19 17:49:48.165464 shell-themer-0.2.0/src/shell_themer/
--rw-r--r--   0 jared      (501) staff       (20)     1228 2023-04-14 15:39:07.000000 shell-themer-0.2.0/src/shell_themer/__init__.py
--rw-r--r--   0 jared      (501) staff       (20)     1350 2023-04-15 23:38:46.000000 shell-themer-0.2.0/src/shell_themer/__main__.py
--rwxr-xr-x   0 jared      (501) staff       (20)    37599 2023-04-15 22:11:33.000000 shell-themer-0.2.0/src/shell_themer/themer.py
--rw-r--r--   0 jared      (501) staff       (20)     1608 2023-04-15 03:09:24.000000 shell-themer-0.2.0/src/shell_themer/version.py
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-19 17:49:48.166157 shell-themer-0.2.0/src/shell_themer.egg-info/
--rw-r--r--   0 jared      (501) staff       (20)     3596 2023-04-19 17:49:48.000000 shell-themer-0.2.0/src/shell_themer.egg-info/PKG-INFO
--rw-r--r--   0 jared      (501) staff       (20)      595 2023-04-19 17:49:48.000000 shell-themer-0.2.0/src/shell_themer.egg-info/SOURCES.txt
--rw-r--r--   0 jared      (501) staff       (20)        1 2023-04-19 17:49:48.000000 shell-themer-0.2.0/src/shell_themer.egg-info/dependency_links.txt
--rw-r--r--   0 jared      (501) staff       (20)       65 2023-04-19 17:49:48.000000 shell-themer-0.2.0/src/shell_themer.egg-info/entry_points.txt
--rw-r--r--   0 jared      (501) staff       (20)      168 2023-04-19 17:49:48.000000 shell-themer-0.2.0/src/shell_themer.egg-info/requires.txt
--rw-r--r--   0 jared      (501) staff       (20)       13 2023-04-19 17:49:48.000000 shell-themer-0.2.0/src/shell_themer.egg-info/top_level.txt
--rw-r--r--   0 jared      (501) staff       (20)     4196 2023-04-19 17:49:33.000000 shell-themer-0.2.0/tasks.py
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-19 17:49:48.166991 shell-themer-0.2.0/tests/
--rw-r--r--   0 jared      (501) staff       (20)     2512 2023-04-15 21:59:15.000000 shell-themer-0.2.0/tests/conftest.py
--rw-r--r--   0 jared      (501) staff       (20)    19596 2023-04-13 23:30:40.000000 shell-themer-0.2.0/tests/test_generate.py
--rw-r--r--   0 jared      (501) staff       (20)     2150 2023-04-11 14:03:52.000000 shell-themer-0.2.0/tests/test_list.py
--rw-r--r--   0 jared      (501) staff       (20)     7093 2023-04-15 23:38:46.000000 shell-themer-0.2.0/tests/test_main_dispatch.py
--rw-r--r--   0 jared      (501) staff       (20)     2318 2023-04-11 15:55:44.000000 shell-themer-0.2.0/tests/test_preview.py
--rw-r--r--   0 jared      (501) staff       (20)    14331 2023-04-15 20:24:06.000000 shell-themer-0.2.0/tests/test_themer.py
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-19 17:49:48.167112 shell-themer-0.2.0/themes/
--rw-r--r--   0 jared      (501) staff       (20)     9310 2023-04-13 23:29:31.000000 shell-themer-0.2.0/themes/dracula.toml
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-05-07 19:48:43.366783 shell-themer-0.3.0/
+-rw-r--r--   0 jared      (501) staff       (20)      430 2023-03-24 22:19:37.000000 shell-themer-0.3.0/.gitignore
+-rw-r--r--   0 jared      (501) staff       (20)      817 2023-05-07 19:46:38.000000 shell-themer-0.3.0/CHANGELOG.md
+-rw-r--r--   0 jared      (501) staff       (20)     5359 2023-04-19 17:43:58.000000 shell-themer-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 jared      (501) staff       (20)     1062 2023-03-15 00:19:15.000000 shell-themer-0.3.0/LICENSE
+-rw-r--r--   0 jared      (501) staff       (20)     3596 2023-05-07 19:48:43.366623 shell-themer-0.3.0/PKG-INFO
+-rw-r--r--   0 jared      (501) staff       (20)     1352 2023-04-07 23:49:41.000000 shell-themer-0.3.0/README.md
+-rw-r--r--   0 jared      (501) staff       (20)     2376 2023-05-07 19:46:38.000000 shell-themer-0.3.0/TODO.md
+-rw-r--r--   0 jared      (501) staff       (20)     2635 2023-04-15 03:22:17.000000 shell-themer-0.3.0/pyproject.toml
+-rw-r--r--   0 jared      (501) staff       (20)       38 2023-05-07 19:48:43.366824 shell-themer-0.3.0/setup.cfg
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-05-07 19:48:43.363113 shell-themer-0.3.0/src/
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-05-07 19:48:43.364713 shell-themer-0.3.0/src/shell_themer/
+-rw-r--r--   0 jared      (501) staff       (20)     1228 2023-04-14 15:39:07.000000 shell-themer-0.3.0/src/shell_themer/__init__.py
+-rw-r--r--   0 jared      (501) staff       (20)     1350 2023-04-15 23:38:46.000000 shell-themer-0.3.0/src/shell_themer/__main__.py
+-rwxr-xr-x   0 jared      (501) staff       (20)    41947 2023-05-07 19:46:38.000000 shell-themer-0.3.0/src/shell_themer/themer.py
+-rw-r--r--   0 jared      (501) staff       (20)     1608 2023-04-15 03:09:24.000000 shell-themer-0.3.0/src/shell_themer/version.py
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-05-07 19:48:43.365429 shell-themer-0.3.0/src/shell_themer.egg-info/
+-rw-r--r--   0 jared      (501) staff       (20)     3596 2023-05-07 19:48:43.000000 shell-themer-0.3.0/src/shell_themer.egg-info/PKG-INFO
+-rw-r--r--   0 jared      (501) staff       (20)      595 2023-05-07 19:48:43.000000 shell-themer-0.3.0/src/shell_themer.egg-info/SOURCES.txt
+-rw-r--r--   0 jared      (501) staff       (20)        1 2023-05-07 19:48:43.000000 shell-themer-0.3.0/src/shell_themer.egg-info/dependency_links.txt
+-rw-r--r--   0 jared      (501) staff       (20)       65 2023-05-07 19:48:43.000000 shell-themer-0.3.0/src/shell_themer.egg-info/entry_points.txt
+-rw-r--r--   0 jared      (501) staff       (20)      168 2023-05-07 19:48:43.000000 shell-themer-0.3.0/src/shell_themer.egg-info/requires.txt
+-rw-r--r--   0 jared      (501) staff       (20)       13 2023-05-07 19:48:43.000000 shell-themer-0.3.0/src/shell_themer.egg-info/top_level.txt
+-rw-r--r--   0 jared      (501) staff       (20)     4195 2023-05-07 19:46:38.000000 shell-themer-0.3.0/tasks.py
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-05-07 19:48:43.366268 shell-themer-0.3.0/tests/
+-rw-r--r--   0 jared      (501) staff       (20)     2512 2023-04-15 21:59:15.000000 shell-themer-0.3.0/tests/conftest.py
+-rw-r--r--   0 jared      (501) staff       (20)    24310 2023-05-07 19:46:38.000000 shell-themer-0.3.0/tests/test_generate.py
+-rw-r--r--   0 jared      (501) staff       (20)     2150 2023-04-11 14:03:52.000000 shell-themer-0.3.0/tests/test_list.py
+-rw-r--r--   0 jared      (501) staff       (20)     7093 2023-04-15 23:38:46.000000 shell-themer-0.3.0/tests/test_main_dispatch.py
+-rw-r--r--   0 jared      (501) staff       (20)     2318 2023-04-11 15:55:44.000000 shell-themer-0.3.0/tests/test_preview.py
+-rw-r--r--   0 jared      (501) staff       (20)    14331 2023-05-07 19:46:38.000000 shell-themer-0.3.0/tests/test_themer.py
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-05-07 19:48:43.366392 shell-themer-0.3.0/themes/
+-rw-r--r--   0 jared      (501) staff       (20)     9310 2023-04-13 23:29:31.000000 shell-themer-0.3.0/themes/dracula.toml
```

### Comparing `shell-themer-0.2.0/CHANGELOG.md` & `shell-themer-0.3.0/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 are documented in this file.
 
 This project uses [Semantic Versioning](http://semver.org/spec/v2.0.0.html) and the
 format of this file follows recommendations from
 [Keep a Changelog](http://keepachangelog.com/en/1.0.0/).
 
 
+## [0.3.0] - 2023-05-07
+
+### Added
+
+- generator for [exa](https://the.exa.website/) colors
+
+
 ## [0.2.0] - 2023-04-19
 
 ### Added
 
 - variable and style interpolation
 - shell generator to run any shell command when activating a theme
 - add `--color` command line option and `SHELL_THEMER_COLORS` environment
```

### Comparing `shell-themer-0.2.0/CONTRIBUTING.md` & `shell-themer-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `shell-themer-0.2.0/LICENSE` & `shell-themer-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shell-themer-0.2.0/PKG-INFO` & `shell-themer-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-themer
-Version: 0.2.0
+Version: 0.3.0
 Summary: Use consistent color themes for a variety of command line tools.
 Author-email: Jared Crapo <jared@kotfu.net>
 License: MIT License
         
         Copyright (c) 2023 kotfu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `shell-themer-0.2.0/README.md` & `shell-themer-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `shell-themer-0.2.0/TODO.md` & `shell-themer-0.3.0/TODO.md`

 * *Files 9% similar despite different names*

```diff
@@ -8,16 +8,18 @@
   disable = true
   // exit code 0 is true, and means to disable it
   // any other exit code means to not disable it
   disable_if = "some shell command here"
   // if you have to negate the exit code, try
   // isiterm2 && [[ $? == 0 ]]
 [x] add option to generate to insert comments into the output
-[ ] allow creation of variables with values, which can be interpolated
+[x] allow creation of variables with values, which can be interpolated
     into other sections
+[ ] move environment variables into their own generator instead of
+    processing them in every generator
 
 - documentation and website
   - show how to set BAT_THEME
 - document how to load a theme
     - eval $(shell-themer) is bad, try the code from `$ starship init bash` instead
 - document a "magic" styles named "background", "foreground", and "text"
   - these will be used by the preview command to show the style properly
@@ -37,7 +39,15 @@
   - don't like process because we use processors for something else
   - generate seems the best so far, then we have generator = "fzf"
 - init = generate the code for the theme-activate (using fzf if not specified), theme-reload
 [x] honor NO_COLOR env variable
 [x] add --no-color option
 [x] add --colors= option
 [x] add SHELL_THEMER_COLORS env variable
+
+
+## Recipe ideas
+
+- show how to enable a scope only for a certain operating system
+- show how to enable a scope only on certain hosts
+- show how to run a macos shortcut from a scope
+-
```

### Comparing `shell-themer-0.2.0/pyproject.toml` & `shell-themer-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shell-themer-0.2.0/src/shell_themer/__init__.py` & `shell-themer-0.3.0/src/shell_themer/__init__.py`

 * *Files identical despite different names*

### Comparing `shell-themer-0.2.0/src/shell_themer/__main__.py` & `shell-themer-0.3.0/src/shell_themer/__main__.py`

 * *Files identical despite different names*

### Comparing `shell-themer-0.2.0/src/shell_themer/themer.py` & `shell-themer-0.3.0/src/shell_themer/themer.py`

 * *Files 13% similar despite different names*

```diff
@@ -567,15 +567,15 @@
             enabled_if = "{shell cmd}" returns a non-zero exit code
 
         if 'enabled = false' is present, then enabled_if is not checked
         """
         scopedef = self.scopedef_for(scope)
         try:
             enabled = scopedef["enabled"]
-            self._assert_bool(None, scope, "enabled", enabled)
+            self._assert_bool(enabled, None, scope, "enabled")
             # this is authoritative, if it exists, ignore enabled_if below
             return enabled
         except KeyError:
             # no enabled command, but we need to still keep checking
             pass
 
         try:
@@ -592,15 +592,15 @@
         proc = subprocess.run(enabled_if, shell=True, check=False, capture_output=True)
         if proc.returncode != 0:
             # the shell command returned a non-zero exit code
             # and this scope should therefore be disabled
             return False
         return True
 
-    def _assert_bool(self, generator, scope, key, value):
+    def _assert_bool(self, value, generator, scope, key):
         if not isinstance(value, bool):
             if generator:
                 errmsg = (
                     f"{self.prog}: {generator} generator for"
                     f" scope '{scope}' requires '{key}' to be true or false"
                 )
             else:
@@ -714,35 +714,37 @@
                 pass
 
         for scope in to_generate:
             # checking here in case they supplied a scope on the command line that
             # doesn't exist
             if self.has_scope(scope):
                 scopedef = self.scopedef_for(scope)
+                # find the generator for this scope
+                try:
+                    generator = scopedef["generator"]
+                except KeyError as exc:
+                    errmsg = f"{self.prog}: scope '{scope}' does not have a generator defined"
+                    raise ThemeError(errmsg) from exc
                 # check if the scope is disabled
                 if not self.is_enabled(scope):
                     if args.comment:
                         print(f"# [scope.{scope}] skipped because it is not enabled")
                     continue
-                # do the rendering elements for all scopes
+                # scope is enabled, so print the comment
                 if args.comment:
                     print(f"# [scope.{scope}]")
-                self._generate_environment(scope, scopedef)
-                # see if we have a generator defined for custom rendering
-                try:
-                    generator = scopedef["generator"]
-                except KeyError:
-                    # no more to do for this scope, skip to the next iteration
-                    # of the loop
-                    continue
 
-                if generator == "fzf":
+                if generator == "environment_variables":
+                    self._generate_environment(scope, scopedef)
+                elif generator == "fzf":
                     self._generate_fzf(scope, scopedef)
                 elif generator == "ls_colors":
                     self._generate_ls_colors(scope, scopedef)
+                elif generator == "exa_colors":
+                    self._generate_exa_colors(scope, scopedef)
                 elif generator == "iterm":
                     self._generate_iterm(scope, scopedef)
                 elif generator == "shell":
                     self._generate_shell(scope, scopedef)
                 else:
                     raise ThemeError(f"{self.prog}: {generator}: unknown generator")
             else:
@@ -894,15 +896,16 @@
         if style.strike:
             attribs += ":strikethrough"
         return attribs
 
     #
     # ls_colors generator
     #
-    LS_COLORS_MAP = {
+    LS_COLORS_BASE_MAP = {
+        # map both a friendly name and the "real" name
         "text": "no",
         "file": "fi",
         "directory": "di",
         "symlink": "ln",
         "multi_hard_link": "mh",
         "pipe": "pi",
         "socket": "so",
@@ -915,42 +918,53 @@
         "setgid": "sg",
         "sticky": "st",
         "other_writable": "ow",
         "sticky_other_writable": "tw",
         "executable_file": "ex",
         "file_with_capability": "ca",
     }
+    # this map allows you to either use the 'native' color code, or the
+    # 'friendly' name defined by shell-themer
+    LS_COLORS_MAP = {}
+    for friendly, actual in LS_COLORS_BASE_MAP.items():
+        LS_COLORS_MAP[friendly] = actual
+        LS_COLORS_MAP[actual] = actual
 
     def _generate_ls_colors(self, scope, scopedef):
         "Render a LS_COLORS variable suitable for GNU ls"
         outlist = []
+        havecodes = []
         # process the styles
         styles = self.styles_from(scopedef)
         # figure out if we are clearing builtin styles
         try:
             clear_builtin = scopedef["clear_builtin"]
-            self._assert_bool("ls_colors", scope, "clear_builtin", clear_builtin)
+            self._assert_bool(clear_builtin, "ls_colors", scope, "clear_builtin")
         except KeyError:
             clear_builtin = False
 
+        # iterate over the styles given in our configuration
+        for name, style in styles.items():
+            if style:
+                mapcode, render = self._ls_colors_from_style(
+                    name, style, self.LS_COLORS_MAP, scope
+                )
+                havecodes.append(mapcode)
+                outlist.append(render)
+
         if clear_builtin:
-            # iterate over all known styles
-            for name in self.LS_COLORS_MAP:
-                try:
-                    style = styles[name]
-                except KeyError:
-                    # style isn't in our configuration, so put the default one in
-                    style = self.get_style("default")
-                if style:
-                    outlist.append(self._ls_colors_from_style(scope, name, style))
-        else:
-            # iterate over the styles given in our configuration
-            for name, style in styles.items():
-                if style:
-                    outlist.append(self._ls_colors_from_style(scope, name, style))
+            style = self.get_style("default")
+            # go through all the color codes, and render them with the
+            # 'default' style and add them to the output
+            for name, code in self.LS_COLORS_BASE_MAP.items():
+                if not code in havecodes:
+                    _, render = self._ls_colors_from_style(
+                        name, style, self.LS_COLORS_MAP, scope
+                    )
+                    outlist.append(render)
 
         # process the filesets
 
         # figure out which environment variable to put it in
         try:
             varname = scopedef["environment_variable"]
             varname = self.variable_interpolate(varname)
@@ -959,35 +973,40 @@
 
         # even if outlist is empty, we have to set the variable, because
         # when we are switching a theme, there may be contents in the
         # environment variable already, and we need to tromp over them
         # we chose to set the variable to empty instead of unsetting it
         print(f'''export {varname}="{':'.join(outlist)}"''')
 
-    def _ls_colors_from_style(self, scope, name, style):
+    def _ls_colors_from_style(self, name, style, mapp, scope):
         """create an entry suitable for LS_COLORS from a style
 
         name should be a valid LS_COLORS entry, could be a code representing
         a file type, or a glob representing a file extension
 
         style is a style object
+
+        mapp is a dictionary of friendly color names to native color names
+            ie map['directory'] = 'di'
+
+        scope is the scope where this mapped occured, used for error message
         """
         ansicodes = ""
         if not style:
-            return ""
+            return "", ""
         try:
-            mapname = self.LS_COLORS_MAP[name]
+            mapname = mapp[name]
         except KeyError as exc:
             # they used a style for a file attribute that we don't know how to map
             # i.e. style.text or style.directory we know what to do with, but
             # style.bundleid we don't know how to map, so we generate an error
             raise ThemeError(
                 (
                     f"{self.prog}: unknown style '{name}' while processing"
-                    f"scope '{scope}' using the 'lscolors' generator"
+                    f" scope '{scope}' using the 'ls_colors' generator"
                 )
             ) from exc
 
         if style.color.type == rich.color.ColorType.DEFAULT:
             ansicodes = "0"
         else:
             # this works, but it uses a protected method
@@ -997,15 +1016,122 @@
             ansistring = style.render("-----")
             # style.render uses this string to build it's output
             # f"\x1b[{attrs}m{text}\x1b[0m"
             # so let's go split it apart
             match = re.match(r"^\x1b\[([;\d]*)m", ansistring)
             # and get the numeric codes
             ansicodes = match.group(1)
-        return f"{mapname}={ansicodes}"
+        return mapname, f"{mapname}={ansicodes}"
+
+    #
+    # exa color generator
+    #
+    EXA_COLORS_BASE_MAP = {
+        # map both a friendly name and the "real" name
+        "text": "no",
+        "file": "fi",
+        "directory": "di",
+        "symlink": "ln",
+        "multi_hard_link": "mh",
+        "pipe": "pi",
+        "socket": "so",
+        "door": "do",
+        "block_device": "bd",
+        "character_device": "cd",
+        "broken_symlink": "or",
+        "missing_symlink_target": "mi",
+        "setuid": "su",
+        "setgid": "sg",
+        "sticky": "st",
+        "other_writable": "ow",
+        "sticky_other_writable": "tw",
+        "executable_file": "ex",
+        "file_with_capability": "ca",
+        "perms_user_read": "ur",
+        "perms_user_write": "uw",
+        "perms_user_execute_files": "ux",
+        "perms_user_execute_directories": "ue",
+        "perms_group_read": "gr",
+        "perms_group_write": "gw",
+        "perms_group_execute": "gx",
+        "perms_other_read": "tr",
+        "perms_other_write": "tw",
+        "perms_other_execute": "tx",
+        "perms_suid_files": "su",
+        "perms_sticky_directories": "sf",
+        "perms_extended_attribute": "xa",
+        "size_number": "sn",
+        "size_unit": "sb",
+        "df": "df",
+        "ds": "ds",
+        "uu": "uu",
+        "un": "un",
+        "gu": "gu",
+        "gn": "gn",
+        "lc": "lc",
+        "lm": "lm",
+        "ga": "ga",
+        "gm": "gm",
+        "gd": "gd",
+        "gv": "gv",
+        "gt": "gt",
+        "punctuation": "xx",
+        "date_time": "da",
+        "in": "in",
+        "bl": "bl",
+        "column_headers": "hd",
+        "lp": "lp",
+        "cc": "cc",
+        "b0": "b0",
+    }
+    # this map allows you to either use the 'native' exa code, or the
+    # 'friendly' name defined by shell-themer
+    EXA_COLORS_MAP = {}
+    for friendly, actual in EXA_COLORS_BASE_MAP.items():
+        EXA_COLORS_MAP[friendly] = actual
+        EXA_COLORS_MAP[actual] = actual
+
+    def _generate_exa_colors(self, scope, scopedef):
+        "Render a EXA_COLORS variable suitable for exa"
+        outlist = []
+        # process the styles
+        styles = self.styles_from(scopedef)
+        # figure out if we are clearing builtin styles
+        try:
+            clear_builtin = scopedef["clear_builtin"]
+            self._assert_bool(clear_builtin, "exa_colors", scope, "clear_builtin")
+        except KeyError:
+            clear_builtin = False
+
+        if clear_builtin:
+            # this tells exa to not use any built-in/hardcoded colors
+            outlist.append("reset")
+
+        # iterate over the styles given in our configuration
+        for name, style in styles.items():
+            if style:
+                _, render = self._ls_colors_from_style(
+                    name, style, self.EXA_COLORS_MAP, scope
+                )
+                outlist.append(render)
+
+        # process the filesets
+
+        # figure out which environment variable to put it in
+        try:
+            varname = scopedef["environment_variable"]
+            varname = self.variable_interpolate(varname)
+        except KeyError:
+            varname = "EXA_COLORS"
+
+        # even if outlist is empty, we have to set the variable, because
+        # when we are switching a theme, there may be contents in the
+        # environment variable already, and we need to tromp over them
+        # we chose to set the variable to empty instead of unsetting it
+        print(f'''export {varname}="{':'.join(outlist)}"''')
 
     #
     # iterm generator and helpers
     #
     def _generate_iterm(self, _, scopedef):
         """send the special escape sequences to make the iterm2
         terminal emulator for macos change its foreground and backgroud
```

### Comparing `shell-themer-0.2.0/src/shell_themer/version.py` & `shell-themer-0.3.0/src/shell_themer/version.py`

 * *Files identical despite different names*

### Comparing `shell-themer-0.2.0/src/shell_themer.egg-info/PKG-INFO` & `shell-themer-0.3.0/src/shell_themer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-themer
-Version: 0.2.0
+Version: 0.3.0
 Summary: Use consistent color themes for a variety of command line tools.
 Author-email: Jared Crapo <jared@kotfu.net>
 License: MIT License
         
         Copyright (c) 2023 kotfu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `shell-themer-0.2.0/src/shell_themer.egg-info/SOURCES.txt` & `shell-themer-0.3.0/src/shell_themer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shell-themer-0.2.0/tasks.py` & `shell-themer-0.3.0/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
 
 namespace.add_task(build)
 
 
 @invoke.task(pre=[build])
 def pypi(context):
     "Build and upload a distribution to pypi"
-    context.run("twine upload --respository pypi dist/*")
+    context.run("twine upload --repository pypi dist/*")
 
 
 namespace.add_task(pypi)
 
 
 @invoke.task(pre=[build])
 def pypi_test(context):
```

### Comparing `shell-themer-0.2.0/tests/conftest.py` & `shell-themer-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shell-themer-0.2.0/tests/test_generate.py` & `shell-themer-0.3.0/tests/test_generate.py`

 * *Files 8% similar despite different names*

```diff
@@ -121,92 +121,24 @@
     assert not out
     assert not err
 
 
 #
 # test rendering of elements common to all scopes
 #
-ENV_INTERPOLATIONS = [
-    ("{style:dark_orange}", "#ff6c1c"),
-    ("{style:dark_orange:hex}", "#ff6c1c"),
-    ("{style:dark_orange:hexnohash}", "ff6c1c"),
-    # for an unknown format or style, don't do any replacement
-    ("{style:current_line}", "{style:current_line}"),
-    ("{style:dark_orange:unknown}", "{style:dark_orange:unknown}"),
-    # we have to have the style keyword, or it all just gets passed through
-    ("{dark_orange}", "{dark_orange}"),
-    ("{variable:green}", "{variable:green}"),
-    # escaped opening bracket, becasue this is toml, if you want a backslash
-    # you have to you \\ because toml strings can contain escape sequences
-    (r"\\{style:bright_blue}", "{style:bright_blue}"),
-    # if you don't have matched brackets, or are missing the
-    # literal 'style:' keyword, don't expect the backslash
-    # to be removed. again here we have two backslashes in the first
-    # argument so that it will survive toml string escaping
-    (r"\\{ some other  things}", r"\{ some other  things}"),
-    (r"\\{escaped unmatched bracket", r"\{escaped unmatched bracket"),
-    # try a mixed variable and style interpolation
-    ("{style:dark_orange} {var:someopts}", "#ff6c1c --option=fred -v"),
-]
-
-
-@pytest.mark.parametrize("phrase, interpolated", ENV_INTERPOLATIONS)
-def test_generate_environment_interpolation(thm_cmdline, capsys, phrase, interpolated):
-    tomlstr = f"""
-        [variables]
-        someopts = "--option=fred -v"
-
-        [styles]
-        dark_orange = "#ff6c1c"
-
-        [scope.gum]
-        environment.export.GUM_OPTS = " --cursor-foreground={phrase}"
-    """
-    exit_code = thm_cmdline("generate", tomlstr)
-    out, err = capsys.readouterr()
-    assert exit_code == Themer.EXIT_SUCCESS
-    assert out == f'export GUM_OPTS=" --cursor-foreground={interpolated}"\n'
-
-
-def test_generate_environment_unset_list(thm_cmdline, capsys):
-    tomlstr = """
-        [scope.ls]
-        # set some environment variables
-        environment.unset = ["SOMEVAR", "ANOTHERVAR"]
-        environment.export.LS_COLORS = "ace ventura"
-    """
-    exit_code = thm_cmdline("generate", tomlstr)
-    out, err = capsys.readouterr()
-    assert exit_code == Themer.EXIT_SUCCESS
-    assert not err
-    assert "unset SOMEVAR" in out
-    assert "unset ANOTHERVAR" in out
-    assert 'export LS_COLORS="ace ventura"' in out
-
-
-def test_generate_environment_unset_string(thm_cmdline, capsys):
-    tomlstr = """
-        [scope.unset]
-        environment.unset = "NOLISTVAR"
-    """
-    exit_code = thm_cmdline("generate", tomlstr)
-    out, err = capsys.readouterr()
-    assert exit_code == Themer.EXIT_SUCCESS
-    assert not err
-    assert "unset NOLISTVAR" in out
-
-
 def test_generate_enabled(thm_cmdline, capsys):
     tomlstr = """
         [scope.nolistvar]
         enabled = false
+        generator = "environment_variables"
         environment.unset = "NOLISTVAR"
 
         [scope.somevar]
         enabled = true
+        generator = "environment_variables"
         environment.unset = "SOMEVAR"
     """
     exit_code = thm_cmdline("generate", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_SUCCESS
     assert not err
     assert "unset SOMEVAR" in out
@@ -214,41 +146,44 @@
 
 
 def test_generate_enabled_false_enabled_if_ignored(thm_cmdline, capsys):
     tomlstr = """
         [scope.unset]
         enabled = false
         enabled_if = "[[ 1 == 1 ]]"
+        generator = "environment_variables"
         environment.unset = "NOLISTVAR"
     """
     exit_code = thm_cmdline("generate", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_SUCCESS
     assert not err
     assert not out
 
 
 def test_generate_enabled_true_enabed_if_ignored(thm_cmdline, capsys):
     tomlstr = """
         [scope.unset]
         enabled = true
         enabled_if = "[[ 0 == 1 ]]"
+        generator = "environment_variables"
         environment.unset = "NOLISTVAR"
     """
     exit_code = thm_cmdline("generate", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_SUCCESS
     assert not err
     assert "unset NOLISTVAR" in out
 
 
 def test_generate_enabled_invalid_value(thm_cmdline, capsys):
     tomlstr = """
         [scope.unset]
         enabled = "notaboolean"
+        generator = "environment_variables"
         environment.unset = "NOLISTVAR"
     """
     exit_code = thm_cmdline("generate", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_ERROR
     assert not out
     assert "to be true or false" in err
@@ -269,14 +204,15 @@
     tomlstr = f"""
         [variables]
         echocmd = "/bin/echo"
         falsetest = "[[ 1 == 0]]"
 
         [scope.unset]
         enabled_if = "{cmd}"
+        generator = "environment_variables"
         environment.unset = "ENVVAR"
     """
     exit_code = thm_cmdline("generate", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_SUCCESS
     assert not err
     if enabled:
@@ -285,18 +221,20 @@
         assert not out
 
 
 def test_generate_comments(thm_cmdline, capsys):
     tomlstr = """
         [scope.nolistvar]
         enabled = false
+        generator = "environment_variables"
         environment.unset = "NOLISTVAR"
 
         [scope.somevar]
         enabled = true
+        generator = "environment_variables"
         environment.unset = "SOMEVAR"
     """
     exit_code = thm_cmdline("generate --comment", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_SUCCESS
     assert not err
     assert "# [scope.nolistvar]" in out
@@ -308,20 +246,108 @@
 def test_unknown_generator(thm_cmdline, capsys):
     tomlstr = """
         [scope.myprog]
         generator = "mrfusion"
         environment.unset = "SOMEVAR"
     """
     exit_code = thm_cmdline("generate", tomlstr)
-    out, err = capsys.readouterr()
+    _, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_ERROR
     assert "unknown generator" in err
     assert "mrfusion" in err
 
 
+def test_no_generator(thm_cmdline, capsys):
+    tomlstr = """
+        [scope.myscope]
+        enabled = false
+    """
+    exit_code = thm_cmdline("generate", tomlstr)
+    _, err = capsys.readouterr()
+    assert exit_code == Themer.EXIT_ERROR
+    assert "does not have a generator defined" in err
+    assert "myscope" in err
+
+
+#
+# test the environment_variables generator
+#
+ENV_INTERPOLATIONS = [
+    ("{style:dark_orange}", "#ff6c1c"),
+    ("{style:dark_orange:hex}", "#ff6c1c"),
+    ("{style:dark_orange:hexnohash}", "ff6c1c"),
+    # for an unknown format or style, don't do any replacement
+    ("{style:current_line}", "{style:current_line}"),
+    ("{style:dark_orange:unknown}", "{style:dark_orange:unknown}"),
+    # we have to have the style keyword, or it all just gets passed through
+    ("{dark_orange}", "{dark_orange}"),
+    ("{variable:green}", "{variable:green}"),
+    # escaped opening bracket, becasue this is toml, if you want a backslash
+    # you have to you \\ because toml strings can contain escape sequences
+    (r"\\{style:bright_blue}", "{style:bright_blue}"),
+    # if you don't have matched brackets, or are missing the
+    # literal 'style:' keyword, don't expect the backslash
+    # to be removed. again here we have two backslashes in the first
+    # argument so that it will survive toml string escaping
+    (r"\\{ some other  things}", r"\{ some other  things}"),
+    (r"\\{escaped unmatched bracket", r"\{escaped unmatched bracket"),
+    # try a mixed variable and style interpolation
+    ("{style:dark_orange} {var:someopts}", "#ff6c1c --option=fred -v"),
+]
+
+
+@pytest.mark.parametrize("phrase, interpolated", ENV_INTERPOLATIONS)
+def test_generate_environment_interpolation(thm_cmdline, capsys, phrase, interpolated):
+    tomlstr = f"""
+        [variables]
+        someopts = "--option=fred -v"
+
+        [styles]
+        dark_orange = "#ff6c1c"
+
+        [scope.gum]
+        generator = "environment_variables"
+        environment.export.GUM_OPTS = " --cursor-foreground={phrase}"
+    """
+    exit_code = thm_cmdline("generate", tomlstr)
+    out, err = capsys.readouterr()
+    assert exit_code == Themer.EXIT_SUCCESS
+    assert out == f'export GUM_OPTS=" --cursor-foreground={interpolated}"\n'
+
+
+def test_generate_environment_unset_list(thm_cmdline, capsys):
+    tomlstr = """
+        [scope.ls]
+        generator = "environment_variables"
+        # set some environment variables
+        environment.unset = ["SOMEVAR", "ANOTHERVAR"]
+        environment.export.LS_COLORS = "ace ventura"
+    """
+    exit_code = thm_cmdline("generate", tomlstr)
+    out, err = capsys.readouterr()
+    assert exit_code == Themer.EXIT_SUCCESS
+    assert not err
+    assert "unset SOMEVAR" in out
+    assert "unset ANOTHERVAR" in out
+    assert 'export LS_COLORS="ace ventura"' in out
+
+
+def test_generate_environment_unset_string(thm_cmdline, capsys):
+    tomlstr = """
+        [scope.unset]
+        generator = "environment_variables"
+        environment.unset = "NOLISTVAR"
+    """
+    exit_code = thm_cmdline("generate", tomlstr)
+    out, err = capsys.readouterr()
+    assert exit_code == Themer.EXIT_SUCCESS
+    assert not err
+    assert "unset NOLISTVAR" in out
+
+
 #
 # test the fzf generator
 #
 ATTRIBS_TO_FZF = [
     ("bold", "regular:bold"),
     ("underline", "regular:underline"),
     ("reverse", "regular:reverse"),
@@ -422,15 +448,15 @@
     ("text", "", ""),
     ("text", "default", "no=0"),
     ("file", "default", "fi=0"),
     ("directory", "#8be9fd", "di=38;2;139;233;253"),
     ("symlink", "green4 bold", "ln=1;38;5;28"),
     ("multi_hard_link", "blue on white", "mh=34;47"),
     ("pipe", "#f8f8f2 on #44475a underline", "pi=4;38;2;248;248;242;48;2;68;71;90"),
-    ("socket", "bright_white", "so=97"),
+    ("so", "bright_white", "so=97"),
     ("door", "bright_white", "do=97"),
     ("block_device", "default", "bd=0"),
     ("character_device", "black", "cd=30"),
     ("broken_symlink", "bright_blue", "or=94"),
     ("missing_symlink_target", "bright_blue", "mi=94"),
     ("setuid", "bright_blue", "su=94"),
     ("setgid", "bright_red", "sg=91"),
@@ -438,18 +464,20 @@
     ("other_writable", "blue_violet italic", "ow=3;38;5;57"),
     ("sticky_other_writable", "deep_pink2 on #ffffaf", "tw=38;5;197;48;2;255;255;175"),
     ("executable_file", "cornflower_blue on grey82", "ex=38;5;69;48;5;252"),
     ("file_with_capability", "red on black", "ca=31;40"),
 ]
 
 
-@pytest.mark.parametrize("name, styledef, lsc", STYLE_TO_LSCOLORS)
-def test_ls_colors_from_style(thm, name, styledef, lsc):
+@pytest.mark.parametrize("name, styledef, expected", STYLE_TO_LSCOLORS)
+def test_ls_colors_from_style(thm, name, styledef, expected):
     style = rich.style.Style.parse(styledef)
-    assert lsc == thm._ls_colors_from_style("scope", name, style)
+    code, render = thm._ls_colors_from_style(name, style, thm.LS_COLORS_MAP, "scope")
+    assert render == expected
+    assert code == expected[0:2]
 
 
 def test_ls_colors_no_styles(thm_cmdline, capsys):
     tomlstr = """
         [scope.lsc]
         generator = "ls_colors"
     """
@@ -495,15 +523,15 @@
         style.directory = "bright_blue"
     """
     exit_code = thm_cmdline("generate", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_SUCCESS
     assert not err
     expected = (
-        'export LS_COLORS="no=0:fi=0:di=94:ln=0:'
+        'export LS_COLORS="di=94:no=0:fi=0:ln=0:'
         "mh=0:pi=0:so=0:do=0:bd=0:cd=0:or=0:mi=0:"
         'su=0:sg=0:st=0:ow=0:tw=0:ex=0:ca=0"\n'
     )
     assert out == expected
 
 
 def test_ls_colors_clear_builtin_not_boolean(thm_cmdline, capsys):
@@ -513,14 +541,124 @@
         clear_builtin = "error"
         style.directory = "bright_blue"
     """
     exit_code = thm_cmdline("generate", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_ERROR
     assert not out
+    assert "'clear_builtin' to be true or false" in err
+
+
+#
+# test the exa_colors generator
+#
+# we only reallly have to test that the style name maps to the right code in ls_colors
+# ie directory -> di, or setuid -> su. The ansi codes are created by rich.style
+# so we don't really need to test much of that
+STYLE_TO_EXACOLORS = [
+    ("text", "", ""),
+    ("text", "default", "no=0"),
+    ("file", "default", "fi=0"),
+    ("directory", "#8be9fd", "di=38;2;139;233;253"),
+    ("symlink", "green4 bold", "ln=1;38;5;28"),
+    ("multi_hard_link", "blue on white", "mh=34;47"),
+    ("pi", "#f8f8f2 on #44475a underline", "pi=4;38;2;248;248;242;48;2;68;71;90"),
+    ("socket", "bright_white", "so=97"),
+    ("door", "bright_white", "do=97"),
+    ("block_device", "default", "bd=0"),
+    ("character_device", "black", "cd=30"),
+    ("broken_symlink", "bright_blue", "or=94"),
+    ("missing_symlink_target", "bright_blue", "mi=94"),
+    ("setuid", "bright_blue", "su=94"),
+    ("setgid", "bright_red", "sg=91"),
+    ("sticky", "blue_violet", "st=38;5;57"),
+    ("other_writable", "blue_violet italic", "ow=3;38;5;57"),
+    ("sticky_other_writable", "deep_pink2 on #ffffaf", "tw=38;5;197;48;2;255;255;175"),
+    ("executable_file", "cornflower_blue on grey82", "ex=38;5;69;48;5;252"),
+    ("file_with_capability", "red on black", "ca=31;40"),
+    ("sn", "#7060eb", "sn=38;2;112;96;235"),
+]
+
+
+@pytest.mark.parametrize("name, styledef, expected", STYLE_TO_EXACOLORS)
+def test_exa_colors_from_style(thm, name, styledef, expected):
+    style = rich.style.Style.parse(styledef)
+    code, render = thm._ls_colors_from_style(name, style, thm.EXA_COLORS_MAP, "scope")
+    assert render == expected
+    assert code == expected[0:2]
+
+
+def test_exa_colors_no_styles(thm_cmdline, capsys):
+    tomlstr = """
+        [scope.exac]
+        generator = "exa_colors"
+    """
+    exit_code = thm_cmdline("generate", tomlstr)
+    out, err = capsys.readouterr()
+    assert exit_code == Themer.EXIT_SUCCESS
+    assert not err
+    assert out == 'export EXA_COLORS=""\n'
+
+
+def test_exa_colors_unknown_style(thm_cmdline, capsys):
+    tomlstr = """
+        [scope.exac]
+        generator = "exa_colors"
+        style.bundleid = "default"
+    """
+    exit_code = thm_cmdline("generate", tomlstr)
+    out, err = capsys.readouterr()
+    assert exit_code == Themer.EXIT_ERROR
+    assert "unknown style" in err
+    assert "exac" in err
+
+
+def test_exa_colors_environment_variable(thm_cmdline, capsys):
+    tomlstr = """
+        [scope.exac]
+        generator = "exa_colors"
+        environment_variable = "OTHER_EXA_COLOR"
+        style.file = "default"
+        style.size_number = "#7060eb"
+    """
+    exit_code = thm_cmdline("generate", tomlstr)
+    out, err = capsys.readouterr()
+    assert exit_code == Themer.EXIT_SUCCESS
+    assert not err
+    assert out == 'export OTHER_EXA_COLOR="fi=0:sn=38;2;112;96;235"\n'
+
+
+def test_exa_colors_clear_builtin(thm_cmdline, capsys):
+    tomlstr = """
+        [scope.exac]
+        generator = "exa_colors"
+        clear_builtin = true
+        style.directory = "bright_blue"
+        style.uu = "bright_red"
+        style.punctuation = "#555555"
+    """
+    exit_code = thm_cmdline("generate", tomlstr)
+    out, err = capsys.readouterr()
+    assert exit_code == Themer.EXIT_SUCCESS
+    assert not err
+    expected = 'export EXA_COLORS="reset:di=94:uu=91:xx=38;2;85;85;85"\n'
+    assert out == expected
+
+
+def test_exa_colors_clear_builtin_not_boolean(thm_cmdline, capsys):
+    tomlstr = """
+        [scope.exac]
+        generator = "exa_colors"
+        clear_builtin = "error"
+        style.directory = "bright_blue"
+    """
+    exit_code = thm_cmdline("generate", tomlstr)
+    out, err = capsys.readouterr()
+    assert exit_code == Themer.EXIT_ERROR
+    assert not out
     assert "'clear_builtin' to be true or false" in err
 
 
 #
 # test the iterm generator
 #
 def test_iterm(thm_cmdline, capsys):
```

### Comparing `shell-themer-0.2.0/tests/test_list.py` & `shell-themer-0.3.0/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `shell-themer-0.2.0/tests/test_main_dispatch.py` & `shell-themer-0.3.0/tests/test_main_dispatch.py`

 * *Files identical despite different names*

### Comparing `shell-themer-0.2.0/tests/test_preview.py` & `shell-themer-0.3.0/tests/test_preview.py`

 * *Files identical despite different names*

### Comparing `shell-themer-0.2.0/tests/test_themer.py` & `shell-themer-0.3.0/tests/test_themer.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,18 +305,18 @@
     (0.5, False),
 ]
 
 
 @pytest.mark.parametrize("val, expected", BOOL_TESTS)
 def test_assert_bool(thm, val, expected):
     if expected:
-        thm._assert_bool("generator", "scope", "key", val)
+        thm._assert_bool(val, "generator", "scope", "key")
     else:
         with pytest.raises(ThemeError):
-            thm._assert_bool("generator", "scope", "key", val)
+            thm._assert_bool(val, "generator", "scope", "key")
 
 
 #
 # test theme_dir() property
 #
 def test_theme_dir_environment_variable(thm, mocker, tmp_path):
     mocker.patch.dict(os.environ, {"THEME_DIR": str(tmp_path)})
```

### Comparing `shell-themer-0.2.0/themes/dracula.toml` & `shell-themer-0.3.0/themes/dracula.toml`

 * *Files identical despite different names*

