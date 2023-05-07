# Comparing `tmp/images_upload_cli-1.1.0.tar.gz` & `tmp/images_upload_cli-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "images_upload_cli-1.1.0.tar", max compression
+gzip compressed data, was "images_upload_cli-1.1.1.tar", max compression
```

## Comparing `images_upload_cli-1.1.0.tar` & `images_upload_cli-1.1.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-02-24 11:07:46.979031 images_upload_cli-1.1.0/LICENSE
--rw-r--r--   0        0        0     4984 2023-02-24 11:07:46.979031 images_upload_cli-1.1.0/README.md
--rw-r--r--   0        0        0     2740 2023-02-24 11:07:46.979031 images_upload_cli-1.1.0/pyproject.toml
--rwxr-xr-x   0        0        0      160 2023-02-24 11:07:46.979031 images_upload_cli-1.1.0/src/images_upload_cli/__init__.py
--rwxr-xr-x   0        0        0      180 2023-02-24 11:07:46.979031 images_upload_cli-1.1.0/src/images_upload_cli/__main__.py
--rwxr-xr-x   0        0        0     1733 2023-02-24 11:07:46.979031 images_upload_cli-1.1.0/src/images_upload_cli/cli.py
--rwxr-xr-x   0        0        0     9324 2023-02-24 11:07:46.979031 images_upload_cli-1.1.0/src/images_upload_cli/upload.py
--rwxr-xr-x   0        0        0     3072 2023-02-24 11:07:46.979031 images_upload_cli-1.1.0/src/images_upload_cli/util.py
--rw-r--r--   0        0        0     6050 1970-01-01 00:00:00.000000 images_upload_cli-1.1.0/setup.py
--rw-r--r--   0        0        0     5943 1970-01-01 00:00:00.000000 images_upload_cli-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-07 14:44:21.650243 images_upload_cli-1.1.1/LICENSE
+-rw-r--r--   0        0        0     5248 2023-05-07 14:44:21.650243 images_upload_cli-1.1.1/README.md
+-rw-r--r--   0        0        0     2506 2023-05-07 14:44:36.218438 images_upload_cli-1.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0      188 2023-05-07 14:44:21.650243 images_upload_cli-1.1.1/src/images_upload_cli/__init__.py
+-rwxr-xr-x   0        0        0      178 2023-05-07 14:44:21.650243 images_upload_cli-1.1.1/src/images_upload_cli/__main__.py
+-rwxr-xr-x   0        0        0     1710 2023-05-07 14:44:21.650243 images_upload_cli-1.1.1/src/images_upload_cli/cli.py
+-rwxr-xr-x   0        0        0    11016 2023-05-07 14:44:21.650243 images_upload_cli-1.1.1/src/images_upload_cli/upload.py
+-rwxr-xr-x   0        0        0     3057 2023-05-07 14:44:21.650243 images_upload_cli-1.1.1/src/images_upload_cli/util.py
+-rw-r--r--   0        0        0     6213 1970-01-01 00:00:00.000000 images_upload_cli-1.1.1/PKG-INFO
```

### Comparing `images_upload_cli-1.1.0/LICENSE` & `images_upload_cli-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `images_upload_cli-1.1.0/README.md` & `images_upload_cli-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,36 +35,38 @@
 | [freeimage](https://freeimage.host/)  |      -       | `https://iili.io/{id}.png`                           |
 | [gyazo](https://gyazo.com/)           |      +       | `https://i.gyazo.com/{id}.png`                       |
 | [imageban](https://imageban.ru/)      |      +       | `https://i2.imageban.ru/out/2022/07/30/{id}.png`     |
 | [imagebin](https://imagebin.ca/)      |      -       | `https://ibin.co/{id}.png`                           |
 | [imgbb](https://imgbb.com/)           |      +       | `https://i.ibb.co/{id}/image.png`                    |
 | [imgchest](https://imgchest.com/)     |      +       | `https://cdn.imgchest.com/files/{id}.png`            |
 | [imgur](https://imgur.com/)           |      -       | `https://i.imgur.com/{id}.png`                       |
+| [lensdump](https://lensdump.com/)     |      +       | `https://i.lensdump.com/i/{id}.png`                  |
 | [pictshare](https://pictshare.net/)   |      -       | `https://pictshare.net/{id}.png`                     |
 | [pixeldrain](https://pixeldrain.com/) |      -       | `https://pixeldrain.com/api/file/{id}`               |
 | [pixhost](https://pixhost.to/)        |      -       | `https://img75.pixhost.to/images/69/{id}_img.png`    |
 | [ptpimg](https://ptpimg.me/)          |      +       | `https://ptpimg.me/{id}.png`                         |
 | [smms](https://sm.ms/)                |      +       | `https://s2.loli.net/2022/07/30/{id}.png`            |
 | [sxcu](https://sxcu.net/)             |      -       | `https://sxcu.net/{id}.png`                          |
 | [telegraph](https://telegra.ph/)      |      -       | `https://telegra.ph/file/{id}.png`                   |
 | [thumbsnap](https://thumbsnap.com/)   |      +       | `https://thumbsnap.com/i/{id}.png`                   |
+| [tixte](https://tixte.com/)           |      +       | `https://{domain}.tixte.co/r/{id}.png`               |
 | [up2sha](https://up2sha.re/)          |      +       | `https://up2sha.re/media/raw/{id}.png`               |
 | [uplio](https://upl.io/)              |      +       | `https://upl.io/i/{id}.png`                          |
 | [uploadcare](https://uploadcare.com/) |      +       | `https://ucarecdn.com/{id}/img.png`                  |
 | [vgy](https://vgy.me/)                |      +       | `https://i.vgy.me/{id}.png`                          |
 
 ## Usage
 
 ```sh
 Usage: images-upload-cli [OPTIONS] IMAGES...
 
   Upload images via APIs.
 
 Options:
-  -h, --hosting [beeimg|catbox|fastpic|filecoffee|freeimage|gyazo|imageban|imagebin|imgbb|imgchest|imgur|pictshare|pixeldrain|pixhost|ptpimg|smms|sxcu|telegraph|thumbsnap|up2sha|uplio|uploadcare|vgy]
+  -h, --hosting [beeimg|catbox|fastpic|filecoffee|freeimage|gyazo|imageban|imagebin|imgbb|imgchest|imgur|lensdump|pictshare|pixeldrain|pixhost|ptpimg|smms|sxcu|telegraph|thumbsnap|tixte|up2sha|uplio|uploadcare|vgy]
                                   [default: imgur]
   -b, --bbcode                    Add bbcode tags.
   -t, --thumbnail                 Add caption thumbnail and bbcode tags.
   -c, --clipboard / -C, --no-clipboard
                                   Copy result to clipboard.  [default: c]
   --version                       Show the version and exit.
   --help                          Show this message and exit.
@@ -77,17 +79,19 @@
 
 FREEIMAGE_KEY=
 GYAZO_TOKEN=
 IMAGEBAN_TOKEN=
 IMGBB_KEY=
 IMGCHEST_KEY=
 IMGUR_CLIENT_ID=
+LENSDUMP_KEY=
 PTPIMG_KEY=
 SMMS_KEY=
 THUMBSNAP_KEY=
+TIXTE_KEY=
 UP2SHA_KEY=
 UPLIO_KEY=
 UPLOADCARE_KEY=
 VGY_KEY=
 ```
 
 You can set these in environment variables, or in `.env` file:
```

### Comparing `images_upload_cli-1.1.0/pyproject.toml` & `images_upload_cli-1.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,110 +1,97 @@
+[build-system]
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
+
 [tool.poetry]
 name = "images-upload-cli"
-version = "1.1.0"
+version = "1.1.1"
 description = "Upload images via APIs"
-authors = ["DeadNews <uhjnnn@gmail.com>"]
+authors = ["DeadNews <aurczpbgr@mozmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/images-upload-cli"
 repository = "https://github.com/DeadNews/images-upload-cli"
 keywords = ["cli", "imgur", "image-upload", "upload-images", "upload-pictures"]
 classifiers = ["Environment :: Console", "Operating System :: OS Independent"]
 
 [tool.poetry.scripts]
 images-upload-cli = "images_upload_cli.cli:cli"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 click = "^8.1.3"
-pillow = "^9.4.0"
+pillow = "^9.5.0"
 pyperclip = "^1.8.2"
-python-dotenv = ">=0.21,<2.0.0"
-requests = "^2.28.2"
+python-dotenv = "^1.0.0"
+requests = "^2.30.0"
 
 [tool.poetry.group.ci.dependencies]
-bandit = "^1.7.4"
-black = "^22.12.0"
-flake8 = "^6.0.0"
-flake8-bugbear = "^23.2.13"
-flake8-builtins = "^2.1.0"
-flake8-comprehensions = "^3.10.1"
-flake8-implicit-str-concat = "^0.4.0"
-flake8-pie = "^0.16.0"
-flake8-pyproject = "^1.2.2"
-flake8-pytest-style = "^1.7.2"
-flake8-requirements = "^1.7.7"
-flake8-simplify = "^0.19.3"
-flake8-unused-arguments = "^0.0.13"
-flake8-use-pathlib = "^0.3.0"
-isort = "^5.12.0"
-mypy = "^1.0.1"
-pep8-naming = "^0.13.3"
-poethepoet = "^0.18.1"
-safety = "^2.3.5"
-types-requests = "^2.28.11.14"
+black = "^23.3.0"
+mypy = "^1.2.0"
+poethepoet = "^0.20.0"
+ruff = "^0.0.265"
+types-requests = "^2.29.0.0"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.2.1"
+pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poe.tasks]
+ruff = "ruff check ."
+black = "black --check ."
+mypy = "mypy ."
+ci.sequence = ["ruff", "black", "mypy"]
+
+[tool.poetry-dynamic-versioning]
+enable = false
+vcs = "git"
+style = "semver"
 
 [tool.black]
 line-length = 99
 
-[tool.isort]
-line_length = 99
-profile = "black"
-
-[tool.flake8]
-max-line-length = 99
-max-complexity = 18
-show-source = true
-ignore = [
-  "E501",   # Line too long.
-  "PIE786", # Use precise exception handlers.
-  "PIE803", # Use lazy % formatting in logging functions.
-  "W503",   # Line break occurred before a binary operator.
-]
-per-file-ignores = [
-  "tests/*: I900", # Package is not listed as a requirement.
-]
-
 [tool.mypy]
 disallow_untyped_defs = true
 follow_imports = "silent"
 ignore_missing_imports = true
 show_column_numbers = true
 show_error_codes = true
 warn_unused_ignores = true
 
 [[tool.mypy.overrides]]
 module = ["tests.*"]
 allow_untyped_defs = true
 
-[tool.bandit]
-exclude_dirs = ["tests"]
-skips = [
-  "B404", # Importing subprocess.
-  "B603", # Calling subprocess.Popen without shell=True.
-]
-
 [tool.pytest.ini_options]
 addopts = "--verbose --cov=./src"
 testpaths = ["tests"]
-markers = ["docker", "slow"]
+markers = ["docker", "key_required"]
 
 [tool.coverage.report]
-exclude_lines = ["if __name__ == .__main__.:"]
+exclude_lines = ["if TYPE_CHECKING:", "if __name__ == .__main__.:"]
 
-[tool.poe.tasks]
-isort = "isort . --check-only --diff"
-black = "black . --check --diff"
-mypy = "mypy ."
-flake8 = "flake8 ."
-bandit = "bandit -r . -c pyproject.toml"
-safety = "safety check -r pyproject.toml -o bare"
-ci.sequence = ["isort", "black", "mypy", "flake8", "bandit", "safety"]
-pc = "pre-commit run -a"
+[tool.ruff]
+line-length = 99
+select = ["ALL"]
+ignore = [
+  "COM812", # Trailing comma missing
+  "D203",   # 1 blank line required before class docstring
+  "D212",   # Multi-line docstring summary should start at the first line
+  "E501",   # Line too long
+  "EXE001", # Shebang is present but file is not executable
+  "FBT001", # Boolean positional arg in function definition
+  "FBT002", # Boolean default value in function definition
+  #
+  "S113", # Missing requests timeout
+  "S603", # Calling subprocess.Popen with shell=False
+]
+
+[tool.ruff.per-file-ignores]
+"__init__.py" = ["F401"]
+"tests/*" = ["ANN", "D", "PLC1901", "PLR2004", "S"]
+
+[tool.ruff.flake8-comprehensions]
+allow-dict-calls-with-keyword-arguments = false
+
+[tool.ruff.flake8-tidy-imports]
+ban-relative-imports = "all"
```

### Comparing `images_upload_cli-1.1.0/src/images_upload_cli/cli.py` & `images_upload_cli-1.1.1/src/images_upload_cli/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python
+"""Entrypoint for cli."""
 from __future__ import annotations
 
 from pathlib import Path
 
 import click
 from dotenv import load_dotenv
 from pyperclip import copy
@@ -32,17 +33,15 @@
 def cli(
     images: tuple[Path],
     hosting: str,
     bbcode: bool,
     thumbnail: bool,
     clipboard: bool,
 ) -> None:
-    """
-    Upload images via APIs.
-    """
+    """Upload images via APIs."""
     # loading .env variables
     load_dotenv(dotenv_path=get_config_path())
 
     # get upload func
     upload_func = UPLOAD[hosting]
 
     # image upload
@@ -60,11 +59,7 @@
 
     # out
     links_str = " ".join(links)
     click.echo(links_str)
     if clipboard:
         copy(links_str)
     kdialog(links_str)
-
-
-if __name__ == "__main__":
-    cli()
```

### Comparing `images_upload_cli-1.1.0/src/images_upload_cli/upload.py` & `images_upload_cli-1.1.1/src/images_upload_cli/upload.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 #!/usr/bin/env python
+"""Upload callables."""
 from __future__ import annotations
 
-from collections.abc import Callable
+from collections.abc import Callable  # noqa: TCH003
 from os import getenv
 from re import DOTALL, search, sub
 from urllib.parse import urlparse
 
 from requests import get, post
 
 from images_upload_cli.util import get_env_val, get_img_ext
 
 
 class UploadError(Exception):
-    pass
+    """Exception raised for upload errors."""
 
 
 def beeimg_upload(img: bytes) -> str:
+    """Upload to beeimg.com."""
     ext = f"img.{get_img_ext(img)}"
 
     response = post(
         url="https://beeimg.com/api/upload/file/json/",
         files={"file": (f"img.{ext}", img, f"image/{ext}")},
     )
     if not response.ok:
         raise UploadError(response.json())
 
     return f"https:{response.json()['files']['url']}"
 
 
 def catbox_upload(img: bytes) -> str:
+    """Upload to catbox.moe."""
     response = post(
         url="https://catbox.moe/user/api.php",
         data={"reqtype": "fileupload"},
         files={"fileToUpload": img},
     )
     if not response.ok:
         raise UploadError(response.text)
 
     return f"{response.text}"
 
 
 def fastpic_upload(img: bytes) -> str:
+    """Upload to fastpic.org."""
     response = post(
         url="https://fastpic.org/upload?api=1",
         data={
             "method": "file",
             "check_thumb": "no",
             "uploading": "1",
         },
@@ -59,142 +63,168 @@
     if image_link is None:
         raise UploadError(response.text)
 
     return image_link
 
 
 def filecoffee_upload(img: bytes) -> str:
+    """Upload to file.coffee."""
     response = post(
         url="https://file.coffee/api/file/upload",
         files={"file": img},
     )
     if not response.ok:
         raise UploadError(response.json())
 
     return response.json()["url"]
 
 
 def freeimage_upload(img: bytes) -> str:
+    """Upload to freeimage.host."""
     key = get_env_val("FREEIMAGE_KEY")
 
     response = post(
         url="https://freeimage.host/api/1/upload",
         data={"key": key},
         files={"source": img},
     )
     if not response.ok:
         raise UploadError(response.json())
 
     return response.json()["image"]["url"]
 
 
 def gyazo_upload(img: bytes) -> str:
+    """Upload to gyazo.com."""
     key = get_env_val("GYAZO_TOKEN")
 
     response = post(
         url=f"https://upload.gyazo.com/api/upload?access_token={key}",
         files={"imagedata": img},
     )
     if not response.ok:
         raise UploadError(response.json())
 
     return response.json()["url"]
 
 
 def imageban_upload(img: bytes) -> str:
+    """Upload to imageban.ru."""
     token = get_env_val("IMAGEBAN_TOKEN")
 
     response = post(
         url="https://api.imageban.ru/v1",
         headers={"Authorization": f"TOKEN {token}"},
         files={"image": img},
     )
     if not response.ok:
         raise UploadError(response.json())
 
     return response.json()["data"]["link"]
 
 
 def imagebin_upload(img: bytes) -> str:
+    """Upload to imagebin.ca."""
     response = post(
         url="https://imagebin.ca/upload.php",
         files={"file": img},
     )
     if not response.ok:
         raise UploadError(response.text)
 
     return sub(r".*url:", "", response.text, flags=DOTALL)
 
 
 def imgbb_upload(img: bytes) -> str:
+    """Upload to imgbb.com."""
     key = get_env_val("IMGBB_KEY")
 
     response = post(
         url="https://api.imgbb.com/1/upload",
         data={"key": key},
         files={"image": img},
     )
     if not response.ok:
         raise UploadError(response.json())
 
     return response.json()["data"]["url"]
 
 
 def imgchest_upload(img: bytes) -> str:
+    """Upload to imgchest.com."""
     key = get_env_val("IMGCHEST_KEY")
-    name = f"img.{get_img_ext(img)}"
+    ext = get_img_ext(img)
 
     response = post(
         url="https://api.imgchest.com/v1/post",
         headers={"Authorization": f"Bearer {key}"},
-        files={"images[]": (name, img)},
+        files={"images[]": (f"img.{ext}", img)},
     )
     if not response.ok:
         raise UploadError(response.json())
 
     return response.json()["data"]["images"][0]["link"].replace("comfiles", "com/files")
 
 
 def imgur_upload(img: bytes) -> str:
+    """Upload to imgur.com."""
     client_id = getenv("IMGUR_CLIENT_ID", "dd32dd3c6aaa9a0")
 
     response = post(
         url="https://api.imgur.com/3/image",
         headers={"Authorization": f"Client-ID {client_id}"},
         files={"image": img},
     )
     if not response.ok:
         raise UploadError(response.json())
 
     return response.json()["data"]["link"]
 
 
+def lensdump_upload(img: bytes) -> str:
+    """Upload to lensdump.com."""
+    key = get_env_val("LENSDUMP_KEY")
+
+    response = post(
+        url="https://lensdump.com/api/1/upload",
+        data={"key": key},
+        files={"source": img},
+    )
+    if not response.ok:
+        raise UploadError(response.json())
+
+    return response.json()["image"]["url"]
+
+
 def pictshare_upload(img: bytes) -> str:
+    """Upload to pictshare.net."""
     response = post(
         url="https://pictshare.net/api/upload.php",
         files={"file": img},
     )
     if not response.ok:
         raise UploadError(response.json())
 
     return response.json()["url"]
 
 
 def pixeldrain_upload(img: bytes) -> str:
+    """Upload to pixeldrain.com."""
     response = post(
         url="https://pixeldrain.com/api/file",
         files={"file": img},
     )
     if not response.ok:
         raise UploadError(response.json())
 
     return f"https://pixeldrain.com/api/file/{response.json()['id']}"
 
 
 def pixhost_upload(img: bytes) -> str:
+    """Upload to pixhost.to."""
     response = post(
         url="https://api.pixhost.to/images",
         data={"content_type": 0},
         files={"img": img},
     )
     if not response.ok:
         raise UploadError(response.json())
@@ -209,28 +239,30 @@
     )
     image_link = None if match is None else match.group(0).strip()
 
     return show_url if image_link is None else image_link
 
 
 def ptpimg_upload(img: bytes) -> str:
+    """Upload to ptpimg.me."""
     key = get_env_val("PTPIMG_KEY")
 
     response = post(
         url="https://ptpimg.me/upload.php",
         data={"api_key": key},
         files={"file-upload[0]": img},
     )
     if not response.ok:
         raise UploadError(response.json())
 
     return f"https://ptpimg.me/{response.json()[0]['code']}.{response.json()[0]['ext']}"
 
 
 def smms_upload(img: bytes) -> str:
+    """Upload to sm.ms."""
     key = get_env_val("SMMS_KEY")
 
     response = post(
         url="https://sm.ms/api/v2/upload",
         headers={"Authorization": key},
         files={"smfile": img},
     )
@@ -241,50 +273,71 @@
         response.json()["images"]
         if response.json()["code"] == "image_repeated"
         else response.json()["data"]["url"]
     )
 
 
 def sxcu_upload(img: bytes) -> str:
+    """Upload to sxcu.net."""
     response = post(
         url="https://sxcu.net/api/files/create",
         files={"file": img},
     )
     if not response.ok:
         raise UploadError(response.text)
 
     return f"{response.json()['url']}.{get_img_ext(img)}"
 
 
 def telegraph_upload(img: bytes) -> str:
+    """Upload to telegra.ph."""
     response = post(
         url="https://telegra.ph/upload",
         files={"file": img},
     )
     if not response.ok:
         raise UploadError(response.json())
 
     return f"https://telegra.ph{response.json()[0]['src']}"
 
 
 def thumbsnap_upload(img: bytes) -> str:
+    """Upload to thumbsnap.com."""
     key = get_env_val("THUMBSNAP_KEY")
 
     response = post(
         url="https://thumbsnap.com/api/upload",
         data={"key": key},
         files={"media": img},
     )
     if not response.ok:
         raise UploadError(response.json())
 
     return response.json()["data"]["media"]
 
 
+def tixte_upload(img: bytes) -> str:
+    """Upload to tixte.com."""
+    key = get_env_val("TIXTE_KEY")
+    ext = get_img_ext(img)
+
+    response = post(
+        url="https://api.tixte.com/v1/upload",
+        headers={"Authorization": key},
+        data={"payload_json": '{"random":true}'},
+        files={"file": (f"img.{ext}", img)},
+    )
+    if not response.ok:
+        raise UploadError(response.json())
+
+    return response.json()["data"]["direct_url"]
+
+
 def up2sha_upload(img: bytes) -> str:
+    """Upload to up2sha.re."""
     key = get_env_val("UP2SHA_KEY")
     ext = get_img_ext(img)
 
     response = post(
         url="https://api.up2sha.re/files",
         headers={"X-Api-Key": key},
         files={"file": (f"img.{ext}", img)},
@@ -292,14 +345,15 @@
     if not response.ok:
         raise UploadError(response.json())
 
     return f"{response.json()['public_url'].replace('file?f=', 'media/raw/')}.{ext}"
 
 
 def uplio_upload(img: bytes) -> str:
+    """Upload to upl.io."""
     key = get_env_val("UPLIO_KEY")
     ext = get_img_ext(img)
 
     response = post(
         url="https://upl.io",
         data={"key": key},
         files={"file": (f"img.{ext}", img)},
@@ -308,14 +362,15 @@
         raise UploadError(response.text)
 
     host, uid = response.text.rsplit("/", 1)
     return f"{host}/i/{uid}.{ext}"
 
 
 def uploadcare_upload(img: bytes) -> str:
+    """Upload to uploadcare.com."""
     key = get_env_val("UPLOADCARE_KEY")
     name = f"img.{get_img_ext(img)}"
 
     response = post(
         url="https://upload.uploadcare.com/base/",
         data={
             "UPLOADCARE_PUB_KEY": key,
@@ -326,21 +381,22 @@
     if not response.ok:
         raise UploadError(response.json())
 
     return f"https://ucarecdn.com/{response.json()['filename']}/{name}"
 
 
 def vgy_upload(img: bytes) -> str:
+    """Upload to vgy.me."""
     key = get_env_val("VGY_KEY")
-    name = f"img.{get_img_ext(img)}"
+    ext = get_img_ext(img)
 
     response = post(
         url="https://vgy.me/upload",
         data={"userkey": key},
-        files={"file[]": (name, img)},
+        files={"file[]": (f"img.{ext}", img)},
     )
     if not response.ok:
         raise UploadError(response.json())
 
     return response.json()["image"]
 
 
@@ -352,22 +408,24 @@
     "freeimage": freeimage_upload,
     "gyazo": gyazo_upload,
     "imageban": imageban_upload,
     "imagebin": imagebin_upload,
     "imgbb": imgbb_upload,
     "imgchest": imgchest_upload,
     "imgur": imgur_upload,
+    "lensdump": lensdump_upload,
     "pictshare": pictshare_upload,
     "pixeldrain": pixeldrain_upload,
     "pixhost": pixhost_upload,
     "ptpimg": ptpimg_upload,
     "smms": smms_upload,
     "sxcu": sxcu_upload,
     "telegraph": telegraph_upload,
     "thumbsnap": thumbsnap_upload,
+    "tixte": tixte_upload,
     "up2sha": up2sha_upload,
     "uplio": uplio_upload,
     "uploadcare": uploadcare_upload,
     "vgy": vgy_upload,
 }
 
 HOSTINGS = tuple(UPLOAD.keys())
```

### Comparing `images_upload_cli-1.1.0/src/images_upload_cli/util.py` & `images_upload_cli-1.1.1/src/images_upload_cli/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,79 @@
 #!/usr/bin/env python
+"""Utils."""
 from __future__ import annotations
 
 from io import BytesIO
 from os import getenv
 from pathlib import Path
 from shutil import which
 from subprocess import Popen
 
 import click
 from PIL import Image, ImageDraw, ImageFont
 
 
-class GetenvError(Exception):
-    pass
+class GetEnvError(Exception):
+    """Exception raised for getenv errors."""
 
 
 def get_config_path() -> Path:
-    """
-    Get app config path.
-    """
+    """Get app config path."""
     return Path(f"{click.get_app_dir('images-upload-cli')}/.env")
 
 
 def get_env_val(key: str) -> str:
-    """
-    Get value from env.
-    """
+    """Get value from env."""
     if value := getenv(key):
         return value
-    else:
-        raise GetenvError(
-            f"Please setup {key} in environment variables or in '{get_config_path()}'."
-        )
+
+    msg = f"Please setup {key} in environment variables or in '{get_config_path()}'."
+    raise GetEnvError(msg)
 
 
 def human_size(num: float, suffix: str = "B") -> str:
-    """
-    This function will convert bytes to human readable units.
-    """
+    """Convert bytes to human readable units."""
+    round_num = 1024.0
     for unit in ["", "Ki", "Mi", "Gi", "Ti", "Pi", "Ei", "Zi"]:
-        if abs(num) < 1024.0:
+        if abs(num) < round_num:
             return f"{num:3.1f} {unit}{suffix}"
-        num /= 1024.0
+        num /= round_num
     return f"{num:.1f} Yi{suffix}"
 
 
 def get_img_ext(img: bytes) -> str:
-    """
-    Get image extension from bytes.
-    """
+    """Get image extension from bytes."""
     return Image.open(BytesIO(img)).format.lower()
 
 
 def get_font() -> ImageFont.FreeTypeFont:
-    """
-    Attempts to retrieve a reasonably-looking TTF font from the system.
-    """
+    """Attempt to retrieve a reasonably-looking TTF font from the system."""
     font_names = [
         "Helvetica",
         "NotoSerif-Regular",
         "Menlo",
         "DejaVuSerif",
         "arial",
     ]
 
     for font_name in font_names:
         try:
             return ImageFont.truetype(font_name, size=14)
         except OSError:
             continue
 
-    raise GetenvError(
+    msg = (
         f"None of the default fonts were found: {font_names}.\n"
-        f"Please setup CAPTION_FONT in environment variables or in '{get_config_path()}'."
+        f"Please setup CAPTION_FONT in environment variables or in '{get_config_path()}'.",
     )
+    raise GetEnvError(msg)
 
 
 def make_thumbnail(img: bytes, size: tuple[int, int] = (300, 300)) -> bytes:
-    """
-    Make this image into a captioned thumbnail.
-    """
+    """Make this image into a captioned thumbnail."""
     # get a pw
     im = Image.open(BytesIO(img))
     pw = im.copy().convert("RGB")
     pw.thumbnail(size=size, resample=Image.Resampling.LANCZOS)
 
     # make a blank image for the text
     pw_with_line = Image.new(
@@ -122,12 +112,10 @@
         progressive=True,
     )
 
     return buffer.getvalue()
 
 
 def kdialog(text_to_print: str) -> None:
-    """
-    Kde notifications.
-    """
+    """Kde notifications."""
     if kdialog := which("kdialog"):
         Popen([kdialog, "--passivepopup", text_to_print])
```

### Comparing `images_upload_cli-1.1.0/setup.py` & `images_upload_cli-1.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,127 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: images-upload-cli
+Version: 1.1.1
+Summary: Upload images via APIs
+Home-page: https://github.com/DeadNews/images-upload-cli
+License: MIT
+Keywords: cli,imgur,image-upload,upload-images,upload-pictures
+Author: DeadNews
+Author-email: aurczpbgr@mozmail.com
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: pillow (>=9.5.0,<10.0.0)
+Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: requests (>=2.30.0,<3.0.0)
+Project-URL: Repository, https://github.com/DeadNews/images-upload-cli
+Description-Content-Type: text/markdown
+
+# images-upload-cli
+
+> Upload images via APIs
+
+[![PyPI version](https://img.shields.io/pypi/v/images-upload-cli)](https://pypi.org/project/images-upload-cli)
+[![AUR version](https://img.shields.io/aur/version/python-images-upload-cli)](https://aur.archlinux.org/packages/python-images-upload-cli)
+[![CI/CD](https://github.com/DeadNews/images-upload-cli/actions/workflows/python-app.yml/badge.svg)](https://github.com/DeadNews/images-upload-cli/actions/workflows/python-app.yml)
+[![pre-commit.ci](https://results.pre-commit.ci/badge/github/DeadNews/images-upload-cli/main.svg)](https://results.pre-commit.ci/latest/github/DeadNews/images-upload-cli/main)
+[![codecov](https://codecov.io/gh/DeadNews/images-upload-cli/branch/main/graph/badge.svg?token=OCZDZIYPMC)](https://codecov.io/gh/DeadNews/images-upload-cli)
+
+## Installation
+
+PyPI
+
+```sh
+pip install images-upload-cli
+# or
+pipx install images-upload-cli
+```
+
+AUR
+
+```sh
+yay -S python-images-upload-cli
+```
+
+## Hostings
+
+| host                                  | key required | return example                                       |
+| :------------------------------------ | :----------: | :--------------------------------------------------- |
+| [beeimg](https://beeimg.com/)         |      -       | `https://beeimg.com/images/{id}.png`                 |
+| [catbox](https://catbox.moe/)         |      -       | `https://files.catbox.moe/{id}`                      |
+| [fastpic](https://fastpic.org/)       |      -       | `https://i120.fastpic.org/big/2022/0730/d9/{id}.png` |
+| [filecoffee](https://file.coffee/)    |      -       | `https://file.coffee/u/{id}.png`                     |
+| [freeimage](https://freeimage.host/)  |      -       | `https://iili.io/{id}.png`                           |
+| [gyazo](https://gyazo.com/)           |      +       | `https://i.gyazo.com/{id}.png`                       |
+| [imageban](https://imageban.ru/)      |      +       | `https://i2.imageban.ru/out/2022/07/30/{id}.png`     |
+| [imagebin](https://imagebin.ca/)      |      -       | `https://ibin.co/{id}.png`                           |
+| [imgbb](https://imgbb.com/)           |      +       | `https://i.ibb.co/{id}/image.png`                    |
+| [imgchest](https://imgchest.com/)     |      +       | `https://cdn.imgchest.com/files/{id}.png`            |
+| [imgur](https://imgur.com/)           |      -       | `https://i.imgur.com/{id}.png`                       |
+| [lensdump](https://lensdump.com/)     |      +       | `https://i.lensdump.com/i/{id}.png`                  |
+| [pictshare](https://pictshare.net/)   |      -       | `https://pictshare.net/{id}.png`                     |
+| [pixeldrain](https://pixeldrain.com/) |      -       | `https://pixeldrain.com/api/file/{id}`               |
+| [pixhost](https://pixhost.to/)        |      -       | `https://img75.pixhost.to/images/69/{id}_img.png`    |
+| [ptpimg](https://ptpimg.me/)          |      +       | `https://ptpimg.me/{id}.png`                         |
+| [smms](https://sm.ms/)                |      +       | `https://s2.loli.net/2022/07/30/{id}.png`            |
+| [sxcu](https://sxcu.net/)             |      -       | `https://sxcu.net/{id}.png`                          |
+| [telegraph](https://telegra.ph/)      |      -       | `https://telegra.ph/file/{id}.png`                   |
+| [thumbsnap](https://thumbsnap.com/)   |      +       | `https://thumbsnap.com/i/{id}.png`                   |
+| [tixte](https://tixte.com/)           |      +       | `https://{domain}.tixte.co/r/{id}.png`               |
+| [up2sha](https://up2sha.re/)          |      +       | `https://up2sha.re/media/raw/{id}.png`               |
+| [uplio](https://upl.io/)              |      +       | `https://upl.io/i/{id}.png`                          |
+| [uploadcare](https://uploadcare.com/) |      +       | `https://ucarecdn.com/{id}/img.png`                  |
+| [vgy](https://vgy.me/)                |      +       | `https://i.vgy.me/{id}.png`                          |
+
+## Usage
+
+```sh
+Usage: images-upload-cli [OPTIONS] IMAGES...
+
+  Upload images via APIs.
+
+Options:
+  -h, --hosting [beeimg|catbox|fastpic|filecoffee|freeimage|gyazo|imageban|imagebin|imgbb|imgchest|imgur|lensdump|pictshare|pixeldrain|pixhost|ptpimg|smms|sxcu|telegraph|thumbsnap|tixte|up2sha|uplio|uploadcare|vgy]
+                                  [default: imgur]
+  -b, --bbcode                    Add bbcode tags.
+  -t, --thumbnail                 Add caption thumbnail and bbcode tags.
+  -c, --clipboard / -C, --no-clipboard
+                                  Copy result to clipboard.  [default: c]
+  --version                       Show the version and exit.
+  --help                          Show this message and exit.
+```
+
+## Env variables
+
+```ini
+CAPTION_FONT= # The default font is system dependent.
+
+FREEIMAGE_KEY=
+GYAZO_TOKEN=
+IMAGEBAN_TOKEN=
+IMGBB_KEY=
+IMGCHEST_KEY=
+IMGUR_CLIENT_ID=
+LENSDUMP_KEY=
+PTPIMG_KEY=
+SMMS_KEY=
+THUMBSNAP_KEY=
+TIXTE_KEY=
+UP2SHA_KEY=
+UPLIO_KEY=
+UPLOADCARE_KEY=
+VGY_KEY=
+```
+
+You can set these in environment variables, or in `.env` file:
+
+- Unix: `~/.config/images-upload-cli/.env`
+- MacOS: `~/Library/Application Support/images-upload-cli/.env`
+- Windows: `C:\Users\<user>\AppData\Roaming\images-upload-cli\.env`
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['images_upload_cli']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['click>=8.1.3,<9.0.0',
- 'pillow>=9.4.0,<10.0.0',
- 'pyperclip>=1.8.2,<2.0.0',
- 'python-dotenv>=0.21,<2.0.0',
- 'requests>=2.28.2,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['images-upload-cli = images_upload_cli.cli:cli']}
-
-setup_kwargs = {
-    'name': 'images-upload-cli',
-    'version': '1.1.0',
-    'description': 'Upload images via APIs',
-    'long_description': '# images-upload-cli\n\n> Upload images via APIs\n\n[![PyPI version](https://img.shields.io/pypi/v/images-upload-cli)](https://pypi.org/project/images-upload-cli)\n[![AUR version](https://img.shields.io/aur/version/python-images-upload-cli)](https://aur.archlinux.org/packages/python-images-upload-cli)\n[![CI/CD](https://github.com/DeadNews/images-upload-cli/actions/workflows/python-app.yml/badge.svg)](https://github.com/DeadNews/images-upload-cli/actions/workflows/python-app.yml)\n[![pre-commit.ci](https://results.pre-commit.ci/badge/github/DeadNews/images-upload-cli/main.svg)](https://results.pre-commit.ci/latest/github/DeadNews/images-upload-cli/main)\n[![codecov](https://codecov.io/gh/DeadNews/images-upload-cli/branch/main/graph/badge.svg?token=OCZDZIYPMC)](https://codecov.io/gh/DeadNews/images-upload-cli)\n\n## Installation\n\nPyPI\n\n```sh\npip install images-upload-cli\n# or\npipx install images-upload-cli\n```\n\nAUR\n\n```sh\nyay -S python-images-upload-cli\n```\n\n## Hostings\n\n| host                                  | key required | return example                                       |\n| :------------------------------------ | :----------: | :--------------------------------------------------- |\n| [beeimg](https://beeimg.com/)         |      -       | `https://beeimg.com/images/{id}.png`                 |\n| [catbox](https://catbox.moe/)         |      -       | `https://files.catbox.moe/{id}`                      |\n| [fastpic](https://fastpic.org/)       |      -       | `https://i120.fastpic.org/big/2022/0730/d9/{id}.png` |\n| [filecoffee](https://file.coffee/)    |      -       | `https://file.coffee/u/{id}.png`                     |\n| [freeimage](https://freeimage.host/)  |      -       | `https://iili.io/{id}.png`                           |\n| [gyazo](https://gyazo.com/)           |      +       | `https://i.gyazo.com/{id}.png`                       |\n| [imageban](https://imageban.ru/)      |      +       | `https://i2.imageban.ru/out/2022/07/30/{id}.png`     |\n| [imagebin](https://imagebin.ca/)      |      -       | `https://ibin.co/{id}.png`                           |\n| [imgbb](https://imgbb.com/)           |      +       | `https://i.ibb.co/{id}/image.png`                    |\n| [imgchest](https://imgchest.com/)     |      +       | `https://cdn.imgchest.com/files/{id}.png`            |\n| [imgur](https://imgur.com/)           |      -       | `https://i.imgur.com/{id}.png`                       |\n| [pictshare](https://pictshare.net/)   |      -       | `https://pictshare.net/{id}.png`                     |\n| [pixeldrain](https://pixeldrain.com/) |      -       | `https://pixeldrain.com/api/file/{id}`               |\n| [pixhost](https://pixhost.to/)        |      -       | `https://img75.pixhost.to/images/69/{id}_img.png`    |\n| [ptpimg](https://ptpimg.me/)          |      +       | `https://ptpimg.me/{id}.png`                         |\n| [smms](https://sm.ms/)                |      +       | `https://s2.loli.net/2022/07/30/{id}.png`            |\n| [sxcu](https://sxcu.net/)             |      -       | `https://sxcu.net/{id}.png`                          |\n| [telegraph](https://telegra.ph/)      |      -       | `https://telegra.ph/file/{id}.png`                   |\n| [thumbsnap](https://thumbsnap.com/)   |      +       | `https://thumbsnap.com/i/{id}.png`                   |\n| [up2sha](https://up2sha.re/)          |      +       | `https://up2sha.re/media/raw/{id}.png`               |\n| [uplio](https://upl.io/)              |      +       | `https://upl.io/i/{id}.png`                          |\n| [uploadcare](https://uploadcare.com/) |      +       | `https://ucarecdn.com/{id}/img.png`                  |\n| [vgy](https://vgy.me/)                |      +       | `https://i.vgy.me/{id}.png`                          |\n\n## Usage\n\n```sh\nUsage: images-upload-cli [OPTIONS] IMAGES...\n\n  Upload images via APIs.\n\nOptions:\n  -h, --hosting [beeimg|catbox|fastpic|filecoffee|freeimage|gyazo|imageban|imagebin|imgbb|imgchest|imgur|pictshare|pixeldrain|pixhost|ptpimg|smms|sxcu|telegraph|thumbsnap|up2sha|uplio|uploadcare|vgy]\n                                  [default: imgur]\n  -b, --bbcode                    Add bbcode tags.\n  -t, --thumbnail                 Add caption thumbnail and bbcode tags.\n  -c, --clipboard / -C, --no-clipboard\n                                  Copy result to clipboard.  [default: c]\n  --version                       Show the version and exit.\n  --help                          Show this message and exit.\n```\n\n## Env variables\n\n```ini\nCAPTION_FONT= # The default font is system dependent.\n\nFREEIMAGE_KEY=\nGYAZO_TOKEN=\nIMAGEBAN_TOKEN=\nIMGBB_KEY=\nIMGCHEST_KEY=\nIMGUR_CLIENT_ID=\nPTPIMG_KEY=\nSMMS_KEY=\nTHUMBSNAP_KEY=\nUP2SHA_KEY=\nUPLIO_KEY=\nUPLOADCARE_KEY=\nVGY_KEY=\n```\n\nYou can set these in environment variables, or in `.env` file:\n\n- Unix: `~/.config/images-upload-cli/.env`\n- MacOS: `~/Library/Application Support/images-upload-cli/.env`\n- Windows: `C:\\Users\\<user>\\AppData\\Roaming\\images-upload-cli\\.env`\n',
-    'author': 'DeadNews',
-    'author_email': 'uhjnnn@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/DeadNews/images-upload-cli',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8.1,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
```

