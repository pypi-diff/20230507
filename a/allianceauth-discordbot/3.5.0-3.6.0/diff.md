# Comparing `tmp/allianceauth-discordbot-3.5.0.tar.gz` & `tmp/allianceauth-discordbot-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allianceauth-discordbot-3.5.0.tar", last modified: Sat Apr 29 03:14:35 2023, max compression
+gzip compressed data, was "allianceauth-discordbot-3.6.0.tar", last modified: Sun May  7 06:32:51 2023, max compression
```

## Comparing `allianceauth-discordbot-3.5.0.tar` & `allianceauth-discordbot-3.6.0.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:14:35.696330 allianceauth-discordbot-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-04-29 03:14:35.696330 allianceauth-discordbot-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:14:35.692330 allianceauth-discordbot-3.5.0/aadiscordbot/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/bot_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:14:35.696330 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/about.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/abuse.py
--rw-r--r--   0 runner    (1001) docker     (123)    16421 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/eastereggs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/eightball.py
--rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/price_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/prom_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/reaction_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/remind.py
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/services.py
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/sov.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/timers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:14:35.696330 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/welcomegoodbye.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:14:35.696330 allianceauth-discordbot-3.5.0/aadiscordbot/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0003_authbotconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0004_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0007_quotemessage.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0008_channels_deleted.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0009_alter_quotemessage_options.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:14:35.696330 allianceauth-discordbot-3.5.0/allianceauth_discordbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-04-29 03:14:35.000000 allianceauth-discordbot-3.5.0/allianceauth_discordbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-29 03:14:35.000000 allianceauth-discordbot-3.5.0/allianceauth_discordbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 03:14:35.000000 allianceauth-discordbot-3.5.0/allianceauth_discordbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-29 03:14:35.000000 allianceauth-discordbot-3.5.0/allianceauth_discordbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 03:14:35.000000 allianceauth-discordbot-3.5.0/allianceauth_discordbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 03:14:35.696330 allianceauth-discordbot-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:32:51.192963 allianceauth-discordbot-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-05-07 06:32:51.192963 allianceauth-discordbot-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:32:51.188963 allianceauth-discordbot-3.6.0/aadiscordbot/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17005 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/bot_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:32:51.188963 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/abuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16421 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/eastereggs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/eightball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/facwar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/price_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/prom_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/reaction_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/remind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/sov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/timers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:32:51.188963 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/cogs/welcomegoodbye.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:32:51.192963 allianceauth-discordbot-3.6.0/aadiscordbot/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0003_authbotconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0004_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0007_quotemessage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0008_channels_deleted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0009_alter_quotemessage_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/aadiscordbot/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:32:51.192963 allianceauth-discordbot-3.6.0/allianceauth_discordbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-05-07 06:32:51.000000 allianceauth-discordbot-3.6.0/allianceauth_discordbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-07 06:32:51.000000 allianceauth-discordbot-3.6.0/allianceauth_discordbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 06:32:51.000000 allianceauth-discordbot-3.6.0/allianceauth_discordbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-07 06:32:51.000000 allianceauth-discordbot-3.6.0/allianceauth_discordbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-07 06:32:51.000000 allianceauth-discordbot-3.6.0/allianceauth_discordbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 06:32:51.192963 allianceauth-discordbot-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-07 06:32:07.000000 allianceauth-discordbot-3.6.0/setup.py
```

### Comparing `allianceauth-discordbot-3.5.0/PKG-INFO` & `allianceauth-discordbot-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-discordbot
-Version: 3.5.0
+Version: 3.6.0
 Summary: Alliance Auth Discord Bot
 Home-page: https://github.com/pvyParts/allianceauth-discordbot
 Author: ak
 Author-email: ak@ak.auth
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `allianceauth-discordbot-3.5.0/README.md` & `allianceauth-discordbot-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/admin.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/app_settings.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/app_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,7 +107,12 @@
 DISCORD_BOT_TASK_RATE_LIMITS = getattr(settings, 'DISCORD_BOT_TASK_RATE_LIMITS',
                                        {"send_channel_message_by_discord_id": "100/s",
                                         "send_direct_message_by_discord_id": "100/s",
                                         "send_direct_message_by_user_id": "100/s"})
 
 DISCORD_BOT_ESS_PING_CHANNEL_ID = getattr(
     settings, 'DISCORD_BOT_ESS_PING_CHANNEL_ID', None)
+
+DISCORD_BOT_SEND_FAILURE_MESSAGES = getattr(
+    settings, 'DISCORD_BOT_SEND_FAILURE_MESSAGES', False)
+DISCORD_BOT_FAILURE_MESSAGES_CHANNEL = getattr(
+    settings, 'DISCORD_BOT_FAILURE_MESSAGES_CHANNEL', False)
```

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/auth_hooks.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/bot.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 import time
 import traceback
 from datetime import datetime
 from socket import timeout
 from typing import Dict
 
 import aiohttp
-import aioredis
 import discord
 import pendulum
 from celery.utils.time import rate
 from discord import ApplicationContext, DiscordException
 from discord.ext import commands, tasks
 from kombu import Connection, Consumer, Queue
 from kombu.utils.limits import TokenBucket
+from redis import asyncio as aioredis
 
 import django
 import django.db
 from django.conf import settings
 from django.utils import timezone
 
 from allianceauth import hooks
@@ -331,35 +331,35 @@
             next_task = self.pending_tasks.pop_next()
 
     async def on_resumed(self):
         print("Resumed...")
 
     async def on_command_error(self, ctx, error):
         if isinstance(error, commands.BadArgument):
-            print(error)
+            logger.error(error)
             await ctx.send(error)
         elif isinstance(error, commands.MissingRequiredArgument):
-            print(error)
+            logger.error(error)
             await ctx.send(error)
         elif isinstance(error, commands.NoPrivateMessage):
-            print(error)
+            logger.error(error)
             await ctx.send(error)
         elif isinstance(error, commands.CommandInvokeError):
-            print(error)
+            logger.error(error)
             return await ctx.send(error)
         elif isinstance(error, commands.BotMissingPermissions):
             await ctx.send(
                 "Sorry, I don't have the required permissions to do that here:\n{}".format(
                     error.missing_permissions)
             )
         elif isinstance(error, commands.MissingPermissions):
             await ctx.message.add_reaction(chr(DISCORD_BOT_ACCESS_DENIED_REACT))
             await ctx.message.reply("Sorry, you do not have permission to do that here.")
         elif isinstance(error, commands.NotOwner):
-            print(error)
+            logger.error(error)
             await ctx.send(error)
         elif isinstance(error, commands.CommandOnCooldown):
             await ctx.message.add_reaction(chr(0x274C))
         elif isinstance(error, commands.CheckFailure):
             await ctx.send(error)
         else:
             logger.error(f"Unknown Error {error}", exc_info=True)
@@ -369,15 +369,29 @@
         if isinstance(exception, commands.CheckFailure):
             await context.send_response(exception, ephemeral=True)
         elif isinstance(exception, commands.MissingPermissions):
             await context.send_response(exception, ephemeral=True)
         elif isinstance(exception, NotAuthenticated):
             await context.send_response(exception, ephemeral=True)
         else:  # Catch everything, and close out the interactions gracefully.
-            logger.error(f"Unknown Error {exception}", exc_info=True)
+            logger.error(f"Unknown Error {exception}")
+            logger.error("\n".join(traceback.format_tb(
+                exception.original.__traceback__)))
+
+            if app_settings.DISCORD_BOT_SEND_FAILURE_MESSAGES and app_settings.DISCORD_BOT_FAILURE_MESSAGES_CHANNEL:
+                message = [f"`{context.command}` failed for `{context.author}`\n",
+                           f"**Exception:** ```{exception}```",
+                           f"\n**Interaction:** ```{context.interaction.data}```",
+                           f"\n**Trace:**```"]
+                message += traceback.format_tb(
+                    exception.original.__traceback__)
+                message.append("\n```")
+                from . import tasks
+                tasks.send_message(message="\n".join(message),
+                                   channel_id=app_settings.DISCORD_BOT_FAILURE_MESSAGES_CHANNEL)
             await context.respond("Something Went Wrong, Please try again Later.", ephemeral=True)
 
     def run(self):
         # self.load_extension("aadiscordbot.slash.admin")
         try:
 
             logger.info(
```

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/bot_tasks.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/bot_tasks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import importlib
 import logging
 import warnings
 from datetime import timedelta
 
 from discord import Embed
 from discord.ext import tasks
+from discord.ext.commands import Bot
 from discord.ui import View
 
 import django
 from django.utils import timezone
 
 logger = logging.getLogger(__name__)
 
 
 @tasks.loop()
-async def run_tasks(bot):
+async def run_tasks(bot: Bot):
     django.db.close_old_connections()
 
     if len(bot.tasks) > 0:
         task, args, kwargs = bot.tasks.pop(0)
         requeue_task = False
         if hasattr(bot, 'rate_limits'):
             if not bot.rate_limits.check_rate_limit(task.__name__):
@@ -29,15 +30,18 @@
             eta = timezone.now() + timedelta(seconds=timeout)
             bot.pending_tasks.append((eta, (task, args, kwargs)))
             #logger.debug(f"Rate Limit hit! Re Queueing `{task}`")
         else:
             try:
                 await task(bot, *args, **kwargs)
                 bot.statistics.add_task(task.__name__)
+                bot.dispatch("authbot_task_completed", task.__name__)
             except Exception as e:
+                bot.dispatch("authbot_task_failed",
+                             task.__name__, args, kwargs, e)
                 logger.error(f"Failed to run task {task} {args} {kwargs} {e}")
     else:
         run_tasks.stop()
     django.db.close_old_connections()
 
 
 async def send_channel_message_by_discord_id(bot, channel_id, message, embed=False, view_class=False, view_args=[], view_kwargs={}):
```

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/about.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/about.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/abuse.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/abuse.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/admin.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/auth.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/auth.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/eastereggs.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/eastereggs.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/eightball.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/eightball.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 from random import randrange
 
 from discord.ext import commands
-from discord.utils import get
 
 from django.conf import settings
 
 from aadiscordbot import __branch__, __version__
 
 logger = logging.getLogger(__name__)
```

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/members.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/members.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/models.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from unicodedata import name
 
 from discord.commands import SlashCommandGroup
 from discord.ext import commands
 
 from django.conf import settings
 from django.core.exceptions import ObjectDoesNotExist
```

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/price_check.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/price_check.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/quote.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/quote.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/reaction_roles.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/reaction_roles.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/remind.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/remind.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/services.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/services.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/sov.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/sov.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/time.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/time.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/timers.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/timers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/utils/decorators.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/welcomegoodbye.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/cogs/welcomegoodbye.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0001_initial.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0003_authbotconfiguration.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0003_authbotconfiguration.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0007_quotemessage.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/migrations/0007_quotemessage.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/models.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/aadiscordbot/tasks.py` & `allianceauth-discordbot-3.6.0/aadiscordbot/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.5.0/allianceauth_discordbot.egg-info/PKG-INFO` & `allianceauth-discordbot-3.6.0/allianceauth_discordbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-discordbot
-Version: 3.5.0
+Version: 3.6.0
 Summary: Alliance Auth Discord Bot
 Home-page: https://github.com/pvyParts/allianceauth-discordbot
 Author: ak
 Author-email: ak@ak.auth
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `allianceauth-discordbot-3.5.0/allianceauth_discordbot.egg-info/SOURCES.txt` & `allianceauth-discordbot-3.6.0/allianceauth_discordbot.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 aadiscordbot/cogs/__init__.py
 aadiscordbot/cogs/about.py
 aadiscordbot/cogs/abuse.py
 aadiscordbot/cogs/admin.py
 aadiscordbot/cogs/auth.py
 aadiscordbot/cogs/eastereggs.py
 aadiscordbot/cogs/eightball.py
+aadiscordbot/cogs/facwar.py
 aadiscordbot/cogs/members.py
 aadiscordbot/cogs/models.py
 aadiscordbot/cogs/price_check.py
 aadiscordbot/cogs/prom_export.py
 aadiscordbot/cogs/quote.py
 aadiscordbot/cogs/reaction_roles.py
 aadiscordbot/cogs/remind.py
```

### Comparing `allianceauth-discordbot-3.5.0/setup.py` & `allianceauth-discordbot-3.6.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,10 +37,10 @@
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     ],
     python_requires='>=3.8',
     install_requires=[
         "allianceauth>=2.9.0,<4.0.0",
         "py-cord>2.0.0,<3.0.0",
         "pendulum>=2.1.2,<3.0.0",
-        "aioredis>=2.0.0"
+        "redis>=4.2.0<5.0.0"
     ],
 )
```

