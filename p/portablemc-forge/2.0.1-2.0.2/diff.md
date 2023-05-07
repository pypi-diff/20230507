# Comparing `tmp/portablemc-forge-2.0.1.tar.gz` & `tmp/portablemc-forge-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portablemc-forge-2.0.1.tar", max compression
+gzip compressed data, was "portablemc-forge-2.0.2.tar", max compression
```

## Comparing `portablemc-forge-2.0.1.tar` & `portablemc-forge-2.0.2.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0    13009 2022-08-06 07:48:20.948435 portablemc-forge-2.0.1/portablemc_forge/__init__.py
--rw-r--r--   0        0        0       86 2022-06-12 20:34:32.742066 portablemc-forge-2.0.1/portablemc_forge/wrapper/.gitignore
--rw-r--r--   0        0        0     1334 2022-06-12 20:34:32.743065 portablemc-forge-2.0.1/portablemc_forge/wrapper/pom.xml
--rw-r--r--   0        0        0       80 2022-06-12 20:34:32.746064 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/argo/jdom/AbstractJsonObject.java
--rw-r--r--   0        0        0      350 2022-06-12 20:34:32.746064 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/argo/jdom/JsonField.java
--rw-r--r--   0        0        0      169 2022-06-12 20:34:32.747063 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/argo/jdom/JsonNode.java
--rw-r--r--   0        0        0      270 2022-06-12 20:34:32.757058 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/argo/jdom/JsonNodeFactories.java
--rw-r--r--   0        0        0      230 2022-06-12 20:34:32.763054 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/argo/jdom/JsonObject.java
--rw-r--r--   0        0        0       77 2022-06-12 20:34:32.764053 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/argo/jdom/JsonRootNode.java
--rw-r--r--   0        0        0      333 2022-06-12 20:34:32.764053 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/argo/jdom/JsonStringNode.java
--rw-r--r--   0        0        0       92 2022-06-12 20:34:32.768052 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/com/google/common/base/Predicate.java
--rw-r--r--   0        0        0      262 2022-06-12 20:34:32.777047 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/actions/Action.java
--rw-r--r--   0        0        0      171 2022-06-12 20:34:32.778046 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/actions/ActionCanceledException.java
--rw-r--r--   0        0        0      422 2022-06-12 20:34:32.778046 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/actions/ClientInstall.java
--rw-r--r--   0        0        0      200 2022-06-12 20:34:32.779045 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/actions/ProgressCallback.java
--rw-r--r--   0        0        0      325 2022-06-12 20:34:32.771051 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/ActionType.java
--rw-r--r--   0        0        0      545 2022-06-12 20:34:32.771051 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/ClientInstall.java
--rw-r--r--   0        0        0       96 2022-06-12 20:34:32.779045 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/json/Install.java
--rw-r--r--   0        0        0       88 2022-06-12 20:34:32.780045 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/json/InstallV1.java
--rw-r--r--   0        0        0      136 2022-06-12 20:34:32.780045 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/json/Util.java
--rw-r--r--   0        0        0      281 2022-06-12 20:34:32.781043 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/package-info.java
--rw-r--r--   0        0        0      580 2022-06-12 20:34:32.772049 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/ServerInstall.java
--rw-r--r--   0        0        0      117 2022-06-12 20:34:32.773049 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/SimpleInstaller.java
--rw-r--r--   0        0        0      357 2022-06-12 20:34:32.774048 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/VersionInfo.java
--rw-r--r--   0        0        0      222 2022-06-12 20:34:32.781043 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/portablemc/wrapper/InstallRunner.java
--rw-r--r--   0        0        0     1670 2022-06-12 20:34:32.787041 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/portablemc/wrapper/InstallRunnerType.java
--rw-r--r--   0        0        0     1160 2022-06-12 20:34:32.787041 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/portablemc/wrapper/Main.java
--rw-r--r--   0        0        0     2603 2022-06-12 20:34:32.787041 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/portablemc/wrapper/V1InstallRunner.java
--rw-r--r--   0        0        0     1655 2022-06-12 20:34:32.788040 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/portablemc/wrapper/V2InstallRunner.java
--rw-r--r--   0        0        0     1052 2022-06-12 20:34:32.789039 portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/portablemc/wrapper/WrapperUtil.java
--rw-r--r--   0        0        0     9660 2022-06-12 20:34:32.790039 portablemc-forge-2.0.1/portablemc_forge/wrapper/target/wrapper.jar
--rw-r--r--   0        0        0      501 2022-08-07 19:15:13.754876 portablemc-forge-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     1816 2022-06-12 20:34:32.727075 portablemc-forge-2.0.1/README.md
--rw-r--r--   0        0        0     3057 1970-01-01 00:00:00.000000 portablemc-forge-2.0.1/setup.py
--rw-r--r--   0        0        0     2526 1970-01-01 00:00:00.000000 portablemc-forge-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    13035 2023-05-07 10:14:18.852648 portablemc-forge-2.0.2/portablemc_forge/__init__.py
+-rw-r--r--   0        0        0       86 2022-06-12 20:34:32.742066 portablemc-forge-2.0.2/portablemc_forge/wrapper/.gitignore
+-rw-r--r--   0        0        0     1334 2022-06-12 20:34:32.743065 portablemc-forge-2.0.2/portablemc_forge/wrapper/pom.xml
+-rw-r--r--   0        0        0       80 2022-06-12 20:34:32.746064 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/argo/jdom/AbstractJsonObject.java
+-rw-r--r--   0        0        0      616 2023-05-07 10:14:18.853649 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/argo/jdom/JsonConstants.java
+-rw-r--r--   0        0        0      350 2022-06-12 20:34:32.746064 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/argo/jdom/JsonField.java
+-rw-r--r--   0        0        0      326 2023-05-07 10:14:18.865648 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/argo/jdom/JsonNode.java
+-rw-r--r--   0        0        0      270 2022-06-12 20:34:32.757058 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/argo/jdom/JsonNodeFactories.java
+-rw-r--r--   0        0        0      102 2023-05-07 10:14:18.894650 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/argo/jdom/JsonNodeType.java
+-rw-r--r--   0        0        0      230 2022-06-12 20:34:32.763054 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/argo/jdom/JsonObject.java
+-rw-r--r--   0        0        0       77 2022-06-12 20:34:32.764053 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/argo/jdom/JsonRootNode.java
+-rw-r--r--   0        0        0      333 2022-06-12 20:34:32.764053 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/argo/jdom/JsonStringNode.java
+-rw-r--r--   0        0        0       92 2022-06-12 20:34:32.768052 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/com/google/common/base/Predicate.java
+-rw-r--r--   0        0        0      262 2022-06-12 20:34:32.777047 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/actions/Action.java
+-rw-r--r--   0        0        0      171 2022-06-12 20:34:32.778046 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/actions/ActionCanceledException.java
+-rw-r--r--   0        0        0      422 2022-06-12 20:34:32.778046 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/actions/ClientInstall.java
+-rw-r--r--   0        0        0      200 2022-06-12 20:34:32.779045 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/actions/ProgressCallback.java
+-rw-r--r--   0        0        0      325 2022-06-12 20:34:32.771051 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/ActionType.java
+-rw-r--r--   0        0        0      545 2022-06-12 20:34:32.771051 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/ClientInstall.java
+-rw-r--r--   0        0        0       96 2022-06-12 20:34:32.779045 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/json/Install.java
+-rw-r--r--   0        0        0       88 2022-06-12 20:34:32.780045 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/json/InstallV1.java
+-rw-r--r--   0        0        0      136 2022-06-12 20:34:32.780045 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/json/Util.java
+-rw-r--r--   0        0        0      281 2022-06-12 20:34:32.781043 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/package-info.java
+-rw-r--r--   0        0        0      580 2022-06-12 20:34:32.772049 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/ServerInstall.java
+-rw-r--r--   0        0        0      117 2022-06-12 20:34:32.773049 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/SimpleInstaller.java
+-rw-r--r--   0        0        0      353 2023-05-07 10:14:18.895649 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/VersionInfo.java
+-rw-r--r--   0        0        0      222 2022-06-12 20:34:32.781043 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/portablemc/wrapper/InstallRunner.java
+-rw-r--r--   0        0        0     1670 2022-06-12 20:34:32.787041 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/portablemc/wrapper/InstallRunnerType.java
+-rw-r--r--   0        0        0     1158 2023-05-07 10:14:18.896650 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/portablemc/wrapper/Main.java
+-rw-r--r--   0        0        0     3275 2023-05-07 10:14:18.897650 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/portablemc/wrapper/V1InstallRunner.java
+-rw-r--r--   0        0        0     1655 2022-06-12 20:34:32.788040 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/portablemc/wrapper/V2InstallRunner.java
+-rw-r--r--   0        0        0     1492 2023-05-07 10:14:18.897650 portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/portablemc/wrapper/WrapperUtil.java
+-rw-r--r--   0        0        0    10188 2023-05-07 10:14:18.898652 portablemc-forge-2.0.2/portablemc_forge/wrapper/target/wrapper.jar
+-rw-r--r--   0        0        0      501 2023-05-07 10:17:49.151564 portablemc-forge-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1816 2022-06-12 20:34:32.727075 portablemc-forge-2.0.2/README.md
+-rw-r--r--   0        0        0     3057 1970-01-01 00:00:00.000000 portablemc-forge-2.0.2/setup.py
+-rw-r--r--   0        0        0     2526 1970-01-01 00:00:00.000000 portablemc-forge-2.0.2/PKG-INFO
```

### Comparing `portablemc-forge-2.0.1/portablemc_forge/__init__.py` & `portablemc-forge-2.0.2/portablemc_forge/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 
         return True
 
     def prepare(self):
 
         # The main dir specific to forge, it needs to be
         self.main_dir = path.dirname(self.version.context.versions_dir)
-        if not path.samefile(self.main_dir, path.dirname(self.version.context.libraries_dir)):
+        if path.isfile(self.main_dir) and not path.samefile(self.main_dir, path.dirname(self.version.context.libraries_dir)):
             raise ForgeInvalidMainDirectory()
 
         last_dl_entry = None
         for possible_version in self.possible_artifact_versions:
             installer_url = f"https://maven.minecraftforge.net/net/minecraftforge/forge/{possible_version}/forge-{possible_version}-installer.jar"
             possible_entry = DownloadEntry(installer_url, self.installer_file, name=f"installer:{possible_version}")
             if last_dl_entry is None:
@@ -233,18 +233,19 @@
         wrapper_completed = subprocess.run([
             self.jvm_exec,
             "-cp", path.pathsep.join([wrapper_jar_file, self.installer_file]),
             "portablemc.wrapper.Main",
             self.main_dir,
             self.version.id
         ], stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+        
         os.remove(self.installer_file)
 
         if wrapper_completed.returncode != 0:
-            raise ForgeInstallerFailed(wrapper_completed.returncode, wrapper_completed.stdout.decode("utf-8"))
+            raise ForgeInstallerFailed(wrapper_completed.returncode, wrapper_completed.stdout)
 
 
 # Forge API
 
 def request_promo_versions() -> Dict[str, str]:
     raw = json_simple_request("https://files.minecraftforge.net/net/minecraftforge/forge/promotions_slim.json")
     return raw["promos"]
@@ -277,15 +278,15 @@
 # Errors
 
 class ForgeInvalidMainDirectory(Exception):
     pass
 
 
 class ForgeInstallerFailed(Exception):
-    def __init__(self, return_code: int, output: str):
+    def __init__(self, return_code: int, output: bytes):
         self.return_code = return_code
         self.output = output
 
 
 class ForgeVersionNotFound(BaseError):
 
     NOT_INSTALLED = "not_installed"
```

### Comparing `portablemc-forge-2.0.1/portablemc_forge/wrapper/pom.xml` & `portablemc-forge-2.0.2/portablemc_forge/wrapper/pom.xml`

 * *Files identical despite different names*

### Comparing `portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/ClientInstall.java` & `portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/ClientInstall.java`

 * *Files identical despite different names*

### Comparing `portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/ServerInstall.java` & `portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/net/minecraftforge/installer/ServerInstall.java`

 * *Files identical despite different names*

### Comparing `portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/portablemc/wrapper/InstallRunnerType.java` & `portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/portablemc/wrapper/InstallRunnerType.java`

 * *Files identical despite different names*

### Comparing `portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/portablemc/wrapper/Main.java` & `portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/portablemc/wrapper/Main.java`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 		
 		File mainDir = new File(args[0]);
 		
 		if (!mainDir.isDirectory()) {
 			System.out.println("error: invalid main directory");
 			System.exit(2);
 		}
-		
+
 		InstallRunner runner = InstallRunnerType.findAndBuildRunner();
 		
 		if (runner == null) {
 			System.out.println("error: cannot find an install runner");
 			System.exit(3);
 		} else {
 			System.out.println("info: using install runner " + runner.getClass().getSimpleName());
```

### Comparing `portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/portablemc/wrapper/V1InstallRunner.java` & `portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/portablemc/wrapper/V1InstallRunner.java`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 package portablemc.wrapper;
 
+import argo.jdom.JsonNode;
 import argo.jdom.JsonField;
 import argo.jdom.JsonRootNode;
 import argo.jdom.JsonStringNode;
 import net.minecraftforge.installer.ClientInstall;
 import net.minecraftforge.installer.ServerInstall;
 import net.minecraftforge.installer.VersionInfo;
 
@@ -19,45 +20,55 @@
  */
 public class V1InstallRunner extends InstallRunner {
 	
 	@Override
 	public String validate(File mainDir) {
 		if (!mainDir.isDirectory()) return "no main dir";
 		File versionRootDir = new File(mainDir, "versions");
-		File minecraftJarFile = VersionInfo.getMinecraftFile(versionRootDir);
-		return minecraftJarFile != null && minecraftJarFile.isFile() ? null : "no version jar file";
+		String version = VersionInfo.getMinecraftVersion();
+		File versionDir = new File(versionRootDir, version);
+		File versionJarFile = new File(versionDir, version + ".jar");
+		return versionJarFile != null && versionJarFile.isFile() ? null : "no version jar file";
 	}
 	
 	@Override
 	public boolean install(File mainDir, String versionId) throws Exception {
 		
 		Path launcherProfile = WrapperUtil.ensureLauncherProfile(mainDir);
 		
 		ServerInstall.headless = true;  // Used by the buildMonitor method to return a wrapper around System.out
 		
-		String oldVersionId = versionId;
-		
 		// Changing version id is quite complicated in this version because we need to change the internal
 		// JSON data through argo JDOM library which is an immutable one.
 		JsonRootNode installProfile = VersionInfo.INSTANCE.versionData;
-		outer: for (JsonField field0 : installProfile.getFieldList()) {
-			if ("install".equals(field0.getName().getText())) {
-				for (JsonField field1 : field0.getValue().getFieldList()) {
-					if ("target".equals(field1.getName().getText())) {
-						JsonStringNode targetNode = (JsonStringNode) field1.getValue();
-						oldVersionId = targetNode.getText();
-						Field field = JsonStringNode.class.getDeclaredField("value");
-						field.setAccessible(true);
-						field.set(targetNode, versionId);
-						break outer;
-					}
+
+		Field stringNodeValueField = JsonStringNode.class.getDeclaredField("value");
+		stringNodeValueField.setAccessible(true);
+		Field fieldValueField = JsonField.class.getDeclaredField("value");
+		fieldValueField.setAccessible(true);
+		Field constFalseField = Class.forName("argo.jdom.JsonConstants").getDeclaredField("FALSE");
+		constFalseField.setAccessible(true);
+		JsonNode constFalse = (JsonNode) constFalseField.get(null);
+
+		JsonStringNode targetNode = (JsonStringNode) installProfile.getNode("install", "target");
+		String oldVersionId = targetNode.getText();
+		stringNodeValueField.set(targetNode, versionId);
+
+		// Here we disable downloads of the libraries, these will be downloaded by the launcher.
+		for (JsonNode libNode : installProfile.getArrayNode("versionInfo", "libraries")) {
+			JsonRootNode libObjNode = (JsonRootNode) libNode;
+			for (JsonField libField : libObjNode.getFieldList()) {
+				String fieldName = libField.getName().getText();
+				if ("serverreq".equals(fieldName) || "clientreq".equals(fieldName)) {
+					// Disable requirement.
+					fieldValueField.set(libField, constFalse);
 				}
 			}
 		}
-		
+
 		ClientInstall install = new ClientInstall();
 		
 		boolean success = install.run(mainDir, a -> true);
 		
 		WrapperUtil.fixVersionMetaId(mainDir, oldVersionId, versionId);
 		
 		if (launcherProfile != null) {
```

### Comparing `portablemc-forge-2.0.1/portablemc_forge/wrapper/src/main/java/portablemc/wrapper/V2InstallRunner.java` & `portablemc-forge-2.0.2/portablemc_forge/wrapper/src/main/java/portablemc/wrapper/V2InstallRunner.java`

 * *Files identical despite different names*

### Comparing `portablemc-forge-2.0.1/README.md` & `portablemc-forge-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `portablemc-forge-2.0.1/setup.py` & `portablemc-forge-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
                       'wrapper/target/*']}
 
 install_requires = \
 ['portablemc>=3,<4']
 
 setup_kwargs = {
     'name': 'portablemc-forge',
-    'version': '2.0.1',
+    'version': '2.0.2',
     'description': "Start Minecraft using the Forge mod loader using '<exec> start forge:[<mc-version>]'.",
     'long_description': '# Forge add-on\nThe forge add-on allows you to install and run Minecraft with forge mod loader in a single command \nline!\n\n![PyPI - Version](https://img.shields.io/pypi/v/portablemc-forge?label=PyPI%20version&style=flat-square) &nbsp;![PyPI - Downloads](https://img.shields.io/pypi/dm/portablemc-forge?label=PyPI%20downloads&style=flat-square)\n\n```console\npip install --user portablemc-forge\n```\n\n## Usage\nThis add-on extends the syntax accepted by the [start](/README.md#start-the-game) sub-command, by \nprepending the version with `forge:`. Almost all releases are supported by forge, the latest \nreleases are often supported, if not please refer to forge website. You can also append either\n`-recommended` or `-latest` to the version to take the corresponding version according to the\nforge public information, this is reflecting the "Download Latest" and "Download Recommended" on\nthe forge website. You can also use version aliases like `release` or equivalent empty version \n(just `forge:`). You can also give the exact forge version like `1.18.1-39.0.7`, in such cases,\nno HTTP request is made if the version is already installed.\n\n*Note that this add-on uses the same JVM used to start the game (see `--jvm` argument).*\n\n## Examples\n```sh\nportablemc start forge:               # Start recommended forge version for latest release\nportablemc start forge:release        # Same as above\nportablemc start forge:1.18.1         # Start recommended forge for 1.18.1\nportablemc start forge:1.18.1-39.0.7  # Start the exact forge version 1.18.1-39.0.7\nportablemc start --dry forge:         # Install (and exit) recommended forge version for latest release\n```\n\n## Credits\n- [Forge Website](https://files.minecraftforge.net/net/minecraftforge/forge/)\n- Consider supporting [LexManos](https://www.patreon.com/LexManos/)\n',
     'author': 'Théo Rozier',
     'author_email': 'contact@theorozier.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `portablemc-forge-2.0.1/PKG-INFO` & `portablemc-forge-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portablemc-forge
-Version: 2.0.1
+Version: 2.0.2
 Summary: Start Minecraft using the Forge mod loader using '<exec> start forge:[<mc-version>]'.
 License: GPL-3.0-only
 Author: Théo Rozier
 Author-email: contact@theorozier.fr
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

