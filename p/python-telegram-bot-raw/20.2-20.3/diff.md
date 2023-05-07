# Comparing `tmp/python-telegram-bot-raw-20.2.tar.gz` & `tmp/python-telegram-bot-raw-20.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-telegram-bot-raw-20.2.tar", last modified: Sat Mar 25 12:33:01 2023, max compression
+gzip compressed data, was "python-telegram-bot-raw-20.3.tar", last modified: Sun May  7 13:32:51 2023, max compression
```

## Comparing `python-telegram-bot-raw-20.2.tar` & `python-telegram-bot-raw-20.3.tar`

### file list

```diff
@@ -1,214 +1,166 @@
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-03-25 12:33:01.827075 python-telegram-bot-raw-20.2/
--rw-r--r--   0 hinrich   (1000) hinrich   (1000)    32422 2020-03-22 11:54:25.000000 python-telegram-bot-raw-20.2/LICENSE
--rw-r--r--   0 hinrich   (1000) hinrich   (1000)    40192 2020-03-22 11:54:25.000000 python-telegram-bot-raw-20.2/LICENSE.dual
--rw-r--r--   0 hinrich   (1000) hinrich   (1000)     7651 2020-03-22 11:54:25.000000 python-telegram-bot-raw-20.2/LICENSE.lesser
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      103 2022-12-15 14:38:37.000000 python-telegram-bot-raw-20.2/MANIFEST.in
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12734 2023-03-25 12:33:01.827075 python-telegram-bot-raw-20.2/PKG-INFO
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12912 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/README.rst
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    11048 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/README_RAW.rst
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      209 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/pyproject.toml
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-03-25 12:33:01.723023 python-telegram-bot-raw-20.2/python_telegram_bot_raw.egg-info/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12734 2023-03-25 12:33:01.000000 python-telegram-bot-raw-20.2/python_telegram_bot_raw.egg-info/PKG-INFO
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6064 2023-03-25 12:33:01.000000 python-telegram-bot-raw-20.2/python_telegram_bot_raw.egg-info/SOURCES.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        1 2023-03-25 12:33:01.000000 python-telegram-bot-raw-20.2/python_telegram_bot_raw.egg-info/dependency_links.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      205 2023-03-25 12:33:01.000000 python-telegram-bot-raw-20.2/python_telegram_bot_raw.egg-info/requires.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        9 2023-03-25 12:33:01.000000 python-telegram-bot-raw-20.2/python_telegram_bot_raw.egg-info/top_level.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1005 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/requirements-opts.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      373 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/requirements.txt
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      199 2022-12-15 14:38:38.000000 python-telegram-bot-raw-20.2/setup-raw.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1841 2023-03-25 12:33:01.831077 python-telegram-bot-raw-20.2/setup.cfg
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4701 2022-12-15 14:38:38.000000 python-telegram-bot-raw-20.2/setup.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-03-25 12:33:01.751037 python-telegram-bot-raw-20.2/telegram/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    13025 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/telegram/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1880 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/__main__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   342189 2023-03-25 12:16:21.000000 python-telegram-bot-raw-20.2/telegram/_bot.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3268 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_botcommand.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10225 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_botcommandscope.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2452 2023-03-25 12:16:22.000000 python-telegram-bot-raw-20.2/telegram/_botdescription.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    29315 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_callbackquery.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   115940 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/telegram/_chat.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8854 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_chatadministratorrights.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6388 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_chatinvitelink.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8029 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_chatjoinrequest.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3295 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_chatlocation.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    24240 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_chatmember.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7099 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_chatmemberupdated.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    11291 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_chatpermissions.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4244 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_choseninlineresult.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7002 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_dice.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-03-25 12:33:01.755039 python-telegram-bot-raw-20.2/telegram/_files/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2022-12-15 14:38:38.000000 python-telegram-bot-raw-20.2/telegram/_files/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3506 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_files/_basemedium.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4834 2023-03-25 12:16:21.000000 python-telegram-bot-raw-20.2/telegram/_files/_basethumbedmedium.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4419 2023-03-25 12:16:22.000000 python-telegram-bot-raw-20.2/telegram/_files/animation.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4656 2023-03-25 12:16:20.000000 python-telegram-bot-raw-20.2/telegram/_files/audio.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7065 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_files/chatphoto.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2680 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_files/contact.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3698 2023-03-25 12:16:22.000000 python-telegram-bot-raw-20.2/telegram/_files/document.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    14404 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_files/file.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4208 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_files/inputfile.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    29640 2023-03-25 12:16:21.000000 python-telegram-bot-raw-20.2/telegram/_files/inputmedia.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4407 2023-03-25 12:16:21.000000 python-telegram-bot-raw-20.2/telegram/_files/inputsticker.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4724 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_files/location.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2777 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_files/photosize.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    17115 2023-03-25 12:16:21.000000 python-telegram-bot-raw-20.2/telegram/_files/sticker.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4416 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_files/venue.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4236 2023-03-25 12:16:21.000000 python-telegram-bot-raw-20.2/telegram/_files/video.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3629 2023-03-25 12:16:22.000000 python-telegram-bot-raw-20.2/telegram/_files/videonote.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3001 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_files/voice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4329 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_forcereply.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6855 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_forumtopic.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-03-25 12:33:01.759041 python-telegram-bot-raw-20.2/telegram/_games/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2022-12-15 14:38:38.000000 python-telegram-bot-raw-20.2/telegram/_games/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1270 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_games/callbackgame.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8251 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_games/game.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2494 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_games/gamehighscore.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-03-25 12:33:01.767045 python-telegram-bot-raw-20.2/telegram/_inline/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2022-12-15 14:38:38.000000 python-telegram-bot-raw-20.2/telegram/_inline/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12814 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinekeyboardbutton.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5591 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinekeyboardmarkup.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9189 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinequery.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2770 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresult.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7967 2023-03-25 12:16:21.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultarticle.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5625 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultaudio.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5088 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultcachedaudio.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5606 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultcacheddocument.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5363 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultcachedgif.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5454 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultcachedmpeg4gif.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5609 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultcachedphoto.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3629 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultcachedsticker.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5526 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultcachedvideo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5301 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultcachedvoice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8252 2023-03-25 12:16:22.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultcontact.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9875 2023-03-25 12:16:20.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultdocument.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2715 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultgame.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10543 2023-03-25 12:16:21.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultgif.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12054 2023-03-25 12:16:22.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultlocation.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10114 2023-03-25 12:16:21.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultmpeg4gif.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8583 2023-03-25 12:16:20.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultphoto.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9874 2023-03-25 12:16:22.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultvenue.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10492 2023-03-25 12:16:21.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultvideo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5527 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultvoice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2716 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_inline/inputcontactmessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12680 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_inline/inputinvoicemessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6528 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_inline/inputlocationmessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1528 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_inline/inputmessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3691 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_inline/inputtextmessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4511 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_inline/inputvenuemessagecontent.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9173 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_keyboardbutton.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2417 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_keyboardbuttonpolltype.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9333 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/telegram/_keyboardbuttonrequest.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5096 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_loginurl.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6762 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_menubutton.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   159062 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/telegram/_message.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1976 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_messageautodeletetimerchanged.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8171 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_messageentity.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1665 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_messageid.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-03-25 12:33:01.771047 python-telegram-bot-raw-20.2/telegram/_passport/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2022-12-15 14:38:38.000000 python-telegram-bot-raw-20.2/telegram/_passport/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    22561 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_passport/credentials.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6303 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_passport/data.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12481 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_passport/encryptedpassportelement.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5161 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_passport/passportdata.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    16944 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_passport/passportelementerrors.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6186 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_passport/passportfile.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-03-25 12:33:01.775049 python-telegram-bot-raw-20.2/telegram/_payment/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2022-12-15 14:38:38.000000 python-telegram-bot-raw-20.2/telegram/_payment/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5016 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_payment/invoice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2664 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_payment/labeledprice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3044 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_payment/orderinfo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5918 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_payment/precheckoutquery.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2938 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_payment/shippingaddress.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2524 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_payment/shippingoption.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4493 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_payment/shippingquery.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4909 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_payment/successfulpayment.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    16122 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_poll.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2813 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_proximityalerttriggered.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    16268 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_replykeyboardmarkup.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3198 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_replykeyboardremove.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2165 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_sentwebappmessage.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4286 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_shared.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    25541 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_telegramobject.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    19416 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_update.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    60726 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/telegram/_user.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2897 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_userprofilephotos.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-03-25 12:33:01.779051 python-telegram-bot-raw-20.2/telegram/_utils/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2022-12-15 14:38:39.000000 python-telegram-bot-raw-20.2/telegram/_utils/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1520 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_utils/argumentparsing.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8394 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_utils/datetime.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4060 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_utils/defaultvalue.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2662 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_utils/enum.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5735 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_utils/files.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2100 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_utils/markup.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3244 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_utils/types.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2010 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_utils/warnings.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3565 2023-03-25 12:16:21.000000 python-telegram-bot-raw-20.2/telegram/_utils/warnings_transition.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2148 2023-03-25 12:16:17.000000 python-telegram-bot-raw-20.2/telegram/_version.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5656 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_videochat.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2405 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_webappdata.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2083 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_webappinfo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7015 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_webhookinfo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1386 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/_writeaccessallowed.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    66656 2023-03-25 12:16:22.000000 python-telegram-bot-raw-20.2/telegram/constants.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5954 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/error.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6729 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/helpers.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2020-11-25 21:05:21.000000 python-telegram-bot-raw-20.2/telegram/py.typed
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-03-25 12:33:01.779051 python-telegram-bot-raw-20.2/telegram/request/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1081 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/request/__init__.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    17975 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/request/_baserequest.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10307 2023-03-25 12:16:22.000000 python-telegram-bot-raw-20.2/telegram/request/_httpxrequest.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5155 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/telegram/request/_requestdata.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7395 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/telegram/request/_requestparameter.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1900 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/telegram/warnings.py
-drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-03-25 12:33:01.827075 python-telegram-bot-raw-20.2/tests/
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   137402 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_bot.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2550 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_botcommand.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7035 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_botcommandscope.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3252 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_botdescription.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    19396 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_callbackquery.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    58090 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_chat.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5600 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_chatadministratorrights.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6149 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_chatinvitelink.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6989 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_chatjoinrequest.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2679 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_chatlocation.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9334 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_chatmember.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9903 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_chatmemberupdated.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8838 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_chatpermissions.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3739 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_choseninlineresult.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5692 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_constants.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2334 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_dice.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7565 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_error.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2781 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_forcereply.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    18270 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_forum.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6235 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/tests/test_helpers.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5804 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_keyboardbutton.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2075 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_keyboardbuttonpolltype.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6629 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_keyboardbuttonrequest.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2607 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_loginurl.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5841 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_menubutton.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    77036 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_message.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2276 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_messageautodeletetimerchanged.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3503 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_messageentity.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2142 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_messageid.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1400 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_meta.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2423 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/tests/test_modules.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12438 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_official.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10418 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_poll.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3736 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_pollhandler.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3776 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_proximityalerttriggered.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6980 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_replykeyboardmarkup.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2368 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_replykeyboardremove.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2419 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_sentwebappmessage.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4115 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_shared.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2414 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/tests/test_slots.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    19315 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_telegramobject.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7151 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_update.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    26275 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_user.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2879 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_userprofilephotos.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3368 2023-02-09 18:35:26.000000 python-telegram-bot-raw-20.2/tests/test_version.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6820 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_videochat.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3371 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_warnings.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2466 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_webappdata.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2177 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_webappinfo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6017 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_webhookinfo.py
--rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1519 2023-03-25 12:08:03.000000 python-telegram-bot-raw-20.2/tests/test_writeaccessallowed.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-05-07 13:32:51.101768 python-telegram-bot-raw-20.3/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    32422 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/LICENSE
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    40192 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/LICENSE.dual
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7651 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/LICENSE.lesser
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      103 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/MANIFEST.in
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12744 2023-05-07 13:32:51.101768 python-telegram-bot-raw-20.3/PKG-INFO
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12922 2023-05-07 12:56:49.000000 python-telegram-bot-raw-20.3/README.rst
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    11058 2023-05-07 12:56:49.000000 python-telegram-bot-raw-20.3/README_RAW.rst
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      464 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/pyproject.toml
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-05-07 13:32:51.081768 python-telegram-bot-raw-20.3/python_telegram_bot_raw.egg-info/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12744 2023-05-07 13:32:50.000000 python-telegram-bot-raw-20.3/python_telegram_bot_raw.egg-info/PKG-INFO
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4840 2023-05-07 13:32:51.000000 python-telegram-bot-raw-20.3/python_telegram_bot_raw.egg-info/SOURCES.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        1 2023-05-07 13:32:50.000000 python-telegram-bot-raw-20.3/python_telegram_bot_raw.egg-info/dependency_links.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      205 2023-05-07 13:32:50.000000 python-telegram-bot-raw-20.3/python_telegram_bot_raw.egg-info/requires.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        9 2023-05-07 13:32:50.000000 python-telegram-bot-raw-20.3/python_telegram_bot_raw.egg-info/top_level.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1005 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/requirements-opts.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      373 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/requirements.txt
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)      199 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/setup-raw.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1841 2023-05-07 13:32:51.101768 python-telegram-bot-raw-20.3/setup.cfg
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4701 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/setup.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-05-07 13:32:51.089768 python-telegram-bot-raw-20.3/telegram/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    13278 2023-05-07 12:56:49.000000 python-telegram-bot-raw-20.3/telegram/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1880 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/__main__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   346047 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_bot.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3268 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_botcommand.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10225 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_botcommandscope.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2462 2023-05-07 12:56:49.000000 python-telegram-bot-raw-20.3/telegram/_botdescription.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1791 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_botname.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    29315 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_callbackquery.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   115940 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_chat.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8854 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_chatadministratorrights.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6714 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_chatinvitelink.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8353 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_chatjoinrequest.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3295 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_chatlocation.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    24730 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_chatmember.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7961 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_chatmemberupdated.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    11291 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_chatpermissions.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4244 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_choseninlineresult.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7002 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_dice.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-05-07 13:32:51.093768 python-telegram-bot-raw-20.3/telegram/_files/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3506 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/_basemedium.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4834 2023-05-07 12:56:49.000000 python-telegram-bot-raw-20.3/telegram/_files/_basethumbedmedium.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4419 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/animation.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4656 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/audio.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7065 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/chatphoto.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2680 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/contact.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3698 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/document.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    14404 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/file.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4156 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/inputfile.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    29640 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/inputmedia.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4407 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/inputsticker.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4724 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/location.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2777 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/photosize.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    17115 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/sticker.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4416 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/venue.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4236 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/video.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3629 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/videonote.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3001 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_files/voice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4329 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_forcereply.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6855 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_forumtopic.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-05-07 13:32:51.093768 python-telegram-bot-raw-20.3/telegram/_games/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_games/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1270 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_games/callbackgame.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8064 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_games/game.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2494 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_games/gamehighscore.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-05-07 13:32:51.097768 python-telegram-bot-raw-20.3/telegram/_inline/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    15081 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinekeyboardbutton.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5591 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinekeyboardmarkup.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9344 2023-05-07 12:56:49.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequery.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2770 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresult.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7967 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultarticle.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5625 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultaudio.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5088 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedaudio.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5606 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcacheddocument.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5363 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedgif.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5454 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedmpeg4gif.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5609 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedphoto.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3629 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedsticker.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5526 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedvideo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5301 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedvoice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8252 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcontact.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9875 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultdocument.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2715 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultgame.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10543 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultgif.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12054 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultlocation.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10114 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultmpeg4gif.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8583 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultphoto.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5363 2023-05-07 12:56:49.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultsbutton.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9874 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultvenue.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10492 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultvideo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5527 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultvoice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2716 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inputcontactmessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12680 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inputinvoicemessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6528 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inputlocationmessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1528 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inputmessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3691 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inputtextmessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4511 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_inline/inputvenuemessagecontent.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9173 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_keyboardbutton.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2417 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_keyboardbuttonpolltype.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     9333 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_keyboardbuttonrequest.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5096 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_loginurl.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6744 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_menubutton.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)   160309 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_message.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1976 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_messageautodeletetimerchanged.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8171 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_messageentity.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1665 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_messageid.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-05-07 13:32:51.097768 python-telegram-bot-raw-20.3/telegram/_passport/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_passport/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    22561 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_passport/credentials.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6303 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_passport/data.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    12481 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_passport/encryptedpassportelement.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5161 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_passport/passportdata.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    16944 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_passport/passportelementerrors.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6186 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_passport/passportfile.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-05-07 13:32:51.097768 python-telegram-bot-raw-20.3/telegram/_payment/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_payment/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5016 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_payment/invoice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2664 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_payment/labeledprice.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3044 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_payment/orderinfo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5918 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_payment/precheckoutquery.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2938 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_payment/shippingaddress.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2516 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_payment/shippingoption.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4493 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_payment/shippingquery.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4909 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_payment/successfulpayment.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    16254 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_poll.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2813 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_proximityalerttriggered.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    16268 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_replykeyboardmarkup.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3198 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_replykeyboardremove.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2165 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_sentwebappmessage.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4286 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_shared.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4076 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_switchinlinequerychosenchat.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    25884 2023-05-07 12:56:49.000000 python-telegram-bot-raw-20.3/telegram/_telegramobject.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    19406 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_update.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    60726 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_user.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2897 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_userprofilephotos.py
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-05-07 13:32:51.101768 python-telegram-bot-raw-20.3/telegram/_utils/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_utils/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1520 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_utils/argumentparsing.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     8956 2023-04-26 19:48:31.000000 python-telegram-bot-raw-20.3/telegram/_utils/datetime.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     4060 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_utils/defaultvalue.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2662 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_utils/enum.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5735 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_utils/files.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1932 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_utils/logging.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2100 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_utils/markup.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3276 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_utils/types.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2010 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_utils/warnings.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     3941 2023-05-07 12:56:49.000000 python-telegram-bot-raw-20.3/telegram/_utils/warnings_transition.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2148 2023-05-07 13:02:55.000000 python-telegram-bot-raw-20.3/telegram/_version.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5982 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_videochat.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2405 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_webappdata.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     2083 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/_webappinfo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7600 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_webhookinfo.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1825 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/_writeaccessallowed.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    68271 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/constants.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     6288 2023-05-07 12:56:49.000000 python-telegram-bot-raw-20.3/telegram/error.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7146 2023-05-07 13:04:05.000000 python-telegram-bot-raw-20.3/telegram/helpers.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)        0 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/py.typed
+drwxrwxr-x   0 hinrich   (1000) hinrich   (1000)        0 2023-05-07 13:32:51.101768 python-telegram-bot-raw-20.3/telegram/request/
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1081 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/request/__init__.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    18113 2023-04-26 19:48:31.000000 python-telegram-bot-raw-20.3/telegram/request/_baserequest.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)    10362 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/request/_httpxrequest.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     5155 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/request/_requestdata.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     7394 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/request/_requestparameter.py
+-rw-rw-r--   0 hinrich   (1000) hinrich   (1000)     1900 2023-04-23 11:52:44.000000 python-telegram-bot-raw-20.3/telegram/warnings.py
```

### Comparing `python-telegram-bot-raw-20.2/LICENSE` & `python-telegram-bot-raw-20.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/LICENSE.dual` & `python-telegram-bot-raw-20.3/LICENSE.dual`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/LICENSE.lesser` & `python-telegram-bot-raw-20.3/LICENSE.lesser`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/PKG-INFO` & `python-telegram-bot-raw-20.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-telegram-bot-raw
-Version: 20.2
+Version: 20.3
 Summary: We have made you a wrapper you can't refuse
 Home-page: https://python-telegram-bot.org/
 Download-URL: https://pypi.org/project/python-telegram-bot-raw/
 Author: Leandro Toledo
 Author-email: devs@python-telegram-bot.org
 License: LGPLv3
 Project-URL: Documentation, https://docs.python-telegram-bot.org
@@ -49,15 +49,15 @@
    :target: https://pypi.org/project/python-telegram-bot-raw/
    :alt: PyPi Package Version
 
 .. image:: https://img.shields.io/pypi/pyversions/python-telegram-bot-raw.svg
    :target: https://pypi.org/project/python-telegram-bot-raw/
    :alt: Supported Python versions
 
-.. image:: https://img.shields.io/badge/Bot%20API-6.6-blue?logo=telegram
+.. image:: https://img.shields.io/badge/Bot%20API-6.7-blue?logo=telegram
    :target: https://core.telegram.org/bots/api-changelog
    :alt: Supported Bot API versions
 
 .. image:: https://img.shields.io/pypi/dm/python-telegram-bot-raw
    :target: https://pypistats.org/packages/python-telegram-bot-raw
    :alt: PyPi Package Monthly Download
 
@@ -81,16 +81,16 @@
    :target: https://isitmaintained.com/project/python-telegram-bot/python-telegram-bot
    :alt: Median time to resolve an issue
 
 .. image:: https://api.codacy.com/project/badge/Grade/99d901eaa09b44b4819aec05c330c968
    :target: https://app.codacy.com/gh/python-telegram-bot/python-telegram-bot/dashboard
    :alt: Code quality: Codacy
 
-.. image:: https://deepsource.io/gh/python-telegram-bot/python-telegram-bot.svg/?label=active+issues
-   :target: https://deepsource.io/gh/python-telegram-bot/python-telegram-bot/?ref=repository-badge
+.. image:: https://app.deepsource.com/gh/python-telegram-bot/python-telegram-bot.svg/?label=active+issues
+   :target: https://app.deepsource.com/gh/python-telegram-bot/python-telegram-bot/?ref=repository-badge
    :alt: Code quality: DeepSource
 
 .. image:: https://results.pre-commit.ci/badge/github/python-telegram-bot/python-telegram-bot/master.svg
    :target: https://results.pre-commit.ci/latest/github/python-telegram-bot/python-telegram-bot/master
    :alt: pre-commit.ci status
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
@@ -124,15 +124,15 @@
 ----
 
 Installing both ``python-telegram-bot`` and ``python-telegram-bot-raw`` in conjunction will result in undesired side-effects, so only install *one* of both.
 
 Telegram API support
 ====================
 
-All types and methods of the Telegram Bot API **6.6** are supported.
+All types and methods of the Telegram Bot API **6.7** are supported.
 
 Installing
 ==========
 
 You can install or upgrade ``python-telegram-bot`` via
 
 .. code:: shell
```

### Comparing `python-telegram-bot-raw-20.2/README.rst` & `python-telegram-bot-raw-20.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
    :target: https://pypi.org/project/python-telegram-bot/
    :alt: PyPi Package Version
 
 .. image:: https://img.shields.io/pypi/pyversions/python-telegram-bot.svg
    :target: https://pypi.org/project/python-telegram-bot/
    :alt: Supported Python versions
 
-.. image:: https://img.shields.io/badge/Bot%20API-6.6-blue?logo=telegram
+.. image:: https://img.shields.io/badge/Bot%20API-6.7-blue?logo=telegram
    :target: https://core.telegram.org/bots/api-changelog
    :alt: Supported Bot API versions
 
 .. image:: https://img.shields.io/pypi/dm/python-telegram-bot
    :target: https://pypistats.org/packages/python-telegram-bot
    :alt: PyPi Package Monthly Download
 
@@ -42,16 +42,16 @@
    :target: https://isitmaintained.com/project/python-telegram-bot/python-telegram-bot
    :alt: Median time to resolve an issue
 
 .. image:: https://api.codacy.com/project/badge/Grade/99d901eaa09b44b4819aec05c330c968
    :target: https://app.codacy.com/gh/python-telegram-bot/python-telegram-bot/dashboard
    :alt: Code quality: Codacy
 
-.. image:: https://deepsource.io/gh/python-telegram-bot/python-telegram-bot.svg/?label=active+issues
-   :target: https://deepsource.io/gh/python-telegram-bot/python-telegram-bot/?ref=repository-badge
+.. image:: https://app.deepsource.com/gh/python-telegram-bot/python-telegram-bot.svg/?label=active+issues
+   :target: https://app.deepsource.com/gh/python-telegram-bot/python-telegram-bot/?ref=repository-badge
    :alt: Code quality: DeepSource
 
 .. image:: https://results.pre-commit.ci/badge/github/python-telegram-bot/python-telegram-bot/master.svg
    :target: https://results.pre-commit.ci/latest/github/python-telegram-bot/python-telegram-bot/master
    :alt: pre-commit.ci status
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
@@ -89,15 +89,15 @@
 ----
 
 Installing both ``python-telegram-bot`` and ``python-telegram-bot-raw`` in conjunction will result in undesired side-effects, so only install *one* of both.
 
 Telegram API support
 ====================
 
-All types and methods of the Telegram Bot API **6.6** are supported.
+All types and methods of the Telegram Bot API **6.7** are supported.
 
 Installing
 ==========
 
 You can install or upgrade ``python-telegram-bot`` via
 
 .. code:: shell
```

### Comparing `python-telegram-bot-raw-20.2/README_RAW.rst` & `python-telegram-bot-raw-20.3/README_RAW.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
    :target: https://pypi.org/project/python-telegram-bot-raw/
    :alt: PyPi Package Version
 
 .. image:: https://img.shields.io/pypi/pyversions/python-telegram-bot-raw.svg
    :target: https://pypi.org/project/python-telegram-bot-raw/
    :alt: Supported Python versions
 
-.. image:: https://img.shields.io/badge/Bot%20API-6.6-blue?logo=telegram
+.. image:: https://img.shields.io/badge/Bot%20API-6.7-blue?logo=telegram
    :target: https://core.telegram.org/bots/api-changelog
    :alt: Supported Bot API versions
 
 .. image:: https://img.shields.io/pypi/dm/python-telegram-bot-raw
    :target: https://pypistats.org/packages/python-telegram-bot-raw
    :alt: PyPi Package Monthly Download
 
@@ -42,16 +42,16 @@
    :target: https://isitmaintained.com/project/python-telegram-bot/python-telegram-bot
    :alt: Median time to resolve an issue
 
 .. image:: https://api.codacy.com/project/badge/Grade/99d901eaa09b44b4819aec05c330c968
    :target: https://app.codacy.com/gh/python-telegram-bot/python-telegram-bot/dashboard
    :alt: Code quality: Codacy
 
-.. image:: https://deepsource.io/gh/python-telegram-bot/python-telegram-bot.svg/?label=active+issues
-   :target: https://deepsource.io/gh/python-telegram-bot/python-telegram-bot/?ref=repository-badge
+.. image:: https://app.deepsource.com/gh/python-telegram-bot/python-telegram-bot.svg/?label=active+issues
+   :target: https://app.deepsource.com/gh/python-telegram-bot/python-telegram-bot/?ref=repository-badge
    :alt: Code quality: DeepSource
 
 .. image:: https://results.pre-commit.ci/badge/github/python-telegram-bot/python-telegram-bot/master.svg
    :target: https://results.pre-commit.ci/latest/github/python-telegram-bot/python-telegram-bot/master
    :alt: pre-commit.ci status
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
@@ -85,15 +85,15 @@
 ----
 
 Installing both ``python-telegram-bot`` and ``python-telegram-bot-raw`` in conjunction will result in undesired side-effects, so only install *one* of both.
 
 Telegram API support
 ====================
 
-All types and methods of the Telegram Bot API **6.6** are supported.
+All types and methods of the Telegram Bot API **6.7** are supported.
 
 Installing
 ==========
 
 You can install or upgrade ``python-telegram-bot`` via
 
 .. code:: shell
```

### Comparing `python-telegram-bot-raw-20.2/python_telegram_bot_raw.egg-info/PKG-INFO` & `python-telegram-bot-raw-20.3/python_telegram_bot_raw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-telegram-bot-raw
-Version: 20.2
+Version: 20.3
 Summary: We have made you a wrapper you can't refuse
 Home-page: https://python-telegram-bot.org/
 Download-URL: https://pypi.org/project/python-telegram-bot-raw/
 Author: Leandro Toledo
 Author-email: devs@python-telegram-bot.org
 License: LGPLv3
 Project-URL: Documentation, https://docs.python-telegram-bot.org
@@ -49,15 +49,15 @@
    :target: https://pypi.org/project/python-telegram-bot-raw/
    :alt: PyPi Package Version
 
 .. image:: https://img.shields.io/pypi/pyversions/python-telegram-bot-raw.svg
    :target: https://pypi.org/project/python-telegram-bot-raw/
    :alt: Supported Python versions
 
-.. image:: https://img.shields.io/badge/Bot%20API-6.6-blue?logo=telegram
+.. image:: https://img.shields.io/badge/Bot%20API-6.7-blue?logo=telegram
    :target: https://core.telegram.org/bots/api-changelog
    :alt: Supported Bot API versions
 
 .. image:: https://img.shields.io/pypi/dm/python-telegram-bot-raw
    :target: https://pypistats.org/packages/python-telegram-bot-raw
    :alt: PyPi Package Monthly Download
 
@@ -81,16 +81,16 @@
    :target: https://isitmaintained.com/project/python-telegram-bot/python-telegram-bot
    :alt: Median time to resolve an issue
 
 .. image:: https://api.codacy.com/project/badge/Grade/99d901eaa09b44b4819aec05c330c968
    :target: https://app.codacy.com/gh/python-telegram-bot/python-telegram-bot/dashboard
    :alt: Code quality: Codacy
 
-.. image:: https://deepsource.io/gh/python-telegram-bot/python-telegram-bot.svg/?label=active+issues
-   :target: https://deepsource.io/gh/python-telegram-bot/python-telegram-bot/?ref=repository-badge
+.. image:: https://app.deepsource.com/gh/python-telegram-bot/python-telegram-bot.svg/?label=active+issues
+   :target: https://app.deepsource.com/gh/python-telegram-bot/python-telegram-bot/?ref=repository-badge
    :alt: Code quality: DeepSource
 
 .. image:: https://results.pre-commit.ci/badge/github/python-telegram-bot/python-telegram-bot/master.svg
    :target: https://results.pre-commit.ci/latest/github/python-telegram-bot/python-telegram-bot/master
    :alt: pre-commit.ci status
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
@@ -124,15 +124,15 @@
 ----
 
 Installing both ``python-telegram-bot`` and ``python-telegram-bot-raw`` in conjunction will result in undesired side-effects, so only install *one* of both.
 
 Telegram API support
 ====================
 
-All types and methods of the Telegram Bot API **6.6** are supported.
+All types and methods of the Telegram Bot API **6.7** are supported.
 
 Installing
 ==========
 
 You can install or upgrade ``python-telegram-bot`` via
 
 .. code:: shell
```

### Comparing `python-telegram-bot-raw-20.2/requirements-opts.txt` & `python-telegram-bot-raw-20.3/requirements-opts.txt`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/setup.cfg` & `python-telegram-bot-raw-20.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/setup.py` & `python-telegram-bot-raw-20.3/setup.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/__init__.py` & `python-telegram-bot-raw-20.3/telegram/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     "BotCommandScopeAllGroupChats",
     "BotCommandScopeAllPrivateChats",
     "BotCommandScopeChat",
     "BotCommandScopeChatAdministrators",
     "BotCommandScopeChatMember",
     "BotCommandScopeDefault",
     "BotDescription",
+    "BotName",
     "BotShortDescription",
     "CallbackGame",
     "CallbackQuery",
     "Chat",
     "ChatAdministratorRights",
     "ChatInviteLink",
     "ChatJoinRequest",
@@ -98,14 +99,15 @@
     "InlineQueryResultContact",
     "InlineQueryResultDocument",
     "InlineQueryResultGame",
     "InlineQueryResultGif",
     "InlineQueryResultLocation",
     "InlineQueryResultMpeg4Gif",
     "InlineQueryResultPhoto",
+    "InlineQueryResultsButton",
     "InlineQueryResultVenue",
     "InlineQueryResultVideo",
     "InlineQueryResultVoice",
     "InputContactMessageContent",
     "InputFile",
     "InputInvoiceMessageContent",
     "InputLocationMessageContent",
@@ -165,14 +167,15 @@
     "SentWebAppMessage",
     "ShippingAddress",
     "ShippingOption",
     "ShippingQuery",
     "Sticker",
     "StickerSet",
     "SuccessfulPayment",
+    "SwitchInlineQueryChosenChat",
     "TelegramObject",
     "Update",
     "User",
     "UserProfilePhotos",
     "UserShared",
     "Venue",
     "Video",
@@ -200,14 +203,15 @@
     BotCommandScopeAllPrivateChats,
     BotCommandScopeChat,
     BotCommandScopeChatAdministrators,
     BotCommandScopeChatMember,
     BotCommandScopeDefault,
 )
 from ._botdescription import BotDescription, BotShortDescription
+from ._botname import BotName
 from ._callbackquery import CallbackQuery
 from ._chat import Chat
 from ._chatadministratorrights import ChatAdministratorRights
 from ._chatinvitelink import ChatInviteLink
 from ._chatjoinrequest import ChatJoinRequest
 from ._chatlocation import ChatLocation
 from ._chatmember import (
@@ -276,14 +280,15 @@
 from ._inline.inlinequeryresultcontact import InlineQueryResultContact
 from ._inline.inlinequeryresultdocument import InlineQueryResultDocument
 from ._inline.inlinequeryresultgame import InlineQueryResultGame
 from ._inline.inlinequeryresultgif import InlineQueryResultGif
 from ._inline.inlinequeryresultlocation import InlineQueryResultLocation
 from ._inline.inlinequeryresultmpeg4gif import InlineQueryResultMpeg4Gif
 from ._inline.inlinequeryresultphoto import InlineQueryResultPhoto
+from ._inline.inlinequeryresultsbutton import InlineQueryResultsButton
 from ._inline.inlinequeryresultvenue import InlineQueryResultVenue
 from ._inline.inlinequeryresultvideo import InlineQueryResultVideo
 from ._inline.inlinequeryresultvoice import InlineQueryResultVoice
 from ._inline.inputcontactmessagecontent import InputContactMessageContent
 from ._inline.inputinvoicemessagecontent import InputInvoiceMessageContent
 from ._inline.inputlocationmessagecontent import InputLocationMessageContent
 from ._inline.inputmessagecontent import InputMessageContent
@@ -332,14 +337,15 @@
 from ._payment.successfulpayment import SuccessfulPayment
 from ._poll import Poll, PollAnswer, PollOption
 from ._proximityalerttriggered import ProximityAlertTriggered
 from ._replykeyboardmarkup import ReplyKeyboardMarkup
 from ._replykeyboardremove import ReplyKeyboardRemove
 from ._sentwebappmessage import SentWebAppMessage
 from ._shared import ChatShared, UserShared
+from ._switchinlinequerychosenchat import SwitchInlineQueryChosenChat
 from ._telegramobject import TelegramObject
 from ._update import Update
 from ._user import User
 from ._userprofilephotos import UserProfilePhotos
 from ._videochat import (
     VideoChatEnded,
     VideoChatParticipantsInvited,
```

### Comparing `python-telegram-bot-raw-20.2/telegram/__main__.py` & `python-telegram-bot-raw-20.3/telegram/__main__.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_bot.py` & `python-telegram-bot-raw-20.3/telegram/_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram Bot."""
 import asyncio
+import contextlib
 import copy
 import functools
-import logging
 import pickle
 from datetime import datetime
 from types import TracebackType
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncContextManager,
@@ -52,14 +52,15 @@
     default_backend = None  # type: ignore[assignment]
     serialization = None  # type: ignore[assignment]
     CRYPTO_INSTALLED = False
 
 from telegram._botcommand import BotCommand
 from telegram._botcommandscope import BotCommandScope
 from telegram._botdescription import BotDescription, BotShortDescription
+from telegram._botname import BotName
 from telegram._chat import Chat
 from telegram._chatadministratorrights import ChatAdministratorRights
 from telegram._chatinvitelink import ChatInviteLink
 from telegram._chatmember import ChatMember
 from telegram._chatpermissions import ChatPermissions
 from telegram._files.animation import Animation
 from telegram._files.audio import Audio
@@ -75,28 +76,30 @@
 from telegram._files.venue import Venue
 from telegram._files.video import Video
 from telegram._files.videonote import VideoNote
 from telegram._files.voice import Voice
 from telegram._forumtopic import ForumTopic
 from telegram._games.gamehighscore import GameHighScore
 from telegram._inline.inlinekeyboardmarkup import InlineKeyboardMarkup
+from telegram._inline.inlinequeryresultsbutton import InlineQueryResultsButton
 from telegram._menubutton import MenuButton
 from telegram._message import Message
 from telegram._messageid import MessageId
 from telegram._passport.passportelementerrors import PassportElementError
 from telegram._payment.shippingoption import ShippingOption
 from telegram._poll import Poll
 from telegram._sentwebappmessage import SentWebAppMessage
 from telegram._telegramobject import TelegramObject
 from telegram._update import Update
 from telegram._user import User
 from telegram._userprofilephotos import UserProfilePhotos
 from telegram._utils.argumentparsing import parse_sequence_arg
 from telegram._utils.defaultvalue import DEFAULT_NONE, DefaultValue
 from telegram._utils.files import is_local_file, parse_file_input
+from telegram._utils.logging import get_logger
 from telegram._utils.types import DVInput, FileInput, JSONDict, ODVInput, ReplyMarkup
 from telegram._utils.warnings import warn
 from telegram._utils.warnings_transition import warn_about_thumb_return_thumbnail
 from telegram._webhookinfo import WebhookInfo
 from telegram.constants import InlineQueryLimit
 from telegram.error import InvalidToken
 from telegram.request import BaseRequest, RequestData
@@ -148,15 +151,15 @@
           serialized instance will not reflect that change. Trying to pickle a bot instance will
           raise :exc:`pickle.PicklingError`. Trying to deepcopy a bot instance will raise
           :exc:`TypeError`.
 
     Examples:
         :any:`Raw API Bot <examples.rawapibot>`
 
-    .. seealso:: :wiki:`Your First Bot <Extensions-–-Your-first-Bot>`,
+    .. seealso:: :wiki:`Your First Bot <Extensions---Your-first-Bot>`,
         :wiki:`Builder Pattern <Builder-Pattern>`
 
     .. versionadded:: 13.2
         Objects of this class are comparable in terms of equality. Two objects of this class are
         considered equal, if their :attr:`bot` is equal.
 
     .. versionchanged:: 20.0
@@ -201,22 +204,25 @@
 
             .. versionadded:: 20.0.
 
     .. include:: inclusions/bot_methods.rst
 
     """
 
+    # This is a class variable since we want to override the logger name in ExtBot
+    # without having to change all places where this is used
+    _LOGGER = get_logger(__name__)
+
     __slots__ = (
         "_token",
         "_base_url",
         "_base_file_url",
         "_private_key",
         "_bot_user",
         "_request",
-        "_logger",
         "_initialized",
         "_local_mode",
     )
 
     def __init__(
         self,
         token: str,
@@ -234,16 +240,15 @@
         self._token: str = token
 
         self._base_url: str = base_url + self._token
         self._base_file_url: str = base_file_url + self._token
         self._local_mode: bool = local_mode
         self._bot_user: Optional[User] = None
         self._private_key: Optional[bytes] = None
-        self._logger = logging.getLogger(__name__)
-        self._initialized = False
+        self._initialized: bool = False
 
         self._request: Tuple[BaseRequest, BaseRequest] = (
             HTTPXRequest() if get_updates_request is None else get_updates_request,
             HTTPXRequest() if request is None else request,
         )
 
         # this section is about issuing a warning when using HTTP/2 and connect to a self hosted
@@ -266,15 +271,15 @@
         ):
             if warning_string:
                 warning_string += " and request"
             else:
                 warning_string = "request"
 
         if warning_string:
-            warn(
+            self._warn(
                 f"You set the HTTP version for the {warning_string} HTTPXRequest instance to "
                 f"HTTP/2. The self hosted bot api instances only support HTTP/1.1. You should "
                 f"either run a HTTP proxy in front of it which supports HTTP/2 or use HTTP/1.1.",
                 PTBUserWarning,
                 stacklevel=2,
             )
 
@@ -331,14 +336,23 @@
     def private_key(self) -> Optional[Any]:
         """Deserialized private key for decryption of telegram passport data.
 
         .. versionadded:: 20.0
         """
         return self._private_key
 
+    @classmethod
+    def _warn(
+        cls, message: str, category: Type[Warning] = PTBUserWarning, stacklevel: int = 0
+    ) -> None:
+        """Convenience method to issue a warning. This method is here mostly to make it easier
+        for ExtBot to add 1 level to all warning calls.
+        """
+        warn(message=message, category=category, stacklevel=stacklevel + 1)
+
     def __reduce__(self) -> NoReturn:
         """Customizes how :func:`copy.deepcopy` processes objects of this type. Bots can not
         be pickled and this method will always raise an exception.
 
         .. versionadded:: 20.0
 
         Raises:
@@ -356,22 +370,21 @@
             :exc:`TypeError`
         """
         raise TypeError("Bot objects cannot be deepcopied!")
 
     # TODO: After https://youtrack.jetbrains.com/issue/PY-50952 is fixed, we can revisit this and
     # consider adding Paramspec from typing_extensions to properly fix this. Currently a workaround
     def _log(func: Any):  # type: ignore[no-untyped-def] # skipcq: PY-D0003
-        logger = logging.getLogger(func.__module__)
-
         @functools.wraps(func)
-        async def decorator(*args, **kwargs):  # type: ignore[no-untyped-def]
-            logger.debug("Entering: %s", func.__name__)
-            result = await func(*args, **kwargs)  # skipcq: PYL-E1102
-            logger.debug(result)
-            logger.debug("Exiting: %s", func.__name__)
+        async def decorator(self: "Bot", *args: Any, **kwargs: Any) -> Any:
+            # pylint: disable=protected-access
+            self._LOGGER.debug("Entering: %s", func.__name__)
+            result = await func(self, *args, **kwargs)  # skipcq: PYL-E1102
+            self._LOGGER.debug(result)
+            self._LOGGER.debug("Exiting: %s", func.__name__)
             return result
 
         return decorator
 
     def _parse_file_input(
         self,
         file_input: Union[FileInput, "TelegramObject"],
@@ -407,18 +420,18 @@
         # We
         # 1) set the correct parse_mode for all InputMedia objects
         # 2) replace all DefaultValue instances with the corresponding normal value.
         for key, val in data.items():
             # 1)
             if isinstance(val, InputMedia):
                 # Copy object as not to edit it in-place
-                val = copy.copy(val)
-                with val._unfrozen():
-                    val.parse_mode = DefaultValue.get_value(val.parse_mode)
-                data[key] = val
+                new = copy.copy(val)
+                with new._unfrozen():
+                    new.parse_mode = DefaultValue.get_value(new.parse_mode)
+                data[key] = new
             elif key == "media" and isinstance(val, Sequence):
                 # Copy objects as not to edit them in-place
                 copy_list = [copy.copy(media) for media in val]
                 for media in copy_list:
                     with media._unfrozen():
                         media.parse_mode = DefaultValue.get_value(media.parse_mode)
 
@@ -475,18 +488,15 @@
         # This also converts datetimes into timestamps.
         # We don't do this earlier so that _insert_defaults (see above) has a chance to convert
         # to the default timezone in case this is called by ExtBot
         request_data = RequestData(
             parameters=[RequestParameter.from_input(key, value) for key, value in data.items()],
         )
 
-        if endpoint == "getUpdates":
-            request = self._request[0]
-        else:
-            request = self._request[1]
+        request = self._request[0] if endpoint == "getUpdates" else self._request[1]
 
         return await request.post(
             url=f"{self._base_url}/{endpoint}",
             request_data=request_data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
@@ -567,15 +577,15 @@
         the request objects used by this bot.
 
         .. seealso:: :meth:`shutdown`
 
         .. versionadded:: 20.0
         """
         if self._initialized:
-            self._logger.debug("This Bot is already initialized.")
+            self._LOGGER.debug("This Bot is already initialized.")
             return
 
         await asyncio.gather(self._request[0].initialize(), self._request[1].initialize())
         # Since the bot is to be initialized only once, we can also use it for
         # verifying the token passed and raising an exception if it's invalid.
         try:
             await self.get_me()
@@ -588,15 +598,15 @@
         :meth:`telegram.request.BaseRequest.shutdown` for the request objects used by this bot.
 
         .. seealso:: :meth:`initialize`
 
         .. versionadded:: 20.0
         """
         if not self._initialized:
-            self._logger.debug("This Bot is already shut down. Returning.")
+            self._LOGGER.debug("This Bot is already shut down. Returning.")
             return
 
         await asyncio.gather(self._request[0].shutdown(), self._request[1].shutdown())
         self._initialized = False
 
     async def __aenter__(self: BT) -> BT:
         try:
@@ -857,24 +867,23 @@
             :obj:`bool`: On success, :obj:`True` is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         data: JSONDict = {"chat_id": chat_id, "message_id": message_id}
-        result = await self._post(
+        return await self._post(
             "deleteMessage",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
-        return result
 
     @_log
     async def forward_message(
         self,
         chat_id: Union[int, str],
         from_chat_id: Union[str, int],
         message_id: int,
@@ -1155,15 +1164,18 @@
             :class:`telegram.Message`: On success, the sent Message is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         thumbnail_or_thumb: FileInput = warn_about_thumb_return_thumbnail(
-            deprecated_arg=thumb, new_arg=thumbnail
+            deprecated_arg=thumb,
+            new_arg=thumbnail,
+            warn_callback=self._warn,
+            stacklevel=3,
         )
         data: JSONDict = {
             "chat_id": chat_id,
             "audio": self._parse_file_input(audio, Audio, filename=filename),
             "duration": duration,
             "performer": performer,
             "title": title,
@@ -1292,15 +1304,18 @@
             :class:`telegram.Message`: On success, the sent Message is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         thumbnail_or_thumb: FileInput = warn_about_thumb_return_thumbnail(
-            deprecated_arg=thumb, new_arg=thumbnail
+            deprecated_arg=thumb,
+            new_arg=thumbnail,
+            warn_callback=self._warn,
+            stacklevel=3,
         )
 
         data: JSONDict = {
             "chat_id": chat_id,
             "document": self._parse_file_input(document, Document, filename=filename),
             "disable_content_type_detection": disable_content_type_detection,
             "thumbnail": self._parse_file_input(thumbnail_or_thumb, attach=True)
@@ -1529,15 +1544,18 @@
             :class:`telegram.Message`: On success, the sent Message is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         thumbnail_or_thumb: FileInput = warn_about_thumb_return_thumbnail(
-            deprecated_arg=thumb, new_arg=thumbnail
+            deprecated_arg=thumb,
+            new_arg=thumbnail,
+            warn_callback=self._warn,
+            stacklevel=3,
         )
         data: JSONDict = {
             "chat_id": chat_id,
             "video": self._parse_file_input(video, Video, filename=filename),
             "duration": duration,
             "width": width,
             "height": height,
@@ -1662,15 +1680,18 @@
             :class:`telegram.Message`: On success, the sent Message is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         thumbnail_or_thumb: FileInput = warn_about_thumb_return_thumbnail(
-            deprecated_arg=thumb, new_arg=thumbnail
+            deprecated_arg=thumb,
+            new_arg=thumbnail,
+            warn_callback=self._warn,
+            stacklevel=3,
         )
         data: JSONDict = {
             "chat_id": chat_id,
             "video_note": self._parse_file_input(video_note, VideoNote, filename=filename),
             "duration": duration,
             "length": length,
             "thumbnail": self._parse_file_input(thumbnail_or_thumb, attach=True)
@@ -1805,14 +1826,16 @@
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         thumbnail_or_thumb: FileInput = warn_about_thumb_return_thumbnail(
             deprecated_arg=thumb,
             new_arg=thumbnail,
+            warn_callback=self._warn,
+            stacklevel=3,
         )
         data: JSONDict = {
             "chat_id": chat_id,
             "animation": self._parse_file_input(animation, Animation, filename=filename),
             "duration": duration,
             "width": width,
             "height": height,
@@ -1994,15 +2017,15 @@
 
         Args:
             chat_id (:obj:`int` | :obj:`str`): |chat_id_channel|
             media (Sequence[:class:`telegram.InputMediaAudio`,\
                 :class:`telegram.InputMediaDocument`, :class:`telegram.InputMediaPhoto`,\
                 :class:`telegram.InputMediaVideo`]): An array
                 describing messages to be sent, must include
-                :tg-const:`telegram.constants.MediaGroupLimit.MIN_MEDIA_LENGTH`–
+                :tg-const:`telegram.constants.MediaGroupLimit.MIN_MEDIA_LENGTH`-
                 :tg-const:`telegram.constants.MediaGroupLimit.MAX_MEDIA_LENGTH` items.
 
                 .. versionchanged:: 20.0
                     |sequenceargs|
             disable_notification (:obj:`bool`, optional): |disable_notification|
             protect_content (:obj:`bool`, optional): |protect_content|
 
@@ -2672,24 +2695,23 @@
 
         """
         data: JSONDict = {
             "chat_id": chat_id,
             "action": action,
             "message_thread_id": message_thread_id,
         }
-        result = await self._post(
+        return await self._post(
             "sendChatAction",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
-        return result
 
     def _effective_inline_results(  # skipcq: PYL-R0201
         self,
         results: Union[
             Sequence["InlineQueryResult"], Callable[[int], Optional[Sequence["InlineQueryResult"]]]
         ],
         next_offset: str = None,
@@ -2704,44 +2726,41 @@
 
         """
         if current_offset is not None and next_offset is not None:
             raise ValueError("`current_offset` and `next_offset` are mutually exclusive!")
 
         if current_offset is not None:
             # Convert the string input to integer
-            if current_offset == "":
-                current_offset_int = 0
-            else:
-                current_offset_int = int(current_offset)
+            current_offset_int = 0 if not current_offset else int(current_offset)
 
             # for now set to empty string, stating that there are no more results
             # might change later
             next_offset = ""
 
             if callable(results):
                 callable_output = results(current_offset_int)
                 if not callable_output:
                     effective_results: Sequence["InlineQueryResult"] = []
                 else:
                     effective_results = callable_output
                     # the callback *might* return more results on the next call, so we increment
                     # the page count
                     next_offset = str(current_offset_int + 1)
+
+            elif len(results) > (current_offset_int + 1) * InlineQueryLimit.RESULTS:
+                # we expect more results for the next page
+                next_offset_int = current_offset_int + 1
+                next_offset = str(next_offset_int)
+                effective_results = results[
+                    current_offset_int
+                    * InlineQueryLimit.RESULTS : next_offset_int
+                    * InlineQueryLimit.RESULTS
+                ]
             else:
-                if len(results) > (current_offset_int + 1) * InlineQueryLimit.RESULTS:
-                    # we expect more results for the next page
-                    next_offset_int = current_offset_int + 1
-                    next_offset = str(next_offset_int)
-                    effective_results = results[
-                        current_offset_int
-                        * InlineQueryLimit.RESULTS : next_offset_int
-                        * InlineQueryLimit.RESULTS
-                    ]
-                else:
-                    effective_results = results[current_offset_int * InlineQueryLimit.RESULTS :]
+                effective_results = results[current_offset_int * InlineQueryLimit.RESULTS :]
         else:
             effective_results = results  # type: ignore[assignment]
 
         return effective_results, next_offset
 
     @no_type_check  # mypy doesn't play too well with hasattr
     def _insert_defaults_for_ilq_results(self, res: "InlineQueryResult") -> "InlineQueryResult":
@@ -2790,45 +2809,46 @@
         inline_query_id: str,
         results: Union[
             Sequence["InlineQueryResult"], Callable[[int], Optional[Sequence["InlineQueryResult"]]]
         ],
         cache_time: int = None,
         is_personal: bool = None,
         next_offset: str = None,
+        # Deprecated params since bot api 6.7
+        # <----
         switch_pm_text: str = None,
         switch_pm_parameter: str = None,
+        # --->
+        # New params since bot api 6.7
+        # <----
+        button: InlineQueryResultsButton = None,
+        # --->
         *,
         current_offset: str = None,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
         api_kwargs: JSONDict = None,
     ) -> bool:
         """
         Use this method to send answers to an inline query. No more than
         :tg-const:`telegram.InlineQuery.MAX_RESULTS` results per query are allowed.
 
-        Example:
-            An inline bot that sends YouTube videos can ask the user to connect the bot to their
-            YouTube account to adapt search results accordingly. To do this, it displays a
-            'Connect your YouTube account' button above the results, or even before showing any.
-            The user presses the button, switches to a private chat with the bot and, in doing so,
-            passes a start parameter that instructs the bot to return an OAuth link. Once done, the
-            bot can offer a switch_inline button so that the user can easily return to the chat
-            where they wanted to use the bot's inline capabilities.
-
         Warning:
             In most use cases :paramref:`current_offset` should not be passed manually. Instead of
             calling this method directly, use the shortcut :meth:`telegram.InlineQuery.answer` with
             :paramref:`telegram.InlineQuery.answer.auto_pagination` set to :obj:`True`, which will
             take care of passing the correct value.
 
         .. seealso:: :wiki:`Working with Files and Media <Working-with-Files-and-Media>`
 
+        .. |api6_7_depr| replace:: Since Bot API 6.7, this argument is deprecated in favour of
+            :paramref:`button`.
+
         Args:
             inline_query_id (:obj:`str`): Unique identifier for the answered query.
             results (List[:class:`telegram.InlineQueryResult`] | Callable): A list of results for
                 the inline query. In case :paramref:`current_offset` is passed,
                 :paramref:`results` may also be
                 a callable that accepts the current page index starting from 0. It must return
                 either a list of :class:`telegram.InlineQueryResult` instances or :obj:`None` if
@@ -2841,33 +2861,63 @@
             next_offset (:obj:`str`, optional): Pass the offset that a client should send in the
                 next query with the same text to receive more results. Pass an empty string if
                 there are no more results or if you don't support pagination. Offset length can't
                 exceed :tg-const:`telegram.InlineQuery.MAX_OFFSET_LENGTH` bytes.
             switch_pm_text (:obj:`str`, optional): If passed, clients will display a button with
                 specified text that switches the user to a private chat with the bot and sends the
                 bot a start message with the parameter :paramref:`switch_pm_parameter`.
+
+                .. deprecated:: 20.3
+                    |api6_7_depr|
             switch_pm_parameter (:obj:`str`, optional): Deep-linking parameter for the
                 :guilabel:`/start` message sent to the bot when user presses the switch button.
                 :tg-const:`telegram.InlineQuery.MIN_SWITCH_PM_TEXT_LENGTH`-
                 :tg-const:`telegram.InlineQuery.MAX_SWITCH_PM_TEXT_LENGTH` characters,
                 only ``A-Z``, ``a-z``, ``0-9``, ``_`` and ``-`` are allowed.
 
+                .. deprecated:: 20.3
+                    |api6_7_depr|
+            button (:class:`telegram.InlineQueryResultsButton`, optional): A button to be shown
+                above the inline query results.
+
+                .. versionadded:: 20.3
+
         Keyword Args:
             current_offset (:obj:`str`, optional): The :attr:`telegram.InlineQuery.offset` of
                 the inline query to answer. If passed, PTB will automatically take care of
                 the pagination for you, i.e. pass the correct :paramref:`next_offset` and truncate
                 the results list/get the results from the callable you passed.
 
         Returns:
             :obj:`bool`: On success, :obj:`True` is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
+        if (switch_pm_text or switch_pm_parameter) and button:
+            raise TypeError(
+                "Since Bot API 6.7, the parameter `button is mutually exclusive to the deprecated "
+                "parameters `switch_pm_text` and `switch_pm_parameter`. Please use the new "
+                "parameter `button`."
+            )
+
+        if switch_pm_text and switch_pm_parameter:
+            self._warn(
+                "Since Bot API 6.7, the parameters `switch_pm_text` and `switch_pm_parameter` are "
+                "deprecated in favour of the new parameter `button`. Please use the new parameter "
+                "`button` instead.",
+                category=PTBDeprecationWarning,
+                stacklevel=3,
+            )
+            button = InlineQueryResultsButton(
+                text=switch_pm_text,
+                start_parameter=switch_pm_parameter,
+            )
+
         effective_results, next_offset = self._effective_inline_results(
             results=results, next_offset=next_offset, current_offset=current_offset
         )
 
         # Apply defaults
         effective_results = [
             self._insert_defaults_for_ilq_results(result) for result in effective_results
@@ -2875,16 +2925,15 @@
 
         data: JSONDict = {
             "inline_query_id": inline_query_id,
             "results": effective_results,
             "next_offset": next_offset,
             "cache_time": cache_time,
             "is_personal": is_personal,
-            "switch_pm_text": switch_pm_text,
-            "switch_pm_parameter": switch_pm_parameter,
+            "button": button,
         }
 
         return await self._post(
             "answerInlineQuery",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
@@ -2978,18 +3027,17 @@
         Returns:
             :class:`telegram.File`
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
-        try:  # Try to get the file_id from the object
+        # Try to get the file_id from the object, if it fails, assume it's a string
+        with contextlib.suppress(AttributeError):
             file_id = file_id.file_id  # type: ignore[union-attr]
-        except AttributeError:  # If it fails, assume it's a string
-            pass
 
         data: JSONDict = {"file_id": file_id}
 
         result = await self._post(
             "getFile",
             data,
             read_timeout=read_timeout,
@@ -3055,26 +3103,24 @@
         data: JSONDict = {
             "chat_id": chat_id,
             "user_id": user_id,
             "revoke_messages": revoke_messages,
             "until_date": until_date,
         }
 
-        result = await self._post(
+        return await self._post(
             "banChatMember",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-        return result
-
     @_log
     async def ban_chat_sender_chat(
         self,
         chat_id: Union[str, int],
         sender_chat_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -3101,26 +3147,24 @@
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         data: JSONDict = {"chat_id": chat_id, "sender_chat_id": sender_chat_id}
 
-        result = await self._post(
+        return await self._post(
             "banChatSenderChat",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-        return result
-
     @_log
     async def unban_chat_member(
         self,
         chat_id: Union[str, int],
         user_id: Union[str, int],
         only_if_banned: bool = None,
         *,
@@ -3148,26 +3192,24 @@
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         data: JSONDict = {"chat_id": chat_id, "user_id": user_id, "only_if_banned": only_if_banned}
 
-        result = await self._post(
+        return await self._post(
             "unbanChatMember",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-        return result
-
     @_log
     async def unban_chat_sender_chat(
         self,
         chat_id: Union[str, int],
         sender_chat_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -3191,26 +3233,24 @@
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         data: JSONDict = {"chat_id": chat_id, "sender_chat_id": sender_chat_id}
 
-        result = await self._post(
+        return await self._post(
             "unbanChatSenderChat",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-        return result
-
     @_log
     async def answer_callback_query(
         self,
         callback_query_id: str,
         text: str = None,
         show_alert: bool = None,
         url: str = None,
@@ -3259,26 +3299,24 @@
             "callback_query_id": callback_query_id,
             "cache_time": cache_time,
             "text": text,
             "show_alert": show_alert,
             "url": url,
         }
 
-        result = await self._post(
+        return await self._post(
             "answerCallbackQuery",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-        return result
-
     @_log
     async def edit_message_text(
         self,
         text: str,
         chat_id: Union[str, int] = None,
         message_id: int = None,
         inline_message_id: str = None,
@@ -3574,15 +3612,15 @@
         Args:
             offset (:obj:`int`, optional): Identifier of the first update to be returned. Must be
                 greater by one than the highest among the identifiers of previously received
                 updates. By default, updates starting with the earliest unconfirmed update are
                 returned. An update is considered confirmed as soon as this method is called with
                 an offset higher than its :attr:`telegram.Update.update_id`. The negative offset
                 can be specified to retrieve updates starting from -offset update from the end of
-                the updates queue. All previous updates will forgotten.
+                the updates queue. All previous updates will be forgotten.
             limit (:obj:`int`, optional): Limits the number of updates to be retrieved. Values
                 between :tg-const:`telegram.constants.PollingLimit.MIN_LIMIT`-
                 :tg-const:`telegram.constants.PollingLimit.MAX_LIMIT` are accepted.
                 Defaults to ``100``.
             timeout (:obj:`int`, optional): Timeout in seconds for long polling. Defaults to ``0``,
                 i.e. usual short polling. Should be positive, short polling should be used for
                 testing purposes only.
@@ -3628,17 +3666,17 @@
                 connect_timeout=connect_timeout,
                 pool_timeout=pool_timeout,
                 api_kwargs=api_kwargs,
             ),
         )
 
         if result:
-            self._logger.debug("Getting updates: %s", [u["update_id"] for u in result])
+            self._LOGGER.debug("Getting updates: %s", [u["update_id"] for u in result])
         else:
-            self._logger.debug("No new updates found.")
+            self._LOGGER.debug("No new updates found.")
 
         return Update.de_list(result, self)
 
     @_log
     async def set_webhook(
         self,
         url: str,
@@ -3749,26 +3787,24 @@
             "allowed_updates": allowed_updates,
             "ip_address": ip_address,
             "drop_pending_updates": drop_pending_updates,
             "secret_token": secret_token,
             "certificate": self._parse_file_input(certificate),  # type: ignore[arg-type]
         }
 
-        result = await self._post(
+        return await self._post(
             "setWebhook",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-        return result
-
     @_log
     async def delete_webhook(
         self,
         drop_pending_updates: bool = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -3789,26 +3825,24 @@
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         data = {"drop_pending_updates": drop_pending_updates}
 
-        result = await self._post(
+        return await self._post(
             "deleteWebhook",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-        return result
-
     @_log
     async def leave_chat(
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -3826,26 +3860,24 @@
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         data: JSONDict = {"chat_id": chat_id}
 
-        result = await self._post(
+        return await self._post(
             "leaveChat",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-        return result
-
     @_log
     async def get_chat(
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -3945,24 +3977,23 @@
             :obj:`int`: Number of members in the chat.
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         data: JSONDict = {"chat_id": chat_id}
-        result = await self._post(
+        return await self._post(
             "getChatMemberCount",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
-        return result
 
     @_log
     async def get_chat_member(
         self,
         chat_id: Union[str, int],
         user_id: Union[str, int],
         *,
@@ -4020,24 +4051,23 @@
             sticker_set_name (:obj:`str`): Name of the sticker set to be set as the group
                 sticker set.
 
         Returns:
             :obj:`bool`: On success, :obj:`True` is returned.
         """
         data: JSONDict = {"chat_id": chat_id, "sticker_set_name": sticker_set_name}
-        result = await self._post(
+        return await self._post(
             "setChatStickerSet",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
-        return result
 
     @_log
     async def delete_chat_sticker_set(
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -4054,24 +4084,23 @@
         Args:
             chat_id (:obj:`int` | :obj:`str`): |chat_id_group|
 
         Returns:
              :obj:`bool`: On success, :obj:`True` is returned.
         """
         data: JSONDict = {"chat_id": chat_id}
-        result = await self._post(
+        return await self._post(
             "deleteChatStickerSet",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
-        return result
 
     @_log
     async def get_webhook_info(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -4451,26 +4480,24 @@
         data: JSONDict = {
             "shipping_query_id": shipping_query_id,
             "ok": ok,
             "shipping_options": shipping_options,
             "error_message": error_message,
         }
 
-        result = await self._post(
+        return await self._post(
             "answerShippingQuery",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-        return result
-
     @_log
     async def answer_pre_checkout_query(  # pylint: disable=invalid-name
         self,
         pre_checkout_query_id: str,
         ok: bool,
         error_message: str = None,
         *,
@@ -4510,26 +4537,24 @@
         """
         data: JSONDict = {
             "pre_checkout_query_id": pre_checkout_query_id,
             "ok": ok,
             "error_message": error_message,
         }
 
-        result = await self._post(
+        return await self._post(
             "answerPreCheckoutQuery",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-        return result
-
     @_log
     async def answer_web_app_query(
         self,
         web_app_query_id: str,
         result: "InlineQueryResult",
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -4633,26 +4658,24 @@
             "chat_id": chat_id,
             "user_id": user_id,
             "permissions": permissions,
             "until_date": until_date,
             "use_independent_chat_permissions": use_independent_chat_permissions,
         }
 
-        result = await self._post(
+        return await self._post(
             "restrictChatMember",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-        return result
-
     @_log
     async def promote_chat_member(
         self,
         chat_id: Union[str, int],
         user_id: Union[str, int],
         can_change_info: bool = None,
         can_post_messages: bool = None,
@@ -4742,26 +4765,24 @@
             "can_pin_messages": can_pin_messages,
             "can_promote_members": can_promote_members,
             "can_manage_chat": can_manage_chat,
             "can_manage_video_chats": can_manage_video_chats,
             "can_manage_topics": can_manage_topics,
         }
 
-        result = await self._post(
+        return await self._post(
             "promoteChatMember",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-        return result
-
     @_log
     async def set_chat_permissions(
         self,
         chat_id: Union[str, int],
         permissions: ChatPermissions,
         use_independent_chat_permissions: bool = None,
         *,
@@ -4803,24 +4824,23 @@
 
         """
         data: JSONDict = {
             "chat_id": chat_id,
             "permissions": permissions,
             "use_independent_chat_permissions": use_independent_chat_permissions,
         }
-        result = await self._post(
+        return await self._post(
             "setChatPermissions",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
-        return result
 
     @_log
     async def set_chat_administrator_custom_title(
         self,
         chat_id: Union[int, str],
         user_id: Union[int, str],
         custom_title: str,
@@ -4847,26 +4867,24 @@
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         data: JSONDict = {"chat_id": chat_id, "user_id": user_id, "custom_title": custom_title}
 
-        result = await self._post(
+        return await self._post(
             "setChatAdministratorCustomTitle",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-        return result
-
     @_log
     async def export_chat_invite_link(
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -4893,24 +4911,23 @@
             :obj:`str`: New invite link on success.
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         data: JSONDict = {"chat_id": chat_id}
-        result = await self._post(
+        return await self._post(
             "exportChatInviteLink",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
-        return result
 
     @_log
     async def create_chat_invite_link(
         self,
         chat_id: Union[str, int],
         expire_date: Union[int, datetime] = None,
         member_limit: int = None,
@@ -5135,26 +5152,24 @@
             :obj:`bool`: On success, :obj:`True` is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
         """
         data: JSONDict = {"chat_id": chat_id, "user_id": user_id}
 
-        result = await self._post(
+        return await self._post(
             "approveChatJoinRequest",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-        return result
-
     @_log
     async def decline_chat_join_request(
         self,
         chat_id: Union[str, int],
         user_id: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -5178,26 +5193,24 @@
             :obj:`bool`: On success, :obj:`True` is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
         """
         data: JSONDict = {"chat_id": chat_id, "user_id": user_id}
 
-        result = await self._post(
+        return await self._post(
             "declineChatJoinRequest",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-        return result
-
     @_log
     async def set_chat_photo(
         self,
         chat_id: Union[str, int],
         photo: FileInput,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -5227,24 +5240,23 @@
             :obj:`bool`: On success, :obj:`True` is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         data: JSONDict = {"chat_id": chat_id, "photo": self._parse_file_input(photo)}
-        result = await self._post(
+        return await self._post(
             "setChatPhoto",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
-        return result
 
     @_log
     async def delete_chat_photo(
         self,
         chat_id: Union[str, int],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -5265,24 +5277,23 @@
             :obj:`bool`: On success, :obj:`True` is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         data: JSONDict = {"chat_id": chat_id}
-        result = await self._post(
+        return await self._post(
             "deleteChatPhoto",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
-        return result
 
     @_log
     async def set_chat_title(
         self,
         chat_id: Union[str, int],
         title: str,
         *,
@@ -5307,24 +5318,23 @@
             :obj:`bool`: On success, :obj:`True` is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         data: JSONDict = {"chat_id": chat_id, "title": title}
-        result = await self._post(
+        return await self._post(
             "setChatTitle",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
-        return result
 
     @_log
     async def set_chat_description(
         self,
         chat_id: Union[str, int],
         description: str = None,
         *,
@@ -5350,24 +5360,23 @@
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         data: JSONDict = {"chat_id": chat_id, "description": description}
 
-        result = await self._post(
+        return await self._post(
             "setChatDescription",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
-        return result
 
     @_log
     async def pin_chat_message(
         self,
         chat_id: Union[str, int],
         message_id: int,
         disable_notification: ODVInput[bool] = DEFAULT_NONE,
@@ -5656,19 +5665,20 @@
                 "`png_sticker`. Please use the new parameters "
                 "`sticker` and `sticker_format` instead."
             )
             # If we had allowed this, the created sticker set would have used the newer parameters
             # only, which would have been confusing.
 
         if png_sticker:
-            warn(
+            self._warn(
                 "Since Bot API 6.6, the parameter `png_sticker` for "
                 "`upload_sticker_file` is deprecated. Please use the new parameters "
                 "`sticker` and `sticker_format` instead.",
-                stacklevel=4,
+                stacklevel=3,
+                category=PTBDeprecationWarning,
             )
 
         data: JSONDict = {
             "user_id": user_id,
             "sticker": self._parse_file_input(sticker),  # type: ignore[arg-type]
             "sticker_format": sticker_format,
             # Deprecated param since bot api 6.6
@@ -5855,19 +5865,20 @@
                 f"{set(pre_api_6_6_params)}. Please use the new parameter "
                 "`stickers` and `sticker_format` instead."
             )
             # If we had allowed this, the created sticker set would have used the newer parameters
             # only, which would have been confusing.
 
         if any(pre_api_6_6_params.values()):
-            warn(
+            self._warn(
                 f"Since Bot API 6.6, the parameters {set(pre_api_6_6_params)} for "
                 "`create_new_sticker_set` are deprecated. Please use the new parameter "
                 "`stickers` and `sticker_format` instead.",
-                stacklevel=4,
+                stacklevel=3,
+                category=PTBDeprecationWarning,
             )
 
         data: JSONDict = {
             "user_id": user_id,
             "name": name,
             "title": title,
             "stickers": stickers,
@@ -5878,26 +5889,24 @@
             "emojis": emojis,
             "png_sticker": self._parse_file_input(png_sticker) if png_sticker else None,
             "tgs_sticker": self._parse_file_input(tgs_sticker) if tgs_sticker else None,
             "webm_sticker": self._parse_file_input(webm_sticker) if webm_sticker else None,
             "mask_position": mask_position,
         }
 
-        result = await self._post(
+        return await self._post(
             "createNewStickerSet",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-        return result
-
     @_log
     async def add_sticker_to_set(
         self,
         user_id: Union[str, int],
         name: str,
         # Deprecated params since bot api 6.6
         # ----
@@ -6028,45 +6037,44 @@
                 "Since Bot API 6.6, the parameter `sticker` "
                 "is mutually exclusive with the deprecated parameters "
                 f"{set(pre_api_6_6_params)}. Please use the new parameter "
                 "`sticker` instead."
             )
 
         if any(pre_api_6_6_params.values()):
-            warn(
+            self._warn(
                 f"Since Bot API 6.6, the parameters {set(pre_api_6_6_params)} for "
                 "`add_sticker_to_set` are deprecated. Please use the new parameter `sticker` "
                 "instead.",
-                stacklevel=4,
+                stacklevel=3,
+                category=PTBDeprecationWarning,
             )
 
         data: JSONDict = {
             "user_id": user_id,
             "name": name,
             "sticker": sticker,
             # Deprecated params since bot api 6.6:
             "emojis": emojis,
             "png_sticker": self._parse_file_input(png_sticker) if png_sticker else None,
             "tgs_sticker": self._parse_file_input(tgs_sticker) if tgs_sticker else None,
             "webm_sticker": self._parse_file_input(webm_sticker) if webm_sticker else None,
             "mask_position": mask_position,
         }
 
-        result = await self._post(
+        return await self._post(
             "addStickerToSet",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-        return result
-
     @_log
     async def set_sticker_position_in_set(
         self,
         sticker: str,
         position: int,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6085,24 +6093,23 @@
             :obj:`bool`: On success, :obj:`True` is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         data: JSONDict = {"sticker": sticker, "position": position}
-        result = await self._post(
+        return await self._post(
             "setStickerPositionInSet",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
-        return result
 
     @_log
     async def delete_sticker_from_set(
         self,
         sticker: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6120,24 +6127,23 @@
             :obj:`bool`: On success, :obj:`True` is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         data: JSONDict = {"sticker": sticker}
-        result = await self._post(
+        return await self._post(
             "deleteStickerFromSet",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
-        return result
 
     @_log
     async def delete_sticker_set(
         self,
         name: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6158,24 +6164,23 @@
             :obj:`bool`: On success, :obj:`True` is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         data: JSONDict = {"name": name}
-        result = await self._post(
+        return await self._post(
             "deleteStickerSet",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
-        return result
 
     @_log
     async def set_sticker_set_thumbnail(
         self,
         name: str,
         user_id: Union[str, int],
         thumbnail: FileInput = None,
@@ -6273,15 +6278,15 @@
         Returns:
             :obj:`bool`: On success, :obj:`True` is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
-        warn(
+        self._warn(
             message=(
                 "Bot API 6.6 renamed the method 'setStickerSetThumb' to 'setStickerSetThumbnail', "
                 "hence method 'set_sticker_set_thumb' was renamed to 'set_sticker_set_thumbnail' "
                 "in PTB."
             ),
             category=PTBDeprecationWarning,
             stacklevel=3,
@@ -6313,26 +6318,24 @@
     ) -> bool:
         data: JSONDict = {
             "name": name,
             "user_id": user_id,
             "thumbnail": self._parse_file_input(thumbnail) if thumbnail else None,
         }
 
-        result = await self._post(
+        return await self._post(
             "setStickerSetThumbnail",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-        return result
-
     @_log
     async def set_sticker_set_title(
         self,
         name: str,
         title: str,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6356,24 +6359,23 @@
             :obj:`bool`: On success, :obj:`True` is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         data: JSONDict = {"name": name, "title": title}
-        result = await self._post(
+        return await self._post(
             "setStickerSetTitle",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
-        return result
 
     @_log
     async def set_sticker_emoji_list(
         self,
         sticker: str,
         emoji_list: Sequence[str],
         *,
@@ -6399,24 +6401,23 @@
         Returns:
             :obj:`bool`: On success, :obj:`True` is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
         """
         data: JSONDict = {"sticker": sticker, "emoji_list": emoji_list}
-        result = await self._post(
+        return await self._post(
             "setStickerEmojiList",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
-        return result
 
     @_log
     async def set_sticker_keywords(
         self,
         sticker: str,
         keywords: Sequence[str] = None,
         *,
@@ -6442,24 +6443,23 @@
         Returns:
             :obj:`bool`: On success, :obj:`True` is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
         """
         data: JSONDict = {"sticker": sticker, "keywords": keywords}
-        result = await self._post(
+        return await self._post(
             "setStickerKeywords",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
-        return result
 
     @_log
     async def set_sticker_mask_position(
         self,
         sticker: str,
         mask_position: MaskPosition = None,
         *,
@@ -6484,24 +6484,23 @@
         Returns:
             :obj:`bool`: On success, :obj:`True` is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
         """
         data: JSONDict = {"sticker": sticker, "mask_position": mask_position}
-        result = await self._post(
+        return await self._post(
             "setStickerMaskPosition",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
-        return result
 
     @_log
     async def set_custom_emoji_sticker_set_thumbnail(
         self,
         name: str,
         custom_emoji_id: str = None,
         *,
@@ -6527,26 +6526,24 @@
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         data: JSONDict = {"name": name, "custom_emoji_id": custom_emoji_id}
 
-        result = await self._post(
+        return await self._post(
             "setCustomEmojiStickerSetThumbnail",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-        return result
-
     @_log
     async def set_passport_data_errors(
         self,
         user_id: Union[str, int],
         errors: Sequence[PassportElementError],
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -6576,24 +6573,23 @@
             :obj:`bool`: On success, :obj:`True` is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         data: JSONDict = {"user_id": user_id, "errors": errors}
-        result = await self._post(
+        return await self._post(
             "setPassportDataErrors",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
-        return result
 
     @_log
     async def send_poll(
         self,
         chat_id: Union[int, str],
         question: str,
         options: Sequence[str],
@@ -6922,26 +6918,24 @@
             :obj:`bool`: Returns :obj:`True` on success.
 
         Raises:
             :obj:`telegram.error.TelegramError`
         """
         data: JSONDict = {"rights": rights, "for_channels": for_channels}
 
-        result = await self._post(
+        return await self._post(
             "setMyDefaultAdministratorRights",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-        return result
-
     @_log
     async def get_my_commands(
         self,
         scope: BotCommandScope = None,
         language_code: str = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -7043,26 +7037,24 @@
         Raises:
             :class:`telegram.error.TelegramError`
 
         """
         cmds = [c if isinstance(c, BotCommand) else BotCommand(c[0], c[1]) for c in commands]
         data: JSONDict = {"commands": cmds, "scope": scope, "language_code": language_code}
 
-        result = await self._post(
+        return await self._post(
             "setMyCommands",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-        return result
-
     @_log
     async def delete_my_commands(
         self,
         scope: BotCommandScope = None,
         language_code: str = None,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -7093,26 +7085,24 @@
             :obj:`bool`: On success, :obj:`True` is returned.
 
         Raises:
             :class:`telegram.error.TelegramError`
         """
         data: JSONDict = {"scope": scope, "language_code": language_code}
 
-        result = await self._post(
+        return await self._post(
             "deleteMyCommands",
             data,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
 
-        return result
-
     @_log
     async def log_out(
         self,
         *,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -8176,14 +8166,102 @@
                 connect_timeout=connect_timeout,
                 pool_timeout=pool_timeout,
                 api_kwargs=api_kwargs,
             ),
             bot=self,
         )
 
+    @_log
+    async def set_my_name(
+        self,
+        name: str = None,
+        language_code: str = None,
+        *,
+        read_timeout: ODVInput[float] = DEFAULT_NONE,
+        write_timeout: ODVInput[float] = DEFAULT_NONE,
+        connect_timeout: ODVInput[float] = DEFAULT_NONE,
+        pool_timeout: ODVInput[float] = DEFAULT_NONE,
+        api_kwargs: JSONDict = None,
+    ) -> bool:
+        """
+        Use this method to change the bot's name.
+
+        .. versionadded:: 20.3
+
+        Args:
+            name (:obj:`str`, optional): New bot name;
+                0-:tg-const:`telegram.constants.BotNameLimit.MAX_NAME_LENGTH`
+                characters. Pass an empty string to remove the dedicated name for the given
+                language.
+
+                Caution:
+                    If :paramref:`language_code` is not specified, a :paramref:`name` *must*
+                    be specified.
+            language_code (:obj:`str`, optional): A two-letter ISO 639-1 language code. If empty,
+                the name will be applied to all users for whose language there is no
+                dedicated name.
+
+        Returns:
+            :obj:`bool`: On success, :obj:`True` is returned.
+
+        Raises:
+            :class:`telegram.error.TelegramError`
+
+        """
+        data: JSONDict = {"name": name, "language_code": language_code}
+
+        return await self._post(
+            "setMyName",
+            data,
+            read_timeout=read_timeout,
+            write_timeout=write_timeout,
+            connect_timeout=connect_timeout,
+            pool_timeout=pool_timeout,
+            api_kwargs=api_kwargs,
+        )
+
+    @_log
+    async def get_my_name(
+        self,
+        language_code: str = None,
+        *,
+        read_timeout: ODVInput[float] = DEFAULT_NONE,
+        write_timeout: ODVInput[float] = DEFAULT_NONE,
+        connect_timeout: ODVInput[float] = DEFAULT_NONE,
+        pool_timeout: ODVInput[float] = DEFAULT_NONE,
+        api_kwargs: JSONDict = None,
+    ) -> BotName:
+        """
+        Use this method to get the current bot name for the given user language.
+
+        Args:
+            language_code (:obj:`str`, optional): A two-letter ISO 639-1 language code or an empty
+                string.
+
+        Returns:
+            :class:`telegram.BotName`: On success, the bot name is returned.
+
+        Raises:
+            :class:`telegram.error.TelegramError`
+
+        """
+        data = {"language_code": language_code}
+        return BotName.de_json(  # type: ignore[return-value]
+            await self._post(
+                "getMyName",
+                data,
+                read_timeout=read_timeout,
+                write_timeout=write_timeout,
+                connect_timeout=connect_timeout,
+                pool_timeout=pool_timeout,
+                api_kwargs=api_kwargs,
+            ),
+            bot=self,
+        )
+
     def to_dict(self, recursive: bool = True) -> JSONDict:  # skipcq: PYL-W0613
         """See :meth:`telegram.TelegramObject.to_dict`."""
         data: JSONDict = {"id": self.id, "username": self.username, "first_name": self.first_name}
 
         if self.last_name:
             data["last_name"] = self.last_name
 
@@ -8420,7 +8498,11 @@
     """Alias for :meth:`delete_sticker_set`"""
     setStickerEmojiList = set_sticker_emoji_list
     """Alias for :meth:`set_sticker_emoji_list`"""
     setStickerKeywords = set_sticker_keywords
     """Alias for :meth:`set_sticker_keywords`"""
     setStickerMaskPosition = set_sticker_mask_position
     """Alias for :meth:`set_sticker_mask_position`"""
+    setMyName = set_my_name
+    """Alias for :meth:`set_my_name`"""
+    getMyName = get_my_name
+    """Alias for :meth:`get_my_name`"""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_botcommand.py` & `python-telegram-bot-raw-20.3/telegram/_botcommand.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_botcommandscope.py` & `python-telegram-bot-raw-20.3/telegram/_botcommandscope.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_botdescription.py` & `python-telegram-bot-raw-20.3/telegram/_botdescription.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     """
 
     __slots__ = ("description",)
 
     def __init__(self, description: str, *, api_kwargs: JSONDict = None):
         super().__init__(api_kwargs=api_kwargs)
-        self.description = description
+        self.description: str = description
 
         self._id_attrs = (self.description,)
 
         self._freeze()
 
 
 class BotShortDescription(TelegramObject):
@@ -64,12 +64,12 @@
 
     """
 
     __slots__ = ("short_description",)
 
     def __init__(self, short_description: str, *, api_kwargs: JSONDict = None):
         super().__init__(api_kwargs=api_kwargs)
-        self.short_description = short_description
+        self.short_description: str = short_description
 
         self._id_attrs = (self.short_description,)
 
         self._freeze()
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_callbackquery.py` & `python-telegram-bot-raw-20.3/telegram/_callbackquery.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_chat.py` & `python-telegram-bot-raw-20.3/telegram/_chat.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_chatadministratorrights.py` & `python-telegram-bot-raw-20.3/telegram/_chatadministratorrights.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_chatinvitelink.py` & `python-telegram-bot-raw-20.3/telegram/_chatinvitelink.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents an invite link for a chat."""
 import datetime
 from typing import TYPE_CHECKING, Optional
 
 from telegram._telegramobject import TelegramObject
 from telegram._user import User
-from telegram._utils.datetime import from_timestamp
+from telegram._utils.datetime import extract_tzinfo_from_defaults, from_timestamp
 from telegram._utils.types import JSONDict
 
 if TYPE_CHECKING:
     from telegram import Bot
 
 
 class ChatInviteLink(TelegramObject):
@@ -50,14 +50,17 @@
             the link need to be approved by chat administrators.
 
             .. versionadded:: 13.8
         is_primary (:obj:`bool`): :obj:`True`, if the link is primary.
         is_revoked (:obj:`bool`): :obj:`True`, if the link is revoked.
         expire_date (:class:`datetime.datetime`, optional): Date when the link will expire or
             has been expired.
+
+            .. versionchanged:: 20.3
+                |datetime_localization|
         member_limit (:obj:`int`, optional): Maximum number of users that can be members of the
             chat simultaneously after joining the chat via this invite link;
             :tg-const:`telegram.constants.ChatInviteLinkLimit.MIN_MEMBER_LIMIT`-
             :tg-const:`telegram.constants.ChatInviteLinkLimit.MAX_MEMBER_LIMIT`.
         name (:obj:`str`, optional): Invite link name.
             0-:tg-const:`telegram.constants.ChatInviteLinkLimit.NAME_LENGTH` characters.
 
@@ -74,14 +77,17 @@
             the link need to be approved by chat administrators.
 
             .. versionadded:: 13.8
         is_primary (:obj:`bool`): :obj:`True`, if the link is primary.
         is_revoked (:obj:`bool`): :obj:`True`, if the link is revoked.
         expire_date (:class:`datetime.datetime`): Optional. Date when the link will expire or
             has been expired.
+
+            .. versionchanged:: 20.3
+                |datetime_localization|
         member_limit (:obj:`int`): Optional. Maximum number of users that can be members
             of the chat simultaneously after joining the chat via this invite link;
             :tg-const:`telegram.constants.ChatInviteLinkLimit.MIN_MEMBER_LIMIT`-
             :tg-const:`telegram.constants.ChatInviteLinkLimit.MAX_MEMBER_LIMIT`.
         name (:obj:`str`): Optional. Invite link name.
             0-:tg-const:`telegram.constants.ChatInviteLinkLimit.NAME_LENGTH` characters.
 
@@ -148,11 +154,14 @@
     def de_json(cls, data: Optional[JSONDict], bot: "Bot") -> Optional["ChatInviteLink"]:
         """See :meth:`telegram.TelegramObject.de_json`."""
         data = cls._parse_data(data)
 
         if not data:
             return None
 
+        # Get the local timezone from the bot if it has defaults
+        loc_tzinfo = extract_tzinfo_from_defaults(bot)
+
         data["creator"] = User.de_json(data.get("creator"), bot)
-        data["expire_date"] = from_timestamp(data.get("expire_date", None))
+        data["expire_date"] = from_timestamp(data.get("expire_date", None), tzinfo=loc_tzinfo)
 
         return super().de_json(data=data, bot=bot)
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_chatjoinrequest.py` & `python-telegram-bot-raw-20.3/telegram/_chatjoinrequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import datetime
 from typing import TYPE_CHECKING, Optional
 
 from telegram._chat import Chat
 from telegram._chatinvitelink import ChatInviteLink
 from telegram._telegramobject import TelegramObject
 from telegram._user import User
-from telegram._utils.datetime import from_timestamp
+from telegram._utils.datetime import extract_tzinfo_from_defaults, from_timestamp
 from telegram._utils.defaultvalue import DEFAULT_NONE
 from telegram._utils.types import JSONDict, ODVInput
 
 if TYPE_CHECKING:
     from telegram import Bot
 
 
@@ -37,29 +37,32 @@
 
     Objects of this class are comparable in terms of equality. Two objects of this class are
     considered equal, if their :attr:`chat`, :attr:`from_user` and :attr:`date` are equal.
 
     Note:
         * Since Bot API 5.5, bots are allowed to contact users who sent a join request to a chat
           where the bot is an administrator with the
-          :attr:`~telegram.ChatMemberAdministrator.can_invite_users` administrator right – even
+          :attr:`~telegram.ChatMemberAdministrator.can_invite_users` administrator right - even
           if the user never interacted with the bot before.
         * Telegram does not guarantee that :attr:`from_user.id <from_user>` coincides with the
           ``chat_id`` of the user. Please use :attr:`user_chat_id` to contact the user in
           response to their join request.
 
     .. versionadded:: 13.8
     .. versionchanged:: 20.1
        In Bot API 6.5 the argument :paramref:`user_chat_id` was added, which changes the position
        of the optional arguments :paramref:`bio` and :paramref:`invite_link`.
 
     Args:
         chat (:class:`telegram.Chat`): Chat to which the request was sent.
         from_user (:class:`telegram.User`): User that sent the join request.
         date (:class:`datetime.datetime`): Date the request was sent.
+
+            .. versionchanged:: 20.3
+                |datetime_localization|
         user_chat_id (:obj:`int`): Identifier of a private chat with the user who sent the join
             request. This number may have more than 32 significant bits and some programming
             languages may have difficulty/silent defects in interpreting it. But it has at most 52
             significant bits, so a 64-bit integer or double-precision float type are safe for
             storing this identifier. The bot can use this identifier for 24 hours to send messages
             until the join request is processed, assuming no other administrator contacted the
             user.
@@ -69,14 +72,17 @@
         invite_link (:class:`telegram.ChatInviteLink`, optional): Chat invite link that was used
             by the user to send the join request.
 
     Attributes:
         chat (:class:`telegram.Chat`): Chat to which the request was sent.
         from_user (:class:`telegram.User`): User that sent the join request.
         date (:class:`datetime.datetime`): Date the request was sent.
+
+            .. versionchanged:: 20.3
+                |datetime_localization|
         user_chat_id (:obj:`int`): Identifier of a private chat with the user who sent the join
             request. This number may have more than 32 significant bits and some programming
             languages may have difficulty/silent defects in interpreting it. But it has at most 52
             significant bits, so a 64-bit integer or double-precision float type are safe for
             storing this identifier. The bot can use this identifier for 24 hours to send messages
             until the join request is processed, assuming no other administrator contacted the
             user.
@@ -120,17 +126,20 @@
     def de_json(cls, data: Optional[JSONDict], bot: "Bot") -> Optional["ChatJoinRequest"]:
         """See :meth:`telegram.TelegramObject.de_json`."""
         data = cls._parse_data(data)
 
         if not data:
             return None
 
+        # Get the local timezone from the bot if it has defaults
+        loc_tzinfo = extract_tzinfo_from_defaults(bot)
+
         data["chat"] = Chat.de_json(data.get("chat"), bot)
         data["from_user"] = User.de_json(data.pop("from", None), bot)
-        data["date"] = from_timestamp(data.get("date", None))
+        data["date"] = from_timestamp(data.get("date", None), tzinfo=loc_tzinfo)
         data["invite_link"] = ChatInviteLink.de_json(data.get("invite_link"), bot)
 
         return super().de_json(data=data, bot=bot)
 
     async def approve(
         self,
         *,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_chatlocation.py` & `python-telegram-bot-raw-20.3/telegram/_chatlocation.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_chatmember.py` & `python-telegram-bot-raw-20.3/telegram/_chatmember.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 """This module contains an object that represents a Telegram ChatMember."""
 import datetime
 from typing import TYPE_CHECKING, ClassVar, Dict, Optional, Type
 
 from telegram import constants
 from telegram._telegramobject import TelegramObject
 from telegram._user import User
-from telegram._utils.datetime import from_timestamp
+from telegram._utils.datetime import extract_tzinfo_from_defaults, from_timestamp
 from telegram._utils.types import JSONDict
 
 if TYPE_CHECKING:
     from telegram import Bot
 
 
 class ChatMember(TelegramObject):
@@ -121,15 +121,18 @@
         }
 
         if cls is ChatMember and data.get("status") in _class_mapping:
             return _class_mapping[data.pop("status")].de_json(data=data, bot=bot)
 
         data["user"] = User.de_json(data.get("user"), bot)
         if "until_date" in data:
-            data["until_date"] = from_timestamp(data["until_date"])
+            # Get the local timezone from the bot if it has defaults
+            loc_tzinfo = extract_tzinfo_from_defaults(bot)
+
+            data["until_date"] = from_timestamp(data["until_date"], tzinfo=loc_tzinfo)
 
         return super().de_json(data=data, bot=bot)
 
 
 class ChatMemberOwner(ChatMember):
     """
     Represents a chat member that owns the chat
@@ -382,14 +385,17 @@
            allowed to add web page previews to their messages.
         can_manage_topics (:obj:`bool`): :obj:`True`, if the user is allowed to create
             forum topics.
 
             .. versionadded:: 20.0
         until_date (:class:`datetime.datetime`): Date when restrictions
            will be lifted for this user.
+
+            .. versionchanged:: 20.3
+                |datetime_localization|
         can_send_audios (:obj:`bool`): :obj:`True`, if the user is allowed to send audios.
 
             .. versionadded:: 20.1
         can_send_documents (:obj:`bool`): :obj:`True`, if the user is allowed to send documents.
 
             .. versionadded:: 20.1
         can_send_photos (:obj:`bool`): :obj:`True`, if the user is allowed to send photos.
@@ -434,14 +440,17 @@
            allowed to add web page previews to their messages.
         can_manage_topics (:obj:`bool`): :obj:`True`, if the user is allowed to create
             forum topics.
 
             .. versionadded:: 20.0
         until_date (:class:`datetime.datetime`): Date when restrictions
            will be lifted for this user.
+
+            .. versionchanged:: 20.3
+                |datetime_localization|
         can_send_audios (:obj:`bool`): :obj:`True`, if the user is allowed to send audios.
 
             .. versionadded:: 20.1
         can_send_documents (:obj:`bool`): :obj:`True`, if the user is allowed to send documents.
 
             .. versionadded:: 20.1
         can_send_photos (:obj:`bool`): :obj:`True`, if the user is allowed to send photos.
@@ -561,21 +570,27 @@
     .. versionadded:: 13.7
 
     Args:
         user (:class:`telegram.User`): Information about the user.
         until_date (:class:`datetime.datetime`): Date when restrictions
            will be lifted for this user.
 
+            .. versionchanged:: 20.3
+                |datetime_localization|
+
     Attributes:
         status (:obj:`str`): The member's status in the chat,
             always :tg-const:`telegram.ChatMember.BANNED`.
         user (:class:`telegram.User`): Information about the user.
         until_date (:class:`datetime.datetime`): Date when restrictions
            will be lifted for this user.
 
+            .. versionchanged:: 20.3
+                |datetime_localization|
+
     """
 
     __slots__ = ("until_date",)
 
     def __init__(
         self,
         user: User,
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_chatmemberupdated.py` & `python-telegram-bot-raw-20.3/telegram/_chatmemberupdated.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from typing import TYPE_CHECKING, Dict, Optional, Tuple, Union
 
 from telegram._chat import Chat
 from telegram._chatinvitelink import ChatInviteLink
 from telegram._chatmember import ChatMember
 from telegram._telegramobject import TelegramObject
 from telegram._user import User
-from telegram._utils.datetime import from_timestamp
+from telegram._utils.datetime import extract_tzinfo_from_defaults, from_timestamp
 from telegram._utils.types import JSONDict
 
 if TYPE_CHECKING:
     from telegram import Bot
 
 
 class ChatMemberUpdated(TelegramObject):
@@ -48,58 +48,75 @@
         :any:`Chat Member Bot <examples.chatmemberbot>`
 
     Args:
         chat (:class:`telegram.Chat`): Chat the user belongs to.
         from_user (:class:`telegram.User`): Performer of the action, which resulted in the change.
         date (:class:`datetime.datetime`): Date the change was done in Unix time. Converted to
             :class:`datetime.datetime`.
+
+            .. versionchanged:: 20.3
+                |datetime_localization|
         old_chat_member (:class:`telegram.ChatMember`): Previous information about the chat member.
         new_chat_member (:class:`telegram.ChatMember`): New information about the chat member.
         invite_link (:class:`telegram.ChatInviteLink`, optional): Chat invite link, which was used
             by the user to join the chat. For joining by invite link events only.
+        via_chat_folder_invite_link (:obj:`bool`, optional): :obj:`True`, if the user joined the
+            chat via a chat folder invite link
+
+            .. versionadded:: 20.3
 
     Attributes:
         chat (:class:`telegram.Chat`): Chat the user belongs to.
         from_user (:class:`telegram.User`): Performer of the action, which resulted in the change.
         date (:class:`datetime.datetime`): Date the change was done in Unix time. Converted to
             :class:`datetime.datetime`.
+
+            .. versionchanged:: 20.3
+                |datetime_localization|
         old_chat_member (:class:`telegram.ChatMember`): Previous information about the chat member.
         new_chat_member (:class:`telegram.ChatMember`): New information about the chat member.
         invite_link (:class:`telegram.ChatInviteLink`): Optional. Chat invite link, which was used
             by the user to join the chat. For joining by invite link events only.
+        via_chat_folder_invite_link (:obj:`bool`): Optional. :obj:`True`, if the user joined the
+            chat via a chat folder invite link
+
+            .. versionadded:: 20.3
 
     """
 
     __slots__ = (
         "chat",
         "from_user",
         "date",
         "old_chat_member",
         "new_chat_member",
         "invite_link",
+        "via_chat_folder_invite_link",
     )
 
     def __init__(
         self,
         chat: Chat,
         from_user: User,
         date: datetime.datetime,
         old_chat_member: ChatMember,
         new_chat_member: ChatMember,
         invite_link: ChatInviteLink = None,
+        via_chat_folder_invite_link: bool = None,
         *,
         api_kwargs: JSONDict = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.chat: Chat = chat
         self.from_user: User = from_user
         self.date: datetime.datetime = date
         self.old_chat_member: ChatMember = old_chat_member
         self.new_chat_member: ChatMember = new_chat_member
+        self.via_chat_folder_invite_link: Optional[bool] = via_chat_folder_invite_link
 
         # Optionals
         self.invite_link: Optional[ChatInviteLink] = invite_link
 
         self._id_attrs = (
             self.chat,
             self.from_user,
@@ -114,17 +131,20 @@
     def de_json(cls, data: Optional[JSONDict], bot: "Bot") -> Optional["ChatMemberUpdated"]:
         """See :meth:`telegram.TelegramObject.de_json`."""
         data = cls._parse_data(data)
 
         if not data:
             return None
 
+        # Get the local timezone from the bot if it has defaults
+        loc_tzinfo = extract_tzinfo_from_defaults(bot)
+
         data["chat"] = Chat.de_json(data.get("chat"), bot)
         data["from_user"] = User.de_json(data.pop("from", None), bot)
-        data["date"] = from_timestamp(data.get("date"))
+        data["date"] = from_timestamp(data.get("date"), tzinfo=loc_tzinfo)
         data["old_chat_member"] = ChatMember.de_json(data.get("old_chat_member"), bot)
         data["new_chat_member"] = ChatMember.de_json(data.get("new_chat_member"), bot)
         data["invite_link"] = ChatInviteLink.de_json(data.get("invite_link"), bot)
 
         return super().de_json(data=data, bot=bot)
 
     def _get_attribute_difference(self, attribute: str) -> Tuple[object, object]:
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_chatpermissions.py` & `python-telegram-bot-raw-20.3/telegram/_chatpermissions.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_choseninlineresult.py` & `python-telegram-bot-raw-20.3/telegram/_choseninlineresult.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_dice.py` & `python-telegram-bot-raw-20.3/telegram/_dice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_files/_basemedium.py` & `python-telegram-bot-raw-20.3/telegram/_files/_basemedium.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_files/_basethumbedmedium.py` & `python-telegram-bot-raw-20.3/telegram/_files/_basethumbedmedium.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
         self.thumbnail: Optional[PhotoSize] = warn_about_deprecated_arg_return_new_arg(
             deprecated_arg=thumb,
             new_arg=thumbnail,
             deprecated_arg_name="thumb",
             new_arg_name="thumbnail",
             bot_api_version="6.6",
-            stacklevel=4,
+            stacklevel=3,
         )
 
     @property
     def thumb(self) -> Optional[PhotoSize]:
         """:class:`telegram.PhotoSize`: Optional. Thumbnail as defined by sender.
 
         .. deprecated:: 20.2
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_files/animation.py` & `python-telegram-bot-raw-20.3/telegram/_files/animation.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_files/audio.py` & `python-telegram-bot-raw-20.3/telegram/_files/audio.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_files/chatphoto.py` & `python-telegram-bot-raw-20.3/telegram/_files/chatphoto.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_files/contact.py` & `python-telegram-bot-raw-20.3/telegram/_files/contact.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_files/document.py` & `python-telegram-bot-raw-20.3/telegram/_files/document.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_files/file.py` & `python-telegram-bot-raw-20.3/telegram/_files/file.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_files/inputfile.py` & `python-telegram-bot-raw-20.3/telegram/_files/inputfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,24 +14,22 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram InputFile."""
 
-import logging
 import mimetypes
 from typing import IO, Optional, Union
 from uuid import uuid4
 
 from telegram._utils.files import load_file
 from telegram._utils.types import FieldTuple
 
 _DEFAULT_MIME_TYPE = "application/octet-stream"
-logger = logging.getLogger(__name__)
 
 
 class InputFile:
     """This object represents a Telegram InputFile.
 
     .. versionchanged:: 20.0
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_files/inputmedia.py` & `python-telegram-bot-raw-20.3/telegram/_files/inputmedia.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_files/inputsticker.py` & `python-telegram-bot-raw-20.3/telegram/_files/inputsticker.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_files/location.py` & `python-telegram-bot-raw-20.3/telegram/_files/location.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_files/photosize.py` & `python-telegram-bot-raw-20.3/telegram/_files/photosize.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_files/sticker.py` & `python-telegram-bot-raw-20.3/telegram/_files/sticker.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_files/venue.py` & `python-telegram-bot-raw-20.3/telegram/_files/venue.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_files/video.py` & `python-telegram-bot-raw-20.3/telegram/_files/video.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_files/videonote.py` & `python-telegram-bot-raw-20.3/telegram/_files/videonote.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_files/voice.py` & `python-telegram-bot-raw-20.3/telegram/_files/voice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_forcereply.py` & `python-telegram-bot-raw-20.3/telegram/_forcereply.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_forumtopic.py` & `python-telegram-bot-raw-20.3/telegram/_forumtopic.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_games/callbackgame.py` & `python-telegram-bot-raw-20.3/telegram/_games/callbackgame.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_games/game.py` & `python-telegram-bot-raw-20.3/telegram/_games/game.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram Game."""
-import sys
 from typing import TYPE_CHECKING, Dict, List, Optional, Sequence, Tuple
 
 from telegram._files.animation import Animation
 from telegram._files.photosize import PhotoSize
 from telegram._messageentity import MessageEntity
 from telegram._telegramobject import TelegramObject
 from telegram._utils.argumentparsing import parse_sequence_arg
@@ -154,17 +153,14 @@
         Raises:
             RuntimeError: If this game has no text.
 
         """
         if not self.text:
             raise RuntimeError("This Game has no 'text'.")
 
-        # Is it a narrow build, if so we don't need to convert
-        if sys.maxunicode == 0xFFFF:
-            return self.text[entity.offset : entity.offset + entity.length]
         entity_text = self.text.encode("utf-16-le")
         entity_text = entity_text[entity.offset * 2 : (entity.offset + entity.length) * 2]
 
         return entity_text.decode("utf-16-le")
 
     def parse_text_entities(self, types: List[str] = None) -> Dict[MessageEntity, str]:
         """
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_games/gamehighscore.py` & `python-telegram-bot-raw-20.3/telegram/_games/gamehighscore.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinekeyboardbutton.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinekeyboardbutton.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 """This module contains an object that represents a Telegram InlineKeyboardButton."""
 
 from typing import TYPE_CHECKING, ClassVar, Optional, Union
 
 from telegram import constants
 from telegram._games.callbackgame import CallbackGame
 from telegram._loginurl import LoginUrl
+from telegram._switchinlinequerychosenchat import SwitchInlineQueryChosenChat
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 from telegram._webappinfo import WebAppInfo
 
 if TYPE_CHECKING:
     from telegram import Bot
 
@@ -107,25 +108,43 @@
         switch_inline_query (:obj:`str`, optional): If set, pressing the button will prompt the
             user to select one of their chats, open that chat and insert the bot's username and the
             specified inline query in the input field. Can be empty, in which case just the bot's
             username will be inserted. This offers an easy way for users to start using your bot
             in inline mode when they are currently in a private chat with it. Especially useful
             when combined with ``switch_pm*`` actions - in this case the user will be automatically
             returned to the chat they switched from, skipping the chat selection screen.
+
+            Tip:
+                This is similar to the new parameter :paramref:`switch_inline_query_chosen_chat`,
+                but gives no control over which chats can be selected.
         switch_inline_query_current_chat (:obj:`str`, optional): If set, pressing the button will
             insert the bot's username and the specified inline query in the current chat's input
             field. Can be empty, in which case only the bot's username will be inserted. This
             offers a quick way for the user to open your bot in inline mode in the same chat - good
             for selecting something from multiple options.
         callback_game (:class:`telegram.CallbackGame`, optional): Description of the game that will
             be launched when the user presses the button. This type of button **must** always be
             the **first** button in the first row.
         pay (:obj:`bool`, optional): Specify :obj:`True`, to send a Pay button. This type of button
             **must** always be the **first** button in the first row and can only be used in
             invoice messages.
+        switch_inline_query_chosen_chat (:obj:`telegram.SwitchInlineQueryChosenChat`, optional):
+            If set, pressing the button will prompt the user to select one of their chats of the
+            specified type, open that chat and insert the bot's username and the specified inline
+            query in the input field.
+
+            .. versionadded:: 20.3
+
+            Tip:
+                This is similar to :paramref:`switch_inline_query`, but gives more control on
+                which chats can be selected.
+
+            Caution:
+                The PTB team has discovered that this field works correctly only if your Telegram
+                client is released after April 20th 2023.
 
     Attributes:
         text (:obj:`str`): Label text on the button.
         url (:obj:`str`): Optional. HTTP or tg:// url to be opened when the button is pressed.
             Links ``tg://user?id=<user_id>`` can be used to mention a user by
             their ID without using a username, if this is allowed by their privacy settings.
 
@@ -150,51 +169,70 @@
         switch_inline_query (:obj:`str`): Optional. If set, pressing the button will prompt the
             user to select one of their chats, open that chat and insert the bot's username and the
             specified inline query in the input field. Can be empty, in which case just the bot's
             username will be inserted. This offers an easy way for users to start using your bot
             in inline mode when they are currently in a private chat with it. Especially useful
             when combined with ``switch_pm*`` actions - in this case the user will be automatically
             returned to the chat they switched from, skipping the chat selection screen.
+
+            Tip:
+                This is similar to the new parameter :paramref:`switch_inline_query_chosen_chat`,
+                but gives no control over which chats can be selected.
         switch_inline_query_current_chat (:obj:`str`): Optional. If set, pressing the button will
             insert the bot's username and the specified inline query in the current chat's input
             field. Can be empty, in which case only the bot's username will be inserted. This
             offers a quick way for the user to open your bot in inline mode in the same chat - good
             for selecting something from multiple options.
         callback_game (:class:`telegram.CallbackGame`): Optional. Description of the game that will
             be launched when the user presses the button. This type of button **must** always be
             the **first** button in the first row.
         pay (:obj:`bool`): Optional. Specify :obj:`True`, to send a Pay button. This type of button
             **must** always be the **first** button in the first row and can only be used in
             invoice messages.
+        switch_inline_query_chosen_chat (:obj:`telegram.SwitchInlineQueryChosenChat`): Optional.
+            If set, pressing the button will prompt the user to select one of their chats of the
+            specified type, open that chat and insert the bot's username and the specified inline
+            query in the input field.
 
+            .. versionadded:: 20.3
+
+            Tip:
+                This is similar to :attr:`switch_inline_query`, but gives more control on
+                which chats can be selected.
+
+            Caution:
+                The PTB team has discovered that this field works correctly only if your Telegram
+                client is released after April 20th 2023.
     """
 
     __slots__ = (
         "callback_game",
         "url",
         "switch_inline_query_current_chat",
         "callback_data",
         "pay",
         "switch_inline_query",
         "text",
         "login_url",
         "web_app",
+        "switch_inline_query_chosen_chat",
     )
 
     def __init__(
         self,
         text: str,
         url: str = None,
         callback_data: Union[str, object] = None,
         switch_inline_query: str = None,
         switch_inline_query_current_chat: str = None,
         callback_game: CallbackGame = None,
         pay: bool = None,
         login_url: LoginUrl = None,
         web_app: WebAppInfo = None,
+        switch_inline_query_chosen_chat: SwitchInlineQueryChosenChat = None,
         *,
         api_kwargs: JSONDict = None,
     ):
         super().__init__(api_kwargs=api_kwargs)
         # Required
         self.text: str = text
 
@@ -203,14 +241,17 @@
         self.login_url: Optional[LoginUrl] = login_url
         self.callback_data: Optional[Union[str, object]] = callback_data
         self.switch_inline_query: Optional[str] = switch_inline_query
         self.switch_inline_query_current_chat: Optional[str] = switch_inline_query_current_chat
         self.callback_game: Optional[CallbackGame] = callback_game
         self.pay: Optional[bool] = pay
         self.web_app: Optional[WebAppInfo] = web_app
+        self.switch_inline_query_chosen_chat: Optional[
+            SwitchInlineQueryChosenChat
+        ] = switch_inline_query_chosen_chat
         self._id_attrs = ()
         self._set_id_attrs()
 
         self._freeze()
 
     def _set_id_attrs(self) -> None:
         self._id_attrs = (
@@ -232,14 +273,17 @@
 
         if not data:
             return None
 
         data["login_url"] = LoginUrl.de_json(data.get("login_url"), bot)
         data["web_app"] = WebAppInfo.de_json(data.get("web_app"), bot)
         data["callback_game"] = CallbackGame.de_json(data.get("callback_game"), bot)
+        data["switch_inline_query_chosen_chat"] = SwitchInlineQueryChosenChat.de_json(
+            data.get("switch_inline_query_chosen_chat"), bot
+        )
 
         return super().de_json(data=data, bot=bot)
 
     def update_callback_data(self, callback_data: Union[str, object]) -> None:
         """
         Sets :attr:`callback_data` to the passed object. Intended to be used by
         :class:`telegram.ext.CallbackDataCache`.
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinekeyboardmarkup.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinekeyboardmarkup.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinequery.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinequery.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram InlineQuery."""
 
 from typing import TYPE_CHECKING, Callable, ClassVar, Optional, Sequence, Union
 
 from telegram import constants
 from telegram._files.location import Location
+from telegram._inline.inlinequeryresultsbutton import InlineQueryResultsButton
 from telegram._telegramobject import TelegramObject
 from telegram._user import User
 from telegram._utils.defaultvalue import DEFAULT_NONE
 from telegram._utils.types import JSONDict, ODVInput
 
 if TYPE_CHECKING:
     from telegram import Bot, InlineQueryResult
@@ -142,14 +143,15 @@
             Sequence["InlineQueryResult"], Callable[[int], Optional[Sequence["InlineQueryResult"]]]
         ],
         cache_time: int = None,
         is_personal: bool = None,
         next_offset: str = None,
         switch_pm_text: str = None,
         switch_pm_parameter: str = None,
+        button: InlineQueryResultsButton = None,
         *,
         current_offset: str = None,
         auto_pagination: bool = False,
         read_timeout: ODVInput[float] = DEFAULT_NONE,
         write_timeout: ODVInput[float] = DEFAULT_NONE,
         connect_timeout: ODVInput[float] = DEFAULT_NONE,
         pool_timeout: ODVInput[float] = DEFAULT_NONE,
@@ -188,14 +190,15 @@
             current_offset=self.offset if auto_pagination else current_offset,
             results=results,
             cache_time=cache_time,
             is_personal=is_personal,
             next_offset=next_offset,
             switch_pm_text=switch_pm_text,
             switch_pm_parameter=switch_pm_parameter,
+            button=button,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
             connect_timeout=connect_timeout,
             pool_timeout=pool_timeout,
             api_kwargs=api_kwargs,
         )
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresult.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresult.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultarticle.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultarticle.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultaudio.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultaudio.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultcachedaudio.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedaudio.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultcacheddocument.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcacheddocument.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultcachedgif.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedgif.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultcachedmpeg4gif.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedmpeg4gif.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultcachedphoto.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedphoto.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultcachedsticker.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedsticker.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultcachedvideo.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedvideo.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultcachedvoice.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcachedvoice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultcontact.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultcontact.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultdocument.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultdocument.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultgame.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultgame.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultgif.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultgif.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultlocation.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultlocation.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultmpeg4gif.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultmpeg4gif.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultphoto.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultphoto.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultvenue.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultvenue.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultvideo.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultvideo.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inlinequeryresultvoice.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inlinequeryresultvoice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inputcontactmessagecontent.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inputcontactmessagecontent.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inputinvoicemessagecontent.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inputinvoicemessagecontent.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inputlocationmessagecontent.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inputlocationmessagecontent.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inputmessagecontent.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inputmessagecontent.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inputtextmessagecontent.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inputtextmessagecontent.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_inline/inputvenuemessagecontent.py` & `python-telegram-bot-raw-20.3/telegram/_inline/inputvenuemessagecontent.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_keyboardbutton.py` & `python-telegram-bot-raw-20.3/telegram/_keyboardbutton.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_keyboardbuttonpolltype.py` & `python-telegram-bot-raw-20.3/telegram/_keyboardbuttonpolltype.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_keyboardbuttonrequest.py` & `python-telegram-bot-raw-20.3/telegram/_keyboardbuttonrequest.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_loginurl.py` & `python-telegram-bot-raw-20.3/telegram/_loginurl.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_menubutton.py` & `python-telegram-bot-raw-20.3/telegram/_menubutton.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,16 +89,15 @@
             cls.COMMANDS: MenuButtonCommands,
             cls.WEB_APP: MenuButtonWebApp,
             cls.DEFAULT: MenuButtonDefault,
         }
 
         if cls is MenuButton and data.get("type") in _class_mapping:
             return _class_mapping[data.pop("type")].de_json(data, bot=bot)
-        out = super().de_json(data=data, bot=bot)
-        return out
+        return super().de_json(data=data, bot=bot)
 
     COMMANDS: ClassVar[str] = constants.MenuButtonType.COMMANDS
     """:const:`telegram.constants.MenuButtonType.COMMANDS`"""
     WEB_APP: ClassVar[str] = constants.MenuButtonType.WEB_APP
     """:const:`telegram.constants.MenuButtonType.WEB_APP`"""
     DEFAULT: ClassVar[str] = constants.MenuButtonType.DEFAULT
     """:const:`telegram.constants.MenuButtonType.DEFAULT`"""
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_message.py` & `python-telegram-bot-raw-20.3/telegram/_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram Message."""
 import datetime
-import sys
 from html import escape
 from typing import TYPE_CHECKING, Dict, List, Optional, Sequence, Tuple, Union
 
 from telegram._chat import Chat
 from telegram._dice import Dice
 from telegram._files.animation import Animation
 from telegram._files.audio import Audio
@@ -53,27 +52,29 @@
 from telegram._payment.successfulpayment import SuccessfulPayment
 from telegram._poll import Poll
 from telegram._proximityalerttriggered import ProximityAlertTriggered
 from telegram._shared import ChatShared, UserShared
 from telegram._telegramobject import TelegramObject
 from telegram._user import User
 from telegram._utils.argumentparsing import parse_sequence_arg
-from telegram._utils.datetime import from_timestamp
+from telegram._utils.datetime import extract_tzinfo_from_defaults, from_timestamp
 from telegram._utils.defaultvalue import DEFAULT_NONE, DefaultValue
 from telegram._utils.types import DVInput, FileInput, JSONDict, ODVInput, ReplyMarkup
+from telegram._utils.warnings import warn
 from telegram._videochat import (
     VideoChatEnded,
     VideoChatParticipantsInvited,
     VideoChatScheduled,
     VideoChatStarted,
 )
 from telegram._webappdata import WebAppData
 from telegram._writeaccessallowed import WriteAccessAllowed
 from telegram.constants import MessageAttachmentType, ParseMode
 from telegram.helpers import escape_markdown
+from telegram.warnings import PTBDeprecationWarning
 
 if TYPE_CHECKING:
     from telegram import (
         Bot,
         GameHighScore,
         InputMedia,
         InputMediaAudio,
@@ -118,34 +119,43 @@
             chat. For example, the channel itself for channel posts, the supergroup itself for
             messages from anonymous group administrators, the linked channel for messages
             automatically forwarded to the discussion group. For backward compatibility,
             :attr:`from_user` contains a fake sender user in non-channel chats, if the message was
             sent on behalf of a chat.
         date (:class:`datetime.datetime`): Date the message was sent in Unix time. Converted to
             :class:`datetime.datetime`.
+
+            .. versionchanged:: 20.3
+                |datetime_localization|
         chat (:class:`telegram.Chat`): Conversation the message belongs to.
         forward_from (:class:`telegram.User`, optional): For forwarded messages, sender of
             the original message.
         forward_from_chat (:class:`telegram.Chat`, optional): For messages forwarded from channels
             or from anonymous administrators, information about the original sender chat.
         forward_from_message_id (:obj:`int`, optional): For forwarded channel posts, identifier of
             the original message in the channel.
         forward_sender_name (:obj:`str`, optional): Sender's name for messages forwarded from
             users who disallow adding a link to their account in forwarded messages.
         forward_date (:class:`datetime.datetime`, optional): For forwarded messages, date the
             original message was sent in Unix time. Converted to :class:`datetime.datetime`.
+
+            .. versionchanged:: 20.3
+                |datetime_localization|
         is_automatic_forward (:obj:`bool`, optional): :obj:`True`, if the message is a channel
             post that was automatically forwarded to the connected discussion group.
 
             .. versionadded:: 13.9
         reply_to_message (:class:`telegram.Message`, optional): For replies, the original message.
             Note that the Message object in this field will not contain further
             ``reply_to_message`` fields even if it itself is a reply.
         edit_date (:class:`datetime.datetime`, optional): Date the message was last edited in Unix
             time. Converted to :class:`datetime.datetime`.
+
+            .. versionchanged:: 20.3
+                |datetime_localization|
         has_protected_content (:obj:`bool`, optional): :obj:`True`, if the message can't be
             forwarded.
 
             .. versionadded:: 13.9
         media_group_id (:obj:`str`, optional): The unique identifier of a media message group this
             message belongs to.
         text (:obj:`str`, optional): For text messages, the actual UTF-8 text of the message,
@@ -335,32 +345,41 @@
             chat. For example, the channel itself for channel posts, the supergroup itself for
             messages from anonymous group administrators, the linked channel for messages
             automatically forwarded to the discussion group. For backward compatibility,
             :attr:`from_user` contains a fake sender user in non-channel chats, if the message was
             sent on behalf of a chat.
         date (:class:`datetime.datetime`): Date the message was sent in Unix time. Converted to
             :class:`datetime.datetime`.
+
+            .. versionchanged:: 20.3
+                |datetime_localization|
         chat (:class:`telegram.Chat`): Conversation the message belongs to.
         forward_from (:class:`telegram.User`): Optional. For forwarded messages, sender of the
             original message.
         forward_from_chat (:class:`telegram.Chat`): Optional. For messages forwarded from channels
             or from anonymous administrators, information about the original sender chat.
         forward_from_message_id (:obj:`int`): Optional. For forwarded channel posts, identifier of
             the original message in the channel.
         forward_date (:class:`datetime.datetime`): Optional. For forwarded messages, date the
             original message was sent in Unix time. Converted to :class:`datetime.datetime`.
+
+            .. versionchanged:: 20.3
+                |datetime_localization|
         is_automatic_forward (:obj:`bool`): Optional. :obj:`True`, if the message is a channel
             post that was automatically forwarded to the connected discussion group.
 
             .. versionadded:: 13.9
         reply_to_message (:class:`telegram.Message`): Optional. For replies, the original message.
             Note that the Message object in this field will not contain further
             ``reply_to_message`` fields even if it itself is a reply.
         edit_date (:class:`datetime.datetime`): Optional. Date the message was last edited in Unix
             time. Converted to :class:`datetime.datetime`.
+
+            .. versionchanged:: 20.3
+                |datetime_localization|
         has_protected_content (:obj:`bool`): Optional. :obj:`True`, if the message can't be
             forwarded.
 
             .. versionadded:: 13.9
         media_group_id (:obj:`str`): Optional. The unique identifier of a media message group this
             message belongs to.
         text (:obj:`str`): Optional. For text messages, the actual UTF-8 text of the message,
@@ -557,16 +576,21 @@
 
             .. versionadded:: 20.1
         chat_shared (:class:`telegram.ChatShared`): Optional. Service message: a chat was shared
             with the bot.
 
             .. versionadded:: 20.1
 
-    .. |custom_emoji_formatting_note| replace:: Custom emoji entities will currently be ignored
-        by this function. Instead, the supplied replacement for the emoji will be used.
+    .. |custom_emoji_formatting_note| replace:: Custom emoji entities will be ignored by this
+        function. Instead, the supplied replacement for the emoji will be used.
+
+    .. |custom_emoji_md1_deprecation| replace:: Since custom emoji entities are not supported by
+       :attr:`~telegram.constants.ParseMode.MARKDOWN`, this method will raise a
+       :exc:`ValueError` in future versions instead of falling back to the supplied replacement
+       for the emoji.
     """
 
     # fmt: on
     __slots__ = (
         "reply_markup",
         "audio",
         "contact",
@@ -823,43 +847,52 @@
         """
         return self.message_id
 
     @property
     def link(self) -> Optional[str]:
         """:obj:`str`: Convenience property. If the chat of the message is not
         a private chat or normal group, returns a t.me link of the message.
+
+            .. versionchanged:: 20.3
+                For messages that are replies or part of a forum topic, the link now points
+                to the corresponding thread view.
         """
         if self.chat.type not in [Chat.PRIVATE, Chat.GROUP]:
-            if self.chat.username:
-                to_link = self.chat.username
-            else:
-                # Get rid of leading -100 for supergroups
-                to_link = f"c/{str(self.chat.id)[4:]}"
-            return f"https://t.me/{to_link}/{self.message_id}"
+            # the else block gets rid of leading -100 for supergroups:
+            to_link = self.chat.username if self.chat.username else f"c/{str(self.chat.id)[4:]}"
+            baselink = f"https://t.me/{to_link}/{self.message_id}"
+
+            # adds the thread for topics and replies
+            if (self.is_topic_message and self.message_thread_id) or self.reply_to_message:
+                baselink = f"{baselink}?thread={self.message_thread_id}"
+            return baselink
         return None
 
     @classmethod
     def de_json(cls, data: Optional[JSONDict], bot: "Bot") -> Optional["Message"]:
         """See :meth:`telegram.TelegramObject.de_json`."""
         data = cls._parse_data(data)
 
         if not data:
             return None
 
+        # Get the local timezone from the bot if it has defaults
+        loc_tzinfo = extract_tzinfo_from_defaults(bot)
+
         data["from_user"] = User.de_json(data.pop("from", None), bot)
         data["sender_chat"] = Chat.de_json(data.get("sender_chat"), bot)
-        data["date"] = from_timestamp(data["date"])
+        data["date"] = from_timestamp(data["date"], tzinfo=loc_tzinfo)
         data["chat"] = Chat.de_json(data.get("chat"), bot)
         data["entities"] = MessageEntity.de_list(data.get("entities"), bot)
         data["caption_entities"] = MessageEntity.de_list(data.get("caption_entities"), bot)
         data["forward_from"] = User.de_json(data.get("forward_from"), bot)
         data["forward_from_chat"] = Chat.de_json(data.get("forward_from_chat"), bot)
-        data["forward_date"] = from_timestamp(data.get("forward_date"))
+        data["forward_date"] = from_timestamp(data.get("forward_date"), tzinfo=loc_tzinfo)
         data["reply_to_message"] = Message.de_json(data.get("reply_to_message"), bot)
-        data["edit_date"] = from_timestamp(data.get("edit_date"))
+        data["edit_date"] = from_timestamp(data.get("edit_date"), tzinfo=loc_tzinfo)
         data["audio"] = Audio.de_json(data.get("audio"), bot)
         data["document"] = Document.de_json(data.get("document"), bot)
         data["animation"] = Animation.de_json(data.get("animation"), bot)
         data["game"] = Game.de_json(data.get("game"), bot)
         data["photo"] = PhotoSize.de_list(data.get("photo"), bot)
         data["sticker"] = Sticker.de_json(data.get("sticker"), bot)
         data["video"] = Video.de_json(data.get("video"), bot)
@@ -3133,18 +3166,14 @@
         Raises:
             RuntimeError: If the message has no text.
 
         """
         if not self.text:
             raise RuntimeError("This Message has no 'text'.")
 
-        # Is it a narrow build, if so we don't need to convert
-        if sys.maxunicode == 0xFFFF:
-            return self.text[entity.offset : entity.offset + entity.length]
-
         entity_text = self.text.encode("utf-16-le")
         entity_text = entity_text[entity.offset * 2 : (entity.offset + entity.length) * 2]
         return entity_text.decode("utf-16-le")
 
     def parse_caption_entity(self, entity: MessageEntity) -> str:
         """Returns the text from a given :class:`telegram.MessageEntity`.
 
@@ -3163,18 +3192,14 @@
         Raises:
             RuntimeError: If the message has no caption.
 
         """
         if not self.caption:
             raise RuntimeError("This Message has no 'caption'.")
 
-        # Is it a narrow build, if so we don't need to convert
-        if sys.maxunicode == 0xFFFF:
-            return self.caption[entity.offset : entity.offset + entity.length]
-
         entity_text = self.caption.encode("utf-16-le")
         entity_text = entity_text[entity.offset * 2 : (entity.offset + entity.length) * 2]
         return entity_text.decode("utf-16-le")
 
     def parse_entities(self, types: List[str] = None) -> Dict[MessageEntity, str]:
         """
         Returns a :obj:`dict` that maps :class:`telegram.MessageEntity` to :obj:`str`.
@@ -3243,16 +3268,15 @@
         entities: Dict[MessageEntity, str],
         urled: bool = False,
         offset: int = 0,
     ) -> Optional[str]:
         if message_text is None:
             return None
 
-        if sys.maxunicode != 0xFFFF:
-            message_text = message_text.encode("utf-16-le")  # type: ignore
+        message_text = message_text.encode("utf-16-le")  # type: ignore
 
         html_text = ""
         last_offset = 0
 
         sorted_entities = sorted(entities.items(), key=lambda item: item[0].offset)
         parsed_entities = []
 
@@ -3264,160 +3288,152 @@
                     if e.offset >= entity.offset
                     and e.offset + e.length <= entity.offset + entity.length
                     and e != entity
                 }
                 parsed_entities.extend(list(nested_entities.keys()))
 
                 orig_text = text
-                text = escape(text)
+                escaped_text = escape(text)
 
                 if nested_entities:
-                    text = Message._parse_html(
+                    escaped_text = Message._parse_html(
                         orig_text, nested_entities, urled=urled, offset=entity.offset
                     )
 
                 if entity.type == MessageEntity.TEXT_LINK:
-                    insert = f'<a href="{entity.url}">{text}</a>'
+                    insert = f'<a href="{entity.url}">{escaped_text}</a>'
                 elif entity.type == MessageEntity.TEXT_MENTION and entity.user:
-                    insert = f'<a href="tg://user?id={entity.user.id}">{text}</a>'
+                    insert = f'<a href="tg://user?id={entity.user.id}">{escaped_text}</a>'
                 elif entity.type == MessageEntity.URL and urled:
-                    insert = f'<a href="{text}">{text}</a>'
+                    insert = f'<a href="{escaped_text}">{escaped_text}</a>'
                 elif entity.type == MessageEntity.BOLD:
-                    insert = f"<b>{text}</b>"
+                    insert = f"<b>{escaped_text}</b>"
                 elif entity.type == MessageEntity.ITALIC:
-                    insert = f"<i>{text}</i>"
+                    insert = f"<i>{escaped_text}</i>"
                 elif entity.type == MessageEntity.CODE:
-                    insert = f"<code>{text}</code>"
+                    insert = f"<code>{escaped_text}</code>"
                 elif entity.type == MessageEntity.PRE:
                     if entity.language:
-                        insert = f'<pre><code class="{entity.language}">{text}</code></pre>'
+                        insert = (
+                            f'<pre><code class="{entity.language}">{escaped_text}</code></pre>'
+                        )
                     else:
-                        insert = f"<pre>{text}</pre>"
+                        insert = f"<pre>{escaped_text}</pre>"
                 elif entity.type == MessageEntity.UNDERLINE:
-                    insert = f"<u>{text}</u>"
+                    insert = f"<u>{escaped_text}</u>"
                 elif entity.type == MessageEntity.STRIKETHROUGH:
-                    insert = f"<s>{text}</s>"
+                    insert = f"<s>{escaped_text}</s>"
                 elif entity.type == MessageEntity.SPOILER:
-                    insert = f'<span class="tg-spoiler">{text}</span>'
+                    insert = f'<span class="tg-spoiler">{escaped_text}</span>'
+                elif entity.type == MessageEntity.CUSTOM_EMOJI:
+                    insert = (
+                        f'<tg-emoji emoji-id="{entity.custom_emoji_id}">{escaped_text}</tg-emoji>'
+                    )
                 else:
-                    insert = text
+                    insert = escaped_text
 
                 if offset == 0:
-                    if sys.maxunicode == 0xFFFF:
-                        html_text += (
-                            escape(message_text[last_offset : entity.offset - offset]) + insert
-                        )
-                    else:
-                        html_text += (
-                            escape(
-                                message_text[  # type: ignore
-                                    last_offset * 2 : (entity.offset - offset) * 2
-                                ].decode("utf-16-le")
-                            )
-                            + insert
-                        )
-                else:
-                    if sys.maxunicode == 0xFFFF:
-                        html_text += message_text[last_offset : entity.offset - offset] + insert
-                    else:
-                        html_text += (
+                    html_text += (
+                        escape(
                             message_text[  # type: ignore
                                 last_offset * 2 : (entity.offset - offset) * 2
                             ].decode("utf-16-le")
-                            + insert
                         )
+                        + insert
+                    )
+                else:
+                    html_text += (
+                        message_text[  # type: ignore
+                            last_offset * 2 : (entity.offset - offset) * 2
+                        ].decode("utf-16-le")
+                        + insert
+                    )
 
                 last_offset = entity.offset - offset + entity.length
 
         if offset == 0:
-            if sys.maxunicode == 0xFFFF:
-                html_text += escape(message_text[last_offset:])
-            else:
-                html_text += escape(
-                    message_text[last_offset * 2 :].decode("utf-16-le")  # type: ignore
-                )
+            html_text += escape(
+                message_text[last_offset * 2 :].decode("utf-16-le")  # type: ignore
+            )
         else:
-            if sys.maxunicode == 0xFFFF:
-                html_text += message_text[last_offset:]
-            else:
-                html_text += message_text[last_offset * 2 :].decode("utf-16-le")  # type: ignore
+            html_text += message_text[last_offset * 2 :].decode("utf-16-le")  # type: ignore
 
         return html_text
 
     @property
     def text_html(self) -> str:
         """Creates an HTML-formatted string from the markup entities found in the message.
 
         Use this if you want to retrieve the message text with the entities formatted as HTML in
         the same way the original message was formatted.
 
-        Note:
-            |custom_emoji_formatting_note|
-
         .. versionchanged:: 13.10
            Spoiler entities are now formatted as HTML.
 
+        .. versionchanged:: 20.3
+           Custom emoji entities are now supported.
+
         Returns:
             :obj:`str`: Message text with entities formatted as HTML.
 
         """
         return self._parse_html(self.text, self.parse_entities(), urled=False)
 
     @property
     def text_html_urled(self) -> str:
         """Creates an HTML-formatted string from the markup entities found in the message.
 
         Use this if you want to retrieve the message text with the entities formatted as HTML.
         This also formats :attr:`telegram.MessageEntity.URL` as a hyperlink.
 
-        Note:
-            |custom_emoji_formatting_note|
-
         .. versionchanged:: 13.10
            Spoiler entities are now formatted as HTML.
 
+        .. versionchanged:: 20.3
+           Custom emoji entities are now supported.
+
         Returns:
             :obj:`str`: Message text with entities formatted as HTML.
 
         """
         return self._parse_html(self.text, self.parse_entities(), urled=True)
 
     @property
     def caption_html(self) -> str:
         """Creates an HTML-formatted string from the markup entities found in the message's
         caption.
 
         Use this if you want to retrieve the message caption with the caption entities formatted as
         HTML in the same way the original message was formatted.
 
-        Note:
-            |custom_emoji_formatting_note|
-
         .. versionchanged:: 13.10
            Spoiler entities are now formatted as HTML.
 
+        .. versionchanged:: 20.3
+           Custom emoji entities are now supported.
+
         Returns:
             :obj:`str`: Message caption with caption entities formatted as HTML.
         """
         return self._parse_html(self.caption, self.parse_caption_entities(), urled=False)
 
     @property
     def caption_html_urled(self) -> str:
         """Creates an HTML-formatted string from the markup entities found in the message's
         caption.
 
         Use this if you want to retrieve the message caption with the caption entities formatted as
         HTML. This also formats :attr:`telegram.MessageEntity.URL` as a hyperlink.
 
-        Note:
-            |custom_emoji_formatting_note|
-
         .. versionchanged:: 13.10
            Spoiler entities are now formatted as HTML.
 
+        .. versionchanged:: 20.3
+           Custom emoji entities are now supported.
+
         Returns:
             :obj:`str`: Message caption with caption entities formatted as HTML.
         """
         return self._parse_html(self.caption, self.parse_caption_entities(), urled=True)
 
     @staticmethod
     def _parse_markdown(
@@ -3428,16 +3444,15 @@
         offset: int = 0,
     ) -> Optional[str]:
         version = int(version)
 
         if message_text is None:
             return None
 
-        if sys.maxunicode != 0xFFFF:
-            message_text = message_text.encode("utf-16-le")  # type: ignore
+        message_text = message_text.encode("utf-16-le")  # type: ignore
 
         markdown_text = ""
         last_offset = 0
 
         sorted_entities = sorted(entities.items(), key=lambda item: item[0].offset)
         parsed_entities = []
 
@@ -3448,138 +3463,130 @@
                     for (e, t) in sorted_entities
                     if e.offset >= entity.offset
                     and e.offset + e.length <= entity.offset + entity.length
                     and e != entity
                 }
                 parsed_entities.extend(list(nested_entities.keys()))
 
-                orig_text = text
-                text = escape_markdown(text, version=version)
+                escaped_text = escape_markdown(text, version=version)
 
                 if nested_entities:
                     if version < 2:
                         raise ValueError(
                             "Nested entities are not supported for Markdown version 1"
                         )
 
-                    text = Message._parse_markdown(
-                        orig_text,
+                    escaped_text = Message._parse_markdown(
+                        text,
                         nested_entities,
                         urled=urled,
                         offset=entity.offset,
                         version=version,
                     )
 
                 if entity.type == MessageEntity.TEXT_LINK:
                     if version == 1:
                         url = entity.url
                     else:
                         # Links need special escaping. Also can't have entities nested within
                         url = escape_markdown(
                             entity.url, version=version, entity_type=MessageEntity.TEXT_LINK
                         )
-                    insert = f"[{text}]({url})"
+                    insert = f"[{escaped_text}]({url})"
                 elif entity.type == MessageEntity.TEXT_MENTION and entity.user:
-                    insert = f"[{text}](tg://user?id={entity.user.id})"
+                    insert = f"[{escaped_text}](tg://user?id={entity.user.id})"
                 elif entity.type == MessageEntity.URL and urled:
-                    if version == 1:
-                        link = orig_text
-                    else:
-                        link = text
-                    insert = f"[{link}]({orig_text})"
+                    link = text if version == 1 else escaped_text
+                    insert = f"[{link}]({text})"
                 elif entity.type == MessageEntity.BOLD:
-                    insert = f"*{text}*"
+                    insert = f"*{escaped_text}*"
                 elif entity.type == MessageEntity.ITALIC:
-                    insert = f"_{text}_"
+                    insert = f"_{escaped_text}_"
                 elif entity.type == MessageEntity.CODE:
                     # Monospace needs special escaping. Also can't have entities nested within
-                    insert = f"`{escape_markdown(orig_text, version, MessageEntity.CODE)}`"
+                    insert = f"`{escape_markdown(text, version, MessageEntity.CODE)}`"
 
                 elif entity.type == MessageEntity.PRE:
                     # Monospace needs special escaping. Also can't have entities nested within
-                    code = escape_markdown(
-                        orig_text, version=version, entity_type=MessageEntity.PRE
-                    )
+                    code = escape_markdown(text, version=version, entity_type=MessageEntity.PRE)
                     if entity.language:
                         prefix = f"```{entity.language}\n"
+                    elif code.startswith("\\"):
+                        prefix = "```"
                     else:
-                        if code.startswith("\\"):
-                            prefix = "```"
-                        else:
-                            prefix = "```\n"
+                        prefix = "```\n"
                     insert = f"{prefix}{code}```"
                 elif entity.type == MessageEntity.UNDERLINE:
                     if version == 1:
                         raise ValueError(
                             "Underline entities are not supported for Markdown version 1"
                         )
-                    insert = f"__{text}__"
+                    insert = f"__{escaped_text}__"
                 elif entity.type == MessageEntity.STRIKETHROUGH:
                     if version == 1:
                         raise ValueError(
                             "Strikethrough entities are not supported for Markdown version 1"
                         )
-                    insert = f"~{text}~"
+                    insert = f"~{escaped_text}~"
                 elif entity.type == MessageEntity.SPOILER:
                     if version == 1:
                         raise ValueError(
                             "Spoiler entities are not supported for Markdown version 1"
                         )
-                    insert = f"||{text}||"
-                else:
-                    insert = text
-
-                if offset == 0:
-                    if sys.maxunicode == 0xFFFF:
-                        markdown_text += (
-                            escape_markdown(
-                                message_text[last_offset : entity.offset - offset], version=version
-                            )
-                            + insert
+                    insert = f"||{escaped_text}||"
+                elif entity.type == MessageEntity.CUSTOM_EMOJI:
+                    if version == 1:
+                        # this ensures compatibility to previous PTB versions
+                        insert = escaped_text
+                        warn(
+                            "Custom emoji entities are not supported for Markdown version 1. "
+                            "Future version of PTB will raise a ValueError instead of falling "
+                            "back to the alternative standard emoji.",
+                            stacklevel=3,
+                            category=PTBDeprecationWarning,
                         )
                     else:
-                        markdown_text += (
-                            escape_markdown(
-                                message_text[  # type: ignore
-                                    last_offset * 2 : (entity.offset - offset) * 2
-                                ].decode("utf-16-le"),
-                                version=version,
-                            )
-                            + insert
+                        # This should never be needed because ids are numeric but the documentation
+                        # specifically mentions it so here we are
+                        custom_emoji_id = escape_markdown(
+                            entity.custom_emoji_id,
+                            version=version,
+                            entity_type=MessageEntity.CUSTOM_EMOJI,
                         )
+                        insert = f"![{escaped_text}](tg://emoji?id={custom_emoji_id})"
                 else:
-                    if sys.maxunicode == 0xFFFF:
-                        markdown_text += (
-                            message_text[last_offset : entity.offset - offset] + insert
-                        )
-                    else:
-                        markdown_text += (
+                    insert = escaped_text
+
+                if offset == 0:
+                    markdown_text += (
+                        escape_markdown(
                             message_text[  # type: ignore
                                 last_offset * 2 : (entity.offset - offset) * 2
-                            ].decode("utf-16-le")
-                            + insert
+                            ].decode("utf-16-le"),
+                            version=version,
                         )
+                        + insert
+                    )
+                else:
+                    markdown_text += (
+                        message_text[  # type: ignore
+                            last_offset * 2 : (entity.offset - offset) * 2
+                        ].decode("utf-16-le")
+                        + insert
+                    )
 
                 last_offset = entity.offset - offset + entity.length
 
         if offset == 0:
-            if sys.maxunicode == 0xFFFF:
-                markdown_text += escape_markdown(message_text[last_offset:], version=version)
-            else:
-                markdown_text += escape_markdown(
-                    message_text[last_offset * 2 :].decode("utf-16-le"),  # type: ignore
-                    version=version,
-                )
+            markdown_text += escape_markdown(
+                message_text[last_offset * 2 :].decode("utf-16-le"),  # type: ignore
+                version=version,
+            )
         else:
-            if sys.maxunicode == 0xFFFF:
-                markdown_text += message_text[last_offset:]
-            else:
-                markdown_text += message_text[last_offset * 2 :].decode(  # type: ignore
-                    "utf-16-le"
-                )
+            markdown_text += message_text[last_offset * 2 :].decode("utf-16-le")  # type: ignore
 
         return markdown_text
 
     @property
     def text_markdown(self) -> str:
         """Creates an Markdown-formatted string from the markup entities found in the message
         using :class:`telegram.constants.ParseMode.MARKDOWN`.
@@ -3590,14 +3597,17 @@
         Note:
             * :tg-const:`telegram.constants.ParseMode.MARKDOWN` is a legacy mode, retained by
               Telegram for backward compatibility. You should use
               :meth:`text_markdown_v2` instead.
 
             * |custom_emoji_formatting_note|
 
+        .. deprecated:: 20.3
+            |custom_emoji_md1_deprecation|
+
         Returns:
             :obj:`str`: Message text with entities formatted as Markdown.
 
         Raises:
             :exc:`ValueError`: If the message contains underline, strikethrough, spoiler or nested
                 entities.
 
@@ -3608,20 +3618,20 @@
     def text_markdown_v2(self) -> str:
         """Creates an Markdown-formatted string from the markup entities found in the message
         using :class:`telegram.constants.ParseMode.MARKDOWN_V2`.
 
         Use this if you want to retrieve the message text with the entities formatted as Markdown
         in the same way the original message was formatted.
 
-        Note:
-            |custom_emoji_formatting_note|
-
         .. versionchanged:: 13.10
            Spoiler entities are now formatted as Markdown V2.
 
+        .. versionchanged:: 20.3
+           Custom emoji entities are now supported.
+
         Returns:
             :obj:`str`: Message text with entities formatted as Markdown.
         """
         return self._parse_markdown(self.text, self.parse_entities(), urled=False, version=2)
 
     @property
     def text_markdown_urled(self) -> str:
@@ -3634,14 +3644,17 @@
         Note:
             * :tg-const:`telegram.constants.ParseMode.MARKDOWN` is a legacy mode, retained by
               Telegram for backward compatibility. You should use :meth:`text_markdown_v2_urled`
               instead.
 
             * |custom_emoji_formatting_note|
 
+        .. deprecated:: 20.3
+            |custom_emoji_md1_deprecation|
+
         Returns:
             :obj:`str`: Message text with entities formatted as Markdown.
 
         Raises:
             :exc:`ValueError`: If the message contains underline, strikethrough, spoiler or nested
                 entities.
 
@@ -3652,20 +3665,20 @@
     def text_markdown_v2_urled(self) -> str:
         """Creates an Markdown-formatted string from the markup entities found in the message
         using :class:`telegram.constants.ParseMode.MARKDOWN_V2`.
 
         Use this if you want to retrieve the message text with the entities formatted as Markdown.
         This also formats :attr:`telegram.MessageEntity.URL` as a hyperlink.
 
-        Note:
-            |custom_emoji_formatting_note|
-
         .. versionchanged:: 13.10
            Spoiler entities are now formatted as Markdown V2.
 
+        .. versionchanged:: 20.3
+           Custom emoji entities are now supported.
+
         Returns:
             :obj:`str`: Message text with entities formatted as Markdown.
         """
         return self._parse_markdown(self.text, self.parse_entities(), urled=True, version=2)
 
     @property
     def caption_markdown(self) -> str:
@@ -3678,14 +3691,17 @@
         Note:
             * :tg-const:`telegram.constants.ParseMode.MARKDOWN` is a legacy mode, retained by
               Telegram for backward compatibility. You should use :meth:`caption_markdown_v2`
               instead.
 
             * |custom_emoji_formatting_note|
 
+        .. deprecated:: 20.3
+            |custom_emoji_md1_deprecation|
+
         Returns:
             :obj:`str`: Message caption with caption entities formatted as Markdown.
 
         Raises:
             :exc:`ValueError`: If the message contains underline, strikethrough, spoiler or nested
                 entities.
 
@@ -3696,20 +3712,20 @@
     def caption_markdown_v2(self) -> str:
         """Creates an Markdown-formatted string from the markup entities found in the message's
         caption using :class:`telegram.constants.ParseMode.MARKDOWN_V2`.
 
         Use this if you want to retrieve the message caption with the caption entities formatted as
         Markdown in the same way the original message was formatted.
 
-        Note:
-            |custom_emoji_formatting_note|
-
         .. versionchanged:: 13.10
            Spoiler entities are now formatted as Markdown V2.
 
+        .. versionchanged:: 20.3
+           Custom emoji entities are now supported.
+
         Returns:
             :obj:`str`: Message caption with caption entities formatted as Markdown.
         """
         return self._parse_markdown(
             self.caption, self.parse_caption_entities(), urled=False, version=2
         )
 
@@ -3724,14 +3740,17 @@
         Note:
             * :tg-const:`telegram.constants.ParseMode.MARKDOWN` is a legacy mode, retained by
               Telegram for backward compatibility. You should use
               :meth:`caption_markdown_v2_urled` instead.
 
             * |custom_emoji_formatting_note|
 
+        .. deprecated:: 20.3
+            |custom_emoji_md1_deprecation|
+
         Returns:
             :obj:`str`: Message caption with caption entities formatted as Markdown.
 
         Raises:
             :exc:`ValueError`: If the message contains underline, strikethrough, spoiler or nested
                 entities.
 
@@ -3742,19 +3761,19 @@
     def caption_markdown_v2_urled(self) -> str:
         """Creates an Markdown-formatted string from the markup entities found in the message's
         caption using :class:`telegram.constants.ParseMode.MARKDOWN_V2`.
 
         Use this if you want to retrieve the message caption with the caption entities formatted as
         Markdown. This also formats :attr:`telegram.MessageEntity.URL` as a hyperlink.
 
-        Note:
-            |custom_emoji_formatting_note|
-
         .. versionchanged:: 13.10
            Spoiler entities are now formatted as Markdown V2.
 
+        .. versionchanged:: 20.3
+           Custom emoji entities are now supported.
+
         Returns:
             :obj:`str`: Message caption with caption entities formatted as Markdown.
         """
         return self._parse_markdown(
             self.caption, self.parse_caption_entities(), urled=True, version=2
         )
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_messageautodeletetimerchanged.py` & `python-telegram-bot-raw-20.3/telegram/_messageautodeletetimerchanged.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_messageentity.py` & `python-telegram-bot-raw-20.3/telegram/_messageentity.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_messageid.py` & `python-telegram-bot-raw-20.3/telegram/_messageid.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_passport/credentials.py` & `python-telegram-bot-raw-20.3/telegram/_passport/credentials.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_passport/data.py` & `python-telegram-bot-raw-20.3/telegram/_passport/data.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_passport/encryptedpassportelement.py` & `python-telegram-bot-raw-20.3/telegram/_passport/encryptedpassportelement.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_passport/passportdata.py` & `python-telegram-bot-raw-20.3/telegram/_passport/passportdata.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_passport/passportelementerrors.py` & `python-telegram-bot-raw-20.3/telegram/_passport/passportelementerrors.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
 
     def __init__(self, type: str, file_hashes: str, message: str, *, api_kwargs: JSONDict = None):
         # Required
         super().__init__("files", type, message, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.file_hashes: str = file_hashes
 
-            self._id_attrs = (self.source, self.type, self.message) + tuple(file_hashes)
+            self._id_attrs = (self.source, self.type, self.message, *tuple(file_hashes))
 
 
 class PassportElementErrorFrontSide(PassportElementError):
     """
     Represents an issue with the front side of a document. The error is considered resolved when
     the file with the front side of the document changes.
 
@@ -358,15 +358,15 @@
 
     def __init__(self, type: str, file_hashes: str, message: str, *, api_kwargs: JSONDict = None):
         # Required
         super().__init__("translation_files", type, message, api_kwargs=api_kwargs)
         with self._unfrozen():
             self.file_hashes: str = file_hashes
 
-            self._id_attrs = (self.source, self.type, self.message) + tuple(file_hashes)
+            self._id_attrs = (self.source, self.type, self.message, *tuple(file_hashes))
 
 
 class PassportElementErrorUnspecified(PassportElementError):
     """
     Represents an issue in an unspecified place. The error is considered resolved when new
     data is added.
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_passport/passportfile.py` & `python-telegram-bot-raw-20.3/telegram/_passport/passportfile.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_payment/invoice.py` & `python-telegram-bot-raw-20.3/telegram/_payment/invoice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_payment/labeledprice.py` & `python-telegram-bot-raw-20.3/telegram/_payment/labeledprice.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_payment/orderinfo.py` & `python-telegram-bot-raw-20.3/telegram/_payment/orderinfo.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_payment/precheckoutquery.py` & `python-telegram-bot-raw-20.3/telegram/_payment/precheckoutquery.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_payment/shippingaddress.py` & `python-telegram-bot-raw-20.3/telegram/_payment/shippingaddress.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_payment/shippingoption.py` & `python-telegram-bot-raw-20.3/telegram/_payment/shippingoption.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from typing import TYPE_CHECKING, Sequence, Tuple
 
 from telegram._telegramobject import TelegramObject
 from telegram._utils.argumentparsing import parse_sequence_arg
 from telegram._utils.types import JSONDict
 
 if TYPE_CHECKING:
-    from telegram import LabeledPrice  # noqa
+    from telegram import LabeledPrice
 
 
 class ShippingOption(TelegramObject):
     """This object represents one shipping option.
 
     Objects of this class are comparable in terms of equality. Two objects of this class are
     considered equal, if their :attr:`id` is equal.
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_payment/shippingquery.py` & `python-telegram-bot-raw-20.3/telegram/_payment/shippingquery.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_payment/successfulpayment.py` & `python-telegram-bot-raw-20.3/telegram/_payment/successfulpayment.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_poll.py` & `python-telegram-bot-raw-20.3/telegram/_poll.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,24 +14,23 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram Poll."""
 import datetime
-import sys
 from typing import TYPE_CHECKING, ClassVar, Dict, List, Optional, Sequence, Tuple
 
 from telegram import constants
 from telegram._messageentity import MessageEntity
 from telegram._telegramobject import TelegramObject
 from telegram._user import User
 from telegram._utils import enum
 from telegram._utils.argumentparsing import parse_sequence_arg
-from telegram._utils.datetime import from_timestamp
+from telegram._utils.datetime import extract_tzinfo_from_defaults, from_timestamp
 from telegram._utils.types import JSONDict
 
 if TYPE_CHECKING:
     from telegram import Bot
 
 
 class PollOption(TelegramObject):
@@ -170,14 +169,17 @@
                * This attribute is now always a (possibly empty) list and never :obj:`None`.
                * |sequenceclassargs|
         open_period (:obj:`int`, optional): Amount of time in seconds the poll will be active
             after creation.
         close_date (:obj:`datetime.datetime`, optional): Point in time (Unix timestamp) when the
             poll will be automatically closed. Converted to :obj:`datetime.datetime`.
 
+            .. versionchanged:: 20.3
+                |datetime_localization|
+
     Attributes:
         id (:obj:`str`): Unique poll identifier.
         question (:obj:`str`): Poll question, :tg-const:`telegram.Poll.MIN_QUESTION_LENGTH`-
             :tg-const:`telegram.Poll.MAX_QUESTION_LENGTH` characters.
         options (Tuple[:class:`~telegram.PollOption`]): List of poll options.
 
             .. versionchanged:: 20.0
@@ -203,14 +205,17 @@
             .. versionchanged:: 20.0
                This attribute is now always a (possibly empty) list and never :obj:`None`.
         open_period (:obj:`int`): Optional. Amount of time in seconds the poll will be active
             after creation.
         close_date (:obj:`datetime.datetime`): Optional. Point in time when the poll will be
             automatically closed.
 
+            .. versionchanged:: 20.3
+                |datetime_localization|
+
     """
 
     __slots__ = (
         "total_voter_count",
         "allows_multiple_answers",
         "open_period",
         "options",
@@ -268,17 +273,20 @@
     def de_json(cls, data: Optional[JSONDict], bot: "Bot") -> Optional["Poll"]:
         """See :meth:`telegram.TelegramObject.de_json`."""
         data = cls._parse_data(data)
 
         if not data:
             return None
 
+        # Get the local timezone from the bot if it has defaults
+        loc_tzinfo = extract_tzinfo_from_defaults(bot)
+
         data["options"] = [PollOption.de_json(option, bot) for option in data["options"]]
         data["explanation_entities"] = MessageEntity.de_list(data.get("explanation_entities"), bot)
-        data["close_date"] = from_timestamp(data.get("close_date"))
+        data["close_date"] = from_timestamp(data.get("close_date"), tzinfo=loc_tzinfo)
 
         return super().de_json(data=data, bot=bot)
 
     def parse_explanation_entity(self, entity: MessageEntity) -> str:
         """Returns the text from a given :class:`telegram.MessageEntity`.
 
         Note:
@@ -296,17 +304,14 @@
         Raises:
             RuntimeError: If the poll has no explanation.
 
         """
         if not self.explanation:
             raise RuntimeError("This Poll has no 'explanation'.")
 
-        # Is it a narrow build, if so we don't need to convert
-        if sys.maxunicode == 0xFFFF:
-            return self.explanation[entity.offset : entity.offset + entity.length]
         entity_text = self.explanation.encode("utf-16-le")
         entity_text = entity_text[entity.offset * 2 : (entity.offset + entity.length) * 2]
 
         return entity_text.decode("utf-16-le")
 
     def parse_explanation_entities(self, types: List[str] = None) -> Dict[MessageEntity, str]:
         """
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_proximityalerttriggered.py` & `python-telegram-bot-raw-20.3/telegram/_proximityalerttriggered.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_replykeyboardmarkup.py` & `python-telegram-bot-raw-20.3/telegram/_replykeyboardmarkup.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_replykeyboardremove.py` & `python-telegram-bot-raw-20.3/telegram/_replykeyboardremove.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_sentwebappmessage.py` & `python-telegram-bot-raw-20.3/telegram/_sentwebappmessage.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_shared.py` & `python-telegram-bot-raw-20.3/telegram/_shared.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_telegramobject.py` & `python-telegram-bot-raw-20.3/telegram/_telegramobject.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,14 +54,20 @@
 class TelegramObject:
     """Base class for most Telegram objects.
 
     Objects of this type are subscriptable with strings. See :meth:`__getitem__` for more details.
     The :mod:`pickle` and :func:`~copy.deepcopy` behavior of objects of this type are defined by
     :meth:`__getstate__`, :meth:`__setstate__` and :meth:`__deepcopy__`.
 
+    Tip:
+        Objects of this type can be serialized via Python's :mod:`pickle` module and pickled
+        objects from one version of PTB are usually loadable in future versions. However, we can
+        not guarantee that this compatibility will always be provided. At least a manual one-time
+        conversion of the data may be needed on major updates of the library.
+
     .. versionchanged:: 20.0
 
         * Removed argument and attribute ``bot`` for several subclasses. Use
           :meth:`set_bot` and :meth:`get_bot` instead.
         * Removed the possibility to pass arbitrary keyword arguments for several subclasses.
         * String representations objects of this type was overhauled. See :meth:`__repr__` for
           details. As this class doesn't implement :meth:`object.__str__`, the default
@@ -277,15 +283,15 @@
         Args:
             state (:obj:`dict`): The data to set as attributes of this object.
         """
         self._unfreeze()
 
         # Make sure that we have a `_bot` attribute. This is necessary, since __getstate__ omits
         # this as Bots are not pickable.
-        setattr(self, "_bot", None)
+        self._bot = None
 
         # get api_kwargs first because we may need to add entries to it (see try-except below)
         api_kwargs = cast(Dict[str, object], state.pop("api_kwargs", {}))
         # get _frozen before the loop to avoid setting it to True in the loop
         frozen = state.pop("_frozen", False)
 
         for key, val in state.items():
@@ -295,15 +301,15 @@
                 # catch cases when old attributes are removed from new versions
                 api_kwargs[key] = val  # add it to api_kwargs as fallback
 
         # For api_kwargs we first apply any kwargs that are already attributes of the object
         # and then set the rest as MappingProxyType attribute. Converting to MappingProxyType
         # is necessary, since __getstate__ converts it to a dict as MPT is not pickable.
         self._apply_api_kwargs(api_kwargs)
-        setattr(self, "api_kwargs", MappingProxyType(api_kwargs))
+        self.api_kwargs = MappingProxyType(api_kwargs)
 
         # Apply freezing if necessary
         # we .get(…) the setting for backwards compatibility with objects that were pickled
         # before the freeze feature was introduced
         if frozen:
             self._freeze()
 
@@ -324,15 +330,15 @@
         """
         bot = self._bot  # Save bot so we can set it after copying
         self.set_bot(None)  # set to None so it is not deepcopied
         cls = self.__class__
         result = cls.__new__(cls)  # create a new instance
         memodict[id(self)] = result  # save the id of the object in the dict
 
-        setattr(result, "_frozen", False)  # unfreeze the new object for setting the attributes
+        result._frozen = False  # unfreeze the new object for setting the attributes
 
         # now we set the attributes in the deepcopied object
         for k in self._get_attrs_names(include_private=True):
             if k == "_frozen":
                 # Setting the frozen status to True would prevent the attributes from being set
                 continue
             if k == "api_kwargs":
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_update.py` & `python-telegram-bot-raw-20.3/telegram/_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,27 +30,27 @@
 from telegram._payment.precheckoutquery import PreCheckoutQuery
 from telegram._payment.shippingquery import ShippingQuery
 from telegram._poll import Poll, PollAnswer
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 if TYPE_CHECKING:
-    from telegram import Bot, Chat, User  # noqa
+    from telegram import Bot, Chat, User
 
 
 class Update(TelegramObject):
     """This object represents an incoming update.
 
     Objects of this class are comparable in terms of equality. Two objects of this class are
     considered equal, if their :attr:`update_id` is equal.
 
     Note:
         At most one of the optional parameters can be present in any given update.
 
-    .. seealso:: :wiki:`Your First Bot <Extensions-–-Your-first-Bot>`
+    .. seealso:: :wiki:`Your First Bot <Extensions---Your-first-Bot>`
 
     Args:
         update_id (:obj:`int`): The update's unique identifier. Update identifiers start from a
             certain positive number and increase sequentially. This ID becomes especially handy if
             you're using Webhooks, since it allows you to ignore repeated updates or to restore the
             correct update sequence, should they get out of order. If there are no new updates for
             at least a week, then identifier of the next update will be chosen randomly instead of
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_user.py` & `python-telegram-bot-raw-20.3/telegram/_user.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_userprofilephotos.py` & `python-telegram-bot-raw-20.3/telegram/_userprofilephotos.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_utils/argumentparsing.py` & `python-telegram-bot-raw-20.3/telegram/_utils/argumentparsing.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_utils/datetime.py` & `python-telegram-bot-raw-20.3/telegram/_utils/datetime.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,18 @@
 Warning:
     Contents of this module are intended to be used internally by the library and *not* by the
     user. Changes to this module are not considered breaking changes and may not be documented in
     the changelog.
 """
 import datetime as dtm  # skipcq: PYL-W0406
 import time
-from typing import Optional, Union
+from typing import TYPE_CHECKING, Optional, Union
+
+if TYPE_CHECKING:
+    from telegram import Bot
 
 # pytz is only available if it was installed as dependency of APScheduler, so we make a little
 # workaround here
 DTM_UTC = dtm.timezone.utc
 try:
     import pytz
 
@@ -158,34 +161,48 @@
     return (
         int(to_float_timestamp(dt_obj, reference_timestamp, tzinfo))
         if dt_obj is not None
         else None
     )
 
 
-def from_timestamp(unixtime: Optional[int], tzinfo: dtm.tzinfo = UTC) -> Optional[dtm.datetime]:
+def from_timestamp(
+    unixtime: Optional[int],
+    tzinfo: Optional[dtm.tzinfo] = None,
+) -> Optional[dtm.datetime]:
     """
     Converts an (integer) unix timestamp to a timezone aware datetime object.
     :obj:`None` s are left alone (i.e. ``from_timestamp(None)`` is :obj:`None`).
 
     Args:
         unixtime (:obj:`int`): Integer POSIX timestamp.
         tzinfo (:obj:`datetime.tzinfo`, optional): The timezone to which the timestamp is to be
-            converted to. Defaults to UTC.
+            converted to. Defaults to :obj:`None`, in which case the returned datetime object will
+            be timezone aware and in UTC.
 
     Returns:
         Timezone aware equivalent :obj:`datetime.datetime` value if :paramref:`unixtime` is not
         :obj:`None`; else :obj:`None`.
     """
     if unixtime is None:
         return None
 
-    if tzinfo is not None:
-        return dtm.datetime.fromtimestamp(unixtime, tz=tzinfo)
-    return dtm.datetime.utcfromtimestamp(unixtime)
+    return dtm.datetime.fromtimestamp(unixtime, tz=UTC if tzinfo is None else tzinfo)
+
+
+def extract_tzinfo_from_defaults(bot: "Bot") -> Union[dtm.tzinfo, None]:
+    """
+    Extracts the timezone info from the default values of the bot.
+    If the bot has no default values, :obj:`None` is returned.
+    """
+    # We don't use `ininstance(bot, ExtBot)` here so that this works
+    # in `python-telegram-bot-raw` as well
+    if hasattr(bot, "defaults") and bot.defaults:
+        return bot.defaults.tzinfo
+    return None
 
 
 def _datetime_to_float_timestamp(dt_obj: dtm.datetime) -> float:
     """
     Converts a datetime object to a float timestamp (with sub-second precision).
     If the datetime object is timezone-naive, it is assumed to be in UTC.
     """
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_utils/defaultvalue.py` & `python-telegram-bot-raw-20.3/telegram/_utils/defaultvalue.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_utils/enum.py` & `python-telegram-bot-raw-20.3/telegram/_utils/enum.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_utils/files.py` & `python-telegram-bot-raw-20.3/telegram/_utils/files.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_utils/markup.py` & `python-telegram-bot-raw-20.3/telegram/_utils/markup.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_utils/types.py` & `python-telegram-bot-raw-20.3/telegram/_utils/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 """Generic type for bot method parameters which can have defaults. ``ODVInput[type]`` is the same
 as ``Optional[Union[DefaultValue[type], type, DefaultValue[None]]``."""
 DVInput = Union["DefaultValue[DVValueType]", DVValueType, "DefaultValue[None]"]
 """Generic type for bot method parameters which can have defaults. ``DVInput[type]`` is the same
 as ``Union[DefaultValue[type], type, DefaultValue[None]]``."""
 
 RT = TypeVar("RT")
-SCT = Union[RT, Collection[RT]]
+SCT = Union[RT, Collection[RT]]  # pylint: disable=invalid-name
 """Single instance or collection of instances."""
 
 ReplyMarkup = Union[
     "InlineKeyboardMarkup", "ReplyKeyboardMarkup", "ReplyKeyboardRemove", "ForceReply"
 ]
 """Type alias for reply markup objects.
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_utils/warnings.py` & `python-telegram-bot-raw-20.3/telegram/_utils/warnings.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_utils/warnings_transition.py` & `python-telegram-bot-raw-20.3/telegram/_utils/warnings_transition.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,30 +19,30 @@
 """This module contains functionality used for transition warnings issued by this library.
 
 It was created to prevent circular imports that would be caused by creating the warnings
 inside warnings.py.
 
 .. versionadded:: 20.2
 """
-import functools
-from typing import Any
+from typing import Any, Callable, Type
 
 from telegram._utils.warnings import warn
 from telegram.warnings import PTBDeprecationWarning
 
 
 # Narrower type hints will cause linting errors and/or circular imports.
 # We'll use `Any` here and put type hints in the calling code.
 def warn_about_deprecated_arg_return_new_arg(
     deprecated_arg: Any,
     new_arg: Any,
     deprecated_arg_name: str,
     new_arg_name: str,
     bot_api_version: str,
-    stacklevel: int = 3,
+    stacklevel: int = 2,
+    warn_callback: Callable[[str, Type[Warning], int], None] = warn,
 ) -> Any:
     """A helper function for the transition in API when argument is renamed.
 
     Checks the `deprecated_arg` and `new_arg` objects; warns if non-None `deprecated_arg` object
     was passed. Returns `new_arg` object (either the one originally passed by the user or the one
     that user passed as `deprecated_arg`).
 
@@ -54,45 +54,54 @@
             f"You passed different entities as '{deprecated_arg_name}' and '{new_arg_name}'. "
             f"The parameter '{deprecated_arg_name}' was renamed to '{new_arg_name}' in Bot API "
             f"{bot_api_version}. We recommend using '{new_arg_name}' instead of "
             f"'{deprecated_arg_name}'."
         )
 
     if deprecated_arg:
-        warn(
+        warn_callback(
             f"Bot API {bot_api_version} renamed the argument '{deprecated_arg_name}' to "
             f"'{new_arg_name}'.",
             PTBDeprecationWarning,
-            stacklevel=stacklevel,
+            stacklevel + 1,
         )
         return deprecated_arg
 
     return new_arg
 
 
 def warn_about_deprecated_attr_in_property(
     deprecated_attr_name: str,
     new_attr_name: str,
     bot_api_version: str,
-    stacklevel: int = 3,
+    stacklevel: int = 2,
 ) -> None:
     """A helper function for the transition in API when attribute is renamed. Call from properties.
 
     The properties replace deprecated attributes in classes and issue these deprecation warnings.
     """
     warn(
         f"Bot API {bot_api_version} renamed the attribute '{deprecated_attr_name}' to "
         f"'{new_attr_name}'.",
         PTBDeprecationWarning,
-        stacklevel=stacklevel,
+        stacklevel=stacklevel + 1,
     )
 
 
-warn_about_thumb_return_thumbnail = functools.partial(
-    warn_about_deprecated_arg_return_new_arg,
-    deprecated_arg_name="thumb",
-    new_arg_name="thumbnail",
-    bot_api_version="6.6",
-)
-"""A helper function to warn about using a deprecated 'thumb' argument and return it or the new
-'thumbnail' argument, introduced in API 6.6.
-"""
+def warn_about_thumb_return_thumbnail(
+    deprecated_arg: Any,
+    new_arg: Any,
+    stacklevel: int = 2,
+    warn_callback: Callable[[str, Type[Warning], int], None] = warn,
+) -> Any:
+    """A helper function to warn about using a deprecated 'thumb' argument and return it or the
+    new 'thumbnail' argument, introduced in API 6.6.
+    """
+    return warn_about_deprecated_arg_return_new_arg(
+        deprecated_arg=deprecated_arg,
+        new_arg=new_arg,
+        warn_callback=warn_callback,
+        deprecated_arg_name="thumb",
+        new_arg_name="thumbnail",
+        bot_api_version="6.6",
+        stacklevel=stacklevel + 1,
+    )
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_version.py` & `python-telegram-bot-raw-20.3/telegram/_version.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             version = f"{version}.{self.micro}"
         if self.releaselevel != "final":
             version = f"{version}{self._rl_shorthand()}{self.serial}"
 
         return version
 
 
-__version_info__ = Version(major=20, minor=2, micro=0, releaselevel="final", serial=0)
+__version_info__ = Version(major=20, minor=3, micro=0, releaselevel="final", serial=0)
 __version__ = str(__version_info__)
 
 # # SETUP.PY MARKER
 # Lines above this line will be `exec`-cuted in setup.py. Make sure that this only contains
 # std-lib imports!
 
 from telegram import constants  # noqa: E402  # pylint: disable=wrong-import-position
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_videochat.py` & `python-telegram-bot-raw-20.3/telegram/_videochat.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 """This module contains objects related to Telegram video chats."""
 import datetime as dtm
 from typing import TYPE_CHECKING, Optional, Sequence, Tuple
 
 from telegram._telegramobject import TelegramObject
 from telegram._user import User
 from telegram._utils.argumentparsing import parse_sequence_arg
-from telegram._utils.datetime import from_timestamp
+from telegram._utils.datetime import extract_tzinfo_from_defaults, from_timestamp
 from telegram._utils.types import JSONDict
 
 if TYPE_CHECKING:
     from telegram import Bot
 
 
 class VideoChatStarted(TelegramObject):
@@ -145,18 +145,24 @@
 
     .. versionchanged:: 20.0
         This class was renamed from ``VoiceChatScheduled`` in accordance to Bot API 6.0.
 
     Args:
         start_date (:obj:`datetime.datetime`): Point in time (Unix timestamp) when the video
             chat is supposed to be started by a chat administrator
+
+            .. versionchanged:: 20.3
+                |datetime_localization|
     Attributes:
         start_date (:obj:`datetime.datetime`): Point in time (Unix timestamp) when the video
             chat is supposed to be started by a chat administrator
 
+            .. versionchanged:: 20.3
+                |datetime_localization|
+
     """
 
     __slots__ = ("start_date",)
 
     def __init__(
         self,
         start_date: dtm.datetime,
@@ -174,10 +180,13 @@
     def de_json(cls, data: Optional[JSONDict], bot: "Bot") -> Optional["VideoChatScheduled"]:
         """See :meth:`telegram.TelegramObject.de_json`."""
         data = cls._parse_data(data)
 
         if not data:
             return None
 
-        data["start_date"] = from_timestamp(data["start_date"])
+        # Get the local timezone from the bot if it has defaults
+        loc_tzinfo = extract_tzinfo_from_defaults(bot)
+
+        data["start_date"] = from_timestamp(data["start_date"], tzinfo=loc_tzinfo)
 
         return super().de_json(data=data, bot=bot)
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_webappdata.py` & `python-telegram-bot-raw-20.3/telegram/_webappdata.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_webappinfo.py` & `python-telegram-bot-raw-20.3/telegram/_webappinfo.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/_webhookinfo.py` & `python-telegram-bot-raw-20.3/telegram/_webhookinfo.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains an object that represents a Telegram WebhookInfo."""
 from typing import TYPE_CHECKING, Optional, Sequence, Tuple
 
 from telegram._telegramobject import TelegramObject
 from telegram._utils.argumentparsing import parse_sequence_arg
-from telegram._utils.datetime import from_timestamp
+from telegram._utils.datetime import extract_tzinfo_from_defaults, from_timestamp
 from telegram._utils.types import JSONDict
 
 if TYPE_CHECKING:
     from telegram import Bot
 
 
 class WebhookInfo(TelegramObject):
@@ -45,55 +45,69 @@
 
     Args:
         url (:obj:`str`): Webhook URL, may be empty if webhook is not set up.
         has_custom_certificate (:obj:`bool`): :obj:`True`, if a custom certificate was provided for
             webhook certificate checks.
         pending_update_count (:obj:`int`): Number of updates awaiting delivery.
         ip_address (:obj:`str`, optional): Currently used webhook IP address.
-        last_error_date (:obj:`int`, optional): Unix time for the most recent error that happened
-            when trying to deliver an update via webhook.
+        last_error_date (:class:`datetime.datetime`): Optional. Datetime for the most recent
+            error that happened when trying to deliver an update via webhook.
+
+            .. versionchanged:: 20.3
+                |datetime_localization|
         last_error_message (:obj:`str`, optional): Error message in human-readable format for the
             most recent error that happened when trying to deliver an update via webhook.
         max_connections (:obj:`int`, optional): Maximum allowed number of simultaneous HTTPS
             connections to the webhook for update delivery.
         allowed_updates (Sequence[:obj:`str`], optional): A list of update types the bot is
             subscribed to. Defaults to all update types, except
             :attr:`telegram.Update.chat_member`.
 
             .. versionchanged:: 20.0
                 |sequenceclassargs|
 
-        last_synchronization_error_date (:obj:`int`, optional): Unix time of the most recent error
-            that happened when trying to synchronize available updates with Telegram datacenters.
+        last_synchronization_error_date (:class:`datetime.datetime`, optional): Datetime of the
+            most recent error that happened when trying to synchronize available updates with
+            Telegram datacenters.
 
             .. versionadded:: 20.0
+
+            .. versionchanged:: 20.3
+                |datetime_localization|
     Attributes:
         url (:obj:`str`): Webhook URL, may be empty if webhook is not set up.
         has_custom_certificate (:obj:`bool`): :obj:`True`, if a custom certificate was provided for
             webhook certificate checks.
         pending_update_count (:obj:`int`): Number of updates awaiting delivery.
         ip_address (:obj:`str`): Optional. Currently used webhook IP address.
-        last_error_date (:obj:`int`): Optional. Unix time for the most recent error that happened
-            when trying to deliver an update via webhook.
+        last_error_date (:class:`datetime.datetime`): Optional. Datetime for the most recent
+            error that happened when trying to deliver an update via webhook.
+
+            .. versionchanged:: 20.3
+                |datetime_localization|
         last_error_message (:obj:`str`): Optional. Error message in human-readable format for the
             most recent error that happened when trying to deliver an update via webhook.
         max_connections (:obj:`int`): Optional. Maximum allowed number of simultaneous HTTPS
             connections to the webhook for update delivery.
         allowed_updates (Tuple[:obj:`str`]): Optional. A list of update types the bot is
             subscribed to. Defaults to all update types, except
             :attr:`telegram.Update.chat_member`.
 
             .. versionchanged:: 20.0
 
                 * |tupleclassattrs|
                 * |alwaystuple|
-        last_synchronization_error_date (:obj:`int`): Optional. Unix time of the most recent error
-            that happened when trying to synchronize available updates with Telegram datacenters.
+        last_synchronization_error_date (:class:`datetime.datetime`, optional): Datetime of the
+            most recent error that happened when trying to synchronize available updates with
+            Telegram datacenters.
 
             .. versionadded:: 20.0
+
+            .. versionchanged:: 20.3
+                |datetime_localization|
     """
 
     __slots__ = (
         "allowed_updates",
         "url",
         "max_connections",
         "last_error_date",
@@ -150,13 +164,16 @@
     def de_json(cls, data: Optional[JSONDict], bot: "Bot") -> Optional["WebhookInfo"]:
         """See :meth:`telegram.TelegramObject.de_json`."""
         data = cls._parse_data(data)
 
         if not data:
             return None
 
-        data["last_error_date"] = from_timestamp(data.get("last_error_date"))
+        # Get the local timezone from the bot if it has defaults
+        loc_tzinfo = extract_tzinfo_from_defaults(bot)
+
+        data["last_error_date"] = from_timestamp(data.get("last_error_date"), tzinfo=loc_tzinfo)
         data["last_synchronization_error_date"] = from_timestamp(
-            data.get("last_synchronization_error_date")
+            data.get("last_synchronization_error_date"), tzinfo=loc_tzinfo
         )
 
         return super().de_json(data=data, bot=bot)
```

### Comparing `python-telegram-bot-raw-20.2/telegram/_writeaccessallowed.py` & `python-telegram-bot-raw-20.3/telegram/_writeaccessallowed.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,25 +13,39 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains objects related to the write access allowed service message."""
+from typing import Optional
+
 from telegram._telegramobject import TelegramObject
 from telegram._utils.types import JSONDict
 
 
 class WriteAccessAllowed(TelegramObject):
     """
-    This object represents a service message about a user allowing a bot added to the attachment
-    menu to write messages. Currently holds no information.
+    This object represents a service message about a user allowing a bot to write messages after
+    adding the bot to the attachment menu or launching a Web App from a link.
 
     .. versionadded:: 20.0
+
+    Args:
+        web_app_name (:obj:`str`, optional): Name of the Web App which was launched from a link.
+
+            .. versionadded:: 20.3
+
+    Attributes:
+        web_app_name (:obj:`str`): Optional. Name of the Web App which was launched from a link.
+
+            .. versionadded:: 20.3
+
     """
 
-    __slots__ = ()
+    __slots__ = ("web_app_name",)
 
-    def __init__(self, *, api_kwargs: JSONDict = None):
+    def __init__(self, web_app_name: str = None, *, api_kwargs: JSONDict = None):
         super().__init__(api_kwargs=api_kwargs)
+        self.web_app_name: Optional[str] = web_app_name
 
         self._freeze()
```

### Comparing `python-telegram-bot-raw-20.2/telegram/constants.py` & `python-telegram-bot-raw-20.3/telegram/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 __all__ = [
     "BOT_API_VERSION",
     "BOT_API_VERSION_INFO",
     "BotCommandLimit",
     "BotCommandScopeType",
     "BotDescriptionLimit",
+    "BotNameLimit",
     "CallbackQueryLimit",
     "ChatAction",
     "ChatID",
     "ChatInviteLinkLimit",
     "ChatLimit",
     "ChatMemberStatus",
     "ChatPhotoSize",
@@ -53,14 +54,15 @@
     "FloodLimit",
     "ForumIconColor",
     "ForumTopicLimit",
     "InlineKeyboardButtonLimit",
     "InlineKeyboardMarkupLimit",
     "InlineQueryLimit",
     "InlineQueryResultLimit",
+    "InlineQueryResultsButtonLimit",
     "InlineQueryResultType",
     "InputMediaType",
     "InvoiceLimit",
     "LocationLimit",
     "MaskPosition",
     "MediaGroupLimit",
     "MenuButtonType",
@@ -110,15 +112,15 @@
 #: :class:`typing.NamedTuple`: A tuple containing the two components of the version number:
 # ``major`` and ``minor``. Both values are integers.
 #: The components can also be accessed by name, so ``BOT_API_VERSION_INFO[0]`` is equivalent
 #: to ``BOT_API_VERSION_INFO.major`` and so on. Also available as
 #: :data:`telegram.__bot_api_version_info__`.
 #:
 #: .. versionadded:: 20.0
-BOT_API_VERSION_INFO = _BotAPIVersion(major=6, minor=6)
+BOT_API_VERSION_INFO = _BotAPIVersion(major=6, minor=7)
 #: :obj:`str`: Telegram Bot API
 #: version supported by this version of `python-telegram-bot`. Also available as
 #: :data:`telegram.__bot_api_version__`.
 #:
 #: .. versionadded:: 13.4
 BOT_API_VERSION = str(BOT_API_VERSION_INFO)
 
@@ -205,14 +207,29 @@
     MAX_SHORT_DESCRIPTION_LENGTH = 120
     """:obj:`int`: Maximum length for the parameter
     :paramref:`~telegram.Bot.set_my_short_description.short_description` of
     :meth:`telegram.Bot.set_my_short_description`
     """
 
 
+class BotNameLimit(IntEnum):
+    """This enum contains limitations for the methods :meth:`telegram.Bot.set_my_name`.
+    The enum members of this enumeration are instances of :class:`int` and can be treated as such.
+
+    .. versionadded:: 20.3
+    """
+
+    __slots__ = ()
+
+    MAX_NAME_LENGTH = 64
+    """:obj:`int`: Maximum length for the parameter :paramref:`~telegram.Bot.set_my_name.name` of
+    :meth:`telegram.Bot.set_my_name`
+    """
+
+
 class CallbackQueryLimit(IntEnum):
     """This enum contains limitations for :class:`telegram.CallbackQuery`/
     :meth:`telegram.Bot.answer_callback_query`. The enum members of this enumeration are instances
     of :class:`int` and can be treated as such.
 
     .. versionadded:: 20.0
     """
@@ -731,19 +748,27 @@
     :meth:`telegram.Bot.answer_inline_query`."""
     MAX_QUERY_LENGTH = 256
     """:obj:`int`: Maximum number of characters in a :obj:`str` passed as the
     :paramref:`~telegram.InlineQuery.query` parameter of :class:`telegram.InlineQuery`."""
     MIN_SWITCH_PM_TEXT_LENGTH = 1
     """:obj:`int`: Minimum number of characters in a :obj:`str` passed as the
     :paramref:`~telegram.Bot.answer_inline_query.switch_pm_parameter` parameter of
-    :meth:`telegram.Bot.answer_inline_query`."""
+    :meth:`telegram.Bot.answer_inline_query`.
+
+    .. deprecated:: 20.3
+        Deprecated in favor of :attr:`InlineQueryResultsButtonLimit.MIN_START_PARAMETER_LENGTH`.
+    """
     MAX_SWITCH_PM_TEXT_LENGTH = 64
     """:obj:`int`: Maximum number of characters in a :obj:`str` passed as the
     :paramref:`~telegram.Bot.answer_inline_query.switch_pm_parameter` parameter of
-    :meth:`telegram.Bot.answer_inline_query`."""
+    :meth:`telegram.Bot.answer_inline_query`.
+
+    .. deprecated:: 20.3
+        Deprecated in favor of :attr:`InlineQueryResultsButtonLimit.MAX_START_PARAMETER_LENGTH`.
+    """
 
 
 class InlineQueryResultLimit(IntEnum):
     """This enum contains limitations for :class:`telegram.InlineQueryResult` and its subclasses.
     The enum members of this enumeration are instances of :class:`int` and can be treated as such.
 
     .. versionadded:: 20.0
@@ -759,14 +784,34 @@
     MAX_ID_LENGTH = 64
     """:obj:`int`: Maximum number of bytes in a :obj:`str` passed as the
     :paramref:`~telegram.InlineQueryResult.id` parameter of
     :class:`telegram.InlineQueryResult` and its subclasses
     """
 
 
+class InlineQueryResultsButtonLimit(IntEnum):
+    """This enum contains limitations for :class:`telegram.InlineQueryResultsButton`.
+    The enum members of this enumeration are instances of :class:`int` and can be treated as such.
+
+    .. versionadded:: 20.3
+    """
+
+    __slots__ = ()
+
+    MIN_START_PARAMETER_LENGTH = InlineQueryLimit.MIN_SWITCH_PM_TEXT_LENGTH
+    """:obj:`int`: Minimum number of characters in a :obj:`str` passed as the
+    :paramref:`~telegram.InlineQueryResultsButton.start_parameter` parameter of
+    :meth:`telegram.InlineQueryResultsButton`."""
+
+    MAX_START_PARAMETER_LENGTH = InlineQueryLimit.MAX_SWITCH_PM_TEXT_LENGTH
+    """:obj:`int`: Maximum number of characters in a :obj:`str` passed as the
+    :paramref:`~telegram.InlineQueryResultsButton.start_parameter` parameter of
+    :meth:`telegram.InlineQueryResultsButton`."""
+
+
 class InlineQueryResultType(StringEnum):
     """This enum contains the available types of :class:`telegram.InlineQueryResult`. The enum
     members of this enumeration are instances of :class:`str` and can be treated as such.
 
     .. versionadded:: 20.0
     """
```

### Comparing `python-telegram-bot-raw-20.2/telegram/error.py` & `python-telegram-bot-raw-20.3/telegram/error.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,25 +44,27 @@
         in_s (:obj:`str`): in string
         lstr (:obj:`str`): substr to strip from left side
 
     Returns:
         :obj:`str`: The stripped string.
 
     """
-    if in_s.startswith(lstr):
-        res = in_s[len(lstr) :]
-    else:
-        res = in_s
-    return res
+    return in_s[len(lstr) :] if in_s.startswith(lstr) else in_s
 
 
 class TelegramError(Exception):
     """
     Base class for Telegram errors.
 
+    Tip:
+        Objects of this type can be serialized via Python's :mod:`pickle` module and pickled
+        objects from one version of PTB are usually loadable in future versions. However, we can
+        not guarantee that this compatibility will always be provided. At least a manual one-time
+        conversion of the data may be needed on major updates of the library.
+
     .. seealso:: :wiki:`Exceptions, Warnings and Logging <Exceptions%2C-Warnings-and-Logging>`
     """
 
     __slots__ = ("message",)
 
     def __init__(self, message: str):
         super().__init__()
```

### Comparing `python-telegram-bot-raw-20.2/telegram/helpers.py` & `python-telegram-bot-raw-20.3/telegram/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,31 +40,35 @@
 if TYPE_CHECKING:
     from telegram import Message, Update
 
 
 def escape_markdown(text: str, version: int = 1, entity_type: str = None) -> str:
     """Helper function to escape telegram markup symbols.
 
+    .. versionchanged:: 20.3
+        Custom emoji entity escaping is now supported.
+
     Args:
         text (:obj:`str`): The text.
         version (:obj:`int` | :obj:`str`): Use to specify the version of telegrams Markdown.
             Either ``1`` or ``2``. Defaults to ``1``.
         entity_type (:obj:`str`, optional): For the entity types
             :tg-const:`telegram.MessageEntity.PRE`, :tg-const:`telegram.MessageEntity.CODE` and
-            the link part of :tg-const:`telegram.MessageEntity.TEXT_LINK`, only certain characters
-            need to be escaped in :tg-const:`telegram.constants.ParseMode.MARKDOWN_V2`.
-            See the official API documentation for details. Only valid in combination with
-            ``version=2``, will be ignored else.
+            the link part of :tg-const:`telegram.MessageEntity.TEXT_LINK` and
+            :tg-const:`telegram.MessageEntity.CUSTOM_EMOJI`, only certain characters need to be
+            escaped in :tg-const:`telegram.constants.ParseMode.MARKDOWN_V2`. See the `official API
+            documentation <https://core.telegram.org/bots/api#formatting-options>`_ for details.
+            Only valid in combination with ``version=2``, will be ignored else.
     """
     if int(version) == 1:
         escape_chars = r"_*`["
     elif int(version) == 2:
         if entity_type in ["pre", "code"]:
             escape_chars = r"\`"
-        elif entity_type == "text_link":
+        elif entity_type in ["text_link", "custom_emoji"]:
             escape_chars = r"\)"
         else:
             escape_chars = r"\_*[]()~`>#+-=|{}.!"
     else:
         raise ValueError("Markdown version must be either 1 or 2!")
 
     return re.sub(f"([{re.escape(escape_chars)}])", r"\\\1", text)
@@ -158,14 +162,19 @@
         payload (:obj:`str`, optional): Parameters to encode in the created URL.
         group (:obj:`bool`, optional): If :obj:`True` the user is prompted to select a group to
             add the bot to. If :obj:`False`, opens a one-on-one conversation with the bot.
             Defaults to :obj:`False`.
 
     Returns:
         :obj:`str`: An URL to start the bot with specific parameters.
+
+    Raises:
+        :exc:`ValueError`: If the length of the :paramref:`payload` exceeds 64 characters,
+            contains invalid characters, or if the :paramref:`bot_username` is less than 4
+            characters.
     """
     if bot_username is None or len(bot_username) <= 3:
         raise ValueError("You must provide a valid bot_username.")
 
     base_url = f"https://t.me/{bot_username}"
     if not payload:
         return base_url
@@ -175,13 +184,10 @@
 
     if not re.match(r"^[A-Za-z0-9_-]+$", payload):
         raise ValueError(
             "Only the following characters are allowed for deep-linked "
             "URLs: A-Z, a-z, 0-9, _ and -"
         )
 
-    if group:
-        key = "startgroup"
-    else:
-        key = "start"
+    key = "startgroup" if group else "start"
 
     return f"{base_url}?{key}={payload}"
```

### Comparing `python-telegram-bot-raw-20.2/telegram/request/__init__.py` & `python-telegram-bot-raw-20.3/telegram/request/__init__.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/request/_baserequest.py` & `python-telegram-bot-raw-20.3/telegram/request/_baserequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import json
 from http import HTTPStatus
 from types import TracebackType
 from typing import AsyncContextManager, ClassVar, List, Optional, Tuple, Type, TypeVar, Union
 
 from telegram._utils.defaultvalue import DEFAULT_NONE as _DEFAULT_NONE
 from telegram._utils.defaultvalue import DefaultValue
+from telegram._utils.logging import get_logger
 from telegram._utils.types import JSONDict, ODVInput
 from telegram._version import __version__ as ptb_ver
 from telegram.error import (
     BadRequest,
     ChatMigrated,
     Conflict,
     Forbidden,
@@ -38,14 +39,16 @@
     RetryAfter,
     TelegramError,
 )
 from telegram.request._requestdata import RequestData
 
 RT = TypeVar("RT", bound="BaseRequest")
 
+_LOGGER = get_logger(__name__, class_name="BaseRequest")
+
 
 class BaseRequest(
     AsyncContextManager["BaseRequest"],
     abc.ABC,
 ):
     """Abstract interface class that allows python-telegram-bot to make requests to the Bot API.
     Can be implemented via different asyncio HTTP libraries. An implementation of this class
@@ -292,18 +295,15 @@
         if HTTPStatus.OK <= code <= 299:
             # 200-299 range are HTTP success statuses
             return payload
 
         response_data = self.parse_json_payload(payload)
 
         description = response_data.get("description")
-        if description:
-            message = description
-        else:
-            message = "Unknown HTTPError"
+        message = description if description else "Unknown HTTPError"
 
         # In some special cases, we can raise more informative exceptions:
         # see https://core.telegram.org/bots/api#responseparameters and
         # https://core.telegram.org/bots/api#making-requests
         parameters = response_data.get("parameters")
         if parameters:
             migrate_to_chat_id = parameters.get("migrate_to_chat_id")
@@ -350,14 +350,15 @@
         Raises:
             TelegramError: If loading the JSON data failed
         """
         decoded_s = payload.decode("utf-8", "replace")
         try:
             return json.loads(decoded_s)
         except ValueError as exc:
+            _LOGGER.error('Can not load invalid JSON data: "%s"', decoded_s)
             raise TelegramError("Invalid server response") from exc
 
     @abc.abstractmethod
     async def do_request(
         self,
         url: str,
         method: str,
```

### Comparing `python-telegram-bot-raw-20.2/telegram/request/_httpxrequest.py` & `python-telegram-bot-raw-20.3/telegram/request/_httpxrequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,31 +13,31 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser Public License for more details.
 #
 # You should have received a copy of the GNU Lesser Public License
 # along with this program.  If not, see [http://www.gnu.org/licenses/].
 """This module contains methods to make POST and GET requests using the httpx library."""
-import logging
 from typing import Optional, Tuple
 
 import httpx
 
 from telegram._utils.defaultvalue import DefaultValue
+from telegram._utils.logging import get_logger
 from telegram._utils.types import ODVInput
 from telegram.error import NetworkError, TimedOut
 from telegram.request._baserequest import BaseRequest
 from telegram.request._requestdata import RequestData
 
 # Note to future devs:
 # Proxies are currently only tested manually. The httpx development docs have a nice guide on that:
 # https://www.python-httpx.org/contributing/#development-proxy-setup (also saved on archive.org)
 # That also works with socks5. Just pass `--mode socks5` to mitmproxy
 
-_logger = logging.getLogger(__name__)
+_LOGGER = get_logger(__name__, "HTTPXRequest")
 
 
 class HTTPXRequest(BaseRequest):
     """Implementation of :class:`~telegram.request.BaseRequest` using the library
     `httpx <https://www.python-httpx.org>`_.
 
     .. versionadded:: 20.0
@@ -118,15 +118,15 @@
         if http_version not in ("1.1", "2"):
             raise ValueError("`http_version` must be either '1.1' or '2'.")
 
         http1 = http_version == "1.1"
 
         # See https://github.com/python-telegram-bot/python-telegram-bot/pull/3542
         # for why we need to use `dict()` here.
-        self._client_kwargs = dict(  # pylint: disable=use-dict-literal
+        self._client_kwargs = dict(  # pylint: disable=use-dict-literal  # noqa: C408
             timeout=timeout,
             proxies=proxy_url,
             limits=limits,
             http1=http1,
             http2=not http1,
         )
 
@@ -162,15 +162,15 @@
         """See :meth:`BaseRequest.initialize`."""
         if self._client.is_closed:
             self._client = self._build_client()
 
     async def shutdown(self) -> None:
         """See :meth:`BaseRequest.shutdown`."""
         if self._client.is_closed:
-            _logger.debug("This HTTPXRequest is already shut down. Returning.")
+            _LOGGER.debug("This HTTPXRequest is already shut down. Returning.")
             return
 
         await self._client.aclose()
 
     async def do_request(
         self,
         url: str,
```

### Comparing `python-telegram-bot-raw-20.2/telegram/request/_requestdata.py` & `python-telegram-bot-raw-20.3/telegram/request/_requestdata.py`

 * *Files identical despite different names*

### Comparing `python-telegram-bot-raw-20.2/telegram/request/_requestparameter.py` & `python-telegram-bot-raw-20.3/telegram/request/_requestparameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from telegram._files.inputsticker import InputSticker
 from telegram._telegramobject import TelegramObject
 from telegram._utils.datetime import to_timestamp
 from telegram._utils.enum import StringEnum
 from telegram._utils.types import UploadFileDict
 
 
-@dataclass(repr=False, eq=False, order=False, frozen=True)
+@dataclass(repr=True, eq=False, order=False, frozen=True)
 class RequestParameter:
     """Instances of this class represent a single parameter to be sent along with a request to
     the Bot API.
 
     .. versionadded:: 20.0
 
     Warning:
```

### Comparing `python-telegram-bot-raw-20.2/telegram/warnings.py` & `python-telegram-bot-raw-20.3/telegram/warnings.py`

 * *Files identical despite different names*

