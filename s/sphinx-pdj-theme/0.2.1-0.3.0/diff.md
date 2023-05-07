# Comparing `tmp/sphinx_pdj_theme-0.2.1.tar.gz` & `tmp/sphinx-pdj-theme-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sphinx_pdj_theme-0.2.1.tar", last modified: Wed Jul  1 20:27:44 2020, max compression
+gzip compressed data, was "sphinx-pdj-theme-0.3.0.tar", last modified: Sun May  7 17:12:25 2023, max compression
```

## Comparing `sphinx_pdj_theme-0.2.1.tar` & `sphinx-pdj-theme-0.3.0.tar`

### file list

```diff
@@ -1,40 +1,46 @@
-drwxrwxr-x   0 juca      (1000) juca      (1000)        0 2020-07-01 20:27:44.202280 sphinx_pdj_theme-0.2.1/
--rw-rw-r--   0 juca      (1000) juca      (1000)       75 2020-06-27 23:26:42.000000 sphinx_pdj_theme-0.2.1/MANIFEST.in
--rw-rw-r--   0 juca      (1000) juca      (1000)     1533 2020-07-01 20:27:44.202280 sphinx_pdj_theme-0.2.1/PKG-INFO
--rw-rw-r--   0 juca      (1000) juca      (1000)      435 2020-06-27 23:26:42.000000 sphinx_pdj_theme-0.2.1/README.rst
--rw-rw-r--   0 juca      (1000) juca      (1000)       38 2020-07-01 20:27:44.202280 sphinx_pdj_theme-0.2.1/setup.cfg
--rw-rw-r--   0 juca      (1000) juca      (1000)     1905 2020-06-27 23:26:42.000000 sphinx_pdj_theme-0.2.1/setup.py
-drwxrwxr-x   0 juca      (1000) juca      (1000)        0 2020-07-01 20:27:44.198279 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/
--rw-rw-r--   0 juca      (1000) juca      (1000)      261 2020-07-01 20:26:45.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/__init__.py
-drwxrwxr-x   0 juca      (1000) juca      (1000)        0 2020-07-01 20:27:44.198279 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/__pycache__/
--rw-rw-r--   0 juca      (1000) juca      (1000)      534 2020-06-27 23:51:54.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 juca      (1000) juca      (1000)     1035 2020-06-27 23:26:42.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/breadcrumbs.html
--rw-rw-r--   0 juca      (1000) juca      (1000)     1327 2020-06-27 23:26:42.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/footer.html
--rw-rw-r--   0 juca      (1000) juca      (1000)     6906 2020-06-28 00:57:52.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/layout.html
--rw-rw-r--   0 juca      (1000) juca      (1000)     7341 2020-06-27 23:26:42.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/layout_old.html
--rw-rw-r--   0 juca      (1000) juca      (1000)     1614 2020-06-28 00:08:34.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/search.html
--rw-rw-r--   0 juca      (1000) juca      (1000)      354 2020-06-27 23:26:42.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/searchbox.html
-drwxrwxr-x   0 juca      (1000) juca      (1000)        0 2020-07-01 20:27:44.198279 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/
-drwxrwxr-x   0 juca      (1000) juca      (1000)        0 2020-07-01 20:27:44.198279 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/css/
--rw-rw-r--   0 juca      (1000) juca      (1000)     3403 2020-06-27 23:26:42.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/css/badge_only.css
--rw-rw-r--   0 juca      (1000) juca      (1000)     5273 2020-07-01 20:26:31.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/css/darker.css
--rw-rw-r--   0 juca      (1000) juca      (1000)    10221 2020-06-28 03:58:01.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/css/pdj.css
--rw-rw-r--   0 juca      (1000) juca      (1000)    90920 2020-06-27 23:26:42.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/css/theme.css
-drwxrwxr-x   0 juca      (1000) juca      (1000)        0 2020-07-01 20:27:44.198279 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/fonts/
--rw-rw-r--   0 juca      (1000) juca      (1000)    38205 2020-06-27 23:26:42.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/fonts/fontawesome-webfont.eot
--rw-rw-r--   0 juca      (1000) juca      (1000)   202148 2020-06-27 23:26:42.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/fonts/fontawesome-webfont.svg
--rw-rw-r--   0 juca      (1000) juca      (1000)    80652 2020-06-27 23:26:42.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/fonts/fontawesome-webfont.ttf
--rw-rw-r--   0 juca      (1000) juca      (1000)    44432 2020-06-27 23:26:42.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/fonts/fontawesome-webfont.woff
-drwxrwxr-x   0 juca      (1000) juca      (1000)        0 2020-07-01 20:27:44.198279 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/img/
--rw-rw-r--   0 juca      (1000) juca      (1000)     1127 2020-06-27 23:26:42.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/img/porao-branco.png
-drwxrwxr-x   0 juca      (1000) juca      (1000)        0 2020-07-01 20:27:44.198279 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/js/
--rw-rw-r--   0 juca      (1000) juca      (1000)      351 2020-06-27 23:26:42.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/js/pdj.js
--rw-rw-r--   0 juca      (1000) juca      (1000)     1675 2020-06-27 23:26:42.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/js/theme.js
--rw-rw-r--   0 juca      (1000) juca      (1000)      138 2020-06-28 00:07:29.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/theme.conf
--rw-rw-r--   0 juca      (1000) juca      (1000)     1219 2020-06-27 23:26:42.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/versions.html
-drwxrwxr-x   0 juca      (1000) juca      (1000)        0 2020-07-01 20:27:44.198279 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme.egg-info/
--rw-rw-r--   0 juca      (1000) juca      (1000)     1533 2020-07-01 20:27:44.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme.egg-info/PKG-INFO
--rw-rw-r--   0 juca      (1000) juca      (1000)     1049 2020-07-01 20:27:44.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme.egg-info/SOURCES.txt
--rw-rw-r--   0 juca      (1000) juca      (1000)        1 2020-07-01 20:27:44.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme.egg-info/dependency_links.txt
--rw-rw-r--   0 juca      (1000) juca      (1000)       58 2020-07-01 20:27:44.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme.egg-info/entry_points.txt
--rw-rw-r--   0 juca      (1000) juca      (1000)       17 2020-07-01 20:27:44.000000 sphinx_pdj_theme-0.2.1/sphinx_pdj_theme.egg-info/top_level.txt
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-07 17:12:25.939728 sphinx-pdj-theme-0.3.0/
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1079 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/LICENSE
+-rw-rw-r--   0 juca      (1001) juca      (1001)       75 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/MANIFEST.in
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1122 2023-05-07 17:12:25.939728 sphinx-pdj-theme-0.3.0/PKG-INFO
+-rw-rw-r--   0 juca      (1001) juca      (1001)      640 2023-05-07 16:20:52.000000 sphinx-pdj-theme-0.3.0/README.md
+-rw-rw-r--   0 juca      (1001) juca      (1001)      435 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/README.rst
+-rw-rw-r--   0 juca      (1001) juca      (1001)      672 2023-05-07 17:11:51.000000 sphinx-pdj-theme-0.3.0/pyproject.toml
+-rw-rw-r--   0 juca      (1001) juca      (1001)       38 2023-05-07 17:12:25.939728 sphinx-pdj-theme-0.3.0/setup.cfg
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-07 17:12:25.935728 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/
+-rw-rw-r--   0 juca      (1001) juca      (1001)      242 2023-05-07 17:08:32.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/__init__.py
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-07 17:12:25.935728 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/__pycache__/
+-rw-rw-r--   0 juca      (1001) juca      (1001)      837 2023-05-07 05:57:19.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/__pycache__/__init__.cpython-311.pyc
+-rwxrwxrwx   0 juca      (1001) juca      (1001)      534 2020-06-27 23:51:54.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/__pycache__/__init__.cpython-37.pyc
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1035 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/breadcrumbs.html
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1328 2023-05-07 16:20:52.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/footer.html
+-rw-rw-r--   0 juca      (1001) juca      (1001)     7198 2023-05-07 16:20:52.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/layout.html
+-rw-rw-r--   0 juca      (1001) juca      (1001)     7341 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/layout_old.html
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1614 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/search.html
+-rw-rw-r--   0 juca      (1001) juca      (1001)      354 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/searchbox.html
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-07 17:12:25.931728 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-07 17:12:25.935728 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/css/
+-rw-rw-r--   0 juca      (1001) juca      (1001)     3403 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/css/badge_only.css
+-rw-rw-r--   0 juca      (1001) juca      (1001)     5164 2023-05-07 16:27:25.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/css/darker.css
+-rw-rw-r--   0 juca      (1001) juca      (1001)    19589 2023-05-07 16:20:52.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/css/img.css
+-rw-rw-r--   0 juca      (1001) juca      (1001)    10251 2023-05-07 16:20:52.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/css/pdj.css
+-rw-rw-r--   0 juca      (1001) juca      (1001)    90920 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/css/theme.css
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-07 17:12:25.939728 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/fonts/
+-rw-rw-r--   0 juca      (1001) juca      (1001)    38205 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/fonts/fontawesome-webfont.eot
+-rw-rw-r--   0 juca      (1001) juca      (1001)   202148 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/fonts/fontawesome-webfont.svg
+-rw-rw-r--   0 juca      (1001) juca      (1001)    80652 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/fonts/fontawesome-webfont.ttf
+-rw-rw-r--   0 juca      (1001) juca      (1001)    44432 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/fonts/fontawesome-webfont.woff
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-07 17:12:25.939728 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/img/
+-rw-rw-r--   0 juca      (1001) juca      (1001)     3260 2023-05-07 16:20:52.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/img/moon.svg
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1127 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/img/porao-branco.png
+-rw-rw-r--   0 juca      (1001) juca      (1001)    18468 2023-05-07 16:20:52.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/img/sun.svg
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-07 17:12:25.939728 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/js/
+-rw-rw-r--   0 juca      (1001) juca      (1001)      351 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/js/pdj.js
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1675 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/js/theme.js
+-rw-rw-r--   0 juca      (1001) juca      (1001)      138 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/theme.conf
+-rw-rw-r--   0 juca      (1001) juca      (1001)     1219 2023-05-07 05:46:47.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/versions.html
+drwxrwxr-x   0 juca      (1001) juca      (1001)        0 2023-05-07 17:12:25.935728 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme.egg-info/
+-rwxrwxrwx   0 juca      (1001) juca      (1001)     1122 2023-05-07 17:12:25.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme.egg-info/PKG-INFO
+-rwxrwxrwx   0 juca      (1001) juca      (1001)     1236 2023-05-07 17:12:25.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme.egg-info/SOURCES.txt
+-rwxrwxrwx   0 juca      (1001) juca      (1001)        1 2023-05-07 17:12:25.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme.egg-info/dependency_links.txt
+-rw-rw-r--   0 juca      (1001) juca      (1001)       57 2023-05-07 17:12:25.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme.egg-info/entry_points.txt
+-rwxrwxrwx   0 juca      (1001) juca      (1001)       17 2023-05-07 17:12:25.000000 sphinx-pdj-theme-0.3.0/sphinx_pdj_theme.egg-info/top_level.txt
```

### Comparing `sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/__pycache__/__init__.cpython-37.pyc` & `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/breadcrumbs.html` & `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/footer.html` & `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/footer.html`

 * *Files 8% similar despite different names*

```diff
@@ -24,10 +24,10 @@
 
     {%- if last_updated %}
       {% trans last_updated=last_updated|e %}Last updated on {{ last_updated }}.{% endtrans %}
     {%- endif %}
     </p>
   </div>
 
-  {% trans %}Built with <a href="http://sphinx-doc.org/">Sphinx</a> using a <a href="https://github.com/jucacrispim/sphinx_pdj_theme">theme</a> provided by <a href="http://poraodojuca.net">Porão do Juca</a>{% endtrans %}.
+  {% trans %}Built with <a href="http://sphinx-doc.org/">Sphinx</a> using a <a href="https://github.com/jucacrispim/sphinx_pdj_theme">theme</a> provided by <a href="https://poraodojuca.dev">Porão do Juca</a>{% endtrans %}.
 
 </footer>
```

### Comparing `sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/layout.html` & `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/layout.html`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.1//EN" "http://www.w3.org/TR/xhtml11/DTD/xhtml11.dtd">
 <html xml:lang="{{ LANGUAGE_CODE }}" lang="{{ LANGUAGE_CODE }}" version="-//W3C//DTD XHTML 1.1//EN" xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
+    <meta name="theme-color" content="">
 
   {% block htmltitle %}
   <title>{{ title|striptags|e }}{{ titlesuffix }}</title>
   {% endblock %}
 
   {# OPENSEARCH #}
   {%- if not embedded %}
@@ -24,29 +25,25 @@
       <link rel="search" type="application/opensearchdescription+xml" title="{% trans docstitle=docstitle|e %}Search within {{ docstitle }}{% endtrans %}" href="{{ pathto('_static/opensearch.xml', 1) }}"/>
     {% endif %}
 
   {% endif %}
 
     <link href='https://fonts.googleapis.com/css?family=Lato:400,700,400italic,700italic|Roboto+Slab:400,700|Inconsolata:400,700' rel='stylesheet' type='text/css'/>
 
-  {%- if not READTHEDOCS %}
-    <link rel="stylesheet" href="{{ pathto('_static/' + style, 1) }}" type="text/css" />
-  {%- endif %}
 
+  <link rel="stylesheet" href="{{ pathto('_static/css/img.css', 1) }}" type="text/css"/>
   {% for cssfile in css_files %}
     <link rel="stylesheet" href="{{ pathto(cssfile, 1) }}" type="text/css" />
   {% endfor %}
 
   {% for cssfile in extra_css_files %}
     <link rel="stylesheet" href="{{ pathto(cssfile, 1) }}" type="text/css" />
   {% endfor %}
 
-  {% if theme_style == "darker" %}
-    <link rel="stylesheet" href="{{ pathto('_static/css/darker.css', 1) }}" type="text/css" />
-  {% endif %}
+  <link rel="stylesheet" href="{{ pathto('_static/css/darker.css', 1) }}" type="text/css" media="(prefers-color-scheme: dark)"/>
 
   {%- block linktags %}
     {%- if hasdoc('about') %}
         <link rel="author" title="{{ _('About these documents') }}"
               href="{{ pathto('about') }}"/>
     {%- endif %}
     {%- if hasdoc('genindex') %}
@@ -81,15 +78,15 @@
 
     {%- block link %}{%- endblock %}
     <!-- Add jQuery library -->
 
     {%- block script %}
     <script type="text/javascript" src="http://code.jquery.com/jquery-latest.min.js"></script>
     <script src="https://cdnjs.cloudflare.com/ajax/libs/modernizr/2.6.2/modernizr.min.js"></script>
-
+    <script type="module" src="https://googlechromelabs.github.io/dark-mode-toggle/src/dark-mode-toggle.mjs"></script>
     {%- endblock %}
 
   </head>
 
   <body class="wy-body-for-nav" role="document">
 
   <div class="wy-grid-for-nav">
@@ -150,18 +147,22 @@
 
 	    <!-- 	<a href="_sources/index.txt" rel="nofollow"> View page source</a> -->
 
 	    <!--   </li> -->
 	    <!-- </ul> -->
 	    <!-- <hr/> -->
 	  </div>
-
           <div role="main" class="{%- if flatpage %} flatpage {%- endif %}">
 
 	    <div id="content" class="hfeed entry-container hentry">
+      	<div id="dark-mode-toggle-container">
+	  <dark-mode-toggle appearance="toggle" dark="switch to light mode" light="switch to dark mode" permanent="true">
+	  </dark-mode-toggle>
+	</div>
+
               {%- block body %}
 	      {%- endblock %}
 	    </div>
             {% include "footer.html" %}
 	</div>
 	</div>
 	  {% if not embedded %}
```

### Comparing `sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/layout_old.html` & `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/layout_old.html`

 * *Files identical despite different names*

### Comparing `sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/search.html` & `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/search.html`

 * *Files identical despite different names*

### Comparing `sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/css/badge_only.css` & `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/css/darker.css` & `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/css/darker.css`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 .wy-side-nav-search,
 .fundo-claro,
 .wy-menu-vertical li.current,
 .rst-content dl:not(.docutils) dt,
 code, .rst-content tt,
 .wy-side-nav-search > a:hover, .wy-side-nav-search .wy-dropdown > a:hover,
 .wy-nav-content{
-    background-color: rgb(24, 26, 27) !important;
+    background-color: rgb(24, 26, 27);
 }
 
 h2 a, h2 a:visited, h2 a:hover {
     color: rgb(209, 206, 199);
 }
 
 body {
@@ -51,24 +51,18 @@
 }
 
 @media screen and (min-width: 768px) {
 .wy-nav-side{
     width: 224px;
 }
 .wy-nav-content-wrap{
-    margin-left: 200px;
     background:rgb(24, 26, 27);
 }
 }
 
-.wy-nav-content-wrap{
-    margin-left: 200px;
-    background: #343131;
-}
-
 .hentry {
      border-bottom: 2px solid rgb(24, 26, 27);
 }
 
 .wy-alert.wy-alert-danger .wy-alert-title, .rst-content .wy-alert-danger.note .wy-alert-title, .rst-content .wy-alert-danger.attention .wy-alert-title, .rst-content .wy-alert-danger.caution .wy-alert-title, .rst-content .danger .wy-alert-title, .rst-content .error .wy-alert-title, .rst-content .wy-alert-danger.hint .wy-alert-title, .rst-content .wy-alert-danger.important .wy-alert-title, .rst-content .wy-alert-danger.tip .wy-alert-title, .rst-content .wy-alert-danger.warning .wy-alert-title, .rst-content .wy-alert-danger.seealso .wy-alert-title, .rst-content .wy-alert-danger.admonition-todo .wy-alert-title, .wy-alert.wy-alert-danger .rst-content .admonition-title, .rst-content .wy-alert.wy-alert-danger .admonition-title, .rst-content .wy-alert-danger.note .admonition-title, .rst-content .wy-alert-danger.attention .admonition-title, .rst-content .wy-alert-danger.caution .admonition-title, .rst-content .danger .admonition-title, .rst-content .error .admonition-title, .rst-content .wy-alert-danger.hint .admonition-title, .rst-content .wy-alert-danger.important .admonition-title, .rst-content .wy-alert-danger.tip .admonition-title, .rst-content .wy-alert-danger.warning .admonition-title, .rst-content .wy-alert-danger.seealso .admonition-title, .rst-content .wy-alert-danger.admonition-todo .admonition-title {
 	background: #db655a;
 }
```

### Comparing `sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/css/pdj.css` & `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/css/pdj.css`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 @import url("theme.css");
 
+:root {
+    --dark-mode-toggle-icon-size: 1.5rem;
+}
+
 .wy-side-nav-search{
     background-color: #595C5E;
+    margin-bottom: 0;
 }
 
 .wy-side-nav-search input[type=text] {
     border-color: #595C5E;
 }
 
 @media screen and (min-width: 768px) {
@@ -13,19 +18,14 @@
     width: 224px;
 }
 .wy-nav-content-wrap{
     margin-left: 200px;
     background: #343131;
 }
 }
-@media screen and (max-width: 768px) {
-    .wy-nav-content{
-	background-color: #343131;
-    }
-}
 
 .wy-nav-top{
     background-color: #595C5E;
 }
 .wy-nav-content{
     padding-top: 1%;
     max-width: 100%;
@@ -488,7 +488,11 @@
 .highlight-cfg .o,
 .highlight-cfg .nv,
 .highlight-cfg .gp,
 .highlight-cfg .s {
     color: #57de4e;
     font-weight: normal;
 }
+
+#dark-mode-toggle-container {
+    float: right;
+}
```

### Comparing `sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/css/theme.css` & `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/css/theme.css`

 * *Files identical despite different names*

### Comparing `sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/fonts/fontawesome-webfont.eot` & `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/fonts/fontawesome-webfont.svg` & `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/fonts/fontawesome-webfont.ttf` & `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/fonts/fontawesome-webfont.woff` & `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/img/porao-branco.png` & `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/img/porao-branco.png`

 * *Files identical despite different names*

### Comparing `sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/static/js/theme.js` & `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/static/js/theme.js`

 * *Files identical despite different names*

### Comparing `sphinx_pdj_theme-0.2.1/sphinx_pdj_theme/versions.html` & `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme/versions.html`

 * *Files identical despite different names*

### Comparing `sphinx_pdj_theme-0.2.1/sphinx_pdj_theme.egg-info/SOURCES.txt` & `sphinx-pdj-theme-0.3.0/sphinx_pdj_theme.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,35 @@
+LICENSE
 MANIFEST.in
+README.md
 README.rst
-setup.py
+pyproject.toml
 sphinx_pdj_theme/__init__.py
 sphinx_pdj_theme/breadcrumbs.html
 sphinx_pdj_theme/footer.html
 sphinx_pdj_theme/layout.html
 sphinx_pdj_theme/layout_old.html
 sphinx_pdj_theme/search.html
 sphinx_pdj_theme/searchbox.html
 sphinx_pdj_theme/theme.conf
 sphinx_pdj_theme/versions.html
 sphinx_pdj_theme.egg-info/PKG-INFO
 sphinx_pdj_theme.egg-info/SOURCES.txt
 sphinx_pdj_theme.egg-info/dependency_links.txt
 sphinx_pdj_theme.egg-info/entry_points.txt
 sphinx_pdj_theme.egg-info/top_level.txt
+sphinx_pdj_theme/__pycache__/__init__.cpython-311.pyc
 sphinx_pdj_theme/__pycache__/__init__.cpython-37.pyc
 sphinx_pdj_theme/static/css/badge_only.css
 sphinx_pdj_theme/static/css/darker.css
+sphinx_pdj_theme/static/css/img.css
 sphinx_pdj_theme/static/css/pdj.css
 sphinx_pdj_theme/static/css/theme.css
 sphinx_pdj_theme/static/fonts/fontawesome-webfont.eot
 sphinx_pdj_theme/static/fonts/fontawesome-webfont.svg
 sphinx_pdj_theme/static/fonts/fontawesome-webfont.ttf
 sphinx_pdj_theme/static/fonts/fontawesome-webfont.woff
+sphinx_pdj_theme/static/img/moon.svg
 sphinx_pdj_theme/static/img/porao-branco.png
+sphinx_pdj_theme/static/img/sun.svg
 sphinx_pdj_theme/static/js/pdj.js
 sphinx_pdj_theme/static/js/theme.js
```

