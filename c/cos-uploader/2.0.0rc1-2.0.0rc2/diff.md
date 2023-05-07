# Comparing `tmp/cos_uploader-2.0.0rc1.tar.gz` & `tmp/cos_uploader-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cos_uploader-2.0.0rc1.tar", max compression
+gzip compressed data, was "cos_uploader-2.0.0rc2.tar", max compression
```

## Comparing `cos_uploader-2.0.0rc1.tar` & `cos_uploader-2.0.0rc2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1091 2023-05-07 17:24:36.085023 cos_uploader-2.0.0rc1/LICENSE
--rw-r--r--   0        0        0     3373 2023-05-07 17:47:54.450391 cos_uploader-2.0.0rc1/README.md
--rw-r--r--   0        0        0     4597 2023-05-07 16:07:41.473804 cos_uploader-2.0.0rc1/cos_uploader/__init__.py
--rw-r--r--   0        0        0      716 2023-05-07 15:23:47.518741 cos_uploader-2.0.0rc1/cos_uploader/common.py
--rw-r--r--   0        0        0      631 2023-05-07 14:43:29.630252 cos_uploader-2.0.0rc1/cos_uploader/config.toml
--rw-r--r--   0        0        0     2052 2023-05-07 15:25:57.984080 cos_uploader-2.0.0rc1/cos_uploader/history.py
--rw-r--r--   0        0        0     1237 2023-05-07 15:55:54.170237 cos_uploader-2.0.0rc1/cos_uploader/install.py
--rw-r--r--   0        0        0      858 2023-05-07 17:49:10.009592 cos_uploader-2.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4262 1970-01-01 00:00:00.000000 cos_uploader-2.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-05-07 17:55:26.777619 cos_uploader-2.0.0rc2/LICENSE
+-rw-r--r--   0        0        0     4761 2023-05-07 18:08:41.052601 cos_uploader-2.0.0rc2/README.md
+-rw-r--r--   0        0        0     4597 2023-05-07 18:08:32.724769 cos_uploader-2.0.0rc2/cos_uploader/__init__.py
+-rw-r--r--   0        0        0      716 2023-05-07 17:55:26.778063 cos_uploader-2.0.0rc2/cos_uploader/common.py
+-rw-r--r--   0        0        0      631 2023-05-07 18:07:55.273444 cos_uploader-2.0.0rc2/cos_uploader/config.toml
+-rw-r--r--   0        0        0     2083 2023-05-07 18:07:37.244130 cos_uploader-2.0.0rc2/cos_uploader/history.py
+-rw-r--r--   0        0        0     1237 2023-05-07 17:55:26.778434 cos_uploader-2.0.0rc2/cos_uploader/install.py
+-rw-r--r--   0        0        0      858 2023-05-07 18:07:47.353705 cos_uploader-2.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     5650 1970-01-01 00:00:00.000000 cos_uploader-2.0.0rc2/PKG-INFO
```

### Comparing `cos_uploader-2.0.0rc1/LICENSE` & `cos_uploader-2.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `cos_uploader-2.0.0rc1/cos_uploader/__init__.py` & `cos_uploader-2.0.0rc2/cos_uploader/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def progress_callback(consumed_bytes, total_bytes):
     if total_bytes:
         rate = int(100 * (float(consumed_bytes) / float(total_bytes)))
         print('\r{0}% '.format(rate), end="", file=sys.stderr, flush=True)
 
 
 def get_filename(file, config):
-    current_time = datetime.datetime.now() if not config["utc_time"] else datetime.datetime.utcnow()
+    current_time = datetime.datetime.now() if not config["utc-time"] else datetime.datetime.utcnow()
     filename, extension = os.path.splitext(os.path.basename(file))
     params = {
         "uuid": str(uuid.uuid4()),
         "name": filename,
         "ext": extension,
         "y": current_time.strftime("%Y"),
         "mo": current_time.strftime("%m"),
@@ -63,15 +63,15 @@
 def upload_to_cos(file, config, typora):
     if not (os.path.exists(file)):
         return None if typora else print(f"ERROR: File Not Found: {file}", file=sys.stderr)
     if os.path.isdir(file):
         return None if typora else print(f"WARNING: Skipping Folder: {file}", file=sys.stderr)
 
     client = CosS3Client(CosConfig(
-        Region="accelerate" if config["oversea_upload"] else config["region"],
+        Region="accelerate" if config["oversea-upload"] else config["region"],
         SecretId=config["secret-id"],
         SecretKey=config["secret-key"]))
     key = get_filename(file, config)
     response = client.upload_file(
         Bucket=config["bucket"],
         LocalFilePath=file,
         Key=key,
```

### Comparing `cos_uploader-2.0.0rc1/cos_uploader/common.py` & `cos_uploader-2.0.0rc2/cos_uploader/common.py`

 * *Files identical despite different names*

### Comparing `cos_uploader-2.0.0rc1/cos_uploader/config.toml` & `cos_uploader-2.0.0rc2/cos_uploader/config.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 secret-id  = "AKIDxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
 secret-key = "qqXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
 region = "ap-shanghai"
 bucket = "bucket-name-1250000000"
 prefix = "cos-uploader/v2/"
 filename = "{uuid}/{y}-{mo}-{d}-{h}-{min}-{s}-utc-{ts}/{name}{ext}"
-utc_time = true
-oversea_upload = false
+utc-time = true
+oversea-upload = false
 
 [domains]
 # domain types: cos, cdn, web, accelerate
 enabled = ["cdn", "cos", "web", "accelerate"]
 
 # available parameters: bucket, region
 cdn = "{bucket}.file.myqcloud.com"
```

### Comparing `cos_uploader-2.0.0rc1/cos_uploader/history.py` & `cos_uploader-2.0.0rc2/cos_uploader/history.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,19 +15,21 @@
     args = parser.parse_args()
 
     year = int(args.year)
     month = int(args.month)
     if year < 2000 or year > 2100 or month < 1 or month > 12:
         print("ERROR: Invalid Year or Month", file=sys.stderr)
         sys.exit(1)
+    year = str(year)
+    month = str(month).zfill(2)
 
     config = load_config()
-    file = os.path.join(config["base"], f"history-{args.year}-{args.month}.ndjson")
+    file = os.path.join(config["base"], f"history-{year}-{month}.log")
     if not os.path.exists(file):
-        print(f"ERROR: History File '{file}' Not Found, maybe you have not uploaded any files in {args.year}-{args.month}?", file=sys.stderr)
+        print(f"ERROR: History File '{file}' Not Found, maybe you have not uploaded any files in {year}-{month} ?", file=sys.stderr)
         sys.exit(1)
     
     lines = []
     with open(file, "r", encoding="utf-8") as f:
         if args.limit == 0:
             lines = f.readlines()
         else:
```

### Comparing `cos_uploader-2.0.0rc1/cos_uploader/install.py` & `cos_uploader-2.0.0rc2/cos_uploader/install.py`

 * *Files identical despite different names*

### Comparing `cos_uploader-2.0.0rc1/pyproject.toml` & `cos_uploader-2.0.0rc2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cos-uploader"
-version = "2.0.0-rc.1"
+version = "2.0.0-rc.2"
 description = "CLI tool for uploading files to Tencent COS"
 authors = ["Joseph Chris <joseph@josephcz.xyz>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "cos_uploader"}]
 include = ["cos_uploader/config.toml"]
 homepage = "https://github.com/baobao1270/cos-uploader"
```

### Comparing `cos_uploader-2.0.0rc1/PKG-INFO` & `cos_uploader-2.0.0rc2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: cos-uploader
-Version: 2.0.0rc1
-Summary: CLI tool for uploading files to Tencent COS
-Home-page: https://github.com/baobao1270/cos-uploader
-License: MIT
-Keywords: tencent-cos,uploader
-Author: Joseph Chris
-Author-email: joseph@josephcz.xyz
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: cos-python-sdk-v5 (>=1.9.24,<2.0.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
-Project-URL: Documentation, https://github.com/baobao1270/cos-uploader/blob/main/README.md
-Project-URL: Repository, https://github.com/baobao1270/cos-uploader.git
-Description-Content-Type: text/markdown
-
 # COS Uploader
 
 跨平台的腾讯云对象存储上传工具
 
  - 支持 Windows、Linux、MacOS
  - 可以用于图片上传（图床）、文件分享等
  - 带有日志记录功能，可以查看上传历史
@@ -58,31 +36,72 @@
  - 重新启动当前 shell，如 `exec zsh` 或 `exec bash`
  - 重新启动当前终端，在 GUI 下应退出终端应用（iTerm2 下按 <kbd>Command ⌘</kbd> + <kbd>Q</kbd>、Windows Terminal 下关闭窗口）
  - 查看 PATH 变量
     - 使用 pipx，需要根据 pipx 的提示将 `~/.local/bin` 添加到 PATH
     - Windows 版的 Python 默认不会将 `Scripts` 添加到 PATH，需要手动添加。打开 [设置——系统——关于](ms-settings:about) 点击右侧「高级系统设置」，添加 `C:\Users\<用户名>\AppData\Roaming\Python\<Python版本>\Scripts` 到 PATH
     - 如果使用了手动创建虚拟环境安装（安装方法 3），请将 `~/.cos-uploader/bin` 添加到 PATH
 
-### Windows 的特殊配置
+配置完成后，可以使用 `cos-uploader` 命令来上传文件。
+
+```bash
+# 上传文件试试，测试配置是否正确
+echo "Hello World" > hello.txt
+cos-uploader hello.txt
+```
+
+### Windows 平台功能
 在运行 `cos-uploader-install` 时，会自动创建「发送到」菜单项。
 
-在配置完成后，右键单击文件，在菜单中选择「发送到」，然后选择「COS Uploader」即可上传文件。
+配置完成 `config.toml`后，在「资源管理器」中右键想要上传的文件，在菜单中选择「发送到」，然后选择「COS Uploader」即可上传该文件。
 
-### MacOS 的特殊配置
+### MacOS 平台功能
 
 请导入 [COS Uploader 快捷指令](https://www.icloud.com/shortcuts/76e95603ee464cddb0a7af9afe89c719)
 
 导入完成后，请打开「快捷指令」App，选择左上角菜单中的「快捷指令——设置——高级」，勾选「允许运行脚本」。
 
-完成后，可以在 Finder 的「快速操作」菜单中选择「COS Uploader」来上传文件。
+配置完成 `config.toml` 后，在 Finder 中右键想要上传的文件，在菜单中选择「快速操作」，然后选择「COS Uploader」即可上传该文件。
+
+## 查看历史
+COS Uploader 会记录上传历史，可以通过 `cos-uploader-history` 命令来查看。输出记录按照时间戳降序排列。
+
+`cos-uploader-history` 默认会输出全部记录，可以通过 `-n` 参数来限制输出的记录数量。
+
+```bash
+cos-uploader-history -n 10
+```
+
+COS Uploader 按月分割文件，文件日志格式为 `~/cos-uploader/history-yyyy-MM.ndjson`，其中 `yyyy-MM` 为年月。`cos-uploader-history` 仅输出当前月份的记录，可以通过 `-y`、`-m` 参数来指定时间。
+
+```bash
+cos-uploader-history -y 2023 -m 1
+```
+
+COS Uploader 使用 NDJSON 格式来记录上传历史，可以通过 `cos-uploader-history -r` 来查看原始记录。
+
+```bash
+cos-uploader-history -n 10 -r
+```
 
 ### 优化海外使用体验
-如果您上传文件的设备位于中国大陆境外，请在配置中将 `oversea_upload` 设置为 `true`，这样可以提高上传速度。
+如果您上传文件的设备位于中国大陆境外，请修改 `config.toml` 如下：
+```toml
+oversea-upload = true
+```
 
-如果您的文件使用者位于中国大陆境外，请在配置中将 `[domains]` 节的 `enabled` 数组添加 `accelerate`，并使用输出的 `Acc URL` 来访问文件。
+如果您的文件使用者位于中国大陆境外，请修改 `config.toml` 如下，并使用输出的 `Acc URL` 来访问文件。注意：需要在腾讯云控制台开启该 bucket 的「加速域名」功能。
+```toml
+[domains]
+enabled = ["accelerate"]  # 在此处添加 accelerate，原来的可以删掉也可以保留
+```
+
+COS Uploader 默认在 URL 格式化的时候，使用 UTC 时间。如果需要使用本地时间（使用上传设备的系统时间），请修改 `config.toml` 如下：
+```toml
+utc-time = false
+```
 
 ## 构建
 COS Uploader 使用 Poetry 构建。请先安装 Poetry，然后执行以下命令：
 
 ```bash
 git clone https://github.com/baobao1270/cos-uploader.git
 cd cos-uploader
@@ -93,8 +112,7 @@
 
 ```bash
 poetry publish --build
 ```
 
 ## 许可
 COS Uploader 使用 MIT 协议
-
```

