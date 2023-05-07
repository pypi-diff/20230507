# Comparing `tmp/smartjs-0.0.6.tar.gz` & `tmp/smartjs-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartjs-0.0.6.tar", max compression
+gzip compressed data, was "smartjs-0.0.7.tar", max compression
```

## Comparing `smartjs-0.0.6.tar` & `smartjs-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      302 2023-05-06 00:37:59.092796 smartjs-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      183 2023-05-05 14:06:40.683599 smartjs-0.0.6/smartjs/__init__.py
--rw-r--r--   0        0        0    13325 2023-05-06 00:12:29.975202 smartjs-0.0.6/smartjs/base.py
--rw-r--r--   0        0        0     2223 2023-05-05 22:02:36.952511 smartjs-0.0.6/smartjs/constants.py
--rw-r--r--   0        0        0     4479 2023-05-04 15:42:17.533986 smartjs-0.0.6/smartjs/elements.py
--rw-r--r--   0        0        0     5801 2023-05-04 01:36:29.647942 smartjs-0.0.6/smartjs/functions.py
--rw-r--r--   0        0        0    13961 2023-05-06 00:12:29.971024 smartjs-0.0.6/smartjs/javascript.py
--rw-r--r--   0        0        0     1660 2023-05-05 21:29:35.092805 smartjs-0.0.6/smartjs/page.py
--rw-r--r--   0        0        0      807 2023-05-05 22:30:55.828371 smartjs-0.0.6/smartjs/path.py
--rw-r--r--   0        0        0     1598 2023-05-05 03:48:44.383638 smartjs-0.0.6/smartjs/style.py
--rw-r--r--   0        0        0      584 2023-05-06 00:38:02.999421 smartjs-0.0.6/setup.py
--rw-r--r--   0        0        0      333 2023-05-06 00:38:02.999645 smartjs-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      302 2023-05-07 01:38:04.683465 smartjs-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-05-05 14:06:40.683599 smartjs-0.0.7/smartjs/__init__.py
+-rw-r--r--   0        0        0    13079 2023-05-06 23:09:29.043999 smartjs-0.0.7/smartjs/base.py
+-rw-r--r--   0        0        0     2223 2023-05-05 22:02:36.952511 smartjs-0.0.7/smartjs/constants.py
+-rw-r--r--   0        0        0     4576 2023-05-06 23:09:29.046930 smartjs-0.0.7/smartjs/elements.py
+-rw-r--r--   0        0        0     5805 2023-05-06 22:41:19.600790 smartjs-0.0.7/smartjs/functions.py
+-rw-r--r--   0        0        0    11888 2023-05-06 23:09:29.039937 smartjs-0.0.7/smartjs/javascript.py
+-rw-r--r--   0        0        0     1660 2023-05-05 21:29:35.092805 smartjs-0.0.7/smartjs/page.py
+-rw-r--r--   0        0        0      994 2023-05-07 01:38:04.688449 smartjs-0.0.7/smartjs/path.py
+-rw-r--r--   0        0        0     1400 2023-05-06 22:39:05.716015 smartjs-0.0.7/smartjs/style.py
+-rw-r--r--   0        0        0      584 2023-05-07 01:38:12.061426 smartjs-0.0.7/setup.py
+-rw-r--r--   0        0        0      333 2023-05-07 01:38:12.061650 smartjs-0.0.7/PKG-INFO
```

### Comparing `smartjs-0.0.6/smartjs/base.py` & `smartjs-0.0.7/smartjs/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -290,15 +290,24 @@
         super().__init__(join(args))
         
 
 class BaseElement(UserString):
     TAG: Tag = None
     KLASS: str = None
     def __init__(self, *args, **kwargs):
+        tag = list_of_type(args, Tag) or kwargs.pop('tag', None)
+        if tag:
+            if isinstance(tag, str):
+                tag = Tag(tag)
+            elif isinstance(tag, list):
+                tag = tag[0]
+        self.tag = tag
         self.klass = SmartList(list_of_type(args, Klass), kwargs.pop('klass', None))
+        if self.KLASS:
+            self.klass =[*self.KLASS.split(), *self.klass]
         self.style = SmartList(list_of_type(args, StyleItem), kwargs.pop('style', None))
         self.elements = SmartList(list_of_type(args, (BaseElement, Text)), kwargs.pop('elements', []))
         self.after = SmartList(kwargs.pop('after', []))
         self.before = SmartList(kwargs.pop('before', []))
         self.list_kwargs = SmartList(list_of_type(args, Kwarg), kwargs.pop('kwargs', None))
         self.args = SmartList(list_of_type(args, Arg), kwargs.pop('args', None))
         self.script: SmartList[BaseScript, str] = SmartList(*kwargs.pop('script', list()))
@@ -323,16 +332,14 @@
     def post_init_elements(self) -> list['BaseElement', str]:
         return []
         
     def render_kwargs(self):
         return f'{join(set_filtered(self.list_kwargs))} {repr_dict(self.dict_kwargs)}'
     
     def render_klass(self):
-        if self.KLASS:
-            self.klass.extend(self.KLASS.split())
         return f'class="{join(set_filtered(self.klass))}"' if list_filtered(self.klass) else ''
     
     def render_style(self):
         return f'style="{join(set_filtered(self.style), sep="; ")}"' if list_filtered(self.style) else ''
     
     def render_after(self):
         return join(self.after) if list_filtered(self.after) else ''
@@ -348,25 +355,25 @@
     
     def render_script(self):
         if self.script:
             return f'<script> {join(self.script, "; ")} </script>'
         return ''
     
     @property
-    def tag(self):
-        return self.TAG or Tag(type(self).__name__.lower())
+    def computed_tag(self):
+        return self.tag or self.TAG or Tag(type(self).__name__.lower())
     
     @property
     def config(self):
         return join([self.render_args(), self.render_klass(), self.render_kwargs(), self.render_style()])
     
     def render(self):
-        if self.tag.value in EMPTY_TAGS:
-            return f'{self.render_before()}<{self.tag} {self.config}>{self.render_elements()}{join(self.render_after())}{self.render_script()}'
-        return f'{self.render_before()}<{self.tag} {self.config}>{self.render_elements()}</{self.tag}>{self.render_after()}{self.render_script()}'
+        if self.computed_tag.value in EMPTY_TAGS:
+            return f'{self.render_before()}<{self.computed_tag} {self.config}>{self.render_elements()}{join(self.render_after())}{self.render_script()}'
+        return f'{self.render_before()}<{self.computed_tag} {self.config}>{self.render_elements()}</{self.computed_tag}>{self.render_after()}{self.render_script()}'
         
         
 class SmartList(UserList):
     def __init__(self, *args):
         self.data = list()
         self.include(*args)
         super().__init__(self.data)
@@ -394,28 +401,14 @@
         for item in args:
             if isinstance(item, (tuple, list, set)):
                 self.include(*item)
             else:
                 self.data.append(item)
         super().__init__(set(self.data))
         
-        
-        
 
-
-if __name__ == '__main__':
-    class Container(BaseElement):
-        TAG = Tag('div')
-        KLASS = 'container'
-        
-    
-    d = Container(Kwarg('data-model', 'person'), Kwarg('id="person"'), *[StyleItem(item) for item in ['font-size: 1rem', 'color: red', 'color: red']])
-    print(Container(d, args='required', klass='d-flex', style=['background: black', 'color: yellow'], elements=d))
     
-    print(vars(d))
     
-    s = BaseStyle.head_style(['--black: black'], [BaseStyle.style_group('html', 'body', font_size='10px')])
-    print(s)
```

### Comparing `smartjs-0.0.6/smartjs/constants.py` & `smartjs-0.0.7/smartjs/constants.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.6/smartjs/functions.py` & `smartjs-0.0.7/smartjs/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 
 
 def today_isoformat() -> str:
     return today().isoformat()
 
 
 def slug(value: str) -> str:
-    return normalize(join([item for item in re.split(r'([A-Z][a-z]+)(?=[A-Z])|\s', value) if item], sep="_")).lower()
+    return normalize(join([item for item in re.split(r'([A-Z|a-z][a-z]+)(?=[A-Z])|\s', value) if item], sep="_")).lower()
 
 
 def camel_case(value: str) -> str:
     items = [*re.split(r'[-_]', slug(value))]
     return ''.join([items[0], *[i.title() for i in items[1:]]])
```

### Comparing `smartjs-0.0.6/smartjs/javascript.py` & `smartjs-0.0.7/smartjs/javascript.py`

 * *Files 16% similar despite different names*

```diff
@@ -314,34 +314,8 @@
         return repr_dict(dict_filtered(self.kwargs), sep=" ")
     
     def render_args(self):
         return join(SmartList(*self.args), '; ')
 
 
     
-
-
-if __name__ == '__main__':
-    # person_key = ScriptFormField('person_key', 'input:text', 'required', label='Pessoa', hx_get='/options/person', hx_trigger='load', hx_target='#person-list', list='person-list')
-    # bdate = ScriptFormField('bdate', 'input:date', 'required', label='Nascimento')
-    # form = ScriptForm('person_new', '/form/new/person', form_fields=[person_key, bdate])
-    # script = Script(form, Script.append_to('main', form.form_name))
-    # print(script)
-    t = ScriptById('my_title').tag('h1').inner_html('Título do Formulário')
-    x = ScriptById('my_name').tag('input').class_name('form-control').true('required').attribute('placeholder', 'my_name').style('backgroundColor', 'red').id_as_name()
-    l = ScriptById('my_name__label').tag('label').class_name('form-label').attribute('for', x.name).inner_html('meu nome')
-    c = ScriptById('my_name__container').tag('div').class_name('form-floating').append_instance(x).append_instance(l)
-    n = ScriptById('my_name2').tag('input').class_name('form-control').true('required').attribute('placeholder', 'my_name').style('backgroundColor', 'green').id_as_name()
-    nl = ScriptById('my_name2__label').tag('label').class_name('form-label').attribute('for', n.name).inner_html('meu nome')
-    nc = ScriptById('my_name2__container').tag('div').class_name('form-floating').append_instance(n).append_instance(nl)
-    i3 = ScriptById('check').tag('input').attribute('type', 'checkbox').id_as_name().class_name('form-check-input')
-    l3 = ScriptById('check__label').tag('label').attribute('for', i3.id).class_name('form-check-label').inner_html('ativo?')
-    c3 = ScriptById('check__container').tag('div').class_name('form-check').append_instance(i3).append_instance(l3)
-    f = ScriptById('form').tag('form').class_name('form-control').style('marginTop', '200px').append_instance(t).append_instance(c).append_instance(nc).append_instance(c3).append_to('main')
-    d = Script.for_loop('formField', 'form.elements', ['console.log(formField)'])
-
-    print(ScriptJoin(*f.args, str(d)))
-    
-    print()
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `smartjs-0.0.6/smartjs/page.py` & `smartjs-0.0.7/smartjs/page.py`

 * *Files identical despite different names*

### Comparing `smartjs-0.0.6/smartjs/style.py` & `smartjs-0.0.7/smartjs/style.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,13 +33,7 @@
 
 class Style(BaseStyle):
     def __init__(self, *args: Union[tuple[StyleRootItem, StyleGroup], StyleRootItem, StyleGroup]):
         self.root = SmartList(list_of_type(args, StyleRootItem))
         self.declarations = SmartList(list_of_type(args, StyleGroup))
         super().__init__(f'<style> {{{f"{StyleRoot(*self.root)} {join(self.declarations)}"}}} </style>')
 
-
-
-if __name__ == '__main__':
-    # print(Style(StyleRootItem('black', 'black'), StyleGroup('body', 'html', StyleItem('margin: 0'))))
-    ...
-    print(StyleRoot('--black: black', '--white: white'))
```

### Comparing `smartjs-0.0.6/setup.py` & `smartjs-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Unidecode>=1.3.6,<2.0.0']
 
 setup_kwargs = {
     'name': 'smartjs',
-    'version': '0.0.6',
+    'version': '0.0.7',
     'description': '',
     'long_description': None,
     'author': 'Daniel Victor',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

