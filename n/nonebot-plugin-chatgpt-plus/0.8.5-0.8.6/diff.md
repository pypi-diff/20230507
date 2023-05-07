# Comparing `tmp/nonebot-plugin-chatgpt-plus-0.8.5.tar.gz` & `tmp/nonebot-plugin-chatgpt-plus-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-chatgpt-plus-0.8.5.tar", last modified: Tue Apr 18 16:32:22 2023, max compression
+gzip compressed data, was "nonebot-plugin-chatgpt-plus-0.8.6.tar", last modified: Sun May  7 13:44:31 2023, max compression
```

## Comparing `nonebot-plugin-chatgpt-plus-0.8.5.tar` & `nonebot-plugin-chatgpt-plus-0.8.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2023-04-18 16:32:11.029165 nonebot-plugin-chatgpt-plus-0.8.5/LICENSE
--rw-r--r--   0        0        0     6831 2023-04-18 16:32:11.029165 nonebot-plugin-chatgpt-plus-0.8.5/README.md
--rw-r--r--   0        0        0    13362 2023-04-18 16:32:11.029165 nonebot-plugin-chatgpt-plus-0.8.5/nonebot_plugin_chatgpt_plus/__init__.py
--rw-r--r--   0        0        0    12072 2023-04-18 16:32:11.029165 nonebot-plugin-chatgpt-plus-0.8.5/nonebot_plugin_chatgpt_plus/chatgpt.py
--rw-r--r--   0        0        0     1043 2023-04-18 16:32:11.029165 nonebot-plugin-chatgpt-plus-0.8.5/nonebot_plugin_chatgpt_plus/config.py
--rw-r--r--   0        0        0      873 2023-04-18 16:32:11.029165 nonebot-plugin-chatgpt-plus-0.8.5/nonebot_plugin_chatgpt_plus/data.py
--rw-r--r--   0        0        0     5678 2023-04-18 16:32:11.029165 nonebot-plugin-chatgpt-plus-0.8.5/nonebot_plugin_chatgpt_plus/utils.py
--rw-r--r--   0        0        0      725 2023-04-18 16:32:11.029165 nonebot-plugin-chatgpt-plus-0.8.5/pyproject.toml
--rw-r--r--   0        0        0     7228 1970-01-01 00:00:00.000000 nonebot-plugin-chatgpt-plus-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-07 13:44:22.032722 nonebot-plugin-chatgpt-plus-0.8.6/LICENSE
+-rw-r--r--   0        0        0     6931 2023-05-07 13:44:22.032722 nonebot-plugin-chatgpt-plus-0.8.6/README.md
+-rw-r--r--   0        0        0    13495 2023-05-07 13:44:22.032722 nonebot-plugin-chatgpt-plus-0.8.6/nonebot_plugin_chatgpt_plus/__init__.py
+-rw-r--r--   0        0        0    12305 2023-05-07 13:44:22.032722 nonebot-plugin-chatgpt-plus-0.8.6/nonebot_plugin_chatgpt_plus/chatgpt.py
+-rw-r--r--   0        0        0     1078 2023-05-07 13:44:22.032722 nonebot-plugin-chatgpt-plus-0.8.6/nonebot_plugin_chatgpt_plus/config.py
+-rw-r--r--   0        0        0      900 2023-05-07 13:44:22.032722 nonebot-plugin-chatgpt-plus-0.8.6/nonebot_plugin_chatgpt_plus/data.py
+-rw-r--r--   0        0        0     5678 2023-05-07 13:44:22.032722 nonebot-plugin-chatgpt-plus-0.8.6/nonebot_plugin_chatgpt_plus/utils.py
+-rw-r--r--   0        0        0      725 2023-05-07 13:44:22.032722 nonebot-plugin-chatgpt-plus-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0     7328 1970-01-01 00:00:00.000000 nonebot-plugin-chatgpt-plus-0.8.6/PKG-INFO
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.5/LICENSE` & `nonebot-plugin-chatgpt-plus-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-plus-0.8.5/README.md` & `nonebot-plugin-chatgpt-plus-0.8.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 在 nonebot2 项目的 `.env` 文件中添加下表中的必填配置（在 **ARM** 平台，可能必须使用 `CHATGPT_SESSION_TOKEN` 登录）
 
 > ⚠️ **Windows** 系统下需要在 `.env.dev` 文件中设置 `FASTAPI_RELOAD=false`
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | CHATGPT_SESSION_TOKEN | 否 | 空字符串 | ChatGPT 的 session_token，如配置则优先使用 |
+| CHATGPT_ACCESS_TOKEN | 否 | 空字符串 | ChatGPT 的 access_token，如配置则优先使用 |
 | CHATGPT_MODEL | 否 | 空字符串 | 模型，免费账号只有一个，PLUS账号可使用`gpt-4` |
 | CHATGPT_ACCOUNT | 否 | 空字符串 | ChatGPT 登陆邮箱，未配置则使用 session_token |
 | CHATGPT_PASSWORD | 否 | 空字符串 | ChatGPT 登陆密码，未配置则使用 session_token |
 | CHATGPT_CD_TIME | 否 | 60 | 冷却时间，单位：秒|
 | CHATGPT_NOTICE | 否 | True | 收到请求时进行回复提醒 |
 | CHATGPT_AUTO_REFRESH | 否 | True | 会话不存在时，自动刷新会话 |
 | CHATGPT_PROXIES | 否 | None | 代理地址，格式为： `http://ip:port` |
```

#### html2text {}

```diff
@@ -18,16 +18,18 @@
 é¡¹ç®ç `bot.py` æä»¶, å¨å¶ä¸­åå¥ nonebot.load_plugin
 ('nonebot_plugin_chatgpt_plus')  ## âï¸ éç½® å¨ nonebot2 é¡¹ç®ç `.env`
 æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½®ï¼å¨ **ARM**
 å¹³å°ï¼å¯è½å¿é¡»ä½¿ç¨ `CHATGPT_SESSION_TOKEN` ç»å½ï¼ > â ï¸
 **Windows** ç³»ç»ä¸éè¦å¨ `.env.dev` æä»¶ä¸­è®¾ç½®
 `FASTAPI_RELOAD=false` | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:--
 --:|:----:|:----:| | CHATGPT_SESSION_TOKEN | å¦ | ç©ºå­ç¬¦ä¸² | ChatGPT ç
-session_tokenï¼å¦éç½®åä¼åä½¿ç¨ | | CHATGPT_MODEL | å¦ | ç©ºå­ç¬¦ä¸²
-| æ¨¡åï¼åè´¹è´¦å·åªæä¸ä¸ªï¼PLUSè´¦å·å¯ä½¿ç¨`gpt-4` | |
+session_tokenï¼å¦éç½®åä¼åä½¿ç¨ | | CHATGPT_ACCESS_TOKEN | å¦ |
+ç©ºå­ç¬¦ä¸² | ChatGPT ç access_tokenï¼å¦éç½®åä¼åä½¿ç¨ | |
+CHATGPT_MODEL | å¦ | ç©ºå­ç¬¦ä¸² |
+æ¨¡åï¼åè´¹è´¦å·åªæä¸ä¸ªï¼PLUSè´¦å·å¯ä½¿ç¨`gpt-4` | |
 CHATGPT_ACCOUNT | å¦ | ç©ºå­ç¬¦ä¸² | ChatGPT
 ç»éé®ç®±ï¼æªéç½®åä½¿ç¨ session_token | | CHATGPT_PASSWORD | å¦ |
 ç©ºå­ç¬¦ä¸² | ChatGPT ç»éå¯ç ï¼æªéç½®åä½¿ç¨ session_token | |
 CHATGPT_CD_TIME | å¦ | 60 | å·å´æ¶é´ï¼åä½ï¼ç§| | CHATGPT_NOTICE |
 å¦ | True | æ¶å°è¯·æ±æ¶è¿è¡åå¤æé | | CHATGPT_AUTO_REFRESH | å¦ |
 True | ä¼è¯ä¸å­å¨æ¶ï¼èªå¨å·æ°ä¼è¯ | | CHATGPT_PROXIES | å¦ | None
 | ä»£çå°åï¼æ ¼å¼ä¸ºï¼ `http://ip:port` | | CHATGPT_REFRESH_INTERVAL |
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.5/nonebot_plugin_chatgpt_plus/__init__.py` & `nonebot-plugin-chatgpt-plus-0.8.6/nonebot_plugin_chatgpt_plus/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 查看人格/查询人格 + 名称   查看已有的人格预设（超级用户）
 人格设定/设置人格 + 名称 + 人格信息 编辑人格信息（超级用户）
 刷新token   强制刷新token（超级用户）""",
     extra={
         "unique_name": "chatgpt-plus",
         "example": """@bot 人格设定 香草""",
         "author": "A-kirami",
-        "version": "0.8.1",
+        "version": "0.8.6",
     },
 )
 __plugin_settings__ = {
     "level": 5,
     "default_status": True,
     "limit_superuser": False,
     "cmd": [
@@ -63,14 +63,15 @@
         "gpt3",
         "gpt4",
     ],
 }
 
 chat_bot = Chatbot(
     token=setting.token or config.chatgpt_session_token,
+    access_token=setting.access_token or config.chatgpt_access_token,
     model=config.chatgpt_model,
     account=config.chatgpt_account,
     password=config.chatgpt_password,
     api=config.chatgpt_api,
     proxies=config.chatgpt_proxies,
     presets=setting.presets,
     timeout=config.chatgpt_timeout,
@@ -137,21 +138,21 @@
                 cvst['conversation_id'].append(None)
                 cvst['parent_id'].append(chat_bot.id)
                 await matcher.send("会话不存在，已自动刷新对话，等待响应...", reply_message=True)
                 msg = await chat_bot(**cvst, played_name=played_name).get_chat_response(text)
             else:
                 msg += ",请刷新会话"
     except Exception as e:
-        lockers[event.user_id] = False
         error = f"{type(e).__name__}: {e}"
         logger.opt(exception=e).error(f"ChatGPT request failed: {error}")
         await matcher.finish(
             f"请求 ChatGPT 服务器时出现问题，请稍后再试\n错误信息: {error}", reply_message=True
         )
-    lockers[event.user_id] = False
+    finally:
+        lockers[event.user_id] = False
     if config.chatgpt_image:
         if msg.count("```") % 2 != 0:
             msg += "\n```"
         img = await md_to_pic(msg, width=config.chatgpt_image_width)
         msg = MessageSegment.image(img)
     await matcher.send(msg, reply_message=True)
     session[event] = chat_bot.conversation_id, chat_bot.parent_id
@@ -252,16 +253,18 @@
 
 refresh = on_command("刷新token", block=True, rule=to_me(), permission=SUPERUSER, priority=1)
 
 
 @refresh.handle()
 @scheduler.scheduled_job("interval", minutes=config.chatgpt_refresh_interval)
 async def refresh_session() -> None:
-    await chat_bot.refresh_session()
+    if chat_bot.session_token:
+        await chat_bot.refresh_session()
     setting.token = chat_bot.session_token
+    setting.access_token = chat_bot.authorization
     setting.save()
     session.save_sessions()
     logger.opt(colors=True).debug(
         f"\ntoken: {setting.token}"
     )
 
 clear = on_command("清空对话", aliases={"清空会话"}, block=True, rule=to_me(), permission=SUPERUSER, priority=1)
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.5/nonebot_plugin_chatgpt_plus/chatgpt.py` & `nonebot-plugin-chatgpt-plus-0.8.6/nonebot_plugin_chatgpt_plus/chatgpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 CF_CLEARANCE_KEY = "cf_clearance"
 
 class Chatbot:
     def __init__(
         self,
         *,
         token: str = "",
+        access_token: str = "",
         model: str = "text-davinci-002-render-sha",
         account: str = "",
         password: str = "",
         api: str = "https://chat.openai.com/",
         proxies: Optional[str] = None,
         presets: dict = {},
         timeout: int = 10,
@@ -33,15 +34,15 @@
         self.session_token = token
         self.model = model
         self.account = account
         self.password = password
         self.api_url = api
         self.proxies = proxies
         self.timeout = timeout
-        self.authorization = ""
+        self.authorization = access_token
         self.conversation_id = None
         self.parent_id = None
         self.played_name = None
         self.presets = presets
 
         if self.session_token:
             self.auto_auth = False
@@ -259,18 +260,22 @@
                 response = await client.get(
                     urljoin(self.api_url, "api/auth/session"),
                     headers={
                         "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.1 Safari/605.1.15",
                     },
                 )
             try:
-                self.session_token = (
-                    response.cookies.get(SESSION_TOKEN_KEY) or self.session_token
-                )
-                self.authorization = response.json()["accessToken"]
+                if response.status_code == 200:
+                    self.session_token = (
+                        response.cookies.get(SESSION_TOKEN_KEY) or self.session_token
+                    )
+                    self.authorization = response.json()["accessToken"]
+                else:
+                    resp_json = response.json()
+                    raise Exception(resp_json["detail"])
             except Exception as e:
                 logger.opt(colors=True, exception=e).error(
                     f"刷新会话失败: <r>HTTP{response.status_code}</r> {response.text}"
                 )
 
     async def login(self) -> None:
         async with httpx.AsyncClient(
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.5/nonebot_plugin_chatgpt_plus/config.py` & `nonebot-plugin-chatgpt-plus-0.8.6/nonebot_plugin_chatgpt_plus/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from nonebot import get_driver
 from pydantic import BaseModel, Extra
 
 
 class Config(BaseModel, extra=Extra.ignore):
     chatgpt_session_token: str = ""
+    chatgpt_access_token: str = ""
     chatgpt_model: str = ""
     chatgpt_account: str = ""
     chatgpt_password: str = ""
     chatgpt_cd_time: int = 60
     chatgpt_notice: bool = True
     chatgpt_auto_refresh: bool = True
     chatgpt_proxies: Optional[str] = None
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.5/nonebot_plugin_chatgpt_plus/data.py` & `nonebot-plugin-chatgpt-plus-0.8.6/nonebot_plugin_chatgpt_plus/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     import json
 
 
 class Setting(BaseModel):
     session: Dict[str, Dict[str, Any]] = Field(default_factory=dict)
     presets: Dict[str, str] = Field(default_factory=dict)
     token: str = ""
+    access_token: str = ""
 
     __file_path: Path = config.chatgpt_data / "setting.json"
 
     @property
     def file_path(self) -> Path:
         return self.__class__.__file_path
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.5/nonebot_plugin_chatgpt_plus/utils.py` & `nonebot-plugin-chatgpt-plus-0.8.6/nonebot_plugin_chatgpt_plus/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-plus-0.8.5/pyproject.toml` & `nonebot-plugin-chatgpt-plus-0.8.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-chatgpt-plus"
-version = "0.8.5"
+version = "0.8.6"
 description = "NoneBot2 plugin for AI chat"
 authors = [
     { name = "Akirami", email = "Akiramiaya@outlook.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc2",
     "nonebot-adapter-onebot>=2.1.5",
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.5/PKG-INFO` & `nonebot-plugin-chatgpt-plus-0.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-plus
-Version: 0.8.5
+Version: 0.8.6
 Summary: NoneBot2 plugin for AI chat
 License: MIT
 Author-email: Akirami <Akiramiaya@outlook.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/AkashiCoin/nonebot-plugin-chatgpt-plus
 Project-URL: Repository, https://github.com/AkashiCoin/nonebot-plugin-chatgpt-plus
 Description-Content-Type: text/markdown
@@ -87,14 +87,15 @@
 在 nonebot2 项目的 `.env` 文件中添加下表中的必填配置（在 **ARM** 平台，可能必须使用 `CHATGPT_SESSION_TOKEN` 登录）
 
 > ⚠️ **Windows** 系统下需要在 `.env.dev` 文件中设置 `FASTAPI_RELOAD=false`
 
 | 配置项 | 必填 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
 | CHATGPT_SESSION_TOKEN | 否 | 空字符串 | ChatGPT 的 session_token，如配置则优先使用 |
+| CHATGPT_ACCESS_TOKEN | 否 | 空字符串 | ChatGPT 的 access_token，如配置则优先使用 |
 | CHATGPT_MODEL | 否 | 空字符串 | 模型，免费账号只有一个，PLUS账号可使用`gpt-4` |
 | CHATGPT_ACCOUNT | 否 | 空字符串 | ChatGPT 登陆邮箱，未配置则使用 session_token |
 | CHATGPT_PASSWORD | 否 | 空字符串 | ChatGPT 登陆密码，未配置则使用 session_token |
 | CHATGPT_CD_TIME | 否 | 60 | 冷却时间，单位：秒|
 | CHATGPT_NOTICE | 否 | True | 收到请求时进行回复提醒 |
 | CHATGPT_AUTO_REFRESH | 否 | True | 会话不存在时，自动刷新会话 |
 | CHATGPT_PROXIES | 否 | None | 代理地址，格式为： `http://ip:port` |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-chatgpt-plus Version: 0.8.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-chatgpt-plus Version: 0.8.6 Summary:
 NoneBot2 plugin for AI chat License: MIT Author-email: Akirami
 outlook.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 AkashiCoin/nonebot-plugin-chatgpt-plus Project-URL: Repository, https://
 github.com/AkashiCoin/nonebot-plugin-chatgpt-plus Description-Content-Type:
 text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
@@ -24,16 +24,18 @@
 é¡¹ç®ç `bot.py` æä»¶, å¨å¶ä¸­åå¥ nonebot.load_plugin
 ('nonebot_plugin_chatgpt_plus')  ## âï¸ éç½® å¨ nonebot2 é¡¹ç®ç `.env`
 æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½®ï¼å¨ **ARM**
 å¹³å°ï¼å¯è½å¿é¡»ä½¿ç¨ `CHATGPT_SESSION_TOKEN` ç»å½ï¼ > â ï¸
 **Windows** ç³»ç»ä¸éè¦å¨ `.env.dev` æä»¶ä¸­è®¾ç½®
 `FASTAPI_RELOAD=false` | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:--
 --:|:----:|:----:| | CHATGPT_SESSION_TOKEN | å¦ | ç©ºå­ç¬¦ä¸² | ChatGPT ç
-session_tokenï¼å¦éç½®åä¼åä½¿ç¨ | | CHATGPT_MODEL | å¦ | ç©ºå­ç¬¦ä¸²
-| æ¨¡åï¼åè´¹è´¦å·åªæä¸ä¸ªï¼PLUSè´¦å·å¯ä½¿ç¨`gpt-4` | |
+session_tokenï¼å¦éç½®åä¼åä½¿ç¨ | | CHATGPT_ACCESS_TOKEN | å¦ |
+ç©ºå­ç¬¦ä¸² | ChatGPT ç access_tokenï¼å¦éç½®åä¼åä½¿ç¨ | |
+CHATGPT_MODEL | å¦ | ç©ºå­ç¬¦ä¸² |
+æ¨¡åï¼åè´¹è´¦å·åªæä¸ä¸ªï¼PLUSè´¦å·å¯ä½¿ç¨`gpt-4` | |
 CHATGPT_ACCOUNT | å¦ | ç©ºå­ç¬¦ä¸² | ChatGPT
 ç»éé®ç®±ï¼æªéç½®åä½¿ç¨ session_token | | CHATGPT_PASSWORD | å¦ |
 ç©ºå­ç¬¦ä¸² | ChatGPT ç»éå¯ç ï¼æªéç½®åä½¿ç¨ session_token | |
 CHATGPT_CD_TIME | å¦ | 60 | å·å´æ¶é´ï¼åä½ï¼ç§| | CHATGPT_NOTICE |
 å¦ | True | æ¶å°è¯·æ±æ¶è¿è¡åå¤æé | | CHATGPT_AUTO_REFRESH | å¦ |
 True | ä¼è¯ä¸å­å¨æ¶ï¼èªå¨å·æ°ä¼è¯ | | CHATGPT_PROXIES | å¦ | None
 | ä»£çå°åï¼æ ¼å¼ä¸ºï¼ `http://ip:port` | | CHATGPT_REFRESH_INTERVAL |
```

