# Comparing `tmp/django-anymail-9.1.tar.gz` & `tmp/django-anymail-9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-anymail-9.1.tar", last modified: Sat Mar 11 20:04:07 2023, max compression
+gzip compressed data, was "django-anymail-9.2.tar", last modified: Tue May  2 20:21:28 2023, max compression
```

## Comparing `django-anymail-9.1.tar` & `django-anymail-9.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-11 20:04:07.135206 django-anymail-9.1/
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-03-11 20:03:59.000000 django-anymail-9.1/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-03-11 20:03:59.000000 django-anymail-9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-03-11 20:03:59.000000 django-anymail-9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8818 2023-03-11 20:04:07.135206 django-anymail-9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6616 2023-03-11 20:03:59.000000 django-anymail-9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-11 20:04:07.123206 django-anymail-9.1/anymail/
--rw-r--r--   0 runner    (1001) docker     (122)      237 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      196 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-11 20:04:07.131206 django-anymail-9.1/anymail/backends/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18113 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/backends/amazon_ses.py
--rw-r--r--   0 runner    (1001) docker     (122)    21031 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/backends/amazon_sesv2.py
--rw-r--r--   0 runner    (1001) docker     (122)    25519 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7858 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/backends/base_requests.py
--rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/backends/console.py
--rw-r--r--   0 runner    (1001) docker     (122)    13602 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/backends/mailersend.py
--rw-r--r--   0 runner    (1001) docker     (122)    20399 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/backends/mailgun.py
--rw-r--r--   0 runner    (1001) docker     (122)    10263 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/backends/mailjet.py
--rw-r--r--   0 runner    (1001) docker     (122)    13738 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/backends/mandrill.py
--rw-r--r--   0 runner    (1001) docker     (122)     4194 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/backends/postal.py
--rw-r--r--   0 runner    (1001) docker     (122)    16132 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/backends/postmark.py
--rw-r--r--   0 runner    (1001) docker     (122)    17038 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/backends/sendgrid.py
--rw-r--r--   0 runner    (1001) docker     (122)     6165 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/backends/sendinblue.py
--rw-r--r--   0 runner    (1001) docker     (122)    10843 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/backends/sparkpost.py
--rw-r--r--   0 runner    (1001) docker     (122)     5663 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/backends/test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1743 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/checks.py
--rw-r--r--   0 runner    (1001) docker     (122)     7096 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    14301 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/inbound.py
--rw-r--r--   0 runner    (1001) docker     (122)     6261 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/message.py
--rw-r--r--   0 runner    (1001) docker     (122)     4247 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     3925 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)    21330 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-11 20:04:07.135206 django-anymail-9.1/anymail/webhooks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/webhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18362 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/webhooks/amazon_ses.py
--rw-r--r--   0 runner    (1001) docker     (122)     6460 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/webhooks/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7579 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/webhooks/mailersend.py
--rw-r--r--   0 runner    (1001) docker     (122)    21452 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/webhooks/mailgun.py
--rw-r--r--   0 runner    (1001) docker     (122)     8316 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/webhooks/mailjet.py
--rw-r--r--   0 runner    (1001) docker     (122)     7662 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/webhooks/mandrill.py
--rw-r--r--   0 runner    (1001) docker     (122)     6562 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/webhooks/postal.py
--rw-r--r--   0 runner    (1001) docker     (122)     9551 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/webhooks/postmark.py
--rw-r--r--   0 runner    (1001) docker     (122)    10459 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/webhooks/sendgrid.py
--rw-r--r--   0 runner    (1001) docker     (122)     3698 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/webhooks/sendinblue.py
--rw-r--r--   0 runner    (1001) docker     (122)     9135 2023-03-11 20:03:59.000000 django-anymail-9.1/anymail/webhooks/sparkpost.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-11 20:04:07.135206 django-anymail-9.1/django_anymail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8818 2023-03-11 20:04:07.000000 django-anymail-9.1/django_anymail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1302 2023-03-11 20:04:07.000000 django-anymail-9.1/django_anymail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-11 20:04:07.000000 django-anymail-9.1/django_anymail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-11 20:04:07.000000 django-anymail-9.1/django_anymail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-03-11 20:04:07.000000 django-anymail-9.1/django_anymail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-03-11 20:04:07.000000 django-anymail-9.1/django_anymail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      459 2023-03-11 20:03:59.000000 django-anymail-9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-03-11 20:04:07.135206 django-anymail-9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4653 2023-03-11 20:03:59.000000 django-anymail-9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:21:28.326285 django-anymail-9.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-05-02 20:21:18.000000 django-anymail-9.2/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-05-02 20:21:18.000000 django-anymail-9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-05-02 20:21:18.000000 django-anymail-9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8857 2023-05-02 20:21:28.326285 django-anymail-9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6616 2023-05-02 20:21:18.000000 django-anymail-9.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:21:28.318285 django-anymail-9.2/anymail/
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      196 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:21:28.322285 django-anymail-9.2/anymail/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18718 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/backends/amazon_ses.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21636 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/backends/amazon_sesv2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25519 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7962 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/backends/base_requests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/backends/console.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13602 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/backends/mailersend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20399 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/backends/mailgun.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10263 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/backends/mailjet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13738 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/backends/mandrill.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4194 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/backends/postal.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16132 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/backends/postmark.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17038 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/backends/sendgrid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6165 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/backends/sendinblue.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10843 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/backends/sparkpost.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5663 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/backends/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1743 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/checks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7096 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14399 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/inbound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6261 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/message.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4247 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3925 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21330 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:21:28.326285 django-anymail-9.2/anymail/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/webhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18362 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/webhooks/amazon_ses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6460 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/webhooks/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7579 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/webhooks/mailersend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21452 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/webhooks/mailgun.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8316 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/webhooks/mailjet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7662 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/webhooks/mandrill.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6562 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/webhooks/postal.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10371 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/webhooks/postmark.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10459 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/webhooks/sendgrid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3698 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/webhooks/sendinblue.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9135 2023-05-02 20:21:18.000000 django-anymail-9.2/anymail/webhooks/sparkpost.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 20:21:28.326285 django-anymail-9.2/django_anymail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8857 2023-05-02 20:21:28.000000 django-anymail-9.2/django_anymail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1302 2023-05-02 20:21:28.000000 django-anymail-9.2/django_anymail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 20:21:28.000000 django-anymail-9.2/django_anymail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 20:21:28.000000 django-anymail-9.2/django_anymail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-02 20:21:28.000000 django-anymail-9.2/django_anymail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-02 20:21:28.000000 django-anymail-9.2/django_anymail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-05-02 20:21:18.000000 django-anymail-9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-05-02 20:21:28.326285 django-anymail-9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4710 2023-05-02 20:21:18.000000 django-anymail-9.2/setup.py
```

### Comparing `django-anymail-9.1/LICENSE` & `django-anymail-9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/PKG-INFO` & `django-anymail-9.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: django-anymail
-Version: 9.1
+Version: 9.2
 Summary: Django email backends and webhooks for Amazon SES, MailerSend, Mailgun, Mailjet, Mandrill, Postal, Postmark, SendGrid, SendinBlue, and SparkPost
 Home-page: https://github.com/anymail/django-anymail
 Author: Mike Edmunds and Anymail contributors
 Author-email: medmunds@gmail.com
 License: BSD License
-Project-URL: Documentation, https://anymail.dev/en/v9.1/
+Project-URL: Documentation, https://anymail.dev/en/v9.2/
 Project-URL: Source, https://github.com/anymail/django-anymail
-Project-URL: Changelog, https://anymail.dev/en/v9.1/changelog/
+Project-URL: Changelog, https://anymail.dev/en/v9.2/changelog/
 Project-URL: Tracker, https://github.com/anymail/django-anymail/issues
 Keywords: Django,email,email backend,ESP,transactional mail,Amazon SES,MailerSend,Mailgun,Mailjet,Mandrill,Postal,Postmark,SendGrid,SendinBlue,SparkPost
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3
@@ -28,14 +28,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Environment :: Web Environment
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: amazon_ses
 Provides-Extra: mailersend
 Provides-Extra: mailgun
 Provides-Extra: mailjet
@@ -88,15 +89,15 @@
 * **SendGrid**
 * **SendinBlue**
 * **SparkPost**
 
 Anymail includes:
 
 * Integration of each ESP's sending APIs into
-  `Django's built-in email <https://docs.djangoproject.com/en/v9.1/topics/email/>`_
+  `Django's built-in email <https://docs.djangoproject.com/en/v9.2/topics/email/>`_
   package, including support for HTML, attachments, extra headers,
   and other standard email features
 * Extensions to expose common ESP-added functionality, like tags, metadata,
   and tracking, with code that's portable between ESPs
 * Simplified inline images for HTML email
 * Normalized sent-message status and tracking notification, by connecting
   your ESP's webhooks to Django signals
@@ -104,40 +105,40 @@
 * Inbound message support, to receive email through your ESP's webhooks,
   with simplified, portable access to attachments and other inbound content
 
 Anymail maintains compatibility with all Django versions that are in mainstream
 or extended support, plus (usually) a few older Django versions, and is extensively
 tested on all Python versions supported by Django. (Even-older Django versions
 may still be covered by an Anymail extended support release; consult the
-`changelog <https://anymail.dev/en/v9.1/changelog/>`_ for details.)
+`changelog <https://anymail.dev/en/v9.2/changelog/>`_ for details.)
 
 Anymail releases follow `semantic versioning <https://semver.org/>`_.
 The package is released under the BSD license.
 
 .. END shared-intro
 
-.. image:: https://github.com/anymail/django-anymail/workflows/test/badge.svg?branch=v9.1
-       :target: https://github.com/anymail/django-anymail/actions?query=workflow:test+branch:v9.1
+.. image:: https://github.com/anymail/django-anymail/workflows/test/badge.svg?branch=v9.2
+       :target: https://github.com/anymail/django-anymail/actions?query=workflow:test+branch:v9.2
        :alt:    test status in GitHub Actions
 
-.. image:: https://github.com/anymail/django-anymail/workflows/integration-test/badge.svg?branch=v9.1
-       :target: https://github.com/anymail/django-anymail/actions?query=workflow:integration-test+branch:v9.1
+.. image:: https://github.com/anymail/django-anymail/workflows/integration-test/badge.svg?branch=v9.2
+       :target: https://github.com/anymail/django-anymail/actions?query=workflow:integration-test+branch:v9.2
        :alt:    integration test status in GitHub Actions
 
-.. image:: https://readthedocs.org/projects/anymail/badge/?version=v9.1
-       :target: https://anymail.dev/en/v9.1/
+.. image:: https://readthedocs.org/projects/anymail/badge/?version=v9.2
+       :target: https://anymail.dev/en/v9.2/
        :alt:    documentation build status on ReadTheDocs
 
 **Resources**
 
-* Full documentation: https://anymail.dev/en/v9.1/
-* Help and troubleshooting: https://anymail.dev/en/v9.1/help/
+* Full documentation: https://anymail.dev/en/v9.2/
+* Help and troubleshooting: https://anymail.dev/en/v9.2/help/
 * Package on PyPI: https://pypi.org/project/django-anymail/
 * Project on Github: https://github.com/anymail/django-anymail
-* Changelog: https://anymail.dev/en/v9.1/changelog/
+* Changelog: https://anymail.dev/en/v9.2/changelog/
 
 
 Anymail 1-2-3
 -------------
 
 .. _quickstart:
 
@@ -173,15 +174,15 @@
             "MAILGUN_SENDER_DOMAIN": 'mg.example.com',  # your Mailgun domain, if needed
         }
         EMAIL_BACKEND = "anymail.backends.mailgun.EmailBackend"  # or sendgrid.EmailBackend, or...
         DEFAULT_FROM_EMAIL = "you@example.com"  # if you don't already have this in settings
         SERVER_EMAIL = "your-server@example.com"  # ditto (default from-email for Django errors)
 
 
-3. Now the regular `Django email functions <https://docs.djangoproject.com/en/v9.1/topics/email/>`_
+3. Now the regular `Django email functions <https://docs.djangoproject.com/en/v9.2/topics/email/>`_
    will send through your chosen ESP:
 
    .. code-block:: python
 
         from django.core.mail import send_mail
 
         send_mail("It works!", "This will get sent through Mailgun",
@@ -217,10 +218,10 @@
 
         # Send it:
         msg.send()
 
 .. END quickstart
 
 
-See the `full documentation <https://anymail.dev/en/v9.1/>`_
+See the `full documentation <https://anymail.dev/en/v9.2/>`_
 for more features and options, including receiving messages and tracking
 sent message status.
```

### Comparing `django-anymail-9.1/README.rst` & `django-anymail-9.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/backends/amazon_ses.py` & `django-anymail-9.2/anymail/backends/amazon_ses.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,26 +55,42 @@
     def open(self):
         if self.client:
             return False  # already exists
         try:
             self.client = boto3.session.Session(**self.session_params).client(
                 "ses", **self.client_params
             )
-        except BOTO_BASE_ERRORS:
+        except Exception:
             if not self.fail_silently:
                 raise
         else:
             return True  # created client
 
     def close(self):
         if self.client is None:
             return
         # self.client.close()  # boto3 doesn't support (or require) client shutdown
         self.client = None
 
+    def _send(self, message):
+        if self.client:
+            return super()._send(message)
+        elif self.fail_silently:
+            # (Probably missing boto3 credentials in open().)
+            return False
+        else:
+            class_name = self.__class__.__name__
+            raise RuntimeError(
+                "boto3 Session has not been opened in {class_name}._send. "
+                "(This is either an implementation error in {class_name}, "
+                "or you are incorrectly calling _send directly.)".format(
+                    class_name=class_name
+                )
+            )
+
     def build_message_payload(self, message, defaults):
         # The SES SendRawEmail and SendBulkTemplatedEmail calls have
         # very different signatures, so use a custom payload for each
         if getattr(message, "template_id", UNSET) is not UNSET:
             return AmazonSESSendBulkTemplatedEmailPayload(message, defaults, self)
         else:
             return AmazonSESSendRawEmailPayload(message, defaults, self)
```

### Comparing `django-anymail-9.1/anymail/backends/amazon_sesv2.py` & `django-anymail-9.2/anymail/backends/amazon_sesv2.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,26 +59,42 @@
     def open(self):
         if self.client:
             return False  # already exists
         try:
             self.client = boto3.session.Session(**self.session_params).client(
                 "sesv2", **self.client_params
             )
-        except BOTO_BASE_ERRORS:
+        except Exception:
             if not self.fail_silently:
                 raise
         else:
             return True  # created client
 
     def close(self):
         if self.client is None:
             return
         self.client.close()
         self.client = None
 
+    def _send(self, message):
+        if self.client:
+            return super()._send(message)
+        elif self.fail_silently:
+            # (Probably missing boto3 credentials in open().)
+            return False
+        else:
+            class_name = self.__class__.__name__
+            raise RuntimeError(
+                "boto3 Session has not been opened in {class_name}._send. "
+                "(This is either an implementation error in {class_name}, "
+                "or you are incorrectly calling _send directly.)".format(
+                    class_name=class_name
+                )
+            )
+
     def build_message_payload(self, message, defaults):
         if getattr(message, "template_id", UNSET) is not UNSET:
             # For simplicity, use SESv2 SendBulkEmail for all templated messages
             # (even though SESv2 SendEmail has a template option).
             return AmazonSESV2SendBulkEmailPayload(message, defaults, self)
         else:
             return AmazonSESV2SendEmailPayload(message, defaults, self)
```

### Comparing `django-anymail-9.1/anymail/backends/base.py` & `django-anymail-9.2/anymail/backends/base.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/backends/base_requests.py` & `django-anymail-9.2/anymail/backends/base_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,24 +43,28 @@
         except requests.RequestException:
             if not self.fail_silently:
                 raise
         finally:
             self.session = None
 
     def _send(self, message):
-        if self.session is None:
+        if self.session:
+            return super()._send(message)
+        elif self.fail_silently:
+            # create_session failed
+            return False
+        else:
             class_name = self.__class__.__name__
             raise RuntimeError(
                 "Session has not been opened in {class_name}._send. "
                 "(This is either an implementation error in {class_name}, "
                 "or you are incorrectly calling _send directly.)".format(
                     class_name=class_name
                 )
             )
-        return super()._send(message)
 
     def create_session(self):
         """Create the requests.Session object used by this instance of the backend.
         If subclassed, you can modify the Session returned from super() to give
         it your own configuration.
 
         This must return an instance of requests.Session."""
```

### Comparing `django-anymail-9.1/anymail/backends/console.py` & `django-anymail-9.2/anymail/backends/console.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/backends/mailersend.py` & `django-anymail-9.2/anymail/backends/mailersend.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/backends/mailgun.py` & `django-anymail-9.2/anymail/backends/mailgun.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/backends/mailjet.py` & `django-anymail-9.2/anymail/backends/mailjet.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/backends/mandrill.py` & `django-anymail-9.2/anymail/backends/mandrill.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/backends/postal.py` & `django-anymail-9.2/anymail/backends/postal.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/backends/postmark.py` & `django-anymail-9.2/anymail/backends/postmark.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/backends/sendgrid.py` & `django-anymail-9.2/anymail/backends/sendgrid.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/backends/sendinblue.py` & `django-anymail-9.2/anymail/backends/sendinblue.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/backends/sparkpost.py` & `django-anymail-9.2/anymail/backends/sparkpost.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/backends/test.py` & `django-anymail-9.2/anymail/backends/test.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/checks.py` & `django-anymail-9.2/anymail/checks.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/exceptions.py` & `django-anymail-9.2/anymail/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/inbound.py` & `django-anymail-9.2/anymail/inbound.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,18 @@
     def get_address_header(self, header):
         """
         Return the value of header parsed into a (possibly-empty)
         list of EmailAddress objects
         """
         values = self.get_all(header)
         if values is not None:
-            values = parse_address_list(values)
+            if "".join(values).strip() == "":
+                values = None
+            else:
+                values = parse_address_list(values)
         return values or []
 
     def get_date_header(self, header):
         """Return the value of header parsed into a datetime.date, or None"""
         value = self[header]
         if value is not None:
             value = parse_rfc2822date(value)
```

### Comparing `django-anymail-9.1/anymail/message.py` & `django-anymail-9.2/anymail/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from email.mime.image import MIMEImage
-from email.utils import unquote
+from email.utils import make_msgid, unquote
 from pathlib import Path
 
-from django.core.mail import EmailMessage, EmailMultiAlternatives, make_msgid
+from django.core.mail import EmailMessage, EmailMultiAlternatives
 
 from .utils import UNSET
 
 
 class AnymailMessageMixin(EmailMessage):
     """Mixin for EmailMessage that exposes Anymail features.
```

### Comparing `django-anymail-9.1/anymail/signals.py` & `django-anymail-9.2/anymail/signals.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/urls.py` & `django-anymail-9.2/anymail/urls.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/utils.py` & `django-anymail-9.2/anymail/utils.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/webhooks/amazon_ses.py` & `django-anymail-9.2/anymail/webhooks/amazon_ses.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/webhooks/base.py` & `django-anymail-9.2/anymail/webhooks/base.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/webhooks/mailersend.py` & `django-anymail-9.2/anymail/webhooks/mailersend.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/webhooks/mailgun.py` & `django-anymail-9.2/anymail/webhooks/mailgun.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/webhooks/mailjet.py` & `django-anymail-9.2/anymail/webhooks/mailjet.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/webhooks/mandrill.py` & `django-anymail-9.2/anymail/webhooks/mandrill.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/webhooks/postal.py` & `django-anymail-9.2/anymail/webhooks/postal.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/webhooks/postmark.py` & `django-anymail-9.2/anymail/webhooks/postmark.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
+import warnings
 
 from django.utils.dateparse import parse_datetime
 
-from ..exceptions import AnymailConfigurationError
+from ..exceptions import AnymailConfigurationError, AnymailWarning
 from ..inbound import AnymailInboundMessage
 from ..signals import (
     AnymailInboundEvent,
     AnymailTrackingEvent,
     EventType,
     RejectReason,
     inbound,
@@ -165,22 +166,40 @@
                 "You seem to have set Postmark's *%s* webhook "
                 "to Anymail's Postmark *inbound* webhook URL." % esp_event["RecordType"]
             )
 
         attachments = [
             AnymailInboundMessage.construct_attachment(
                 content_type=attachment["ContentType"],
-                content=attachment["Content"],
+                content=(
+                    attachment.get("Content")
+                    # WORKAROUND:
+                    # The test webhooks are not like their real webhooks
+                    # This allows the test webhooks to be parsed.
+                    or attachment["Data"]
+                ),
                 base64=True,
                 filename=attachment.get("Name", "") or None,
                 content_id=attachment.get("ContentID", "") or None,
             )
             for attachment in esp_event.get("Attachments", [])
         ]
 
+        # Warning to the user regarding the workaround of above.
+        for attachment in esp_event.get("Attachments", []):
+            if "Data" in attachment:
+                warnings.warn(
+                    "Received a test webhook attachment. "
+                    "It is recommended to test with real inbound events. "
+                    "See https://github.com/anymail/django-anymail/issues/304 "
+                    "for more information.",
+                    AnymailWarning,
+                )
+                break
+
         message = AnymailInboundMessage.construct(
             from_email=self._address(esp_event.get("FromFull")),
             to=", ".join([self._address(to) for to in esp_event.get("ToFull", [])]),
             cc=", ".join([self._address(cc) for cc in esp_event.get("CcFull", [])]),
             # bcc? Postmark specs this for inbound events,
             # but it's unclear how it could occur
             subject=esp_event.get("Subject", ""),
```

### Comparing `django-anymail-9.1/anymail/webhooks/sendgrid.py` & `django-anymail-9.2/anymail/webhooks/sendgrid.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/webhooks/sendinblue.py` & `django-anymail-9.2/anymail/webhooks/sendinblue.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/anymail/webhooks/sparkpost.py` & `django-anymail-9.2/anymail/webhooks/sparkpost.py`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/django_anymail.egg-info/PKG-INFO` & `django-anymail-9.2/django_anymail.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: django-anymail
-Version: 9.1
+Version: 9.2
 Summary: Django email backends and webhooks for Amazon SES, MailerSend, Mailgun, Mailjet, Mandrill, Postal, Postmark, SendGrid, SendinBlue, and SparkPost
 Home-page: https://github.com/anymail/django-anymail
 Author: Mike Edmunds and Anymail contributors
 Author-email: medmunds@gmail.com
 License: BSD License
-Project-URL: Documentation, https://anymail.dev/en/v9.1/
+Project-URL: Documentation, https://anymail.dev/en/v9.2/
 Project-URL: Source, https://github.com/anymail/django-anymail
-Project-URL: Changelog, https://anymail.dev/en/v9.1/changelog/
+Project-URL: Changelog, https://anymail.dev/en/v9.2/changelog/
 Project-URL: Tracker, https://github.com/anymail/django-anymail/issues
 Keywords: Django,email,email backend,ESP,transactional mail,Amazon SES,MailerSend,Mailgun,Mailjet,Mandrill,Postal,Postmark,SendGrid,SendinBlue,SparkPost
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3
@@ -28,14 +28,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Environment :: Web Environment
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: amazon_ses
 Provides-Extra: mailersend
 Provides-Extra: mailgun
 Provides-Extra: mailjet
@@ -88,15 +89,15 @@
 * **SendGrid**
 * **SendinBlue**
 * **SparkPost**
 
 Anymail includes:
 
 * Integration of each ESP's sending APIs into
-  `Django's built-in email <https://docs.djangoproject.com/en/v9.1/topics/email/>`_
+  `Django's built-in email <https://docs.djangoproject.com/en/v9.2/topics/email/>`_
   package, including support for HTML, attachments, extra headers,
   and other standard email features
 * Extensions to expose common ESP-added functionality, like tags, metadata,
   and tracking, with code that's portable between ESPs
 * Simplified inline images for HTML email
 * Normalized sent-message status and tracking notification, by connecting
   your ESP's webhooks to Django signals
@@ -104,40 +105,40 @@
 * Inbound message support, to receive email through your ESP's webhooks,
   with simplified, portable access to attachments and other inbound content
 
 Anymail maintains compatibility with all Django versions that are in mainstream
 or extended support, plus (usually) a few older Django versions, and is extensively
 tested on all Python versions supported by Django. (Even-older Django versions
 may still be covered by an Anymail extended support release; consult the
-`changelog <https://anymail.dev/en/v9.1/changelog/>`_ for details.)
+`changelog <https://anymail.dev/en/v9.2/changelog/>`_ for details.)
 
 Anymail releases follow `semantic versioning <https://semver.org/>`_.
 The package is released under the BSD license.
 
 .. END shared-intro
 
-.. image:: https://github.com/anymail/django-anymail/workflows/test/badge.svg?branch=v9.1
-       :target: https://github.com/anymail/django-anymail/actions?query=workflow:test+branch:v9.1
+.. image:: https://github.com/anymail/django-anymail/workflows/test/badge.svg?branch=v9.2
+       :target: https://github.com/anymail/django-anymail/actions?query=workflow:test+branch:v9.2
        :alt:    test status in GitHub Actions
 
-.. image:: https://github.com/anymail/django-anymail/workflows/integration-test/badge.svg?branch=v9.1
-       :target: https://github.com/anymail/django-anymail/actions?query=workflow:integration-test+branch:v9.1
+.. image:: https://github.com/anymail/django-anymail/workflows/integration-test/badge.svg?branch=v9.2
+       :target: https://github.com/anymail/django-anymail/actions?query=workflow:integration-test+branch:v9.2
        :alt:    integration test status in GitHub Actions
 
-.. image:: https://readthedocs.org/projects/anymail/badge/?version=v9.1
-       :target: https://anymail.dev/en/v9.1/
+.. image:: https://readthedocs.org/projects/anymail/badge/?version=v9.2
+       :target: https://anymail.dev/en/v9.2/
        :alt:    documentation build status on ReadTheDocs
 
 **Resources**
 
-* Full documentation: https://anymail.dev/en/v9.1/
-* Help and troubleshooting: https://anymail.dev/en/v9.1/help/
+* Full documentation: https://anymail.dev/en/v9.2/
+* Help and troubleshooting: https://anymail.dev/en/v9.2/help/
 * Package on PyPI: https://pypi.org/project/django-anymail/
 * Project on Github: https://github.com/anymail/django-anymail
-* Changelog: https://anymail.dev/en/v9.1/changelog/
+* Changelog: https://anymail.dev/en/v9.2/changelog/
 
 
 Anymail 1-2-3
 -------------
 
 .. _quickstart:
 
@@ -173,15 +174,15 @@
             "MAILGUN_SENDER_DOMAIN": 'mg.example.com',  # your Mailgun domain, if needed
         }
         EMAIL_BACKEND = "anymail.backends.mailgun.EmailBackend"  # or sendgrid.EmailBackend, or...
         DEFAULT_FROM_EMAIL = "you@example.com"  # if you don't already have this in settings
         SERVER_EMAIL = "your-server@example.com"  # ditto (default from-email for Django errors)
 
 
-3. Now the regular `Django email functions <https://docs.djangoproject.com/en/v9.1/topics/email/>`_
+3. Now the regular `Django email functions <https://docs.djangoproject.com/en/v9.2/topics/email/>`_
    will send through your chosen ESP:
 
    .. code-block:: python
 
         from django.core.mail import send_mail
 
         send_mail("It works!", "This will get sent through Mailgun",
@@ -217,10 +218,10 @@
 
         # Send it:
         msg.send()
 
 .. END quickstart
 
 
-See the `full documentation <https://anymail.dev/en/v9.1/>`_
+See the `full documentation <https://anymail.dev/en/v9.2/>`_
 for more features and options, including receiving messages and tracking
 sent message status.
```

### Comparing `django-anymail-9.1/django_anymail.egg-info/SOURCES.txt` & `django-anymail-9.2/django_anymail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-anymail-9.1/setup.py` & `django-anymail-9.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 # Additional requirements for development/build/release
 requirements_dev = [
     "pre-commit",
     "sphinx",
     "sphinx-rtd-theme",
     "tox",
     "twine",
+    "virtualenv<20.22.0",  # tox dependency, pinned for Python 3.6 tox testenv
     "wheel",
 ]
 
 # Additional requirements for running tests
 requirements_test = []
 
 
@@ -111,15 +112,15 @@
         "Intended Audience :: Developers",
         "Framework :: Django",
         "Framework :: Django :: 3.0",
         "Framework :: Django :: 3.1",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
-        # not yet registered: "Framework :: Django :: 4.2",
+        "Framework :: Django :: 4.2",
         "Environment :: Web Environment",
     ],
     long_description=long_description,
     long_description_content_type="text/x-rst",
     project_urls=OrderedDict(
         [
             ("Documentation", "https://anymail.dev/en/%s/" % release_tag),
```

