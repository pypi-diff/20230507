# Comparing `tmp/django-appdata-0.3.2.tar.gz` & `tmp/django-appdata-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-appdata-0.3.2.tar", last modified: Wed Oct 28 08:23:04 2020, max compression
+gzip compressed data, was "django-appdata-0.4.0.tar", last modified: Sun May  7 16:00:29 2023, max compression
```

## Comparing `django-appdata-0.3.2.tar` & `django-appdata-0.4.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-10-28 08:23:04.000000 django-appdata-0.3.2/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     1483 2020-10-15 12:52:04.000000 django-appdata-0.3.2/LICENSE
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      216 2020-10-15 12:52:04.000000 django-appdata-0.3.2/MANIFEST.in
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     8578 2020-10-28 08:23:04.000000 django-appdata-0.3.2/PKG-INFO
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     6160 2020-10-15 12:52:04.000000 django-appdata-0.3.2/README.rst
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-10-28 08:23:04.000000 django-appdata-0.3.2/app_data/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      219 2015-01-03 07:27:33.000000 django-appdata-0.3.2/app_data/__init__.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     4781 2020-10-28 08:19:19.000000 django-appdata-0.3.2/app_data/admin.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     7916 2020-05-12 16:01:15.000000 django-appdata-0.3.2/app_data/containers.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     3053 2020-05-12 16:01:15.000000 django-appdata-0.3.2/app_data/fields.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)    10783 2020-05-12 16:01:15.000000 django-appdata-0.3.2/app_data/forms.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     1995 2015-01-03 07:27:33.000000 django-appdata-0.3.2/app_data/registry.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)       14 2020-10-13 08:35:55.000000 django-appdata-0.3.2/dev_requirements.txt
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-10-28 08:23:04.000000 django-appdata-0.3.2/django_appdata.egg-info/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     8578 2020-10-28 08:23:04.000000 django-appdata-0.3.2/django_appdata.egg-info/PKG-INFO
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      764 2020-10-28 08:23:04.000000 django-appdata-0.3.2/django_appdata.egg-info/SOURCES.txt
--rw-rw-r--   0 yakky     (1000) yakky     (1000)        1 2020-10-28 08:23:04.000000 django-appdata-0.3.2/django_appdata.egg-info/dependency_links.txt
--rw-rw-r--   0 yakky     (1000) yakky     (1000)        1 2015-01-03 07:28:03.000000 django-appdata-0.3.2/django_appdata.egg-info/not-zip-safe
--rw-rw-r--   0 yakky     (1000) yakky     (1000)       11 2020-10-28 08:23:04.000000 django-appdata-0.3.2/django_appdata.egg-info/requires.txt
--rw-rw-r--   0 yakky     (1000) yakky     (1000)        9 2020-10-28 08:23:04.000000 django-appdata-0.3.2/django_appdata.egg-info/top_level.txt
--rw-rw-r--   0 yakky     (1000) yakky     (1000)       38 2020-10-28 08:23:04.000000 django-appdata-0.3.2/setup.cfg
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     1568 2020-10-28 08:19:31.000000 django-appdata-0.3.2/setup.py
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-10-28 08:23:04.000000 django-appdata-0.3.2/test_app_data/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      499 2019-01-11 06:55:49.000000 django-appdata-0.3.2/test_app_data/__init__.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      674 2020-10-28 08:19:19.000000 django-appdata-0.3.2/test_app_data/admin.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      693 2019-01-11 06:55:49.000000 django-appdata-0.3.2/test_app_data/cases.py
--rwxrwxr-x   0 yakky     (1000) yakky     (1000)      727 2015-01-03 07:27:33.000000 django-appdata-0.3.2/test_app_data/manage.py
-drwxrwsr-x   0 yakky     (1000) yakky     (1000)        0 2020-10-28 08:23:04.000000 django-appdata-0.3.2/test_app_data/migrations/
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     2180 2019-01-11 06:55:49.000000 django-appdata-0.3.2/test_app_data/migrations/0001_initial.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)        0 2019-01-11 06:55:49.000000 django-appdata-0.3.2/test_app_data/migrations/__init__.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     1620 2019-01-11 06:55:49.000000 django-appdata-0.3.2/test_app_data/models.py
--rwxrwxr-x   0 yakky     (1000) yakky     (1000)      788 2019-01-11 06:55:49.000000 django-appdata-0.3.2/test_app_data/run_tests.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     1429 2020-10-28 08:19:19.000000 django-appdata-0.3.2/test_app_data/settings.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     2441 2019-01-11 06:55:49.000000 django-appdata-0.3.2/test_app_data/test_admin.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     7053 2019-01-11 06:55:49.000000 django-appdata-0.3.2/test_app_data/test_fields.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)     8377 2019-01-11 06:55:49.000000 django-appdata-0.3.2/test_app_data/test_forms.py
--rw-rw-r--   0 yakky     (1000) yakky     (1000)      234 2019-01-11 06:55:49.000000 django-appdata-0.3.2/test_app_data/urls.py
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:00:29.821337 django-appdata-0.4.0/
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     1483 2023-02-12 11:19:46.000000 django-appdata-0.4.0/LICENSE
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      111 2023-05-07 15:52:57.000000 django-appdata-0.4.0/MANIFEST.in
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     7095 2023-05-07 16:00:29.821337 django-appdata-0.4.0/PKG-INFO
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     6141 2023-05-07 15:59:47.000000 django-appdata-0.4.0/README.rst
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:00:29.821337 django-appdata-0.4.0/app_data/
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      298 2023-05-07 15:59:15.000000 django-appdata-0.4.0/app_data/__init__.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     4696 2023-05-07 15:52:57.000000 django-appdata-0.4.0/app_data/admin.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     7756 2023-05-07 15:52:57.000000 django-appdata-0.4.0/app_data/containers.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     2931 2023-05-07 15:52:57.000000 django-appdata-0.4.0/app_data/fields.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)    11021 2023-05-07 15:52:57.000000 django-appdata-0.4.0/app_data/forms.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     1923 2023-05-07 15:52:57.000000 django-appdata-0.4.0/app_data/registry.py
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:00:29.821337 django-appdata-0.4.0/django_appdata.egg-info/
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     7095 2023-05-07 16:00:29.000000 django-appdata-0.4.0/django_appdata.egg-info/PKG-INFO
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      767 2023-05-07 16:00:29.000000 django-appdata-0.4.0/django_appdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)        1 2023-05-07 16:00:29.000000 django-appdata-0.4.0/django_appdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)        1 2023-02-12 11:26:51.000000 django-appdata-0.4.0/django_appdata.egg-info/not-zip-safe
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)        7 2023-05-07 16:00:29.000000 django-appdata-0.4.0/django_appdata.egg-info/requires.txt
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)        9 2023-05-07 16:00:29.000000 django-appdata-0.4.0/django_appdata.egg-info/top_level.txt
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      496 2023-05-07 15:52:57.000000 django-appdata-0.4.0/pyproject.toml
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     1274 2023-05-07 16:00:29.825337 django-appdata-0.4.0/setup.cfg
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)       38 2023-05-07 15:52:57.000000 django-appdata-0.4.0/setup.py
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:00:29.821337 django-appdata-0.4.0/test_app_data/
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      499 2023-05-07 15:52:57.000000 django-appdata-0.4.0/test_app_data/__init__.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      660 2023-05-07 15:52:57.000000 django-appdata-0.4.0/test_app_data/admin.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      650 2023-05-07 15:52:57.000000 django-appdata-0.4.0/test_app_data/cases.py
+-rwxrwxr-x   0 yakky     (1000) yakky     (1000)      727 2023-05-07 15:52:57.000000 django-appdata-0.4.0/test_app_data/manage.py
+drwxrwxr-x   0 yakky     (1000) yakky     (1000)        0 2023-05-07 16:00:29.821337 django-appdata-0.4.0/test_app_data/migrations/
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     3396 2023-05-07 15:52:57.000000 django-appdata-0.4.0/test_app_data/migrations/0001_initial.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)        0 2023-02-12 11:19:46.000000 django-appdata-0.4.0/test_app_data/migrations/__init__.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     1615 2023-05-07 15:52:57.000000 django-appdata-0.4.0/test_app_data/models.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      406 2023-05-07 15:52:57.000000 django-appdata-0.4.0/test_app_data/runtests.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     1129 2023-05-07 15:52:57.000000 django-appdata-0.4.0/test_app_data/settings.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     2295 2023-05-07 15:52:57.000000 django-appdata-0.4.0/test_app_data/test_admin.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     7036 2023-05-07 15:52:57.000000 django-appdata-0.4.0/test_app_data/test_fields.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)     8434 2023-05-07 15:52:57.000000 django-appdata-0.4.0/test_app_data/test_forms.py
+-rw-rw-r--   0 yakky     (1000) yakky     (1000)      228 2023-05-07 15:52:57.000000 django-appdata-0.4.0/test_app_data/urls.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-appdata-0.3.2/LICENSE` & `django-appdata-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-appdata-0.3.2/PKG-INFO` & `django-appdata-0.4.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,206 +1,207 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-appdata
-Version: 0.3.2
+Version: 0.4.0
 Summary: Extendable field that enables Django apps to store their data on your models.
-Home-page: https://github.com/ella/django-appdata/
+Home-page: https://github.com/ella/django-appdata
 Author: Ella Development Team
 Author-email: dev@ellaproject.cz
 License: BSD
-Description: Django AppData
-        ##############
-        
-        Extandable field and related tools that enable Django apps to extend your
-        reusable app.
-        
-        Motivation
-        **********
-        
-        When working with reusable django apps we often found that we needed to add
-        something extra to the model or form the app provided. Some apps try to solve
-        this by providing a flexible model definition and a pluggable form (see
-        ``django.contrib.comments`` for an exmple of this approach) but even then it
-        leads to some duplication of efforts.
-        
-        ``django-appdata`` app tries, through ``AppDataField``, ``MultiForm`` and ``AppDataModelAdmin``,
-        to provide a standardised approach to extending existing apps.
-        
-        Supported versions
-        ******************
-        
-        Python: 2.7, 3.5, 3.6, 3.7, 3.8
-        Django: 1.11, 2.2, 3.0, 3.1
-        
-        Upgrading to 0.3
-        ****************
-        
-        If you are upgrading from a 0.2.x version, please note the following incompatible changes in 0.3
-        
-        * Dropped Django < 1.11 and Python 3.4 compatibility
-        
-        
-        Extending Models
-        ****************
-        
-        When you have an extendable django app using the ``AppDataField``::
-        
-            from django.db import models
-            from app_data import AppDataField
-        
-            class BlogPost(models.Model):
-                text = models.TextField()
-                app_data = AppDataField()
-        
-        your code can register a namespace on any (or all) ``AppDataField`` and store
-        it's own data there by registering a *container* (subclass of
-        ``AppDataContainer``). To define the data you use django's form framework::
-        
-            from django.forms.models import ModelMultipleChoiceField
-            from app_data import app_registry, AppDataForm, AppDataContainer
-        
-            from .models import Tag
-        
-            class TaggingAppDataForm(AppDataForm):
-                public_tags = ModelMultipleChoiceField(Tag.objects.all())
-                admin_tags = ModelMultipleChoiceField(Tag.objects.all())
-        
-            class TaggingAppDataContainer(AppDataContainer):
-                form_class = TaggingAppDataForm
-        
-                def tag_string(self):
-                    print ', '.join(t.name for t in self.public_tags)
-        
-            app_registry.register('tagging', TaggingAppDataContainer)
-        
-        This should give you access to ``'tagging'`` namespace in any defined ``AppDataField``::
-        
-            from blog_app.models import BlogPost
-        
-            bp = BlogPost()
-            assert bp.app_data.tagging.tag_string() == ""
-        
-        
-        Additional Options
-        ~~~~~~~~~~~~~~~~~~
-        
-        Note that if you don't need to add custom methods to your container you can
-        just use a factory to create the subclass::
-        
-            app_registry.register('tagging', AppDataContainer.from_form(TaggingAppDataForm))
-        
-        Additionaly you can restrict the registration to a given model::
-        
-            from blog_app.models import BlogPost
-        
-            app_registry.register('tagging', TaggingAppDataContainer, BlogPost)
-        
-        Extending Forms
-        ***************
-        
-        ``django-appdata`` supplies a ``MultiForm`` class - a wrapper around django's ``ModelForm``
-        with optional added sub-forms that corresponds to namespaces registered in the
-        model's ``AppDataField``, typically the extendable app would create and use a
-        ``MultiForm`` instead of a regular ``ModelForm``::
-        
-            from app_data.forms import multiform_factory
-            from .models import BlogPost
-        
-            BlogPostMultiForm = multiform_factory(BlogPost)
-        
-        And when using that app any project can add additional sub-forms to that ``MultiForm``::
-        
-            from blog_app.forms import BlogPostMultiForm
-        
-            BlogPostMultiForm.add_form('tagging', {'fields': ['public_tags']})
-        
-        This way when the reusable app's code can remain unchanged and we can inject
-        additional form logic to its processing.
-        
-        Additional Options
-        ~~~~~~~~~~~~~~~~~~
-        
-        Any arguments and keyword arguments are passed without change to the
-        ``ModelForm`` class the ``MultiForm`` is wrapping so even if you have custom args
-        for your ``ModelForm`` everything will still work::
-        
-            from django.forms.models import BaseModelForm
-        
-            class ModelFormWithUser(ModelForm):
-                def __init__(self, user, *args, **kwargs):
-                    self.user = user
-                    super(ModelFormWithUser, self).__init__(*args, **kwargs)
-        
-            BlogPostMultiForm = multiform_factory(BlogPost, form=ModelFormWithUser)
-        
-        And of course you are not limited to the use of a factory function::
-        
-            from app_data import MultiForm
-        
-            class MyMultiForm(MultiForm):
-                ModelForm = BlogPostModelForm
-        
-        MultiForms in Admin
-        *******************
-        
-        If you wish to add your own code to the admin interface, just use
-        ``AppDataModelAdmin``::
-        
-            from django.contrib import admin
-            from app_data.admin import AppDataModelAdmin
-            from blog_app.models import BlogPost
-        
-            class BlogPostAdmin(AppDataModelAdmin):
-                # due to the behavior of django admin validation we need to use
-                # get_fieldsets instead of just fieldsets
-                def get_fieldsets(self, request, obj=None):
-                     return [
-                         (None, {'fields': ['text', ]}),
-                         ('Tagging', {'fields': [('tagging.public_tags', 'tagging.admin_tags')]})
-                     ]
-            admin.site.register(BlogPost, BlogPostAdmin)
-        
-        Additional Options
-        ~~~~~~~~~~~~~~~~~~
-        
-        As with django's admin and forms you can supply your own ``MultiForm`` class by
-        using the ``multiform`` attribute of ``AppDataModelAdmin``.
-        
-        Behind the scenes
-        *****************
-        
-        ``django-appdata`` uses a ``TextField`` to store the data on the model using JSON
-        and django's forms framework for (de)serialization and validation of the data.
-        
-        When accessing the containers in the field we will try to locate the
-        appropriate container in the registry. If none is found, plain data will be
-        returned if present (dict). To assure everything working properly we recommend
-        putting some sort of init code in place for your project that will make sure all
-        the registration is done before any actual code is run. We are using a module
-        called ``register`` in our apps and then a `piece of code`_ similar to admin's
-        autodiscover to iterate through installed apps and load this module.
-        
-        .. _`piece of code`: https://github.com/ella/ella/blob/master/ella/utils/installedapps.py#L27
-        
-        Build status
-        ************
-        
-        :Master branch:
-        
-          .. image:: https://secure.travis-ci.org/ella/django-appdata.png?branch=master
-             :alt: Travis CI - Distributed build platform for the open source community
-             :target: http://travis-ci.org/#!/ella/django-appdata
-Platform: UNKNOWN
+Project-URL: Documentation, https://django-appdata.readthedocs.io/
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 1.11
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Django AppData
+##############
+
+Extendable field and related tools that enable Django apps to extend your
+reusable app.
+
+Motivation
+**********
+
+When working with reusable django apps we often found that we needed to add
+something extra to the model or form the app provided. Some apps try to solve
+this by providing a flexible model definition and a pluggable form (see
+``django.contrib.comments`` for an exmple of this approach) but even then it
+leads to some duplication of efforts.
+
+``django-appdata`` app tries, through ``AppDataField``, ``MultiForm`` and ``AppDataModelAdmin``,
+to provide a standardised approach to extending existing apps.
+
+Supported versions
+******************
+
+Python: 3.9, 3.10, 3.11
+Django: 3.2, 4.2
+
+Upgrading to 0.4
+****************
+
+If you are upgrading from a 0.3.x version, please note the following incompatible changes in 0.4
+
+* Dropped Django < 3.2 and Python < 3.9 compatibility
+
+
+Extending Models
+****************
+
+When you have an extendable django app using the ``AppDataField``::
+
+    from django.db import models
+    from app_data import AppDataField
+
+    class BlogPost(models.Model):
+        text = models.TextField()
+        app_data = AppDataField()
+
+your code can register a namespace on any (or all) ``AppDataField`` and store
+it's own data there by registering a *container* (subclass of
+``AppDataContainer``). To define the data you use django's form framework::
+
+    from django.forms.models import ModelMultipleChoiceField
+    from app_data import app_registry, AppDataForm, AppDataContainer
+
+    from .models import Tag
+
+    class TaggingAppDataForm(AppDataForm):
+        public_tags = ModelMultipleChoiceField(Tag.objects.all())
+        admin_tags = ModelMultipleChoiceField(Tag.objects.all())
+
+    class TaggingAppDataContainer(AppDataContainer):
+        form_class = TaggingAppDataForm
+
+        def tag_string(self):
+            print ', '.join(t.name for t in self.public_tags)
+
+    app_registry.register('tagging', TaggingAppDataContainer)
+
+This should give you access to ``'tagging'`` namespace in any defined ``AppDataField``::
+
+    from blog_app.models import BlogPost
+
+    bp = BlogPost()
+    assert bp.app_data.tagging.tag_string() == ""
+
+
+Additional Options
+~~~~~~~~~~~~~~~~~~
+
+Note that if you don't need to add custom methods to your container you can
+just use a factory to create the subclass::
+
+    app_registry.register('tagging', AppDataContainer.from_form(TaggingAppDataForm))
+
+Additionaly you can restrict the registration to a given model::
+
+    from blog_app.models import BlogPost
+
+    app_registry.register('tagging', TaggingAppDataContainer, BlogPost)
+
+Extending Forms
+***************
+
+``django-appdata`` supplies a ``MultiForm`` class - a wrapper around django's ``ModelForm``
+with optional added sub-forms that corresponds to namespaces registered in the
+model's ``AppDataField``, typically the extendable app would create and use a
+``MultiForm`` instead of a regular ``ModelForm``::
+
+    from app_data.forms import multiform_factory
+    from .models import BlogPost
+
+    BlogPostMultiForm = multiform_factory(BlogPost)
+
+And when using that app any project can add additional sub-forms to that ``MultiForm``::
+
+    from blog_app.forms import BlogPostMultiForm
+
+    BlogPostMultiForm.add_form('tagging', {'fields': ['public_tags']})
+
+This way when the reusable app's code can remain unchanged and we can inject
+additional form logic to its processing.
+
+Additional Options
+~~~~~~~~~~~~~~~~~~
+
+Any arguments and keyword arguments are passed without change to the
+``ModelForm`` class the ``MultiForm`` is wrapping so even if you have custom args
+for your ``ModelForm`` everything will still work::
+
+    from django.forms.models import BaseModelForm
+
+    class ModelFormWithUser(ModelForm):
+        def __init__(self, user, *args, **kwargs):
+            self.user = user
+            super(ModelFormWithUser, self).__init__(*args, **kwargs)
+
+    BlogPostMultiForm = multiform_factory(BlogPost, form=ModelFormWithUser)
+
+And of course you are not limited to the use of a factory function::
+
+    from app_data import MultiForm
+
+    class MyMultiForm(MultiForm):
+        ModelForm = BlogPostModelForm
+
+MultiForms in Admin
+*******************
+
+If you wish to add your own code to the admin interface, just use
+``AppDataModelAdmin``::
+
+    from django.contrib import admin
+    from app_data.admin import AppDataModelAdmin
+    from blog_app.models import BlogPost
+
+    class BlogPostAdmin(AppDataModelAdmin):
+        # due to the behavior of django admin validation we need to use
+        # get_fieldsets instead of just fieldsets
+        def get_fieldsets(self, request, obj=None):
+             return [
+                 (None, {'fields': ['text', ]}),
+                 ('Tagging', {'fields': [('tagging.public_tags', 'tagging.admin_tags')]})
+             ]
+    admin.site.register(BlogPost, BlogPostAdmin)
+
+Additional Options
+~~~~~~~~~~~~~~~~~~
+
+As with django's admin and forms you can supply your own ``MultiForm`` class by
+using the ``multiform`` attribute of ``AppDataModelAdmin``.
+
+Behind the scenes
+*****************
+
+``django-appdata`` uses a ``TextField`` to store the data on the model using JSON
+and django's forms framework for (de)serialization and validation of the data.
+
+When accessing the containers in the field we will try to locate the
+appropriate container in the registry. If none is found, plain data will be
+returned if present (dict). To assure everything working properly we recommend
+putting some sort of init code in place for your project that will make sure all
+the registration is done before any actual code is run. We are using a module
+called ``register`` in our apps and then a `piece of code`_ similar to admin's
+autodiscover to iterate through installed apps and load this module.
+
+.. _`piece of code`: https://github.com/ella/ella/blob/master/ella/utils/installedapps.py#L27
+
+Build status
+************
+
+:Master branch:
+
+  .. image:: https://secure.travis-ci.org/ella/django-appdata.png?branch=master
+     :alt: Travis CI - Distributed build platform for the open source community
+     :target: http://travis-ci.org/#!/ella/django-appdata
```

### Comparing `django-appdata-0.3.2/README.rst` & `django-appdata-0.4.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Django AppData
 ##############
 
-Extandable field and related tools that enable Django apps to extend your
+Extendable field and related tools that enable Django apps to extend your
 reusable app.
 
 Motivation
 **********
 
 When working with reusable django apps we often found that we needed to add
 something extra to the model or form the app provided. Some apps try to solve
@@ -15,23 +15,23 @@
 
 ``django-appdata`` app tries, through ``AppDataField``, ``MultiForm`` and ``AppDataModelAdmin``,
 to provide a standardised approach to extending existing apps.
 
 Supported versions
 ******************
 
-Python: 2.7, 3.5, 3.6, 3.7, 3.8
-Django: 1.11, 2.2, 3.0, 3.1
+Python: 3.9, 3.10, 3.11
+Django: 3.2, 4.2
 
-Upgrading to 0.3
+Upgrading to 0.4
 ****************
 
-If you are upgrading from a 0.2.x version, please note the following incompatible changes in 0.3
+If you are upgrading from a 0.3.x version, please note the following incompatible changes in 0.4
 
-* Dropped Django < 1.11 and Python 3.4 compatibility
+* Dropped Django < 3.2 and Python < 3.9 compatibility
 
 
 Extending Models
 ****************
 
 When you have an extendable django app using the ``AppDataField``::
 
@@ -176,8 +176,7 @@
 ************
 
 :Master branch:
 
   .. image:: https://secure.travis-ci.org/ella/django-appdata.png?branch=master
      :alt: Travis CI - Distributed build platform for the open source community
      :target: http://travis-ci.org/#!/ella/django-appdata
-
```

### Comparing `django-appdata-0.3.2/app_data/admin.py` & `django-appdata-0.4.0/app_data/admin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,124 +1,122 @@
 from functools import partial
 
-from django.contrib.admin.utils import flatten_fieldsets
-from django.contrib.admin.options import ModelAdmin, InlineModelAdmin
 from django import forms
+from django.contrib.admin.options import InlineModelAdmin, ModelAdmin
+from django.contrib.admin.utils import flatten_fieldsets
 from django.forms.models import modelform_defines_fields
 
-from app_data.forms import multiform_factory, multiinlineformset_factory, MultiForm, AppDataBaseInlineFormSet
+from app_data.forms import AppDataBaseInlineFormSet, MultiForm, multiform_factory, multiinlineformset_factory
 
 
-class AppDataAdminMixin(object):
-
+class AppDataAdminMixin:
     multiform = MultiForm
     app_form_opts = {}
 
     def get_fieldsets(self, request, obj=None):
         try:
             return self.declared_fieldsets
         except AttributeError:
-            return super(AppDataAdminMixin, self).get_fieldsets(request, obj)
+            return super().get_fieldsets(request, obj)
 
     def _get_form_factory_opts(self, request, obj=None, **kwargs):
         fieldsets = self.get_fieldsets(request, obj)
         if fieldsets:
             fields = flatten_fieldsets(fieldsets)
         else:
             fields = None
         if self.exclude is None:
             exclude = []
         else:
             exclude = list(self.exclude)
         exclude.extend(self.get_readonly_fields(request, obj))
-        if self.exclude is None and hasattr(self.form, '_meta') and self.form._meta.exclude:
+        if self.exclude is None and hasattr(self.form, "_meta") and self.form._meta.exclude:
             # Take the custom ModelForm's Meta.exclude into account only if the
             # ModelAdmin doesn't define its own.
             exclude.extend(self.form._meta.exclude)
 
         # construct the form_opts from declared_fieldsets
         form_opts = self.app_form_opts.copy()
         if fields is not None:
             # put app_name prefixed fields into form_opts
             for f in fields:
-                if '.' not in f:
+                if "." not in f:
                     continue
-                label, name = f.split('.')
-                app_fields = form_opts.setdefault(label, {}).setdefault('fields', [])
+                label, name = f.split(".")
+                app_fields = form_opts.setdefault(label, {}).setdefault("fields", [])
                 if name not in app_fields:
                     app_fields.append(name)
             # .. and remove them from fields for the model form
-            fields = [f for f in fields if '.' not in f]
+            fields = [f for f in fields if "." not in f]
 
         # do the same for exclude
         for f in exclude:
-            if '.' not in f:
+            if "." not in f:
                 continue
-            label, name = f.split('.')
-            app_fields = form_opts.setdefault(label, {}).setdefault('exclude', [])
+            label, name = f.split(".")
+            app_fields = form_opts.setdefault(label, {}).setdefault("exclude", [])
             if name not in app_fields:
                 app_fields.append(name)
-        exclude = [f for f in exclude if '.' not in f]
+        exclude = [f for f in exclude if "." not in f]
 
         # Django 3.1 always adds the fields attribute to the kwargs
         # and we must remove appdata fields from this list
-        kwargs["fields"] = [f for f in fields if '.' not in kwargs.get("fields", [])]
+        kwargs["fields"] = [f for f in fields if "." not in kwargs.get("fields", [])]
 
         # if exclude is an empty list we pass None to be consistant with the
         # default on modelform_factory
         exclude = exclude or None
         defaults = {
             "form": self.form,
             "multiform": self.multiform,
             "form_opts": form_opts,
             "fields": fields,
             "exclude": exclude,
             "formfield_callback": partial(self.formfield_for_dbfield, request=request),
         }
         defaults.update(kwargs)
 
-        if hasattr(forms, 'ALL_FIELDS'):
+        if hasattr(forms, "ALL_FIELDS"):
             # Django 1.7
-            if defaults['fields'] is None and not modelform_defines_fields(defaults['form']):
-                defaults['fields'] = forms.ALL_FIELDS
+            if defaults["fields"] is None and not modelform_defines_fields(defaults["form"]):
+                defaults["fields"] = forms.ALL_FIELDS
 
         return defaults
 
 
 class AppDataModelAdmin(AppDataAdminMixin, ModelAdmin):
     def get_form(self, request, obj=None, change=False, **kwargs):
         """
         Returns a Form class for use in the admin add view. This is used by
         add_view and change_view.
         """
         if self.multiform is None:
-            return super(AppDataModelAdmin, self).get_form(request, obj=obj, **kwargs)
+            return super().get_form(request, obj=obj, **kwargs)
         return multiform_factory(self.model, **self._get_form_factory_opts(request, obj, **kwargs))
 
 
 class AppDataInlineModelAdmin(AppDataAdminMixin, InlineModelAdmin):
     formset = AppDataBaseInlineFormSet
 
     def get_formset(self, request, obj=None, **kwargs):
         if self.multiform is None:
-            return super(AppDataInlineModelAdmin, self).get_formset(request, obj=obj, **kwargs)
+            return super().get_formset(request, obj=obj, **kwargs)
         can_delete = self.can_delete
-        if hasattr(self, 'has_delete_permission'):
+        if hasattr(self, "has_delete_permission"):
             can_delete = can_delete and self.has_delete_permission(request, obj)
         defaults = {
             "formset": self.formset,
             "fk_name": self.fk_name,
             "extra": self.extra,
             "max_num": self.max_num,
             "can_delete": can_delete,
         }
         defaults.update(self._get_form_factory_opts(request, obj, **kwargs))
         return multiinlineformset_factory(self.parent_model, self.model, **defaults)
 
 
 class AppDataStackedInline(AppDataInlineModelAdmin):
-    template = 'admin/edit_inline/stacked.html'
+    template = "admin/edit_inline/stacked.html"
 
 
 class AppDataTabularInline(AppDataInlineModelAdmin):
-    template = 'admin/edit_inline/tabular.html'
-
+    template = "admin/edit_inline/tabular.html"
```

### Comparing `django-appdata-0.3.2/app_data/containers.py` & `django-appdata-0.4.0/app_data/containers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,73 +1,71 @@
 from copy import copy
 
-import six
-
 from django.core.exceptions import ValidationError
 
-from .registry import app_registry
 from .forms import AppDataForm
+from .registry import app_registry
 
 
 class AppDataContainerFactory(dict):
     def __init__(self, model_instance, *args, **kwargs):
         self._model = model_instance.__class__
         self._instance = model_instance
-        self._app_registry = kwargs.pop('app_registry', app_registry)
-        super(AppDataContainerFactory, self).__init__(*args, **kwargs)
+        self._app_registry = kwargs.pop("app_registry", app_registry)
+        super().__init__(*args, **kwargs)
 
     def __repr__(self):
-        return '<AppDataContainerFactory: %s>' % super(AppDataContainerFactory, self).__repr__()
+        return "<AppDataContainerFactory: %s>" % super().__repr__()
 
     def __setattr__(self, name, value):
-        if name.startswith('_') or self._app_registry.get_class(name, self._model) is None:
-            super(AppDataContainerFactory, self).__setattr__(name, value)
+        if name.startswith("_") or self._app_registry.get_class(name, self._model) is None:
+            super().__setattr__(name, value)
         else:
             self[name] = copy(value)
 
     def __getattr__(self, name):
-        if name.startswith('_') or self._app_registry.get_class(name, self._model) is None:
-            raise AttributeError('No Container registered under %s for class %s' % (name, self._model.__name__))
+        if name.startswith("_") or self._app_registry.get_class(name, self._model) is None:
+            raise AttributeError("No Container registered under {} for class {}".format(name, self._model.__name__))
         return self[name]
 
     def __getitem__(self, name):
         class_ = self._app_registry.get_class(name, self._model)
         try:
-            val = super(AppDataContainerFactory, self).__getitem__(name)
+            val = super().__getitem__(name)
         except KeyError:
             if class_ is None:
                 raise
             val = class_(self._instance)
             self[name] = val
         else:
             if class_ is not None and not isinstance(val, class_):
                 val = class_(self._instance, val)
                 self[name] = val
 
         return val
 
     def __reduce__(self):
-        return (dict, (self.serialize(), ))
+        return (dict, (self.serialize(),))
 
     def validate(self, model_instance):
         errors = {}
-        for key, value in six.iteritems(self):
-            if hasattr(value, 'validate') and getattr(value, 'accessed', True):
+        for key, value in self.items():
+            if hasattr(value, "validate") and getattr(value, "accessed", True):
                 try:
                     value.validate(self, model_instance)
                 except ValidationError as e:
                     errors[key] = e.message_dict
         if errors:
             raise ValidationError(errors)
 
     def serialize(self):
-        for key, value in six.iteritems(self):
+        for key, value in self.items():
             if isinstance(value, AppDataContainer):
                 value = value.serialize() if value.accessed else value._data
-                super(AppDataContainerFactory, self).__setitem__(key, value)
+                super().__setitem__(key, value)
         # return a copy so that it's a fresh dict, not AppDataContainerFactory
         return self.copy()
 
     def get(self, name, default=None):
         if name in self:
             return self[name]
 
@@ -80,46 +78,50 @@
 
         return default
 
 
 INITIAL = object()
 
 
-class AppDataContainer(object):
+class AppDataContainer:
     form_class = AppDataForm
 
     @classmethod
     def from_form(cls, form_class):
-        return type('%sAppDataContainer' % form_class.__name__, (cls, ), {'fields': {}, 'form_class': form_class})
+        return type(
+            "%sAppDataContainer" % form_class.__name__,
+            (cls,),
+            {"fields": {}, "form_class": form_class},
+        )
 
     @property
     def accessed(self):
         """Return a boolean indicating whether the data have been accessed."""
         return self._accessed
 
     def __init__(self, model_instance, *args, **kwargs):
         self._data = dict(*args, **kwargs)
         self._attr_cache = {}
         self._accessed = False
         self._instance = model_instance
 
     def __repr__(self):
-        return '<%s: %r>' % (self.__class__.__name__, self.serialize())
+        return "<{}: {!r}>".format(self.__class__.__name__, self.serialize())
 
     def __eq__(self, other):
         if isinstance(other, AppDataContainer):
             return self.serialize() == other.serialize()
         elif isinstance(other, dict):
             return other == self.serialize()
         return False
 
     @property
     def _form(self):
         """Form instance used to clean/(de)serialize field values."""
-        if not hasattr(self, '_form_instance'):
+        if not hasattr(self, "_form_instance"):
             self._form_instance = self.get_form()
         return self._form_instance
 
     def __setitem__(self, name, value):
         self._accessed = True
         # if dealing with defined field...
         if name in self._form.fields:
@@ -127,16 +129,16 @@
             self._attr_cache[name] = value
         else:
             # fallback to behaving as normal dict otherwise
             self._data[name] = value
 
     def __setattr__(self, name, value):
         """Provide access to fields as attributes."""
-        if name.startswith('_'):
-            super(AppDataContainer, self).__setattr__(name, value)
+        if name.startswith("_"):
+            super().__setattr__(name, value)
         else:
             self.__setitem__(name, value)
 
     def __getitem__(self, name):
         self._accessed = True
 
         # defined field, still uncleaned, retrieve from self._form and put in cache
@@ -152,15 +154,15 @@
         if name in self._attr_cache:
             return self._attr_cache[name]
 
         return self._data[name]
 
     def __getattr__(self, name):
         """Provide access to fields as attributes."""
-        if name.startswith('_'):
+        if name.startswith("_"):
             raise AttributeError(name)
         try:
             return self.__getitem__(name)
         except KeyError:
             raise AttributeError(name)
 
     def __delitem__(self, name):
@@ -175,37 +177,37 @@
             return self[name]
         except KeyError:
             if default is INITIAL:
                 return None
             return default
 
     def update(self, data):
-        for k, v in six.iteritems(data):
+        for k, v in data.items():
             self[k] = v
 
     def validate(self, app_data, model_instance):
         self.serialize()
         form = self.get_form(self._data)
         if not form.is_valid():
             raise ValidationError(form.errors)
 
     def serialize(self):
         """Go through attribute cache and use ._form to serialze those values into ._data."""
-        for name, value in six.iteritems(self._attr_cache):
+        for name, value in self._attr_cache.items():
             f = self._form.fields[name]
             value = f.prepare_value(value)
             # Widget.format_value in 1.11 has a different semantic than Widget._format_value in previous versions
             # in case the value is *exactly* True / False / None returns None
             # To handle this we pick the formatted value *only if* both formatted and original values evaluates to true
             # Choices fields must not be formatted because we need the python value, not the formatted one
             new_value = None
-            if not hasattr(f, 'choices'):
-                if hasattr(f.widget, 'format_value'):
+            if not hasattr(f, "choices"):
+                if hasattr(f.widget, "format_value"):
                     new_value = f.widget.format_value(value)
-                elif hasattr(f.widget, '_format_value'):
+                elif hasattr(f.widget, "_format_value"):
                     new_value = f.widget._format_value(value)
             if value and new_value:
                 value = new_value
             self._data[name] = value
         return self._data
 
     def get_form(self, data=None, files=None, fields=(), exclude=(), form_class=None, **kwargs):
```

### Comparing `django-appdata-0.3.2/app_data/fields.py` & `django-appdata-0.4.0/app_data/fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 import json
 
-import six
-
 from django import forms
 from django.db.models import TextField
-from django.utils.encoding import smart_text
+from django.utils.encoding import smart_str
 
-from .registry import app_registry
 from .containers import AppDataContainerFactory
+from .registry import app_registry
 
 
-class AppDataDescriptor(object):
+class AppDataDescriptor:
     """Ensure the user attribute is accessible via the profile"""
 
     def __init__(self, field):
         self.field = field
 
     def __get__(self, instance, instance_type=None):
         if instance is None:
             return self
 
         value = instance.__dict__[self.field.name]
 
-        if isinstance(value, six.string_types):
+        if isinstance(value, str):
             value = json.loads(value)
 
         if isinstance(value, dict) and not isinstance(value, AppDataContainerFactory):
             value = AppDataContainerFactory(instance, value, app_registry=self.field.app_registry)
             instance.__dict__[self.field.name] = value
 
         value._instance = instance
@@ -40,49 +38,50 @@
         if isinstance(value, dict) and not isinstance(value, AppDataContainerFactory):
             value = AppDataContainerFactory(instance, value, app_registry=self.field.app_registry)
         instance.__dict__[self.field.name] = value
 
 
 class AppDataField(TextField):
     def __init__(self, *args, **kwargs):
-        self.app_registry = kwargs.pop('app_registry', app_registry)
-        kwargs.setdefault('default', '{}')
-        kwargs.setdefault('editable', False)
-        super(AppDataField, self).__init__(*args, **kwargs)
+        self.app_registry = kwargs.pop("app_registry", app_registry)
+        kwargs.setdefault("default", "{}")
+        kwargs.setdefault("editable", False)
+        super().__init__(*args, **kwargs)
 
     def contribute_to_class(self, cls, name, **kwargs):
-        super(AppDataField, self).contribute_to_class(cls, name, **kwargs)
+        super().contribute_to_class(cls, name, **kwargs)
         setattr(cls, name, AppDataDescriptor(self))
 
     def get_db_prep_value(self, value, connection, prepared=False):
         """Convert JSON object to a string"""
         if isinstance(value, AppDataContainerFactory):
             value = value.serialize()
         if isinstance(value, dict):
             value = json.dumps(value)
         return value
 
     def validate(self, value, model_instance):
-        super(AppDataField, self).validate(value, model_instance)
+        super().validate(value, model_instance)
         value.validate(model_instance)
 
     def value_to_string(self, obj):
         value = self.value_from_object(obj)
 
         if isinstance(value, AppDataContainerFactory):
             value = value.serialize()
         if isinstance(value, dict):
             value = json.dumps(value)
 
-        return smart_text(value)
+        return smart_str(value)
 
 
 class ListModelMultipleChoiceField(forms.ModelMultipleChoiceField):
     """
     A ModelMultipleChoiceField that cleans to a list instead of a QuerySet
 
     Use this on AppDataForms rather than a ModelMultipleChoiceField to make it
     possible to manipulate the app data field like a list.
     """
+
     def clean(self, value):
-        value = super(ListModelMultipleChoiceField, self).clean(value)
+        value = super().clean(value)
         return list(value)
```

### Comparing `django-appdata-0.3.2/app_data/forms.py` & `django-appdata-0.4.0/app_data/forms.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-from operator import methodcaller
 from copy import deepcopy
-
-import six
+from operator import methodcaller
 
 from django.forms.forms import NON_FIELD_ERRORS, Form
 from django.forms.formsets import formset_factory
-from django.forms.models import modelform_factory, _get_foreign_key, BaseInlineFormSet, BaseModelFormSet
+from django.forms.models import BaseInlineFormSet, BaseModelFormSet, _get_foreign_key, modelform_factory
 from django.forms.utils import pretty_name
 from django.utils.safestring import mark_safe
 
 
 class AppDataForm(Form):
     def __init__(self, app_container, data=None, files=None, fields=(), exclude=(), *args, **kwargs):
         self.app_container = app_container
-        super(AppDataForm, self).__init__(data, files, *args, **kwargs)
+        super().__init__(data, files, *args, **kwargs)
 
         if fields or exclude:
             for f in list(self.fields.keys()):
                 if fields and f not in fields:
                     del self.fields[f]
                 elif f in exclude:
                     del self.fields[f]
@@ -26,62 +24,62 @@
     def instance(self):
         return self.app_container._instance
 
     def save(self):
         self.app_container.update(self.cleaned_data)
 
 
-class BaseFieldsDescriptor(object):
+class BaseFieldsDescriptor:
     """Combines the base_fields and prefixes them properly. Descriptor because needed on class level."""
-    def __get__(self, instance, owner):
 
-        if not hasattr(self, '_base_fields'):
+    def __get__(self, instance, owner):
+        if not hasattr(self, "_base_fields"):
             self._base_fields = bf = {}
 
             # construct an empty model to get to the data container and thus to the form classes
             app_container = getattr(owner.ModelForm._meta.model(), owner.app_data_field)
 
             # all the fields form model_form
             bf.update(owner.ModelForm.base_fields)
 
             # go through all the app forms...
-            for label, opts in six.iteritems(owner.get_app_form_opts()):
-                Form = app_container[label].form_class
-                exclude = set(opts.get('exclude', ()))
-                fields = opts.get('fields', None)
-                for name, field in six.iteritems(Form.base_fields):
+            for label, opts in owner.get_app_form_opts().items():
+                Form = app_container[label].form_class  # noqa: N806
+                exclude = set(opts.get("exclude", ()))
+                fields = opts.get("fields", None)
+                for name, field in Form.base_fields.items():
                     # skip proper fields
                     if fields is not None and name not in fields:
                         continue
                     if name in exclude:
                         continue
                     # prefix the fields
-                    bf['%s.%s' % (label, name)] = field
+                    bf["{}.{}".format(label, name)] = field
 
         return self._base_fields
 
 
-class AppFormOptsDescriptor(object):
+class AppFormOptsDescriptor:
     def __get__(self, instance, owner):
         # we cannot check hasattr because parent's app_form_opts would pick it up
-        if not '_app_form_opts' in owner.__dict__:
-            setattr(owner, '_app_form_opts', {})
+        if "_app_form_opts" not in owner.__dict__:
+            owner._app_form_opts = {}
         return owner._app_form_opts
 
 
 class MultiFormMetaclass(type):
     # This property is needed by BaseInlineFormSet which expect the form *class* to have a "real" _meta
     # and thus the proxing in the instance property won't work
     @property
     def _meta(cls):
         return cls.ModelForm._meta
 
 
-class MultiForm(six.with_metaclass(MultiFormMetaclass, object)):
-    app_data_field = 'app_data'
+class MultiForm(metaclass=MultiFormMetaclass):
+    app_data_field = "app_data"
     app_form_opts = AppFormOptsDescriptor()
 
     def __init__(self, *args, **kwargs):
         # construct the main model form
         self.model_form = self.ModelForm(*args, **kwargs)
         try:
             self.label_suffix = self.model_form.label_suffix
@@ -92,49 +90,50 @@
             files = self.model_form.files
         else:
             data, files = None, None
 
         # construct all the app forms
         self.app_forms = {}
         app_container = getattr(self.model_form.instance, self.app_data_field)
-        for label, label_opts in six.iteritems(self.get_app_form_opts()):
+        for label, label_opts in self.get_app_form_opts().items():
             prefix = label
             if self.model_form.prefix:
-                prefix = '%s-%s' % (self.model_form.prefix, prefix)
+                prefix = "{}-{}".format(self.model_form.prefix, prefix)
             self.app_forms[label] = app_container[label].get_form(data, files, prefix=prefix, **label_opts)
 
     @classmethod
     def get_app_form_opts(cls):
         """Utility method to combine app_form_opts from all base classes."""
         # subclass may wish to remove superclass's app_form
         skip_labels = set()
 
         form_opts = {}
         # go through class hierarchy and collect form definitions
         for c in cls.mro():
             # not a MultiForm, skip
-            if not hasattr(c, 'app_form_opts'):
+            if not hasattr(c, "app_form_opts"):
                 continue
-            for label, label_opts in six.iteritems(c.app_form_opts):
+            for label, label_opts in c.app_form_opts.items():
                 if label in form_opts or label in skip_labels:
                     # form already defined, or should be skipped
                     continue
 
                 elif label_opts is None:
                     # mark as to-be-skipped
                     skip_labels.add(label)
 
                 else:
                     # add form def
                     form_opts[label] = label_opts
         return form_opts
 
     @classmethod
-    def add_form(cls, label, form_options={}):
+    def add_form(cls, label, form_options=None):
         """Add an app_data form to the multi form after its creation."""
+        form_options = form_options or {}
         cls.app_form_opts[label] = form_options.copy()
 
     @classmethod
     def remove_form(cls, label):
         """
         Remove an app_data form to the multi form after its creation.
         Even if this form would be specified in a superclass it would be skipped.
@@ -186,119 +185,159 @@
         return self.model_form.is_bound
 
     # methods combining outputs from all forms
     base_fields = BaseFieldsDescriptor()
 
     def _get_all_forms(self):
         yield self.model_form
-        for f in six.itervalues(self.app_forms):
-            yield f
+        yield from self.app_forms.values()
 
     def __unicode__(self):
         return self.as_table()
 
     def as_ul(self):
-        return mark_safe(u'\n'.join(map(methodcaller('as_ul'), self._get_all_forms())))
+        return mark_safe("\n".join(map(methodcaller("as_ul"), self._get_all_forms())))
 
     def as_table(self):
-        return mark_safe(u'\n'.join(map(methodcaller('as_table'), self._get_all_forms())))
+        return mark_safe("\n".join(map(methodcaller("as_table"), self._get_all_forms())))
 
     def as_p(self):
-        return mark_safe(u'\n'.join(map(methodcaller('as_p'), self._get_all_forms())))
+        return mark_safe("\n".join(map(methodcaller("as_p"), self._get_all_forms())))
 
     def is_valid(self):
-        return all(map(methodcaller('is_valid'), self._get_all_forms()))
+        return all(map(methodcaller("is_valid"), self._get_all_forms()))
 
     def has_changed(self):
-        return any(map(methodcaller('has_changed'), self._get_all_forms()))
+        return any(map(methodcaller("has_changed"), self._get_all_forms()))
 
     def __getitem__(self, name):
         # provide access to app.field as well
         app = None
-        if '.' in name:
-            app, name = name.split('.', 1)
+        if "." in name:
+            app, name = name.split(".", 1)
 
         if app is None:
             form = self.model_form
         else:
             try:
                 form = self.app_forms[app]
             except KeyError:
-                raise KeyError('AppForm %r not found in MultiForm.' % name)
+                raise KeyError("AppForm %r not found in MultiForm." % name)
 
         try:
             field = form[name]
         except KeyError:
-            raise KeyError('Field %r not found in Form %s' % (name, form.fields))
+            raise KeyError("Field {!r} not found in Form {}".format(name, form.fields))
 
         return field
 
     @property
     def changed_data(self):
-        if not hasattr(self, '_changed_data'):
+        if not hasattr(self, "_changed_data"):
             self._changed_data = cd = self.model_form.changed_data[:]
-            for label, form in six.iteritems(self.app_forms):
-                cd.extend(map(lambda n: '%s.%s' % (label, n), form.changed_data))
+            for label, form in self.app_forms.items():
+                cd.extend(map(lambda n: "{}.{}".format(label, n), form.changed_data))  # noqa: B023, C417
         return self._changed_data
 
     @property
     def errors(self):
         # combine all the errors
-        if not hasattr(self, '_errors'):
+        if not hasattr(self, "_errors"):
             self._errors = self.model_form.errors.copy()
-            for label, form in six.iteritems(self.app_forms):
-                for k, v in six.iteritems(form.errors):
+            for label, form in self.app_forms.items():
+                for k, v in form.errors.items():
                     if k == NON_FIELD_ERRORS:
                         self._errors.setdefault(k, self.model_form.error_class()).extend(v)
                     else:
-                        self._errors['%s.%s' % (label, k)] = v
+                        self._errors["{}.{}".format(label, k)] = v
         return self._errors
 
     def non_field_errors(self):
         return self.errors.get(NON_FIELD_ERRORS, self.model_form.error_class())
 
     def save(self, **kwargs):
         # save the app_data forms first
         for f in self.app_forms.values():
             f.save()
         # save the model itself
         return self.model_form.save(**kwargs)
 
 
 class AppDataBaseInlineFormSet(BaseInlineFormSet):
-
     def add_fields(self, form, index):
         """appcontainer fields are no longer added to the empty form, we can inject them hooking here."""
-        super(AppDataBaseInlineFormSet, self).add_fields(form, index)
+        super().add_fields(form, index)
         for name, field in form.base_fields.items():
             if name not in form.fields:
                 form.fields[name] = deepcopy(field)
                 if not form.fields[name].label:
-                    form.fields[name].label = pretty_name(name.split('.')[1])
+                    form.fields[name].label = pretty_name(name.split(".")[1])
 
 
-def multiform_factory(model, multiform=MultiForm, app_data_field='app_data', name=None, form_opts={}, **kwargs):
+def multiform_factory(model, multiform=MultiForm, app_data_field="app_data", name=None, form_opts=None, **kwargs):
+    form_opts = form_opts or {}
     model_form = modelform_factory(model, **kwargs)
-    name = name or '%sWithAppDataForm' % model_form._meta.model.__name__
+    name = name or "%sWithAppDataForm" % model_form._meta.model.__name__
     return type(
-        name, (multiform, ),
-        {'ModelForm': model_form, 'app_data_field': app_data_field, '_app_form_opts': form_opts}
+        name,
+        (multiform,),
+        {
+            "ModelForm": model_form,
+            "app_data_field": app_data_field,
+            "_app_form_opts": form_opts,
+        },
     )
 
 
-def multiformset_factory(model, multiform=MultiForm, app_data_field='app_data', name=None, form_opts={},
-                         formset=BaseModelFormSet, extra=3, can_order=False, can_delete=True, max_num=None,
-                         **kwargs):
+def multiformset_factory(
+    model,
+    multiform=MultiForm,
+    app_data_field="app_data",
+    name=None,
+    form_opts=None,
+    formset=BaseModelFormSet,
+    extra=3,
+    can_order=False,
+    can_delete=True,
+    max_num=None,
+    **kwargs,
+):
+    form_opts = form_opts or {}
     multiform = multiform_factory(model, multiform, app_data_field, name, form_opts, **kwargs)
-    FormSet = formset_factory(multiform, formset=formset, extra=extra, can_order=can_order, can_delete=can_delete, max_num=max_num)
+    FormSet = formset_factory(  # noqa: N806
+        multiform,
+        formset=formset,
+        extra=extra,
+        can_order=can_order,
+        can_delete=can_delete,
+        max_num=max_num,
+    )
     FormSet.model = model
     return FormSet
 
 
-def multiinlineformset_factory(parent_model, model, multiform=MultiForm, app_data_field='app_data', name=None, form_opts={},
-                                formset=BaseInlineFormSet, fk_name=None, **kwargs):
+def multiinlineformset_factory(
+    parent_model,
+    model,
+    multiform=MultiForm,
+    app_data_field="app_data",
+    name=None,
+    form_opts=None,
+    formset=BaseInlineFormSet,
+    fk_name=None,
+    **kwargs,
+):
+    form_opts = form_opts or {}
     fk = _get_foreign_key(parent_model, model, fk_name=fk_name)
     if fk.unique:
-        kwargs['max_num'] = 1
-    FormSet = multiformset_factory(model, multiform, app_data_field, name, form_opts, formset=formset, **kwargs)
+        kwargs["max_num"] = 1
+    FormSet = multiformset_factory(  # noqa: N806
+        model,
+        multiform,
+        app_data_field,
+        name,
+        form_opts,
+        formset=formset,
+        **kwargs,
+    )  # noqa: N806
     FormSet.fk = fk
     return FormSet
```

### Comparing `django-appdata-0.3.2/app_data/registry.py` & `django-appdata-0.4.0/app_data/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-class NamespaceConflict(Exception):
+class NamespaceConflict(Exception):  # noqa: N818
     pass
 
 
 class NamespaceMissing(KeyError):
     pass
 
 
-class NamespaceRegistry(object):
+class NamespaceRegistry:
     """
     Global registry of app_specific storage classes in app_data field
     """
+
     def __init__(self, default_class=None):
         self.default_class = default_class
         self._reset()
 
     def _reset(self):
         # stuff registered by apps
         self._global_registry = {}
@@ -36,26 +37,21 @@
         # fallback to default
         return self.default_class
 
     def register(self, namespace, class_, model=None, override=False):
         registry = self._model_registry.setdefault(model, {}) if model is not None else self._global_registry
         if namespace in registry and not override:
             raise NamespaceConflict(
-                'Namespace %r already assigned to class %r%s.' % (
-                    namespace,
-                    registry[namespace],
-                    '' if model is None else ' for model %s' % model._meta
-                )
+                "Namespace %r already assigned to class %r%s."
+                % (namespace, registry[namespace], "" if model is None else " for model %s" % model._meta),
             )
         registry[namespace] = class_
 
     def unregister(self, namespace, model=None):
         registry = self._model_registry.setdefault(model, {}) if model is not None else self._global_registry
         if namespace not in registry:
-            raise NamespaceMissing(
-                'Namespace %r is not registered yet.' % namespace)
+            raise NamespaceMissing("Namespace %r is not registered yet." % namespace)
 
         del registry[namespace]
 
-app_registry = NamespaceRegistry()
-
 
+app_registry = NamespaceRegistry()
```

### Comparing `django-appdata-0.3.2/django_appdata.egg-info/PKG-INFO` & `django-appdata-0.4.0/django_appdata.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,206 +1,207 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-appdata
-Version: 0.3.2
+Version: 0.4.0
 Summary: Extendable field that enables Django apps to store their data on your models.
-Home-page: https://github.com/ella/django-appdata/
+Home-page: https://github.com/ella/django-appdata
 Author: Ella Development Team
 Author-email: dev@ellaproject.cz
 License: BSD
-Description: Django AppData
-        ##############
-        
-        Extandable field and related tools that enable Django apps to extend your
-        reusable app.
-        
-        Motivation
-        **********
-        
-        When working with reusable django apps we often found that we needed to add
-        something extra to the model or form the app provided. Some apps try to solve
-        this by providing a flexible model definition and a pluggable form (see
-        ``django.contrib.comments`` for an exmple of this approach) but even then it
-        leads to some duplication of efforts.
-        
-        ``django-appdata`` app tries, through ``AppDataField``, ``MultiForm`` and ``AppDataModelAdmin``,
-        to provide a standardised approach to extending existing apps.
-        
-        Supported versions
-        ******************
-        
-        Python: 2.7, 3.5, 3.6, 3.7, 3.8
-        Django: 1.11, 2.2, 3.0, 3.1
-        
-        Upgrading to 0.3
-        ****************
-        
-        If you are upgrading from a 0.2.x version, please note the following incompatible changes in 0.3
-        
-        * Dropped Django < 1.11 and Python 3.4 compatibility
-        
-        
-        Extending Models
-        ****************
-        
-        When you have an extendable django app using the ``AppDataField``::
-        
-            from django.db import models
-            from app_data import AppDataField
-        
-            class BlogPost(models.Model):
-                text = models.TextField()
-                app_data = AppDataField()
-        
-        your code can register a namespace on any (or all) ``AppDataField`` and store
-        it's own data there by registering a *container* (subclass of
-        ``AppDataContainer``). To define the data you use django's form framework::
-        
-            from django.forms.models import ModelMultipleChoiceField
-            from app_data import app_registry, AppDataForm, AppDataContainer
-        
-            from .models import Tag
-        
-            class TaggingAppDataForm(AppDataForm):
-                public_tags = ModelMultipleChoiceField(Tag.objects.all())
-                admin_tags = ModelMultipleChoiceField(Tag.objects.all())
-        
-            class TaggingAppDataContainer(AppDataContainer):
-                form_class = TaggingAppDataForm
-        
-                def tag_string(self):
-                    print ', '.join(t.name for t in self.public_tags)
-        
-            app_registry.register('tagging', TaggingAppDataContainer)
-        
-        This should give you access to ``'tagging'`` namespace in any defined ``AppDataField``::
-        
-            from blog_app.models import BlogPost
-        
-            bp = BlogPost()
-            assert bp.app_data.tagging.tag_string() == ""
-        
-        
-        Additional Options
-        ~~~~~~~~~~~~~~~~~~
-        
-        Note that if you don't need to add custom methods to your container you can
-        just use a factory to create the subclass::
-        
-            app_registry.register('tagging', AppDataContainer.from_form(TaggingAppDataForm))
-        
-        Additionaly you can restrict the registration to a given model::
-        
-            from blog_app.models import BlogPost
-        
-            app_registry.register('tagging', TaggingAppDataContainer, BlogPost)
-        
-        Extending Forms
-        ***************
-        
-        ``django-appdata`` supplies a ``MultiForm`` class - a wrapper around django's ``ModelForm``
-        with optional added sub-forms that corresponds to namespaces registered in the
-        model's ``AppDataField``, typically the extendable app would create and use a
-        ``MultiForm`` instead of a regular ``ModelForm``::
-        
-            from app_data.forms import multiform_factory
-            from .models import BlogPost
-        
-            BlogPostMultiForm = multiform_factory(BlogPost)
-        
-        And when using that app any project can add additional sub-forms to that ``MultiForm``::
-        
-            from blog_app.forms import BlogPostMultiForm
-        
-            BlogPostMultiForm.add_form('tagging', {'fields': ['public_tags']})
-        
-        This way when the reusable app's code can remain unchanged and we can inject
-        additional form logic to its processing.
-        
-        Additional Options
-        ~~~~~~~~~~~~~~~~~~
-        
-        Any arguments and keyword arguments are passed without change to the
-        ``ModelForm`` class the ``MultiForm`` is wrapping so even if you have custom args
-        for your ``ModelForm`` everything will still work::
-        
-            from django.forms.models import BaseModelForm
-        
-            class ModelFormWithUser(ModelForm):
-                def __init__(self, user, *args, **kwargs):
-                    self.user = user
-                    super(ModelFormWithUser, self).__init__(*args, **kwargs)
-        
-            BlogPostMultiForm = multiform_factory(BlogPost, form=ModelFormWithUser)
-        
-        And of course you are not limited to the use of a factory function::
-        
-            from app_data import MultiForm
-        
-            class MyMultiForm(MultiForm):
-                ModelForm = BlogPostModelForm
-        
-        MultiForms in Admin
-        *******************
-        
-        If you wish to add your own code to the admin interface, just use
-        ``AppDataModelAdmin``::
-        
-            from django.contrib import admin
-            from app_data.admin import AppDataModelAdmin
-            from blog_app.models import BlogPost
-        
-            class BlogPostAdmin(AppDataModelAdmin):
-                # due to the behavior of django admin validation we need to use
-                # get_fieldsets instead of just fieldsets
-                def get_fieldsets(self, request, obj=None):
-                     return [
-                         (None, {'fields': ['text', ]}),
-                         ('Tagging', {'fields': [('tagging.public_tags', 'tagging.admin_tags')]})
-                     ]
-            admin.site.register(BlogPost, BlogPostAdmin)
-        
-        Additional Options
-        ~~~~~~~~~~~~~~~~~~
-        
-        As with django's admin and forms you can supply your own ``MultiForm`` class by
-        using the ``multiform`` attribute of ``AppDataModelAdmin``.
-        
-        Behind the scenes
-        *****************
-        
-        ``django-appdata`` uses a ``TextField`` to store the data on the model using JSON
-        and django's forms framework for (de)serialization and validation of the data.
-        
-        When accessing the containers in the field we will try to locate the
-        appropriate container in the registry. If none is found, plain data will be
-        returned if present (dict). To assure everything working properly we recommend
-        putting some sort of init code in place for your project that will make sure all
-        the registration is done before any actual code is run. We are using a module
-        called ``register`` in our apps and then a `piece of code`_ similar to admin's
-        autodiscover to iterate through installed apps and load this module.
-        
-        .. _`piece of code`: https://github.com/ella/ella/blob/master/ella/utils/installedapps.py#L27
-        
-        Build status
-        ************
-        
-        :Master branch:
-        
-          .. image:: https://secure.travis-ci.org/ella/django-appdata.png?branch=master
-             :alt: Travis CI - Distributed build platform for the open source community
-             :target: http://travis-ci.org/#!/ella/django-appdata
-Platform: UNKNOWN
+Project-URL: Documentation, https://django-appdata.readthedocs.io/
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 1.11
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Django AppData
+##############
+
+Extendable field and related tools that enable Django apps to extend your
+reusable app.
+
+Motivation
+**********
+
+When working with reusable django apps we often found that we needed to add
+something extra to the model or form the app provided. Some apps try to solve
+this by providing a flexible model definition and a pluggable form (see
+``django.contrib.comments`` for an exmple of this approach) but even then it
+leads to some duplication of efforts.
+
+``django-appdata`` app tries, through ``AppDataField``, ``MultiForm`` and ``AppDataModelAdmin``,
+to provide a standardised approach to extending existing apps.
+
+Supported versions
+******************
+
+Python: 3.9, 3.10, 3.11
+Django: 3.2, 4.2
+
+Upgrading to 0.4
+****************
+
+If you are upgrading from a 0.3.x version, please note the following incompatible changes in 0.4
+
+* Dropped Django < 3.2 and Python < 3.9 compatibility
+
+
+Extending Models
+****************
+
+When you have an extendable django app using the ``AppDataField``::
+
+    from django.db import models
+    from app_data import AppDataField
+
+    class BlogPost(models.Model):
+        text = models.TextField()
+        app_data = AppDataField()
+
+your code can register a namespace on any (or all) ``AppDataField`` and store
+it's own data there by registering a *container* (subclass of
+``AppDataContainer``). To define the data you use django's form framework::
+
+    from django.forms.models import ModelMultipleChoiceField
+    from app_data import app_registry, AppDataForm, AppDataContainer
+
+    from .models import Tag
+
+    class TaggingAppDataForm(AppDataForm):
+        public_tags = ModelMultipleChoiceField(Tag.objects.all())
+        admin_tags = ModelMultipleChoiceField(Tag.objects.all())
+
+    class TaggingAppDataContainer(AppDataContainer):
+        form_class = TaggingAppDataForm
+
+        def tag_string(self):
+            print ', '.join(t.name for t in self.public_tags)
+
+    app_registry.register('tagging', TaggingAppDataContainer)
+
+This should give you access to ``'tagging'`` namespace in any defined ``AppDataField``::
+
+    from blog_app.models import BlogPost
+
+    bp = BlogPost()
+    assert bp.app_data.tagging.tag_string() == ""
+
+
+Additional Options
+~~~~~~~~~~~~~~~~~~
+
+Note that if you don't need to add custom methods to your container you can
+just use a factory to create the subclass::
+
+    app_registry.register('tagging', AppDataContainer.from_form(TaggingAppDataForm))
+
+Additionaly you can restrict the registration to a given model::
+
+    from blog_app.models import BlogPost
+
+    app_registry.register('tagging', TaggingAppDataContainer, BlogPost)
+
+Extending Forms
+***************
+
+``django-appdata`` supplies a ``MultiForm`` class - a wrapper around django's ``ModelForm``
+with optional added sub-forms that corresponds to namespaces registered in the
+model's ``AppDataField``, typically the extendable app would create and use a
+``MultiForm`` instead of a regular ``ModelForm``::
+
+    from app_data.forms import multiform_factory
+    from .models import BlogPost
+
+    BlogPostMultiForm = multiform_factory(BlogPost)
+
+And when using that app any project can add additional sub-forms to that ``MultiForm``::
+
+    from blog_app.forms import BlogPostMultiForm
+
+    BlogPostMultiForm.add_form('tagging', {'fields': ['public_tags']})
+
+This way when the reusable app's code can remain unchanged and we can inject
+additional form logic to its processing.
+
+Additional Options
+~~~~~~~~~~~~~~~~~~
+
+Any arguments and keyword arguments are passed without change to the
+``ModelForm`` class the ``MultiForm`` is wrapping so even if you have custom args
+for your ``ModelForm`` everything will still work::
+
+    from django.forms.models import BaseModelForm
+
+    class ModelFormWithUser(ModelForm):
+        def __init__(self, user, *args, **kwargs):
+            self.user = user
+            super(ModelFormWithUser, self).__init__(*args, **kwargs)
+
+    BlogPostMultiForm = multiform_factory(BlogPost, form=ModelFormWithUser)
+
+And of course you are not limited to the use of a factory function::
+
+    from app_data import MultiForm
+
+    class MyMultiForm(MultiForm):
+        ModelForm = BlogPostModelForm
+
+MultiForms in Admin
+*******************
+
+If you wish to add your own code to the admin interface, just use
+``AppDataModelAdmin``::
+
+    from django.contrib import admin
+    from app_data.admin import AppDataModelAdmin
+    from blog_app.models import BlogPost
+
+    class BlogPostAdmin(AppDataModelAdmin):
+        # due to the behavior of django admin validation we need to use
+        # get_fieldsets instead of just fieldsets
+        def get_fieldsets(self, request, obj=None):
+             return [
+                 (None, {'fields': ['text', ]}),
+                 ('Tagging', {'fields': [('tagging.public_tags', 'tagging.admin_tags')]})
+             ]
+    admin.site.register(BlogPost, BlogPostAdmin)
+
+Additional Options
+~~~~~~~~~~~~~~~~~~
+
+As with django's admin and forms you can supply your own ``MultiForm`` class by
+using the ``multiform`` attribute of ``AppDataModelAdmin``.
+
+Behind the scenes
+*****************
+
+``django-appdata`` uses a ``TextField`` to store the data on the model using JSON
+and django's forms framework for (de)serialization and validation of the data.
+
+When accessing the containers in the field we will try to locate the
+appropriate container in the registry. If none is found, plain data will be
+returned if present (dict). To assure everything working properly we recommend
+putting some sort of init code in place for your project that will make sure all
+the registration is done before any actual code is run. We are using a module
+called ``register`` in our apps and then a `piece of code`_ similar to admin's
+autodiscover to iterate through installed apps and load this module.
+
+.. _`piece of code`: https://github.com/ella/ella/blob/master/ella/utils/installedapps.py#L27
+
+Build status
+************
+
+:Master branch:
+
+  .. image:: https://secure.travis-ci.org/ella/django-appdata.png?branch=master
+     :alt: Travis CI - Distributed build platform for the open source community
+     :target: http://travis-ci.org/#!/ella/django-appdata
```

### Comparing `django-appdata-0.3.2/django_appdata.egg-info/SOURCES.txt` & `django-appdata-0.4.0/django_appdata.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.rst
-dev_requirements.txt
+pyproject.toml
+setup.cfg
 setup.py
 app_data/__init__.py
 app_data/admin.py
 app_data/containers.py
 app_data/fields.py
 app_data/forms.py
 app_data/registry.py
@@ -16,15 +17,15 @@
 django_appdata.egg-info/requires.txt
 django_appdata.egg-info/top_level.txt
 test_app_data/__init__.py
 test_app_data/admin.py
 test_app_data/cases.py
 test_app_data/manage.py
 test_app_data/models.py
-test_app_data/run_tests.py
+test_app_data/runtests.py
 test_app_data/settings.py
 test_app_data/test_admin.py
 test_app_data/test_fields.py
 test_app_data/test_forms.py
 test_app_data/urls.py
 test_app_data/migrations/0001_initial.py
 test_app_data/migrations/__init__.py
```

### Comparing `django-appdata-0.3.2/test_app_data/admin.py` & `django-appdata-0.4.0/test_app_data/admin.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,23 +3,21 @@
 from app_data.admin import AppDataModelAdmin, AppDataTabularInline
 
 from .models import Article, Author
 
 
 class AuthorInline(AppDataTabularInline):
     model = Author
-    declared_fieldsets = [
-        ('Personal', {'fields': [('personal.first_name', 'personal.last_name')]})
-    ]
+    declared_fieldsets = [("Personal", {"fields": [("personal.first_name", "personal.last_name")]})]
 
 
 class ArticleModelAdmin(AppDataModelAdmin):
-    fields = ['file']
+    fields = ["file"]
     declared_fieldsets = [
-        (None, {'fields': ['rss.title', 'file']}),
-        ('Meta', {'fields': ['rss.author']}),
-        ('Publish', {'fields': [('publish.publish_from', 'publish.published')]}),
+        (None, {"fields": ["rss.title", "file"]}),
+        ("Meta", {"fields": ["rss.author"]}),
+        ("Publish", {"fields": [("publish.publish_from", "publish.published")]}),
     ]
     inlines = [AuthorInline]
 
 
 site.register(Article, ArticleModelAdmin)
```

### Comparing `django-appdata-0.3.2/test_app_data/cases.py` & `django-appdata-0.4.0/test_app_data/cases.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-from django.test import TestCase
 from django.conf import settings
+from django.test import TestCase
 
 from app_data.registry import app_registry
 
 
 class AppDataTestCase(TestCase):
     def setUp(self):
-        super(AppDataTestCase, self).setUp()
+        super().setUp()
         self._old_global_registry = app_registry._global_registry.copy()
         self._old_model_registry = app_registry._model_registry.copy()
 
     def tearDown(self):
-        super(AppDataTestCase, self).tearDown()
-        if hasattr(settings, 'APP_DATA_CLASSES'):
+        super().tearDown()
+        if hasattr(settings, "APP_DATA_CLASSES"):
             del settings.APP_DATA_CLASSES
         app_registry.default_class = None
         app_registry._global_registry = self._old_global_registry
         app_registry._model_registry = self._old_model_registry
-
```

### Comparing `django-appdata-0.3.2/test_app_data/manage.py` & `django-appdata-0.4.0/test_app_data/manage.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 #!/usr/bin/env python
 
 import os
-from os.path import join, pardir, abspath, dirname, split
 import sys
+from os.path import abspath, dirname, join, pardir, split
 
 from django.core.management import execute_from_command_line
 
-
 # fix PYTHONPATH and DJANGO_SETTINGS for us
 # django settings module
-DJANGO_SETTINGS_MODULE = '%s.%s' % (split(abspath(dirname(__file__)))[1], 'settings')
+DJANGO_SETTINGS_MODULE = "{}.{}".format(split(abspath(dirname(__file__)))[1], "settings")
 # pythonpath dirs
 PYTHONPATH = [
-    abspath(join( dirname(__file__), pardir, pardir)),
-    abspath(join( dirname(__file__), pardir)),
+    abspath(join(dirname(__file__), pardir, pardir)),
+    abspath(join(dirname(__file__), pardir)),
 ]
 
 # inject few paths to pythonpath
 for p in PYTHONPATH:
     if p not in sys.path:
         sys.path.insert(0, p)
 
 # django needs this env variable
-os.environ['DJANGO_SETTINGS_MODULE'] = DJANGO_SETTINGS_MODULE
+os.environ["DJANGO_SETTINGS_MODULE"] = DJANGO_SETTINGS_MODULE
 
 
 if __name__ == "__main__":
     execute_from_command_line()
-
```

### Comparing `django-appdata-0.3.2/test_app_data/migrations/0001_initial.py` & `django-appdata-0.4.0/test_app_data/migrations/0001_initial.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,113 @@
 # Generated by Django 2.1 on 2018-12-24 01:39
 
-import app_data.fields
-from django.db import migrations, models
 import django.db.models.deletion
+from django.db import migrations, models
 
+import app_data.fields
 
-class Migration(migrations.Migration):
 
+class Migration(migrations.Migration):
     initial = True
 
-    dependencies = [
-    ]
+    dependencies = []
 
     operations = [
         migrations.CreateModel(
-            name='AlternateRegistryModel',
+            name="AlternateRegistryModel",
             fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('app_data', app_data.fields.AppDataField(default='{}', editable=False)),
+                (
+                    "id",
+                    models.AutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                (
+                    "app_data",
+                    app_data.fields.AppDataField(default="{}", editable=False),
+                ),
             ],
         ),
         migrations.CreateModel(
-            name='Author',
+            name="Author",
             fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('app_data', app_data.fields.AppDataField(default='{}', editable=False)),
+                (
+                    "id",
+                    models.AutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                (
+                    "app_data",
+                    app_data.fields.AppDataField(default="{}", editable=False),
+                ),
             ],
         ),
         migrations.CreateModel(
-            name='Category',
+            name="Category",
             fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('app_data', app_data.fields.AppDataField(default='{}', editable=False)),
+                (
+                    "id",
+                    models.AutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                (
+                    "app_data",
+                    app_data.fields.AppDataField(default="{}", editable=False),
+                ),
             ],
         ),
         migrations.CreateModel(
-            name='Publishable',
+            name="Publishable",
             fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('app_data', app_data.fields.AppDataField(default='{}', editable=False)),
+                (
+                    "id",
+                    models.AutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                (
+                    "app_data",
+                    app_data.fields.AppDataField(default="{}", editable=False),
+                ),
             ],
         ),
         migrations.CreateModel(
-            name='Article',
+            name="Article",
             fields=[
-                ('publishable_ptr', models.OneToOneField(auto_created=True, on_delete=django.db.models.deletion.CASCADE, parent_link=True, primary_key=True, serialize=False, to='test_app_data.Publishable')),
-                ('file', models.FileField(blank=True, upload_to='')),
+                (
+                    "publishable_ptr",
+                    models.OneToOneField(
+                        auto_created=True,
+                        on_delete=django.db.models.deletion.CASCADE,
+                        parent_link=True,
+                        primary_key=True,
+                        serialize=False,
+                        to="test_app_data.Publishable",
+                    ),
+                ),
+                ("file", models.FileField(blank=True, upload_to="")),
             ],
-            bases=('test_app_data.publishable',),
+            bases=("test_app_data.publishable",),
         ),
         migrations.AddField(
-            model_name='author',
-            name='publishable',
-            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='test_app_data.Publishable'),
+            model_name="author",
+            name="publishable",
+            field=models.ForeignKey(
+                on_delete=django.db.models.deletion.CASCADE,
+                to="test_app_data.Publishable",
+            ),
         ),
     ]
```

### Comparing `django-appdata-0.3.2/test_app_data/models.py` & `django-appdata-0.4.0/test_app_data/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django import forms
 from django.db import models
 
-from app_data import AppDataField, AppDataContainer, AppDataForm, NamespaceRegistry, app_registry
+from app_data import AppDataContainer, AppDataField, AppDataForm, NamespaceRegistry, app_registry
 
 
 class Category(models.Model):
     app_data = AppDataField()
 
 
 class Publishable(models.Model):
@@ -43,12 +43,11 @@
     last_name = forms.CharField(max_length=20, required=False)
 
 
 class AlternateRegistryAppForm(AppDataForm):
     alternate_field = forms.CharField(max_length=20, required=False)
 
 
-app_registry.register('publish', AppDataContainer.from_form(PublishAppForm))
-app_registry.register('rss', AppDataContainer.from_form(RSSAppForm))
-app_registry.register('personal', AppDataContainer.from_form(PersonalAppForm))
-AlternateRegistryModel.alternate_registry.register(
-    'alternate', AppDataContainer.from_form(AlternateRegistryAppForm))
+app_registry.register("publish", AppDataContainer.from_form(PublishAppForm))
+app_registry.register("rss", AppDataContainer.from_form(RSSAppForm))
+app_registry.register("personal", AppDataContainer.from_form(PersonalAppForm))
+AlternateRegistryModel.alternate_registry.register("alternate", AppDataContainer.from_form(AlternateRegistryAppForm))
```

### Comparing `django-appdata-0.3.2/test_app_data/settings.py` & `django-appdata-0.4.0/test_app_data/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,43 @@
 DEBUG = True
 
-ROOT_URLCONF = 'test_app_data.urls'
-STATIC_URL = '/static/'
-MEDIA_URL = '/media/'
+ROOT_URLCONF = "test_app_data.urls"
+STATIC_URL = "/static/"
+MEDIA_URL = "/media/"
 
-TEMPLATE_LOADERS = (
-    'django.template.loaders.app_directories.Loader',
-)
+TEMPLATE_LOADERS = ("django.template.loaders.app_directories.Loader",)
 
 TEMPLATE_OPTIONS = {
-    'context_processors': [
-        'django.contrib.auth.context_processors.auth',
-        'django.template.context_processors.request',
-        'django.contrib.messages.context_processors.messages',
+    "context_processors": [
+        "django.contrib.auth.context_processors.auth",
+        "django.template.context_processors.request",
+        "django.contrib.messages.context_processors.messages",
     ],
-    'loaders': TEMPLATE_LOADERS,
+    "loaders": TEMPLATE_LOADERS,
 }
 
 TEMPLATES = [
     {
-        'BACKEND': 'django.template.backends.django.DjangoTemplates',
-        'OPTIONS': TEMPLATE_OPTIONS
+        "BACKEND": "django.template.backends.django.DjangoTemplates",
+        "OPTIONS": TEMPLATE_OPTIONS,
     },
 ]
 
-SECRET_KEY = 'very-secret'
-
-DATABASES = {
-    'default': {
-        'ENGINE': 'django.db.backends.sqlite3',
-        'NAME': '/tmp/app_data.db',
-    }
-}
+SECRET_KEY = "very-secret"
 
-MIDDLEWARE_CLASSES = (
-    'django.middleware.common.CommonMiddleware',
-    'django.contrib.sessions.middleware.SessionMiddleware',
-    'django.contrib.auth.middleware.AuthenticationMiddleware',
-    'django.contrib.messages.middleware.MessageMiddleware',
-)
+DATABASES = {"default": {"ENGINE": "django.db.backends.sqlite3", "NAME": ":memory:"}}
 
 MIDDLEWARE = (
-    'django.middleware.common.CommonMiddleware',
-    'django.contrib.sessions.middleware.SessionMiddleware',
-    'django.contrib.auth.middleware.AuthenticationMiddleware',
-    'django.contrib.messages.middleware.MessageMiddleware',
+    "django.middleware.common.CommonMiddleware",
+    "django.contrib.sessions.middleware.SessionMiddleware",
+    "django.contrib.auth.middleware.AuthenticationMiddleware",
+    "django.contrib.messages.middleware.MessageMiddleware",
 )
 
 INSTALLED_APPS = (
-    'django.contrib.auth',
-    'django.contrib.contenttypes',
-    'django.contrib.sessions',
-    'django.contrib.admin',
-    'django.contrib.messages',
-    'test_app_data',
+    "django.contrib.auth",
+    "django.contrib.contenttypes",
+    "django.contrib.sessions",
+    "django.contrib.admin",
+    "django.contrib.messages",
+    "test_app_data",
 )
```

### Comparing `django-appdata-0.3.2/test_app_data/test_fields.py` & `django-appdata-0.4.0/test_app_data/test_fields.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,93 @@
+import pickle
 from datetime import date
 
 from django import forms
 
-from nose import tools
-
-from app_data.registry import NamespaceConflict, NamespaceMissing, app_registry
 from app_data.containers import AppDataContainer, AppDataForm
+from app_data.registry import NamespaceConflict, NamespaceMissing, app_registry
 
-from .models import Article, Publishable, AlternateRegistryModel
 from .cases import AppDataTestCase
-
-try:
-    import cPickle as pickle
-except ImportError:
-    import pickle
+from .models import AlternateRegistryModel, Article, Publishable
 
 
 class DummyAppDataContainer(AppDataContainer):
     pass
 
 
 class DummyAppDataContainer2(AppDataContainer):
     pass
 
 
 class TestForms(AppDataTestCase):
     def test_container_from_form(self):
         class MyForm(AppDataForm):
             publish_from = forms.DateField()
-        MyAppContainer = AppDataContainer.from_form(MyForm)
-        app_registry.register('myapp', MyAppContainer)
+
+        MyAppContainer = AppDataContainer.from_form(MyForm)  # noqa: N806
+        app_registry.register("myapp", MyAppContainer)
 
         art = Article()
-        tools.assert_true(isinstance(art.app_data['myapp'], MyAppContainer))
+        self.assertTrue(isinstance(art.app_data["myapp"], MyAppContainer))
 
     def test_initial_get_used_as_default(self):
         class MyForm(AppDataForm):
-            title = forms.CharField(max_length=25, initial='Hullo!')
-        MyAppContainer = AppDataContainer.from_form(MyForm)
-        app_registry.register('myapp', MyAppContainer)
+            title = forms.CharField(max_length=25, initial="Hullo!")
+
+        MyAppContainer = AppDataContainer.from_form(MyForm)  # noqa: N806
+        app_registry.register("myapp", MyAppContainer)
 
         art = Article()
-        tools.assert_true(isinstance(art.app_data['myapp'], MyAppContainer))
-        tools.assert_equals('Hullo!', art.app_data.myapp.get('title'))
+        self.assertTrue(isinstance(art.app_data["myapp"], MyAppContainer))
+        self.assertEqual("Hullo!", art.app_data.myapp.get("title"))
 
     def test_get_fallback_value(self):
         class MyForm(AppDataForm):
-            title = forms.CharField(max_length=25, initial='Hullo!')
-        MyAppContainer = AppDataContainer.from_form(MyForm)
-        app_registry.register('myapp', MyAppContainer)
+            title = forms.CharField(max_length=25, initial="Hullo!")
+
+        MyAppContainer = AppDataContainer.from_form(MyForm)  # noqa: N806
+        app_registry.register("myapp", MyAppContainer)
 
         art = Article()
-        tools.assert_equals(None, art.app_data.myapp.get('foo'))
-        tools.assert_equals('bar', art.app_data.myapp.get('foo', 'bar'))
+        self.assertEqual(None, art.app_data.myapp.get("foo"))
+        self.assertEqual("bar", art.app_data.myapp.get("foo", "bar"))
 
     def test_get_semantics_for_getitem(self):
         class MyForm(AppDataForm):
-            title = forms.CharField(max_length=25, initial='Hullo!')
+            title = forms.CharField(max_length=25, initial="Hullo!")
             description = forms.CharField(max_length=25, required=False)
-        MyAppContainer = AppDataContainer.from_form(MyForm)
-        app_registry.register('myapp', MyAppContainer)
+
+        MyAppContainer = AppDataContainer.from_form(MyForm)  # noqa: N806
+        app_registry.register("myapp", MyAppContainer)
 
         art = Article()
-        tools.assert_equals('Hullo!', art.app_data.myapp.title)
+        self.assertEqual("Hullo!", art.app_data.myapp.title)
         # empty initial value falls back to field's type
-        tools.assert_equals('', art.app_data.myapp.description)
+        self.assertEqual("", art.app_data.myapp.description)
 
 
 class TestSerialization(AppDataTestCase):
     class MyForm(AppDataForm):
         publish_from = forms.DateField()
 
     def setUp(self):
-        super(TestSerialization, self).setUp()
+        super().setUp()
 
-        MyAppContainer = AppDataContainer.from_form(self.MyForm)
-        app_registry.register('myapp', MyAppContainer)
+        MyAppContainer = AppDataContainer.from_form(self.MyForm)  # noqa: N806
+        app_registry.register("myapp", MyAppContainer)
         self.article = Article()
         self.article.app_data.myapp.publish_from = date(2012, 8, 26)
         self.article.save()
 
     def _test_article(self, art):
-        tools.assert_equals({'myapp': {'publish_from': '2012-08-26'}}, art.app_data)
-        tools.assert_equals({'publish_from': '2012-08-26'}, art.app_data.myapp._data)
+        self.assertEqual({"myapp": {"publish_from": "2012-08-26"}}, art.app_data)
+        self.assertEqual({"publish_from": "2012-08-26"}, art.app_data.myapp._data)
 
-        tools.assert_equals(date(2012, 8, 26), art.app_data.myapp['publish_from'])
-        tools.assert_equals(date(2012, 8, 26), art.app_data.myapp.publish_from)
+        self.assertEqual(date(2012, 8, 26), art.app_data.myapp["publish_from"])
+        self.assertEqual(date(2012, 8, 26), art.app_data.myapp.publish_from)
 
     def test_dates_are_serialized_on_write(self):
         art = Article.objects.get(pk=self.article.pk)
         self._test_article(art)
 
     def test_pickle_support(self):
         data = pickle.dumps(self.article)
@@ -101,76 +99,79 @@
         data = pickle.dumps(self.article)
         unpickled_article = pickle.loads(data)
         self._test_article(unpickled_article)
 
 
 class TestAppDataContainers(AppDataTestCase):
     def test_registered_classes_can_behave_as_attrs(self):
-        app_registry.register('dummy', DummyAppDataContainer)
+        app_registry.register("dummy", DummyAppDataContainer)
         art = Article()
-        tools.assert_true(isinstance(art.app_data.dummy, DummyAppDataContainer))
+        self.assertTrue(isinstance(art.app_data.dummy, DummyAppDataContainer))
 
     def test_registered_classes_can_be_set_as_attrs(self):
-        app_registry.register('dummy', DummyAppDataContainer)
+        app_registry.register("dummy", DummyAppDataContainer)
         art = Article()
-        art.app_data.dummy = {'answer': 42}
-        tools.assert_true(isinstance(art.app_data.dummy, DummyAppDataContainer))
-        tools.assert_equals(DummyAppDataContainer(art, {'answer': 42}), art.app_data.dummy)
-        tools.assert_equals({'dummy': {'answer': 42}}, art.app_data)
+        art.app_data.dummy = {"answer": 42}
+        self.assertTrue(isinstance(art.app_data.dummy, DummyAppDataContainer))
+        self.assertEqual(DummyAppDataContainer(art, {"answer": 42}), art.app_data.dummy)
+        self.assertEqual({"dummy": {"answer": 42}}, art.app_data)
 
     def test_registered_classes_get_stored_on_access(self):
-        app_registry.register('dummy', DummyAppDataContainer)
+        app_registry.register("dummy", DummyAppDataContainer)
         art = Article()
-        art.app_data['dummy']
-        tools.assert_equals({'dummy': {}}, art.app_data)
+        art.app_data["dummy"]
+        self.assertEqual({"dummy": {}}, art.app_data)
 
-    @tools.raises(NamespaceConflict)
     def test_namespace_can_only_be_registered_once(self):
-        app_registry.register('dummy', DummyAppDataContainer)
-        app_registry.register('dummy', DummyAppDataContainer2)
+        with self.assertRaises(NamespaceConflict):
+            app_registry.register("dummy", DummyAppDataContainer)
+            app_registry.register("dummy", DummyAppDataContainer2)
 
-    @tools.raises(NamespaceMissing)
     def test_unregistered_namespace_cannot_be_unregistered(self):
-        app_registry.register('dummy', DummyAppDataContainer)
-        app_registry.unregister('dummy')
-        app_registry.unregister('dummy')
+        with self.assertRaises(NamespaceMissing):
+            app_registry.register("dummy", DummyAppDataContainer)
+            app_registry.unregister("dummy")
+            app_registry.unregister("dummy")
 
     def test_override_class_for_model_only(self):
-        app_registry.register('dummy', DummyAppDataContainer)
-        app_registry.register('dummy', DummyAppDataContainer2, model=Publishable)
+        app_registry.register("dummy", DummyAppDataContainer)
+        app_registry.register("dummy", DummyAppDataContainer2, model=Publishable)
         inst = Publishable()
-        tools.assert_true(isinstance(inst.app_data.get('dummy', {}), DummyAppDataContainer2))
+        self.assertTrue(isinstance(inst.app_data.get("dummy", {}), DummyAppDataContainer2))
 
     def test_get_app_data_returns_registered_class_instance(self):
-        app_registry.register('dummy', DummyAppDataContainer)
+        app_registry.register("dummy", DummyAppDataContainer)
         inst = Publishable()
-        tools.assert_true(isinstance(inst.app_data.get('dummy', {}), DummyAppDataContainer))
+        self.assertTrue(isinstance(inst.app_data.get("dummy", {}), DummyAppDataContainer))
 
     def test_existing_values_get_wrapped_in_proper_class(self):
-        app_registry.register('dummy', DummyAppDataContainer)
+        app_registry.register("dummy", DummyAppDataContainer)
         inst = Publishable()
-        inst.app_data = {'dummy': {'hullo': 'there'}}
-        tools.assert_true(isinstance(inst.app_data['dummy'], DummyAppDataContainer))
+        inst.app_data = {"dummy": {"hullo": "there"}}
+        self.assertTrue(isinstance(inst.app_data["dummy"], DummyAppDataContainer))
 
     def test_get_app_data_returns_default_class_if_not_registered(self):
         app_registry.default_class = AppDataContainer
         inst = Publishable()
-        tools.assert_true(isinstance(inst.app_data.get('dummy', {}), AppDataContainer))
+        self.assertTrue(isinstance(inst.app_data.get("dummy", {}), AppDataContainer))
 
     def test_app_data_container_behaves_like_dict(self):
         inst = Publishable()
-        data = inst.app_data.get('dummy', {})
-        data['foo'] = 'bar'
-        tools.assert_equals(data['foo'], 'bar')
-        tools.assert_equals(list(data.keys()), ['foo'])
-        tools.assert_equals(list(data.values()), ['bar'])
+        data = inst.app_data.get("dummy", {})
+        data["foo"] = "bar"
+        self.assertEqual(data["foo"], "bar")
+        self.assertEqual(list(data.keys()), ["foo"])
+        self.assertEqual(list(data.values()), ["bar"])
 
     def test_alternate_registry(self):
         def _get_namespace(instance, namespace):
             return getattr(instance, namespace)
+
         alt = AlternateRegistryModel()
         # only the "alternate" namespace should be in this model's registry
-        tools.assert_equals(alt.app_data.alternate.alternate_field, '')
-        tools.assert_raises(AttributeError, _get_namespace, alt, 'publish')
+        self.assertEqual(alt.app_data.alternate.alternate_field, "")
+        with self.assertRaises(AttributeError):
+            _get_namespace(alt, "publish")
         # and the "alternate" namespace shouldn't be in the global registry
         inst = Publishable()
-        tools.assert_raises(AttributeError, _get_namespace, inst, 'alternate')
+        with self.assertRaises(AttributeError):
+            _get_namespace(inst, "alternate")
```

### Comparing `django-appdata-0.3.2/test_app_data/test_forms.py` & `django-appdata-0.4.0/test_app_data/test_forms.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,237 +1,240 @@
 from datetime import date
 
 from django import forms
 from django.forms.models import ModelChoiceField, modelform_factory
 
+from app_data.containers import AppDataContainer, AppDataForm
 from app_data.fields import ListModelMultipleChoiceField
-from app_data.forms import multiform_factory, MultiForm, multiformset_factory
+from app_data.forms import MultiForm, multiform_factory, multiformset_factory
 from app_data.registry import app_registry
-from app_data.containers import AppDataContainer, AppDataForm
-
-from nose import tools
 
 from .cases import AppDataTestCase
 from .models import Article, Category
 
 
 class TestMultiForm(AppDataTestCase):
     class MyMultiForm(MultiForm):
         pass
 
     class MyForm(AppDataForm):
         title = forms.CharField(max_length=100)
         publish_from = forms.DateField()
         publish_to = forms.DateField(required=False)
-        related_article = ModelChoiceField(queryset=Article.objects.all(), required=False)
+        related_article = ModelChoiceField(
+            queryset=Article.objects.all(),
+            required=False,
+        )
 
     class MyForm2(AppDataForm):
         foo = forms.CharField(max_length=100)
 
     def setUp(self):
-        super(TestMultiForm, self).setUp()
-        MyAppContainer = AppDataContainer.from_form(self.MyForm)
-        app_registry.register('myapp', MyAppContainer)
-        app_registry.register('myapp2', AppDataContainer.from_form(self.MyForm2))
+        super().setUp()
+        MyAppContainer = AppDataContainer.from_form(self.MyForm)  # noqa: N806
+        app_registry.register("myapp", MyAppContainer)
+        app_registry.register("myapp2", AppDataContainer.from_form(self.MyForm2))
 
     def test_multi_form_can_work_with_formsets(self):
-        FormSet = multiformset_factory(Article, form_opts={'myapp': {}}, exclude=())
+        FormSet = multiformset_factory(Article, form_opts={"myapp": {}}, exclude=())  # noqa: N806
         data = {
-            'fs-TOTAL_FORMS': '1',
-            'fs-INITIAL_FORMS': '0',
-
-            'fs-0-myapp-title': 'First',
-            'fs-0-myapp-publish_from': '2010-11-12',
+            "fs-TOTAL_FORMS": "1",
+            "fs-INITIAL_FORMS": "0",
+            "fs-0-myapp-title": "First",
+            "fs-0-myapp-publish_from": "2010-11-12",
         }
-        formset = FormSet(data, prefix='fs')
+        formset = FormSet(data, prefix="fs")
 
-        tools.assert_true(formset.is_valid())
+        self.assertTrue(formset.is_valid())
         formset.save()
-        tools.assert_equals(1, Article.objects.count())
+        self.assertEqual(1, Article.objects.count())
         art = Article.objects.all()[0]
-        tools.assert_equals(
+        self.assertEqual(
             {
-                'myapp': {
-                    'publish_from': '2010-11-12',
-                    'publish_to': None,
-                    'related_article': None,
-                    'title': u'First'
+                "myapp": {
+                    "publish_from": "2010-11-12",
+                    "publish_to": None,
+                    "related_article": None,
+                    "title": "First",
                 },
             },
-            art.app_data
+            art.app_data,
         )
 
     def test_multi_form_saves_all_the_forms(self):
-        MF = multiform_factory(Article, form_opts={'myapp': {}, 'myapp2': {}}, exclude=())
+        MF = multiform_factory(Article, form_opts={"myapp": {}, "myapp2": {}}, exclude=())  # noqa: N806
         data = {
-            'myapp-title': 'First',
-            'myapp-publish_from': '2010-11-12',
-            'myapp2-foo': 'Second',
+            "myapp-title": "First",
+            "myapp-publish_from": "2010-11-12",
+            "myapp2-foo": "Second",
         }
         form = MF(data)
-        tools.assert_true(form.is_valid())
-        tools.assert_equals({}, form.errors)
+        self.assertTrue(form.is_valid())
+        self.assertEqual({}, form.errors)
         art = form.save()
-        tools.assert_equals(
+        self.assertEqual(
             {
-                'myapp': {
-                    'publish_from': '2010-11-12',
-                    'publish_to': None,
-                    'related_article': None,
-                    'title': u'First'
+                "myapp": {
+                    "publish_from": "2010-11-12",
+                    "publish_to": None,
+                    "related_article": None,
+                    "title": "First",
                 },
-                'myapp2': {'foo': 'Second'}
+                "myapp2": {"foo": "Second"},
             },
-            art.app_data
+            art.app_data,
         )
 
     def test_form_can_be_added_to_parent(self):
-        MF = multiform_factory(Article, multiform=self.MyMultiForm, exclude=())
-        self.MyMultiForm.add_form('myapp', {})
+        MF = multiform_factory(Article, multiform=self.MyMultiForm, exclude=())  # noqa: N806
+        self.MyMultiForm.add_form("myapp", {})
         data = {
-            'myapp-title': 'First',
-            'myapp-publish_from': '2010-11-12',
+            "myapp-title": "First",
+            "myapp-publish_from": "2010-11-12",
         }
         form = MF(data)
-        tools.assert_true(form.is_valid())
-        tools.assert_equals({}, form.errors)
+        self.assertTrue(form.is_valid())
+        self.assertEqual({}, form.errors)
         art = form.save()
-        tools.assert_equals(
+        self.assertEqual(
             {
-                'myapp': {
-                    'publish_from': '2010-11-12',
-                    'publish_to': None,
-                    'related_article': None,
-                    'title': u'First'
-                }
+                "myapp": {
+                    "publish_from": "2010-11-12",
+                    "publish_to": None,
+                    "related_article": None,
+                    "title": "First",
+                },
             },
-            art.app_data
+            art.app_data,
         )
 
     def test_form_can_be_added(self):
-        MF = multiform_factory(Article, exclude=())
-        MF.add_form('myapp', {})
+        MF = multiform_factory(Article, exclude=())  # noqa: N806
+        MF.add_form("myapp", {})
         data = {
-            'myapp-title': 'First',
-            'myapp-publish_from': '2010-11-12',
+            "myapp-title": "First",
+            "myapp-publish_from": "2010-11-12",
         }
         form = MF(data)
-        tools.assert_true(form.is_valid())
-        tools.assert_equals({}, form.errors)
+        self.assertTrue(form.is_valid())
+        self.assertEqual({}, form.errors)
         art = form.save()
-        tools.assert_equals(
+        self.assertEqual(
             {
-                'myapp': {
-                    'publish_from': '2010-11-12',
-                    'publish_to': None,
-                    'related_article': None,
-                    'title': u'First'
-                }
+                "myapp": {
+                    "publish_from": "2010-11-12",
+                    "publish_to": None,
+                    "related_article": None,
+                    "title": "First",
+                },
             },
-            art.app_data
+            art.app_data,
         )
 
     def test_added_form_doesnt_appear_on_parent(self):
-        ArticleModelForm = modelform_factory(Article, exclude=())
+        ArticleModelForm = modelform_factory(Article, exclude=())  # noqa: N806
+
         class MF(MultiForm):
             ModelForm = ArticleModelForm
-        MF.add_form('myapp', {})
 
-        tools.assert_equals({}, MultiForm.app_form_opts)
+        MF.add_form("myapp", {})
+
+        self.assertEqual({}, MultiForm.app_form_opts)
 
     def test_form_can_be_removed(self):
-        MF = multiform_factory(Article, form_opts={'myapp': {}}, exclude=())
-        MF.remove_form('myapp')
+        MF = multiform_factory(Article, form_opts={"myapp": {}}, exclude=())  # noqa: N806
+        MF.remove_form("myapp")
         data = {
-            'myapp-title': 'First',
-            'myapp-publish_from': '2010-11-12',
+            "myapp-title": "First",
+            "myapp-publish_from": "2010-11-12",
         }
         form = MF(data)
-        tools.assert_true(form.is_valid())
-        tools.assert_equals({}, form.errors)
+        self.assertTrue(form.is_valid())
+        self.assertEqual({}, form.errors)
         art = form.save()
-        tools.assert_equals({}, art.app_data)
+        self.assertEqual({}, art.app_data)
 
 
 class TestAppDataForms(AppDataTestCase):
     class MyForm(AppDataForm):
         title = forms.CharField(max_length=100)
         publish_from = forms.DateField()
         publish_to = forms.DateField(required=False)
         related_article = ModelChoiceField(queryset=Article.objects.all(), required=False)
 
     class MyOtherForm(AppDataForm):
         categories = ListModelMultipleChoiceField(Category.objects.all(), required=False)
 
     def setUp(self):
-        super(TestAppDataForms, self).setUp()
-        MyAppContainer = AppDataContainer.from_form(self.MyForm)
-        app_registry.register('myapp', MyAppContainer)
-        self.data = {
-            'title': 'First!',
-            'publish_from': '2010-10-1'
-        }
-        MyOtherContainer = AppDataContainer.from_form(self.MyOtherForm)
-        app_registry.register('myotherapp', MyOtherContainer)
+        super().setUp()
+        MyAppContainer = AppDataContainer.from_form(self.MyForm)  # noqa: N806
+        app_registry.register("myapp", MyAppContainer)
+        self.data = {"title": "First!", "publish_from": "2010-10-1"}
+        MyOtherContainer = AppDataContainer.from_form(self.MyOtherForm)  # noqa: N806
+        app_registry.register("myotherapp", MyOtherContainer)
 
     def test_empty_list_model_multiple_choice_field(self):
         article = Article()
-        tools.assert_true(isinstance(article.app_data.myotherapp.categories, list))
-        tools.assert_equals([], article.app_data.myotherapp.categories)
+        self.assertTrue(isinstance(article.app_data.myotherapp.categories, list))
+        self.assertEqual([], article.app_data.myotherapp.categories)
 
     def test_list_model_multiple_choice_field(self):
         c1, c2 = Category.objects.create(), Category.objects.create()
 
         article = Article()
-        data = {'categories': [str(c1.pk), str(c2.pk)]}
+        data = {"categories": [str(c1.pk), str(c2.pk)]}
         form = article.app_data.myotherapp.get_form(data)
-        tools.assert_true(form.is_valid())
+        self.assertTrue(form.is_valid())
         form.save()
         article.save()
         article = Article.objects.get(pk=article.pk)
-        tools.assert_true(isinstance(article.app_data.myotherapp.categories, list))
-        tools.assert_equals([c1, c2], article.app_data.myotherapp.categories)
+        self.assertTrue(isinstance(article.app_data.myotherapp.categories, list))
+        self.assertEqual([c1, c2], article.app_data.myotherapp.categories)
 
     def test_instance_is_accessible_to_the_form(self):
         art = Article()
         form = art.app_data.myapp.get_form(self.data)
 
-        tools.assert_true(art is form.instance)
+        self.assertTrue(art is form.instance)
 
     def test_foreign_keys_can_be_used(self):
         rel = Article.objects.create()
-        self.data['related_article'] = str(rel.pk)
+        self.data["related_article"] = str(rel.pk)
 
         article = Article()
         form = article.app_data.myapp.get_form(self.data)
-        tools.assert_true(form.is_valid())
+        self.assertTrue(form.is_valid())
         form.save()
         article.save()
         article = Article.objects.get(pk=article.pk)
-        tools.assert_equals(rel, article.app_data.myapp.related_article)
+        self.assertEqual(rel, article.app_data.myapp.related_article)
 
     def test_current_app_data_will_be_used_as_initial(self):
         article = Article()
-        article.app_data = {'myapp': {'title': 'Hello', 'publish_from': '2012-10-10'}}
+        article.app_data = {"myapp": {"title": "Hello", "publish_from": "2012-10-10"}}
         form = article.app_data.myapp.get_form()
-        tools.assert_equals({'title': 'Hello', 'publish_from': '2012-10-10'}, form.initial)
+        self.assertEqual({"title": "Hello", "publish_from": "2012-10-10"}, form.initial)
 
     def test_form_save_alters_data_on_model(self):
         article = Article()
         form = article.app_data.myapp.get_form(self.data)
-        tools.assert_true(form.is_valid())
+        self.assertTrue(form.is_valid())
         form.save()
         article.save()
         article = Article.objects.get(pk=article.pk)
-        tools.assert_equals(date(2010, 10, 1), article.app_data.myapp.publish_from)
+        self.assertEqual(date(2010, 10, 1), article.app_data.myapp.publish_from)
 
     def test_form_with_limitted_fields_only_updates_those(self):
         article = Article()
-        form = article.app_data.myapp.get_form(self.data, fields=['title',])
-        tools.assert_true(form.is_valid())
+        form = article.app_data.myapp.get_form(
+            self.data,
+            fields=[
+                "title",
+            ],
+        )
+        self.assertTrue(form.is_valid())
         form.save()
 
         article.save()
         article = Article.objects.get(pk=article.pk)
-        tools.assert_equals('First!', article.app_data.myapp._data['title'])
-        tools.assert_false('publish_from' in article.app_data.myapp._data)
-
+        self.assertEqual("First!", article.app_data.myapp._data["title"])
+        self.assertFalse("publish_from" in article.app_data.myapp._data)
```

