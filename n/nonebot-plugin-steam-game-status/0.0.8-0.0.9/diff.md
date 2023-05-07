# Comparing `tmp/nonebot_plugin_steam_game_status-0.0.8.tar.gz` & `tmp/nonebot_plugin_steam_game_status-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_steam_game_status-0.0.8.tar", last modified: Sun Apr 23 03:41:50 2023, max compression
+gzip compressed data, was "nonebot_plugin_steam_game_status-0.0.9.tar", last modified: Sun May  7 07:53:33 2023, max compression
```

## Comparing `nonebot_plugin_steam_game_status-0.0.8.tar` & `nonebot_plugin_steam_game_status-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 03:41:50.274453 nonebot_plugin_steam_game_status-0.0.8/
--rw-rw-rw-   0        0        0    35823 2023-04-03 08:15:10.000000 nonebot_plugin_steam_game_status-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1927 2023-04-23 03:41:50.274453 nonebot_plugin_steam_game_status-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1498 2023-04-23 03:41:17.000000 nonebot_plugin_steam_game_status-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 03:41:50.268453 nonebot_plugin_steam_game_status-0.0.8/nonebot_plugin_steam_game_status/
--rw-rw-rw-   0        0        0    11023 2023-04-23 03:37:54.000000 nonebot_plugin_steam_game_status-0.0.8/nonebot_plugin_steam_game_status/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 03:41:50.272452 nonebot_plugin_steam_game_status-0.0.8/nonebot_plugin_steam_game_status.egg-info/
--rw-rw-rw-   0        0        0     1927 2023-04-23 03:41:50.000000 nonebot_plugin_steam_game_status-0.0.8/nonebot_plugin_steam_game_status.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2023-04-23 03:41:50.000000 nonebot_plugin_steam_game_status-0.0.8/nonebot_plugin_steam_game_status.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 03:41:50.000000 nonebot_plugin_steam_game_status-0.0.8/nonebot_plugin_steam_game_status.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-23 03:41:50.000000 nonebot_plugin_steam_game_status-0.0.8/nonebot_plugin_steam_game_status.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2023-04-23 03:41:50.000000 nonebot_plugin_steam_game_status-0.0.8/nonebot_plugin_steam_game_status.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 03:41:50.275452 nonebot_plugin_steam_game_status-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      868 2023-04-23 03:38:42.000000 nonebot_plugin_steam_game_status-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 07:53:33.353895 nonebot_plugin_steam_game_status-0.0.9/
+-rw-rw-rw-   0        0        0    35823 2023-04-03 08:15:10.000000 nonebot_plugin_steam_game_status-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     2388 2023-05-07 07:53:33.352895 nonebot_plugin_steam_game_status-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1961 2023-05-07 07:51:21.000000 nonebot_plugin_steam_game_status-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 07:53:33.348894 nonebot_plugin_steam_game_status-0.0.9/nonebot_plugin_steam_game_status/
+-rw-rw-rw-   0        0        0    11227 2023-05-07 07:44:34.000000 nonebot_plugin_steam_game_status-0.0.9/nonebot_plugin_steam_game_status/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 07:53:33.351894 nonebot_plugin_steam_game_status-0.0.9/nonebot_plugin_steam_game_status.egg-info/
+-rw-rw-rw-   0        0        0     2388 2023-05-07 07:53:33.000000 nonebot_plugin_steam_game_status-0.0.9/nonebot_plugin_steam_game_status.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-05-07 07:53:33.000000 nonebot_plugin_steam_game_status-0.0.9/nonebot_plugin_steam_game_status.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 07:53:33.000000 nonebot_plugin_steam_game_status-0.0.9/nonebot_plugin_steam_game_status.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-05-07 07:53:33.000000 nonebot_plugin_steam_game_status-0.0.9/nonebot_plugin_steam_game_status.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2023-05-07 07:53:33.000000 nonebot_plugin_steam_game_status-0.0.9/nonebot_plugin_steam_game_status.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 07:53:33.353895 nonebot_plugin_steam_game_status-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      868 2023-05-07 07:52:51.000000 nonebot_plugin_steam_game_status-0.0.9/setup.py
```

### Comparing `nonebot_plugin_steam_game_status-0.0.8/LICENSE` & `nonebot_plugin_steam_game_status-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_game_status-0.0.8/PKG-INFO` & `nonebot_plugin_steam_game_status-0.0.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,39 @@
-Metadata-Version: 2.1
-Name: nonebot_plugin_steam_game_status
-Version: 0.0.8
-Summary: 在群内播报steam游戏状态的Nonebot插件
-Home-page: https://github.com/nek0us/nonebot_plugin_steam_game_status
-Author: nek0us
-Author-email: nekouss@gmail.com
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![PyPi](https://img.shields.io/pypi/v/nonebot_plugin_steam_game_status.svg)](https://pypi.python.org/pypi/nonebot_plugin_steam_game_status)
 
 # nonebot_plugin_steam_game_status
 在群内播报steam游戏状态的Nonebot插件
 ==========
 
 ## 安装
 
 ```bash
+# 使用pip安装，记得手动添加插件名到配置文件
 pip install nonebot_plugin_steam_game_status
+
+# 使用nb-cli安装
+nb plugin install nonebot_plugin_steam_game_status
+
+# 更新至最新版 
+pip install nonebot_plugin_steam_game_status --upgrade
 ```
 
 ## 配置
 ### 获取steam_web_api_key
 
-获取steam_web_key[steam_web_key](https://steamcommunity.com/dev/apikey)
+获取[steam_web_key](https://steamcommunity.com/dev/apikey)
 
 配置文件内填写：
 ```bash
 steam_web_key="your key"
 ```
 ### 获取Steam ID
 
-    打开 Steam 客户端，点击<商店> <库> <社区> 右侧的个人昵称，
-    在打开的页面中，右键 -> 复制网页URL，
-    任意找个地方粘贴，“profiles” 后两个 “/” 之间的数字即为个人 ID，
+    Steam 桌面网站或桌面客户端：点开右上角昵称下拉菜单，点击账户明细，即可看到Steam ID
+    Steam 应用：点击右上角头像，点击账户明细，即可看到Steam ID
 
 ## 指令表
 
 | 指令 | 需要@ | 范围 | 权限 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | steam绑定/添加/.add | 否 | 群聊 | 群员 | 后加个人Steam ID |    
 | steam解绑/删除/.del | 否 | 群聊 | 群员 | 后加个人Steam ID |   
@@ -47,12 +41,27 @@
 | steam播报开启/播报打开 | 否 | 群聊 | 超管/群管 | 管理员命令 |    
 | steam播报关闭/播报停止 | 否 | 群聊 | 超管/群管 | 管理员命令 |    
 
 ## 创意来源
 
 群友的koishi bot的该效果插件
 
+## 注意事项
+
+1.也许不支持播报Linux Steam客户端游戏
+
+2.不支持播报Steam隐身状态下进行的游戏
+
 ## 更新记录
 
+2023.05.07
+
+1.优化了日志输出，和部分代码
+
+2.感谢 [050644zf](https://github.com/050644zf) 提供了更适合的steam id获取方式
+
+
 2023.04.23
+
 1.优化了监控代码，解决请求阻塞过久的问题
+
 2.解决消息在多账号下无法发送的问题
```

### Comparing `nonebot_plugin_steam_game_status-0.0.8/nonebot_plugin_steam_game_status/__init__.py` & `nonebot_plugin_steam_game_status-0.0.9/nonebot_plugin_steam_game_status/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN,GROUP_OWNER
 from nonebot.adapters.onebot.v11 import Message,MessageEvent,Bot,GroupMessageEvent
 from nonebot.matcher import Matcher
 from nonebot.params import CommandArg
 from nonebot.log import logger
 import nonebot
 from nonebot.adapters.onebot.v11.adapter import Adapter
+from nonebot.exception import MatcherException
 from pathlib import Path
 import json
 import time
 from httpx import AsyncClient
 import asyncio
 
 
@@ -94,16 +95,16 @@
                     except:
                         pass
                 group_list[group_num][id] = user_info
                 dirpath.write_text(json.dumps(group_list))
             elif "gameextrainfo" not in res_info and group_list[group_num][id][1] == "":
                 # 一直没玩
                 pass
-        except:
-            pass
+        except Exception as e:
+            logger.debug(f"steam id:{id} 查询状态失败，{e}")
     
     
     
 @scheduler.scheduled_job("interval",minutes=1,id="steam",misfire_grace_time=59)
 async def now_steam():
     task_list = []
     group_list = json.loads(dirpath.read_text("utf8"))
@@ -117,64 +118,59 @@
                     
                     
 steam_bind = on_command("steam绑定",aliases={"steam.add","steam添加"},priority=5)
 @steam_bind.handle()
 async def steam_bind_handle(bot: Bot,event: MessageEvent,matcher: Matcher,arg: Message = CommandArg()):
     if isinstance(event,GroupMessageEvent):
         if not steam_web_key:
-            await steam_bind.finish("steam_web_key 未配置") 
+            await matcher.finish("steam_web_key 未配置") 
         if len(arg.extract_plain_text()) != 17:
-            await steam_bind.finish("steam id格式错误") 
+            await matcher.finish("steam id格式错误") 
         steam_name: str = ""
         try:
             async with AsyncClient() as client:
                 url = "https://api.steampowered.com/ISteamUser/GetPlayerSummaries/v0002/?key=" + steam_web_key + "&steamids=" + arg.extract_plain_text()
                 res = await client.get(url,headers=header,timeout=30)
-                if res.status_code != 200:
-                    await steam_bind.finish(arg + " 绑定失败") 
-                steam_name = json.loads(res.text)["response"]["players"][0]['personaname']
-        except:
-            await steam_bind.finish(arg + " 绑定失败")
+            if res.status_code != 200:
+                logger.debug(f"{arg.extract_plain_text()} 绑定失败，{res.status_code} {res.text}")
+                await matcher.finish(f"{arg.extract_plain_text()} 绑定失败，{res.status_code} {res.text}") 
+            if json.loads(res.text)["response"]["players"] == []:
+                logger.debug(f"{arg.extract_plain_text()} 绑定失败，查无此人，请检查输入的id")
+                await matcher.finish(f"{arg.extract_plain_text()} 绑定失败，查无此人，请检查输入的id") 
+            steam_name = json.loads(res.text)["response"]["players"][0]['personaname']
+        except MatcherException:
+            raise
+        except Exception as e:
+            logger.debug(f"{arg.extract_plain_text()} 绑定失败，{e}")
+            await matcher.finish(f"{arg.extract_plain_text()} 绑定失败，{e}")
         
         group_list = json.loads(dirpath.read_text("utf8"))
         if str(event.group_id) not in group_list:
             group_list[str(event.group_id)] = {"status":"on"}
         group_list[str(event.group_id)][arg.extract_plain_text()] = [0,"",steam_name]
         dirpath.write_text(json.dumps(group_list))
-        await steam_bind.finish(f"Steam ID：{arg}\nSteam Name：{steam_name}\n 绑定成功了")
+        await matcher.finish(f"Steam ID：{arg.extract_plain_text()}\nSteam Name：{steam_name}\n 绑定成功了")
                             
 steam_del = on_command("steam删除",aliases={"steam.del","steam解绑"},priority=5)
 @steam_del.handle()
 async def steam_del_handle(bot: Bot,event: MessageEvent,matcher: Matcher,arg: Message = CommandArg()):
     if isinstance(event,GroupMessageEvent):
-        if not steam_web_key:
-            await steam_bind.finish("steam_web_key 未配置") 
         if len(arg.extract_plain_text()) != 17:
-            await steam_bind.finish("steam id格式错误") 
+            await steam_del.finish("steam id格式错误") 
         steam_name: str = ""
-        try:
-            async with AsyncClient() as client:
-                url = "https://api.steampowered.com/ISteamUser/GetPlayerSummaries/v0002/?key=" + steam_web_key + "&steamids=" + arg.extract_plain_text()
-                res = await client.get(url,headers=header,timeout=30)
-                if res.status_code != 200:
-                    await steam_bind.finish(arg + " 解绑失败") 
-                steam_name = json.loads(res.text)["response"]["players"][0]['personaname']
-        except:
-            await steam_bind.finish(arg + " 解绑失败")
-        
-        
         group_list = json.loads(dirpath.read_text("utf8"))
         if str(event.group_id) not in group_list:
             group_list[str(event.group_id)] = {}
         try:
+            steam_name = group_list[str(event.group_id)][arg.extract_plain_text()][2]
             group_list[str(event.group_id)].pop(arg.extract_plain_text()) 
         except:
-            await steam_bind.finish(f"没有找到Steam ID：{arg}")
+            await steam_del.finish(f"没有找到Steam ID：{arg.extract_plain_text()}")
         dirpath.write_text(json.dumps(group_list))
-        await steam_bind.finish(f"Steam ID：{arg}\nSteam Name：{steam_name}\n 删除成功了")
+        await steam_del.finish(f"Steam ID：{arg.extract_plain_text()}\nSteam Name：{steam_name}\n 删除成功了")
             
         
         
         
 steam_bind_list = on_command("steam列表",aliases={"steam绑定列表","steam播报列表"},priority=5,permission=SUPERUSER|GROUP_ADMIN|GROUP_OWNER)
 @steam_bind_list.handle()
 async def steam_bind_list_handle(bot: Bot,event: MessageEvent,matcher: Matcher):
@@ -184,44 +180,44 @@
             msg = []
             for id in id_list:
                 if "status" not in id:
                     msg += await node_msg(event.user_id,f"id：{id}\nname：{id_list[id][2]}")
                     
             await bot.send_group_forward_msg(group_id=event.group_id,messages=msg)
         except:
-            await steam_bind.finish(f"本群未绑定ID，请先绑定。")
+            await steam_bind_list.finish(f"本群未绑定任何steam ID，请先绑定。")
         
     
 
 steam_on = on_command("steam播报开启",aliases={"steam播报打开"},priority=5,permission=SUPERUSER|GROUP_ADMIN|GROUP_OWNER)
 @steam_on.handle()
 async def steam_on_handle(bot: Bot,event: MessageEvent,matcher: Matcher):
     if isinstance(event,GroupMessageEvent):
         group_list = json.loads(dirpath.read_text("utf8"))
         if str(event.group_id) not in group_list:
             group_list[str(event.group_id)] = {}
         group_list[str(event.group_id)]["status"] = "on"
         f = open(dirpath.__str__(),"w")
         f.write(json.dumps(group_list))
         f.close()
-        await steam_on.finish("播报开启了")
+        await steam_on.finish("steam播报开启了")
 
 steam_off = on_command("steam播报关闭",aliases={"steam播报停止"},priority=5,permission=SUPERUSER|GROUP_ADMIN|GROUP_OWNER)
 @steam_off.handle()
 async def steam_off_handle(bot: Bot,event: MessageEvent,matcher: Matcher):
     if isinstance(event,GroupMessageEvent):
         f = open(dirpath.__str__(),"r+")
         group_list = f.read()
         f.close()
         group_list = json.loads(group_list)
         if str(event.group_id) not in group_list:
             group_list[str(event.group_id)] = {}
         group_list[str(event.group_id)]["status"] = "off"
         dirpath.write_text(json.dumps(group_list))
-        await steam_on.finish("播报关闭了")
+        await steam_off.finish("steam播报关闭了")
         
 async def node_msg(user_id,plain_text):
     if not plain_text:
         plain_text = "无"
     node = [
 	{
 		"type": "node",
```

### Comparing `nonebot_plugin_steam_game_status-0.0.8/nonebot_plugin_steam_game_status.egg-info/PKG-INFO` & `nonebot_plugin_steam_game_status-0.0.9/nonebot_plugin_steam_game_status.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-steam-game-status
-Version: 0.0.8
+Version: 0.0.9
 Summary: 在群内播报steam游戏状态的Nonebot插件
 Home-page: https://github.com/nek0us/nonebot_plugin_steam_game_status
 Author: nek0us
 Author-email: nekouss@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -15,31 +15,37 @@
 # nonebot_plugin_steam_game_status
 在群内播报steam游戏状态的Nonebot插件
 ==========
 
 ## 安装
 
 ```bash
+# 使用pip安装，记得手动添加插件名到配置文件
 pip install nonebot_plugin_steam_game_status
+
+# 使用nb-cli安装
+nb plugin install nonebot_plugin_steam_game_status
+
+# 更新至最新版 
+pip install nonebot_plugin_steam_game_status --upgrade
 ```
 
 ## 配置
 ### 获取steam_web_api_key
 
-获取steam_web_key[steam_web_key](https://steamcommunity.com/dev/apikey)
+获取[steam_web_key](https://steamcommunity.com/dev/apikey)
 
 配置文件内填写：
 ```bash
 steam_web_key="your key"
 ```
 ### 获取Steam ID
 
-    打开 Steam 客户端，点击<商店> <库> <社区> 右侧的个人昵称，
-    在打开的页面中，右键 -> 复制网页URL，
-    任意找个地方粘贴，“profiles” 后两个 “/” 之间的数字即为个人 ID，
+    Steam 桌面网站或桌面客户端：点开右上角昵称下拉菜单，点击账户明细，即可看到Steam ID
+    Steam 应用：点击右上角头像，点击账户明细，即可看到Steam ID
 
 ## 指令表
 
 | 指令 | 需要@ | 范围 | 权限 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | steam绑定/添加/.add | 否 | 群聊 | 群员 | 后加个人Steam ID |    
 | steam解绑/删除/.del | 否 | 群聊 | 群员 | 后加个人Steam ID |   
@@ -47,12 +53,27 @@
 | steam播报开启/播报打开 | 否 | 群聊 | 超管/群管 | 管理员命令 |    
 | steam播报关闭/播报停止 | 否 | 群聊 | 超管/群管 | 管理员命令 |    
 
 ## 创意来源
 
 群友的koishi bot的该效果插件
 
+## 注意事项
+
+1.也许不支持播报Linux Steam客户端游戏
+
+2.不支持播报Steam隐身状态下进行的游戏
+
 ## 更新记录
 
+2023.05.07
+
+1.优化了日志输出，和部分代码
+
+2.感谢 [050644zf](https://github.com/050644zf) 提供了更适合的steam id获取方式
+
+
 2023.04.23
+
 1.优化了监控代码，解决请求阻塞过久的问题
+
 2.解决消息在多账号下无法发送的问题
```

### Comparing `nonebot_plugin_steam_game_status-0.0.8/setup.py` & `nonebot_plugin_steam_game_status-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r",encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 requirements = ["nonebot2","nonebot-adapter-onebot","nonebot-plugin-apscheduler","httpx"] # 这里填依赖包信息
 
 setup(
     name="nonebot_plugin_steam_game_status",
-    version="0.0.8",
+    version="0.0.9",
     author="nek0us",
     author_email="nekouss@gmail.com",
     description="在群内播报steam游戏状态的Nonebot插件",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/nek0us/nonebot_plugin_steam_game_status",
     packages=find_packages(),
```

