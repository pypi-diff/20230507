# Comparing `tmp/pyprojectx-1.0.0b3.tar.gz` & `tmp/pyprojectx-1.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprojectx-1.0.0b3.tar", last modified: Wed Apr 12 12:44:51 2023, max compression
+gzip compressed data, was "pyprojectx-1.0.0b4.tar", last modified: Sun May  7 12:42:55 2023, max compression
```

## Comparing `pyprojectx-1.0.0b3.tar` & `pyprojectx-1.0.0b4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1071 2023-04-12 12:42:32.085685 pyprojectx-1.0.0b3/LICENSE
--rw-r--r--   0        0        0     4600 2023-04-12 12:42:32.085685 pyprojectx-1.0.0b3/README.md
--rw-r--r--   0        0        0     3345 2023-04-12 12:44:51.825925 pyprojectx-1.0.0b3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/src/pyprojectx/__init__.py
--rw-r--r--   0        0        0     4218 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/src/pyprojectx/cli.py
--rw-r--r--   0        0        0     6435 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/src/pyprojectx/config.py
--rw-r--r--   0        0        0     5537 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/src/pyprojectx/env.py
--rw-r--r--   0        0        0        0 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/src/pyprojectx/initializer/__init__.py
--rw-r--r--   0        0        0      348 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/src/pyprojectx/initializer/global-template.toml
--rw-r--r--   0        0        0     7226 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/src/pyprojectx/initializer/initializers.py
--rw-r--r--   0        0        0      839 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/src/pyprojectx/initializer/pdm-template.toml
--rw-r--r--   0        0        0      858 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/src/pyprojectx/initializer/poetry-template.toml
--rw-r--r--   0        0        0       32 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/src/pyprojectx/initializer/poetry.toml
--rw-r--r--   0        0        0      863 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/src/pyprojectx/initializer/project-template.toml
--rw-r--r--   0        0        0      303 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/src/pyprojectx/log.py
--rw-r--r--   0        0        0        0 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/src/pyprojectx/wrapper/__init__.py
--rw-r--r--   0        0        0       30 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/src/pyprojectx/wrapper/pw.bat
--rwxr-xr-x   0        0        0     5804 2023-04-12 12:42:44.689711 pyprojectx-1.0.0b3/src/pyprojectx/wrapper/pw.py
--rwxr-xr-x   0        0        0      253 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/src/pyprojectx/wrapper/px
--rw-r--r--   0        0        0      373 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/src/pyprojectx/wrapper/px.bat
--rwxr-xr-x   0        0        0      275 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/src/pyprojectx/wrapper/pxg
--rw-r--r--   0        0        0      270 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/src/pyprojectx/wrapper/pxg.bat
--rw-r--r--   0        0        0        0 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/tests/__init__.py
--rw-r--r--   0        0        0      907 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/tests/conftest.py
--rw-r--r--   0        0        0      188 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/tests/data/alias-abbreviations.toml
--rw-r--r--   0        0        0       21 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/tests/data/invalid.toml
--rw-r--r--   0        0        0      682 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/tests/data/pw-test.toml
--rw-r--r--   0        0        0       19 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/tests/data/test-no-config.toml
--rw-r--r--   0        0        0       94 2023-04-12 12:42:32.089685 pyprojectx-1.0.0b3/tests/data/test-no-tool-config.toml
--rw-r--r--   0        0        0      644 2023-04-12 12:42:32.093685 pyprojectx-1.0.0b3/tests/data/test.toml
--rw-r--r--   0        0        0        0 2023-04-12 12:42:32.093685 pyprojectx-1.0.0b3/tests/integration/__init__.py
--rw-r--r--   0        0        0     5380 2023-04-12 12:42:32.093685 pyprojectx-1.0.0b3/tests/integration/test_pw.py
--rw-r--r--   0        0        0     4046 2023-04-12 12:42:32.093685 pyprojectx-1.0.0b3/tests/integration/test_px.py
--rw-r--r--   0        0        0        0 2023-04-12 12:42:32.093685 pyprojectx-1.0.0b3/tests/unit/__init__.py
--rw-r--r--   0        0        0     6940 2023-04-12 12:42:32.093685 pyprojectx-1.0.0b3/tests/unit/test_cli.py
--rw-r--r--   0        0        0     4034 2023-04-12 12:42:32.093685 pyprojectx-1.0.0b3/tests/unit/test_config.py
--rw-r--r--   0        0        0     3139 2023-04-12 12:42:32.093685 pyprojectx-1.0.0b3/tests/unit/test_env.py
--rw-r--r--   0        0        0     5286 1970-01-01 00:00:00.000000 pyprojectx-1.0.0b3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/LICENSE
+-rw-r--r--   0        0        0     4600 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/README.md
+-rw-r--r--   0        0        0     4217 2023-05-07 12:42:55.060940 pyprojectx-1.0.0b4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/__init__.py
+-rw-r--r--   0        0        0     5041 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/cli.py
+-rw-r--r--   0        0        0     6377 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/config.py
+-rw-r--r--   0        0        0     5471 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/env.py
+-rw-r--r--   0        0        0        0 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/initializer/__init__.py
+-rw-r--r--   0        0        0      348 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/initializer/global-template.toml
+-rw-r--r--   0        0        0     7263 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/initializer/initializers.py
+-rw-r--r--   0        0        0      839 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/initializer/pdm-template.toml
+-rw-r--r--   0        0        0      858 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/initializer/poetry-template.toml
+-rw-r--r--   0        0        0       32 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/initializer/poetry.toml
+-rw-r--r--   0        0        0      863 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/initializer/project-template.toml
+-rw-r--r--   0        0        0      303 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/log.py
+-rw-r--r--   0        0        0        0 2023-05-07 12:40:54.835344 pyprojectx-1.0.0b4/src/pyprojectx/wrapper/__init__.py
+-rw-r--r--   0        0        0       30 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/src/pyprojectx/wrapper/pw.bat
+-rwxr-xr-x   0        0        0     5949 2023-05-07 12:41:03.159443 pyprojectx-1.0.0b4/src/pyprojectx/wrapper/pw.py
+-rwxr-xr-x   0        0        0      253 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/src/pyprojectx/wrapper/px
+-rw-r--r--   0        0        0      373 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/src/pyprojectx/wrapper/px.bat
+-rwxr-xr-x   0        0        0      275 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/src/pyprojectx/wrapper/pxg
+-rw-r--r--   0        0        0      270 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/src/pyprojectx/wrapper/pxg.bat
+-rw-r--r--   0        0        0        0 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/__init__.py
+-rw-r--r--   0        0        0      905 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/conftest.py
+-rw-r--r--   0        0        0      188 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/data/alias-abbreviations.toml
+-rw-r--r--   0        0        0       21 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/data/invalid.toml
+-rw-r--r--   0        0        0      682 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/data/pw-test.toml
+-rw-r--r--   0        0        0       19 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/data/test-no-config.toml
+-rw-r--r--   0        0        0       94 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/data/test-no-tool-config.toml
+-rw-r--r--   0        0        0      644 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/data/test.toml
+-rw-r--r--   0        0        0        0 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/integration/__init__.py
+-rw-r--r--   0        0        0     5341 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/integration/test_pw.py
+-rw-r--r--   0        0        0     4008 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/integration/test_px.py
+-rw-r--r--   0        0        0        0 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/unit/__init__.py
+-rw-r--r--   0        0        0     6968 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/unit/test_cli.py
+-rw-r--r--   0        0        0     4038 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/unit/test_config.py
+-rw-r--r--   0        0        0     3142 2023-05-07 12:40:54.839344 pyprojectx-1.0.0b4/tests/unit/test_env.py
+-rw-r--r--   0        0        0     5411 1970-01-01 00:00:00.000000 pyprojectx-1.0.0b4/PKG-INFO
```

### Comparing `pyprojectx-1.0.0b3/LICENSE` & `pyprojectx-1.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b3/README.md` & `pyprojectx-1.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b3/src/pyprojectx/config.py` & `pyprojectx-1.0.0b4/src/pyprojectx/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,31 +6,27 @@
 
 import tomli
 
 from pyprojectx.wrapper.pw import BLUE, CYAN, RESET
 
 
 class Config:
-    """
-    Encapsulates the PyprojectX config inside a toml file
-    """
+    """Encapsulates the PyprojectX config inside a toml file."""
 
     def __init__(self, toml_path: Path) -> None:
-        """
-        :param toml_path: The toml config file
-        """
+        """:param toml_path: The toml config file"""
         self._toml_path = toml_path
         try:
-            with open(self._toml_path, "rb") as f:
+            with toml_path.open("rb") as f:
                 toml_dict = tomli.load(f)
                 self._tools = toml_dict.get("tool", {}).get("pyprojectx", {})
                 self._aliases = self._tools.get("aliases", {})
                 self._os_aliases = self._merge_os_aliases()
-        except Exception as e:
-            raise Warning(f"Could not parse {self._toml_path}: {e}") from e
+        except Exception as e:  # noqa: BLE001
+            raise Warning(f"Could not parse {toml_path}: {e}") from e
 
     def show_info(self, cmd, error=False):
         tool, alias = self.get_alias(cmd)
         out = sys.stderr if error else sys.stdout
         if alias:
             print(f"{cmd}{BLUE} is an alias in {CYAN}{self._toml_path.absolute()}", file=sys.stderr)
             if tool:
@@ -49,16 +45,16 @@
                 )
             print(f"{BLUE}available aliases:{RESET}", file=sys.stderr)
             print("\n".join(self._aliases.keys()), file=out)
             print(f"{BLUE}available tools:{RESET}", file=sys.stderr)
             print("\n".join(self._tools.keys() - ["aliases", "os"]), file=out)
 
     def get_tool_requirements(self, key) -> dict:
-        """
-        Get the requirements (dependencies) for a configured tool in the [tool.pyprojectx] section.
+        """Get the requirements (dependencies) for a configured tool in the [tool.pyprojectx] section.
+
         The requirements can either be specified as a string, a list of strings or an object with requirements and
         post-install as keys.
         A multiline string is treated as one requirement per line.
         :param key: The key (tool name) to look for
         :return: a dict with the requirements as a list and the post-install script, or None if key is not found
         """
         requirements_config = self._tools.get(key)
@@ -74,26 +70,26 @@
                 requirements = reqs.splitlines()
             if isinstance(reqs, list):
                 requirements = reqs
             post_install = requirements_config.get("post-install")
         return {"requirements": requirements, "post-install": post_install}
 
     def is_tool(self, key) -> bool:
-        """
-        Check whether a key (tool name) exists in the [tool.pyprojectx] section.
+        """Check whether a key (tool name) exists in the [tool.pyprojectx] section.
+
         :param key: The key (tool name) to look for
         :return: True if the key exists in the [tool.pyprojectx] section.
         """
         return self._tools.get(key) is not None
 
     def get_alias(self, key) -> Tuple[Optional[str], Optional[str]]:
-        """
-        Get an alias command configured in the [tool.pyprojectx.alias] section.
+        """Get an alias command configured in the [tool.pyprojectx.alias] section.
+
         The alias is considered to be part of a tool if its command starts with the name of the tool
-        or if the the command starts with '@tool-name:'.
+        or if the command starts with '@tool-name:'.
         :param key: The key (name) of the alias
         :return: A tuple containing the corresponding tool (or None) and
          the alias command (without the optional @tool-name part), or None if there is no alias with the given key.
         """
         alias_cmd = self._aliases.get(key)
         if not alias_cmd:
             return None, None
@@ -106,27 +102,27 @@
             return tool, alias_cmd
         tool = alias_cmd.split()[0]
         if self.is_tool(tool):
             return tool, alias_cmd
         return None, alias_cmd
 
     def find_aliases(self, abbrev: str) -> List[str]:
-        """
-        Find all alias keys that match the abbreviation.
+        """Find all alias keys that match the abbreviation.
+
         The abbreviation can use camel case patterns that are expanded to match camel case and kebab case names.
         For example the pattern foBa (or even fB) matches fooBar and foo-bar.
         If the abbreviation is exactly equal to an alias key, only that key is returned, even if the abbreviation
         matches other alias keys.
         :param abbrev: abbreviated or full alias key to search for
         :return: a list of matching alias keys
         """
-        if abbrev in self._aliases.keys():
+        if abbrev in self._aliases:
             return [abbrev]
 
-        return [key for key in self._aliases.keys() if camel_match(abbrev, key)]
+        return [key for key in self._aliases if camel_match(abbrev, key)]
 
     def __repr__(self):
         return str(self._tools)
 
     def _merge_os_aliases(self):
         aliases = self._tools.get("aliases", {})
         os_dict = self._tools.get("os", {})
@@ -141,11 +137,11 @@
     full_parts = to_camel_parts(key)
     return all(f.startswith(s) for s, f in zip_longest(abbrev_parts, full_parts, fillvalue=""))
 
 
 def to_camel_parts(key):
     if not key:
         return []
-    if len(key) < 2:
+    if len(key) < 2:  # noqa PLR2004
         return [key]
     camel = re.sub(r"(-\w)", lambda m: m.group(0)[1].upper(), key)
     return filter(len, re.split("([A-Z][^A-Z]*)", camel[0].lower() + camel[1:]))
```

### Comparing `pyprojectx-1.0.0b3/src/pyprojectx/env.py` & `pyprojectx-1.0.0b4/src/pyprojectx/env.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-"""
-Creates and manages isolated build environments.
-"""
+# ruff: noqa: S324
+"""Creates and manages isolated build environments."""
 import hashlib
 import os
 import shutil
 import subprocess
 import sys
 import tempfile
 from collections import OrderedDict
@@ -19,92 +18,82 @@
 def calculate_path(base_path: Path, name: str, requirements: Iterable[str], post_install: str) -> Path:
     md5 = hashlib.md5()
     for req in requirements:
         md5.update(req.strip().encode())
     if post_install:
         md5.update(post_install.strip().encode())
     return Path(
-        base_path, f"{name.lower()}-{md5.hexdigest()}-py{sys.version_info.major}.{sys.version_info.minor}"
+        base_path,
+        f"{name.lower()}-{md5.hexdigest()}-py{sys.version_info.major}.{sys.version_info.minor}",
     ).absolute()
 
 
 class IsolatedVirtualEnv:
-    """
-    Encapsulates the location and installation of an isolated virtual environment.
-    """
+    """Encapsulates the location and installation of an isolated virtual environment."""
 
     def __init__(self, base_path: Path, name: str, requirements_config: dict) -> None:
-        """
+        """Construct an IsolatedVirtualEnv.
+
         :param base_path: The base path for all environments
         :param name: The name for the environment
         :param requirements_config: The requirements and post-install script to install in the environment
         """
         self._name = name
         self._base_path = base_path
         self._requirements = requirements_config.get("requirements", [])
         self._path = calculate_path(base_path, name, self._requirements, requirements_config.get("post-install"))
         self._scripts_path_file = self._path.joinpath(".scripts_path")
         self._executable = None
 
     @property
     def name(self) -> str:
-        """
-        The name of the isolated environment.
-        """
+        """The name of the isolated environment."""
         return self._name
 
     @property
     def path(self) -> Path:
-        """
-        The location of the isolated environment.
-        """
+        """The location of the isolated environment."""
         return self._path
 
     @property
     def executable(self) -> Optional[Path]:
-        """
-        The location of the Python executable of the isolated environment.
-        """
+        """The location of the Python executable of the isolated environment."""
         return self._executable
 
     @property
     def scripts_path(self) -> Optional[Path]:
-        """
-        The location of the scripts directory.
-        """
+        """The location of the scripts directory."""
         if self._scripts_path_file.exists():
-            with open(self._scripts_path_file, "r") as sf:
+            with self._scripts_path_file.open() as sf:
                 return Path(sf.readline())
         return None
 
     @property
     def is_installed(self) -> bool:
         return self.scripts_path and self.scripts_path.is_dir()
 
     def install(self, quiet=False) -> None:
-        """
-        Create the virtual environment and install requirements
-        """
+        """Create the virtual environment and install requirements."""
         logger.debug("Installing IsolatedVirtualEnv in %s", self.path)
         scripts_dir = self._create_virtual_env()
         self._install_requirements(quiet)
-        with open(self._scripts_path_file, "w") as sf:
+        with self._scripts_path_file.open("w") as sf:
             sf.write(str(scripts_dir))
 
     def _create_virtual_env(self) -> Path:
         cmd = [str(self.path), "--no-setuptools", "--no-wheel", "--activators", ""]
         logger.debug("Calling virtualenv.cli_run: %s", " ".join(cmd))
         result = virtualenv.cli_run(cmd, setup_logging=False)
         scripts_dir = result.creator.script_dir
         self._executable = result.creator.exe
         return scripts_dir
 
     def _install_requirements(self, quiet=False):
         logger.info("Installing packages in isolated environment... (%s)", ", ".join(sorted(self._requirements)))
-        # pip does not honour environment markers in command line arguments
+        # pip does not honour environment markers in command line arguments,
         # but it does for requirements from a file
         with tempfile.NamedTemporaryFile("w+", prefix="build-reqs-", suffix=".txt", delete=False) as req_file:
             req_file.write(os.linesep.join(self._requirements))
         try:
             cmd = [
                 str(self._executable),
                 "-Im",
@@ -113,34 +102,32 @@
             ]
             if quiet:
                 cmd.append("--quiet")
             cmd += [
                 "--use-pep517",
                 "--no-warn-script-location",
                 "-r",
-                os.path.abspath(req_file.name),
+                Path(req_file.name).resolve(),
             ]
             subprocess.run(
                 cmd,
                 stdout=sys.stderr,
                 check=True,
             )
         finally:
-            os.remove(req_file.name)
+            Path(req_file.name).unlink()
 
     def remove(self):
-        """
-        Remove the entire virtual environment
-        """
+        """Remove the entire virtual environment."""
         logger.info("Removing isolated environment in %s", self.path)
         shutil.rmtree(self.path)
 
     def run(self, cmd: Union[str, List[str]]) -> subprocess.CompletedProcess:
-        """
-        Run a command inside the virtual environment.
+        """Run a command inside the virtual environment.
+
         :param cmd: The command string to run
         :return: The subprocess.CompletedProcess instance
         """
         logger.info("Running command in isolated venv %s: %s", self.name, cmd)
         if isinstance(cmd, List):
             extension = ".exe" if sys.platform.startswith("win") else ""
             cmd[0] = str(self.scripts_path.joinpath(cmd[0] + extension))
```

### Comparing `pyprojectx-1.0.0b3/src/pyprojectx/initializer/initializers.py` & `pyprojectx-1.0.0b4/src/pyprojectx/initializer/initializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     print(f"{BLUE}Available --init commands:{RESET}", file=sys.stderr)
     for cmd, fn in INIT_COMMANDS.items():
         print(f"{CYAN}{cmd}{RESET}", fn.__doc__, file=sys.stderr)
 
 
 def initialize_project(_):
     """Initialize pyprojectx setup in the current working directory.
+
     If pyproject.toml already exists and doesn't yet contain a tool.pyprojectx section,
     an example section will be appended.
     """
     _initialize_template("project-template.toml")
     _print_usage()
 
 
@@ -58,30 +59,32 @@
 
 def _initialize_build_tool(tool, options):
     template = f"{tool}-template.toml"
     _initialize_template(template, toml_file=template)
 
     logger.info("installing %s...", tool)
     proc = subprocess.run(
-        f"{SCRIPT_PREFIX}pw --toml {template} {tool} --version", shell=True, check=True, capture_output=True
+        f"{SCRIPT_PREFIX}pw --toml {template} {tool} --version",
+        shell=True,
+        check=True,
+        capture_output=True,
     )
     version = re.search(r"(\d+\.)+(\d+)", proc.stdout.decode("utf-8"))[0]
     old_requirement = f"{tool}>=1.1"
     new_requirement = f"{tool}=={version}"
     logger.info("setting version in %s : %s", PYPROJECT_TOML, new_requirement)
     _replace_in_file(old_requirement, new_requirement, template)
     subprocess.run(
         f"{SCRIPT_PREFIX}pw --toml {template} {tool} init " + " ".join(options.cmd_args), shell=True, check=True
     )
     logger.debug("appending template to %s...", PYPROJECT_TOML)
-    with open(template, "rt") as src:
-        with open(PYPROJECT_TOML, "at") as dest:
-            dest.write(src.read())
+    with open(template) as src, open(PYPROJECT_TOML, "a") as dest:  # noqa PTH123
+        dest.write(src.read())
     _print_usage()
-    os.remove(template)
+    os.remove(template)  # noqa PTH123
     print(
         f"\n{BLUE}You can run all {CYAN}{tool}{BLUE} commands by typing {RESET}{SCRIPT_PREFIX}pw {BLUE} in front",
         file=sys.stderr,
     )
     print(f"Example: {RESET}{SCRIPT_PREFIX}pw {tool} update", file=sys.stderr)
     print(f"{BLUE}Or use the shorter aliases like {RESET}{SCRIPT_PREFIX}pw install {BLUE}and", file=sys.stderr)
     print(
@@ -101,26 +104,26 @@
         logger.info("wrapper scripts already present")
     target_toml = Path(toml_file)
     template = Path(__file__).with_name(template_name)
     if not target_toml.exists():
         logger.info("copying %s template", template_name)
         shutil.copy2(template, target_toml)
     else:
-        with open(target_toml, "a+") as dst:
+        with target_toml.open("a+") as dst:
             toml_dict = tomli.load(dst)
             if not toml_dict.get("tool", {}).get("pyprojectx"):
-                with open(template, "rt") as src:
+                with template.open() as src:
                     logger.info("appending template to %s", toml_file)
                     dst.write(src.read())
 
 
 def _replace_in_file(old, new, file):
-    with open(file, "rt") as f:
+    with open(file) as f:  # noqa PTH123
         text = f.read().replace(old, new)
-    with open(file, "wt") as f:
+    with open(file, "w") as f:  # noqa PTH123
         f.write(text)
 
 
 def _print_usage():
     print(f"{BLUE}Pyprojectx scripts are installed in the current directory.", file=sys.stderr)
     print("You can add pw and pw.bat under version control if applicable.", file=sys.stderr)
     if sys.platform.startswith("win"):
@@ -130,20 +133,21 @@
         f" to see the available tools and aliases in your project.{RESET}",
         file=sys.stderr,
     )
 
 
 def initialize_global(options):
     """Initialize the global pyprojectx setup in your home directory.
+
     Use '--init global --force' to overwrite.
     """
     global_dir = HOME_DIR.joinpath(DEFAULT_INSTALL_DIR, "global")
     wrapper_dir = Path(__file__).parent.parent.joinpath("wrapper")
     logger.debug("creating global directory %s", global_dir)
-    os.makedirs(global_dir, exist_ok=True)
+    global_dir.mkdir(parents=True, exist_ok=True)
 
     target_pw = global_dir.joinpath("pw")
     if target_pw.exists() and "--force" not in options.cmd_args:
         print(f"{target_pw} {BLUE} already exists, use '--init global --force' to overwrite{RESET}", file=sys.stderr)
         return
 
     shutil.copy2(wrapper_dir.joinpath("pw.py"), target_pw)
@@ -164,26 +168,25 @@
         f"Run {RESET}pxg --info -{BLUE} to see the available tools and aliases in the global pyprojectx.{RESET}",
         file=sys.stderr,
     )
 
 
 def ensure_path(location: Path):
     global_path = str(location.parent.absolute())
-    # pylint: disable=broad-except
     try:
         if userpath.in_current_path(global_path):
             print(f"{global_path} is already in PATH.", file=sys.stderr)
         else:
             userpath.append(global_path, "pyprojectx")
             print(f"{global_path} has been been added to PATH", file=sys.stderr)
         if userpath.need_shell_restart(global_path):
             print(
                 " but you need to open a new terminal or re-login for this PATH change to take effect.", file=sys.stderr
             )
-    except Exception:
+    except Exception:  # noqa BLE001
         print(
             f"{global_path} {RED} could not be added automatically to PATH. You will need to add it manually{RESET}",
             file=sys.stderr,
         )
 
 
 INIT_COMMANDS = {
```

### Comparing `pyprojectx-1.0.0b3/src/pyprojectx/initializer/pdm-template.toml` & `pyprojectx-1.0.0b4/src/pyprojectx/initializer/pdm-template.toml`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b3/src/pyprojectx/initializer/poetry-template.toml` & `pyprojectx-1.0.0b4/src/pyprojectx/initializer/poetry-template.toml`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b3/src/pyprojectx/initializer/project-template.toml` & `pyprojectx-1.0.0b4/src/pyprojectx/initializer/project-template.toml`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b3/src/pyprojectx/wrapper/pw.py` & `pyprojectx-1.0.0b4/src/pyprojectx/wrapper/pw.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import argparse
 import os
 import subprocess
 import sys
 from pathlib import Path
 from venv import EnvBuilder
 
-VERSION = "1.0.0b3"
+VERSION = "1.0.0b4"
 
 PYPROJECTX_INSTALL_DIR_ENV_VAR = "PYPROJECTX_INSTALL_DIR"
 PYPROJECTX_PACKAGE_ENV_VAR = "PYPROJECTX_PACKAGE"
 PYPROJECT_TOML = "pyproject.toml"
 DEFAULT_INSTALL_DIR = ".pyprojectx"
 
 CYAN = "\033[96m"
@@ -111,14 +111,19 @@
     parser.add_argument(
         "--init",
         action="store_true",
         help="Create or prepare a pyproject.toml and pyprojectx wrapper scripts. "
         "Run with '--init help' to show available init options",
     )
     parser.add_argument(
+        "--upgrade",
+        action="store_true",
+        help="Download the latest pyprojectx wrapper scripts.",
+    )
+    parser.add_argument(
         "command", nargs=argparse.REMAINDER, help="The command/alias with optional arguments to execute."
     )
     return parser
 
 
 def ensure_pyprojectx(options):
     env_builder = EnvBuilder(with_pip=True)
@@ -137,23 +142,23 @@
         out = sys.stderr
 
     if not pyprojectx_script.is_file() and not pyprojectx_exe.is_file():
         if not options.quiet:
             print(f"{CYAN}creating pyprojectx venv in {BLUE}{venv_dir}{RESET}", file=sys.stderr)
         env_builder.create(venv_dir)
         subprocess.run(
-            pip_cmd + ["--upgrade", "pip"],
+            [*pip_cmd, "--upgrade", "pip"],
             stdout=out,
             check=True,
         )
 
         if not options.quiet:
             print(
                 f"{CYAN}installing pyprojectx {BLUE}{options.version}: {options.pyprojectx_package} {RESET}",
                 file=sys.stderr,
             )
-        subprocess.run(pip_cmd + [options.pyprojectx_package], stdout=out, check=True)
+        subprocess.run([*pip_cmd, options.pyprojectx_package], stdout=out, check=True)
     return pyprojectx_script
 
 
 if __name__ == "__main__":
     run(sys.argv[1:])
```

### Comparing `pyprojectx-1.0.0b3/tests/conftest.py` & `pyprojectx-1.0.0b4/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 from pathlib import Path
 
 import pytest
 
 from pyprojectx.wrapper import pw
 
 
-@pytest.fixture
+@pytest.fixture()
 def tmp_dir():
     path = tempfile.mkdtemp(prefix="build-env-")
     yield Path(path)
     shutil.rmtree(path)
 
 
 @pytest.fixture(scope="session")
 def tmp_project():
     tmp = Path(tempfile.mkdtemp(prefix="build-env-"))
     toml = Path(__file__).with_name("data").joinpath("pw-test.toml")
     shutil.copyfile(toml, tmp.joinpath(pw.PYPROJECT_TOML))
     pw_copy = Path(tmp, "pw")
     project_dir = Path(__file__).parent.parent
     shutil.copyfile(project_dir.joinpath("src/pyprojectx/wrapper/pw.py"), pw_copy)
-    os.chmod(pw_copy, stat.S_IRWXU | stat.S_IRWXG)
+    pw_copy.chmod(stat.S_IRWXU | stat.S_IRWXG)
     shutil.copy(project_dir.joinpath("src/pyprojectx/wrapper/pw.bat"), tmp)
     env = os.environ.copy()
     env["PYPROJECTX_PACKAGE"] = str(project_dir.absolute())
     yield tmp, env
     shutil.rmtree(tmp)
```

### Comparing `pyprojectx-1.0.0b3/tests/data/pw-test.toml` & `pyprojectx-1.0.0b4/tests/data/pw-test.toml`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b3/tests/data/test.toml` & `pyprojectx-1.0.0b4/tests/data/test.toml`

 * *Files identical despite different names*

### Comparing `pyprojectx-1.0.0b3/tests/integration/test_pw.py` & `pyprojectx-1.0.0b4/tests/integration/test_pw.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 import sys
 from pathlib import Path
 
 import pytest
 
 from pyprojectx.initializer.initializers import SCRIPT_PREFIX
 
-# pylint: disable=redefined-outer-name
-
 
 def test_logs_and_stdout_with_quiet(tmp_project):
     project_dir, env = tmp_project
     cmd = f"{SCRIPT_PREFIX}pw -q pycowsay Hello px!"
     assert Path(project_dir, f"{SCRIPT_PREFIX}pw").is_file()
     proc_result = subprocess.run(cmd, shell=True, capture_output=True, cwd=project_dir, env=env, check=True)
 
@@ -30,25 +28,25 @@
            ||     ||
 
 """.replace(
             "\n", os.linesep
         )
     )
     if not sys.platform.startswith("win"):
-        assert proc_result.stderr.decode("utf-8") == ""
+        assert not proc_result.stderr.decode("utf-8")
 
     cmd = f"{SCRIPT_PREFIX}pw -q list-files *.toml"
     proc_result = subprocess.run(cmd, shell=True, capture_output=True, cwd=project_dir, env=env, check=True)
     assert proc_result.stdout.decode("utf-8").strip() == "pyproject.toml"
 
 
 def test_logs_and_stdout_when_alias_invoked_from_sub_directory_with_verbose(tmp_project):
     project_dir, env = tmp_project
     cwd = project_dir.joinpath("subdir")
-    os.makedirs(cwd, exist_ok=True)
+    cwd.mkdir(parents=True, exist_ok=True)
     cmd = f"..{os.sep}pw --verbose --verbose combine-pw-scripts"
     proc_result = subprocess.run(cmd, shell=True, capture_output=True, cwd=cwd, env=env, check=True)
 
     assert "< hi >" in proc_result.stdout.decode("utf-8")
     assert "< hello >" in proc_result.stdout.decode("utf-8")
     assert "INFO:pyprojectx.log:Running command in isolated venv pycowsay: pycowsay hi" in proc_result.stderr.decode(
         "utf-8"
@@ -61,27 +59,27 @@
 
 def test_alias_abbreviations(tmp_project):
     project_dir, env = tmp_project
     cmd = f"{SCRIPT_PREFIX}pw -q pHe"
     proc_result = subprocess.run(cmd, shell=True, capture_output=True, cwd=project_dir, env=env, check=True)
     assert "< hello >" in proc_result.stdout.decode("utf-8")
     if not sys.platform.startswith("win"):
-        assert proc_result.stderr.decode("utf-8") == ""
+        assert not proc_result.stderr.decode("utf-8")
 
     cmd = f"{SCRIPT_PREFIX}pw -q pycow"
     proc_result = subprocess.run(cmd, shell=True, capture_output=True, cwd=project_dir, env=env, check=False)
     assert proc_result.returncode
     assert "'pycow' is ambiguous" in proc_result.stderr.decode("utf-8")
     assert "pycowsay, pycowsay-hi, pycowsay-hello" in proc_result.stderr.decode("utf-8")
     if not sys.platform.startswith("win"):
-        assert proc_result.stdout.decode("utf-8") == ""
+        assert not proc_result.stdout.decode("utf-8")
 
 
 @pytest.mark.parametrize(
-    "cmd, stderr",
+    ("cmd", "stderr"),
     [
         (
             f"{SCRIPT_PREFIX}pw -q failing-install",
             "PYPROJECTX ERROR: installation of 'failing-install' failed with exit code",
         ),
         (f"{SCRIPT_PREFIX}pw -q failing-shell", "go-foo-bar"),
         (f"{SCRIPT_PREFIX}pw -q foo-bar", "foo-bar.+is not configured as tool or alias in.+pyproject.toml"),
@@ -91,15 +89,15 @@
         ),
     ],
 )
 def test_output_with_errors(cmd, stderr, tmp_project):
     project_dir, env = tmp_project
     proc_result = subprocess.run(cmd, shell=True, capture_output=True, cwd=project_dir, env=env, check=False)
     assert proc_result.returncode
-    assert proc_result.stdout.decode("utf-8") == ""
+    assert not proc_result.stdout.decode("utf-8")
     assert re.search(stderr, proc_result.stderr.decode("utf-8"))
 
 
 def test_post_install(tmp_project):
     project_dir, env = tmp_project
     cmd = f"{SCRIPT_PREFIX}pw -q say-post-install"
     assert Path(project_dir, f"{SCRIPT_PREFIX}pw").is_file()
@@ -128,15 +126,15 @@
            ||     ||
 
 """.replace(
             "\n", os.linesep
         )
     )
     if not sys.platform.startswith("win"):
-        assert proc_result.stderr.decode("utf-8") == ""
+        assert not proc_result.stderr.decode("utf-8")
 
     cmd = f"{SCRIPT_PREFIX}pw -q list-files *.txt"
     proc_result = subprocess.run(cmd, shell=True, capture_output=True, cwd=project_dir, env=env, check=True)
     assert proc_result.stdout.decode("utf-8").strip() == "post-install-file.txt"
 
 
 def test_alias_with_quoted_args(tmp_project):
```

### Comparing `pyprojectx-1.0.0b3/tests/integration/test_px.py` & `pyprojectx-1.0.0b4/tests/integration/test_px.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 import subprocess
 import sys
 from pathlib import Path
 
 import pytest
 
 from pyprojectx.initializer.initializers import SCRIPT_EXTENSION, SCRIPT_PREFIX
-
-# pylint: disable=redefined-outer-name
 from pyprojectx.wrapper.pw import PYPROJECT_TOML
 
 
 def test_px_invoked_from_sub_directory(tmp_project):
     project_dir, env = tmp_project
     cwd = project_dir.joinpath("subdir")
     copy_px(cwd)
@@ -73,15 +71,15 @@
     subprocess.run(
         f"{SCRIPT_PREFIX}px run python --version", shell=True, capture_output=True, cwd=cwd, env=env, check=True
     )
     proc_result = subprocess.run(
         f"{SCRIPT_PREFIX}px {tool} --version", shell=True, capture_output=True, cwd=cwd, env=env, check=False
     )
     version = re.search(r"(\d+\.)+(\d+)", proc_result.stdout.decode("utf-8"))[0]
-    with open(cwd.joinpath(PYPROJECT_TOML), "rt") as f:
+    with cwd.joinpath(PYPROJECT_TOML).open() as f:
         assert f'{tool} = "{tool}=={version}"' in f.read()
 
 
 def test_initialize_global(tmp_project):
     project_dir, env = tmp_project
     cwd = project_dir.joinpath("global")
     copy_px(cwd)
@@ -93,9 +91,9 @@
     assert px_dir.joinpath("global", PYPROJECT_TOML).exists()
     assert px_dir.joinpath("global", "pw").exists()
     assert px_dir.joinpath(f"px{SCRIPT_EXTENSION}").exists()
     assert px_dir.joinpath(f"pxg{SCRIPT_EXTENSION}").exists()
 
 
 def copy_px(dir_name):
-    os.makedirs(dir_name, exist_ok=True)
+    dir_name.mkdir(parents=True, exist_ok=True)
     shutil.copy(Path(__file__).parent.parent.joinpath(f"../src/pyprojectx/wrapper/px{SCRIPT_EXTENSION}"), dir_name)
```

### Comparing `pyprojectx-1.0.0b3/tests/unit/test_cli.py` & `pyprojectx-1.0.0b4/tests/unit/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
+# ruff: noqa: PLR2004
 import os.path
 import sys
 from pathlib import Path
 from unittest.mock import ANY
 
 import pytest
 
 from pyprojectx.cli import _get_options, _run
 from pyprojectx.wrapper import pw
 
-# pylint: disable=protected-access, no-member
-
 PY_VER = f"py{sys.version_info.major}.{sys.version_info.minor}"
 SCRIPTS_DIR = "Scripts" if sys.platform.startswith("win") else "bin"
 EXTENSION = ".exe" if sys.platform == "win32" else ""
 
 
 def test_parse_args():
     assert _get_options(["--toml", "an-option", "my-cmd"]).toml_path == Path("an-option")
@@ -33,29 +32,31 @@
 
     assert _get_options(["--init", "global"]).init
     assert _get_options(["-i", "all"]).info
 
     assert _get_options(["my-cmd", "--in"]).cmd == "my-cmd"
     assert not _get_options(["my-cmd", "--init"]).init
 
+    assert _get_options(["--upgrade"]).upgrade
+
 
 def test_run_tool(tmp_dir, mocker):
     toml = Path(__file__).parent.with_name("data").joinpath("test.toml")
     run_mock = mocker.patch("subprocess.run")
 
     _run(["path/to/pyprojectx", "--install-dir", str(tmp_dir), "-t", str(toml), "tool-1"])
 
     pip_install_args = _get_call_args(run_mock.mock_calls[0])
     first_arg = str(pip_install_args[0])
     assert (
         f"{tmp_dir.name}{os.sep}venvs{os.sep}"
         f"tool-1-db298015454af73633c6be4b86b3f2e8-{PY_VER}{os.sep}{SCRIPTS_DIR}{os.sep}python" in first_arg
     )
     assert pip_install_args[1:-1] == ["-Im", "pip", "install", "--use-pep517", "--no-warn-script-location", "-r"]
-    assert "build-reqs-" in pip_install_args[-1]
+    assert "build-reqs-" in str(pip_install_args[-1])
 
     run_args = _get_call_args(run_mock.mock_calls[1])
     run_kwargs = _get_call_kwargs(run_mock.mock_calls[1])
     assert len(run_args) == 1
     assert run_args[0].endswith(
         f"{tmp_dir.name}{os.sep}venvs{os.sep}"
         f"tool-1-db298015454af73633c6be4b86b3f2e8-{PY_VER}{os.sep}{SCRIPTS_DIR}{os.sep}tool-1{EXTENSION}"
```

### Comparing `pyprojectx-1.0.0b3/tests/unit/test_config.py` & `pyprojectx-1.0.0b4/tests/unit/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 def test_unexisting_toml():
     with pytest.raises(Warning, match=r"No such file or directory"):
         Config(Path(__file__).parent.with_name("data").joinpath("unexisting.toml"))
 
 
 @pytest.mark.parametrize(
-    "shorcut, aliases",
+    ("shorcut", "aliases"),
     [
         ("aaa-bbb-ccc", ["aaa-bbb-ccc"]),
         ("aaaBbbDdd", ["aaaBbbDdd"]),
         ("b123-c123-d123", ["b123-c123-d123"]),
         ("c123D123", ["c123D123"]),
         ("d123-E123", ["d123-E123"]),
         ("aBC", ["aaa-bbb-ccc"]),
```

### Comparing `pyprojectx-1.0.0b3/tests/unit/test_env.py` & `pyprojectx-1.0.0b4/tests/unit/test_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
+# ruff: noqa: PLR2004
 import os
 import subprocess
 import sys
 
 import pytest
 from packaging.version import Version
 
 from pyprojectx.env import IsolatedVirtualEnv
 from pyprojectx.log import set_verbosity
 
-# pylint: disable=no-member
-
 
 def test_isolated_env_path(tmp_dir):
     env = IsolatedVirtualEnv(
         tmp_dir,
         "env-name",
         {
             "requirements": [
@@ -46,17 +45,17 @@
     assert not env.path.exists()
 
 
 def test_isolation(tmp_dir):
     subprocess.check_call([sys.executable, "-c", "import pyprojectx.env"])
     env = IsolatedVirtualEnv(tmp_dir, "env-name", {})
     env.install()
+    debug_import = "import sys; import os; print(os.linesep.join(sys.path));"
     with pytest.raises(subprocess.CalledProcessError):
-        debug = "import sys; import os; print(os.linesep.join(sys.path));"
-        subprocess.check_call([str(env.executable), "-c", f"{debug} import pyprojectx.env"])
+        subprocess.check_call([str(env.executable), "-c", f"{debug_import} import pyprojectx.env"])
 
 
 def test_isolated_env_install_arguments(mocker, tmp_dir):
     run_mock = mocker.patch("subprocess.run")
     env = IsolatedVirtualEnv(
         tmp_dir,
         "env-name",
```

### Comparing `pyprojectx-1.0.0b3/PKG-INFO` & `pyprojectx-1.0.0b4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: pyprojectx
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: Execute scripts from pyproject.toml, installing tools on-the-fly
 Keywords: build dependency pyprojectx
 Home-page: https://github.com/pyprojectx/pyprojectx
 Author-Email: Houbie <ivo@houbrechts-it.be>
 License: MIT
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: Homepage, https://github.com/pyprojectx/pyprojectx
 Project-URL: Documentation, https://pyprojectx.github.io
 Requires-Python: >=3.7
-Requires-Dist: tomli>=2.0.1
-Requires-Dist: virtualenv>=20.21.0
-Requires-Dist: userpath>=1.8.0
+Requires-Dist: click==8.1.3
+Requires-Dist: distlib==0.3.6
+Requires-Dist: filelock==3.11.0
+Requires-Dist: platformdirs==3.2.0
+Requires-Dist: tomli==2.0.1
+Requires-Dist: userpath==1.8.0
+Requires-Dist: virtualenv==20.23.0
 Description-Content-Type: text/markdown
 
 ![pyprojectx](docs/docs/assets/px.png)
 
 # Pyprojectx: All-inclusive Python Projects
 
 Execute scripts from pyproject.toml, installing tools on-the-fly
```

