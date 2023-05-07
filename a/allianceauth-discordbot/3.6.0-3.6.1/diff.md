# Comparing `tmp/allianceauth-discordbot-3.6.0.tar.gz` & `tmp/allianceauth-discordbot-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allianceauth-discordbot-3.6.0.tar", last modified: Sun May  7 06:32:51 2023, max compression
+gzip compressed data, was "allianceauth-discordbot-3.6.1.tar", last modified: Sun May  7 14:19:13 2023, max compression
```

## Comparing `allianceauth-discordbot-3.6.0.tar` & `allianceauth-discordbot-3.6.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:32:51.192963 allianceauth-discordbot-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-05-07 06:32:51.192963 allianceauth-discordbot-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:32:51.188963 allianceauth-discordbot-3.6.0/aadiscordbot/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17005 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/bot_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:32:51.188963 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/about.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/abuse.py
--rw-r--r--   0 runner    (1001) docker     (123)    16421 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/eastereggs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/eightball.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/facwar.py
--rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/price_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/prom_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/reaction_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/remind.py
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/services.py
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/sov.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/timers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:32:51.188963 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/welcomegoodbye.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:32:51.192963 allianceauth-discordbot-3.6.0/aadiscordbot/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0003_authbotconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0004_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0007_quotemessage.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0008_channels_deleted.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0009_alter_quotemessage_options.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:32:51.192963 allianceauth-discordbot-3.6.0/allianceauth_discordbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-05-07 06:32:51.000000 allianceauth-discordbot-3.6.0/allianceauth_discordbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-07 06:32:51.000000 allianceauth-discordbot-3.6.0/allianceauth_discordbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 06:32:51.000000 allianceauth-discordbot-3.6.0/allianceauth_discordbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-07 06:32:51.000000 allianceauth-discordbot-3.6.0/allianceauth_discordbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-07 06:32:51.000000 allianceauth-discordbot-3.6.0/allianceauth_discordbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 06:32:51.192963 allianceauth-discordbot-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:19:13.189020 allianceauth-discordbot-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-05-07 14:19:13.189020 allianceauth-discordbot-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:19:13.185020 allianceauth-discordbot-3.6.1/aadiscordbot/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17005 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/bot_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:19:13.189020 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/abuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16421 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/eastereggs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/eightball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/facwar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/price_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/prom_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/reaction_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/remind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/sov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/timers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:19:13.189020 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/cogs/welcomegoodbye.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:19:13.189020 allianceauth-discordbot-3.6.1/aadiscordbot/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/migrations/0003_authbotconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/migrations/0004_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/migrations/0007_quotemessage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/migrations/0008_channels_deleted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/migrations/0009_alter_quotemessage_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/aadiscordbot/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:19:13.189020 allianceauth-discordbot-3.6.1/allianceauth_discordbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-05-07 14:19:13.000000 allianceauth-discordbot-3.6.1/allianceauth_discordbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-07 14:19:13.000000 allianceauth-discordbot-3.6.1/allianceauth_discordbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 14:19:13.000000 allianceauth-discordbot-3.6.1/allianceauth_discordbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-07 14:19:13.000000 allianceauth-discordbot-3.6.1/allianceauth_discordbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-07 14:19:13.000000 allianceauth-discordbot-3.6.1/allianceauth_discordbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 14:19:13.189020 allianceauth-discordbot-3.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-07 14:18:28.000000 allianceauth-discordbot-3.6.1/setup.py
```

### Comparing `allianceauth-discordbot-3.6.0/PKG-INFO` & `allianceauth-discordbot-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-discordbot
-Version: 3.6.0
+Version: 3.6.1
 Summary: Alliance Auth Discord Bot
 Home-page: https://github.com/pvyParts/allianceauth-discordbot
 Author: ak
 Author-email: ak@ak.auth
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `allianceauth-discordbot-3.6.0/README.md` & `allianceauth-discordbot-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/admin.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/app_settings.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/app_settings.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/auth_hooks.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/bot.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/bot.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/bot_tasks.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/bot_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/about.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/cogs/about.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/abuse.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/cogs/abuse.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/admin.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/cogs/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/auth.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/cogs/auth.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/eastereggs.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/cogs/eastereggs.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/eightball.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/cogs/eightball.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/facwar.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/cogs/facwar.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/members.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/cogs/members.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/models.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/cogs/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/price_check.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/cogs/price_check.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/prom_export.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/cogs/prom_export.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/quote.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/cogs/quote.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/reaction_roles.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/cogs/reaction_roles.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/remind.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/cogs/remind.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/services.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/cogs/services.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/sov.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/cogs/sov.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/time.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/cogs/time.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/timers.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/cogs/timers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/utils/decorators.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/cogs/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/welcomegoodbye.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/cogs/welcomegoodbye.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0001_initial.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0003_authbotconfiguration.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/migrations/0003_authbotconfiguration.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0007_quotemessage.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/migrations/0007_quotemessage.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/models.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/aadiscordbot/tasks.py` & `allianceauth-discordbot-3.6.1/aadiscordbot/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/allianceauth_discordbot.egg-info/PKG-INFO` & `allianceauth-discordbot-3.6.1/allianceauth_discordbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-discordbot
-Version: 3.6.0
+Version: 3.6.1
 Summary: Alliance Auth Discord Bot
 Home-page: https://github.com/pvyParts/allianceauth-discordbot
 Author: ak
 Author-email: ak@ak.auth
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `allianceauth-discordbot-3.6.0/allianceauth_discordbot.egg-info/SOURCES.txt` & `allianceauth-discordbot-3.6.1/allianceauth_discordbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.6.0/setup.py` & `allianceauth-discordbot-3.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,10 +37,10 @@
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     ],
     python_requires='>=3.8',
     install_requires=[
         "allianceauth>=2.9.0,<4.0.0",
         "py-cord>2.0.0,<3.0.0",
         "pendulum>=2.1.2,<3.0.0",
-        "redis>=4.2.0<5.0.0"
+        "redis>=4.2.0,<5.0.0",
     ],
 )
```

