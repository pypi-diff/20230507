# Comparing `tmp/vmn-0.8.2rc1-py3-none-any.whl.zip` & `tmp/vmn-0.8.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 45389 bytes, number of entries: 10
+Zip file size: 45054 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      152 b- defN 21-Jul-06 16:25 version_stamp/__init__.py
--rw-r--r--  2.0 unx    53098 b- defN 23-Apr-16 14:06 version_stamp/stamp_utils.py
--rw-r--r--  2.0 unx       58 b- defN 23-May-04 07:59 version_stamp/version.py
--rw-r--r--  2.0 unx   112040 b- defN 23-May-04 07:40 version_stamp/vmn.py
--rw-r--r--  2.0 unx    35127 b- defN 23-May-04 07:59 vmn-0.8.2rc1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      470 b- defN 23-May-04 07:59 vmn-0.8.2rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-04 07:59 vmn-0.8.2rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-May-04 07:59 vmn-0.8.2rc1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-May-04 07:59 vmn-0.8.2rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      804 b- defN 23-May-04 07:59 vmn-0.8.2rc1.dist-info/RECORD
-10 files, 201902 bytes uncompressed, 44019 bytes compressed:  78.2%
+-rw-r--r--  2.0 unx    53161 b- defN 23-May-07 17:24 version_stamp/stamp_utils.py
+-rw-r--r--  2.0 unx       50 b- defN 23-May-07 17:32 version_stamp/version.py
+-rw-r--r--  2.0 unx   109842 b- defN 23-May-07 16:56 version_stamp/vmn.py
+-rw-r--r--  2.0 unx    35127 b- defN 23-May-07 17:32 vmn-0.8.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      467 b- defN 23-May-07 17:32 vmn-0.8.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-07 17:32 vmn-0.8.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-May-07 17:32 vmn-0.8.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-May-07 17:32 vmn-0.8.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      786 b- defN 23-May-07 17:32 vmn-0.8.4.dist-info/RECORD
+10 files, 199738 bytes uncompressed, 43720 bytes compressed:  78.1%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: version_stamp/version.py
 Comment: 
 
 Filename: version_stamp/vmn.py
 Comment: 
 
-Filename: vmn-0.8.2rc1.dist-info/LICENSE.txt
+Filename: vmn-0.8.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: vmn-0.8.2rc1.dist-info/METADATA
+Filename: vmn-0.8.4.dist-info/METADATA
 Comment: 
 
-Filename: vmn-0.8.2rc1.dist-info/WHEEL
+Filename: vmn-0.8.4.dist-info/WHEEL
 Comment: 
 
-Filename: vmn-0.8.2rc1.dist-info/entry_points.txt
+Filename: vmn-0.8.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: vmn-0.8.2rc1.dist-info/top_level.txt
+Filename: vmn-0.8.4.dist-info/top_level.txt
 Comment: 
 
-Filename: vmn-0.8.2rc1.dist-info/RECORD
+Filename: vmn-0.8.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## version_stamp/stamp_utils.py

```diff
@@ -176,27 +176,25 @@
         cwd = os.environ["VMN_WORKING_DIR"]
 
     root_path = os.path.realpath(os.path.expanduser(cwd))
     """
             ".git" is the default app's backend in this case. If other backends will be added, 
             then it can be moved to the configuration file as a default_backend or similar. 
         """
-    exist = os.path.exists(os.path.join(root_path, ".vmn")) or os.path.exists(
-        os.path.join(root_path, ".git")
-    )
+    exist = os.path.exists(os.path.join(root_path, ".git"))
+    exist = exist or os.path.exists(os.path.join(root_path, ".vmn"))
     while not exist:
         try:
             prev_path = root_path
             root_path = os.path.realpath(os.path.join(root_path, ".."))
             if prev_path == root_path:
                 raise RuntimeError()
 
-            exist = os.path.exists(os.path.join(root_path, ".vmn")) or os.path.exists(
-                os.path.join(root_path, ".git")
-            )
+            exist = os.path.exists(os.path.join(root_path, ".git"))
+            exist = exist or os.path.exists(os.path.join(root_path, ".vmn"))
         except Exception as exc:
             VMN_LOGGER.debug(f"Logged exception: ", exc_info=True)
             root_path = None
             break
     if root_path is None:
         raise RuntimeError("Running from an unmanaged directory")
 
@@ -211,15 +209,15 @@
 
     def filter(self, record):
         if self._low <= record.levelno <= self._high:
             return True
         return False
 
 
-def init_stamp_logger(rotating_log_path=None, debug=False):
+def init_stamp_logger(rotating_log_path=None, debug=False, supress_stdout=False):
     global VMN_LOGGER
 
     VMN_LOGGER = logging.getLogger(VMN_USER_NAME)
     clear_logger_handlers(VMN_LOGGER)
     glob_logger = logging.getLogger()
     clear_logger_handlers(glob_logger)
 
@@ -233,15 +231,17 @@
     stdout_handler.setFormatter(formatter)
 
     min_stdout_level = logging.INFO
     if debug:
         min_stdout_level = logging.DEBUG
 
     stdout_handler.addFilter(LevelFilter(min_stdout_level, logging.INFO))
-    VMN_LOGGER.addHandler(stdout_handler)
+
+    if not supress_stdout or debug:
+        VMN_LOGGER.addHandler(stdout_handler)
 
     stderr_handler = logging.StreamHandler(sys.stderr)
     stderr_handler.setFormatter(formatter)
     stderr_handler.setLevel(logging.WARNING)
     VMN_LOGGER.addHandler(stderr_handler)
 
     if rotating_log_path is None:
```

## version_stamp/version.py

```diff
@@ -1,3 +1,3 @@
 name = "vmn"
-version = "0.8.2-rc1"
-_version = "0.8.2-rc1"
+version = "0.8.4"
+_version = "0.8.4"
```

## version_stamp/vmn.py

```diff
@@ -397,15 +397,15 @@
             del self.backend
             self.backend = None
 
     # Note: this function generates a version (including prerelease)
     def gen_advanced_version(
         self, initial_version, initialprerelease, initialprerelease_count
     ):
-        verstr = self.advance_version(initial_version, self.release_mode)
+        verstr = self._advance_version(initial_version)
 
         prerelease = self.prerelease
         # If user did not specify a change in prerelease,
         # stay with the previous one
         if prerelease is None and self.release_mode is None:
             prerelease = initialprerelease
         prerelease_count = copy.deepcopy(initialprerelease_count)
@@ -454,72 +454,72 @@
         prerelease_count[counter_key] += 1
 
         if self.release_mode is not None:
             prerelease_count = {counter_key: 1}
 
         return counter_key, prerelease_count
 
-    def increase_octet(self, tag_name_prefix: str, version_number_oct: str, release_mode: str, globally: bool) -> str:
+    def increase_octet(self, tag_name_prefix: str, version_number_oct: str) -> str:
         tag = self.backend.get_latest_available_tag(tag_name_prefix)
         version_number_oct = int(version_number_oct)
-        if tag and globally:
+        if tag:
             props = stamp_utils.VMNBackend.deserialize_vmn_tag_name(tag)
-            version_number_oct = max(version_number_oct, int(props[release_mode]))
+            version_number_oct = max(version_number_oct, int(props[self.release_mode]))
         version_number_oct += 1
         return str(version_number_oct)
 
-    def advance_version(self, version, release_mode, globally=True):
+    def _advance_version(self, version):
         # TODO: maybe move up the version validity test
         match = re.search(stamp_utils.VMN_REGEX, version)
         gdict = match.groupdict()
         if gdict["hotfix"] is None:
             gdict["hotfix"] = "0"
 
         major = gdict["major"]
         minor = gdict["minor"]
         patch = gdict["patch"]
         hotfix = gdict["hotfix"]
 
-        if release_mode == "major":
+        if self.release_mode == "major":
             tag_name_prefix = stamp_utils.VMNBackend.app_name_to_git_tag_app_name(
                 self.name
             )
 
             tag_name_prefix = f"{tag_name_prefix}_*"
-            major = self.increase_octet(tag_name_prefix, major, release_mode, globally)
+            major = self.increase_octet(tag_name_prefix, major)
 
             minor = "0"
             patch = "0"
             hotfix = "0"
-        elif release_mode == "minor":
+        elif self.release_mode == "minor":
             tag_name_prefix = stamp_utils.VMNBackend.app_name_to_git_tag_app_name(
                 self.name
             )
 
             tag_name_prefix = f"{tag_name_prefix}_{major}*"
-            minor = self.increase_octet(tag_name_prefix, minor, release_mode, globally)
+            minor = self.increase_octet(tag_name_prefix, minor)
 
             patch = "0"
             hotfix = "0"
-        elif release_mode == "patch":
+        elif self.release_mode == "patch":
             tag_name_prefix = stamp_utils.VMNBackend.app_name_to_git_tag_app_name(
                 self.name
             )
 
             tag_name_prefix = f"{tag_name_prefix}_{major}.{minor}*"
-            patch = self.increase_octet(tag_name_prefix, patch, release_mode, globally)
+            patch = self.increase_octet(tag_name_prefix, patch)
 
             hotfix = "0"
-        elif release_mode == "hotfix":
+        elif self.release_mode == "hotfix":
             tag_name_prefix = stamp_utils.VMNBackend.app_name_to_git_tag_app_name(
                 self.name
             )
 
             tag_name_prefix = f"{tag_name_prefix}_{major}.{minor}.{patch}*"
-            hotfix = self.increase_octet(tag_name_prefix, hotfix, release_mode, globally)
+            hotfix = self.increase_octet(tag_name_prefix, hotfix)
 
         return stamp_utils.VMNBackend.serialize_vmn_version_hotfix(
             self.hide_zero_hotfix,
             major,
             minor,
             patch,
             hotfix,
@@ -1432,24 +1432,32 @@
 
 
 @stamp_utils.measure_runtime_decorator
 def handle_stamp(vmn_ctx):
     vmn_ctx.vcs.prerelease = vmn_ctx.args.pr
     vmn_ctx.vcs.buildmetadata = None
     vmn_ctx.vcs.release_mode = vmn_ctx.args.release_mode
-    vmn_ctx.vcs.optional_release_mode = vmn_ctx.args.orm
     vmn_ctx.vcs.override_root_version = vmn_ctx.args.orv
     vmn_ctx.vcs.override_version = vmn_ctx.args.ov
     vmn_ctx.vcs.dry_run = vmn_ctx.args.dry
 
     # For backward compatibility
     if vmn_ctx.vcs.release_mode == "micro":
         vmn_ctx.vcs.release_mode = "hotfix"
 
-    assert vmn_ctx.vcs.release_mode is None or vmn_ctx.vcs.optional_release_mode is None
+    if vmn_ctx.vcs.tracked and vmn_ctx.vcs.release_mode is None:
+        vmn_ctx.vcs.current_version_info["stamping"]["app"][
+            "release_mode"
+        ] = vmn_ctx.vcs.ver_infos_from_repo[vmn_ctx.vcs.selected_tag]["ver_info"][
+            "stamping"
+        ][
+            "app"
+        ][
+            "release_mode"
+        ]
 
     optional_status = {"modified", "detached"}
     expected_status = {
         "repos_exist_locally",
         "repo_tracked",
         "app_tracked",
         "deps_synced_with_conf",
@@ -1500,57 +1508,14 @@
     ) = VersionControlStamper.get_version_number_from_file(
         vmn_ctx.vcs.version_file_path
     )
 
     if vmn_ctx.vcs.override_version:
         initial_version = vmn_ctx.vcs.override_version
 
-    is_release = vmn_ctx.vcs.ver_infos_from_repo[vmn_ctx.vcs.selected_tag]["ver_info"]["stamping"]["app"][
-                     "prerelease"] == "release"
-    if vmn_ctx.vcs.optional_release_mode and is_release:
-        verstr = vmn_ctx.vcs.advance_version(initial_version, vmn_ctx.vcs.optional_release_mode, globally=False)
-        tag_name_prefix = f'{vmn_ctx.vcs.name.replace("/", "-")}_{verstr}*'
-        tag = vmn_ctx.vcs.backend.get_latest_available_tag(tag_name_prefix)
-        if tag is not None and len(tag) < len(tag_name_prefix):
-            tag = None
-
-        if not tag:
-            vmn_ctx.vcs.release_mode = vmn_ctx.vcs.optional_release_mode
-        else:
-            props = stamp_utils.VMNBackend.deserialize_vmn_tag_name(tag)
-
-            (_, temp_ver_infos_from_repo) = vmn_ctx.vcs.get_version_info_from_verstr(
-                f"{props['version']}-{props['prerelease']}")
-
-            vmn_ctx.vcs.ver_infos_from_repo[vmn_ctx.vcs.selected_tag]["ver_info"]["stamping"]["app"]["_version"] = \
-                temp_ver_infos_from_repo[tag]["ver_info"]["stamping"]["app"]["_version"]
-            vmn_ctx.vcs.ver_infos_from_repo[vmn_ctx.vcs.selected_tag]["ver_info"]["stamping"]["app"]["prerelease"] = \
-                temp_ver_infos_from_repo[tag]["ver_info"]["stamping"]["app"]["prerelease"]
-            vmn_ctx.vcs.ver_infos_from_repo[vmn_ctx.vcs.selected_tag]["ver_info"]["stamping"]["app"][
-                "prerelease_count"] = \
-                temp_ver_infos_from_repo[tag]["ver_info"]["stamping"]["app"]["prerelease_count"]
-            vmn_ctx.vcs.ver_infos_from_repo[vmn_ctx.vcs.selected_tag]["ver_info"]["stamping"]["app"]["release_mode"] = \
-                temp_ver_infos_from_repo[tag]["ver_info"]["stamping"]["app"]["release_mode"]
-
-            initial_version = verstr
-            if prerelease == "release":
-                prerelease = temp_ver_infos_from_repo[tag]["ver_info"]["stamping"]["app"]["prerelease"]
-                prerelease_count = temp_ver_infos_from_repo[tag]["ver_info"]["stamping"]["app"]["prerelease_count"]
-
-    if vmn_ctx.vcs.tracked and vmn_ctx.vcs.release_mode is None:
-        vmn_ctx.vcs.current_version_info["stamping"]["app"][
-            "release_mode"
-        ] = vmn_ctx.vcs.ver_infos_from_repo[vmn_ctx.vcs.selected_tag]["ver_info"][
-            "stamping"
-        ][
-            "app"
-        ][
-            "release_mode"
-        ]
-
     try:
         version = _stamp_version(
             vmn_ctx.vcs,
             vmn_ctx.args.pull,
             vmn_ctx.args.check_vmn_version,
             initial_version,
             prerelease,
@@ -1702,14 +1667,17 @@
         return 1
 
     return 0
 
 
 @stamp_utils.measure_runtime_decorator
 def handle_show(vmn_ctx):
+    if version_mod.version == "0.0.0":
+        stamp_utils.VMN_LOGGER.info("Test logprint in show")
+
     vmn_ctx.params["from_file"] = vmn_ctx.args.from_file
 
     # root app does not have raw version number
     if vmn_ctx.vcs.root_context:
         vmn_ctx.params["raw"] = False
     else:
         vmn_ctx.params["raw"] = vmn_ctx.args.raw
@@ -2215,15 +2183,15 @@
 
     if tag_name not in ver_infos:
         ver_info = None
     else:
         ver_info = ver_infos[tag_name]["ver_info"]
 
     if ver_info is None:
-        stamp_utils.VMN_LOGGER.info(
+        stamp_utils.VMN_LOGGER.error(
             "Version information was not found " "for {0}.".format(vcs.name)
         )
 
         raise RuntimeError()
 
     data = {}
 
@@ -2814,15 +2782,18 @@
         stamp_utils.init_stamp_logger()
         args = parse_user_commands(command_line)
     except Exception as exc:
         stamp_utils.VMN_LOGGER.debug("Logged exception: ", exc_info=True)
         return 1, None
 
     try:
-        stamp_utils.init_stamp_logger(debug=args.debug)
+        if args.command == "show":
+            stamp_utils.init_stamp_logger(debug=args.debug, supress_stdout=True)
+        else:
+            stamp_utils.init_stamp_logger(debug=args.debug)
 
         root_path = stamp_utils.resolve_root_path()
         vmn_path = os.path.join(root_path, ".vmn")
         pathlib.Path(vmn_path).mkdir(parents=True, exist_ok=True)
 
     except Exception as exc:
         stamp_utils.VMN_LOGGER.error(
@@ -2841,15 +2812,19 @@
             lock_file_path = os.environ[LOCK_FILE_ENV]
 
         lock = FileLock(lock_file_path)
 
         # start of non-parallel code section
         lock.acquire()
 
-        stamp_utils.init_stamp_logger(os.path.join(vmn_path, LOG_FILENAME), args.debug)
+        if args.command == "show":
+            stamp_utils.init_stamp_logger(os.path.join(vmn_path, LOG_FILENAME), args.debug, supress_stdout=True)
+        else:
+            stamp_utils.init_stamp_logger(os.path.join(vmn_path, LOG_FILENAME), args.debug)
+
         command_line = copy.deepcopy(command_line)
 
         if command_line is None or not command_line:
             command_line = sys.argv
             if command_line is None:
                 command_line = ["vmn"]
 
@@ -3026,22 +3001,14 @@
         "--release-mode",
         choices=["major", "minor", "patch", "hotfix", "micro"],
         default=None,
         help="major / minor / patch / hotfix",
         metavar="",
     )
     pstamp.add_argument(
-        "--orm",
-        "--optional-release-mode",
-        choices=["major", "minor", "patch", "hotfix"],
-        default=None,
-        help="major / minor / patch / hotfix",
-        metavar="",
-    )
-    pstamp.add_argument(
         "--pr",
         "--prerelease",
         default=None,
         help="Prerelease version. Can be anything really until you decide "
         "to release the version",
     )
     pstamp.add_argument("--pull", dest="pull", action="store_true")
```

## Comparing `vmn-0.8.2rc1.dist-info/LICENSE.txt` & `vmn-0.8.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `vmn-0.8.2rc1.dist-info/RECORD` & `vmn-0.8.4.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 version_stamp/__init__.py,sha256=p_9bnBNpi1jHdKDsmBM7tN2Da3N-QOYEe8s09k9NIrk,152
-version_stamp/stamp_utils.py,sha256=aQupNHxBbWzjJjyFvIze6utVhFgqzD5w_Gb5RjPtMRM,53098
-version_stamp/version.py,sha256=TG3tt9N6VaM-wPtzpPkyKx8LJqqSP95NRnL04M1dtTE,58
-version_stamp/vmn.py,sha256=FjVwGdRjHO80RaBbB-cFiPhl5xty7hE2VlrME5l3Xio,112040
-vmn-0.8.2rc1.dist-info/LICENSE.txt,sha256=f6flbA23EQX0tZpqCsQCJesFmHb4XNOAOD99egZuaL4,35127
-vmn-0.8.2rc1.dist-info/METADATA,sha256=aiBelMVfrsfATQK0phyOxqNVqXgC9yUcLbAFuNbUHI4,470
-vmn-0.8.2rc1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-vmn-0.8.2rc1.dist-info/entry_points.txt,sha256=8JQYxf_iGN3GSYg7ezJs-P8FM3Ss6Hspgg6QcV_s3uk,47
-vmn-0.8.2rc1.dist-info/top_level.txt,sha256=nVR6dU2EinKSe5A4ZJa7NR1aOPNV7QMXvB5Sm-rWbJs,14
-vmn-0.8.2rc1.dist-info/RECORD,,
+version_stamp/stamp_utils.py,sha256=uzHbTJwDRB8m0ECj88WmIz8-qynzMX8gd12OaL8sonM,53161
+version_stamp/version.py,sha256=kgkQJNiKLG4ZGU5sBP2icY_Rrxm3IWIRbdV7wq2ODek,50
+version_stamp/vmn.py,sha256=imFHAynh5i-A8kn7HjIykSmLpk4kde__SC1-Q9UmZbY,109842
+vmn-0.8.4.dist-info/LICENSE.txt,sha256=f6flbA23EQX0tZpqCsQCJesFmHb4XNOAOD99egZuaL4,35127
+vmn-0.8.4.dist-info/METADATA,sha256=dVQ0lqUcvSRFSaGcitliXZ6R03rs2jVudl8PGnznfFs,467
+vmn-0.8.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+vmn-0.8.4.dist-info/entry_points.txt,sha256=8JQYxf_iGN3GSYg7ezJs-P8FM3Ss6Hspgg6QcV_s3uk,47
+vmn-0.8.4.dist-info/top_level.txt,sha256=nVR6dU2EinKSe5A4ZJa7NR1aOPNV7QMXvB5Sm-rWbJs,14
+vmn-0.8.4.dist-info/RECORD,,
```

