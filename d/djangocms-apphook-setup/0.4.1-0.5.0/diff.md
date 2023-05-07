# Comparing `tmp/djangocms-apphook-setup-0.4.1.tar.gz` & `tmp/djangocms-apphook-setup-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangocms-apphook-setup-0.4.1.tar", last modified: Sun Dec 22 21:39:12 2019, max compression
+gzip compressed data, was "djangocms-apphook-setup-0.5.0.tar", last modified: Sun May  7 16:47:20 2023, max compression
```

## Comparing `djangocms-apphook-setup-0.4.1.tar` & `djangocms-apphook-setup-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2019-12-22 21:39:12.000000 djangocms-apphook-setup-0.4.1/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      132 2015-10-24 17:04:19.000000 djangocms-apphook-setup-0.4.1/AUTHORS.rst
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     3328 2015-10-24 17:03:50.000000 djangocms-apphook-setup-0.4.1/CONTRIBUTING.rst
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      849 2019-12-22 21:38:59.000000 djangocms-apphook-setup-0.4.1/HISTORY.rst
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     1487 2015-10-24 17:03:50.000000 djangocms-apphook-setup-0.4.1/LICENSE
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      198 2015-10-24 17:03:50.000000 djangocms-apphook-setup-0.4.1/MANIFEST.in
--rw-rw-r--   0 yakky     (1000) yakky     (1000)    10502 2019-12-22 21:39:12.000000 djangocms-apphook-setup-0.4.1/PKG-INFO
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     6785 2019-12-22 17:07:25.000000 djangocms-apphook-setup-0.4.1/README.rst
-drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2019-12-22 21:39:12.000000 djangocms-apphook-setup-0.4.1/djangocms_apphook_setup/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      189 2019-12-22 21:38:59.000000 djangocms-apphook-setup-0.4.1/djangocms_apphook_setup/__init__.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     6998 2019-12-22 17:07:25.000000 djangocms-apphook-setup-0.4.1/djangocms_apphook_setup/base.py
-drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2019-12-22 21:39:12.000000 djangocms-apphook-setup-0.4.1/djangocms_apphook_setup.egg-info/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)    10502 2019-12-22 21:39:12.000000 djangocms-apphook-setup-0.4.1/djangocms_apphook_setup.egg-info/PKG-INFO
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      438 2019-12-22 21:39:12.000000 djangocms-apphook-setup-0.4.1/djangocms_apphook_setup.egg-info/SOURCES.txt
--rw-rw-r--   0 yakky     (1000) yakky     (1000)        1 2019-12-22 21:39:12.000000 djangocms-apphook-setup-0.4.1/djangocms_apphook_setup.egg-info/dependency_links.txt
--rw-rw-r--   0 yakky     (1000) yakky     (1000)        1 2019-12-22 21:39:12.000000 djangocms-apphook-setup-0.4.1/djangocms_apphook_setup.egg-info/not-zip-safe
--rw-rw-r--   0 yakky     (1000) yakky     (1000)       11 2019-12-22 21:39:12.000000 djangocms-apphook-setup-0.4.1/djangocms_apphook_setup.egg-info/requires.txt
--rw-rw-r--   0 yakky     (1000) yakky     (1000)       24 2019-12-22 21:39:12.000000 djangocms-apphook-setup-0.4.1/djangocms_apphook_setup.egg-info/top_level.txt
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      500 2019-12-22 21:39:12.000000 djangocms-apphook-setup-0.4.1/setup.cfg
--rwxrwxr-x   0 yakky     (1000) yakky     (1000)     1604 2019-12-22 21:38:59.000000 djangocms-apphook-setup-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:47:20.424675 djangocms-apphook-setup-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-07 16:46:34.000000 djangocms-apphook-setup-0.5.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-07 16:46:34.000000 djangocms-apphook-setup-0.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-07 16:46:34.000000 djangocms-apphook-setup-0.5.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-07 16:46:34.000000 djangocms-apphook-setup-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-07 16:46:34.000000 djangocms-apphook-setup-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-05-07 16:47:20.424675 djangocms-apphook-setup-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6873 2023-05-07 16:46:34.000000 djangocms-apphook-setup-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:47:20.424675 djangocms-apphook-setup-0.5.0/djangocms_apphook_setup/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-07 16:46:34.000000 djangocms-apphook-setup-0.5.0/djangocms_apphook_setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-05-07 16:46:34.000000 djangocms-apphook-setup-0.5.0/djangocms_apphook_setup/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:47:20.424675 djangocms-apphook-setup-0.5.0/djangocms_apphook_setup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-05-07 16:47:20.000000 djangocms-apphook-setup-0.5.0/djangocms_apphook_setup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-07 16:47:20.000000 djangocms-apphook-setup-0.5.0/djangocms_apphook_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 16:47:20.000000 djangocms-apphook-setup-0.5.0/djangocms_apphook_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 16:47:03.000000 djangocms-apphook-setup-0.5.0/djangocms_apphook_setup.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-07 16:47:20.000000 djangocms-apphook-setup-0.5.0/djangocms_apphook_setup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-07 16:47:20.000000 djangocms-apphook-setup-0.5.0/djangocms_apphook_setup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-07 16:46:34.000000 djangocms-apphook-setup-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-07 16:47:20.428675 djangocms-apphook-setup-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 16:46:34.000000 djangocms-apphook-setup-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:47:20.424675 djangocms-apphook-setup-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-05-07 16:46:34.000000 djangocms-apphook-setup-0.5.0/tests/test_setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `djangocms-apphook-setup-0.4.1/LICENSE` & `djangocms-apphook-setup-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-apphook-setup-0.4.1/README.rst` & `djangocms-apphook-setup-0.5.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 =======================
 djangocms-apphook-setup
 =======================
 
-|Gitter| |PyPiVersion| |PyVersion| |Status| |TestCoverage| |CodeClimate| |License|
+|Gitter| |PyPiVersion| |PyVersion| |GAStatus| |TestCoverage| |CodeClimate| |License|
 
 Utility function to auto setup apphooks on project startup.
 
 Supported Django versions:
 
-* Django 1.11 to 2.2
+* Django: 2.2, 3.0, 3.1
 
 Supported django CMS versions:
 
-* django CMS 3.5, 3.6, 3.7
+* django CMS: 3.7, 3.8
 
+********
 Features
---------
+********
 
 The mixin included in this utility allows to automatically add an Apphook to a django CMS
 project on the first access to the website.
 
 This is intended for use by the django CMS application developers by extending their own
 ``CMSApp`` classes.
 
@@ -38,16 +39,17 @@
 In case the application uses ``aldryn-apphooks-config``, a Apphook Config instance is created
 and added to the application page together with the Apphook.
 
 .. note:: To avoid issues with ``AldrynSearch`` during the creation of pages, the url of the
           pages is faked; this is normally not an issues as the pages will be reindexed
           whenever the content is updated.
 
+*****
 Usage
------
+*****
 
 This utility can be used by extending the ``CMSApp`` class, adding the ``auto_setup`` attribute
 with relevant configuration options and triggering setup at the end of ``cms_app.py``::
 
 
     @apphook_pool.register
     class App4(AutoCMSAppMixin, CMSConfigApp):
@@ -66,17 +68,17 @@
             'sites': True,
         }
 
 
     # trigger djangocms-apphook-setup function
     App4.setup()
 
-
+********************************************
 Customizing ApphookConfig instances creation
---------------------------------------------
+********************************************
 
 While ``config_fields`` and ``config_translated_fields`` should cover most use cases when it comes
 to ApphookConfig instances creation, you may need more control over the process.
 
 For this, it's possible to override ``AutoCMSAppMixin._create_config`` and
 ``AutoCMSAppMixin._create_config_translation``.
 
@@ -95,17 +97,17 @@
             setattr(config, field, data)
         config.save_translations()
 
 
 You can completely redefine the methods, provided you return an ApphookConfig instance
 in ``_create_config``.
 
-
+*********************
 Configuration options
----------------------
+*********************
 
 The behavior of the setup function can be customized by setting the following keys in the
 ``auto_setup`` attribute:
 
 * ``enabled``: If ``True`` the setup is invoked; a good option is to use a setting to control this
   to allow application users to disable the behavior (default: ``True``)
 * ``home title``: Title of the home page if created by the setup function; this **must** be set in
@@ -119,17 +121,17 @@
   for non-translated fields.
 * ``config_translated_fields``: Fields used when creating the ApphookConfigModel instance;
   use this attribute for translated fields (currently only ``django-parler`` is supported).
 * ``sites``: List of site ids for which to create the pages; if set to ``True`` (the default value)
   pages will be created for all sites. A single apphook config is created for all the sites;
   instance is created only on first page creation.
 
-
+****************
 Notes on testing
-----------------
+****************
 
 As this utility works by triggering setup function at import time, extra steps must be taken
 in the tests to unload the modules between the tests (this is only needed when testing the setup).
 
 Example cleanup to be included in ``setUp`` method::
 
     def setUp(self):
@@ -157,17 +159,17 @@
     :target: https://pypi.python.org/pypi/djangocms-apphook-setup
     :alt: Latest PyPI version
 
 .. |PyVersion| image:: https://img.shields.io/pypi/pyversions/djangocms-apphook-setup.svg?style=flat-square
     :target: https://pypi.python.org/pypi/djangocms-apphook-setup
     :alt: Python versions
 
-.. |Status| image:: https://img.shields.io/travis/nephila/djangocms-apphook-setup.svg?style=flat-square
-    :target: https://travis-ci.org/nephila/djangocms-apphook-setup
-    :alt: Latest Travis CI build status
+.. |GAStatus| image:: https://github.com/nephila/djangocms-apphook-setup/workflows/Tox%20tests/badge.svg
+    :target: https://github.com/nephila/djangocms-apphook-setup
+    :alt: Latest CI build status
 
 .. |TestCoverage| image:: https://img.shields.io/coveralls/nephila/djangocms-apphook-setup/master.svg?style=flat-square
     :target: https://coveralls.io/r/nephila/djangocms-apphook-setup?branch=master
     :alt: Test coverage
 
 .. |License| image:: https://img.shields.io/github/license/nephila/djangocms-apphook-setup.svg?style=flat-square
    :target: https://pypi.python.org/pypi/djangocms-apphook-setup/
```

### Comparing `djangocms-apphook-setup-0.4.1/djangocms_apphook_setup/base.py` & `djangocms-apphook-setup-0.5.0/djangocms_apphook_setup/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,27 @@
-# -*- coding: utf-8 -*-
-from __future__ import absolute_import, print_function, unicode_literals
-
 import warnings
 
 from django.contrib.sites.models import Site
 
 
-class AutoCMSAppMixin(object):
-
+class AutoCMSAppMixin:
     auto_setup = {
-        'enabled': True,
-        'home title': None,
-        'page title': None,
-        'namespace': None,
-        'config_fields': {},
-        'config_translated_fields': {},
-        'sites': True
+        "enabled": True,
+        "home title": None,
+        "page title": None,
+        "namespace": None,
+        "config_fields": {},
+        "config_translated_fields": {},
+        "sites": True,
     }
 
     @classmethod
-    def _create_page(cls, page, lang, auto_title, cms_app=None, parent=None, namespace=None,
-                     site=None, set_home=False):
+    def _create_page(
+        cls, page, lang, auto_title, cms_app=None, parent=None, namespace=None, site=None, set_home=False
+    ):
         """
         Create a single page or titles
 
         :param page: Page instance
         :param lang: language code
         :param auto_title: title text for the newly created title
         :param cms_app: Apphook Class to be attached to the page
@@ -36,25 +33,28 @@
         """
         from cms.api import create_page, create_title
         from cms.utils.conf import get_templates
 
         default_template = get_templates()[0][0]
         if page is None:
             page = create_page(
-                auto_title, language=lang, parent=parent, site=site,
-                template=default_template, in_navigation=True, published=True
+                auto_title,
+                language=lang,
+                parent=parent,
+                site=site,
+                template=default_template,
+                in_navigation=True,
+                published=True,
             )
             page.application_urls = cms_app
             page.application_namespace = namespace
             page.save()
             page.publish(lang)
         elif lang not in page.get_languages():
-            create_title(
-                language=lang, title=auto_title, page=page
-            )
+            create_title(language=lang, title=auto_title, page=page)
             page.publish(lang)
         if set_home:
             page.set_as_homepage()
         return page.get_draft_object()
 
     @classmethod
     def _create_config(cls):
@@ -62,17 +62,15 @@
         Creates an ApphookConfig instance
 
         ``AutoCMSAppMixin.auto_setup['config_fields']`` is used to fill in the data
         of the instance.
 
         :return: ApphookConfig instance
         """
-        return cls.app_config.objects.create(
-            namespace=cls.auto_setup['namespace'], **cls.auto_setup['config_fields']
-        )
+        return cls.app_config.objects.create(namespace=cls.auto_setup["namespace"], **cls.auto_setup["config_fields"])
 
     @classmethod
     def _create_config_translation(cls, config, lang):
         """
         Creates a translation for the given ApphookConfig
 
         Only django-parler kind of models are currently supported.
@@ -80,15 +78,15 @@
         ``AutoCMSAppMixin.auto_setup['config_translated_fields']`` is used to fill in the data
         of the instance for all the languages.
 
         :param config: ApphookConfig instance
         :param lang: language code for the language to create
         """
         config.set_current_language(lang, initialize=True)
-        for field, data in cls.auto_setup['config_translated_fields'].items():
+        for field, data in cls.auto_setup["config_translated_fields"].items():
             setattr(config, field, data)
         config.save_translations()
 
     @classmethod
     def _setup_pages(cls, config):
         """
         Create the page structure.
@@ -103,55 +101,52 @@
         from cms.models import Page
         from cms.utils import get_language_list
         from django.conf import settings
         from django.utils.translation import override
 
         app_page = None
         get_url = False
-        if getattr(settings, 'ALDRYN_SEARCH_CMS_PAGE', False):
+        if getattr(settings, "ALDRYN_SEARCH_CMS_PAGE", False):
             from aldryn_search.search_indexes import TitleIndex
 
             def fake_url(self, obj):
-                return ''
+                return ""
 
             get_url = TitleIndex.get_url
             TitleIndex.get_url = fake_url
         site = Site.objects.get_current()
-        auto_sites = cls.auto_setup.get('sites', True)
+        auto_sites = cls.auto_setup.get("sites", True)
         if auto_sites is True or site.pk in auto_sites:
-            if getattr(cls, 'app_config', False):
+            if getattr(cls, "app_config", False):
                 configs = cls.app_config.objects.all()
                 if not configs.exists():
                     config = cls._create_config()
                 else:
                     config = configs.first()
 
             langs = get_language_list(site.pk)
             if not Page.objects.on_site(site.pk).filter(application_urls=cls.__name__).exists():
                 for lang in langs:
                     with override(lang):
                         if config:
-                            if cls.auto_setup['config_translated_fields']:
+                            if cls.auto_setup["config_translated_fields"]:
                                 cls._create_config_translation(config, lang)
                             namespace = config.namespace
                         elif cls.app_name:
                             namespace = cls.app_name
                         else:
                             namespace = None
                         try:
                             home = Page.objects.get_home(site.pk).get_draft_object()
                         except NoHomeFound:
                             home = None
-                        set_home = hasattr(Page, 'set_as_homepage')
-                        home = cls._create_page(
-                            home, lang, cls.auto_setup['home title'], site=site, set_home=set_home
-                        )
+                        set_home = hasattr(Page, "set_as_homepage")
+                        home = cls._create_page(home, lang, cls.auto_setup["home title"], site=site, set_home=set_home)
                         app_page = cls._create_page(
-                            app_page, lang, cls.auto_setup['page title'], cls.__name__, home,
-                            namespace, site=site
+                            app_page, lang, cls.auto_setup["page title"], cls.__name__, home, namespace, site=site
                         )
         if get_url:
             TitleIndex.get_url = get_url
 
     @classmethod
     def setup(cls):
         """
@@ -159,29 +154,23 @@
 
         It must be called after the Apphook registration::
 
             apphook_pool.register(MyApp)
             MyApp.setup()
         """
         try:
-            if cls.auto_setup and cls.auto_setup.get('enabled', False):
-                if not cls.auto_setup.get('home title', False):
-                    warnings.warn(
-                        '"home title" is not set in {0}.auto_setup attribute'.format(cls)
-                    )
+            if cls.auto_setup and cls.auto_setup.get("enabled", False):
+                if not cls.auto_setup.get("home title", False):
+                    warnings.warn('"home title" is not set in {}.auto_setup attribute'.format(cls))
                     return
-                if not cls.auto_setup.get('page title', False):
-                    warnings.warn(
-                        '"page title" is not set in {0}.auto_setup attribute'.format(cls)
-                    )
+                if not cls.auto_setup.get("page title", False):
+                    warnings.warn('"page title" is not set in {}.auto_setup attribute'.format(cls))
                     return
-                if cls.app_name and not cls.auto_setup.get('namespace', False):
-                    warnings.warn(
-                        '"page title" is not set in {0}.auto_setup attribute'.format(cls)
-                    )
+                if cls.app_name and not cls.auto_setup.get("namespace", False):
+                    warnings.warn('"page title" is not set in {}.auto_setup attribute'.format(cls))
                     return
                 config = None
                 cls._setup_pages(config)
         except Exception:
             # Ignore any error during setup. Worst case: pages are not created, but the instance
             # won't break
             pass
```

